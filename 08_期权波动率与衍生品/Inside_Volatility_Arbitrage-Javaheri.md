

<!-- === Source: MinerU_markdown_Inside_Volatility_Arbitrage-Javaheri_1_2122707067558010897.md (Page 1) === -->

# INSIDE VOLATILITY ARBITRAGE

The Secrets of Skewness 

ALIREZAJAVAHERI 

## Inside Volatility Arbitrage

Founded in 1807, John Wiley & Sons is the oldest independent publishing company in the United States. With offices in North America, Europe, Australia, and Asia, Wiley is globally committed to developing and marketing print and electronic products and services for our customers’ professional and personal knowledge and understanding. 

The Wiley Finance series contains books written specifically for finance and investment professionals as well as sophisticated individual investors and their financial advisors. Book topics range from portfolio management to e-commerce, risk management, financial engineering, valuation and financial instrument analysis, as well as much more. 

For a list of available titles, visit our Web site at www.WileyFinance.com. 

# Inside Volatility Arbitrage

## The Secrets of Skewness

## ALIREZA JAVAHERI

Copyright © 2005 by Alireza Javaheri. All rights reserved Published by John Wiley & Sons, Inc., Hoboken, New Jersey Published simultaneously in Canada 

No part of this publication may be reproduced, stored in a retrieval system, or transmitted in any form or by any means, electronic, mechanical, photocopying, recording, scanning, or otherwise, except as permitted under Section 107 or 108 of the 1976 United States Copyright Act, without either the prior written permission of the Publisher, or authorization through payment of the appropriate per-copy fee to the Copyright Clearance Center, 222 Rosewood Drive, Danvers, MA 01923, (978) 750-8400, fax (978) 750-4470, or on the web at www.copyright.com. Requests to the Publisher for permission should be addressed to the Permissions Department, John Wiley & Sons, Inc., 111 River Street, Hoboken, NJ 07030, (201) 748-6011, fax (201) 748-6008, or online at http://www.wiley.com/go/permissions. 

Limit of Liability/Disclaimer of Warranty: While the publisher and the author have used their best efforts in preparing this book, they make no representations or warranties with respect to the accuracy or completeness of the contents of this book and specifically disclaim any implied warranties of merchantability or fitness for a particular purpose. No warranty may be created or extended by sales representatives or written sales materials. The advice and strategies contained herein may not be suitable for your situation. You should consult with a professional where appropriate. Neither the publisher nor the author shall be liable for any loss of profit or any other commercial damages, including but not limited to special, incidental, consequential, or other damages. 

For general information about our other products and services, please contact our Customer Care Department within the United States at (800) 762-2974, outside the United States at (317) 572-3993 or fax (317) 572-4002. 

Wiley also publishes its books in a variety of electronic formats. Some content that appears in print may not be available in electronic books. For more information about Wiley products, visit our web site at www.wiley.com. 

Library of Congress Cataloging-in-Publication Data 

Javaheri, Alireza. Inside volatility arbitrage : the secrets of skewness / Alireza Javaheri. p. cm. Includes bibliographical references and index. ISBN 0-471-73387-3 (cloth) 

1. Stocks–Proces–Mathematical models. 2. Stochastic processes. I. Title. HG4636.J38 2005 332.63’222’0151922–dc22 

2005004696 

Printed in the United States of America 10 9 8 7 6 5 4 3 2 1 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/809a17543c10ff834b035311c2ee5ca147f6100ef08b25db37d85fe0bdeb2934.jpg)


## Contents

Illustrations ix
Acknowledgments XV
Introduction xvii
Summary xvii
Contributions and Further Research xxiii
Data and Programs xxiv
APTER 1
The Volatility Problem 1
Introduction 1
The Stock Market 2
The Stock Price Process 2
Historic Volatility 3
The Derivatives Market 4
The Black-Scholes Approach 5
The Cox-Ross-Rubinstein Approach 6
Jump Diffusion and Level-Dependent Volatility 7
Jump Diffusion 8
Level-Dependent Volatility 10
Local Volatility 14
The Dupire Approach 14
The Derman-Kani Approach 17
Stability Issues 18
Calibration Frequency 19
Stochastic Volatility 20
Stochastic Volatility Processes 20
GARCH and Diffusion Limits 21
The Pricing PDE Under Stochastic Volatility 24
The Market Price of Volatility Risk 25
The Two-Factor PDE 26
The Generalized Fourier Transform 27
The Transform Technique 27
Special Cases 28
The Mixing Solution 30
The Romano-Touzi Approach 30 

A One-Factor Monte Carlo Technique 32  
The Long-Term Asymptotic Case 34  
The Deterministic Case 34  
The Stochastic Case 35  
A Series Expansion on Volatility-of-Volatility 37  
Pure-Jump Models 40  
Variance Gamma 40  
Variance Gamma with Stochastic Arrival 43  
Variance Gamma with Gamma Arrival Rate 45  

CHAPTER 2 The Inference Problem 46  
Introduction 46  
Using Option Prices 49  
Direction Set (Powell) Method 49  
Numeric Tests 50  
The Distribution of the Errors 50  
Using Stock Prices 54  
The Likelihood Function 54  
Filtering 57  
The Simple and Extended Kalman Filters 59  
The Unscented Kalman Filter 62  
Kushner's Nonlinear Filter 65  
Parameter Learning 67  
Parameter Estimation via MLE 81  
Diagnostics 95  
Particle Filtering 98  
Comparing Heston with Other Models 120  
The Performance of the Inference Tools 127  
The Bayesian Approach 144  
Using the Characteristic Function 157  
Introducing Jumps 158  
Pure Jump Models 168  
Recapitulation 184  
Model Identification 185  
Convergence Issues and Solutions 185  

CHAPTER 3 The Consistency Problem 187  
Introduction 187  
The Consistency Test 189  
The Setting 190 

The Cross-Sectional Results 190
Robustness Issues for the Cross-Sectional Method 190
Time-Series Results 193
Financial Interpretation 194
The Peso Theory 197
Background 197
Numeric Results 199
Trading Strategies 199
Skewness Trades 200
Kurtosis Trades 200
Directional Risks 200
An Exact Replication 202
The Mirror Trades 203
An Example of the Skewness Trade 203
Multiple Trades 208
High Volatility-of-Volatility and High Correlation 209
Non-Gaussian Case 213
VGSA 215
A Word of Caution 218
Foreign Exchange, Fixed Income, and Other Markets 219
Foreign Exchange 219
Fixed Income 220
References 224
Index 236 

## Illustrations

## Figures

1.1 The SPX Historic Rolling Volatility from 2000/01/03 to 2001/12/31.
1.2 The SPX Volatility Smile on February 12, 2002 with Index = $1107.50, 1 Month and 7 Months to Maturity.
1.3 The CEV Model for SPX on February 12, 2002 with Index = $1107.50, 1 Month to Maturity.
1.4 The BCG Model for SPX on February 12, 2002 with Index = $1107.50, 1 Month to Maturity.
1.5 The GARCH Monte Carlo Simulation with the Square-Root Model for SPX on February 12, 2002 with Index = $1107.50, 1 Month to Maturity.
1.6 The SPX implied surface as of 03/09/2004.
1.7 Mixing Monte Carlo Simulation with the Square-Root Model for SPX on February 12, 2002 with Index = $1107.50, 1 Month and 7 Months to Maturity.
1.8 Comparing the Volatility-of-Volatility Series Expansion with the Monte Carlo Mixing Model.
1.9 Comparing the Volatility-of-Volatility Series Expansion with the Monte Carlo Mixing Model.
1.10 Comparing the Volatility-of-Volatility Series Expansion with the Monte Carlo Mixing Model.
1.11 The Gamma Cumulative Distribution Function P(a, x) for Various Values of the Parameter a.
1.12 The Modified Bessel Function of Second Kind for a Given Parameter.
1.13 The Modified Bessel Function of Second Kind as a Function of the Parameter.
2.1 The S&P500 Volatility Surface as of 05/21/2002 with Index = 1079.88.
2.2 Mixing Monte Carlo Simulation with the Square-Root Model for SPX on 05/21/2002 with Index = $1079.88, Maturity 08/17/2002 Powell (direction set) optimization method was used for least-square calibration. 

2.3 Mixing Monte Carlo Simulation with the Square-Root Model for SPX on 05/21/2002 with Index = $1079.88, Maturity 09/21/2002.
52
2.4 Mixing Monte Carlo Simulation with the Square-Root Model for SPX on 05/21/2002 with Index = $1079.88, Maturity 12/21/2002.
52
2.5 Mixing Monte Carlo Simulation with the Square-Root Model for SPX on 05/21/2002 with Index = $1079.88, Maturity 03/22/2003.
53
2.6 A Simple Example for the Joint Filter.
69
2.7 The EKF Estimation (Example 1) for the Drift Parameter ω.
71
2.8 The EKF Estimation (Example 1) for the Drift Parameter θ.
72
2.9 The EKF Estimation (Example 1) for the Volatility-of-Volatility Parameter ξ.
72
2.10 The EKF Estimation (Example 1) for the Correlation Parameter ρ.
73
2.11 Joint EKF Estimation for the Parameter ω.
78
2.12 Joint EKF Estimation for the Parameter θ.
79
2.13 Joint EKF Estimation for the Parameter ξ.
79
2.14 Joint EKF Estimation for the Parameter ρ.
80
2.15 Joint EKF Estimation for the Parameter ω Applied to the Heston Model as Well as to a Modified Model Where the Noise Is Reduced by a Factor 252.
81
2.16 The SPX Historic Data (1996–2001) is Filtered via EKF and UKF.
84
2.17 The EKF and UKF Absolute Filtering Errors for the Same Time Series.
85
2.18 Histogram for Filtered Data via EKF versus the Normal Distribution.
86
2.19 Variograms for Filtered Data via EKF and UKF.
97
2.20 Variograms for Filtered Data via EKF and UKF.
98
2.21 Filtering Errors: Extended Kalman Filter and Extended Particle Filter Are Applied to the One-Dimensional Heston Model.
115
2.22 Filtering Errors: All Filters Are Applied to the One-Dimensional Heston Model.
116
2.23 Filters Are Applied to the One-Dimensional Heston Model.
117
2.24 The EKF and GHF Are Applied to the One-Dimensional Heston Model.
118
2.25 The EPF Without and with the Metropolis-Hastings Step Is Applied to the One-Dimensional Heston Model.
120 

2.26 Comparison of EKF Filtering Errors for Heston, GARCH, and 3/2 Models. 123
2.27 Comparison of UKF Filtering Errors for Heston, GARCH, and 3/2 Models. 123
2.28 Comparison of EPF Filtering Errors for Heston, GARCH, and 3/2 Models. 124
2.29 Comparison of UPF Filtering Errors for Heston, GARCH, and 3/2 Models. 124
2.30 Comparison of Filtering Errors for the Heston Model. 125
2.31 Comparison of Filtering Errors for the GARCH Model. 125
2.32 Comparison of Filtering Errors for the 3/2 Model. 126
2.33 Simulated Stock Price Path via Heston Using Ψ*. 128
2.34 f(ω) = L(ω, θ̂, ξ̂, ρ̂) Has a Good Slope Around ω̂ = 0.10. 129
2.35 f(θ) = L(ω̂, θ, ξ̂, ρ̂) Has a Good Slope Around θ̂ = 10.0. 130
2.36 f(ξ) = L(ω̂, θ̂, ξ̂, ρ̂) Is Flat Around ξ̂ = 0.03. 130
2.37 f(ρ) = L(ω̂, θ̂, ξ̂, ρ̂) Is Flat and Irregular Around ρ̂ = -0.50. 131
2.38 f(ξ) = L(ω̂, θ̂, ξ̂, ρ̂) via EKF for N = 5000 Points. 132
2.39 f(ξ) = L(ω̂, θ̂, ξ̂, ρ̂) via EKF for N = 50,000 Points. 134
2.40 f(ξ) = L(ω̂, θ̂, ξ̂, ρ̂) via EKF for N = 100,000 Points. 134
2.41 f(ξ) = L(ω̂, θ̂, ξ̂, ρ̂) via EKF for N = 500,000 Points. 135
2.42 Density for ω̂ Estimated from 500 Paths of Length 5000 via EKF. 142
2.43 Density for θ̂ Estimated from 500 Paths of Length 5000 via EKF. 142
2.44 Density for ξ̂ Estimated from 500 Paths of Length 5000 via EKF. 143
2.45 Density for ρ̂ Estimated from 500 Paths of Length 5000 via EKF. 143
2.46 Gibbs Sampler for μ in N(μ, σ). 147
2.47 Gibbs Sampler for σ in N(μ, σ). 148
2.48 Metropolis-Hastings Algorithm for μ in N(μ, σ). 151
2.49 Metropolis-Hastings Algorithm for σ in N(μ, σ). 152
2.50 Plots of the Incomplete Beta Function. 152
2.51 Comparison of EPF Results for Heston and Heston+Jumps Models. The presence of jumps can be seen in the residuals. 166
2.52 Comparison of EPF Results for Simulated and Estimated Jump-Diffusion Time Series. 167
2.53 The Simulated Arrival Rates via Ψ = (κ = 0, η = 0, λ = 0, σ = 0.2, θ = 0.02, ν = 0.005) and Ψ = (κ = 0.13, η = 0, λ = 0.40, σ = 0.2, θ = 0.02, ν = 0.005) Are Quite Different; compare with Figure 2.54.
2.54 However, the Simulated Log Stock Prices are Close. 177 

2.55 The Observation Errors for the VGSA Model with a Generic Particle Filter.
2.56 The Observation Errors for the VGSA model and an Extended Particle filter.
2.57 The VGSA Residuals Histogram.
2.58 The VGSA Residuals Variogram.
2.59 Simulation of VGG-based Log Stock Prices with Two Different Parameter Sets $\Psi = (\mu_{a} = 10.0, \nu_{a} = 0.01, \nu = 0.05, \sigma = 0.2, \theta = 0.002)$ and $\Psi = (9.17, 0.19, 0.012, 0.21, 0.0019)$ .
3.1 Implied Volatilities of Close to ATM Puts and Calls as of 01/02/2002.
3.2 The Observations Have Little Sensitivity to the Volatility Parameters.
3.3 The state Has a Great Deal of Sensitivity to the Volatility Parameters.
3.4 The Observations Have a Great Deal of Sensitivity to the Drift Parameters.
3.5 The State Has a Great Deal of Sensitivity to the Drift Parameters.
3.6 Comparing SPX Cross-Sectional and Time-Series Volatility Smiles (with Historic $\xi$ and $\rho$ ) as of January 2, 2002.
3.7 A Generic Example of a Skewness Strategy to Take Advantage of the Undervaluation of the Skew by Options.
3.8 A Generic Example of a Kurtosis Strategy to Take Advantage of the Overvaluation of the Kurtosis by Options.
3.9 Historic Spot Level Movements During the Trade Period.
3.10 Hedging PnL Generated During the Trade Period.
3.11 Cumulative Hedging PnL Generated During the Trade Period.
3.12 A Strong Option-Implied Skew: Comparing MMM (3M Co) Cross-Sectional and Time-Series Volatility Smiles as of March 28, 2003.
3.13 A Weak Option-Implied Skew: Comparing CMI (Cummins Inc) Cross-Sectional and Time-Series Volatility Smiles as of March 28, 2003.
3.14 GW (Grey Wolf Inc.) Historic Prices (03/31/2002–03/31/2003) Show a High Volatility-of-Volatility But a Weak Stock-Volatility Correlation.
3.15 The Historic GW (Grey Wolf Inc.) Skew Is Low and Not in Agreement with the Options Prices. 

3.16 MSFT (Microsoft) Historic Prices (03/31/2002–03/31/2003) Show a High Volatility-of-Volatility and a Strong Negative Stock-Volatility Correlation.
3.17 The Historic MSFT (Microsoft) Skew Is High and in Agreement with the Options Prices.
3.18 NDX (Nasdaq) Historic Prices (03/31/2002–03/31/2003) Show a High Volatility-of-Volatility and a Strong Negative Stock-Volatility Correlation.
3.19 The Historic NDX (Nasdaq) Skew Is High and in Agreement with the Options Prices.
3.20 Arrival Rates for Simulated SPX Prices Using $\Psi = (\kappa = 0.0000, \eta = 0.0000, \lambda = 0.000000, \sigma = 0.117200, \theta = 0.0056, \nu = 0.002)$ and $\Psi = (\kappa = 79.499687, \eta = 3.557702, \lambda = 0.000000, \sigma = 0.049656, \theta = 0.006801, \nu = 0.008660, \mu = 0.030699).$ 3.21 Gamma Times for Simulated SPX Prices Using $\Psi = (\kappa = 0.0000, \eta = 0.0000, \lambda = 0.000000, \sigma = 0.117200, \theta = 0.0056, \nu = 0.002)$ and $\Psi = (\kappa = 79.99687, \eta = 3.557702, \lambda = 0.000000, \sigma = 0.049656, \theta = 0.006801, \nu = 0.008660, \mu = 0.030699).$ 3.22 Log Stock Prices for Simulated SPX Prices Using $\Psi = (\kappa = 0.0000, \eta = 0.0000, \lambda = 0.000000, \sigma = 0.117200, \theta = 0.0056, \nu = 0.002)$ and $\Psi = (\kappa = 79.899687, \eta = 3.557702, \lambda = 0.000000, \sigma = 0.49656, \theta = 0.006801, \nu = 0.08660, \mu = 0.31699).$ 3.23 A Time Series of the Euro Index from January 2000 to January 2005.
211
211
212
213
216
217
218
222 

## Tables

1.1 SPX Implied Surface as of 03/09/2004. T is the maturity and M = K/S the inverse of the moneyness. 30
1.2 Heston Prices Fitted to the 2004/03/09 Surface. 30
2.1 The Estimation is Performed for SPX on t = 05/21/2002 with Index = $1079.88 for Different Maturities T. 53
2.2 The True Parameter Set Ψ* Used for Data Simulation. 127
2.3 The Initial Parameter Set Ψ₀ Used for the Optimization Process. 127
2.4 The Optimal Parameter Set Ψ̂. 128
2.5 The Optimal EKF Parameters ξ̂ and ρ̂ Given a Sample Size N. 132
2.6 The True Parameter Set Ψ* Used for Data Generation. 133 

2.7 The Initial Parameter Set $\Psi_0$ Used for the Optimization Process. 133  
2.8 The Optimal EKF Parameter Set $\hat{\Psi}$ Given a Sample Size $N$ . 133  
2.9 The Optimal EKF Parameter Set $\hat{\Psi}$ via the HRS Approximation Given a Sample Size $N$ . 136  
2.10 The Optimal PF Parameter Set $\hat{\Psi}$ Given a Sample Size $N$ . 137  
2.11 Real and Optimal Parameter Sets Obtained via NGARCH MLE. 138  
2.12 Real and Optimal Parameter Sets Obtained via NGARCH MLE as well as EKF. 139  
2.13 The Optimal Parameter Set $\hat{\Psi}$ for 5,000,000 Data Points. 139  
2.14 Mean and (Standard Deviation) for the Estimation of Each Parameter via EKF Over $P = 500$ Paths of Lengths $N = 5000$ and $N = 50,000$ . 141  
2.15 MPE and RMSE for the VGSA Model Under a Generic PF as well as the EPF. 179  
3.1 Average Optimal Heston Parameter Set (Under the Risk-Neutral Distribution) Obtained via LSE Applied to One-Year SPX Options in January 2002. 191  
3.2 Average Optimal Heston Parameter Set (Under the Statistical Distribution) Obtained via Filtered MLE Applied to SPX Between January 1992 and January 2004. 193  
3.3 VGSA Statistical Parameters Estimated via PF. 218  
3.4 VGSA Risk-Neutral Arrival-Rate Parameters Estimated from Carr et al. [48]. 219  
3.5 The Volatility and Correlation Parameters for the Cross-Sectional and Time-Series Approaches. 220 

# Acknowledgments

I would like to thank my advisor, Alain Galli, for his guidance and help. Many thanks go to Margaret Armstrong and Delphine Lautier and the entire CERNA team for their support. 

A special thank-you goes to Yves Rouchaleau for helping make all this possible in the first place. 

I would like to sincerely thank other committee members, Marco Avellaneda, Lane Hughston, Piotr Karasinski, and Bernard Lapeyre, for their comments and time. 

I am grateful to Farshid Asl, Peter Carr, Raphael Douady, Robert Engle, Stephen Figlewski, Espen Haug, Ali Hirsa, Michael Johannes, Simon Julier, Alan Lewis, Dilip Madan, Vlad Piterbarg, Youssef Randjiou, David Wong, and the participants at ICBI 2003 and 2004 for all the interesting discussions and idea exchanges. 

I am particularly indebted to Paul Wilmott for encouraging me to speak with Wiley about converting my dissertation into this book. 

Finally, I would like to thank my wife, Firoozeh, and my daughters, Neda and Ariana, for their patience and support. 

## SUMMARY

This book focuses on developing methodologies for estimating stochastic volatility (SV) parameters from the stock-price time series under a classical framework. The text contains three chapters structured as follows. 

In Chapter 1, we shall introduce and discuss the concept of various parametric SV models. This chapter represents a brief survey of the existing literature on the subject of nondeterministic volatility. 

We start with the concept of log-normal distribution and historic volatility. We then introduce the Black-Scholes [38] framework. We also mention alternative interpretations as suggested by Cox and Rubinstein [66]. We state how these models are unable to explain the negative skewness and the leptokurticity commonly observed in the stock markets. Also, the famous implied-volatility smile would not exist under these assumptions. 

At this point we consider the notion of level-dependent volatility as advanced by researchers, such as Cox and Ross [64] and [65], as well as Bensoussan, Crouhy, and Galai [33]. Either an artificial expression of the instantaneous variance will be used, as is the case for constant elasticity variance (CEV) models, or an implicit expression will be deduced from a firm model, similar to Merton’s [189], for instance. 

We also bring up the subject of Poisson jumps [190] in the distributions providing a negative skewness and larger kurtosis. These jump-diffusion models offer a link between the volatility smile and credit phenomena. 

We then discuss the idea of local volatility [36] and its link to the instantaneous unobservable volatility. Work by researchers such as Dupire [89] and by Derman and Kani [74] will be cited. We also describe the limitations of this idea owing to an ill-poised inversion phenomenon, as revealed by Avellaneda [16] and others. 

Unlike nonparametric local volatility models, parametric stochastic volatility (SV) models [140] define a specific stochastic differential equation for the unobservable instantaneous variance. We therefore introduce the notion of two-factor stochastic volatility and its link to one-factor generalized autoregressive conditionally heteroskedastic (GARCH) processes [40]. The SV model class is the one we focus upon. Studies by scholars, such as 

Engle [94], Nelson [194], and Heston [134], are discussed at this juncture. We briefly mention related works on stochastic implied volatility by Schonbucher [213], as well as uncertain volatility by Avellaneda [17]. 

Having introduced SV, we then discuss the two-factor partial differential equations (PDE) and the incompleteness of the markets when only cash and the underlying asset are used for hedging. 

We then examine option pricing techniques, such as inversion of the Fourier transform and mixing Monte Carlo, as well as a few asymptotic pricing techniques, as explained, for instance, by Lewis [177]. 

At this point we tackle the subject of pure-jump models, such as Madan’s variance gamma [182] or its variants VG with stochastic arrivals (VGSA) [48]. The latter adds to the traditional VG a way to introduce the volatility clustering (persistence) phenomenon. We mention the distribution of the stock market as well as various option-pricing techniques under these models. The inversion of the characteristic function is clearly the method of choice for option pricing in this context. 

In Chapter 2, we tackle the notion of inference (or parameter estimation) for parametric SV models. We first briefly analyze cross-sectional inference and then focus upon time-series inference. 

We start with a concise description of cross-sectional estimation of SV parameters in a risk-neutral framework. A least-square estimation (LSE) algorithm is discussed. The direction-set optimization algorithm [204] is introduced at this point. The fact that this optimization algorithm does not use the gradient of the input function is important because we shall later deal with functions that contain jumps and are not necessarily differentiable everywhere. 

We then discuss the parameter inference from a time series of the underlying asset in the real world. We do this in a classical (non-Bayesian) [240] framework, and in particular we will estimate the parameters via a maximization of likelihood estimation (MLE) [127] methodology. We explain the idea of MLE, its link to the Kullback-Leibler [100] distance, as well as the calculation of the likelihood function for a two-factor SV model. 

We see that unlike GARCH models, SV models do not admit an analytic (integrated) likelihood function. This is why we need to introduce the concept of filtering [129]. 

The idea behind filtering is to obtain the best possible estimation of a hidden state given all the available information up to that point. This estimation is done in an iterative manner in two stages: The first step is a time update in which the prior distribution of the hidden state at a given point in time is determined from all the past information via a Chapman-Kolmogorov equation. The second step would then involve a measurement update where this prior distribution is used together with the conditional likelihood of the newest observation in order to compute the posterior distribution of the hidden state. The Bayes rule is used for this purpose. Once the posterior distribution is determined, it can be exploited for the optimal estimation of the hidden state. 

We start with the Gaussian case where the first two moments characterize the entire distribution. For the Gaussian-linear case, the optimal Kalman filter (KF) [129] is introduced. Its nonlinear extension, the extended KF (EKF), is described next. A more suitable version of KF for strongly nonlinear cases, the unscented KF (UKF) [166], is also analyzed. In particular, we see how this filter is related to Kushner’s nonlinear filter (NLF) [173] and [174]. 

The unscented KF uses a first-order Taylor approximation on the nonlinear transition and observation functions, in order to bring us back into a simple KF framework. On the other hand, UKF uses the true nonlinear functions without any approximation. It, however, supposes that the Gaussianity of the distribution is preserved through these functions. The UKF determines the first two moments via integrals that are computed upon a few appropriately chosen “sigma points.” The NLF does the same exact thing via a Gauss-Hermite quadrature. However, NLF often introduces an extra centering step, which will avoid poor performance owing to an insufficient intersection between the prior distribution and the conditional likelihood. 

As we observe, in addition to their use in the MLE approach, the filters can be applied to a direct estimation of the parameters via a joint filter (JF) [133]. The JF would simply involve the estimation of the parameters together with the hidden state via a dimension augmentation. In other words, one would treat the parameters as hidden states. After choosing initial conditions and applying the filter to an observation data set, one would then disregard a number of initial points and take the average upon the remaining estimations. This initial rejected period is known as the “burn-in” period. 

We test various representations or state space models of the stochastic volatility models, such as Heston’s [134]. The concept of observability [205] is introduced in this context. We see that the parameter estimation is not always accurate given a limited amount of daily data. 

Before a closer analysis of the performance of these estimation methods, we introduce simulation-based particle filters (PF) [79] and [122], which can be applied to non-Gaussian distributions. In a PF algorithm, the importance sampling technique is applied to the distribution. Points are simulated via a chosen proposal distribution, and the resulting weights proportional to the conditional likelihood are computed. Because the variance of these weights tends to increase over time and cause the algorithm to diverge, the simulated points go through a variance reduction technique commonly referred to as resampling [14]. During this stage, points with too small a weight are disregarded and points with large weights are reiterated. This technique could cause a sample impoverishment, which can be corrected via a Metropolis-Hastings accept/reject test. Work by researchers such as Doucet [79] and Smith and Gordon [122] are cited and used in this context. 

Needless to say, the choice of the proposal distribution could be fundamental in the success of the PF algorithm. The most natural choice would be to take a proposal distribution equal to the prior distribution of the hidden state. Even if this makes the computations simpler, the danger would be a nonalignment between the prior and the conditional likelihood as we previously mentioned. To avoid this, other proposal distributions taking into account the observation should be considered. The extended PF (EPF) and the unscented PF (UPF) [229] precisely do this by adding an extra Gaussian filtering step to the process. Other techniques, such as auxiliary PF (APF), have been developed by Pitt and Shephard [203]. 

Interestingly, we will see that PF brings only marginal improvement to the traditional KF’s when applied to daily data. However, for a larger time step where the nonlinearity is stronger, the PF does help more. 

At this point, we also compare the Heston model with other SV models, such as the “3/2” model [177] using real market data, and we see that the latter performs better than the former. This is in line with the findings of Engle and Ishida [95]. We can therefore apply our inference tools to perform model identification. 

Various diagnostics [129] are used to judge the performance of the estimation tools. Mean price errors (MPE) and root mean square errors (RMSE) are calculated from the residual errors. The same residuals could be submitted to a Box-Ljung test, which will allow us to see whether they still contain auto correlation. Other tests, such as the chi-square normality test as well as plots of histograms and variograms [110], are performed. 

Most importantly, for the inference process, we back-test the tools upon artificially simulated data, and we observe that although they give the correct answer asymptotically, the results remain inaccurate for a smaller amount of data points. It is reassuring to know that these observations are in agreement with work by other researchers, such as Bagchi [19]. 

Here, we attempt to find an explanation for this mediocre performance. One possible interpretation comes from the fact that in the SV problem, the parameters affect the noise of the observation and not its drift. This is doubly true of volatility-of-volatility and stock-volatility correlation, which affect the noise of the noise. We should, however, note that the product of these two parameters enters in the equations at the same level as the drift of the instantaneous variance, and it is precisely this product that appears in the skewness of the distribution. 

Indeed, the instantaneous volatility is observable only at the second order of a Taylor (or Ito) expansion of the logarithm of the asset price. This also explains why one-factor GARCH models do not have this problem. In their context, the instantaneous volatility is perfectly known as a function of previous data points. The problem therefore seems to be a low signal-to-noise ratio (SNR). We could improve our estimation by considering additional data points. Using a high frequency (several quotes a day) for the data does help in this context. However, one needs to obtain clean and reliable data first. 

Furthermore, we can see why a large time step (e.g., yearly) makes the inference process more robust by improving the observation quality. Still, using a large time step brings up other issues, such as stronger nonlinearity as well as fewer available data points, not to mention the inapplicability of the Girsanov theorem. 

We analyze the sampling distributions of these parameters over many simulations and see how unbiased and efficient the estimators are. Not surprisingly, the inefficiency remains significant for a limited amount of data. 

One needs to question the performance of the actual optimization algorithm as well. It is known that the greater the number of the parameters we are dealing with, the flatter the likelihood function and therefore the more difficult to find a global optimum. Nevertheless, it is important to remember that the SNR and therefore the performance of the inference tool depend on the actual value of the parameters. Indeed, it is quite possible that the real parameters are such that the inference results are accurate. 

We then apply our PF to a jump-diffusion model (such as the Bates [28] model), and we see that the estimation of the jump parameters is more robust than the estimation of the diffusion parameters. This reconfirms that the estimation of parameters affecting the drift of the observation is more reliable. 

We finally apply the PF to non-Gaussian models such as VGSA [48], and we observe results similar to those for the diffusion-based models. Once again the VG parameters directly affecting the observation are easier to estimate, whereas the arrival rate parameters affecting the noise are more difficult to recover. 

Although as mentioned we use a classical approach, we briefly discuss Bayesian methods [34], such as Markov Chain Monte Carlo (MCMC) [163]—including the Gibbs Sampler [55] and the Metropolis-Hastings (MH) [58] algorithm. Bayesian methods consider the parameters not as fixed numbers, but as random variables having a prior distribution. One then updates these distributions from the observations similarly to what is done in the measurement update step of a filter. Sometimes the prior and posterior distributions of the parameters belong to the same family and are referred to as conjugates. The parameters are finally estimated via an averaging procedure similar to the one employed in the JF. Whether the Bayesian methods are actually better or worse than the classical ones has been a subject of long philosophical debate [240] and remains for the reader to decide. 

Other methodologies that differ from ours are the nonparametric (NP) and the semi-nonparametric (SNP). These methods are based on kernel interpolation procedures and have the obvious advantage of being less restrictive. However, parametric models, such as the ones used by us, offer the possibility of comparing and interpreting parameters such as drift and volatility of the instantaneous variance explicitly. Researchers, such as Gallant and Tauchen [109] and Aït-Sahalia [6], use NP/SNP approaches. 

Finally, in Chapter 3, we apply the aforementioned parametric inference methodologies to a few assets and will question the consistency of information contained in the options markets on the one hand, and in the stock market on the other hand. 

We see that there seems to be an excess negative skewness and kurtosis in the former. This is in contradiction with the Girsanov theorem for a Heston model and could mean either that the model is misspecified or that there is a profitable transaction to be made. Another explanation could come from the peso theory [12] (or crash-o-phobia [155]), where an expectation of a so-far absent crash exists in the options markets. 

Adding a jump component to the distributions helps to reconcile the volatility-of-volatility and correlation parameters; however, it remains insufficient. This is in agreement with statements made by Bakshi, Cao, and Chen [20]. 

It is important to realize that, ideally, one should compare the information embedded in the options and the evolution of the underlying asset during the life of these options. Indeed, ordinary put or call options are forward (and not backward) looking. However, given the limited amount of available daily data through this period, we make the assumption that the dynamics of the underlying asset do not change before and during the existence of the options. We therefore use time series that start long before the commencement of these contracts. 

This assumption allows us to consider a skewness trade [6], in which we would exploit such discrepancies by buying out-of-the-money (OTM) call options and selling OTM put options. We see that the results are not necessarily conclusive. Indeed, even if the trade often generates profits, occasional sudden jumps cause large losses. This transaction is therefore similar to “selling insurance.” 

We also apply the same idea to the VGSA model in which despite the non-Gaussian features, the volatility of the arrival rate is supposed to be the same under the real and risk-neutral worlds. 

Let us be clear on the fact that this chapter does not constitute a thorough empirical study of stock versus options markets. It rather presents a set of examples of application for our previously constructed inference tools. There clearly could be many other applications, such as model identification as discussed in the second chapter. 

Yet another application of the separate estimations of the statistical and risk-neutral distributions is the determination of optimal positions in derivatives securities, as discussed by Carr and Madan [52]. Indeed, the expected utility function to be maximized needs the real-world distribution, whereas the initial wealth constraint exploits the risk-neutral distribution. This can be seen via a self-financing portfolio argument similar to the one used by Black and Scholes [38]. 

Finally, we should remember that in all of the foregoing, we are assuming that the asset and options dynamics follow a known and fixed model, such as Heston or VGSA. This is clearly a simplification of reality. The true markets follow an unknown and, perhaps more importantly, constantly changing model. The best we can do is to use the information hitherto available and hope that the future behavior of the assets is not too different from that of the past. Needless to say, as time passes by and new information becomes available, we need to update our models and parameter values. This could be done within either a Bayesian or classical framework. 

Also, we apply the same procedures to other asset classes, such as foreign exchange and fixed income. It is noteworthy that although most of the text is centered on equities, almost no change whatsoever is necessary in order to apply the methodologies to these asset classes, which shows again how flexible the tools are. 

In the Bibliography, many but not all relevant articles and books are cited. Only some of them are directly referred to in the text. 

## CONTRIBUTIONS AND FURTHER RESEARCH

The contribution of the book is in presenting a general and systematic way to calibrate any parametric SV model (diffusion based or not) to a time series under a classical (non-Bayesian) framework. Although the concept of filtering has been used for estimating volatility processes before [130], to my knowledge, this has always been for specific cases and was never generalized. The use of particle filtering allows us to do this in a flexible and simple manner. We also study the convergence properties of our tools and show their limitations. 

Whether the results of these calibrations are consistent with the information contained in the options markets is a fundamental question. The applications of this test are numerous, among which the skewness trade is only one example. 

What else can be done?—a comparative study between our approach and Bayesian approaches on the one hand, and nonparametric approaches on the other hand. Work by researchers such as Johannes, Polson, and Aït-Sahalia would be extremely valuable in this context. 

## DATA AND PROGRAMS

This book centers on time-series methodologies and exploits either artificially generated inputs or real market data. When real market data is utilized, the source is generally Bloomberg. However, most of the data could be obtained from other public sources available on the Internet. 

All numeric computations are performed via routines implemented in the C++ programming language. Some algorithms, such as the direction-set optimization algorithm are taken from Numerical Recipes in C [204]. No statistical packages, such as S-Plus or R, have been used. 

The actual C++ code for some of the crucial routines (such as EKF or UPF) is provided in this text. 

# The Volatility Problem

Suppose we use the standard deviation of possible future returns on a stock as a measure of its volatility. Is it reasonable to take that volatility as a constant over time? I think not. 

— Fischer Black 

## INTRODUCTION

It is widely accepted today that an assumption of a constant volatility fails to explain the existence of the volatility smile as well as the leptokurtic character (fat tails) of the stock distribution. The above Fischer Black quote, made shortly after the famous constant-volatility Black-Scholes model was developed, proves the point. 

In this chapter, we will start by describing the concept of Brownian motion for the stock price return as well as the concept of historic volatility. We will then discuss the derivatives market and the ideas of hedging and risk neutrality. We will briefly describe the Black-Scholes partial derivatives equation (PDE) in this section. Next, we will talk about jumps and level dependent volatility models. We will first mention the jump diffusion process and introduce the concept of leverage. We will then refer to two popular level dependent approaches: the constant elasticity variance (CEV) model and the Bensoussan-Crouhy-Galai (BCG) model. At this point, we will mention local volatility models developed in the recent past by Dupire and Derman-Kani, and we will discuss their stability. 

Following this, we will tackle the subject of stochastic volatility, where we will mention a few popular models, such as the square-root model and the general autoregressive conditional heteroskedasticity (GARCH) model. We will then talk about the pricing PDE under stochastic volatility and the risk-neutral version of it. For this we will need to introduce the concept of market price of risk. 

The generalized Fourier transform is the subject of the following section. This technique was used by Alan Lewis extensively for solving stochastic volatility problems. Next, we will discuss the mixing solution, both in correlated and uncorrelated cases. We will mention its link to the fundamental transform and its usefulness for Monte Carlo–based methods. We will then describe the long-term asymptotic case, where we get closed-form approximations for many popular methods, such as the square-root model. Lastly, we will talk about pure-jump models, such as variance gamma and variance gamma with stochastic arrival. 

## THE STOCK MARKET

## The Stock Price Process

The relationship between the stock market and the mathematical concept of Brownian motion goes back to Bachelier [18]. A Brownian motion corresponds to a process, the increments of which are independent stationary normal random variables. Given that a Brownian motion can take negative values, it cannot be used for the stock price. Instead, Samuelson [211] suggested using this process to represent the return of the stock price, which will make the stock price a geometric (or exponential) Brownian motion. 

In other words, the stock price S follows a log-normal process<sup>1</sup> 

$$
d S _ {t} = \mu S _ {t} d t + \sigma S _ {t} d B _ {t}\tag{1.1}
$$

where d $B _ { t }$ is a Brownian motion process, $\mu$ the instantaneous expected total return of the stock (possibly adjusted by a dividend yield), and $\sigma$ the instantaneous standard deviation of stock price returns, called the volatility in financial markets. 

Using Ito’s lemma $, ^ { 2 }$ we also have 

$$
d \ln (S _ {t}) = \left(\mu - \frac {1}{2} \sigma^ {2}\right) d t + \sigma d B _ {t}\tag{1.2}
$$

The stock return $\mu$ could easily become time dependent without changing any of our arguments. For simplicity, we will often refer to it as $\mu$ even if we mean $\mu _ { t }$ . This remark holds for other quantities, such as $r _ { t } ,$ the interest-rate, or $q _ { t } ,$ the dividend yield. 

Equation (1.1) represents a continuous process. We can either take this as an approximation of the real discrete tick-by-tick stock movements or consider it the real unobservable dynamics of the stock price, in which case the discrete prices constitute a sample from this continuous ideal process. Either way, the use of a continuous equation makes the pricing of financial instruments more analytically tractable. 

The discrete equivalent of (1.2) is 

$$
\ln S _ {t + \Delta t} = \ln S _ {t} + \left(\mu - \frac {1}{2} \sigma^ {2}\right) \Delta t + \sigma \sqrt {\Delta t} B _ {t}\tag{1.3}
$$

where $( B _ { t } )$ is a sequence of independent normal random variables with zero mean and variance of 1. 

## Historic Volatility

This suggests a first simple way to estimate the volatility, $\sigma ,$ namely the historic volatility. Considering $S _ { 1 } , . . . , S _ { N }$ as a sequence of known historic daily stock close prices, calling $R _ { n } = \ln ( S _ { n + 1 } / S _ { n } )$ the stock price return between two days and $\begin{array} { r } { \bar { R } = \frac { 1 } { N } \sum _ { n = 0 } ^ { N - 1 } { R _ { n } } } \end{array}$ the mean return, the historic volatility would be the annualized standard deviation of the returns, namely 

$$
\sigma_ {h i s t} = \sqrt {\frac {2 5 2}{N - 1} \sum_ {n = 0} ^ {N - 1} (R _ {n} - \bar {R}) ^ {2}}\tag{1.4}
$$

Because we work with annualized quantities, and we are using daily stock closing prices, we needed the factor 252, supposing that there are approximately 252 business days in a year.<sup>3</sup> 

Note that N, the number of observations, can be more or less than one year; therefore when talking about a historic volatility, it is important to know what time horizon we are considering. We can indeed have threemonth historic volatility or three-year historic volatility. Needless to say, taking too few prices would give an inaccurate estimation. Similarly, the begin and end date of the observations matter. It is preferable to take the end date as close as possible to today so that we include recent observations. 

An alternative was suggested by Parkinson [200] in which instead of daily closing prices we use the high and the low prices of the stock on that day, and $R _ { n } = \mathrm { l n } ( S _ { n } ^ { b i g b } / S _ { n } ^ { l o w } )$ . The volatility would then be 

$$
\sigma_ {p a r k i n s o n} = \sqrt {\frac {2 5 2}{N - 1} \frac {1}{4 \ln (2)} \sum_ {n = 0} ^ {N - 1} (R _ {n} - \bar {R}) ^ {2}}
$$

This second moment estimation derived by Parkinson is based upon the fact that the range $R _ { n }$ of the asset follows a Feller distribution. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/2c85c4919ddd32c360c98eb3ba2ae2356374b6c99d721d3b005216a21185b97b.jpg)



FIGURE 1.1 The SPX Historic Rolling Volatility from 01/03/2000 to 12/31/2001. As we can see, the volatility is clearly nonconstant.


Plotting, for instance, the one-year rolling<sup>4</sup> historic volatility (1.4) of the S&P 500 Stock Index, it is easily seen that this quantity is not constant over time (Figure 1.1). This observation was made as early as the 1960s by many financial mathematicians and followers of the chaos theory. We therefore need time-varying volatility models. 

One natural extension of the constant volatility approach is to make $\sigma _ { t }$ a deterministic function of time. This is equivalent to giving the volatility a term structure, by analogy with interest rates. 

## THE DERIVATIVES MARKET

Until now, we have mentioned the stock price movements independently from the derivatives market, but we now are going to include the financial derivatives (especially options) prices as well. These instruments became very popular and as liquid as the stocks themselves after Black and Scholes introduced their risk-neutral pricing formula in [38]. 

## The Black-Scholes Approach

The Black-Scholes approach makes a number of reasonable assumptions about markets being frictionless and uses the log-normal model for the stock price movements. It also supposes a constant or deterministically timedependent stock drift and volatility. Under these conditions, they prove that it is possible to hedge a position in a contingent claim dynamically by taking an offsetting position in the underlying stock and hence become immune to the stock movements. This risk neutrality is possible because, as they show, we can replicate the financial derivative (for instance, an option) by taking positions in cash and the underlying security. This condition of the possibility of replication is called market completeness. 

In this situation, everything happens as if we were replacing the stock drift $\mu _ { t }$ with the risk-free rate of interest $r _ { t }$ in (1.1) or $r _ { t } - q _ { t }$ if there is a dividend-yield $q _ { t }$ . The contingent claim $f ( S , t )$ having a payoff $G ( S _ { T } )$ will satisfy the famous Black-Scholes equation 

$$
r f = \frac {\partial f}{\partial t} + (r - q) S \frac {\partial f}{\partial S} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} f}{\partial S ^ {2}}\tag{1.5}
$$

Indeed the hedged portfolio $\begin{array} { r } { \Pi = f - \frac { \partial f } { \partial S } S } \end{array}$ is immune to the stock random movements and, according to Ito’s lemma, verifies 

$$
d \Pi = \left(\frac {\partial f}{\partial t} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} f}{\partial S ^ {2}}\right) d t
$$

which must also be equal to rdt or else there would be possibility of Riskless arbitrage.<sup>5</sup> 

Note that this equation is closely related to the Feynman-Kac equation satisfied by $F ( S , t ) = \mathbf { E } _ { t } ( b ( S _ { T } ) )$ for any function h under the risk-neutral measure; $F ( S , t )$ must be a Martinga $\mathrm { l e } ^ { 6 }$ under this measure and therefore must be driftless, which implies $\begin{array} { r } { d \boldsymbol { F } = \sigma \boldsymbol { S } \frac { \partial \boldsymbol { F } } { \partial \boldsymbol { S } } d \boldsymbol { B } _ { t } } \end{array}$ and 

$$
0 = \frac {\partial F}{\partial t} + (r - q) S \frac {\partial F}{\partial S} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} F}{\partial S ^ {2}}
$$

This would indeed be a different way to reach the same Black-Scholes equation, by using $f ( S , t ) = \exp ( - r t ) F ( S , t )$ , as was done, for instance, in Shreve [218]. 

Let us insist again on the fact that the real drift of the stock price does not appear in the preceding equation, which makes the volatility $\sigma _ { t }$ the only unobservable quantity. As we said, the volatility could be a deterministic function of time without changing the foregoing argument, in which case all we need to do is to replace $\sigma ^ { 2 }$ with $\textstyle { \frac { 1 } { t } } \int _ { 0 } ^ { t } { \boldsymbol { \sigma } } _ { s } ^ { 2 } d s$ , and keep everything else the same. 

For calls and puts, where the payoffs $G ( S _ { T } )$ are respectively $M A X ( 0 , S _ { T } -$ $K )$ and $M A X ( 0 , K - S _ { T } )$ and where K is the strike price and $T$ the maturity of the option, the Black-Scholes partial derivatives equation is solvable and gives the celebrated Black-Scholes formulae 

$$
c a l l _ {t} = S _ {t} e ^ {- q (T - t)} \Phi (d _ {1}) - K e ^ {- r (T - t)} \Phi (d _ {2})\tag{1.6}
$$

and 

$$
p u t _ {t} = - S _ {t} e ^ {- q (T - t)} \Phi (- d _ {1}) + K e ^ {- r (T - t)} \Phi (- d _ {2})\tag{1.7}
$$

where 

$$
\Phi (x) = \frac {1}{\sqrt {2 \pi}} \int_ {- \infty} ^ {x} e ^ {- \frac {u ^ {2}}{2}} d u
$$

is the cumulative standard normal function and 

$$
d _ {1} = d _ {2} + \sigma \sqrt {T - t} \quad \text { and } \quad d _ {2} = \frac {\ln \left(\frac {S _ {t}}{K}\right) + \left(r - q - \frac {1}{2} \sigma^ {2}\right) (T - t)}{\sigma \sqrt {T - t}}
$$

Note that using the well-known symmetry property for normal distributions $\Phi ( - x ) = 1 - \Phi ( x )$ in the above formulae, we could reach the put-call parity relationship 

$$
c a l l _ {t} - p u t _ {t} = S _ {t} e ^ {- q (T - t)} - K e ^ {- r (T - t)}\tag{1.8}
$$

which we can also rearrange as 

$$
S _ {t} e ^ {- q (T - t)} - c a l l _ {t} = K e ^ {- r (T - t)} - p u t _ {t}
$$

The left-hand side of this last equation is called a covered call and is equivalent to a short position in a put combined with a bond. 

## The Cox-Ross-Rubinstein Approach

Later, Cox, Ross, and Rubinstein [66] developed a simplified approach using the binomial law to reach the same pricing formulae. The approach commonly referred to as the binomial tree uses a tree of recombining spot prices, in which at a given time step n we have $n + 1$ possible $S [ n ] [ j ]$ spot prices, with $0 \leq j \leq n$ . Calling $\boldsymbol { p }$ the upward transition probability and $1 - p$ the downward transition probability, S the stock price today, and $S _ { u } = u S$ and ${ \cal S } _ { d } = d { \cal S }$ upper and lower possible future spot prices, we can write the expectation equation<sup>7</sup> 

$$
\mathbf {E} [ S ] = p u S + (1 - p) d S = e ^ {r \Delta t} S
$$

which immediately gives us 

$$
p = \frac {a - d}{u - d}
$$

with $a = \exp ( r \Delta t )$ 

We can also write the variance equation 

$$
V a r [ S ] = p u ^ {2} S ^ {2} + (1 - p) d ^ {2} S ^ {2} - e ^ {2 r \Delta t} S ^ {2} \approx \sigma^ {2} S ^ {2} \Delta t
$$

which after choosing a centering condition, such as $u d = 1$ , will provide us with $u = \exp ( \sigma \sqrt { \Delta t } )$ and $d = \exp ( - \sigma \sqrt { \Delta t } )$ . Using the values for $u , d ,$ and $\boldsymbol { p }$ we can build the tree, and using the final payoff we can calculate the option price by backward induction.<sup>8</sup> We can also build this tree by applying an explicit finite difference scheme to the PDE (1.5), as was done in Wilmott [238]. An important advantage of the tree method is that it can be applied to American options (with early exercise) as well. 

It is possible to deduce the implied volatility of call and put options by solving a reverse Black-Scholes equation, that is, find the volatility that would equate the Black-Scholes price to the market price of the option. This is a good way to see how derivatives markets perceive the underlying volatility. It is easy to see that if we change the maturity and strike prices of options (and keep everything else fixed) the implied volatility will not be constant. It will have a linear skew and a convex form as the strike price changes. This famous “smile” cannot be explained by simple time dependence, hence the necessity of introducing new models (Figure 1.2).<sup>9</sup> 

## JUMP DIFFUSION AND LEVEL-DEPENDENT VOLATILITY

In addition to the volatility smile observable from the implied volatilities of the options, there is evidence that the assumption of a pure normal distribution (also called pure diffusion) for the stock return is not accurate. Indeed “fat tails” have been observed away from the mean of the stock return. This phenomenon is called leptokurticity and could be explained in many different ways. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/dc8c687b2e1ae45031bece79314415d349ece744b1813704081be9ac8b3a699c.jpg)



FIGURE 1.2 The SPX Volatility Smile on February 12, 2002 with Index = $1107.50, 1 Month and 7 Months to Maturity. The negative skewness is clearly visible. Note how the smile becomes flatter as time to maturity increases.


## Jump Diffusion

Some try to explain the smile and the leptokurticity by changing the underlying stock distribution from a diffusion process to a jump-diffusion process. A jump diffusion is not a level-dependent volatility process; however, we are mentioning it in this section to demonstrate the importance of the leverage effect. Merton [190] was first to actually introduce jumps in the stock distribution. Kou [172] recently used the same idea to explain both the existence of fat tails and the volatility smile. 

The stock price will follow a modified stochastic process under this assumption. If we add to the Brownian motion, d $B _ { t } \mathbf { ; }$ a Poisson (jump) process<sup>10</sup> dq with an intensity<sup>11</sup> λ, and then calling $k = \mathbf { E } ( Y - 1 )$ with Y 1 the random variable percentage change in the stock price, we will have 

$$
d S _ {t} = (\mu - \lambda k) S _ {t} d t + \sigma S _ {t} d B _ {t} + S _ {t} d q\tag{1.9}
$$

or equivalently, 

$$
S _ {t} = S _ {0} \exp \left[ \left(\mu - \frac {\sigma^ {2}}{2} - \lambda k\right) t + \sigma B _ {t} \right] Y _ {n}
$$

where $Y _ { 0 } = 1$ and $\begin{array} { r } { Y _ { n } = \prod _ { j = 1 } ^ { n } Y _ { j } , } \end{array}$ , with $Y _ { j } { ' } { \bf { s } }$ independently identically distri-buted random variables and n a Poisson random variable with a parameter $\lambda t .$ 

It is worth noting that for the special case where the jump corresponds to total ruin or default, we have $k = - 1$ , which will give us 

$$
d S _ {t} = (\mu + \lambda) S _ {t} d t + \sigma S _ {t} d B _ {t} + S _ {t} d q\tag{1.10}
$$

and 

$$
S _ {t} = S _ {0} \exp \left[ \left(\mu + \lambda - \frac {\sigma^ {2}}{2}\right) t + \sigma B _ {t} \right] Y _ {n}
$$

Given that in this case $\mathbf { E } ( Y _ { n } ) = \mathbf { E } ( Y _ { n } ^ { 2 } ) = e ^ { - \lambda t } ,$ it is fairly easy to see that in the risk-neutral world 

$$
\mathbf {E} (S _ {t}) = S _ {0} e ^ {r t}
$$

exactly as in the pure diffusion case, but 

$$
V a r (S _ {t}) = S _ {0} ^ {2} e ^ {2 r t} \bigl (e ^ {(\sigma^ {2} + \lambda) t} - 1 \bigr) \approx S _ {0} ^ {2} \bigl (\sigma^ {2} + \lambda \bigr) t\tag{1.11}
$$

unlike the pure diffusion case, where $V a r ( S _ { t } ) \approx S _ { 0 } ^ { 2 } \sigma ^ { 2 } t .$ 

Proof: Indeed 

$$
\begin{array}{c} \mathbf {E} (S _ {t}) = S _ {0} \exp ((r + \lambda) t) \exp \biggl (- \frac {\sigma^ {2}}{2} t \biggr) \mathbf {E} [ \exp (\sigma B _ {t}) ] \mathbf {E} (Y _ {n}) \\ = S _ {0} \exp ((r + \lambda) t) \exp \biggl (- \frac {\sigma^ {2}}{2} t \biggr) \exp \biggl (\frac {\sigma^ {2}}{2} t \biggr) \exp (- \lambda t) = S _ {0} \exp (r t) \end{array}
$$

and 

$$
\begin{array}{l} \mathbf {E} (S _ {t} ^ {2}) = S _ {0} ^ {2} \exp (2 (r + \lambda) t) \exp \bigl (- \sigma^ {2} t \bigr) \mathbf {E} [ \exp (2 \sigma B _ {t}) ] \mathbf {E} (Y _ {n} ^ {2}) \\ \qquad = S _ {0} ^ {2} \exp (2 (r + \lambda) t) \exp \bigl (- \sigma^ {2} t \bigr) \exp \biggl (\frac {(2 \sigma) ^ {2}}{2} \biggr) \exp (- \lambda t) \\ \qquad = S _ {0} ^ {2} \exp ((2 r + \lambda) t) \exp \bigl (\sigma^ {2} t \bigr) \end{array}
$$

and as usual 

$$
V a r (S _ {t}) = \mathbf {E} \big (S _ {t} ^ {2} \big) - \mathbf {E} ^ {2} (S _ {t})
$$

(QED) 

Link to Credit Spread Note that for a zero-coupon risky bond $Z$ with no recovery, a credit spread C and a face value X paid at time t we have 

$$
Z = e ^ {- (r + C) t} X = e ^ {- \lambda t} (e ^ {- r t} X) + (1 - e ^ {- \lambda t}) (0)
$$

consequently $\lambda = C$ and using (1.11) we can write 

$$
\tilde {\sigma} ^ {2} (C) = \sigma^ {2} + C
$$

where $\sigma$ is the fixed (pure diffusion) volatility and $\tilde { \sigma }$ is the modified jump diffusion volatility. The preceding equation relates the volatility and leverage, a concept we will see later in level-dependent models as well. 

Also, we could see that everything happens as if we were using the Black-Scholes pricing equation but with a modified “interest rate,” which is $r + \mathrm { C }$ Indeed the hedged portfolio $\begin{array} { r } { \Pi = f - \frac { \partial f } { \partial S } S } \end{array}$ now satisfies 

$$
d \Pi = \left(\frac {\partial f}{\partial t} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} f}{\partial S ^ {2}}\right) d t
$$

under the no-default case, which occurs with a probability of $e ^ { - \lambda d t } \approx 1 - \lambda d t$ and 

$$
d \Pi = - \Pi
$$

We therefore have 

$$
1 - e ^ {- \lambda d t} \approx \lambda d t
$$

$$
\mathbf {E} (d \Pi) = \left(\frac {\partial f}{\partial t} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} f}{\partial S ^ {2}} - \lambda \Pi\right) d t
$$

and using a diversification argument we can always say that $\mathbf { E } ( d \Pi ) = r \Pi d t$ which provides us with 

$$
(r + \lambda) f = \frac {\partial f}{\partial t} + (r + \lambda) S \frac {\partial f}{\partial S} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} f}{\partial S ^ {2}}\tag{1.12}
$$

which again is the Black-Scholes PDE with a “risky rate.” 

A generalization of the jump diffusion process would be the use of the Levy process. A Levy process is a stochastic process with independent and stationary increments. Both the Brownian motion and the Poisson process are included in this category. For a description, see Matacz [186]. 

## Level-Dependent Volatility

Many assume that the smile and the fat tails are due to the level dependence of the volatility. The idea would be to make $\sigma _ { t }$ level dependent or a function of the spot itself; we would therefore have 

$$
d S _ {t} = \mu_ {t} S _ {t} d t + \sigma (S, t) S _ {t} d B _ {t}\tag{1.13}
$$

Note that to be exact, a level-dependent volatility is a function of the spot price alone. When the volatility is a function of the spot price and time, it is referred to as local volatility, which we shall discuss further. 

The Constant Elasticity Variance Approach One of the very first attempts to use this approach was the constant elasticity variance (CEV) method realized by Cox [64] and [65] (Figure 1.3). In this method we would suppose an equation of the type 

$$
\sigma (S, t) = C S _ {t} ^ {\gamma}\tag{1.14}
$$

where C and $\gamma$ are parameters to be calibrated either from the stock price returns themselves or from the option prices and their implied volatilities. The CEV method was recently analyzed by Jones [165] in a paper in which he uses two γ exponents. 

This level-depending volatility represents an important feature that is observed in options markets as well as in the underlying prices: the negative correlation between the stock price and the volatility, also called the leverage effect. 

The Bensoussan-Crouhy-Galai Approach Bensoussan, Crouhy, and Galai (BCG) [33] try to find the level dependence of the volatility in a manner that differs from that of Cox and Ross (Figure 1.4). Indeed in the CEV model, Cox and 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/a83aed1d9166175a290bd631552418a0a5c314f6dcb4023b40b546cbd5c40a84.jpg)



FIGURE 1.3 The CEV Model for SPX on February 12, 2002 with Index = $1107.50, 1 Month to Maturity. The smile is fitted well, but the model assumes a perfect (negative) correlation between the stock and the volatility.


Ross first suppose that $\sigma ( S , t )$ has a certain exponential form and only then try to calibrate the model parameters to the market. Alternatively, BCG try to deduce the functional form of $\sigma ( S , t )$ by using a firm structure model. 

The idea of firm structure is not new and goes back to Merton [189], when he considers that the firm assets follow a log-normal process 

$$
d V = \mu_ {V} V d t + \sigma_ {V} V d B _ {t}\tag{1.15}
$$

where $\mu _ { V }$ and $\sigma _ { V }$ are the asset’s return and volatility. One important point is that $\sigma _ { V }$ is considered constant. Merton then argues that the equity S of the firm could be considered a call option on the assets of the firm with a strike price K equal to the face value of the firm liabilities and an expiration T equal to the average liability maturity. 

Using Ito’s lemma, it is fairly easy to see that 

$$
\begin{array}{l} d S = \mu S d t + \sigma (S, t) S d B _ {t} \\ = \left(\frac {\partial S}{\partial t} + \mu_ {V} V \frac {\partial S}{\partial V} + \frac {1}{2} \sigma_ {V} ^ {2} V ^ {2} \frac {\partial^ {2} S}{\partial V ^ {2}}\right) d t + \sigma_ {V} V \frac {\partial S}{\partial V} d B _ {t} \end{array}\tag{1.16}
$$

which immediately provides us with 

$$
\sigma (S, t) = \sigma_ {V} \frac {V}{S} \frac {\partial S}{\partial V}\tag{1.17}
$$

which is an implicit functional form for $\sigma ( S , t )$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/07e5dfb16869535d5b516ce95c976351e1a5a3f83d265b234e2abb756b9bb4e8.jpg)



FIGURE 1.4 The BCG Model for SPX on February 12, 2002 with Index = $1107.50, 1 Month to Maturity. The smile is fitted well.


Next, BCG eliminate the asset term in the preceding functional form and end up with a nonlinear PDE 

$$
\frac {\partial \sigma}{\partial t} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} \sigma}{\partial S ^ {2}} + (r + \sigma^ {2}) S \frac {\partial \sigma}{\partial S} = 0\tag{1.18}
$$

This PDE gives the dependence of $\sigma$ on S and $t$ 

Proof: A quick sketch of the proof is as follows: With S being a contingent claim on V , we have the risk-neutral Black-Scholes PDE 

$$
\frac {\partial S}{\partial t} + r V \frac {\partial S}{\partial V} + \frac {1}{2} \sigma_ {V} ^ {2} V ^ {2} \frac {\partial^ {2} S}{\partial V ^ {2}} = r S
$$

and using $\textstyle { \frac { \partial S } { \partial V } } = 1 / { \frac { \partial V } { \partial S } }$ as well as $\begin{array} { r } { \frac { \partial S } { \partial t } = - \frac { \partial S } { \partial V } \frac { \partial V } { \partial t } } \end{array}$ and $\begin{array} { r } { \frac { \partial ^ { 2 } S } { \partial V ^ { 2 } } = - \frac { \partial ^ { 2 } V } { \partial S ^ { 2 } } / \left( \frac { \partial V } { \partial S } \right) ^ { 3 } } \end{array}$ we have the reciprocal Black-Scholes equation 

$$
\frac {\partial V}{\partial t} + r S \frac {\partial V}{\partial S} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} V}{\partial S ^ {2}} = r V
$$

Now posing $\Psi ( S , t ) = \ln V ( S , t )$ , we have $\begin{array} { r } { { \frac { \partial V } { \partial t } } = V { \frac { \partial \Psi } { \partial t } } } \end{array}$ as well as $\begin{array} { r } { \frac { \partial V } { \partial S } = V \frac { \partial \Psi } { \partial S } } \end{array}$ and $\begin{array} { r } { \frac { \partial ^ { 2 } V } { \partial S ^ { 2 } } = V \left( \frac { \partial ^ { 2 } \Psi } { \partial S ^ { 2 } } + ( \frac { \partial \Psi } { \partial S } ) ^ { 2 } \right) } \end{array}$ , and we will have the new PDE 

$$
r = \frac {\partial \Psi}{\partial t} + r S \frac {\partial \Psi}{\partial S} + \frac {1}{2} \sigma^ {2} S ^ {2} \left(\frac {\partial^ {2} \Psi}{\partial S ^ {2}} + \left(\frac {\partial \Psi}{\partial S}\right) ^ {2}\right)
$$

and the equation 

$$
\sigma = \sigma_ {V} / \left(S \frac {\partial \Psi}{\partial S}\right)
$$

This last identity implies that $\begin{array} { r } { \frac { \partial \Psi } { \partial S } = \frac { \sigma _ { V } } { S \sigma } } \end{array}$ as well as $\begin{array} { r } { \frac { \partial ^ { 2 } \Psi } { \partial S ^ { 2 } } = \frac { - \sigma _ { V } ( \sigma + S \frac { \partial \sigma } { \partial S } ) } { S ^ { 2 } \sigma ^ { 2 } } } \end{array}$ , and therefore the PDE becomes 

$$
r = \frac {\partial \Psi}{\partial t} + r \sigma_ {V} / \sigma + \frac {1}{2} \left(\sigma_ {V} ^ {2} - \sigma_ {V} \left(\sigma + S \frac {\partial \sigma}{\partial S}\right)\right)
$$

taking the derivative with respect to S and using $\begin{array} { r } { \frac { \partial ^ { 2 } \Psi } { \partial S \partial t } = - \frac { \sigma _ { V } } { S \sigma ^ { 2 } } \frac { \partial \sigma } { \partial t } } \end{array}$ we get the final PDE 

$$
\frac {\partial \sigma}{\partial t} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} \sigma}{\partial S ^ {2}} + (r + \sigma^ {2}) S \frac {\partial \sigma}{\partial S} = 0
$$

as previously stated. (QED) 

We therefore have an implicit functional form for $\sigma ( S , t )$ , and, just as for the CEV case, we need to calibrate the parameters to the market data. 

## LOCAL VOLATILITY

In the early 1990s, Dupire [89], as well as Derman and Kani [74], developed a concept called local volatility, in which the volatility smile was retrieved from the option prices. 

## The Dupire Approach

The Breeden & Litzenberger Identity This approach uses the options prices to get the implied distribution for the underlying stock. To do this we can write 

$$
V (S _ {0}, K, T) = \operatorname{call} (S _ {0}, K, T) = e ^ {- r T} \int_ {0} ^ {+ \infty} (S - K) ^ {+} p (S _ {0}, S, T) d S\tag{1.19}
$$

where $S _ { 0 }$ is the stock price at time $t = 0$ and K the strike price of the call, and $\ p ( S _ { 0 } , S , T )$ is the unknown transition density for the stock price. As usual, $x ^ { + } = M A X ( x , 0 )$ 

Using Equation (1.19) and differentiating with respect to K twice, we get the Breeden and Litzenberger [44] implied distribution 

$$
p (S _ {0}, K, T) = e ^ {r T} \frac {\partial^ {2} V}{\partial K ^ {2}}\tag{1.20}
$$

Proof: The proof is straightforward if we write 

$$
e ^ {r T} V (S _ {0}, K, T) = \int_ {K} ^ {+ \infty} S p (S _ {0}, S, T) d S - K \int_ {K} ^ {+ \infty} p (S _ {0}, S, T) d S
$$

and take the first derivative 

$$
e ^ {r T} \frac {\partial V}{\partial K} = - K p (S _ {0}, K, T) + K p (S _ {0}, K, T) - \int_ {K} ^ {+ \infty} p (S _ {0}, S, T) d S
$$

and the second derivative in the same manner. (QED) 

The Dupire Identity Now, according to the Fokker-Planck (or forward Kolmogorov) equation<sup>12</sup> for this density, we have 

$$
{\frac {\partial p}{\partial T}} = {\frac {1}{2}} {\frac {\partial^ {2} (\sigma^ {2} (S , t) S ^ {2} p)}{\partial S ^ {2}}} - r {\frac {\partial (S p)}{\partial S}}
$$

and therefore after a little rearrangement have 

$$
\frac {\partial V}{\partial T} = \frac {1}{2} \sigma^ {2} K ^ {2} \frac {\partial^ {2} V}{\partial K ^ {2}} - r K \frac {\partial V}{\partial K}
$$

which provides us with the local volatility formula 

$$
\sigma^ {2} (K, T) = \frac {\frac {\partial V}{\partial T} + r K \frac {\partial V}{\partial K}}{\frac {1}{2} K ^ {2} \frac {\partial^ {2} V}{\partial K ^ {2}}}\tag{1.21}
$$

Proof: For a quick proof of the above let us use the zero interest rates case (the general case could be done similarly). We would then have 

$$
p (S _ {0}, K, T) = \frac {\partial^ {2} V}{\partial K ^ {2}}
$$

as well as Fokker-Planck 

$$
\frac {\partial p}{\partial T} = \frac {1}{2} \frac {\partial^ {2} (\sigma^ {2} (S , t) S ^ {2} p)}{\partial S ^ {2}}
$$

Now 

$$
\begin{array}{l} \frac {\partial V}{\partial T} = \int_ {0} ^ {+ \infty} (S _ {T} - K) ^ {+} \frac {\partial p}{\partial T} d S _ {T} \\ = \int_ {0} ^ {+ \infty} (S _ {T} - K) ^ {+} \frac {1}{2} \frac {\partial^ {2} (\sigma^ {2} (S , T) S ^ {2} p)}{\partial S ^ {2}} d S _ {T} \end{array}
$$

and integrating by parts twice and using the fact that 

$$
\frac {\partial^ {2} (S _ {T} - K) ^ {+}}{\partial K ^ {2}} = \delta (S _ {T} - K)
$$

with $\delta ( . )$ , the Dirac function, we will have 

$$
\frac {\partial V}{\partial T} = \frac {1}{2} \sigma^ {2} (K, T) K ^ {2} p (S _ {0}, K, T) = \frac {1}{2} K ^ {2} \sigma^ {2} (K, T) \frac {\partial^ {2} V}{\partial K ^ {2}}
$$

as stated. (QED) 

It is also possible to use the implied volatility, $\sigma _ { B S }$ , from the Black-Scholes formula (1.6) and express the foregoing local volatility in terms of $\sigma _ { B S }$ instead of V. For a detailed discussion, we could refer to Wilmott [237]. 

Local Volatility vs. Instantaneous Volatility Clearly, the local volatility is related to the instantaneous variance $\nu _ { t } ,$ , as Gatheral [113] shows; the relationship could be written as 

$$
\sigma^ {2} (K, T) = \mathbf {E} [ \nu_ {T} | S _ {T} = K ]\tag{1.22}
$$

that is, local variance is the risk-neutral expectation of the instantaneous variance conditional on the final stock price being equal to the strike price.<sup>13</sup> 

Proof: Let us show the above identity for the case of zero interest rates.<sup>14</sup> As mentioned, we have 

$$
\sigma^ {2} (K, T) = \frac {\frac {\partial V}{\partial T}}{\frac {1}{2} K ^ {2} \frac {\partial^ {2} V}{\partial K ^ {2}}}
$$

On the other hand, using the call payoff $V ( S _ { 0 } , K , t = T ) = \mathbf { E } [ ( S _ { T } - K ) ^ { + } ]$ we have 

$$
\frac {\partial V}{\partial K} = \mathbf {E} [ H (S _ {T} - K) ]
$$

with H(.), the heaviside function and 

$$
\frac {\partial^ {2} V}{\partial K ^ {2}} = \mathbf {E} [ \delta (S _ {T} - K) ]
$$

with $\delta ( . )$ , the Dirac function. 

Therefore the Ito lemma at $t = T$ would provide 

$$
d (S _ {T} - K) ^ {+} = H (S _ {T} - K) d S _ {T} + \frac {1}{2} \nu_ {T} S _ {T} ^ {2} \delta (S _ {T} - K) d T
$$

Using the fact that the forward price (here with zero interest rates, the stock price) is a Martingale under the risk-neutral measure 

$$
d V = d \mathbf {E} [ (S _ {T} - K) ^ {+} ] = \frac {1}{2} \mathbf {E} \left[ \nu_ {T} S _ {T} ^ {2} \delta (S _ {T} - K) \right] d T
$$

Now we have 

$$
\begin{array}{r} \mathbf {E} [ \nu_ {T} S _ {T} ^ {2} \delta (S _ {T} - K) ] = \mathbf {E} [ \nu_ {T} | S _ {T} = K ] K ^ {2} \mathbf {E} [ \delta (S _ {T} - K) ] \\ = \mathbf {E} [ \nu_ {T} | S _ {T} = K ] K ^ {2} \frac {\partial^ {2} V}{\partial K ^ {2}} \end{array}
$$

Putting all this together 

$$
\frac {\partial V}{\partial T} = \frac {1}{2} K ^ {2} \frac {\partial^ {2} V}{\partial K ^ {2}} \mathbf {E} [ \nu_ {T} | S _ {T} = K ]
$$

and by the preceding expression of $\sigma ^ { 2 } ( K , T )$ , we will have 

$$
\sigma^ {2} (K, T) = \mathbf {E} [ \nu_ {T} | S _ {T} = K ]
$$

as claimed. (QED) 

## The Derman-Kani Approach

The Derman-Kani technique is very similar to the above approach, except that it uses the binomial (or trinomial) tree framework instead of the continuous one. Using the binomial tree notations, their upward transition probability $\ b _ { \mathscr { p } _ { i } }$ from the spot $s _ { i }$ at time $t _ { n }$ to the upper node $S _ { i + 1 }$ at the following time-step $t _ { n + 1 }$ , is obtained from the usual 

$$
p _ {i} = \frac {F _ {i} - S _ {i}}{S _ {i + 1} - S _ {i}}\tag{1.23}
$$

where $F _ { i }$ is the stock forward price known from the market and $S _ { i }$ the lower spot at the step $t _ { n + 1 }$ 

In addition, we have for a call expiring at time step $t _ { n + 1 }$ 

$$
C (K, t _ {n + 1}) = e ^ {- r \Delta t} \sum_ {j = 1} ^ {n} \left[ \lambda_ {j} p _ {j} + \lambda_ {j + 1} \left(1 - p _ {j + 1}\right) \right] M A X (S _ {j + 1} - K, 0)
$$

where $\lambda _ { j } { \bf \dot { s } }$ are the known Arrow-Debreu prices corresponding to the discounted probability of getting to the point $s _ { j }$ at time $t _ { n }$ from $S _ { 0 } .$ , the initial stock price. These probabilities could easily be derived iteratively. 

This allows us after some calculation to obtain $S _ { i + 1 }$ as a function of $s _ { i }$ and $S _ { i : }$ , namely 

$$
S _ {i + 1} = \frac {S _ {i} [ e ^ {r \Delta t} C (s _ {i} , K , t _ {n + 1}) - \Sigma ] - \lambda_ {i} s _ {i} (F _ {i} - S _ {i})}{[ e ^ {r \Delta t} C (s _ {i} , K , t _ {n + 1}) - \Sigma ] - \lambda_ {i} (F _ {i} - S _ {i})}
$$

where the term  represents the sum $\begin{array} { r } { \sum _ { j = i + 1 } ^ { n } \lambda _ { j } ( F _ { j } - s _ { i } ) } \end{array}$ . This means that after choosing the usual centering condition for the binomial tree 

$$
s _ {i} ^ {2} = S _ {i} S _ {i + 1}
$$

we have all the elements to build the tree and deduce the implied distribution from the Arrow-Debreu prices. 

## Stability Issues

The local volatility models are very elegant and theoretically sound; however, they present in practice many stability issues. They are ill-posed inversion problems and are extremely sensitive to the input data.<sup>15</sup> This might introduce arbitrage opportunities and in some cases negative probabilities or variances. Derman and Kani suggest overwriting techniques to avoid such problems. 

Andersen [13] tries to improve this issue by using an implicit finite difference method; however, he recognizes that the negative variance problem could still happen. 

One way to make the results smoother is to use a constrained optimization. In other words, when trying to fit theoretical results $C _ { t b e o }$ to the market prices $C _ { m r k t } ,$ instead of minimizing 

$$
\sum_ {j = 1} ^ {N} \bigl (C _ {t h e o} \bigl (K _ {j} \bigr) - C _ {m r k t} \bigl (K _ {j} \bigr) \bigr) ^ {2}
$$

we could minimize 

$$
\lambda \frac {\partial \sigma}{\partial t} + \sum_ {j = 1} ^ {N} \bigl (C _ {t h e o} \bigl (K _ {j} \bigr) - C _ {m r k t} \bigl (K _ {j} \bigr) \bigr) ^ {2}
$$

where λ is a constraint parameter, which could also be interpreted as a Lagrange multiplier. However, this is an artificial way to smoothen the results and the real issue remains that, once again, we have an inversion problem that is inherently unstable. Furthermore, local volatility models imply that future implied volatility smiles will be flat relative to today’s, which is another limitation.<sup>16</sup> As we will see in the following section, stochastic volatility models offer more time-homogeneous volatility smiles. 

An alternative approach suggested in [16] would be to choose a prior risk-neutral distribution for the asset (based on a subjective view) and then minimize the relative entropy distance between the desired surface and this prior distribution. This approach uses the Kullback-Leibler distance (which we will discuss in the context of maximum likelihood estimation [MLE]) and performs the minimization via dynamic programming [35] on a tree. 

## Calibration Frequency

One of the most attractive features of local-vol models is their ability to match plain-vanilla puts and calls exactly. This will avoid arbitrage situations, or worse, market manipulations by traders to create “phantom” profits. As explained in Hull [147], these arbitrage-free models were developed by researchers with a single calibration (SC) methodology assumption. However, in practice, traders use them with a continual recalibration (CR) strategy. Indeed if they used the SC version of the model, significant errors would be introduced from one week to the following as shown by Dumas et al. [88]. However, once this CR version is used, there is no guarantee that the no-arbitrage property of the original SC model is preserved. Indeed the Dupire equation determines the marginal stock distribution at different points in time, but not the joint distribution of these stock prices. Therefore a path-dependent option could very well be mispriced, and the more path-dependent this option, the greater the mispricing. 

Hull [147] takes the example of a bet option, a compound option, and a barrier option. The bet option depends on the distribution of the stock at one point in time and therefore is correctly priced with a continually recalibrated local vol model. The compound option has some path dependency, and hence a certain amount of mispricing compared with a stochastic volatility (SV) model. Finally, the barrier option has a strong degree of path dependency and will introduce large errors. Note that this is due to the discrete nature of the data. Indeed, the maturities we have are limited. If we had all possible maturities in a continuous way, the joint distribution would be determined completely. Also, when interpolating in time, it is customary to interpolate upon the true variance $t \sigma _ { t } ^ { 2 }$ rather than the volatility $\sigma _ { t }$ given the equation 

$$
T _ {2} \sigma^ {2} (T _ {2}) = T _ {1} \sigma^ {2} (T _ {1}) + (T _ {2} - T _ {1}) \sigma^ {2} (T _ {1}, T _ {2})
$$

Interpolating upon the true variance will provide smoother results as shown by Jackel [152]. 

Proof: Indeed, calling for $0 \leq T _ { 1 } \leq T _ { 2 }$ , the spot return variances 

$$
\begin{array}{l} V a r (0, T _ {2}) = T _ {2} \sigma^ {2} (T _ {2}) \\ V a r (0, T _ {1}) = T _ {1} \sigma^ {2} (T _ {1}) \end{array}
$$

for a Brownian motion, we have independent increments and therefore a forward variance $V a r ( T _ { 1 } , T _ { 2 } )$ such that 

$$
\operatorname{Var} \left(0, T _ {1}\right) + \operatorname{Var} \left(T _ {1}, T _ {2}\right) = \operatorname{Var} \left(0, T _ {2}\right)
$$

which demonstrates the point. (QED) 

## STOCHASTIC VOLATILITY

Unlike nonparametric local volatility models, parametric stochastic volatility (SV) models define a specific stochastic differential equation for the unobservable instantaneous variance. As we shall see, the previously defined CEV model could be considered a special case of these models. 

## Stochastic Volatility Processes

The idea would be to use a different stochastic process for σ altogether. Making the volatility a deterministic function of the spot is a special “degenerate” two-factor, a natural generalization of which would precisely be to have two stochastic processes with an imperfect correlation.<sup>17</sup> 

Several different stochastic processes have been suggested for the volatility. A popular one is the Ornstein-Uhlenbeck (OU) process: 

$$
d \sigma_ {t} = - \alpha \sigma_ {t} d t + \beta d Z _ {t}\tag{1.24}
$$

where $\alpha$ and $\beta$ are two parameters, remembering the stock equation 

$$
d S _ {t} = \mu_ {t} S _ {t} d t + \sigma_ {t} S _ {t} d B _ {t}
$$

there is a (usually negative) correlation $\rho$ between $d Z _ { t }$ and $d B _ { t } ,$ , which can in turn be time or level dependent. Heston [134] and Stein [223] were among those who suggested the use of this process. Using Ito’s lemma, we can see that the stock-return variance $\nu _ { t } = \sigma _ { t } ^ { 2 }$ satisfies a square-root or Cox-Ingersoll-Ross (CIR) process 

$$
d \nu_ {t} = (\omega - \theta \nu_ {t}) d t + \xi \sqrt {\nu_ {t}} d Z _ {t}\tag{1.25}
$$

with $\omega = \beta ^ { 2 } , \theta = 2 \alpha$ , and $\xi = 2 \beta .$ 

Note that the OU process has a closed-form solution 

$$
\sigma_ {t} = \sigma_ {0} e ^ {- \alpha t} + \beta \int_ {0} ^ {t} e ^ {- \alpha (t - s)} d Z _ {s}
$$

which means that $\sigma _ { t }$ follows in law $\Phi \left( \sigma _ { 0 } e ^ { - \alpha t } , \frac { \beta ^ { 2 } } { 2 \alpha } \left( 1 - e ^ { - 2 \alpha t } \right) \right)$ , with  again the normal distribution. This was discussed in Fouque [104] and Shreve [218]. 

Heston and Nandi [137] show that this process corresponds to a special case of the general auto regressive conditional heteroskedasticity (GARCH) model, which we will discuss next. Another popular process is the GARCH (1,1) process, where we would have 

$$
d \nu_ {t} = (\omega - \theta \nu_ {t}) d t + \xi \nu_ {t} d Z _ {t}\tag{1.26}
$$

## GARCH and Diffusion Limits

The most elementary GARCH process, called GARCH(1,1), was developed originally in the field of econometrics by Engle [94] and Bollerslev [40] in a discrete framework. The stock discrete equation (1.3) could be rewritten by taking $\Delta t = 1$ and $\nu _ { n } = \sigma _ { n } ^ { 2 }$ as 

$$
\ln S _ {n + 1} = \ln S _ {n} + \left(\mu - \frac {1}{2} \nu_ {n + 1}\right) + \sqrt {\nu_ {n + 1}} B _ {n + 1}\tag{1.27}
$$

calling the mean adjusted return 

$$
u _ {n} = \ln \left(\frac {S _ {n}}{S _ {n - 1}}\right) - \left(\mu - \frac {1}{2} \nu_ {n}\right) = \sqrt {\nu_ {n}} B _ {n}\tag{1.28}
$$

the variance process in GARCH(1,1) is supposed to be 

$$
\nu_ {n + 1} = \omega_ {0} + \beta \nu_ {n} + \alpha u _ {n} ^ {2} = \omega_ {0} + \beta \nu_ {n} + \alpha \nu_ {n} B _ {n} ^ {2}\tag{1.29}
$$

where $\alpha$ and $\beta$ are weight parameters and $\omega _ { 0 }$ is a parameter related to the long-term variance.<sup>18</sup> 

Nelson [194] shows that as the time interval length decreases and becomes infinitesimal, Equation (1.29) becomes precisely the previously cited Equation (1.26). To be more accurate, there is a weak convergence of the discrete GARCH process to the continuous diffusion limit.<sup>19</sup> For a GARCH(1,1) continuous diffusion, the correlation between $d Z _ { t }$ and $d B _ { t }$ is zero. 

It might appear surprising that even if the GARCH(1,1) process has only one source of randomness, namely $B _ { n } ,$ , the continuous version has two independent Brownian motions. This is understandable if we consider $B _ { n }$ a standard normal random variable and $A _ { n } = B _ { n } ^ { 2 } - 1$ another random variable. It is fairly easy to see that $A _ { n }$ and $B _ { n }$ are uncorrelated even if $A _ { n }$ is a function of $B _ { n }$ . As we go toward the continuous version, we can use Donsker’s theorem,<sup>20</sup> by letting the time interval $\Delta t \to 0$ , to prove that we end up with two uncorrelated and therefore independent Brownian motions. This is a limitation of the GARCH(1,1) model–hence the introduction of the nonlinear asymmetric GARCH (NGARCH) model. 

Duan [83] attempts to explain the volatility smile by using the NGARCH process expressed by 

$$
\nu_ {n + 1} = \omega_ {0} + \beta \nu_ {n} + \alpha \big (u _ {n} - c \sqrt {\nu_ {n}} \big) ^ {2}\tag{1.30}
$$

where $c$ is a parameter to be determined. 

The NGARCH process was first introduced by Engle [97]. The continuous counterpart of NGARCH is the same equation (1.26), except unlike the equation resulting from GARCH(1,1) there is a nonzero correlation between the stock process and the volatility process. This correlation is created precisely because of the parameter c that was introduced, and is once again called the leverage effect. The parameter $c$ is sometimes referred to as the leverage parameter. 

We can find the following relationships between the discrete process and the continuous diffusion limit parameters by letting the time interval become infinitesimal 

$$
\begin{array}{l} \omega = \frac {\omega_ {0}}{d t ^ {2}} \\ \theta = \frac {1 - \alpha (1 + c ^ {2}) - \beta}{d t} \\ \xi = \alpha \sqrt {\frac {\kappa - 1 + 4 c ^ {2}}{d t}} \end{array}
$$

and the correlation between $d B _ { t }$ and $d Z _ { t }$ 

$$
\rho = \frac {- 2 c}{\sqrt {\kappa - 1 + 4 c ^ {2}}}
$$

where κ represents the Pearson kurtosis<sup>21</sup> of the mean adjusted returns $( u _ { n } )$ As we can see, the sign of the correlation $\rho$ is determined by the parameter c. 

Proof: A quick proof of the convergence to diffusion limit could be outlined as follows. Let us assume that $c = 0$ for simplicity; we therefore are dealing with the GARCH(1,1) case. As we saw 

$$
\nu_ {n + 1} = \omega_ {0} + \beta \nu_ {n} + \alpha \nu_ {n} B _ {n} ^ {2}
$$

therefore 

$$
\nu_ {n + 1} - \nu_ {n} = \omega_ {0} + \beta \nu_ {n} - \nu_ {n} + \alpha \nu_ {n} - \alpha \nu_ {n} + \alpha \nu_ {n} B _ {n} ^ {2}
$$

or 

$$
\nu_ {n + 1} - \nu_ {n} = \omega_ {0} - (1 - \alpha - \beta) \nu_ {n} + \alpha \nu_ {n} (B _ {n} ^ {2} - 1)
$$

Now, allowing the time-step $\Delta t$ to become variable and posing $Z _ { n } =$ $( B _ { n } ^ { 2 } - 1 ) / \sqrt { \kappa - 1 }$ 

$$
\nu_ {n + \Delta t} - \nu_ {n} = \omega \Delta t ^ {2} - \theta \Delta t \nu_ {n} + \xi \nu_ {n} \sqrt {\Delta t} Z _ {n}
$$

and annualizing $\nu _ { n }$ by posing $\nu _ { t } = \nu _ { n } / \Delta t$ , we shall have 

$$
\nu_ {t + \Delta t} - \nu_ {t} = \omega \Delta t - \theta \Delta t \nu_ {t} + \xi \nu_ {t} \sqrt {\Delta t} Z _ {n}
$$

and as $\Delta t \to 0 .$ , we get 

$$
d \nu_ {t} = (\omega - \theta \nu_ {t}) d t + \xi \nu_ {t} d Z _ {t}
$$

as claimed. (QED) 

Note that the discrete GARCH version of the square-root process (1.25 ) is 

$$
\nu_ {n + 1} = \omega_ {0} + \beta \nu_ {n} + \alpha (B _ {n} - c \sqrt {\nu_ {n}}) ^ {2}\tag{1.31}
$$

as Heston and Nandi show<sup>22</sup> in [137] (Figure 1.5). 

Also, note that having a diffusion process d $\begin{array} { r } { \mathrm { { ' } } \nu _ { t } = b ( \nu _ { t } ) d t + a ( \nu _ { t } ) d Z _ { t } } \end{array}$ we can apply an Euler approximation<sup>23</sup> to discretize and obtain a Monte Carlo process, such as $\nu _ { n + 1 } - \nu _ { n } = b ( \nu _ { n } ) \Delta t + a ( \nu _ { n } ) \sqrt { \Delta t } Z _ { n }$ . It is important to note that if we use a GARCH process and go to the continuous diffusion limit, and then apply an Euler approximation, we will not necessarily find the original GARCH process again. Indeed, there are many different ways to discretize the continuous diffusion limit and the GARCH process corresponds to one special way. In particular, if we use (1.31) and allow $\Delta t \to 0$ to get to the continuous diffusion limit, we shall obtain (1.25). As we will see later in the section on mixing solutions, we can then apply a discretization to this process and obtain a Monte Carlo simulation 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/0d7ff4395187acf3eb454c6be5432634cf6552e9c05b637d5da116056526618c.jpg)



FIGURE 1.5 The GARCH Monte Carlo Simulation with the Square-Root Model for SPX on February 12, 2002 with Index = $1107.50, 1 Month to Maturity. The Powell optimization method was used for least-square calibration.


$$
\nu_ {n + 1} = \nu_ {n} + (\omega - \theta \nu_ {n}) \Delta t + \xi \sqrt {\nu_ {n}} \sqrt {\Delta t} Z _ {n}
$$

which is again different from (1.31) but obviously has to be consistent in terms of pricing. However, we should know which method we are working with from the very beginning to perform our calibration on the corresponding specific process. 

Corradi [61] explains this in the following manner: The discrete GARCH model could converge either toward a two-factor continuous limit if one chooses the Nelson parameterization, or could very well converge to a onefactor diffusion limit if one chooses another parameterization. Furthermore, an appropriate Euler discretization of the one-factor continuous model will provide a GARCH discrete process, while as previously mentioned the discretization of the two-factor diffusion model provides a two-factor discrete process. This distinction is fundamental and could explain why GARCH and SV behave differently in terms of parameter estimation. 

## THE PRICING PDE UNDER STOCHASTIC VOLATILITY

A very important issue to underline here is that, because of the unhedgeable second source of randomness, the concept of market completeness is lost. 

We can no longer have a straightforward risk-neutral pricing. This is where the market price of risk will come into consideration. 

## The Market Price of Volatility Risk

Indeed, taking a more general form for the variance process 

$$
d \nu_ {t} = b (\nu_ {t}) d t + a (\nu_ {t}) d Z _ {t}\tag{1.32}
$$

as we previously said, using the Black-Scholes risk-neutrality argument, Equation (1.1) could be replaced with 

$$
d S _ {t} = (r _ {t} - q _ {t}) S _ {t} d t + \sigma_ {t} S _ {t} d B _ {t}\tag{1.33}
$$

This is equivalent to changing the probability measure from the real one to the risk-neutral one.<sup>24</sup> We therefore need to use (1.33) together with the risk-adjusted volatility process 

$$
d \nu_ {t} = \tilde {b} (\nu_ {t}) d t + a (\nu_ {t}) d Z _ {t}\tag{1.34}
$$

where 

$$
\tilde {b} (\nu_ {t}) = b (\nu_ {t}) - \lambda a (\nu_ {t})
$$

with $\lambda$ the market price of volatility risk. This quantity is closely related to the market price of risk for the stock $\lambda _ { e } = ( \mu - r ) / \sigma$ . Indeed, as Hobson [140] and Lewis [177] both show, we have 

$$
\lambda = \rho \lambda_ {e} + \sqrt {1 - \rho^ {2}} \lambda^ {*}\tag{1.35}
$$

where $\lambda ^ { * }$ is the market price of risk associated with d $B _ { t } - \rho d Z _ { t } ,$ , which can also be regarded as the market price of risk for the hedged portfolio. 

The passage from Equation (1.32) to Equation (1.34) and the introduction of the market price of volatility risk could also be explained by the Girsanov theorem, as was done for instance in Fouque [104]. 

It is important to underline the difference between the real and the riskneutral measures here. If we use historic stock prices together with the real stock-return drift $\mu$ to estimate the process parameters, we will obtain the real volatility drift b(v). An alternative method would be to estimate $\tilde { b } ( \nu )$ by using current option prices and performing a least-square estimation. These calibration methods will be discussed in detail in the following chapters. 

The risk-neutral version for a discrete NGARCH model would also involve the market price of risk and instead of the usual 

$$
\begin{array}{c} \ln S _ {n + 1} = \ln S _ {n} + \left(\mu - \frac {1}{2} v _ {n + 1}\right) + \sqrt {v _ {n + 1}} B _ {n + 1} \\ v _ {n + 1} = \omega_ {0} + \beta v _ {n} + \alpha v _ {n} (B _ {n} - c) ^ {2} \end{array}
$$

we would have 

$$
\begin{array}{c} \ln S _ {n + 1} = \ln S _ {n} + \left(r - \frac {1}{2} \nu_ {n + 1}\right) + \sqrt {\nu_ {n + 1}} \tilde {B} _ {n + 1} \\ \nu_ {n + 1} = \omega_ {0} + \beta \nu_ {n} + \alpha \nu_ {n} \big (\tilde {B} _ {n} - c - \lambda_ {e} \big) ^ {2} \end{array}\tag{1.36}
$$

where $\tilde { B } _ { n } = B _ { n } + \lambda _ { e } .$ , which could be regarded as the discrete version of the Girsanov theorem. Note that the market price of risk for the stock $\lambda _ { e }$ is not separable from the leverage parameter c in the above formulation. Duan shows in [84] and [86] that risk-neutral GARCH system (1.36) will indeed converge toward the continuous risk-neutral GARCH 

$$
\begin{array}{r l} & d S _ {t} = S _ {t} r d t + S _ {t} \sqrt {\nu_ {t}} d B _ {t} \\ & d \nu_ {t} = (\omega - \tilde {\theta} \nu_ {t}) d t + \xi \nu_ {t} d Z _ {t} \end{array}
$$

as we expected. 

## The Two-Factor PDE

From here, writing a two-factor PDE for a derivative security $f$ becomes a simple application of the two-dimensional Ito’s lemma. The PDE will $\mathrm { b e } ^ { 2 5 }$ 

$$
\begin{array}{r} r f = \frac {\partial f}{\partial t} + (r - q) S \frac {\partial f}{\partial S} + \frac {1}{2} \nu S ^ {2} \frac {\partial^ {2} f}{\partial S ^ {2}} + \tilde {b} (\nu) \frac {\partial f}{\partial \nu} \\ + \frac {1}{2} a ^ {2} (\nu) \frac {\partial^ {2} f}{\partial \nu^ {2}} + \rho a (\nu) \sqrt {\nu} S \frac {\partial^ {2} f}{\partial S \partial \nu} \end{array}\tag{1.37}
$$

Therefore, it is possible, after calibration, to apply a finite difference method<sup>26</sup> to the above PDE to price the derivative $f ( S , t , \nu )$ . An alternative would be to use directly the stochastic processes for $d S _ { t }$ and $d \nu _ { t }$ and apply a two-factor Monte Carlo simulation. Later in the chapter we will also mention other possible methods, such as the mixing solution or asymptotic approximations. 

Other possible approaches for incomplete markets and stochastic volatility assumption include super-replication and local risk minimization.<sup>27</sup> The super-replication strategy is the cheapest self-financing strategy with a terminal value no less than the payoff of the derivative contract. This technique was primarily developed by El-Karoui and Quenez in [91]. Local risk minimization involves a partial hedging of the risk. The risk is reduced to an “intrinsic component” by taking an offsetting position in the underlying security as usual. This method was developed by Follmer and Sondermann in [102]. 

## THE GENERALIZED FOURIER TRANSFORM

## The Transform Technique

One useful technique to apply to the PDE (1.37) is the generalized Fourier <sup>transform.28</sup> <sup>First,</sup> <sup>we</sup> <sup>can</sup> <sup>use</sup> <sup>the</sup> <sup>variable</sup> x = ln S <sup>in</sup> <sup>which</sup> <sup>case,</sup> <sup>using</sup> <sup>Ito’s</sup> lemma, Equation (1.37) could be rewritten as 

$$
r f = \frac {\partial f}{\partial t} + \left(r - q - \frac {1}{2} \nu\right) \frac {\partial f}{\partial x} + \frac {1}{2} \nu \frac {\partial^ {2} f}{\partial x ^ {2}} + \tilde {b} (\nu) \frac {\partial f}{\partial \nu} + \frac {1}{2} a ^ {2} (\nu) \frac {\partial^ {2} f}{\partial \nu^ {2}} + \rho a (\nu) \sqrt {\nu} \frac {\partial^ {2} f}{\partial x \partial \nu}\tag{1.38}
$$

Calling 

$$
\hat {f} (k, \nu , t) = \int_ {- \infty} ^ {+ \infty} e ^ {i k x} f (x, \nu , t) d x\tag{1.39}
$$

where $k$ is a complex $\mathrm { n u m b e r } , ^ { 2 9 } \hat { f }$ will be defined in a complex strip where the imaginary part of k is between two real numbers α and $\beta .$ Once $\hat { f }$ is suitably defined, meaning that $k _ { i } = \mathcal { T } ( k )$ (the imaginary part of k) is within the appropriate strip, we can write the inverse Fourier transform 

$$
f (x, \nu , t) = \frac {1}{2 \pi} \int_ {i k _ {i} - \infty} ^ {i k _ {i} + \infty} e ^ {- i k x} \hat {f} (k, \nu , t) d k\tag{1.40}
$$

where we are integrating for a fixed $k _ { i }$ parallel to the real axis. 

Each derivative satisfying (1.37) or equivalently (1.38) has a known payoff $G ( S _ { T } )$ at maturity. For instance, as we said before, a call option has a payoff $M A X ( 0 , S _ { T } - K )$ where K is the call strike price. It is easy to see that for $k _ { i } > 1$ the Fourier transform of a call option exists and the payoff transform is 

$$
- \frac {K ^ {i k + 1}}{k ^ {2} - i k}\tag{1.41}
$$

Proof: Indeed, we can write 

$$
\begin{array}{r l} \int_ {- \infty} ^ {+ \infty} e ^ {i k x} (e ^ {x} - K) ^ {+} d x & = \int_ {\ln K} ^ {+ \infty} e ^ {i k x} (e ^ {x} - K) d x \\ & = 0 - \left(\frac {K ^ {i k + 1}}{i k + 1} - K \frac {K ^ {i k}}{i k}\right) \\ & = - K ^ {i k + 1} \left(\frac {1}{i k + 1} - \frac {1}{i k}\right) = - K ^ {i k + 1} \frac {1}{k ^ {2} - i k} \end{array}
$$

as stated. (QED) 

The same could be applied to a put option or other derivative securities. In particular, a covered call (stock minus call) having a payoff $M I N ( S _ { T } , K )$ will have a transform for $0 < k _ { i } < 1$ equal to 

$$
\frac {K ^ {i k + 1}}{k ^ {2} - i k}\tag{1.42}
$$

Applying the transform to the PDE (1.38) and introducing $\tau = T - t$ and 

$$
\hat {b} (k, \nu , \tau) = e ^ {(r + i k (r - q)) \tau} \hat {f} (k, \nu , \tau)\tag{1.43}
$$

and posing $\begin{array} { r } { \begin{array} { r l r } { { 3 } 0 } & { { } c ( k ) = \frac { 1 } { 2 } ( k ^ { 2 } - i k ) } \end{array} } \end{array}$ , we get the new PDE equation 

$$
\frac {\partial \hat {b}}{\partial \tau} = \frac {1}{2} a ^ {2} (\nu) \frac {\partial^ {2} \hat {b}}{\partial \nu^ {2}} + (\tilde {b} (\nu) - i k \rho (\nu) a (\nu) \sqrt {\nu}) \frac {\partial \hat {b}}{\partial \nu} - c (k) \nu \hat {b}\tag{1.44}
$$

Lewis calls the fundamental transform a function $\hat { H } ( k , \nu , \tau )$ satisfying the PDE (1.44) and satisfying the initial condition $\hat { H } ( k , \nu , \tau = 0 ) = 1$ . If we know this fundamental transform, we can then multiply it by the derivative security’s payoff transform and then divide it by $e ^ { ( r + i k ( r - q ) ) { \dot { \tau } } }$ and apply the inverse Fourier technique by keeping $k _ { i }$ in an appropriate strip and finally get the derivative as a function of $x = \ln S$ 

## Special Cases

There are cases where the fundamental transform is known. The case of a constant (or deterministic) volatility is the most elementary one. Indeed, using (1.44) together with $d \nu _ { t } = 0 $ , we can easily find 

$$
\hat {H} (k, \nu , \tau) = e ^ {- c (k) \nu \tau}
$$

which is analytic in $k$ over the entire complex plane. Using the call payoff transform (1.41), we can rederive the Black-Scholes equation. The same can be done if we have a deterministic volatility $d \nu _ { t } = b ( \nu _ { t } ) d t$ by using the function $Y ( \nu , t )$ where d $Y = b ( Y ) d t .$ 

The square-root model (1.25) is another important case where $\hat { H } ( k , \nu , \tau )$ is known and analytic. We have for this process 

$$
d \nu_ {t} = (\omega - \theta \nu_ {t}) d t + \xi \sqrt {\nu_ {t}} d Z _ {t}
$$

or under the risk-neutral measure 

$$
d \nu_ {t} = (\omega - \tilde {\theta} \nu_ {t}) d t + \xi \sqrt {\nu_ {t}} d Z _ {t}
$$

with $\tilde { \theta } = ( 1 - \gamma ) \rho \xi + \sqrt { \theta ^ { 2 } - \gamma ( 1 - \gamma ) \xi ^ { 2 } }$ , where $\gamma \leq 1$ represents the riskaversion factor. 

For the fundamental transform, we get 

$$
\hat {H} (k, \nu , \tau) = \exp [ f _ {1} (t) + f _ {2} (t) \nu ]\tag{1.45}
$$

with 

$$
t = \frac {1}{2} \xi^ {2} \tau \quad \tilde {\omega} = \frac {2}{\xi^ {2}} \omega \quad \tilde {c} = \frac {2}{\xi^ {2}} c (k) \qquad \mathrm{and}
$$

$$
f _ {1} (t) = \left[ t g - \ln \left(\frac {1 - h e ^ {t d}}{1 - h}\right) \right] \tilde {\omega}
$$

$$
f _ {2} (t) = \left[ \frac {1 - e ^ {t d}}{1 - b e ^ {t d}} \right] g
$$

where 

$$
d = \sqrt {\bar {\theta} ^ {2} + 4 \tilde {c}} g = \frac {1}{2} (\bar {\theta} + d) h = \frac {\bar {\theta} + d}{\bar {\theta} - d}
$$

and 

$$
\bar {\theta} = \frac {2}{\xi^ {2}} \left[ (1 - \gamma + i k) \rho \xi + \sqrt {\theta^ {2} - \gamma (1 - \gamma) \xi^ {2}} \right]
$$

The above transform has a cumbersome expression, but it can be seen that it is analytic in k and therefore always exists. For a proof of the foregoing refer to Lewis [177]. 


TABLE 1.1 SPX Implied Surface as of 03/09/2004. T is the maturity and $M = K / S$ the inverse of the moneyness


<table><tr><td>T/M</td><td>0.70</td><td>0.80</td><td>0.85</td><td>0.90</td><td>0.95</td><td>1.00</td><td>1.05</td><td>1.10</td><td>1.15</td><td>1.20</td><td>1.30</td></tr><tr><td>1.000</td><td>24.61</td><td>21.29</td><td>19.73</td><td>18.21</td><td>16.81</td><td>15.51</td><td>14.43</td><td>13.61</td><td>13.12</td><td>12.94</td><td>13.23</td></tr><tr><td>2.000</td><td>21.94</td><td>18.73</td><td>18.68</td><td>17.65</td><td>16.69</td><td>15.79</td><td>14.98</td><td>14.26</td><td>13.67</td><td>13.22</td><td>12.75</td></tr><tr><td>3.000</td><td>20.16</td><td>18.69</td><td>17.96</td><td>17.28</td><td>16.61</td><td>15.97</td><td>15.39</td><td>14.86</td><td>14.38</td><td>13.96</td><td>13.30</td></tr><tr><td>4.000</td><td>19.64</td><td>18.48</td><td>17.87</td><td>17.33</td><td>16.78</td><td>16.26</td><td>15.78</td><td>15.33</td><td>14.92</td><td>14.53</td><td>13.93</td></tr><tr><td>5.000</td><td>18.89</td><td>18.12</td><td>17.70</td><td>17.29</td><td>16.88</td><td>16.50</td><td>16.13</td><td>15.77</td><td>15.42</td><td>15.11</td><td>14.54</td></tr><tr><td>6.000</td><td>18.46</td><td>17.90</td><td>17.56</td><td>17.23</td><td>16.90</td><td>16.57</td><td>16.25</td><td>15.94</td><td>15.64</td><td>15.35</td><td>14.83</td></tr><tr><td>7.000</td><td>18.32</td><td>17.86</td><td>17.59</td><td>17.30</td><td>17.00</td><td>16.71</td><td>16.43</td><td>16.15</td><td>15.88</td><td>15.62</td><td>15.15</td></tr><tr><td>8.000</td><td>17.73</td><td>17.54</td><td>17.37</td><td>17.17</td><td>16.95</td><td>16.72</td><td>16.50</td><td>16.27</td><td>16.04</td><td>15.82</td><td>15.40</td></tr></table>

The inversion of the Fourier transform for the square-root (Heston) model is a very popular and powerful approach. It is appealing because of its robustness and speed. The following example is based on SPX options as of 03/09/2004 expiring in 1 to 8 years from the calibration date (Tables 1.1 and 1.2). 

As we shall see further, the optimal Heston parameter set to fit this surface could be found via a least-square estimation approach and for the index at $S = \$ 1156.86$ we find the optimal parameters $\hat { \nu } _ { 0 } = 0 . 1 9 4 0$ and 

$$
\hat {\Psi} = (\hat {\omega}, \hat {\theta}, \hat {\xi}, \hat {\rho}) = (0. 0 5 2 0 4 2 3 3 2, 1. 8 4 0 8, 0. 4 7 1 0, - 0. 4 6 7 7)
$$

## THE MIXING SOLUTION

## The Romano-Touzi Approach

The idea of mixing solutions was probably presented for the first time by Hull and White [149] for a zero correlation case. Later, Romano and Touzi [209] generalized this approach for a correlated case. The basic idea is to separate the random processes of the stock and the volatility, integrate the stock process conditionally upon a given volatility, and finally end up with a one-factor problem. Let us be reminded of the two processes we had: 


TABLE 1.2 Heston Prices Fitted to the 03/09/2004 Surface


<table><tr><td>T / M</td><td>0.70</td><td>0.80</td><td>0.85</td><td>0.90</td><td>0.95</td><td>1.00</td><td>1.05</td><td>1.10</td><td>1.15</td><td>1.20</td><td>1.30</td></tr><tr><td>1.000</td><td>30.67</td><td>21.44</td><td>17.09</td><td>13.01</td><td>9.33</td><td>6.18</td><td>3.72</td><td>2.03</td><td>1.03</td><td>0.50</td><td>0.13</td></tr><tr><td>2.000</td><td>31.60</td><td>22.98</td><td>18.98</td><td>15.25</td><td>11.87</td><td>8.89</td><td>6.37</td><td>4.35</td><td>2.83</td><td>1.78</td><td>0.66</td></tr><tr><td>3.000</td><td>32.31</td><td>24.18</td><td>20.44</td><td>16.98</td><td>13.82</td><td>11.00</td><td>8.55</td><td>6.47</td><td>4.77</td><td>3.43</td><td>1.66</td></tr><tr><td>4.000</td><td>33.21</td><td>25.48</td><td>21.93</td><td>18.66</td><td>15.63</td><td>12.91</td><td>10.50</td><td>8.39</td><td>6.61</td><td>5.10</td><td>2.93</td></tr><tr><td>5.000</td><td>33.87</td><td>26.54</td><td>23.20</td><td>20.09</td><td>17.22</td><td>14.63</td><td>12.30</td><td>10.21</td><td>8.39</td><td>6.82</td><td>4.36</td></tr><tr><td>6.000</td><td>34.56</td><td>27.55</td><td>24.34</td><td>21.36</td><td>18.60</td><td>16.08</td><td>13.79</td><td>11.73</td><td>9.89</td><td>8.26</td><td>5.64</td></tr><tr><td>7.000</td><td>35.35</td><td>28.61</td><td>25.52</td><td>22.64</td><td>19.96</td><td>17.49</td><td>15.24</td><td>13.19</td><td>11.35</td><td>9.70</td><td>6.97</td></tr><tr><td>8.000</td><td>35.77</td><td>29.34</td><td>26.39</td><td>23.64</td><td>21.07</td><td>18.69</td><td>16.51</td><td>14.51</td><td>12.68</td><td>11.04</td><td>8.24</td></tr></table>

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/2f4569ad9868fab097c1dfd0752ff37dea21ee3cc1f75fa9c400ad8ce4c9afd8.jpg)



FIGURE 1.6 The SPX implied surface as of 03/09/2004. We can observe the negative skewness as well as the flattening of the slope with maturity.


$$
d S _ {t} = (r _ {t} - q _ {t}) S _ {t} d t + \sigma_ {t} S _ {t} d B _ {t}
$$

and 

$$
d \nu_ {t} = \tilde {b} (\nu_ {t}) d t + a (\nu_ {t}) d Z _ {t}
$$

under a risk-neutral measure. 

Given a correlation $\rho _ { t }$ between $d B _ { t }$ and $d Z _ { t } ,$ we can introduce the Brownian motion $d \mathbb { W } _ { t }$ independent of $d Z _ { t }$ and write the usual Cholesky<sup>31</sup> factorization: 

$$
d B _ {t} = \rho_ {t} d Z _ {t} + \sqrt {1 - \rho_ {t} ^ {2}} d W _ {t}
$$

We can then introduce the same $X _ { t } ~ = ~ \ln S _ { t }$ and write the new system of equations: 

$$
\begin{array}{l} {d X _ {t} = (r - q) d t + d Y _ {t} - \frac {1}{2} \big (1 - \rho_ {t} ^ {2} \big) \sigma_ {t} ^ {2} d t + \sqrt {1 - \rho_ {t} ^ {2}} \sigma_ {t} d W _ {t}} \\ {d Y _ {t} = - \frac {1}{2} \rho_ {t} ^ {2} \sigma_ {t} ^ {2} d t + \rho_ {t} \sigma_ {t} d Z _ {t}} \\ {d v _ {t} = \tilde {b} _ {t} d t + a _ {t} d Z _ {t}} \end{array}\tag{1.46}
$$

where, once again, the two Brownian motions are independent. 

It is now possible to integrate the stock process for a given volatility and end up with an expectation on the volatility process only. We can think of (1.46) as the limit of a discrete process, while the time step $\Delta t \to 0$ 

For a derivative security $f ( S _ { 0 } , \nu _ { 0 } , T )$ with a payo $\mathsf { f f } ^ { 3 2 } \ G ( S _ { T } )$ , using the bivariate normal density for two uncorrelated variables, we can write 

$$
\begin{array}{l}f (S _ {0}, \nu_ {0}, T) = e ^ {- r T} \mathbf {E} _ {0} [ G (S _ {T}) ]\\= e ^ {- r T} \lim _ {\Delta t \rightarrow 0} \int_ {- \infty} ^ {\infty} \dots \int_ {- \infty} ^ {\infty} G (S _ {T}) \prod_ {t = 0} ^ {T - \Delta t} \exp \left[ - \frac {1}{2} \left(Z _ {t} ^ {2} + W _ {t} ^ {2}\right)\right] \frac {d Z _ {t} d W _ {t}}{2 \pi}\end{array}\tag {1.47}
$$

If we know how to integrate the above over dW for a given volatility and we know the result $f ^ { * } ( S , \nu , T )$ (for instance, for a European call option, we know the Black-Scholes formula (1.6), there are many other cases where we have closed-form solutions), then we can introduce the auxiliary variables<sup>33</sup> 

$$
S ^ {e f f} = S _ {0} e ^ {Y _ {T}} = S _ {0} \exp \left(- \frac {1}{2} \int_ {0} ^ {T} \rho_ {t} ^ {2} \sigma_ {t} ^ {2} d t + \int_ {0} ^ {T} \rho_ {t} \sigma_ {t} d Z _ {t}\right)\tag{1.48}
$$

and 

$$
\nu^ {e f f} = \frac {1}{T} \int_ {0} ^ {T} (1 - \rho_ {t} ^ {2}) \sigma_ {t} ^ {2} d t\tag{1.49}
$$

and as Romano and Touzi prove in [209], we will have 

$$
f (S _ {0}, \nu_ {0}, T) = \mathbf {E} _ {0} [ f ^ {*} (S ^ {e f f}, \nu^ {e f f}, T) ]\tag{1.50}
$$

where this last expectation is being taken on d $\left. \vert Z _ { t } \right.$ only. Note that in the zero correlation case discussed by Hull and White [149] we have $S ^ { e f f } = S _ { 0 }$ and $\begin{array} { r } { \nu ^ { e f f } { = } \nu _ { T } = \frac { 1 } { T } \int _ { 0 } ^ { T } \sigma _ { t } ^ { 2 } d t , } \end{array}$ which makes the expression (1.50) a natural weighted average. 

## A One-Factor Monte Carlo Technique

As Lewis suggests, this will enable us to run a single-factor Monte Carlo simulation on the $d Z _ { t }$ and apply the known closed form for each simulated path. The method does suppose, however, that the payoff $G ( S _ { T } )$ does not depend on the volatility. Indeed, going back to (1.46) we can do a simulation on $Y _ { t }$ and $\nu _ { t }$ using the random sequence of $( Z _ { t } ) ;$ ; then, after one path is generated, we can calculate $S ^ { e f f } { = } S _ { 0 } \exp ( Y _ { T } )$ and $\begin{array} { r } { \nu ^ { e f f } { = } \frac { 1 } { T } \sum _ { t = 0 } ^ { T - \Delta t } ( 1 - \dot { \rho _ { t } ^ { 2 } } ) \nu _ { t } \Delta t } \end{array}$ and then apply the known closed form (e.g. Black-Scholes for a call or put) with $S ^ { e f f }$ and $\dot { \nu ^ { e f f } }$ . Repeating this procedure for a large number of times and averaging over the paths, as we usually do in Monte-Carlo methods, we will have $f ( S _ { 0 } , \nu _ { 0 } , T )$ . This will give us a way to calibrate the model parameters to the market data. For instance, using the square-root model 


Volatility Smile


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/3a2c9a56e8b7b1aad4e2fc1f1c6e9205749b5b6ca5056871c3896265695f6f37.jpg)



FIGURE 1.7 Mixing Monte Carlo Simulation with the Square-Root Model for SPX on February 12, 2002 with $\mathrm { I n d e x } = \$ 1107.50$ , 1 month and $7$ months to Maturity. The Powell optimization method was used for least-square calibration. As we can see, both maturities are fitted fairly well.


$$
d \nu_ {t} = (\omega - \theta \nu_ {t}) d t + \xi \sqrt {\nu_ {t}} d Z _ {t}
$$

we can estimate $\omega , \theta , \xi ,$ and $\rho$ from the market prices via a least-square estimation applied to theoretical prices obtained from the preceding Monte Carlo method (Figure 1.7). We can either use a single calibration and suppose we have time-independent parameters or perform one calibration per maturity. The single calibration method is known to provide a bad fit, hence the idea of adding jumps to the stochastic volatility process as described by Matytsin [187]. However, this method will introduce new parameters for calibration.<sup>34</sup> 

## THE LONG-TERM ASYMPTOTIC CASE

In this section we will discuss the case in which the contract time to maturity is very large, $t  \infty$ . We will focus on the special case of a square-root process because this is the model we will use in many cases. 

## The Deterministic Case

We shall start with the case of deterministic volatility and use that for the more general case of the stochastic volatility. 

We know that under the square-root model the variance follows 

$$
d \nu_ {t} = (\omega - \theta \nu_ {t}) d t + \xi \sqrt {\nu_ {t}} d Z _ {t}
$$

As an approximation, we can drop the stochastic term and obtain 

$$
\frac {d \nu_ {t}}{d t} = \omega - \theta \nu_ {t}
$$

which is an ordinary differential equation providing us immediately with 

$$
\nu_ {t} = \frac {\omega}{\theta} + \left(\nu - \frac {\omega}{\theta}\right) e ^ {- \theta t}\tag{1.51}
$$

where v is the initial variance for $t = 0$ 

Using the results from the fundamental transform for a covered call option and put-call parity, we have for $0 < k _ { i } < 1$ 

$$
c a l l (S, \nu , \tau) = S e ^ {- q \tau} - K e ^ {- r \tau} \frac {1}{2 \pi} \int_ {i k _ {i} - \infty} ^ {i k _ {i} + \infty} e ^ {- i k X} \frac {\hat {H} (k , \nu , \tau)}{k ^ {2} - i k} d k\tag{1.52}
$$

where $\tau = T - t$ and $\begin{array} { r } { X = \ln \bigl ( \frac { S e ^ { - q \tau } } { K e ^ { - r \tau } } \bigr ) } \end{array}$ represent the adjusted moneyness of the option. For the special $^ { \mathrm { { e } } } \mathrm { a t - t h e - m o n e y } ^ { \mathfrak { N } 3 5 }$ case, where $X = 0 .$ , we have 

$$
c a l l (S, \nu , \tau) = K e ^ {- r \tau} \left[ 1 - \frac {1}{2 \pi} \int_ {i k _ {i} - \infty} ^ {i k _ {i} + \infty} \frac {\hat {H} (k , \nu , \tau)}{k ^ {2} - i k} d k \right]\tag{1.53}
$$

As we previously said for a deterministic volatility case, we know the fundamental transform 

$$
\hat {H} (k, \nu , \tau) = \exp [ - c (k) U (\nu , \tau) ]
$$

With $\begin{array} { r } { U ( \nu , \tau ) = \int _ { 0 } ^ { \tau } \nu ( t ) d t } \end{array}$ and as before $c ( k ) = { \textstyle { \frac { 1 } { 2 } } } ( k ^ { 2 } - i k )$ , which in the special case of the square-root model (1.51), will provide us with 

$$
U (\nu , \tau) = \frac {\omega}{\theta} \tau + \left(\nu - \frac {\omega}{\theta}\right) \left(\frac {1 - e ^ {- \theta \tau}}{\theta}\right)
$$

This shows once again that $\hat { H } ( k )$ is analytic in $k$ over the entire complex plane. 

Now if we let $\tau \to \infty$ , we can write the approximation 

$$
\frac {c a l l (S , \nu , \tau)}{K e ^ {- r \tau}} \approx 1 - \frac {1}{2 \pi} \int_ {i k _ {i} - \infty} ^ {i k _ {i} + \infty} \exp \left[ - c (k) \frac {\omega}{\theta} \tau - c (k) \frac {1}{\theta} \left(\nu - \frac {\omega}{\theta}\right) \right] \frac {d k}{k ^ {2} - i k}\tag{1.54}
$$

We can either calculate the above integral exactly using the Black-Scholes theory, or take the minimum where $c ^ { \prime } ( k _ { 0 } ) = 0 ,$ meaning $\begin{array} { r } { k _ { 0 } = \frac { i } { 2 } , } \end{array}$ , and perform a Taylor approximation parallel to the real axis around the point $\begin{array} { r } { k = k _ { r } + \frac { i } { 2 } . } \end{array}$ which will give us 

$$
\frac {\operatorname{call} (S , \nu , \tau)}{K e ^ {- r \tau}} \approx 1 - \frac {2}{\pi} \exp \left(- \frac {\omega}{8 \theta} \tau\right) \exp \left[ - \frac {1}{8 \theta} \left(\nu - \frac {\omega}{\theta}\right) \right] \int_ {- \infty} ^ {\infty} \exp \left(- k _ {r} ^ {2} \frac {\omega}{2 \theta} \tau\right) d k _ {r}
$$

the integral being a Gaussian we will get the result 

$$
\frac {c a l l (S , \nu , \tau)}{K e ^ {- r \tau}} \approx 1 - \sqrt {\frac {8 \theta}{\pi \omega \tau}} \exp \left[ - \frac {1}{8 \theta} \left(\nu - \frac {\omega}{\theta}\right) \right] \exp \left(- \frac {\omega}{8 \theta} \tau\right)\tag{1.55}
$$

which finishes our deterministic approximation case. 

## The Stochastic Case

For the stochastic volatility case, Lewis uses the same Taylor expansion. He notices that for the deterministic case we had 

$$
\hat {H} (k, \nu , \tau) = \exp [ - c (k) U (\nu , \tau) ] \approx \exp [ - \lambda (k) \tau ] u (k, \nu)
$$

for $\tau \to \infty$ , where 

$$
\lambda (k) = c (k) \frac {\omega}{\theta}
$$

and 

$$
u (k, \nu) = \exp \left[ - c (k) \frac {1}{\theta} \left(\nu - \frac {\omega}{\theta}\right) \right]
$$

If we suppose that this identity holds for the stochastic volatility case as well, we can use the PDE (1.44) and interpret the result as an eigenvalueeigenfunction identity with the eigenvalue $\lambda ( k )$ and the eigenfunction $u ( k , \nu )$ 

This assumption is reasonable because the first Taylor approximation term for the stochastic process is deterministic. Indeed, introducing the operator 

$$
\Lambda (u) = - \frac {1}{2} a ^ {2} (\nu) \frac {d ^ {2} u}{d \nu^ {2}} - \left[ \tilde {b} (\nu) - i k \rho (\nu) a (\nu) \sqrt {\nu} \right] \frac {d u}{d \nu} + c (k) v u
$$

we have 

$$
\Lambda (u) = \lambda (k) u\tag{1.56}
$$

Now the idea would be to perform a Taylor expansion around the minimum $k _ { 0 }$ where $\lambda ^ { \prime } ( k _ { 0 } ) = 0 .$ . Lewis shows that such $k _ { 0 }$ is always situated on the imaginary axis. This property is referred to as the “ridge” property. 

The Taylor expansion along the real axis could be written as 

$$
\lambda (k) = \lambda (k _ {0} + k _ {r}) \approx \lambda (k _ {0}) + \frac {1}{2} k _ {r} ^ {2} \lambda^ {\prime \prime} (k _ {0})
$$

Note that we are dealing with a minimum, and therefore $\lambda ^ { \prime \prime } ( k _ { 0 } ) > 0 .$ . Using the above second-order approximation for $\lambda ( k )$ , we get 

$$
\frac {c a l l (S , \nu , \tau)}{K e ^ {- r \tau}} \approx 1 - \frac {u (k _ {0} , \nu)}{k _ {0} ^ {2} - i k _ {0}} \frac {1}{\sqrt {2 \pi \lambda^ {\prime \prime} (k _ {0}) \tau}} \exp [ - \lambda (k _ {0}) \tau ]
$$

We can then move from the special “at-the-money” case to the general case by reintroducing $\begin{array} { r } { X = \ln \bigl ( \frac { S e ^ { - q \tau } } { K e ^ { - r \tau } } \bigr ) } \end{array}$ , and we will finally obtain 

$$
\frac {c a l l (S , \nu , \tau)}{K e ^ {- r \tau}} \approx e ^ {X} - \frac {u (k _ {0} , \nu)}{k _ {0} ^ {2} - i k _ {0}} \frac {1}{\sqrt {2 \pi \lambda^ {\prime \prime} (k _ {0}) \tau}} \exp [ - \lambda (k _ {0}) \tau - i k _ {0} X ]\tag{1.57}
$$

which completes our determination of the asymptotic closed form in the general case. 

For the special case of the square-root model, taking the risk-neutral case $\gamma = 1$ , we $\mathrm { h a v e } ^ { 3 6 }$ 

$$
\lambda (k) = - \omega g ^ {*} (k) = \frac {\omega}{\xi^ {2}} \left[ \sqrt {(\theta + i k \rho \xi) ^ {2} + (k ^ {2} - i k) \xi^ {2}} - (\theta + i k \rho \xi) \right]
$$

which also allows us to calculate $\lambda ^ { \prime \prime } ( k )$ . Also 

$$
u (k, \nu) = \exp [ g ^ {*} (k) \nu ]
$$

where we use the notations from (1.45) and we pose 

$$
g ^ {*} = g - d
$$

The $k _ { 0 }$ such that $\lambda ^ { \prime } ( k _ { 0 } ) = 0$ is 

$$
k _ {0} = \frac {i}{1 - \rho^ {2}} \left(\frac {1}{2} - \frac {\rho}{\xi} \left[ \theta - \frac {1}{2} \sqrt {4 \theta^ {2} + \xi^ {2} - 4 \rho \theta \xi} \right]\right)
$$

which together with (1.57) provides us with the result for $c a l l ( S , \nu , \tau )$ in the asymptotic case under the square-root stochastic volatility model. 

Note that for $\xi \to 0$ and $\rho  0 ;$ , we find again the deterministic result $k _ { 0 }  { \frac { i } { 2 } } .$ 

## A Series Expansion on Volatility-of-Volatility

Another asymptotic approach for the stochastic volatility model suggested by Lewis $[ 1 7 7 ]$ is a Taylor expansion on the volatility-of-volatility. There are two possibilities for this: We can perform the expansion either for the option price $o r$ for the implied volatility directly. In what follows, we consider the former approach. Once again, we use the fundamental transform $H ( k , V , \tau )$ with $H ( k , V , 0 ) = 1$ and 

$$
\frac {\partial H}{\partial \tau} = \frac {1}{2} a ^ {2} (\nu) \frac {\partial^ {2} H}{\partial \nu^ {2}} + \left(\tilde {b} (\nu) - i k \rho (\nu) a (\nu) \sqrt {\nu}\right) \frac {\partial H}{\partial \nu} - c (k) \nu H
$$

and $c ( k ) = { \textstyle { \frac { 1 } { 2 } } } ( k ^ { 2 } - i k )$ . We then pose $a ( \nu ) = \xi \eta ( \nu )$ and expand $H ( k , V , \tau )$ on powers of $\xi$ and finally apply the inverse Fourier transform to obtain an expansion on the call price. 

With our usual notations $\begin{array} { r } { \tau = T - t , X = \ln ( \frac { S } { K } ) + ( r - q ) \tau } \end{array}$ and $Z ( V ) = V \tau ,$ the series will be 

$$
\begin{array}{l} C (S, V, \tau) = c _ {B S} (S, \nu , \tau) + \xi \tau^ {- 1} J _ {1} \tilde {R} _ {1 1} \frac {\partial c _ {B S} (S , \nu , \tau)}{\partial V} \\ \qquad + \xi^ {2} \bigg [ \tau^ {- 2} J _ {3} \tilde {R} _ {2 0} + \tau^ {- 1} J _ {4} \tilde {R} _ {1 2} + \frac {1}{2} \tau^ {- 2} J _ {1} ^ {2} \tilde {R} _ {2 2} \bigg ] \frac {\partial c _ {B S} (S , \nu , \tau)}{\partial V} + O (\xi^ {3}) \end{array}
$$

where $\nu ( V , \tau )$ is the deterministic variance 

$$
\nu (V, \tau) = \frac {\omega}{\theta} + \left(V - \frac {\omega}{\theta}\right) \left(\frac {1 - e ^ {- \theta \tau}}{\theta \tau}\right)
$$

and $\tilde { R } _ { p q } = R _ { p q } ( X , \nu ( V , \tau ) , \tau )$ with $R _ { \mathit { p q } }$ given polynomials of $( X , Z )$ of degree four at most, and $J _ { n } \mathbf { \dot { s } }$ known functions of $( V , \tau )$ 

The explicit expressions for all these functions are given in the third chapter of the Lewis book [177]. 

The obvious advantages of this approach are its speed and stability. The issue of lack of time homogeneity of the parameters $\Psi = ( \omega , \theta , \xi , \rho )$ could be addressed by performing one calibration per time interval. In this case, for each time interval $[ t _ { n } , t _ { n + 1 } ]$ we will have one set of parameters $\Psi _ { n } = ( \omega _ { n } , \theta _ { n } , \xi _ { n } , \rho _ { n } )$ and depending on what maturity T we are dealing with, we will use one or the other parameter set. 

We compare the values obtained from this series-based approach with those from a mixing Monte Carlo method in Figure 1.8. We are taking the example that Heston studied in [134]. The graph shows the difference $C ( S , V , \tau ) - c _ { B S } ( S , V , \tau )$ for a fixed $K = \$ 100$ and $\tau = 0 . 5 0$ year. The other inputs are $\omega = 0 . 0 2 , \theta = 2 . 0 0 , \xi = 0 . 1 0 , \rho = - 0 . 5 0 , V = 0 . 0 1 ,$ and $r = q = 0 .$ As we can see, the true value of the call is lower than the Black-Scholes value for the out-of-the-money (OTM) region. The higher ξ and $| \rho |$ are, the larger this difference will be. 

In Figures 1.9 and 1.10, we reset the correlation $\rho$ to zero to have a symmetric distribution, but we use a volatility-of-volatility of $\xi = 0 . 1 0$ and $\xi = 0 . 2 0$ respectively. As discussed, the parameter $\xi$ is the one creating the leptokurticity phenomenon. A higher volatility-of-volatility causes higher valuation for far-from-the-money options.<sup>37</sup> 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/c90b8984fb3a14b2e03717234ea0dc0dcb5f835f85944d321666374b200e56a1.jpg)



FIGURE 1.8 Comparing the Volatility-of-Volatility Series Expansion with the Monte Carlo Mixing Model. The graph shows the price difference $C ( S , V , \tau ) - c _ { B S } ( S , V , \tau )$ We are taking $\xi = 0 . 1 0$ and $\rho = - 0 . 5 0$ . This example was used in the original Heston paper.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/ad37646e3d5441eead76e5fefab22293412ccf80363ee3b7f9fa47edb181fdab.jpg)



FIGURE 1.9 Comparing the Volatility-of-Volatility Series Expansion with the Monte Carlo Mixing Model. The graph shows the price difference $C ( S , V , \tau ) - c _ { B S } ( S , V , \tau )$ We are taking $\xi = 0 . 1 0$ and $\rho = 0$ . This example was used in the original Heston paper.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/bb1bb217b64f667ec654472ce39874da281ce4c503d2df49028dfc893862ba0a.jpg)



FIGURE 1.10 Comparing the Volatility-of-Volatility Series Expansion with the Monte Carlo Mixing Model. The graph shows the price difference $C ( S , V , \tau )$ $- c _ { B S } ( S , V , \tau )$ . We are taking $\xi = 0 . 2 0$ and $\rho = 0 ,$ . This example was used in the original Heston paper.


Unfortunately, the foregoing series approximation becomes poor as soon as the volatility-of-volatility becomes larger than 0.40 and the maturity becomes of the order of 1 year. This case is not unusual at all and therefore makes the use of this method limited. This is why the method of choice remains the inversion of the Fourier transform, as previously described. 

## PURE-JUMP MODELS

## Variance Gamma

An alternative point of view is to drop the diffusion assumption altogether and replace it with a pure-jump process. Note that this is different from the jump-diffusion process previously discussed. Madan et al. suggested the following framework, called variance-gamma (VG) in [182]. We would have the log-normal-like stock process 

$$
d \ln S _ {t} = (\mu_ {S} + \omega) d t + X (d t; \sigma , \nu , \theta)
$$

where as before $\mu _ { S }$ is the real-world statistical drift of the stock log return and $\begin{array} { r } { \omega = \frac { 1 } { \nu } \ln ( 1 - \theta \nu - \sigma ^ { 2 } \nu / 2 ) } \end{array}$ 

As for $X ( d t ; \sigma , \nu , \theta )$ , it has the following meaning: 

$$
X (d t; \sigma , \nu , \theta) = B (\gamma (d t, 1, \nu); \theta , \sigma)
$$

where $B ( d t ; \theta , \sigma )$ would be a Brownian motion with drift θ and volatility σ. In other words 

$$
B (d t; \theta , \sigma) = \theta d t + \sigma \sqrt {d t} N (0, 1)
$$

and N(0- 1) is a standard Gaussian realization. 

The time interval at which the Brownian motion is considered is not dt but γ(dt- 1- ν) which is a random realization following a gamma distribution with a mean 1 and variance rate ν. The corresponding probability density function is 

$$
f _ {\nu} (d t, \tau) = \frac {\tau^ {\frac {d t}{\nu} - 1} e ^ {- \frac {\tau}{\nu}}}{\nu^ {\frac {d t}{\nu}} \Gamma (\frac {d t}{\nu})}
$$

where $\Gamma ( x )$ is the usual gamma function. 

Note that the stock log-return density could actually be integrated for the VG model, and the density of ln $( S _ { t } / S _ { 0 } )$ is known and could be implemented via $K _ { \alpha } ( x )$ , the modified Bessel function of the second kind. Indeed, calling $z = \ln ( S _ { k } / S _ { k - 1 } )$ and $b = t _ { k } { - } t _ { k - 1 }$ and posing $\begin{array} { r } { x _ { b } = z - \mu _ { S } b - \frac { b } { \nu } \ln ( 1 - \theta \nu - \sigma ^ { 2 } \nu / 2 ) } \end{array}$ we have 

$$
p (z | b) = \frac {2 \exp (\theta x _ {b} / \sigma^ {2})}{\nu^ {\frac {b}{\nu}} \sqrt {2 \pi} \sigma \Gamma (\frac {b}{\nu})} \left(\frac {x _ {b} ^ {2}}{2 \sigma^ {2} / \nu + \theta^ {2}}\right) ^ {\frac {b}{2 \nu} - \frac {1}{4}} K _ {\frac {b}{\nu} - \frac {1}{2}} \left(\frac {1}{\sigma^ {2}} \sqrt {x _ {b} ^ {2} (2 \sigma^ {2} / \nu + \theta^ {2})}\right)
$$

Moreover, as Madan et al. show, the option valuation under VG is fairly straightforward and admits an analytically tractable closed form that can be implemented via the above modified Bessel function of second kind and a degenerate hypergeometric function. All details are available in [182]. 

Remark on the Gamma Distribution The gamma cumulative distribution function (CDF) could be defined as 

$$
P (a, x) = \frac {1}{\Gamma (a)} \int_ {0} ^ {x} e ^ {- t} t ^ {a - 1} d t
$$

Note that with our notations 

$$
F _ {\nu} (h, x) = F (h, x, \mu = 1, \nu)
$$

with 

$$
F (b, x, \mu , \nu) = \frac {1}{\Gamma (\frac {\mu^ {2} b}{\nu})} \left(\frac {\mu}{\nu}\right) ^ {\frac {\mu^ {2} b}{\nu}} \int_ {0} ^ {x} e ^ {- \frac {\mu t}{\nu}} t ^ {\frac {\mu^ {2} b}{\nu} - 1} d t
$$

In other words 

$$
F (h, x, \mu , \nu) = P \left(\frac {\mu^ {2} h}{\nu}, \frac {\mu x}{\nu}\right)
$$

The behavior of this CDF is displayed in Figure 1.11 for different values of the parameter $a > 0$ and for $0 < x < + \infty$ 

Using the inverse of this CDF, we can have a simulated data set for the gamma law: 

$$
x ^ {(i)} = F _ {\nu} ^ {- 1} (b, \mathcal {U} ^ {(i)} [ 0, 1 ])
$$

with $1 \leq i \leq N _ { s i m s }$ and $\mathcal { U } ^ { ( i ) } [ 0 , 1 ]$ a uniform random realization between zero and one. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/0a10515362437be617b98ded2640e5fb53444cb9c79953daf19d9fd6b705e1be.jpg)



FIGURE 1.11 The Gamma Cumulative Distribution Function $P \left( \boldsymbol { a } , \boldsymbol { x } \right)$ for Various Values of the Parameter a. The implementation is based on code available in Numerical Recipes in C [204].


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/7e31075c3ceee1a842bb216ab4b3137519c1aa468e1a6b53f9096423c15b01ac.jpg)



FIGURE 1.12 The Modified Bessel Function of Second Kind for a Given Parameter. The implementation is based on code available in Numerical Recipes in C [204].


Stochastic Volatility vs. Time-Changed processes As mentioned in [23], this alternative formulation leading to time-changed processes is closely related to the previously discussed stochastic volatility approach in the following way. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/71569b858178da95ccfe7d3741e8af243998dace347bb1efa0e77c81ba2e34ec.jpg)



FIGURE 1.13 The Modified Bessel Function of Second Kind as a Function of the Parameter. The implementation is based on code available in Numerical Recipes in C [204].


Taking the foregoing VG stochastic differential equation 

$$
d \ln S _ {t} = (\mu_ {S} + \omega) d t + \theta \gamma (d t, 1, \nu) + \sigma \sqrt {\gamma (d t , 1 , \nu)} N (0, 1)
$$

one could consider $\sigma ^ { 2 } \gamma ( t , 1 , \nu )$ as the integrated variance and define $\nu _ { t } ( \nu )$ the instantaneous variance, as 

$$
\sigma^ {2} \gamma (d t, 1, \nu) = \nu_ {t} (\nu) d t
$$

in which case, we would have 

$$
\begin{array}{c} d \ln S _ {t} = (\mu_ {S} + \omega) d t + (\theta / \sigma^ {2}) \nu_ {t} (\nu) d t + \sqrt {\nu_ {t} (\nu) d t} N (0, 1) \\ = (\mu_ {S} + \omega + (\theta / \sigma^ {2}) \nu_ {t} (\nu)) d t + \sqrt {\nu_ {t} (\nu)} d Z _ {t} \end{array}
$$

where d $Z _ { t }$ is a Brownian motion. This last expression is a traditional stochastic volatility equation. 

## Variance Gamma with Stochastic Arrival

An extension of the VG model would be a variance gamma model with stochastic arrival (VGSA), which would include the volatility clustering effect. This phenomenon (also represented by GARCH) means that a high (low) volatility will be followed by a series of high (low) volatilities. In this approach, we replace the $d t$ in the previously defined $\textstyle f _ { \nu } ( d t , \tau )$ with $y _ { t } d t$ where $y _ { t }$ follows a square-root (CIR) process 

$$
d y _ {t} = \kappa (\eta - y _ {t}) d t + \lambda \sqrt {y _ {t}} d W _ {t}
$$

where the Brownian motion d $\mathbb { W } _ { t }$ is independent from other processes in the model. This is therefore a VG process in which the arrival time itself is stochastic. The mean reversion of the square-root process will cause the volatility persistence effect that is empirically observed. Note that (not counting $\mu _ { S } )$ the new model parameter set is $\Psi = ( \kappa , \eta , \lambda , \nu , \theta , \sigma )$ 

Option Pricing under VGSA The option pricing could be carried out via a Monte Carlo simulation algorithm under the risk-neutral measure, where, as before, $\mu _ { S }$ is replaced with $r - q$ . We first would simulate the path of $y _ { t }$ by writing 

$$
y _ {k} = y _ {k - 1} + \kappa (\eta - y _ {k - 1}) \Delta t + \lambda \sqrt {y _ {k - 1}} \sqrt {\Delta t} Z _ {k}
$$

then calculate 

$$
Y _ {T} = \sum_ {k = 0} ^ {N - 1} y _ {k} \Delta t
$$

and finally apply one-step simulations 

$$
T ^ {*} = F _ {\nu} ^ {- 1} \left(Y _ {T}, \mathcal {U} [ 0, 1 ]\right)
$$

and<sup>38</sup> 

$$
\ln S _ {T} = \ln S _ {0} + (r - q + \omega) T + \theta T ^ {*} + \sigma \sqrt {T ^ {*}} B _ {k}
$$

Note that we have two normal random variables $B _ { k } , Z _ { k }$ as well as a gammadistributed random variable $T ^ { * } ,$ and that they are all uncorrelated. Once the stock price $S _ { T }$ is properly simulated, we can calculate the option price as usual. 

The Characteristic Function As previously discussed, another way to tackle the option-pricing issue would be to use the characteristic functions. For ${ \mathrm { V G } } .$ the characteristic function is 

$$
\Psi (u, t) = \mathbf {E} [ e ^ {i u X (t)} ] = \left(\frac {1}{1 - i \frac {\nu}{\mu} u}\right) ^ {\frac {\mu 2}{\nu} t}
$$

Therefore the log-characteristic function could be written as 

$$
\psi (u, t) = \ln (\Psi (u, t)) = t \psi (u, 1)
$$

In other words 

$$
\mathbf {E} [ e ^ {i u X (t)} ] = \Psi (u, t) = \exp (t \psi (u, 1))
$$

Using which, the VGSA characteristic function becomes 

$$
\mathbf {E} \left[ e ^ {i u X (Y (t))} \right] = \mathbf {E} [ \exp (Y (t) \psi (u, 1)) ] = \phi (- i \psi (u, 1))
$$

with $\phi ( )$ the CIR characteristic function, namely 

$$
\phi (u _ {t}) = \mathbf {E} [ \exp (i u Y _ {t}) ] = A (t, u) \exp (B (t, u) y _ {0})
$$

where 

$$
\begin{array}{l} A (t, u) = \frac {\exp (\kappa^ {2} \eta t / \lambda^ {2})}{[ \cosh (\gamma t / 2) + \kappa / \gamma \sinh (\gamma t / 2) ] ^ {\frac {2 \kappa \eta}{\lambda^ {2}}}} \\ B (t, u) = \frac {2 i u}{\kappa + \gamma \coth (\gamma t / 2)} \end{array}
$$

and 

$$
\gamma = \sqrt {\kappa^ {2} - 2 \lambda^ {2} i u}
$$

This allows us to determine the VGSA characteristic function, which we can use to calculate options prices via numeric Fourier inversion as described in [48] and [51]. 

## Variance Gamma with Gamma Arrival Rate

For the variance gamma with gamma arrival rate (VGG), as before, the stock process under the risk-neutral framework is 

$$
d \ln S _ {t} = (r - q + \omega) d t + X (h (d t); \sigma , \nu , \theta)
$$

with $\begin{array} { r } { \omega = \frac { 1 } { \nu } \ln ( 1 - \theta \nu - \sigma ^ { 2 } \nu / 2 ) } \end{array}$ and 

$$
X (h (d t); \sigma , \nu , \theta) = B (\gamma (h (d t), 1, \nu); \theta , \sigma)
$$

and the general gamma cumulative distribution function for $\gamma ( b , \mu , \nu )$ is 

$$
F (\mu , \nu ; h, x) = \frac {1}{\Gamma \left(\frac {\mu^ {2} h}{\nu}\right)} \left(\frac {\mu}{\nu}\right) ^ {\frac {\mu^ {2} h}{\nu}} \int_ {0} ^ {x} e ^ {- \frac {\mu t}{\nu}} t ^ {\frac {\mu^ {2} h}{\nu} - 1} d t
$$

and here $b ( d t ) = d Y _ { t }$ with $Y _ { t }$ is also gamma-distributed 

$$
d Y _ {t} = \gamma (d t, \mu_ {a}, \nu_ {a})
$$

The parameter set is therefore $\Psi = ( \mu _ { a } , \nu _ { a } , \nu , \theta , \sigma )$ 

# The Inference Problem

In applying option pricing models, one always encounters the difficulty that the spot volatility and the structural parameters are unobservable. 

— Gurdip Bakshi, Charles Cao, and Zhiwu Chen 

## INTRODUCTION

Regardless of which specific model we are using, it seems that we cannot avoid the issue of calibration. There are two possible sets of data that we can use for estimating the model parameters: options prices and historic stock prices.<sup>1</sup> 

Using options prices via a least-square estimator (LSE) has the obvious advantage of guaranteeing that we will match the used option market prices within a certain tolerance. However, the availability of option data is typically limited, which would force us to use interpolation and extrapolation methods. These data manipulation approaches might deteriorate the quality and the smoothness of our inputs. More importantly, matching a set of plain-vanilla option prices does not necessarily mean that we would obtain the correct price for an exotic derivative. 

Using stock prices has the disadvantage of offering no guarantee of matching option prices. However, supposing that the model is right, we do have a great quantity of data input for calibration, which is a powerful argument in favor of this approach. 

It is important, however, to note that in using historic stock prices we are assuming that our time step t is small enough that we are almost in a continuous setting. Further, we are assuming the validity of the Girsanov theorem, which is applicable to a diffusion-based model. This also means we are implicitly assuming that the market price of volatility risk is stable and so are the risk-neutral volatility-drift parameters. 

More accurately, having for instance a real-world model 

$$
d \nu_ {t} = (\omega - \theta \nu_ {t}) d t + \xi \nu_ {t} ^ {p} d Z _ {t}
$$

with $p = 0 . 5$ corresponding to the Heston model, we know that the riskneutral volatility-drift parameter is 

$$
\theta^ {(r)} = \theta + \lambda \xi \nu_ {t} ^ {p - 1}
$$

As a result, supposing that $\theta ^ { ( r ) }$ is a stable (or even constant) parameter is equivalent to supposing that λ the market-price-of-volatility-risk<sup>2</sup> verifies 

$$
\lambda = \phi \nu_ {t} ^ {1 - p}
$$

with $\phi$ a constant coefficient. The implication of this assumption for a model with a real-world parameter set $\Psi = ( \omega , \theta , \xi , \rho )$ and a risk-neutral counterpart $\Psi ^ { ( r ) } = ( \omega ^ { ( r ) } , \hat { \theta ^ { ( r ) } } , \xi ^ { ( r ) } , \rho ^ { ( r ) } )$ is 

$$
\begin{array}{r} \xi = \xi^ {(r)} \\ \rho = \rho^ {(r)} \\ \omega = \omega^ {(r)} \\ \theta = \theta^ {(r)} - \phi \end{array}
$$

Let us insist on the fact that the above assumption<sup>3</sup> is valid only for a diffusion-based model. For some non-Gaussian pure-jump models, such as VGG, we lose the comparability between the statistical and the riskneutral parameters. We could instead use the stock-price time series to determine the statistical density $p ( z )$ on the one hand, use the options prices to determine the risk-neutral density $q ( z )$ on the other, and calculate the ratio $r ( z ) = \phi ( z ) / q ( z )$ corresponding to the Radon-Nikodym derivative of the two measures for this model. 

The central question of this chapter is therefore the inference of the parameters embedded in a stochastic volatility model. The logical subdivisions of the problem are summarized as follows. 

1. Cross-Sectional vs. Time Series: The former uses options prices at a given point in time, and the latter a series of the underlying prices for a given period. As mentioned earlier, the former provides an estimation of the parameters in the risk-neutral universe and the latter estimation takes place in the statistical universe. 

2. Classical vs. Bayesian: Using time series, one could suppose that there exists an unknown but fixed set of parameters and try to estimate them as closely as possible. This is a classical (frequentist) approach. Alternatively, one could use a Bayesian approach, in which the parameters are supposed to be random variables and have their prior distributions that one can update via the observations. 

3. Learning vs. Likelihood Maximization: Under the classical hypothesis, one could try to estimate the instantaneous variance together with the fixed parameters, which corresponds to a learning process. A more robust way would be to estimate the likelihood function and maximize it over all the possible values of the parameters. 

4. Gaussian vs. Non-Gaussian: In any of the preceding approaches, the stochastic volatility (SV) model could be diffusion based or not. As we will see further, this will affect the actual estimation methodology. Among the Gaussian SV models we consider are Heston, GARCH, and 3/2. Among the Non-Gaussian ones are Bates, VGSA, and VGG. 

5. State-Space Representation: For each of the above approaches and for each SV model, we have a number of ways of choosing a state and represent the instantaneous variance as well as the spot price. Needless to say, a more parsimonious and lower-dimension state is preferable. 

6. Diagnostics and Sampling Distribution: Once the inference process is finished, one has to verify its accuracy via various tests. Quantities such as MPE, RMSE, Box-Ljung, or $\chi ^ { 2 }$ numbers correspond to some of the possible diagnostics. Observing the sampling distribution over various paths is another way of checking the validity of the inference methodology. 

Finally, it is worth noting that our entire approach is based on parametric stochastic volatility models. This model class is more restrictive than the nonor semiparametric; however, it has the advantage of offering the possibility of a direct interpretation of the resulting parameters. 

## USING OPTION PRICES

Using a set of current vanilla option prices, we can perform an LSE and assess the risk-neutral model parameters. Taking a set of J strike prices $K _ { j } { ' } \mathbf { s }$ with their corresponding option prices $C _ { m k t } ( K _ { j } )$ for a given maturity, we would try to minimize 

$$
\sum_ {j = 1} ^ {J} (C _ {m o d e l} (K _ {j}) - C _ {m k t} (K _ {j})) ^ {2}
$$

The minimization<sup>4</sup> could, for example, be done via the direction set (Powell) method, the conjugate gradient (Fletcher-Reeves-Polak-Ribiere) method, or the Levenberg-Marquardt (LM) method. We will now briefly describe the Powell optimization algorithm. 

## Direction Set (Powell) Method

The optimization method we will use later is the direction set (Powell) method and does not require any gradient or Hessian computation.<sup>5</sup> This is a quadratically convergent method producing mutually conjugate directions. 

Most multi dimensional optimization algorithms require a one-dimensional line minimization routine that does the following: Given as input the vectors P and n and the function $f ,$ find the scalar λ that minimizes $f ( \mathbf { P } + \lambda \mathbf { n } )$ , and then replace P with P λn and n with λn. The idea would be to take a set of directions that are as noninterfering as possible in order to avoid spoiling one minimization with the subsequent one. This way an interminable cycling through the set of directions will not occur. This is why we seek conjugate directions. Calling the function to be minimized $f ( \mathbf { x } )$ , with x a vector of dimension N, we can write the second-order Taylor expansion around a particular point P 

$$
f (\mathbf {x}) \approx f (\mathbf {P}) + \nabla f (\mathbf {P}) \mathbf {x} + \frac {1}{2} \mathbf {x} \mathbf {H} \mathbf {x}
$$

where $\begin{array} { r } { \mathbf { H } _ { i j } = \frac { \partial ^ { 2 } f } { \partial x _ { i } \partial x _ { j } } } \end{array}$ is the Hessian matrix of the function at point P. We therefore have for the variation of the gradient $\delta ( \nabla f ) = \mathbf { H } \delta \mathbf { x }$ , and, in order to have a noninterfering new direction, we choose v such that the motion along v remains perpendicular to our previous direction u 

$$
\mathbf {u} \delta (\nabla f) = \mathbf {u H v} = 0
$$

In this case, the directions u and v are said to be conjugate. 

Powell suggests a quadratically convergent method that produces a set of N mutually conjugate directions. The following description is taken from Press [204], where the corresponding source code could be found as well. 

1. Initialize the set of directions $\mathbf { u } _ { i }$ to the basis vectors for $i = 1 , . . . , N$ 

2. Save the starting point as ${ \bf P } _ { 0 }$ 

3. Move $\mathbf { P } _ { i - 1 }$ to the minimum along direction $\mathbf { u } _ { i }$ and call it $\mathbf { P } _ { i }$ 

4. Set $\mathbf { u } _ { i } \ \mathbf { t o } \ \mathbf { u } _ { i + 1 }$ for $i = 1 , . . . , N - 1$ and set $\mathbf { u } _ { N }$ to $\mathbf { P } _ { N } - \mathbf { P } _ { 0 }$ 

5. Move ${ \bf P } _ { N }$ to the minimum along $\mathbf { u } _ { N }$ and call this point ${ \bf P } _ { 0 }$ , and go back to Step 2 

For a quadratic form, k iterations of this algorithm will produce a set of directions whose last k members are mutually conjugate. The idea is to repeat the steps until the function stops decreasing. However, this procedure tends to produce directions that are linearly dependent and therefore provides us with the minimum only over a sub space —hence—the idea of discarding the direction along which $f$ makes the largest decrease. This seems paradoxical; we are dropping our best direction in the new iteration. However, this is the best chance of avoiding a buildup of linear dependence. 

In what follows we apply the Powell algorithm to SPX options valued via the mixing Monte Carlo method. 

## Numeric Tests

We apply the Powell algorithm to SPX options valued via the mixing Monte Carlo method. The optimization is performed across close-to-the-money strike prices as of $t _ { 0 } ~ = ~ 0 5 / 2 1 / 2 0 0 2$ with the index $S _ { 0 } = 1 0 7 9 . 8 8$ and maturities $T = 0 8 / 1 7 / 2 0 0 2$ $T = 0 9 / 2 1 / 2 0 0 2$ $T = 1 2 / 2 1 / 2 0 0 2$ and $^ T =$ 03/22/2003 (Figures 2.1 through 2.5). 

As we see in Table 2.1, the estimated parameters are fairly stable for different maturities and therefore the stochastic volatility model seems to be fairly time homogeneous. 

## The Distribution of the Errors

Because the parameter set  contains only a few elements and we can have many options prices, it is clear that the matching of the model and market prices is not perfect. Thus, we observe the distribution of the errors 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/f3ca7ebb1bd94cf51f436e9154a8f33250c151dbceec31c7e74e31d26ab8a243.jpg)



FIGURE 2.1 The S&P 500 Volatility Surface as of 05/21/2002 with Index $1079.88. The surface will be used for fitting via the direction set (Powell) optimization algorithm applied to a square-root model implemented with a one-factor Monte Carlo mixing method.



Volatility Smile Fitting


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/960a5cc16bdb574f707fad59f36cf7b4eb07f21ad916e7c8469cadbc9cf1e1cb.jpg)



FIGURE 2.2 Mixing Monte Carlo Simulation with the Square-Root Model for SPX on 05/21/2002 with Index $1079.88, Maturity 08/17/2002. Powell (direction set) optimization method was used for least-square calibration. Optimal parameters $\hat { \omega } =$ 0.081575, $\hat { \theta } = 3 . 3 0 8 0 2 3$ 2 $\hat { \xi } = 0 . 2 6 8 1 5 1$ ， $\hat { \rho } = - 0 . 9 9 9 9 9 9 9$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/e3551764f4f103a44cfa3ad6a8c8138c5e59cea5482eb4dd9519d8809987a5c7.jpg)



FIGURE 2.3 Mixing Monte Carlo Simulation with the Square-Root Model for SPX on 05/21/2002 with Index $1079.88, Maturity 09/21/2002. Powell (direction set) optimization method was used for least-square calibration. Optimal parameters $\hat { \omega } =$ 0.108359, θ<sup>ˆ</sup> 3.798900, <sup>ˆ</sup>ξ 0.242820, ρˆ 0.999830.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/35a204e1333b07cfff75b567d9678e69952358fbd36ed86b7ecba57af873118b.jpg)



FIGURE 2.4 Mixing Monte Carlo Simulation with the Square-Root Model for SPX on 05/21/2002 with Index $1079.88, Maturity 12/21/2002. Powell (direction set) optimization method was used for least-square calibration. Optimal parameters $\hat { \omega } = 0 . 1 2 6 5 1 9 , \hat { \theta } = 3 . 4 7 3 9 1 0 , \hat { \xi } = 0 . 2 2 2 5 3 2 , \hat { \rho } = - 0 . 9 9 9 9 9 1$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/1d783385de8cb40f3dbb8b7fc197513b58ec217ad0b0cb17170744b197e90958.jpg)



FIGURE 2.5 Mixing Monte-Carlo Simulation with the Square-Root Model for SPX on 05/21/2002 with Index $1079.88, Maturity 03/22/2003. Powell (direction set) optimization method was used for least-square calibration. Optimal parameters $\hat { \omega } =$ 0.138687, $\hat { \theta } = 3 . 4 9 7 7 7 9$ , <sup>ˆ</sup>ξ 0.180010, ρˆ 1.000000.


$$
C _ {m k t} (K _ {j}) = C _ {m o d e l} (K _ {j}, \hat {\Psi}) \exp \left\{- \frac {1}{2} \Upsilon^ {2} + \Upsilon \mathcal {N} ^ {(j)} (0, 1) \right\}
$$

with $1 \leq j \leq J$ and ϒ the error standard deviation and $\hat { \Psi }$ the optimal parameter set. As usual, $\mathcal { N } ( 0 , 1 )$ is the standard normal distribution. Note that our previously discussed LSE approach is not exactly equivalent to the maximization of a likelihood function based on the above distribution because the latter would correspond to the minimization of the sum of the squared log returns. 


TABLE 2.1 The Estimation is Performed for SPX on $t = 0 5 / 2 1 / 2 0 0 2$ with Index $= \$ 1079.88$ for Different Maturities T.


<table><tr><td>T</td><td><eq>\hat{\omega}</eq></td><td><eq>\hat{\theta}</eq></td><td><eq>\hat{\xi}</eq></td><td><eq>\hat{\rho}</eq></td></tr><tr><td>08172002</td><td>0.081575</td><td>3.308023</td><td>0.268151</td><td>-0.999999</td></tr><tr><td>09212002</td><td>0.108359</td><td>3.798900</td><td>0.242820</td><td>-0.999830</td></tr><tr><td>12212002</td><td>0.126519</td><td>3.473910</td><td>0.222532</td><td>-0.999991</td></tr><tr><td>03222003</td><td>0.138687</td><td>3.497779</td><td>0.180010</td><td>-1.000000</td></tr></table>

A good bias test would be to check for the predictability of the errors. For this, one could run a regression of the error 

$$
e _ {j} = C _ {m k t} (K _ {j}) - C _ {m o d e l} (K _ {j}, \hat {\Psi})
$$

on a few factors corresponding, for instance, to moneyness or maturity. A low $R ^ { 2 }$ for the regression would prove that the model errors are not predictable and there is no major bias. For a detailed study, see [182] for instance. 

## USING STOCK PRICES

## The Likelihood Function

If, as in the previous section, we use European options with a given maturity T and with different strike prices, then we will be estimating 

$$
q (S _ {T} | S _ {0}; \Psi)
$$

which corresponds to the risk-neutral density, given a known current stock price $S _ { 0 }$ and given a constant parameter set . As discussed, least-squares estimation (LSE) is used to find the best guess for the unknown ideal parameter set. Alternatively, if we use a time series of stock prices $( S _ { t } ) _ { 0 \leq t \leq T } ,$ we would be dealing with the joint probability 

$$
p (S _ {1}, \dots , S _ {T} | S _ {0}; \Psi)
$$

which we can rewrite as 

$$
p (S _ {1}, \dots , S _ {T} | S _ {0}; \Psi) = \prod_ {t = 1} ^ {T} p (S _ {t} | S _ {t - 1}, \dots , S _ {0}; \Psi)
$$

It is this joint probability that is commonly referred to as the likelihood function ${ \cal L } _ { 0 : T } ( \Psi )$ . Maximizing the likelihood over the parameter set  would provide us with the best parameter set for the statistical density $p ( S _ { T } | S _ { 0 } ; \Psi )$ Note that we are using a classical (frequentist) approach, in which we assume that the parameters are unknown but are fixed over [0 T ]. In other words, we would be dealing with the same parameter set for any of the $p ( S _ { t } | S _ { t - 1 } , . . . , S _ { 0 } ;$ ) with $1 \leq t \leq T$ 

It is often convenient to work with the log of the likelihood function since this will produce a sum 

$$
\ln L _ {0: T} (\Psi) = \sum_ {t = 1} ^ {T} \ln p (S _ {t} | S _ {t - 1},..., S _ {0}; \Psi)
$$

The Justification for the MLE As explained, for instance, in [100], one justification of the maximization of the (log) likelihood function comes from the Kullback-Leibler (KL) distance. The KL distance is defined $\boldsymbol { \mathsf { a s } } ^ { 6 }$ 

$$
d (p ^ {*}, p) = \int p ^ {*} (x) \left(\ln p ^ {*} (x) - \ln p (x)\right) d x
$$

where $p ^ { * } ( x )$ is the ideal density, and $p ( x )$ is the density under estimation. We can write 

$$
d (p ^ {*}, p) = \mathbf {E} ^ {*} \ln \left(p ^ {*} (x) / p (x)\right)
$$

Note that using the Jensen (log convexity) inequality 

$$
d (p ^ {*}, p) = - \mathbf {E} ^ {*} \ln \left(p (x) / p ^ {*} (x)\right) \geq - \ln \left(\mathbf {E} ^ {*} (p (x) / p ^ {*} (x))\right)
$$

so 

$$
d (p ^ {*}, p) \geq - \ln \int p ^ {*} (x) p (x) / p ^ {*} (x) d x = 0
$$

and $d ( p , p ^ { * } ) = 0$ if and only if $\boldsymbol { p } = \boldsymbol { p } ^ { * }$ , which confirms that $d ( . , . )$ is a distance. Now minimizing $d ( p , p ^ { * } )$ over $p ( \ v u )$ would be equivalent to minimizing the term 

$$
- \int p ^ {*} (x) \ln p (x) d x
$$

since the rest of the expression depends on $p ^ { * } ( \ u )$ only. This latter expression could be written in the discrete framework, having $T$ observations $S _ { 1 } , . . . , S _ { T }$ as 

$$
- \sum_ {t = 1} ^ {T} \ln p (S _ {t})
$$

because the observations are by assumption distributed according to the ideal $p ^ { * } ( \ u )$ . This justifies our maximizing 

$$
\prod_ {t = 1} ^ {T} p (S _ {t})
$$

Note that in a pure parameter estimation, this would be the MLE approach. However, the minimization of the KL distance is more general and can allow for model identification. 

Maximum likelihood estimation has many desirable asymptotic attributes as explained, for example, in [127]. Indeed, ML estimators are consistent and converge to the right parameter set as the number of observations increases. They actually reach the lower bound for the error, referred to as the Cramer-Rao bound, which corresponds to the inverse of the Fisher information matrix. 

Calling the first derivative of the log likelihood the score function 

$$
b (\Psi) = \frac {\partial \ln L _ {0 : T} (\Psi)}{\partial \Psi}
$$

it is known that MLE could be interpreted as a special case of the general method of moments (GMM), where the moment $g ( \Psi )$ such that 

$$
\mathbf {E} [ g (\Psi) ] = 0
$$

is simply taken to be the above score function. Indeed we would then have 

$$
\mathbf {E} [ h (\Psi) ] = \int \frac {\partial \ln L _ {0 : T} (\Psi)}{\partial \Psi} L _ {0: T} (\Psi) d z _ {0: T} = 0
$$

which means that 

$$
\int \frac {\partial L _ {0 : T} (\Psi)}{\partial \Psi} d z _ {0: T} = 0
$$

as previously discussed in the MLE. 

Note that taking the derivative of the above with respect to the parameter set (using one-dimensional notations for simplicity) 

$$
\int \frac {\partial}{\partial \Psi} \left(h (\Psi) L _ {0: T} (\Psi)\right) d z _ {0: T} = 0
$$

which will give us 

$$
\begin{array}{r} \int \frac {\partial^ {2} \ln L _ {0 : T} (\Psi)}{\partial \Psi^ {2}} L _ {0: T} (\Psi) d z _ {0: T} = - \int \frac {\frac {\partial L _ {0 : T} (\Psi)}{\partial \Psi}}{L _ {0 : T} (\Psi)} \frac {\partial L _ {0 : T} (\Psi)}{\partial \Psi} d z _ {0: T} \\ = - \int \left(\frac {\partial \ln L _ {0 : T} (\Psi)}{\partial \Psi}\right) ^ {2} L _ {0: T} (\Psi) d z _ {0: T} \end{array}
$$

meaning that 

$$
\mathcal {J} = - E \left[ \frac {\partial^ {2} \ln L _ {0 : T} (\Psi)}{\partial \Psi^ {2}} \right] = E \left[ \left(\frac {\partial \ln L _ {0 : T} (\Psi)}{\partial \Psi}\right) ^ {2} \right]
$$

which is referred to as the information matrix identity. $\operatorname { A s }$ previously stated, asymptotically we have for the optimal parameter set $\Psi$ and the ideal $\Psi ^ { * }$ 

$$
\hat {\Psi} - \Psi^ {*} \sim \mathcal {N} (0, \mathcal {J} ^ {- 1})
$$

Likelihood Evaluation and Filtering For GARCH models, the likelihood is known under an integrated form. Indeed, calling $\boldsymbol { u } _ { t }$ the mean-adjusted stock return, $\nu _ { t }$ the variance, and $( B _ { t } )$ a Gaussian sequence, we have for any GARCH model 

$$
u _ {t} = b (\nu_ {t}, B _ {t})
$$

and 

$$
\nu_ {t} = f (\nu_ {t - 1}, u _ {t - 1}; \Psi)
$$

where $f ( )$ and $b ( \ u )$ are two deterministic functions. This will allow us to directly determine and optimize<sup>7</sup> 

$$
L _ {1: T} (\Psi) \propto - \sum_ {t = 1} ^ {T} \ln (\nu_ {t}) + \frac {u _ {t} ^ {2}}{\nu_ {t}}
$$

This is possible because GARCH models have one source of randomness and there is a time shift between the variance and the spot equations. 

Unlike GARCH, most stochastic volatility models have two (imperfectly correlated) sources of randomness $( B _ { t } )$ and $( Z _ { t } )$ and have equations of the form 

$$
u _ {t} = b (\nu_ {t}, B _ {t})
$$

$$
\nu_ {t} = f (\nu_ {t - 1}, Z _ {t}; \Psi)
$$

which means that the likelihood function is not directly known under an integrated form, and we need filtering techniques for its estimation and optimization. 

Another justification for filtering is its application to parameter learning. As we shall see, in this approach we use the joint distribution of the hidden state and the parameters. In order to obtain the optimal value of the hidden state $\nu _ { t }$ given all the observations $z _ { 1 : t } ,$ we need to use a filter. 

## Filtering

The idea here is to use the filtering theory for the estimation of stochastic volatility model parameters. What we are trying to do is to find the probability density function (pdf) corresponding to a state $x _ { k }$ at time step k given all the observations $z _ { 1 : k }$ up to that time. Looking for the pdf $\begin{array} { r } { p ( x _ { k } | z _ { 1 : k } ) } \end{array}$ , we can proceed in two stages. 

1. First we can write the time update iteration by applying the Chapman-Kolmogorov equation<sup>8</sup> 

$$
\begin{array}{c} p (x _ {k} | z _ {1: k - 1}) = \int p (x _ {k} | x _ {k - 1}, z _ {1: k - 1}) p (x _ {k - 1} | z _ {1: k - 1}) d x _ {k - 1} \\ = \int p (x _ {k} | x _ {k - 1}) p (x _ {k - 1} | z _ {1: k - 1}) d x _ {k - 1} \end{array}
$$

by using the Markov property. 

2. Following this, for the measurement update we use the Bayes rule 

$$
p (x _ {k} | z _ {1: k}) = \frac {p (z _ {k} | x _ {k}) p (x _ {k} | z _ {1 : k - 1})}{p (z _ {k} | z _ {1 : k - 1})}
$$

where the denominator $p ( z _ { k } | z _ { 1 : k - 1 } )$ could be written as 

$$
p (z _ {k} | z _ {1: k - 1}) = \int p (z _ {k} | x _ {k}) p (x _ {k} | z _ {1: k - 1}) d x _ {k}
$$

and corresponds to the likelihood function for the time-step $k$ . 

Proof: Indeed we have 

$$
\begin{array}{l} p (x _ {k} | z _ {1: k}) = \frac {p (z _ {1 : k} | x _ {k}) p (x _ {k})}{p (z _ {1 : k})} \\ = \frac {p (z _ {k} , z _ {1 : k - 1} | x _ {k}) p (x _ {k})}{p (z _ {k} , z _ {1 : k - 1})} \\ = \frac {p (z _ {k} | z _ {1 : k - 1} , x _ {k}) p (z _ {1 : k - 1} | x _ {k}) p (x _ {k})}{p (z _ {k} | z _ {1 : k - 1}) p (z _ {1 : k - 1})} \\ = \frac {p (z _ {k} | z _ {1 : k - 1} , x _ {k}) p (x _ {k} | z _ {1 : k - 1}) p (z _ {1 : k - 1}) p (x _ {k})}{p (z _ {k} | z _ {1 : k - 1}) p (z _ {1 : k - 1}) p (x _ {k})} \\ = \frac {p (z _ {k} | x _ {k}) p (x _ {k} | z _ {1 : k - 1})}{p (z _ {k} | z _ {1 : k - 1})} \end{array}
$$

(QED) 

Note that we use the fact that at time step k the value of $z _ { 1 : k }$ is perfectly known. 

The Kalman Filter (detailed below) is a special case where the distributions are normal and could be written as 

$$
p (x _ {k} | z _ {k - 1}) = \mathcal {N} (\hat {x} _ {k} ^ {-}, P _ {k} ^ {-})
$$

$$
p (x _ {k} | z _ {k}) = \mathcal {N} (\hat {x} _ {k}, P _ {k})
$$

In the special Gaussian case, each distribution could be entirely characterized via its first two moments. However, it is important to remember that the Kalman filter (KF) is optimal in the Gaussian linear case. In the nonlinear case, it will always be suboptimal. 

Interpretation of the Kalman Gain The basic idea behind the KF is the following observation. Having x a normally distributed random variable with a mean $m _ { x }$ and variance $S _ { x x } ,$ having z a normally distributed random variable with a mean $m _ { z }$ and variance $S _ { z z } ,$ as well as $S _ { z x } = S _ { x z }$ the covariance between x and $z ,$ the conditional distribution of $x | z$ is also normal with 

$$
m _ {x | z} = m _ {x} + K (z - m _ {z})
$$

with 

$$
K = S _ {x z} S _ {z z} ^ {- 1}
$$

Interpreting x as the hidden-state and z as the observation, the above matrix K would correspond to the Kalman filter in the linear case. We also have 

$$
S _ {x | z} = S _ {x x} - K S _ {x z}
$$

An alternative interpretation of the Kalman filter could be based on linear regression. Indeed, if we knew the time-series of $( z _ { k } )$ and $( x _ { k } )$ , then the regression could be written as 

$$
x _ {k} = \beta z _ {k} + \alpha + \epsilon_ {k}
$$

with $\beta$ the slope, α the intercept, and $( \epsilon _ { k } )$ the residuals. It is known that under a least-square regression, we have 

$$
\beta = S _ {x z} S _ {z z} ^ {- 1}
$$

which again is the expression for the Kalman gain. 

We now will describe various nonlinear extensions of the Kalman filter. 

## The Simple and Extended Kalman Filters

The first algorithms we choose here are the simple and extended Kalman filters,<sup>9</sup> owing to their well-known flexibility and ease of implementation. The simple or traditional Kalman filter (KF) applies to linear Gaussian cases, whereas the extended KF (EKF) could be used for nonlinear Gaussian cases via a first-order linearization. We shall therefore describe EKF and consider the simple KF as a special case. In order to clarify the notations, let us briefly rewrite the EKF equations. Given a dynamic process $\mathbf { x } _ { k }$ following a possibly nonlinear transition equation 

$$
\mathbf {x} _ {k} = \mathbf {f} (\mathbf {x} _ {k - 1}, \mathbf {w} _ {k})\tag{2.1}
$$

we suppose we have a measurement $\mathbf { z } _ { k }$ via a possibly nonlinear observation equation 

$$
\mathbf {z} _ {k} = \mathbf {h} (\mathbf {x} _ {k}, \mathbf {u} _ {k})\tag{2.2}
$$

where $\mathbf { w } _ { k }$ and ${ \bf u } _ { k }$ are two mutually uncorrelated sequences of temporally uncorrelated normal random variables with zero means and covariance matrices $\mathbf { Q } _ { k } , \mathbf { R } _ { k } ,$ , respectively.<sup>10</sup> Moreover, $\mathbf { w } _ { k }$ is uncorrelated with $\mathbf { X } \boldsymbol { k } _ { - 1 }$ and ${ \bf u } _ { k }$ uncorrelated with $\mathbf { x } _ { k }$ 

We define the linear a priori process estimate as 

$$
\hat {\mathbf {x}} _ {k} ^ {-} = \mathbf {E} [ \mathbf {x} _ {k} ]\tag{2.3}
$$

which is the estimation at time step $k - 1$ prior to measurement. Similarly, we define the linear a posteriori estimate 

$$
\hat {\mathbf {x}} _ {k} = \mathbf {E} [ \mathbf {x} _ {k} | \mathbf {z} _ {k} ]\tag{2.4}
$$

which is the estimation at time step k after the measurement. 

We also have the corresponding estimation errors $\mathbf { e } _ { k } ^ { - } = \mathbf { x } _ { k } - \hat { \mathbf { x } } _ { k } ^ { - }$ and $\mathbf { e } _ { k } = \mathbf { x } _ { k } - \hat { \mathbf { x } } _ { k }$ and the estimate error covariances 

$$
\mathbf {P} _ {k} ^ {-} = \mathbf {E} [ \mathbf {e} _ {k} ^ {-} \mathbf {e} _ {k} ^ {- t} ]\tag{2.5}
$$

$$
\mathbf {P} _ {k} = \mathbf {E} [ \mathbf {e} _ {k} \mathbf {e} _ {k} ^ {t} ]\tag{2.6}
$$

where the superscript t corresponds to the transpose operator. 

We now define the Jacobian matrices of f with respect to the system process and the system noise as $\mathbf { A } _ { k }$ and $\mathbf { W } _ { k }$ respectively. Similarly, we define the gradient matrices of h with respect to the system process and the measurement noise as $\mathbf { H } _ { k }$ and $\mathbf { U } _ { k }$ respectively. More accurately, for every row i and column j we have 

$$
\begin{array}{l l} \mathbf {A} _ {i j} = \partial \mathbf {f} _ {i} / \partial \mathbf {x} _ {j} (\hat {\mathbf {x}} _ {k - 1}, 0) & \quad \mathbf {W} _ {i j} = \partial \mathbf {f} _ {i} / \partial \mathbf {w} _ {j} (\hat {\mathbf {x}} _ {k - 1}, 0) \\ \mathbf {H} _ {i j} = \partial \mathbf {h} _ {i} / \partial \mathbf {x} _ {j} (\hat {\mathbf {x}} _ {k} ^ {-}, 0) & \quad \mathbf {U} _ {i j} = \partial \mathbf {h} _ {i} / \partial \mathbf {u} _ {j} (\hat {\mathbf {x}} _ {k} ^ {-}, 0) \end{array}
$$

We therefore have the following time update equations 

$$
\hat {\mathbf {x}} _ {k} ^ {-} = \mathbf {f} (\hat {\mathbf {x}} _ {k - 1}, 0)\tag{2.7}
$$

and 

$$
\mathbf {P} _ {k} ^ {-} = \mathbf {A} _ {k} \mathbf {P} _ {k - 1} \mathbf {A} _ {k} ^ {t} + \mathbf {W} _ {k} \mathbf {Q} _ {k - 1} \mathbf {W} _ {k} ^ {t}\tag{2.8}
$$

We define the Kalman gain as the matrix $\mathbf { K } _ { k }$ used in the measurement update equations 

$$
\hat {\mathbf {x}} _ {k} = \hat {\mathbf {x}} _ {k} ^ {-} + \mathbf {K} _ {k} (\mathbf {z} _ {k} - \mathbf {h} (\hat {\mathbf {x}} _ {k} ^ {-}, 0))\tag{2.9}
$$

and 

$$
\mathbf {P} _ {k} = (\mathbf {I} - \mathbf {K} _ {k} \mathbf {H} _ {k}) \mathbf {P} _ {k} ^ {-}\tag{2.10}
$$

where I represents the identity matrix. 

The optimal Kalman gain corresponds to the mean of the conditional distribution of $\mathbf { x } _ { k }$ upon the observation $\mathbf { z } _ { k }$ or, equivalently, the matrix that would minimize the mean square error $\mathbf { P } _ { k }$ within the class of linear estimators. This optimal gain is 

$$
\mathbf {K} _ {k} = \mathbf {P} _ {k} ^ {-} \mathbf {H} _ {k} ^ {t} (\mathbf {H} _ {k} \mathbf {P} _ {k} ^ {-} \mathbf {H} _ {k} ^ {t} + \mathbf {U} _ {k} \mathbf {R} _ {k} \mathbf {U} _ {k} ^ {t}) ^ {- 1}\tag{2.11}
$$

The foregoing equations complete the Kalman filter algorithm. 

Another Interpretation of the Kalman Gain Note that an easy way to observe that $K _ { k }$ minimizes the a posteriori error covariance $P _ { k }$ is to consider the onedimensional linear case 

$$
\hat {x} _ {k} = \hat {x} _ {k} ^ {-} + K _ {k} (z _ {k} - H _ {k} \hat {x} _ {k} ^ {-}) = \hat {x} _ {k} ^ {-} + K _ {k} (z _ {k} - H _ {k} x _ {k} + H _ {k} e _ {k} ^ {-})
$$

so 

$$
e _ {k} = x _ {k} - \hat {x} _ {k} = e _ {k} ^ {-} - K _ {k} (u _ {k} + H _ {k} e _ {k} ^ {-})
$$

Therefore 

$$
P _ {k} = \mathbf {E} (e _ {k} ^ {2}) = P _ {k} ^ {-} + K _ {k} ^ {2} (R _ {k} + H _ {k} ^ {2} P _ {k} ^ {-} + 0) - 2 K _ {k} H _ {k} P _ {k} ^ {-}
$$

and taking the derivative with respect to $K _ { k }$ and setting it to zero, we get 

$$
K _ {k} = \frac {P _ {k} ^ {-} H _ {k}}{H _ {k} ^ {2} P _ {k} ^ {-} + R _ {k}}
$$

which is the one-dimensional expression for the linear Kalman gain. 

Residuals, Mean Price Error (MPE) and Root Mean Square Error (RMSE) In what follows we shall call the estimated observations $\hat { z } _ { k } ^ { - }$ . For the simple and extended Kalman filters, we have 

$$
\hat {z} _ {k} ^ {-} = b (\hat {x} _ {k} ^ {-}, 0)
$$

The residuals are the observation errors, defined as 

$$
\tilde {z} _ {k} = z _ {k} - \hat {z} _ {k} ^ {-}
$$

Needless to say, the smaller these residuals, the higher the quality of the filter. Therefore, to measure the performance, we define the mean price error (MPE) and root mean square error (RMSE) as the mean and standard deviation of the residuals 

$$
M P E = \frac {1}{N} \sum_ {k = 1} ^ {N} \tilde {z} _ {k}
$$

$$
R M S E = \sqrt {\frac {1}{N} \sum_ {k = 1} ^ {N} (\tilde {z} _ {k} - M P E) ^ {2}}
$$

## The Unscented Kalman Filter

Recently, Julier and Uhlmann [166] proposed a new extension of the Kalman filter to nonlinear systems, one that is completely different from the EKF. They argue that EKF could be difficult to implement and, more importantly, difficult to tune and that it would be reliable only for systems that are almost linear within the update intervals. The new method, called the unscented Kalman filter (UKF), will calculate the mean to a higher order of accuracy than the EKF and the covariance to the same order of accuracy. Unlike the EKF, this method does not require any Jacobian calculation since it does not approximate the nonlinear functions of the process and the observation. Therefore, it uses the true nonlinear models but approximates the distribution of the state random variable $\mathbf { x } _ { k }$ by applying an unscented transformation to it. As we will see in the following, we construct a set of sigma points that capture the mean and covariance of the original distribution and, when propagated through the true nonlinear system, capture the posterior mean and covariance accurately to the third order. 

Similarly to the EKF, we start with an initial choice for the state vector $\hat { \mathbf { x } } _ { 0 } = \mathbf { E } [ \mathbf { x } _ { 0 } ]$ and its covariance matrix ${ \bf P } _ { 0 } = { \bf E } [ ( { \bf x } _ { 0 } - \hat { \bf x } _ { 0 } ) ( { \bf x } _ { 0 } - \hat { \bf x } _ { 0 } ) ^ { t } ]$ . We then concatenate the space vector with the system noise and the observation noise<sup>11</sup> and create an augmented state vector for each step k greater than one 

$$
\mathbf {x} _ {k - 1} ^ {a} = \left( \begin{array}{c} \mathbf {x} _ {k - 1} \\ \mathbf {w} _ {k - 1} \\ \mathbf {u} _ {k - 1} \end{array} \right)
$$

and therefore 

$$
\hat {\mathbf {x}} _ {k - 1} ^ {a} = \left( \begin{array}{c} \hat {\mathbf {x}} _ {k - 1} \\ \mathbf {0} \\ \mathbf {0} \end{array} \right)
$$

and 

$$
\mathbf {P} _ {k - 1} ^ {a} = \left( \begin{array}{c c c} \mathbf {P} _ {k - 1} & \mathbf {P} _ {x w} (k - 1 | k - 1) & \mathbf {0} \\ \mathbf {P} _ {x w} (k - 1 | k - 1) & \mathbf {P} _ {w w} (k - 1 | k - 1) & \mathbf {0} \\ \mathbf {0} & \mathbf {0} & \mathbf {P} _ {u u} (k - 1 | k - 1) \end{array} \right)
$$

for each iteration k. The augmented state will therefore have a dimension $n _ { a } = n _ { x } + n _ { w } + n _ { u }$ 

We then need to calculate the corresponding sigma points through the unscented transformation: 

$$
\chi_ {k - 1} ^ {a} (0) = \hat {\mathbf {x}} _ {k - 1} ^ {a}
$$

For $i = 1 , . . . , n _ { a }$ 

$$
\chi_ {k - 1} ^ {a} (i) = \hat {\mathbf {x}} _ {k - 1} ^ {a} + \left(\sqrt {(n _ {a} + \lambda) \mathbf {P} _ {k - 1} ^ {a}}\right) _ {i}
$$

and for $i = n _ { a } + 1 , . . . , 2 n _ { a }$ 

$$
\chi_ {k - 1} ^ {a} (i) = \hat {\mathbf {x}} _ {k - 1} ^ {a} - \left(\sqrt {(n _ {a} + \lambda) \mathbf {P} _ {k - 1} ^ {a}}\right) _ {i - n _ {a}}
$$

where the above subscripts i and $i - n _ { a }$ correspond to the $i ^ { t h }$ and $i - n _ { a } ^ { t b }$ columns of the square-root matrix.<sup>12</sup> This prepares us for the time update and the measurement update equations, similarly to the EKF. 

The time update equations are 

$$
\chi_ {k | k - 1} (i) = \mathbf {f} (\chi_ {k - 1} ^ {x} (i), \chi_ {k - 1} ^ {w} (i))
$$

for $i = 0 , . . . , 2 n _ { a } + 1$ and 

$$
\hat {\mathbf {x}} _ {k} ^ {-} = \sum_ {i = 0} ^ {2 n _ {a}} W _ {i} ^ {(m)} \chi_ {k | k - 1} (i)
$$

and 

$$
\mathbf {P} _ {k} ^ {-} = \sum_ {i = 0} ^ {2 n _ {a}} W _ {i} ^ {(c)} (\chi_ {k | k - 1} (i) - \hat {\mathbf {x}} _ {k} ^ {-}) (\chi_ {k | k - 1} (i) - \hat {\mathbf {x}} _ {k} ^ {-}) ^ {t}
$$

where the superscripts x and $_ { \nu }$ respectively correspond to the state and system-noise portions of the augmented state. 

The ${ \mathbb { W } } _ { i } ^ { ( m ) }$ and $\mathbb { W } _ { i } ^ { ( c ) }$ weights are defined as 

$$
W _ {0} ^ {(m)} = \frac {\lambda}{n _ {a} + \lambda}
$$

and 

$$
W _ {0} ^ {(c)} = \frac {\lambda}{n _ {a} + \lambda} + (1 - \alpha^ {2} + \beta)
$$

and for $i = 1 , . . . , 2 n _ { a }$ 

$$
W _ {i} ^ {(m)} = W _ {i} ^ {(c)} = \frac {1}{2 (n _ {a} + \lambda)}
$$

The scaling parameters $\alpha , \beta ,$ κ and $\lambda = \alpha ^ { 2 } ( n _ { a } + \kappa ) - n _ { a }$ will be chosen for tuning. 

We also define within the time update equations 

$$
\mathbf {Z} _ {k | k - 1} (i) = \mathbf {h} (\chi_ {k | k - 1} (i), \chi_ {k - 1} ^ {u} (i))
$$

and 

$$
\hat {\mathbf {z}} _ {k} ^ {-} = \sum_ {i = 0} ^ {2 n _ {a}} W _ {i} ^ {(m)} \mathbf {Z} _ {k | k - 1} (i)
$$

where the superscript u corresponds to the observation-noise portion of the augmented state. 

As for the measurement update equations, we have 

$$
\mathbf {P} _ {z _ {k} z _ {k}} = \sum_ {i = 0} ^ {2 n _ {a}} W _ {i} ^ {(c)} (\mathbf {Z} _ {k | k - 1} (i) - \hat {\mathbf {z}} _ {k} ^ {-}) (\mathbf {Z} _ {k | k - 1} (i) - \hat {\mathbf {z}} _ {k} ^ {-}) ^ {t}
$$

and 

$$
\mathbf {P} _ {x _ {k} z _ {k}} = \sum_ {i = 0} ^ {2 n _ {a}} W _ {i} ^ {(c)} (\chi_ {k | k - 1} (i) - \hat {\mathbf {x}} _ {k} ^ {-}) (\mathbf {Z} _ {k | k - 1} (i) - \hat {\mathbf {z}} _ {k} ^ {-}) ^ {t}
$$

which gives us the Kalman gain 

$$
\mathbf {K} _ {k} = \mathbf {P} _ {x _ {k} z _ {k}} \mathbf {P} _ {z _ {k} z _ {k}} ^ {- 1}
$$

and we get as before 

$$
\hat {\mathbf {x}} _ {k} = \hat {\mathbf {x}} _ {k} ^ {-} + \mathbf {K} _ {k} (\mathbf {z} _ {k} - \hat {\mathbf {z}} _ {k} ^ {-})
$$

where again $\mathbf { z } _ { k }$ is the observation at time (iteration) k. Also, we have 

$$
\mathbf {P} _ {k} = \mathbf {P} _ {k} ^ {-} - \mathbf {K} _ {k} \mathbf {P} _ {z _ {k} z _ {k}} \mathbf {K} _ {k} ^ {t}
$$

which completes the measurement update equations. 

## Kushner’s Nonlinear Filter

It would be instructive to compare this algorithm to the nonlinear filtering algorithm based on an approximation of the conditional distribution by Kushner et al. [174]. In this approach, the authors suggest using a Gaussian quadrature in order to calculate the integral at the measurement update (or the time update) step.<sup>13</sup> As the Kushner paper indicates, having an N-dimensional normal random variable $\mathbf { X } = \bar { \mathcal { N } } ( \mathbf { m } , \mathbf { P } )$ , with m and P the corresponding mean and covariance, for a polynomial G of degree 2M 1, we can write<sup>14</sup> 

$$
\mathbf {E} [ G (\mathbf {X}) ] = \frac {1}{(2 \pi) ^ {\frac {N}{2}} | \mathbf {P} | ^ {\frac {1}{2}}} \int G (\mathbf {y}) \exp \left[ - \frac {(\mathbf {y} - \mathbf {m}) ^ {t} \mathbf {P} ^ {- 1} (\mathbf {y} - \mathbf {m})}{2} \right] d \mathbf {y}
$$

which is equal to 

$$
\mathbf {E} [ G (\mathbf {X}) ] = \sum_ {i _ {1} = 1} ^ {M} \dots \sum_ {i _ {N} = 1} ^ {M} w _ {i _ {1}} \dots w _ {i _ {N}} G \left(\mathbf {m} + \sqrt {\mathbf {P}} \zeta\right)
$$

where $\zeta ^ { t } = ( \zeta _ { i _ { 1 } } , . . . , \zeta _ { i _ { N } } )$ is the vector of the Gauss-Hermite roots of order M and $\displaystyle \boldsymbol { w } _ { i _ { 1 } } , . . . , \boldsymbol { w } _ { i _ { N } }$ are the corresponding weights. Note that even if both Kushner’s NLF and UKF use Gaussian qadratures, UKF only uses $2 N + 1$ sigma points, whereas NLF needs $M ^ { N }$ points for the integral computation. 

Kushner and Budhiraja suggest using this technique primarily for the measurement update (filtering) step. They claim that provided this step is properly implemented, the time update (prediction) step can be carried out via a linearization similar to the EKF. 

Details of the Kushner algorithm Let us use the same notations as for the UKF algorithm. We therefore have the augmented state $\mathbf { x } _ { k - 1 } ^ { a }$ and its covariance $\mathbf { P } _ { k - 1 } ^ { a }$ as before. Here, for a quadrature order of M on an N-dimensional variable, the sigma points are defined for $j = 1 , . . . , N$ and $i _ { j } = 1 , . . . , M$ as 

$$
\chi_ {k - 1} ^ {a} (i _ {1}, \dots , i _ {N}) = \hat {\mathbf {x}} _ {k - 1} ^ {a} + \sqrt {\mathbf {P} _ {k - 1} ^ {a}} \zeta (i _ {1}, \dots , i _ {N})
$$

where the square root here corresponds to the Cholesky factorization, and again $\zeta ( i _ { 1 } , \ldots , i _ { N } ) [ j ] = \zeta _ { i _ { i } }$ for each $j$ between 1 and the dimension N and each $i _ { j }$ between 1 and the quadrature order M. Similarly to the UKF, we have the time update equations 

$$
\chi_ {k | k - 1} (i _ {1}, \dots , i _ {N}) = \mathbf {f} \big (\chi_ {k - 1} ^ {x} (i _ {1}, \dots , i _ {N}), \chi_ {k - 1} ^ {w} (i _ {1}, \dots , i _ {N}) \big)
$$

but now 

$$
\hat {\mathbf {x}} _ {k} ^ {-} = \sum_ {i _ {1} = 1} ^ {M} \dots \sum_ {i _ {N} = 1} ^ {M} w _ {i _ {1}} \dots w _ {i _ {N}} \chi_ {k | k - 1} (i _ {1}, \dots , i _ {N})
$$

and 

$$
\mathbf {P} _ {k} ^ {-} = \sum_ {i _ {1} = 1} ^ {M} \dots \sum_ {i _ {N} = 1} ^ {M} w _ {i _ {1}} \dots w _ {i _ {N}} (\chi_ {k | k - 1} (i _ {1},..., i _ {N}) - \hat {\mathbf {x}} _ {k} ^ {-}) (\chi_ {k | k - 1} (i _ {1},..., i _ {N}) - \hat {\mathbf {x}} _ {k} ^ {-}) ^ {t}
$$

Again, we have 

$$
\mathbf {Z} _ {k \mid k - 1} (i _ {1},..., i _ {N}) = \mathbf {h} \left(\chi_ {k \mid k - 1} (i _ {1},..., i _ {N}), \chi_ {k - 1} ^ {u} (i _ {1},..., i _ {N})\right)
$$

and 

$$
\hat {\mathbf {z}} _ {k} ^ {-} = \sum_ {i _ {1} = 1} ^ {M} \dots \sum_ {i _ {N} = 1} ^ {M} w _ {i _ {1}} \dots w _ {i _ {N}} \mathbf {Z} _ {k | k - 1} (i _ {1}, \dots , i _ {N})
$$

Therefore, the measurement update equations will be 

$$
\mathbf {P} _ {z _ {k} z _ {k}} = \sum_ {i _ {1} = 1} ^ {M} \dots \sum_ {i _ {N} = 1} ^ {M} w _ {i _ {1}} \dots w _ {i _ {N}} (\mathbf {Z} _ {k | k - 1} (i _ {1},..., i _ {N}) - \hat {\mathbf {z}} _ {k} ^ {-}) (\mathbf {Z} _ {k | k - 1} (i _ {1},..., i _ {N}) - \hat {\mathbf {z}} _ {k} ^ {-}) ^ {t}
$$

and 

$$
\mathbf {P} _ {x _ {k} z _ {k}} = \sum_ {i _ {1} = 1} ^ {M} \dots \sum_ {i _ {N} = 1} ^ {M} w _ {i _ {1}} \dots w _ {i _ {N}} (\chi_ {k | k - 1} (i _ {1},..., i _ {N}) - \hat {\mathbf {x}} _ {k} ^ {-}) (\mathbf {Z} _ {k | k - 1} (i _ {1},..., i _ {N}) - \hat {\mathbf {z}} _ {k} ^ {-}) ^ {t}
$$

which gives us the Kalman gain 

$$
\mathbf {K} _ {k} = \mathbf {P} _ {x _ {k} z _ {k}} \mathbf {P} _ {z _ {k} z _ {k}} ^ {- 1}
$$

and we get as before 

$$
\hat {\mathbf {x}} _ {k} = \hat {\mathbf {x}} _ {k} ^ {-} + \mathbf {K} _ {k} (\mathbf {z} _ {k} - \hat {\mathbf {z}} _ {k} ^ {-})
$$

where again $\mathbf { z } _ { k }$ is the observation at time (iteration) k. 

Also, we have 

$$
\mathbf {P} _ {k} = \mathbf {P} _ {k} ^ {-} - \mathbf {K} _ {k} \mathbf {P} _ {z _ {k} z _ {k}} \mathbf {K} _ {k} ^ {t}
$$

which completes the measurement update equations. 

When N 1 and λ 2, the numeric integration in the UKF will correspond to a Gauss-Hermite quadrature of order $M = 3$ . However, in the UKF we can tune the filter and reduce the higher term errors via the previously mentioned parameters α and $\beta .$ 

Note that when $b ( \boldsymbol { x } , \boldsymbol { u } )$ is strongly nonlinear, the Gauss Hermite integration is not efficient for evaluating the moments of the measurement update equation, since the term $\scriptstyle p ( z _ { k } | x _ { k } )$ contains the exponent $z _ { k } - b ( x _ { k } , u _ { k } )$ . The iterative methods based on the idea of importance sampling proposed in [174] correct this problem at the price of a strong increase in computation time. As suggested in [151], one way to avoid this integration would be to make the additional hypothesis that $x _ { k } , b ( x _ { k } , u _ { k } ) | z _ { 1 : k - 1 }$ is Gaussian. 

## Parameter Learning

One important issue to realize is that the Kalman filter can be used either for state estimation (filtering) or for parameter estimation (machine learning). When we have both state estimation and parameter estimation, we are dealing with a dual estimation or a joint estimation. The latter case is the one concerning us because we are estimating the state volatility as well as the model parameters. As explained in Haykin’s book [133], in a dual filter we separate the state vector from the parameters and we apply two intertwined filters to them. By contrast, in a joint filter, we concatenate the state vector and the parameters and apply one filter to this augmented state. Note that in the dual filter we need to compute recurrent derivatives with respect to parameters, whereas in a joint filter no such step is needed. 

It is possible to interpret the joint filter in the following way. In a regular filter, that is, filtering of the state $x _ { k }$ for a fixed set of parameters $\Psi _ { 0 } ,$ we are maximizing the conditional density 

$$
p (x _ {1: k} | z _ {1: k}, \Psi_ {0})
$$

and as we said, to do that we write 

$$
p (x _ {1: k} | z _ {1: k}, \Psi_ {0}) = \frac {p (z _ {1 : k} | x _ {1 : k} , \Psi_ {0}) p (x _ {1 : k} | \Psi_ {0})}{p (z _ {1 : k} | \Psi_ {0})}
$$

so we maximize the above with respect to the state $x _ { k }$ for a given set of parameters. This means that the optimal state $\hat { x } _ { 1 : k }$ for a given parameter set is given by 

$$
\hat {x} _ {1: k} = \operatorname{argmax} \left[ p \left(z _ {1: k}, x _ {1: k} \mid \Psi_ {0}\right) \right]
$$

As we will see, in an MLE approach we use this optimal state filtering for each iteration of the likelihood maximization over the parameter set $\Psi$ . 

In a joint filter, we are directly optimizing the joint conditional density 

$$
p (x _ {1: k}, \Psi | z _ {1: k})
$$

which we can also write as 

$$
p (x _ {1: k}, \Psi | z _ {1: k}) = \frac {p (z _ {1 : k} | x _ {1 : k} , \Psi) p (x _ {1 : k} | \Psi) p (\Psi)}{p (z _ {1 : k})}
$$

given that the denominator is functionally independent of $x _ { 1 : k }$ and $\Psi ,$ and given that $p ( \Psi )$ contains no prior information,<sup>15</sup> the maximization will be upon 

$$
p (z _ {1: k} | x _ {1: k}, \Psi) p (x _ {1: k} | \Psi) = p (z _ {1: k}, x _ {1: k} | \Psi)
$$

That is to say, in a joint filter, the optimal state $\hat { x } _ { 1 : k }$ and parameter set $\hat { \Psi }$ are found by writing 

$$
(\hat {x} _ {1: k}, \hat {\Psi}) = a r g m a x [ p (z _ {1: k}, x _ {1: k} | \Psi) ]
$$

In what follows, we apply the joint EKF methodology to a few examples. 

An Illustration Before using this technique for the stochastic volatility model, let us take a simple example 

$$
\xi_ {k} = \xi_ {k - 1} + \pi + 0. 1 0 w _ {k}
$$

and 

$$
z _ {k} = \xi_ {k} + 0. 1 0 u _ {k}
$$

where $\pi \approx 3 . 1 4 1 5 9$ and $w _ { k } , u _ { k }$ are independent Gaussian random variables. The linear state-space system could be written as 

$$
\mathbf {x} _ {k} = \binom{\xi_ {k}}{\pi_ {k}} = \left( \begin{array}{c c} 1 & 1 \\ 0 & 1 \end{array} \right) \mathbf {x} _ {k - 1} + 0. 1 0 \binom{w _ {k}}{0}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/815b05889d250f05e25c3d2ac430d5751a9f861709830581b1100aa8017df0e9.jpg)



FIGURE 2.6 A Simple Example for the Joint Filter. The convergence toward the constant parameter π happens after a few iterations.


and 

$$
z _ {k} = (1 0) \mathbf {x} _ {k} + 0. 1 0 u _ {k}
$$

We choose the initial values $\xi _ { 0 } = z _ { 0 } = 0$ and $\pi _ { 0 } ~ = ~ 1 . 0$ . We also take Q $= 0 . 1 \mathbf { I } _ { 2 }$ and $R = 0 . 1 0$ . Applying the Kalman filter to an artificially generated data set, we plot the resulting $\pi _ { k }$ in Figure 2.6. As we can see, the parameter converges very quickly to its true value. 

Even if we associated a noise of 0.10 to the constant parameter $\pi ,$ we can see that for 5000 observations, taking the mean of the filtered state between observations 20 and 5000 we get 

$$
\hat {\pi} = 3. 1 4 1 3 9 0 4 8 8
$$

which is very close to the value 3.14159 used in data generation process. 

Joint Filtering Examples After going through this simple example, we now apply the JF technique to our stochastic volatility problem. We shall study a few examples in order to find the best state-space representation. 

Example 1 Our first example would be the square-root stochastic volatility model 

$$
\ln S _ {k} = \ln S _ {k - 1} + \left(\mu_ {S} - \frac {1}{2} \nu_ {k - 1}\right) \Delta t + \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} B _ {k - 1}
$$

$$
\nu_ {k} = \nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} Z _ {k - 1}
$$

To simplify we suppose that the value of $\mu _ { S }$ is known. We can now define the state variable<sup>16</sup> 

$$
\mathbf {x} _ {k} = \left( \begin{array}{c} \ln S _ {k} \\ \nu_ {k} \\ \omega \\ \theta \\ \xi \\ \rho \end{array} \right)
$$

and the system noise 

$$
\mathbf {w} _ {k} = \binom{B _ {k}}{Z _ {k}}
$$

with its covariance matrix 

$$
\mathbf {Q} _ {k} = \left( \begin{array}{c c} 1 & \rho \\ \rho & 1 \end{array} \right)
$$

and therefore 

$$
\mathbf {x} _ {k} = \mathbf {f} (\mathbf {x} _ {k - 1}, \mathbf {w} _ {k - 1}) = \left( \begin{array}{c} \ln S _ {k - 1} + (\mu_ {S} - \frac {1}{2} \nu_ {k - 1}) \Delta t + \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} B _ {k - 1} \\ \nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} Z _ {k - 1} \\ \omega \\ \theta \\ \xi \\ \rho \end{array} \right)
$$

and therefore the Jacobian $\mathbf { A } _ { k }$ is 

$$
\mathbf {A} _ {k} = \left( \begin{array}{c c c c c c} 1 & - \frac {1}{2} \Delta t & 0 & 0 & 0 & 0 \\ 0 & 1 - \theta \Delta t & \Delta t & - \nu_ {k - 1} \Delta t & 0 & 0 \\ 0 & 0 & 1 & 0 & 0 & 0 \\ 0 & 0 & 0 & 1 & 0 & 0 \\ 0 & 0 & 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 0 & 0 & 1 \end{array} \right)
$$

and 

$$
\mathbf {W} _ {k} = \left( \begin{array}{c c} \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} & 0 \\ 0 & \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} \\ 0 & 0 \\ 0 & 0 \\ 0 & 0 \\ 0 & 0 \end{array} \right)
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/00558d663034d3bedf12984a6c74844854aee05d073e80b0429336dee9a632a7.jpg)



FIGURE 2.7 The EKF Estimation (Example 1) for the Drift Parameter $\omega .$ The SPX index daily close prices were used over five years from 10/01/1996 to 09/28/2001. The convergence is fairly good.


having the measurement $z _ { k } = \ln S _ { k }$ we can write 

$$
\mathbf {H} _ {k} = \left( \begin{array}{c c c c c c} 1 & 0 & 0 & 0 & 0 & 0 \end{array} \right)
$$

and $U _ { k } = 0$ 

We could, however, introduce a measurement noise $R$ corresponding to the intraday stock price movements and the bid-ask spread, in which case we would have $z _ { k } = \ln S _ { k } + R \epsilon _ { k }$ , where $\epsilon _ { k }$ represents a sequence of uncorrelated standard normal random variables. This means that $R _ { k } = R$ and $U _ { k } = 1$ . We can then tune the value of R in order to get more stable results (Figures 2.7 through 2.10). 

Example 2 The same exact methodology could be used in the GARCH framework. We define the state variable $\mathbf { x } _ { k } ^ { t } = ( \ln S _ { k } , \nu _ { k } , \omega _ { 0 } , \alpha , \beta , c )$ and take for observation the logarithm of the actual stock price $S _ { k }$ . The system could be written as 

$$
\mathbf {x} _ {k} = \mathbf {f} (\mathbf {x} _ {k - 1}, \mathbf {w} _ {k - 1})
$$

Extended Kalman Filter 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/6035c74468524978bf26c16411b1d9e0b28a68aae0bb6835fb9e35b2a64af26d.jpg)



FIGURE 2.8 The EKF Estimation (Example 1) for the Drift Parameter θ. The SPX index daily close prices were used over five years from 10/01/1996 to 09/28/2001. The convergence is fairly good.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/ed2b04d11cabdbf0a3b3a41d3113c79f949ea898afbf7a484a8985199ef6f550.jpg)



FIGURE 2.9 The EKF Estimation (Example 1) for the Volatility-of-Volatility Parameter ξ. The SPX index daily close prices were used over five years from 10/01/1996 to 09/28/2001. The convergence is rather poor. We shall explain this via the concept of observability.



Extended Kalman Filter


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/e967e8b567ea13c37c9788d63f90b9432768cc31a0027117c637b321e034d1f8.jpg)



FIGURE 2.10 The EKF Estimation (Example 1) for the correlation parameter $\rho .$ The SPX index daily close prices were used over five years from 10/01/1996 to 09/28/2001. The convergence is rather poor. We shall explain this via the concept of observability.


with $\mathbf { w } _ { k } = B _ { k }$ a one-dimensional source of noise with a variance $\mathcal Q _ { k } = 1$ and 

$$
\mathbf {f} (\mathbf {x} _ {k - 1}, \mathbf {w} _ {k - 1}) = \left( \begin{array}{c} \ln S _ {k - 1} + \left(\mu_ {S} - \frac {1}{2} \nu_ {k - 1}\right) + \sqrt {\nu_ {k - 1}} B _ {k - 1} \\ \omega_ {0} + \beta \nu_ {k - 1} + \alpha (B _ {k - 1} - c \sqrt {\nu_ {k - 1}}) ^ {2} \\ \omega_ {0} \\ \alpha \\ \beta \\ c \end{array} \right)
$$

and the Jacobian 

$$
\mathbf {A} _ {k} = \left( \begin{array}{c c c c c c} 1 & - \frac {1}{2} & 0 & 0 & 0 & 0 \\ 0 & \beta + \alpha c ^ {2} & 1 & c ^ {2} v _ {k - 1} & v _ {k - 1} & 2 \alpha c v _ {k - 1} \\ 0 & 0 & 1 & 0 & 0 & 0 \\ 0 & 0 & 0 & 1 & 0 & 0 \\ 0 & 0 & 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 0 & 0 & 1 \end{array} \right)
$$

and 

$$
\mathbf {W} _ {k} = \left( \begin{array}{c} \sqrt {\nu_ {k - 1}} \\ - 2 \alpha c \sqrt {\nu_ {k - 1}} \\ 0 \\ 0 \\ 0 \\ 0 \end{array} \right)
$$

The observation $z _ { k }$ will be 

$$
\mathbf {z} _ {k} = \mathbf {h} (\mathbf {x} _ {k}) = \ln (S _ {k})
$$

exactly as in the previous example. The rest of the algorithm would therefore be identical to the one included in Example 1. 

Example 3 In Examples 1 and 2, we included all the variables in the system process and we observed part of the system. It is also possible to separate the measurement and the system variables as follows. 

Taking a general discrete stochastic volatility process $\mathsf { a s } ^ { 1 7 }$ 

$$
\begin{array}{c} \ln S _ {k} = \ln S _ {k - 1} + \left(\mu_ {S} - \frac {1}{2} \nu_ {k}\right) \Delta t + \sqrt {\nu_ {k}} \sqrt {\Delta t} B _ {k} \\ \nu_ {k} = \nu_ {k - 1} + b (\nu_ {k - 1}) \Delta t + a (\nu_ {k - 1}) \sqrt {\Delta t} Z _ {k} \end{array}
$$

with $B _ { k }$ and $Z _ { k }$ two Normal random sequences with a mean of zero and variance one, with a correlation equal to $\rho .$ 

Posing $y _ { k } = \sqrt { \nu _ { k } } Z _ { k }$ and performing the usual Cholesky factorization $B _ { k } = \rho Z _ { k } + \sqrt { 1 - \rho ^ { 2 } } X _ { k }$ , where $Z _ { k }$ and $X _ { k }$ are uncorrelated, we can now take the case of a square-root process and write 

$$
\mathbf {x} _ {k} = \left( \begin{array}{c} \nu_ {k} \\ y _ {k} \\ \omega \\ \theta \\ \xi \\ \rho \end{array} \right)
$$

and $\mathbf { x } _ { k } = \mathbf { f } ( \mathbf { x } _ { k - 1 } , Z _ { k } )$ with 

$$
\mathbf {f} (x _ {k - 1}, Z _ {k}) = \left( \begin{array}{c} \nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} Z _ {k} \\ \left(\nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} Z _ {k}\right) ^ {\frac {1}{2}} Z _ {k} \\ \omega + Q Z _ {k} \\ \theta + Q Z _ {k} \\ \xi + Q Z _ {k} \\ \rho + Q Z _ {k} \end{array} \right)
$$

which provides us with the Jacobian 

$$
\mathbf {A} _ {k} = \left( \begin{array}{c c c c c c} 1 - \theta \Delta t & 0 & \Delta t & - \nu_ {k - 1} \Delta t & 0 & 0 \\ 0 & 0 & 0 & 0 & 0 & 0 \\ 0 & 0 & 1 & 0 & 0 & 0 \\ 0 & 0 & 0 & 1 & 0 & 0 \\ 0 & 0 & 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 0 & 0 & 1 \end{array} \right)
$$

and 

$$
\mathbf {W} _ {k} = \left( \begin{array}{c} \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} \\ (\nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t) ^ {\frac {1}{2}} \\ Q \\ Q \\ Q \\ Q \end{array} \right)
$$

The measurement equation is 

$$
z _ {k} = \ln \left(\frac {S _ {k}}{S _ {k - 1}}\right) = \left(\mu_ {S} - \frac {1}{2} \nu_ {k}\right) \Delta t + \rho \sqrt {\Delta t} y _ {k} + \sqrt {1 - \rho^ {2}} \sqrt {\nu_ {k}} \sqrt {\Delta t} X _ {k}
$$

and therefore 

$$
\mathbf {H} _ {k} = \left( \begin{array}{c c c c c c} - \frac {1}{2} \Delta t & \rho \sqrt {\Delta t} & 0 & 0 & 0 & 0 \end{array} \right)
$$

with $u _ { k } = X _ { k }$ and $U _ { k } = \sqrt { 1 - \rho ^ { 2 } } \sqrt { \nu _ { k } } \sqrt { \Delta t } .$ , which completes our set of equa-tions. Again we could tune the system noise Q in order to obtain more stable results. 

Observability From the preceding tests, it seems that the EKF provides us with a nonrobust calibration methodology. Indeed the results are very sensitive to the choice of system noise Q and observation noise R. We chose for this case $\mathcal { Q } = 1 0 ^ { - 3 }$ and $R \approx 0$ 

This brings to attention the issue of observability. A nonlinear system with a state vector $\mathbf { x } _ { k }$ of dimension n is observable if 

$$
\mathbf {O} = \left( \begin{array}{c} \mathbf {H} \\ \mathbf {H A} \\ \mathbf {H A} ^ {2} \\ \dots \\ \mathbf {H A} ^ {n - 1} \end{array} \right)
$$

has a full rank of n. For an explanation, refer to Reif et al. [205]. 

It is fairly easy to see that among the foregoing examples, the first and third (corresponding to the stochastic volatility formulation) have for the observation matrix O a rank of four and therefore are not observable. This explains why they do not converge well and are so sensitive to the tuning parameters $\mathcal { Q }$ and $R$ . This means that the choices of the state variables for Examples 1 and 3 were rather poor. One reason is that in our state-space choice, we considered 

$$
z _ {k} = b (\nu_ {k - 1}, \dots)
$$

and 

$$
x _ {k} = (\dots , \nu_ {k}, \dots) = f (x _ {k - 1}, \dots)
$$

which implies that 

$$
\frac {\partial h}{\partial \nu_ {k}} = 0
$$

We shall see how to correct this in the next section by choosing a more appropriate state-space representation. 

The One-Dimensional State within the Joint Filter Considering the state equation 

$$
\begin{array}{c} \nu_ {k} = \nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} Z _ {k - 1} \\ - \rho \xi \bigg [ \ln S _ {k - 1} + \bigg (\mu_ {S} - \frac {1}{2} \nu_ {k - 1} \bigg) \Delta t + \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} B _ {k - 1} - \ln S _ {k} \bigg ] \end{array}
$$

posing for every $k$ 

$$
\tilde {Z} _ {k} = \frac {1}{\sqrt {1 - \rho^ {2}}} (Z _ {k} - \rho B _ {k})
$$

we will have as expected $\tilde { Z } _ { k }$ uncorrelated with $B _ { k }$ . Therefore, considering the augmented state 

$$
\mathbf {x} _ {k} = \left( \begin{array}{c} \nu_ {k} \\ \omega \\ \theta \\ \xi \\ \rho \end{array} \right)
$$

we will have the state transition equation 

$$
\begin{array}{l} \mathbf {f} (\mathbf {x} _ {k - 1}, \tilde {Z} _ {k - 1}) \\ = \left( \begin{array}{c} \nu_ {k - 1} + [ (\omega - \rho \xi \mu_ {S}) - \left(\theta - \frac {1}{2} \rho \xi\right) \nu_ {k - 1} ] \Delta t + \rho \xi \ln \left(\frac {S _ {k}}{S _ {k - 1}}\right) + \xi \sqrt {1 - \rho^ {2}} \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} \tilde {Z} _ {k - 1} \\ \omega \\ \theta \\ \xi \\ \rho \end{array} \right) \end{array}
$$

and the measurement equation would be 

$$
z _ {k} = \ln S _ {k + 1} = \ln S _ {k} + \left(\mu_ {S} - \frac {1}{2} \nu_ {k}\right) \Delta t + \sqrt {\nu_ {k}} \sqrt {\Delta t} B _ {k}
$$

The corresponding EKF Jacobians for this system are 

$$
\mathbf {A} _ {k} = \left( \begin{array}{c c c c c} 1 - \left(\theta - \frac {1}{2} \rho \xi\right) \Delta t & \Delta t & - v _ {k - 1} \Delta t & \rho \left(\ln \left(\frac {S _ {k}}{S _ {k - 1}}\right) - \left(\mu_ {S} - \frac {1}{2} v _ {k - 1}\right) \Delta t\right) & \xi \left(\ln \left(\frac {S _ {k}}{S _ {k - 1}}\right) - \left(\mu_ {S} - \frac {1}{2} v _ {k - 1}\right) \Delta t\right) \\ 0 & 1 & 0 & 0 & 0 \\ 0 & 0 & 1 & 0 & 0 \\ 0 & 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 0 & 1 \end{array} \right)
$$

$$
\mathbf {W} _ {k} = \left( \begin{array}{c} \xi \sqrt {1 - \rho^ {2}} \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} \\ 0 \\ 0 \\ 0 \\ 0 \end{array} \right)
$$

$$
\begin{array}{c} \mathbf {H} _ {k} = \left( \begin{array}{c c c c c} - \frac {1}{2} \Delta t & 0 & 0 & 0 & 0 \end{array} \right) \\ \mathbf {U} _ {k} = \sqrt {\nu_ {k}} \sqrt {\Delta t} \end{array}
$$

It is easy to check that this system is observable since the observation matrix $\mathbf { O } _ { k }$ is of full rank. This shows that our state-space choice is better than the previous ones. 

The UKF would be implemented in a fashion similar to that of the transition and observation equations above. Again, for the UKF, we would not need to compute any Jacobians. 

An important issue to consider is that of tuning. We could add extra noise to the observation and hence lower the weight associated with the observations. In which case, after choosing a tuning parameter $R _ { : }$ , we would write 

$$
\mathbf {U} _ {k} = \left( \begin{array}{c c} \sqrt {\nu_ {k}} \sqrt {\Delta t} & R \end{array} \right)
$$

and 

$$
\mathbf {U} _ {k} \mathbf {U} _ {k} ^ {t} = \nu_ {k} \Delta t + R ^ {2}
$$

The choice of the initial conditions and the tuning parameters could make the algorithm fail or succeed. It therefore seems that there is little robustness in this procedure. 

We consider the example of 5000 data points artificially produced via a Heston stochastic volatility process with a parameter set 

$$
\Psi^ {*} = (\omega = 0. 1 0, \theta = 1 0. 0, \xi = 0. 0 3, \rho = - 0. 5 0)
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/b92c7650be25ce1ae287bfbb9898d46bd19884fe5a3d50f188a904116769c522.jpg)



FIGURE 2.11 Joint EKF Estimation for the Parameter ω. Prices were simulated with $\Psi ^ { * } = ( 0 . 1 0 , 1 0 . 0 , 0 . 0 3 , - 0 . 5 0 )$ . The convergence remains mediocre. We shall explain this in the following section.


with a given $\mu _ { S } = 0 . 0 2 5$ . We then choose a tuning parameter $R = 0 . 1 0$ and take a reasonable guess for the initial conditions 

$$
\Psi_ {0} = (\omega_ {0} = 0. 1 5, \theta_ {0} = 1 0. 0, \xi_ {0} = 0. 0 2, \rho_ {0} = - 0. 5 1)
$$

and apply the joint filter. The results are displayed in Figures 2.11 to 2.14. As we can see, the convergence for ω and $\theta$ is better than it was for the two others. We shall see later why this is. 

Allowing a burn-in period of 1000 points, we can calculate the mean (and the standard deviation) of the generated parameters, after the simulation 1000. 

Joint Filters and Time Interval One difficulty with the application of the joint filter (JF) to the stochastic volatility problem is the following: Unless we are dealing with a longer time interval, such as $\Delta t = 1$ , the observation error $\sqrt { \nu _ { k } } \sqrt { \Delta t } B _ { k }$ is too large compared with the sensitivity of the filter with respect to the state through $- 0 . 5 \nu _ { k } \Delta t$ . Indeed, for a $\Delta t = 1 / 2 5 2$ we have<sup>18</sup> 

$$
\Delta t = o (\sqrt {\Delta t})
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/d2d765397becc38077d253781613b63f2f8f70eff1f24fbf2717c94257793ca1.jpg)



FIGURE 2.12 Joint EKF Estimation for the Parameter $\theta .$ Prices were simulated with $\Psi ^ { * } = ( 0 . 1 0 , 1 0 . 0 , 0 . 0 3 , - 0 . 5 0 )$ . The convergence remains mediocre. We shall explain this in the following section.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/c0b6cf8f6e61819072fe4e3df67dca9ca36a27b98e778ba2f616441aa73af358.jpg)



FIGURE 2.13 Joint EKF Estimation for the Parameter $\xi .$ Prices were simulated with $\Psi ^ { * } = ( 0 . 1 0 , 1 0 . 0 , 0 . 0 3 , - 0 . 5 0 )$ . The convergence remains mediocre. We shall explain this in the following section.


A simple Monte Carlo test will allow us to verify this. We simulate a Heston model and another model in which we multiply both Brownian motions by a factor $\Delta t$ . This will make the errors smaller by a factor of 252 for the daily case. We call this model the modified model. After generating 5000 data points with a parameter set $( \omega ^ { * } = 0 . 1 0 , \theta ^ { * } = 1 0 . 0 , \xi ^ { * } = 0 . 0 3 , \rho ^ { * } = - 0 . 5 0 )$ and a drift $\mu _ { S } = 0 . 0 2 5$ , we suppose we know all parameters except $\omega .$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/31a7285ddcb61829fd84a4e2e5914688bccb1bcd9b371963f2787cc4f593b997.jpg)



FIGURE 2.14 Joint EKF Estimation for the Parameter $\rho .$ Prices were simulated with $\Psi ^ { * } = ( 0 . 1 0 , 1 0 . 0 , 0 . 0 3 , - 0 . 5 0 )$ . The convergence remains mediocre. We shall explain this in the following section.


We then apply the JKF to find the estimate ${ \hat { \omega } } .$ We can observe in Figure 2.15 that the filter diverges when applied to the Heston model but converges fast when applied to the modified model. However, in reality we have no control over the observation error, which is precisely the volatility! In a way, this brings up a more fundamental issue regarding the stochastic volatility estimation problem: By definition, volatility represents the noise of the stock process. If we had taken the spot price $S _ { k }$ as the observation and the variance $\nu _ { k }$ as the state, we would have 

$$
S _ {k} = S _ {k - 1} + S _ {k - 1} \mu_ {S} \Delta t + S _ {k - 1} \sqrt {\nu_ {k}} \sqrt {\Delta} t B _ {k}
$$

we would then have an observation function gradient $H = 0$ and the system would be unobservable! It is precisely because we use a Taylor second-order 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/f1d4716dd01e9a6c2fec1a904898cca928f06d2eff0f36c444ebaf312e5ee2f1.jpg)



FIGURE 2.15 Joint EKF Estimation for the Parameter ω Applied to the Heston Model as Well as to a Modified Model Where the Noise is Reduced by a Factor 252. As we can see, the convergence for the modified model is improved dramatically. This justifies our comments on large observation error.


expansion 

$$
\ln (1 + R) \approx R - \frac {1}{2} R ^ {2}
$$

that we obtain access to $\nu _ { k }$ through the observation function. However, the error remains dominant as the first order of the expansion. 

Some [130] have tried 

$$
\ln \left(\ln^ {2} (\frac {S _ {k}}{S _ {k - 1}})\right) \approx \ln (\nu_ {k}) + \ln (\Delta t) + \ln (B _ {k} ^ {2})
$$

and 

$$
\ln (B _ {k} ^ {2}) \sim - 1. 2 7 + \frac {\pi}{\sqrt {2}} \mathcal {N} (0, 1)
$$

but the latter approximation may or may not be valid depending on the problem under study. 

## Parameter Estimation via MLE

As previously stated, one of the principal methods of estimation under the classical framework is the maximization of the likelihood. Indeed this estimation method has many desirable asymptotic properties. Therefore, instead of using the filters alone, we could separate the parameter set $\Psi = ( \omega , \theta , \xi , \rho )$ from the state vector $( \ln S _ { k } , \nu _ { k } )$ and use the Kalman filter for state filtering within each MLE iteration<sup>19</sup> and estimate the parameters iteratively. 

An Illustration Let us first consider the case of the previous illustration 

$$
\xi_ {k} = \xi_ {k - 1} + \pi + 0. 1 0 w _ {k}
$$

and 

$$
z _ {k} = \xi_ {k} + 0. 1 0 u _ {k}
$$

where $\pi \approx 3 . 1 4 1 5 9$ and $w _ { k } , u _ { k }$ are independent Gaussian random variables. Here we take 

$$
x _ {k} = \xi_ {k}
$$

and 

$$
\begin{array}{c} {A _ {k} = H _ {k} = 1} \\ {W _ {k} = U _ {k} = 0. 1} \end{array}
$$

The maximization of the Gaussian likelihood with respect to the parameter π is equivalent to minimizing 

$$
L _ {1: N} = \sum_ {k = 1} ^ {N} \left[ \ln (F _ {k}) + \frac {\tilde {z} _ {k} ^ {2}}{F _ {k}} \right]
$$

with residuals 

$$
\tilde {z} _ {k} = z _ {k} - \hat {z} _ {k} ^ {-} = z _ {k} - \hat {x} _ {k} ^ {-}
$$

and 

$$
F _ {k} = P _ {z _ {k} z _ {k}} = H _ {k} P _ {k} ^ {-} H _ {k} ^ {t} + U _ {k} R _ {k} U _ {k} ^ {t}
$$

Note that we used scalar notations here, and in vectorial notations we would have 

$$
L _ {1: N} = \sum_ {k = 1} ^ {N} \left[ \ln (| \mathbf {F} _ {k} |) + \tilde {\mathbf {z}} _ {k} ^ {t} \mathbf {F} _ {k} ^ {- 1} \tilde {\mathbf {z}} _ {k} \right]
$$

where $| \mathbf { F } _ { k } |$ is the determinant of $\mathbf { F } _ { k }$ . We use the scalar notations for simplicity and also because in the stochastic volatility problem we usually deal with one-dimensional observations (namely, the stock price). 

The minimization via a direction set (Powell) method over 500 artificially generated observation points will provide 

$$
\hat {\pi} = 3. 1 4 5 9 5 3
$$

very quickly. 

Stochastic Volatility Examples For Example 1, the system state vector now becomes 

$$
\mathbf {x} _ {k} = \binom{\ln S _ {k}}{\nu_ {k}}
$$

which means the dimension of our state is now two, and 

$$
\mathbf {x} _ {k} = \mathbf {f} (\mathbf {x} _ {k - 1}, \mathbf {w} _ {k - 1}) = \binom{\ln S _ {k - 1} + \left(\mu_ {S} - \frac {1}{2} \nu_ {k - 1}\right) \Delta t + \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} B _ {k - 1}}{\nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} Z _ {k - 1}}
$$

The system noise is still 

$$
\mathbf {w} _ {k} = \binom{B _ {k}}{Z _ {k}}
$$

and the corresponding covariance matrix is 

$$
\mathbf {Q} _ {k} = \left( \begin{array}{c c} 1 & \rho \\ \rho & 1 \end{array} \right)
$$

We have the measurement $z _ { k } = \ln S _ { k } .$ , and therefore we can write 

$$
\mathbf {H} _ {k} = \left( \begin{array}{c c} 1 & 0 \end{array} \right)
$$

Now for a given set of parameters $( \omega , \theta , \xi , \rho )$ we can filter this system with the EKF (or the UKF) using 

$$
\mathbf {A} _ {k} = \left( \begin{array}{c c} 1 & - \frac {1}{2} \Delta t \\ 0 & 1 - \theta \Delta t \end{array} \right)
$$

and 

$$
\mathbf {W} _ {k} = \left( \begin{array}{c c} \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} & 0 \\ 0 & \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} \end{array} \right)
$$

Note that the observation matrix is 

$$
\mathbf {O} _ {k} = \left( \begin{array}{c c} 1 & 0 \\ 1 & - \frac {1}{2} \Delta t \end{array} \right)
$$

which is of full rank. Our system is therefore observable. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/dd430858d73ef02c04a3cadfe4ad119a303ee9ea9034638ef295cc9238b91711.jpg)



FIGURE 2.16 The SPX Historic Data (1996–2001) is Filtered via EKF and UKF. The results are very close, however, the estimated parameters $\hat { \Psi } \ = \ ( \hat { \omega } , \hat { \theta } , \hat { \xi } , \hat { \rho } )$ differ. Indeed we find $( \hat { \omega } = 0 . 0 7 3 0 2 8 , \hat { \theta } = 1 . 6 4 4 4 8 8 , \hat { \xi } = 0 . 1 9 0 4 6 1 , \hat { \rho } = - 1 . 0 0 0 0 0 0$ for the EKF and $( { \hat { \omega } } = 0 . 5 4 0 7 1 5 , { \hat { \theta } } = 1 3 . 0 1 3 5 7 7 , { \hat { \xi } } = 0 . 4 3 7 5 2 3 , { \hat { \rho } } = - 1 . 0 0 0 0 0 0 )$ for the UKF. This might be due to the relative insensitivity of the filters to the parameter set  or the non-uniqueness of the optimal parameter set. We shall explain this low sensitivity in more detail.


After filtering for this set of parameters, we calculate the sum to be minimized 

$$
\phi (\omega , \theta , \xi , \rho) = \sum_ {k = 1} ^ {N} \left[ \ln (F _ {k}) + \frac {\tilde {z} _ {k} ^ {2}}{F _ {k}} \right]
$$

with 

$$
\tilde {\mathbf {z}} _ {k} = \mathbf {z} _ {k} - \mathbf {h} (\hat {\mathbf {x}} _ {k} ^ {-}, 0)
$$

and 

$$
\mathbf {F} _ {k} = \mathbf {H} _ {k} \mathbf {P} _ {k} ^ {-} \mathbf {H} _ {k} ^ {t} + \mathbf {U} _ {k} \mathbf {R} _ {k} \mathbf {U} _ {k} ^ {t}
$$

The minimization could once again be done via a direction set (Powell) method, as described previously. This will avoid a calculation of the gradient $\nabla \phi .$ 

It is interesting to observe (cf. Figures 2.16 and 2.17) that the results of the EKF and UKF are very close and the filter errors are comparable. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/7dcee74e5ed26cbe43a3e3eb53ca43cd82efefcf72a96679b8f58ef238d10548.jpg)



FIGURE 2.17 EKF and UKF Absolute Filtering-Errors for the Same Time-Series. As we can see, there is no clear superiority of one algorithm over the other.


However, the estimated parameter set $\Psi = ( \omega , \theta , \xi , \rho )$ can have a different set of values depending on which filter is actually used.<sup>20</sup> 

This leads us to the question, how sensitive are these filters to ? In order to answer, we can run an estimation for EKF and use the estimated parameters in UKF and observe how good a fit we obtain. The results show that this sensitivity is fairly low. Again, this might be due to the relative insensitivity of the filters to the parameter set  or the non-uniqueness of the optimal parameter set. As we will see, the answer to this question also depends on the sample size. 

Optimization Constraints for the Square Root Model In terms of the optimization constraints, in addition to the usual 

$$
\begin{array}{c} \omega \geq 0 \\ \theta \geq 0 \\ \xi \geq 0 \\ - 1 \leq \rho \leq 1 \end{array}\tag{2.12}
$$

we need to make sure that the value of the variance remains positive; that is, 

$$
\nu_ {k} + (\omega - \theta \nu_ {k}) \Delta t + \xi \sqrt {\nu_ {k}} \sqrt {\Delta t} Z _ {k} \geq 0
$$

for any $\nu _ { k } \ge 0$ and any Gaussian random value $Z _ { k }$ . For a Gaussian random variable $Z _ { k }$ and any positive real number $Z ^ { * }$ , we can write $Z _ { k } \geq - Z ^ { * }$ with a probability $P ^ { * }$ . For instance if $Z ^ { * } = 4$ then $P ^ { * } = 0 . 9 9 9 9 6 8$ . Therefore, fixing a choice of $Z ^ { * }$ , it is almost always enough for us to have 

$$
\nu_ {k} + (\omega - \theta \nu_ {k}) \Delta t - \xi \sqrt {\nu_ {k}} \sqrt {\Delta t} Z ^ {*} \geq 0
$$

for any $\nu _ { k } \ge 0$ 

Considering the function $f ( x ) = x + ( \omega - \theta x ) \Delta t - \xi \sqrt { x } \sqrt { \Delta t } Z ^ { * }$ , it is fairly easy to see that $f ( 0 ) = \omega \Delta t \geq 0$ by assumption, and for x very large $f ( x ) \approx ( 1 - \theta \Delta t ) x$ , which is positive if 

$$
\theta \leq \frac {1}{\Delta t}\tag{2.13}
$$

This is most of the time realized for a small $\Delta t$ such as ours. 

Now $f ( x )$ being a continuous function and having positive values at zero and infinity, it would be sufficient to make sure that its one minimum on $[ 0 , + \infty ]$ is also positive. A simple derivative computation shows that $\begin{array} { r } { x _ { m i n } = \frac { \xi ^ { 2 } \Delta t ( Z ^ { * } ) ^ { 2 } } { 4 ( 1 - \theta \Delta t ) ^ { 2 } } } \end{array}$ and therefore the positivity is realized $\mathrm { i f } ^ { 2 1 }$ 

$$
\xi \leq \frac {2}{Z ^ {*}} \sqrt {\omega (1 - \theta \Delta t)}\tag{2.14}
$$

which completes our set of constraints. 

An Alternative Implementation We could also perform the same estimation, but based on our previous third example. Again we have 

$$
\begin{array}{c} \ln S _ {k} = \ln S _ {k - 1} + \left(\mu_ {S} - \frac {1}{2} \nu_ {k}\right) \Delta t + \sqrt {\nu_ {k}} \sqrt {\Delta t} B _ {k} \\ \nu_ {k} = \nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} Z _ {k} \end{array}
$$

with $B _ { k }$ and $Z _ { k }$ two normal random sequences with a mean of zero, a variance of one, and a correlation equal to $\rho .$ . However, since for a Kalman filter the process noise and the measurement noise must be uncorrelated, we introduce 

$$
y _ {k} = \sqrt {\nu_ {k}} Z _ {k}
$$

and performing the usual Cholesky factorization $B _ { k } = \rho Z _ { k } + \sqrt { 1 - \rho ^ { 2 } } X _ { k } .$ where $Z _ { k }$ and $X _ { k }$ are uncorrelated, we can write 

$$
\mathbf {x} _ {k} = \binom{\nu_ {k}}{y _ {k}}
$$

and $\mathbf { x } _ { k } = \mathbf { f } ( \mathbf { x } _ { k - 1 } , Z _ { k } )$ with 

$$
\mathbf {f} (x _ {k - 1}, Z _ {k}) = \binom{\nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} Z _ {k}}{(\nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} Z _ {k}) ^ {\frac {1}{2}} Z _ {k}}
$$

which provides us with the Jacobian 

$$
\mathbf {A} _ {k} = \left( \begin{array}{c c} 1 - \theta \Delta t & 0 \\ 0 & 0 \end{array} \right)
$$

and 

$$
\mathbf {W} _ {k} = \binom{\xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t}}{(\nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t) ^ {\frac {1}{2}}}
$$

The measurement equation is 

$$
z _ {k} = \ln S _ {k} = \ln S _ {k - 1} + \left(\mu_ {S} - \frac {1}{2} \nu_ {k}\right) \Delta t + \rho \sqrt {\Delta t} y _ {k} + \sqrt {1 - \rho^ {2}} \sqrt {\nu_ {k}} \sqrt {\Delta t} X _ {k}
$$

and therefore 

$$
\mathbf {H} _ {k} = \left( \begin{array}{c c} - \frac {1}{2} \Delta t & \rho \sqrt {\Delta t} \end{array} \right)
$$

with $u _ { k } = X _ { k }$ and $U _ { k } = \sqrt { 1 - \rho ^ { 2 } } \sqrt { \nu _ { k } } \sqrt { \Delta t }$ which completes our set of equations. Note that the observation matrix is 

$$
\mathbf {O} _ {k} = \left( \begin{array}{c c} - \frac {1}{2} \Delta t & \rho \sqrt {\Delta t} \\ - \frac {1}{2} \Delta t (1 - \theta \Delta t) & 0 \end{array} \right)
$$

which is of full rank. Our system is therefore observable. 

The One-Dimensional State Finally, a simpler way of writing the state-space system, which will be our method of choice hereafter, would be to subtract from both sides of the state equation $x _ { k } = f ( x _ { k - 1 } , w _ { k - 1 } )$ a multiple of the quantity $b ( x _ { k - 1 } , u _ { k - 1 } ) - z _ { k - 1 } .$ , which is equal to zero. This would allow us to eliminate the correlation between the system and the measurement noises. 

In fact, if the system equation is 

$$
\ln S _ {k} = \ln S _ {k - 1} + \left(\mu_ {S} - \frac {1}{2} \nu_ {k - 1}\right) \Delta t + \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} B _ {k - 1}
$$

$$
\nu_ {k} = \nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} Z _ {k - 1}
$$

writing 

$$
\begin{array}{r l} & {\nu_ {k} = \nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} Z _ {k - 1}} \\ & {- \rho \xi \bigg [ \ln S _ {k - 1} + \bigg (\mu_ {S} - \frac {1}{2} \nu_ {k - 1} \bigg) \Delta t + \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} B _ {k - 1} - \ln S _ {k} \bigg ]} \end{array}
$$

posing for every k 

$$
\tilde {Z} _ {k} = \frac {1}{\sqrt {1 - \rho^ {2}}} (Z _ {k} - \rho B _ {k})
$$

we will have as expected $\tilde { Z } _ { k }$ uncorrelated with $B _ { k }$ and 

$$
\begin{array}{l} x _ {k} = \nu_ {k} = \nu_ {k - 1} + \left[ (\omega - \rho \xi \mu_ {S}) - \left(\theta - \frac {1}{2} \rho \xi\right) \nu_ {k - 1} \right] \Delta t \\ \quad + \rho \xi \ln \left(\frac {S _ {k}}{S _ {k - 1}}\right) + \xi \sqrt {1 - \rho^ {2}} \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} \tilde {Z} _ {k - 1} \end{array}\tag{2.15}
$$

and the measurement equation would be 

$$
z _ {k} = \ln S _ {k + 1} = \ln S _ {k} + \left(\mu_ {S} - \frac {1}{2} \nu_ {k}\right) \Delta t + \sqrt {\nu_ {k}} \sqrt {\Delta t} B _ {k}\tag{2.16}
$$

With this system everything becomes one-dimensional and the computations become much faster both for the EKF and UKF. 

For the EKF we will have 

$$
A _ {k} = 1 - \left(\theta - \frac {1}{2} \rho \xi\right) \Delta t
$$

and 

$$
W _ {k} = \xi \sqrt {1 - \rho^ {2}} \sqrt {\nu_ {k - 1}} \sqrt {\Delta t}
$$

as well as 

$$
H _ {k} = - \frac {1}{2} \Delta t
$$

and 

$$
U _ {k} = \sqrt {\nu_ {k}} \sqrt {\Delta t}
$$

Again, for the MLE we will try to minimize 

$$
\phi (\omega , \theta , \xi , \rho) = \sum_ {k = 1} ^ {N} \left[ \ln (F _ {k}) + \frac {\tilde {z} _ {k} ^ {2}}{F _ {k}} \right]
$$

with residuals 

$$
\tilde {\mathbf {z}} _ {k} = \mathbf {z} _ {k} - \mathbf {h} (\hat {\mathbf {x}} _ {k} ^ {-}, 0)
$$

and 

$$
\mathbf {F} _ {k} = \mathbf {H} _ {k} \mathbf {P} _ {k} ^ {-} \mathbf {H} _ {k} ^ {t} + \mathbf {U} _ {k} \mathbf {U} _ {k} ^ {t}
$$

The same time update and measurement update will be used with the UKF. The ML estimator can be used as usual. 

The following is a C++ routine for the implementation of the EKF applied to the Heston model: 

```c
// log_stock_prices are the log of stock prices
// muS is the real-world stock drift
// n_stock_prices is the number of the above stock prices
// (omega, theta, xi, rho) are the Heston parameters
// u[] is the set of means of observation errors
// v[] is the set of variances of observation errors
// estimates[] are the estimated observations from the filter

void estimate_extended_kalman_parameters_1_dim(
double *log_stock_prices,
double muS,
int n_stock_prices,
double omega,
double theta,
double xi,
double rho,
double *u,
double *v,
double *estimates)
{
    int i1;
    double x, x1, W, H, A;
    double P, P1, z, U, K;
    double delt=1.0/252.0;
    double eps=0.00001;

    x = 0.04;
    P=0.01;
    u[0]=u[n_stock_prices-1]=0.0;
    v[0]=v[n_stock_prices-1]=1.0;
    estimates[0]=estimates[1]=log_stock_prices[0]+eps;

    for (i1=1;i1<n_stock_prices-1;i1++)
    {
    if (x<0) x=0.00001; 
```

```txt
x1 = x + (omega-rho*xi*muS - (theta-0.5*rho*xi) * x) * delt +
    rho*xi* (log_stock_prices[i1] - log_stock_prices[i1-1]);
A = 1.0 - (theta-0.5*rho*xi)*delt;
W = xi*sqrt((1-rho*rho) * x * delt);
P1 = W*W + A*P*A;

if (x1<0) x1=0.00001;

H = -0.5*delt;
U = sqrt(x1*delt);
K = P1*H/( H*P1*H + U*U);
z = log_stock_prices[i1+1];
x = x1 + K * (z - (log_stock_prices[i1] + (muS-0.5*x1)*delt));

u[i1] = z - (log_stock_prices[i1] + (muS-0.5*x1)*delt);
v[i1] = H*P1*H + U*U;
estimates[i1+1] = log_stock_prices[i1] + (muS-0.5*x1)*delt;

P=(1.0-K*H)*P1;
}

// Having u[] and v[] we can evaluate the (minus log) Likelihood as
// the sum of log(v[i1]) + u[i1]*u[i1]/v[i1]
// and minimize the sum in order to obtain the optimal parameters
// the minimization could be done for instance via the direction set routine
// available in the Numerical Recipes in C 
```

And what follows next is the same routine for the unscented filter. 

```txt
void estimate_unscented_kalman_parameters_1_dim(
    double *log_stock_prices,
    double muS,
    int n_stock_prices,
    double omega,
    double theta, double xi,
    double rho,
    double *u,
    double *v,
    double *estimates) 
```

```lisp
int i1,i2, i3, t1;
int ret;
int na=3;
double x, xa[3];
double X[7], Xa[3][7];
double Wm[7], Wc[7], Z[7];
double x1;
double prod, prod1;
double P, P1;
double **Pa, **proda;
double z, U, Pzz, K;
double delt=1.0/252.0;
double a=0.001, b=0.0, k=0.0, lambda;
double eps=0.00001;

lambda = a*a*(na +k)-na;

proda=new double * [na];
Pa = new double * [na];
for (i1=0;i1<na;i1++)
{
    Pa[i1]= new double [na];
    proda[i1]= new double [na];
}

xa[1]=xa[2]=0.0;
x= 0.04;
u[0]=u[n_stock_prices-1]=0.0;
v[0]=v[n_stock_prices-1]=1.0;
estimates[0]=estimates[1]=log_stock_prices[0]+eps;
xa[0]=x;

Pa[0][0]= Pa[1][1]= Pa[2][2] = 1.0;
Pa[1][0]= Pa[0][1]= Pa[1][2]=Pa[2][1]= Pa[0][2]=Pa[2][0]=0;

for (i1=0;i1<na;i1++)
{
    for (i2=0;i2<na;i2++)
    {
    proda[i1][i2]=0.0;
    }
}

Wm[0]=lambda/(na+lambda); 
```

```lisp
Wc[0]=lambda/(na+lambda) + (1-a*a+b);
for (i3=1;i3<(2*na+1);i3++)
{
    Wm[i3]=Wc[i3]=1/(2*(na+lambda));
}

for (t1=1;t1<n_stock_prices-1;t1++)
{
    for (i1=0;i1<na;i1++)
    {
    Xa[i1][0]=xa[i1];
    }

    for (i1=0;i1<na;i1++)
    {
    for (i2=0;i2<na;i2++)
    {
    if (i1==i2)
    {
    if (Pa[i1][i2]<1.0e-10)
    Pa[i1][i2]=1.0e-10;
    }
    else
    {
    if (Pa[i1][i2]<1.0e-10)
    Pa[i1][i2]=0.0;
    }
    }
    }

    ret = sqrt_matrix(Pa,proda,na);

    for (i3=1;i3<(1+na);i3++)
    {
    for (i1=0;i1<na;i1++)
    {
    Xa[i1][i3]=xa[i1] + sqrt(na+lambda) * proda[i1][i3-1];
    }
    }
    for (i3=(1+na);i3<(2*na+1);i3++)
    {
    for (i1=0;i1<na;i1++)
    {
    Xa[i1][i3]=xa[i1] - sqrt(na+lambda) * proda[i1][i3-na-1];
    }
} 
```

```c
}
for (i3=0;i3<(2*na+1);i3++)
{
    if (Xa[0][i3]<0) Xa[0][i3]=0.0001;
    X[i3]= Xa[0][i3] + (omega-muS*rho*xi - (theta-0.5*rho*xi) *Xa[0][i3])*delt +
rho*xi* (log_stock_prices[t1]-log_stock_prices[t1-1]) + xi*sqrt((1-rho*rho)*delt*Xa[0][i3])*Xa[1][i3];
}

x1 = 0;
for (i3=0;i3<(2*na+1);i3++)
{
    x1 += Wm[i3]*X[i3];
}

P1=0.0;
for (i3=0;i3<(2*na+1);i3++)
{
    P1 += Wc[i3]*(X[i3]-x1)*(X[i3]-x1);
}

z=0;
for (i3=0;i3<(2*na+1);i3++)
{
    if (X[i3]<0) X[i3]=0.00001;
    Z[i3] = log_stock_prices[t1] + (muS-0.5*X[i3])*delt + sqrt(X[i3]*delt)*Xa[2][i3];
    z += Wm[i3]*Z[i3];
}

Pzz=0;
for (i3=0;i3<(2*na+1);i3++)
{
    Pzz += Wc[i3]*(Z[i3]-z)*(Z[i3]-z);
}

prod=0.0;
for (i3=0;i3<(2*na+1);i3++)
{
    prod += Wc[i3]*(X[i3]-x1)*(Z[i3]-z);
} 
```

```txt
K= prod/Pzz;

    u[t1] = log_stock_prices[t1+1] - z;
    v[t1] = Pzz;
    estimates[t1+1] = z;

    x = x1 + K*(log_stock_prices[t1+1] - z);
    P = P1 - K*K * Pzz;

    xa[0]=x;
    Pa[0][0] = P;

    if (x<0) x=0.0001;

    Pa[1][0] = Pa[0][1] = Pa[1][2]=Pa[2][1] = Pa[0][2]=Pa[2][0]=0;
    }

    for (i1=0;i1<na;i1++)
    {
    delete [] Pa[i1];
    delete [] proda[i1];
    }
    delete [] Pa;
    delete [] proda;

    }

    // the routine sqrt_matrix() can be constructed via the Cholesly decomposition
    // also available as choldc() in the Numerical Recipes in C 
```

Other stochastic volatility models It is easy to generalize the above state-space model to other stochastic volatility approaches. Indeed we could replace the Heston equation with 

$$
\nu_ {k} = \nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \nu_ {k - 1} ^ {p} \sqrt {\Delta t} Z _ {k}
$$

where $ \mathit { p } = 1 / 2$ would naturally correspond to the Heston model, $p = 1$ to the GARCH diffusion-limit model, and $ \mathit { p } = 3 / 2$ to the $\frac 3 2$ model described in [177]. This idea will be developed further in the chapter. 

## Diagnostics

After having estimated the parameter set , we should test for model misspecification. Two important questions are 

1. Do the normalized residuals $( { \bf z } _ { k } - \hat { \bf z } _ { k } ^ { - } ) / { \bf F } _ { k }$ follow a standard normal $\mathcal { N } ( 0 , 1 )$ law? 

2. Do these residuals have zero auto correlation? 

Chi-Square Test The first question could be answered by performing a chisquare test. We take a number $N _ { B }$ of intervals or “bins” bounded by the points $x _ { 0 } , x _ { 1 } , . . . , x _ { J }$ . We then count the number of observations $N _ { j }$ within each bin $[ x _ { j } , x _ { j + 1 } ]$ for j between zero and $N _ { B } - 1$ . We then compare these numbers with the theoretical numbers implied by the normal distribution $n _ { j } = [ \Phi ( x _ { j + 1 } ) - \Phi ( x _ { j } ) ] N$ with  the cumulative normal function and N the total number of observations. The sum 

$$
\sum_ {j = 0} ^ {N _ {B} - 1} \frac {(N _ {j} - n _ {j}) ^ {2}}{n _ {j}}
$$

asymptotically follows a $\chi _ { \nu } ^ { 2 }$ law with degrees of freedom ν equal to $N _ { B } - 1$ 

Box-Ljung Test The second question could be answered with a Box-Ljung test. We should first calculate a number of autocorrelations 

$$
r _ {k} = \frac {\sum_ {i = 1} ^ {N - k} (\tilde {z} _ {i} - \bar {\tilde {z}}) (\tilde {z} _ {i + k} - \bar {\tilde {z}})}{\sum_ {i = 1} ^ {N} (\tilde {z} _ {i} - \bar {\tilde {z}}) ^ {2}}
$$

for k between one and a prespecified integer K. Once again, $\tilde { z } _ { i } = z _ { i } - \hat { z } _ { i } ^ { - }$ and $\bar { \tilde { z } }$ corresponds to their mean. We then consider the sum 

$$
N (N + 2) \sum_ {k = 1} ^ {K} \frac {r _ {k} ^ {2}}{N - k}
$$

which asymptotically follows a $\chi _ { \nu } ^ { 2 }$ law with degrees of freedom ν equal to $K - p$ where $p = 4$ is the numbers of parameters we estimated. 

Test Results In the previously studied SPX examples, we had $N = 1 2 5 6$ . For the normality test, we choose $N _ { B } = 2 1$ and for the Box-Ljung test we take $K \ : = \ : 2 4 ;$ in both cases, we will have to compare the outputs to the critical threshold $\chi _ { 2 0 } ^ { 2 }$ , which for a confidence of 0.95 is around 31.5. For the (one-dimensional) EKF, we obtain 27.738862 for the normality test and 0.007889 for the Box-Ljung test. For the (one-dimensional) UKF, we obtain 22.657545 for the normality test and again 0.016053 for the Box-Ljung test. This means that there is very little autocorrelation in our system noise. Also, it seems reasonable to model the noise as approximately normally distributed. The chi-square test proves that the normality assumption is plausible and the Kalman filter can be used. A visual confirmation of this could be achieved by plotting the corresponding histograms. As we can see in Figure 2.18, there are no excessively “fat tails”; however, the central value at zero is higher than the normal distribution. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/af727f38cf6e468e26758fdc33b94f185a1e764aea0ca4de127b17d168b52350.jpg)



FIGURE 2.18 Histogram for Filtered Data via EKF versus the Normal Distribution. The residuals are fairly normal.


Variogram Similarly to Fouque et al. [104], we can use a variogram to visualize the volatility behavior of the model. As Galli [110] mentions, the main reasons to use variograms instead of covariance or correlograms are that variograms do not need to estimate the mean, and they are interpretable under wider conditions than are covariances or correlograms. 

The expression for the variogram of a process $I _ { t }$ is 

$$
\gamma_ {I} (b) = \frac {1}{2} \mathbf {E} [ (I (t + b) - I (t)) ^ {2} ] \approx \frac {1}{2 N _ {b _ {i}}} \sum_ {t = 0} ^ {N _ {b _ {i}}} (I (t + b _ {i}) - I (t)) ^ {2}
$$

where $N _ { b _ { i } }$ is the total number of points such that $I ( t + b _ { i } )$ exists. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/a87c3519f770124d6871a88f9b8a2e3a2e9815113553acf65de9a19397141527.jpg)



FIGURE 2.19 Variograms for Filtered Data via EKF and UKF. The input corresponds to a sequence of independent Gaussian random variables. As we can see, the variograms are close to one.


For instance, for a sequence of independent Gaussian random variables, we should have 

$$
\gamma_ {I} (b) = \frac {1}{2} \mathbf {E} [ I ^ {2} (t + b) ] + \frac {1}{2} \mathbf {E} [ I ^ {2} (t) ] - \mathbf {E} [ I (t) I (t + b) ] = \frac {1}{2} + \frac {1}{2} - 0 = 1
$$

In our case, the process $I _ { t }$ could be defined, for instance, as 

$$
I _ {t} = \frac {z _ {t} - \hat {z} _ {t} ^ {-}}{\sqrt {F _ {t}}}
$$

which should correspond to a sequence of independent Gaussian random variables. 

As we can see in Figure 2.19, the variogram is consistent with the Gaussian assumption, which reconfirms what we observed from the histograms. Another way of expressing the same idea is to build a Brownian motion from the foregoing sequence. Calling the independent Gaussian random variables $( B _ { k } )$ , we can write 

$$
I _ {n} = \sqrt {\Delta t} \sum_ {k = 0} ^ {n} B _ {k}
$$

and plot the variogram for the Brownian Motion $I _ { n }$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/fa1ba795457a8fa8820432c46227eb03c0cc12f7f3021697994240c3bd6a02cf.jpg)



FIGURE 2.20 Variograms for Filtered Data via EKF and UKF. The input corresponds to a Brownian motion. As we can see, the variograms are close to $x / 2$


For a Brownian motion, it is easy to see that the variogram should be linear 

$$
\gamma_ {I} (b) = \frac {1}{2} (t + b) + \frac {1}{2} t - t = \frac {1}{2} b
$$

This could indeed be seen in Figure 2.20. 

## Particle Filtering

A different approach to filtering and parameter estimation has recently become popular [79], [122], [171]. In this approach, we use Monte Carlo simulations instead of Gaussian approximations for $( x _ { k } | z _ { k } )$ , as the Kalman or Kushner filters do. This will precisely allow us to deal with fundamentally non-Gaussian situations.<sup>22</sup> 

Underlying Theory The idea is based on the Importance Sampling technique: We can calculate an expected value 

$$
\mathbf {E} [ f (x _ {0: k}) ] = \int f (x _ {0: k}) p (x _ {0: k} | z _ {1: k}) d x _ {0: k}\tag{2.17}
$$

by using a known and simple proposal distribution $q ( \ u )$ 

More precisely, it is possible to write 

$$
\mathbf {E} [ f (x _ {0: k}) ] = \int f (x _ {0: k}) \frac {p (x _ {0 : k} | z _ {1 : k})}{q (x _ {0 : k} | z _ {1 : k})} q (x _ {0: k} | z _ {1: k}) d x _ {0: k}
$$

which could be also written as 

$$
\mathbf {E} [ f (x _ {0: k}) ] = \int f (x _ {0: k}) \frac {w _ {k} (x _ {0 : k})}{p (z _ {1 : k})} q (x _ {0: k} | z _ {1: k}) d x _ {0: k}\tag{2.18}
$$

with 

$$
w _ {k} (x _ {0: k}) = \frac {p (z _ {1 : k} | x _ {0 : k}) p (x _ {0 : k})}{q (x _ {0 : k} | z _ {1 : k})}
$$

defined as the filtering non-normalized weight as step $k$ . 

Proof: 

$$
\begin{array}{c} \frac {p (x _ {0 : k} | z _ {1 : k})}{q (x _ {0 : k} | z _ {1 : k})} = \frac {p (z _ {1 : k} | x _ {0 : k}) p (x _ {0 : k})}{p (z _ {1 : k}) q (x _ {0 : k} | z _ {1 : k})} \\ = \frac {w _ {k} (x _ {0 : k})}{p (z _ {1 : k})} \end{array}
$$

(QED) 

We therefore have 

$$
\mathbf {E} [ f (x _ {0: k}) ] = \frac {\mathbf {E} _ {q} [ w _ {k} (x _ {0 : k}) f (x _ {0 : k}) ]}{\mathbf {E} _ {q} [ w _ {k} (x _ {0 : k}) ]} = \mathbf {E} _ {q} [ \tilde {w} _ {k} (x _ {0: k}) f (x _ {0: k}) ]\tag{2.19}
$$

with 

$$
\tilde {w} _ {k} (x _ {0: k}) = \frac {w _ {k} (x _ {0 : k})}{\mathbf {E} _ {q} [ w _ {k} (x _ {0 : k}) ]}
$$

defined as the filtering normalized weight as step k. 

Proof: We write 

$$
\begin{array}{c} \mathbf {E} [ f (x _ {0: k}) ] = \frac {1}{p (z _ {1 : k})} \int f (x _ {0: k}) w _ {k} (x _ {0: k}) q (x _ {0: k} | z _ {1: k}) d x _ {0: k} \\ = \frac {\int f (x _ {0 : k}) w _ {k} (x _ {0 : k}) q (x _ {0 : k} | z _ {1 : k}) d x _ {0 : k}}{\int p (z _ {1 : k} | x _ {0 : k}) p (x _ {0 : k}) \frac {q (x _ {0 : k} | z _ {1 : k})}{q (x _ {0 : k} | z _ {1 : k})} d x _ {0 : k}} \end{array}
$$

$$
= \frac {\int f (x _ {0 : k}) w _ {k} (x _ {0 : k}) q (x _ {0 : k} | z _ {1 : k}) d x _ {0 : k}}{\int w _ {k} (x _ {0 : k}) q (x _ {0 : k} | z _ {1 : k}) d x _ {0 : k}}
$$

which is the ratio of the expectations, as earlier stated. $( \mathcal { Q } E D )$ 

Using Monte-Carlo sampling from the distribution $q \left( x _ { 0 : k } | z _ { 1 : k } \right)$ we can write in the discrete framework: 

$$
\mathbf {E} [ f (x _ {0: k}) ] \approx \sum_ {i = 1} ^ {N _ {s i m s}} \tilde {w} _ {k} (x _ {0: k} ^ {(i)}) f (x _ {0: k} ^ {(i)})\tag{2.20}
$$

with again 

$$
\tilde {w} _ {k} (x _ {0: k} ^ {(i)}) = \frac {w _ {k} \left(x _ {0 : k} ^ {(i)}\right)}{\sum_ {j = 1} ^ {N _ {s i m s}} w _ {k} \left(x _ {0 : k} ^ {(j)}\right)}
$$

Now supposing that our proposal distribution $q ( \ u )$ satisfies the Markov property, it can be shown that $w _ { k }$ verifies the recursive identity 

$$
w _ {k} ^ {(i)} = w _ {k - 1} ^ {(i)} \frac {p \left(z _ {k} | x _ {k} ^ {(i)}\right) p \left(x _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}\right)}{q \left(x _ {k} ^ {(i)} | x _ {0 : k - 1} ^ {(i)} , z _ {1 : k}\right)}\tag{2.21}
$$

which completes the sequential importance sampling algorithm. 

Proof: The Markov property just mentioned could be written as 

$$
q (x _ {0: k} | z _ {1: k}) = q (x _ {k} | x _ {0: k - 1}, z _ {1: k}) q (x _ {0: k - 1} | z _ {1: k - 1})\tag{2.22}
$$

We also assume that the state $( x _ { k } )$ is a Markov process, meaning 

$$
p (x _ {k} | x _ {0: k - 1}) = p (x _ {k} | x _ {k - 1})
$$

and the observations $( z _ { k } )$ are conditionally independent given the states, so that 

$$
p (z _ {k} | x _ {0: k}) = p (z _ {k} | x _ {k})
$$

Finally we use the fact that at time-step $k _ { : }$ , all previous observations are perfectly known, and 

$$
p (z _ {k} | x _ {k}, z _ {1: k - 1}) = p (z _ {k} | x _ {k})
$$

Therefore 

$$
w _ {k} (x _ {k}) = \frac {p (z _ {1 : k} | x _ {0 : k}) p (x _ {0 : k})}{q (x _ {0 : k} | z _ {1 : k})}
$$

$$
= \frac {p (z _ {k} | x _ {k}) p (z _ {1 : k - 1} | x _ {0 : k - 1}) p (x _ {k} | x _ {k - 1}) p (x _ {0 : k - 1})}{q (x _ {k} | x _ {0 : k - 1} , z _ {1 : k}) q (x _ {0 : k - 1} | z _ {1 : k - 1})}
$$

(QED) 

It is important to note that what the foregoing means is that the state $x _ { k }$ cannot depend on future observations; that is, we are dealing with filtering and not smoothing. 

Resampling One major problem with this algorithm is that the variance of the weights increases randomly over time. In order to solve this, we need to use a resampling algorithm, which would map our unequally weighted $x _ { k } { } ^ { \circ } { \mathrm { s } }$ to a new set of equally weighted sample points. Various methods have been suggested for this. See, for instance, Arulampalam [14], [171]. The basic idea is to compare the cumulative distribution function (CDF) created from the normalized weights with a CDF constructed from a uniformly simulated number [0 1]. We would then eliminate the indices having too small a weight and repeat those having a sufficiently large weight. 

More accurately, at a given time step $k ,$ , for $1 \leq j \leq N _ { s i m s } .$ , if 

$$
\frac {1}{N _ {\text { sims }}} (\mathcal {U} [ 0, 1 ] + j - 1) \geq \sum_ {l = 1} ^ {i} \tilde {w} _ {k} ^ {(l)}
$$

then increment and “skip” $i ;$ otherwise, take $x _ { k } ^ { ( i ) }$ and set its weight to $\frac { 1 } { N _ { s i m s } }$ 

Note that the resampling algorithm could create a situation where the resulting sample has many repeated points. This is known as sample impoverishment and could lead to an extreme case in which all points collapse to a unique particle after a few iterations. This phenomenon is more likely if the process noise is small. One possible solution to this problem is to add a Markov chain Monte Carlo (MCMC) step after the resampling. As will be described further, a Metropolis-Hastings (MH) sampling algorithm would be suitable. 

Needless to say, the choice of the proposal distribution is crucial. Many suggest using 

$$
q (x _ {k} | x _ {0: k - 1}, z _ {1: k}) = p (x _ {k} | x _ {k - 1})
$$

since it will give us a simple weight identity 

$$
w _ {k} ^ {(i)} = w _ {k - 1} ^ {(i)} p (z _ {k} | x _ {k} ^ {(i)})
$$

Based on this type of choice, hereafter we shall simplify and write 

$$
q (x _ {k} | x _ {0: k - 1}, z _ {1: k}) = q (x _ {k} | x _ {k - 1}, z _ {1: k})
$$

without any change to our arguments. However, this choice of the proposal distribution does not take into account our most recent observation $z _ { k }$ at all and therefore could become inefficient. Hence aries the idea of using a 

Gaussian approximation for the proposal and, in particular, an approximation based on the Kalman filter, in order to incorporate the observations. We therefore will have 

$$
q (x _ {k} | x _ {k - 1}, z _ {1: k}) = \mathcal {N} (\hat {x} _ {k}, P _ {k})\tag{2.23}
$$

using the same notations as in the section on the Kalman filter. Such filters are sometimes referred to as the extended particle filter (EPF) or the unscented particle filter (UPF). This is similar to the iterative gentering algorithm in Kushner’s NLF. 

From here, in order to estimate the parameter set  we can either use dual/Joint filter, or use an ML estimator. Note that since the particle filter does not necessarily assume Gaussian noise, the likelihood function to be maximized has a more general form than the one used in previous sections. Given the likelihood at step k 

$$
l _ {k} = p (z _ {k} | z _ {1: k - 1}) = \int p (z _ {k} | x _ {k}) p (x _ {k} | z _ {1: k - 1}) d x _ {k}
$$

the total likelihood is the product of the $l _ { k }  { \mathrm { ^ { * } } }$ and therefore the log likelihood to be maximized is 

$$
\ln (L _ {1: N}) = \sum_ {k = 1} ^ {N} \ln (l _ {k})\tag{2.24}
$$

Now $l _ { k }$ could be written as 

$$
l _ {k} = \int p (z _ {k} | x _ {k}) \frac {p (x _ {k} | z _ {1 : k - 1})}{q (x _ {k} | x _ {k - 1} , z _ {1 : k})} q (x _ {k} | x _ {k - 1}, z _ {1: k}) d x _ {k}
$$

and given that by construction the $x _ { k } ^ { ( i ) }$ ’s are distributed according to $q ( \ u )$ , we can write the Monte Carlo approximation 

$$
l _ {k} \approx \sum_ {i = 1} ^ {N _ {\text {sims}}} \frac {p \left(z _ {k} | x _ {k} ^ {(i)}\right) p \left(x _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}\right)}{q \left(x _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)} , z _ {1 : k}\right)}\tag{2.25}
$$

which we already computed for the sequential importance sampling weight update. 

As we shall see in the next paragraph, it is also possible to interpret the step k likelihood, as a quantity related to the total weight 

$$
\sum_ {i = 1} ^ {N _ {s i m s}} w _ {k} ^ {(i)}
$$

Finally, we could interpret the particle filter as follows. We are using a Monte Carlo simulation (via an importance sampling technique) to calculate the integral $\begin{array} { r } { \int f ( x _ { k } ) \ d p ( x _ { k } | \ d z _ { 1 : k } ) d x _ { k } } \end{array}$ . This is exactly what other filtering techniques try to do. The Kushner nonlinear filter (NLF) tries to calculate the integral via a Gaussian quadrature. Indeed, NLF uses Hermite polynomials because it treats the distributions as normal.<sup>23</sup> 

Implementation Given the above theory, the algorithm for an extended or unscented particle filter could be implemented in the following way: 

1. For time step $k = 0 .$ , choose $x _ { 0 }$ and $P _ { 0 } > 0$ 

For i such that $1 \leq i \leq N _ { s i m s }$ , take 

$$
x _ {0} ^ {(i)} = x _ {0} + \sqrt {P _ {0}} Z ^ {(i)}
$$

where $Z ^ { ( i ) }$ is a standard Gaussian simulated number. Also take $P _ { 0 } ^ { ( i ) } = P _ { 0 }$ and 

$$
w _ {0} ^ {(i)} = \frac {1}{N _ {s i m s}}
$$

While $1 \leq k \leq N$ 

2. For each simulation index i 

$$
\hat {x} _ {k} ^ {(i)} = \mathbf {K F} (x _ {k - 1} ^ {(i)})
$$

with $P _ { k } ^ { ( i ) }$ the associated a posteriori error covariance matrix. (KF could be either the EKF or the UKF.) 

3. For each i between 1 and $N _ { s i m s }$ 

$$
\tilde {x} _ {k} ^ {(i)} = \hat {x} _ {k} ^ {(i)} + \sqrt {P _ {k} ^ {(i)}} Z ^ {(i)}
$$

where again $Z ^ { ( i ) }$ is a standard Gaussian simulated number. 

4. Calculate the associated weights for each i 

$$
w _ {k} ^ {(i)} = w _ {k - 1} ^ {(i)} \frac {p (z _ {k} | \tilde {x} _ {k} ^ {(i)}) p (\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)})}{q (\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)} , z _ {1 : k})}
$$

with $q ( \ u )$ the normal density with mean $\hat { x } _ { k } ^ { ( i ) }$ and variance $P _ { k } ^ { \left( i \right) }$ . 

5. Normalize the weights 

$$
\tilde {w} _ {k} ^ {(i)} = \frac {w _ {k} ^ {(i)}}{\sum_ {i = 1} ^ {N _ {s i m s}} w _ {k} ^ {(i)}}
$$

6. Resample the points $\tilde { x } _ { k } ^ { ( i ) }$ and get $x _ { k } ^ { ( i ) }$ and reset $\begin{array} { r } { w _ { k } ^ { ( i ) } = \tilde { w } _ { k } ^ { ( i ) } = \frac { 1 } { N _ { s i m s } } } \end{array}$ 

7. Increment $k ;$ go back to Step 2 and Stop at the end of the While loop. 

From Step 4 we have 

$$
\bar {l} _ {k} = \sum_ {i = 1} ^ {N _ {\text {sims}}} \frac {p \left(z _ {k} | \tilde {x} _ {k} ^ {(i)}\right) p \left(\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}\right)}{q \left(\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)} , z _ {1 : k}\right)}
$$

where $\bar { l } _ { k }$ is a Monte Carlo proxy for the likelihood $l _ { k }$ at the step k. As we saw in the previous section, by minimizing 

$$
- \sum_ {k = 1} ^ {N} \ln (\bar {l} _ {k})
$$

using, for instance, the direction set algorithm, we will be maximizing the likelihood function and hence we will be obtaining the optimal parameter set $\hat { \Psi }$ . 

Given the resetting of $w _ { k } ^ { ( i ) }$ to a constant $\frac { 1 } { N _ { s i m s } }$ during the resampling step, we can also replace $l _ { k }$ with 

$$
\tilde {l} _ {k} = \sum_ {i = 1} ^ {N _ {s i m s}} w _ {k} ^ {(i)}
$$

which will provide us with an interpretation of the likelihood as the total weight. 

An Illustration Let us consider once again the case of the previous illustration 

$$
\xi_ {k} = \xi_ {k - 1} + \pi + 0. 1 0 w _ {k}
$$

and 

$$
z _ {k} = \xi_ {k} + 0. 1 0 u _ {k}
$$

where $\pi \approx 3 . 1 4 1 5 9$ and $w _ { k } , u _ { k }$ are independent Gaussian random variables. We apply the same Kalman filter and then apply the previous algorithm to the system. Calling 

$$
\mathbf {n} (x, \mathbf {m}, \mathbf {s}) = \frac {1}{\sqrt {2 \pi} \mathbf {s}} \exp \left(- \frac {(x - \mathbf {m}) ^ {2}}{2 \mathbf {s} ^ {2}}\right)
$$

the normal density with mean m and standard deviation s, we will have 

$$
q \left(\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}, z _ {1: k}\right) = \mathbf {n} \left(\tilde {x} _ {k} ^ {(i)}, \mathbf {m} = \hat {x} _ {k} ^ {(i)}, \mathbf {s} = \sqrt {P _ {k} ^ {(i)}}\right)
$$

as well as 

$$
p \left(z _ {k} | \tilde {x} _ {k} ^ {(i)}\right) = \mathbf {n} \left(z _ {k}, \mathbf {m} = \tilde {x} _ {k} ^ {(i)}, \mathbf {s} = 0. 1 0\right)
$$

and 

$$
p \left(\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}\right) = \mathbf {n} \left(\tilde {x} _ {k} ^ {(i)}, \mathbf {m} = x _ {k - 1} ^ {(i)} + \pi , \mathbf {s} = 0. 1 0\right)
$$

Taking 100 particles and 500 observation points, the EPF converges very quickly to $\hat { \pi } = 3 . 1 4 8 2 0 0$ . Alternatively, the simple PF (with no Kalman component) would converge to $\hat { \pi } = 3 . 1 4 0 2 6 6$ 

Note that this example is Gaussian and linear, and therefore the particle filtering is not an improvement over the Kalman filter! Indeed the Kalman filter is optimal for Gaussian linear cases. 

Application to the Heston Model We could now apply the above particle filtering algorithm to our one-dimensional state, where $x _ { k } = \nu _ { k }$ and $z _ { k } = \ln S _ { k + 1 }$ as before. Calling 

$$
\mathbf {n} (x, \mathbf {m}, \mathbf {s}) = \frac {1}{\sqrt {2 \pi} \mathbf {s}} \exp \left(- \frac {(x - \mathbf {m}) ^ {2}}{2 \mathbf {s} ^ {2}}\right)
$$

the normal density with mean m and standard deviation s, we will have 

$$
q \left(\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}, z _ {1: k}\right) = \mathbf {n} \left(\tilde {x} _ {k} ^ {(i)}, \mathbf {m} = \hat {x} _ {k} ^ {(i)}, \mathbf {s} = \sqrt {P _ {k} ^ {(i)}}\right)
$$

as well as 

$$
p \left(z _ {k} | \tilde {x} _ {k} ^ {(i)}\right) = \mathbf {n} \left(z _ {k}, \mathbf {m} = z _ {k - 1} + \left(\mu_ {S} - \frac {1}{2} \tilde {x} _ {k} ^ {(i)}\right) \Delta t, \mathbf {s} = \sqrt {\tilde {x} _ {k} ^ {(i)}} \sqrt {\Delta t}\right)
$$

and 

$$
p \left(\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}\right) =
$$

$$
\mathbf {n} \left(\tilde {x} _ {k} ^ {(i)}, \mathbf {m} = x _ {k - 1} ^ {(i)} + \left[ (\omega - \rho \xi \mu_ {S}) - \left(\theta - \frac {1}{2} \rho \xi\right) x _ {k - 1} ^ {(i)} \right] \Delta t + \rho \xi (z _ {k - 1} - z _ {k - 2}), \mathbf {s}\right)
$$

with 

$$
\mathbf {s} = \xi \sqrt {1 - \rho^ {2}} \sqrt {x _ {k - 1} ^ {(i)}} \sqrt {\Delta t}
$$

which provides us with the densities we need for the filter implementation. 

The estimation of the observable state $z _ { k }$ is 

$$
\hat {z} _ {k} ^ {-} = \frac {1}{N _ {s i m s}} \sum_ {i = 1} ^ {N _ {s i m s}} \hat {z} _ {k} ^ {(i)}
$$

with $\hat { z } _ { k } ^ { ( i ) }$ the estimation of $z _ { k }$ from $\mathbf { K F } ( x _ { k - 1 } ^ { ( i ) } )$ 

Following is a C++ routine for the EPF applied to the Heston model; 1000 particles are being used. 

```lisp
// log_stock_prices are the log of stock prices
// muS is the real-world stock drift
// n_stock_prices is the number of the above stock prices
// (omega, theta, xi, rho) are the Heston parameters
// ll is the value of (negative log) Likelihood function
// estimates[] are the estimated observations from the filter

// The function ran2() is from Numerical Recipes in C
// and generates uniform random variables
// The function Normal_inverse() can be found from many sources
// and is the inverse of the Normal CDF
// Normal_inverse(ran2(.)) generates a set of Normal random variables

void estimate_particle_extended_kalman_parameters_1_dim(
double *log_stock_prices,
double muS,
int n_stock_prices,
double omega,
double theta,
double xi,
double rho,
double *ll,
double *estimates)
{
    int i1, i2, i3;
    double H, A, x0, P0, z;
    int M=1000;
    double x[1000], xx[1000], x1[1000], x2[1000];
    double P[1000], P1[1000], U[1000], K[1000], W[1000];
    double w[1000], u[1000], c[1000];
    double q, pz, px, s, m, l;
    double delt=1.0/252.0, x1_sum;
    long idum=-1;

    A = 1.0-(theta-0.5*rho*xi)*delt;
    H = -0.5*delt;

    x0 = 0.04;
    P0 = 0.000001;
    for (i2=0; i2<M; i2++) 
```

```lisp
{
    x[i2] = x0 + sqrt(P0)* Normal_inverse(ran2(&idum));
    P[i2] = P0;
}

*ll=0.0;
for (i1=1;i1<n_stock_prices-1;i1++)
{
    l = 0.0;
    x1_sum=0.0;
    for (i2=0; i2<M; i2++)
    {
    /* EKF for the proposal distribution */
    if (x[i2]<0) x[i2]=0.00001;
    x1[i2] = x[i2] + (omega-rho*xi*muS - (theta-0.5*rho*xi) * x[i2]) * delt + rho*xi*
    (log_stock_prices[i1]-log_stock_prices[i1-1]);
    W[i2] = xi*sqrt((1-rho*rho) * x[i2] * delt);
    P1[i2] = W[i2]*W[i2] + A*P[i2]*A;
    if (x1[i2]<0) x1[i2]=0.00001;
    U[i2] = sqrt(x1[i2]*delt);
    K[i2] = P1[i2]*H/( H*P1[i2]*H + U[i2]*U[i2]);
    z = log_stock_prices[i1+1];
    x2[i2] = x1[i2] + K[i2] * (z - (log_stock_prices[i1] + (muS-0.5*x1[i2])*delt));
    x1_sum+= x1[i2];
    P[i2]=(1.0-K[i2]*H)*P1[i2];
    /* sample */
    xx[i2] = x2[i2]+sqrt(P[i2])*Normal_inverse(ran2(&idum));
    if (xx[i2]<0) xx[i2]=0.00001;
    /* calculate weights */
    m = x2[i2];
    s = sqrt(P[i2]);
    q = 0.39894228/s * exp(- 0.5* (xx[i2] - m)* (xx[i2] - m)/(s*s));
    m = log_stock_prices[i1] + (muS-0.5*xx[i2])*delt;
    s = sqrt(xx[i2]*delt);
    pz = 0.39894228/s * exp(- 0.5* (z - m)*(z - m)/(s*s));
    m = x[i2] + (omega-rho*xi*muS - (theta-0.5* rho*xi) * x[i2]) * delt + rho*xi*
    (log_stock_prices[i1]-log_stock_prices[i1-1]);
    s = xi*sqrt((1-rho*rho) * x[i2] * delt);
    px = 0.39894228/s * exp(- 0.5* (xx[i2] - m)* (xx[i2] - m)/(s*s)); 
```

```c
w[i2] = pz * px / MAX(q, 1.0e-10);
l += w[i2];
}
*ll += log(l);
estimates[i1+1] = log_stock_prices[i1] + (muS-0.5*x1_sum/M)*delt;
/* normalize weights */
for (i2=0; i2<M; i2++)
    w[i2] /= l;
/* resample and reset weights */
c[0]=0;
for (i2=1; i2<M; i2++)
    c[i2] = c[i2-1] + w[i2];
i2=0;
u[0] = 1.0/M * ran2(&idum);
for (i3=0; i3<M; i3++)
{
    u[i3] = u[0] + 1.0/M *i3;
    while (u[i3] > c[i2])
    i2++;
    x[i3] = xx[i2];
    w[i3] = 1.0/M;
}
}
*ll *= -1.0;
}

// *ll is the value of (negative log) Likelihood function
// we can minimize it to obtain the optimal parameter-set 
```

Next is the same routine for the unscented filter. 

```txt
void estimate_particle_unscented_kalman_parameters_1_dim(
double *log_stock_prices,
double muS,
int n_stock_prices,
double omega,
double theta,
double xi, 
```

```txt
double rho,
double *ll,
double *estimates)
{
    int i1, i2, i3, i4;
    int na=3;
    double x0, P0;
    double Wm[7], Wc[7];
    int M=1000;
    double x[1000], xx[1000], x1[1000], x2[1000], zz[1000], Z[1000][7];
    double X[1000][7], Xa[1000][3][7];
    double xa[1000][3], prod[1000];
    double P[1000], P1[1000], U[1000], K[1000], W[1000], Pzz[1000];
    double w[1000], u[1000], c[1000];
    double ***Pa, ***proda;
    double q, pz, px, s, m, l, z;
    double delt=1.0/252.0;
    long idum=-1;
    int ret;
    double a=0.001, b=0.0, k=0.0, lambda;

    proda = new double ** [M];
    Pa = new double ** [M];
    for (i2=0;i2<M;i2++)
    {
    Pa[i2]= new double * [na];
    proda[i2]= new double * [na];
    for (i1=0;i1<na;i1++)
    {
    Pa[i2][i1]= new double [na];
    proda[i2][i1]= new double [na];
    }
    }

    for (i2=0;i2<M;i2++)
    {
    for (i1=0;i1<na;i1++)
    {
    for (i3=0;i3<na;i3++)
    {
    proda[i2][i1][i3]=0.0; 
```

```txt
}
}
}
lambda = a*a*(na +k) - na;
Wm[0] = lambda / (na + lambda);
Wc[0] = lambda / (na + lambda) + (1 - a*a + b);
for (i3 = 1; i3 < (2 * na + 1); i3++)
{
    Wm[i3] = Wc[i3] = 1 / (2 * (na + lambda));
}

x0 = 0.04;
P0 = 0.000001;
for (i2 = 0; i2 < M; i2++)
{
    x[i2] = x0 + sqrt(P0) * Normal_inverse(ran2(&idum
    P[i2] = P0;

    xa[i2][0] = x[i2];
    xa[i2][1] = xa[i2][2] = 0.0;

    Pa[i2][0][0] = P[i2];
    Pa[i2][1][1] = Pa[i2][2][2] = 1.0;
    Pa[i2][1][0] = Pa[i2][0][1] = Pa[i2][1][2] =
    Pa[i2][2][1] =
    Pa[i2][0][2] = Pa[i2][2][0] = 0.0;
}

*ll=0.0;
for (i1=1;i1<n_stock_prices-1;i1++)
{
    l = 0.0;
    estimates[i1+1]=0.0;
    for (i2=0; i2<M; i2++)
    {
    /* UKF for the proposal distribution */
    for (i3=0;i3<na;i3++)
    {
    Xa[i2][i3][0] = xa[i2][i3];
    }
} 
```

```txt
for (i3=0;i3<na;i3++)
{
    for (i4=0;i4<na;i4++)
    {
    if (i3==i4)
    {
    if (Pa[i2][i3][i4] < 1.0e-10)
    Pa[i2][i3][i4]= 1.0e-10;
    }
    else
    {
    if (Pa[i2][i3][i4] < 1.0e-10)
    Pa[i2][i3][i4] = 0.0;
    }
    }
    }

    ret = sqrt_matrix(Pa[i2],proda[i2],na);

    for (i3=1;i3<(1+na);i3++)
    {
    for (i4=0;i4<na;i4++)
    {
    Xa[i2][i4][i3]= xa[i2][i4] + sqrt(na+lambda) * proda[i2][i4][i3-1];
    }
    }
    for (i3=(1+na);i3<(2*na+1);i3++)
    {
    for (i4=0;i4<na;i4++)
    {
    Xa[i2][i4][i3]= xa[i2][i4] - sqrt(na+lambda) * proda[i2][i4][i3-na-1];
    }
    }

    for (i3=0;i3<(2*na+1);i3++)
    {
    if (Xa[i2][0][i3]<0) Xa[i2][0][i3]=0.0001;
    X[i2][i3]= Xa[i2][0][i3] + (omega-muS*rho*xi - (theta-0.5*rho*xi) *Xa[i2][0][i3])*delt +
    rho*xi*(log_stock_prices[i1]- 
```

```c
log_stock_prices[i1-1]) +
xi*sqrt((1-rho*rho)*delt*Xa[i2][0][i3])* 
Xa[i2][1][i3];
}

x1[i2] = 0;
for (i3=0;i3<(2*na+1);i3++)
{
    x1[i2] += Wm[i3]*X[i2][i3];
}

P1[i2]=0.0;
for (i3=0;i3<(2*na+1);i3++)
{
    P1[i2] += Wc[i3]*(X[i2][i3]-x1[i2])*(X[i2][i3]-
    x1[i2]);
}

zz[i2]=0;
for (i3=0;i3<(2*na+1);i3++)
{
    if (X[i2][i3]<0) X[i2][i3]=0.00001;
    Z[i2][i3] = log_stock_prices[i1] + 
(muS-0.5*X[i2][i3])*delt + sqrt(X[i2][i3]*delt)*Xa[i2][2][i3];
    zz[i2] += Wm[i3]*Z[i2][i3];
}

Pzz[i2]=0;
for (i3=0;i3<(2*na+1);i3++)
{
    Pzz[i2] += Wc[i3]*(Z[i2][i3]-zz[i2])*(Z[i2][i3]-
    zz[i2]);
}

prod[i2]=0.0;
for (i3=0;i3<(2*na+1);i3++)
{
    prod[i2] += Wc[i3]*(X[i2][i3]-x1[i2])*(Z[i2][i3]-
    zz[i2]);
}

K[i2]=prod[i2]/Pzz[i2]; 
```

```c
z = log_stock_prices[i1+1];
estimates[i1+1] += zz[i2]/M;

x2[i2] = x1[i2] + K[i2]*(z - zz[i2]);
P[i2] = P1[i2] - K[i2]*K[i2] * Pzz[i2];

xa[i2][0]=x2[i2];
Pa[i2][0][0] = P[i2];

if (x2[i2]<0) x2[i2]=0.0001;

Pa[i2][1][0]= Pa[i2][0][1]= Pa[i2][1][2]
=Pa[i2][2][1]= Pa[i2][0][2]=Pa[i2][2][0]=[0];
/* sample */
xx[i2] = x2[i2] + sqrt(P[i2])*Normal_inverse(ran2(&idum));
if (xx[i2]<0) xx[i2]=0.00001;
/* calculate weights */
m = x2[i2];
s = sqrt(P[i2]);
q = 0.39894228/s * exp(-0.5*(xx[i2] - m)*
(xx[i2] - m)/(s*s));
m= log_stock_prices[i1] + (muS-0.5*xx[i2])*delt;
s= sqrt(xx[i2]*delt);
pz= 0.39894228/s * exp(-0.5*(z - m)*
(z - m)/(s*s));
m= x[i2] + (omega-rho*xi*muS -
(theta-0.5*rho*xi) * x[i2]) * delt +
rho*xi* (log_stock_prices[i1]-
log_stock_prices[i1-1]);
s= xi*sqrt((1-rho*rho) * x[i2] * delt);
px= 0.39894228/s * exp(-0.5*(xx[i2] - m)*
(xx[i2] - m)/(s*s));

w[i2]= MAX(pz, 1.0e-10) *
MAX(px, 1.0e-10) / MAX(q, 1.0e-10);
l += w[i2];
}
*ll += log(l);
/* normalize weights */ 
```

```txt
for (i2=0; i2<M; i2++)
    w[i2] /= 1;
/* resample and reset weights */
c[0]=0;
for (i2=1; i2<M; i2++)
    c[i2] = c[i2-1] + w[i2];
    i2=0;
    u[0] = 1.0/M * ran2(&idum);
for (i3=0; i3<M; i3++)
{
    u[i3] = u[0] + 1.0/M *i3;
    while (u[i3] > c[i2])
    i2++;
    x[i3] = xx[i2];
    w[i3]=1.0/M;
}
}
*ll *= -1.0;

for (i2=0;i2<M;i2++)
{
    for (i1=0;i1<na;i1++)
    {
    delete [] Pa[i2][i1];
    delete [] proda[i2][i1];
    }
}
for (i2=0;i2<M;i2++)
{
    delete [] Pa[i2];
    delete [] proda[i2];
}
delete [] Pa;
delete [] proda; 
```

Test Results The results from an extended particle filter (EPF) are shown in Figure 2.21. The filter was constructed with the one-dimensional Heston model and was applied to a simulated time series of 5000 points with 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/7dbc50ecbd48925bee8fc5d570e3d7f2514ee6f2b667f501a1d697c7274d36b3.jpg)



FIGURE 2.21 Filtering Errors: Extended Kalman Filter and Extended Particle Filter Are Applied to the One-Dimensional Heston Model. The PF has better performance.


$$
\Psi^ {*} = (0. 4 0, 1 0. 0, 0. 0 1, - 0. 5 0)
$$

As we can see in the figure, no clear superiority of the EPF is detected. The optimal parameters found via EPF are 

$$
\hat {\Psi} _ {E P F} = (0. 0 2 0 3 3 1, 0. 4 9 9 9 8 7, 0. 0 4 0 0 0 0, 0. 0 5 0 0 2 6)
$$

which could not be considered as an improvement over 

$$
\hat {\Psi} _ {E K F} = (0. 0 6 5 8 8 6, 1. 7 1 1 6 8 6, 0. 1 8 0 8 8 4, 0. 1 4 7 6 6 0)
$$

Again the long-term-variances $\frac { \omega } { \theta }$ are close to 0.04 for all cases, which is consistent with what we had observed. 

The next natural step would be to implement and test the unscented particle filter (UPF), in which everything is done similarly to the EPF except for the choice of the proposal distribution. The use of the UPF has been strongly recommended by Wan and Van der Merwe in [231] and [133]. The authors claim that the filtering error from the UPF is considerably smaller than that from EKF, UKF, or EPF. As we can see in Figure 2.22, it is true that the filtering error resulting from UPF is considerably lower than the error generated from the other filters. However, the optimal parameter set 

$$
\hat {\Psi} _ {U P F} = (0. 0 2 0 1 3 2, 0. 5 0 0 0 3 1, 0. 0 4 0 0 0 0, 0. 0 5 0 0 0 4)
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/eb551870980e7e1f94afea5605e868a1f6dea154900d7ce36a31742cfcb5be0a.jpg)



FIGURE 2.22 Filtering Errors: All Filters Are Applied to the One-Dimensional Heston Model. The PF’s have better performance.


obtained via UPF is again very different from the original parameter set $\Psi ^ { * }$ used in the data generation. We shall analyze the reasons behind this poor inference result more closely in the following sections. 

Error Size One possibility is that our time series has too small an error for the filters to make a significant difference. We thus study another case, where $\Delta t = 1$ year. Let us take 200 points generated with the parameter set 

$$
\Psi^ {*} = (0. 0 2, 0. 5, 0. 0 5, - 0. 5)
$$

We obtain 

$$
\hat {\Psi} _ {E K F} = (0. 0 3 6, 0. 0 9 3, 0. 0 3 6, - 1. 0 0)
$$

and 

$$
\hat {\Psi} _ {U K F} = (0. 0 3 3, 0. 0 8 6, 0. 0 3 3, - 0. 9 8)
$$

which shows that UKF results are very close to EKF ones. Using the particle filters, we get 

$$
\hat {\Psi} _ {E P F} = (0. 0 1 9, 0. 5, 0. 0 3, - 0. 5 8)
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/6545750548b18b0078da962516e4b63403d7812a2c8e20b8b41ed7e72bc57d1d.jpg)



FIGURE 2.23 Filters Are Applied to the One-Dimensional Heston Model. The time series has a larger time-step $\Delta t = 1 . 0$ . Naturally, the errors are larger than the case where $\Delta t = 1 / 2 5 2$


which is considerably closer to the original set $\Psi ^ { * }$ . Therefore EPF did bring an improvement over the traditional nonlinear filters and seems to be simpler and more $\mathrm { r o b u s t } ^ { 2 4 }$ than its competitors. 

As for the filtering errors, it can be seen in Figure 2.23 that the EPF errors are smaller than (although comparable to) those produced by EKF and UKF, which is consistent with the particle filtering theory. 

As for UPF, we obtain 

$$
\hat {\Psi} _ {U P F} = (0. 0 1 9 4 8 0, 0. 4 8 9 3 7 5, 0. 0 4 7 0 3 0, - 0. 2 2 9 2 4 2)
$$

which is very close to the EPF result. As we can see, the UPF errors are even smaller than those generated by EPF. In addition to the filters just discussed, it would be interesting to test a Gauss-Hermite filter (GHF) [151]. We obtain 

$$
\hat {\Psi} _ {G H F} = (0. 0 2 0 3 9 8, 0. 5 2 4 2 1 5, 0. 0 6 9 6 6 1, - 1. 0 0 0 0 0 0)
$$

which is closer to the real parameter set $\Psi ^ { * }$ compared with EKF or UKF results. However, the filtering error is more variable than that of its competitors, as can be seen in Figure 2.24. Note, however, that this would mean that we would have access to 200 years of historic data, which is clearly unrealistic.<sup>25</sup> This issue will be revisited in the following sections. Also, here we generated the data via a discrete equation with $\Delta t = 1$ . Thus there was no discretization error from a continuous equation. We cannot apply the same method to data coming from a continuous process. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/a22a27d94ae27ad5a02d6601923bf3c344f0f30d764794aabe947ab4e25d5e01.jpg)



FIGURE 2.24 The EKF and GHF Are Applied to the One-Dimensional Heston Model. The time series has a larger time step $\Delta t = 1 . 0$ . Naturally, the errors are larger than the case where $\Delta t = 1 / 2 5 2$


As a measure of performance, we can compute the mean price error (MPE) as well as the root mean square error (RMSE) for each filter. These correspond respectively to the mean and the standard deviation of the plotted errors. For the MPEs, we obtain 

<table><tr><td></td><td>MPE</td><td>RMSE</td></tr><tr><td>EKF</td><td>0.007484269</td><td>0.003422215</td></tr><tr><td>UKF</td><td>0.007660269</td><td>0.003733748</td></tr><tr><td>GKF</td><td>0.009129157</td><td>0.005816919</td></tr><tr><td>EPF</td><td>0.007620208</td><td>0.002269224</td></tr><tr><td>UPF</td><td>0.007076066</td><td>0.001359393</td></tr></table>

This shows us again that the particle filters outperform the other ones. Again, let us remember that given 200 points with $\Delta t = 1$ and a true parameter set 

$$
\Psi^ {*} = (0. 0 2, 0. 5, 0. 0 5, - 0. 5)
$$

we obtained 

<table><tr><td></td><td><eq>\hat{\omega}</eq></td><td><eq>\hat{\theta}</eq></td><td><eq>\hat{\xi}</eq></td><td><eq>\hat{\rho}</eq></td></tr><tr><td>EKF</td><td>0.036</td><td>0.093</td><td>0.036</td><td>-1.00</td></tr><tr><td>UKF</td><td>0.033</td><td>0.086</td><td>0.033</td><td>-0.98</td></tr><tr><td>GKF</td><td>0.020</td><td>0.524</td><td>0.070</td><td>-1.00</td></tr><tr><td>EPF</td><td>0.019</td><td>0.500</td><td>0.033</td><td>-0.58</td></tr><tr><td>UPF</td><td>0.019</td><td>0.489</td><td>0.047</td><td>-0.22</td></tr></table>

The MH Enhancement As mentioned earlier, the resampling algorithm helps with the issue of degeneracy, which means that it will reduce the variance of the weights. However, it might introduce a sample impoverishment phenomenon, in which all particles will have a tendency to collapse to one. The Metropolis-Hastings (MH) algorithm could be a solution to this problem and is implemented as follows. After resampling, Step 6, we obtain a set $\tilde { \tilde { x } } _ { 1 : k } ^ { ( i ) }$ 

6-a. Reapply the Kalman filter (extended or unscented) to this set in order to obtain 

$$
x _ {k} ^ {* (i)} = K F \left(\tilde {\tilde {x}} _ {k - 1} ^ {(i)}\right)
$$

6-b. Choose between $x _ { k } ^ { * ( i ) }$ and $\tilde { \tilde { x } } _ { k } ^ { ( i ) }$ as follows. Define 

$$
\alpha = m i n \left(1, \frac {p (z _ {k} | x _ {k} ^ {* (i)}) p (x _ {k} ^ {* (i)} | x _ {k - 1} ^ {(i)}) q (\tilde {\tilde {x}} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)} , z _ {1 : k})}{p (z _ {k} | \tilde {\tilde {x}} _ {k} ^ {(i)}) p (\tilde {\tilde {x}} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}) q (x _ {k} ^ {* (i)} | x _ {k - 1} ^ {(i)} , z _ {1 : k})}\right)
$$

then sample v from $\boldsymbol { \mathcal { U } } [ 0 , 1 ]$ and choose $x _ { k } ^ { * ( i ) }$ if $\alpha > \nu$ and choose $\tilde { \tilde { x } } _ { k } ^ { ( i ) }$ if $\alpha \leq \nu$ 

The result is then $x _ { k } ^ { ( i ) }$ , and we go to Step 7 as before. 

Note that α could be interpreted as the ratio of the non-normalized weights for the two particles we are choosing from. Indeed 

$$
\alpha = \alpha_ {k} ^ {(i)} = m i n \left(1, \frac {w (x _ {k} ^ {* (i)})}{w (\tilde {\tilde {x}} _ {k} ^ {(i)})}\right)
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/0ef819625ed8162be39157c0e6c3123dcdf6093e3aeffce5fd23527a2efdf7fa.jpg)



FIGURE 2.25 The EPF Without and with the Metropolis-Hastings Step is Applied to the One-Dimensional Heston Model. The time series has a time step $\Delta t = 1 . 0$ . The improvement is hardly visible.


Applied to the same time series as in the previous paragraphs, the EPF with the MH modification will provide 

$$
\hat {\Psi} _ {E P F - M H} = (0. 0 1 9, 0. 4 9 9, 0. 0 4 0, - 0. 3 5 8)
$$

and 

$$
\begin{array}{r l} M P E _ {E P F - M H} & = 0. 0 0 7 7 5 3 \\ R M S E _ {E P F - M H} & = 0. 0 0 1 9 2 7 \end{array}
$$

compared with the previous EPF 

$$
\begin{array}{c} M P E _ {E P F} = 0. 0 0 7 6 2 \\ R M S E _ {E P F} = 0. 0 0 2 2 6 9 \end{array}
$$

As we can see from these results and Figure 2.25, there is only a marginal improvement from the introduction of the MH step in the filtering process. This is in line with the findings in the literature, such as in [231]. 

## Comparing Heston with other Models

We can now apply our inference tools to real market data in order to see which model matches the true dynamics of the assets more closely, and therefore perform model identification. 

The Models It is easy to generalize the Heston state-space model to other stochastic volatility approaches. Indeed we could replace the Heston state equation with 

$$
\nu_ {k} = \nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \nu_ {k - 1} ^ {p} \sqrt {\Delta t} Z _ {k - 1}\tag{2.26}
$$

where $p = 1 / 2$ would naturally correspond to the Heston (square root) model, $p = 1$ to the GARCH diffusion-limit model, and $ \mathit { p } = 3 / 2$ to the $3 / 2$ model. These models have all been described and analyzed in $[ 1 7 7 ]$ . The new state transition equation would therefore become 

$$
\begin{array}{l} \nu_ {k} = \nu_ {k - 1} + \left[ \omega - \rho \xi \mu_ {S} \nu_ {k - 1} ^ {p - \frac {1}{2}} - \left(\theta - \frac {1}{2} \rho \xi \nu_ {k - 1} ^ {p - \frac {1}{2}}\right) \nu_ {k - 1} \right] \Delta t \\ \qquad + \rho \xi \nu_ {k - 1} ^ {p - \frac {1}{2}} \ln \left(\frac {S _ {k}}{S _ {k - 1}}\right) + \xi \sqrt {1 - \rho^ {2}} \nu_ {k - 1} ^ {p} \sqrt {\Delta t} \tilde {Z} _ {k - 1} \end{array}\tag{2.27}
$$

where the same choice of state space $x _ { k } = \nu _ { k }$ is made. 

For the EKF, we will have 

$$
\begin{array}{l} A _ {k} = 1 - \left[ \rho \xi \mu_ {S} \left(p - \frac {1}{2}\right) \nu_ {k - 1} ^ {p - \frac {3}{2}} + \theta - \frac {1}{2} \rho \xi \left(p + \frac {1}{2}\right) \nu_ {k - 1} ^ {p - \frac {1}{2}} \right] \Delta t \\ \quad + \left(p - \frac {1}{2}\right) \rho \xi \nu_ {k - 1} ^ {p - \frac {3}{2}} \ln \left(\frac {S _ {k}}{S _ {k - 1}}\right) \end{array}
$$

and 

$$
W _ {k} = \xi \sqrt {1 - \rho^ {2}} v _ {k - 1} ^ {p} \sqrt {\Delta t}
$$

as well as 

$$
H _ {k} = - \frac {1}{2} \Delta t
$$

and 

$$
U _ {k} = \sqrt {\nu_ {k}} \sqrt {\Delta t}
$$

The same time update and measurement update equations could be used with the UKF or Kushner’s NLF. 

We could also apply the particle filtering algorithm to our problem. Using the same notations as before and calling 

$$
\mathbf {n} (x, \mathbf {m}, \mathrm{s}) = \frac {1}{\sqrt {2 \pi} \mathrm{s}} \exp \left(- \frac {(x - \mathbf {m}) ^ {2}}{2 \mathrm{s} ^ {2}}\right)
$$

the normal density with mean m and standard deviation s, we will have 

$$
q (\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}, z _ {1: k}) = \mathbf {n} \left(\tilde {x} _ {k} ^ {(i)}, \mathbf {m} = \hat {x} _ {k} ^ {(i)}, \mathbf {s} = \sqrt {P _ {k} ^ {(i)}}\right)
$$

as well as 

$$
p (z _ {k} | \tilde {x} _ {k} ^ {(i)}) = \mathbf {n} \left(z _ {k}, \mathbf {m} = z _ {k - 1} + \left(\mu_ {S} - \frac {1}{2} \tilde {x} _ {k} ^ {(i)}\right) \Delta t, \mathbf {s} = \sqrt {\tilde {x} _ {k} ^ {(i)}} \sqrt {\Delta t}\right)
$$

and 

$$
p \left(\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}\right) = \mathbf {n} \left(\tilde {x} _ {k} ^ {(i)}, \mathbf {m} _ {\mathbf {x}}, \mathbf {s} = \xi \sqrt {1 - \rho^ {2}} \left(x _ {k - 1} ^ {(i)}\right) ^ {p} \sqrt {\Delta t}\right)
$$

with 

$$
\begin{array}{l} \mathbf {m} _ {\mathbf {x}} = x _ {k - 1} ^ {(i)} + \left[ \omega - \rho \xi \mu_ {S} \left(x _ {k - 1} ^ {(i)}\right) ^ {p - \frac {1}{2}} - \left(\theta - \frac {1}{2} \rho \xi \left(x _ {k - 1} ^ {(i)}\right) ^ {p - \frac {1}{2}}\right) x _ {k - 1} ^ {(i)} \right] \Delta t \\ \qquad + \rho \xi \left(x _ {k - 1} ^ {(i)}\right) ^ {p - \frac {1}{2}} (z _ {k - 1} - z _ {k - 2}) \end{array}
$$

and as before we have 

$$
w _ {k} ^ {(i)} = w _ {k - 1} ^ {(i)} \frac {p \left(z _ {k} | \tilde {x} _ {k} ^ {(i)}\right) p \left(\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}\right)}{q \left(\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)} , z _ {1 : k}\right)}
$$

which provides us with what we need for the filter implementation. 

The Results The preceding filters were applied to five years of S&P 500 time series (1996 to 2001 ), and the filtering errors were considered for the Heston, the GARCH, and the $3 / 2$ models. Daily index closing prices were used for this purpose, and the time interval was set to $\Delta t = 1 / 2 5 2$ (see the following table; Figures 2.26 through 2.32). 

<table><tr><td>Filter and Model</td><td>MPE</td><td>RMSE</td></tr><tr><td>EKF-Heston</td><td>3.58207e-05</td><td>1.83223e-05</td></tr><tr><td>EKF-GARCH</td><td>2.78438e-05</td><td>1.42428e-05</td></tr><tr><td>EKF-3/2</td><td>2.63227e-05</td><td>1.74760e-05</td></tr><tr><td>UKF-Heston</td><td>3.00000e-05</td><td>1.91280e-05</td></tr><tr><td>UKF-GARCH</td><td>2.99275e-05</td><td>2.58131e-05</td></tr><tr><td>UKF-3/2</td><td>2.82279e-05</td><td>1.55777e-05</td></tr><tr><td>EPF-Heston</td><td>2.70104e-05</td><td>1.34534e-05</td></tr><tr><td>EPF-GARCH</td><td>2.48733e-05</td><td>4.99337e-06</td></tr><tr><td>EPF-3/2</td><td>2.26462e-05</td><td>2.58645e-06</td></tr><tr><td>UPF-Heston</td><td>2.04000e-05</td><td>2.74818e-06</td></tr><tr><td>UPF-GARCH</td><td>2.63036e-05</td><td>8.44030e-07</td></tr><tr><td>UPF -3/2</td><td>1.73857e-05</td><td>4.09918e-06</td></tr></table>

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/570ad62609ee63864290a7671704798442e581de05efa521998783a1d683ee8c.jpg)



FIGURE 2.26 Comparison of EKF Filtering Errors for Heston, GARCH, and 3/2 Models. The latter seems to perform better.



UKF Errors for Various SV Models


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/baf34ce03ee772b0485d61fdf5c290a76573dbdbdc787aeb07008e312a97703c.jpg)



FIGURE 2.27 Comparison of UKF Filtering Errors for Heston, GARCH, and 3/2 Models. The latter seems to perform better.


Two immediate observations can be made: On one hand, particle filters have a better performance than do the Gaussian, which reconfirms what one would anticipate. On the other hand, for most of the filters, the 3/2 model seems to outperform the Heston model, which is in line with the findings of Engle & Ishida [95]. Again, this shows that the filtering process could be used not only for parameter estimation but also for model identification. This suggests further filtering on other existing models, such as jump diffusion [190]. Clearly, because of the non-Gaussianity of jump-based models, the particle filtering technique will need to be applied to them. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/f42fe731b1e1b1e6d86235b46892402d56fe61a39a99bb59f63d9cb8e87b0f0b.jpg)



FIGURE 2.28 Comparison of EPF Filtering Errors for Heston, GARCH, and 3/2 Models. The latter seems to perform better.



UPF Errors for Various SV Models


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/45600f0d37ac0ff55f89647b113569a27dd2beffba653da0e75437288271f412.jpg)



FIGURE 2.29 Comparison of UPF Filtering Errors for Heston, GARCH, and 3/2 Models. The latter seems to perform better.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/6185cacb8024e4ad76176766520d6f029963268201aab0ec57b4ad803b535956.jpg)



FIGURE 2.30 Comparison of Filtering Errors for the Heston Model. PFs seem to perform better.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/b3c01b9c8596fdedae72ed0b507757ea0073e4f2deeaac3da091e203626a50ae.jpg)



FIGURE 2.31 Comparison of Filtering Errors for the GARCH Model. PFs seem to perform better.


Parameter Learning Revisited We tried a joint filter (JF) via the Kalman filter where the parameters were given a prior distribution. We can now apply the particle filtering techniques to this framework as in [176] and [224]: We simulate $x _ { k } ^ { ( i ) }$ at time step k from the prior $p ( x _ { k } | x _ { k - 1 } ^ { ( i ) } )$ , and we also simulate each parameter $\boldsymbol { \psi } ^ { ( i ) }$ from its prior $q ( \psi ) = \mathcal { N } ( m _ { \psi } , s _ { \psi } )$ where these mean and standard deviations are to be determined. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/157e877cf48ac26687c638522bf039c7508f4ea38651d9f0c7413c2b682bbc7f.jpg)



FIGURE 2.32 Comparison of Filtering Errors for the 3/2 Model. PFs seem to perform better.


We then update the priors by incorporating the observation $z _ { k }$ 

$$
p \left(x _ {k} ^ {(i)} | z _ {k}\right) \propto p \left(z _ {k} | x _ {k} ^ {(i)}, \psi^ {(i)}\right) p \left(x _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}\right)
$$

and similarly 

$$
p (\psi^ {(i)} | z _ {k}) \propto p (z _ {k} | x _ {k} ^ {(i)}, \psi^ {(i)}) p (\psi^ {(i)} | x _ {k - 1} ^ {(i)})
$$

and we obtain the posterior distributions. Calling 

$$
w _ {k} ^ {(i)} = \frac {p (z _ {k} | x _ {k} ^ {(i)} , \psi^ {(i)}) w _ {k - 1} ^ {(i)}}{\sum_ {i = 1} ^ {N _ {s i m s}} p (z _ {k} | x _ {k} ^ {(i)} , \psi^ {(i)}) w _ {k - 1} ^ {(i)}}
$$

We now have the posteriors of $x _ { k }$ and $\psi ,$ and we can simulate them for the following step via a Metropolis-Hastings (MH) accept/reject technique with the proposal distribution $q ( \psi , m _ { \psi } , s _ { \psi } )$ with 

$$
m _ {\psi} = \sum_ {i = 1} ^ {N _ {s i m s}} w _ {k} ^ {(i)} \psi^ {(i)}
$$

and 

$$
s _ {\psi} = \sum_ {i = 1} ^ {N _ {s i m s}} w _ {k} ^ {(i)} \left(\psi^ {(i)} - m _ {\psi}\right) ^ {2}
$$

TABLE 2.2 The True Parameter Set $\Psi ^ { * }$ Used for Data Simulation 

$$
\Psi^ {*}
$$

$$
\omega^ {*} = 0. 1 0
$$

$$
\theta^ {*} = 1 0. 0
$$

$$
\xi^ {*} = 0. 0 3
$$

$$
\rho^ {*} = - 0. 5 0
$$

TABLE 2.3 The Initial Parameter Set $\Psi _ { 0 }$ Used for the Optimization Process 

$$
\Psi_ {0}
$$

$$
\omega_ {0} = 0. 1 5
$$

$$
\theta_ {0} = 1 5. 0
$$

$$
\xi_ {0} = 0. 0 2
$$

$$
\rho_ {0} = - 0. 5 0
$$

The MH step will consist of the following. We accept the simulation point $\tilde { \psi } ^ { ( i ) }$ from $q ( \ u )$ with a probability $\alpha ( \psi ^ { ( i ) } , \tilde { \psi } ^ { ( \tilde { i } ) } )$ , where i between 1 and $N _ { s i m s }$ we have 

$$
\alpha \left(\psi^ {(i)}, \tilde {\psi} ^ {(i)}\right) = m i n \left(1. 0, \frac {p \left(\tilde {\psi} ^ {(i)} | z _ {k}\right) / q \left(\tilde {\psi} ^ {(i)}\right)}{p \left(\psi^ {(i)} | z _ {k}\right) / q \left(\psi^ {(i)}\right)}\right)
$$

In practice, we simulate a uniform random variable u and accept the simulated point $\tilde { \psi } ^ { ( i ) }$ if $\alpha > u ,$ and reject it (and keep $\psi ^ { ( i ) } )$ otherwise. We keep simulating alternatively the state variable and each parameter by incorporating the observations at each step and wait for the parameters to converge to their ideal mean. 

It is important to note that this joint filtering differs from the usual MCMC techniques, such as in [156] and [92], where we update the particles by incorporating all observations at each simulation step. 

## The Performance of the Inference Tools

We have applied various Gaussian and particle-based filters to daily historic data. None of the methodologies performed very well at that frequency.<sup>26</sup> We now try to analyze the reasons. 

A known weakness of optimization algorithms is the following. The higher the number of parameters, the worse the performance of the algorithm. This means that a one-parameter optimization should perform best. To test this, we simulate 5000 points<sup>27</sup> via the Heston model with a parameter set $\Psi ^ { * }$ as shown in the following (also see Figure 2.33). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/f1cc337b663207b9cb55621c927dd4791593c6dbe5e3e6ec5a01a1fa60409058.jpg)



FIGURE 2.33 Simulated Stock-Price Path via Heston Using $\Psi ^ { * }$ . This is an artificial time series following the Heston model.


We use a drift of $\mu _ { S } = 0 . 0 2 5$ and a time step $\Delta t = 1 / 2 5 2$ as before. In order to get the best performance, we fix all parameters except one. For instance, to obtain $\hat { \omega }$ we fix $\theta = 1 0 . 0 , \xi = 0 . 0 3 , \rho = - 0 . 5 0 , \mu _ { S } = 0 . 0 2 5$ ; we choose a reasonable initial point $\omega _ { 0 }$ and then optimize upon $\omega$ only. We choose an initial parameter set $\Psi _ { 0 }$ as will be shown. The results are displayed in Table 2.4. 


TABLE 2.4 The Optimal Parameter Set $\hat { \Psi } .$ . The estimation is performed individually for each parameter on the artificially generated time series. Particle filters use 1000 simulations.


<table><tr><td>Filter</td><td><eq>\hat{\omega}</eq></td><td><eq>\hat{\theta}</eq></td><td><eq>\hat{\xi}</eq></td><td><eq>\hat{\rho}</eq></td></tr><tr><td>EKF</td><td>0.098212</td><td>10.188843</td><td>0.052324</td><td>-0.873571</td></tr><tr><td>UKF</td><td>0.107281</td><td>10.089381</td><td>0.000001</td><td>+0.598434</td></tr><tr><td>EPF</td><td>0.098287</td><td>10.130531</td><td>0.044437</td><td>-0.827729</td></tr><tr><td>UPF</td><td>0.100581</td><td>10.221816</td><td>0.051902</td><td>-0.487695</td></tr></table>

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/8beae8030ff173a91f13068aee97575c0ed91756e8c07f1176cb960a7ad79791.jpg)



FIGURE 2.34 $f ( \omega ) = L ( \omega , \hat { \theta } , \hat { \xi } , \hat { \rho } )$ Has a Good Slope Around $\hat { \omega } = 0 . 1 0$


It is interesting to note that the estimation of the volatility-drift parameters $( \omega , \theta )$ could be done fairly well via $\mathrm { E K F } . ^ { 2 8 }$ This makes sense because the dependence on these parameters is linear. 

The estimation of volatility and correlation parameters $( \xi , \rho )$ is not as straightforward. This could be seen by plotting the likelihood $L ( \Psi )$ as a function of $\omega , \theta , \xi ,$ and $\rho$ separately. We fix three parameters to their optimal values and plot $L ( \Psi )$ as a function of the last one. We observe in Figures 2.34 through $2 . 3 7$ that the likelihood function is fairly easy to optimize for $( \omega , \theta )$ However, the function is very flat around the optimal $\xi$ and $\rho .$ Therein lies the difficulty of finding the optimums! 

Sample Size It seems therefore that the estimation is inefficient for the parameter $\xi$ no matter which filter we use. The issue is that of inefficiency (large error variance) for this given sample size. This is indeed one of the shortcomings of maximum likelihood estimators (MLE). For a given sample size, they can very well be inefficient and even have a bias.<sup>29</sup> The choice of the filter will not solve this problem. However, under minimal regularity 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/cad079dafac13988e72de97443e33d1932f3f137334bb15d1da31fdac50db5e5.jpg)



FIGURE 2.35 $f ( \theta ) = L ( \hat { \omega } , \theta , \hat { \xi } , \hat { \rho } )$ Has a Good Slope Around $\hat { \theta } = 1 0 . 0$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/2e9e15a522d22ef567fece04ce68295604b2163091102e77f9140134dc69843e.jpg)



FIGURE 2.36 $f ( \xi ) = L ( \hat { \omega } , \hat { \theta } , \xi , \hat { \rho } )$ Is Flat Around $\hat { \xi } = 0 . 0 3$


$\begin{array} { r } { \hat { \nu } _ { N } = \frac { 1 } { N } \sum _ { k = 1 } ^ { N } ( x _ { k } - \hat { \mu } _ { N } ) ^ { 2 } } \end{array}$ . The latter ML estimation is biased, and the correct estimation would be $\begin{array} { r } { \hat { \hat { \nu } } _ { N } = \frac { 1 } { N - 1 } \sum _ { k = 1 } ^ { N } ( x _ { k } - \hat { \mu } _ { N } ) ^ { 2 } } \end{array}$ . However, it is clear that as $N \to + \infty$ we have $\hat { \nu } _ { N } \approx \hat { \hat { \nu } } _ { N }$ and the bias gradually disappears. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/f3f42360ea24d6ef7706477b8c648c7c446bfad08de69be23a5bc3153504c205.jpg)



FIGURE 2.37 $f ( \rho ) = L ( \hat { \omega } , \hat { \theta } , \hat { \xi } , \rho )$ Is Flat and Irregular Around $\hat { \rho } = - 0 . 5 0$


conditions, MLEs are consistent and therefore asymptotically converge to the correct optimum. This means that the sample size is key. To test this, we can choose larger samples of $N = 5 0 , 0 0 0 , N = 1 0 0 , 0 0 0$ , and $N = 5 0 0 , 0 0 0$ points and rerun the simplest filter, namely, the EKF. As expected, the optimum of the likelihood function becomes closer and closer to $\xi ^ { * }$ . This can be seen in Figures 2.38 to 2.41 as well as in Table 2.5. The same exact observations could be made for the correlation parameter $\rho ,$ and the results are also displayed in Table 2.5. The likelihood graphs are omitted in the interest of brevity. 

As for the drift parameters ω and $\theta ,$ the convergence was good even for $N = 5 0 0 0$ , as previously observed. Unfortunately, in reality we have limited historic data. Even at a daily frequency, 50 000 points would correspond to 200 years! 

One possibility would be to use intra-day data; however, that assumes that the behavior of the stock price is the same intra-day (which is reasonable considering we started with a continuous SDE). Moreover, clean intra-day data is usually not readily available and needs preprocessing. Therefore, having $\boldsymbol { p }$ parameters in the optimal parameter set $\hat { \Psi } _ { N } = \left( \hat { \Psi } _ { N } [ j ] \right) _ { 1 \leq j \leq p }$ for a sample size N, we have for each parameter [j] 

$$
\lim _ {N \to + \infty} \hat {\Psi} _ {N} [ j ] \quad | \quad \left\{\Psi [ k ] = \Psi^ {*} [ k ]; 1 \leq k \leq p; k \neq j \right\} = \Psi^ {*} [ j ]\tag{2.28}
$$

What is more, this is true for any valid initial value $\Psi _ { 0 } [ j ]$ , which means the MLE is robust. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/fa57c65436df6c5edd57bca929b09bcb65cbaeeffaebf730789296894b15f14e.jpg)



FIGURE 2.38 $f ( \xi ) = L ( \hat { \omega } , \hat { \theta } , \xi , \hat { \rho } )$ via EKF for N 5000 Points. The true value is $\xi ^ { * } = 0 . 0 3$



TABLE 2.5 The Optimal EKF Parameters $\hat { \xi }$ and $\hat { \boldsymbol \rho }$ Given a Sample Size N. The true parameters are $\xi ^ { * } = 0 . 0 3$ and $\rho ^ { * } = - 0 . 5 0$ . The initial values were $\xi _ { 0 } = 0 . 0 2$ and $\rho _ { 0 } = - 0 . 4 0$


<table><tr><td>N</td><td><eq>\hat{\xi}</eq></td><td><eq>\hat{\rho}</eq></td></tr><tr><td>5000</td><td>0.052324</td><td>-0.873571</td></tr><tr><td>50,000</td><td>0.036463</td><td>-0.608088</td></tr><tr><td>100,000</td><td>0.033400</td><td>-0.556868</td></tr><tr><td>500,000</td><td>0.031922</td><td>-0.532142</td></tr></table>

Joint Estimation of the Parameters Let us now assume that we do not know any of the parameters; we choose an initial set $\Psi _ { 0 }$ and test the consistency of the MLE. We shall apply the EKF to the data and take the same true parameter set $\Psi ^ { * }$ as in the previous section. We assume that $\mu _ { S } = 0 . 0 2 5$ is known; otherwise, it could be estimated together with the model parameters. 

As previously mentioned, the likelihood function becomes flat and therefore harder to maximize under a higher number of parameters. The convergence of the estimator will therefore be slower. Despite this, we can observe in Table 2.8 the asymptotic convergence of the estimator even under the joint estimation of all parameters. We have now 

$$
\lim _ {N \to + \infty} \hat {\Psi} _ {N} = \Psi^ {*}\tag{2.29}
$$

TABLE 2.6 The True Parameter Set $\Psi ^ { * }$ Used for Data Generation 

$$
\Psi^ {*}
$$

$$
\omega^ {*} = 0. 1 0
$$

$$
\theta^ {*} = 1 0. 0
$$

$$
\xi^ {*} = 0. 0 3
$$

$$
\rho^ {*} = - 0. 5 0
$$

TABLE 2.7 The Initial Parameter Set $\Psi _ { 0 }$ Used for the Optimization Process 

$$
\Psi_ {0}
$$

$$
\omega_ {0} = 0. 1 5
$$

$$
\theta_ {0} = 1 5. 0
$$

$$
\xi_ {0} = 0. 0 2
$$

$$
\rho_ {0} = - 0. 4 0
$$


TABLE 2.8 The Optimal EKF Parameter Set $\hat { \Psi }$ Given a Sample Size N. The four parameters are estimated jointly.


<table><tr><td>N</td><td><eq>\hat{\omega}</eq></td><td><eq>\hat{\theta}</eq></td><td><eq>\hat{\xi}</eq></td><td><eq>\hat{\rho}</eq></td></tr><tr><td>5000</td><td>0.150854</td><td>15.294576</td><td>0.266175</td><td>-0.128835</td></tr><tr><td>50,000</td><td>0.126387</td><td>12.748852</td><td>0.020521</td><td>-1.000000</td></tr><tr><td>100,000</td><td>0.136023</td><td>13.700906</td><td>0.044353</td><td>-0.439961</td></tr><tr><td>500,000</td><td>0.100097</td><td>10.030336</td><td>0.061688</td><td>-0.257305</td></tr><tr><td>1,000,000</td><td>0.105264</td><td>10.548642</td><td>0.043818</td><td>-0.356234</td></tr><tr><td>2,000,000</td><td>0.103183</td><td>10.334876</td><td>0.039767</td><td>-0.374677</td></tr><tr><td>4,000,000</td><td>0.105292</td><td>10.538019</td><td>0.043288</td><td>-0.347562</td></tr><tr><td>5,000,000</td><td>0.101097</td><td>10.118951</td><td>0.028588</td><td>-0.514346</td></tr></table>

which corresponds to the generalization of (2.28) in the previous section. 

We ran other filters (UKF, EPF, UPF) on the same data set and observed only marginal improvement. The results are omitted in the interest of brevity. It therefore seems that the fundamental issue is related to the slow convergence of the MLEs regardless of the filtering method. 

A related issue previously mentioned is the size of the observation error $U _ { k } \propto \sqrt { \Delta t } .$ , which is large compared with the observation function $H _ { k } \propto \Delta t$ for daily observations. 

Error Size Revisited As previously mentioned, this underlines the more fundamental problem for the SV estimation: By definition, volatility represents the noise of the stock process. Indeed if we had taken the spot price $S _ { k }$ as the observation and the variance $\nu _ { k }$ as the state, we would have 

$$
S _ {k + 1} = S _ {k} + S _ {k} \mu_ {S} \Delta t + S _ {k} \sqrt {\nu_ {k}} \sqrt {\Delta t} B _ {k}
$$

we would then have an observation function gradient $H = 0$ and the system would be unobservable! It is precisely because we use a Taylor second-order 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/fb016cbd496dc66e4addde2fa7bacbbfd3cd0e8febc0b5cf00ba1eb4a9f95e89.jpg)



FIGURE 2.39 $f ( \xi ) = L ( \hat { \omega } , \hat { \theta } , \xi , \hat { \rho } )$ via EKF for $N = 5 0 , 0 0 0$ Points. The true value is $\xi ^ { * } = 0 . 0 3$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/6948e609a0bb2156afe7027a90b2cc9223c58b60b5a7a5ecb46d410ad6a03bff.jpg)



FIGURE 2.40 $f ( \xi ) = L ( \hat { \omega } , \hat { \theta } , \xi , \hat { \rho } )$ via EKF for $N = 1 0 0 , 0 0 0$ Points. The true value is $\xi ^ { * } = 0 . 0 3$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/0b6d96ed958ebbcbabd3dd8f8f8f5545f0f482e6ba1adb369c4951eb0acd71cc.jpg)



FIGURE 2.41 $f ( \xi ) = L ( \hat { \omega } , \hat { \theta } , \xi , \hat { \rho } )$ via EKF for $N = 5 0 0 , 0 0 0$ Points. The true value is $\xi ^ { * } = 0 . 0 3$


expansion 

$$
\ln (1 + x) \approx x - \frac {1}{2} x ^ {2}
$$

that we obtain access to $\nu _ { k }$ through the observation function. However, in 

$$
\ln \left(\frac {S _ {k + 1}}{S _ {k}}\right) = \left(\mu_ {S} - \frac {1}{2} \nu_ {k}\right) \Delta t + \sqrt {\nu_ {k}} \sqrt {\Delta t} B _ {k}
$$

the error remains dominant as the first order of the expansion.<sup>30</sup> Harvey, Ruiz, and Shephard [130] use the approximation $\Delta t = o ( \sqrt { \Delta t } )$ and take 

$$
z _ {k} = \ln \left(\ln^ {2} \left(\frac {S _ {k + 1}}{S _ {k}}\right)\right) \approx \ln (\nu_ {k}) + \ln (\Delta t) + \ln \left(B _ {k} ^ {2}\right)
$$

Note that under this form EKF would blow up because $\begin{array} { r } { z _ { k } ^ { - } = b ( \nu _ { k } , 0 ) = } \end{array}$ $- \infty$ . They therefore use the fact that E[ln $( B _ { k } ^ { 2 } ) ] = - 1 . 2 7$ and $s t d e \nu [ \ln ( B _ { k } ^ { 2 } ) ] =$ $\pi / { \sqrt { 2 } }$ and consider the Gaussian approximation 


TABLE 2.9 The Optimal EKF Parameter Set $\hat { \Psi }$ via the HRS Approximation Given a Sample Size N. The four parameters are estimated jointly.


<table><tr><td>N</td><td><eq>\hat{\omega}</eq></td><td><eq>\hat{\theta}</eq></td><td><eq>\hat{\xi}</eq></td><td><eq>\hat{\rho}</eq></td></tr><tr><td>5000</td><td>0.722746</td><td>71.753861</td><td>0.044602</td><td>-1.000000</td></tr><tr><td>50,000</td><td>0.234110</td><td>23.575193</td><td>0.028056</td><td>-1.000000</td></tr><tr><td>100,000</td><td>0.150512</td><td>15.186113</td><td>0.017748</td><td>-1.000000</td></tr><tr><td>500,000</td><td>0.109738</td><td>11.020391</td><td>0.027140</td><td>-0.531481</td></tr></table>

$$
\ln \left(B _ {k} ^ {2}\right) \sim - 1. 2 7 + \frac {\pi}{\sqrt {2}} \mathcal {N} (0, 1)
$$

which may or may not be valid. We call this approximation Harvey-Ruiz-Shephard (HRS) and apply it to the same case as in the previous paragraphs. As can be seen in Table 2.9, the approximation seems to be valid for our example. Note that UKF would not have this problem because we would work with the real nonlinear function $z = h ( x , u )$ . However, we would still deal with logs of very small quantities, which could be numerically unstable. 

Another way of tackling the same equation would be via a particle filter, where 

$$
z _ {k} = \ln \left(\left| \ln \left(\frac {S _ {k + 1}}{S _ {k}}\right) \right|\right) \approx \frac {1}{2} \ln (\nu_ {k}) + \frac {1}{2} \ln (\Delta t) + \ln (| B _ {k} |)
$$

and as stated in [10] the density of $\ln ( | B _ { k } | )$ is 

$$
f (x) = 2 e ^ {x} n \left(e ^ {x}\right)
$$

with $n ( )$ the normal density.<sup>31</sup> 

Testing the same data set provides Table 2.10, which does not seem to improve upon the KF. 

It is important to note that even if we took the example of the Heston model, the same issues are true for any stochastic volatility model of type 

$$
\nu_ {k} = \nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \nu_ {k - 1} ^ {p} \sqrt {\Delta t} Z _ {k - 1}
$$

<sup>31</sup>It is easy to see that if X is a standard normal variable, then the CDF of $\ln ( | X | )$ is 

$$
F (x) = P (\ln (| X |) \leq x) = P \left(| X | \leq e ^ {x}\right) = P \left(- e ^ {x} \leq X \leq e ^ {x}\right)
$$

$$
F (x) = N \left(e ^ {x}\right) - N \left(- e ^ {x}\right) = 2 N (e ^ {x}) - 1
$$


TABLE 2.10 The Optimal PF Parameter Set $\hat { \Psi }$ Given a Sample Size N. The four parameters are estimated jointly.


<table><tr><td>N</td><td><eq>\hat{\omega}</eq></td><td><eq>\hat{\theta}</eq></td><td><eq>\hat{\xi}</eq></td><td><eq>\hat{\rho}</eq></td></tr><tr><td>5000</td><td>0.147212</td><td>14.999999</td><td>0.070407</td><td>-0.555263</td></tr></table>

including the GARCH diffusion and the $3 / 2$ models. As previously mentioned, even if the transition equation is different here, the observation equation remains the same. Applying the EKF, we have the transition matrix and noise 

$$
\begin{array}{l} A _ {k} = 1 - \left[ \rho \xi \mu_ {S} \left(p - \frac {1}{2}\right) \nu_ {k - 1} ^ {p - \frac {3}{2}} + \theta - \frac {1}{2} \rho \xi \left(p + \frac {1}{2}\right) \nu_ {k - 1} ^ {p - \frac {1}{2}} \right] \Delta t \\ \qquad + \left(p - \frac {1}{2}\right) \rho \xi \nu_ {k - 1} ^ {p - \frac {3}{2}} \ln \left(\frac {S _ {k}}{S _ {k - 1}}\right) \end{array}
$$

$$
W _ {k} = \xi \sqrt {1 - \rho^ {2}} \nu_ {k - 1} ^ {p} \sqrt {\Delta t}
$$

However, we still have the observation matrix and noise 

$$
H _ {k} = - \frac {1}{2} \Delta t
$$

and 

$$
U _ {k} = \sqrt {\nu_ {k}} \sqrt {\Delta t}
$$

and the same problem of $\Delta t = o \left( \sqrt { \Delta t } \right)$ still exists at observation level for any value of $\boldsymbol { p }$ . 

Another point that should be mentioned is that even if $\xi$ and $\rho$ are separately harder to estimate than $\omega$ and $\theta ,$ the product $\rho \xi$ appears in the equations at the same level. Indeed, as we just saw, in $A _ { k }$ only the product $\rho \xi$ is available. However, at the noise level $\mathbb { W } _ { k } ,$ we can distinguish the two parameters $\rho$ and $\xi .$ For instance, in our previous EKF joint estimation table, we had for 50 000 points $\hat { \xi } \approx 0 . 0 2 0 5 2 1 , \hat { \rho } \approx - 1 . 0 0 0 0$ and again, the individual estimations of $\xi$ and $\rho$ remained far from their true values. However, we have $\hat { \xi } \hat { \rho } \approx - 0 . 0 \dot { 2 } 0 5 2 1$ , which is much closer to $\xi ^ { * } \rho ^ { * } = - 0 . 0 1 5$ . Interestingly, the product $\rho \xi$ is what we need to determine the skewness of the distribution.<sup>32</sup> However, we do need to determine $\xi$ alone to obtain the distribution kurtosis. 

It is also worth noting that in a GARCH framework, we do not have this problem of poor observability for the discrete case. In fact, at each point in time, $\nu _ { k }$ is known exactly as a function of previous observations. Only later, we go to the two-factor diffusion limit, as Nelson [194] does. However, we have to bear in mind that this GARCH diffusion limit is a very special case of the stochastic volatility problem, since it misses the second source of randomness in the discrete case. As Corradi [61] explains, a discrete GARCH model may very well converge toward a one-factor diffusion process without stochastic volatility. Interestingly, when discretizing the one-factor continuous process, we can recover GARCH, whereas when discretizing the two-factor continuous process we will not obtain GARCH but the two-factor discrete process we have been working with. 


TABLE 2.11 Real and Optimal Parameter Sets Obtained via NGARCH MLE. The 5000 points were generated via the one-factor NGARCH with daily parameters.


<table><tr><td></td><td><eq>\omega</eq></td><td><eq>\alpha</eq></td><td><eq>\beta</eq></td><td><eq>c</eq></td></tr><tr><td><eq>\Psi^{*}</eq></td><td>0.00000176</td><td>0.0626</td><td>0.89760</td><td>0.00</td></tr><tr><td><eq>\hat{\Psi}</eq></td><td>0.00000200</td><td>0.0530</td><td>0.89437</td><td>0.05</td></tr></table>

This explains why GARCH MLE (without filtering) can recover parameters used in a simulated time series of length 5000 created via a one-factor GARCH process, whereas it cannot recover the diffusion-limit parameters from a time series created via a two-factor stochastic volatility process as accurately.<sup>33</sup> One can see this in Tables 2.11 and 2.12. 

This also explains why estimating ω and θ alone works so much better with 5000 points. After all, if we had $\xi = 0$ and therefore a deterministic instantaneous variance, we would have no observability problem to talk about. Indeed, $\nu _ { t }$ would be exactly known at each time step, as is the case in a GARCH framework. 


TABLE 2.12 Real and Optimal Parameter Sets Obtained via NGARCH MLE as well as EKF. The 5000 points were generated via the two-factor GARCH diffusion limit with annual parameters.


<table><tr><td></td><td><eq>\omega</eq></td><td><eq>\theta</eq></td><td><eq>\xi \rho</eq></td></tr><tr><td><eq>\Psi^{*}</eq></td><td>0.100000</td><td>10.00</td><td>-0.015</td></tr><tr><td><eq>\hat{\Psi}_{GARCH}</eq></td><td>0.063504</td><td>6.84</td><td>-0.019</td></tr><tr><td><eq>\hat{\Psi}_{EKF}</eq></td><td>0.148000</td><td>14.48</td><td>-0.023</td></tr></table>

Finally, we can now see better why the estimation worked fairly well even with 200 points if $\Delta t = 1$ year—simply because we do not have $\Delta t =$ $o ( \sqrt { \Delta t } )$ and the observability is much more accurate. Nevertheless, with such a large $\Delta t .$ , other problems, such as strong nonlinearity and the nonapplicability of the Grisanov theorem arise. Not to mention the fact that 200 points would correspond to 200 years of data! 

High-Frequency Data Given that the results seem to converge for a large number of data points, one idea would be to use a higher sampling frequency. If instead of using daily data we sample every five seconds, then with a ten-year range we will have $1 0 \times 2 5 2 \times 6 . 5 \times 6 0 \times 6 0 \div 5 = 1 1$  793 600 data points, which is very sufficient for our MLEs. For testing the use of highfrequency data, we can generate via Monte Carlo 5 000 000 points with a $\Delta t = 1 / 2 5 2 , 0 0 0$ , which corresponds to 20 years. We obtain the results in Table 2.13. Both rows have reasonable results. It is, however, notable that the EKF/HRS method seems to perform better than the plain EKF. 

It may seem a little surprising that for the same time period [0 T ] dividing $\Delta t$ by 1000 and multiplying N by 1000 helps us. Why don’t the two operations cancel one another? Observing the negative of log-likelihood function in an EKF framework 


TABLE 2.13 The Optimal Parameter Set $\hat { \Psi }$ for 5 000 000 Data Points. The sampling is performed 1000 times a day and therefore the data set corresponds to 5000 business days. The four parameters are estimated jointly.


<table><tr><td></td><td><eq>\hat{\omega}</eq></td><td><eq>\hat{\theta}</eq></td><td><eq>\hat{\xi}</eq></td><td><eq>\hat{\rho}</eq></td></tr><tr><td>EKF</td><td>0.090280</td><td>9.019962</td><td>0.042984</td><td>-0.283236</td></tr><tr><td>EKF/HRS</td><td>0.092372</td><td>9.224421</td><td>0.030951</td><td>-0.507763</td></tr></table>

$$
\phi (\omega , \theta , \xi , \rho) = \sum_ {k = 1} ^ {N} \left[ \ln (F _ {k}) + \frac {\tilde {z} _ {k} ^ {2}}{F _ {k}} \right]
$$

with 

$$
\tilde {\mathbf {z}} _ {k} = \mathbf {z} _ {k} - \mathbf {h} (\hat {\mathbf {x}} _ {k} ^ {-}, 0)
$$

and 

$$
\mathbf {F} _ {k} = \mathbf {H} _ {k} \mathbf {P} _ {k} ^ {-} \mathbf {H} _ {k} ^ {t} + \mathbf {U} _ {k} \mathbf {U} _ {k} ^ {t}
$$

We can see that considering first-order terms, dividing $\Delta t$ by 1000, or equivalently multiplying it by $\epsilon = 1 / 1 0 0 0$ , will cause the transition matrix $A _ { k }$ to be unchanged, the transition noise $\mathbb { W } _ { k }$ to be multiplied by $\sqrt { \epsilon }$ , the observation matrix $H _ { k }$ to be multiplied by $\epsilon ,$ and the observation noise $U _ { k }$ to be multiplied by $\sqrt { \epsilon }$ . Furthermore, $A _ { k }$ being unchanged will cause $P _ { k } ^ { - }$ and $P _ { k }$ to remain unchanged as well. Therefore, $\tilde { \mathbf { z } } _ { k }$ will be multiplied by $\sqrt { \epsilon } ,$ the term $F _ { k }$ will be multiplied by $\epsilon ,$ and the fraction used in the log-likelihood sum will remain the same. This causes the sum $\phi ( \omega , \theta , \xi , \rho )$ to be higher by a factor $1 / \epsilon ,$ which shows that higher frequency does allow us to obtain a higher likelihood function and therefore better convergence. This is in agreement with what we observed in the above test. 

The Frequency of the Observations Note that the ideal stochastic differential equations are supposed to be continuous; however, we only have discrete observations obtained via an Euler scheme. This introduces a discretization error that may become important as the time interval $\Delta t$ becomes larger. $\mathrm { A } s$ mentioned in [92], [164], and [201], the solution would be to $\it { \hbar } t l l$ the missing data via additional simulations in time: For the observation time step $1 \leq k \leq N$ , the simulation $1 \leq i \leq N _ { s i m s }$ , and the additional time step $1 \leq j \leq M$ , we would have the particles 

$$
\tilde {x} _ {k + \frac {j}{M}} ^ {(i)} = \tilde {x} _ {k + \frac {j - 1}{M}} ^ {(i)} + \left(\omega - \theta \tilde {x} _ {k + \frac {j - 1}{M}} ^ {(i)}\right) \frac {\Delta t}{M} + \xi \sqrt {\tilde {x} _ {k + \frac {j - 1}{M}} ^ {(i)}} \sqrt {\frac {\Delta t}{M}} Z _ {k + \frac {j}{M}} ^ {(i)}
$$

and the observation 

$$
z _ {k + 1} = z _ {k} + \sum_ {j = 1} ^ {M} \left(\mu_ {S} - \frac {1}{2} \tilde {x} _ {k + \frac {j}{M}}\right) \frac {\Delta t}{M} + \sqrt {\sum_ {j = 1} ^ {M} \tilde {x} _ {k + \frac {j}{M}} \frac {\Delta t}{M}} B _ {k}
$$

where each $Z _ { k + \frac { j } { M } } ^ { ( i ) }$ has a correlation $\rho$ with $B _ { k }$ . Naturally, the innovations $Z _ { l }$ are mutually uncorrelated. However, as discussed in [164], the discretization error is small when $\Delta t = 1 / 2 5 2$ , which is the case we are dealing with. 


TABLE 2.14 Mean and (Standard Deviation) for the Estimation of Each Parameter via EKF Over $P = 5 0 0$ Paths of Lengths N 5000 and $N = 5 0 , 0 0 0$ . The true values are $( \omega ^ { * } = 0 . 1 0 , \theta ^ { * } = 1 0 , \xi ^ { * } = 0 . 0 3 , \rho ^ { * } = - 0 . 5 0 )$


<table><tr><td></td><td><eq>\hat{\omega}</eq></td><td><eq>\hat{\theta}</eq></td><td><eq>\hat{\xi}</eq></td><td><eq>\hat{\rho}</eq></td></tr><tr><td>N=5000</td><td>0.11933899(0.098995729)</td><td>11.92271488(9.673829518)</td><td>0.056092146(0.049741887)</td><td>-0.34321724(0.297433861)</td></tr><tr><td>N=50,000</td><td>0.102554592(0.027020734)</td><td>10.26233092(2.706564396)</td><td>0.04383931(0.013004526)</td><td>-0.351998284(0.074998408)</td></tr></table>

Sampling Distribution Even if in practice we deal with one historic path, we should determine the distribution of the optimal parameter set as follows. We simulate $P = 5 0 0$ paths of length $N = 5 0 0 0$ and estimate for each path $j$ the optimal set ${ \hat { \Psi } } ^ { ( j ) }$ . We then can estimate 

$$
\bar {\hat {\Psi}} = \frac {1}{P} \sum_ {j = 0} ^ {P - 1} \hat {\Psi} ^ {(j)}
$$

as well as the variance 

$$
V (\hat {\Psi}) = \frac {1}{P} \sum_ {j = 0} ^ {P - 1} (\hat {\Psi} ^ {(j)} - \bar {\hat {\Psi}}) ^ {2}
$$

In this way we will know how the estimator performs on average and how far we could be from this average. The distribution of the parameter set around its mean is referred to as the sampling distribution [168]. As we can see in Table 2.14, the average-estimated parameter set is closer to the true set than the one-path-estimated set we were considering in the previous section. However, the corresponding standard deviation is quite high and we could very well get poor results as previously seen. 

From Figures 2.42 to 2.45, we can see that for this data length N and this sample size P the parameters $\omega$ and $\theta$ are determined via EKF in a fairly unbiased way. However, the estimator is not efficient and has a large standard deviation. As for $\xi$ and $\rho ,$ we have both bias and inefficiency. This is not surprising given the results of the previous paragraphs. We obtained good results for $( \omega , \theta )$ when estimated alone, and not so good results for $( \xi , \rho )$ . As mentioned, classical filtering theory works well when the parameters affect the drift of the observation and not the noise. This causes a slow convergence problem for all our parameters. But this is doubly true for $( \xi , \rho )$ since they affect the “noise of the noise.” As previously observed, the bias and inefficiency will disappear as $N \to + \infty .$ , as is the case for any MLE estimator. The biases and the standard deviations are smaller for $N = 5 0 , 0 0 0$ than for $N = 5 0 0 0$ as we can see in Table 2.14. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/7980636a94cfb8d718776a7f6e604a2075dad847a472b2daeb28500c519ce1b2.jpg)



FIGURE 2.42 Density for $\hat { \omega }$ Estimated from 500 Paths of Length 5000 via EKF. The true value is $\omega ^ { * } = 0 . 1 0$ . The sampling distribution is fairly unbiased, but is inefficient.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/be4ff4887a89ad3b0a71ca4e082ca7d8b5fca178fd60369573f1c43f5a411a60.jpg)



FIGURE 2.43 Density for $\hat { \theta }$ Estimated from 500 Paths of Length 5000 via EKF. The true value is $\theta ^ { * } = 1 0$ . The sampling distribution is fairly unbiased, but is inefficient.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/c59a065eb70068c2be4857134cc1eed5aa1b986356e740533c32713fa418f84f.jpg)



FIGURE 2.44 Density for $\hat { \xi }$ Estimated from 500 Paths of Length 5000 via EKF. The true value is $\xi ^ { * } = 0 . \dot { 0 } 3$ . The sampling distribution is inefficient and even has a bias.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/f7848af0f0e424887da53254104d01ad355299d9fa302c6cf1989cb0431a7d7b.jpg)



FIGURE 2.45 Density for $\hat { \rho }$ Estimated from 500 Paths of Length 5000 via EKF. The true value is $\rho ^ { * } = - 0 . 5 0$ . The sampling distribution is inefficient and even has a bias.


## The Bayesian Approach

Even if our method of choice is the classical one, it is worth going over the Bayesian philosophy and methodologies, which have some similarities but also some fundamental differences compared with our point of view. The MLE methodology is a classical (frequentist) approach, in which we assume that there is a set of unknown but fixed parameters. Alternatively, in the Bayesian approach the parameters are considered as random variables with a given prior distribution. We then use the observations (the likelihood) to update these distributions and obtain the posterior distributions. 

It would seem that in order to be as objective as possible and to use the observations as much as possible, one should use priors that are noninformative. However, this sometimes creates degeneracy issues and one should choose a different prior for this reason. 

Markov Chain Monte Carlos (MCMC) include the Gibbs sampler as well as the Metropolis-Hastings (MH) algorithm. The theoretical justification is provided by the Hammersley-Clifford theorem and the ergodic averaging theorem. Details can for instance, be found in [34] or [163]. 

Briefly, the Hammersley-Clifford theorem states that having a parameter set , a state x, and an observation z, we can obtain the joint distribution $\scriptstyle \ p ( \Psi , x | z )$ from $p ( \Psi | x , z )$ and $p ( x | \Psi , z )$ , under some mild regularity conditions. Therefore by applying the theorem iteratively, we can break a complicated multidimensional estimation problem into many simple onedimensional problems. Creating a Markov Chain $\Psi ^ { ( i ) }$ via a Monte Carlo process, the ergodic averaging theorem states that the time average of a parameter will converge toward its posterior mean. 

The Gibbs Sampler The Gibbs sampler consists of iterative simulations from the posterior distributions. Having a parameter set 

$$
\Psi = (\Psi_ {j}) _ {1 \leq j \leq J}
$$

a hidden state 

$$
x = (x _ {k}) _ {1 \leq k \leq N}
$$

and an observation set 

$$
z = (z _ {k}) _ {1 \leq k \leq N}
$$

We proceed as follows: Initialize the state vector and the parameter set to $x ^ { ( 0 ) }$ and $\Psi ^ { ( 0 ) }$ , and choose the prior distribution $p ( \psi )$ . For each simulation index i between 1 and $N _ { s i m s }$ , do: 

1. Simulate $x ^ { ( i ) }$ as 

$$
x ^ {(i)} \sim p (x | z, \Psi^ {(i - 1)})
$$

2. Simulate each parameter from its posterior conditional on partially updated parameters: For each j between 1 and J 

$$
\Psi_ {j} ^ {(i)} \sim p (\psi | z, x, \Psi_ {0} ^ {(i)},..., \Psi_ {j - 1} ^ {(i)}, \Psi_ {j + 1} ^ {(i - 1)},..., \Psi_ {J} ^ {(i - 1)})
$$

with 

$$
p (\psi | z, x, \dots) \propto p (z | x, \psi , \dots) p (x | \psi) p (\psi)
$$

3. Go back to Step 1 and stop after i reaches $N _ { s i m s }$ 

4. Calculate the posterior mean for each parameter after allowing a “burn-$\mathrm { i n } "$ period 

$$
\hat {\Psi} _ {j} = \frac {1}{N _ {s i m s} - i _ {0}} \sum_ {i = i _ {0} + 1} ^ {N _ {s i m s}} \Psi_ {j} ^ {(i)}
$$

with, for instance, $i _ { 0 } = N _ { s i m s } / 1 0 .$ 

It is important to note that in some cases, the prior and the posterior distributions are the same and only differ in parameters. In this case the priors are referred to as conjugate priors. 

The justification is available for instance in [55] and can be summed up as follows: Having two random variables (X Y ), we can write 

$$
\mathbf {E} [ X ] = \int x p (x) d x
$$

but 

$$
p (x) = \int p (x | y) p (y) d y = \int p (x | y) \int p (y | \xi) p (\xi) d \xi d y
$$

therefore, we have 

$$
p (x) = \int p (\xi) h (x, \xi) d \xi
$$

with 

$$
h (x, \xi) = \int p (x | y) p (y | \xi) d y
$$

which shows that $p ( x )$ is a stationary solution for the foregoing integral equation, and $h ( x , \xi )$ corresponds to the limit transition density. 

Similarly, it is possible to show that for a sequence $( x _ { k } )$ generated from a Gibbs Sampler, we have 

$$
P \left(x _ {k} | x _ {0}\right) = \int P \left(x _ {k - 1} | x _ {0}\right) P \left(x _ {k}, x _ {k - 1}\right) d x _ {k - 1}
$$

It is therefore possible to see that as $k  + \infty$ we have 

$$
P (x _ {k} | x _ {0}) \rightarrow p (x _ {k})
$$

and 

$$
P \left(x _ {k} | x _ {k - 1}\right)\rightarrow b (x _ {k}, x _ {k - 1})
$$

which are the stationary marginal and transition densities. 

A Simple Illustration For a simple illustration, consider a sequence of normally distributed data points z with an unknown mean $\mu$ and an unknown variance $1 / \lambda .$ . The parameter λ is often referred to as the precision of the distribution. One possible way to proceed is to choose uniform (noninformative) priors $p ( \mu )$ and $p ( \lambda ) \propto 1 / \lambda$ and use the known results [34] 

$$
p (\mu | z, \sigma) = N (\bar {Z}, \sigma)
$$

with $N ( m , s )$ the normal distribution with mean m and standard deviation s and 

$$
\bar {Z} = \frac {1}{N} \sum_ {k = 1} ^ {N} z _ {k}
$$

as well as 

$$
p (\lambda | z, \mu) = G \left(\frac {N}{2}, \frac {S}{2}\right)
$$

with $G ( a , A )$ the previously described gamma distribution<sup>34</sup> and 

$$
S = \sum_ {k = 1} ^ {N} (z _ {k} - \mu) ^ {2}
$$

and again 

$$
\sigma = 1 / \sqrt {\lambda}
$$

We therefore know both posterior distributions and can simulate from them iteratively and perform Gibbs sampling as described above. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/22c25139690e4d1e6955d7172822d30fe68b65429fde885d1ab1271d0b1d3528.jpg)



FIGURE 2.46 Gibbs Sampler for $\mu$ in $N ( \mu , \sigma )$ . The true value is $\mu ^ { * } = 1 0 . 0 $


For testing this, we generated a time series of 1000 Gaussian points with a mean of $\mu ^ { * } = 1 0$ and a standard deviation of $\sigma ^ { * } = 5$ . We applied the Gibbs sampler via $N _ { s i m s } = 1 0$  000 simulations and considered the average between the $\bar { 1 } 0 0 0 ^ { t h }$ and $1 0 , 0 0 0 ^ { t b }$ simulations. We chose initial values $\mu _ { 0 } = 7 . 0$ and $\sigma _ { 0 } = 3 . 0$ and obtained 

$$
\hat {\mu} = 9. 9 4 3 4 1 6
$$

$$
\hat {\sigma} = 4. 8 1 6 3 0 0
$$

We ploted the simulations from the posteriors in Figures 2.46 and 2.47. 

The Metropolis-Hastings Algorithm The Gibbs sampler is fast and simple when the posterior distributions are known and easy to sample from. However, in practice, and in particular for our stochastic volatility problem, this often is not the case. We assume for simplicity that we do know the posteriors for the parameters and therefore can use the Gibbs sampler for them; however, we cannot do the same for the latent state. 

In this case, the Metropolis-Hastings (MH) algorithm approach can be used for $_ x$ as follows: Initialize the state vector and the parameter set to $x ^ { ( 0 ) }$ and $\Psi ^ { ( 0 ) }$ and choose the prior distribution $p ( \psi )$ . Also choose a proposal distribution $q ( x | z , \Psi )$ for the state. For each simulation index between 1 and $N _ { s i m s }$ do: 

1-a. Simulate from the proposal distribution 

$$
x ^ {(i)} \sim q (x | z, \Psi)
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/65cee06e7997f84c7bd1179e880c99355ca0e079eb6c7b96ef621cfa9d61e957.jpg)



FIGURE 2.47 Gibbs Sampler for σ in $N ( \mu , \sigma )$ . The true value is $\sigma ^ { * } = 5 . 0$


1-b. Compare with a randomly generated uniform random variable u the ratio 

$$
\alpha = \min \left(1, \frac {p (x ^ {(i)} | z , \Psi) / q (x ^ {(i)} | z , \Psi)}{p (x ^ {(i - 1)} | z , \Psi) / q (x ^ {(i - 1)} | z , \Psi)}\right)
$$

and accept $x ^ { ( i ) }$ if $\alpha > u ;$ otherwise, reject it and set $x ^ { ( i ) } = x ^ { ( i - 1 ) }$ 

2. Simulate $\Psi ^ { ( i ) }$ via a Gibbs sampler. 

3. Go back to Step 1-a and continue until i reaches $N _ { s i m s }$ 

4. Calculate the posterior mean for each parameter after allowing a “burn-in” period 

$$
\hat {\Psi} _ {j} = \frac {1}{N _ {s i m s} - i _ {0}} \sum_ {i = i _ {0} + 1} ^ {N _ {s i m s}} \Psi_ {j} ^ {(i)}
$$

with, for instance, $i _ { 0 } = N _ { s i m s } / 1 0$ 

Two special cases are worth being mentioned. 

■ First, if we simulate from the posterior, the MH ratio becomes 1.0 and every simulation will be accepted. This is therefore a Gibbs sampler. 

■ Second, if we simulate from the prior, the MH ratio becomes the likelihood ratio, which makes the computation simpler. We shall use this second case extensively in our stochastic volatility inferences. 

The justification for the MH algorithm is available, for instance, in [58] $\mathrm { o r } \left[ 1 2 0 \right]$ . The idea is to find the transition probability from x to y $P \left( x , y \right)$ such that for a given target density π we would have the invariant distribution property 

$$
\pi (d y) = \int P (x, d y) \pi (x) d x
$$

It is possible to express the transition probability $P ( x , d y )$ as 

$$
P (x, d y) = p (x, y) d y + \left(1 - \int p (x, z) d z\right) \delta_ {x} (d y)
$$

with $\delta _ { x } ( )$ the Dirac function. The first term corresponds to the passage probability from x to a point in $d y$ and the second term to the probability of staying at x. 

Now, if the function $p ( x , y )$ satisfies the reversibility condition 

$$
\pi (x) p (x, y) = \pi (y) p (y, x)
$$

then we can see that $\pi ( )$ is the invariant distribution as described previously. Indeed then calling the rejection probability 

$$
r (x) = 1 - \int p (x, z) d z
$$

we have 

$$
\begin{array}{l} \int P (x, A) \pi (x) d x = \int \left[ \int_ {A} p (x, y) d y + r (x) \delta_ {x} (A) \right] \pi (x) d x \\ \qquad = \int_ {A} \left[ \int p (x, y) \pi (x) d x \right] d y + \int_ {A} r (x) \pi (x) d x \\ \qquad = \int_ {A} \left[ \int p (y, x) \pi (y) d x \right] d y + \int_ {A} r (x) \pi (x) d x \\ \qquad = \int_ {A} (1 - r (y)) \pi (y) d y + \int_ {A} r (x) \pi (x) d x \\ \qquad = \int_ {A} \pi (y) d y \end{array}
$$

which proves that $\pi ( x )$ is the invariant distribution for the transition probability $P ( x , y )$ 

However, in practice, the reversibility condition is hardly ever satisfied, and therefore we need to construct an MH density that would indeed be reversible. Taking any proposal density $q ( x , y )$ , we would simply write 

$$
p _ {M H} (x, y) = q (x, y) \min \left(1, \frac {\pi (y) / q (x , y)}{\pi (x) / q (y , x)}\right)
$$

Then $\phi _ { M H } ( x , y )$ would be reversible and hence admit $\pi ( x )$ as its invariant distribution. 

Proof: To see why, let us consider the case where $\frac { \pi ( y ) / q ( x , y ) } { \pi ( x ) / q ( y , x ) } > 1$ , which means its inverse is smaller than 1. We would then have 

$$
p _ {M H} (x, y) \pi (x) = q (x, y) \pi (x) = q (y, x) \frac {\pi (x) / q (y , x)}{\pi (y) / q (x , y)} \pi (y) = p _ {M H} (y, x) \pi (y)
$$

(QED) 

One more point we need to explain is the “blocking” technique. Having two random variables $X _ { 1 } , X _ { 2 }$ , the product of the conditional transition densities, admits the joint distribution $\pi ( X 1 , X 2 )$ for invariant distribution. This is why we can alternate between parameters and hidden states. 

Thus 

$$
\begin{array}{l} \int \int P _ {1} (x _ {1}, d y _ {1} | x _ {2}) P _ {2} (x _ {2}, d y _ {2} | y _ {1}) \pi (x _ {1}, x _ {2}) d x _ {1} d x _ {2} \\ = \int P _ {2} (x _ {2}, d y _ {2} | y _ {1}) \left[ \int P _ {1} (x _ {1}, d y _ {1} | x _ {2}) \pi_ {1 | 2} (x _ {1} | x _ {2}) d x _ {1} \right] \pi_ {2} (x _ {2}) d x _ {2} \\ = \int P _ {2} (x _ {2}, d y _ {2} | y _ {1}) \pi_ {1 | 2} (d y _ {1} | x _ {2}) \pi_ {2} (x _ {2}) d x _ {2} \\ = \int P _ {2} (x _ {2}, d y _ {2} | y _ {1}) \pi_ {2 | 1} (x _ {2} | y _ {1}) \pi_ {1} (d y _ {1}) d x _ {2} \\ = \pi_ {1} (d y _ {1}) \int P _ {2} (x _ {2}, d y _ {2} | y _ {1}) \pi_ {2 | 1} (x _ {2} | y _ {1}) d x _ {2} \\ = \pi_ {1} (d y _ {1}) \pi_ {2 | 1} (d y _ {2} | y _ {1}) = \pi (d y _ {1}, d y _ {2}) \end{array}
$$

which proves that $\pi ( x _ { 1 } , x _ { 2 } )$ is the invariant distribution for this product transition probability. 

Illustration We use the same example as for the Gibbs sampler, only this time we simulate from the priors and use the likelihood ratio to accept or reject the simulations. We choose the priors 

$$
\mu \sim N (7. 0, 3. 0)
$$

and 

$$
\sigma \sim \frac {1}{\sqrt {G (1 / 9 . 0 , 1 . 0)}}
$$

We obtain after $M = 1 0 , 0 0 0$ simulations 

$$
\hat {\mu} = 9. 9 8 9 5 0 4
$$


MH Sampler for the Normal Mean


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/f39ebd4ec489f60e7862894bc25dd50c99c47aed25c526d6bdd17c2de8c5b1f9.jpg)



FIGURE 2.48 Metropolis-Hastings Algorithm for $\mu$ in $N ( \mu , \sigma )$ . The true value is $\mu ^ { * } = 1 0 . 0 .$


and 

$$
\hat {\sigma} = 4. 7 9 7 1 0 5
$$

Naturally, the evaluation of the Markov Chain is different from that of the Gibbs sampler. This can be seen in Figures 2.48 and 2.49. 

A Few Distributions Here are a few distributions commonly used in MCMC algorithms. 

The student cumulative distribution function 

$$
F (x, \nu) = 1 - I \left(\frac {\nu}{\nu + x ^ {2}}, \frac {\nu}{2}, \frac {1}{2}\right)
$$

with $I ( x , a , b )$ the incomplete beta function (IBF) 

$$
I (x, a, b) = \frac {B (x , a , b)}{B (1 , a , b)}
$$

where 

$$
B (x, a, b) = \int_ {0} ^ {x} t ^ {a - 1} (1 - t) ^ {b - 1} d t
$$

with $a , b$ two strictly positive parameters. A few plots of the IBF are provided in Figure 2.50. 


MH Sampler for the Normal Standard Deviation


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/e54cadbc97b928a07a79c1136285515edb2a502f16630d1902ced8c0b0d01a94.jpg)



FIGURE 2.49 Metropolis-Hastings Algorithm for $\sigma$ in $N ( \mu , \sigma )$ . The true value is $\sigma ^ { * } = 5 . 0 .$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/8cb57109bf53717bd694d514ee53a13509689e79cb29e5a6ab592326c98228b2.jpg)



FIGURE 2.50 Plots of the Incomplete Beta Function. Implementation is based on code from Numerical Recipes in C.


The inverse-gamma (IG) cumulative distribution function $I G ( a , x )$ could be defined from that of the previously defined gamma distribution $P \left( a , x \right)$ 

$$
P (a, x) = \frac {1}{\Gamma (a)} \int_ {0} ^ {x} e ^ {- t} t ^ {a - 1} d t
$$

By definition, if the random variable X is gamma-distributed, $Y = 1 / X$ will be IG-distributed and therefore 

$$
I G (a, x) = P (Y \leq x) = P \left(X \geq \frac {1}{x}\right) = 1 - P \left(a, \frac {1}{x}\right)
$$

As for the densities, they are related by 

$$
f _ {I G} (a, x) = \frac {1}{x ^ {2}} f _ {G} \left(a, \frac {1}{x}\right)
$$

Regression Analysis We have the following useful results as described in [34] and [163] using some of the previous distributions. Considering a univariate regression 

$$
Y = \beta X + \epsilon
$$

where 

$$
\epsilon \sim \mathcal {N} (0, \sigma^ {2})
$$

We suppose we know the priors 

$$
p (\beta) = N (a, A)
$$

where a corresponds to the mean and A to the variance. 

$$
p \left(\sigma^ {2}\right) = I G (b, B)
$$

with the density 

$$
f _ {I G} (x, b, B) = \frac {B ^ {b} e ^ {- \frac {B}{x}}}{\Gamma (b) x ^ {b + 1}}
$$

Then we have for the $\beta$ posterior: 

$$
p (\beta | Y, X, \sigma^ {2}) \propto p (Y | X, \beta , \sigma^ {2}) p (\beta) \propto N (a ^ {*}, A ^ {*})
$$

with 

$$
a ^ {*} = \left(\frac {1}{A} + \frac {1}{2} X ^ {t} X\right) ^ {- 1} \left(\frac {a}{A} + \frac {X ^ {t} Y}{\sigma^ {2}}\right)
$$

$$
A ^ {*} = \left(\frac {1}{A} + \frac {X ^ {t} X}{\sigma^ {2}}\right) ^ {- 1}
$$

As for the $\sigma ^ { 2 }$ posterior we have 

$$
p (\sigma^ {2} | Y, X, \beta) \propto p (Y | X, \beta , \sigma^ {2}) p (\sigma^ {2}) \propto I G (b ^ {*}, B ^ {*})
$$

with 

$$
b ^ {*} = T + b
$$

and 

$$
B ^ {*} = (Y - \beta X) ^ {t} (Y - \beta X) + B
$$

Application to Gaussian SV Models (Heston) Various MCMC approaches have been suggested for the SV problem. Jacquier, Polson, and Rossi [156] were first to a apply a hybrid of the Gibbs sampler and the MH algorithm to a log-SV model. Kim, Shephard, and Chib [169] used a slightly different approach for the same model. 

Here, we describe the method employed by Forbes, Martin, and Wright (FMW) [103]. Using their notations 

$$
d \nu_ {t} = \kappa (\theta - \nu_ {t}) d t + \sigma_ {\nu} \sqrt {\nu_ {t}} d Z _ {t}
$$

Obviously our $( \omega , \theta , \xi , \rho )$ could easily be obtained as $( \kappa \theta , \kappa , \sigma _ { \nu } , \rho )$ . The algorithm becomes as follows. 

Initialize $\nu ^ { ( 0 ) } = ( \nu _ { k } ^ { ( 0 ) } ) _ { 1 \leq k \leq N }$ and choose constant and therefore non informative priors for the parameter $\mathsf { s e t } ^ { 3 5 }$ 

$$
\Psi = (\kappa , \theta , \sigma_ {\nu}, \rho)
$$

1. We simulate the state $\nu _ { t }$ from the Heston prior; we have for any time step $k$ between 1 and N and simulation i 

$$
\nu_ {k} ^ {(i)} = \nu_ {k - 1} ^ {(i)} + \kappa (\theta - \nu_ {k - 1} ^ {(i)}) \Delta t + \sigma_ {\nu} \sqrt {\nu_ {k - 1} ^ {(i)} \Delta t} Z _ {k - 1}
$$

As previously mentioned, the MH ratio is therefore the likelihood ratio: 

$$
\alpha = \min \left(1. 0, \frac {p (\ln S | \nu^ {(i)} , \Psi)}{p (\ln S | \nu^ {(i - 1)} , \Psi)}\right)
$$

where 

$$
p (\ln S | \nu , \Psi) \propto \prod_ {k = 1} ^ {N} \frac {1}{\sqrt {(1 - \rho^ {2}) \Delta t \nu_ {k - 1}}} \exp \left\{- \frac {1}{2 (1 - \rho^ {2}) \nu_ {k - 1} \Delta t} (\ln S _ {k} - \mu_ {k}) ^ {2} \right\}
$$

with 

$$
\mu_ {k} = \ln S _ {k - 1} + \left(\mu_ {S} - \frac {1}{2} \nu_ {k - 1}\right) \Delta t + \frac {\rho}{\sigma_ {\nu}} (\nu_ {k} - [ \theta \kappa \Delta t + (1 - \kappa \Delta t) \nu_ {k - 1} ])
$$

Any negative variance would be rejected in the MH step. 

2. The Heston equation 

$$
\nu_ {k} = \nu_ {k - 1} + \kappa (\theta - \nu_ {k - 1}) \Delta t + \sigma_ {\nu} \sqrt {\nu_ {k - 1} \Delta t} Z _ {k - 1}
$$

could be rewritten 

$$
\frac {\nu_ {k} - (1 - \kappa \Delta t) \nu_ {t - 1}}{\sqrt {\nu_ {t - 1} \Delta t}} = \theta \frac {\kappa \Delta t}{\sqrt {\nu_ {t - 1} \Delta t}} + \sigma_ {v} Z _ {k - 1}
$$

which is a linear regression 

$$
y _ {k} = \theta x _ {k} + e _ {k}
$$

with 

$$
y _ {k} = \frac {\nu_ {k} - (1 - \kappa \Delta t) \nu_ {t - 1}}{\sqrt {\nu_ {t - 1} \Delta t}}
$$

$$
x _ {k} = \frac {\kappa \Delta t}{\sqrt {\nu_ {t - 1} \Delta t}}
$$

and 

$$
e _ {k} \sim N (0, \sigma_ {\nu})
$$

Hence, taking constant priors, we have 

$$
\theta | \kappa , \sigma_ {\nu}, \nu \sim N (\bar {\theta}, \sigma_ {\theta})
$$

with 

$$
\bar {\theta} = \frac {\sum_ {k = 1} ^ {N} x _ {k} y _ {k}}{\sum_ {k = 1} ^ {N} x _ {k} ^ {2}}
$$

and 

$$
\sigma_ {\theta} = \sigma_ {\nu} / \sqrt {\sum_ {k = 1} ^ {N} x _ {k} ^ {2}}
$$

What is more 

$$
\sigma_ {\nu} ^ {2} | \kappa , \nu \sim I G (N - 1, s _ {\nu} ^ {2})
$$

with 

$$
s _ {\nu} ^ {2} = \sum_ {k = 1} ^ {N} (y _ {k} - \bar {\theta} x _ {k}) ^ {2}
$$

It is also possible to show that 

$$
p (\kappa | \nu) \propto S t (\bar {\kappa}, \sigma_ {\mathcal {K}}) \left(\sum_ {k = 1} ^ {N} x _ {k} ^ {2}\right) ^ {- \frac {1}{2}}
$$

where $S t ( m , s )$ corresponds to Student’s law of mean m and standard deviation s. The expressions for these mean and standard deviations could be found in [103]. 

We can therefore simulate from the priors, except we have an adjustment factor $\left( \sum _ { k = 1 } ^ { N } x _ { k } ^ { 2 } \right) ^ { - \frac { 1 } { 2 } }$ to multiply the prior by. The MH ratio will therefore be 

$$
\alpha = m i n \left(1. 0, \frac {p (\ln S | \nu , \kappa^ {(i)} , \theta^ {(i)} , \sigma_ {\nu} ^ {(i)} , \rho) \bigl (\sum_ {k = 1} ^ {N} \bigl (x _ {k} ^ {(i)} \bigr) ^ {2} \bigr) ^ {- \frac {1}{2}}}{p (\ln S | \nu , \kappa^ {(i - 1)} , \theta^ {(i - 1)} , \sigma_ {\nu} ^ {(i - 1)} , \rho) \bigl (\sum_ {k = 1} ^ {N} \bigl (x _ {k} ^ {(i - 1)} \bigr) ^ {2} \bigr) ^ {- \frac {1}{2}}}\right)
$$

3. As for the correlation paramater $\rho ,$ we choose a normal proposal distribution and use a constant prior again. Therefore 

$$
\alpha = \min \left(1. 0, \frac {p (\ln S | \nu , \kappa , \theta , \sigma_ {\nu} , \rho^ {(i)}) / q (\rho^ {(i)} | \nu , \kappa , \theta , \sigma_ {\nu} , S)}{p (\ln S | \nu , \kappa , \theta , \sigma_ {\nu} , \rho^ {(i - 1)}) / q (\rho^ {(i)} | \nu , \kappa , \theta , \sigma_ {\nu} , S)}\right)
$$

with $q ( \ u )$ the normal distribution with mean 

$$
\frac {\sum_ {k = 1} ^ {N} x _ {k} y _ {k}}{\sum_ {k = 1} ^ {N} x _ {k} ^ {2}}
$$

and variance 

$$
\frac {\Delta t}{\sum_ {k = 1} ^ {N} x _ {k} ^ {2}}
$$

with 

$$
\begin{array}{l} x _ {k} = \frac {\nu_ {k} - \kappa \theta \Delta t - (1 - \kappa \Delta t) \nu_ {k - 1}}{\sigma_ {\nu} \sqrt {\nu_ {k - 1}}} \\ y _ {k} = \frac {\ln S _ {k} - \ln S _ {k - 1} - (\mu_ {S} - \frac {1}{2} \nu_ {k - 1}) \Delta t}{\nu_ {k - 1}} \end{array}
$$

Note that for any of the foregoing parameters if we simulate one that does not satisfy the usual constraints $\theta \geq 0 , \kappa \geq 0 , \sigma _ { \nu } \geq 0 , \sigma _ { \nu } \leq 2 \kappa \theta .$ , and $- 1 \leq \rho \leq 1$ , then we simply do not accept them during the MH accept/reject step. Also note that we update $( \kappa , \theta , \sigma _ { \nu } )$ in a “block” instead of updating them one by one. This technique is used by many since it makes the algorithm faster. 

For the actual results, the reader could refer to Forbes et al. [103]. The authors test their Bayesian estimator against simulated data, and observe inefficiency. This is in agreement with our observations when applying MLE techniques to simulated data. 

## Using the Characteristic Function

In a recent article [31], the use of the characteristic function has been suggested for the purpose of filtering. In this approach, however, we have to limit ourselves to the case where $F ( U , V , x _ { t } ) = \mathbf { E } [ \exp ( U z _ { t + 1 } + V x _ { t + 1 } ) | x _ { t } ]$ has a known form. One natural form would be the affine process, where 

$$
F (U, V, x _ {t}) = \mathbf {E} [ \exp (U z _ {t + 1} + V x _ {t + 1}) | x _ {t} ] = \exp \{C (U, V) + D (U, V) x _ {t} \}
$$

After choosing the initial conditions, the time update equation 

$$
p (z _ {t + 1}, x _ {t + 1} | t) = \int p (z _ {t + 1}, x _ {t + 1} | x _ {t}) p (x _ {t} | t) d x _ {t}
$$

becomes in terms of the characteristic function 

$$
\begin{array}{r l} & F _ {z x | t} (U, V) = \mathbf {E} _ {t} [ \mathbf {E} (\exp (U z _ {t + 1} + V x _ {t + 1}) | x _ {t}) ] \\ & \qquad = \mathbf {E} [ \exp \{C (U, V) + D (U, V) x _ {t} \} | z _ {1: t} ] \\ & \qquad = \exp [ C (U, V) ] G _ {t | t} [ D (U, V) ] \end{array}
$$

where $G _ { t | s } ( U ) = \mathbf { E } [ \exp ( U x _ { t } ) | z _ { 1 : s } ]$ is the moment-generating function of $x _ { t }$ conditional on the observations up to time s. 

The Measurement Update equation 

$$
p (x _ {t + 1} | t + 1) = \frac {p (z _ {t + 1} , x _ {t + 1} | t)}{p (z _ {t + 1} | t)}
$$

becomes in terms of the characteristic function 

$$
G _ {t + 1 | t + 1} (V) = \frac {\int_ {- \infty} ^ {+ \infty} F _ {z x | t} (i U , V) \exp (- i U z _ {t + 1}) d U}{\int_ {- \infty} ^ {+ \infty} F _ {z x | t} (i U , 0) \exp (- i U z _ {t + 1}) d U}
$$

This remarkably gives us a one-step induction expression 

$$
G _ {t + 1 | t + 1} (V) = \frac {\int_ {- \infty} ^ {+ \infty} \exp [ C (i U , V) - i U z _ {t + 1} ] G _ {t | t} [ D (i U , V) ] d U}{\int_ {- \infty} ^ {+ \infty} \exp [ C (i U , 0) - i U z _ {t + 1} ] G _ {t | t} [ D (i U , 0) ] d U}
$$

which allows us to determine the a posteriori estimate and errors 

$$
\hat {x} _ {t} = G _ {t | t} ^ {\prime} (0)
$$

and 

$$
P _ {t} = V a r _ {t} (x _ {t}) = G _ {t | t} ^ {\prime \prime} (0) - \left(G _ {t | t} ^ {\prime} (0)\right) ^ {2}
$$

at each iteration. 

In this framework, the likelihood function could be written as 

$$
L _ {1: T} = \prod_ {t = 0} ^ {T - 1} l _ {t}
$$

with 

$$
l _ {t} = \frac {1}{2 \pi} \int_ {- \infty} ^ {+ \infty} \exp [ C (i U, 0) - i U z _ {t + 1} ] G _ {t | t} [ D (i U, 0) ] d U
$$

which is equivalent to 

$$
l _ {t} = \frac {1}{\pi} \int_ {0} ^ {+ \infty} \mathcal {R} \left\{\exp [ C (i U, 0) - i U z _ {t + 1} ] G _ {t | t} [ D (i U, 0) ] \right\} d U\tag{2.30}
$$

where corresponds to the real part of a complex number. In order to be able to calculate the integral, we need to know the value of $G _ { t \mid t } ( x )$ at each point. For this, Bates [31] suggests making an assumption on the distribution of the hidden state. For a gamma distribution, we have a moment-generating function of the form 

$$
G _ {t | t} (x) = (1 - \kappa x) ^ {- \nu_ {t}}
$$

The integral (2.30) can be evaluated numerically; however, when dealing with “outliers” the density of the observation takes near-zero values, which makes the integration difficult. Bates suggests scaling transformations equivalent to the importance sampling technique used in particle filtering. 

Independently from this, Dragulescu and Yakovenko, [81] and [219], derived a semianalytic expression for the likelihood under the Heston model, by using Fourier inversion. Note that a particle filter calculates this very integral via Monte Carlo simulations. 

It is worth noting that the main advantage of our particle filtering approach is its complete generality. Indeed the Bates method would work only for model classes that have an exponentially affine Fourier transform. It is true that the Heston model falls in this category; however, a VGG (variance gamma with gamma-distributed arrival rate) process would not, and therefore could only be analyzed through a simulation-based methodology. 

## Introducing Jumps

The Model As in Bates [28], let us introduce a jump process (independent from Brownian motion) with a given intensity λ and a fixed<sup>36</sup> fractional jump size $0 \leq j < 1$ . The number of jumps between t and $t + d t$ will therefore be $d N _ { t }$ . Needless to say, if either the intensity $\lambda = 0$ or the jump size $j = 0$ then we are back to the pure diffusion case. 

The new stochastic differential equation for the stock price in the riskneutral framework will be 

$$
d S _ {t} = (\mu_ {S} + \lambda j) S _ {t} d t + \sqrt {\nu_ {t}} S _ {t} d B _ {t} - S _ {t} j d N _ {t}
$$

and applying Ito’s lemma for semi-Martingales 

$$
d \ln S _ {t} = \left(\mu_ {S} - \frac {1}{2} \nu_ {t} + \lambda j\right) d t + \sqrt {\nu_ {t}} d B _ {t} + \ln (1 - j) d N _ {t}
$$

which we can rewrite in the discrete version as 

$$
\ln S _ {k + 1} = \ln S _ {k} + \left(\mu_ {S} - \frac {1}{2} \nu_ {k} + \lambda j\right) \Delta t + \sqrt {\nu_ {t}} \sqrt {\Delta t} B _ {k} + \mu_ {k}
$$

with $\mu _ { 0 } = 0$ and 

$$
\mu_ {k} = \delta_ {0} (0) e ^ {- \lambda \Delta t} + \delta_ {0} (\ln (1 - j)) (1 - e ^ {- \lambda \Delta t})
$$

where $\delta _ { 0 } ( )$ corresponds to the Dirac delta function.<sup>37</sup> Also 

$$
\begin{array}{l} \nu_ {k} = \nu_ {k - 1} + (\omega - \theta \nu_ {k - 1}) \Delta t + \xi \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} Z _ {k - 1} \\ \qquad - \rho \xi \bigg [ \ln S _ {k - 1} + \bigg (\mu_ {S} + \lambda j - \frac {1}{2} \nu_ {k - 1} \bigg) \Delta t + \sqrt {\nu_ {k - 1}} \sqrt {\Delta t} B _ {k - 1} + \mu_ {k - 1} - \ln S _ {k} \bigg ] \end{array}
$$

which completes our set of equations. 

It is important to note that the new parameter set is 

$$
\Psi = (\omega , \theta , \xi , \rho , \lambda , j)
$$

which effectively gives us two additional degrees of freedom.<sup>38</sup> 

The Generic Particle Filter Since $\mu _ { k }$ is following a Poisson process, we have to use a non-Gaussian filter. The use of a generic particle filter (GPF) is therefore natural. In a generic particle filter, the proposal distribution $q ( x _ { k } )$ is simply set equal to $ { p } ( x _ { k } | x _ { k - 1 } )$ . The state $x _ { k }$ could be chosen as 

$$
x _ {k} = \left( \begin{array}{l} \mu_ {k} \\ \nu_ {k} \end{array} \right)
$$

and the transition equation becomes 

$$
x _ {k} = \binom{\delta_ {0} (0) e ^ {- \lambda \Delta t} + \delta_ {0} (\ln (1 - j)) (1 - e ^ {- \lambda \Delta t})}{v _ {k - 1} + [ (\omega - \rho \xi (\mu_ {S} + \lambda j) - (\theta - \frac {1}{2} \rho \xi) v _ {k - 1} ] \Delta t + \rho \xi [ \ln (\frac {S _ {k}}{S _ {k - 1}}) - \mu_ {k - 1} ] + \xi \sqrt {1 - \rho^ {2}} \sqrt {v _ {k - 1}} \sqrt {\Delta t} \tilde {Z} _ {k - 1}}
$$

It becomes therefore possible to implement a particle filter as follows. 

1. Choose $\nu _ { 0 }$ and $P _ { 0 } > 0$ and set $\mu _ { 0 } = 0$ , so for i in $1 , . . . , N _ { s i m s }$ 

$$
x _ {0} ^ {(i)} = \binom{0}{\nu_ {0} + \sqrt {P _ {0}} Z ^ {(i)}}
$$

Then for each k with $1 \leq k \leq N$ do 

2. Write the new $\tilde { x } _ { k } ^ { ( i ) } = ( \tilde { \mu } _ { k } ^ { ( i ) } , \tilde { \nu } _ { k } ^ { ( i ) } ) ^ { t }$ as the result of simulations 

$$
\begin{array}{c} \tilde {v} _ {k} ^ {(i)} \sim \mathcal {N} \bigg (\mathbf {m} = v _ {k - 1} ^ {(i)} + \bigg [ \omega - \rho \xi (\mu_ {S} + \lambda j) - \bigg (\theta - \frac {1}{2} \rho \xi \bigg) v _ {k - 1} ^ {(i)} \bigg ] \\ \times \Delta t + \rho \xi \bigg [ \ln \left(\frac {S _ {k}}{S _ {k - 1}}\right) - \mu_ {k - 1} ^ {(i)} \bigg ], \mathbf {s} \bigg) \end{array}
$$

with $\mathbf { s } = \xi \sqrt { 1 - \rho ^ { 2 } } \sqrt { \nu _ { k - 1 } ^ { ( i ) } } \sqrt { \Delta t }$ and 

$$
\tilde {\mu} _ {k} ^ {(i)} = 0
$$

if $\mathcal { U } [ 0 , 1 ] \leq e ^ { - \lambda \Delta t }$ and 

$$
\tilde {\mu} _ {k} ^ {(i)} = \ln (1 - j)
$$

otherwise. 

3. Define the weights 

$$
w _ {k} ^ {(i)} = w _ {k - 1} ^ {(i)} p (z _ {k} | \tilde {x} _ {k} ^ {(i)})
$$

with 

$$
p (z _ {k} | \tilde {x} _ {k} ^ {(i)}) = n \left(z _ {k}, z _ {k - 1} + \left(\mu_ {S} + \lambda j - \frac {1}{2} \tilde {v} _ {k} ^ {(i)}\right) \Delta t + \tilde {\mu} _ {k} ^ {(i)}, \sqrt {\tilde {v} _ {k} ^ {(i)} \Delta t}\right)
$$

4. Normalize the weights 

$$
\tilde {w} _ {k} ^ {(i)} = \frac {w _ {k} ^ {(i)}}{\sum_ {i = 1} ^ {N _ {s i m s}} w _ {k} ^ {(i)}}
$$

5. Resample the points $\tilde { x } _ { k } ^ { ( i ) }$ and get $x _ { k } ^ { ( i ) }$ and reset $w _ { k } ^ { ( i ) } = \tilde { w } _ { k } ^ { ( i ) } = 1 / N _ { s i m s }$ This completes the generic particle filtering algorithm. Note that there is no Kalman filtering here and therefore 

$$
\hat {z} _ {k} ^ {-} = \frac {1}{N _ {s i m s}} \sum_ {i = 1} ^ {N _ {s i m s}} \hat {z} _ {k} ^ {(i)}
$$

with $\hat { z } _ { k } ^ { ( i ) }$ the estimation of $z _ { k }$ from $x _ { k - } ^ { ( i ) }$ 

$$
\hat {z} _ {k} ^ {(i)} = z _ {k - 1} + \left(\mu_ {S} + \lambda j - \frac {1}{2} \nu_ {k - 1} ^ {(i)}\right) \Delta t + \mu_ {k - 1} ^ {(i)}
$$

and the estimation error is $\boldsymbol { z } _ { k } - \boldsymbol { \hat { z } } _ { k } ^ { - }$ as before. 

The likelihood maximization is not different from the EPF or UPF. We need to maximize 

$$
\sum_ {k = 1} ^ {N} \ln \left(\sum_ {i = 1} ^ {N _ {s i m s}} w _ {k} ^ {(i)}\right)
$$

where $\boldsymbol { w _ { k } ^ { ( i ) } \ \mathrm { \overline { { s } } } }$ are defined at Step 3. 

Extended/Unscented Particle Filters Using the same model, we can take advantage of the independence of $\nu _ { k }$ and $\mu _ { k }$ and apply the (nonlinear) Gaussian Kalman filter to the former. In this case, the Steps 2 and 3 should be replaced with: 

2-a. Write $\hat { x } _ { k } ^ { ( i ) } = \left( \hat { \mu } _ { k } ^ { ( i ) } , \hat { \nu } _ { k } ^ { ( i ) } \right) ^ { t }$ with 

$$
\hat {\nu} _ {k} ^ {(i)} = \mathbf {K F} (\nu_ {k - 1} ^ {(i)})
$$

with $P _ { k } ^ { ( i ) }$ the associated a posteriori error covariance matrix, KF the extended or unscented Kalman filter, and 

$$
\hat {\mu} _ {k} ^ {(i)} = \mu_ {k - 1} ^ {(i)}
$$

2-b. Now take the simulations 

$$
\tilde {\nu} _ {k} ^ {(i)} \sim \mathcal {N} \left(\hat {\nu} _ {k} ^ {(i)}, P _ {k} ^ {(i)}\right)
$$

and 

$$
\tilde {\mu} _ {k} ^ {(i)} = 0
$$

if $\mathcal { U } [ 0 , 1 ] \leq e ^ { - \lambda \Delta t }$ and 

$$
\tilde {\mu} _ {k} ^ {(i)} = \ln (1 - j)
$$

otherwise. 

3. Define the weights 

$$
w _ {k} ^ {(i)} = w _ {k - 1} ^ {(i)} \frac {p (z _ {k} | \tilde {x} _ {k} ^ {(i)}) p (\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)})}{q (\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)} , z _ {1 : k})}
$$

with 

$$
\begin{array}{c} p \left(z _ {k} | \tilde {x} _ {k} ^ {(i)}\right) = n \left(z _ {k}, z _ {k - 1} + \left(\mu_ {S} + \lambda j - \frac {1}{2} \tilde {\nu} _ {k} ^ {(i)}\right) \Delta t + \tilde {\mu} _ {k} ^ {(i)}, \sqrt {\tilde {\nu} _ {k} ^ {(i)} \Delta t}\right) \\ p \left(\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}\right) = n \left(\tilde {\nu} _ {k} ^ {(i)}, \mathbf {m}, \mathbf {s} = \xi \sqrt {1 - \rho^ {2}} \sqrt {\nu_ {k - 1} ^ {(i)}} \sqrt {\Delta t}\right) p \left(\tilde {\mu} _ {k} ^ {(i)} | \mu_ {k - 1} ^ {(i)}\right) \end{array}
$$

with 

$$
\mathbf {m} = \nu_ {k - 1} ^ {(i)} + \left[ \omega - \rho \xi (\mu_ {S} + \lambda j) - \left(\theta - \frac {1}{2} \rho \xi\right) \nu_ {k - 1} ^ {(i)} \right] \Delta t + \rho \xi \ln \left(\frac {S _ {k}}{S _ {k - 1}}\right) - \rho \xi \mu_ {k - 1} ^ {(i)}
$$

and 

$$
q \left(\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}, z _ {1: k}\right) = n \left(\tilde {v} _ {k} ^ {(i)}, \hat {v} _ {k} ^ {(i)}, P _ {k} ^ {(i)}\right) p \left(\tilde {\mu} _ {k} ^ {(i)} | \mu_ {k - 1} ^ {(i)}\right)
$$

Note that as for the GPF, the terms $p \left( \tilde { \mu } _ { k } ^ { ( i ) } | \mu _ { k - 1 } ^ { ( i ) } \right)$ cancel out and need not be evaluated. 

The rest of the algorithm remains the same. This way we will not lose the information contained in the Kalman gain for the Gaussian dimension. 

The following is the C++ code for the application of EPF to the Bates model. 

```txt
// log_stock_prices are the log of stock prices
// muS is the real-world stock drift
// n_stock_prices is the number of the above stock prices
// (omega, theta, xi, rho, lambda, j) are the Bates parameters
// ll is the value of (negative log) Likelihood function
// estimates[] are the estimated observations from the filter 
```

```lisp
// The function ran2() is from Numerical Recipes in C
// and generates uniform random variables
// The function Normal_inverse() can be found from
many sources
// and is the inverse of the Normal CDF
// Normal_inverse(ran2(.)) generates a set of Normal
random variables

void estimate_particle_jump_diffusion_parameters_1_dim(
double *log_stock_prices,
double muS, int n_stock_prices,
double omega,
double theta,
double xi,
double rho,
double lambda,
double j,
double *ll,
double *estimates)
{
    int i1, i2, i3;
    double H, A, x0, P0, z;
    int M=1000;
    double x[1000], xx[1000], x1[1000], x2[1000];
    double mu[1000], mm[1000], m1[1000], m2[1000];
    double P[1000], P1[1000], U[1000], K[1000], W[1000];
    double w[1000], u[1000], c[1000];
    double q, pz, px, s, m, l;
    double delt=1.0/252.0, x1_sum, m1_sum;
    long idum=-1;
    int i1_prev=0;
    double u_t=0.0;
    int *jump;

    jump=new int [n_stock_prices];
    for (i1=0; i1<n_stock_prices; i1++)
    jump[i1]=0;

    A = 1.0-(theta-0.5*rho*xi)*delt;
    H = -0.5*delt;

    x0 = 0.04;
    P0 = 0.000001;
    for (i2=0; i2<M; i2++)
    { 
```

```lisp
x[i2] = x0 + sqrt(P0)* Normal_inverse(ran2(&idum));
mu[i2]=0;
P[i2] = P0;
}
*ll=0.0;
for (i1=1;i1<n_stock_prices-1;i1++)
{
    l = 0.0;
    x1_sum=0.0;
    m1_sum=0.0;
    for (i2=0; i2<M; i2++)
    {
    /* EKF for the proposal distribution */
    if (x[i2]<0) x[i2]=0.00001;
    x1[i2] = x[i2] + (omega-rho*xi*(muS+lambda*j) - (theta-0.5*rho*xi) * x[i2]) * delt +
    rho*xi* (log_stock_prices[i1]-
    log_stock_prices[i1-1]) - rho*xi*mu[i2];
    m1[i2]=mu[i2];
    W[i2] = xi*sqrt((1-rho*rho) * x[i2] * delt);
    P1[i2] = W[i2]*W[i2] + A*P[i2]*A;
    if (x1[i2]<0) x1[i2]=0.00001;
    U[i2] = sqrt(x1[i2]*delt);
    K[i2] = P1[i2]*H/( H*P1[i2]*H + U[i2]*U[i2]);
    z = log_stock_prices[i1+1];
    x2[i2] = x1[i2] + K[i2] *
    (z - (log_stock_prices[i1] + (muS+lambda*j-0.5*x1[i2])*delt + m1[i2]));
    m2[i2] = m1[i2];
    x1_sum+= x1[i2];
    m1_sum+= m1[i2];
    P[i2]=(1.0-K[i2]*H)*P1[i2];
    /* sample */
    xx[i2] = x2[i2] + sqrt(P[i2])*Normal_inverse(ran2(&idum));
    if (xx[i2]<0) xx[i2]=0.00001;

    if (ran2(&idum) < exp(-lambda*delt))
    mm[i2]=0.0;
    else
    mm[i2]=log(1.0-j);

    /* calculate weights */
    m = x2[i2]; 
```

```lisp
s = sqrt(P[i2]);
q = 0.39894228/s * exp(-0.5*(xx[i2] - m)*(xx[i2] - m)/(s*s));
m= log_stock_prices[i1] + (muS+lambda*j-0.5*xx[i2])*delt + mm[i2];
s= sqrt(xx[i2]*delt);
pz= 0.39894228/s *
exp(-0.5*(z - m)*(z - m)/(s*s));
m= x[i2] + (omega-rho*xi*(muS+lambda*j) - (theta-0.5*rho*xi) * x[i2]) * delt +
rho*xi*(log_stock_prices[i1]-
log_stock_prices[i1-1]) -rho*xi*mu[i2];
s= xi*sqrt((1-rho*rho) * x[i2] * delt);
px= 0.39894228/s *
exp(-0.5*(xx[i2] - m)*(xx[i2] - m)/(s*s))

w[i2]= pz * px / MAX(q, 1.0e-10);
l += w[i2];
}
*ll += log(l);
estimates[i1+1]= log_stock_prices[i1] + (muS+lambda*j-0.5*x1_sum/M)*delt+m1_sum/M;
/* normalize weights */
for (i2=0; i2<M; i2++)
    w[i2] /= l;
/* resample and reset weights */
c[0]=0;
for (i2=1; i2<M; i2++)
    c[i2] = c[i2-1] + w[i2];
i2=0;
u[0] = 1.0/M * ran2(&idum);
for (i3=0; i3<M; i3++)
{
    u[i3] = u[0] + 1.0/M *i3;
    while (u[i3] > c[i2])
    i2++;
    x[i3]= xx[i2];
    mu[i3]=mm[i2];
    w[i3]=1.0/M;
}
}

*ll *= -1.0;

delete [] jump; 
```

```txt
}
// *ll corresponds to the (negative log) Likelihood
// which we will need to minimize to obtain optimal parameters 
```

The Srivastava Approach Srivastava [222] suggests the following approach for simulating the jump component. Instead of allowing a jump at each time interval $[ t _ { k } , t _ { k } + \Delta t ]$ with a probability $1 - e ^ { - \lambda \Delta t }$ as we do now, we can flag the time steps such that 

$$
t _ {k - 1} <   \frac {1}{\lambda} \ln \left(\frac {1}{\mathcal {U} [ 0 , 1 ]}\right) \leq t _ {k}
$$

where $\boldsymbol { \mathcal { U } } [ 0 , 1 ]$ is a uniform random variable between zero and one, and then perform a jump of size $| \ln ( 1 - j ) |$ on these steps for all paths. We therefore would first initialize $t _ {  { p } } = 0$ and loop through k’s between 1 and N, and if 

$$
e ^ {- \lambda (t _ {k} - t _ {p})} \leq \mathcal {U} [ 0, 1 ] <   e ^ {- \lambda (t _ {k - 1} - t _ {p})}
$$

we flag this k and set $t _ { p } = t _ { k }$ and resimulate $\mathcal { U } [ 0 , 1 ]$ . In the particle filter, we would set for all indices i’s 

$$
\tilde {\mu} _ {k} ^ {(i)} = \ln (1 - j)
$$

for the flagged $k ^ { * } s .$ , and we would set $\tilde { \mu } _ { k } ^ { ( i ) } = 0$ for other indices. 

It is important to note that in this approach the simulation for the jump component is completely “orthogonal” to the diffusion SIS part. Indeed the index i in the foregoing is irrelevant for the entity $\tilde { \mu } _ { k } ^ { ( i ) }$ . This means that in the KF step, the weight calculation and the resampling are independent of the Jump component altogether. 

Numeric results As a check, we simulate a time series with the parameter set 

$$
\Psi^ {*} = (\omega^ {*} = 0, \theta^ {*} = 0, \xi^ {*} = 0, \rho^ {*} = 0, \lambda^ {*} = 2. 5 2, j ^ {*} = 0. 2 0)
$$

which corresponds to a jump frequency of $\lambda \Delta t = 0 . 0 1$ and a jump size of 20 <sup>percent.</sup> <sup>We</sup> <sup>generated</sup> N = 245 <sup>points</sup> <sup>and</sup> <sup>used</sup> M = 1000 <sup>particles.</sup> 

The estimated set via the above EPF is 

$$
\hat {\Psi} = (\hat {\omega} = 0. 2 3, \hat {\theta} = 1. 5, \hat {\xi} = 0. 3 4, \hat {\rho} = 0. 2 1, \hat {\lambda} = 2. 6 5, \hat {j} = 0. 2 0)
$$

As we see, the diffusion parameters are not close to the original ones, but this is probably due to the small $\Delta t .$ , as previously discussed. The jump parameters are close to the original ones, which means that the filter is valid for the jump component. Note that despite the difference in the diffusion parameters, the estimated and original time series are rather close for a new simulation, as can be seen in Figures 2.51 and 2.52. This reconfirms our previous remark: When the parameters affect the drift of the observation (as opposed to its noise), their estimation is far more accurate and requires fewer data points. 


Extended Particle Filter for Heston and Heston+Jumps Models


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/9824a65b4cdbf572fcbb9d33773ab892fbe789d7400608229916f113a9774e94.jpg)



FIGURE 2.51 Comparison of EPF Results for Heston and Heston+Jumps Models. The presence of jumps can be seen in the residuals.



Simulated versus Estimated Time Series


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/7d9a9e89-c767-4435-b922-5b8c275b0931/7489c6c8d81d061f057ba5bcd065df606e587a0ebaf6fff9fcd647147873a59c.jpg)



FIGURE 2.52 Comparison of EPF Results for Simulated and Estimated Jump-Diffusion Time Series. The filtered data matches the real data fairly well.


The Optimization Algorithm It is important to realize that the likelihood function here (owing to the jumps) is not differentiable everywhere, and, therefore, gradient-based maximization methods could not be applied. The optimization could, however, still be carried out via the direction set algorithm as previously described. Note that as mentioned in [164] so far there has been no formal proof on the convergence of the discretized jump diffusion equations toward the continuous ones; however, empirical evidence makes the convergence assumption plausible. 

## Pure Jump Models

The variance gamma with stochastic arrival (VGSA) and the variance gamma with gamma arrival (VGG) models were defined in Chapter 1. These models are non-Gaussian, and we could apply the particle filtering technique to them. We are not dealing with diffusion models, and therefore we do not have the Girsanov theorem. We are estimating the parameter set 

$$
\Psi = (\mu_ {S}, \theta , \sigma , \nu , \dots)
$$

In order to make the back-testing simpler, we suppose that we know the stock drift and try to estimate the other parameters. However, as mentioned earlier, for a high-frequency data set we have 

$$
\Delta t = o \left(\sqrt {\Delta t}\right)
$$

and the drift term has a negligible impact. 

VG The variance gamma model has the advantage of offering an integrated density, which allows us to calculate the exact likelihood. Calling $z =$ ln $( S _ { k } / S _ { k - 1 } )$ and $b = t _ { k } - t _ { k - 1 }$ and posing $\begin{array} { r } { x _ { b } = z - \mu _ { S } b - \frac { b } { \nu } \ln ( 1 - \theta \nu - \sigma ^ { 2 } \nu / 2 ) } \end{array}$ we have 

$$
p (z | b) = \frac {2 \exp (\theta x _ {b} / \sigma^ {2})}{\nu^ {\frac {b}{\nu}} \sqrt {2 \pi} \sigma \Gamma (\frac {b}{\nu})} \left(\frac {x _ {b} ^ {2}}{2 \sigma^ {2} / \nu + \theta^ {2}}\right) ^ {\frac {b}{2 \nu} - \frac {1}{4}} K _ {\frac {b}{\nu} - \frac {1}{2}} \left(\frac {1}{\sigma^ {2}} \sqrt {x _ {b} ^ {2} (2 \sigma^ {2} / \nu + \theta^ {2})}\right)
$$

and the likelihood is 

$$
L _ {1: N} = \prod_ {k = 1} ^ {N} p (z _ {k} | z _ {k - 1}, b)
$$

The implementation of this estimation procedure is straightforward and has already been done in [182]. 

One could also back-test the estimation procedure in the following way: First choose a parameter set $( \theta , \sigma , \nu )$ as well as a drift $\mu _ { S }$ and a time-step $\Delta t$ . Then simulate via Monte Carlo a gamma-distributed random variable as well as a Gaussian one. Deduce an artificial stock-price time series, apply the MLE procedure to it, and try to recover the original parameter set. 

Using $\Delta t = 1 / 2 5 2 , \mu _ { S } ^ { * } = 0 . 0 5$ , and 

$$
\theta^ {*} = 0. 0 2
$$

$$
\sigma^ {*} = 0. 2
$$

$$
\nu^ {*} = 0. 0 0 5
$$

We simulated 500 data points, applied the MLE, and found an optimal parameter set $\hat { \Psi } = ( 0 . 0 1 8 , \stackrel { \cdot } { 0 } . 2 2 , 0 . 0 \stackrel { \cdot } { 0 } 6 )$ , which is close to the original set. 

VGSA Using the same notations as in the previous chapter, the Euler discretized VGSA process could be written via the auxiliary variable 

$$
y _ {k} = y _ {k - 1} + \kappa (\eta - y _ {k - 1}) \Delta t + \lambda \sqrt {y _ {k - 1}} \sqrt {\Delta t} W _ {k - 1}
$$

and the state 

$$
x _ {k} = F _ {\nu} ^ {- 1} (y _ {k} \Delta t, \mathcal {U} [ 0, 1 ])
$$

as well as the observation $z _ { k } = \ln S _ { k + 1 }$ 

$$
z _ {k} = z _ {k - 1} + (\mu_ {S} + \omega) \Delta t + \theta x _ {k} + \sigma \sqrt {x _ {k}} B _ {k}
$$

with $\begin{array} { r } { \omega = \frac { 1 } { \nu } \ln ( 1 - \theta \nu - \sigma ^ { 2 } \nu / 2 ) } \end{array}$ 

The Filtering Algorithm The PF algorithm could therefore be written as follows. 

1. Initialize the arrival-rate $y _ { 0 } ^ { ( j ) } ,$ , the state $x _ { 0 } ^ { ( i ) }$ , and the weight $\boldsymbol { w } _ { 0 } ^ { ( i ) }$ for j between 1 and $M _ { s i m s }$ , and i between 1 and $N _ { s i m s }$ 

$$
\text { While } 1 \leq k \leq N
$$

2. Simulate the arrival-rate $y _ { k }$ for j between 1 and $M _ { s i m s }$ 

$$
y _ {k} ^ {(j)} = y _ {k - 1} ^ {(j)} + \kappa (\eta - y _ {k - 1} ^ {(j)}) \Delta t + \lambda \sqrt {y _ {k - 1} ^ {(j)} \sqrt {\Delta t}} \mathcal {N} ^ {- 1} \left(\mathcal {U} ^ {(j)} [ 0, 1 ]\right)
$$

3-a. Simulate the state $x _ { k }$ for each $y _ { k } ^ { ( j ) }$ and for i between 1 and $N _ { s i m s }$ 

$$
\tilde {x} _ {k} ^ {(i | j)} = F _ {\nu} ^ {- 1} \left(y _ {k} ^ {(j)} \Delta t, \mathcal {U} ^ {(i)} [ 0, 1 ]\right)
$$

3-b. Compute the unconditional state 

$$
\tilde {x} _ {k} ^ {(i)} = \int \tilde {x} _ {k} ^ {(i)} (y _ {k}) p (y _ {k} | y _ {k - 1}) d y _ {k} \approx \frac {1}{M _ {s i m s}} \sum_ {j = 1} ^ {M _ {s i m s}} \tilde {x} _ {k} ^ {(i | j)}
$$

4. Calculate the associated weights for each i 

$$
w _ {k} ^ {(i)} = w _ {k - 1} ^ {(i)} p \left(z _ {k} | \tilde {x} _ {k} ^ {(i)}\right)
$$

with 

$$
p \left(z _ {k} | \tilde {x} _ {k} ^ {(i)}\right) = n (z _ {k}, m, s)
$$

the normal density with mean $m = z _ { k - 1 } + ( \mu _ { S } + \omega ) \Delta t + \theta \tilde { x } _ { k } ^ { ( i ) }$ and standard deviation $s = \sigma \sqrt { \tilde { x } _ { k } ^ { ( i ) } }$ 

5. Normalize the weights 

$$
\tilde {w} _ {k} ^ {(i)} = \frac {w _ {k} ^ {(i)}}{\sum_ {i = 1} ^ {N _ {s i m s}} w _ {k} ^ {(i)}}
$$

6. Resample the points $\tilde { x } _ { k } ^ { ( i ) }$ and get $x _ { k } ^ { ( i ) }$ and reset $w _ { k } ^ { ( i ) } = \tilde { w } _ { k } ^ { ( i ) } = 1 / N _ { s i m s }$ 

7. Increment k, go back to Step 2, and Stop at the end of the While loop. 

Parameter Estimation As usual, the log likelihood to be maximized is 

$$
\ln (L _ {1: N}) = \sum_ {k = 1} ^ {N} \ln \left(\sum_ {i = 1} ^ {N _ {s i m s}} w _ {k} ^ {(i)}\right)
$$

The maximization takes place over the parameter set $\Psi = ( \kappa , \eta , \lambda , \nu , \theta , \sigma )$ Again, in reality the stock drift $\mu _ { S }$ should be estimated together with the other parameters; however, with a view to simplifying, we suppose we know $\mu _ { S }$ in our back-testing procedures. 

A More Efficient Algorithm We could take advantage of the fact that VG provides an integrated density of stock return. Calling $z = \ln ( S _ { k } / S _ { k - 1 } )$ and $b = t _ { k } - t _ { k - 1 } ,$ and posing $\begin{array} { r } { x _ { b } = z - \mu _ { S } b - \frac { b } { \nu } \ln ( 1 - \theta \nu - \sigma ^ { 2 } \nu / 2 ) } \end{array}$ , we have 

$$
p (z | b) = \frac {2 \exp (\theta x _ {b} / \sigma^ {2})}{\nu^ {\frac {b}{\nu}} \sqrt {2 \pi} \sigma \Gamma (\frac {b}{\nu})} \left(\frac {x _ {b} ^ {2}}{2 \sigma^ {2} / \nu + \theta^ {2}}\right) ^ {\frac {b}{2 \nu} - \frac {1}{4}} K _ {\frac {b}{\nu} - \frac {1}{2}} \left(\frac {1}{\sigma^ {2}} \sqrt {x _ {b} ^ {2} (2 \sigma^ {2} / \nu + \theta^ {2})}\right)
$$

As we can see, the dependence on the gamma distribution is “integrated out” in the above. 

For VGSA, for a given arrival rate $d t ^ { * } = y _ { t } d t$ , we have a VG distribution and 

$$
d \ln S _ {t} = (\mu_ {S} + \omega) d t + B (\gamma (d t ^ {*}, 1, \nu); \theta , \sigma)
$$

and the corresponding integrated density becomes 

$$
p (z | h, h ^ {*}) = \frac {2 \exp (\theta x _ {h} / \sigma^ {2})}{\nu^ {\frac {b ^ {*}}{\nu}} \sqrt {2 \pi} \sigma \Gamma (\frac {b ^ {*}}{\nu})} \left(\frac {x _ {h} ^ {2}}{2 \sigma^ {2} / \nu + \theta^ {2}}\right) ^ {\frac {b ^ {*} - 1}{2 \nu}} K _ {\frac {b ^ {*}}{\nu} - \frac {1}{2}} \left(\frac {1}{\sigma^ {2}} \sqrt {x _ {h} ^ {2} (2 \sigma^ {2} / \nu + \theta^ {2})}\right)\tag{2.31}
$$

Indeed, as described in [182] for VG, we have 

$$
p (z | h) = \int_ {0} ^ {+ \infty} p (z | g, h) p (g | h) d g
$$

with $\textstyle p ( z | g , b )$ a normal density and $p ( g | b )$ a gamma density. More accurately 

$$
p (z | g, h) = \frac {1}{\sigma \sqrt {2 \pi g}} \exp \left(- \frac {1}{2 \sigma^ {2} g} \left(z - \mu_ {S} h - \frac {h}{\nu} \ln \left(1 - \theta \nu - \sigma^ {2} \nu / 2\right) - \theta g\right) ^ {2}\right)
$$

and 

$$
p (g | b) = \frac {g ^ {\frac {b}{\nu} - 1} \exp (- \frac {g}{\nu})}{\nu^ {\frac {b}{\nu}} \Gamma (\frac {b}{\nu})}
$$

Now, for VGSA we simply have a different arrival rate $b ^ { * }$ for the gamma process and therefore 

$$
p (z | h, h ^ {*}) = \int_ {0} ^ {+ \infty} p (z | g, h) p (g | h ^ {*}) d g
$$

which demonstrates the point. This gives us the idea of using the arrival rate as the state, and we use the following algorithm. 

1. Initialize the state $x _ { 0 } ^ { ( i ) }$ and the weight $\boldsymbol { w } _ { 0 } ^ { ( i ) }$ for i between 1 and $N _ { s i m s }$ 

$$
\text { While } 1 \leq k \leq N
$$

2. Simulate the state $x _ { k }$ for i between 1 and $N _ { s i m s }$ 

$$
\tilde {x} _ {k} ^ {(i)} = x _ {k - 1} ^ {(i)} + \kappa (\eta - x _ {k - 1} ^ {(i)}) \Delta t + \lambda \sqrt {x _ {k - 1} ^ {(i)}} \sqrt {\Delta t} \mathcal {N} ^ {- 1} \left(\mathcal {U} ^ {(i)} [ 0, 1 ]\right)
$$

3. Calculate the associated weights for each i 

$$
w _ {k} ^ {(i)} = w _ {k - 1} ^ {(i)} p \big (z _ {k} | \tilde {x} _ {k} ^ {(i)} \big)
$$

with $p ( z _ { k } | \tilde { x } _ { k } ^ { ( i ) } )$ as defined in (2.31), where h will be set to $\Delta t$ and $b ^ { * }$ to the simulated state $\tilde { x } _ { k } ^ { ( i ) }$ times $\Delta t$ 

4. Normalize the weights 

$$
\tilde {w} _ {k} ^ {(i)} = \frac {w _ {k} ^ {(i)}}{\sum_ {i = 1} ^ {N _ {s i m s}} w _ {k} ^ {(i)}}
$$

5. Resample the points $\tilde { x } _ { k } ^ { ( i ) }$ and get $x _ { k } ^ { ( i ) }$ and reset $w _ { k } ^ { ( i ) } = \tilde { w } _ { k } ^ { ( i ) } = 1 / N _ { s i m s }$ 

6. Increment $k , \mathrm { g o }$ back to Step 2 and Stop at the end of the While loop. 

The advantage of this method is that there is one simulation process instead of two, and we “skip” the gamma distribution altogether. However, the dependence of the observation $z _ { k }$ on $x _ { k }$ is highly nonlinear, which makes the convergence more difficult. 

An Extended/Unscented Particle Filter Finally, a natural idea would be to use a proposal distribution $q ( x )$ for the state, taking into account the observation information. In order to be able to use a Kalman-based proposal distribution (EPF or UPF), we need a Gaussian approximation. Note that given the strong non-Gaussianity of the equations, we absolutely need the particle filtering aspect. The Gaussian approximation for the observation equation would $\mathrm { b e } ^ { 3 9 }$ 

$$
z _ {k} = z _ {k - 1} + \left(\mu_ {S} + \omega + \theta x _ {k}\right) \Delta t + \sqrt {\theta^ {2} \nu + \sigma^ {2}} \sqrt {x _ {k} \Delta t} B _ {k}
$$

which is of the form $z _ { k } = b ( x _ { k } , B _ { k } )$ and allows us to use the Kalman filtering algorithm. We therefore replace Steps 2 and 3 of the previous algorithm with the following. 

2-a. Apply an extended/unscented Kalman filter for i between 1 and $N _ { s i m s }$ to the state $x _ { k - 1 } ^ { ( i ) }$ and obtain 

$$
\hat {x} _ {k} ^ {(i)} = \mathbf {K F} \left(x _ {k - 1} ^ {(i)}\right)
$$

as well as the associated covariance $P _ { k } ^ { ( i ) }$ 

2-b. Simulate the state for i between 1 and $N _ { s i m s }$ 

$$
\tilde {x} _ {k} ^ {(i)} = \hat {x} _ {k} ^ {(i)} + \sqrt {P _ {k} ^ {(i)}} \mathcal {N} ^ {- 1} \left(\mathcal {U} ^ {(i)} [ 0, 1 ]\right)
$$

3. Calculate the associated weights for each i 

$$
w _ {k} ^ {(i)} = w _ {k - 1} ^ {(i)} \frac {p \left(z _ {k} | \tilde {x} _ {k} ^ {(i)}\right) p \left(\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)}\right)}{q \left(\tilde {x} _ {k} ^ {(i)} | x _ {k - 1} ^ {(i)} , z _ {1 : k}\right)}
$$

with $p \left( z _ { k } | \tilde { x } _ { k } ^ { ( i ) } \right)$ as defined in (2.31), where h will be set to t and $b ^ { * }$ to the simulated state $\tilde { x } _ { k } ^ { ( i ) }$ times $\Delta t$ , where $p \left( \tilde { x } _ { k } ^ { ( i ) } | x _ { k - 1 } ^ { ( i ) } \right)$ is the normal density with mean $x _ { k - 1 } ^ { ( i ) } + \kappa \left( \eta - x _ { k - 1 } ^ { ( i ) } \right) \Delta t$ and standard deviation $\lambda \sqrt { x _ { k - 1 } ^ { ( i ) } } \sqrt { \Delta t } ,$ and where $q \left( \tilde { x } _ { k } ^ { ( i ) } | x _ { k - 1 } ^ { ( i ) } , z _ { 1 : k } \right)$ is the normal density with mean $\hat { x } _ { k } ^ { ( i ) }$ and standard deviation $\sqrt { P _ { k } ^ { ( i ) } }$ 

The rest of the algorithm is exactly the same as the previous one. What follows is a C++ routine for the EPF applied to VGSA. 

```c
// log_stock_prices are the log of stock prices
// muS is the real-world stock drift
// n_stock_prices is the number of the above stock prices
// (kappa,eta,lambda,sigma,theta,nu) are the VGSA parameters
// ll is the value of (negative log) Likelihood function
// estimates[] are the estimated observations from the filter
// errors are the observation errors

// The function ran2() is from Numerical Recipes in C
// and generates uniform random variables
// The function Normal_inverse() can be found from many sources
// and is the inverse of the Normal CDF
// Normal_inverse(ran2(.)) generates a set of Normal random variables

// The Bessel and Gamma functions bessik() and gammln()
// are also available in Numerical Recipes in C

void estimate_particle_extended_VGSA_parameters_bessel(
double *log_stock_prices,
double mu,
int n_stock_prices,
double kappa,
double eta,
double lambda,
double sigma,
double theta,
double nu,
double *ll,
double *estimates, 
```

```lisp
double *errors)
{
    int i1, i2, i3;
    double y0, z, omega;
    int M=1000;
    double x[1000], xx[1000], X;
    double w[1000], u[1000], c[1000];
    double pz, px, q, s, m, l, x1_sum;
    long idum=-1;
    double delt=1.0/252.0;
    double eps=1.0e-30;
    double Ka, Ia, Kp, Ip, Kx, Knu;

    double H, A, x0, P0;
    double P[1000], P1[1000], U[1000], K[1000], W[1000];
    double x1[1000], x2[1000];

    /* initialize */
    omega=log(1.0-theta*nu- sigma*sigma*nu/2.0)/nu;
    x0 = 1.0;
    P0 = 0.000001;
    for (i2=0; i2<M; i2++)
    {
    x[i2] = x0 + sqrt(P0)* Normal_Inverse(ran2(&idum));
    P[i2] = P0;
    }
    A = 1.0-kappa*delt;
    H = theta*delt;
    /* time loop */
    *ll=0.0;
    for (i1=1;i1<n_stock_prices-1;i1++)
    {
    z = log_stock_prices[i1+1]-log_stock_prices[i1];
    X=z - mu*delt - delt/nu*log(1.0-theta*nu-sigma*sigma*nu/2.0);
    l = 0.0;
    x1_sum=0.0;
    for (i2=0; i2<M; i2++)
    {
    /* EKF for the proposal distribution */
    x1[i2] = x[i2] + kappa*(eta - x[i2])*delt;
    W[i2] = lambda*sqrt(x[i2] * delt);
    P1[i2] = W[i2]*W[i2] + A*P[i2]*A;
    x1[i2]=MAX(x1[i2],eps);
    }
} 
```

```txt
U[i2] = sqrt(theta*theta*nu+sigma*sigma)*sqrt(x1[i2]*delt);
K[i2] = P1[i2]*H/( H*P1[i2]*H + U[i2]*U[i2]);
x2[i2] = x1[i2] + K[i2] *
(z - (mu+omega+theta*x1[i2])*delt);
x1_sum+= x1[i2];
P[i2]=(1.0-K[i2]*H)*P1[i2];
/* sample */
xx[i2] = x2[i2] + sqrt(P[i2])*Normal_Inverse(ran2(&idum));
xx[i2]=MAX(xx[i2],eps);
/* calculate weights */
m = x2[i2];
s = sqrt(P[i2]);
q = 0.39894228/s * exp(-0.5*(xx[i2]-m)*(xx[i2]-m)/(s*s));
m = x[i2] + kappa*(eta-x[i2])*delt;
s = lambda*sqrt(x[i2]*delt);
px = 0.39894228/s * exp(-0.5*(xx[i2]-m)*(xx[i2]-m)/(s*s));
Kx = MAX(eps, 1.0/(sigma*sigma)*sqrt(X*X*(2*sigma*sigma/nu+theta*theta)));
Knu = MAX(eps, (xx[i2]*delt/nu-0.5));
bessik(Kx, Knu, &Ia, &Ka, &Kp, &Ip);
pz=2.0*exp(theta*X/(sigma*sigma)) / (pow(nu,xx[i2]*delt/nu)*sigma*
exp(gammln(xx[i2]*delt/nu)) *0.39894228*
pow(X*X/(2*sigma*sigma/nu+theta*theta), 0.5*xx[i2]*delt/nu-0.25) * Ka;

w[i2]=pz * px / MAX(q, eps);
l += w[i2];
}
*ll += log(l);
/* estimates[i1+1] for z[i1] => error term */
estimates[i1+1]=log_stock_prices[i1+1]-(log_stock_prices[i1] + (mu+omega+theta*x1_sum/M)*delt);
errors[i1] = (theta*theta*nu + sigma*sigma)*x1_sum/M*delt;
/* normalize weights */
for (i2=0; i2<M; i2++)
    w[i2] /= l;
/* resample and reset weights */
c[0]=0; 
```

<!-- === Source: MinerU_markdown_Inside_Volatility_Arbitrage-Javaheri_201_2122707067558010898.md (Page 201) === -->

```txt
for (i2=1; i2<M; i2++)
    c[i2] = c[i2-1] + w[i2];
i2=0;
u[0] = 1.0/M * ran2(&idum);
for (i3=0; i3<M; i3++)
{
    u[i3] = u[0] + 1.0/M *i3;
    while (u[i3] > c[i2])
    i2++;
    x[i3] = xx[i2];
    w[i3]=1.0/M;
}
}
*ll *= -1.0;
// *ll represents the (negative log) Likelihood 
```

Numeric Results We performed the same kind of back-testing procedure as for the VG model, using either of the foregoing particle filters applied to an artificially generated stock-price time series. We chose $\Delta t = 1 / 2 5 2 , \mu _ { S } ^ { * } = 0 ,$ $y _ { 0 } = 1$ and 

$$
\Psi^ {*} = (\kappa^ {*} = 0, \eta^ {*} = 0, \lambda^ {*} = 0, \nu^ {*} = 0. 0 0 5, \theta^ {*} = 0. 0 2, \sigma^ {*} = 0. 2)
$$

after applying the importance sampling/resampling PF via the modified Bessel function, we found 

$$
\hat {\Psi} = (0. 1 3, 0. 0 0 1, 0. 3 7, 0. 0 0 4 8, 0. 0 1 8, 0. 2 1)
$$

which seems to indicate that the estimation process for $( \nu , \theta , \sigma )$ works well, whereas the one for $( \kappa , \eta , \lambda )$ does not. However, if we simulate two sets of spot-price times series with these different parameter sets, we will see that the generated paths are very similar. See Figures 2.53 and 2.54. This also confirms our previous remarks about the estimation of the parameters affecting the noise. 

We performed a second test with a more realistic choice of parameters, with once again $\Delta t = 1 / 2 5 2 , N _ { s i m s } = 1 0 0$ , and 500 data points corresponding to two years. The real values were 

$$
\Psi^ {*} = (\kappa^ {*} = 2. 1 0, \eta^ {*} = 5. 7 0, \lambda^ {*} = 2. 0 0, \nu^ {*} = 0. 0 5, \theta^ {*} = - 0. 4 0, \sigma^ {*} = 0. 2 0)
$$


Simulated Arrival Rates


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/d151237876726c666ace1de08d9cef4a2fe9794d1fdc0b8a6bc0fc244e2631bd.jpg)



FIGURE 2.53 The Simulated Arrival Rates via $\Psi \ = \ ( \kappa \ = \ 0 , \eta \ = \ 0 , \lambda \ = \ 0 ,$ $\sigma = 0 . 2 , \theta = 0 . 0 2 , \nu = 0 . 0 0 5 )$ and $\Psi = ( \kappa = 0 . 1 3 , \eta = 0 , \lambda = 0 . 4 0 , \sigma = 0 . 2 ,$ $\theta = 0 . 0 2 , \nu = 0 . 0 0 5 )$ Are Quite Different; compare with Figure 2.54.



Simulated Log Stock Prices


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/b96dd4fc033c79b262f4689c7809fc837e4228f48926efba501781b6ba3b9f59.jpg)



FIGURE 2.54 However, the Simulated Log Stock Prices are Close. (Compare with Figure 2.53.)


Note that θ has a negative value that corresponds to the negative skewness of the distribution. We choose a fairly reasonable initial set 

$$
\Psi_ {0} = (\kappa_ {0} = 2. 0 0, \eta_ {0} = 6. 0 0, \lambda_ {0} = 1. 5 0, \nu_ {0} = 0. 0 3, \theta_ {0} = - 0. 3 0, \sigma_ {0} = 0. 3 0)
$$

and 

$$
\mu_ {0} = \mu^ {*} = 0. 0 5
$$

We find the optimal parameter set 

$$
\hat {\Psi} = (\hat {\kappa} = 4. 2 5, \hat {\eta} = 7. 8 9, \hat {\lambda} = 3. 2 5, \hat {\nu} = 0. 0 4 7, \hat {\theta} = - 0. 4 0, \hat {\sigma} = 0. 1 9)
$$

and 

$$
\hat {\mu} = \mu^ {*} = 0. 0 5
$$

Again we see that the estimations for the three VG parameters $( \nu , \theta , \sigma )$ are much more accurate than those corresponding to the arrival process $( \kappa , \eta , \lambda )$ —and this despite our choosing the initial arrival parameters close to the real ones. As previously stated, the time series of spot prices has little sensitivity to the arrival-rate parameters and a higher degree of sensitivity to the gamma process parameters. Again, this shows that estimation methodologies such as MLE work much better when applied to parameters that affect the drift of an observation, and not its noise. 

Diagnostics As for diagnostics, we need to estimate the observation error associated with the algorithm. We define once again 

$$
\begin{array}{r} \hat {z} _ {k} ^ {(i)} = z _ {k - 1} + (\mu_ {S} + \omega + \theta \tilde {x} _ {k} ^ {(i)}) \Delta t \\ \hat {z} _ {k} ^ {-} = \frac {1}{N _ {s i m s}} \sum_ {i = 1} ^ {N _ {s i m s}} \hat {z} _ {k} ^ {(i)} \end{array}
$$

or 

$$
\hat {z} _ {k} ^ {-} = z _ {k - 1} + (\mu_ {S} + \omega) \Delta t + \theta \Delta t \frac {1}{N _ {s i m s}} \sum_ {i = 1} ^ {N _ {s i m s}} \tilde {x} _ {k} ^ {(i)}
$$

and the error term 

$$
e _ {k} = z _ {k} - \hat {z} _ {k} ^ {-}
$$

The variance associated with this error is 

$$
s _ {k} = \left(\theta^ {2} \nu + \sigma^ {2}\right) \frac {1}{N _ {s i m s}} \sum_ {i = 1} ^ {N _ {s i m s}} \tilde {x} _ {k} ^ {(i)} \Delta t
$$

and 

$$
\tilde {e} _ {k} = e _ {k} / s _ {k}
$$

would represent the normalized error. 


VGSA Observation Errors with GPF


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/c3a374d4054ffeafed270c15d7e791e7b9457316c3646e3a2b879e5b89abda49.jpg)



FIGURE 2.55 The Observation Errors for the VGSA Model with a Generic Particle Filter.



TABLE 2.15 MPE and RMSE for the VGSA Model Under a Generic PF as well as the EPF.


<table><tr><td></td><td>MPE</td><td>RMSE</td></tr><tr><td>PF</td><td>-0.000350241</td><td>0.005867065</td></tr><tr><td>EPF</td><td>-4.74747e-07</td><td>0.005869782</td></tr></table>

MPE/RMSE In order to measure the performance, once again we use the mean price error (MPE) and the root mean-squared error (RMSE). As an example, we use the S&P 500 data between 1992 and 1994 (as used in [182]). For the generic particle filter (GPF) and the extended particle filter (EPF), we find the results in Table 2.15. 

As we can see, the use of the extended Kalman filter as the proposal distribution brings some improvement. Also see Figures 2.55 and 2.56. 

Chi-Square Test The residuals are normal; a $\chi _ { 2 0 } ^ { 2 }$ test provides us with a value of 10.397699, which is below the threshold value of 31.5 for a confidence of 0.95. This means that the non-Gaussianity was “filtered out” of the time series successfully. This could also be observed in the corresponding histogram in Figure 2.57. 


VGSA Observation Errors with EPF


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/5fb1ef6e83add13841af0dc7ef8d4c45f31d0af17aee94baa295dab2c5a7ebb4.jpg)



FIGURE 2.56 The Observation Errors for the VGSA Model and an Extended Particle Filter.



Histogram for the VGSA Residuals


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/e85df7f5b4ccd5ccd4472ddf4525a59d1ca0081d5cdf0523d879667bdaa37297.jpg)



FIGURE 2.57 The VGSA Residuals Histogram. The residuals are fairly normal.



Variogram for the VGSA Residuals


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/9fe05f29347b2cdf4d6e7a8c725dd64c28ef1c4387459064637e276442a719c7.jpg)



FIGURE 2.58 The VGSA Residuals Variogram. The variogram is close to 1 as expected.


Auto-Correlation Having $\ b = 7$ parameters and taking $K = 2 7$ , we shall have $K - p = 2 0$ , so we will compare the output of the Box-Ljung test to the $\chi _ { 2 0 } ^ { 2 }$ threshold, which, as previously mentioned, for a confidence of 0.95 is around 31.5. We find a value of 0.001138, which definitely passes the test. This shows that the residuals are indeed uncorrelated. 

Variogram The variogram still indicates that we have independent and identically distributed random variables. Calling 

$$
\gamma_ {b} = \frac {1}{2} \mathbf {E} \left[ (\tilde {e} _ {k + b} - \tilde {e} _ {k}) ^ {2} \right] = \frac {1}{2} \mathbf {E} \left[ \tilde {e} _ {k + b} ^ {2} \right] + \frac {1}{2} \mathbf {E} \left[ \tilde {e} _ {k} ^ {2} \right] - \mathbf {E} [ \tilde {e} _ {k + b} \tilde {e} _ {k} ]
$$

we should obtain $\frac { 1 } { 2 } + \frac { 1 } { 2 } - 0 = 1$ , which is indeed the case as seen in Figure 2.58. 

VGG The observation is $z _ { k } = \ln S _ { k + 1 }$ 

$$
z _ {k} = z _ {k - 1} + (\mu_ {S} + \omega) \Delta t + \theta x _ {k} + \sigma \sqrt {x _ {k}} B _ {k}
$$

with $\begin{array} { r } { \omega = \frac { 1 } { \nu } \ln ( 1 - \theta \nu - \sigma ^ { 2 } \nu / 2 ) } \end{array}$ , and the hidden state is 

$$
x _ {k} = Y _ {k} (\Delta t)
$$

We could take advantage of the fact that VG provides an integrated density of stock return [182]. Calling $z = \ln ( S _ { k } / S _ { k - 1 } )$ and $b = t _ { k } - t _ { k - 1 }$ and posing 

$$
\xi_ {b} = z - \mu_ {S} b - \frac {b}{\nu} \ln (1 - \theta \nu - \sigma^ {2} \nu / 2)
$$

we have 

$$
p (z | b) = \frac {2 \exp (\theta \xi_ {b} / \sigma^ {2})}{\nu^ {\frac {b}{\nu}} \sqrt {2 \pi} \sigma \Gamma (\frac {b}{\nu})} \left(\frac {\xi_ {b} ^ {2}}{2 \sigma^ {2} / \nu + \theta^ {2}}\right) ^ {\frac {b}{2 \nu} - \frac {1}{4}} K _ {\frac {b}{\nu} - \frac {1}{2}} \left(\frac {1}{\sigma^ {2}} \sqrt {\xi_ {b} ^ {2} (2 \sigma^ {2} / \nu + \theta^ {2})}\right)
$$

where $K _ { \alpha } ( x )$ corresponds to the modified Bessel function of second kind. As we can see, the dependence on the gamma distribution is “integrated out.” For the VGG for a given arrival rate $d t ^ { * } = d Y _ { t }$ we have a VG distribution and 

$$
d \ln S _ {t} = (\mu + \omega) d t + B (\gamma (d t ^ {*}, 1, \nu); \theta , \sigma)
$$

and the corresponding integrated density becomes 

$$
p (z | b, b ^ {*}) = \frac {2 \exp (\theta \xi_ {b} / \sigma^ {2})}{\nu^ {\frac {b ^ {*}}{\nu}} \sqrt {2 \pi} \sigma \Gamma (\frac {b ^ {*}}{\nu})} \left(\frac {\xi_ {b} ^ {2}}{2 \sigma^ {2} / \nu + \theta^ {2}}\right) ^ {\frac {b ^ {*} - 1}{2 \nu}} K _ {\frac {b ^ {*}}{\nu} - \frac {1}{2}} \left(\frac {1}{\sigma^ {2}} \sqrt {\xi_ {b} ^ {2} (2 \sigma^ {2} / \nu + \theta^ {2})}\right)\tag{2.32}
$$

hence the idea of using the arrival rate as the state and using the following algorithm. 

1. Initialize the state $x _ { 0 } ^ { ( i ) }$ and the weight $\boldsymbol { w } _ { 0 } ^ { ( i ) }$ for i between 1 and $N _ { s i m s }$ 

$$
\text { While } 1 \leq k \leq N
$$

2. Simulate the state $x _ { k }$ for i between 1 and $N _ { s i m s }$ 

$$
\tilde {x} _ {k} ^ {(i)} = F ^ {- 1} \big (\mu_ {a}, \nu_ {a}; \Delta t, \mathcal {U} ^ {(i)} [ 0, 1 ] \big)
$$

where as before F represents the gamma CDF. 

3. Calculate the associated weights for each i 

$$
w _ {k} ^ {(i)} = w _ {k - 1} ^ {(i)} p (z _ {k} | \tilde {x} _ {k} ^ {(i)})
$$

with $p ( z _ { k } | \tilde { x } _ { k } ^ { ( i ) } )$ as defined in (2.32) where h will be set to $\Delta t$ and $b ^ { * }$ to $\tilde { x } _ { k } ^ { ( i ) }$ 

4. Normalize the weights 

$$
\tilde {w} _ {k} ^ {(i)} = \frac {w _ {k} ^ {(i)}}{\sum_ {i = 1} ^ {N _ {s i m s}} w _ {k} ^ {(i)}}
$$

5. Resample the points $\tilde { x } _ { k } ^ { ( i ) }$ and get $x _ { k } ^ { ( i ) }$ and reset $w _ { k } ^ { ( i ) } = \tilde { w } _ { k } ^ { ( i ) } = 1 / N _ { s i m s }$ 

6. Increment k, go back to Step 2 and Stop at the end of the While loop. 

As for VGSA, numeric tests were carried out in the following way. After choosing a time step $\Delta t = 1 / 2 5 2 , \mu _ { S } = 0$ and a parameter set 

$$
\Psi = (\mu_ {a} = 1 0. 0, \nu_ {a} = 0. 0 1, \nu = 0. 0 5, \sigma = 0. 2, \theta = 0. 0 0 2)
$$

an artificial time series of $N = 5 0 0$ spot prices was generated. The preceding filtering algorithm was then applied to this time series and the resulting likelihood was maximized. The optimal parameter set was 

$$
\hat {\Psi} = (9. 1 7, 0. 1 9, 0. 0 1 2, 0. 2 1, 0. 0 0 1 9)
$$

It therefore seems that the parameters ν and $\nu _ { a }$ are not recovered properly. Hence we ask, how sensitive are the observable spot prices to these variables? Simulating two time series with the two different parameter sets, we can see in Figure 2.59 that the results could be very close. This once again brings up the issue of inference reliability. Not having enough data points, we can get parameter sets that are quite different from the real ones and that could generate similar time series. This is consistent with what we have seen for diffusion-based processes. 


Simulated Log Stock Prices


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/03629a8bbc25c5688b74421757637202a6378938f5eb61613fa79105987f785a.jpg)



FIGURE 2.59 Simulation of VGG-based Log Stock Prices with Two Different Parameter Sets $\Psi = ( \mu _ { a } = 1 0 . 0 , \nu _ { a } = 0 . 0 1 , \nu = 0 . 0 5 , \sigma = 0 . 2 , \theta = 0 . 0 0 2 )$ and $\Psi =$ (9.17 0.19 0.012 0.21 0.0019). The observed time series remain close.


A Bayesian Approach for VGSA An approach similar to the one in the paragraph on the Bayesian approach for Heston could be used here, because the latent state follows the same square-root SDE. The only thing that changes is the likelihood function. Instead of having a conditionally log normal observation, we have a conditionally VG observation. Furthermore, we do know the density of the VG distribution under a closed form as previously mentioned. 

Indeed as previously mentioned, we have the state (the arrival rate) 

$$
d y _ {t} = \kappa (\theta - y _ {t}) d t + \sigma_ {y} \sqrt {y _ {t}} d W _ {t}
$$

and the observation 

$$
d \ln S _ {t} = (\mu_ {S} + \omega) d t + B (\gamma (d t ^ {*}, 1, \nu); \theta , \sigma)
$$

and the corresponding conditional likelihood becomes 

$$
\begin{array}{r} p (\ln S _ {k} | y _ {k}, \Psi) = \frac {2 \exp (\theta x _ {b} / \sigma^ {2})}{\nu^ {\frac {b ^ {*}}{\nu}} \sqrt {2 \pi} \sigma \Gamma (\frac {b ^ {*}}{\nu})} \left(\frac {x _ {b} ^ {2}}{2 \sigma^ {2} / \nu + \theta^ {2}}\right) ^ {\frac {b ^ {*} - 1}{2 \nu}} \\ \times K _ {\frac {b ^ {*}}{\nu} - \frac {1}{2}} \left(\frac {1}{\sigma^ {2}} \sqrt {x _ {b} ^ {2} (2 \sigma^ {2} / \nu + \theta^ {2})}\right) \end{array}
$$

with $K _ { \alpha } ( x )$ the modified Bessel function and 

$$
\begin{array}{l} {x _ {b} = \ln (S _ {k} / S _ {k - 1}) - \mu_ {S} b - \frac {b}{\nu} \ln \bigl (1 - \theta \nu - \sigma^ {2} \nu / 2 \bigr)} \\ {b = \Delta t} \end{array}
$$

and 

$$
b ^ {*} = y _ {k} \Delta t
$$

Finally, integrating over time, we have 

$$
p (\ln S | y, \Psi) = \prod_ {k = 1} ^ {N} p (\ln S _ {k} | y _ {k}, \Psi)
$$

Note that in the classical VGSA model there is no correlation between the system noise and the observation noise. This means that the likelihood function will not depend on the parameters $\kappa , \theta , \sigma _ { y }$ , and therefore the MH update step becomes almost a Gibbs sampler (except for the adjustment factor $\textstyle \sum _ { k = 1 } ^ { N } x _ { k } ^ { 2 } )$ 

## RECAPITULATION

We tested three categories of models: the Heston/GARCH category where a pure diffusion assumption was used, the Bates category where Poisson jumps were added to the stock SDE, and the VG category where a gamma distribution was applied to the time dimension. 

## Model Identification

We saw from the table in Section 2.3.10 that in the pure diffusion category, a power of $3 / 2$ outperformed the Heston model (power of $1 / 2 )$ . As stated, this is in line with the findings of Engle & Ishida [95]. 

Needless to say, adding Poisson jumps (Bates model) will reduce the MPE/RMSE of the filters; however, it will also cause the number of parameters to increase. A simple comparison between the residual errors is therefore not fair. In other words, given the fundamental differences between the categories, we need to judge their appropriateness not by comparing the residuals, but by using financial arguments such as, should the stock process contain jumps or not? Once a category is chosen, then we can compare the performance of models belonging to a given category. 

Note that a number of likelihood-based tools exist, such as the Akaike information criterion [100], which will take into the account the number of parameters when assessing the goodness of fit for a model. These tools would therefore allow us to compare models belonging to different categories (e.g, Heston vs. VGSA). However, these criteria remain valid only asymptotically. As we saw, this often requires a large number of data points, which may or may not be readily available. 

## Convergence Issues and Solutions

No matter which category we choose, it seems that the same convergence issues exist. For all the foregoing models, we can see that a parameter affecting the drift of the observation is much easier to estimate than one affecting the noise of the observation. For the pure diffusion category, we saw that all four parameters $\omega , \theta , \xi ,$ and $\rho$ were difficult to estimate (in some cases) and that the two latter parameters, which affect the noise of the noise, were even harder to estimate properly. For the Bates model, we saw that the jump parameters $\lambda , j$ were much more straightforward to estimate than the aforementioned four diffusion parameters. For the VGSA models, we saw that the VG parameters $\theta , \nu ,$ and $\sigma$ (which once again, affect the observation drift) are much easier to infer than the arrival-rate parameters $\kappa , \eta ,$ and λ. 

All this was explained via the poor observability at a daily frequency level owing to the fact that $\Delta t = o \left( \sqrt { \Delta t } \right)$ . We tested the validity of this statement by artificially reducing the observation noise and saw the convergence rate increase dramatically. 

As stated, a possible solution would be to employ more observation points via the use of high-frequency data. We saw that the increase in the number of observations and the decrease in $\Delta t$ (after a certain level) do not cancel, and a higher frequency would indeed cause the likelihood function to have a higher value and provide a better estimation of the parameters. In any case, because we do not know in advance how good the inference results will be and whether we are in the asymptotic area or not, it is always a good idea to perform a simulation test and determine the sampling distribution of each parameter. 

In the next chapter, we shall apply these inference tools to a specific question: are the implied distributions from the stock and options markets consistent? 

# The Consistency Problem

Whether cross-sectional option prices are consistent with the time-series properties of the underlying asset returns is probably the most fundamental of tests. 

— David S. Bates 

## INTRODUCTION

In the previous chapter, we discussed two approaches for stochastic volatility parameter estimation: the cross-sectional one, in which we use a number of options prices for given strike prices (and possibly maturities), and the time-series approach, in which we use the stock prices over a certain period of time. One natural question<sup>1</sup> would therefore be the following: Will the theoretically invariant portion of the parameter sets obtained by the two methods be the same? 

More accurately, supposing we are at time $t = 0$ and we use J options with strikes $K _ { 1 } , . . . , K _ { J }$ and with maturity T , we have 

$$
\begin{array}{c} \hat {\Psi} _ {o p t i o n s} = a r g m i n \left\{\sum_ {j = 1} ^ {J} \left[ C _ {m o d e l} (t = 0, S _ {0}, K _ {j}, T, \Psi) \right. \right. \\ \left. \left. - C _ {m k t} (t = 0, S _ {0}, K _ {j}, T) \right] ^ {2} \right\} \end{array}\tag{3.1}
$$

These options could include calls or puts. Alternatively, during the period [0 T ] we can observe $( S _ { k } ) _ { 0 \leq k \leq N }$ corresponding to the time points $t _ { 0 } , . . . , t _ { N }$ with $t _ { 0 } = 0$ and $t _ { N } = T _ { \mathrm { { 3 } } }$ , and then apply one of the previously discussed filters and estimate the parameter set via the maximum likelihood method. 

$$
\hat {\Psi} _ {s t o c k s} = a r g m a x \{L (S _ {0}, \dots , S _ {N}, \Psi) \}\tag{3.2}
$$

Now the question is how different these estimations for $( \xi , \rho )$ are and why. 

As we saw in the previous chapter, the size of the time interval $\Delta t$ and the time-series length are to be questioned: Indeed $\Delta t$ has to be small enough for us to be able to apply the Girsanov theorem. However, we saw that for a very small $\Delta t ,$ the filtering errors are so little that the MLE will not necessarily converge to the right parameter set. On the other hand, we would need the time series to be as long as possible, which requires a high observation frequency. 

This brings up a more fundamental question. The current financial econometrics literature seems to make inference-based conclusions using a limited amount of daily data. As we saw in Chapter 2, the time-series inference results are not necessarily reliable unless the number of observations is sufficiently large. This is the central question of this chapter: Are the implied parameters from the options markets and the assets time series indeed inconsistent? 

Many practical issues need to be questioned: How many strikes should we be using in the cross-sectional analysis and which ones? Should we use only OTM puts and calls for liquidity reasons? Many use a penalty function $p ( \ v u )$ in the cross-sectional optimization in order to get reasonable results. Do we need such a function here? In the cross-sectional method, what value for $\nu _ { 0 }$ are we using? Should we estimate this value together with the other four parameters? If so, should this estimated $\hat { \nu } _ { 0 }$ be used in the time series? 

If the results are substantially different for the parameters $\xi$ and $\rho$ (assuming the validity of the Girsanov theorem), can this test be used as an argument against the validity of the Heston stochastic volatility model? Or would it mean that the options markets do not predict the stock movements as they should? And if so, does this mean that there is a profitable trading strategy to take? That is, are options systematically mispriced? 

If the Heston model is judged to be incorrect, what is the correct model—GARCH or 3/2? Is the diffusion assumption itself to be questioned? Do we need to introduce jumps?<sup>2</sup> 

Another way to approach the question is to reason in the following manner. If the information contained in the options markets is indeed inconsistent with the one embedded in the assets time series, there should be a regularly and conclusively profitable trade strategy. For instance, a higher volatility-of-volatility and more negative correlation in the options market should indicate the possibility of a profitable skewness trade (to be explained later) in absence of crashes. We could therefore use the profit/loss of this trade as an empirical measure of the inconsistency of the information. 

If (and only if!) there exists a regular and definite profit generated from this strategy, we can conclude that there is inconsistency. It is important to note that this empirical measure is model free. 

In our empirical analysis, unless stated otherwise, we shall use S&P 500 calls and puts. There are two main reasons for this. First, these are the most liquid european options available on the CBOE. They expire on the third Friday of each contract month at the open. Second, abundant research has already been carried out on these options. Aït-Sahalia [6]; Bakshi, Cao, and Chen [20]; Bates [30]; Dumas, Fleming, and Whaley [88] and many others have all carried out their empirical analysis on S&P 500 options. 

The data quality is obviously dependent on the degree of liquidity. Another issue we need to take into account is that of synchronization between the spot close price and the option close price. Even if the timing of these two closings is off by a few minutes, the accuracy of the implied volatility can be affected. Bates [32] specifically mentions this issue. 

Let us be clear on the fact that this chapter does not constitute a thorough empirical study of the stock versus the options markets. It rather presents a set of examples of application of our inference tools constructed in the previous chapter. There clearly could be many other applications for these tools. As discussed in Chapter 2, model identification is another instance. 

## THE CONSISTENCY TEST

In this section we shall compare the values of $( \xi , \rho )$ in the results $\hat { \Psi } _ { o p t i o n s }$ to $\hat { \Psi } _ { s t o c k s }$ obtained via MLE. The time period [0 T ] is fixed, and the time interval $\Delta t$ for the stock is daily, as in Chapter 2. 

## The Setting

The test is based on SPX options as of 01/02/2002 expiring in approximately 1 year from the calibration date. The daily time series is taken during a period of 12 years corresponding to approximately 3000 points. The start of the period is 10 years before the calibration date and the end of the period is 1 year after the expiration of the options. Ideally we should only use the asset prices between the calibration date and the expiration to see whether the options predict the asset movements consistently. However, this would provide us with too few observation points. 

In what follows we will be considering one example of comparison between cross-sectional and time-series implied parameters. Many other similar examples were examined. They are not reported here because they do not change the conclusions. The original contribution of our approach is presenting a systematic way to evaluate time-series embedded parameters. We shall do this via the methodologies detailed in Chapter 2. 

## The Cross-Sectional Results

We consider one-year options as of January 2, 2002, for close-to-the-money options. The calibration is done via LSE Monte Carlo mixing as well as the Fourier inversion applied to the Heston model. We fix the instantaneous variance $\nu _ { 0 }$ at 0.04, and we take the index level at $S _ { 0 } = \$ 1154.67$ . As usual we take the appropriate interest-rate $r _ { T }$ and dividend-yield<sup>3</sup> q<sub>T</sub>, where T represents the options’ maturity. The dividend yield could, for instance, be the one implied from the forward contracts $F _ { T }$ calculated as 

$$
q _ {T} = r _ {T} - 1 / T \ln (F _ {T} / S _ {0})
$$

We use various strike-price sets $( K _ { j } )$ and determine the average optimal one-year parameters. Needless to say, the results are obtained under the risk-neutral measure. We obtain the risk-neutral implied parameter set in Table 3.1. which represents a rather high negative skewness and a high kurtosis.<sup>4</sup> The long-term volatility is $\sqrt { \omega / \theta } \approx 0 . 1 7$ . Needless to say, these parameter values vary everyday, but usually remain in the same range. 

## Robustness Issues for the Cross-Sectional Method

1. For the cross-sectional analysis, we have used a mixing Monte Carlo method. The Monte Carlo time steps of this method were spaced weekly. 


TABLE 3.1 Average Optimal Heston Parameter Set (Under the Risk-Neutral Distribution) Obtained via LSE Applied to One-Year SPX Options in January 2002. Various strike-price sets were used.


<table><tr><td>ω</td><td>θ</td><td>ξ</td><td>ρ</td></tr><tr><td>0.03620</td><td>1.1612</td><td>0.4202</td><td>-0.6735</td></tr></table>

Therefore, one natural question is how sensitive to this choice the results are. In order to verify this, we reran the simulations with daily Monte Carlo time steps and obtained 

$$
\begin{array}{r} \hat {\Psi} _ {o p t i o n s - d a i l y} = (\omega = 0. 0 3 6 8 4 6, \theta = 1. 1 6 9 7 0 9, \\ \xi = 0. 4 2 1 1 2, \rho = - 0. 6 7 4 5 8) \end{array}
$$

which is close to the original set. We also checked the results with the volatility-of-volatility series method, as well as the Fourier inversion method, and obtained comparable parameters. 

2. For our cross-sectional calibration, we used call bid prices. It is well known that calls and put prices are not always consistent. Indeed, as can be seen in Figure 3.1 the Put and Call implied-volatilities are slightly different, which seems to be a violation of put-call parity.<sup>5</sup> However, this difference is not large enough (the put and call bid–ask spreads actually overlap), and a profitable arbitrage cannot take place simply based upon this difference. This is why we consider the midpoint between puts and calls to be bids and asks. 


SPX Put and Call Implied Vols


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/9f6a8e0b3ff731e7d9220cf06b16935ebbcc72e6fff61a5267b2fd7460d92880.jpg)



FIGURE 3.1 Implied Volatilities of Close to ATM Puts and Calls as of 01/02/2002. Maturity is 2002/12/21 and index at 1154.67 USD’s. The bid–ask spread can clearly be observed.


Our implied volatility is therefore 

$$
\begin{array}{r c l} \sigma_ {i m p} & = & \frac {1}{4} \left[ \sigma_ {i m p} (C a l l _ {B i d}) + \sigma_ {i m p} (C a l l _ {A s k}) + \sigma_ {i m p} (P u t _ {B i d}) \right. \\ & & \left. + \sigma_ {i m p} (P u t _ {A s k}) \right] \end{array}
$$

Using these “mid” implied volatilities as opposed to the original call bids we obtain a parameter set 

$$
\begin{array}{c} \hat {\Psi} _ {o p t i o n s - m i d - c a l l - p u t} = (\omega = 0. 0 4 3 1 8 4, \\ \theta = 1. 1 7 3 1 1 9, \xi = 0. 4 0 2 5 8, \rho = - 0. 6 4 5 9 3) \end{array}
$$

3. If we do include $\nu _ { 0 }$ in the set of parameters $\Psi = ( \omega , \theta , \xi , \rho , \nu _ { 0 } )$ , then we obtain 

$$
\begin{array}{c} \hat {\Psi} _ {o p t i o n s - m i d - c a l l - p u t} = (\omega = 0. 0 4 3 2 2 4, \theta = 1. 1 4 4 9 5 7, \xi = 0. 4 8 2 0 0 9, \\ \rho = - 0. 6 6 1 4 2 7, \sqrt {\nu_ {0}} = 0. 2 2 4 6 5 9) \end{array}
$$

It is possible to see that the optimal $\sqrt { \hat { \nu } _ { 0 } }$ is around 0.20, which corresponds to our initial choice. 

4. As already mentioned, further-from-the-money options are less reliable in terms of pricing and liquidity. However, disregarding them decreases the cross-sectional sensitivity to the volatility-of-volatility parameter. 

Adding to the previous close-to-the-money strikes, additional furtherfrom-the-money ones, we find 

$$
\begin{array}{r l} \hat {\Psi} _ {o p t i o n s} = & (\omega = 0. 0 3 5 8 9 6, \theta = 1. 1 4 9 3 2 4, \xi = 0. 3 8 6 4 5 3, \\ \rho = & - 0. 6 5 9 3 1 9, \sqrt {\nu_ {0}} = 0. 2 2 1 9 8 8) \end{array}
$$

Again, the drift parameters are stable, and so is $\nu _ { 0 }$ . The question is, how are the volatility parameters affected? Interestingly, we do not observe a great difference from what we had with the previous sets. We therefore have a good degree of robustness. In any case, we use various sets of strike prices and take an average over the optimal parameter sets. 

5. One issue to consider in the cross-sectional method is how the riskneutral implied distribution or, in our case the parameter set - evolves over time. Needless to say, if the model was perfectly correct these parameters would never change; however, as we know, this is never the case. 

The question therefore becomes, how time-homogeneous are these parameters? Considering the same maturity 12/21/2002 but at a date closer to this maturity, we use close-to-the-money strikes. More accurately, we stand at 09/03/2002, take the spot at $878.02, and use the yield curve as of 09/03/2002. 

The strikes are 

$$
K _ {s e t} = \{7 7 5. 0 0, 8 0 0. 0 0, 8 2 5. 0 0, 8 5 0. 0 0, 8 7 5. 0 0,
$$

$$
\left. 9 0 0. 0 0, 9 2 5. 0 0, 9 5 0. 0 0, 9 7 5. 0 0 \right\}
$$

The optimization via Monte Carlo mixing provides 

$$
\hat {\Psi} _ {o p t i o n s} = (\omega = 0. 0 5 0 1 2 4 4, \theta = 1. 1 8 9 8 1 7, \xi = 0. 5 4 7 1 4 9,
$$

$$
\rho = - 0. 6 6 1 5 5 2, \sqrt {\nu_ {0}} = 0. 2 6 5 4 4 1)
$$

which is not too far from the other parameter sets. 

## Time-Series Results

As mentioned, the first idea is to choose a period corresponding to the life of the options considered in the previous section. In fact, we would like to see whether the options are predicting the underlying asset dynamics correctly during their life. However, this provides us with one year of daily data, or 252 points, which as we know from the previous chapter is highly insufficient for time-series estimators. In order to obtain more reliable results, we use various filters (EKF, EPF, etc.) and take the average optimal parameter set. For a period of 12 years ending on January 2004 (which includes the options’ life) and applying the filters studied in Chapter 2, we obtain the average results given in Table 3.2. 

The results in Table 3.2 show a lower $( \xi , \rho )$ and therefore a lower implied skewness and kurtosis—lower than the ones obtained from the options markets. 

Robustness Issues for the Time-Series Method Given the above results, it would be instructive to test the sensitivity of the observations to the drift parameters $( \omega , \theta )$ on the one hand, and to the volatility parameters $( \xi , \rho )$ on the other.<sup>6</sup> The point is that even if the state $\nu _ { k }$ itself is greatly affected by these volatility parameters, the impact of these parameters on the observations is small. However, the impact of the drift parameters is quite large. This could explain why the cross-sectional and time-series volatility-of-volatility parameters are not close. This point can be observed in the simulations represented in Figures 3.2 through 3.5. Note that this issue is related to the discussion in Chapter 2 on the sampling distribution. As previously stated, $\xi$ and $\rho$ have a lesser effect on the observations because they affect the “noise of the noise.” 


TABLE 3.2 Average Optimal Heston Parameter Set (Under the Statistical Distribution) Obtained via Filtered MLE Applied to SPX between January 1992 and January 2004. Various filters were used in the MLE.


<table><tr><td>ω</td><td>θ</td><td>ξ</td><td>ρ</td></tr><tr><td>0.018620</td><td>0.523947</td><td>0.096389</td><td>-0.132527</td></tr></table>


Sensitivity of Observations to Volatility Parameters


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/dc7902239d021dba7ec6622ef21c458f2f0378b7c8a74cd422f1884f98247cc9.jpg)



FIGURE 3.2 The Observations Have Little Sensitivity to the Volatility Parameters. One-year simulation with $\sqrt { \nu _ { 0 } } = 0 . 2 0 , \omega = 0 . 0 4 , \theta = 0 . 5$ . Cross-sectional uses $\xi = 0 . 0 3 6$ and $\rho = 0 . 5 0 \mathrm { ; }$ , whereas time series uses $\xi = 0 . 0 9$ and $\rho = - 0 . 8 0$ . This is consistent with what we had seen previously.


## Financial Interpretation

The current financial econometrics consensus is the following: No matter which case we consider, the cross-sectional parameters $\xi$ and $\rho$ are always greater (in absolute value) than the time-series ones. This means that the skewness and the kurtosis implied from options are stronger than those implied from the time series. As we will see in the following paragraphs, this could suggest a trade to take advantage of this inconsistency, supposing that 


Sensitivity of the State to Volatility Parameters


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/1f77dfda0914a1e64ea941f7d7eb2cba2fa7fe6baf01c96f329980fe468738e2.jpg)



FIGURE 3.3 The State Has a Great Deal of Sensitivity to the Volatility Parameters. One-year simulation with $\sqrt { \nu _ { 0 } } = 0 . 2 0 , \omega = 0 . 0 4 , \theta = 0 . 5 .$ . Cross-sectional uses $\xi = 0 . 0 3 6$ and $\rho = 0 . 5 0 \mathrm { _ { \it { i } } }$ , whereas time series uses $\xi = 0 . 0 9$ and $\rho = - 0 . 8 0$



Sensitivity of Observations to Drift Parameters


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/b23ef9f5030dfa05bc5dfb1ef3b9c4e63577b99738ec8f3bab0a6ab6cb92e7a4.jpg)



FIGURE 3.4 The Observations Have a Great Deal of Sensitivity to the Drift Parameters. One-year simulation with $\sqrt { \nu _ { 0 } } = 0 . 2 0 , \xi = 0 . 0 3 6 , \rho = 0 . 5 0 .$ . Cross-sectional uses $\omega = 0 . 0 4$ and $\theta = 0 . 5 0$ whereas time series uses $\omega = 0 . 0 8$ and $\theta = 5 . 0 .$


## Sensitivity of the State to Drift Parameters

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/ded590e8a2e96d682861f6a398722a1c2f07333689d9f77d2084c8771498be05.jpg)



FIGURE 3.5 The State Has a Great Deal of Sensitivity to the Drift Parameters. Oneyear simulation with $\sqrt { \nu _ { 0 } } = 0 . 2 0 , \xi = 0 . 0 3 6 , \rho = 0 . 5 0 ,$ . Cross-sectional uses $\omega = 0 . 0 4$ and $\theta = 0 . 5 0 \mathrm { { ; } }$ , whereas time series uses $\omega = 0 . 0 8$ and $\theta = 5 . 0 \AA$


the options are misjudging the spot movements. We can observe the above statement graphically by plotting the SPX volatility smile from the options market prices on the one hand, and from the time-series implied parameters on the other. Note that we need no calibration for the options because we are using the usual Black-Scholes implied volatility. Figure 3.6 shows the difference between the two slopes. Again, the options curve has a stronger (negative) slope, which is consistent with a stronger negative product $\xi \rho .$ 

As explained in [69], the higher moments of the stock-price return can be calculated from the stochastic-volatility model parameters. Indeed, for a given parameter set $\Psi = ( \omega , \theta , \xi , \rho )$ , we have 

$$
s k e w n e s s = \left(\frac {3 \xi \rho e ^ {\frac {1}{2} \theta T}}{\sqrt {\theta}}\right) \left[ \frac {\frac {\omega}{\theta} (2 - 2 e ^ {\theta T} + \theta T + \theta T e ^ {\theta T}) - \nu_ {0} (1 + \theta T - e ^ {\theta T})}{\left(\frac {\omega}{\theta} [ (1 - \theta T + \theta T e ^ {\theta T}) + \nu_ {0} (e ^ {\theta T} - 1) ]\right) ^ {\frac {3}{2}}} \right]
$$

and 

$$
k u r t o s i s = 3 \left[ 1 + \xi^ {2} \left(\frac {\frac {\omega}{\theta} A _ {1} - \nu_ {0} A _ {2}}{B}\right) \right]
$$

Options Implied versus Historic Volatility Smile for SPX as of 01/02/2002 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/14e2bce08dadbc2f90b8773a31b910d597c0385438d4d183aeecda98bac905c8.jpg)



FIGURE 3.6 Comparing SPX Cross-Sectional and Time-Series Volatility Smiles (with Historic $\xi$ and $\rho )$ as of January 2, 2002. The spot is at $1154.67.


with $y = \theta T$ and 

$$
\begin{array}{r l} A _ {1} & = \left[ 1 + 4 e ^ {y} - 5 e ^ {2 y} + 4 y e ^ {y} + 2 y e ^ {2 y} \right] + 4 \rho^ {2} \\ & \left[ 6 e ^ {y} - 6 e ^ {2 y} + 4 y e ^ {y} + 2 y e ^ {2 y} + y ^ {2} e ^ {y} \right] \\ A _ {2} & = 2 \left[ 1 - e ^ {2 y} + 2 y e ^ {y} \right] + 8 \rho^ {2} \left[ 2 e ^ {y} - 2 e ^ {2 y} + 2 y e ^ {y} + y ^ {2} e ^ {y} \right] \\ B & = 2 \theta \left[ \frac {\omega}{\theta} (1 - e ^ {y} + y e ^ {y}) + v _ {0} (e ^ {y} - 1) \right] ^ {2} \end{array}
$$

Without entering into the details of the calculations, we can see that for given $\omega$ and $\theta ,$ higher $( \xi , | \rho | )$ correspond to higher skewness and kurtosis. As we said in the previous chapter, the skewness depends on $\omega , \theta$ and the product $\xi \rho ,$ which has a more reliable estimation than the separate values of $\xi$ and $\rho .$ This makes the estimation of the skewness more trustworthy. 

## THE PESO THEORY

## Background

As [6] mentions, one possibility regarding the cross-sectional versus timeseries observed differences is the following. As we know, the time series corresponds to one realization of the stock-return stochastic process. Now supposing that the true stock stochastic differential equation (SDE) contains jumps, there is a possibility that the historic path we are observing does not contain any of these jumps.<sup>7</sup> This is referred to as the peso theory. As mentioned in [12], this term goes back to Milton Friedman in his analysis of Mexican peso during the early 1970s. The Mexican interest rates remained significantly above the U.S. interest rates, although the peso was pegged at 0.08 dollar per peso. Friedman argued that the interest rates reflected an expectation about a future devaluation of the peso. In August 1976, the peso was devaluated by 37.5% to a new rate of 0.05 dollar per peso, thus validating the previous interest rate differential. 

This assumption seems reasonable because, as we saw in the previous tests, the cross-sectional method usually provides higher volatility parameters $( \xi , \rho )$ and therefore higher skewness (in absolute value) and kurtosis. Introducing a jump component in the options pricing model should lower these optimal parameters. 

Note that in [3], Aït-Sahalia tries to find out whether the discrete observations of S&P 500 come from a diffusion, or from a distribution containing jumps. He derives a criterion for continuity of the paths 

$$
\frac {\partial^ {2}}{\partial x \partial y} \ln (p (\Delta t, y = X _ {t + \Delta t} | x = X _ {t})) > 0
$$

for every $\Delta t > 0$ and given $( x , y )$ . Based on the implied cross-sectional distribution, he finds that S&P 500 options do consider jumps in the paths. 

Using the jump diffusion model, as we did in Chapter 2 

$$
\begin{array}{c} d \ln S _ {t} = \left(\mu_ {S} - \frac {1}{2} \nu_ {t} + \lambda j\right) d t + \sqrt {\nu_ {t}} d B _ {t} + \ln (1 - j) d N _ {t} \\ d \nu_ {t} = (\omega - \theta \nu_ {t}) d t + \xi \sqrt {\nu_ {t}} d Z _ {t} \end{array}
$$

we may very well see no difference introduced from the parameters $( \lambda , j )$ for the time series and we can even disregard them. However, this does not mean that the stock process does not contain jumps but rather that this specific path happens to contain none. 

The options, by contrast, always include the possibility of jumps in their pricing. Adding $( \lambda , j )$ will affect the resulting $( \xi , \rho )$ from the cross-sectional method. 

## Numeric Results

We use the same options and time series as in the previous section. As shown in Merton’s paper [190], we have for a given volatility path $\sigma = \sqrt \nu$ 

$$
\text { Call } = \sum_ {n = 0} ^ {+ \infty} e ^ {- \lambda (1 - j) T} \frac {(\lambda (1 - j) T) ^ {n}}{n !} C _ {B S} (S, K, T, \sigma , r _ {n})
$$

with 

$$
r _ {n} = r + \lambda j + \frac {n}{T} \ln (1 - j)
$$

We then take the expectation upon the volatility stochastic process as we usually do in a mixing algorithm.<sup>8</sup> 

We find for the parameter set $\hat { \Psi } = ( \omega , \theta , \xi , \rho , \lambda , j )$ the values 

$$
\begin{array}{r l} \hat {\Psi} _ {o p t i o n s} = & (\omega , \theta , \xi , \rho , \sqrt {\nu_ {0}}, \lambda , j) = (0. 0 3 2 6 4 8, 1. 1 6 5 5 9 8, 0. 3 6 0 6 4 6, \\ & - 0. 5 8 5 3 0 2, 0. 2 1 8 3 3 3, 0. 0 0 8 9 8 2, 0. 9 1 3 7 7 2) \end{array}
$$

instead of the previous pure-diffusion parameter set 

$$
\begin{array}{c} \hat {\Psi} _ {o p t i o n s - m i d - c a l l - p u t} = (\omega = 0. 0 4 3 2 2 4, \theta = 1. 1 4 4 9 5 7, \xi = 0. 4 8 2 0 0 9, \\ \rho = - 0. 6 6 1 4 2 7, \sqrt {\nu_ {0}} = 0. 2 2 4 6 5 9) \end{array}
$$

As we see even with the addition of jump parameters $( \lambda , j )$ , the cross-sectional volatility parameters $( \xi , \rho )$ remain significantly above the time-series parameters. This is in agreement with the findings of Bakshi, Cao, and Chen [20]. We have a small λ and a j close to one. This means that options are expecting a large but infrequent jump; that is, they are factoring in the possibility of a crash. 

## TRADING STRATEGIES

Supposing that the model we are dealing with is correct, and if the options are mistaken in evaluating the stock distribution during their lifetime, there should be an arbitrage opportunity to take advantage of. The ninth chapter of the Härdle et al. book [128] has a description of these strategies. Note that both these strategies are European and cannot be changed<sup>9</sup> until maturity. 

At this point we should reiterate that the profit and loss of this trade could be used as an empirical and model-free measure of how consistent or inconsistent the information embedded in the options is with the one in the underlying stocks. 

## Skewness Trades

To capture an undervalued third moment, we can buy OTM calls and sell OTM puts. Note that Aït-Sahalia [6] says that the options are overly skewed, which means that the options skew is larger in absolute value. However, given the negative sign of the skew, the cross-sectional skew is actually lower than the one implied by the time series, hence the described strategy. 

Note that in order to be immune to parallel shifts of the volatility curve, we should make the trade as vega-neutral as possible. The correspondence between the call and the put is usually not one-to-one. Therefore, calling the vega, ’s the hedge ratios for C the call and P the put option, then the hedged portfolio  will be 

$$
\Pi = C (S _ {t}, K _ {C}) - \frac {\mathcal {V} _ {C}}{\mathcal {V} _ {P}} P (S _ {t}, K _ {P}) - \left(\Delta_ {C} - \frac {\mathcal {V} _ {C}}{\mathcal {V} _ {P}} \Delta_ {P}\right) S _ {t}
$$

and the positions in the options should be dynamically adjusted in theory. However, that would cause too much transaction cost and exposure to the bid-ask spread. 

As we shall see in the paragraph on “exact replication,” more-elaborate strategies are available to better exploit the third-moment differences. 

## Kurtosis Trades

To capture an overvalued fourth moment, we need to use the “fat tails” of the distribution. For this we can, for instance, sell ATM and far OTM options, and buy close OTM options. 

## Directional Risks

Despite the delta-hedging, the skewness trade applied to an undervalued third moment has an exposure to the direction of the markets. A bullish market is favorable to it, and a bearish one unfavorable. The kurtosis trade applied to an overvalued fourth moment generates a profit if the market stays at one point and moves sideways but loses money if there are large movements. 


Skewness Trading Strategy Pay-Off


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/ebff1ec10b4b813fe19db4cb0a56d8718e853656595dbd840f99e597a5904435.jpg)



FIGURE 3.7 A Generic Example of a Skewness Strategy to Take Advantage of the Undervaluation of the Skew by Options. This strategy could be improved upon by trading additional OTM puts and calls.


This exposure to market conditions is consistent with the peso theory. The skewness and kurtosis trading strategies above are profitable given the options’ implied moments, unless the options were actually right in factoring in a large and sudden downward movement. This also makes sense because the way the options were priced changed only after the crash of 1987. Prior to that, the volatility negative skew was practically absent altogether. Figures 3.7 and 3.8 show generic examples of the strategies described above. 

Note that as the skew formula in [69] shows, the volatility-of-volatility ξ affects the skew as much as the correlation ρ does. This explains why sudden upward movements can hurt us as well. If the overall correlation is negative but there are large movements in both directions, we will have large third (in absolute value) and fourth moments, which would make the options expectations correct. In fact, as we will see in the following example, a large upward movement can make us lose on our hedge account. 

As many, such as [32] and [128], have mentioned, it is possible to interpret this trade as an insurance selling strategy. The trade will generate moderate and consistent profits if no crash happens. But if the crash does happen we could suffer a large loss. 

Skewness vs. Kurtosis The skewness trade seems to be a simpler one and has a better chance to be realized. Indeed, in order to have a large negative skew, we need a large volatility-of-volatility $\xi$ (as we do for the kurtosis trade) and a large negative correlation $\rho .$ . In other words, if for a given stock time series we have a large volatility-of-volatility but a weak correlation, we will not have a kurtosis trade opportunity but we will have a skewness trade opportunity. The historic skew will be small and the historic kurtosis high. Graphically, we could have the following interpretation. For these assets, the historic distribution does have fat tails, but remains symmetric, whereas the implied distribution has a fatter left tail. This is why we have a skewness trade opportunity, even if we do not have a kurtosis trade opportunity. Finally, as we previously mentioned, the estimation of the skewness from a time series is more reliable because it depends only on the product of the volatilityof-volatility and the correlation. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/7799fb0868cd619bc8b5d71df70dc6c5def2ee72c6cbc3a466b57a7dd48727d9.jpg)



FIGURE 3.8 A Generic Example of a Kurtosis Strategy to Take Advantage of the Overvaluation of the Kurtosis by Options. This strategy could be improved upon by trading additional puts and calls.


## An Exact Replication

These trading strategies can be refined using a Carr-Madan replication. As explained in [50], we have for any payoff function $f ( )$ the following identity 

$$
\begin{array}{r l} \mathbf {E} [ f (S _ {T}) ] = & f (F) + e ^ {r T} \int_ {0} ^ {F} f ^ {\prime \prime} (K) P (S _ {0}, K, t = 0, T) d K \\ & + e ^ {r T} \int_ {F} ^ {+ \infty} f ^ {\prime \prime} (K) C (S _ {0}, K, t = 0, T) d K \end{array}
$$

with $F = S _ { 0 } e ^ { r T }$ the forward price. 

In order to get the Das [69] skew and kurtosis calculations, we need to take for the $n ^ { t h }$ moment 

$$
f (S _ {T}) = (Z _ {T} - \mathbf {E} (Z _ {T})) ^ {n}
$$

with 

$$
Z _ {T} = \ln (S _ {T} / S _ {0})
$$

However, this trade will clearly have a much higher transaction cost than the one described in the previous paragraph. 

## The Mirror Trades

Should we see the opposite conditions in the market, that is, having the skew (in absolute value) or kurtosis undervalued by the options given a historic path, we could obviously put on the mirror trades. The inverse of the peso theory would be as follows. The stock in question has already had a crash and the options are supposing there probably will not be another one in the near future. Setting up the overvalued kurtosis trade in the previous paragraph, we picked up a premium and made an immediate profit and hoped that there would not be a sudden movement. Here we start by losing money and hope a crash will happen within the life of the option so that we can generate a profit. Because jumps and crashes are rare by nature, this trade does not seem very attractive. Moreover, if there was a recent crash, the possibility of another one is indeed reduced and we should believe the options prediction. However, these mirror trades could be considered as buying insurance and therefore as a protection against a possible crash. 

## An Example of the Skewness Trade

The algorithm is as follows. For a given date $t _ { 0 }$ we have $S _ { 0 }$ and choose the closest maturity to $T = t _ { 0 } + 0 . 2 5$ in order to have a three-month trade, we then take the call and put strikes $K _ { \mathrm { C } }$ and $K _ { P }$ as the closest ones to $1 . 1 0 S _ { 0 }$ and $0 . 9 0 S _ { 0 }$ , respectively. 

The original cost is therefore 

$$
o p t i o n s (0) = C a l l _ {A s k} (S _ {0}, K _ {C}, t _ {0}, T) - P u t _ {B i d} (S _ {0}, K _ {P}, t _ {0}, T)
$$

Note that we buy a call at the offer price and sell the put at the market bid price. At maturity, the position is worth 

$$
o p t i o n s (T) = M A X (0, S _ {T} - K _ {C}) - M A X (0, K _ {P} - S _ {T})
$$

During the trade, we have a delta-hedging cash flow of 

$$
h e d g e = - \sum_ {t = 0} ^ {T - 1} \Delta (S _ {t}, t, T) (S _ {t + 1} - S _ {t})
$$

with 

$$
\Delta (S _ {t}, t, T) = \Delta_ {\text { Call }} (S _ {t}, K _ {C}, t, T, \sigma_ {i m p} (t _ {0}, K _ {C})) - \Delta_ {P u t} (S _ {t}, K _ {P}, t, T, \sigma_ {i m p} (t _ {0}, K _ {P}))
$$

where the implied volatilities used in the hedge ratios are using the mid prices (between bid and ask prices). The interest-rate cash flow is 

$$
i n t e r e s t = \sum_ {t = 0} ^ {T - 1} \Delta (S _ {t}, t, T) (e ^ {r _ {t} \Delta t} - 1) S _ {t}
$$

Our final profit or loss (PnL) is therefore 

$$
P n L = o p t i o n s (T) - o p t i o n s (0) + h e d g e + i n t e r e s t
$$

If the options’ implied skew is indeed higher than justified by the stock movements, then this trade should be profitable. However, in case of a sudden large movement, this will not be true anymore. 

We consider the case of the S&P 500 between 04/04/2002 and 06/22/2002. At that point in time, $S _ { 0 } = \mathbb { S } 1 1 2 6 . 3 4$ , which means we can take $K _ { \mathrm { C } } = \$ 1250$ and $K _ { P } = \$ 1050$ . We also have $C a l l _ { A s k } ( t _ { 0 } , K = 1 2 5 0 ) = \ S 3 . 2 0$ and $P u t _ { B i d } ( t _ { 0 } , K = 1 0 5 0 ) = \ S 1 4 . 2 0$ , as well as the mid implied volatilities of $\sigma _ { i m p } ( K _ { \mathrm { C } } ) = 0 . 1 5 4$ and $\sigma _ { i m p } ( K _ { P } ) = 0 . 2 1 4$ 

As can be seen in Figures 3.9 and 3.10, the sudden spot movements generate most of the loss (for instance, around day 50). We have at the end of the trade 

$$
\begin{array}{c} S _ {T} = 9 8 9. 1 4 \\ h e d g e = 5 0. 3 9 \\ i n t e r e s t = 1. 3 2 \end{array}
$$

Therefore, the final PnL (in dollars) is 

$$
P n L = [ 0 - (1 0 5 0 - 9 8 9. 1 4) ] + (1 4. 2 0 - 3. 2 0) + 5 0. 3 9 + 1. 3 2 = 1. 8 5
$$

As we can see, we hardly generated a profit, given the “jumps” occurring in the middle of the trade. 

Note that we generated a profit in the beginning by selling an OTM put that was more expensive than the OTM call we bought. We lost a large amount because the spot ended below the put strike. However, we compensated that via the hedge. 


FIGURE 3.9 Historic Spot Level Movements During the Trade Period. Hedge PnL During the Trade



SPX Movements During the Trade


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/7224850bb77d1e4de9d7457fb6adf402158828d63f3f34c4797428519d8a7c13.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/9f53d2b59b7b97dfca0365410ec833489d0b968d54048723bd5920d37e72288a.jpg)



FIGURE 3.10 Hedging PnL Generated During the Trade Period. As we can see, losses occur upon jumps.


The Options Bid–Ask Spread It is important to know where we are buying the call and selling the put on the start date. Are we buying the call at the offer price and selling the put at the bid price? If so, we can lose the bid–ask spread, as compared to the case in which we would buy and sell both options at the mid market. This spread averages approximately $1 for 10% OTM SPX options. 


Cumulative Hedge PnL


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/e99189e2e1e1cbe696dd139116305cc0aceb396b72ba56100fee221f5c15fb16.jpg)



FIGURE 3.11 Cumulative Hedging PnL Generated During the Trade Period. This positive PnL will be offset by the option premiums and payoffs.


Early Termination We also should consider an early unwinding of the trade. Indeed as we get closer to maturity, our hedge-ratio might be close to one, which will make our hedge account extremely sensitive to adverse stock movements. In order to have a smoother PnL, we can buy back the put and sell the call at a date (e.g. one month) prior to maturity. Again, it is important to know whether we are unwinding the trade by selling the call at the bid and buying back the put at the offer. If so, we will have suffered from the bid–ask spread twice: once on the start date and once on the unwinding (termination) date. 

This is not just a small detail, indeed having the right execution (at midmarket) can change the average sign of the PnL altogether. Furthermore, regardless of the bid–ask spread, we are subject to the movements of the options prices. By contrast, if we hold the positions until expiration, we will have a pure strategy between the original options prices and the spot price movements. 

Implied Volatility Term Structure Yet another issue to take into account is that, in our back-testing, we used fixed implied volatilities in order to calculate the hedge ratios during the life of the trade. In reality, the implied volatilities change every day even if we assume a sticky strike regime, in which the stock price will not affect the implied volatility level. Even if our strikes are fixed, the time-to-maturities of the options decreases, and this will make the implied volatilities vary. For S&P 500 the term structure of implied volatility is upward-sloping, which means that theoretically all implied volatilities should come down from their original levels at the unwinding date. 


Options Implied versus Historic Volatility Smile for MMM as of 03/28/2003


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/efe6a6df4e774ed273ae99bb8bb808a37c8ac8485c98225faf0399e9a79ee356.jpg)



FIGURE 3.12 A Strong Option-Implied Skew: Comparing MMM (3M Co) Cross-Sectional and Time-Series Volatility Smiles as of March 28, 2003. The spot is at $131.66.



Options Implied versus Historic Volatility Smile for CUM as of 03/28/2003


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/0b180a8b6279638b6e3fbbeb0410a3788a8428bc5edf8050e47d52289502cce3.jpg)



FIGURE 3.13 A Weak Option-Implied Skew: Comparing CMI (Cummins Inc) Cross-Sectional and Time-Series Volatility Smiles as of March 28, 2003. The spot is at $24.59.


Which Hedge Ratio should we use? In the hedging of our skew portfolio, which  should we apply? In other words, we ask which implied volatility should we use in the usual 

$$
e ^ {- q (T - t)} N (d _ {1} (S _ {t}, K, t, T, \sigma_ {i m p}))
$$

If we believe that the volatility predicted by the options is wrong and the historic levels are correct, we should then use 

$$
\sigma_ {s t o c k s} ^ {i m p} (K, T) = C _ {B S} ^ {- 1} \left(C _ {m o d e l} (S _ {0}, t _ {0}, K, T, \hat {\Psi} _ {s t o c k s})\right)
$$

where 

$$
\hat {\Psi} _ {s t o c k s} = (\hat {\omega} _ {o p t s}, \hat {\theta} _ {o p t s}, \hat {\xi} _ {s t o c k s}, \hat {\rho} _ {s t o c k s})
$$

Note that this might give us a mismatch in terms of mark-to-market with the existing option levels in the market. However, if the time series is actually correct, the skew should eventually collapse before the options mature.<sup>10</sup> We should note, however, that using the options’ implied volatilities makes better practical sense because those are the ones at which the options are actually traded. 

## Multiple Trades

The next natural step would be to repeat the previous trade in order to see whether the trade would be statistically profitable. We use SPX puts and calls between 01/02/2002 and 02/01/2003 on the expiration month such that the original life of the trade is around three months. We systematically unwind the trades around 20 business days to expiration. Once again, we buy 10% OTM calls and we sell 10% OTM puts. 

We cover in this manner forty different cases. We calculate the PnL’s as previously described and take their average. 

The results are mixed: Ifwe put the trade on and unwind at the bid and ask levels, we will actually suffer a loss. However, if we can execute at the mid, then we will generate a profit. 

This shows a lack of decisive proof on an inconsistency between the options and stock markets.<sup>11</sup> Indeed we have used the PnL of this trade as a measure of discrepancy.<sup>12</sup> 

## High Volatility-of-Volatility and High Correlation

As previously discussed, many stocks do have a high historic volatility-ofvolatility $\xi ;$ however, given a weak (or even positive) spot-volatility correlation $\rho ,$ the historic skew is still very low. This is especially true of “penny” stocks. Indeed, when these stocks increase in price, in some sense they “come back to life” and therefore become more volatile. This means that the historic skew is actually positive, which seems to indicate an even stronger case for a skewness trade. However, given that we are dealing with penny stocks, the possibility of a crash for these stocks is high, and that is precisely what causes the negative option–implied skew! The stock GW (Grey Wolf Inc.) in Figure 3.14 is a good example for this case. This presents a trading opportunity as shown in Figure 3.15. By contrast, there are cases, such as MSFT (Microsoft), where we do have a strong historic negative correlation as well as a high volatility-of-volatility. As the stock price goes down, the asset becomes riskier and therefore more volatile. We can see this in Figure 3.16. This justifies the option-implied skew observable in Figure 3.17 and means that there is no trade opportunity. The safest trade therefore seems to be an index skewness trade, given that the likelihood of a crash is lower thanks to the diversification effect. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/2877a6056bdcb2b656f943dd4ebe886358ee1d4ace421c00d60fe18585198103.jpg)



FIGURE 3.14 GW (Grey Wolf Inc.) Historic Prices (03/31/2002–03/31/2003) Show a High Volatility-of-Volatility But a Weak Stock-Volatility Correlation. The resulting negative skew is low.



Options Implied versus Historic Volatility Smile for GW as of 03/31/2003


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/252b74f881d0a3dec7814166b49a94034296e424c768012d30e10c61648e85d1.jpg)



FIGURE 3.15 The Historic GW (Grey Wolf Inc.) Skew Is Low and Not in Agreement with the Options Prices. There is a skew trading opportunity here.



Historic Spot Prices for MSFT


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/80e889869bb598e7d6ff6e207ded7037c6339b9e2e95bfbb7151898192efaff9.jpg)



FIGURE 3.16 MSFT (Microsoft) Historic Prices (03/31/2002–03/31/2003) Show a High Volatility-of-Volatility and a Strong Negative Stock-Volatility Correlation. The resulting negative skew is high.



Options Implied versus Historic Volatility Smile for MSFT as of 03/31/2003


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/e59a8e57bcddfab4bc9781f7de73e03d73134ec1a760c99ff59fe8a517005a43.jpg)



FIGURE 3.17 The Historic MSFT (Microsoft) Skew Is High and in Agreement with the Options Prices. There is no skew trading opportunity here.



Historic Spot Prices for NDX


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/e542cac85e1354da292ac75c9d5df8d25f57ae2340655e52d5cb8068a7adc542.jpg)



FIGURE 3.18 NDX (Nasdaq) Historic Prices (03/31/2002–03/31/2003) Show a High Volatility-of-Volatility and a Strong Negative Stock-Volatility Correlation. The resulting negative skew is high.


Note that the strong negative historic skew is not limited to individual stocks. Taking the case of the NDX index in Figures 3.18 and 3.19, we can see that there is no trading opportunity available and the historic skewness is in line with the one implied by the options prices. 

Therefore we have two possible reasons<sup>13</sup> why a skewness trade opportunity may exist. 

1. Weak historic volatility-of-volatility (e.g., SPX [S&P 500]) 

2. Weak Historic Correlation (e.g., GW [Grey Wolf Inc.]) 

If neither of the above is verified (e.g., NDX [Nasdaq] or MSFT [Microsoft]), there is no skew trading opportunity. 

The graphical interpretation seen in Figures 3.12 through 3.19 is based on the comparison of the observable options-implied skew 

$$
\sigma_ {o p t i o n s} ^ {i m p} (K, T) = C _ {B S} ^ {- 1} (C _ {m k t} (S _ {0}, t _ {0}, K, T))
$$

and the skew implied from historic stock-price movements 

$$
\sigma_ {s t o c k s} ^ {i m p} (K, T) = C _ {B S} ^ {- 1} \left(C _ {m o d e l} (S _ {0}, t _ {0}, K, T, \hat {\Psi} _ {s t o c k s})\right)
$$

Options Implied versus Historic Volatility Smile for NDX as of 03/31/2003 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/044e9af4a5230cbb25fe42ced026877f14edf0669c8f48b3ff76eea46229ce78.jpg)



FIGURE 3.19 The Historic NDX (Nasdaq) Skew is High and in Agreement with the Options Prices. There is no skew trading opportunity here.


where $C _ { B S }$ corresponds the usual Black-Scholes pricing function. 

Again we use the option-implied volatility-drift parameters $\hat { \omega } _ { o p t i o n s } ,$ $\widehat { \theta } _ { o p t i o n s }$ in $\hat { \Psi } _ { s t o c k s } .$ The only assumption here would be that of diffusion in the processes. Then, according to the Girsanov theorem, the volatilityof-volatility and the correlation should be the same for the continuous statistical and risk-neutral processes. 

## NON-GAUSSIAN CASE

As previously discussed, once we start dealing with some of the pure-jump models, such as VGG, we will no longer have the Girsanov theorem and cannot compare the parameters directly. However, no matter what the arrival process is, we still have the VG parameters $( \sigma , \nu , \theta )$ as in 

$$
d \ln S _ {t} = (\mu_ {S} + \omega) d t + X (d t; \sigma , \nu , \theta)
$$

where, as before, $\mu _ { S }$ is the real-world statistical drift of the stock log-return and $\begin{array} { r } { \omega = \frac { 1 } { \nu } \ln ( 1 - \theta \nu - \sigma ^ { 2 } \nu / 2 ) } \end{array}$ . As for $X ( d t ; \sigma , \nu , \theta )$ , it has the following meaning 

$$
X (d t; \sigma , \nu , \theta) = B (\gamma (d t, 1, \nu); \theta , \sigma)
$$

where $B ( d t ; \theta , \sigma )$ would be a Brownian motion with drift θ and volatility $\sigma .$ In other words 

$$
B (d t; \theta , \sigma) = \theta d t + \sigma \sqrt {d t} N (0, 1)
$$

where $N ( 0 , 1 )$ is a standard Gaussian realization. 

Further, we know what the centralized third and fourth moments (skewness and kurtosis) are 

$$
\begin{array}{r l} & s k e w n e s s = \left(2 \theta^ {3} \nu^ {2} + 3 \sigma^ {2} \theta \nu\right) t \\ & k u r t o s i s = \left(3 \sigma^ {4} \nu + 1 2 \sigma^ {2} \theta^ {2} \nu^ {2} + 6 \theta^ {4} \nu^ {3}\right) t + \left(3 \sigma^ {4} + 6 \sigma^ {2} \theta^ {2} \nu + 3 \theta^ {4} \nu^ {2}\right) t ^ {2} \end{array}
$$

We therefore can always compare the skewness and kurtosis implied from time series with those implied from options. However, a mismatch between the two does not indicate an arbitrage opportunity because once again we are comparing them under two different measures. Having said this, the determination of the statistical density $p ( \ u )$ and the risk-neutral density $q ( \ u )$ is still useful in the sense that it could allow us to determine the optimal position we would take in the derivatives market given a utility function, as described in [52] and [53]. 

Indeed, having an increasing concave utility function $U ( ) ,$ the idea is to find the optimal payoff $\phi ( S )$ , maximizing the expected utility at a given horizon $T$ , and among all possible payoffs $f ( S )$ 

$$
\phi = \operatorname{argmax} \int_ {0} ^ {+ \infty} U [ f (S _ {T}) ] p (S _ {T}) d S _ {T}
$$

In addition to this, we have the initial budget $W _ { 0 } .$ , which imposes a constraint: The discounted risk-neutral expected value of the payoff cannot be greater than this initial budget. 

$$
\exp (- r T) \int_ {0} ^ {+ \infty} f (S _ {T}) q (S _ {T}) d S _ {T} \leq W _ {0}
$$

This can be seen by using a “self-financing” portfolio argument, as was done by Black and Scholes. Using the two foregoing equations, we can write the Lagrangian 

$$
\mathcal {L} (f) = \int_ {0} ^ {+ \infty} U [ f (S _ {T}) ] p (S _ {T}) d S _ {T} - \lambda \exp (- r T) \int_ {0} ^ {+ \infty} f (S _ {T}) q (S _ {T}) d S _ {T}
$$

where λ is the Lagrange multiplier. We then can differentiate with respect to the payoff $f ( )$ and obtain the optimal payoff satisfying 

$$
\exp (r T) \frac {p (S)}{q (S)} U ^ {\prime} [ \phi (S) ] = \lambda
$$

or equivalently 

$$
\phi (S) = \left(U ^ {\prime}\right) ^ {- 1} \left(\lambda \exp (- r T) \frac {q (S)}{p (S)}\right)
$$

and the constant λ could be determined by a normalization, such as 

$$
\exp (- r T) \int_ {0} ^ {+ \infty} (U ^ {\prime}) ^ {- 1} \left(\lambda \exp (- r T) \frac {q (S)}{p (S)}\right) q (S _ {T}) d S _ {T} = W _ {0}
$$

This would provide us with the optimal payoff function that we would need to choose in the derivatives market, and therefore motivates the estimation of the statistical and risk-neutral densities $\boldsymbol { p }$ and q even for the non-Gaussian case. 

## VGSA

Unlike VGG and many other pure-jump models, VGSA has a conditionally Gaussian arrival rate. This means that the volatility of the arrival-rate λ should remain the same under the statistical and risk-neutral measures. We therefore do have an approach that is analogous to the diffusion-based models for VGSA. 

VGSA vs. VG In their original paper [182], Carr, Madan, and Chang found comparable results for the VG model applied to the S&P 500 for the period 1992–1994. As previously discussed, the VG model has an integrated density, and therefore the MLE could be performed without any filtering. The statistical (historical) parameters are 

$$
(\sigma = 0. 1 1 7 2 0 0, \theta = 0. 0 0 5 6, \nu = 0. 0 0 2)
$$

And their risk-neutral parameters are 

$$
(\sigma = 0. 1 2 1 3, \theta = - 0. 1 4 3 6, \nu = 0. 1 6 8 6)
$$

Again we can see that the historical estimate for θ is close to zero, whereas the risk-neutral one is significantly negative. This negative θ is what creates the negative skewness observed in cross-sectional estimations. 

We can try to reproduce the foregoing parameters with the VGSA model. The resulting time-series parameter set is 

$$
(\kappa = 7 9. 4 9 9 6 8 7, \eta = 3. 5 5 7 7 0 2, \lambda = 0. 0 0 0 0 0 0)
$$

$$
(\sigma = 0. 0 4 9 6 5 6, \theta = 0. 0 0 6 8 0 1, \nu = 0. 0 0 8 6 6 0, \mu = 0. 0 3 0 6 9 9)
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/ca81f6b7ef4d8e0a4541b3fcfed650af258d1109ef2c87fa975d6bc33e5a1807.jpg)



FIGURE 3.20 Arrival Rates for Simulated SPX Prices Using $\Psi = ( \kappa = 0 . 0 0 0 0$ $\eta = 0 . 0 0 0 0 ,$  λ 0.000000 σ 0.117200 θ 0.0056 ν 0.002) and $\Psi = ( \kappa =$ 79.499687, η 3.557702 λ 0.000000 σ 0.049656 θ 0.006801, $\nu =$ 0.008660, $\mu = 0 . 0 3 0 6 9 9 )$ . We can see that they are quite different.


Although the results seem to be very different, upon simulation we can see that even if the resulting arrival rates and gamma variables are different, the log stock prices are close. This can be seen in Figures 3.20, 3.21, and 3.22. 

An alternative would be to use the EPF algorithm with the VGSA model over the same period, in which case we would obtain 

$$
(\kappa = 1 9 0. 4 0 9 7 2 1, \eta = 3. 4 5 9 2 8 8, \lambda = 5. 4 3 0 7 5 9)
$$

$$
(\sigma = 0. 0 5 0 2 4 3, \theta = 0. 0 0 2 3 6 6, \nu = 0. 0 0 7 9 4 5, \mu = 0. 0 3 2 5 7 6)
$$

Once again the most unstable parameters are $( \kappa , \eta , \lambda )$ , or the ones corresponding to the arrival rate. We have seen this many times; the estimation of the parameters affecting the noise is less reliable. This is in agreement with what we had observed in Chapter 2 and shows the limitations of these inference tools. 

Cross-Sectional vs. Time-Series VGSA Applying the particle filtering algorithm described in Chapter 2 to S&P 500, we find for 2001–2003 period the statistical parameter set 

$$
(\kappa = 5 5. 0 1 7 7 8, \eta = 3. 7 2 1 5 8 3, \lambda = 8. 6 6 6 7 1 7,
$$

$$
\sigma = 0. 1 1 8 6 3 7, \theta = 0. 0 6 0 0 5 3, \nu = 0. 0 0 1 0 3)
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/19a01991d6fe9e742ef276520c4e2488fe24db9feee09910c1637f0fa61dcbd6.jpg)



FIGURE 3.21 Gamma Times for Simulated SPX Prices Using $\Psi = ( \kappa = 0 . 0 0 0 0$ ， η 0.0000 λ 0.000000 σ 0.117200 θ 0.0056 ν 0.002) and - (κ 79.499687 η 3.557702 λ 0.000000 σ 0.049656 θ 0.006801 ν 0.008660, µ 0.030699).


$$
\mu_ {S} = - 0. 2 9 1 0
$$

and for the 1995–1999 period 

$$
\begin{array}{c} (\kappa = 1. 1 5 1 9 5 2, \eta = 5. 4 1 8 2 2 6, \lambda = 2. 8 4 0 4 6 1, \sigma = 0. 0 5 5 8 1 1, \\ \theta = 0. 0 0 8 6 2 6, \nu = 0. 0 0 6 0 2 1) \\ \mu_ {S} = 0. 2 4 9 0 5 1 \end{array}
$$

A typical cross-sectional risk-neutral parameter set 

$$
(\kappa = 2. 7 2, \eta = 2. 1 8, \lambda = 5. 6 8, \sigma = 0. 2 1, \theta = - 0. 4 1, \nu = 0. 0 6)
$$

As we can see, the implied skew and kurtosis are stronger for the crosssectional method compared with the statistical one. This is consistent with results observed with other diffusion-based models. 

We perform more recent parameter estimations corresponding to 06/10/1999–06/10/2003 and 09/10/1999–09/10/2003 (via PF based on 1000 particles) for S&P 500. The results are reported in Table 3.3. As we can see, the algorithm for the estimation of the statistical parameters seems fairly stable provided that the initial parameters are chosen sufficiently close to the optimal ones. 


Simulated Log Stock Prices


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/893e9eb1fccc1f34af8c3e503ee007cecf4b6263ef969949606ac7f2dfc9b5f2.jpg)



FIGURE 3.22 Log Stock Prices for Simulated SPX Prices Using $\Psi = ( \kappa = 0 . 0 0 0 0$ ， η 0.0000 λ 0.000000 σ 0.117200 θ 0.0056 ν 0.002) and $\begin{array} { r } { \Psi \ = \ ( \kappa \ = \ } \end{array}$ 79.499687 $\eta = 3 . 5 5 7 7 0 2 ,$  λ 0.000000 σ 0.049656 θ 0.006801 ν 0.008660, $\mu = 0 . 0 3 0 6 9 9 )$ . Unlike arrival rates, the spot prices are hard to distinguish. This is consistent with our previous observations.



TABLE 3.3 VGSA Statistical Parameters Estimated via PF. The stock drifts $\mu _ { S }$ are 0.009999 and 0.010000 respectively.


<table><tr><td>period</td><td><eq>\kappa</eq></td><td><eq>\eta</eq></td><td><eq>\lambda</eq></td><td><eq>\sigma</eq></td><td><eq>\theta</eq></td><td><eq>\nu</eq></td></tr><tr><td>990910-030910</td><td>5.131967</td><td>6.499669</td><td>4.360002</td><td>0.087000</td><td>-0.024862</td><td>0.002000</td></tr><tr><td>990610-030610</td><td>6.514068</td><td>6.500001</td><td>4.360000</td><td>0.085000</td><td>-0.025000</td><td>0.001800</td></tr></table>

The cross-sectional results could be computed in the same way as for diffusion-based models. Quoting the results of Carr et al. [48], we have Table 3.4. As shown, for some periods the risk-neutral implied λ is much larger than the statistical one. This implies the possibility of a skewness trade, as previously discussed. 

It therefore seems that, depending on the period, the statistical and riskneutral parameters λ may or may not be consistent. 

## A WORD OF CAUTION

Accuracy issues of the inference tools aside, there are practical considerations we need to bear in mind. We are applying basic models, such as Heston or 


TABLE 3.4 VGSA Risk-Neutral Arrival-Rate Parameters Estimated from Carr et al. [48]


<table><tr><td>period</td><td>κ</td><td>η</td><td>λ</td></tr><tr><td>Mar 2000</td><td>4.08</td><td>15.99</td><td>16.52</td></tr><tr><td>Jun 2000</td><td>7.24</td><td>32.15</td><td>24.81</td></tr><tr><td>Sep 2000</td><td>0.25</td><td>0.00</td><td>3.76</td></tr><tr><td>Dec 2000</td><td>2.18</td><td>5.71</td><td>5.67</td></tr></table>

VGSA, to a complex and constantly changing market. The true dynamics of the stock and option markets are unknown, and, even if the above models approximate them fairly well, there is no guarantee that there will not be a mutation in future dynamics. The best we can do is to use the information hitherto available and hope that the future behavior of the assets is not too different from the past. 

Needless to say, as time passes by and new information becomes available, we need to update our models and parameter values. This could be done within either a Bayesian or classical framework. Therefore, detecting an inconsistency between the stock and option markets does not allow us to make a riskless profit, because we simply do not know what the future is reserving for us. Once again, the skewness transaction described in this chapter is more similar to selling insurance than to an arbitrage. 

## FOREIGN EXCHANGE, FIXED INCOME, AND OTHER MARKETS

## Foreign Exchange

It is important to note that everything discussed in this book can be applied to time series from other asset classes. A popular asset class to which the Heston and Bates models are often applied is the foreign exchange (FX). Bates [27] applies his jump diffusion model to the USD/deutsche Mark (now euro) exchange rate. 

Calling $X _ { t }$ the FX rate process, for a Heston model, we would have under the real-world measure P 

$$
\begin{array}{c} d \ln X _ {t} = \left(\mu_ {X} - \frac {1}{2} v _ {t}\right) d t + \sqrt {v _ {t}} d B _ {t} \\ d v _ {t} = (\omega - \theta v _ {t}) d t + \xi \sqrt {v _ {t}} \left(\rho d B _ {t} + \sqrt {1 - \rho^ {2}} d Z _ {t}\right) \end{array}
$$


TABLE 3.5 The Volatility and Correlation Parameters for the Cross-Sectional and Time-Series Approaches.


<table><tr><td>Method</td><td>ξ</td><td>ρ</td></tr><tr><td>Cross-Sectional</td><td>0.45</td><td>-0.05</td></tr><tr><td>Time-Series</td><td>0.11</td><td>-0.09</td></tr></table>

with $< d B _ { t } , d Z _ { t } > = 0 \nonumber$ . We could therefore apply any of the previously used filters to the discretization of the above SDE and obtain the optimal parameters via MLE. 

Under the risk-neutral measure Q, the FX drift is the difference between the domestic and the foreign interest rates $r _ { D }$ and $r _ { F }$ . Therefore, we would have 

$$
\begin{array}{c} d \ln X _ {t} = \left[ r _ {D} (t) - r _ {F} (t) - \frac {1}{2} v _ {t} \right] d t + \sqrt {\nu_ {t}} d B _ {t} ^ {(r)} \\ d \nu_ {t} = (\omega^ {(r)} - \theta^ {(r)} \nu_ {t}) d t + \xi \sqrt {\nu_ {t}} \left(\rho d B _ {t} ^ {(r)} + \sqrt {1 - \rho^ {2}} d Z _ {t} ^ {(r)}\right) \end{array}
$$

with $< d B _ { t } ^ { ( r ) } , d Z _ { t } ^ { ( r ) } > = 0 .$ . Note that the usual Heston closed-form optionpricing expression is valid for the FX process. 

As previously discussed, according to the Girsanov theorem, $( \xi , \rho )$ should be the same under the two measures. It is well known that compared with equities, FX options markets have a much lower correlation $\rho$ and have a more symmetric smile. A skewness trade would therefore be more difficult to carry out in this market, but a kurtosis trade taking advantage of the high volatility-of-volatility ξ embedded in the options markets could be appropriate (Table 3.5). 

Similarly to what we did for the equities, we estimate the model parameters from the three-month EUR/USD options cross-sectionally via a leastsquares method on January 2004. And we estimate the time-series parameters (January 2000 to January 2005) via our second chapter filters. As before, adding jumps to the Heston model will help lower the cross-sectional volatility-of-volatility, but it remains insufficient to reconcile them. 

## Fixed Income

The Time Series The same principles could be applied to the interest-rate models with stochastic volatility. Using, for instance, a generalization of the extended-Vasicek [146] short-rate model<sup>14</sup>, we would have under P 

$$
\begin{array}{l} d r _ {t} = a [ \mu (t) - r _ {t} ] d t + \sqrt {\nu_ {t}} d B _ {t} \\ d \nu_ {t} = (\omega - \theta \nu_ {t}) d t + \xi \sqrt {\nu_ {t}} \left(\rho d B _ {t} + \sqrt {1 - \rho^ {2}} d Z _ {t}\right) \end{array}
$$

with $< d B _ { t } , d Z _ { t } > = 0 .$ The difference between this first SDE and the corresponding ones in FX or equities is that the short-rate process is not directly observable. What is observable is the bond yield, which has a closed-form expression as a function of $r _ { t }$ . In an extended Vasicek model, for a given path of $\nu _ { t }$ the price of a forward starting zero-coupon bond is 

$$
P (t, T) = A (t, T) e ^ {- B (t, T) r (t)}
$$

with 

$$
B (t, T) = \frac {1 - e ^ {- a (T - t)}}{a}
$$

$$
\begin{array}{l} \ln A (t, T) = \ln \frac {P (0 , T)}{P (0 , t)} - B (t, T) \frac {\partial \ln P (0 , t)}{\partial t} \\ \qquad - \frac {1}{2} \left(B (t, T) \frac {\partial B (0 , t)}{\partial t}\right) ^ {2} \int_ {0} ^ {t} \left(1 / \frac {\partial B (0 , u)}{\partial u}\right) ^ {2} v _ {u} d u \end{array}
$$

and the bond yield is 

$$
R (t, T) = - \frac {\ln P (t , T)}{T - t}
$$

From the foregoing expressions we can fairly easily deduce that at a given time t, the short rate simply becomes 

$$
r (t) = R (t, t) = - \frac {\partial \ln P}{\partial t} (t, t)
$$

Therefore, we can observe the current short rate as the (negative) initial slope of the yield curve, and we are back to the same framework as for equities and FX processes. 

The Cross Section For the option pricing under Q we would have 

$$
\begin{array}{l} d r _ {t} = a ^ {(r)} \left[ \mu^ {(r)} (t) - r _ {t} \right] d t + \sqrt {\nu_ {t}} d B _ {t} ^ {(r)} \\ d \nu_ {t} = (\omega^ {(r)} - \theta^ {(r)} \nu_ {t}) d t + \xi \sqrt {\nu_ {t}} \left(\rho d B _ {t} ^ {(r)} + \sqrt {1 - \rho^ {2}} d Z _ {t} ^ {(r)}\right) \end{array}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/644f7f4e-b391-4e7f-be0c-22bc5b5ebe38/493bfa059425a6d286e217aa9f6e6a036303ea7ea64d68e921d6e48e43e8457c.jpg)



FIGURE 3.23 A Time Series of the Euro Index from January 2000 to January 2005.


with $< d B _ { t } ^ { ( r ) } , d Z _ { t } ^ { ( r ) } > = 0 .$ Naturally because of the randomness of the volatility, we would lose the closed-form expressions for the options on bonds (or caps or swaptions). However, we can still value them via a two-factor Monte Carlo algorithm. Indeed, we have for an option with maturity U on a zerocoupon bond with maturity $T > U$ 

$$
\begin{array}{l} c = \mathbf {E} _ {0} \left[ \left(\exp (- \int_ {U} ^ {T} r _ {t} d t) - 1\right) ^ {+} \right] \\ = \int_ {0} ^ {+ \infty} \int_ {0} ^ {+ \infty} \left(\exp (- \int_ {U} ^ {T} r _ {t} d t) - 1\right) ^ {+} q (r _ {U}, v _ {U}) d r _ {U} d v _ {U} \end{array}
$$

where $q ( r , \nu )$ represents the joint density of the short rate and its volatility. 

Once again, the Girsanov theorem would require the same $( \xi , \rho )$ parameters under the real-world and risk-neutral measures. A more negative correlation in the cross-sectional options market would therefore favor a skewness trade, and a higher volatility-of-volatility, a kurtosis trade. 

One noticeable point is that, for a given level of option maturity U, we can have many bond maturities. It is known that a swaption can be modeled and priced as an option on a coupon bond.<sup>15</sup> However, there may be many swap tenors for the same option expiration, which introduces an extra dimension. But nothing stops us from using many tenors and option maturities at once for a cross-sectional calibration. 

The choice of the time-series period is still to be questioned. Do we consider the period beginning at our cross-sectional date, or do we consider a start date before this date? The latter would provide us with more data points; however, these points would be historic. As we saw, we probably would need the longer time series in order to have more reliable estimations. 



[1] Ackerberg D. A. (2000) “Importance Sampling and the Method of Simulated Moments” Department of Economics, Boston University and NBER. 





[2] Aihara S., Bagchi A. (2000) “Estimation of Stochastic Volatility in the Hull-White Model” Applied Mathematical Finance, 7. 





[3] Aït-Sahalia Y. (2001) “Telling from Discrete Data Whether the Underlying Continuous-Time Model Is a Diffusion” Journal of Finance, Vol. 57, No. 5. 





[4] Aït-Sahalia Y. (2002) “Maximum Likelihood Estimation of Discretely Sampled Diffusions: A Closed-Form Approximation Approach” Econometrica, Vol. 70, No. 1. 





[5] Aït-Sahalia Y. (2003) “Disentangling Volatility from Jumps” Working Paper, Princeton University. 





[6] Aït-Sahalia Y., Wang Y., Yared F. (2001) “Do Option Markets Correctly Price the Probabilities of Movement of the Underlying Asset?” Journal of Econometrics, 101. 





[7] Alexander C. (1999) “A Primer on the Orthogonal GARCH Model” ISMA Center, University of Reading. 





[8] Alexander C. (2000) “Principles of Skew” RISK. 





[9] Alexander C. (2001) “Market Models: A Guide to Financial Data Analysis” John Wiley & Sons, Ltd. 





[10] Alizadeh S., Brandt M. W., Diebold F. X. (2002) “Range-Based Estimation of Stochastic Volatility Models” Journal of Finance, Vol. 57, No. 3. 





[11] Amin K. I., Ng V. (1993) “Option Valuation with Systematic Stochastic Volatility” Journal of Finance, Vol. 48, Issue 3. 





[12] Andersen A. B. (2000) “Quantifying the Peso Problem Bias: A Switching Regime Approach” Department of Finance, The Aarhus Schools of Business, Denmark. 





[13] Andersen L. B. G., Brotherton-Ratcliffe R. (1997) “The Equity Option Volatility Smile: An Implicit Finite Difference Approach” Journal of Computational Finance, Vol. 1(2). 





[14] Arulampalam S., Maskell S., Gordon N., Clapp T. (2002) “A Tutorial on Particle Filters for On-line Non-linear/ Non-Gaussian Bayesian Tracking” IEEE Transactions on Signal Processing, Vol. 50. No. 2. 





[15] Avellaneda M. (2002) “Empirical Aspects of Dispersion Trading in U.S. Equity Markets” Slides from Presentation at Le Petit Dejeuner de la Finance, Paris. 





[16] Avellaneda M., Friedman C., Holmes R., Samperi D. (1997) “Calibrating Volatility Surfaces via Relative-Entropy Minimization” Applied Mathematical Finance, 4(1). 





[17] Avellaneda M., Levy A., Paras A. (1995) “Pricing and Hedging Derivative Securities in Markets with Uncertain Volatilities” Applied Mathematical Finance, 2. 





[18] Bachelier L. (1900) “Théorie de la Spéculation” Annales Scientifiques de l’École Normale Supérieure, Troisième Série, 17. 





[19] Bagchi A. (2004) “Volatility Estimation under Heston’s Framework” Supervisor, University of Twente Working Paper. 





[20] Bakshi G., Cao C., Chen Z. (1997) “Empirical Performance of Alternative Option Pricing Models” Journal of Finance, Vol. 52, Issue 5. 





[21] Balland P. (2002) “Deterministic Implied Volatility Models” Quantitative Finance, Vol. 2. 





[22] Barle S., Cakici N. (1995) “Growing a Smiling Tree” RISK Magazine, Vol. 8, No. 10. 





[23] Barndorff-Nielsen O. E., Nicolato E., Shephard N. (2002) “Some Recent Developments in Stochastic Volatility Modeling” Quantitative Finance, 2. 





[24] Barndorff-Nielsen O. E., Shephard N. (2001) “Non-Gaussian Ornstein-Uhlenbeck-based Models and Some of Their Uses in Financial Economics” Royal Statistical Society, 63, Part 2. 





[25] Barndorff-Nielsen O. E., Shephard N. (2002) “Econometric Analysis of Realized Volatility and Its Use in Estimating Stochastic Volatility Models” Journal of the Royal Statistical Society, Series B, Vol. 64. 





[26] Bates D. S. (1991) “The Crash of 87: Was It Expected? The Evidence from Options Markets” Journal of Finance, Vol. 46, Issue 3. 





[27] Bates D. S. (1996) “Jumps and Stochastic Volatility: Exchange Rate Processes Implicit in Deutsche Mark Options” Review of Financial Studies, 9. 





[28] Bates D. S. (1998) “Pricing Options Under Jump Diffusion Processes” The Wharton School, University of Pennsylvania. 





[29] Bates D. S. (1998) “Hedging the Smirk” University of Iowa & NBER. 





[30] Bates D. S. (2000) “Post-87 Crash Fears in the S&P 500 Futures Option Market” Journal of Econometrics, 94. 





[31] Bates D. S. (2002) “Maximum Likelihood Estimation of Latent Affine Processes” University of Iowa & NBER. 





[32] Bates D. S. (2002) “Empirical Option Pricing: A Retrospection” Forthcoming in Journal of Econometrics. 





[33] Bensoussan A., Crouhy M. and Galai D. (1995) “Stochastic Equity Volatility Related to the Leverage Effect I: Equity Volatility Behavior” Applied Mathematical Finance, 1. 





[34] Bernardo J., Smith A. F. M. (2001) “Bayesian Theory” John Wiley and Sons. 





[35] Bertsekas D. P. (2000) “Dynamic Programming and Optimal Control” (2nd Edition, Vols. 1 and 2), Athena Scientific. 





[36] Blacher G. (1998) “Local Volatility” RISK Conference Presentation. 





[37] Black F. (1976) “Studies in Stock Price Volatility Changes” Proceedings of the 1976 Meeting of the Business and Economics Statistics Section, American Statistical Association. 





[38] Black F., Scholes M. (1973) “The Pricing of Options and Corporate Liabilities” Journal of Political Economy, 81. 





[39] Blinnikov S., Moessner R. (1998) “Expansion for Nearly Gaussian Distributions” Astronomy and Astrophysics Supplement Series, 130. 





[40] Bollerslev T. (1986) “Generalized Autoregressive Conditional Heteroskedasticity” Journal of Econometrics, 31. 





[41] Bouchaud J. P., Perelló J., Masoliver J. (2003) “Multiple Time-Scales in Volatility and Leverage Correlations: A Stochastic Volatility Model” Working Paper, Centre d’Etudes de Saclay and Universitat de Barcelona. 





[42] Bouchouev I. (1998) “Derivatives Valuation for General Diffusion Processes” The International Association of Financial Engineers (IAFE) Conferences. 





[43] Brandt M. W., Santa-Clara P. (2002) “Simulated Likelihood Estimation of Diffusions with an Application to Exchange Rate Dynamics in Incomplete Markets” Journal of Financial Economics, 63. 





[44] Breeden D. T., Litzenberger R. H. (1978) “Prices of State-Contingent Claims Implicit in Option Prices” Journal of Business, Vol. 51, No. 4. 





[45] Brockhaus O., Long D. (2000) “Volatility Swaps Made Simple” RISK, January 2000. 





[46] Buraschi A., Jackwerth A. C. (2001) “The Price of a Smile: Hedging and Spanning in Option Markets” Review of Financial Studies, 14. 





[47] Carr P., Geman H., Madan D., Yor M. (2002) “The Fine Structure of Asset Returns” Journal of Business, Vol. 75, No. 2. 





[48] Carr P., Geman H., Madan D., Yor M. (2003) “Stochastic Volatility for Lévy Processes” Mathematical Finance, Vol. 13, No. 3. 





[49] Carr P., Lewis K. (2002) “Corridor Variance Swaps” Research Papers, Courant Institute of Mathematical Sciences, New York University. 





[50] Carr P., Madan D. (1998) “Toward a Theory of Volatility Trading” Research Papers, Courant Institute of Mathematical Sciences, New York University. 





[51] Carr P., Madan D. (1998) “Option Valuation Using the Fast Fourier Transform” Morgan Stanley and University of Maryland. 





[52] Carr P., Madan D. (2001) “Optimal Positioning in Derivative Securities” Quantitative Finance, Vol. 1. 





[53] Carr P., Madan D. (2001) “Optimal Investment in Derivative Securities” Finance and Stochastics, Vol. 5. 





[54] Carr P., Wu L. (2003) “Time-Changed Lévy Processes and Option Pricing” Journal of Financial Economics. 





[55] Casella G., George E. I. (1992) “Explaining the Gibbs Sampler” The American Statistician, Vol. 46, No. 3. 





[56] Chernov M., Ghysels E. (2000) “A Study Toward a Unified Approach to the Joint Estimation of Objective and Risk-Neutral Measures for the Purpose of Option Valuation” Journal of Financial Economics, 56. 





[57] Chib S., Nadari F., Shephard N. (1998) “Markov Chain Monte-Carlo Methods for Generalized Stochastic Volatility Models” Washington University and The University of Oxford. 





[58] Chib S., Greenberg E. (1995) “Understanding the Metropolis-Hastings Algorithm” The American Statistician, Vol. 49, No. 4. 





[59] Chourdakis K. M. (2001) “Volatility Persistence, Regime Switches and Option Pricing” Department of Economics, University of London. 





[60] Chriss N. A. (1997) “Black Scholes and Beyond: Option Pricing Models” Irwin/McGraw Hill. 





[61] Corradi V. (2000) “Reconsidering the Continuous Time Limit of the GARCH(1,1) Process” Journal of Econometrics, 96. 





[62] Corrado C. J., Su T. (1997) “Implied Volatility Skews and Stock Index Skewness and Kurtosis Implied by S&P 500 Index Option Prices” University of Missouri at Columbia, University of Miami at Coral-Gables. 





[63] Corrado C. J., Su T. (1997) “Implied Volatility Skews and Stock Return Skewness and Kurtosis Implied by Stock Option Prices” The European Journal of Finance, 3. 





[64] Cox J. C. (1996) “The Constant Elasticity of Variance Option Pricing Model” Journal of Portfolio Management, Special Issue. 





[65] Cox J. C., Ross S. (1976) “The Valuation of Options for Alternative Stochastic Processes” Journal of Financial Economics, 3. 





[66] Cox J. C., Ross S., Rubinstein M. (1979) “Option Pricing: A Simplified Approach” Journal of Financial Economics, 7. 





[67] Cox J. C., Rubinstein M. (1985) “Options Markets” Prentice Hall. 





[68] Crosbie P. J. (1999) “Modeling Default Risk” KMV Working Papers. 





[69] Das S. R., Sundaram R. K. (1997) “Taming the Skew: Higher-Order Moments in Modeling Asset-Price Processes in Finance” National Bureau of Economic Research. 





[70] Demeterfi K., Derman E., Kamal M., Zou J. (1999) “More than You Ever Wanted to Know About Volatility Swaps” Goldman Sachs Quantitative Strategy Papers. 





[71] Dempster M. A. H., Gotsis G. Ch. (1998) “On the Martingale Problem for Jumping Diffusions” University of Cambridge and Hellenic Capital Market Commission. 





[72] Deng S. (2000) “Stochastic Models for Energy Commodity Prices and Their Applications: Mean-Reversion with Jumps and Spikes” Industrial and Systems Engineering, Georgia Institute of Technology. 





[73] Derman E. (1999) “Regimes of Volatility: Some Observations on the Variations of S&P 500 Implied Volatilities” Goldman Sachs Quantitative Strategy Papers. 





[74] Derman E., Kani I. (1994) “Riding on a Smile” RISK Magazine, 7. 





[75] Derman E., Kani I. (1994) “The Volatility Smile and Its Implied Tree” Goldman Sachs Quantitative Strategy Papers. 





[76] Derman E., Kani I. (1998) “Stochastic Implied Trees: Arbitrage Pricing with Stochastic Term and Strike Structure of Volatility” International Journal of Theoretical and Applied Finance, 1. 





[77] Derman E., Kani I., Chriss N. (1996) “Implied Trinomial Trees of the Volatility Smile” Goldman Sachs Quantitative Strategy Papers. 





[78] Derman E., Kani I., Zou J. (1995) “The Local Volatility Surface: Unlocking the Information in Index Option Prices” Goldman Sachs Quantitative Strategy Papers. 





[79] Doucet A., De Freitas N., Gordon N. (2001) “Sequential Monte-Carlo Methods in Practice” Springer-Verlag. 





[80] Doucet A., Gordon N., Krishnamurthy V. (2001) “Particle Filters for State Estimation of Jump Markov Linear Systems” IEEE Transactions on Signal Processing, Vol. 49, No. 3. 





[81] Dragulescu A. A., Yakovenko V. M. (2002) “Probability Distribution of Returns in the Heston Model with Stochastic Volatility” Department of Physics, University of Maryland. 





[82] Duan J. C. (1995) “The GARCH Option Pricing Model” Mathematical Finance, 5. 





[83] Duan J. C. (1996) “Cracking the Smile” RISK Magazine, 9. 





[84] Duan J. C. (1996) “A Unified Theory of Option Pricing Under Stochastic Volatility: From GARCH to Diffusion” Hong Kong University of Science and Technology. 





[85] Duan J. C. (1997) “Augmented GARCH(p,q) Process and Its Diffusion Limit” Journal of Econometrics, 79. 





[86] Duan J. C. (2001) “Risk Premium and Pricing of Derivatives in Complete Markets” Rotman School of Management, University of Toronto. 





[87] Dufresne Daniel (2001) “The Integrated Square-Root Process” Center for Actuarial Studies, The University of Melbourne. 





[88] Dumas B., Fleming J., Whaley R. E. (1998) “Implied Volatility Functions: Empirical Tests” Journal of Finance, Vol. 53, Issue 6. 





[89] Dupire B. (1994) “Pricing with a Smile” RISK Magazine, 7. 





[90] Durrett R. (1996) “Stochastic Calculus: A Practical Introduction” CRC Press, Boca Raton, Florida. 





[91] El-Karoui N., Quenez M. C. (1995) “Dynamic Programming and Pricing of Contingent Claims in Incomplete Markets” SIAM Journal of Control and Optimization, 33(1). 





[92] Elerian O., Chib S., Shephard N. (2001) “Likelihood Inference for Discretely Observed Nonlinear Diffusions” Econometrica. 





[93] Elliott R. J., Lahaie C. H., Madan D. (1997) “Filtering Derivative Security Valuations from Market Prices” University of Alberta, University of Maryland. 





[94] Engle R. F. (1982) “Autoregressive Conditional Heteroskedasticity with Estimates of the Variance of United Kingdom Inflation” Econometrica, Vol. 50, No. 4. 





[95] Engle R. F., Ishida I. (2002) “The Square-Root, the Affine, and the CEV GARCH Models” Working Paper, New York University and University of California, San Diego. 





[96] Engle R. F., Mezrich J. (1995) “Grappling with GARCH” RISK Magazine, 9. 





[97] Engle R. F., Ng V. (1993) “Measuring and Testing the Impact of News on Volatility” Journal of Finance, Vol. 48, Issue 5. 





[98] Eraker B., Johannes M., Polson N. (2003) “The Impact of Jumps in Equity Index Volatility and Returns” Journal of Finance, 58. 





[99] Fama E. (1965) “The Behavior of Stock Market Prices” Journal of Business, 38. 





[100] Fan J., Yao Q. (2003) “Nonlinear Time Series: Nonparametric and Parametric Methods” Springer. 





[101] Fleming J., Kirby C. (2003) “A Closer Look at the Relation Between GARCH and Stochastic Autoregressive Volatility” Journal of Financial Econometrics, Vol. 1, December. 





[102] Follmer H., Sondermann D. (1986) “Hedging of Non-Redundant Contingent-Claims” Contributions to Mathematical Economics, North-Holland. 





[103] Forbes C. S., Martin G. M., Wright J. (2002) “Bayesian Estimation of a Stochastic Volatility Model Using Option and Spot Prices” Department of Econometrics and Business Statistics, Monash University, Australia. 





[104] Fouque J. P., Papanicolaou G., Sircar K. (2000) “Derivatives in Financial Markets with Stochastic Volatility” Cambridge University Press. 





[105] Fouque J. P., Papanicolaou G., Sircar K. (2000) “Mean Reverting Stochastic Volatility” International Journal of Theoretical and Applied Finance, 3(1). 





[106] Fouque J. P., Tullie T. A. (2002) “Variance Reduction for Monte-Carlo Simulation in a Stochastic Volatility Environment” Quantitative Finance, 2. 





[107] Frey R. (1997) “Derivative Asset Analysis in Models with Level-Dependent and Stochastic Volatility” Department of Mathematics, ETH Zurich. 





[108] Fridman M., Harris L. (1998) “A Maximum Likelihood Approach for Non-Gaussian Stochastic Volatility Models” Journal of Business and Economic Statistics. 





[109] Gallant A. R., Tauchen G. (2001) “Efficient Method of Moments” University of North Carolina and Duke University. 





[110] Galli A. (2000) “Variograms and Cross-Variograms” Ecole des Mines de Paris, Working Paper. 





[111] Galli A., Lautier D. (2001) “Un Modèle de Structure par Terme des Prix des Matières Premières avec Comportement Asymétrique du Rendement d’Opportunité” École des Mines de Paris & CEREG, Université Paris IX. 





[112] Garcia R., Ghyseles E., Renault E. (2002) “The Econometrics of Option Pricing” Université de Montreal and University of North Carolina. 





[113] Gatheral J. G. (2001) “Stochastic Volatility and Local Volatility” Courant Institute of Mathematical Sciences, New York University. 





[114] Gatheral J. G. (2001) “Fitting the Volatility Skew” Courant Institute of Mathematical Sciences, New York University. 





[115] Gatheral J. G. (2001) “Asymptotics and Dynamics of the Volatility Skew” Courant Institute of Mathematical Sciences, New York University. 





[116] Gatheral J. G. (2001) “Volatility and Variance Swaps” Courant Institute of Mathematical Sciences, New York University. 





[117] Geman H., El-Karoui N., Rochet J. C. (1995) “Changes of Numeraire, Changes of Probability Measure and Option Pricing” Journal of Applied Probability, 32(2). 





[118] Geman H., Madan D., Yor M. (2001) “Stochastic Volatility, Jumps and Hidden Time Changes” Finance and Stochastics. 





[119] Geske R. (1979) “The Valuation of Compound Options” Journal ofFinancial Economics, 7. 





[120] Gilks W. R., Richardson S., Spiegelhalter D. J. (1995) “Markov Chain Monte Carlo in Practice” Chapman & Hall/ CRC. 





[121] Gondzio J., Kouwenberg R., Vorst T. (2003) “Hedging Options Under Transaction Costs and Stochastic Volatility” Journal of Economic Dynamics and Control, 27. 





[122] Gordon N. J., Salmond D. J. Smith A. F. M. (1993) “Novel Approach to Nonlinear/Non-Gaussian Bayesian State Estimation” IEE Proceedings-F, Vol. 140, No. 2. 





[123] Gourieroux C., A. Monfort, Renault E. (1993) “Indirect Inference” Journal of Applied Econometrics, 8. 





[124] Gourieroux C., Jasiak J. (2001) “Financial Econometrics” Princeton University Press. 





[125] Grabbe J. O. (1983) “The Pricing of Put and Call Options on Foreign Exchange” Journal of International Money and Finance, December. 





[126] Hamilton J. D. (1989) “A New Approach to the Econometric Analysis of Non-stationary Time Series and the Business Cycle” Econometrica, Vol. 57, No. 2. 





[127] Hamilton J. D. (1994) “Time Series Analysis” Princeton University Press. 





[128] Härdle W., Kleinow T., Stahl G. (2002) “Applied Quantitative Finance” Springer-Verlag. 





[129] Harvey A. C. (1989) “Forecasting, Structural Time Series Models, and the Kalman Filter” Cambridge University Press. 





[130] Harvey A. C., Ruiz E., Shephard Neil (1994) “Multivariate Stochastic Variance Models” Review of Economic Studies, Vol. 61, Issue 2. 





[131] Harvey C. R., Whaley R. E. (1991) “S&P 100 Index Option Volatility” Journal of Finance, Vol. 46, Issue 4. 





[132] Haug E. G. (1997) “The Complete Guide to Option Pricing Formulas” McGraw-Hill, New York. 





[133] Haykin S. (2001) “Kalman Filtering and Neural Networks” Wiley Inter-Science. 





[134] Heston S. (1993) “A Closed-Form Solution for Options with Stochastic Volatility with Applications to Bond and Currency Options” Review of Financial Studies, 6. 





[135] Heston S. (2000) “Derivatives on Volatility: Some Simple Solutions Based on Observables” Federal Reserve Bank of Atlanta, Working Paper. 





[136] Heston S., Christoffersen P., Jacobs K. (2004) “Option Valuation with Conditional Skewness” University of Maryland and McGill University. 





[137] Heston S., Nandi S. (1997) “A Closed Form GARCH Option Pricing Model” Federal Reserve Bank of Atlanta, Working Paper 97-9. 





[138] Hipp C., Taksar M. (2000) “Hedging in Incomplete Markets and Optimal Control” University of Karlsruhe and SUNY at Stony-Brook. 





[139] Hirsa A., Javaheri A. (2003) “A Particle Filtering Algorithm for the VGSA Model” Working Paper, Morgan Stanley and RBC Capital Markets. 





[140] Hobson D. G. (1996) “Stochastic Volatility” School ofMathematical Sciences, University of Bath. 





[141] Hobson D. G., Rogers L. C. G. (1998) “Complete Models with Stochastic Volatility” Mathematical Finance, 8. 





[142] Honoré P. (1998) “Pitfalls in Estimating Jump-Diffusion Models” Department of Finance, The Aarhus School of Business, Denmark. 





[143] Howison S. D., Rafailidis A., Rasmussen H. O. (2000) “A Note on the Pricing and Hedging of Volatility Derivatives” The University of Oxford, Kings College London. 





[144] Hughston L. P. (2004) “International Models for Interest Rates and Foreign Exchange: A General Framework for the Unification of Interest Rate Dynamics and Stochastic Volatility” Global Derivatives and Risk Management, May 2004. 





[145] Hughston L. P., Rafailidis A. (2004) “A Chaotic Approach to Interest Rate Modeling” Finance and Stochastic. 





[146] Hull J. (1999) “Options, Futures, and Other Derivative Securities” Englewood Cliffs, 4th Edition. 





[147] Hull J., Suo W. (2002) “A Methodology for Assessing Model Risk and its Application to the Implied Volatility Function Model”Journal of Financial and Quantitative Analysis. 





[148] Hull J., Suo W. (2002) “Modeling the Volatility Surface” University of Toronto and Queen’s University. 





[149] Hull J., White A. (1987) “The Pricing of Options on Assets with Stochastic Volatility” Journal of Finance, Vol. 42, Issue 2. 





[150] Hull J., White A. (1988) “An Analysis of the Bias in Option Pricing Caused by a Stochastic Volatility” Advances in Futures and Options Research, 3. 





[151] Ito K., Xiong K. (1999) “Gaussian Filters for Nonlinear Filtering Problems” Center for Research in Scientific Computation, North Carolina State University. 





[152] Jackel P. (2002) “Monte-Carlo Methods in Finance” Wiley Series in Finance. 





[153] Jackson N., Suli E., Howison S. (1998) “Computation of Deterministic Volatility Surfaces” Journal of Computational Finance Vol. 2(2). 





[154] Jackwerth J. C. (2000) “Option-Implied Risk-Neutral Distributions and Implied Binomial Trees: A Literature Review” Journal of Derivatives, 7. 





[155] Jackwerth J. C., Rubinstein M. (1996) “Recovering Probability Distributions from Option Prices” Journal of Finance, Vol. 51, Issue 5. 





[156] Jacquier E., Polson N. G., Rossi P. E. (1994) “Bayesian Analysis of Stochastic Volatility Models” Journal of Business and Economic Statistics, Vol. 12, No, 4. 





[157] Jarrow R., Rudd A. (1982) “Approximate Option Valuation for Arbitrary Stochastic Processes” Journal of Financial Economics, 10. 





[158] Javaheri A., Wilmott P., Haug E. G. (2002) “GARCH and Volatility Swaps” Wilmott, January 2002. 





[159] Javaheri A., Lautier D., Galli A. (2003) “Filtering in Finance” Wilmott, Issue 5. 





[160] Javaheri A. (2004) “Inference and Stochastic Volatility” Wilmott, Issue 11. 





[161] Jex M., Henderson R., Wang D. (1999) “Pricing Exotics Under the Smile” RISK Magazine. 





[162] Jiang G. J., Van der Sluis P. J. (2000) “Index Option Pricing with Stochastic Volatility and Stochastic Interest Rates” Center for Economic Research. 





[163] Johannes M., Polson N. (2002) “MCMC Methods for Financial Econometrics” The Handbook of Financial Econometrics. 





[164] Johannes M., Polson N., Stroud J. (2002) “Nonlinear Filtering of Stochastic Differential Equations with Jumps” Working Paper, Columbia University, University of Chicago and University of Pennsylvania. 





[165] Jones C. S. (2001) “The Dynamics of Stochastic Volatility: Evidence from Underlying and Options Markets” Simon School of Business, University of Rochester. 





[166] Julier S. J., Uhlmann J. K. (1997) “A New Extension of the Kalman Filter to Nonlinear Systems” The University of Oxford, The Robotics Research Group. 





[167] Karatzas I., Shreve S. (1991) “Brownian Motion and Stochastic Calculus” Springer-Verlag, 2nd Edition. 





[168] Kennedy P. (1998) “A Guide to Econometrics” MIT Press, 4th Edition. 





[169] Kim S., Shephard N., Chib S. (1998) “Stochastic Volatility: Likelihood Inference and Comparison with ARCH Models” Review of Economic Studies, Vol. 65. 





[170] Kitagawa G. (1987) “Non-Gaussian State Space Modeling of Non-Stationary Time Series” Journal of American Statistical Association, 82. 





[171] Kitagawa G. (1996) “Monte-Carlo Filter and Smoother for Non-Gaussian Nonlinear Sate Space Models” Journal of Computational and Graphical Statistics, Vol. 5, No. 1. 





[172] Kou S. (2000) “A Jump Diffusion Model for Option Pricing with Three Properties: Leptokurtic Feature, Volatility Smile, and Analytical Tractability” Econometric Society World Congress 2000 Contributed Papers. 





[173] Kushner H. J. (1967) “Approximations to Optimal Nonlinear Filters” IEEE Transactions on Automatic Control, Vol. 12. 





[174] Kushner H. J., Budhiraja A. S. (2000) “A Nonlinear Filtering Algorithm Based on an Approximation of the Conditional Distribution” IEEE Transactions on Automatic Control, Vol. 45. No. 3. 





[175] Lagnado R., Osher S. (1997) “A Technique for Calibrating Derivative Security Pricing Model: Numerical Solution of an Inverse Problem” Journal of Computational Finance, Vol. 1(1). 





[176] Lee D. S., Chia N. K. K (2002) “A Particle Algorithm for Sequential Bayesian Parameter Estimation and Model Selection” IEEE Transactions on Signal Processing, Vol. 50, No. 2. 





[177] Lewis A. L. (2000) “Option Valuation under Stochastic Volatility” Finance Press. 





[178] Lewis A. L. (2001) “A Simple Option Formula for General Jump-Diffusion and Other Exponential Levy Processes” OptionCity.net Publications. 





[179] Lewis A. L. (2002) “The Mixing Approach to Stochastic Volatility and Jump Models” Wilmott, March 2002. 





[180] Lewis A. L. (2002) “Fear of Jumps” Wilmott, Issue 2. 





[181] Li Y. (2000) “A New Algorithm for Constructing Implied Binomial Trees: Does the Implied Model Fit Any Volatility Smile?” Journal of Computational Finance, Vol. 4(2). 





[182] Madan D., Carr P., Chang E. C. (1998) “The Variance-Gamma Process and Option Pricing” European Finance Review, Vol. 2, No. 1. 





[183] Maes K. (2001) “Panel Data Estimating Continuous-Time Arbitrage-Free Affine Term-Structure Models with the Kalman Filter” International Economics, Leuven University. 





[184] Maheu J. M., McCurdy T. H. (2003) “News Arrival, Jump Dynamics, and Volatility Components for Individual Stock Returns” University of Toronto. 





[185] Markowiz H. M. (1990) “Mean-Variance Analysis in Portfolio Choice and Capital Markets” Basil Blackwell. 





[186] Matacz A. (1997) “Financial Modeling and Option Theory with the Truncated Levy Process” School of Mathematics and Statistics, University of Sidney. 





[187] Matytsin A. (1999) “Modeling Volatility and Volatility Derivatives” Columbia Practitioners Conference on the Mathematics of Finance. 





[188] Merton R. C. (1973) “The Theory of Rational Option Pricing” Bell Journal of Economics and Management, 7. 





[189] Merton R. C. (1974) “On the Pricing of Corporate Debt: The Risk Structure of Interest Rates” Journal of Finance, Vol. 29, Issue 2. 





[190] Merton R. C. (1976) “Option Pricing When the Underlying Stock Returns Are Discontinuous” Journal of Financial Economics. 





[191] Meyer R., Fournier D. A., Berg A. (2003) “Stochastic Volatility: Bayesian Computation Using Automatic Differentiation and the Extended Kalman Filter” Econometrics Journal, Vol. 6. 





[192] Muzzioli S., Torricelli C. (2001) “Implied Trees in Illiquid Markets: A Choquet Pricing Approach” Universita degli Studi di Modena e Reggio Emilia, Dipartimento di Economia Politica. 





[193] Neftci S. N. (1996) “An Introduction to the Mathematics of Financial Derivatives” Academic Press, San Diego, CA. 





[194] Nelson D. B. (1990) “ARCH Models as Diffusion Approximations” Journal of Econometrics, 45. 





[195] Nelson D. B. (1990) “Conditional Heteroskedasticity and Asset Returns: A New Approach” Econometrica, 59. 





[196] Nelson D. B., Foster D. P. (1994) “Asymptotic Filtering Theory for Univariate ARCH Models” Econometrica, Vol. 62, Issue 1. 





[197] Oksendal B. (1998) “Stochastic Differential Equations: An Introduction with Applications” Springer-Verlag New York, 5th Edition. 





[198] Pan G. (2001) “Equity to Credit Pricing” RISK November 2001. 





[199] Pan J. (2002) “The Jump Risk-Primia Implicit in Options: Evidence from an Integrated Time-Series Study” Journal of Financial Economics, 63. 





[200] Parkinson M. (1980) “The Extreme Value Method for Estimating the Variance of the Rate of Return” Journal of Business, 53. 





[201] Pedersen A. R. (1995) “A New Approach to Maximum Likelihood Estimation for Stochastic Differential Equations Based on Discrete Observations” Scandinavian Journal of Statistics, 22. 





[202] Pham H. (2001) “Smooth Solutions to Optimal Investment Models with Stochastic Volatilities and Portfolio Constraints” CNRS and Université Paris 7. 





[203] Pitt M. K., Shephard N. (1999) “Filtering via Simulation: Auxiliary Particle Filters” Journal of the American Statistical Association, 94. 





[204] Press W. H., Teukolsky S. A., Vetterling W. T., Flannery B. P. (1997) “Numerical Recipes in C: The Art of Scientific Computing” Cambridge University Press, 2nd Edition. 





[205] Reif K., Gunther S., Yaz A. (1999) “Stochastic Stability of the Discrete-Time Extended Kalman Filter” IEEE Transactions on Automatic Control. 





[206] Renault E., Touzi N. (1996) “Option Hedging and Implied Volatilities in a Stochastic Volatility Model” Mathematical Finance, 6. 





[207] Ribiero C., Webber N. (2002) “Valuing Path-Dependent Options in the Variance-Gamma Model by Monte-Carlo with a Gamma Bridge” Working Paper, University of Warwick and City University of London. 





[208] Ritchken P., Trevor R. (1997) “Pricing Options under Generalized GARCH and Stochastic Volatility Processes” CMBF Papers, Macquarie University, 19. 





[209] Romano M., Touzi N. (1997) “Contingent Claims and Market Completeness in a Stochastic Volatility Model” Mathematical Finance, 7. 





[210] Rubinstein M. (1983) “Displaced Diffusion Option Pricing” Journal of Finance, Vol. 38, Issue 1. 





[211] Samuelson P. A. (1965) “Rational Theory of Warrant Pricing” Industrial Management Review, 6, 2. 





[212] Sandmann G., Koopman S. J. (1998) “Estimation of Stochastic Volatility Models via Monte-Carlo Maximum Likelihood”Journal ofEconometrics, 87. 





[213] Schonbucher P. J. (1998) “A Market Model for Stochastic Implied Volatility” Department of Statistics, Bonn University. 





[214] Scott L. O. (1987) “Option Pricing when the Variance Changes Randomly: Theory, Estimation, and Application” Journal of Financial and Quantitative Analysis, Dec. 





[215] Scott L. O. (1997) “Pricing Stock Options in a Jump-Diffusion Model with Stochastic Volatility and Interest Rates: Applications of Fourier Inversion Methods” Mathematical Finance, 7. 





[216] Shimko D. (1993) “Bounds on Probability” RISK, 6. 





[217] Shimko D., Tejima N., Van Deventer D. R. (1993) “The Pricing of Risky Debt when Interest Rates are Stochastic” Journal ofFixed Income, September 1993. 





[218] Shreve S., Chalasani P., Jha S. (1997) “Stochastic Calculus and Finance” Carnegie Mellon University. 





[219] Silva A. C., Yakovenko V. M. (2002) “Comparison Between the Probability Distribution of Returns in the Heston Model and Empirical Data for Stock Indices” Department of Physics, University of Maryland. 





[220] Sin C. A. (1998) “Complications with Stochastic Volatility Models” Advances in Applied Probability, 30. 





[221] Smith A. F. M., Gelfand A. E. (1992) “Bayesian Statistics Without Tears: A Sampling-Resampling Perspective” The American Statistician, Vol. 46, No. 2. 





[222] Srivastava A., Grenander U., Jensen G. R., Miller M. I. (2002) “Jump-Diffusion Markov Processes on Orthogonal Groups for Object Recognition” Journal of Statistical Planning and Inference, Special Issue. 





[223] Stein E. M., Stein J. (1991) “Stock Price Distributions with Stochastic Volatility: An Analytic Approach” Review of Financial Studies, 4. 





[224] Storvik G. (2002) “Particle Filters in State Space Models with Presence of Unknown Static Parameters” IEEE Transactions on Signal Processing, 50. 





[225] Taleb N. (1996) “Dynamic Hedging: Managing Vanilla and Exotic Options” John Wiley & Sons, Ltd. 





[226] Tavella D., Klopfer W. (2001) “Implying Local Volatility” Wilmott, August 2001. 





[227] Tavella D., Randall C. (2000) “Pricing Financial Instruments: The Finite Difference Method” John Wiley & Sons, Ltd. 





[228] Toft K. B., Prucyk B. (1997) “Options on Leveraged Equity: Theory and Empirical Tests” Journal of Finance Vol. 52, Issue 3. 





[229] Van der Merwe R., Doucet A., de Freitas N., Wan E. (2000) “The Unscented Particle Filter” Oregon Graduate Institute, Cambridge University, and UC Berkeley. 





[230] Varadhan S. R. S. (2000) “Probability Theory” Courant Institute of Mathematical Sciences, New York University. 





[231] Wan E. A., Van der Merwe R. (2000) “The Unscented Kalman Filter for Nonlinear Estimation” Oregon Graduate Institute ofScience and Technology. 





[232] Wan E. A., Van der Merwe R., Nelson A. (2000) “Dual Estimation and the Unscented Transformation” Oregon Graduate Institute of Science and Technology. 





[233] Welch G., Bishop G. (2002) “An Introduction to the Kalman Filter” Department of Computer Science, University of North Carolina at Chapel Hill. 





[234] Wells C. (1996) “The Kalman Filter in Finance (Advanced Studies in Theoretical and Applied Econometrics), Vol. 32” Kluwer Academic Publishers. 





[235] Whitt W. (2001) “Stochastic Process Limits: An Introduction to Stochastic Process Limits and Their Application to Queues” AT&T Labs Research, Springer. 





[236] Wiggins J. B. (1987) “Option Values under Stochastic Volatility” Journal of Financial Economics, 19. 





[237] Wilmott P. (2000) “Paul Wilmott on Quantitative Finance” John Wiley & Sons, Ltd. 





[238] Wilmott P., Dewynne J., Howison S. (1993) “Option Pricing: Mathematical Pricing and Computations” Oxford Financial Press. 





[239] Wilmott P., Rasmussen H. O. (2002) “Asymptotic Analysis of Stochastic Volatility Models” Wilmott Associates. 





[240] Zellner A. (2000) “Bayesian and Non-Bayesian Approaches to Scientific Modeling and Inference in Economics and Econometrics” University of Chicago. 





[241] Zhang L., Mykland P. A., Aït-Sahalia Y. (2003) “A Tale of Two Time-Scales: Determining Integrated Volatility with Noisy High-Frequency Data” Working Paper. Carnegie Melon University, University of Chicago, and Princeton University. 





[242] Zhou C. (1997) “A Jump-Diffusion Approach to Modeling Credit Risk and Valuing Defaultable Securities” Federal Reserve Board, Washington, DC. 



3/2 models, 122, 188 

Ackerberg, D.A., 224 

Aihara, S., 224 

Ait-Sahalia, Y., 159, 187–189, 198, 200, 224, 235 

Alexander, C., 224 

Alizadeh, S., 224 

Amin, K.I., 224 

Andersen, A.B., 224 

Andersen, L.B., 224 

Arbitrage opportunity, 214 

Arrival rate, 171, 182 

Arrow-Debreu prices, 17 

Arulampalam, S., 224 

Asset term, elimination, 13 

Augmented state, 76 vector, 63 

Auto-correlation, usage, 181 

Auto-regressive moving average model, 21 

Avellaneda, M., 20, 224, 225 

Bachelier, L., 2, 225 

Back-testing procedures, 170 

Bagchi, A., 224, 225 

Bakshi, G., 47, 187, 189, 199, 225 

Balland, P., 225 

Barle, S., 225 

Barndorff-Nielsen, O.E., 225 

Bates, D.S., 158, 189, 208, 225 

Bates model, 185 

EPF application, 162–165 

Bayesian approach, 48, 144–156 example, 146–147 

Bensoussan, A., 225 

Bensoussan-Crouhy-Galai (BCG) approach, 11–13 model, 1 

Berg, A., 233 

Bernardo, J., 225 

Bertsekas, D.P., 225 

Bessel function, 184 

Bias test, 54 

Bid-ask spread, 71, 206 

Binomial tree, usage, 6, 17 

Bishop, G., 235 

Blacher, G., 225 

Black, F., 225 

Black-Scholes approach, 5–6 

Black-Scholes equation rederiving, 29 

Black-Scholes formula, usage, 15 

Black-Scholes implied volatility, 196 

Black-Scholes PDE, 1 

Black-Scholes pricing function, 213 

Black-Scholes risk-neutral pricing formula, 4 

Black-Scholes risk-neutrality argument, usage, 25 

Blocking technique, 150 

Bollerslev, T., 226 

Bouchaud, J.P., 226 

Bouchouev, I., 226 

Box-Ljung test, 48, 95–96 

Brandt, M.W., 224, 226 

Breeden, D.T., 14, 226 

Breeden-Litzenberger identity, 14 

Brockhaus, O., 226 

Brotherton-Ratcliffe, R., 224 

Brownian motion, 22, 40, 43 construction, 97 independence, 44, 158 process, 2 spot return variances, 19 

Budhiraja, A.S., 232 

Buraschi, A., 226 

Burn-in period, 76 

Cakici, N., 225 

Calibration frequency, 19 

Cao, C., 47, 189, 199, 225 

Carr, P., 215, 226, 232 

Carr-Madan replication, 202–203 

Chalasani, P., 234 

Chang, E.C., 215, 232 

Chapman-Kolmogorov equation, application, 58 

Characteristic function, usage, 157–158 

Chen, Z., 47, 189, 199, 225 

Chernov, M., 226 

Chia, N.K.K., 232 

Chib, S., 226, 228, 232 

Chi-square test, 95 usage, 179–181 

Cholesky factorization, usage, 31, 66, 74, 87 

Chourdakis, K.M., 159, 226 

Chriss, N.A., 227 

Christoffersen, P., 230 

CIR process, usage, 44 

Clapp, T., 224 

Close-to-the-money strike prices, optimization, 50 

Close-to-the-money strikes, 192 

Conjugate directions, 49 

Conjugate priors, 145 

Consistency test, 189–197 

cross-sectional results, 190–193 robustness issues, 190–193 setting, 190 

Constant elasticity variance (CEV), 1 approach, 11 

Constant volatility approach, extension, 4 

Constraint parameter, 18 

Continual recalibration (CR) strategy, 19 

Continuous ideal process, sample, 3 

Continuous SDE, 131 

Convergence issues/solutions, 185–186 

Corradi, V., 24, 227 

Corrado, C.J., 227 

Correlation parameter, 156 

Covariance matrix, 70, 83, 161 

Covered call option, transform results, 34 

Cox, J.C., 7, 11, 227 

Cox-Ross-Rubinstein approach, 6–7 

Cramer-Rao bound, 56 

Credit spread, link, 10 

Cross-sectional VGSA, time-series VGSA (contrast), 216–218 

Crouhy, M., 225 

Cumulative distribution function (CDF), 41, 45, 101 

Das, S.R., 203, 227 De Freitas, N., 227, 235 Delta hedging, 200, 204 Demeterfi, K., 227 Dempster, M.A.H., 227 Deng, S., 159, 227 Derivative security, payoff inclusion, 32 Derivatives market, 4–7 Derman, E., 14, 227 Derman-Kani approach, 17 Deterministic volatility, example, 34–35 Dewynne, J., 235 Diagnostics, 95–98 Diebold, F.X., 224 Diffusion limits, 21–24 Diffusion-based model, 47 Direction set method (Powell method), 49–50, 83–84 Directional risks, 200–202 Discrete GARCH, 23–24 Discrete NGARCH, risk-neutral version, 26 Diversification argument, usage, 10 Doucet, A., 227, 235 Dragulescu, A.A., 158, 228 Duan, J.C., 228 Dufresne, Daniel, 228 Dumas, B., 187, 189, 228 Dupire, B., 14, 228 Dupire approach, 14–17 Dupire identity, 14–15 Durrett, R., 228 

Early termination, 206 

Elerian, O., 228 

El-Karoui, N., 27, 228, 229 Elliott, R.J., 228 Engle, R.F., 21, 123, 228 Entropy distance, 18 Eraker, B., 228 Ergodic averaging theorem, 144 Errors, distribution, 50–54 Euler approximation, usage, 23 Euler scheme, 140 EUR/USD options, 220 Extended Kalman filter (EKF), 59–62, 88, 161–162 application, 132, 172–173 convergence, 105 estimation, 85, 139 framework, log-likelihood function, 140 implementation, 89–94 Jacobians, 77 observability, 75–76 Extended particle filter (EPF), 102, 161–166, 172–176, 179 

Fama, E., 228 Fan, J., 228 Feller distribution, 3–4 Feynmann-Kac equation, 6 Filter errors, 84 Filtering, 57–59 errors, 115, 117 normalized/non-normalized weights, 99 Financial interpretation, 194–197 Firm structure model, usage, 12 Fisher information matrix, 56 Fixed fractional jump size, 158–159 Fixed income, 219–223 Flannery, B.P., 233 Fleming, J., 189, 228 

Fletcher-Reeves-Polak-Ribiere method, 49 

Fokker-Planck equation, 14–15 

Follmer, H., 228 

Forbes, C.S., 229 

Foreign exchange (FX), 219–220 rate process, 219 

Forward Kolmogorov equation, 14–15 

Foster, D.P., 233 

Fouque, J.P., 21, 96, 229 

Fourier transform, inversion, 30 

Fournier, D.A., 233 

Frey, R., 229 

Fridman, M., 229 

Friedman, C., 224 

Friedman, Milton, 198 

Further-from-the-money options, 192 

Future spot prices, 7 

Galai, D., 225 

Garcia, R., 229 

Gauss-Hermite quadrature of order, 67 

Gauss-Hermite roots of order, 65 

Gamma-distributed random variable, 44 

Gatheral, J.G., 16, 229 

Gamma. See Variance gamma distribution, 41–42, 158, 172 dependence, 170 variables, 216 

Gallant, A.R., 229 

Gaussian approximation, 136 

Gaussian cases, 59 

Gaussian random variables, 97, 104 

Gaussian likelihood, maximization, 82 diffusion-limit model, 94, 121 

process, weak convergence, 21 

Galli, A., 96, 229, 231 

Gaussian quadrature, 65 

Gaussian realization, 40, 214 

diffusion, 137 

Gaussian SV models, MCMC application, 154–156 

MLE, 138 

Gelfand, A.E., 234 

Generalized Fourier transform, 2, 27–30 

Geman, H., 226, 229 

Generalized autoregressive conditional heteroskedasticity (GARCH), 1, 21–24 

Generic particle filter, 160–161, 179 

George, E.I., 226 

Geske, R., 229 

Ghyseles, E., 226, 229 

Gibbs sampler, 144–150, 154 

Gilks, W.R., 229 

Girsanov theorem, 25–26, 188, 213, 220 

Gondzio, J., 229 

Gordon, N., 224, 227 

Gordon, N.J., 229 

Gotsis, G.Ch., 227 

Gourieroux, C., 229, 230 

Grabbe, J.O., 230 

Greenberg, E., 226 

Grenander, U., 234 

Gunther, S., 233 

Hamilton, J.D., 159, 230 

Hammersley-Clifford theorem, 144 

Härdle, W., 199, 230 

Harris, L., 229 

Harvey, A.C., 135, 230 

Harvey-Ruiz-Shephard (HRS) method, 136, 139 

Haug, E.G., 230, 231 

Haykin, S., 67, 230 

Induction expression, 157 

Heaviside function, 16 

Hedge ratio usage, selection, 208 

Inference problem, 46 

Hedged portfolio, 6 

Henderson, R., 231 

Hermite polynomials, usage, 103 

Hessian matrix, 39 

Heston, S., 21, 230 

high-frequency data, 139–140 

Heston state-space model, 47 comparison, 120–127 EPF, application, 105–114 equation, 154–156 particle filtering, application, 105–114 results, 122–125 

High correlation, 209–213 

High volatility-of-volatility, 209–213 

observations, frequency, 140–141 

High-frequency data, 185–186 parameters, joint estimation, 132–133 

Hipp, C., 230 

Hirsa, A., 230 

Importance sampling technique, 99–100 

Inference tools 

Implied volatility term structure, 206–208 

Inverse gamma (IG) CDF, 152–153 

Ill-posed inversion problems, 18 

Ishida, I., 123, 228 

Historic correlation, 212 

Incomplete beta function (IBF), 151 

Ito’s lemma, usage, 2, 6, 26 

Inverse Fourier transform, 27 

Information matrix identity, 56 

Insurance selling strategy, 201 

Ito, K., 231 

Historic volatility, 3–4 

Hobson, D.G., 230 

Holmes, R., 224 

Honoré, P., 230 

Jackel, P., 19, 231 

Howison, S.D., 230, 231, 235 

Jackson, N., 231 

Jackwerth, A.C., 226 

Hughston, L.P., 230, 231 

Hull, J., 2, 6, 19, 30, 231 

Jackwerth, J.C., 198, 231 

Jacobian calculation, 62, 70, 73–74, 87 

Jacobian matrices, defining, 60–61 

Jacobs, K., 230 

Jacquier, E., 231 

Jarrow, R., 231 

Jasiak, J., 230 

Javaheri, A., 230, 231 

Jensen, G.R., 234 

Jex, M., 231 

Jha, S., 234 

Jiang, G.J., 231 

Johannes, M., 159, 228, 231 

Joint filter (JF), 68 time interval, interaction, 78–81 usage, 125 Joint filtering (JF), example, 69–75 Jones, C.S., 231 Julier, S.J., 231 Jump-based models, non-Gaussianity, 124 Jumps component, orthogonality, 167 diffusion, 7–10 model, usage, 198 introduction, 158–168 model, 158–160 numeric results, 167 parameters, 167 simulation, Srivastava approach, 166–167 

Kalman filter (KF) reapplication, 119 usage, 58–59, 86–87, 96, 102 Kalman gain, interpretation, 59, 61, 67 Kamal, M., 227 Kani, I., 14, 227 Karatzas, I., 2, 6, 231 Kennedy, P., 232 Kim, S., 232 Kirby, C., 228 Kitagawa, G., 232 Kleinow, T., 230 Klopfer, W., 234 Koopman, S.J., 234 Kou, S., 8, 232 Kouwenberg, R., 229 Krishnamurthy, V., 227 

Kullback-Leibler distance, 18, 55 Kurtosis, trades/trading, 200–203, 222 Kushner, H.J., 65, 232 Kushner algorithm, details, 66–67 Kushner filters, 98 Kushner’s nonlinear filter, 65–67 

Lagnado, R., 232 Lagrange multiplier, 18, 214 Lahaie, C.H., 228 Lautier, D., 229, 231 Least-square estimation (LSE) approach, 30, 53, 54 Least-square estimator (LSE), 46, 49 Lee, D.S., 232 Leptokurticity, 8 Level-dependent volatility, 7, 10–13 Levenberg-Marquardt (LM) method, 49 Leverage effect, 8, 22 parameter, 22, 26 Levy, A., 225 Levy process, 10 Lewis, Alan L., 2, 28–29, 34–38, 232 Lewis, K., 226 Li, Y., 232 Liability maturity, 12 Likelihood evaluation, 57 filtering, 57 function, 54–57, 129, 132 maximization, 81, 161 Line minimization routine, 49 Linear a posteriori estimate, 60 Linear state-space system, 68–69 

Litzenberger, R.H., 14, 226 

Local risk minimization, 27 

Local volatility, 14–19 instantaneous volatility, contrast, 16–17 stability issues, 18 

Log-normal process, 2 

Long, D., 226 

Long-term asymptotic example, 34–40 

Madan, D., 40–41, 215, 226, 228–229, 232 

Maes, K., 232 

Maheu, J.M., 159, 232 

Market completeness, 5 

Markov chain, creation, 144 

Markov chain Monte Carlo (MCMC), 144 algorithms, distributions (usage), 151–153 approaches, 154 step, addition, 101 

Markov process, 100 

Markov property, usage, 58 

Markowitz, H.M., 232 

Martin, G.M., 229 

Martingale, 16 

Maskell, S., 224 

Masoliver, J., 226 

Matacz, A., 232 

Matytsin, A., 232 

Maximum likelihood estimate (MLE), 18, 68, 88–89 

iteration, 82 

justification, 55–56 

McCurdy, T.H., 159, 232 

Mean price error (MPE), 62, 118 reduction, 185 usage, 179 

Mean-adjusted stock returns, 57 

Measurement equation, 87–88 noise, uncorrelation, 86–87 update equations, 61, 64, 66 

Merton, R.C., 8, 199, 233 

Metropolis-Hastings (MH) accept/reject technique, 126–127, 156 

Metropolis-Hastings (MH) algorithm, 144, 147–150 enhancement, 119–120 example, 150–151 

Metropolis-Hastings (MH) density, 149 

Metropolis-Hastings (MH) modification, 120 

Metropolis-Hastings (MH) sampling algorithm, 101 

Meyer, R., 233 

Mezrich, J., 228 

MH. See Metropolis-Hastings 

Miller, M.I., 234 

Mirror trades, 203 

Mixing solutions, 30–33 

Models, identification, 120–121, 185 

Modified model, 80 

Monfort, A., 229 

Monte Carlo algorithm, 222 

Monte Carlo approximation, 102 

Monte Carlo method, usage, 50 

Monte Carlo mixing, 193 

Monte Carlo process, obtaining, 23 

Monte Carlo sampling, usage, 100 

Monte Carlo simulation, 32–33, 98, 169 Monte Carlo time steps, 190 Monte Carlo-based models, 2 Multiple trades, 208–209 Muzzioli, S., 233 Mykland, P.A., 235 

Nadari, F., 226 Nandi, S., 21, 230 Neftci, S.N., 233 Nelson, D.B., 233 Ng, V., 224, 228 Nicolato, E., 225 No-default case, 10 Noise drift, 167 one-dimensional source, 73 Non-Gaussian case, 213–218 Non-Gaussian filters, 160 Non-Gaussian pure jump model, 47 Non-Gaussianity, 179 Nonlinear asymmetric GARCH (NGARCH), 22 Nonlinear filter (NLF), 65, 103, 121 Nonlinear Gaussian KF, 161 Nonlinear PDE, 13 Nonlinear transition equation, 60 Numeric tests, 50, 183 

Observation error, 178–179 matrix, 83–84, 87 noise, 75 Oksendal, B., 2, 233 One-dimensional EKF/UKF, 96 One-dimensional Heston model, 114–115 

One-dimensional state, 87–94 joint filter, inclusion, 76–78 One-factor diffusion process, 138 One-factor Monte Carlo technique, 32–33 Optimization algorithm, 168 weakness, 127–128 Option prices, usage, 49–54 Option pricing, cross section, 221–223 Options bid-ask spread, 205–206 maturity, 6 time-to-maturities, decrease, 208 Ornstein-Uhlenbeck (OU) process, 20 Osher, S., 232 Out-of-the-money (OTM) options, 200 puts/calls, usage, 188, 209 region, Black-Scholes value, 38 

Pan, G., 233 Pan, J., 233 Papanicolaou, G., 229 Parameter estimation, 217. See also Pure jump models MLE usage, 81–94 example, 82–83 implementation, alternate, 86–87 Parameter learning, 67–81, 125–127 example, 68–69 Parametric SV, 20 Paras, A., 225 Parkinson, M., 3, 233 

Partial differential equation (PDE). See Black-Scholes PDE; Nonlinear PDE; Two-factor PDE pricing, stochastic volatility (impact), 24–27 risk-neutral version, 2 Particle filter (PF) algorithm, writing, 169–170 implementation, 160 Particle filtering, 98–120 algorithm, application, 121–122 application. See Heston space-state model error size, 116–119 example, 104–105 implementation, 103–104 resampling, 101–103 test results, 114–116 theory, 99–101, 117 Pearson kurtosis, 22 Pedersen, A.R., 233 Penny stocks, skew, 209 Perelló, J., 226 Peso theory, 197–199 background, 197–198 numeric results, 199 Pham, H., 233 Phantom profits, creation, 19 Pitt, M.K., 233 Poisson jumps, 159 Poisson process, 8–9 Poisson random variable, 9 Polson, N.G., 159, 228, 231 Powell algorithm, application, 50 Press, W.H., 31, 50, 233 Prucyk, B., 234 Pure diffusion, 7–9 parameter, 199 

Pure jump models, 40–45, 168–184, 215 algorithms, usage, 170–172 diagnostics, 178–179 filtering algorithm, usage, 169–170 numeric results, 176–178 parameter estimation, 170 

Quenez, M.C., 27, 228 

Rafailidis, A., 230, 231 Randall, C., 234 Rasmussen, H.O., 230 Regression analysis, 153 Reif, K., 233 Rejection probability, 149 Renault, E., 229, 233 Resampling algorithm, 101 Residuals, 62 Reverse Black-Scholes equation, solving, 7 Reversibility condition, 149–150 Ribiero, C., 233 Richardson, S., 229 Ridge property, 36 Risk, market price, 25 Riskless arbitrage, 6 Risk-neutral GARCH system, 26 Risk-neutral implied parameter, 190 Risk-neutral parameters, 215 Risk-neutral pricing formula. See Black-Scholes risk-neutral pricing formula Ritchken, P., 234 Robustness, issues. See Consistency test; Time-series method Rochet, J.C., 229 

Rogers, L.C.G., 230 

Romano, M., 32, 234 

Romano-Touzi approach, 30–32 

Root mean square error (RMSE), 62, 118 reduction, 185 usage, 179 

Ross, S., 227 

Rossi, P.E., 231 

Rubinstein, M., 198, 227, 231, 234 

Rudd, A., 231 

Ruiz, E., 135, 230 

Salmond, D.J., 229 

Samperi, D., 224 

Sample impoverishment, 119 

Samuelson, P. A., 2, 234 

Sandmann, G., 234 

Santa-Clara, P., 226 

Scholes, M., 225 

Schonbucher, P.J., 234 

Scott, L.O., 234 

Self-financing portfolio argument, usage, 214–215 

Sequential importance sampling, 100 

Shephard, N., 135, 225, 226, 228, 232, 233 

Shimko, D., 234 

Shreve, S., 6, 21, 231, 234 

Signal-to-noise ratio (SNR), 138 

Silva, A.C., 234 

Simple Kalman filter, 59–62 

Sin, C.A., 234 

Single calibration (SC) methodology assumption, 19 

Sircar, K., 229 

Skewness kurtosis, contrast, 201–202 

Smith, A.F.M., 225, 229, 234 

Sondermann, D., 228 

Spiegelhalter, D.J., 229 

Spot prices, observation, 183 

Spread. See Options bid-ask spread 

Square root model, optimization constraints, 85–86 

Square root SDE, 184 

Square root SV model, 37, 69–70 

Srivastava, A., 166, 234 

Srivastava approach. See Jumps 

Stability issues. See Local volatility 

Stahl, G., 230 

Standard & Poor’s (S&P), 208 options, 189, 198 S&P 500, 204, 216–218 Stock Index, 4 

Stein, E.M., 234 

Stein, J., 234 

Stochastic differential equation (SDE), 197–198, 221 

Stochastic volatility (SV), 20–24 behavior, 24 

example, 35–37, 83–85 

formulation, 76 

impact. See Partial differential equation 

problem, 78–79 

processes, 20–21 

time-changed processes, contrast, 42–43 

Stochastic volatility (SV) models, 94, 136 

embedded parameters, inference (problem), 48 

Heston state-space model, comparison, 121–122 

parameters, 196 

Stock forward price, 17 Stock log return density, 40 Stock market, 2–4 Stock prices movement, log-normal model, 5 process, 2–3 stochastic differential equation, 159 time series, 176 usage, 54 Stock process, noise (representation), 133–135 Storvik, G., 234 Strike prices, 6, 187 Stroud, J., 159, 231 Student’s law of mean, 155 Su, T., 227 Suli, E., 231 Sundaram, R.K., 227 Suo, W., 231 Super-replication, 27 SV. See Stochastic volatility 

Taksar, M., 230 Taleb, N., 234 Tauchen, G., 229 Tavella, D., 234 Taylor approximation, usage, 35–36 Taylor expansion, usage, 36 Teukolsky, S.A., 233 Time series, 116, 220–221 usage, 48 Time update equations, 61–65 Time-independent parameters, 33 Time-series implied parameters, 190 Time-series method, robustness issues, 193–194 Time-series results, 193–194 

Toft, K.B., 234 Torricelli, C., 233 Touzi, N., 32, 233, 234 Trading strategies, 199–213 replication, 202–203 Transform. See Generalized Fourier transform special cases, 28–30 technique, 27–28 Transition noise, 140 Trevor, R., 234 Trinomial tree, usage, 17 Tullie, T.A., 229 Two-factor Monte Carlo simulation, application, 26 Two-factor PDE, 26–27 

Uhlmann, J.K., 231 Uncertain volatility, concept, 20 Univariate regression, 153 Unscented Kalman filter (UKF), 62–65, 88, 161–162 algorithm, 66 application, 172–173 implementation, 77 Unscented particle filter (UPF), 102, 161–166 

Van der Merwe, R., 115, 235 Van der Sluis, P.J., 231 Varadhan, S.R.S., 235 Variance equation, writing, 7 Variance gamma (VG), 40–43 characteristic function, 44–45 model, 168–169 parameters, 178 usage, 182 

Variance gamma with gamma arrival rate (VGG), 45, 158, 166 usage, 181–183 Variance gamma with stochastic arrival (VGSA), 43–45, 169, 215 Bayesian approach, 184 EPF application, 173–176 model, 168 option pricing, 44 VG, contrast, 215–216 Variograms, 96–98 usage, 181 Vetterling, W.T., 233 Volatility. See Historic volatility; Level-dependent volatility; Local volatility; Stochastic volatility clustering effect, 43 curve, 200 dependence, discovery, 11 drift, 25 parameters, 213 perception, 7 problem, 1 risk, market price, 25–26, 47 term structure. See Implied volatility term structure usage, 2 value, 3 Volatility-of-volatility, 202. See also High volatility-of-volatility 

parameter, 192, 194 series expansion, 37–40 series method, 191 Vorst, T., 229 

Wan, E.A., 115, 235 Wang, D., 231 Webber, N., 233 Weights, 160–162 calculation, 171–172, 182 normalization, 170 Welch, G., 235 Wells, C., 235 Whaley, R.E., 189, 228 White, A., 30, 231 Whitt, W., 235 Wiggins, J.B., 235 Wilmott, P., 7, 231, 235 Wright, J., 229 Wu, L., 226 

Xiong, K., 231 

Yakovenko, V.M., 158, 228, 234 Yao, Q., 228 Yaz, A., 233 You, M., 226, 229 

Zellner, A., 235 Zero-coupon risky bond, 10 Zhang, L., 235 Zhou, C., 235 Zou, J., 227 