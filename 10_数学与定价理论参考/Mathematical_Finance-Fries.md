

<!-- === Source: MinerU_markdown_Mathematical_Finance-Fries_1_2122706940055363588.md (Page 1) === -->

# Mathematical Finance Theory, Modeling and Implementation

Christian P. Fries 

Stochastic Processes • Interest Rate Structures • Hybrid Models Numerical Methods • Object Oriented Implementation 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/71c548766d1bc4a43374252d5bb2a34f089aa1d81e871131f6473c1d32d97438.jpg)


$$
\begin{array}{r l} & {\mathsf {d} L _ {j} (t) = \quad L _ {j} (t) \cdot \mu_ {j} (t) \mathsf {d} t + L _ {j} (t) \cdot \sigma_ {j} (t) \mathsf {d} W _ {j}} \\ & {\mathsf {d} F X (t) = F X (t) \cdot \mu^ {F X} (t) \mathsf {d} t + F X \cdot \sigma^ {F X} (t) \mathsf {d} W ^ {F X}} \\ & {\mathsf {d} \tilde {L} _ {j} (t) = \quad \tilde {L} _ {j} (t) \cdot \tilde {\mu} _ {j} (t) \mathsf {d} t + \tilde {L} _ {j} (t) \cdot \tilde {\sigma} _ {j} (t) \mathsf {d} \tilde {W} _ {j}} \end{array}
$$

$$
\begin{array}{r l} & {\mu_ {j} (t) = \sum_ {\beta (t) \leq l \leq j} \frac {L _ {l} \delta_ {l}}{(1 + L _ {l} \delta_ {l})} \cdot \sigma_ {j} (t) \sigma_ {l} (t) \rho_ {j, l}} \\ & {\int_ {T _ {i}} ^ {T _ {i + 1}} \mu^ {F X} (t) \mathsf {d} t = \log \left(\frac {1 + L _ {i} (T _ {i}) \delta_ {i}}{1 + \tilde {L} _ {i} (T _ {i}) \delta_ {i}}\right)} \\ & {\tilde {\mu} _ {j} (t) = \sum_ {\beta (t) \leq l \leq j} \frac {\tilde {L} _ {l} \delta_ {l}}{(1 + \tilde {L} _ {l} \delta_ {l})} \cdot \tilde {\sigma} _ {j} (t) \tilde {\sigma} _ {l} (t) \rho_ {j, l} - \tilde {\sigma} _ {j} (t) \sigma^ {F X} (t) \rho_ {\tilde {j}, F X} (t)} \end{array}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/cd17532dc8b1d025eb755520e48d073165d965f7207c6ac1b88445546354e365.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/4544444ee3511b7a758a685395df926d72b290af93e0c308236e50206c856ad3.jpg)


# Mathematical Finance Theory, Modeling and Implementation

Stochastic Processes, Interest Rate Models, Hybrid Models, Numerical Methods, Object Oriented Implementation 

Christian P. Fries 

1st May 2007 

preliminary, uncorrected and incomplete version (public beta) 

Oscar Wilde The Picture ofDorian Gray, [38]. 

Typeset by the author using TeXShop for Mac OS X™. Drawings by the author using OmniGrafle for Mac OS X™. Charts created using Java™ Code by the author. 

## Licence

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/2f6253aaf51ecec8f85c9a7a3366659251e3589e61f90412c926e061b8b8b39b.jpg)


This work is licensed under Creative Commons License. 

Lizensiert fuer <ayonbd2000@yahoo.com> (Muntasir Hasan) 

## Suggested citation

FRIEs, CHRIsTIAN P.: Mathematical Finance: Theory, Modeling, Implementation. Frankfurt am Main, 2007. 

http://www.christian-fries.de/finmath/book. 

## Feedback

Please help to improve this work! 

Please send error reports and suggestions to 

Christian Fries email@christian-fries.de 

Thank you. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/cf4850aa4739a66a317b6a74b77a59c53ffb67cc9a93db4f7858ab3be9f9834c.jpg)


Among all replies we will rafle an iPod nano. Your winning chance will be approximately proportional to the number of errors or suggestions sent in. 

Due date is 30 September 2007. 

## Resources

In connection with this book the following resources are available: 

• Interactive experiments and exercises: 

http://www.christian-fries.de/finmath/applets 

• Updates: For updates and error corrections see 

http://www.christian-fries.de/finmath/book 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/4159ea88948914aa4450901026791915ffdb34f96ecc597660c49f48b5716870.jpg)


## Picture Credits

All figures are © copyright Christian Fries except the special section icons (see Section 1.3.2) licensed through iStockphoto.com. 

## Note

This book is also available in German, see 

http://www.christian-fries.de/finmath/book 

## Acknowledgement

I am grateful to Andreas Bahmer, Hans-Josef Beauvisage, Michael Belledin, Dr. Urs Braun, Oliver Dauben, Peter Dellbrugger, Dr. J¨ org Dickersbach, Sinan Dikmen, Dr. Dirk Ebmeyer,¨ Fabian Eckstadt, Dr. Lydia Fechner, Christian Ferber, Frank Genheimer, Dr. Gido Herbers,¨ Prof. Dr. Ansgar Jungel, Dr. Christoph Kiehn, JProf. Dr. Christoph K¨ uhn, Dr. J¨ urgen Linde,¨ Markus Meister, Dr. Sean Matthews, Dilys and Bill McCann, Michael Paulsen, Matthias Peter, Dr. Erwin Pier-Ribbert, Rosemarie Philippi, Dr. Radu Tunaru, Frank Ritz, Marius Rott, Thomas Schwiertz, Arndt Unterweger, Benedikt Wilbertz, Andre Woker, Polina Zeydis, and Jorg Zinnegger.¨ 

Their support and their feedback as well as the stimulating discussions we had contributed significantly to this work. 

I am most grateful to my wife and my family. I thank them for their continuous support and generous tolerance. 

## Contents

1 Introduction 15
1.1 Theory, Modeling and Implementation 15
1.2 Interest Rate Models and Interest Rate Derivatives 15
1.3 How to Read this Book 15
1.3.1 Abridged Versions 16
1.3.2 Special Sections 16
1.3.3 Notation 18

I Foundations 19

2 Foundations 21
2.1 Probability Theory 21
2.2 Stochastic Processes 28
2.3 Filtration 30
2.4 Brownian Motion 31
2.5 Wiener Measure, Canonical Setup 33
2.6 Itô Calculus 34
2.6.1 Itô Integral 36
2.6.2 Itô Process 38
2.6.3 Itô Lemma and Product Rule 40
2.7 Brownian Motion with Instantaneous Correlation 43
2.8 Martingales 44
2.8.1 Martingale Representation Theorem 44
2.9 Change of Measure (Girsanov, Cameron, Martin) 45
2.10 Stochastic Integration 49
2.11 Partial Differential Equations (PDE) 50
2.11.1 Feynman-Kač Theorem 50
2.12 List of Symbols 52

3 Replication 53
3.1 Replication Strategies 53
3.1.1 Introduction 53
3.1.2 Replication in a discrete Model 56
3.2 Foundations: Equivalent Martingale Measure 60
3.2.1 Challenge and Solution Outline 60 

3.2.2 Steps towards the Universal Pricing Theorem 62
3.3 Excursus: Relative Prices and Risk Neutral Measures 70
3.3.1 Why relative prices? 70
3.3.2 Risk Neutral Measure 71

II First Applications 73

4 Pricing of a European Stock Option under the Black-Scholes Model 75
5 Excursus: The Density of the Underlying of a European Call Option 79
6 Excursus: Interpolation of European Option Prices 81
6.1 No-Arbitrage Conditions for Interpolated Prices 81
6.2 Arbitrage Violations through Interpolation 82
6.2.1 Example (1): Interpolation of four Prices 82
6.2.2 Example (2): Interpolation of two Prices 85
6.3 Arbitrage-Free Interpolation of European Option Prices 86

7 Hedging in Continuous and Discrete Time and the Greeks 89
7.1 Introduction 89
7.2 Deriving the Replications Strategy from Pricing Theory 90
7.2.1 Deriving the Replication Strategy under the Assumption of a Locally Riskless Product 91
7.2.2 The Black-Scholes Differential Equation 92
7.2.3 The Derivative V(t) as a Function of its Underlyings Si(t) 92
7.2.4 Example: Replication Portfolio and PDE under a Black-Scholes Model 93
7.3 Greeks 96
7.3.1 Greeks of a european Call-Option under the Black-Scholes model 97
7.4 Hedging in Discrete Time: Delta and Delta-Gamma Hedging 97
7.4.1 Delta Hedging 98
7.4.2 Error Propagation 99
7.4.3 Delta-Gamma Hedging 102
7.4.4 Vega Hedging 105
7.5 Hedging in Discrete Time: Minimizing the Residual Error (Bouchaud-Sornette Method) 107
7.5.1 Minimizing the Residual Error at Maturity T 108
7.5.2 Minimizing the Residual Error in each Time Step 109

III Interest Rate Structures, Interest Rate Products and Analytic Pricing Formulas 111

Motivation and Overview 113

8 Interest Rate Structures 115
8.1 Introduction 115 

8.1.1 Fixing Times and Tenor Times 115
8.2 Definitions 116
8.3 Interest Rate Curve Bootstrapping 120
8.4 Interpolation of Interest Rate Curves 121
8.5 Implementation 122

9 Simple Interest Rate Products 123
9.1 Interest Rate Products Part 1: Products without Optionality 123
9.1.1 Fix, Floating and Swap 123
9.1.2 Money-Market Account 129
9.2 Interest Rate Products Part 2: Simple Options 130
9.2.1 Cap, Floor, Swaption 130
9.2.2 Foreign Caplet, Quanto 132

10 The Black Model for a Caplet 133

11 Pricing of a Quanto Caplet (Modeling the FFX) 135
11.1 Choice of Numéraire 135

12 Exotic Derivatives 139
12.1 Prototypical Product Properties 139
12.2 Interest Rate Products Part 3: Exotic Interest Rate Derivatives 141
12.2.1 Structured Bond, Structured Swap, Zero Structure 141
12.2.2 Bermudan Option 145
12.2.3 Bermudan Callable and Bermudan Cancelable 146
12.2.4 Compound Options 148
12.2.5 Trigger Products 148
12.2.6 Structured Coupons 150
12.2.7 Shout Options 153
12.3 Product Toolbox 154

IV Discretization and Numerical Valuation Methods 157
Motivation and Overview 159

13 Discretization of time and state space 161
13.1 Discretization of Time: The Euler and the Milstein Scheme 161
13.1.1 Definitions 161
13.1.2 Time-Discretization of a Lognormal Process 164
13.2 Discretization of Paths (Monte-Carlo Simulation) 165
13.2.1 Monte-Carlo Simulation 166
13.2.2 Weighted Monte-Carlo Simulation 166
13.2.3 Implementation 167
13.2.4 Review 171
13.3 Discretization of State Space 172
13.3.1 Definitions 172
13.3.2 Backward-Algorithm 174 

13.3.3 Review 174
13.4 Path Simulation through a Lattice: Two Layers 174

14 Numerical Methods for Partial Differential Equations 177

15 Pricing Bermudan Options in a Monte-Carlo Simulation 179
15.1 Introduction 179
15.2 Bermudan Options: Notation 179
15.2.1 Bermudan Callable 180
15.2.2 Relative Prices 181
15.3 Bermudan Option as Optimal Exercise Problem 181
15.3.1 Bermudan Option Value as single (unconditioned) Expectation: The Optimal Exercise Value 182
15.4 Bermudan Option Pricing - The Backward Algorithm 182
15.5 Re-simulation 183
15.6 Perfect Foresight 184
15.7 Conditional Expectation as Functional Dependence 185
15.8 Binning 186
15.8.1 Binning as a Least-Square Regression 188
15.9 Foresight Bias 189
15.10 Regression Methods - Least Square Monte-Carlo 190
15.10.1 Least Square Approximation of the Conditional Expectation 190
15.10.2 Example: Evaluation of a Bermudan Option on a Stock (Backward Algorithm with Conditional Expectation Estimator) 191
15.10.3 Example: Evaluation of a Bermudan Callable 192
15.10.4 Implementation 196
15.10.5 Binning as linear Least-Square Regression 197
15.11 Optimization Methods 198
15.11.1 Andersen Algorithm for Bermudan Swaptions 198
15.11.2 Review of the Threshold Optimization Method 199
15.11.3 Optimization of Exercise Strategy: A more general Formulation 201
15.11.4 Comparison of Optimization Method and Regression Method 201
15.12 Duality Method: Upper Bound for Bermudan Option Prices 202
15.12.1 Foundations 202
15.12.2 American Option Evaluation as Optimal Stopping Problem 204
15.13 Primal-Dual Method: Upper and Lower Bound 207

16 Pricing Path Dependent Options in a Backward Algorithm 209
16.1 State Space Extension 209
16.2 Implementation 210
16.3 Examples 210
16.3.1 Evaluation of a Snowball in a Backward Algorithm 210
16.3.2 Evaluation of a Flexi Cap in a Backward Algorithm 211

17 Sensitivities (Partial Derivatives) of Monte-Carlo Prices 213
17.1 Introduction 213
17.2 Problem Description 213
17.2.1 Pricing using Monte-Carlo Simulation 214 

17.2.2 Sensitivities from Monte-Carlo Pricing 214
17.2.3 Example: The Linear and the Discontinuous Payout 215
17.2.4 Example: Trigger Products 216
17.3 Generic Sensitivities: Bumping the Model 216
17.4 Sensitivities by Finite Differences 219
17.4.1 Example: Finite Differences applied to Smooth and Discontinuous Payout 220
17.5 Sensitivities by Pathwise Differentiation 221
17.5.1 Example: Delta of a European Option under a Black-Scholes Model 222
17.5.2 Pathwise Differentiation for Discontinuous Payouts 222
17.6 Sensitivities by Likelihood Ratio Weighting 223
17.6.1 Example: Delta of a European Option under a Black-Scholes Model using Pathwise Derivative 223
17.6.2 Example: Variance Increase of the Sensitivity when using Likelihood Ratio Method for Smooth Payouts 224
17.7 Sensitivities by Malliavin Weighting 224
17.8 Proxy Simulation Scheme 225

18 Proxy Simulation Schemes for Monte-Carlo Sensitivities and Importance Sampling 227
18.1 Full Proxy Simulation Scheme 227
18.1.1 Calculation of Monte-Carlo weights 228
18.2 Sensitivities by Finite Differences on a Proxy Simulation Scheme 229
18.2.1 Localization 229
18.2.2 Object-Oriented Design 230
18.3 Importance Sampling 230
18.3.1 Example 230
18.4 Partial Proxy Simulation Schemes 233
18.4.1 Linear Proxy Constraint 233
18.4.2 Comparison to Full Proxy Scheme Method 234
18.4.3 Non-Linear Proxy Constraint 234
18.4.4 Transition Probability from a Nonlinear Proxy Constraint 235
18.4.5 Sensitivity with respect to the Diffusion Coefficients – Vega 238
18.4.6 Example: LIBOR Target Redemption Note 238
18.4.7 Example: CMS Target Redemption Note 239

V Pricing Models for Interest Rate Derivatives 243

19 Market Models 245
19.1 LIBOR Market Model 245
19.1.1 Derivation of the Drift Term 247
19.1.2 The Short Period Bond $P(T_{m(t)+1};t)$ 252
19.1.3 Discretization and (Monte-Carlo) Simulation 253
19.1.4 Calibration - Choice of the free Parameters 254
19.1.5 Interpolation of Forward Rates in the LIBOR Market Model 259
19.2 Object Oriented Design 263 

19.2.1 Reuse of Implementation . 263
19.2.2 Separation of Product and Model . 264
19.2.3 Abstraction of Model Parameters . 264
19.2.4 Abstraction of Calibration . 265
19.3 Swap Rate Market Models (Jamshidian 1997) . 266
19.3.1 The Swap Measure . 267
19.3.2 Derivation of the Drift Term . 268
19.3.3 Calibration - Choice of the free Parameters . 268

20 Excursus: Instantaneous Correlation and Terminal Correlation 271
20.1 Definitions . 271
20.2 Terminal Correlation examined in a LIBOR Market Model Example . 272
20.2.1 De-correlation in a One-Factor Model . 274
20.2.2 Impact of the Time Structure of the Instantaneous Volatility on Caplet and Swaption Prices . 274
20.2.3 The Swaption Value as a Function of Forward Rates . 274
20.3 Terminal Correlation is dependent on the Equivalent Martingale Measure . 276
20.3.1 Dependence of the Terminal Density on the Martingale Measure . 277

21 Heath-Jarrow-Morton Framework: Foundations 279
21.1 Short Rate Process in the HJM Framework . 280
21.2 The HJM Drift Condition . 280

22 Short Rate Models 283
22.1 Introduction . 283
22.2 The Market Price of Risk . 284
22.3 Overview: Some Common Models . 285
22.4 Implementations . 286
22.4.1 Monte-Carlo Implementation of Short-Rate Models . 286
22.4.2 Lattice Implementation of Short-Rate Models . 286

23 Heath-Jarrow-Morton Framework: Immersion of Short Rate Models and LIBOR Market Model 287
23.1 Short Rate Models in the HJM Framework . 287
23.1.1 Example: The Ho-Lee Model in the HJM Framework . 287
23.1.2 Example: The Hull-White Model in the HJM Framework . 288
23.2 LIBOR Market Model in the HJM Framework . 289
23.2.1 HJM Volatility Structure of the LIBOR Market Model . 289
23.2.2 LIBOR Market Model Drift under the $\mathbb{Q}^B$ Measure . 291
23.2.3 LIBOR Market Model as a Short Rate Model . 292

24 Excursus: Shape of the Interest Rate Curve under Mean Reversion and a Multi-Factor Model 295
24.1 Model . 295
24.2 Interpretation of the Figures . 296
24.3 Mean Reversion . 296
24.4 Factors . 297
24.5 Exponential Volatility Function . 299 

24.6 Instantaneous Correlation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 301   
25 Markov Functional Models 303   
25.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . 303   
25.1.1 The Markov Functional Assumption (independent of the model considered) . . . . . . . . . . . . . . . . . 304   
25.1.2 Outline of this Chapter . . . . . . . . . . . . . . 304   
25.2 Equity Markov Functional Model. 305   
25.2.1 Markov Functional Assumption 305   
25.2.2 Example: The Black-Scholes Model 306   
25.2.3 Numerical Calibration to a Full Two-Dimensional European Option Smile Surface 306   
25.2.4 Interest Rates 308   
25.2.5 Model Dynamics 309   
25.2.6 Implementation 313   
25.3 LIBOR Markov Functional Model 313   
25.3.1 LIBOR Markov Functional Model in Terminal Measure 314   
25.4 Implementation: Lattice 318   
25.4.1 Convolution with the Normal Probability Density 318   
25.4.2 State space discretization 320   
VI Extended Models 323   
26 Hybrid Models 325   
26.1 Cross Currency LIBOR Market Model 325   
26.1.1 Derivation of the Drift Term under Spot-Measure 326   
26.1.2 Implementation 329   
26.2 Equity Hybrid LIBOR Market Model 329   
26.2.1 Derivation of the Drift Term under Spot-Measure 330   
26.2.2 Implementation 331   
26.3 Equity-Hybrid Cross-Currency LIBOR Market Model 331   
26.3.1 Summary 333   
26.3.2 Implementation 334   
VII Implementation 335   
27 Object-Oriented Implementation in $\mathbf{Java}^{\mathrm{TM}}$ 337   
27.1 Elements of Object Oriented Programming: Class and Objects 337   
27.1.1 Example: Class of a Binomial Distributed Random Variable 338   
27.1.2 Constructor 339   
27.1.3 Methods: Getter, Setter, Static Methods 340   
27.2 Principles of Object Oriented Programming 341   
27.2.1 Encapsulation and Interfaces 341   
27.2.2 Abstraction and Inheritance 344 

27.2.3 Polymorphism 346  
27.3 Example: A Class Structure for One Dimensional Root Finders 347  
27.3.1 Root Finder for General Functions 347  
27.3.2 Root Finder for Functions with Analytic Derivative: Newton Method 349  
27.3.3 Root Finder for Functions with Derivative Estimation: Secant Method 349  
27.4 Anatomy of a Java™ Class 353  
27.5 Libraries 353  
27.5.1 Java™ 2 Platform, Standard Edition (j2se) 353  
27.5.2 Java™ 2 Platform, Enterprise Edition (j2ee) 354  
27.5.3 Colt 354  
27.5.4 Commons-Math: The Jakarta Mathematics Library 354  
27.6 Some Final Remarks 354  
27.6.1 Object Oriented Design (OOD) / Unified Modeling Language (UML) 354 

## VIII Appendix

A Tools (Selection) 359  
A.1 Linear Regression . 359  
A.2 Generation of Random Numbers . 360  
A.2.1 Uniform Distributed Random Variables . 360  
A.2.2 Transformation of the Random Number Distribution via the In-verse Distribution Function . 360  
A.2.3 Normal Distributed Random Variables . 360  
A.2.4 Poisson Distributed Random Variables . 361  
A.2.5 Generation of Paths of an n-dimensional Brownian Motion . 361  
A.3 Factor Decomposition - Generation of Correlated Brownian Motion . 363  
A.4 Factor Reduction . 364  
A.5 Optimization (one-dimensional): Golden Section Search . 367  
A.6 Convolution with Normal Density . 368  

B Exercises 369  
C List of Symbols 375  
D Java™ Source Code (Selection) 377  
D.1 Java™ Classes for Chapter 27 . 377  

List of Figures 380  
List of Tables 383  
List of Listings 385  
Bibliography 387 

## Introduction

## 1.1. Theory, Modeling and Implementation

This book tries to give a balanced representation of the theoretical foundations of mathematical finance, especially derivative pricing, state of the art models, which are actually used in practice, and their implementation. 

In practice, none of the three aspects theory, modeling and implementation can be considered alone. Knowledge of the theory is worthless if it isn’t applied. Theory provides the tools for consistent modeling. A model without implementation is essentially worthless. Good implementation requires a deep understanding of the model and the underlying theory. 

With this in mind, the book tries to build a bridge from academia to practice and from theory to object-oriented implementation. 

## 1.2. Interest Rate Models and Interest Rate Derivatives

The text concentrates on the modeling of interest rates as stochastic (undetermined) quantities and the evaluation of interest rate derivatives under such models. However, this is not a specialization! Although the mathematical modeling of stock prices was the historical starting point and interest rates were assumed to be constant, some important theoretical aspects are significant only for stochastic interest rates (e.g. the change of numeraire-technique). So for´ didactic reasons it is meaningful to start with interest rate models. Another reason to start with interest rate models is that interest rate models are the foundation of hybrid models. Since the numeraire, the reference asset, is most likely an interest rate related product, a need for´ stochastic interest rates implies the need to build upon an interest rate model, see Figures 1.1 and 1.2. We will do so in Chapter 26. Nevertheless, the first model studied will be, of course, the Black-Scholes model for a single stock, after we will move to stochastic interest rates. 

## 1.3. How to Read this Book

The text may be read in a non-linear way, i.e. the chapters have been kept as free-standing as possible. Chapter 2 provides the foundations in the order of their dependence. The reader familiar with the concepts of stochastic processes and martingales may skip the chapter and use it as reference only. To get a feeling for the mathematical concepts one should read the special sections Interpretation and Motivation. Readers familiar with programming and im plementation may prefer Chapter 13 as an illustration of the basic concepts. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/010763d503b6bf470f74b29b16285b9fb5177a63bf81dc509abcc8659ad336e3.jpg)



Figure 1.1.: The num´eraire, the reference asset in the modeling of price processes, is most likely an interest rate product. This choice is not mathematically necessary, but common for almost all models. Interest rate processes are the natural starting pointfor the modeling ofprice processes.


The appendix gives a selection of the results and techniques from diverse areas (linear algebra, calculus, optimization) which are used in the text and in the implementation, but which are less important for understanding the essential concepts. 

## 1.3.1. Abridged Versions

For a crash course focusing on particular aspects some chapters may be skipped. What follows are a few suggestions in this direction. 

## 1.3.1.1. Abridged version “Monte-Carlo pricing”

Foundations (Ch. 2) → Replication (Ch. 3) → Black-Scholes Model (Ch. 4) → Discretization / Monte-Carlo Simulation (Ch. 13) 

## 1.3.1.2. Abridged version “LIBOR Market Model”

Foundations (Ch. 2) → Replication (Ch. 3) → Interest Rate Structures (Ch. 8) 

→ Black Model (Ch. 10) → LIBOR Market Model (Ch. 19) 

→ Instantaneous and Terminal Correlation (Ch. 20) 

→ Shape of the Interest Rate Curve (Ch. 24) 

## 1.3.1.3. Abridged version “Markov Functional Model”

Foundations (Ch. 2) → Replication (Ch. 3) → Interest Rate Structures (Ch. 8) 

→ Black Model (Ch. 10) → The Density of the Underlying of a European Option (Ch. 5) 

→ Markov Functional Models (Ch. 25) 

## 1.3.2. Special Sections

The text contains special sections giving notes on interpretation, motivation and practical aspects. These are marked by the following symbols: 


Black-Scholes Model


<table><tr><td>Equity Model</td><td>dS = μ S dt + σ S dW(t)</td></tr><tr><td>Interest Rate Model</td><td>dB = r B dt</td></tr></table>

Equity Hybrid LIBOR Market Model 

<table><tr><td>Equity Model</td><td>dS = μ S dt + σ S dW(t)</td></tr><tr><td>Interest Rate Model</td><td>dLi = μi Li dt + σi Li dWi(t)</td></tr></table>


Figure 1.2.: The Black-Scholes model may be interpreted as a hybrid model with deterministic interest rates. The solution of dB(t) = rB(t)dt is B(0) · exp(r · t), i.e. it is deterministic and given in closedform. Thus the interest rate component is trivial. Within a LIBOR Market Model the interest rate is a stochastic quantity. This also changes properties of the stock process.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/d496a7672fbbb57d293b5f3c16107a418f602940856573ad01400092006083e3.jpg)


Interpretation: Provides an interpretation of the preceding topic. Casts light on purposes and practical aspects. C| 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/676461700fc37821926964b602ae10cbfa1d7fbd597f754362884ff0c8fb67e8.jpg)


Motivation: Provides motivation for the following topic. Sometimes notes deficiencies in the previous results. C| 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/5352872d5208f6ccd30f74f35f652c0e80f9bbafd17047fa0d365445b82654c2.jpg)


Further Reading: Suggested literature and associated topics. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/19989a0dbb1be8090512d51f9965584bee544baf38668e9b45fce8183eca1663.jpg)


Experiment: Guidefor a software experiment where aspects ofthe preceding topic can be explored. C| 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/68f795b97993af20091e3397f7f279fa8e8757ac7d7736741a790a0f738ba4e3.jpg)


Tip: Hints for practical use and software implementation of the preceding topics. C| 

## 1.3.3. Notation

We will model the time evolution of stocks or interest rates with random variables parametrized through a time parameter t. Such stochastic processes may depend on other parameters like maturity or interest rate period. We will separate these two diferent kinds of parameters by a semicolon - see Figure 1.3. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/b30ce56c3c3a6a2b9e56ed39fb750edd0b9e2a7c994e8f3ed4cce784940f7286.jpg)



Figure 1.3.: On the notation


Part I. 

Foundations: Probability Theory, Stochastic Processes and Risk Neutral Evaluation 

## Foundations

## 2.1. Probability Theory

Definition 1 (Probability Space, <sub>σ</sub> Algebra): Let Ω denote a set and F a family of subsets of Ω. F is a <sub>σ</sub>-algebra if 

1. $\varnothing \in { \mathcal { F } }$ 

2. $F \in { \mathcal { F } } \Rightarrow \Omega \backslash F \in { \mathcal { F } }$ 

3. $F _ { 1 } , F _ { 2 } , F _ { 3 } , \ldots \in { \mathcal { F } } \Rightarrow \bigcup _ { i = 1 } ^ { \infty } F _ { i } \in { \mathcal { F } } .$ 

The pair $( \Omega , { \mathcal { F } } )$ is a measurable space. A function $P : \mathcal { F }  [ 0 , \infty )$ is a probability measure if 

1. $P ( \emptyset ) = 0 , P ( \Omega ) = 1 .$ 

2. For $F _ { 1 } , F _ { 2 } , F _ { 3 } , \ldots \in { \mathcal { F } }$ mutually disjoint $( \mathrm { i . e . ~ } i \ne j \implies F _ { i } \cap F _ { j } = \emptyset )$ , we have 

$$
P \left(\bigcup_ {i = 1} ^ {\infty} F _ {i}\right) = \sum_ {i = 1} ^ {\infty} P (F _ {i}).
$$

The triple $( \Omega , { \mathcal { F } } , P )$ is called probability space (if instead of 1 we require only $P ( \emptyset ) = 0$ then P is called measure and $( \Omega , { \mathcal { F } } , P )$ is called measure space). y 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/18be9ee68cbbf483e220e76a0aae95762f90e3d937e41b18b8c46662a78e0b79.jpg)


Interpretation: The set Ω may be interpreted as the set of elementary events. Only one such event may occur. The subset $F \subset \Omega$ may then be interpreted as an event configuration, e.g. as if one asked only for a specific property of an event, a property that might be shared by more than one event. Then the complement of a set of events corresponds to the negation of the property in question, and the union of two subset $F _ { 1 } , F _ { 2 } \subset \Omega$ corresponds to combining the questions for the two corresponding properties with an $\ " \mathrm { o r } ^ { \prime \mathrm { : } }$ . Likewise the intersection corresponds to an “and”: only those events that share both properties are part of the intersection. A -algebra may then be interpreted as a set of properties, e.g. the set of properties by which we may distinguish the events or the set of properties on which we may base decisions and answer questions. Thus the <sub>σ</sub>-algebra may be interpreted as information (on properties of events). 

Thus a probability space $( \Omega , { \mathcal { F } } , P )$ may be interpreted as a set of elementary events, a family of properties of the events and a map that assigns a probability to each property of the events, the probability that an event with the respective properties will occur. C| 

Since conditional expectation will be one of the central concepts, we remind the reader of the notions of conditional probability and independence: 

Definition 2 (Independence, Conditional Probability): Let (Ω F P) denote a probability space and $A , B \in { \mathcal { F } }$ 

1. We say that A and B are independent, if 

$$
P (A \cap B) = P (A) \cdot P (B).
$$

2. For $P ( B ) > 0$ we define the conditional probability ofA under the hypothesis B as 

$$
P (A | B) := \frac {P (A \cap B)}{P (B)}.
$$

The Borel <sub>σ</sub>-algebra B(R) or ${ \mathcal { B } } ( \mathbb { R } ^ { n } )$ plays a special role in integration theory. We define it next. 

## Definition 3 (Borel <sub>σ</sub> Algebra, Lebesgue Measure):

Let $n \in \mathbb { N }$ and $a _ { i } < b _ { i } ( i = 1 , \ldots , n )$ . By B(R<sup>n</sup>) we denote the smallest -algebra for which 

$$
(a _ {1}, b _ {1}) \times \dots \times (a _ {n}, b _ {n}) \in \mathcal {B} (\mathbb {R} ^ {n}).
$$

B(R<sup>n</sup>) is called the Borel <sub>σ</sub>-algebra. The measure λ defined on ${ \mathcal { B } } ( \mathbb { R } ^ { n } )$ with 

$$
\lambda \bigl ((a _ {1}, b _ {1}) \times \dots \times (a _ {n}, b _ {n}) \bigr) := \prod_ {i = 1} ^ {n} (b _ {i} - a _ {i})
$$

is called a Lebesgue measure on B(R<sup>n</sup>). 

Remark 4 (Lebesgue Measure): Obviously the Lebesgue measure is not a probability measure on $( \mathbb { R } ^ { n } , \mathcal { B } ( \mathbb { R } ^ { n } ) )$ since $\lambda ( \mathbb { R } ^ { n } ) = \infty$ . It will be needed in the discussion of Lebesgue integration and we give the definition merely for completeness.<sup>1</sup> 

## Definition 5 (Measurable, Random Variable):

Let $( \Omega , { \mathcal { F } } )$ and (S S) denote two measurable spaces. 

1. A map $T : \Omega \mapsto S$ is called $( { \mathcal { F } } , S )$ -measurable $\mathrm { i f } ^ { 2 }$ 

$$
T ^ {- 1} (A) \in \mathcal {F} \text {   for   all   } A \in \mathcal {S}.
$$

If $T : \Omega \mapsto S$ is a $( { \mathcal { F } } , S )$ -measurable map we write more concisely 

$$
T: (\Omega , \mathcal {F}) \mapsto (S, \mathcal {S}).
$$

<sup>1</sup> The Lebesgue measure measures intervals $( n = 1 )$ according to their length, rectangles $( n = 2 )$ according to their area and cubes $( n = 3 )$ according to their volume. 

<sup>2</sup> We define $T ^ { - 1 } ( A ) : = \left\{ \omega \in \Omega \mid T ( \omega ) \in A \right\}$ 

2. A measurable map $X : ( \Omega , { \mathcal { F } } ) \mapsto ( S , S )$ is also called a random variable. A random variable $X : ( \Omega , { \mathcal { F } } ) \mapsto ( S , S )$ is called a n-dimensional real-valued random variable if $S = \mathbb { R } ^ { n }$ and $\begin{array} { r } { { \cal S } = \mathcal { B } ( \mathbb { R } ^ { n } ) } \end{array}$ . 

We are interested in the probability for which a given random variable attains a certain value or range of values. This is given by 

## Definition 6 (Image Measure):

Let $X : ( \Omega , { \mathcal { F } } ) \mapsto ( S , S )$ denote a random variable and P a measure on the measureable space (Ω F). Then 

$$
P _ {X} (A) := P (X ^ {- 1} (A)) \quad \forall A \in \mathcal {S}
$$

defines a probability measure on (S S) which we call the image measure of P with respect to X. y 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/fb9f7b5de1d6238bd501a7586e76ee720b30828ab67f6e079851ee3e78adf747.jpg)


Interpretation: A real-valued random variable assigns a real value (or vector of values) to each elementary event <sub>ω</sub>. This value may be interpreted as the result of an experiment, depending on the events. In our context the random variables mostly stand for payments or values of financial products depending on the state 

of the world. How random a random variable is depends on the random variable itself. The random variable that assigns the same value to all events <sub>ω</sub> exhibits no randomness at all. If we could observe only the result of such an experiment (random variable) we would not be able to say anything about the state of the world that led to the result. 

The image measure is the probability measure induced by the probability measure P (a probability measure on (Ω F )) and the map X on the image space (S S). 

The property of being measurable may be interpreted as the property that the distinguishable events in the image space (S S) are not finer (better distinguishable) than the events in the preimage space (Ω F). Only then it is possible to use the probability measure P on $( \Omega , { \mathcal { F } } )$ to define a probability measure on (S S). C| 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/12e86ee52a24784fdd0423e5b49283c5a83107d557b6f4a692aaba96974ddbd6.jpg)



Ω


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/d579e706789728d2baf3033da1f0c8aca754879152fb3be583fa3ef27928a284.jpg)



!


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/12ce71737fdbf8a15baf8085ddd14327faf81609f019f0036f149e83e1429bfa.jpg)



X


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/15df1765e6c96cc47a0fbea3fb65015cb26f00d1083560c837bfd465853bb033.jpg)



Z



Figure 2.1.: Illustration of Measurability: The random variables X and Z assign a grey value to each elementary event $\omega _ { 1 } , \ldots , \omega _ { 1 0 }$ as shown. The -algebra F is generated by the sets $F _ { 1 } = \{ \omega _ { 1 } , \omega _ { 2 } , \omega _ { 3 } \}$ $F _ { 2 } = \{ \omega _ { 4 } , \omega _ { 5 } , \omega _ { 6 } \} , F _ { 3 } = \{ \omega _ { 7 } , \ldots , \omega _ { 1 0 } \} .$ . The random variable X is measurable with respect to $\mathcal { F } _ { : }$ , the random variable Z is not measurable with respect to $\mathcal { F }$ .


Exercise: Let X be as in Definition 6. Show that 

$$
\{X ^ {- 1} (A) \mid A \in \mathcal {S} \}
$$

is a <sub>σ</sub>-algebra. What would be an interpretation of $X ^ { - 1 } ( A ) \ ?$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/97c7b15fe1c7426109798ac48352e84581c16d9281c6d77c9e88ff1b2cad6d96.jpg)


Motivation: We will now define the Lebesgue integral and give an interpretation and a comparison to the (possibly more familiar) Riemann integral. 

The definition of the Lebesgue integral is not only given to prepare the definition of the conditional expectation (definition 15). The definition will also show the construction of the Lebesgue integral and we will later use similar steps to construct the Itoˆ integral. C| 

## Definition 7 (Integral, Lebesgue Integral):

Let $( \Omega , { \mathcal { F } } , \mu )$ denote a measure space. 

1. Let $f$ denote a $( \mathcal { F } , \mathcal { B } ( \mathbb { R } ) ,$ )-measurable real valued, non-negative map. $f$ is called an elementary function if f takes on only a finite number of values $a _ { 1 } , \ldots , a _ { n }$ . For an elementary function we define 

$$
\int_ {\Omega} f (\omega) \mathrm{d} \mu (\omega) := \sum_ {i = 1} ^ {n} a _ {i} \mu (A _ {i})
$$

where $A _ { i } : = f ^ { - 1 } ( \{ a _ { i } \} ) ( \Rightarrow A _ { i } \in \mathcal { F } ) ^ { 3 }$ as the (Lebesgue) Integral of $f .$ 

2. Let $f$ denote a non-negative map defined on $\Omega ,$ such that a monotone increasing sequence $( u _ { k } ) _ { k \in \mathbb { N } }$ of elementary maps with $f : = \operatorname* { s u p } _ { k \in \mathbb { N } } u _ { k }$ exists. Then 

$$
\int_ {\Omega} f (\omega) \mathrm{d} \mu (\omega) := \sup _ {k \in \mathbb {N}} \int_ {\Omega} u _ {k} (\omega) \mathrm{d} \mu (\omega)
$$

is unique and is called the (Lebesgue) integral of $f .$ 

3. Let $f$ denote a map on Ω such that we have for $f ^ { + } : = \operatorname* { m a x } ( f , 0 )$ and $f ^ { - } : = \operatorname* { m a x } ( - f , 0 )$ respectively a monotone increasing sequence of elementary maps as in the previous definition. Furthermore we require that $\int _ { \Omega } f ^ { \pm } \mathrm { d } \mu < \infty$ . Then $f$ is called integrable with respect to $\mu$ and we define 

$$
\int_ {\Omega} f \mathrm{d} \mu := \int_ {\Omega} f ^ {+} \mathrm{d} \mu - \int_ {\Omega} f ^ {-} \mathrm{d} \mu
$$

as the (Lebesgue) integral of $f .$ 

Remark 8 $( \int f ( x ) \mathrm { d } x , \int f ( t )$ dt): If the measure $\mu$ is the Lebesgue measure $\mu = \lambda$ we use the shortend notation 

$$
\int_ {A} f (x) \mathrm{d} \lambda (x) =: \int_ {A} f (x) \mathrm{d} x.
$$

In this case $\Omega = \mathbb { R } ^ { n }$ and we denote the elements of Ω by latin leters, e.g. x (instead of <sub>ω</sub>). If the elements of $\Omega = \mathbb { R }$ have the interpretation of a time we usually denoted them by t. 

Theorem 9 (measurable ⇔ integrable for non-negative maps): For a non-negative map $f$ on Ω a monotone increasing sequence $( u _ { k } ) _ { k \in \mathbb { N } }$ of elementary maps with $f = \operatorname* { s u p } _ { k \in \mathbb { N } } u _ { k }$ exists if and only if f is ${ \mathcal F } .$ -measurable. 

Proof: See [1], §12. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/1aeb71f078230eb01ea96a82b4a808acfe216877fafbfb6ae167a5f3c45a99b1.jpg)


Interpretation: To develop an understanding of the (Lebesgue) integral we consider its definition for elementary maps 

$$
\int_ {\Omega} f (\omega) \mathrm{d} \mu (\omega) = \sum_ {i = 1} ^ {n} a _ {i} \mu (A _ {i}), \qquad A _ {i} := f ^ {- 1} (\{a _ {i} \}).
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/74dd6e379125bf12e35f1d0f9b6f1ff514d106e571b62a0818b32fca9c7ffe21.jpg)


The Lebesgue integral of an (elementary) map $f$ is the weighted sum of the function values $a _ { i }$ of $f ,$ each weighted by the measure $\mu ( A _ { i } )$ of the set on which this value is attained $( \mathrm { i . e . } \ A _ { i } = f ^ { - 1 } ( \{ a _ { i } \} ) )$ 

If in addition we have $\mu ( \Omega ) = 1$ , where Ω is the domain of $f ,$ , then the integral is a weighted average of the function values $a _ { i }$ of $f$ . 

For a real valued (elementary) function of a real valued argument, e.g. $f : [ a , b ] \mapsto \mathbb { R } .$ , and the Lebesgue measure the integral corresponds to the naive concept of 

an integral as being the sum all rectangles given by 

base area (Lebesgue measure of the interval) × height (function value) 

which is also the concept behind the Riemann integral. 

Part 2 and 3 of Definition 7 extend this concept via a limit approximation to more general functions. C| 

## Excursus: On the difference between Lebesgue and Riemann integrals<sup>4</sup>

The construction of the Lebesgue integral difers from the construction of the Riemann integral (which is perhaps more familiar) in the way the sets A are chosen. The Riemann integral starts from a given partition of the domain and multiplies the size of each subinterval by a corresponding functional value of (any) chosen point belonging to that interval (e.g. the center point). The Lebesgue integral chooses the partition as pre-image $f ^ { - 1 } ( \{ a _ { i } \} )$ of given function values $a _ { i } .$ . In short: the Riemann integral partitions the domain of $f ,$ the Lebesgue integral partitions the range of $f .$ For elementary functions both approaches give the same integral value, see Figure 2.2. For general functions the corresponding integrals are defined as the limit of a sequence of approximating elementary functions (if it exists). Here, the two concepts are diferent: In the limit, all Riemann integrable functions are Lebesgue integrable and the two limits give the same value for the integral. However, there exist Lebesgue integrable functions for which the Riemann integral is not defined (its limit construction does not converge). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/c669d3536d4dc8b79ec7622eb660df9c77764cc976709e5da1d3034fb07efe4a.jpg)



Figure 2.2.: On the diference ofLebesgue and Riemann integral


## Definition 10 (Distribution):

Let P denote a probability measure on (R B(R)) (e.g. the image measure of a random variable). The function 

$$
F _ {P} (x) := P ((- \infty , x))
$$

is called the distributionfunction<sup>5</sup> of P. 

If P denotes a probability measure on (R<sup>n</sup> B(R<sup>n</sup>)) the n-dimensional distribution function is defined as 

$$
F _ {P} (x _ {1}, \dots , x _ {n}) := P ((- \infty , x _ {1}) \times \dots \times (- \infty , x _ {n})).
$$

The distribution function of a random variable X is defined as the distribution function of its image measure $P _ { X }$ (see Definition 6). y 

## Definition 11 (Density):

Let $F _ { P }$ denote the distribution function of a probability measure P. If $F _ { P }$ is diferentiable we define 

$$
\phi (x) := \frac {\partial}{\partial x} F _ {P} (x)
$$

as the density of $P .$ If P is the image measure of some random variable X we also say that $\phi$ is the density of X. y 

Remark 12 (Integration using a known density / distribution): To calculate the integral of a function of a random variable $\left( \mathrm { e . g } \right.$ . to calculate expectation or variance) it is suficient to know the density or distribution function of the random variable. Let g denote a suficiently smooth function and X a random variable on $( \Omega , { \mathcal { F } } , P )$ ; then we have 

$$
\int_ {\Omega} g (X (\omega)) \mathrm{d} P (\omega) = \int_ {- \infty} ^ {\infty} g (x) \mathrm{d} F _ {P _ {X}} (x) = \int_ {- \infty} ^ {\infty} g (x) \phi (x) \mathrm{d} x,
$$

<sup>5</sup> We have $( - \infty , x ) \in { \mathcal { B } } ( { \mathbb R } )$ since (−∞ $x ) = \cup _ { i = 1 } ^ { \infty } ( x - i , x )$ - see Definition 1. 

where $F _ { P _ { X } }$ denotes the distribution function of X and φ the density of X (i.e. of $P _ { X } )$ . In this case it is neither necessary to know the underlying space $\Omega ,$ , the measure P, nor how X is modeled (i.e. defined) on this space. 

## Definition 13 (Independence of Random Variables):

Let $X : ( \Omega , { \mathcal { F } } ) \mapsto ( S , S )$ and $Y : ( \Omega , { \mathcal { F } } ) \mapsto ( S , S )$ denote two random variables. X and Y are called independent, if for all $A , B \in { \mathcal { S } }$ the events $X ^ { - 1 } ( A )$ and $Y ^ { - 1 } ( B )$ are independent in the sense of Definition 2. y 

Remark 14 (Independence): For $i = 1 , \ldots , n$ let $X _ { i } : \Omega \mapsto \mathbb { R }$ denote random variables with distribution functions $F _ { X _ { i } }$ and let $F _ { ( X _ { 1 } , \ldots , X _ { n } ) }$ denote the distribution function of $( X _ { 1 } , \ldots , X _ { n } )$ $\Omega \mapsto \mathbb { R } ^ { n }$ . Then the $X _ { i }$ are pairwise independent if and only if 

$$
F _ {(X _ {1}, \dots , X _ {n})} (x _ {1}, \dots , x _ {n}) = F _ {X _ {1}} (x _ {1}) \cdot \dots \cdot F _ {X _ {n}} (x _ {n}).
$$

## Definition 15 (Expectation, Conditional Expectation):

Let X denote a real valued random variable on the probability space $( \Omega , { \mathcal { F } } , P )$ 

1. If X is P-integrable we define 

$$
E ^ {P} (X) := \int_ {\Omega} X \mathrm{d} P
$$

as the expectation of X. 

2. Furthermore, let $F _ { i } \in { \mathcal { F } }$ with $P ( F _ { i } ) > 0$ . Then 

$$
E ^ {P} (X | F _ {i}) := \frac {1}{P (F _ {i})} \int_ {F _ {i}} X \mathrm{d} P
$$

is called the conditional expectation ofX under (the hypothesis) $F _ { i }$ 

Theorem 16 (Conditional Expectation<sup>6</sup>): Let X denote a real valued random variable on $( \Omega , { \mathcal { F } } , P )$ , either non-negative or integrable. Then we have for each <sub>σ</sub>-algebra $C \subset { \mathcal { F } }$ a nonnegative or integrable real valued random variable $X _ { | C }$ on Ω, unique in the sense of almost sure equality<sup>7</sup>, such that $X _ { | C }$ is C-measurable and 

$$
\forall C \in \mathcal {C}: \quad \int_ {C} X _ {| \mathcal {C}} \mathrm{d} P = \int_ {C} X \mathrm{d} P, \text {i.e.} \quad \mathrm{E} ^ {P} (X | C) = \mathrm{E} ^ {P} (X _ {\mathcal {C}} | C).
$$

We will discuss the interpretation of this theorem after giving a name to $X _ { C } { \mathrm { : } }$ : 

## Definition 17 (Conditional Expectation (continued)):

Under the assumptions and with the notation of Theorem 16 we define: 

1. The random variable $X _ { | C }$ is called the conditional expectation ofX under (the hypothesis) C and is denoted by 

$$
E ^ {P} (X | \mathcal {C}) := X _ {| \mathcal {C}}.
$$

(2.1) 

2. Let Y denote another random variable on the same measure space. We define: 

$$
E ^ {P} (X | Y) := E (X | \sigma (Y)),\tag{2.2}
$$

where $\sigma ( Y )$ is the <sub>σ</sub>-algebra generated by Y, i.e. the smallest <sub>σ</sub>-algebra, with respect to which Y is measurable, $\mathrm { i . e . } \sigma ( Y ) : = \sigma ( Y ^ { - 1 } ( S ) )$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/b540052bd2945ad77d8c0b5d26cfdb2a837cd2d88b4d31d43f55a9ca403fe87f.jpg)


Interpretation: First note that the two concepts of expectations from Definition 15 are just special cases of the conditional expectation defined in Definition 17, namely: 

• Let $C = \{ \boldsymbol { 0 } , \boldsymbol { \Omega } \}$ 

Then $E ( X | C ) = X _ { | C }$ where $X _ { | C } ( \omega ) = E ( X ) \quad \forall \omega \in \Omega$ 

• For $C = \{ \varnothing , F , \Omega \setminus F , \Omega \}$ we have $X _ { | C } ( \omega ) = \left\{ \begin{array} { l l } { E ( X | F ) } & { \mathrm { i f } \omega \in F } \\ { E ( X | \Omega \setminus F ) } & { \mathrm { i f } \omega \in \Omega \setminus F } \end{array} \right. ,$ 

with $E ( X ) = P ( F ) \cdot E ( X | F ) + ( 1 - P ( F ) ) \cdot E ( X | \Omega \setminus F )$ 

The conditional expectation is a random variable that is derived from X such that only events (sets) in C can be distinguished. In the first case we have a very coarse C and the image of $X _ { | C }$ contains only the expectation $E ( X )$ . This is the smallest piece of information on $X , ~ \mathrm { A s } ~ C$ becomes finer more and more information about X becomes visible in $X _ { | C }$ . Furthermore: If X itself is C-measurable then X and $X _ { | C }$ are (P-almost surely) indistinguishable. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/74da2bc855168ebbda202fdc3472bc37555d0f3be4bb72ab6fc23cf961251377.jpg)



X


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/816f5de9f0b106134bc95605278bb87d3bab0434c64a90b4938dc58a34d6a44a.jpg)



C


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/5e0fd31fd747072449ea0a2e23c7d25f3f2f226e9a2abe4dcec9aecac1cba63c.jpg)



E(X|C)



Figure 2.3.: Conditional Expectation: Let the -algebra C be generated by the sets $C _ { 1 } = \{ \omega _ { 1 } , \omega _ { 2 } , \omega _ { 3 } \}$ $C _ { 2 } = \{ \omega _ { 4 } , \omega _ { 5 } , \omega _ { 6 } \} , C _ { 3 } = \{ \omega _ { 7 } , \ldots , \omega _ { 1 0 } \} .$


In this sense C may be interpreted as an information set and $X _ { | C }$ as a filtered version of X. If it is only possible to make statements about events in C then we can only make statements about X which could also be made about $X _ { | C }$ C| 

## 2.2. Stochastic Processes

## Definition 18 (Stochastic Process):

A family $X = \{ X _ { t } \mid 0 \leq t < \infty \}$ of random variables 

$$
X _ {t}: (\Omega , \mathcal {F}) \to (S, \mathcal {S})
$$

is called (time continuous) stochastic process. ${ \mathrm { I f ~ } } ( S , S ) = ( \mathbb { R } ^ { d } , { \mathcal { B } } ( \mathbb { R } ^ { d } ) )$ , we say that X is a ddimensional stochastic process. The family X may also be interpreted as a $X : [ 0 , \infty ) \times \Omega  S$ : 

$$
X (t, \omega) := X _ {t} (\omega) \qquad \forall (t, \omega) \in [ 0, \infty) \times \Omega .
$$

If the range (S S) is not given explicitly we assume $( S , S ) = ( \mathbb { R } ^ { d } , \mathcal { B } ( \mathbb { R } ^ { d } ) )$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/e733dc16daa1012626817d23bdca2da404aafc717ad52f9485467f55915249ab.jpg)


Interpretation: The parameter t obviously refers to time. For fixed $t \in [ 0 , \infty )$ we view X(t) as the outcome of an experiment at time t. Note that all random variables X(t) are modeled over the same measurable space $( \Omega , { \mathcal { F } } )$ . Thus we do not assume a family $( \Omega _ { t } , \mathcal { F } _ { t } )$ of measurable spaces, one for each X . The stochastic 

process X assigns a path to each $\omega \in \Omega \colon$ For a fixed $\omega \in \Omega$ the path $X ( \cdot , \omega ) : = \{ ( t , X ( t , \omega ) ) \mid t \in$ $[ 0 , \infty ) \}$ is a sequence of outcomes of the random experiments $X _ { t }$ (a trajectory) associated with a state <sub>ω</sub>. Knowledge about $\omega \in \Omega$ implies knowledge of the whole history (past, present and future) X(<sub>ω</sub>). 

To model the diferent levels of knowledge and thus distinguish between past and future we will define in 2.3 the concept of a filtration and an adapted process. C| 

## Definition 19 (Path):

Let X denote a stochastic process. For a fixed $\omega \in \Omega$ the mapping $t \mapsto X ( t , \omega )$ is called the path of X (in state <sub>ω</sub>). y 

## Definition 20 (Equality of Stochastic Processes):

We define three notions of equality of stochastic processes: 

1. Two stochastic processes X and Y are called indistinguishable, if 

$$
P (X _ {t} = Y _ {t}: \forall 0 \leq t <   \infty) = 1.
$$

2. A stochastic process Y is a modification of X, if 

$$
P (X _ {t} = Y _ {t}) = 1: \forall 0 \leq t <   \infty .
$$

3. Two stochastic processes X and Y have the samefinite dimensional distributions, if 

$$
\begin{array}{l} \forall   n:   \forall   0 \leq t _ {1} <   t _ {2} <   \ldots <   t _ {n} <   \infty :   \forall   A \in \mathcal {B} (S ^ {n}): \\ P ((X _ {t _ {1}}, \ldots , X _ {t _ {n}}) \in A) = P ((Y _ {t _ {1}}, \ldots , Y _ {t _ {n}}) \in A). \end{array}
$$

Remark 21 (on the equality of stochastic processes): While in Definition 20.3 only the distributions generated by the processes are considered, the Definitions 20.1 and 20.2 consider the pointwise diferences between the processes. The diference between 20.1 and 20.2 will become apparent in the following example: 

Let $Z : ( \mathbb { R } , { \mathcal { B } } ( \mathbb { R } ) ) \to ( [ - 1 , 1 ] , { \mathcal { B } } ( [ - 1 , 1 ] ) )$ be a random variable on $( \Omega , \mathcal { F } , P ) = ( \mathbb { R } , \mathcal { B } , \lambda )$ and $t \mapsto X ( t ) : = t \cdot Z$ be a stochastic process.<sup>8</sup> Let $P ( \{ Z \in A \} ) = P ( \{ - Z \in A \} ) \forall A \in { \mathcal { B } } ( [ - 1 , 1 ] )$ and 

<sup>8</sup> An interpretation of this process would be the position of a moving particle, having at time 0 the position 0 and the random speed Z. 

$P ( \{ Z = x \} ) = 0 \forall x \in [ - 1 , 1 ]$ , e.g. an equally distributed Z. Furthermore let $\forall \left( t , \omega \right) \in \left[ 0 , \infty \right) \times \mathbb { R }$ 

$$
Y _ {1} (t, \omega) := \left\{ \begin{array}{l l} X (t, \omega) & \text { for } t \neq \omega \\ - X (t, \omega) & \text { for } t = \omega \end{array} \right., \qquad Y _ {2} (t, \omega) := - X (t, \omega).
$$

The $Y _ { 1 }$ is a modification of $X ,$ since $Y _ { 1 } ( t )$ difers from $X ( t )$ (for fixed t) only on a set with probability 0. However, X and $Y _ { 1 }$ are not indistinguishable, since $\begin{array} { r } { P ( X ( t ) = Y _ { 1 } ( t ) \ : \ \forall \ 0 \leq t < \infty ) = \frac { 1 } { \gamma } } \end{array}$ (the two processes are diferent on 50% of all paths). $Y _ { 2 }$ is neither indistinguishable nor a modification of $X ,$ but due to $P ( \{ Z \in A \} ) = P ( \{ Z \in - A \} ) \ \forall A \in { \mathcal { B } } ( [ - 1 , 1 ] )$ it fulfills condition 20.3. 

To summarize, 20.1 considers the equality of the processes X, Y, 20.2 considers equality of the random variables X(t), Y(t) for fixed t, and 20.3 considers the equality of distributions. In our applications we are interested only in the distributions of processes. 

## 2.3. Filtration

## Definition 22 (Filtration):

Let (Ω F) denote a measurable space. A Family of <sub>σ</sub>-algebras $\{ \mathcal { F } _ { t } \mid t \geq 0 \}$ , where 

$$
\mathcal {F} _ {s} \subseteq \mathcal {F} _ {t} \subseteq \mathcal {F} \quad \text {   for   } 0 \leq s \leq t,
$$

is called a Filtration on $( \Omega , { \mathcal { F } } )$ . 

## Definition 23 (Generated Filtration):

Let X denote a stochastic process on (Ω F). We define 

$$
\mathcal {F} _ {t} ^ {X} := \sigma (X _ {s}; 0 \leq s \leq t)
$$

:= the smallest <sub>σ</sub>-algebra with respect to which $X _ { s }$ is measurable $\forall s \in [ 0 , t ]$ 

## Definition 24 (Adapted Process):

Let X denote a stochastic process on $( \Omega , { \mathcal { F } } )$ and $\{ \mathcal { F } _ { t } \}$ a filtration on $( \Omega , { \mathcal { F } } )$ . The process X is called $\{ \mathcal { F } _ { t } \}$ -adapted, if $X _ { t }$ is $\mathcal { F } _ { t }$ -measurable for all $t \geq 0$ y 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/6d5ec5797ce7e49b22ba02bace9ab4d54c20a1659a8809ebb4dc4ef6c322cab6.jpg)


Interpretation: In Figure 2.4 we depict a filtration of four <sub>σ</sub>-algebras with increasing refinement (left to right). The black borders surround the generators of the corresponding <sub>σ</sub>-algebra. If a stochastic process maps a grey value for each elementary event (or path) $\omega _ { i }$ of Ω (left), then the process is adapted if it takes 

a constant gray value on the generators of the respective <sub>σ</sub>-algebra. If at time $t _ { 2 }$ the process depicted were to assign to $\omega _ { 7 }$ the dark grey of $\omega _ { 8 }$ , then the process would be adapted, otherwise it is not. 

By means of the conditional expectation (see Theorem 16 and the interpretation of Figure 2.3) we may create an adapted process from a given filtration $\{ \mathcal { F } _ { t } \mid t \geq 0 \}$ and an $\mathcal { F } .$ measurable random variable Z: 

Lemma 25 (Process of the Conditional Expectation): Let $\{ \mathcal { F } _ { t } \mid t \geq 0 \}$ denote a filtration $\mathcal { F } _ { s } \subseteq \mathcal { F } _ { t } \subseteq \mathcal { F }$ and $Z$ an $\mathcal { F }$ measurable random variable. Then 

$$
X (t) := \operatorname{E} (Z \mid \mathcal {F} _ {t})
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/1b7347f0ee3bd6cad11b4672c089bac10d8395f64eb99b35a4d8fda81df053f1.jpg)



Figure 2.4.: Illustration of a filtration and an adapted process


is a {F<sub>t</sub>}-adapted process. 

This lemma shows how the filtration (and the corresponding adapted process) may be viewed as a model for information: The random variable X(t) in Lemma 25 allows with increasing t more and more specific statements about the nature of Z. Compare this to the illustrations in Figure 2.1 and 2.3. C| 

The concepts of an adapted process only links random variables $X ( t )$ to <sub>σ</sub>-algebras $\mathcal { F } _ { t }$ for any t. It does not necessarily imply that the stochastic process X (interpreted as a random variable on $[ 0 , \infty ) \times \Omega )$ is measurable. A stronger requirement is given by: 

## Definition 26 (Progressively Measurable):

An (n-dimensional) stochastic process X is called progessively measurable with respect to the filtration $\{ \mathcal { F } _ { t } \}$ if for each $T > 0$ the mapping 

$$
X: ([ 0, T ] \times \Omega , \mathcal {B} ([ 0, T ] \otimes \mathcal {F} _ {t})) \rightarrow (\mathbb {R}, \mathcal {B} (\mathbb {R} ^ {n}))
$$

meßbar ist. 

Remark 27: Any progressively measurable process is measurable and adapted. Conversly a measurable and adapted process has a progressively measurable modification, see [20]. 

## 2.4. Brownian Motion

## Definition 28 (Brownian Motion):

Let $W : [ 0 , \infty ) \times \Omega  \mathbb { R } ^ { n }$ denote a stochastic process with the following properties: 

1. W(0) = 0 (P-almost surely) 

2. The map $t \mapsto W ( t )$ is continuous (P-almost surely) 

3. For given $t _ { 0 } < t _ { 1 } < . . . < t _ { k }$ the increments $W ( t _ { 1 } ) - W ( t _ { 0 } ) , \ldots , W ( t _ { k } ) - W ( t _ { k - 1 } )$ are mutually independent. 

4. For all $0 \le s \le t$ we have $W ( t ) - W ( s ) \sim \smash { N ( 0 , ( t - s ) I _ { n } ) }$ , i.e. the increment is normally distributed with mean 0 and covariance matrix $( t - s ) I _ { n }$ , where $I _ { n }$ denotes the n×n identity matrix. 

Then W is called (n-dimensional) P-Brownian motion or a (n-dimensional) P-Wiener process. 

We have not yet discussed the question of whether a process with such properties exists (it does). The question for its existence is non-trivial. For example if we want to replace normally distributed by lognormally distributed in property 4 there would be no such process.<sup>9</sup> If we set $s = 0$ in 4 we see that we have prescribed the distribution of $W ( t )$ as well as the distribution of the increments $W ( t ) - W ( s )$ . 

Remark 29 (Brownian Motion): The property 4 is less axiomatic than one might assume: The central requirement is the independence of the increments together with the requirement that increments of the same time step size $t - s$ have the same non negative variance (here $t - s )$ and mean 0. That the increments are normal distributed is more a consequence than an requirement, see Theorem 30. This theorem also gives a construction of the Brownian motion. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/37bdf403542222cc074c4b887010961e3095970c11a06dd3dcce082e2b02f890.jpg)



Figure 2.5.: Time discretization ofa Brownian motion: The transition $\Delta W ( T _ { i } ) : = W ( T _ { i + 1 } ) - W ( T _ { i } )$ from time $T _ { i }$ to $T _ { i + 1 }$ is normal distributed. The mean ofthe transition is 0, i.e. under the condition that at time $T _ { i }$ the state $W ( T _ { i } ) = x ^ { * }$ was attained, the (conditional) expectation $o f W ( T _ { i + 1 } ) i s x ^ { * } .$ $\operatorname { E } ( W ( T _ { i + 1 } ) \mid W ( T _ { i } ) = x ^ { * } ) \ = \ x ^ { * } .$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/7073b84f1b7c503583c988850decfb06c12bd68c18b890b7b47d57acc2cdf916.jpg)


Tip (time-discrete realizations): In the following we will often consider the realizations of a stochastic process at discrete times $0 = T _ { 0 } < T _ { 1 } < . . . < T _ { N }$ only (e.g. this will be the case when we consider the implementation). If we need only the realizations $W ( T _ { i } )$ we may generate them by the time-discrete increments $\Delta W ( T _ { i } ) : = W ( T _ { i + 1 } ) - W ( T _ { i } )$ since from Definition 28 we have $\begin{array} { r } { W ( T _ { i } ) = \sum _ { k = 0 } ^ { i - 1 } \Delta W ( T _ { k } ) , W ( T _ { 0 } ) : = } \end{array}$ 0. See Figure 2.5. C| 

<sup>9</sup> Note that the sum of two (independent) normal distributed random variables is normally distributed, but the sum of two lognormal distributed random variables is not lognormal 

## 2.5. Wiener Measure, Canonical Setup

The following theorem gives a construction (or approximation) of a Brownian motion. It defines the Wiener measure and shows that the properties of a Brownian motion are less axiomatic than one might assume from Definition 28; rather they are consequences of independence. 

Theorem 30 (Invariance Principle ofDonsker (1951), see. [20] §2): 

Let $( \Omega , { \mathcal { F } } , P )$ denote a probability space and $( Y _ { j } ) _ { i = 1 } ^ { \infty }$ a sequence of independent identically distributed random variables (not necessarily normal distributed!) with mean 0 and variance $\sigma ^ { 2 } > 0$ . Define $S _ { 0 } : = 0$ and $\begin{array} { r } { S _ { k } : = \sum _ { j = 1 } ^ { k } Y _ { j } } \end{array}$ . Let $X ^ { n }$ denote a stochastic process defined as the (scaled) linear interpolation of the $S _ { k } \mathrm { : }$ ’s at time steps of size ${ \frac { 1 } { n } } ;$ 

$$
X ^ {n} (t) := \frac {1}{\sigma \sqrt {n}} \big ((t \cdot n - [ t \cdot n ]) S _ {[ t \cdot n ] + 1} + ([ t \cdot n ] + 1 - t \cdot n)) S _ {[ t \cdot n ]} \big),
$$

where [x] denotes the largest integer number less or equal x. 

A path $X ^ { n } ( \omega ) , \omega \in \Omega$ , defines a continuous map $[ 0 , \infty ) \ \mapsto \ \mathbb { R }$ and $X ^ { n }$ is $( \Omega , { \mathcal { F } } )$ 7→ $( C ( [ 0 , \infty ) )$ B(C([0 ∞))))-measurable<sup>10</sup>. Let $P ^ { n }$ denote the image measure of $X ^ { n }$ defined on $( C ( [ 0 , \infty ) ) , \mathcal { B } ( C ( [ 0 , \infty ) ) )$ . Then we have: 

$\{ P _ { n } \} _ { n = 1 } ^ { \infty }$ converges on $( C ( [ 0 , \infty ) ) , \mathcal { B } ( C ( [ 0 , \infty ) ) ) )$ to a measure $P ^ { * }$ in the weak sense<sup>11</sup>. 

• The process W defined on $( C ( [ 0 , \infty ) ) , \mathcal { B } ( C ( [ 0 , \infty ) ) ) )$ by 

$$
W (t, \omega) := \omega (t)
$$

is a $P ^ { * }$ Brownian motion. 

Proof: See [20] §2. 

Definition 31 (Wiener Measure): 

The measure $P ^ { * }$ from Theorem 30 is called Wiener measure. 

Definition 32 (Canonical Setup): 

The space 

$$
(C ([ 0, \infty)), \mathcal {B} (C ([ 0, \infty)), P ^ {*})
$$

(as defined in Theorem 30) is called the canonical setup for a Brownian motion W defined by $W ( t , \omega ) : = \omega ( t ) , \omega \in C ( [ 0 , \infty ) )$ . y 

Remark 33: A more detailed discussion of Theorem 30 may be found in [20]. A less formal discussion of properties of the Brownian motion may be found in [14]. 

## 2.6. Ito Calculusˆ

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/73eb873e8836c7e1c639ff09de7ba999616797d29bc4f6570828a93481ca7f86.jpg)


Motivation: The Brownian motion W is our first encounter with an important continuous stochastic process. The Brownian motion may be viewed as the limit of a scaled random $w a l k . ^ { 1 2 }$ If we interpret the Brownian motion W in this sense as a model for the movement of a particle, then $W ( T )$ denotes the position of the 

particle at time T and $W ( T + \Delta T ) - W ( T )$ the position change that occurs from T to $T + \Delta T$ ; to be precise, W(T) models the probability distribution of the particle position. 

The model of a Brownian motion is that position changes are normal distributed with mean 0 and standard deviation $\sqrt { \Delta { T } }$ . Requiring mean 0 corresponds to requiring that the position change has no directional preference. The standard deviation $\sqrt { \Delta { T } }$ is, apart from a constant which we assume to be 1, a consequence of the requirement that position changes are independent of the position and time at which they occur. 

To motivate the class of Ito processes we consider the Brownian motion at discrete timesˆ $0 ~ = ~ T _ { 0 } ~ < ~ T _ { 1 } ~ < ~ . . . ~ < ~ T _ { N }$ . The random variable $W ( T _ { i } )$ (position of the particle) may be expressed through the increments $\Delta W ( T _ { i } ) : = W ( T _ { i + 1 } ) - W ( T _ { i } )$ 

$$
W (T _ {i}) = \sum_ {j = 0} ^ {i - 1} \Delta W (T _ {j}).
$$

Using the increments $\Delta W ( T _ { j } )$ we may define a whole family of discrete stochastic pro-

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/806f956bd024495a7f3b6a485dbc0755be16d862633bb436158ff7a1a0be004a.jpg)



Figure 2.6.: Paths ofa (discretization ofa) Brownian motion


cesses. We give a step by step introduction and use the illustrative interpretation of a particle movement: First we assume that the particle may lose energy over time (for example). Then the increments may still be normal distributed but their standard deviation no longer will be $\sqrt { T _ { j + 1 } - T _ { j } }$ . Instead it might be a time-dependent scaling thereof, $\mathbf { e . g . } e ^ { - T _ { j } } \cdot \sqrt { T _ { j + 1 } - T _ { j } }$ where the standard deviation decays exponentially. Multiplying the increments $\Delta W ( T _ { j } )$ by a factor gives normal distributed increments with arbitrary standard deviations. Thus we consider a process of the form 

$$
X (T _ {i}) = \sum_ {j = 0} ^ {i - 1} \sigma (T _ {j}) \Delta W (T _ {j}),
$$

where in our example we would use $\sigma ( T _ { j } ) : = e ^ { - T _ { j } }$ 

<sup>12</sup> In a (one-dimensional) random walk a particle changes position at discrete time steps by a (constant) distance (say 1) in either direction with equal probability. In other words, we have binomial distributed $Y _ { i }$ in Theorem 30. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/4b4d1721eb1bfebbe265679640d6b65afda3f358167396f201bc6e3e442aaa69.jpg)



Figure 2.7.: Paths ofa (discretization ofa) Brownian motion with time dependent instantaneous volatility


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/994b35f72a3c5843ca26c4c9dccb75d98447d6d3821ef572efdafa3648f3d338.jpg)



Figure 2.8.: Paths ofa (discretization ofa) Brownian motion with a drift


Next we consider the case where the particle has a preference for a certain direction, i.e. a $d r i f t .$ . This is modeled by increments having a mean diferent from zero. The addition of a constant $\mu$ to a normal distributed random variable with mean zero will give a normal distributed random variable with mean $\mu .$ We want $\mu$ to be the drift per time unit and allow that $\mu$ may change over time. Thus we add $\mu ( T _ { j } ) \cdot ( T _ { j + 1 } - T _ { j } )$ to the corresponding increment over period $T _ { j }$ to $T _ { j + 1 }$ . If we also consider the starting point to be random, modeled by a random variable $X ( 0 )$ we then consider processes of the form 

$$
X (T _ {i}) = X (0) + \sum_ {j = 0} ^ {i - 1} \underbrace {\mu (T _ {j}) \underbrace {(T _ {j + 1} - T _ {j})} _ {=: \Delta T _ {j}} + \sigma (T _ {j}) \Delta W (T _ {j})} _ {\text { Normal   distributed   with   mean } \mu (T _ {j}) \Delta T _ {j} \text { and   standard   deviation } \sigma (T _ {j}) \sqrt {\Delta T _ {j}}} \quad ,
$$

i.e. 

$$
X (T _ {j + 1}) - X (T _ {j}) = \mu (T _ {j}) \underbrace {(T _ {j + 1} - T _ {j})} _ {=: \Delta T _ {j}} + \sigma (T _ {j}) \Delta W (T _ {j}).
$$

Our next generalization of the process is that the parameters $\mu ( T _ { j } )$ and $\sigma ( T _ { j } )$ could depend on the paths, i.e. are assumed to be random variables. This might appear odd since then one could create any time-discrete stochastic processes.<sup>13</sup> However, it would make sense to allow the parameters $\mu ( T _ { j } )$ and/or $\sigma ( T _ { j } )$ (used in the increment from $X ( T _ { j } ) \mathrm { t o } X ( T _ { j + 1 } ) )$ to depend on the current state of $X ( T _ { j } )$ as in 

$$
\underbrace {X (T _ {j + 1}) - X (T _ {j})} _ {=: \Delta X (T _ {j})} = X (T _ {j}) \underbrace {(T _ {j + 1} - T _ {j})} _ {=: \Delta T _ {j}} + \sigma (T _ {j}) \Delta W (T _ {j}).
$$

Here we would have $\mu ( T _ { j } ) = \mu ( T _ { j } , X ( T _ { j } ) ) = X ( T _ { j } ) .$ , i.e. a drift that is a random variable. It is an important fact that the drift for the increment from $T _ { j } : { \mathrm { t o } } T _ { j + 1 }$ is known in $T _ { j }$ . More general we allow $\mu$ and $\sigma$ to be stochastic processes if they are {F<sub>t</sub>}-adapted.<sup>14</sup> 

The continuous analog to the time-discrete processes considered above are Ito processes,ˆ i.e. processes of the form 

$$
X (T) = X (0) + \int_ {0} ^ {T} \mu (t) d t + \int_ {0} ^ {T} \sigma (t) d W (t),\tag{2.3}
$$

i.e. 

$$
X (T) - X (0) = \int_ {0} ^ {T} \mu (t) \mathrm{d} t + \int_ {0} ^ {T} \sigma (t) \mathrm{d} W (t)
$$

and as a short-hand we will write 

$$
\mathrm{d} X (t) = \mu (t) \mathrm{d} t + \sigma (t) \mathrm{d} W (t).
$$

While the dt part of (2.3) may be (and will be) understood pathwise as a Lebesgue (or even Riemann) integral, we need to define the dW(t) part (as we will see), the Itˆo Integral.<sup>15</sup> C| 

## 2.6.1. Ito Integralˆ

In this section we define the Ito integralˆ $\int _ { S } ^ { T } f ( t , \omega ) \ \mathrm { d } W ( t , \omega )$ . We do not present the mathematical theory in full detail. For a more detailed discussion of the Ito integral see, e.g,ˆ [14, 27, 20, 21]). 

## Definition 34 (The Filtration {F<sub>t</sub>} generated by W):

Let $( \Omega , { \mathcal { F } } , P )$ denote a probability space and $W ( t )$ a Brownian motion defined on $( \Omega , { \mathcal { F } } , P )$ (e.g. by the canonical setup). We define $\mathcal { F } _ { t }$ as the -algebra generated by $W ( s ) , s \leq t ,$ i.e. the smallest -algebra, which contains sets of the form 

$$
\{\omega ; W (t _ {1}, \omega) \in F _ {1}, \dots , W (t _ {k}, \omega) \in F _ {k}, \} = \bigcap_ {i = 1} ^ {k} W (t _ {i}) ^ {- 1} (F _ {i})
$$

for arbitrary $t _ { i } < t$ and $F _ { i } \subset \mathbb { R } , F _ { i } \in \mathcal { B } ( \mathbb { R } ) ( j \leq k )$ and arbitrary $k \in \mathbb { N } .$ . Furthermore we assume that all sets of measure zero belong to $\mathcal { F } _ { t }$ . Then $\{ \mathcal { F } _ { t } \}$ is a filtration which we call the filtration generated by W. y 

Remark 35: W is a $\{ \mathcal { F } _ { t } \}$ -adapted process. 

## Definition 36 (Ito integral for elementary processes):ˆ

A stochastic process φ is called elementary, if 

$$
\phi (t, \omega) = \sum_ {j \in \mathbb {N} \cup \{0 \}} e _ {j} (\omega) \cdot 1 _ {(t _ {j}, t _ {j + 1} ]} (t),
$$

where $\{ t _ { j } | j \in \mathbb { N } \cup \{ 0 \} \}$ is a strictly monotone sequence in $[ 0 , \infty )$ with $t _ { 0 } : = 0$ and $\{ e _ { j } | j \in \mathbb { N } \cup \{ 0 \} \}$ a sequence of $\mathcal { F } _ { t _ { j } }$ -measurable random variables and $1 _ { ( t _ { j } , t _ { j + 1 } ] }$ denotes the indicator function $^ { 1 6 } \cdot ^ { 1 7 }$ 

For an elementary process we define the Ito integral asˆ 

$$
\begin{array}{l} \int_ {0} ^ {\infty} \phi (t, \omega) \mathrm{d} W (t) := \sum_ {j \in \mathbb {N} \cup \{0 \}} e _ {j} (\omega) \cdot (W (t _ {j + 1}, \omega) - W (t _ {j}, \omega)), \\ \int_ {S} ^ {T} \phi (t, \omega) \mathrm{d} W (t) := \int_ {0} ^ {\infty} \phi (t, \omega) \cdot 1 _ {(S, T ]} (t) \mathrm{d} W (t). \end{array}
$$

Remark 37 (on the one sided continuity of the integrand): In some textbooks (e.g. [27]) the elementary integral is defined using the indicator function $1 _ { [ t _ { j } , t _ { j + 1 } ) }$ in place of $1 _ { ( t _ { j } , t _ { j + 1 } ] } .$ . For continuous integrators, as we consider here $\mathbf { \rho } ( W ( t ) )$ , it makes no diference which variant we use. However, if jump processes are considered (see e.g. [29]), and also with respect to the interpretation of the integral as a trading strategy (see page 63), our definition is the better suited. 

Lemma 38 (Ito Isometry):ˆ Let φ denote an elementary process such that $\phi ( \cdot , \omega )$ is bounded. Then we have 

$$
\mathrm{E} \left[ \left(\int_ {S} ^ {T} \phi (t, \cdot) \mathrm{d} W (t)\right) ^ {2} \right] = \mathrm{E} \left[ \int_ {S} ^ {T} \phi (t, \cdot) ^ {2} \mathrm{d} t \right].
$$

## Definition 39 (Ito Integral):ˆ

The class ofintegrands ofthe Itˆo integral is defined as the set of maps 

$$
f: [ 0, \infty) \times \Omega \mapsto \mathbb {R},
$$

for which 

1. $f$ is a ${ \mathcal { B } } \times { \mathcal { F } }$ -measurable map, 

2. $f$ is an $\mathcal { F } _ { t }$ -adapted process, 

3. $f$ is P-almost sure of finite quadratic variation, i.e. we have E- $\int _ { S } ^ { T } f ( t , \omega ) ^ { 2 } \mathrm { d } t ] < \infty$ 

If f belongs to this class then there exists an approximating sequence $\{ \phi _ { n } \}$ of elementary processes with 

$$
\mathrm{E} ^ {P} \left[ \int_ {S} ^ {T} (f (t, \omega) - \phi_ {n} (t, \omega)) ^ {2} \mathrm{d} t \right]\rightarrow 0 \quad (\text { for } n \rightarrow \infty),
$$

and the Itˆo integral is defined as the (unique) $L _ { 2 }$ limit 

$$
\int_ {S} ^ {T} f (t, \omega) \mathrm{d} W (t) := \lim _ {n \rightarrow \infty} \int_ {S} ^ {T} \phi_ {n} (t, \omega) \mathrm{d} W (t).
$$

Remark 40: For a proof of the statements made in this definition (e.g. the existence and uniqueness of the limit) see [27]. 

## 2.6.2. Ito Processˆ

Definition 41 (Ito Process):ˆ 

Let $\sigma$ denote a stochastic process belonging to the class of integrands of the Ito integralsˆ (see 39) with 

$$
P \left(\int_ {0} ^ {t} \sigma (\tau , \omega) ^ {2} \mathrm{d} \tau <   \infty \forall t \geq 0\right) = 1
$$

and $\mu$ an $\{ \mathcal { F } _ { t } \}$ -adapted process with 

$$
P \left(\int_ {0} ^ {t} | \mu (\tau , \omega) | \mathrm{d} \tau <   \infty \forall t \geq 0\right) = 1.
$$

Then the process X defined through 

$$
X (t, \omega) = X (0, \omega) + \int_ {0} ^ {t} \mu (s, \omega) \mathrm{d} s + \int_ {0} ^ {t} \sigma (s, \omega) \mathrm{d} W (s, \omega),
$$

where $X ( 0 , \cdot )$ is $( \mathcal { F } _ { 0 } , \mathcal { B } ( \mathbb { R } ) )$ -measurable is called Itˆo process (Remark: X is $\mathcal { F } _ { t }$ -adapted). y 

This definition is generalized by the m-dimensional Brownian motion as 

## Definition 42 (Ito Process (ˆ m-factorial, n-dimensional)<sup>18</sup>):

Let $W = ( W _ { 1 } , \ldots , W _ { m } ) ^ { \top }$ denote an m-dimensional Brownian motion defined on $( \Omega , { \mathcal { F } } , P )$ . Let $\sigma _ { i , j } ( i = 1 , \ldots , n , j = 1 , \ldots , m )$ denote stochastic processes belonging to the class of integrands of the Ito integral (compare Definitionˆ 39) with 

$$
P \left(\int_ {0} ^ {t} \sigma_ {i, j} (\tau , \omega) ^ {2} \mathrm{d} \tau <   \infty \forall t \geq 0\right) = 1 \quad i = 1, \dots , n, j = 1, \dots , m,
$$

and $\mu _ { i } ( i = 1 , \ldots , n )$ an $\{ \mathcal { F } _ { t } \}$ -adapted process with 

$$
P \left(\int_ {0} ^ {t} | \mu_ {i} (\tau , \omega) | \mathrm{d} \tau <   \infty \forall t \geq 0\right) = 1 \quad i = 1, \dots , n.
$$

<sup>18</sup> Compare [27], §4.2 

Then the (n-dimensional) process $X = ( X _ { 1 } , \ldots , X _ { n } ) ^ { \mathsf { T } }$ with $X ( 0 , \cdot )$ being $( \mathcal { F } _ { 0 } , \mathcal { B } ( \mathbb { R } ^ { n } ) ) ,$ )-measurable and 

$$
X _ {i} (t, \omega) = X _ {i} (0, \omega) + \int_ {0} ^ {t} \mu_ {i} (s, \omega) \mathrm{d} s + \sum_ {j = 1} ^ {m} \int_ {0} ^ {t} \sigma_ {i, j} (s, \omega) \mathrm{d} W _ {j} (s, \omega) \quad (i = 1, \dots , n),
$$

is called (n-dimensional) (m-factorial) Itˆo process.<sup>19</sup> We will write X in the shorter matrix notation as 

$$
X (t, \omega) = X (0, \omega) + \int_ {0} ^ {t} \mu (s, \omega) d s + \int_ {0} ^ {t} \sigma (s, \omega) \cdot d W (s, \omega),
$$

with 

$$
X = \left( \begin{array}{c} X _ {1} \\ \vdots \\ X _ {n} \end{array} \right) \qquad \qquad \mu = \left( \begin{array}{c} \mu_ {1} \\ \vdots \\ \mu_ {n} \end{array} \right) \qquad \qquad \sigma = \left( \begin{array}{c c c} \sigma_ {1, 1} & \ldots & \sigma_ {1, m} \\ \vdots & & \vdots \\ \sigma_ {n, 1} & \ldots & \sigma_ {n, m} \end{array} \right).
$$

Remark 43 (Ito Process, diˆ ferential notation): For an Ito processˆ 

$$
X (T, \omega) = X (0, \omega) + \int_ {0} ^ {T} \mu (t, \omega) d t + \int_ {0} ^ {T} \sigma (t, \omega) \cdot d W (t, \omega),
$$

as defined by Definition 41 and 42 we will use the shortened notation 

$$
\mathrm{d} X (t, \omega) = \mu (t, \omega) \mathrm{d} t + \sigma (t, \omega) \cdot \mathrm{d} W (t, \omega).
$$

The stochastic integral 

$$
\int_ {t _ {1}} ^ {t _ {2}} X (t) \mathrm{d} Y (t)
$$

was defined pathwise for integrators Y that are Brownian motions $( \mathrm { d } Y = \mathrm { d } W )$ and for integrands X belonging to the class of integrands of the Ito integral. We extend the definition ofˆ the stochastic integral to integrators that are Ito processes:ˆ 

Definition 44 (Integral with Ito Process as Integrator):ˆ 

Let Y denote an Ito process of the fromˆ 

$$
\mathrm{d} Y = \mu \mathrm{d} t + \sigma \mathrm{d} W
$$

and X a stochastic process such that $X ( t ) \mu ( t )$ is integrable with respect to t and $X ( t ) \sigma ( t )$ is integrable with respect to $W ( t )$ . Then we define 

$$
\int_ {t _ {1}} ^ {t _ {2}} X (t) \mathrm{d} Y (t) := \int_ {t _ {1}} ^ {t _ {2}} X (t) \mu (t) \mathrm{d} t + \int_ {t _ {1}} ^ {t _ {2}} X (t) \sigma (t) \mathrm{d} W (t).
$$

As in Remark 43 we will write 

$$
X (t) \mathrm{d} Y (t) := X (t) \mu (t) \mathrm{d} t + X (t) \sigma (t) \mathrm{d} W (t).
$$

## 2.6.3. Ito Lemma and Product Ruleˆ

Theorem 45 (Ito Lemmaˆ $( \mathbf { 1 } \ \mathbf { D } ) ^ { 2 0 } ) \colon$ Let X denote an Ito process withˆ 

$$
\mathrm{d} X (t) = \mu \mathrm{d} t + \sigma \mathrm{d} W.
$$

Let $g ( t , x ) \in C ^ { 2 } ( [ 0 , \infty ] \times \mathbb { R } )$ . Then 

$$
Y (t) := g (t, X (t))
$$

is an Ito process withˆ 

$$
\mathrm{d} Y = \frac {\partial g}{\partial t} (t, X (t)) \mathrm{d} t + \frac {\partial g}{\partial x} (t, X (t)) \mathrm{d} X + \frac {1}{2} \frac {\partial^ {2} g}{\partial x ^ {2}} (t, X (t)) \cdot (\mathrm{d} X) ^ {2},\tag{2.4}
$$

where $( \mathrm { d } X ) ^ { 2 } = ( \mathrm { d } X ) \cdot ( \mathrm { d } X )$ is given by formal expansion using 

$$
\begin{array}{c} \mathrm{d} t \cdot \mathrm{d} t = 0, \\ \mathrm{d} W \cdot \mathrm{d} t = 0, \end{array}
$$

$$
\begin{array}{c} \mathrm{d} t \cdot \mathrm{d} W = 0, \\ \mathrm{d} W \cdot \mathrm{d} W = \mathrm{d} t, \end{array}
$$

i.e. 

$$
\begin{array}{r l} & {(\mathrm{d} X) ^ {2} = (\mathrm{d} X) \cdot (\mathrm{d} X) = (\mu \mathrm{d} t + \sigma \mathrm{d} W) \cdot (\mu \mathrm{d} t + \sigma \mathrm{d} W)} \\ & {\qquad = \mu^ {2} \cdot \mathrm{d} t \cdot \mathrm{d} t + \mu \cdot \sigma \cdot \mathrm{d} t \cdot \mathrm{d} W + \mu \cdot \sigma \cdot \mathrm{d} W \cdot \mathrm{d} t + \sigma^ {2} \cdot \mathrm{d} W \cdot \mathrm{d} W = \sigma^ {2} \mathrm{d} t} \end{array}
$$

Theorem 46 (Itoˆ $\mathbf { L e m m a } ^ { 2 1 } )$ : Let X denote an n-dimensional, m-factorial Ito process withˆ 

$$
\mathrm{d} X (t) = \mu \mathrm{d} t + \sigma \mathrm{d} W.
$$

Let $g ( t , x ) \in C ^ { 2 } ( [ 0 , \infty ] \times \mathbb { R } ^ { n } ; \mathbb { R } ^ { d } ) , g = ( g _ { 1 } , \ldots , g _ { d } ) ^ { \mathsf { T } }$ . Then 

$$
Y (t) := g (t, X (t))
$$

is an d-dimensional, n-factorial Ito process withˆ 

$$
\begin{array}{l} \mathrm{d} Y _ {k} (t) = \frac {\partial g _ {k}}{\partial t} (t, X (t)) \mathrm{d} t + \sum_ {i = 1} ^ {n} \frac {\partial g _ {k}}{\partial x _ {i}} (t, X (t)) \mathrm{d} X _ {i} (t) \\ \qquad + \frac {1}{2} \sum_ {i, j = 1} ^ {n} \frac {\partial^ {2} g _ {k}}{\partial x _ {i} x _ {j}} (t, X (t)) \cdot (\mathrm{d} X _ {i} (t) \cdot \mathrm{d} X _ {j} (t)), \end{array}
$$

where $\mathrm { d } X _ { i } ( t ) \mathrm { d } X _ { j } ( t )$ is given by formal expansion using 

$$
\begin{array}{c} \mathrm{d} t \cdot \mathrm{d} t = 0, \\ \mathrm{d} W _ {i} \cdot \mathrm{d} t = 0, \end{array}
$$

$$
\begin{array}{c} \mathrm{d} t \cdot \mathrm{d} W _ {j} = 0, \\ \mathrm{d} W _ {i} \cdot \mathrm{d} W _ {j} = \left\{ \begin{array}{l l} \mathrm{d} t & i = j \\ 0 & i \neq j \end{array} \right.. \end{array}
$$

Theorem 47 (Product Rule): Let X, Y and $X _ { 1 } , \ldots , X _ { n }$ denote Ito processes. Then we haveˆ 

1. $\mathrm { d } ( X \cdot Y ) = Y \cdot \mathrm { d } X + X \cdot \mathrm { d } Y + \mathrm { d } X \cdot \mathrm { d } Y$ 

2. 

$$
\mathrm{d}\left(\prod_{i = 1}^{N}X_{i}\right) = \sum_{i = 1}^{N}\prod_{\substack{k = 1\\ k\neq i}}^{N}X_{k}\cdot \mathrm{d}X_{i} + \sum_{\substack{i,j = 1\\ j > i}}^{N}\prod_{\substack{k = 1\\ k\neq i,j}}^{N}X_{k}\cdot \mathrm{d}X_{i}\mathrm{d}X_{j}
$$

Proof: We prove only 1 since 2 follows from 1 by induction. We apply the Ito lemma to theˆ map 

$$
g: \mathbb {R} \times \mathbb {R} \times \mathbb {R} \to \mathbb {R}, \qquad g (t, x, y) := x \cdot y.
$$

We have 

$$
\frac {\partial g}{\partial t} = 0 \quad \frac {\partial g}{\partial x} = y \quad \frac {\partial g}{\partial y} = x
$$

$$
{\frac {\partial g ^ {2}}{\partial x ^ {2}}} = 0 \qquad \qquad {\frac {\partial g ^ {2}}{\partial y ^ {2}}} = 0
$$

$$
{\frac {\partial g ^ {2}}{\partial x y}} = 1 \qquad \qquad {\frac {\partial g ^ {2}}{\partial y x}} = 1
$$

and thus 

$$
\mathrm{d} (X \cdot Y) = \mathrm{d} (g (X, Y)) = Y \cdot \mathrm{d} X + X \cdot \mathrm{d} Y + \mathrm{d} X \cdot \mathrm{d} Y.
$$

| 

Theorem 48 (Quotient Rule): Let X and Y and $Y _ { 1 } , \ldots , Y _ { n }$ denote Ito processes where,ˆ $Y > c$ for a given $c \in \mathbb { R }$ . Then we have 

1. 

$$
\mathrm{d} \left(\frac {X}{Y}\right) = \frac {X}{Y} \left(\frac {\mathrm{d} X}{X} - \frac {\mathrm{d} Y}{Y} - \frac {\mathrm{d} X}{X} \cdot \frac {\mathrm{d} Y}{Y} + \left(\frac {\mathrm{d} Y}{Y}\right) ^ {2}\right)
$$

2. 

$$
\mathrm{d} \left(\frac {1}{Y}\right) = - \frac {1}{Y ^ {2}} \mathrm{d} Y + \frac {1}{Y ^ {3}} \mathrm{d} Y \mathrm{d} Y
$$

3. 

$$
\mathrm{d} \left(\prod_ {i = 1} ^ {N} \frac {1}{Y _ {i}}\right) = \prod_ {i = 1} ^ {N} \frac {1}{Y _ {i}} \cdot \sum_ {i = 1} ^ {N} \left(\frac {- \mathrm{d} Y _ {i}}{Y _ {i}} + \sum_ {j \geq i} ^ {N} \frac {\mathrm{d} Y _ {i}}{Y _ {i}} \frac {\mathrm{d} Y _ {j}}{Y _ {j}}\right)
$$

Lemma 49 (Drift Adjustment of Lognormal Process): Let $S \left( t \right) > 0$ denote an Ito processˆ of the form 

$$
\mathrm{d} S (t) = \mu (t) S (t) \mathrm{d} t + \sigma (t) S (t) \mathrm{d} W (t),
$$

and $Y ( t ) : = \log ( S ( t ) )$ . Then we have 

$$
\mathrm{d} Y (t) = (\mu (t) - \frac {1}{2} \sigma^ {2} (t)) \mathrm{d} t + \sigma (t) \mathrm{d} W (t).
$$

Proof: See Exercise 8. 

| 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/f3833aa015d8a1a7d3a76d530a4eef7d1f689ed0cc95a23567aad349c8a7b55c.jpg)


Interpretation: The Ito lemma and its implications like Lemmaˆ 49 may appear unfamiliar. They state that a non-linear function of a stochastic process will induce a drift of the mean. This may be seen in an elementary example: Consider the time-discrete stochastic process $X ( t _ { i } )$ constructed from binomial distributed 

increments $\Delta B ( t _ { i } )$ (instead of Brownian increments $\mathrm { d } W ( t ) )$ , where $\Delta B ( t _ { i } )$ are independent and attain with probability $\begin{array} { r } { p = \frac { 1 } { 2 } } \end{array}$ the value $+ 1 \mathrm { o r } - 1$ , respectively. Assuming $X ( t _ { 0 } ) = 1 0$ we draw the process 

$$
X (t _ {i + 1}) = X (t _ {i}) + \Delta B (t _ {i})
$$

in Figure 2.9 (left), i.e. $\Delta X ( t _ { i } ) = \Delta B ( t _ { i } )$ . This process does not exhibit a drift. We have 

$$
X (t _ {i}) = \operatorname{E} (X (t _ {i + 1}) \mid \mathcal {F} _ {t _ {i}}).
$$

In other words: In each node in Figure 2.9 the process X attains the mean of the values from the two child nodes. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/8cb3776a35cc66b71fa3e180a9338929f22202ebf517ecf8ff4b45d53271f365.jpg)



Figure 2.9.: Non-linearfunctions ofstochastic processes induce a drift to the mean.


As in Figure 2.9 (right) we then consider the process $Y ( t _ { i } ) = f ( X ( t _ { i } ) ) = X ( t _ { i } ) ^ { 2 }$ . This process exhibits in each time step a drift of the mean of +1. One can easily check that the increments of the process Y are given by 

$$
Y (t _ {i + 1}) = Y (t _ {i}) + 1 + 2 \cdot X (t _ {i}) \cdot \Delta B (t _ {i})
$$

(check this in Figure 2.9). This corresponds to the result stated by Ito’s lemma (see Theoremˆ 45 with $g ( t , x ) = f ( x ) = x ^ { 2 } )$ . Indeed we have 

$$
\begin{array}{r l} & Y (t _ {i + 1}) = (X (t _ {i + 1})) ^ {2} = (X (t _ {i}) + \Delta X (t _ {i})) ^ {2} \\ & \quad = X (t _ {i}) ^ {2} + \Delta X (t _ {i}) ^ {2} + 2 \cdot X (t _ {i}) \cdot \Delta X (t _ {i}) \\ & \quad = Y (t _ {i}) + \Delta B (t _ {i}) ^ {2} + 2 \cdot X (t _ {i}) \cdot \Delta B (t _ {i}) \\ & \quad = Y (t _ {i}) + 1 + 2 \cdot X (t _ {i}) \cdot \Delta B (t _ {i}) \\ & \quad = Y (t _ {i}) + \frac {1}{2} \frac {\partial^ {2} f}{\partial x ^ {2}} (X (t _ {i})) \cdot (\Delta X (t _ {i})) ^ {2} + \frac {\partial f}{\partial x} (X (t _ {i})) \Delta X (t _ {i}). \end{array}
$$

Obviously we may interpret Ito formula (ˆ 2.4) in Ito’s lemma as a (formal) Taylor expansionˆ of $g ( X + \mathrm { d } X )$ up to the order $( \mathrm { d } X ) ^ { 2 }$ . For the continuous case the higher order increments are (almost surely) 0. For the discrete case this is not the case. E.g. consider $( X ( t _ { i } ) + \Delta X ( t _ { i } ) ) ^ { 3 }$ in the example above. C| 

## 2.7. Brownian Motion with Instantaneous Correlation

In Definition 28 Brownian motion was defined through normal distributed increments $W ( t ) -$ $W ( s ) , t > s$ having covariance matrix $( t - s ) I _ { n }$ . In other words, for $W = ( W _ { 1 } , \ldots , W _ { n } )$ the components are one-dimensional Brownian motions with pairwise independent increments, i.e. for $i \neq j$ we have that $W _ { i } ( t ) - W _ { i } ( s )$ and $W _ { j } ( t ) - W _ { j } ( s )$ are independent (thus uncorrelated). 

We define the Brownian motion with instantaneously correlated increments as a special Itoˆ process: 

## Definition 50 (Brownian Motion with instantaneous correlated Increments):

Let U denote an m-dimensional Brownian motion as defined in Definition 28. Let $f _ { i , j } ( i =$ $1 , \ldots , n , j = 1 , \ldots , m )$ denote stochastic processes belonging to the class of integrands of the Ito integral (see Definitionˆ 39 and Definition 42) with 

$$
P \left(\int_ {0} ^ {t} f _ {i, j} (\tau , \omega) ^ {2} \mathrm{d} \tau <   \infty \forall t \geq 0\right) = 1 \quad i = 1, \dots , n, j = 1, \dots , m,
$$

furthermore let 

$$
F (t) := (f _ {1}, \ldots , f _ {m}) := \left( \begin{array}{c c c} f _ {1, 1} (t) & \ldots & f _ {1, m} (t) \\ \vdots & & \vdots \\ f _ {n, 1} (t) & \ldots & f _ {n, m} (t) \end{array} \right)
$$

denote an n × m matrix with 

$$
\sum_ {j = 1} ^ {m} f _ {i, j} ^ {2} (t) = 1, \quad \forall i = 1, \ldots , n.
$$

Then the Ito processˆ 

$$
\mathrm{d} W (t) = F (t) \cdot \mathrm{d} U (t), \qquad W (0) = 0
$$

(see Definition 42) is called m-factorial, n-dimensional Brownian motion with factors $f _ { j } , j =$ $1 , \ldots , m$ . With $R : = F F ^ { \mathrm { T } }$ we call R the instantaneous correlation and W a Brownian motion with instantaneous correlation R. F is called thefactor matrix. y 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/79fa595770e4fde7467766797b0bcd3e9a896c4d74883d38d3d692f35edfd448.jpg)


Interpretation: For simplicity let us consider a constant matrix ${ \cal F } = $ $( f _ { 1 } , \ldots , f _ { m } )$ . Then we have for time-discrete increments 

$$
\Delta W (T _ {k}) = F \cdot \Delta U (T _ {k}) = f _ {1} \Delta U _ {1} (T _ {k}) + \ldots + f _ {m} \Delta U _ {m} (T _ {k}).\tag{2.5}
$$

Note that $\Delta U _ { i } ( T _ { k } )$ and $\Delta U _ { j } ( T _ { k } )$ are independent. They may be interpreted as independent scenarios. If <sub>ω</sub> is a path with $\Delta U _ { i } ( T _ { k } ; \omega ) \neq 0$ and $\Delta U _ { j } ( T _ { k } ; \omega ) = 0$ for $j \neq i ,$ then we have from (2.5) that $\Delta W ( T _ { k } ; \omega ) = f _ { i } \cdot \Delta U _ { i } ( T _ { k } ; \omega )$ , i.e. on the path the vector W will receive increments corresponding to the scenario $f _ { i }$ (multiplied the amplitude $\Delta U _ { i } ( T _ { k } ; \omega ) )$ . If, for example, $f _ { 1 } = ( 1 , \ldots , 1 ) ^ { \mathrm { T } }$ then the scenario corresponds parallel shift of W (by the shift size $\Delta U _ { 1 } ( T _ { k } ) )$ . 

Our definition of a factor matrix does not allow arbitrary scenarios since we require that $\textstyle \sum _ { j = 1 } ^ { m } f _ { i , j } ^ { 2 } ( t ) = 1$ , i.e. that $R : = F F ^ { \mathrm { T } }$ is a correlation matrix. By this assumption we ensure that the components of $W _ { i }$ of W are one-dimensional Brownian motions in the sense of Definition 28. 

By means of the factor matrix F we may interpret the implied correlation structure R in a geometrical way. The calculation of F from a given R is a Cholesky decomposition. 

We will make use of this construction in the modeling of interest rate curves (Chapter 19: LIBOR Market Model). Here the interpretation of the factors is given by movements of the interest rate curve. The possible shapes of an interest rate curve will then be investigated (Chapter 24)). The question of how to obtain a set of factors or reduce a given set of factors to the relevant ones is discussed in Appendix A.3 and A.4. C| 

## 2.8. Martingales

## Definition 51 (Martingale):

The stochastic process $\{ X ( t ) , \mathcal { F } _ { t } : 0 \leq t < \infty \}$ is called a martingale with respect to the filtration $\{ \mathcal { F } _ { t } \}$ and the measure P if 

$$
X _ {s} = E (X (t) \mid \mathcal {F} _ {s}) \quad P \text {   almost   sure, } \quad \forall 0 \leq s <   t <   \infty .\tag{2.6}
$$

If (2.6) holds for ≤ in place of =, then X is called sub-martingale. If (2.6) holds for ≥ in place of =, then X is called super-martingale. y 

Lemma 52 (Martingale Ito-Processes are drift-free): ˆ Let X denote an Ito process of the ˆ form 

$$
\mathrm{d} X = \mu \mathrm{d} t + \sigma \mathrm{d} W \quad \text { under } P
$$

with $\mathrm { E } ^ { P } \Big ( \big ( \int _ { 0 } ^ { T } \sigma ^ { 2 } ( t ) \ : \mathrm { d } t \big ) ^ { 1 / 2 } \Big ) < \infty$ . Then we have 

$$
X \text {   is   a   } P \text {   martingale   } \Leftrightarrow \mu = 0 \quad \text {(i.e.   } X \text {   is   drift - free) }.
$$

## 2.8.1. Martingale Representation Theorem

Theorem 53 (Martingale Representation Theorem<sup>22</sup>): Let $W ( t ) = ( W _ { 1 } ( t ) , \ldots , W _ { m } ( t ) ) ^ { \intercal }$ denote an m-dimensional Brownian motion, F the corresponding filtration. Let M(t) denote a martingale with respect to $\mathcal { F } _ { t }$ with $\int _ { \Omega } | M ( t ) | ^ { 2 } \mathrm { d } P < \infty ( \forall t \dot { \geq } 0 )$ 

Then there exists a stochastic process $g$ (with g(t) belonging to the class of integrands of the Ito integral) withˆ 

$$
M (t) = M (0) + \int_ {0} ^ {t} g (s) \mathrm{d} W (s) \quad P \text {   almost   sure,   } \forall t \geq 0.
$$

## 2.9. Change of Measure (Girsanov, Cameron, Martin)

## Definition 54 (Measure with Density):

Let $( \Omega , { \mathcal { F } } , P )$ denote a measure space and φ a P integrable non-negative real valued random variable. Then 

$$
Q (A) := \int_ {A} \phi \mathrm{d} P
$$

defines a measure on (Ω F ) which we call measure with density φ with respect to $P .$ y 

Definition 55 (Equivalent Measure): 

Let P and Q denote two measures on the same measurable space (Ω F). 

1. Q is called continuous with respect to $\begin{array} { r l } { P } & { { } \Leftrightarrow \quad \left( P ( A ) = 0 \Rightarrow Q ( A ) = 0 \forall A \in { \mathcal { F } } \right) } \end{array}$ 

2. P and Q are called equivalent $\begin{array} { r l } { \Leftrightarrow \ } & { { } \left( P ( A ) = 0 \Leftrightarrow Q ( A ) = 0 \forall A \in { \mathcal { F } } \right) } \end{array}$ 

Theorem 56 (Radon-Nikodym Density): ´ Let P and Q denote two measures on a measurable space (Ω F). Then we have 

Q is continuous with respect to P ⇔ Q has a density with respect to $P .$ 

Proof: See [1]. 

## Definition 57 (Radon-Nikodym Density):´

If Q is continuous with respect to P then we call the density of Q with respect to P the Radon-Nikod´ym density and denote it by $\frac { \mathrm { d } Q } { \mathrm { d } P }$ y 

Theorem 58 (Change of Measure (Girsanov, Cameron, Martin)): Let W denote a $( d \cdot$ dimensional) P-Brownian motion and $\{ \mathcal { F } _ { t } \}$ the filtration generated by W fulfilling the usual conditions<sup>23</sup>. Let Q denote a measure equivalent to P (w.r.t. {F}). 

1. Then there exists a {F}-previsible process C with 

$$
\left. \frac {\mathrm{d} Q}{\mathrm{d} P} \right| _ {\mathcal {F} _ {t}} = \exp \left(\int_ {0} ^ {t} C (s) \mathrm{d} W (s) - \frac {1}{2} \int_ {0} ^ {t} | C (s) | ^ {2} \mathrm{d} s\right).\tag{2.7}
$$

2. Let $T > 0$ fixed. Reversed, if $\rho$ denotes a strictly positive P-martingale with respect to $\{ \mathcal { F } _ { t } \mid t \in [ 0 , T ] \}$ with $\mathrm { E } ^ { P } ( \rho ) = \overset { \cdot } { 1 }$ , then $\rho ( t )$ has the representation (2.7) and defines (as a Radon-Nikodym process) a measure´ $Q = Q ^ { T }$ which is equivalent to $P$ with respect to ${ \mathcal { F } } _ { T } ,$ , given by 

$$
Q (A) := \int_ {A} \rho (T) \mathrm{d} P \quad \forall A \in \mathcal {F} _ {T}.\tag{2.8}
$$

<sup>23</sup> Given a complete, filtered probability space $( \Omega , { \mathcal { F } } , \{ { \mathcal { F } } _ { t } ~ | t \in [ 0 , T ] \} , P ) .$ the filtration $\{ \mathcal { F } _ { t } \mid t \in [ 0 , T ] \}$ satisfies the “usual conditions”, if it is right-continuous (i.e. $\mathcal { F } _ { t } = \cap _ { \epsilon > 0 } \mathcal { F } _ { t + \epsilon } )$ and $\mathcal { F } _ { 0 }$ (and thus $\mathcal { F } _ { t }$ for every $t \in [ 0 , t ] )$ contains all P-nullsets of $\mathcal { F }$ . 

In any given case 

$$
\tilde {W} (t) := W (t) - \int_ {0} ^ {t} C (s) d s\tag{2.9}
$$

is a Q-Brownian motion (with respect to $\{ \mathcal { F } _ { t } \} )$ (and for $t \leq T$ in the second case). 

Remark 59 (Change of Measure - Change of Drift): Equation (2.9) may be written as 

$$
\mathrm{d} \tilde {W} (t) = - C (t) \mathrm{d} t + \mathrm{d} W (t)\tag{2.10}
$$

and we see that the change of measure (2.7) corresponds to a change of drift (2.10). The second case has a restriction on a finite time horizon $T .$ , which will be irrelevant in the following applications. 

Remark 60 (Radon-Nikodym process): ´ Note that 

$$
\rho (t) := \exp \left(\int_ {0} ^ {t} C (s) \mathrm{d} W (s) - \frac {1}{2} \int_ {0} ^ {t} | C (s) | ^ {2} \mathrm{d} s\right).
$$

is a P-martingale. From this we have that for $A \in { \mathcal { F } } _ { t }$ 

$$
\begin{array}{l} Q (A) := \int_ {A} \rho (T) \mathrm{d} P = \mathrm{E} ^ {P} (\mathbf {1} _ {A} \cdot \rho (T)) = \mathrm{E} ^ {P} \left(\mathrm{E} ^ {P} (\mathbf {1} _ {A} \cdot \rho (T) | \mathcal {F} _ {t})\right) \\ \stackrel {{\text {(B.1)}}} {{=}} \mathrm{E} ^ {P} \left(\mathbf {1} _ {A} \cdot \mathrm{E} ^ {P} (\rho (T) | \mathcal {F} _ {t})\right) = \mathrm{E} ^ {P} (\mathbf {1} _ {A} \cdot \rho (t)) = \int_ {A} \rho (t) \mathrm{d} P. \end{array}
$$

Thus, $\rho$ definies a process of consistent Radon-Nikodym densities´ $\left. \frac { \mathrm { d } Q } { \mathrm { d } P } \right| _ { \mathcal { F } _ { t } } \mathrm { o n } \left( \Omega , \mathcal { F } _ { t } \right)$ 

Exercise: (Change of Measure in a binomial tree): Calculate the probabilities (the measure) such that the process Y depicted in Figure 2.9 is a martingale. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/13a51fd2c7f63660d0fe07c51997928adac525fd32620bc185fdf4322fea4dfe.jpg)


Interpretation: The form of the change of measure (2.7) may be motivated via a simple calculation and derived for a time-discrete Ito processˆ 

$$
\Delta X (T _ {i}) = \mu (T _ {i}) \Delta T _ {i} + \sigma (T _ {i}) \Delta W (T _ {i})
$$

by elementary calculations. 

At first: Let Z denote a normal distributed random variable with mean 0 and standard deviation on a probability space $( \Omega , { \mathcal { F } } , P )$ . Under which measure will Z be normal distributed with mean c and standard deviation $\sigma ?$ The density of a normal distributed random variable with mean c and standard deviation is $\begin{array} { r } { z \mapsto \frac { 1 } { \sqrt { 2 \pi } \sigma } \exp ( - \frac { ( z - c ) ^ { 2 } } { 2 \sigma ^ { 2 } } ) } \end{array}$ Thus we seek a change of measure $\frac { \mathrm { d } Q } { \mathrm { d } P }$ such that 

$$
\underbrace {\frac {1}{2 \sqrt {\pi} \sigma} \exp (- \frac {(z - c) ^ {2}}{2 \sigma^ {2}})} _ {\frac {\mathrm{d} Q}{\mathrm{d} z} = \text {desired density under} Q} \mathrm{d} z = \mathrm{d} Q = \frac {\mathrm{d} Q}{\mathrm{d} P} \mathrm{d} P = \underbrace {\frac {1}{2 \sqrt {\pi} \sigma} \exp (- \frac {z ^ {2}}{2 \sigma^ {2}})} _ {\frac {\mathrm{d} P}{\mathrm{d} z} = \text {known density under} P} \underbrace {\frac {\mathrm{d} Q}{\mathrm{d} P}} _ {= ?} \mathrm{d} z.
$$

With 

$$
\exp (- \frac {(z - c) ^ {2}}{2 \sigma^ {2}}) = \exp (- \frac {z ^ {2} - 2 c z + c ^ {2}}{2 \sigma^ {2}}) = \exp (- \frac {z ^ {2}}{2 \sigma^ {2}}) \exp (\frac {c z - \frac {1}{2} c ^ {2}}{\sigma^ {2}})
$$

it follows that the desired change of measure is 

$$
\frac {\mathrm{d} Q}{\mathrm{d} P} = \exp (\frac {c z - \frac {1}{2} c ^ {2}}{\sigma^ {2}}).\tag{2.11}
$$

This corresponds to the term in (2.7). 

To illustrate this we consider the time-discrete process 

$$
\Delta X (T _ {i}) = \mu^ {P} (T _ {i}) \Delta T _ {i} + \sigma (T _ {i}) \Delta W (T _ {i}) \quad \text { under } P.
$$

Under which measure is $X \mathrm { a }$ (time-discrete) martingale? We have: 

$$
\begin{array}{r l} X \text {is a Q -martingale} & \Leftrightarrow \mu^ {Q} (T _ {i}) = 0 \Leftrightarrow \mathrm{E} ^ {Q} (\Delta X (T _ {i}) | \mathcal {F} _ {T _ {i}}) = 0 \\ & \Leftrightarrow \mathrm{E} ^ {Q} (\frac {1}{\sigma (T _ {i})} \Delta X (T _ {i}) | \mathcal {F} _ {T _ {i}}) = 0 \end{array}
$$

First consider a single increment: The random variable 

$$
\frac {1}{\sigma (T _ {i})} \Delta X (T _ {i}) = \frac {\mu (T _ {i})}{\sigma (T _ {i})} \cdot \Delta T _ {i} + \Delta W (T _ {i})
$$

is (under P) normal distributed with mean $\frac { \mu ( T _ { i } ) } { \sigma ( T _ { i } ) } \cdot \Delta T _ { i }$ and standard deviation $\sqrt { \Delta { T _ { i } } }$ . For the conditional (!) expectation under Q we have 

$$
\mathrm{E} ^ {Q} (\frac {1}{\sigma (T _ {i})} \Delta X (T _ {i}) | \mathcal {F} _ {T _ {i}}) = \frac {\mu (T _ {i})}{\sigma (T _ {i})} \cdot \Delta T _ {i} + \mathrm{E} ^ {Q} (\Delta W (T _ {i}) | \mathcal {F} _ {T _ {i}})
$$

Then $\begin{array} { r } { \mathrm { E } ^ { \mathcal { Q } } ( \frac { 1 } { \sigma ( T _ { i } ) } \Delta X ( T _ { i } ) \mid \mathcal { F } _ { T _ { i } } ) = 0 \mathrm { i f } \mathrm { E } ^ { \mathcal { Q } } ( \Delta W ( T _ { i } ) \mid \mathcal { F } _ { T _ { i } } ) = C ( T _ { i } ) \Delta T _ { i } } \end{array}$ where $\begin{array} { r } { C ( T _ { i } ) = - \frac { \mu ( T _ { i } ) } { \sigma ( T _ { i } ) } } \end{array}$ (we correct for the drift). Given the considerations above we have to apply a change of measure 

$$
\left. \frac {\mathrm{d} Q}{\mathrm{d} P} \right| _ {\Delta T _ {i}} := \exp (C (T _ {i}) \Delta W (T _ {i}) - \frac {1}{2} C (T _ {i}) ^ {2} \Delta T _ {i})
$$

for the time step $\Delta T _ { i }$ (apply (2.11) with $Z = \Delta W ( T _ { i } ) , c = C ( T _ { i } ) \Delta T _ { i }$ and $\sigma = \sqrt { \Delta { T } _ { i } } )$ 

This is just the change of measure needed to make the increment $\Delta X ( T _ { i } )$ drift-free. Since the increments $\Delta W ( T _ { i } )$ are independent we get the change of measure for the process X from $T _ { 0 }$ to $T _ { n }$ by multiplying the Radon-Nikodym densities, i.e. 

$$
\begin{array}{l} \frac {\mathrm{d} Q}{\mathrm{d} P} \Big | _ {T _ {n}} := \prod_ {i = 0} ^ {n - 1} \frac {\mathrm{d} Q}{\mathrm{d} P} \Big | _ {\Delta T _ {i}} = \prod_ {i = 0} ^ {n - 1} \exp (C (T _ {i}) \Delta W (T _ {i}) - \frac {1}{2} C (T _ {i}) ^ {2} \Delta T _ {i}) \\ \qquad = \exp (\sum_ {i = 0} ^ {n - 1} C (T _ {i}) \Delta W (T _ {i}) - \frac {1}{2} \sum_ {i = 0} ^ {n - 1} C (T _ {i}) ^ {2} \Delta T _ {i}). \end{array}\tag{2.12}
$$

The change of measure $\left. \frac { \mathrm { d } Q } { \mathrm { d } P } \right| _ { T _ { n } }$ will make all increments $\Delta X ( T _ { i } )$ drift-free for $i = 0 , \ldots , n - 1$ Due to the independence of the increments $\Delta W ( T _ { i } )$ we obtain independence of the $\left. \frac { \mathrm { d } Q } { \mathrm { d } P } \right| _ { \Delta T _ { i } }$ and thus 

$$
\mathrm{E} ^ {Q} (\Delta W (T _ {i})) = \mathrm{E} ^ {P} (\Delta W (T _ {i}) \cdot \prod_ {j = 0} ^ {n - 1} \frac {\mathrm{d} Q}{\mathrm{d} P} \Big | _ {\Delta T _ {j}}) = \prod_ {j \neq i} \underbrace {\mathrm{E} ^ {P} (1 \cdot \frac {\mathrm{d} Q}{\mathrm{d} P} \Big | _ {\Delta T _ {j}})} _ {= 1} \cdot \mathrm{E} ^ {P} (\Delta W (T _ {i}) \cdot \frac {\mathrm{d} Q}{\mathrm{d} P} \Big | _ {\Delta T _ {i}}).
$$

The term (2.12) is a discrete version of (2.7). To some extent we have just proven a version of the change of measure theorem for time-discrete Ito processes.ˆ 

The term $- C ( t ) ^ { 2 } \mathrm { d } t$ in (2.7) $( \mathrm { o r } - C ( T _ { i } ) ^ { 2 } \Delta T _ { i }$ in (2.12)) may also be motivated as follows: The random variable 10 

$$
Z (t) := \left. \frac {\mathrm{d} Q}{\mathrm{d} P} \right| _ {\mathcal {F} _ {t}}
$$

represents a density of the measure $Q | _ { \mathcal { F } _ { t } }$ with respect to the measure $P | _ { \mathcal { F } _ { t } }$ . Since $Q | _ { \mathcal { F } _ { t } }$ should be a probability measure we must have 

$$
Q | _ {\mathcal {F} _ {t}} (\Omega) = \mathrm{E} ^ {P | _ {\mathcal {F} _ {t}}} (Z (t)) = 1\tag{2.13}
$$

and with $Z ( 0 ) = 1$ this follows if Z is a martingale. Thus the drift correction $- C ( t ) ^ { 2 } \mathrm { d } t$ t follows from Lemma 49, because Z is a lognormal process. C| 

## 2.10. Stochastic Integration

In the previous sections the following integrals were considered: 

Maps: Maps: 

$\int _ { t _ { 1 } } ^ { t _ { 2 } } f ( t ) \mathrm { d } t$ Lebesgue or Riemann integral. Integral of a real valued function with respect to t. 

Random Variables: 

$\int _ { \Omega } Z ( \omega ) \mathrm { d } { \cal P } ( \omega )$ Lebesgue integral. Integral of a random variable Z with respect to a measure P (cf. expectation). 

Stochastic Processes: 

$\int _ { \Omega } X ( t _ { 1 } , \omega ) \mathrm { d } P ( \omega )$ Lebesgue integral. Integral of a random variable $X ( t _ { 1 } )$ with respect to a measure P. 

$\int _ { t _ { 1 } } ^ { t _ { 2 } } X ( t ) \mathrm { d } t$ Lebesgue Integral or Riemann integral. The (pathwise) integral of the stochastic process X with respect to t. 

$\int _ { t _ { 1 } } ^ { t _ { 2 } } X ( t ) \mathrm { d } W ( t )$ Ito integral.ˆ The (pathwise) integral of the stochastic process X with respect to a Brownian motion W. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/c1275e709a644ab7226c2fe1e50649c3f816300b8669dd5c5b806e8424b07a4b.jpg)



Figure 2.10.: Integration ofstochastic processes


The notion of a stochastic integral may be extended to more general integrands and/or more general integrators. For completeness we mention: 

## Definition 61 (Previsible Process):

Let X denote a (real valued) stochastic process on $( \Omega , { \mathcal { F } } )$ and $\{ \mathcal { F } _ { t } \}$ a filtration on $( \Omega , { \mathcal { F } } )$ . The process X is called {F<sub>t</sub>}-previsible, if X is $\{ \mathcal { F } _ { t } \}$ }-adapted and bounded with left continuous paths. y 

Definition 62 (Integral with respect to a semi-martingale as integrator<sup>24</sup>): Let Y denote a semi-martingale of the form 

$$
Y (t) = A (t) + M (t),
$$

where $A ( t )$ is a process with locally bounded variation and $M ( t )$ a local martingale. Let X(t) denote a previsible process. Then we define 

$$
\int_ {t _ {1}} ^ {t _ {2}} X (t) \mathrm{d} Y (t) := \int_ {t _ {1}} ^ {t _ {2}} X (t) \mathrm{d} A (t) + \int_ {t _ {1}} ^ {t _ {2}} X (t) \mathrm{d} M (t).
$$

Remark 63 (Stochastic Integral): The class of processes (integrands) for which we may define a stochastic integral depends on the properties of the integrators (and vice versa). For continuous integrators (as the Brownian motion) the integrands merely have to be adapted processes. To allow more general integrators one has to restrict to a smaller class of integrands, e.g. previsible processes. Compare Example 4.1 and Remark 4.4 in [14]. For more detailed discussion of the stochastic integral see [6], §5.5 and (especially for more general integrators) [14], §4 and [20], §3. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/731de214d3caa9b4ffdac2c6f965e8f36d514a5f4735d8638b325706f681e352.jpg)


Further Reading: On stochastic processes: As introduction: [27]. For an in-depth discussion: [20], [29] and [31]. 

C| 

## 2.11. Partial Differential Equations (PDE)

We consider partial diferential equations only marginally. In Section 7.2.2 we derive the Black-Scholes partial diferential equation. The bridge from stochastic diferential equations (SDE) to partial diferential equations (PDE) is given through the following Feynman-Kacˇ theorem. 

## 2.11.1. Feynman-Kac Theoremˇ

Theorem 64 (Feynman-Kac):ˇ Let X denote a d-dimensional Ito process,ˆ $X = ( X _ { 1 } , \ldots , X _ { d } ) $ following the stochastic diferential equation (SDE) 

$$
\mathrm{d} X _ {i} (t) = \mu_ {i} (t, X) \mathrm{d} t + \sigma_ {i} (t, X) \mathrm{d} W _ {i} ^ {\mathbb {Q}} (t) \qquad \text { on } [ 0, T ] \text { under } \mathbb {Q}.
$$

Furthermore let V denote the solution of the parabolic partial diferential equation (PDE) 

$$
\begin{array}{r c l} \frac {\partial V}{\partial t} + \sum_ {i = 1} ^ {d} \mu_ {i} (t, x) \frac {\partial V}{\partial x _ {i}} + \sum_ {i, j = 1} ^ {d} \gamma_ {i, j} (t, x) \frac {\partial^ {2} V}{\partial x _ {i} \partial x _ {j}} & = & 0 \qquad \text {on} I \times \Omega \\ V (T, \cdot) & = & \phi (\cdot) \qquad \text {on} \mathbb {R} ^ {d} \end{array}
$$

with $\gamma _ { i , j } = \sigma _ { i } \sigma _ { j } \rho _ { i , j }$ and $\mathrm d W _ { i } ( t ) \mathrm d W _ { j } ( t ) = \rho _ { i , j } \mathrm d t .$ 

$$
V (t, x) = \mathrm{E} ^ {\mathbb {Q}} (\phi (X (T)) \mid X (t) = x) \qquad \mathrm{for} (t, x) \in [ 0, T ] \times \mathbb {R} ^ {d}\tag{2.14}
$$

Remark 65 (solving backward in time): Note that the PDE solves V backward in time. V is given at the final time T and the PDE described V for $t < T$ . The meaning of this will become apparent in the following interpretation, however, to fully understand the interpretation in our context the knowledge of the next chapter is helpful. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/d8d8f7f1d172803ff6ae7d1f64ea19ced35bf69dacbb3316ce482c1607921ae0.jpg)


Interpretation: A stochastic diferential equation decribes how a stochastic process X changes from X(t) to X(T). The change is the increment $\Delta X = \textstyle \int _ { t } ^ { T }$ dX – a random variable. The increment decribes how values change and give the probability for such a change. 

If we now look at a stochastic process that is a function of X, say $V ( t ) = V ( t , X ( t ) )$ then Ito’sˆ Lemma allows us to derive the stochastic diferential equation for V, i.e. we have a formula for dV. The change from V(t) to V(T) is the increment $\Delta V = \int _ { t } ^ { T } \mathrm { d } V$ , and again, the increment decribes how values change and give the probabilties for such a change. However, the probabilities do not change. If X moves from $X ( t ) = x$ to $X ( T ) = y$ with some (transition) probability density $\phi ( t , x ; T , y )$ , then V moves from $V ( t , x ) = : u$ to $V ( T , y ) = : \nu$ with the same (transition) probability density $\phi ( t , x ; T , y )$ 

So for V just the attained values change. The underlying transition probabilities are the ones of X. These are of course just the direct consequences our assumption that V is a function of X. This assumption “splits” the definition of the stochastic process V into two parts: The transition probabilites are given by X. The values that are attained are given by $( t , x ) \mapsto V ( t , x )$ 

Now, if we consider the function V to be the conditional expectation operator in $( 2 . 1 4 )$ , then it is not surprising that there is a rule of how to calculate V(t) from V(T) using the coeficients of the SDE of X, because these coeficients essentially contain the transition probabilties of X. This rule for calculating V is a partial diferential equation. 

The theorem makes two restrictive assumptions on the process V, namely 

$V ( t )$ is a function of some underlying state variables $X ( t ) .$ , and 

$V ( t )$ is the conditional expectation of $V ( T )$ 

However, as we will learn in the next chapter, under suitable (and meaningful) assumptions all the stochastic processes describing the prices of financial derivatives will fullfil these assumptions. Thus, the theorem allows us to derive the prices of a financial derivative V as a function of some other quantity X through a PDE, given we know that function at some future time T. For financial derivatives, the time T function V(T) is often known (e.g. for a call option on X we know that at time T its value is max $X ( T ) - K , 0 )$ . Solving the PDE gives the function V(0) from V(T). If today’s value $x _ { 0 } : = X ( 0 )$ of X is known, then the function V(0) gives today’s value of V as $V ( 0 , x _ { 0 } )$ C| 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/ae38b744e6965f0b458935da7e88dcf0cea88cced49e04c13e2e45eccbf700c5.jpg)


Further Reading: In [34] a short proof of the Feynman–Kac theorem isˇ given. The instructive books of Wilmott, e.g. [40], give, besides an introduction to mathematical finance, an overview on PDE methods. The numerical methods for pricing derivatives by PDEs are discussed, e.g., in [11, 35, 40]. C| 

## 2.12. List of Symbols

The following list of symbols summarizes the most important concepts from Chapter 2: 

<table><tr><td>Symbol</td><td>Object</td><td>Interpretation</td></tr><tr><td><eq>\omega</eq></td><td>element of <eq>\Omega</eq></td><td>State. In the context of stochastic processes: path.</td></tr><tr><td><eq>\Omega</eq></td><td>set</td><td>State space.</td></tr><tr><td>X</td><td>random variable</td><td>Map which assigns an event / outcome (e.g. a number) to a state. Example: the payoff of a financial product (this may be interpreted as a snapshot of the financial product itself).</td></tr><tr><td>X</td><td>stochastic process</td><td>Sequence (in time) of random variables (e.g. the evolution of a financial product (could be its payoffs but also its value)).</td></tr><tr><td><eq>X(t), X_t</eq></td><td>stochastic process evaluated at time <eq>t</eq>(≡ random variable)</td><td>see above</td></tr><tr><td><eq>X(\omega)</eq></td><td>stochastic process evaluated in state <eq>\omega</eq></td><td>Path of X in state <eq>\omega</eq>.</td></tr><tr><td>W</td><td>Brownian motion</td><td>Model for a continuous (random) movement of a particle with independent increments (position changes).</td></tr><tr><td><eq>\mathcal{F}</eq></td><td><eq>\sigma</eq>-algebra (set of sets)</td><td>Set of information configurations (set of sets of states).</td></tr><tr><td><eq>\{ \mathcal{F}_t \mid t \geq 0 \}</eq></td><td>filtration</td><td><eq>\mathcal{F}_t</eq> is the information known at time <eq>t</eq>.</td></tr></table>

# Replication

Nowadays people know the price of everything and the value of nothing. 

Oscar Wilde The Picture ofDorian Gray, [38] 

## 3.1. Replication Strategies

## 3.1.1. Introduction

We motivate the important principle of replication by considering the simplest financial derivative, theforward contract. Consider the following products: 

A (Forward Contract on Rain): At time $T _ { 1 } > 0$ the amount of rain fallen $R ( T _ { 1 } )$ is measured (in mm) at a predefined place and the $ amount 

$$
A (T _ {1}) := (R (T _ {1}) - X) \cdot \frac {}{\mathrm{mm}}
$$

is paid. Here, X denotes a constant reference amount of rain. 

B (Forward Contract on IBM Stock): At time $T _ { 1 } > 0$ the value $S ( T _ { 1 } )$ of an IBM stock is fixed and the $ amount 

$$
B (T _ {1}) := (S (T _ {1}) - X)
$$

is paid. Here, X denotes a constant reference value. 

These products may be interpreted as a guarantee or insurance.<sup>1</sup> The product A is a weather derivative, the product B is an equity derivative. What is a fair value for the product A and the product B? What do we expect to pay in $T _ { 0 }$ (today) for such a guarantee? 

Consider the product A: It appears that the determination of its fair value requires an exact assessment of the probability of rain at time $T _ { 1 }$ . So let $R _ { T _ { 1 } } : \Omega $ R denote a random variable (rain quantity at time $T _ { 1 }$ , modeled over a suitable probability space – for $\omega \in \Omega$ the $R _ { T _ { 1 } } ( \omega )$ denotes the quantity of rain that falls in state . Then, the random variable $A ( T _ { 1 } ) : = R _ { T _ { 1 } } - X$ defines the payof of product A. We wish to determine the value $A ( T _ { 0 } )$ of this product at time $T _ { 0 }$ 

For the trivial case of a single-point distribution, i.e. 

$$
R _ {T _ {1}} (\omega) = R ^ {*} = \text { const. } \quad \forall \omega \in \Omega ,
$$

i.e. the amount of rain at time $T _ { 1 }$ is $R ^ { * }$ with probability 1, in other words: it is certain that in $T _ { 1 }$ the amount of rain falling is R<sup>∗</sup>. Then the product A pays at time $T _ { 1 }$ the amount $A ^ { * } : = R ^ { * } - X$ with probability 1. In this case, the product corresponds to a savings account. Let $P ( T _ { 0 } )$ denote the value that has to be invested at time $T _ { 0 }$ (into a savings account) to receive in $T _ { 1 }$ (including interest) the amount 1 $( = : P ( T _ { 1 } ) )$ , then the product $\mathbf { A }$ pays in $T _ { 1 }$ the value $A ^ { * }$ -times the value of $P .$ . Since A is equivalent to $A ^ { * }$ times $P ,$ , we have 

$$
A (T _ {0}) = A ^ {*} \cdot P (T _ {0})
$$

(we assumed that the interest rate paid is independent of the amount invested, i.e. the interest is proportional to the amount invested). With $P ( T _ { 1 } ) = 1$ this may be written as 

$$
\frac {A (T _ {0})}{P (T _ {0})} = \frac {A ^ {*}}{P (T _ {1})}.
$$

For the (quite unrealistic) case of a one-point distribution (i.e. a deterministic payment) we may derive the value of the product A by comparing it to the value of another product with deterministic payof (the savings account). 

In the general case, where a probability distribution of $R ( T _ { 1 } )$ is known, it is questionable that we can replace the value $\frac { A ^ { * } } { P ( T _ { 1 } ) }$ by - e.g. - the expectation – 

$$
\frac {A (T _ {0})}{P (T _ {0})} \stackrel {?} {=} \mathrm{E} \left(\frac {A (T _ {1})}{P (T _ {1})}\right)
$$

– if so, this would imply that the risk (for example the variance of $A ( T _ { 1 } ) )$ does not influence the value. Since the product A is an insurance against the risk of variations in rainfall, this appears to be nonsense. 

Product B is very similar to product A. Instead of the amount of rain $R ( T _ { 1 } )$ the value of a stock $S ( T _ { 1 } )$ determines the payout. The considerations of the previous section apply accordingly. However, for B it is possible to determine its value in $T _ { 0 } = 0$ independent of the specific probability distribution of $S ( T _ { 1 } )$ 

In time $T _ { 0 }$ we take a credit with fixed interest rate such that the amount to be repaid at time $T _ { 1 }$ is $X .$ This credit pays us in $T _ { 0 }$ the amount $X \cdot P ( T _ { 1 } ; T _ { 0 } ) . ^ { 2 }$ In addition we acquire the stock at its current market price $S ( T _ { 0 } )$ . In total we have to pay in $T _ { 0 }$ the amount 

$$
V (T _ {0}) = S (T _ {0}) - X P (T _ {1}; T _ {0}).\tag{3.1}
$$

At time $T _ { 1 }$ this portfolio (stock + credit) (replication portfolio) will have the value 

$$
V (T _ {1}) = S (T _ {1}) - X,
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/122c62d6124739b094ed4eec983b4af7b30bee9df3c44ade8f3a675cfde197b2.jpg)



Figure 3.1.: Buy and Hold-replication strategy


i.e. it matches exactly the value of the product B at time $T _ { 1 }$ 

Thus, we have found a strategy (replication strategy) to construct a portfolio for which its value in $T _ { 1 }$ matches our product B exactly. This property is fulfilled in any state $\omega \in \Omega$ independent of the probability distribution of $S ( T _ { 1 } )$ . Furthermore, the cost to acquire the portfolio in $T _ { 0 } , \mathrm { i . e . } V ( T _ { 0 } )$ , is known. As a random variable $B ( T _ { 1 } )$ is indistinguishable from $V ( T _ { 1 } )$ . Thus we have (valuing on a fair basis), that the price $B ( T _ { 0 } )$ of product B is equal to the cost of the portfolio $V ( T _ { 0 } )$ . To determine $V ( T _ { 0 } )$ it is only required to know today’s price for the stock and today’s price for a credit (see Equation (3.1)). 

The replication strategy used in this example is called buy-and-hold, since all parts of the product required for replication are bought at time $T _ { 0 }$ . See Figure 3.1. 

The essential diference between product A and product B is that for product B the quantity that carries the insecurity (the stock) can be bought. In other words, it is possible to buy (and sell) “risk”. We assume that we may buy and sell parts of stocks (and other traded products) in arbitrary (real valued) quantities. 

Th key for the construction of the replication portfolio is that: 

• It is possible to express today’s value of a deterministic future payment and thus there is a vehicle to transfer a deterministic future payment to an earlier time: $P ( T _ { 1 } ; t )$ is a traded product. 

• It is possible to buy or sell the underlying (the risk carrier) at any time in any quantity: $S \left( t \right)$ is a traded product. 

It is a surprising consequence of the construction of a replication portfolio that: 

• The real probabilities do not enter into the current value of the replication portfolio. 

Our strategy is to construct a portfolio at time $T _ { 0 }$ and wait until time $T _ { 1 }$ (buy-and-hold strategy). Obviously the strategy may be refined by restructuring the portfolio at other times. Dynamic (infinitesimal) restructuring will allow the replication of arbitrary (continuous) payouts, given that the underlying random variables (the underlyings) are traded products. It is 

<sup>2</sup> We denote here by $P ( T _ { 1 } ; T _ { 0 } )$ the amount paid by a credit in $T _ { 0 } ,$ which has to be repaid in $T _ { 1 }$ by the amount $1 = : P ( T _ { 1 } ; T _ { 1 } )$ and such a credit is acquired X-times. See 1.3.3 on the notation $P ( T _ { 1 } ; T _ { 0 } )$ ). 

this condition that prevents the replication of product A: We can not buy or sell the random variable “rain”.<sup>3</sup> 

Consider again the equation 

$$
\frac {B (T _ {0})}{P (T _ {1} ; T _ {0})} = \mathrm{E} ^ {\mathbb {P}} \left(\frac {B (T _ {1})}{P (T _ {1} ; T _ {1})}\right).
$$

This equation would reduce the pricing (i.e. the calculation of $B ( T _ { 0 } ) )$ to the calculation of an expectation. The equation holds, if 

$$
\frac {S (T _ {0})}{P (T _ {1} ; T _ {0})} = \mathrm{E} ^ {\mathbb {P}} \left(\frac {S (T _ {1})}{P (T _ {1} ; T _ {1})}\right).
$$

Obvisously this equation cannot hold in general (or only the expectation of $S ( T _ { 1 } )$ would enter into the pricing and we would be ignorant of any risk). However, it is possible to change the measure such that the corresponding equation holds, i.e. there is a measure Q such that 

$$
\frac {S \left(T _ {0}\right)}{P \left(T _ {1} ; T _ {0}\right)} = \mathrm{E} ^ {\mathbb {Q}} \left(\frac {S \left(T _ {1}\right)}{P \left(T _ {1} ; T _ {1}\right)}\right).
$$

A change of measure is indeed an admissible tool when considering replication portfolios, since - as we have seen - the real probabilities (the measure P) do not enter into the calculation. To motivate this important concept let us consider the following (simple) example: 

## 3.1.2. Replication in a discrete Mode

## 3.1.2.1. Example: two times $( T _ { 0 } , T _ { 1 } )$ , two states $( \omega _ { 1 } , \omega _ { 2 } )$ , two assets $( S , N )$

Let S and N denote stochastic processes defined over a filtered probability space $( \Omega , { \mathcal { F } } , P , { \mathcal { F } } _ { t } )$ with $\Omega \ = \ \{ \omega _ { 1 } , \omega _ { 2 } \}$ . Here $S ( t , \omega )$ denotes the value of a financial product $\mathbf { \vec { \Delta } } ^ { 6 } \mathbf { S } ^ { \prime }$ and N(t <sub>ω</sub>) denote the value of a financial product $\mathbf { \bar { \Psi } } ^ { 6 6 } \mathbf { N } ^ { \prime }$ . We consider two points in time $T _ { 0 }$ (present) and $T _ { 1 }$ (future). We assume that $\mathbf { \Delta ^ { 6 6 } S } ^ { \prime }$ and $\mathbf { \bar { \Psi } } ^ { 6 6 } \mathbf { N } ^ { \prime }$ are traded at these times. Let the filtration be given by $F _ { T _ { 0 } } = \{ 0 , \Omega \}$ and $F _ { T _ { 1 } } = \{ 0 , \{ \omega _ { 1 } \} , \{ \omega _ { 2 } \} , \Omega \}$ , i.e. in $T _ { 0 }$ it is not possible to decide which of the states <sub>ω1</sub>, <sub>ω2</sub> we are in, but in $T _ { 1 }$ this information is known. Assume that the processes S and N are {F<sub>t</sub>}-adapted, i.e. in $T _ { 0 }$ we have $S ( T _ { 0 } , \omega _ { 1 } ) = S ( T _ { 0 } , \omega _ { 2 } )$ and $N ( T _ { 0 } , \omega _ { 1 } ) = N ( T _ { 0 } , \omega _ { 2 } )$ . So, independent of the (unknown) state, the products have a defined value in $T _ { 0 }$ 

Given a derivative product (with the stochastic value process V) depending in $T _ { 1 }$ on the attained state $\omega _ { i }$ . We seek to determine the value of V in $T _ { 0 } .$ . Our setup is illustrated in Figure 3.2. 

To have the derivative product V replicated by a portfolio we seek $\alpha , \beta$ such that 

$$
\begin{array}{l} V (T _ {1}, \omega_ {1}) = \alpha S (T _ {1}, \omega_ {1}) + \beta N (T _ {1}, \omega_ {1}), \\ V (T _ {1}, \omega_ {2}) = \alpha S (T _ {1}, \omega_ {2}) + \beta N (T _ {1}, \omega_ {2}). \end{array}\tag{3.2}
$$

This system of equations has a solution $( \alpha , \beta )$ , if 

$$
S (T _ {1}, \omega_ {1}) N (T _ {1}, \omega_ {2}) \neq S (T _ {1}, \omega_ {2}) N (T _ {1}, \omega_ {1}).\tag{3.3}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/0a15790e91059fb275f97cbaa27300ff0ae840b2385e10adbad3daa1053155c2.jpg)



Figure 3.2.: Replication: The two-times-two-states-two-assets example


With this solution the value of the replication portfolio (and thus the cost of replication) is known in $T _ { 0 } .$ , and thus the “fair” value of the derivative product $\mathbf { \Delta ^ { 6 6 } V } ^ { 5 }$ in $T _ { 0 }$ as 

$$
V (T _ {0}) = \alpha S (T _ {0}) + \beta N (T _ {0}).\tag{3.4}
$$

As before, the probabilities $P ( \{ \omega _ { 1 } \} ) , P ( \{ \omega _ { 2 } \} )$ do not enter into the calculation of the cost of replication and thus $V ( T _ { 0 } )$ . Let us investigate now whether $V ( T _ { 0 } )$ may be expressed in terms of an expectation. Assume that $N \neq 0$ and consider (3.2), (3.3), (3.4) for N-relative prices. Equivalent to (3.2), (3.3), (3.4) the portfolio satisfies in $T _ { 1 }$ 

$$
\frac {V \left(T _ {1} , \omega_ {1}\right)}{N \left(T _ {1} , \omega_ {1}\right)} = \alpha \frac {S \left(T _ {1} , \omega_ {1}\right)}{N \left(T _ {1} , \omega_ {1}\right)} + \beta \quad \frac {V \left(T _ {1} , \omega_ {2}\right)}{N \left(T _ {1} , \omega_ {2}\right)} = \alpha \frac {S \left(T _ {1} , \omega_ {2}\right)}{N \left(T _ {1} , \omega_ {2}\right)} + \beta\tag{3.5}
$$

with the solvability condition being 

$$
\frac {S (T _ {1} , \omega_ {1})}{N (T _ {1} , \omega_ {1})} \neq \frac {S (T _ {1} , \omega_ {2})}{N (T _ {1} , \omega_ {2})}\tag{3.6}
$$

and in $T _ { 0 }$ we have 

$$
\frac {V (T _ {0})}{N (T _ {0})} = \alpha \frac {S (T _ {0})}{N (T _ {0})} + \beta .\tag{3.7}
$$

Obviously we have 

$$
\frac {V (T _ {0})}{N (T _ {0})} = \mathrm{E} \left(\frac {V (T _ {1})}{N (T _ {1})} \mid \mathcal {F} _ {T _ {0}}\right) \quad \Leftrightarrow \quad \frac {S (T _ {0})}{N (T _ {0})} = \mathrm{E} \left(\frac {S (T _ {1})}{N (T _ {1})} \mid \mathcal {F} _ {T _ {0}}\right).
$$

Now let $q \in \mathbb { R }$ such that 

$$
\frac {S (T _ {0})}{N (T _ {0})} = q \cdot \frac {S (T _ {1} , \omega_ {1})}{N (T _ {1} , \omega_ {1})} + (1 - q) \cdot \frac {S (T _ {1} , \omega_ {2})}{N (T _ {1} , \omega_ {2})},
$$

i.e. 

$$
q = \frac {\frac {S (T _ {0})}{N (T _ {0})} - \frac {S (T _ {1} , \omega_ {2})}{N (T _ {1} , \omega_ {2})}}{\frac {S (T _ {1} , \omega_ {1})}{N (T _ {1} , \omega_ {1})} - \frac {S (T _ {1} , \omega_ {2})}{N (T _ {1} , \omega_ {2})}}
$$

(c.f. (3.6)). If in addition to (3.6), we have 

$$
0 \leq q \leq 1,\tag{3.8}
$$

then $\mathbb { Q } ^ { N } ( \{ \omega _ { 1 } \} ) : = q , \mathbb { Q } ^ { N } ( \{ \omega _ { 2 } \} ) : = 1 - q$ defines a probability measure and under $\mathbb { Q } ^ { N }$ we have 

$$
\frac {S (T _ {0})}{N (T _ {0})} = \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {S (T _ {1})}{N (T _ {1})} | \mathcal {F} _ {T _ {0}}) \quad \text { d.h } \quad \frac {V (T _ {0})}{N (T _ {0})} = \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {V (T _ {1})}{N (T _ {1})} | \mathcal {F} _ {T _ {0}}).\tag{3.9}
$$

So instead of calculating the parameters $( \alpha , \beta )$ for the replication portfolio we may alternatively calculate the measure $\mathbb { Q } ^ { N }$ , i.e. the parameter q. At first it appears to be equally complex to calculate $\mathbb { Q } ^ { N }$ as it is to calculate the replication strategy. However, determining $\mathbb { Q } ^ { \dot { N } }$ has a striking advantage: The calculation of $\bar { \mathbb { Q } ^ { N } }$ is independent of the derivative V, but the pricing formula (3.9) is valid for all derivatives $V .$ If $\mathbb { Q } ^ { N }$ has been determined once, all derivatives $V$ may be priced as a $\mathbb { Q } ^ { N }$ -expectation. 

In Equations (3.5) to (3.9) we have considered N-relative prices, i.e. the value of any product $V$ was expressed in fractions of $N ,$ i.e. by ${ \frac { V } { N } } .$ As long as $S ~ \ne ~ 0$ , we may repeat these considerations with S -relative prices, i.e. we have 

$$
\frac {V (T _ {1} , \omega_ {1})}{S (T _ {1} , \omega_ {1})} = \alpha + \beta \frac {N (T _ {1} , \omega_ {1})}{S (T _ {1} , \omega_ {1})} \quad \frac {V (T _ {1} , \omega_ {2})}{S (T _ {1} , \omega_ {2})} = \alpha + \beta \frac {N (T _ {1} , \omega_ {2})}{S (T _ {1} , \omega_ {2})}\tag{3.10}
$$

with the same $( \alpha , \beta )$ and we obtain the same value for the replication portfolio $V ( T _ { 0 } )$ , namely 

$$
\frac {V (T _ {0})}{S (T _ {0})} = \alpha + \beta \frac {N (T _ {0})}{S (T _ {0})}.\tag{3.11}
$$

If we determine the measure $\mathbb { Q } ^ { S }$ , such that 

$$
\frac {N (T _ {0})}{S (T _ {0})} = \mathrm{E} ^ {\mathbb {Q} ^ {s}} (\frac {N (T _ {1})}{S (T _ {1})} | \mathcal {F} _ {T _ {0}}) \quad \text { d.h } \quad \frac {V (T _ {0})}{S (T _ {0})} = \mathrm{E} ^ {\mathbb {Q} ^ {s}} (\frac {V (T _ {1})}{S (T _ {1})} | \mathcal {F} _ {T _ {0}}),\tag{3.12}
$$

then the measure $\mathbb { Q } ^ { S }$ is diferent from $\mathbb { Q } ^ { N }$ - we have for example 

$$
\mathbb {Q} ^ {S} \left(\{\omega_ {1} \}\right) = \frac {\frac {N (T _ {0})}{S (T _ {0})} - \frac {N (T _ {1} , \omega_ {2})}{S (T _ {1} , \omega_ {2})}}{\frac {N (T _ {1} , \omega_ {1})}{S (T _ {1} , \omega_ {1})} - \frac {N (T _ {1} , \omega_ {2})}{S (T _ {1} , \omega_ {2})}}.
$$

However, the measure $\mathbb { Q } ^ { S }$ also allows us to calculate the value of all derivatives V as a $\mathbb { Q } ^ { S } .$ expectation via (3.12). 

We conclude this section with some remarks: 

• Under the measure $\mathbb { Q } ^ { N }$ the relative price $\frac { S } { N }$ is a martingale: This is the defining property for the measure $\mathbb { Q } ^ { N }$ 

• Under the measure $\mathbb { Q } ^ { N }$ the relative price $\frac { V } { N }$ of any replication portfolio V is a martingale:<sup>4</sup> This allows the calculation of the price of V as $\mathbb { Q } ^ { N }$ -expectation of N-relative payout. 

• The choice of the product that functions as reference (numeraire) is arbitrary (as long as´ it is non-zero). The measure $\mathbb { Q } ,$ under which any numeraire-relative replication portfolio´ becomes a martingale, depends on the chosen numeraire. This makes it possible to´ change the numeraire-measure-pair´ $( N , \mathbb { Q } ^ { N } )$ , e.g. if this simplifies the calculation of the expectation. 

• It is necessary to consider relative prices, such that 

<sup>4</sup> This follows since the replication portfolio is a linear combination of martingales and the expectation is linear. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/2e88c09bcff0097040ed3f75b4d3deeaa464ff68e20e4ecc98b63c9ad93900f1.jpg)



Figure 3.3.: Replication: Generalization to multiple states


$\mathbb { Q } ^ { N }$ is independent of V, 

$\mathbb { Q } ^ { N }$ is a probability measure, i.e. $\mathbb { Q } ^ { N } ( \Omega ) = 1$ 

## Exercise: Change of Measure

1. Reconsider the above under the numeraire´ S , calculate $\mathbb { Q } ^ { S }$ and show (e.g. for an example) that $\mathbb { Q } ^ { N } \neq \mathbb { Q } ^ { S }$ 

2. Instead of relative prices consider absolute prices, i.e. choose as numeraire 1 and deter-´ mine the measure $\mathbb { Q } ^ { 1 }$ for which 

$$
V (T _ {0}) = \mathrm{E} ^ {\mathbb {Q} ^ {1}} \bigl (V (T _ {1}) | \mathcal {F} _ {T _ {0}} \bigr).
$$

Show that $\mathbb { Q } ^ { 1 }$ depends on the specific $V ( T _ { 1 } )$ and is thus not universal for all replication portfolios. 

In case we wish to replicate a payof X(T), which depends on multiple states $\omega _ { 1 } , \ldots , \omega _ { n } .$ then the above may be extended either by considering multiple time steps $T _ { 0 } , T _ { 1 } , . . . , T _ { n - 1 } = T$ (dynamic replication) or multiple assets $N , S _ { 1 } , \ldots , S _ { n - 1 }$ - see Figure 3.3. 

## 3.2. Foundations: Equivalent Martingale Measure

## 3.2.1. Challenge and Solution Outline

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/6a85ccdcfbf187cd95cdb35b5da67871b5757dc72e9530f1a5d83b99b9a6d5b9.jpg)


Motivation: According to the previous example, the evaluation of a product through the value of a corresponding replication strategy may be given as the $\mathbb { Q } ^ { N } .$ expectation of the N-relative price (where N denotes the chosen reference asset - the num´eraire). 

How can we determine the measure $\mathbb { Q } ^ { N } ;$ , given that we know the price processes under the real measure P? Note that under the measure $\mathbb { Q } ^ { N }$ , the N-relative prices are martingales, i.e. as Ito-processes they are drift-free (Lemma ˆ 52) - this is the defining property of $\mathbb { Q } ^ { \breve { N } } \textrm { - }$ , and a change of measure $\dot { \mathbb { P } } \to \mathbb { Q } ^ { N }$ implies a change of drift for Ito processes (Theoremˆ 58). 

Thus, if we know the price processes under the real measure P (i.e. given a “model”), first we can derive the N-relative price processes under the real measure P by using the quotient rule. Then we can derive the equivalent martingale measure $\mathbb { Q } ^ { N }$ from the change of drift by using Girsanov’s theorem (Theorem 58) (see Figure3.4). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/037f90bebf1194b8186c13479a918ed8a0e72f517c97bfa4d3d19ccfbf3178a2.jpg)



Figure 3.4.: Real Measure versus Martingale Measure.


Surprisingly, in our applications we never need to calculate the equivalent martingale measure: Since we know the processes under $\mathbb { Q } ^ { N }$ (we know their drift under $\mathbb { Q } ^ { N }$ and only the drift changes under a change of measure), we know the conditional probability densities under $\mathbb { Q } ^ { N }$ and these are enough to calculate expectations (see Definition 10). 

What remains is to clarify under which conditions a given payof function may be replicated and under which conditions an equivalent martingale measure exists. In this chapter we give a short overview of the corresponding mathematical foundations. In our later applications we will not discuss the existence of the equivalent martingale measure. C| 

## Problem description:

Given: $M = \{ X _ { 1 } , \ldots , X _ { n } \}$ , where $X _ { i }$ denotes price processes under the (real) measure $\mathbb { P } ,$ and a contingent claim (payof profile) $V ^ { ( T ) }$ , where $V ^ { ( T ) }$ is $\mathrm { a } \mathcal { F } _ { T }$ measurable random variable. Wanted: Price indication, i.e. the value $V ( t )$ of $V ^ { ( T ) }$ at time $t < T$ , especially $V ( 0 )$ , where V is a $\{ \mathcal { F } _ { t } \}$ -adapted stochastic process. 

## Solution (sketched):

• Choice of num´eraire: Let $N \in { \mathcal { M } }$ denote a price process that may function as reference asset (num´eraire). Without loss of generality let $N = X _ { 1 }$ 

• Existence of a martingale measure for N-relative prices: By Theorem 74 there exists a measure $\mathbb { Q } ^ { \dot { N } }$ , such that $\frac { X _ { i } } { N }$ is a martingale with respect to $\mathcal { F } _ { t } , \forall \ : i = 1 , \ldots , n$ 

• Definition ofthe (candidate) ofa value process ofthe replication portfolio: Define 

$$
V (t) := N (t) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {V ^ {(T)}}{N (T)} | \mathcal {F} _ {t}\right).
$$

Then $\frac { V ( t ) } { N ( t ) }$ is a $\mathbb { Q } ^ { N }$ -martingale with respect to $\mathcal { F } _ { t }$ (tower law). 

• Martingale representation theorem gives trading strategy: Since the processes $\begin{array} { l l } { { { \frac { X } { N } } } } & { { = } } \end{array}$ $\big ( \frac { X _ { 1 } } { N } , \dots , \frac { X _ { n } } { N } \big )$ and $\frac { V } { N }$ are martingale under $\mathbb { Q } ^ { N }$ , there exists a $\phi = ( \phi _ { 1 } , \ldots , \phi _ { n } )$ such that 

$$
\frac {V (t)}{N (t)} = \frac {V (0)}{N (0)} + \int_ {0} ^ {t} \phi (s) \cdot \mathrm{d} \left(\frac {X (s)}{N (s)}\right)\tag{3.13}
$$

(Martingale Representation Theorem). 

• The portfolio process φ may be chosen to be self-financing by setting 

$$
\phi_ {1} (t) := \frac {V (0)}{N (0)} + \sum_ {i = 2} ^ {n} \int_ {0} ^ {t} \phi_ {i} (s) \mathrm{d} \left(\frac {X _ {i} (s)}{N (s)}\right) - \sum_ {i = 2} ^ {n} \phi_ {i} (t) \frac {X _ {i} (t)}{N (t)}.
$$

Note: $\begin{array} { r } { \mathrm { d } \left( \frac { X _ { 1 } } { N } \right) = \mathrm { d } \left( \frac { N } { N } \right) = 0 . } \end{array}$ , i.e. (3.13) holds unchanged. 

• The portfolio process φ describes a replication portfoliofor $V ^ { ( T ) }$ : We have 

$$
V ^ {(T)} = \sum_ {i = 1} ^ {n} \phi_ {i} (T) X _ {i} (T) = \sum_ {i = 1} ^ {n} \phi_ {i} (0) X _ {i} (0) + \int_ {0} ^ {T} \phi (s) \cdot \mathrm{d} X (s).
$$

• The evaluation does not require to explicit determination of the replication portfolio: V(t) is the value of the replication portfolio at time t and we have 

$$
\frac {V (t)}{N (t)} = \mathrm{E} ^ {\mathbb {Q} ^ {N}} \big (\frac {V ^ {(T)}}{N (T)} | \mathcal {F} _ {t} \big).\tag{3.14}
$$

## 3.2.2. Steps towards the Universal Pricing Theorem

We will now list the central building blocks of risk-neutral pricing, towards the Universal Pricing Theorem (3.14): 

• Trading Strategies and characterization of self-financing of a trading strategy - in the following in Number 66-72. 

• Equivalent Martingale Measure, to obtain a trading strategy from the martingale representation theorem, as a candidate for the replication strategy - in the following in Number 73-74. 

• Replication of given payoffunctions and Universal Pricing Theorem followed by definition of a martingale process $t \mapsto \mathrm { E } ^ { \bigotimes ^ { N } } ( { } _ { N ( T ) } ^ { V ^ { ( T ) } } \mid { \mathcal { F } } _ { t } )$ for the given payof function $V ^ { T } \mathrm { ~ \scriptsize ~ - ~ i n ~ }$ the following in Number 76-79. 

This program is found in this order in most of the literature, some being less technical ([3]), some being more technical ([6, 27]). We will usually sketch the theory without technical proofs, but include references to the literature. 

## Basic Assumptions (Part 1 of 3)

Let $M = \{ X _ { 1 } , \ldots , X _ { n } \}$ denote a family of (Ito) stochastic processes, defined over the filteredˆ probability space $( \Omega , { \mathcal { F } } , { \mathbb { P } } , \{ { \mathcal { F } } _ { t } \} )$ 

$$
\mathrm{d} X _ {i} = \mu_ {i} ^ {\mathbb {P}} \mathrm{d} t + \sum_ {j = 1} ^ {m} \sigma_ {i, j} \mathrm{d} W _ {j},
$$

where $\{ \mathcal { F } _ { t } \}$ is the (augmentation of the) filtration generated by the (independent) Brownian motions $W _ { j }$ and the coeficients $\mu ^ { \mathbb { P } }$ and <sub>σ</sub> fulfill the integrability conditions 

$$
\int_ {0} ^ {T} \left| \mu_ {i} ^ {\mathbb {P}} (s) \right| d s <   \infty \quad \int_ {0} ^ {T} \sum_ {j = 1} ^ {m} \left| \sigma_ {i, j} (s) \right| ^ {2} d s <   \infty \quad \mathbb {P} - \text { almost   surely }.
$$

The elements of M are price processes of traded assets (M represents the market). We consider these only upto a finite time horizon T and thus assume furthermore $\mathcal { F } = \mathcal { F } _ { T }$ 

## 3.2.2.1. Self-financing Trading Strategy

Definition 66 (Portfolio, Trading Strategy, Self-financing): 

1. An n-dimensional $\{ \mathcal { F } _ { t } \}$ -progressively measurable process $\phi = ( \phi _ { 1 } , \ldots , \phi _ { n } )$ with 

$$
\int_ {0} ^ {T} | \phi_ {i} \mu_ {i} ^ {\mathbb {P}} (s) | \mathrm{d} s <   \infty \quad \int_ {0} ^ {T} \sum_ {j = 1} ^ {m} | \phi_ {i} \sigma_ {i, j} (s) | ^ {2} \mathrm{d} s <   \infty \quad \mathbb {P} \text {-almost surely.}
$$

is called portfolio process or trading strategy. 

2. The value ofthe portfolio φ at time t is given by the scalar product 

$$
V _ {\phi} (t) := \phi (t) \cdot X (t) = \sum_ {i = 1} ^ {n} \phi_ {i} (t) X _ {i} (t).
$$

The process $V _ { \phi }$ is called wealth process of the portfolio φ. 

3. The gain process of the portfolio φ is defined by 

$$
G _ {\phi} (t) := \int_ {0} ^ {t} \phi (\tau) \cdot \mathrm{d} X (\tau) = \sum_ {i = 1} ^ {n} \int_ {0} ^ {t} \phi_ {i} (\tau) \cdot \mathrm{d} X _ {i} (\tau).
$$

4. The portfolio process φ is called self-financing, if 

$$
V _ {\phi} (t) = V _ {\phi} (0) + G _ {\phi} (t) \forall t \in [ 0, T ] \quad \mathbb {P} \text {-almost surely},\tag{3.15}
$$

i.e. 

$$
\mathrm{d} V _ {\phi} = \phi \cdot \mathrm{d} X.\tag{3.16}
$$

Remark 67: The integrability condition in Definition 66.1 ensures that the Ito integralˆ $\int _ { 0 } ^ { t } \phi ( s )$ dX(s) exists. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/c382d41ade5f7b42a4b3c56b993b0e8f1aabef00a9475498e53b40f32211c1f9.jpg)


Interpretation: We interpret $\{ X _ { i } \mid i = 1 , \ldots , n \mid$ } as a family of stock price processes and ${ \boldsymbol { \phi } } ( t ) : = ( \phi _ { 1 } ( t ) , \ldots , \phi _ { n } ( t ) )$ as a stock portfolio, i.e. $\phi _ { i }$ denotes the number of stocks X in the portfolio. 

」 The relation (3.16) may be interpreted as following: A change in the portfolio value $V _ { \phi }$ comes only from changes in the stocks X, as if the portfolio remained unchanged, i.e. we hold a portfolio of φ stocks and gain over dt the amount φ · dX. On the other hand, if $\phi$ is an Ito-process we have from theˆ product rule 

$$
\mathrm{d} V _ {\phi} = \mathrm{d} (\phi \cdot X) = X \cdot \mathrm{d} \phi + \phi \cdot \mathrm{d} X + \mathrm{d} \phi \cdot \mathrm{d} X = \phi \cdot \mathrm{d} X + \mathrm{d} \phi \cdot (X + \mathrm{d} X)
$$

and thus we find from (3.16) the equivalent characterization of self-financing 

$$
\mathrm{d} \phi \cdot (X + \mathrm{d} X) = 0
$$

and with $\mathrm { d } \phi \cdot \mathrm { d } X = 0$ thus 

$$
\mathrm{d} \phi \cdot X = 0.\tag{3.17}
$$

In other words, the portfolio may change, but such a change must not change the value. The portfolio change does not produce any cost: it finances itself. 

The interpretation of condition (3.17) becomes clear if we consider the time-discrete variant of a self-financing strategy: 

• At time $T _ { i }$ there exists a $\phi ( T _ { i } )$ of the products $X ( T _ { i } )$ . Its value is $V _ { \phi } ( T _ { i } ) = \phi ( T _ { i } ) \cdot X ( T _ { i } )$ 

• At time $T _ { i }$ the products X are traded at prices $X ( T _ { i } )$ and the portfolio is rearranged in a self-financing manner. The portfolio changes by $\Delta \phi ( T _ { i + 1 } ) = \phi ( T _ { i + 1 } ) - \phi ( T _ { i } )$ . This change does not imply a change in value: $\Delta \phi ( T _ { i + 1 } ) \cdot X ( T _ { i } ) = 0$ . This corresponds to the continuous case: 

$$
\mathrm{d} \phi \cdot X = 0.
$$

• Over the interval $\Delta T _ { i } : = T _ { i + 1 } - T _ { i }$ the value of the products X changes by $\Delta X ( T _ { i } ) : =$ $X ( T _ { i + 1 } ) - X ( T _ { i } )$ . The value of the portfolio thus changes by $\phi ( T _ { i + 1 } ) \cdot \Delta X ( T _ { i } )$ , i.e. 

$$
\Delta V _ {\phi} (T _ {i}) = \phi (T _ {i + 1}) X (T _ {i + 1}) - \phi (T _ {i}) X (T _ {i})
$$

$$
= \phi (T _ {i + 1}) \Delta X (T _ {i}) + \underbrace {\Delta \phi (T _ {i}) X (T _ {i})} _ {= 0}.
$$

This corresponds to the continuous case: 

$$
\mathrm{d} V _ {\phi} = \phi \cdot \mathrm{d} X.
$$

Note that this interpretation is consistent with the definition of the elementary Ito inte-ˆ gral, see also Remark 37. 

• The first step of the rearrangement of the portfolio is done (conditionally) independent of future changes in the product prices. The portfolio cannot anticipate future changes of the product prices. This information does not exist at the time of the portfolio rearrangement; we have considered the two time-discrete changes $\Delta \phi ( T _ { i } )$ and $\Delta X ( T _ { i } )$ as being consecutive. This independence corresponds to the continuous case: 

$$
\mathrm{d} \phi \cdot \mathrm{d} X = 0.
$$

• (repeat) 

Remark: We will discuss this time-discrete variant of a trading strategy (which does not result in a complete replication) in Chapter 7. C| 

## 3.2.2.2. Relative Prices

## Definition 68 (Numeraire):´

A price-process $N \in { \mathcal { M } }$ is called num´eraire (on [0 T]), if 

$$
\mathbb {P} (\{N (t) > 0 \mid \forall t \leq T \}) = 1.
$$

## Basic Assumptions (Part 2 of 3)

For the remainder of this chapter we assume that $X _ { 1 }$ is a numeraire and we will use the symbol´ $N : = X _ { 1 }$ . Furthermore we require that the chosen numeraire is such that the integrability´ condition formulated in Definition 66 is equivalent to the corresponding integrability condition under the normalized system of the relative price processes $\begin{array} { r } { \tilde { X } = ( \frac { X _ { 2 } } { N } , \ldots , \frac { X _ { n } } { N } ) } \end{array}$ , i.e. with 

$$
\mathrm{d} \tilde {X} = \tilde {\mu} \mathrm{d} t + \tilde {\sigma} \mathrm{d} W
$$

we require that for all $\{ \mathcal { F } _ { t } \}$ }-progressively measurable $\tilde { \boldsymbol { \phi } } = ( \phi _ { 2 } , \ldots , \phi _ { n } ) , \boldsymbol { \phi } = ( 0 , \phi _ { 2 } , \ldots , \phi _ { n } )$ 

$$
\begin{array}{l l} & \int_ {0} ^ {T} | \phi (s) \cdot \mu (s) | + \| \phi (s) \cdot \sigma (s) \| _ {2} ^ {2}   \mathrm{d} s <   \infty \\ \Leftrightarrow & \int_ {0} ^ {T} | \tilde {\phi} (s) \cdot \tilde {\mu} (s) | + \| \tilde {\phi} (s) \cdot \tilde {\sigma} (s) \| _ {2} ^ {2}   \mathrm{d} s <   \infty \end{array} \qquad \begin{array}{l l} & \mathbb {P} \text {-almost surely}, \\ & \mathbb {P} \text {-almost surely}. \end{array}
$$

Remark 69 (Assumptions on the Numeraire):´ We pose an additional assumption on the numeraire, namely that it is such that the known integrability condition can be equivalently´ formulated with respect to the normalized system $\frac { X } { N }$ , i.e. the relative price processes. In many cases this follows from a more specific choice for the numeraire, e.g. for a locally riskless´ numeraire´ ${ \mathrm { d } } N = r ( t ) N ( t )$ dt or for $\begin{array} { r } { \mathrm { d } N = r ( t ) N ( t ) \mathrm { d } t + \sum _ { i = 1 } ^ { m } \sigma _ { 1 , j } ( t ) N ( t ) \mathrm { d } W _ { j } } \end{array}$ with bounded $\sigma _ { 1 , j } .$ Thus, in many works the requirement on the normalized system does not appear in this form since it is implied by the specific choice of the numeraires.´ 

Lemma 70 (Condition of self-financing is invariant under a move to relative prices): Let $\boldsymbol { \phi } = ( \phi _ { 1 } , \ldots , \phi _ { n } )$ denote a portfolio. Then we have 

$$
\mathrm{d} V _ {\phi} = \sum_ {i = 1} ^ {n} \phi_ {i} \mathrm{d} X _ {i} \Leftrightarrow \mathrm{d} \frac {V _ {\phi}}{N} = \sum_ {i = 1} ^ {n} \phi_ {i} \mathrm{d} \frac {X _ {i}}{N}.
$$

In other words, $\phi$ is self-financing if and only if 

$$
\mathrm{d} \frac {V _ {\phi}}{N} = \sum_ {i = 1} ^ {n} \phi_ {i} \mathrm{d} \frac {X _ {i}}{N}.
$$

Proof: Let 

$$
\mathrm{d} V _ {\phi} = \sum_ {i = 1} ^ {n} \phi_ {i} \mathrm{d} X _ {i}.\tag{3.18}
$$

Then we find from $\mathrm { d } X _ { i } \cdot ( \frac { 1 } { N } + \mathrm { d } ( \frac { 1 } { N } ) ) + X _ { i } \cdot \mathrm { d } ( \frac { 1 } { N } ) = \mathrm { d } \frac { X _ { i } } { N }$ 

$$
\begin{array}{r c l} \mathrm{d} \frac {V _ {\phi}}{N} & = & \mathrm{d} V _ {\phi} \cdot (\frac {1}{N} + \mathrm{d} (\frac {1}{N})) + V _ {\phi} \cdot \mathrm{d} (\frac {1}{N}) \\ & \stackrel {(3. 1 8)} {=} & \sum_ {i = 1} ^ {n} \phi_ {i} \mathrm{d} X _ {i} \cdot (\frac {1}{N} + \mathrm{d} (\frac {1}{N})) + \sum_ {i = 1} ^ {n} \phi_ {i} X _ {i} \cdot \mathrm{d} (\frac {1}{N}) \\ & = & \sum_ {i = 1} ^ {n} \phi_ {i} \mathrm{d} \frac {X _ {i}}{N} = \sum_ {i = 2} ^ {n} \phi_ {i} \mathrm{d} \frac {X _ {i}}{N}. \end{array}
$$

Conversely we have from 

$$
\mathrm{d} \frac {V _ {\phi}}{N} = \sum_ {i = 1} ^ {n} \phi_ {i} \mathrm{d} \frac {X _ {i}}{N}\tag{3.19}
$$

with $\begin{array} { r } { { 1 } \frac { X _ { i } } { N } \cdot ( N + \mathrm { d } N ) + \frac { X _ { i } } { N } \cdot \mathrm { d } N = \mathrm { d } X _ { i } } \end{array}$ , that 

$$
\begin{array}{r c l} \mathrm{d} V _ {\phi} & = & \mathrm{d} (\frac {V _ {\phi}}{N} \cdot N) = \mathrm{d} \frac {V _ {\phi}}{N} \cdot (N + \mathrm{d} N) + \frac {V _ {\phi}}{N} \cdot \mathrm{d} N \\ & \stackrel {(3. 1 9)} {=} & \sum_ {i = 1} ^ {n} \phi_ {i} \mathrm{d} \frac {X _ {i}}{N} \cdot (N + \mathrm{d} N) + \sum_ {i = 1} ^ {n} \phi_ {i} \frac {X _ {i}}{N} \cdot \mathrm{d} N \\ & = & \sum_ {i = 1} ^ {n} \phi_ {i} \mathrm{d} X _ {i}. \end{array}
$$

Remark 71: Note that due to the choice of the numeraire,´ $\phi _ { 1 }$ does not enter into the sum over $\mathrm { d } { \frac { X _ { i } } { N } }$ . We will use this in the following Lemma to construct a self-financing replication portfolio. 

The move to relative prices makes it possible to construct a self-financing portfolio from a partial portfolio $\phi _ { 2 } , \ldots , \phi _ { n }$ which fulfills for a given process V the relation 

$$
\mathrm{d} \frac {V}{N} = \sum_ {i = 2} ^ {n} \phi_ {i} \mathrm{d} \frac {X _ {i}}{N}.\tag{3.20}
$$

Note that in (3.20) V stands for an arbitrary process, not limited to $V _ { \phi }$ (the value process of the portfolio). This process becomes the value process of a self-financing portfolio by the following choice of $\phi _ { 1 }$ (replication): 

Lemma 72 (Self-financing strategy for given partial portfolio and given initial value): Let $\tilde { \boldsymbol { \phi } } = ( \phi _ { 2 } , \ldots , \phi _ { n } )$ be {F}-progressivly measurable and such that 

$$
\int_ {0} ^ {t} | \tilde {\phi} (s) \tilde {\mu} (s) | + \| \tilde {\phi} (s) \cdot \tilde {\sigma} (s) \| _ {2} ^ {2} d s <   \infty \quad \mathbb {P} - a l m o s t \text {   surely. }
$$

Then we have that $\boldsymbol { \phi } = ( \phi _ { 1 } , \ldots , \phi _ { n } )$ where 

$$
\phi_ {1} (t) := \frac {V _ {0}}{N (0)} + \sum_ {i = 2} ^ {n} \int_ {0} ^ {t} \phi_ {i} (s) \mathrm{d} \left(\frac {X _ {i} (s)}{N (s)}\right) - \sum_ {i = 2} ^ {n} \phi_ {i} (t) \frac {X _ {i} (t)}{N (t)}\tag{3.21}
$$

defines a self-financing strategy with $V _ { \phi } ( 0 ) = V _ { 0 }$ 

Proof: To show that $\phi$ is self-financing it is suficient to show that (Lemma 70) 

$$
\mathrm{d} \frac {V _ {\phi}}{N} = \sum_ {i = 1} ^ {n} \phi_ {i} \mathrm{d} \frac {X _ {i}}{N}.\tag{3.22}
$$

From equation (3.21) it follows (note that $\begin{array} { r } { \frac { X _ { 1 } } { N } = 1 } \end{array}$ and d $\begin{array} { r } { \cdot { \frac { X _ { 1 } } { N } } = 0 ) } \end{array}$ that 

$$
\sum_ {i = 1} ^ {n} \phi_ {i} (t) \frac {X _ {i} (t)}{N (t)} = \frac {V _ {0}}{N (0)} + \sum_ {i = 1} ^ {n} \int_ {0} ^ {t} \phi_ {i} (s) \mathrm{d} \left(\frac {X _ {i} (s)}{N (s)}\right)
$$

and thus (3.22). The initial condition $V _ { \phi } ( 0 ) = V _ { 0 }$ follows from setting $t = 0$ 

The relation (3.20) would follow from the martingale representation theorem, if the corresponding processes were martingales. It thus becomes natural to ask for a measure under which the relative prices $\frac { X _ { i } } { N }$ become martingales. 

## 3.2.2.3. Equivalent Martingale Measure

## Definition 73 (Equivalent Martingale Measure):

Let N denote a numeraire. A probability measure´ $\mathbb { Q } ^ { N }$ defined on $( \Omega , { \mathcal { F } } )$ is called equivalent martingale measure with respect to N (equivalent N-martingale measure) (on M), if 

1. $\mathbb { Q } ^ { N }$ and P are equivalent, and 

2. the N relative price processes $\begin{array} { r } { \frac { X _ { i } } { N } ( i = 1 , . . . , n ) } \end{array}$ are $\mathcal { F } _ { t }$ -martingales with respect to $\mathbb { Q } ^ { N }$ 

Theorem 74 (Equivalent Martingale Measure, Existence and Uniqueness): Let $\tilde { X } \ =$ $\big ( \frac { X _ { 2 } } { N } , \dots , \frac { X _ { n } } { N } \big )$ with 

$$
\mathrm{d} \tilde {X} = \tilde {\mu} \mathrm{d} t + \tilde {\sigma} \mathrm{d} W (t).
$$

Suppose that there exists a progressively measurable process $C : [ 0 , T ] \times \Omega  \mathbb { R } ^ { n - 1 }$ such that $\int _ { 0 } ^ { T } \| C ( s ) \| ^ { 2 } \mathrm { d } s <$ ∞ and 

$$
\tilde {\mu} = \tilde {\sigma} \cdot C \quad \lambda \times \mathbb {P} \text {-almost surely on} [ 0, T ] \times \Omega .
$$

Let $\begin{array} { r } { Z ( t ) : = \exp ( \int _ { 0 } ^ { t } C ( s ) \mathrm { d } W ( s ) - \frac { 1 } { 2 } \int _ { 0 } ^ { t } \| C ( s ) \| ^ { 2 } \mathrm { d } s . } \end{array}$ 

1. (Existence) $\mathrm { I f ~ E ^ { P } ~ } ( Z ( T ) ) = 1$ then the measure $\mathbb { Q } ^ { N }$ defined through 

$$
\left. \frac {\mathrm{d} \mathbb {Q} ^ {N}}{\mathrm{d} \mathbb {P}} \right| _ {\mathcal {F} _ {t}} = Z (t)\tag{3.23}
$$

is an equivalent martingale measure. 

2. (Uniqueness) If further the process C defined in (74) is unique, then $\mathbb { Q } ^ { N }$ is the unique equivalent martingale measure. 

Remark 75 (State Price Deflator): $\mathrm { I f ~ E ^ { \mathbb { P } } ~ } ( Z ( T ) ) < 1$ then (3.23) does not define a Radon-Nikodym process of a probability measure. Then it is not possible to define an equivalent´ martingale (probability) measure through (3.23). However, it is still possible to define an universal pricing theorem through 

$$
\frac {V (t)}{N (t)} = \mathrm{E} ^ {\mathbb {P}} \left(\frac {V ^ {(T)}}{N (T)} Z (T)   \Big |   \mathcal {F} _ {t}\right).
$$

The process $\frac { Z } { N }$ is called state price deflator. 

## 3.2.2.4. Payoff Replication

Given the existence of an equivalent martingale measure we can define a self-financing trading strategy replicating a given contingent claim $V ^ { T }$ 

## Definition 76 (Admissible trading strategy):

A self-financing trading strategy φ is called admissible, if 

$$
V _ {\phi} \geq - K
$$

for some finite $K .$ 

## Definition 77 (Attainable contingent claim, complete):

Let ${ T > 0 } . \mathrm { ~ A ~ } { \mathcal { F } _ { T } }$ -measurable random variable $V ^ { ( T ) }$ is called attainable contingent claim (or replicable payof), if there exists (at least one) admissible trading strategy $\phi$ such that 

$$
V _ {\phi} (T) = V ^ {(T)}.
$$

The market M is called complete if any contingent claim (payof function) is attainable (replicable). y 

## Basic Assumptions (Part 3 of 3)

Using the martingale representation theorem on $\begin{array} { r } { \mathbf { E } ^ { \mathbb { Q } ^ { N } } \big ( \frac { V ^ { ( T ) } } { N ( T ) } \big | \mathcal { F } _ { t } \big ) } \end{array}$  we find a representation $\tilde { \theta } \mathrm { d } W ^ { \mathbb { Q } ^ { N } }$ In order to find the replication portfolio $\tilde { \phi }$ such that θ<sup>˜</sup>d $\dot { { \cal W } } ^ { \mathbb { Q } ^ { N } } = \tilde { \phi } { \mathrm { d } } \tilde { X } = \tilde { \phi } \cdot \tilde { \sigma } { \mathrm { d } } W ^ { \mathbb { Q } ^ { N } }$ we need to solve $\widetilde { \phi } \cdot \widetilde { \sigma } = \widetilde { \theta }$ . We assume that for any $\tilde { \theta } , \int _ { 0 } ^ { T } \big | \big | \tilde { \theta } ( s ) \big | \big | _ { 2 } ^ { 2 } \mathrm { d } s <$ ∞ there exists a φ<sup>˜</sup>, $\int _ { 0 } ^ { T } \big | \big | \tilde { \theta } ( s ) \big | \big | _ { 2 } ^ { 2 } \mathrm { d } s \ <$ ∞ such that 

$$
\tilde {\phi} \cdot \tilde {\sigma} = \tilde {\theta}.
$$

What follows is 

Theorem 78 (self-financing replication portfolio of a given payof function): Let $\mathbb { Q } ^ { N }$ denote an equivalent martingale measure and $V ^ { ( T ) }$ a given payof function (contingent claim) with ${ \mathrm { E } } ^ { { \mathbb { Q } } ^ { N } } \left( \left| \frac { V ^ { ( T ) } } { N ( T ) } \right| ^ { 2 } \right) < \infty$ . Furthermore let 

$$
V (t) := N (t) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {V ^ {(T)}}{N (T)} \mid \mathcal {F} _ {t}\right).
$$

From that it follows that $\frac { V } { N }$ is a $\mathbb { Q } ^ { N }$ -Martingal. Furthermore let $\phi _ { 2 } , . . . , \phi _ { n }$ be as in the martingale representation theorem, i.e. 

$$
\mathrm{d} \frac {V}{N} = \sum_ {i = 2} ^ {n} \phi_ {i} \mathrm{d} \frac {X _ {i}}{N}.
$$

For the portfolio $\boldsymbol { \phi } = ( \phi _ { 1 } , \ldots , \phi _ { n } )$ let $\phi _ { 1 }$ be chosen as in Lemma 72 with $V _ { \phi } ( 0 ) : = V ( 0 )$ 

Then $\phi$ is a self-financing replication portfolio of V, i.e. we have 

$$
V (t) = V _ {\phi} = \sum_ {i = 1} ^ {n} \phi_ {i} X _ {i}.
$$

In other words: $V ^ { ( T ) }$ is an attainable contingent claim. 

Proof: That $\frac { V } { N }$ is a $\mathbb { Q } ^ { N }$ -martingale follows immediately from the definition and the tower $l a w ^ { 5 }$ . From the definition of the martingale measure, $\frac { X _ { i } } { N }$ are $\mathbb { Q } ^ { N }$ -martingales and the martingale representation theorem gives the existence of $\phi _ { 2 } , . . . , \phi _ { n }$ with 

$$
\mathrm{d} \frac {V}{N} = \sum_ {i = 2} ^ {n} \phi_ {i} \mathrm{d} \frac {X _ {i}}{N}.
$$

<sup>5</sup> See Exercise 2 on Page 369 

Choosing $\phi _ { 1 }$ as in Lemma $^ { 7 2 }$ will make φ self-financing. For the value process $V _ { \phi }$ we find from Lemma 70 that 

$$
\mathrm{d} \frac {V _ {\phi}}{N} = \sum_ {i = 2} ^ {n} \phi_ {i} \mathrm{d} \frac {X _ {i}}{N}
$$

and thus d $\begin{array} { r } { \mathrm { l } \frac { V _ { \phi } } { N } = \mathrm { d } \frac { V } { N } } \end{array}$ , so together with $V _ { \phi } ( 0 ) = V ( 0 )$ 

$$
V (t) = V _ {\phi} (t) = \sum_ {i = 1} ^ {n} \phi_ {i} \mathrm{d} X _ {i}.
$$

Since the definition of the martingale measure $\mathbb { Q } ^ { N }$ was totally independent of V we have Theorem 79 (Risk-Neutral Valuation Formula, Universal Pricing Theorem): Let $\phi$ denote an admissible self-financing trading strategy and $\mathbb { Q } ^ { N }$ an equivalent martingale measure with respect to the numeraire´ N with $\begin{array} { r } { \mathsf { E } ^ { \mathbb { Q } ^ { N } } \left( \Big | \frac { V _ { \phi } ( T ) } { N ( T ) } \Big | ^ { 2 } \right) \ < \ \infty } \end{array}$ . Then 

$$
\frac {V _ {\phi} (t)}{N (t)} = \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {V _ {\phi} (T)}{N (T)} \mid \mathcal {F} _ {t}\right).\tag{3.24}
$$

## 3.3. Excursus: Relative Prices and Risk Neutral Measures

## 3.3.1. Why relative prices?

In our simple example from Section 3.1.2, using time-discrete processes with discrete states, it became apparent that the useful martingale measure may be chosen independently of the payof function only if we consider relative prices. However, looking at the continuous time theory from Section 3.2.2, the consideration of relative prices seems to be less motivated. To motivate the relative prices we repeat steps of the continuous time theory by considering absolute prices: 

Let 

$$
\mathrm{d} X _ {i} = \mu_ {i} \cdot \mathrm{d} t + \sigma_ {i} \cdot \mathrm{d} W _ {i} ^ {\mathbb {P}}, i = 1, \ldots , n
$$

denote the price processes of n traded assets. We assume that $\sigma _ { i } > 0 , \forall i .$ The processes are given under the real measure P. Since $\sigma _ { i } > 0 _ { : }$ , we have from Girsanov’s Theorem that there exists a measure $\mathbb { Q } ^ { 1 }$ , such that the processes are $\mathbb { Q } ^ { 1 }$ -martingales, i.e. 

$$
\mathrm{d} X _ {i} = \sigma_ {i} \cdot \mathrm{d} W _ {i} ^ {\mathbb {Q} ^ {1}}, \quad i = 1, \dots , n.
$$

If $V ^ { T }$ denotes a given payof function, then 

$$
V (t) := \mathrm{E} ^ {\mathbb {Q} ^ {1}} (V ^ {(T)} \mid \mathcal {F} _ {t})\tag{3.25}
$$

is a $\mathbb { Q } ^ { 1 }$ -martingale and from the martingale representation theorem we get the existence of a portfolio process $( \phi _ { 1 } , \ldots , \phi _ { n } )$ with 

$$
\mathrm{d} V (t) = \sum_ {i = 1} ^ {n} \phi_ {i} \cdot \mathrm{d} X _ {i}.
$$

At this point we have to ask ourselves whether $( \phi _ { 1 } , \ldots , \phi _ { n } )$ is a self-financing replication portfolio, i.e. whether 

$$
V (t) = \sum_ {i = 1} ^ {n} \phi_ {i} \cdot X _ {i}.
$$

Without this identity $V ( t ) - V ( 0 )$ is just the gain process of the trading strategy $( \phi _ { 1 } , \ldots , \phi _ { n } ) . ^ { 6 }$ The key in the construction of the self-financing replication portfolio was the ability to use one asset as storage, here e.g. $X _ { 1 }$ . We divided by this asset and applied the representation theorem only to the remaining $n - 1$ processes $\frac { X _ { 2 } } { X _ { 1 } } , \ldots , \frac { X _ { n } } { X _ { 1 } }$ . After that we could use $\phi _ { 1 }$ to ensure self-financing since $\begin{array} { r } { \frac { X _ { 1 } } { X _ { 1 } } ~ ( = 1 ) } \end{array}$ did not carry any risk (see Lemma 70). So: 

• If we use the representation theorem on $( X _ { 1 } , \ldots , X _ { n } )$ we find a representation of the gain process, but it is not clear if the portfolio $( \phi _ { 1 } , \ldots , \phi _ { n } )$ is self-financing and replicating. 

• If we use the representation theorem on $( X _ { 2 } , \ldots , X _ { n } )$ and set $\phi _ { 1 }$ through Lemma 70, then the portfolio $( \phi _ { 1 } , \ldots , \phi _ { n } )$ is self-financing, but it is not clear if the portfolio replicates $V ^ { ( T ) }$ 

<sup>6</sup> Reconsider the definition of self-financing: The required condition is $\begin{array} { r } { \mathrm { d } ( \sum _ { i = 1 } ^ { n } \phi _ { i } X _ { i } ) = \sum _ { i = 1 } ^ { n } \phi _ { i } \mathrm { d } X _ { i } } \end{array}$ 

In order to construct a self-financing replicating trading strategy there has to be an assets that (locally) does not carry any risk. The n processes $X _ { 1 } , \ldots , X _ { n }$ have to be driven by $n - 1$ brownian motions, i.e. the $n - 1$ processes $\frac { \dot { X } _ { 2 } } { X _ { 1 } } , \dots , \frac { X _ { n } } { X _ { 1 } }$ have to be driven by $n - 1$ brownian motions. 

We consider price processes as before, however now let $\sigma _ { 1 } = 0$ and, e.g., $\mu _ { 1 } = r \cdot X _ { 1 }$ with $r > 0$ and $X _ { 1 } ( 0 ) > 0$ . In this case $X _ { 1 }$ corresponds to the value of a riskless $( \sigma _ { 1 } = 0 )$ asset with continuously compounded interest rate r: 

$$
\mathrm{d} X _ {1} = r \cdot X _ {1} \cdot \mathrm{d} t, \quad \text { i.e. } \quad X _ {1} (t) = X _ {1} (0) \cdot \exp (r \cdot t).
$$

Obviously, there exists no measure under which $X _ { 1 }$ would be a martingale. The product is riskless, i.e. $X _ { 1 }$ is not stochastic and the expectation is thus independent of the probability measure. To make all processes martingales via a change of measure we have to move to relative prices. Dividing all processes by $N : = X _ { 1 }$ we have $\begin{array} { r l r } { \frac { X _ { 1 } } { N } } & { { } = } & { 1 } \end{array}$ , which trivially is a martingale (under any measure). The remaining processes $\frac { X _ { i } } { N }$ are either risky (i.e. with nonzero volatility) or martingales (i.e. if they are riskless they are constant), since the presence of a riskless N-relative process with drift diferent from 1 would imply arbitrage.<sup>7</sup> 

It is not necessary to chose the riskless asset as numeraire. We could have divided by any´ asset. Either $\frac { X _ { 1 } } { N }$ is stochastic (i.e. has non zero volatility) and can be turned into a martingale by a change of measure, or $\frac { X _ { 1 } } { N }$ is drift-free.<sup>8</sup> 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/2fa36ff754640dd93c81d3956ec3b1d5b44c89eb0c75e6a83d5782805360ce58.jpg)


Interpretation: The transformation to relative prices corresponds to the transformation of the riskless rate of return (drift) to 0. This corresponds to the change of the frame of reference in physics. Since there is only one riskless asset, there is only one measure under which all processes become martingales. With this mea-

sure we can use the martingale representation theorem to derive the universal pricing theorem. 

## 3.3.2. Risk Neutral Measure

For each numeraire´ N there usually exists a diferent equivalent martingale measure $\mathbb { Q } ^ { N }$ . As risk-neutral measure we denote the equivalent martingale measure $\mathbb { Q } ^ { B }$ corresponding to the (locally) riskless asset B with 

$$
\mathrm{d} B = r \cdot B \cdot \mathrm{d} t.
$$

The name risk-neutral measure stems from the following considerations: Under the measure $\mathbb { Q } ^ { B }$ we have for any financial asset S that $\frac { S } { B }$ is a martingale. Thus, relative to B, S does not have any additional drift. So under $\mathbb { Q } ^ { B }$ the asset S has the same local rate of return as the riskless asset B, i.e. we have (written as a lognormal process) 

$$
\mathrm{d} S = r \cdot S \cdot \mathrm{d} t + \sigma \cdot S \cdot \mathrm{d} W ^ {\mathbb {Q} ^ {B}}.
$$

If $\mathbb { Q } ^ { B }$ had been the real measure, then this would imply that the real local rate of return of S would be the same as B. In such a market all assets would have the same local rate of return, namely r, independent of their risk $\sigma .$ . In other words: On average, the market participants are neutral with respect to risk: they are neither risk-afine, nor risk-averse. 

In general one would expect that under the real measure all risky assets $( \sigma > 0 )$ have a local rate of return, i.e. drift, $> r ,$ since investors like to get rewarded for the risk they take. There are however counter examples: For a lottery the expected payof is usually much less than the initial investment, since the lottery pays out only a part of the total investments. 

Part II. 

First Applications: Black-Scholes Model, Hedging and Greeks 

# Pricing of a European Stock Option under the Black-Scholes Model

We assume here that interest rates are deterministic and that a bank account exists which may be used to invest or draw cash at a continuously compounded rate $r ( t )$ , i.e. the investment of $B ( 0 ) = 1$ in $t = 0$ evolves as 

$$
\mathrm{d} B (t) = r (t) B (t) \mathrm{d} t,
$$

i.e. 

$$
B (t) = \exp \left(\int_ {0} ^ {t} r (\tau) \mathrm{d} \tau\right)\tag{4.1}
$$

(here r denotes a known real valued function of time, not a random variable). Furthermore we assume that the stock $S \left( t \right)$ follows 

$$
\mathrm{d} S (t) = \mu^ {\mathbb {P}} (t) S (t) \mathrm{d} t + \sigma (t) S (t) \mathrm{d} W ^ {\mathbb {P}} (t) \quad \text { under   the   real   measure } \mathbb {P},\tag{4.2}
$$

(if <sub>σ</sub> is a constant, then $\sigma$ is called Black-Scholes volatility). The measure P denotes the real measure. Let $K \in \mathbb { R }$ . We wish to derive the value V(0) of the contract paying 

$$
V (T) = \max (S (T) - K, 0)
$$

in $t = T$ 

We use the techniques from Chapter 3 (the following steps will be repeated similarly in other applications): As a Numeraire´ $N ( t )$ , i.e. as reference quantity, we choose the bank account $N ( t ) : = B ( t )$ . From Theorem 74 we have the existence of a measure $\mathbb { Q } ^ { N }$ , equivalent to $\mathbb { P } ,$ such that $\frac { S ( t ) } { N ( t ) }$ and $\frac { V ( t ) } { N ( t ) }$ are both martingales.<sup>1</sup> From Theorem 58 S is given $\mathbb { Q } ^ { N }$ with a changed drift, i.e. 

$$
\mathrm{d} S (t) = \mu^ {\mathbb {Q} ^ {N}} (t) S (t) \mathrm{d} t + \sigma (t) S (t) \mathrm{d} W ^ {\mathbb {Q} ^ {N}} (t) \quad \text { under } \mathbb {Q} ^ {N},
$$

<sup>1</sup> By V(t) we denote the value of the replication portfolio consisting of S (t), B(t) such that $V ( T ) = \operatorname* { m a x } ( S ( T ) - K , 0 )$ 

(where $W ^ { \mathbb { Q } ^ { N } }$ denotes a $\mathbb { Q } ^ { N }$ -Brownian motion).<sup>2</sup> From the quotient rule 48 we find 

$$
\begin{array}{l} \mathrm{d} \left(\frac {S (t)}{B (t)}\right) = \frac {S (t)}{B (t)} \big [ \mu^ {\mathbb {Q} ^ {N}} (t) \mathrm{d} t + \sigma (t) \mathrm{d} W ^ {\mathbb {Q} ^ {N}} (t) \big ] - \frac {S (t)}{B (t)} \big [ r (t) \mathrm{d} t \big ] \\ - \frac {S (t)}{B (t)} \big [ \mu^ {\mathbb {Q} ^ {N}} (t) \mathrm{d} t + \sigma (t) \mathrm{d} W ^ {\mathbb {Q} ^ {N}} (t) \big ] \big [ r (t) \mathrm{d} t \big ] \\ - \frac {S (t)}{B (t)} \big [ r (t) \mathrm{d} t \big ] \big [ r (t) \mathrm{d} t \big ] \end{array}
$$

and by formal expansion, see Theorem 45 

$$
= \frac {S (t)}{B (t)} \left[ \left(\mu^ {\mathbb {Q} ^ {N}} (t) - r (t)\right) \mathrm{d} t + \sigma (t) \mathrm{d} W ^ {\mathbb {Q} ^ {N}} (t) \right] \quad \text { under } \mathbb {Q} ^ {N}.
$$

From Lemma 52 it follows that $\mu ^ { \mathbb { Q } ^ { N } } ( t ) = r ( t )$ . For the process $Y : = \log ( S )$ we then have by Lemma 49 

$$
\mathrm{d} (\log (S (t)) = (r (t) - \frac {1}{2} \sigma^ {2} (t)) \mathrm{d} t + \sigma (t) \mathrm{d} W ^ {\mathbb {Q} ^ {N}} (t) \quad \text { under } \mathbb {Q} ^ {N},
$$

i.e. log(S (T)) has normal distribution with mean $\bar { \mu } : = \mathrm { l o g } ( S ( 0 ) ) + \bar { r } T - { \textstyle { \frac { 1 } { 2 } } } \bar { \sigma } ^ { 2 } T$ and standard deviation $\bar { \sigma } \sqrt { T }$ , where we define ¯r and ¯ as 

$$
\bar {r} = \frac {1}{T} \left(\int_ {0} ^ {T} r (t) \mathrm{d} t\right)
$$

$$
\bar {\sigma} = \left(\frac {1}{T} \int_ {0} ^ {T} \sigma^ {2} (t) \mathrm{d} t\right) ^ {1 / 2}. ^ {3}
$$

That the distribution of $\log ( S ( T ) )$ is normal follows from the definition of the Ito process: Byˆ 

$$
\mathrm{d} (\log (S (t)) = (r (t) - \frac {1}{2} \sigma^ {2} (t)) \mathrm{d} t + \sigma (t) \mathrm{d} W ^ {\mathbb {Q} ^ {N}} (t)
$$

we have just stated that 

$$
\begin{array}{l} \log (S (T)) = \log (S (0)) + \int_ {0} ^ {T} (r (t) - \frac {1}{2} \sigma^ {2} (t)) \mathrm{d} t + \int_ {0} ^ {T} \sigma (t) \mathrm{d} W ^ {\mathbb {Q} ^ {N}} (t) \\ = \log (S (0)) + \bar {r} T - \frac {1}{2} \bar {\sigma} ^ {2} T + \int_ {0} ^ {T} \sigma (t) \mathrm{d} W ^ {\mathbb {Q} ^ {N}} (t) \\ = \log (S (0)) + \bar {r} T - \frac {1}{2} \bar {\sigma} ^ {2} T + \bar {\sigma} W ^ {\mathbb {Q} ^ {N}} (T). \end{array}
$$

We thus know the dynamics of S (t) and $B ( t )$ and more importantly the distribution of $S ( T )$ under the measure $\mathbb { Q } ^ { N }$ . Furthermore we know that the value of $V ( 0 )$ satisfies 

$$
\frac {V (0)}{B (0)} = \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {V (T)}{B (T)}\right),
$$

<sup>2</sup> Since B has no stochastic component, i.e. does not depend on the path parameter <sub>ω</sub> ∈ Ω, (4.1) holds under $\mathbb { Q } ^ { N }$ too. 

thus (with $B ( 0 ) = 1 , B ( T ) = \exp ( \bar { r } T ) )$ 

$$
\begin{array}{l} V (0) = B (0) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} \Big (\frac {V (T)}{B (T)} \Big) = 1 \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} \Big (\frac {\max (S (T) - K , 0)}{\exp (\bar {r} T)} \Big) \\ = \exp (- \bar {r} T) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} \Big (\max (S (T) - K, 0) \Big) \\ = \exp (- \bar {r} T) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} \Big (\max (\exp (\log (S (T))) - K, 0) \Big) \\ = \exp (- \bar {r} T) \cdot \int_ {- \infty} ^ {\infty} \max (\exp (y) - K, 0) \cdot \frac {1}{\bar {\sigma}   \sqrt {T}} \phi \Big (\frac {y - \bar {\mu}}{\bar {\sigma}   \sqrt {T}} \Big)   \mathrm{d} y, \end{array}
$$

where $\begin{array} { r } { \phi ( x ) : = \frac { 1 } { \sqrt { 2 \pi } } \exp ( - x ^ { 2 } / 2 ) } \end{array}$ denotes the density of the standard normal distribution. The above integral may be represented as 

$$
V (0) = S (0) \Phi (d _ {+}) - \exp (- \bar {r} T) K \Phi (d _ {-}),\tag{4.3}
$$

where $\begin{array} { r } { \Phi ( x ) : = \frac { 1 } { \sqrt { 2 \pi } } \int _ { - \infty } ^ { x } \exp ( \frac { - y ^ { 2 } } { 2 } } \end{array}$ )dy and $\begin{array} { r } { d _ { \pm } = \frac { 1 } { \bar { \sigma } \sqrt { T } } \big [ \log ( \frac { S ( 0 ) } { K } ) + \bar { r } T \pm \frac { \bar { \sigma } ^ { 2 } T } { 2 } \big ] . } \end{array}$ 

To derive this formula we consider for given $K , \mu , \sigma \in \mathbb { R } \left( \sigma > 0 \right)$ 

$$
\begin{array}{l} \int_ {- \infty} ^ {\infty} \max (\exp (y) - K, 0) \cdot \frac {1}{\sigma} \phi (\frac {y - \mu}{\sigma}) \mathrm{d} y \\ = \int_ {\log (K)} ^ {\infty} (\exp (y) - K) \cdot \frac {1}{\sqrt {2 \pi} \sigma} \exp (- \frac {(y - \mu) ^ {2}}{2 \sigma^ {2}}) \mathrm{d} y \\ = \frac {1}{\sqrt {2 \pi} \sigma} \int_ {\log (K)} ^ {\infty} \exp (y) \cdot \exp (- \frac {(y - \mu) ^ {2}}{2 \sigma^ {2}}) \mathrm{d} y \\ - \frac {1}{\sqrt {2 \pi} \sigma} K \int_ {\log (K)} ^ {\infty} \exp (- \frac {(y - \mu) ^ {2}}{2 \sigma^ {2}}) \mathrm{d} y. \end{array}
$$

It is 

$$
\begin{array}{l} \frac {1}{\sqrt {2 \pi} \sigma} \int_ {\log (K)} ^ {\infty} \exp (y) \cdot \exp (- \frac {(y - \mu) ^ {2}}{2 \sigma^ {2}}) \mathrm{d} y \\ = \frac {1}{\sqrt {2 \pi} \sigma} \int_ {\log (K)} ^ {\infty} \exp (- \frac {(y - \mu) ^ {2} - 2 \sigma^ {2} y}{2 \sigma^ {2}}) \mathrm{d} y \end{array}
$$

$$
\begin{array}{r l} \mathrm{n} (y - \mu) ^ {2} - 2 \sigma^ {2} y & = (y - (\mu + \sigma^ {2})) ^ {2} - 2 \mu \sigma^ {2} - \sigma^ {4} \\ & = \frac {1}{\sqrt {2 \pi} \sigma} \int_ {\log (K)} ^ {\infty} \exp (- \frac {(y - (\mu + \sigma^ {2})) ^ {2}}{2 \sigma^ {2}} + \mu + \frac {1}{2} \sigma^ {2}) \mathrm{d} y \\ & = \frac {1}{\sqrt {2 \pi} \sigma} \exp (\mu + \frac {1}{2} \sigma^ {2}) \int_ {\log (K)} ^ {\infty} \exp (- \frac {(y - (\mu + \sigma^ {2})) ^ {2}}{2 \sigma^ {2}}) \mathrm{d} y \end{array}
$$

and with the substitution ${ \frac { y - ( \mu + \sigma ^ { 2 } ) } { \sigma } } \mapsto y$ 

$$
= \frac {1}{\sqrt {2 \pi}} \exp (\mu + \frac {1}{2} \sigma^ {2}) \int_ {\frac {\log (K) - (\mu + \sigma^ {2})}{\sigma}} ^ {\infty} \exp (- \frac {y ^ {2}}{2}) d y.
$$

<sup>4</sup> We denote the cumulative normal distribution function by Φ. In some books, especially in connection with the Black-Scholes model, it is denoted by N (which we usually use for the numeraire). Instead of´ $d _ { + } , d _ { - }$ one often uses the symbols $d _ { 1 } , d _ { 2 }$ 

Similarly we have with the substitution $\frac { y - \mu } { \sigma } \mapsto y$ 

$$
\begin{array}{l} \frac {1}{\sqrt {2 \pi} \sigma} K \int_ {\log (K)} ^ {\infty} \cdot \exp (- \frac {(y - \mu) ^ {2}}{2 \sigma^ {2}}) \mathrm{d} y \\ = \frac {1}{\sqrt {2 \pi}} K \int_ {\frac {\log (K) - \mu}{\sigma}} ^ {\infty} \exp (- \frac {y ^ {2}}{2}) \mathrm{d} y \end{array}
$$

Defining $\begin{array} { r } { \Phi ( x ) : = \frac { 1 } { \sqrt { 2 \pi } } \int _ { - \infty } ^ { x } \exp \big ( - \frac { y ^ { 2 } } { 2 } \big ) \mathrm { d } y } \end{array}$ we thus get from $\begin{array} { r } { \frac { 1 } { \sqrt { 2 \pi } } \int _ { x } ^ { \infty } \exp \big ( - \frac { y ^ { 2 } } { 2 } \big ) \mathrm { d } y = \Phi ( - x ) } \end{array}$ that 

$$
\begin{array}{l} \int_ {- \infty} ^ {\infty} \max (\exp (y) - K, 0) \cdot \frac {1}{\sigma} \phi (\frac {y - \mu}{\sigma}) \mathrm{d} y \\ \qquad = \exp (\mu + \frac {1}{2} \sigma^ {2}) \Phi (\frac {\mu + \sigma^ {2} - \log (K)}{\sigma}) - K \Phi (\frac {\mu - \log (K)}{\sigma}). \end{array}
$$

Remark 80 (Implied Black-Scholes Volatility): From Equation (4.3) and the definition of $d _ { \pm }$ we see that under the model (4.2) the price of an option depends on $S ( 0 ) , \bar { r }$ and $\bar { \sigma }$ only (apart from product parameters like T and K). The parameter 

$$
\bar {\sigma} = \left(\frac {1}{T} \int_ {0} ^ {T} \sigma^ {2} (t) \mathrm{d} t\right) ^ {1 / 2}
$$

is called the Black-Scholes volatility, while $\sigma ( t )$ is called the instantaneous volatility of the model (4.2). The Black-Scholes volatility is the square root of the average instantaneous variance (which is the square of the instantaneous volatility)<sup>5</sup>. 

For fixed S (0), ¯r the pricing formula (4.3) is a bijection 

$$
\begin{array}{c} \bar {\sigma} \mapsto V (0) \\ [ 0, \infty) \to [ \max (S (0) - \exp (- \bar {r} T) K, 0), S (0) ] \end{array}
$$

and thus we may calculate the Black-Scholes volatility corresponding to a given price $V ( 0 )$ This volatility is called the implied Black-Scholes volatility. 

# Excursus: The Density of the Underlying of a European Call Option

Lemma 81 (Probability density of the underlying of a European call option): Let S denote a price process and N a numeraire on the probability space´ $( \mathbb { R } , \mathcal { B } ( \mathbb { R } ) , \mathbb { Q } ^ { N } )$ . Let $K \in \mathbb { R }$ and $T _ { 0 } < T _ { 1 } \leq T _ { 2 }$ , where $T _ { 1 }$ denotes a fixing date and $T _ { 2 }$ a payment date of a European option with payout 

$$
V (K; T _ {2}) := \max (S (T _ {1}) - K, 0).
$$

Let us further assume that the numeraire´ N has been chosen such that $N ( T _ { 2 } ) = 1$ . Then we have for the probability density<sup>1</sup> $\phi _ { S ( T _ { 1 } ) } ( s )$ of $S ( T _ { 1 } )$ under $\mathbb { Q } ^ { N }$ 

$$
\phi_ {S (T _ {1})} (s) = \frac {1}{N (T _ {0})} \cdot \left. \frac {\partial^ {2} V (K , T _ {0})}{\partial K ^ {2}} \right| _ {K = s},
$$

i.e. 

$$
\frac {\partial^ {2} V (K , T _ {0})}{\partial K ^ {2}} = N (T _ {0}) \cdot \phi_ {S (T _ {1})} (K) = \frac {\mathrm{d} \mathbb {Q} ^ {N}}{\mathrm{d} S} (\{\omega : S (\omega) = K \}).
$$

Remark 82 (Application): We may apply Lemma 81 to European stock options $( T _ { 1 } = T _ { 2 }$ and $N ( t ) = \exp ( r \cdot ( T _ { 1 } - t ) )$ , see Section 4, or to Caplets, see Section 10. 

If a model is given (e.g. as a “black box” through some pricing software) and if the model allows the pricing of arbitrary European options, then we can use this Lemma to infer the probability distribution of S (T) created by this model. This allows for some simple model tests: If the probability density is 0 in any region, then the model should be discarded if these regions play any role in the pricing. If the model exhibits regions with negative probability density, then the model is not arbitrage-free. It is easy to set up interpolatory models that fail when tested by this lemma. See Chapter 6. 

Proof: Under the measure $\mathbb { Q } ^ { N }$ , N-relative prices are martingales. Thus we have 

$$
\frac {V (K ; T _ {0})}{N (T _ {0})} = \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {V (K ; T _ {2})}{N (T _ {2})}\right)
$$

<sup>1</sup> To be precise, $\phi _ { S ( T _ { 1 } ) } ( s )$ is the conditional probability density, conditioned on $\mathcal { F } _ { T _ { 0 } }$ . For simplicity we assume that $\mathcal { F } _ { T _ { 0 } } = \{ 0 , \Omega \}$ and write $\mathsf { E } ^ { \mathbb { Q } ^ { N } } ( \cdot )$ for $\mathrm { E } ^ { \mathbb { Q } ^ { N } } ( \cdot | \mathcal { F } _ { T _ { 0 } } )$ 

i.e. 

$$
\begin{array}{l} V (K; T _ {0}) = N (T _ {0}) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {V (K ; T _ {2})}{N (T _ {2})}\right) \\ = N (T _ {0}) \cdot \int_ {\Omega} \max (S (T _ {1}; \omega) - K, 0)   \mathrm{d} \mathbb {Q} ^ {N} (\omega) \\ = N (T _ {0}) \cdot \int_ {- \infty} ^ {\infty} \max (s - K, 0) \cdot \phi_ {S (T _ {1})} (s)   \mathrm{d} s, \end{array}
$$

and thus 

$$
\begin{array}{r l} \frac {\partial}{\partial K} V (K; T _ {0}) & = N (T _ {0}) \cdot \int_ {- \infty} ^ {\infty} - 1 _ {[ 0, \infty)} (s - K) \phi_ {S (T _ {1})} (s)   \mathrm{d} s \\ & = N (T _ {0}) \cdot \int_ {K} ^ {\infty} - \phi_ {S (T _ {1})} (s)   \mathrm{d} s, \end{array}
$$

i.e. 

$$
\frac {\partial^ {2}}{\partial K ^ {2}} V (K; T _ {0}) = N (T _ {0}) \cdot \phi_ {S (T _ {1})} (K).
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/970c052c7d8ac86c477ca42d6a00a0d2aedfe5e20d4224c1b9f642d3104bb2e3.jpg)


As a direct consequence we have 

Lemma 83 (Prices of European options are convex): Prices of European options are a convex function of the strike. 

# Excursus: Interpolation of European Option Prices

Insufficient facts always invite danger. 

Spock 

Space Seed, stardate 3141.9, (Wikiquote). 

## 6.1. No-Arbitrage Conditions for Interpolated Prices

We consider the price $V ( K ; 0 )$ of a European option with payof ma $( S ( T ) - K , 0 )$ as a function of the strike K. We assume $S ( T ) \geq 0$ . Let $P ( T ; 0 )$ denote the value of the zero-coupon bond with nominal 1.<sup>1</sup> From Lemma 83, the mapping 

$$
K \mapsto V (K)
$$

(we write shortly V(K) for $V ( K ; 0 ) )$ , which maps a strike K to the corresponding option price $V ( K )$ (for fixed, given maturity T and notional 1), has to satisfy the following conditions: 

• V(0) = P(T; 0) · S (0) (since $S ( T ) \geq 0 )$ 

$V ( K ) = V ( 0 ) - P ( T ; 0 ) \cdot K$ for $K < 0$ (since $S ( T ) \geq 0 )$ , i.e. V(K) is linear for $K < 0 .$ 

$\operatorname* { l i m } _ { K \to \infty } V ( K ) = 0 ,$ 

$\begin{array} { r } { \frac { \mathrm { d } ^ { 2 } V } { \mathrm { d } K ^ { 2 } } \geq 0 } \end{array}$ (from Lemma 81), i.e. V(K) is convex. 

Given strikes $K _ { 1 } < K _ { 2 }$ and corresponding option prices $V ( K _ { 1 } )$ and $V ( K _ { 2 } )$ respectively, we find geometric conditions for the possible (arbitrage-free) strike-price-points $( K , V ( K ) )$ . The price points $c = ( K _ { 1 } , V ( K _ { 1 } ) )$ and $d = ( K _ { 2 } , V ( K _ { 2 } ) )$ as well as $a = ( - 1 , V ( 0 ) - P ( T ; 0 ) ) , b =$ $( 0 , V ( 0 ) )$ and $e = ( 0 , V ( K _ { 2 } ) )$ define lines ab, bc, cd and de which are boundaries of the set of admissible strike-price points. As depicted in Figure 6.1 we have: 

• For $K < K _ { 1 } < K _ { 2 }$ 

$$
- V (K) \geq V (0) - P (T; 0) \cdot K
$$

$$
((K, V (K)) \geq \overline {{a b}}).
$$

<sup>1</sup> See 1.3.3 on the notation P(T; 0). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/cb8c90d7f9ed484974aaa898486f4f3d89f644148f1cf6a92790ade8f65d610a.jpg)



Figure 6.1.: Arbitrage-free option prices for European options (payof max $( S ( T ) - K , 0 ) )$ with strike $K < K _ { 1 }$ or $K _ { 1 } < K < K _ { 2 }$ or $K > K _ { 2 } ;$ assuming that two option prices V(K<sub>1</sub>) > V(K<sub>2</sub>) (for $K _ { 1 } < K _ { 2 } )$ are given.


$$
- V (K) \geq V (K _ {1}) \frac {K _ {2} - K}{K _ {2} - K _ {1}} + V (K _ {2}) \frac {K - K _ {1}}{K _ {2} - K _ {1}}\tag{\(((K,V(K))\geq \overline{cd}).\}
$$

$$
- V (K) \geq V (0) + (V (K _ {1}) - V (0)) \frac {K}{K _ {1}}\tag{\(((K,V(K))\leq \overline{bc}).\}
$$

• For $K _ { 1 } < K < K _ { 2 } ;$ 

$$
- V (K) \geq V (K _ {0}) + (V (K _ {1}) - V (0)) \frac {K}{K _ {1}}\tag{\(((K,V(K))\geq \overline{bc}).\}
$$

((K<sub>,</sub> V(K)) ≥ de). 

$$
- V (K) \leq V (K _ {1}) \frac {K _ {2} - K}{K _ {2} - K _ {1}} + V (K _ {2}) \frac {K - K _ {1}}{K _ {2} - K _ {1}}\tag{\(((K,V(K))\leq \overline{cd}).\}
$$

• For $K _ { 1 } < K _ { 2 } < K $ 

$$
\begin{array}{l} - V (K) \geq V (K _ {1}) \frac {K _ {2} - K}{K _ {2} - K _ {1}} + V (K _ {2}) \frac {K - K _ {1}}{K _ {2} - K _ {1}} \\ - V (K) \leq V (K _ {2}) \end{array}\tag{\(((K,V(K))\geq \overline{cd}).\}
$$

((K<sub>,</sub> V(K)) ≤ de). 

## 6.2. Arbitrage Violations through Interpolation

In this section we give some examples to show that simple interpolation of prices or implied volatilities may lead to arbitrage. 

## 6.2.1. Example (1): Interpolation of four Prices

Consider a stock S with a current value of $S ( 0 ) = 1 . 0 $ and a European option on S having maturity $T = 1 . 0$ and strike K, i.e. we consider the payof 

$$
\max (S (1. 0) - K, 0).
$$

Assume that for strikes K = 0 5 0 75 1 25 2 0 the following prices were given: 

<table><tr><td>i</td><td>Strike <eq>K_i</eq></td><td>Price <eq>V(K_i)</eq></td><td>Implied Volatility <eq>\sigma(K_i)</eq></td></tr><tr><td>1</td><td>0.50</td><td>0.5277</td><td>0.4</td></tr><tr><td>2</td><td>0.75</td><td>0.3237</td><td>0.4</td></tr><tr><td>3</td><td>1.25</td><td>0.1739</td><td>0.6</td></tr><tr><td>4</td><td>2.00</td><td>0.0563</td><td>0.6</td></tr></table>


The given implied volatility is the of a Black-Scholes Model with assumed interest rate (short rate) of $r = 0 . 0 5$ . Note however that we start with given prices which are model-independent. 


We will now discuss several “obvious” interpolation methods applied to this data. One approach consists of the interpolation of prices, the other approach consists of the interpolation of implied volatilities and calculating interpolated prices from the interpolated volatilities. These interpolations are not model-independent. The interpolation method itself constitutes a model. This is obvious with the second approach, where a model is involved in the calculation, but also applies to the first approach. From Lemma 81 we have that the interpolation method constitutes a model for the underlying’s probability density. It does not model the underlying’s dynamics. 

## 6.2.1.1. Linear Interpolation of Prices

In Figure 6.2 we show the linear interpolation of the given option prices. The prices do not allow arbitrage, which is obvious from the convexity of their linear interpolation. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/ca2d6db26be5c3aed8658baa565da36fcf51a914f2a71aaadafd908eb8d3ed19.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/199baed9c66756c436efc2413f0c396dbad0304f179f0a09bcd0f0309d996c13.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/4f525686692bfef45f7a8482f20ad4fbf967c018d311548549459918701c4d00.jpg)



Figure 6.2.: Linear interpolation ofoption prices.


However, the linear interpolation of prices has severe disadvantages: The linear interpolation of option prices implies a model under which the underlying may not attain values $K \neq K _ { i }$ the corresponding probability density is zero for these values. For values corresponding to the given strikes $K _ { i }$ a point measure is assigned, see Figure 6.2, right. In addition the corresponding implied volatilities look strange. 

## 6.2.1.2. Linear Interpolation of Implied Volatilities

In Figure 6.2 we show the linear interpolation of the corresponding implied volatilities (center), while the corresponding prices are re-calculated via the Black-Scholes formula (left). The linear interpolation of implied (Black-Scholes) volatilities may lead to prices allowing for arbitrage: At the edges $K = 0 . 7 5$ and $K = 1 . 2 5$ we have a point measure, the measure for $S ( T ) = 1 . 2 5$ being negative. Thus the implied measure is not a probability measure, see Figure 6.2, right. From Lemma 81 we have: There is no arbitrage-free pricing model that generates this interpolated price curve. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/69ca64d93d0846d32c6df08800e6af42809baa4663ea511d50d6e4a796993cf2.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/5c9f9f2c5c11ce3a0526fe9da25f079e3dc79e2821f76dc3b7fc70e6cea0203a.jpg)



Figure 6.3.: Linear interpolation ofimplied volatilities.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/acb304b38114f2a8ec51fb4fcf37aea1b7fab3aad109baa07a92f40d28cd1b49.jpg)


On the other hand, linear interpolation of implied volatilities also has a nice property: If the given prices correspond to prices from a Black-Scholes model, i.e. if the implied volatilities are constant, then, trivially, the interpolated prices correspond to the same Black-Scholes model. 

## 6.2.1.3. Spline Interpolation of Prices and Implied Volatilities

To remove the disadvantage of degenerated densities (i.e. the formation of point measures) as it appears for a linear interpolation, we move to a smooth (diferentiable) interpolation method, e.g. spline interpolation. Figure 6.4 shows the spline interpolation of the given data. The upper row shows the spline interpolation of the option prices. The lower row shows the spline interpolation of the implied volatilities. Using (cubic) spline interpolation the probability densities 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/cb61c89c65e02ae021d1a27f812939306df32ddbb6d0efd4de87486b41fbacac.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/e24c25e84d9110f24c3cf791c93a3d80ca17f9906a00c22da36515cfe25d88ff.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/d5b32da2b561817918d3331e86bf144f354f0ab652865e5e877e7b230f3d145c.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/8e348c131e85fbe709c7d79a7e339471a98be3583b3edd780a323af5440c5992.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/fe7e832a1960378918839638a79cc2b68c1390df0da8527364622f08c9cb9618.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/fa0911d3bda469fe74195ef0b70400ca663c459bd8c6cfcf7a4baf5606ae918b.jpg)



Figure 6.4.: Spline interpolation ofoption prices (upper row) and implied volatilities (lower row)


are continuous functions. However, it shows large regions with negative densities (Figure 6.4 right), thus the density is not a probability density and arbitrage possibilities exist. The strike price-curve is not convex (Figure 6.4, left). 

A spline interpolation of prices generates negative densities, because the spline interpolation of convex sample points is not convex. 

## 6.2.2. Example (2): Interpolation of two Prices

The example from Section 6.2.1 of a linear interpolation of implied volatilities may suggest that the problem arises at the joins of the linear interpolation, i.e. the behavior at $K _ { 2 } = 0 . 7 5$ and $K _ { 3 } = 1 . 2 5$ . One could hope that a local smoothing would solve this problem. Instead we will give an example showeing that a linear growth of implied volatility may be inadmissible alone, although the interpolated prices are admissible. 

We consider two prices $V ( K _ { 2 } ) > V ( K _ { 3 } )$ . The monotony ensures that these two prices alone do not allow for an arbitrage. 

## 6.2.2.1. Linear Interpolation for decreasing Implied Volatilities

Consider the following prices 

<table><tr><td>i</td><td>Strike <eq>K_i</eq></td><td>Price <eq>V(K_i)</eq></td><td>Implied Volatility <eq>\sigma(K_i)</eq></td></tr><tr><td>2</td><td>0.75</td><td>0.4599</td><td>0.9</td></tr><tr><td>3</td><td>1.25</td><td>0.0018</td><td>0.1</td></tr></table>

The implied volatility decreases with the strike K. Figure 6.5 shows the linear interpolation of the implied volatilities (center). The density (see Figure 6.5, right) shows a large region with 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/eac4c5409933bca015aa96d91c928945e6d6709e0dec8c3c22148adc85c8ce57.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/fd34288e05e03cb654ac15e5a47f9e9226718acd47d558d15f2fd028808ee478.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/fcaff1fe5ff83acdd07defedb9353263c6a3fec2b339d16b81828fd8d4987418.jpg)



Figure 6.5.: Linear interpolationfor decreasing implied volatility.


negative values, thus it is not a probability density. The reason is a too fast decay of the implied volatility. 

Conclusion: An arbitrarily fast decrease of implied volatility is not possible. 

## 6.2.2.2. Linear Interpolation for increasing Implied Volatilities

For the example of increasing implied volatility we consider the prices 

<table><tr><td>i</td><td>Strike <eq>K_i</eq></td><td>Price <eq>V(K_i)</eq></td><td>Implied Volatility <eq>\sigma(K_i)</eq></td></tr><tr><td>2</td><td>0.75</td><td>0.2897</td><td>0.2</td></tr><tr><td>3</td><td>1.25</td><td>0.2532</td><td>0.8</td></tr></table>

Figure 6.5 shows the linear increasing interpolation of the implied volatilities. 

At first sight the density implied by the linear interpolation of the implied volatilities exhibits no flaw (positive, no point measure). However, it is not a probability density. The integral below the segment is larger than 1. That this is inevitable is obvious from the price curve. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/dd9cd146b59312cd1d99c8a7d050550ac24009c19379d4baca20b7197fb8ec64.jpg)



Figure 6.6.: Linear interpolationfor increasing implied volatility


The price curve is convex (and thus the density positive), but not monotone. The arbitrage is obvious, since the option with strike 1 0 is cheaper than the option with strike 1 25. If the prices should converge to 0 for increasing strike, then it is inevitable that the convexity will be violated. Thus it is inevitable that the density will exhibit a region with negative values beyond the interpolation region (this however will make the integral of the density to 1). 

Conclusion: An arbitrarily fast increase of implied volatility is not possible. 

## 6.3. Arbitrage-Free Interpolation of European Option Prices

The examples of the previous sections bring up the question for arbitrage-free interpolation methods. 

Every arbitrage-free pricing model defines an arbitrage-free interpolation method, if it is able to reproduce the given prices. However, this insight is almost useless, since: 

• Most models are not able to reproduce arbitrarily given prices exactly. 

– The Black-Scholes model (Chapter 4) and (in its simplest form) the LIBOR Market model (Chapter 19) allow, by the choice of their volatility, the perfect fit for only one European option per maturity. 

– Extended models (e.g. models with stochastic volatility), which allow for a calibration to more than one option price per maturity, do this in an approximative way, i.e. the residual error of the fitting is minimized, but not necessarily 0. However, this may also be a desired efect, since such a fitting is more robust against errors in the input data. 

• Extended models, that fit more than one option price per maturity usually require great efort to find the corresponding model parameters. These models are intended for the pricing of complex derivatives (which justifies the efort), but not primarily as an interpolation method to price European options. Examples of such model extensions are stochastic volatility or jump-difusion extensions of the LIBOR Market Model, [23]. 

• Some models even require a continuum of European option prices K 7→ V(T K) as input. Then they require an interpolation. An example for such a model is the Markov Functional Model, see Chapter 25. 

Thus, special methods and models have been developed to specifically achieve the interpolation of given European option prices. Often they reproduce given prices only approximately in the sense of a “best $\mathrm { \ f t ^ { \prime \prime } }$ – they are not an interpolation in the original sense. The construction of an (interpolating or approximating) price function $( T , K ) \mapsto V ( T , K )$ of European option prices with maturity T and strike K is called modeling ofthe volatility surface. 

## Definition 84 (Volatility Surface):

Given a continuum $( T , K ) \mapsto V ( T , K )$ of prices of European options with maturity T and strike K. Let $\sigma ( T , K )$ denote the implied volatility of $V ( T , K )$ , i.e. the volatility for which a riskneutral pricing with a lognormal model $\mathrm { d } S = r S \mathrm { d } t + \sigma ( T , K ) S \mathrm { d } W , S ( 0 ) = S _ { 0 }$ (Black-Scholes model) will reproduce the prices $V ( T , K )$ . Then $( T , K ) \mapsto \sigma ( T , K )$ is called volatility surface. 

The modeling of a volatility surface may be viewed as important post processing of market data. On the other hand it may be viewed as an integral part of the pricing model. A detailed discussion of volatility surface modeling is beyond the scope of this little excursus and we restrict ourself to citing a few methods: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/231adf30ddd6b24ec9878f4799ce8ef05345b8fcfd8659fc655263671173a8ac.jpg)


Further Reading: The mixture of lognormal approach [54] uses the fact that if the probability density $\phi _ { S } ( T )$ of the underlying $S ( T )$ is given as convex combination 

$$
\phi_ {S (T)} = \sum_ {i = 1} ^ {n} \lambda_ {i} \phi_ {\sigma_ {n}}, \quad \sum_ {i = 1} ^ {n} \lambda_ {i} = 1, \quad \lambda_ {i} \geq 0
$$

of lognormal densities $\phi _ { \sigma _ { i } }$ , then the price of a European option is given as a convex combination (using the same weights $\vec { \lambda _ { i } ^ { \mathrm { ~ s ) } } }$ of corresponding Black-Scholes formulas.<sup>2</sup> In some cases this allows for a choice of the $\phi _ { \sigma _ { i } } \mathrm { ' s }$ and $\lambda _ { i } ^ { \mathrm { ~ ~ } } \mathrm { { s } }$ that exactly reproduces given option prices. However, the method is not able to reproduce arbitrary arbitrage-free prices. 

In [62] Fengler applies a cubic spline interpolation with an additional shape constraint to given option prices. This leads to an arbitrage-free smoothing algorithm for the implied volatility. 

The SABR model [71] is a four parameter model $( \sigma , \alpha , \beta , \rho )$ for European interest rate options (the underlying is an interest rate, see 8). It reproduces given prices only approximately, but models a more realistic behavior of the dependency of the volatility surface from the spot value of the underlying. C| 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/1d307212d7f19ed45a8600ee0cf776353460ce6d609962df5eff5d6812e688d7.jpg)


Experiment: At http://www.christian-fries.de/finmath/ applets/OptionPriceInterpolation.html several interpolation methods may be applied to a user-defined configuration of European option prices. The figures in this chapter were produced with this software. C| 

# Hedging in Continuous and Discrete Time and the Greeks

## 7.1. Introduction

The evaluation theory we have presented so far relies on the possibility of replicating a financial derivative by a portfolio of traded assets (replication portfolio) and a self-financing strategy. 

If we assume a perfect replication, we can evaluate a derivative product without explicitly deriving the replicating strategy. This is made possible by the introduction of the equivalent martingale measure and the universal pricing theorem. However, in practice the price calculated by this risk-neutral evaluation theory makes sense only if the corresponding replication is conducted. Thus, it is necessary to explicitly determine the replication portfolio in order to do the replication. 

In the first part of this chapter we will show that the replication strategy may be derived from the risk-neutral evaluation surprisingly simply. 

Depending on the state space modeled, the following basic requirement has to hold in order to replicate arbitrary payof functions: 

• To replicate arbitrary payof functions modeled over a continuous state space it is in general necessary to trade continuously and in infinitesimal amounts of the underlyings. The existence of such a replicating trading strategy is ensured by the martingale representation theorem, see Theorem 53, Page 44. 

• To replicate arbitrary payof functions modeled over a finite, discrete state space, it is only necessary to trade at discrete times. However, the number of traded assets (underlyings) has to match the number of possible state transitions over one time step, see Section 3.1.2, Page 56. 

Both modelings (continuous or discrete replication) do not represent reality exactly: On the one hand it is not possible to trade continuously in infinitesimal amounts; On the other hand the number of possible states is usually much larger than the number of traded assets.<sup>1</sup> 

Apart from the question of how to derive the replication strategy for time-continuous trading, we are especially interested in the replication when trading takes place at discrete points in time only. In this case, which is closer to reality, a complete replication is not possible. A residual risk remains. 

## Definition 85 (Hedge):

A replication portfolio (almost) replicating a derivative product and thus, if considered together with the derivative product neutralizing (reducing) the total risk, is called a (partial or incomplete) hedge. The corresponding trading strategy is called hedging. y 

First we will derive the delta hedge, delta-gamma hedge and vega hedge from the risk-neutral evaluation theory (Section 7.2). We will then transfer these hedges to the case of trading in discrete time, these being incomplete hedges, and analyse the residual error (Section 7.4). 

Bouchaud-Sornette method (Section 7.5) determines the replication portfolio that minimizes the residual risk. The residual risk has to be measured in the real measure P. There is a real risk of a loss due to incomplete hedging. The real measure is no longer irrelevant since a complete replication is no longer possible. 

## 7.2. Deriving the Replications Strategy from Pricing Theory

Let $\mathcal { M } : = \{ S _ { 0 } , S _ { 1 } , \ldots , S _ { n } \}$ denote a set of Ito price processes, representing a complete marketˆ of traded assets. Let the process $N = S _ { 0 }$ be a numeraire and´ $\mathbb { Q } ^ { N }$ the corresponding martingale measure. Let $t \mapsto V ( t )$ denote the price process of a derivative product, i.e. 

$$
V (t) = N (t) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {V (T)}{N (T)} | \mathcal {F} _ {t}\right).
$$

We assume that the value of the derivative product V can be written as a function of $( t , S _ { 0 } ( t ) , S _ { 1 } ( t ) , \ldots , S _ { n } ( t ) )$ , i.e. we have 

$$
V (t) = V (t, S _ {0} (t), S _ {1} (t), \ldots , S _ {n} (t)).\tag{7.1}
$$

If V(t) is given by an evaluation theory - i.e. an analytic formula or pricing algorithm - as a function of the underlyings, then the self-financing replication portfolio 

$$
\Pi (t) := \phi_ {0} (t) S _ {0} (t) + \phi_ {1} (t) S _ {1} (t) + \ldots + \phi_ {n} (t) S _ {n} (t)\tag{7.2}
$$

with $\Pi ( t ) = V ( t )$ (replication) may be determined as follows: 

The property that Π is self-financing may be written as (see Definition 66) 

$$
\mathrm{d} \Pi (t) = \phi_ {0} (t) \mathrm{d} S _ {0} + \phi_ {1} (t) \mathrm{d} S _ {1} (t) + \dots + \phi_ {n} (t) \mathrm{d} S _ {n} (t) = \sum_ {i = 0} ^ {n} \phi_ {i} \mathrm{d} S _ {i}.
$$

Furthermore we find from Ito’s Lemmaˆ (Theorem 46) applied to (7.1) 

$$
\mathrm{d} V (t) = \frac {\partial V (t)}{\partial t} \mathrm{d} t + \sum_ {i = 0} ^ {n} \frac {\partial V (t)}{\partial S _ {i}} \mathrm{d} S _ {i} + \frac {1}{2} \sum_ {i, j = 0} ^ {n} \frac {\partial^ {2} V (t)}{\partial S _ {i} \partial S _ {j}} \underbrace {\mathrm{d} S _ {i} \mathrm{d} S _ {j}} _ {= (\dots) \mathrm{d} t}.
$$

From $\mathrm { d } \Pi ( t ) = \mathrm { d } V ( t )$ (replication), we find $\phi _ { 0 } , . . . , \phi _ { n }$ by comparing coeficients. It is 

$$
\phi_ {0} (t) = \frac {\partial V (t)}{\partial S 0}, \phi_ {1} (t) = \frac {\partial V (t)}{\partial S _ {1}}, \dots , \phi_ {n} (t) = \frac {\partial V (t)}{\partial S _ {n}}\tag{7.3}
$$

$$
\frac {\partial V (t)}{\partial t} \mathrm{d} t + \frac {1}{2} \sum_ {i, j = 0} ^ {n} \frac {\partial^ {2} V (t)}{\partial S _ {i} \partial S _ {j}} \underbrace {\mathrm{d} S _ {i} \mathrm{d} S _ {j}} _ {= (\dots) \mathrm{d} t} = 0.\tag{7.4}
$$

Conclusion: Under a model, which permits the evaluation of V through a martingale measure and universal pricing theorem, i.e. without explicit construction of the replication portfolio, the replication portfolio may be calculated a posteriori from the partial derivative of the price after the underlyings. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/71d581fe97b135da4ee0e173cb316fd045057fc1db8127d6358061e3358ea7f7.jpg)


Interpretation: Comparing coeficients of dV and dΠ we find the equations (7.3) for the replication portfolio process $\phi .$ . The partial diferential equation (7.4) is just a reformulation that 

$$
V (t) = V (t, S _ {0} (t), S _ {1} (t), \ldots , S _ {n} (t))
$$

is the value process of a self-financing portfolio in the coordinates $( S _ { 0 } ( t ) , S _ { 1 } ( t ) , \ldots , S _ { n } ( t ) ) )$ The Equation (7.4) may be used together with thefinal condition 

$$
V (T, S _ {0} (T), S _ {1} (T), \ldots , S _ {n} (T)) = V ^ {T}
$$

to determine $V ( t )$ for $t < T$ from the given payof profile $V ^ { T }$ . This is the entry point to the pricing of derivatives by partial diferential equations, see Chapter 2.11. C| 

## 7.2.1. Deriving the Replication Strategy under the Assumption of a Locally Riskless Product

The ansatz $V ( t ) = V ( t , S _ { 0 } ( t ) , S _ { 1 } ( t ) , \ldots , S _ { n } ( t ) )$ is just one possible way of interpreting V as a function of the underlyings. It is a specific choice of the coordinate system leading to very natural equations for the portfolio parameters and the partial diferential equations for V. If $N = S _ { 0 }$ is locally riskfree we may easily give V in the coordinates $( t , S _ { 1 } ( t ) , \ldots , S _ { n } ( t ) )$ alone. A special case which we consider now: Let $N \ = \ S _ { 0 }$ denote a locally risk free numeraire,´ i.e. assume that the process $N \left( \mathrm { i } . \mathrm { e } . \ S _ { 0 } \right)$ is of the form 

$$
\mathrm{d} N = \frac {\partial N}{\partial t} \mathrm{d} t,\tag{7.5}
$$

i.e. we assume that dN does not have a dW-component.<sup>2</sup> For $N > 0 ( N$ is a numeraire) we´ have $\begin{array} { r } { r : = \frac { \partial \log ( N ) } { \partial t } } \end{array}$ 

$$
\mathrm{d} N = \frac {\partial N}{\partial t} \mathrm{d} t = \frac {\partial \log (N)}{\partial t} N \mathrm{d} t = r N \mathrm{d} t.\tag{7.6}
$$

<sup>2</sup> The property is local, since $\textstyle { \frac { \partial N } { \partial t } }$ may very well be stochastic. An example would be ${ \mathrm { d } } N = r \cdot N \cdot { \mathrm { d } } t ,$ as it was considered for the Black-Scholes model in Section 4. 

We assume that for a given $N V ( t )$ is given as a function in the coordinates $( t , S _ { 1 } ( t ) , \ldots , S _ { n } ( t ) )$ and denote this function by V again, i.e. 

$$
V (t) = V (t, S _ {1} (t), \dots , S _ {n} (t)).\tag{7.7}
$$

In other words: N is no longer a modeled free quanti $\mathbf { \cdot y } . ^ { 3 }$ 

If V(T) is given in this from, we may derive the self-financing replication portfolio (7.2) with $\Pi ( t ) = V ( t )$ as follows: From Ito’s Lemma (Theoremˆ 46), applied to $V ( t , S _ { 1 } ( t ) , \ldots , S _ { n } ( t ) )$ we have 

$$
\mathrm{d} V (t) = \frac {\partial V (t)}{\partial t} \mathrm{d} t + \sum_ {i = 1} ^ {n} \frac {\partial V (t)}{\partial S _ {i}} \mathrm{d} S _ {i} + \frac {1}{2} \sum_ {i, j = 1} ^ {n} \frac {\partial^ {2} V (t)}{\partial S _ {i} \partial S _ {j}} \underbrace {\mathrm{d} S _ {i} \mathrm{d} S _ {j}} _ {= (\dots) \mathrm{d} t}.
$$

With $\begin{array} { r } { \mathrm { d } \Pi ( t ) = \sum _ { i = 0 } ^ { n } \phi _ { i } \mathrm { d } S _ { i } = \mathrm { d } V ( t ) } \end{array}$ self-financing of Π, replication of V) we find $\phi _ { 0 } , \ldots , \phi _ { n }$ by comparing the coeficients of dt und $\mathrm { d } S _ { i } , i \geq 1$ as 

$$
\begin{array}{c} \phi_ {1} (t) = \frac {\partial V (t)}{\partial S _ {1}}, \ldots , \phi_ {n} (t) = \frac {\partial V (t)}{\partial S _ {n}} \\ \phi_ {0} (t) \frac {\partial N}{\partial t} \mathrm{d} t = \frac {\partial V (t)}{\partial t} \mathrm{d} t + \frac {1}{2} \sum_ {i, j = 1} ^ {n} \frac {\partial^ {2} V (t)}{\partial S _ {i} \partial S _ {j}} \underbrace {\mathrm{d} S _ {i} \mathrm{d} S _ {j}} _ {= (\ldots) \mathrm{d} t}. \end{array}\tag{7.8}
$$

The equation for $\phi _ { 0 }$ seems unnaturally complex when compared to the equation for $\phi _ { 1 }$ , , $\phi _ { n } .$ . This is a consequence of the representation (7.7) which we had assumed for $V ,$ see Section 7.2.3. However, since the portfolio is self-financing it is not necessary to calculate φ from (7.8); φ<sub>0</sub> follows from the condition of self-financing portfolios: $\textstyle \sum _ { i = 0 } ^ { n } ( \mathrm { d } \phi _ { i } ) \cdot S _ { i } = 0$ 

## 7.2.2. The Black-Scholes Differential Equation

Writing $\begin{array} { r } { \frac { \partial N } { \partial t } = \frac { \partial \log ( N ) } { \partial t } \cdot N = : r N } \end{array}$ the equation for $\phi _ { 0 }$ in (7.8) becomes 

$$
\phi_ {0} (t) r (t) N (t) \mathrm{d} t = \frac {\partial V (t)}{\partial t} \mathrm{d} t + \frac {1}{2} \sum_ {i, j = 1} ^ {n} \frac {\partial^ {2} V (t)}{\partial S _ {i} \partial S _ {j}} \underbrace {\mathrm{d} S _ {i} \mathrm{d} S _ {j}} _ {= (\dots) \mathrm{d} t}.
$$

Since $\begin{array} { r } { V = \phi _ { 0 } N + \sum _ { i = 1 } ^ { n } \phi _ { i } S _ { i } \stackrel { ( 7 . 8 ) } { = } \phi _ { 0 } N + \sum _ { i = 1 } ^ { n } \frac { \partial V ( t ) } { \partial S _ { i } } S _ { i } } \end{array}$ we also have $\begin{array} { r } { \phi _ { 0 } N = V - \sum _ { i = 1 } ^ { n } \frac { \partial V ( t ) } { \partial S _ { i } } S _ { i } } \end{array}$ and denoting the instantaneous correlations by $\rho _ { i , j } ,$ i.e. $\mathrm { d } S _ { i } \mathrm { d } S _ { j } = \sigma _ { i } \sigma _ { j } \rho _ { i , j } \mathrm { d } t$ we arrive at 

$$
\frac {\partial V (t)}{\partial t} + r (t) \sum_ {i = 1} ^ {n} \frac {\partial V (t)}{\partial S _ {i}} S _ {i} + \frac {1}{2} \sum_ {i, j = 1} ^ {n} \frac {\partial^ {2} V (t)}{\partial S _ {i} \partial S _ {j}} \sigma_ {i} \sigma_ {j} \rho_ {i, j} = r (t) V (t).
$$

This is a variant of the Black-Scholes partial diferential equation in the coordinates $( t , S _ { 1 } , \ldots , S _ { n } )$ 

## 7.2.3. The Derivative V(t) as a Function of its Underlyings $S _ { i } ( t )$

The representation of the portfolio process components $\phi _ { i }$ as a partial derivative of V as well as the partial diferential equation for V depend of course on the chosen coordinate system of the underlyings. Instead of comparing coeficients of $\mathrm { d } S _ { i } , i \geq 1$ and dt (as above), in general it is possible to compare the coeficients of dt and the diferentials of the driving Brownian motions ${ \mathrm { d } } W _ { i }$ 

To illustrate that we have just considered a change (or rather substitution) of coordinates, let us reconsider V written in the two diferent coordinate systems above, i.e 

$$
\begin{array}{l} V (t) = V ^ {n + 1} (t, S _ {0} (t), S _ {1} (t), \ldots , S _ {n} (t)) \\ V (t) = V ^ {n} (t, S _ {1} (t), \ldots , S _ {n} (t)). \end{array}
$$

With $S _ { 0 } = N$ and $\mathrm { d } N ( t ) = r ( t ) N ( t ) \mathrm { d } t$ (this assumption makes it possible to replace the dependence on $S _ { 0 }$ by a dependence on t) it is 

$$
V ^ {n} (t, S _ {1}, \ldots , S _ {n}) = V ^ {n + 1} (t, N (t), S _ {1}, \ldots , S _ {n}),
$$

thus 

$$
\frac {\partial V ^ {n}}{\partial t} = \frac {\partial V ^ {n + 1}}{\partial t} + \frac {\partial V ^ {n + 1}}{\partial N} \cdot \frac {\partial N}{\partial t} = \frac {\partial V ^ {n + 1}}{\partial t} + \phi_ {0} \cdot \frac {\partial N}{\partial t},
$$

i.e. 

$$
\frac {\partial V ^ {n}}{\partial t} - \phi_ {0} \cdot \frac {\partial N}{\partial t} = \frac {\partial V ^ {n + 1}}{\partial t}.
$$

Together with dS ${ \bf \nabla } _ { i } \mathrm { d } S _ { j } = 0$ if $i = 0$ or $j = 0$ in (7.4) this gives 

$$
\frac {\partial V (t) ^ {n + 1}}{\partial t} \mathrm{d} t + \frac {1}{2} \sum_ {i, j = 0} ^ {n} \frac {\partial^ {2} V ^ {n + 1} (t)}{\partial S _ {i} \partial S _ {j}} \underbrace {\mathrm{d} S _ {i} \mathrm{d} S _ {j}} _ {= (\dots) \mathrm{d} t} = 0
$$

⇔ 

$$
\frac {\partial V ^ {n} (t)}{\partial t} \mathrm{d} t - \phi_ {0} \cdot \frac {\partial N}{\partial t} \mathrm{d} t + \frac {1}{2} \sum_ {i, j = 1} ^ {n} \frac {\partial^ {2} V ^ {n} (t)}{\partial S _ {i} \partial S _ {j}} \underbrace {\mathrm{d} S _ {i} \mathrm{d} S _ {j}} _ {= (\dots) \mathrm{d} t} = 0
$$

⇔ 

$$
\frac {\partial V ^ {n} (t)}{\partial t} + r (t) \sum_ {i = 1} ^ {n} \frac {\partial V ^ {n} (t)}{\partial S _ {i}} S _ {i} + \frac {1}{2} \sum_ {i, j = 1} ^ {n} \frac {\partial^ {2} V ^ {n} (t)}{\partial S _ {i} \partial S _ {j}} \sigma_ {i} \sigma_ {j} \rho_ {i, j} = r (t) V ^ {n} (t)\tag{7.9}
$$

## 7.2.3.1. Path-dependent options

Our assumption that $V ( t )$ is a function of $S _ { i } ( t )$ excludes path-dependent options. However, our considerations may be easily extended to the case of path-dependent options by writing $V$ as a function of the corresponding path quantities. For example, considering a path-dependent option of the form $\begin{array} { r } { V ( t ) ~ = ~ V ( t , S ( t ) , \int _ { 0 } ^ { t } S ( \tau ) \mathrm { d } \tau ) } \end{array}$ with $\begin{array} { r } { I ( t ) = \int _ { 0 } ^ { t } S ( \tau ) \mathrm { d } \tau } \end{array}$ we derive $\mathrm { d } V ( t ) =$ $\begin{array} { r } { \frac { \partial V ( t ) } { \partial t } \mathbf { d } t + \frac { \partial V ( t ) } { \partial S } \mathbf { d } S + \frac { \partial V ( t ) } { \partial I } \dot { \mathbf { c } } } \end{array}$ I and substitute $\mathrm { d } I ( t ) = S ( t ) \mathrm { d } t$ . For the replication portfolio we thus $\begin{array} { r } { \operatorname* { g e t } \phi _ { 1 } = \frac { \partial V ( t , S , I ) } { \partial S } } \end{array}$ 

## 7.2.4. Example: Replication Portfolio and Partial Differential Equation of a European Option under a Black-Scholes Model

As an illustration we reconsider these calculations for a simple model, the Black-Scholes model, with price processes N for the savings account and S for the stock 

$$
\begin{array}{l} \mathrm{d} N (t) = r N (t) \mathrm{d} t, \\ \mathrm{d} S (t) = \mu S (t) \mathrm{d} t + \sigma S (t) \mathrm{d} W (t), \end{array}
$$

$$
\begin{array}{l} {N (0) = 1,} \\ {S (0) = S _ {0}.} \end{array}
$$

For a European option with strike K and maturity T, i.e. Payout max $( S ( T ) - K , 0 ) ) \stackrel { ! } { = } V ( T )$ the Black-Scholes-Merton formula (4.3) for the value V at time t 

$$
V (t, S (t)) = S (t) \Phi (d _ {+}) - \exp (- \bar {r} (T - t)) K \Phi (d _ {-}),
$$

$\begin{array} { r } { d _ { \pm } = \frac { 1 } { \bar { \sigma } \sqrt { ( T - t ) } } \big [ \log ( \frac { S ( t ) } { K } ) + \bar { r } ( T - t ) \pm \frac { \bar { \sigma } ^ { 2 } ( T - t ) } { 2 } \big ] . } \end{array}$ , see (4.3) on Page 77 in Chapter 4. 

This gives V as a function of t und S (t), since r is seen as constant and thus $N ( t )$ is known as a deterministic function of t. With $N ( t ) = \exp ( r \cdot t )$ we may write V as a function of $( t , N ( t ) , S ( t ) )$ namely 

$$
V (t, N (t), S (t)) = S (t) \Phi (d _ {+}) - N (t) \frac {K}{N (T)} \Phi (d _ {-}),\tag{7.10}
$$

where 

$$
d _ {\pm} = \frac {1}{\bar {\sigma} \sqrt {(T - t)}} [ \log (\frac {S (t)}{N (t)} \cdot \frac {N (T)}{K}) \pm \frac {\bar {\sigma} ^ {2} (T - t)}{2} ].
$$

It is 

$$
\begin{array}{r l} & {\frac {\partial V}{\partial S (t)} = \Phi (d _ {+}) + S (t) \phi (d _ {+}) \frac {1}{S (t)} \frac {1}{\sigma \sqrt {T - t}} - N (t) \frac {K}{N (T)} \phi (d _ {-}) \frac {1}{S (t)} \frac {1}{\sigma \sqrt {T - t}}} \\ & {\qquad = \Phi (d _ {+}) + \frac {1}{S (t)} \frac {1}{\sigma \sqrt {T - t}} \cdot \left(S (t) \phi (d _ {+}) - N (t) \frac {K}{N (T)} \phi (d _ {-})\right)} \\ & {\qquad = \Phi (d _ {+}) + \frac {1}{S (t)} \frac {1}{\sigma \sqrt {T - t}} \cdot \left(S (t) \phi (d _ {+}) - N (t) \frac {K}{N (T)} \phi (d _ {-})\right)} \end{array}
$$

With 

$$
\begin{array}{l} \phi (d _ {\pm}) = C \cdot \exp (- \frac {1}{2} d _ {\pm} ^ {2}) \\ \qquad = C \cdot \exp \Big [ - \frac {\log (\frac {S (t)}{N (t)} \cdot \frac {N (T)}{K}) ^ {2} \pm 2 \log (\frac {S (t)}{N (t)} \cdot \frac {N (T)}{K}) \cdot \frac {\bar {\sigma} ^ {2} (T - t)}{2} + \frac {\bar {\sigma} ^ {4} (T - t) ^ {2}}{4}}{2 \bar {\sigma} ^ {2} (T - t)} \Big ] \\ \qquad = C \cdot \exp \Big [ \pm \frac {1}{2} \log (\frac {N (t)}{S (t)} \cdot \frac {K}{N (T)}) - \frac {\log (\frac {S (t)}{N (t)} \cdot \frac {N (T)}{K}) ^ {2} + \frac {\bar {\sigma} ^ {4} (T - t) ^ {2}}{4}}{2 \bar {\sigma} ^ {2} (T - t)} \Big ] \\ \qquad = (\frac {N (t)}{S (t)} \cdot \frac {K}{N (T)}) ^ {\pm 1 / 2} \cdot C \cdot \exp \Big [ - \frac {\log (\frac {S (t)}{N (t)} \cdot \frac {N (T)}{K}) ^ {2} + \frac {\bar {\sigma} ^ {4} (T - t) ^ {2}}{4}}{2 \bar {\sigma} ^ {2} (T - t)} \Big ] \end{array}
$$

we $\begin{array} { r } { \mathrm { g e t } \phi ( d _ { - } ) = \frac { S ( t ) } { N ( t ) } \cdot \frac { N ( T ) } { K } \cdot \phi ( d _ { + } ) } \end{array}$ and thus 

$$
\frac {\partial V}{\partial S (t)} = \Phi (d _ {+}) + \frac {1}{S (t)} \frac {1}{\sigma \sqrt {T - t}} \cdot \big (\underbrace {S (t) \phi (d _ {+}) - N (t) \frac {K}{N (T)} \phi (d _ {-})} _ {= 0} \big) = \Phi (d _ {+}).
$$

Similarly, we can derive 

$$
\frac {\partial V}{\partial N (t)} = - \frac {K}{N (T)} \cdot \Phi (d _ {-}).
$$

To sum up, we have $V ( t , N ( t ) , S \left( t \right) ) = \phi _ { 0 } ( t ) N ( t ) + \phi _ { 1 } ( t ) S \left( t \right)$ with 

$$
\phi_ {0} (t) = - \frac {K}{N (T)} \cdot \Phi (d _ {-}), \quad \phi_ {1} (t) = \Phi (d _ {+}).
$$

Indeed, we might simply have read of the representation of the replication portfolio from (7.10). 

For the function 

$$
V (t, n, s) = s \Phi (d _ {+}) - n \frac {K}{N (T)} \Phi (d _ {-})
$$

with 

$$
d _ {\pm} = \frac {1}{\bar {\sigma} \sqrt {(T - t)}} \big [ \log (\frac {s}{n} \cdot \frac {N (T)}{K}) \pm \frac {\bar {\sigma} ^ {2} (T - t)}{2} \big ].
$$

it is 

$$
\frac {\partial V (t)}{\partial t} \mathrm{d} t + \frac {1}{2} \frac {\partial^ {2} V (t)}{\partial n \partial n} \mathrm{d} N \mathrm{d} N + \frac {\partial^ {2} V}{\partial n \partial s} \mathrm{d} N \mathrm{d} S + \frac {1}{2} \frac {\partial^ {2} V (t)}{\partial s \partial s} \mathrm{d} S \mathrm{d} S = 0
$$

$$
\begin{array}{c} \mathrm{d} N \mathrm{d} N = 0 \\ \mathrm{d} N \mathrm{d} S = 0 \\ \Longleftrightarrow \end{array}
$$

$$
\frac {\partial V (t)}{\partial t} \mathrm{d} t + \frac {1}{2} \frac {\partial^ {2} V (t)}{\partial s \partial s} \sigma^ {2} = 0.
$$

See Exercise 10. Furthermore, the final condition 

$$
V (T, N (T), s) = \max (s - K, 0)
$$

holds. 

## 7.2.4.1. Interpretation of V as a Function in (t S )

For the Black-Scholes model, the classical way is to write V as a function of t and $S \left( t \right)$ only. In this case we get (see (7.8)) 

$$
\begin{array}{c} \phi_ {1} = \frac {\partial V (t)}{\partial S} = \Phi (d _ {+}) \\ \phi_ {0} r N = (\frac {\partial V (t)}{\partial t} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} V (t)}{\partial S ^ {2}}), \end{array}
$$

In addition we have from $V = \phi _ { 0 } N + \phi _ { 1 } S$ 

$$
\phi_ {0} N = V - \phi_ {1} S,
$$

which brings us once again to the Black-Scholes partial diferential equation 

$$
\begin{array}{l} r V = r \phi_ {0} (t) N (t) + r \phi_ {1} S (t) \\ = \frac {\partial V (t)}{\partial t} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} V (t)}{\partial S ^ {2}} + r \frac {\partial V (t)}{\partial S} S \end{array}
$$

and thus 

$$
\frac {\partial V (t)}{\partial t} + r \frac {\partial V (t)}{\partial S} S + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} V (t)}{\partial S ^ {2}} = r V.
$$

## Definition 86 (Delta Hedge):

This choice of the replication portfolio given in (7.2), (7.3) is called Delta hedge 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/0683665364f2b154a618e2128327f21e82aa1ddc3ed3738962ab798f9ec6c70e.jpg)


Interpretation: Considering the derivative product V as a function of the underlyings S , then the portfolio Π given by the delta hedge is the local linear approximation of V, see Figure 7.2. For a fixed path <sub>ω</sub> the map $t \mapsto S ( t , \omega )$ is almost surely continuous (a property of Ito processes) and on that path weˆ 

have $\begin{array} { r } { V ( T ) = \int _ { 0 } ^ { T } \mathrm { d } V = \int _ { 0 } ^ { T } \mathrm { d }  V = \int _ { 0 } ^ { T } } \end{array}$ dΠ. This corresponds to the main theorem of ordinary calculus: $\begin{array} { r } { f ( T ) = \int _ { 0 } ^ { T } \mathrm { d } f = \int _ { 0 } ^ { T } f ^ { \prime } ( t ) \mathrm { d } t } \end{array}$ (e.g. for diferentiable f). This illustrates, why the portfolio Π is only required to coincide with V upon their first derivative by S , i.e. the so called delta: $\begin{array} { r } { \frac { \partial V } { \partial S } = \frac { \partial \Pi } { \partial S } } \end{array}$ C| 

## 7.3. Greeks

The partial derivatives of the value V(t) of a derivative product upon product- or modelparameters are important quantities. They describe how the product reacts to infinitesimal changes and are essential for the construction of the replication portfolios. These quantities are usually denoted by Greek letters and therefore called Greeks. Here we give definitions of the most important greeks: 

## Definition 87 (Delta):

The first order partial derivative of the price of a derivative product with respect to the underlyings is called delta. It is the first order sensitivity of the derivative product to price changes of the market traded assets (or market quotes). y 

## Definition 88 (Gamma):

The second order partial derivative of the price of a derivative product with respect to the underlyings is called gamma. It is the second order sensitivity of the derivative product to price changes of the market traded assets (or market quotes). y 

## Definition 89 (Vega<sup>4</sup>):

The first order partial derivative of the price of a derivative product with respect to the underlyings log-volatility is called vega. It is the first order sensitivity of the derivative product to log-volatility changes of the market traded European options. y 

## Definition 90 (Theta):

The first order partial derivative of the price of a derivative product with respect to time is called theta. It is the first order sensitivity of the derivative product to time. y 

## Definition 91 (Rho):

The first order partial derivative of the price of a derivative product with respect to the interest rate (r) is called rho. It is the first order sensitivity of the derivative product to a change in interest rate. 

The definition of rho is only used for models with non-stochastic interest rates. For interest rate derivatives (evaluated under a model of stochastic interest rates), as will be considered in the later chapters, the interest rates are underlyings and rho is just a delta. y 

## 7.3.1. Greeks of a european Call-Option under the Black-Scholes model

Given the Black-Scholes model with price processes for the savings account N and the stock S 

$$
\begin{array}{l l} \mathrm{d} N (t) = r N (t) \mathrm{d} t, & N (0) = 1, \\ \mathrm{d} S (t) = \mu S (t) \mathrm{d} t + \sigma S (t) \mathrm{d} W (t), & S (0) = S _ {0}, \end{array}
$$

consider a european stock option with payout max $( S ( T ) - K , 0 ) ) \stackrel { ! } { = } V ( T )$ . From Chapter 4 the price V(0) of the option under this model is given by the Black-Scholes-Merton formula (4.3): 

$$
V (0) = S _ {0} \Phi (d _ {+}) - \exp (- r T) K \Phi (d _ {-}),
$$

where $\begin{array} { r } { \Phi ( x ) : = \frac { 1 } { \sqrt { 2 \pi } } \int _ { - \infty } ^ { x } \exp ( \frac { y ^ { 2 } } { 2 } ) \mathrm { d } y } \end{array}$ and $\begin{array} { r } { d _ { \pm } = \frac { 1 } { \sigma \sqrt { T } } \big [ \log ( \frac { S ( 0 ) } { K } ) + r T \pm \frac { \sigma ^ { 2 } T } { 2 } \big ] } \end{array}$ . Thus, the price is a function of $S _ { 0 } , r , K , \sigma$ and T. 

From the Black-Scholes-Merton formula we may derive the Greeks analytically. They are given in Table 7.1. 

<table><tr><td>Greek</td><td>Definition</td><td>within the Black-Scholes model</td></tr><tr><td>Delta (Δ)</td><td><eq>\frac{\partial V}{\partial S_0}</eq></td><td>= <eq>\Phi(d_+)</eq></td></tr><tr><td>Gamma (Γ)</td><td><eq>\frac{\partial^2V}{\partial S_0^2}</eq></td><td>= <eq>\frac{\Phi&#x27;(d_+)}{S_0\sigma\sqrt{T}}</eq></td></tr><tr><td>Vega</td><td><eq>\frac{\partial V}{\partial\sigma}</eq></td><td>= <eq>S_0\sqrt{T}\Phi&#x27;(d_+)</eq></td></tr><tr><td>Theta (Θ)</td><td><eq>-\frac{\partial V}{\partial T}</eq></td><td>= <eq>-\frac{S_0\Phi&#x27;(d_+) \sigma}{2\sqrt{T}} - rK\exp(-rT)\Phi(d_-)</eq></td></tr><tr><td>Rho (ρ)</td><td><eq>\frac{\partial V}{\partial r}</eq></td><td>= <eq>KT\exp(-rT)\Phi(d_-)</eq></td></tr></table>


Table 7.1.: Greeks within the Black-Scholes model.


## 7.4. Hedging in Discrete Time: Delta and Delta-Gamma Hedging

If a delta hedge is applied continuously, then it achieves a perfect replication. At any time, the portfolio V − Π is neutral with respect to infinitesimal changes in the underlyings $S _ { i } .$ . However, if the delta hedge is applied only at discrete times $t _ { k } ,$ i.e. the portfolio process $( \phi _ { 0 } , \phi _ { 1 } , \ldots , \phi _ { n } )$ is kept constant on time intervals $[ t _ { k } , t _ { k + 1 } )$ , then the replication is no longer exact.<sup>5</sup> While in 

continuous time 

$$
\begin{array}{l} \mathrm{d} V (t) = \frac {\partial V (t)}{\partial t} \mathrm{d} t + \sum_ {i = 0} ^ {n} \frac {\partial V (t)}{\partial S _ {i}} \mathrm{d} S _ {i} + \frac {1}{2} \sum_ {i, j = 0} ^ {n} \frac {\partial^ {2} V (t)}{\partial S _ {i} \partial S _ {j}} \mathrm{d} S _ {i} \mathrm{d} S _ {j}, \\ = \sum_ {i = 0} ^ {n} \frac {\partial V (t)}{\partial S _ {i}} \mathrm{d} S _ {i} + \underbrace {\frac {\partial V (t)}{\partial t} \mathrm{d} t + \frac {1}{2} \sum_ {i , j = 0} ^ {n} \frac {\partial^ {2} V (t)}{\partial S _ {i} \partial S _ {j}} \mathrm{d} S _ {i} \mathrm{d} S _ {j}} _ {= 0}, \end{array}
$$

is exact by Ito’s Lemmaˆ (and (7.4)), we have for the time-discrete case $( \Delta V = V ( t + \Delta t ) - V ( t ) )$ 

$$
\Delta V (t) = \frac {\partial V (t)}{\partial t} \Delta t + \sum_ {i = 0} ^ {n} \frac {\partial V (t)}{\partial S _ {i}} \Delta S _ {i} + \frac {1}{2} \sum_ {i, j = 0} ^ {n} \frac {\partial^ {2} V (t)}{\partial S _ {i} \partial S _ {j}} \underbrace {\Delta S _ {i} \Delta S _ {j}} _ {\neq (\dots) \Delta t}\tag{7.11}
$$

$$
= \sum_ {i = 0} ^ {n} \frac {\partial V (t)}{\partial S _ {i}} \Delta S _ {i} + \frac {1}{2} \sum_ {i, j = 0} ^ {n} \frac {\partial^ {2} V (t)}{\partial S _ {i} \partial S _ {j}} \underbrace {(\Delta S _ {i} \Delta S _ {j} - \gamma_ {i , j} \Delta t)} _ {\neq 0} + \text { h.o.t. },\tag{7.12}
$$

where $\gamma _ { i , j }$ is given by $\mathrm { d } S _ { i } \mathrm { d } S _ { j } = \gamma _ { i , j } \mathrm { d } t$ and h $\mathrm { . . o . t . } = O ( | \Delta t | ^ { 2 } , | \Delta t \Delta S _ { i } | , | \Delta S _ { i } | ^ { 3 } ) . ^ { 6 }$ For comparison, for the replication portfolio we have in the time-discrete case 

$$
\Delta \Pi (t) = \sum_ {i = 0} ^ {n} \phi_ {i} \Delta S _ {i}.\tag{7.13}
$$

Assuming we have an exact replication at time $t \left( V ( t ) = \Pi ( t ) \right)$ , then there is no choice for the replication portfolio $\phi$ such that $\Delta V ( t ) = \Delta \Pi ( t )$ in general. An exact replication at time $t + \Delta t$ is not guaranteed. 

To ensure that the replication portfolio is self-financing, we have to re-formulate the requirement in the time-discrete setting. Trading at discrete times $t _ { k }$ the self-financing property is 

$$
\sum_ {i = 0} ^ {n} \bigl (\phi_ {i} (t _ {k}) - \phi_ {i} (t _ {k - 1}) \bigr) S _ {i} (t _ {k}) = 0.
$$

This may be ensured, $\mathrm { e . g . }$ , by the choice of $\phi _ { 0 }$ according to 

$$
\phi_ {0} (t _ {k}) = \phi_ {0} (t _ {k - 1}) - \frac {1}{S _ {0} (t _ {k})} \cdot \left(\sum_ {i = 1} ^ {n} \big (\phi_ {i} (t _ {k}) - \phi_ {i} (t _ {k - 1}) \big) S _ {i} (t _ {k})\right)\tag{7.14}
$$

(we have $S _ { 0 } \ne 0$ since we assumed that $S _ { 0 }$ is a numeraire). While in continuous time´ $V$ may be replicated exactly with a self-financing portfolio, there is a choice whether $\phi _ { 0 }$ is chosen to reduce the replication error or $\phi _ { 0 }$ is chosen to keep the portfolio self-financing. 

The restriction to a self-financing portfolio leads to an error propagation of the replication error via (7.14), see Section 7.4.2. 

## 7.4.1. Delta Hedging

A delta hedge determines the replication portfolio such that the delta of the replication portfolio Π matches the delta of $V .$ In other words, the delta of the replication error $V - \Pi$ is zero. The replication error to first-order insensitive to movements of the underlyings. If we consider the requirement of self-financing to be ensured by the choice of $\phi _ { 0 } ,$ then we chose 

$$
\begin{array}{l} \phi_ {i} (t _ {k}) = \frac {\partial V (t _ {k})}{\partial S _ {i}} \\ \phi_ {0} (t _ {k}) = \phi_ {0} (t _ {k - 1}) - \frac {1}{S _ {0} (t _ {k})} \cdot \left(\sum_ {i = 1} ^ {n} (\phi_ {i} (t _ {k}) - \phi_ {i} (t _ {k - 1})) S _ {i} (t _ {k})\right). \end{array}
$$

For the error $\Delta V ( t ) - \Delta \Pi ( t )$ we get from (7.12) and (7.13) 

$$
\begin{array}{l} \Delta V (t) - \Delta \Pi (t) \\ = \sum_ {i = 0} ^ {n} \left(\frac {\partial V (t)}{\partial S _ {i}} - \phi_ {i}\right) \Delta S _ {i} + \frac {1}{2} \sum_ {i, j = 0} ^ {n} \frac {\partial^ {2} V (t)}{\partial S _ {i} \partial S _ {j}} \underbrace {\left(\Delta S _ {i} \Delta S _ {j} - \gamma_ {i , j} \Delta t\right)} _ {\neq 0} + \text { h.o.t. } \end{array}
$$

and with $\begin{array} { r } { \phi _ { i } = \frac { \partial V ( t ) } { \partial S _ { i } } } \end{array}$ for $i \neq 0$ 

$$
= (\frac {\partial V (t)}{\partial S _ {0}} - \phi_ {0}) \Delta S _ {0} + \frac {1}{2} \sum_ {i, j = 0} ^ {n} \frac {\partial^ {2} V (t)}{\partial S _ {i} \partial S _ {j}} \underbrace {(\Delta S _ {i} \Delta S _ {j} - \gamma_ {i , j} \Delta t)} _ {\neq 0} + \text { h.o.t. },
$$

where $\mathrm { { h . o . t . } } = O ( { | \Delta t | ^ { 2 } } , { | \Delta t \Delta S _ { i } | } , { | \Delta S _ { i } | ^ { 3 } } )$ 

## 7.4.2. Error Propagation

The choice of $\phi _ { 0 }$ at time $t = 0$ is determined by the initial condition $\Pi ( 0 ) = V ( 0 )$ and at later times $t = t _ { k } , k = 1 , 2 , . . .$ by the requirement for a self-financing trading strategy 

$$
\sum_ {i = 0} ^ {n} \phi_ {i} (t _ {k}) S _ {i} (t _ {k}) = \sum_ {i = 0} ^ {n} \phi_ {i} (t _ {k - 1}) S _ {i} (t _ {k}).\tag{7.15}
$$

This results in an error propagation. Assuming that at time $t _ { k }$ the replication error due to the previous choice of $\phi _ { i } ( t _ { k - 1 } )$ is $\begin{array} { r } { V ( t _ { k } ) - \sum _ { i = 0 } ^ { n } \phi _ { i } ( t _ { k - 1 } ) S _ { i } ( t _ { k } ) = : e ( t _ { k } ) } \end{array}$ , then we have with 

$$
V (t _ {k}) = \sum_ {i = 0} ^ {n} \frac {\partial V (t _ {k})}{\partial S _ {i}} S _ {i} (t _ {k}), \quad \Pi (t _ {k}) = \sum_ {i = 0} ^ {n} \phi_ {i} (t _ {k}) S _ {i} (t _ {k})\tag{7.16}
$$

and $\begin{array} { r } { \phi _ { i } ( t _ { k } ) = \frac { \partial V ( t _ { k } ) } { \partial S _ { i } } } \end{array}$ for $k \neq 0$ (delta hedge), that 

$$
e (t _ {k}) = V (t _ {k}) - \sum_ {i = 0} ^ {n} \phi_ {i} (t _ {k - 1}) S _ {i} (t _ {k}) \stackrel {(7. 1 5)} {=} V (t _ {k}) - \Pi (t _ {k}) \stackrel {(7. 1 6)} {=} (\frac {\partial V (t _ {k})}{\partial S _ {0}} - \phi_ {0} (t _ {k})) \cdot S _ {0}.
$$

Thus the requirement for a self-financing portfolio implies 

$$
\phi_ {0} (t) = \frac {\partial V (t)}{\partial S _ {0}} - \frac {1}{S _ {0}} (V (t) - \Pi (t)).
$$

This shows how the replication error at time $t _ { k }$ is propagated over the time step $\Delta t$ by the requirement for a self-financing strategy through φ<sub>0</sub>. 

Summarising, we have for the delta hedge 

$$
\begin{array}{l} \Delta V (t) - \Delta \Pi (t) \\ = (V (t) - \Pi (t)) \cdot \frac {\Delta S _ {0}}{S _ {0}} + \frac {1}{2} \sum_ {i, j = 0} ^ {n} \frac {\partial^ {2} V (t)}{\partial S _ {i} \partial S _ {j}} \underbrace {(\Delta S _ {i} \Delta S _ {j} - \gamma_ {i , j} \Delta t)} _ {\neq 0} + \text { h.o.t. }, \end{array}
$$

where h. $\mathrm { _ { 0 . t . } } = O ( { | \Delta t | ^ { 2 } } , { | \Delta t \Delta S _ { i } | } , { | \Delta S _ { i } | ^ { 3 } } )$ 

## 7.4.2.1. Example: Time discrete delta hedge under a Black-Scholes model

We consider a Black-Scholes model with the notation as above. For the replication portfolio $\phi _ { 0 } ( t ) N ( t ) + \phi _ { 1 } ( t ) S ( t )$ we have $\begin{array} { r } { \phi _ { 1 } ( t ) = \frac { \partial V ( t ) } { \partial S ( t ) } = \Phi ( \frac { 1 } { \sigma \sqrt { T - t } } [ \log ( \frac { S ( t ) } { K } ) + r ( T - t ) + \frac { \sigma ^ { 2 } } { 2 } ] ) } \end{array}$ 

We use this choice to trade within the replication portfolio at discrete times $t _ { k } , k = 0 ;$ 1   . The size of the “cash position” is chosen such that the portfolio remains self-financing, i.e. 

$$
\begin{array}{l} \phi_ {1} (t _ {k}) = \frac {\partial V (t _ {k})}{\partial S (t _ {k})} = N \left(\frac {1}{\sigma \sqrt {T - t _ {k}}} [ \log (\frac {S (t _ {k})}{K}) + r (T - t _ {k}) + \frac {\sigma^ {2}}{2} ]\right) \\ \phi_ {0} (t _ {k}) = \frac {1}{N (t _ {k})} (\phi (t _ {k - 1}) N (t _ {k}) + \phi_ {1} (t _ {k - 1}) S (t _ {k}) - \phi_ {1} (t _ {k}) S (t _ {k})) \end{array}
$$

At time $t _ { 0 } = 0$ the portfolio is set up according to the option value known from the evaluation formula.<sup>7</sup> 

$$
\phi_ {0} (t _ {0}) = \frac {1}{N (t _ {0})} \bigl (V (t _ {0}) - \phi_ {1} (t _ {0}) S (t _ {0}) \bigr)
$$

Figure 7.1 shows the result of a weekly delta hedge. 


Hedge Portfolio versus Payof


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/a87161a1572c9ccd21a1670f3b21d801894f67b4a3bbb68e11e810ed1f691425.jpg)



Figure 7.1.: Samples of the value of the replication portfolio using weekly delta hedging. The market $( N , S )$ follows a Black-Scholes model $\mathrm { d } N ( t ) = r N ( t ) \mathrm { d } t ,$ , dS (t) = S (t)dt + S (t)dW(t) with $( N ( 0 ) , S ( 0 ) ) =$ $( 1 . 0 , 1 . 0 ) , r = \mu = 0 . 0 5$ and $\sigma ( t ) = 0 . 5 .$ . We aim to replicate the payout $X ( T ) = \operatorname* { m a x } ( S ( T ) - K , 0 ) )$ with $K = 1 . 0$ and $T = 6 . 0$ (green line). The replication portfolio $\Pi = \phi _ { 0 } N + \phi _ { 1 } S$ is chosen according to a delta hedge at times $\begin{array} { r } { t _ { k } = k \cdot \frac { 1 } { 5 2 } } \end{array}$ . Shown are the realized values Π(T) (red dots) over S (T). In the figure on the left the delta hedge uses the correct model parameters. In the figure on the right the portfolio is constructed assuming a volatility of 0 4 (instead of 0 5). As a result the option value is under-estimated and the replication portfolio is set up without enough initial value, such that at maturity $T = 6 . 0$ the mean of the replication portfolio is systematically below the option payout. In addition, the variance of the replication portfolio is increased, since the delta hedge used is wrong.


## 7.4.3. Delta-Gamma Hedging

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/1633c93979b0b760cef3d45e890de0e0aaf8e365c257a859d23799b6c739289a.jpg)


Motivation (The delta hedge again): A delta hedge applied in timediscrete steps $\Delta t _ { j } = t _ { j + 1 } - t _ { j }$ is not exact since the option value ${ \mathrm { i s } } ,$ in general, a non-linear function of the changes of the underlyings $\Delta S _ { i } = S _ { i } ( t _ { j + 1 } ) - S _ { i } ( t _ { j } )$ However, the replication portfolio is linear in the underlyings. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/46cd7cb5b8181cc965ceec6db982a4ebddb98bde98946e68d4788e97ecf101f2.jpg)


For motivation reconsider a market consisting of a stock S and some other numeraire asset´ N (as in the Black-Scholes model) and a derivative product V as a function of $( t , S ) \colon V = V ( t , S )$ . At fixed time $t _ { j } \ : V$ will be a non-linear function $S \mapsto V ( t _ { j } , S )$ of S in general. However, the replication portfolio $\Pi = \phi _ { 0 } N + \phi _ { 1 } S$ is linear in S . Locally, for a fixed point $S ( t _ { j } , \omega )$ the replication portfolio may match the value and the first derivative in S (the delta) of V: For in-

Figure 7.2.: Delta Hedge 

finitesimal changes dS the infinitesimal changes of derivative (dV) and replication portfolio dΠ agree. If the movements of S are within in a larger (non-infinitesimal) range $\Delta S ( t _ { j } )$ , then derivative and replication portfolio may deviate significantly. C| 

The error given by the only linear approximation of the derivative product may be reduced by adding products to the replication portfolio which are itself non-linear, e.g. options. This is possible if such products are traded and may be used for replication: Some standardised options are traded in suficient quantities and may be used to replicate derivative products that are not traded in liquid quantities. An example of such a case would be options traded at standardized maturities, which could be used to build a replication portfolio for an option with a non-standard maturity (and/or strike). 

We consider a portfolio consisting of $S _ { 0 } , S _ { 1 } , \ldots , S _ { n }$ and additional (derivative) products $C _ { 1 } , \ldots , C _ { m }$ 

$$
\Pi (t) = \phi_ {0} (t) S _ {0} (t) + \ldots + \phi_ {n} (t) S _ {n} (t) + \psi_ {1} (t) C _ {1} (t) + \ldots + \psi_ {m} (t) C _ {m} (t)
$$

Assuming that, like $V ( T )$ , the $C _ { k } ( t ) \mathrm { { ' s } }$ may be written as functions $C _ { k } ( t , S _ { 0 } , \ldots , S _ { n } )$ of the $S _ { i } { } ^ { \ ' } \mathbf { s } ,$ we have for the replication portfolio Π(t) instead of (7.13) that 

$$
\begin{array}{l} \Delta \Pi (t) = \sum_ {i = 0} ^ {n} \phi_ {i} \Delta S _ {i} + \sum_ {k = 1} ^ {m} \psi_ {k} \Delta C _ {k} \\ \qquad = \sum_ {i = 0} ^ {n} (\phi_ {i} + \sum_ {k = 1} ^ {m} \psi_ {k} \frac {\partial C _ {k}}{\partial S _ {i}}) \Delta S _ {i} + \sum_ {k = 1} ^ {m} \psi_ {k} \frac {\partial C _ {k}}{\partial t} \Delta t \\ \qquad + \sum_ {i, j = 1} ^ {n} \sum_ {k = 1} ^ {m} \psi_ {k} \frac {\partial^ {2} C _ {k}}{\partial S _ {i} \partial S _ {j}} \Delta S _ {i} \Delta S _ {j} + \text {h.o.t.} \\ \qquad = \sum_ {i = 0} ^ {n} (\phi_ {i} + \sum_ {k = 1} ^ {m} \psi_ {k} \frac {\partial C _ {k}}{\partial S _ {i}}) \Delta S _ {i} + \sum_ {i, j = 1} ^ {n} \sum_ {k = 1} ^ {m} \psi_ {k} \frac {\partial^ {2} C _ {k}}{\partial S _ {i} \partial S _ {j}} (\Delta S _ {i} \Delta S _ {j} - \gamma_ {i, j} \Delta t) + \text {h.o.t.} \end{array}
$$

where again h. $\mathrm { _ { 0 . t . } } = O ( | \Delta t | ^ { 2 } , | \Delta t \Delta S _ { i } | , | \Delta S _ { i } | ^ { 3 } )$ . Let us compare this with the expansion of V from (7.12): 

$$
\Delta V (t) = \sum_ {i = 0} ^ {n} \frac {\partial V (t)}{\partial S _ {i}} \Delta S _ {i} + \frac {1}{2} \sum_ {i, j = 0} ^ {n} \frac {\partial^ {2} V (t)}{\partial S _ {i} \partial S _ {j}} \underbrace {(\Delta S _ {i} \Delta S _ {j} - \gamma_ {i , j} \Delta t)} _ {\neq 0} + \text { h.o.t. }
$$

If the portfolio process $( \phi _ { 0 } , \ldots , \phi _ { n } , \psi _ { 1 } , \ldots , \psi _ { m } )$ solves the equations 

$$
\sum_ {k = 1} ^ {n} \frac {\partial^ {2} C _ {k}}{\partial S _ {i} \partial S _ {j}} \cdot \psi_ {k} = \frac {\partial^ {2} V}{\partial S _ {i} \partial S _ {j}} \qquad i \leq j = 1, \ldots , n\tag{7.17}
$$

$$
\phi_ {i} + \sum_ {k = 1} ^ {n} \frac {\partial C _ {k}}{\partial S _ {i}} \cdot \psi_ {k} = \frac {\partial V}{\partial S _ {i}} \quad i = 1, \dots , n,\tag{7.18}
$$

then the residual risk is $\Delta V ( t ) - \Delta \Pi ( t ) = O ( | \Delta t | ^ { 2 } , | \Delta t \Delta S _ { i } | , | \Delta S _ { i } | ^ { 3 } )$ . To neutralize the gamma of a derivative product V it requires at most as many hedge derivatives $C _ { k } ,$ , as partial derivatives $\begin{array} { r } { \frac { \partial ^ { 2 } V } { \partial S _ { i } \partial S _ { i } } ~ i \le j = 0 , . . . , n } \end{array}$ (gamma) are non-zero. It requires at most $m = n \cdot ( n - 1 ) / 2$ additional derivative products. 

Remark 92 (linear product, static hedge): If a derivative product V is a linear function of the underlyings, then the delta hedge replicates the product globally. In this case, not only is a gamma hedge unnecessary (gamma and all higher order derivatives are zero), but neither is the dynamic adjustment of the replication portfolio is not required. In this case the hedge is called static and the derivative product is called linear product. 

## 7.4.3.1. Example: Time discrete delta-gamma hedge under a Black-Scholes model

We consider a Black-Scholes model with the notation as above. Let $C _ { 1 }$ denote an option with maturity $T ^ { * }$ and payof profile ma $\colon ( S ( T ^ { * } ) - K ^ { * } , 0 )$ . We aim to replicate an option V with maturity $T \ < \ T ^ { * }$ and payof profile max $( S ( T ) - K , 0 )$ . We allow trading at discrete times $0 = t _ { 0 } < t _ { 1 } < . . . .$ 

For the option to be replicated V we have 

$$
\begin{array}{r l} \Delta V (t _ {k}) = & \frac {\partial V (t _ {k})}{\partial t} \Delta t _ {k} + \frac {\partial V (t _ {k})}{\partial S} \Delta S (t _ {k}) + \frac {1}{2} \frac {\partial^ {2} V (t _ {k})}{\partial S ^ {2}} (\Delta S (t _ {k})) ^ {2} \\ & + O (| \Delta t _ {k} | ^ {2}, | \Delta t _ {k} \Delta S (t _ {k}) |, | \Delta S (t _ {k}) | ^ {3}). \end{array}
$$

For the replication portfolio Π we have 

$$
\begin{array}{l} \Delta \Pi (t _ {k}) = \phi_ {0} (t) \Delta N (t _ {k}) + \phi_ {1} (t _ {k}) \Delta S (t) + \psi_ {1} (t _ {k}) \Delta C (t _ {k}) \\ \qquad = \phi_ {0} (t) \Delta N (t _ {k}) + \phi_ {1} (t _ {k}) \Delta S (t) + \psi_ {1} (t _ {k}) \frac {\partial C (t _ {k})}{\partial t} \Delta t _ {k} \\ \qquad + \psi_ {1} (t _ {k}) \frac {\partial C (t _ {k})}{\partial S} \Delta S (t _ {k}) + \psi_ {1} (t _ {k}) \frac {1}{2} \frac {\partial^ {2} C (t _ {k})}{\partial S ^ {2}} (\Delta S (t _ {k})) ^ {2} \\ \qquad + O (| \Delta t _ {k} | ^ {2}, | \Delta t _ {k} \Delta S (t _ {k}) |, | \Delta S (t _ {k}) | ^ {3}) \end{array}
$$

For the replication portfolio $\Pi ( t ) = \phi _ { 0 } ( t ) N ( t ) + \phi _ { 1 } ( t ) S ( t ) + \psi _ { 1 } ( t ) C ( t )$ we find $\begin{array} { r } { \phi _ { 1 } ( t ) = \frac { \partial V ( t ) } { \partial S ( t ) } = } \end{array}$ $\begin{array} { r } { \Phi ( \frac { 1 } { \sigma \sqrt { T - t } } [ \log ( \frac { S ( t ) } { K } ) + r ( T - t ) + \frac { \sigma ^ { 2 } } { 2 } ] ) . } \end{array}$ 

We chose this to trade within the replication portfolio at discrete times $t _ { k } .$ . The size of the “cash position” is chosen such that the portfolio remains self-financing, i.e. 

$$
\phi_ {1} (t _ {k}) = \frac {\partial V (t _ {1})}{\partial S (t _ {1})} = N \left(\frac {1}{\sigma \sqrt {T - t _ {k}}} \left[ \log \left(\frac {S (t _ {k})}{K}\right) + r (T - t _ {k}) + \frac {\sigma^ {2}}{2} \right]\right)
$$

$$
\phi_ {0} (t _ {k}) = \frac {1}{N (t _ {k})} \big (\phi (t _ {k - 1}) N (t _ {k}) + \phi_ {1} (t _ {k - 1}) S (t _ {k}) - \phi_ {1} (t _ {k}) S (t _ {k}) \big)
$$

At time $t _ { 0 } = 0$ the portfolio is set up according to the option value known from the evaluation formula.<sup>8</sup> 

$$
\phi_ {0} (t _ {0}) = \frac {1}{N (t _ {k})} \bigl (V (t _ {0}) - \phi_ {1} (t _ {0}) S (t _ {0}) \bigr)
$$


Hedge Portfolio versus Payoff


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/e5b49a9609e2bc73f4587f30a104f783f670262f279d6be95a8f180c9fa89ee5.jpg)



Figure 7.3.: Samples of the value of the replication portfolio using monthly hedging: delta versus deltagamma hedge.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/866a5e204624dcfaa2ce425cd22db6741b38ed6dc680ea8958909ac1428df502.jpg)


Interpretation (role of the hold period ∆t): The delta hedge neutralizes the first order error in S , the delta-gamma hedge neutralizes the first and second order error in S . The residual error of the delta gamma hedge is of the order 

$$
O (| \Delta t | ^ {2}, | \Delta t \Delta S _ {i} |, | \Delta S _ {i} | ^ {3}).
$$

A question arises: 

• Why is the error in ∆t not considered? 

<sup>8</sup> Eventually the initial investment into the replication portfolio is not suficient, see Figure 7.1, right. 


Hedge Portfolio versus Payoff


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/37bafe17329773ed374cd858875d47433f6ff6b743c2705506eb12edfd0c9ec7.jpg)



Figure 7.4.: Samples of the value of the replication portfolio using weekly hedging with wrong interest rate.


First, the answer is given in the interpretation of the hedge-strategies: They aim to minimize the risk in the underlyings $S _ { i }$ , i.e. the dependence of $V ( t ) - \Pi ( t )$ on $S _ { i } ( t )$ . The interpretation is, that the length of the hold period ∆t is not known a priori. In our considerations we thus assume $\Delta t \to 0$ . Then the residual error is $O ( \Delta S _ { i } ^ { 2 } )$ for the delta hedge and $O ( \Delta S _ { i } ^ { 3 } )$ for the delta-gamma hedge. 

Furthermore: An error in $\Delta S _ { j }$ is stochastic, i.e. a risk. An error in ∆t is deterministic. If the hold period ∆t is known a priori, then the error in ∆t may be compensated for if the portfolio is not required to match the derivative value initially, i.e. $\Pi ( 0 ) = V ( 0 )$ . The derivative value $V ( 0 )$ corresponds to the replication portfolio for infinitesimal hold periods $\Delta t \to 0$ . We will consider a known hold period $\Delta t > 0$ in the following Section 7.5. C| 

## 7.4.4. Vega Hedging

As in the delta-gamma hedging, where in addition to a hedge of the option’s delta a hedge of the option’s gamma is considered, we may consider further dependencies of the pricing function. If the dependence on the log-volatility of the underlyings, i.e. $\textstyle { \frac { \partial V } { \partial \sigma _ { i } } }$ for $\mathrm { d } S _ { i } = \mu _ { i } S _ { i } \mathrm { d } t + \sigma _ { i } S _ { i } \mathrm { d } W _ { i }$ is neutralized, then this called vega hedging. 


Hedge Portfolio versus Payoff


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/09eb7d3807f49ebd656ae16e77fc8bdc1ab8d3eb455ce0097bdfccc92256bd73.jpg)



Figure 7.5.: Value of the replication portfolio without re-hedging. The replication portfolio is set up in t = 0 0 corresponding to a delta- or delta-gamma hedge and kept fixed until option maturity T (model and option parameter are as in Figure 7.1).


## 7.5. Hedging in Discrete Time: Minimizing the Residual Error (Bouchaud-Sornette Method)

The delta hedge transfers the optimal trading strategy for trading in continuous time to the timediscrete case, for which the strategy is not necessarily optimal. A more adequate calculation of a risk minimizing trading strategy may be derived from the residual risk: We look for a trading strategy that minimizes<sup>9</sup> the residual risk. This is the idea of the method of Bouchaud-Sornette [49]. Since for the time-discrete case the replication portfolio does not give an exact replication, we have yet to clarify in which sense a replication portfolio is optimal, i.e. in which norm the hedge error is measured. The optimal replication portfolio derived from this criterion is not necessarily identical with the replication portfolio of the delta hedge and depends on the norm that is used to measure the residual risk. 

At time T a payof profile $V ( T )$ has to be replicated as closely as possible by a replication portfolio $t \mapsto \Pi ( t ) | _ { t = T }$ . We consider the mean squared error, i.e. the variance of $V ( T ) - \Pi ( T )$ 

$$
\operatorname{Var} (V (T) - \Pi (T)).
$$

We also wish to minimize the variance in a conditional sense and repeat the required definitions and a lemma: 

## Definition 93 (Conditional Variance):

Let $C \subset { \mathcal { F } }$ denote two <sub>σ</sub> algebra and X an ${ \mathcal { F } } .$ -measurable random variable over a probability space $( \Omega , \mathbb { P } , \mathcal { F } )$ . Then 

$$
\operatorname{Var} (X | \mathcal {C}) := \operatorname{E} (X ^ {2} | \mathcal {C}) - (\operatorname{E} (X | \mathcal {C})) ^ {2}
$$

is the conditional variance of X under C. 

Remark 94 (Conditional Variance): The conditional variance is a C-measurable random variable. 

Lemma 95 (Conditional Variance): Let $C \subset { \mathcal { F } }$ denote two $\sigma$ algebras, X a $\mathcal { F }$ -measurable random variable and $Y \mathrm { ~ a ~ } C$ -measurable random variable over the probability space $( \Omega , \mathbb { P } , \mathcal { F } )$ . Then 

$$
\operatorname{Var} (X + Y | \mathcal {C}) = \operatorname{Var} (X | \mathcal {C})
$$

Proof: The proof is elementary. From $\operatorname { E } ( X \cdot Y | C ) = Y \cdot \operatorname { E } ( X | C )$ and $\mathrm { E } ( Y ^ { 2 } | C ) = Y ^ { 2 }$ we get 

$$
\begin{array}{l} \operatorname{Var} (X + Y | \mathcal {C}) \stackrel {{\text {Def.}}} {{=}} \operatorname{E} ((X + Y) ^ {2} | \mathcal {C}) - (\operatorname{E} (X + Y | \mathcal {C})) ^ {2} \\ = \operatorname{E} (X ^ {2} | \mathcal {C}) + 2 \cdot \operatorname{E} (X \cdot Y | \mathcal {C}) + \operatorname{E} (Y ^ {2} | \mathcal {C}) \\ \qquad - \operatorname{E} (X | \mathcal {C}) ^ {2} - 2 \cdot \operatorname{E} (X | \mathcal {C}) \cdot \operatorname{E} (Y | \mathcal {C}) - \operatorname{E} (Y | \mathcal {C}) ^ {2} \\ = \operatorname{E} (X ^ {2} | \mathcal {C}) + \underline {{2 \cdot Y}} \cdot \operatorname{E} (X | \mathcal {C}) + \overline {{Y}} ^ {2} - \operatorname{E} (X | \mathcal {C}) ^ {2} - \underline {{2 \cdot Y}} \cdot \operatorname{E} (X | \mathcal {C}) - \overline {{Y}} ^ {2} \\ = \operatorname{E} (X ^ {2} | \mathcal {C}) - \operatorname{E} (X | \mathcal {C}) ^ {2} = \operatorname{Var} (X | \mathcal {C}) \end{array}
$$

Let $0 = t _ { 0 } < t _ { 1 } < \ldots < t _ { m } = T$ denote a time discretization and $\phi ( t ) = \left( \phi _ { 0 } , \ldots , \phi _ { n } \right)$ a portfolio process $\begin{array} { r } { \Pi ( t ) = \phi ( t ) \cdot S \left( t \right) = \sum _ { i = 0 } ^ { n } \phi _ { i } ( t ) S _ { i } ( t ) } \end{array}$ , with piecewise constant φ<sub>i</sub>, i.e. we assume that trading takes place only at discrete times $( \phi _ { i } ( t ) = \phi _ { i } ( t _ { j } )$ fur¨ $t _ { j } \leq t < t _ { j + 1 } )$ 

## 7.5.1. Minimizing the Residual Error at Maturity $T$

Trading strategy: At time $t _ { k }$ the self-financing portfolio $\phi ( t _ { k } )$ is chosen such that the residual risk is minimized, i.e. 

$$
\operatorname{Var} (V (T) - \Pi (T) \mid \mathcal {F} _ {t _ {k}}) \rightarrow \min,
$$

where $\{ \mathcal { F } _ { t } \}$ denote the filtration generated by $S _ { \textrm { \tiny { \cdot } } }$ . 

To simplify notation let $S _ { 0 } : = P ( T )$ denote the bond with maturity $T .$ , i.e. the financial product that guarantees a payment of 1 at time $T , P ( T ) : t \mapsto P ( T ; t )$ with $P ( T ; T ) \equiv 1$ This product will later lay the foundation for the theory of interest rates, see Definition 97 in Chapter 8. It is not required that one of the products is the Bond with maturity T, but it simplifies the notation since 

$$
\operatorname{Var} (V (T) - \Pi (T)) = \operatorname{Var} \left(\frac {V (T)}{S _ {0} (T)} - \frac {\Pi (T)}{S _ {0} (T)}\right)
$$

and instead 

$$
\Pi (T) = \Pi (0) + \sum_ {l = 0} ^ {m - 1} \phi (t _ {l}) \cdot \Delta S (t _ {l})
$$

we may equivalently write 

$$
\begin{array}{c} \Pi (T) = \frac {\Pi (T)}{S _ {0} (T)} = \frac {\Pi (0)}{S _ {0} (0)} + \sum_ {l = 0} ^ {m - 1} \sum_ {i = 0} ^ {m - 1} \phi_ {i} (t _ {l}) \cdot \Delta \frac {S _ {i} (t _ {l})}{S _ {0} (t _ {l})} \\ = \frac {\Pi (0)}{S _ {0} (0)} + \sum_ {l = 0} ^ {m - 1} \sum_ {i = 1} ^ {m - 1} \phi_ {i} (t _ {l}) \cdot \Delta \frac {S _ {i} (t _ {l})}{S _ {0} (t _ {l})} \end{array}
$$

– note that $\phi _ { 0 }$ does not enter in the last sum. Thus $\phi _ { 0 }$ may be chosen such that the condition of self-financing is fulfilled and $\phi _ { i } , i \geq 1$ determines the “optimal hedge”. 

With the notation $\begin{array} { r } { \tilde { S } = \frac { S } { S _ { 0 } } } \end{array}$ we have 

$$
\begin{array}{c} V (T) - \Pi (T) = V (T) - \Pi (0) - \sum_ {l = 0} ^ {m - 1} \phi (t _ {l}) \cdot \Delta \tilde {S} (t _ {l}) \\ = V (T) - \Pi (0) - \sum_ {l = 0} ^ {k - 1} \phi (t _ {l}) \cdot \Delta \tilde {S} (t _ {l}) \\ - \sum_ {l = k + 1} ^ {m - 1} \phi (t _ {l}) \cdot \Delta \tilde {S} (t _ {l}) - \phi (t _ {k}) \cdot \Delta \tilde {S} (t _ {k}) \end{array}
$$

and with Lemma 95 

$$
\begin{array}{l} \operatorname{Var} (V (T) - \Pi (T) | \mathcal {F} _ {t _ {k}}) \\ = \operatorname{Var} (V (T) - \sum_ {l = k + 1} ^ {m - 1} \phi (t _ {l}) \cdot \Delta \tilde {S} (t _ {l}) | \mathcal {F} _ {t _ {k}}) - \phi (t _ {k}) \cdot \Delta \tilde {S} (t _ {k}) \\ = \operatorname{Var} (V (T) - \sum_ {l = k + 1} ^ {m - 1} \phi (t _ {l}) \cdot \Delta \tilde {S} (t _ {l}) | \mathcal {F} _ {t _ {k}} - \phi (t _ {k}) \cdot \Delta \tilde {S} (t _ {k}) | \mathcal {F} _ {t _ {k}}) \\ = \operatorname{Var} (V (T) - \sum_ {l = k + 1} ^ {m - 1} \phi (t _ {l}) \cdot \Delta \tilde {S} (t _ {l}) | \mathcal {F} _ {t _ {k}} | \mathcal {F} _ {t _ {k}}) \\ - 2 \cdot \operatorname{Cov} (V (T) - \sum_ {l = k + 1} ^ {m - 1} \phi (t _ {l}) \cdot \Delta \tilde {S} (t _ {l}), \phi (t _ {k}) \cdot \Delta \tilde {S} (t _ {k}) | \mathcal {F} _ {t _ {k}}) \\ + \operatorname{Var} (\phi (t _ {k}) \cdot \Delta \tilde {S} (t _ {k}) | \mathcal {F} _ {t _ {k}}). \end{array}
$$

Finally we ge from 

$$
\frac {1}{2} \frac {\partial}{\partial \phi (t _ {k})} \mathrm{Var} (V (T) - \Pi (T) | \mathcal {F} _ {t _ {k}}) = 0
$$

the equation for $\phi ( t _ { k } )$ 

$$
\begin{array}{l} \phi (t _ {k}) \cdot \mathrm{Cov} (\Delta \tilde {S} (t _ {k}), \Delta \tilde {S} (t _ {k}) | \mathcal {F} _ {t _ {k}}) \cdot \phi (t _ {k}) ^ {T} \\ - \mathrm{Cov} (V (T) - \sum_ {l = k + 1} ^ {m - 1} \phi (t _ {l}) \cdot \Delta \tilde {S} (t _ {l}), \Delta \tilde {S} (t _ {k}) | \mathcal {F} _ {t _ {k}}) = 0. \end{array}\tag{7.19}
$$

## 7.5.2. Minimizing the Residual Error in each Time Step

The strategy described in the previous Section 7.5.1 focusses at each time $t _ { k }$ on the minimization of the residual risk at maturity T. An alternative trading strategy is to require at each time $t _ { k }$ that the residual risk at time $t _ { k + 1 }$ is minimized by the choice of the portfolio $\phi ( t _ { k } )$ 

$$
\operatorname{Var} (V (t _ {k + 1}) - \Pi (t _ {k + 1}) \mid \mathcal {F} _ {t _ {k}}) \rightarrow \min.
$$

Obviously (consider the last time step $k = m - 1$ in (7.19)) the equation for $\phi ( t _ { k } )$ then follows as 

$$
\phi (t _ {k}) \cdot \mathrm{Cov} (\Delta \tilde {S} (t _ {k}), \Delta \tilde {S} (t _ {k}) | \mathcal {F} _ {t _ {k}}) \cdot \phi (t _ {k}) ^ {T} - \mathrm{Cov} \bigl (V (t _ {k + 1}), \Delta \tilde {S} (t _ {k}) | \mathcal {F} _ {t _ {k}} \bigr) = 0.
$$

Remark 96 (Measure): The measure under which the minimization, and thus the covariance in (7.19), has to be considered is the real measure P. A consideration under a martingale measure essentially corresponds to a measuring of the risk under a diferent norm. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/e59b2853eceba8e8429f836eca9553709d14c1a2c54191014a1baaf127061c30.jpg)


Experiment: At http://www.christian-fries.de/finmath/ applets/HedgeSimulator.html a hedge simulator can be found. There, in a Monte-Carlo simulation, paths $t \mapsto ( N ( t , \omega ) , S ( t , \omega ) )$ are generated corresponding to a given model. Along each path a self-financing trading strategy is applied to a replication portfolio. At maturity T the value of the replication portfolio is compared to the option value $V ( T )$ . It is possible to choose the model parameters assumed in the construction of the replication portfolio independent from the model parameters, which determine the evolution of the market. A mismatch in the parameters results in an increased residual risk (see Figure 7.1). C| 

Part III. 

Interest Rate Structures, Interest Rate Products and Analytic Pricing Formulas 

## Motivation and Overview - Part III

Part III will consider the interest rate structures and the analytical pricing of interest rate derivatives. The methods for pricing financial products may roughly be classified into three groups. These are 

• Model-independent analytic pricing: The financial product can be separated into a portfolio of traded assets. The value of the derivative product is then given by the value of the portfolio. The portfolio represents a replication portfolio, i.e. a static hedge. 

• Model-dependent analytic pricing: The replication of the financial product requires dynamic hedging, i.e. a continuous adjustment of the portfolio, and thus requires a model for the underlying stochastics. The value of the replication portfolio depends on the model. However, the product and the choosen model is simple enough to derive an analytic pricing formula. 

• Model-dependent numeric pricing: The replication of the financial product requires dynamic hedging and thus requires a model for the underlying stochastics. The value of the replication portfolio depends on the model. The complexity of the product or of the model requires a numerical calculation of the price. 

In Chapter 8 we will define some elementary products and interest rates. In Section 9.1 simple interest rate products will be presented which allow model-independent analytic pricing. Here, the corresponding pricing is discussed right after the definition of the product. In Section 9.2 we define some simple options. In Chapter 10 and 11 we will show how to derive some analytic pricing formulas using some simple standard models. In Chapter 12 more exotic options will be presented, for which pricing requires generally numerical methods. 

Numerical pricing methods and complex pricing models will be considered in Part IV and V. 

# Interest Rate Structures

## 8.1. Introduction

In previous sections we have considered a one-dimensional stochastic process as the underlying, representing a stock for example. We will now turn to the modeling of interest rates and later the pricing of interest rate derivatives. Interest rates potentially ofer a richer structure than a single stock, since at each time t we have to consider an interest rate curve $F ( T ; t ) , T \geq t$ instead of a scalar stock price $S ( t )$ 

Let $F ( T ; t )$ denote the interest earned on an investment made over the period $[ t , T ] .$ , if the contract is written at the beginning t of the period, i.e. we assume that $N \cdot ( 1 + F ( T ; t ) \cdot ( T - t ) )$ is the amount one receives at time T, if one invests the amount N at time t, and the contract is fixed at the beginning of the period, i.e. in $t . ^ { 1 }$ For diferent times $T _ { 1 } < T _ { 2 }$ two such interest rates $F ( T _ { 1 } ; t )$ and $F ( T _ { 2 } ; t )$ ) may be diferent, the reason being the diferent interest earned on the two sub-periods $[ t , T _ { 1 } ]$ and $[ T _ { 1 } , T _ { 2 } ]$ , e.g. if interest rates are expected to rise or fall in future. Thus, if one decomposes the time-axis into small interest rate periods $[ T _ { i } , T _ { i + 1 } ]$ and defines 

$$
(1 + F (T _ {k}; t) (T _ {k} - t)) =: (1 + L (T _ {0}, T _ {1}; t) (T _ {1} - T _ {0})) \cdot \dots \cdot (1 + L (T _ {k - 1}, T _ {k}; t) (T _ {k} - T _ {k - 1})),\tag{8.1}
$$

then it is rational to represent each interest rate $L ( T _ { i } , T _ { i + 1 } ; t )$ by its own stochastic process. Here we assume $T _ { 0 } = t$ and $L ( T _ { i } , T _ { i + 1 } ; t )$ denotes the interest rate earned over the period $[ T _ { i } , T _ { i + 1 } ]$ as given by a contract which is fixed in $t . ^ { 2 }$ See Figure 8.1. It is common to have interest rate derivatives that depend on more than one interest rate and in this sense depend on the movement of the whole curve. 

## 8.1.1. Fixing Times and Tenor Times

If the interest rates $F ( T _ { i } ; t )$ for periods $[ t , T _ { i } ]$ for $i = 1 , \ldots , k$ are known, then we can derive from Equation (8.1) the rates for the sub-periods $[ T _ { i - 1 } , T _ { i } ]$ . It is 

$$
L (T _ {i - 1}, T _ {i}; t) = \frac {1}{T _ {i} - T _ {i - 1}} \left(\frac {1 + F (T _ {i} ; t) (T _ {i} - t)}{1 + F (T _ {i - 1} ; t) (T _ {i - 1} - t)} - 1\right).\tag{8.2}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/bdef8a0a075e2ca6be9e8ff97e0fc4366840b46b67ec8793453caa2653960e3b.jpg)



Figure 8.1.: Modeling an interest rate curve by a family of stochastic processes.


The rate $L ( T _ { i - 1 } , T _ { i } ; t )$ is the interest rate for the future period $T _ { i - 1 } , T _ { i }$ , that has been derived from the interest rate curve as of time t. The interest rate has been fixed at time t, i.e. the stochastic process is evaluated in t. The time t is the simulation time of the stochastic process, it thus determines that the random variable $L ( T _ { i - 1 } , T _ { i } ; t )$ has to be (at least) F-measurable. The times $T _ { i }$ mark the start and the end of the periods. The period structure $\{ T _ { 0 } , T _ { 1 } , \ldots , T _ { k } \}$ is also called the tenor structure. 

## 8.2. Definitions

All of the following random variables and stochastic processes are assumed to be defined over the same probability space $( \Omega , { \mathcal { F } } , { \mathbb { P } } )$ . As the building block of all interest rates we define the Bond: 

## Definition ${ \bf 9 7 } \ : ( { \bf B o n d } ^ { 3 } )$ :

Assume that a guaranteed payment of a unit currency<sup>4</sup> 1 in time $T _ { 2 }$ is a traded product at any earlier time $t < T _ { 2 }$ and its value in state $\omega \in \Omega$ is uniquely determined by $( t , \omega )$ . The value of this product is called the price of the $T _ { 2 }$ bond as seen in $( t , \omega )$ and will be denoted by $P ( T _ { 2 } ; t , \omega )$ . It defines a stochastic process on $[ 0 , T _ { 2 } ]$ which we denote by $P ( T _ { 2 } )$ 

$$
P (T _ {2}): [ 0, T _ {2} ] \times \Omega \mapsto \mathbb {R}.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/fb71a5dcab67deb41270ed10ee935ef487cfd15d0cfc2233111660da5e03c113.jpg)


Interpretation: The value of the bond $P ( T _ { 2 } ; t , \omega )$ is the amount we have to invest at a given time t and a given state to receive 1 in $T _ { 2 }$ . Thus for a (riskless) investment of 1 at time t we get a guaranteed payment of $1 / P ( T _ { 2 } ; t , \omega )$ at time $T _ { 2 } ,$ , because we simply buy $1 / P ( T _ { 2 } ; t , \omega )$ times the bond. Note that we assume 

that all products may be traded in arbitrary fractions and that the price is unique, the same for selling and buying. Thus $P ( T _ { 2 } ; t , \omega )$ not only implies the interest earned on an investment, it also implies the interest to be paid for a corresponding credit. C| 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/6caf0940cf8d883887c6b5ab0bed831dbb7c4142e77d8b9e9ace156a01f025bf.jpg)



Figure 8.2.: Cash-flowfor aforward bond.


Definition 98 (Forward Bond): 

Let $0 \leq T _ { 1 } \leq T _ { 2 } < \infty$ . Asforward bond we denote the stochastic process 

$$
P (T _ {1}, T _ {2}) := \frac {P (T _ {2})}{P (T _ {1})},
$$

defined on $[ 0 , T _ { 1 } ]$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/ccfa347d6c03e4c074cd1a6aa876006dcd31e4352db93c6e1e01a074a45f2e71.jpg)


Interpretation: Theforward bond $P ( T _ { 1 } , T _ { 2 } ; t )$ corresponds to the amount that has to be invested at time $T _ { 1 }$ to receive a guaranteed payment of 1 in $T _ { 2 } ,$ , if that contract is finalized at time t in state $\omega .$ To receive 1 in $T _ { 2 }$ one has to invest $P ( T _ { 2 } ; t )$ in t. This investment is financed by borrowing until $T _ { 1 }$ , i.e. we borrow )-times the value of a -times the value of a $P ( T _ { 1 } )$ bond (compare Figure 8.2) 

$P ( T _ { 2 } ; t ) \cdot 1 / P ( T _ { 1 } ; t )$ bond (compare Figure 8.2). 

It is important to understand that $P ( T _ { 1 } , T _ { 2 } ; t )$ is not the value of a forward bond at time t. The value of that contract is simply 0. What is denoted by $P ( T _ { 1 } , T _ { 2 } ; t )$ is the amount that has to be paid in $T _ { 1 }$ as part of a contract written in t. The subject of the contract is a bond which liesforward in time. 

Obviously we have $P ( T _ { 2 } ; t ) = P ( t , T _ { 2 } ; t )$ 

C| 

Often the bond (or forward bond) will be represented by a rate (or forward rate). However, the interest rate that corresponds to a bond depends on how we think of interest earned, e.g. if compounding, i.e. interest paid on interest received, is considered. Thus, there are many different definitions of interest rates. For that reason we see an interest rate as a derived quantity. We define some interest rates: 

## Definition 99 (Forward Rate ((Forward) LIBOR)):

Let $T _ { 1 } < T _ { 2 }$ . The (forward) LIBOR<sup>5</sup> $L ( T _ { 1 } , T _ { 2 } )$ is defined by 

$$
\begin{array}{c} \frac {P (T _ {1})}{P (T _ {2})} = \frac {1}{P (T _ {1} , T _ {2})} =: (1 + L (T _ {1}, T _ {2}) \cdot (T _ {2} - T _ {1})) \quad , \text { i.e. } \\ L (T _ {1}, T _ {2}) := \frac {1}{T _ {2} - T _ {1}} \cdot \frac {P (T _ {1}) - P (T _ {2})}{P (T _ {2})}. \end{array}
$$

## Definition 100 ((continuously compounded) Yield):

Let $T _ { 1 } < T _ { 2 }$ . The (continuously compounded) (forward) yield $r ( T _ { 1 } , T _ { 2 } )$ is defined by 

$$
\begin{array}{l} \frac {P (T _ {1})}{P (T _ {2})} = \frac {1}{P (T _ {1} , T _ {2})} =: \exp (r (T _ {1}, T _ {2}) \cdot (T _ {2} - T _ {1})) \quad , \text {i.e.} \\ r (T _ {1}, T _ {2}) := \frac {- \log (P (T _ {1} , T _ {2}))}{(T _ {2} - T _ {1})} = - \frac {\log (P (T _ {2})) - \log (P (T _ {1}))}{(T _ {2} - T _ {1})}. \end{array}
$$

## Definition 101 (Instantaneous Forward Rate):

The instantaneousforward rate is defined by 

$$
f (t, T) := \lim _ {T _ {2} \searrow T} L (T, T _ {2}; t).
$$

It may be interpreted as the interest rate for the infinitesimal period $[ T , T + \mathrm { d } T ]$ 

Remark 102 (Instantaneous Forward Rate): We have 

$$
\begin{array}{c} f (t, T) = \lim _ {T _ {2} \searrow T} L (T, T _ {2}; t) = \lim _ {T _ {2} \searrow T} \frac {1}{P (T _ {2} ; t)} \frac {P (T ; t) - P (T _ {2} ; t)}{T _ {2} - T} \\ = - \frac {1}{P (T ; t)} \frac {\partial P (T ; t)}{\partial T} = - \frac {\partial \log (P (T ; t))}{\partial T}. \end{array}
$$

## Definition 103 (Short rate):

Let $t \geq 0$ . The short rate r(t) is defined by 

$$
\begin{array}{c} r (t) := \lim _ {T \searrow t} r (t, T; t) = \frac {\partial}{\partial T} - \log (P (T; t)) \Big | _ {T = t} \\ = \frac {- \frac {\partial P (T ; t)}{\partial T}}{P (T ; t)} \Big | _ {T = t} = - \frac {\partial P (T ; t)}{\partial T} \Big | _ {T = t}. \end{array}
$$

Remark 104 (Short rate): Note that in Definitions 99, 100 and 101 we define families of stochastic processes, while the short rate from Definition 103 is a single, scalar stochastic process. 

The short rate is a limit of the spotforward rate (LIBOR) and the yield. We have 

$$
r (t) = \lim _ {T \searrow t} r (t, T; t) = \lim _ {T \searrow t} L (t, T; t).
$$

This short rate is the interest rate for the infinitesimal period $[ t , t + \mathrm { d } t ]$ , as seen in t. 

Remark 105 (Forward forward): The term “forward” is used ambiguously: In Definition 99 and 100 we define stochastic processes for interest rates, i.e. for a given observation time t we define $L ( T _ { 1 } , T _ { 2 } ; t )$ and $r ( T _ { 1 } , T _ { 2 } ; t$ ) as rates for the period $[ T _ { 1 } , T _ { 2 } ]$ as seen in t. If $T _ { 1 } > t ,$ then these rates are called “forward” (i.e.forward LIBOR,forward Yield), since the rate is associated with a future period, lying forward in time. If $T _ { 1 } = t$ we would use the attribute “spot” instead. 

However, on the other hand, the rate $L ( T _ { 1 } , T _ { 2 } ; T _ { 1 } )$ (note $t = T _ { 1 } )$ is often denoted as forward rate, since it is an interest rate for an interval up to $T _ { 2 }$ . This is in contrast to the short rate, which is defined for an infinitesimal period. Being precise, terms like “forward forward rate” should be used. 

There is a similar ambiguity for volatilities. The term forward volatility may be interpreted as the volatility of a forward rate or as a volatility of some process considered at a future period in time. 

Remark 106 (Interest Rate Models): The various definitions of interest rates (as stochastic processes) are the starting point for the corresponding interest rate modeling. The corresponding models are 

<table><tr><td>Interest Rate</td><td>Model</td></tr><tr><td>Forward Rate L</td><td>LIBOR Market Model → Chapter 19.1</td></tr><tr><td>Instantaneous Forward Rate f</td><td>HJM Framework → Chapter 21</td></tr><tr><td>Short Rate r</td><td>Short Rate Models → Chapter 22</td></tr></table>


Table 8.1.: Interest Rate Models.


Although the models above do not model the bond prices directly, we view zero-bond prices as the basic building blocks. 

Remark 107 (Bond prices as a function of interest rates): The bond prices may be calculated from the interest rates. We have 

$$
\begin{array}{l} P (T; t) = \exp (- r (t, T; t) (T - t)) \\ P (T; t) = \exp (- \int_ {t} ^ {T} f (t, \tau) \mathrm{d} \tau) \\ P (T; t) = \prod_ {i = 0} ^ {n - 1} (1 + L (T _ {i}, T _ {i + 1}; t) (T _ {i + 1} - T _ {i})) ^ {- 1} \quad \text { for } t = T _ {0} <   T _ {1} <   \ldots <   T _ {n} = T \end{array}
$$

The short rate is an exception. Here the reconstruction of the bond prices is possible only if the short rate process is known under the equivalent martingale measure $\mathbb { Q } ^ { N }$ corresponding to the numeraire´ $\begin{array} { r } { N ( t ) : = \exp ( \int _ { 0 } ^ { t } r ( \tau ) } \end{array}$ d<sub>τ</sub>). Then we have 

$$
P (T; t) = \mathrm{E} ^ {\mathbb {Q} ^ {N}} \big (\exp (- \int_ {t} ^ {T} r (\tau) \mathrm{d} \tau) | \mathcal {F} _ {t} \big)
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/9996500a4d5fb4595ca49c2db2d4a2f4cab33dfd3d0663a63c10bf9ab0936dec.jpg)


Tip (Discount factors as a basic market data object): We consider the price of zero bonds as given and view interest rates as derived quantities. It is natural to take this view in the implementation as well. If we want to provide information on market interest rates through a Class<sup>6</sup>, then we store internally 

a discretization of the Bond price curve $j \mapsto P ( T _ { j } ; 0 )$ (also called discount factors). The class then provides the various interest rates under various conventions through methods. This design reduces the errors of misinterpretation of the stored data (especially if more than one developer works on the class), since the data stored is free of market conventions and the convention used to calculate the rates is explicit in the implementation of the corresponding method. This also reduces the documentation overhead for the data model. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/e6f3e595d69d827c9bd3b043fb5e83cd4d78084227dba02edeac337218569685.jpg)



Figure 8.3.: UML diagram: The class DiscountFactors internally stores discount factors and provides various interest rates through corresponding methods.


A problem of this design is that discount factors are usually not the quantities that are observable in the interest rate market. The market quotes the prices of various diferent interest rate products (e.g. futures or swaps), from which discount factors have to be calculated. This calculation is called bootstrapping. Under some conditions, it might be useful to store the original market data. One such application is the numerical calculation of partial derivatives with respect to a change in these input prices.<sup>7</sup> C| 

## 8.3. Interest Rate Curve Bootstrapping

Since bootstrapping of discount factors from market prices involves the inversion of a pricing formula, we have to discuss the interest rate products and their pricing. We will do so in Chapter 9, but give an anticipatory abstract description of the bootstrap algorithm here: 

Let $0 = T _ { 0 } < T _ { 1 } < T _ { 2 } < . .$ denote a time discretization. For given discount factors $d f _ { j } =$ $P ( T _ { j } ; 0 ) , j = 0 , 1 , \ldots , i$ we assume the existence of an interpolation function $d f ( d f _ { 0 } , \ldots , d f _ { i } ; t ) .$ 

having the property that an additional sample point beyond $T _ { i }$ will not change the interpolation in $t \leq T _ { i } , \mathrm { i . e }$ 

$$
d f (d f _ {0}, \dots , d f _ {i}; t) = d f (d f _ {0}, \dots , d f _ {i}, d f _ {i + 1}; t) \quad \forall t \leq T _ {i} \quad \forall i = 1, 2, 3, \dots .
$$

Let $V _ { i } ^ { \mathrm { m a r k e t } }$ denote given market prices of interest rate products for which the price may be expressed as a function $V _ { i }$ of the discount factors in $t \leq T _ { i }$ , i.e. 

$$
V _ {i} = V _ {i} (\{d f (t) \mid t \leq T _ {i} \}).
$$

We further assume that the discount factor $d f ( T _ { i } )$ enters into the pricing, i.e. let $\begin{array} { r } { \frac { \partial } { \partial d f ( T _ { i } ) } V _ { i } \neq 0 } \end{array}$ Then the bootstrap algorithm is given by: 

Induction start $( T _ { 0 } ) \colon$ 

$$
\bullet d f _ {0} := d f (T _ {0}) = P (T _ {0}; 0) = P (0; 0) = 1. 0;
$$

Induction step $( T _ { i - 1 } \to T _ { i } ) \colon$ 

• Calculate $d f _ { i } : = d f ( T _ { i } )$ such that, using the discount factor interpolation, we have 

$$
V _ {i} (\{d f (d f _ {0}, \dots , d f _ {i}; t) \mid t \leq T _ {i} \}) \stackrel {!} {=} V _ {i} ^ {\text { market }}.\tag{8.3}
$$

In some cases the Equation (8.3) may be directly solved for $d f _ { i } ,$ especially if it does not depend on the interpolation method used. Normally, a numerical solution is possible (see Appendix $\mathbf { A . } 5 )$ 8 

## 8.4. Interpolation of Interest Rate Curves

We consider, as before, a family of bond prices $T \mapsto P ( T ; 0 )$ , i.e. the discount factor curve, as the basic representation of the interest rate curve. If the prices $d f _ { i } : = P ( T _ { i } ; 0 )$ are known for times $0 = T _ { 0 } < T _ { 1 } < T _ { 2 } < . . .$ , we seek a meaningful interpolation method to calculate interest rates for sub-periods. The interpolation method should fulfill two basic requirements: 

• The interpolation method should be suficiently smooth, at least continuously diferentiable. This is desirable, because the calculation of an interest rate corresponds to a finite diference, i.e. converges to a derivative for decreasing period lengths. 

• The interpolation method should preserve the monotonicity of discount factors, i.e. if we have monotone decreasing sample points then the interpolation should be a monotone decreasing curve. 

The following additional requirement is also desirable: 

• If the sample points correspond to a set of constant rates, then their interpolation should give constant rates. In other words: The interpolation of sample points from a flat interest rate curve should be flat (where flat means flat with respect to a rate). 

<sup>8</sup> If interest rates are positive, a simple interval bisection like the Golden Section Search works, since $d f _ { i } \in [ 0 , d f _ { i - 1 } ]$ 

The linear interpolation of bond prices fulfills the second, but neither the first, nor the third requirement. The linear interpolation of forward rates fulfills the first and third requirement, but not necessarily the second. A simple interpolation method, which is also popular in practice, is the linear interpolation of the logarithm of the discount factors, i.e. the linear interpolation of $r ( 0 , T _ { j } ) \cdot T _ { j } \mathrm { . }$ 

$$
d f (t) = \exp \left(\frac {T _ {j + 1} - t}{T _ {j + 1} - T _ {j}} \cdot \log \left(d f \left(T _ {j}\right)\right) + \frac {t - T _ {j}}{T _ {j + 1} - T _ {j}} \cdot \log \left(d f \left(T _ {j + 1}\right)\right)\right).
$$

This interpolation fulfills the second and the third requirement. 

A more complete discussion of various interpolation methods for interest rate curves may be found in [72]. 

## 8.5. Implementation

We extend the design of the DiscountFactors class of Figure 8.3 by an interpolation algorithm and a bootstrap algorithm. 

If the interpolation method is realized as part of the getDiscountFactor() method, and if the methods which calculate interest rates from discount factors (like getForwardRate() or getYield()) only use getDiscountFactor() (and not the internal data model), then the interpolation method is available in all derived interest rates once it has been implemented in getDiscountFactor().<sup>9</sup> 

The bootstrapper is then realized through one additional method appendDiscountFactor(ProductSpecification productSpec, double marketPrice), where productSpec contains the description of the financial product for which an additional discount factor has to be calculated from the given market price marketPrice. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/95e6811d99b1707107f47c5f9eddb8e3ebe8aaeec016c2bbb87c9b1476f207c2.jpg)



Figure 8.4.: UML Diagram: The class DiscountFactors internally stores discount factors and provides various interest rates through corresponding methods. The method appendDiscountFactor(ProductSpecification productSpec, double marketPrice) implements one induction step ofa bootstrap algorithm.


<sup>9</sup> This is one reason for encapsulation of the internal data model, which should only be accessible to a small set of methods (even within the same class!). 

# Simple Interest Rate Products

So far we have defined a single interest rate product, the zero coupon bond $P ( T )$ . In the following, we give the definitions of some basic interest rate products. Many definitions use Definition 99 of the forward rate (which, of course, is based on the definition of the zero bond). 

## 9.1. Interest Rate Products Part 1: Products without Optionality

## 9.1.1. Fix, Floating and Swap

We define a trivial generalization of the zero bond: 

Definition 108 (Coupon Bond): 

$\mathbf { A }$ coupon bond with coupon $C _ { i } , i = 1 , \dots , n - 1$ and tenor structure $T _ { i } , i = 1 , \ldots$ n and maturity $T _ { n }$ pays 

$$
C _ {i} \cdot (T _ {i + 1} - T _ {i}) + \left\{ \begin{array}{l l} 0 & \text { if } i + 1 <   n \\ 1 & \text { if } i + 1 = n \end{array} \right. \quad \text { in } T _ {i + 1}
$$

(n − 1 payments). 

Theorem 109 (Value of a Coupon Bond): The Coupon Bond consists of $n - 1$ guaranteed payments with diferent payment dates. Clearly, the value of the coupon bond as seen in $t < T _ { 2 }$ is given by 

$$
\sum_ {i = 1} ^ {n - 1} C _ {i} \cdot (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t) + P (T _ {n}; t).\tag{9.1}
$$

Remark 110 (Dirty Price, Clean Price, Accrued Interest): The value of a coupon bond as given by Equation (9.1) is called dirty price. The dirty price is sometimes split into two parts, called the Clean Price and Accrued Interest. 

If $T _ { 1 } < t < T _ { 2 }$ , i.e. the bond is evaluated within the first interest rate period, then the accrued interest is defined by 

$$
A (T _ {1}, T _ {2}; t) := \frac {t - T _ {1}}{T _ {2} - T _ {1}} \cdot C _ {1} \cdot (T _ {2} - T _ {1}).
$$

Remember that in Definition 109 it is assumed that $t ~ < ~ T _ { 2 } . ~ A ( T _ { 1 } , T _ { 2 } ; t )$ is called accrued interest. Dirty price and clean price are now related through 

$$
\begin{array}{l} P _ {\text {Dirty}} (t) = \sum_ {i = 1} ^ {n - 1} C _ {i} \cdot (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t) + P (T _ {n}; t), \\ P _ {\text {Clean}} (t) = P _ {\text {Dirty}} (t) - A (T _ {1}, T _ {2}; t). \end{array}
$$

The accrued interest represents the fraction of the future coupon payment that relates to the past fraction of the period. This stems from the interpretation of the coupon payment as equally distributed. The price of a bond is often quoted only by its Clean Price. 

The decomposition in clean price and accrued interest may appear useless, since upon trading their sum, i.e. the dirty price, has to be paid. However, quoting the clean price has an advantage: The clean price evolves continuously in t across period end dates, while the dirty price exhibits a jump at the end of a period, due to the paid coupon. 

The zero bond $P ( T _ { 1 } ; t )$ is the time t value of a guaranteed payment of 1 in $T _ { 1 }$ . It thus represents a fixed interest rate payment. A product with variable interest rate payments is the floater. 

## Definition 111 (Floater):

Let $T _ { i } , i = 1 , \ldots , n$ denote a given time discretization (a tenor structure). A floater pays 

$$
N \cdot L (T _ {i}, T _ {i + 1}; T _ {i}) \cdot (T _ {i + 1} - T _ {i}) \quad \text { in } T _ {i + 1}
$$

for $i = 1 , \ldots , n - 1 ( n - 1$ payments). 

Theorem 112 (Value of a Floater): At time $t \leq T _ { 1 }$ the value of a floater (as in Definition 111) is given by 

$$
\begin{array}{l} V _ {\text { Floater }} (t) = N \cdot \sum_ {i = 1} ^ {n - 1} L (T _ {i}, T _ {i + 1}; t) \cdot (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t) \\ = N \cdot (P (T _ {1}) - P (T _ {n})). \end{array}
$$

Proof: Variant 1 of the proof : From the definition of the forward rate we have for a single payment of the floater in time $T _ { i + 1 }$ 

$$
V _ {\text { Floater }} ^ {i} (T _ {i + 1}) := N \cdot L (T _ {i}, T _ {i + 1}; T _ {i}) \cdot (T _ {i + 1} - T _ {i}) \stackrel {{\text { Def. } L}} {{=}} N \cdot \frac {P (T _ {i} ; T _ {i}) - P (T _ {i + 1} ; T _ {i})}{P (T _ {i + 1} ; T _ {i})}.
$$

This payment is a $\mathcal { F } _ { T _ { i } }$ -measurable random variable. The interest rate of $V _ { \mathrm { F l o a t e r } } ^ { i }$ was fixed in $T _ { i }$ and is no longer stochastic when observed on $[ T _ { i } , T _ { i + 1 } ]$ . As seen in $T _ { i }$ the value of this payment is thus a multiple of $P ( T _ { i + 1 } ; T _ { i } )$ , namely 

$$
V _ {\mathrm{Floater}} ^ {i} (T _ {i}) = V _ {\mathrm{Floater}} ^ {i} (T _ {i + 1}) \cdot P (T _ {i + 1}; T _ {i}) = N \cdot (P (T _ {i}; T _ {i}) - P (T _ {i + 1}; T _ {i})).
$$

Thus we see that the time $T _ { i }$ value of the floater is given by a portfolio of bonds. The time t value of this portfolio is known. Thus we have 

$$
V _ {\mathrm{Floater}} ^ {i} (t) = N \cdot (P (T _ {i}; t) - P (T _ {i + 1}; t)) = N \cdot L (T _ {i}, T _ {i + 1}; t) \cdot (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t).
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/775564ad593f81c820e3bab0b8b212334a399c9e3e1a70f84e2c63ea2fbf3f53.jpg)



Figure 9.1.: Cash-flow ofafloater with exchange ofnotional N.


This is the value of a single floater payment. The claim follows by summation over i. 

Variant 2 ofthe proof: We have to value $V _ { \mathrm { F l o a t e r } } ^ { i } ( T _ { i + 1 } )$ . Choose $N ( t ) = P ( T _ { i + 1 } ; t )$ as numeraire´ and let $\mathbb { Q } ^ { N }$ denote a corresponding martingale measure. Then $N ( T _ { i + 1 } ) = 1$ and 

$$
\begin{array}{l} V _ {\text {Floater}} ^ {i} (t) = N (t) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {V _ {\text {Floater}} ^ {i} (T _ {i + 1})}{N (T _ {i + 1})} | \mathcal {F} _ {t}) = N (t) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} (V _ {\text {Floater}} ^ {i} (T _ {i + 1}) | \mathcal {F} _ {t}) \\ \qquad = N (t) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} (N \cdot \frac {P (T _ {i} ; T _ {i}) - P (T _ {i + 1} ; T _ {i})}{P (T _ {i + 1} ; T _ {i})} | \mathcal {F} _ {t}) \\ \qquad = N (t) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} (N \cdot \frac {P (T _ {i} ; T _ {i}) - P (T _ {i + 1} ; T _ {i})}{N (T _ {i})} | \mathcal {F} _ {t}) \\ \qquad = N (t) \cdot N \cdot \frac {P (T _ {i} ; t) - P (T _ {i + 1} ; t)}{N (t)} \\ \qquad = N \cdot (P (T _ {i}; t) - P (T _ {i + 1}; t)) = N \cdot L (T _ {i}, T _ {i + 1}; t) \cdot (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t). \end{array}
$$

This is the value of a single floater payment. The claim follows by summation over i. | 

Definition 113 (Floating Rate Bond): 

Let $T _ { i } , i = 1 , \ldots , n$ denote a given time discretization (a tenor structure). A floating rate bond pays 

$$
N \cdot L (T _ {i}, T _ {i + 1}; T _ {i}) \cdot (T _ {i + 1} - T _ {i}) + N \cdot \left\{ \begin{array}{l l} 0 & \text {if} i + 1 <   n \\ 1 & \text {if} i + 1 = n \end{array} \right. \quad \text {in} T _ {i + 1}
$$

for $i = 1 , \ldots , n - 1 ( n - 1$ payments). 

The value of a floating rate bond is $N \cdot P ( T _ { 1 } )$ , because it is just the sum of a floater (value $N \cdot P ( T _ { 1 } ) ) - N \cdot P ( T _ { 2 } ) )$ and a zero coupon bond with maturity $T _ { 2 }$ (value $N \cdot P ( T _ { 2 } ) )$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/c6038839e0dfe76ab583d659e0950d56b08b74d816f3067b518a5b1651c2c84a.jpg)


Interpretation: Definition 111 considers only the coupon payments of a floater. Normally an exchange of notional takes place at the beginning and end of the product: A payment of −N is made in $T _ { 1 }$ (receive notional) and a payment of N is made in $T _ { 2 }$ (pay notional). Since from Theorem 112 the value of the pure 

coupon payments is $N \cdot P ( T _ { 1 } ) - N \cdot P ( T _ { n } )$ , the value of a floater with exchange of notional is 0. 

Figure 9.1 shows a cash-flow diagram for a floater with exchange of notional. At time $T _ { 1 }$ the notional N is invested over the period $[ T _ { 1 } , T _ { 2 } ]$ with an interest rate $L ( T _ { 1 } , T _ { 2 } ; T _ { 1 } )$ , fixed at the beginning of the period. In $T _ { 2 }$ the interest is paid and the notional N is reinvested over the following period (with a newly fixed rate). At the end $T _ { n }$ the interest for the last period is paid together with the notional. C| 

As shown, there are two diferent ways to derive the value of the floater. The first method uses the fact that the payment $N { \cdot } L ( T _ { i } , T _ { i + 1 } ; T _ { i } ) { \cdot } ( T _ { i + 1 } - T _ { i } )$ is a $\mathcal { F } _ { T _ { i } }$ -measurable random variable paid in $T _ { i + 1 }$ . Thus, its value as of time1<sub>1</sub> $T _ { i }$ is given by multiplication with $P ( T _ { i + 1 } ; T _ { i } )$ . Since this value could be expressed as a portfolio of bonds we know its time t value. Essentially, we 2 T1 2 · P(t;T2)      2 derive a replication portfolio for each cash-flow. The second method considers relative prices and applies Theorem 79. 

<sub>In this context, the time</sub>   2 d T<sub>2</sub>. $T _ { i }$ is calledfixing date and the time $T _ { i + 1 }$ is called payment date.<sup>!</sup>| 

Definition 114 (Fixing Date, Payment Date): 

Let $T _ { 2 } \geq T _ { 1 }$ and $V _ { T _ { 1 } } ( T _ { 2 } )$ be $\mathrm { a } \mathcal { F } _ { T _ { 1 } }$ -measurable random variable defining a payment made in $T _ { 2 } .$ Then $T _ { 1 }$ is called Fixing Date and $T _ { 2 }$ is called Payment Date of $V _ { T _ { 1 } } ( T _ { 2 } )$ <sub>. See also Figure 9.2.</sub>   itpunkt ab, an 

Lemma 115 (Moving the payment date): Let $t \geq T _ { 1 }$ . The value of a payment $V _ { T _ { 1 } } ( T _ { 2 } )$ with fixing date $T _ { 1 }$ and payment date $T _ { 2 }$ corresponds to the value of a payment of $V _ { T _ { 1 } } ( T _ { 2 } ) \cdot P ( T _ { 2 } ; t )$ in t for $t < T _ { 2 }$ and the value of a payment of $\begin{array} { r } { V _ { T _ { 1 } } ( T _ { 2 } ) \cdot \frac { 1 } { P ( t ; T _ { 2 } ) } } \end{array}$ in t for $t > T _ { 2 }$ 

Proof: The first part follows as in the proof of Theorem 112, the second part follows fromdes Fixing Dates. Fur¨ Zeitpunkte kleiner als das Fixing Dates ist Lemma 106 ixing Dates. Fur¨ Zeitpunkte kleiner als das Fixing Dates ist Lemma 106 nicht exchanging t andanwendbar.ndbar. In diesem $T _ { 2 }$ | 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/21bd1c3ee6b7810b014bee3ad94012245b70ca2e8cb1c3d3f9a0d7730cf04757.jpg)



Figure 9.2.: Fixing date, payment date and evaluation date


Remark 116 (On the additivity of cashflows with diferent payment dates): The value of Definition 108 (Swap (Payer Swap)): ition 108 (Swap (Payer Swap)): "<sub>a financial product or a single cash flow depends on its evaluation time, the time we select to</sub> Ein Swap ist eine Austasuchzahlung einer festen Zinsrate gegen eine variable Zinswap ist eine Austasuchzahlung einer festen Zinsrate gegen eine variable Zinsrate.observe it. Two payments with the same payment date may be added to create a single one. Der Swap zahltwap zahltFor two payments with diferent payment dates a summation is not meaningful. To calculate the total value of several products or cash flows at time t we have to move all cash flows as in N (L(T T ; T ) S ) (T T ) in TLemma 115. However, Lemma 115 applies only to times t larger than the fixing dates. The lemma is not applicable for times before the fixing date. Here, a risk-neutral evaluation has to iten T , . . . ,be performed. 

−     ∈       <sub>Relative prices behave diferently: Relative prices are additive (independent of the fixing</sub> <sup>+</sup> date). Let $V _ { T _ { 1 } }$ <sup>i+1</sup> <sup>i</sup>   denote a $\mathcal { F } _ { T }$ -measurable random variable defining the value of a financial product in time $T _ { 2 }$ . Then we have: 

Defi  <sub>• For</sub> $t < T _ { 1 } \colon \mathsf { E } ^ { \mathbb { Q } ^ { N } } \Big ( \frac { V _ { T _ { 1 } } } { N ( T _ { 2 } ) } | \mathcal { F } _ { t } \Big )$ wap, Receiver Swap):   <sub>is the N(t)-relative value of</sub> $V _ { T _ { 1 } }$ at time t. This follows from Der in Definnition 108 dTheorem 79. 

• For $\begin{array} { r } { t > T _ { 1 } \colon \mathbb { E } ^ { \mathbb { Q } ^ { N } } \bigl ( \frac { V _ { T _ { 1 } } } { N ( T _ { 2 } ) } | \mathcal { F } _ { t } \bigr ) = V _ { T _ { 1 } } \cdot \mathbb { E } ^ { \mathbb { Q } ^ { N } } \bigl ( \frac { 1 } { N ( T _ { 2 } ) } | \mathcal { F } _ { t } \bigr ) = \frac { V _ { T _ { 1 } } \cdot P ( T _ { 2 } ; t ) } { N ( t ) } } \end{array}$ is the $N ( t )$ -relative value of $V _ { T _ { 1 } }$ at time t. This follows from Lemma 115. 

The additivity of relative prices follows from the linearity of the expectation operator. 

## Definition 117 (Swap (Payer Swap)):

A swap is an exchange payment of fixed rate for a floating rate. Let $0 = T _ { 0 } < T _ { 1 } < T _ { 2 } < . . . <$ $T _ { n }$ denote a given tenor structure. A swap pays 

$$
N \cdot (L (T _ {i}, T _ {i + 1}; T _ {i}) - S _ {i}) \cdot (T _ {i + 1} - T _ {i}) \quad \text { in } T _ {i + 1}
$$

for $i = 1 , \ldots , n { - 1 } \left( n { - 1 } \right.$ payments), where $S _ { i } \in \mathbb { R }$ denotes the fixed swap rate and $L ( T _ { i } , T _ { i + 1 } ; T _ { i } )$ denotes the forward rate from Definition 99, and N denotes the notional. The swap defined here is a payer swap, see Definition 118. y 

## Definition 118 (Payer Swap, Receiver Swap):

The swap defined in Definition 117 with payments 

$$
N \cdot (L (T _ {i}, T _ {i + 1}; T _ {i}) - S _ {i}) \cdot (T _ {i + 1} - T _ {i}) \quad \text { in } T _ {i + 1}
$$

is called payer swap. In contrast, the swap with reversed payments 

$$
N \cdot (S _ {i} - L (T _ {i}, T _ {i + 1}; T _ {i})) \cdot (T _ {i + 1} - T _ {i}) \quad \text { in } T _ {i + 1}
$$

is called receiver swap. The term payer / receiver indicates whether the holder of the swap has to pay the fixed coupon (it enters negative) or receives the fixed coupon (it enters positive). y 

## Definition 119 (Floating Leg, Fixed Leg):

The payments of a swap may be decomposed into 

$$
N \cdot L (T _ {i}, T _ {i + 1}; T _ {i}) \cdot (T _ {i + 1} - T _ {i}) \quad \mathrm{in} T _ {i + 1}\tag{9.2}
$$

and 

$$
N \cdot S _ {i} \cdot (T _ {i + 1} - T _ {i}) \quad \text { in } T _ {i + 1}.\tag{9.3}
$$

The payments (9.2) of the variable rates are called floating $l e g .$ , the payments of the constant rates (9.3) are calledfixed leg. y 

Theorem 120 (Value of a Swap): At time $t \leq T _ { 1 }$ the value of a swap is given by 

$$
V _ {\text { Swap }} (t) = N \cdot \sum_ {i = 1} ^ {n - 1} \left(L \left(T _ {i}, T _ {i + 1}; t\right) - S _ {i}\right) \cdot \left(T _ {i + 1} - T _ {i}\right) \cdot P \left(T _ {i + 1}; t\right).
$$

Proof: The swap consists of a floater (floating leg, (9.2)) and fixed payments $- N { \cdot } S _ { i } { \cdot } ( T _ { i + 1 } { - } T _ { i } )$ in $T _ { i + 1 }$ for which their time t value is the corresponding multiple of $P ( T _ { i + 1 } ; t )$ . The claim follows by applying Theorem 112 to the floating leg. | 

Remark 121 (Swap rate): Let $T _ { 1 } , \ldots , T _ { n }$ be a given tenor structure. Consider a swap as in Definition 117. The par swap rate S (in t) is the unique rate for which a swap with $S _ { i } : = S$ has the time t value 0, i.e. the total time t value of the payments 

$$
N \cdot (L (T _ {i}, T _ {i + 1}; T _ {i}) - S) \cdot (T _ {i + 1} - T _ {i}) \quad \mathrm{in} T _ {i + 1}
$$

is 0. Since the time t value of such a swap is given by 

$$
N \cdot \sum_ {i = 1} ^ {n - 1} (L (T _ {i}, T _ {i + 1}; t) - S) \cdot (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t),
$$

then 

$$
\begin{array}{c} S = \frac {\sum_ {i = 1} ^ {n - 1} L (T _ {i} , T _ {i + 1} ; t) (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1} ; t)}{\sum_ {i = 1} ^ {n - 1} (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1} ; t)} \\ = \frac {P (T _ {1} ; t) - P (T _ {n} ; t)}{\sum_ {i = 1} ^ {n - 1} (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1} ; t)}. \end{array}
$$

Definition 122 (Par swap rate): 

Let $T _ { 1 } < T _ { 2 } < \ldots < T _ { n }$ . The par swap rate (often just called swap rate) $S ( T _ { 1 } , \dots , T _ { n } )$ is defined by 

$$
S \left(T _ {1}, \dots , T _ {n}; t\right) := \frac {P \left(T _ {1} ; t\right) - P \left(T _ {n} ; t\right)}{\sum_ {i = 1} ^ {n - 1} \left(T _ {i + 1} - T _ {i}\right) \cdot P \left(T _ {i + 1} ; t\right)}.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/5d2b55e0a0bbff708022c4e63a0fce47197c07e7a4263d2cd2b35318a322df1b.jpg)


$$
k = i, \dots , j - 1
$$

Interpretation: Since the par swap rate is the rate for which a corresponding swap has value 0, we may see the par swap rate $S _ { i , j } : = S ( T _ { i } , \ldots , T _ { j } )$ as some mean of the forward rates $L _ { k } , k = i , \ldots , j - 1$ . Indeed, the par swap rate $S _ { i , j }$ 」 is a convex combination (and thus a weighted average) of the forward rated $L _ { k } ,$ j − 1 as shown in the following lemma. C| 

Lemma 123 (Swap rate as convex combination of the forward rates): Let $T _ { i } < T _ { i + 1 } <$ $\dots < T _ { j }$ denote a given tenor structure. Then we have 

$$
S _ {i, j} = \sum_ {k = i} ^ {j - 1} \alpha_ {k} L _ {k}, \quad \text { with } \quad \alpha_ {k} \geq 0, \quad \sum_ {k = i} ^ {j - 1} \alpha_ {k} = 1.
$$

The weights $\alpha _ { k }$ are given by $\begin{array} { r } { \alpha _ { k } : = \frac { P ( T _ { k + 1 } ) \cdot ( T _ { k + 1 } - T _ { k } ) } { \sum _ { l = i } ^ { j - 1 } P ( T _ { l + 1 } ) \cdot ( T _ { l + 1 } - T _ { l } ) } } \end{array}$ . The weights are stochastic. 

Proof: With $P ( T _ { k + 1 } ) ( T _ { k + 1 } - T _ { k } ) \cdot L _ { k } = P ( T _ { k } ) - P ( T _ { k + 1 } )$ we have 

$$
\sum_ {k = i} ^ {j - 1} P (T _ {k + 1}) (T _ {k + 1} - T _ {k}) \cdot L _ {k} = P (T _ {i}) - P (T _ {j}),
$$

and thus 

$$
\sum_ {k = i} ^ {j - 1} \frac {P (T _ {k + 1}) (T _ {k + 1} - T _ {k})}{\sum_ {l = i} ^ {j - 1} P (T _ {l + 1}) \cdot (T _ {l + 1} - T _ {l})} \cdot L _ {k} = \frac {P (T _ {i}) - P (T _ {j})}{\sum_ {l = i} ^ {j - 1} P (T _ {l + 1}) \cdot (T _ {l + 1} - T _ {l})} = S _ {i, j}.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/dcb16a5ac510e7879d5dc7d2dececa285758f4b41704e6b28cf200d6c0c82bc5.jpg)


Interpretation (Usage of the term bond and swap): The terms bond and swap are also used in a much broader sense than given. A financial product with coupon payments and final notional payments at maturity is called a bond. A financial product where coupon payments are exchanged (and no notional is paid) 

is called a swap. The terms are used independently of the specific structure of the coupons. A coupon may be a constant (fix), a variable rate (float) or a complex function of one or more interest rates (structured). In the last case, the coupon is called a structured coupon and the corresponding bond and swap are called structured bond and structured swap. 

A swap may be interpreted as a portfolio of a bond long (i.e. with positive cash-flow) and a bond short (i.e. with negative cash-flow), where the two notional payments cancel. In Section 12.2.1 we will consider the relationship between bonds and swaps. C| 

## 9.1.2. Money-Market Account

If we invest at time $T _ { 0 } = 0$ a unit currency over the period $[ T _ { 0 } , T _ { 1 } ]$ , then we receive at $T _ { 1 }$ the amount $1 + L ( T _ { 0 } , T _ { 1 } ; T _ { 0 } ) \cdot ( T _ { 1 } - T _ { 0 } )$ . If this amount is reinvested for another period and if this process is continued for periods $[ T _ { j } , T _ { j + 1 } ]$ with $j = 1 , 2 , . . . ,$ then we have at time $T _ { i }$ a value of 

$$
\prod_ {j = 0} ^ {i - 1} (1 + L (T _ {j}, T _ {j + 1}; T _ {j}) \cdot (T _ {j + 1} - T _ {j})).\tag{9.4}
$$

Equivalently, we may write this with the instantaneous forward rate as 

$$
\prod_ {j = 0} ^ {i - 1} \exp \left(\int_ {T _ {j}} ^ {T _ {j + 1}} f (T _ {j}, \tau) \mathrm{d} \tau\right) = \exp \left(\sum_ {j = 0} ^ {i - 1} \int_ {T _ {j}} ^ {T _ {j + 1}} f (T _ {j}, \tau) \mathrm{d} \tau\right).\tag{9.5}
$$

If we consider a continuum of infinitesimal periods, i.e. we consider continuously compounding with the short rate, then the corresponding value will evolve as 

$$
B (t) = \exp \big (\int_ {T _ {0}} ^ {t} r (\tau) \mathrm{d} \tau \big).\tag{9.6}
$$

Definition 124 (Rolling Bond): 

The financial product 

$$
R (t) := P \left(T _ {m (t) + 1}; t\right) \cdot \prod_ {j = 0} ^ {m (t)} \left(1 + L \left(T _ {j}, T _ {j + 1}; T _ {j}\right) \cdot \left(T _ {j + 1} - T _ {j}\right)\right),
$$

where $m ( t ) : = \operatorname* { m a x } \{ i { \mathrm { ~ } } : T _ { i } \leq t \}$ , is called (single period) rolling bond. 

## Definition 125 (Savings Account, Money Market Account):

The financial product B in (9.6) is called savings account or money market account. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/f5ad480f1607156a1889dfffff7520c2381f91eec81c3ea99952a74f7fb8ee3d.jpg)


Interpretation: The financial product B has to be interpreted as an idealization (like the short rate itself), since infinitesimal periods are an idealization. 

Note that (9.4) and (9.5) are equivalent, whereas $B ( T _ { i } )$ does not coincide with 1 the value of (9.4) generally. The expressions (9.4) and (9.5) depend on the choice the periods and if evaluated in $T _ { i } ,$ , they are $\mathcal { F } _ { T _ { i - } }$ measurable random variables, whereas $B ( T _ { i } )$ $\mathcal { F } _ { T _ { i } }$ measurable only. C| 

## 9.2. Interest Rate Products Part 2: Simple Options

## 9.2.1. Cap, Floor, Swaption

## Definition 126 (Caplet):

A Caplet is an option on theforward rate (LIBOR) and pays 

$$
V _ {\text { caplet }} (T _ {2}) = N \cdot \max \left(L (T _ {1}, T _ {2}; T _ {1}) - K, 0\right) \cdot (T _ {2} - T _ {1}) \quad \text { in } T _ {2}\tag{9.7}
$$

where K is the strike rate, $L ( T _ { 1 } , T _ { 2 } ; t )$ the LIBOR and N the notional. Payment date and fixing date $0 < T _ { 1 } < T _ { 2 }$ coincide with the LIBOR period $[ T _ { 1 } , T _ { 2 } ]$ y 

## Definition 127 (Cap):

A cap is a portfolio of caplets. Let $0 = T _ { 0 } < T _ { 1 } < T _ { 2 } < . . . < T _ { n }$ denote a given tenor structure. A cap pays 

$$
N \cdot \max \left(L (T _ {i}, T _ {i + 1}; T _ {i}) - K _ {i} , 0\right) \cdot (T _ {i + 1} - T _ {i}) \quad \text { in } T _ {i + 1}\tag{9.8}
$$

for $i = 1 , \ldots , n - 1 ( n - 1 \mathrm { p a y m e n t s } )$ , where $K _ { i }$ are the strike rates, $L ( T _ { i } , T _ { i + 1 } ; T _ { i } )$ are the LIBOR rates and N denotes the notional. y 

Remark 128 (Floorlet, Floor): If in (9.8) or correspondingly in (9.7) the payof is 

$$
N \cdot \max \left(K _ {i} - L (T _ {i}, T _ {i + 1}; T _ {i}) , 0\right) \cdot (T _ {i + 1} - T _ {i}) \quad \text { in } T _ {i + 1},
$$

then the product is called Floor or Floorlet, respectively. 

Remark 129 (Caplet, Cap): The name caplet (and thus cap) seems counter-intuitive. A cap is usually an upper bound, a floor a lower bound. Indeed, the payof 

$$
[ L ] ^ {K} := \min (L, K)
$$

is called capped and the payof 

$$
[ L ] _ {K} := \max (L, K)
$$

is called floored. The counter-intuitive name caplet for (9.7) stems from its application as a swap that exchanges a floating rate L against a capped coupon $[ L ] ^ { K }$ : 

$$
L - [ L ] ^ {K} = \max (L - K, 0),
$$

i.e. 

$$
- [ L ] ^ {K} = - L + \max (L - K, 0).
$$

If we have the obligation to pay a variable interest rate (−L), buying a cap $( + \operatorname* { m a x } ( L - K , 0 ) )$ will cover the risk of an increasing interest rate, i.e. the payment is capped $( - [ L ] ^ { K } )$ . The cap is the product one has to buy to have floating payments capped.<sup>1</sup> 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/cb86338771accbdd1b62637548a3172ea228e134e37f4732d24a330ec83407af.jpg)



Figure 9.3.: Call spread approximation of a digital option by two call options.


## Definition 130 (Swaption):

A swaption is an option on a swap. Let $V _ { \mathrm { s w a p } } ( t )$ denote the time t value of a swap as defined by Definition 117. Then the value of a swaption (with underlying $V _ { \mathrm { s w a p } } )$ is given by the payout 

$$
V _ {\text { swaption }} (T _ {1}) := \max \left(V _ {\text { swap }} (T _ {1}), 0\right) \quad \text { in } T _ {1}.
$$

Definition 131 (Digital Caplet): 

A digital caplet pays 

$$
V _ {\text { digital }} (T _ {2}) = N \cdot \mathbf {1} (L (T _ {1}, T _ {2}; T _ {1}) - K) \cdot (T _ {2} - T _ {1}) \quad \text { in } T _ {2},
$$

where K is the strike rate, $L ( T _ { 1 } , T _ { 2 } ; t )$ is the LIBOR, N denotes the notional and 1 denotes the indicator function (with $\mathbf { 1 } ( x ) : = 1$ for $x > 0$ and $\mathbf { 1 } ( x ) : = 0 { \mathrm { e l s e } } )$ y 

Lemma 132 (Digital Caplet valuation, Call-Spread): For the value $V _ { \mathrm { d i g i t a l } } ( K , 0 )$ of a digital caplet with strike K we have 

$$
V _ {\text { digital }} (K; 0) = - \frac {\partial}{\partial K} V _ {\text { caplet }} (K; 0).
$$

The approximation of the diferential using finite diferences 

$$
\tilde {V} _ {\text {digital}} (K; 0) = - \frac {V _ {\text {caplet}} (K + \epsilon ; 0) - V _ {\text {caplet}} (K - \epsilon ; 0)}{2 \epsilon}
$$

is called call spread. 

Proof: The proof follows the lines of the proof in Lemma 81. 

## 9.2.1.1. Example: Option on a Coupon Bond

Consider the option to receive at $T _ { 1 }$ a coupon bond in exchange for a notional payment. A coupon bond with tenor structure $T _ { i } , i = 1 , \ldots , n ,$ , coupons $C _ { i }$ and maturity $T _ { n }$ pays 

$$
C _ {i} \cdot (T _ {i + 1} - T _ {i}) + \left\{ \begin{array}{l l} 0 & \text { if } i + 1 <   n \\ 1 & \text { if } i + 1 = n \end{array} \right. \quad \text { in } T _ {i + 1}.
$$

The time t value of a forward starting coupon bond with an initial notional payment 1 in $T _ { 1 }$ i 

$$
V _ {\mathrm{fwdCpnBnd}} (t) = \sum_ {i = 1} ^ {n - 1} C _ {i} \cdot (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t) + P (T _ {n}; t) - P (T _ {1}; t),
$$

for $t \leq T _ { 1 }$ , see (9.1). Since $P ( T _ { 1 } ; t ) - P ( T _ { n } ; t )$ is the value of a floating rate bond, see Definition 113, this is just a swap 

$$
= \sum_ {i = 1} ^ {n - 1} (C _ {i} - L (T _ {i}, T _ {i + 1}; t)) \cdot (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t).
$$

Consequently, an option on forward starting coupon bond is just a swaption. 

## 9.2.2. Foreign Caplet, Quanto

## Definition 133 (Foreign Caplet):

A foreign caplet is a caplet in a foreign currency. From the domestic investor’s point of view it pays 

$$
\tilde {N} \cdot \max \left(\tilde {L} (T _ {1}, T _ {2}; T _ {1}) - K, 0\right) \cdot (T _ {2} - T _ {1}) \cdot F X (T _ {2}) \quad \text { in } T _ {2},
$$

where $K \in \mathbb { R }$ is the strike rate, $\tilde { L } ( T _ { 1 } , T _ { 2 } ; t )$ is the foreign LIBOR, $F X ( T _ { 2 } )$ is the exchange rate and N<sup>˜</sup> denotes the notional in foreign currency.<sup>2</sup> y 

Remark 134 (Units): It is useful to consider units, just as one would do in physics. A domestic bond P has the unit of one domestic currency, $[ P ] = { \mathrm { d o m } }$ . Interest rates have the dimension $\textstyle { \frac { 1 } { \mathrm { t i m e } } } , \mathbf { e } . \mathbf { g } .$ . for the forward rate (LIBOR) we have $[ L ( T _ { i } , T _ { i + 1 } ) \cdot ( T _ { i + 1 } - T _ { i } ) ] = 1$ , since it is the quotient of two bonds. The unit of the stochastic process FX is $\textstyle [ F X ] = { \frac { \mathrm { d o m } } { \mathrm { f o r } } }$ , i.e. FX(t) is the time t value of a foreign currency unit in domestic currency. In Definition 133 we have $[ \tilde { N } ] = \mathrm { f o r }$ . For the following product it is crucial to consider units. 

## Definition 135 (Quanto, Quanto Caplet):

A quanto is a financial product for which a payout will be converted from a foreign currency to a domestic currency without use of the exchange rate. Instead of $F X ( t )$ it uses $1 \frac { \hat { \mathrm { d o m } } } { \hat { \mathrm { f o r } } }$ or another conversion factor (the quanto rate) fixed apriori. 

Let $0 < T _ { 1 } < T _ { 2 }$ denotefixing and payment date, respectively. A quanto caplet pays 

$$
\tilde {N} \cdot \max \left(\tilde {L} (T _ {1}, T _ {2}; T _ {1}) - K, 0\right) \cdot (T _ {2} - T _ {1}) \cdot 1 \frac {\text { dom }}{\text { for }} \quad \text { in } T _ {2},
$$

where K is the strike rate (dimension $\begin{array} { r } { \frac { 1 } { \mathrm { t i m e } } ) , \tilde { L } ( T _ { 1 } , T _ { 2 } ; t ) } \end{array}$ is the foreign LIBOR (dimensionless) and $\tilde { N }$ denotes the notional inforeign currency. y 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/26b74a563f69364b33883da4e60d3347db2d80e0b9da61764528814992cca65f.jpg)


Further Reading: An introduction to the basics of interest rates products may be found in [5] (in German). C| 

# The Black Model for a Caplet

We consider a caplet as defined by Definition 126 as an option on the forward rate $L _ { 1 } : =$ $L ( T _ { 1 } , T _ { 2 } )$ for given times $0 < T _ { 1 } < T _ { 2 }$ 

The Black model for the valuation of a caplet postulates a lognormal dynamic of the underlying LIBOR<sup>1</sup> 

$$
\mathrm{d} L _ {1} (t) = \mu^ {\mathbb {P}} (t) L _ {1} (t) \mathrm{d} t + \sigma (t) L _ {1} (t) \mathrm{d} W ^ {\mathbb {P}} (t), \quad \sigma (t) \geq 0, \text { under } \mathbb {P}.\tag{10.1}
$$

We seek the price V(0) of the payof profile 

$$
V (T _ {2}) := \max \left(\left(L _ {1} \left(T _ {1}\right) - K\right) \cdot \left(T _ {2} - T _ {1}\right), 0\right),
$$

where $L _ { 1 } \cdot ( T _ { 2 } - T _ { 1 } ) : = P ( T _ { 1 } ) / P ( T _ { 2 } ) - 1 , { \mathrm { i . e . } } L _ { 1 } = L _ { 1 } ( T _ { 1 } , T _ { 2 } )$ denotes the forward rate (the (forward) LIBOR) of the period $[ T _ { 1 } , T _ { 2 } ]$ . Without loss of generality we assume that the notional is 1. We choose the $T _ { 2 ^ { - } } { \bf B }$ ond as Numeraire´ 

$$
N (t) := P \left(T _ {2}; t\right).
$$

This choice of the numeraire is the crucial trick in the derivation of a risk-neutral pricing´ formula. Since 

$$
\begin{array}{l} L _ {1} = \frac {1}{(T _ {2} - T _ {1})} \cdot (P (T _ {1}) / P (T _ {2}) - 1) = \frac {1}{(T _ {2} - T _ {1})} \cdot \frac {P (T _ {1}) - P (T _ {2})}{P (T _ {2})} \\ = \frac {\frac {1}{(T _ {2} - T _ {1})} \cdot (P (T _ {1}) - P (T _ {2}))}{N}, \end{array}
$$

$L _ { 1 }$ is the N-relative price of a traded $\mathrm { a s s e t . } ^ { 2 }$ From Theorem 74 we have the existence of an equivalent martingale measure $\mathbb { Q } ^ { N }$ such that all N-relative prices of traded assets are martingales. Thus $L _ { 1 }$ is drift-free (see Lemma 52), i.e. 

$$
\mathrm{d} L _ {1} (t) = \sigma (t) L _ {1} (t) \mathrm{d} W ^ {\mathbb {Q} ^ {N}} (t), \quad \text { under } \mathbb {Q} ^ {N}.
$$

For the process $Y : = \log ( L _ { 1 } )$ we have it from Lemma 49 that 

$$
\mathrm{d} (\log (L _ {1} (t)) = - \frac {1}{2} \sigma (t) ^ {2} \mathrm{d} t + \sigma (t) \mathrm{d} W ^ {\mathbb {Q} ^ {N}} (t),
$$

<sup>1</sup> The lognormal Process is often written in the form $\begin{array} { r } { \frac { \mathrm { d } L _ { 1 } ( t ) } { L _ { 1 } ( t ) } = \mu ^ { \mathbb { P } } ( t ) \mathrm { d } t \ + \ \sigma ( t ) \mathrm { d } W ^ { \mathbb { P } } ( t ) . } \end{array}$ 

<sup>2</sup> The traded asset is the portfolio $\begin{array} { r } { \frac { 1 } { ( T _ { 2 } - T _ { 1 } ) } \cdot ( P ( T _ { 1 } ) - P ( \stackrel { . } { T } _ { 2 } ) ) } \end{array}$ consisting of $\frac { 1 } { ( T _ { 2 } - T _ { 1 } ) }$ fractions of a $T _ { 1 }$ -bond (long) and $T _ { 2 }$ -bond (short). 

i.e. $\log ( L _ { 1 } ( T ) )$ is normal distributed with mean log $\begin{array} { r } { ( L _ { 1 } ( 0 ) ) - \frac { 1 } { 2 } \bar { \sigma } ^ { 2 } T } \end{array}$ and standard deviation $\bar { \sigma } \sqrt { T }$ , with $\begin{array} { r } { \bar { \sigma } : = \big ( \frac { 1 } { T } \int _ { 0 } ^ { T } \sigma ^ { 2 } ( t ) \mathrm { d } t \big ) ^ { 1 / 2 } } \end{array}$ , see Section 4. 

For the option value we now have 

$$
V (T _ {2}) = \max \left(\left(L _ {1} (T _ {1}) - K\right) \cdot \left(T _ {2} - T _ {1}\right), 0\right) \quad \text { in } T _ {2}
$$

and from $N ( T _ { 2 } ) = 1$ we have<sup>3</sup> 

$$
\begin{array}{l} \frac {V (0)}{N (0)} = \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {V (T _ {2})}{N (T _ {2})} \mid \mathcal {F} _ {0}\right) = \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(V (T _ {2}) \mid \mathcal {F} _ {0}\right) \\ = \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\max ((L _ {1} (T _ {1}) - K) \cdot (T _ {2} - T _ {1}), 0) \mid \mathcal {F} _ {0}\right) \end{array}
$$

i.e. 

$$
V (0) = P \left(T _ {2}; 0\right) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\max \left(\left(L _ {1} \left(T _ {1}\right) - K\right), 0\right)\right) \cdot \left(T _ {2} - T _ {1}\right).
$$

Knowing the distribution of $L _ { 1 }$ under $\mathbb { Q } ^ { N }$ this expectation may be represented as 

$$
V (0) = P \left(T _ {2}; 0\right) \cdot \left[ L _ {1} (0) \Phi \left(d _ {+}\right) - K \Phi \left(d _ {-}\right) \right] \cdot \left(T _ {2} - T _ {1}\right),\tag{10.2}
$$

where $\begin{array} { r } { \Phi ( x ) : = \frac { 1 } { \sqrt { 2 \pi } } \int _ { - \infty } ^ { x } \exp ( - \frac { y ^ { 2 } } { 2 } ) \mathrm { d } y } \end{array}$ and $\begin{array} { r } { d _ { \pm } = \frac { \ln ( \frac { L _ { 1 } ( 0 ) } { K } ) \pm \frac { 1 } { 2 } \bar { \sigma } ^ { 2 } T _ { 1 } } { \bar { \sigma } \sqrt { T _ { 1 } } } } \end{array}$ , see Section 4. 

Remark 136 (Implied Black Volatility): Similarly to Remark 80 on page 78 we have: Equation (4.3) gives us the price of the option under the model (10.1) as a function of the model parameter $\bar { \sigma } .$ . In this context ¯<sub>σ</sub> is called the Black volatility. Taking the other model and product parameters $( r , K , T _ { 1 } , T _ { 2 } )$ as constants, the pricing formula (10.2) represents a bijection 

$$
\begin{array}{c} \bar {\sigma} \mapsto V (0) \\ [ 0, \infty) \to [ P (T _ {2}; 0) \cdot \max (L (0) - K, 0), P (T _ {2}; 0) \cdot L (0) ]. \end{array}
$$

The $\bar { \sigma }$ calculated for a given price V(0) through inversion of the pricing formula is called the implied Black volatility. 

Lemma 137 (Price of a digital caplet under the Black model dynamics): The price of a digital caplet under the Black model is 

$$
V _ {\text { digital }} (K; 0) = N \cdot P (T _ {2}; 0) \cdot \Phi (d _ {-}) \cdot (T _ {2} - T _ {1}),
$$

where $\begin{array} { r } { \Phi ( x ) : = \frac { 1 } { \sqrt { 2 \pi } } \int _ { - \infty } ^ { x } \exp ( \frac { - y ^ { 2 } } { 2 } ) \mathrm { d } y \mathrm { a n d } d _ { - } = \frac { \ln ( \frac { L _ { 1 } ( 0 ) } { K } ) - \frac { 1 } { 2 } \bar { \sigma } ^ { 2 } T _ { 1 } } { \bar { \sigma } \sqrt { T _ { 1 } } } . } \end{array}$ 

# Pricing of a Quanto Caplet (Modeling the FFX)

In this section all quantities related to a foreign currency are marked with a ˜tilde. Let $0 < T _ { 1 } <$ $T _ { 2 }$ denote fixing and payment date respectively. The payof profile of a quanto caplet is given by 

$$
V (T _ {2}) = \max \left(\tilde {L} (T _ {1}, T _ {2}; T _ {1}) - K, 0\right) \cdot (T _ {2} - T _ {1}) \cdot 1 \frac {\mathrm{dom}}{\text { for }} \quad \text { in } T _ {2},
$$

where $K$ is the given strike rate and $\tilde { L } ( T _ { 1 } , T _ { 2 } ; t )$ is the foreign forward rate. The notional and quanto rate are assumed to be 1. 

We assume a lognormal dynamic for the foreign LIBOR, i.e. we model it $\mathrm { a s ^ { 1 } }$ 

$$
\mathrm{d} \tilde {L} (t) = \mu^ {\mathbb {P}} (t) \tilde {L} (t) \mathrm{d} t + \sigma_ {\tilde {L}} (t) \tilde {L} (t) \mathrm{d} W _ {3} ^ {\mathbb {P}} (t).
$$

## 11.1. Choice of Numeraire´

If we choose the foreign $T _ { 2 }$ -bond converted to domestic currency, i.e. $\tilde { P } ( T _ { 2 } ; t ) F X ( t )$ , as numeraire, then from´ $\begin{array} { r } { \tilde { L } ( T _ { 1 } , T _ { 2 } ; t ) = \frac { 1 } { T _ { 2 } - T _ { 1 } } \frac { \tilde { P } ( T _ { 1 } ) - \tilde { P } ( T _ { 2 } ) } { \tilde { P } ( T _ { 2 } ) } = \frac { 1 } { T _ { 2 } - T _ { 1 } } \frac { \tilde { P } ( T _ { 1 } ) F X ( t ) - \tilde { \bar { P } } ( T _ { 2 } ) F X ( t ) } { \tilde { P } ( T _ { 2 } ) F X ( t ) } } \end{array}$ (see Section 10) we find 

$$
\mathrm{d} \tilde {L} (t) = \sigma_ {\tilde {L}} (t) \tilde {L} (t) \mathrm{d} W _ {3} (t) \quad \text { under } \mathbb {Q} ^ {\tilde {P} (T _ {2}) \cdot F X}.
$$

Remark 138 (Foreign Market, Cross Currency Change of Numeraire):´ Note that the foreign LIBOR is not a martingale with respect to $\mathbb { Q } ^ { \tilde { P } ( T _ { 2 } ) }$ , since we are based in the domestic market. For the domestic investor the foreign bond $\tilde { P } ( T _ { i } )$ is not a traded asset, but the foreign bond converted to domestic currency $\tilde { P } ( T _ { i } ) \cdot F X$ is a traded asset. Although we have 

$$
\mathrm{d} \tilde {L} (t) = \sigma_ {\tilde {L}} (t) \tilde {L} (t) \mathrm{d} W _ {3} (t) \quad \text { under } \mathbb {Q} ^ {\tilde {P} (T _ {2})},
$$

we cannot use this change of measure, since $\tilde { P } ( T _ { 2 } )$ is not a traded asset and thus not a numeraire´ in the domestic market. Choosing the domestic bond $P ( T _ { 2 } )$ (a traded asset) as numeraire, we´ generally have 

$$
\mathrm{d} \tilde {L} (t) \neq \sigma_ {\tilde {L}} (t) \tilde {L} (t) (t) \mathrm{d} W _ {3} (t) \quad \text { under } \mathbb {Q} ^ {P (T _ {2})}.
$$

<sup>1</sup> We write L<sup>˜</sup> for $\tilde { L } ( T _ { 1 } , T _ { 2 } )$ 

Since the payof profile of the quanto caplet is 

$$
V (T _ {2}) = \max \left(\tilde {L} (T _ {1}, T _ {2}; T _ {1}) - K, 0\right) \cdot (T _ {2} - T _ {1}) \cdot 1 \frac {\mathrm{dom}}{\text { for }} \quad \text { in } T _ {2},
$$

it is advantageous to know the dynamics of $\tilde { L } ( T _ { 1 } , T _ { 2 } )$ under the measure $\mathbb { Q } ^ { P ( T _ { 2 } ) }$ , the domestic $T _ { 2 }$ terminal measure. Choosing $P ( T _ { 2 } )$ as numeraire, the num´ eraire is 1 at payment date and will´ not show up in the expectation operator above. This trick has already been used in Chapter 10, where we were lucky that additionally the underlying was a martingale under this measure. 

By the change of measure from $\bar { \mathsf { Q } } ^ { \tilde { P } ( T ; t ) \cdot F X ( t ) } \ \dot { \mathsf { t o } } \ \bar { \mathsf { Q } } ^ { P ( T _ { 2 } ) }$ we have a change of the drift, see Theorem 58 (Girsanov, Cameron, Martin), i.e. 

$$
\mathrm{d} \tilde {L} (t) = \mu^ {P (T _ {2})} (t) \tilde {L} (t) \mathrm{d} t + \sigma_ {\tilde {L}} (t) \tilde {L} (t) \mathrm{d} W _ {3} ^ {P (T _ {2})} (t) \quad \text { under } \mathbb {Q} ^ {P (T _ {2})}.
$$

With other words: The dynamics of the underlying is known under the measure $\mathbb { Q } ^ { \tilde { P } ( T ; t ) \cdot F X ( t ) }$ From the shape of the payof function a change of numeraire from´ $\tilde { P } ( { \cal T } ; t ) \cdot F X ( t )$ to $P ( T ; t )$ thus a change of measure from $\mathbb { Q } ^ { \tilde { P } ( T ; t ) \cdot F X ( t ) } \mathrm { t o } \breve { \mathbb { Q } } ^ { P ( T ; t ) }$ is desirable. We thus define: 

## Definition 139 (Forward FX Rate):

Let $0 < t < T$ . The forward FX rate FFX(T) is defined as 

$$
F F X (T; t) := \frac {\tilde {P} (T ; t)}{P (T ; t)} F X (t).
$$

Remark 140 (Forward FX Rate): The forward FX rate (also known as FX forward) is a relative price of two domestic traded assets. It is dimensionless, since $[ \tilde { P } ( T ; t ) ] ~ = ~ 1 \mathrm { f o r } ,$ $\begin{array} { r } { [ P ( T ; t ) ] = } \end{array}$ 1dom and $\begin{array} { r } { [ F X ( t ) ] = 1 \frac { \mathrm { d o m } } { \mathrm { f o r } } } \end{array}$ . It is a $\mathbb { Q } ^ { P ( T ) }$ martingale. 

We assume lognormal dynamics for $F F X ( T _ { 2 } )$ , i.e. 

$$
\mathrm{d} F F X (T _ {2}; t) = \sigma_ {F F X} (t) F F X (T _ {2}; t) \mathrm{d} W _ {2} ^ {P (T _ {2})} (t) \quad \text { under } \mathbb {Q} ^ {P (T _ {2})}.
$$

Since 

$$
\begin{array}{c} \tilde {L} (T _ {1}, T _ {2}) \cdot F F X (T _ {2}) = \frac {1}{T _ {2} - T _ {1}} \frac {\tilde {P} (T _ {1}) - \tilde {P} (T _ {2})}{\tilde {P} (\mathcal {T} _ {2})} \cdot \frac {\tilde {P} (\mathcal {T} _ {2})}{P (T _ {2})} F X (t) \\ = \frac {1}{T _ {2} - T _ {1}} \frac {(\tilde {P} (T _ {1}) - \tilde {P} (T _ {2})) F X (t)}{P (T _ {2})} \end{array}
$$

is a $P ( T _ { 2 } )$ )-relative price of domestic traded assets (namely a portfolio of foreign bonds), we have that $\tilde { L } ( T _ { 1 } , T _ { 2 } ) \cdot F F X ( T _ { 2 } )$ is a martingale under $\mathbb { Q } ^ { P ( T _ { 2 } ) }$ , i.e. 

$$
\operatorname{Drift} ^ {\mathbb {Q} ^ {P (T _ {2})}} \left(\tilde {L} \left(T _ {1}, T _ {2}\right) \cdot F F X \left(T _ {2}\right)\right) = 0.\tag{11.1}
$$

On the other hand 

$$
\begin{array}{l} \mathrm{d} (\tilde {L} \cdot F F X) \\ = \mathrm{d} \tilde {L} \cdot F F X + \tilde {L} \cdot \mathrm{d} F F X + \mathrm{d} \tilde {L} \cdot \mathrm{d} F F X \\ = F F X \cdot \tilde {L} \cdot \mu^ {P (T _ {2})} \mathrm{d} t + F F X \cdot \tilde {L} \cdot \sigma_ {\tilde {L}} \mathrm{d} W _ {3} ^ {P (T _ {2})} \\ + F F X \cdot \tilde {L} \cdot \sigma_ {F F X} \mathrm{d} W _ {2} ^ {P (T _ {2})} + F F X \sigma_ {F F X} \mathrm{d} W _ {2} ^ {P (T _ {2})} \cdot \sigma_ {\tilde {L}} \tilde {L} \mathrm{d} W _ {3} ^ {P (T _ {2})}, \end{array}
$$

and assuming an instantaneous correlation $\rho ( t )$ for $\mathrm { d } W _ { 2 } ^ { P ( T _ { 2 } ) }$ and $\mathrm { d } W _ { 3 } ^ { P ( T _ { 2 } ) }$ 

$$
= F F X \cdot \tilde {L} \left((\mu^ {P (T _ {2})} + \rho \sigma_ {F F X} \sigma_ {\tilde {L}}) \mathrm{d} t + \sigma_ {\tilde {L}} \mathrm{d} W _ {3} ^ {P (T _ {2})} + \sigma_ {F F X} \mathrm{d} W _ {2} ^ {P (T _ {2})}\right).
$$

From (11.1) we thus find 

$$
\mu^ {P (T _ {2})} (t) = - \rho (t) \sigma_ {F F X} (t) \sigma_ {\tilde {L}} (t).
$$

We now know the dynamics of L<sup>˜</sup> under $\mathbb { Q } ^ { P ( T _ { 2 } ) }$ 

$$
\mathrm{d} \tilde {L} = - \rho (t) \sigma_ {F F X} (t) \sigma_ {\tilde {L}} (t) \tilde {L} (t) \mathrm{d} t + \sigma_ {\tilde {L}} (t) \tilde {L} (t) \mathrm{d} W _ {3} ^ {P (T _ {2})} (t)
$$

and (as in Chapter 10) we know the distribution of $\tilde { L } ( T _ { 1 } , T _ { 2 } )$ (under $\mathbb { Q } ^ { P ( T _ { 2 } ) } )$ is lognormal with 

$$
\begin{array}{l} \log (\tilde {L} (T)) = \mathcal {N} \bigg (\log (\tilde {L} (0)) - \int_ {0} ^ {T} \rho (t) \sigma_ {F F X} (t) \sigma_ {\tilde {L}} (t) \mathrm{d} t - \frac {1}{2} \bar {\sigma} _ {\tilde {L}} ^ {2} \cdot T, \bar {\sigma} _ {\tilde {L}} ^ {2} \cdot T \bigg) \\ = \mathcal {N} \bigg (\log \left(\tilde {L} (0) \cdot e ^ {- \int_ {0} ^ {T} \rho (t) \sigma_ {F F X} (t) \sigma_ {\tilde {L}} (t) \mathrm{d} t}\right) - \frac {1}{2} \bar {\sigma} _ {\tilde {L}} ^ {2} \cdot T, \bar {\sigma} _ {\tilde {L}} ^ {2} \cdot T \bigg), \end{array}
$$

where 

$$
\bar {\sigma} _ {\tilde {L}} ^ {2} = \frac {1}{T} \int_ {0} ^ {T} \sigma_ {\tilde {L}} ^ {2} (t) \mathrm{d} t \quad (\text { mean   variance }).
$$

Altogether it follows an (adjusted) Black formula, where in contrast to the Black formula from Chapter $1 0 \tilde { L } ( 0 )$ is replaced by $\tilde { L } ( 0 ) \cdot e ^ { - \int _ { 0 } ^ { T } \rho ( t ) \sigma _ { F F X } ( t ) \sigma _ { \tilde { L } } ( t ) \mathrm { d } t }$ . The factor 

$$
e ^ {- \int_ {0} ^ {T} \rho (t) \sigma_ {F F X} (t) \sigma_ {\tilde {L}} (t) \mathrm{d} t}
$$

is called the quanto adjustment. 

## Exotic Derivatives

We have already introduced some simple interest rate derivatives. In this section we give a selection of so called exotic derivatives. The name “exotic” does not mean that these derivative products are of less importance. With respect to evaluation models the converse is true: The value of exotic derivatives usually depends on a multitude of model properties, which may not even play a role in the pricing of simple derivatives. An example is the time structure t 7→ <sub>σ</sub>(t) of the volatility in the Black-(Scholes-)Model (4.2), (10.1): Its distribution over time does not play a role in the pricing of a European option, only the integrated variance enters into the pricing formula. It will however play a role for the pricing of a Bermudan option. 

Thus, in this sense we may view certain prototypical properties of exotic derivatives (e.g. having more than one exercise date) as test functions for prototypical properties of (complex) models (e.g. the term structure of volatility).<sup>1</sup> 

## 12.1. Prototypical Product Properties

The list of exotic interest rate derivatives we give in Section 12.2 does not claim to be complete or representative. It is exemplary for prototypical product properties and for applications of the pricing models and methodologies which we will discuss later. We focus a bit on more recent products, where we will discuss the relationship of prototypical product properties to models and their implementation. 

Some product properties, like path dependency or early exercise characterize a whole class of products. To evaluate a product of the respective class, the object path, i.e. the history, for path dependency and conditional expectation for early exercise are central. The path dependency is best represented in a path simulation (forward algorithm). The conditional expectation is best represented in a state lattice (backward algorithm). See Table 12.1. 

Furthermore, some models have a preferred mode of implementation, i.e. as path simulation or as state lattice. Whether a model can be implemented on a state lattice is often decided by it’s Markov dimension, see Table 12.2. 

Thus, prototypical product properties impose requirements on model and implementation. 

<table><tr><td>Prototypical Product Property</td><td>Model Requirement / Implementation</td></tr><tr><td>Early Exercise / Bermudan, low Markov dimension</td><td>backward algorithm, coarse time discretization → state lattice / tree, Section 13.3</td></tr><tr><td>Early Exercise / American, low Markov dimension</td><td>backward algorithm, fine time discretization → PDE, Chapter 14</td></tr><tr><td>Path Dependency, high Markov dimension</td><td>forward algorithm → path simulation, Section 13.1</td></tr><tr><td>Pfad Dependency, model: low Markov dimension product: high Markov dimension</td><td>path simulation through a lattice → Section 13.4</td></tr><tr><td>Early Exercise, high Markov dimension</td><td>forward algorithm with estimator of conditional expectation → Chapter 15</td></tr><tr><td>Pfad Dependency, low Markov dimension</td><td>backward algorithm with extension of state space → Chapter 16</td></tr></table>


Table 12.1.: Prototypical product properties and corresponding model requirements and implementation techniques.


<table><tr><td colspan="2">Model</td><td>Property</td></tr><tr><td>Short Rate Models</td><td>(→ Chapter 22)</td><td>low Markov dimension</td></tr><tr><td>Market Models</td><td>(→ Chapter 19)</td><td>high Markov dimension</td></tr><tr><td>Markov Functional Models</td><td>(→ Chapter 25)</td><td>low Markov dimension</td></tr></table>


Table 12.2.: Markov dimension ofsome models.


## 12.2. Interest Rate Products Part 3: Exotic Interest Rate Derivatives

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/e58c8b5c86af5b8cfb80d0c08cf3ec59c0480863d4d6ff889a77e87fc89208d2.jpg)


Motivation $( \mathbf { \mu } ^ { \mathsf { \epsilon } } \mathbf { W } \mathbf { h } \mathbf { y }$ exotic derivatives?”): A simple European option with payof max $( L ( T ) - K , 0 )$ ) may be interpreted as an insurance against an increase of the interest rate $L ( T )$ . It pays in case of an increasing interest rate the corresponding compensation. 

To interpret an exotic derivatives, e.g. one with payof 

$$
\begin{array}{l l} C _ {i} & \text { if } L (T _ {j}) <   K \forall j \leq i \\ C _ {i} + 1 & \text { if } L (T _ {i - 1}) <   K \leq L (T _ {i}) \\ 0 & \text { else. } \end{array} \quad \begin{array}{l l} \text { and } i + 1 <   n \\ \text { or } i + 1 = n \end{array}
$$

as an insurance is not intuitive. The payof above constitutes a coupon bond which matures if $L ( T _ { i } )$ exceeds the rate K. Such a structure is usually ofered with an above average coupon $C _ { 1 }$ and below average coupons $C _ { i } , i > 1 . ^ { 2 }$ Thus, this product is appealing if the investor would like to receive a high initial coupon (this could be done with a standard coupon bond) and at the same time expects that the interest rate will rise faster than the market predicts. Since the coupon will mature early if interest rates rise, the lower than average coupons $C _ { i } , i > 1$ do not take efect. Thus, in this case, the investor would have a coupon bond with an above average coupon. Since the investor takes the risk that he will receive lower than average coupons if interest rates do not rise, the product will be much cheaper than a standard coupon bond paying a coupon $C _ { 1 }$ and maturing early. The investor is financing the initial above average coupon by taking the risk of loosing his bet on rising interest rates. He is a risk taker. The product is appealing to the investor since he has a diferent view on the future as the market (i.e. the average). 

Exotic derivatives interpreted as an investment usually link a guaranteed high initial payment with a risky structure, which extracts the favorable case of the investor’s market view. 

An exotic derivative may both reward for taking risk as well as cover risk (in the sense of an insurance). Both interpretations jointly exist. For example the structure above has an insurance against total loss of investment. The worst case scenario is a coupon bond with below average coupons. C| 

## 12.2.1. Structured Bond, Structured Swap, Zero Structure

Exotic interest rate options mainly come in two diferent forms: as a (structured) bond or a (structured) swap. The products bond and swap are closely related. For a given (coupon) bond we may define a swap, such that the swap together with a floating rate bond replicates the coupon bond. We consider this relationship first for the trivial case of a simple coupon bond, then for the more tricky case of a zero coupon bond. All coupons may be structured coupons. 

A structured bond is a bond for which the coupons $C _ { i }$ are arbitrary complex functions of interest rates or other market observables.<sup>3</sup> In this case the coupons are called structured coupons. A corresponding swap exchanges the structured coupon payments of the bond by coupon payments of a corresponding floating rate bond, see Figure 12.1 and 12.2. Taking the swap and the floating rate bond (which just pays the current market rate on the notional) together, we may hedge the structured bond. For the values of the products in $T _ { 0 }$ we thus have $N _ { 1 } + V _ { \mathrm { s w a p } } = V _ { \mathrm { b o n d } }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/5155c3bac35a339f410f9e3bf2de57308d485e4f8b104021dd2827a2d56e79f2.jpg)



Figure 12.1.: Cashflows for a coupon bond. Left: with imaginary exchange of notionals at the end of each period; right: with efective cash-flow only.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/236964342b2de16535781f9608e6c7f4147d74f376304f00bd0df4fc8a28dfd5.jpg)



Figure 12.2.: Cashflows for a swap whose fixed leg corresponds to the coupon bond in Figure 12.1. Left: with imaginary exchange ofnotionals at the end ofeach period; right: with efective cash-flow only.


The structured bond and its (hedge-)swap are separate products, since they are often ofered by separate institutions.<sup>4</sup> 

## Zero Structures

Besides (structured) coupon paying bonds, another common type of bond is that for which the coupon is accrued instead of paid. Then, as for the zero coupon bond, there will be a single payment at maturity, see Figure 12.3, right. An accruing product is called a zero structure. A bond with accruing coupons is sometimes called a zero coupon bond. 

For an accruing zero coupon bond we may define a corresponding swap too. To do so we consider the following (equivalent) representation of the bond: At the end of each coupon pe-

<sup>4</sup> E.g. mortgage bank and investment bank. 

riod the notional and the period’s coupon is paid. The amount defines the new notional for the following period and is reinvested (this corresponds to accruing the coupon), see Figure 12.3 left. The swap is then defined such that it exchanges the structured coupon (on the various notionals) by a corresponding coupon with a given market rate. 

The swap will then allow to build up the bond’s payment at maturity using the starting notional invested at market rates, see Figure 12.4. 

Zero Coupon Bond (Accruing Structured Coupon) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/35bddc9f17a32fb03efa663ca297474080b3c8821c0b71ce4f3286813532d7b6.jpg)



Figure 12.3.: Cashflowsfor a zero coupon bond. Left: with imaginary exchange ofnotionals at the end ofeach period; right: with efective cash-flow only


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/2ecce37c21652461c8c0c23f1b700a0fad2adec9c63c175457c5a8f5adb7b81c.jpg)



Figure 12.4.: Cashflowsfor a swap whosefixed leg corresponds to the zero coupon bond in Figure 12.3 Left: with imaginary exchange ofnotionals at the end ofeach period; right: with efective cash-flow only


For the valuation in $T _ { 0 }$ we again have 

$$
N _ {1} + V _ {\mathrm{swap}} = V _ {\mathrm{bond}},\tag{12.1}
$$

where the swap is interpreted as payer swap, i.e. it pays $C _ { i } - L _ { i }$ . That Equation (12.1) holds, follows iteratively by considering a single period: The nominal $N _ { 1 }$ is invested at the market rate like a floating rate bond. The floating rate bond pays $N _ { 1 } + N _ { 1 } \cdot L _ { 1 }$ in $T _ { 2 }$ . The swap exchanges the coupon $N _ { 1 } \cdot L _ { 1 }$ for the structured coupon. Thus we have $N _ { 1 } + N _ { 1 } \cdot C _ { 1 } = : N _ { 2 }$ which is the notional $N _ { 2 }$ which is used for the same construction for the following period. 

Such a construction is especially meaningful if the zero coupon bond may be canceled at the end of a coupon period. In this case it would pay the accrued notional up to this period. For a cancelable bond the swap has the same cancellation right and is canceled simultaneously.<sup>5</sup> 

We repeat the notions structured bond and structured swap in a definition, although these definitions difer only in one minor aspect from the ones for coupon bond or swap respectively: the coupon $C _ { i }$ may be an arbitrary $\mathcal { F } _ { T _ { i + } }$ -measurable random variable: 

## Definition 141 (Structured Bond):

Let $0 = T _ { 0 } < T _ { 1 } < T _ { 2 } < . . . < T _ { n }$ denote a given tenor structure. 

For $i = 1 , \ldots , n - 1$ let $C _ { i }$ denote a (generalized) “interest $\mathrm { r a t e } ^ { \prime \prime }$ for the periods $[ T _ { i } , T _ { i + 1 } ]$ respectively. Let $C _ { i }$ be a $\mathcal { F } _ { T _ { i + 1 } }$ -measurable random variable. 

Furthermore let $N _ { i }$ denote a constant value (notional). The structured bond pays 

$$
N _ {i} \cdot C _ {i} \cdot (T _ {i + 1} - T _ {i}) + N _ {i} \cdot \left\{ \begin{array}{l l} 0 & (i \neq n) \\ 1 & (i = n - 1) \end{array} \right.
$$

in $T _ { i + 1 }$ . The value of the structured bond seen in $t < T _ { 2 }$ is 

$$
V _ {\text { Bond }} (T _ {1}, \dots , T _ {n}; t) = N (t) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\sum_ {k = 1} ^ {n - 1} \frac {N _ {k} \cdot C _ {k} \cdot (T _ {k + 1} - T _ {k})}{N (T _ {k + 1})} | \mathcal {F} _ {t}) + N _ {n - 1} \cdot P (T _ {n}; t).
$$

Definition 142 (Structured Swap (Structured Receiver Swap)): 

$\mathrm { L e t } 0 = T _ { 0 } < T _ { 1 } < T _ { 2 } < . . . < T _ { n }$ denote a given tenor structure. 

For $i = 1 , \ldots , n - 1$ let $C _ { i }$ denote a (generalized) “interest $\mathrm { r a t e } ^ { \prime \prime }$ for the periods $[ T _ { i } , T _ { i + 1 } ]$ respectively. Let $C _ { i }$ be a $\mathcal { F } _ { T _ { i + 1 } }$ -measurable random variable. 

Furthermore let $s _ { i }$ denote a constant interest rate (spread) and $N _ { i }$ a constant value (notional). The structured swap pays 

$$
X _ {i} := N _ {i} \cdot \left(C _ {i} - (L (T _ {i}, T _ {i + 1}; T _ {i}) + s _ {i})\right) \cdot (T _ {i + 1} - T _ {i}).
$$

in $T _ { i + 1 }$ . The value of the structured swap seen in $t < T _ { 2 }$ is 

$$
V _ {\text { Swap }} (T _ {1}, \dots , T _ {n}; t) = N (t) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\sum_ {k = 1} ^ {n - 1} \frac {X _ {k}}{N (T _ {k + 1})} | \mathcal {F} _ {t}).
$$

Remark 143 (Structured Coupon): By $C _ { i }$ we denote an arbitrary, generalized interest rate. In general it will be a function of $L ( T _ { k } , T _ { k + 1 } )$ with fixing date $T _ { i } ,$ , and thus even $\mathcal { F } _ { T _ { i } }$ -measurable. We allow that the generalized interest rate $C _ { i }$ depends on events within the period $[ T _ { i } , T _ { i + 1 } ]$ and requires $\mathcal { F } _ { T _ { i + 1 } }$ -measurability only. An example of $C _ { i }$ is a constant rate $C _ { i } = \mathrm { c o n s t . }$ ., the forward rate $C _ { i } = L ( T _ { i } , T _ { i + 1 } ; T _ { i } )$ , or a swap rate $C _ { i } = S ( T _ { i } , \dots , T _ { k } ; T _ { i } )$ 

Remark 144 (Zero Structure): The swap in Definition 142 is called zero structure, if the notional $N _ { i }$ if given by 

$$
N _ {i + 1} := N _ {i} \cdot C _ {i} \cdot (T _ {i + 1} - T _ {i}) \quad i = 1, \dots , n - 1.
$$

<sup>5</sup> Other arguments for this construction are reduction of default and market risk. 

Remark 145 (Structured Payer Swap / Structured Receiver Swap): The swap defined in Definition 142 is a receiver swap. A swap with reversed payments 

$$
X _ {i} := N _ {i} \cdot \left(\left(L (T _ {i}, T _ {i + 1}; T _ {i}) + s _ {i}\right) - C _ {i}\right) \cdot \left(T _ {i + 1} - T _ {i}\right)
$$

is called structured payer swap. See Definition 118. 

## 12.2.2. Bermudan Option

## Definition 146 (Bermudan):

A financial product is called Bermudan, if it has multiple exercise dates (options), i.e. there are times $T _ { i }$ at which the holder of a Bermudan may choose between diferent payments or financial products (underlyings). y 

A more formal definition of the Bermudan option, anticipating the result that the optimal exercise is to choose the maximum of the exercise and non-exercise value, is given in the following definition: 

## Definition 147 (Bermudan Option):

Let $\{ T _ { i } \} _ { i = 1 , \dots , n }$ denote a set of exercise dates and $\{ V _ { \mathrm { u n d e r l } , i } \} _ { i = 1 , \dots , n }$ a corresponding set of underlyings. The Bermudan option is the right to receive at one and only one time $T _ { i }$ the corresponding underlying $V _ { \mathrm { u n d e r l } , i }$ (with $i = 1 , \ldots , n )$ or receive nothing. 

At each exercise date $T _ { i } ,$ the optimal strategy compares the value of the product upon exercise with the value of the product upon non-exercise and chooses the larger one. Thus the value of the Bermudan is given recursively 

$$
\underbrace{V_{\text{berm}}(T_{i},\ldots,T_{n};T_{i})}_{\substack{\text{Bermudan with}\\ \text{exercise dates}\\ T_{i},\ldots ,T_{n}}}:= \max \big(\underbrace{V_{\text{berm}}(T_{i + 1},\ldots,T_{n};T_{i})}_{\substack{\text{Bermudan with}\\ \text{exercise dates}\\ T_{i + 1},\ldots ,T_{n}}},\underbrace{V_{\text{underl},i}(T_{i})}_{\substack{\text{Product}\\ \text{received upon}\\ \text{exercise in} T_{i}}}\big),
$$

where $V _ { \mathrm { b e r m } } ( T _ { n } ; T _ { n } ) : = 0$ and $V _ { \mathrm { u n d e r l } , i } ( T _ { i } )$ denotes the value of the underlying $V _ { \mathrm { u n d e r l } , i }$ at exercise date $T _ { i }$ y 

An example is given by the Bermudan swaption. Here the option holder has the right to enter a swap at several diferent times. The optimal exercise strategy chooses the maximal value from either the swap or the Bermudan with the remaining exercise dates. 

## Definition 148 (Bermudan Swaption):

Let $0 = T _ { 0 } < T _ { 1 } < T _ { 2 } < \ldots < T _ { n }$ denote a given tenor structure. The value $V _ { \mathrm { B e r m S w p t } } ( T _ { 1 } , \dots , T _ { n } ; T _ { 0 } )$ of a Bermudan swaption seen at time $T _ { 0 }$ is defined recursively by 

$$
\begin{array}{l} V _ {\text {BermSwpt}} (T _ {i}, \ldots , T _ {n}; T _ {i}) \\ := \max \big (V _ {\text {BermSwpt}} (T _ {i + 1}, \ldots , T _ {n}; T _ {i}), V _ {\text {Swap}} (T _ {i}, \ldots , T _ {n}; T _ {i}) \big), \end{array}\tag{12.2}
$$

where $V _ { \mathrm { B e r m S w p t } } ( T _ { n } ; T _ { n } ) : = 0$ and $V _ { \operatorname { S w a p } } ( T _ { i } , \dots , T _ { n } ; T _ { i } )$ denotes the value of a swap with $\mathit { f i x } .$ ing dates $T _ { i } , \ldots , T _ { n - 1 }$ and payment dates $T _ { i + 1 } , \ldots , T _ { n } ,$ , seen in $T _ { i } .$ . Furthermore, with a given numeraire ´ N and a corresponding equivalent martingale measure $\mathbb { Q } ^ { N }$ 

$$
V _ {\mathrm{BermSwpt}} (T _ {i + 1}, \ldots , T _ {n}; T _ {i}) = N (T _ {i}) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {V _ {\mathrm{BermSwpt}} (T _ {i + 1} , \ldots , T _ {n} ; T _ {i + 1})}{N (T _ {i + 1})} | \mathcal {F} _ {T _ {i}}).\tag{12.3}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/4d5d7204b6475f657a53fcb4b7f178559d4ff999ef500a2cdf0056938ee4b314.jpg)


Interpretation: The Bermudan swaption $V _ { \mathrm { B e r m S w p t } } ( T _ { n - 1 } , T _ { n } )$ is simply a swaption (option on a swap) and since the swap has only a single period $[ T _ { n - 1 } , T _ { n } ]$ it is actually a caplet. The Bermudan swaption $V _ { \mathrm { B e r m S w p t } } ( T _ { n - 2 } , T _ { n - 1 } , T _ { n } )$ is an option which allows a choice in time $T _ { n - 2 }$ between a swaption (with later exercise date) 

or a (longer) swap. Thus it is an option on an option. Iteratively the Bermudan swaption is an option on an option (on an option, etc.). 

Taking the underlying swap as the defining object, we see that the Bermudan swaption $V _ { \mathrm { B e r m S w p t } } ( T _ { 1 } , \dots , T _ { n } )$ can also be interpreted as an option either to enter at times $T _ { 1 } , \ldots , T _ { n - 1 }$ a swap with remaining periods up to $T _ { n } ,$ , or to wait. Options with multiple exercise times are called Bermudan. Options with a single exercise time are called European. C| 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/28636f20f9c8efa333cd16e745362a262add6bf8d8f2069e5866542ff43dba0c.jpg)



Figure 12.5.: Bermudan Swaption


Remark 149 (Bermudan Swaption): It is key to the evaluation of the Bermudan swaption that by Equation (12.3) we have at each exercise date $T _ { i }$ an evaluation of a derivative product. For this the conditional expectation has to be calculated. Depending on the model and the implementation, the calculation of conditional expectations may be non-trivial. In Chapter 15 we give an in-depth discussion on how to calculate a conditional expectation in a path simulation (Monte-Carlo simulation). 

## 12.2.3. Bermudan Callable and Bermudan Cancelable

We will now define a product class that generalizes the structure of a Bermudan swaption. 

Definition 150 (Bermudan Callable Structured Swap<sup>6</sup>): 

Let $0 = T _ { 0 } < T _ { 1 } < T _ { 2 } < . . . < T _ { n }$ denote a given tenor structure. 

For $i = 1 , \ldots , n - 1$ let $C _ { i }$ denote a (generalized) “interest rate” for the periods $[ T _ { i } , T _ { i + 1 } ]$ respectively. Let $C _ { i }$ be $\mathrm { ~ a ~ } \mathcal { F } _ { T _ { i + 1 } }$ -measurable random variable. 

Furthermore let s denote a constant interest rate (spread), $N _ { i }$ a constant value (notional) and 

$$
X _ {i} := N _ {i} \cdot (C _ {i} - (L (T _ {i}, T _ {i + 1}) + s _ {i})) \cdot (T _ {i + 1} - T _ {i}).
$$

Let $V _ { \mathrm { u n d e r l } } ( T _ { i } , \dots , T _ { n } ; T _ { i } )$ denote the value of the product paying $X _ { k }$ in $T _ { k + 1 }$ for $k = i , \ldots , n - 1$ seen in $T _ { i }$ . If N denotes a numeraire and´ $\mathbb { Q } ^ { N }$ a corresponding equivalent martingale measure, 

<sup>6</sup> Compare [85]. 

then 

$$
V _ {\text { underl }} (T _ {i}, \dots , T _ {n}; T _ {i}) = N (T _ {i}) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\sum_ {k = i} ^ {n - 1} \frac {X _ {k}}{N (T _ {k + 1})} | \mathcal {F} _ {T _ {i}}).\tag{12.4}
$$

The value of a Bermudan callable swap with structured leg $C _ { i } { } ^ { 7 }$ is recursively defined by 

$$
\begin{array}{l} V _ {\text { BermCall }} (T _ {i}, \ldots , T _ {n}; T _ {i}) \\ := \max \big (V _ {\text { BermCall }} (T _ {i + 1}, \ldots , T _ {n}; T _ {i}), V _ {\text { underl }} (T _ {i}, \ldots , T _ {n}; T _ {i}) \big), \end{array}\tag{12.5}
$$

where $V _ { \mathrm { B e r m C a l l } } ( T _ { n } ; T _ { n } ) : = 0$ and 

$$
V _ {\text { BermCall }} (T _ {i + 1}, \dots , T _ {n}; T _ {i}) = N (T _ {i}) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {V _ {\text { BermCall }} (T _ {i + 1} , \dots , T _ {n} ; T _ {i + 1})}{N (T _ {i + 1})} | \mathcal {F} _ {T _ {i}}).\tag{12.6}
$$

Remark 151 (Bermudan Callable, structured Leg): For $C _ { i } = S _ { i } =$ const the product defined in Definition 150 is a Bermudan swaption. 

The payments (cash flows) $X _ { i }$ consist of some part $N _ { i } \cdot C _ { i } \cdot ( T _ { i + 1 } - T _ { i } )$ which is called the structured $l e g$ and another part $N _ { i } \cdot ( L ( T _ { i } , T _ { i + 1 } ) + s _ { i } ) \cdot ( T _ { i + 1 } - T _ { i } )$ which is called thefloating leg. 

The underlying $V _ { \mathrm { u n d e r l } } ( T _ { i } , \dots , T _ { n } )$ is a swap swapping the rate $C _ { i }$ against $L ( T _ { i } , T _ { i + 1 } ) + s _ { i }$ , with fixing dates $T _ { i } , \ldots , T _ { n - 1 }$ and payment dates $T _ { i + 1 } , \dots , T _ { n }$ 

To evaluate a Bermudan option we need to calculate at most two conditional expectations (12.4), (12.6) at each exercise time $T _ { i } .$ . Under the assumption of optimal exercise these two values are linked by (12.5), going backward from exercise date to exercise date. In Chapter 15 we give an in-depth discussion of the calculation of conditional expectation in a path simulation (Monte-Carlo simulation). 

The Bermudan swaption (or a Bermudan callable) allows an (eventually structured) swap to be entered into at one single time the of predefined times $T _ { i }$ . In contrast to this, the Bermudan cancelable swap allows the cancelation a swap at one single time of the predefined times $T _ { i }$ 

Definition 152 (Bermudan Cancelable Swap): 

With the notation from Definition 150 let 

$$
V _ {\text { coupons }} (T _ {i}; T _ {i}) = N (T _ {i}) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {X _ {i}}{N (T _ {k + 1})}   | \mathcal {F} _ {T _ {i}}).
$$

the value of the coupon payments (cash flows) for the period $[ T _ { i } , T _ { i + 1 } ]$ , seen in $T _ { i \cdot }$ 

The value of a Bermudan Cancelable with structured leg $C _ { i }$ is recursively defined by 

$$
\begin{array}{l} V _ {\text { BermCancel}} (T _ {i}, \ldots , T _ {n}; T _ {i}) \\ := \max \big (V _ {\text { coupons }} (T _ {i}; T _ {i}) + V _ {\text { BermCancel }} (T _ {i + 1}, \ldots , T _ {n}; T _ {i})  ,   0 \big), \end{array}
$$

where $V _ { \mathrm { B e r m C a n c e l } } ( T _ { n } ; T _ { n } ) : = 0$ and 

$$
V _ {\text { BermCancel }} (T _ {i + 1}, \dots , T _ {n}; T _ {i}) = N (T _ {i}) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {V _ {\text { BermCancel }} (T _ {i + 1} , \dots , T _ {n} ; T _ {i + 1})}{N (T _ {i + 1})} | \mathcal {F} _ {T _ {i}}).
$$

Remark 153 (Bermudan Cancelable): With the notation from Definition 150 and 152 we have 

$$
V _ {\text { BermCancel }} (T _ {i}, \dots , T _ {n}; T _ {i}) = V _ {\text { underl }} (T _ {i}, \dots , T _ {n}; T _ {i}) + V _ {\text { BermCallPayer }} (T _ {i}, \dots , T _ {n}; T _ {i}),\tag{12.7}
$$

where $V _ { \mathrm { B e r m C a l l P a y e r } }$ denotes a Bermudan callable with reversed sign in the underlying. The right to cancel the structured swap $V _ { \mathrm { u n d e r l } }$ corresponds to the right to enter such a structured swap with reversed cash-flow. 

Likewise we have 

$$
V _ {\text { BermCall }} \left(T _ {i}, \dots , T _ {n}; T _ {i}\right) = V _ {\text { underl }} \left(T _ {i}, \dots , T _ {n}; T _ {i}\right) + V _ {\text { BermCancelPayer }} \left(T _ {i}, \dots , T _ {n}; T _ {i}\right),\tag{12.8}
$$

where $V _ { \mathrm { B e r m C a n c e l P a y e r } }$ denotes a Bermudan cancelable with reversed sign in the underlying. 

From this we conclude that the problem of evaluating a Bermudan cancelable corresponds to the problem of evaluating a Bermudan callable - and vice versa. 

Remark 154 (Bermudan Callable): Our definition of a Bermudan option is a general one: for each exercise date the corresponding underlying can be specified arbitrarily. The Bermudan callable is a special variant of a Bermudan option, where the underlyings share the same cash-flow after exercise.<sup>8</sup> The Bermudan callable is the right to enter a financial product at some later time. The Bermudan cancelable is the right to terminate a financial product at some later time. Bermudan callable and Bermudan cancelable are counterparts in the sense of Equation (12.7). 

For (structured) bonds it is usually the case that the issuer (i.e. the party that pays the coupons) has the right to cancel the bond.<sup>9</sup> Due to the relationship (12.7) it is the case that the issuer of a bond having the right to cancel the issued bond essentially has a callable bond. Therefore the use of the words callable and the call right are often used where our definition would seem to point to a cancelable contract. 

## 12.2.4. Compound Options

A compound option is an option on an option. Popular are a European call option on a European call option, a call on a put, a put on a call and a put on a put. The compound option is closely related to the Bermudan option with two exercise dates. The compound option may be viewed as a special variant of a Bermudan option. 

As for the Bermudan option, the evaluation of a compound option requires the evaluation of an option at a future time (the exercise date of the first option). The methods used for the pricing of Bermudan options can thus be applied to the evaluation of compound options. 

## 12.2.5. Trigger Products

For a Bermudan options and a Bermudan cancelable the exercise criterion is given by optimal exercise: The option holder chooses the maximum value. Thus the recursive definition of the product value uses the maximum function on the values of the two alternatives non-exercise and exercise. For a trigger product the exercise is given by some criterion, the trigger, which does not necessarily represent an optimal exercise. An example of such a product is the auto cap, which we will define in Section 12.2.6.4 below, or the following target redemption note. 

## 12.2.5.1. Target Redemption Note

## Definition 155 (Target Redemption Note):

Let $0 = T _ { 0 } < T _ { 1 } < T _ { 2 } < . . . < T _ { n }$ denote a given tenor structure. 

For $i = 1 , \ldots , n - 1$ let $C _ { i }$ denote a (generalized) “interest rate” for the periods $[ T _ { i } , T _ { i + 1 } ]$ respectively. Let $C _ { i }$ be a $\mathcal { F } _ { T _ { i + 1 } }$ -measurable random variable. 

Furthermore let $N _ { i }$ denote a constant value (notional). A target redemption note pays 

$$
N _ {i} \cdot X _ {i} \qquad \mathrm{in} \qquad T _ {i + 1}
$$

with 

$$
\begin{array}{l} X _ {i} := \left\{ \begin{array}{l l} C _ {1} & \text { for } i = 1, \\ \min (C _ {i}, K - \sum_ {k = 1} ^ {i - 1} C _ {k}) & \text { for } i > 1 \end{array} \right. \quad \text { structured   coupon } \\ + \left\{ \begin{array}{l l} 1 & \text { for } \sum_ {k = 1} ^ {i - 1} C _ {k} <   K <   = \sum_ {k = 1} ^ {i} C _ {k} \text { or } i = n, \\ 0 & \text { else. } \end{array} \right. \quad (\text { redemption }) \\ + \left\{ \begin{array}{l l} \max (0, K - \sum_ {k = 1} ^ {i} C _ {k}) & \text { for } i = n \\ 0 & \text { else. } \end{array} \right. \quad (\text { target   coupon   guarantee }). \end{array}
$$

Remark 156 (Target Redemption Note Coupon): The rule that defines the coupon $C _ { i }$ in Definition 155 may vary and Definition 155 is only the framework of the product. With a coupon, e.g., like 

$$
C _ {i} = K - a \cdot L _ {i} \cdot (T _ {i + 1} - T _ {i}) \qquad \mathrm{for} i > 1.\tag{12.9}
$$

the product is also called variable maturity inversefloater (VMIF). We will consider structured coupons in Section 12.2.6. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/f4edb05a8d21ae0e1c562db58387962fc230b7fc06ad18000ace25661c49eb7c.jpg)


Interpretation: The holder of a target redemption note receives the coupon $C _ { i }$ as long as the sum of the coupons has reached $K ,$ the target coupon. If the accumulated coupon exceeds the target coupon $\textstyle ( \sum _ { k = 1 } ^ { i } C _ { k } > = K )$ , then the diference between the target coupon and the notional is paid. After this no coupon 

payments will be made. The structure is canceled if the target coupon has been reached. If the target coupon has not been reached over the full life time of the product, then the diference between the target coupon and the notional is paid at maturity. 

Thus, the target redemption note guarantees the payment of a coupon $K$ and the redemption of the notional. What is uncertain is the time of payment and the maturity, and thus the yield of the product. The yield of the product depends on when the condition 

$$
\sum_ {k = 1} ^ {i} C _ {k} = K \quad \text { and } \quad \sum_ {k = 1} ^ {i - 1} C _ {k} <   K\tag{12.10}
$$

is fulfilled. 

It is normal to have an above average initial coupon $C _ { 1 }$ . The life time of the product varies between $T _ { 2 }$ and $T _ { n } ,$ giving yields between $K / T _ { 2 }$ and $K / T _ { n } .$ An investor would buy this product if he assumed that the condition (12.10) would be fulfilled early, such that the yield of the product (is expected to be) above average. 

An example of a target redemption note, actually ofered in 2004, is 

$$
C _ {i} = 7.5 \% - 2 \cdot L _ {i} \cdot (T _ {i + 1} - T _ {i}) \quad \text { for } i > 1.
$$

Here the option holder profits from the product if the interest rates $L _ { i }$ decline faster than expected (and thus the product will be redeemed early). C| 

## 12.2.6. Structured Coupons

In the previous definitions we have defined the structured bond (Definition 141), the structured swap (Definition 142), the Bermudan option (Definition 150), the Bermudan cancelable (Definition 152) and the Target Redemption Note (Definition 155) without specifying the coupons $C _ { i } .$ We now refine our definitions by defining some of the most common structured coupons $C _ { i } .$ In the respective definitions we only give the characteristic that describes the coupon. The characteristics defined in the following exist for bonds and swaps and for Bermudan callable and Bermudan cancelables alike. For example, we define a coupon of a CMS spread product and the name of the corresponding Bermudan callable swap as a Bermudan callable CMS spread swap. 

## 12.2.6.1. Capped, Floored, Inverse, Spread, CMS

## Definition 157 (Capped Floater):

A product as in Definition 141, 142, 150 or 152 with 

$$
C _ {i} := \min (L (T _ {i}, T _ {i + 1}) + s _ {i}, c _ {i})
$$

is called a Capped Floater. Here $c _ { i }$ denotes a constant (cap). 

## Definition 158 (Floored Floater):

A product as in Definition 141, 142, 150 or 152 with 

$$
C _ {i} := \max (L (T _ {i}, T _ {i + 1}) + s _ {i}, f _ {i})
$$

is called a Floored Floater. Here $f _ { i }$ denotes a constant (floor). 

## Definition 159 (Inverse Floater):

A product as in Definition 141, 142, 150 or 152 with 

$$
C _ {i} = \min \left(\max \left(k _ {i} - L (T _ {i}, T _ {i + 1}), f _ {i}\right), c _ {i}\right)
$$

is called an Inverse Floater. Here $f _ { i } < c _ { i }$ (Floor, Cap) and $k _ { i }$ are constants. 

## Definition 160 (Capped CMS Floater):

A product as in Definition 141, 142, 150 or 152 with 

$$
C _ {i} := \min (S _ {i, i + m} + s _ {i}, c _ {i}),
$$

where $s _ { i } , c _ { i }$ denote constants (Spread, Cap) and $\boldsymbol { S } _ { i , i + m } = \boldsymbol { S } ( T _ { i } , \dots , T _ { i + m } )$ denotes a swap rate as in Definition 122, is called a Capped CMS<sup>10</sup> Floater. The rate $S _ { i , i + m }$ is called constant maturity 

<sup>10</sup> CMS stands for Constant Maturity Swap, i.e. the maturity of the underlying swap relative to the swap start $( T _ { i + m } -$ T ) is constant. For simplicity we assume here that the tenor structure is equidistant. 

swap rate (CMS) since the maturity relative to the period start $T _ { i } ,$ is constant $( T _ { i + m } - T _ { i }$ is constant, i.e. independent of i), assuming an equidistant tenor structure. y 

## Definition 161 (Inverse CMS Floater):

A product as in Definition 141, 142, 150 or 152 with 

$$
C _ {i} = \min \left(\max \left(k _ {i} - S _ {i, i + m}, f _ {i}\right), c _ {i}\right),
$$

where $k _ { i } , f _ { i } , c _ { i }$ denote constants (Strike, Floor, Cap) and $\boldsymbol { S } _ { i , i + m } = \boldsymbol { S } ( T _ { i } , \dots , T _ { i + m } )$ denotes a swap rate as in Definition 122, is called an Inverse CMS Floater. y 

## Definition 162 (CMS Spread):

A product as in Definition 141, 142, 150 or 152 with 

$$
C _ {i} = \min \left(\max \left(S _ {i, i + m _ {1}} ^ {1} - S _ {i, i + m _ {2}} ^ {2}, f _ {i}\right), c _ {i}\right),
$$

where $f _ { i } , \ c _ { i }$ denote constants (Floor, Cap) and $\begin{array} { r c l } { S _ { i , i + m _ { 1 } } } & { = } & { S ( T _ { i } , . . . , T _ { i + m _ { 1 } } ) , S _ { i , i + m _ { 2 } } } & { = } \end{array}$ $S ( T _ { i } , \ldots , T _ { i + m _ { 2 } } )$ denotes a swap rate as in Definition 122, is called a CMS Spread. y 

## 12.2.6.2. Range Accruals

## Definition 163 (Range Accrual):

Let $t _ { i , k } \in [ T _ { i } , T _ { i + 1 } )$ denote given observation points for the period $[ T _ { i } , T _ { i + 1 } )$ . Furthermore let $K _ { i }$ and $b _ { i } ^ { l } < b _ { i } ^ { h }$ denote given interest rates (constants). A product as in Definition 141, 142, 150 or 152 with 

$$
C _ {i} := K _ {i} \cdot \frac {1}{n _ {i}} \sum_ {k = 1} ^ {n _ {i}} \mathbf {1} _ {[ b _ {i} ^ {l}, b _ {i} ^ {b} ]} (L (t _ {i, k}, t _ {i, k} + \Delta T _ {i}; t _ {i, k})) \quad \text { in } T _ {i + 1}.
$$

is called a Range Accrual. Here $\Delta T _ { i } : = T _ { i + 1 } - T _ { i }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/9cf2f05f9e913527f9e6d955af4dc5e424d988a863bd64856da903a207dee74e.jpg)


Interpretation: The interval $[ b _ { i } ^ { l } , b _ { i } ^ { h } ]$ describes an interest rate corridor. It is calculated how often the reference rate $L ( t , t + \Delta T _ { i } ; t )$ stays within this corridor at the times $t _ { i , k }$ . The product pays the corresponding fractional amount of the rate $K _ { i }$ at the end of the period. 

Since the interest rate corridor may be chosen as a function of the period i, the product makes it possible to profit from a specific evolution of the rate. C| 

## 12.2.6.3. Path Dependent Coupons

## Definition 164 (Snowball / Memory):

A product as in Definition 141, 142, 150 or 152 with 

$$
C _ {i} = \min \left(\max \left(C _ {i - 1} + X _ {i}, f _ {i}\right), c _ {i}\right),
$$

is called Snowball, where $X _ { i }$ is some coupon as in Definition 157-163 and $f _ { i } , c _ { i }$ denote constants (Floor, Cap) and $C _ { i - 1 }$ denotes the coupon of the previous periods with $C _ { 0 } : = 0$ y 

Example: A coupon 

$$
C _ {i} = \min \left(\max \left(C _ {i - 1} + k _ {i} - L (T _ {i}, T _ {i + 1}), f _ {i}\right), c _ {i}\right)
$$

is called an inverse floater memory. 

Definition 165 (Power Memory): 

With the notation from the previous Definition 164 the coupon 

$$
C _ {i} = \min \left(\max \left(\alpha C _ {i - 1} + X _ {i}, f _ {i}\right), c _ {i}\right),
$$

is called a Power Memory $( \mathrm { f o r } \alpha \neq 1 )$ 

Remark 166 (Snowball, Path Dependency): The snowball is called a path-dependent product, since its coupon depends on the previous coupon, i.e. on the history. 

Definition 167 (Ratchet-Cap): 

The Ratchet Cap pays in $T _ { i + 1 }$ 

$$
X _ {i} = N \cdot \max \left(L (T _ {i}, T _ {i + 1}; T _ {i}) - K _ {i}, 0\right) \cdot (T _ {i + 1} - T _ {i})
$$

for times $T _ { 1 } , \ldots , T _ { n } .$ , where 

$$
K _ {i} := \min \left(K _ {i - 1} + R, L (T _ {i}, T _ {i + 1}; T _ {i})\right) \quad \text { for } i > 1
$$

and $K _ { 1 } , R$ denote constants (strike and Ratchet), $L ( T _ { i } , T _ { i + 1 } ; T _ { i } )$ denote the forward rate (LIBOR) and N denotes the notional. y 

Remark 168 (Ratchet Cap): The ratchet cap has an automatic adjustment of the strike $K _ { i } .$ Since the adjustment depends on past realizations, the ratchet cap is a path-dependent product. 

## 12.2.6.4. Flexi Cap

Theflexi cap comes in two variants: As an auto cap with a simple (automatic) exercise criterion and as an chooser cap with an assumed optimal exercise (like for the Bermudan). Both caps have in common that the maximum number of exercises is limited. 

## Definition 169 (Auto Cap):

Let $n _ { \mathrm { m a x E x } } \in \mathbb { N } .$ . An Auto Cap pays in $T _ { i + 1 }$ 

If $| \{ j : j < i$ und $X _ { j } > 0 \} \vert < n _ { \mathrm { m a x E x } } \backslash$ 

$$
X _ {i} := N \cdot \max \left(L (T _ {i}, T _ {i + 1}; T _ {i}) - K _ {i} , 0\right) \cdot (T _ {i + 1} - T _ {i})
$$

or else: 

$$
X _ {i} := 0
$$

for times $T _ { 1 } , \ldots , T _ { n } ,$ , where $K _ { i }$ denotes the strike rate, $L ( T _ { i } , T _ { i + 1 } ; T _ { i } )$ denotes the forward rate (LIBOR) and N denotes the notional. The auto cap pays in the same way as a normal cap as long as the number of past (positive) payments is below $n _ { \mathrm { { m a x E x } } } .$ y 

Definition 170 (Chooser-Cap): Let $n _ { \mathrm { m a x E x } }$ ∈ N. A Chooser Cap pays in $T _ { i + }$ 1 

$\operatorname { I f } | \{ j : j < i$ and $X _ { j } > 0 \} \vert < n _ { \mathrm { m a x E x } }$ and payment is chosen: 

$$
X _ {i} := N \cdot \max \left(L (T _ {i}, T _ {i + 1}; T _ {i}) - K _ {i}, 0\right) \cdot (T _ {i + 1} - T _ {i})
$$

otherwise: 

$$
X _ {i} := 0
$$

for times $T _ { 1 } , \ldots , T _ { n } ,$ , where $K _ { i }$ denotes the strike rate, $L ( T _ { i } , T _ { i + 1 } ; T _ { i } )$ denotes the forward rate (LIBOR) and N denotes the notional. y 

Remark 171 (Auto Cap): The auto cap is a path-dependent product, since at a future time the number of exercises allowed depends on the history. It is also a trigger product, since the exercise is not optimal, but triggered by a simple trigger. The corresponding optimal exercise is given by the chooser cap. 

Remark 172 (Chooser Cap (Backward Algorithm)): Since the option holder chooses to exercise optimally, we have that the value $V _ { \mathrm { C h o o s e r } } ^ { ( \breve { n } _ { \mathrm { m a x E x } } , T _ { 1 } , T _ { n } ) } ( T _ { 0 } )$ of the chooser cap is given by 

$$
V _ {\text { Chooser }} ^ {(n _ {\text { Ex }}, T _ {i}, T _ {n})} (T _ {i}) = \max \left(X _ {i} + V _ {\text { Chooser }} ^ {(n _ {\text { Ex }} - 1, T _ {i + 1}, T _ {n})} (T _ {i})\right), V _ {\text { Chooser }} ^ {(n _ {\text { Ex }}, T _ {i + 1}, T _ {n})} (T _ {i})),
$$

where 

$$
X _ {i} := N \cdot \max \left(L (T _ {i}, T _ {i + 1}; T _ {i}) - K _ {i}, 0\right) \cdot (T _ {i + 1} - T _ {i})
$$

and 

$$
V _ {\text { Chooser }} ^ {(n _ {\text { Ex }}, T _ {n}, T _ {n})} (T _ {n}) = 0 \qquad , \qquad V _ {\text { Chooser }} ^ {(0, T _ {i}, T _ {n})} (T _ {i}) = 0,
$$

where $V _ { \mathrm { C h o o s e r } } ^ { ( n _ { \mathrm { E x } } , T _ { i } , T _ { n } ) } ( T _ { k } )$ denotes the value of a chooser cap with at most $n _ { \mathrm { E x } }$ exercises in $T _ { i } , \ldots , T _ { n }$ seen in $T _ { k }$ 

Remark 173 (Chooser Cap as Bermudan): A chooser cap with $n _ { \mathrm { m a x E x } } = 1$ exercises is a Bermudan cap. 

## 12.2.7. Shout Options

## Definition 174 (Shout Option):

Assume that a financial product pays an Underlying $S ( t ^ { * } )$ at time T, i.e. t<sup>∗</sup> is the fixing date and T the payment date. The owner of the financial product has a shout right on the underlying, if the holder of the right can determine once at any time t with $T _ { 1 } \leq t \leq T _ { 2 } \leq T$ the fixing date $t ^ { * }$ as $t ^ { * } : = t .$ . The holder determines by shouting that the underlying should be fixed. y 

Remark 175: While for an American option or a Bermudan option, e.g. on $S ( t ) - K$ , the fixing date and the payment date are both determined upon exercise, i.e. $S ( t ^ { * } ) - K$ is paid in $t ^ { * }$ , for a Shout option the fixing date is determined upon exercise, while the payment date stays predefined. 

Theorem 176 (Value of a Shout Right)): A shout right on a convex function of a sub martingale (under terminal measure) is worthless. 

Proof: Let T denote the payment date of $f ( S ( t ) )$ , where t is fixed as $t = t ^ { * }$ by shouting. For the chosen numeraire´ N we assume $N ( T ) = 1$ (terminal measure). Let f be convex and S a sub-martingale under $\mathbb { Q } ^ { N }$ . Then we have: 

$$
S (t) \leq \mathrm{E} (S (T _ {2}) | \mathcal {F} _ {t})
$$

(sub-martingale property) 

$$
f (S (t)) \leq \mathrm{E} (f (S (T _ {2})) | \mathcal {F} _ {t})
$$

(Jensen’s inequality) 

$$
\mathrm{E} (f (S (t)) \mid \mathcal {F} _ {T _ {0}}) \leq \mathrm{E} (f (S (T _ {2})) \mid \mathcal {F} _ {T _ {0}})
$$

$$
\mathrm{E} \left(\frac {f (S (t))}{N (T)} \mid \mathcal {F} _ {T _ {0}}\right) \leq \mathrm{E} \left(\frac {f (S (T _ {2}))}{N (T)} \mid \mathcal {F} _ {T _ {0}}\right)
$$

(tower law) 

(terminal measure) 

Thus, to maximize the value the option holder will always exercise the shout right at $t ^ { * } = T _ { 2 }$ | 

## 12.3. Product Toolbox

The terms used in the previous section, like Capped, Inverse, Ratchet, etc., describe properties of the payof function. In practice the terms are used less strictly and the name of a product corresponds to its mathematical definition only loosely. Here marketing aspects are more important. Key product features are, nevertheless, indicated by the name of a product. 

The following Table 12.3 gives a rough idea of some of the most common terms used to denote properties of the product or payof function. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/84af9d077119f6ef3ed153103adc77725dfaad33583f2f1fcdfdee44de92083c.jpg)


Experiment: At http://www.christian-fries.de/finmath/ applets/LMMPricing.html several interest rate products can be priced, among them a cancelable swap. The model used is a LIBOR Market Model implemented in a Monte-Carlo simulation. C| 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/95c3c373b5a4b9d49f8d38d69c9c9ed93d847a8a5c79c4a69df519e5269db8d5.jpg)


properties. 

Further Reading: An overview of exotic derivatives can be obtained from the customer information service of some investment banks or the term sheets of the products. They contain descriptions of the product and definitions of the payofs, similar to the definitions in this chapter, as well as a short discussion of product 

Zhang’s book, [43], presents some of the most important exotic options, in particular, exotic equity options. C| 

<table><tr><td>Attribute</td><td>Product Property</td></tr><tr><td>Bond (aka. Note)</td><td>Receive coupons. At maturity receive the notional.See Definition 141</td></tr><tr><td>Swap</td><td>Exchange coupons (usually against float).See Definition 142</td></tr><tr><td>Bermudan Option</td><td>Receive an underlying at one of multiple exercise dates.See Definition 146</td></tr><tr><td>Bermudan Cancelable</td><td>Cancel product (e.g. bond or swap) at one of multiple cancelation dates. See Definition 152</td></tr><tr><td>Target Redemption</td><td><eq>\min(C_i, K - \sum_{k=1}^{i-1} C_k)</eq> with cancelation and notional redemption at (12.10) (trigger). See Definition 155</td></tr><tr><td>Chooser</td><td>Receive an underlying at some of multiple exercise dates.See Definition 170</td></tr><tr><td colspan="2"></td></tr><tr><td>Attribute</td><td>Payoff Function</td></tr><tr><td>LIBOR / Floater</td><td><eq>C_i = L(T_i, T_{i+1}; T_i)</eq></td></tr><tr><td>CMS</td><td><eq>C_i</eq> is swap rate with constant time to maturity</td></tr><tr><td>Capped</td><td><eq>\min(C_i - K_i, c_i)</eq></td></tr><tr><td>Floored</td><td><eq>\max(C_i - K_i, f_i)</eq></td></tr><tr><td>Inverse</td><td><eq>K_i - C_i</eq></td></tr><tr><td>Spread</td><td><eq>C_i^1 - C_i^2</eq></td></tr><tr><td>Ratchet</td><td><eq>K_i = \min(K_{i-1} + R, C_i)</eq></td></tr><tr><td>Snowball</td><td><eq>C(T_i) = C(T_{i-1}) + K_i - L_i(T_i)</eq></td></tr><tr><td>Range Accrual</td><td><eq>K_i \cdot \frac{1}{n_i} \sum_{k=1}^{n_i} \mathbf{1}_{[b_i&#x27;, b_i^h]} (L(t_{i,k}, t_{i,k} + \Delta T_i; t_{i,k}))</eq></td></tr></table>


Table 12.3.: Product Toolbox: Common attributes and their representation in product property and payoffunction.


Part IV. 

# Discretization of Stochastic Differential Equations and Numerical Valuation Methods

## Motivation and Overview - Part IV

In Chapter 4 we presented the Black-Scholes Model of a stock S and a riskless account B 

$$
\begin{array}{l} \mathrm{d} S (t) = \mu^ {\mathbb {P}} (t) S (t) \mathrm{d} t + \sigma (t) S (t) \mathrm{d} W ^ {\mathbb {P}} (t), \\ \mathrm{d} B (t) = r (t) B (t) \mathrm{d} t. \end{array}
$$

In Chapter 10 we presented the corresponding Black Model for a forward interest rate $L _ { 1 } =$ $L ( T _ { 1 } , T _ { 2 } )$ 

$$
\mathrm{d} L _ {1} (t) = \mu^ {\mathbb {P}} (t) L _ {1} (t) \mathrm{d} t + \sigma (t) L _ {1} (t) \mathrm{d} W ^ {\mathbb {P}} (t), \quad \sigma (t) \geq 0.
$$

Using these models we could derive analytic pricing formulas for the corresponding European options. An obvious generalization of these models consists in modeling multiple stocks, e.g. 

$$
\begin{array}{l} \mathrm{d} S _ {i} (t) = \mu_ {i} ^ {\mathbb {P}} (t) S _ {i} (t) \mathrm{d} t + \sigma_ {i} (t) S _ {i} (t) \mathrm{d} W _ {i} ^ {\mathbb {P}} (t), \\ \mathrm{d} B (t) = r (t) B (t) \mathrm{d} t, \end{array}
$$

respectively a model for multiple forward rates, e.g. $L _ { i } = L ( T _ { i } , T _ { i + 1 } )$ for $T _ { 1 } < T _ { 2 } < . .$ with $\mathrm { e . g }$ 

$$
\mathrm{d} L _ {i} (t) = \mu_ {i} ^ {\mathbb {P}} (t) L _ {i} (t) \mathrm{d} t + \sigma_ {i} (t) L _ {i} (t) \mathrm{d} W _ {i} ^ {\mathbb {P}} (t), \quad \sigma (t) \geq 0.\tag{12.11}
$$

The model (12.11) is called the LIBOR Market Model. 

Such models may then be used for the evaluation of complex derivatives, e.g. a spread option, where the payout depends on two or more forward rates. The pricing, i.e. the calculation of the expectation $\mathrm { E } ^ { \mathbb { Q } ^ { N } } ( \frac { V ( T ) } { N ( T ) } | \mathcal { F } _ { 0 } )$ , where N is a chosen numeraire and´ $\mathbb { Q } ^ { \bar { N } }$ is a corresponding martingale measure, often requires a numerical method, e.g. a Monte-Carlo integration 

$$
\mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {V (T)}{N (T)} | \mathcal {F} _ {0}) \approx \frac {1}{n} \sum_ {i = 1} ^ {n} \frac {\tilde {V} (T , \omega_ {i})}{\tilde {N} (T , \omega_ {i})}
$$

for a sampling $\omega _ { 1 } , \ldots , \omega _ { n }$ . Here, $\tilde { V }$ and $\tilde { N }$ denote approximations of V and N respectively, since the corresponding Monte-Carlo samples are generally generated for an approximating model, namely a time-discrete model. 

In Chapter 13 we start by examining the approximation of time-continuous stochastic processes through time-discrete stochastic processes. We then consider the approximation of the random variables by a Monte-Carlo simulation or a discretization of the state space. 

These discretizations allow us to calculate (approximate) expectations and thus derivative prices. It turns out that within the discrete set-up some calculations are dificult. In a Monte-Carlo simulation the calculation of a conditional expectation is non-trivial. A conditional expectation may be required in the pricing of Bermudan products, see Chapter 15. In a discretization of a state space the calculation of path-dependent quantities is non-trivial. Path dependent quantities appear in path-dependent options, see Chapter 16. 

The treatment of complex models, like the LIBOR Market Model, will be given in Part V. 

# Discretization of time and state space

In this chapter we present methods for discretization and implementation of Ito stochasticˆ processes. We give an integrated presentation of “path simulation” (Monte-Carlo simulation) and “lattice methods” (e.g. trees). Finally, we show how both methods can be combined, see Section 13.4. 

Throughout our discussion of the discretization and implementation we will repeat some of the terms from Chapter 2, e.g. path, <sub>σ</sub>-algebra, filtration, process and $\mathcal { F } _ { t } .$ -adapted. Thus, this chapter will also serve as an illustration of some of the mathematical concepts from Chapter 2. 

The discretization and implementation should not be seen as a minor additional step after the mathematical analysis and it should not be under estimated. The discretization and implementation allow us a second look, possibly providing further insights into a model. 

In Figure 13.1 we give an overview of the steps involved in the discretization and implementation of Ito processes.ˆ 

## 13.1. Discretization of Time: The Euler and the Milstein Scheme

As a first step we shall consider the discretization of time and present the Euler scheme and Milstein scheme. 

## 13.1.1. Definitions

Definition 177 (Euler Scheme): 

Given an Ito processˆ 

$$
\mathrm{d} X (t) = \mu (t, X (t)) \mathrm{d} t + \sigma (t, X (t)) \mathrm{d} W (t),
$$

and a time discretization {t $\mid i = 0 , \ldots , n \}$ with $0 = t _ { 0 } < \ldots < t _ { n } .$ , then the time-discrete stochastic process X<sup>˜</sup> defined by 

$$
\tilde {X} (t _ {i + 1}) = \tilde {X} (t _ {i}) + \mu (t _ {i}, \tilde {X} (t _ {i})) \Delta t _ {i} + \sigma (t _ {i}, \tilde {X} (t _ {i})) \Delta W (t _ {i})
$$

is called an Euler scheme of the process X (where $\Delta t _ { i } : = t _ { i + 1 } - t _ { i }$ and $\Delta W ( t _ { i } ) : = W ( t _ { i + 1 } ) - W ( t _ { i } ) )$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/bbdd273ee35d660459962485cbeda5005c90fb6184b9c0e23595b291a8ff09dc.jpg)



Figure 13.1.: Discretization and Implementation ofItˆo Processes


C| 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/96b17d7e6968fcbb8521799a433ebc7a08c724bc5ccc80d6cf8321f0da20e700.jpg)


Interpretation (Euler discretization): The Euler scheme derives from a simple integration rule. From the definition of the Ito process we haveˆ 

$$
X \left(t _ {i + 1}\right) = X \left(t _ {i}\right) + \int_ {t _ {i}} ^ {t _ {i + 1}} \mu (t, X (t)) \mathrm{d} t + \int_ {t _ {i}} ^ {t _ {i + 1}} \sigma (t, X (t)) \mathrm{d} W (t).
$$

Obviously, the Euler scheme is given by the approximation of the integrals 

$$
\begin{array}{c} \int_ {t _ {i}} ^ {t _ {i + 1}} \mu (t, X (t)) \mathrm{d} t \approx \int_ {t _ {i}} ^ {t _ {i + 1}} \mu (t _ {i}, X (t _ {i})) \mathrm{d} t = \mu (t _ {i}, X (t _ {i})) \Delta t _ {i} \\ \int_ {t _ {i}} ^ {t _ {i + 1}} \sigma (t, X (t)) \mathrm{d} W (t) \approx \int_ {t _ {i}} ^ {t _ {i + 1}} \sigma (t _ {i}, X (t _ {i})) \mathrm{d} W (t) = \sigma (t _ {i}, X (t _ {i})) \Delta W (t _ {i}). \end{array}
$$

The following Milstein scheme improves the approximation of the stochastic integral R dW. Definition 178 (Milstein Scheme): q 

Given an Ito processˆ 

$$
\mathrm{d} X (t) = \mu (t, X (t)) \mathrm{d} t + \sigma (t, X (t)) \mathrm{d} W (t),
$$

and a time discretization {t<sub>i</sub> $\mid i = 0 , \ldots , n \}$ with $0 = t _ { 0 } < \ldots < t _ { n } ,$ then the time-discrete stochastic process X<sup>˜</sup> defined by 

$$
\begin{array}{r l} \tilde {X} (t _ {i + 1}) = \tilde {X} (t _ {i}) + \mu (t _ {i}, \tilde {X} (t _ {i})) \Delta t _ {i} + \sigma (t _ {i}, \tilde {X} (t _ {i})) \Delta W (t _ {i}) & \\ + \frac {1}{2} \sigma (t _ {i}, \tilde {X} (t _ {i})) \sigma^ {\prime} (t _ {i}, \tilde {X} (t _ {i})) (\Delta W (t _ {i}) ^ {2} - \Delta t _ {i}) & \end{array}
$$

is called a Milstein Scheme of the process X (where $\Delta t _ { i } : = t _ { i + 1 } - t _ { i }$ and $\Delta W ( t _ { i } ) : = W ( t _ { i + 1 } ) - W ( t _ { i } )$ and $\begin{array} { r } { \sigma ^ { \prime } : = \frac { \partial } { \partial X } \sigma ) } \end{array}$ y 

Remark 179 (Milstein Scheme): The Milstein scheme gives an “improvement” only if <sub>σ</sub> depends on X. 

Let us consider another discretization scheme: 

Definition 180 (Euler Scheme with Predictor-Corrector Step): Given an Ito processˆ 

$$
\mathrm{d} X (t) = \mu (t, X (t)) \mathrm{d} t + \sigma (t, X (t)) \mathrm{d} W (t),
$$

and a time discretization {t $\mid i = 0 , \ldots , n \}$ with $0 = t _ { 0 } < \ldots < t _ { n }$ , then the time-discrete stochastic process X<sup>˜</sup> defined by 

$$
\tilde {X} (t _ {i + 1}) = \tilde {X} (t _ {i}) + \frac {1}{2} (\mu (t _ {i}, \tilde {X} (t _ {i})) + \mu (t _ {i + 1}, \tilde {X} ^ {*} (t _ {i + 1}))) \Delta t _ {i} + \sigma (t _ {i}, \tilde {X} (t _ {i})) \Delta W (t _ {i})
$$

with 

$$
\tilde {X} ^ {*} (t _ {i + 1}) = \tilde {X} (t _ {i}) + \mu (t _ {i}, \tilde {X} (t _ {i})) \Delta t _ {i} + \sigma (t _ {i}, \tilde {X} (t _ {i})) \Delta W (t _ {i})
$$

is called an Euler Scheme with Predictor-Corrector Step of the process X (where $\Delta t _ { i } : = t _ { i + 1 } - t _ { i }$ and $\Delta W ( t _ { i } ) : = W ( t _ { i + 1 } ) - W ( t _ { i } ) )$ . y 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/153e2567e2cd2abea238fab51443bc046f7ac27bba6a53f6acf35ba0e5b96f75.jpg)


Interpretation (Predictor-corrector scheme): The predictor-corrector scheme improves the integration of the drift term $\textstyle \int \mathrm { d } t ,$ not of the stochastic integral R dW. Instead of approximating the integral $\int _ { t _ { i } } ^ { t _ { i + 1 } } \mu ( t , X ( t ) ) ($ dt by a rectangular rule $\dot { \mu } ( t _ { i } , X ( t _ { i } ) ) \cdot \Delta t _ { i }$ the method aims to use a trapezoidal rule. With a trapezoidal rule the integral $\int _ { t _ { i } } ^ { t _ { i + 1 } } \mu ( t , \boldsymbol { X } ( t ) )$ dt would be approximated as $\begin{array} { r } { \frac { 1 } { 2 } ( \mu ( t _ { i } , X ( t _ { i } ) ) + \mu ( t _ { i + 1 } , X ( t _ { i + 1 } ) ) ) \cdot \Delta t _ { i } . } \end{array}$ Since the realization $X ( t _ { i + 1 } )$ and thus $\mu ( t _ { i + 1 } , X ( t _ { i + 1 } ) )$ is unknown, it is approximated by an Euler step $\tilde { X } ^ { * } ( t _ { i + 1 } )$ (predictor step) and the trapezoidal rule is applied with this approximation. This corresponds to correcting $\tilde { X } ^ { * } ( t _ { i + 1 } )$ (corrector step). We have: 

$$
\begin{array}{c} \tilde {X} (t _ {i + 1}) = \tilde {X} ^ {*} (t _ {i + 1}) - \mu (t _ {i}, \tilde {X} (t _ {i})) \cdot \Delta t _ {i} + \frac {1}{2} (\mu (t _ {i}, \tilde {X} (t _ {i})) + \mu (t _ {i + 1}, \tilde {X} ^ {*} (t _ {i + 1}))) \cdot \Delta t _ {i} \\ = \tilde {X} ^ {*} (t _ {i + 1}) + \underbrace {\frac {1}{2} (\mu (t _ {i + 1} , \tilde {X} ^ {*} (t _ {i + 1})) - \mu (t _ {i} , \tilde {X} (t _ {i}))) \cdot \Delta t _ {i}} _ {\text {correction term}}. \end{array}\tag{13.1}
$$

C| 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/f33928eedac8c5470d7772f7ad03fed6bf5d5f9a7cc95ed5871301cfa74cc412.jpg)


Tip (Implementation of the predictor-corrector scheme): Note that for an implementation the Formula (13.1) is more eficient than the two Euler steps in the original Definition (180) of the scheme. The second Euler step is replaced by a correction term applied to $\tilde { X } ^ { * } ( t _ { i + 1 } )$ and requires only the additional calculation . C| 

of $\dot { { \boldsymbol \mu } } ( t _ { i + 1 } , \tilde { X } ^ { * } ( t _ { i + 1 } ) )$ 

The schemes presented give a time-discrete stochastic process $\tilde { X }$ such that $\tilde { X } ( t _ { i } )$ is an approximation of $X ( t _ { i } )$ . An in-depth discussion of numerical methods of approximating stochastic processes can be found in [21]. 

## 13.1.2. Time-Discretization of a Lognormal Process

Consider the process 

$$
\mathrm{d} X = \mu (t, X (t)) X (t) \mathrm{d} t + \sigma (t) X (t) \mathrm{d} W (t),\tag{13.2}
$$

where $( t , x ) \mapsto \mu ( t , x )$ and $t \mapsto \sigma ( t )$ are given deterministic functions. With Lemma 49 we have 

$$
\mathrm{d} \log (X) = (\mu (t, X (t)) - \frac {1}{2} \sigma^ {2} (t)) \mathrm{d} t + \sigma (t) \mathrm{d} W (t).\tag{13.3}
$$

in the following we discuss several possible time-discretizations of the process X. The discussion is of special importance since the Black-Scholes model, the Black model and the LIBOR Market Model are all of the form (13.2). 

## 13.1.2.1. Discretization via Euler scheme

The Euler scheme for the stochastic diferential equation (13.2) is given by 

$$
\tilde {X} (t _ {i + 1}) = \tilde {X} (t _ {i}) + \mu (t _ {i}, \tilde {X} (t _ {i})) \tilde {X} (t _ {i}) \Delta t _ {i} + \sigma (t _ {i}) \tilde {X} (t _ {i}) \Delta W (t _ {i}).
$$

The random variables $\tilde { X } ( t )$ generated by this scheme difer from the random variables $X ( t )$ of the time-continuous process by a discretization error $X ( t ) - \tilde { X } ( t )$ . This discretization error might be relatively large. Take for example the even simpler case of a vanishing drift $\mu = 0 .$ Then $\tilde { X } ( t _ { 1 } )$ is normal distributed, while $X ( t _ { 1 } )$ is lognormal distributed. Note that $\tilde { X }$ can attain negative values, while X cannot (this follows from (13.3)). 

## 13.1.2.2. Discretization via Milstein scheme

One way of reducing the discretization error is to use the Milstein scheme (Definition 178): 

$$
\begin{array}{r l} & {\tilde {X} (t _ {i + 1}) = \tilde {X} (t _ {i}) + (\mu (t _ {i}, \tilde {X} (t _ {i})) - \frac {1}{2} \sigma (t _ {i}) ^ {2}) \tilde {X} (t _ {i}) \Delta t _ {i}} \\ & {\qquad + \sigma (t _ {i}) \tilde {X} (t _ {i}) \Delta W (t _ {i}) + \frac {1}{2} \sigma (t _ {i}) ^ {2} \tilde {X} (t _ {i}) \Delta W (t _ {i}) ^ {2}.} \end{array}
$$

## 13.1.2.3. Discretization of the Log-Process

A much better discretization than the two previous schemes is given by the Euler discretization of the Ito process of log(ˆ X). The Euler scheme of (13.3) is given by 

$$
\log (\tilde {X} (t _ {i + 1})) = \log (\tilde {X} (t _ {i})) + (\mu (t _ {i}, \tilde {X} (t _ {i})) - \frac {1}{2} \sigma (t _ {i}) ^ {2}) \Delta t _ {i} + \sigma (t _ {i}) \Delta W (t _ {i}),\tag{13.4}
$$

and applying the exponential we have 

$$
\tilde {X} (t _ {i + 1}) = \tilde {X} (t _ {i}) \cdot \exp \big ((\mu (t _ {i}, \tilde {X} (t _ {i})) - \frac {1}{2} \sigma (t _ {i}) ^ {2}) \Delta t _ {i} + \sigma (t _ {i}) \Delta W (t _ {i}) \big).
$$

Using this scheme will give a lognormal random variable $\tilde { X } ( t _ { 1 } )$ . 

## 13.1.2.4. Exact Discretization

For the special case where $\mu$ does not depend on X, e.g. if X is a relative price under the corresponding martingale measure and thus even drift-free, then we can take the exact solution as a discretization scheme. We then have: 

$$
X (t _ {i + 1}) = X (t _ {i}) \cdot \exp \big ((\mu_ {i} - \frac {1}{2} \sigma_ {i} ^ {2}) \Delta t _ {i} + \sigma_ {i} \Delta W (t _ {i}) \big),\tag{13.5}
$$

where 

$$
\mu_ {i} := \frac {1}{\Delta t _ {i}} \int_ {t _ {i}} ^ {t _ {i + 1}} \mu (\tau) \mathrm{d} \tau , \quad \sigma_ {i} := \sqrt {\frac {1}{\Delta t _ {i}} \int_ {t _ {i}} ^ {t _ {i + 1}} \sigma^ {2} (\tau) \mathrm{d} \tau}.
$$

## 13.2. Discretization of Paths (Monte-Carlo Simulation)

Consider the time-discrete stochastic process 

$$
X (t _ {i + 1}) = X (t _ {i}) + \mu (t _ {i}, X (t _ {i})) \Delta t _ {i} + \sigma (t _ {i}, X (t _ {i})) \Delta W (t _ {i}).\tag{13.6}
$$

This is an Euler scheme. The considerations below apply to any other discretization scheme. Furthermore, we do not apply a tilde to the process X since we are only considering the timediscrete process, and so do not have to distinguish it from the original time-continuous process. 

## 13.2.1. Monte-Carlo Simulation

The random variables $\Delta W ( t _ { i } )$ of the respective time steps are mutually independent, see Definition 28. At every time step t a random number is drawn according to the distribution of $\Delta W ( t _ { i } )$ (i.e. a vector of random numbers if $\Delta W ( t _ { i } )$ is vector valued), which we denote by $\Delta W ( t _ { i } , \omega _ { j } )$ Then 

$$
X (t _ {i + 1}, \omega_ {j}) = X (t _ {i}, \omega_ {j}) + \mu (t _ {i}, X (t _ {i}, \omega_ {j})) \Delta t _ {i} + \sigma (t _ {i}, X (t _ {i}, \omega_ {j})) \Delta W (t _ {i}, \omega_ {j})
$$

determines the process X on a path, which we denote by $\omega _ { j } .$ Here $\Delta W ( t _ { i } , \omega _ { j } )$ and $\Delta W ( t _ { k } , \omega _ { j } )$ $( i \neq k )$ are independent random numbers, following the definition of the Brownian motion. If we follow this rule to generate paths $\omega _ { 1 } , \ldots , \ldots , \omega _ { n _ { \mathrm { p a t h s } } }$ , where $\Delta W ( t _ { i } , \omega _ { j } )$ and $\Delta W ( t _ { i } , \omega _ { k } ) ~ ( j \neq k )$ are independent, then we say that the set 

$$
\{X (t _ {i}, \omega_ {k}) \mid i = 0, 1, \dots , n _ {\mathrm{times}}; k = 0, 1, \dots , n _ {\mathrm{paths}} \}
$$

is a Monte-Carlo simulation of the process X. The generation of random numbers is discussed 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/272ef36c4a6c590b8e01d246c5369b85af70310319183721ce58e87d87da815c.jpg)



Figure 13.2.: Monte-Carlo Simulation


in Section A.2. 

An approximation of the expectation of some function f of the $X ( t _ { i } ) ^ { \circ } \mathrm { s }$ is then given by 

$$
\mathrm{E} ^ {\mathbb {P}} \left(f \left(X \left(t _ {0}\right), \dots , X \left(t _ {n _ {\text { times }}}\right)\right) \mid \mathcal {F} _ {t _ {0}}\right) \approx \sum_ {j = 1} ^ {n _ {\text { paths }}} f \left(X \left(t _ {0}, \omega_ {j}\right), \dots , X \left(t _ {n _ {\text { times }}}, \omega_ {j}\right)\right) \cdot \frac {1}{n _ {\text { paths }}}.
$$

## 13.2.2. Weighted Monte-Carlo Simulation

A generalization of the procedure is to generate the random numbers $\Delta W ( t _ { i } , \omega _ { j } )$ not according to the distribution $\Delta W ( t _ { i } )$ , which means that all paths $\omega _ { j }$ are generated with non-uniform weights $\begin{array} { r } { p _ { j } \ : ( \sum _ { j = 1 } ^ { n _ { \mathrm { p a t h s } } } p _ { j } = 1 ) } \end{array}$ . In this case we call the simulation weighted Monte-Carlo simulation. For the expectation we have 

$$
\mathrm{E} ^ {\mathbb {P}} \left(f \left(X \left(t _ {0}\right), \dots , X \left(t _ {n _ {\text { times }}}\right)\right) \mid \mathcal {F} _ {t _ {0}}\right) \approx \sum_ {j = 1} ^ {n _ {\text { paths }}} p _ {j} f \left(X \left(t _ {0}, \omega_ {j}\right), \dots , X \left(t _ {n _ {\text { times }}}, \omega_ {j}\right)\right).
$$

To summarize, the Monte-Carlo simulation consists of the time-discrete process X in (13.6), represented over a discrete probability space $( \tilde { \Omega } , \tilde { \mathcal { F } } , \tilde { P } )$ , where 

$$
\tilde {\Omega} = \{\omega_ {1}, \dots , \omega_ {n _ {\text { paths }}} \} \subset \Omega , \quad \tilde {\mathcal {F}} = \sigma (\{\omega_ {j} \} | j = 1, \dots , n _ {\text { paths }}), \quad \tilde {P} (\{\omega_ {j} \}) = p _ {j}.
$$

## 13.2.3. Implementation

The Figures 13.3, 13.4 show an example for an object-oriented design. The Figures follow the Unified Modeling Language (UML) 1.3, see [28]. 

The generation of a Monte-Carlo simulation of a lognormal process is realized through the abstract base class LogNormaLPRocess. The class defines abstract methods for initial conditions, drift and volatility. A specific model has to be derived from this class and implement the three methods. The abstract base class LogNormaLProcEss provides the implementation of the discretization scheme, using the methods for initial conditions, drift and volatility. 

The calculation of the Brownian increments, i.e. the random numbers, is given by an additional class: BROWNIANMoTION 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/6f2b388c12e1e092309f891727612a30881855b5041855e81c98dd238482d1e2.jpg)



Figure 13.3.: UML Diagram: Monte-Carlo Simulation / Lognormal Process.


## 13.2.3.1. Example: Valuation of a Stock Option under the Black-Scholes Model using Monte-Carlo Simulation

Consider the model from Section 4, the Black-Scholes model: We have to simulate the process 

$$
\mathrm{d} S (t) = r (t) S (t) \mathrm{d} t + \sigma (t) S (t) \mathrm{d} W ^ {\mathbb {P}} (t) \quad \text { under   the   measure } \mathbb {Q} ^ {N} \quad S (0) = S _ {0}
$$

together with the numeraire´ 

$$
\mathrm{d} N (t) = r (t) N (t) \mathrm{d} t
$$

$$
N (0) = 1,
$$

which is not stochastic here. For this example we have to set $X = ( X _ { 1 } , X _ { 2 } ) \ : = \ : ( S , N )$ in the previous section. We choose r and <sub>σ</sub> constant and apply the Euler scheme to log(S ), following Section 13.1.2.3: 

$$
\begin{array}{l l} S (t _ {i + 1}) = S (t _ {i}) \cdot \exp ((r - \frac {1}{2} \sigma^ {2}) \Delta t _ {i} + \sigma \Delta W (t _ {i})) & S (0) = S _ {0} \\ N (t _ {i + 1}) = N (t _ {i}) \cdot \exp (r \Delta t _ {i}). & N (0) = 1. \end{array}
$$

In this example the time discretization does not introduce an approximation error, because we are in the special situation of Section 13.1.2.4. If $\omega _ { \mathrm { 1 } } , \ldots , n _ { \mathrm { p a t h s } }$ are paths of a Monte-Carlo simulation, then we have for the price V of a European option with maturity $t _ { k }$ and strike K 

$$
V (0) \approx N (0) \frac {1}{n _ {\text { paths }}} \sum_ {j = 1} ^ {n _ {\text { paths }}} \frac {\max \left(S \left(t _ {k} , \omega_ {j}\right) - K , 0\right)}{N \left(t _ {k}\right)}.
$$

We can extend the object-oriented design from Figure 13.3 to derive the class BLAckSc-HoLEsMopEL from the abstract base class LoGNoRMALPROCESs. The class BLACKScHoLEsMopEI implements the methods providing the initial value (returning S (0)), the drift (returning r) and the factor loading (returning <sub>σ</sub>). In this context the factor loading is identical to the volatility.<sup>2</sup> In addition the class implements a method that returns the corresponding numeraire.´ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/d6413a8456a8f2a70f6aaa2c13a2e9b28b33f1282f6c35ca2456071448d89b60.jpg)



Figure 13.4.: UML Diagram: Evaluation under a Black-Scholes Model via Monte-Carlo Simulation. This class hierarchy is realized in the Java™ code.


## 13.2.3.2. Separation of Product and Model

The evaluation of a derivative product, in our case a simple European option, is realized in its own class STockOPTIoN. This class communicates not directly with the BLAckScHoLEsMoDEL. Instead it expects an interface MoNTECARLoSTockPRocEssMoDEL and the model implements this interface. 

The interface MoNTECARLoSTockPRocEssMoDEL means, that the stock model makes the stock process and the numeraire available to the stock product as a Monte-Carlo simulation.´ All corresponding Monte-Carlo evaluations of stock products expect this interface only. All corresponding Monte-Carlo stock models implement this interface. This produces a separation of product and model. The model used to evaluate the products may be exchanged for another, as long as the interface is respected. 

We will use this principle in the object-oriented design of the LIBOR Market Model, a multi-dimensional interest rate model. There we will reuse the classes BrowNIAnMotioN and LoGNoRMALPRocEss, see Section 19.2 

<sup>2</sup> In a multi-factor model the factor loading is given by the square root of the covariance matrix. 

## 13.2.3.3. Model-Product Communication Protocol

In designing a Monte-Carlo simulation, one of the first steps is the design of the core data objects representing the realizations of the stochastic process. These are the data objects that are sent from the model to the product (via call to a method of the model). They define the communication protocol between model and product. 

If we think of a more complex model, e.g. a model for a family of forward rates $\{ L ( T _ { i } , T _ { i + 1 } ) \mid i = 0 , 1 , 2 , \ldots , n - 1 \}$ , as given by the LIBOR Market Model, then the product needs access to a whole family of stochastic processes to process it. 

The question we would like to briefly address here is how this data should be stored and in what order it is usually accessed and processed. Of course, the favored solution may vary with the specific application, so we shall remain on a fairly general level. More specifically we would like to consider the order in which data objects are aggregated. For example: is it better to store a family of stochastic processes, each being a family of one-dimensional random variables (parametrized by simulation time), each being a set of realizations on a path, i.e. 

$$
\{\{\{X _ {i} (t _ {j}, \omega_ {k}) \mid k = 0, 1, 2, \dots \} \mid j = 0, 1, 2, \dots \} \mid i = 0, 1, 2, \dots \},
$$

or would we rather store a family of sample paths (with path index $k )$ of a function of $t _ { j }$ (with time index $j )$ each being vector values (with component index $i ) ,$ i.e. 

$$
\{\{\{X _ {i} (t _ {j}, \omega_ {k}) \mid i = 0, 1, 2, \dots \} \mid j = 0, 1, 2, \dots \} \mid k = 0, 1, 2, \dots \}.\tag{13.7}
$$

Examples of such data objects are a family of forward rates $X _ { i } : = L ( T _ { i } , T _ { i + 1 } )$ , e.g. as modeled by a LIBOR Market Model, or a set of stock price processes $X _ { i }$ , for example as underlyings of a basket. 

One is tempted to believe that for a Monte-Carlo simulation the paths $\omega _ { k }$ are totally independent objects and thus that it would be reasonable to have the index k on the top-most level of aggregation / parametrization, as is the case in (13.7). Indeed, this would make it easy to parallelize the processing since the algorithm could be called with diferent subsets of paths. However, this is only possible for simple (say European) options. 

The solution we recommend is to aggregate the data (from outer to inner objects) as a family of random variables parametrized by $t _ { j } ,$ each random variable being a vector consisting of onedimensional random variables parametrized by i, each one-dimensional random variable being represented by a vector of evaluations on sample paths parametrized by $k ,$ i.e. 

$$
\{\{\{L (T _ {i}, T _ {i + 1}; t _ {j}, \omega_ {k}) \mid k = 0, 1, 2, \dots \} \mid i = 0, 1, 2, \dots \} \mid j = 0, 1, 2, \dots \}.
$$

In other words: We build our data object or array (from inner to outer) as follows: 

Core Object: Random Variable The core object is a one-dimensional random variable evaluated on given sample paths, 

$$
x _ {k} := X (\omega_ {k}),
$$

defining a vector of realizations $\hat { X } : = ( x _ { 1 } , \ldots , x _ { m } ) ^ { \mathrm { T } }$ . There are two major reasons for using this vector as a basic object: 

• Product payofs are functions of the underlyings, i.e. functions operating on random variables. This makes it possible to define the functions as functions acting on vectors (vector arithmetic), which greatly increases the readability of the code. Loops over the paths are hidden inside the methods acting on the random variable objects. For example, the payof of an option max $S _ { T } - X , 0 )$ would appear as such in the code while the pathwise evaluation is hidden in the implementation of the max-function. 

• For Bermudan options it is necessary to calculate conditional expectations. To do so, one needs access to the realizations on other paths, e.g. when using the regression method (see Section 15.10.1). To some extent, the pricing of Bermudan options breaks the naive parallelization of pricings through subsets of sample paths. See the discussion of the foresight bias in Section 15.9. 

Aggregation 1: Vector of Random Variables of same Simulation Time When simulating multiple stochastic processes, like for example a basket of underlyings or a family of forward rates, access to the whole family for a fixed simulation time t is normally required. So on the next aggregation level the basic object thus is a vector of random variables sharing the same measurability property, 

$$
X _ {i} \qquad \text { where } X _ {i} \text { is } \mathcal {F} _ {t} \text { measurable. }
$$

This makes sense since we often build a new stochastic process by defining its time t value as a function of the time t value of other stochastic processes. We give two examples: 

• At time t, the value of a basket of stocks is the sum of the underlyings $S _ { T } ^ { i }$ . 

• At time t the swap rate is a function of forward rates L<sub>i</sub>(t). 

Aggregation 2: Time-discrete Stochastic Process Aggregating these vectors of random variables over all simulation times is finally the complete description of the Monte-Carlo simulation. 

Storage, Access and Processing To summarize, we say that for most applications the storage should be allocated as a three dimensional array 

```javascript
double[][][] process; 
```

## where

```javascript
double[] randomVariable = process[simulationTimeIndex][stochasticProcessIndex]; 
```

results in a reference (!) to a vector containing the sample paths of a random variable $X _ { j } ( t _ { i } )$ If basic functionalities are implemented as methods acting on random variables, then we may work directly with this reference. It may be convenient to define this as a class, eventually endowing it with additional information, e.g. 

```dart
class RandomVariable {
    double time; // Corresponding filtration time in the context of stochastic processes.
    double[] realizations;
} 
```

Remark 181 (Counter Example): There are applications where other storage layouts are advantageous. Path-dependent products such as Asian or lookback options, usually require to apply a function to a path (parametrized by $t _ { j } )$ . In such cases it may be convenient to work with (13.7). 

Remark 182 (Performance and Readability of the Code): The storage layout has an impact on the performance. Usually a large number of paths (10000-100000) for a few stochastic processes (1-100) given at a modest number of time discretization points (50-500) are considered. Therefore, it is sensible to use the random variable as the core object so that one needs to allocate only a few objects containing large continuous blocks of memory (which is more eficient than doing it vice versa) and one can optimize core methods which iterate often.<sup>3</sup> 

Last but not least, the entire mathematical theory is built on random variables as the central modeling entity. Thus, using random variables as core objects will improve the readability of the code. Whenever code is developed as a collaborative efort, this should be considered as a top priority. 

## 13.2.4. Review

Through the Monte-Carlo simulation we can evaluate simple and pure path-dependent products. The Monte-Carlo evaluation of derivatives where an expectation has to be calculated that is conditional to a future time $t _ { i }$ is non-trivial, e.g. 

$$
\operatorname{E} \left(X (t _ {j}) \mid \mathcal {F} _ {t _ {i}}\right)
$$

for $t _ { j } > t _ { i } > t _ { 0 } . ^ { 4 }$ Why this is non-trivial becomes apparent when we consider the filtration: 

In a path simulation in general no two paths will have a common past. The reason is that the number of possible states $X ( t _ { i } )$ is much higher than the number of paths that are simulated. If no two paths have a common past, then we have the following filtration 

$$
\begin{array}{l} \tilde {\mathcal {F}} _ {t _ {i}} = \tilde {\mathcal {F}} \quad \text { for   all } t _ {i} > t _ {0} \text { and } \\ \tilde {\mathcal {F}} _ {t _ {0}} = \tilde {\Omega}. \end{array}
$$

The calculation of a condition expectation in a Monte-Carlo simulation is not straight forward, since no suitable time discretization of the filtration $\mathcal { F } _ { t _ { i } }$ of X is $\mathrm { g i v e n . } ^ { 5 }$ The filtration of the Monte-Carlo simulation depicted in Figure 13.2 is given by 

$$
\begin{array}{l} \tilde {\mathcal {F}} _ {t _ {0}} = \{\emptyset , \tilde {\Omega} \} \\ \tilde {\mathcal {F}} _ {t _ {1}} = \sigma (\{\{\omega_ {1} \}, \{\omega_ {2} \}, \{\omega_ {3} \}, \{\omega_ {4} \} \}) \\ \tilde {\mathcal {F}} _ {t _ {2}} = \sigma (\{\{\omega_ {1} \}, \{\omega_ {2} \}, \{\omega_ {3} \}, \{\omega_ {4} \} \}) \\ \tilde {\mathcal {F}} _ {t _ {3}} = \sigma (\{\{\omega_ {1} \}, \{\omega_ {2} \}, \{\omega_ {3} \}, \{\omega_ {4} \} \}). \end{array}
$$

For the path simulation depicted in Figure 13.5 the filtrations are not all the same. The 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/b1bdce2cea02bb6266f9d9cf5b76fc571badeb7b70862476d38c9acc0fc693e5.jpg)



Figure 13.5.: Monte-Carlo Simulation


filtration is given by 

$$
\begin{array}{r l} & {\tilde {\mathcal {F}} _ {t _ {0}} = \{\emptyset , \Omega \}} \\ & {\tilde {\mathcal {F}} _ {t _ {1}} = \sigma \big (\{\{\omega_ {1}, \omega_ {2} \}, \{\omega_ {3} \}, \{\omega_ {4}, \omega_ {5}, \omega_ {6} \} \} \big)} \\ & {\tilde {\mathcal {F}} _ {t _ {2}} = \sigma \big (\{\{\omega_ {1} \}, \{\omega_ {2} \}, \{\omega_ {3} \}, \{\omega_ {4} \}, \{\omega_ {5}, \omega_ {6} \} \} \big)} \\ & {\tilde {\mathcal {F}} _ {t _ {3}} = \sigma \big (\{\{\omega_ {1} \}, \{\omega_ {2} \}, \{\omega_ {3} \}, \{\omega_ {4} \}, \{\omega_ {5} \}, \{\omega_ {6} \} \} \big).} \end{array}
$$

To achieve a time-discretization of the filtration, we restrict the possible values of X in each simulation time step. We thus assume a discretization of state space. 

## 13.3. Discretization of State Space

## 13.3.1. Definitions

Instead of the time-discrete process 

$$
X (t _ {i + 1}) = X (t _ {i}) + \mu (t _ {i}, X (t _ {i})) \Delta t _ {i} + \sigma (t _ {i}, X (t _ {i})) \Delta W (t _ {i})
$$

we will consider the time-discrete process 

$$
X (t _ {i + 1}) = X (t _ {i}) + \mu (t _ {i}, X (t _ {i})) \Delta t _ {i} + \sigma (t _ {i}, X (t _ {i})) \Delta B (t _ {i}),\tag{13.8}
$$

where the increments $\Delta B ( t _ { i } )$ are random variables that take only a finite number of values and are mutually independent. According to Theorem 30 we can choose the $\Delta B ( t _ { i } )$ such that in the limit $\Delta t _ { i } \to 0$ we recover a Brownian motion, i.e. for X we recover the original time-continuous process. 

Using the increments $\Delta B ( t _ { i } )$ the process X from (13.8) can take only a finite number of values too 

$$
X (t _ {i}) \in \{x _ {t _ {i}} ^ {j} | j = 0, \ldots , n _ {t _ {i}}; i = 0, \ldots , n _ {\mathrm{times}} \}.
$$

We denote this set as a lattice. Let 

$$
\left\{p _ {i} ^ {j _ {1}, j _ {2}} \mid j _ {1} = 0, \dots , n _ {i}; j _ {2} = 0, \dots , n _ {i + 1}; i = 0, \dots , n _ {\text { times }} - 1 \right\},
$$

denote the transition probabilities of the $\Delta B ( t _ { i } ) ^ { \mathrm { ' } } \mathrm { s }$ i.e. $p _ { i } ^ { j _ { 1 } , j _ { 2 } } : = P ( X ( t _ { i + 1 } ) = x _ { t _ { i + 1 } } ^ { j _ { 2 } } | X ( t _ { i } ) = x _ { t _ { i } } ^ { j _ { 1 } } ) .$ Depending on the probability distribution assumed for the $\Delta B ( t _ { i } )$ , the matrix of transitional probabilities $\big ( p _ { i } ^ { j _ { 1 } , j _ { 2 } } \big ) _ { j _ { 1 } , j _ { 2 } }$ from $t _ { i }$ to $t _ { i + 1 }$ is sparse. For a binomial tree, i.e. binomial distributed $\Delta B ( t _ { i } ) { \bf \dot { s } } ,$ in each row only two entries are non zero. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/6cdec3c66d10c94fbf854f12048708797d148f0701b270eac5474fe034701d29.jpg)



Figure 13.6.: Lattice


In the given situation of a discretized state space, it is far more eficient to store transition probabilities than to simulate all possible paths. For example the lattice in Figure 13.6 exhibits 9 states at each of the 4 time steps. In this lattice there exist $9 ^ { 4 } = 6 5 6 1$ paths, however there are only $9 + 3 \cdot 9 ^ { 2 } = 2 5 2$ transition probabilities. The amount of memory needed to store all paths grows exponentially with time, whereas the amount of memory needed to store all states and transition probabilities shows only linear growth over time. 

If we use binomial distributed increments $\Delta B ( t _ { i } )$ , then we obtain a binomial tree. Figure 13.8 shows the paths that can be distinguished in the binomial tree depicted in Figure 13.7. For the 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/2f7ab9ba886764f130b8aa6b1ddd21236e6c52a2dcd9dede6b4f594c11e164b0.jpg)



Figure 13.7.: Binomial tree


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/eda49fa8a28e9f3900bb8546f3147ebdb85a12648c14e0baafeb879ec4f14743.jpg)



Figure 13.8.: Paths ofthe binomial tree


binomial tree the filtration is no longer trivial. It exhibits a hierarchy of refinements. For the binomial tree in Figure 13.7 the filtration is given by 

$$
\begin{array}{r l} & {\mathcal {F} _ {t _ {0}} = \{\emptyset , \Omega \}} \\ & {\mathcal {F} _ {t _ {1}} = \sigma (\{\{\omega_ {1}, \omega_ {2}, \omega_ {3}, \omega_ {5} \}, \{\omega_ {4}, \omega_ {6}, \omega_ {7}, \omega_ {8} \} \})} \\ & {\mathcal {F} _ {t _ {1}} = \sigma (\{\{\omega_ {1}, \omega_ {2} \}, \{\omega_ {3}, \omega_ {5} \}, \{\omega_ {4}, \omega_ {6} \}, \{\omega_ {7}, \omega_ {8} \} \})} \\ & {\mathcal {F} _ {t _ {3}} = \sigma (\{\{\omega_ {1} \}, \{\omega_ {2} \}, \{\omega_ {3} \}, \{\omega_ {4} \}, \{\omega_ {5} \}, \{\omega_ {6} \}, \{\omega_ {7} \}, \{\omega_ {8} \} \}),} \end{array}
$$

i.e. in addition we have a suitable time-discretization of the filtration. This allows for a calcu lation of conditional expectations. 

## 13.3.2. Backward-Algorithm

Given a lattice we may calculate the conditional expectation of a function f of $X ( t _ { i + 1 } )$ , condition to $X ( t _ { i } ) = x _ { t _ { i } } ^ { j _ { 1 } }$ as 

$$
\mathrm{E} ^ {\mathbb {P}} (f (X (t _ {i + 1})) \mid \{X (t _ {i}) = x _ {t _ {i}} ^ {j _ {1}} \}) \approx \sum_ {j _ {2} = 1} ^ {n _ {t _ {i + 1}}} p _ {i} ^ {j _ {1}, j _ {2}} \cdot f (x _ {t _ {i + 1}} ^ {j _ {2}}).
$$

A step by step application finally gives the expectation $\operatorname { E } ^ { \mathbb { P } } ( f ( X ( t _ { i + 1 } ) ) \mid \{ X ( t _ { 0 } ) = x _ { t _ { 0 } } ^ { 1 } \} )$ . Assuming that $X ( t _ { 0 } ) = \mathrm { c o n s t . } = x _ { t _ { 0 } } ^ { 1 }$ , i.e. that the lattice has a single state in $t _ { 0 }$ , this corresponds to 

$$
\mathrm{E} ^ {\mathbb {P}} (f (X (t _ {i + 1})) \mid \mathcal {F} (t _ {0})).
$$

This procedure is called Backward Algorithm. If we consider the case of a numeraire´ N and a derivative product V given at time $t _ { i + 1 }$ as a function of the states $X ( t _ { i + 1 } )$ , then we find 

$$
\frac {V (t _ {i} , x _ {t _ {i}} ^ {j _ {1}})}{N (t _ {i} , x _ {t _ {i}} ^ {j _ {1}})} \approx \sum_ {j _ {2} = 1} ^ {n _ {t _ {i + 1}}} p _ {i} ^ {j _ {1}, j _ {2}} \cdot \frac {V (t _ {i + 1} , x _ {t _ {i + 1}} ^ {j _ {2}})}{N (t _ {i + 1} , x _ {t _ {i + 1}} ^ {j _ {2}})}.\tag{13.9}
$$

Thus, financial products which are functions of the states $X ( t _ { i } )$ , are evaluated in a lattice by storing the numeraire-relative prices at the nodes´ $x _ { t _ { i + 1 } } ^ { j _ { 2 } }$ and calculating the N-relative value in node $x _ { t _ { i } } ^ { j _ { 1 } }$ via (13.9). The transition (13.9) is also called rollback. 

## 13.3.3. Review

## 13.3.3.1. Path Dependencies

If a lattice with states $x _ { t _ { i } } ^ { j }$ and transition probabilities $p _ { i } ^ { j _ { 1 } , j _ { 2 } }$ is set up, we are able to calculate (certain) conditional expectations. However it is non-trivial to calculate path-dependent products, i.e. financial products that not only depend on the current state of the underlying, but also on the history (the paths). The backward algorithm carries information from the future backward in time but cannot consider information from the past. In contrast the Monte-Carlo simulation is aforward algorithm that carries information forward in time. 

## 13.3.3.2. Course of Dimension

A further problem of lattices becomes apparent for vector values processes X. The number of possible transitions (and thus the amount of transition probabilities that must be stored) grows exponentially with the dimension of the vector X and already for dimensions like 3 or higher the numerical calculation of the rollback (13.9) is critical with respect to the resources required (CPU time and memory). 

## 13.4. Path Simulation through a Lattice: Two Layers

To calculate a path-dependent product in a lattice we may create a Monte-Carlo simulation according to the state-discretized process (13.8). This may be depicted as a “Monte-Carlo simulation through a lattice” or a second Monte-Carlo layer laid over the lattice. See Figure 13.9. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/e8224aef13f470b3f4fdfc49eb28c99592cfcdb003924002b16b712fc419950e.jpg)



Figure 13.9.: Lattice with overlaid Monte-Carlo Simulation


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/5c2a856c0e946a3612af7f245c5636cf90550b51ddf6030653407c8eaa8f4c54.jpg)


Further Reading: An in-depth discussion of numerical methods to approximate stochastic processes is to be found in [21]. C| 

# Numerical Methods for Partial Differential Equations

The Feynman-Kac Theoremˇ creates the link to partial diferential equations. The calculation of an expectation, i.e. the pricing of a derivative, becomes equivalent to the solution of the PDE 

$$
\begin{array}{r c l} \frac {\partial u}{\partial t} + \sum_ {i = 1} ^ {d} \mu_ {i} (t, x) \frac {\partial u}{\partial x _ {i}} + \sum_ {i, j = 1} ^ {d} \gamma_ {i, j} (t, x) \frac {\partial^ {2} u}{\partial x _ {i} \partial x _ {j}} & = & 0 \qquad \text {auf} I \times \Omega \\ u (T, \cdot) & = & \phi (\cdot) \qquad \text {on} \mathbb {R} ^ {d}. \end{array}
$$

Endowed with the pricing PDE we can apply the proven numerical methods for the solution of partial diferential equations, likefinite diferences andfinite elements. In the context of PDEs, the binomial or trinomial tree is just a special variant of a finite diference method (namely an explicit Euler scheme). On the other hand, PDE implementations are just special version of lattices. 

The field of numerical methods for partial diferential equations is huge. In this book we focus more on Monte-Carlo methods, which, to some extent, have a much broader range of application. Here is a brief reference to some literature. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/88df0c2d508ad5297d7150ebf92421649c204268ec95610d21822150cc231522.jpg)


Further Reading: Numerical methods for partial diferential equations in the context of mathematical finance may be found in Gunther & J¨ ungel [¨ 17], Seydel [32], Wilmott [40]. A discussion of the implementation of the Cheyette model’s PDE is given in [80]. C| 

# Pricing Bermudan Options in a Monte-Carlo Simulation

## 15.1. Introduction

Let us first consider the simple case of a Bermudan option $V _ { \mathrm { b e r m } } ( T _ { 1 } , T _ { 2 } )$ with two exercise dates only: The option holder has the right to receive an underlying $V _ { \mathrm { u n d e r l } , 1 }$ in $T _ { 1 }$ or wait and retain the right to either receive an underlying $V _ { \mathrm { u n d e r l } , 2 }$ in $T _ { 2 }$ or receive nothing. Put diferently, the option holder has the choice of receiving the underlying value $V _ { \mathrm { u n d e r l } , 1 } ( T _ { 1 } )$ or the value of an option $V _ { \mathrm { o p t i o n } } ( T _ { 1 } )$ on $V _ { \mathrm { u n d e r l } , 2 } ( T _ { 2 } )$ . The Bermudan may be interpreted as an option on an option. In $T _ { 1 }$ the optimal exercise is given by choosing the maximum value 

$$
\max (V _ {\text { underl }} (T _ {1}), V _ {\text { option }} (T _ {1})),\tag{15.1}
$$

where (having chosen a numeraire´ N) 

$$
\begin{array}{c} V _ {\text { option }} (T _ {1}) = N (T _ {1}) \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {V _ {\text { option }} (T _ {2})}{N (T _ {2})} \mid \mathcal {F} _ {T _ {1}}) \\ = N (T _ {1}) \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {\max (V _ {\text { underl } , 2} (T _ {2}) , 0)}{N (T _ {2})} \mid \mathcal {F} _ {T _ {1}}). \end{array}\tag{15.2}
$$

is the value of the option with exercise in $T _ { 2 } ,$ evaluated in $T _ { 1 }$ . 

Thus, to evaluate the exercise criterion (15.1) it is necessary to calculate a conditional expectation. The calculation of a conditional expectation within a Monte-Carlo simulation is a non trivial problem. The two main issues are complexity and foresight bias, which we will illustrate in Section 15.5 and 15.6. In the following section we will present methods to eficiently estimate conditional expectations and/or the Bermudan exercise criterion within Monte-Carlo simulation. The application to the pricing of Bermudan options is exemplary.The methods presented are not limited to Bermudan option pricing. 

## 15.2. Bermudan Options: Notation

Reconsider the general definition of a Bermudan option (see Definition 146). Let $\{ T _ { i } \} _ { i = 1 , \ldots , n }$ denote a set of exercise dates and $\{ V _ { \mathrm { u n d e r l } , i } \} _ { i = 1 , \dots , n }$ a corresponding set of underlyings. The 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/e37dd42e3fa9b872a106cc69ff2db6e474d3ea886c878669be3895da1ccc6e2c.jpg)



Figure 15.1.: A simple Bermudan option with two exercise dates.


Bermudan option is the right to receive at one and only one time $T _ { i }$ the corresponding underlying $V _ { \mathrm { u n d e r l } , i }$ (with $i = 1 , \ldots , n )$ or receive nothing. 

At each exercise date $T _ { i } ,$ the optimal strategy compares the value of the product upon exercise with the value of the product upon non-exercise and chooses the larger one. Thus the value of the Bermudan is given recursively 

$$
\underbrace{V_{\text{berm}}(T_{i},\ldots,T_{n};T_{i})}_{\substack{\text{Bermudan with}\\ \text{exercise dates}\\ T_{i},\ldots ,T_{n}}}:= \max \big(\underbrace{V_{\text{berm}}(T_{i + 1},\ldots,T_{n};T_{i})}_{\substack{\text{Bermudan with}\\ \text{exercise dates}\\ T_{i + 1},\ldots ,T_{n}}},\underbrace{V_{\text{underl},i}(T_{i})}_{\substack{\text{Product}\\ \text{received upon}\\ \text{exercise in} T_{i}}}\big),\tag{15.3}
$$

where $V _ { \mathrm { b e r m } } ( T _ { n } ; T _ { n } ) : = 0$ and $V _ { \mathrm { u n d e r l } , i } ( T _ { i } )$ denotes the value of the underlying $V _ { \mathrm { u n d e r l } , i }$ at exercise date $T _ { i }$ 

## 15.2.1. Bermudan Callable

The most common Bermudan option is the Bermudan $\mathrm { C a l l a b l e ^ { 1 } }$ . For a Bermudan Callable the underlyings consist of periodic payments $X _ { k }$ and difer only by the start of the periodic payments. The value of the underlying then becomes 

$$
V _ {\text { underl }, i} (T _ {i}) = V _ {\text { underl }} (T _ {i}, \dots , T _ {n}; T _ {i}) = N (T _ {i}) \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\sum_ {k = i} ^ {n - 1} \frac {X _ {k}}{N (T _ {k + 1})} | \mathcal {F} _ {T _ {i}}\right)
$$

Here $X _ { k }$ denotes a payment fixed in $T _ { k } \left( \mathrm { i . e . } \mathcal { F } _ { T _ { k } } \right.$ measurable) and paid in $T _ { k + 1 }$ . This is the usual setup for interest rate Bermudan Callables. Other payment dates are a minor modification, they simply change the time argument of the numeraire. For the value upon non exercise we have´ as before 

$$
V _ {\text { b   e   r   m }} \left(T _ {i + 1}, \dots , T _ {n}; T _ {i}\right) = N \left(T _ {i}\right) \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {V _ {\text { b   e   r   m }} \left(T _ {i + 1} , \dots , T _ {n} ; T _ {i + 1}\right)}{N \left(T _ {i + 1}\right)} \mid \mathcal {F} _ {T _ {i}}\right).
$$

If the value of the underlying cannot be expressed by means of an analytical formula two conditional expectations have to be evaluated to calculate the exercise strategy (15.3). 

## 15.2.2. Relative Prices

Since the conditional expectation of a numeraire relative price is a num´ eraire relative price´ the presentation will be simplified by considering the numeraire relative quantities. We will´ therefore define: 

$$
\tilde {V} _ {\text { underl }, i} (T _ {j}) := \frac {V _ {\text { underl } , i} (T _ {j})}{N (T _ {j})} \quad \text { and } \quad \tilde {V} _ {\text { berm }, i} (T _ {j}) := \frac {V _ {\text { berm }} (T _ {i} , \ldots , T _ {n} ; T _ {j})}{N (T _ {j})},
$$

thus we have 

$$
\begin{array}{c} \tilde {V} _ {\mathrm{berm}, n} \equiv 0, \\ \tilde {V} _ {\mathrm{berm}, i + 1} (T _ {i}) = \operatorname{E} ^ {\mathbb {Q} ^ {N}} (\tilde {V} _ {\mathrm{berm}, i + 1} (T _ {i + 1}) \mid \mathcal {F} _ {T _ {i}}), \\ \tilde {V} _ {\mathrm{berm}, i} (T _ {i}) = \max (\tilde {V} _ {\mathrm{berm}, i + 1} (T _ {i}), \tilde {V} _ {\mathrm{underl}, i} (T _ {i})), \end{array}
$$

and in the case of a Bermudan callable 

$$
\tilde {V} _ {\text { underl }, i} (T _ {j}) = \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\sum_ {k = i} ^ {n - 1} \tilde {X} _ {k} \left(T _ {k + 1}\right) \mid \mathcal {F} _ {T _ {j}}\right) \quad \text { where } \quad \tilde {X} _ {i} \left(T _ {i + 1}\right) := \frac {X _ {i}}{N \left(T _ {i + 1}\right)}.
$$

The relative prices are marked by a tilde. 

Remark 183 (Notation): The processes $t \mapsto \tilde { V } _ { \mathrm { u n d e r l } , i } ( t )$ and $t \mapsto \tilde { V } _ { \mathrm { { b e r m } } , i } ( t )$ are $\mathcal { F } _ { t }$ conditional expectations of ${ \tilde { V } } _ { \mathrm { u n d e r l } , i } ( T _ { i } )$ and $\tilde { V } _ { \mathrm { b e r m } , i } ( T _ { i } )$ respectively and thus martingales by definition. The time-discrete processes $i \mapsto \tilde { V } _ { \mathrm { u n d e r l } , i } ( T _ { i } ) , i \mapsto \tilde { V } _ { \mathrm { b e r m } , i } ( T _ { i } )$ ) consist of diferent products at diferent times and are thus not normally time-discrete martingales. 

## 15.3. Bermudan Option as Optimal Exercise Problem

A Bermudan option consists of the right to receive one (and only one) of the underlyings $V _ { \mathrm { u n d e r l } , i }$ at the corresponding exercise date $T _ { i } .$ . The recursive definition (15.3) represents the optimal exercise strategy in each exercise time. We formalize this optimal exercise strategy: 

For a given path $\omega \in \Omega$ let 

$$
T (\omega) := \min \{T _ {i}: V _ {\text { b   e   r   m }, i + 1} (T _ {i}, \omega) <   V _ {\text { u   n   d   e   r   l }, i} (T _ {i}, \omega) \},
$$

and 

$$
\eta : \{1, \ldots , n - 1 \} \times \Omega \to \{0, 1 \}, \qquad \eta (i, \omega) := \left\{ \begin{array}{l l} 1 & \text { if } T _ {i} \geq T (\omega) \\ 0 & \text { else. } \end{array} \right.
$$

The definitions of $T$ and give equivalent descriptions of the exercise strategy: $T ( \omega )$ is the optimal exercise time on a given path $\omega , \eta ( \cdot , \omega )$ is an indicator function which changes from 0 to 1 at the time index i corresponding to $T _ { i } = T ( \omega )$ . The boundary $\partial \{ \eta = 1 \}$ of the set $\{ \eta = 1 \}$ is termed the exercise boundary. It should be noted that $\eta ( k )$ is $\mathcal { F } _ { T _ { k } }$ measurable. 

## 15.3.1. Bermudan Option Value as single (unconditioned) Expectation: The Optimal Exercise Value

With the definition of the optimal exercise strategy T (or <sub>η</sub>) it is possible to define a random variable which allows the Bermudan option value to be expressed as a single (unconditioned) expectation. With 

$$
\tilde {U} (T _ {i}) := \tilde {V} _ {\mathrm{underl}, i} (T _ {i}) \quad i = 1, \ldots , n
$$

denoting the relative price of the i-th underlying upon its exercise date $T _ { i }$ we have for the Bermudan value 

$$
\tilde {V} _ {\mathrm{berm}} (T _ {0}) = \mathrm{E} ^ {\mathbb {Q}} (\tilde {U} (T) \big | \mathcal {F} _ {T _ {0}}).
$$

For the Bermudan Callable we may alternatively write 

$$
\tilde {V} _ {\mathrm{berm}} (T _ {0}) = \mathrm{E} ^ {\mathbb {Q}} \big (\sum_ {k = 1} ^ {n - 1} \tilde {X} _ {k} (T _ {k + 1}) \cdot \eta (k)   \Big |   \mathcal {F} _ {T _ {0}} \big).
$$

The random variable $\tilde { U } ( T )$ can be calculated directly using the backward algorithm. We will look at this in the next section and conclude by giving $\tilde { U } ( T )$ a name: 

## Definition 184 (Option Value upon Optimal Exercise):

Let $\tilde { U }$ be the stochastic process whose time t value $U ( t )$ is the (numeraire relative) option value´ received upon exercise in t. Let T be the optimal exercise strategy. The random variable $\tilde { U } ( T )$ where 

$$
\tilde {U} (T) [ \omega ] := U (T (\omega), \omega)
$$

is the (numeraire relative)´ option value received upon optimal exercise. The (numeraire rela-´ tive) Bermudan option value is given by $\mathrm { E } ^ { \mathbb { Q } } ( \tilde { U } ( T ) \big | \mathcal { F } _ { T _ { 0 } } )$ y 

Thus the value of $V _ { \mathrm { b e r m } } ( T _ { 1 } , \dots , T _ { n } )$ can be expressed through a single expectation conditioned to $T _ { 0 }$ and does not need an expectation conditional to a later time to be calculated, $i f$ we have the optimal exercise date $T ( \omega )$ (and thus $\eta ( \cdot , \omega ) )$ for any path <sub>ω</sub>. 

Remark 185 (Stopped Process): The random variable $\tilde { U } ( T )$ is termed a stopped process. $\tilde { U }$ is a stochastic process and T is a random variable with the interpretation of a (stochastic) time. Furthermore $T$ is a stopping-time, see Definition 197. Here the stochastic process U<sup>˜</sup> is the family of underlyings received upon exercise, parametrized by exercise time, and $T$ is the optimal exercise time. Thus $\tilde { U } ( T )$ is the underlying received upon optimal exercise. All quantities are stochastic. 

## 15.4. Bermudan Option Pricing - The Backward Algorithm

The random variable $\tilde { U } ( T )$ can be derived in a Monte-Carlo simulation through the backward algorithm, given the exercise criterion (15.3), i.e. the conditional expectation. The algorithm consists of the application of the recursive definition of the Bermudan value in (15.3) with a slight modification. Let: 

Induction start: 

$$
\tilde {U} _ {n + 1} \equiv 0
$$

Induction step $i + 1  i$ for $i = n , \ldots ,$ 1: 

$$
\tilde {U} _ {i} = \left\{ \begin{array}{l l} \tilde {U} _ {i + 1} & \text { if } \tilde {V} _ {\text { underl }, i} (T _ {i}) <   \mathrm{E} ^ {\mathbb {Q}} (\tilde {U} _ {i + 1} | \mathcal {F} _ {T _ {i}}) \\ \tilde {V} _ {\text { underl }, i} (T _ {i}) & \text { else. } \end{array} \right.
$$

From the Tower Law<sup>2</sup> $\mathrm { E } ^ { \mathcal { Q } } ( \tilde { U } _ { i + 1 } \vert \mathcal { F } _ { T _ { i } } ) = \mathrm { E } ^ { \mathcal { Q } } ( \tilde { V } _ { \mathrm { b e r m } , i + 1 } ( T _ { i } ) \vert \mathcal { F } _ { T _ { i } } )$ by induction and thus 

$$
\tilde {V} _ {\mathrm{berm}} (T _ {1}, \dots , T _ {n}, T _ {0}) = \mathrm{E} ^ {\mathbb {Q}} (\tilde {U} _ {1} | \mathcal {F} _ {T _ {0}})\tag{15.4}
$$

and $\tilde { U } _ { 1 } = \tilde { U } ( T )$ with the notation from the previous section. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/59fc63e092779b0769e59d2e185ee289a4907497a51a745270eabce6a1856916.jpg)


Interpretation: The recursive definition of $\tilde { U } _ { i }$ difers from the recursive definition of $\tilde { V } _ { \mathrm { b e r m } , i } ( T _ { i } )$ . We have 

$$
\tilde {U} _ {i} = \left\{ \begin{array}{l l} \tilde {U} _ {i + 1} & \text { if } \tilde {V} _ {\text { underl }, i} (T _ {i}) <   \mathrm{E} ^ {\mathbb {Q}} (\tilde {U} _ {i + 1} | \mathcal {F} _ {T _ {i}}) \\ \tilde {V} _ {\text { underl }, i} (T _ {i}) & \text { else, } \end{array} \right.
$$

and 

$$
\tilde {V} _ {\text {berm}, i} (T _ {i}) = \left\{ \begin{array}{l l} \mathrm{E} ^ {\mathbb {Q}} (\tilde {V} _ {\text {berm}, i + 1} (T _ {i + 1}) | \mathcal {F} _ {T _ {i}}) & \text {if} \tilde {V} _ {\text {underl}, i} (T _ {i}) <   \mathrm{E} ^ {\mathbb {Q}} (\tilde {U} _ {i + 1} | \mathcal {F} _ {T _ {i}}) \\ \tilde {V} _ {\text {underl}, i} (T _ {i}) & \text {else.} \end{array} \right.
$$

There is a subtle but crucial diference. While both definitions give the Bermudan option value (through application of (15.4)), the definition of $\tilde { U } _ { i }$ requires the conditional expectation operator only to calculate the exercise criterion. 

Since a Monte-Carlo simulation requires advanced methods to obtain an (often not very accurate) estimate for the conditional expectation it is important to reduce their use. 

Note that $\tilde { V } _ { \mathrm { b e r m } , i } ( T _ { i } ) \mathrm { i s } \mathcal { F } _ { T _ { i } }$ measurable by definition as a $\mathcal { F } _ { T _ { i } }$ conditional expectation, while all $\tilde { U } _ { i }$ are at most $\mathcal { F } _ { T _ { r } }$ measurable since they are defined pathwise from $\mathcal { F } _ { T _ { k } }$ measurable random variables $\tilde { V } _ { \mathrm { u n d e r l } , k } ( T _ { k } )$ for $i \leq k \leq n$ C| 

The pricing of a Bermudan option may thus be reduced to either the calculation of conditional expectations or to the calculation of the optimal exercise strategy T. 

As a motivation, in Sections 15.5 and 15.6 we will look at two methods which are not suitable for calculating conditional expectations. 

## 15.5. Re-simulation

Let us consider the simplified example of a Bermudan option as given in Section 15.1. If no analytical calculation of the conditional expectation (15.2) is possible and if Monte-Carlo is the numerical tool for calculating expectations the straightforward way to calculate the conditional expectation is to create in $T _ { 1 }$ a new Monte-Carlo simulation (conditioned) on each path - see 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/52bc259ebb11446b83b2d9abc02831e01405265173f03bdb5022d21e644a62fb.jpg)



Figure 15.2.: Brute-force calculation of the conditional expectation by (path-wise) re-simulation.


Figure 15.2. This leads to a much higher number of total simulation paths needed. If one considers more than one exercise date (option on option on option. . . ) this method becomes particularly impractical. The required number of paths, i.e. the complexity of the algorithm and thus the calculation time, grows exponentially with the number of exercise dates. This creates the need for eficient alternatives. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/b39416216bcac023efd3fdecb1af3842ebb3be42b9b52a152d0e629ee2ea75df.jpg)


Interpretation: The calculation of conditional expectation in a path simulation requires further measures since the path simulation does not ofer a suitable discretization of the filtration. C| 

## 15.6. Perfect Foresight

If one refuses to use a full resimulation and sticks to the paths generated in the original simulation then one efectively estimates the conditional expectation by a single path, namely by 

$$
\mathrm{E} ^ {\mathbb {Q}} \left(\frac {V (T _ {2})}{N (T _ {2})} \mid \mathcal {F} _ {T _ {1}}\right) \approx \frac {V (T _ {2})}{N (T _ {2})}.
$$

Basically, this is a limit-case of the resimulation where each resimulation consists of a single path only, namely the one of the original simulation. If this estimate is used in the exercise criterion the exercise will be super optimal since it is based on future information that would be unknown otherwise. 

The exercise criterion at time $T _ { 1 }$ may only depend on information available in $T _ { 1 } ,$ , i.e. on $\mathcal { F } _ { T _ { 1 } }$ measurable random variables. The estimate $\frac { V ( T _ { 2 } ^ { \bullet } ) } { N ( T _ { 2 } ) }$ is not $\mathcal { F } _ { T _ { 1 } }$ measurable. 

For an illustration of the super-optimality, consider the simulation consisting of two paths, see Figure 15.3. Both paths are identical on $[ 0 , T _ { 1 } ] ,$ i.e. ${ \mathcal F } _ { T _ { 1 } } ~ = ~ \{ 0 , \Omega \} ~ = ~ \{ 0 , \{ \omega _ { 1 } , \omega _ { 2 } \} \}$ . We consider the option V to receive either $S ( T _ { 1 } ) = 2$ at time $T _ { 1 }$ or $S ( T _ { 2 } ) ~ \in ~ \{ 1 , 4 \}$ at a later time $T _ { 2 }$ . The random variable $\eta : \Omega \to \{ 0 , 1 \}$ denotes the exercise strategy for $T _ { 1 } { \mathrm { : } }$ It is 1 on paths that exercise in $T _ { 1 }$ , otherwise 0. With perfect foresight the super optimal exercise strategy is $T ( \omega _ { 1 } ) = T _ { 2 } , T ( \omega _ { 2 } ) = T _ { 1 } , \mathrm { i . e . } \ \eta ( \omega _ { 1 } ) = 0 , \eta ( \omega _ { 2 } ) = 1$ and an average value of $\begin{array} { r } { V ( T _ { 0 } ) = \frac { 1 } { 2 } ( 4 + 2 ) = \frac { 6 } { 2 } } \end{array}$ will be received. Note that then <sub>η</sub> is not $\mathcal { F } _ { T _ { 1 } }$ measurable. The exercise decision is made in $T _ { 1 }$ with knowledge of the future outcome. If we restrict the exercise strategy to the set of $\mathcal { F } _ { T _ { 1 } }$ measurable random variables we either get $\textstyle { \frac { 1 } { 2 } } ( 4 + 1 ) = { \frac { 5 } { 2 } }$ using $\eta \equiv 0$ or $\textstyle { \frac { 1 } { 2 } } ( 2 + 2 ) = { \frac { 4 } { 2 } }$ using $\eta \equiv 1$ . Thus the optimal, $\mathcal { F } _ { T _ { 1 } }$ measurable (and thus admissible) exercise strategy is $\eta ( \omega _ { 1 } ) = \eta ( \omega _ { 2 } ) = 0$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/88f233470f2d6038cbe03230fd67e78976592b21e1de62bf9c1b299906d8cb08.jpg)



Figure 15.3.: Illustration of perfect foresight.


Perfect foresight is not a suitable method for estimating conditional expectation and calculating the exercise criterion. 

## 15.7. Conditional Expectation as Functional Dependence

Let us reconsider the calculation of the conditional expectation through brute-force resimulation as described in Section 15.5 and depicted in Figure 15.2. On each path of the original simulation a re-simulation has to be created. These re-simulations difer in their initial conditions (e.g. the value $S ( T _ { 1 } )$ in a simulation of a stock price following a Black-Scholes Model, or the values $L _ { i } ( T _ { 1 } )$ in a simulation of forward rates following a LIBOR Market Model). The initial conditions are $\mathcal { F } _ { T _ { 1 } }$ measurable random variables (known as of $T _ { 1 } )$ . Thus the conditional expectation is a function of these initial conditions (and possibly other model parameters known in $T _ { 1 } )$ . If it is known that the conditional expectation is a function of a $\mathcal { F } _ { T _ { 1 } }$ measurable random variable Z (we assume here that $Z : \Omega \to \mathbb { R } ^ { d }$ with some d) we have 

$$
\mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {V (T _ {2})}{N (T _ {2})} \mid \mathcal {F} _ {T _ {1}}\right) = \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {V (T _ {2})}{N (T _ {2})} \mid Z\right).\tag{15.5}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/edb637ac3bb661665f948624e0eaeaa3615e8f20840871fc3c41014b9d2747e7.jpg)


Interpretation: If the random variable Z is such that $\mathcal { F } _ { T _ { 1 } }$ is the smallest $\sigma$ field with respect to which Z is measurable (i.e. we have $Z ^ { - 1 } ( \dot { \mathcal { B } } ( \mathbb { R } ^ { q } ) ) = \mathcal { F } _ { T _ { 1 } } )$ , then equation (15.5) is merely the definition of an expectation conditioned on a random variable. If, however, the conditional expectation on the left hand side $\begin{array} { r } { ( \mathrm { i . e . } \ \frac { V ( T _ { 1 } ) } { N ( T _ { 1 } ) } ) } \end{array}$ is known to be measurable with respect to a smaller field (e.g. because its functional depends on a smaller set of random variables), then it might be advantageous to use the right hand side representation. This representation is also useful for deriving an approximation, e.g. if the functional dependence with respect to one component of Z is known to be weak and thus neglectable. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/0f45cf5a02375d9e60585efcf543ed35dc22d11420e53a17b17951de23809a5b.jpg)



Figure 15.4.: Predictor variable versus realized value (continuation value): A diagram showing the path value of the predictor variable Z(<sub>ω</sub> ) and the path value of $\begin{array} { r } { \tilde { V } ( T _ { 2 } ; \omega _ { i } ) = \frac { V ( T _ { 2 } ; \omega _ { i } ) } { N ( T _ { 2 } ; \omega _ { i } ) } } \end{array}$ . The conditional expectation is afunction ofZ dividing the cloud ofdots.


Example: Consider a LIBOR Market Model with stochastic processes for the forward rates $L _ { 1 } , L _ { 2 } , \dots L _ { n }$ . In $T _ { 1 }$ we wish to calculate the conditional expectation of a derivative with a numeraire relative payo´ f that depends on $L _ { 2 } , \ldots , L _ { k }$ only (e.g. on a swap rate). While the filtration $\mathcal { F } _ { T _ { 1 } }$ is generated by the full set of forward rates $L _ { 1 } ( T _ { 1 } ) , L _ { 2 } ( T _ { 1 } ) , \dots L _ { n } ( T _ { 1 } )$ it is suficient to know $L _ { 2 } ( T _ { 1 } ) , \dots , L _ { k } ( T _ { 1 } )$ to describe the conditional expectation (i.e. the conditional value of the product). C| 

We will now describe methods that derive the functional dependance of the conditional expectation from a given set of random variables. 

## 15.8. Binning

In a path simulation the approximation of $\begin{array} { r } { \mathrm { E } ^ { \mathbb { Q } } \left( \frac { V ( T _ { 2 } ) } { N ( T _ { 2 } ) } \mid Z \right) } \end{array}$ will be given by averaging all paths for which Z attains the same value. For the simple example in Figure 15.3 this would remove the perfectforesight since $S ( T _ { 1 } ) ^ { - 1 } ( 2 ) = \Omega$ . In general the situation will be such that there are no two or more paths for which Z attains the same value - apart from the construction of the unfeasible re-simulation. Thus this approximation will show a perfect foresight. 

An improvement is given by a binning method, where the averaging will be done over those paths for which Z lies in a neighborhood (bin). If the quantities are continuous we have: 

$$
\mathrm{E} ^ {\mathbb {Q}} \left(\frac {V (T _ {2})}{N (T _ {2})} \mid Z\right) [ \omega ] \approx \mathrm{E} ^ {\mathbb {Q}} \left(\frac {V (T _ {2})}{N (T _ {2})} \mid Z \in U _ {\epsilon} (Z (\omega))\right),
$$

where $U _ { \epsilon } ( Z ( \omega ) ) : = \{ y | \| Z ( \omega ) - y \| < \epsilon \} .$ 

Instead of defining a bin $U _ { \epsilon } ( Z ( \omega ) )$ for each path it is more eficient to start with a partition of $Z ( \Omega )$ into a finite set of disjoint bins $U _ { i } \subset Z ( \Omega )$ . The approximation of the conditional 

expectation 

$$
\mathrm{E} ^ {\mathbb {Q}} \left(\frac {V (T _ {2})}{N (T _ {2})} \mid Z (\omega)\right)
$$

will then be given by 

$$
H _ {i} := \mathrm{E} ^ {\mathbb {Q}} \left(\frac {V (T _ {2})}{N (T _ {2})} \mid Z \in U _ {i}\right)
$$

where $U _ { i }$ denotes the set with $Z ( \omega ) \in U _ { i }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/098d0cda0aab6053df33c9ec0afb98e53f4c970f85d9ca99c729d4e6287a9a67.jpg)



Figure 15.5.: Calculation of the conditional expectation by binning: Neighbouring paths, i.e. paths which belong to the same bin, are bundled. The bins are defined by means ofthe $\mathcal { F } _ { T _ { 1 } }$ -measurable predictor variable Z. Thefigure shows the special case $Z = W ( T _ { 1 } )$ .


## Example: Pricing of a simple Bermudan Option on a Stock

We illustrate the method in a simple Black-Scholes model for a stock S . In $T _ { 1 }$ we wish to evaluate the option of receiving $N _ { 1 } \cdot ( S ( T _ { 1 } ) - K _ { 1 } )$ in $T _ { 1 }$ or receiving $N _ { 2 } \cdot \operatorname* { m a x } ( S ( T _ { 2 } ) - K _ { 2 } , 0 )$ at later time $T _ { 2 }$ (where $N _ { 1 } , N _ { 2 }$ (notional), $K _ { 1 } , K _ { 2 }$ (strike) are given). The optimal exercise in $T _ { 1 }$ compares the exercise value with the value of the $T _ { 2 }$ option, i.e. 

$$
\mathrm{E} ^ {\mathbb {Q}} \left(\frac {N _ {2} \cdot \max (S (T _ {2}) - K _ {2} , 0)}{N (T _ {2})} \mid \mathcal {F} _ {T _ {1}}\right).
$$

From the model specification, $\mathrm { e . g . }$ . here a Black-Scholes model 

$$
\mathrm{d} S (t) = r \cdot S (t) \mathrm{d} t + \sigma S (t) \mathrm{d} W ^ {\mathbb {Q}} (t), \qquad N (t) = \exp (r t)
$$

it is obvious that the price of the $T _ { 2 }$ option seen in $T _ { 1 }$ is a given function $S ( T _ { 1 } )$ and the given model parameters $( r , \sigma )$ . Thus it is suficient to calculate 

$$
\mathrm{E} ^ {\mathbb {Q}} \left(\frac {N _ {2} \cdot \max (S (T _ {2}) - K _ {2} , 0)}{N (T _ {2})} \mid S (T _ {1})\right).
$$

In this example the functional dependence is known analytically. It is given by the Black-Scholes formula (4.3). Nevertheless we use the binning to calculate an approximation to the conditional expectation. If we plot 

$$
\underbrace {\frac {N _ {2} \cdot \max (S (T _ {2} , \omega_ {i}) - K _ {2} , 0)}{N (T _ {2})}} _ {\text {   Continuation   Value   }} \quad \text {   as   a   function   of   } \quad \underbrace {S (T _ {1} , \omega_ {i})} _ {\text {   Underlying   }}
$$

we obtain the scatter plot in Figure 15.6, left. For a given $S ( T _ { 1 } )$ none or very few values of the continuation values exist. An estimate is not possible or else exhibits a foresight bias. For an interval $[ S _ { 1 } - \epsilon , S _ { 1 } + \epsilon ]$ with suficiently large <sub></sub> we have enough values to estimate 

$$
\mathrm{E} ^ {\mathbb {Q}} \left(\frac {N _ {2} \cdot \max (S (T _ {2}) - K _ {2} , 0)}{N (T _ {2})} \mid S (T _ {1}) \in [ S _ {1} - \epsilon , S _ {1} + \epsilon ]\right)
$$

which in turn may be used as an estimate of 

$$
\mathrm{E} ^ {\mathbb {Q}} \left(\frac {N _ {2} \cdot \max (S (T _ {2}) - K _ {2} , 0)}{N (T _ {2})} \mid S (T _ {1}) = S _ {1}\right).
$$

In Figure 15.6, right, we calculate this estimate for $S _ { \textrm { l } } = 1$ and $\epsilon = 0 . 0 5$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/b4befa4c09d8cd565898d9f265fd35e4a467ddfb87b1335787632e26e6723c53.jpg)



Figure 15.6.: The Continuation Value as a function of the Underlying (Spot Value) and the calculation ofthe conditional expectation by a binning


## 15.8.1. Binning as a Least-Square Regression

Consider the binning again: As an estimate of the conditional expectation $\begin{array} { r } { \mathrm { E } ^ { \mathbb { Q } } \left( { \frac { V ( T _ { 2 } ) } { N ( T _ { 2 } ) } } \mid Z ( \omega ) \right) } \end{array}$ we calculated the conditional expectation 

$$
H _ {i} := \mathrm{E} ^ {\mathbb {Q}} \left(\frac {V (T _ {2})}{N (T _ {2})} \mid Z \in U _ {i}\right)\tag{15.6}
$$

given a bin $U _ { i }$ with $Z ( \omega ) \in U _ { i }$ 

For the expectation operator $\mathrm { E ^ { \mathbb { Q } } }$ an alternative characterization may be used: 

Lemma 186 (Characterization of the Expectation as Least-Square Approximation): The expectation of a random variable X is the number h for which $X - h$ has the smallest variance (i.e. $L _ { 2 } ( \Omega )$ norm). 

Proof: Let X be a real valued random variable. Then we have for any $h \in \mathbb { R }$ 

$$
E ((X - h) ^ {2}) = E (X ^ {2}) - 2 \cdot E (X) \cdot h + h ^ {2} =: f (h).
$$

Since $f ^ { \prime } = 0 \Leftrightarrow h = E ( X )$ and $f ^ { \prime \prime } = 1 \geq 0$ we have that $f$ attains its minimum in $h = E ( \boldsymbol { X } )$ For vector valued random variables this follows componentwise. The same result holds for conditional expectations. | 

Using Lemma 186 we can write (15.6) as a minimization problem: 

$$
\mathrm{E} ^ {\mathbb {Q}} \left(\left(\frac {V (T _ {2})}{N (T _ {2})} - H _ {i}\right) ^ {2} \mid Z \in U _ {i}\right) = \min _ {G \in \mathbb {R}} \mathrm{E} ^ {\mathbb {Q}} \left(\left(\frac {V (T _ {2})}{N (T _ {2})} - G\right) ^ {2} \mid Z \in U _ {i}\right).
$$

For disjoint bins $U _ { i }$ this may be written in a single minimization problem for the vector $( H _ { i } ) _ { i = 1 , \ldots }$ : 

$$
\sum_ {i} \mathrm{E} ^ {\mathbb {Q}} \left(\left(\frac {V (T _ {2})}{N (T _ {2})} - H _ {i}\right) ^ {2} \mid Z \in U _ {i}\right) = \min _ {G _ {i} \in \mathbb {R}} \sum_ {i} \mathrm{E} ^ {\mathbb {Q}} \left(\left(\frac {V (T _ {2})}{N (T _ {2})} - G\right) ^ {2} \mid Z \in U _ {i}\right).\tag{15.7}
$$

This condition admits an alternative interpretation: $H _ { i }$ represents the piecewise constant function (constant on $U _ { i } )$ with the minimal distance from $\frac { \mathbf { \dot { V } } ( T _ { 2 } ^ { \mathbf { a } } ) } { N ( T _ { 2 } ) }$ in the least square sense. 

Let H be the space of functions $H : \Omega $ R being constant on the bins $Z ^ { - 1 } ( U _ { i } ) . ^ { 3 }$ Let $H \in { \mathcal { H } }$ with $H ( \omega ) : = H _ { i }$ for <sub>ω</sub> $\in Z ^ { - 1 } ( U _ { i } )$ . Then (15.7) is equivalent to 

$$
\mathrm{E} ^ {\mathbb {Q}} \left(\left(\frac {V (T _ {2})}{N (T _ {2})} - H\right) ^ {2} \mid Z\right) = \min _ {G \in \mathcal {H}} \mathrm{E} ^ {\mathbb {Q}} \left(\left(\frac {V (T _ {2})}{N (T _ {2})} - G\right) ^ {2} \mid Z\right).\tag{15.8}
$$

Equation (15.8) is the definition of a regression: Find the function H from a function space H with minimum distance to $\frac { V ( T _ { 2 } ) } { N ( T _ { 2 } ) }$ in the $L _ { 2 }$ norm. Binning is just a special choice of functional space: 

Lemma 187 (Binning as $L _ { 2 }$ Regression): Binning is an $L _ { 2 }$ regression on the space of functions being piecewise constant on $U _ { i } .$ 

## 15.9. Foresight Bias

## Definition 188 (Foresight Bias (Definition 1)):

Aforesight bias is a super optimal exercise strategy. 

A foresight bias arises due to a violation of the measurability requirements: If the exercise decision in $T _ { i }$ is based on a random variable which is not $\mathcal { F } _ { T _ { i } }$ measurable the exercise may be super optimal, i.e. better than if based on the information theoretically available $( \mathcal { F } _ { T _ { i } } )$ . If we use the same Monte-Carlo simulation to first estimate the exercise criterion and then use this criterion to price the derivative we will definitely generate a foresight bias. In this case the foresight bias is created by the Monte-Carlo error of the estimate, which is in general not $\mathcal { F } _ { T _ { i } }$ measurable. The existence of this problem becomes obvious if we consider a limit case of binning where each bin contains a single path only. Here we would have perfect foresight. 

If our exercise criterion at time $T _ { i }$ uses only $\mathcal { F } _ { T _ { i } }$ measurable random variables then there is - in theory - no foresight bias. If, however, the exercise criterion is calculated within a Monte-Carlo simulation, the Monte-Carlo error of the calculation represents a non $\mathcal { F } _ { T _ { i } }$ measurable random variable, thus it induces a foresight bias. In this case we can give an alternative definition for the foresight bias: 

## Definition 189 (Foresight Bias (Definition 2)):

Theforesight bias is the value of the option on the Monte-Carlo error. 

As number of paths increases the foresight bias introduced by binning converges to zero since the Monte-Carlo error with respect to a bin converges to zero. 

A general solution to the problem of a foresight bias is given by using two independent Monte-Carlo simulations: One to estimate the exercise criterion (for binning this is given by the $H _ { i }$ corresponding to the $U _ { i } { } ^ { \prime } \mathbf { s } )$ , the other to apply the criterion in pricing. This is a numerical removal of the foresight bias. In [64] an analytic formula for the (Monte-Carlo error induced) foresight bias is derived. It can be used to correct the foresight bias analytically. 

## 15.10. Regression Methods - Least Square Monte-Carlo

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/fa0d276ab4b569c8481e35f0fc19bc03cb217fc5c321ae7ffd0767675b856990.jpg)


Motivation Disadvantage of Binning: The partition of the state space $Z ( \Omega )$ into a finite number of bins results in a piecewise constant approximation of the conditional expectation. An obvious improvement would be to approximate the conditional expectation by some smooth function of the state variable $Z .$ 

The considerations in Section 15.8.1 suggest a simple yet powerful improvement to the binning: The function giving our estimate for the conditional expectation is defined by a least square approximation (regression). C| 

## 15.10.1. Least Square Approximation of the Conditional Expectation

Let us start with a fairly general definition of the least square approximation of the conditional expectation of random variable U. 

Definition 190 (Least Square Approximation of the Conditional Expectation): 7 Let $( \Omega , \mathcal { F } , \mathbb { Q } , \{ \mathcal { F } _ { t } \} )$ be a filtered probability space and $V \mathrm { ~ a ~ } \mathcal { F } _ { T _ { 1 } }$ measurable random variable defined as the conditional expectation of U 

$$
V = \mathrm{E} ^ {\mathbb {Q}} (U \mid \mathcal {F} _ {T _ {1}}),
$$

where $U$ is at leas $\mathcal { F }$ measurable. Furthermore let $Y : = ( Y _ { 1 } , \ldots , Y _ { p } )$ be a given $\mathcal { F } _ { T _ { 1 } }$ measurable random variable and $f : \mathbb { R } ^ { p } \times \mathbb { R } ^ { q } \mathrm { ~ a ~ }$ given function. Let $\Omega ^ { * } = \{ \omega _ { 1 } , \hdots \omega _ { m } \}$ be a drawing from Ω (e.g. a Monte-Carlo simulation corresponding to Q) and $\alpha ^ { * } : = ( \alpha _ { 1 } , \ldots , \alpha _ { q } )$ such that 

$$
\| U - f (Y, \alpha^ {*}) \| _ {L _ {2} (\Omega^ {*})} = \min _ {\alpha} \| U - f (Y, \alpha) \| _ {L _ {2} (\Omega^ {*})}
$$

where $\lVert U - f ( Y , \alpha ^ { * } ) \rVert _ { L _ { 2 } ( \Omega ^ { * } ) } ^ { 2 } = \sum _ { j = 1 } ^ { m } ( U ( \omega _ { j } ) - f ( Y ( \omega _ { j } ) , \alpha ^ { * } ) ) ^ { 2 }$ . We set 

$$
V ^ {\mathrm{LS}} := f (Y, \alpha^ {*}).
$$

The random variable $V ^ { \mathrm { L S } }$ is $\mathcal { F } _ { T _ { 1 } }$ measurable. It is defined over Ω and a least square approximation of V on $\Omega ^ { * }$ y 

The approach of Carriere, Longstaf and Schwartz<sup>4</sup> uses a function $f$ with $q = p$ and 

$$
f (y _ {1}, \ldots , y _ {p}, \alpha_ {1}, \ldots , \alpha_ {p}) := \sum_ {i = 1} ^ {p} \alpha_ {i} \cdot y _ {i},
$$

such that $\alpha ^ { * }$ may be calculated analytically as a linear regression. 

Lemma 191 (Linear Regression): Let $\Omega ^ { * } ~ = ~ \{ \omega _ { 1 } , \ldots , \omega _ { m } \}$ be a given sample space, $V : \Omega ^ { * } \to \mathbb { R }$ and $Y : = ( Y _ { 1 } , \ldots , Y _ { p } ) : \Omega ^ { * } \to \mathbb { R } ^ { p }$ given random variables. Furthermore let 

$$
f (y _ {1}, \ldots , y _ {p}, \alpha_ {1}, \ldots , \alpha_ {p}) := \sum \alpha_ {i} y _ {i}.
$$

Then we have for any $\alpha ^ { * }$ with $X ^ { \top } X \alpha ^ { * } = X ^ { \top } \nu$ 2 

$$
\| V - f (Y, \alpha^ {*}) \| _ {L _ {2} (\Omega^ {*})} = \min _ {\alpha} \| V - f (Y, \alpha) \| _ {L _ {2} (\Omega^ {*})},
$$

where 

$$
X := \left( \begin{array}{c c c} Y _ {1} (\omega_ {1}) & \ldots & Y _ {p} (\omega_ {1}) \\ \vdots & & \vdots \\ Y _ {1} (\omega_ {m}) & \ldots & Y _ {p} (\omega_ {m}) \end{array} \right), \qquad v := \left( \begin{array}{c} V (\omega_ {1}) \\ \vdots \\ V (\omega_ {m}) \end{array} \right).
$$

If $( X ^ { \top } X ) ^ { - 1 }$ exists then $\alpha ^ { * } : = ( X ^ { \mathsf { T } } X ) ^ { - 1 } X ^ { \mathsf { T } } \nu$ . 

Proof: See Appendix A.1. 

## Definition 192 (Basis Functions):

The random variables $Y _ { 1 } , \dots , Y _ { p }$ of Lemma 191 are called Basis Functions (explanatory variables). y 

## 15.10.2. Example: Evaluation of a Bermudan Option on a Stock (Backward Algorithm with Conditional Expectation Estimator)

Consider a simple Bermudan option on a Stock. The Bermudan should allow exercise at times $T _ { 1 } < T _ { 2 } < \ldots T _ { n }$ . Upon exercise in $T _ { i }$ the holder of the option will receive 

$$
N _ {i} \cdot (S (T _ {i}) - K _ {i})
$$

once, but nothing if no exercise is made. 

We will apply the backward algorithm to derive the optimal exercise strategy. All payments will be considered in their numeraire relative form. Thus the exercise criterion is given by a´ comparison of the conditional expectation of the payments received upon non-exercise with the payments received upon exercise. 

Induction start: $t > T _ { n }$ After the last exercise time we have: 

• The value of the (future) payments is $\tilde { U } _ { n + 1 } = 0$ 

Induction step: $t = T _ { i } , i = n , n - 1 , n - 2 , \ldots 1$ In $T _ { i }$ we have: 

• In the case of exercise in $T _ { i }$ the value is 

$$
\tilde {V} _ {\text { underl,i }} (T _ {i}) := \frac {N _ {i} (S (T _ {i}) - K _ {i})}{N (T _ {i})}.\tag{15.9}
$$

• In the case of non-exercise in $T _ { i }$ the value is $\tilde { V } _ { \mathrm { h o l d , i } } ( T _ { i } ) = \mathrm { E } ^ { \complement } ( \tilde { U } _ { i + 1 } \mid \mathcal { F } _ { T _ { i } } )$ . This value is estimated through a regression for given paths $\omega _ { 1 } , \ldots , \omega _ { m } \colon$ 

– Let $B _ { j }$ be given $( \mathcal { F } _ { T _ { i } }$ measurable) basis functions.<sup>5</sup> Let the matrix X consist of the column vectors $B _ { j } ( \omega _ { k } ) , k = 1 , \ldots , m$ . Then we have 

$$
\left( \begin{array}{c} \tilde {V} _ {\text {hold,i}} (T _ {i}, \omega_ {1}) \\ \vdots \\ \tilde {V} _ {\text {hold,i}} (T _ {i}, \omega_ {m}) \end{array} \right) \approx X \cdot (X ^ {\mathsf {T}} \cdot X) ^ {- 1} \cdot X ^ {\mathsf {T}} \cdot \left( \begin{array}{c} \tilde {U} _ {i + 1} (\omega_ {1}) \\ \vdots \\ \tilde {U} _ {i + 1} (\omega_ {m}) \end{array} \right).\tag{15.10}
$$

• The value of the payments of the product in $T _ { i }$ under optimal exercise is given by 

$$
\tilde {U} _ {i} := \left\{ \begin{array}{l l} \tilde {V} _ {\text { underl,i }} (T _ {i}) & \text { if } \tilde {V} _ {\text { hold,i }} (T _ {i}) <   \tilde {V} _ {\text { underl,i }} (T _ {i}) \\ \tilde {U} _ {i + 1} & \text { else. } \end{array} \right.
$$

Remark 193: Our example is of course just the backward algorithm with an explicit specification of an underlying (15.9) and an explicit specification of an exercise criterion, here given by the estimator of the conditional expectation (15.10). 

## 15.10.3. Example: Evaluation of a Bermudan Callable

Consider a Bermudan Callable. The Bermudan should allow exercise at times $T _ { 1 } ~ < ~ T _ { 2 } ~ <$ $\cdots T _ { n }$ . Upon exercise in $T _ { i }$ the holder of the option will receive a payment of $X _ { i }$ in $T _ { i + 1 }$ , i.e. the relative value $\begin{array} { r } { \tilde { X } _ { i } ( T _ { i + 1 } ) : = \frac { X _ { i } } { N ( T _ { i + 1 } ) } } \end{array}$ 

We will apply the backward algorithm to derive the optimal exercise strategy. All payments will be considered in their numeraire relative form.´ 

Induction start: $t > T _ { n }$ After the last exercise time we have: 

• The value of the (future) payments is $\tilde { U } _ { n + 1 } = 0$ 

<sup>5</sup> Suitable basis functions for this example are 1 (constant), $S ( T _ { i } ) , S ( T _ { i } ) ^ { 2 } , S ( T _ { i } ) ^ { 3 }$ , etc., such that the regression function f will be a polynomial in $S ( T _ { i } )$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/9cf197930ef8f7b13e656f3f28c714ffe71ab2d2afebd57deeeb6d1a4456069e.jpg)



Figure 15.7.: Regression of the conditional expectation estimator without restriction of the regression domain: We consider a Bermudan option with two exercise dates $T _ { 1 } = 1 . 0 , T _ { 1 } = 2 . 0 .$ Notional and strike are as follows: $N _ { 1 } = 0 . 7 ,$ $N _ { 2 } = 1 . 0$ $K _ { 1 } = 0 . 8 2 ,$ $K _ { 2 } = 1 . 0 .$ The model for the underlying S is a Black-Scholes model with $r = 0 . 0 5$ and $\sigma = 2 0 \%$ . The plot shows the values received upon exercise depending on the values received upon non-exercise in $T _ { 1 } .$ . Each dot corresponds to a path. The regression polynomial gives the estimatorfor the expectation of the value upon non-exercise. It is optimal to exercise if this estimate lies above the value received upon exercise. The regression polynomial is a second order polynomial in $S ( T _ { 1 } )$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/0aca23cc208a014eb15d8cf6aa731606bbe51aec95f3a4f66d2569a3c7e9bc4c.jpg)



Figure 15.8.: Regression of the conditional expectation estimator with restriction of the regression domain: Parameters as in Figure 15.7. The regression polynomial is a second order polynomial in max $( S ( T _ { 1 } ) - K _ { 1 } , 0 ) .$ . Thus, values where $S ( T _ { 1 } ) - K _ { 1 } \leq 0$ are aggregated into a single point. For the product under consideration this is advantageous since for $S ( T _ { 1 } ) - K _ { 1 } \leq 0$ exercise is not optimal with probability 1. This restriction of the regression domain increases the regression accuracy over the remaining regression domain. Compare with Figure 15.7.


Induction step: $t = T _ { i } , i = n , n - 1 , n - 2 , \ldots 1$ In $T _ { i }$ we have: 

• In the case of exercise in $T _ { i }$ the value is 

$$
\tilde {V} _ {\text { underl,i }} (T _ {i}) := \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\sum_ {k = i} ^ {n - 1} \frac {X _ {k}}{N (T _ {k + 1})} | \mathcal {F} _ {T _ {i}}\right).
$$

This value is estimated by a regression for given paths $\omega _ { 1 } , \ldots , \omega _ { m } \colon$ 

Let $B _ { j } ^ { 1 }$ be given $( \mathcal { F } _ { T _ { i } }$ measurable) basis functions. Let the matrix $X ^ { 1 }$ consist of the column vectors $B _ { i } ^ { 1 } ( \omega _ { k } ) , k = 1 , \ldots , m$ . Then we have 

$$
\left( \begin{array}{c} \tilde {V} _ {\text {underl,i}} (T _ {i}, \omega_ {1}) \\ \vdots \\ \tilde {V} _ {\text {underl,i}} (T _ {i}, \omega_ {m}) \end{array} \right) \approx X ^ {1} \cdot (X ^ {1, \mathsf {T}} \cdot X ^ {1}) ^ {- 1} \cdot X ^ {1, \mathsf {T}} \cdot \left( \begin{array}{c} \sum_ {k = i} ^ {n - 1} \frac {X _ {k} (\omega_ {1})}{N (T _ {k + 1} , \omega_ {1})} \\ \vdots \\ \sum_ {k = i} ^ {n - 1} \frac {X _ {k} (\omega_ {m})}{N (T _ {k + 1} , \omega_ {m})} \end{array} \right).\tag{15.11}
$$

• In the case of non-exercise in $T _ { i }$ the value is $\tilde { V } _ { \mathrm { h o l d , i } } ( T _ { i } ) = \mathrm { E } ^ { \mathbb { Q } } ( \tilde { U } _ { i + 1 } \mid \mathcal { F } _ { T _ { i } } )$ . This value is estimated by a regression for given paths $\omega _ { 1 } , \ldots , \omega _ { m } \colon$ 

Let $B _ { j } ^ { 0 }$ be given $( \mathcal { F } _ { T _ { i } }$ measurable) basis functions. Let the matrix $X ^ { 0 }$ consist of the 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/4a1b01c4075c539d4ed3a53897f0a05a298d1f2fdb45c27b39b7aee22d095b37.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/da10ab5613dc16e992e1a7cf7cc58da1d1a6a08c362a4d4692cdc3e8f8865b85.jpg)



Figure 15.9.: Regression of the conditional expectation estimator - polynomial offourth (above) and eighth (below) order in max $( S ( T _ { 1 } ) - K _ { 1 } , 0 )$ . Parameters as in Figure 15.7. A polynomial ofhigher order shows wiggles at the boundary of the regression domain. However, only few paths are afected by the wrong estimate. Restricting the regression domain may reduce the errors (compare the left end of the regression domain with the right end).


column vectors $B _ { j } ^ { 0 } ( \omega _ { k } ) , k = 1 , \ldots , m$ . Then we have 

$$
\left( \begin{array}{c} \tilde {V} _ {\text {hold,i}} (T _ {i}, \omega_ {1}) \\ \vdots \\ \tilde {V} _ {\text {hold,i}} (T _ {i}, \omega_ {m}) \end{array} \right) \approx X ^ {0} \cdot (X ^ {0, \mathsf {T}} \cdot X ^ {0}) ^ {- 1} \cdot X ^ {0, \mathsf {T}} \cdot \left( \begin{array}{c} \tilde {U} _ {i + 1} (\omega_ {1}) \\ \vdots \\ \tilde {U} _ {i + 1} (\omega_ {m}) \end{array} \right).
$$

• The value of the payments of the product in $T _ { i }$ under optimal exercise is given by 

$$
\tilde {U} _ {i} := \left\{ \begin{array}{l l} \sum_ {k = i} ^ {n - 1} \frac {X _ {k}}{N (T _ {k + 1})} & \text { if } \tilde {V} _ {\text { hold,i }} (T _ {i}) <   \tilde {V} _ {\text { underl,i }} (T _ {i}) \\ \tilde {U} _ {i + 1} & \text { else. } \end{array} \right.
$$

Remark 194 (Bermudan Callable): The modification to the backward algorithm to price a Bermudan callable consists of the use of two conditional expectation estimators: one for the continuation value and (additionally) one for the underlying. As before, the conditional expectation estimators are used only for the exercise criterion (and not for the payment). 

Remark 195 (Longstaf-Schwartz): 

• The estimator of the conditional expectation is used in the estimation of the exercise strategy only. 

• The choice of basis functions is crucial to the quality of the estimate. 

Clement, Lamberton and Protter showed convergence of the Longsta´ f-Schwartz regression method to the exact solution, see [60]. 

## 15.10.4. Implementation

## MonteCarloConditionalExpectationLongstaffSchwartz

setBasisFunctionsEstimator(RandomVariable[] basisFunctionsEstimator) setBasisFunctionsPredictor(RandomVariable[] basisFunctionsPredictor) 

getConditionalExpectation(RandomVariable randomVariable) 

Figure 15.10.: UML Diagram: Conditional Expectation Estimator. The method setBasisFunctionsEstimator sets the basis functions which form the matrix X. The method setBasisFunctionsPredictor sets the basisfunctions whichform the matrix $X ^ { * } .$ . These are the same basisfunctions asfor X, but possibly evaluated in an independent Monte-Carlo simulation (to avoid foresight bias). The method getConditionalExpectation calculates the regression parameter $\alpha ^ { * } = ( X ^ { \mathsf { T } } X ) ^ { - 1 } X ^ { \mathsf { T } } \cdot \nu$ from a given vector v and returns the conditional expectation estimator $X ^ { * } \cdot \alpha ^ { * }$ ofv. See Lemma 191. 

The Longstaf-Schwartz conditional expectation estimator may easily be implemented in a corresponding class, independent of the given model or Monte-Carlo simulation - see Figure 15.10. This class contains nothing more than a linear regression, but the methodology may be replaced by alternative algorithms (e.g. non parametric regressions). 

As pointed out in the discussion of the backward algorithm, it is not normally necessary to explicitly calculate the exercise strategy in form of $T$ to <sub>η</sub>. It is suficient to calculate the random variables $\tilde { U } _ { i }$ in a backward recursion. Since finally only $\tilde { U } _ { 1 }$ is needed to calculate the price of the Bermudan option, the $\tilde { U } _ { i } { } ^ { , }$ s may be stored in the same vector of Monte-Carlo realizations. 

## 15.10.5. Binning as linear Least-Square Regression

We return once again to the binning. In Section 15.8.1 it turned out that Binning may be interpreted as least square regression with a specific set of basis functions: The indicator variables of the bins $U _ { j }$ which we denote by 

$$
h _ {j} (\omega) := \left\{ \begin{array}{l l} 1 & \text { for } \omega \in U _ {j} \\ 0 & \text { else. } \end{array} \right.\tag{15.12}
$$

We now give an explicit calculation using the linear regression algorithm with the bin indicator variables as basis functions. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/8e87caaf1e4ed78c968221e1c4aa0be56fe9e051a4925734aa7def9007b0b070.jpg)



Figure 15.11.: Binning using the linear regression algorithm with piecewise constant basis functions: We use 20 bins (basis functions). Each bin consist of approximately the same number ofpaths. Modelund product parameters are as in Figure 15.7.


Let $\omega _ { k }$ denote the paths of a Monte-Carlo simulation and X the matrix $\left( h _ { j } ( \omega _ { k } ) \right)$ , j column index, k row index. Since the $U _ { j } { } ^ { , } \mathrm { s }$ are disjoint we have $X ^ { \mathsf { T } } X = \dim ( m _ { 1 } , \ldots , \bar { m } _ { p } )$ , where $m _ { j }$ is the number of paths for which $h _ { j } ( \omega _ { k } ) = 1$ . Thus we have for the regression parameter 

$$
\alpha^ {*} = (X ^ {\mathsf {T}} X) ^ {- 1} X ^ {\mathsf {T}} \cdot v = \operatorname{diag} (\frac {1}{m _ {1}}, \dots , \frac {1}{m _ {p}}) \cdot X ^ {\mathsf {T}} \cdot v.
$$

It follows that the regression parameter gives the expectation on the corresponding bin 

$$
\alpha_ {j} ^ {*} = \frac {1}{m _ {j}} \sum_ {v _ {k} \in U _ {j}} v _ {k} \quad \text { for } j = 1, \dots , p.
$$

## 15.11. Optimization Methods

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/813aa2bd-ecde-4fff-bcc8-13f3da522d71/a1ff0fc6ac066d322ab3b8142e7cee396cdecf19dda74a36a19dc8fd6c990592.jpg)


Motivation: In the discussion of the backward algorithm it has become obvious that the conditional expectation estimator is needed to derive the optimal exercise strategy only. Since a sub-optimal exercise will lead to a lower Bermudan price the optimal exercise has an alternative characterization: it maximizes the Bermudan value. A solution to the pricing problem of the Bermudan thus consists of maximizing the Bermudan value over a suitable, suficiently large space of admissible<sup>6</sup> exercise strategies. C| 

## 15.11.1. Andersen Algorithm for Bermudan Swaptions

The following method was proposed for the valuation of Bermudan swaptions by L. Andersen in [44]. We thus restrict our presentation to the evaluation of the Bermudan Callable and use the notation of Section 15.10.3. In [44] the method appears less generic than the Longstraf & Schwartz regression. However, one might reformulate the optimization method in a fairly generic way. As the optimization is a high dimensional one, the method then becomes less useful in practice. 

The exercise strategy is given by a parametrized function of the underlyings 

$$
I _ {i} (\lambda) := f (V _ {\mathrm{underl}, i} (T _ {i}, \omega), \dots , V _ {\mathrm{underl}, n - 1} (T _ {i}, \omega), \lambda)
$$

where we replace the optimal exercise 

$$
\tilde {V} _ {\mathrm{underl}, i} (T _ {i}) <   \mathrm{E} ^ {\mathbb {Q}} (\tilde {U} _ {i + 1} \mid \mathcal {F} _ {T _ {i}})
$$

by 

$$
I _ {i} (\lambda) > 0.
$$

Here the function f may represent a variety of exercise criteria, e.g. 

$$
I _ {i} (\omega , \lambda) = V _ {\mathrm{underl}, i} (T _ {i}, \omega) - \lambda .\tag{15.13}
$$

We assume that $I _ { i }$ is such that it may be calculated without resimulation, i.e. we assume that the underlyings $V _ { \mathrm { u n d e r l } , j } ( T _ { i } )$ are either given by an analytic formula or a suitable approximation. E.g. this is the case for a swap within a LIBOR Market Model. If we use the optimization method within the backward algorithm, it now looks as follows: 

<sup>6</sup> By an admissible exercise strategy we denote one that respects the measurability requirements. As we noted, a violation of measurability requirements, i.e. a foresight bias or even perfect foresight, will result in a super-optimal strategy. The Bermudan value with a super-optimal strategy is higher than the Bermudan value with the optimal strategy, however super-optimal exercise is impossible. 

<!-- === Source: MinerU_markdown_Mathematical_Finance-Fries_201_2122706940055363589.md (Page 201) === -->

Induction start: $t > T_{n}$ After the last exercise time we have: 

- The value of the (future) payments is $\tilde{U}_{n+1} = 0$ 

Induction step: $t = T_{i}, i = n, n - 1, n - 2, \ldots 1$ In $T_{i}$ we have: 

- In the case of exercise in $T_{i}$ the value is $\tilde{V}_{\mathrm{underl,i}}(T_i)$ 

- In the case of non-exercise in $T_{i}$ the value is $\tilde{V}_{\mathrm{hold,i}}(T_i) = \mathrm{E}^{\mathbb{Q}}(\tilde{U}_{i + 1}|\mathcal{F}_{T_i})$ . This value is estimated through an optimization for given paths $\omega_{1},\ldots ,\omega_{m}$ : 

$$
\begin{array}{l} - I _ {i} (\lambda , \omega) = f (V _ {\text {underl}, i} (T _ {i}, \omega), \ldots , V _ {\text {underl}, n - 1} (T _ {i}, \omega), \lambda). \\ - \tilde {U} _ {i} (\lambda , \omega) := \left\{ \begin{array}{l l} \tilde {V} _ {\text {underl}, i} (T _ {i}) & \text {if} I _ {i} (\lambda , \omega) > 0 \\ \tilde {U} _ {i + 1} & \text {else.} \end{array} \right. \\ - \tilde {V} _ {\text {berm}, i} (T _ {0}, \lambda) = \mathrm{E} ^ {\mathbb {Q}} (\tilde {U} _ {i} (\lambda)   |   \mathcal {F} _ {T _ {0}})   \approx   \frac {1}{m} \sum_ {k} \tilde {U} _ {i} (\lambda , \omega_ {k}) \\ - \lambda^ {*} = \arg \max _ {\lambda} \left(\frac {1}{m} \sum_ {k} \tilde {U} _ {i} (\lambda , \omega_ {k})\right) \end{array}
$$

- The value of the payments of the product in $T_{i}$ under optimal exercise is given by 

$$
\tilde {U} _ {i} (\omega) := \left\{ \begin{array}{l l} \tilde {V} _ {\text { underl,i }} (T _ {i}) & \text { if } I _ {i} (\lambda^ {*}, \omega) > 0 \\ \tilde {U} _ {i + 1} & \text { else. } \end{array} \right. = \tilde {U} _ {i} (\lambda^ {*}, \omega)
$$

The exercise strategy is estimated in $T_{i}$ by choosing the $\lambda^{*}$ for which $I_{i}$ gives the maximal Bermudan option value. This is done by going backward in time, from exercise date to exercise date. 

## 15.11.2. Review of the Threshold Optimization Method

## 15.11.2.1. Fitting the exercise strategy to the product

Let us apply the optimization method to the pricing of a simple Bermudan option on a stock following a Black-Scholes model. This shows that a too simple choice of the exercise strategy will give surprisingly unreliable results. 

The simple strategy $(15.13)$ fails for the simplest type of Bermudan option. Consider the option to receive 

$$
N _ {1} \cdot (S (T _ {1}) - K _ {1})
$$

in $T_{1}$ or receive 

$$
\max (N _ {2} \cdot (S (T _ {2}) - K _ {2}), 0)
$$

in $T_{2}$ , where - as before $-N_{i}$ and $K_{i}$ denote notional and strike and S follows a Black-Scholes model. This gives us an analytic formula for the option in $T_{2}$ and thus the true optimal exercise. Figure 15.12 shows an example where the optimization of the simple strategy (15.13) gives the value of the Bermudan option. 

A small change in notional $N_{1}$ and strike $K_{1}$ changes the picture. If both are smaller than $N_{2}$ and $K_{2}$ respectively, we obtain two intersection points of the exercise and continuation value. In $T_{1}$ it is optimal to exercise in between these two intersection points. Our simple exercise criterion cannot render this case. Optimizing the threshold parameter $\lambda$ shows two maxima: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/8c51effd4ab835b47fd1c95d2c6c39df8dc6d12519b40458b192d899492d776f.jpg)



- exercise (1. option) — continuation (2. option) — bermudan
- exercise criteria given by threshold



Figure 15.12.: Example of the successful optimization of the exercise criterion (intersection of the two price curves, left). The graph on the right shows the Bermudan option value as a function of the exercise threshold $\lambda$ .


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/3b7f350920ae63b22abef4bffdca68b33aa982bf17fe923c27c7c5443069efd4.jpg)



Figure 15.13.: Example of a failing optimization of the exercise criterion (intersection of the two price curves, left)). The graph on the right shows the Bermudan option value as a function of the exercise threshold $\lambda$ .


the value of the two European options “exercise never” and “exercise always”. Both values are below the true Bermudan option value, see Figure 15.13, right. 

The conclusion of this is example is that the choice of the exercise strategy has to be made carefully in accordance with the product. But this remark applies to some extent to any method. 

## 15.11.2.2. Disturbance of the Optimizer through Discontinuities and local Minima

The Monte-Carlo Bermudan price calculated from the backward algorithm is a discontinuous function of the exercise criterion. The Bermudan price jumps if the exercise criterion $I(\omega, \lambda)$ changes sign for a given path $\omega$ . The price jumps by the difference of exercise value and continuation value. Even in the case of an optimal exercise criterion (i.e. $\lambda = \lambda_{max}$ ) we see a jump in price since even then exercise value and continuation value will generally be different (at optimal exercise, only the expected (!) continuation value equals the exercise value). 

As a function of $\lambda$ , the price will not only exhibit discontinuities, but also small local maxima induced by them, see Figure 15.12 (right). These may prevent the optimizing algorithm from finding the global maxima. 

However, if there are a sufficient number of paths, the local maxima appear only on a small scale. The jumps in price will be of the order $O(\frac{1}{n})$ , where n denotes the number of paths. Thus with a robust minimizer one would rarely encounter this problem. For example consider the case that the limit function (for $n \to \infty$ ) would satisfy an estimate of the form $V_{\max} - V(\lambda) > C(\lambda - \lambda_{\max})^{2}$ , i.e. without the Monte-Carlo discontinuities no other local maxima or saddle point would exist. Then a bisection search on the disturbed function will miss the true maxima only by the order of a jump $O(\frac{1}{n})$ . 

## 15.11.3. Optimization of Exercise Strategy: A more general Formulation

There is a trivial generalization of the optimization method considered in Section 15.11.1: 

- The exercise criterion will be given as a function of arbitrary $\mathcal{F}_{T_i}$ measurable random variables. 

- The exercise criterion will be given as a function of a parameter vector $\lambda \in \mathbb{R}^k$ . 

Thus we replace the "true" exercise criterion used in the backward algorithm 

$$
\tilde {V} _ {\mathrm{underl}, i} (T _ {i}) <   \mathrm{E} ^ {\mathbb {Q}} (\tilde {U} _ {i + 1} \mid \mathcal {F} _ {T _ {i}})
$$

by a function 

$$
I _ {i} (\lambda , \omega) := f (B _ {i, 1} (\omega), \dots , B _ {i, m} (\omega), \lambda),
$$

where $B_{i,j}$ is a set of $\mathcal{F}_{T_i}$ measurable random variables and $\lambda \in \mathbb{R}^k$ . 

## 15.11.4. Comparison of Optimization Method and Regression Method

The difference between the optimization method and the regression method becomes apparent in Figure 15.7-15.9. While the regression method requires the regression functions to give a good fit to the conditional expectations across the whole domain of the independent variable, the optimization method only requires that the functional $I_{i}(\lambda)$ captures the exercise boundary. In Figures 15.7-15.9 the conditional expectation estimator is a curve, but the exercise boundary is given by two points only (the intersection of the conditional expectation estimator with the bisector). 

Thus the optimization method can cope with far fewer parameters than the regression. On the other hand, as noted in the example above, it is far more important that the functional is adapted to the Bermudan product under consideration. 

It is trivial to choose the map $I_{i}(\lambda)$ such that the optimal $\lambda^{*}$ give the same or a better value than the least-square regression. If $B_{i,j}$ denote the basis functions used in the least-square regression for exercise date $T_{i}$ we set 

$$
I _ {i} (\lambda_ {1}, \ldots , \lambda_ {n}) = (\lambda_ {1} B _ {i, 1} + \ldots + \lambda_ {1} B _ {i, m}) - \tilde {V} _ {\mathrm{underl}, i} (T _ {i}).
$$

Then for $\lambda = \alpha^{*}$ , where $\alpha^{*}$ is the regression parameter from the least-square regression, the exercise criterion agrees with the one from the least-square regression. This result however is rarely an advantage of the optimization method since in practice a high dimensional optimization does not represent an alternative. 

## 15.12. Duality Method: Upper Bound for Bermudan Option Prices

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/6dc377372a54374cd3d7805aeaceb0e4c407d0ae5ad6d7ec806bb2b11c47f613.jpg)


Motivation: So far, the ansatz to evaluate a Bermudan option has been to estimate the exercise strategy, i.e. the stopping-time $\tau$ . If this estimate is itself a stopping-time, i.e. no foresight bias is present, then the evaluation with the estimated exercise strategy gives a lower bound for the true value of the Bermudan 

option. The stopping-time $\tau$ maximizes the option price; all other stopping-times give lower prices, because they are sub-obtimal. In order to decide if the given lower bound is sufficiently close to the optimal value, a corresponding upper would come in handy. 

In this section we present a method that gives, in the limit of a vanishing Monte-Carlo error, an upper bound for the Bermundan option value. The upper bound itself converges to the true option value as a given space of test functions converges to the whole space. Putting aside the Monte-Carlo error, together with the lower bound methods (15.8 - 15.11.1) we then obtain an interval for the true value of the Bermudan price. 

The method was introduced by Rogers [87], Haugh & Kogan [73], and originally by Davis & Karatzas [61]. 

## 15.12.1. Foundations

Let us review some foundations: 

Definition 196 (Super-martingale): 

The stochastic process $\{X_t, \mathcal{F}_t; 0 \leq t < \infty\}$ is called a super-martingale with respect to the filtration $\mathcal{F}_t$ and the measure $\mathbb{P}$ , if 

$$
X _ {s} \geq E (X _ {t} | \mathcal {F} _ {s}), \quad \mathbb {P} \text {a.s.}, \quad \forall 0 \leq s <   t <   \infty .
$$

Definition 197 (Stopping-time (time-discrete process)): 

Let $T: \Omega \to \{T_0, \ldots, T_n\}$ denote a random variable. $T$ is called a stopping-time, if 

$$
\{T = T _ {i} \} \in \mathcal {F} _ {T _ {i}}.\tag{15.14}
$$

Remark 198 (Stopping-Time): Equivalent to (15.14) is 

$$
\{T \leq T _ {i} \} \in \mathcal {F} _ {T _ {i}},\tag{15.15}
$$

since $\mathcal{F}_{T_j} \subset \mathcal{F}_{T_i}$ for $T_j < T_i$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/18a8deabbacb8af39c751ef4a5ea08f16868775656b9f08829b93aaf6c1219ce.jpg)


Interpretation: A stopping-time may be viewed as the mathematical representation of an exercise strategy of a Bermudan option. If for a given path $\omega$ , $T(\omega) = T_i$ denotes the time at which an event occurs (e.g. the decision to exercise an option), then (15.15) constitutes the requirement that the decision is based on that is available on or before $T_i$ - expressed through the $\mathcal{F}_T$ -measurability. 

information that is available on or before $T_{i}$ - expressed through the $F_{T_{i}}$ -measurability. 

The condition (15.15) precludes a foresight bias. Compare Section 15.6 $^{7}$ . 

< 

Given a stochastic process and a stopping-time, we may construct the stopped process: 

## Definition 199 (Stopped Process):

Let $X$ denote a stochastic process and $T$ a stopping-time. The process $X^T$ given through $X$ stopped in $T$ , is defined by 

$$
X ^ {T} (t, \omega) = \left\{ \begin{array}{l l} X (t, \omega) & t <   T (\omega) \\ X (T (\omega), \omega) & t \geq T (\omega). \end{array} \right.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/e1c496a8b62fa0b21270c5ee338e4efc7914754f1ff87e17da8e842f11bda0d7.jpg)


Interpretation: On every path $\omega$ the stopped process $X^{T}$ coincides with X for times before the stopping-time. For times on or after the stopping-time the stopped process takes the constant value of X at the stopping-time. It is stopped. This is similar to what happens for the (relative) price of a Bermudan option. 

Before the exercise date, the option value is stochastic. Upon exercise the value is frozen to the value upon exercise. 

## Definition 200 (Snell Envelope):

Let $Z$ denote a time-discrete adapted process and $U$ defined by 

$$
\begin{array}{l} U (T _ {n}) = Z (T _ {n}) \\ U (T _ {i}) = \max (Z (T _ {i}), \operatorname{E} (U (T _ {i + 1}) \mid \mathcal {F} _ {T _ {i}}). \end{array}
$$

The process $U$ is called Snell envelope of $Z$ . 

Lemma 201 (Snell Envelope): The Snell envelope of Z is the smallest super-martingale which dominates Z. 

$^{7}$ For the example discussed in Section 15.6 $T(\omega_{1}) = T(\omega_{2}) = T_{1}$ and $T(\omega_{1}) = T(\omega_{2}) = T_{2}$ are both stopping-times (check!), however the super-optimal exercise strategy $T(\omega_{1}) = T_{1}$ , $T(\omega_{2}) = T_{2}$ is not a stopping-time. 

Theorem 202 (Doob-Meyer Decomposition): Let $U$ denote a (time-discrete) supermartingale. Then there exists a (unique) decomposition 

$$
U (T _ {i}) = M (T _ {i}) - A (T _ {i}),
$$

where M is a (time-discrete) martingale and A is a (time-discrete) previsible non-decreasing process (i.e. $A(T_{i-1}, \omega) \leq A(T_i, \omega)$ ) where $A(T_0) = 0$ . 

Proof: 

$$
\begin{array}{l l} M (T _ {i}) := M (T _ {i - 1}) + U _ {i} - \mathrm{E} (U _ {i} \mid \mathcal {F} _ {T _ {i - 1}}) & M (T _ {0}) = U (T _ {0}) \\ A (T _ {i}) := A (T _ {i - 1}) + U _ {i - 1} - \mathrm{E} (U _ {i} \mid \mathcal {F} _ {T _ {i - 1}}) & A (T _ {0}) = 0 \end{array}
$$

□| 

## 15.12.2. American Option Evaluation as Optimal Stopping Problem

We repeat the Bermudan option evaluation as optimal stopping: Let $0 = T_{0} < T_{1} < \ldots < T_{n}$ . Let $V_{\text{underl}}(T_{i}), i = 1, \ldots, n - 1$ denote a sequence of $F_{T_{i}}$ -measurable random variables, giving the value of financial products at time $T_{i}$ . We define recursively 

$$
V _ {\text { b   e   r   m }} \left(T _ {i}\right) := \max \left(V _ {\text { u   n   d   e   r   l }} \left(T _ {i}\right), \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(V _ {\text { b   e   r   m }} \left(T _ {i + 1}\right) \cdot \frac {N \left(T _ {i}\right)}{N \left(T _ {i + 1}\right)} \mid \mathcal {F} _ {T _ {i}}\right)\right),
$$

where $(N, \mathbb{Q}^{N})$ denotes a given numéraire-martingale measure pair. Furthermore let $\tilde{V}_{\mathrm{U}}(T_{i}) := \frac{V_{\mathrm{underl}}(T_{i})}{N(T_{i})}$ , $\tilde{V}_{\mathrm{B}}(T_{i}) := \frac{V_{\mathrm{berm}}(T_{i})}{N(T_{i})}$ denote the corresponding N-relative prices, i.e. 

$$
\tilde {V} _ {\mathrm{B}} (T _ {i}) := \max (\tilde {V} _ {\mathrm{U}} (T _ {i}), \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\tilde {V} _ {\mathrm{B}} (T _ {i + 1}) \mid \mathcal {F} _ {T _ {i}}).
$$

Theorem 203 (American Option Price - Dual Formulation (Rogers) (time-continuous version)): Let 

$$
V _ {\text { amer }} (0) := \sup _ {T \text {   stoppingtime }} \mathrm{E} (\tilde {V} _ {\mathrm{U}} (T) \mid \mathcal {F} _ {0}).
$$

Then 

$$
V _ {\text { amer }} (0) = \inf _ {M \in H _ {0} ^ {1}} \operatorname{E} (\sup _ {0 \leq t \leq T} (\tilde {V} _ {\mathrm{U}} (t) - M (t)) \mid \mathcal {F} _ {0}),
$$

where $H_0^1$ denotes the set of all martingales $M$ with $\sup_{0 \leq t \leq T} |M(t)| \in \mathrm{L}_1(\Omega)$ and $M(0) = 0$ . 

Since we consider only the evaluation of Bermudan options, i.e. options a finite number of exercise dates, we give a time-discrete version of Theorem 203: 

Theorem 204 (Bermudan Option Price - Dual Formulation (Rogers) (time-discrete version)): Let 

$$
\tilde {V} _ {\mathrm{B}} (T _ {i}) := \max (\tilde {V} _ {\mathrm{U}} (T _ {i}), \operatorname{E} (\tilde {V} _ {\mathrm{B}} (T _ {i + 1}) | \mathcal {F} _ {T _ {i}})).
$$

$$
\tilde {V} _ {\mathrm{B}} (T _ {0}) = \inf _ {M \in H _ {0} ^ {1}} \operatorname{E} (\max _ {T _ {i}} (\tilde {V} _ {\mathrm{U}} (T _ {i}) - M (T _ {i})) \mid \mathcal {F} _ {0}),\tag{15.16}
$$

where $H_{0}^{1}$ denotes the set of all (time-discrete) martingales M with 

$$
\begin{array}{l} M (T _ {0}) = 0 \\ M (T _ {i}) = \operatorname{E} (M (T _ {i + 1}) | \mathcal {F} _ {T _ {i}}) \end{array}
$$

$$
M (T _ {i}) \in \mathrm{L} _ {1} (\Omega)
$$

and $\max_{T_i}(\tilde{V}_{\mathrm{U}}(T_i) - M(T_i))$ has to be understood pathwise, i.e. 

$$
\max _ {T _ {i}} (\tilde {V} _ {\mathrm{U}} (T _ {i}) - M (T _ {i})) [ \omega ] = \max _ {T _ {i}} (\tilde {V} _ {\mathrm{U}} (T _ {i}, \omega) - M (T _ {i}, \omega))
$$

(and not as a maximum over all stopping-times). 

Remark 205 (on Theorem 204): First, it is worth noting that in Theorem 204 the maximum is applied pathwise. If the pathwise maximum is applied to $V_{\mathrm{underl}}$ then $\max_{T_i}(V_{\mathrm{underl}}(T_i))$ gives the value of a perfect foresight. As we will show in Lemma 206, a foresight error is precluded by the martingale $M$ . 

The expectation in (15.16) is conditioned to $F_{T_{0}} = F_{0}$ only, i.e. it is not required to calculate a conditional expectation at a later time. However, the expectation has to be minimized over all martingales M. This is as complex as the calculation of the optimal exercise strategy (by maximizing over all stopping-times $\tau$ ). But Theorem 204 indeed gives an upper bound for the value of the Bermudan option: 

$$
V _ {\text { berm }} (T _ {0}) \leq \mathrm{E} ^ {\mathbb {Q} ^ {N}} \Bigl (\max _ {T _ {i}} (V _ {\text { underl }} (T _ {i}) \cdot \frac {N (0)}{N (T _ {i})} - M (T _ {i}) \mid \mathcal {F} _ {0}) \Bigr), \quad M \in H _ {0} ^ {1},
$$

and this upper bound may be arbitrarily close to the option price $V_{\mathrm{berm}}(T_{0})$ if M is suitably chosen. 

Lemma 206 (Eliminating Foresight): 

Let $\tilde{V}_{\mathrm{U}}(T_i)$ , $\tilde{V}_{\mathrm{B}}(T_i)$ be as before, i.e. 

$$
\tilde {V} _ {\mathrm{B}} (T _ {i}) := \max _ {T _ {i}} (\tilde {V} _ {\mathrm{U}} (T _ {i}), \operatorname{E} (\tilde {V} _ {\mathrm{B}} (T _ {i + 1}) | \mathcal {F} _ {T _ {i}})),\tag{15.17}
$$

and $M$ as in the Doob-Meyer decomposition of $\tilde{V}_{\mathrm{B}}(T_i)$ 

$$
\begin{array}{l} M (T _ {0}) := 0, \\ M (T _ {i}) := M (T _ {i - 1}) + \tilde {V} _ {\mathrm{B}} (T _ {i}) - \operatorname{E} (\tilde {V} _ {\mathrm{B}} (T _ {i + 1}) \mid \mathcal {F} _ {T _ {i}}). \end{array}\tag{15.18}
$$

Let $T^{\text{opt}} : \Omega \to \{T_1, \ldots, T_n\}$ denote the (optimal) stopping-time given by 

$$
T ^ {\mathrm{opt}} (\omega) := \min \left\{T _ {j}: \tilde {V} _ {\mathrm{U}} \left(T _ {j}, \omega\right) \geq \mathrm{E} \left(\tilde {V} _ {\mathrm{B}} \left(T _ {j + 1}\right) \mid \mathcal {F} _ {T _ {j}}\right) [ \omega ] \right\}
$$

(this implies $\tilde{V}_{\mathrm{B}}(T_0) = \mathrm{E}(\tilde{V}_{\mathrm{U}}(T^{\mathrm{opt}})\mid \mathcal{F}_{T_0}))$ 

Then we have (pathwise!) 

$$
\max _ {T _ {j}} (\tilde {V} _ {\mathrm{U}} (T _ {j}, \omega) - M (T _ {j}, \omega)) = \tilde {V} _ {\mathrm{U}} (T ^ {\mathrm{opt}} (\omega), \omega) - M (T ^ {\mathrm{opt}}, \omega).
$$

Proof: We give the proof only with $(15.17)$ and $(15.18)$ . Let $\omega \in \Omega$ . By definition we have 

$$
\tilde {V} _ {\mathrm{B}} (T _ {j}, \omega) = \mathrm{E} (\tilde {V} _ {\mathrm{B}} (T _ {j + 1}) \mid \mathcal {F} _ {T _ {j}}) [ \omega ]
$$

$$
\text { for } T _ {j} <   T ^ {\mathrm{opt}} (\omega)\tag{15.19}
$$

$$
\tilde {V} _ {\mathrm{B}} (T _ {j}, \omega) \geq \mathrm{E} (\tilde {V} _ {\mathrm{B}} (T _ {j + 1}) | \mathcal {F} _ {T _ {j}}) [ \omega ]
$$

$$
\mathrm{for} T _ {j} \geq T ^ {\mathrm{opt}} (\omega)\tag{15.20}
$$

and 

$$
\tilde {V} _ {\mathrm{B}} (T _ {i}, \omega) = \tilde {V} _ {\mathrm{U}} (T _ {i}, \omega)
$$

$$
\mathrm{for} T _ {i} = T ^ {\mathrm{opt}} (\omega).\tag{15.21}
$$

1. For $T_{i} = T^{\mathrm{opt}}(\omega)$ and $T_{j} < T_{i}$ we have 

$$
\begin{array}{l l} \bullet & \tilde {V} _ {\mathrm{U}} (T _ {i}, \omega) - M (T _ {i}, \omega) = \tilde {V} _ {\mathrm{B}} (T _ {i}, \omega) - M (T _ {i}, \omega) \\ \bullet & \tilde {V} _ {\mathrm{B}} (T _ {j + 1}, \omega) - M (T _ {j + 1}, \omega) \\ & = \underline {{\tilde {V} _ {\mathrm{B}} (T _ {j + 1} , \omega)}} - M (T _ {j}, \omega) - \underline {{\tilde {V} _ {\mathrm{B}} (T _ {j + 1} , \omega)}} + \mathrm{E} (\tilde {V} _ {\mathrm{B}} (T _ {j + 1}, \omega) | \mathcal {F} _ {T _ {j}}) [ \omega ] \\ & = \tilde {V} _ {\mathrm{B}} (T _ {j}, \omega) - M (T _ {j}, \omega) \\ \bullet & \tilde {V} _ {\mathrm{B}} (T _ {j}, \omega) - M (T _ {j}, \omega) \geq \tilde {V} _ {\mathrm{U}} (T _ {j}, \omega) - M (T _ {j}, \omega) \end{array}
$$

and thus for $T_{j}\leq T_{i}$ : 

$$
\tilde {V} _ {\mathrm{U}} (T _ {j}, \omega) - M (T _ {j}, \omega) \leq \tilde {V} _ {\mathrm{U}} (T _ {i}, \omega) - M (T _ {i}, \omega)
$$

2. For $T_{i} = T^{\mathrm{opt}}(\omega)$ and $T_{j} > T_{i}$ we have 

$$
\begin{array}{l l} \bullet & \tilde {V} _ {\mathrm{U}} (T _ {i}, \omega) - M (T _ {i}, \omega) \\ & = \tilde {V} _ {\mathrm{U}} (T _ {i}, \omega) - M (T _ {i + 1}, \omega) + \tilde {V} _ {\mathrm{B}} (T _ {j + 1}, \omega) - \mathrm{E} (\tilde {V} _ {\mathrm{B}} (T _ {j + 1}) | \mathcal {F} _ {T _ {j}}) [ \omega ] \\ & = \tilde {V} _ {\mathrm{B}} (T _ {i}, \omega) - M (T _ {i + 1}, \omega) + \tilde {V} _ {\mathrm{B}} (T _ {j + 1}, \omega) - \mathrm{E} (\tilde {V} _ {\mathrm{B}} (T _ {j + 1}) | \mathcal {F} _ {T _ {j}}) [ \omega ] \\ & \geq \tilde {V} _ {\mathrm{B}} (T _ {i + 1}, \omega) - M (T _ {i + 1}, \omega) \\ \bullet & \tilde {V} _ {\mathrm{B}} (T _ {j}, \omega) - M (T _ {j}, \omega) \\ & = \tilde {V} _ {\mathrm{B}} (T _ {j}, \omega) - M (T _ {j + 1}, \omega) + \tilde {V} _ {\mathrm{B}} (T _ {j + 1}, \omega) - \mathrm{E} (\tilde {V} _ {\mathrm{B}} (T _ {j + 1},) | \mathcal {F} _ {T _ {j}}) [ \omega ] \\ & \geq \tilde {V} _ {\mathrm{B}} (T _ {j + 1}, \omega) - M (T _ {j + 1}, \omega) \\ \bullet & \tilde {V} _ {\mathrm{B}} (T _ {j + 1}, \omega) - M (T _ {j + 1}, \omega) \geq \tilde {V} _ {\mathrm{U}} (T _ {j + 1}, \omega) - M (T _ {j + 1}, \omega) \end{array}
$$

and thus for $T_{j}\geq T_{i}$ 

$$
\tilde {V} _ {\mathrm{U}} (T _ {i}, \omega) - M (T _ {i}, \omega) \geq \tilde {V} _ {\mathrm{U}} (T _ {j}, \omega) - M (T _ {j}, \omega).
$$

Thus, for all $T_{j}$ 

$$
\tilde {V} _ {\mathrm{U}} (T _ {i}, \omega) - M (T _ {i}, \omega) \geq \tilde {V} _ {\mathrm{U}} (T _ {j}, \omega) - M (T _ {j}, \omega).
$$

□ 

Remark 207 (Foresight Bias): The Lemma 206 shows that the martingale $M$ eliminates the foresight bias. We have 

$$
\tilde {V} _ {\mathrm{U}} (T _ {i}) - M (T _ {i}) \geq \tilde {V} _ {\mathrm{U}} (T _ {j}) - M (T _ {j})
$$

$$
\forall T _ {j},
$$

however, in general 

$$
\tilde {V} _ {\mathrm{U}} (T _ {i}) \ngeq \tilde {V} _ {\mathrm{U}} (T _ {j})
$$

$$
\forall T _ {j}.
$$

Lemma 208 (Optimal Stopping): It is 

$$
\operatorname{E} (\tilde {V} _ {\mathrm{U}} (T ^ {\mathrm{opt}}) \mid \mathcal {F} _ {T _ {0}}) = \operatorname{E} (\max _ {T _ {j}} (\tilde {V} _ {\mathrm{U}} (T _ {j}) - M (T _ {j})) \mid \mathcal {F} _ {T _ {0}}).
$$

Proof: It is 

$$
\begin{array}{c} \operatorname{E} (\tilde {V} _ {\mathrm{U}} (T ^ {\mathrm{opt}}) \mid \mathcal {F} _ {T _ {0}}) \stackrel {{\text {Def.} T ^ {\mathrm{opt}}}} {{=}} \operatorname{E} (\underset {T \text {stopping - time}} {\sup} \tilde {V} _ {\mathrm{U}} (T) \mid \mathcal {F} _ {T _ {0}}) \\ = \operatorname{E} (\underset {T \text {stopping - time}} {\sup} \tilde {V} _ {\mathrm{U}} (T) - M (T) \mid \mathcal {F} _ {T _ {0}}) \\ \stackrel {{\text {La.} 2 0 6}} {{=}} \operatorname{E} (\underset {T _ {i}} {\max} \tilde {V} _ {\mathrm{U}} (T _ {i}) - M (T _ {i}) \mid \mathcal {F} _ {T _ {0}}) \end{array}
$$

## 15.13. Primal-Dual Method: Upper and Lower Bound

The calculation of the exercise strategy and from it the price of the Bermudan option via an (approximation) of the conditional expectation is called primal. The calculation of the exercise strategy via the stopping-time through 15.12 is called dual. 

With the result from Lemma 206 we can combine both methods. From Theorem 204 and Lemma 206 we have 

$$
\tilde {V} _ {\mathrm{B}} (T _ {0}) = \operatorname{E} (\max _ {T _ {i}} (\tilde {V} _ {\mathrm{U}} (T _ {i}) - M (T _ {i})) | \mathcal {F} _ {0}),\tag{15.22}
$$

with 

$$
M (T _ {i}) := M (T _ {i - 1}) + U _ {i} - \mathrm{E} (U _ {i} \mid \mathcal {F} _ {T _ {i - 1}}) \quad M (T _ {0}) = U (T _ {0}).\tag{15.23}
$$

The conditional expectation in $(15.23)$ can be estimated with a primal method. If the conditional expectation has already been estimated in an calculation of the lower bound or the Bermudan option price, then $(15.22)$ immediately gives a corresponding upper bound. 

Compare also [45]. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/f23f1681d8b49e2f11945321e46f780d206e7c8611ed3d830b38e36b506aa875.jpg)


Further Reading: The books [16] and [18] and the article [53] consider Monte-Carlo methods for derivative pricing in general. In [60] the convergence of the regression methods is proven. The optimization method for Bermudan swaptions is given in [44], a primal-dual method is given in [45]. The discussion ght bias is found in [64]. 

of the foresight bias is found in [64]. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/993ea7e6bc02efab3ba85279e9f48c50e8436e47d4154af360ad5739904d9641.jpg)


Experiment: At http://www.christian-fries.de/finmath/applets/BermudanStockOptionPricing.html the evaluation of a Bermudan option on a stock following a Black-Scholes model may be studied. There is a choice of different evaluation methods. 

# Pricing Path Dependent Options in a Backward Algorithm

A backward algorithm - e.g. as given by a model implemented as a lattice - allows the calculation of the conditional expectation 

$$
V (T _ {i - 1}) = N (T _ {i - 1}) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {V (T _ {i})}{N (T _ {i})} \mid \mathcal {F} _ {T _ {i - 1}}\right),
$$

and thus defines induction steps $T_{i} \rightarrow T_{i-1}$ backward in time. Path-dependent quantities cannot be considered directly. One way of allowing for path-dependent quantities in a backward algorithm is to eliminate the path-dependency by extending the state space. 

## 16.1. State Space Extension

Let V denote a product whose time $T_{i}$ value depends on a quantity $C_{i}$ given by an update rule 

$$
C _ {i} = f (T _ {i}, C _ {i - 1}, X _ {i}), \quad C _ {0} = \text { constant },\tag{16.1}
$$

were $X_{i}$ is a random variable that is a function of the time $T_{i}$ values of the model primitives, i.e. non-path dependent. Thus $X_{i}$ and hence $C_{i}$ are $F_{T_{i}}$ measurable. Equation (16.1) constitutes the path-dependency of $C_{i}$ ; it may not be written as a function of the time $T_{i}$ values of the model primitives. It depends on the past since it depends on the previous value $C_{i-1}$ . 

To remove the path-depency in V we add $C_{i}$ as an additional state. We consider the time $T_{i}$ value of V as a function of $C_{i}$ 

$$
V (T _ {i}) = V (T _ {i}, C _ {i}), \qquad i = 0, 1, \ldots , n.
$$

Then backward algorithm is: 

- Given $V(T_{i},C_{i})$ . 

- Apply the update rule to define 

$$
\tilde {V} (T _ {i}, C _ {i - 1}, X _ {i}) := V (T _ {i}, f (C _ {i - 1}, X _ {i}))\tag{16.2}
$$

- Define 

$$
V (T _ {i - 1}, C _ {i - 1}) := N (T _ {i - 1}) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {\tilde {V} (T _ {i} , C _ {i - 1} , X _ {i})}{N (T _ {i})} \mid \mathcal {F} _ {T _ {i - 1}}\right).\tag{16.3}
$$

Note that conditional to $\mathcal{F}_{T_{i - 1}}$ the state $C_{i - 1}$ is a constant. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/c0107fd2bfb7d0461a05a04ed44b280cdafe437d67c3462b823a2d31ffaf345a.jpg)


Interpretation (State Space Extension): The method is called state space extension because the discrete stochastic process $T_{i} \mapsto C(T_{i}) := C_{i}$ can be interpreted as an additional state of the model and (16.1) defines the evolution of this process. Seen over this extended space the product is non-path dependent. 

## 16.2. Implementation

In order to implement the state space extension we discretize the additional state random variables $C_{i}$ into $k_{i}$ state values 

$$
C _ {i} \in \{c _ {i, 1}, \dots , c _ {i, k _ {i}} \}.
$$

For the implementation of the update rule $(16.2)$ an interpolation has to be used, e.g. a linear interpolation 

$$
\frac {f \left(c _ {i - 1 , j} , X _ {i}\right) - c _ {i , l _ {j}}}{c _ {i , l _ {j} + 1} - c _ {i , l _ {j}}} V \left(T _ {i}, c _ {i, l _ {j} + 1}\right) + \frac {c _ {i , l _ {j} + 1} - f \left(c _ {i - 1 , j} , X _ {i + 1}\right)}{c _ {i , l _ {j} + 1} - c _ {i , l _ {j}}} V \left(T _ {i}, c _ {i, l _ {j}}\right),
$$

where $l_{j}$ is such that $c_{i,l_j} \leq f(c_{i-1,j}, X_i) < c_{i,l_j+1}$ . 

Then the conditional expectation (16.3) is calculated for each state realization $c_{i-1,j}$ giving $V(T_{i-1},c_{i-1,1}),\ldots,V(T_{i-1},c_{i-1,k_{i}})$ . 

Remark 209: For some products the value $V(T_{i}, c)$ is linear in c. In such cases two states are sufficient and the approximation of the update rule by the linear interpolation is exact. Examples are zero structures, where the additional state is the accrued notional; the value of the future cashflow is linear in the notional. 

## 16.3. Examples

We illustrate the method of state space extension for the valuation of a Snowball / Memory (Definition 164) and for the evaluation of a Flexi-Cap (Definition 169). 

## 16.3.1. Evaluation of a Snowball in a Backward Algorithm

A Snowball / Memory pays a coupon $C_i$ in $T_{i+1}$ which depends on the previous coupon. The coupon $C_i$ is given by an update rule 

$$
C _ {i} = f (T _ {i}, C _ {i - 1}, X _ {i})
$$

with an $\mathcal{F}_{T_i}$ -measurable $X_{i}$ (the index), i.e. $C_i$ is path-dependent. 

We add the value of the coupon $C_i$ as an additional state and write the product value as a function of this state. 

The backward induction from 16.1 gives the product value $V(T_0, C_0)$ as a function of the initial (or past) coupon $C_0$ , which is known. 

Remark 210 (In Arrears Fixing): Note that we assumed that the index $X_{i}$ is a function of the time $T_{i}$ values of the model primitives and thus $F_{T_{i}}$ -measurable. If the index $X_{i-1}$ is a function of the time $T_{i}$ values of the model primitives, i.e. fixed in arrears, then the additional state variable is the value of the previous coupon. 

## 16.3.2. Evaluation of a Flexi Cap in a Backward Algorithm

An Auto Cap pays at time $T_{i+1}$ the amount 

$$
\begin{array}{l} X _ {i} := N \cdot \max \left(L _ {i} (T _ {i}) - K _ {i}, 0\right) \cdot (T _ {i + 1} - T _ {i}) \\ \quad . \left\{ \begin{array}{l l} 1 & \text { if } | \{j: j <   i \text { and } L _ {j} (T _ {j}) - K _ {j} > 0 \} | <   n _ {\max \mathrm{Ex}} \\ 0 & \text { else }, \end{array} \right. \end{array}
$$

where $L_{i}(t) := L(T_{i}, T_{i+1}; t)$ denotes the forward rate for the period $[T_{i}, T_{i+1}]$ seen in $t \leq T_{i}$ . 

As a function of the processes $L_{i}$ the payoff $X_{i}$ is path-dependent since the payoff function is not given by the random variables $L_{k}(T_{i})$ alone, but also by the past realizations of the processes $L_{k}$ (entering though $L_{j}(T_{j}), j < i$ ). 

We extend the model by the stochastic process 

$$
\begin{array}{c} \eta (t): \Omega \to \{0, \ldots , n - 1 \}, \\ \omega \mapsto \big | \{L _ {j} (T _ {j}) - K > 0 \mid T _ {j} \leq t, j = 1, \ldots , n - 1 \} \big |. \end{array}
$$

Given $L_{i}, \eta$ the payoffs $X_{i}$ are a function of the realizations $L_{i}(T_{i}), \eta(T_{i})$ : 

$$
X _ {i} := N \cdot \max \left(L _ {i} (T _ {i}) - K _ {i}, 0\right) \cdot (T _ {i + 1} - T _ {i}) \cdot \left\{ \begin{array}{l l} 1 & \text { if } \eta (T _ {j}) <   n _ {\max \mathrm{Ex}} \\ 0 & \text { else. } \end{array} \right.
$$

# Sensitivities (Partial Derivatives) of Monte-Carlo Prices

## 17.1. Introduction

The technique of risk-neutral pricing, i.e. the change towards the martingale measure, allows us to calculate the cost of a (self-financing) replication portfolio, to be expressed as an expectation. Determination of the replication portfolio itself is not necessary. However, once a pricing formula or pricing algorithm (e.g. a Monte-Carlo simulation) has been derived, the replication portfolio can be given in terms of the partial derivatives of the price with respect to current model parameters (like the initial values of the underlyings). $^{1}$ The partial derivatives of the price with respect to the model parameters are also called sensitivities or Greeks. They are important to assess the risk of a financial product, see also Chapter 7. 

For complex products, like Bermudan options, an analytic pricing formula is usually not available. The pricing has to be done numerically. Under a high-dimensional model, like the LIBOR market model, the numerical method of choice is usually a Monte-Carlo simulation. Given that, we will investigate the numerical calculation of sensitivities (partial derivatives) of Monte-Carlo prices. 

The simplest way of calculating a derivative is by applying finite differences. Unfortunately, this can lead to a Monte-Carlo algorithm giving unstable or inaccurate results. 

## 17.2. Problem Description

Let us consider a pricing algorithm that uses Monte-Carlo simulation to calculate a price of a financial product as the expectation of the numéraire-relative value under an equivalent martingale measure $\mathbb{Q}$ 

$$
V (t _ {0}) = N (t _ {0}) \cdot \mathrm{E} ^ {\mathbb {Q}} \left(\frac {V (T)}{N (T)} \mid \mathcal {F} _ {t _ {0}}\right).
$$

We are interested in the calculation of a partial derivative of $V(t_{0})$ with respect to some model parameter, e.g. the initial values of the underlying ( $\rightarrow$ delta), the volatility ( $\rightarrow$ vega), etc. 

Since we treat this problem as a general numerical problem, not necessarily related to derivative pricing, we do not adopt a specific model but use a notation that is slightly more general. To fix notation, let us restate Monte-Carlo pricing first: 

## 17.2.1. Pricing using Monte-Carlo Simulation

Assume that our model is given as a stochastic process X, for example an Itô process 

$$
\mathrm{d} X = \mu \mathrm{d} t + \sigma \cdot \mathrm{d} W (t)
$$

modeling our model primitives like functions of the underlyings (e.g. financial products (stocks) or rates (forward rates, swap rates, fx rates)). For example, for the Black-Scholes model we would have $X = (\log(S), \log(B))$ . Let $X^{*}(t_{i})$ denote an approximation of $X(t_{i})$ generated by some (time-)discretization scheme, e.g. an Euler scheme 

$$
X ^ {*} (t _ {i + 1}) = X ^ {*} (t _ {i}) + \mu (t _ {i}) \Delta t _ {i} + \sigma (t _ {i}) \cdot \Delta W (t _ {i})
$$

or one of the more advanced schemes $^{2}$ . We assume that our financial product depends only on realizations of X at a finite number of time points, i.e. we assume that the risk-neutral pricing of the financial product may be expressed as the expectation (with respect to the pricing measure) of a function f of some realizations $Y := (X(t_{0}), X(t_{1}), \ldots, X(t_{m}))$ . This is true for many products (e.g. Bermudan options). If these are approximated through the realizations of the numerical scheme we have: 

$$
\operatorname{E} (f (Y) | \mathcal {F} _ {t _ {0}}) \approx \operatorname{E} (f (Y ^ {*}) | \mathcal {F} _ {t _ {0}}) = \operatorname{E} (f ((X ^ {*} (t _ {0}), X ^ {*} (t _ {1}), \ldots , X ^ {*} (t _ {m}))) | \mathcal {F} _ {t _ {0}}).
$$

Here f denotes the numéraire-relative payoff function. 

The Monte-Carlo pricing consists of the averaging over some (often equidistributed) sample paths $\omega_{i}, i = 1, \ldots, n$ 

$$
\mathrm{E} (f (Y ^ {*}) | \mathcal {F} _ {t _ {0}}) \approx \hat {\mathrm{E}} (f (Y ^ {*}) | \mathcal {F} _ {t _ {0}}) := \frac {1}{n} \sum_ {i = 1} ^ {n} f (Y ^ {*} (\omega_ {i})).
$$

To summarize: we have two approximation steps involved: The first one approximates the time-continuous process by a time-discrete process. The second one approximates the expectation by a Monte-Carlo simulation of n sample paths. This is the minimum requirement to have the pricing implemented as a Monte-Carlo simulation. 

## 17.2.2. Sensitivities from Monte-Carlo Pricing

Assume that $\theta$ denotes some model parameter $^{3}$ or a parametrization of a generic market data movement and let $Y_{\theta}$ denote the model realizations dependent on that parameter. Let us further assume that $\phi_{Y_{\theta}}$ denotes the probability density of $Y_{\theta}$ . Then the analytic calculation of the sensitivity is given by 

$$
\frac {\partial}{\partial \theta} \mathrm{E} (f (Y _ {\theta}) | \mathcal {F} _ {t _ {0}}) = \frac {\partial}{\partial \theta} \int_ {\mathbb {R} ^ {m}} f (y) \phi_ {Y _ {\theta}} (y) \mathrm{d} y.
$$

While the payoff f may be discontinuous, the density in general is a smooth function of $\theta$ . In which case the expectation $\mathrm{E}(f(Y_{\theta})|\mathcal{F}_{t_{0}})$ (the price) is a smooth function of $\theta$ , too. The price inherits the smoothness of $\phi_{Y_{\theta}}$ . 

The calculation of sensitivities using finite differences on a Monte-Carlo based pricing algorithm is known to exhibit instabilities, if the payoff function is not smooth enough, e.g. if the payoff exhibits discontinuities as for a digital option. The difficulties arise when we consider the Monte-Carlo approximation. It inherits the regularity of the payoff f, not that of the density $\phi$ : 

$$
\hat {\mathrm{E}} (f (Y _ {\theta}) | \mathcal {F} _ {t _ {0}}) = \frac {1}{n} \sum_ {i = 1} ^ {n} f (Y _ {\theta} (\omega_ {i})).
$$

So while $\mathrm{E}(f(Y_{\theta})|\mathcal{F}_{t_{0}})$ may be smooth in $\theta$ , the Monte-Carlo approximation $\hat{\mathrm{E}}(f(Y_{\theta})|\mathcal{F}_{t_{0}})$ may have discontinuities. In this case a finite difference approximation of the derivative applied to the Monte-Carlo pricing will perform poorly. 

## 17.2.3. Example: The Linear and the Discontinuous Payout

The challenge in calculating Monte-Carlo sensitivities becomes obvious if we consider two very simple examples: 

## 17.2.3.1. Linear Payout

First consider a linear payout, say 

$$
f (X (T)) = a \cdot X (T) + b.
$$

The (discounted) payout depends only on the time T realization of X (as one would have for a European option). Let $Y_{\theta}(\omega) := X(T, \omega, \theta)$ , where $\theta$ denotes some model parameter. The partial derivative of the Monte-Carlo value of the payout with respect to $\theta$ is 

$$
\frac {\partial}{\partial \theta} \hat {\mathrm{E}} (f (Y _ {\theta}) | \mathcal {F} _ {t _ {0}}) = \frac {1}{n} \sum_ {i = 1} ^ {n} \frac {\partial}{\partial \theta} f (Y _ {\theta} (\omega_ {i})) = \frac {1}{n} \sum_ {i = 1} ^ {n} a \cdot \frac {\partial}{\partial \theta} Y _ {\theta} (\omega_ {i})
$$

Obviously the accuracy of the Monte-Carlo approximation depends on the variance of $\frac{\partial Y_{\theta}}{\partial\theta}$ only. When $\frac{\partial}{\partial\theta}Y_{\theta}(\omega_{i})$ does not depend on $\omega_{i}$ , then the Monte-Carlo approximation gives the exact value of the partial derivative, even if we use only a single path. 

## 17.2.3.2. Discontinuous Payout

Next, consider a discontinuous payout, say 

$$
f (X (T)) = \left\{ \begin{array}{l l} 1 & \text { if } X (T) > K \\ 0 & \text { else. } \end{array} \right.
$$

Analytically we know from $Y_{\theta + h} = Y_{\theta} + \frac{\partial Y_{\theta}}{\partial \theta} \cdot h + O(h^2)$ and 

$$
\mathrm{E} ^ {\mathbb {Q}} (f (Y _ {\theta + h}) \mid \mathcal {F} _ {t _ {0}}) = \mathbb {Q} (\{Y _ {\theta} > K - \frac {\partial Y _ {\theta}}{\partial \theta} \cdot h - O (h ^ {2}) \}) = \int_ {K - \frac {\partial Y _ {\theta}}{\partial \theta} \cdot h - O (h ^ {2})} ^ {\infty} \phi_ {Y _ {\theta}} (y) \mathrm{d} y
$$

that 

$$
\lim _ {h \to 0} \frac {1}{2 h} (\mathrm{E} ^ {\mathbb {Q}} (f (Y _ {\theta + h}) \mid \mathcal {F} _ {t _ {0}}) - \mathrm{E} ^ {\mathbb {Q}} (f (Y _ {\theta - h}) \mid \mathcal {F} _ {t _ {0}})) = \phi_ {Y _ {\theta}} (K) \cdot \frac {\partial Y _ {\theta}}{\partial \theta}.
$$

However, the partial derivative of the Monte-Carlo value of the payout is 

$$
\frac {\partial}{\partial \theta} \hat {\mathrm{E}} (f (Y _ {\theta}) | \mathcal {F} _ {t _ {0}}) = \frac {1}{n} \sum_ {i = 1} ^ {n} \frac {\partial}{\partial \theta} f (Y _ {\theta} (\omega_ {i})) = 0 \text {   assuming   that   } Y _ {\theta} (\omega_ {i}) \neq K \text {   for   all   } i.
$$

Thus, here, the partial derivative of the Monte-Carlo value is always wrong. 

## 17.2.4. Example: Trigger Products

The two simple examples above suggest that a finite difference approximation of a Monte-Carlo price works well, if the payout is smooth, but fails if the payout exhibits discontinuities. The problem becomes a bit more subtle if we consider products where the discontinuous behaviour is just one part of the payout which, in addition, may also be of more complex nature. Consider for example the auto cap. For given times $T_{1}, \ldots, T_{n}$ the auto cap pays at each payment date $T_{i+1}$ the payout of a caplet max $(L(T_{i}, T_{i+1}; T_{i}) - K_{i}, 0) \cdot (T_{i+1} - T_{i})$ , but does so only if the number of non-zero payments up to $T_{i}$ is less than some $n_{\text{maxEx}}$ . This latter condition represents a trigger which makes the otherwise continuous payoff discontinuous, see Figure 17.1. 

## 17.3. Generic Sensitivities: Bumping the Model

The finite difference approximation calculates the sensitivity by 

$$
\frac {\partial}{\partial \theta} \mathrm{E} (f (Y _ {\theta}) | \mathcal {F} _ {t _ {0}}) \approx \frac {\mathrm{E} (f (Y _ {\theta + h}) | \mathcal {F} _ {t _ {0}}) - \mathrm{E} (f (Y _ {\theta - h}) | \mathcal {F} _ {t _ {0}})}{2 h}.
$$

This brute-force finite difference calculation of sensitivities is sometimes referred to as bumping the model. Bumping the model has a charming advantage: If you keep your model and your pricing code separated (a design pattern one should always consider) then you may implement a generic code for generating sensitivities by feeding the pricing code with differently bumped models. In other words: 

## Once the pricing code is written, all sensitivities are available.

(17.1) 

It seems as if you get sensitivities almost for free (i.e. without any effort in modeling and implementation) and the only price you pay is a doubling of calculation time compared to pricing. However, it is known that applying such a finite difference approximation to a Monte-Carlo implementation will often result in extremely large Monte-Carlo errors. Especially if the payout function of the derivative is discontinuous, this Monte-Carlo error tends to infinity as h tends to zero. And discontinuous payout is present whenever a trigger feature is present. 

Sensitivities in Monte-Carlo are known as a challenge. Numerous methods have been proposed for calculating sensitivities in Monte-Carlo, among them the likelihood ratio $[55]$ and the application of Malliavin calculus, which has attracted increased attention recently, $[63]$ . These methods improve the robustness of sensitivities, but require more information. 

It appears as if the measures you have to take to improve Monte-Carlo sensitivities will lose the advantage $(17.1)$ of bumping the model. Later, we will present a method (which is also an implementation design pattern) that makes it possible to calculate sensitivities through bumping the model while providing the accuracy and robustness achieved by the likelihood ratio or Malliavin calculus approach. The method is essentially a likelihood ratio reconsidered on the level of the numerical scheme. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/d155e110dd9a43b3d86fac0352bbfa2695382bb3ad73c1c25d82e105870cefe4.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/193a458b5a1619021beb4bbbbb08d628d93c266e8eab09100164fb5729fb69bc.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/e3ee84e1cccfdb63027915b53a42003e23175558a9e293f57d03d5bec0ccf1ec.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/e410ea304b9b93436340d74d105336173e6e09cf0d026d49b68d64a545982aa2.jpg)



Figure 17.1.: The payoff of an auto cap paying a maximum of two out of three caplets, considered under a parallel shift of the interest rate curve (black line). The strike rate is depicted by a blue dot, a positive payout is marked in green: In scenarios a) and b) the first caplet does not lead to a positive payout while the second and third caplet do generate a positive payout. The shift of the interest rate curve from a) to b) changes the payout continuously. In scenario c) the first caplet leads to a positive payout. Since the auto cap is limited to two positive payouts the payout of the third caplet is lost as soon as the first caplet pays a positive amount. Thus, from scenario b) to c) the payout of the auto cap changes discontinuously.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/45572077818fb33afd080109ed8573e2c1968763831b0585cb743170485011ee.jpg)



Figure 17.2.: The value of an auto cap as a function of the shift size of a parallel shift of the interest rate curve. Using only a small number of paths, a small shift does not lead to a change of the exercise strategy. The price change is driven by the sensitivity of the underlying caplets. Thus, for small shifts one might be tempted to call the sensitivity stable. For a larger shift the exercise strategy changes on some paths, leading to a jump in payoff.


There are basically two different methods for calculating sensitivities in Monte-Carlo: 

- the pathwise method, which differentiates the payout on every simulation path, see 17.5 

- the likelihood ratio method, which differentiates the probability density, see 17.6. 

Numerically, these two methods may be realized as 

• (traditional) finite differences, see 17.4 

- finite differences applied to a proxy simulation scheme. 

However, a proxy simulation scheme is a much more powerful design, see Chapter 18. It is also possible to mix the two approaches by considering a partial proxy simulation scheme, see Section 18.4. 

In the following we will present the different methods for calculating sensitivities in Monte-Carlo simulations. Each section starts with a short description of the approximating formula and gives the method requirements and properties as bullet points. We assume that a Monte-Carlo pricing algorithm has been implemented and we mention only requirements additional to the pricing. 

## 17.4. Sensitivities by Finite Differences

The finite difference approximation is given by 

$$
\begin{array}{r c l} \frac {\partial}{\partial \theta} \mathrm{E} ^ {\mathbb {Q}} (f (Y _ {\theta}) \mid \mathcal {F} _ {t _ {0}}) & \approx & \frac {1}{2 h} (\mathrm{E} ^ {\mathbb {Q}} (f (Y _ {\theta + h}) \mid \mathcal {F} _ {t _ {0}}) - \mathrm{E} ^ {\mathbb {Q}} (f (Y _ {\theta - h}) \mid \mathcal {F} _ {t _ {0}})) \\ & \approx & \frac {1}{2 h} (\hat {\mathrm{E}} ^ {\mathbb {Q}} (f (Y _ {\theta + h}) \mid \mathcal {F} _ {t _ {0}}) - \hat {\mathrm{E}} ^ {\mathbb {Q}} (f (Y _ {\theta - h}) \mid \mathcal {F} _ {t _ {0}})) \\ & = & \frac {1}{n} \sum_ {i = 1} ^ {n} \frac {1}{2 h} \big (f (Y _ {\theta + h} (\omega_ {i}) - f (Y _ {\theta - h} (\omega_ {i})) \end{array}
$$

## Requirements

- No additional information from the model sde $X$ 

- No additional information from the simulation scheme $X^{*}(t_{i+1})$ 

- No additional information from the payout $f$ 

- No additional information on the nature of $\theta$ ( $\Rightarrow$ generic sensitivities) 

## Properties

- Biased derivative for large $h$ due to finite difference of order $h$ 

- Extremely large variance for discontinuous payouts and small $h$ (order $h^{-1}$ ) 

The most important feature of finite differences is their genericity. Once the pricing code has been written, all kinds of sensitivities may be calculated. 

For smooth payouts, the finite difference approximation converges to the derivative for $h \rightarrow 0$ . Thus, if the payout is smooth, small shift sizes h are favourable. Using large h the approximation of the derivative is biased. 

For discontinuous payouts, as $h \rightarrow 0$ the finite difference of the Monte-Carlo price does not converge to the derivative of the Monte-Carlo price. The reason is that for discontinuous payouts the Monte-Carlo approximation ( $n \rightarrow \infty$ ) and the approximation of the derivative ( $h \rightarrow 0$ ) are not interchangeable. 

For discontinuous payouts finite differences with a fixed, small shift size h perform poorly. The contribution of a discontinuity to the sensitivity may be calculated analytically. It is the jump size multiplied by the probability density at the discontinuity. Finite differences resolve this contribution only through those sample paths which fall into a neighbourhood around the discontinuity, having the width of the shift size. Thus, if the shift size is small, the discontinuity is resolved by a few points, ultimately resulting in a large Monte-Carlo error. For discontinuous payouts large shift sizes are preferable. However, if the shift size is large, the derivative becomes biased by second order effects (if present). 

Since finite difference does not require anything more than a given pricing algorithm, we are tempted to apply it to any product for which a Monte-Carlo pricing may be calculated. If the product exhibits discontinuities in the payout, the finite difference approximation tends to be unreliable, and a careful analysis of the Monte-Carlo error for a given shift size h has to be performed. 

## 17.4.1. Example: Finite Differences applied to Smooth and Discontinuous Payout

Let us consider a finite difference approximation of the partial derivative for the case of the linear payout $f(X(T)) = a \cdot X(T) + b$ from Section 17.2.3.1. We have 

$$
\begin{array}{r c l} \frac {\partial}{\partial \theta} \mathrm{E} ^ {\mathbb {Q}} (f (Y _ {\theta}) \mid \mathcal {F} _ {t _ {0}}) & \approx & \frac {1}{2 h} (\mathrm{E} ^ {\mathbb {Q}} (f (Y _ {\theta + h}) \mid \mathcal {F} _ {t _ {0}}) - \mathrm{E} ^ {\mathbb {Q}} (f (Y _ {\theta - h}) \mid \mathcal {F} _ {t _ {0}})) \\ & \approx & \frac {1}{2 h} (\hat {\mathrm{E}} ^ {\mathbb {Q}} (f (Y _ {\theta + h}) \mid \mathcal {F} _ {t _ {0}}) - \hat {\mathrm{E}} ^ {\mathbb {Q}} (f (Y _ {\theta - h}) \mid \mathcal {F} _ {t _ {0}})) \\ & = & \frac {1}{n} \sum_ {i = 1} ^ {n} \frac {1}{2 h} \big (f (Y _ {\theta + h} (\omega_ {i}) - f (Y _ {\theta - h} (\omega_ {i})) \\ & = & \frac {1}{n} \sum_ {i = 1} ^ {n} a \cdot \frac {1}{2 h} (Y _ {\theta + h} (\omega_ {i}) - Y _ {\theta - h} (\omega_ {i})), \end{array}
$$

which is a good approximation, if $\frac{\partial}{\partial\theta}Y_{\theta}(\omega_{i})) \approx \frac{1}{2h}(Y_{\theta+h}(\omega_{i}) - Y_{\theta-h}(\omega_{i}))$ . This is usually the case and throughout this chapter we assume that the model is such, that its realizations $Y_{\theta}(\omega_{i})$ are smooth in the model parameters $\theta$ . 

For the discontinuous payout $f(X(T)) = 1$ if $X(T) > K$ and $f(X(T)) = 0$ else, considered in Section 17.2.3.2, we have 

$$
\begin{array}{l} \frac {\partial}{\partial \theta} \mathrm{E} ^ {\mathbb {Q}} (f (Y _ {\theta}) \mid \mathcal {F} _ {t _ {0}}) \approx \frac {1}{2 h} (\mathrm{E} ^ {\mathbb {Q}} (f (Y _ {\theta + h}) \mid \mathcal {F} _ {t _ {0}}) - \mathrm{E} ^ {\mathbb {Q}} (f (Y _ {\theta - h}) \mid \mathcal {F} _ {t _ {0}})) \\ \approx \frac {1}{2 h} (\hat {\mathrm{E}} ^ {\mathbb {Q}} (f (Y _ {\theta + h}) \mid \mathcal {F} _ {t _ {0}}) - \hat {\mathrm{E}} ^ {\mathbb {Q}} (f (Y _ {\theta - h}) \mid \mathcal {F} _ {t _ {0}})) \\ = \frac {1}{n} \sum_ {i = 1} ^ {n} \frac {1}{2 h} (f (Y _ {\theta + h} (\omega_ {i})) - f (Y _ {\theta - h} (\omega_ {i}))) \\ = \frac {1}{n} \sum_ {i = 1} ^ {n} \frac {1}{2 h} \left\{ \begin{array}{l l} 1 & \text {if Y_{\theta -h} (\omega_{i}) <   K <   Y_{\theta +h} (\omega_{i})} \\ - 1 & \text {if Y_{\theta -h} (\omega_{i}) > K > Y_{\theta +h} (\omega_{i})} \\ 0 & \text {else.} \end{array} \right. \end{array}
$$

This is a valid approximation, but it has a large Monte-Carlo variance, since the true value is sampled by 0 and $\frac{1}{2h}$ occurring in the appropriate frequency. If h gets smaller, then we have to represent true value by a sampling of 0 and a very large constant. 

Simplified Example: Assume for simplicity that $Y_{\theta}$ is linear in $\theta$ , i.e. we have $Y_{\theta+h} = Y_{\theta} + \frac{\partial Y_{\theta}}{\partial \theta} \cdot h$ and thus 

$$
\begin{array}{l} \frac {f (Y _ {\theta + h} (\omega_ {i})) - f (Y _ {\theta - h} (\omega_ {i}))}{2 h} = \left\{ \begin{array}{l l} \frac {1}{2 h} & \text { if } Y _ {\theta - h} (\omega_ {i}) <   K <   Y _ {\theta + h} (\omega_ {i}) \\ \frac {- 1}{2 h} & \text { if } Y _ {\theta - h} (\omega_ {i}) > K > Y _ {\theta + h} (\omega_ {i}) \\ 0 & \text { else. } \end{array} \right. \\ = \left\{ \begin{array}{l l} \frac {\text { sign } \frac {\partial Y _ {\theta}}{\partial \theta}}{2 h} & \text { if } Y _ {\theta} (\omega_ {i}) \in [ K - \epsilon , K + \epsilon ] \\ 0 & \text { else. } \end{array} \right. \end{array}
$$

where $\epsilon := \left|\frac{\partial Y_{\theta}}{\partial\theta}\right| \cdot h$ . For the probability we have 

$$
q := \mathbb {Q} (Y _ {\theta} \in [ K - \epsilon , K + \epsilon ]) \approx \phi_ {Y _ {\theta}} (K) \cdot 2 \epsilon = \phi_ {Y _ {\theta}} (K) \cdot \left| \frac {\partial Y _ {\theta}}{\partial \theta} \right| \cdot 2 h.
$$

In other words: We are sampling the partial derivative of the expectation by a binomial experiment: 

$$
\frac {\text { sign } \frac {\partial Y _ {\theta}}{\partial \theta}}{2 h} \quad \text { with   probability   } q \quad \text { and } \quad 0 \quad \text { with   probability   } 1 - q.
$$

The expectation of this binomial experiment is 

$$
\frac {\mathrm{sign} \frac {\partial Y _ {\theta}}{\partial \theta}}{2 h} \cdot q + 0 \cdot (1 - q) \approx \phi_ {Y _ {\theta}} (K) \cdot \frac {\partial Y _ {\theta}}{\partial \theta},
$$

which is the desired analytic value for the finite difference approximation as $h \rightarrow 0$ . The variance of the binomial experiment is 

$$
\left(\frac {1}{2 h}\right) ^ {2} \cdot q \cdot (1 - q) \approx \phi_ {Y _ {\theta}} (K) \cdot \frac {\partial Y _ {\theta}}{\partial \theta} \cdot (1 - q) \cdot \frac {1}{2 h} = O \left(\frac {1}{2 h}\right),
$$

which explodes as $h \to 0$ . 

## 17.5. Sensitivities by Pathwise Differentiation

The pathwise differentiation method is given by 

$$
\begin{array}{l} \frac {\partial}{\partial \theta} \mathrm{E} ^ {\mathbb {Q}} (f (Y (\theta)) \mid \mathcal {F} _ {t _ {0}}) = \frac {\partial}{\partial \theta} \int_ {\Omega} f (Y (\omega , \theta))   \mathrm{d} \mathbb {Q} (\omega) = \int_ {\Omega} \frac {\partial}{\partial \theta} f (Y (\omega , \theta))   \mathrm{d} \mathbb {Q} (\omega) \\ = \int_ {\Omega} f ^ {\prime} (Y (\omega , \theta)) \cdot \frac {\partial Y (\omega , \theta)}{\partial \theta}   \mathrm{d} \mathbb {Q} (\omega) = \mathrm{E} ^ {\mathbb {Q}} (f ^ {\prime} (Y (\theta)) \cdot \frac {\partial Y (\theta)}{\partial \theta} \mid \mathcal {F} _ {t _ {0}}) \\ \stackrel {{f \text {   smooth }}} {{\approx}} \hat {\mathrm{E}} ^ {\mathbb {Q}} (f ^ {\prime} (Y (\theta)) \cdot \frac {\partial Y (\theta)}{\partial \theta} \mid \mathcal {F} _ {t _ {0}}) = \frac {1}{n} \sum_ {i = 1} ^ {n} f ^ {\prime} (Y (\omega_ {i}, \theta)) \cdot \frac {\partial Y (\omega_ {i} , \theta)}{\partial \theta} \end{array}
$$

## Requirements

• Additional information on the model sde X 

- No additional information on the simulation scheme $X(t_{i+1})$ 

- Additional information on the payout $f$ (derivative of $f$ must be known) 

- Additional information on the nature of $\theta$ ( $\Rightarrow$ no generic sensitivities) 

## Properties

- Unbiased derivative 

- Discontinuous payouts may be dealt with (interpret $f'$ as distribution, see below) 

The pathwise method requires the knowledge of the derivative of the payout $f'$ and the derivative of the process realizations with respect to the parameter $\theta$ , i.e. $\frac{\partial\tilde{Y}(\omega_{i},\theta)}{\partial\theta}$ . It is thus only applicable for a restricted class of models and model parameters, where $\frac{\partial Y(\omega_{i},\theta)}{\partial\theta}$ may be calculated analytically. 

It seems as if a discontinuity in the payout cannot be dealt with, since we require $f'$ to exist. However, the impact of a discontinuity can be calculated analytically, see 17.5.2. 

It is a major disadvantage of the method that it requires special knowledge of the payout function and of model realizations. 

## 17.5.1. Example: Delta of a European Option under a Black-Scholes Model

We consider a Black-Scholes Model 

$$
\begin{array}{l} S (t) = S (0) \cdot \exp (\bar {r} t - \frac {1}{2} \bar {\sigma} ^ {2} t + \bar {\sigma} W (t)), \qquad S (0) = S _ {0} \\ B (t) = B (0) \cdot \exp (\bar {r} t) \end{array}\tag{17.2}
$$

In this case we have, e.g. 

$$
\frac {\partial}{\partial S _ {0}} S (T) = \frac {S (T)}{S _ {0}}.
$$

Using the notation above, our model primitive is $X = (S, B)$ . We assume that the payout of our derivative depends on $Y = X(T) = (S(T), B(T))$ only, i.e. we are considering a European option. Then we have 

$$
\begin{array}{r c l} \frac {\partial}{\partial S _ {0}} \mathrm{E} ^ {\mathbb {Q}} (f (S (T)) \mid \mathcal {F} _ {t _ {0}}) & = & \mathrm{E} ^ {\mathbb {Q}} (f ^ {\prime} (S (T)) \cdot \frac {S (T)}{S _ {0}} \mid \mathcal {F} _ {t _ {0}}) \\ & \approx & \hat {\mathrm{E}} ^ {\mathbb {Q}} (f ^ {\prime} (S (T)) \cdot \frac {S (T)}{S _ {0}} \mid \mathcal {F} _ {t _ {0}}) \\ & = & \frac {1}{n} \sum_ {i = 1} ^ {n} f ^ {\prime} (S (T, \omega_ {i})) \cdot \frac {S (T , \omega_ {i})}{S _ {0}} \end{array}
$$

## 17.5.2. Pathwise Differentiation for Discontinuous Payouts

In case that the payout f exhibits discontinuities the pathwise method may be applied, provided that f allows for a decomposition 

$$
f = g + \sum_ {i} \alpha_ {i} \mathbf {1} (\{Y (\theta) > y _ {i} \}),
$$

with $g$ being smooth. In this case we have 

$$
\begin{array}{l} \frac {\partial}{\partial \theta} \mathrm{E} ^ {\mathbb {Q}} (f (Y (\theta)) \mid \mathcal {F} _ {T _ {0}}) = \frac {\partial}{\partial \theta} \int_ {\Omega} f (Y (\omega , \theta))   \mathrm{d} \mathbb {Q} (\omega) = \int_ {\Omega} \frac {\partial}{\partial \theta} f (Y (\omega , \theta))   \mathrm{d} \mathbb {Q} (\omega) \\ = \int_ {\Omega} f ^ {\prime} (Y (\omega , \theta)) \cdot \frac {\partial Y (\omega , \theta)}{\partial \theta}   \mathrm{d} \mathbb {Q} (\omega) = \mathrm{E} ^ {\mathbb {Q}} (f ^ {\prime} (Y (\theta)) \cdot \frac {\partial Y (\theta)}{\partial \theta} \mid \mathcal {F} _ {T _ {0}}) \\ \stackrel {{g \text {   smooth }}} {{\approx}} \hat {\mathrm{E}} ^ {\mathbb {Q}} (g ^ {\prime} (Y (\theta)) \cdot \frac {\partial Y (\theta)}{\partial \theta} \mid \mathcal {F} _ {T _ {0}}) + \sum_ {i} \alpha_ {i} \cdot \phi (y _ {i}) \cdot \frac {\partial Y (\theta)}{\partial \theta} | _ {Y (\theta) = y _ {i}} \end{array}
$$

See [79, 88] for examples of how to use pathwise differentiation with discontinuous payouts (there in the context of $\mathfrak{n}^{\text{th}}$ to default swaps, CDOs). 

## 17.6. Sensitivities by Likelihood Ratio Weighting

The pathwise method differentiates the path value $Y(\theta)$ of the underlying process realizations Y. Provided there is a probability density $\phi_{Y(\theta)}$ of $Y(\theta)$ we may write the expectation as a convolution with the density. The likelihood ratio weighting [53, 55, 16] is then given by 

$$
\begin{array}{l} \frac {\partial}{\partial \theta} \mathrm{E} ^ {\mathbb {Q}} (f (Y (\theta)) \mid \mathcal {F} _ {t _ {0}}) = \frac {\partial}{\partial \theta} \int_ {\Omega} f (Y (\omega , \theta))   \mathrm{d} \mathbb {Q} (\omega) = \frac {\partial}{\partial \theta} \int_ {\mathbb {R} ^ {m}} f (y) \cdot \phi_ {Y (\theta)} (y)   \mathrm{d} y \\ = \int_ {\mathbb {R} ^ {m}} f (y) \cdot \frac {\frac {\partial}{\partial \theta} \phi_ {Y (\theta)} (y)}{\phi_ {Y (\theta)} (y)} \cdot \phi_ {Y (\theta)} (y)   \mathrm{d} y = \mathrm{E} ^ {\mathbb {Q}} (f (Y) \cdot w (\theta) \mid \mathcal {F} _ {t _ {0}}) \\ \approx \hat {\mathrm{E}} ^ {\mathbb {Q}} (f (Y) \cdot w (\theta) \mid \mathcal {F} _ {t _ {0}}) = \frac {1}{n} \sum_ {i = 1} ^ {n} f (Y (\omega_ {i})) \cdot w (\theta , \omega_ {i}), \end{array}
$$

where $w(\theta) := \frac{\frac{\partial}{\partial\theta} \phi_{Y(\theta)}(Y(\theta))}{\phi_{Y(\theta)}(Y(\theta))}$ . 

## Requirements

• Additional information on the model sde $X (\rightarrow \phi_{Y(\theta)})$ 

- No additional information on the simulation scheme $X(t_{i+1})$ 

- No additional information on the payout $f$ 

- Additional information on the nature of $\theta$ ( $\Rightarrow$ no generic sensitivities) 

## Properties

- Unbiased derivative 

- Discontinuous payouts may be dealt with. 

The Likelihood Ratio method requires no additional information on the payout function. This is an advantage compared to the pathwise differentiation. However, it requires that the density of the model sde's realizations $X(t)$ is known and furthermore, that its derivative is known analytically with respect to the parameter $\theta$ . This is rarely the case and thus a major drawback of the method. 

The likelihood ratio method does not require the payout to be smooth. The method works very well for calculating the impact of a discontinuity in the payout. However, the method has its problems with smooth payouts: the Monte-Carlo error of the approximation using Likelihood Ratio is larger than the Monte-Carlo error of the finite-difference approximation. We give a simple example of this effect next. 

## 17.6.1. Example: Delta of a European Option under a Black-Scholes Model using Pathwise Derivative

Let us look again at a European Option using the Black-Schloes model (17.2). Since B is deterministic we need to consider the probability density of S. Since $\log(S(T))$ is normally distributed, see Chapter 4, we have for the density of $S(T)$ 

$$
\phi_ {S (T)} (s) = \frac {\phi_ {\mathrm{std.norm.}} \big (\frac {1}{\bar {\sigma} \sqrt {T}} (\log (s) + \bar {r} (T) - \frac {1}{2} \bar {\sigma} (T) ^ {2} - \log (S _ {0})) \big)}{s},
$$

where $\phi_{\mathrm{std.norm.}}(x) = \frac{1}{\sqrt{2\pi}}\exp (-x^2 /2)$ is the density of the standard normal distribution. 

Thus, the delta of a European option with (numéraire-rebased) payout $f(S(T), B(T))$ , calculated by the likelihood ratio method, is given by 

$$
\mathrm{E} ^ {\mathbb {Q}} \left(f (S (T), B (T)) \cdot \frac {\frac {\partial}{\partial S _ {0}} \phi_ {S (T)} (S (T))}{\phi_ {S (T)} (S (T))} \mid \mathcal {F} _ {0}\right).
$$

## 17.6.2. Example: Variance Increase of the Sensitivity when using Likelihood Ratio Method for Smooth Payouts

For some smooth payouts, the Likelihood Ratio method may perform less accurately than the pathwise method 17.5 or its finite difference approximation 17.4. A simple example illustrates this effect: Consider constant payout $f(S(T), B(T)) = b$ . Then, the likelihood ratio method gives the delta of this option as 

$$
\begin{array}{l} \mathrm{E} ^ {\mathbb {Q}} \left(f (S (T), B (T)) \cdot \frac {\frac {\partial}{\partial S _ {0}} \phi_ {S (T)} (S (T))}{\phi_ {S (T)} (S (T))} \mid \mathcal {F} _ {0}\right) = \int_ {\mathbb {R}} f (s, B (T)) \cdot \frac {\partial}{\partial S _ {0}} \phi_ {S (T)} (s)   \mathrm{d} s \\ \stackrel {{f = b = \text {const.}}} {{=}} b \cdot \int_ {\mathbb {R}} \frac {\partial}{\partial S _ {0}} \phi_ {S (T)} (s)   \mathrm{d} s \end{array}
$$

and indeed (using substitution $y = \log(s)$ , $\mathrm{dy} = \frac{1}{s}\mathrm{d}s$ ) we see that the delta is zero: 

$$
= \int_ {\mathbb {R}} \frac {\partial}{\partial S _ {0}} \phi () \mathrm{d} y = 0
$$

The Monte-Carlo approximation is 

$$
\begin{array}{l} \mathrm{E} ^ {\mathbb {Q}} \left(f (S (T), B (T)) \cdot \frac {\frac {\partial}{\partial S _ {0}} \phi_ {S (T)} (S (T))}{\phi_ {S (T)} (S (T))} \mid \mathcal {F} _ {0}\right) \\ \approx \frac {1}{n} \sum_ {i = 1} ^ {n} f (S (T, \omega_ {i}), B (T)) \cdot \frac {\frac {\partial}{\partial S _ {0}} \phi (S (T , \omega_ {i}))}{\phi (S (T , \omega_ {i}))} = \frac {1}{n} \sum_ {i = 1} ^ {n} b \cdot \frac {\frac {\partial}{\partial S _ {0}} \phi (S (T , \omega_ {i}))}{\phi (S (T , \omega_ {i}))}, \end{array}
$$

which is in general non zero. It is an approximation of zero, having some variance. 

On the other hand, note that the pathwise method and even a finite difference approximation thereof would give a delta of zero with zero Monte-Carlo variance. 

## 17.7. Sensitivities by Malliavin Weighting

The Malliavin weighting is similar to the Likelihood Ratio method: the sensitivity is expressed as the expectation of a weighted payout function. 

$$
\begin{array}{r l} \frac {\partial}{\partial \theta} \mathrm{E} ^ {\mathbb {Q}} (f (Y (\theta)) | \mathcal {F} _ {t _ {0}}) = & \mathrm{E} ^ {\mathbb {Q}} (f (Y (\theta)) \cdot w (\theta) | \mathcal {F} _ {t _ {0}}) \\ & \approx \hat {\mathrm{E}} ^ {\mathbb {Q}} (f (Y (\theta)) \cdot w (\theta) | \mathcal {F} _ {t _ {0}}) = \frac {1}{n} \sum_ {i = 1} ^ {n} f (Y (\theta , \omega_ {i})) \cdot w (\theta , \omega_ {i}) \end{array}
$$

## Requirements

• Additional information on the model sde $X$ ( $\rightarrow w$ ) 

- No additional information on the simulation scheme $X(t_{i+1})$ 

- No additional information on the payout $f$ 

- Additional information on the nature of $\theta$ ( $\Rightarrow$ no generic sensitivities) 

## Properties

- Unbiased derivative 

- Discontinuous payouts may be dealt with. 

Benhamou [47] showed that the Likelihood Ratio corresponds to the Malliavin weights with minimal variance and may be expressed as a conditional expectation of all corresponding Malliavin weights (we thus view the Likelihood Ratio as an example of the Malliavin weighting method). 

However, here the weights are derived directly through Malliavin calculus which makes this method more general and applicable even if the density is not known. The derivation of the Malliavin weights requires in-depth knowledge of the underlying continuous process X and it is heavily dependent on the nature of $\theta$ . 

## 17.8. Proxy Simulation Scheme

The proxy simulation scheme defines a design of a Monte-Carlo pricing engine that has the remarkable properties that the application of finite differences to the pricing will result in Likelihood Ratio weighted sensitivities without actually the need to know the density $\phi$ analytically. Thus it combines the robustness of Likelihood Ratio or Malliavin weighting with the genericity of finite differences. 

Since the proxy simulation scheme method is not solely devoted to the calculation of sensitivities it will be discussed in an own chapter in 18. For a detailed discussion of the proxy simulation scheme see also $[65, 66]$ . Here, we will summarize the key properties. 

The Monte-Carlo sensitivity under a proxy simulation scheme is given by 

$$
\begin{array}{r l} \frac {\partial}{\partial \theta} \mathrm{E} ^ {\mathbb {Q}} (f (Y ^ {*} (\theta)) \mid \mathcal {F} _ {t _ {0}}) & \approx \frac {1}{2 h} \big (\mathrm{E} ^ {\mathbb {Q}} (f (Y ^ {*} (\theta + h)) \mid \mathcal {F} _ {t _ {0}}) - \mathrm{E} ^ {\mathbb {Q}} (f (Y ^ {*} (\theta - h)) \mid \mathcal {F} _ {t _ {0}}) \big) \\ & = \frac {\partial}{\partial \theta} \int_ {\mathbb {R} ^ {m}} f (y) \cdot \frac {1}{2 h} (\phi_ {Y ^ {*} (\theta + h)} (y) - \phi_ {Y ^ {*} (\theta - h)} (y))   \mathrm{d} y \\ & = \int_ {\mathbb {R} ^ {m}} f (y) \cdot \frac {\frac {1}{2 h} (\phi_ {Y ^ {*} (\theta + h)} (y) - \phi_ {Y ^ {*} (\theta - h)} (y))}{\phi_ {Y ^ {\circ}} (y)} \cdot \phi_ {Y ^ {\circ}} (y)   \mathrm{d} y \\ & \approx \frac {1}{n} \sum_ {i = 1} ^ {n} f (Y ^ {\circ} (\omega_ {i})) \cdot \frac {1}{2 h} (w (\theta + h, \omega_ {i}) - w (\theta - h, \omega_ {i})) \end{array}
$$

## Requirements

- No additional information on the model sde $X$ 

• Additional information on the simulation scheme $X^{*}(t_{i+1}), X^{\circ}(t_{i+1})$ 

- No additional information on the payout $f$ 

- No additional information on the nature of $\theta$ ( $\Rightarrow$ generic sensitivities) 

## Properties

- Biased derivative (but small shift $h$ possible!) 

- Discontinuous payouts may be dealt with. 

# Proxy Simulation Schemes for Monte-Carlo Sensitivities and Importance Sampling

In this chapter we describe the proxy simulation scheme technique as it is given in [66] and [65]. 

## 18.1. Full Proxy Simulation Scheme

We take the notation of the previous chapter, see 17.2 and 17.3 and consider two time-discrete schemes for the stochastic process $X$ : 

$$
\begin{array}{l l} X ^ {*} & t _ {i} \mapsto X ^ {*} (t _ {i}) \quad i = 0, 1, 2, \ldots \quad \text { time   discretization   scheme   of } X \\ & \to \text { target   scheme } \end{array}
$$

$X^{\circ}\quad t_{i}\mapsto X^{\circ}(t_{i})\quad i = 0,1,2,\ldots$ any other time-discrete stochastic process (assumed to be close to $X^{*}$ ) $\rightarrow$ proxy scheme 

Let $\phi_{Y^{\circ}}(y)$ denote the density of $Y^{\circ}$ and $\phi_{Y^{*}}(y)$ the density of $Y^{*}$ . We require 

$$
\forall y: \phi^ {Y ^ {\circ}} (y) = 0 \Rightarrow \phi^ {Y ^ {*}} (y) = 0.\tag{18.1}
$$

Using the additional scheme $X^{\circ}$ the pricing of a payout function $f$ is now performed in the following way: Let $Y = (X(t_1),\ldots ,X(t_m))$ , $Y^{*} = (X^{*}(t_{1}),\ldots ,X^{*}(t_{m}))$ , $Y^{\circ} = (X^{\circ}(t_{1}),\ldots ,X^{\circ}(t_{m}))$ . We have $\mathrm{E}^{\mathbb{Q}}(f(Y(\theta))|\mathcal{F}_{t_0})\approx \mathrm{E}^{\mathbb{Q}}(f(Y^{*}(\theta))|\mathcal{F}_{t_0})$ and furthermore 

$$
\begin{array}{r l} \mathrm{E} ^ {\mathbb {Q}} (f (Y ^ {*} (\theta)) \mid \mathcal {F} _ {t _ {0}}) & = \int_ {\Omega} f (Y ^ {*} (\omega , \theta))   \mathrm{d} \mathbb {Q} (\omega) = \int_ {\mathbb {R} ^ {m}} f (y) \cdot \phi_ {Y ^ {*} (\theta)} (y)   \mathrm{d} y \\ & = \int_ {\mathbb {R} ^ {m}} f (y) \cdot \frac {\phi_ {Y ^ {*} (\theta)} (y)}{\phi_ {Y ^ {\circ}} (y)} \cdot \phi_ {Y ^ {\circ}} (y)   \mathrm{d} y = \mathrm{E} ^ {\mathbb {Q}} (f (Y ^ {\circ}) \cdot w (\theta) \mid \mathcal {F} _ {t _ {0}}, \end{array}
$$

where $w(\theta) = \frac{\phi_{Y^*(\theta)}(y)}{\phi_{Y^\circ}(y)}$ . 

For the Monte-Carlo approximation this implies that the sample paths are generated from the scheme $X^{\circ}$ while the probability densities are corrected towards the target scheme $X^{*}$ . 

## Notes

- For $X^{\circ} = X^{*}$ we have $w(\theta) = 1$ , and in this case the proxy simulation scheme corresponds to the ordinary Monte-Carlo simulation of $X^{*}$ . 

- The proxy scheme $X^{\circ}$ and thus its realization vector $Y^{\circ}$ are seen as being independent of $\theta$ . This has important implications on the calculation of sensitivities, see Section 18.2. 

- The requirement $\forall y: \phi^{Y^{\circ}}(y) = 0 \Rightarrow \phi^{Y^{\circ}}(y) = 0$ corresponds to the non-degeneracy condition of the diffusion matrix as it appears in the application of the likelihood ratio and Malliavin weights. However, here this requirement is far less restrictive since we are free to choose the proxy scheme $X^{\circ}$ . 

## 18.1.1. Calculation of Monte-Carlo weights

For the most common numerical schemes the densities $\phi^{Y^{\circ}}$ , $\phi^{Y^{*}}$ and thus the Monte-Carlo weights may be calculated numerically. Consider for example the schemes 

target scheme: $X^{*}(t_{i + 1}) = X^{*}(t_{i}) + \mu^{X^{*}}(t_{i})\Delta t_{i} + \Sigma (t_{i})\cdot \Gamma (t_{i})\cdot \Delta U(t_{i})$ 

proxy scheme: $X^{\circ}(t_{i+1}) = X^{\circ}(t_{i}) + \mu^{X^{\circ}}(t_{i})\Delta t_{i} + \Sigma^{\circ}(t_{i})\cdot\Gamma^{\circ}(t_{i})\cdot\Delta U(t_{i})$ 

where $\Sigma$ denotes an invertible volatility matrix and $\Gamma$ denotes a projection matrix, the factor matrix which defines the correlation structure $R = \Gamma\Gamma^{T}$ . 

Assume for simplicity that $\mu^{X^{*}}(t_{i})$ depends on $X^{*}(t_{i})$ , $X^{*}(t_{i+1})$ only (and similar for $\mu^{X^{\circ}}(t_{i})$ ) (this holds for, e.g. Euler Scheme, Predictor Corrector), then we have for the transition probability densities 

$$
\begin{array}{r l} \phi^ {X ^ {*}} (t _ {i}, X _ {i} ^ {*}; t _ {i + 1}, X _ {i + 1} ^ {*}) = & \\ & \frac {1}{(2 \Pi \Delta t _ {i}) ^ {n / 2}} \exp \Big (- \frac {1}{2 \Delta t _ {i}}   (\Lambda^ {- 1 / 2} F ^ {\mathrm{T}} \Sigma^ {- 1} (X _ {i + 1} ^ {*} - X _ {i} ^ {*} - \mu^ {X ^ {*}} (t _ {i}) \Delta t _ {i})) ^ {2} \Big) \end{array}
$$

$$
\begin{array}{l} \phi^ {X ^ {\circ}} (t _ {i}, X _ {i} ^ {\circ}; t _ {i + 1}, X _ {i + 1} ^ {\circ}) = \\ \frac {1}{(2 \Pi \Delta t _ {i}) ^ {n / 2}} \exp \Big (- \frac {1}{2 \Delta t _ {i}} \big (\Lambda^ {\circ - 1 / 2} F ^ {\circ \mathrm{T}} \Sigma^ {\circ - 1} (X _ {i + 1} ^ {\circ} - X _ {i} ^ {\circ} - \mu^ {X ^ {\circ}} (t _ {i}) \Delta t _ {i}) \big) ^ {2} \Big). \end{array}
$$

And the proxy scheme weights are given by 

$$
w (t _ {i + 1}) \mid_ {\mathcal {F} _ {t _ {k}}} = \prod_ {j = k} ^ {i} \frac {\phi^ {X ^ {*}} (t _ {j} , X _ {j} ^ {\circ} ; t _ {j + 1} , X _ {j + 1} ^ {\circ})}{\phi^ {X ^ {\circ}} (t _ {j} , X _ {j} ^ {\circ} ; t _ {j + 1} , X _ {j + 1} ^ {\circ})},
$$

see [66] for details. 

## Notes

- We used the factor decomposition (PCA) $\Gamma = F \cdot \sqrt{\Lambda}$ where $\Lambda = \mathrm{diag}(\lambda_1, \ldots, \lambda_m)$ are the non-zero eigenvalues of $\Gamma \cdot \Gamma^\top$ . 

- A change of market data / calibration affects only the transition probabilities. 

# 18.2. Sensitivities by Finite Differences on a Proxy Simulation Scheme

$$
\begin{array}{l} \frac {\partial}{\partial \theta} \mathrm{E} ^ {\mathbb {Q}} (f (Y ^ {*} (\theta)) \mid \mathcal {F} _ {t _ {0}}) \approx \frac {1}{2 h} \big (\mathrm{E} ^ {\mathbb {Q}} (f (Y ^ {*} (\theta + h)) \mid \mathcal {F} _ {t _ {0}}) - \mathrm{E} ^ {\mathbb {Q}} (f (Y ^ {*} (\theta - h)) \mid \mathcal {F} _ {t _ {0}}) \big) \\ = \frac {\partial}{\partial \theta} \int_ {\mathbb {R} ^ {m}} f (y) \cdot \frac {1}{2 h} (\phi_ {Y ^ {*} (\theta + h)} (y) - \phi_ {Y ^ {*} (\theta - h)} (y))   \mathrm{d} y \\ = \int_ {\mathbb {R} ^ {m}} f (y) \cdot \frac {\frac {1}{2 h} (\phi_ {Y ^ {*} (\theta + h)} (y) - \phi_ {Y ^ {*} (\theta - h)} (y))}{\phi_ {Y ^ {\circ}} (y)} \cdot \phi_ {Y ^ {\circ}} (y)   \mathrm{d} y \\ \approx \frac {1}{n} \sum_ {i = 1} ^ {n} f (Y ^ {\circ} (\omega_ {i})) \cdot \frac {1}{2 h} (w (\theta + h, \omega_ {i}) - w (\theta - h, \omega_ {i})) \end{array}
$$

## Requirements

- No additional information on the model sde $X$ 

• Additional information on the simulation scheme $X^{*}(t_{i+1})$ , $X^{\circ}(t_{i+1})$ 

- No additional information on the payout $f$ 

- No additional information on the nature of $\theta$ ( $\Rightarrow$ generic sensitivities) 

## Properties

- Biased derivative (but small shift $h$ possible!) 

- Discontinuous payouts may be dealt with. 

## Notes

We noted above that additional information on the simulation scheme is required, that is, the densities of the two schemes. Note however that we require these densities to setup the pricing algorithm. For the sensitivity calculation no additional information is needed. Note also that the required densities are densities of numerical schemes, which can usually be calculated from known transition probability densities (see Section 18.1.1). 

## 18.2.1. Localization

If the payout function f is smooth then ordinary finite differences perform better than the weighting techniques. The latter shows an increase in Monte-Carlo variance of the sensitivity. This effect is not only visible for smooth payouts f, but also for large finite difference shifts. 

A solution that has been proposed in [63] is localization. Here the weighting is applied only to a region where the payoff is discontinuous. 

Let $g$ denote the localization function, i.e. a smooth function $0 \leq g \leq 1$ such that $g = 1$ at discontinuities of $f$ . Consider the decomposition 

$$
f = (1 - g) \cdot f + g \cdot f.
$$

We define the pricing of the payout $f$ as 

$$
\operatorname{E} (f (Y ^ {*}) | \mathcal {F} _ {t _ {0}}) = \operatorname{E} ((1 - g (Y ^ {*})) \cdot f (Y ^ {*}) | \mathcal {F} _ {t _ {0}}) + \operatorname{E} (g (Y ^ {\circ}) \cdot f (Y ^ {\circ}) \cdot \frac {\phi_ {Y ^ {*}}}{\phi_ {Y ^ {\circ}}} | \mathcal {F} _ {t _ {0}}).
$$

In other words: We use a pricing based on a proxy simulation scheme for $g \cdot f$ and a pricing based on direct simulation for $(1 - g) \cdot f$ . 

It should be noted that localization is carried out by a redefinition of the payout. The product is split into two parts, where one is priced by a direct simulation scheme and the other is priced by a proxy simulation scheme method. This allows us to implement localization on the product level, completely independent of the actual simulation properties. In addition, localization does not reduce the ability to calculate generic sensitivities. 

## 18.2.2. Object-Oriented Design

The proxy scheme simulation method may in part also be viewed as an implementation design. In Figure 18.1(a) we depict the object-oriented design of a standard Monte-Carlo simulation where a change in market data results in a change of simulation path. In Figure 18.1(b) we contrast the proxy scheme simulation method where a change in market data results in a change of Monte-Carlo weights. In practice, we propose that the model driving the generation of the proxy schemes paths is calibrated to market data used for pricing while a market data scenario used for sensitivity calculation, i.e. by bumping the model, only impacts the Monte-Carlo weights. A method should be offered to reset the proxy simulation's market data to the target simulation's market data. 

## 18.3. Importance Sampling

The key idea of importance sampling is to generate the paths according to their importance to the application, not according to their probability law, and in doing so, adjust towards their probability by a suitable Monte-Carlo weight (the change of measure). 

Using a proxy simulation scheme, the paths are generated according to the proxy scheme while a Monte-Carlo weight adjusts their probability towards the target scheme. Actually, once the proxy simulation scheme framework has been established, the Monte-Carlo weights are calculated automatically from the two numerical schemes. 

Thus, choosing the proxy scheme such that it creates paths according to their importance to the application is a form of importance sampling. It has the advantage that specifying a suitable process might come easier than calculating the optimal sampling and the corresponding Monte-Carlo weights. 

## 18.3.1. Example

Let us look at the pricing of an out-of-the-money option under a lognormal model (like the Black-Scholes model or the LIBOR market model): 

$$
\begin{array}{l l} \text { Log   Euler   Scheme: } & \mathrm{d} \log (X) (t _ {j + 1}) = \log (X) (t _ {j + 1}) + \mu (t) \mathrm{d} t + \sigma \mathrm{d} W \\ \text { OTM   option: } & \max (X (T) - K, 0), \end{array}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/a3e63e59cac4c983c502df7004b4fcca5ddd4b53ac066dc15c93fadb905aec05.jpg)



(a) Standard Monte-Carlo Simulation


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/bc617e2388de007f3ea3ed35b9b90abc17e1b0a933e9c22975bd6cefe140661b.jpg)



(b) Proxy Scheme Monte-Carlo Simulation



Figure 18.1.: Object-oriented design of the Monte-Carlo pricing engine: We depict the impact of a change of different market data scenarios $\theta + h$ and $\theta - h$ on the pricing code of a standard Monte-Carlo simulation and a proxy scheme simulation.


where $X(0) = X_{0}$ and $K >> X_{0}$ . The drift of the model is determined by the specific pricing measure. However, in our application we would prefer that the mean of $X(T)$ is close to the option strike K rather than being $\exp\left(\log X_{0} + \int_{0}^{T} \mu(t) \, dt\right)$ . To achieve this, simply use a proxy scheme with artificial drift: 

$$
\begin{array}{l l} \text {Proxy Scheme:} & \mathrm{d} \log (X) (t _ {j + 1}) = \log (X) (t _ {j + 1}) + \frac {\log (K) - \log (X _ {0})}{T} \mathrm{d} t + \sigma_ {i} \mathrm{d} W \\ \text {Target Scheme:} & \mathrm{d} \log (X) (t _ {j + 1}) = \log (X) (t _ {j + 1}) + \mu (t) \mathrm{d} t + \sigma \mathrm{d} W \end{array}
$$

This will bring the paths to the region that is important for the pricing of the option, while the proxy simulation scheme framework automatically adjusts probabilities accordingly. Figure 18.2 shows a comparison of distribution of Monte-Carlo prices obtained from direct simulation compared to the prices obtained from importance adjusted proxy scheme simulation. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/49d0f95dbc297d1cf621cb05e8a4fcae2969ec35b96b435f87663f37c01ee1e7.jpg)



Figure 18.2.: Importance sampling using a drift adjusted proxy scheme. The example was created using a LIBOR market model to price a caplet with strike K = 0.3, the initial forward rate being $X_{0} = L_{i}(0) = 0.1$ .


## 18.4. Partial Proxy Simulation Schemes

The (full) proxy simulation scheme method requires the density of the target scheme realization to be zero if the density of the proxy scheme is zero, $(18.1)$ . In other words, it is required that the paths simulated under the proxy scheme comprise all paths possible under the target scheme. If the property is violated, then the Monte-Carlo expectation using the weighted paths of the proxy scheme will leave out some mass. This limits the application of the full proxy simulation scheme. For the calculation of sensitivities the limitation means that we cannot calculate the sensitivity with respect to all possible perturbations. 

However, in order to improve the calculation of sensitivities of trigger products it is not necessary to keep all underlying quantities rigid (as for a full proxy simulation); it is sufficient to keep the quantity that induces the discontinuity rigid. This gives rise to the notion of a partial proxy simulation scheme, [65]. 

Let $K^0$ denote the unperturbed scheme and $K^*$ some perturbation of $K^0$ , e.g. a scheme with different initial data. We will call $K^0$ the reference scheme and $K^*$ the target scheme. 

The usual procedure of bump-and-revalue for computing Greeks would simulate paths of $K^{*}$ having Monte-Carlo weight $\frac{1}{n}$ . The proxy simulation schemes would simulate paths of $K^{0}$ using Monte-Carlo weights $\frac{1}{n} \cdot \frac{\phi^{*}}{\phi^{0}}$ . Instead, here we consider a third scheme $K^{1}$ , the (partial) proxy simulation scheme where paths are such that the path-wise values of some (but not all) components of $K^{1}$ (or a function thereof) agree with the corresponding pathwise quantities under $K^{0}$ . 

## 18.4.1. Linear Proxy Constraint

Let $\Pi(t_i)$ denote a projection operator of rank $k$ . Let $v(t_i)$ be defined as 

$$
v (t _ {i}) := (\Pi \cdot \Gamma (t _ {i})) ^ {- 1} \cdot (\Pi \cdot K ^ {*} (t _ {i + 1}) - \Pi \cdot K ^ {0} (t _ {i + 1})),\tag{18.2}
$$

where $(\Pi \cdot \Gamma(t_{i}))^{-1}$ is the quasi inverse of $\Pi \cdot \Gamma(t_{i})$ , i.e. v is the solution of 

$$
\| \Pi \cdot K ^ {0} (t _ {i + 1}) - \Pi \cdot (K ^ {*} (t _ {i + 1}) - \Pi \Gamma (t _ {i}) v (t _ {i})) \| _ {L _ {2}} \to \min.\tag{18.3}
$$

We define the k-dimensional partial proxy scheme $K^{1}$ as: 

$$
\begin{array}{r l} {K ^ {1} (t _ {0})} & {:= K ^ {*} (t _ {0})} \\ {K ^ {1} (t _ {i + 1})} & {:= K ^ {*} (t _ {i + 1}) - \Gamma (t _ {i}) \cdot v (t _ {i}).} \end{array}\tag{18.4}
$$

The scheme $K^{1}$ has the following properties: 

- It coincides with $K^0$ on the $k$ -dimensional sub-manifold defined by $\Pi$ , i.e. $\Pi \cdot K^1(t_i) = \Pi \cdot K^0(t_i)$ . 

- It is given through a mean shift $v(t_i)$ on the Brownian increment $\Delta W(t_i)$ of the target scheme $K^*$ . 

Consequently, the Monte-Carlo weight of the partial proxy scheme is given by 

$$
w (t _ {i}) = \frac {\phi^ {K ^ {*}} (t _ {i} , K ^ {1} (t _ {i}) ; t _ {i + 1} , K ^ {1} (t _ {i + 1}))}{\phi^ {K ^ {1}} (t _ {i} , K ^ {1} (t _ {i}) ; t _ {i + 1} , K ^ {1} (t _ {i + 1}))}.
$$

In the case of a linear proxy constraint, the mean shift $v(t_{i})$ is $F_{t_{i}}$ measurable. $^{1}$ Then, using simple Euler schemes, the transition probabilities are 

$$
\begin{array}{r l} \phi^ {K ^ {1}} (t _ {i}, K ^ {1} (t _ {i}); t _ {i + 1}, K ^ {1} (t _ {i + 1})) & = \phi^ {W} (t _ {i}, W (t _ {i}), t _ {i + 1}, W (t _ {i + 1})) \\ \phi^ {K ^ {*}} (t _ {i}, K ^ {1} (t _ {i}); t _ {i + 1}, K ^ {1} (t _ {i + 1})) & = \phi^ {W} (t _ {i}, W (t _ {i}), t _ {i + 1}, W (t _ {i + 1}) - v (t _ {i})). \end{array}\tag{18.5}
$$

From this we can derive $w(t_{i})$ as a simple analytic formula, see Section 18.4.4.2. 

We would like to note that in $(18.3)$ we may replace the projection operator by a general nonlinear function, if necessary. We will discuss this case in Section 18.4.3 and we will consider this case in our example in Section 18.4.7. 

## 18.4.2. Comparison to Full Proxy Scheme Method

The proxy simulation scheme proposed in [66] corresponds to $K^1 = K^0$ . Thus, it is a special case of (18.2), (18.4) if $\Pi$ is the identity and if 

$$
\Gamma (t _ {i}) v (t _ {i}) := K ^ {*} (t _ {i + 1}) - K ^ {0} (t _ {i + 1})\tag{18.6}
$$

has a solution $v(t_{i})$ (not only in the sense of a closest approximation). If however (18.6) has no solution, $v(t_{i})$ from (18.2) still defines a valid mean shift for the scheme $K^{*}$ . The scheme $K^{1}$ will be the closest approximation to $K^{0}$ fulfilling the measure continuity condition with respect to $K^{*}$ . 

A major advantage of the partial proxy scheme is that the projection $\Pi$ may be chosen such that (18.2) has an exact solution with respect to the sub-manifold defined by $\Pi$ , so $K^{1}$ and $K^{0}$ coincide on a k-dimensional sub-manifold. We will make use of this in our example in Section 18.4.6. 

## 18.4.3. Non-Linear Proxy Constraint

An obvious (and commonly required) generalization is to replace the linear projection operator $\Pi$ by a general, possibly non-linear function $f : R^{n} \to R^{k}$ and define $v(t_{i})$ as the solution of 

$$
f (t _ {i + 1}, K ^ {0} (t _ {i + 1})) = f (t _ {i + 1}, K ^ {*} (t _ {i + 1}) - \Gamma (t _ {i}) \cdot v (t _ {i})).\tag{18.7}
$$

Thus we have $f(t_{i+1}, K^{0}(t_{i+1})) = f(t_{i+1}, K^{1}(t_{i+1}))$ . An example of an application of this generalization is a LIBOR Market Model, where f represents a certain swap rate or function of swap rates (e.g. a CMS spread). The condition will then ensure that the path values of the swap rate(s) are the same under $K^{0}$ and $K^{1}$ . 

## 18.4.3.1. Linearization of the Proxy Constraint

While a constraint like (18.7) will be the general application, its numerical implementation may be expensive, since one has to solve the non-linear equation on every path in every timestep. However, if $K^{*}(t_{i+1})$ is a small perturbation of $K^{0}(t_{i+1})$ , we may linearize Equation 18.7. In other words we would set 

$$
\Pi := f ^ {\prime} (K ^ {0} (t _ {i + 1})).\tag{18.8}
$$

Note that the proxy simulation method is constructed such that a finite difference using small perturbation will remain stable, i.e. $K^{*}(t_{i+1})$ may be chosen to be arbitrarily close to $K^{0}(t_{i+1})$ . 

$^{1}$ We will later consider the general case of non-linear proxy constraints and $F_{t_{i}}$ measurable mean shifts, see Section 18.4.3 and 18.4.4. 

## 18.4.3.2. Finite Difference Approximation of the Non-Linear Proxy Constraint

The linearization (18.8) of $f$ may still result in relatively large computational costs, because the projection operator has to be calculated on every path. Note that we linearize around $K^0(t_{i+1},\omega)$ . Thus the quasi-inverse of $\Pi \Gamma$ has to be calculated on every path in every time-step. If we want to implement a faster calculation of the mean shift $v(t_i,\omega_j)$ we can calculate an approximate solution of (18.7) by guessing the directional shift $\tilde{v}(t_i)$ and finite differences to determine the shift size: 

Assume we knew that the directional shift $\tilde{v}(t_{i})$ does not lie in Kernf'Γ. Then for some $\epsilon > 0$ calculate 

$$
\Delta_ {- \epsilon \Gamma \tilde {v} (t _ {i})} f := \frac {1}{\epsilon} (f (t _ {i + 1}, K ^ {*} (t _ {i + 1}) - \epsilon \cdot \Gamma (t _ {i}) \cdot \tilde {v} (t _ {i})) - f (t _ {i + 1}, K ^ {0} (t _ {i + 1})))\tag{18.9}
$$

and set 

$$
\Gamma \cdot v (t _ {i}) := (\Delta_ {- \epsilon \tilde {v} (t _ {i})}) ^ {- 1} \cdot \tilde {v} (t _ {i})\tag{18.10}
$$

in the definition of the partial proxy scheme $K^1$ , (18.4). 

This solution has the desirable property, that its implementation allows the constraint function f to be specified exogenously by the user; this constraint function may vary with the application. 

Example: If K is the log of the forward rates under a LIBOR Market Model and f is a swap rate, i.e. we would like to keep a swap rate rigid, then we can achieve this by modifying the first factor. This corresponds to $\tilde{v}(t_{i}) = (1, 0, \ldots, 0)$ . From (18.9) we can calculate the impact of a shift of the first factor on the swap rate; from (18.10) we can calculate the required magnitude of this shift (it is scalar equation with a scalar unknown $v_{1}(t_{i})$ ). 

We will consider a constraint like $(18.7)$ next, in our benchmark application, a trigger option on an index like a CMS swap rate considered under the LIBOR Market Model. 

## 18.4.4. Transition Probability from a Nonlinear Proxy Constraint

## 18.4.4.1. The Proxy Constraint Revisited

There is subtle but crucial detail in the definition of the mean shift $v(t_i)$ : It is defined by comparing $K^{*}(t_{i + 1})$ to $K^0 (t_{i + 1})$ 

$$
f (t _ {i + 1}, K ^ {0} (t _ {i + 1})) = f (t _ {i + 1}, K ^ {*} (t _ {i + 1}) - \Gamma (t _ {i}) \cdot v (t _ {i})),\tag{18.11}
$$

not by comparing $K^{*}(t_{i})$ to $K^{0}(t_{i})$ . Thus, in general, $v(t_{i})$ is a $F_{t_{i+1}}$ -measurable random variable, but not $F_{t_{i+1}}$ -measurable. $^{2}$ If we would define $v(t_{i})$ through 

$$
f (t _ {i + 1}, K ^ {0} (t _ {i})) = f (t _ {i + 1}, K ^ {*} (t _ {i}) - \Gamma (t _ {i}) \cdot v (t _ {i})),
$$

then it is not guaranteed that 

$$
f (t _ {i + 1}, K ^ {0} (t _ {i + 1})) = f (t _ {i + 1}, K ^ {*} (t _ {i + 1}) - \Gamma (t _ {i}) \cdot v (t _ {i})),
$$

$^{2}$ In the following we will say $v(t_{i})$ is $F_{t_{i+1}}$ -measurable only, if it is $F_{t_{i+1}}$ -measurable but not $F_{t_{i}}$ -measurable. 

holds, after the drift and the diffusion from $t_{i}$ to $t_{i+1}$ has been applied. To account for the drift we could define $v(t_{i})$ through 

$$
f (t _ {i + 1}, K ^ {0} (t _ {i}) + \mu^ {0} (t _ {i}) \Delta t _ {i}) = f (t _ {i + 1}, K ^ {*} (t _ {i}) + \mu^ {*} (t _ {i}) \Delta t _ {i} - \Gamma (t _ {i}) \cdot v (t _ {i})),\tag{18.12}
$$

which makes $v(t_{i})$ a $F_{t_{i}}$ -measurable random variable, but there is still no guarantee that the proxy constraint holds after the diffusion has been applied. However, it will be the case for linear constraints. 

From this consideration it becomes obvious that for the linearization of the proxy constraint, we would have to linearize around $K^{0}(t_{i+1})$ and not around $K^{0}(t_{i})$ . As a solution of this linearization $v(t_{i})$ will be $F_{t_{i+1}}$ -measurable only. 

If the mean shift $v(t_{i})$ is defined by (18.11) as a $F_{t_{i+1}}$ -measurable random variable it means - using Euler schemes - that $v(t_{i})$ depends non-linearly on the increment $\Delta W(t_{i})$ and the formula for the corresponding transition probability involves inverting this dependence. Here are two examples: 

## 18.4.4.2. Transition Probabilities for General Proxy Constraints

If the proxy constraint on time $t_{i+1}$ is linear, then it may be realized by an $F_{t_{i}}$ measurable mean-shift $v(t_{i})$ . In this case the calculation of the transition probabilities that form the Monte-Carlo weight leads to very simple formulas. From (18.5) we find that for an $F_{t_{i}}$ -measurable mean-shift 

$$
w (t _ {i}) = \prod_ {k = 1} ^ {m} \exp \left(- \frac {(x _ {k} - v _ {k} (t _ {i})) ^ {2} + x _ {k} ^ {2}}{2 \Delta t _ {i}}\right) \qquad \text { where } x _ {k} := \Delta W _ {k} (t _ {i}).\tag{18.13}
$$

If the mean shift $v(t_{i})$ is only $F_{t_{i+1}}$ -measurable, then it is still possible to obtain a simple analytic formula for the transition probability; however, this formula requires the differentiation of the functional dependence of $v(t_{i})$ on the increment $\Delta W(t_{i})$ . 

Consider the general case where the mean shift $v(t_i)$ depends on the Brownian increment $\Delta W(t_i)$ , i.e. 

$$
v (t _ {i}) = v (t _ {i}, \Delta W (t _ {i})).
$$

Define $\tilde{x} = g(x) := x - v(t_i, x)$ . Obviously we have 

$$
\phi (\tilde {x}) \mathrm{d} \tilde {x} \stackrel {\tilde {x} = g (x)} {=} \phi (g (x)) \mathrm{det} \left(\frac {\partial v (t _ {i} , x)}{\partial x}\right) \mathrm{d} x = \frac {\phi (g (x)) \mathrm{det} \left(\frac {\partial g (x)}{\partial x}\right)}{\phi (x)} \phi (x) \mathrm{d} x.\tag{18.14}
$$

Here x denotes the (realization of the) Brownian increment $\Delta W$ and $\phi$ denotes its probability density. Evaluating functions of $\tilde{x} = g(x)$ corresponds to pricing under the partial proxy scheme $K^{1}$ ; evaluating functions of x corresponds to the pricing under the target scheme $K^{*}$ . From (18.14) we can read off the Monte-Carlo weights for the pricing under the scheme $K^{1}$ as 

$$
w \left(t _ {i}\right) = \det \left(I - \frac {\partial v \left(t _ {i} , x\right)}{\partial x}\right) \cdot \prod_ {k = 1} ^ {m} \exp \left(- \frac {\left(x _ {k} - v _ {k} \left(t _ {i}\right)\right) ^ {2} + x _ {k} ^ {2}}{2 \Delta t _ {i}}\right) \quad \text { where } x _ {k} := \Delta W _ {k} \left(t _ {i}\right).\tag{18.15}
$$

Obviously this result is not limited to the case of Euler schemes. The only requirement with respect to the scheme is that it is generated by the Brownian increments $\Delta W(t_{i})$ (e.g. as for a Milstein scheme). We summarise our result in a theorem: 

Lemma (partial proxy): Let $K^{*}(t_{i}), i = 0, 1, 2, \ldots$ , denote a numerical scheme generated from the Brownian increments $\Delta W(t_{i}), i = 0, 1, 2, \ldots$ (target scheme), i.e. 

$$
K ^ {*} (t _ {i + 1}) = K ^ {*} (t _ {i + 1}, K ^ {*} (t _ {i}), \Delta W (t _ {i}) - v (t _ {i}))
$$

Let $K^{0}(t_{i}), i = 0,1,2,\ldots$ denote another numerical scheme, also generated from the Brownian increments $\Delta W(t_{i})$ and close to $K^{*}$ . 

For a given function $f$ (the proxy constraint) let $v(t_i)$ denote a solution of 

$$
f (t _ {i + 1}, K ^ {*} (t _ {i + 1}, K ^ {*} (t _ {i}), \Delta W (t _ {i}) - v (t _ {i}))) = f (t _ {i + 1}, K ^ {1} (t _ {i + 1}))
$$

and - assuming a solution exists - define the scheme $K^{1}$ by 

$$
K ^ {1} (t _ {i + 1}) := K ^ {*} (t _ {i + 1}, K ^ {*} (t _ {i}), \Delta W (t _ {i}) - v (t _ {i})).
$$

Then the Monte-Carlo pricing under the scheme $K^{*}$ is, in the Monte-Carlo limit, equivalent to the pricing under the scheme $K^1$ using the Monte-Carlo weights $\prod w_i$ with $w_i$ given by (18.15). 

We call the scheme $K^1$ the (partial) proxy scheme satisfying the proxy constraint $f(t_{i+1}, K^1(t_{i+1})) = f(t_{i+1}, K^0(t_{i+1}))$ . 

## 18.4.4.3. Example

Since we desire an implementation that is both generic and fast, we would like to discuss a special case, sufficiently general for all our applications and simple enough to give direct formulas for the transition probabilities: 

Assume that $v(t_{i})$ is linearly dependent on the increment $\Delta W(t_{i})$ , i.e. 

$$
v (t _ {i}) := A (t _ {i}) \cdot \Delta W (t _ {i}) + b (t _ {i}),
$$

with A and b being $F_{t_{i}}$ -measurable. Then we have for the mean-shifted diffusion 

$$
\Delta W (t _ {i}) - v (t _ {i}) = (1 - A (t _ {i})) \cdot (\Delta W (t _ {i}) - b (t _ {i})).
$$

Thus the corresponding transition probability is normal distributed with mean $b(t_{i})$ and standard deviation $(1 - A(t_{i}))\sqrt{\Delta t_{i}}$ . Note that if the target scheme is a small perturbation of the reference scheme, then $A(t_{i})$ is small and $(1 - A(t_{i}))$ is non singular. 

So here, the $F_{t_{i+1}}$ -measurable mean shift is given by an $F_{t_{i}}$ -measurable mean shift b and a scaling of the “factor” $\Delta W$ . We will make use of this in our next example: A proxy constraint stabilizing the calculation of vega, the sensitivity with respect to a change in the diffusion coefficient. 

## 18.4.4.4. Approximating an $F_{t_{i+1}}$ -measurable proxy constraint by an $F_{t_{i}}$ -measurable proxy constraint

To allow rapid calculation of the transition probability we propose to approximate the proxy constraint (18.11) by (18.12). Thus $v(t_{i})$ is a $F_{t_{i}}$ -measurable mean-shift and the ratio of the transition probabilities is given by (18.13). 

In addition we propose to linearize this constraint around $K^{0}(t_{i}) + \mu^{0}(t_{i})\Delta t_{i}$ , defining the linear proxy constraint by $\Pi := f'(K^{0}(t_{i}) + \mu^{0}(t_{i})\Delta t_{i})$ . 

All of our benchmark examples are based on the approximative constraint (18.12) or its linearization. 

## 18.4.5. Sensitivity with respect to the Diffusion Coefficients – Vega

If we consider only an $F_{t_{i}}$ -measurable mean shift applied to the Brownian increment $\Delta W(t_{i})$ , then the method is not applicable to the calculation of a sensitivity with respect to the diffusion coefficient $\Gamma(t_{i})$ -a.k.a. vega. The reason is simple: There is no $F_{t_{i}}$ -measurable mean shift that will ensure that the proxy constraint holds at $t_{i+1}$ after a different ( $F_{t_{i+1}}$ -measurable) diffusion has been applied – not even if the proxy constraint is a linear equation. Neglecting the Brownian increment, as suggested in 18.4.4.4, is a step in the wrong direction, since we are interested in the sensitivity with respect to the diffusion coefficient. 

Of course, in our general formulation (18.11), a $F_{t_{i+1}}$ -measurable mean shift applied to the diffusion $\Delta W(t_{i})$ will ensure that the proxy constraint holds at time $t_{i+1}$ , even if the diffusion coefficient has changed. However, to obtain a simple formula for the transition probability and thus the Monte-Carlo weight $w(t_{i})$ , it is helpful to take an alternative view to the problem: The idea is similar to what is done in the case of a full proxy scheme (see [66]): We modify the diffusion of the proxy scheme to match the diffusion of the reference scheme and calculate the corresponding change of measure. In other words, we use the unperturbed diffusion coefficient for the (partial) proxy scheme. This adjustment is made prior to the calculation of the mean shift $v(t_{i})$ for the corresponding proxy constraint, which will correct additional differences in the drift, if any. 

From the previous section it is clear that this is equivalent to specifying a $F_{t_{i+1}}$ -measurable mean shift, being linear in the Brownian increment $\Delta W(t_{i})$ . 

## 18.4.6. Example: LIBOR Target Redemption Note

We are going to calculate delta and gamma for a TARN swap. The coupon for the period $[T_{i}, T_{i+1}]$ is an inverse floater $\max(K - 2 \cdot L(T_{i}, T_{i+1}), 0)$ and it is swapped against floating rate $L(T_{i}, T_{i+1})$ until the accumulated coupon reaches a given target coupon. If the accumulated coupon does not reach the target coupon, then the difference to the target coupon is paid at maturity. 

Thus the coupon of the tarn is linked to a trigger feature, similar to the digital caplet. However, here, the trigger depends on more than one rate, so it is not sufficient to set up a proxy constraint for a single forward rate, unlike for the digital caplet. 

Our unperturbed scheme is the LIBOR market model with the initial yield curve, evolving the log-LIBOR with an Euler scheme. The natural perturbed scheme is then the same, except for a different initial condition. We will use the following proxy constraint: 

$$
L ^ {1} (T _ {j}, T _ {j + 1}; t) = L ^ {0} (T _ {j}, T _ {j + 1}; t) \quad \forall t \in (T _ {j - 1}, T _ {j} ],
$$

for all periods of the model to obtain the preferred proxy scheme. The constraint is realized by a mean shift of the diffusion of the first factor, and since the forward rate follows a lognormal process, we have $v = (v_{1}, 0, \ldots, 0)$ with 

$$
v _ {1} (t) = \frac {\log (L ^ {0} (T _ {j} , T _ {j + 1} ; t)) - \log (L ^ {1} (T _ {j} , T _ {j + 1} ; t))}{f _ {1 , j}},
$$

where $f_{1,j}$ denotes the j-th component of the first factor. We assume here that $f_{1,j} \neq 0$ . A non-zero factor loading exists as long as the forward rate $L(T_{j}, T_{j+1})$ has a non-zero volatility. 

The results can be improved if the factor having the largest absolute factor loading is chosen (factor-pivoting). 

Figure 18.3 shows the delta and gamma of a TARN swap for different shift sizes of finite differences applied to standard re-simulation and partial proxy scheme simulation. For this example the interest rate curve was upward sloping from 2% to 10% and for the TARN we took K = 10% and a target coupon of 10%. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/67972ca2c9c644bc108b69489c60bffb19810b52601102dc6b5c17e6f87759a3.jpg)



Figure 18.3.: Dependence of the TARN gamma on the shift size of the finite difference approximation. Finite difference is applied to a direct simulation (red) and to a (partial) proxy scheme simulation (green). Each dot corresponds to one Monte-Carlo simulation with the stated number of paths. The red and green corridors represent the corresponding standard deviation.



The proxy scheme simulation shows no variance increase for small shift sizes while giving stable expected values for the sensitivity.


With small shifts the variance of the delta and gamma calculated under full re-evaluation increases and the mean becomes unstable, while the mean for delta and gamma calculated under partial proxy scheme remains stable and the variance small. For increasing shift size full re-evaluation stabilizes, but higher order effects give a significant bias. Very high shift increases the Monte-Carlo variance of the likelihood ratio and thus increases the variance of the delta and gamma calculated under the partial proxy scheme simulation. 

## 18.4.7. Example: CMS Target Redemption Note

Next we will kook at a target redemption note with a coupon $\max(K - 2 \cdot I(T_{i}), 0)$ , where the index $I(T_{i})$ is a constant maturity swaprate, i.e. $I(T_{i}) = S_{i,i+k}(T_{i})$ with 

$$
\begin{array}{r l} S _ {i, i + k} = \frac {P (T _ {i}) - P (T _ {i + k})}{\sum_ {j = i} ^ {k - 1} (T _ {j + 1} - T _ {j}) P (T _ {j + 1})} = \frac {\frac {P (T _ {i})}{P (T _ {i + k})} - 1}{\sum_ {j = i} ^ {k - 1} (T _ {j + 1} - T _ {j}) \frac {P (T _ {j + 1})}{P (T _ {i + k})}} \\ = \frac {\prod_ {l = i} ^ {i + k - 1} (1 + L (T _ {l}) (T _ {l + 1} - T _ {l})) - 1}{\sum_ {j = i} ^ {k - 1} (T _ {j + 1} - T _ {j}) \prod_ {l = j + 1} ^ {i + k - 1} (1 + L (T _ {l}) (T _ {l + 1} - T _ {l}))} \end{array}
$$

The swaprate $S_{i,i + k}(t)$ is a non-linear function of the forward rate curve $L_{j}(t), j = i,\dots ,i +$ 

## $k - 1$ which we denote by $S$ :

$$
S _ {i, i + k} (t) = S (L _ {i} (t), \ldots , L _ {i + k - 1} (t)).
$$

From the proxy simulation scheme we require $S$ under $L^1$ to match $S$ under the reference scheme $L^0$ . Our proxy constraint is therefore 

$$
S (L _ {i} ^ {1} (t), \ldots , L _ {i + k - 1} ^ {1} (t)) = S (L _ {i} ^ {0} (t), \ldots , L _ {i + k - 1} ^ {0} (t)).
$$

We solve this equation by modifying the first factor, i.e. in each time step $t_{j}$ we determine a single scalar $v_{1}(t_{j})$ such that 

$$
\begin{array}{r l} & S (L _ {i} ^ {*} (t _ {j + 1}) + v _ {1} (t _ {j}) \cdot f _ {1, i}, \ldots , L _ {i + k - 1} ^ {*} (t _ {j + 1}) + v _ {1} (t _ {j}) \cdot f _ {1, i + k - 1}) \\ & \qquad = S (L _ {i} ^ {0} (t _ {j + 1}), \ldots , L _ {i + k - 1} ^ {0} (t _ {j + 1})) \end{array}\tag{18.16}
$$

and define $L_{i}^{1}(t_{j+1}):=L_{i}^{*}(t_{j+1})+v_{1}(t_{j})\cdot f_{1,i}.$ 

To simplify and speed up the calculation, we (numerically) linearize equation (18.16) and get an explicit (first order) formula for $v_{1}$ , see (18.10). 

## 18.4.7.1. Delta and Gamma of a CMS TARN

The result of the calculation of delta and gamma is depicted in Figure 18.4. Using the simple linearized proxy constraint we see a small increase in Monte-Carlo variance for the gamma with very small shifts. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/885d5e4d45954421f807acbbdde9fbb9abba29e83d6bd4d6f3ad1ad44e1f2ee6.jpg)



Figure 18.4.: Dependence of the CMS TARN gamma on the shift size of the finite difference approximation. Finite difference is applied to a direct simulation (red) and to a (partial) proxy scheme simulation (green). The proxy constraint used was a simple (numerical) linearization of (18.16).


The linearized constraint remains stable for small shifts. However, using a few Newton iterations on the linearization solves the non-linear constraint and further improves the result for the gamma, see Figure 18.5. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/79b684bef6b65edc3dd77035e6f14dcd2919aa134bb03c30545fa28fc8f9a656.jpg)



Figure 18.5.: Dependence of the CMS TARN gamma on the shift size of the finite difference approximation. Finite difference is applied to a direct simulation (red) and to a (partial) proxy scheme simulation (green). The proxy constraint is given by applying a few Newton iterations to the (numerical) linearization of (18.16).


## 18.4.7.2. Vega of a CMS TARN

We will calculate the vega of a CMS TARN, i.e. the sensitivity of the CMS TARN with respect to a parallel shift of all instantaneous volatilities. The result is depicted in Figure 18.6. For medium and large shift size the vega calculated from finite differences applied to a partial proxy is similar to the vega calculated from finite differences applied to direct simulation. However, note that for very small shift sizes (around 1 bp), the vega calculated from finite differences applied to direct simulation converges to an incorrect value and that this result occurs with a very small Monte-Carlo variance. 

The reason for this effect is that the shifts are too small to trigger a change in the exercise strategy. Hence, the vega calculated is the sensitivity conditional on no change in exercise strategy, which is of course a different thing, see Section 17.2.4. 

This effect is also present for delta and gamma and for all trigger products, but it has not been visible in the figures so far due to the scale of the shift sizes and the number of paths used there. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/4658d97dd4c780617f056a72b045d097e8d44ca93589a9e38a72fb7da4bb68a7.jpg)



Figure 18.6.: Dependence of the CMS TARN vega on the shift size of the finite difference approximation. Finite difference is applied to a direct simulation (red) and to a (partial) proxy scheme simulation (green). The proxy constraint was given by applying a few Newton iterations to the (numerical) linearization of (18.16).


Part V. 

# Pricing Models for Interest Rate Derivatives

Oscar Wilde 

The Importance of Being Earnest, [39]. 

Up until now we have been considering models of a single scalar stochastic process and options on it: The Black-Scholes model for a stock S, or the Black model for a forward rate L. The true challenge in evaluation of interest rate products lies in the modeling of the whole interest rate curve (instead of a scalar) and in the evaluation of complex derivatives, which depend on the whole curve. 

Historically the path to modeling the interest rate curve started with the modeling of the short rate, from which we may calculate the whole interest rate curve, see Remark 104. The initial motivation for considering the short rate derived from the wish to model a scalar quantity, thus to be able to apply familiar numerical methods from stock models, e.g. binomial trees. 

For didactic reasons we are not going to present things chronologically. Instead, we consider the LIBOR Market Model first. It is a high dimensional model, which discretizes the interest rate curve into a finite number of forward rates. It is highly flexibly due to its huge number of free parameters. It will allow us to study model properties like mean reversion, number of factors (Chapter 24), instantaneous volatility, instantaneous and terminal correlation (Chapter 20). Despite its presumed complexity, the LIBOR Market Model is essentially a very simple model: It is nothing more than the simultaneous consideration of multiple Black models under a common measure. So we are carrying on from Chapter 10. 

For the Short Rate models the modeled quantity is the short rate, a quantity not directly observable. Here we model quantities which are observable as market quotes, like the LIBOR or the Swaprate. The class of models that model quantities which are directly observable on the market are called “Market Models”. We will look at the LIBOR Market Model first: 

## 19.1. LIBOR Market Model

We assume a time discretization (tenor structure) 

$$
0 = T _ {0} <   T _ {1} <   \dots <   T _ {n}.
$$

We model the forward rates $L_{i} := L(T_{i}, T_{i+1})$ for $i = 0, \ldots, n-1$ , see Definition 99. This represents a discretization of the interest rate curve, where the continuum of maturities has 

been discretized. $^{1}$ 

The LIBOR market model assumes a lognormal dynamic for LIBORs $L_{i} := L(T_{i}, T_{i+1})$ , i.e. $^{2}$ 

$$
\frac {\mathrm{d} L _ {i} (t)}{L _ {i} (t)} = \mu_ {i} ^ {\mathbb {P}} (t) \mathrm{d} t + \sigma_ {i} (t) \mathrm{d} W _ {i} ^ {\mathbb {P}} (t) \quad \text { for } i = 0, \dots , n - 1, \text { under } \mathbb {P},\tag{19.1}
$$

with initial conditions 

$$
L _ {i} (0) = L _ {i, 0},
$$

$$
\text { with } L _ {i, 0} \in [ 0, \infty), i = 0, \dots , n - 1,
$$

where $W_{i}^{P}$ denote (possibly instantaneously correlated) P-Brownian motions with 

$$
\mathrm{d} W _ {i} ^ {\mathbb {P}} (t) \mathrm{d} W _ {j} ^ {\mathbb {P}} (t) = \rho_ {i, j} (t) \mathrm{d} t.
$$

Let $\sigma_{i}:[0,T]\mapsto\mathbb{R}$ and $\rho_{i,j}:[0,T]\mapsto\mathbb{R}$ be deterministic functions and $\mu_{i}$ the Drift as $\mathcal{F}_{t}$ -adapted process. By $R(t):=(\rho_{i,j}(t))_{i,j=0,\ldots,n-1}$ we denote the correlation matrix. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/655ff4e8416f6c97dce5dc1ad579f78cdf6089ae1b2cf2039e53fbd877dd72a6.jpg)


Motivation: Equation (19.1) is a lognormal model for the forward rates $L_{i}$ . If we consider only a single equation, i.e. fix $i \in \{1, \ldots, n-1\}$ , it represents the Black model considered in Section 10: Equation (19.1) is identical with Equation (10.1). If we change the measure such that $L_{i}$ is drift-free (see Section 10), we see that distribution of $L_{i}$ is lognormal. 

the terminal distribution of $L_{i}$ is lognormal. 

Thus, the LIBOR market model is equivalent to the consideration of n Black models under a unified measure. 

As was discussed in Section 10, to evaluate a caplet under this model it is not relevant that $\sigma_{i}$ is time dependent (we have assumed time-dependency of $\sigma_{i}$ in Section 10 for didactical reasons). However, for the value of complex derivatives the time dependency matters. A further degree of freedom introduced in (19.1) is the instantaneous correlation $\rho_{i,j}$ of the driving Brownian motions. For the value of a caplet the instantaneous correlation is insignificant (indeed, it does not enter in the Black model). For the evaluation of Swaptions the correlation of the forward rates is significant. 

For further generalizations of the model, consider non-deterministic $\sigma_{i}$ , i.e. stochastic volatility models. In this case the terminal LIBOR distributions no longer correspond to the Black model ones, which is, of course, intended. Equation (19.1) is to be seen as a starting point of a whole model family. The model (19.1) has been chosen as the starting point, because (historically) the lognormal (Black) model is well understood, especially by traders. $^{3}$ 

Remark 211 (Interest Rate Structure): Equation (19.1) models the evolution of the LIBOR $L(T_{i}, T_{i+1})$ . Without further interpolation assumption, these are the shortest forward rates that can be considered in our time discretization (tenor structure). The equation system (19.1) thus determines the evolution of all bond prices with maturities $T_{i}$ and all forward rates for the 

periods $[T_i, T_k]$ , since 

$$
\begin{array}{c} 1 + L (T _ {i}, T _ {k}) (T _ {k} - T _ {i}) = \frac {P (T _ {i})}{P (T _ {k})} = \prod_ {j = i} ^ {k - 1} \frac {P (T _ {j})}{P (T _ {j + 1})} \\ = \prod_ {j = i} ^ {k - 1} (1 + L (T _ {j}, T _ {j + 1}) (T _ {j + 1} - T _ {j})). \end{array}
$$

To shorten notation we write $\delta_{i} := T_{i+1} - T_{i}, i = 0, \ldots, n - 1$ for the period length. 

## 19.1.1. Derivation of the Drift Term

As in Chapters 10 and 11, our first step is to choose some numéraire N and derive the drift under a martingale measure $Q^{N}$ . If the processes have been derived under the martingale measure $Q^{N}$ , then the (discretized) interest rate curve may be simulated numerically and a derivative V may be prices through $V(0) = N(0)\mathrm{E}^{\mathbb{Q}^{N}}\left(\frac{V}{N}|\mathcal{F}_{T_{0}}\right)$ (see Chapter 13). 

We fix a numéraire N. Let the assumptions of Theorem 74 hold, such that there exists a corresponding equivalent martingale measure $Q^{N}$ such that N-relative prices are martingales. From Theorem 58 under $Q^{N}$ the process (19.1) has a changed drift, namely 

$$
\frac {\mathrm{d} L _ {i} (t)}{L _ {i} (t)} = \mu_ {i} ^ {\mathbb {Q} ^ {N}} (t) \mathrm{d} t + \sigma_ {i} (t) \mathrm{d} W _ {i} ^ {\mathbb {Q} ^ {N}} (t) \quad \text { for } i = 0, \dots , n - 1.\tag{19.2}
$$

## 19.1.1.1. Derivation of the Drift Term under the Terminal Measure

We fix the $T_{n}$ -Bond $N(t) = P(T_{n}; t)$ as numéraire. From Theorem 58 under $\mathbb{Q}^{P(T_n)}$ the process (19.1) has a changed drift: 

$$
\frac {\mathrm{d} L _ {i} (t)}{L _ {i} (t)} = \mu_ {i} ^ {\mathbb {Q} ^ {P (T _ {n})}} (t) \mathrm{d} t + \sigma_ {i} (t) \mathrm{d} W _ {i} ^ {\mathbb {Q} ^ {P (T _ {n})}} (t) \quad \text { for } i = 0, \dots , n - 1.\tag{19.3}
$$

We need to determine $\mu_i^{\mathbb{Q}^{P(T_n)}}$ . The martingale measure $\mathbb{Q}^{P(T_n)}$ corresponding to $N(t) = P(T_n; t)$ is also called terminal measure (since $T_n$ is the time horizon of our time discretization). 

As in Chapter 10, we will construct relative prices with respect to $P(T_{n})$ and obtain equations from which we will derive the drifts $\mu_{i}$ . From Definition 99 

$$
\prod_ {k = i} ^ {n - 1} \underbrace {(1 + \delta_ {k} L _ {k})} _ {= \frac {P (T _ {k})}{P (T _ {k + 1})}} = \prod_ {k = i} ^ {n - 1} \frac {P (T _ {k})}{P (T _ {k + 1})} = \frac {P (T _ {i})}{P (T _ {n})} \quad \text { for } i = 0, \ldots , n - 1.\tag{19.4}
$$

Since we have a $P(T_{n})$ -relative price of a traded product on the right hand side in (19.4), we have for the drifts: 

$$
\underset {\mathbb {Q} ^ {P (T _ {n})}} {\text { Drift }} \left[ \prod_ {k = i} ^ {n - 1} (1 + \delta_ {k} L _ {k}) \right] = 0, \qquad i = 0, \ldots , n - 1.
$$

We apply Theorem 47 and obtain $\forall i = 0, \ldots, n - 1$ 

$$
\begin{aligned} \mathrm{d}\left(\prod_{k = i}^{n - 1}(1 + \delta_{k}L_{k})\right) & = \sum_{j = i}^{n - 1}\prod_{\substack{k = i\\ k\neq j}}^{n - 1}(1 + \delta_{k}L_{k})\cdot \delta_{j}\mathrm{d}L_{j} + \sum_{\substack{j,l = i\\ l > j}}^{n - 1}\prod_{\substack{k = i\\ k\neq j,l}}^{n - 1}(1 + \delta_{k}L_{k})\cdot \delta_{j}\mathrm{d}L_{j}\delta_{l}\mathrm{d}L_{l}\\ & = \prod_{k = i}^{n - 1}(1 + \delta_{k}L_{k})\cdot \left(\sum_{j = i}^{n - 1}\frac{\delta_{j}\mathrm{d}L_{j}}{(1 + \delta_{j}L_{j})} +\sum_{\substack{j,l = i\\ l > j}}^{n - 1}\frac{\delta_{j}\mathrm{d}L_{j}}{(1 + \delta_{j}L_{j})}\cdot \frac{\delta_{l}\mathrm{d}L_{l}}{(1 + \delta_{l}L_{l})}\right)\\ & = \prod_{k = i}^{n - 1}(1 + \delta_{k}L_{k})\cdot \sum_{j = i}^{n - 1}\left(\frac{\delta_{j}\mathrm{d}L_{j}}{(1 + \delta_{j}L_{j})} +\sum_{\substack{l\geq j + 1\\ l\leq n - 1}}\frac{\delta_{j}\mathrm{d}L_{j}}{(1 + \delta_{j}L_{j})}\cdot \frac{\delta_{l}\mathrm{d}L_{l}}{(1 + \delta_{l}L_{l})}\right). \end{aligned}
$$

Since $\forall i = 0,\dots ,n - 1$ 

$$
\underset {\mathbb {Q} ^ {P (T _ {n})}} {\text { Drift }} \left[ \prod_ {k = i} ^ {n - 1} (1 + \delta_ {k} L _ {k}) \right] = 0\tag{19.5}
$$

it follows that $\forall i = 0, \ldots, n - 1$ 

$$
\sum_{j = i}^{n - 1}\operatorname{Drift}_{\mathbb{Q}^{P(T_{n})}}\left[\frac{\delta_{j}\mathrm{d}L_{j}}{(1 + \delta_{j}L_{j})} +\sum_{\substack{l\geq j + 1\\ l\leq n - 1}}\frac{\delta_{j}\mathrm{d}L_{j}}{(1 + \delta_{j}L_{j})}\cdot \frac{\delta_{l}\mathrm{d}L_{l}}{(1 + \delta_{l}L_{l})}\right] = 0\tag{19.6}
$$

and thus $\forall j = 0, \ldots, n - 1$ 

$$
\operatorname{Drift}_{\mathbb{Q}^{P(T_{n})}}\left[ \frac{\delta_{j}\mathrm{d}L_{j}}{(1 + \delta_{j}L_{j})} +\sum_{\substack{l\geq j + 1\\ l\leq n - 1}}\frac{\delta_{j}\mathrm{d}L_{j}}{(1 + \delta_{j}L_{j})}\cdot \frac{\delta_{l}\mathrm{d}L_{l}}{(1 + \delta_{l}L_{l})} \right] = 0\tag{19.7}
$$

If we now use 

$$
\mathrm{d} L _ {j} = L _ {j} \mu_ {j} ^ {\mathbb {Q} ^ {P (T _ {n})}} \mathrm{d} t + L _ {j} \sigma_ {j} \mathrm{d} W _ {j} ^ {\mathbb {Q} ^ {P (T _ {n})}} \quad \text { and } \quad \mathrm{d} L _ {j} \cdot \mathrm{d} L _ {l} = L _ {j} L _ {l} \sigma_ {j} \sigma_ {l} \rho_ {j, l} \mathrm{d} t
$$

in (19.7), then we have 

$$
\mu_{j}^{\mathbb{Q}^{P(T_{n})}}\frac{\delta_{j}L_{j}}{(1 + \delta_{j}L_{j})} +\sum_{\substack{l\geq j + 1\\ l\leq n - 1}}\frac{\delta_{j}L_{j}}{(1 + \delta_{j}L_{j})}\cdot \frac{\delta_{l}L_{l}}{(1 + \delta_{l}L_{l})}\cdot \sigma_{j}\sigma_{l}\rho_{j,l} = 0,
$$

i.e. 

$$
\mu_{j}^{\mathbb{Q}^{P(T_{n})}}(t) = -\sum_{\substack{l\geq j + 1\\ l\leq n - 1}}\frac{\delta_{l}L_{l}(t)}{(1 + \delta_{l}L_{l}(t))}\cdot \sigma_{j}(t)\sigma_{l}(t)\rho_{j,l}(t).\tag{19.8}
$$

The procedure above may be summarized as follows: To derive the n drifts we write down n independent traded assets as a function of the model quantities. By considering the drifts of their relative prices we obtain n equations for the drifts of the modeled quantities. 

## 19.1.1.2. Derivation of the Drift Term under the Spot LIBOR Measure

We fix the rolled over one period bond as numéraire, i.e. the investment of 1 at time $T_{0}$ into the $T_{1}$ -Bond and after its maturity the reinvestment of the proceeds into the bond of the next period, i.e. in $T_{j}$ the reinvestment inf the $T_{j+1}$ -Bond. It is 

$$
\begin{array}{l} N (t) := P (T _ {m (t) + 1}; t) \prod_ {j = 1} ^ {m (t) + 1} \underbrace {\frac {1}{P (T _ {j} ; T _ {j - 1})}} _ {= \frac {P (T _ {j - 1} ; T _ {j - 1})}{P (T _ {j} ; T _ {j - 1})} = (1 + L _ {j - 1} (T _ {j - 1}) \delta_ {j - 1})} \end{array} = P (T _ {m (t) + 1}; t) \prod_ {j = 0} ^ {m (t)} (1 + L _ {j} (T _ {j}) \cdot \delta_ {j}),\tag{19.9}
$$

$m(t) := \max\{i : T_i \leq t\}$ and $\delta_j := T_{j+1} - T_j$ . The corresponding equivalent martingale measure $\mathbb{Q}^N$ is called the spot measure. 

As before, we consider the processes of $N$ -relative prices of traded products (from which we know that they have drift 0 under $\mathbb{Q}^N$ ). We consider the $N$ -relative prices of the bonds $P(T_i)$ . It is 

$$
\begin{array}{l} \frac {P (T _ {i} ; t)}{N (t)} = \frac {P (T _ {i} ; t)}{P (T _ {m (t) + 1} ; t)} \cdot \prod_ {j = 0} ^ {m (t)} (1 + L _ {j} (T _ {j}) \delta_ {j}) ^ {- 1} \\ = \prod_ {j = m (t) + 1} ^ {i - 1} (1 + L _ {j} (t) \delta_ {j}) ^ {- 1} \cdot \prod_ {j = 0} ^ {m (t)} (1 + L _ {j} (T _ {j}) \delta_ {j}) ^ {- 1}, \end{array}\tag{19.10}
$$

thus 

$$
\operatorname{Drift} _ {\mathbb {Q} ^ {N}} \left[ \prod_ {k = m (t) + 1} ^ {i - 1} \left(1 + L _ {k} \delta_ {k}\right) ^ {- 1} \right] = 0.\tag{19.11}
$$

Since 

$$
\begin{array}{l} \mathrm{d} \left(\prod_ {j = m (t) + 1} ^ {i - 1} (1 + L _ {j} (t) \delta_ {j}) ^ {- 1} \cdot \prod_ {j = 0} ^ {m (t)} (1 + L _ {j} (T _ {j}) \delta_ {j}) ^ {- 1}\right) \\ = \mathrm{d} \left(\prod_ {j = m (t) + 1} ^ {i - 1} (1 + L _ {j} (t) \delta_ {j}) ^ {- 1}\right) \cdot \prod_ {j = 0} ^ {m (t)} (1 + L _ {j} (T _ {j}) \delta_ {j}) ^ {- 1} \end{array}
$$

we consider 

$$
\begin{aligned} & \mathrm{d}\left(\prod_{k = m(t) + 1}^{i - 1}\frac{1}{(1 + \delta_kL_k)}\right)\\ & = \sum_{j = m(t) + 1}^{i - 1}\prod_{\substack{k = m(t) + 1 \\ k\neq j}}^{i - 1}\frac{1}{(1 + \delta_kL_k)}\cdot \left(\frac{-\delta_j\mathrm{d}L_j}{(1 + \delta_jL_j)^2} +\frac{\delta_j^2\mathrm{d}L_j\mathrm{d}L_j}{(1 + \delta_jL_j)^3}\right)\\ & \quad +\sum_{\substack{j,l = m(t) + 1 \\ l <   j}}^{i - 1}\prod_{\substack{k = m(t) + 1 \\ k\neq j,l}}^{i - 1}\frac{1}{(1 + \delta_kL_k)}\cdot \left(\frac{\delta_j\mathrm{d}L_j}{(1 + \delta_jL_j)^2} +\frac{\delta_j^2\mathrm{d}L_j\mathrm{d}L_j}{(1 + \delta_jL_j)^3}\right)\left(\frac{\delta_l\mathrm{d}L_l}{(1 + \delta_lL_l)^2} +\frac{\delta_l^2\mathrm{d}L_l\mathrm{d}L_l}{(1 + \delta_lL_l)^3}\right)\\ & = \prod_{k = m(t) + 1}^{i - 1}\frac{1}{(1 + \delta_kL_k)}\cdot \left(\sum_{j = m(t) + 1}^{i - 1}\frac{-\delta_j\mathrm{d}L_j}{(1 + \delta_jL_j)} +\frac{\delta_j^2\mathrm{d}L_j\mathrm{d}L_j}{(1 + \delta_jL_j)^2} +\sum_{\substack{j,l = m(t) + 1 \\ l <   j}}^{i - 1}\frac{-\delta_j\mathrm{d}L_j}{(1 + \delta_jL_j)}\cdot \frac{-\delta_l\mathrm{d}L_l}{(1 + \delta_lL_l)}\right)\\ & = \prod_{k = m(t) + 1}^{i - 1}\frac{1}{(1 + \delta_kL_k)}\cdot \sum_{j = m(t) + 1}^{i - 1}\left(-\frac{\delta_j\mathrm{d}L_j}{(1 + \delta_jL_j)} +\sum_{l = m(t) + 1}^{j}\frac{\delta_j\mathrm{d}L_j}{(1 + \delta_jL_j)}\cdot \frac{\delta_l\mathrm{d}L_l}{(1 + \delta_lL_l)}\right). \end{aligned}
$$

With (19.11) we have $\forall i = 0, \ldots, n - 1$ 

$$
\sum_ {j = m (t) + 1} ^ {i - 1} \mathrm{Drift} _ {\mathbb {Q} ^ {N}} \left[ - \frac {\delta_ {j} \mathrm{d} L _ {j}}{(1 + \delta_ {j} L _ {j})} + \sum_ {l = m (t) + 1} ^ {j} \frac {\delta_ {j} \mathrm{d} L _ {j}}{(1 + \delta_ {j} L _ {j})} \cdot \frac {\delta_ {l} \mathrm{d} L _ {l}}{(1 + \delta_ {l} L _ {l})} \right] = 0
$$

and thus $\forall j = 0, \dots, n - 1$ 

$$
\operatorname{Drift} _ {\mathbb {Q} ^ {N}} \left[ \frac {- \delta_ {j} \mathrm{d} L _ {j}}{(1 + \delta_ {j} L _ {j})} + \sum_ {l = m (t) + 1} ^ {j} \frac {\delta_ {j} \mathrm{d} L _ {j}}{(1 + \delta_ {j} L _ {j})} \cdot \frac {\delta_ {l} \mathrm{d} L _ {l}}{(1 + \delta_ {l} L _ {l})} \right] = 0\tag{19.12}
$$

If we now use 

$$
\mathrm{d} L _ {j} = L _ {j} \mu_ {j} ^ {\mathbb {Q} ^ {N}} \mathrm{d} t + L _ {j} \sigma_ {j} \mathrm{d} W _ {j} \quad \text { and } \quad \mathrm{d} L _ {j} \cdot \mathrm{d} L _ {l} = L _ {j} L _ {l} \sigma_ {j} \sigma_ {l} \rho_ {j, l} \mathrm{d} t
$$

in (19.7), then we have $^{4}$ 

$$
- \mu_ {j} ^ {\mathbb {Q} ^ {N}} \frac {\delta_ {j} L _ {j}}{(1 + \delta_ {j} L _ {j})} + \sum_ {l = m (t) + 1} ^ {j} \frac {\delta_ {j} L _ {j}}{(1 + \delta_ {j} L _ {j})} \cdot \frac {\delta_ {l} L _ {l}}{(1 + \delta_ {l} L _ {l})} \cdot \sigma_ {j} \sigma_ {l} \rho_ {j, l} = 0,
$$

i.e. 

$$
\mu_ {j} ^ {\mathbb {Q} ^ {N}} (t) = \sum_ {l = m (t) + 1} ^ {j} \frac {\delta_ {l} L _ {l} (t)}{1 + \delta_ {l} L _ {l} (t)} \sigma_ {j} (t) \sigma_ {l} (t) \rho_ {j, l} (t).
$$

## 19.1.1.3. Derivation of the Drift Term under the $T_{k}$ -Forward Measure

Exercise: (Drift under the $T_{k}$ -forward measure) Consider 

$$
N (t) := \left\{ \begin{array}{l l} P (T _ {k}; t)  , & t \leq T _ {k} \\ P (T _ {m (t) + 1}; t) \prod_ {j = k + 1} ^ {m (t) + 1} \frac {1}{P (T _ {j} ; T _ {j - 1})}  , & t > T _ {k}, \end{array} \right.
$$

where $m(t) := \max\{i : T_i \leq t\}$ . 

$^{4}$ Since the coefficient of dt equals 0. 

1. Give an interpretation of $N(t)$ as traded product. 

2. Derive the drift of the model (19.1) under the $\mathbb{Q}^N$ measure with the numéraire $N$ . 

Solution: 

$$
\mu_ {j} (t) = - \sum_ {l = j + 1} ^ {k - 1} \frac {\delta_ {l} L _ {l}}{(1 + \delta_ {l} L _ {l})} \sigma_ {j} \sigma_ {l} \rho_ {j, l} \quad \text { for } j <   k - 1 \quad \text { and } t \leq T _ {k}
$$

$$
\mu_ {j} (t) = 0
$$

$$
\text {   for   } j = k - 1 \quad \text {   and   } t \leq T _ {k}
$$

$$
\mu_ {j} (t) = \sum_ {l = m (t) + 1} ^ {j} \frac {\delta_ {l} L _ {l}}{(1 + \delta_ {l} L _ {l})} \sigma_ {j} \sigma_ {l} \rho_ {j, l}
$$

$$
\mu_ {j} (t) = \sum_ {l = k} ^ {j} \frac {\delta_ {l} L _ {l}}{(1 + \delta_ {l} L _ {l})} \sigma_ {j} \sigma_ {l} \rho_ {j, l} \qquad \mathrm{for} j \geq k \qquad \mathrm{and} t \leq T _ {k}
$$

$$
\text { for } t > T _ {k}.
$$

## 19.1.2. The Short Period Bond $P(T_{m(t)+1}; t)$

For $t \notin \{T_{1}, \ldots, T_{n}\}$ neither the numéraire $N(t)$ of the terminal measure nor the numéraire of the spot measure is not fully described by the processes $L_{i}(t)$ . The unspecified bond $P(T_{m(t)+1}; t)$ occurs in both numéraires. We will now discuss the relevance of $P(T_{m(t)+1}; t)$ . 

## 19.1.2.1. Role of the short bond in a LIBOR Market Model

For the modeling of the forward rates $L_{i}(t) := L(T_{i}, T_{i+1}; t)$ on the tenor periods $[T_{i}, T_{i+1}]$ , $i = 0, \ldots, n$ the specification of $P(m(t) + 1; t)$ is irrelevant. For the derivation of the corresponding drift terms it was not relevant to specify the stochastic of $P(T_{m(t)+1}; t)$ , since the term canceled for the relative prices considered. 

Conversely, the LIBOR Market Model does not describe the stochastic of the short bond $P(T_{m(t)+1}; t)$ , since it is not given as a function of the processes $L_{i}(t)$ . 

## 19.1.2.2. Link to continuous time tenors

The specification of the short bond $P(T_{m(t)+1};t)$ becomes relevant if the model has to describe interest rates of interest rate periods which are not part of the tenor structure. The specification of $P(m(t)+1;t)$ will determine how the fractional forward rates $L(T_{s},T_{e};t)$ with $T_{s}\notin\{T_{1},\ldots,T_{n}\}$ and/or $T_{e}\notin\{T_{1},\ldots,T_{n}\}$ will evolve (see Section 19.1.5). It is the link from a model with discrete tenors (LIBOR Market Model) to a model with continuous time tenors (Heath-Jarrow-Morton Framework). In the special case where $P(m(t)+1;t)$ has zero volatility, the LIBOR Market Model under spot measure coincides with a Heath-Jarrow-Morton Framework with a special volatility structure under the risk-neutral measure (see Section 23.2). 

## 19.1.2.3. Drift of the short bond in a LIBOR Market Model

Within the LIBOR Market Model there is no constraint on the drift of $P(m(t) + 1; t)$ , because in $\frac{P(m(t)+1;t)}{N(t)}$ the term cancels out. The relative price $\frac{P(m(t)+1;t)}{N(t)}$ is always a martingale for any choice of $P(m(t) + 1; t)$ . This might come as a surprise, but we have already encountered this behavior: In the Black-Scholes model the drift r of $B(t)$ is a free parameter, because it is the drift of the numéraire. The parameter r is determined by calibration to a market interest rate. In a short rate model the drift is a free parameter. It is determined by calibration to the market interest rate curve, see Section 22. Here, similarly, $P(m(t) + 1; t)$ determines the interpolation of the initial interest rate curve. 

The trivial fact that the numéraire relative price of the numéraire, i.e. $\frac{N(t)}{N(t)}$ , is always a martingale plays a role in Markov functional models. There, the numéraire is postulated to be a functional of some Markov process. 

## 19.1.3. Discretization and (Monte-Carlo) Simulation

In this section we will discuss the discretization and implementation of the model. Let us therefore assume that the free parameters $\sigma_{i}, \rho_{i,j}$ and $L_{i,0} (i, j = 1, \ldots, n)$ are given. Together with the drift formula obtained in the previous section the model is fully specified. In Section 19.1.4 will then discuss how the parameters $L_{i,0}, \sigma_{i}, \rho_{i,j}$ are obtained. 

## 19.1.3.1. Generation of the (time-discrete) Forward Rate Process

As discussed in Chapter 13, we choose the Euler discretization of the Itô process of $\log (L_i)$ . From Lemma 49 we have 

$$
\mathrm{d} (\log (L _ {i} (t))) = \left(\mu_ {i} ^ {\mathbb {Q} ^ {N}} (t) - \frac {1}{2} \sigma_ {i} ^ {2} (t)\right) \mathrm{d} t + \sigma_ {i} (t) \mathrm{d} W _ {i} ^ {\mathbb {Q} ^ {N}} (t)\tag{19.13}
$$

and the corresponding Euler scheme of (19.13) is 

$$
\log (\tilde {L} _ {i} (t + \Delta t)) = \log (\tilde {L} _ {i} (t)) + (\mu_ {i} (t) - \frac {1}{2} \sigma_ {i} ^ {2} (t)) \Delta t + \sigma_ {i} (t) \Delta W _ {i} (t),.\tag{19.14}
$$

Applying the exponential gives us the discretization scheme of $L_{i}$ as 

$$
\tilde {L} _ {i} (t + \Delta t) = \tilde {L} _ {i} (t) \cdot \exp \big ((\mu_ {i} (t) - \frac {1}{2} \sigma_ {i} ^ {2} (t)) \Delta t + \sigma_ {i} (t) \Delta W _ {i} (t) \big).\tag{19.15}
$$

In the special case that the process $L_{i}$ is considered under the measure $\mathbb{Q}^{P(T_{i+1})}$ , i.e. $\mu_{i}^{\mathbb{Q}^{P(T_{i+1})}}(t)=0$ , and that the given $\sigma_{i}(t)$ is a known deterministic function, then we may use the exact solution for a discretization scheme: 

$$
L _ {i} (t + \Delta t) = L _ {i} (t) \cdot \exp \big (- \frac {1}{2} \bar {\sigma} _ {i} ^ {2} (t, t + \Delta t) \Delta t + \bar {\sigma} _ {i} (t, t + \Delta t) \Delta W _ {i} \big),
$$

where 

$$
\bar {\sigma} _ {i} (t, t + \Delta t) := \sqrt {\frac {1}{\Delta t} \int_ {t} ^ {t + \Delta t} \sigma_ {i} ^ {2} (\tau) \mathrm{d} \tau}.
$$

In the case where $L_{i}$ is not drift-free, we choose instead of (19.15) the discretization scheme 

$$
L _ {i} (t + \Delta t) = L _ {i} (t) \cdot \exp \big ((\mu_ {i} (t) - \frac {1}{2} \bar {\sigma} _ {i} (t, t + \Delta t) ^ {2}) \Delta t + \bar {\sigma} _ {i} (t, t + \Delta t) \Delta W _ {i} (t) \big)\tag{19.16}
$$

(we write L in place of $\tilde{L}$ , although (19.16) is an approximation of (19.1)). The diffusion dW is discretized by exact solution; the drift dt is discretized by an Euler scheme. The discretization error of this scheme stems from the discretization of the stochastic drift $\mu_{i}$ only. This discretization error results in a violation of the no-arbitrage requirement of the model (the discretized model does not have the correct, arbitrage-free drift). Methods which do not exhibit an arbitrage due to a discretization error are called arbitrage-free discretization, see [69]). 

The volatility functions $\sigma_{i}$ are usually assumed to be piecewise constant functions on $[T_{j}, T_{j+1})$ , such that $\bar{\sigma}_{i}(t, t + \Delta t)$ may be calculated analytically. It is $\bar{\sigma}_{i}(t, t + \Delta t) = \sigma_{i}(t)$ . 

## 19.1.3.2. Generation of the Sample Paths

Equipped with the time discretization (19.16), realizations of the process are calculated for a given number of paths $\omega_{1},\omega_{2},\omega_{3},\ldots$ . To do so, normal distributed random numbers $\Delta W_{i}(t_{j})(\omega_{k})$ , correlated according to $R = (\rho_{i,j})$ , are generated (see Appendix A.2 and A.3). These are used in the scheme (19.16). The result is a three dimensional tensor $L_{i}(t_{j},\omega_{k})$ parametrized by 

i : Index of the interest rate period (tenor structure), 

j : Index of the simulation time, 

k : Index of the simulation path. 

## 19.1.3.3. Generation of the Numéraire

Given a simulated interest rate curve $L_{i}(t_{j},\omega_{k})$ , we can calculate the numéraire. Of course we have to use the numéraire that was chosen for the martingale measure under which the process was simulated (form of the drift in (19.13)). For the terminal measure we would calculate 

$$
N (T _ {i}, \omega_ {k}) = \prod_ {j = i} ^ {n - 1} (1 + L _ {j} (T _ {i}, \omega_ {k}) \cdot (T _ {j + 1} - T _ {j})) ^ {- 1}.
$$

Note: The numéraire is given only at the tenor times $t = T_{i}$ , since for $t \neq T_{i}$ we did not define the short period bond $P(T_{m(t)+1}; t)$ .⁵ An interpolation is possible, see Section 19.1.5 and [90]. 

## 19.1.4. Calibration - Choice of the free Parameters

We are now going to explain how the free parameters of the model can be chosen. The free parameters are 

- the initial conditions $L_{i,0}$ , 

- the volatility functions or volatility processes $^{6}$ $\sigma_{i}$ , 

• the (instantaneous) correlation $\rho_{i,j}$ , 

$$
\begin{array}{c} i = 0, \ldots , n - 1, \\ i = 1, \ldots , n - 1, \\ i, j = 1, \ldots , n - 1. \end{array}
$$

The determination of the free parameters is also called calibration of the model. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/9d44938185028b9b8c3e2665b05ec68a53f8d4c6f5d18167dc24826760e73fa4.jpg)


Motivation (Reproduction of Market Prices versus Historical Estimation): With the LIBOR Market Model we have a high-dimensional model framework. The main task is the derivation or estimation of the huge amount of free parameters. Two approaches are possible: 

- Reproduction of Market Prices: The parameters are chosen such that the model reproduces given market prices. 

- Historical Estimation: The parameters are estimated from historical data, e.g. time series of interest rate fixings. 

$^{6}$ The parameters $\sigma_{i}$ may well be stochastic processes. In this cases $\sigma_{i}$ is called a stochastic volatility model. 

It may be surprising at first, but the second approach is not meaningful, being in the context of risk-neutral evaluation. The model is considered under the martingale measure $Q^{N}$ and its aim is the evaluation and hedging (!) of derivatives. An expectation of the relative value under the martingale measure corresponds to the relative value of the replication portfolio. This replication portfolio has to be setup from traded products, traded at current (!) market prices. If the model did not replicate current market prices, then it would not possible to buy the replication portfolio of a derivative at the model price of the derivative. The model price would inevitably be wrong. 

This remark applies to all free model parameters. In practice, however, it may be difficult or impossible to derive all parameters from market prices. This could be because for a specific product no reliable price is known (low liquidity). It could also be that a corresponding product does not exist. This is often the case for correlation sensitive products from which we would like to derive the correlation parameters. If a parameter cannot be derived from a market price a historical estimate becomes an option. If in such a case complete hedge is not possible, the residual risk has to be considered, e.g. by a conservative estimate of the parameter. 

For the LIBOR market model a parameter reduction is usually applied first, based on historical estimates of rough market assessment. An example of such parameter reduction is the assumption of a family of functional forms for the volatility $\sigma_{i}(t)$ or the correlation $\rho_{i,j}(t)$ . The remaining degrees of freedom are then derived from market prices. 

## 19.1.4.1. Choice of the Initial Conditions

Reproduction of Bond Market Prices Let $P^{\text{Market}}(T_i) \in [0, 1]$ denote a market observed (i.e. given) price of a $T_i$ -bond. If we set 

$$
L _ {i, 0} := \frac {P ^ {\mathrm{Market}} (T _ {i}) - P ^ {\mathrm{Market}} (T _ {i + 1})}{P ^ {\mathrm{Market}} (T _ {i + 1}) (T _ {i + 1} - T _ {i})},
$$

then the model reproduces the given market prices of the bonds $P^{Market}$ . This is ensured by the model having the “right” drift and it is independent of the other parameters. 

## 19.1.4.2. Choice of the Volatilities

Reproduction of Caplet Market Prices We assume here that the $\sigma_{i}$ 's are deterministic functions (i.e. not random variables or stochastic processes). The forward rate $L_{i}$ follows the Itô process 

$$
\mathrm{d} L _ {i} (t) = \mu_ {i} ^ {\mathbb {Q}} (t) L _ {i} (t) \mathrm{d} t + \sigma_ {i} (t) L _ {i} (t) \mathrm{d} W _ {i} ^ {\mathbb {Q}} (t) \quad \text { under } \mathbb {Q} := \mathbb {Q} ^ {N}.
$$

Thus the model corresponds to the Black model discussed in Chapter 10. Under $\mathbb{Q}^{P(T_{i + 1})}$ we have $\mu_i^{\mathbb{Q}^{P(T_{i + 1})}} = 0$ , the distribution of $L_{i}(T_{i})$ is lognormal and there exists an analytic evaluation formula for caplets. The only model parameters that enter the caplet price are $L_0(T_i)$ and 

$$
\sigma_ {i} ^ {\text { Black,Model }} := \left(\frac {1}{T _ {i}} \int_ {0} ^ {T _ {i}} \sigma_ {i} ^ {2} (t) \mathrm{d} t\right) ^ {1 / 2}.\tag{19.17}
$$

If the market price $V_{Caplet,i}^{Market}$ of a caplet on the forward rate $L_{i}(T_{i})$ is given, then the corresponding implied Black volatility $\sigma_{i}^{Black,Market}$ may be calculated by inverting $^{7}$ Equation (10.2). If then 

$^{7}$ For inversion of pricing formula we may use a simple numerical algorithm. For the Black formula $(10.2)$ the price is increasing strictly monotone in the volatility. 

$\sigma_{i}(t)$ is chosen such that 

$$
\sigma_ {i} ^ {\mathrm{Black,Model}} = \sigma_ {i} ^ {\mathrm{Black,Market}},\tag{19.18}
$$

then the model reproduces the given caplet price $V_{\mathrm{Caplet,i}}^{\mathrm{Market}}$ . A possible trivial choice is, e.g., $\sigma_i(t) = \sigma_i^{\mathrm{Black,Market}} \forall t$ . 

Remark 212 (Caplet Smile Modeling): The fact that the LIBOR Market Model calibrates to the cap market by a simple boundary condition is one reason for its initial popularity. However, since the model restricted to a single LIBOR is a Black model, the implied volatility does not depend on the strike of an option. Thus, in this form, the model may calibrate to a single caplet per maturity only. It cannot render a caplet smile, yet. 

For extensions of the model that try to remove this restriction see [23]. 

Reproduction of Swaption Market Prices If the correlation $R = (\rho_{i,j})$ is given and fixed, then we influence swaption prices through the time structure of the volatility function $t \mapsto \sigma_{i}$ . We consider swaptions that correspond to our tenor structure, i.e. option on the Swaprates 

$$
S (T _ {i}, \dots , T _ {j}; T _ {i}), \quad 0 <   i <   j \leq n.
$$

From the definition of the swap and swap rate it is obvious that the price of a corresponding swaption with exercise date on or before $T_{i}$ and periods $[T_{i}, T_{i+1}], \ldots, [T_{j-1}, T_{j}]$ depends only on the behavior of the forward rates $L_{i}(t), \ldots, L_{j-1}(t)$ until the fixing $t \leq T_{i}$ , see Figure 19.1. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/fdb25e0c9396c4b60ad4957a85ddd16d9030bb4d6766757449eb98e44280bd55.jpg)



Figure 19.1.: Swaption as a function of the forward rates: The swap with periods $[T_{i}, T_{i+1}], \ldots, [T_{j-1}, T_{j}]$ is a function of the forward rates $L(T_{i}, T_{i+1}; T_{i}), \ldots, L(T_{j-1}, T_{j}; T_{i})$ (all with fixing in $T_{i}$ ). The corresponding swaption depends only on the joint distribution of these forward rates. Under our model, with given initial conditions $L_{i,0}$ and correlation $R = (\rho_{i,j})$ , the swaption price depends on $\sigma_{i}(t), \ldots, \sigma_{j-1}(t), t \in [0, T_{i}]$ only. The dynamic of these forward rated beyond the $t > T_{i}$ and all other forward rates do not influence the swaption price.


If we discretize the volatility function corresponding to the tenor structure and define 

$$
\sigma_ {k, l} := \left(\frac {1}{T _ {l + 1} - T _ {l}} \int_ {T _ {l}} ^ {T _ {l + 1}} \sigma_ {k} ^ {2} (t) \mathrm{d} t\right) ^ {1 / 2},
$$

the price of an option on the swap rate $S(T_{i},\ldots,T_{j};T_{i})$ depends only on $\sigma_{k,l}$ for $k=i,\ldots,j-1$ and $l=0,\ldots,i-1$ . This allows an iterative calculation of $\sigma_{k,l}$ from given swaption market prices: 

For $i = 1,\dots ,n - 1$ 

For $j = i + 1, \dots, n$ : 

Calculate $\sigma_{j-1,i-1}$ from the price of an option on $S(T_{i},\ldots,T_{j};T_{i})$ by considering the already calculated $\sigma_{k,l}$ with $k=i,\ldots,j-1$ and $l=0,\ldots,i-2$ from the previous iterations. 

To derive $\sigma_{j-1,i-1}$ from the market price $V_{\text{swaption}}^{\text{market}}(T_i, \ldots, T_j)$ we have to invert the mapping 

$$
\sigma_ {j - 1, i - 1} \mapsto V _ {\mathrm{swaption}} ^ {\mathrm{model}} (T _ {i}, \ldots , T _ {j}).
$$

In principle this mapping may be realized by a Monte-Carlo evaluation of the swaption. To allow for faster pricing, and thus faster calibration, analytic approximation formulas for swaption prices within a LIBOR Market Model have been derived, see also Section 19.1.4.4. 

Remark 213 (Bootstrapping): The above procedure of calculating a piecewise constant instantaneous volatility from swaption prices is called volatility bootstrapping. 

Remark 214 (Review: Overfitting): The calculation of a piecewise constant volatility function $\sigma_{i,j}$ from swaption prices bears the risk of an overfitting of the model. Note that if this procedure is applied, then we accept completely the validity of every single given swaption price, i.e. that the prices are of sufficiently good quality with respect to topicality (fixing time of the price) and liquidity. If not all prices are of the same quality, then some have to be interpolated, smoothed or corrected by hand. In this case, the calibration problem has been replaced by an interpolation problem. If the interpolation and maintenance of the market data is not done with care, a calibration that fits to these prices exactly may be useless. See for example Chapter 6. 

In addition, the bootstrapping of the instantaneous volatility from swaption prices does not allow for a weighting of the swaption prices according to their importance. 

A solution to this is the reduction of the free parameters by a reduction of the family of admissible volatility functions with consequent loss of the perfect fit. 

Functional Forms To reduce the risk of overfitting, the admissible volatility functions may be restricted to a parametrized family of volatility functions. For example, a functional which is empirically motivated by the historical shapes of the volatility and which is common in practice is 

$$
\sigma_ {i} (t) := \left(a + b \cdot \left(T _ {i} - t\right)\right) \cdot \exp (- c \cdot \left(T _ {i} - t\right)) + d.
$$

Given a functional form, the calibration of the model consists of a selection of (liquid) market prices of caps and swaptions and an optimization of the remaining parameters (e.g. a, b, c, d above) to fit the model prices to the market prices. 

For a detailed discussions of a robust calibration to cap and swaption prices we refer to the literature, especially $[8, 30]$ . 

## 19.1.4.3. Choice of the Correlations

Factors We assumed in (19.1) a model in which (potentially) each forward rate $L_{i}$ Brownian motion $W_{i}$ . The model is driven by an n-dimensional $^{8}$ Brownian motion 

$$
W = \left( \begin{array}{c} W _ {0} \\ W _ {1} \\ \dots \\ W _ {n - 1} \end{array} \right).
$$

The effective number of factors, i.e. the number of independent Brownian motions, that are driving the model is determined by the correlation 

$$
\rho_ {i, j} (t) \mathrm{d} t = \mathrm{d} W _ {i} (t) \cdot \mathrm{d} W _ {j} (t).
$$

By an eigenvector decomposition (PCA) of the correlation matrix $R = (\rho_{i,j})_{i,j=1\ldots n}$ we may represent dW as 

$$
\mathrm{d} W (t) = F (t) \mathrm{d} U (t),
$$

where $U := (U_{1}, \ldots, U_{m})^{\mathrm{T}}$ and $U_{1}, \ldots, U_{m}$ denote independent Brownian motions and $F = (f_{i,j})$ denotes a $n \times m$ -matrix. In other words, we have 

$$
\mathrm{d} W _ {i} (t) = \sum_ {j = 1} ^ {m} f _ {i, j} (t) \mathrm{d} U _ {j} (t), \quad \rho_ {i, j} (t) = \sum_ {k = 1} ^ {m} f _ {i, k} (t) \cdot f _ {j, k} (t).
$$

A proof of this representation is in the Appendix A.3. Note that here we can have $m < n$ . The columns of the matrix $F$ are called factors. 

Functional Forms A full rank correlation matrix R is hard to derive from market instruments. As before a common procedure is to reduce the family of admissible correlation matrices R. One ansatz consists of functional forms, for example 

$$
\rho_ {i, j} (t) := \exp (- \alpha \cdot | i - j |).\tag{19.19}
$$

Factor Reduction The specification of the correlation matrix as a functional form is usually followed by a reduction of the number of factors. This is done in what is known as factor reduction (PCA, Principal Component Analysis). There only the eigenvectors corresponding to the largest eigenvalues of R are considered and a new correlation matrix is formed from these selected factors. For a discussion of the factor reduction see Appendix A.4. 

The advantage of the factor reduction is that afterwards only an m-dimensional Brownian motion has to be simulated (and not an n-dimensional Brownian motion). Often $n \geq 40$ is required (e.g. a 20 year interest rate curve with semi-annual periods), however often $m \leq 5$ is sufficient. The choice of the actual number m of factors depends on the application, see Chapter 24. 

$^{8}$ An n - 1-dimensional Brownian motion is sufficient here, since we can choose $W_{0} = 0$ , because the forward rate $L_{0}$ is not stochastic. It is fixed in $T_{0} = 0$ . Formally we achieve this by setting $\sigma_{0} \equiv 0$ . 

Calibration The correlation model, e.g. the free parameter a in $(19.19)$ , may be chosen such that the fit of model prices to given market prices is improved. Alternatively it may be chosen to give more realistic interest rate correlations. See also Remark 214. 

It should be stressed that we calibrate the instantaneous correlation, i.e. the correlation of the Brownian increments dW, and not the terminal correlation, i.e. the correlations of the distribution of the interest rates at a fixed time. We will consider the relation of the two in Chapter 20. 

## 19.1.4.4. Covariance Matrix, Calibration by Parameter Optimization

In the previous sections we considered volatility and correlation separately. This is not necessary, as both can be considered together in the form of the correlation matrix $(\sigma_{i}\sigma_{j}\rho_{i,j})$ . Thus the calibration problem consists of the calculation of the (market implied) covariance matrix (or covariance matrix function). 

Defining the parametrized functional forms for volatility and correlation, e.g. as 

$$
\sigma_ {i} (t) := (a + b \cdot (T _ {i} - t)) \cdot \exp (- c \cdot (T _ {i} - t)) + d, \quad \rho_ {i, j} (t) := \exp (- \alpha \cdot | i - j |)
$$

reduces the number of degrees of freedom of the covariance model and thus the possible number of products for which an exact fit is possible. This might be a desired feature, e.g. to avoid an overfitting. A disadvantage is the lack of transparency of the parameters. To derive the parameters a numerical optimization has normally to be used, e.g. the minimization of a suitable norm of the error vector of some selected product prices as a function of the model parameters. The optimization of volatility parameters and correlation parameters may occur jointly, i.e. we consider a functional form of the covariance structure. 

## 19.1.4.5. Analytic Evaluation of Caplets and Swaptions

To calculate the calibration error we need to calculate the corresponding model prices. Since a numerical calculation of the model price (e.g. by a full Monte-Carlo simulation) is time consuming, and since the optimization requires many calculation of model prices, there is a need for fast analytical pricing formulas of specific calibration products. 

Analytic Evaluation of a Caplet in the LIBOR Market Model The analytic evaluation of caplets in the LIBOR market model by the Black formula $(10.2)$ using $(19.17)$ to calculate the Black volatility. 

Analytic Evaluation of a Swaption in the LIBOR Market Model The analytic evaluation of swaption in the LIBOR market model is possible by an approximation formula only. An approximation formula can be derived by expressing the volatility of the swap rate as a function of the volatility and correlation of the forward rates. Assuming a lognormal model for the swap rate, which is already an approximation, we can then apply the Black formula for Swaptions. $^{9}$ Corresponding approximation formulas may be found in [8]. 

## 19.1.5. Interpolation of Forward Rates in the LIBOR Market Model

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/0c78f35071fe16057fa27fedcaf1dbcd6609c5cd01e160413e0fb59caa950e16.jpg)


Motivation: An implementation of the LIBOR Market Model (e.g. as Monte-Carlo simulation) allows us to calculate the forward rate $L(T_{j}, T_{k}; t_{i})$ for interest rate periods $[T_{j}, T_{k}]$ , $T_{j} < T_{k}$ and fixing times $t_{i}$ .¹⁰ Using these rates we can evaluate almost all interest rate derivatives that can be represented as a function s. 

of these rates. 

The discretization of the simulation time $\{t_{i}\}$ determines at which times we may have interest rates fixings. The discretization of the tenor structure $\{T_{j}\}$ determines for which periods forward rates are available and, since the numéraire is only defined at $t = T_{j}$ , it determines at which times we may have payment dates. The tenor structure imposes a significant restriction since a change of the tenor structure is essentially a change of the model. 

In practice, it is desired to calculate as many financial products as possible with the same model. First, the aggregation of risk measures, i.e. of sensitivities $^{11}$ of products to the sensitivity of a portfolio, is correct only if the product sensitivities have been calculated using the same model. Second, the setup of a pricing model (calibration, generation of Monte-Carlo paths) usually requires much more calculation time than the evaluation of a product, i.e., is possibly efficient to reuse a model. 

Thus, it is desirable to know how to calculate from a given LIBOR market model the quantities $L(T^{s}, T^{e}; t)$ for $T^{s}, T^{e} \notin \{T_{0}, T_{1}, \ldots, T_{n}\}$ (unaligned period) and / or $t \notin \{t_{0}, t_{1}, \ldots, t_{n}\}$ (unaligned fixing). 

## 19.1.5.1. Interpolation of the Tenor Structure $\{T_{i}\}$

Let us look at how to interpolate the tenor structure. We will derive an expression for $L(T^s, T^e; t)$ for $T^s \notin \{T_0, T_1, \ldots, T_n\}$ and/or $T^e \notin \{T_0, T_1, \ldots, T_n\}$ . Let $T^s < T^e$ . 

The forward rates $L(T^{s}, T^{e}; t)$ may be derived from corresponding bonds $P(T; t)$ . We have 

$$
1 + L (T ^ {s}, T ^ {e}; t) \cdot (T ^ {e} - T ^ {s}) = \frac {P (T ^ {s} ; t)}{P (T ^ {e} ; t)}
$$

For arbitrary T > t the bond $P(T; t)$ is given by 

$$
P (T; t) = N (t) \cdot \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {1}{N (T)} \mid \mathcal {F} _ {t}\right).
$$

The definition of the numéraire of the LIBOR Market Model shows that the specification of the short period bond $P(T_{m(t)+1}; t)$ is sufficient (and necessary) to determine all bonds $P(T; t)$ and thus all forward rates. $^{12}$ 

Assumption 1: No stochastic shortly before maturity. We assume that $P(T_{m(t)+1}; t)$ is a $F_{T_{m(t)}}$ -measurable random variable, i.e. the bond has no volatility at time t with $T_{m(t)} \leq t \leq T_{m(t)+1}$ , i.e. shortly before its maturity. With other words: $t \mapsto P(T_{m(t)+1}; t)$ is a deterministic interpolation functions on quantities known at the period start $T_{m(t)}$ . In this case for the bond with maturity $t$ , seen at time $s$ with $T_{m(t)} \leq s \leq t \leq T_{m(t)+1}$ we have: 

$$
\begin{array}{l} P (t; s) = N (s) \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {1}{N (t)} | \mathcal {F} _ {s}) \\ = N (s) \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {P (T _ {m (t) + 1} ; t)}{N (t)} \cdot \frac {1}{P (T _ {m (t) + 1} ; t)} | \mathcal {F} _ {s}) \\ = N (s) \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {P (T _ {m (t) + 1} ; t)}{N (t)} | \mathcal {F} _ {s}) \cdot \frac {1}{P (T _ {m (t) + 1} ; t)} = \frac {P (T _ {m (t) + 1} ; s)}{P (T _ {m (t) + 1} ; t)} \end{array}\tag{19.20}
$$

Especially for $s = T_{m(t)}$ 

$$
P (t; T _ {m (t)}) = \frac {P (T _ {m (t) + 1} ; T _ {m (t)})}{P (T _ {m (t) + 1} ; t)}.\tag{19.21}
$$

Thus we see that (under Assumption 1), the interpolation function $t \mapsto P(t; T_{m(t)})$ (interpolation of the maturity t) is derived directly from the interpolation function $t \mapsto P(T_{m(t)+1}; t)$ (interpolation of the evaluation time t) and vice versa. The functions are reciprocal. 

Assumption 2: Linearity shortly before maturity. If the chosen interpolation function $T \mapsto P(T; T_{m(t)})$ is linear, then the interpolation of bond prices $P(T; s)$ seen in $s < T_{m(t)}$ is linear too. This follows directly from the linearity of the expectation: 

$$
P (T; s) = N (s) \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {P (T ; T _ {m (t)})}{N (T _ {m (t)})} | \mathcal {F} _ {s}).\tag{19.22}
$$

In this way the linear interpolation takes a distinct role. With $P(T_{m(t)}; T_{m(t)}) = 1$ and $P(T_{m(t)+1}; T_{m(t)}) = \frac{1}{1 + L_{T_{m(t)}}(T_{m(t)}) \cdot (T_{m(t)+1} - T_{m(t)})}$ the linear interpolation of $t \mapsto P(t; T_{m(t)})$ follows as 

$$
\begin{array}{r l} P (t; T _ {m (t)}) = & \frac {T _ {m (t) + 1} - t}{T _ {m (t) + 1} - T _ {m (t)}} P (T _ {m (t)}; T _ {m (t)}) + \frac {t - T _ {m (t)}}{T _ {m (t) + 1} - T _ {m (t)}} P (T _ {m (t) + 1}; T _ {m (t)}) \\ = & \frac {1 + L _ {T _ {m (t)}} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t)}{1 + L _ {T _ {m (t)}} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - T _ {m (t)})}. \end{array}\tag{19.23}
$$

The corresponding interpolation for the short period bond $P(T_{m(t) + 1};t)$ thus with (19.21) 

$$
P (T _ {m (t) + 1}; t) := \frac {1}{1 + L _ {T _ {m (t)}} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t)}.
$$

Applying (19.22) to the (in $t$ ) linear interpolation (19.23) we find for all $s \leq T_{m(t)}$ 

$$
\frac {P (t ; s)}{P (T _ {m (t)} ; s)} = \frac {1 + L _ {T _ {m (t)}} (s) \cdot (T _ {m (t) + 1} - t)}{1 + L _ {T _ {m (t)}} (s) \cdot (T _ {m (t) + 1} - T _ {m (t)})},
$$

and thus 

$$
\frac {P (t ; s)}{P \left(T _ {m (t) + 1} ; s\right)} = 1 + L _ {T _ {m (t)}} (s) \cdot \left(T _ {m (t) + 1} - t\right).
$$

From (19.20) we have for $T_{m(t)} \leq s \leq t$ 

$$
P (t; s) = \frac {1 + L _ {T _ {m (t)}} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t)}{1 + L _ {T _ {m (t)}} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - s)}.
$$

We summarize this result in a theorem: 

Theorem 215 (Interpolation of Forward Rates on unaligned Periods): Given a tenor structure $T_0 < T_1 < T_2 < \ldots$ . For all $t$ let the short bond $P(T_{m(t)+1}; t)$ be given by the interpolation 

$$
P (T _ {m (t) + 1}; t) := \frac {1}{1 + L _ {T _ {m (t)}} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t)}.\tag{19.24}
$$

Then we have for arbitrary $t \leq T$ with $k = m(t), l = m(T)$ 

$$
\begin{array}{l} P (T; t) = P (T _ {k + 1}; t) \cdot \prod_ {j = k + 1} ^ {l} \frac {P (T _ {j + 1})}{P (T _ {j})} \cdot \frac {P (T ; t)}{P (T _ {l + 1} ; t)} \\ = \frac {1}{1 + L _ {k} (T _ {k}) \cdot (T _ {k + 1} - t)} \cdot \prod_ {j = k + 1} ^ {l} \frac {1}{1 + L _ {j} (t) \cdot (T _ {j + 1} - T _ {j})} \cdot (1 + L _ {l} (t ^ {*}) \cdot (T _ {l + 1} - T)), \end{array}
$$

where $t^{*} = \min(t, T_{l})$ . For $T_{s} \leq T_{e}$ with $T_{k} < T_{s} \leq T_{k+1}$ and $T_{l} \leq T_{e} < T_{l+1}$ we have 

$$
\begin{array}{l} 1 + L (T _ {s}, T _ {e}; t) \cdot (T _ {e} - T _ {s}) \\ = \frac {P (T _ {s} ; t)}{P (T _ {e} ; t)} = \frac {P (T _ {s} ; t)}{P (T _ {k + 1} ; t)} \cdot \prod_ {i = k + 1} ^ {l} \frac {P (T _ {i} ; t)}{P (T _ {i + 1} ; t)} \cdot \frac {P (T _ {l + 1} ; t)}{P (T _ {e} ; t)} \\ = (1 + L _ {k} (t ^ {*}) \cdot (T _ {k + 1} - T _ {s})) \cdot \prod_ {i = k + 1} ^ {l} (1 + L _ {i} (t) \cdot (T _ {i + 1} - T _ {i})) \cdot \frac {1}{1 + L _ {l} (t ^ {*}) \cdot (T _ {l + 1} - T _ {e})}. \end{array}\tag{19.25}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/26e4c5a354827ef94ea44ad6d74ae3bdc5d492c322232dab8d3a0f347b584ab8.jpg)


Experiment: At http://www.christian-fries.de/finmath/applets/LMMPricing.html several interest rate products can be priced using a LIBOR market model. 

## 19.2. Object Oriented Design

Figure 19.2 and 19.3 shows an object-oriented design of a Monte-Carlo LIBOR Market Model. The following important aspects are considered in the design: 

- Reuse of Implementation 

• Separation of Product and Model 

• Abstraction of Model Parameters 

• Abstraction of Calibration 

We will describe these aspects in the following. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/a254ebdc02c3f5fb56a4a75fe51468bc68ab38a763e9eb896b57b4c14f7f01b4.jpg)



Figure 19.2.: UML Diagram: Evaluation of LIBOR related products in a LIBOR Market Model via Monte-Carlo Simulation.


## 19.2.1. Reuse of Implementation

For the Monte-Carlo simulation of the lognormal process we use the same classes as in the example of the Black-Scholes model, see Figure 13.4 on Page 168. To do so the classes BROWNIANMOTION and LOGNORMALPROCESS were from the beginning designed for vector-valued, i.e. multi-factorial processes, although the Black-Scholes model does not require it. Improvements to the classes BROWNIANMOTION and LOGNORMALPROCESS will result in improvement of both applications. 

## 19.2.2. Separation of Product and Model

The interface ABSTRACTLIBORMARKETMODEL defines how LIBOR related products communicate with a Monte-Carlo LIBOR model. Through this interface the model serves to make the process of the underlyings (the forward rates) and the numéraire available to the product as a Monte-Carlo simulation. All corresponding Monte-Carlo evaluations of interest rate products expect this interface. All corresponding Monte-Carlo LIBOR models implement this interface. This realizes a separation of product and model. The specific LIBOR Market Model is realized through the class SIMPLELIBORMARKETMODEL. Model extensions may be introduced without the need to change classes that realize LIBOR related Monte-Carlo products. 

## 19.2.3. Abstraction of Model Parameters

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/c511f69c20e8f936a0e9f100984b6da0cda8cf7ddd6e195c1e76b54dc560f08f.jpg)



Figure 19.3.: UML Diagram: LIBOR Market Model: Abstraction of model parameters.


The model parameters, i.e. the covariance structure, are encapsulated in their own classes. The model parameter classes implement a simple interface LIBORCoVARIANCEModel. A specific covariance model $(i,j,t)\mapsto\gamma_{i,j}(t)=\sigma_{i}(t)\sigma_{j}(t)\rho_{i,j}(t)$ is realized through a class that implements the interface LIBORCoVARIANCEModel. This class is then served to the model. The interfaces are designed such that $(i,j,t)\mapsto\gamma_{i,j}(t)$ may be stochastic. $^{13}$ See Figure 19.3. 

This abstraction of model parameters makes it easy to exchange different modelings of covariance, i.e. volatility and correlation. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/583dc410a4c8f5b6e1f36c7091150f5247e901fcb96588dc3b341717a6045e3f.jpg)


Warning: In cases where the covariance structure is modeled by volatility and correlation it seems reasonable to define corresponding interfaces LIBOR-VOLATILITYMODEL and LIBORCORRELATIONMODEL. A simple class LIBORCOVARIANCEMODELFROMVOLATILITYANDCORRLATION calculates the factor loadings and covariances from given volatility and correlation models. See Figure 19.4. However, the separation of volatility and correlation into their own classes will bring some disadvantages for a joint calibration and general covariance modeling. The corresponding code may become over-designed. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/900d854983304e37e58bf21cd6aac76ade224d93727fecb87caadb29f1c1c550.jpg)



Figure 19.4.: UML Diagram: LIBOR Market Model: Abstraction of model parameters as volatility and correlation. Introducing separate classes for volatility and correlation has some disadvantages for joint calibration and general covariance modeling. The design above might be considered over-designed.


The design in Figure 19.4 would make sense if one whished to explore many combinations of different volatility and correlation models. 

## 19.2.4. Abstraction of Calibration

The abstraction of model parameters allows for the abstraction of calibration. The algorithm calibrating the covariance model is clearly a part of the covariance model. Thus each covariance model object can carry calibration data (e.g. market data) that, once set, is used to calibrate the model. The calibration data itself may be anything from given correlation and volatility parameters to a list of products with associated target values. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/40ca4201c3e705ee182cf2d3c091fcdf545dfbe6d3a06d2676f8b8bd635449da.jpg)



Figure 19.5.: UML Diagram: LIBOR Market Model: Abstraction of model parameters: Parametric covariance models.


## 19.3. Swap Rate Market Models (Jamshidian 1997)

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/9b458011280bdeecde829fcf395460ebd6f4d887a2311cdabcab602d11645e1d.jpg)


Motivation: The LIBOR Market Model postulates as lognormal dynamic for the forward rate $L_{i} := L(T_{i}, T_{i+1})$ . In other words, each single forward rate follows a Black model. This allows an easy calibration of the IBOR market model to Caplet prices. We only have to fulfill condition (19.18). 

If, however, swap options (i.e. swaption or swaption related products like Bermudan swaptions) are in the focus, then a model that simulates the swap rate directly might be a better choice. $^{14}$ If, for example, the swap rate follows a lognormal process, then the corresponding swaptions may be calibrated by a simple condition involving the implied Black-Volatility of the swap rate. 

Instead of a lognormal dynamic for the forward rate $L(T_{i}, T_{i+1})$ , which is the starting point of the LIBOR Market Model, we postulate here a lognormal dynamic of the swap rate 

$$
S _ {i, k} (t) := S \left(T _ {i}, T _ {k}; t\right) := \frac {P \left(T _ {i} ; t\right) - P \left(T _ {k} ; t\right)}{\sum_ {j = i} ^ {k - 1} \left(T _ {j + 1} - T _ {j}\right) \cdot P \left(T _ {j + 1} ; t\right)}, \quad k > i.\tag{19.26}
$$

Since the set of swap rates defined for a given tenor structure $T_0 < T_1 < \ldots < T_n$ is a two parametric family of $\frac{(n-1)\cdot n}{2}$ rates which are related by functional dependencies, a meaningful 

$^{14}$ Later, we will explain why a forward rate based model might be the choice even for swap rate related products, see Remark 217. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/0ab539485cb14f918eb4bf0f404e97c289c4b53d5ab14bdd7bd11673125deb77.jpg)


dynamic can be given only for a subset of swap rates. $^{15}$ 

When choosing a system of swap rates $S_{i,k}$ , for which we wish to specify the dynamics, we have to take care that the system is neither over-determined or, with respect to the given tenor structure, under-determined. The system of rates has to consist of n swap rates since on the tenor structure $0 = T_{0} < T_{1} < \ldots < T_{n}$ we have n degrees of freedom in terms of bond prices. 

Two common variants are given by the set of co-sliding swap rates and co-terminal swap rates, see Table 19.1. When specifying co-sliding swap rates it is necessary to close the system. 

$$
\text { Co - Sliding: } \quad S _ {i, \min (i + k, n)} \quad i = 0, 1, \dots , n - 1
$$

$$
\text { Co - Terminal: } \quad S _ {i, n} \quad i = 0, 2, \dots , n - 1
$$

## Table 19.1.: co-sliding and co-terminal swap rates

Our definition achieves this by first considering the swap rates $S_{i,i+k}$ with k periods (co-sliding, i < n - 1 - k) and starting with i = n - k we consider co-terminal swap rates. 

If the selection of swap rates is made, we model each $S_{i,k}$ from the selection as a lognormal process: 

$$
\mathrm{d} S _ {i, k} (t) = \mu_ {i, k} ^ {\mathbb {P}} (t) S _ {i, k} (t) \mathrm{d} t + \sigma_ {i, k} (t) S _ {i, k} (t) \mathrm{d} W _ {i, k} ^ {\mathbb {P}} (t) \quad \text { under } \mathbb {P},\tag{19.27}
$$

with initial conditions 

$$
S _ {i, k} (0) = S _ {i, k, 0}.
$$

Interpretation: The modeling of co-terminal swap rates is a suitable choice if, e.g., we have to price Bermudan swaptions, which have these swap rates as underlying. The modeling of co-sliding swap rates is a suitable choice if we have to price products relying on swap rates with constant time to maturity (CMS 

## 19.3.1. The Swap Measure

If we consider the Definition of the swap rate in (19.26), it is apparent that $S_{i,k}$ is a martingale under the martingale measure $\mathbb{Q}^N$ corresponding to the numéraire 

$$
N (t) := A \left(T _ {i}, \dots , T _ {k}; t\right) := \sum_ {j = i} ^ {k - 1} \left(T _ {j + 1} - T _ {j}\right) \cdot P \left(T _ {j + 1}; t\right), \quad k > i, t \leq T _ {i + 1}.\tag{19.28}
$$

The right hand side in $(19.28)$ is a portfolio of zero bonds and thus a traded product and the swap rate is the N-relative price of a traded product. 

## Definition 216 (Swap Measure, Swap Annuity):

The equivalent martingale measure $\mathbb{Q}^N$ corresponding to the numéraire $N$ in (19.28) is called swap measure corresponding to the swap rate $S(T_1, \ldots, T_k)$ . The expression on the right hand side in (19.28) is also called swap annuity. 

The numéraire is, so far, defined for $t \leq T_{i+1}$ only, since at $t = T_{i+1}$ the first bond $P(T_{i+1})$ is at its maturity and we have to specify how its payment has to be reinvested. $^{17}$ A continuation of the numéraire definition to $t > T_{i+1}$ can be given by a re-investment into the next swap annuity. This is the analog to the numéraire (19.9) of the Spot Measures. For $i = 1, \ldots, k - 1$ we have 

$$
N (t) = A \left(T _ {i}, \dots , T _ {k}; t\right) \cdot \prod_ {j = 1} ^ {i - 1} \frac {A \left(T _ {j} , \dots , T _ {k} ; T _ {j + 1}\right)}{A \left(T _ {j + 1} , \dots , T _ {k} ; T _ {j + 1}\right)}, \quad T _ {i - 1} \leq t <   T _ {i}
$$

where $T_{0} := 0$ . The swap rates we are considering here are co-terminal. Of course we may consider co-sliding swaps in a similar way, using the swap annuities $A(T_{j}, \ldots, T_{j+k}; t)$ . The corresponding numéraire of re-investment in co-sliding swap annuities, i.e. a rolling co-sliding swap annuity then is 

$$
N (t) = A \left(T _ {i}, \dots , T _ {i + k}; t\right) \cdot \prod_ {j = 1} ^ {i - 1} \frac {A \left(T _ {j} , \dots , T _ {j + k} ; T _ {j + 1}\right)}{A \left(T _ {j + 1} , \dots , T _ {j + 1 + k} ; T _ {j + 1}\right)}, \quad T _ {i - 1} \leq t <   T _ {i}.
$$

For $k = i + 1$ this corresponds to (19.9). 

## 19.3.2. Derivation of the Drift Term

For the swap rate market model we have multiple sets of swap rates, which may be modeled and (as in the LIBOR Market Model) multiple possible choices of numéraires. This section does not give a detailed derivation of the drift terms. The derivation is done similarly to the derivation of the drift in the LIBOR Market Model by expressing a martingale through the elementary swap rate processes $S_{i,j}$ . If for example $A_{k,l}$ is the numéraire, we consider the $Q^{A_{k,l}}$ -martingale $(S_{i,j} \cdot \frac{A_{i,j}}{A_{k,l}})$ . 

## 19.3.3. Calibration - Choice of the free Parameters

## 19.3.3.1. Choice of the Initial Conditions

Reproduction of Bond Market Prices or Swap Market Prices If we set t to the preset time in the definition of the swap rate $(19.26)$ , i.e. t = 0 following our convention, then we get an equation relating today's bond prices to today's swap rates $S_{i,k}(0)$ and the latter are just the initial conditions of the chosen swap rate processes. Thus the initial conditions of the processes are given by $(19.26)$ with t = 0 and today's bond prices, i.e. today's interest rate curve. 

Although we regard the family of zero bonds as the natural description of the interest rate curve and we see swap rates and swap prices as derived quantities, it is in this case natural to calculate today's swap rates directly from today's swap prices (assuming they are given). In this case the initial conditions are given by today's swap prices. With this choice, the model will reproduce these prices. 

## 19.3.3.2. Choice of the Volatilities

Reproduction of Swaption Market Prices The calibration of the model to swaption prices is analog to the calibration of the LIBOR Market Model to caplet prices. Let the dynamic of the swap rate $S_{i,k}$ be given by (19.27). Furthermore let $\sigma_{i,k}^{Black,Market}$ denote the market prices of an option on $S_{i,k}$ given as implied Black-volatility. If we calculate 

$$
\sigma_ {i, k} ^ {\text { Black,Model }} := \left(\frac {1}{T _ {i}} \int_ {0} ^ {T _ {i}} \sigma_ {i, k} ^ {2} (t) \mathrm{d} t\right) ^ {1 / 2},
$$

then the model reproduces the given swaption market prices if 

$$
\sigma_ {i, k} ^ {\text { Black,Model }} = \sigma_ {i, k} ^ {\text { Black,Market }}.
$$

This statement is trivial since, if we consider only a single swap rate $S_{i,k}$ , then (19.27) is a Black model for this swap rate and under this model the implied volatility is defined by inverting the pricing formula. The inversion of the pricing formula is what a calibration should achieve. 

Remark 217 (LIBOR Market Model versus Swaprate Market Model): The question of whether one should choose a LIBOR Market Model or a Swaprate Market Model seems to depend on the application only, to be precise, on whether the model should calibrate to caplets or swaptions - and whether or not one sees a lognormal forward rate or a lognormal swap rate as realistic model. $^{18}$ 

Therefore, the criterion that defines the choice of the model thus is the quality of the model calibration to the specific application. 

However, the swap rate market model has a disadvantage compared to the LIBOR market model: If we calculate a forward rate $L_{i}$ in a swap rate market model, then the forward rate tends to suffer from numerical instabilities. Conversely the calculation of a swap rate from forward rates models in a LIBOR Market Model is generally much more stable. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/d4ea3af1d2df873f2eb9cd3de77b88bf8e1897b67427fc17f1ca6cdd7a30216a.jpg)


Interpretation: The reason lies in the representation of the swap rate as a convex combination of the forward rates. From Lemma 123 we have 

$$
S _ {i, j} = \sum_ {k = i} ^ {j - 1} \alpha_ {k} ^ {i, j} L _ {k}, \quad \text { with } \quad \alpha_ {k} ^ {i, j} \geq 0 \quad \text { and } \quad \sum_ {k = i} ^ {j - 1} \alpha_ {k} ^ {i, j} = 1,
$$

with $\alpha_{k}^{i,j} := \frac{P(T_{k+1}) \cdot (T_{k+1} - T_k)}{\sum_{k=i}^{j-1} P(T_{k+1}) \cdot (T_{k+1} - T_k)}$ . 

If we calculate a forward rate $L_{i}$ froms (e.g. co-terminal) swap rates $S_{j,n}$ we have 

$$
\begin{array}{c} L _ {i} = \frac {1}{\alpha_ {i} ^ {i , n}} S _ {i, n} - \frac {1}{\alpha_ {i} ^ {i + 1 , n}} S _ {i + 1, n + 1} \\ = \frac {1}{\alpha_ {i} ^ {i , n}} (S _ {i, n} - S _ {i + 1, n}) + (\frac {1}{\alpha_ {i} ^ {i , n}} - \frac {1}{\alpha_ {i} ^ {i + 1 , n}}) S _ {i + 1, n}. \end{array}
$$

$^{18}$ In general both assumptions cannot hold and it is necessary to modify the models with respect to their distribution assumption. Such a modification of the model is called smile modeling. 

Assuming for simplicity $\alpha_{j}^{i,n}=\frac{1}{n-i-1}$ , which is with $\sum_{j=i}^{n-1}\alpha_{j}^{i,n}=1$ plausible $^{19}$ , then we have 

$$
\begin{array}{c} S _ {i, n} = \frac {1}{n - i - 1} \sum_ {k = i} ^ {n - 1} L _ {k} \\ L _ {i} = (n - i - 1) \cdot (S _ {i, n} - S _ {i + 1, n}) + S _ {i + 1, n}. \end{array}
$$

This shows: 

- The calculation of a swap rate $S_{i,n}$ from forward rates $L_{k}$ corresponds to the calculation of an average (rate) - the swap rate can be interpreted as an integral of the forward rates. Errors in $L_{k}$ are averaged and thus smoothed. The variance of an unsystematic error is reduced. 

- The calculation of a forward rate $L_{i}$ from swap rates $S_{i,n}$ , $S_{i+1,n}$ consists of a finite difference term - this part of the forward rate may be interpreted as a derivative. The calculation of a difference is very sensitive to errors in the swap rates (e.g. small jumps) and the error is scaled up by the factor $(n-i-1)$ for n large and i small. Thus forward rates for short periods in a model of long period swap rates have a tendency to numerical instability. 

< 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/19435704c25b0d17ceb70c6ada8ce641d81d762cd7c5338017c63f23e39b8388.jpg)


Tip: If there is no strong reason for a swap rate market model, a generic LIBOR Market Model with calculation of the corresponding swap rates from forward rates is preferable. This provides a single, thus consistent model for multiple applications (products), which allows the aggregation of risk parameters (Delta, 

Gamma). The difference in the distributional properties is often negligible (see [8]). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/25145cfe71542e49e777cda79b7ef3cc9c4b67deab053533a6cb5a368c20b4d7.jpg)


Further Reading: The original articles on the LIBOR market model are [50] and [84]; for the swap rate market model see [77]; for the calibration of the LIBOR Market Model see [8, 30]; for the arbitrage-free discretization see [69]; for the interpolation of forward rates see [90]. The evaluation of Bermudan options Carlo is considered in Chapter 15; see also [44, 45]. 

in Monte-Carlo is considered in Chapter 15; see also [44, 45]. 

We will use the LIBOR Market model as foundation for further investigations into general interest rate model properties. In Chapter 20 we will investigate the instantaneous correlation $\rho_{i,j}$ and volatility $\sigma_{i}$ and their effect on terminal correlation. In Chapter 24 we will investigate the mean reversion and multi-factoriality on the shape of interest rate curve. 

# Excursus: Instantaneous Correlation and Terminal Correlation

In this chapter we will use the LIBOR Market Model to discuss the influence of instantaneous volatility and instantaneous correlation on option prices. Although our study is based on the LIBOR market model, the intuition gained from our experiments is universally valid. 

We will experiment with different (extreme) parameter configurations and we will see how a single-factor model, in which all interest rates $L(T_{i}, T_{i+1})$ move (instantaneously) perfectly correlated may, however, exhibit at time t > 0 (terminal) perfectly de-correlated random variables $L(T_{j}, T_{j+1}; t)$ , $L(T_{k}, T_{k+1}; t)$ . 

We will start by repeating some basic concepts: 

## 20.1. Definitions

Definition 218 (Covariance, Correlation): 

Let X, Y denote two (numeric) random variables, $\bar{X} = \mathrm{E}(X)$ , $\bar{Y} = \mathrm{E}(Y)$ . Then 

$$
\operatorname{Cov} (X, Y) := \operatorname{E} ((X - \bar {X}) \cdot (Y - \bar {Y}))
$$

is called the covariance of X and Y, $\operatorname{Var}(X) := \operatorname{Cov}(X, X)$ is called the variance of X and 

$$
\operatorname{Cor} (X, Y) := \frac {\operatorname{E} ((X - \bar {X}) \cdot (Y - \bar {Y}))}{\sqrt {\operatorname{Var} (X)} \cdot \sqrt {\operatorname{Var} (Y)}}
$$

is called the correlation of X and Y. 

Let $L = (L_{1}, \ldots, L_{n})$ denote an $n$ -dimensional $m$ -factorial Itô-process of the form 

$$
\mathrm{d} L _ {i} = \mu_ {i} \mathrm{d} t + \sigma_ {i} \mathrm{d} W _ {i}, \quad \text { where } \quad \mathrm{d} W _ {i} = \sum_ {k = 1} ^ {m} f _ {i, k} \mathrm{d} U _ {k}\tag{20.1}
$$

and $U_{k}$ denote independent Brownian motions. Furthermore, let $f_{i,k}$ such that 

$$
R := \left(\rho_ {i, j} (t)\right) _ {i, j = 1, \dots , n} = \left(\sum_ {k = 1} ^ {m} f _ {i, k} f _ {j, k}\right) _ {i, j = 1, \dots , n}
$$

is a correlation matrix (i.e. $\sum_{k=1}^{m} f_{i,k}^2 = 1$ ). We have 

$$
<   \mathrm{d} W (t), \mathrm{d} W (t) > = R \mathrm{d} t.
$$

Definition 219 (Instantaneous Covariance, Instantaneous Correlation): With the notation above we call 

$$
\rho_ {i, j}, \quad \text { defined   by } \quad \rho_ {i, j} (t) := \left(\sum_ {k = 1} ^ {m} f _ {i, k} f _ {j, k}\right) _ {i, j = 1, \dots , n},
$$

the instantaneous correlation of the processes $L_{i}$ and $L_{j}$ , and we call $\sigma_{i}\sigma_{j}\rho_{i,j}$ the instantaneous covariance of the processes $L_{i}$ and $L_{j}$ . 

With the notation above we call 

$$
\rho_ {i, j} ^ {\text { Term }}, \quad \text { defined   by } \quad \rho_ {i, j} ^ {\text { Term }} (t) := \text { Cor } (L _ {i} (t), L _ {j} (t)),
$$

the terminal correlation of the processes $L_{i}$ and $L_{j}$ . Correspondingly we call $t \mapsto \operatorname{Cov}(L_i(t), L_j(t))$ the terminal covariance of the processes $L_{i}$ and $L_{j}$ . 

## 20.2. Terminal Correlation examined in a LIBOR Market Model Example

We are considering a LIBOR Market Model with semi-annual tenor structure $T_{i} := 0.5 \cdot i$ and investigating the behaviour of the two rates $L_{10} = L(5.0, 5.5)$ and $L_{11} = L(5.5, 6.0)$ . Under the numéraire $N = P(T_{12}) = P(6.0)$ we have for the dynamic of these rates (see (19.3), (19.8)) 

$$
\begin{array}{l l} \mathrm{d} L _ {i} (t) = \mu_ {i} (t) L _ {i} (t) \mathrm{d} t + \sigma_ {i} (t) L _ {i} (t) \mathrm{d} W _ {i} ^ {\mathbb {Q} ^ {N}} (t) & (i = 1 0, 1 1) \\ \mu_ {1 0} = - \frac {\delta_ {1 1} L _ {1 1} (t)}{(1 + \delta_ {1 1} L _ {1 1} (t))} \cdot \sigma_ {1 0} (t) \cdot \sigma_ {1 1} (t) \cdot \rho_ {1 0, 1 1} (t), & \delta_ {1 1} := T _ {1 1} - T _ {1 0} \\ \mu_ {1 1} = 0. \end{array}\tag{20.2}
$$

If we neglect the drift (i.e. set $\mu_{10} = 0$ ) and assume a constant instantaneous covariance $\sigma_{10}\sigma_{11}\rho_{10,11} = const.$ , then it follows from (20.1) that the terminal correlation is 

$$
\rho_ {i, j} ^ {\mathrm{Term}} (t) = \rho_ {1 0, 1 1} \quad \forall t.
$$

As one might have expected, the terminal correlation is given by the choice of the instantaneous correlation. In this case, to achieve a terminal correlation different from zero we need at least a two-factor model. Figure 20.1 shows a scatter plot for a one-factor and a five-factor model $^{1}$ of the interest rates $L_{10}(t)$ , $L_{11}(t)$ at time $t = T_{10} = 5.0$ . 

$^{1}$ The exact model specification is: $L_{i,0} = 0.1$ , $\sigma_{i} = 0.1$ , and $\rho_{i,j} = \exp(-0.5|i - j|)$ , followed by a factor reduction as given in Section A.4. For the five-factor model we have $\rho_{10,11} = 0.94$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/b7b93a24947c2a0ae79e5f54c7900542cf959313ec3cf066dbcf60bdd1405f5b.jpg)



Figure 20.1.: The two (adjacent) rates $L_{10} = L(5.0, 5.5)$ and $L_{11} = L(5.5, 6.0)$ in a one- and a multifactor model for constant instantaneous volatility $\sigma_{10}(t) = \sigma_{11}(t) = \text{const}$ . In a one-factor model both random variables are perfectly correlated (left). In a five-factor model both random variables show a correlation different from 1. This is a consequence of the instantaneous correlation $\rho_{10,11}$ being different from 1.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/0d39504d547e0a6cce3f5b479920ac0a1524b1fa2547008a959dfda069670348.jpg)



Figure 20.2.: The two (adjacent) rates $L_{10} = L(5.0, 5.5)$ and $L_{11} = L(5.5, 6.0)$ in a one-factor model. Left: The two random variables exhibit a correlation close to 0 (perfect de-correlation). Right: The two random variables exhibit a very different variances. The covariance is close to zero since the variance of $L_{11}$ is close to 0. Both scenarios are the consequence of a very special choice for the instantaneous volatility.


## 20.2.1. De-correlation in a One-Factor Model

It is possible to achieve a terminal de-correlation for processes which have perfect instantaneous correlation. Consider 

$$
\sigma_ {1 0} (t) \left\{ \begin{array}{l l} > 0 & \text { for } t <   2. 5, \\ = 0 & \text { for } t \geq 2. 5, \end{array} \right. \quad \sigma_ {1 1} (t) \left\{ \begin{array}{l l} = 0 & \text { for } t <   2. 5, \\ > 0 & \text { for } t \geq 2. 5, \end{array} \right.\tag{20.3}
$$

i.e. the processes receive the Brownian increment $\mathrm{d}W(t)$ at different times t, thus the increments received are independent. Since in this case we have $\mu_{10} = \mu_{11} = 0$ in (20.2), the two random variables $L_{10}(5.0)$ , $L_{11}(5.0)$ are given by 

$$
\begin{array}{l} \log (L _ {1 0}) (5. 0) = - \frac {1}{2} \bar {\sigma} _ {1 0} ^ {2} \cdot 2. 5 + \bar {\sigma} _ {1 0} (W _ {1 0} (2. 5) - W _ {1 0} (0)) \\ \log (L _ {1 1}) (5. 0) = - \frac {1}{2} \bar {\sigma} _ {1 1} ^ {2} \cdot 2. 5 + \bar {\sigma} _ {1 1} (W _ {1 1} (5. 0) - W _ {1 1} (2. 5)), \end{array}
$$

where $\bar{\sigma}_{10}^{2}=\frac{1}{2.5}\int_{0}^{2.5}\sigma_{10}^{2}(t)\,\mathrm{d}t$ and $\bar{\sigma}_{11}^{2}=\frac{1}{2.5}\int_{2.5}^{5.0}\sigma_{11}^{2}(t)\,\mathrm{d}t$ . 

Since, even for a one-factor model, the increments $(W(2.5) - W(0))$ , $(W(5) - W(2.5))$ are independent, $L_{10}(5.0)$ , $L_{11}(5.0)$ are independent as well, see Figure 20.2, left. 

## 20.2.2. Impact of the Time Structure of the Instantaneous Volatility on Caplet and Swaption Prices

The previous example of the de-correlation of the rates $L_{10}$ , $L_{11}$ in a one-factor model shows the importance of the time structure of the instantaneous volatility for the (terminal) distribution of $(L_{10}, L_{11})$ at time t = 5.0. Now we will look at the corresponding caplets and a swaption with maturity 5.0 and payment dates 5.5, 6.0, which is dependent on $L_{10}$ and $L_{11}$ : 

<table><tr><td>Scenario</td><td><eq>\sigma_{i}(t)</eq></td><td><eq>\rho_{10,11}</eq></td><td>Caplet5.0-5.5</td><td>Caplet5.5-6.0</td><td>Swaption5.0-6.0</td></tr><tr><td>1</td><td>0.1</td><td>1.0</td><td>0.26%</td><td>0.26%</td><td>0.51%</td></tr><tr><td>2</td><td>0.1</td><td>0.94</td><td>0.26%</td><td>0.26%</td><td>0.50%</td></tr><tr><td>3</td><td>as in (20.3)</td><td>1.0</td><td>0.26%</td><td>0.26%</td><td>0.36%</td></tr><tr><td>4</td><td><eq>0.7\exp(4.9(T_{i}-t))</eq></td><td>1.0</td><td>0.26%</td><td>0.26%</td><td>0.27%</td></tr></table>


Table 20.1.: Caplet and swaption prices for different instantaneous correlations and volatilities.


In all scenarios we have $\int_{0}^{T_{i}}\sigma_{i}(t)^{2}\,\mathrm{d}t=0.05$ for i=10, thus all caplet prices are the same. $^{2}$ The Figures 20.1, 20.2 are generated with these parameters. 

## 20.2.3. The Swaption Value as a Function of Forward Rates

To interpret these results we analyze the dependency of the swaption value from the rates $L_{10}$ , $L_{11}$ . 

$^{2}$ We have $\int_{0}^{T_{i}}\left(b\cdot\exp(-c\cdot(T_{i}-t))\right)^{2}\mathrm{d}t=\frac{b^{2}}{2c}(1-\exp(-2\cdot c\cdot T_{i}))$ . For $T_{i}=5.0$ , b=0.7, c=4.9 we thus have $\int_{0}^{T_{i}}\sigma_{i}(t)^{2}\mathrm{d}t=0.05(1-\exp(-49))=0.05(1-5\cdot10^{-22})$ . 

For the value of a swaption $V_{\text{Swaption}}(T_0)$ with fixed swap rate (strike) K we have 

$$
V _ {\text { Swaption }} (T _ {0}) = N (0) \mathrm{E} ^ {\mathbb {Q} ^ {N}} \left(\frac {\max (S (T _ {i}) - K , 0) \cdot A (T _ {i})}{N (T _ {i})} \mid \mathcal {F} _ {T _ {0}}\right)
$$

with 

$$
\begin{array}{l l} A (T _ {i}) = \sum_ {j = i} ^ {n - 1} (T _ {j + 1} - T _ {j}) P (T _ {j + 1}; T _ {i}) & \text {(swap annuity)} \\ S (T _ {i}) = \frac {1 - P (T _ {n} ; T _ {i})}{A (T _ {i})} & \text {(par swap rate)}. \end{array}
$$

With the numéraire $N = P(T_{n})$ we have 

$$
\begin{array}{c} \frac {A (T _ {i})}{N (T _ {i})} = \frac {A (T _ {i})}{P (T _ {n} ; T _ {i})} = \sum_ {j = i} ^ {n - 1} (T _ {j + 1} - T _ {j}) \frac {P (T _ {j + 1} ; T _ {i})}{P (T _ {n} ; T _ {i})} \\ = \sum_ {j = i} ^ {n - 1} (T _ {j + 1} - T _ {j}) \prod_ {k = j + 1} ^ {n - 1} (1 + L _ {k} (T _ {i}) (T _ {k + 1} - T _ {k})) \end{array}
$$

and 

$$
S (T _ {i}) \frac {A (T _ {i})}{N (T _ {i})} = \frac {1 - P (T _ {n} ; T _ {i})}{P (T _ {n} ; T _ {i})} = \prod_ {j = i} ^ {n - 1} (1 + L _ {j} (T _ {i}) (T _ {j + 1} - T _ {j})) - 1,
$$

i.e. it is 

$$
V _ {\text { Swaption }} (T _ {0}) = P (T _ {n}; T _ {0}) \mathrm{E} ^ {\mathbb {Q} ^ {P (T _ {n})}} (\max (\frac {(S (T _ {i}) - K) \cdot A (T _ {i})}{P (T _ {n} ; T _ {i})}, 0) \mid \mathcal {F} _ {T _ {0}})
$$

with 

$$
\begin{array}{c} \frac {(S (T _ {i}) - K) \cdot A (T _ {i})}{P (T _ {n} ; T _ {i})} = \prod_ {j = i} ^ {n - 1} (1 + L _ {j} (T _ {i}) (T _ {j + 1} - T _ {j})) - 1 - \\ K \cdot \sum_ {j = i} ^ {n - 1} (T _ {j + 1} - T _ {j}) \prod_ {k = j + 1} ^ {n - 1} (1 + L _ {k} (T _ {i}) (T _ {k + 1} - T _ {k})). \end{array}
$$

If we apply this to the special case of a swaption with a two period tenor $\{T_i,\ldots ,T_n\} = \{T_{10},T_{11},T_{12}\} = \{5.0,5.5,6.0\}$ we get 

$$
\begin{array}{l} \max (\frac {S (T _ {i}) - K \cdot A (T _ {i})}{P (T _ {n} ; T _ {i})}, 0) \\ = \max ((1 + L _ {1 0} \Delta T) (1 + L _ {1 1} \Delta T) - K (\Delta T (1 + L _ {1 1} \Delta T) + \Delta T), 0) \\ = \max ((L _ {1 0} - K) \Delta T + (L _ {1 1} - K) \Delta T + L _ {1 1} (L _ {1 0} - K) (\Delta T) ^ {2}), 0). \end{array}\tag{20.4}
$$

From (20.4) we can derive the following observations for the value of the swaption: 

- If $L_{11}(T_{10}) = K$ , then the value of the swaption corresponds to the value of a caplet paying $\max(L_{10} - K, 0)$ . If $L_{11}$ has at time $T_{10}$ no or small variance and if $L_{11}(T_{10})$ is close to $K$ , then the value of the swaption is close to the value of a caplet with payoff $\max(L_{10} - K, 0)$ . 

- Neglecting the term $L_{11}(T_{10})(L_{10}(T_{10}) - K)(\Delta T)^{2}$ , which is justified for small rates and short periods $\Delta T$ , and considering thus only 

$$
(L _ {1 0} (T _ {1 0}) - K) \Delta T + (L _ {1 1} (T _ {1 0}) - K) \Delta T
$$

$$
= (L _ {1 0} (T _ {1 0}) + L _ {1 1} (T _ {1 0}) - 2 K) \Delta T,
$$

we see that the option price is determined by the variance of $L_{10}(T_{10}) + L_{11}(T_{10})$ . For this we have 

$$
\begin{array}{l} \operatorname{Var} (L _ {1 0} (T _ {1 0}) + L _ {1 1} (T _ {1 0})) \\ = \operatorname{Var} (L _ {1 0} (T _ {1 0})) + \operatorname{Var} (L _ {1 1} (T _ {1 0})) + 2 \cdot \operatorname{Cov} (L _ {1 0} (T _ {1 0}), L _ {1 1} (T _ {1 0})) \end{array}
$$

- From the previous we know that the option value is maximal for $\rho_{10,11}^{\mathrm{Term}}(T_{10}) = 1$ and minimal (even 0) for $\rho_{10,11}^{\mathrm{Term}}(T_{10}) = -1$ (still neglecting the term $L_{11}(T_{10})(L_{10}(T_{10}) - K)\Delta T^2$ ). 

From these remarks the results in table 20.1 become plausible. In Scenario 4 the rate $L_{11}(T_{10})$ has a negligible small variance (compare Figure 20.2, right). The swaption value is close to the caplet value. The caplet on the period $[T_{11}, T_{12}]$ however has the same price as in the other scenarios, since the high instantaneous volatility for $t \in [T_{10}, T_{11}]$ will give the rate $L_{11}(T_{11})$ the required (terminal) variance. 

While for the swaption the rate $L_{11}(T_{10})$ is relevant, for the caplet it is the rate $L_{11}(T_{10})$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/7eecfe6e94e3e487d8a5181706755fbcf84758ab33ec2325ceb3083c753503e4.jpg)


Experiment: The influence of the instantaneous volatility and instantaneous correlation on terminal correlation, caplet and swaption prices may be investigated at 

http://www.christian-fries.de/finmath/applets/LMMCorrelation.html. 

< 

## 20.3. Terminal Correlation is dependent on the Equivalent Martingale Measure

The terminal correlation is dependent on the martingale measure and thus the numéraire used. The whole (terminal) probability density is of course measure dependent, see also Lemma 81 in Chapter 5. Thus an interpretation of terminal correlation and other terminal quantities should be made with caution. 

How the chosen martingale measure influences the terminal distribution, especially the terminal correlation, may easily be seen in a LIBOR Market Model. Consider the processes $L_{i} = L(T_{i}, T_{i+1})$ and $L_{i+1} = L(T_{i+1}, T_{i+2})$ , i.e. two adjacent forward rates, under the martingale measure $\mathbb{Q}^{P(T_{n})}$ corresponding to the numéraire $P(T_{n})$ (terminal measure). It is 

$$
\mathrm{d} \log (L _ {i}) = - \sum_ {i <   j <   n} \frac {\delta_ {j} L _ {j} (t)}{(1 + \delta_ {j} L _ {j} (t))} \cdot \sigma_ {i} (t) \sigma_ {j} (t) \rho_ {i, j} (t) \mathrm{d} t + \frac {1}{2} \sigma_ {i} (t) ^ {2} \mathrm{d} t + \sigma_ {i} (t) \mathrm{d} W _ {i} ^ {\mathbb {Q} ^ {P (T _ {n})}}.
$$

With $\mathrm{d}K_{j}(t):=\frac{\delta_{j}L_{j}(t)}{(1+\delta_{j}L_{j}(t))}\mathrm{d}t$ we thus have 

$$
\begin{array}{c} \mathrm{d} \log (L _ {i}) = \sigma_ {i} \cdot \Big (- \sigma_ {i + 1} \rho_ {i, i + 1} \mathrm{d} K _ {i + 1}   - \sum_ {i + 1 <   j <   n} \sigma_ {j} \rho_ {i + 1, j} \mathrm{d} K _ {j}   + \frac {1}{2} \sigma_ {i} (t) \mathrm{d} t + \mathrm{d} W _ {i} ^ {\mathbb {Q} ^ {P (T _ {n})}} \Big) \\ \mathrm{d} \log (L _ {i + 1}) = \sigma_ {i + 1} \cdot \Big (\\ \hline - \sum_ {i + 1 <   j <   n} \sigma_ {j} \rho_ {i + 1, j} \mathrm{d} K _ {j}   + \frac {1}{2} \sigma_ {i + 1} \mathrm{d} t + \mathrm{d} W _ {i + 1} ^ {\mathbb {Q} ^ {P (T _ {n})}} \Big). \end{array}
$$

The terminal correlation is influenced by the common drift term $\sum_{i+1<j<n} dK_j$ and this influence can be increased arbitrarily through the factor $\sigma_j$ in front of $K_j$ . If and how this term is present depends on the chosen martingale measure: For $n = i + 2$ the sum is empty and the term is = 0, for $n > i + 2$ the term is > 0. In theory it might be possible that $L_i$ and $L_{i+1}$ appear almost perfectly correlated under $\mathbb{Q}^{P(T_{i+3})}$ and perfectly uncorrelated under $\mathbb{Q}^{P(T_{i+2})}$ . 

## 20.3.1. Dependence of the Terminal Density on the Martingale Measure

How the chosen martingale measure influences the terminal distribution function is shown in the following examples. In Figure 20.3 we look at the density of a forward rate under a one-factor LIBOR Market model with constant instantaneous volatility, equal for all rates. Under different martingale measures (spot measure, terminal measure) the distribution is slightly different. If, however, the volatility of the other rates is increased, then, depending on the chosen martingale measure, the distribution will change, see Figure 20.4. As before, the change in the distribution function stems from the drift of the LIBOR Market Model. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/b9aa27f93fb262dd8ff0b9876e27f8ce16e859ebd3b453a3eac7f82dc92b0aba.jpg)



Figure 20.3.: The terminal distribution function of a forward rate under different martingale measures. Shown is the rate $L(5.0, 5.5)$ upon its fixing at $t = 5.0$ . All rates are simulated in a one-factor LIBOR market model with constant instantaneous volatility $\sigma = 10\%$ .


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/487b26c11dc220ae29f52ad4df951898c5cf2d744acbf5b84ad40fa00d0950dd.jpg)



Figure 20.4.: The terminal distribution function of a forward rate under different martingale measures. Shown is the rate $L(5.0, 5.5)$ upon its at fixing $t = 5.0$ . In contrast to Figure 20.3 the rates $L(T_i, T_{i+1})$ for $T_i < 5.0$ are simulated differently. They are simulated with a high volatility of $150\%$ . All other rates are simulated as in Figure 20.3 with volatility $\sigma = 10\%$ . The change of the simulation of the other rates has an significant impact on the distribution of $L(5.0, 5.5)$ under the spot measure.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/e150bf6b0e2a74875d28977230d572638fffced035a51800530b745688a8197e.jpg)


Tip (Terminal Quantities Independent of the Martingale Measure): In place of martingale measure dependent quantities, like the terminal distribution of the terminal correlation, we can define meaningful alternatives. The implied (Black-)volatility is an example of a martingale measure independent quantity. 

Apart from the scaling with the square root of the maturity $\sqrt{T_{k}}$ it corresponds to the terminal standard deviation under the $T_{k+1}$ -forward measure. If, for example, 

$$
\begin{array}{l} \mathrm{d} \log (L _ {i} (t)) = (\ldots) \mathrm{d} t + \sigma_ {i} (t) \mathrm{d} W _ {i} (t) \\ \mathrm{d} \log (L _ {j} (t)) = (\ldots) \mathrm{d} t + \sigma_ {j} (t) \mathrm{d} W _ {j} (t) \end{array}
$$

are given processes, then the integrated instantaneous covariance 

$$
\int_ {0} ^ {T} \mathrm{d} \log (L _ {i} (t)) \mathrm{d} \log (L _ {j} (t)) = \int_ {0} ^ {T} \sigma_ {i} (t) \sigma j (t) \rho_ {i, j} (t) \mathrm{d} t
$$

is independent of the chosen martingale measure. $^{3}$ It would correspond to the covariance of $\log(L_{i}(t))$ and $\log(L_{j}(t))$ , if both were martingales. 

# Heath-Jarrow-Morton Framework: Foundations

The Heath-Jarrow-Morton Framework [74] postulates an Itô process as a model for the instantaneous forward rate $^{1}$ : 

$$
\begin{array}{l} \mathrm{d} f (t, T) = \alpha^ {\mathbb {P}} (t, T) \mathrm{d} t + \sigma (t, T) \cdot \mathrm{d} W ^ {\mathbb {P}} (t) \\ f (0, T) = f _ {0} (T) \end{array}\tag{21.1}
$$

for $0 \leq t < T$ , where $W^{P} = (W_{1}^{P}, \ldots, W_{m}^{P})$ is an m-dimensional P-Brownian motion with instantaneously uncorrelated components. $^{2}$ Furthermore we assume that $\sigma(t, T) = (\sigma_{1}(t, T), \ldots, \sigma_{m}(t, T))$ and $\alpha^{P}(t, T)$ are adapted processes. 

In case of its existence, let Q denote the risk-neutral measure, i.e. the martingale measure $Q = Q^{B}$ corresponding to the numéraire B with 

$$
B (t) := \exp \Big (\int_ {0} ^ {t} f (\tau , \tau) \mathrm{d} \tau \Big) = \exp \Big (\int_ {0} ^ {t} r (\tau) \mathrm{d} \tau \Big),\tag{21.2}
$$

where $r$ denotes the short rate - see Definition 103. 

Girsanov's Theorem (Theorem 58), gives the process (21.1) under $\mathbb{Q}$ as 

$$
\begin{array}{l} \mathrm{d} f (t, T) = \alpha^ {\mathbb {Q}} (t, T) \mathrm{d} t + \sigma (t, T) \cdot \mathrm{d} W ^ {\mathbb {Q}} (t) \\ f (0, T) = f _ {0} (T). \end{array}\tag{21.3}
$$

Equation (21.3) represents a family of stochastic processes parametrized by $T$ , which give a complete description of the interest rate curve: From Definition (101) we have $f(t,T) = -\frac{\partial\log(P(T;t))}{\partial T}$ , i.e. 

$$
P (T; t) = \exp \big (- \int_ {0} ^ {T} f (t, \tau) \mathrm{d} \tau \big).
$$

Apart from the requirement that the processes are Itô processes, we do not consider a specific model or its implementation. A specific model would be given, if we had specified the form of $(t,T)\mapsto\sigma(t,T)$ . With a specific choice of $\sigma(t,T)$ (21.3) may become a known short rate model or the LIBOR market model, see Chapter 23. 

In this chapter we will discuss the no-arbitrage conditions of $(21.3)$ and discuss how other models fit into this framework. 

## 21.1. Short Rate Process in the HJM Framework

The specification of the families of processes $f(\cdot, T)$ implies a process for the short rate $r$ . We write Equation (21.3) in integral form<sup>3</sup> 

$$
f (t, T) = f _ {0} (T) + \int_ {0} ^ {t} \alpha (s, T) \mathrm{d} s + \int_ {0} ^ {t} \sigma (s, T) \cdot \mathrm{d} W (s).\tag{21.4}
$$

With $T \to t$ we find for the short rate $r(t) := \lim_{T \searrow t} f(t, T)$ that 

$$
r (t) = f (t, t) = f _ {0} (t) + \int_ {0} ^ {t} \alpha (s, t) \mathrm{d} s + \int_ {0} ^ {t} \sigma (s, t) \cdot \mathrm{d} W (s)\tag{21.5}
$$

and thus the short rate process is in differential notation given as 

$$
\begin{array}{c} \mathrm{d} r (t) = \left(\frac {\partial f _ {0}}{\partial T} (t) + \alpha (t, t) + \int_ {0} ^ {t} \frac {\partial \alpha}{\partial T} (s, t) \mathrm{d} s + \int_ {0} ^ {t} \frac {\partial \sigma}{\partial T} (s, t) \cdot \mathrm{d} W (s)\right) \mathrm{d} t \\ + \sigma (t, t) \cdot \mathrm{d} W (t). \end{array}\tag{21.6}
$$

Remark 221 (Notation): Equation (21.6) follows from (21.5) by differentiating with respect to t. Since t enters into the second argument of $\alpha$ and $\sigma$ , we have to calculate the partial derivative of $\alpha$ and $\sigma$ with respect to their second argument. In accordance with the notation in (21.1) we denote the partial derivative of $\alpha$ with respect to its second argument by $\frac{\partial\alpha}{\partial T}$ and the partial derivative of $\sigma$ with respect to its second argument by $\frac{\partial\sigma}{\partial T}$ . Likewise we denote the (partial) derivative of $f_{0}$ with respect to its argument by $\frac{\partial f_{0}}{\partial T}$ . 

## 21.2. The HJM Drift Condition

Theorem 222 (Heath, Jarrow, Morton - HJM Drift Condition): For the family of bond price processes $P(T)$ the following holds: The $B$ -relative price $\frac{P(T)}{B}$ is a $\mathbb{Q}^B$ -martingale, if and only if 

$$
\int_ {s} ^ {T} \alpha (s, S) \mathrm{d} S = \frac {1}{2} \int_ {s} ^ {T} \sigma (s, S) \mathrm{d} S \cdot \int_ {s} ^ {T} \sigma (s, S) \mathrm{d} S.
$$

From this we have: All bond price processes of the bond curve $T \mapsto P(T)$ are $Q^{B}$ -martingales, i.e. the model is arbitrage-free, if and only if 

$$
\alpha^ {\mathbb {Q} ^ {\mathbb {B}}} (t, T) = \sigma (t, T) \cdot \int_ {t} ^ {T} \sigma (t, \tau) \mathrm{d} \tau \quad \forall T.\tag{21.7}
$$

Equation (21.7) is called the HJM drift condition. 

Proof (of the HJM drift condition): Let T denote a fixed maturity. With $B(t) = \exp(\int_{0}^{t} r(s) \, ds)$ and $P(T; t) = \exp(-\int_{t}^{T} f(t, S) \, ds)$ it follows for the B-relative price of the bond $P(T)$ that: 

$$
\frac {P (T ; t)}{B (t)} = \exp (X (t)) \quad \text { with } \quad X (t) = - \int_ {t} ^ {T} f (t, S) \mathrm{d} S - \int_ {0} ^ {t} r (s) \mathrm{d} s.
$$

From (21.4) and (21.5) follows 

$$
\begin{array}{l} X (t) = - \int_ {t} ^ {T} f (t, S) \mathrm{d} S - \int_ {0} ^ {t} r (s) \mathrm{d} s \\ = - \int_ {t} ^ {T} f _ {0} (S) \mathrm{d} S - \int_ {t} ^ {T} \int_ {0} ^ {t} \alpha (s, S) \mathrm{d} s \mathrm{d} S - \int_ {t} ^ {T} \int_ {0} ^ {t} \sigma (s, S) \mathrm{d} W (s) \mathrm{d} S \\ - \int_ {0} ^ {t} f _ {0} (S) \mathrm{d} S - \int_ {0} ^ {t} \int_ {0} ^ {u} \alpha (s, u) \mathrm{d} s \mathrm{d} u - \int_ {0} ^ {t} \int_ {0} ^ {u} \sigma (s, u) \mathrm{d} W (s) \mathrm{d} u. \end{array}
$$

With $\int_0^t\int_0^u\mathrm{d}W(s)\mathrm{d}u = \int_0^t\int_s^t\mathrm{d}udW(s)$ and the interchange of the integrals this is 

$$
\begin{array}{l} = - \int_ {t} ^ {T} f _ {0} (S) \mathrm{d} S - \int_ {0} ^ {t} \int_ {t} ^ {T} \alpha (s, S) \mathrm{d} S \mathrm{d} s - \int_ {0} ^ {t} \int_ {t} ^ {T} \sigma (s, S) \mathrm{d} S \mathrm{d} W (s) \\ - \int_ {0} ^ {t} f _ {0} (S) \mathrm{d} S - \int_ {0} ^ {t} \int_ {s} ^ {t} \alpha (s, u) \mathrm{d} u \mathrm{d} s - \int_ {0} ^ {t} \int_ {s} ^ {t} \sigma (s, u) \mathrm{d} u \mathrm{d} W (s) \\ = - \int_ {0} ^ {T} f _ {0} (S) \mathrm{d} S - \int_ {0} ^ {t} \int_ {s} ^ {T} \alpha (s, S) \mathrm{d} S \mathrm{d} s - \int_ {0} ^ {t} \int_ {s} ^ {T} \sigma (s, S) \mathrm{d} S \mathrm{d} W (s) \\ = X (0) + \int_ {0} ^ {t} A (s) \mathrm{d} s + \int_ {0} ^ {t} \Sigma (s) \mathrm{d} W (s), \end{array}
$$

thus 

$$
\mathrm{d} X (t) = A (t) \mathrm{d} t + \Sigma (t) \mathrm{d} W (t),
$$

where 

$$
\begin{array}{l} X (0) = - \int_ {0} ^ {T} f _ {0} (S) \mathrm{d} S \\ A (s) = - \int_ {s} ^ {T} \alpha (s, S) \mathrm{d} S \\ \Sigma (s) = - \int_ {s} ^ {T} \sigma (s, S) \mathrm{d} S. \end{array}
$$

Let the $B$ -relative price of $P(T)$ be a martingale under $\mathbb{Q}^B$ , i.e. the process $\exp(X(t))$ is drift-free. From Itô's Lemma we have $\mathrm{d}\exp(X(t)) = X(t)\mathrm{d}X(t) + \frac{1}{2} X(t)\mathrm{d}X(t)\mathrm{d}X(t)$ , i.e. 

$$
\mathrm{d} \exp (X (t)) = X (t) \cdot \big ((A (s) + \frac {1}{2} \Sigma (s) \Sigma (s)) \mathrm{d} t + \Sigma (t) \mathrm{d} W (t) \big).
$$

That $\exp(X(t))$ is drift-free thus implies $A(s) + \frac{1}{2}\Sigma(s)\Sigma(s) = 0$ , i.e. 

$$
\int_ {s} ^ {T} \alpha (s, S) \mathrm{d} S = \frac {1}{2} \int_ {s} ^ {T} \sigma (s, S) \mathrm{d} S \cdot \int_ {s} ^ {T} \sigma (s, S) \mathrm{d} S.
$$

If this equation is valid for all T, we get by differentiation $\frac{\partial}{\partial T}$ the HJM drift condition 

$$
\alpha (t, T) = \sigma (t, T) \cdot \int_ {t} ^ {T} \sigma (t, S) \mathrm{d} S.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/9353b1559c84d6008bd1d64a1f823aabfd0c82aa7c2d3ddad67af3f925bb4ee9.jpg)


Interpretation (Bond Volatility): The expression $\Sigma(t) = -\int_{t}^{T} \sigma(t, S) \, \mathrm{d}S$ corresponds to the volatility of the bond price process $P(T)$ at time t (bond volatility), since we have 

$$
\begin{array}{l} \mathrm{d} P (T; t) = \mathrm{d} \big (B (t) \exp (X (t)) \big) = B (t) \mathrm{d} \exp \big (X (t) \big) \\ \qquad = B (t) \exp \big (X (t) \big) \cdot \big (\mathrm{d} X (t) + \frac {1}{2} \mathrm{d} X (t) \cdot \mathrm{d} X (t) \big) \\ \qquad = P (T; t) \cdot ((\ldots) \mathrm{d} t + \Sigma (t) \cdot \mathrm{d} W (t)) \\ \qquad = P (T; t) \cdot (\ldots) \mathrm{d} t + P (T; t) \cdot \Sigma (t) \cdot \mathrm{d} W (t). \end{array}\tag{◀|}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/1c5c89f8d2a8785a949f72e214abf3a8f0b23a327f4960c3f17574c16edf5924.jpg)


Motivation (Embedding other Models): If an interest rate model is arbitrage-free and if the processes of the instantaneous forward rates $f(\cdot, T)$ are Itô processes, then the model has to fulfill the HJM drift condition (21.7). Thus, these interest rate models may be derived as a special case of the HJM framework. 

Since the volatility structure $(t,T)\mapsto\sigma(t,T)$ and the initial conditions $f(0,T)$ are the only free parameters of the HJM framework, this embedding of arbitrage-free interest rate models can be achieved by choosing the HJM volatility structure and the initial interest rate curve. We will show in Chapter 23 how short rate models and the LIBOR market model can be interpreted as special HJM volatility structures. 

# Short Rate Models

## 22.1. Introduction

At a fixed point t in time the short rate is given by 

$$
r (t) := - \frac {\partial P (T ; t)}{\partial T} \Big | _ {T = t},
$$

see Definition 103. Thus $r: t \mapsto r(t)$ is a real valued stochastic process. We make the following assumptions: 

1. Given is a model for r (short rate model), e.g. in the form of an Itô process 

$$
\mathrm{d} r = \mu^ {\mathbb {P}} (t, r) \mathrm{d} t + \sigma (t, r) \mathrm{d} W ^ {\mathbb {P}} (t), \quad r (0) = r _ {0},\tag{22.1}
$$

where P denote the real probability measure. 

2. The continuously compounding money market account $B(t)$ , 

$$
\mathrm{d} B (t) = r (t) B (t) \mathrm{d} t, \quad B (0) = 1, \quad \text { d   .   h } \quad B (t) = \exp \left(\int_ {0} ^ {t} r (\tau) \mathrm{d} \tau\right),
$$

is a traded asset. $^{1}$ 

3. Corresponding to the numéraire $N(t) = B(t)$ there exists a martingale measure $\mathbb{Q} = \mathbb{Q}^B$ equivalent to $\mathbb{P}$ . 

From the Girsanov's Theorem $^{2}$ the process of r under Q is 

$$
\mathrm{d} r = \mu^ {\mathbb {Q}} (t, r) \mathrm{d} t + \sigma (t, r) \mathrm{d} W ^ {\mathbb {Q}} (t), \quad r (0) = r _ {0}.\tag{22.2}
$$

with $\mu^{\mathbb{Q}}(t,r) = \mu^{\mathbb{P}}(t,r) + C(t)$ . Since under $\mathbb{Q}$ all $B$ -relative prices of traded assets are martingales, all bond prices are given by 

$$
P (T; t) = B (t) \mathrm{E} ^ {\mathbb {Q}} \left(\frac {1}{B (T)} \mid \mathcal {F} _ {t}\right) = \mathrm{E} ^ {\mathbb {Q}} \left(\exp \left(- \int_ {t} ^ {T} r (\tau) \mathrm{d} \tau\right) \mid \mathcal {F} _ {t}\right).
$$

From the bond prices $P(T;t)$ we can calculate all derived quantities such as forward rates or swap rates, see Section 8.2. Thus, the short rate model (22.2) gives a complete description of the interest rate curve dynamic. 

Short rate models were and are popular, since the underlying stochastic process r is one-dimensional (i.e. scalar valued). Thus many techniques that are known from the modeling of (also one-dimensional) stock price processes can be used (e.g. finite difference implementations). Depending on the specific model (i.e. the form of $\mu^{Q}$ and $\sigma$ ), analytic formulas for bond prices or simple European interest rate options may be derived, similar to the Black-Scholes formula for European stock options under a Black-Scholes model. 

Instead of specifying the model (22.1) of the short rate process under the real measure P and applying the measure transformation to Q, is is usual to specify the model (22.2) directly under Q and calibrate given model parameters. 

## 22.2. The Market Price of Risk

Consider a bond with maturity T. Under a short rate model its price price process $P(T): t \mapsto P(T; t)$ is a function of $(t, r(t))$ and if Itô's Lemma is applicable we have $^{3}$ 

$$
\mathrm{d} P (T) = \alpha_ {T} ^ {\mathbb {P}} (t, r) P (T) \mathrm{d} t + \sigma_ {T} (t, r) P (T) \mathrm{d} W ^ {\mathbb {P}} (t),\tag{22.3}
$$

where the price process is considered under the real measure P. 

Let $P(T_{1})$ and $P(T_{2})$ denote two bonds with different maturities $T_{1} \neq T_{2}$ . We construct a portfolio process $(\phi_{0}, \phi_{1})$ for a self-financing portfolio of B and $P(T_{1})$ , which replicates $P(T_{2})$ . The portfolio process $(\phi_{0}, \phi_{1})$ has to satisfy the following equations: 

$$
\phi_ {0} B + \phi_ {1} P (T _ {1}) = P (T _ {2})
$$

$$
(\text { "replicating" })\tag{22.4}
$$

$$
\mathrm{d} \left(\phi_ {0} B + \phi_ {1} P \left(T _ {1}\right)\right) = \phi_ {0} \mathrm{d} B + \phi_ {1} \mathrm{d} P \left(T _ {1}\right)
$$

$$
\left(" \text { self - financing }"\right).\tag{22.5}
$$

From (22.4) we find $\mathrm{d}P(T_2) = \mathrm{d}(\phi_0B + \phi_1P(T_1))$ and with 

$$
\begin{array}{c} \mathrm{d} (\phi_ {0} B + \phi_ {1} P (T _ {1})) \stackrel {{(2 2. 5)}} {{=}} (\phi_ {0} r B + \phi_ {1} \alpha_ {T _ {1}} ^ {\mathbb {P}} P (T _ {1})) \mathrm{d} t + \phi_ {1} \sigma_ {T _ {1}} P (T _ {1}) \mathrm{d} W ^ {\mathbb {P}} (t) \\ \mathrm{d} P (T _ {2}) \stackrel {{(2 2. 3)}} {{=}} \alpha_ {T _ {2}} ^ {\mathbb {P}} P (T _ {2}) \mathrm{d} t + \sigma_ {T _ {2}} P (T _ {2}) \mathrm{d} W ^ {\mathbb {P}} (t). \end{array}
$$

we have, by comparing coefficients, 

$$
\alpha_ {T _ {2}} ^ {\mathbb {P}} P (T _ {2}) = \phi_ {0} r B + \phi_ {1} \alpha_ {T _ {1}} ^ {\mathbb {P}} P (T _ {1})\tag{22.6}
$$

$$
\sigma_ {T _ {2}} P (T _ {2}) = \phi_ {1} \sigma_ {T _ {1}} P (T _ {1}).\tag{22.7}
$$

While (22.7) and (22.4) uniquely determine the portfolio process $(\phi_{0},\phi_{1})$ , (22.6) is a consistency condition for r, $\alpha_{T_{1}}$ and $\alpha_{T_{2}}$ . If (22.6) were violated, then the model would not be arbitrage-free. We rewrite the consistency condition (22.6) as: 

$$
\alpha_ {T _ {2}} ^ {\mathbb {P}} \cdot P (T _ {2}) = \phi_ {0} \cdot r \cdot B + \phi_ {1} \cdot \alpha_ {T _ {1}} ^ {\mathbb {P}} \cdot P (T _ {1})
$$

$$
\alpha_ {T _ {2}} ^ {\mathbb {P}} \cdot P (T _ {2}) = \phi_ {0} \cdot r \cdot B + \phi_ {1} \cdot r \cdot P (T _ {1}) + \phi_ {1} \cdot (\alpha_ {T _ {1}} ^ {\mathbb {P}} - r) \cdot P (T _ {1})
$$

$$
\alpha_ {T _ {2}} ^ {\mathbb {P}} \cdot P (T _ {2}) = r \cdot P (T _ {2}) + \phi_ {1} \cdot (\alpha_ {T _ {1}} ^ {\mathbb {P}} - r) \cdot P (T _ {1})
$$

$$
(\alpha_ {T _ {2}} ^ {\mathbb {P}} - r) \cdot P (T _ {2}) = \phi_ {1} \cdot (\alpha_ {T _ {1}} ^ {\mathbb {P}} - r) \cdot P (T _ {1})
$$

$$
\frac {\alpha_ {T _ {2}} ^ {\mathbb {P}} - r}{\sigma_ {T _ {2}}} = \frac {\alpha_ {T _ {1}} ^ {\mathbb {P}} - r}{\sigma_ {T _ {1}}}.
$$

It follows that there exists a $\lambda^{P}$ , such that for all bond price processes 

$$
\mathrm{d} P (T) = \alpha_ {T} ^ {\mathbb {P}} (t, r) \cdot P (T) \cdot \mathrm{d} t + \sigma_ {T} (t, r) \cdot P (T) \cdot \mathrm{d} W ^ {\mathbb {P}} (t)
$$

we have 

$$
\frac {\alpha_ {T} ^ {\mathbb {P}} - r}{\sigma_ {T}} =: \lambda^ {\mathbb {P}}.
$$

Since $\alpha^{\mathbb{P}}$ is the local rate of return of the bond, we may interpret $\lambda^{\mathbb{P}}$ as the local excess return rate over $r$ per risk unit $\sigma_T$ . 

## Definition 223 (Market Price of Risk):

The quantity $\lambda^{P} := \frac{\alpha_{T}^{E}-r}{\sigma_{T}}$ , which is independent of T, is called the Market Price of Risk. 

If we consider the bond price process 

$$
\mathrm{d} P (T) = \alpha_ {T} ^ {\mathbb {Q}} (t) P (T) \mathrm{d} t + \sigma_ {T} (t) P (T) \mathrm{d} W ^ {\mathbb {Q}} (t)
$$

under the measure $\mathbb{Q}$ , it is obvious that $\alpha_T^{\mathbb{Q}} = r$ for all $T$ , since all $B$ -relative prices are $\mathbb{Q}$ -martingales. Thus, under $\mathbb{Q}$ the Price of Risk $\lambda^{\mathbb{Q}} = 0$ . It follows that 

$$
\mu_ {T} ^ {\mathbb {Q}} = \lambda^ {\mathbb {Q}} \cdot \sigma_ {T} + r = 0 + r = \lambda^ {\mathbb {P}} \cdot \sigma_ {T} + r - \lambda^ {\mathbb {P}} \cdot \sigma_ {T} = \mu_ {T} ^ {\mathbb {P}} - \lambda^ {\mathbb {P}} \cdot \sigma_ {T},
$$

and we find that Market Price of Risk $\lambda^{P}$ appears in the change of drift to the measure Q, i.e. we have $C(t) = -\lambda^{P} \cdot \sigma_{T}$ in Theorem 58. 

## Definition 224 (Risk Neutral Measure):

Let $r(t)$ denote the short rate. The martingale measure $\mathbb{Q}^B$ corresponding to the numéraire $B(t) = \exp\left(\int_0^t r(\tau)\mathrm{d}\tau\right)$ is called the risk-neutral measure. 

Remark 225 (Risk Neutral Measure): The continuously compounding money market account B is locally risk free, since the process $\mathrm{d}B(t) = r(t)B(t)\mathrm{d}t$ does not exhibit a $\mathrm{d}W(t)$ term. However, $r(t)$ may be stochastic. If r were not stochastic, then B would be globally risk free. 

## 22.3. Overview: Some Common Models

## Table 22.3 gives a selection of the most common short rate models.

The Hull-White model is sometimes called extended Vasicek model. The Vasicek, Hull-White and Ho-Lee models allow for negative short rates. The Black-Derman-Toy (BDT) and 

<table><tr><td>Name</td><td>Model</td></tr><tr><td>Vasicek Model</td><td><eq>\mathrm{d}r = (b - ar)\mathrm{d}t + \sigma\mathrm{d}W^{\mathbb{Q}}</eq></td></tr><tr><td>Hull-White Model</td><td><eq>\mathrm{d}r = (\phi(t) - ar)\mathrm{d}t + \sigma(t)\mathrm{d}W^{\mathbb{Q}}</eq></td></tr><tr><td>Ho-Lee Model</td><td><eq>\mathrm{d}r = a(t)\mathrm{d}t + \sigma(t)\mathrm{d}W^{\mathbb{Q}}</eq></td></tr><tr><td>Dothan Model</td><td><eq>\mathrm{d}r = ar\mathrm{d}t + \sigma r\mathrm{d}W^{\mathbb{Q}}</eq></td></tr><tr><td>Black-Derman-Toy Model</td><td><eq>\mathrm{d}\ln(r) = \phi(t)\mathrm{d}t + \sigma(t)\mathrm{d}W^{\mathbb{Q}}</eq></td></tr><tr><td>Black-Karasinski Model</td><td><eq>\mathrm{d}\ln(r) = (\phi(t) - a\ln(r))\mathrm{d}t + \sigma(t)\mathrm{d}W^{\mathbb{Q}}</eq></td></tr><tr><td>Cox-Ingersoll-Ross Model</td><td><eq>\mathrm{d}r = (b - ar)\mathrm{d}t + \sigma(t)\sqrt{r}\mathrm{d}W^{\mathbb{Q}}</eq></td></tr></table>


Table 22.1.: Selection of Short Rate Models


Black-Karansinski (BK) models use a lognormal process and the Cox-Ingersoll-Ross model uses a square-root process. Neither of these two processes allow for negative rates. $^{4}$ 

## 22.4. Implementations

## 22.4.1. Monte-Carlo Implementation of Short-Rate Models

A short-rate model gives a description of the dynamic of the short rate. To obtain a complete interest rate curve at a given simulation time t, we have to calculate the bond prices from $(22.1)$ as conditional expectation. To calculate a conditional expectation in a Monte-Carlo simulation numerically requires additional, numerically expensive methods, see Chapter 15. To obtain a Monte-Carlo simulation of the full interest rate curve from a Monte-Carlo simulation of the short rate, analytic formulas for bond-prices are indispensable. The popularity of short rate models is thus partly due to the need for a simple and efficient implementation. 

For a fast calibration to a given interest rate curve it is also required to calculate bond prices analytically. 

## 22.4.2. Lattice Implementation of Short-Rate Models

If the short rate model is Markovsch in low dimensions, then it is best to implement the short rate model on a lattice, allowing for a backward algorithm. $^{5}$ Depending on the model, implementations using binomial or trinomial trees or general finite differences for pde's are used. See [35] for a detailed discussion. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/7447d4115ab9a991975494b8368962fe7f66c971b2dbb781191d91c80358e8a4.jpg)


Further Reading: Björg's book [7] contains a discussion of short rate model with affine term structure. Tavella and Randal's book [35] gives an introduction to finite difference methods, also with applications to interest rate models. 

# Heath-Jarrow-Morton Framework: Immersion of Short Rate Models and LIBOR Market Model

You're going to find that many of the truths we cling to depend greatly on our own point of view. 

Obi-Wan Kenobi / George Lucas Star Wars: Episode VI, (Wikiquote). 

## 23.1. Short Rate Models in the HJM Framework

The Heath-Jarrow-Morton framework 

$$
\begin{array}{c} \mathrm{d} f (t, T) = \alpha (t, T) \mathrm{d} t + \sigma (t, T) \mathrm{d} W (t) \\ f (0, T) = f _ {0} (T) \end{array}\tag{was 21.3}
$$

implies the short rate process 

$$
\begin{array}{l} \mathrm{d} r (t) = \left(\frac {\partial f _ {0}}{\partial T} (t) + \alpha (t, t) + \int_ {0} ^ {t} \frac {\partial \alpha}{\partial T} (s, t) \mathrm{d} s + \int_ {0} ^ {t} \frac {\partial \sigma}{\partial T} (s, t) \mathrm{d} W (s)\right) \mathrm{d} t \\ \qquad \qquad \qquad \qquad \qquad \qquad \qquad + \sigma (t, t) \mathrm{d} W (t), \end{array}\tag{was 21.6}
$$

both under the measure $Q^{B}$ - see (21.3), (21.4), (21.5), (21.6) on Page 280. The short rate model is thus given by the specific choice of the HJM volatility structure $\sigma(t,t)$ ( $\rightarrow$ short rate volatility) and initial conditions $f_{0}$ ( $\rightarrow$ short rate drift). 

## 23.1.1. Example: The Ho-Lee Model in the HJM Framework

Consider the simple case of a constant volatility function 

$$
\sigma (t, T) = \sigma = c o n s t.
$$

From (21.7) we have $\alpha(t, T) = \sigma \cdot \int_t^T \sigma \, \mathrm{d}\tau = \sigma^2 \cdot (T - t)$ , i.e. 

$$
\mathrm{d} f (t, T) = \sigma^ {2} \cdot (T - t) \mathrm{d} t + \sigma \mathrm{d} W (t), \qquad f (0, T) = f _ {0} (T).
$$

For the short rate it follows that 

$$
\begin{array}{l} r (t) = f (t, t) = f _ {0} (t) + \int_ {0} ^ {t} \sigma^ {2} \cdot (T - s) \mathrm{d} s \bigg | _ {T = t} + \int_ {0} ^ {t} \sigma \mathrm{d} W (s) \\ = f _ {0} (t) + \frac {1}{2} \sigma^ {2} t ^ {2} + \sigma W (t), \end{array}
$$

i.e. 

$$
\mathrm{d} r (t) = \Big (\frac {\mathrm{d} f _ {0}}{\mathrm{d} T} (t) + \sigma^ {2} t \Big) \mathrm{d} t + \sigma \mathrm{d} W (t).
$$

Using the notation from the Ho-Lee model, $\mathrm{d}r(t)=\phi(t)\mathrm{d}t+\sigma\mathrm{d}W(t)$ , it is 

$$
\phi (t) = \frac {\mathrm{d} f _ {0}}{\mathrm{d} T} (t) + \sigma^ {2} t.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/ecb4e80665d719312a551510a557a2a8e1654cc6a15842a50d3c29fca8b1e9f5.jpg)


Interpretation: The Equation (23.1.1) allows a calibration of the Ho-Lee model to a given curve of bond prices $P(T)$ by setting $\phi(t) = -\frac{\mathrm{d}^{2}\log(P(T))}{\mathrm{d}T^{2}}(t) + \sigma^{2}t$ . With this choice the model reproduces the given bond prices. 

If we consider the interest rate curve $f_{T_1}(T) := f(T_1, T_1 + T)$ , $T \geq 0$ at a later time $T_1 > 0$ , then from 

$$
\frac {\mathrm{d} f _ {T _ {1}}}{\mathrm{d} T} (t) + \sigma^ {2} t = \phi (T _ {1} + t) = \frac {\mathrm{d} f _ {0}}{\mathrm{d} T} (T _ {1} + t) + \sigma^ {2} (T _ {1} + t),
$$

we find that $f_{T_1}(t) = f_{T_1}(0) + f_0(T_1 + t) - f_0(t) + \sigma^2 (T_1\cdot t + \frac{1}{2} t^2).$ 

So to summarize, the model reproduces all bond prices, but in the evolution the interest rate curve gets steeper and steeper - a rather unrealistic behavior. 

## 23.1.2. Example: The Hull-White Model in the HJM Framework

Consider the case of an exponentially volatility function 

$$
\sigma (t, T) = \sigma \cdot e ^ {- a \cdot (T - t)}, \qquad (a > 0).
$$

Then we have $\frac{\partial\sigma}{\partial T}(t,T) = -a\cdot \sigma \cdot e^{-a\cdot (T - t)} = -a\sigma (t,T)$ . For the drift $\mu (t)$ of the short rate process $\mathrm{dr}(t) = \mu (t)\mathrm{d}t + \sigma (t,t)\mathrm{d}W(t)$ we get 

$$
\begin{array}{r l} \mu (t) & \stackrel {(2 1. 6)} {=} \frac {\partial f _ {0}}{\partial T} (t) + \alpha (t, t) + \int_ {0} ^ {t} \frac {\partial \alpha}{\partial T} (s, t) \mathrm{d} s + \int_ {0} ^ {t} \frac {\partial \sigma}{\partial T} (s, t) \mathrm{d} W (s) \\ & = \frac {\partial f _ {0}}{\partial T} (t) + \alpha (t, t) + \int_ {0} ^ {t} \frac {\partial \alpha}{\partial T} (s, t) \mathrm{d} s - \int_ {0} ^ {t} a \cdot \sigma (s, t) \mathrm{d} W (s) \\ & \stackrel {(2 1. 5)} {=} \frac {\partial f _ {0}}{\partial T} (t) + \alpha (t, t) + \int_ {0} ^ {t} \frac {\partial \alpha}{\partial T} (s, t) \mathrm{d} s - a \cdot r (t) + a \cdot f _ {0} (t) + \int_ {0} ^ {t} a \alpha (s, t) \mathrm{d} s, \end{array}
$$

i.e. 

$$
\mathrm{d} r (t) = (\phi (t) - a r (t)) \mathrm{d} t + \sigma \mathrm{d} W (t)
$$

with 

$$
\phi (t) = \frac {\partial f _ {0}}{\partial T} (t) + a \cdot f _ {0} (t) + \alpha (t, t) + \int_ {0} ^ {t} \frac {\partial \alpha}{\partial T} (s, t) \mathrm{d} s + \int_ {0} ^ {t} a \cdot \alpha (s, t) \mathrm{d} s.
$$

With the HJM drift condition (21.7) it follows that $\alpha(t, T) = \sigma^2 \cdot e^{-a \cdot (T - t)} \cdot \frac{1}{a} (1 - e^{-a \cdot (T - t)}) = \sigma^2 \cdot \frac{1}{a} (e^{-a \cdot (T - t)} - e^{-2a \cdot (T - t)})$ and thus 

$$
\begin{array}{l} \phi (t) = \frac {\partial f _ {0}}{\partial T} (t) + a \cdot f _ {0} (t) + \alpha (t, t) + \int_ {0} ^ {t} \frac {\partial \alpha}{\partial T} (s, t) \mathrm{d} s + \int_ {0} ^ {t} a \cdot \alpha (s, t) \mathrm{d} s \\ = \frac {\partial f _ {0}}{\partial T} (t) + a \cdot f _ {0} (t) + \int_ {0} ^ {t} \sigma^ {2} e ^ {- 2 a \cdot (t - s)} \mathrm{d} s \\ = \frac {\partial f _ {0}}{\partial T} (t) + a \cdot f _ {0} (t) + \frac {\sigma^ {2}}{2 a} (1 - e ^ {- 2 a \cdot t}). \end{array}
$$

Altogether we have 

$$
\mathrm{d} r (t) = \left(\frac {\partial f _ {0}}{\partial T} (t) + a \cdot f _ {0} (t) + \frac {\sigma^ {2}}{2 a} \left(1 - e ^ {- 2 a \cdot t}\right) - a r (t)\right) \mathrm{d} t + \sigma \mathrm{d} W (t).
$$

Note that this equation allows a calibration of the Hull-White model to a given curve of bond prices. From the bond price curve we can calculate $\frac{\partial f_{0}}{\partial T}(t) + a \cdot f_{0}(t)$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/660a707b3791243bb51a2488e28996d30a498b104aa34a87a62cbccc719508f5.jpg)


Interpretation (Mean Reversion): The derivation of a Hull-White model from a Heath-Jarrow-Morton model gives an important insight to the relevance of the timer structure of the volatility function: 

A volatility function of the instantaneous forward rate $f(t, T)$ , which is exponentially decaying in $(T - t)$ (time to maturity), i.e. $\sigma(t, T) = \exp(-a(T - t))$ , corresponds to a mean reversion term for the short rate process $r(t)$ with mean reversion speed a. 

Correspondingly, this effect is visible in the LIBOR Market Model, see Chapter 24. 

## 23.2. LIBOR Market Model in the HJM Framework

## 23.2.1. HJM Volatility Structure of the LIBOR Market Model

In the specification (19.1) of the LIBOR Market Model dW denoted the increment of a n-dimensional Brownian motion with instantaneous correlation R. In the specification (21.3) of the HJM Framework dW denoted the increment of a m-dimensional Brownian motion with instantaneous uncorrelated components. To resolve this conflict we employ the notation of Section 2.7: Let U denote an m-dimensional Brownian motion with instantaneous uncorrelated components and W denote an n-dimensional Brownian motion with $\mathrm{d}W(t) = F(t) \cdot \mathrm{d}U(t)$ , i.e. the instantaneous correlation of W is $R := FF^{T}$ . Consider the HJM model 

$$
\begin{array}{l} \mathrm{d} f (t, T) = \alpha^ {\mathbb {Q}} (t, T) \mathrm{d} t + \sigma (t, T) \mathrm{d} U ^ {\mathbb {Q}} (t) \\ f (0, T) = f _ {0} (T) \end{array}\tag{23.1}
$$

with $\mathrm{d}U = (\mathrm{d}U_1,\dots ,\mathrm{d}U_m)$ . From 

$$
P (T; t) = \exp \big (- \int_ {t} ^ {T} f (t, \tau) \mathrm{d} \tau \big).
$$

(see Remark 102) it follows that the forward Rate $L_{i}(t) := L(T_{i}, T_{i+1}; t)$ is given by 

$$
1 + L _ {i} (t) \cdot \Delta T _ {i} = \frac {P \left(T _ {i} ; t\right)}{P \left(T _ {i + 1} ; t\right)} = \exp \left(\int_ {T _ {i}} ^ {T _ {i + 1}} f (t, \tau) \mathrm{d} \tau\right).
$$

Note that for $X(t) := \int_{T_i}^{T_{i+1}} f(t, \tau) \mathrm{d}\tau$ we have by the linearity of the integral that $\mathrm{d}X = \int_{T_i}^{T_{i+1}} \mathrm{d}f(t, \tau) \mathrm{d}\tau$ , thus we find from Itô's Lemma that within the HJM framework the process of the forward rate $L_i(t)$ is 

$$
\begin{array}{l} \mathrm{d} L _ {i} (t) \cdot \Delta T _ {i} = \mathrm{d} \exp (X) = \exp (X) \cdot (\mathrm{d} X + \frac {1}{2} \mathrm{d} X \cdot \mathrm{d} X) \\ = \exp \left(\int_ {T _ {i}} ^ {T _ {i + 1}} f (t, \tau) \mathrm{d} \tau\right) \cdot \left[ \int_ {T _ {i}} ^ {T _ {i + 1}} (\mathrm{d} f (t, \tau)) \mathrm{d} \tau \right. \\ \qquad \qquad \qquad \qquad \qquad \qquad + \frac {1}{2} \int_ {T _ {i}} ^ {T _ {i + 1}} (\mathrm{d} f (t, \tau)) \mathrm{d} \tau \cdot \int_ {T _ {i}} ^ {T _ {i + 1}} (\mathrm{d} f (t, \tau)) \mathrm{d} \tau \Bigg ] \\ = (1 + L _ {i} (t) \cdot \Delta T _ {i}) \cdot \left[ (A (t) + \frac {1}{2} \Sigma (t) \cdot \Sigma (t)) \mathrm{d} t + \Sigma \cdot \mathrm{d} U ^ {\mathbb {Q}} \right] \end{array}
$$

where $A(t)=\int_{T_{i}}^{T_{i+1}}\alpha^{\mathbb{Q}}(t,\tau)\mathrm{d}\tau$ and $\Sigma(t)=\int_{T_{i}}^{T_{i+1}}\sigma(t,\tau)\mathrm{d}\tau.$ 

$$
\mathrm{d} L _ {i} (t) = \frac {1 + L _ {i} (t) \cdot \Delta T _ {i}}{\Delta T _ {i}} \cdot \left((A (t) + \frac {1}{2} \Sigma (t) \cdot \Sigma (t)) \mathrm{d} t + \int_ {T _ {i}} ^ {T _ {i + 1}} \sigma (t, \tau) \mathrm{d} \tau \mathrm{d} U ^ {\mathbb {Q}} (t)\right)\tag{23.2}
$$

We will now choose the volatility structure such that (23.2) corresponds to the process of a LIBOR market model: Let $W = (W_{1},\ldots ,W_{n})$ denote an $n$ -dimensional Brownian motion as given in Section 2.7. 

$\mathrm{d}W(t) = F(t)\cdot \mathrm{d}U(t),$ with correlation matrix $R:= FF^{\mathrm{T}}$ 

i.e. 

$$
\mathrm{d} W _ {i} (t) = F _ {i} (t) \cdot \mathrm{d} U (t), \qquad \text { with } F = \left( \begin{array}{c} F _ {1} \\ \vdots \\ F _ {n} \end{array} \right).
$$

Let the volatility structure be chosen as 

$$
\sigma (t, \tau) = \left\{ \begin{array}{l l} \frac {L _ {i} (t)}{1 + L _ {i} (t) \Delta T _ {i}} \sigma_ {i} (t) \cdot F _ {i} (t) & \text { for } t \leq T _ {i} \\ (0, \ldots , 0) & \text { for } t > T _ {i}, \end{array} \right.\tag{23.3}
$$

where $i$ is such that $\tau \in [T_i, T_{i+1})$ . Then we have 

$$
\frac {1 + L _ {i} (t) \cdot \Delta T _ {i}}{\Delta T _ {i}} \cdot \int_ {T _ {i}} ^ {T _ {i + 1}} \sigma (t, \tau) \mathrm{d} \tau \mathrm{d} U = \left\{ \begin{array}{l l} L _ {i} (t) \sigma_ {i} (t) \mathrm{d} W (t) & \text {for t\leq T_{i}}, \\ 0 & \text {for t > T_{i}}, \end{array} \right.
$$

The forward rate then follows the process 

$$
\mathrm{d} L _ {i} = \mu_ {i} ^ {\mathbb {Q} ^ {B}} (t) L _ {i} (t) \mathrm{d} t + \sigma_ {i} (t) L _ {i} (t) \mathrm{d} W _ {i} (t),
$$

where 

$$
\mu_ {i} ^ {\mathbb {Q} ^ {B}} = \frac {1 + L _ {i} (t) \cdot \Delta T _ {i}}{L _ {i} (t) \Delta T _ {i}} \cdot \left(\int_ {T _ {i}} ^ {T _ {i + 1}} \alpha^ {\mathbb {Q}} (t, \tau) d \tau + \frac {1}{2} \int_ {T _ {i}} ^ {T _ {i + 1}} \sigma (t, \tau) d \tau \cdot \int_ {T _ {i}} ^ {T _ {i + 1}} \sigma (t, \tau) d \tau\right).
$$

Interpretation (LIBOR Market Model as HJM Framework with discrete Tenor Structure): Apart from the factor $\frac{L_{i}(t)}{1+L_{i}(t)\Delta T_{i}}$ , (23.3) gives the volatility structure $\sigma(t,T)$ of $f(t,T)$ as piecewise constant in T. The factor $L_{i}(t)$ results from the requirement to have a lognormal process for $L_{i}$ . The factor $\frac{1}{1+L_{i}(t)\Delta T_{i}}$ results 

from the discretization of the tenor structure. This shows that the LIBOR Market Model can be interpreted as HJM framework with discrete tenor structure. In the limit $\Delta T_{i} \to 0$ the factor $\frac{1}{1 + L_i(t)\Delta T_i}$ vanishes and we obtain (apart from the restriction to a lognormal model) the HJM framework. 

## 23.2.2. LIBOR Market Model Drift under the $Q^{B}$ Measure

The HJM drift condition states that 

$$
\alpha^ {\mathbb {Q} ^ {B}} (t, T) = \sigma (t, T) \cdot \int_ {t} ^ {T} \sigma (t, \tau) \mathrm{d} \tau .
$$

Since for fixed $t \sigma(t, T)$ is a piecewise constant function in $T$ - namely constant on $[T_i, T_{i+1})$ , we have for $T \in [T_i, T_{i+1})$ 

$$
\alpha^ {\mathbb {Q} ^ {B}} (t, T) = \sigma (t, T _ {i}) \cdot \big (\underbrace {\sigma (t , t) (T _ {m (t) + 1} - t)} _ {= 0} + \sum_ {j = m (t) + 1} ^ {i - 1} \sigma (t, T _ {j}) \Delta T _ {j} + \sigma (t, T _ {i}) (T - T _ {i}) \big)
$$

where $m(t) := \max\{i : T_i \leq t\}$ . Thus we have 

$$
\int_ {T _ {i}} ^ {T _ {i + 1}} \alpha^ {\mathbb {Q} ^ {B}} (t, \tau) \mathrm{d} \tau = \sigma (t, T _ {i}) \Delta T _ {i} \cdot \big (\sum_ {j = m (t) + 1} ^ {i - 1} \sigma (t, T _ {j}) \Delta T _ {j} + \frac {1}{2} \sigma (t, T _ {i}) \Delta T _ {i} \big).
$$

With $\sigma (t,T_i)\cdot \sigma (t,T_j) = \frac{\sigma_iL_i}{1 + L_i\Delta T_i}\frac{\sigma_jL_j}{1 + L_j\Delta T_j}\rho_{i,j}$ we find 

$$
\begin{array}{l} \mu_ {i} ^ {\mathbb {Q} ^ {B}} = \frac {1 + L _ {i} (t) \cdot \Delta T _ {i}}{L _ {i} (t) \Delta T _ {i}} \cdot \Big (\int_ {T _ {i}} ^ {T _ {i + 1}} \alpha^ {\mathbb {Q} ^ {B}} (t, \tau) \mathrm{d} \tau + \frac {1}{2} \int_ {T _ {i}} ^ {T _ {i + 1}} \sigma (t, \tau) \mathrm{d} \tau \cdot \int_ {T _ {i}} ^ {T _ {i + 1}} \sigma (t, \tau) \mathrm{d} \tau \Big) \\ = \frac {1 + L _ {i} (t) \cdot \Delta T _ {i}}{L _ {i} (t) \Delta T _ {i}} \cdot \frac {\sigma_ {i} L _ {i} \Delta T _ {i}}{1 + L _ {i} \Delta T _ {i}} \cdot (\sum_ {j = m (t) + 1} ^ {i - 1} \frac {\sigma_ {j} L _ {j} \Delta T _ {j}}{1 + L _ {j} \Delta T _ {j}} \rho_ {i, j} + \frac {\sigma_ {i} L _ {i} \Delta T _ {i}}{1 + L _ {i} \Delta T _ {i}}) \\ = \frac {1 + L _ {i} (t) \cdot \Delta T _ {i}}{L _ {i} (t) \Delta T _ {i}} \cdot \frac {\sigma_ {i} L _ {i} \Delta T _ {i}}{1 + L _ {i} \Delta T _ {i}} \cdot (\sum_ {j = m (t) + 1} ^ {i} \frac {\sigma_ {j} L _ {j} \Delta T _ {j}}{1 + L _ {j} \Delta T _ {j}} \rho_ {i, j}) \\ = \sigma_ {i} \cdot (\sum_ {j = m (t) + 1} ^ {i} \frac {\sigma_ {j} L _ {j} \Delta T _ {j}}{1 + L _ {j} \Delta T _ {j}} \rho_ {i, j}). \end{array}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/ae9ebcda15221c8bec1893457ef18a63d9777b8a16d0906cea5458ed9a6929c7.jpg)


Interpretation: Surprisingly, we find that the drift under $Q^{B}$ is identical to the drift under the spot LIBOR measure (see Section 19.1.1.2)) 

$$
N (t) = P (T _ {m (t) + 1}; t) \prod_ {j = 0} ^ {m (t)} (1 + L _ {j} (T _ {j}) \cdot \Delta T _ {j}), \quad (\text { Spot   LIBOR   Measure,   s. } 1 9. 9)
$$

The reason is simple: Under the assumed volatility structure the numéraires $B(t)$ and $N(t)$ are identical. To be precise, it is the assumption 

$$
\sigma (t, T) = 0 \quad \mathrm{for} T _ {m (t)} \leq t \leq T <   T _ {m (t) + 1}\tag{23.4}
$$

which implies that the two numéraires coincide. By this the HJM drift implies 

$$
\alpha^ {\mathbb {Q} ^ {B}} (t, T) = 0 \quad \text { for } T _ {m (t)} \leq t \leq T <   T _ {m (t) + 1}
$$

and thus for $T_{m(t)} \leq T < T_{m(t) + 1}$ : 

$$
f (t, T) = f \left(T _ {m (t)}, T\right) + \underbrace {\int_ {T _ {i}} ^ {t} \alpha^ {\mathbb {Q} ^ {B}} (\tau , T) \mathrm{d} \tau} _ {= 0} + \underbrace {\int_ {T _ {i}} ^ {t} \sigma (\tau , T) \mathrm{d} W ^ {\mathbb {Q} ^ {B}} (\tau)} _ {= 0}.
$$

From $f(t,T) = f(T_{m(t)},T)$ we have 

$$
\begin{array}{l} \frac {B (t)}{B (T _ {m (t)})} = \exp \left(\int_ {T _ {m (t)}} ^ {t} f (\tau , \tau) \mathrm{d} \tau\right) = \exp \left(\int_ {T _ {m (t)}} ^ {t} f (T _ {i}, \tau) \mathrm{d} \tau\right) \\ = \frac {P (T _ {m (t) + 1} ; t)}{P (T _ {m (t) + 1} ; T _ {m (t)})} = \frac {N (t)}{N (T _ {m (t)})}, \end{array}
$$

with $B(0) = N(0) = 1$ i.e. $B(t) = N(t)$ . 

◀| 

We will summarize this result as a theorem: 

Theorem 226 (Equivalence of the risk-neutral measure and the spot LIBOR measure): Given a tenor structure $0 = T_0 < T_1 < \ldots < T_n$ . Under the assumption the $T_{i+1}$ -bond $P(T_{i+1}; t)$ has volatility 0 on $t \in [T_i, T_{i+1}]$ for all $i = 0, 1, 2, \ldots$ , we have 

$$
B (t) = N (t)
$$

for $B(t)$ as in (21.2) and $N(t)$ as in (19.9). 

Proof: The claim follows from the considerations above, since the assumption in the theorem is equivalent to (23.4). □ 

## 23.2.3. LIBOR Market Model as a Short Rate Model

In 23.2.1 we have given the volatility structure for $(t,T)\mapsto f(t,T)$ under which the forward rates $L_{i}$ evolve as in a LIBOR market model. Since the short rate is given as $r(t):=\lim_{T\searrow t}f(t,T)$ , the volatility structure also implies a short rate model. Furthermore, the numéraire $B(t) = \exp(\int_{0}^{t} r(\tau) \mathrm{d}\tau)$ is fully determined by the short rate, thus the short rate process under $Q^{B}$ gives a complete description of all bond prices (and all derivatives): 

$$
P (T; t) = B (t) \mathrm{E} ^ {\mathbb {Q} ^ {B}} \left(\frac {1}{B (T)} | \mathcal {F} _ {t}\right).
$$

The short rate process $r$ implied by the volatility structure (23.3) generates a LIBOR market model. The short rate process under $\mathbb{Q}^B$ is given by (21.6): 

$$
\begin{array}{c} \mathrm{d} r (t) = \left(\frac {\partial f _ {0}}{\partial T} (t) + \alpha^ {\mathbb {Q} ^ {B}} (t, t) + \int_ {0} ^ {t} \frac {\partial \alpha^ {\mathbb {Q} ^ {B}}}{\partial T} (s, t) \mathrm{d} s + \int_ {0} ^ {t} \frac {\partial \sigma}{\partial T} (s, t) \mathrm{d} W ^ {\mathbb {Q} ^ {B}} (s)\right) \mathrm{d} t \\ + \sigma (t, t) \mathrm{d} W ^ {\mathbb {Q} ^ {B}} (t), \end{array}\tag{was 21.6}
$$

The drift of this short rate model is, as a function of $\{r(s)|0 \leq s \leq t\}$ , path-dependent. Only in high dimensions, namely as a function of $\{L_{i}(t)|i = 0, \ldots, n\}$ , will the model be Markovian (i.e. the drift is no longer path-dependent). 

CHAPTER 23. HEATH-JARROW-MORTON FRAMEWORK: IMMERSION OF SHORT RATE MODELS AND LIBOR MARKET MODEL 

# Excursus: Shape of the Interest Rate Curve under Mean Reversion and a Multi-Factor Model

In this chapter we are considering the influence of model properties like mean reversion, number of factors, instantaneous correlation and instantaneous volatility on the possible future shapes of the interest rate curve. 

As in Chapter 20, which discussed the relation of instantaneous correlation and instantaneous volatility to the terminal correlation, our goal is to develop an understanding of the significance of the model properties rather than looking at them rigorously in abstract mathematical terms. We thus pose the question of how the interest rate curve differs qualitatively under different model configurations. 

## 24.1. Model

As a model framework we will use the LIBOR Market Model. Due to its many parameters it gives us enough freedom to play with. We will restrict the set of parameters and concentrate on three (important) parameters that are sufficient to create the interesting phenomena we are interested in. 

Let us restrict the model to a simple volatility structure, namely 

$$
\sigma_ {i} (t) = \sigma^ {*} \cdot \exp (- a \cdot (T _ {i} - t))\tag{24.1}
$$

with $\sigma^{*} = 0.1$ and $a = 0.05$ . We will choose an equally simple correlation model, namely $\mathrm{d}W_{i}\mathrm{d}W_{j} = \rho_{i,j}\mathrm{d}t$ with 

$$
\rho_ {i, j} = \exp (- r \cdot | T _ {i} - T _ {j} |).\tag{24.2}
$$

To this correlation model we apply a factor reduction (Principal Component Analysis), see Appendix A.4. The number of factors is the number of independent Brownian motions (effectively) entering the model, see Definition 50. Upon a factor reduction the m largest eigenvalues of the correlation matrix are determined. Together with the corresponding eigenvectors a new correlation matrix is constructed, having at most m non-zero eigenvalues. This process guarantees that the resulting correlation model defines a valid correlation matrix. 

We simulate under the terminal measure and start with an initially flat interest rate curve $L_{i}(0) = 0.1$ , $i = 0, 1, 2, \ldots$ . 

To summarize, our model framework consists of three degrees of freedom which will be varied in our analysis: 

<table><tr><td>Parameter</td><td>Effect</td></tr><tr><td>a</td><td>Damping of the exponentially decaying, time-homogenous volatility</td></tr><tr><td>r</td><td>Damping of the exponentially decaying instantaneous correlation</td></tr><tr><td>m</td><td>Number of factors extracted from the correlation matrix</td></tr></table>


Table 24.1.: Free parameters of the LIBOR Market Model considered.


## 24.2. Interpretation of the Figures

The Figures 24.1, 24.2, 24.3 and 24.4 show 100 paths of a Monte-Carlo simulation of the interest rate curve. The simulation was frozen at a fixed point in time (t = 7.5 in 24.2, 24.3 and 24.4 and t = 17.5 in 24.1). To the left of this point the forward rates $L_{i}(T_{i})$ are shown, each upon their individual maturity, - this is a discrete analog of the short rate. To the right of this point the future forward rate curve $L_{j}(t)$ is drawn. 

The figures differ only in the parameters used to generate the paths. The same random numbers are used, thus the simulated paths depend smoothly on a and r. 

To improve the visibility of the individual paths, each path is given a different color, where the hue of the color depends smoothly on the level of the last rate $L_{n}(t)$ .¹ This makes its it very easy to check if the interest rate curves are parallel or exhibit some regular structure, see Figure 24.2. 

## 24.3. Mean Reversion

We will consider the example of a simple one-factor Brownian motion ( $\rho_{i,j}=1$ , i.e. r=0). Figure 24.1 shows the simulated forward rates for different parameters a in (24.1). 

From the derivation of the Hull-White-Model from the HJM-Framework it became obvious that an exponentially decreasing volatility structure of the forward rate corresponds to a mean reversion of the short rate, see page 289. We rediscover this property qualitatively here. Figure 24.1 shows 100 paths of a Monte-Carlo simulation of a LIBOR market model with different values for the parameter $a$ : $a = 0$ , $a = 0.05$ in the upper and $a = 0.1$ , $a = 0.15$ in the lower row (left to right). Observe the fixed rates $L_{i}(T_{i})$ left from the simulation time. They may be interpreted as a direct analog of the short rate. In Figure 24.1 it becomes obvious that with an increasing parameter $a$ the paths develop a tendency to revert to the mean (mean reversion). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/5dfef4ece1f16f44d2d05920822b2f7641f51d2dbc4a65ae14d4cadca3c3f84a.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/25b4d4b0403fa58801cc152bafdf2cc59f5ea87165a7478fd512d0be50a8942d.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/d88aa8846988205cb7f8330cd45b4d7490280e52995375a27ec11d94b06b9d69.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/b65f810bc28937b4dcb094785e1879fe3af2791634663620b1366571746e4f52.jpg)



Figure 24.1.: Shape of the fixed rates $L_{i}(T_{i})$ and the interest rate curve for different instantaneous volatilities (corresponds to different mean reversion) frozen at time t = 17.5 using a one-factor mode. We used a = 0 (upper left), a = 0.05 (upper right), a = 0.10 (lower left) and a = 0.15 (lower right). For interpretation see Section 24.3.


## 24.4. Factors

Figure 24.2 shows a Monte-Carlo simulation with the parameters above and varying numbers of factors m. The possible shapes of the interest rate curve are given by combinations of the factors parallel shift, tilt, bend and oscillations with increasing frequencies, see also Figure A.1 on Page 364. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/e8445f11ae639a40d0e553ffd5e49086d1d74efbaff8f94474ef564fe49f5331.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/1582be10da84bd09840a54225d5503ae11792b729767701209419086fcc7b8d1.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/9e314c3be7f077d541ef243a5656743262de289b0f77b7817ad343615355bd68.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/0a71db12e51006b71bb164d5e1c98c01dbfe7bc784a7d3d8b94813fd5a94a61e.jpg)



Figure 24.2.: Shape of the interest rate curve with different factor configurations, seen at time t = 7.5: One, two, three and five factors (from upper left to lower right). For interpretation see Section 24.4.


## 24.5. Exponential Volatility Function

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/b1950f9413171b36e263d9def25f679714820be1cf94e4300d1f72f1656798c4.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/3774e5da382fe3be4fc97803e4bee6fbddbfeac62d330f6134e17b43f8b684d0.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/13e52282e509d53819c50acdc786c6d9a888dfe9be8d83554c30759b07ae7726.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/10cd959d74fa0b11ae6b32a389f84a06dc1dcb3edecfba2c2a4268541a421320.jpg)



Figure 24.3.: Shape of the fixed rates $L_{i}(T_{i})$ and the interest rate curve with different instantaneous volatilities (corresponds to mean reversion) at time t = 7.5 in a one-factor model (upper row and lower left) with a = 0.0, a = 0.05 and a = 0.1 and a three-factor model (lower right) with a = 0.1. For interpretation see Section 24.5.


As in Figure 24.1 we consider the Monte-Carlo simulation under different parameters a. First a = 0, a = 0.05 and a = 0.1 in a one-factor model (r = 0, m = 1), and last a = 0.1 in a three-factor model. We are observing this at simulation time t = 7.5 and concentrate here on the section right of the simulation time, i.e. the interest rate curve $L_{j}(t)$ for $j > m(t)$ . 

It is apparent that the curve $\{L_{j}(t) \mid j > m(t)\}$ shows a shape similar to an exponential in j, depending on the parameter a, see Figure 24.3, lower left (a = 0.1) to the right of the simulation time. If we consider a one-factor model (as used in the figure), we have: 

$$
L _ {j} (t) = L _ {j} (0) \cdot \exp \left(\int_ {0} ^ {t} \mu_ {j} (\tau) \mathrm{d} \tau + \sqrt {\int_ {0} ^ {t} \sigma_ {j} (\tau)} \mathrm{d} \tau \cdot W (t)\right).
$$

For a fixed point in time $t$ (and a state (path) $\omega$ ) the interest rate curve shows the following dependence on $j$ 

$$
j \mapsto L _ {j} (0) \cdot \exp \left(\int_ {0} ^ {t} \mu_ {j} (\tau , \omega) \mathrm{d} \tau\right) \cdot \exp \left(k \cdot \sqrt {\int_ {0} ^ {t} \sigma_ {j} ^ {2} (\tau)} \mathrm{d} \tau\right)
$$

where $k := W(t, \omega)$ . 

For the volatility structure (24.1) particularly, we find 

$$
\begin{array}{r l} \int_ {0} ^ {t} \sigma_ {j} ^ {2} (\tau) & = \int_ {0} ^ {t} \exp (- 2 a (T _ {j} - \tau)) \mathrm{d} \tau \\ & = \frac {1}{2 a} \big (\exp (- 2 a (T _ {j} - t)) - \exp (- 2 a (T _ {j} - 0)) \big) \\ & = \frac {1}{2 a} \cdot (\exp (2 a \cdot t) - 1) \cdot \exp (- 2 a T _ {j}) \end{array}
$$

$$
i \mapsto L _ {j} (0) \cdot \exp \left(\int_ {0} ^ {t} \mu_ {j} (\tau , \omega) \mathrm{d} \tau\right) \cdot \exp \left(\tilde {k} \cdot \exp (- a T _ {j})\right),\tag{24.3}
$$

where $\tilde{k} = k\cdot \sqrt{\frac{1}{2a} (\exp(2a\cdot t) - 1)}.$ 

The drift $\int_{0}^{t}\mu_{j}(\tau,\omega)\mathrm{d}\tau$ is monotone increasing in j, see (19.8). This explains the shape of the interest rate curve in Figure 24.3 upper left. With increasing parameter a the interest rate curve is multiplied by the double exponential (24.3) with increasing steepness. This explains the shape of the interest rate curve in Figure 24.3 upper right and lower left. Only the addition of more driving factors allows for a richer family of possible curves. If the parallel movement (level) remains the dominant factor, then the shape (24.3) still dominates the interest rate curve, Figure 24.3 lower right. 

## 24.6. Instantaneous Correlation

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/e24ecb76def4f5051e858fdc351e8ee6891d8b79a19298044a290fcabda64632.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/30d47c94c20c811b1013e174debb2822fabfa9fc36fe18763107c4f70a1265d3.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/e661faec2977e5ac924f45be44f6333c84bfb0137ee1eb928714c1e0e21595ce.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/054d4a2a41ba6d8482f7de04dd4b7d9add490dda30a3eaa99525ff0b1fcae2f8.jpg)



Figure 24.4.: Shape of the fixed rates $L_{i}(T_{i})$ and the interest rate curve with different instantaneous correlations, seen at time t = 7.5. We used a correlation matrix with (all) 40 factors and r = 0.01 (upper left, high correlation), r = 0.1 (upper right) and r = 1.0 (lower left, high de-correlation). In the lower right we used a correlation matrix with r = 1.0 (the same as in lower left), but reduced the number of factors to three. For interpretation see Section 24.6.


We fix a slightly decreasing volatility structure (24.1) with $a = 0.1$ and vary the parameter $r$ of the correlation function (24.2). We do not apply a factor reduction, thus keep all 40 factors. The parameter $r = 0.01$ corresponds to an almost perfect correlation of the processes. Thus the possible shapes of the curve are almost parallel, the curve is very smooth since we started from a smooth (namely flat) curve. If the correlation parameter is increased to $r = 1.0$ , then the distribution of rates within the curve is almost independent. See Figure 24.4 upper left, upper right and lower left. 

It should be noted that this (terminal) de-correlation is also achievable under r = 0.01 by an appropriate choice of the volatility structure, see Chapter 20. The instantaneous de-correlation introduces an additional terminal de-correlation. The statement that a model with perfect instantaneous correlation exhibits perfect terminal de-correlation of the forward rates is wrong. 

Finally we have chosen in Figure 24.4 lower right the parameter r = 1.0 again (as for the lower left with strong de-correlation), but have applied a reduction to the three largest factors. It is obvious that this strongly reduces the possibility of de-correlation. The three factors only allow that the beginning, the middle and the end of the curve attain different values. Adjacent rates are still on similar levels. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/394e6fed8db4aebfd310d3bbdde28aeb6637a88e84c57ce409f4068f8522e9a5.jpg)


Experiment: At http://www.christian-fries.de/finmath/applets/LMMSimulation.html a simulation of an interest rate curve with the model framework above is to be found. The parameters may be chosen at will to study the different shapes of the interest rate curve. 

# Markov Functional Models

## 25.1. Introduction

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/2db5e0253d1c2ff308e0c221bdeb4ea74226de1188dd55485cca39c45a9496c0.jpg)


Motivation: From Chapter 5 we have a relation between the prices of European options and the probability distribution function (or probability density) of the underlying (under the martingale measure). If we consider a European option on some underlying, say the forward rate $L_{i} := L(T_{i}, T_{i+1}; T_{i})$ (i.e. a caplet), then 

Lemma 81 allows us to calculate the probability density of $L_{i}$ from the given market prices. It seems as if this allows perfect calibration of a “model” to a continuum of given market prices. However, the terminal distribution alone does not determine a pricing model. What is missing is the specification of the dynamics, i.e. the specification of transition probabilities, and, of course, the specification of the numéraire. This is the motivation for the Markov functional modeling. There we postulate a simple Markov process, e.g. $\mathrm{d}x = \sigma(t)\mathrm{d}W(t)$ for which the distribution function $\xi \mapsto P(x(T) \leq \xi)$ is known analytically. Then we require the underlying $L_{i}$ to be a function of $x(T_{i})$ . Let us denote this function by $g_{i}$ , i.e. let $L_{i}(\omega) = g_{i}(x(T_{i}, \omega))$ for all paths $\omega$ . If the functional $g_{i}$ is strictly monotone, then with $K = g_{i}(\xi)$ 

$$
\begin{array}{c} F _ {L _ {i}} (K) := P (L _ {i} \leq K) = P (g _ {i} (x (T)) \leq K) \\ = P (x (T) \leq \xi) =: F _ {x (T _ {i})} (\xi) = F _ {x (T _ {i})} (g _ {i} ^ {- 1} (K)). \end{array}
$$

With a given distribution function $F_{L_{i}}$ of $L_{i}$ (e.g. extracted from market prices through Lemma 81), the choice of the functional $g_{i}$ allows the calibration to the distribution of $L_{i}$ , while the process x (and the sequence of functionals $\{g_{i}\}$ ) describe the dynamics. To achieve a fully specified pricing model we further require the specification of the numéraire as function of the Markov process x. To achieve this we may use Theorem 79, if 

- $x$ is given under the equivalent martingale measure $\mathbb{Q}$ and 

- $x$ generates the filtration. 

Given a filtered probability space $(\mathbb{R}, \mathcal{B}(\mathbb{R}), \mathbb{Q}, \{\mathcal{F}_{t}\})$ . Consider a time-discretization $0 = T_{0} < T_{1} < \ldots < T_{n}$ . Financial products beyond $T_{n}$ are not considered. 

Let $t \mapsto N(t)$ denote the price process of a traded asset, which we choose as numéraire and let $\mathbb{Q}$ denote the corresponding equivalent martingale measure. Then for any replicable asset price process $V(t)$ (see Definition 73 and Theorem 79) 

$$
\frac {V (T _ {i})}{N (T _ {i})} = \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {V (T _ {k})}{N (T _ {k})} | \mathcal {F} _ {T _ {i}}).
$$

In particular for every zero coupon bond $P(T_{k})$ , paying 1 in $T_{k}$ 

$$
\begin{array}{l} \frac {P (T _ {k} ; T _ {i})}{N (T _ {i})} = \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {1}{N (T _ {k})} | \mathcal {F} _ {T _ {i}}), \text {d.h.} \\ P (T _ {k}; T _ {i}) = N (T _ {i}) \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {1}{N (T _ {k})} | \mathcal {F} _ {T _ {i}}). \end{array}
$$

Let $x$ denote a $\mathcal{F}_t$ -adapted stochastic process with 

$$
\mathrm{d} x (t) = \sigma (t) \mathrm{d} W (t), \quad x (0) = x _ {0}.
$$

The filtration should be generated by $x$ . On this space we consider time-discrete stochastic processes, namely those for which their $T_{i}$ -realization is a function of $(x(T_0),\ldots ,x(T_i))$ , for all $i$ . We particularly consider processes for which their time $T_{i}$ -realization is a function of $x(T_{i})$ alone (i.e. independent of the process's history). 

## 25.1.1. The Markov Functional Assumption (independent of the model considered)

We assume that the time $T_{i}$ -realization of the numéraire process is a function of $x(T_{i})$ , i.e. 

$$
N (T _ {i}, \omega) = N (T _ {i}, x (T _ {i}, \omega)),\tag{25.1}
$$

where we use the same letter $N$ for the (deterministic) functional $\xi \mapsto N(T_i, \xi)$ . 

Then, for any payoff $V(T_{k})$ that is itself a function of $x(T_{k})$ for some k, the value process $V(T_{i})$ for $i \leq k$ is 

$$
V (T _ {i}) = N (T _ {i}) \mathrm{E} \left(\frac {V (T _ {k})}{N (T _ {k})} | \mathcal {F} _ {T _ {i}}\right) = N (T _ {i}, x (T _ {i})) \mathrm{E} \left(\frac {V (T _ {k} , x (T _ {k}))}{N (T _ {k} , x (T _ {k}))} | \sigma (x (T _ {i}))\right).
$$

Thus, the time $T_{i}$ realization of the value process $V(T_{i})$ is also a functional of $x(T_{i})$ which we denote by the same letter $V$ . The functional $\xi \mapsto V(T_{i},\xi)$ of the value process is 

$$
\xi \mapsto N (T _ {i}, \xi) \mathrm{E} \left(\frac {V (T _ {k} , x (T _ {k}))}{N (T _ {k} , x (T _ {k}))} | \{x (T _ {i}) = \xi \}\right).
$$

Note: The markov functional assumption (25.1) may be relaxed such that the numéraire is allowed to depend on $x(T_{0}),\ldots,x(T_{i})$ . This relaxation is used in the LIBOR Markov Functional Model in spot measure. 

## 25.1.2. Outline of this Chapter

In 25.2 we consider a Markov Functional Model for a stock (or any other non-interest rate related (single) asset). In 25.3 we will then consider a Markov Functional Model for the forward rate $L(T_{i}, T_{i+1}; T_{i})$ , which may be viewed as a time-discrete analog of the short rate. Both sections are essentially independent of each other. In Section 25.4 we will discuss how to implement a Markov functional model using a lattice in the state space. 

## 25.2. Equity Markov Functional Model

## 25.2.1. Markov Functional Assumption

Consider a simple one-dimensional Markov process, e.g. 

$$
\mathrm{d} x (t) = \sigma (t) \cdot \mathrm{d} W ^ {\mathbb {Q}} (t), \quad x (0) = x _ {0},\tag{25.2}
$$

where $\sigma$ is a deterministic function and $W^{Q}$ denotes a Q-Brownian motion. Without loss of generality we may assume $x_{0}=0$ . Equation (25.2) is the most simple choice of a Markovian driver process. We will consider the addition of a drift term to (25.2) in our discussion of model dynamics in Section 25.2.5. 

Let $S(t)$ denote the time t value of some asset for which we assume that we have a continuum of European option prices. Let x and S be adapted stochastic processes defined on $(\Omega, \mathbb{Q}, \mathcal{F}_t)$ , where $\{\mathcal{F}_t\}$ denotes the filtration generated by $W^{\mathbb{Q}}$ . 

We assume that the time t value of the asset S is a function of $x(t)$ , i.e. we assume the existence of a functional $(t,\xi)\mapsto S(t,\xi)$ such that 

$$
S (t, \omega) = S (t, x (t, \omega)),
$$

where the left hand side denotes our asset value at time t on path $\omega$ and the right hand side denotes some functional of our Markovian driver x, which we ambiguously name S. We allow some ambiguity in notation here. From here on S will also denote a deterministic mapping (the functional) 

$$
(t, \xi) \mapsto S (t, \xi).
$$

It will be clear from the arguments of $S$ if we speak of the functional $(t, \xi) \mapsto S(t, \xi)$ or of the process $t \mapsto S(t)$ . 

For $t_1 < t_2$ we trivially have that 

$$
\frac {S (t _ {1})}{S (t _ {1})} = \mathrm{E} ^ {\mathbb {Q}} (\frac {S (t _ {2})}{S (t _ {2})} \mid \mathcal {F} _ {t _ {1}}).
$$

We now postulate that $\mathbb{Q}$ is the equivalent martingale measure with respect to the Numéraire $S$ and that a universal pricing theorem holds for all other traded products, i.e. that their $S$ relative price is a $\mathbb{Q}$ -martingale. 

This implies that the zero coupon bond $P(T; t)$ having maturity $T$ and being observed in $t < T$ fulfills 

$$
\frac {P (T ; t)}{S (t)} = \mathrm{E} ^ {\mathbb {Q}} (\frac {1}{S (T)} \mid \mathcal {F} _ {t}).
$$

Using the functional representation of S we find that $P(T; t)$ is represented as a functional of $x(t)$ too, namely 

$$
(t, \xi) \mapsto P (T; t)
$$

with 

$$
\frac {P (T ; t , \xi)}{S (t , \xi)} = \mathrm{E} ^ {\mathbb {Q}} (\frac {1}{S (T , x (T))} \mid \{x (t) = \xi \}).\tag{25.3}
$$

## 25.2.2. Example: The Black-Scholes Model

Let us assume a Markovian driver with constant instantaneous volatility $\sigma(t) = \sigma$ . For the Black-Scholes Model we have 

$$
S (t, \xi) = S (0) \cdot \exp \big (r \cdot t + \frac {1}{2} \sigma_ {\mathrm{BS}} ^ {2} t + \frac {\sigma_ {\mathrm{BS}}}{\sigma} \cdot \xi \big),\tag{25.4}
$$

where $\sigma_{BS}$ denotes the (constant) Black-Scholes volatility. Plugging this into (25.3) we find 

$$
P (T; t, \xi) = \exp (- r (T - t)),
$$

so that interest rates are indeed deterministic here. 

This is the Black-Scholes model: From the definition of the Markovian driver we have $\frac{1}{\sigma} \cdot x(t) = W(t)$ and thus 

$$
S (t, x (t)) = S (0) \cdot \exp \left(r \cdot t + \frac {1}{2} \sigma_ {\mathrm{BS}} ^ {2} t + \sigma_ {\mathrm{BS}} \cdot W (t)\right).
$$

In other words, the $\mathbb{Q}$ dynamics of $S$ is<sup>1</sup> 

$$
\mathrm{d} S (t) = r S (t) \mathrm{d} t + \sigma_ {\mathrm{BS}} ^ {2} S (t) \mathrm{d} t + \sigma_ {\mathrm{BS}} S (t) \cdot \mathrm{d} W ^ {\mathbb {Q}} (t).
$$

Introducing a new Numéraire 

$$
\mathrm{d} B (t) = r B (t) \mathrm{d} t, \quad B (0) = 1
$$

we find for the change of Numéraire process $\frac{S}{B}$ that 

$$
\mathrm{d} \frac {S}{B} = \sigma_ {\mathrm{BS}} ^ {2} S (t) \mathrm{d} t + \sigma_ {\mathrm{BS}} S (t) \cdot \mathrm{d} W ^ {\mathbb {Q}} (t).
$$

For $\frac{S}{B}$ to be a martingale under $Q^{B}$ it has to be $\mathrm{d}W^{\mathbb{Q}}(t)=\mathrm{d}W^{\mathbb{Q}^{\mathbb{B}}}-\sigma_{\mathrm{BS}}^{2}\mathrm{d}t$ and thus 

$$
\begin{array}{l} \mathrm{d} S (t) = r S (t) \mathrm{d} t + \sigma_ {\mathrm{BS}} \cdot S (t) \cdot \mathrm{d} W ^ {\mathbb {Q} ^ {\mathbb {B}}} (t) \\ \mathrm{d} B (t) = r B (t) \mathrm{d} t. \end{array}
$$

Note: $\mathrm{d}W^{\mathbb{Q}}(t)$ is a Q Brownian motion, where Q is the equivalent martingale measure with respect to the Numéraire S, while $\mathrm{d}W^{\mathbb{Q}^{B}}(t)$ is a $Q^{B}$ Brownian motion, where $Q^{B}$ is the equivalent martingale measure with respect to the Numéraire B. 

## 25.2.3. Numerical Calibration to a Full Two-Dimensional European Option Smile Surface

As for the interest rate Markov functional model we are able to calculate the functionals numerically from a given two-dimensional smile surface. Our approach here is similar to the approach for the one-dimensional LIBOR Markov functional model under spot measure, [67]. Consider the following time $T$ payout: 

$$
V (T, K; T) := \left\{ \begin{array}{l l} S (T) & \text { if } S (T) > K \\ 0 & \text { otherwise. } \end{array} \right.\tag{25.5}
$$

$^{1}$ Note that Q is the equivalent martingale measure with respect to the Numéraire S. 

Obviously 

$$
V (T, K; T) = \max (S (T) - K, 0) + K \cdot \left\{ \begin{array}{l l} 1 & \text { if } S (T) > K \\ 0 & \text { else }, \end{array} \right.
$$

i.e. the value of V is given by the value of a portfolio of one call option and K digital options, all having strike K. This is our calibration product. 

## 25.2.3.1. Market Price

Let $\bar{\sigma}_{\mathrm{BS}}(T,K)$ denote the Black-Scholes implied volatility surface given by market prices. Then the market price of V is 

$$
\begin{array}{l} V ^ {\text { market }} (T, K; 0) = \underbrace {S (0) \Phi (d _ {+}) - \exp (- r T) K \Phi (d _ {-})} _ {\text { call   option   part }} \\ \qquad + K \underbrace {\exp (- r T) (\Phi (d _ {-}) + S (0) \sqrt {T} \Phi^ {\prime} (d _ {+}) \frac {\partial \bar {\sigma} _ {\text { BS }} (T , K)}{\partial K}} _ {\text { digital   part }} \\ \qquad = S (0) \Phi (d _ {+}) + K S (0) \sqrt {T} \Phi^ {\prime} (d _ {+}) \frac {\partial \bar {\sigma} _ {\text { BS }} (T , K)}{\partial K}, \end{array}
$$

where $\Phi(x) := \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{x} \exp(-\frac{y^2}{2}) \, \mathrm{d}y$ and $d_\pm = \frac{\ln(\frac{\exp(rT)S(0)}{K}) \pm \frac{1}{2} \bar{\sigma}_{\mathrm{BS}}^2(T,K)T}{\bar{\sigma}_{\mathrm{BS}}(T,K) \sqrt{T}}$ . 

## 25.2.3.2. Model Price

Within our model the price of the product (25.5) is 

$$
\begin{array}{l} V ^ {\text { model }} (T, K; 0) = S (0) \cdot \mathrm{E} ^ {\mathbb {Q}} (\frac {S (T , x (T)) \cdot \mathbf {1} _ {\{S (T , x (T)) > K \}}}{S (T)} \mid \{x (0) = x _ {0} \}) \\ = S (0) \cdot \mathrm{E} ^ {\mathbb {Q}} (\mathbf {1} _ {\{S (T, x (T)) > K \}} \mid \{x (0) = x _ {0} \}) \end{array}
$$

Assuming that our functional $(T,\xi)\mapsto S(T,\xi)$ is monotonely increasing in $\xi$ we may write 

$$
V ^ {\mathrm{model}} (T, K; 0) = S (0) \cdot \mathrm{E} ^ {\mathbb {Q}} \big (\mathbf {1} _ {\{x (T) > x ^ {*} \}} \mid \{x (0) = x _ {0} \} \big),\tag{25.6}
$$

where $x^{*}$ is the (unique) solution of $S(T, x^{*}) = K$ . Note that (25.6) depends on $x^{*}$ and the probability distribution of $x(T)$ only and that $x(T)$ is known due to the simple form of our Markovian driver. It does not depend on the functional $S!$ Thus for given $x^{*}$ we can calculate 

$$
V ^ {\mathrm{model}} (T, x ^ {*}; 0) := S (0) \cdot \mathrm{E} ^ {\mathbb {Q}} (\mathbf {1} _ {\{x (T) > x ^ {*} \}} \mid \{x (0) = x _ {0} \}).
$$

## 25.2.3.3. Solving for the Functional

For given $x^{*}$ we now solve the equation 

$$
V ^ {\text { market }} (T, K ^ {*}; 0) = V ^ {\text { model }} (T, x ^ {*}; 0)
$$

to find $S(T, x^{*}) = K^{*}$ and thus the functional form $(T, \xi) \mapsto S(T, \xi)$ . This can be done very efficiently using fast one-dimensional root finders, e.g. Newton's method. 

## 25.2.4. Interest Rates

## 25.2.4.1. A Note on Interest Rates and the No-Arbitrage Requirement

Functional models for equity option pricing have been investigated before, see e.g. $[57]$ and references therein. However, the approach considered there chooses deterministic interest rates and the bank account as Numéraire. As suggested in Section 25.2.2, this will impose a very strong self-similarity requirement on the functionals (which is fulfilled by the Black-Scholes model). Such models may calibrate only to a one-dimensional sub-manifold of a given implied volatility surface, see $[58]$ . For the Markov functional model this follows directly from $(25.3)$ . Assuming that the Markovian driver x is given and that the interest rate dynamic $P(T;t,\xi)$ is given, we find from $(25.3)$ that 

$$
S (t, \xi) = \frac {P (T ; t , \xi)}{\mathrm{E} ^ {\mathbb {Q}} (\frac {1}{S (T , x (T))} \mid \{x (t) = \xi \})}.
$$

So once a terminal time T functional $\xi \mapsto S(T, \xi)$ has been defined, all other functionals are implied by the interest rate dynamics P and the dynamics of the Markovian driver. 

Sticking to prescribed interest rates, the only way to allow for more general functional is to violate the no-arbitrage requirement $(25.3)$ or change the Markovian driver. The latter will be considered in Section 25.2.5. 

## 25.2.4.2. Where are the Interest Rates?

Our model calibrates to a continuum of options on S. We do not even specify interest rates. This is not necessary, since the specification of the interest rates is already contained in the specification of a continuum of options on S. Consider options on $S(T)$ , i.e. options with maturity T. First note that from a continuum $K \mapsto V_{\text{call}}^{\text{market}}(T, K; 0)$ of market prices for call option payouts 

$$
V _ {\mathrm{call}} ^ {\mathrm{market}} (T, K; T) = \max (S (T) - K, 0)
$$

we obtain prices for the corresponding digital payouts 

$$
V _ {\text { digital }} ^ {\text { market }} (T, K; T) = \left\{ \begin{array}{l l} 1 & \quad S (T) > K \\ 0 & \quad \text { else } \end{array} \right.
$$

by 

$$
V _ {\text { digital }} ^ {\text { market }} (T, K; 0) = - \frac {\partial}{\partial K} V _ {\text { call }} ^ {\text { market }} (T, K; 0).
$$

Thus the value of the zero coupon bond with maturity T is 

$$
P (T; 0) = \lim _ {K \searrow 0} V _ {\text { digital }} ^ {\text { market }} (T, K; 0) = - \lim _ {K \searrow 0} \frac {\partial}{\partial K} V _ {\text { call }} ^ {\text { market }} (T, K; 0).\tag{25.7}
$$

Note that this argument is model-independent. 

Within the functional model, Equation (25.7) holds locally in each state. Given that we are at time t in state $x(t) = \xi$ we have for the corresponding bond 

$$
P (T; t, \xi) = \lim _ {K \searrow 0} V _ {\text { digital }} ^ {\text { model }} (T, K; t, \xi).
$$

From this it becomes clear why specifying interest rates would represent a violation of the no-arbitrage requirement. $^{2}$ 

In the next section we show that the model implied interest rate dynamics are likely to be undesirable. However, as is known from interest rate hybrid Markov functional models $[67]$ , it is possible to calibrate to different model dynamics by changing the Markovian driver x. 

## 25.2.5. Model Dynamics

## 25.2.5.1. Introduction

Markov functional models calibrate perfectly to a continuum of option prices, i.e. to the market implied probability density of the underlying, cf. [52]. Indeed, the functional $(t,\xi)\mapsto S(t,\xi)$ is nothing more than the transformation of the measure from the probability density of $x(t)$ to the market implied probability density of the underlying $S(t)$ . 

While calibration to terminal probability densities is a desirable feature, it is not the only requirement imposed on a model, specifically if the model is used to price complex derivatives like Bermudan options. Here the transition probabilities play a role, i.e. the model dynamics. The most prominent aspects of model dynamics are 

- Interest Rate Dynamics: For an equity Markov functional model the joint movement of the interest rate and the asset has to be analysed. It is possible to calibrate to given interest rate dynamics by adding a drift to the Markovian driver, see Section 25.2.5.2. 

- Forward volatility: This is the implied volatility of an option with maturity T and strike K, given we are in state $(t, \xi)$ , i.e. 

$$
S (t, \xi) \cdot \mathrm{E} ^ {\mathbb {Q}} (\frac {\max (S (T , x (T)) - K , 0)}{S (T)} | \{x (t) = \xi \}).
$$

Obviously it will play an important role for compound options and Bermudan options. The forward volatility may be calibrated by changing the instantaneous volatility of the Markovian driver, see Section 25.2.5.3. 

- Auto correlation / Forward spread volatility: The auto correlation of the process S impacts the forward spread volatility. This is the implied volatility of an option on $S(T_{2}) - S(T_{1})$ with maturity $T_{2}$ , given we are in state $(t, \xi)$ , i.e. 

$$
S (t, \xi) \cdot \mathrm{E} ^ {\mathbb {Q}} (\frac {\max (S (T _ {2} , x (T _ {2})) - S (T _ {1} , x (T _ {1})) , 0)}{S (T _ {2} , x (T _ {2}))} \mid \{x (t) = \xi \}).
$$

Markov functional models allow limited calibration to different model dynamics by changing the dynamics of the Markovian driver x. For our choice 

$$
\mathrm{d} x = \sigma (t) \cdot \mathrm{d} W (t)
$$

we can change the auto-correlation of x by choosing different instantaneous volatility functions $\sigma$ . Since the calibration of the functionals is scale invariant with respect to the terminal standard deviation $\bar{\sigma}(t)$ of $x(t)$ , the calibration to the terminal probability densities is independent of the choice of $\sigma$ . See the Black-Scholes example in Section 25.2.2 for an example of this invariance. 

## Time Copula

The specification of the auto-correlation of x (through $\sigma$ ) is sometimes called time copula, [57], since it may be specified through the joint distribution of $(x(t_{1}), x(t_{2}))$ . For this reason similar functional models are sometimes called copula models, a term that is more associated with credit models, where joint default distribution is constructed from marginal default distributions. 

In addition to a specification of the instantaneous volatility, the Markovian driver may be endowed with a drift. 

## Time-Discrete Markovian Driver

We assume a given time discretization $\{0 = t_{0} < t_{1} < t_{2} < \ldots\}$ and consider the realizations $x(t_{i})$ of the Markovian driver x given by increments $\Delta x(t_{i}) = x(t_{i+1}) - x(t_{i})$ . It is natural that a practical implementation of the model will feature a certain time discretization. Thus, speaking of calibration of a specific time-discretized implementation, it is best to consider the Markovian driver given by an Euler scheme (as in (25.8), (25.9)) 

$$
x (t _ {i + 1}) = x (t _ {i}) + \mu (t _ {i}, x (t _ {i})) \Delta t _ {i} + \sigma (t _ {i}, x (t _ {i})) \Delta W (t _ {i}).
$$

## 25.2.5.2. Interest Rate Dynamics

## Example: Black-Scholes Model with a Term Structure of Volatility

Let us first assume that the Markovian driver is given by 

$$
x (t _ {i + 1}) = x (t _ {i}) + \sigma_ {i} \Delta W (t _ {i}).\tag{25.8}
$$

Consider a term structure of Black-Scholes implied volatilities, i.e. let $\bar{\sigma}_{\mathrm{BS}}(t_{i})$ denote the implied volatility of an option with maturity $t_{i}$ . With the simple Markovian driver (25.8), the corresponding functionals that calibrate to these options are 

$$
S (t _ {i}, \xi) = S (0) \cdot \exp \big (r \cdot t _ {i} + \frac {1}{2} \bar {\sigma} _ {\mathrm{BS}} (t _ {i}) ^ {2} t + \frac {\bar {\sigma} _ {\mathrm{BS}} (t _ {i})}{\bar {\sigma} _ {i}} \cdot \xi \big),
$$

where $\bar{\sigma}_i^2 := \frac{1}{t_i} \sum_{j=0}^{i-1} \sigma_j^2 \Delta t_j$ . 

Within this model a stochastic interest rate dynamic is already implied. From $(25.3)$ we find 

$$
\begin{array}{r l} P (t _ {i + 1}; t _ {i}, \xi) & = S (t _ {i}, \xi) \cdot \mathrm{E} ^ {\mathbb {Q}} (\frac {1}{S (t _ {i + 1} , x (t _ {i + 1}))} \mid \{x (t _ {i}) = \xi \}) \\ & = \exp (- r \cdot (t _ {i + 1} - t _ {i}) - \frac {1}{2} (\bar {\sigma} _ {\mathrm{BS}} (t _ {i + 1}) ^ {2} \cdot (t _ {i + 1} - \frac {\sigma_ {i} ^ {2}}{\bar {\sigma} _ {i + 1} ^ {2}} \Delta t _ {i}) - \bar {\sigma} _ {\mathrm{BS}} (t _ {i}) ^ {2} \cdot t _ {i}) \\ & \qquad - (\frac {\bar {\sigma} _ {\mathrm{BS}} (t _ {i + 1})}{\bar {\sigma} _ {i + 1}} - \frac {\bar {\sigma} _ {\mathrm{BS}} (t _ {i})}{\bar {\sigma} _ {i}}) \cdot \xi), \end{array}
$$

If the volatility of the Markovian driver x decays faster than the implied Black-Scholes volatility, then the interest rate will move positively correlated with the stock. If the volatility of the Markovian driver x decays slower than the implied Black-Scholes volatility, then the interest rate will move in a negatively correlated way. $^{3}$ If we choose the instantaneous volatility of x such that $\bar{\sigma}_{i} = \bar{\sigma}_{\mathrm{BS}}(t_{i})$ , 

$$
P (t _ {i + 1}; t _ {i}, \xi) = \exp (- r \cdot (t _ {i + 1} - t _ {i})),
$$

i.e. we have recovered a model with deterministic interest rates. Reconsidering the case of a continuous driver $\mathrm{d}x = \sigma(t)\mathrm{d}W(t)$ , we see that for $\frac{1}{t}\int_{0}^{t}\sigma(\tau)^{2}\mathrm{d}\tau = \bar{\sigma}_{\mathrm{BS}}(t)^{2}$ the functionals above define a Black-Scholes model with instantaneous volatility $\sigma$ . 

However, we do not need to sacrifice the instantaneous volatility of x to match the interest rate dynamics. A much more natural choice is to add a suitable drift to the Markovian driver x. Consider a Markovian driver x such that 

$$
x (t _ {i + 1}) = x (t _ {i}) + \alpha_ {i} x (t _ {i}) \Delta t _ {i} + \sigma_ {i} \Delta W (t _ {i}), \qquad x (t _ {0}) = x _ {0} = 0.\tag{25.9}
$$

Note that the $x(t_i)$ 's are normally distributed with mean 0 (assuming $x_0 = 0$ ) and standard deviations $\gamma_i\sqrt{t_i}$ where 

$$
\gamma_ {i + 1} ^ {2} t _ {i + 1} = \gamma_ {i} ^ {2} t _ {i} \cdot (1 + \alpha_ {i} \Delta t _ {i}) + \sigma_ {i} ^ {2} \Delta t _ {i}.
$$

Together with the functionals 

$$
\begin{array}{r l} {S (t _ {i}, \xi) = S (0) \cdot \exp (r \cdot t _ {i} + \frac {1}{2} \bar {\sigma} _ {\mathrm{BS}} (t _ {i}) ^ {2} + \frac {\bar {\sigma} _ {\mathrm{BS}} (t _ {i})}{\gamma_ {i}} \cdot \xi)} \\ {S (t _ {i + 1}, \xi) = S (0) \cdot \exp (r \cdot t _ {i + 1} + \frac {1}{2} \bar {\sigma} _ {\mathrm{BS}} (t _ {i + 1}) ^ {2} + \frac {\bar {\sigma} _ {\mathrm{BS}} (t _ {i + 1})}{\gamma_ {i + 1}} \cdot \xi)} \end{array}
$$

we have 

$$
\begin{array}{l} P (t _ {i + 1}; t _ {i}, \xi) = S (t _ {i}, \xi) \cdot \mathrm{E} ^ {\mathbb {Q}} (\frac {1}{S (t _ {i + 1} , x (t _ {i + 1}))} \mid \{x (t _ {i}) = \xi \}) \\ = \exp (- r \cdot \Delta t _ {i} - \frac {1}{2} (\bar {\sigma} _ {\mathrm{BS}} (t _ {i + 1}) ^ {2} \cdot (t _ {i + 1} - \frac {\sigma_ {i} ^ {2}}{\gamma_ {i + 1} ^ {2}} \Delta t _ {i}) - \bar {\sigma} _ {\mathrm{BS}} (t _ {i}) ^ {2} \cdot t _ {i}) \\ \qquad - (\frac {\bar {\sigma} _ {\mathrm{BS}} (t _ {i + 1})}{\gamma_ {i + 1}} (1 + \alpha_ {i} \Delta t _ {i}) - \frac {\bar {\sigma} _ {\mathrm{BS}} (t _ {i})}{\gamma_ {i}}) \cdot \xi) \\ = \exp (- r \cdot \Delta t _ {i} - \frac {1}{2} (\bar {\sigma} _ {\mathrm{BS}} (t _ {i + 1}) ^ {2} \cdot \frac {\gamma_ {i} ^ {2}}{\gamma_ {i + 1} ^ {2}} (1 + \alpha_ {i} \Delta t _ {i}) ^ {2} - \bar {\sigma} _ {\mathrm{BS}} (t _ {i}) ^ {2} \cdot t _ {i}) \\ \qquad - (\frac {\bar {\sigma} _ {\mathrm{BS}} (t _ {i + 1})}{\gamma_ {i + 1}} (1 + \alpha_ {i} \Delta t _ {i}) - \frac {\bar {\sigma} _ {\mathrm{BS}} (t _ {\mathrm{i}})}{\gamma_ {i}}) \cdot \xi). \end{array}
$$

Choosing $\alpha_{i}$ such that 

$$
(\frac {\bar {\sigma} _ {\mathrm{BS}} (t _ {i + 1})}{\gamma_ {i + 1}} (1 + \alpha_ {i} \Delta t _ {i}) - \frac {\bar {\sigma} _ {\mathrm{BS}} (t _ {i})}{\gamma_ {i}}) = 0\tag{25.10}
$$

we have 

$$
P (t _ {i + 1}; t _ {i}, \xi) = \exp (- r \cdot (t _ {i + 1} - t _ {i})).
$$

Interestingly, the Markov functional model (25.9)-(25.10) does not necessarily need to be a Black-Scholes model having the $\mathbb{Q}^{\mathbb{B}}$ -dynamics 

$$
\begin{array}{l} \mathrm{d} S (t) = r S (t) \mathrm{d} t + \sigma_ {\mathrm{BS}} (t) \cdot S (t) \cdot \mathrm{d} W ^ {\mathbb {Q} ^ {\mathbb {B}}} (t) \\ \mathrm{d} B (t) = r B (t) \mathrm{d} t, \end{array}\tag{25.11}
$$

$^{3}$ Note that on average the interest rate is still r. 

where $\bar{\sigma}_{\mathrm{BS}}(t_{i})^{2} = \frac{1}{t_{i}} \int_{0}^{t_{i}} \sigma_{\mathrm{BS}}(t)^{2} \, dt$ . The two models are not the same, although their terminal probability densities (European option prices) and their interest rate dynamics agree. The difference lies in the forward volatility, which may be changed for the Markov functional model by the instantaneous volatility of x. Only for $\sigma(t) = \sigma_{\mathrm{BS}}(t)$ we have the dynamics (25.11). In this case the $\alpha_{i}$ in (25.10) will be zero, i.e. we are in the situation of the previous example. 

## Calibration to arbitrary Interest Rate Dynamics

Within the no-arbitrage constraints, it is possible to calibrate the model to a given arbitrary interest rate dynamics by choosing the appropriate drift. To do so, we have to find $\mu(t_{i},\xi)$ such that 

$$
P (t _ {i + 1}; t _ {i}, \xi) = \mathrm{E} ^ {\mathbb {Q}} (\frac {S (t _ {i} , \xi)}{S (t _ {i + 1} , x (t _ {i + 1}))} | \{x (t _ {i}) = \xi - \mu (t _ {i}, \xi) \Delta t _ {i} \}).
$$

This can be done numerically by means of a one-dimensional root finder. The functional $S(t_{i+1})$ has to be re-calibrated in every iteration. $^{4}$ 

## 25.2.5.3. Forward Volatility

The calibration to European option prices (Section 25.2.3) and joint movements of asset and interest rates (Section 25.2.5.2) still leaves the instantaneous volatility $\sigma$ of the Markovian driver $x$ a free parameter. It may be used to calibrate the forward volatility, i.e. the volatility of an option, conditionally we are at time $t > 0$ in state $\xi$ . 

## Example: Black-Scholes Model with a Term Structure of Volatility

Consider the simple Black-Scholes-like example from Section 25.2.5.2. For simplicity we consider a Markovian driver without drift, i.e. 

$$
x (t _ {i + 1}) = x (t _ {i}) + \sigma_ {i} \Delta W (t _ {i}).
$$

together with functionals 

$$
S (t _ {i}, \xi) = S (0) \cdot \exp \left(r \cdot t _ {i} + \frac {1}{2} \bar {\sigma} _ {\mathrm{BS}} (t _ {i}) ^ {2} t + \frac {\bar {\sigma} _ {\mathrm{BS}} (t _ {i})}{\bar {\sigma} _ {i}} \cdot \xi\right)
$$

calibrating to European options with implied volatility $\bar{\sigma}_{\mathrm{BS}}(t_{i})$ .⁵ 

Then we have that the standard deviation of the increment $x(t_k) - x(t_i)$ is $\bar{\sigma}_{t_i,t_k} \cdot \sqrt{(t_k - t_i)}$ , where $\frac{1}{t_k - t_i} \sum_{j=i}^{k-1} \sigma_j^2 \Delta t_j$ . It follows that the implied volatility of an option with maturity $t_k$ , given we are in state $(t_i, \xi)$ , is 

$$
\bar {\sigma} _ {\mathrm{BS}} (t _ {k}) \cdot \frac {\bar {\sigma} _ {t _ {i} , t _ {k}}}{\bar {\sigma} _ {t _ {k}}}.
$$

Thus a decay in the instantaneous volatility of the driver process will result in a forward volatility decaying with simulation time $t_{i}$ (for fixed maturity $t_{k}$ ). 

## Example: Exponential Decaying Instantaneous Volatility

Consider the case of a time continuous Markovian driver $dx = \sigma(t)\mathrm{d}W$ with decaying instantaneous volatility 

$$
\sigma (t) = \exp (- a \cdot t), \quad a \neq 0.
$$

Then $\bar{\sigma}_{t_1,t_2}:=\sqrt{\frac{1}{t_2-t_1}\int_{t_1}^{t_2}\sigma(t)\mathrm{d}t}=\sqrt{\frac{-1}{2a(t_2-t_1)}(\exp(-2at_2)-\exp(-2at_1))}$ . Assuming functionals 

$$
S (t, \xi) = S (0) \cdot \exp \left(r \cdot t + \frac {1}{2} \bar {\sigma} _ {\mathrm{BS}} (t) ^ {2} t + \frac {\bar {\sigma} _ {\mathrm{BS}} (t)}{\bar {\sigma} (0 , t)} \cdot \xi\right)
$$

the forward volatility for an option with maturity T, given we are in t, is 

$$
\bar {\sigma} _ {\mathrm{BS}} (T) \cdot \frac {\bar {\sigma} (t , T)}{\bar {\sigma} (0 , T)} = \bar {\sigma} _ {\mathrm{BS}} (T) \cdot \sqrt {\frac {T}{T - t} \frac {\exp (- 2 a t) - \exp (- 2 a T)}{1 - \exp (- 2 a T)}}.
$$

## 25.2.6. Implementation

The model may be implemented in the same way as is done for a one-dimensional Markov functional LIBOR model. The basic steps for a numerical implementation are, see Figure 25.1: 

- Choose a suitable discretization of $(t, x(t))$ , i.e. set up a grid $(t_i, x_{i,j})$ . 

- For each $x^{*} = x_{i,j}$ : 

- Calculate $V^{\mathrm{model}}(T, x^{*}; 0)$ . 

- Find $K^*$ such that $V^{\mathrm{market}}(T, K^*; 0) = V^{\mathrm{model}}(T, x^*; 0)$ . 

$$
- \text {   Set   } S (x _ {i, j}) := K ^ {*}.
$$

See Section 25.4. 

## 25.3. LIBOR Markov Functional Model

We postulate that the forward rate viewed on its reset date (fixing) may be given as a function of the realization of the underlying Markov process x: 

$$
\text { The   forward   rate   (LIBOR) } L (T _ {k}) = L _ {k} (T _ {k}) = \frac {1 - P (T _ {k + 1} ; T _ {k})}{P (T _ {k + 1} ; T _ {k}) (T _ {k + 1} - T _ {k})}
$$

(seen on its reset date $T_{k}$ ) is a (deterministic) function of $x(T_{k})$ , 

$$
\text { where } x \text { is   a   Markov   process   of   the   form }\tag{25.12}
$$

$$
\mathrm{d} x = \sigma (t) \mathrm{d} W \quad \text { under } \mathbb {Q} ^ {N}, \qquad x (0) = x _ {0}.
$$

At that point we leave the choice of the numéraires N and the corresponding martingale measure Q open. We will make this choice now, and depending on this we obtain a Markov functional model in terminal measure (Section 25.3.1) or in spot measure (Section ??). 

## 25.3.1. LIBOR Markov Functional Model in Terminal Measure

We choose as numéraire the $T_{n}$ -bond $N := P(T_{n})$ . The measure Q should denote the corresponding martingale measure (terminal measure). From assumption 25.12 we have: 

Lemma 227 (Numéraire of the Markov Functional Model under Terminal Measure): The numéraire $N(T_i) = P(T_n; T_i)$ is a (deterministic) function of $x(T_i)$ , i.e. $N(T_i) = N(T_i, x(T_i))$ . For the functional $\xi \mapsto N(T_i, \xi)$ we have the recursion 

$$
N (T _ {n}, \xi) = 1
$$

$$
N (T _ {i}, \xi) = \left(\mathrm{E} ^ {\mathbb {Q}} \left(\frac {1}{N (T _ {i + 1} , x (T _ {i + 1}))} | \{x (T _ {i}) = \xi \}\right) \cdot (1 + L _ {i} (T _ {i}, \xi) (T _ {i + 1} - T _ {i}))\right) ^ {- 1}.\tag{25.13}
$$

Remark 228 (Notation for the Functionals): Here and in the following we denote the functionals by the same symbol as the corresponding random variables they are representing. In the equation 

$$
N (T _ {i}) = N (T _ {i}, x (T _ {i}))
$$

the $N(T_{i})$ on the left hand side denotes the random variable, on the right hand side $\xi \mapsto N(T_{i}, \xi)$ denotes a function. If we used different symbols it would reduce the readability of the following text. The difference between the two will be obvious from the additional argument $\xi$ or $x(T_{i})$ in its place. 

Proof: Since $\mathbb{Q}$ is the corresponding martingale measure we can use the pricing theorem. Thus for the zero coupon bond $P(T_k)$ (maturity in $T_k$ ) 

$$
\begin{array}{l} \frac {P (T _ {k} ; T _ {i})}{N (T _ {i})} = \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {1}{N (T _ {k})} | \mathcal {F} _ {T _ {i}}), \text {d.h.} \\ P (T _ {k}; T _ {i}) = N (T _ {i}) \mathrm{E} ^ {\mathbb {Q} ^ {N}} (\frac {1}{N (T _ {k})} | \mathcal {F} _ {T _ {i}}). \end{array}
$$

Since the process $x$ generates the filtration $\{\mathcal{F}_{T_i}\}$ and since $x$ is Markovian, it is sufficient to know the $\mathcal{F}_{T_i}$ -measurable random variable $P(T_k; T_i)$ on the set $\{x(T_i) = \xi\}$ . Thus the bond $P(T_k)$ seen at time $T_i$ may be given as a function of $x(T_i)$ , namely as $P(T_k; T_i) = P(T_k; T_i, x(T_i))$ with 

$$
P (T _ {k}; T _ {i}, \xi) := N (T _ {i}, \xi) \mathrm{E} ^ {\mathbb {Q}} (\frac {1}{N (T _ {k} , x (T _ {k}))} | \{x (T _ {i}) = \xi \})\tag{25.14}
$$

Since (compare Definition 99) 

$$
1 + L _ {i} (T _ {i}) \left(T _ {i + 1} - T _ {i}\right) := \frac {P \left(T _ {i} ; T _ {i}\right)}{P \left(T _ {i + 1} ; T _ {i}\right)} = \frac {1}{P \left(T _ {i + 1} ; T _ {i}\right)},
$$

we have 

$$
1 + L _ {i} (T _ {i}, \xi) (T _ {i + 1} - T _ {i}) = \left(N (T _ {i}, \xi) \mathrm{E} ^ {\mathbb {Q}} \left(\frac {1}{N (T _ {i + 1} , x (T _ {i + 1})} | \{x (T _ {i}) = \xi \}\right)\right) ^ {- 1},
$$

and thus (25.13). 

With $N(T_{n}) = P(T_{n};T_{n}) = 1$ we have from (25.13) a recursion to determine the functionals $N(T_{i},\xi)$ from the functionals $L_{i}(T_{i},\xi)$ . 

With the specification of the numéraire the model is fully described. The functionals $\xi \mapsto L_{i}(T_{i}, \xi)$ are the free quantities that may be used to calibrate the model. 

## 25.3.1.1. Evaluation within the LIBOR Markov Functional Model

As preparation for the discussion of the calibration of the model we consider the evaluation of a caplet and a digital caplet using the LIBOR Markov functional model. 

## Valuation of a Caplets within the LIBOR Markov Functional Model

Let $T_{i}$ denote the fixing and $T_{i+1}$ the payment date of caplet with notional 1 and strike K. Then for its value $V_{\text{caplet}}(T_0)$ in the LIBOR Markov functional model 

$$
\begin{array}{c} V _ {\text {caplet}} (T _ {0}) = N (T _ {0}) \cdot \mathrm{E} ^ {\mathbb {Q}} (\frac {\max (L (T _ {i} , x (T _ {i})) - K , 0) \cdot (T _ {i + 1} - T _ {i})}{N (T _ {i + 1} , x (T _ {i + 1})} \mid \{x (T _ {0}) = x _ {0} \}) \\ = N (T _ {0}) \cdot \mathrm{E} ^ {\mathbb {Q}} (\max (L (T _ {i}, x (T _ {i})) - K, 0) \cdot (T _ {i + 1} - T _ {i}) \\ \cdot \bar {P} (T _ {i + 1}; T _ {i}, x (T _ {i})) \mid \{x (T _ {0}) = x _ {0} \}), \end{array}\tag{25.15}
$$

where $\bar{P}(T_{i+1};T_i,\xi) = \mathrm{E}^{\mathbb{Q}}\big(\frac{1}{N(T_{i+1},x(T_{i+1})}\mid\{x(T_i)=\xi\}\big)$ . 

## Valuation of a Digital Caplets within the LIBOR Markov Functional Model

Let $T_{i}$ denote the fixing and $T_{i + 1}$ the payment date of digital caplet with notional 1 and strike $K$ . Then for its value $V_{\mathrm{digital}}(T_0)$ in the LIBOR Markov functional model 

$$
\begin{array}{c} V _ {\text {digital}} (T _ {0}) = N (T _ {0}) \cdot \mathrm{E} ^ {\mathbb {Q}} (\frac {\mathbf {1} (L (T _ {i} , x (T _ {i})) - K) \cdot (T _ {i + 1} - T _ {i})}{N (T _ {i + 1} , x (T _ {i + 1}))} \mid \{x (T _ {0}) = x _ {0} \}) \\ = N (T _ {0}) \cdot \mathrm{E} ^ {\mathbb {Q}} (\mathbf {1} (L (T _ {i}, x (T _ {i})) - K) \cdot (T _ {i + 1} - T _ {i}) \\ \cdot \bar {P} (T _ {i + 1}; T _ {i}, x (T _ {i})) \mid \{x (T _ {0}) = x _ {0} \}), \end{array}\tag{25.16}
$$

where $\bar{P}(T_{i+1};T_{i},\xi)=\mathrm{E}^{\mathbb{Q}}\big(\frac{1}{N(T_{i+1},x(T_{i+1}))}\mid\{x(T_{i})=\xi\}$ . A detailed description of how the given expectations may be numerically calculated, i.e. how to implement the model, is given in Section 25.4. 

## 25.3.1.2. Calibration of the LIBOR Functional

The LIBOR functionals may be derived from the market prices of caplets. One possibility is to give a parametrization of the functional and optimize the parameters by comparing the model prices to given market prices. Another possibility is to derive the functional point-wise from a continuum of given market prices. For this we have to know the market prices of the caplets with periods $[T_{i}, T_{i+1}]$ and strikes $K \in [0, \infty)$ . If the prices are known only for a finite number of strikes $K_{j}$ , then we require a corresponding interpolation of the caplet prices. This is non-trivial, see Chapter 6. 

## Calibration of parametrized LIBOR Functionals

If we assume a parametrized functional form for $L(T_{i})$ , then we can calculate the model prices of caplet on $L(T_{i})$ from a known functional for $N(T_{i+1})$ . This allows us to optimize the parameters of a parametrized functional form to achieve the replication of given market prices. Thus we have the following backward induction: 

## Induction start:

- $N(T_{n}) = 1$ . 

## Induction step $(T_{i+1} \rightarrow T_{i})$ :

- Calculate $\bar{P}(T_{i+1}; T_i, \xi) = \mathrm{E}^{\mathbb{Q}}\big(\frac{1}{N(T_{i+1}, x(T_{i+1}))} \mid \{x(T_i) = \xi\}\big)$ . 

- “Optimize” $L(T_i)$ by comparing (25.15) with given market prices. 

- Calculate $N(T_i)$ from $L(T_i)$ and $\bar{P}(T_{i+1}; T_i)$ via (25.13). 

If $L(T_{i})$ should be almost lognormally distributed, then a good starting point for the parametrization is an exponential. In [26] the following parametrization is discussed: 

$$
L _ {i} (\xi) = \exp (a + b \xi + c (\xi - d) ^ {2}).
$$

## Calibration of discretized LIBOR Functionals (point-wise)

The evaluation of a digital caplet allows us to calculate the value $L(T_i, x^*)$ of the functional for an arbitrary point $x^*$ . We make the following additional assumption: 

$$
\begin{array}{l} \text { The   LIBOR   functional   } \xi \mapsto L (T _ {i}, \xi) \text {   is } \\ \text { strictly   monotone   increasing   in   } \xi . \end{array}\tag{25.17}
$$

With this assumption we can provide a simple algorithm to derive the functional $L(T_{i})$ from a given curve of caplet market prices. $^{6}$ We assume that for any $T_{i}$ and any strike K we have a market caplet price $V_{\mathrm{caplet}}(T_{i}, K; T_{0})$ . $^{7}$ Then we can calculate all digital caplet prices $V_{\mathrm{digital}}^{\mathrm{market}}(T_{i}, K^{*}; T_{0})$ . We have 

$$
V _ {\text { digital }} ^ {\text { market }} (T _ {i}, K; T _ {0}) = \frac {\partial}{\partial K} V _ {\text { caplet }} ^ {\text { market }} (T _ {i}, K; T _ {0}).\tag{25.18}
$$

Let $x^{*}$ denote a given state point. We wish to derive the functional $\xi \mapsto L(T_{i},\xi)$ , i.e. $K^{*} := L(T_{i},x^{*})$ . The model price $V_{\mathrm{digital}}^{\mathrm{model}}(T_i, K^ {*}; T_0)$ for a digital caplet with strike $K^{*}$ is given by 

$$
\begin{array}{c} V _ {\text {digital}} (T _ {0}) = N (T _ {0}) \cdot \mathrm{E} ^ {\mathbb {Q}} \big (\mathbf {1} (L (T _ {i}, x (T _ {i})) - K) \cdot (T _ {i + 1} - T _ {i}) \\ \qquad \cdot \bar {P} (T _ {i + 1}; T _ {i}, x (T _ {i})) \mid \{x (T _ {0}) = 0 \} \big), \\ = N (T _ {0}) \cdot \mathrm{E} ^ {\mathbb {Q}} \big (\mathbf {1} (x (T _ {i}) - x ^ {*}) \cdot (T _ {i + 1} - T _ {i}) \\ \qquad \cdot \bar {P} (T _ {i + 1}; T _ {i}, x (T _ {i})) \mid \{x (T _ {0}) = 0 \} \big), \end{array}\tag{25.19}
$$

thus, from the monotony assumption $(L(x(T_{i})) > K \Leftrightarrow x(T_{i}) > x^{*})$ it follows that the product may be evaluated without the knowledge of the LIBOR functional $L(T_{i})$ . We thus write in brief $V_{\text{digital}}^{\text{model}}(T_{i}, x^{*}; T_{0})$ . By solving the equation 

$$
V _ {\mathrm{digital}} ^ {\mathrm{market}} (T _ {i}, K; T _ {0}) = V _ {\mathrm{digital}} ^ {\mathrm{model}} (T _ {i}, x ^ {*}; T _ {0})\tag{25.20}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/a301a79a607e03abc3ea5a84c9e97476dfb77e82596e2babe83bfa4ba20fda76.jpg)



Figure 25.1.: Calibration of the LIBOR functional $L(x)$ within the Markov functional model: For a given $x^{*}$ we calculate the model price of a digital caplet with strike $K^{*} = L(x^{*})$ (payoff profile in black). This is possible without knowing the functional $L$ . For the given model price $V(x^{*})$ (grey surface) we find the corresponding strike $K^{*}$ by looking it up on the (inverse) of the market price curve (green). This determines the LIBOR functional (blue).


to K we obtain $K^{*}$ , i.e. $L(x^{*})$ , for the given $x^{*}$ . Compare Figure 25.1. 

The LIBOR functional obtained from this procedure replicates the given market price curve of the digital caplets and thus the market price curve of the caplets. Using backward induction we can calibrate the model to caplets of different maturities: 

Induction start: 

- $N(T_{n}) = 1$ . 

Induction step ( $T_{i+1} \rightarrow T_{i}$ ): 

- Calculate $P(T_{i+1}; T_i, \xi) = \mathrm{E}^{\mathbb{Q}}\big(\frac{1}{N(T_{i+1}, x(T_{i+1})} \mid \{x(T_i) = \xi\}\big)$ . 

- For any given $\{x_k^*\}$ : 

- Calculate the model price $V_{\mathrm{digital}}^{\mathrm{model}}(T_i, x^*; T_0)$ from (25.19). 

- Calculate $K^{*} = L(x^{*})$ from (25.20) and (25.18). 

- If required, calculate an interpolation from sample points $x^{*}$ , $L(x^{*})$ obtained in the previous step. 

- Calculate $N(T_i)$ from $L(T_i)$ and $P(T_{i+1};T_i)$ through (25.13). 

## 25.4. Implementation: Lattice

Consider an implementation which relies on functionals discretized in the state space (in contrast to parametrized functionals). In addition to the time discretization $\{0 = T_{0} < \ldots < T_{n}\}$ we consider a discretization of the state space 

$$
x _ {i, j} \in x (T _ {i}) (\Omega) = \mathbb {R} \quad j = 1, \dots , m _ {i}, \quad i = 0, \dots , n.\tag{25.21}
$$

For any given time discretization point $T_{i}$ and any given space discretization point $x^{*} = x_{i,j}$ we calculate the model price of the digital caplet $V_{\mathrm{digital}}^{\mathrm{model}}(T_{i}, x^{*}; T_{0})$ and calculate from it the value of the LIBOR functional $L(T_{i}, x_{i,j})$ and from there the numéraire functional $N(T_{i}, x_{i,j})$ . It remains to specify how we interpolate the functionals $\xi \mapsto L(T_{i}, \xi)$ , $\xi \mapsto N(T_{i}, \xi)$ for $\xi \neq x_{i,j}$ and calculate the conditional expectations, i.e. how we perform the numerical integration 

$$
\mathrm{E} ^ {\mathbb {Q}} \left(\frac {1}{N (T _ {i + 1} , x (T _ {i + 1}))} \mid \{x (T _ {i}) = x _ {i, j} \}\right) = \int_ {- \infty} ^ {\infty} \frac {1}{N (T _ {i + 1} , \xi)} \cdot \phi (\xi - x _ {i, j}, \sigma_ {i}) \mathrm{d} \xi
$$

where $\phi (\xi -\mu ,\sigma_i) = \frac{1}{\sqrt{2\pi}\sigma_i}\exp (-\frac{(\xi - \mu)^2}{2\sigma_i^2})$ denotes the (transition) probability density of $x(T_{i + 1}) - x(T_i)|_{x(T_i) = \mu}$ with $\sigma_{i}:= (\int_{T_{i}}^{T_{i + 1}}\sigma^{2}(t)\mathrm{d}t)^{1 / 2}$ . 

## 25.4.1. Convolution with the Normal Probability Density

A main part of the implementation of the model is the numerical integration, i.e. the convolution of a functional with the density of the normal probability 

$$
\mathrm{E} ^ {\mathbb {Q}} \left(f (x (T _ {i + 1})) \mid \{x (T _ {i}) = x _ {i, j} \}\right) = \int_ {- \infty} ^ {\infty} f (\xi) \cdot \phi (\xi - x _ {i, j}, \sigma_ {i}) \mathrm{d} \xi =: I\tag{25.22}
$$

with $\phi (\xi -\mu ,\sigma_i) = \frac{1}{\sqrt{2\pi}\sigma_i}\exp (-\frac{(\xi - \mu)^2}{2\sigma_i^2})$ . In the literature one can find many methods for numerical integration. Since $f$ is given only at the state space sample points (lattice) $\{x_{i + 1,k}|j = 1,\dots ,m_i\}$ , but the density $\phi$ is given analytically, it is natural to make use of this. 

## 25.4.1.1. Piecewise constant Approximation

Let $x_{i+1,k+\frac{1}{2}} = \frac{x_{i+1,k+1} + x_{i+1,k}}{2}$ denote the center point of the interval $[x_{i+1,k}, x_{i+1,k+1}]$ and let $f_k := f(x_{i+1,k})$ . Then an approximation of the integral $I$ from (25.22) is given by 

$$
I \approx \sum_ {k = 1} ^ {k = n} f _ {k} \cdot (\Phi_ {x _ {i, j}, \sigma_ {i}} (x _ {i + 1, k + \frac {1}{2}}) - \Phi_ {x _ {i, j}, \sigma_ {i}} (x _ {i + 1, k - \frac {1}{2}})),
$$

where $\Phi_{\mu,\sigma}(x)=\int_{-\infty}^{x}\phi(\xi-\mu,\sigma)\mathrm{d}\xi$ . For the cumulative normal distribution function $\Phi_{\mu,\sigma}$ there are very accurate approximations using rational functions. 

## 25.4.1.2. Piecewise polynomial Approximation

If we approximate the integrand $f$ by a piecewise polynomial, then we have to calculate integrals of the form 

$$
\int_ {h _ {1}} ^ {h _ {2}} \xi^ {m} \cdot \phi (\xi - x _ {i, j}, \sigma_ {i}) \mathrm{d} \xi .
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/954f5195d386884a4293b54b8da50deac27f8fc8d2f179673fa029e08a41eb35.jpg)



Figure 25.2.: Calculation of the conditional expectation (numerical integration) within a “lattice”.


These may be given recursively in terms of the cumulative distribution function $\Phi$ . We have Lemma 229 (Convolution of a monomial with the normal distribution function $^{8}$ ): 

$$
\begin{array}{r l} \int_ {h _ {1}} ^ {h _ {2}} \xi^ {m} \cdot \phi (\xi - \mu , \sigma) \mathrm{d} \xi & = \mu \cdot \int_ {h _ {1}} ^ {h _ {2}} \xi^ {m - 1} \cdot \phi (\xi - \mu , \sigma) \mathrm{d} \xi \\ & + (m - 1) \cdot \int_ {h _ {1}} ^ {h _ {2}} \xi^ {m - 2} \cdot \phi (\xi - \mu , \sigma) \mathrm{d} \xi \\ & - \sigma^ {2} \left[ \xi^ {m - 1} \cdot \phi (\xi - \mu , \sigma) \right] _ {h _ {1}} ^ {h _ {2}} \end{array}
$$

Proof: For $m\in \mathbb{N}$ 

$$
\begin{array}{l} \frac {\partial}{\partial \xi} \xi^ {m - 1} \cdot \exp \Big (- \frac {1}{2} (\frac {\xi - \mu}{\sigma}) ^ {2} \Big) \\ \qquad = (m - 1) \cdot \xi^ {m - 2} \cdot \exp \Big (- \frac {1}{2} (\frac {\xi - \mu}{\sigma}) ^ {2} \Big) + \xi^ {m - 1} \exp \Big (- \frac {1}{2} (\frac {\xi - \mu}{\sigma}) ^ {2} \Big) \frac {- (\xi - \mu)}{\sigma^ {2}} \\ \qquad = (m - 1) \cdot \xi^ {m - 2} \cdot \exp \Big (- \frac {1}{2} (\frac {\xi - \mu}{\sigma}) ^ {2} \Big) - \frac {\xi^ {m}}{\sigma^ {2}} \exp \Big (- \frac {1}{2} (\frac {\xi - \mu}{\sigma}) ^ {2} \Big) \\ \qquad + \frac {\mu}{\sigma^ {2}} \xi^ {m - 1} \exp \Big (- \frac {1}{2} (\frac {\xi - \mu}{\sigma}) ^ {2} \Big), \end{array}
$$

i.e. 

$$
\begin{array}{l} \xi^ {m} \exp \Big (- \frac {1}{2} (\frac {\xi - \mu}{\sigma}) ^ {2} \Big) \\ = (m - 1) \sigma^ {2} \cdot \xi^ {m - 2} \cdot \exp \Big (- \frac {1}{2} (\frac {\xi - \mu}{\sigma}) ^ {2} \Big) + \mu \xi^ {m - 1} \exp \Big (- \frac {1}{2} (\frac {\xi - \mu}{\sigma}) ^ {2} \Big) \\ - \frac {\partial}{\partial \xi} \sigma^ {2} \xi^ {m - 1} \cdot \exp \Big (- \frac {1}{2} (\frac {\xi - \mu}{\sigma}) ^ {2} \Big). \end{array}
$$

$^{8}$ Compare [26]. 

The claim follows after multiplication with $\frac{1}{\sqrt{2\pi}\sigma}$ and integration $\int_{h_1}^{h_2}$ . 

To calculate the interpolating polynomials many different methods may be used (e.g. Cubic Spline Interpolation). The Neville algorithm gives a simple recursion by which we can calculate a piecewise polynomial interpolation function: 

Lemma 230 (Neville Algorithm - Piecewise polynomial interpolation function): Let $x_{i}$ denote given sample points and $f_{i}$ the corresponding values. If $F_{i - k_1,i + k_2}$ is a polynomial of degree $k_{1} + k_{2}$ interpolating the points $(x_{j},f_{j}), j = i - k_{1},\ldots i + k_{2}$ , i.e. 

$$
F _ {i - k _ {1}, i + k _ {2}} (x _ {j}) = f _ {j} \quad \text { for } j = i - k _ {1}, \dots i + k _ {2},
$$

then 

$$
F _ {i - k _ {1}, i + k _ {2} + 1} (\xi) = \frac {(\xi - x _ {i - k _ {1}}) \cdot F _ {i - k _ {1} + 1 , i + k _ {2} + 1} (\xi) + (x _ {i + k _ {2} + 1} - \xi) \cdot F _ {i - k _ {1} , i + k _ {2}}}{x _ {i + k _ {2} + 1} - x _ {i - k _ {1}}}
$$

defines an interpolating polynomial of degree $k_{1} + k_{2} + 1$ for the points $(x_{j}, f_{j})$ , $j = i - k_{1}, \ldots, i + k_{2} + 1$ . With the trivial interpolating polynomial $F_{i,i} \equiv f_{i}$ having degree 0, induction gives a construction of the desired interpolating polynomial. 

Proof: A polynomial of degree $k_{1} + k_{2} + 1$ is uniquely determined by $k_{1} + k_{2} + 2$ points. The claim follows then by induction, evaluating the approximations polynomial $F_{i - k_1,i + k_2 + 1}$ at the sample points $x_{i + k_2 + 1}, x_{i - k_1}$ and the sample points which are common to $F_{i - k_1 + 1,i + k_2 + 1}$ and $F_{i - k_1,i + k_2}$ . 

The algorithm is called the Neville algorithm. The polynomial $F_{i-k_{1},i+k_{2}}(x_{j})$ will then be used as an interpolating polynomial on the interval $x_{i}, x_{i+1}$ .⁹ Using Lemma 229 the corresponding integral part is calculated. 

The interpolation function is (for degree $>0$ ) continuous, but is not differentiable at the interval bounds, as would be the case with a cubic spline interpolation. 

## 25.4.2. State space discretization

The rule for choosing the state space discretization points $x_{i,j}, j = 1, \ldots, m_{i}$ (the lattice) for the realization of the Markovian driver $x(T_{i})$ has a major impact on the accuracy of the model. 

## 25.4.2.1. Equidistant discretization

A simple rule gives an equidistant discretization of the interval $[x_{i,\min}, x_{i,\max}]$ , where the interval has been chosen such that the neglected area $(-\infty, x_{i,\min}) \cup (x_{i,\max}, \infty)$ supports only a small probability measure $\mathbb{Q}(x(T_i) \notin [x_{i,\min}, x_{i,\max}]) = \epsilon$ , see Figure 25.3. The bounds $x_{i,\min}$ , $x_{i,\max}$ may be derived from the definition of the process $x$ , e.g. in terms of the standard deviation of $x(T_i)$ : 

$$
x _ {i, m a x} = - x _ {i, m i n} = k \cdot \bar {\sigma} _ {i}, \quad \bar {\sigma} _ {i} := \big (\int_ {0} ^ {T _ {i}} \sigma^ {2} (t) d t \big) ^ {1 / 2}.
$$

The factor $k$ has to be chosen sufficiently large (e.g. $k > 3$ ). 

Instead of an equidistant discretization one may choose the interval $[x_{i,j}, x_{i,j+1}]$ such that all intervals support the same probability mass, i.e. 

$$
\mathbb {Q} (x _ {i, j} \leq x (T _ {i}) \leq x _ {i, j + 1}) = \frac {1 - \epsilon}{m _ {i} - 1}.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/fb9344e4623a6a9234c37bd9a3fdabaa9d3b4171cd10a3519339e88757d1b6d9.jpg)



Figure 25.3.: State space discretization for the Markov functional model: A simple rule to choose the discretization points $x_{i,j}$ .


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/642a8d6f052ac9f8c3f982d7a6d91a8b71eb2497d6fd3ba0be1f695322f378fe.jpg)


Further Reading: The LIBOR and Swaprate Markov Functional Model in terminal measure is discussed in the books $[14, 26]$ as well as in the original article $[75]$ . A LIBOR Markov functional model in spot measure and a hybrid Markov functional model is discussed in $[67]$ . 

Part VI. 

Extended Models 

## Hybrid Models

In this chapter we introduce several kinds of hybrid models. A hybrid model is a model that models multiple (different) assets in a single unified model. In general one combines several well known models into a single unified model. Since different models usually come under different pricing measures, the essence of a hybrid model is the question “How do these models look under a common pricing measure?”. So apart from the prerequisite that the models are compatible, the construction of a hybrid model is just a change of measure. 

In this sense, we have already encountered the basic technique required for a hybrid model in the discussion of the LIBOR Market Model: There we wrote down multiple individual Black models (Chapter 10) and asked ourselves how they look under a common pricing measure. The result was the LIBOR Market Model. 

## 26.1. Cross Currency LIBOR Market Model

For two currencies, “domestic” and “foreign”, we model the interest rate curves, each with a LIBOR Market Model, as was discussed for an interest rate curve in a single currency in Section 19.1. 

In addition we model the foreign exchange rate $FX(t)$ . In Chapter 11 we presented the pricing of a quanto caplet by modeling the $FX$ forward as a lognormal process. Here the spot exchange rate $FX(t)$ is modeled directly, also as a lognormal process. Let $FX(t)$ denote the amount (in domestic currency) that has to be paid by a domestic investor at time $t$ for one unit of foreign currency (for). Thus, $FX(t)$ has the (physical) unit $[FX(t)] = \frac{1}{1}\frac{\text{dom}}{\text{for}}$ . 

We assume that for the chosen numéraire N that there exists a corresponding equivalent martingale measure $Q^{N}$ . By the change of measure theorem (Girsanov theorem, 58) the modeled quantities are again lognormal processes under $Q^{N}$ , i.e. 

$$
\begin{array}{l} \mathrm{d} L _ {i} (t) = L _ {i} (t) \cdot \mu_ {i} (t) \mathrm{d} t + L _ {i} (t) \sigma_ {i} (t) \mathrm{d} W _ {i} ^ {\mathbb {Q} ^ {N}} (t) \qquad (0 \leq i \leq n - 1) \\ \mathrm{d} F X (t) = F X (t) \cdot \mu^ {F X} (t) \mathrm{d} t + F X (t) \sigma^ {F X} (t) \mathrm{d} W _ {F X} ^ {\mathbb {Q} ^ {N}} (t) \\ \mathrm{d} \tilde {L} _ {i} (t) = \tilde {L} _ {i} (t) \cdot \tilde {\mu} _ {i} (t) \mathrm{d} t + \tilde {L} _ {i} (t) \tilde {\sigma} _ {i} (t) \mathrm{d} \tilde {W} _ {i} ^ {\mathbb {Q} ^ {N}} (t) \qquad (0 \leq i \leq n - 1) \end{array}
$$

with initial conditions 

$$
L _ {i} (0) = L _ {i, 0}, \qquad F X (0) = F X _ {0}, \qquad \tilde {L} _ {i} (0) = \tilde {L} _ {i, 0}.
$$

As before, this is the starting point for 

- Determination of the drift terms $\mu_{i},\mu^{FX}$ und $\tilde{\mu}_i$ for a chosen numéraire $N(t)$ using the $\mathbb{Q}^N$ -martingale property of $N$ -relative prices. 

- Determination of the initial conditions $L_{i,0}$ , $FX_{0}$ , $\tilde{L}_{i,0}$ using the bond and foreign-bond prices observed at time t = 0. 

- Determination/choice of the volatility and correlation to reproduce given option prices. 

## 26.1.1. Derivation of the Drift Term under Spot-Measure

As numéraire we chose the rolled over one period bond we had already made use of in Section 19.1.1.2 

$$
N (t) := P \left(T _ {m (t) + 1}; t\right) \prod_ {j = 0} ^ {m (t)} \left(1 + L _ {j} \left(T _ {j}\right) \cdot \delta_ {j}\right).
$$

where $m(t) := \max\{i : T_i \leq t\}$ , $\delta_j := T_{j+1} - T_j$ . We will now derive the corresponding processes (i.e. the drifts) under the corresponding equivalent martingale measure $Q^N$ , the spot measure. 

## 26.1.1.1. Dynamic of the domestic LIBOR under Spot Measure

For the drift $\mu_{i}$ we have, exactly as in Section 19.1.1.2 

$$
\mu_ {i} (t) = \sum_ {l = m (t) + 1} ^ {i} \frac {\delta_ {l} L _ {l} (t)}{(1 + \delta_ {l} L _ {l} (t))} \sigma_ {i} (t) \sigma_ {l} (t) \rho_ {i, l} (t).
$$

This is the already known LIBOR Market Model in domestic currency. 

## 26.1.1.2. Dynamic of the foreign LIBOR under Spot Measure

We derive the drift $\tilde{\mu}_{i}(t)$ of the foreign LIBOR by considering financial product from the foreign market. The foreign bond $\tilde{P}(T_{i+1})$ , converted to domestic currency, i.e. $\tilde{P}(T_{i+1})\cdot FX$ is a traded asset for the domestic investor. Thus, $\frac{\tilde{P}(T_{i+1};t)\cdot FX(t)}{N(t)}$ is a $Q^{N}$ -martingale. $^{1}$ 

$$
\operatorname{Drift} _ {\mathbb {Q} ^ {N}} \left(\frac {\tilde {P} (T _ {i + 1} ; t) \cdot F X (t)}{N (t)}\right) = 0.\tag{26.1}
$$

Likewise 

$$
\tilde {L} _ {i} \cdot \tilde {P} (T _ {i + 1}) \cdot F X = \frac {\tilde {P} (T _ {i}) - \tilde {P} (T _ {i + 1})}{T _ {i + 1} - T _ {i}} \cdot F X\tag{26.2}
$$

is a traded asset for the domestic investor, because it is a portfolio of (foreign) bonds converted to domestic currency. Thus, 

$$
\operatorname{Drift} _ {\mathbb {Q} ^ {N}} \left(\tilde {L} _ {i} \cdot \frac {\tilde {P} (T _ {i + 1} ; t) \cdot F X (t)}{N (t)}\right) = 0.
$$

$^{1}$ In the view of the domestic investor the foreign bond is not a traded asset. Only after conversion to the domestic currency by the applicable conversion rate $FX(t)$ does the product becomes tradable for the domestic investor. This is also apparent from the fact that relative prices are dimensionless: While $\frac{\tilde{P}(T_{i+1};t)FX(t)}{N(t)}$ is dimensionless, we find that $\frac{\tilde{P}(T_{i+1};t)}{N(t)}$ has the (physical) unit $\frac{1}{1}$ for $\frac{1}{1}$ dom. 

From the product rule we find 

$$
\begin{array}{l} \mathrm{d} (\tilde {L} _ {i} (t) \cdot \frac {\tilde {P} (T _ {i + 1} ; t) \cdot F X (t)}{N (t)}) \\ = \frac {\tilde {P} (T _ {i + 1} ; t) \cdot F X (t)}{N (t)} \cdot \mathrm{d} \tilde {L} _ {i} + \tilde {L} _ {i} \cdot \mathrm{d} (\frac {\tilde {P} (T _ {i + 1} ; t) \cdot F X (t)}{N (t)}) \\ + \mathrm{d} \tilde {L} _ {i} \cdot \mathrm{d} (\frac {\tilde {P} (T _ {i + 1} ; t) \cdot F X (t)}{N (t)}) \end{array}\tag{26.3}
$$

(26.4) 

from which we derive $\tilde{\mu}_{i}$ after calculation of $\mathrm{d}\frac{\tilde{P}(T_{i+1};t)\cdot FX(t)}{N(t)}$ by comparing drift terms. We have 

$$
\mathrm{d} \Big (\frac {\tilde {P} (T _ {i + 1} ; t) \cdot F X (t)}{N (t)} \Big) = \mathrm{d} \Big (\frac {\tilde {P} (T _ {m (t) + 1} ; t)}{P (T _ {m (t) + 1} ; t)} \frac {\prod_ {j = m (t) + 1} ^ {i} \big (1 + \tilde {L} _ {j} (t) \delta_ {j} \big) ^ {- 1}}{\prod_ {i = 0} ^ {m (t)} \big (1 + L _ {j} (T _ {j}) \delta_ {j} \big)} \cdot F X (t) \Big).
$$

Remark 231 (Interpolation of Bond Prices): At this point we encounter an interesting difference to the single currency LIBOR Market Modell (see Section 19.1): While for the case of the domestic currency the corresponding term $\frac{P(T_{m(t)+1};t)}{P(T_{m(t)+1};t)}$ vanishes, it is necessary to provide an interpretation of $\frac{\tilde{P}(T_{m(t)+1};t)}{P(T_{m(t)+1};t)}$ . See also Section 19.1.2.3. 

We have not yet defined the value of the short period bonds $P(T_{i+1}; t)$ and $\tilde{P}(T_{i+1}; t)$ for $t \neq T_j$ , $j = 0, 1, 2, \ldots$ . We do this now and define for $T_j < t \leq T_{j+1}$ 

$$
\begin{array}{r l} & P (T _ {m (t) + 1}; t) := \big (1 + L _ {m (t)} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t) \big) ^ {- 1}, \\ & \tilde {P} (T _ {m (t) + 1}; t) := \big (1 + \tilde {L} _ {m (t)} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t) \big) ^ {- 1}. \end{array}
$$

This concludes the definition of the numéraire. 

From this we find 

$$
\mathrm{d} \frac {\tilde {P} (T _ {m (t) + 1} ; t)}{P (T _ {m (t) + 1} ; t)} = \frac {\partial}{\partial t} \left(\frac {1 + L _ {m (t)} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t)}{1 + \tilde {L} _ {m (t)} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t)}\right) \mathrm{d} t,
$$

i.e. the term $\frac{P(T_{i+1};t)}{P(T_{i+1};t)}$ has no diffusion part dW for $T_{j} < t \leq T_{j+1}$ . This is sufficient for the following derivation: the specific form of the drift does not need to be known. 

Indeed, it would be sufficient to require that $P(T_{i+1};t)$ and $\tilde{P}(T_{i+1};t)$ have zero volatility, i.e. no diffusion part, in the short period $t \in (T_i, T_{i+1}]$ . No specific interpolation is required. The zero volatility assumption for $P(T_{i+1};t)$ and $\tilde{P}(T_{i+1};t)$ on $t \in (T_i, T_{i+1}]$ closes the definition of the LIBOR Market Model for all $t \in \{T_0, T_1, \ldots\}$ . 

Continuing with the derivation of the drift, we have 

$$
\begin{array}{l} \mathrm{d} \Big (\frac {\tilde {P} (T _ {i + 1} ; t) \cdot F X (t)}{N (t)} \Big) \\ = \mathrm{d} \Big (\frac {\tilde {P} (T _ {i + 1} ; t)}{P (T _ {i + 1} ; t)} \frac {\prod_ {j =} ^ {i} \big (1 + \tilde {L} _ {j} (t) \delta_ {j} \big) ^ {- 1}}{\prod_ {j = 0} ^ {- 1} \big (1 + L _ {j} (T _ {j}) \delta_ {j} \big)} \cdot F X (t) \Big) \\ = (\ldots) \mathrm{d} t - \frac {\tilde {P} (T _ {i + 1} ; t) \cdot F X (t)}{N (t)} \cdot \sum_ {j = m (t) + 1} ^ {i} \frac {\delta_ {j} \tilde {L} _ {j}}{(1 + \delta_ {j} \tilde {L} _ {j})} \tilde {\sigma} _ {j} \mathrm{d} \tilde {W} _ {j} ^ {\mathbb {Q} ^ {N}} (t) \\ + \frac {\tilde {P} (T _ {i + 1} ; t) \cdot F X (t)}{N (t)} \cdot \sigma^ {F X} (t) \mathrm{d} W _ {F X} ^ {\mathbb {Q} ^ {N}} (t) \end{array}
$$

If we plug this into (26.4) and compare drift terms (the coefficients of dt) we get, together with (26.1) and (26.2), 

$$
\begin{array}{l} 0 = \frac {\tilde {P} (T _ {i + 1} ; t) \cdot F X (t)}{N (t)} \cdot \tilde {L} _ {i} (t) \cdot \tilde {\mu} _ {i} (t) + 0 \\ \qquad + \frac {\tilde {P} (T _ {i + 1} ; t) \cdot F X (t)}{N (t)} \cdot \tilde {L} _ {i} (t) \Big (- \sum_ {j = m (t) + 1} ^ {i} \frac {\delta_ {j} \tilde {L} _ {j}}{(1 + \delta_ {j} \tilde {L} _ {j})} \tilde {\sigma} _ {i} \tilde {\sigma} _ {j} \mathrm{d} \tilde {W} _ {i} ^ {\mathbb {Q} ^ {N}} (t) \mathrm{d} \tilde {W} _ {j} ^ {\mathbb {Q} ^ {N}} (t) \\ \qquad + \left. \tilde {\sigma} _ {i} \sigma^ {F X} (t) \mathrm{d} \tilde {W} _ {j} ^ {\mathbb {Q} ^ {N}} (t) \mathrm{d} W _ {F X} ^ {\mathbb {Q} ^ {N}} (t)\right). \end{array}
$$

Denoting the interest rate correlation within the foreign currency by $\tilde{\rho}_{i,j}$ , i.e. 

$$
\mathrm{d} \tilde {W} _ {i} ^ {\mathbb {Q} ^ {N}} (t) \mathrm{d} \tilde {W} _ {j} ^ {\mathbb {Q} ^ {N}} (t) = \tilde {\rho} _ {i, j} (t) \mathrm{d} t
$$

and denoting the correlation of the foreign currency and the foreign exchange rate by $\rho_{i,FX}$ , i.e. 

$$
\mathrm{d} \tilde {W} _ {i} ^ {\mathbb {Q} ^ {N}} (t) \mathrm{d} W _ {F X} ^ {\mathbb {Q} ^ {N}} (t) = \rho_ {\tilde {i}, \mathrm{FX}} (t) \mathrm{d} t,
$$

gives 

$$
\tilde {\mu} _ {i} (t) = \sum_ {j = m (t) + 1} ^ {i} \frac {\delta_ {j} \tilde {L} _ {j} (t)}{(1 + \delta_ {j} \tilde {L} _ {j}) (t)} \tilde {\sigma} _ {i} (t) \tilde {\sigma} _ {j} (t) \tilde {\rho} _ {i, j} (t) - \tilde {\sigma} _ {i} (t) \sigma^ {F X} (t) \rho_ {i, \mathrm{FX}}.
$$

## 26.1.1.3. Dynamic of the FX Rate under Spot Measure

For a given $t \in [T_{m(t)}, T_{m(t)+1})$ consider the foreign bond with maturity $T_{m(t)+1}$ – the next possible maturity in our tenor discretization. Converting it to domestic currency its N-relative value $\frac{FX(t)\cdot\tilde{P}(T_{m(t)+1};t)}{N(t)}$ is a martingale. Furthermore we have 

$$
\begin{array}{l l} & \mathrm{d} \Big (F X (t) \cdot \frac {\tilde {P} (T _ {m (t) + 1} ; t)}{N (t)} \Big) \\ \stackrel {{\text {Def.}}} {{=}} N & \prod_ {j = 0} ^ {m (t)} (1 + L _ {j} (T _ {j}) \delta_ {j}) \cdot \mathrm{d} \Big (F X (t) \cdot \frac {\tilde {P} (T _ {m (t) + 1} ; t)}{P (T _ {m (t) + 1} ; t)} \Big) \\ = & \mathrm{d} F X (t) \cdot \frac {\tilde {P} (T _ {m (t) + 1} ; t)}{N (t)} \\ & + F X (t) \prod_ {j = 0} ^ {m (t)} (1 + L _ {j} (T _ {j}) \delta_ {j}) \frac {\partial}{\partial t} \left(\frac {\tilde {P} (T _ {m (t) + 1} ; t)}{P (T _ {m (t) + 1} ; t)}\right) \mathrm{d} t \\ \stackrel {{\text {Def.}}} {{=}} N & \mathrm{d} F X (t) \cdot \frac {\tilde {P} (T _ {m (t) + 1} ; t)}{N (t)} + F X (t) \cdot \frac {\tilde {P} (T _ {m (t) + 1} ; t)}{N (t)} \frac {\frac {\partial}{\partial t} \left(\frac {\tilde {P} (T _ {m (t) + 1} ; t)}{P (T _ {m (t) + 1} ; t)}\right)}{\frac {\tilde {P} (T _ {m (t) + 1} ; t)}{P (T _ {m (t) + 1} ; t)}} \mathrm{d} t \end{array}
$$

and thus 

$$
\begin{array}{c} \mu^ {F X} (t) = - \frac {\frac {\partial}{\partial t} \left(\frac {\tilde {P} (T _ {m (t) + 1} ; t)}{P (T _ {m (t) + 1} ; t)}\right)}{\frac {\tilde {P} (T _ {m (t) + 1} ; t)}{P (T _ {m (t) + 1} ; t)}} = - \frac {\partial}{\partial t} \log \left(\frac {\tilde {P} (T _ {m (t) + 1} ; t)}{P (T _ {m (t) + 1} ; t)}\right) \\ = \frac {\partial}{\partial t} \log \left(\frac {P (T _ {m (t) + 1} ; t)}{\tilde {P} (T _ {m (t) + 1} ; t)}\right). \end{array}
$$

The drift $\mu^{FX}(t)$ thus depends on the chosen interpolation of the bond prices, see Remark 231. However, for its use in an implementation via a time-discretization scheme it is not necessary to calculate the corresponding derivative after $t$ , since only the integrated drift enters the time-discretization scheme. For the integral $\int_{T_i}^{T_{i+1}}\mu^{FX}(t)\mathrm{d}t$ we have 

$$
\begin{array}{l} \int_ {T _ {i}} ^ {T _ {i + 1}} \mu^ {F X} (t) \mathrm{d} t = \log \left(\frac {P (T _ {i + 1} ; T _ {i + 1})}{\tilde {P} (T _ {i + 1} ; T _ {i + 1})}\right) - \log \left(\frac {P (T _ {i + 1} ; T _ {i})}{\tilde {P} (T _ {i + 1} ; T _ {i})}\right) = - \log \left(\frac {P (T _ {i + 1} ; T _ {i})}{\tilde {P} (T _ {i + 1} ; T _ {i})}\right) \\ = \log \left(\frac {1 + \tilde {L} (T _ {i} , T _ {i + 1} ; T _ {i})}{1 + L (T _ {i} , T _ {i + 1} ; T _ {i})}\right), \end{array}
$$

i.e. it is independent of the interpolation of the bond prices. See also Section 26.3.2. 

## 26.1.2. Implementation

We will discuss the implementation together with the Equity Hybrid LIBOR Market Model in Section 26.3.2. 

## 26.2. Equity Hybrid LIBOR Market Model

In Section 4 we introduced the Black-Scholes Modell for a (single) stock. The stock $S$ was modeled as a lognormal process 

$$
\mathrm{d} S (t) = \mu^ {S, \mathbb {P}} (t) S (t) \mathrm{d} t + \sigma^ {S} (t) S (t) \mathrm{d} W ^ {S, \mathbb {P}} (t)
$$

under the real measure $\mathbb{P}$ . 

We had assumed interest rates to be non-stochastic and constant and the chosen numéraire was then $B(t) := \exp(r \cdot t)$ . Under the corresponding martingale measure $Q^{B}$ we could then derive an analytic formula for the price of a European stock option. 

The pricing of products exhibiting optionalities related to both stock and interest rates requires joint stochastic modeling of the stock and the interest rates. If we chose as the interest rate model the LIBOR Market Model and as the stock process model the Black-Scholes Modell, then the construction of the joint model is simply the derivation of the drifts under a common measure. 

## 26.2.1. Derivation of the Drift Term under Spot-Measure

As before, we choose as numéraire the rolled over one period bond 

$$
N (t) := P \left(T _ {m (t) + 1}; t\right) \prod_ {j = 0} ^ {m (t)} \left(1 + L _ {j} \left(T _ {j}\right) \cdot \delta_ {j}\right),
$$

where $m(t) := \max\{i : T_i \leq t\}$ and $\delta_j := T_{j+1} - T_j$ . 

## 26.2.1.1. Dynamic of the Stock Process under Spot Measure

The stock $S$ is a traded assed, thus $\frac{S}{N}$ is a martingale under the equivalent martingale measure $\mathbb{Q}^N$ . From the product rule we have 

$$
\mathrm{d} \left(\frac {S}{N}\right) = \mathrm{d} S \cdot \frac {1}{N} + S \mathrm{d} \left(\frac {1}{N}\right) + \mathrm{d} S \mathrm{d} \left(\frac {1}{N}\right).
$$

For $T_{i} < t < T_{i+1}$ let the bond price $P(T_{i+1}; t)$ defined (interpolated) as in Remark 231, i.e. 

$$
P (T _ {i + 1}; t) := \left(1 + L _ {i} (T _ {i}) \cdot (T _ {i + 1} - t)\right) ^ {- 1} \quad \mathrm{for} T _ {i} <   t <   T _ {i + 1}.
$$

In this case 

$$
\begin{array}{l} \mathrm{d} \Big (\frac {1}{N} \Big) = \Big (\frac {1}{P (T _ {m (t) + 1} ; t)} \cdot \prod_ {j = 0} ^ {m (t)} (1 + L _ {j} (T _ {j}) \delta_ {j}) \Big) \\ \qquad = \mathrm{d} \Big (\frac {1}{P (T _ {m (t) + 1} ; t)} \cdot \prod_ {j = 0} ^ {m (t)} (1 + L _ {j} (T _ {j}) \delta_ {j}) \Big) \\ \qquad = \mathrm{d} \Big ((1 + L _ {m (t)} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t)) \cdot \prod_ {j = 0} ^ {m (t)} (1 + L _ {j} (T _ {j}) \delta_ {j}) \Big) \\ \qquad = - L _ {m (t)} (T _ {m (t)}) \mathrm{d} t \cdot \prod_ {j = 0} ^ {m (t)} (1 + L _ {j} (T _ {j}) \delta_ {j}) \\ \qquad = - \frac {L _ {m (t)} (T _ {m (t)})}{1 + L _ {m (t)} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t)} \mathrm{d} t \cdot \frac {1}{N} \\ \qquad = \frac {\partial}{\partial t} \log \big (1 + L _ {m (t)} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t) \big) \mathrm{d} t \frac {1}{N}. \end{array}
$$

Remark 232 (on the numéraire process $\frac{1}{N}$ ): Under the assumption that $N(t)$ does not have a diffusion (i.e. dW) term, which is the case for the above definition of the short period bond, then $\mathrm{d}\left(\frac{1}{N}\right)=\left(\frac{\partial}{\partial t}\frac{1}{N}\right)\mathrm{d}t$ . Nothing else has been calculated above. See also remark 231. 

Assuming that $N$ does not have a diffusion (i.e. $\mathrm{d}W$ ) term, $\mathrm{d}S\mathrm{d}\left(\frac{1}{N}\right) = 0$ and from $\mathrm{Drift}_{\mathbb{Q}^N}\left(\frac{S}{N}\right) = 0$ we find 

$$
0 = \mu^ {S} \frac {S}{N} + \left[ \frac {\partial}{\partial t} \log \left(1 + L _ {m (t)} \left(T _ {m (t)}\right) \cdot \left(T _ {m (t) + 1} - t\right)\right) \right] \frac {S}{N} + 0,
$$

thus 

$$
\begin{array}{r c l} \mu^ {S} (t) & = & - \frac {\partial}{\partial t} \log \big (1 + L _ {m (t)} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t) \big) \\ & = & \frac {L _ {m (t)} (T _ {m (t)})}{1 + L _ {m (t)} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t)}. \end{array}\tag{26.5}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/45b29b5d88c368048c16e3a44fa4ff310e7536de524e861ead8f77587d707338.jpg)


Interpretation (Comparison to the Dynamic of the Black-Scholes Model): Using the numéraire $B(t) := \exp(r \cdot t)$ used in the Black-Scholes model (see Section 4) we had derived the drift of the stock process under the martingale measure $\mathbb{Q}^B$ as $\mu^{S, \mathbb{Q}^B} = r$ . Equation (26.5) is simply a discrete (and a series of which $E_{\mathrm{th}}$ and $\mathrm{d}_{\mathrm{th}}$ are similar to $T$ ). 

stochastic) version of this drift: For the average drift over one period $[T_{i}, T_{i+1}]$ 

$$
\begin{array}{r l} \frac {1}{T _ {i + 1} - T _ {i}} \int_ {T _ {i}} ^ {T _ {i + 1}} \mu^ {S, \mathbb {Q} ^ {N}} (t) \mathrm{d} t & = \log (1) - \log (1 + L _ {i} (T _ {i})) \cdot (T _ {i + 1} - T _ {i})) \\ & = - \frac {\log (1 + L _ {i} (T _ {i})) \cdot (T _ {i + 1} - T _ {i}))}{T _ {i + 1} - T _ {i}} \end{array}
$$

and for infinitesimal period lengths $T_{i+1} \to T_i$ we find - see Definition 103 - that 

$$
\frac {- \log (1 + L _ {i} (T _ {i})) \cdot (T _ {i + 1} - T _ {i}))}{T _ {i + 1} - T _ {i}} \underset {T _ {i + 1} \to T _ {i}} {\longrightarrow} r (T _ {i}) = \mu^ {S, \mathbb {Q} ^ {B}},
$$

i.e. 

$$
\mu^ {S, \mathbb {Q} ^ {N}} (t) \underset {T _ {i + 1} \to T _ {i}} {\longrightarrow} \mu^ {S, \mathbb {Q} ^ {B}}.\tag{◀|}
$$

## 26.2.2. Implementation

We discuss the implementation together with the previously discussed Cross Currency LIBOR Market Model in Section 26.3.2. 

## 26.3. Equity-Hybrid Cross-Currency LIBOR Market Model

The models given in Section 26.1 and 26.2 may be combined. This is now trivial since the numéraire and thus the martingale measure are the same in both models. Thus we have a unified model for interest rates, foreign exchange rates, foreign interest rates and equity. We will now add the model of a foreign stock. Let $\tilde{S}$ denote another stock process, modeling a stock from the foreign market, i.e. the process $\tilde{S}$ has the dimension (currency unit) 1for. 

## 26.3.0.1. Dynamic of the Foreign Stock under Spot-Measure

We assume that the foreign stock $\tilde{S}$ follows a lognormal process 

$$
\mathrm{d} \tilde {S} (t) = \mu^ {\tilde {S}, \mathbb {P}} (t) \tilde {S} (t) \mathrm{d} t + \sigma^ {\tilde {S}} (t) \tilde {S} (t) \mathrm{d} W ^ {\tilde {S}, \mathbb {P}} (t) \quad \text { under   the   real   measure } \mathbb {P}.
$$

As in the previous Sections 26.1 and 26.2, we chose as numéraire $N(t) := P(T_{m(t)+1}; t) \prod_{j=0}^{m(t)} (1 + L_j(T_j) \cdot \delta_j)$ . As for the Cross-Currency LIBOR Market Model, the foreign stock $\tilde{S}$ has to be converted to domestic currency to be a traded asset for the domestic investor. I.e. $FX \cdot \tilde{S}$ is a traded asset and the $N$ -relative price $\frac{FX\cdot\tilde{S}}{N}$ a $\mathbb{Q}^N$ -martingale. From the product rule 

$$
\mathrm{d} \left(\frac {F X \cdot \tilde {S}}{N}\right) = \mathrm{d} (F X \cdot \tilde {S}) \cdot \frac {1}{N} + F X \cdot \tilde {S} \cdot \mathrm{d} \left(\frac {1}{N}\right) + \mathrm{d} (F X \cdot \tilde {S}) \cdot \mathrm{d} \left(\frac {1}{N}\right)
$$

and 

$$
\mathrm{d} (F X \cdot \tilde {S}) = \mathrm{d} F X \cdot \tilde {S} + F X \cdot \mathrm{d} \tilde {S} + \mathrm{d} F X \cdot \mathrm{d} \tilde {S}.
$$

With the definition of the numéraire from Remark 231 und 232 

$$
\mathrm{d} (\frac {1}{N}) = (\frac {\partial}{\partial t} \frac {1}{N}) \mathrm{d} t = (\frac {1}{N} \cdot \frac {\partial}{\partial t} \log (\frac {1}{N})) \mathrm{d} t
$$

and thus 

$$
\begin{array}{l} \operatorname{Drift} \left(\frac {F X \cdot \tilde {S}}{N}\right) \\ = \frac {F X \cdot \tilde {S}}{N} \cdot \left(\mu^ {F X} + \mu^ {\tilde {S}} + \sigma^ {F X} (t) \mathrm{d} W _ {F X} ^ {\mathbb {Q} ^ {N}} (t) \cdot \sigma^ {\tilde {S}} (t) \mathrm{d} W _ {\tilde {S}} ^ {\mathbb {Q} ^ {N}} (t) + \frac {\partial}{\partial t} \log \left(\frac {1}{N}\right)\right) \end{array}
$$

If we denote the instantaneous correlation of the stock process $\tilde{S}$ and the foreign exchange rate process $FX$ by $\rho_{FX,\tilde{S}}$ , i.e. we have $\mathrm{d}W_{FX}^{\mathbb{Q}^N}(t)\cdot \mathrm{d}W_{\tilde{S}}^{\mathbb{Q}^N}(t) = \rho_{FX,\tilde{S}}\mathrm{d}t$ , then we get with $\mathrm{Drift}_{\mathbb{Q}^N}\left(\frac{FX.\tilde{S}}{N}\right) = 0$ 

$$
\mu^ {\tilde {S}} = - \mu^ {F X} - \frac {\partial}{\partial t} \log \big (\frac {1}{N} \big) - \sigma^ {F X} (t) \sigma^ {\tilde {S}} (t) \rho_ {F X, \tilde {S}} (t)).
$$

With 

$$
\mu^ {F X} (t) = \frac {\partial}{\partial t} \log \left(\frac {P (T _ {m (t) + 1} ; t)}{\tilde {P} (T _ {m (t) + 1} ; t)}\right)
$$

and 

$$
\frac {\partial}{\partial t} \log \left(\frac {1}{N}\right) = \frac {\partial}{\partial t} \log \left(\frac {1}{P (T _ {m (t) + 1} ; t)}\right)
$$

we get 

$$
\begin{array}{l} \mu^ {\tilde {S}} = \frac {\partial}{\partial t} \log (\tilde {P} (T _ {m (t) + 1}; t)) - \sigma^ {F X} (t) \sigma^ {\tilde {S}} (t) \rho_ {F X, \tilde {S}} (t)) \\ = - \frac {\partial}{\partial t} \log \Big (1 + \tilde {L} _ {m (t)} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t) \Big) - \sigma^ {F X} (t) \sigma^ {\tilde {S}} (t) \rho_ {F X, \tilde {S}} (t)). \end{array}
$$

## 26.3.1. Summary

Under the numéraire 

$$
N (t) := P \left(T _ {m (t) + 1}; t\right) \prod_ {j = 0} ^ {m (t)} \left(1 + L _ {j} \left(T _ {j}\right) \cdot \delta_ {j}\right),
$$

where $m(t) := \max\{i : T_i \leq t\}$ , and the assumption that $N(t)$ does not have a diffusion part, as would be the case for 

$$
\left. \begin{array}{l} P (T _ {i + 1}; t) := \big (1 + L _ {i} (T _ {i}) \cdot (T _ {i + 1} - t) \big) ^ {- 1} \\ \tilde {P} (T _ {i + 1}; t) := \big (1 + \tilde {L} _ {i} (T _ {i}) \cdot (T _ {i + 1} - t) \big) ^ {- 1} \end{array} \right\} \quad \text { for } T _ {i} <   t <   T _ {i + 1},\tag{26.6}
$$

the dynamic of the Equity-Hybrid Cross-Currency LIBOR Market Model under the corresponding martingale measure $Q^{N}$ (spot measure) is given by 

$$
\mathrm{d} L _ {i} (t) = L _ {i} (t) \cdot \mu_ {i} (t) \mathrm{d} t + L _ {i} (t) \sigma_ {i} (t) \mathrm{d} W _ {i} ^ {\mathbb {Q} ^ {N}} (t) \quad \text {for i = 0,\ldots,n - 1 ,}
$$

$$
\mathrm{d} F X (t) = F X (t) \cdot \mu^ {F X} (t) \mathrm{d} t + F X (t) \sigma^ {F X} (t) \mathrm{d} W _ {F X} ^ {\mathbb {Q} ^ {N}} (t)
$$

$$
\mathrm{d} \tilde {L} _ {i} (t) = \tilde {L} _ {i} (t) \cdot \tilde {\mu} _ {i} (t) \mathrm{d} t + \tilde {L} _ {i} (t) \tilde {\sigma} _ {i} (t) \mathrm{d} \tilde {W} _ {i} ^ {\mathbb {Q} ^ {N}} (t) \qquad \text {for} i = 0, \ldots , n - 1,
$$

$$
\mathrm{d} S (t) = S (t) \mu^ {S} (t) \mathrm{d} t + S (t) \sigma^ {S} (t) \mathrm{d} W _ {S} ^ {\mathbb {Q} ^ {N}} (t)
$$

$$
\mathrm{d} \tilde {S} (t) = \tilde {S} (t) \mu^ {\tilde {S}} (t) \mathrm{d} t + \tilde {S} (t) \sigma^ {\tilde {S}} (t) \mathrm{d} W _ {\tilde {S}} ^ {\mathbb {Q} ^ {N}} (t)
$$

where 

$$
\mu_ {i} = \sum_ {l = m (t) + 1} ^ {i} \frac {\delta_ {l} L _ {l}}{(1 + \delta_ {l} L _ {l})} \sigma_ {i} \sigma_ {l} \rho_ {i, l},
$$

$$
\tilde {\mu} _ {i} (t) = \sum_ {j = m (t) + 1} ^ {i} \frac {\delta_ {j} \tilde {L} _ {j}}{(1 + \delta_ {j} \tilde {L} _ {j})} \tilde {\sigma} _ {i} \tilde {\sigma} _ {j} \tilde {\rho} _ {i, j} - \tilde {\sigma} _ {i} \sigma^ {F X} (t) \rho_ {\tilde {i}, \mathrm{FX}},
$$

$$
\mu^ {F X} (t) = \frac {\partial}{\partial t} \log \left(\frac {P (T _ {m (t) + 1} ; t)}{\tilde {P} (T _ {m (t) + 1} ; t)}\right)
$$

$$
\mu^ {S} (t) = \frac {\partial}{\partial t} \log (P (T _ {m (t) + 1}; t))
$$

$$
\mu^ {\tilde {S}} (t) = \frac {\partial}{\partial t} \log (\tilde {P} (T _ {m (t) + 1}; t)) - \sigma^ {F X} (t) \sigma^ {\tilde {S}} (t) \rho_ {F X, \tilde {S}} (t).
$$

If we choose for $P(T_{m(t) + 1};t)$ and $\tilde{P} (T_{m(t) + 1};t)$ the interpolation given in (26.6), then it follows that 

$$
\begin{array}{r l} & {\mu^ {F X} (t) = \frac {\partial}{\partial t} \log \left(\frac {1 + \tilde {L} _ {m (t)} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t)}{1 + L _ {m (t)} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t)}\right)} \\ & {\mu^ {\mathcal {S}} (t) = \frac {\partial}{\partial t} \log \left(\frac {1}{1 + L _ {m (t)} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t)}\right)} \\ & {\mu^ {\tilde {\mathcal {S}}} (t) = \frac {\partial}{\partial t} \log \left(\frac {1}{1 + \tilde {L} _ {m (t)} (T _ {m (t)}) \cdot (T _ {m (t) + 1} - t)}\right) - \sigma^ {F X} (t) \sigma^ {\tilde {\mathcal {S}}} (t) \rho_ {F X, \tilde {\mathcal {S}}} (t).} \end{array}
$$

## 26.3.2. Implementation

Due to the many state variables, i.e. the high Markov dimension, it is natural to consider an implementation to be path simulation (Monte-Carlo simulation). The first step towards an implementation is the discretization of the simulation time t by suitable discretization scheme. Since the processes are lognormal processes, we use the Euler-scheme for the log-process, see Section 13.1, 13.1.2.3. 

The discretization of the interest rate processes $L_{i}$ has been presented in Section 19.1.3, the interest rate processes of the foreign currency rates $\tilde{L}_{i}$ are discretized likewise. For FX we find 

$$
\begin{array}{l} F X (t + \Delta t) \\ = F X (t) \cdot \exp \big (\int_ {t} ^ {t + \Delta t} \mu^ {F X} (\tau) - \frac {1}{2} \sigma^ {F X} (\tau) ^ {2} \mathrm{d} \tau + \int_ {t} ^ {t + \Delta t} \sigma^ {F X} (\tau) \mathrm{d} W ^ {F X} (\tau) \big) \\ = F X (t) \cdot \exp \big ((\bar {\mu} ^ {F X} (t) - \frac {1}{2} \bar {\sigma} ^ {F X} (t) ^ {2}) \Delta t + \bar {\sigma} ^ {F X} (t) \Delta W ^ {F X} (t) \big) \end{array}
$$

with $\Delta W^{FX}(t):= W^{FX}(t + \Delta t) - W^{FX}(t)$ and 

$$
\begin{array}{l} \bar {\mu} ^ {F X} (t) := \frac {1}{\Delta t} \int_ {t} ^ {t + \Delta t} \mu^ {F X} (\tau) \mathrm{d} \tau \\ \bar {\sigma} ^ {F X} (t) := \sqrt {\frac {1}{\Delta t} \int_ {t} ^ {t + \Delta t} \sigma^ {F X} (\tau) ^ {2} \mathrm{d} \tau} \end{array}
$$

If we especially choose the time discretization of the Monte-Carlo Simulation to match the tenor structure $T_{0}, T_{1}, T_{2}, \ldots$ , then we have 

$$
F X (T _ {i + 1}) \quad = \quad F X (T _ {i}) \cdot \exp \left(\bar {\mu} ^ {F X} (T _ {i}) \Delta T _ {i} - \frac {1}{2} \bar {\sigma} ^ {F X} (T _ {i}) ^ {2} \Delta T _ {i} + \bar {\sigma} ^ {F X} (T _ {i}) \Delta W ^ {F X} (T _ {i})\right),
$$

with $\Delta T_{i} := T_{i+1} - T_{i}$ and $\Delta W^{FX}(T_{i}) := W^{FX}(T_{i+1}) - W^{FX}(T_{i})$ and 

$$
\begin{array}{l} \bar {\mu} ^ {F X} (T _ {i}) = \frac {1}{\Delta T _ {i}} \int_ {T _ {i}} ^ {T _ {i + 1}} \mu^ {F X} (\tau) \mathrm{d} \tau \\ \qquad = \frac {1}{\Delta T _ {i}} \log \left(\frac {1 + \tilde {L} _ {i} (T _ {i}) \cdot (T _ {i + 1} - t)}{1 + L _ {i} (T _ {i}) \cdot (T _ {i + 1} - t)}\right) \bigg | _ {t = T _ {i}} ^ {T _ {i + 1}} \\ \qquad = \frac {1}{\Delta T _ {i}} \log \left(\frac {1 + L _ {i} (T _ {i}) \cdot (T _ {i + 1} - T _ {i})}{1 + \tilde {L} _ {i} (T _ {i}) \cdot (T _ {i + 1} - T _ {i})}\right) \\ \bar {\sigma} ^ {F X} (T _ {i}) := \sqrt {\frac {1}{\Delta T _ {i}} \int_ {T _ {i}} ^ {T _ {i + 1}} \sigma^ {F X} (\tau) ^ {2} \mathrm{d} \tau}. \end{array}
$$

This Euler discretization is exact. The discretization of the processes S and $\tilde{S}$ follows likewise. With “discrete drift term” 

$$
\begin{array}{l} \bar {\mu} ^ {S} (T _ {i}) = \frac {1}{\Delta T _ {i}} \log (1 + L _ {i} (T _ {i}) \cdot (T _ {i + 1} - T _ {i})), \\ \bar {\mu} ^ {\tilde {S}} (T _ {i}) = \frac {1}{\Delta T _ {i}} \log (1 + \tilde {L} _ {i} (T _ {i}) \cdot (T _ {i + 1} - T _ {i})) - \int_ {T _ {i}} ^ {T _ {i + 1}} \sigma^ {F X} (t) \sigma^ {\tilde {S}} (t) \rho_ {F X, \tilde {S}} (t) \mathrm{d} t. \end{array}
$$

Part VII.
Implementation 

# Object-Oriented Implementation in Java™

From early on, we wanted a product that would seem so natural and so inevitable and so simple, you almost wouldn't think of it as having been designed. 

Jonathan Ive iPod™ Design Team, Apple Computer, [37]. 

## 27.1. Elements of Object Oriented Programming: Class and Objects

First we define the two concepts class and object. 

Definition 233 (Class): 

A class consists of 

• A description of a data structure. 

- A description of a set of functions, the methods that act on the data structures and other data (given as arguments). The description of the methods consists of 

- A description of the calling convention of the methods, the interface, see Section 27.1.3 and Definition 236. 

- A description of how the method (function) actually acts on the data, the implementation. 

## Definition 234 (Object):

We say that $X$ is an object of the class $K$ , if 

- $X$ provides memory to store data according to the structure (layout) described by $K$ and 

- the methods described in $K$ may be applied to the data in $X$ . 

In this case, $K$ is also called the type of $X$ . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/be6b3520ae6144a69e86f7ce862fd41dfa0b935cdbaaa18792bc1357ec037281.jpg)


Interpretation: A class is the blue print of an object, while an object is a real instance of the class. 

Considering how a classes and objects are realized in a computer, it becomes apparent that an object X of class K merely stores the data according to the storage layout in K, while the algorithms (code) that operate on X are given by K. The class is a description of the storage layout and the functionality, while the object represents the corresponding data record. The definition of a class exists only once, while object of a class (data records) may exist multiple times. Class and object distinguish between logic (code) and data. Obviously, the logic, i.e. the class, has to know the layout (structure) of the data. 

To illustrate the relation of classes and objects some authors use an analogy like, e.g., human is a class while the specific individual “Christian Fries” is an object of the class human. Such analogies do not hold very far. For example it does not become apparent that an object is just a data storage, dis-functional without the class and that the code, i.e. the algorithm that acts on the data exists only once, namely inside the class. However, each individual has its own experiences (data) and patterns of (re-)action (code processing experiences). 

That the code is stored only inside the class also becomes apparent in the memory requirements: If we add a data field to a class and create 100 objects (instances) of this class, then, of course, this consumes 100 times the memory of the new data field. If a new method is added to a class then its code is stored only once and the memory requirement is totally independent of the number of objects created. 

As well as the data described in the class, an object carries another data item, namely its type. This type specifies the class of the objects. Thus there is a link back from the object to the class and thus to the methods that may be invoked on the objects' data. 

## 27.1.1. Example: Class of a Binomial Distributed Random Variable

Let B denote a binomial distributed random variable defined over a probability space $(\Omega, \mathcal{F}, P)$ with $\Omega = \{\omega_{1}, \omega_{2}\}$ . Probability space and random variable may be characterized by three values $b_{1}, b_{2}, p \in R$ : 

$$
\begin{array}{l l} B (\omega_ {1}) = b _ {1}, & P (\omega_ {1}) = p \\ B (\omega_ {2}) = b _ {2}, & P (\omega_ {2}) = 1 - p. \end{array}\tag{27.1}
$$

Equation (27.1) describes the class of “binomial distributed random variables” while the random variable C with 

$$
\begin{array}{l l} C (\omega_ {1}) = 1, & P (\omega_ {1}) = 0. 5 \\ C (\omega_ {2}) = - 1, & P (\omega_ {2}) = 0. 5. \end{array}\tag{27.2}
$$

is a (specific) object, i.e. an instance of the class “binomial distributed random variable”. Of course, operators that may be applied to this random variable have to be defined only on the class level. For example, the calculation of the mean is defined by 

$$
\mathrm{E} ^ {\mathbb {P}} (B) = \int_ {\Omega} B \mathrm{d} P = p \cdot B (\omega_ {1}) + (1 - p) \cdot B (\omega_ {2}) = p \cdot b _ {1} + (1 - p) \cdot b _ {2}.\tag{27.3}
$$

That $\operatorname{E}(C) = 0.5 \cdot 1.0 + 0.5 \cdot (-1.0) = 0.0$ follows from (27.3). 

In Java $^{TM}$ a corresponding class could look as follows: The class definition starts (after a comment) with the description of the data layout, here value1, value2 and probabilityOfState1 for $b_{1}, b_{2}$ and p respectively. 

Listing 27.1: BinomialDistributedRandomVariable: A class for binomial distributed random variables 

```java
package com.christianfries.finmath.tutorial.example1;
/**
 * @author Christian Fries
 * @version 1.0
 */
class BinomialDistributedRandomVariable {
    private double value1;
    private double value2;
    private double probabilityOfState1;
} 
```

## followed by the constructor

```java
/**
 * This class implements a binomial distributed random variable
 * @param value1 The value in state 1.
 * @param value2 The value in state 2.
 * @param probabilityOfState1 The probability of state 1.
 */
public BinomialDistributedRandomVariable(double value1, double value2, double probabilityOfState1) {
    this.value1 = value1;
    this.value2 = value2;
    this.probabilityOfState1 = probabilityOfState1;
} 
```

and the description of the method getExpectation. 

```txt
/**
 * @return The expectation of the random variable
 */
public double getExpectation() {
    double expectation = probabilityOfState1 * value1
    + (1-probabilityOfState1) * value2;
    return expectation;
}
} 
```

## 27.1.2. Constructor

The constructor of a class is a (special) method that is called upon the instantiation (construction) of an object (there may be many different constructors and then it is possible to choose which constructor is called). With a constructor it is possible to do additional initializations beyond the allocation of the memory - in our case the initializations are setting the value of $b_{1}$ , $b_{2}$ and p. 

The code of the above constructor of the class BinomialDistributedRandomVariable may be confusing: The arguments of the constructor have the same names as the data fields of the class. This is allowed, and is often used for data initialization in constructors, but is dangerously confusing in other methods with longer code. In this case the corresponding name always denotes the argument of the constructor (or method). To access the data field with the corresponding name the prefix this. has to be added. So the constructor above sets the data fields of the object to the values given by the arguments. 

## 27.1.3. Methods: Getter, Setter, Static Methods

## 27.1.3.1. Calling Convention, Signatures

The calling convention of a method is the name of the methods together with the list of its argument types, i.e. the calling convention defines which name and argument type have to be used to call a method. The list of argument types is called the signature of a method. Two methods of the same name but with different signature are seen as different methods. Providing another method with the same name but a different signature is called overloading the method. $^{1}$ 

## 27.1.3.2. Getter, Setter

If the data fields of an object are made accessible, then they may be accessed through objectName.dataFieldName, i.e. they may be read or modified. The access to the data fields of an object may be allowed or denied, see also data hiding in Section 27.2.1. 

After an object has been constructed data fields may still be changed by means of methods. We may set the data or get the data. Methods that do this are called setter or getter. It is a convention that all getter methods start with the prefix get and all setter methods start with the prefix set, both followed a name of the entity they modify, starting with a capital letter. 

We add a setter for the value of $b_{1}$ to the class definition: 

```java
/**
 * @param value1 The value of state 1.
 */
public void setValue1(double value1) {
    this.value1 = value1;
} 
```

The method only changes the state of object and thus does not return a value. This is indicated by the keyword void. 

## 27.1.3.3. Static Methods

Methods that do not require knowledge of the data fields of an object, i.e. that do not read or modify data from an object, are called static methods. Put differently: The method does not need an object, it is sufficient to have the class definition. 

## Definition 235 (static method):

A method of class $K$ which keeps objects of the class $K$ invariant and is independent of its data is called static. A static method is also called a class method. 

In Java $^{TM}$ method is declared static by the keyword static. 

To apply the (non-static) method to data we (have to) create objects. A corresponding code, demonstrating how to work with object of the toy class above by doing some tests is given in the main-method $^{2}$ . 

```java
public static void main(String args[]) {
    /*
    * Test of class BinomialDistributedRandomVariable
    */
    System.out.println("Creating_random_variable.");
    BinomialDistributedRandomVariable randomVariable = new BinomialDistributedRandomVariable(1.0, -1.0, 0.5); // Create object 
```

$^{1}$ Within a class there can not be two methods with the same name and the same signature. The return value may not be changed by overloading. 

$^{2}$ The main-method may be called from outside without requiring a corresponding object. It is static. Thus (especially since it does not require the existence of an object) it may function as a possible entry point to a program. 

```java
double expectation = randomVariable.getExpectation(); 34
    System.out.println("Expectation_is:_" + expectation); 35
    System.out.println("Changing_value_of_state_1_to_0.4."); 36
    randomVariable.setValue(0.4);
    expectation = randomVariable.getExpectation(); 37
    System.out.println("Expectation_is:_" + expectation); 38
} 
```

In line 33 we create a new object of the type BinomialDistributedRandomVariable by using the keyword new (reserving the memory corresponding to the data layout) followed by the specification of the constructor to use (note that the constructor is essentially a method having the same name as the class) (right side of =). The result is stored in an object reference of type BinomialDistributedRandomVariable (left side of =). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/d716240a2c2871cd89510ff33b10756ae7ffc876c6daef14b5c06401c7c958cd.jpg)


Further Reading: In [12, 36]: primitive types, object references, static methods (the keyword static), return values (the keyword void), the main-method, comments and the JavaDoc standard. 

## 27.2. Principles of Object Oriented Programming: Data Hiding, Abstraction, Inheritance, Polymorphism

## 27.2.1. Encapsulation and Interfaces

To access the data of an object there are two possible ways: One is to provide two (or more) methods that allow us to read and modify the data, i.e. getters and setters are implemented. In our example class BinomialDistributedRandomVariable we provide an example of this for the data field probabilityOfState1: 

## Listing 27.2: Getter and setter

```java
/**
 * @return Returns the probability of state 1.
 */
public double getProbabilityOfState1() {
    return probabilityOfState1;
}

/**
 * @param probabilityOfState1 The probability of state 1.
 */
public void setProbabilityOfState1(double probabilityOfState1) {
    this.probabilityOfState1 = probabilityOfState1;
} 
```

## The use of these methods could look as follows:

```txt
BinomialDistributedRandomVariable randomVariable =
    new BinomialDistributedRandomVariable(1.0,-1.0,0.5);

double p = randomVariable.getProbabilityOfState1(); // Get probability of state 1
System.out.println("Current_value_of_p_is:" + p);

randomVariable.setProbabilityOfState1(0.3); // Change probability of state 1 to 0.3 
```

## Another possibly is to use the direct access to the corresponding data field:

```txt
BinomialDistributedRandomVariable randomVariable =
    new BinomialDistributedRandomVariable(1.0,-1.0,0.5);

double p = randomVariable.probabilityOfState1; // Get probability of state 1
System.out.println("Current_value_of_p_is:" + p);

randomVariable.probabilityOfState1 = 0.3; // Change probability of state 1 to 0.3 
```

The last variant works without special methods. $^{3}$ It is the direct access to the internal data of the object. 

This kind of access to the data structure appears to be more convenient for both the developer who does not need to implement special getter and setter methods as well as for the user of the class. Direct access to the internal data structure of a class has to be allowed explicitly. To allow direct access to a data field the keyword public has to be used: 

```java
class BinomialDistributedRandomVariable {
public double value1;
public double value2;
public double probabilityOfState1; 
```

## 27.2.1.1. Encapsulation

Hiding the internal data structure and implementation and thus denying direct access to the data structure is called encapsulation. The fundamental advantage of encapsulation is that the data structure and the way the methods process that data may be changed. Users of the class, having access to methods on the objects only, may be left untouched by such changes. From “outside” the class behaves as before. 

The advantage of encapsulation may be illustrated with the very simple example of a binomial distributed random variable. We give two examples: 

Example of Encapsulation: Offering alternative methods Like the getter and setter for the probability $P(\{\omega_{1}\})$ of the state $\omega_{1}$ we offer a getter and setter for the probability $P(\{\omega_{2}\})$ of the state $\omega_{2}$ : 

```java
/**
 * @return Returns the probability of state 2.
 */
public double getProbabilityOfState2() {
    return 1.0 - probabilityOfState1;
}

/**
 * @param probabilityOfState2 The probability of state 2.
 */
public void setProbabilityOfState2(double probabilityOfState2) {
    this.probabilityOfState1 = 1.0 - probabilityOfState2;
} 
```

Previously, the state $\omega_{1}$ was distinguished by the methods available (only its probability p could be read) and the probability of the state $\omega_{2}$ was a derived quantity $P(\{\omega_{2}\}) = 1 - p$ . Now both states are equally represented. How the properties of a binomial distributed random variable are represented internally, i.e. how the data is store, cannot be inferred from outside. It is possible to change the data layout and keep the specification (behaviour) of the methods unchanged by adapting their implementation. 

Example of Encapsulation: Performance improvement by adding a cache to the internal data modell The data model described in Listing reflst:BinomialDistributedRandomVariable consists of $B(\omega_{1})$ (value1), $B(\omega_{2})$ (value2) and $P(\{\omega_{1}\})$ (probabilityOfState1). As a consequence we have to calculate the expectation as 

$$
\operatorname{E} (B) := p \cdot (B (\omega_ {1}) + (1 - p) \cdot B (\omega_ {2})) = p \cdot (B (\omega_ {1}) - B (\omega_ {2})) + B (\omega_ {2}).
$$

$^{3}$ As long as access to the data is allowed, in Java $^{TM}$ this is done by adding the keyword public before the data. 

This is done by the method getExpectation(). If this method is called very often we may improve performance by calculating the result once and storing it in a cache. We add a data field mean as cache 

```txt
class BinomialDistributedRandomVariable {
    private double value1;
    private double value2;
    private double probabilityOfState1;
    private double mean; // Cache for the mean 
```

which is updated to the mean by the method updateMean 

```java
private void updateMean() {
    mean = probabilityOfState1 * value1 + (1-probabilityOfState1) * value2;
} 
```

In addition we add a call to updateMean() at the end of the constructor as well as at the end of any setter modifying the state of the object, i.e. modifying the data. This ensures that the field mean contains the valid mean. The method getExpectation does not do any calculations, but merely returns the value from the cache mean: 

```java
/**
 * @return The expectation of the random variable
 */
public double getExpectation() {
    return mean;
} 
```

A multiply call to getExpectation does not result in a multiple calculation of the (same) mean. 

Obviously, the user must not gain access to the field mean of a corresponding mean. This would be fatal. The lines 

```txt
System.out.println("Creating_random_variable.");
BinomialDistributedRandomVariable randomVariable = new BinomialDistributedRandomVariable(1.0,-1.0,0.5); // Create object
randomVariable.mean = 0.2; 
```

would put the object randomVariable into an inconsistent state. The user must neither assume the existence of a cache nor manipulate it. Thus both mean and updateMean are declared private. All other data fields also have to be declared private. If they are changed, then mean has to be recalculated. This is ensured by adding a call to updateMean to any setter. A direct manipulation of the data fields would disable this. 

## 27.2.1.2. Interfaces

The advantage of encapsulation is that the internal data layout may be changed if required. By adapting the implementation of the methods which is also hidden it is ensured that the methods offer the same functionality as before. For the user of (the objects of) a class it is only relevant to know the calling convention of the methods, the interface 

## Definition 236 (Interface):

The description of the calling convention of methods is called the interface. Similar to Definition 233 an interface consists of 

- A description of the calling convention of a set of functions, the methods. 

## Definition 237 (Encapsulation):

If a class offers its functionality only through an interface, then we call the class encapsulated. This is called encapsulation. 

```txt
Lizensiert fuer <ayonbd2000@yahoo.com> (Muntasir Hasan)  
This work is licensed under a Creative Commons License.  
http://creativecommons.org/licenses/by-nc-nd/2.5/deed.en 
```

An example of an interface for an discrete real valued random variable, i.e. a real valued random variable defined over a space $\Omega = \{\omega_{1}, \ldots, \omega_{n}\}$ , is given by 

Listing 27.3: DiscreteRandomVariableInterface: Interface description of a discrete random variable 

```java
/*
 * Created on 04.12.2004
 *
 * (c) Copyright Christian P. Fries, Germany. All rights reserved. Contact: email@christian-fries.de.
 */
package com.christianfries.finmath.tutorial.randomVariables;

/**
 * This is the interface for a discrete real valued random variable.
 *
 * @author Christian Fries
 */
public interface DiscreteRandomVariableInterface {
    int getNumberOfStates();
    double getProbabilityOfState(int stateIndex);
    double getValueOfState(int stateIndex);

    double getExpectation();
    double getVariance();
} 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/97334448866d60d918c539497e342b8d513466aea37bd2025ab7ea5ab6c7f15c.jpg)



Further Reading: In [12, 36]: The keywords public, private and protected for data fields and interfaces.


## 27.2.2. Abstraction and Inheritance

Interface and class are two extremes and something in between may be considered, namely classes in which some methods have an implementation, while others are given only through their calling convention (i.e. as an interface). Methods for which the implementation is not yet specified are called abstract methods. 

An example may be given by considering the interface DiscreteRandomVariableInterface above: The implementation of expectation and variance may be added without the knowledge of the internal data layout of the class. It is possible to add a partial implementation. $^{4}$ 

Listing 27.4: DiscreteRandomVariable: Abstract base class for a discrete random variable 

```java
/*
 * Created on 05.12.2004
 *
 * (c) Copyright Christian P. Fries, Germany. All rights reserved. Contact: email@christian-fries.de.
 */
package com.christianfries.finmath.tutorial.randomVariables;

/**
 * @author Christian Fries
 */
public abstract class DiscreteRandomVariable implements DiscreteRandomVariableInterface {
    public double getExpectation() {
    double expectation = 0.0;
    for(int stateIndex=0; stateIndex<this NumberedStates(); stateIndex++) {
    expectation += this.getValueOfState(stateIndex) * this.getProbabilityOfState(stateIndex);
    }
    return expectation;
    }

    public double getVariance() {

    // Calculate second moment
    double secondMoment = 0.0;
    for(int stateIndex=0; stateIndex<this NumberedStates(); stateIndex++) {
    double value = this.getValueOfState(stateIndex);
    secondMoment += value * value * this.getProbabilityOfState(stateIndex);
    } 
```

$^{4}$ An abstract class does not need to have any data layout. 

```javascript
// Calculate expectation
double expectation = this.getExpectation();

// Return variance
return secondMoment - expectation*expectation;
} 
```

To define a class which provides an implementation to the interface DiscreteRandomVariableInterface is only necessary to extend the class DiscreteRandomVariable with the implementations of the remaining abstract methods. This is possible in an elegant way by specifying that the new class should inherit the already defined properties from DiscreteRandomVariable. By doing so we may define a (new) class for the binomial distributed random variable: 

Listing 27.5: BinomialDistributedRandomVariable: 

DiscreteRandomVariable 

derived from 

```dart
/*
 * Created on 05.12.2004
 *
 * (c) Copyright Christian P. Fries, Germany. All rights reserved. Contact: email@christian-fries.de.
 */
package com.christianfries.finmath.tutorial.randomVariables;

/**
 * @author Christian Fries
 * @version 1.0
 */
class BinomialDistributedRandomVariable extends DiscreteRandomVariable {

    double value1;
    double value2;
    double probabilityOfState1;

    class ChangeOfMeasureException extends Exception {
    String cause;

    /**
    * @param cause The reason for this exception.
    */
    public ChangeOfMeasureException(String cause) {
    super(cause);
    this.cause = cause;
    }
    }

    /**
    * This class implements a binomial distributed random variable
    *
    * @param value1 The value in state 1.
    * @param value2 The value in state 2.
    * @param probabilityOfState1 The probability of state 1.
    */
    public BinomialDistributedRandomVariable(double value1, double value2, double probabilityOfState1) {
    this.value1 = value1;
    this.value2 = value2;
    this.probabilityOfState1 = probabilityOfState1;
    }

    public int getNumberOfStates() {
    return 2;
    }

    public double getProbabilityOfState(int stateIndex) {
    if (stateIndex == 0)
    return probabilityOfState1;
    else 
    return 1.0 - probabilityOfState1;
    }

    public double getValueOfState(int stateIndex) {
    if (stateIndex == 0)
    return value1;
    else 
    return value2;
    }

    public void changeMeasureToMatchGivenExpectation(double expectation)
    throws ArithmeticException, ChangeOfMeasureException {

    // Check if we have anything to do
    if (expectation == this.getExpectation()) return; // Noting to do here

    // Check if change of measure is possible: check if random variable is stochastic
    if (value1 == value2)
    throw new ArithmeticException("Random_variable_is_not_stochastic.");
} 
```

```txt
// Calculate candidate for new measure
double quasiProbability = (expectation - value2) / (value1 - value2);

if (quasiProbability < 0 || quasiProbability > 1)
    throw new ChangeOfMeasureException("Given_expectation_out_of_possible_range.");
// Check if change of measure is possible
probabilityOfState1 = quasiProbability;
} 
```

Inheritance is not limited to the implementation of abstract methods, i.e. inheriting from abstract classes. It is also possible to inherit from a class (not necessarily abstract) and to extend this class by a new data layout, new methods or new implementation of existing methods. 

## Definition 238 (Inherited Class):

Let A and B denote classes. B is called inherited from A, if B implements (at least) the interface of A. B is also called derived class. A is called base class, also super class. 

If class $B$ is inherited from $A$ , then all objects of type $B$ are simultaneously objects of the type $A$ , they are polymorph, see Definition 240. 

A convenient element of inheritance is the possibility of using the implementation of the base class by default. If the derived class does not provide an implementation for a base class method, then the implementation is inherited from the base class. To be precise, a call to a method on an object of the derived class is routed automatically to the base class object if the derived class does not provide an implementation. The method then works on the data fields of the base class object. 

## Definition 239 (Overwriting (a method)):

Supplying a new implementation to a method of a base class in a derived class is called over-writing the method. 

## 27.2.3. Polymorphism

The property that objects of a derived class are of multiple types is very important. Since the derived class implements the interface defined by the super class, objects of the derived class's type may be used equally well in all applications of base class objects. This is possible and meaningful because these objects may simultaneously be seen as objects of type A (type of the super class) and as objects of type B (type of the derived class). We say that these objects are polymorph. $^{5}$ If a base class is itself a derived class, then objects of the derived class have all types of all base classes. 

## Definition 240 (Polymorph):

An object is called polymorph, if it is of multiple type and behaves according to its derived type, even if it is used in a context (originally) expecting a base class. 

The importance of polymorphism becomes apparent in the method call of polymorphic objects. Method calls on polymorphic objects use what is called late binding. There a method call on a polymorphic object is routed to the implementation of the derived class even if the call is invoked in a context originally expecting a base class. 

Remark 241 (Interface, The Message Paradigm): The concept of an interface is a central concept of object-oriented programming. Inheritance is to some extent only a short way of saying that a class offers a super-set of the interface of another class, where the shortening is 

$^{5}$ Objects are polymorph, i.e. of multiple types, not classes. 

that for methods that do not have an implementation in the derived class the implementation in the base class is used as a proxy. 

For inheritance (in Java $^{TM}$ ) there is also the concept of the type of an object (and thus the concept of polymorphism). In Java $^{TM}$ it is possible that two objects of two different classes providing methods with identical calling conventions, i.e. providing the same interfaces, are not interchangeable in their use since they are of different types. If this additional restriction (type safety) is left out, then the only characteristic of a class is the interface provided. The calling convention of a method is often interpreted as a “message which may be received by an object”. Some programming languages do not have the concept of type safety and distinguish objects only by the messages they may receive. Nice examples are Smalltalk and Objective-C. 

## 27.3. Example: A Class Structure for One Dimensional Root Finders

We consider the problem of finding a root $^{6}$ of a function $f: R \to R$ . The algorithm for seeking the root is realized in a class that does not know the special shape of the function. Instead we realize a question-answer-pattern: In each iteration the class proposes a value x (through a getter) for which it awaits the function value to be set, i.e. the class questions the function value $f(x)$ for a (chosen) x and develops a strategy for approaching the solution from the answers. 

## 27.3.1. Root Finder for General Functions

## 27.3.1.1. Interface

Such a class has to provide a method that returns the suggested point x (double getNextPoint()) and a method that receives the corresponding value $f(x)$ (void setValue(double)). Together with some methods for controlling the iteration (counting, accuracy achieved) we have to provide the following interface: 

## Listing 27.6: RootFinder: interface for a one-dimensional root finder

```java
/*
 * Created on 30.05.2004
 *
 * (c) Copyright Christian P. Fries, Germany. All rights reserved. Contact: email@christian-fries.de.
 */
package net.finmath.rootFinder;

/**
 * This is the interface for a one dimensional root finder
 * implemented as an question-and-answer algorithm.
 *
 * @author Christian Fries
 */
public interface RootFinder {

    /**
    * @return Next point for which a value should be set
    * using <code>setValue</code>.
    */
    public double getNextPoint();

    /**
    * @param value Value corresponding to point returned
    * by previous <code>getNextPoint</code> call.
    */
    public void setValue(double value);

    /**
    * @return Returns the numberOfIterations.
    */ 
```

$^{6}$ x is a root of f if $f(x)=0$ . 

```txt
public static void testRootFinder(RootFinder rootFinder) {
    System.out.println("Testing_" + rootFinder.getClass().getName() + ":");

    // Find a solution to x^3 + x^2 + x + 1 = 0
    while(rootFinder.getAccuracy() > 1E-11 && !rootFinder.isDone()) {
    double x = rootFinder.getNextPoint();

    double y = x*x*x + x*x + x + 1;    // Our test function. Analytic solution is -1.0.
    rootFinder.setValue(y);
    }

    // Print result:
    DecimalFormat formatter = new DecimalFormat("0.00E00");
    System.out.print("Root.....:" + formatter.format(rootFinder improvesPoint()) + "###");
    System.out.print("Accuracy...:" + formatter.format(rootFinder improvesAccuracy()) + "###");
    System.out.print("Iterations:_" + rootFinder NumberOfIterations() + "\n");
} 
```

```txt
CHAPTER 27. OBJECT-ORIENTED IMPLEMENTATION IN JAVA™ 
```

```java
public int getNumberOfIterations();
/**
 * @return Best point obtained so far
 */
public double getBestPoint();
/**
 * @return Returns the accuracy.
 */
public double getAccuracy();
/**
 * @return Returns the isDone.
 */
public boolean isDone();
} 
```

We still have no data layout and no specific implementation. RootFinder only describes the interface. Obviously, a class implementing a root finder according to this interface has to have some storage on the current state of the search (say a data field for the current x) to derive a strategy for seeking the root, Which strategy is used (the implementation) and which information is needed for the strategy (the data layout) is not required in order to use it. It is sufficient to know the interface. Thus we may write a method that tests a given RootFinder against some test function f without actually having a specific class implementing the RootFinder: 

## Listing 27.7: Test for RootFinder classes

## 27.3.1.2. Bisection Search

A simple root finding algorithm is the bisection search. 

## Definition 242 (Bisection Search):

Given a continuous function $f : R \mapsto R$ and $x_{1}, x_{2}$ with $f(x_{1}) \cdot f(x_{2}) < 0$ . The sequence 

$$
x _ {i + 1} = \left\{ \begin{array}{l l} \frac {x _ {i} + x _ {i - 1}}{2}, & \text { for } f (x _ {i - 1}) \cdot f (x _ {i}) <   0 \\ \frac {x _ {i} + x _ {i - 2}}{2}, & \text { else. } \end{array} \right.
$$

is called bisection search. 

The class BisectionSearch realizes this algorithm by implementing the interface RootFinder. A corresponding code is given in Appendix D.1. 

## 27.3.2. Root Finder for Functions with Analytic Derivative: Newton Method

Some root finding methods, like the Newton method, require knowledge of the derivative $f' = \frac{\partial f}{\partial x}$ . The "search strategy" of the Newton method is 

$$
x _ {i + 1} = x _ {i} - \frac {f (x _ {i})}{f ^ {\prime} (x _ {i})}.
$$

## 27.3.2.1. Interface

Obviously a corresponding class has to implement a slightly modified interface. Instead of a method setValue(double value) the interface RootFinderWithDerivative provides a method setValueAndDerivative(double value, double derivative). 

## 27.3.2.2. Newton Method

The class NewtonsMethod implements the interface RootFinderWithDerivative using a Newton method. For the Newton method the corresponding implementation looks as follows: 

Listing 27.8: NewtonsMethod: implementing the RootFinderWithDerivative interface 

```txt
/**
 * @param value
 *    The value corresponding to the point returned by previous
 *    <code>getNextPoint</code> call.
 * @param derivative
 *    The derivative corresponding to the point returned by previous
 *    <code>getNextPoint</code> call.
 */
public void setValueAndDerivative(double value, double derivative) {
    if(Math.abs(value) < accuracy)
    {
    accuracy    = Math.abs(value);
    bestPoint  = nextPoint;
    }

    // Calculate next point
    nextPoint = nextPoint - value/derivative;

    numberOfIterations++;
    return;
} 
```

## 27.3.3. Root Finder for Functions with Derivative Estimation: Secant Method

## 27.3.3.1. Inheritance

The power of inheritance and interfaces becomes apparent in the following realization of the secant method. The search strategy of the secant method is 

$$
x _ {i + 1} = x _ {i} - \frac {f (x _ {i})}{\frac {f (x _ {i}) - f (x _ {i - 1})}{x _ {i} - x _ {i - 1}}}.
$$

From that, two aspects become apparent: 

```txt
CHAPTER 27. OBJECT-ORIENTED IMPLEMENTATION IN JAVA™ 
```

- The secant method is a Newton method with an estimate for the derivative: $f'(x_i) \approx \frac{f(x_i) - f(x_{i-1})}{x_i - x_{i-1}}$ . 

- In each iteration the secant method only required knowledge of the function value $f(x_{i})$ for the proposed point $x_{i}$ . 

For the class, these properties translate to: 

- The secant method extends the class NewtonsMethod by an estimator for the derivative. 

- The secant method implements the RootFinder interface. 

Thus, a corresponding class would look as follows: 

Listing 27.9: SecantMethod: implementing the RootFinder interface 

```java
/*
 * Created on 19.02.2004
 *
 * (c) Copyright Christian P. Fries, Germany. All rights reserved. Contact: email@christian-fries.de.
 */
package net.finmath.rootFinder;

/**
 * This class implements a root finder as auestion-and-answer algorithm using
 * the secant method.
 *
 * @author Christian Fries
 * @version 1.1
 */
public class SecantMethod extends NewtonsMethod implements RootFinder {

    // We need a second guess for the initial secant
    double secondGuess;

    // State of the solver
    double currentPoint;    // Actually the same as NewtonsMethod.nextPoint
    double lastPoint;
    double價值;
    /**
    * @param firstGuess The first guess for the solver to use.
    * @param secondGuess A second guess for the solver to use (has to be different from first guess).
    */
    public SecantMethod(double firstGuess, double secondGuess) {
    super(firstGuess);
    this.secondGuess = secondGuess;
    }

    public double getNextPoint() {
    // Ask NewtonsMethods for next point and rember it as current point
    currentPoint = super.getNextPoint();
    return currentPoint;
    }
    /**
    * @param value The value corresponding to the point returned by previous <code>getNextPoint</code> call.
    */
    public void setValue(double value) {
    // Calculate approximation for derivative
    double derivative;
    if (getNumberOfIterations() == 0) {
    // This is a trick: This derivative will let Newton's method propose the second guess as next point
    derivative = value / (secondGuess - currentPoint);
    } else {
    derivative = (value - PropertyValue) / (currentPoint - lastPoint);
    }

    // Remember last point
    lastPoint = currentPoint;
    PropertyValue = value;

    super.setValueAndDerivative(value, derivative);

    return;
    }

    /**
    * @param value
    * The value corresponding to the point returned by previous
    * <code>getNextPoint</code> call.
    * @param derivative
    * The derivative corresponding to the point returned by previous
    * <code>getNextPoint</code> call.
}
```

```txt
*/
public void setValueAndDerivative(double value, double derivative) {
    // Remember last point
    lastPoint = nextPoint;
    lastValue = value;

    super.setValueAndDerivative(value, derivative);

    return;
} 
```

Remark 243 (SecantMethod): Note that in our implementation of the second method we stored the current point x of each iteration in a field currentPoint. This is not necessary, as we could have used the field nextPoint from the base class NewtonsMethod. However, then we have to make the field visible to the derived class. $^{7}$ Using the additional field currentPoint makes the derived class independent of the data model of the base class (but also a bit less efficient since the point is stored twice). 

## 27.3.3.2. Polymorphie

The class SecantMethod shows how polymorphism works. Objects of the class SecantMethod are simultaneously objects of the class NewtonMethod, since SecantMethod inherits from NewtonMethod and thus offers the corresponding interface. Thus the class SecantMethod not only implements the interface RootFinder, but also implements the interface RootFinderWithDerivative as a Newton method. It is truly polymorphic. With respect to the interface RootFinderWithDerivative behaves like a NewtonMethod (by routing calls to the base class), with respect to the interface RootFinder it implements the secant method. That the class SecantMethod may act like a NewtonMethod is not surprising: We have not change a method of the interface of the base class (no method has been overwritten). This is also apparent in out test program Listing 27.10, testing all the root finders, see 27.11. 

Remark 244 (Inheritance: Specialization and Extension): The construct “B inherits from A” is often interpreted as “B is an A”. For example “a discrete random variable is a random variable” or “a binomially distributed random variable is a discrete random variable”. The motivation for this “mnemonic trick” is the conception that the derived class B is a specialization of the base class A. This interpretation may help us to design a class hierarchy, but it is not universal. For example “the secant method is a Newton method” appears to be wrong. The use of “… extends …” in place of “… is $a(n)$ …” is much more universal. For example: “The secant method extends the Newton method by an approximation for the derivative” makes sense. And in Java $^{TM}$ the corresponding keyword is extends. 

We test the implementation of our root finders with the class TestRootFinders. Since there are only two different interfaces we have to write only two different test routines: 

Listing 27.10: Test for RootFinder and RootFinderWithDerivative classes 

```java
/*
 * Created on 02.12.2004
 *
 * (c) Copyright Christian P. Fries, Germany. All rights reserved. Contact: email@christian-fries.de.
 */
package net.finmath.rootFinder;

import java.text.DecimalFormat; 
```

$^{7}$ It would be sufficient to declare the field protected, a weaker form of public making it visible only to derived classes. 

## CHAPTER 27. OBJECT-ORIENTED IMPLEMENTATION IN JAVA™

```java
/**
 * @author Christian Fries
 */
public class TestRootFinders {
    public static void main(String[] args) {
    System.out.println("Applying_root_findders_to_x^3_+_2*y^2_+_x_+_1_=0\n");
    System.out.println("Root_findders_without_derivative:");
    System.out.println("----");
    RootFinder rootFinder;
    rootFinder = new BisectionSearch(-10.0, 10.0);
    testRootFinder(rootFinder);
    rootFinder = new RiddersMethod(-10.0, 10.0);
    testRootFinder(rootFinder);
    rootFinder = new SecantMethod(2.0, 10.0);
    testRootFinder(rootFinder);
    System.out.println("");
    System.out.println("Root_findders_with--------derivative:");
    System.out.println("----");
    RootFinderWithDerivative rootFinderWithDerivative;
    rootFinderWithDerivative = new NewtonsMethod(2.0);
    testRootFinderWithDerivative(rootFinderWithDerivative);
    rootFinderWithDerivative = new SecantMethod(2.0, 10.0);
    testRootFinderWithDerivative(rootFinderWithDerivative);
}

public static void testRootFinder(RootFinder rootFinder) {
    System.out.println("Testing_" + rootFinder.getClass().getName() + ":");

    // Find a solution to x^3 + x^2 + x + 1 = 0
    while(rootFinder.getAccuracy() > 1E-11 && !rootFinder不做()) {
    double x = rootFinder.getNextPoint();
    double y = x*x*x + x*x + x + 1;    // Our test function. Analytic solution is -1.0.
    rootFinder.setValue(y);
    }

    // Print result:
    DecimalFormat formatter = new DecimalFormat("0.00E00");
    System.out.print("Root.....:_" + formatter.format(rootFinder.getBestPoint()) + "____");
    System.out.print("Accuracy.:_" + formatter.format(rootFinder.getAccuracy()) + "____");
    System.out.print("Iterations:_" + rootFinder.getNumberOfIterations() + "\n");
}

public static void testRootFinderWithDerivative(RootFinderWithDerivative rootFinder) {
    System.out.println("Testing_" + rootFinder.getClass().getName() + ":");

    // Find a solution to x^3 + x^2 + x + 1 = 0
    while(rootFinder.getAccuracy() > 1E-11 && !rootFinder不做()) {
    double x = rootFinder.getNextPoint();
    double y = x*x*x + x*x + x + 1;
    double p = 3*x*x + 2*x + 1;

    rootFinder.setValueAndDerivative(y, p);
    }

    // Print result:
    DecimalFormat formatter = new DecimalFormat("0.00E00");
    System.out.print("Root.....:_" + formatter.format(rootFinder.getBestPoint()) + "____");
    System.out.print("Accuracy.:_" + formatter.format(rootFinder.getAccuracy()) + "____");
    System.out.print("Iterations:_" + rootFinder.getNumberOfIterations() + "\n");
}
```

## Listing 27.11: Output of the test 27.10

```txt
Applying root finders to x^3 + 2*y^2 + x + 1 = 0
Root finders without derivative:
_____
Testing net.finmath.fdml.rootFinder.BisectionSearch:
Root.....: -1,00E00 Accuracy.: 9,09E-12 Iterations: 43
Testing net.finmath.fdml.rootFinder.RiddersMethod:
Root.....: -1,00E00 Accuracy.: 3,33E-16 Iterations: 22
Testing net.finmath.fdml.rootFinder.SecantMethod:
Root.....: -1,00E00 Accuracy.: 0,00E00 Iterations: 15
Root finders with    derivative:
_____
Testing net.finmath.fdml.rootFinder.NewtonsMethod: 
```

## 27.4. Anatomy of a Java™ Class

In Figure 27.1 on Page 356 we show (part of) a Java $^{TM}$ class with the most important elements. Before the declaration of the class the name of the packet to which the class belongs is specified. The full class name is the concatenation of the packet name and the class name and it should be unique. To achieve this, the packet name is often derived from the internet address of its creator. 

This is followed by the specification of other classes used in the declaration of this class by means of the keyword import followed by the full class name. 

The declaration of the class starts with the keyword class followed by the class name and introduced by the keywords extends and implements the optional specification of a base class and the implemented interfaces. If the specification of a base class is missing, then java.lang.Object is used as a base class. Thus all objects inherit directly or indirectly from java.lang.Object. 

Following is the declaration of the data layout by a list of data fields, also called attributes. An attribute is defined by the specification of its type (primitive types, like double, int, etc., or a class) and its name. To determine its visibility (encapsulation) it may be preceded by the keywords private, protected or public. Without such a keyword the visibility private is assumed. 

The remainder of the class declaration consists of the declaration and implementation of the constructors and methods. The method name is preceded by the type of the return value (or void for a method without return value). This may be preceded by further keywords (visibility: public, private, declaration as class method: static, prevention of overwriting: final). A constructor is a method for which the name corresponds to the class name. It is public and has no return value (the keyword void is missing however). $^{8}$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/0bf9417dc6e8f7f28076b12a8a510530d97edb1d06275c126ff98c398ec56691.jpg)


Further Reading: The Java™ keywords private, protected, public, void, static, final, implements, extends, package and import in [12, 36]. 

## 27.5. Libraries

A major advantage of Java $^{™}$ is its rich set of class libraries, which may easily be incorporated due their unique package name and clear interfaces and often coming with a JavaDoc documentation. Not only basic data management like collections are available, but also numerical libraries with algorithms from linear algebra, statistic and stochastic. 

## 27.5.1. Java™ 2 Platform, Standard Edition (j2se)

The packets java.* of the Java™ 2 Platform, Standard Edition offer basic functionalities, especially for the management of lists, strings and files. 

$^{8}$ Actually, the object created should be viewed as the return value of the constructor. 

```txt
CHAPTER 27. OBJECT-ORIENTED IMPLEMENTATION IN JAVA™ 
```

```txt
Packet(s) ...: java.*
Manufacturer : Sun Microsystems
Source .....: http://java.sun.com/j2se/
Licence .....: free, see http://java.sun.com/j2se/ 
```

## 27.5.2. Java™ 2 Platform, Enterprise Edition (j2ee)

The packets javax.* of the Java™ 2 Platform, Enterprise Edition provide functionalities for the graphical user interface Swing and internet communication. 

```yaml
Packet(s) ...: javax.*
Manufacturer : Sun Microsystems
Source dotfill: http://java.sun.com/j2ee/
Licence .....: free, see http://java.sun.com/j2ee/ 
```

## 27.5.3. Colt

The Colt library offers in the packets cern.colt.* functionalities from linear algebra (matrix multiplication, matrix inversion, eigenvector decomposition) and in the packets cern.jet.* functionalities from stochastics (random number generators, distribution functions). 

```txt
Packet(s) ...: cern.colt.*,cern.jet.*,cern.clhep
Manufacturer : Wolfgang Hoschek.
Copyright (c) 1999 CERN - European Organization for Nuclear Research.
Source .....: http://dsd.lbl.gov/~hoschek/colt/
Licence .....: The packets cern.colt*,cern.jet*,cern.clhep are free for commercial use, see http://dsd.lbl.gov/~hoschek/colt/license.html. 
```

## 27.5.4. Commons-Math: The Jakarta Mathematics Library

```txt
Manufacturer : Various (Open Source), The Apache Software Foundation.
Source .....: http://jakarta.apache.org/commons/math/
Licence .....: Apache License, http://jakarta.apache.org/commons/license.html. 
```

## 27.6. Some Final Remarks

## 27.6.1. Object Oriented Design (OOD) / Unified Modeling Language (UML)

Two key advantages of object-oriented programming are the modularization of the solution of a problem by encapsulation and abstraction and the reuse and extensibility of the solution of a problem by inheritance and polymorphism. Clean interfaces allow the independent development, refinement and optimization of parts, independent both in time and personal. 

Working out an object-oriented solution starts with the definition of the interfaces. These should provide an efficient communication of the objects. The design of the interfaces (and from that the classes) is called object-oriented design (OOD), [15]. For the design of more complex solutions a graphical language may be used (a convention of symbols): the unified modeling language (UML), [28]. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/cf31f3cb2b6384b06ca8c2957681fbeb09ee2e29cf00af37e407fbedb7649b82.jpg)


Further Reading: On the object-oriented design: Design patterns in [15], UML in [28]. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/5e15ad3b12ac01b117ab42ea54de56a607914a019def5d8c132b0fff509ed4e3.jpg)



Figure 27.1.: Anatomy of Java $^{TM}$ class.


Part VIII. 

## Appendix

# Tools (Selection)

## A.1. Linear Regression

Lemma 245 (Linear Regression): Let $\Omega^{*} = \{\omega_{1},\ldots ,\omega_{n}\}$ be a given sample space, $V:$ $\Omega^{*}\to \mathbb{R}$ and $Y\coloneqq (Y_1,\dots ,Y_p):\Omega^*\rightarrow \mathbb{R}^p$ given random variables. Furthermore let 

$$
f (y _ {1}, \ldots , y _ {p}, \alpha_ {1}, \ldots , \alpha_ {p}) := \sum \alpha_ {i} y _ {i}.
$$

Then for any $\alpha^{*}$ with $X^{\mathsf{T}}X\alpha^{*} = X^{\mathsf{T}}v$ 

$$
\| V - f (Y, \alpha^ {*}) \| _ {L _ {2} (\Omega^ {*})} = \min _ {\alpha} \| V - f (Y, \alpha) \| _ {L _ {2} (\Omega^ {*})},
$$

where 

$$
X := \left( \begin{array}{c c c} Y _ {1} (\omega_ {1}) & \ldots & Y _ {p} (\omega_ {1}) \\ \vdots & & \vdots \\ Y _ {1} (\omega_ {n}) & \ldots & Y _ {p} (\omega_ {n}) \end{array} \right), \qquad v := \left( \begin{array}{c} V (\omega_ {1}) \\ \vdots \\ V (\omega_ {n}) \end{array} \right).
$$

If $(X^{\mathsf{T}}X)^{-1}$ then $\alpha^{*} := (X^{\mathsf{T}}X)^{-1}X^{\mathsf{T}}v$ . The $Y_{1}, \ldots, Y_{p}$ are called basis functions or explanatory variables. 

Proof: We have to solve the minimization problem 

$$
g (\alpha) := \| V - f (Y, \alpha) \| _ {L _ {2} (\Omega^ {*})} ^ {2} = (v - X \cdot \alpha) ^ {\top} \cdot (v - X \cdot \alpha) \to m i n.
$$

The quadratic function on the right hand side attains its minimum where the partial derivatives with respect to $\alpha_{i}$ are zero. We have 

$$
\frac {\partial g}{\partial \alpha} = 2 X ^ {\mathsf {T}} \cdot (v - X \cdot \alpha) = 2 (X ^ {\mathsf {T}} v - X ^ {\mathsf {T}} X \cdot \alpha)
$$

and thus 

$$
\frac {\partial g}{\partial \alpha} = 0 \Leftrightarrow X ^ {\mathsf {T}} v = X ^ {\mathsf {T}} X \cdot \alpha .
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/aa0555d2ecab36f9b1b30d862ce3cc6470d3c53d2725551f42243ba6eabf9b3e.jpg)


## A.2. Generation of Random Numbers

This section will consider the generation of (pseudo-)random numbers and shows how to construct a Monte-Carlo simulation from these. There are numerous methods to generate random numbers and Monte-Carlo simulations and a discussion of the various aspects of the quality of random numbers will not be discussed. We will give only an example based on the Mersenne-Twister. However, the methods presented are sufficient for most applications. 

## A.2.1. Uniform Distributed Random Variables

## A.2.1.1. Mersenne Twister

A very popular (and also very good) random number generator for $[0,1]$ -equi-distributed random numbers is the Mersenne Twister (MT 19937). The random number generator has a period length of $2^{19937}-1$ , i.e. the random numbers generated repeat for the first time after $2^{19937}$ samples. The random numbers are also equi-distributed in high dimensions (up to 623), see [83]. Based on the MT 19937 we may thus generate an n-dimensional stochastic process by drawing n sequential random numbers in each time step to calculate the increments of the stochastic process. $^{1}$ 

Many libraries contain an implementation of the MT 19937. For the most popular languages it is available as source code. 

## A.2.2. Transformation of the Random Number Distribution via the Inverse Distribution Function

If Z is an $[0,1]$ -equi-distributed random variable and $\Phi$ a cumulative distribution function, then $X := \Phi^{-1}(Z)$ is a random variable with a distribution given by $\Phi$ . If a random number generator for equi-distributed random numbers is given (e.g. the Mersenne Twister), then we draw realizations $Z(\omega_{i}), i = 1, 2, \ldots$ and obtain from $\Phi^{-1}(Z(\omega_{i}))$ realizations of X. Thus, in addition to an $[0,1]$ -equi-distributed random number generator, we only require an inverse distribution function. 

## A.2.3. Normal Distributed Random Variables

## A.2.3.1. Inverse Distribution Function

The density of the standard normal distribution is $\phi(x):=\frac{1}{\sqrt{2\pi}}\exp\left(-\frac{x^{2}}{2}\right)$ , the (cumulative) distribution function is $\Phi(x):=\int_{-\infty}^{x}\phi(\xi)\mathrm{d}\xi$ . The algorithm described in [91] gives an approximation $\tilde{\Phi}^{-1}$ of $\Phi^{-1}$ with a relative error of $\frac{|\tilde{\Phi}^{-1}-\Phi^{-1}|}{1+|\Phi^{-1}|}<10^{-15}$ . 

## A.2.3.2. Box-Muller Transformation

The Box-Muller transformation transforms two independent $[0,1]$ -equi-distributed random numbers into two independent normally distributed random numbers. 

Lemma 246 (Box-Muller Transformation): If $z_{1}$ and $z_{2}$ are two independent [0, 1]-equi-

distributed random variables, then 

$$
x _ {1} := \rho \cos (\theta), \quad x _ {2} := \rho \sin (\theta)
$$

with $\rho := \sqrt{-2\log(z_{1})}$ and $\theta := 2\pi z_{2}$ two independent normally distributed random variables with mean 0 and standard deviation 1. 

## A.2.4. Poisson Distributed Random Variables

## A.2.4.1. Inverse Distribution Function

The cumulative) distribution function of the Poisson distribution is $\Phi(\tau):=1-\exp\left(-\int_{0}^{\tau}\lambda(t)\mathrm{d}t\right)$ , where $\lambda$ denotes the intensity. If $\lambda$ is constant then 

$$
\Phi^ {- 1} (z) = - \frac {\log (1 - z)}{\lambda}.
$$

If q is the probability that an event will occur in the interval $[T_{1}, T_{2}]$ and if $\lambda$ is constant then 

$$
\lambda = - \frac {\log (1 - q)}{T _ {2} - T _ {1}}.
$$

## A.2.5. Generation of Paths of an n-dimensional Brownian Motion

Let $T_0 < T_1 < \ldots < T_m$ denote a given time discretization. We wish to generate the realization of an $N$ -dimensional Brownian motion $W := (W_1, \ldots, W_n)$ on sample paths $\omega_1, \ldots, \omega_k$ . For a single path we have to draw $n \cdot m$ random numbers. To generate the $n \cdot m$ -tuples we use the Mersenne Twister and apply a transformation. 

Let $\{z_i\}_{i=1,2,\ldots}$ denote the sequence of $[0,1]$ -equi-distributed random numbers drawn from the Mersenne Twister. Then $\{\Phi^{-1}(z_i)\}_{i=1,2,\ldots}$ is a sequence of standard normally distributed random variables. If normalDistribution.nextDouble() is a method returning a new element of the sequence $\{\Phi^{-1}(z_i)\}_{i=1,2,\ldots}$ upon each call, then a time-discrete Brownian motion is generated by the code in Listing A.1. 

## Listing A.1: Generation of an n -dimensional Brownian motion

```java
/**
 * This class represents a multidimensional brownian motion W = (W(1), ..., W(n))
 * where W(i), W(j) are uncorrelated for i not equal j.
 * Here the dimension n is called factors since this brownian motion is used to
 * generate multi-dimensional multi-factor Ito processes and there one might use
 * a different number of factors to generate Ito processes of different dimension.
 *
 * @author Christian Fries
 * @version 1.1
 */
public class BrownianMotion {
    double[][][] brownianIncrement;

    double[] timeDiscretization;
    int numberOfFactors;
    int numberOfPaths;
    int seed; 
```

```typescript
private void doGenerateBrownianMotion() {
    // Create random number sequence generator
    AbstractDistribution normalDistribution = new Normal(0,1,new MersenneTwister64(seed));
    // Allocate memory
    brownianIncrement = new double[(timeDiscretization.length-1)][numberOfFactors][numberOfPaths]; 
```

```txt
// Precalculate square roots of deltaT
double[] sqrtOfTimeStep = new double[timeDiscretization.length-1];
for(int timeIndex=0; timeIndex<timeDiscretization.length-1; timeIndex++) {
    sqrtOfTimeStep[timeIndex]
    = Math.sqrt(timeDiscretization[timeIndex+1]-timeDiscretization[timeIndex]);
}

// Set increments
for(int path=0; path<numberOfPaths; path++) {
    for(int timeIndex=0; timeIndex<timeDiscretization.length-1; timeIndex++) {
    double sqrtDeltaT = sqrtOfTimeStep[timeIndex];
    // Generate uncorrelated Brownian increment
    for(int factor=0; factor<numberOfFactors; factor++) {
    brownianIncrement[timeIndex][factor][path] = normalDistribution.nextDouble() * sqrtDeltaT;
    }
    }
    }
} 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/d544927a332e554fcbffa3f6c5a7ed8fc88a8354f8716a6b5dc79272c620afd7.jpg)


## Tip (Generation of paths of time-discrete stochastic processes):

The Mersenne Twister is equi-distributed in 623 dimensions. How well this property is preserved in higher dimensions is not clear. For an n-dimensional Brownian motion with independent increments we have first the requirement that 

the increments are derived through a transformation of independent equi-distributed random variables. For this reason it is advisable to generate the random numbers of the n increments of the n-dimensional processes in a sequence (i.e. as an n-tuple). Furthermore we have the requirement of the temporal independence of the m increments of the stochastic process, here the increments $\Delta W(T_{i}) := W(T_{i+1}) - W(T_{i})$ of the Brownian motion. Thus, a path $\omega$ corresponds to the realization of an $n \cdot m$ -dimensional random variable, here 

$$
(\Delta W _ {j} (T _ {i})) _ {j = 1, \dots , n, i = 1, \dots , m}.
$$

In other words: If we have to generate paths of an n-dimensional process with m time steps, then we draw an $n \cdot m$ -tuple for every paths. This requires the random number generator to create the desired distribution in $n \cdot m$ dimensions. Thus, the high dimension of the Mersenne Twister is of interest to our application. With the Mersenne Twister we may, e.g., generate a 7-dimensional Process with 89 time steps ( $7 \cdot 89 = 623$ ). $^{2}$ 

Thus, the order of the loops in Listing A.1 has been chosen deliberately. 

< 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/0e5cc973e2705982c7609ec5aeca7b8b22febce0243e2463cb30524800e7a3c7.jpg)


Further Reading: For the generation of random numbers, especially in the context of Monte-Carlo simulations and derivative pricing, see $[18]$ . Background information on the Mersenne Twister and references to its source code and libraries may be found in the Wikipedia article “Mersenne Twister”, http: 

//de.wikipedia.org/wiki/Mersenne_Twister. 

# A.3. Factor Decomposition - Generation of Correlated Brownian Motion

Lemma 247 (Factor decomposition): Let $R = (\rho_{i,j})_{i,j=1\ldots n}$ denote a given correlation matrix. Thus $R$ is symmetric and positive semi-definite. This implies that $R$ has real eigenvalues $\lambda_1 \geq \ldots \geq \lambda_n \geq 0$ and that a corresponding ortho-normal basis of eigenvectors $v_1, \ldots, v_n$ of $R$ exists, i.e. 

$$
\exists V: \quad V ^ {\mathrm{T}} R V = D := \left( \begin{array}{c c c} \lambda_ {1} & & 0 \\ 0 & \ddots & 0 \\ 0 & & \lambda_ {n} \end{array} \right), \qquad \text { where } V = (v _ {1}, \ldots , v _ {n}).
$$

and $R = VDV^{\mathrm{T}}$ as well as $V^{\mathrm{T}}V = I$ . 

Let $U_{1},\ldots,U_{n}$ denote independent Brownian motions, $U:=(U_{1},\ldots,U_{n})^{\mathrm{T}}$ . Then W with 

$$
\mathrm{d} W := \left(\mathrm{d} W _ {1}, \dots , \mathrm{d} W _ {n}\right) ^ {\mathrm{T}} := V \sqrt {D} \mathrm{d} U
$$

is an n-dimensional Brownian motion with 

$$
<   \mathrm{d} W _ {i}, \mathrm{d} W _ {j} > = \rho_ {i, j} \mathrm{d} t.
$$

With $F := (v_{1} \sqrt{\lambda_{1}}, \ldots, v_{n} \sqrt{\lambda_{n}})$ we thus have $\mathrm{d}W = F\mathrm{d}U$ . 

Proof: Obviously, a correlation matrix is symmetric and thus its eigenvalues are all real. If R is the correlation matrix of the random variable vector $X = (X_{1}, \ldots, X_{n})^{\mathrm{T}}$ with $\operatorname{Var}(X_{i}) = 1$ and $\operatorname{E}(X_{i}) = 0$ , then $R = \operatorname{E}(X \cdot X^{\mathrm{T}})$ . If $v_{i}$ denotes the eigenvector corresponding to the eigenvalue $\lambda_{i}$ , then 

$$
\operatorname{E} (\| X ^ {\mathrm{T}} v _ {i} \| _ {l _ {2}} ^ {2}) = \operatorname{E} (v _ {i} ^ {\mathrm{T}} X \cdot X ^ {\mathrm{T}} v _ {i}) = v _ {i} ^ {\mathrm{T}} R v _ {i} = \lambda_ {i} \| v _ {i} \| _ {l _ {2}} ^ {2}
$$

and thus 

$$
\lambda_ {i} = \frac {\mathrm{E} (\| X ^ {\mathrm{T}} v _ {i} \| _ {l _ {2}} ^ {2})}{\| v _ {i} \| _ {l _ {2}} ^ {2}} \geq 0.
$$

Thus, R is positive semi-definite and $dW := V \sqrt{D} dU$ is well defined. 

## A.4. Factor Reduction

Using the construction of correlated Brownian motion discussed in Section A.3, we may reduce the number of relevant factors (i.e. the number of non-zero eigen values), while keeping the correlation structure close to the original correlation structure. Let R, V, D be as in Section A.3 and m < n. Using 

$$
(f _ {1}, \ldots , f _ {n}) = F = V \sqrt {D}, \qquad f _ {i} = (f _ {j, i}) _ {j = 1} ^ {n}
$$

define 

$$
F^{r} = (f_{i}^{r})_{i = 1,\ldots ,m} = (f_{j,i}^{r})_{\substack{j = 1,\ldots ,n\\ i = 1,\ldots ,m}},\qquad f_{j,i}^{r}:= \frac{f_{j,i}}{(\sum_{k}f_{j,k}^{2})^{1 / 2}},
$$

i.e. the $n \times m$ -matrix $F^r$ is calculate from the $n \times m$ -Matrix $(v_1 \sqrt{\lambda_1}, \ldots, v_m \sqrt{\lambda_m})$ by renormalizing the $n$ rows. 

Let $U_{1},\ldots,U_{m}$ denote independent Brownian motions, $U:=(U_{1},\ldots,U_{m})^{\mathrm{T}}$ . Then W defined by 

$$
\mathrm{d} W := (\mathrm{d} W _ {1}, \dots , \mathrm{d} W _ {n}) ^ {\mathrm{T}} := F ^ {r} \mathrm{d} U
$$

is an n-dimensional m-factorial Brownian motion. 

The factor reduction corresponds to a principal component analysis followed by a re-normalization of the components. 

Remark 248 (Factor Reduction): The magnitude of the absolute value of the eigenvalue of $\lambda_{i}$ represents the importance of the corresponding factor $f_{i}$ . It may be used to decide upon the number of factors to use. A simple example is given by the limit case of perfect correlation $\rho_{i,j} = 1$ . The corresponding correlation matrix has one eigenvalue n corresponding to the eigenvector $(1, \ldots, 1)$ and an n - 1-fold eigenvalue 0 corresponding to the orthogonal space. This implies that the dynamic of the n dimensional Brownian motion may be explained by a one-dimensional Brownian motion (one factor). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/76cf9704f0fbb7403ec1c62c3f07ed695b1b96d201bcc3c73def7be86d652467.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/d6531d2df1c7725bad59eaeacd0a7f016b59d526e51e7527b477e26b5387cb46.jpg)



Figure A.1.: Factor reduction in the case of high correlation: The factors $f_{i}$ (eigenvectors) of the correlation matrix $\rho_{i,j} = \exp(-0.005 * |i - j|)$ (left) and a reduction to the three factors having the largest eigenvalues (right).


In Figure A.1 we depict a reduction to the first three factors for the case of a high correlation $\rho_{i,j} = \exp(-0.005 * |i - j|)$ . However, if many factors with relatively high weight (eigenvalues) are neglected, then the factor reduction has a significant impact on the correlation structure (see Figure A.3) as well as on the shape of the remaining factors (see Figure A.2). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/78a74d2d0cebd4342a507b4c1ddf09a5503195f3b59f52a905a171dec23dfb9f.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/5e69f25b53d136667fb6e98c5afb59580def14e6d7a5c5097b960aa8ca973fdb.jpg)



Figure A.2.: Factor reduction in the case of low correlation: The factors $f_{i}$ (eigen values) of the correlation matrix $\rho_{i,j} = \exp(-0.1 * |i - j|)$ (left) and a reduction to the two factors having the largest eigenvalues (right).


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/56d8322ad92199ac10b79b2de95edf5a75758f2f54c7596f36580597bd7e81ce.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/87d6fbef4c8415968d46813cb0f957f02fb3c552a8de444063fcc7e3738b5899.jpg)



Figure A.3.: Factor reduction in the case of low correlation: The original correlation matrix $\rho_{i,j} = \exp(-0.1 * |i - j|)$ (left) and the correlation matrix corresponding to the reduction to two factors (right). This case corresponds to the factor reduction in Figure A.2.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/e09fa6e46216a696257139180b4dd305cf2575708dd26fd491bbdfc95c70fc7f.jpg)


Experiment: The impact of a factor reduction on the correlation matrix may be studied for different correlation structures at 

http://www.christian-fries.de/finmath/applets/FactorReduction.html. 

## A.5. Optimization (one-dimensional): Golden Section Search

Given a function $f : [a, b] \to R$ . Furthermore let $\lambda \in (0, 1)$ and $m_{0} = \lambda a + (1 - \lambda)b$ such that $f(m_{0}) < \min\{f(a), f(b)\}$ . Then the sequence $\{m_{i}\}_{i=0}^{\infty}$ defined by the following algorithm converges to a local minimum of f (and thus to a global minimum on [a, b], if f is strictly convex on [a, b]): 

Iteration start: 

$$
a _ {0} := a, \qquad m _ {0} := \lambda a + (1 - \lambda) b, \qquad b _ {0} := b
$$

Iteration step: 

- If $b_{i} - m_{i} > m_{i} - a_{i}$ then set $z := \lambda m_{i} + (1 - \lambda)b_{i}$ and 

$$
\text {if} f (m _ {i}) <   f (z) \colon \left\{ \begin{array}{l l} a _ {i + 1} & := a _ {i} \\ m _ {i + 1} & := m _ {i} \\ b _ {i + 1} & := z \end{array} \right\} \qquad \text {else:} \left\{ \begin{array}{l l} a _ {i + 1} & := m _ {i} \\ m _ {i + 1} & := z \\ b _ {i + 1} & := b _ {i} \end{array} \right\}.
$$

- If $b_{i} - m_{i} \leq m_{i} - a_{i}$ then set $z := \lambda a_{i} + (1 - \lambda)m_{i}$ and 

$$
\text {if} f (z) <   f (m _ {i}) \colon \left\{ \begin{array}{l l} a _ {i + 1} & := a _ {i} \\ m _ {i + 1} & := z \\ b _ {i + 1} & := m _ {i} \end{array} \right\} \qquad \text {else:} \left\{ \begin{array}{l l} a _ {i + 1} & := z \\ m _ {i + 1} & := m _ {i} \\ b _ {i + 1} & := b _ {i} \end{array} \right\}.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/426a5eea-c5be-4b9d-ae93-0413162bf4b6/5bbe938ff15a3a2b437f8d2cc7f9f2886953342a6bed7fe0fa80be4735e5ef6c.jpg)



Figure A.4.: Golden Section Search


The algorithm places a point $(z)$ into the larger of the two intervals $[a, m]$ , $[m, b]$ and from the resulting three intervals it rejects the one that is adjacent to the larger value of $f(m)$ , $f(z)$ . 

For the division ratio $\lambda$ the value 

$$
\lambda = \frac {3 - \sqrt {5}}{2}
$$

is optimal in the following sense: In the worst case, in which the algorithm rejects the smaller intervall and retains the larger interval at every iteration step, then the value $\lambda = \frac{3 - \sqrt{5}}{2}$ will result in the fastest convergence rate. Since this ratio is the golden section, the algorithm is called the Golden Section Search. 

## A.6. Convolution with Normal Density

Lemma 249 (Integration of $\exp(a \cdot X)$ , $X$ normally distributed): It is 

$$
\int_ {h _ {1}} ^ {h _ {2}} e ^ {a \cdot x} \cdot \phi (x; y, \sigma) d x = \left[ \Phi \left(\frac {h _ {2} - (y + a \sigma^ {2})}{\sigma}\right) - \Phi \left(\frac {h _ {1} - (y + a \sigma^ {2})}{\sigma}\right) \right] e ^ {a y + \frac {a ^ {2} \sigma^ {2}}{2}},
$$

where $\phi (\xi ;\mu ,\sigma) = \frac{1}{\sqrt{2\pi}\sigma}\cdot e^{-\frac{(\xi - \mu)^2}{2\sigma^2}}$ denotes the density and $\Phi (x):= \int_{-\infty}^{x}\phi (\xi ;0,1)\mathrm{d}\xi$ denotes the distribution function of the normal distribution. In particular: 

$$
\int_ {- \infty} ^ {\infty} e ^ {a \cdot x} \cdot \phi (x; y, \sigma) d x = e ^ {a y + \frac {a ^ {2} \sigma^ {2}}{2}}.
$$

Proof: It is 

$$
\begin{array}{r l} \int_ {h _ {1}} ^ {h _ {2}} e ^ {a \cdot x} \cdot \phi (x; y, \sigma) \mathrm{d} x & = \frac {1}{\sqrt {2 \pi} \sigma} \int_ {h _ {1}} ^ {h _ {2}} e ^ {a \cdot x} \cdot e ^ {- \frac {1}{2} (\frac {x - y}{\sigma}) ^ {2}} \mathrm{d} x \\ & = \frac {1}{\sqrt {2 \pi} \sigma} \int_ {h _ {1}} ^ {h _ {2}} \exp (a \cdot x - \frac {1}{2} (\frac {x - y}{\sigma}) ^ {2}) \mathrm{d} x. \end{array}
$$

Since 

$$
\begin{array}{l} \exp (a \cdot x - \frac {1}{2} (\frac {x - y}{\sigma}) ^ {2}) \\ \quad = \exp (a \cdot x - \frac {1}{2 \sigma^ {2}} (x ^ {2} - 2 x \cdot y + y ^ {2})) \\ \quad = \exp (- \frac {1}{2 \sigma^ {2}} (x ^ {2} - 2 x \cdot y + y ^ {2} - 2 a \sigma^ {2} \cdot x)) \\ \quad = \exp (- \frac {1}{2 \sigma^ {2}} (x ^ {2} - 2 x (y + a \sigma^ {2}) + y ^ {2})) \\ \quad = \exp (- \frac {1}{2 \sigma^ {2}} (x ^ {2} - 2 x (y + a \sigma^ {2}) + (y + a \sigma^ {2}) ^ {2} - 2 a \sigma^ {2} y - a ^ {2} \sigma^ {4})) \\ \quad = \exp (- \frac {1}{2 \sigma^ {2}} (x ^ {2} - 2 x (y + a \sigma^ {2}) + (y + a \sigma^ {2}) ^ {2}) \cdot \exp (a y + \frac {a ^ {2} \sigma^ {2}}{2}) \\ \quad = \exp (- \frac {(x - (y + a \sigma^ {2})) ^ {2}}{2 \sigma^ {2}} \cdot \exp (a y + \frac {a ^ {2} \sigma^ {2}}{2}), \end{array}
$$

it follows that 

$$
\begin{array}{l} \int_ {h _ {1}} ^ {h _ {2}} e ^ {a \cdot x} \cdot \phi (x; y, \sigma) \mathrm{d} x \\ = \frac {1}{\sqrt {2 \pi} \sigma} \int_ {h _ {1}} ^ {h _ {2}} \exp (- \frac {(x - (y + a \sigma^ {2})) ^ {2}}{2 \sigma^ {2}} \mathrm{d} x \cdot \exp (a y + \frac {a ^ {2} \sigma^ {2}}{2}) \\ = \int_ {h _ {1}} ^ {h _ {2}} \phi (x; y + a \sigma^ {2}, \sigma) \mathrm{d} x \cdot \exp (a y + \frac {a ^ {2} \sigma^ {2}}{2}). \end{array}
$$

□| 

## Exercises

In this chapter we give a small selection of exercises. The points are a rough indication of the complexity of the solution. 

Exercise 1 (Probability space, random variable [15 points]): Let $(\Omega, \mathcal{F}, P)$ denote a probability space and $X: \Omega \to \mathbb{R}$ a random variable. 

1. Give an example of a (false) modeling $\Omega, \mathcal{F}, X$ of some random experiment, such that $X$ is not $(\mathcal{F}, \mathcal{B}(\mathbb{R}))$ -measurable (give the definition of the mathematical objects and their interpretation). 

2. Now let $X$ be $(\mathcal{F},\mathcal{B}(\mathbb{R}))$ -measurable. 

a) Show that 

$$
\{X ^ {- 1} (A) \mid A \in \mathcal {B} (\mathbb {R}) \}
$$

is a $\sigma$ -algebra and a subset of $\mathcal{F}$ (sub- $\sigma$ -algebra of $\mathcal{F}$ ). Give a possible an interpretation of the object? 

b) Show that 

$$
P _ {X} (A) := P \left(X ^ {- 1} (A)\right) \quad \forall A \in \mathcal {B} (\mathbb {R}))
$$

defines a probability measure (the image measure). 

Exercise 2 (Conditional Expectation [20 points]) $^{1}$ : Let X denote an F-measurable (numerical) random variable and G a $\sigma$ -algebra with $G \subset F$ (i.e. G is a sub- $\sigma$ -algebra of F). Prove the following properties of the conditional expectation: 

1. If $X$ is a $\mathcal{G}$ -measurable random variable, then $\operatorname{E}(X|\mathcal{G}) = X$ ( $P$ -almost surely). 

2. If $X \geq 0$ , then $\operatorname{E}(X|\mathcal{G}) \geq 0$ . 

3. (Tower Law) If $\mathcal{H}$ is an $\sigma$ -algebra with $\mathcal{H} \subset \mathcal{G}$ , then $\mathrm{E}(\mathrm{E}(X|\mathcal{G})|\mathcal{H}) = \mathrm{E}(X|\mathcal{H})$ . 

4. (Taking out what is known) If Z is a bounded G-measurable random variable, then 

$$
\operatorname{E} (Z X | \mathcal {G}) = Z \operatorname{E} (X | \mathcal {G}).\tag{B.1}
$$

$^{1}$ See [41]. 

Exercise 3 (Distribution Function [10 points]) $^{2}$ : Let $X : \Omega \to R$ denote a random variable and F the distribution function of X, i.e. $F(x) := P_{X}((- \infty, x))$ . Show that: 

1. F is left continuous, i.e. $F(x) = \lim_{h \nearrow 0} F(x + h)$ . 

2. If $g : R \to R$ is measurable with $\mathrm{E}(|g(X)|) < \infty$ , then 

$$
\operatorname{E} (g (X)) = \int_ {- \infty} ^ {\infty} g (x) d F (x),
$$

where the integral is interpreted as Lebesgue-Stieltjes integral (see [27]). 

Exercise 4 (Brownian Scaling [10 points]) $^{3}$ : Let W denote a Brownian motion and c > 0. Show that with 

$$
\tilde {W} (t) := \frac {1}{c} W (c ^ {2} t)
$$

$\tilde{W}$ is also a Brownian motion. Are the two processes $W$ and $\tilde{W}$ equal in any sense (c.f. Definition 20)? 

Exercise 5 (Quadratic Variation [10 points]) $^{4}$ : Let X denote a continuous stochastic process $^{5}$ . For p > 0 let the p-th variation process be defined as 

$$
<   X, X > ^ {(p)} (t, \omega) := \lim _ {\Delta t \rightarrow 0} \sum_ {t _ {k} \leq t} | X (t _ {k + 1}, \omega) - X (t _ {k + 1}, \omega) | ^ {p},
$$

where $\{t_i\}_{i=1}^{\infty}$ is a strictly monotone sequence with $t_0 = 0$ , $\lim_{k \to \infty} t_k = \infty$ , $\Delta t := \sup_k |t_{k+1} - t_k|$ . The process $< X, X >^{(1)}$ is called the total variation of $X$ and the process $< X, X >:=< X, X >^{(2)}$ is called the quadratic variation of $X$ . 

Let $W$ denote a (one-dimensional) Brownian motion. 

1. Show that 

$$
<   W, W > (t, \omega) = t \quad P \text {-almost surely.}
$$

2. Show that 

$$
<   W, W > ^ {1} (t, \omega) = \infty \quad P \text {-almost surely.}
$$

Note that these properties hold pathwise for almost all paths and not only just in an averaged sense. 

Exercise 6 (Itô Integral [10 points]) $^{4}$ : Show by direct use of the definition of the Itô integrals, that 

$$
1. \int_ {0} ^ {T} t \mathrm{d} W (t) = T \cdot W (T) - \int_ {0} ^ {T} W (t) \mathrm{d} t,
$$

$$
2. \int_ {0} ^ {T} W (t) ^ {2} \mathrm{d} W (t) = \frac {1}{3} W (T) ^ {3} - \int_ {0} ^ {T} W (t) \mathrm{d} W (t).
$$

Exercise 7 (Stratonovich Integral [10 points]) $^{7}$ : Let $T^{(n)} := \{t_{0}, \ldots, t_{n}\}$ with $0 = t_{0} < t_{1} < \ldots < t_{n} = T$ denote a decomposition of the interval $[0, T]$ and $\Delta T^{(n)} := \sup_{i} |t_{i} - t_{i-1}|$ its fineness. Furthermore let $f : [0, T] \times \Omega \to R$ be of the class of integrands of the Itô integral (on $[0, T]$ ) and $t \mapsto f(t, \omega)$ continuous for (almost) all $\omega$ . Then 

$$
\int_ {0} ^ {T} f (t, \omega) \mathrm{d} W (t, \omega) = \lim _ {\Delta T ^ {(n)} \rightarrow 0} \sum_ {j = 1} ^ {n} f \left(t _ {j - 1}, \omega\right)\left(W \left(t _ {j}, \omega\right) - W \left(t _ {j - 1}, \omega\right)\right)
$$

is in $L_{2}(P)$ (proof?). The Stratonovich Integral is defined correspondingly as 

$$
\int_ {0} ^ {T} f (t, \omega) \circ \mathrm{d} W (t, \omega) = \lim _ {\Delta T ^ {(n)} \rightarrow 0} \sum_ {j = 1} ^ {n} f \left(t _ {j - \frac {1}{2}}, \omega\right)\left(W \left(t _ {j}, \omega\right) - W \left(t _ {j - 1}, \omega\right)\right)
$$

with $t_{j - \frac{1}{2}} := \frac{t_{i-1} + t_i}{2}$ . Calculate 

1. $\int_0^T W(t,\omega)\circ \mathrm{d}W(t,\omega)$ and 

$$
2. \int_ {0} ^ {T} W (t, \omega) \circ \mathrm{d} W (t, \omega) - \int_ {0} ^ {T} W (t, \omega) \mathrm{d} W (t, \omega).
$$

Solution: It is 

$$
\int_ {0} ^ {T} W (t, \omega) \circ \mathrm{d} W (t, \omega) = \lim _ {\Delta T ^ {(n)} \rightarrow 0} \sum_ {j = 1} ^ {n} W \left(t _ {j - \frac {1}{2}}, \omega\right)\left(W \left(t _ {j}, \omega\right) - W \left(t _ {j - 1}, \omega\right)\right)
$$

and 

$$
\begin{array}{r l} & W (t _ {j - \frac {1}{2}}, \omega) (W (t _ {j}, \omega) - W (t _ {j - 1}, \omega)) \\ = & W (t _ {j - \frac {1}{2}}, \omega) (W (t _ {j}, \omega) - W (t _ {j - \frac {1}{2}}, \omega)) + W (t _ {j - \frac {1}{2}}, \omega) (W (t _ {j - \frac {1}{2}}, \omega) - W (t _ {j - 1}, \omega)) \\ = & \frac {1}{2} (W (t _ {j}, \omega) + W (t _ {j - \frac {1}{2}}, \omega)) (W (t _ {j}, \omega) - W (t _ {j - \frac {1}{2}}, \omega)) \\ & - \frac {1}{2} (W (t _ {j}, \omega) - W (t _ {j - \frac {1}{2}}, \omega)) (W (t _ {j}, \omega) - W (t _ {j - \frac {1}{2}}, \omega)) \\ & + \frac {1}{2} (W (t _ {j - \frac {1}{2}}, \omega) - W (t _ {j - 1}, \omega)) (W (t _ {j - \frac {1}{2}}, \omega) - W (t _ {j - 1}, \omega)) \\ & + \frac {1}{2} (W (t _ {j - \frac {1}{2}}, \omega) + W (t _ {j - 1}, \omega)) (W (t _ {j - \frac {1}{2}}, \omega) - W (t _ {j - 1}, \omega)) \\ = & \frac {1}{2} (W (t _ {j}, \omega) ^ {2} - W (\underline {{t _ {j - \frac {1}{2}} , \omega}}) ^ {2}) + \frac {1}{2} (\underline {{W (t _ {j - \frac {1}{2}} , \omega)}} ^ {2} - W (t _ {j - 1}, \omega) ^ {2}) \\ & - \frac {1}{2} (W (t _ {j}, \omega) - W (t _ {j - \frac {1}{2}}, \omega)) (W (t _ {j}, \omega) - W (t _ {j - \frac {1}{2}}, \omega)) \\ & + \frac {1}{2} (W (t _ {j - \frac {1}{2}}, \omega) - W (s t _ {j - 1}, \omega)) (W (t _ {j - \frac {1}{2}}, \omega) - W (s t _ {j - 1}, \omega)) \\ = & \frac {1}{2} (W (t _ {j}, \omega) ^ {2} - W (s t _ {j - 1}, \omega) ^ {2}) \\ & - \frac {1}{2} (W (t _ {j}, \omega) - W (s t _ {j - \frac {1}{2}}, \omega)) ^ {2} + \frac {1}{2} (W (s t _ {j - \frac {1}{2}}, \omega) - W (s t _ {j - 1}, \omega)) ^ {2}. \end{array}
$$

$^{7}$ See [27]. 

Thus, from 

$$
\lim _ {\Delta T ^ {(n)} \rightarrow 0} \sum_ {j = 1} ^ {n} (W (t _ {j}, \omega) - W (t _ {j - \frac {1}{2}}, \omega)) ^ {2} = \lim _ {\Delta T ^ {(n)} \rightarrow 0} \sum_ {j = 1} ^ {n} (W (t _ {j - \frac {1}{2}}, \omega) - W (t _ {j - 1}, \omega)) ^ {2}
$$

we have 

$$
\int_ {0} ^ {T} W (t, \omega) \circ \mathrm{d} W (t, \omega) = \frac {1}{2} W (t _ {n}, \omega) ^ {2}.
$$

Exercise 8 (Itô Product Rule, Itô Quotient Rule [15 points]): Use the Itô formula and prove 

1. The product rule: Let X and Y denote Itô processes. Then 

$$
\mathrm{d} (X \cdot Y) = Y \cdot \mathrm{d} X + X \cdot \mathrm{d} Y + \mathrm{d} X \cdot \mathrm{d} Y
$$

2. The quotient rule: Let $X$ and $Y$ denote Itô processes, $Y > c$ for some $c \in (0, \infty)$ . Then 

$$
\mathrm{d} \left(\frac {X}{Y}\right) = \frac {X}{Y} \left(\frac {\mathrm{d} X}{X} - \frac {\mathrm{d} Y}{Y} - \frac {\mathrm{d} X}{X} \cdot \frac {\mathrm{d} Y}{Y} + \left(\frac {\mathrm{d} Y}{Y}\right) ^ {2}\right)
$$

3. The drift adjustment of a lognormal process: Let $S(t) > 0$ denote an Itô process of the form 

$$
\mathrm{d} S (t) = \mu (t) S (t) \mathrm{d} t + \sigma (t) S (t) \mathrm{d} W (t),
$$

$$
\mathrm{d} Y (t) = (\mu (t) - \frac {1}{2} \sigma^ {2} (t)) \mathrm{d} t + \sigma (t) \mathrm{d} W (t).
$$

Exercise 9 (Martingale: Itô formula [15 points]) $^{8}$ : Use the Itô formula and show that the following processes are $F_{t}$ -martingales: 

1. $X(t) = \exp(\frac{1}{2}t) \cos(W(t))$ 

2. $X(t) = \exp (\frac{1}{2} t)\sin (W(t))$ 

3. $X(t) = (t + W(t)) \exp(-\frac{1}{2} t - W(t))$ 

$(W(t) \text{ is a one-dimensional Brownian motion}).$ 

Exercise 10 (Black-Scholes partial differential equation in the coordinates t, $N(t)$ , $S(t)$ [20 points]): Show that the function 

$$
V (t, n, s)) = s \Phi (d _ {+}) - n \frac {K}{N (T)} \Phi (d _ {-})
$$

with 

$$
d _ {\pm} = \frac {1}{\bar {\sigma} \sqrt {(T - t)}} \big [ \log (\frac {s}{n} \cdot \frac {N (T)}{K}) \pm \frac {\bar {\sigma} ^ {2} (T - t)}{2} \big ].
$$

$^{8}$ See [27]. 

and $\Phi'(x) = \phi(x) = C\exp(-x^2/2)$ solves the partial differential equation 

$$
\frac {\partial V (t)}{\partial t} \mathrm{d} t + \frac {1}{2} \frac {\partial^ {2} V (t)}{\partial s \partial s} \sigma^ {2} = 0
$$

with the final time condition 

$$
V (T, N (T), s) = \max (s - K, 0).
$$

Exercise 11 (Black 76 Formula for Swaption [30 points]): Let $T_{1} < \ldots < T_{n}$ denote given times. Let $V_{\text{swap}}$ denote s swap as in Definition 117 with constant swap rates $S_{i} = K$ , $i = 1, \ldots, n - 1$ ( $T_{1}, \ldots, T_{n-1}$ are fixing dates and $T_{2}, \ldots, T_{n}$ are payment dates). Let $S$ denote the corresponding par swap rate as in Definition 122 (c.f. Remark 121). Derive the formula for the value $V_{\text{swaption}}$ of an (European) option on $V_{\text{swap}}$ (with exercise date $T_{1}$ ), assuming the $S$ has lognormal dynamics 

$$
\mathrm{d} S (t) = \mu (t) S (t) \mathrm{d} t + \sigma (t) S (t) \mathrm{d} W (t) \quad \text { unter } \mathbb {P}.
$$

Hint: First rewrite the value of the swap $V_{swap}$ as a function of S and K by transforming cash-flow: $L(T_{i}, T_{i+1}) - K = (L(T_{i}, T_{i+1}) - S) + (S - K)$ , note the definition of S. Then consider the value of the swap at exercise date of the option, i.e. $V_{\text{swap}}(T_{1})$ and try to choose a suitable numéraire (compare with the evaluation of a caplet). Say why the numéraire chosen is a traded product. 

Solution (sketched): From Definition 117 a swap pays 

$$
\left(L \left(T _ {i}, T _ {i + 1}; T _ {i}\right) - S _ {i}\right) \cdot \left(T _ {i + 1} - T _ {i}\right) \quad \text { in } T _ {i + 1}.\tag{B.2}
$$

Let $t \leq T_{1}$ . The value of the payment (B.2) in t is 

$$
\left(L \left(T _ {i}, T _ {i + 1}; T _ {i}\right) - S _ {i}\right) \cdot \left(T _ {i + 1} - T _ {i}\right) \cdot P \left(T _ {i + 1}; t\right).
$$

Thus, the value of the value of the swap in t is given by 

$$
V _ {\text { swap }} (t) = \sum_ {i = 1} ^ {n - 1} \left(L (T _ {i}, T _ {i + 1}; T _ {i}) - S _ {i}\right) \cdot (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t).
$$

By Definition 122 the par swap rate is given by 

$$
S _ {\mathrm{par}} (t) := \frac {P (T _ {1} ; t) - P (T _ {n} ; t)}{\sum_ {i = 1} ^ {n - 1} (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1} ; t)},
$$

so that 

$$
\sum_ {i = 1} ^ {n - 1} \left(L (T _ {i}, T _ {i + 1}; T _ {i}) - S _ {\text { par }} (t)\right) \cdot (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t) = 0.
$$

Thus 

$$
\begin{array}{l} V _ {\text { swap }} (t) = \sum_ {i = 1} ^ {n - 1} \left(L (T _ {i}, T _ {i + 1}; T _ {i}) - S _ {i}\right) \cdot (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t) \\ \qquad = \sum_ {i = 1} ^ {n - 1} \left(L (T _ {i}, T _ {i + 1}; T _ {i}) - S _ {\text { par }} (t)\right) \cdot (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t) \\ \qquad + \sum_ {i = 1} ^ {n - 1} \left(S _ {\text { par }} (t) - S _ {i}\right) \cdot (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t) \\ \qquad = \sum_ {i = 1} ^ {n - 1} \left(S _ {\text { par }} (t) - S _ {i}\right) \cdot (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t). \end{array}
$$

For a swap with $S_{i} = K$ this implies 

$$
\begin{array}{c} V _ {\text { swap }} (t) = (S _ {\text { par }} (t) - K) \cdot \sum_ {i = 1} ^ {n - 1} (T _ {i + 1} - T _ {i}) \cdot P (T _ {i + 1}; t) \\ = (S _ {\text { par }} (t) - K) \cdot A (t), \end{array}
$$

where $A(t) := \sum_{i=1}^{n-1}(T_{i+1} - T_i) \cdot P(T_{i+1}; t)$ is called swap annuity. Since $A(t) > 0$ we have for the value of the option on this swap 

$$
V _ {\text { swaption }} (t) = \max (S _ {\text { par }} (t) - K, 0) \cdot A (t).
$$

Now chose A as numéraire. Under the corresponding martingale measure $Q^{A}$ , S is an A-relative price, thus a martingale and thus $\mathrm{d}S(t) = \sigma(t)S(t)\mathrm{d}W^{\mathbb{Q}^{A}}(t)$ . The evaluation formula for a swaption now follows as in the derivation of the Black formula for a caplet. 

## APPENDIX C

## List of Symbols

Symbol Interpretation 

$\emptyset$ Empty set. 

1 Indicator function. $\mathbf{1}(x)=\left\{\begin{aligned}&1&\text{for }x>0,\\ &0&\text{else.}\end{aligned}\right.$ 

$\mathbf{1}_{(a,b]}(x)$ Indicator function. $\mathbf{1}_{(a,b]}(x)=\left\{\begin{aligned}&1&\text{for } x\in(a,b],\\ &0&\text{else}.\end{aligned}\right.$ 

$\mathcal{N}(\mu, \sigma^2)$ Normal distribution with mean $\mu$ and variance $\sigma^2$ . 

W Brownian motion. See Definition 28. 

P Real measure. 

$Q^{N}$ Martingale measure corresponding to the numéraire N. N-relative price processes $\frac{V}{N}$ of traded assets V are $Q^{N}$ -martingales. Exists (as a measure equivalent to P) under certain assumptions. 

[x] Gauß bracket. Largest integer, being less than or equal to x. [x] := max{n ∈ {0, 1, 2, ...} | n ≤ x} 

$\| x\| _1$ $\ell_1$ -norm of a vector $x = (x_{1},\dots ,x_{n})$ . $\| x\| _1 = \sum_{i = 1}^{n}|x_i|$ 

$\| x\| _2$ $\ell_2$ -norm of a vector $x = (x_{1},\dots ,x_{n})$ . $\| x\| _2^2 = \sum_{i = 1}^{n}|x_i|^2$ 

$P(T)$ Zero-coupon bond with maturity $T$ . $P(T)$ (in general) is a stochastic process. Evaluated at time $t$ on path $\omega$ we write $P(T; t, \omega)$ . See Definition 97. 

$L(T_{1},T_{2})$ Forward rate for the period $[T_1,T_2]$ . See Definition 99. 

$S_{i,j}$ $S_{i,j}:= S(T_i,\ldots,T_j)$ . Swap rate for the tenor structure $T_i,\ldots,T_j$ . See Definition 122. 

B Money market account. See Equation (9.6). 

$m(t)$ $m(t) := \max\{i : T_i \leq t\}$ . Projection to last fixing in tenor structure. See Definition 124. 

# Java™ Source Code (Selection)

## D.1. Java™ Classes for Chapter 27

Listing D.1: BinomialDistributedRandomVariable: A toy sample class to illustrate the concepts of “classes”, “data” and “methods”. 

```groovy
package com.christianfries.finmath.tutorial.example1;

/**
 * @author Christian Fries
 * @version 1.0
 */
class BinomialDistributedRandomVariable {

    private double value1;
    private double value2;
    private double probabilityOfState1;

    /**
    * This class implements a binomial distributed random variable
    * @param value1 The value in state 1.
    * @param value2 The value in state 2.
    * @param probabilityOfState1 The probability of state 1.
    */
    public BinomialDistributedRandomVariable(double value1, double value2, double probabilityOfState1) {
    this.value1 = value1;
    this.value2 = value2;
    this.probabilityOfState1 = probabilityOfState1;
    }

    public static void main(String args[]) {
    /*
    * Test of class BinomialDistributedRandomVariable
    */
    System.out.println("Creating_random_variable.");
    BinomialDistributedRandomVariable randomVariable = new BinomialDistributedRandomVariable(1.0,-1.0,0.5); // Create object

    double expectation = randomVariable.getExpectation();
    System.out.println("Expectation_is:_" + expectation);

    System.out.println("Changing_value_of_state_1_to_0.4.");
    randomVariable.setValue1(0.4);

    expectation = randomVariable.getExpectation();
    System.out.println("Expectation_is:_" + expectation);
    }

    /**
    * @param value1 The value of state 1.
    */
    public void setValue1(double value1) {
    this.value1 = value1;
    }

    /**
    * @return Returns the probability of state 1.
    */
    public double getProbabilityOfState1() {
    return probabilityOfState1;
    } 
```

APPENDIX D. JAVA™ SOURCE CODE (SELECTION) 

```java
/**
 * @param probabilityOfState1 The probability of state 1.
 */
public void setProbabilityOfState1(double probabilityOfState1) {
    this.probabilityOfState1 = probabilityOfState1;
}

/**
 * @return Returns the probability of state 2.
 */
public double getProbabilityOfState2() {
    return 1.0 - probabilityOfState1;
}

/**
 * @param probabilityOfState2 The probability of state 2.
 */
public void setProbabilityOfState2(double probabilityOfState2) {
    this.probabilityOfState1 = 1.0 - probabilityOfState2;
}

/**
 * @return The expectation of the random variable
 */
public double getExpectation() {
    double expectation = probabilityOfState1 * value1 + (1-probabilityOfState1) * value2;
    return expectation;
} 
```

Listing D.2: BisectionSearch: Root finder implementing the RootFinder-interface using the bisection method. 

```java
/*
 * Created on 16.02.2004
 *
 * (c) Copyright Christian P. Fries, Germany. All rights reserved. Contact: email@christian-fries.de.
 */
package net.finmath.rootFinder;

/**
 * This class implements a Bisection search algorithm,
 * implemented as a question-and-answer search algorithm.
 *
 * @author Christian Fries - http://www.christian-fries.de
 * @version 1.1
 */
public class BisectionSearch implements RootFinder {

    // We store the left and right end point of the intervall
    double[] points = new double[2]; // left, right
    double[] values = new double[2]; // left, right

    /*
    * State of solver
    */

    double nextPoint;    // Stores the next point to return bySMSPoint()
    int numberOfIterations = 0;    // Number of numberOfIterations
    double accuracy;    // Current accuracy of solution
    boolean isDone = false;    // Will be true if machine accuracy has been reached

    public static void main(String[] args) {
    // Test
    BisectionSearch search = new BisectionSearch(-1.0, 5.0);

    while (search.getAccuracy() > 1E-13 && !search.isDone()) {
    double x = search.getNextPoint();

    double y = (x - 0.656);

    search.setValue(y);
    }

    System.out.println(search.getBestPoint());
    }

    /**
    * @param leftPoint left point of search interval
    * @param rightPoint right point of search interval
    */
    public BisectionSearch(double leftPoint, double rightPoint) {
    super();
    points[0] = leftPoint;
    points[1] = rightPoint;

    nextPoint = points[0];
    accuracy = points[1]-points[0];
    }
} 
```

```java
/**
 * @return Best point obtained so far
 */
public double getBestPoint() {
    // Lazy: we always return the middle point as best point
    return (points[1] + points[0]) / 2.0;
}

/**
 * @return Next point for which a value should be set using <code>setValue</code>.
 */
public double getNextPoint() {
    return nextPoint;
}

/**
 * @param value Value corresponding to point returned by previous <code>getNextPoint</code> call.
 */
public void setValue(double value) {
    if (numberOfIterations < 2) {
    /**
    * Initially fill values
    */
    values[numberOfIterations] = value;

    if (numberOfIterations < 1) {
    nextPoint = points[numberOfIterations + 1];
    } else {
    nextPoint = (points[1] + points[0]) / 2.0;
    /**
    * @todo Check if values[0]*values[1] < 0 here
    */
    }
    } else {
    /**
    * Bisection search update rule
    */

    if (values[1] * value > 0) {
    /*
    * Throw away right point
    */
    points[1] = nextPoint;    // This is not yet the nextPoint, it is the point corresponding to value.
    values[1] = value;
    } else {
    /*
    * Throw away left point
    */
    points[0] = nextPoint;    // This is not yet the nextPoint, it is the point corresponding to value.
    values[0] = value;
    }

    // Calculate next point (bisection)
    nextPoint = (points[1] + points[0]) / 2.0;

    // Savety belt: check if still improve or if we have reached machine accuracy
    if (points[1]-points[0] >= accuracy) isDone = true;

    // Update accuracy
    accuracy = points[1]-points[0];
}

    numberOfIterations++;
    return;
}

/**
 * @return Returns the numberOfIterations.
 */
public int getNumberOfIterations() {
    return numberOfIterations;
}

/**
 * @return Returns the accuracy.
 */
public double getAccuracy() {
    return accuracy;
}

/**
 * @return Returns the isDone.
 */
public boolean isDone() {
    return isDone;
} 
```

## List of Figures

1.1 Hybrid Models 16  
1.2 The Black-Scholes model as a hybrid model 17  
1.3 On the notation 18  
2.1 Illustration of Measurability 23  
2.2 Lebesgue integral versus Riemann integral 26  
2.3 Conditional Expectation 28  
2.4 Illustration of a filtration and an adapted process 31  
2.5 Brownian motion: Time discretization 32  
2.6 Brownian motion: Paths 34  
2.7 Brownian motion with time dependent instantaneous volatility 35  
2.8 Brownian motion with drift 35  
2.9 Drift as a consequence of a non-linear function of a stochastic process 42  
2.10 Integration of stochastic processes 49  
3.1 Buy and Hold-replication strategy 55  
3.2 Replication: The two-times-two-states-two-assets example 57  
3.3 Replication: Generalization to multiple states 59  
3.4 Real Measure versus Martingale Measure 60  
6.1 Arbitrage-free option prices 82  
6.2 Linear interpolation of option prices 83  
6.3 Linear interpolation of implied volatilities 84  
6.4 Spline interpolation of option prices and implied volatilities 84  
6.5 Linear interpolation for decreasing implied volatility 85  
6.6 Linear interpolation for increasing implied volatility 86  
7.1 Samples of the value of the replication portfolio using weekly delta hedging . 101  
7.2 Delta Hedge . 102  
7.3 Samples of the value of the replication portfolio using monthly hedging: delta versus delta-gamma hedge . 104  
7.4 Samples of the value of the replication portfolio using weekly hedging with wrong interest rate . 105  
7.5 Value of the replication portfolio without re-hedging . 106  
8.1 Modeling an interest rate curve by a family of stochastic processes. . 116  
8.2 Cash-flow for a forward bond. . 117  
8.3 UML Diagram: The class DiscountFactors . 120 

8.4 UML Diagram: The class DiscountFactors with bootstrapper ..... 122
9.1 Cash-flow of a floater with exchange of notional N. ..... 125
9.2 Fixing date, payment date and evaluation date ..... 126
9.3 Call spread approximation of a digital option ..... 131
12.1 Cashflows for a coupon bond ..... 142
12.2 Cashflows for a swap ..... 142
12.3 Cashflows for a zero coupon bond ..... 143
12.4 Cashflows for a swap whose fixed leg corresponds to the zero coupon bond in Figure 12.3 ..... 143
12.5 Bermudan Swaption ..... 146
13.1 Discretization and Implementation of Itô Processes ..... 162
13.2 Monte-Carlo Simulation ..... 166
13.3 UML Diagram: Monte-Carlo Simulation / Lognormal Process ..... 167
13.4 UML Diagram: Black-Scholes Model / Monte-Carlo Simulation ..... 168
13.5 Monte-Carlo Simulation ..... 172
13.6 Lattice ..... 173
13.7 Binomial tree ..... 173
13.8 Paths of the binomial tree ..... 173
13.9 Lattice with overlaid Monte-Carlo Simulation ..... 175
15.1 Bermudan Option ..... 180
15.2 Calculation of the conditional expectation by re-simulation ..... 184
15.3 Perfect Foresight ..... 185
15.4 Predictor variable versus realized value (continuation value) ..... 186
15.5 Calculation of the conditional expectation by binning ..... 187
15.6 Continuation Value and Binning ..... 188
15.7 Regression of the conditional expectation estimator without restriction of the regression domain ..... 193
15.8 Regression of the conditional expectation estimator with restriction of the regression domain ..... 194
15.9 Regression of the conditional expectation estimator - polynomial of fourth and eighth order ..... 195
15.10 UML Diagram: Conditional Expectation Estimator ..... 196
15.11 Binning using the linear regression algorithm with piecewise constant basis functions ..... 197
15.12 Bermudan Option: Example of a successful optimization of the exercise criterion ..... 200
15.13 Bermudan Option: Example of a failing optimization of the exercise criterion ..... 200
17.1 Payoff of an auto cap under a parallel shift of the interest rate curve ..... 217
17.2 Value of an auto cap under a parallel shift of the interest rate curve ..... 217
18.1 Object-oriented design of the Monte-Carlo pricing engine ..... 231
18.2 Importance sampling using a drift adjusted proxy scheme ..... 232
18.3 Dependence of the TARN gamma on the shift size of the finite difference approximation ..... 239 

18.4 Dependence of the CMS TARN gamma on the shift size of the finite difference approximation . 240
18.5 Dependence of the CMS TARN gamma on the shift size of the finite difference approximation . 241
18.6 Dependence of the CMS TARN vega on the shift size of the finite difference approximation . 242
19.1 Swaption as a function of the forward rates . 256
19.2 UML Diagram: LIBOR Market Model / Monte-Carlo Simulation . 263
19.3 UML Diagram: LIBOR Market Model: Abstraction of model parameters . 264
19.4 UML Diagram: LIBOR Market Model: Abstraction of model parameters as volatility and correlation . 265
19.5 UML Diagram: LIBOR Market Model: Abstraction of model parameters: Parametric covariance models . 266
20.1 Correlation in a one- and multi-factor model . 273
20.2 Correlation: Full De-correlation in a One-Factor Model . 273
20.3 The terminal distribution function of a forward rate under different martingale measures . 277
20.4 The terminal distribution function of a forward rate under different martingale measures . 278
24.1 Shape of the fixed rates $L_i(T_i)$ and the interest rate curve for different instantaneous volatilities . 297
24.2 Shape of the interest rate curve with different factor configurations . 298
24.3 Shape of the fixed rates $L_i(T_i)$ and the interest rate curve with different instantaneous volatilities . 299
24.4 Shape of the fixed rates $L_i(T_i)$ and the interest rate curve with different instantaneous correlations . 301
25.1 Markov Functional Model: Calibration of the LIBOR Functionals . 317
25.2 Conditional Expectation in a Lattice . 319
25.3 State space discretization for the Markov functional model . 321
27.1 Anatomy of Java™ class . 356
A.1 Factor reduction in the case of high correlation . 364
A.2 Factor reduction in the case of low correlation - factors . 365
A.3 Factor reduction in the case of low correlation - correlations . 365
A.4 Golden Section Search . 367 

## List of Tables

7.1 Greeks within the Black-Scholes model 97   
8.1 Interest Rate Models. 119   
12.1 Prototypical product properties and corresponding model requirements and implementation techniques. 140   
12.2 Markov dimension of some models. 140   
12.3 Product Toolbox 155   
19.1 co-sliding and co-terminal swap rates 267   
20.1 Caplet and swaption prices for different instantaneous correlations and volatilities 274   
22.1 Selection of Short Rate Models 286   
24.1 Free parameters of the LIBOR Market Model considered 296 

## List of Listings

27.1 BinomialDistributedRandomVariable .... 339
27.2 Getter and setter .... 341
27.3 DiscreteRandomVariableInterface .... 344
27.4 DiscreteRandomVariable .... 344
27.5 BinomialDistributedRandomVariable: derived from DiscreteRandomVariable .... 345
27.6 RootFinder .... 347
27.7 Test for RootFinder classes .... 348
27.8 NewtonsMethod .... 349
27.9 SecantMethod .... 350
27.10 Test for RootFinder and RootFinderWithDerivative classes .... 351
27.11 Output of the test 27.10 .... 352
A.1 Generation of an n -dimensional Brownian motion .... 361
D.1 BinomialDistributedRandomVariable .... 377
D.2 BisectionSearch .... 378 

## Bibliography

## Books



[1] BAUER, HEINZ: Maßtheorie und Integrationstheorie. 2. Auflage. de Gruyter, Berlin, 1992. ISBN 3-11-013625-2. 





[2] BAUER, HEINZ: Wahrscheinlichkeitstheorie. de Gruyter, Berlin 2001. ISBN 3-11-017236-4. 





[3] BAXTER, MARTIN W.; RENNIE, ANDREW J.O.: Financial Calculus: An introduction to derivative pricing. Cambridge University Press, Cambridge, 2001. ISBN 0-521-55289-3. 





[4] BRANGER, NICOLE; SCHLAG, CHRISTIAN: Zinsderivate - Modelle und Bewertung. Springer Verlag, 2004. 199 Seiten. ISBN 3-540-21228-0. 





[5] BIERMANN, BERND: Die Mathematik von Zinsinstrumenten. Oldenbourg Verlag, 2002. ISBN 3-486-25976-8. 





[6] BINGHAM, NICHOLAS H.; KIESEL, RÜDIGER: Risk-neutral valuation: pricing and hedging of financial derivatives. (Springer Finance). Springer Verlag, London, 1998. ISBN 1-852-33458-4. 296 Seiten. 





[7] BJÖRK, THOMAS: Arbitrage Theory in Continuous Time. Oxford University Press, 1999. ISBN 0-198-77518-0. 328 Seiten. 





[8] BRIGO, DAMIANO; MERCURIO, FABIO: Interest Rate Models - Theory and Practice. Springer-Verlag, Berlin, 2001. ISBN 3-540-41772-9. 





[9] CONT, RAMA; TANKOV, PETER: Financial Modelling with Jump Processes. CRC Press, 2003. ISBN 1-584-88413-4. 





[10] DRAPER, NORMAN R.; SMITH, HARRY: Applied Regression Analysis. Third Edition. Wiley-Interscience, 1998. ISBN 0-471-02995-5. 





[11] DUFFY, DANIEL J.: Finite Difference Methods in Financial Engineering: A Partial Differential Equation Approach. John Wiley & Sons, 2006. 440 pages. ISBN 0-470-85882-6. 





[12] ECKEL, BRUCE: Thinking in Java (3rd Edition). Prentice Hall PTR, 2002. ISBN 0-131-00287-2. 





[13] EBMEYER, DIRK: Essays on Incomplete Financial Markets. Doctoral Thesis. University of Bielefeld. 





[14] HUNT, PHIL J.; KENNEDY, JOANNE E.: Financial Derivatives in Theory and Practice. John Wiley & Sons, 2000. ISBN 0-471-96717-3. 





[15] GAMMA, ERICH; HELM, RICHARD; JOHNSON, RALPH E.: Design Patterns. Addison-Wesley Professional, 1997. ISBN 0-2-016-3361-2. 





[16] GLASSERMAN, PAUL: Monte-Carlo Methods in Financial Engineering. 596 Seiten. Springer, 2003. ISBN 0-387-00451-3. 





[17] GÜNTHER, MICHAEL; JÜNGEL, ANSGAR: Finanzderivate mit MATLAB. Mathematische Modellierung und numerische Simulation. Vieweg, 2003. ISBN 3-528-03204-9. 





[18] JÄCKEL, PETER: Monte-Carlo Methods in Finance. 238 Seiten. John Wiley and Sons Ltd., 2002. ISBN 0-471-49741-X. 





[19] Joshi, Mark S.: The Concepts and Practice of Mathematical Finance. Cambridge University Press, 2003. ISBN 0-521-82355-2. 





[20] KARATZAS, IOANNIS; SHREVE, STEVEN E.: Brownian Motion and Stochastic Calculus. Second Edition. Springer Verlag, 1991. ISBN 0-387-97655-8. 





[21] KLOEDEN, PETER E.; PLATEN, ECKHARD: Numerical Solution of Stochastic Differential Equations (Applications of Mathematics. Stochastic Modelling and Applied Probability Vol. 23). Springer Verlag, 1999. ISBN 3-540-54062-8. 





[22] MALLIAVIN, PAUL: Stochastic Analysis (Grundlehren Der Mathematischen Wissenschaften). Springer Verlag, 1997. ISBN 3-540-57024-1. 





[23] MEISTER, MARKUS: Smile Modeling in the LIBOR Market Model. Diploma Thesis. University of Karlsruhe, 2004. 





[24] MUSIELA, MAREK; RUTKOWSKI, MAREK: Martingale methods in financial modeling: theory and applications. Springer-Verlag, 1997. ISBN 3-540-61477-X. 





[25] PAUL, WOLFGANG; BASCHNAGEL JÖRG: Stochastic Processes. From Physics to Finance. Springer-Verlag, 2000. ISBN 3-540-66560-9. 





[26] PELSSER, ANTOON: Efficient Methods for Valuing Interest Rate Derivatives. Springer-Verlag, 2000. ISBN 1-852-33304-9. 





[27] ∅KSENDAL, BERNT K.: Stochastic differential equations: an introduction with applications. Springer-Verlag, 2000. ISBN 3-540-63720-6. 





[28] OESTEREICH, BERND: Objektorientierte Softwareentwicklung. Oldenburg Verlag, 2004. ISBN 3-486-27266-7. 





[29] PROTTER, PHILIP E.: Stochastic Integration and Differential Equations. Springer-Verlag, 2003. ISBN 3-540-00313-4. 415 Seiten. 





[30] REBONATO, RICCARDO: Modern Pricing of Interest-Rate Derivatives: The Libor Market Model and Beyond. Princeton University Press, 2002. ISBN 0-691-08973-6. 





[31] ROGERS, L. C. G.; WILLIAMS, DAVID: Diffusions, Markov Processes and Martingales: Volume 2, Ito Calculus (2nd Edition). Cambridge University Press, 2000. ISBN 0-521-77593-0. 





[32] SEYDEL, RÜDIGER: Tools for Computational Finance. Springer Verlag, Berlin, 2003. 240 Seiten. ISBN 3-540-40604-2. 





[33] SHIRYAEV, ALBERT N.: Essentials of Stochastic Finance: Facts, Models, Theory. World Scientific Publishing Company, 1999. ISBN 9-810-23605-0. 





[34] J. MICHAEL STEELE: Stochastic Calculus and Financial Applications. Springer-Verlag, 2001. 344 pages. ISBN 0-387-95016-8 





[35] TAVELLA, DOMINGO; RANDALL CURT: Pricing Financial Instruments: The Finite Difference Method. Wiley, 2000. 237 pages. ISBN 0-471-19760-2 





[36] ULLENBOOM, CHRISTIAN: Java ist auch eine Insel, mit CD ROM. 5. Auflage. Galileo Press, 2004. ISBN 3-898-42526-6. 





[37] YOUNG, JEFFREY S.; SIMON, WILLIAM L.: iCon Steve Jobs. John Wiley & Sons, 2005. ISBN 0-471-72083-6. 





[38] WILDE, OSCAR: The Picture of Dorian Gray. ISBN 0-679-60001-9. 





[39] WILDE, OSCAR: The Importance of Being Earnest and Other Plays. Oxford University Press (Reprint). ISBN 0-198-12167-9. 





[40] WILMOTT, PAUL: Paul Wilmott on Quantitative Finance. John Wiley, 2000. ISBN 0-471-87438-8. 





[41] WILLIAMS, DAVID: Probability with Martingales. Cambridge University Press, 2002. ISBN 0-521-40605-6. (First published 1991) 





[42] WILLIAMS, DAVID: Weighing the Odds: A Course in Probability and Statistics. Cambridge University Press, 2001. ISBN 0-521-00618-X. 





[43] ZHANG, PETER: Exotic Options: A Guide to Second Generation Options, 1998. ISBN 9-810-23521-6. 



## Papers

[44] ANDERSEN, LEIF: A simple approach to the pricing of Bermudan swaptions in the multifactor Libor market model. Working paper. General Re Financial Products, 1999. 

[45] ANDERSEN, LEIF; BROADIE, MARK: A Primal-Dual Simulation Algorithm for Pricing Multi-Dimensional American Options. Working paper. General Re Financial Products, 1999. 



[46] ANDERSEN, LEIF; SIDENIUS, JAKOB; BASU, SUSANTA: All your hedges in one basket. Risk Magazine 11/2003, 67-72 (2003). 





[47] BENHAMOU, ERIC: Optimal Malliavin Weighting Function for the Computation of the Greeks. 2001. 





[48] BLACK, FISCHER: The Pricing of Commodity Contracts. Journal of Financial Economics 3, 167-179, 1976. North-Holland Publishing Company, 1976. 





[49] BOUCHAUD, JEAN-PHILIPPE; SORNETTE, DIDIER: The Black-Scholes Option Pricing Problem in Mathematical Finance: Generalizations and Extensions for a Large Class of Stochastic Processes. Journal de Physique I 4, 863, 1994. 





[50] BRACE, ALAN; GATAREK, DARIUSZ; MUSIELA, MAREK: The Market Model of Interest Rate Dynamics. Mathematical Finance 7, p. 127. Blackwell 1997. 





[51] BRASCH, HANS-JÜRGEN: A Note on Efficient Pricing and Risk Calculation of Credit Basket Products. Preprint, 2005. http://defaultrisk.com/pp_crdrv_54.htm. 





[52] BREEDEN, D. T.; LITZENBERGER, R. H.: Prices of state-contingent claims implicit in option prices. Journal of Business 51(4), 621?651, 1978. 





[53] BOYLE, PHELIM; BOADIE, MARK; GLASSERMAN, PAUL: Monte-Carlo methods for security pricing. Journal of Economic Dynamics and Control, 21, 1267-1321 (1997). 





[54] BRIGO, DAMIANO; MERCURIO, FABIO; RAPISARDA, FRANCESCO: Lognormal-mixture dynamics and calibration to market volatility smiles. 2000. http://www.damianobrigo.it 





[55] BROADIE, MARK; GLASSERMAN, PAUL: Estimating Security Price Derivatives using Simulation. Management Science, 1996, Vol. 42, No. 2, 269-285. 





[56] BROADIE, MARK; GLASSERMAN, PAUL: Pricing American-Style Securities by Simulation. Journal of Economic Dynamics and Control, 1997, Vol. 21, 1323-1352. 





[57] BROCKHAUS, OLIVER: Implied Monte-Carlo. Bachelier Conference Crete, June 2002. 





[58] CARR, PETER; THALELA, M.; ZARIPHOPOULOU, T.: Closed From option Valuation with Smiles. Working Paper (1999). 





[59] CARRIERE, JACQUES F.: Valuation of Early-Exercise Price of Options Using Simulations and Nonparametric Regression. Insurance: Mathematics and Economics 19, 19-30, 1996. 





[60] CLÉMENT, EMMANUELLE; LAMBERTON, DAMIEN; PROTTER, PHILIP: An analysis of a least squares regression method for American option pricing. Finance and Stochastics 6, 449-471, 2002. 





[61] DAVIS, MARK; KARATZAS, IOANNIS: A Deterministic Approach to Optimal Stopping, with Applications. In: Whittle, Peter (Ed.): Probability, Statistics and Optimization: A Tribute to Peter Whittle, 455-466, 1994. John Wiley & Sons, New York and Chichester, 1994. 





[62] FENGLER, MATTHIAS R.: Arbitrage-Free Smoothing of the Implied Volatility Surface. SFB 649 Discussion Paper 2005-019. Berlin. ISSN 1860-5664. http://sfb649.wiwi.hu-berlin.de/. 





[63] FOURNIÉ, ERIC; LASRY JEAN-MICHEL; LEBUCHOUX, JÉRÔME; LIONS, PIERRE-LOUIS; TOUZI, NIZAR: Applications of Malliavin calculus to Monte-Carlo methods in finance. Finance Stochastics. 3, 391-412 (1999). Springer- Verlag 1999. 





[64] FRIES, CHRISTIAN P.: The Foresight Bias in Monte-Carlo Pricing of Options with Early Exercise: Classification, Calculation and Removal. 2005.
http://www.christian-fries.de/finmath/foresightbias. 





[65] FRIES, CHRISTIAN P.; JOSHI, MARK S.: Partial Proxy Simulation Schemes for Generic and Robust Monte-Carlo Greeks. 2006. http://www.christian-fries.de/finmath/proxyscheme 





[66] FRIES, CHRISTIAN P.; KAMPEN, JÖRG: Proxy Simulation Schemes for generic robust Monte-Carlo sensitivities, process oriented importance sampling and high accuracy drift approximation (with applications to the LIBOR Market Model). 2005. http://www.christian-fries.de/finmath/proxyscheme 





[67] FRIES, CHRISTIAN P.; ROTT, MARIUS G.: Cross Currency and Hybrid Markov Functional Models. Preprint, 2004. http://www.christian-fries.de/finmath/markovfunctional 





[68] GLASSERMAN, PAUL; LI, JINGYI: Importance Sampling for Portfolio Credit Risk. Working paper, Columbia University (2003). http://www2.gsb.columbia.edu/faculty/pglasserman/Other/is_credit.pdf. 





[69] GLASSERMAN, PAUL; ZHAO, XIAOLIANG: Arbitrage-free discretization of lognormal forward Libor and swap rate models. Finance and Stochastics 4, 35-68, 2000. Springer-Verlag, 2000. 





[70] GLASSERMAN, PAUL; ZHAO, XIAOLING: Fast greeks in forward LIBOR models. Journal of Computational Finance. 3, 5-39 (1999). 





[71] HAGAN, PATRIK S.; KUMAR, DEEP; LESNIEWSKI, ANDREW S.; WOODWARD, DIANA E.: Managing Smile Risk (SABR Model), Wilmott Magazin, September 2002. 





[72] HAGAN, PATRIK S.; WEST, GRAEME: Interpolation Methods for Curve Construction. Preprint. 2005. 





[73] HAUGH, MARTIN; KOGAN, LEONIS: Pricing American Options: A Duality Approach, MIT Sloan Working Paper No. 4340-01, 2001. 





[74] HEATH, DAVID; JARROW, ROBERT; MORTON, ANDREW: Bond Pricing and the Term Structure of Interest Rates: A New Methodology for Contingent Claims Valuation. Econometrica 60, No. 1 (January), 77-105, 1992. 





[75] HUNT, PHIL J.; KENNEDY, JOANNE E.; PELSSER, ANTOON: Markov-Functional Interest Rate Models. Finance and Stochastics, Volume 4 (4), 391-408, 2000. Springer-Verlag, 2000. Reprinted in: Hughston, Lane (ed.): The New Interest Rate Models, RISK Publications. 





[76] HUNTER, CHRISTOPHER J.; JÄCKEL, PETER; JOSHI, MARK S.: Drift Approximations in a Forward-Rate-Based LIBOR Market Model. Getting the Drift. Risk 14, 81-84 (July, 2001). 





[77] JAMSHIDIAN, FARSHID: LIBOR and swap market models and measures. Finance and Stochastics 1, 293-330 (1997). Springer-Verlag, 1997. 





[78] Joshi, Mark S.: Applying Importance Sampling to Pricing Single Tranches of CDOs in a One-Factor Li Model. QUARC, Group Risk Management, Royal Bank of Scotland. Working paper, 2004. 





[79] JOSHI, MARK S.; KAINTH, DHERMINDER: Rapid computation of prices and deltas of $n^{th}$ to default swaps in the Li Model. Quantitative Finance, volume 4, issue 3, (June 04), p. 266-275.
http://www.quarchome.org/. 





[80] KOHL-LANDGRAF, PETER: A PDE Approach to the Valuation of Interest Rate Products under Markovian Yield Curve Dynamics. Diploma-Thesis. University of Bayreuth. 2007. 





[81] Li,D.: On Default Correlation: a Copula Approach (Journal of Fixed Income, 9, 43-45) 





[82] LONGSTAFF, FRANCIS A.; SCHWARTZ EDUARDO S.: Valuing American Options by Simulation: A Simple Least-Square Approach. Review of Financial Studies 14:1, 113-147, 2001. 





[83] MATSUMOTO, M.; NISHIMURA, T.: Mersenne twister: A 623-dimensionally equidistributed uniform pseudorandom number generator. ACM Transactions on Modeling and Computer Simulations, 1998. 





[84] MILTERSEN, KRISTIAN R.; SANDMANN, KLAUS; SONDERMANN, DIETER: Closed Form Solutions for Term Structure Derivatives with Lognormal Interest Rates. Journal of Finance 52, 409-430 (1997). 





[85] PITERBARG, VLADIMIR V.: A practitioner's guide to pricing and hedging callable LIBOR exotics in forward LIBOR models, Preprint. 2003. 





[86] PITERBARG, VLADIMIR V.: Computing deltas of callable LIBOR exotics in forward LIBOR models. Journal of Computational Finance. 7 (2003). 





[87] ROGERS, L. C. G.: Monte-Carlo valuation of American options, Preprint. 2001. 





[88] ROTT, MARIUS G.; FRIES, CHRISTIAN P.: Fast and Robust Monte-Carlo CDO Sensitivities and their Efficient Object Oriented Implementation. 2005. http://www.christian-fries.de/finmath/cdogreeks 





[89] SCHLÖGL, ERIK: A Multicurrency Extension of the Lognormal Interest Rate Market Models. Finance and Stochastics 6 (2), 173-196 (2002). Springer-Verlag, 2002. 





[90] SCHLÖGL, ERIK: Arbitrage-Free Interpolation in Models of Market Observable Interest Rates. Preprint (2002). 





[91] WICHURA, MICHAEL J.: Algorithm AS 241: The percentage points of the normal distribution. Applied Statistics 37, 477-484, 1988. 



## Index

## A

abstract method .... 344
accrued interest .... 123
annuity .... 374
arbitrage-free option prices .... 81
arrears .... 211
auto cap .... 152, 211 

## B

backward algorithm ..... 174, 182
– for short rate models ..... 286
base class ..... 346
Bermudan ..... 145
Bermudan callable ..... 180, 181
– structured swap ..... 146
Bermudan cancelable ..... 147
Bermudan option ..... 145, 154, 179–181
Bermudan swaption ..... 145, 146
binning ..... 186
binomial tree ..... 173
– paths ..... 173
bisection search ..... 348
Black model ..... 133
Black volatility ..... 134
Black-Derman-Toy model ..... 286
Black-Karasinski model ..... 286
Black-Scholes
– partial differential equation ..... 92, 95
– pde ..... 92, 95
Black-Scholes model
– delta hedge ..... 100
– delta-gamma hedge ..... 103 

- evaluation via Monte-Carlo ..... 167
- greeks ..... 97
Black-Scholes volatility ..... 75, 78
Black-Scholes-Merton formula ..... 77, 94
Black-Scholes-Merton model ..... 75–78
bond ..... 116
- forward bond ..... 117
- interpolation of prices ..... 327
- zero bond ..... 116
bond option ..... 131
bond volatility ..... 282
bootstrapping ..... 120
- implementation ..... 122
Borel σ-algebra ..... 22
Bouchaud-Sornette method ..... 90
Brownian motion ..... 32 

## C

cache 342, 343  
calibration 254  
call spread 131  
cancelation right 147  
canonical setup 33  
cap 130, 150  
caplet 130  
capped 130, 154  
capped CMS floater 150  
capped floater 150  
cash flow 126  
CDO 222  
change of measure theorem 45  
change of numéraire  
- cross currency 135 

chooser cap ..... 153
class ..... 337
class ..... 353
class method ..... 340
clean price ..... 123
CMS ..... 150, 151, 154, 267
CMS spread ..... 151
complete (marktet) ..... 68
compound option ..... 148
conditional expectation ..... 27–28
- calculation in a path-simulation (Monte-Carlo) ..... 184, 187
- least square approximation ..... 190
- process ..... 30
- properties ..... 369
conditional probability ..... 22
conditional variance ..... 107
constant maturity swap ..... 150
constructor ..... 339
contingent claim ..... 68
continuously compounded yield ..... 118
convergence
- weak ..... 33
correlation ..... 271–278
- definition ..... 271
- instantaneous ..... 43, 272
- terminal ..... 272
correlation model ..... 259
coupon ..... 125
coupon bond ..... 123, 141
- cash-flow diagram ..... 142
covariance
- definition ..... 271
- instantaneous ..... 272
- terminal ..... 272
Cox-Ingersoll-Ross model ..... 286
cross-currency LIBOR market model .. 325
- implementation ..... 329 

## D

data hiding 341  
data structure 337  
decomposition 371  
- fineness 371  
delta 96  
delta hedge 95 

- within Black-Scholes model ..... 100
delta-gamma hedge ..... 102
- within Black-Scholes model ..... 103
density ..... 26
- measure with density ..... 45
derived class ..... 346
design patterns ..... 355
digital caplet ..... 131
- in the Markov functional model ..... 316
- valuation ..... 131
- valuation under Black model ..... 134
dirty price ..... 123
discount factor ..... 120
discretization ..... 159
- Euler scheme ..... 161
- Milstein scheme ..... 163
- of Itô processes ..... 162
- predictor-corrector scheme ..... 163
distribution ..... 26
- terminal ..... 277, 278
distribution function ..... 26, 370
- n-dimensional ..... 26
Donsker invariance principle ..... 33
Doob-Meyer decomposition ..... 204
Dothan model ..... 286
drift ..... 35, 42, 44
drift adjustment
- of a lognormal process ..... 372 

## E

encapsulation .... 342, 343
equity hybrid LIBOR market model .... 329
equity-hybrid cross-currency LIBOR market model
- implementation .... 334
equity-hybrid LIBOR market model
- implementation .... 331
equivalent martingale measure .... see martingale measure
equivalent measure .... 45
Euler scheme .... 161
European option
- arbitrage-free prices .... 82
- interpolation of prices .... 81
- probability density of the underlying .. 79
exercise boundary .... 181 

exercise strategy .... 181  
exotic derivatives .... 139  
expectation .... 27  
extended Vasicek model .... 285  
extends .... 351, 353  
extension (inheritance) .... 351 

## F

factor loading ..... 168  
factor matrix ..... 43  
factor reduction ..... 295  
factors ..... 295  
Feynman-Kač ..... 50  
filtration ..... 30  
– generated filtration ..... 30, 36, 37  
– usual conditions ..... 45  
finite differences ..... 177  
finite elements ..... 177  
fixed leg ..... 127  
fixing date ..... 126  
flexi cap ..... 152  
floater ..... 124  
– cash-flow diagram ..... 125  
floating leg ..... 127  
floating rate bond ..... 125  
floor ..... 130, 150  
floored ..... 130, 154  
floored floater ..... 150  
floorlet ..... 130  
foreign caplet ..... 132  
foresight bias ..... 170, 189, 190  
– elimination ..... 206  
– elimination ..... 205  
forward algorithm ..... 174  
forward bond  
– cash-flow diagram ..... 117  
forward forward ..... 119  
forward FX rate ..... 136  
forward rate ..... 118  
– instantaneous ..... 118, 279  
forward volatility ..... 119  
FX ..... 132  
FX forward ..... 136 

## G

gamma 96  
getter 340  
Girsanov, Cameron, Martin theorem 45  
golden section 367  
Greeks 96  
- delta 96  
- gamma 96  
- in the Black-Scholes model 97  
- rho 96  
- theta 96  
- vega 96 

## H

Heath-Jarrow-Morton 279, 287  
- drift condition 280  
hedge 89, 90  
- static 103  
hedging 89, 90  
HJM 279, 280, 287  
Ho-Lee model 286  
Hull-White model 286 

## |

image measure ..... 23, 369
implementation ..... 337
- Black-Scholes model (via Monte-Carlo simulation) ..... 167
- cross-currency LIBOR market model ..... 329
- equity-hybrid cross-currency LIBOR market model ..... 334
- equity-hybrid LIBOR market model . 331
- LIBOR market model ..... 253, 263
implements ..... 353
implied Black volatility ..... 134
implied Black-Scholes volatility ..... 78
implied volatility ..... 87
import ..... 353
importance sampling
- using a proxy scheme ..... 232
independence
- of events ..... 22
- of random variables ..... 27
information (filtration) ..... 31
inheritance ..... 351
instance 

- of a class ..... 338
instantaneous correlation ..... 43
- definition ..... 272
- in the LIBOR Market Model .... 246, 254
- within the model for a quanto caplet . 137
instantaneous covariance
- definition ..... 272
instantaneous forward rate ..... 118, 279
integrable (with respect to a measure) ... 24
Integral ..... 24
integral ..... 49
- Itô integral ..... 36
- Lebesgue integral ..... 24, 25
- Riemann integral ..... 25
- stochastic integral ..... 49
- Stratonovich integral ..... 371
integrated covariance ..... 278
integrator ..... 39
intensity ..... 361
interest rate curve
- interpolation ..... 121
interest rates ..... 115
interface ..... 168, 337, 341, 343, 348
interpolation
- of bond prices ..... 327
- of interest rates ..... 121
- of option prices ..... 81
inverse ..... 154
Inverse CMS floater ..... 151
inverse floater ..... 150
iPod™ ..... 337
Itô calculus ..... 34–42
Itô integral ..... 36–38
- integrand ..... 37
Itô isometry ..... 37
Itô lemma ..... 40–42
- multi dimensional ..... 40
- one-dimensional ..... 40
Itô process ..... 38
- m-factorial ..... 38
- n-dimensional ..... 38
- differential notation ..... 39
- product rule ..... 41, 372
- quotient rule ..... 41, 372 

late binding ..... 346  
lattice ..... 172, 173  
– numerical integration ..... 319  
– state space discretization ..... 320, 321  
– with overlaid Monte-Carlo simulation ..... 175  
Lebesgue integral ..... 24, 25  
Lebesgue measure ..... 22  
Lebesgue-Stieltjes integral ..... 370  
LIBOR  
– definition ..... 118  
– forward LIBOR ..... 118  
LIBOR market model ..... 245  
– cross-currency LIBOR market model ..... 325  
– equity hybrid LIBOR market model .. 329  
– implementation ..... 253, 263  
– UML digram ..... 263  
linear product ..... 103  
lognormal process  
– drift adjustment ..... 41, 372 

## M

market models ..... 245  
market price of risk ..... 285  
– definition ..... 285  
Markov functional model ..... 303  
– calibration of the forward rate ..... 317  
martingale ..... 44  
– drift ..... 44  
– representation theorem ..... 44  
– super-martingale ..... 202  
martingale measure ..... 67  
mean reversion ..... 289, 295  
measurable ..... 22  
– progressively measurable ..... 31  
measurable space ..... 21  
measure ..... 21  
– $T_k$ -forward measure ..... 250  
– equivalent ..... 45  
– equivalent martingale mesure ..... 67  
– image measure ..... 369  
– risk-neutral ..... 279  
– risk-neutral measure ..... 71, 285  
– spot measure ..... 249, 326  
– swap measure ..... 267  
– terminal measure ..... 136, 154, 247, 314  
measure independent quantities ..... 278 

<!-- === Source: MinerU_markdown_Mathematical_Finance-Fries_401_2122709467580706824.md (Page 401) === -->

measure space 21  
memory 151  
Mersenne Twister 360  
method 337, 343  
- abstract 344  
Milstein scheme 163  
mixture of lognormal 87  
models  
- Black model 133  
- Black-Scholes-Merton model 75  
- Heath-Jarrow-Morton 279  
- LIBOR market model 245  
- Markov functional model 303  
- short rate model 283  
money-market account 129  
Monte-Carlo simulation 166, 172  
- weighted 166  
MT 19937 360 

## N

Neville algorithm 320  
Newton method 349  
notional 125, 127  
numéraire 58, 64 

## O

object 337  
object-oriented design 354  
Objective-C 347  
OOD 354  
optimal exercise 181  
optimal stopping problem 204  
overfitting 257  
overloading (of a method) 340 

## P

P-almost surely (footnote) 27  
par swap rate 128, 373  
partial differential equation 50, 91  
path 29  
path-dependent produkt 152  
payer swap 127  
payment date 126  
payoff 68 

PCA .... see principal component analysis
PDE .... see partial differential equation
perfect foresight ..... 184, 185
Poisson distribution ..... 361
polymorph ..... 346
polymorphism ..... 346
portfolio process ..... 63
power memory ..... 152
predictor-corrector scheme ..... 163
previsible process ..... 49
price of risk ..... 285
principal component analysis . 258, 295, 364
probability
- conditional ..... 22
probability density ..... 26
- of the underlying of a European call option ..... 79
probability space ..... 21
product
- bond option ..... 131
product rule
- Itô process ..... 372
products
- auto cap ..... 152, 211
- Bermudan ..... 145
- Bermudan callable ..... 146, 180, 181
- Bermudan cancelable ..... 147
- Bermudan option ..... 145, 179–181
- Bermudan swaption ..... 145, 146
- call spread ..... 131
- cancelable ..... 147
- cap ..... 130
- caplet ..... 130
- capped CMS floater ..... 150
- capped floater ..... 150
- chooser cap ..... 153
- CMS spread ..... 151
- compound option ..... 148
- coupon bond ..... 123
- digital caplet ..... 131
- exotic derivatives ..... 139
- flexi cap ..... 152
- floater ..... 124
- floating rate bond ..... 125
- floor ..... 130
- floored floater ..... 150
- floorlet ..... 130
- foreign-caplet ..... 132 

- inverse CMS floater ..... 151
- inverse floater ..... 150
- linear product ..... 103
- memory ..... 151
- money-market account ..... 129
- path-dependent ..... 152
- payer swap ..... 127
- power memory ..... 152
- product toolbox ..... 154
- quanto caplet ..... 132
- range accrual ..... 151
- ratchet cap ..... 152
- receiver swap ..... 127
- rolling bond ..... 129
- savings account ..... 129
- shout option ..... 153
- snowball ..... 151
- structured bond ..... 129, 141
- structured swap ..... 129, 141
- swap ..... 127
- swaption ..... 131, 256, 373
- target redemption note ..... 149
- variable maturity inverse floater ..... 149
- zero structure ..... 141
progressively measurable ..... 31
protected ..... 351
proxy simulation scheme ..... 227–241
- importance sampling ..... 232
- partial proxy ..... 233
public ..... 342 

## Q

quadratic variation 370  
quanto  
- adjustment 137  
- caplet 132  
- definition 132  
quanto caplet  
- definition 132  
- valuation (w/ FFX) 135  
quanto rate 132  
quotient rule  
- Itô process 372 

## R

random number generator .... 360
random variable .... 22
range accrual .... 151
ratchet .... 152, 154
ratchet cap .... 152
receiver swap .... 127
relative prices .... 58, 70
Rho .... 96
Riemann integral .... 24, 25
risk-neutral measure .... 71, 279
– definition .... 285
rollback .... 174
rolling bond .... 129 

## S

savings account 129  
secant method 349  
self-financing 63  
self-financing trading strategy 63  
setter 340  
short rate 119  
– definition 118  
short rate model 283  
– Black-Derman-Toy 286  
– Black-Karasinski 286  
– Cox-Ingersoll-Ross 286  
– Dothan 286  
– Ho-Lee 286  
– Hull-White 286  
– Vasicek 286  
shout option 153  
shout right 153  
σ-algebra 21  
– Borel σ-algebra 22  
– sub-σ-algebra 369  
signature (of a method) 340  
Smalltalk 347  
smile  
– caplet smile 256  
Snell envelope 203  
snowball 151  
specialization (inheritance) 351  
spot measure 249, 326  
spread 154  
state price deflator 67  
static 340 

static hedge ..... 103  
static methods ..... 340  
stochastic differential equation  
- discretization ..... 159  
stochastic integral ..... 49  
- Itô process as integrator ..... 39  
- semi-martingale as integrator ..... 50  
- with Brownian motion as integrator .. 37  
stochastic process ..... 28, 29  
- equality ..... 29  
- indistinguishable ..... 29  
- lognormal ..... 41  
- modification ..... 29  
- previsible ..... 49  
- previsible process ..... 49  
- quadratic variation ..... 370  
- stopped process ..... 203  
- total variation ..... 370  
stopped process ..... 203  
stopping-time ..... 203  
Stratonovich integral ..... 371  
structured bond ..... 129, 141  
- definition ..... 144  
structured coupon ..... 129  
structured swap ..... 129, 141  
- definition ..... 144  
super class ..... 346  
Super-martingale ..... 202  
swap ..... 127  
- cash-flow diagram ..... 142  
- payer ..... 127  
- receiver ..... 127  
- swap annuity ..... 268  
- swap measure ..... 267  
- swap rate ..... 127, 275  
swap annuity ..... 268, 275, 374  
swap measure ..... 267  
swap rate ..... 127, 128, 275  
- co-sliding ..... 267  
- co-terminal ..... 267  
- constant maturity ..... 151  
swaption ..... 131, 256  
- as function of the forward rates ..... 256  
- Black 76 formula ..... 373 

## T

taking out what is known ..... 369  
target redemption note ..... 149  
tenor structure ..... 116, 245  
term sheet ..... 154  
terminal correlation  
– definition ..... 272  
terminal covariance  
– definition ..... 272  
terminal measure ..... 136, 154, 247, 314  
Theta ..... 96  
time to maturity ..... 289 $T_{k}$ -forward measure ..... 250  
total variation ..... 370  
tower law ..... 369  
trading strategy ..... 63, 67  
– admissible ..... 67  
type  
– of an object ..... 337, 338  
– safety ..... 347 

## U

UML 167, 355  
UML diagram  
- Black-Scholes model 168  
- conditional expectation estimator 196  
- discount factors 120, 122  
- LIBOR market model 263  
- LMM covariance model 266  
- LMM model parameters 264  
- LMM plug ins 265  
- lognormal process 167  
underlying 131  
unified modeling language 167, 355  
usual conditions 45 

## V

variable maturity inverse floater ..... 149
variance
– conditional variance ..... 107
Vasicek model ..... 286
– extended Vasicek model ..... 285
Vega ..... 96
Vega Hedge ..... 105
void ..... 340
volatility 

## INDEX

- bootstrapping .... 257
- forward volatility .... 119
- implied volatility .... 78, 87
- surface .... 87
- time structure .... 289 

## W

weak convergence .... 33  
weather derivative .... 53  
weighted Monte-Carlo .... 166  
Wiener  
- measure .... 33  
- process .... 32 

## Y

yield 118 

## Z

zero coupon bond
- cash-flow diagram .... 143
zero structure .... 141
- definition .... 144
zero swap
- cash-flow diagram .... 143 

403 pages. 89 figures. 9 tables. 