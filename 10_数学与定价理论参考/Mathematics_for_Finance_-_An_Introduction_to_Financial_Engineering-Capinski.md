

<!-- === Source: MinerU_markdown_Mathematics_for_Finance_-_An_Introduction_to_Financial_Engineering-Capinski_1_2122706940055363596.md (Page 1) === -->

# Mathematics for Finance: An Introduction to Financial Engineering

Marek Capinski Tomasz Zastawniak 

Springer 

Springer London Berlin Heidelberg New York Hong Kong Milan Paris Tokyo 

## Advisory Board

P.J. Cameron Queen Mary and Westfield College 

M.A.J. Chaplain University ofDundee 

K. Erdmann Oxford University 

L.C.G. Rogers University of Cambridge 

E. Süli Oxford University 

J.F. Toland University ofBath 

## Other books in this series

A First Course in Discrete Mathematics I. Anderson 

Analytic Methods for Partial Differential Equations G. Evans, J. Blackledge, P. Yardley 

Applied Geometry for Computer Graphics and CAD D. Marsh 

Basic Linear Algebra, Second Edition T.S. Blyth and E.F. Robertson 

Basic Stochastic Processes Z. Brze´zniak and T. Zastawniak 

Elementary Differential Geometry A. Pressley 

Elementary Number Theory G.A. Jones and J.M. Jones 

Elements of Abstract Analysis M. Ó Searcóid 

Elements of Logic via Numbers and Sets D.L. Johnson 

Essential Mathematical Biology N.F. Britton 

Fields, Flows and Waves: An Introduction to Continuum Models D.F. Parker 

Further Linear Algebra T.S. Blyth and E.F. Robertson 

Geometry R. Fenn 

Groups, Rings and Fields D.A.R. Wallace 

Hyperbolic Geometry J.W. Anderson 

Information and Coding Theory G.A. Jones and J.M. Jones 

Introduction to Laplace Transforms and Fourier Series P.P.G. Dyke 

Introduction to Ring Theory P.M. Cohn 

Introductory Mathematics: Algebra and Analysis G. Smith 

Linear Functional Analysis B.P. Rynne and M.A. Youngson 

Matrix Groups: An Introduction to Lie Group Theory A. Baker 

Measure, Integral and Probability M. Capi´nski and E. Kopp 

Multivariate Calculus and Geometry S. Dineen 

Numerical Methods for Partial Differential Equations G. Evans, J. Blackledge, P. Yardley 

Probability Models J. Haigh 

Real Analysis J.M. Howie 

Sets, Logic and Categories P. Cameron 

Special Relativity N.M.J. Woodhouse 

Symmetries D.L. Johnson 

Topics in Group Theory G. Smith and O. Tabachnikova 

Topologies and Uniformities I.M. James 

Vector Calculus P.C. Matthews 

# Mathematics for Finance

An Introduction to Financial Engineering 

With 75 Figures 

Marek Capi´nski 

# Nowy Sacz School of Business–National Louis University, 33-300 Nowy Sacz, ul. Zielona 27, Poland

Tomasz Zastawniak 

# Department of Mathematics, University of Hull, Cottingham Road, Kingston upon Hull, HU6 7RX, UK

Cover illustration elements reproduced by kind permission of: 

Aptech Systems, Inc., Publishers of the GAUSS Mathematical and Statistical System, 23804 S.E. Kent-Kangley Road, Maple Valley, WA 98038, USA. Tel: (206) 432 - 7855 Fax (206) 432 - 7832 email: info@aptech.com URL: www.aptech.com. 

American Statistical Association: Chance Vol 8 No 1, 1995 article by KS and KW Heiner ‘Tree Rings of the Northern Shawangunks’ page 32 fig 2. 

Springer-Verlag: Mathematica in Education and Research Vol 4 Issue 3 1995 article by Roman E Maeder, Beatrice Amrhein and Oliver Gloor Illustrated Mathematics: Visualization of Mathematical Objects' page 9 fig 11, originally published as a CD ROMIllustrated Mathematics' by TELOS: ISBN 0-387-14222-3, German edition by Birkhauser: ISBN 3-7643-5100-4. 

Mathematica in Education and Research Vol 4 Issue 3 1995 article by Richard J Gaylord and Kazume Nishidate ‘Traffic Engineering wit Cellular Automata' page 35 fig 2. Mathematica in Education and Research Vol 5 Issue 2 1996 article by Michael Trott The Implicitization of a Trefoil Knot’ page 14. 

Mathematica in Education and Research Vol 5 Issue 2 1996 article by Lee de Cola Coins, Trees, Bars and Bells: Simulation of the Binomial Process’ page 19 fig 3. Mathematica in Education and Research Vol 5 Issue 2 1996 article by Richard Gaylord and Kazume Nishidate ‘Contagious Spreading’ page 33 fig 1. Mathematica in Education and Research Vol 5 Issue 2 1996 article by Joe Buhler and Stan Wagon ‘Secrets of theMadelung Constant’ page 50 fig 1. 

British Library Cataloguing in Publication Data 

Capi´nski, Marek, 1951- 

Mathematics for finance : an introduction to financial 

engineering. - (Springer undergraduate mathematics series) 

1. Business mathematics 2. Finance – Mathematical models 

I. Title II. Zastawniak, Tomasz, 1959- 

332’.0151 

ISBN 1852333308 

Library of Congress Cataloging-in-Publication Data 

Capi´nski, Marek, 1951- 

Mathematics for finance : an introduction to financial engineering / Marek Capi´nski and Tomasz Zastawniak 

p. cm. — (Springer undergraduate mathematics series) 

Includes bibliographical references and index. 

ISBN 1-85233-330-8 (alk. paper) 

1. Finance – Mathematical models. 2. Investments – Mathematics. 3. Business 

mathematics. I. Zastawniak, Tomasz, 1959- II. Title. III. Series. 

HG106.C36 2003 

332.6’01’51—dc21 

2003045431 

Apart from any fair dealing for the purposes of research or private study, or criticism or review, as permitted under the Copyright, Designs and Patents Act 1988, this publication may only be reproduced, stored or transmitted, in any form or by any means, with the prior permission in writing of the publishers, or in the case of reprographic reproduction in accordance with the terms of licences issued by the Copyright Licensing Agency. Enquiries concerning reproduction outside those terms should be sent to the publishers. 

Springer Undergraduate Mathematics Series ISSN 1615-2085 

ISBN 1-85233-330-8 Springer-Verlag London Berlin Heidelberg 

a member of BertelsmannSpringer Science+Business Media GmbH 

http://www.springer.co.uk 

© Springer-Verlag London Limited 2003 

Printed in the United States of America 

The use of registered names, trademarks etc. in this publication does not imply, even in the absence of a specific statement, that such names are exempt from the relevant laws and regulations and therefore free for general use 

The publisher makes no representation, express or implied, with regard to the accuracy of the information contained in this book and cannot accept any legal responsibility or liability for any errors or omissions that may be made. 

Typesetting: Camera ready by the authors 12/3830-543210 Printed on acid-free paper SPIN 10769004 

True to its title, this book itself is an excellent financial investment. For the price of one volume it teaches two Nobel Prize winning theories, with plenty more included for good measure. How many undergraduate mathematics textbooks can boast such a claim? 

Building on mathematical models of bond and stock prices, these two theo ries lead in diferent directions: Black–Scholes arbitrage pricing of options and other derivative securities on the one hand, and Markowitz portfolio optimisa tion and the Capital Asset Pricing Model on the other hand. Models based on the principle of no arbitrage can also be developed to study interest rates and their term structure. These are three major areas of mathematical finance, all having an enormous impact on the way modern financial markets operate. This textbook presents them at a level aimed at second or third year undergraduate students, not only of mathematics but also, for example, business management, finance or economics. 

The contents can be covered in a one-year course of about 100 class hours. Smaller courses on selected topics can readily be designed by choosing the appropriate chapters. The text is interspersed with a multitude of worked examples and exercises, complete with solutions, providing ample material for tutorials as well as making the book ideal for self-study. 

Prerequisites include elementary calculus, probability and some linear alge bra. In calculus we assume experience with derivatives and partial derivatives, finding maxima or minima of diferentiable functions of one or more variables, Lagrange multipliers, the Taylor formula and integrals. Topics in probability include random variables and probability distributions, in particular the bi nomial and normal distributions, expectation, variance and covariance, condi tional probability and independence. Familiarity with the Central Limit The orem would be a bonus. In linear algebra the reader should be able to solve systems of linear equations, add, multiply, transpose and invert matrices, and compute determinants. In particular, as a reference in probability theory we recommend our book: M. Capi´nski and T. Zastawniak, Probability Through Problems, Springer-Verlag, New York, 2001. 

In many numerical examples and exercises it may be helpful to use a computer with a spreadsheet application, though this is not absolutely essential. Microsoft Excel files with solutions to selected examples and exercises are avail able on our web page at the addresses below. 

We are indebted to Nigel Cutland for prompting us to steer clear of an inaccuracy frequently encountered in other texts, of which more will be said in Remark 4.1. It is also a great pleasure to thank our students and colleagues fo their feedback on preliminary versions of various chapters. 

Readers of this book are cordially invited to visit the web page below to check for the latest downloads and corrections, or to contact the authors. You comments will be greatly appreciated. 

Marek Capi´nski and Tomasz Zastawniak January 2003 

www springer co uk/M4F 

1. Introduction: A Simple Market Model 1  
1.1 Basic Notions and Assumptions 1  
1.2 No-Arbitrage Principle 5  
1.3 One-Step Binomial Model 7  
1.4 Risk and Return 9  
1.5 Forward Contracts 11  
1.6 Call and Put Options 13  
1.7 Managing Risk with Options 19  

2. Risk-Free Assets 21  
2.1 Time Value of Money 21  
2.1.1 Simple Interest 22  
2.1.2 Periodic Compounding 24  
2.1.3 Streams of Payments 29  
2.1.4 Continuous Compounding 32  
2.1.5 How to Compare Compounding Methods 35  
2.2 Money Market 39  
2.2.1 Zero-Coupon Bonds 39  
2.2.2 Coupon Bonds 41  
2.2.3 Money Market Account 43  

3. Risky Assets 47  
3.1 Dynamics of Stock Prices 47  
3.1.1 Return 49  
3.1.2 Expected Return 53  
3.2 Binomial Tree Model 55 

3.2.1 Risk-Neutral Probability 58
3.2.2 Martingale Property 61
3.3 Other Models 63
3.3.1 Trinomial Tree Model 64
3.3.2 Continuous-Time Limit 66
4. Discrete Time Market Models 73
4.1 Stock and Money Market Models 73
4.1.1 Investment Strategies 75
4.1.2 The Principle of No Arbitrage 79
4.1.3 Application to the Binomial Tree Model 81
4.1.4 Fundamental Theorem of Asset Pricing 83
4.2 Extended Models 85
5. Portfolio Management 91
5.1 Risk 91
5.2 Two Securities 94
5.2.1 Risk and Expected Return on a Portfolio 97
5.3 Several Securities 107
5.3.1 Risk and Expected Return on a Portfolio 107
5.3.2 Efficient Frontier 114
5.4 Capital Asset Pricing Model 118
5.4.1 Capital Market Line 118
5.4.2 Beta Factor 120
5.4.3 Security Market Line 122
6. Forward and Futures Contracts 125
6.1 Forward Contracts 125
6.1.1 Forward Price 126
6.1.2 Value of a Forward Contract 132
6.2 Futures 134
6.2.1 Pricing 136
6.2.2 Hedging with Futures 138
7. Options: General Properties 147
7.1 Definitions 147
7.2 Put-Call Parity 150
7.3 Bounds on Option Prices 154
7.3.1 European Options 155
7.3.2 European and American Calls on Non-Dividend Paying Stock 157
7.3.3 American Options 158 

7.4 Variables Determining Option Prices....159
7.4.1 European Options....160
7.4.2 American Options....165
7.5 Time Value of Options....169

8. Option Pricing....173
8.1 European Options in the Binomial Tree Model....174
8.1.1 One Step....174
8.1.2 Two Steps....176
8.1.3 General N-Step Model....178
8.1.4 Cox-Ross-Rubinstein Formula....180
8.2 American Options in the Binomial Tree Model....181
8.3 Black-Scholes Formula....185

9. Financial Engineering....191
9.1 Hedging Option Positions....192
9.1.1 Delta Hedging....192
9.1.2 Greek Parameters....197
9.1.3 Applications....199
9.2 Hedging Business Risk....201
9.2.1 Value at Risk....202
9.2.2 Case Study....203
9.3 Speculating with Derivatives....208
9.3.1 Tools....208
9.3.2 Case Study....209

10. Variable Interest Rates....215
10.1 Maturity-Independent Yields....216
10.1.1 Investment in Single Bonds....217
10.1.2 Duration....222
10.1.3 Portfolios of Bonds....224
10.1.4 Dynamic Hedging....226
10.2 General Term Structure....229
10.2.1 Forward Rates....231
10.2.2 Money Market Account....235

11. Stochastic Interest Rates....237
11.1 Binomial Tree Model....238
11.2 Arbitrage Pricing of Bonds....245
11.2.1 Risk-Neutral Probabilities....249
11.3 Interest Rate Derivative Securities....253
11.3.1 Options....254 

11.3.2 Swaps 255  
11.3.3 Caps and Floors 258  
11.4 Final Remarks 259  
Solutions 263  
Bibliography 303  
Glossary of Symbols 305  
Index 307 

## 1.1 Basic Notions and Assumptions

Suppose that two assets are traded: one risk-free and one risky security. The former can be thought of as a bank deposit or a bond issued by a government, a financial institution, or a company. The risky security will typically be some stock. It may also be a foreign currency, gold, a commodity or virtually any asset whose future price is unknown today. 

Throughout the introduction we restrict the time scale to two instants only: today, t = 0, and some future time, say one year from now, t = 1. More refined and realistic situations will be studied in later chapters. 

The position in risky securities can be specified as the number of shares of stock held by an investor. The price of one share at time t will be denoted by S(t). The current stock price S(0) is known to all investors, but the future price S(1) remains uncertain: it may go up as well as down. The diference $S ( 1 ) - S ( 0 )$ as a fraction of the initial value represents the so-called rate of return, or briefly return: 

$$
K _ {S} = \frac {S (1) - S (0)}{S (0)},
$$

which is also uncertain. The dynamics of stock prices will be discussed in Chapter 3. 

The risk-free position can be described as the amount held in a bank ac count. As an alternative to keeping money in a bank, investors may choose to invest in bonds. The price of one bond at time t will be denoted by A(t). The current bond price A(0) is known to all investors, just like the current stock price. However, in contrast to stock, the price A(1) the bond will fetch at time 1 is also known with certainty. For example, A(1) may be a payment guaranteed by the institution issuing bonds, in which case the bond is said to mature at time 1 with face value $A ( 1 )$ . The return on bonds is defined in a similar way as that on stock, 

$$
K _ {A} = \frac {A (1) - A (0)}{A (0)}.
$$

Chapters 2, 10 and 11 give a detailed exposition of risk-free assets. 

Our task is to build a mathematical model of a market of financial securities. A crucial first stage is concerned with the properties of the mathematical objects involved. This is done below by specifying a number of assumptions, the purpose of which is to find a compromise between the complexity of the real world and the limitations and simplifications of a mathematical model, imposed in order to make it tractable. The assumptions reflect our current position on this compromise and will be modified in the future. 

## Assumption 1.1 (Randomness)

The future stock price S(1) is a random variable with at least two diferen values. The future price A(1) of the risk-free security is a known number. 

## Assumption 1.2 (Positivity of Prices)

All stock and bond prices are strictly positive, 

$$
A (t) > 0 \quad \text { and } \quad S (t) > 0 \quad \text { for } t = 0, 1.
$$

The total wealth of an investor holding x stock shares and y bonds at a time instant $t = 0$ , 1 is 

$$
V (t) = x S (t) + y A (t).
$$

The pair $( x , y )$ is called a portfolio, V(t) being the value of this portfolio or, in other words, the wealth of the investor at time t. 

The jumps of asset prices between times 0 and 1 give rise to a change of the portfolio value: 

$$
V (1) - V (0) = x (S (1) - S (0)) + y (A (1) - A (0)).
$$

This diference (which may be positive, zero, or negative) as a fraction of the initial value represents the return on the portfolio, 

$$
K _ {V} = \frac {V (1) - V (0)}{V (0)}.
$$

The returns on bonds or stock are particular cases of the return on a portfolio (with $x \ = \ 0$ or $y = 0$ , respectively). Note that because $S ( 1 )$ is a random variable, so is $V ( 1 )$ as well as the corresponding returns $K _ { S }$ and $K _ { V }$ . The return $K _ { A }$ on a risk-free investment is deterministic. 

## Example 1.1

Let $A ( 0 ) = 1 0 0$ and $A ( 1 ) = 1 1 0$ dollars. Then the return on an investment in bonds will be 

$$
K _ {A} = 0. 1 0,
$$

that is, 10%. Also, let $S ( 0 ) = 5 0 $ dollars and suppose that the random variable $S ( 1 )$ can take two values, 

$$
S (1) = \left\{ \begin{array}{l l} 5 2 & \text {with probability p}, \\ 4 8 & \text {with probability 1 - p}, \end{array} \right.
$$

for a certain $0 < p < 1$ . The return on stock will then be 

$$
K _ {S} = \left\{ \begin{array}{r l} 0. 0 4 & \text {if stock goes up,} \\ - 0. 0 4 & \text {if stock goes down,} \end{array} \right.
$$

that is, 4% or $- 4 \%$ 

## Example 1.2

Given the bond and stock prices in Example 1.1, the value at time 0 of a portfolio with $x = 2 0$ stock shares and $y = 1 0$ bonds is 

$$
V (0) = 2, 0 0 0
$$

dollars. The time 1 value of this portfolio will be 

$$
V (1) = \left\{ \begin{array}{l l} 2, 1 4 0 & \text {if stock goes up}, \\ 2, 0 6 0 & \text {if stock goes down}, \end{array} \right.
$$

so the return on the portfolio will be 

$$
K _ {V} = \left\{ \begin{array}{l l} 0. 0 7 & \text {if stock goes up,} \\ 0. 0 3 & \text {if stock goes down,} \end{array} \right.
$$

that is, $7 \%$ or 3%. 

## Exercise 1.1

Let $A ( 0 ) = 9 0 , A ( 1 ) = 1 0 0 , S ( 0 ) = 2 5 ~ \mathrm { d o l l a r s ~ a n d ~ l e t }$ 

$$
S (1) = \left\{ \begin{array}{l l} 3 0 & \text {with probability} p, \\ 2 0 & \text {with probability} 1 - p, \end{array} \right.
$$

where $0 < p < 1$ . For a portfolio with $x = 1 0$ shares and $y = 1 5$ bonds calculate V(0), V(1) and $K _ { V }$ 

## Exercise 1.2

Given the same bond and stock prices as in Exercise 1.1, find a portfolio whose value at time 1 is 

$$
V (1) = \left\{ \begin{array}{l l} 1, 1 6 0 & \text {if stock goes up}, \\ 1, 0 4 0 & \text {if stock goes down}. \end{array} \right.
$$

What is the value of this portfolio at time 0? 

It is mathematically convenient and not too far from reality to allow arbitrary real numbers, including negative ones and fractions, to represent the risky and risk-free positions x and y in a portfolio. This is reflected in the following assumption, which imposes no restrictions as far as the trading positions are concerned. 

## Assumption 1.3 (Divisibility, Liquidity and Short Selling)

An investor may hold any number x and y of stock shares and bonds, whether integer or fractional, negative, positive or zero. In general, 

$$
x, y \in \mathbb {R}.
$$

The fact that one can hold a fraction of a share or bond is referred to as divisibility. Almost perfect divisibility is achieved in real world dealings whenever the volume of transactions is large as compared to the unit prices. 

The fact that no bounds are imposed on x or y is related to another marke attribute known as liquidity. It means that any asset can be bought or sold on demand at the market price in arbitrary quantities. This is clearly a mathematical idealisation because in practice there exist restrictions on the volume of trading. 

If the number of securities of a particular kind held in a portfolio is positive, we say that the investor has a long position. Otherwise, we say that a short position is taken or that the asset is shorted. A short position in risk-free securities may involve issuing and selling bonds, but in practice the same fi nancial efect is more easily achieved by borrowing cash, the interest rate being determined by the bond prices. Repaying the loan with interest is referred to as closing the short position. A short position in stock can be realised by short selling. This means that the investor borrows the stock, sells it, and uses the proceeds to make some other investment. The owner of the stock keeps all the rights to it. In particular, she is entitled to receive any dividends due and may wish to sell the stock at any time. Because of this, the investor must always have suficient resources to fulfil the resulting obligations and, in particular, to close the short position in risky assets, that is, to repurchase the stock and return it to the owner. Similarly, the investor must always be able to close a short position in risk-free securities, by repaying the cash loan with interest. In view of this, we impose the following restriction. 

## Assumption 1.4 (Solvency)

The wealth of an investor must be non-negative at all times, 

$$
V (t) \geq 0 \quad \text { for } t = 0, 1.
$$

A portfolio satisfying this condition is called admissible. 

In the real world the number of possible diferent prices is finite because they are quoted to within a specified number of decimal places and because there is only a certain final amount of money in the whole world, supplying an upper bound for all prices. 

## Assumption 1.5 (Discrete Unit Prices)

The future price S(1) of a share of stock is a random variable taking only finitely many values. 

## 1.2 No-Arbitrage Principle

In this section we are going to state the most fundamental assumption about the market. In brief, we shall assume that the market does not allow for risk-free profits with no initial investment. 

For example, a possibility of risk-free profits with no initial investment can emerge when market participants make a mistake. Suppose that dealer A in New York ofers to buy British pounds at a rate $d _ { A } = 1 . 6 2$ dollars to a pound, while dealer B in London sells them at a rate $d _ { B } = 1 . 6 0$ dollars to a pound. If this were the case, the dealers would, in efect, be handing out free money. An investor with no initial capital could realise a profit of $d _ { A } - d _ { B } = 0 . 0 2$ dollars per each pound traded by taking simultaneously a short position with dealer B and a long position with dealer A. The demand for their generous services would quickly compel the dealers to adjust the exchange rates so that this profitable opportunity would disappear. 

## Exercise 1.3

On 19 July 2002 dealer A in New York and dealer B in London used the following rates to change currency, namely euros (EUR), British pounds (GBP) and US dollars (USD): 

<table><tr><td>dealer A</td><td>buy</td><td>sell</td></tr><tr><td>1.0000 EUR</td><td>1.0202 USD</td><td>1.0284 USD</td></tr><tr><td>1.0000 GBP</td><td>1.5718 USD</td><td>1.5844 USD</td></tr></table>

<table><tr><td>dealer B</td><td>buy</td><td>sell</td></tr><tr><td>1.0000 EUR</td><td>0.6324 GBP</td><td>0.6401 GBP</td></tr><tr><td>1.0000 USD</td><td>0.6299 GBP</td><td>0.6375 GBP</td></tr></table>


Spot a chance of a risk-free profit without initial investment.


The next example illustrates a situation when a risk-free profit could be realised without initial investment in our simplified framework of a single time step. 

## Example 1.3

Suppose that dealer A in New York ofers to buy British pounds a year from now at a rate $d _ { A } = 1 . 5 8$ dollars to a pound, while dealer B in London would sell British pounds immediately at a rate $d _ { B } = 1 . 6 0$ dollars to a pound. Suppose further that dollars can be borrowed at an annual rate of 4%, and British pounds can be invested in a bank account at 6%. This would also create an opportunity for a risk-free profit without initial investment, though perhaps not as obvious as before. 

For instance, an investor could borrow 10, 000 dollars and convert them into 6, 250 pounds, which could then be deposited in a bank account. After one yea interest of 375 pounds would be added to the deposit, and the whole amoun could be converted back into 10, 467.50 dollars. (A suitable agreement would have to be signed with dealer A at the beginning of the year.) After paying back the dollar loan with interest of 400 dollars, the investor would be left with a profit of 67.50 dollars. 

Apparently, one or both dealers have made a mistake in quoting their ex change rates, which can be exploited by investors. Once again, increased de mand for their services will prompt the dealers to adjust the rates, reducing $d _ { A }$ and/or increasing $d _ { B }$ to a point when the profit opportunity disappears. 

We shall make an assumption forbidding situations similar to the above example. 

## Assumption 1.6 (No-Arbitrage Principle)

There is no admissible portfolio with initial value $V ( 0 ) = 0$ such that $V ( 1 ) > 0$ with non-zero probability. 

In other words, if the initial value of an admissible portfolio is zero, $V ( 0 ) =$ 0, then $V ( 1 ) = 0$ with probability 1. This means that no investor can lock in a profit without risk and with no initial endowment. If a portfolio violating this principle did exist, we would say that an arbitrage opportunity was available. 

Arbitrage opportunities rarely exist in practice. If and when they do, the gains are typically extremely small as compared to the volume of transactions, making them beyond the reach of small investors. In addition, they can be more subtle than the examples above. Situations when the No-Arbitrage Principle is violated are typically short-lived and dificult to spot. The activities of investors (called arbitrageurs) pursuing arbitrage profits efectively make the market free of arbitrage opportunities. 

The exclusion of arbitrage in the mathematical model is close enough to reality and turns out to be the most important and fruitful assumption. Arguments based on the No-arbitrage Principle are the main tools of financial mathematics. 

## 1.3 One-Step Binomial Model

In this section we restrict ourselves to a very simple example, in which the stock price $S ( 1 )$ takes only two values. Despite its simplicity, this situation is suficiently interesting to convey the flavour of the theory to be developed later on. 

## Example 1.4

Suppose that $S ( 0 ) = 1 0 0$ dollars and S(1) can take two values, 

$$
S (1) = \left\{ \begin{array}{l l} 1 2 5 & \text { with   probability } p, \\ 1 0 5 & \text { with   probability } 1 - p, \end{array} \right.
$$

where $0 < p < 1$ , while the bond prices are $A ( 0 ) = 1 0 0$ and $A ( 1 ) = 1 1 0$ dollars. Thus, the return $K _ { S }$ on stock will be 25% if stock goes up, or 5% if stock goes down. (Observe that both stock prices at time 1 happen to be higher than that at time 0; ‘going $\mathrm { u p } ^ { \mathrm { \prime } }$ or ‘down’ is relative to the other price at time 1.) The 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/d58b707e035b8e10f3f1ad7ed11b51495429b52c499e592a3ed492c65f443473.jpg)



Figure 1.1 One-step binomial tree of stock prices


risk-free return will be $K _ { A } = 1 0 \%$ . The stock prices are represented as a tree in Figure 1.1. 

In general, the choice of stock and bond prices in a binomial model is con strained by the No-Arbitrage Principle. Suppose that the possible up and down stock prices at time 1 are 

$$
S (1) = \left\{ \begin{array}{l l} S ^ {\mathrm{u}} & \text { with   probability } p, \\ S ^ {\mathrm{d}} & \text { with   probability } 1 - p, \end{array} \right.
$$

where $S ^ { \mathrm { d } } < S ^ { \mathrm { u } }$ and $0 < p < 1$ 

## Proposition 1.1

If $S ( 0 ) = A ( 0 )$ , then 

$$
S ^ {\mathrm{d}} <   A (1) <   S ^ {\mathrm{u}},
$$

or else an arbitrage opportunity would arise. 

## Proof

We shall assume for simplicity that $S ( 0 ) = A ( 0 ) = 1 0 0$ dollars. Suppose that $A ( 1 ) \leq S ^ { \mathrm { d } }$ . In this case, at time 0: 

Borrow $100 risk-free. 

Buy one share of stock for $100. 

This way, you will be holding a portfolio $( x , y )$ with $x = 1$ shares of stock and $y = - 1$ bonds. The time 0 value of this portfolio is 

$$
V (0) = 0.
$$

At time 1 the value will become 

$$
V (1) = \left\{ \begin{array}{l l} S ^ {\mathrm{u}} - A (1) & \text { if   stock   goes   up }, \\ S ^ {\mathrm{d}} - A (1) & \text { if   stock   goes   down }. \end{array} \right.
$$

If $A ( 1 ) \leq S ^ { \mathrm { d } }$ , then the first of these two possible values is strictly positive, while the other one is non-negative, that is, $V ( 1 )$ is a non-negative random variable such that $V ( 1 ) > 0$ with probability $p > 0$ . The portfolio provides an arbitrage opportunity, violating the No-Arbitrage Principle. 

Now suppose that $A ( 1 ) \geq S ^ { \mathrm { u } }$ . If this is the case, then at time 0: 

Sell short one share for $100. 

Invest $100 risk-free. 

As a result, you will be holding a portfolio $( x , y )$ with $x = - 1$ and $y = 1$ , again of zero initial value, 

$$
V (0) = 0.
$$

The final value of this portfolio will be 

$$
V (1) = \left\{ \begin{array}{l l} - S ^ {\mathrm{u}} + A (1) & \text {if stock goes up,} \\ - S ^ {\mathrm{d}} + A (1) & \text {if stock goes down,} \end{array} \right.
$$

which is non-negative, with the second value being strictly positive, since $A ( 1 ) \geq S ^ { \mathrm { u } }$ . Thus, $V ( 1 )$ is a non-negative random variable such that $V ( 1 ) > 0$ with probability $1 - p > 0$ . Once again, this indicates an arbitrage opportunity, violating the No-Arbitrage Principle. □ 

The common sense reasoning behind the above argument is straightforward: Buy cheap assets and sell (or sell short) expensive ones, pocketing the diference. 

## 1.4 Risk and Return

Let $A ( 0 ) = 1 0 0$ and $A ( 1 ) = 1 1 0$ dollars, as before, but $S ( 0 ) = 8 0 $ dollars and 

$$
S (1) = \left\{ \begin{array}{c l} 1 0 0 & \mathrm{withprobability0.8,} \\ 6 0 & \mathrm{withprobability0.2.} \end{array} \right.
$$

Suppose that you have $10, 000 to invest in a portfolio. You decide to buy $x = 5 0$ shares, which fixes the risk-free investment at $y = 6 0$ . Then 

$$
V (1) = \left\{ \begin{array}{c l} 1 1, 6 0 0 & \text {if stock goes up}, \\ 9, 6 0 0 & \text {if stock goes down}, \end{array} \right.
$$

$$
K _ {V} = \left\{ \begin{array}{r l} 0. 1 6 & \text { if   stock   goes   up }, \\ - 0. 0 4 & \text { if   stock   goes   down }. \end{array} \right.
$$

The expected return, that is, the mathematical expectation of the return on the portfolio is 

$$
E (K _ {V}) = 0. 1 6 \times 0. 8 - 0. 0 4 \times 0. 2 = 0. 1 2,
$$

that is, 12%. The risk of this investment is defined to be the standard deviation of the random variable $K _ { V }$ 

$$
\sigma_ {V} = \sqrt {(0 . 1 6 - 0 . 1 2) ^ {2} \times 0 . 8 + (- 0 . 0 4 - 0 . 1 2) ^ {2} \times 0 . 2} = 0. 0 8,
$$

that is 8%. Let us compare this with investments in just one type of security. If $x = 0$ , then $y = 1 0 0$ , that is, the whole amount is invested risk-free. In this case the return is known with certainty to be $K _ { A } = 0 . 1$ , that is, 10% and the risk as measured by the standard deviation is zero, $\sigma _ { A } = 0$ 

On the other hand, if $x = 1 2 5$ and $y = 0$ , the entire amount being invested in stock, then 

$$
V (1) = \left\{ \begin{array}{c l} 1 2, 5 0 0 & \text { if   stock   goes   up }, \\ 7, 5 0 0 & \text { if   stock   goes   down }, \end{array} \right.
$$

and $E ( K _ { S } ) = 0 . 1 5$ with $\sigma _ { S } = 0 . 2 0$ , that is, 15% and 20%, respectively. 

Given the choice between two portfolios with the same expected return, any investor would obviously prefer that involving lower risk. Similarly, if the risk levels were the same, any investor would opt for higher return. However, in the case in hand higher return is associated with higher risk. In such circumstances the choice depends on individual preferences. These issues will be discussed in Chapter 5, where we shall also consider portfolios consisting of several risky securities. The emerging picture will show the power of portfolio selection and portfolio diversification as tools for reducing risk while maintaining the expected return. 

## Exercise 1.4

For the above stock and bond prices, design a portfolio with initial wealth of $10, 000 split fifty-fifty between stock and bonds. Compute the ex pected return and risk as measured by standard deviation. 

## 1.5 Forward Contracts

A forward contract is an agreement to buy or sell a risky asset at a specified future time, known as the delivery date, for a price F fixed at the presen moment, called the forward price. An investor who agrees to buy the asset is said to enter into a long forward contract or to take a long forward position. If an investor agrees to sell the asset, we speak of a short forward contract or a short forward position. No money is paid at the time when a forward contract is exchanged. 

## Example 1.5

Suppose that the forward price is $80. If the market price of the asset turns out to be $84 on the delivery date, then the holder of a long forward contract will buy the asset for $80 and can sell it immediately for $84, cashing the diference of $4. On the other hand, the party holding a short forward position will have to sell the asset for $80, sufering a loss of $4. However, if the market price of the asset turns out to be $75 on the delivery date, then the party holding a long forward position will have to buy the asset for $80, sufering a loss of $5. Meanwhile, the party holding a short position will gain $5 by selling the asset above its market price. In either case the loss of one party is the gain of the other. 

In general, the party holding a long forward contract with delivery date 1 will benefit if the future asset price S(1) rises above the forward price F. If the asset price $S ( 1 )$ falls below the forward price F, then the holder of a long forward contract will sufer a loss. In general, the payof for a long forward position is $S ( 1 ) - F$ (which can be positive, negative or zero). For a short forward position the payof is $F - S ( 1 )$ 

Apart from stock and bonds, a portfolio held by an investor may contain forward contracts, in which case it will be described by a triple $( x , y , z )$ . Here x and y are the numbers of stock shares and bonds, as before, and z is the number of forward contracts (positive for a long forward position and negative for a short position). Because no payment is due when a forward contract is exchanged, the initial value of such a portfolio is simply 

$$
V (0) = x S (0) + y A (0).
$$

At the delivery date the value of the portfolio will become 

$$
V (1) = x S (1) + y A (1) + z (S (1) - F).
$$

Assumptions 1.1 to 1.5 as well as the No-Arbitrage Principle extend readily to this case. 

The forward price F is determined by the No-Arbitrage Principle. In particular, it can easily be found for an asset with no carrying costs. A typical example of such an asset is a stock paying no dividend. (By contrast, a commodity will usually involve storage costs, while a foreign currency will earn interest, which can be regarded as a negative carrying cost.) 

A forward position guarantees that the asset will be bought for the forward price F at delivery. Alternatively, the asset can be bought now and held until delivery. However, if the initial cash outlay is to be zero, the purchase must be financed by a loan. The loan with interest, which will need to be repaid at the delivery date, is a candidate for the forward price. The following proposition shows that this is indeed the case. 

## Proposition 1.2

Suppose that $A ( 0 ) = 1 0 0 , A ( 1 ) = 1 1 0$ , and $S ( 0 ) = 5 0 $ dollars, where the risky security involves no carrying costs. Then the forward price must be $F = 5 5$ dollars, or an arbitrage opportunity would exist otherwise. 

## Proof

Suppose that $F > 5 5$ . Then, at time 0: 

Borrow $50. 

Buy the asset for $S ( 0 ) = 5 0 ~ \mathrm { d o l l a r s } .$ 

Enter into a short forward contract with forward price F dollars and delivery date 1. 

The resulting portfolio $( 1 , - \frac { 1 } { 2 } , - 1 )$ consisting of stock, a risk-free position, and a short forward contract has initial value $V ( 0 ) = 0$ . Then, at time 1: 

Close the short forward position by selling the asset for F dollars. 

Close the risk-free position by paying $\textstyle { \frac { 1 } { 2 } } \times 1 1 0 = 5 5$ dollars. 

The final value of the portfolio, $V ( 1 ) = F - 5 5 > 0$ , will be your arbitrage profit, violating the No-Arbitrage Principle. 

On the other hand, if $F < 5 5$ , then at time 0: 

Sell short the asset for $50. 

Invest this amount risk-free. 

Take a long forward position in stock with forward price F dollars and delivery date 1. 

The initial value of this portfolio $( - 1 , { \frac { 1 } { 2 } } , 1 )$ is also $V ( 0 ) = 0$ . Subsequently, at time 1: 

Cash $55 from the risk-free investment. 

Buy the asset for F dollars, closing the long forward position, and return the asset to the owner. 

Your arbitrage profit will be $V ( 1 ) = 5 5 - F > 0$ , which once again violates the No-Arbitrage Principle. It follows that the forward price must be $F = 5 5$ dollars. □ 

## Exercise 1.5

Let $A ( 0 ) = 1 0 0 , A ( 1 ) = 1 1 2$ and $S ( 0 ) = 3 4 $ dollars. Is it possible to find an arbitrage opportunity if the forward price of stock is $F = 3 8 . 6 0$ dollars with delivery date 1? 

## Exercise 1.6

Suppose that $A ( 0 ) = 1 0 0$ and $A ( 1 ) = 1 0 5$ dollars, the present price of pound sterling is S(0) = 1.6 dollars, and the forward price is $F = 1 . 5 0$ dollars to a pound with delivery date 1. How much should a sterling bond cost today if it promises to pay £100 at time 1? Hint: The forward contract is based on an asset involving negative carrying costs (the interest earned by investing in sterling bonds). 

## 1.6 Call and Put Options

$$
\text {   Let   } A (0) = 1 0 0, A (1) = 1 1 0, S (0) = 1 0 0 \text {   dollars   and   }
$$

$$
S (1) = \left\{ \begin{array}{c l} 1 2 0 & \text { with   probability } p, \\ 8 0 & \text { with   probability } 1 - p, \end{array} \right.
$$

where $0 < p < 1$ 

A call option with strike price or exercise price $100 and exercise time 1 is a contract giving the holder the right (but no obligation) to purchase a share of stock for $100 at time 1. 

If the stock price falls below the strike price, the option will be worthless. There would be little point in buying a share for $100 if its market price is $80, and no-one would want to exercise the right. Otherwise, if the share price rises to $120, which is above the strike price, the option will bring a profit of $20 to the holder, who is entitled to buy a share for $100 at time 1 and may sell it immediately at the market price of $120. This is known as exercising the option. The option may just as well be exercised simply by collecting the diference of $20 between the market price of stock and the strike price. In practice, the latter is often the preferred method because no stock needs to change hands. 

As a result, the payof of the call option, that is, its value at time 1 is a random variable 

$$
C (1) = \left\{ \begin{array}{c l} 2 0 & \text {if stock goes up,} \\ 0 & \text {if stock goes down.} \end{array} \right.
$$

Meanwhile, $C ( 0 )$ will denote the value of the option at time 0, that is, the price for which the option can be bought or sold today. 

## Remark 1.1

At first sight a call option may resemble a long forward position. Both involve buying an asset at a future date for a price fixed in advance. An essential diference is that the holder of a long forward contract is committed to buying the asset for the fixed price, whereas the owner of a call option has the righ but no obligation to do so. Another diference is that an investor will need to pay to purchase a call option, whereas no payment is due when exchanging a forward contract. 

In a market in which options are available, it is possible to invest in a portfolio $( x , y , z )$ consisting of x shares of stock, y bonds and z options. The time 0 value of such a portfolio is 

$$
V (0) = x S (0) + y A (0) + z C (0).
$$

At time 1 it will be worth 

$$
V (1) = x S (1) + y A (1) + z C (1).
$$

Just like in the case of portfolios containing forward contracts, Assumptions 1.1 to 1.5 and the No-Arbitrage Principle can be extended to portfolios consisting of stock, bonds and options. 

Our task will be to find the time 0 price $C ( 0 )$ of the call option consistent with the assumptions about the market and, in particular, with the absence of arbitrage opportunities. Because the holder of a call option has a certain right, but never an obligation, it is reasonable to expect that $C ( 0 )$ will be positive: one needs to pay a premium to acquire this right. We shall see that the option price $C ( 0 )$ can be found in two steps: 

## Step 1

Construct an investment in x stocks and y bonds such that the value of the investment at time 1 is the same as that of the option, 

$$
x S (1) + y A (1) = C (1),
$$

no matter whether the stock price $S ( 1 )$ goes up to $120 or down to $80. This is known as replicating the option. 

## Step 2

Compute the time 0 value of the investment in stock and bonds. It will be shown that it must be equal to the option price, 

$$
x S (0) + y A (0) = C (0),
$$

because an arbitrage opportunity would exist otherwise. This step will be referred to as pricing or valuing the option. 

## Step 1 (Replicating the Option)

The time 1 value of the investment in stock and bonds will be 

$$
x S (1) + y A (1) = \left\{ \begin{array}{c l} x 1 2 0 + y 1 1 0 & \text {if stock goes up,} \\ x 8 0 + y 1 1 0 & \text {if stock goes down.} \end{array} \right.
$$

Thus, the equality $x S ( 1 ) + y A ( 1 ) = C ( 1 )$ between two random variables can be written as 

$$
\left\{ \begin{array}{r l} x 1 2 0 + y 1 1 0 & = 2 0, \\ x 8 0 + y 1 1 0 & = 0. \end{array} \right.
$$

The first of these equations covers the case when the stock price goes up to $120, whereas the second equation corresponds to the case when it drops to $80. Because we want the value of the investment in stock and bonds at time 1 to match exactly that of the option no matter whether the stock price goes up or down, these two equations are to be satisfied simultaneously. Solving for x and y, we find that 1 

$$
x = \frac {1}{2}, y = - \frac {4}{1 1}.
$$

To replicate the option we need to buy $\textstyle { \frac { 1 } { 2 } }$ a share of stock and take a short position of $- { \frac { 4 } { 1 1 } }$ in bonds (or borrow $\begin{array} { r } { \frac { 4 } { 1 1 } \times \mathbf { \bar { 1 } } 0 0 = \frac { 4 0 0 } { 1 1 } } \end{array}$ dollars in cash). 

## Step 2 (Pricing the Option)

We can compute the value of the investment in stock and bonds at time 0: 

$$
x S (0) + y A (0) = \frac {1}{2} \times 1 0 0 - \frac {4}{1 1} \times 1 0 0 \cong 1 3. 6 3 6 4
$$

dollars. The following proposition shows that this must be equal to the price of the option. 

## Proposition 1.3

If the option can be replicated by investing in the above portfolio of stock and bonds, then $\begin{array} { r } { C ( 0 ) = \frac { 1 } { 2 } S ( 0 ) - \frac { 4 } { 1 1 } A ( 0 ) } \end{array}$ , or else an arbitrage opportunity would exist. 

## Proof

Suppose that $\begin{array} { r } { C ( 0 ) + \frac { 4 } { 1 1 } A ( 0 ) > \frac { 1 } { 2 } S ( 0 ) } \end{array}$ . If this is the case, then at time 0: 

Issue and sell 1 option for $C ( 0 )$ dollars. 

Borrow $\textstyle { \frac { 4 } { 1 1 } } \times 1 0 0 = { \frac { 4 0 0 } { 1 1 } }$ dollars in cash (or take a short position $\begin{array} { r } { y = - \frac { 4 } { 1 1 } } \end{array}$ in bonds by selling them). 

Purchase $\begin{array} { r } { x = \frac { 1 } { 2 } } \end{array}$ shares of stock for $\begin{array} { r } { x S ( 0 ) = \frac { 1 } { 2 } \times 1 0 0 = 5 0 } \end{array}$ dollars. 

The cash balance of these transactions is positive, $\begin{array} { r } { C ( 0 ) + \frac { 4 } { 1 1 } A ( 0 ) - \frac { 1 } { 2 } S ( 0 ) > 0 } \end{array}$ Invest this amount risk-free. The resulting portfolio consisting of shares, risk free investments and a call option has initial value $V ( 0 ) = 0$ . Subsequently, at time 1: 

If stock goes up, then settle the option by paying the diference of $20 between the market price of one share and the strike price. You will pay nothing if stock goes down. The cost to you will be $C ( 1 )$ , which covers both possibilities. 

Repay the loan with interest (or close your short position $\begin{array} { r } { y = - \frac { 4 } { 1 1 } } \end{array}$ in bonds). This will cost you $\textstyle { \frac { 4 } { 1 1 } } \times 1 1 0 = 4 0$ dollars. 

Sell the stock for ${ \scriptstyle { \frac { 1 } { 2 } } } S ( 1 )$ obtaining either $\frac { 1 } { 2 } \times 1 2 0 = 6 0$ dollars if the price goes up, or $\begin{array} { r } { { \frac { 1 } { 2 } } \times 8 0 = 4 0 } \end{array}$ dollars if it goes down. 

The cash balance of these transactions will be zero, $\begin{array} { r } { - C ( 1 ) + \frac { 1 } { 2 } S ( 1 ) - \frac { 4 } { 1 1 } A ( 1 ) = 0 , } \end{array}$ regardless of whether stock goes up or down. But you will be left with the initial risk-free investment of $\begin{array} { r } { C ( 0 ) + \frac { 4 } { 1 1 } A ( 0 ) - \frac { 1 } { 2 } S ( 0 ) } \end{array}$ plus interest, thus realising an arbitrage opportunity. 

On the other hand, if $\begin{array} { r } { C ( 0 ) + \frac { 4 } { 1 1 } A ( 0 ) < \frac { 1 } { 2 } S ( 0 ) } \end{array}$ , then, at time 0: 

Buy 1 option for $C ( 0 )$ dollars. 

Buy $\textstyle { \frac { 4 } { 1 1 } }$ bonds for $\textstyle { \frac { 4 } { 1 1 } } \times 1 0 0 = { \frac { 4 0 0 } { 1 1 } }$ dollars. 

Sell short $\begin{array} { r } { x = \frac { 1 } { 2 } } \end{array}$ shares of stock for $\textstyle { \frac { 1 } { 2 } } \times 1 0 0 = 5 0$ dollars. 

The cash balance of these transactions is positive, $\begin{array} { r } { - C ( 0 ) - \frac { 4 } { 1 1 } A ( 0 ) + \frac { 1 } { 2 } S ( 0 ) > 0 , } \end{array}$ and can be invested risk-free. In this way you will have constructed a portfolio with initial value $V ( 0 ) = 0$ . Subsequently, at time 1: 

If stock goes up, then exercise the option, receiving the diference of $20 between the market price of one share and the strike price. You will receive nothing if stock goes down. Your income will be $C ( 1 )$ , which covers both possibilities. 

Sell the bonds for $\textstyle { \frac { 4 } { 1 1 } } A ( 1 ) = { \frac { 4 } { 1 1 } } \times 1 1 0 = 4 0$ dollars. 

Close the short position in stock, $\mathrm { p a y i n g } \ { \textstyle { \frac { 1 } { 2 } } } S ( 1 )$ , that is, $\textstyle { \frac { 1 } { 2 } } \times 1 2 0 = 6 0$ dollars if the price goes up, or $\textstyle { \frac { 1 } { 2 } } \times 8 0 = 4 0$ dollars if it goes down. 

The cash balance of these transactions will be zero, $\begin{array} { r } { C ( 1 ) + \frac { 4 } { 1 1 } A ( 1 ) - \frac { 1 } { 2 } S ( 1 ) = 0 } \end{array}$ regardless of whether stock goes up or down. But you will be left with an arbitrage profit resulting from the risk-free investment of $\begin{array} { r } { - C ( 0 ) - \frac { 4 } { 1 1 } A ( 0 ) + } \end{array}$ ${ \scriptstyle { \frac { 1 } { 2 } } } S ( 0 )$ plus interest, again a contradiction with the No-Arbitrage Principle. 

Here we see once more that the arbitrage strategy follows a common sense pattern: Sell (or sell short if necessary) expensive securities and buy cheap ones, as long as all your financial obligations arising in the process can be discharged, regardless of what happens in the future. 

Proposition 1.3 implies that today’s price of the option must be 

$$
C (0) = \frac {1}{2} S (0) - \frac {4}{1 1} A (0) \cong 1 3. 6 3 6 4
$$

dollars. Anyone who would sell the option for less or buy it for more than this price would be creating an arbitrage opportunity, which amounts to handing out free money. This completes the second step of our solution. 

## Remark 1.2

Note that the probabilities p and 1 p of stock going up or down are irrelevant in pricing and replicating the option. This is a remarkable feature of the theory and by no means a coincidence. 

## Remark 1.3

Options may appear to be superfluous in a market in which they can be repli cated by stock and bonds. In the simplified one-step model this is in fact a valid objection. However, in a situation involving multiple time steps (or continuous time) replication becomes a much more onerous task. It requires adjustments to the positions in stock and bonds at every time instant at which there is a change in prices, resulting in considerable management and transaction costs. In some cases it may not even be possible to replicate an option precisely. This is why the majority of investors prefer to buy or sell options, replication being normally undertaken only by specialised dealers and institutions. 

## Exercise 1.7

Let the bond and stock prices $A ( 0 ) , A ( 1 ) , S ( 0 ) , S ( 1 )$ be as above. Com pute the price $C ( 0 )$ of a call option with exercise time 1 and a) strike price $90, b) strike price $110. 

## Exercise 1.8

Let the prices $A ( 0 ) , S ( 0 ) , S ( 1 )$ be as above. Compute the price C(0) of a call option with strike price $100 and exercise time 1 if a) $A ( 1 ) = 1 0 5$ dollars, b) $A ( 1 ) = 1 1 5$ dollars. 

A put option with strike price $100 and exercise time 1 gives the right to sell one share of stock for $100 at time 1. This kind of option is worthless if the stock goes up, but it brings a profit otherwise, the payof being 

$$
P (1) = \left\{ \begin{array}{r l} 0 & \text {if stock goes up,} \\ 2 0 & \text {if stock goes down,} \end{array} \right.
$$

given that the prices $A ( 0 ) , A ( 1 ) , S ( 0 ) , S ( 1 )$ are the same as above. The notion of a portfolio may be extended to allow positions in put options, denoted by z, as before. 

The replicating and pricing procedure for puts follows the same pattern as for call options. In particular, the price $P ( 0 )$ of the put option is equal to the time 0 value of a replicating investment in stock and bonds. 

## Remark 1.4

There is some similarity between a put option and a short forward position: both involve selling an asset for a fixed price at a certain time in the future. However, an essential diference is that the holder of a short forward contract is committed to selling the asset for the fixed price, whereas the owner of a put option has the right but no obligation to sell. Moreover, an investor who wants to buy a put option will have to pay for it, whereas no payment is involved when a forward contract is exchanged. 

## Exercise 1.9

Once again, let the bond and stock prices A(0), A(1), S(0), S(1) be as above. Compute the price P(0) of a put option with strike price $100. 

An investor may wish to trade simultaneously in both kinds of options and, in addition, to take a forward position. In such cases new symbols z<sub>1</sub>, z<sub>2</sub>, z<sub>3</sub>, . . . will need to be reserved for all additional securities to describe the positions in a portfolio. A common feature of these new securities is that their payofs depend on the stock prices. Because of this they are called derivative securities or contingent claims. The general properties of derivative securities will be discussed in Chapter 7. In Chapter 8 the pricing and replicating schemes will be extended to more complicated (and more realistic) market models, as well as to other financial instruments. 

## 1.7 Managing Risk with Options

The availability of options and other derivative securities extends the possible investment scenarios. Suppose that your initial wealth is $1, 000 and compare the following two investments in the setup of the previous section: 

buy 10 shares; at time 1 they will be worth 

$$
1 0 \times S (1) = \left\{ \begin{array}{c l} 1, 2 0 0 & \text { if   stock   goes   up }, \\ 8 0 0 & \text { if   stock   goes   down }; \end{array} \right.
$$

or 

buy 1, 000/13.6364 ∼= 73.3333 options; in this case your final wealth will be 

$$
7 3. 3 3 3 3 \times C (1) \cong \left\{ \begin{array}{c l} 1, 4 6 6. 6 7 & \text {if stock goes up}, \\ 0. 0 0 & \text {if stock goes down}. \end{array} \right.
$$

If stock goes up, the investment in options will produce a much higher return than shares, namely about 46.67%. However, it will be disastrous otherwise: you will lose all your money. Meanwhile, when investing in shares, you would gain just 20% or lose 20%. Without specifying the probabilities we cannot compute the expected returns or standard deviations. Nevertheless, one would readily agree that investing in options is more risky than in stock. This can be exploited by adventurous investors. 

## Exercise 1.10

In the above setting, find the final wealth of an investor whose initial capital of $1, 000 is split fifty-fifty between stock and options. 

Options can also be employed to reduce risk. Consider an investor planning to purchase stock in the future. The share price today is S(0) = 100 dollars, but the investor will only have funds available at a future time t = 1, when the share price will become 

$$
S (1) = \left\{ \begin{array}{c l} 1 6 0 & \text {with probability p}, \\ 4 0 & \text {with probability 1 - p}, \end{array} \right.
$$

for some $0 \textless p \textless 1$ . Assume, as before, that $A ( 0 ) = 1 0 0$ and $A ( 1 ) = 1 1 0$ dollars, and compare the following two strategies: 

wait until time 1, when the funds become available, and purchase the stock for S(1); 

or 

at time 0 borrow money to buy a call option with strike price $100; then, at time 1 repay the loan with interest and purchase the stock, exercising the option if the stock price goes up. 

The investor will be open to considerable risk if she chooses to follow the first strategy. On the other hand, following the second strategy, she will need to borrow $C ( 0 ) \cong 3 1 . 8 1 8 2$ dollars to pay for the option. At time 1 she will have to repay $35 to clear the loan and may use the option to purchase the stock, hence the cost of purchasing one share will be 

$$
S (1) - C (1) + 3 5 = \left\{ \begin{array}{c l} 1 3 5 & \text {if stock goes up,} \\ 7 5 & \text {if stock goes down.} \end{array} \right.
$$

Clearly, the risk is reduced, the spread between these two figures being narrower than before. 

## Exercise 1.11

Compute the risk (as measured by the standard deviation of the return) involved in purchasing one share with and without the option if a) $p =$ 0.25, b) $p = 0 . 5 , \mathrm { { c } } ) \ p = 0 . 7 5$ 

## Exercise 1.12

Show that the risk (as measured by the standard deviation) of the above strategy involving an option is a half of that when no option is purchased, no matter what the probability $0 < p < 1$ is. 

If two options are bought, then the risk will be reduced to nil: 

$$
S (1) - 2 \times C (1) + 7 0 = 1 1 0 \text { with   probability } 1.
$$

This strategy turns out to be equivalent to a long forward contract, since the forward price of the stock is exactly $110 (see Section 1.5). It is also equivalent to borrowing money to purchase a share for $100 today and repaying $110 to clear the loan at time 1. 

Chapter 9 on financial engineering will discuss various ways of managing risk with options: magnifying or reducing risk, dealing with complicated risk exposure, and constructing payof profiles tailor made to meet the specific needs of an investor. 

## 2.1 Time Value of Money

It is a fact of life that $100 to be received after one year is worth less than the same amount today. The main reason is that money due in the future o locked in a fixed term account cannot be spent right away. One would therefore expect to be compensated for postponed consumption. In addition, prices may rise in the meantime and the amount will not have the same purchasing power as it would have at present. Finally, there is always a risk, even if a negligible one, that the money will never be received. Whenever a future payment is uncertain to some degree, its value today will be reduced to compensate for the risk. (However, in the present chapter we shall consider situations free from such risk.) As generic examples of risk-free assets we shall consider a bank deposit or a bond. 

The way in which money changes its value in time is a complex issue of fundamental importance in finance. We shall be concerned mainly with two questions: 

What is the future value of an amount invested or borrowed today? 

What is the present value of an amount to be paid or received at 

a certain time in the future? 

The answers depend on various factors, which will be discussed in the present chapter. This topic is often referred to as the time value of money. 

## 2.1.1 Simple Interest

Suppose that an amount is paid into a bank account, where it is to earn interest. The future value of this investment consists of the initial deposit, called the principal and denoted by $P _ { : }$ , plus all the interest earned since the money was deposited in the account. 

To begin with, we shall consider the case when interest is attracted only by the principal, which remains unchanged during the period of investment. For example, the interest earned may be paid out in cash, credited to anothe account attracting no interest, or credited to the original account after some longer period. 

After one year the interest earned will be $r P$ , where $r > 0$ is the interest rate. The value of the investment will thus become $V ( 1 ) = P + r P = ( 1 + r ) P .$ After two years the investment will grow to $V ( 2 ) = ( 1 + 2 r ) P .$ . Consider a fraction of a year. Interest is typically calculated on a daily basis: the interest earned in one day will be $\scriptstyle { \frac { 1 } { 3 6 5 } } r P$ . After n days the interest will be ${ \frac { n } { 3 6 5 } } r P$ and the total value of the investment will become $\begin{array} { r } { V ( \frac { n } { 3 6 5 } ) \ : = \ : ( 1 + \frac { n } { 3 6 5 } r ) P . } \end{array}$ This motivates the following rule of simple interest: The value of the investment at time t, denoted by $V ( t )$ , is given by 

$$
V (t) = (1 + t r) P,\tag{2.1}
$$

where time t, expressed in years, can be an arbitrary non-negative real number; see Figure 2.1. In particular, we have the obvious equality $V ( 0 ) = P . $ The number $1 + r t$ is called the growth factor. Here we assume that the interest rate $r$ is constant. If the principal P is invested at time s, rather than at time 0, then the value at time $t \geq s$ will be 

$$
V (t) = (1 + (t - s) r) P.\tag{2.2}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/61c00442ae01414bf137efb6d09401c254de8d1ec1d9fd6697beb1d97ca431d6.jpg)



Figure 2.1 Principal attracting simple interest at 10% $( r = 0 . 1 , P = 1 )$


Throughout this book the unit of time will be one year. We shall transform any period expressed in other units (days, weeks, months) into a fraction of a year. 

## Example 2.1

Consider a deposit of $150 held for 20 days and attracting simple interest at a rate of 8%. This gives $\begin{array} { r } { t { } = \frac { 2 0 } { 3 6 5 } } \end{array}$ and $r = 0 . 0 8$ . After 20 days the deposit wil grow to $\begin{array} { r } { V ( \frac { 2 0 } { 3 6 5 } ) = ( 1 + \frac { 2 0 } { 3 6 5 } \times 0 . 0 8 ) \times 1 5 0 \cong 1 5 0 . 6 6 } \end{array}$ 

The return on an investment commencing at time s and terminating at time t will be denoted by $K ( s , t )$ . It is given by 

$$
K (s, t) = \frac {V (t) - V (s)}{V (s)}.\tag{2.3}
$$

In the case of simple interest 

$$
K (s, t) = (t - s) r,
$$

which clearly follows from (2.2). In particular, the interest rate is equal to the return over one year, 

$$
K (0, 1) = r.
$$

As a general rule, interest rates will always refer to a period of one year, fa cilitating the comparison between diferent investments, independently of their actual duration. By contrast, the return reflects both the interest rate and the length of time the investment is held. 

## Exercise 2.1

A sum of $9, 000 paid into a bank account for two months (61 days) to attract simple interest will produce $9, 020 at the and of the term. Find the interest rate r and the return on this investment. 

## Exercise 2.2

How much would you pay today to receive $1, 000 at a certain future date if you require a return of 2%? 

## Exercise 2.3

How long will it take for a sum of $800 attracting simple interest to become $830 if the rate is 9%? Compute the return on this investment. 

## Exercise 2.4

Find the principal to be deposited initially in an account attracting simple interest at a rate of 8% if $1, 000 is needed after three months (91 days). 

The last exercise is concerned with an important general problem: Find the initial sum whose value at time t is given. In the case of simple interest the answer is easily found by solving (2.1) for the principal, obtaining 

$$
V (0) = V (t) (1 + r t) ^ {- 1}.\tag{2.4}
$$

This number is called the present or discounted value of $V ( t )$ and $( 1 + r t ) ^ { - 1 }$ is the discount factor. 

## Example 2.2

A perpetuity is a sequence of payments of a fixed amount to be made at equal time intervals and continuing indefinitely into the future. For example, suppose that payments of an amount C are to be made once a year, the first payment due a year hence. This can be achieved by depositing 

$$
P = \frac {C}{r}
$$

in a bank account to earn simple interest at a constant rate r. Such a deposit will indeed produce a sequence of interest payments amounting to $C = r P$ payable every year. 

In practice simple interest is used only for short-term investments and for certain types of loans and deposits. It is not a realistic description of the value of money in the longer term. In the majority of cases the interest already earned can be reinvested to attract even more interest, producing a higher return than that implied by (2.1). This will be analysed in detail in what follows. 

## 2.1.2 Periodic Compounding

Once again, suppose that an amount P is deposited in a bank account, at tracting interest at a constant rate $r > 0$ . However, in contrast to the case of simple interest, we assume that the interest earned will now be added to the principal periodically, for example, annually, semi-annually, quarterly, monthly, or perhaps even on a daily basis. Subsequently, interest will be attracted not just by the original deposit, but also by all the interest earned so far. In these circumstances we shall talk of discrete or periodic compounding. 

## Example 2.3

In the case of monthly compounding the first interest payment of ${ \scriptstyle { \frac { r } { 1 2 } } } P$ will be due after one month, increasing the principal to $\begin{array} { r } { ( 1 + \frac { r } { 1 2 } ) P , } \end{array}$ all of which wil attract interest in the future. The next interest payment, due after two months, will thus be $\textstyle { \frac { r } { 1 2 } } ( 1 + { \frac { r } { 1 2 } } ) P ,$ and the capital will become $( 1 + { \textstyle { \frac { r } { 1 2 } } } ) ^ { 2 } P$ . After one year it will become $\begin{array} { r } { ( \bar { 1 } + \frac { r } { 1 2 } ) ^ { 1 2 } P , } \end{array}$ after n months it will be $( 1 + { \textstyle { \frac { r } { 1 2 } } } ) ^ { n } P ,$ and after t years $\begin{array} { r } { ( 1 + \frac { r } { 1 2 } ) ^ { 1 2 t } P } \end{array}$ . The last formula admits t equal to a whole number of months, that is, a multiple of $\textstyle { \frac { 1 } { 1 2 } }$ 

In general, if m interest payments are made per annum, the time between two consecutive payments measured in years will be $\textstyle { \frac { 1 } { m } }$ , the first interest payment being due at time $\textstyle { \frac { 1 } { m } }$ . Each interest payment will increase the principal by a factor of $\textstyle 1 + { \frac { r } { m } }$ . Given that the interest rate r remains unchanged, after t years the future value of an initial principal P will become 

$$
V (t) = \left(1 + \frac {r}{m}\right) ^ {t m} P,\tag{2.5}
$$

because there will be tm interest payments during this period. In this formula t must be a whole multiple of the period $\begin{array} { l } { { \frac { 1 } { m } } } \end{array}$ . The numbe $\begin{array} { r } { \left( 1 + \frac { r } { m } \right) ^ { t m } } \end{array}$ is the growth factor. 

The exact value of the investment may sometimes need to be known at time instants between interest payments. In particular, this may be so if the accoun is closed on a day when no interest payment is due. For example, what is the value after 10 days of a deposit of $100 subject to monthly compounding at 12%? One possible answer is $100, since the first interest payment would be due only after one whole month. This suggests that (2.5) should be extended to arbitrary values of t by means of a step function with steps of duration $\textstyle { \frac { 1 } { m } }$ as shown in Figure 2.2. Later on, in Remark 2.6 we shall see that the extension consistent with the No-Arbitrage Principle should use the right-hand side of (2.5) for all $t \geq 0$ 

## Exercise 2.5

How long will it take to double a capital attracting interest at $6 \%$ compounded daily? 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/e7dab746445d1f2b3f852ae84929517b7ef9cb0e81a8a80fb3d366b8bedeca68.jpg)



Figure 2.2 Annual compounding at 10% (m = 1, r = 0.1, P = 1)


## Exercise 2.6

What is the interest rate if a deposit subject to annual compounding is doubled after 10 years? 

## Exercise 2.7

Find and compare the future value after two years of a deposit of $100 attracting interest at a rate of 10% compounded a) annually and b) semiannually. 

## Proposition 2.1

The future value V(t) increases if any one of the parameters m, t, r or P increases, the others remaining unchanged. 

## Proof

It is immediately obvious from (2.5) that V(t) increases if t, r or P increases. To show that V(t) increases as the compounding frequency m increases, we need to verify that if $m < k$ , then 

$$
\left(1 + \frac {r}{m}\right) ^ {t m} <   \left(1 + \frac {r}{k}\right) ^ {t k}.
$$

The latter clearly reduces to 

$$
\left(1 + \frac {r}{m}\right) ^ {m} <   \left(1 + \frac {r}{k}\right) ^ {k},
$$

which can be verified directly using the binomial formula: 

$$
\begin{array}{l} \left(1 + \frac {r}{m}\right) ^ {m} = 1 + r + \frac {1 - \frac {1}{m}}{2 !} r ^ {2} + \dots + \frac {\left(1 - \frac {1}{m}\right) \times \cdots \times \left(1 - \frac {m - 1}{m}\right)}{m !} r ^ {m} \\ \leq 1 + r + \frac {1 - \frac {1}{k}}{2 !} r ^ {2} + \dots + \frac {\left(1 - \frac {1}{k}\right) \times \cdots \times \left(1 - \frac {m - 1}{k}\right)}{m !} r ^ {m} \\ <   1 + r + \frac {1 - \frac {1}{k}}{2 !} r ^ {2} + \dots + \frac {\left(1 - \frac {1}{k}\right) \times \cdots \times \left(1 - \frac {k - 1}{k}\right)}{k !} r ^ {k} \\ = \left(1 + \frac {r}{k}\right) ^ {k}. \end{array}
$$

The first inequality holds because each term of the sum on the left-hand side is no greater than the corresponding term on the right-hand side. The second inequality is true because the sum on the right-hand side contains m k additional non-zero terms as compared to the sum on the left-hand side. This completes the proof. □ 

## Exercise 2.8

Which will deliver a higher future value after one year, a deposit of $1, 000 attracting interest at 15% compounded daily, or at 15.5% compounded semi-annually? 

## Exercise 2.9

What initial investment subject to annual compounding at 12% is needed to produce $1, 000 after two years? 

The last exercise touches upon the problem of finding the present value of an amount payable at some future time instant in the case when periodic compounding applies. Here the formula for the present or discounted value of V(t) is 

$$
V (0) = V (t) (1 + \frac {r}{m}) ^ {- t m},
$$

the number $\begin{array} { r } { ( 1 + \frac { r } { m } ) ^ { - t m } } \end{array}$ being the discount factor. 

## Remark 2.1

Fix the terminal value V(t) of an investment. It is an immediate consequence of Proposition 2.1 that the present value increases if any one of the factors r, t, m decreases, the other ones remaining unchanged. 

## Exercise 2.10

Find the present value of $100, 000 to be received after 100 years if the interest rate is assumed to be 5% throughout the whole period and a) daily or b) annual compounding applies. 

One often requires the value $V ( t )$ of an investment at an intermediate time $0 < t < T$ , given the value $V ( T )$ at some fixed future time T. This can be achieved by computing the present value of $V ( T )$ , taking it as the principal, and running the investment forward up to time t. Under periodic compounding with frequency m and interest rate r, this obviously gives 

$$
V (t) = \left(1 + \frac {r}{m}\right) ^ {- (T - t) m} V (T).\tag{2.6}
$$

To find the return on a deposit attracting interest compounded periodically we use the general formula (2.3) and readily arrive at 

$$
K (s, t) = \frac {V (t) - V (s)}{V (s)} = (1 + \frac {r}{m}) ^ {(t - s) m} - 1.
$$

In particular, 

$$
K (0, \frac {1}{m}) = \frac {r}{m},
$$

which provides a simple way of computing the interest rate given the return. 

## Exercise 2.11

Find the return over one year under monthly compounding with $r =$ 10%. 

## Exercise 2.12

Which is greater, the interest rate r or the return $K ( 0 , 1 )$ if the compounding frequency m is greater than 1? 

## Remark 2.2

The return on a deposit subject to periodic compounding is not additive. Take, for simplicity, $m = 1$ . Then 

$$
\begin{array}{l} K (0, 1) = K (1, 2) = r, \\ K (0, 2) = (1 + r) ^ {2} - 1 = 2 r + r ^ {2}, \end{array}
$$

and clearly $K ( 0 , 1 ) + K ( 1 , 2 ) \neq K ( 0 , 2 )$ 

## 2.1.3 Streams of Payments

An annuity is a sequence of finitely many payments of a fixed amount due at equal time intervals. Suppose that payments of an amount C are to be made once a year for n years, the first one due a year hence. Assuming that annual compounding applies, we shall find the present value of such a stream of payments. We compute the present values of all payments and add them up to get 

$$
\frac {C}{1 + r} + \frac {C}{(1 + r) ^ {2}} + \frac {C}{(1 + r) ^ {3}} + \dots + \frac {C}{(1 + r) ^ {n}}.
$$

It is sometimes convenient to introduce the following seemingly cumbersome piece of notation: 

$$
\mathrm{PA} (r, n) = \frac {1}{1 + r} + \frac {1}{(1 + r) ^ {2}} + \dots + \frac {1}{(1 + r) ^ {n}}.\tag{2.7}
$$

This number is called the present value factor for an annuity. It allows us to express the present value of an annuity in a concise form: 

$$
\mathrm{PA} (r, n) \times C.
$$

The expression for $\operatorname { P A } ( r , n )$ can be simplified by using the formula 

$$
a + q a + q ^ {2} a + \dots + q ^ {n - 1} a = a \frac {1 - q ^ {n}}{1 - q}.
$$

In our case $\textstyle a = { \frac { 1 } { 1 + r } }$ and $\textstyle q = { \frac { 1 } { 1 + r } }$ , hence 

$$
\mathrm{PA} (r, n) = \frac {1 - (1 + r) ^ {- n}}{r}.\tag{2.8}
$$

## Remark 2.3

Note that an initial bank deposit of 

$$
P = \mathrm{PA} (r, n) \times C = \frac {C}{1 + r} + \frac {C}{(1 + r) ^ {2}} + \dots + \frac {C}{(1 + r) ^ {n}}
$$

attracting interest at a rate r compounded annually would produce a stream of n annual payments of C each. A deposit of $C ( 1 + r ) ^ { - 1 }$ would grow to $C$ after one year, which is just what is needed to cover the first annuity payment. A deposit of $C ( 1 + r ) ^ { - 2 }$ would become C after two years to cover the second payment, and so on. Finally, a deposit of $C ( 1 + r ) ^ { - n }$ would deliver the last payment of C due after n years. 

## Example 2.4

Consider a loan of $1, 000 to be paid back in 5 equal instalments due at yearly intervals. The instalments include both the interest payable each year calculated at 15% of the current outstanding balance and the repayment of a fraction of the loan. A loan of this type is called an amortised loan. The amount of each instalment can be computed as 

$$
\frac {1 , 0 0 0}{\mathrm{PA} (15\% , 5)} \cong 2 9 8. 3 2.
$$

This is because the loan is equivalent to an annuity from the point of view of the lender. 

## Exercise 2.13

What is the amount of interest included in each instalment? How much of the loan is repaid as part of each instalment? What is the outstanding balance of the loan after each instalment is paid? 

## Exercise 2.14

How much can you borrow if the interest rate is 18%, you can aford to pay $10, 000 at the end of each year, and you want to clear the loan in 10 years? 

## Exercise 2.15

Suppose that you deposit $1, 200 at the end of each year for 40 years, subject to annual compounding at a constant rate of 5%. Find the balance after 40 years. 

## Exercise 2.16

Suppose that you took a mortgage of $100, 000 on a house to be paid back in full by 10 equal annual instalments, each consisting of the in terest due on the outstanding balance plus a repayment of a part of the amount borrowed. If you decided to clear the mortgage after eight years, how much money would you need to pay on top of the 8th instalment, assuming that a constant annual compounding rate of 6% applies throughout the period of the mortgage? 

Recall that a perpetuity is an infinite sequence of payments of a fixed amoun C occurring at the end of each year. The formula for the present value of a perpetuity can be obtained from (2.7) in the limit as $n \to \infty$ 

$$
\lim _ {n \to \infty} \mathrm{PA} (r, n) \times C = \frac {C}{1 + r} + \frac {C}{(1 + r) ^ {2}} + \frac {C}{(1 + r) ^ {3}} + \dots = \frac {C}{r}.\tag{2.9}
$$

The limit amounts to taking the sum of a geometric series. 

## Remark 2.4

The present value of a perpetuity is given by the same formula as in Example 2.2, even though periodic compounding has been used in place of simple interest. In both cases the annual payment C is exactly equal to the interest earned throughout the year, and the amount remaining to earn interest in the following year is always $\frac { C } { r }$ . Nevertheless, periodic compounding allows us to view the same sequence of payments in a diferent way: The present value $\frac { C } { r }$ of the perpetuity is decomposed into infinitely many parts, as in (2.9), each responsible for producing one future payment of C. 

## Remark 2.5

Formula (2.8) for the annuity factor is easier to memorise in the following way, using the formula for a perpetuity: The sequence of n payments of $C = 1$ can be represented as the diference between two perpetuities, one starting now and the other after n years. (Cutting of the tail of a perpetuity, we obtain an annuity.) In doing so we need to compute the present value of the latter perpetuity. This can be achieved by means of the discount factor $\left( 1 + r \right) ^ { - n }$ Hence, 

$$
\mathrm{PA} (r, n) = \frac {1}{r} - \frac {1}{r} \times \frac {1}{(1 + r) ^ {n}} = \frac {1 - (1 + r) ^ {- n}}{r}.
$$

## Exercise 2.17

Find a formula for the present value of an infinite stream of payments of the form C, $C ( 1 + g ) , C ( 1 + g ) ^ { 2 } , \ldots ,$ , growing at a constant rate g. By the tail-cutting procedure find a formula for the present value of n such payments. 

## 2.1.4 Continuous Compounding

Formula (2.5) for the future value at time t of a principal P attracting interest at a rate $r > 0$ compounded m times a year can be written as 

$$
V (t) = \left[ \left(1 + \frac {r}{m}\right) ^ {\frac {m}{r}} \right] ^ {t r} P.
$$

In the limit as $m \to \infty$ , we obtain 

$$
V (t) = \mathrm{e} ^ {t r} P,\tag{2.10}
$$

where 

$$
\mathrm{e} = \lim _ {x \rightarrow \infty} \left(1 + \frac {1}{x}\right) ^ {x}
$$

is the base of natural logarithms. This is known as continuous compounding. The corresponding growth factor is $\mathrm { e } ^ { t r }$ . A typical graph of $V ( t )$ is shown in Figure 2.3. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/b4c2f8ebd89b6ee0635acb48dba5a4b87255e9bac13fec2041b50b4af3ce0884.jpg)



Figure 2.3 Continuous compounding at 10% $( r = 0 . 1 , P = 1 )$


The derivative of $V ( t ) = \mathrm { e } ^ { t r } P$ is 

$$
V ^ {\prime} (t) = r \mathrm{e} ^ {t r} P = r V (t).
$$

In the case of continuous compounding the rate of the growth is proportional to the current wealth 

Formula (2.10) is a good approximation of the case of periodic compounding when the frequency m is large. It is simpler and lends itself more readily to transformations than the formula for periodic compounding. 

## Exercise 2.18

How long will it take to earn $1 in interest if $1, 000, 000 is deposited at 10% compounded continuously? 

## Exercise 2.19

In 1626 Peter Minuit, governor of the colony of New Netherland, bought the island of Manhattan from Indians paying with beads, cloth, and trinkets worth $24. Find the value of this sum in year 2000 at 5% com pounded a) continuously and b) annually. 

## Proposition 2.2

Continuous compounding produces higher future value than periodic compounding with any frequency m, given the same initial principal P and interest rate r. 

## Proof

It sufices to verify that 

$$
\mathrm{e} ^ {t r} > (1 + \frac {r}{m}) ^ {t m} = \left[ (1 + \frac {r}{m}) ^ {\frac {m}{r}} \right] ^ {r t}.
$$

The inequality holds because the sequence $( 1 + { \frac { r } { m } } ) ^ { \frac { m } { r } }$ is increasing and converges to e as m $\nearrow \infty$ □ 

## Exercise 2.20

What will be the diference between the value after one year of $100 deposited at 10% compounded monthly and compounded continuously? How frequent should the periodic compounding be for the diference to be less than $0.01? 

The present value under continuous compounding is obviously given by 

$$
V (0) = V (t) \mathrm{e} ^ {- t r}.
$$

In this case the discount factor is $\mathrm { e } ^ { - t r }$ . Given the terminal value $V ( T )$ , we clearly have 

$$
V (t) = \mathrm{e} ^ {- r (T - t)} V (T).\tag{2.11}
$$

## Exercise 2.21

Find the present value of $1, 000, 000 to be received after 20 years assuming continuous compounding at 6%. 

## Exercise 2.22

Given that the future value of $950 subject to continuous compounding will be $1, 000 after half a year, find the interest rate. 

The return $K ( s , t )$ defined by (2.3) on an investment subject to continuous compounding fails to be additive, just like in the case of periodic compounding. It proves convenient to introduce the logarithmic return 

$$
k (s, t) = \ln {\frac {V (t)}{V (s)}}.\tag{2.12}
$$

## Proposition 2.3

The logarithmic return is additive, 

$$
k (s, t) + k (t, u) = k (s, u).
$$

## Proof

This is an easy consequence of (2.12): 

$$
\begin{array}{c} k (s, t) + k (t, u) = \ln \frac {V (t)}{V (s)} + \ln \frac {V (u)}{V (t)} \\ = \ln \frac {V (t)}{V (s)} \frac {V (u)}{V (t)} = \ln \frac {V (u)}{V (s)} = k (s, u). \end{array}
$$

If $V ( t )$ is given by (2.10), then $k ( s , t ) = r ( t - s )$ , which enables us to recover the interest rate 

$$
r = \frac {k (s , t)}{t - s}.
$$

## Exercise 2.23

Suppose that the logarithmic return over 2 months on an investment subject to continuous compounding is 3%. Find the interest rate. 

## 2.1.5 How to Compare Compounding Methods

As we have already noticed, frequent compounding will produce a higher future value than less frequent compounding if the interest rates and the initial principal are the same. We shall consider the general circumstances in which one compounding method will produce either the same or higher future value than another method, given the same initial principal. 

## Example 2.5

Suppose that certificates promising to pay $120 after one year can be purchased or sold now, or at any time during this year, for $100. This is consistent with a constant interest rate of 20% under annual compounding. If an investor decided to sell such a certificate half a year after the purchase, what price would it fetch? Suppose it is $110, a frequent first guess based on halving the annual profit of $20. However, this turns out to be too high a price, leading to the following arbitrage strategy: 

Borrow $1, 000 to buy 10 certificates for $100 each. 

After six months sell the 10 certificates for $110 each and buy 11 new certificates for $100 each. The balance of these transactions is nil. 

After another six months sell the 11 certificates for $110 each, cashing $1, 210 in total, and pay $1, 200 to clear the loan with interest. The balance of $10 would be the arbitrage profit. 

A similar argument shows that the certificate price after six months cannot be too low, say, $109. 

The price of a certificate after six months is related to the interest rate under semi-annual compounding: If this rate is $r ,$ then the price is 100 $\left( 1 + { \frac { r } { 2 } } \right) $ dollars and vice versa. Arbitrage will disappear if the corresponding growth factor $\begin{array} { r } { \left( 1 + \frac { r } { 2 } \right) ^ { 2 } } \end{array}$ over one year is equal to the growth factor 1.2 under annual compounding, 

$$
\left(1 + \frac {r}{2}\right) ^ {2} = 1. 2,
$$

which gives $r \cong 0 . 1 9 0 9$ , or 19.09%. If so, then the certificate price after six months should be 100 $\textstyle \left( 1 + { \frac { 0 . 1 9 0 9 } { 2 } } \right) \cong 1 0 9 . 5 4$ dollars. 

The idea based on considering the growth factors over a fixed period, typi cally one year, can be used to compare any two compounding methods. 

## Definition 2.1

We say that two compounding methods are equivalent if the corresponding growth factors over a period of one year are the same. If one of the growth factors exceeds the other, then the corresponding compounding method is said to be preferable. 

## Example 2.6

Semi-annual compounding at 10% is equivalent to annual compounding at 10.25%. Indeed, in the former case the growth factor over a period of one year is 

$$
\left(1 + \frac {0 . 1}{2}\right) ^ {2} = 1. 1 0 2 5,
$$

which is the same as the growth factor in the latter case. Both are preferable to monthly compounding at 9%, for which the growth factor over one year is only 

$$
\left(1 + \frac {0 . 0 9}{1 2}\right) ^ {1 2} \cong 1. 0 9 3 8.
$$

We can freely switch from one compounding method to another equivalent method by recalculating the interest rate. In the chapters to follow we shall normally use either annual or continuous compounding. 

## Exercise 2.24

Find the rate for continuous compounding equivalent to monthly compounding at 12%. 

## Exercise 2.25

Find the frequency of periodic compounding at 20% to be equivalent to annual compounding at 21%. 

Instead of comparing the growth factors, it is often convenient to compare the so-called efective rates as defined below. 

## Definition 2.2

For a given compounding method with interest rate r the efective rate $r _ { \mathrm { e } }$ is one that gives the same growth factor over a one year period under annual compounding. 

In particular, in the case of periodic compounding with frequency m and rate $r$ the efective rate $r _ { \mathrm { e } }$ satisfies 

$$
\left(1 + \frac {r}{m}\right) ^ {m} = 1 + r _ {\mathrm{e}}.
$$

In the case of continuous compounding with rate $r$ 

$$
\mathrm{e} ^ {r} = 1 + r _ {\mathrm{e}}.
$$

## Example 2.7

In the case of semi-annual compounding at 10% the efective rate is 10.25%, see Example 2.6. 

## Proposition 2.4

Two compounding methods are equivalent if and only if the corresponding efective rates $r _ { \mathrm { e } }$ and $r _ { \mathrm { e } } ^ { \prime }$ are equal, $r _ { \mathrm { e } } = r _ { \mathrm { e } } ^ { \prime }$ . The compounding method with efective rate $r _ { \mathrm { e } }$ is preferable to the other method if and only if $r _ { \mathrm { e } } > r _ { \mathrm { e } } ^ { \prime }$ 

## Proof

This is because the growth factors over one year are $1 + r _ { \mathrm { e } }$ and $1 + r _ { \mathrm { e } } ^ { \prime }$ , respectively. □ 

## Example 2.8

In Exercise 2.8 we have seen that daily compounding at 15% is preferable to semi-annual compounding at 15.5%. The corresponding efective rates $r _ { \mathrm { e } }$ and $r _ { \mathrm { e } } ^ { \prime }$ can be found from 

$$
1 + r _ {\mathrm{e}} = \left(1 + \frac {0 . 1 5}{3 6 5}\right) ^ {3 6 5} \cong 1. 1 6 1 8,
$$

$$
1 + r _ {\mathrm{e}} ^ {\prime} = \left(1 + \frac {0 . 1 5 5}{2}\right) ^ {2} \cong 1. 1 6 1 0.
$$

This means that $r _ { \mathrm { e } }$ is about 16.18% and $r _ { \mathrm { e } } ^ { \prime }$ about 16.10%. 

## Remark 2.6

Recall that formula (2.5) for periodic compounding, that is, 

$$
V (t) = \left(1 + \frac {r}{m}\right) ^ {t m} P,
$$

admits only time instants t being whole multiples of the compounding period $\textstyle { \frac { 1 } { m } }$ . An argument similar to that in Example 2.5 shows that the appropriate noarbitrage value of an initial sum P at any time $t \geq 0$ should be $\begin{array} { r } { \left( 1 + \frac { r } { m } \right) ^ { t m } P } \end{array}$ A reasonable extension of (2.5) is therefore to use the right-hand side for all $t \geq 0$ rather than just for whole multiples of $\begin{array} { l } { { \frac { 1 } { m } } } \end{array}$ . From now on we shall always use this extension. 

In terms of the efective rate $r _ { \mathrm { e } }$ the future value can be written as 

$$
V (t) = \left(1 + r _ {\mathrm{e}}\right) ^ {t} P.
$$

for all $t \geq 0$ . This applies both to continuous compounding and to periodic compounding extended to arbitrary times as in Remark 2.6. Proposition 2.4 implies that, given the same initial principal, equivalent compounding methods will produce the same future value for all times $t \geq 0$ . Similarly, a compounding method preferable to another one will produce a higher future value for all $t > 0$ 

## Remark 2.7

Simple interest does not fit into the scheme for comparing compounding meth ods. In this case the future value $V ( t )$ is a linear function of time t, whereas it is an exponential function if either continuous or periodic compounding applies. The graphs of such functions have at most two intersection points, so they can never be equal to one another for all times $t \geq 0$ (except for the trivial case of zero principal). 

## Exercise 2.26

What is the present value of an annuity consisting of monthly payments of an amount $C$ continuing for n years? Express the answer in terms of the efective rate $r _ { \mathrm { e } }$ . 

## Exercise 2.27

What is the present value of a perpetuity consisting of bimonthly payments of an amount $C ?$ Express the answer in terms of the efective rate $r _ { \mathrm { e } }$ 

## 2.2 Money Market

The money market consists of risk-free (more precisely, default-free) securities. An example is a bond, which is a financial security promising the holder a sequence of guaranteed future payments. Risk-free means here that these payments will be delivered with certainty. (Nevertheless, even in this case risk cannot be completely avoided, since the market prices of such securities may fluctuate unpredictably; see Chapters 10 and 11.) There are many kinds of bonds like treasury bills and notes, treasury, mortgage and debenture bonds, commercial papers, and others with various particular arrangements concern ing the issuing institution, duration, number of payments, embedded rights and guarantees. 

## 2.2.1 Zero-Coupon Bonds

The simplest case of a bond is a zero-coupon bond, which involves just a single payment. The issuing institution (for example, a government, a bank or a company) promises to exchange the bond for a certain amount of money F, called the face value, on a given day T, called the maturity date. Typically, the life span of a zero-coupon bond is up to one year, the face value being some round figure, for example 100. In efect, the person or institution who buys the bond is lending money to the bond writer. 

Given the interest rate, the present value of such a bond can easily be computed. Suppose that a bond with face value F = 100 dollars is maturing in one year, and the annual compounding rate r is 12%. Then the present value of the bond should be 

$$
V (0) = F (1 + r) ^ {- 1} \cong 8 9. 2 9
$$

dollars. 

In reality, the opposite happens: Bonds are freely traded and their prices are determined by market forces, whereas the interest rate is implied by the bond prices, 

$$
r = \frac {F}{V (0)} - 1.\tag{2.13}
$$

This formula gives the implied annual compounding rate. For instance, if a one-year bond with face value $100 is being traded at $91, then the implied rate is 9.89%. 

For simplicity, we shall consider unit bonds with face value equal to one uni of the home currency, $F = 1$ 

Typically, a bond can be sold at any time prior to maturity at the market price. This price at time t is denoted $B ( t , T )$ . In particular, $B ( 0 , T )$ is the current, time 0 price of the bond, and $B ( T , T ) = 1$ is equal to the face value. Again, these prices determine the interest rates by applying formulae (2.6) and (2.11) with $V ( t ) = B ( t , T ) , V ( T ) = 1$ . For example, the implied annual compounding rate satisfies the equation 

$$
B (t, T) = (1 + r) ^ {- (T - t)}.
$$

The last formula has to be suitably modified if a diferent compounding method is used. Using periodic compounding with frequency m, we need to solve the equation 

$$
B (t, T) = \left(1 + \frac {r}{m}\right) ^ {- m (T - t)}.
$$

In the case of continuous compounding the equation for the implied rate satisfie 

$$
B (t, T) = \mathrm{e} ^ {- r (T - t)}.
$$

Of course all these diferent implied rates are equivalent to one another, since the bond price does not depend on the compounding method used. 

## Remark 2.8

In general, the implied interest rate may depend on the trading time t as well as on the maturity time T. This is an important issue, which will be discussed in Chapters 10 and 11. For the time being, we adopt the simplifying assumption that the interest rate remains constant throughout the period up to maturity. 

## Exercise 2.28

An investor paid $95 for a bond with face value $100 maturing in six months. When will the bond value reach $99 if the interest rate remains constant? 

## Exercise 2.29

Find the interest rates for annual, semi-annual and continuous compounding implied by a unit bond with $B ( 0 . 5 , 1 ) = 0 . 9 4 5 5$ 

Note that $B ( 0 , T )$ is the discount factor and $B ( 0 , T ) ^ { - 1 }$ is the growth factor for each compounding method. These universal factors are all that is needed to compute the time value of money, without resorting to the corresponding interest rates. However, interest rates are useful because they are more intuitive. 

For an average bank customer the information that a one-year $100 bond can be purchased for $92.59 may not be as clear as the equivalent statement that a deposit will earn 8% interest if kept for one year. 

## 2.2.2 Coupon Bonds

Bonds promising a sequence of payments are called coupon bonds. These pay ments consist of the face value due at maturity, and coupons paid regularly, typically annually, semi-annually, or quarterly, the last coupon due at maturity. The assumption of constant interest rates allows us to compute the price of a coupon bond by discounting all the future payments. 

## Example 2.9

Consider a bond with face value F = 100 dollars maturing in five years, $T = 5$ with coupons of $C = 1 0$ dollars paid annually, the last one at maturity. This means a stream of payments of 10, 10, 10, 10, 110 dollars at the end of each consecutive year. Given the continuous compounding rate r, say 12%, we can find the price of the bond: 

$$
V (0) = 1 0 \mathrm{e} ^ {- r} + 1 0 \mathrm{e} ^ {- 2 r} + 1 0 \mathrm{e} ^ {- 3 r} + 1 0 \mathrm{e} ^ {- 4 r} + 1 1 0 \mathrm{e} ^ {- 5 r} \cong 9 0. 2 7
$$

dollars. 

## Exercise 2.30

Find the price of a bond with face value $100 and $5 annual coupons that matures in four years, given that the continuous compounding rate is a) 8% or b) 5%. 

## Exercise 2.31

Sketch the graph of the price of the bond in Exercise 2.30 as a function of the continuous compounding rate r. What is the value of this function for $r = 0 ?$ What is the limit as $r  \infty ?$ 

## Example 2.10

We continue Example 2.9. After one year, once the first coupon is cashed, the bond becomes a four-year bond worth 

$$
V (1) = 1 0 \mathrm{e} ^ {- r} + 1 0 \mathrm{e} ^ {- 2 r} + 1 0 \mathrm{e} ^ {- 3 r} + 1 1 0 \mathrm{e} ^ {- 4 r} \cong 9 1. 7 8
$$

dollars. Observe that the total wealth at time 1 is 

$$
V (1) + C = V (0) \mathrm{e} ^ {r}.
$$

Six months later the bond will be worth 

$$
V (1. 5) = 1 0 \mathrm{e} ^ {- 0. 5 r} + 1 0 \mathrm{e} ^ {- 1. 5 r} + 1 0 \mathrm{e} ^ {- 2. 5 r} + 1 1 0 \mathrm{e} ^ {- 3. 5 r} \cong 9 7. 4 5
$$

dollars. After four years the bond will become a zero-coupon bond with face value $110 and price 

$$
V (4) = 1 1 0 \mathrm{e} ^ {- r} \cong 9 7. 5 6
$$

dollars. 

An investor may choose to sell the bond at any time prior to maturity. The price at that time can once again be found by discounting all the payments due at later times. 

## Exercise 2.32

Sketch the graph of the price of the coupon bond in Examples 2.9 and 2.10 as a function of time. 

## Exercise 2.33

How long will it take for the price of the coupon bond in Examples 2.9 and 2.10 to reach $95 for the first time? 

The coupon can be expressed as a fraction of the face value. Assuming that coupons are paid annually, we shall write $C = i F$ , where i is called the coupon rate. 

## Proposition 2.5

Whenever coupons are paid annually, the coupon rate is equal to the interest rate for annual compounding if and only if the price of the bond is equal to its face value. In this case we say that the bond sells at par. 

## Proof

To avoid cumbersome notation we restrict ourselves to an example. Suppose that annual compounding with $r = i$ applies, and consider a bond with face value $F = 1 0 0$ maturing in three years, $T = 3$ . Then the price of the bond is 

$$
\frac {C}{1 + r} + \frac {C}{(1 + r) ^ {2}} + \frac {F + C}{(1 + r) ^ {3}} = \frac {r F}{1 + r} + \frac {r F}{(1 + r) ^ {2}} + \frac {F (1 + r)}{(1 + r) ^ {3}}
$$

$$
= \frac {r F}{1 + r} + \frac {r F}{(1 + r) ^ {2}} + \frac {F}{(1 + r) ^ {2}} = \frac {r F}{1 + r} + \frac {F (1 + r)}{(1 + r) ^ {2}} = F.
$$

Conversely, note that 

$$
{\frac {C}{1 + r}} + {\frac {C}{(1 + r) ^ {2}}} + {\frac {F + C}{(1 + r) ^ {3}}}
$$

is one-to-one as a function of $r$ (in fact, a strictly decreasing function), so it assumes the value $F$ exactly once, and we know this happens for $r = i .$ □ 

## Remark 2.9

If a bond sells below the face value, it means that the implied interest rate is higher than the coupon rate (since the price of a bond decreases when the interest rate goes up). If the bond price is higher than the face value, it means that the interest rate is lower than the coupon rate. This may be important information in real circumstances, where the bond price is determined by the market and gives an indication of the level of interest rates. 

## Exercise 2.34

A bond with face value $F = 1 0 0$ and annual coupons $C = 8$ maturing after three years, at $T = 3$ , is trading at par. Find the implied continuous compounding rate. 

## 2.2.3 Money Market Account

An investment in the money market can be realised by means of a financial intermediary, typically an investment bank, who buys and sells bonds on behalf of its customers (thus reducing transaction costs). The risk-free position of an investor is given by the level of his or her account with the bank. It is convenient to think of this account as a tradable asset, which is indeed the case, since the bonds themselves are tradable. A long position in the money market involves buying the asset, that is, investing money. A short position amounts to borrowing money. 

First, consider an investment in a zero-coupon bond closed prior to maturity. $\mathrm { A n }$ initial amount $A ( 0 )$ invested in the money market makes it possible to purchase $A ( 0 ) / B ( 0 , T )$ bonds. The value of each bond will fetch 

$$
B (t, T) = \mathrm{e} ^ {- (T - t) r} = \mathrm{e} ^ {r t} \mathrm{e} ^ {- r T} = \mathrm{e} ^ {r t} B (0, T)
$$

at time t. As a result, the investment will reach 

$$
A (t) = \frac {A (0)}{B (0 , T)} B (t, T) = A (0) \mathrm{e} ^ {r t}
$$

at time $t \leq T$ 

## Exercise 2.35

Find the return on a 75-day investment in zero-coupon bonds if $B ( 0 , 1 ) =$ 0.89. 

## Exercise 2.36

The return on a bond over six months is $7 \%$ . Find the implied continuous compounding rate. 

## Exercise 2.37

After how many days will a bond purchased for $B ( 0 , 1 ) = 0 . 9 2$ produce a 5% return? 

The investment in a bond has a finite time horizon. It will be terminated with $A ( T ) = A ( 0 ) \mathrm { e } ^ { r T }$ at the time $T$ of maturity of the bond. To extend the position in the money market beyond T one can reinvest the amount $A ( T )$ into a bond newly issued at time T, maturing at $T ^ { \prime } > T$ . Taking $A ( T )$ as the initial investment with T playing the role of the starting time, we have 

$$
A (t ^ {\prime}) = A (T) \mathrm{e} ^ {r (t ^ {\prime} - T)} = A (0) \mathrm{e} ^ {r t ^ {\prime}}
$$

for $T \leq t ^ { \prime } \leq T ^ { \prime }$ . By repeating this argument, we readily arrive at the conclusion that an investment in the money market can be prolonged for as long as required, the formula 

$$
A (t) = A (0) \mathrm{e} ^ {r t}\tag{2.14}
$$

being valid for all $t \geq 0$ 

## Exercise 2.38

Suppose that one dollar is invested in zero-coupon bonds maturing after one year. At the end of each year the proceeds are reinvested in new bonds of the same kind. How many bonds will be purchased at the end of year 9? Express the answer in terms of the implied continuous compounding rate. 

An alternative way to prolong an investment in the money market for as long as required is to reinvest the face value of any bonds maturing at time T in other bonds issued at time $0 ,$ but maturing at a later time $t > T$ . Having invested $A ( 0 )$ initially to buy unit bonds maturing at time $T ,$ , we will have the sum of $A ( 0 ) / B ( 0 , T )$ at our disposal at time T. At this time we chose a bond maturing at time t, its price at $T$ being $B ( T , t )$ . At time t this investment will be worth 

$$
\frac {A (0)}{B (0 , T) B (T , t)} = \frac {A (0)}{B (0 , t)} = A (0) \mathrm{e} ^ {r t},
$$

the same as in (2.14). 

Finally, consider coupon bonds as a tool to manufacture an investment in the money market. Suppose for simplicity that the first coupon $C$ is due after one year. At time 0 we buy $A ( 0 ) / V ( 0 )$ coupon bonds. After one year we cash the coupon and sell the bond for $V ( 1 )$ , receiving the total sum $C + V ( 1 ) = V ( 0 ) \mathrm { e } ^ { r }$ (see Example 2.10). Because the interest rate is constant, this sum of money is certain. In this way we have efectively created a zero-coupon bond with face value $V ( 0 ) \mathrm { e } ^ { r }$ maturing at time 1. It means that the scheme worked out above for zero-coupon bonds applies to coupon bonds as well, resulting in the same formula (2.14) for $A ( t )$ 

## Exercise 2.39

The sum of $1, 000 is invested in five-year bonds with face value $100 and $8 coupons paid annually. All coupons are reinvested in bonds of the same kind. Assuming that the bonds are trading at par and the interest rate remains constant throughout the period to maturity, compute the number of bonds held during each consecutive year of the investment. 

As we have seen, under the assumption that the interest rate is constant, the function $A ( t )$ does not depend on the way the money market account is run, that is, it neither depends on the types of bonds selected for investment nor on the method of extending the investment beyond the maturity of the bonds. 

Throughout most of this book we shall assume $A ( t )$ to be deterministic and known. Indeed, we assume that $A ( t ) = \mathrm { e } ^ { r t }$ , where r is a constant interest rate. Variable interest rates will be considered in Chapter 10 and a random money market account will be studied in Chapter 11. 

This page intentionally left blank 

The future prices of any asset are unpredictable to a certain extent. In this chapter we shall typically be concerned with common stock, though any security such as foreign currency, a commodity, or even a partially unpredictable future cash flow can be considered. Market prices depend on the choices and decisions made by a great number of agents acting under conditions of uncertainty. It is therefore reasonable to treat the prices of assets as random. However, little more can be said in a fully general situation. We shall therefore impose specific conditions on asset prices, motivated by a need for the mathematical model to be realistic and relevant on the one hand, and tractable on the other hand. 

## 3.1 Dynamics of Stock Prices

The price of stock at time t will be denoted by $S ( t )$ . It is assumed to be strictly positive for all t. We take $t = 0$ to be the present time, $S ( 0 )$ being the current stock price, known to all investors. The future prices $S ( t )$ for $t > 0$ remain unknown, in general. Mathematically, $S ( t )$ can be represented as a positive random variable on a probability space Ω, that is, 

$$
S (t): \Omega \to (0, \infty).
$$

The probability space $\varOmega$ consists of all feasible price movement ‘scenarios’ $\omega \in$ $\varOmega$ . We shall write $S ( t , \omega )$ to denote the price at time t if the market follows scenario $\omega \in \varOmega$ 

The current stock price $S ( 0 )$ known to all investors is simply a positive number, but it can be thought of as a constant random variable. The unknown future prices $S ( t )$ for $t > 0$ are non-constant random variables. This means that for each $t > 0$ there are at least two scenarios $\omega , \widetilde { \omega } \in \varOmega$ such that $S ( t , \omega ) \neq $ $S ( t , \widetilde { \omega } )$ 

We assume that time runs in a discrete manner, $\textit { t } = \ n \tau$ , where $n =$ $0 , 1 , 2 , 3 , \ldots$ . and $\tau$ is a fixed time step, typically a year, a month, a week, a day, or even a minute or a second to describe some hectic trading. Because we take one year as the unit measure of time, a month corresponds to $\tau = 1 / 1 2$ , a week corresponds to $\tau = 1 / 5 2$ , a day to $\tau = 1 / 3 6 5$ , and so on. 

To simplify our notation we shall write $S ( 0 ) , S ( 1 ) , S ( 2 ) , \ldots , S ( n ) , . .$ . instead of $S ( 0 ) , S ( \tau ) , S ( 2 \tau ) , \ldots , S ( n \tau ) , \ldots .$ , identifying n with $n \tau$ . This convention will in fact be adopted for many other time-dependent quantities. 

## Example 3.1

Consider a market that can follow just two scenarios, boom or recession, de noted by $\omega _ { 1 }$ and $\omega _ { 2 }$ , respectively. The current share price of a certain stock is $10, which may rise to $12 after one year if there is a boom or come down to $7 in the case of recession. In these circumstances $\varOmega = \{ \omega _ { 1 } , \omega _ { 2 } \}$ and, putting $\tau = 1$ , we have 

<table><tr><td>Scenario</td><td><eq>S(0)</eq></td><td><eq>S(1)</eq></td></tr><tr><td><eq>\omega_{1}</eq>(boom)</td><td>10</td><td>12</td></tr><tr><td><eq>\omega_{2}</eq>(recession)</td><td>10</td><td>7</td></tr></table>

## Example 3.2

Suppose that there are three possible market scenarios, $\varOmega = \{ \omega _ { 1 } , \omega _ { 2 } , \omega _ { 3 } \}$ , the stock prices taking the following values over two time steps: 

<table><tr><td>Scenario</td><td><eq>S(0)</eq></td><td><eq>S(1)</eq></td><td><eq>S(2)</eq></td></tr><tr><td><eq>\omega_1</eq></td><td>55</td><td>58</td><td>60</td></tr><tr><td><eq>\omega_2</eq></td><td>55</td><td>58</td><td>52</td></tr><tr><td><eq>\omega_3</eq></td><td>55</td><td>52</td><td>53</td></tr></table>

These price movements can be represented as a tree, see Figure 3.1. It is convenient to identify the scenarios with paths through the tree leading from the single node on the left (the ‘root’ of the tree) to the rightmost branch tips. 

Such a tree structure of price movements, if found realistic and desirable, can readily be implemented in a mathematical model. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/b70a7248efaae9923241af438204dfb592697072845359307ee7d00875600fc1.jpg)



Figure 3.1 Tree of price movements in Example 3.2


## Exercise 3.1

Sketch a tree representing the scenarios and price movements in Example 3.1. 

## Exercise 3.2

Suppose that the stock price on any given day can either be 5% higher or $4 \%$ lower than on the previous day. Sketch a tree representing possible stock price movements over the next three days, given that the price today is $20. How many diferent scenarios can be distinguished? 

## 3.1.1 Return

It proves convenient to describe the dynamics of stock prices $S ( n )$ in terms of returns. We assume that the stock pays no dividends. 

## Definition 3.1

The rate of return, or briefly the return $K ( n , m )$ over a time interval $[ n , m ]$ (in fact $[ m \tau , n \tau ] )$ , is defined to be the random variable 

$$
K (n, m) = \frac {S (m) - S (n)}{S (n)}.
$$

The return over a single time step $[ n - 1 , n ]$ will be denoted by $K ( n )$ , that is 

$$
K (n) = K (n - 1, n) = \frac {S (n) - S (n - 1)}{S (n - 1)},
$$

which implies that 

$$
S (n) = S (n - 1) (1 + K (n)).\tag{3.1}
$$

## Example 3.3

In the situation considered in Example 3.2 the returns are random variables taking the following values: 

<table><tr><td>Scenario</td><td><eq>K(1)</eq></td><td><eq>K(2)</eq></td></tr><tr><td><eq>\omega_{1}</eq></td><td>5.45%</td><td>3.45%</td></tr><tr><td><eq>\omega_{2}</eq></td><td>5.45%</td><td>-10.34%</td></tr><tr><td><eq>\omega_{3}</eq></td><td>-5.45%</td><td>1.92%</td></tr></table>

## Exercise 3.3

Given the following returns and assuming that S(0) = 45 dollars, find the possible stock prices in a three-step economy and sketch a tree of price movements: 

<table><tr><td>Scenario</td><td><eq>K(1)</eq></td><td><eq>K(2)</eq></td><td><eq>K(3)</eq></td></tr><tr><td><eq>\omega_1</eq></td><td>10%</td><td>5%</td><td>-10%</td></tr><tr><td><eq>\omega_2</eq></td><td>5%</td><td>10%</td><td>10%</td></tr><tr><td><eq>\omega_3</eq></td><td>5%</td><td>-10%</td><td>10%</td></tr></table>

## Remark 3.1

If the stock pays a dividend of div(n) at time n, then the definition of return has to be modified. Typically, when a dividend is paid, the stock price drops by that amount. Since the right to a dividend is decided prior to the payment day, the drop of stock price is already reflected in S(n). As a result, an investor who buys stock at time n 1 paying $S ( n - 1 )$ and wishes to sell the stock a time n will receive S(n) + div(n) and the return must reflect this: 

$$
K (n) = \frac {S (n) - S (n - 1) + \operatorname{div} (n)}{S (n - 1)}.
$$

## Exercise 3.4

Introduce the necessary modifications in Exercise 3.3 if a dividend of $1 is paid at the end of each time step. 

It is important to understand the relationship between one-step returns and the return over a longer time interval. 

## Example 3.4

Suppose that $S ( 0 ) = 1 0 0$ dollars. 

1. Consider a scenario in which $S ( 1 ) = 1 1 0$ and $S ( 2 ) = 1 0 0$ dollars. In this case $K ( 0 , 2 ) = 0 \%$ , while $K ( 1 ) = 1 0 \%$ and $K ( 2 ) \cong - 9 . 0 9 \%$ , the sum of the one-step returns K(1) and K(2) being positive and greater than K(0, 2). 

2. Consider another scenario with lower price $S ( 1 ) = 9 0 $ dollars and with $S ( 2 ) = 1 0 0 $ dollars as before. Then $K ( 1 ) = - 1 0 \%$ and $K ( 2 ) \cong 1 1 . 1 1 \%$ their sum being once again greater than $K ( 0 , 2 ) = 0 \%$ 

3. In a scenario such that S(1) = 110 and S(2) = 121 dollars we have $K ( 0 , 2 ) =$ 21%, which is greater than $K ( 1 ) + K ( 2 ) = 1 0 \% + 1 0 \% = 2 0 \%$ 

## Exercise 3.5

Find K(0, 2) and K(0, 3) for the data in Exercise 3.3 and compare the results with the sums of one-step returns $K ( 1 ) + K ( 2 )$ and $K ( 1 ) + K ( 2 ) +$ K(3), respectively. 

## Remark 3.2

The non-additivity of returns, already observed in Chapter 2 for deterministic returns, is worth pointing out, since it is common practice to compute the average of recorded past returns as a prediction for the future. This may result in misrepresenting the information, for example, overestimating the future return if the historical prices tend to fluctuate, or underestimating if they do not. 

## Proposition 3.1

The precise relationship between consecutive one-step returns and the return over the aggregate period is 

$$
1 + K (n, m) = (1 + K (n + 1)) (1 + K (n + 2)) \dots (1 + K (m)).
$$

## Proof

Compare the following two formulae for S(m): 

$$
S (m) = S (n) (1 + K (n, m))
$$

and 

$$
S (m) = S (n) (1 + K (n + 1)) (1 + K (n + 2)) \dots (1 + K (m)).
$$

Both of them follow from Definition 3.1. 

## Exercise 3.6

In each of the following three scenarios find the one-step returns, assuming that $K ( 1 ) = K ( 2 )$ : 

<table><tr><td>Scenario</td><td>S(0)</td><td>S(2)</td></tr><tr><td><eq>\omega_1</eq></td><td>35</td><td>41</td></tr><tr><td><eq>\omega_2</eq></td><td>35</td><td>32</td></tr><tr><td><eq>\omega_3</eq></td><td>35</td><td>28</td></tr></table>

## Exercise 3.7

Given that $K ( 1 ) = 1 0 \% \ \mathrm { o r } \ - 1 0 \%$ , and $K ( 0 , 2 ) = 2 1 \% , 1 0 \% \ \mathrm { { o r } \ - 1 \% }$ find a possible structure of scenarios such that K(2) takes at most two diferent values. 

The lack of additivity is often an inconvenience. This can be rectified by introducing the logarithmic return on a risky security, motivated by simila considerations for risk-free assets in Chapter 2. 

## Definition 3.2

The logarithmic return over a time interval $[ n , m ]$ (more precisely, $[ \tau n , \tau m ] )$ is a random variable $k ( n , m )$ defined by 

$$
k (n, m) = \ln {\frac {S (m)}{S (n)}}.
$$

The one-step logarithmic return will be denoted simply by $k ( n )$ , that is, 

$$
k (n) = k (n - 1, n) = \ln {\frac {S (n)}{S (n - 1)}},
$$

so that 

$$
S (n) = S (n - 1) \mathrm{e} ^ {k (n)}.\tag{3.2}
$$

The relationship between the return $K ( m , n )$ and the logarithmic return $k ( m , n )$ is obvious by comparing their definitions, namely 

$$
1 + K (m, n) = \mathrm{e} ^ {k (m, n)}.
$$

Because of this we can readily switch from one return to the other. 

## Remark 3.3

If the stock pays a dividend of div(n) at time n and this is reflected in the price S(n), then the following version of the logarithmic return should be used: 

$$
k (n) = \ln {\frac {S (n) + \operatorname{div} (n)}{S (n - 1)}}.
$$

Consecutive one-step logarithmic returns can be combined in an additive manner to find the return during the overall time period. 

## Exercise 3.8

For the data in Example 3.2 find the random variables k(1), k(2) and k(0, 2). Compare k(0, 2) with $k ( 1 ) + k ( 2 )$ 

## Proposition 3.2

If no dividends are paid, then 

$$
k (n, m) = k (n + 1) + k (n + 2) + \dots + k (m).
$$

## Proof

On the one hand, 

$$
S (m) = S (n) \mathrm{e} ^ {k (n, m)}
$$

by the definition of the logarithmic return. On the other hand, using one-step logarithmic returns repeatedly, we obtain, 

$$
S (m) = S (n) \mathrm{e} ^ {k (n + 1)} \mathrm{e} ^ {k (n + 2)} \dots \mathrm{e} ^ {k (m)} = S (n) \mathrm{e} ^ {k (n + 1) + k (n + 2) + \dots + k (m)}.
$$

The result follows by comparing these two expressions. 

## 3.1.2 Expected Return

Suppose that the probability distribution of the return K over a certain time period is known. Then we can compute the mathematical expectation $E ( K )$ , called the expected return. 

## Example 3.5

We estimate the probabilities of recession, stagnation and boom to be 1/4, 1/2, 1/4, respectively. If the predicted annual returns on some stock in these scenarios are $- 6 \% , 4 \% , 3 0 \%$ , respectively, then the expected annual return is 

$$
- 6 \% \times \frac {1}{4} + 4 \% \times \frac {1}{2} + 30 \% \times \frac {1}{4} = 8 \%.
$$

## Exercise 3.9

With the probabilities of recession, stagnation and boom equal to $1 / 2$ $1 / 4 , 1 / 4$ and the predicted annual returns in the first two of these scenarios at $- 5 \%$ and $6 \%$ , respectively, find the annual return in the remaining scenario if the expected annual return is known to be $6 \%$ 

## Exercise 3.10

Suppose that the stock prices in the following three scenarios are 

<table><tr><td>Scenario</td><td><eq>S(0)</eq></td><td><eq>S(1)</eq></td><td><eq>S(2)</eq></td></tr><tr><td><eq>\omega_1</eq></td><td>100</td><td>110</td><td>120</td></tr><tr><td><eq>\omega_2</eq></td><td>100</td><td>105</td><td>100</td></tr><tr><td><eq>\omega_3</eq></td><td>100</td><td>90</td><td>100</td></tr></table>

with probabilities $1 / 4 , 1 / 4 , 1 / 2$ , respectively. Find the expected returns $E ( K ( 1 ) ) , E ( K ( 2 ) )$ and $E ( K ( 0 , 2 ) )$ ). Compare $1 + E ( K ( 0 , 2 ) )$ ) with $( 1 +$ $E ( K ( 1 ) ) ) ( 1 + E ( K ( 2 ) ) )$ 

The last exercise shows that the relation established in Proposition 3.1 doe not extend to expected returns. For that we need an additional assumption. 

## Proposition 3.3

If the one-step returns $K ( n + 1 ) , \ldots , K ( m )$ are independent, then 

$$
1 + E (K (n, m)) = (1 + E (K (n + 1))) (1 + E (K (n + 2))) \dots (1 + E (K (m))).
$$

## Proof

This is an immediate consequence of Proposition 3.1 and the fact that the expectation of a product of independent random variables is the product of expectations. (Note that if the $K ( i )$ are independent, then so are the random variables $1 + K ( i )$ for $i = n + 1 , \ldots , m . )$ □ 

## Exercise 3.11

Suppose that the time step is taken to be three months, $\tau = 1 / 4$ , and the quarterly returns K(1), K(2), K(3), K(4) are independent and identically distributed. Find the expected quarterly return $E ( K ( 1 ) )$ and the expected annual return $E ( K ( 0 , 4 ) )$ if the expected return $E ( K ( 0 , 3 ) )$ 1 over three quarters is 12%. 

## Remark 3.4

In the case of logarithmic returns additivity extends to expected returns, even if the one-step returns are not independent. Namely 

$$
E (k (n, m)) = E (k (n + 1)) + E (k (n + 2)) + \dots + E (k (m)).
$$

This is because the expectation of a sum of random variables is the sum of expectations. 

## Remark 3.5

In practice it is dificult to estimate the probabilities and returns in each scenario, needed to compute the expected return. What can readily be computed is the average return over a past period. The result can be used as an estimate for the expected future return. For example, if the stock prices on the last 10 consecutive days were $98, $100, $99, $95, $88, $82, $89, $98, $101, $105, then the average of the resulting nine daily returns would be about 0.77%. However, the average of the last four daily returns would be about 6.18%. (We use log arithmic returns because of their additivity.) This shows that the result may depend heavily on the choice of data. Using historical prices for prediction is a complex statistical issue belonging to Econometrics, which is beyond the scope of this book. 

## 3.2 Binomial Tree Model

We shall discuss an extremely important model of stock prices. On the one hand, the model is easily tractable mathematically because it involves a small number of parameters and assumes an identical simple structure at each node of the tree of stock prices. On the other hand, it captures surprisingly many features of real-world markets. 

The model is defined by the following conditions. 

## Condition 3.1

The one-step returns $K ( n )$ on stock are identically distributed independen random variables such that 

$$
K (n) = \left\{ \begin{array}{l l} u & \text { with   probability } p, \\ d & \text { with   probability } 1 - p, \end{array} \right.
$$

at each time step n, where $- 1 < d < u { \mathrm { ~ a n d ~ } } 0 < p < 1$ 

This condition implies that the stock price $S ( n )$ can move up or down by a factor 1 + u or 1 + d at each time step. The inequalities $- 1 < d < u$ guarantee that all prices $S ( n )$ will be positive if $S ( 0 )$ is. 

Let r be the return on a risk-free investment over a single time step of length $\tau .$ . 

## Condition 3.2

The one-step return r on a risk-free investment is the same at each time step and 

$$
d <   r <   u.
$$

The last condition describes the movements of stock prices in relation to risk-free assets such as bonds or cash held in a bank account. The inequalities $d < r <$ u are justified because of Proposition 1.1 in Chapter 1 (which will be generalised in Proposition 4.2). 

Since $S ( 1 ) / S ( 0 ) = 1 + K ( 1 )$ , Condition 3.1 implies that the random variable $S ( 1 )$ can take two diferent values, 

$$
S (1) = \left\{ \begin{array}{l l} S (0) (1 + u) & \text { with   probability } p, \\ S (0) (1 + d) & \text { with   probability } 1 - p. \end{array} \right.
$$

## Exercise 3.12

How many diferent values do the random variables $S ( 2 )$ and $S ( 3 )$ take? What are these values and the corresponding probabilities? 

The values of $S ( n )$ along with the corresponding probabilities can be found for any n by extending the solution to Exercise 3.12. In an n-step tree of stock prices each scenario (or path through the tree) with exactly i upward and $n - i$ downward price movements produces the same stock price $S ( 0 ) ( 1 + u ) ^ { i } ( 1 +$ $d ) ^ { n - i }$ at time n. There are $\binom { n } { i }$ such scenarios, the probability of each equal to $p ^ { i } ( 1 - p ) ^ { n - i }$ . As a result, 

$$
S (n) = S (0) (1 + u) ^ {i} (1 + d) ^ {n - i} \text { with   probability } \binom {n} {i} p ^ {i} (1 - p) ^ {n - i}\tag{3.3}
$$

for $i = 0 , 1 , \ldots , n$ . The stock price $S ( n )$ at time n is a discrete random variable with $n + 1$ diferent values. The distribution of $S ( n )$ as given by (3.3) is shown in Figure 3.2 for $n = 1 0 , p = 0 . 5 , S ( 0 ) = 1 , u = 0 . 1$ and $d = - 0 . 1$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/6046c1833aac619c3122e24673c3adfa76337b5e479e3b1a5857f6928878e1dc.jpg)



Figure 3.2 Distribution of S(10)


The number i of upward price movements is a random variable with a binomial distribution. The same is true for the number $n - i$ of downward movements. We therefore say that the price process follows a binomial tree. In an n-step binomial three the set $\varOmega$ of all scenarios, that is, n-step paths moving up or down at each step has $2 ^ { n }$ elements. An example of a two-step binomial tree of stock prices is shown in Figure 3.3 and a three-step tree in Figure 3.4. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/b1827c8264f2ae87d411f7175cb7ab2d5e9e23f4c04f1b670f7f34a276f2c5a2.jpg)



Figure 3.3 Two-step binomial tree of stock prices


In both figures $S ( 0 ) = 1$ for simplicity. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/7f50779d9ef4a722daabb0d07db8effdf55db50aa1b4786bb788d96f5b90f0ca.jpg)



Figure 3.4 Three-step binomial tree of stock prices


## Exercise 3.13

Find d and u if S(1) can take two values, $87 or $76, and the top possible value of S(2) is $92. 

## Exercise 3.14

Suppose that the risk-free rate under continuous compounding is 14%, the time step $\tau$ is one month, $S ( 0 ) = 2 2 $ dollars and $d = - 0 . 0 1$ . Find the bounds on the middle value of S(2) consistent with Condition 3.2. 

## Exercise 3.15

Suppose that $32, $28 and x are the possible values of $S ( 2 )$ . Find $x ,$ assuming that stock prices follow a binomial tree. Can you complete the tree? Can this be done uniquely? 

## Exercise 3.16

Suppose that stock prices follow a binomial tree, the possible values of S(2) being $121, $110 and $100. Find u and d when S(0) = 100 dollars. Do the same when $S ( 0 ) = 1 0 4$ dollars. 

## 3.2.1 Risk-Neutral Probability

While the future value of stock can never be known with certainty, it is possible to work out expected stock prices within the binomial tree model. It is then natural to compare these expected prices and risk-free investments. This simple idea will lead us towards powerful and surprising applications in the theory of derivative securities (for example, options, forwards, futures), to be studied in 

later chapters. 

To begin with, we shall work out the dynamics of expected stock prices $E ( S ( n ) )$ . For $n = 1$ 

$$
E (S (1)) = p S (0) (1 + u) + (1 - p) S (0) (1 + d) = S (0) (1 + E (K (1))),
$$

where 

$$
E (K (1)) = p u + (1 - p) d
$$

is the expected one-step return. This extends to any n as follows. 

## Proposition 3.4

The expected stock prices for $n = 0 , 1 , 2 , \ldots$ . are given by 

$$
E (S (n)) = S (0) (1 + E (K (1))) ^ {n}.
$$

Proof 

Since the one-step returns $K ( 1 ) , K ( 2 ) , \ldots$ . are independent, so are the random variables $1 + K ( 1 ) , 1 + K ( 2 ) , \ldots$ . It follows that 

$$
\begin{array}{r l} & E (S (n)) = E (S (0) (1 + K (1)) (1 + K (2)) \dots (1 + K (n))) \\ & \quad = S (0) E (1 + K (1)) E (1 + K (2)) \dots E (1 + K (n)) \\ & \quad = S (0) (1 + E (K (1))) (1 + E (K (2))) \dots (1 + E (K (n))). \end{array}
$$

Because the $K ( n )$ are identically distributed, they all have the same expectation, 

$$
E (K (1)) = E (K (2)) = \dots = E (K (n)),
$$

which proves the formula for $E ( S ( n ) )$ 

If the amount $S ( 0 )$ were to be invested risk-free at time 0, it would grow to $S ( 0 ) ( 1 + r ) ^ { n }$ after n steps. Clearly, to compare $E ( S ( n ) )$ and $S ( 0 ) ( 1 + r ) ^ { n }$ we only need to compare $E ( K ( 1 ) )$ and r. 

An investment in stock always involves an element of risk, simply because the price $S ( n )$ is unknown in advance. A typical risk-averse investor will require that $E ( K ( 1 ) ) > r ;$ , arguing that he or she should be rewarded with a higher expected return as a compensation for risk. The reverse situation when $E ( K ( 1 ) ) < r$ may nevertheless be attractive to some investors if the risky re turn is high with small non-zero probability and low with large probability. (A typical example is a lottery, where the expected return is negative.) An investor of this kind can be called a risk-seeker. We shall return to this topic in Chapter $5 ,$ , where a precise definition of risk will be developed. The borde case of a market in which $E ( K ( 1 ) ) = r$ is referred to as risk-neutral. 

It proves convenient to introduce a special symbol $p _ { * }$ for the probability as well as $E _ { * }$ for the corresponding expectation satisfying the condition 

$$
E _ {*} (K (1)) = p _ {*} u + (1 - p _ {*}) d = r\tag{3.4}
$$

for risk-neutrality, which implies that 

$$
p _ {*} = \frac {r - d}{u - d}.
$$

We shall call $p _ { * }$ the risk-neutral probability and $E _ { * }$ the risk-neutral expectation. It is important to understand that $p _ { * }$ is an abstract mathematical object, which may or may not be equal to the actual market probability $p .$ Only in a risk-neutral market do we have $p = p _ { * }$ . Even though the risk-neutral probabil ity $p _ { * }$ may have no relation to the actual probability $p ,$ it turns out that for the purpose of valuation of derivative securities the relevant probability is $p _ { * }$ rather than $p .$ . This application of the risk-neutral probability, which is of great practical importance, will be discussed in detail in Chapter 8. 

## Exercise 3.17

Let $u = 2 / 1 0$ and $r = 1 / 1 0$ . Investigate the properties of $p _ { * }$ as a function of d. 

Exercise 3.18 

Show that $d < r < u$ if and only if $0 < p _ { * } < 1$ 

Condition (3.4) implies that 

$$
p _ {*} (u - r) + (1 - p _ {*}) (d - r) = 0.
$$

Geometrically, this means that the pair $( p _ { * } , 1 - p _ { * } )$ regarded as a vector on the plane $\mathbb { R } ^ { 2 }$ is orthogonal to the vector with coordinates $( u - r , d - r )$ , which represents the possible one-step gains (or losses) of an investor holding a single share of stock, the purchase of which was financed by a cash loan attracting interest at a rate $r ,$ see Figure 3.5. The line joining the points (1, 0) and (0, 1) consists of all points with coordinates $( p , 1 - p )$ , where $0 < p < 1$ . One of these points corresponds to the actual market probability and one to the risk-neutral probability. 

Another interpretation of condition (3.4) for the risk-neutral probability is illustrated in Figure 3.6. If masses $p _ { * }$ and $1 - p _ { * }$ are attached at the points with coordinates u and d on the real axis, then the centre of mass will be at $r .$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/13949893f1bef1c7395805f6183bf0392ae26f1105c9997485816db922b0346e.jpg)



Figure 3.5 Geometric interpretation of risk-neutral probability $p _ { * }$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/65f1abbdfe5d5a795877a58c90f7fff3a86f03376977ca1bdfec430707369572.jpg)



Figure 3.6 Barycentric interpretation of risk-neutral probability $p _ { * }$


## 3.2.2 Martingale Property

By Proposition 3.4 the expectation of $S ( n )$ with respect to the risk-neutral probability $p _ { * }$ is 

$$
E _ {*} (S (n)) = S (0) (1 + r) ^ {n},\tag{3.5}
$$

since $r = E _ { * } ( K ( 1 ) )$ 

## Example 3.6

Consider a two-step binomial tree model such that $S ( 0 ) = 1 0 0$ dollars, $u = 0 . 2$ 2 $d = - 0 . 1$ and $r = 0 . 1$ . Then $p _ { * } = 2 / 3$ is the risk-neutral probability, and the expected stock price after two steps is 

$$
E _ {*} (S (2)) = S (0) (1 + r) ^ {2} = 1 2 1
$$

dollars. After one time step, once it becomes known whether the stock price has gone up or down, we shall need to recompute the expectation of $S ( 2 )$ . Suppose that the stock price has gone up to $120 after the first step. In these circum stances the set of possible scenarios reduces to those for which $S ( 1 ) = 1 2 0$ dollars, and the tree of stock prices reduces to the subtree in Figure 3.7. Given that $S ( 1 ) = 1 2 0$ dollars, the risk-neutral expectation of $S ( 2 )$ will therefore be ${ \begin{array} { l } { { \frac { 2 } { 3 } } \times 1 4 4 + { \frac { 1 } { 3 } } \times 1 0 8 = 1 3 2 } \end{array} }$ dollars, which is equal to $1 2 0 ( 1 + r )$ . Formally, this can be written using the conditional expectation<sup>1</sup> of S(2) given that $S ( 1 ) = 1 2 0$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/1b3a14d7880c5b566e9c8f74f0bdd4c42ab747f67bf2c3518181ba3f6158d529.jpg)



Figure 3.7 Subtree such that $S ( 1 ) = 1 2 0$ dollars


$$
E _ {*} (S (2) | S (1) = 1 2 0) = 1 2 0 (1 + r).
$$

Similarly, if the stock price drops to $90 after one time step, the set of possible scenarios will reduce to those for which $S ( 1 ) = 9 0 $ dollars, and the tree of stock prices will reduce to the subtree in Figure 3.8. Given that $S ( 1 ) = 9 0 $ dollars, 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/773d92025e6ad22681dc1a9b45a398168dfab3b9637e975c65649d20bee7c630.jpg)



Figure 3.8 Subtree such that $S ( 1 ) = 9 0 $ dollars


the risk-neutral expectation of $S ( 2 )$ will be ${ \frac { 2 } { 3 } } \times 1 0 8 + { \frac { 1 } { 3 } } \times 8 1 = 9 9$ dollars, which is equal to $9 0 ( 1 + r )$ . This can be written as 

$$
E _ {*} (S (2) | S (1) = 9 0) = 9 0 (1 + r).
$$

The last two formulae involving conditional expectation can be written as a single equality, properly understood: 

$$
E _ {*} (S (2) | S (1)) = S (1) (1 + r).
$$

This analysis can be extended to any time step in the binomial tree model. Suppose that n time steps have passed and the stock price has become $S ( n )$ What is the risk-neutral expectation of the price $S ( n + 1 )$ after one more step? 

## Proposition 3.5

Given that the stock price $S ( n )$ has become known at time n, the risk-neutral conditional expectation of $S ( n + 1 )$ will be 

$$
E _ {*} (S (n + 1) | S (n)) = S (n) (1 + r).
$$

## Proof

Suppose that $S ( n ) = x$ after n time steps. Then 

$$
E _ {*} (S (n + 1) | S (n) = x) = p _ {*} x (1 + u) + (1 - p _ {*}) x (1 + d)
$$

because $S ( n + 1 )$ takes the value $x ( 1 + u )$ with probability $p _ { * }$ and $x ( 1 + d )$ with probability $1 - p _ { * }$ . But $p _ { * } ( 1 + u ) + ( 1 - p _ { * } ) ( 1 + d ) = 1 + r$ by (3.4), which implies that 

$$
E _ {*} (S (n + 1) | S (n) = x) = x (1 + r)
$$

for any possible value x of $S ( n )$ , completing the proof. 

Dividing both sides of the equality in Proposition 3.5 by $( 1 + r ) ^ { n + 1 }$ , we obtain the following important result for the discounted stock prices $\widetilde { S } ( n ) =$ $S ( n ) \left( 1 + r \right) ^ { - n }$ 

## Corollary 3.6 (Martingale Property)

For any $n = 0 , 1 , 2 , \ldots$ 

$$
E _ {*} (\widetilde {S} (n + 1) | S (n)) = \widetilde {S} (n).
$$

We say that the discounted stock prices $\widetilde { S } ( n )$ form a martingale under the risk-neutral probability $p _ { * }$ . The probability $p _ { * }$ itself is also referred to as the martingale probability. 

Exercise 3.19 

Let $r = 0 . 2$ . Find the risk-neutral conditional expectation of $S ( 3 )$ given that $S ( 2 ) = 1 1 0$ dollars. 

## 3.3 Other Models

This section may be skipped at first reading because the main ideas to follow later do not depend on the models presented here. 

## 3.3.1 Trinomial Tree Model

A natural generalisation of the binomial tree model extends the range of possible values of the one-step returns $K ( n )$ to three. The idea is to allow the price not only to move up or down, but also to take an intermediate value at any given step. 

## Condition 3.3

The one-step returns $K ( n )$ are independent random variables of the form 

$$
K (n) = \left\{ \begin{array}{l l} u & \text {with probability p}, \\ n & \text {with probability q}, \\ d & \text {with probability 1 - p - q}, \end{array} \right.
$$

where $d < n < u$ and $0 < p , q , p + q < 1$ 

This means that u and d represent upward and downward price movements, as before, whereas n stands for the middle price movement, typically a neutral one, $n = 0$ 

## Condition 3.4

The one-step return r on a risk-free investment is the same at each time step and 

$$
d <   r <   u.
$$

Since $S ( 1 ) / S ( 0 ) = 1 + K ( 1 )$ , Condition 3.3 implies that $S ( 1 )$ takes three diferent values, 

$$
S (1) = \left\{ \begin{array}{l l} S (0) (1 + u) & \text {with probability p}, \\ S (0) (1 + n) & \text {with probability q}, \\ S (0) (1 + d) & \text {with probability 1 - p - q}. \end{array} \right.
$$

## Exercise 3.20

How many diferent values does the random variable $S ( 2 )$ take? What are these values and the corresponding probabilities? 

The condition $E _ { * } ( K ( n ) ) ~ = ~ r$ for risk-neutral probabilities $p _ { * } , q _ { * }$ can be written as 

$$
p _ {*} (u - r) + q _ {*} (n - r) + (1 - p _ {*} - q _ {*}) (d - r) = 0.\tag{3.6}
$$

The triple $( p _ { * } , q _ { * } , 1 - p _ { * } - q _ { * } )$ regarded as a vector in $\mathbb { R } ^ { 3 }$ is orthogonal to the vector with coordinates $( u - r , n - r , d - r )$ representing the possible one-step gains (or losses) of an investor holding a singe share of stock, the purchase of which was financed by a cash loan. This means that $( p _ { * } , q _ { * } , 1 - p _ { * } - q _ { * } )$ lies on the intersection of the triangle $\left\{ ( a , b , c ) : a , b , c \geq 0 , a + b + c = 1 \right\}$ and the plane orthogonal to the gains vector $( u - r , n - r , d - r )$ , as in Figure 3.9. Condition 3.4 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/ce0c19c8651aa3c9ea638edf30c560dcca1ebe8ac973e7552ed2bad448ac4387.jpg)



Figure 3.9 Geometric interpretation of risk-neutral probabilities $p _ { * } , q _ { * }$


guarantees that the intersection is non-empty, since the line containing the vector $( u - r , n - r , d - r )$ does not pass through the positive octant. In this case there are infinitely many risk-neutral probabilities, the intersection being a line segment. 

Another interpretation of condition (3.6) for the risk-neutral probability is illustrated in Figure 3.10. If masses $p _ { * } , \ q _ { * }$ and $1 - p _ { * } - q _ { * }$ are attached at the points with coordinates u, n and d on the real axis, then the centre of mass will be at r. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/185a19079f58ce09d641114c84f1a935c8a9fb018e9afcbdca6d1546b798ca3b.jpg)



Figure 3.10 Barycentric interpretation of risk-neutral probabilitie $p _ { * } , q _ { * }$


Exercise 3.21 

Let $u = 0 . 2 , n = 0 , d = - 0 . 1$ , and $r = 0$ . Find all risk-neutral probabili ties. 

## 3.3.2 Continuous-Time Limit

Discrete-time and discrete-price models have apparent disadvantages. They clearly restrict the range of asset price movements as well as the set of time instants at which these movements may occur. In this section we shall outline an approach free from such restrictions. It will be obtained by passing to the continuous-time limit from the binomial tree model. 

We shall consider a sequence of binomial tree models with time step $\textstyle { \tau = { \frac { 1 } { N } } }$ letting $N \to \infty$ . For all binomial tree models in the approximating sequence it will be assumed that the probability of upward and downward price movements is $\textstyle { \frac { 1 } { 2 } }$ in each step. 

In this context it proves convenient to use the logarithmic return 

$$
k (n) = \ln (1 + K (n)) = \left\{ \begin{array}{l l} \ln (1 + u) & \text { with   probability } 1 / 2, \\ \ln (1 + d) & \text { with   probability } 1 / 2. \end{array} \right.
$$

In place of the risk-free rate of return over one time step, we shall use the equivalent continuous compounding rate r, so that the return over a time step of length $\tau$ will be $\mathrm { e } ^ { \tau r }$ 

We denote by m the expectation and by $\sigma$ the standard deviation of the logarithmic return $k ( 1 ) { + } k ( 2 ) { + } { \cdot } \cdot { + } k ( N )$ over the unit time interval from 0 to 1, consisting of N steps of τ. The logarithmic returnslength $k ( 1 ) , k ( 2 ) , \ldots , k ( N )$ are identically distributed and independent, just as $K ( 1 ) , K ( 2 ) , \ldots , K ( N )$ are. It follows that 

$$
\begin{array}{r l} & m = E \left(k (1) + k (2) + \dots + k (N)\right) \\ & \quad = E (k (1)) + E (k (2)) + \dots + E (k (N)) = N E (k (n)), \\ & \sigma^ {2} = \mathrm{Var} \left(k (1) + k (2) + \dots + k (N)\right) \\ & \quad = \mathrm{Var} \left(k (1)\right) + \mathrm{Var} \left(k (2)\right) + \dots + \mathrm{Var} \left(k (N)\right) = N \mathrm{Var} \left(k (n)\right) \end{array}
$$

for each $n = 1 , 2 , \ldots , N$ . This means that each $k ( n )$ has expectation $\textstyle { \frac { m } { N } } = m \tau$ and standard deviation $\begin{array} { r } { \sqrt { \frac { \sigma ^ { 2 } } { N } } = \sigma \sqrt { \tau } } \end{array}$ , so the two possible values of each $k ( n )$ must be 

$$
\begin{array}{l} \ln (1 + u) = m \tau + \sigma \sqrt {\tau}, \\ \ln (1 + d) = m \tau - \sigma \sqrt {\tau}. \end{array}\tag{3.7}
$$

Exercise 3.22 

Find m and $\sigma$ for $u = 0 . 0 2 , d = - 0 . 0 1 \ \mathrm { a n d } \ \tau = 1 / 1 2$ 

Introducing a sequence of independent random variables $\xi ( n )$ , each with two values 

$$
\xi (n) = \left\{ \begin{array}{l l} + \sqrt {\tau} & \text {with probability 1 / 2}, \\ - \sqrt {\tau} & \text {with probability 1 / 2}, \end{array} \right.
$$

we can write the logarithmic return as 

$$
k (n) = m \tau + \sigma \xi (n).
$$

## Exercise 3.23

Find the expectation and variance of $\xi ( n )$ and $k ( n )$ 

## Exercise 3.24

Write S(1) and S(2) in terms of $m , \sigma , \tau , \xi ( 1 )$ and $\xi ( 2 )$ 

Next, we introduce an important sequence of random variables $w ( n )$ , called a symmetric random walk, such that 

$$
w (n) = \xi (1) + \xi (2) + \dots + \xi (n),
$$

and $w ( 0 ) = 0$ . Clearly, $\xi ( n ) = w ( n ) - w ( n - 1 )$ . Because of the last equality, the $\xi ( n )$ are referred to as the increments of $w ( n )$ 

From now on we shall often write $S ( t )$ and $w ( t )$ instead of $S ( n )$ and $w ( n )$ for $t = \tau n$ , where $n = 1 , 2 , \ldots$ 

## Proposition 3.7

The stock price at time $t = \tau n$ is given by 

$$
S (t) = S (0) \exp (m t + \sigma w (t)).
$$

Proof 

By (3.2) 

$$
\begin{array}{r l} & S (t) = S (n \tau) = S (n \tau - \tau) \mathrm{e} ^ {k (n)} \\ & \quad = S (n \tau - 2 \tau) \mathrm{e} ^ {k (n - 1) + k (n)} \\ & \quad = \dots = S (0) \mathrm{e} ^ {k (1) + \dots + k (n)} \\ & \quad = S (0) \mathrm{e} ^ {m n \tau + \sigma (\xi (1) + \dots + \xi (n))} \\ & \quad = S (0) \mathrm{e} ^ {m t + \sigma w (t)}, \end{array}
$$

as required. 

In order to pass to the continuous-time limit we use the approximation 

$$
\mathrm{e} ^ {x} \approx 1 + x + \frac {1}{2} x ^ {2},
$$

accurate for small values of x, to obtain 

$$
\frac {S (n \tau + \tau)}{S (n \tau)} = \mathrm{e} ^ {k (n + 1)} \approx 1 + k (n + 1) + \frac {1}{2} k (n + 1) ^ {2}.
$$

Then, we compute 

$$
k (n + 1) ^ {2} = (m \tau + \sigma \xi (n + 1)) ^ {2} = \sigma^ {2} \tau + \dots ,
$$

where the dots represent all terms with powers of $\tau$ higher than 1, which will be omitted because they are much smaller than the leading term whenever $\tau$ is small. Next, 

$$
\begin{array}{c} \frac {S (n \tau + \tau)}{S (n \tau)} \approx 1 + m \tau + \sigma \xi (n + 1) + \frac {1}{2} \sigma^ {2} \tau \\ = 1 + \left(m + \frac {1}{2} \sigma^ {2}\right) \tau + \sigma \xi (n + 1), \end{array}
$$

and so 

$$
S (n \tau + \tau) - S (n \tau) \approx \left(m + \frac {1}{2} \sigma^ {2}\right) S (n \tau) \tau + \sigma S (n \tau) \xi (n + 1).
$$

Since $\xi ( n + 1 ) = w ( n \tau + \tau ) - w ( n \tau )$ , we obtain an approximate equation describing the dynamics of stock prices: 

$$
S (t + \tau) - S (t) \approx \left(m + \frac {1}{2} \sigma^ {2}\right) S (t) \tau + \sigma S (t) (w (t + \tau) - w (t)),\tag{3.8}
$$

where $t = n \tau$ . The solution $S ( t )$ of this approximate equation is given by the same formula as in Proposition 3.7. 

For any $N = 1 , 2 , . . .$ . we consider a binomial tree model with time step of length $\textstyle \tau = { \frac { 1 } { N } }$ . Let $S _ { N } ( t )$ be the corresponding stock prices and let $w _ { N } ( t )$ be the corresponding symmetric random walk with increments $\xi _ { N } ( t ) = w _ { N } ( t ) -$ $\begin{array} { r } { w _ { N } ( t - \frac { 1 } { N } ) } \end{array}$ , where $\begin{array} { r } { t = \frac { n } { N } } \end{array}$ is the time after n steps. 

Exercise 3.25 

Compute the expectation and variance of $w _ { N } ( t )$ , where $\begin{array} { r } { t = \frac { n } { N } } \end{array}$ 

We shall use the Central Limit Theorem<sup>2</sup> to obtain the limit as $N \to \infty$ of the random walk $w _ { N } ( t )$ . To this end we put 

$$
x (n) = \frac {k (n) - m \tau}{\sigma \sqrt {\tau}}
$$

for each $n = 1 , 2 , \ldots$ , which is a sequence of independent identically distributed random variables, each with expectation 0 and variance 1. The Central Limi Theorem implies that 

$$
\frac {x (1) + x (2) + \cdots + x (n)}{\sqrt {n}} \rightarrow X
$$

in distribution as $n \to \infty$ , where X is a random variable with standard normal distribution (mean 0 and variance 1). 

Let us fix any $t > 0$ . Because the random walk $w _ { N }$ is only defined at discrete times being whole multiples of the step $\textstyle { \tau = { \frac { 1 } { N } } }$ , we consider $w _ { N } ( t _ { N } )$ , where $t _ { N }$ is the whole multiple of $\textstyle { \frac { 1 } { N } }$ nearest to t. Then, clearly, $N t _ { N }$ is a whole number for each N, and we can write 

$$
w _ {N} (t _ {N}) = \sqrt {t _ {N}} \frac {x (1) + x (2) + \cdots + x (N t _ {N})}{\sqrt {N t _ {N}}}.
$$

As $N \to \infty$ , we have $t _ { N } \to t$ and $N t _ { N }  \infty$ , so that 

$$
w _ {N} (t _ {N}) \rightarrow W (t)
$$

in distribution, where $W ( t ) ~ = ~ \sqrt { t } X$ . The last equality means that $W ( t )$ is normally distributed with mean 0 and variance t. 

This argument, based on the Central Limit Theorem, works for any single fixed time $t > 0$ . It is possible to extend the result to obtain a limit for all times $t \geq 0$ simultaneously, but this is beyond the scope of this book. The limit $W ( t )$ is called the Wiener process (or Brownian motion). It inherits many of the properties of the random walk, for example: 

1. $W ( 0 ) = 0 \quad$ , which corresponds to $w _ { N } ( 0 ) = 0$ 

2. $E ( W ( t ) ) = 0$ , corresponding to $E ( w _ { N } ( t ) ) = 0$ (see the solution of Exercise 3.25). 

3. Var $( W ( t ) ) = t ,$ , with the discrete counterpart $\mathrm { V a r } ( w _ { N } ( t ) ) = t$ (see the solu tion of Exercise 3.25). 

4. The increments $W ( t _ { 3 } ) - W ( t _ { 2 } )$ and $W ( t _ { 2 } ) - W ( t _ { 1 } )$ are independent for $0 \leq$ $t _ { 1 } \leq t _ { 2 } \leq t _ { 3 } ;$ so are the increments $w _ { N } ( t _ { 3 } ) - w _ { N } ( t _ { 2 } )$ and $w _ { N } ( t _ { 2 } ) - w _ { N } ( t _ { 1 } )$ 

5. $W ( t )$ has a normal distribution with mean 0 and variance t, that is, with density $\textstyle { \frac { 1 } { \sqrt { 2 \pi t } } } \mathrm { e } ^ { - { \frac { x ^ { 2 } } { 2 t } } }$ . This is related to the distribution of $w _ { N } ( t )$ . The latter is not normal, but approaches the normal distribution in the limit according to the Central Limit Theorem. 

An important diference between $W ( t )$ and $w _ { N } ( t )$ is that $W ( t )$ is defined for all $t \geq 0$ , whereas the time in $w _ { N } ( t )$ is discrete, $t = n / N$ for $n = 0 , 1 , 2 , \ldots$ 

The price process obtained in the limit from $S _ { N } ( t )$ as $N  \infty$ will be denoted by $S ( t )$ . While $S _ { N } ( t )$ satisfies the approximate equation (3.8) with the appropriate substitutions, namely 

$$
S _ {N} (t + \frac {1}{N}) - S _ {N} (t) \approx \left(m + \frac {1}{2} \sigma^ {2}\right) S _ {N} (t) \frac {1}{N} + \sigma S _ {N} (t) (w _ {N} (t + \frac {1}{N}) - w _ {N} (t)),
$$

the continuous-time stock prices $S ( t )$ satisfy an equation of the form 

$$
\mathrm{d} S (t) = \left(m + \frac {1}{2} \sigma^ {2}\right) S (t) \mathrm{d} t + \sigma S (t) \mathrm{d} W (t).\tag{3.9}
$$

Here d $S ( t ) = S ( t { + } \mathrm { d } t ) - S ( t )$ and $\mathrm { d } W ( t ) = W ( t + \mathrm { d } t ) - W ( t )$ are the increments of $S ( t )$ and $W ( t )$ over an infinitesimal time interval dt. The explicit formulae for the solutions are also similar, 

$$
S _ {N} (t) = S _ {N} (0) \exp (m t + \sigma w _ {N} (t))
$$

in the discrete case, whereas 

$$
S (t) = S (0) \exp (m t + \sigma W (t))
$$

in the continuous case. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/782f9b3afdd887fefb77ab33debb5eb04783282590b864359cab03f15fb2f89b.jpg)



Figure 3.11 Density of the distribution of $S ( 1 0 )$


Since $W ( t )$ has a normal distribution with mean 0 and variance t, it follows that ln $S ( t )$ has a normal distribution with mean ln $S ( 0 ) + m t$ and variance $\sigma ^ { 2 } t$ Because of this it is said that the continuous-time price process $S ( t )$ has the log normal distribution. The number $\sigma$ is called the volatility of the price $S ( t )$ . The density of the distribution of S(t) is shown in Figure 3.11 for $t = 1 0 , S ( 0 ) = 1$ , $m = 0$ and $\sigma = 0 . 1$ . This can be compared with the discrete distribution in Figure 3.2. 

## Remark 3.6

Equation (3.9) and the increments dS(t), dW(t) and dt are introduced above only informally by analogy with the discrete case. They can be given a precise status in Stochastic Calculus, a theory with fundamental applications in advanced mathematical finance. In particular, (3.9) is an example of what is known as a stochastic diferential equation. 

This page intentionally left blank 

# Discrete Time Market Models

Having discussed a number of diferent models of stock price dynamics, we shall now generalise and pursue a little further some of the ideas introduced in Chapter 1. In particular, we shall reformulate and extend the general notions and assumptions underlying mathematical finance already mentioned in that chapter. 

As in Chapter 3, we assume that time runs in steps of fixed length $\tau .$ . For many time-dependent quantities we shall simplify the notation by writing n in place of the time $t = n \tau$ of the nth step. 

## 4.1 Stock and Money Market Models

Suppose that m risky assets are traded. These will be referred to as stocks. Their prices at time $n = 0 , 1 , 2 , \ldots$ are denoted by $S _ { 1 } ( n ) , \ldots , S _ { m } ( n )$ . In addition, investors have at their disposal a risk-free asset, that is, an investment in the money market. Unless stated otherwise, we take the initial level of the riskfree investment to be one unit of the home currency, $A ( 0 ) = 1$ . However, in some numerical examples and exercises we shall often take $A ( 0 ) = 1 0 0$ for convenience. Because the money market account can be manufactured using bonds (see Chapter 2), we shall frequently refer to a risk-free investment as a position in bonds, finding it convenient to think of $A ( n )$ as the bond price at time n. 

The risky positions in assets number $1 , \ldots , m$ will be denoted by $x _ { 1 } , \ldots , x _ { m }$ respectively, and the risk-free position by $y .$ . The wealth of an investor holding such positions at time n will be 

$$
V (n) = \sum_ {j = 1} ^ {m} x _ {j} S _ {j} (n) + y A (n).\tag{4.1}
$$

Assumptions 1.1 to 1.5 of Chapter 1 can readily be adapted to this general setting. The motivation and interpretation of these assumptions are the same as in Chapter 1, with the natural changes from one to several time steps and from one to several risky assets. 

## Assumption 4.1 (Randomness)

The future stock prices $S _ { 1 } ( n ) , \ldots , S _ { m } ( n )$ are random variables for any $n =$ $1 , 2 , \ldots$ . The future prices $A ( n )$ of the risk-free security for any $n = 1 , 2 , \dots$ . are known numbers. 

## Assumption 4.2 (Positivity of Prices)

All stock and bond prices are strictly positive, 

$$
S (n) > 0 \quad \text { and } \quad A (n) > 0 \quad \text { for   } n = 0, 1, 2, \ldots .
$$

## Assumption 4.3 (Divisibility, Liquidity and Short Selling)

An investor may buy, sell and hold any number $x _ { k }$ of stock shares of each kind $k = 1 , \ldots , m$ and take any risk-free position $y ,$ whether integer or fractional, negative, positive or zero. In general, 

$$
x _ {1}, \ldots , x _ {m}, y \in \mathbb {R}.
$$

## Assumption 4.4 (Solvency)

The wealth of an investor must be non-negative at all times, 

$$
V (n) \geq 0 \quad \text { for } n = 0, 1, 2, \dots .
$$

## Assumption 4.5 (Discrete Unit Prices)

For each $n = 0 , 1 , 2 , . . .$ . the share prices $S _ { 1 } ( n ) , \ldots , S _ { m } ( n )$ are random variables taking only finitely many values. 

## 4.1.1 Investment Strategies

The positions held by an investor in the risky and risk-free assets can be altered at any time step by selling some assets and investing the proceeds in other assets. In real life cash can be taken out of the portfolio for consumption or injected from other sources. Nevertheless, we shall assume that no consumption or injection of funds takes place in our models to keep things as simple as possible. 

Decisions made by any investor of when to alter his or her portfolio and how many assets to buy or sell are based on the information currently available. We are going to exclude the unlikely possibility that investors could foresee the future, as well as the somewhat more likely (but illegal) one that they will act on insider information. However, all the historical information about the market up to and including the time instant when a particular trading decision is executed will be freely available. 

## Example 4.1

Let $m = 2$ and suppose that 

$$
\begin{array}{c c c c} S _ {1} (0) = 6 0, & S _ {1} (1) = 6 5, & S _ {1} (2) = 7 5, \\ S _ {2} (0) = 2 0, & S _ {2} (1) = 1 5, & S _ {2} (2) = 2 5, \\ A (0) = 1 0 0, & A (1) = 1 1 0, & A (2) = 1 2 1, \end{array}
$$

in a certain market scenario. At time 0 initial wealth $V ( 0 ) = 3 , 0 0 0$ dollars is invested in a portfolio consisting of $x _ { 1 } ( 1 ) = 2 0$ shares of stock number one, $x _ { 2 } ( 1 ) = 6 5$ shares of stock number two, and $y ( 1 ) = 5$ bonds. Our notational convention is to use 1 rather than 0 as the argument in $x _ { 1 } ( 1 ) , x _ { 2 } ( 1 )$ and $y ( 1 )$ to reflect the fact that this portfolio will be held over the first time step. At time 1 this portfolio will be worth $V ( 1 ) = 2 0 \times 6 5 + 6 5 \times 1 5 + 5 \times 1 1 0 = 2$ , 825 dollars. At that time the number of assets can be altered by buying or selling some of them, as long as the total value remains $2, 825. For example, we could form a new portfolio consisting of $x _ { 1 } ( 2 ) = 1 5$ shares of stock one, $x _ { 2 } ( 2 ) = 9 4 $ shares of stock two, and $y ( 2 ) = 4$ bonds, which will be held during the second time step. The value of this portfolio will be $V ( 2 ) = 1 5 \times 7 5 + 9 4 \times 2 5 + 4 \times 1 2 1 = 3 , 9 5 9$ dollars at time 2, when the positions in stocks and bonds can be adjusted once again, as long as the total value remains $3, 959, and so on. However, if no adjustments are made to the original portfolio, then it will be worth $2, 825 at time 1 and $3, 730 at time 2. 

## Definition 4.1

A portfolio is a vector $( x _ { 1 } ( n ) , \ldots , x _ { m } ( n ) , y ( n ) )$ indicating the number of shares and bonds held by an investor between times $n - 1$ and n. A sequence of portfolios indexed by $n = 1 , 2 , \ldots$ . is called an investment strategy. The wealth of an investor or the value of the strategy at time $n \geq 1$ is 

$$
V (n) = \sum_ {j = 1} ^ {m} x _ {j} (n) S _ {j} (n) + y (n) A (n).
$$

At time $n = 0$ the initial wealth is given by 

$$
V (0) = \sum_ {j = 1} ^ {m} x _ {j} (1) S _ {j} (0) + y (1) A (0).
$$

We have seen in Example 4.1 that the contents of a portfolio can be adjusted by buying or selling some assets at any time step, as long as the current value of the portfolio remains unaltered. 

## Definition 4.2

An investment strategy is called self-financing if the portfolio constructed at time $n \geq 1$ to be held over the next time step $n + 1$ is financed entirely by the current wealth $V ( n )$ , that is, 

$$
\sum_ {j = 1} ^ {m} x _ {j} (n + 1) S _ {j} (n) + y (n + 1) A (n) = V (n).\tag{4.2}
$$

## Example 4.2

Let the stock and bond prices be as in Example 4.1. Suppose that an initial wealth of $V ( 0 ) = 3$ , 000 dollars is invested by purchasing $x _ { 1 } ( 1 ) = 1 8 . 2 2$ shares of the first stock, short selling $x _ { 2 } ( 1 ) = - 1 6 . 8 1$ shares of the second stock, and buying $y ( 1 ) = 2 2 . 4 3$ bonds. The time 1 value of this portfolio will be $V ( 1 ) = 1 8 . 2 2 \times 6 5 - 1 6 . 8 1 \times 1 5 + 2 2 . 4 3 \times 1 1 0 = 3 , 3 9 9 . 4 5$ dollars. The investor will benefit from the drop of the price of the shorted stock. This example illustrates the fact that portfolios containing fractional or negative numbers of assets are allowed. 

We do not impose any restrictions on the numbers $x _ { 1 } ( n ) , \ldots , x _ { m } ( n ) , y ( n )$ The fact that they can take non-integer values is referred to as divisibility. Negative $x _ { j } ( n )$ means that stock number $j$ is sold short (in other words, a short position is taken in stock j), negative $y ( n )$ corresponds to borrowing cash (taking a short position in the money market, for example, by issuing and selling a bond). The absence of any bounds on the size of these numbers means that the market is liquid, that is, any number of assets of each type can be purchased or sold at any time. 

In practice some security measures to control short selling may be imple mented by stock exchanges. Typically, investors are required to pay a certain percentage of the short sale as a security deposit to cover possible losses. If their losses exceed the deposit, the position must be closed. The deposit creates a burden on the portfolio, particularly if it earns no interest for the investor. However, restrictions of this kind may not concern dealers who work for ma jor financial institutions holding large numbers of shares deposited by smaller investors. These shares may be borrowed internally in lieu of short selling. 

## Example 4.3

We continue assuming that stock prices follow the scenario in Example 4.1. Suppose that 20 shares of the first stock are sold short, $x _ { 1 } ( 1 ) = - 2 0 .$ . The investor will receive $2 0 \times 6 0 = 1$ , 200 dollars in cash, but has to pay a security deposit of, say 50%, that is, $600. One time step later she will sufer a loss of $2 0 \times 6 5 - 1 , 2 0 0 = 1 0 0$ dollars. This is subtracted from the deposit and the position can be closed by withdrawing the balance of $6 0 0 - 1 0 0 = 4 0 0$ dollars. On the other hand, if 60 shares of the second stock are shorted, that is, $x _ { 2 } ( 1 ) = - 6 0$ , then the investor will make a profit of 1, $2 0 0 - 6 0 \times 1 5 = 3 0 0$ dollars after one time step. The position can be closed with final wealth $6 0 0 + 3 0 0 = 9 0 0$ dollars. In both cases the final balance should be reduced by $6 0 0 \times 0 . 1 = 6 0$ dollars, the interest that would have been earned on the amount deposited, had it been invested in the money market. 

An investor constructing a portfolio at time n has no knowledge of future stock prices. In particular, no insider dealing is allowed. Investment decisions can be based only on the performance of the market to date. This is reflected in the following definition. 

## Definition 4.3

An investment strategy is called predictable if for each $n = 0 , 1 , 2 , . . .$ . the portfolio $( x _ { 1 } ( n + 1 ) , \ldots , x _ { m } ( n + 1 ) , y ( n + 1 ) )$ constructed at time n depends only on the nodes of the tree of market scenarios reached up to and including time n. 

The next proposition shows that the position taken in the risk-free asset is 

always determined by the current wealth and the positions in risky assets. 

## Proposition 4.1

Given the initial wealth $V ( 0 )$ and a predictable sequence $( x _ { 1 } ( n ) , \dots , x _ { m } ( n ) )$ , $n = 1 , 2 , \ldots$ . of positions in risky assets, it is always possible to find a sequence $y ( n )$ of risk-free positions such that $( x _ { 1 } ( n ) , \ldots , x _ { m } ( n ) , y ( n ) )$ is a predictable self-financing investment strategy. 

Proof 

Put 

$$
y (1) = \frac {V (0) - x _ {1} (1) S _ {1} (0) - \cdots - x _ {m} (1) S _ {m} (0)}{A (0)}
$$

and then compute 

$$
V (1) = x _ {1} (1) S _ {1} (1) + \dots + x _ {m} (1) S _ {m} (1) + y (1) A (1).
$$

Next, 

$$
\begin{array}{c} y (2) = \frac {V (1) - x _ {1} (2) S _ {1} (1) - \cdots - x _ {m} (2) S _ {m} (1)}{A (1)}, \\ V (2) = x _ {1} (2) S _ {1} (2) + \dots + x _ {m} (2) S _ {m} (2) + y (2) A (2), \end{array}
$$

and so on. This clearly defines a self-financing strategy. The strategy is predictable because $y ( n + 1 )$ can be expressed in terms of stock and bond price up to time n. □ 

## Exercise 4.1

Find the number of bonds $y ( 1 )$ and $y ( 2 )$ 1 held by an investor during the first and second steps of a predictable self-financing investment strategy with initial value $V ( 0 ) = 2 0 0$ dollars and risky asset positions 

$$
\begin{array}{l l} x _ {1} (1) = 3 5. 2 4, & x _ {1} (2) = - 4 0. 5 0, \\ x _ {2} (1) = 2 4. 1 8, & x _ {2} (2) = \quad 1 0. 1 3, \end{array}
$$

if the prices of assets follow the scenario in Example 4.1. Also find the time 1 value $V ( 1 )$ and time 2 value V(2) of this strategy. 

## Example 4.4

Once again, suppose that the stock and bond prices follow the scenario in Example 4.1. If an amount $V ( 0 ) = 1 0 0$ dollars were invested in a portfolio with $x _ { 1 } ( 1 ) = - 1 2 , x _ { 2 } ( 1 ) = 3 1$ and $y ( 1 ) = 2$ , then it would lead to insolvency, since the time 1 value of this portfolio is negative, $V ( 1 ) = - 1 2 \times 6 5 + 3 1 \times 1 5 + 2 \times 1 1 0 =$ 95 dollars . 

Such a portfolio, which is excluded by Assumption 4.4, would be impossible to construct in practice. No short position will be allowed unless it can be closed at any time and in any scenario (if necessary, by selling other assets in the portfolio to raise cash). This means that the wealth of an investor must be non-negative at all times. 

## Definition 4.4

A strategy is called admissible if it is self-financing, predictable, and for each $n = 0 , 1 , 2 , . . .$ 

$$
V (n) \geq 0
$$

with probability 1. 

## Exercise 4.2

Consider a market consisting of one risk-free asset with $A ( 0 ) = 1 0$ and $A ( 1 ) = 1 1$ dollars, and one risky asset such that $S ( 0 ) = 1 0 $ and $S ( 1 ) =$ 13 or 9 dollars. On the x, y plane draw the set of all portfolios $( x , y )$ such that the one-step strategy involving risky position x and risk-free position y is admissible. 

## 4.1.2 The Principle of No Arbitrage

We are ready to formulate the fundamental principle underlying all mathematical models in finance. It generalises the simplified one-step version of the No-Arbitrage Principle in Chapter 1 to models with several time steps and several risky assets. Whereas the notion of a portfolio is suficient to state the one-step version, in the general setting we need to use a sequence of portfolios forming an admissible investment strategy. This is because investors can adjust their positions at each time step. 

## Assumption 4.6 (No-Arbitrage Principle)

There is no admissible strategy such that $V ( 0 ) = 0$ and $V ( n ) > 0$ with positive probability for some $n = 1 , 2 , \ldots$ 

## Exercise 4.3

Show that the No-Arbitrage Principle would be violated if there was a self-financing predictable strategy with initial value $V ( 0 ) = 0$ and final value $0 \neq V ( 2 ) \geq 0$ , such that $V ( 1 ) < 0$ with positive probability. 

The strategy in Exercise 4.3 clearly violates the solvency assumption (As sumption 4.4), since V(1) may be negative. In fact, this assumption is not essential for the formulation of the No-Arbitrage Principle. An admissible strategy realising an arbitrage opportunity can be found whenever there is a predictable self-financing strategy (possibly violating Assumption 4.4) such that $V ( 0 ) = 0$ and $0 \neq V ( n ) \geq 0$ for some $n > 0$ 

## Exercise 4.4

Consider a market with one risk-free asset and one risky asset that follows the binomial tree model. Suppose that whenever stock goes up, you can predict that it will go down at the next step. Find a self-financing (but not necessarily predictable) strategy with $V ( 0 ) = 0 , V ( 1 ) \geq 0$ and $0 \neq V ( 2 ) \geq 0 .$ 

This exercise indicates that predictability is an essential assumption in the No-Arbitrage Principle. An investor who could foresee the future behaviour of stock prices (here, if stock goes down at one step, you can predict what it will do at the next step) would always be able to find a suitable investment strategy to ensure a risk-free profit. 

## Exercise 4.5

Consider a market with a risk-free asset such that $A ( 0 ) = 1 0 0 , A ( 1 ) =$ 110, $A ( 2 ) = 1 2 1$ dollars and a risky asset, the price of which can follow three possible scenarios, 

<table><tr><td>Scenario</td><td><eq>S(0)</eq></td><td><eq>S(1)</eq></td><td><eq>S(2)</eq></td></tr><tr><td><eq>\omega_1</eq></td><td>100</td><td>120</td><td>144</td></tr><tr><td><eq>\omega_2</eq></td><td>100</td><td>120</td><td>96</td></tr><tr><td><eq>\omega_3</eq></td><td>100</td><td>90</td><td>96</td></tr></table>

Is there an arbitrage opportunity if a) there are no restrictions on short selling, and b) no short selling of the risky asset is allowed? 

## Exercise 4.6

Given the bond and stock prices in Exercise 4.5, is there an arbitrage strategy if short selling of stock is allowed, but the number of units of each asset in a portfolio must be an integer? 

## Exercise 4.7

Given the bond and stock prices in Exercise 4.5, is there an arbitrage strategy if short selling of stock is allowed, but transaction costs of 5% of the transaction volume apply whenever stock is traded. 

## 4.1.3 Application to the Binomial Tree Model

We shall see that in the binomial tree model with several time steps Condi tion 3.2 is equivalent to the lack of arbitrage. 

## Proposition 4.2

The binomial tree model admits no arbitrage if and only if $d < r < u .$ 

## Proof

We shall begin with a one-step binomial tree. This will then be used as a building block in the case of several time steps. 

One step. Suppose that $r \leq d .$ . If so, then: 

Borrow 1 dollar at the risk-free rate. 

Buy $1 / S ( 0 )$ shares. 

That is to say, construct a portfolio with $x = 1 / S ( 0 )$ and $y = - 1$ , the value of which is $V ( 0 ) = 0$ . After one step, either $S ( 1 ) = S ( 0 ) ( 1 + d )$ and $V ( 1 ) =$ $- r + d \ge 0 , \mathrm { o r } S ( 1 ) = S ( 0 ) ( 1 + u )$ and $V ( 1 ) = - r + u > 0$ , leading to arbitrage. Suppose that $u \leq r$ . In this case: 

Buy one bond. 

Sell short $1 / S ( 0 )$ shares. 

The resulting portfolio with $x = - 1 / S ( 0 )$ and $y = 1$ will once again have initial value $V ( 0 ) = 0$ . After one step this portfolio will be worth $V ( 1 ) = r - u \geq 0$ if the stock price goes up, or $V ( 1 ) = r - d > 0$ if it goes down, also realising an arbitrage opportunity. 

Finally, suppose that d $< r < u$ . Every portfolio with $V ( 0 ) = 0$ must be of the form $x = a / S ( 0 )$ and $y = - a$ for some real number a. Consider the 

following three cases: 

1) $a = 0$ (a trivial portfolio consisting of no cash and no stock). Then $V ( 1 ) = 0$ identically. 

2) $a > 0$ (a cash loan invested in stock). Then $V ( 1 ) = a ( d - r ) < 0$ if the price of stock goes down. 

3) $a \textless 0$ (a long position in bonds financed by shorting stock). In this case $V ( 1 ) = a ( u - r ) < 0$ if stock goes up. 

Arbitrage is clearly impossible when d $< r < u$ 

The above argument shows that d $< r < u$ if and only if there is no arbitrage in the one-step case. 

Several steps. Let $d < r < u$ and suppose there is an arbitrage strategy. The tree of stock prices can be considered as a collection of one-step subtrees, as in Figure 4.1. By taking the smallest n for which $V ( n ) \neq 0$ , we can find a one-step subtree with $V ( n - 1 ) = 0$ at its root and $V ( n ) \geq 0$ at each node growing out of this root, with $V ( n ) > 0$ at one or more of these nodes. By the one-step case this is impossible if $d < r < u$ , leading to a contradiction. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/4b62d97b6cb0ebbd4167328181524d8cf26041dda5ce2954b8c19a7f2b3e4a5d.jpg)



Figure 4.1 One-step subtrees in a two-step binomial model


Conversely, suppose that there is no arbitrage in the binomial tree model with several steps. Then for any strategy such that $V ( 0 ) = 0$ it follows that $V ( n ) = 0$ for any n and, in particular, $V ( 1 ) = 0$ . This implies that $d < r < u$ by the above argument in the one-step case. □ 

We shall conclude this chapter with a brief discussion of a fundamental relationship between the risk-neutral probability and the No-Arbitrage Principle. First, we observe that the lack of arbitrage is equivalent to the existence of a risk-neutral probability in the binomial tree model. 

## Proposition 4.3

The binomial tree model admits no arbitrage if and only if there exists a risk neutral probability $p _ { * }$ such that $0 < p _ { * } < 1$ 

## Proof

This is an immediate consequence of Exercise 3.18 and Proposition 4.2. 

## 4.1.4 Fundamental Theorem of Asset Pricing

In this section, which can be omitted on first reading, we return to the general setting under Assumptions 4.1 to 4.5. 

We already know that the discounted stock prices in the binomial tree mode form a martingale under the risk-neutral probability, see Proposition 3.5 and Corollary 3.6. The following result extends these observations to any discrete model. 

## Theorem 4.4 (Fundamental Theorem of Asset Pricing)

The No-Arbitrage Principle is equivalent to the existence of a probability $P _ { * }$ on the set of scenarios $\varOmega$ such that $P _ { * } ( \omega ) > 0$ for each scenario $\omega \in \varOmega$ and the discounted stock prices $\widetilde { S } _ { j } ( n ) = S _ { j } ( n ) / A ( n )$ satisfy 

$$
E _ {*} (\widetilde {S} _ {j} (n + 1) | S (n)) = \widetilde {S} _ {j} (n)\tag{4.3}
$$

for any $j = 1 , \dots , m$ and $n = 0 , 1 , 2 , \ldots$ , where $E _ { * } ( { \bf \Omega } \cdot { \bf \Omega } | S ( n ) )$ denotes the conditional expectation with respect to probability $P _ { * }$ computed once the stock price $S ( n )$ becomes known at time n. 

The proof of the Fundamental Theorem of Asset Pricing is quite technical and will be omitted. 

## Definition 4.5

A sequence of random variables $X ( 0 ) , X ( 1 ) , X ( 2 ) , . .$ . such that 

$$
E _ {*} (X (n + 1) | S (n)) = X (n)
$$

for each $n = 0 , 1 , 2 , \ldots$ . is said to be a martingale with respect to $P _ { * }$ . 

Condition (4.3) can be expressed by saying that the discounted stock prices $\widetilde { S } _ { j } ( 0 ) , \widetilde { S } _ { j } ( 1 ) , \widetilde { S } _ { j } ( 2 ) ,$ , . . . form a martingale with respect to $P _ { * }$ . The latter is called a risk-neutral or martingale probability on the set of scenarios $\varOmega$ . Moreover, $E _ { * }$ is called a risk-neutral or martingale expectation. 

## Example 4.5

Let $A ( 0 ) = 1 0 0 , A ( 1 ) = 1 1 0 , A ( 2 ) = 1 2 1$ and suppose that stock prices can follow four possible scenarios: 

<table><tr><td>Scenario</td><td>S(0)</td><td>S(1)</td><td>S(2)</td></tr><tr><td><eq>\omega_1</eq></td><td>90</td><td>100</td><td>112</td></tr><tr><td><eq>\omega_2</eq></td><td>90</td><td>100</td><td>106</td></tr><tr><td><eq>\omega_3</eq></td><td>90</td><td>80</td><td>90</td></tr><tr><td><eq>\omega_4</eq></td><td>90</td><td>80</td><td>80</td></tr></table>

The tree of stock prices is shown in Figure 4.2. The risk-neutral probability $P _ { * }$ is represented by the branching probabilities $p _ { * } , q _ { * } , r _ { * }$ at each node. Condition 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/056c5cc35779ea33af432d24cdab96c35976e183e26cf1b7ebaa631c7a667c97.jpg)



Figure 4.2 Tree of stock prices in Example 4.5


(4.3) for $\widetilde { S } ( n ) = S ( n ) / A ( n )$ can be written in the form of three equations, one for each node of the tree, 

$$
\frac {1 0 0}{1 1 0} p _ {*} + \frac {8 0}{1 1 0} (1 - p _ {*}) = \frac {9 0}{1 0 0},
$$

$$
\frac {1 1 2}{1 2 1} q _ {*} + \frac {1 0 6}{1 2 1} (1 - q _ {*}) = \frac {1 0 0}{1 1 0},
$$

$$
\frac {9 0}{1 2 1} r _ {*} + \frac {8 0}{1 2 1} (1 - r _ {*}) = \frac {8 0}{1 1 0}.
$$

These can be solved to find 

$$
p _ {*} = \frac {1 9}{2 0}, q _ {*} = \frac {2}{3}, r _ {*} = \frac {4}{5}.
$$

For each scenario (each path through the tree) the corresponding risk-neutral probability can be computed as follows: 

$$
P _ {*} (\omega_ {1}) = p _ {*} q _ {*} = \frac {1 9}{2 0} \times \frac {2}{3} = \frac {1 9}{3 0},
$$

$$
P _ {*} (\omega_ {2}) = p _ {*} (1 - q _ {*}) = \frac {1 9}{2 0} \times \left(1 - \frac {2}{3}\right) = \frac {1 9}{6 0},
$$

$$
P _ {*} (\omega_ {3}) = (1 - p _ {*}) r _ {*} = \left(1 - \frac {1 9}{2 0}\right) \times \frac {4}{5} = \frac {1}{2 5},
$$

$$
P _ {*} (\omega_ {4}) = (1 - p _ {*}) (1 - r _ {*}) = \left(1 - \frac {1 9}{2 0}\right) \times \left(1 - \frac {4}{5}\right) = \frac {1}{1 0 0}.
$$

By Theorem 4.4 the existence of a risk-neutral probability implies that there is no arbitrage. 

## 4.2 Extended Models

Securities such as stock, which are traded independently of other assets, are called primary securities. By contrast, derivative securities such as, for exam ple, options or forwards (in Chapter 1 we have seen some simple examples of these) are legal contracts conferring certain financial rights or obligations upon the holder, contingent on the prices of other securities, referred to as the underlying securities. An underlying security may be a primary security, as for a forward contract on stock, but it may also be a derivative security, as in the case of an option on futures. A derivative security cannot exist in its own right, unless the underlying security or securities are traded. Derivative securities are also referred to as contingent claims because their value is contingent on the underlying securities. 

For example, the holder of a long forward contract on a stock is committed to buying the stock for the forward price at a specified time of delivery, no matter how much the actual stock price turns out to be at that time. The value of the forward position is contingent on the stock. It will become positive if the market price of stock turns out to be higher than the forward price on delivery. If the stock price turns out to be lower than the forward price, then the value of the forward position will be negative. 

## Remark 4.1

The assumptions in Section 4.1, including the No-Arbitrage Principle, are stated for strategies consisting of primary securities only, such as stocks and bonds (or the money market account). Nevertheless, in many texts they are invoked in arbitrage proofs involving strategies constructed out of derivative securities in addition to stocks and bonds. To avoid this inaccuracy the assumptions need to be extended to strategies consisting of both primary and derivative securities. 

The setting of Section 4.1, involving portfolios of risky stocks and the money market account, will be extended to include risky securities of various other kinds in addition to (and sometimes in place of) stock. In particular, to cover real-life situations we need to include derivative securities such as forwards or options, but also primary securities such as bonds of various maturities, the future prices of which may be random (except, of course, at maturity). We shall also relax the assumption that an investment in a money market accoun should be risk-free, with a view towards modelling random interest rates. In this way we prepare the stage for a detailed study of derivative securities in Chapters 6, 7 and 8, and random bond prices and the term structure of interest rates in Chapters 10 and 11. 

Securities of various kinds will be treated on a similar footing as stock in Section 4.1. We shall denote by $S _ { 1 } ( n ) , \ldots , S _ { m } ( n )$ the time n prices of m dif ferent primary securities, typically m diferent stocks, though they may also include other assets such as foreign currency, commodities or bonds of various maturities. Moreover, the price of one distinguished primary security, the money market account, will be denoted by $A ( n )$ . In addition, we introduce k diferent derivative securities such as forwards, call and put options, or indeed any other contingent claims, whose time n market prices will be denoted by $D _ { 1 } ( n ) , \ldots , D _ { k } ( n )$ 

As opposed to stocks and bonds, we can no longer insist that the prices of all derivative securities should be positive. For example, at the time of exchanging a forward contract its value is zero, which may and often does become negative later on because the holder of a long forward position may have to buy the stock above its market price at delivery. The future prices $S _ { 1 } ( n ) , \ldots , S _ { m } ( n )$ and $A ( n )$ of primary securities and the future prices $D _ { 1 } ( n ) , \ldots , D _ { k } ( n )$ of derivative securities may be random for $n = 1 , 2 , \ldots$ , but we do not rule out the possibility that some of them, such as the prices of bonds at maturity, may in fact be known in advance, being represented by constant random variables or simply real numbers. All the current prices $S _ { 1 } ( 0 ) , \ldots , S _ { m } ( 0 ) , A ( 0 ) , D _ { 1 } ( 0 ) , \ldots , D _ { k } ( 0 )$ are of course known at time 0, that is, are also just real numbers. 

The positions in primary securities, including the money market account, will be denoted by $x _ { 1 } , \ldots , x _ { m }$ and $y .$ , and those in derivative securities by $z _ { 1 } , \ldots , z _ { k }$ , respectively. The wealth of an investor holding such positions a time n will be 

$$
V (n) = \sum_ {j = 1} ^ {m} x _ {j} S _ {j} (n) + y A (n) + \sum_ {i = 1} ^ {k} z _ {i} D _ {i} (n),
$$

which extends formula (4.1). 

The assumptions in Section 4.1 need to be replaced by the following. 

## Assumption 4.1a (Randomness)

The asset prices $S _ { 1 } ( n ) , \ldots , S _ { m } ( n ) , A ( n ) , D _ { 1 } ( n ) , \ldots , D _ { k } ( n )$ are random vari ables for any $n = 1 , 2 , \ldots$ 

## Assumption 4.2a (Positivity of Prices)

The prices of primary securities, including the money market account, are positive, 

$$
S _ {1} (n), \dots , S _ {m} (n), A (n) > 0 \quad \text { for } n = 0, 1, 2, \dots .
$$

## Assumption 4.3a (Divisibility, Liquidity and Short Selling)

An investor may buy, sell and hold any number of assets, whether integer or fractional, negative, positive or zero. In general, 

$$
x _ {1}, \ldots , x _ {m}, y, z _ {1}, \ldots , z _ {k} \in \mathbb {R}.
$$

## Assumption 4.4a (Solvency)

The wealth of an investor must be non-negative at all times, 

$$
V (n) \geq 0 \quad \text { for } n = 0, 1, 2, \dots .
$$

## Assumption 4.5a (Discrete Unit Prices)

For each $n = 0 , 1 , 2 , . . .$ . the prices $S _ { 1 } ( n ) , \ldots , S _ { m } ( n ) , A ( n ) , D _ { 1 } ( n ) , \ldots , D _ { k } ( n )$ are random variables taking only finitely many values. 

Definitions 4.1 to 4.4 also extend immediately to the case in hand. 

## Definition 4.1a

A portfolio is a vector 

$$
(x _ {1} (n), \dots , x _ {m} (n), y (n), z _ {1} (n), \dots , z _ {k} (n))
$$

indicating the number of primary and derivative securities held by an investor between times $n - 1$ and n. A sequence of portfolios indexed by $n = 1 , 2 , \ldots$ is called an investment strategy. The wealth of an investor or the value of the strategy at time $n \geq 1$ is 

$$
V (n) = \sum_ {j = 1} ^ {m} x _ {j} (n) S _ {j} (n) + y (n) A (n) + \sum_ {i = 1} ^ {k} z _ {i} (n) D _ {i} (n).
$$

At time $n = 0$ the initial wealth is given by 

$$
V (0) = \sum_ {j = 1} ^ {m} x _ {j} (1) S _ {j} (0) + y (1) A (0) + \sum_ {i = 1} ^ {k} z _ {i} (1) D _ {i} (0).
$$

## Definition 4.2a

An investment strategy is called self-financing if the portfolio constructed at time $n \geq 1$ to be held over the next time step $n + 1$ is financed entirely by the current wealth $V ( n )$ , that is, 

$$
\sum_ {j = 1} ^ {m} x _ {j} (n + 1) S _ {j} (n) + y (n + 1) A (n) + \sum_ {i = 1} ^ {k} z _ {i} (n + 1) D _ {i} (n) = V (n).
$$

## Definition 4.3a

An investment strategy is called predictable if for each $n = 0 , 1 , 2 , . . .$ . the portfolio 

$$
(x _ {1} (n + 1), \dots , x _ {m} (n + 1), y (n + 1), z _ {1} (n + 1), \dots , z _ {k} (n + 1))
$$

constructed at time n depends only on the nodes of the tree of market scenarios reached up to and including time n. 

## Definition 4.4a

A strategy is called admissible if it is self-financing, predictable, and for each $n = 0 , 1 , 2 , . . .$ 

$$
V (n) \geq 0
$$

with probability 1. 

The No-Arbitrage Principle extends without any modifications. 

## Assumption 4.6a (No-Arbitrage Principle)

There is no admissible strategy such that $V ( 0 ) = 0$ and $V ( n ) > 0$ with positive probability for some $n = 1 , 2 , \ldots$ 

Finally, the Fundamental Theorem of Asset Pricing takes the following form. 

## Theorem 4.4a (Fundamental Theorem of Asset Pricing)

The No-Arbitrage Principle is equivalent to the existence of a probability $P _ { * }$ on the set of scenarios Ω such that $P _ { * } ( \omega ) > 0$ for each scenario $\omega \in \varOmega$ and the discounted prices of primary and derivative securities $\widetilde { S } _ { j } ( n ) = S _ { j } ( n ) / A ( n )$ and $\widetilde { D } _ { i } ( n ) = D _ { i } ( n ) / A ( n )$ form martingales with respect to $P _ { * }$ , that is, satisfy 

$$
E _ {*} (\widetilde {S} _ {j} (n + 1) | S (n)) = \widetilde {S} _ {j} (n), \quad E _ {*} (\widetilde {D} _ {i} (n + 1) | S (n)) = \widetilde {D} _ {i} (n)
$$

for any $j = 1 , \dots , m _ { ; }$ , any $i = 1 , \ldots , k$ and any $n = 0 , 1 , 2 , \ldots$ , where $E _ { * } ( { \bf \cdot } | S ( n ) )$ denotes the conditional expectation with respect to probability $P _ { * }$ computed once the stock price $S ( n )$ becomes known at time n. 

## Example 4.6

We shall use the same scenarios $\omega _ { 1 } , \omega _ { 2 } , \omega _ { 3 } , \omega _ { 4 }$ , stock prices $S ( 0 ) , S ( 1 ) , S ( 2 )$ and money market prices $A ( 0 ) , A ( 1 ) , A ( 2 )$ as in Example 4.5. In addition, we consider a European call option giving the holder the right (but no obligation) to buy the stock for the strike price of $X = 8 5$ dollars at time 2. 

In this situation we need to consider an extended model with three assets, the stock, the money market, and the option, with unit prices $S ( n ) , A ( n ) , C ^ { \operatorname { E } } ( n )$ respectively, where $C ^ { \mathrm { E } } ( n )$ is the market price of the option at time $n = 0 , 1 , 2$ 

The time 2 option price is determined by the strike price and the stock price, 

$$
C ^ {\mathrm{E}} (2) = \max \{S (2) - X, 0 \}.
$$

The prices $C ^ { \mathrm { E } } ( 0 )$ and $C ^ { \mathrm { E } } ( 1 )$ can be found using the Fundamental Theorem of Asset Pricing. (Which explains the name of the theorem!) According to the theorem, there is a probability $P _ { * }$ such that the discounted stock and option prices $\widetilde { S } ( n ) = S ( n ) / A ( n )$ and $\widetilde { C } ^ { \mathrm { E } } ( n ) = C ^ { \mathrm { E } } ( n ) / A ( n )$ are martingales, or else an arbitrage opportunity would exist. However, there is only one probability $P _ { * }$ turning $\widetilde { S } ( n )$ into a martingale, namely that found in Example 4.5. As a result, $\widetilde C ^ { \mathrm { E } } ( n )$ must be a martingale with respect to the same probability $P _ { * }$ This gives 

$$
C ^ {\mathrm{E}} (1) = \frac {A (1)}{A (2)} E _ {*} (C ^ {\mathrm{E}} (2) | S (1)) \quad \text { and } \quad C ^ {\mathrm{E}} (0) = \frac {A (0)}{A (1)} E _ {*} (C ^ {\mathrm{E}} (1)).
$$

The values of $P _ { * }$ for each scenario found in Example 4.5 can now be used to compute $C ^ { \mathrm { E } } ( 1 )$ and then $C ^ { \mathrm { E } } ( 0 )$ . For example, 

$$
\begin{array}{c} C ^ {\mathrm{E}} (1, \omega_ {1}) = C ^ {\mathrm{E}} (1, \omega_ {2}) = \frac {A (1)}{A (2)} \frac {P _ {*} (\omega_ {1}) C ^ {\mathrm{E}} (2 , \omega_ {1}) + P _ {*} (\omega_ {2}) C ^ {\mathrm{E}} (2 , \omega_ {2})}{P _ {*} (\omega_ {1}) + P _ {*} (\omega_ {2})} \\ = \frac {1 1 0}{1 2 1} \frac {\frac {1 9}{3 0} \times 2 7 + \frac {1 9}{6 0} \times 2 1}{\frac {1 9}{3 0} + \frac {1 9}{6 0}} \cong 2 2. 7 3 \end{array}
$$

dollars. Proceeding in a similar way, we obtain 

<table><tr><td>Scenario</td><td><eq>C^{\text{E}}(0)</eq></td><td><eq>C^{\text{E}}(1)</eq></td><td><eq>C^{\text{E}}(2)</eq></td></tr><tr><td><eq>\omega_1</eq></td><td>19.79</td><td>22.73</td><td>27.00</td></tr><tr><td><eq>\omega_2</eq></td><td>19.79</td><td>22.73</td><td>21.00</td></tr><tr><td><eq>\omega_3</eq></td><td>19.79</td><td>3.64</td><td>5.00</td></tr><tr><td><eq>\omega_4</eq></td><td>19.79</td><td>3.64</td><td>0.00</td></tr></table>

## Exercise 4.8

Apply the Fundamental Theorem of Asset Pricing to find the time 0 and 1 prices of a put option with strike price $110 maturing after two steps, given the same scenarios $\omega _ { 1 } , \omega _ { 2 } , \omega _ { 3 } , \omega _ { 4 }$ , stock prices S(0), S(1), S(2) and money market prices $A ( 0 ) , A ( 1 ) , A ( 2 )$ as in Example 4.5. 

An investment in a risky security always carries the burden of possible losses or poor performance. In this chapter we analyse the advantages of spreading the investment among several securities. Even though the mathematical tools involved are quite simple, they lead to formidable results. 

## 5.1 Risk

First of all, we need to identify a suitable quantity to measure risk. An investment in bonds returning, for example, 8% at maturity is free of risk, in which case the measure of risk should be equal to zero. If the return on an investmen is, say 11% or 13%, depending on the market scenario, then the risk is clearly smaller as compared with an investment returning 2% or 22%, respectively. However, the spread of return values can hardly be used to measure risk be cause it ignores the probabilities. If the return rate is 22% with probability 0.99 and 2% with probability 0.01, the risk can be considered quite small, whereas the same rates of return occurring with probability 0.5 each would indicate a rather more risky investment. The desired quantity needs to capture the following two aspects of risk: 1) the distances between a certain reference value and the rates of return in each market scenario and 2) the probabilities of diferent scenarios. 

The return K on a risky investment is a random variable. It is natural to take the expectation E(K) as the reference value. The variance Var(K) turns 

out to be a convenient measure of risk. 

## Exercise 5.1

Compute the risk $\mathrm { V a r } ( K _ { 1 } )$ , $\mathrm { V a r } ( K _ { 2 } )$ and $\mathrm { V a r } ( K _ { 3 } )$ in each of the following three investment projects, where the returns $K _ { 1 } , K _ { 2 }$ and $K _ { 3 }$ depend on the market scenario: 

<table><tr><td>Scenario</td><td>Probability</td><td>Return <eq>K_{1}</eq></td><td>Return <eq>K_{2}</eq></td><td>Return <eq>K_{3}</eq></td></tr><tr><td><eq>\omega_{1}</eq></td><td>0.25</td><td>12%</td><td>11%</td><td>2%</td></tr><tr><td><eq>\omega_{2}</eq></td><td>0.75</td><td>12%</td><td>13%</td><td>22%</td></tr></table>


Which of these is the most risky and the least risky project? 


## Exercise 5.2

Consider two scenarios, $\omega _ { 1 }$ with probability $\textstyle { \frac { 1 } { 4 } }$ and $\omega _ { 2 }$ with probability $\textstyle { \frac { 3 } { 4 } }$ . Suppose that the return on a certain security is $K _ { 1 } ( \omega _ { 1 } ) = - 2 \%$ in the first scenario and $K _ { 1 } ( \omega _ { 2 } ) = 8 \%$ in the second scenario. If the return on another security is $K _ { 2 } ( \omega _ { 1 } ) = - 4 \%$ in the first scenario, find the return $K _ { 2 } ( \omega _ { 2 } )$ in the other scenario such that the two securities have the same risk. 

In some circumstances the standard deviation $\sigma _ { K } = \sqrt { \mathrm { V a r } ( K ) }$ of the return is a more convenient measure of risk. If a quantity is measured in certain units, then the standard deviation will be expressed in the same units, so it can be related directly to the original quantity, in contrast to variance, which will be expressed in squared units. 

## Example 5.1

Let the return on an investment be $K = 3 \% \ \mathrm { { o r } \ - 1 \% }$ , both with probability 0.5. Then the risk is 

$$
\operatorname{Var} (K) = 0. 0 0 0 4 \quad \text { or } \quad \sigma_ {K} = 0. 0 2,
$$

depending on whether we choose the variance or standard deviation. Now suppose that the return on another investment is double that on the first investment, being equal to $2 K = 6 \% \ \mathrm { { o r } \ - 2 \% } .$ , also with probability 0.5 each. Then the risk of the second investment will be 

$$
\operatorname{Var} (2 K) = 0. 0 0 1 6 \quad \text { or } \quad \sigma_ {2 K} = 0. 0 4.
$$

The risk as measured by the variance is quadrupled, while the standard devi ation is simply doubled. 

This illustrates the following general rule: 

$$
\operatorname{Var} (a K) = a ^ {2} \operatorname{Var} (K),
$$

$$
\sigma_ {a K} = | a | \sigma_ {K}
$$

for any real number a. 

## Remark 5.1

Another natural way to quantify risk would be to use the variance $\mathrm { V a r } ( k )$ (or the standard deviation $\sigma _ { k } )$ of the logarithmic return k. The choice between K and k is dictated to a large extent by the properties needed to handle the task in hand. For example, if one is interested in a sequence of investments following one another in time, then the variance of the logarithmic return may be more useful as a measure of risk. This is because of the additivity of risks based on logarithmic returns: 

$$
\operatorname{Var} (k (0, n)) = \operatorname{Var} (k (1)) + \dots + \operatorname{Var} (k (n)),
$$

where $k ( i )$ is the logarithmic return in time step $i = 1 , \ldots , n$ and $k ( 0 , n )$ is the logarithmic return over the whole time interval from 0 to n, provided that the $k ( i )$ are independent. The above formula holds because $k ( 0 , n ) = k ( 1 ) + \cdot \cdot \cdot +$ $k ( n )$ by Proposition 3.2, and the variance of a sum of independent random variables is the sum of their variances. (This is not necessarily so without independence.) 

However, in the present chapter we shall be concerned with a portfolio of several securities held simultaneously over a single time step. The properties of $E ( K )$ and $\mathrm { V a r } ( K )$ , where K is the ordinary return on the portfolio (see formulae (5.4) and (5.5) below), are much more convenient for this purpose than those for the logarithmic return. 

## Exercise 5.3

Consider two risky securities with returns $K _ { 1 }$ and $K _ { 2 }$ given by 

<table><tr><td>Scenario</td><td>Probability</td><td>Return <eq>K_{1}</eq></td><td>Return <eq>K_{2}</eq></td></tr><tr><td><eq>\omega_{1}</eq></td><td>0.5</td><td>10.53%</td><td>7.23%</td></tr><tr><td><eq>\omega_{2}</eq></td><td>0.5</td><td>13.87%</td><td>10.57%</td></tr></table>

Compute the corresponding logarithmic returns $k _ { 1 }$ and $k _ { 2 }$ and compare $\mathrm { V a r } ( k _ { 1 } )$ with ${ \mathrm { V a r } } ( k _ { 2 } )$ and $\mathrm { V a r } ( K _ { 1 } )$ with $\mathrm { V a r } ( K _ { 2 } )$ 

## 5.2 Two Securities

We begin a detailed discussion of the relationship between risk and expected return in the simple situation of a portfolio with just two risky securities. 

## Example 5.2

Suppose that the prices of two stocks behave as follows: 

<table><tr><td>Scenario</td><td>Probability</td><td>Return <eq>K_{1}</eq></td><td>Return <eq>K_{2}</eq></td></tr><tr><td><eq>\omega_{1}</eq></td><td>0.5</td><td>10%</td><td>-5%</td></tr><tr><td><eq>\omega_{2}</eq></td><td>0.5</td><td>-5%</td><td>10%</td></tr></table>

If we split our money equally between these two stocks, then we shall earn 5% in each scenario (losing 5% on one stock, but gaining 10% on the other). Even though an investment in either stock separately involves risk, we have reduced the overall risk to nil by splitting the investment between the two stocks. This is a simple example of diversification, which is particularly efective here because the returns are negatively correlated. 

In addition to the description of a portfolio in terms of the number of shares of each security held (developed in Section 4.1), we shall introduce another very convenient notation to describe the allocation of funds between the securities. 

## Example 5.3

Suppose that the prices of two kinds of stock are $S _ { 1 } ( 0 ) = 3 0$ and $S _ { 2 } ( 0 ) = 4 0$ dollars. We prepare a portfolio worth $V ( 0 ) = 1 , 0 0 0$ dollars by purchasing $x _ { 1 } = 2 0$ shares of stock number 1 and $x _ { 2 } = 1 0$ shares of stock number 2. The allocation of funds between the two securities is 

$$
w _ {1} = \frac {3 0 \times 2 0}{1 , 0 0 0} = 60 \%, \quad w _ {2} = \frac {1 0 \times 4 0}{1 , 0 0 0} = 40 \%.
$$

The numbers $w _ { 1 }$ and $w _ { 2 }$ are called the weights. If the stock prices change to $S _ { 1 } ( 1 ) = 3 5$ and $S _ { 2 } ( 1 ) = 3 9$ dollars, then the portfolio will be worth $V ( 1 ) =$ $2 0 \times 3 5 + 1 0 \times 3 9 = 1 , 0 9 0$ dollars. Observe that this amount is no longer spli between the two securities as 60% to 40%, but as follows: 

$$
\frac {2 0 \times 3 5}{1 , 0 9 0} \cong 64.22\% , \quad \frac {1 0 \times 3 9}{1 , 0 9 0} \cong 35.78\% ,
$$

even though the actual number of shares of each stock in the portfolio remains unchanged. 

The weights are defined by 

$$
w _ {1} = \frac {x _ {1} S _ {1} (0)}{V (0)}, \quad w _ {2} = \frac {x _ {2} S _ {2} (0)}{V (0)},
$$

where $x _ { 1 }$ and $x _ { 2 }$ are share numbers of stock 1 and 2 in the portfolio. This means that $w _ { k }$ is the percentage of the initial value of the portfolio invested in security number k. Observe that the weights always add up to 100%, 

$$
w _ {1} + w _ {2} = \frac {x _ {1} S _ {1} (0) + x _ {2} S _ {2} (0)}{V (0)} = \frac {V (0)}{V (0)} = 1.\tag{5.1}
$$

If short selling is allowed, then one of the weights may be negative and the other one greater than 100%. 

## Example 5.4

Suppose that a portfolio worth $V ( 0 ) = 1 , 0 0 0$ dollars is constructed by taking a long position in stock number 1 and a short position in stock number 2 in Example 5.3 with weights $w _ { 1 } = 1 2 0 \%$ and $w _ { 2 } = - 2 0 \%$ . The portfolio will consist of 

$$
x _ {1} = w _ {1} \frac {V (0)}{S _ {1} (0)} = 120 \% \times \frac {1,000}{30} = 40,
$$

$$
x _ {2} = w _ {2} \frac {V (0)}{S _ {2} (0)} = - 20 \% \times \frac {1 , 0 0 0}{4 0} = - 5
$$

shares of type 1 and 2. If the stock prices change as in Example 5.3, then thi portfolio will be worth 

$$
\begin{aligned} V(1) & = x_{1}S_{1}(1) + x_{2}S_{2}(1) = V(0)\left(w_{1}\frac{S_{1}(1)}{S_{1}(0)} +w_{2}\frac{S_{2}(1)}{S_{2}(0)}\right)\\ & = 1,000\left(120\% \times \frac{35}{30} -20\% \times \frac{39}{40}\right) = 1,205 \end{aligned}
$$

dollars, benefiting from both the rise of the price of stock 1 and the fall of stock 2. However, a small investor may have to face some restrictions on short selling. For example, it may be necessary to pay a security deposit equal to 50% of the sum raised by shorting stock number 2. The deposit, which would amount to $5 0 \% \times 2 0 0 = 1 0 0$ dollars, can be borrowed at the risk-free rate and the interest paid on this loan will need to be subtracted from the final value $V ( 1 )$ of the portfolio. 

## Exercise 5.4

Compute the value $V ( 1 )$ of a portfolio worth initially $V ( 0 ) ~ = ~ 1 0 0$ dollars that consists of two securities with weights $w _ { 1 } ~ = ~ 2 5 \%$ and $w _ { 2 } = 7 5 \%$ , given that the security prices are $S _ { 1 } ( 0 ) = 4 5$ and $S _ { 2 } ( 0 ) = 3 3$ dollars initially, changing to $S _ { 1 } ( 1 ) = 4 8$ and $S _ { 2 } ( 1 ) = 3 2$ dollars. 

We can see in Example 5.4 and Exercise 5.4 that $V ( 1 ) / V ( 0 )$ depends on the prices of securities only through the ratios $S _ { 1 } ( 1 ) / S _ { 1 } ( 0 ) = 1 + K _ { 1 }$ and $S _ { 2 } ( 1 ) / S _ { 2 } ( 0 ) = 1 + K _ { 2 }$ . This indicates that the return on the portfolio should depend only on the weights $w _ { 1 } , w _ { 2 }$ and the returns $K _ { 1 } , K _ { 2 }$ on each of the two securities. 

## Proposition 5.1

The return $K _ { V }$ on a portfolio consisting of two securities is the weighted average 

$$
K _ {V} = w _ {1} K _ {1} + w _ {2} K _ {2},\tag{5.2}
$$

where $w _ { 1 }$ and $w _ { 2 }$ are the weights and $K _ { 1 }$ and $K _ { 2 }$ the returns on the two components. 

## Proof

Suppose that the portfolio consists of $x _ { 1 }$ shares of security 1 and $x _ { 2 }$ shares of security 2. Then the initial and final values of the portfolio are 

$$
\begin{array}{c} V (0) = x _ {1} S _ {1} (0) + x _ {2} S _ {2} (0), \\ V (1) = x _ {1} S _ {1} (0) (1 + K _ {1}) + x _ {2} S _ {2} (0) (1 + K _ {2}) \\ = V (0) \left(w _ {1} (1 + K _ {1}) + w _ {2} (1 + K _ {2})\right). \end{array}
$$

As a result, the return on the portfolio is 

$$
K _ {V} = \frac {V (1) - V (0)}{V (0)} = w _ {1} K _ {1} + w _ {2} K _ {2}.
$$

## Exercise 5.5

Find the return on a portfolio consisting of two kinds of stock with weights $w _ { 1 } = 3 0 \%$ and $w _ { 2 } = 7 0 \%$ if the returns on the components are 

as follows: 

<table><tr><td>Scenario</td><td>Return <eq>K_{1}</eq></td><td>Return <eq>K_{2}</eq></td></tr><tr><td><eq>\omega_{1}</eq></td><td>12%</td><td>-4%</td></tr><tr><td><eq>\omega_{2}</eq></td><td>10%</td><td>7%</td></tr></table>

## Remark 5.2

A similar formula to (5.2) holds for logarithmic returns, 

$$
\mathrm{e} ^ {k _ {V}} = w _ {1} \mathrm{e} ^ {k _ {1}} + w _ {2} \mathrm{e} ^ {k _ {2}}.\tag{5.3}
$$

However, this is not particularly useful if the expectations and variances or standard deviations of returns need to be related to the weights. On the other hand, as will be seen below, formula (5.2) lends itself well to this task. 

Exercise 5.6 

Verify formula (5.3). 

## 5.2.1 Risk and Expected Return on a Portfolio

The expected return on a portfolio consisting of two securities can easily be expressed in terms of the weights and the expected returns on the components, 

$$
E (K _ {V}) = w _ {1} E (K _ {1}) + w _ {2} E (K _ {2}).\tag{5.4}
$$

This follows at once from (5.2) by the additivity of mathematical expectation. 

## Example 5.5

Consider three scenarios with the probabilities given below (a trinomial model). Let the returns on two diferent stocks in these scenarios be as follows: 

<table><tr><td>Scenario</td><td>Probability</td><td>Return <eq>K_{1}</eq></td><td>Return <eq>K_{2}</eq></td></tr><tr><td><eq>\omega_{1}</eq> (recession)</td><td>0.2</td><td>-10%</td><td>-30%</td></tr><tr><td><eq>\omega_{2}</eq> (stagnation)</td><td>0.5</td><td>0%</td><td>20%</td></tr><tr><td><eq>\omega_{3}</eq> (boom)</td><td>0.3</td><td>10%</td><td>50%</td></tr></table>

The expected returns on stock are 

$$
E (K _ {1}) = - 0. 2 \times 10 \% + 0. 5 \times 0 \% + 0. 3 \times 10 \% = 1 \%,
$$

$$
E (K _ {2}) = - 0. 2 \times 30 \% + 0. 5 \times 20 \% + 0. 3 \times 50 \% = 19 \%.
$$

Suppose that $w _ { 1 } = 6 0 \%$ of available funds is invested in stock 1 and $4 0 \%$ in stock 2. The expected return on such a portfolio is 

$$
\begin{array}{r l} E (K _ {V}) & = w _ {1} E (K _ {1}) + w _ {2} E (K _ {2}) \\ & = 0. 6 \times 1 \% + 0. 4 \times 19 \% = 8. 2 \%. \end{array}
$$

## Exercise 5.7

Compute the weights in a portfolio consisting of two kinds of stock if the expected return on the portfolio is to be $E ( K _ { V } ) = 2 0 \%$ , given the following information on the returns on stock 1 and 2: 

<table><tr><td>Scenario</td><td>Probability</td><td>Return <eq>K_{1}</eq></td><td>Return <eq>K_{2}</eq></td></tr><tr><td><eq>\omega_{1}</eq> (recession)</td><td>0.1</td><td>-10%</td><td>10%</td></tr><tr><td><eq>\omega_{2}</eq> (stagnation)</td><td>0.5</td><td>0%</td><td>20%</td></tr><tr><td><eq>\omega_{3}</eq> (boom)</td><td>0.4</td><td>20%</td><td>30%</td></tr></table>

To compute the variance of $K _ { V }$ we need to know not only the variances of the returns $K _ { 1 }$ and $K _ { 2 }$ on the components in the portfolio, but also the covariance between the two returns. 

## Theorem 5.2

The variance of the return on a portfolio is given by 

$$
\operatorname{Var} (K _ {V}) = w _ {1} ^ {2} \operatorname{Var} (K _ {1}) + w _ {2} ^ {2} \operatorname{Var} (K _ {2}) + 2 w _ {1} w _ {2} \operatorname{Cov} (K _ {1}, K _ {2}).\tag{5.5}
$$

Proof 

Substituting $K _ { V } = w _ { 1 } K _ { 1 } + w _ { 2 } K _ { 2 }$ and collecting the terms with $w _ { 1 } ^ { 2 } , \ w _ { 2 } ^ { 2 }$ and $w _ { 1 } w _ { 2 }$ , we compute 

$$
\begin{array}{r l} & {\mathrm{Var} (K _ {V}) = E (K _ {V} ^ {2}) - E (K _ {V}) ^ {2}} \\ & {\qquad = w _ {1} ^ {2} [ E (K _ {1} ^ {2}) - E (K _ {1}) ^ {2} ] + w _ {2} ^ {2} [ E (K _ {2} ^ {2}) - E (K _ {2}) ^ {2} ]} \\ & {\qquad + 2 w _ {1} w _ {2} [ E (K _ {1} K _ {2}) - E (K _ {1}) E (K _ {2}) ]} \\ & {\qquad = w _ {1} ^ {2} \mathrm{Var} (K _ {1}) + w _ {2} ^ {2} \mathrm{Var} (K _ {2}) + 2 w _ {1} w _ {2} \mathrm{Cov} (K _ {1}, K _ {2}).} \end{array}
$$

To avoid clutter, we introduce the following notation for the expectation and variance of a portfolio and its components: 

$$
\begin{array}{r l} \mu_ {V} = E (K _ {V}), & \sigma_ {V} = \sqrt {\mathrm{Var} (K _ {V})}, \\ \mu_ {1} = E (K _ {1}), & \sigma_ {1} = \sqrt {\mathrm{Var} (K _ {1})}, \\ \mu_ {2} = E (K _ {2}), & \sigma_ {2} = \sqrt {\mathrm{Var} (K _ {2})}. \end{array}
$$

We shall also use the correlation coeficient 

$$
\rho_ {1 2} = \frac {\mathrm{Cov} (K _ {1} , K _ {2})}{\sigma_ {1} \sigma_ {2}}.\tag{5.6}
$$

Formulae (5.4) and (5.5) can be written as 

$$
\mu_ {V} = w _ {1} \mu_ {1} + w _ {2} \mu_ {2},\tag{5.7}
$$

$$
\sigma_ {V} ^ {2} = w _ {1} ^ {2} \sigma_ {1} ^ {2} + w _ {2} ^ {2} \sigma_ {2} ^ {2} + 2 w _ {1} w _ {2} \rho_ {1 2} \sigma_ {1} \sigma_ {2}.\tag{5.8}
$$

## Remark 5.3

For risky securities the returns $K _ { 1 }$ and $K _ { 2 }$ are always assumed to be nonconstant random variables. Because of this $\sigma _ { 1 } , \sigma _ { 2 } > 0$ and $\rho _ { 1 2 }$ is well defined, since the denominator $\sigma _ { 1 } \sigma _ { 2 }$ in (5.6) is non-zero. 

## Example 5.6

We use the following data: 

<table><tr><td>Scenario</td><td>Probability</td><td>Return <eq>K_{1}</eq></td><td>Return <eq>K_{2}</eq></td></tr><tr><td><eq>\omega_{1}</eq> (recession)</td><td>0.4</td><td>-10%</td><td>20%</td></tr><tr><td><eq>\omega_{2}</eq> (stagnation)</td><td>0.2</td><td>0%</td><td>20%</td></tr><tr><td><eq>\omega_{3}</eq> (boom)</td><td>0.4</td><td>20%</td><td>10%</td></tr></table>

We want to compare the risk of a portfolio such that $w _ { 1 } = 4 0 \%$ and $w _ { 2 } =$ 60% with the risks of its components as measured by the variance. Direct computations give 

$$
\sigma_ {1} ^ {2} \cong 0. 0 1 8 4, \quad \sigma_ {2} ^ {2} \cong 0. 0 0 2 4, \quad \rho_ {1 2} \cong - 0. 9 6 3 0 9.
$$

By (5.8) 

$$
\begin{array}{l} \sigma_ {V} ^ {2} \cong (0. 4) ^ {2} \times 0. 0 1 8 4 + (0. 6) ^ {2} \times 0. 0 0 2 4 \\ \qquad + 2 \times 0. 4 \times 0. 6 \times (- 0. 9 6 3 0 9) \times \sqrt {0 . 0 1 8 4} \times \sqrt {0 . 0 0 2 4} \\ \qquad \cong 0. 0 0 0 7 3 6. \end{array}
$$

Observe that the variance $\sigma _ { V } ^ { 2 }$ is smaller than $\sigma _ { 1 } ^ { 2 }$ and $\sigma _ { 2 } ^ { 2 }$ . 

## Example 5.7

Consider another portfolio with weights $w _ { 1 } = 8 0 \%$ and $w _ { 2 } = 2 0 \%$ , all other things being the same as in Example 5.6. Then 

$$
\begin{array}{r l} & {\sigma_ {V} ^ {2} \cong (0. 8) ^ {2} \times 0. 0 1 8 4 + (0. 2) ^ {2} \times 0. 0 0 2 4} \\ & {\qquad + 2 \times 0. 8 \times 0. 2 \times (- 0. 9 6 3 0 9) \times \sqrt {0 . 0 1 8 4} \times \sqrt {0 . 0 0 2 4}} \\ & {\qquad \cong 0. 0 0 9 8 2 4,} \end{array}
$$

which is between $\sigma _ { 1 } ^ { 2 }$ and $\sigma _ { 2 } ^ { 2 }$ 

## Proposition 5.3

The variance $\sigma _ { V } ^ { 2 }$ of a portfolio cannot exceed the greater of the variances $\sigma _ { 1 } ^ { 2 }$ and $\sigma _ { 2 } ^ { 2 }$ of the components, 

$$
\sigma_ {V} ^ {2} \leq \max \{\sigma_ {1} ^ {2}, \sigma_ {2} ^ {2} \},
$$

if short sales are not allowed. 

## Proof

Let us assume that $\sigma _ { 1 } ^ { 2 } \le \sigma _ { 2 } ^ { 2 }$ . If short sales are not allowed, then $w _ { 1 } , w _ { 2 } \geq 0$ and 

$$
w _ {1} \sigma_ {1} + w _ {2} \sigma_ {2} \leq (w _ {1} + w _ {2}) \sigma_ {2} = \sigma_ {2}.
$$

Since the correlation coeficient satisfies $- 1 \le \rho _ { 1 2 } \le 1$ , it follows that 

$$
\begin{array}{r l} & {\sigma_ {V} ^ {2} = w _ {1} ^ {2} \sigma_ {1} ^ {2} + w _ {2} ^ {2} \sigma_ {2} ^ {2} + 2 w _ {1} w _ {2} \rho_ {1 2} \sigma_ {1} \sigma_ {2}} \\ & {\qquad \leq w _ {1} ^ {2} \sigma_ {1} ^ {2} + w _ {2} ^ {2} \sigma_ {2} ^ {2} + 2 w _ {1} w _ {2} \sigma_ {1} \sigma_ {2}} \\ & {\qquad = (w _ {1} \sigma_ {1} + w _ {2} \sigma_ {2}) ^ {2} \leq \sigma_ {2} ^ {2}.} \end{array}
$$

If $\sigma _ { 1 } ^ { 2 } \geq \sigma _ { 2 } ^ { 2 }$ , the proof is analogous. 

## Example 5.8

Now consider a portfolio with weights $w _ { 1 } = - 5 0 \%$ and $w _ { 2 } = 1 5 0 \%$ (allowing short sales of security 1), all the other data being the same as in Example 5.6. The variance of this portfolio is 

$$
\begin{array}{r l} & {\sigma_ {V} ^ {2} \cong (- 0. 5) ^ {2} \times 0. 0 1 8 4 + (1. 5) ^ {2} \times 0. 0 0 2 4} \\ & {\qquad + 2 \times (- 0. 5) \times 1. 5 \times (- 0. 9 6 3 0 9) \times \sqrt {0 . 0 1 8 4} \times \sqrt {0 . 0 0 2 4}} \\ & {\qquad \cong 0. 0 1 9 6,} \end{array}
$$

which is greater than both $\sigma _ { 1 } ^ { 2 }$ and $\sigma _ { 2 } ^ { 2 }$ . 

## Exercise 5.8

Using the data in Example 5.6, find the weights in a portfolio with expected return $\mu _ { V } = 4 6 \%$ and compute the risk $\sigma _ { V } ^ { 2 }$ of this portfolio. 

The correlation coeficient always satisfies $- 1 \le \rho _ { 1 2 } \le 1$ . The next proposition is concerned with the two special cases when $\rho _ { 1 2 }$ assumes one of the extreme values 1 or 1, which means perfect positive or negative correlation between the securities in the portfolio. 

## Proposition 5.4

If $\rho _ { 1 2 } = 1$ , then $\sigma _ { V } = 0$ when $\sigma _ { 1 } \neq \sigma _ { 2 }$ and 

$$
w _ {1} = - \frac {\sigma_ {2}}{\sigma_ {1} - \sigma_ {2}}, w _ {2} = \frac {\sigma_ {1}}{\sigma_ {1} - \sigma_ {2}}.\tag{5.9}
$$

(Short sales are necessary, since either $w _ { 1 }$ or $w _ { 2 }$ is negative.) 

If $\rho _ { 1 2 } = - 1$ , then $\sigma _ { V } = 0$ for 

$$
w _ {1} = \frac {\sigma_ {2}}{\sigma_ {1} + \sigma_ {2}}, w _ {2} = \frac {\sigma_ {1}}{\sigma_ {1} + \sigma_ {2}}.\tag{5.10}
$$

(No short sales are necessary, since both $w _ { 1 }$ and $w _ { 2 }$ are positive.) 

## Proof

Let $\rho _ { 1 2 } = 1$ . Then (5.8) takes the form 

$$
\sigma_ {V} ^ {2} = w _ {1} ^ {2} \sigma_ {1} ^ {2} + w _ {2} ^ {2} \sigma_ {2} ^ {2} + 2 w _ {1} w _ {2} \sigma_ {1} \sigma_ {2} = (w _ {1} \sigma_ {1} + w _ {2} \sigma_ {2}) ^ {2}
$$

and $\sigma _ { V } ^ { 2 } = 0$ if and only if $w _ { 1 } \sigma _ { 1 } + w _ { 2 } \sigma _ { 2 } = 0$ . This is equivalent to $\sigma _ { 1 } \neq \sigma _ { 2 }$ and (5.9) because $w _ { 1 } + w _ { 2 } = 1$ 

Now let $\rho _ { 1 2 } = - 1$ . Then (5.8) becomes 

$$
\sigma_ {V} ^ {2} = w _ {1} ^ {2} \sigma_ {1} ^ {2} + w _ {2} ^ {2} \sigma_ {2} ^ {2} - 2 w _ {1} w _ {2} \sigma_ {1} \sigma_ {2} = (w _ {1} \sigma_ {1} - w _ {2} \sigma_ {2}) ^ {2}
$$

and $\sigma _ { V } ^ { 2 } = 0$ if and only if $w _ { 1 } \sigma _ { 1 } - w _ { 2 } \sigma _ { 2 } = 0$ . The last equality is equivalent to (5.10) because $w _ { 1 } + w _ { 2 } = 1$ □ 

Each portfolio can be represented by a point with coordinates $\sigma _ { V }$ and $\mu _ { V }$ on the $\sigma , \mu$ plane. Figure 5.1 shows two typical lines representing portfolios with $\rho _ { 1 2 } = - 1$ (left) and $\rho _ { 1 2 } = 1$ (right). The bold segments correspond to portfolios without short selling 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/14364d1effd67143756a44c8e938b571efdbdb02f130b030402a7791aa43ccdd.jpg)



Figure 5.1 Typical portfolio lines with $\rho _ { 1 2 } = - 1$ and 1


Suppose that $\rho _ { 1 2 } = - 1$ . It follows from the proof of Proposition 5.4 that $\sigma _ { V } = | w _ { 1 } \sigma _ { 1 } - w _ { 2 } \sigma _ { 2 } |$ . In addition, $\mu _ { V } = w _ { 1 } \mu _ { 1 } + w _ { 2 } \mu _ { 2 }$ by (5.7) and $w _ { 1 } + w _ { 2 } = 1$ by (5.1). We can choose $s = w _ { 2 }$ as a parameter. Then $1 - s = w _ { 1 }$ and 

$$
\begin{array}{l} \sigma_ {V} = | (1 - s) \sigma_ {1} - s \sigma_ {2} |, \\ \mu_ {V} = (1 - s) \mu_ {1} + s \mu_ {2}. \end{array}
$$

These parametric equations describe the line in Figure 5.1 with a broken segment between $( \sigma _ { 1 } , \mu _ { 1 } )$ and $( \sigma _ { 2 } , \mu _ { 2 } )$ . As s increases, the point $( \sigma _ { V } , \mu _ { V } )$ moves along the line in the direction from $( \sigma _ { 1 } , \mu _ { 1 } )$ to $( \sigma _ { 2 } , \mu _ { 2 } )$ 

If $\rho _ { 1 2 } = 1$ , then $\sigma _ { V } = | w _ { 1 } \sigma _ { 1 } + w _ { 2 } \sigma _ { 2 } |$ . We choose $s = w _ { 2 }$ as a parameter once again, and obtain the parametric equations 

$$
\begin{array}{l} \sigma_ {V} = | (1 - s) \sigma_ {1} + s \sigma_ {2} |, \\ \mu_ {V} = (1 - s) \mu_ {1} + s \mu_ {2} \end{array}
$$

of the line in Figure 5.1 with a straight segment between $( \sigma _ { 1 } , \mu _ { 1 } )$ and $( \sigma _ { 2 } , \mu _ { 2 } )$ 

If no short selling is allowed, then $0 \leq s \leq 1$ in both cases, which corresponds to the bold line segments. 

## Exercise 5.9

Suppose that there are just two scenarios $\omega _ { 1 }$ and $\omega _ { 2 }$ and consider two risky securities with returns $K _ { 1 }$ and $K _ { 2 }$ . Show that $K _ { 1 } = a K _ { 2 } + b$ for some numbers $a \neq 0$ and b, and deduce that $\rho _ { 1 2 } = 1 ~ \mathrm { o r } ~ { - 1 }$ 

Our next task is to find a portfolio with minimum risk for any given $\rho _ { 1 2 }$ such that $- 1 < \rho _ { 1 2 } < 1$ . Again, we take $s = w _ { 2 }$ as a parameter. Then (5.7) 

and (5.8) take the form 

$$
\mu_ {V} = (1 - s) \mu_ {1} + s \mu_ {2},\tag{5.11}
$$

$$
\sigma_ {V} ^ {2} = (1 - s) ^ {2} \sigma_ {1} ^ {2} + s ^ {2} \sigma_ {2} ^ {2} + 2 s (1 - s) \rho_ {1 2} \sigma_ {1} \sigma_ {2}.\tag{5.12}
$$

Obviously, $\mu _ { V }$ as a function of s is a straight line and $\sigma _ { V } ^ { 2 }$ is a quadratic function of s with a positive coeficient at $s ^ { 2 }$ (namely $\sigma _ { 1 } ^ { 2 } + \sigma _ { 2 } ^ { 2 } - 2 \rho _ { 1 2 } \sigma _ { 1 } \sigma _ { 2 } > \sigma _ { 1 } ^ { 2 } + \sigma _ { 2 } ^ { 2 } -$ $2 \sigma _ { 1 } \sigma _ { 2 } = ( \sigma _ { 1 } - \sigma _ { 2 } ) ^ { 2 } \geq 0 )$ . The problem of minimising the variance $\sigma _ { V } ^ { 2 }$ (or, equivalently, the standard deviation $\sigma _ { V } )$ of a portfolio is solved in the next theorem. First we find the minimum without any restrictions on short sales. If short sales are not allowed, we shall have to take into account the bounds $0 \leq s \leq 1$ on the parameter. 

## Theorem 5.5

For $- 1 < \rho _ { 1 2 } < 1$ the portfolio with minimum variance is attained at 

$$
s _ {0} = \frac {\sigma_ {1} ^ {2} - \rho_ {1 2} \sigma_ {1} \sigma_ {2}}{\sigma_ {1} ^ {2} + \sigma_ {2} ^ {2} - 2 \rho_ {1 2} \sigma_ {1} \sigma_ {2}}.\tag{5.13}
$$

If short sales are not allowed, then the smallest variance is attained at 

$$
s _ {\min} = \left\{ \begin{array}{l l} 0 & \text {if s_{0} <   0 ,} \\ s _ {0} & \text {if 0\leq s_{0} \leq 1 ,} \\ 1 & \text {if 1<   s_{0} .} \end{array} \right.
$$

## Proof

We compute the derivative of $\sigma _ { V } ^ { 2 }$ with respect to s and equate it to 0: 

$$
- 2 (1 - s) \sigma_ {1} ^ {2} + 2 s \sigma_ {2} ^ {2} + 2 (1 - s) \rho_ {1 2} \sigma_ {1} \sigma_ {2} - 2 s \rho_ {1 2} \sigma_ {1} \sigma_ {2} = 0.
$$

Solving for s gives the above $s _ { 0 }$ . The second derivative is positive, 

$$
2 \sigma_ {1} ^ {2} + 2 \sigma_ {2} ^ {2} - 4 \rho_ {1 2} \sigma_ {1} \sigma_ {2} > 2 \sigma_ {1} ^ {2} + 2 \sigma_ {2} ^ {2} - 4 \sigma_ {1} \sigma_ {2} = 2 (\sigma_ {1} - \sigma_ {2}) ^ {2} \geq 0,
$$

which shows that there is a minimum at $s _ { 0 }$ . It is a global minimum because $\sigma _ { V } ^ { 2 }$ is a quadratic function of s. 

If short sales are not allowed, then we need to find the minimum for $0 \leq$ $s \leq 1$ . If $0 \leq s _ { 0 } \leq 1$ , then the minimum is at $s _ { 0 }$ . If $s _ { 0 } < 0$ , then the minimum is at 0, and if $s _ { 0 } > 1$ , then it is at 1, since $\sigma _ { V } ^ { 2 }$ is a quadratic function of s with a positive coeficient at $s ^ { 2 }$ . This is illustrated in Figure 5.2. The bold parts of the curve correspond to portfolios with no short selling. □ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/12751ce389473dab1cf2a0c4359c1445be36b3696d9cdfcd6eee122ad38ecc2d.jpg)



Figure 5.2 The minimum of $\sigma _ { V } ^ { 2 }$ as a function of s


The line on the $\sigma , \mu$ plane defined by the parametric equations (5.11) and (5.12) represents all possible portfolios with given $\sigma _ { 1 } , \sigma _ { 2 } > 0$ and $- 1 \le \rho _ { 1 2 } \le 1$ The parameter s can be any real number whenever there are no restrictions on short selling. If short selling is not allowed, then $0 \leq s \leq 1$ and we only obtain a segment of the line. As s increases from 0 to 1, the corresponding point $( \sigma _ { V } , \mu _ { V } )$ travels along the line in the direction from $( \sigma _ { 1 } , \mu _ { 1 } )$ to $( \sigma _ { 2 } , \mu _ { 2 } )$ ). Figure 5.3 shows two typical examples of such lines, with $\rho _ { 1 2 }$ close to but greater than 1 (left) and with $\rho _ { 1 2 }$ close to but smaller than 1 (right). Portfolios without short selling are indicated by the bold line segments. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/20ba25bd6bafed05773f109573e9cb120f08dcdb7b9d94de4a52869f65d53f74.jpg)



Figure 5.3 Typical portfolio lines with $- 1 < \rho _ { 1 2 } < 1$


Figure 5.4 illustrates the following corollary. 

## Corollary 5.6

Suppose that $\sigma _ { 1 } \leq \sigma _ { 2 }$ . The following three cases are possible: 

1) If $\begin{array} { r } { - 1 \le \rho _ { 1 2 } < \frac { \sigma _ { 1 } } { \sigma _ { 2 } } } \end{array}$ , then there is a portfolio without short selling such tha $\sigma _ { V } < \sigma _ { 1 }$ (lines 4 and 5 in Figure 5.4); 

2) If $\textstyle \rho _ { 1 2 } = { \frac { \sigma _ { 1 } } { \sigma _ { 2 } } }$ , then $\sigma _ { V } \geq \sigma _ { 1 }$ for each portfolio (line 3 in Figure 5.4); 

3) If $\begin{array} { r } { \frac { \sigma _ { 1 } } { \sigma _ { 2 } } \ < \ \rho _ { 1 2 } \ \le \ 1 } \end{array}$ , then there is a portfolio with short selling such that $\sigma _ { V } < \sigma _ { 1 }$ , but for each portfolio without short selling $\sigma _ { V } \geq \sigma _ { 1 }$ (lines 1 and 2 in Figure 5.4). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/58b665c53017f33f54f661f34e86384fc9a89444bec0c9ab026eb81ad2b31881.jpg)



Figure 5.4 Portfolio lines for various values of $\rho _ { 1 2 }$


## Proof

1) If $\begin{array} { r } { - 1 \le \rho _ { 1 2 } < \frac { \sigma _ { 1 } } { \sigma _ { 2 } } } \end{array}$ , then $\begin{array} { r } { \frac { \sigma _ { 1 } } { \sigma _ { 1 } + \sigma _ { 2 } } > s _ { 0 } > 0 } \end{array}$ . But $\begin{array} { r } { \frac { \sigma _ { 1 } } { \sigma _ { 1 } + \sigma _ { 2 } } < 1 } \end{array}$ , so $0 < s _ { 0 } < 1$ , which means that the portfolio with minimum variance, which corresponds to the parameter $s _ { 0 }$ , involves no short selling and satisfies $\sigma _ { V } < \sigma _ { 1 }$ 

2) If $\begin{array} { r } { \rho _ { 1 2 } = \frac { \sigma _ { 1 } } { \sigma _ { 2 } } } \end{array}$ , then $s _ { 0 } = 0$ . As a result, $\sigma _ { V } \geq \sigma _ { 1 }$ for every portfolio because $\sigma _ { 1 } ^ { 2 }$ is the minimum variance. 

3) Finally, if $\begin{array} { r } { \frac { \sigma _ { 1 } } { \sigma _ { 2 } } < \rho _ { 1 2 } \le 1 } \end{array}$ , then $s _ { 0 } < 0$ . In this case the portfolio with minimum variance that corresponds to $s _ { 0 }$ involves short selling of security 1 and satisfies $\sigma _ { V } < \sigma _ { 1 }$ . For $s \geq s _ { 0 }$ the variance $\sigma _ { V }$ is an increasing function of $s ,$ which means that $\sigma _ { V } > \sigma _ { 1 }$ for every portfolio without short selling. □ 

The above corollary is important because it shows when it is possible to construct a portfolio with risk lower than that of any of its components. In case 1) this is possible without short selling. In case 3) this is also possible, but only if short selling is allowed. In case 2) it is impossible to construct such a portfolio. 

## Example 5.9

Suppose that 

$$
\sigma_ {1} ^ {2} = 0. 0 0 4 1, \quad \sigma_ {2} ^ {2} = 0. 0 1 2 1, \quad \rho_ {1 2} = 0. 9 7 9 6.
$$

Clearly, $\sigma _ { 1 } < \sigma _ { 2 }$ and $\begin{array} { r } { \frac { \sigma _ { 1 } } { \sigma _ { 2 } } < \rho _ { 1 2 } < 1 } \end{array}$ , so this is case 3) in Corollary 5.6. Our task will be to find the portfolio with minimum risk with and without short selling. 

Using Theorem 5.5, we compute 

$$
s _ {0} \cong - 1. 1 6 6 3, s _ {\mathrm{min}} = 0.
$$

It follows that in the portfolio with minimum risk the weights of securities should be $w _ { 1 } \cong 2 . 1 6 6 3$ and $w _ { 2 } \cong - 1 . 1 6 6 3$ if short selling is allowed. Without short selling $w _ { 1 } = 1$ and $w _ { 2 } = 0$ 

## Exercise 5.10

Compute the weights in the portfolio with minimum risk for the data in Example 5.6. Does this portfolio involve short selling? 

We conclude this section with a brief discussion of portfolios in which one of the securities is risk-free. The variance of the risky security (a stock) is positive, whereas that of the risk-free component (a bond) is zero. 

## Proposition 5.7

The standard deviation $\sigma _ { V }$ of a portfolio consisting of a risky security with expected return $\mu _ { 1 }$ and standard deviation $\sigma _ { 1 } > 0$ , and a risk-free security with return $r _ { F }$ and standard deviation zero depends on the weight $w _ { 1 }$ of the risky security as follows: 

$$
\sigma_ {V} = | w _ {1} | \sigma_ {1}.
$$

## Proof

Let $\sigma _ { 1 } > 0$ and $\sigma _ { 2 } = 0$ . Then (5.7) reduces to $\sigma _ { V } ^ { 2 } = w _ { 1 } ^ { 2 } \sigma _ { 1 } ^ { 2 }$ , and the formula for $\sigma _ { V }$ follows by taking the square root. □ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/bac85727e636237b694b4f46ba1da7250a8afc4b3bb65f9be31a13ff0ceca5cb.jpg)



Figure 5.5 Portfolio line for one risky and one risk-free security


The line on the $\sigma , \mu$ plane representing portfolios constructed from one risky and one risk-free security is shown in Figure 5.5. As usual, the bold line segment corresponds to portfolios without short selling. 

## 5.3 Several Securities

## 5.3.1 Risk and Expected Return on a Portfolio

A portfolio constructed from n diferent securities can be described in terms of their weights 

$$
w _ {i} = \frac {x _ {i} S _ {i} (0)}{V (0)}, \quad i = 1, \dots , n,
$$

where $x _ { i }$ is the number of shares of type $i$ in the portfolio, $S _ { i } ( 0 )$ is the initial price of security i, and $V ( 0 )$ is the amount initially invested in the portfolio. It will prove convenient to arrange the weights into a one-row matrix 

$$
\pmb {w} = \left[ \begin{array}{l l l l} w _ {1} & w _ {2} & \dots & w _ {n} \end{array} \right].
$$

Just like for two securities, the weights add up to one, which can be written in matrix form as 

$$
1 = \pmb {u} \pmb {w} ^ {T},\tag{5.14}
$$

where 

$$
\boldsymbol {u} = \left[ \begin{array}{l l l l} 1 & 1 & \dots & 1 \end{array} \right]
$$

is a one-row matrix with all n entries equal to 1, $\mathbf { \Delta } w ^ { T }$ is a one-column matrix, the transpose of ${ \pmb w } _ { \mathrm { : } }$ , and the usual matrix multiplication rules apply. The attainable set consists of all portfolios with weights w satisfying (5.14), called the attainable portfolios. 

Suppose that the returns on the securities are $K _ { 1 } , \ldots , K _ { n }$ . The expected returns $\mu _ { i } = E ( K _ { i } )$ for $i = 1 , \ldots , n$ will also be arranged into a one-row matrix 

$$
\boldsymbol {m} = \left[ \begin{array}{l l l l} \mu_ {1} & \mu_ {2} & \dots & \mu_ {n} \end{array} \right].
$$

The covariances between returns will be denoted by $c _ { i j } = \operatorname { C o v } ( K _ { i } , K _ { j } )$ . They are the entries of the $n \times n$ covariance matrix 

$$
\boldsymbol {C} = \left[ \begin{array}{c c c c} c _ {1 1} & c _ {1 2} & \dots & c _ {1 n} \\ c _ {2 1} & c _ {2 2} & \dots & c _ {2 n} \\ \vdots & \vdots & \ddots & \vdots \\ c _ {n 1} & c _ {n 2} & \dots & c _ {n n} \end{array} \right].
$$

It is well known that the covariance matrix is symmetric and positive definite. The diagonal elements are simply the variances of returns, $c _ { i i } = \mathrm { V a r } ( K _ { i } )$ . In what follows we shall assume, in addition, that C has an inverse $C ^ { - 1 }$ 

## Proposition 5.8

The expected return $\mu _ { V } = E ( K _ { V } )$ and variance $\sigma _ { V } ^ { 2 } = \operatorname { V a r } ( K _ { V } )$ of a portfolio with weights w are given by 

$$
\mu_ {V} = \pmb {m} \pmb {w} ^ {T},\tag{5.15}
$$

$$
\sigma_ {V} ^ {2} = \boldsymbol {w} \boldsymbol {C} \boldsymbol {w} ^ {T}.\tag{5.16}
$$

## Proof

The formula for $\mu _ { V }$ follows by the linearity of expectation, 

$$
\mu_ {V} = E (K _ {V}) = E \left(\sum_ {i = 1} ^ {n} w _ {i} K _ {i}\right) = \sum_ {i = 1} ^ {n} w _ {i} \mu_ {i} = \boldsymbol {m} \boldsymbol {w} ^ {T}.
$$

For $\sigma _ { V } ^ { 2 }$ we use the linearity of covariance with respect to each of its arguments, 

$$
\begin{array}{l} \sigma_ {V} ^ {2} = \operatorname{Var} (K _ {V}) = \operatorname{Var} \left(\sum_ {i = 1} ^ {n} w _ {i} K _ {i}\right) \\ \qquad = \operatorname{Cov} \left(\sum_ {i = 1} ^ {n} w _ {i} K _ {i}, \sum_ {j = 1} ^ {n} w _ {j} K _ {j}\right) = \sum_ {i, j = 1} ^ {n} w _ {i} w _ {j} c _ {i j} \\ \qquad = \boldsymbol {w} \boldsymbol {C} \boldsymbol {w} ^ {T}. \end{array}
$$

## Exercise 5.11

Compute the expected return $\mu _ { V }$ and standard deviation $\sigma _ { V }$ of a portfolio consisting of three securities with weights $w _ { 1 } = 4 0 \% , w _ { 2 } = - 2 0 \%$ , $w _ { 3 } = 8 0 \%$ , given that the securities have expected returns $\mu _ { 1 } = 8 \%$ , $\mu _ { 2 } = 1 0 \% , \mu _ { 3 } = 6 \%$ , standard deviations $\sigma _ { 1 } = 1 . 5 , \sigma _ { 2 } = 0 . 5 , \sigma _ { 3 } = 1 . 2$ and correlations $\rho _ { 1 2 } = 0 . 3 , \rho _ { 2 3 } = 0 . 0 , \rho _ { 3 1 } = - 0 . 2$ 

We shall solve the following two problems: 

1. To find a portfolio with the smallest variance in the attainable set. It will be called the minimum variance portfolio. 

2. To find a portfolio with the smallest variance among all portfolios in the attainable set whose expected return is equal to a given number $\mu _ { V }$ . The family of such portfolios, parametrised by $\mu _ { V }$ , is called the minimum variance line. 

Since the variance is a continuous function of the weights, bounded below by 0, the minimum clearly exists in both cases. 

## Proposition 5.9 (Minimum Variance Portfolio)

The portfolio with the smallest variance in the attainable set has weights 

$$
\pmb {w} = \frac {\pmb {u} C ^ {- 1}}{\pmb {u} C ^ {- 1} \pmb {u} ^ {T}},
$$

provided that the denominator is non-zero. 

## Proof

We need to find the minimum of (5.16) subject to the constraint (5.14). To this end we can use the method of Lagrange multipliers. Let us put 

$$
F (\boldsymbol {w}, \lambda) = \boldsymbol {w} \boldsymbol {C} \boldsymbol {w} ^ {T} - \lambda \boldsymbol {u} \boldsymbol {w} ^ {T},
$$

where λ is a Lagrange multiplier. Equating to zero the partial derivatives of F with respect to the weights $w _ { i }$ we obtain $2 w C - \lambda u = 0$ , that is, 

$$
\pmb {w} = \frac {\lambda}{2} \pmb {u} C ^ {- 1},
$$

which is a necessary condition for a minimum. Substituting this into constraint (5.14) we obtain 

$$
1 = \frac {\lambda}{2} \boldsymbol {u} \boldsymbol {C} ^ {- 1} \boldsymbol {u} ^ {T},
$$

where we use the fact that $C ^ { - 1 }$ is a symmetric matrix because C is. Solving this for λ and substituting the result into the expression for w will give the asserted formula. □ 

## Proposition 5.10 (Minimum Variance Line)

The portfolio with the smallest variance among attainable portfolios with ex pected return $\mu _ { V }$ has weights 

$$
\boldsymbol {w} = \frac {\left| \begin{array}{c c} 1 & \boldsymbol {u} \boldsymbol {C} ^ {- 1} \boldsymbol {m} ^ {T} \\ \mu_ {V} & \boldsymbol {m} \boldsymbol {C} ^ {- 1} \boldsymbol {m} ^ {T} \end{array} \right| \boldsymbol {u} \boldsymbol {C} ^ {- 1} + \left| \begin{array}{c c} \boldsymbol {u} \boldsymbol {C} ^ {- 1} \boldsymbol {u} ^ {T} & 1 \\ \boldsymbol {m} \boldsymbol {C} ^ {- 1} \boldsymbol {u} ^ {T} & \mu_ {V} \end{array} \right| \boldsymbol {m} \boldsymbol {C} ^ {- 1}}{\left| \begin{array}{c c} \boldsymbol {u} \boldsymbol {C} ^ {- 1} \boldsymbol {u} ^ {T} & \boldsymbol {u} \boldsymbol {C} ^ {- 1} \boldsymbol {m} ^ {T} \\ \boldsymbol {m} \boldsymbol {C} ^ {- 1} \boldsymbol {u} ^ {T} & \boldsymbol {m} \boldsymbol {C} ^ {- 1} \boldsymbol {m} ^ {T} \end{array} \right|},
$$

provided that the determinant in the denominator is non-zero. The weights depend linearly on $\mu _ { V }$ 

## Proof

Here we need to find the minimum of (5.16) subject to two constraints (5.14) and (5.15). We take 

$$
G (\boldsymbol {w}, \lambda , \mu) = \boldsymbol {w} \boldsymbol {C} \boldsymbol {w} ^ {T} - \lambda \boldsymbol {u} \boldsymbol {w} ^ {T} - \mu \boldsymbol {m} \boldsymbol {w} ^ {T},
$$

where λ and $\mu$ are Lagrange multipliers. The partial derivatives of $G$ with respect to the weights $w _ { i }$ equated to zero give a necessary condition for a minimum, $2 w C - \lambda u - \mu m = 0$ , which implies that 

$$
\boldsymbol {w} = \frac {\lambda}{2} \boldsymbol {u} \boldsymbol {C} ^ {- 1} + \frac {\mu}{2} \boldsymbol {m} \boldsymbol {C} ^ {- 1}.
$$

Substituting this into the constraints (5.14) and (5.15), we obtain a system of linear equations 

$$
\begin{array}{c} {1 = \frac {\lambda}{2} \pmb {u} \pmb {C} ^ {- 1} \pmb {u} ^ {T} + \frac {\mu}{2} \pmb {u} \pmb {C} ^ {- 1} \pmb {m} ^ {T},} \\ {\mu_ {V} = \frac {\lambda}{2} \pmb {m} \pmb {C} ^ {- 1} \pmb {u} ^ {T} + \frac {\mu}{2} \pmb {m} \pmb {C} ^ {- 1} \pmb {m} ^ {T},} \end{array}
$$

to be solved for λ and $\mu .$ . The asserted formula follows by substituting the solution into the expression for w. □ 

## Example 5.10

(3 securities) Consider three securities with expected returns, standard devia tions of returns and correlations between returns 

$$
\begin{array}{l l l} \mu_ {1} = 0. 1 0, & \sigma_ {1} = 0. 2 8, & \rho_ {1 2} = \rho_ {2 1} = - 0. 1 0, \\ \mu_ {2} = 0. 1 5, & \sigma_ {2} = 0. 2 4, & \rho_ {2 3} = \rho_ {3 2} = 0. 2 0, \\ \mu_ {3} = 0. 2 0, & \sigma_ {3} = 0. 2 5, & \rho_ {3 1} = \rho_ {1 3} = 0. 2 5. \end{array}
$$

We arrange the $\mu _ { i } \mathrm { { ^ { s } } }$ into a one-row matrix m and 1’s into a one-row matrix ${ \mathbf { } } ^ { \mathbf { } } \mathbf { \Delta } \mathbf { u } ,$ 

$$
\boldsymbol {m} = \left[ \begin{array}{c c c} 0. 1 0 & 0. 1 5 & 0. 2 0 \end{array} \right], \quad \boldsymbol {u} = \left[ \begin{array}{c c c} 1 & 1 & 1 \end{array} \right].
$$

Next we compute the entries $c _ { i j } = \rho _ { i j } \sigma _ { i } \sigma _ { j }$ of the covariance matrix $C _ { i }$ , and find the inverse matrix to $C$ 

$$
\boldsymbol {C} \cong \left[ \begin{array}{c c c} 0. 0 7 8 4 & - 0. 0 0 6 7 & 0. 0 1 7 5 \\ - 0. 0 0 6 7 & 0. 0 5 7 6 & 0. 0 1 2 0 \\ 0. 0 1 7 5 & 0. 0 1 2 0 & 0. 0 6 2 5 \end{array} \right], \boldsymbol {C} ^ {- 1} \cong \left[ \begin{array}{c c c} 1 3. 9 5 4 & 2. 5 4 4 & - 4. 3 9 6 \\ 2. 5 4 4 & 1 8. 5 4 8 & - 4. 2 7 4 \\ - 4. 3 9 6 & - 4. 2 7 4 & 1 8. 0 5 1 \end{array} \right]
$$

From Proposition 5.9 we can compute the weights in the minimum variance portfolio. Since 

$$
\begin{array}{c} \boldsymbol {u} \boldsymbol {C} ^ {- 1} \cong \left[ \begin{array}{c c c} 1 2. 1 0 2 & 1 6. 8 1 8 & 9. 3 8 2 \end{array} \right], \\ \boldsymbol {u} \boldsymbol {C} ^ {- 1} \boldsymbol {u} ^ {T} \cong 3 8. 3 0 2, \end{array}
$$

we obtain 

$$
\boldsymbol {w} = \frac {\boldsymbol {u} \boldsymbol {C} ^ {- 1}}{\boldsymbol {u} \boldsymbol {C} ^ {- 1} \boldsymbol {u} ^ {T}} \cong \left[ \begin{array}{l l l} 0. 3 1 6 & 0. 4 3 9 & 0. 2 4 5 \end{array} \right].
$$

The expected return and standard deviation of this portfolio are 

$$
\mu_ {V} = \pmb {m} \pmb {w} ^ {T} \cong 0. 1 4 6, \quad \sigma_ {V} = \sqrt {\pmb {w} \pmb {C} \pmb {w} ^ {T}} \cong 0. 1 6 2.
$$

The minimum variance line can be computed using Proposition 5.10. To this end we compute 

$$
\boldsymbol {u} \boldsymbol {C} ^ {- 1} \cong \left[ \begin{array}{l l l} 1 2. 1 0 2 & 1 6. 8 1 8 & 9. 3 8 2 \end{array} \right],
$$

$$
\boldsymbol {m} \boldsymbol {C} ^ {- 1} \cong \left[ \begin{array}{c c c} 0. 8 9 8 & 2. 1 8 2 & 2. 5 3 0 \end{array} \right],
$$

$$
\boldsymbol {u} \boldsymbol {C} ^ {- 1} \boldsymbol {u} ^ {T} \cong 3 8. 3 0 2, \quad \boldsymbol {m} \boldsymbol {C} ^ {- 1} \boldsymbol {m} ^ {T} \cong 0. 9 2 3,
$$

$$
\pmb {u} \pmb {C} ^ {- 1} \pmb {m} ^ {T} = \pmb {m} \pmb {C} ^ {- 1} \pmb {u} ^ {T} \cong 5. 6 0 9.
$$

Substituting these into the formula for w in Proposition 5.10, we obtain the weights in the portfolio with minimum variance among all portfolios with ex pected return $\mu _ { V } :$ 

$$
\boldsymbol {w} \cong \left[ \begin{array}{c c c} 1. 5 7 8 - 8. 6 1 4 \mu_ {V} & 0. 8 4 5 - 2. 7 6 9 \mu_ {V} & - 1. 4 2 2 + 1 1. 3 8 4 \mu_ {V} \end{array} \right].
$$

The standard deviation of this portfolio is 

$$
\sigma_ {V} = \sqrt {\pmb {w} \pmb {C} \pmb {w} ^ {T}} \cong \sqrt {0 . 2 3 7 - 2 . 8 8 5 \mu_ {V} + 9 . 8 5 0 \mu_ {V} ^ {2}}.
$$

## Exercise 5.12

Among all attainable portfolios constructed using three securities with expected returns $\mu _ { 1 } = 0 . 2 0 , \mu _ { 2 } = 0 . 1 3 , \mu _ { 3 } = 0 . 1 7$ , standard deviations of returns $\sigma _ { 1 } = 0 . 2 5 , \sigma _ { 2 } = 0 . 2 8 , \sigma _ { 3 } = 0 . 2 0$ , and correlations between returns $\rho _ { 1 2 } = 0 . 3 0 , \rho _ { 2 3 } = 0 . 0 0 , \rho _ { 3 1 } = 0 . 1 5$ , find the minimum variance portfolio. What are the weights in this portfolio? Also compute the expected return and standard deviation of this portfolio. 

## Exercise 5.13

Among all attainable portfolios with expected return $\mu _ { V } = 2 0 \%$ constructed using the three securities in Exercise 5.12 find the portfolio with the smallest variance. Compute the weights and the standard deviation of this portfolio. 

## Example 5.11

(3 securities visualised) There are two convenient ways to visualise all portfolios that can be constructed from the three securities in Example 5.10. One is presented in Figure 5.6. Here two of the three weights, namely $w _ { 2 }$ and $w _ { 3 }$ , 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/e9466b7dbd38e7dc00a68c7a4c435d7e103d2635fdd114ce58f785e781929132.jpg)



Figure 5.6 Attainable portfolios on the $w _ { 2 } , w _ { 3 }$ plane


are used as parameters. The remaining weight is given by $w _ { 1 } = 1 - w _ { 2 } -$ $w _ { 3 }$ . (Of course any other two weights can also be used as parameters.) Each point on the $w _ { 2 } , w _ { 3 }$ plane represents a diferent portfolio. The vertices of the triangle represent the portfolios consisting of only one of the three securities. For example, the vertex with coordinates (1, 0) corresponds to weights $w _ { 1 } = 0 , w _ { 2 } =$ 1 and $w _ { 3 } = 0$ , that is, represents a portfolio with all money invested in security number 2. The lines through the vertices correspond to portfolios consisting of two securities only. For example, the line through (1, 0) and (0, 1) corresponds to portfolios containing securities 2 and 3 only. Points inside the triangle, including the boundaries, correspond to portfolios without short selling. For example, $\textstyle { \left( { \frac { 2 } { 5 } } , { \frac { 1 } { 2 } } \right) }$ represents a portfolio with 10% of the initial funds invested in security 1, 40% in security 2, and 50% in security 3. Points outside the triangle correspond to portfolios with one or two of the three securities shorted. The minimum variance line is a straight line because of the linear dependence of the weights on the expected return. It is represented by the bold line in Figure 5.6. 

Figure 5.7 shows another way to visualise attainable portfolios by plot ting the expected return of a portfolio against the standard deviation. This is sometimes called the risk–expected return graph. The three points indicated in this picture correspond to portfolios consisting of only one of the three securities. For instance, the portfolio with all funds invested in security 2 is represented by the point (0.24, 0.15). The lines passing through a pair of these three points correspond to portfolios consisting of just two securities. These are the two-security lines studied in detail in Section 5.2. For example, all portfolios containing securities 2 and 3 only lie on the line through (0.24, 0.15) and (0.25, 0.20). The three points and the lines passing through them correspond to the vertices of the triangle and the straight lines passing through them in Figure 5.6. The shaded area (both dark and light), including the boundary, represents portfolios that can be constructed from the three securities, that is, all attainable portfolios. The boundary, shown as a bold line, is the minimum variance line. The shape of it is known as the Markowitz bullet. The darker part of the shaded area corresponds to the interior of the triangle in Figure 5.6, that is, it represents portfolios without short selling. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/e7066a9c600ada3dfc2cd80e13f0475b9b2739c9f11d710ff858aac781d0d109.jpg)



Figure 5.7 Attainable portfolios on the $\sigma , \mu$ plane


It is instructive to imagine how the whole $w _ { 2 } , w _ { 3 }$ plane in Figure 5.6 is mapped onto the shaded area representing all attainable portfolios in Fig ure 5.7. Namely, the $w _ { 2 } , w _ { 3 }$ plane is folded along the minimum variance line, be ing simultaneously warped and stretched to attain the shape of the Markowitz bullet. This means, in particular, that pairs of points on opposite sides of the minimum variance line on the $w _ { 2 } , w _ { 3 }$ plane are mapped into single points on the $\sigma , \mu$ plane. In other words, each point inside the shaded area in Figure 5.7 corresponds to two diferent portfolios. However, each point on the minimum variance line corresponds to a single portfolio. 

## Example 5.12

(3 securities without short selling) For the same three securities as in Exam ples 5.10 and 5.11, Figure 5.8 shows what happens if no short selling is allowed. All portfolios without short selling are represented by the interior and bound ary of the triangle on the $w _ { 1 } , w _ { 2 }$ plane and by the shaded area with boundary on the $\sigma , \mu$ plane. The minimum variance line without short selling is shown as a bold line in both plots. For comparison, the minimum variance line with short selling is shown as a broken line. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/6c4d8d748d58ae6ad7edf8776ee8d2a554a577479cfb003d47a11edf24c12139.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/a3c772b014900110d84dbae1f7509b09c628401bb9d024d143758dd92f6d7a69.jpg)



Figure 5.8 Portfolios without short selling


## Exercise 5.14

For portfolios constructed with and without short selling from the three securities in Exercise 5.12 compute the minimum variance line parametrised by the expected return and sketch it a) on the $w _ { 2 } , w _ { 3 }$ plane and b) on the $\sigma , \mu$ plane. Also sketch the set of all attainable portfolios with and without short selling. 

## 5.3.2 Eficient Frontier

Given the choice between two securities a rational investor will, if possible, choose that with higher expected return and lower standard deviation, that is, lower risk. This motivates the following definition. 

## Definition 5.1

We say that a security with expected return $\mu _ { 1 }$ and standard deviation $\sigma _ { 1 }$ dominates another security with expected return $\mu _ { 2 }$ and standard deviation $\sigma _ { 2 }$ whenever 

$$
\mu_ {1} \geq \mu_ {2} \quad \mathrm{and} \quad \sigma_ {1} \leq \sigma_ {2}.
$$

This definition readily extends to portfolios, which can of course be considered as securities in their own right. 

## Remark 5.4

Given two securities such that one dominates the other, the dominated security may appear quite redundant on first sight. Nevertheless, it can also be of some use. Employing the techniques of Section 5.2, it may be possible to construct portfolios consisting of the two securities with smaller risk than either of the securities, as in Figure 5.9, in which the security with $\sigma _ { 2 } , \mu _ { 2 }$ is dominated by that with $\sigma _ { 1 } , \mu _ { 1 }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/7c91249f7393b19823eb4d63291e9949f6972dfa336ba559419d03fb201b4f00.jpg)



Figure 5.9 Reduction of risk using a dominated security


## Definition 5.2

A portfolio is called eficient if there is no other portfolio, except itself, that dominates it. The set of eficient portfolios among all attainable portfolios is called the eficient frontier. 

Every rational investor will choose an eficient portfolio, always preferring a dominating portfolio to a dominated one. However, diferent investors may select diferent portfolios on the eficient frontier, depending on their individual preferences. Given two eficient portfolios with $\mu _ { 1 } \leq \mu _ { 2 }$ and $\sigma _ { 1 } \le \sigma _ { 2 }$ , a cautious person may prefer that with lower risk $\sigma _ { 1 }$ and lower expected return $\mu _ { 1 }$ , while others may choose a portfolio with higher risk $\sigma _ { 2 }$ , regarding the higher expected return $\mu _ { 2 }$ as compensation for increased risk. 

In particular, an eficient portfolio has the highest expected return among all attainable portfolios with the same standard deviation (the same risk), and has the lowest standard deviation (the lowest risk) among all attainable portfolios with the same expected return. As a result, the eficient frontier must be a subset of the minimum variance line. To understand the structure of the eficient frontier we shall first study the minimum variance line in more detail and then select a suitable subset. 

## Proposition 5.11

Take any two diferent portfolios on the minimum variance line, with weights $\mathbf { \Delta } w ^ { \prime }$ and $\pmb { w } ^ { \prime \prime }$ . Then the minimum variance line consists of portfolios with weights $c { \pmb w } ^ { \prime } + ( 1 - c ) { \pmb w } ^ { \prime \prime }$ for any $c \in \mathbb { R }$ and only of such portfolios. 

## Proof

By Proposition 5.10 the minimum variance line consists of portfolios whose weights are given by a certain linear function of the expected return $\mu _ { V }$ on the portfolio, ${ \pmb w } = { \pmb a } \mu _ { V } + { \pmb b }$ . If $\mathbf { \Delta } w ^ { \prime }$ and $\pmb { w } ^ { \prime \prime }$ are the weights of two diferent portfolios on the minimum variance line, then ${ \pmb w } ^ { \prime } = { \pmb a } \mu _ { V ^ { \prime } } + { \pmb b }$ and $\pmb { w } ^ { \prime \prime } = \pmb { a } \mu _ { V ^ { \prime \prime } } + \pmb { b }$ for some $\mu _ { V ^ { \prime } } \neq \mu _ { V ^ { \prime \prime } }$ . Because numbers of the form $c \mu _ { V ^ { \prime } } + ( 1 - c ) \mu _ { V ^ { \prime \prime } }$ for $c \in \mathbb { R }$ exhaust the whole real line, it follows that portfolios with weights $c { \pmb w } ^ { \prime } + ( 1 - c ) { \pmb w } ^ { \prime \prime }$ for $c \in \mathbb { R }$ exhaust the whole minimum variance line. □ 

This proposition is important. It means that the minimum variance line has the same shape as the set of portfolios constructed from two securities, studied in great detail in Section 5.2. It also means that the shape of the attainable set on the $\sigma , \mu$ plane (the Markowitz bullet), which we have seen so far for portfolios constructed from two or three securities, will in fact be the same for any number of securities. 

Once the shape of the minimum variance line is understood, distinguishing the eficient frontier is easy, also in the case of $n$ securities. This is illustrated in Figure 5.10. The eficient frontier consists of all portfolios on the minimum variance line whose expected return is greater than or equal to the expected return on the minimum variance portfolio. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/dcea45803005d4a4efdee11f9ddb09b2d777005800db3d415deaef6cee429da6.jpg)



Figure 5.10 Eficient frontier constructed from several securities


The next proposition provides a property of the eficient frontier which wil prove useful in the Capital Asset Pricing Model. 

## Proposition 5.12

The weights w of any portfolio belonging to the eficient frontier (except for 

the minimum variance portfolio) satisfy the condition 

$$
\gamma \boldsymbol {w} \boldsymbol {C} = \boldsymbol {m} - \mu \boldsymbol {u}\tag{5.17}
$$

for some real numbers $\gamma > 0$ and $\mu .$ . 

## Proof

Let $\textbf { \em w }$ be the weights of a portfolio, other than the minimum variance portfolio, belonging to the eficient frontier. The portfolio has expected return $\mu _ { V } ~ =$ $\mathbf { \Psi } _ { m w } { \cal T }$ and standard deviation $\sigma _ { V } = \sqrt { \pmb { w } C \pmb { w } ^ { T } }$ . On the $\sigma , \mu$ plane we draw the tangent line to the eficient frontier through the point representing the portfolio. This line will intersect the vertical axis at some point with coordinate $\mu ,$ , the gradient of the line being $\frac { m w ^ { T } - \mu } { \sqrt { w C w ^ { T } } }$ . This gradient is maximal among all lines passing through the point on the vertical axis with coordinate $\mu$ and intersecting the set of attainable portfolios. The maximum is to be taken over all weights w subject to the constraint $\boldsymbol { u } \boldsymbol { w } ^ { T } = 1$ . We put 

$$
F (\pmb {w}, \lambda) = \frac {\pmb {m} \pmb {w} ^ {T} - \mu}{\sqrt {\pmb {w} \pmb {C} \pmb {w} ^ {T}}} - \lambda \pmb {u} \pmb {w} ^ {T},
$$

where $\lambda$ is a Lagrange multiplier. A necessary condition for a constrained maximum is that the partial derivatives of $F$ with respect to the weights should be zero. This gives 

$$
\boldsymbol {m} - \lambda \sigma_ {V} \boldsymbol {u} = \frac {\mu_ {V} - \mu}{\sigma_ {V} ^ {2}} \boldsymbol {w} \boldsymbol {C}.
$$

Multiplying by $\mathbf { \omega } _ { w } ^ { T }$ on the right and using the constraint, we find that $\textstyle \lambda = { \frac { \mu } { \sigma _ { V } } }$ For $\begin{array} { r } { \gamma = \frac { \mu _ { V } - \mu } { \sigma _ { V } ^ { 2 } } } \end{array}$ this gives the asserted condition. Because the tangent line has positive slope, we have $\mu _ { V } > \mu$ , that is, $\gamma > 0$ □ 

## Remark 5.5

An interpretation of $\gamma$ and $\mu$ follows clearly from the proof: $\gamma \sigma _ { V }$ is the gradien of the tangent line to the eficient frontier at the point representing the given portfolio, $\mu$ being the intercept of this tangent line on the $\sigma , \mu$ plane. 

## Exercise 5.15

In a market consisting of the three securities in Exercise 5.12, conside the portfolio on the eficient frontier with expected return $\mu _ { V } = 2 1 \%$ Compute the values of $\gamma$ and $\mu$ such that the weights w in this portfolio satisfy $\gamma \pmb { w } \pmb { C } = \pmb { m } - \mu \pmb { u }$ 

## 5.4 Capital Asset Pricing Model

In the days when computers where slow it was dificult to use portfolio theory. For a market with n = 1, 000 traded securities the covariance matrix C will have $n ^ { 2 } = 1 , 0 0 0 , 0 0 0$ entries. To find the eficient frontier we have to compute the inverse matrix $C ^ { - 1 }$ , which is computationally intensive. Accurate estimation of C may pose considerable problems in practice. The Capital Asset Pricing Model (CAPM) provides a solution that is much more eficient computation ally, does not involve an estimate of $C$ , but ofers a deep, even if somewhat oversimplified, insight into some fundamental economic issues. 

Within the CAPM it is assumed that every investor uses the same values of expected returns, standard deviation and correlations for all securities, making investment decisions based only on these values. In particular, every investor will compute the same eficient frontier on which to select his or her portfo lio. However, investors may difer in their attitude to risk, selecting diferent portfolios on the eficient frontier. 

## 5.4.1 Capital Market Line

Form now on we shall assume that a risk-free security is available in addition to n risky securities. The return on the risk-free security will be denoted by $r _ { F }$ The standard deviation is of course zero for the risk-free security. 

Consider a portfolio consisting of the risk-free security and a specified risky security (possibly a portfolio of risky securities) with expected return $\mu _ { 1 }$ and standard deviation $\sigma _ { 1 } > 0$ . By Proposition 5.7 all such portfolios form a broken line on the $\sigma , \mu$ plane consisting of two rectilinear half-lines, see Figure 5.5. By taking portfolios containing the risk-free security and a security with $\sigma _ { 1 } , \mu _ { 1 }$ anywhere in the attainable set represented by the Markowitz bullet on the $\sigma , \mu$ plane, we can construct any portfolio between the two half-lines shown in Figure 5.11. The eficient frontier of this new set of portfolios, which may contain the risk-free security, is the upper half-line tangent to the Markowitz bullet and passing through the point with coordinates $0 , r _ { F }$ . According to the assumptions of the CAPM, every rational investor will select his or her portfolio on this half-line, called the capital market line. This argument works as long as the risk-free return $r _ { F }$ is not too high, so the upper half-line is tangent to the bullet. (If $r _ { F }$ is too high, then the upper half-line will no longer be tangent to the bullet.) 

The tangency point with coordinates $\sigma _ { M } , \mu _ { M }$ plays a special role. Every portfolio on the capital market line can be constructed from the risk-free se curity and the portfolio with standard deviation $\sigma _ { M }$ and expected return $\mu _ { M }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/958eefafa280ebdcc726dcf67e360bc893d941e25f1b2c8c826f5b011c5d7f28.jpg)



Figure 5.11 Eficient frontier for portfolios with a risk-free security


Since every investor will select a portfolio on the capital market line, everyone will be holding a portfolio with the same relative proportions of risky securities. But this means that the portfolio with standard deviation $\sigma _ { M }$ and expected return $\mu _ { M }$ has to contain all risky securities with weights equal to their relative share in the whole market. Because of this property it is called the market portfolio. In practice the market portfolio is approximated by a suitable stock exchange index. 

The capital market line joining the risk-free security and the market portfolio satisfies the equation 

$$
\mu = r _ {F} + \frac {\mu_ {M} - r _ {F}}{\sigma_ {M}} \sigma .\tag{5.18}
$$

For a portfolio on the capital market line with risk $\sigma$ the term $\frac { \mu _ { M } - r _ { F } } { \sigma _ { M } } \sigma$ is called the risk premium. This additional return above the risk-free level provides compensation for exposure to risk. 

## Example 5.13

We shall apply Proposition 5.12 to compute the market portfolio for a toy market consisting of the three securities in Example 5.10 and a risk-free security with return $r _ { F } = 5 \%$ . The weights w in the market portfolio, which belongs to the eficient frontier, satisfy condition (5.17), which implies that 

$$
\gamma \boldsymbol {w} = (\boldsymbol {m} - \mu \boldsymbol {u}) \boldsymbol {C} ^ {- 1}.
$$

From the proof of Proposition 5.12 we know that $\mu = r _ { F }$ because the capita market line, tangent to the eficient frontier at the point representing the market portfolio, intersects the $\mu$ axis at $r _ { F }$ . Substituting the numerical values from Example 5.10, we find that 

$$
\gamma \boldsymbol {w} \cong \left[ \begin{array}{c c c} 0. 2 9 3 & 1. 3 4 1 & 2. 0 6 1 \end{array} \right].
$$

Since w must satisfy (5.14), it follows that $\gamma \cong 3 . 6 9 4$ and the weights in the market portfolio are 

$$
\boldsymbol {w} \cong \left[ \begin{array}{c c c} 0. 0 7 9 & 0. 3 6 3 & 0. 5 5 8 \end{array} \right].
$$

## Exercise 5.16

Suppose that the risk-free return is $r _ { F } = 5 \%$ . Compute the weights in the market portfolio constructed from the three securities in Exercise 5.11. Also compute the expected return and standard deviation of the marke portfolio. 

## 5.4.2 Beta Factor

It is important to understand how the return $K _ { V }$ on a given portfolio or a single security will react to trends afecting the whole market. To this end we can plot the values of $K _ { V }$ for each market scenario against those of the return $K _ { M }$ on the market portfolio and compute the line of best $f i t$ , also known as the regression line or the characteristic line. In Figure 5.12 the values of $K _ { M }$ are marked along the $x$ axis and the values of $K _ { V }$ along the $y$ axis. The equation of the line of best fit will be 

$$
y = \beta_ {V} x + \alpha_ {V}.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/fdf5d70bf64976d9a95a3225a72d38b4a3f90a9ff7e0b758b516bf6fbe490cd7.jpg)



Figure 5.12 Line of best fit


For any given $\beta$ and α the values of the random variable $\alpha + \beta K _ { M }$ can be regarded as predictions for the return on the given portfolio. The diference $\varepsilon = K _ { V } - \left( \alpha + \beta K _ { M } \right)$ between the actual return $K _ { V }$ and the predicted return $\alpha + \beta K _ { M }$ is called the residual random variable. The condition defining the line of best fit is that 

$$
E (\varepsilon^ {2}) = E (K _ {V} ^ {2}) - 2 \beta E (K _ {V} K _ {M}) + \beta^ {2} E (K _ {M} ^ {2}) + \alpha^ {2} - 2 \alpha E (K _ {V}) + 2 \alpha \beta E (K _ {M})
$$

as a function of $\beta$ and α should attain its minimum at $\beta = \beta _ { V }$ and $\alpha = \alpha _ { V }$ In other words, the line of best fit should lead to predictions that are as close as possible to the true values of $K _ { V }$ . A necessary condition for a minimum is that the partial derivatives with respect to $\beta$ and $\alpha$ should be zero at $\beta = \beta _ { V }$ and $\alpha = \alpha _ { V }$ . This leads to the system of linear equations 

$$
\begin{array}{c} \alpha_ {V} E (K _ {M}) + \beta_ {V} E (K _ {M} ^ {2}) = E (K _ {V} K _ {M}), \\ \alpha_ {V} + \beta_ {V} E (K _ {M}) = E (K _ {V}), \end{array}
$$

which can be solved to find the gradient $\beta _ { V }$ and intercept $\alpha _ { V }$ of the line of best fit, 

$$
\beta_ {V} = \frac {\mathrm{Cov} (K _ {V} , K _ {M})}{\sigma_ {M} ^ {2}}, \quad \alpha_ {V} = \mu_ {V} - \beta_ {V} \mu_ {M}.
$$

Here we employ the usual notation $\mu _ { V } = E ( K _ { V } ) , \mu _ { M } = E ( K _ { M } )$ and $\sigma _ { M } ^ { 2 } =$ Var $\left( K _ { M } \right)$ 

## Exercise 5.17

Suppose that the returns $K _ { V }$ on a given portfolio and $K _ { M }$ on the market portfolio take the following values in diferent market scenarios: 

<table><tr><td>Scenario</td><td>Probability</td><td>Return <eq>K_V</eq></td><td>Return <eq>K_M</eq></td></tr><tr><td><eq>\omega_1</eq></td><td>0.1</td><td>-5%</td><td>10%</td></tr><tr><td><eq>\omega_2</eq></td><td>0.3</td><td>0%</td><td>14%</td></tr><tr><td><eq>\omega_3</eq></td><td>0.4</td><td>2%</td><td>12%</td></tr><tr><td><eq>\omega_3</eq></td><td>0.2</td><td>4%</td><td>16%</td></tr></table>

Compute the gradient $\beta _ { V }$ and intercept $\alpha _ { V }$ of the line of best fit. 

## Definition 5.3

We call 

$$
\beta_ {V} = \frac {\mathrm{Cov} (K _ {V} , K _ {M})}{\sigma_ {M} ^ {2}}
$$

the beta factor of the given portfolio or individual security. 

The beta factor is an indicator of expected changes in the return on a particular portfolio or individual security in response to the behaviour of the market as a whole. Since ${ \mu } _ { V } = \beta _ { V } { \mu } _ { M } + \alpha _ { V }$ , the return on a security with a positive beta factor tends to increase as the return on the market portfolio increases, while the return on a security with a negative beta factor tends to increase if the return on the market portfolio goes down. 

In what follows we discuss another interpretation of the beta factor. The risk $\sigma _ { V } ^ { 2 } = \mathrm { V a r } ( K _ { V } )$ of a security or portfolio can be written as 

$$
\sigma_ {V} ^ {2} = \mathrm{Var} (\varepsilon_ {V}) + \beta_ {V} ^ {2} \sigma_ {M} ^ {2}.
$$

This formula is easy to verify upon substituting the expression $\varepsilon _ { V } = K _ { V } -$ $\left( \alpha _ { V } + \beta _ { V } K _ { M } \right)$ for the residual random variable. The first term $\mathrm { V a r } ( \varepsilon _ { V } )$ is called the residual variance or diversifiable risk. It vanishes for the market portfolio, $\mathrm { V a r } ( \varepsilon _ { M } ) = 0$ . This part of risk can ‘diversified away’ by investing in the market portfolio. The second term $\beta _ { V } ^ { 2 } \sigma _ { M } ^ { 2 }$ is called the systematic or undiversifiable risk. The market portfolio involves only this kind of risk. The beta factor $\beta _ { V }$ can be regarded as a measure of systematic risk associated with a security or portfolio. 

This interpretation of the beta factor is of crucial importance. In the CAPM systematic risk, measured by $\beta _ { V }$ , will be linked to the expected return $\mu _ { V }$ and hence to the pricing of individual securities and portfolios: The higher the systematic risk, the higher the return required by investors as a premium for exposure to this kind of risk. However, diversifiable risk will attract no additional premium, having no efect on $\mu _ { V }$ . This is because diversifiable risk can be eliminated by spreading an investment in a portfolio of many securities and, in particular, by investing in the market portfolio. The next section is devoted to establishing the link between $\beta _ { V }$ and $\mu _ { V }$ 

## Exercise 5.18

Show that the beta factor $\beta _ { V }$ of a portfolio consisting of n securities with weights $w _ { 1 } , \ldots , w _ { n }$ is given by $\beta _ { V } = w _ { 1 } \beta _ { 1 } + \cdot \cdot \cdot + w _ { n } \beta _ { n }$ , where $\beta _ { 1 } , \ldots , \beta _ { n }$ are the beta factors of the securities. 

## 5.4.3 Security Market Line

Consider an arbitrary portfolio with weights ${ \pmb w } _ { V }$ . The weights in the market portfolio will be denoted by ${ \pmb w } _ { M }$ . The market portfolio belongs to the eficient frontier of the attainable set of portfolios consisting of risky securities. Thus, by Proposition 5.12 

$$
\gamma \pmb {w} _ {M} \pmb {C} = \pmb {m} - \mu \pmb {u}
$$

for some numbers $\gamma > 0$ and $\mu .$ . The beta factor of the portfolio with weights ${ \pmb w } _ { V }$ can, therefore, be written as 

$$
\beta_ {V} = \frac {\mathrm{Cov} (K _ {V} , K _ {M})}{\sigma_ {M} ^ {2}} = \frac {\pmb {w} _ {M} \pmb {C} \pmb {w} _ {V} ^ {T}}{\pmb {w} _ {M} \pmb {C} \pmb {w} _ {M} ^ {T}} = \frac {\gamma (\pmb {m} - \mu \pmb {u}) \pmb {w} _ {V} ^ {T}}{\gamma (\pmb {m} - \mu \pmb {u}) \pmb {w} _ {M} ^ {T}} = \frac {\mu_ {V} - \mu}{\mu_ {M} - \mu}.
$$

To find $\mu$ consider the risk-free security, with return $r _ { F }$ and beta factor $\beta _ { F } = 0$ Substituting $\beta _ { F }$ and $r _ { F }$ for $\beta _ { V }$ and $\mu _ { V }$ in the above equation, we find that $\mu = r _ { F }$ . We have proved the following remarkable property. 

## Theorem 5.13

The expected return $\mu _ { V }$ on a portfolio (or an individual security) is a linear function of the beta coeficient $\beta _ { V }$ of the portfolio, 

$$
\mu_ {V} = r _ {F} + (\mu_ {M} - r _ {F}) \beta_ {V}.\tag{5.19}
$$

The expected return plotted against the beta coeficient of any portfolio or individual security will form a straight line on the $\beta , \mu$ plane, called the security market line. This is shown in Figure 5.13, in which the security market line is plotted next to the capital market line for comparison. A number of diferent portfolios and individual securities are indicated by dots in both graphs. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/93485360451a5424a630dbb80255578d78931dc905f41ffdfbf7c0568d1b7f5a.jpg)



Figure 5.13 Capital market line and security market line


Similarly as in formula (5.18) for the capital market line, the term $( \mu _ { M } -$ $r _ { F } ) \beta _ { V }$ in (5.19) is the risk premium, interpreted as compensation for exposure to systematic risk. However, (5.18) applies only to portfolios on the capital market line, whereas (5.19) is much more general: It applies to all portfolios and individual securities. 

## Exercise 5.19

Show that the characteristic lines of all securities intersect at a common point in the CAPM. What are the coordinates of this point? 

The CAPM describes a state of equilibrium in the market. Everyone is holding a portfolio of risky securities with the same weights as the market portfolio. Any trades that may be executed by investors will only afect their split of funds between the risk-free security and the market portfolio. As a result, the demand and supply of all securities will be balanced. This will remain so as long as the estimates of expected returns and beta factors satisfy (5.19). 

However, as soon as some new information about the market becomes available to investors, it may afect their estimates of expected returns and beta factors. The new estimated values may no longer satisfy (5.19). Suppose, for example, that 

$$
\mu_ {V} > r _ {F} + (\mu_ {M} - r _ {F}) \beta_ {V}
$$

for a particular security. In this case investors will want to increase their relative position in this security, which ofers a higher expected return than required as compensation for systematic risk. Demand will exceed supply, the price of the security will begin to rise and the expected return will decline. On the other hand, if the reverse inequality 

$$
\mu_ {V} <   r _ {F} + (\mu_ {M} - r _ {F}) \beta_ {V}
$$

holds, investors will want to sell the security. In this case supply will exceed demand, the price will fall and the expected return will increase. This will continue until the prices and with them the expected returns of all securities settle at a new level, restoring equilibrium. 

The above inequalities are important in practice. They send a clear signal to investors whether any particular security is underpriced or, respectively, overpriced, that is, whether it should be bought or sold. 

# Forward and Futures Contracts

## 6.1 Forward Contracts

A forward contract is an agreement to buy or sell an asset on a fixed date in the future, called the delivery time, for a price specified in advance, called the forward price. The party to the contract who agrees to sell the asset is said to be taking a short forward position. The other party, obliged to buy the asset at delivery, is said to have a long forward position. The principal reason for entering into a forward contract is to become independent of the unknown future price of a risky asset. There are a variety of examples: a farmer wishing to fix the sale price of his crops in advance, an importer arranging to buy foreign currency at a fixed rate in the future, a fund manager who wants to sell stock for a price known in advance. A forward contract is a direct agreement between two parties. It is typically settled by physical delivery of the asset on the agreed date. As an alternative, settlement may sometimes be in cash. 

Let us denote the time when the forward contract is exchanged by 0, the delivery time by T, and the forward price by $F ( 0 , T )$ . The time t market price of the underlying asset will be denoted by $S ( t )$ . No payment is made by either party at time 0, when the forward contract is exchanged. At delivery the party with a long forward position will benefit if $F ( 0 , T ) < S ( T )$ ). They can buy the asset for $F ( 0 , T )$ and sell it for the market price $S ( T )$ , making an instant profit of $S ( T ) - F ( 0 , T )$ . Meanwhile, the party holding a short forward position will sufer a loss of $S ( T ) - F ( 0 , T )$ because they will have to sell below the market price. If $F ( 0 , T ) > S ( T )$ , then the situation will be reversed. The payofs at delivery are $S ( T ) - F ( 0 , T )$ for a long forward position and $F ( 0 , T ) - S ( T )$ for a short position; see Figure 6.1. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/1d74354f99602bbf085c39cf76d3f683f009340cadefed773646cc02a36db675.jpg)



Figure 6.1 Payof for long and short forward positions at delivery


If the contract is initiated at time $t < T$ rather than 0, then we shall write $F ( t , T )$ for the forward price, the payof at delivery being $S ( T ) - F ( t , T )$ for a long forward position and $F ( t , T ) - S ( T )$ for a short position. 

## 6.1.1 Forward Price

The No-Arbitrage Principle makes it possible to obtain formulae for the forward prices of assets of various kinds. We begin with the simplest case. 

Stock Paying No Dividends. Consider a security that can be stored at no cost and brings no profit (except perhaps for capital gains arising from random price fluctuations). A typical example is a stock paying no dividends. We shall denote by r the risk-free rate under continuous compounding and assume that it is constant throughout the period in question. 

An alternative to taking a long forward position in stock with delivery at time T and forward price $F ( 0 , T )$ is to borrow $S ( 0 )$ dollars to buy the stock at time 0 and keep it until time T. The amount $S ( 0 ) \mathrm { e } ^ { r T }$ to be paid to settle the loan with interest at time T is a natural candidate for the forward price $F ( 0 , T )$ . The following theorem makes this intuitive argument formal. 

## Theorem 6.1

For a stock paying no dividends the forward price is 

$$
F (0, T) = S (0) \mathrm{e} ^ {r T},\tag{6.1}
$$

where r is a constant risk-free interest rate under continuous compounding. If the contract is initiated at time $t \leq T$ , then 

$$
F (t, T) = S (t) \mathrm{e} ^ {r (T - t)}.\tag{6.2}
$$

## Proof

We shall prove formula (6.1). Suppose that $F ( 0 , T ) > S ( 0 ) \mathrm { e } ^ { r T }$ . In this case, at time 0 

borrow the amount S(0) until time T; 

buy one share for $S ( 0 )$ ; 

take a short forward position, that is, agree to sell one share for $F ( 0 , T )$ at time T. 

Then, at time T 

sell the stock for $F ( 0 , T )$ ; 

• <sup>pay</sup> $S ( 0 ) \mathrm { e } ^ { r T }$ to clear the loan with interest. 

This will bring a risk-free profit of 

$$
F (0, T) - S (0) \mathrm{e} ^ {r T} > 0,
$$

contrary to the No-Arbitrage Principle. Next, suppose that $F ( 0 , T ) < S ( 0 ) \mathrm { e } ^ { r T }$ In this case we construct the opposite strategy to the one above. At time 0 

sell short one share for $S ( 0 )$ ; 

invest the proceeds at the risk-free rate; 

enter into a long forward contract with forward price $F ( 0 , T )$ 

Then, at time $T$ 

cash the risk-free investment with interest, collecting $S ( 0 ) \mathrm { e } ^ { r T }$ dollars; 

buy the stock for $F ( 0 , T )$ using the forward contract; 

close out the short position in stock by returning it to the owner. 

You will end up with a positive amount 

$$
S (0) \mathrm{e} ^ {r T} - F (0, T) > 0,
$$

again a contradiction with the No-Arbitrage Principle. 

The proof of (6.2) is similar. Simply replace 0 by t, observing that the time elapsed between exchanging the forward contract and delivery is now $T - t$ . 

In a market with restrictions on short sales of stock the inequality $F ( 0 , T ) <$ $S ( 0 ) \mathrm { e } ^ { r T }$ does not necessarily lead to arbitrage opportunities. 

## Exercise 6.1

Suppose that $S ( 0 ) = 1 7$ dollars, $F ( 0 , 1 ) = 1 8$ dollars, $r = 8 \%$ , and shortselling requires a 30% security deposit attracting interest at $d = 4 \%$ . Is there an arbitrage opportunity? Find the highest rate d for which there is no arbitrage opportunity. 

## Exercise 6.2

Suppose that the price of stock on 1 April 2000 turns out to be 10% lower than it was on 1 January 2000. Assuming that the risk-free rate is constant at $r = 6 \%$ , what is the percentage drop of the forward price on 1 April 2000 as compared to that on 1 January 2000 for a forward contract with delivery on 1 October 2000? 

## Remark 6.1

In the case considered here we always have $F ( t , T ) = S ( t ) \mathrm { e } ^ { r ( T - r ) } > S ( t )$ . The diference $F ( t , T ) - S ( t )$ , which is called the basis, converges to 0 as $t \nearrow T$ 

## Remark 6.2

Under periodic compounding the forward price is given by 

$$
F (0, T) = S (0) (1 + \frac {r}{m}) ^ {m T}.
$$

In terms of zero-coupon bond prices, this formula becomes 

$$
F (0, T) = S (0) B (0, T) ^ {- 1}.
$$

The last formula is in fact more general, requiring no assumption about constant interest rates. 

Including Dividends. We shall generalise the formula for the forward price to cover assets that generate income during the lifetime of the forward contract. The income may be in the form of dividends or a convenience yield. We shall also cover the case when the asset involves some costs (called the cost of carry), such as storage or insurance, by treating the costs as negative income. 

Suppose that the stock is to pay a dividend div at an intermediate time t between initiating the forward contract and delivery. At time t the stock price will drop by the amount of the dividend paid. The formula for the forward price, which involves the present stock price, can be modified by subtracting the present value of the dividend. 

## Theorem 6.2

The forward price of a stock paying dividend div at time t, where $0 < t < T$ , is 

$$
F (0, T) = [ S (0) - \mathrm{e} ^ {- r t} \mathrm{div} ] \mathrm{e} ^ {r T}.\tag{6.3}
$$

## Proof

Suppose that 

$$
F (0, T) > [ S (0) - \mathrm{e} ^ {- r t} \mathrm{div} ] \mathrm{e} ^ {r T}.
$$

We shall construct an arbitrage strategy. At time 0 

enter into a short forward contract with forward price $F ( 0 , T )$ and delivery time $T ;$ ; 

borrow $S ( 0 )$ dollars and buy one share. 

At time t 

cash the dividend div and invest it at the risk-free rate for the remaining time $T - t$ 

At time T 

sell the share for $F ( 0 , T )$ ; 

pay $S ( 0 ) \mathrm { e } ^ { r T }$ to clear the loan with interest and collect $\mathrm { e } ^ { r ( T - t ) }$ div. 

The final balance will be positive: 

$$
F (0, T) - S (0) \mathrm{e} ^ {r T} + \mathrm{e} ^ {r (T - t)} \mathrm{div} > 0,
$$

a contradiction with the No-Arbitrage Principle. On the other hand, suppose that 

$$
F (0, T) <   [ S (0) - \mathrm{e} ^ {- r t} \mathrm{div} ] \mathrm{e} ^ {r T}.
$$

In this case, at time 0 

enter into a long forward contract with forward price $F ( 0 , T )$ and delivery at time $T ;$ ; 

sell short one share and invest the proceeds $S ( 0 )$ at the risk-free rate. 

At time t 

borrow div dollars and pay a dividend to the stock owner. 

At time T 

buy one share for $F ( 0 , T )$ and close out the short position in stock; 

cash the risk-free investment with interest, collecting the amount $S ( 0 ) \mathrm { e } ^ { r T }$ , and pay $\mathrm { e } ^ { r ( T - t ) } \mathrm { d i v }$ to clear the loan with interest. 

The final balance will again be positive, 

$$
- F (0, T) + S (0) \mathrm{e} ^ {r T} - \mathrm{e} ^ {r (T - t)} \mathrm{div} > 0,
$$

completing the proof. 

The formula can easily be generalised to the case when dividends are paid more than once: 

$$
F (0, T) = [ S (0) - \mathrm{div} _ {0} ] \mathrm{e} ^ {r T},\tag{6.4}
$$

where $\mathrm { d i v _ { 0 } }$ is the present value of all dividends due during the lifetime of the forward contract. 

## Exercise 6.3

Consider a stock whose price on 1 January is $120 and which will pay a dividend of $1 on 1 July 2000 and $2 on 1 October 2000. The interest rate is 12%. Is there an arbitrage opportunity if on 1 January 2000 the forward price for delivery of the stock on 1 November 2000 is $131? If so, compute the arbitrage profit. 

## Exercise 6.4

Suppose that the risk-free rate is $8 \%$ . However, as a small investor, you can invest money at $7 \%$ only and borrow at $1 0 \%$ . Does either of the strategies in the proof of Proposition 6.2 give an arbitrage profit if $F ( 0 , 1 ) = 8 9 $ and $S ( 0 ) = 8 3 $ dollars, and a $2 dividend is paid in the middle of the year, that is, at time $1 / 2 ?$ 

Dividend Yield. Dividends are often paid continuously at a specified rate, rather than at discrete time instants. For example, in a case of a highly diversified portfolio of stocks it is natural to assume that dividends are paid continuously rather than to take into account frequent payments scattered throughout the year. Another example is foreign currency, attracting interest at the corresponding rate. 

We shall first derive a formula for the forward price in the case of foreign currency. Let the price of one British pound in New York be $P ( t )$ dollars, and let the risk-free interest rates for investments in British pounds and US dollars be r<sub>GBP</sub> and r<sub>USD</sub>, respectively. Let us compare the following strategies: 

A: Invest $P ( 0 )$ dollars at the rate $r _ { \mathrm { U S D } }$ for time $T .$ 

B: Buy 1 pound for $P ( 0 )$ dollars, invest it for time $T$ at the rate r<sub>GBP</sub>, and take a short position in $\mathrm { e } ^ { r _ { \mathrm { G B P } } T }$ pound sterling forward contracts with delivery time $T$ and forward price $F ( 0 , T )$ 

Both strategies require the same initial outlay, so the final values should be also the same: 

$$
P (0) \mathrm{e} ^ {r _ {\mathrm{USD}} T} = \mathrm{e} ^ {r _ {\mathrm{GBP}} T} F (0, T).
$$

It follows that 

$$
F (0, T) = P (0) \mathrm{e} ^ {(r _ {\mathrm{USD}} - r _ {\mathrm{GBP}}) T}.\tag{6.5}
$$

Next, suppose that a stock pays dividends continuously at a rate $r _ { \mathrm { d i v } } > 0$ , called the (continuous) dividend yield. If the dividends are reinvested in the stock, then an investment in one share held at time 0 will increase to become $\mathrm e ^ { r \mathrm { d i v } T }$ shares at time T. (The situation is similar to continuous compounding.) Consequently, in order to have one share at time T we should begin with $\mathrm { e } ^ { - r _ { \mathrm { d i v } } T }$ shares at time 0. This observation is used in the arbitrage proof below. 

## Theorem 6.3

The forward price for stock paying dividends continuously at a rate $r _ { \mathrm { d i v } }$ is 

$$
F (0, T) = S (0) \mathrm{e} ^ {(r - r _ {\mathrm{div}}) T}.\tag{6.6}
$$

Proof 

Suppose that 

$$
F (0, T) > S (0) \mathrm{e} ^ {(r - r _ {\mathrm{div}}) T}.
$$

In this case, at time 0 

enter into a short forward contract; 

borrow the amount $S ( 0 ) \mathrm { e } ^ { - r _ { \mathrm { d i v } } T }$ to buy $\mathrm { e } ^ { - r _ { \mathrm { d i v } } T }$ shares. 

Between time 0 and T collect the dividends paid continuously, reinvesting them in the stock. At time T you will have 1 share, as explained above. At that time 

sell the share for $F ( 0 , T )$ , closing out the short forward position; 

• <sup>pay</sup> $S ( 0 ) \mathrm { e } ^ { ( r - r _ { \mathrm { d i v } } ) T }$ to clear the loan with interest. 

The final balance $F ( 0 , T ) - S ( 0 ) \mathrm { e } ^ { ( r - r _ { \mathrm { d i v } } ) T } > 0$ will be your arbitrage profit. Now suppose that 

$$
F (0, T) <   S (0) \mathrm{e} ^ {(r - r _ {\mathrm{div}}) T}.
$$

If this is the case, then at time 0 

take a long forward position; 

sell short a fraction $\mathrm { e } ^ { - r _ { \mathrm { d i v } } T }$ of a share investing the proceeds $S ( 0 ) \mathrm { e } ^ { - r _ { \mathrm { d i v } } T }$ risk free. 

Between time 0 and T you will need to pay dividends to the stock owner, raising cash by shorting the stock. Your short position in stock will thus increase to 1 share at time T. At that time 

buy one share for $F ( 0 , T )$ and return it to the owner, closing out the long forward position and the short position in stock; 

receive $S ( 0 ) \mathrm { e } ^ { ( r - r _ { \mathrm { d i v } } ) T }$ from the risk-free investment. 

Again you will end up with a positive amount $S ( 0 ) \mathrm { e } ^ { ( r - r _ { \mathrm { d i v } } ) T } - F ( 0 , T ) > 0 ,$ contrary to the No-Arbitrage Principle. □ 

In general, if the contract is initiated at time $t < T$ , then 

$$
F (t, T) = S (t) \mathrm{e} ^ {(r - r _ {\mathrm{div}}) (T - t)}.\tag{6.7}
$$

## Exercise 6.5

A US importer of German cars wants to arrange a forward contract to buy euros in half a year. The interest rates for investments in US dollars and euros are $r _ { \mathrm { U S D } } ~ = ~ 4 \%$ and $r _ { \mathrm { E U R } } ~ = ~ 3 \%$ , respectively, the current exchange rate being 0.9834 euros to a dollar. What is the forward price of euros expressed in dollars (that is, the forward exchange rate)? 

## 6.1.2 Value of a Forward Contract

Every forward contract has value zero when initiated. As time goes by, the price of the underlying asset may change. Along with it, the value of the forward contract will vary and will no longer be zero, in general. In particular, the value of a long forward contract will be $S ( T ) - F ( 0 , T )$ at delivery, which may turn out to be positive, zero or negative. We shall derive formulae to capture the changes in the value of a forward contract. 

Suppose that the forward price $F ( t , T )$ for a forward contract initiated at time t, where $0 < t < T$ , is higher than $F ( 0 , T )$ . This is good news for an investor with a long forward position initiated at time 0. At time T such an investor will gain $F ( t , T ) - F ( 0 , T )$ as compared to an investor entering into a new long forward contract at time t with the same delivery date T. To find the value of the original forward position at time t all we have to do is to discount this gain back to time t. This discounted amount would be received (or paid, if negative) by the investor with a long position should the forward contract initiated at time 0 be closed out at time t, that is, prior to delivery $T .$ . This intuitive argument needs to be supported by a rigorous arbitrage proof. 

## Theorem 6.4

For any t such that $0 \leq t \leq T$ the time t value of a long forward contract with forward price $F ( 0 , T )$ is given by 

$$
V (t) = [ F (t, T) - F (0, T) ] \mathrm{e} ^ {- r (T - t)}.\tag{6.8}
$$

Proof 

Suppose that 

$$
V (t) <   [ F (t, T) - F (0, T) ] \mathrm{e} ^ {- r (T - t)}.
$$

If so, then at time t 

borrow the amount $V ( t )$ 1 to enter into a long forward contract with forward price $F ( 0 , T )$ and delivery time $T ;$ ; 

initiate a short forward position with forward price $F ( t , T )$ , at no cost. 

Next, at time T 

close out the forward contracts collecting (or paying, if negative) the amounts $S ( T ) \mathrm { ~ - ~ } F ( 0 , T )$ for the long position and $- S ( T ) + F ( t , T )$ for the short position; 

pay back the loan with interest amounting to $V ( t ) \mathrm { e } ^ { t ( T - t ) }$ in total. 

The final balance $F ( t , T ) - F ( 0 , T ) - V ( t ) \mathrm { e } ^ { t ( T - t ) } > 0$ will be your arbitrage profit. 

We leave the case when 

$$
V (t) > [ F (t, T) - F (0, T) ] \mathrm{e} ^ {- r (T - t)}
$$

as an exercise. 

□ 

Exercise 6.6 

Show that $V ( t ) > [ F ( t , T ) - F ( 0 , T ) ] \mathrm { e } ^ { - r ( T - t ) }$ leads to an arbitrage opportunity. 

Observe that $V ( 0 ) = 0$ , which is the initial value of the forward contract, and $V ( T ) = S ( T ) - F ( 0 , T )$ (since $F ( T , T ) = S ( T ) )$ , which is the terminal payof. 

For a stock paying no dividends formula (6.8) gives 

$$
V (t) = [ S (t) \mathrm{e} ^ {r (T - t)} - S (0) \mathrm{e} ^ {r T} ] \mathrm{e} ^ {- r (T - t)} = S (t) - S (0) \mathrm{e} ^ {r t}.\tag{6.9}
$$

The message is: If the stock price grows at the same rate as a risk-free investment, then the value of the forward contract will be zero. Growth above the risk-free rate results in a gain for the holder of a long forward position. 

## Remark 6.3

Consider a contract with delivery price X rather than $F ( 0 , T )$ . The value of this contract at time t will be given by (6.8) with $F ( 0 , T )$ replaced by X, 

$$
V _ {X} (t) = [ F (t, T) - X ] \mathrm{e} ^ {- r (T - t)}.
$$

Such a contract may have non-zero value initially. In the case of a stock paying no dividends 

$$
V _ {X} (0) = [ F (0, T) - X ] \mathrm{e} ^ {- r T} = S (0) - X \mathrm{e} ^ {- r T}.\tag{6.10}
$$

For a stock paying one dividend between times 0 and T the initial value of the contract is 

$$
V _ {X} (0) = S (0) - \mathrm{div} _ {0} - X \mathrm{e} ^ {- r T},
$$

div<sub>0</sub> being the value of the dividend discounted to time 0. For a stock paying dividends continuously at a rate $r _ { \mathrm { d i v } }$ , the initial value of the contract is 

$$
V _ {X} (0) = S (0) \mathrm{e} ^ {- r _ {\mathrm{div}} T} - X \mathrm{e} ^ {- r T}.
$$

## Exercise 6.7

Suppose that the price of a stock is $45 at the beginning of the year, the risk-free rate is 6%, and a $2 dividend is to be paid after half a year. For a long forward position with delivery in one year, find its value after 9 months if the stock price at that time turns out to be a) $49, b) $51. 

## 6.2 Futures

One of the two parties to a forward contract will be losing money. There is always a risk of default by the party sufering a loss. Futures contracts are designed to eliminate such risk. 

We assume for a while that time is discrete with steps of length τ, typically a day. 

Just like a forward contract, a futures contract involves an underlying asset and a specified time of delivery, a stock with prices $S ( n )$ for $n = 0 , 1 , \ldots$ . and time T, say. In addition to the usual stock prices, the market dictates the socalled futures prices $f ( n , T )$ for each step $n = 0 , 1 , \ldots$ . such that $n \tau \leq T$ . These prices are unknown at time 0, except for $f ( 0 , T )$ , and we shall treat them as random variables. 

As in the case of a forward contract, it costs nothing to initiate a futures position. The diference lies in the cash flow during the lifetime of the contract. A long forward contract involves just a single payment $S ( T ) - F ( 0 , T )$ at delivery. A futures contract involves a random cash flow, known as marking to market. Namely, at each time step $n = 1 , 2 , \ldots$ . such that $n \tau \leq T$ the holder of a long futures position will receive the amount 

$$
f (n, T) - f (n - 1, T)
$$

if positive, or will have to pay it if negative. The opposite payments apply fo a short futures position. The following two conditions are imposed: 

1. The futures price at delivery is $f ( T , T ) = S ( T )$ 

2. At each time step $n = 0 , 1 , \ldots$ . such that $n \tau \leq T$ the value of a futures position is zero. (At each step $n \geq 1$ this value is computed after marking to market.) 

The second condition means that, in particular, it costs nothing to close, open or alter a futures position at any time step between 0 and T. 

## Remark 6.4

To ensure that the obligations involved in a futures position are fulfilled, certain practical regulations are enforced. Each investor entering into a futures contract has to pay a deposit, called the initial margin, which is kept by the clearing house as collateral. In the case of a long futures position the amount $f ( n , T ) -$ $f ( n - 1 , T )$ is added to the deposit if positive or subtracted if negative at each time step n, typically once a day. (The opposite amount is added or subtracted for a short futures position.) Any excess that builds up above the initial margin can be withdrawn by the investor. On the other hand, if the deposit drops below a certain level, called the maintenance margin, the clearing house will issue a margin call, requesting the investor to make a payment and restore the deposit to the level of the initial margin. A futures position can be closed at any time, in which case the deposit will be returned to the investor. In particular, the futures position will be closed immediately by the clearing house if the investor fails to respond to a margin call. As a result, the risk of default is eliminated. 

## Example 6.1

Suppose that the initial margin is set at 10% and the maintenance margin at 5% of the futures price. The table below shows a scenario with futures prices $f ( n , T )$ . The columns labelled ‘margin 1’ and ‘margin 2’ show the deposit at the beginning and at the end of each day, respectively. The ‘payment’ column con tains the amounts paid to top up the deposit (negative numbers) or withdrawn 

(positive numbers). 

<table><tr><td>n</td><td>f(n,T)</td><td>cash flow</td><td>margin 1</td><td>payment</td><td>margin 2</td></tr><tr><td>0</td><td>140</td><td>opening:</td><td>0</td><td>-14</td><td>14</td></tr><tr><td>1</td><td>138</td><td>-2</td><td>12</td><td>0</td><td>12</td></tr><tr><td>2</td><td>130</td><td>-8</td><td>4</td><td>-9</td><td>13</td></tr><tr><td>3</td><td>140</td><td>+10</td><td>23</td><td>+9</td><td>14</td></tr><tr><td>4</td><td>150</td><td>+10</td><td>24</td><td>+9</td><td>15</td></tr><tr><td></td><td></td><td>closing:</td><td>15</td><td>+15</td><td>0</td></tr><tr><td></td><td></td><td></td><td>total:</td><td>10</td><td></td></tr></table>

On day 0 a futures position is opened and a 10% deposit paid. On day 1 the futures price drops by $2, which is subtracted from the deposit. On day 2 the futures price drops further by $8, triggering a margin call because the deposit falls below 5%. The investor has to pay $9 to restore the deposit to the 10% level. On day 3 the forward price increases and $9 is withdrawn, leaving a 10% margin. On day 4 the forward price goes up again, allowing the investor to withdraw another $9. At the end of the day the investor decides to close the position, collecting the balance of the deposit. The total of all payments is $10, the increase in the futures price between day 0 and 4. 

## Remark 6.5

An important feature of the futures market is liquidity. This is possible due to standardisation and the presence of a clearing house. Only futures contracts with particular delivery dates are traded. Moreover, futures contracts on commodities such as gold or timber specify standardised delivery arrangements as well as standardised physical properties of the assets. The clearing house acts as an intermediary, matching the total of a large number of short and long futures positions of various sizes. The clearing house also maintains the margin deposit for each investor to eliminate the risk of default. This is in contrast to forward contracts negotiated directly between two parties. 

## 6.2.1 Pricing

We shall show that in some circumstances the forward and the futures prices are the same. Let r be the risk-free rate under continuous compounding. 

## Theorem 6.5

If the interest rate is constant, then $f ( 0 , T ) = F ( 0 , T )$ 

## Proof

Suppose for simplicity that marking to market is performed at just two intermediate time instants $0 < t _ { 1 } < t _ { 2 } < T$ . The argument below can readily be extended to cover more frequent marking to market. 

Take a long forward position with forward price $F ( 0 , T )$ and invest the amount of $\mathrm { e } ^ { - r T } F ( 0 , T )$ risk free. At time T close the risk-free investment, collecting the amount $F ( 0 , T )$ , purchase one share for $F ( 0 , T )$ using the forward contract, and sell the share for the market price $S ( T )$ . Your final wealth will be $S ( T )$ 

Our goal is to replicate this payof by a suitable strategy using futures contracts. At time 0 

we open a fraction $\mathrm { e } ^ { - r ( T - t _ { 1 } ) }$ of a long futures position (at no cost); 

we invest the amount $ { \mathrm { e } } ^ { - r T } f ( 0 , T )$ risk free (this investment will grow to $v _ { 0 } = f ( 0 , T )$ at time T). 

At time $t _ { 1 }$ 

we receive (or pay) the amount $\mathrm { e } ^ { - r ( T - t _ { 1 } ) } [ f ( t _ { 1 } , T ) - f ( 0 , T ) ]$ as a result of marking to market; 

we invest (or borrow, depending on the sign) $\mathrm { e } ^ { - r ( T - t _ { 1 } ) } [ f ( t _ { 1 } , T ) - f ( 0 , T ) ]$ (this investment will grow to $v _ { 1 } = f ( t _ { 1 } , T ) - f ( 0 , T )$ at time T); 

we increase our long futures position to $\mathrm { e } ^ { - r ( T - t _ { 2 } ) }$ of a contract (at no cost). 

At time $t _ { 2 }$ 

we cash (or pay) $\mathrm { e } ^ { - r ( T - t _ { 2 } ) } [ f ( t _ { 2 } , T ) - f ( t _ { 1 } , T ) ]$ as a result of marking to market; 

we invest (or borrow, depending on the sign) $\mathrm { e } ^ { - r ( T - t _ { 2 } ) } [ f ( t _ { 2 } , T ) - f ( t _ { 1 } , T ) ]$ (this investment will grow to $v _ { 2 } = f ( t _ { 2 } , T ) - f ( t _ { 1 } , T )$ at time T); 

we increase the long futures position to 1 (at no cost). 

At time T 

we close the risk-free investment, collecting the amount $v _ { 0 } + v _ { 1 } + v _ { 2 } =$ $f ( t _ { 2 } , T )$ ; 

we close the futures position, receiving (or paying) the amount $S ( T ) -$ $f ( t _ { 2 } , T )$ 

The final wealth will be $S ( T )$ , as before. Therefore, to avoid arbitrage, the initial investments initiating both strategies have to be the same, that is, 

$$
\mathrm{e} ^ {- r T} F (0, T) = \mathrm{e} ^ {- r T} f (0, T),
$$

which proves the claim. 

This construction cannot be performed if the interest rate changes unpre dictably. However if interest rate changes are known in advance, the argument can be suitably modified and the equality between the futures and forward prices remains valid. 

In an economy with constant interest rates r we obtain a simple structure of futures prices, 

$$
f (t, T) = S (t) \mathrm{e} ^ {r (T - t)}\tag{6.11}
$$

if the stock pays no dividends. The futures prices are random, but this is caused entirely by the randomness of the prices of the underlying asset. If the futures prices depart from the values given by the above formula, it is a reflection of the market’s view of future interest rate changes. 

## Exercise 6.8

Suppose the interest rate r is constant. Given S(0), find the price S(1) of the stock after one day such that the marking to market of futures with delivery in 3 months is zero on that day. 

This exercise shows an important benchmark for the profitability of a fu tures position: An investor who wants to take advantage of a predicted increase in the price of stock above the risk-free rate should enter into a long futures position. A short futures position will bring a profit should the stock price go down or increase below the risk-free rate. 

## 6.2.2 Hedging with Futures

The Basis. One relatively simple way to hedge an exposure to stock price variations is to enter a forward contract. However, a contract of this kind may not be readily available, not to mention the risk of default. Another possibility is to hedge using the futures market, which is well-developed, liquid and protected from the risk of default. 

## Example 6.2

Let $S ( 0 ) = 1 0 0$ dollars and let the risk-free rate be constant at $r = 8 \%$ . Assume that marking to market takes place once a month, the time step being $\tau = 1 / 1 2$ Suppose that we wish to sell the stock after 3 months. To hedge the exposure to stock price variations we enter into one short futures contract on the stock with delivery in 3 months. The payments resulting from marking to market are invested (or borrowed), attracting interest at the risk-free rate. The results for two diferent stock price scenarios are displayed below. The column labelled ‘m2m’ represents the payments due to marking to market and the last column shows the interest accrued up to the delivery date. 


Scenario 1


<table><tr><td>n</td><td>S(n)</td><td>f(n,3/12)</td><td>m2m</td><td>interest</td></tr><tr><td>0</td><td>100</td><td>102.02</td><td></td><td></td></tr><tr><td>1</td><td>102</td><td>103.37</td><td>-1.35</td><td>-0.02</td></tr><tr><td>2</td><td>101</td><td>101.67</td><td>+1.69</td><td>+0.01</td></tr><tr><td>3</td><td>105</td><td>105.00</td><td>-3.32</td><td>0.00</td></tr><tr><td></td><td></td><td>total:</td><td>-2.98</td><td>-0.01</td></tr></table>

In this scenario we sell the stock for $105.00, but marking to market brings losses, reducing the sum to $1 0 5 . 0 0 - 2 . 9 8 - 0 . 0 1 = 1 0 2 . 0 1$ dollars. Note that if the marking to market payments were not invested at the risk-free rate, then the realized sum would be $1 0 5 . 0 0 - 2 . 9 8 = 1 0 2 . 0 2$ dollars, that is, exactly equal to the futures price $f ( 0 , 3 / 1 2 )$ 


Scenario 2


<table><tr><td>n</td><td>S(n)</td><td>f(n,3/12)</td><td>m2m</td><td>interest</td></tr><tr><td>0</td><td>100</td><td>102.02</td><td></td><td></td></tr><tr><td>1</td><td>98</td><td>99.31</td><td>+2.70</td><td>+0.04</td></tr><tr><td>2</td><td>97</td><td>97.65</td><td>+1.67</td><td>+0.01</td></tr><tr><td>3</td><td>92</td><td>92.00</td><td>+5.65</td><td>0.00</td></tr><tr><td></td><td></td><td>total:</td><td>+10.02</td><td>+0.05</td></tr></table>

In this case we sell the stock for $92.00 and benefit from marking to market along with the interest earned, bringing the final sum to $9 2 . 0 0 + 1 0 . 0 2 + 0 . 0 5 =$ 102. 07 dollars. Without the interest the final sum would be $9 2 . 0 0 + 1 0 . 0 2 =$ 102.02 dollars, once again exactly the futures price $f ( 0 , 3 / 1 2 )$ 

In reality the calculations in Example 6.2 are slightly more complicated because of the presence of the initial margin, which we have neglected for simplicity. Some limitations come from the standardisation of futures contracts. As a result, a dificulty may arise in matching the terms of the contract to our needs. For example, the exercise dates for futures are typically certain fixed days in four specified months in a year, for example the third Friday in March, June, September and December. If we want to close out our investment at the end of April, we will need to hedge with futures contracts with delivery date beyond the end of April, for example, in June. 

## Example 6.3

Suppose we wish to sell stock after 2 months and we hedge using futures with delivery in 3 months (we work in the same scenarios as in Example 6.2): 


Scenario 1


<table><tr><td>n</td><td>S(n)</td><td>f(n,3/12)</td><td>m2m</td><td>interest</td></tr><tr><td>0</td><td>100</td><td>102.02</td><td></td><td></td></tr><tr><td>1</td><td>102</td><td>103.37</td><td>-1.35</td><td>-0.01</td></tr><tr><td>2</td><td>101</td><td>101.67</td><td>1.69</td><td>0.00</td></tr><tr><td></td><td></td><td>total:</td><td>0.34</td><td>-0.01</td></tr></table>

We sell the stock for $101.00, which together with marking to market and interest will give $101.33. 


Scenario 2


<table><tr><td>n</td><td>S(n)</td><td>f(n,3/12)</td><td>m2m</td><td>interest</td></tr><tr><td>0</td><td>100</td><td>102.02</td><td></td><td></td></tr><tr><td>1</td><td>98</td><td>99.31</td><td>2.70</td><td>0.02</td></tr><tr><td>2</td><td>97</td><td>97.65</td><td>1.67</td><td>0.00</td></tr><tr><td></td><td></td><td>total:</td><td>4.37</td><td>0.02</td></tr></table>

In this case we sell the stock for $97.00, and together with marking to market and interest obtain $101.39. 

We almost hit the target, which is the futures price $f ( 0 , 2 ) \cong 1 0 1 . 3 4$ dollars, that is, the value of $100 compounded at the risk-free rate. 

## Remark 6.6

The diference between the spot and futures prices is called the basis (as for forward contracts): 

$$
b (t, T) = S (t) - f (t, T).
$$

(Sometimes the basis is defined as $f ( t , T ) - S ( t ) . )$ The basis converges to zero as $t \to T$ , since $f ( T , T ) = S ( T )$ . In a market with constant interest rates it is given explicitly by 

$$
b (t, T) = S (t) \left(1 - \mathrm{e} ^ {r (T - t)}\right),
$$

being negative for $t < T$ . If the asset pays dividends at a rate $r _ { \mathrm { d i v } } > r _ { \mathrm { : } }$ , then the basis is positive: 

$$
b (t, T) = S (t) \left(1 - \mathrm{e} ^ {\left(r - r _ {\text {div}}\right) (T - t)}\right).
$$

Going back to the problem of designing a hedge, suppose that we wish to sell an asset at time $t < T$ . To protect ourselves against a decrease in the asset price, at time 0 we can short a futures contract with futures price $f ( 0 , T )$ . At time t we shall receive $S ( t )$ from selling the asset plus the cash flow $f ( 0 , T ) - f ( t , T )$ due to marking to market (for simplicity, we neglect any intermediate cash flow, assuming that t is the first instance when marking to market takes place), that is, we obtain 

$$
f (0, T) + S (t) - f (t, T) = f (0, T) + b (t, T).
$$

The price $f ( 0 , T )$ is known at time 0, so the risk involved in the hedging position will be related to the unknown level of the basis. This uncertainty is mainly concerned with unknown future interest rates. 

If the goal of a hedger is to minimise risk, it may be best to use a certain optimal hedge ratio, that is to enter into N futures contracts, with N not necessarily equal to the number of shares of the underlying asset held. To see this compute the risk as measured by the variance of the basis $b _ { N } ( t , T ) =$ $S ( t ) - N f ( t , T )$ : 

$$
\mathrm{Var} (b _ {N} (t, T)) = \sigma_ {S (t)} ^ {2} + N ^ {2} \sigma_ {f (t, T)} ^ {2} - 2 N \sigma_ {S (t)} \sigma_ {f (t, T)} \rho_ {S (t) f (t, T)},
$$

where $\rho _ { S ( t ) f ( t , T ) }$ is the correlation coeficient between the spot and futures prices, and $\sigma _ { S ( t ) } , \sigma _ { f ( t , T ) }$ are the standard deviations. The variance is a quadratic function in N and has a minimum at 

$$
N = \rho_ {S (t) f (t, T)} \frac {\sigma_ {S (t)}}{\sigma_ {f (t , T)}},
$$

which is the optimal hedge ratio. 

## Exercise 6.9

Find the optimal hedge ratio if the interest rates are constant. 

Futures on Stock Index. A stock exchange index is a weighted average of a selection of stock prices with weights proportional to the market capitalisation of stocks. An index of this kind will be approximately proportional to the value of the market portfolio (see Chapter 5) if the chosen set of stocks is large enough. For example, the Standard and Poor Index S&P500 is computed using 500 stocks, representing about 80% of trade at the New York Stock Exchange. For the purposes of futures markets the index can be treated as a security. This is because the index can be identified with a portfolio, even though in practice transaction costs would impede trading in this portfolio. The futures prices $f ( n , T )$ , expressed in index points, are assumed to satisfy the same conditions as before. Marking to market is given by the diference $f ( n , T ) - f ( n - 1 , T )$ 

multiplied by a fixed amount ($500 for futures on S&P500). If the number of stocks included in the index is large, it is possible and convenient to assume that the index is an asset with dividends paid continuously. 

## Exercise 6.10

Suppose that the value of a stock exchange index is 13, 500, the futures price for delivery in 9 months is 14, 100 index points, and the interest rate is 8%. Find the dividend yield. 

Our goal in this section is to study applications of index futures for hedging based on the Capital Asset Pricing Model introduced in Chapter 5. As we know, see (5.19), the expected return on a portfolio over a time step of length $\tau$ is given by 

$$
\mu_ {V} = r _ {F} + (\mu_ {M} - r _ {F}) \beta_ {V},
$$

where $\beta _ { V }$ is the beta coeficient of the portfolio, $\mu _ { M }$ is the expected return on the market portfolio and $r _ { F }$ is the risk-free return over one time step. By $V ( n )$ we shall denote the value of the portfolio at the nth time step. We assume for simplicity that the index is equal to the value of the market portfolio, so that the futures prices are given by 

$$
f (n, T) = M (n) (1 + r _ {F}) ^ {T - n},
$$

M(n) being the value of the market portfolio at the nth time step. (Here we use discrete time and ordinary returns together with periodic compounding in the spirit of Portfolio Theory.) 

We can form a new portfolio with value $\widetilde V ( n )$ by supplementing the original portfolio with N short futures contracts on the index with delivery time $T .$ The initial value $\widetilde V ( 0 )$ of the new portfolio is the same as the value $V ( 0 )$ of the original portfolio, since it costs nothing to initiate a futures contract. The value 

$$
\widetilde {V} (n) = V (n) - N (f (n, T) - f (n - 1, T))
$$

of the new portfolio at the nth step includes the marking to market cash flow. The return on the new portfolio over the first step is 

$$
K _ {\tilde {V}} = \frac {\widetilde {V} (1) - \widetilde {V} (0)}{\widetilde {V} (0)} = \frac {V (1) - N (f (1 , T) - f (0 , T)) - V (0)}{V (0)}.
$$

We shall show that the beta coeficient $\beta _ { \widetilde { V } }$ of the new portfolio can be modified arbitrarily by a suitable choice of the futures position N. 

## Proposition 6.6

If 

$$
N = (\beta_ {V} - a) \frac {(1 + r _ {F}) V (0)}{f (0 , T)},
$$

then $\beta _ { \widetilde { V } } = a$ for any given number a. 

Proof 

We shall compute the beta coeficient from the definition: 

$$
\begin{array}{r l} & {\beta_ {\widetilde {V}} = \mathrm{Cov} (K _ {\widetilde {V}}, K _ {M}) / \sigma_ {M} ^ {2}} \\ & {\quad = \mathrm{Cov} (K _ {V}, K _ {M}) / \sigma_ {M} ^ {2} - \frac {1}{V (0)} \mathrm{Cov} (N (f (1, T) - f (0, T)), K _ {M}) / \sigma_ {M} ^ {2},} \end{array}
$$

where $K _ { M }$ is the return on the market portfolio and $K _ { V }$ the return on the portfolio without futures. Since Cov $( f ( 0 , T ) , K _ { M } ) = 0$ and covariance is linear with respect to each argument, 

$$
\operatorname{Cov} (N (f (1, T) - f (0, T)), K _ {M}) = N \operatorname{Cov} (f (1, T), K _ {M}).
$$

Inserting the futures price $f ( 1 , T ) = M ( 1 ) ( 1 + r _ { F } ) ^ { T - 1 }$ , we have 

$$
\operatorname{Cov} (f (1, T), K _ {M}) = (1 + r _ {F}) ^ {T - 1} \operatorname{Cov} (M (1), K _ {M}).
$$

Again by the linearity of covariance in each argument 

$$
\operatorname{Cov} (M (1), K _ {M}) = M (0) \operatorname{Cov} (\frac {M (1) - M (0)}{M (0)}, K _ {M}) = M (0) \sigma_ {M} ^ {2}.
$$

Subsequent substitutions give 

$$
\beta_ {\tilde {V}} = \beta_ {V} - \frac {(1 + r _ {F}) ^ {T - 1} N M (0)}{V (0)} = \beta_ {V} - N \frac {f (0 , T)}{V (0) (1 + r _ {F})},
$$

which implies the asserted property. 

## Corollary 6.7

If $a = 0$ , then $\mu _ { \tilde { V } } = r _ { F }$ 

## Example 6.4

Suppose that the index drops from $M ( 0 ) = 8 9 0$ down to $M ( 1 ) = 8 5 0$ , that is, by 4.49% within one time step. Suppose further that the risk-free rate is 1%. 

This means that the futures prices on the index (with delivery after 3 steps) are 

$$
\begin{array}{l} f (0, 3) = M (0) (1 + r _ {F}) ^ {3} = 8 9 0 \times 1. 0 1 ^ {3} \cong 9 1 6. 9 7, \\ f (1, 3) = M (1) (1 + r _ {F}) ^ {3} = 8 5 0 \times 1. 0 1 ^ {2} \cong 8 6 7. 0 9. \end{array}
$$

Consider a portfolio with $\beta _ { V } = 1 . 5$ and initial value V(0) = 100 dollars. This portfolio will have negative expected return 

$$
\begin{array}{r} \mu_ {V} = r _ {F} + (\mu_ {M} - r _ {F}) \beta_ {V} \\ \cong 1\% + (- 4. 49\% - 1\%) 1. 5 \cong - 7. 24\%. \end{array}
$$

To construct a new portfolio with $\beta _ { \widetilde { V } } ~ = ~ 0$ we can supplement the original portfolio with 

$$
N = \beta_ {V} \frac {(1 + r _ {F}) V (0)}{f (0 , 3)} \cong 1. 5 \times \frac {1 . 0 1 \times 1 0 0}{9 1 6 . 9 7} \cong 0. 1 6 5 2
$$

short forward contracts on the index with delivery after 3 steps. 

Suppose that the actual return on the original portfolio during the first time step happens to be equal to the expected return. This gives $V ( 1 ) \cong 9 2 . 7 6$ dollars. Marking to market gives a payment of 

$$
- N (f (1, 3) - f (0, 3)) \cong - 0. 1 6 5 2 \times (8 6 7. 0 9 - 9 1 6. 9 7) \cong 8. 2 4
$$

dollars due to the holder of $N \cong 0 . 1 6 5 2$ short forward contracts. This makes the new portfolio worth 

$$
\widetilde {V} (1) = V (1) - N \left(f (1, 3) - f (0, 3)\right) \cong 9 2. 7 6 + 8. 2 4 = 1 0 1. 0 0
$$

dollars at time 1, matching the risk-free growth exactly. 

## Exercise 6.11

Perform the same calculations in the case when the index increases from 890 to 920. 

## Remark 6.7

The ability to adjust the beta of a portfolio is valuable to investors who may wish either to reduce or to magnify the systematic risk. For example, suppose that an investor is able to design a portfolio with superior average performance to that of the market. By entering into a futures position such that the beta of the resulting portfolio is zero, the investor will be hedged against adverse movements of the market. This is crucial in the event of recession, so that the superior performance of the portfolio as compared to the market can be turned into a profit despite a decline in the market. On the other hand, should the market show some growth, the expected return on the hedged portfolio will be reduced by comparison because the futures position will result in a loss. 

It needs to be emphasized that this type of hedging with futures works only on average. In particular, setting the beta coeficient to zero will not make the investment risk-free. 

Let us conclude this chapter with a surprising application of index futures. 

## Example 6.5

In emerging markets short sales are rarely available. This was the case in Poland in the late 1990’s. However, index futures were traded. Due to the fact that one of the indices (WIG20) was composed of 20 stocks only, it was possible to manufacture a short sale of any stock among those 20 by entering into a short futures position on the index, combined with purchasing a suitable portfolio of the remaining 19 stocks. With a larger number of stocks comprising the index the transaction costs would have been too high to make such a construction practicable. 

This page intentionally left blank 

Options: General Properties 

In Chapters 1 and 4 we have seen simple examples of call and put options in a one-step discrete-time setting. Here we shall establish some fundamental properties of options, looking at them from a wider perspective and using continuous time. Nevertheless, many conclusions will also be valid in discrete time. Chapter 8 will be devoted to pricing and hedging options. 

## 7.1 Definitions

A European call option is a contract giving the holder the right to buy an asset, called the underlying, for a price X fixed in advance, known as the exercise price or strike price, at a specified future time T, called the exercise or expiry time. A European put option gives the right to sell the underlying asset for the strike price X at the exercise time T. 

An American call or put option gives the right to buy or, respectively, to sell the underlying asset for the strike price X at any time between now and a specified future time T, called the expiry time. In other words, an American option can be exercised at any time up to and including expiry. 

The term ‘underlying asset’ has quite general scope. Apart from typical assets such as stocks, commodities or foreign currency, there are options on stock indices, interest rates, or even on the snow level at a ski resort. Some underlying assets may be impossible to buy or sell. The option is then cleared in cash in a fashion which resembles settling a bet. For example, the holder of a European call option on the Standard and Poor Index (see page 141) with strike price 800 will gain if the index turns out to be 815 on the exercise date. The writer of the option will have to pay the holder an amount equal to the diference $8 1 5 - 8 0 0 = 1 5$ multiplied by a fixed sum of money, say by $100. No payment will be due if the index turns out to be lower than 800 on the exercise date. 

An option is determined by its payof, which for a European call is 

$$
\left\{ \begin{array}{l l} S (T) - X & \text { if } S (T) > X, \\ 0 & \text { otherwise }. \end{array} \right.
$$

This payof is a random variable, contingent on the price $S ( T )$ of the underlying on the exercise date T. (This explains why options are often referred to as contingent claims.) It is convenient to use the notation 

$$
x ^ {+} = \left\{ \begin{array}{l l} x & \text {if} x > 0, \\ 0 & \text {otherwise.} \end{array} \right.
$$

for the positive part of a real number x. Then the payof of a European call option can be written as $( S ( T ) - X ) ^ { + }$ . For a put option the payof is $( X -$ $S ( T ) ) ^ { + }$ 

Since the payofs are non-negative, a premium must be paid to buy an option. If no premium had to be paid, an investor purchasing an option could under no circumstances lose money and would in fact make a profit whenever the payof turned out to be positive. This would be contrary to the No-Arbitrage Principle. The premium is the market price of the option. 

Establishing bounds and some general properties for option prices is the primary goal of the present chapter. The next chapter will be devoted to de tailed techniques of computing these prices. We assume that options are freely traded, that is, can readily be bought and sold at the market price. The prices of calls and puts will be denoted by $C ^ { \mathrm { E } } , P ^ { \mathrm { E } }$ for European options and $C ^ { \mathrm { A } } , P ^ { \mathrm { A } }$ for American options, respectively. The same constant interest rate r will apply for lending and borrowing money without risk, and continuous compounding will be used. 

## Example 7.1

On 22 March 1997 European calls on Rolls-Royce stock with strike price 220 pence to be exercised on 22 May 1997 traded at 19.5 pence at the London International Financial Futures Exchange (LIFFE). Suppose that the purchase of such an option was financed by a loan at 5.23% compounded continuously, so that $1 9 . 5 \mathrm { e } ^ { 0 . 0 5 2 3 \times \frac { 2 } { 1 2 } } \cong 1 9 . 6 7$ pence would have to be paid back on the exercise date. The investment would bring a profit if the stock price turned out to be higher than $2 2 0 + 1 9 . 6 7 = 2 3 9 . 6 7$ pence on the exercise date. 

## Exercise 7.1

Find the stock price on the exercise date for a European put option with strike price $36 and exercise date in three months to produce a profit of $3 if the option is bought for $4.50, financed by a loan at 12% compounded continuously. 

The gain of an option buyer (writer) is the payof modified by the premium $C ^ { \mathrm { E } }$ or $P ^ { \mathrm { E } }$ paid (received) for the option. At time T the gain of the buyer of a European call is $( S ( T ) - X ) ^ { + } - C ^ { \mathrm { E } } \mathrm { e } ^ { r T }$ , where the time value of the premium is taken into account. For the buyer of a European put the gain is $( X - S ( T ) ) ^ { + } -$ $P ^ { \mathrm { E } } \mathrm { e } ^ { r T }$ . These gains are illustrated in Figure 7.1. For the writer of an option the gains are $C ^ { \mathrm { E } } \mathrm { e } ^ { r T } - ( S ( T ) - X ) ^ { + }$ for a call and $P ^ { \mathrm { E } } \mathrm { e } ^ { r T } - ( X - S ( T ) ) ^ { + }$ for a put option. Note that the potential loss for a buyer of a call or put is always limited to the premium paid. For a writer of an option the loss can be much higher, even unbounded in the case of a call option. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/68ca395c4e60a580d8e25649dcde3846a82a0b79df356cdec1d23654e68400a4.jpg)



Figure 7.1 Payofs (solid lines) and gains (broken lines) for a buyer of Euro pean calls and puts


## Exercise 7.2

Find the expected gain (or loss) for a holder of a European call option with strike price $90 to be exercised in 6 months if the stock price on the exercise date may turn out to be $87, $92 or $97 with probability $\textstyle { \frac { 1 } { 3 } }$ each, given that the option is bought for $8, financed by a loan at 9% compounded continuously. 

## 7.2 Put-Call Parity

In this section we shall make an important link between the prices of European call and put options. 

Consider a portfolio constructed by and writing and selling one put and buying one call option, both with the same strike price X and exercise date T. Adding the payofs of the long position in calls and the short position in puts, we obtain the payof of a long forward contract with forward price X and delivery time T. Indeed, if $S ( T ) \geq X$ , then the call will pay $S ( T ) - X$ and the put will be worthless. If $S ( T ) < X$ , then the call will be worth nothing and the writer of the put will need to pay $X - S ( T )$ . In either case, the value of the portfolio will be $S ( T ) - X$ at expiry, the same as for the long forward position, see Figure 7.2. As a result, the current value of such a portfolio of options should be that of the forward contract, which is $S ( 0 ) - X \mathrm { e } ^ { - r T }$ , see Remark 6.3. This motivates the theorem below. Even though the theorem follows from the above intuitive argument, we shall give a diferent proof with a view to possible generalisations. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/aaca71bfbd7f722117ccaabc73c6e517040e19ecfb96f84c9fa57da5a68e2df3.jpg)



Figure 7.2 Long forward payof constructed from calls and puts


## Theorem 7.1 (Put-Call Parity)

For a stock that pays no dividends the following relation holds between the prices of European call and put options, both with exercise price X and exercise time T: 

$$
C ^ {\mathrm{E}} - P ^ {\mathrm{E}} = S (0) - X \mathrm{e} ^ {- r T}.\tag{7.1}
$$

Proof 

Suppose that 

$$
C ^ {\mathrm{E}} - P ^ {\mathrm{E}} > S (0) - X \mathrm{e} ^ {- r T}.\tag{7.2}
$$

In this case an arbitrage strategy can be constructed as follows: At time 0 

buy one share for $S ( 0 )$ ; 

buy one put option for $P ^ { \mathrm { E } }$ ; 

write and sell one call option for $C ^ { \mathrm { E } }$ ; 

invest the sum $C ^ { \mathrm { E } } { - } P ^ { \mathrm { E } } { - } S ( 0 )$ (or borrow, if negative) on the money market at the interest rate r. 

The balance of these transactions is 0. Then, at time $T$ 

close out the money market position, collecting (or paying, if negative) the sum $( C ^ { \mathrm { E } } - P ^ { \mathrm { E } } - S ( 0 ) ) \mathrm { e } ^ { r T }$ ; 

sell the share for X either by exercising the put if $S ( T ) \leq X$ or settling the short position in calls if $S ( T ) > X$ 

The balance will be $( C ^ { \mathrm { E } } - P ^ { \mathrm { E } } - S ( 0 ) ) \mathrm { e } ^ { r T } + X$ , which is positive by (7.2), contradicting the No-Arbitrage Principle. 

Now suppose that 

$$
C ^ {\mathrm{E}} - P ^ {\mathrm{E}} <   S (0) - X \mathrm{e} ^ {- r T}.\tag{7.3}
$$

Then the following reverse strategy will result in arbitrage: At time 0 

sell short one share for $S ( 0 )$ 

write and sell a put option for $P ^ { \mathrm { E } }$ ; 

buy one call option for $C ^ { \mathrm { E } }$ ; 

invest the sum $S ( 0 ) { \mathrm { - } } C ^ { \mathrm { E } } { + } P ^ { \mathrm { E } }$ (or borrow, if negative) on the money marke at the interest rate r. 

The balance of these transactions is 0. At time $T$ 

close out the money market position, collecting (or paying, if negative) the sum $( S ( 0 ) - C ^ { \mathrm { E } } + P ^ { \mathrm { E } } ) \mathrm { e } ^ { r T }$ ; 

buy one share for X either by exercising the call if $S ( T ) > X$ or settling the short position in puts if $S ( T ) \leq X$ , and close the short position in stock. 

The balance will be $( S ( 0 ) - C ^ { \mathrm { E } } + P ^ { \mathrm { E } } ) \mathrm { e } ^ { r T } - X$ , positive by (7.3), once again contradicting the No-Arbitrage Principle. □ 

## Exercise 7.3

Suppose that a stock paying no dividends is trading at $15.60 a share. European calls on the stock with strike price $15 and exercise date in three months are trading at $2.83. The interest rate is $r = 6 . 7 2 \%$ , compounded continuously. What is the price of a European put with the same strike price and exercise date? 

## Exercise 7.4

European call and put options with strike price $24 and exercise date in six months are trading at $5.09 and $7.78. The price of the underlying stock is $20.37 and the interest rate is 7.48%. Find an arbitrage opportunity. 

## Remark 7.1

We can make a simple but powerful observation based on Theorem 7.1: The prices of European calls and puts depend in the same way on any variables absent in the put-call parity relation (7.1). In other words, the diference of these prices does not depend on such variables. As an example, consider the expected return on stock If the price of a call should grow along with the expected return, which on first sight seems consistent with intuition because higher stock prices mean higher payofs on calls, then the price of a put would also grow. The latter, however, contradicts common sense because higher stock prices mean lower payofs on puts. Because of this, one could argue that put and call prices should be independent of the expected return on stock. We shall see that this is indeed the case once the Black–Scholes formula is derived for call and put options in Chapter 8. 

Following the argument presented at the beginning of this section, we can reformulate put-call parity as follows: 

$$
C ^ {\mathrm{E}} - P ^ {\mathrm{E}} = V _ {X} (0),\tag{7.4}
$$

where $V _ { X } ( 0 )$ is the value of a long forward contract, see (6.10). Note that if X is equal to the theoretical forward price $S ( 0 ) \mathrm { e } ^ { r T }$ of the asset, then the value of the forward contract is zero, $V _ { X } ( 0 ) = 0$ , and so $C ^ { \mathrm { E } } = P ^ { \mathrm { E } }$ . Formula (7.4) allows us to generalise put-call parity by drawing on the relationships established in Remark 6.3. Namely, if the stock pays a dividend between times 0 and T, then $V _ { X } ( 0 ) = S ( 0 ) - \mathrm { { d i v } } _ { 0 } - X \mathrm { { e } } ^ { - r T }$ , where div<sub>0</sub> is the present value of the dividend. It follows that 

$$
C ^ {\mathrm{E}} - P ^ {\mathrm{E}} = S (0) - \operatorname{div} _ {0} - X \mathrm{e} ^ {- r T}.\tag{7.5}
$$

If dividends are paid continuously at a rate $r _ { \mathrm { d i v } }$ , then $\begin{array} { r } { V _ { X } ( 0 ) = S ( 0 ) \mathrm { e } ^ { - r _ { \mathrm { d i v } } T } - } \end{array}$ $X \mathrm { e } ^ { - r T }$ , so 

$$
C ^ {\mathrm{E}} - P ^ {\mathrm{E}} = S (0) \mathrm{e} ^ {- r _ {\mathrm{div}} T} - X \mathrm{e} ^ {- r T}.\tag{7.6}
$$

Exercise 7.5 

Outline an arbitrage proof of (7.5). 

Exercise 7.6 

Outline an arbitrage proof of (7.6). 

## Exercise 7.7

For the data in Exercise 6.5, find the strike price for European calls and puts to be exercised in six months such that $C ^ { \mathrm { E } } = P ^ { \mathrm { E } }$ 

For American options put-call parity gives only an estimate, rather than a strict equality involving put and call prices. 

## Theorem 7.2 (Put-Call Parity Estimates)

The prices of American put and call options with the same strike price X and expiry time T on a stock that pays no dividends satisfy 

$$
S (0) - X \mathrm{e} ^ {- r T} \geq C ^ {\mathrm{A}} - P ^ {\mathrm{A}} \geq S (0) - X.
$$

## Proof

Suppose that the first inequality fails to hold, that is, 

$$
C ^ {\mathrm{A}} - P ^ {\mathrm{A}} - S (0) + X \mathrm{e} ^ {- r T} > 0.
$$

Then we can write and sell a call, and buy a put and a share, financing the transactions on the money market. If the holder of the American call chooses to exercise it at time $t \leq T$ , then we shall receive X for the share and settle the money market position, ending up with the put and a positive amount 

$$
\begin{array}{r l} & X + (C ^ {\mathrm{A}} - P ^ {\mathrm{A}} - S (0)) \mathrm{e} ^ {r t} = (X \mathrm{e} ^ {- r t} + C ^ {\mathrm{A}} - P ^ {\mathrm{A}} - S (0)) \mathrm{e} ^ {r t} \\ & \qquad \geq (X \mathrm{e} ^ {- r T} + C ^ {\mathrm{A}} - P ^ {\mathrm{A}} - S (0)) \mathrm{e} ^ {r t} > 0. \end{array}
$$

If the call option is not exercised at all, we can sell the share for X by exercising the put at time T and close the money market position, also ending up with a positive amount 

$$
X + (C ^ {\mathrm{A}} - P ^ {\mathrm{A}} - S (0)) \mathrm{e} ^ {r T} > 0.
$$

Now suppose that 

$$
C ^ {\mathrm{A}} - P ^ {\mathrm{A}} - S (0) + X <   0.
$$

In this case we can write and sell a put, buy a call and sell short one share, investing the balance on the money market. If the American put is exercised at time $t \leq T$ , then we can withdraw X from the money market to buy a share and close the short sale. We shall be left with the call option and a positive amount 

$$
(- C ^ {\mathrm{A}} + P ^ {\mathrm{A}} + S (0)) \mathrm{e} ^ {r t} - X > X \mathrm{e} ^ {r t} - X \geq 0.
$$

If the put is not exercised at all, then we can buy a share for X by exercising the call at time $T$ and close the short position in stock. On closing the money market position, we shall also end up with a positive amount 

$$
(- C ^ {\mathrm{A}} + P ^ {\mathrm{A}} + S (0)) \mathrm{e} ^ {r T} - X > X \mathrm{e} ^ {r T} - X > 0.
$$

The theorem, therefore, holds by the No-Arbitrage Principle. 

## Exercise 7.8

Modify the proof of Theorem 7.2 to show that 

$$
S (0) - X \mathrm{e} ^ {- r T} \geq C ^ {\mathrm{A}} - P ^ {\mathrm{A}} \geq S (0) - \operatorname{div} _ {0} - X
$$

for a stock paying a dividend between time 0 and the expiry time T, where div is the value of the dividend discounted to time 0. 

## Exercise 7.9

Modify the proof of Theorem 7.2 to show that 

$$
S (0) - X \mathrm{e} ^ {- r T} \geq C ^ {\mathrm{A}} - P ^ {\mathrm{A}} \geq S (0) \mathrm{e} ^ {- r _ {\mathrm{div}} T} - X
$$

for a stock paying dividends continuously at a rate $r _ { \mathrm { d i v } }$ 

## 7.3 Bounds on Option Prices

First of all, we note the obvious inequalities 

$$
C ^ {\mathrm{E}} \leq C ^ {\mathrm{A}}, \quad P ^ {\mathrm{E}} \leq P ^ {\mathrm{A}},\tag{7.7}
$$

for European and American options with the same strike price X and expiry time T. They hold because an American option gives at least the same rights as the corresponding European option. 

Figure 7.3 shows a scenario of stock prices in which the payof of a European call is zero at the exercise time T, whereas that of an American call will be positive if the option is exercised at an earlier time $t < T$ when the stock price $S ( t )$ is higher than X. Nevertheless, it does not necessarily follow that the inequalities in (7.7) can be replaced by strict ones; see Section 7.3.2, where it is shown that $C ^ { \mathrm { E } } = C ^ { \mathrm { A } }$ for call options on an asset that pays no dividends. 

Exercise 7.10 

Prove (7.7) by an arbitrage argument. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/d4bb13f77757073b6b068b8fd1e37397dcfa4606c4348e2b5626287d385bf0d0.jpg)



Figure 7.3 Scenario in which an American call can bring a positive payof, but a European call cannot


It is also obvious that the price of a call or put option has to be non-negative because an option of this kind ofers the possibility of a future gain with no liability. Therefore, 

$$
C ^ {\mathrm{E}} \geq 0, \quad P ^ {\mathrm{E}} \geq 0.
$$

Similar inequalities are of course valid for the more valuable American options. In fact the prices of options are nearly always strictly positive, except for some very special circumstances, for example, $C ^ { \mathrm { E } } = 0$ for a call option with strike price $X = 1 2 0$ dollars one day prior to exercise when the underlying stock is trading at $100 and daily price movements are limited by stock exchange regulations $\mathrm { t o \pm 1 0 \% }$ 

In what follows we are going to discuss some further simple bounds for the prices of European and American options. The advantage of such bounds is that they are universal. They are independent of any particular model of stock prices and follow from the No-Arbitrage Principle alone. 

## 7.3.1 European Options

We shall establish some upper and lower bounds on the prices of European call and put options. 

On the one hand, observe that 

$$
C ^ {\mathrm{E}} <   S (0).
$$

If the reverse inequality were satisfied, that is, if $C ^ { \mathrm { E } } ~ \ge ~ S ( 0 )$ , then we could write and sell the option and buy the stock, investing the balance on the money market. On the exercise date $T$ we could then sell the stock for min $( S ( T ) , X )$ , settling the call option. Our arbitrage profit would be $( C ^ { \mathrm { E } } - S ( 0 ) ) \mathrm { e } ^ { r T } + \operatorname* { m i n } ( S ( T ) , X ) > 0$ . This proves that $C ^ { \mathrm { E } } < S ( 0 )$ . On the 

other hand, we have the lower bound 

$$
S (0) - X \mathrm{e} ^ {- r T} \leq C ^ {\mathrm{E}},
$$

which follows immediately by put-call parity, since $P ^ { \mathrm { E } } \geq 0$ . Moreover, put-call parity implies that 

$$
P ^ {\mathrm{E}} <   X \mathrm{e} ^ {- r T},
$$

since $C ^ { \mathrm { E } } < S ( 0 )$ (0), and 

$$
- S (0) + X \mathrm{e} ^ {- r T} \leq P ^ {\mathrm{E}},
$$

since $C ^ { \mathrm { E } } \geq 0$ 

These results are summarised in the following proposition and illustrated in Figure 7.4. The shaded areas correspond to option prices that satisfy the bounds. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/b4f83129a6275a7e6742df1bb6127d1edbeb31757060a30442f962ecdac0d812.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/64c58b6f831f9a61b5dbaa7a9074eb97db6014da45e35bae5cd3b6b41745a753.jpg)



Figure 7.4 Bounds on European call and put prices


## Proposition 7.3

The prices of European call and put options on a stock paying no dividends satisfy the inequalities 

$$
\begin{array}{r} \max \{0, S (0) - X \mathrm{e} ^ {- r T} \} \leq C ^ {\mathrm{E}} <   S (0), \\ \max \{0, - S (0) + X \mathrm{e} ^ {- r T} \} \leq P ^ {\mathrm{E}} <   X \mathrm{e} ^ {- r T}. \end{array}
$$

For dividend-paying stock the bounds are 

$$
\begin{array}{c} \max \{0, S (0) - \operatorname{div} _ {0} - X \mathrm{e} ^ {- r T} \} \leq C ^ {\mathrm{E}} <   S (0) - \operatorname{div} _ {0}, \\ \max \{0, - S (0) + \operatorname{div} _ {0} + X \mathrm{e} ^ {- r T} \} \leq P ^ {\mathrm{E}} <   X \mathrm{e} ^ {- r T}. \end{array}
$$

Exercise 7.11 

Prove the above bounds on option prices for dividend-paying stock. 

## Exercise 7.12

For dividend-paying stock sketch the regions of call and put prices de termined by the bounds. 

## 7.3.2 European and American Calls on Non-Dividend Paying Stock

Consider European and American call options with the same strike price X and expiry time T. We know that $C ^ { \mathrm { { A } } } \geq C ^ { \mathrm { { E } } }$ , since the American option gives more rights than its European counterpart. If the underlying stock pays no dividends, then $C ^ { \mathrm { E } } \geq S ( 0 ) - X \mathrm { e } ^ { - r T }$ by Proposition 7.3. It follows that $C ^ { \mathrm { A } } > S ( 0 ) - X$ if $r > 0$ . Because the price of the American option is greater than the payof, the option will sooner be sold than exercised at time 0. 

The choice of 0 as the starting time is of course arbitrary. Replacing 0 by any given $t < T$ , we can show by the same argument that the American option will not be exercised at time t. This means that the American option will in fact never be exercised prior to expiry. This being so, it should be equivalent to the European option. In particular, their prices should be equal, leading to the following theorem. 

## Theorem 7.4

The prices of European and American call options on a stock that pays no dividends are equal, $C ^ { \mathrm { { A } } } = C ^ { \mathrm { { E } } }$ , whenever the strike price X and expiry time $T$ are the same for both options. 

## Proof

We already know that $C ^ { \mathrm { { A } } } \geq C ^ { \mathrm { { E } } }$ , see (7.7) and Exercise 7.10. If $C ^ { \mathrm { A } } > C ^ { \mathrm { E } }$ , then write and sell an American call and buy a European call, investing the balance $C ^ { \mathrm { { A } } } - C ^ { \mathrm { { E } } }$ at the interest rate r. If the American call is exercised at time $t \leq T$ then borrow a share and sell it for X to settle your obligation as writer of the call option, investing X at rate $r .$ Then, at time $T$ you can use the European call to buy a share for X and close your short position in stock. Your arbitrage profit will be $( C ^ { \mathrm { { A } } } - C ^ { \mathrm { { E } } } ) \mathrm { { e } } ^ { r T } + X \mathrm { { e } } ^ { r ( T - t ) } - X > 0$ . If the American option is not exercised at all, you will end up with the European option and an arbitrage profit of $( C ^ { \mathrm { A } } - C ^ { \mathrm { E } } ) \mathrm { e } ^ { r T } > 0$ . This proves that $C ^ { \mathrm { { A } } } = C ^ { \mathrm { { E } } }$ □ 

Theorem 7.4 may seem counter-intuitive at first sight. While it is possible to gain $S ( t ) - X$ by exercising an American call option if $S ( t ) > X$ at time $t < T$ , this is not so with a European option, which cannot be exercised at time $t < T$ . It might, therefore, appear that the American call option should be more valuable than the European one. Nevertheless, there is no contradiction. Even though a European call option cannot be exercised at time $t < T$ , it can be sold for at least $S ( t ) - X$ 

The situation is diferent for dividend-paying stock. Example 8.2 in the next chapter shows a case in which an American call option is worth more than its European counterpart and should be exercised prior to expiry, at least in some scenarios. 

On the other hand, it often happens that an American put should be exercised prematurely even if the underlying stock pays no dividends, as in the following example. 

## Example 7.2

Suppose that the stock price is $10, the strike price of an American put expiring in one year is $80, and the interest rate is 16%. Exercising the option now, we can gain $\$ 70$ , which can be invested at 16% to become $81.20 after one year. The value of a put option cannot possibly exceed the strike price, see (7.8), so we are definitely better of by exercising the option early. 

## 7.3.3 American Options

First we consider options on non-dividend paying stock. In this case the price of an American call is equal to that of a European call, $C ^ { \mathrm { { A } } } = C ^ { \mathrm { { E } } }$ , see Theorem 7.4, so it must satisfy the same bounds as in Proposition 7.3. For an American put we have 

$$
- S (0) + X \leq P ^ {\mathrm{A}}
$$

because $P ^ { \mathrm { A } }$ cannot be less than the payof of the option at time 0. This gives a sharper lower bound than that for a European put. However, the upper bound has to be relaxed as compared to a European put. Namely, 

$$
P ^ {\mathrm{A}} <   X.\tag{7.8}
$$

Indeed, if $P ^ { \mathrm { A } } \geq X$ , then the following arbitrage strategy could be constructed: Write and sell an American put for $P ^ { \mathrm { A } }$ and invest this amount at the interest rate r. If the put is exercised at time $t \leq T$ , then a share of the underlying stock will have to be bought for X and can then be sold for $S ( t )$ . The final cash balance will be positive, $P ^ { \mathrm { A } } \mathrm { e } ^ { r t } - X + S ( t ) > 0$ . If the option is not exercised at all, the final balance will also be positive, $P ^ { \mathrm { A } } \mathrm { e } ^ { r T } > 0$ , at expiry. These results can be summarised as follows. 

## Proposition 7.5

The prices of American call and put options on a stock paying no dividends satisfy the inequalities 

$$
\begin{array}{c} \max \{0, S (0) - X \mathrm{e} ^ {- r T} \} \leq C ^ {\mathrm{A}} <   S (0), \\ \max \{0, - S (0) + X \} \leq P ^ {\mathrm{A}} <   X. \end{array}
$$

Next we consider options on dividend-paying stock. The lower bounds for European options imply that $S ( 0 ) - \mathrm { { d i v } } _ { 0 } - X \mathrm { { e } } ^ { - r T } \leq C ^ { \mathrm { { E } } } \leq C ^ { \mathrm { { A } } }$ and $- S ( 0 ) +$ $\mathrm { d i v } _ { 0 } + X \mathrm { e } ^ { - r T } \leq P ^ { \mathrm { E } } \leq P ^ { \mathrm { A } }$ . But because the price of an American option cannot be less than its payof at any time, we also have $S ( 0 ) - X \leq C ^ { \mathrm { A } }$ and $X - S ( 0 ) \le P ^ { \mathtt { A } }$ . Moreover, the upper bounds $C ^ { \mathrm { A } } < S ( 0 )$ and $P ^ { \mathrm { A } } < X$ can be established in a similar manner as for non-dividend paying stock. All these inequalities can be summarised as follows: For dividend-paying stock 

$$
\begin{array}{c} \max \{0, S (0) - \operatorname{div} _ {0} - X \mathrm{e} ^ {- r T}, S (0) - X \} \leq C ^ {\mathrm{A}} <   S (0), \\ \max \{0, - S (0) + \operatorname{div} _ {0} + X \mathrm{e} ^ {- r T}, - S (0) + X \} \leq P ^ {\mathrm{A}} <   X. \end{array}
$$

## Exercise 7.13

Prove by an arbitrage argument that $C ^ { \mathrm { A } } < S ( 0 )$ for an American call on dividend-paying stock. 

## 7.4 Variables Determining Option Prices

The option price depends on a number of variables. These can be variables characterising the option, such as the strike price X or expiry time $T ,$ variables describing the underlying asset, for example, the current price $S ( 0 )$ or dividend rate $r _ { \mathrm { d i v } }$ , variables connected with the market as a whole such as the risk-free rate r, and of course the running time t. 

We shall analyse option prices as functions of one of the variables, keeping the remaining variables constant. This is a significant simplification because usually a change in one variable is accompanied by changes in some or all of the other variables. Nevertheless, even the simplified situation will provide interesting insights. 

## 7.4.1 European Options

Dependence on the Strike Price. We shall consider options on the same underlying asset and with the same exercise time T, but with diferent values of the strike price X. The call and put prices will be denoted by $C ^ { \mathrm { E } } ( X )$ and, respectively, $P ^ { \mathrm { E } } ( X )$ to emphasise their dependence on X. All remaining variables such as the exercise time $T ,$ , running time t and the underlying asset price $S ( 0 )$ will be kept fixed for the time being. 

## Proposition 7.6

If $X ^ { \prime } < X ^ { \prime \prime }$ , then 

$$
\begin{array}{l} C ^ {\mathrm{E}} (X ^ {\prime}) > C ^ {\mathrm{E}} (X ^ {\prime \prime}), \\ P ^ {\mathrm{E}} (X ^ {\prime}) <   P ^ {\mathrm{E}} (X ^ {\prime \prime}). \end{array}
$$

This means that $C ^ { \mathrm { E } } ( X )$ is a strictly decreasing and $P ^ { \mathrm { E } } ( X )$ a strictly increasing function of X. 

These inequalities are obvious. The right to buy at a lower price is more valuable than the right to buy at a higher price. Similarly, it is better to sell an asset at a higher price than at a lower one. 

## Exercise 7.14

Give a rigorous arbitrage argument to prove the inequalities in Proposition 7.6. 

Proposition 7.7 

If $X ^ { \prime } < X ^ { \prime \prime }$ , then 

$$
\begin{array}{l} C ^ {\mathrm{E}} (X ^ {\prime}) - C ^ {\mathrm{E}} (X ^ {\prime \prime}) <   \mathrm{e} ^ {- r T} (X ^ {\prime \prime} - X ^ {\prime}), \\ P ^ {\mathrm{E}} (X ^ {\prime \prime}) - P ^ {\mathrm{E}} (X ^ {\prime}) <   \mathrm{e} ^ {- r T} (X ^ {\prime \prime} - X ^ {\prime}). \end{array}
$$

Proof 

By put-call parity (7.1) 

$$
C ^ {\mathrm{E}} (X ^ {\prime}) - P ^ {\mathrm{E}} (X ^ {\prime}) = S (0) - X ^ {\prime} \mathrm{e} ^ {- r T},
$$

$$
C ^ {\mathrm{E}} (X ^ {\prime \prime}) - P ^ {\mathrm{E}} (X ^ {\prime \prime}) = S (0) - X ^ {\prime \prime} \mathrm{e} ^ {- r T}.
$$

Subtracting, we get 

$$
\left(C ^ {\mathrm{E}} (X ^ {\prime}) - C ^ {\mathrm{E}} (X ^ {\prime \prime})\right) + \left(P ^ {\mathrm{E}} (X ^ {\prime \prime}) - P ^ {\mathrm{E}} (X ^ {\prime})\right) = (X ^ {\prime \prime} - X ^ {\prime}) \mathrm{e} ^ {- r T}.
$$

Since, by Proposition 7.6, both terms on the left-hand side are positive, each is strictly smaller than the right-hand side. □ 

## Remark 7.2

In the language of mathematics the inequalities mean that the call and put prices as functions of the strike price satisfy the Lipschitz condition with constant $\mathrm { e } ^ { - r T } < 1$ ， 

$$
\begin{array}{r} | C ^ {\mathrm{E}} (X ^ {\prime \prime}) - C ^ {\mathrm{E}} (X ^ {\prime}) | \leq \mathrm{e} ^ {- r T} | X ^ {\prime \prime} - X ^ {\prime} |, \\ | P ^ {\mathrm{E}} (X ^ {\prime \prime}) - P ^ {\mathrm{E}} (X ^ {\prime}) | \leq \mathrm{e} ^ {- r T} | X ^ {\prime \prime} - X ^ {\prime} |. \end{array}
$$

In particular, the slope of the graph of the option price as a function of the strike price is less than $4 5 ^ { \circ }$ . This is illustrated in Figure 7.5 for a call option. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/8a26fa71596f91f6cf6dcea47f739344ec83f230dcf40aeeaeb02411c3bb6a2f.jpg)



Figure 7.5 Lipschitz property of call prices $C ^ { \mathrm { E } } ( X )$


## Proposition 7.8

Let $X ^ { \prime } < X ^ { \prime \prime }$ and let $\alpha \in ( 0 , 1 )$ . Then 

$$
\begin{array}{l} C ^ {\mathrm{E}} (\alpha X ^ {\prime} + (1 - \alpha) X ^ {\prime \prime}) \leq \alpha C ^ {\mathrm{E}} (X ^ {\prime}) + (1 - \alpha) C ^ {\mathrm{E}} (X ^ {\prime \prime}), \\ P ^ {\mathrm{E}} (\alpha X ^ {\prime} + (1 - \alpha) X ^ {\prime \prime}) \leq \alpha P ^ {\mathrm{E}} (X ^ {\prime}) + (1 - \alpha) P ^ {\mathrm{E}} (X ^ {\prime \prime}). \end{array}
$$

In other words, $C ^ { \mathrm { E } } ( X )$ and $P ^ { \mathrm { E } } ( X )$ are convex functions of X. 

## Proof

For brevity, we put $X = \alpha X ^ { \prime } + ( 1 - \alpha ) X ^ { \prime \prime }$ . Suppose that 

$$
C ^ {\mathrm{E}} (X) > \alpha C ^ {\mathrm{E}} (X ^ {\prime}) + (1 - \alpha) C ^ {\mathrm{E}} (X ^ {\prime \prime}).
$$

We can write and sell an option with strike price X, and purchase α options with strike price $X ^ { \prime }$ and $1 - \alpha$ options with strike price $X ^ { \prime \prime }$ , investing the balance $C ^ { \operatorname { E } } ( X ) - \left( \alpha C ^ { \operatorname { E } } ( X ^ { \prime } ) + ( 1 - \alpha ) C ^ { \operatorname { E } } ( X ^ { \prime \prime } ) \right) > 0$ without risk. If the option with strike price X is exercised at expiry, then we shall have to pay $( S ( T ) - X ) ^ { + }$ We can raise the amount $\alpha \left( S ( T ) - X ^ { \prime } \right) ^ { + } + ( 1 - \alpha ) \left( S ( T ) - X ^ { \prime \prime } \right) ^ { + }$ by exercising α calls with strike $X ^ { \prime }$ and $1 - \alpha$ calls with strike $X ^ { \prime \prime }$ . In this way we will realise an arbitrage profit because of the following inequality, which is easy to verify (the details are left to the reader, see Exercise 7.15): 

$$
(S (T) - X) ^ {+} \leq \alpha (S (T) - X ^ {\prime}) ^ {+} + (1 - \alpha) (S (T) - X ^ {\prime \prime}) ^ {+}.\tag{7.9}
$$

Convexity for put options follows from that for calls by put-call parity (7.1). Alternatively, an arbitrage argument can be given along similar lines as for call options. □ 

Exercise 7.15 

Verify inequality (7.9). 

## Remark 7.3

According to Proposition 7.8, $C ^ { \mathrm { E } } ( X )$ and $P ^ { \mathrm { E } } ( X )$ are convex functions of X. Geometrically, this means that if two points on the graph of the function are joined with a straight line, then the graph of the function between the two points will lie below the line. This is illustrated in Figure 7.6 for call prices. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/236c846dadc0785ca9fc10b82ac161ba55847365cb21433a7902594275341e95.jpg)



Figure 7.6 Convexity of call prices $C ^ { \mathrm { E } } ( X )$


Dependence on the Underlying Asset Price. The current price $S ( 0 )$ of the underlying asset is given by the market and cannot be altered. However, we can consider an option on a portfolio consisting of x shares, worth $S = x S ( 0 )$ . The payof of a European call with strike price $X$ on such a portfolio to be exercised at time $T$ will be $( x S ( T ) - X ) ^ { + }$ . For a put the payof will be $( X - x S ( T ) ) ^ { + }$ . We shall study the dependence of option prices on S. Assuming that all remaining variables are fixed, we shall denote the call and put prices by $C ^ { \mathrm { E } } ( S )$ and $P ^ { \mathrm { E } } ( S )$ 

## Remark 7.4

Even though options on a portfolio of stocks are of little practical significance, the functions $C ^ { \mathrm { E } } ( S )$ and $P ^ { \mathrm { E } } ( S )$ are important because they also reflect the dependence of option prices on very sudden changes of the price of the underlying such that the remaining variables remain almost unaltered. 

## Proposition 7.9

If $S ^ { \prime } < S ^ { \prime \prime }$ , then 

$$
\begin{array}{l} C ^ {\mathrm{E}} (S ^ {\prime}) <   C ^ {\mathrm{E}} (S ^ {\prime \prime}), \\ P ^ {\mathrm{E}} (S ^ {\prime}) > P ^ {\mathrm{E}} (S ^ {\prime \prime}), \end{array}
$$

that is, $C ^ { \mathrm { E } } ( S )$ is a strictly increasing function and $P ^ { \mathrm { E } } ( S )$ a strictly decreasing function of S. 

## Proof

Suppose that $C ^ { \mathrm { E } } ( S ^ { \prime } ) \ge C ^ { \mathrm { E } } ( S ^ { \prime \prime } )$ for some $S ^ { \prime } < S ^ { \prime \prime }$ , where $S ^ { \prime } = x ^ { \prime } S ( 0 )$ and $S ^ { \prime \prime } =$ $x ^ { \prime \prime } S ( 0 )$ . We can write and sell a call on a portfolio with $x ^ { \prime }$ shares and buy a call on a portfolio with $x ^ { \prime \prime }$ shares, the two options sharing the same strike price $X$ and exercise time $T ,$ , and we can invest the balance $C ^ { \mathrm { E } } ( S ^ { \prime } ) - C ^ { \mathrm { E } } ( S ^ { \prime \prime } )$ without risk. Since $x ^ { \prime } < x ^ { \prime \prime }$ , the payofs satisfy $( x ^ { \prime } S ( T ) - X ) ^ { + } \leq ( x ^ { \prime \prime } S ( T ) - X ) ^ { + }$ with strict inequality whenever $X < x ^ { \prime \prime } S ( T )$ . If the option sold is exercised at time $T .$ , we can, therefore, exercise the other option to cover our liability and will be left with an arbitrage profit. 

The inequality for puts follows by a similar arbitrage argument. 

Exercise 7.16 

Prove the inequality in Proposition 7.9 for put options. 

Proposition 7.10 

Suppose that $S ^ { \prime } < S ^ { \prime \prime }$ . Then 

$$
C ^ {\mathrm{E}} (S ^ {\prime \prime}) - C ^ {\mathrm{E}} (S ^ {\prime}) <   S ^ {\prime \prime} - S ^ {\prime},
$$

$$
P ^ {\mathrm{E}} (S ^ {\prime}) - P ^ {\mathrm{E}} (S ^ {\prime \prime}) <   S ^ {\prime \prime} - S ^ {\prime}.
$$

## Proof

We employ put-call parity (7.1): 

$$
C ^ {\mathrm{E}} (S ^ {\prime \prime}) - P ^ {\mathrm{E}} (S ^ {\prime \prime}) = S ^ {\prime \prime} - X \mathrm{e} ^ {- r T},
$$

$$
C ^ {\mathrm{E}} (S ^ {\prime}) - P ^ {\mathrm{E}} (S ^ {\prime}) = S ^ {\prime} - X \mathrm{e} ^ {- r T}.
$$

Subtracting, we get 

$$
(C ^ {\mathrm{E}} (S ^ {\prime \prime}) - C ^ {\mathrm{E}} (S ^ {\prime})) + (P ^ {\mathrm{E}} (S ^ {\prime}) - P ^ {\mathrm{E}} (S ^ {\prime \prime})) = S ^ {\prime \prime} - S ^ {\prime}.
$$

Both terms on the left-hand side are non-negative by the previous theorem, so each is strictly less than the right-hand side. □ 

## Remark 7.5

A consequence of Proposition 7.10 is that the slope of the straight line joining two points on the graph of the call or put price as a function of S is less than $4 5 ^ { \circ }$ This is illustrated in Figure 7.7 for call options. In other words, the call and 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/a4bd73adc141ce40e390c2c11a9a911cceb855d87c0ba34a1decca059f332716.jpg)



Figure 7.7 Lipschitz property of call prices $C ^ { \mathrm { E } } ( S )$


put prices $C ^ { \mathrm { E } } ( S )$ and $P ^ { \mathrm { E } } ( S )$ satisfy the Lipschitz condition with constant 1, 

$$
\left| C ^ {\mathrm{E}} (S ^ {\prime \prime}) - C ^ {\mathrm{E}} (S ^ {\prime}) \right| \leq | S ^ {\prime \prime} - S ^ {\prime} |,
$$

$$
\left| P ^ {\mathrm{E}} (S ^ {\prime \prime}) - P ^ {\mathrm{E}} (S ^ {\prime}) \right| \leq | S ^ {\prime \prime} - S ^ {\prime} |.
$$

Proposition 7.11 

Let $S ^ { \prime } < S ^ { \prime \prime }$ and let $\alpha \in ( 0 , 1 )$ . Then 

$$
C ^ {\mathrm{E}} \left(\alpha S ^ {\prime} + (1 - \alpha) S ^ {\prime \prime}\right) \leq \alpha C ^ {\mathrm{E}} \left(S ^ {\prime}\right) + (1 - \alpha) C ^ {\mathrm{E}} \left(S ^ {\prime \prime}\right),
$$

$$
P ^ {\mathrm{E}} (\alpha S ^ {\prime} + (1 - \alpha) S ^ {\prime \prime}) \leq \alpha P ^ {\mathrm{E}} (S ^ {\prime}) + (1 - \alpha) P ^ {\mathrm{E}} (S ^ {\prime \prime}).
$$

This means that the call and put prices are convex functions of S. 

Proof 

We put $S = \alpha S ^ { \prime } + ( 1 - \alpha ) S ^ { \prime \prime }$ for brevity. Let $S ^ { \prime } = x ^ { \prime } S ( 0 ) , S ^ { \prime \prime } = x ^ { \prime \prime } S ( 0 )$ and $S = x S ( 0 ) , \mathrm { s o } x = \alpha x ^ { \prime } + ( 1 - \alpha ) x ^ { \prime \prime }$ . Suppose that 

$$
C ^ {\mathrm{E}} (S) > \alpha C ^ {\mathrm{E}} (S ^ {\prime}) + (1 - \alpha) C ^ {\mathrm{E}} (S ^ {\prime \prime}).
$$

We write and sell a call on a portfolio with x shares, and purchase α calls on a portfolio with $x ^ { \prime }$ shares and $1 - \alpha$ calls on a portfolio with $x ^ { \prime \prime }$ shares, investing the balance $C ^ { \mathrm { E } } ( S ) - \alpha C ^ { \mathrm { E } } ( S ^ { \prime } ) - ( 1 - \alpha ) C ^ { \mathrm { E } } ( S ^ { \prime \prime } )$ without risk. If the option sold is exercised at time T, then we shall have to pay $( x S ( T ) - X ) ^ { + }$ . To cover this liability we can exercise the other options. Since 

$$
(x S (T) - X) ^ {+} \leq \alpha (x ^ {\prime} S (T) - X) ^ {+} + (1 - \alpha) (x ^ {\prime \prime} S (T) - X) ^ {+},
$$

this is an arbitrage strategy. 

The inequality for put options can be proved by a similar arbitrage argument or using put-call parity. □ 

## 7.4.2 American Options

In general, American options have similar properties to their European counter parts. One dificulty is the absence of put-call parity; we only have the weaker estimates in Theorem 7.2. In addition, we have to take into account the possibility of early exercise. 

Dependence on the Strike Price. We shall denote the call and put prices by $C ^ { \mathrm { { A } } } ( X )$ and $P ^ { \mathrm { { A } } } ( X )$ to emphasise the dependence on $X$ , keeping any other variables fixed. 

The following proposition is obvious for the same reasons as for European options: Higher strike price makes the right to buy less valuable and the right to sell more valuable. 

Proposition 7.12 

If $X ^ { \prime } < X ^ { \prime \prime }$ , then 

$$
\begin{array}{l} C ^ {\mathrm{A}} (X ^ {\prime}) > C ^ {\mathrm{A}} (X ^ {\prime \prime}), \\ P ^ {\mathrm{A}} (X ^ {\prime}) <   P ^ {\mathrm{A}} (X ^ {\prime \prime}). \end{array}
$$

Exercise 7.17 

Give a rigorous arbitrage proof of Proposition 7.12. 

Proposition 7.13 

Suppose that $X ^ { \prime } < X ^ { \prime \prime }$ . Then 

$$
C ^ {\mathrm{A}} (X ^ {\prime}) - C ^ {\mathrm{A}} (X ^ {\prime \prime}) <   X ^ {\prime \prime} - X ^ {\prime},
$$

$$
P ^ {\mathrm{A}} (X ^ {\prime \prime}) - P ^ {\mathrm{A}} (X ^ {\prime}) <   X ^ {\prime \prime} - X ^ {\prime}.
$$

## Proof

Suppose that $X ^ { \prime } < X ^ { \prime \prime }$ , but $C ^ { \mathrm { A } } ( X ^ { \prime } ) - C ^ { \mathrm { A } } ( X ^ { \prime \prime } ) \ge X ^ { \prime \prime } - X ^ { \prime }$ . We write and sell a call with strike price $X ^ { \prime }$ , buy a call with strike price $X ^ { \prime \prime }$ and invest the balance $C ^ { \mathrm { { A } } } ( X ^ { \prime } ) - C ^ { \mathrm { { A } } } ( X ^ { \prime \prime } )$ without risk. If the written option is exercised at time $t \leq T$ , then we shall have to pay $( S ( t ) - X ^ { \prime } ) ^ { + }$ . Exercising the other option immediately, we shall receive $( S ( t ) - X ^ { \prime \prime } ) ^ { + }$ . Observe that 

$$
(S (t) - X ^ {\prime \prime}) ^ {+} - (S (t) - X ^ {\prime}) ^ {+} \geq - (X ^ {\prime \prime} - X ^ {\prime})
$$

with strict inequality whenever $S ( t ) < X ^ { \prime \prime }$ . Together with the risk-free invest ment, amounting to at least $X ^ { \prime \prime } - X ^ { \prime }$ , we shall therefore end up with a non negative sum of money, and in fact realise an arbitrage profit if $S ( t ) < X ^ { \prime \prime }$ 

The proof is similar for put options. 

## Theorem 7.14

Suppose that $X ^ { \prime } < X ^ { \prime \prime }$ and let $\alpha \in ( 0 , 1 )$ . Then 

$$
C ^ {\mathrm{A}} (\alpha X ^ {\prime} + (1 - \alpha) X ^ {\prime \prime}) \leq \alpha C ^ {\mathrm{A}} (X ^ {\prime}) + (1 - \alpha) C ^ {\mathrm{A}} (X ^ {\prime \prime}),
$$

$$
P ^ {\mathrm{A}} (\alpha X ^ {\prime} + (1 - \alpha) X ^ {\prime \prime}) \leq \alpha P ^ {\mathrm{E}} (X ^ {\prime}) + (1 - \alpha) P ^ {\mathrm{A}} (X ^ {\prime \prime}).
$$

## Proof

For brevity, we put $X = \alpha X ^ { \prime } + ( 1 - \alpha ) X ^ { \prime \prime }$ . Suppose that 

$$
C ^ {\mathrm{A}} (X) > \alpha C ^ {\mathrm{A}} (X ^ {\prime}) + (1 - \alpha) C ^ {\mathrm{A}} (X ^ {\prime \prime}).
$$

We write an option with strike price X and buy α options with strike price $X ^ { \prime }$ and $( 1 - \alpha )$ options with strike price $X ^ { \prime \prime }$ , investing without risk the positive balance of these transactions. If the written option is exercised at time $t \leq T$ , then we exercise both options held. In this way we shall achieve arbitrage because 

$$
(S (t) - X) ^ {+} \leq \alpha \left(S (t) - X ^ {\prime}\right) ^ {+} + (1 - \alpha) \left(S (t) - X ^ {\prime \prime}\right) ^ {+}.
$$

The proof for put options is similar. 

Dependence on the Underlying Asset Price. Once again, we shall consider options on a portfolio of x shares. The prices of American calls and puts on such a portfolio will be denoted by $C ^ { \mathrm { { A } } } ( S )$ and $P ^ { \mathrm { { A } } } ( S )$ , where $S = x S ( 0 )$ is the value of the portfolio, all remaining variables being fixed. The payofs at time t are $( x S ( t ) - X ) ^ { + }$ for calls and $\left( X - x S ( t ) \right) ^ { + }$ for puts. 

Proposition 7.15 

If $S ^ { \prime } < S ^ { \prime \prime }$ , then 

$$
C ^ {\mathrm{A}} (S ^ {\prime}) <   C ^ {\mathrm{A}} (S ^ {\prime \prime}),
$$

$$
P ^ {\mathrm{A}} (S ^ {\prime}) > P ^ {\mathrm{A}} (S ^ {\prime \prime}).
$$

## Proof

Suppose that $C ^ { \mathrm { A } } ( S ^ { \prime } ) \ge C ^ { \mathrm { A } } ( S ^ { \prime \prime } )$ for some $S ^ { \prime } < S ^ { \prime \prime }$ , where $S ^ { \prime } = x ^ { \prime } S ( 0 )$ and $S ^ { \prime \prime } = x ^ { \prime \prime } S ( 0 )$ . We can write and sell a call on a portfolio with $x ^ { \prime }$ shares and buy a call on a portfolio with price $x ^ { \prime \prime }$ shares, both options having the same strike price X and expiry time $T .$ . The balance $C ^ { \mathrm { A } } ( S ^ { \prime } ) - C ^ { \mathrm { A } } ( S ^ { \prime \prime } )$ of these transactions can be invested without risk. If the written option is exercised at time $t \leq T$ , then we can meet the liability by exercising the other option immediately. Because $x ^ { \prime } < x ^ { \prime \prime }$ , the payofs satisfy $( x ^ { \prime } S ( t ) - X ) ^ { + } \ \leq \ ( x ^ { \prime \prime } S ( t ) - X ) ^ { + }$ with strict inequality whenever $X < x ^ { \prime \prime } S ( t )$ . As a result, this strategy will provide an arbitrage opportunity. 

The proof is similar for put options. 

Proposition 7.16 

Suppose that $S ^ { \prime } < S ^ { \prime \prime }$ . Then 

$$
C ^ {\mathrm{A}} (S ^ {\prime \prime}) - C ^ {\mathrm{A}} (S ^ {\prime}) <   S ^ {\prime \prime} - S ^ {\prime},
$$

$$
P ^ {\mathrm{A}} (S ^ {\prime}) - P ^ {\mathrm{A}} (S ^ {\prime \prime}) <   S ^ {\prime \prime} - S ^ {\prime}.
$$

Proof 

By the inequalities in Theorem 7.2 

$$
C ^ {\mathrm{A}} (S ^ {\prime}) - P ^ {\mathrm{A}} (S ^ {\prime}) \geq S ^ {\prime} - X,
$$

$$
C ^ {\mathrm{A}} (S ^ {\prime \prime}) - P ^ {\mathrm{A}} (S ^ {\prime \prime}) \leq S ^ {\prime \prime} - X \mathrm{e} ^ {- r T}.
$$

On subtracting, we obtain 

$$
\begin{array}{c} \big (C ^ {\mathrm{A}} (S ^ {\prime \prime}) - C ^ {\mathrm{A}} (S ^ {\prime}) \big) + \big (P ^ {\mathrm{A}} (S ^ {\prime}) - P ^ {\mathrm{A}} (S ^ {\prime \prime}) \big) \leq S ^ {\prime \prime} - S ^ {\prime} + X (1 - \mathrm{e} ^ {- r T}) \\ \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \\ \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qend{array}
$$

Each of the two terms on the left-hand side is positive, so it must be strictly less than $S ^ { \prime \prime } - S ^ { \prime }$ , which completes the proof. □ 

## Proposition 7.17

Let $S ^ { \prime } < S ^ { \prime \prime }$ and let $\alpha \in ( 0 , 1 )$ . Then 

$$
\begin{array}{l} C ^ {\mathrm{A}} (\alpha S ^ {\prime} + (1 - \alpha) S ^ {\prime \prime}) \leq \alpha C ^ {\mathrm{A}} (S ^ {\prime}) + (1 - \alpha) C ^ {\mathrm{A}} (S ^ {\prime \prime}), \\ P ^ {\mathrm{A}} (\alpha S ^ {\prime} + (1 - \alpha) S ^ {\prime \prime}) \leq \alpha P ^ {\mathrm{A}} (S ^ {\prime}) + (1 - \alpha) P ^ {\mathrm{A}} (S ^ {\prime \prime}). \end{array}
$$

Proof 

Let $S = \alpha S ^ { \prime } + ( 1 - \alpha ) S ^ { \prime \prime }$ and let $S ^ { \prime } = x ^ { \prime } S ( 0 ) , S ^ { \prime \prime } = x ^ { \prime \prime } S ( 0 )$ and $S = x S ( 0 )$ Suppose that 

$$
C ^ {\mathrm{A}} (S) > \alpha C ^ {\mathrm{A}} (S ^ {\prime}) + (1 - \alpha) C ^ {\mathrm{A}} (S ^ {\prime \prime}).
$$

We can write and sell a call on a portfolio with x shares, and purchase α calls on a portfolio with $x ^ { \prime }$ shares and $1 - \alpha$ calls on a portfolio with $x ^ { \prime \prime }$ shares, all three options sharing the same strike price X and expiry time T. The positive balance $C ^ { \mathrm { { A } } } ( S ) - \alpha C ^ { \mathrm { { A } } } ( S ^ { \prime } ) - ( 1 - \alpha ) C ^ { \mathrm { { A } } } ( S ^ { \prime \prime } )$ of these transactions can be invested without risk. If the written option is exercised at time $t \leq T$ , then we shall have to pay $( x S ( t ) - X ) ^ { + }$ , where $x = \alpha x ^ { \prime } + \left( 1 - \alpha \right) x ^ { \prime \prime }$ . We can exercise the other two options to cover the liability. This is an arbitrage strategy because 

$$
(x S (t) - X) ^ {+} \leq \alpha (x ^ {\prime} S (t) - X) ^ {+} + (1 - \alpha) (x ^ {\prime \prime} S (t) - X) ^ {+}.
$$

The proof for put options is similar. 

Dependence on the Expiry Time. For American options we can also formulate a general result on the dependence of their prices on the expiry time $T .$ To emphasise this dependence, we shall now write $C ^ { \mathrm { A } } ( T )$ and $P ^ { \mathrm { R } } ( T )$ for the prices of American calls and puts, assuming that all other variables are fixed. 

Proposition 7.18 

If $T ^ { \prime } < T ^ { \prime \prime }$ , then 

$$
C ^ {\mathrm{A}} (T ^ {\prime}) \leq C ^ {\mathrm{A}} (T ^ {\prime \prime}),
$$

$$
P ^ {\mathrm{A}} (T ^ {\prime}) \leq P ^ {\mathrm{A}} (T ^ {\prime \prime}).
$$

## Proof

Suppose that $C ^ { \mathrm { A } } ( T ^ { \prime } ) > C ^ { \mathrm { A } } ( T ^ { \prime \prime } )$ . We write and sell one option expiring at time $T ^ { \prime }$ and buy one with the same strike price but expiring at time $T ^ { \prime \prime }$ , investing the balance without risk. If the written option is exercised at time $t \leq T ^ { \prime }$ , we can exercise the other option immediately to cover our liability. The posi tive balance $C ^ { \mathrm { A } } ( T ^ { \prime } ) - C ^ { \mathrm { A } } ( T ^ { \prime \prime } ) > 0$ invested without risk will be our arbitrage profit. 

The argument is the same for puts. 

## 7.5 Time Value of Options

The following convenient terminology is often used. We say that at time t a call option with strike price X is 

in the money if $S ( t ) > X$ • 

at the money if $S ( t ) = X$ 

out of the money if $S ( t ) < X$ 

Similarly, for a put option we say that it is 

in the money if $S ( t ) < X$ 

at the money if $S ( t ) = X$ 

out of the money $\operatorname { i f } S ( t ) > X$ 

Also convenient, though less precise, are the terms deep in the money and deep out of the money, which mean that the diference between the two sides in the respective inequalities is considerable. 

An American option in the money will bring a positive payof if exercised immediately, whereas an option out of the money will not. We use the same terms for European options, though their meaning is diferent: Even if the option is currently in the money, it may no longer be so on the exercise date, when the payof may well turn out to be zero. A European option in the money is no more than a promising asset. 

## Definition 7.1

At time $t \leq T$ the intrinsic value of a call option with strike price X is equal to $( S ( t ) - X ) ^ { + }$ . The intrinsic value of a put option with the same strike price is $\left( X - S ( t ) \right) ^ { + }$ 

We can see that the intrinsic value is zero for options out of the money or at the money. Options in the money have positive intrinsic value. The price of an option at expiry T coincides with the intrinsic value. The price of an American option prior to expiry may be greater than the intrinsic value because of the possibility of future gains. The price of a European option prior to the exercise time may be greater or smaller than the intrinsic value. 

## Definition 7.2

The time value of an option is the diference between the price of the option and its intrinsic value, that is, 

$$
C ^ {\mathrm{E}} (t) - (S (t) - X) ^ {+} \quad \text { for   a   European   call, }
$$

$$
P ^ {\mathrm{E}} (t) - (X - S (t)) ^ {+} \quad \mathrm{foraEuropeanput},
$$

$$
C ^ {\mathrm{A}} (t) - (S (t) - X) ^ {+} \quad \text { for   an   American   call, }
$$

P <sup>A</sup>(t)  (X  S(t))<sup>+</sup> for an American put. 

## Example 7.3


Let us examine some typical data. Suppose that the current price of stock is $125.23 per share. Consider the following:


<table><tr><td rowspan="2">Srike Price</td><td colspan="2">Intrinsic Value</td><td colspan="2">Time Value</td><td colspan="2">Option Price</td></tr><tr><td>Call</td><td>Put</td><td>Call</td><td>Put</td><td>Call</td><td>Put</td></tr><tr><td>110</td><td>15.23</td><td>0.00</td><td>3.17</td><td>2.84</td><td>18.40</td><td>2.84</td></tr><tr><td>120</td><td>5.23</td><td>0.00</td><td>7.04</td><td>6.46</td><td>12.27</td><td>6.46</td></tr><tr><td>130</td><td>0.00</td><td>5.23</td><td>6.78</td><td>4.41</td><td>6.78</td><td>9.64</td></tr></table>

An American call option with strike price $110 is in the money and has $15.23 intrinsic value. The option price must be at least equal to the intrinsic value, since the option may be exercised immediately. Typically, the price will be higher than the intrinsic value because of the possibility of future gains. On the other hand, a put option with strike price $110 will be out of the money and its intrinsic value will be zero. The positive price of the put is entirely due to the possibility of future gains. Similar relationships for other strike prices can be seen in the table. 

The time value of a European call as a function of S is shown in Figure 7.8. It can never be negative, and for large values of S it exceeds the diference $X - X \mathrm { e } ^ { - r T }$ . This is because of the inequality $C ^ { \mathrm { E } } ( S ) \geq S - X \mathrm { e } ^ { - r T }$ , see Proposition 7.3. 

The market value of a European put may be lower than its intrinsic value, that is, the time value may be negative, see Figure 7.9. This may be so only if the put option is in the money, $S < X$ , and it should be deep in the money. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/3ffe9dd8556a4eaab622fd4c153c371d10cf1aab8289fa866eadd2389dbd6f76.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/d6acf2a11dd6204eba85203a1b82ad5ce7f28529c6d2fcb31d3da55d98d8726b.jpg)



Figure 7.8 Time value $C ^ { \mathrm { E } } ( S ) - ( S - X ) ^ { + }$ of a European call option


For a European option we have to wait until the exercise time $T$ to realise the payof. The risk that the stock price will rise above X in the meantime may be considerable, which reduces the value of the option. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/1ebf762829d2f6fe789a3225614e6042f7b09fb39caf5e83d005a4fce21b6cbf.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/369a65d09834e7440c5f716dbbbc82b87e4ea12b8c71c23d146e6b8edb3ae8cd.jpg)



Figure 7.9 Time value $P ^ { \operatorname { E } } ( S ) - ( X - S ) ^ { + }$ of a European put option


The time value of an American call option is the same as that of a European call (if there are no dividends) and Figure 7.8 applies. For an American put a typical graph of the time value is shown in Figure 7.10. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/fbd442b1eb36e68e6a411990417f9694b1ae0c26e6a8552d5c5bed98c3e773a9.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/cfc4db39235b1de8c6103bf80b84a8a8ada96c471e9e863dca59519f04e55f7b.jpg)



Figure 7.10 Time value $C ^ { \mathrm { A } } ( S ) - ( S - X ) ^ { + }$ of an American put option


Figures 7.8, 7.9 and 7.10 also illustrate the following assertion. 

## Proposition 7.19

For any European or American call or put option with strike price X, the time value attains its maximum at $S = X$ 

## Proof

We shall present an argument for European calls. For $S \ \leq \ X$ the intrinsic value of the option is zero. Since $C ^ { \mathrm { E } } ( S )$ is an increasing function of S by Proposition 7.9, this means that the time value is an increasing function of S for $S \leq X$ . On the other hand, $C ^ { \mathrm { E } } ( S ^ { \prime \prime } ) - C ^ { \mathrm { E } } ( S ^ { \prime } ) \le S ^ { \prime \prime } - S ^ { \prime }$ for any $S ^ { \prime } < S ^ { \prime \prime }$ by Proposition 7.10. It follows that $C ^ { \mathrm { E } } ( S ^ { \prime \prime } ) - ( S ^ { \prime \prime } - X ) ^ { + } \le C ^ { \mathrm { E } } ( S ^ { \prime } ) - ( S ^ { \prime } - X ) ^ { + }$ if $X \le S ^ { \prime } < S ^ { \prime \prime }$ , which means that the time value is a decreasing function of S for $S \geq X$ . As a result, the time value has a maximum at $S = X$ 

The proof for other options is similar. 

Exercise 7.18 

Prove Proposition 7.19 for put options. 

# 8 Option Pricing

By a European derivative security or contingent claim with stock S as the underlying asset we mean a random variable of the form $D ( T ) = f ( S ( T ) )$ , where f is a given function, called the $p a y o f f$ . This is a direct generalisation of a call option with $f ( S ) = ( S - X ) ^ { + }$ , a put option with $f ( S ) = ( X - S ) ^ { + }$ , or a forward contract with $f ( S ) = S - X$ (for the long position). 

We have already learnt the basic method of pricing options in the one-step model (see Section 1.6) based on replicating the option payof. Not surprisingly, this idea extends to a general binomial tree model constructed out of such onestep two-state building blocks. Developing this extension will be our primary task in this chapter. 

## Theorem 8.1

Suppose that for any contingent claim $D ( T )$ there exists a replication strategy, that is, an admissible strategy $x ( t ) , y ( t )$ with final value $V ( T ) = D ( T )$ . Then the price $D ( 0 )$ of the contingent claim at time 0 must be equal to that of the replicating strategy, $V ( 0 ) = D ( 0 )$ 

## Proof

The proof is just a modification of that of Proposition 1.3. If $D ( 0 ) > V ( 0 )$ , then we write the derivative security and take a long position in the strategy. Our obligation will be covered by the strategy, the diference $D ( 0 ) - V ( 0 )$ being our arbitrage profit. If $D ( 0 ) < V ( 0 )$ , then we take the opposite positions, with $V ( 0 ) - D ( 0 )$ the resulting arbitrage profit. □ 

Replication also solves the problem of hedging the position of the option writer. If the cash received for the option is invested in the replicating strategy, then all the risk involved in writing the option will be eliminated. 

In this chapter we shall gradually develop such pricing methods for options, starting with a comprehensive analysis of the one-step binomial model, which will then be extended to a multi-step model. Finally, the Black–Scholes formula in continuous time will be introduced. 

## 8.1 European Options in the Binomial Tree Model

## 8.1.1 One Step

This simple case was discussed in Chapter 1. Here we shall reiterate the ideas in a more general setting: We shall be pricing general derivative securities and not just call or put options. This will enable us to extend the approach to the multi-step model. 

We assume that the random stock price $S ( 1 )$ at time 1 may take two values denoted by 

$$
\left\{ \begin{array}{l} S ^ {\mathrm{u}} = S (0) (1 + u), \\ S ^ {\mathrm{d}} = S (0) (1 + d), \end{array} \right.
$$

with probabilities $p$ and $1 - p .$ , respectively. To replicate a general derivative security with payof f we need to solve the system of equations 

$$
\left\{ \begin{array}{l l} x (1) S ^ {\mathrm{u}} + y (1) (1 + r) = f (S ^ {\mathrm{u}}), \\ x (1) S ^ {\mathrm{d}} + y (1) (1 + r) = f (S ^ {\mathrm{d}}), \end{array} \right.
$$

for $x ( 1 )$ and $y ( 1 )$ . This gives 

$$
x (1) = \frac {f (S ^ {\mathrm{u}}) - f (S ^ {\mathrm{d}})}{S ^ {\mathrm{u}} - S ^ {\mathrm{d}}},
$$

which is the replicating position in stock, called the delta of the option. We also find the money market position 

$$
y (1) = - \frac {(1 + d) f (S ^ {\mathrm{u}}) - (1 + u) f (S ^ {\mathrm{d}})}{(u - d) (1 + r)}.
$$

The initial value of the replicating portfolio is $x ( 1 ) S ( 0 ) + y ( 1 )$ . By Theorem 8.1 

$$
\begin{array}{l} D (0) = x (1) S (0) + y (1) \\ \qquad = \frac {f (S ^ {\mathrm{u}}) - f (S ^ {\mathrm{d}})}{u - d} - \frac {(1 + d) f (S ^ {\mathrm{u}}) - (1 + u) f (S ^ {\mathrm{d}})}{(u - d) (1 + r)}. \end{array}\tag{8.1}
$$

## Exercise 8.1

Show that the price of a call option grows with $u ,$ the other variables being kept constant. Analyse the impact of a change of d on the option price. 

## Exercise 8.2

Find a formula for the price $C ^ { \mathrm { E } } ( 0 )$ of a call option if $r = 0$ and $S ( 0 ) =$ $X = 1$ dollar. Compute the price for $u = 0 . 0 5$ and $d = - 0 . 0 5$ , and also for $u = 0 . 0 1$ and $d = - 0 . 1 9$ . Draw a conclusion about the relationship between the variance of the return on stock and that on the option. 

Recall the notion of the risk-neutral probability, given by 

$$
p _ {*} = \frac {r - d}{u - d},\tag{8.2}
$$

which turns the discounted stock price process $( 1 + r ) ^ { - n } S ( n )$ into a martingale, see Chapter 3. 

## Theorem 8.2

The expectation of the discounted payof computed with respect to the risk neutral probability is equal to the present value of the contingent claim, 

$$
D (0) = E _ {*} \big ((1 + r) ^ {- 1} f (S (1)) \big).\tag{8.3}
$$

## Proof

This is an immediate consequence of (8.1): 

$$
\begin{array}{l} D (0) = \frac {f (S ^ {\mathrm{u}}) - f (S ^ {\mathrm{d}})}{u - d} + \frac {(1 + u) f (S ^ {\mathrm{d}}) - (1 + d) f (S ^ {\mathrm{u}})}{(u - d) (1 + r)} \\ \qquad = \frac {1}{1 + r} \left(\frac {(r - d) f (S ^ {\mathrm{u}})}{(u - d)} + \frac {(u - r) f (S ^ {\mathrm{d}})}{u - d}\right) \\ \qquad = \frac {1}{1 + r} \left(p _ {*} f (S ^ {\mathrm{u}}) + (1 - p _ {*}) f (S ^ {\mathrm{d}})\right) \\ \qquad = E _ {*} \big ((1 + r) ^ {- 1} f (S (1)) \big), \end{array}
$$

as claimed. 

## Exercise 8.3

Find the initial value of the portfolio replicating a call option if proportional transaction costs are incurred whenever the underlying stock is sold. (No transaction costs apply when the stock is bought.) Compare this value with the case free of such costs. Assume that $S ( 0 ) = X = 1 0 0$ dollars, u = 0.1, d = 0.1 and $r = 0 . 0 5$ , admitting transaction costs at $c = 2 \%$ (the seller receiving 98% of the stock value). 

## Exercise 8.4

Let $S ( 0 ) = 7 5 $ dollars and let $u = 0 . 2$ and $d = - 0 . 1$ . Suppose that you can borrow money at 12%, but the rate for deposits is lower at 8%. Find the values of the replicating portfolios for a put and a call. Is the answer consistent with the put and call prices following from Theorem 8.2? 

## 8.1.2 Two Steps

We begin with two time steps. The stock price $S ( 2 )$ has three possible values 

$$
S ^ {\mathrm{uu}} = S (0) (1 + u) ^ {2}, \quad S ^ {\mathrm{ud}} = S (0) (1 + u) (1 + d), \quad S ^ {\mathrm{dd}} = S (0) (1 + d) ^ {2},
$$

and $S ( 1 )$ has two values 

$$
S ^ {\mathrm{u}} = S (0) (1 + u), \quad S ^ {\mathrm{d}} = S (0) (1 + d),
$$

at the nodes of the tree in Figure 8.1 marked by the corresponding sequences of letters u and d. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/dc415aed6bece76cdee5a1b6402a70a760574f8c07161625f4a21dbd9ca8305d.jpg)



Figure 8.1 Branchings in the two-step binomial tree


For each of the three subtrees in Figure 8.1 we can use the one-step repli cation procedure as described above. At time 2 the derivative security is represented by its payof, 

$$
D (2) = f (S (2)),
$$

which has three possible values. The derivative security price $D ( 1 )$ has two values 

$$
\frac {1}{1 + r} \left[ p _ {*} f (S ^ {\mathrm{uu}}) + (1 - p _ {*}) f (S ^ {\mathrm{ud}}) \right], \quad \frac {1}{1 + r} \left[ p _ {*} f (S ^ {\mathrm{du}}) + (1 - p _ {*}) f (S ^ {\mathrm{dd}}) \right],
$$

found by the one-step procedure applied to the two subtrees at nodes u and d. This gives 

$$
\begin{array}{l} D (1) = \frac {1}{1 + r} \big [ p _ {*} f (S (1) (1 + u)) + (1 - p _ {*})   f (S (1) (1 + d)) \big ] \\ = g (S (1)), \end{array}
$$

where 

$$
g (x) = \frac {1}{1 + r} \big [ p _ {*} f (x (1 + u)) + (1 - p _ {*}) f (x (1 + d)) \big ].
$$

As a result, D(1) can be regarded as a derivative security expiring at time 1 with payof g. (Though it cannot be exercised at time 1, the derivative security can be sold for $D ( 1 ) = g ( S ( 1 ) ) . )$ This means that the one-step procedure can be applied once again to the single subtree at the root of the tree. We have, therefore, 

$$
D (0) = \frac {1}{1 + r} \big [ p _ {*} g (S (0) (1 + u)) + (1 - p _ {*}) g (S (0) (1 + d)) \big ].
$$

It follows that 

$$
\begin{array}{l} D (0) = \frac {1}{1 + r} \big [ p _ {*} g (S ^ {\mathrm{u}}) + (1 - p _ {*})   g (S ^ {\mathrm{d}}) \big ] \\ = \frac {1}{(1 + r) ^ {2}} \big [ p _ {*} ^ {2} f (S ^ {\mathrm{uu}}) + 2 p _ {*}   (1 - p _ {*})   f (S ^ {\mathrm{ud}}) + (1 - p _ {*}) ^ {2}   f (S ^ {\mathrm{dd}}) \big ]. \end{array}
$$

The last expression in square brackets is the risk-neutral expectation of $f ( S ( 2 ) )$ ). This proves the following result. 

## Theorem 8.3

The expectation of the discounted payof computed with respect to the risk neutral probability is equal to the present value of the derivative security, 

$$
D (0) = E _ {*} \big ((1 + r) ^ {- 2} f (S (2)) \big).
$$

## Exercise 8.5

Let $S ( 0 ) = 1 2 0$ dollars, u = 0.2, $d = - 0 . 1$ and $r = 0 . 1$ . Consider a call option with strike price $X = 1 2 0$ dollars and exercise time $T = 2$ . Find the option price and the replicating strategy. 

## Exercise 8.6

Using the data in the previous exercise, find the price of a call and the replicating strategy if a 15 dollar dividend is paid at time 1. 

## 8.1.3 General N-Step Model

The extension of the results above to a multi-step model is straightforward. Beginning with the payof at the final step, we proceed backwards, solving the one-step problem repeatedly. Here is the procedure for the three-step model: 

$$
\begin{array}{l} D (3) = f (S (3)), \\ D (2) = \frac {1}{1 + r} \left[ p _ {*} f (S (2) (1 + u)) + (1 - p _ {*}) f (S (2) (1 + d)) \right] \\ \qquad = g (S (2)), \\ D (1) = \frac {1}{1 + r} \left[ p _ {*} g (S (1) (1 + u)) + (1 - p _ {*}) g (S (1) (1 + d)) \right] \\ \qquad = h (S (1)), \\ D (0) = \frac {1}{1 + r} \left[ p _ {*} h (S (0) (1 + u)) + (1 - p _ {*}) h (S (0) (1 + d)) \right], \end{array}
$$

where 

$$
g (x) = \frac {1}{1 + r} \left[ p _ {*} f (x (1 + u)) + (1 - p _ {*}) f (x (1 + d)) \right],
$$

$$
h (x) = \frac {1}{1 + r} \left[ p _ {*} g (x (1 + u)) + (1 - p _ {*}) g (x (1 + d)) \right].
$$

It follows that 

$$
\begin{array}{r l} & D (0) = \frac {1}{1 + r} \big [ p _ {*} h (S ^ {\mathrm{u}}) + (1 - p _ {*}) h (S ^ {\mathrm{d}})) \big ] \\ & \quad = \frac {1}{(1 + r) ^ {2}} \big [ p _ {*} ^ {2} g (S ^ {\mathrm{uu}}) + 2 p _ {*} (1 - p _ {*}) g (S ^ {\mathrm{ud}}) + (1 - p _ {*}) ^ {2} g (S ^ {\mathrm{dd}})) \big ] \\ & \quad = \frac {1}{(1 + r) ^ {3}} \big [ p _ {*} ^ {3} f (S ^ {\mathrm{uuu}}) + 3 p _ {*} ^ {2} (1 - p _ {*}) f (S ^ {\mathrm{uud}}) \\ & \qquad \qquad \qquad \qquad \qquad \qquad + 3 p _ {*} (1 - p _ {*}) ^ {2} f (S ^ {\mathrm{udd}}) + (1 - p _ {*}) ^ {3} f (S ^ {\mathrm{ddd}})) \big ]. \end{array}
$$

The emerging pattern is this: Each term in the square bracket is characterised by the number k of upward stock price movements. This number determines the power of $p _ { * }$ and the choice of the payof value. The power of $1 - p _ { * }$ is the number of downward price movements, equal to $3 - k$ in the last expression, and $N - k$ in general, where N is the number of steps. The coeficients in front of each term give the number of scenarios (paths through the tree) that lead to the corresponding payof, equal to $\begin{array} { r } { \binom { N } { k } = \frac { N ! } { k ! ( N - k ) ! } } \end{array}$ , the number of k-element combinations out of N elements. For example, there are three paths through the 3-step tree leading to the node udd. 

As a result, in the N-step model 

$$
D (0) = \frac {1}{(1 + r) ^ {N}} \sum_ {k = 0} ^ {N} \binom {N} {k} p _ {*} ^ {k} (1 - p _ {*}) ^ {N - k} f \Bigl (S (0) (1 + u) ^ {k} (1 + d) ^ {N - k} \Bigr).\tag{8.4}
$$

The expectation of $f ( S ( N ) )$ under the risk-neutral probability can readily be recognised in this formula. The result can be summarised as follows. 

## Theorem 8.4

The value of a European derivative security with payof $f ( S ( N ) )$ in the $N _ { - }$ step binomial model is the expectation of the discounted payof under the risk-neutral probability: 

$$
D (0) = E _ {*} \Big ((1 + r) ^ {- N} f (S (N)) \Big).
$$

## Remark 8.1

There is no need to know the actual probability $p$ to compute $D ( 0 )$ . This remarkable property of the option price is important in practice, as the value of $p$ may be dificult to estimate from market data. Instead, the formula fo $D ( 0 )$ features $p _ { * }$ , the risk-neutral probability, which may have nothing in common with $p ,$ but is easy to compute from (8.2). 

## 8.1.4 Cox–Ross–Rubinstein Formula

The payof for a call option with strike price X satisfie $f ( x ) = 0$ for $x \le X$ which reduces the number of terms in (8.4). The summation starts with the least m such that 

$$
S (0) (1 + u) ^ {m} (1 + d) ^ {N - m} > X.
$$

Hence 

$$
C ^ {\mathrm{E}} (0) = (1 + r) ^ {- N} \sum_ {k = m} ^ {N} \binom {N} {k} p _ {*} ^ {k} (1 - p _ {*}) ^ {N - k} \Bigl (S (0) (1 + u) ^ {k} (1 + d) ^ {N - k} - X \Bigr).
$$

This can be written as 

$$
C ^ {\mathrm{E}} (0) = x (1) S (0) + y (1),
$$

relating the option price to the initial replicating portfolio $x ( 1 ) , y ( 1 )$ , where 

$$
x (1) = (1 + r) ^ {- N} \sum_ {k = m} ^ {N} {\binom {N} {k}} p _ {*} ^ {k} (1 - p _ {*}) ^ {N - k} (1 + u) ^ {k} (1 + d) ^ {N - k},
$$

$$
y (1) = - X (1 + r) ^ {- N} \sum_ {k = m} ^ {N} {\binom {N} {k}} p _ {*} ^ {k} (1 - p _ {*}) ^ {N - k}.
$$

The expression for x(1) can be rewritten as 

$$
x (1) = \sum_ {k = m} ^ {N} \binom {N} {k} \left(p _ {*} \frac {1 + u}{1 + r}\right) ^ {k} \left((1 - p _ {*}) \frac {1 + d}{1 + r}\right) ^ {N - k} = \sum_ {k = m} ^ {N} \binom {N} {k} q ^ {k} (1 - q) ^ {N - k},
$$

where 

$$
q = p _ {*} \frac {1 + u}{1 + r}.
$$

(Note that $p _ { * } \frac { 1 + u } { 1 + r }$ and $( 1 - p _ { * } ) \frac { 1 + d } { 1 + r }$ add up to one.) Similar formulae can be derived for put options, either directly or using put-call parity. 

These important results are summarised in the following theorem, in which $\varPhi ( m , N , p )$ denotes the cumulative binomial distribution with N trials and probability p of success in each trial, 

$$
\Phi (m, N, p) = \sum_ {k = 0} ^ {m} \binom {N} {k} p ^ {k}   (1 - p) ^ {N - k}  .
$$

## Theorem 8.5 (Cox–Ross–Rubinstein Formula)

In the binomial model the price of a European call and put option with strike price X to be exercised after N time steps is given by 

$$
C ^ {\mathrm{E}} (0) = S (0) \left[ 1 - \varPhi (m - 1, N, q) \right] - (1 + r) ^ {- N} X \left[ 1 - \varPhi (m - 1, N, p _ {*}) \right],
$$

$$
P ^ {\mathrm{E}} (0) = - S (0) \varPhi (m - 1, N, q) + (1 + r) ^ {- N} X \varPhi (m - 1, N, p _ {*}).
$$

The initial replicating portfolio $x ( 1 ) , y ( 1 )$ is given by 

<table><tr><td></td><td>x(1)</td><td>y(1)</td></tr><tr><td>for a call</td><td>$ 1 - \Phi(m-1, N, q) $</td><td>$ -(1 + r)^{-N} X [1 - \Phi(m-1, N, p_*)] $</td></tr><tr><td>for a put</td><td>$ -\Phi(m-1, N, q) $</td><td>$ (1 + r)^{-N} X \Phi(m-1, N, p_*) $</td></tr></table>

## Exercise 8.7

Let $S ( 0 ) = 5 0 $ dollars, $r = 5 \% , u = 0 . 3$ and $d = - 0 . 1$ . Find the price of a European call and put with strike price $X = 6 0$ dollars to be exercised after $N = 3$ time steps. 

## Exercise 8.8

Let $S ( 0 ) = 5 0 $ dollars, $r = 0 . 5 \% , u = 0 . 0 1$ and $d = - 0 . 0 1$ . Find $m , x ( 1 )$ ， and the price $C ^ { \mathrm { E } } ( 0 )$ of a European call option with strike X = 60 dollars to be exercised after $N = 5 0$ time steps. 

## Exercise 8.9

Consider the scenario in which stock goes up at each step. At which step will the delta of a European call become 1? 

## 8.2 American Options in the Binomial Tree Model

Even the formulation of a precise mathematical definition of an American type contingent claim presents some dificulties. Nevertheless, the informal descrip tion is simple: The option can be exercised at any time step n such that $0 \leq n \leq N$ , with payof $f ( S ( n ) )$ . Of course, it can be exercised only once. The price of an American option at time n will be denoted by $D ^ { \mathrm { A } } ( n )$ 

To begin with, we shall analyse an American option expiring after 2 time steps. Unless the option has already been exercised, at expiry it will be worth 

$$
D ^ {\mathrm{A}} (2) = f (S (2)),
$$

where we have three values depending on the values of $S ( 2 )$ . At time 1 the option holder will have the choice to exercise immediately, with payof $f ( S ( 1 ) )$ , or to wait until time 2, when the value of the American option will become $f ( S ( 2 ) )$ The value of waiting can be computed by treating $f ( S ( 2 ) )$ ) as a one-step European contingent claim to be priced at time 1, which gives the value 

$$
\frac {1}{1 + r} \left[ p _ {*} f (S (1) (1 + u)) + (1 - p _ {*}) f (S (1) (1 + d)) \right]
$$

at time 1. In efect, the option holder has the choice between the latter value or the immediate payof $f ( S ( 1 ) )$ . The American option at time 1 will, therefore, be worth the higher of the two, 

$$
\begin{array}{l} D ^ {\mathrm{A}} (1) = \max \left\{f (S (1)), \frac {1}{1 + r} \left[ p _ {*} f (S (1) (1 + u)) + (1 - p _ {*}) f (S (1) (1 + d)) \right] \right\} \\ = f _ {1} (S (1)) \end{array}
$$

(a random variable with two values), where 

$$
f _ {1} (x) = \max \Big \{f (x), \frac {1}{1 + r} \left[ p _ {*} f (x (1 + u)) + (1 - p _ {*}) f (x (1 + d)) \right] \Big \}.
$$

A similar argument gives the American option value at time 0, 

$$
D ^ {\mathrm{A}} (0) = \max \Big \{f (S (0)), \frac {1}{1 + r} \left[ p _ {*} f _ {1} (S (0) (1 + u)) + (1 - p _ {*}) f _ {1} (S (0) (1 + d)) \right] \Big \}.
$$

## Example 8.1

To illustrate the above procedure we consider an American put option with strike price $X = 8 0$ dollars expiring at time 2 on a stock with initial price $S ( 0 ) = 8 0 $ dollars in a binomial model with $u = 0 . 1 , d = - 0 . 0 5$ and $r = 0 . 0 5$ (We consider a put, as we know that there is no diference between American and European call options, see Theorem 7.4.) The stock values are 

<table><tr><td>n</td><td colspan="2">0</td><td colspan="2">1</td><td>2</td></tr><tr><td rowspan="3">S(n)</td><td rowspan="3">80.00</td><td rowspan="3">&lt;</td><td>88.00</td><td>&lt;</td><td>96.80</td></tr><tr><td>76.00</td><td>&lt;</td><td>83.60</td></tr><tr><td></td><td></td><td>72.20</td></tr></table>

The price of the American put will be denoted by $P ^ { \mathrm { A } } ( n )$ for $n = 0 , 1 , 2$ . At expiry the payof will be positive only in the scenario with two downward stock price movements, 

<table><tr><td>n</td><td colspan="2">0</td><td colspan="2">1</td><td>2</td></tr><tr><td rowspan="3"><eq>P^{\mathrm {A}}(n)</eq></td><td rowspan="3">?</td><td rowspan="3">&lt;</td><td>?</td><td>&lt;</td><td>0.00</td></tr><tr><td>?</td><td>&lt;</td><td>0.00</td></tr><tr><td>?</td><td>&lt;</td><td>7.80</td></tr></table>

At time 1 the option writer can choose between exercising the option immedi ately or waiting until time 2. In the up state at time 1 the immediate payof and the value of waiting are both zero. In the down state the immediate payof is 4 dollars, while the value of waiting is $1 . 0 5 ^ { - 1 } \times \frac { 1 } { 3 } \times 7 . 8 \cong 2 . 4 8$ dollars. The option holder will choose the higher value (exercising the option in the down state at time 1). This gives the time 1 values of the American put, 

<table><tr><td>n</td><td colspan="2">0</td><td colspan="2">1</td><td>2</td></tr><tr><td rowspan="2"><eq>P^{\mathrm {A}}(n)</eq></td><td rowspan="2">?</td><td rowspan="2">&lt;</td><td>0.00</td><td>&lt;</td><td>0.00</td></tr><tr><td>4.00</td><td>&lt;</td><td>7.80</td></tr></table>

At time 0 the choice is, once again, between the payof, which is zero, or the value of waiting, which is $1 . 0 5 ^ { - 1 } \times \frac { 1 } { 3 } \times 4 \cong 1 . 2 7$ dollars. Taking the higher of the two completes the tree of option prices, 

$$
\begin{array}{c c c c c} n & 0 & 1 & 2 \\ \hline & & & 0. 0 0 \\ P ^ {\mathrm{A}} (n) & 1. 2 7 & <   & 0. 0 0 & <   \\ & & 4. 0 0 & <   \\ & & & 7. 8 0 \end{array}
$$

For comparison, the price of a European put is $P ^ { \mathrm { E } } ( 0 ) = 1 . 0 5 ^ { - 1 } \times \frac { 1 } { 3 } \times 2 . 4 8 \cong 0 . 7 9$ dollars, clearly less than the American put price $P ^ { \mathrm { A } } ( 0 ) \cong 1 . 2 7$ dollars. 

This can be generalised, leading to the following definition. 

## Definition 8.1

An American derivative security or contingent claim with payof function f expiring at time N is a sequence of random variables defined by backward 

induction: 

$$
\begin{array}{l} D ^ {\mathrm{A}} (N) = f (S (N)), \\ D ^ {\mathrm{A}} (N - 1) = \max \Big \{f (S (N - 1)), \frac {1}{1 + r} [ p _ {*} f (S (N - 1) (1 + u)) \\ \qquad + (1 - p _ {*}) f (S (N - 1) (1 + d)) ] \Big \} =: f _ {N - 1} (S (N - 1)), \\ D ^ {\mathrm{A}} (N - 2) = \max \Big \{f (S (N - 2)), \frac {1}{1 + r} [ p _ {*} f _ {N - 1} (S (N - 2) (1 + u)) \\ \qquad + (1 - p _ {*}) f _ {N - 1} (S (N - 2) (1 + d)) ] \Big \} =: f _ {N - 2} (S (N - 2)), \\ \vdots \\ D ^ {\mathrm{A}} (1) = \max \Big \{f (S (2)), \frac {1}{1 + r} [ p _ {*} f _ {2} (S (1) (1 + u)) \\ \qquad + (1 - p _ {*}) f _ {2} (S (1) (1 + d)) ] \Big \} =: f _ {1} (S (1)), \\ D ^ {\mathrm{A}} (0) = \max \Big \{f (S (0)), \frac {1}{1 + r} [ p _ {*} f _ {1} (S (0) (1 + u)) \\ \qquad + (1 - p _ {*}) f _ {1} (S (0) (1 + d)) ] \Big \}. \end{array}
$$

## Exercise 8.10

Compute the value of an American put expiring at time 3 with strike price X = 62 dollars on a stock with initial price S(0) = 60 dollars in a binomial model with $u = 0 . 1 , d = - 0 . 0 5$ and $r = 0 . 0 3$ 

## Exercise 8.11

Compare the prices of an American call and a European call with strike price X = 120 dollars expiring at time 2 on a stock with initial price S(0) = 120 dollars in a binomial model with $u = 0 . 2 , d = - 0 . 1$ and $r = 0 . 1$ 

## Example 8.2

The last exercise can be modified to show that the equality of European and American call prices may not hold if a dividend is paid. Suppose that a dividend of 14 dollars is paid at time 2. Otherwise, we shall use the same data as in 


Exercise 8.11. The ex-dividend stock prices are


<table><tr><td>n</td><td colspan="2">0</td><td colspan="2">1</td><td>2</td></tr><tr><td></td><td></td><td></td><td></td><td></td><td>158.80</td></tr><tr><td>S(n)</td><td>120.00</td><td>&lt;</td><td>144.00</td><td>&lt;</td><td></td></tr><tr><td>ex-div</td><td></td><td></td><td>108.00</td><td>&lt;</td><td>115.60</td></tr><tr><td></td><td></td><td></td><td></td><td></td><td>83.20</td></tr></table>


The corresponding European and American call values will be


<table><tr><td>n</td><td>0</td><td>1</td><td>2</td></tr><tr><td></td><td></td><td></td><td>38.80</td></tr><tr><td></td><td></td><td></td><td>38.80</td></tr><tr><td></td><td></td><td>23.52</td><td rowspan="2">&lt;</td></tr><tr><td></td><td></td><td>24.00</td></tr><tr><td><eq>C^E(n)</eq></td><td>14.25</td><td rowspan="2">&lt;</td><td>0.00</td></tr><tr><td><eq>C^A(n)</eq></td><td>14.55</td><td>0.00</td></tr><tr><td></td><td></td><td>0.00</td><td rowspan="2">&lt;</td></tr><tr><td></td><td></td><td>0.00</td></tr><tr><td></td><td></td><td></td><td>0.00</td></tr><tr><td></td><td></td><td></td><td>0.00</td></tr></table>

The American call should be exercised early in the up state at time 1 with payof 24 dollars (bold figures), which is more than the value of holding the option to expiry. As a result, the price of the American call is higher than that of the European call. 

## Exercise 8.12

Compute the prices of European and American puts with exercise and strike price X = 14 dollars expiring at time 2 on a stock with $S ( 0 ) = 1 2 $ dollars in a binomial model with $u = 0 . 1$ , $d = - 0 . 0 5$ and $r \ = \ 0 . 0 2$ , assuming that a dividend of 2 dollars is paid at time 1. 

## 8.3 Black–Scholes Formula

We shall present an outline of the main results for European call and put options in continuous time, culminating in the famous Black–Scholes formula. Our treatment of continuous time is a compromise lacking full mathematical rigour, which would require a systematic study of Stochastic Calculus, a topic treated in detail in more advanced texts. In place of this, we shall exploit an analogy with the discrete time case. 

As a starting point we take the continuous time model of stock prices developed in Chapter 3 as a limit of suitably scaled binomial models with time steps going to zero. In the resulting continuous time model the stock price is given by 

$$
S (t) = S (0) \mathrm{e} ^ {m t + \sigma W (t)},\tag{8.5}
$$

where $W ( t )$ is the standard Wiener process (Brownian motion), see Sec tion 3.3.2. This means, in particular, that $S ( t )$ has the log normal distribution. 

Consider a European option on the stock expiring at time $T$ with payof $f ( S ( T ) )$ . As in the discrete-time case, see Theorem 8.4, the time 0 price $D ( 0 )$ of the option ought to be equal to the expectation of the discounted payof $ { \mathrm { e } } ^ { - r T } f ( S ( T ) )$ , 

$$
D (0) = E _ {*} \big (\mathrm{e} ^ {- r T} f (S (T)) \big),\tag{8.6}
$$

under a risk-neutral probability $P _ { * }$ that turns the discounted stock price process $\mathrm { e } ^ { - r t } S ( t )$ into a martingale. Here we shall accept this formula without proof, by analogy with the discrete time result. (The proof is based on an arbitrage argument combined with a bit of Stochastic Calculus, the latter beyond the scope of this book.) 

What is the risk-neutral probability $P _ { * }$ , then? A necessary condition is that the expectation of the discounted stock prices $\mathrm { e } ^ { - r t } S ( t )$ should be constant (independent of $t )$ , just like in the discrete time case, see (3.5). 

Let us compute this expectation using the real market probability P. Since $W ( t )$ is normally distributed with mean 0 and variance t, it has density $\textstyle { \frac { 1 } { \sqrt { 2 \pi t } } } \mathrm { e } ^ { - { \frac { x ^ { 2 } } { 2 t } } }$ under probability P. As a result, 

$$
\begin{array}{r l} & E \big (\mathrm{e} ^ {- r t} S (t) \big) = S (0) E \Big (\mathrm{e} ^ {\sigma W (t) + (m - r) t} \Big) \\ & \quad = S (0) \int_ {- \infty} ^ {\infty} \mathrm{e} ^ {\sigma x + (m - r) t} \frac {1}{\sqrt {2 \pi t}} \mathrm{e} ^ {- \frac {x ^ {2}}{2 t}} \mathrm{d} x \\ & \quad = S (0) \mathrm{e} ^ {(m - r + \frac {1}{2} \sigma^ {2}) t} \int_ {- \infty} ^ {\infty} \frac {1}{\sqrt {2 \pi t}} \mathrm{e} ^ {- \frac {(x - \sigma t) ^ {2}}{2 t}} \mathrm{d} x \\ & \quad = S (0) \mathrm{e} ^ {(m - r + \frac {1}{2} \sigma^ {2}) t} \int_ {- \infty} ^ {\infty} \frac {1}{\sqrt {2 \pi t}} \mathrm{e} ^ {- \frac {y ^ {2}}{2 t}} \mathrm{d} y \\ & \quad = S (0) \mathrm{e} ^ {(m - r + \frac {1}{2} \sigma^ {2}) t}. \end{array}
$$

If $m + { \textstyle { \frac { 1 } { 2 } } } \sigma ^ { 2 } \ne r$ , then the expectation $E ( \mathrm { e } ^ { - r t } S ( t ) ) = S ( 0 ) \mathrm { e } ^ { ( m - r + { \frac { 1 } { 2 } } \sigma ^ { 2 } ) t }$ clearly depends on t, so $S ( t )$ cannot be a martingale under P. 

However, the calculations above suggest a modification $P _ { * }$ of P that would make the corresponding expectation $E _ { * } ( \mathrm { e } ^ { - r t } S ( t ) )$ independent of t by eliminating the exponential factor $\mathrm { e } ^ { ( m - r + { \frac { 1 } { 2 } } \sigma ^ { 2 } ) t }$ . Namely, if $P$ can be replaced by a probability $P _ { * }$ such that $V ( t ) = W ( t ) + \left( m - r + { \textstyle { \frac { 1 } { 2 } } } \sigma ^ { 2 } \right) t / \sigma$ (rather than $W ( t )$ itself) becomes a Wiener process under $P _ { * }$ , then the exponential factor $\mathrm { e } ^ { ( m - r + \frac { 1 } { 2 } \sigma ^ { 2 } ) { \ ' } t }$ will be eliminated from the final expression. (The existence of such a probability $P _ { * }$ follows from an advanced result in Stochastic Calculus, the socalled Girsanov theorem.) Indeed, since $V ( t )$ has density $\textstyle { \frac { 1 } { \sqrt { 2 \pi t } } } \mathrm { e } ^ { - { \frac { x ^ { 2 } } { 2 t } } }$ under $P _ { * }$ that is, it is normally distributed with mean 0 and variance $t ,$ it follows that 

$$
\begin{array}{r l} & E _ {*} \big (\mathrm{e} ^ {- r t} S (t) \big) = S (0) E _ {*} \Big (\mathrm{e} ^ {\sigma W (t) + (m - r) t} \Big) \\ & \qquad = S (0) E _ {*} \Big (\mathrm{e} ^ {\sigma V (t) - \frac {1}{2} \sigma^ {2} t} \Big) \\ & \qquad = S (0) \int_ {- \infty} ^ {\infty} \mathrm{e} ^ {\sigma x - \frac {1}{2} \sigma^ {2} t} \frac {1}{\sqrt {2 \pi t}} \mathrm{e} ^ {- \frac {x ^ {2}}{2 t}} \mathrm{d} x \\ & \qquad = S (0) \int_ {- \infty} ^ {\infty} \frac {1}{\sqrt {2 \pi t}} \mathrm{e} ^ {- \frac {(x - \sigma t) ^ {2}}{2 t}} \mathrm{d} x \\ & \qquad = S (0) \int_ {- \infty} ^ {\infty} \frac {1}{\sqrt {2 \pi t}} \mathrm{e} ^ {- \frac {y ^ {2}}{2 t}} \mathrm{d} y = S (0). \end{array}
$$

The fact that $E _ { * } ( \mathrm { e } ^ { - r t } S ( t ) ) = S ( 0 )$ does not depend on time t is a necessary condition for the discounted price process $\mathrm { e } ^ { - r t } S ( t )$ to be a martingale under $P _ { * }$ To show that $\mathrm { e } ^ { - r t } S ( t )$ is indeed a martingale under $P _ { * }$ we need in fact to verify the stronger condition 

$$
E _ {*} \big (\mathrm{e} ^ {- r t} S (t) | S (u) \big) = \mathrm{e} ^ {- r u} S (u)\tag{8.7}
$$

for any $t \geq u \geq 0$ , involving the conditional expectation of $\mathrm { e } ^ { - r t } S ( t )$ given $S ( u )$ $\mathrm { S o }$ far we have dealt with conditional expectation where the condition was given in terms of a discrete random variable, see Section 3.2.2. Here, however, the condition is expressed in terms of $S ( u )$ , a random variable with continuou distribution. In this case the precise mathematical meaning of $\left( 8 . 7 \right)$ is that for every $a > 0$ 

$$
E _ {*} \big (\mathrm{e} ^ {- r t} S (t) 1 _ {S (u) <   a} \big) = E _ {*} \big (\mathrm{e} ^ {- r u} S (u) 1 _ {S (u) <   a} \big),\tag{8.8}
$$

where $1 _ { S ( u ) < a }$ is the indicator random variable, equal to 1 if $S ( u ) < a$ and to 0 if $S ( u ) \geq a$ 

Exercise 8.13 

Verify equality (8.8). 

Exercise 8.14 

Find the density of $W ( t )$ under the risk-neutral probability $P _ { * }$ 

Above we have identified the risk-neutral probability $P _ { * }$ . Now we shall con sider a European call option on the stock with strike price $X$ to be exercised at time $T$ . The general formula (8.6) for the price of an option becomes 

$$
C ^ {\mathrm{E}} (0) = E _ {*} \left(\mathrm{e} ^ {- r T} (S (T) - X) ^ {+}\right).
$$

Let us compute this expectation. Because $\begin{array} { r } { V ( T ) = W ( t ) + \left( m - r + { \frac { 1 } { 2 } } \sigma ^ { 2 } \right) \frac { t } { \sigma } } \end{array}$ for $t \geq 0$ is a Wiener process under $P _ { * }$ , the random variable $V ( T ) = W ( T ) +$ $\begin{array} { r } { \left( m - r + \frac { 1 } { 2 } \sigma ^ { 2 } \right) \frac { T } { \sigma } } \end{array}$ is normally distributed with mean 0 and variance $T ,$ , that is, it has density $\scriptstyle { \frac { 1 } { \sqrt { 2 \pi T } } } \mathrm { e } ^ { - { \frac { x ^ { 2 } } { 2 T } } }$ . As a result, 

$$
\begin{array}{l} C ^ {\mathrm{E}} (0) = E _ {*} \big (\mathrm{e} ^ {- r T} (S (T) - X) ^ {+} \big) \\ \qquad = E _ {*} \bigg (\Big (S (0) \mathrm{e} ^ {\sigma V (t) - \frac {1}{2} \sigma^ {2} T} - X \mathrm{e} ^ {- r T} \Big) ^ {+} \bigg) \\ \qquad = \int_ {- d _ {2} \sqrt {T}} ^ {\infty} \Big (S (0) \mathrm{e} ^ {\sigma x - \frac {1}{2} \sigma^ {2} T} - X \mathrm{e} ^ {- r T} \Big) \frac {1}{\sqrt {2 \pi T}} \mathrm{e} ^ {- \frac {x ^ {2}}{2 T}} \mathrm{d} x \\ \qquad = S (0) \int_ {- d _ {1}} ^ {\infty} \frac {1}{\sqrt {2 \pi}} \mathrm{e} ^ {- \frac {y ^ {2}}{2}} \mathrm{d} y - X \mathrm{e} ^ {- r T} \int_ {- d _ {2}} ^ {\infty} \frac {1}{\sqrt {2 \pi}} \mathrm{e} ^ {- \frac {y ^ {2}}{2}} \mathrm{d} y \\ \qquad = S (0) N (d _ {1}) - X \mathrm{e} ^ {- r T} N (d _ {2}), \end{array}
$$

where 

$$
d _ {1} = \frac {\ln \frac {S (0)}{X} + \left(r + \frac {1}{2} \sigma^ {2}\right) T}{\sigma \sqrt {T}}, \qquad d _ {2} = \frac {\ln \frac {S (0)}{X} + \left(r - \frac {1}{2} \sigma^ {2}\right) T}{\sigma \sqrt {T}},\tag{8.9}
$$

and where 

$$
N (x) = \int_ {- \infty} ^ {x} \frac {1}{\sqrt {2 \pi}} \mathrm{e} ^ {- \frac {y ^ {2}}{2}} \mathrm{d} y = \int_ {- x} ^ {\infty} \frac {1}{\sqrt {2 \pi}} \mathrm{e} ^ {- \frac {y ^ {2}}{2}} \mathrm{d} y\tag{8.10}
$$

is the normal distribution function. 

What we have just derived is the celebrated Black–Scholes formula for European call options. The choice of time 0 to compute the price of the option is arbitrary. In general, the option price can be computed at any time $t < T$ 2 in which case the time remaining before the option is exercised will be $T - t$ Substituting t for 0 and $T - t$ for $T$ in the above formulae, we thus obtain the following result. 

## Theorem 8.6 (Black–Scholes Formula)

The time t price of a European call with strike price X and exercise time $T _ { : }$ where $t < T$ , is given by 

$$
C ^ {\mathrm{E}} (t) = S (t) N (d _ {1}) - X \mathrm{e} ^ {- r (T - t)} N (d _ {2})
$$

with 

$$
d _ {1} = \frac {\ln \frac {S (0)}{X} + \left(r + \frac {1}{2} \sigma^ {2}\right) (T - t)}{\sigma \sqrt {T - t}}, d _ {2} = \frac {\ln \frac {S (0)}{X} + \left(r - \frac {1}{2} \sigma^ {2}\right) (T - t)}{\sigma \sqrt {T - t}}.\tag{8.11}
$$

Exercise 8.15 

Derive the Black–Scholes formula 

$$
P ^ {\mathrm{E}} (t) = X \mathrm{e} ^ {- r (T - t)} N (- d _ {2}) - S (t) N (- d _ {1}),
$$

with $d _ { 1 }$ and $d _ { 2 }$ given by (8.11), for the price of a European put with strike X and exercise time T. 

## Remark 8.2

Observe that the Black–Scholes formula contains no m. It is a property analogous to that in Remark 8.1, and of similar practical significance: There is no need to know m to work out the price of a European call or put option in continuous time. 

It is interesting to compare the Black–Scholes formula for the price of a European call with the Cox–Ross–Rubinstein formula. There is close analogy between the terms. Apart from the obvious correspondence between the con tinuous and discrete time discount factors $\mathrm { e } ^ { - r T }$ and $( 1 + r ) ^ { - N }$ , the binomial and normal distribution terms appearing in these formulae are also related to one another. The precise relationship comes from a version of the Central Limit Theorem: It can be shown that the option price given by the Cox–Ross– Rubinstein formula tends to that in the Black–Scholes formula in the continuou time limit described in Chapter 3. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/1e1be695-8dd8-452d-ae78-fcbdd5827aec/9bcf58b84020e44b65c8864679704c0f7d0b372252edb87dc987684fc9bba36c.jpg)



Figure 8.2 Option price $C ^ { \mathrm { E } }$ in continuous and discrete time models as a function of time T remaining before the option is exercised


<!-- === Source: MinerU_markdown_Mathematics_for_Finance_-_An_Introduction_to_Financial_Engineering-Capinski_201_2122706940055363597.md (Page 201) === -->

Rather than looking at the details of this limit, we just refer to Figure 8.2 for illustration. It shows the price $C ^ { \mathrm { E } }$ of a European call with strike $X = 1 0 0$ on a stock with $S ( 0 ) = 1 0 0 , \sigma = 0 . 3$ and $m = 0 . 2$ . (Though m is irrelevant for the Black–Scholes formula, it still features in the discrete time approximation.) The continuous compounding interest rate is taken to be $r = 0 . 2$ . The option price is computed in two ways, as a function of the time T remaining before the option is exercised: 

a) (solid line) from the Black–Scholes formula for T between 0 and 1; 

b) (dots) using the Cox–Ross–Rubinstein formula with $T$ increasing from 0 to 1 in $N = 1 0$ steps of duration $\tau = 0 . 1$ each; the discrete growth rates for each step are computed using formulae (3.7). 

Even with as few as 10 steps there is remarkably good agreement between the discrete and continuous time formulae. 

# Financial Engineering

This chapter shows some applications of derivative securities to managing the risk exposure in various situations. The presentation will be by means of examples and mini case studies. Even though these are concerned with very particular circumstances, the methods are applicable to a wide range of tasks handled by financial managers. 

First, we shall present methods for eliminating or reducing the risk involved in writing options. This is a problem faced by financial institutions who issue and sell derivative securities, but may not wish to bear the accompanying risk. Such institutions are typically satisfied by the commission charged for their services, without taking an active position in the market. 

Next, we shall analyse methods of reducing undesirable risk stemming from certain business activities. Our case studies will be concerned with foreign ex change risk. It is possible to deal in a similar way with the risk resulting from un expected future changes of various market variables such as commodity prices, interest rates or stock prices. We shall introduce a measure of risk called Value at Risk (VaR), which has recently become very popular. Derivative securities will be used to design portfolios with a view to reducing this kind of risk. 

Finally, we shall consider an application of options to manufacturing a levered investment, for which increased risk will be accompanied by high expected return. 

## 9.1 Hedging Option Positions

The writer of a European call option is exposed to risk, as the option may end up in the money. The risk profile for a call writer is $C ^ { \mathrm { E } } \mathrm { e } ^ { r T } - ( S ( T ) - X ) ^ { + }$ , where $C ^ { \mathrm { E } } \mathrm { e } ^ { r T }$ is the value at the exercise time $T$ of the premium $C ^ { \mathrm { E } }$ received for the option and invested without risk. Theoretically, the loss to the writer may be unlimited. For a put option the risk profile has the form $P ^ { \mathrm { E } } \mathrm { e } ^ { r T } - ( X - S ( T ) ) ^ { + }$ , with limited loss, though still possibly very large compared to the premium $P ^ { \mathrm { E } }$ received. We shall see how to eliminate or at least reduce this risk over a short time horizon by taking a suitable position in the underlying asset and, if necessary, also in other derivative securities written on the same asset. 

In practice it is impossible to hedge in a perfect way by designing a single portfolio to be held for the whole period up to the exercise time $T .$ . The hedging portfolio will need to be modified whenever the variables afecting the option change with time. In a realistic case of non-zero transaction costs these mod ifications cannot be performed too frequently and some compromise strategy may be required. Nevertheless, here we shall only discuss hedging over a single short time interval, neglecting transaction costs. 

## 9.1.1 Delta Hedging

The value of a European call or put option as given by the Black–Scholes formula clearly depends on the price of the underlying asset. This can be seen in a slightly broader context. 

Consider a portfolio whose value depends on the current stock price $S =$ $S ( 0 )$ and is hence denoted by $V ( S )$ . Its dependence on $S$ can be measured by the derivative $\textstyle { \frac { \mathrm { d } } { \mathrm { d } S } } V ( S )$ , called the delta of the portfolio. For small price variations from $S$ to $S + \varDelta S$ the value of the portfolio will change by 

$$
\varDelta V (S) \cong \frac {\mathrm{d}}{\mathrm{d} S} V (S) \times \varDelta S.
$$

The principle of delta hedging is based on embedding derivative securities in a portfolio, the value of which does not alter too much when $S$ varies. This can be achieved by ensuring that the delta of the portfolio is equal to zero. Such a portfolio is called delta neutral. 

We take a portfolio composed of stock, bonds and the hedged derivative security, its value given by 

$$
V (S) = x S + y + z D (S),
$$

where the derivative security price is denoted by $D ( S )$ and a bond with curren value 1 is used. Specifically, suppose that a single derivative security has been 

written, that is, $z = - 1$ . Then 

$$
\frac {\mathrm{d}}{\mathrm{d} S} V (S) = x - \frac {\mathrm{d}}{\mathrm{d} S} D (S).
$$

The last term $\textstyle { \frac { \mathrm { d } } { \mathrm { d } S } } D ( S )$ , which is the delta of the derivative security, can readily be computed if the model of stock prices is specified, so that an explicit formula for $D ( S )$ is available. 

## Proposition 9.1

Denote the European call option price in the Black–Scholes model by $C ^ { \mathrm { E } } ( S )$ The delta of the option is given by 

$$
\frac {\mathrm{d}}{\mathrm{d} S} C ^ {\mathrm{E}} (S) = N (d _ {1}),
$$

where $N ( x )$ is the normal distribution function given by (8.10) and $d _ { 1 }$ is defined by (8.9). 

## Proof

The price $S = S ( 0 )$ appears in three places in the Black–Scholes formula, see Theorem 8.6, so the diferentiation requires a bit of work, with plenty of nice cancellations in due course, and is left to the reader. Bear in mind that the derivative ${ \frac { \mathrm { d } } { \mathrm { d } S } } C ^ { \mathrm { E } } ( S )$ is computed at time $t = 0$ □ 

## Exercise 9.1

Find a similar expression for the delta $\textstyle { \frac { \mathrm { d } } { \mathrm { d } S } } P ^ { \mathrm { E } } ( S )$ of a European put option in the Black–Scholes model. 

For the remainder of this section we shall consider a European call option within the Black–Scholes model. By Proposition 9.1 the portfolio $( x , y , z ) =$ $( N ( d _ { 1 } ) , y , - 1 )$ , where the position in stock $N ( d _ { 1 } )$ is computed for the initial stock price $S = S ( 0 )$ , has delta equal to zero for any money market position y. Consequently, its value 

$$
V (S) = N (d _ {1}) S + y - C ^ {\mathrm{E}} (S)
$$

does not vary much under small changes of the stock price about the initial value. It is convenient to choose y so that the initial value of the portfolio is equal to zero. By the Black–Scholes formula for $C ^ { \mathrm { E } } ( S )$ this gives 

$$
y = - X \mathrm{e} ^ {- T r} N (d _ {2}),
$$

with $d _ { 2 }$ is given by (8.9). 

Let us analyse the following example, which will subsequently be expanded and modified. Suppose that the risk-free rate is 8% and consider a 90-day call option with strike price $X = 6 0$ dollars written on a stock with current price $S = 6 0$ dollars. Assume that the stock volatility is $\sigma = 3 0 \%$ . The Black–Scholes formula gives the option price $C ^ { \mathrm { E } } = 4 . 1 4 4 5 2$ dollars, the delta of the option being equal to 0.581957. 

Suppose that we write and sell 1, 000 call options, cashing a premium of $4, 144.52. To construct the hedge we buy 581.96 shares for $34, 917.39, borrowing $30, 772.88. Our portfolio will be $( x , y , z )$ with $x = 5 8 1 . 9 6 , y = - 3 0 , 7 7 2 . 8 8$ $z = - 1$ , 000 and with total value zero. (While it might be more natural math ematically to consider a single option with $z = - 1$ , in practice options are traded in batches.) 

We shall analyse the value of the portfolio after one day by considering some possible scenarios. The time to expiry will then be 89 days. Suppose that the stock volatility and the risk-free rate do not vary, and consider the following three scenarios of stock price movements: 

1. The stock price remains unaltered, $S ( \frac { 1 } { 3 6 5 } ) = 6 0$ dollars. A single option is now worth $4.11833, so our liability due to the short position in options is reduced. Our debt on the money market is increased by the interest due. The position in stock is worth the same as initially. The balance on day one is 

<table><tr><td>stock</td><td>34,917.39</td></tr><tr><td>money</td><td>-30,779.62</td></tr><tr><td>options</td><td>-4,118.33</td></tr><tr><td>TOTAL</td><td>19.45</td></tr></table>

Without hedging $( x = 0 , y = 4 , 1 1 8 . 3 3 , z = - 1 , 0 0 0 )$ our wealth would have been $27.10, that is, we would have benefited from the reduced value of the option and the interest due on the premium invested without risk. 

2. The stock price goes up to $\begin{array} { r } { S ( \frac { 1 } { 3 6 5 } ) = 6 1 } \end{array}$ dollars. A single option is now worth $4.72150, which is more than initially. The unhedged (naked) position would have sufered a loss of $576.07. On the other hand, for a holder of a delta neutral portfolio the loss on the options is almost completely balanced out by the increase in the stock value: 

<table><tr><td>stock</td><td>35,499.35</td></tr><tr><td>money</td><td>-30,779.62</td></tr><tr><td>options</td><td>-4,721.50</td></tr><tr><td>TOTAL</td><td>-1.77</td></tr></table>

3. The stock price goes down to $\begin{array} { r } { S ( \frac { 1 } { 3 6 5 } ) = 5 9 } \end{array}$ dollars. The value of the written options decreases, a single option now being worth $3.55908. The value of the stock held decreases too. The portfolio brings a small loss: 

<table><tr><td>stock</td><td>34,335.44</td></tr><tr><td>money</td><td>-30,779.62</td></tr><tr><td>options</td><td>-3,559.08</td></tr><tr><td>TOTAL</td><td>-3.26</td></tr></table>

In this scenario it would have been much better not to have hedged at all, since then we would have gained $586.35. 

It may come as a surprise that the hedging portfolio brings a profit when the stock price remains unchanged. As we shall see later in Exercise 9.5, a general rule is at work here. 

## Exercise 9.2

Find the stock price on day one for which the hedging portfolio attains its maximum value. 

## Exercise 9.3

Suppose that 50, 000 puts with exercise date in 90 days and strike price $X = 1 . 8 0$ dollars are written on a stock with current price $S ( 0 ) = 1 . 8 2 $ dollars and volatility $\sigma = 1 4 \%$ . The risk-free rate is $r = 5 \%$ . Construct a delta neutral portfolio and compute its value after one day if the stock price drops to $\begin{array} { r } { S ( \frac { 1 } { 3 6 5 } ) = 1 . 8 1 } \end{array}$ dollars. 

Going back to our example, let us collect the values V of the delta neutral portfolio for various stock prices after one day as compared to the values U of the unhedged position: 

<table><tr><td>S</td><td>V</td><td>U</td></tr><tr><td>58.00</td><td>-71.35</td><td>1,100.22</td></tr><tr><td>58.50</td><td>-31.56</td><td>849.03</td></tr><tr><td>59.00</td><td>-3.26</td><td>586.35</td></tr><tr><td>59.50</td><td>13.69</td><td>312.32</td></tr><tr><td>60.00</td><td>19.45</td><td>27.10</td></tr><tr><td>60.50</td><td>14.22</td><td>-269.11</td></tr><tr><td>61.00</td><td>-1.77</td><td>-576.07</td></tr><tr><td>61.50</td><td>-28.24</td><td>-893.53</td></tr><tr><td>62.00</td><td>-64.93</td><td>-1,221.19</td></tr></table>

Now, let us see what happens if the stock price changes are considerable: 

<table><tr><td>S</td><td>V</td><td>U</td></tr><tr><td>50</td><td>-2,233.19</td><td>3,594.03</td></tr><tr><td>55</td><td>-554.65</td><td>2,362.79</td></tr><tr><td>60</td><td>19.45</td><td>27.10</td></tr><tr><td>65</td><td>-481.60</td><td>-3,383.73</td></tr><tr><td>70</td><td>-1,765.15</td><td>-7,577.06</td></tr></table>

If we fear that such large changes might happen, the above hedge is not a satisfactory solution. If we do not hedge, at least we have a gamble with a positive outcome whenever the stock price goes down. Meanwhile, no matter whether the stock price goes up or down, the delta neutral portfolio may bring losses, though considerably smaller than the naked position. 

Let us see what can happen if some other variables, in addition to the stock price, change after one day: 

1. Suppose that the interest rate increases to 9% with volatility as before. Some loss will result from an increase in the option value. The interest on the cash loan due on day one is not afected because the new rate will only have an efect on the interest payable on the second day or later. The values of the hedging portfolio are given in the second column in the table below. 

2. Now suppose that σ grows to 32%, with the interest rate staying at the original level of 8%. The option price will increase considerably, which is not compensated by the stock position even if the stock price goes up. The results are given in the third column in the following table: 

<table><tr><td rowspan="2">S</td><td colspan="2">V</td></tr><tr><td>r=9%,σ=30%</td><td>r=8%,σ=32%</td></tr><tr><td>58.00</td><td>-133.72</td><td>-299.83</td></tr><tr><td>58.50</td><td>-97.22</td><td>-261.87</td></tr><tr><td>59.00</td><td>-72.19</td><td>-234.69</td></tr><tr><td>59.50</td><td>-58.50</td><td>-218.14</td></tr><tr><td>60.00</td><td>-55.96</td><td>-212.08</td></tr><tr><td>60.50</td><td>-64.38</td><td>-216.33</td></tr><tr><td>61.00</td><td>-83.51</td><td>-230.68</td></tr><tr><td>61.50</td><td>-113.07</td><td>-254.90</td></tr><tr><td>62.00</td><td>-152.78</td><td>-288.74</td></tr></table>

As we can see, in some circumstances delta hedging may be far from satisfactory. We need to improve the stability of hedging when the underlying asset price changes considerably and/or some other variables change simultaneously. In what follows, after introducing some theoretical tools we shall return again to the current example. 

## Exercise 9.4

Find the value of the delta neutral portfolio in Exercise 9.3 if the risk-free rate of interest decreases to 3% on day one. 

## 9.1.2 Greek Parameters

We shall define so-called Greek parameters describing the sensitivity of a portfolio with respect to the various variables determining the option price. The strike price X and expiry date T are fixed once the option is written, so we have to analyse the four remaining variables S, t, r, σ. 

Let us write the value of a general portfolio containing stock and some contingent claims based on this stock as a function $V ( S , t , \sigma , r )$ of these variables and denote 

$$
\begin{array}{c} \mathrm{delta} _ {V} = \frac {\partial V}{\partial S}, \\ \mathrm{gamma} _ {V} = \frac {\partial^ {2} V}{\partial S ^ {2}}, \\ \mathrm{theta} _ {V} = \frac {\partial V}{\partial t}, \\ \mathrm{vega} _ {V} = \frac {\partial V}{\partial \sigma}, \\ \mathrm{rho} _ {V} = \frac {\partial V}{\partial r}. \end{array}
$$

For small changes ∆S, ∆t, ∆σ, ∆r of the variables we have the following approximate equality (by the Taylor formula): 

$$
\begin{array}{l} \Delta V \cong \mathrm{delta} _ {V} \times \Delta S + \mathrm{theta} _ {V} \times \Delta t + \mathrm{vega} _ {V} \times \Delta \sigma + \mathrm{rho} _ {V} \times \Delta r \\ \qquad + \frac {1}{2} \mathrm{gamma} _ {V} \times (\Delta S) ^ {2}. \end{array}
$$

Hence, a way to immunise a portfolio against small changes of a particular vari able is to ensure that the corresponding Greek parameter is equal to zero. For instance, to hedge against volatility movements we should construct a vega neu tral portfolio, with vega equal to zero. To retain the benefits of delta hedging, we should design a portfolio with both delta and vega equal to zero (deltavega neutral). A delta-gamma neutral portfolio will be immune against larger changes of the stock price. Examples of such hedging portfolios will be examined below. 

The Black–Scholes formula allows us to compute the derivatives explicitly for a single option. For a European call we have 

$$
\mathrm{delta} _ {C ^ {\mathrm{E}}} = N (d _ {1}),
$$

$$
\mathrm{gamma} _ {C ^ {\mathrm{E}}} = \frac {1}{S \sigma \sqrt {2 \pi T}} \mathrm{e} ^ {- \frac {d _ {1} ^ {2}}{2}},
$$

$$
\mathrm{theta} _ {C ^ {\mathrm{E}}} = - \frac {S \sigma}{2 \sqrt {2 \pi T}} \mathrm{e} ^ {- \frac {d _ {1} ^ {2}}{2}} - r X \mathrm{e} ^ {- r T} N (d _ {2}),
$$

$$
\mathrm{vega} _ {C ^ {\mathrm{E}}} = \frac {S \sqrt {T}}{\sqrt {2 \pi}} e ^ {- \frac {d _ {1} ^ {2}}{2}},
$$

$$
\mathrm{rho} _ {C ^ {\mathrm{E}}} = T X \mathrm{e} ^ {- r T} N (d _ {2}).
$$

(The Greek parameters are computed at time $t = 0 . )$ 

## Remark 9.1

It is easy to see from the above that 

$$
\mathrm{theta} _ {C ^ {\mathrm{E}}} + r S \mathrm{delta} _ {C ^ {\mathrm{E}}} + \frac {1}{2} \sigma^ {2} S ^ {2} \mathrm{gamma} _ {C ^ {\mathrm{E}}} = r C ^ {\mathrm{E}}.
$$

In general, the price D of any European derivative security can be shown to satisfy the Black–Scholes equation 

$$
\frac {\partial D}{\partial t} + r S \frac {\partial D}{\partial S} + \frac {1}{2} \sigma^ {2} S ^ {2} \frac {\partial^ {2} D}{\partial S ^ {2}} = r D.
$$

## Exercise 9.5

Show that a delta neutral portfolio with initial value zero hedging a single call option will gain in value with time if the stock price, volatility and risk-free rate remain unchanged. 

## Exercise 9.6

Derive formulae for the Greek parameters of a put option. 

## 9.1.3 Applications

To show some possibilities ofered by Greek parameters we consider hedging the position of a writer of European call options. 

Delta-Gamma Hedging. The construction is based on making both delta and gamma zero. A portfolio of the form $( x , y , z )$ is insuficient for this. Given the position in options, say $z = - 1 , 0 0 0$ , there remains only one parameter that can be adjusted, namely the position x in the underlying. This allows us to make the delta of the portfolio zero. To make the gamma also equal to zero an additional degree of freedom is needed. To this end we consider another option on the same underlying stock, for example, a call expiring after 60 days, $\widehat { T } = 6 0 / 3 6 5$ , with strike price ${ \widehat { X } } = 6 5$ , and construct a portfolio $( x , y , z , { \widehat { z } } )$ where $\widehat { z }$ %is a position in the additional option. The other variables are as in the %previous examples: $r = 8 \% , \sigma = 3 0 \% , S ( 0 ) = 6 0$ 

Let us sum up all the information about the prices and selected Greek parameters (we also include vega, which will be used later): 

<table><tr><td>option</td><td>time to expiry</td><td>strike price</td><td>option price</td><td>delta</td><td>gamma</td><td>vega</td></tr><tr><td>original</td><td>90/365</td><td>60</td><td>4.14452</td><td>0.581957</td><td>0.043688</td><td>11.634305</td></tr><tr><td>additional</td><td>60/365</td><td>65</td><td>1.37826</td><td>0.312373</td><td>0.048502</td><td>8.610681</td></tr></table>

We choose x and $\widehat { z }$ so that the delta and gamma of the portfolio are zero, 

$$
\mathrm{delta} _ {V} = x - 1, 0 0 0 \mathrm{delta} _ {C ^ {\mathrm{E}}} + \widehat {z} \mathrm{delta} _ {\widehat {C} ^ {\mathrm{E}}} = 0,
$$

$$
\mathrm{gamma} _ {V} = - 1, 0 0 0 \mathrm{gamma} _ {C ^ {\mathrm{E}}} + \widehat {z} \mathrm{gamma} _ {\widehat {C} ^ {\mathrm{E}}} = 0,
$$

and the money position y so that the value of the portfolio is zero, 

$$
V (S) = x S + y - 1, 0 0 0 C ^ {\mathrm{E}} (S) + \widehat {z} \widehat {C} ^ {\mathrm{E}} (S) = 0.
$$

This gives the following system of equations: 

$$
\begin{array}{c} x - 5 8 1. 9 5 7 + 0. 3 1 2 3 7 3 \widehat {z} = 0, \\ - 4 3. 6 8 8 + 0. 0 4 8 5 0 2 \widehat {z} = 0, \end{array}
$$

with solution $x \cong 3 0 0 . 5 8 , \widehat { z } \cong 9 0 0 . 7 6$ . It follows that $y \cong - 1 5 , 1 3 1 . 7 7$ . That %is, we take long positions in stock and the additional option, and a short cash position. (We already have a short position $z = - 1 , 0 0 0$ in the original option.) 

After one day, if stock goes up, the original option will become more expensive, increasing our liability, which will be set of by increases in the value of stock and the additional options held. The reverse happens if the stock price declines. Our money debt increases in either case by the interest due after one day. The values of the portfolio are given below (for comparison we also recall the values of the delta neutral portfolio): 

<table><tr><td><eq>S(\frac{1}{365})</eq></td><td>delta-gamma</td><td>delta</td></tr><tr><td>58.00</td><td>-2.04</td><td>-71.35</td></tr><tr><td>58.50</td><td>0.30</td><td>-31.56</td></tr><tr><td>59.00</td><td>1.07</td><td>-3.26</td></tr><tr><td>59.50</td><td>0.81</td><td>13.69</td></tr><tr><td>60.00</td><td>0.02</td><td>19.45</td></tr><tr><td>60.50</td><td>-0.79</td><td>14.22</td></tr><tr><td>61.00</td><td>-1.11</td><td>-1.77</td></tr><tr><td>61.50</td><td>-0.49</td><td>-28.24</td></tr><tr><td>62.00</td><td>1.52</td><td>-64.93</td></tr></table>

We can see that we are practically safe within the given range of stock prices. For larger changes we are also in a better position as compared with delta hedging: 

<table><tr><td><eq>S(\frac{1}{365})</eq></td><td>delta-gamma</td><td>delta</td></tr><tr><td>50</td><td>-614.08</td><td>-2,233.19</td></tr><tr><td>55</td><td>-78.22</td><td>-554.65</td></tr><tr><td>60</td><td>0.02</td><td>19.45</td></tr><tr><td>65</td><td>63,13</td><td>-481.60</td></tr><tr><td>70</td><td>440.81</td><td>-1,765.15</td></tr></table>

As predicted, a delta-gamma neutral portfolio ofers better protection against stock price changes than a delta neutral one. 

Delta-Vega Hedging. Next we shall hedge against an increase in volatility, while retaining cover against small changes in the stock price. This will be achieved by constructing a delta-vega neutral portfolio containing, as before, an additional option. The conditions imposed are 

$$
\mathrm{delta} _ {V} = x - 1, 0 0 0 \mathrm{delta} _ {C ^ {\mathrm{E}}} + \widehat {z} \mathrm{delta} _ {\widehat {C} ^ {\mathrm{E}}} = 0,
$$

$$
\mathrm{vega} _ {V} = - 1, 0 0 0 \mathrm{vega} _ {C ^ {\mathrm{E}}} + \widehat {z} \mathrm{vega} _ {\widehat {C} ^ {\mathrm{E}}} = 0.
$$

They lead to the system of equations 

$$
\begin{array}{c} x - 5 8 1. 9 5 7 + 0. 3 1 2 3 7 3 \widehat {z} = 0, \\ - 1, 1 6 3 4. 3 0 5 + 8. 6 1 0 6 8 1 \widehat {z} = 0, \end{array}
$$

with an approximate solution $x \cong 1 5 9 . 8 9 , \widehat { z } \cong 1 , 3 5 1 . 1 5$ . The corresponding money position is $y \cong - 7 , 3 1 1 . 1 2$ 

Suppose that the volatility increases to $\sigma = 3 2 \%$ on day one. Let us compare the results for delta-vega and delta hedging: 

<table><tr><td>S(1/365)</td><td>delta-vega</td><td>delta</td></tr><tr><td>58.00</td><td>-5.90</td><td>-299.83</td></tr><tr><td>58.50</td><td>-12.81</td><td>-261.87</td></tr><tr><td>59.00</td><td>-16.05</td><td>-234.69</td></tr><tr><td>59.50</td><td>-14.99</td><td>-218.14</td></tr><tr><td>60.00</td><td>-9.06</td><td>-212.08</td></tr><tr><td>60.50</td><td>2.27</td><td>-216.33</td></tr><tr><td>61.00</td><td>19.52</td><td>-230.68</td></tr><tr><td>61.50</td><td>43.17</td><td>-254.90</td></tr><tr><td>62.00</td><td>73.62</td><td>-288.74</td></tr></table>

## Exercise 9.7

Using the data in our ongoing example (stock price $60, volatility 30%, interest rate 8%), construct a delta-rho neutral portfolio to hedge a short position of 1, 000 call options expiring after 90 days with strike price $60, taking as an additional component a call option expiring after 120 days with strike price $65. Analyse the sensitivity of the portfolio value to stock price variations if the interest rate goes up to 9% after one day, comparing with the previous results. What will happen if the interest rate jumps to 15%? 

The examples above illustrate the variety of possible hedging strategies. The choice between them depends on individual aims and preferences. We have not touched upon questions related to transaction costs or long term hedging. Nor have we discussed the optimality of the choice of an additional derivative instru ment. Portfolios based on three Greek parameters would require yet another derivative security as a component. They could provide comprehensive cover, though their performance might deteriorate if the variables remain unchanged. In addition, they might prove expensive if transaction costs were included. 

## 9.2 Hedging Business Risk

We begin by introducing an alternative measure of risk, related to an intuitive understanding of risk as the size and likelihood of a possible loss. 

## 9.2.1 Value at Risk

Let us present the basic idea using a simple example. We buy a share of stock for $S ( 0 ) = 1 0 0$ dollars to sell it after one year. The selling price $S ( 1 )$ is random. We shall sufer a loss if $S ( 1 ) < 1 0 0 \mathrm { e } ^ { r }$ , where r is the risk-free rate under continuous compounding. (The purchase can either be financed by a loan, or, if the initial sum is already at our disposal, we take into account the foregone opportunity of a risk-free investment.) What is the probability of a loss being less than a given amount, for example, 

$$
P (1 0 0 \mathrm{e} ^ {r} - S (1) <   2 0) = ?
$$

Let us reverse the question and fix the probability, 95% say. Now we seek an amount such that the probability of a loss not exceeding this amount is 95%. This is referred to as Value at Risk at 95% confidence level and denoted by VaR. (Other confidence levels can also be used.) So, VaR is an amount such that 

$$
P (1 0 0 \mathrm{e} ^ {r} - S (1) <   \mathrm{VaR}) = 95 \%.
$$

It should be noted that the majority of textbooks neglect the time value of money in this context, stating the definition of VaR only for $r = 0$ 

## Example 9.1

Suppose that the distribution of the stock price is log normal, the logarithmic return $k = \ln ( S ( 1 ) / S ( 0 ) )$ having normal distribution with mean $m = 1 2 \%$ and standard deviation $\sigma = 3 0 \%$ . With probability 95% the return will satisfy $k > m + x \sigma \cong - 3 7 . 5 0 \%$ , where $N ( x ) \cong 5 \%$ , so $x \cong - 1 . 6 4 5$ . (Here $N ( x )$ is the normal distribution function (8.10) with mean 0 and variance 1.) Hence with probability 95% the future price S(1) will satisfy 

$$
S (1) > S (0) \mathrm{e} ^ {m + x \sigma} \cong 6 8. 8 3 \text {   dollars },
$$

and so, given that $r = 8 \%$ , 

$$
\mathrm{VaR} = S (0) \mathrm{e} ^ {r} - S (0) \mathrm{e} ^ {m + x \sigma} \cong 3 9. 5 0 \text { dollars }.
$$

## Exercise 9.8

Evaluate VaR at 95% confidence level for a one-year investment of $1, 000 into euros if the interest rate for risk-free investments in euros is $r _ { \mathrm { E U R } } =$ 4% and the exchange rate from euros into US dollars follows the log normal distribution with $m = 1 \%$ and $\sigma = 1 5 \%$ . Take into account the foregone opportunity of investing dollars without risk, given that the risk-free interest rate for dollars is $r _ { \mathrm { U S D } } = 5 \%$ 

## Exercise 9.9

Suppose that $1, 000 is invested in European call options on a stock with current price S(0) = 60 dollars. The options expire after 6 months with strike price X = 40 dollars. Assume that $\sigma = 3 0 \% , r = 8 \%$ , and the expected logarithmic return on stock is 12%. Compute VaR after 6 months at 95% confidence level. Find the final wealth if the stock price grows at the expected rate. Find the stock price level that will be exceeded with 5% probability and compute the corresponding final payof. 

## 9.2.2 Case Study

We shall discuss a number of ways in which VaR can be managed with the aid of derivative securities. The methods will be illustrated by a simple example of business activity. 

## Case 9.1

A company manufactures goods in the UK for sale in the USA. The investment to start production is 5 million pounds. Additional funds can be raised by borrowing British pounds at 16% to finance a hedging strategy. The rate of return demanded by investors, bearing in mind the risk involved, is 25%. The sales are predicted to generate 8 million dollars at the end of the year. The manufacturing costs are 3 million pounds per year. The interest rate is 8% for dollars and 11% for pounds. The current rate of exchange is 1.6 dollars to a pound. The volatility of the logarithmic return on the rate of exchange is estimated at 15%. The company pays 20% tax on earnings. 

First note that to satisfy the expectations of investors the company should be able to achieve a profit of 1.25 million pounds a year to pay the dividend. A lower profit would mean a loss. The profit depends on the rate of exchange d at the end of the year, hence some risk emerges. (We assume that the other values will be as predicted.) 

To begin with, suppose that no action is taken to manage the risk. 

1. Unhedged Position. If the exchange rate d turns out to be 1.6 dollars to a pound at the end of the year, then the net earnings will be 1.6 million pounds, as shown in the following profit and loss statement (all amounts in 

pounds): 

<table><tr><td>sales</td><td>5,000,000</td></tr><tr><td>cost of sales</td><td>-3,000,000</td></tr><tr><td>earnings before tax</td><td>2,000,000</td></tr><tr><td>tax</td><td>-400,000</td></tr><tr><td>earnings after tax</td><td>1,600,000</td></tr><tr><td>dividend</td><td>-1,250,000</td></tr><tr><td>result</td><td>350,000</td></tr></table>


The surplus income will be 0.35 million pounds. 


However, if the exchange rate d becomes 2 dollars to a pound, the company will end up with a loss of 0.45 million pounds (and the dividend will in fact have to be reduced): 

<table><tr><td>sales</td><td>4,000,000</td></tr><tr><td>cost of sales</td><td>-3,000,000</td></tr><tr><td>earnings before tax</td><td>1,000,000</td></tr><tr><td>tax</td><td>-200,000</td></tr><tr><td>earnings after tax</td><td>800,000</td></tr><tr><td>dividend</td><td>-1,250,000</td></tr><tr><td>result</td><td>-450,000</td></tr></table>

Let us compute VaR. We assume that the rate of exchange has lognormal distribution with mean return equal to the diference between the interest rates, $8 \% - 1 1 \% = - 3 \% . 1$ With the volatility of the return on the exchange rate at 15%, the return on the investment will exceed 3% + $1 . 6 5 \times 1 5 \% = 2 1 . 7 5 \%$ with probability 95%. This corresponds to an exchange rate $d = 1 . 6 \times \mathrm { e } ^ { 2 1 . 7 5 \% } \cong 1 . 9 8 8 7$ dollars to a pound, for which the income statement will be as follows (all amounts rounded to the nearest pound): 

<table><tr><td>sales</td><td>4,022,728</td></tr><tr><td>cost of sales</td><td>-3,000,000</td></tr><tr><td>earnings before tax</td><td>1,022,728</td></tr><tr><td>tax</td><td>-204,546</td></tr><tr><td>earnings after tax</td><td>818,182</td></tr><tr><td>dividend</td><td>-1,250,000</td></tr><tr><td>result</td><td>-431,818</td></tr></table>

As a result, $\mathrm { V a R } \cong 4 3 1 , 8 1 8$ dollars. The final balance as a function of the exchange rate d is 

$$
\begin{aligned} b(d) & = 80\% \times (\frac {8,000,000}{d} -3,000,000) - 1,250,000 \\ & = \frac {6,400,000}{d} -3,650,000. \end{aligned}
$$

The break even exchange rate, which solves $b ( d ) = 0$ , is approximately equal to 1.7534 dollars to a pound. In an optimistic scenario in which the pound weakens, for example, down to 1.5 dollars, the final balance will be about £616, 666. 

The question is how to manage this risk exposure. 

2. Forward Contract. The easiest solution would be to fix the exchange rate in advance by entering into a long forward contract. The forward rate is $1 . 6 \times \mathrm { e } ^ { - 3 \% } \cong 1 . 5 5 2 7$ dollars to a pound. As a result, the company can obtain the following statement with guaranteed surplus, but no possibility of further gains should the exchange rate become more favourable: 

<table><tr><td>sales</td><td>5,152,315</td></tr><tr><td>cost of sales</td><td>-3,000,000</td></tr><tr><td>earnings before tax</td><td>2,152,315</td></tr><tr><td>tax</td><td>-430,463</td></tr><tr><td>net income</td><td>1,721,852</td></tr><tr><td>dividend</td><td>-1,250,000</td></tr><tr><td>result</td><td>471,852</td></tr></table>

3. Full Hedge with Options. Options can be used to ensure that the rate of exchange is capped at a certain level, whilst the benefits associated with favourable exchange rate movements are retained. However, this may be costly because of the premium paid for options. 

The company can buy call options on the exchange rate. A European call to buy one pound with strike price 1.6 dollars to a pound will cost £0.0669.<sup>2</sup> Suppose that the company buys 5 million of such options, paying a £334, 510 premium, which they have to borrow at 16%. The interest is tax deductible, making the loan less costly. Nevertheless, the final result is 


disappointing:


<table><tr><td>sales</td><td>5,000,000</td></tr><tr><td>cost of sales</td><td>-3,000,000</td></tr><tr><td>earnings before interest and tax</td><td>2,000,000</td></tr><tr><td>interest</td><td>-53,522</td></tr><tr><td>earnings before tax</td><td>1,946,478</td></tr><tr><td>tax</td><td>-389,296</td></tr><tr><td>net income</td><td>1,557,182</td></tr><tr><td>loan repaid</td><td>-334,510</td></tr><tr><td>dividend</td><td>-1,250,000</td></tr><tr><td>result</td><td>-27,328</td></tr></table>

The optimal (in the sense of minimising the loss) strike price is 1.5734 dollars to a pound, resulting in a loss of £24, 283. If the exchange rate drops to 1.5 dollars to a pound, the options will not be exercised and the sum obtained from sales will reach £5, 333, 333, with a positive final result of £239, 339. This strategy leads to a better result than the hedge involving a forward contract only if the rate of exchange drops below 1.42 dollars to a pound. 

4. Partial Hedge with Options. To reduce the cost of options the company can hedge partially by buying call options to cover only a fraction of the dollar amount from sales. Suppose that the company buys 2, 500, 000 units of the same call option as above, paying a half of the previous premium. A half of the revenue is then exposed to risk. To find VaR at 95% confidence level we assume that this sum is exchanged at 1.9887 dollars to a pound, as in the case of an unhedged position, the other half being exchanged at the exercise price: 

<table><tr><td>sales</td><td>4,511,364</td></tr><tr><td>cost of sales</td><td>-3,000,000</td></tr><tr><td>earnings before interest and tax</td><td>1,511,364</td></tr><tr><td>interest</td><td>-26,761</td></tr><tr><td>earnings before tax</td><td>1,484,603</td></tr><tr><td>tax</td><td>-296,921</td></tr><tr><td>net income</td><td>1,187,682</td></tr><tr><td>loan repaid</td><td>-167,255</td></tr><tr><td>dividend</td><td>-1,250,000</td></tr><tr><td>result</td><td>-229,573</td></tr></table>

If the exchange rate drops to 1.5 dollars to a pound, the company will have a surplus of £428, 003. 

5. Combination of Options and Forward Contracts. Finally, let us inves tigate what happens if the company hedges with both kinds of derivatives. Half of their position will be hedged with options. In the worst case scenario they will buy pounds for half of their dollar revenue at the rate of 1.6 dollars to a pound, the remaining half being exchanged at the forward rate of 1.5527 dollars to a pound. The outcome is shown below, where we summarise the resulting VaR for all strategies considered (the result below is equal to minus VaR): 

$$
\begin{array}{c c c c c c} \text {strategy} & 1 & 2 & 3 & 4 & 5 \\ \text {result} & - 4 3 1, 8 1 8 & 4 7 1, 8 5 2 & - 2 7, 3 2 8 & - 2 2 9, 5 7 3 & 2 2 2, 2 6 3 \end{array}
$$

These values are computed at 95% confidence level, corresponding to the exchange rate of 1.9887 dollars to a pound. 

Clearly, VaR provides only partial information about possible outcomes of various strategies. Figure 9.1 shows the graphs of the final result as a function of the exchange rate d for each of the above strategies. The graphs are labelled by the strategy number as above. The strategy using a forward contract (strat 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/aabca44ef0853a284b76ef045661c615529df105e1bb5ba5c28fcf593a8053ad.jpg)



Figure 9.1 Comparison of various strategies


egy 2) appears to be the safest one. An adventurous investor who strongly believes that the pound will weaken considerably may prefer to remain uncovered (strategy 1). A variety of middle-of-the-road strategies are also available. The probability distribution of the exchange rate d should also be taken into account when examining the graphs. 

## 9.3 Speculating with Derivatives

## 9.3.1 Tools

Options can be used as building blocks to design sophisticated investment instruments. We shall consider an investor with specific views on the future behaviour of stock prices and willing to take risks. Our task will be to design a portfolio of securities with a prescribed payof profile that would satisfy this kind of investor. 

Suppose that the investor expects the stock price to rise and wants to gamble on that. One simple way is to buy a call option. An option with strike price $X ^ { \prime }$ close to the current stock price is considerably cheaper than the stock itself, creating a risky leverage position, as will be seen in the case study to follow. The premium may be reduced by selling a call option with strike price $X ^ { \prime \prime } > X ^ { \prime }$ . In this way we can build a so-called bull spread with payof shown in Figure 9.2. This strategy will bring a good return if stock price increases are moderate. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/5764319fd305e202c43504a189439bf1b9d98732c7e7f36373eb4f1d3ed8c56b.jpg)



Figure 9.2 Bull spread


Using put options with strike prices $X ^ { \prime } < X ^ { \prime \prime }$ ', selling the former and purchasing the latter, we can construct a bear spread with positive payoff for low future stock prices, see Figure 9.3. This may be employed by an investor who expects a moderate decline in the stock price. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/3119c07cd959ba2f4eeca2b3c72ccc728453c913594231da755dc93c269ee584.jpg)



Figure 9.3 Bear spread


An investor who believes that the stock price will stay unaltered or change insignificantly may choose a butterfly. It is constructed from three call options with strike prices $X ^ { \prime } < X ^ { \prime \prime } < X ^ { \prime \prime \prime }$ . Two calls are bought, one with strike $X ^ { \prime }$ and one with strike $X ^ { \prime \prime \prime }$ , and two calls with strike price $X ^ { \prime \prime }$ are sold. Figure 9.4 shows the case when $X ^ { \prime \prime }$ is the average of the other two strike prices. Reversed butterfly is the opposite strategy, bringing profits when the stock price changes. (We have already come across the butterfly in the proof of Proposition 7.8.) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/b115a7dcb14dc64d61dc11dca9cdb4be0adcb4c90407a62a9de5d6db746a4383.jpg)



Figure 9.4 Butterfly


Finally, we observe that any continuous payof function consisting of straight line segments can be manufactured from put and call options. Figure 9.5 out lines the step-by-step decomposition of a target profile into a portfolio of options with various strike price values. The number of options for each strike price is chosen to match the slopes of the target profile. Such a construction is suficient for practical purposes because any continuous payof function can be approximated by straight line segments. 

## 9.3.2 Case Study

We shall combine the portfolio theory techniques with the tools described above. We have in mind an investor with specific views on the future prices of assets, who is prepared to accept some risk in order to increase expected return. 

## Case 9.2

An investor with $15, 000 believes that a certain stock price should rise during the next month, with expected annualised return $\mu _ { S } = 3 1 \%$ . The current stock price is $S ( 0 ) = 6 0 $ dollars. Call options expiring in 20 days with strike price $60 are available at $2.112. The efective risk-free rate is 12%. 

To analyse this case we shall use the binomial model, assuming that trading takes place once a day and that the market probabilities are the same for up and down price jumps. We also assume for simplicity that there are 360 days in a year. The risk-free return over 20 days is $r _ { F } \cong 0 . 6 3 1 6 \%$ . (Implied by the efec tive rate of 12%.) The $15, 000 invested without risk would become $15, 094.74 at the end of the 20-day period. Consider the following risky investments: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/d521e569dc26abbac66627462ba972b2f077082c22106ae6de008eaf3f34b043.jpg)



Figure 9.5 Decomposition of a target payof into options


1. Stock. An investment in stock should bring an expected return of $\mu _ { S } \cong$ 1.5115%. (Equivalent to 31% annually.) Buying 250 shares, the investor would expect to end up with $15, 226.72 after 20 days. The risk can be estimated from the option price, see below. 

2. Call Options. A more risky alternative is to buy call options. The return 

is random and depends on the stock price after 20 days, 

$$
K _ {C} = \frac {(S (2 0 / 3 6 5) - 6 0) ^ {+} - C}{C}.
$$

To compute the expected return on an option we can find the parameters of the binomial model consistent with the option price and the expected return on stock, assuming that the market probability of up and down price movements is 1/2. First we find the risk-free return over a single day, 

$$
r = (1 + 12\%)^{\frac{1}{360}} - 1 \cong 0.0315\% .
$$

Then we write down a condition on the up and down daily stock returns such that the expected annual return is 31%, 

$$
\frac {u + d}{2} = (1 + 31\%) ^ {\frac {1}{360}} - 1 \cong 0.075 \%.
$$

The call price gives another condition for u and d, and we finally arrive at the following values:<sup>3</sup> 

$$
u \cong 1.85\%, \quad d \cong -1.70\% .
$$

Now we can compute the standard deviation for the period in question (using the actual market probabilities $p _ { k } = { \binom { 2 0 } { k } } 0 . 5 ^ { 2 0 } , k = 0 , 1 , . . . , 2 0 )$ , 

$$
\sigma_ {S} \cong 8. 0 9 6 2 \%.
$$

Finally, we compute the expected return and risk of the investment in options, 

$$
\mu_ {C} \cong 14.1268\%, \quad \sigma_ {C} \cong 153.006\% .
$$

The return is impressive, but so is the risk. Observe that with probability 0.4119 the investor can lose all his or her money. 

3. Forward Contracts. The forward price is approximately $60.38. Suppose that entering into a forward contract requires a 20% deposit of the initial stock price, that is $12 per share. The investor can aford to enter into 1, 250 forward contracts. The expected return and risk in the binomial model are 

$$
\mu_ {F} \cong 4. 3 9 9 3 \%, \quad \sigma_ {F} \cong 4 0. 4 8 1 1 \%.
$$

Note that if the stock price falls below $48.38, the investor will lose the deposit and sufer an additional loss, resulting in a return below 100%. 

4. Options Combined with Risk-Free Investment. The risk can be ad justed to an arbitrary level if options are combined with a risk-free asset. Suppose that the investor is willing to accept similar risk to the stock investment. Investing 94.77% of the capital without risk and the remainder in options, the investor can construct a portfolio with the same standard deviation as that for the stock. The expected return on the portfolio is slightly lower than that on stock, 

$$
\mu_ {P} \cong 1.3457\%, \quad \sigma_ {P} \cong 8.0962 \% .
$$

## Remark 9.2

The slope of the line connecting the risk-free asset F with any other portfolio A on the $( \sigma , \mu )$ plane is given by $\frac { \mu _ { A } - r _ { F } } { \sigma _ { A } }$ , called the market price of risk. It can be used to compare diferent portfolios: Those with steep slope are preferable. We can see that the above risky investments have similar values of the marke price of risk, about 0.1 in each case. (These values would in fact be identical if the Black–Scholes model were used for stock prices.) 

The advantage of the investment in a portfolio of options and risk-free assets can be seen if we consider VaR, given in the table below for two diferent confidence levels (chosen to be compatible with the probabilities in the binomial model). On the other hand, VaR would be disastrously high if the whole amount were invested only in options: The investor could lose everything at the given confidence levels. 

<table><tr><td>Investment</td><td>Stock</td><td>Call options</td><td>Forwards</td><td>Calls with risk-free asset</td></tr><tr><td>Market price of risk</td><td>0.1087</td><td>0.0882</td><td>0.0931</td><td>0.0882</td></tr><tr><td>VaR at 94.23%</td><td>$1,931.78</td><td>$15,000.00</td><td>$9,753.63</td><td>$798.73</td></tr><tr><td>VaR at 99.41%</td><td>$2,836.84</td><td>$15,000.00</td><td>$14,278.95</td><td>$798.73</td></tr></table>

## Case 9.3

An analyst researching the company has come to the conclusion that the stock price after 20 days will not fall below $58 or raise above $66. All market parameters remain as in Case 9.2. From the point of view of the analyst, compare the expected return and risk for stock, options and a bull spread with strike prices $58 and $62. 

We shall build a simple model reflecting the analysts’s point of view. Addi tional information obtained by the analyst will result in modified probabilities as compared to the market probability P. (We assume, as before, that the market probability of up and down movements is $1 / 2$ in each step.) Namely, the probability $Q$ assigned by the analyst will be the market probability $P$ conditioned by the event $5 8 \leq S ( 2 0 ) \leq 6 2$ . In particular, 

$$
\begin{array}{l} Q (S (2 0) = x) = P (S (2 0) = x | 5 8 \leq S (2 0) \leq 6 2) \\ \qquad = \left\{ \begin{array}{c l} \frac {P (S (2 0) = x)}{P (5 8 \leq S (2 0) \leq 6 2)} & \text { if } 5 8 \leq x \leq 6 2, \\ 0 & \text { if } x <   5 0 \text { or } x > 6 2. \end{array} \right. \end{array}
$$

As a result, the analyst will arrive at the following values: 

1. Stock. Under the modified probability $Q$ 

$$
\mu_ {S} \cong 2. 6 7 8 8 \%, \quad \sigma_ {S} \cong 3. 9 2 5 7 \%.
$$

2. Call Options. Take a call with strike price $X ~ = ~ 5 8$ dollars. Hence $C ^ { \mathrm { E } } \cong 3 . 2 9 2 3$ dollars (this price is found in the binomial model without any restriction on the range of stock prices after 20 days). For an investment in options we find that 

$$
\mu_ {C} \cong 8. 8 8 1 6 \%, \quad \sigma_ {C} \cong 71. 0 9 5 \%.
$$

3. Bull Spread. Construct the spread by purchasing a call with strike $58 and selling a call with strike $60. The premium received for the latter is $2.10, hence a single spread costs $1.18. The expected return and risk are 

$$
\mu_ {\mathrm{bull}} \cong 38.4094\%, \quad \sigma_ {\mathrm{bull}} \cong 52.3997 \%.
$$

4. Bull Spread Combined with Risk-Free Asset. Investing 94.58% of the capital in the risk-free asset and the remainder in a bull spread, we can construct a portfolio P with the same expected return as stock, but lower risk, 

$$
\mu_ {P} \cong 2.6788\%, \quad \sigma_ {P} \cong 2.8396 \% .
$$

From the point of view of VaR, we consider the worst case scenario (among those admitted by the investor) when $S ( 2 0 ) \cong 5 8 . 5 9$ dollars, which may happen with conditional probability 0.2597. In this scenario each of the above investments will bring a loss, which can be regarded as VaR at 74.03% confidence level. The values of VaR and the market price of risk are collected below: 

<table><tr><td>Investment</td><td>Stock</td><td>Call options</td><td>Bull spread</td><td>Bull spread with risk-free asset</td></tr><tr><td>Market price of risk</td><td>0.5</td><td>0.1</td><td>0.7</td><td>0.7</td></tr><tr><td>VaR at 74.03%</td><td>$447</td><td>$12,426</td><td>$7,602</td><td>$412</td></tr></table>

The bull spread combined with risk-free will clearly be preferable to the other investments as it has the highest market price of risk and lowest VaR. 

## Exercise 9.10

Check the above computations and consider a modification such that the bull spread is constructed by buying a call with strike price $60 and selling a call with strike price $62. Compute the expected return, risk and VaR. 

## Exercise 9.11

Within the framework of the binomial model used above consider an analyst who has reasons to believe that the stock price will fall, but no more than 20% after 20 days. For a bear spread with strikes $56 and $58 constructed from put options compute the expected return, risk, and VaR for the worst possible outcome. 

# 10 Variable Interest Rates

This chapter begins with a model in which the interest rates implied by bonds do not depend on maturity. If the rates are deterministic, then they must be constant and the model turns out to be too simple to describe any real-life situation. In an extension allowing random changes of interest rates the problem of risk management will be dealt with by introducing a mathematical tool called the duration of bond investments. Finally, we shall show that maturitydependent rates cannot be deterministic either, preparing the motivation and notation for the next chapter, in which a model of stochastic rates will be explored. 

As in Chapter 2, $B ( t , T )$ will denote the price at time t (the running time) of a zero-coupon unit bond maturing at time $T$ (the maturity time). The dependence on two time variables gives rise to some dificulties in mathematical models of bond prices. These prices are exactly what is needed to describe the time value of money. In Chapter 2 we saw how bond prices imply the interest rate, under the assumption that the rate is constant. Here, we want to relax this restriction, allowing variable interest rates. 

In this chapter and the next one time will be discrete, though some parts of the theory can easily be extended to continuous time. We shall fix a time step $\tau$ , writing $t = \tau n$ for the running time and $T = \tau N$ for the maturity time. In the majority of examples we shall take either $\begin{array} { r } { \tau = \frac { 1 } { 1 2 } } \end{array}$ or $\tau = 1$ . The notation $B ( n , N )$ will be employed instead of $B ( t , T )$ for the price of a zero-coupon unit bond. We shall use continuous compounding, bearing in mind that it simplifies notation and makes it possible to handle time steps of any length consistently. 

## 10.1 Maturity-Independent Yields

The present value of a zero-coupon unit bond determines an interest rate called the yield and denoted by $y ( 0 )$ to emphasise the fact that it is computed at time 0: 

$$
B (0, N) = \mathrm{e} ^ {- N \tau y (0)}.
$$

For a diferent running time instant n such that $0 < n < N$ the implied yield may in general be diferent from $y ( 0 )$ . For each such n we thus have a number $y ( n )$ satisfying 

$$
B (n, N) = \mathrm{e} ^ {- (N - n) \tau y (n)}.
$$

Generally (and in most real cases), a bond with diferent maturity N will imply a diferent yield. Nevertheless, in this section we consider the simplified situation when $y ( n )$ is independent of N, that is, bonds with diferent maturities generate the same yield. Independence of maturity will be relaxed later in Section 10.2. 

## Proposition 10.1

If the yield $y ( n )$ for some $n > 0$ were known at time 0, then $y ( 0 ) = y ( n )$ or else an arbitrage strategy could be found. 

## Proof

Suppose that $y ( 0 ) < y ( n )$ . (We need to know not only $y ( 0 )$ but also $y ( n )$ at time 0 to decide whether or not this inequality holds.) 

Borrow a dollar for the period between 0 and $n + 1$ and deposit it for the period between 0 and n, both at the rate $y ( 0 )$ . (The yield can be regarded as the interest rate for deposits and loans.) 

At time n withdraw the deposit with interest, $ { \mathrm { e } } ^ { n \tau y ( 0 ) }$ in total, and invest this sum for a single time step at the rate $y ( n )$ . At time $n + 1$ this brings $\mathrm { e } ^ { n \tau y ( 0 ) + \tau y ( n ) }$ . The initial loan requires repayment of $\mathrm { e } ^ { ( n + 1 ) \tau y ( 0 ) }$ , leaving a positive balance $\mathrm { e } ^ { n \tau y ( 0 ) } ( \mathrm { e } ^ { \tau y ( n ) } - \mathrm { e } ^ { \tau y ( 0 ) } )$ , which is the arbitrage profit. 

The reverse inequality $y ( 0 ) > y ( n )$ can be dealt with in a similar manner. 

## Exercise 10.1

Let $\begin{array} { r } { \tau = \frac { 1 } { 1 2 } } \end{array}$ . Find arbitrage if the yields are independent of maturity, and unit bonds maturing at time 6 (half a year) are traded at $B ( 0 , 6 ) =$ 0.9320 dollars and $B ( 3 , 6 ) = 0 . 9 6 6 5$ dollars, both prices being known at time 0. 

As a consequence of Proposition 10.1, if the yield is independent of maturity and deterministic (that is, $y ( n )$ is known in advance for any $n \geq 0 )$ , then it must be constant, $y ( n ) = y$ for all n. This is the situation in Chapter 2, where all the bond prices were determined by a single interest rate. The yield $y ( n ) = y ,$ independent of n, is then equal to the constant risk-free interest rate denoted previously by r. 

Historical bond prices show a diferent picture: The yields implied by the bond prices recorded in the past clearly vary with time. In an arbitrage-free model, to admit yields varying with time but independent of maturity we should allow them to be random, so it is impossible to predict in advance whether $y ( n )$ will be higher or lower than $y ( 0 )$ 

We assume, therefore, that at each time instant the yield $y ( n )$ is a positive random number independent of the maturity of the underlying bond. 

Our goal is to analyse the return on a bond investment and the imminent risk arising from random changes of interest rates. Suppose that we intend to invest a certain sum of money P for a fixed period of N time steps. If the yield y remains constant, then, as observed in Chapter 2, our terminal wealth will be $P \mathrm { e } ^ { N \tau y }$ . This will be our benchmark for designing strategies hedged against unpredictable interest rate movements. 

## 10.1.1 Investment in Single Bonds

If we invest in zero-coupon bonds and keep them to maturity, the rate of return is guaranteed, since the final payment is fixed in advance and is not afected by any future changes of interest rates. However, if we choose to close out our investment prior to maturity by selling the bonds, we face the risk that the interest rates may change in the meantime with an adverse efect on the final value of the investment. 

## Example 10.1

Suppose we invest in bonds for a period of six months. Let $\textstyle \tau = { \frac { 1 } { 1 2 } }$ . We buy a number of unit bonds that will mature after one year, paying $B ( 0 , 1 2 ) = 0 . 9 3 0 0$ for each. This price implies a rate $y ( 0 ) \cong 7 . 2 6 \%$ . Since we are going to sell the bonds at time $n = 6$ , we are concerned with the price $B ( 6 , 1 2 )$ or, equivalently, with the corresponding rate $y ( 6 )$ . Let us discuss some possible scenarios: 

1. The rate is stable, $y ( 6 ) = 7 . 2 6 \%$ . The bond price is $B ( 6 , 1 2 ) \cong 0 . 9 6 4 4$ and the logarithmic return on the investment is 3.63%, a half of the interest rate, in line with the additivity of logarithmic returns. 

2. The rate decreases to $y ( 6 ) = 6 . 2 6 \%$ , say. (The convention is that 0.01% is one basis point, so here the rate drops by 100 basis points.) Then $B ( 6 , 1 2 ) \cong$ 0.9692, which is more than in scenario 1. As a result, we are going to earn more, achieving a logarithmic return of 4.13%. 

3. The rate increases to $y ( 6 ) = 8 . 2 6 \%$ . In this case the logarithmic return on our investment will be 3.13%, which is lower than in scenario 1, the bond price being $B ( 6 , 1 2 ) \cong 0 . 9 5 9 6$ 

We can see a pattern here: One is better of if the rate drops and worse of if the rate increases. A general formula for the return on this kind of investment is easy to find. 

Suppose that the initial yield $y ( 0 )$ changes randomly to become $y ( n ) \neq y ( 0 )$ at time n. Hence 

$$
B (0, N) = \mathrm{e} ^ {- y (0) \tau N}, \quad B (n, N) = \mathrm{e} ^ {- y (n) \tau (N - n)},
$$

and the return on an investment closed at time n will be 

$$
k (0, n) = \ln {\frac {B (n , N)}{B (0 , N)}} = \ln \mathrm{e} ^ {y (0) \tau N - y (n) \tau (N - n)} = y (0) \tau N - y (n) \tau (N - n).
$$

We can see that the return decreases as the rate $y ( n )$ increases. The impac of a rate change on the return depends on the timing. For example, if $\textstyle \tau = { \frac { 1 } { 1 2 } }$ ， $N = 1 2$ and $n = 6$ , then a rate increase of 120 basis points will reduce the return by 0.6% as compared to the case when the rate remains unchanged. 

## Exercise 10.2

Let $\begin{array} { r } { \tau { } = \frac { 1 } { 1 2 } } \end{array}$ . Invest $100 in six-month zero-coupon bonds trading at $B ( 0 , 6 ) = 0 . 9 4 0 0$ dollars. After six months reinvest the proceeds in bonds of the same kind, now trading at $B ( 6 , 1 2 ) = 0 . 9 3 6 8$ dollars. Find the implied interest rates and compute the number of bonds held at each time. Compute the logarithmic return on the investment over one year. 

## Exercise 10.3

Suppose that $B ( 0 , 1 2 ) = 0 . 8 7 0 0$ dollars. What is the interest rate after 6 months if an investment for 6 months in zero-coupon bonds gives a logarithmic return of 14% ? 

## Exercise 10.4

In this exercise we take a finer time scale with $\begin{array} { r } { \tau = \ \frac { 1 } { 3 6 0 } } \end{array}$ . (A year is assumed to have 360 days here.) Suppose that $B ( 0 , 3 6 0 ) = 0 . 9 2 0 0$ dollars, the rate remains unchanged for the first six months, goes up by 200 basis points on day 180, and remains at this level until the end of the year. If a bond is bought at the beginning of the year, on which day should it be sold to produce a logarithmic return of 4.88% or more? 

An investment in coupon bonds is more complicated. Even if the bond is kept to maturity, the coupons are paid in the meantime and can be reinvested. The return on such an investment depends on the interest rates prevailing at the times when the coupons are due. First consider the relatively simple case of an investment terminated as soon as the first coupon is paid. 

## Example 10.2

Let us invest the sum of $1, 000 in 4-year bonds with face value $100 and $10 annual coupons. A coupon bond of this kind can be regarded as a collection of four zero-coupon bonds maturing after 1, 2, 3 and 4 years with face value $10, $10, $10 and $110, respectively. Suppose that such coupon bonds trade at $91.78, which can be expressed as the sum of the prices of the four zero-coupon bonds, 

$$
9 1. 7 8 = 1 0 \mathrm{e} ^ {- y (0)} + 1 0 \mathrm{e} ^ {- 2 y (0)} + 1 0 \mathrm{e} ^ {- 3 y (0)} + 1 1 0 \mathrm{e} ^ {- 4 y (0)}.
$$

(The length of a time step is $\tau = 1 . )$ This equation can be solved to find the yield, $y ( 0 ) \cong 1 2 \%$ . We can aford to buy 10.896 coupon bonds. After one year we cash the coupons, collecting $108.96, and sell the bonds, which are now 3-year coupon bonds. Consider three scenarios: 

1. After one year the interest rate remains unchanged, $y ( 1 ) = 1 2 \%$ , the coupon bonds being valued at 

$$
1 0 \mathrm{e} ^ {- 0. 1 2} + 1 0 \mathrm{e} ^ {- 2 \times 0. 1 2} + 1 1 0 \mathrm{e} ^ {- 3 \times 0. 1 2} \cong 9 3. 4 8
$$

dollars, and we shall receive $1 0 8 . 9 6 + 1 , 0 1 8 . 5 2 \cong 1 , 1 2 7 . 4 8$ dollars in total. 

2. The rate drops to 10%. As a result, the coupon bonds will be worth 

$$
1 0 \mathrm{e} ^ {- 0. 1} + 1 0 \mathrm{e} ^ {- 2 \times 0. 1} + 1 1 0 \mathrm{e} ^ {- 3 \times 0. 1} \cong 9 8. 7 3
$$

dollars each. We shall end up with $1, 184.63. 

3. The rate goes up to 14%, the coupon bonds trading at $88.53. The final value of our investment will be $1, 073.51. 

## Exercise 10.5

Find the rate $y ( 1 )$ such that the logarithmic return on the investment in Example 10.2 will be a) 12%, b) 10%, c) 14%. 

If the lifetime of our investment exceeds one year, we will be facing the problem of reinvesting coupons. In the following example we assume that the coupons are used to purchase the same bond. 

## Example 10.3

We begin as in Example 10.2, but our intention is to terminate the investment after 3 years. After one year we reinvest the coupons obtained in the same, now a 3-year, coupon bond. Consider the following scenarios after one year: 

1. The rate remains the same for the period of our investment, $y ( 0 ) = y ( 1 ) =$ $y ( 2 ) = y ( 3 ) = 1 2 \%$ . The bond price is $93.48, so for the $108.96 received from coupons we can buy 1.17 additional bonds, increasing the number of bonds held to 12.06. We can monitor the value of our investment by simply multiplying the number of bonds held by the current bond price. We repeat this in the following year. After three years we cash the coupons and sell the bonds, the final value of the investment being $1, 433.33. This number will be used as a benchmark for other scenarios. Observe that 

$$
1, 4 3 3. 3 3 \cong 1, 0 0 0 \mathrm{e} ^ {3 \times 12\%},
$$

the same as the value after 3 years of $1, 000 invested on zero-coupon bonds. The building blocks of our investment are summarised in the table below. 

<table><tr><td>Year</td><td>0</td><td>1</td><td>2</td><td>3</td></tr><tr><td>Rate</td><td>12%</td><td>12%</td><td>12%</td><td>12%</td></tr><tr><td>PV of coupon 1</td><td>$8.87</td><td>$10.00</td><td></td><td></td></tr><tr><td>PV of coupon 2</td><td>$7.87</td><td>$8.87</td><td>$10.00</td><td></td></tr><tr><td>PV of coupon 3</td><td>$6.98</td><td>$7.87</td><td>$8.87</td><td>$10.00</td></tr><tr><td>PV of coupon 4</td><td>$6.19</td><td>$6.98</td><td>$7.87</td><td>$8.87</td></tr><tr><td>PV of face value</td><td>$61.88</td><td>$69.77</td><td>$78.66</td><td>$88.69</td></tr><tr><td>Bond price</td><td>$91.78</td><td>$93.48</td><td>$95.40</td><td>$97.56</td></tr><tr><td>Cashed coupons</td><td></td><td>$108.96</td><td>$120.60</td><td>$133.26</td></tr><tr><td>Additional bonds</td><td></td><td>1.17</td><td>1.26</td><td></td></tr><tr><td>Number of bonds</td><td>10.90</td><td>12.06</td><td>13.33</td><td></td></tr><tr><td>Value of investment</td><td>$1,000.00</td><td>$1,127.50</td><td>$1,271.25</td><td>$1,433.33</td></tr></table>

2. Suppose that the rate goes down by 2% after one year and then remains at the new level. The drop of the rate results in an increase of all bond prices. The number of additional bonds that can be bought for the coupons is lower than in scenario 1. Nevertheless, the final value of the investment is 


higher because so is the price at which we sell the bonds after three years.


<table><tr><td>Year</td><td>0</td><td>1</td><td>2</td><td>3</td></tr><tr><td>Rate</td><td>12%</td><td>10%</td><td>10%</td><td>10%</td></tr><tr><td>PV of coupon 1</td><td>$8.87</td><td>$10.00</td><td></td><td></td></tr><tr><td>PV of coupon 2</td><td>$7.87</td><td>$9.05</td><td>$10.00</td><td></td></tr><tr><td>PV of coupon 3</td><td>$6.98</td><td>$8.19</td><td>$9.05</td><td>$10.00</td></tr><tr><td>PV of coupon 4</td><td>$6.19</td><td>$7.41</td><td>$8.19</td><td>$9.05</td></tr><tr><td>PV of face value</td><td>$61.88</td><td>$74.08</td><td>$81.87</td><td>$90.48</td></tr><tr><td>Bond price</td><td>$91.78</td><td>$98.73</td><td>$99.11</td><td>$99.53</td></tr><tr><td>Cashed coupons</td><td></td><td>$108.96</td><td>$119.99</td><td>$132.10</td></tr><tr><td>Additional bonds</td><td></td><td>1.10</td><td>1.21</td><td></td></tr><tr><td>Number of bonds</td><td>10.90</td><td>12.00</td><td>13.21</td><td></td></tr><tr><td>Value of investment</td><td>$1,000.00</td><td>$1,184.65</td><td>$1,309.25</td><td>$1,446.94</td></tr></table>


3. If the rate increases to 14% and stays there, the bonds will be cheaper than in Scenario 1. The final value of the investment will be disappointing.


<table><tr><td>Year</td><td>0</td><td>1</td><td>2</td><td>3</td></tr><tr><td>Rate</td><td>12%</td><td>14%</td><td>14%</td><td>14%</td></tr><tr><td>PV of coupon 1</td><td>$8.87</td><td>$10.00</td><td></td><td></td></tr><tr><td>PV of coupon 2</td><td>$7.87</td><td>$8.69</td><td>$10.00</td><td></td></tr><tr><td>PV of coupon 3</td><td>$6.98</td><td>$7.56</td><td>$8.69</td><td>$10.00</td></tr><tr><td>PV of coupon 4</td><td>$6.19</td><td>$6.57</td><td>$7.56</td><td>$8.69</td></tr><tr><td>PV of face value</td><td>$61.88</td><td>$65.70</td><td>$75.58</td><td>$86.94</td></tr><tr><td>Bond price</td><td>$91.78</td><td>$88.53</td><td>$91.83</td><td>$95.63</td></tr><tr><td>Cashed coupons</td><td></td><td>$108.96</td><td>$121.26</td><td>$134.46</td></tr><tr><td>Additional bonds</td><td></td><td>1.23</td><td>1.32</td><td></td></tr><tr><td>Number of bonds</td><td>10.90</td><td>12.13</td><td>13.45</td><td></td></tr><tr><td>Value of investment</td><td>$1,000.00</td><td>$1,073.53</td><td>$1,234.85</td><td>$1,420.41</td></tr></table>


As a motivation for certain theoretical notions, consider the above investment, with the same possible scenarios, but involving a specially designed security, a coupon bond with annual coupons paying $32, all other parameters remaining unchanged. The results are as follows:


<table><tr><td>Scenario</td><td>Value after 3 years</td></tr><tr><td>12%, 12%, 12%, 12%</td><td>$1,433.33</td></tr><tr><td>12%, 10%, 10%, 10%</td><td>$1,433.68</td></tr><tr><td>12%, 14%, 14%, 14%</td><td>$1,433.78</td></tr></table>

It is remarkable that any change in interest rates improves the result of our investment. We do not lose if the rates change unfavourably. On the other hand, we do not gain in other circumstances. This is explained by the fact, that a certain parameter of the bond, called duration and defined below, is exactly equal to the lifetime of our investment. In some sense, the bond behaves approximately like a zero-coupon bond with prescribed maturity. 

Exercise 10.6 

Check the numbers given in the above tables. 

Exercise 10.7 

Compute the value after three years of $1, 000 invested in a 4-year bond with $32 annual coupons and $100 face value if the rates in consecutive years are as follows: 

Scenario 1: 12%, 11%, 12%, 12%; 

Scenario 2: 12%, 13%, 12%, 12%. 

Design a spreadsheet and experiment with various interest rates. 

## 10.1.2 Duration

We have seen that variable interest leads to uncertainty as to the future value of an investment in bonds. This may be undesirable, or even unacceptable, for example for a pension fund manager. We shall introduce a tool which makes it possible to immunise such an investment, at least in the special situation of maturity-independent rates considered in this section. 

For notational simplicity we denote the current yield $y ( 0 )$ by y. Consider a coupon bond with coupons $C _ { 1 } , C _ { 2 } , \dots , C _ { N }$ payable at times $0 < \tau n _ { 1 } < \tau n _ { 2 } <$ $\dots < \tau n _ { N }$ and face value F, maturing at time $\tau n _ { N }$ . Its current price is given by 

$$
P (y) = C _ {1} \mathrm{e} ^ {- \tau n _ {1} y} + C _ {2} \mathrm{e} ^ {- \tau n _ {2} y} + \dots + (C _ {N} + F) \mathrm{e} ^ {- \tau n _ {N} y}.\tag{10.1}
$$

The duration of the coupon bond is defined to be 

$$
D (y) = \frac {\tau n _ {1} C _ {1} \mathrm{e} ^ {- \tau n _ {1} y} + \tau n _ {2} C _ {2} \mathrm{e} ^ {- \tau n _ {2} y} + \cdots + \tau n _ {N} (C _ {N} + F) \mathrm{e} ^ {- \tau n _ {N} y}}{P (y)}.\tag{10.2}
$$

The numbers $C _ { 1 } \mathrm { e } ^ { - \tau n _ { 1 } y } / P ( y ) , C _ { 2 } \mathrm { e } ^ { - \tau n _ { 2 } y } / P ( y ) , \ldots , ( C _ { N } + F ) \mathrm { e } ^ { - \tau n _ { N } y } / P ( y )$ are non-negative and add up to one, so they may be regarded as weights or probabilities. It can be said that the duration is a weighted average of future payment times. The duration of any future cash flow can be defined in a similar manner. 

Duration measures the sensitivity of the bond price to changes in the interest rate. To see this we compute the derivative of the bond price with respect to y, 

$$
\frac {\mathrm{d}}{\mathrm{d} y} P (y) = - \tau n _ {1} C _ {1} \mathrm{e} ^ {- \tau n _ {1} y} - \tau n _ {2} C _ {2} \mathrm{e} ^ {- \tau n _ {2} y} - \dots - \tau n _ {N} (C _ {N} + F) \mathrm{e} ^ {- \tau n _ {N} y},
$$

which gives 

$$
\frac {\mathrm{d}}{\mathrm{d} y} P (y) = - D (y) P (y).
$$

The last formula is sometimes taken as the definition of duration. 

## Example 10.4

A 6-year bond with $10 annual coupons, $100 face value and yield of 6% has a duration of 4.898 years. A 6-year bond with the same coupons and yield, but with $500 face value, will have a duration of 5.671 years. The duration of any zero-coupon bond is equal to its lifetime. 

## Exercise 10.8

A 2-year bond with $100 face value pays a $6 coupon each quarter and has 11% yield. Compute the duration. 

## Exercise 10.9

What should be the face value of a 5-year bond with 10% yield, paying $10 annual coupons to have duration 4? Find the range of durations that can be obtained by altering the face value, as long as a coupon cannot exceed the face value. If the face value is fixed, say $100, find the level of coupons for the duration to be 4. What durations can be manufactured in this way? 

## Exercise 10.10

Show that P is a convex function of $y .$ 

If we invest in a bond with the intention to close the investment at time $t ,$ then the future value of the money invested in a single bond will be $P ( y ) \mathrm { e } ^ { t y }$ provided that the interest rate remains unchanged (being equal to the initial yield $y ( 0 ) )$ . To see how sensitive this amount is to interest rate changes compute the derivative with respect to y, 

$$
\frac {\mathrm{d}}{\mathrm{d} y} (P (y) \mathrm{e} ^ {t y}) = \left(\frac {\mathrm{d}}{\mathrm{d} y} P (y)\right) \mathrm{e} ^ {t y} + t P (y) \mathrm{e} ^ {t y} = (t - D (y)) P (y) \mathrm{e} ^ {t y}.
$$

If the duration of the bond is exactly t, then 

$$
\frac {\mathrm{d}}{\mathrm{d} y} (P (y) \mathrm{e} ^ {t y}) = 0.
$$

If the derivative is zero at some point, then the graph of the function is ‘flat near this point. This means that small changes of the rate will have little efect on the future value of the investment. 

## 10.1.3 Portfolios of Bonds

If a bond of desirable duration is not available, it may be possible to create a synthetic one by investing in a suitable portfolio of bonds of diferent durations. 

## Example 10.5

If the initial interest rate is 14%, then a 4-year bond with annual coupons $C = 1 0$ and face value $F = 1 0 0$ has duration 3.44 years. A zero-coupon bond with $F = 1 0 0$ and N = 1 has duration 1. A portfolio consisting of two bonds, one of each kind, can be regarded as a single bond with coupons $C _ { 1 } = 1 1 0$ $C _ { 2 } = C _ { 3 } = C _ { 4 } = 1 0 , F = 1 0 0$ . Its duration can be computed using the general formula (10.2), which gives 2.21 years. 

We shall derive a formula for the duration of a portfolio in terms of the durations of its components. Denote by $P _ { A } ( y )$ and $P _ { B } ( y )$ the values of two bonds A and B with durations $D _ { A } ( y )$ and $D _ { B } ( y )$ . Take a portfolio consisting of a bonds A and b bonds B, its value being a $P _ { A } ( y ) + b P _ { B } ( y )$ . The task of finding the duration of the portfolio will be divided into two steps: 

1. Find the duration of a portfolio consisting of a bonds of type A. We shall write aA to denote such a portfolio. Its price is obviously a $P _ { A } ( y )$ . Since 

$$
\frac {\mathrm{d}}{\mathrm{d} y} (a P _ {A} (y)) = - D _ {A} (y) (a P _ {A} (y)),
$$

it follows that 

$$
D _ {a A} (y) = D _ {A} (y).
$$

This is clear if we examine the cash flow of aA. Each coupon and the face value are multiplied by a, which cancels out in the computation of duration directly from (10.2). 

2. Find the duration of a portfolio consisting of one bond A and one bond B, which will be denoted by $A + B$ . The price of this portfolio is $P _ { A } ( y ) + P _ { B } ( y )$ 

Diferentiating the last expression, we obtain 

$$
\begin{array}{c} \frac {\mathrm{d}}{\mathrm{d} y} (P _ {A} (y) + P _ {B} (y)) = \frac {\mathrm{d}}{\mathrm{d} y} P _ {A} (y) + \frac {\mathrm{d}}{\mathrm{d} y} P _ {B} (y) \\ = - D _ {A} (y) P _ {A} (y) - D _ {B} (y) P _ {B} (y). \end{array}
$$

The last term can be written as $- D _ { A + B } ( y ) ( P _ { A } ( y ) + P _ { B } ( y ) )$ if we put 

$$
D _ {A + B} (y) = D _ {A} (y) \frac {P _ {A} (y)}{P _ {A} (y) + P _ {B} (y)} + D _ {B} (y) \frac {P _ {B} (y)}{P _ {A} (y) + P _ {B} (y)}.
$$

This means that $D _ { A + B } ( y )$ is a linear combination of $D _ { A } ( y )$ and $D _ { B } ( y )$ , the coeficients being the percentage weights of each bond in the portfolio. 

From the above considerations we obtain the general formula 

$$
D _ {a A + b B} (y) = D _ {A} (y) w _ {A} + D _ {B} (y) w _ {B},
$$

where 

$$
w _ {A} = \frac {a P _ {A} (y)}{a P _ {A} (y) + b P _ {B} (y)}, \quad w _ {B} = \frac {b P _ {A} (y)}{a P _ {A} (y) + b P _ {B} (y)},
$$

are the percentage weights of individual bonds. 

If we allow negative values of a or b (which corresponds to writing a bond instead of purchasing it, in other words, to borrowing money instead of investing), then, given two durations $D _ { A } \neq D _ { B }$ , the duration D of the portfolio can take any value because $\boldsymbol { w } _ { B } = 1 - \boldsymbol { w } _ { A }$ and 

$$
D = D _ {A} w _ {A} + D _ {B} (1 - w _ {A}) = D _ {B} + w _ {A} (D _ {A} - D _ {B}).
$$

The value of D can even be negative, which corresponds to a negative cash flow, that is, sums of money to be paid rather than received. 

## Example 10.6

Let $D _ { A } = 1$ and $D _ { B } = 3$ . We wish to invest $1, 000 for 6 months. For the duration to match the lifetime of the investment we need $0 . 5 = w _ { A } + 3 w _ { B }$ . Since $w _ { A } + w _ { B } = 1$ , it follows that $w _ { B } = - 0 . 2 5$ and $w _ { A } = 1 . 2 5$ . With $P _ { A } = 0 . 9 2$ dollars and $P _ { B } = 1 . 0 1$ dollars, we invest $1, 250 in $\textstyle \frac { 1 2 5 0 } { 0 . 9 2 } \cong 1 , 3 5 8 . 7 0$ bonds A and we issue $\textstyle { \frac { 2 5 0 } { 1 . 0 1 } } \cong 2 4 7 . 5 2$ bonds B. 

## Exercise 10.11

Find the number of bonds of type A and B to be bought if $D _ { A } = 2 \quad$ , $D _ { B } = 3 . 4 , P _ { A } = 0 . 9 8 , P _ { B } = 1 . 0 2$ and you need a portfolio worth $5, 000 with duration 6. 

## Exercise 10.12

Invest $1, 000 in a portfolio of bonds with duration 2 using 1-year zerocoupon bonds with $100 face value and 4-year bonds with $15 annual coupons and $100 face value that trade at $102. 

A portfolio with duration matching the investment lifetime is insensitive to small changes of interest rates. However in practice we shall have to modify the portfolio if, for example, the investment is for 3 years and one of the bonds is a zero-coupon bond expiring after one year. In addition, the duration may, as we shall see below, go of the target. As a result, it will become necessary to update the portfolio during the lifetime of the investment. This is the subject of the next subsection. 

## 10.1.4 Dynamic Hedging

Even if a portfolio is selected with duration matching the desired investment lifetime, this will only be valid at the initial instant, since duration changes with time as well as with the interest rate. 

## Example 10.7

Take a 5-year bond with $10 annual coupons and $100 face value. If $y = 1 0 \%$ then the duration will be about 4.16 years. Before the first coupon is paid the duration decreases in line with time: After 6 months it will be 3.66, and after 9 months 4.16 0.75 = 3.31. If the duration matches our investment’s lifetime and the interest rates do not change, no action will be necessary until a coupon becomes payable. As soon as the first coupon is paid after one year, the bond will become a 4-year one with duration 3.48, no longer consistent with the investment lifetime. 

## Exercise 10.13

Assuming that the interest rate does not change, show that before the first coupon is paid the duration after time t will D t, where D is the duration computed at time 0. 

The next example shows the impact of the interest rate on duration. 

## Example 10.8

The bond in Example 10.7 will have duration 4.23 if $y \ : = \ : 6 \%$ , and 4.08 if $y = 1 4 \%$ 

## Exercise 10.14

Show that the duration of a 2-year bond with annual coupons decreases as the yield increases. 

Duration will now be applied to design an investment strategy immune to interest rate changes. This will be done by monitoring the position at the end of each year, or more frequently if needed. For clarity of exposition we restrict ourselves to an example. 

Set the lifetime of the investment to be 3 years and the target value to be $100, 000. Suppose that the interest rate is 12% initially. We invest $69, 767.63, which would be the present value of $100, 000 if the interest rate remained constant. 

We restrict our attention to two instruments, a 5-year bond A with $10 annual coupons and $100 face value, and a 1-year zero-coupon bond B with the same face value. We assume that a new bond of type B is always available. In subsequent years we shall combine it with bond A. 

At time 0 the bond prices are $90.27 and $88.69, respectively. We find $D _ { A } \cong 4 . 1 2$ and the weights $w _ { A } \cong 0 . 6 4 0 5 , w _ { B } \cong 0 . 3 5 9 5$ which give a portfolio with duration 3. We split the initial sum according to the weights, spending $44, 687.93 to buy $a \cong 4 9 5 . 0 5$ bonds A and $25, 079.70 to buy $b \cong 2 8 2 . 7 7$ bonds B. Consider some possible scenarios of future interest rate changes. 

1. After one year the rate increases to 14%. The value of our portfolio is the sum of: 

the first coupons of bonds A: $4, 950.51, 

the face value of cashed bonds B: $28, 277.29, 

the market value of bonds A held, which are now 4-year bonds selling at $85.65: $42, 403.53. 

This gives $75, 631.32 altogether. The duration of bonds A is now 3.44. The desired duration is 2, so we find $w _ { A } \cong 0 . 4 0 9 4$ and $w _ { B } \cong 0 . 5 9 0 6$ and arrive at the number of bonds to be held in the portfolio: 361.53 bonds A and 513.76 bonds B. (This means that we have to sell 133.52 bonds A and buy 513.76 new bonds B.) 

a) After two years the rate drops to 9%. To compute our wealth we add: 

the coupons of A: $3, 615.30, 

the face values of B: $51, 376.39, 

the market value of A, selling at $101.46: $36, 682.22. 

The result is $91, 673.92. We invest all the money in bonds B, since the required duration is now 1. (The payof of these bonds is guaranteed next year.) We can aford to buy 1, 003.07 bonds B selling at $91.39. The terminal value of the investment will be about $100,307. 

b) After two years the rate goes up to 16%. We cash the same amount as above for coupons and zero-coupon bonds, but bonds A are now cheaper, selling at $83.85, so we have less money in total: $85, 305.68. However, the zero-coupon bonds are now cheap as well, selling at $85.21, and we can aford to buy 1, 001.07 of them, ending up with $100,107. 

2. After one year the rate drops to 9%. In a similar way as before, we arrive at the current value of the investment by adding the coupons of A, the face value of B and the market value of bonds A held, obtaining $83, 658.73. Then we find the weights $w _ { A } \cong 0 . 4 0 1 3 , w _ { B } \cong 0 . 5 9 8 7$ , determining our new portfolio of 329.56 bonds A and 548.04 bonds B. (We have to sell 165.50 bonds A and buy 548.04 new bonds B.) 

a) After two years the rate goes up to 14%. We cash $3, 295.55 from the coupons of A, which together with the $54, 803.77 obtained from B and the market value of $29, 174.39 of bonds A gives $87, 273.72 in total. We buy 1003.89 new zero-coupon bonds B, ending up with $100,389 after 3 years. 

b) After two years the rate drops to 6%. Our wealth will then be $94, 405.29, we can aford to buy 1, 002.43 bonds B, and the final value of our in vestment will be $100,243. 

As we can see, we end up with more than $100, 000 in each scenario.<sup>1</sup> 

## Exercise 10.15

Design an investment of $20, 000 in a portfolio of duration 2 years consisting of two kinds of coupon bonds maturing after 2 years, with annual coupons, bond A with $20 coupons and $100 face value, and bond B with $5 coupons and $500 face value, given that the initial rate is 8%. How much will this investment be worth after 2 years? 

## 10.2 General Term Structure

Here we shall discuss a model of bond prices without the condition that the yield should be independent of maturity. 

The prices $B ( n , N )$ of zero-coupon unit bonds with various maturities determine a family of yields $y ( n , N )$ by 

$$
B (n, N) = \mathrm{e} ^ {- (N - n) \tau y (n, N)}.
$$

Note that the yields have to be positive, since $B ( n , N )$ has to be less than 1 for $n < N$ . The function $y ( n , N )$ of two variables $n < N$ is called the term structure of interest rates. The yields $y ( 0 , N )$ dictated by the current prices are called the spot rates. 

The initial term structure $y ( 0 , N )$ formed by the spot rates is a function of one variable N. Typically, it is an increasing function, but other graphs have also been observed in financial markets. In particular, the initial term structure may be $f l a t$ , that is, the yields may be independent of N, which is the case considered in the previous section. 

$$
E x e r c i s e 1 0. 1 6
$$

If $B ( 0 , 6 ) = 0 . 9 6$ dollars, find $B ( 0 , 3 )$ and $B ( 0 , 9 )$ such that the initia term structure is flat. 

The price of a coupon bond as the present value of future payments can be written using the spot rates in the following way: 

$$
P = C _ {1} \mathrm{e} ^ {- \tau n _ {1} y (0, n _ {1})} + C _ {2} \mathrm{e} ^ {- \tau n _ {2} y (0, n _ {2})} + \dots + (C _ {N} + F) \mathrm{e} ^ {- \tau n _ {N} y (0, n _ {N})}\tag{10.3}
$$

for a bond with coupons $C _ { 1 } , C _ { 2 } , \dots , C _ { N }$ due at times $0 < \tau n _ { 1 } < \tau n _ { 2 } < \cdot \cdot \cdot <$ $\tau n _ { N }$ and with face value F, maturing at time $\tau n _ { N }$ 

Despite the fact that for a coupon bond we cannot use a single rate for discounting future payments, such a rate can be introduced just as an artificial quantity. It is called the yield to maturity, and is defined to be the number y solving the equation 

$$
P = C _ {1} \mathrm{e} ^ {- \tau n _ {1} y} + C _ {2} \mathrm{e} ^ {- \tau n _ {2} y} + \dots + (F + C _ {N}) \mathrm{e} ^ {- \tau n _ {N} y}.
$$

Yield to maturity provides a convenient simple description of coupon bonds and is quoted in the financial press. Of course, if the interest rates are independent of maturity, then this formula is the same as (10.1). 

## Remark 10.1

To determine the initial term structure we need the prices of zero-coupon bonds. However, for longer maturities (typically over one year) only coupon bonds may be traded, making it necessary to decompose coupon bonds into zero-coupon bonds with various maturities. This can be done by applying formula (10.3) repeatedly to find the yield with the longest maturity, given the bond price and all the yields with shorter maturities. This procedure was recognised by the U.S. Treasury, who in 1985 introduced a programme called STRIPS (Separate Trading of Registered Interest and Principal Securities), allowing an investor to keep the required cash payments (for certain bonds) by selling the rest (the ‘stripped’ bond) back to the Treasury. 

## Example 10.9

Suppose that a one-year zero-coupon bond with face value $100 is trading at $91.80 and a two-year bond with $10 annual coupons and face value $100 is trading at $103.95. This gives the following equations for the yields 

$$
\begin{array}{c} {9 1. 8 0 = 1 0 0 \mathrm{e} ^ {- y (0, 1)},} \\ {1 0 3. 9 5 = 1 0 \mathrm{e} ^ {- y (0, 1)} + 1 1 0 \mathrm{e} ^ {- 2 y (0, 2)}.} \end{array}
$$

From the first equation we obtain $y ( 0 , 1 ) \cong 8 . 5 6 \%$ . On substituting this into the second equation, we find $y ( 0 , 2 ) \cong 7 . 4 5 \%$ . As a result, the price of the ‘stripped’ two-year bond, a zero-coupon bond maturing in two years with face value $100, will be $1 0 0 \mathrm { e } ^ { - 2 y ( 0 , 2 ) } \cong 8 6 . 1 6$ dollars. Given the price of a three-year coupon bond, we could then evaluate $y ( 0 , 3 )$ , and so on. 

Going back to our general study of bonds, let us consider a deterministic term structure (thus known in advance with certainty). The next proposition indicates that this, in fact, is not realistic. 

## Proposition 10.2

If the term structure is deterministic, then the No-Arbitrage Principle implies that 

$$
B (0, N) = B (0, n) B (n, N).\tag{10.4}
$$

Proof 

If $B ( 0 , N ) < B ( 0 , n ) B ( n , N )$ , then: 

Buy a bond maturing at time N and write a fraction $B ( n , N )$ of a bond maturing at n. (Here we use the assumption that the future bond prices are known today.) This gives $B ( 0 , n ) B ( n , N ) - B ( 0 , N )$ dollars now. 

At time n settle the written bonds, raising the required sum of $B ( n , N )$ by issuing a single unit bond maturing at N. 

At time N close the position, retaining the initial profit. 

The reverse inequality $B ( 0 , N ) > B ( 0 , n ) B ( n , N )$ can be dealt with in a similar manner, by adopting the opposite strategy. □ 

Employing the representation of bond prices in terms of yields, we have 

$$
B (n, N) = \frac {B (0 , N)}{B (0 , n)} = \mathrm{e} ^ {\tau n y (0, n) - \tau N y (0, N)}.
$$

This would mean that all bonds prices (and so the whole term structure) are determined by the initial term structure. However, it is clear that one cannot expect this to hold in real bond markets. In particular, this relation is not supported by historical data. 

This shows that assuming deterministic bond prices would go too far in reducing the complexity of the model. We have no choice but to allow the future term structure to be random, only the initial term structure being known with certainty. In what follows, future bond prices will be random, as will be the quantities determined by them. 

## 10.2.1 Forward Rates

We begin with an example showing how to secure in advance the interest rate for a deposit to be made or a loan to be taken at some future time. 

## Example 10.10

Suppose that the business plan of your company will require taking a loan of $100, 000 one year from now in order to purchase new equipment. You expect to have the means to repay the loan after another year. You would like to arrange the loan today at a fixed interest rate, rather than to gamble on future rates. Suppose that the spot rates are $y ( 0 , 1 ) = 8 \%$ and $y ( 0 , 2 ) = 9 \% \ ( \mathrm { w i t h } \ \tau = 1 )$ You buy 1, 000 one-year bonds with $100 face value, paying $1 0 0 , 0 0 0 \mathrm { e } ^ { - 8 \% } \cong$ 92, 311.63 dollars. This sum is borrowed for 2 years at 9%. After one year you will receive the $100, 000 from the bonds, and after two years you can settle the loan with interest, the total amount to pay being 92, $3 1 1 . 6 3 \mathrm { e } ^ { 2 \times 9 \% } \cong$ 110, 517.09 dollars. Thus, the interest rate on the constructed future loan will be ln $( 1 1 0 , 5 1 7 . 0 9 / 1 0 0 , 0 0 0 ) \cong 1 0 \%$ . Financial intermediaries may simplify your task by ofering a so-called Forward Rate Agreement and perform the above construction of the loan on your behalf. 

## Exercise 10.17

Explain how a deposit of $50, 000 for six months can be arranged to start in six months and find the rate if $y ( 0 , 6 ) = 6 \%$ and $y ( 0 , 1 2 ) = 7 \%$ , where $\textstyle \tau = { \frac { 1 } { 1 2 } }$ 

In general, the initial forward rate $f ( 0 , M , N )$ is an interest rate such that 

$$
B (0, N) = B (0, M) \mathrm{e} ^ {- (N - M) \tau f (0, M, N)},
$$

so 

$$
f (0, M, N) = - \frac {1}{\tau (N - M)} \ln \frac {B (0 , N)}{B (0 , M)} = - \frac {\ln B (0 , N) - \ln B (0 , M)}{\tau (N - M)}.
$$

Note that this rate is deterministic, since it is worked out using the present bond prices. It can be conveniently expressed in terms of the initial term structure. Insert into the above expression the bond prices as determined by the yields, $B ( 0 , N ) = \mathrm { e } ^ { - \tau N y ( 0 , N ) }$ and $B ( 0 , M ) = \mathrm { e } ^ { - \tau M y ( 0 , M ) }$ , to get 

$$
f (0, M, N) = \frac {N y (0 , N) - M y (0 , M)}{N - M}.\tag{10.5}
$$

## Exercise 10.18

Suppose that the following spot rates are provided by central London banks (LIBOR, the London Interbank Ofer Rate, is the rate at which money can be deposited; LIBID, the London Interbank Bid Rate, is the rate at which money can be borrowed): 

<table><tr><td>Rate</td><td>LIBOR</td><td>LIBID</td></tr><tr><td>1 month</td><td>8.41%</td><td>8.59%</td></tr><tr><td>2 months</td><td>8.44%</td><td>8.64%</td></tr><tr><td>3 months</td><td>9.01%</td><td>9.23%</td></tr><tr><td>6 months</td><td>9.35%</td><td>9.54%</td></tr></table>

As a bank manager acting for a customer who wishes to arrange a loan of $100, 000 in a month’s time for a period of 5 months, what rate could you ofer and how would you construct the loan? Suppose that another institution ofers the possibility of making a deposit for 4 months, starting 2 months from now, at a rate of 10.23%. Does this present an arbitrage opportunity? All rates stated in this exercise are continuous compounding rates. 

As time passes, the bond prices will change and, consequently, so will the forward rates. The forward rate over the interval [M, N] determined at time $n < M < N$ is defined by 

$$
B (n, N) = B (n, M) \mathrm{e} ^ {- (N - M) \tau f (n, M, N)},
$$

that is, 

$$
f (n, M, N) = - \frac {\ln B (n , N) - \ln B (n , M)}{(N - M) \tau}.
$$

The instantaneous forward rates $f ( n , N ) = f ( n , N , N + 1 )$ are the forward rates over a one-step interval. Typically, when τ is one day, the instantaneous forward rates correspond to overnight deposits or loans. The formula for the forward rate 

$$
f (n, N) = - \frac {\ln B (n , N + 1) - \ln B (n , N)}{\tau}\tag{10.6}
$$

will enable us to reconstruct the bond prices, given the forward rates at a particular time n. 

## Example 10.11

Let $\tau = { \textstyle { \frac { 1 } { 1 2 } } } , n = 0 , N = 0 , 1 , 2 , 3$ , and suppose that the bond prices are 

$$
\begin{array}{l} B (0, 1) = 0. 9 9 0 1, \\ B (0, 2) = 0. 9 8 2 8, \\ B (0, 3) = 0. 9 7 2 6. \end{array}
$$

Then we have the following implied yields 

$$
\begin{array}{l}y(0,1)\cong 11.94\% ,\\ y(0,2)\cong 10.41\% ,\\ y(0,3)\cong 11.11\% , \end{array}
$$

and forward rates 

$$
\begin{array}{l}f(0,0)\cong 11.94\% ,\\ f(0,1)\cong \quad 8.88\% ,\\ f(0,2)\cong 12.52\% . \end{array}
$$

Observe that, using the formula for the forward rates, we get 

$$
\exp \left(- (0. 1 1 9 4 + 0. 0 8 8 8 + 0. 1 2 5 2) / 1 2\right) \cong 0. 9 7 2 6 = B (0, 3)
$$

which illustrates the next proposition. 

## Proposition 10.3

The bond price is given by 

$$
B (n, N) = \exp \{- \tau (f (n, n) + f (n, n + 1) + \dots + f (n, N - 1)) \}.
$$

Proof 

For this purpose note that 

$$
f (n, n) = - \frac {\ln B (n , n + 1)}{\tau},
$$

since $B ( n , n ) = 1$ , so 

$$
B (n, n + 1) = \exp \{- \tau f (n, n) \}.
$$

Next, 

$$
f (n, n + 1) = - \frac {\ln B (n , n + 2) - \ln B (n , n + 1)}{\tau}
$$

and, after inserting the expression for $B ( n , n + 1 )$ ， 

$$
B (n, n + 2) = \exp \{- \tau (f (n, n) + f (n, n + 1)) \}.
$$

Repeating this a number of times, we arrive at the required general formula. 

We have a simple representation of the forward rates in terms of the yields: 

$$
f (n, N) = (N + 1 - n) y (n, N + 1) - (N - n) y (n, N).\tag{10.7}
$$

In particular, 

$$
f (n, n) = y (n, n + 1),
$$

resulting in the intuitive formula 

$$
y (n, N) = \frac {f (n , n) + f (n , n + 1) + \cdots + f (n , N - 1)}{N - n}.
$$

## Example 10.12

We can clearly see from the above formulae that if the term structure is flat, that is, $y ( n , N )$ is independent of N, then $f ( n , N ) = y ( n , N )$ . Now consider an example of $f ( n , N )$ increasing with N for a fixed n, and compute the corresponding yields 

$$
f (0, 0) = 8.01\%, \quad y (0, 1) = 8.01\% ,
$$

$$
f (0, 1) = 8.03\%, \quad y (0, 2) = 8.02\% ,
$$

$$
f (0, 2) = 8. 0 8 \%, y (0, 3) = 8. 0 4 \%.
$$

We can see that the yields also increase. (See Exercise 10.20 below for a generalisation of this.) 

However, the forward rates do not have to increase with maturity even if the yields do: 

$$
f (0, 0) = 9.20\%, \quad y (0, 1) = 9.20\% ,
$$

$$
f (0, 1) = 9.80\%, \quad y (0, 2) = 9.50\%,
$$

$$
f (0, 2) = 9.56\%, \quad y (0, 3) \cong 9.52\% .
$$

Exercise 10.19 

Can a forward rate be negative? 

Exercise 10.20 

Prove that if $f ( n , N )$ increases with N, then the same is true for $y ( n , N )$ 

## 10.2.2 Money Market Account

The short rate is defined by $r ( n ) = f ( n , n )$ . An alternative expression is $r ( n ) =$ $y ( n , n + 1 )$ , so this is a rate valid for one step starting at time n. The short rates are unknown in advance, except for the current one, $r ( 0 )$ . It is important to distinguish between $r ( n )$ and $f ( 0 , n )$ . Both rates apply to a single step from time n to $n + 1$ , but the former is random, whereas the latter is known at the present moment and determined by the initial term structure. 

The money market account denoted by $A ( n ) , n \geq 1$ , is defined by 

$$
A (n) = \exp \{\tau (r (0) + r (1) + \dots + r (n - 1)) \}
$$

with $A ( 0 ) = 1$ , and represents the value at time n of one dollar invested in an account attracting interest given by the short rate under continuous compounding. For example, if $\textstyle \tau = { \frac { 1 } { 3 6 5 } }$ , then the interest is given by the overnight rate. 

The money market account defined in Chapter 2 was a deterministic sequence independent of the particular way the initial dollar is invested. Here $A ( n )$ is random and, as will be seen below, in general diferent from $\exp \{ \tau n y ( 0 , n ) \}$ , the latter being deterministic and constructed by using zerocoupon bonds maturing at time n. 

## Example 10.13

In the setting introduced in Example 10.11, suppose that the bond prices change 

as follows: 

$$
\begin{array}{l} B (0, 1) = 0. 9 9 0 1, \\ B (0, 2) = 0. 9 8 2 8, \quad B (1, 2) = 0. 9 9 4 7, \\ B (0, 3) = 0. 9 7 2 6, \quad B (1, 3) = 0. 9 8 4 8, \quad B (2, 3) = 0. 9 9 0 5. \end{array}
$$

The corresponding yields are 

$$
\begin{array}{l}y(0,1)\cong 11.94\% ,\\ y(0,2)\cong 10.41\% ,\quad y(1,2)\cong 6.38\% ,\\ y(0,3)\cong 11.11\% ,\quad y(1,3)\cong 9.19\% ,\quad y(2,3)\cong 11.45\% . \end{array}
$$

The forward rates are 

$$
\begin{array}{l}f(0,0)\cong 11.94\% ,\\ f(0,1)\cong 8.88\% , \quad f(1,1)\cong 6.38\% ,\\ f(0,2)\cong 12.52\% , \quad f(1,2)\cong 12.00\% , \quad f(2,2)\cong 11.45\% . \end{array}
$$

We can read of the short rates and compute the values of the money market account 

$$
\begin{array}{l l} & A(0) = 1, \\ r(0) = f(0,0)\cong 11.94\% , & A(1)\cong 1.0100,\\ r(1) = f(1,1)\cong 6.38\% , & A(2)\cong 1.0154,\\ r(2) = f(2,2)\cong 11.45\% , & A(3)\cong 1.0251. \end{array}
$$

## Exercise 10.21

Which bond prices in Example 10.13 can be altered so that the values of the money market remain unchanged? 

## Exercise 10.22

Using the data in Example 10.13, compare the logarithmic return on an investment in the following securities over the period from 0 to 3: a) zero-coupon bonds maturing at time 3; b) single-period zero-coupon bonds; c) the money market account. 

# Stochastic Interest Rates

This chapter is devoted to modelling the time evolution of random interest rates. We adopt an approach similar to the binomial model of stock prices in Chapter 3. Modelling the evolution of interest rates can be reduced to modelling the evolution of the bond prices, since the latter determine the former. We begin with some properties that a model of bond prices should satisfy, emphasising the diferences between bonds and stock. 

First, let us recall that the evolution of interest rates or bond prices is described by functions of two variables, the running time and the maturity time, whereas stock prices are functions of just one variable, the running time. 

Second, there are many ways of describing the term structure: bond prices, implied yields, forward rates, short rates. Bond prices and yields are clearly equivalent, being linked by a simple formula. Bond prices and forward rates are also equivalent. The short rates are diferent, easier to handle, but the problem of reconstructing the term structure emerges. This may be non-trivial, since short rates usually carry less information. 

Third, the model needs to match the initial data. For a stock this is just the current price. In the case of bonds the whole initial term structure is given, imposing more restrictions on the model, which has to be consistent with all currently available market information. 

Fourth, bonds become non-random at maturity. This is in sharp contrast with stock prices. The fact that a bond gives a sure dollar at maturity has to be included in the model. 

Finally, the dependence of yields on maturity must be quite special. Bonds with similar maturities will typically behave in a similar manner. In statistical terms this means that they are strongly positively correlated. 

## 11.1 Binomial Tree Model

The shape of the tree will be similar to that in Section 3.2. However, to facilitate the necessary level of sophistication of the model, it has to be more complex. Namely, the probabilities and returns will depend on the position in the tree. We need suitable notation to distinguish between diferent positions. 

By a state we mean a finite sequence of consecutive up or down movements. The state depends, first of all, on time or, in other words, on the number of steps. We shall use sequences of letters u and d of various lengths, the length corresponding to the time elapsed (the number of steps from the root of the tree). At time 1 we have just two states $s _ { 1 } = \mathrm { u }$ or d, at time 2 four states $s _ { 2 } = \mathrm { u d }$ , dd, du, or uu. We shall write $s _ { 2 } = s _ { 1 } \mathrm { u }$ or $s _ { 1 } \mathrm { d } .$ , meaning that we go up or, respectively, down at time 2, having been at $s _ { 1 }$ at time 1. In general, $s _ { n + 1 } = s _ { n } \mathrm { u }$ or $s _ { n } \mathrm { d }$ 

The probabilities will be allowed to depend on particular states. We write $p ( s _ { n } )$ to denote the probability of going up at time $n + 1$ , having started at state $s _ { n }$ at time n. At the first step the probability of going up will be denoted by p without an argument. In Figure 11.1 we have $p = 0 . 3 , p ( \mathrm { u } ) = 0 . 1 , p ( \mathrm { d } ) =$ $0 . 4 , p ( \mathrm { u u } ) = 0 . 4 , p ( \mathrm { u d } ) = 0 . 2 , p ( \mathrm { d u } ) = 0 . 5 , p ( \mathrm { d d } ) = 0 . 4 ,$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/37cb80011c1e2ec4575f28b4aeab355291e88f42207a0e7d59021b96e679bf96.jpg)



Figure 11.1 States and probabilities


Let us fix a natural number N as the time horizon. It will be the upper bound of the maturities of all the bonds considered. The states $s N$ at time N represent the complete scenarios of bond price movements. 

Next, we shall describe the evolution of bond prices. At time 0 we are given the initial bond prices for all maturities up to N, that is, a sequence of N numbers 

$$
B (0, 1), B (0, 2), B (0, 3), \dots , B (0, N - 1), B (0, N).
$$

At time 1 one of the prices becomes redundant, namely the first bond matures and only the remaining $N - 1$ bonds are still being traded. We introduce randomness by allowing two possibilities distinguished by the states u and d, so we have two sequences 

$$
\begin{array}{l} B (1, 2; \mathrm{u}), B (1, 3, \mathrm{u}), \ldots , B (1, N - 1; \mathrm{u}), B (1, N; \mathrm{u}), \\ B (1, 2; \mathrm{d}), B (1, 3; \mathrm{d}), \ldots , B (1, N - 1; \mathrm{d}), B (1, N; \mathrm{d}). \end{array}
$$

At time 2 we have four states and four sequences of length $N - 2$ 

$$
\begin{array}{l} B (2, 3; \mathrm{uu}), \ldots , B (2, N - 1; \mathrm{uu}), B (2, N; \mathrm{uu}), \\ B (2, 3; \mathrm{ud}), \ldots , B (2, N - 1; \mathrm{ud}), B (2, N; \mathrm{ud}), \\ B (2, 3; \mathrm{du}), \ldots , B (2, N - 1; \mathrm{du}), B (2, N; \mathrm{du}), \\ B (2, 3; \mathrm{dd}), \ldots , B (2, N - 1; \mathrm{dd}), B (2, N; \mathrm{dd}). \end{array}
$$

We do not require that the ud and du prices coincide, which was the case fo stock prices movements in Section 3.2. 

This process continues in the same manner. At each step the length of the sequence decreases by one and the number of sequences doubles. At time $N - 1$ we have just single numbers, $2 ^ { N - 1 }$ of them, 

$$
B (N - 1, N; s _ {N - 1})
$$

indexed by all possible states $s N - 1$ . The tree structure breaks down here because the last movement is certain: The last bond matures, becoming a sure dollar at time N, $B ( N , N ; s _ { N } ) = 1$ for all states. 

## Example 11.1

A particular evolution of bond prices for $N = 3$ , with monthly steps $\textstyle ( \tau = { \frac { 1 } { 1 2 } } )$ is given in Figure 11.2. The prices of three bonds with maturities 1, 2, and 3 are shown. 

The evolution of bond prices can be described be means of returns. Suppose we have reached state $s _ { n - 1 }$ and the bond price $B ( n - 1 , N ; s _ { n - 1 } )$ becomes known. Then we can write 

$$
B (n, N; s _ {n - 1} \mathrm{u}) = B (n - 1, N; s _ {n - 1}) \exp \{k (n, N; s _ {n - 1} \mathrm{u}) \},
$$

$$
B (n, N; s _ {n - 1} \mathrm{d}) = B (n - 1, N; s _ {n - 1}) \exp \{k (n, N; s _ {n - 1} \mathrm{d}) \},
$$

$$
\begin{array}{c} B (0, 1) = 0. 9 9 0 1 \\ B (0, 2) = 0. 9 8 2 8 \\ B (0, 3) = 0. 9 7 2 6 \end{array} \begin{array}{c} B (1, 2; u) = 0. 9 9 4 8 \\ B (1, 3; u) = 0. 9 8 4 8 \end{array} \begin{array}{c} B (2, 3; u u) = 0. 9 9 0 5 \\ B (2, 3; u d) = 0. 9 8 7 5 \end{array} \begin{array}{c} B (1, 2; d) = 0. 9 9 0 7 \\ B (1, 3; d) = 0. 9 8 0 8 \end{array} \begin{array}{c} B (2, 3; d u) = 0. 9 9 0 8 \\ B (2, 3; d d) = 0. 9 8 9 1 \end{array}
$$

Figure 11.2 Evolution of bond prices in Example 11.1 

implicitly defining the logarithmic returns 

$$
\begin{array}{l} k (n, N; s _ {n - 1} \mathrm{u}) = \ln \frac {B (n , N ; s _ {n - 1} \mathrm{u})}{B (n - 1 , N ; s _ {n - 1})}, \\ k (n, N; s _ {n - 1} \mathrm{d}) = \ln \frac {B (n , N ; s _ {n - 1} \mathrm{d})}{B (n - 1 , N ; s _ {n - 1})}. \end{array}
$$

We assume here that $k ( n , N ; s _ { n - 1 } \mathrm { u } ) \ge k ( n , N ; s _ { n - 1 } \mathrm { d } )$ 

## Remark 11.1

Note that there are some places in the tree where the returns are non-random given the state $s _ { n - 1 }$ is known. Namely, 

$$
k (n, n; s _ {n - 1} \mathrm{u}) = k (n, n; s _ {n - 1} \mathrm{d}) = \ln {\frac {1}{B (n - 1 , n ; s _ {n - 1})}},
$$

since $B ( n , n ; s _ { n } ) = 1$ for all $s _ { n }$ 

## Example 11.2

From the data in Example 11.1 we extract the prices of bonds with maturity $^ { 3 , }$ completing the picture with the final value 1. The tree shown in Figure 11.3 

$$
B (0, 3) = 0. 9 7 2 6 \begin{array}{l} B (1, 3; u) = 0. 9 8 4 8 \\ B (1, 3; d) = 0. 9 8 0 8 \end{array} \begin{array}{l} B (2, 3; u u) = 0. 9 9 0 5 \longrightarrow B (3, 3) = 1 \\ B (2, 3; u d) = 0. 9 8 7 5 \longrightarrow B (3, 3) = 1 \\ B (2, 3; d u) = 0. 9 9 0 8 \longrightarrow B (3, 3) = 1 \\ B (2, 3; d d) = 0. 9 8 9 1 \longrightarrow B (3, 3) = 1 \end{array}
$$

Figure 11.3 Prices of the bond maturing at time 3 in Example 11.2 describes the random evolution of a single bond purchased at time 0 for 0.9726. The returns are easy to compute, for instance 

$$
k (2, 3; \mathrm{ud}) = \ln {\frac {B (2 , 3 ; \mathrm{ud})}{B (1 , 3 ; \mathrm{u})}} \cong 0. 27 \%.
$$

The results are gathered in Figure 11.4. (Recall that the length of each step is one month.) 

$$
\begin{array}{c} k (1, 3; u) = 1.25 \% \\ k (1, 3; d) = 0.84 \% \end{array} \begin{array}{c} k (2, 3; u u) = 0.58 \% \longrightarrow k (3, 3) = 0.95 \% \\ k (2, 3; u d) = 0.27 \% \longrightarrow k (3, 3) = 1.26 \% \\ k (2, 3; d u) = 1.01 \% \longrightarrow k (3, 3) = 0.92 \% \\ k (2, 3; d d) = 0.84 \% \longrightarrow k (3, 3) = 1.10 \% \end{array}
$$

Figure 11.4 Returns on the bond maturing at time 3 in Example 11.2 

## Exercise 11.1

For the tree of weekly returns shown in Figure 11.5 construct the tree of bond prices and fill in the missing returns. 

$$
\begin{array}{l} k (1, 3; u) = 0. 2 6 \% \\ \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \quad \end{array}
$$

Figure 11.5 Returns in Exercise 11.1 

The evolution of bond prices is in perfect correspondence with the evolution of implied yields to maturity. Namely, 

$$
y (n, m; s _ {n}) = \frac {1}{\tau (m - n)} \ln {\frac {1}{B (n , m ; s _ {n})}}
$$

with the same tree structure as for bond prices. In particular, the final yields are non-random given that the state $s _ { n - 1 }$ at the penultimate step is known. Note that the words ‘up’ and ‘down’ lose their meaning here because the yield goes down as the bond price goes up. Nevertheless, we keep the original indicators u and d. 

## Example 11.3

We continue Example 11.1 and find the yields, bearing in mind that $\textstyle \tau = { \frac { 1 } { 1 2 } }$ The results are collected in Figure 11.6. 

$$
\begin{array}{c} y (0, 1) = 1 1. 9 4 \% \\ y (0, 2) = 1 0. 4 1 \% \\ y (0, 3) = 1 1. 1 1 \% \end{array} \begin{array}{c} y (1, 2; u) = 6. 2 6 \% \\ y (1, 3; u) = 9. 1 9 \% \end{array} \begin{array}{c} y (2, 3; u u) = 1 1. 4 5 \% \\ y (2, 3; u d) = 1 5. 0 9 \% \end{array} \begin{array}{c} y (1, 2; d) = 1 1. 2 1 \% \\ y (1, 3; d) = 1 1. 6 3 \% \end{array} \begin{array}{c} y (2, 3; d u) = 1 1. 0 9 \% \\ y (2, 3; d d) = 1 3. 1 5 \% \end{array}
$$

Figure 11.6 Yields in Example 11.3 

## Exercise 11.2

Take the returns in Exercise 11.1 and find the yield $y ( 0 , 3 )$ . What is the general relationship between the returns and yields to maturity? Can you complete the missing returns without computing the bond prices? 

Now consider the instantaneous forward rates. At the initial time 0 there are N forward rates 

$$
f (0, 0), f (0, 1), f (0, 2), \ldots , f (0, N - 1)
$$

generated by the initial bond prices. Note that the first number is the short rate $r ( 0 ) = f ( 0 , 0 )$ . For all subsequent steps the current bond prices imply the forward rates. Formula (10.6) applied to random bond prices allows us to find the random evolution of forward rates: 

$$
f (n, N; s _ {n}) = - \frac {\ln B (n , N + 1 ; s _ {n}) - \ln B (n , N ; s _ {n})}{\tau}.\tag{11.1}
$$

At time 1 we have two possible sequences of $N - 1$ forward rates obtained from two sequences of bond prices 

$$
\begin{array}{l} f (1, 1; \mathrm{u}), f (1, 2; \mathrm{u}), \ldots , f (1, N - 1; \mathrm{u}), \\ f (1, 1; \mathrm{d}), f (1, 2; \mathrm{d}), \ldots , f (1, N - 1; \mathrm{d}). \end{array}
$$

At time 2 we have four sequences of N 2 forward rates, and so on. At time N 1 we have $2 ^ { N - 1 }$ single numbers $f ( N - 1 , N - 1 ; s _ { N - 1 } )$ 

## Example 11.4

Using (11.1), we can evaluate the forward rates for the data in Example 11.1. For instance, 

$$
f (1, 2; \mathrm{u}) = - \frac {\ln B (1 , 3 ; \mathrm{u}) - \ln B (1 , 2 ; \mathrm{u})}{\tau}.
$$

Alternatively, we can use the yields found in Example 11.3 along with formula (10.7): 

$$
f (1, 2; \mathrm{u}) = 2 y (1, 3; \mathrm{u}) - y (1, 2; \mathrm{u}).
$$

The results are gathered in Figure 11.7. 

$$
\begin{array}{c} f (1, 1; u) = 6.26 \% \\ f (1, 2; u) = 12.12 \% \\ \left\{ \begin{array}{l} f (2, 2; u u) = 11.45 \% \\ f (2, 2; u d) = 15.09 \% \\ f (1, 1; d) = 11.21 \% \\ f (1, 2; d) = 12.05 \% \end{array} \right. \\ \left\{ \begin{array}{l} f (2, 2; d u) = 11.09 \% \\ f (2, 2; d d) = 13.15 \% \end{array} \right. \end{array}
$$

Figure 11.7 Forward rates in Example 11.4 

The information contained in forward rates is suficient to reconstruct the bond prices, as was shown in Proposition 10.3. 

## Exercise 11.3

Suppose a tree of forward rates is given as in Figure 11.8. Find the corresponding bond prices (using one-month steps). 

The short rates are just special cases of forward rates, 

$$
r (n; s _ {n}) = f (n, n; s _ {n})
$$

for $n \geq 1$ , with deterministic $r ( 0 ) = f ( 0 , 0 )$ . The short rates are also given by $r ( n ; s _ { n } ) = y ( n , n + 1 ; s _ { n } ) , n \geq 1$ , and $r ( 0 ) = y ( 0 , 1 )$ , that is, by the rates of return on a bond maturing at the next step. This is obvious from the relations between the forward rates and yields. 

$$
\begin{array}{c} f (0, 0) = 9.28 \% \\ f (0, 1) = 9.47 \% \\ f (0, 2) = 8.44 \% \end{array} \begin{array}{c} f (1, 1; u) = 7.95 \% \\ f (1, 2; u) = 12.39 \% \\ f (1, 1; d) = 11.82 \% \\ f (1, 2; d) = 6.93 \% \end{array} \begin{array}{c} f (2, 2; u u) = 10.72 \% \\ f (2, 2; u d) = 14.12 \% \\ f (2, 2; d u) = 10.61 \% \\ f (2, 2; d d) = 12.18 \% \end{array}
$$

Figure 11.8 Forward rates in Exercise 11.3 

We are now ready to describe the money market account. It starts with A(0) = 1. The next value 

$$
A (1) = \exp (\tau r (0))
$$

is still deterministic. It becomes random at subsequent steps. At time 2 there are two values depending on the states at time 1: 

$$
\begin{array}{r l} & A (2; \mathrm{u}) = \exp (\tau (r (0) + r (1; \mathrm{u})) = A (1) \exp \{\tau r (1; \mathrm{u}) \}, \\ & A (2; \mathrm{d}) = \exp (\tau (r (0) + r (1; \mathrm{d})) = A (1) \exp \{\tau r (1; \mathrm{d}) \}. \end{array}
$$

Next, for example, 

$$
A (3; \mathrm{ud}) = \exp (\tau (r (0) + r (1; \mathrm{u}) + r (2; \mathrm{ud})) = A (2; \mathrm{u}) \exp \{\tau r (2; \mathrm{ud}) \}.
$$

In general, 

$$
\begin{array}{l} A (n + 1; s _ {n - 1} \mathrm{u}) = A (n; s _ {n - 1}) \exp \{\tau r (n; s _ {n - 1} \mathrm{u}) \}, \\ A (n + 1; s _ {n - 1} \mathrm{d}) = A (n; s _ {n - 1}) \exp \{\tau r (n; s _ {n - 1} \mathrm{d}) \}. \end{array}
$$

## Exercise 11.4

Find the evolution of the money market account if the forward rates are the same as in Exercise 11.3. 

For bond investments the money market account plays the same role as the risk-free component of investment strategies on the stock market in ear lier chapters. It is used to discount future cash flows when valuing bonds and derivative securities, as will be shown below. 

## 11.2 Arbitrage Pricing of Bonds

Suppose that we are given the binomial tree of bond prices $B ( n , N ; s _ { n } )$ for a bond maturing at the fixed time horizon N. In addition, we are given the money market process $A ( n ; s _ { n - 1 } )$ . As was mentioned in the introduction to this chapter, the prices of other bonds cannot be completely arbitrary. We shall show that the prices $B ( n , M ; s _ { n } )$ for $M < N$ can be replicated by means of bonds with maturity N and the money market. As a consequence of the No-Arbitrage Principle, the prices of $B ( n , M ; s _ { n } )$ will have to be equal to the values of the corresponding replicating strategies. 

## Example 11.5

Consider the data in Example 11.1. At the first step the short rate is deterministic, being implied by the price $B ( 0 , 1 )$ . The first two values of the money market account are $A ( 0 ) = 1$ and $A ( 1 ) = 1 . 0 1$ . As the underlying instrument we take the bond maturing at time 3. The prices of this bond at time 0 and 1 are given in Figure 11.9, along with the prices of the bond maturing at time 2. We can find a portfolio $( x , y )$ , with x being the number of bonds of maturity 3 

$$
\begin{array}{l} B (0, 2) = 0. 9 8 2 8 \\ B (0, 3) = 0. 9 7 2 6 \end{array} \begin{array}{l} B (1, 2; u) = 0. 9 9 4 8 \\ B (1, 3; u) = 0. 9 8 4 8 \\ B (1, 2; d) = 0. 9 9 0 7 \\ B (1, 3; d) = 0. 9 8 0 8 \end{array}
$$

## Figure 11.9 Bond prices from Example 11.1

and y the position in the money market, such that the value of this portfolio matches the time 1 prices of the bond maturing at time 2. To this end we solve the following system of equations 

$$
\begin{array}{l} 0. 9 8 4 8 x + 1. 0 1 y = 0. 9 9 4 8, \\ 0. 9 8 0 8 x + 1. 0 1 y = 0. 9 9 0 7, \end{array}
$$

obtaining $x \ = \ 1$ and $y \cong \mathrm { 0 . 0 0 9 8 } .$ . The value of this portfolio at time 0 is $1 \times B ( 0 , 3 ) + 0 . 0 0 9 8 \times A ( 0 ) \cong 0 . 9 8 2 4$ , which is not equal to $B ( 0 , 2 )$ . The prices in Figure 11.9 provide an arbitrage opportunity: 

Sell a bond maturing at time 2 for $0.9828 and buy the portfolio constructed above for $0.9824. 

Whatever happens at time 1, the value of the portfolio will be suficient to buy the bond back, the initial balance $0.0004 being the arbitrage profit. 

The model in Example 11.1 turns out to be inconsistent with the No-Arbitrage Principle and has to be rectified. We can only adjust some of the future prices, since the present prices of all bonds are dictated by the market. It is easy to see that by taking $B ( 1 , 2 ; \mathrm { u } ) = 0 . 9 9 5 8$ with $B ( 1 , 2 ; \mathrm { d } )$ unchanged, or by letting $B ( 1 , 2 ; \mathrm { d } ) = 0 . 9 9 1 3$ with $B ( 1 , 2 ; \mathrm { u } )$ unchanged, we can eliminate the arbitrage opportunity. Of course, there are many other ways of repairing the model by a simultaneous change of both values of $B ( 1 , 2 )$ . Let us put $B ( 1 , 2 ; \mathrm { d } ) = 0 . 9 9 1 3$ and leave $B ( 1 , 2 ; \mathrm { u } )$ unchanged. The rectified tree of bond prices is shown in Figure 11.10 and the corresponding yields in Figure 11.11. 

$$
\begin{array}{c} B (0, 1) = 0. 9 9 0 1 \\ B (0, 2) = 0. 9 8 2 8 \\ B (0, 3) = 0. 9 7 2 6 \end{array} \begin{array}{c} B (1, 2; u) = 0. 9 9 4 8 \\ B (1, 3; u) = 0. 9 8 4 8 \\ B (1, 2; d) = 0. 9 9 1 3 \\ B (1, 3; d) = 0. 9 8 0 8 \end{array} \begin{array}{c} B (2, 3; u u) = 0. 9 9 0 5 \\ B (2, 3; u d) = 0. 9 8 7 5 \\ B (2, 3; d u) = 0. 9 9 0 8 \\ B (2, 3; d d) = 0. 9 8 9 1 \end{array}
$$


Figure 11.10 Rectified tree of bond prices in Example 11.5


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/cea0cf5122a6e83a9fc7c6d98f535510ca8eb569f844f14dec848796a9ed9ad9.jpg)



Figure 11.11 Rectified tree of yields in Example 11.5


## Remark 11.2

The process of rectifying bond prices in Example 11.5 bears some resemblance to the pricing of general derivative securities described in Chapter 8. The role of the derivative security is played by the bond maturing at time 2. The bond maturing at time 3 plays the role of the underlying security. The diference is that the present price of the bond of maturity 2 is fixed and we can only adjust the future prices in the model to eliminate arbitrage. At this stage we are concerned only with building consistent models rather than with pricing securities. 

## Exercise 11.5

Evaluate the prices of a bond maturing at time 2 given a tree of prices of a bond maturing at time 3 and short rates as shown in Figure 11.12, with $\tau = 1 / 1 2$ 

$$
B(0,3) = 0.9927 \begin{cases} B(1,3;u) = 0.9962 \\ r(0) = 4.11\% \\ B(1,3;d) = 0.9959 \end{cases} \begin{aligned} & B(2,3;uu) = 0.9991 \\ & r(1;u) = 2.40\% \\ & B(2,3;ud) = 0.9960 \\ & B(2,3;du) = 0.9986 \\ & r(1;d) = 3.00\% \\ & B(2,3;dd) = 0.9969 \end{aligned}
$$

Figure 11.12 Bond prices and short rates in Exercise 11.5 

We can readily generalize Example 11.5. The underlying bond matures at time N and we can find the structure of prices of any bond maturing at $M < N$ The replication proceeds backwards step-by-step starting from time M, for which $B ( M , M ; s _ { M } ) = 1$ in each state $s _ { M }$ . The first step is easy: for each state $s M - 1$ we take a portfolio with $x = 0$ and $y = 1 / A ( M ; s _ { M - 1 } )$ , since the bond becomes risk free one step prior to maturity. 

Next, consider time $M - 2$ . For any state $s M - 2$ we find $x = x ( M - 1 ; s _ { M - 2 } )$ , the number of bonds maturing at $N$ , and $y = y ( M - 1 ; s _ { M - 2 } )$ , the position in the money market, by solving the system 

$$
\begin{array}{l} x B (M - 1, N; s _ {M - 2} \mathrm{u}) + y A (M - 1; s _ {M - 2}) = B (M - 1, M; s _ {M - 2} \mathrm{u}), \\ x B (M - 1, N; s _ {M - 2} \mathrm{d}) + y A (M - 1; s _ {M - 2}) = B (M - 1, M; s _ {M - 2} \mathrm{d}). \end{array}
$$

In this way we can find the prices at time $M - 2$ of the bond maturing at time M, 

$$
\begin{array}{r} B (M - 2, M; s _ {M - 3} \mathrm{u}) = x B (M - 2, N; s _ {M - 3} \mathrm{u}) + y A (M - 2; s _ {M - 3}), \\ B (M - 2, M; s _ {M - 3} \mathrm{d}) = x B (M - 2, N; s _ {M - 3} \mathrm{d}) + y A (M - 2; s _ {M - 3}). \end{array}
$$

We can iterate the replication process moving backwards through the tree. 

## Remark 11.3

Replication is possible if a no-arbitrage condition analogous to Condition 3.2 is satisfied for the binomial tree. Here the condition $u > r >$ d of Chapter 3 is 

replaced by 

$$
k (n, N; s _ {n - 1} \mathrm{u}) > \tau r (n - 1; s _ {n - 1}) > k (n, N; s _ {n - 1} \mathrm{d}).\tag{11.2}
$$

Any future cash flow can be replicated in a similar fashion. Consider, for example, a coupon bond with fixed coupons. 

## Example 11.6

Take a coupon bond maturing at time 2 with face value $F = 1 0 0$ , paying coupons $C = 1 0$ at times 1 and 2. We price the future cash flow by using the zero-coupon bond maturing at time 3 as the underlying security. The coupon bond price P at a particular time will not include the coupon due (the socalled ex-coupon price). Assume that the structure of the bond prices is as in Figure 11.10. 

Consider time 1. In state u the short rate is determined by the price $B ( 1 , 2 ; \mathrm { u } ) = 0 . 9 9 4 7$ , so we have $r ( 1 ; \mathrm { u } ) \cong 6 . 3 8 \%$ . Hence $P ( \mathrm { 1 } ; \mathrm { u } ) \cong \mathrm { 1 0 9 . 4 1 } 7 0$ In state d we use $B ( 1 , 2 ; \mathrm { d } ) = 0 . 9 9 1 3$ to find $r ( 1 ; \mathrm { d } ) \cong 1 0 . 4 9 \%$ and $P ( 1 ; \mathrm { d } ) \cong$ 109.0485. 

Consider time 0. The cash flow at time 1 which we are to replicate includes the coupon due, so it is given by $P ( 1 ; \mathrm { u } ) + 1 0 \cong 1 1 9 . 4 1 7$ and $P ( 1 ; \mathrm { d } ) + 1 0 \cong$ 119.0485. The short rate $r ( 0 ) \cong 1 1 . 9 4 \%$ determines the money market account as in Example 11.5, $A ( 1 ) = 1 . 0 1$ , and we find $x \cong 9 2 . 1 3 3 7$ 7, $y \cong 2 8 . 3 9 9 8$ . Hence $P ( 0 ) \cong 1 1 8 . 0 0 9$ is the present price of the coupon bond. 

An alternative is to use the spot yields: $y ( 0 , 1 ) \cong 1 1 . 9 4 \%$ and $y ( 0 , 2 ) \cong$ 10.41% to discount the future payments with the same result: $1 1 8 . 0 0 9 \cong 1 0 \times$ $\begin{array} { r } { \exp ( - \frac { 1 } { 1 2 } \times 1 1 . 9 4 \% ) + 1 1 0 \times \exp ( - \frac { 2 } { 1 2 } \times 1 0 . 4 1 \% ) } \end{array}$ 

In general, 

$$
\begin{array}{c} P (0) = C _ {1} \exp \{- \tau y (0, 1) \} + C _ {2} \exp \{- 2 \tau y (0, 2) \} \\ + \dots + (C _ {N} + F) \exp \{- N \tau y (0, N) \}. \end{array}\tag{11.3}
$$

(For simplicity we include all time steps, so $C _ { k } = 0$ at the time steps k when no coupon is paid.) At each time k when a coupon is paid, the cash flow is the sum of the (deterministic) coupon and the (stochastic) price of the remaining bond: 

$$
\begin{array}{c} C _ {k} + P (k; s _ {k}) = C _ {k} + C _ {k + 1} \exp \{- \tau y (k, k + 1; s _ {k}) \} \\ + \dots + (C _ {n} + F) \exp \{- \tau (n - k) y (k, n; s _ {k}) \}. \end{array}
$$

Quite often the coupons depend on other quantities. In this way a coupon bond may become a derivative security. An important benchmark case is described below, where the coupons are computed as fractions of the face value. 

These fractions, defining the coupon rate, are obtained by converting the short rate to an equivalent discrete compounding rate. In practice, when $\tau$ is one day, the coupon rate will be the overnight LIBOR rate. 

## Proposition 11.1

A coupon bond maturing at time N with random coupons 

$$
C _ {k} (s _ {k - 1}) = (\exp \{\tau r (k - 1; s _ {k - 1}) \} - 1) F\tag{11.4}
$$

for $0 < k \le N$ is trading at par. (That is, the price $P ( 0 )$ is equal to the face value $F . )$ 

## Proof

Fix time $N - 1$ and a state $s N - 1$ . In this state the value $P ( N - 1 ; s _ { N - 1 } )$ of the bond is $F + C _ { N } ( s _ { N - 1 } )$ discounted at the short rate, which gives $P ( N - 1 ; s _ { N - 1 } ) = F$ if the coupon is expressed by (11.4). Proceeding backwards through the tree and applying the same argument for each state, we finally arrive at $P ( 0 ) = F$ □ 

## Exercise 11.6

Find the coupons of a bond trading at par and maturing at time 2, given the yields as in Example 11.5, see Figure 11.11. 

## 11.2.1 Risk-Neutral Probabilities

In Chapter 3 we have learnt that the stock price $S ( n )$ at time n is equal to the expectation under the risk-neutral probability of the stock price $S ( n + 1 )$ at time $n + 1$ discounted to time n. The situation is similar in the binomial model of interest rates. 

The discount factors are determined by the money market account, or, in other words, by the short rates. In general, they are random, being of the form exp $\left\{ - \tau r ( n ; s _ { n } ) \right\}$ 

Suppose that state $s _ { n }$ has occurred at time n. The short rate determining the time value of money for the next step is now known with certainty. Consider a bond maturing at time N with $n < N - 1$ . We are given the bond price $B ( n , N ; s _ { n } )$ and two possible values at the next step, $B ( n + 1 , N ; s _ { n } \mathrm { u } )$ and $B ( n +$ $1 , N ; s _ { n } \mathrm { d } )$ . These values represent a random variable, which will be denoted by $B ( n + 1 , N ; s _ { n } \cdot )$ . If $n = N - 1$ , then the bond matures at the next step N, when it has just one price independent of the state, namely the face value. We are looking for a probability $p _ { * }$ such that 

$$
\begin{array}{c} B (n, N; s _ {n}) = [ p _ {*} B (n + 1, N; s _ {n} \mathrm{u}) + (1 - p _ {*}) B (n + 1, N; s _ {n} \mathrm{d}) ] \\ \times \exp \{- \tau r (n; s _ {n}) \}. \end{array}\tag{11.5}
$$

This equation can be solved for $p _ { * }$ , which in principle depends on n, N and $s _ { n }$ (As will turn out soon, see Proposition 11.2, $p _ { * }$ is in fact independent of maturity N.) Recalling the definition of logarithmic returns, we have 

$$
B (n + 1, N; s _ {n + 1}) = B (n, N; s _ {n}) \exp \{k (n + 1, N; s _ {n + 1}) \},
$$

which gives 

$$
p _ {*} (n, N; s _ {n}) = \frac {\exp \{\tau r (n ; s _ {n}) \} - \exp \{k (n + 1 , N ; s _ {n} \mathrm{d}) \}}{\exp \{k (n + 1 , N ; s _ {n} \mathrm{u}) \} - \exp \{k (n + 1 , N ; s _ {n} \mathrm{d}) \}}.\tag{11.6}
$$

These numbers are called the risk-neutral or martingale probabilities. Condi tion (11.2) for the lack of arbitrage can now be written as 

$$
0 <   p _ {*} (n, N; s _ {n}) <   1.
$$

## Example 11.7

We shall find the tree of risk-neutral probabilities $p _ { * } ( n , 3 ; s _ { n } )$ for $n = 0 , 1$ , using the data in Example 11.5 (the bond prices as shown in Figure 11.10). 

First we compute the returns on the money market. The simplest way is to use the yields (Figure 11.11). With $\begin{array} { r } { \tau = \frac { 1 } { 1 2 } } \end{array}$ we have $\tau r ( n ; s _ { n } ) = y ( n , n +$ $1 ; s _ { n } ) / 1 2 , n = 0 , 1$ , which gives the following values: 

$$
\tau r(0) = 0.995\% \quad <  \quad \begin{array}{l}\tau r(1;\mathrm{u}) = 0.521\% \\ \tau r(1;\mathrm{d}) = 0.874\% \end{array}
$$

Next, we find the returns $k ( 1 , 3 ; s _ { 1 } )$ and $k ( 2 , 3 ; s _ { 2 } )$ on bonds. For example, if $s _ { 2 } = \mathrm { u d }$ , then $\begin{array} { r } { k ( 2 , 3 ; \mathrm { u d } ) = \ln ( \frac { 0 . 9 8 7 5 } { 0 . 9 8 4 8 } ) } \end{array}$ . The results are collected below: 

$$
\begin{array}{l l l l} & & k(2,3;\mathrm{uu}) = 0.58\% \\ & k(1,3;\mathrm{u}) = 1.25\% & <  & \\ / & & k(2,3;\mathrm{ud}) = 0.27\% \\ & & k(2,3;\mathrm{du}) = 1.01\% \\ \backslash & k(1,3;\mathrm{d}) = 0.84\% & <  & \\ & & k(2,3;\mathrm{dd}) = 0.84\% \end{array}
$$

We can see that the no-arbitrage conditions are satisfied: $0 . 8 4 \% < 0 . 9 9 \% <$ $1 . 2 5 \% , 0 . 2 7 \% < 0 . 5 2 \% < 0 . 5 8 \%$ and $0 . 8 4 \% < 0 . 8 7 \% < 1 . 0 1 \%$ 

Finally, we find the desired probabilities by a direct application of (11.6): $p _ { * } ( 0 ) = 0 . 3 8 1 3 , p _ { * } ( 1 ; \mathrm { u } ) = 0 . 8 1 5 9 , p _ { * } ( 1 ; \mathrm { d } ) = 0 . 1 8 1 1$ , see Figure 11.13. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/6de4bb9c06192856b24bdace920d3870c8df847caefa0696729cd16e4e77818a.jpg)



Figure 11.13 Risk-neutral probabilities in Example 11.7


A crucial observation about the model is this: Pricing via replication is equivalent to pricing by means of the risk-neutral probability. This follows from the No-Arbitrage Principle and applies to any cash flow, even a random one, where the amounts depend on the states. This opens a way to pricing absolutely any security by means of the expectation with respect to the probabilitie $p _ { * } ( n , N ; s _ { n } )$ . The expectation is computed step-by-step, starting at the last one and proceeding backwards through the tree. 

## Example 11.8

Consider a coupon bond maturing at N = 2 with face value $F = 1 0 0$ and with coupons equal to 5% of the current value of the bond, paid at times 1 and 2. In particular, the coupon at maturity is $C _ { 2 } = 5$ in each state. Using the risk-neutral probabilities from Example 11.7, we can find the bond values at time 1. In the up state we have the discounted value of 105 due at maturity using the short rate $r ( 1 ; \mathrm { u } ) \cong 6 . 2 6 \%$ , which gives 104.4540. In the same way in the down state we obtain 104.0865. Now we add 5% coupons, so the amounts due at time 1 become 109.6767 in the up state and 109.2908 in the down state. Using the risk-neutral probabilities, we find the present value of the bond: $1 0 8 . 3 5 4 5 \cong ( 0 . 3 8 1 3 \times 1 0 9 . 6 7 6 7 + 0 . 6 1 8 7 \times 1 0 9 . 2 9 0 8 ) / 1 . 0 1$ 

## Exercise 11.7

Use the risk-neutral probabilities in Example 11.7 to find the present value of the following random cash flow: At time 2 we receive $20 in the state uu, $10 in the states ud and du, and nothing in the state dd. No payments are due at other times. 

## Exercise 11.8

Find an arbitrage opportunity for the bond prices in Figure 11.14. 

$$
\begin{array}{c} B (0, 1) = 0. 9 9 5 4 \\ B (0, 2) = 0. 9 8 7 3 \\ B (0, 3) = 0. 9 7 8 8 \end{array} \begin{array}{c} B (1, 2; u) = 0. 9 9 2 4 \\ B (1, 3; u) = 0. 9 8 3 8 \end{array} \begin{array}{c} B (2, 3; u u) = 0. 9 9 5 2 \\ B (2, 3; u d) = 0. 9 9 1 5 \end{array} \begin{array}{c} B (1, 2; d) = 0. 9 9 0 2 \\ B (1, 3; d) = 0. 9 8 1 8 \end{array} \begin{array}{c} B (2, 3; d u) = 0. 9 9 2 1 \\ B (2, 3; d d) = 0. 9 9 0 1 \end{array}
$$

Figure 11.14 Bond prices in Exercise 11.8 

## Exercise 11.9

Suppose that the risk-neutral probabilities are equal to $\textstyle { \frac { 1 } { 2 } }$ in every state. Given the following short rates, find the prices of a bond maturing at time 3 (with a one-month time step, $\begin{array} { r } { \tau = \frac { 1 } { 1 2 } ) } \end{array}$ : 

$$
\begin{array}{c c c c c} & & & & r (2; \mathrm{uu}) = 8.3 \% \\ & & r (1; \mathrm{u}) = 8.5 \% & <   & \\ & / & & & r (2; \mathrm{ud}) = 8.9 \% \\ r (0) = 9.5 \% & & & & \\ & \backslash & & & r (2; \mathrm{du}) = 9.1 \% \\ & & r (1; \mathrm{d}) = 9.8 \% & <   & \\ & & & & r (2; \mathrm{dd}) = 9.3 \% \end{array}
$$

The next proposition gives an important result, which simplifies the model significantly. 

## Proposition 11.2

The lack of arbitrage implies that the risk-neutral probabilities are independent of maturity. 

## Proof

Consider two bonds with maturities $M \leq N$ and fix an $n \leq M$ . For each of the two bonds we have 

$$
B (n, M; s _ {n}) = \left[ p _ {*} (n, M; s _ {n}) B (n + 1, M; s _ {n} \mathrm{u}) + \left(1 - p _ {*} (n, M; s _ {n})\right) \right.
$$

$$
\left. \times B (n + 1, M; s _ {n} \mathrm{d}) \right] \exp \{- \tau r (n; s _ {n}) \},\tag{11.7}
$$

(11.8) 

Our goal is to show that $p _ { * } ( n , M ; s _ { n } ) = p _ { * } ( n , N ; s _ { n } )$ in any state $s _ { n }$ . 

We can replicate the prices of the bond maturing at time M by means of the bond with maturity N and the money market account. Hence we find numbers x, y such that 

$$
\begin{array}{l} B (n + 1, M; s _ {n} \mathrm{u}) = x B (n + 1, N; s _ {n} \mathrm{u}) + y A (n + 1; s _ {n}), \\ B (n + 1, M; s _ {n} \mathrm{d}) = x B (n + 1, N; s _ {n} \mathrm{d}) + y A (n + 1; s _ {n}). \end{array}
$$

The No-Arbitrage Principle implies that equalities of this kind must also hold at time n, 

$$
\begin{array}{l} B (n, M; s _ {n - 1} \mathrm{u}) = x B (n, N; s _ {n - 1} \mathrm{u}) + y A (n; s _ {n - 1}), \\ B (n, M; s _ {n - 1} \mathrm{d}) = x B (n, N; s _ {n - 1} \mathrm{d}) + y A (n; s _ {n - 1}). \end{array}
$$

Inserting the values of the M-bonds into (11.7) and using the formula for the money market account, after some algebraic transformations we obtain 

$$
\begin{array}{c} B (n, N; s _ {n}) = [ p _ {*} (n, M; s _ {n}) B (n + 1, N; s _ {n} \mathrm{u}) + (1 - p _ {*} (n, M; s _ {n})) \\ \times B (n + 1, N; s _ {n} \mathrm{d}) ] \exp \{- \tau r (n; s _ {n}) \}. \end{array}
$$

This can be solved for $p _ { * } ( n , M ; s _ { n } )$ . It turns out that the solution coincides with the probability $p _ { * } ( n , N ; s _ { n } )$ implied by (11.8), as claimed. □ 

Exercise 11.10 

Spot an arbitrage opportunity if the bond prices are as in Figure 11.15. 

## 11.3 Interest Rate Derivative Securities

The tools introduced above make it possible to price any derivative security based on interest rates or, equivalently, on bond prices. Within the binomial tree model the cash flow associated with the derivative security can be replicated using the money market account and a bond with suficiently long maturity. The bond does not even have to be the underlying security, since the prices of various bonds must be consistent. An alternative is to use the risk-neutral probabilities. The latter approach is often preferable to replication because of its simplicity. The equivalence of both methods should be clear in view of what has been said before. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/2c4610dae1e55386a67f09d13e1d87c52d9bc0db1fbe6ca534221fd8dc597b23.jpg)



Figure 11.15 Data for Exercise 11.10


The pricing of complex securities can essentially be reduced to finding the associated cash flows. Below we present examples of some classical interest rate contingent claims. We begin with the simplest case of options. 

## 11.3.1 Options

The underlying securities for interest rate options are bonds of various kinds. 

## Example 11.9

With the bond prices as in Example 11.5 (Figure 11.10), consider a call option with exercise time 2 and strike price $X = 0 . 9 9$ on a zero-coupon bond maturing at time 3. Starting with the final payofs shown in the last column in the table below, we move back step-by-step, computing the risk-neutral expectations of the consecutive values discounted by the appropriate short rates: 

$$
\begin{array}{c c c c} n = 0 & n = 1 & n = 2 \\ \hline & & 0. 0 0 0 5 \\ & 0. 0 0 0 4 1 & <   \\ 0. 0 0 0 2 4 & / & 0 \\ & \backslash & 0. 0 0 0 8 \\ & 0. 0 0 0 1 4 & <   \\ & & 0 \end{array}
$$

As a result, the price of the option is 0.00024. 

## Exercise 11.11

Assume the structure of bond prices in Example 11.5 (Figure 11.10). Consider a coupon bond maturing at time 2 with face value $F = 1 0 0$ and coupons $C = 1$ payable at each step. Find the price of an American call option expiring at time 2 with strike price $X = 1 0 1 . 3 0$ . (Include the coupon in the bond price at each step.) 

Call options on bonds can be used by institutions issuing bonds to include the possibility of buying the bond back prior to maturity for a prescribed price. A bond that carries such a provision is called a callable bond. Its price should be reduced by the price of the attached option. 

## 11.3.2 Swaps

Writing and selling a bond is a method of borrowing money. In the case of a coupon bond trading at par the principal represents the sum borrowed and the coupons represent the interest. This interest may be fixed or floating (variable). The interest is fixed if all coupons are the same. Floating interest can be realised in many ways. Here we assume that it is determined by the short rates as in (11.4). The basis for our discussion is laid by Proposition 11.1, according to which the market value of such a floating-coupon bond must be equal to its face value, the bond trading at par. For a fixed-coupon bond trading at par the size of the coupons can easily be found from (11.3). We could say that the resulting fixed coupon rate is equivalent to the variable short rate over the lifetime of the bond. 

## Example 11.10

Consider a fixed-coupon bond and a floating-coupon bond, both with annual coupons, trading at par and maturing after two years with face value $F = 1 0 0$ Given that the tree of one- and two-year zero-coupon bond prices is 

$$
\begin{array}{l l} & B (1, 2; \mathrm{u}) = 0. 9 1 0 1 \\ B (0, 1) = 0. 9 1 2 3 & <   \\ B (0, 2) = 0. 8 2 5 6 & B (1, 2; \mathrm{d}) = 0. 8 9 8 7 \end{array}
$$

where a time step is taken to be one year, $\tau = 1$ , we can evaluate the coupons of the fixed- and floating-coupon bonds. The size of the floating coupons can be found from (11.4), 

$$
\begin{array}{c} C _ {1} = (B (0, 1) ^ {- 1} - 1) F \cong 9. 6 1 3 1, \\ C _ {2} (\mathrm{u}) = (B (1, 2; \mathrm{u}) ^ {- 1} - 1) F \cong 9. 8 7 8 0, \\ C _ {2} (\mathrm{d}) = (B (1, 2; \mathrm{d}) ^ {- 1} - 1) F \cong 1 1. 2 7 1 8. \end{array}
$$

The fixed coupons C can be found by solving equation (11.3), which takes the form 

$$
F = C B (0, 1) + (C + F) B (0, 2).
$$

This gives 

$$
C \cong 1 0. 0 3 5 1.
$$

By buying a fixed-coupon bond and selling a floating-coupon one (or the other way round, selling a fixed-coupon bond and buying a floating-coupon one) an investor can create an random cash flow with present value zero, since the two kinds of bond have the same initial price. 

A company who has sold fixed-coupon bonds and is paying fixed interest may sometimes wish to switch into paying the floating rate instead. This can be realised by writing a floating-coupon bond and buying a fixed-coupon bond with the same present value. In practice, a financial intermediary will provide this service by ofering a contract called a swap. Clearly, a swap of this kind will cost nothing to enter. Here is an example of a practical situation, where the role of the intermediary is to match the needs of two particular companies. 

## Example 11.11

Suppose that company A wishes to borrow at a variable rate, whereas B prefers a fixed rate. Banks ofer the following efective rates (that is, rates referring to 

annual compounding): 

<table><tr><td></td><td>A</td><td>B</td></tr><tr><td>fixed</td><td>11.40%</td><td>13.40%</td></tr><tr><td>variable</td><td>LIBOR + 2%</td><td>LIBOR + 3%</td></tr></table>

In this case we say that A has comparative advantage over B in the fixed rate, with B having comparative advantage over A in the variable rate. (Notwithstanding the fact that the overall credit rating of A is better, as reflected by the lower interest rates ofered.) In these circumstances A should borrow at the fixed rate, B should borrow at the variable rate, and they can swap their interest payments. 

Consider a principal of $100, 000 borrowed for one year and suppose that LIBOR is 10% and (just for simplicity) remains the same during the first year of the loan. If A borrows at the variable rate and B at the fixed rate, then the total interest paid will be $25, 400 between them. However, if A borrows at the fixed rate and B at the variable rate, the interest payments will be only $24, 400 in total. The diference of $1, 000 will be available to share between the two companies if they arrange to swap the rates. (In practice, this amoun would be reduced by a fee charged by the intermediary arranging the deal.) If LIBOR changes to 9%, say, in the second year of the loan, so will the total interest payable, but the diference will remain at $1, 000. 

How should this diference be shared between the two companies? To answer the question, we assume the term structure of interest rates determined by the prices of one- and two-year zero-coupon bonds in Example 11.10. In particular, we can identify LIBOR with the efective short rate implied by the bond prices, $B ( 0 , 1 ) ^ { - 1 } - 1$ in year one and $B ( 1 , 2 ) ^ { - 1 } - 1$ in year two. These are the same rates as those implied by the floating coupons in Example 11.10. The fixed coupons in the same example imply a rate of 10.04%. 

Instead of swapping interest payments with B, company A would achieve the same result by taking a loan of $100, 000 at the fixed rate of 11.40% ofered by the bank, buying 1, 000 of the fixed-coupon bonds, and writing 1, 000 of the floating-coupon bonds considered in Example 11.10. As a result, company A will have borrowed $100, 000 at the rate $1 1 . 4 0 \% - 1 0 . 0 4 \% + \mathrm { { L I B O R } = \mathrm { { L I B O R } + } }$ 1.36%. Compared to the variable rate of LIBOR + 2% ofered to company A, this is a gain of 0.64%. On a $100, 000 loan this would mean a gain of $640 in each year. 

By a similar argument, instead of swapping with A, company B could bor row $100, 000 at the variable rate $\mathrm { L I B O R } + 3 \%$ , buy 1, 000 floating-coupon bonds and write 1, 000 fixed-coupon bonds. As a result, B would pay interest at $\mathrm { L I B O R } + 3 \% - \mathrm { L I B O R } + 1 0 . 0 4 \% = 1 3 . 0 4 \%$ , a gain of 0.36% as compared to the fixed rate of 13.40% it was ofered. This means a gain of $360 in each year on an $100, 000 loan. 

The result is that the $1, 000 gain should be shared as $640 and $360 be tween companies A and B. 

Finally, note that the value of the swap may vary with time and state, departing from the initial value of zero. If a company wishes to enter into a swap agreement at a later time, it may purchase a swaption, which is a call option on the value of the swap (with prescribed strike price and expiry time). 

## 11.3.3 Caps and Floors

A cap is a provision attached to a variable-rate bond which specifies the maxi mum coupon rate paid in each period over the lifetime of a loan. A caplet is a similar provision applied to a particular single period. In other words, a caplet is a European option on the level of interest paid or received. A cap can be thought of as a series of caplets. 

## Example 11.12

We take a loan by selling a par floating-coupon bond maturing at time 3. (That is, a bond which always has the par value, the coupons being implied by the short rates as in (11.4).) We use the bond prices and rates in Example 11.5, see Figures 11.10 and 11.11. The cash flow shown below includes the initial amount received for selling the bond together with the coupons and face value to be paid: 

$$
\begin{array}{c c c c c} n = 0 & & n = 1 & & n = 2 \\ \hline & & - 0. 9 9 9 9 0 & - & - 1 0 0. 5 2 2 7 2 \\ 1 0 0 & <   & & & \\ & & - 0. 9 9 9 9 0 & - & - 1 0 0. 8 7 7 6 4 \end{array}
$$

Consider a caplet that applies at time 1 (one month) with strike interest rate of 8% (corresponding to 0.67% for a one-month period). The coupon determined by the caplet rate is 0.66889 and we modify the cash flow accordingly. At time 0 we find the bond price by discounting its time 1 value, 100.66889 in each state, that is 100 plus the coupon. This gives the following cash flow: 

$$
\begin{array}{c c c c c} n = 0 & & n = 1 & & n = 2 \\ \hline & & - 0. 6 6 8 8 9 & - & - 1 0 0. 5 2 2 7 2 \\ 9 9. 6 7 2 2 7 & <   & & & \\ & & - 0. 6 6 8 8 9 & - & - 1 0 0. 8 7 7 6 4 \end{array}
$$

The price of the bond is reduced by the value of the caplet, that is, by 0.32773. 

For a caplet at time 2 with the same strike rate the maximum size of the coupon is 0.66889, as before. In the up state we pay the original interest, exercising the caplet in the down state. The value of the bond at time 1 is not 100, since the final coupons are no longer the same as for the par bond. The time 1 prices are obtained by discounting the time 2 values. At time 0 we find the bond price by evaluating the risk-neutral expectation of the discounted values of the bond at time 1. The resulting cash flow is 

$$
\begin{array}{c c c c c} n = 0 & & n = 1 & & n = 2 \\ \hline & & - 0. 9 9 9 9 0 & - & - 1 0 0. 5 2 2 7 2 \\ 9 9. 8 7 3 2 3 & <   & & & \\ & & - 0. 9 9 9 9 0 & - & - 1 0 0. 6 6 8 8 9 \end{array}
$$

This fixes the price of this caplet at 0.12677. 

Finally, consider a cap for both times 1 and 2 with the same strike rate as above. The cash flow can be obtained in a similar manner: 

$$
\begin{array}{c c c c c} n = 0 & & n = 1 & & n = 2 \\ \hline & & - 0. 6 6 8 8 9 & - & - 1 0 0. 5 2 2 7 2 \\ 9 9. 5 4 5 5 0 & <   & & & \\ & & - 0. 6 6 8 8 9 & - & - 1 0 0. 6 6 8 8 9 \end{array}
$$

We can see that the value of the cap, 0.45450, is the sum of the values of the caplets. 

Analogously, a floor is a provision limiting the coupon from below. This will be of value for a bond holder. It is composed from a series of floorlets, each referring to a single period. 

## Exercise 11.12

In the framework of the above example, value a floor expiring at time 2 with strike rate 8%, based on the bond prices in Example 11.5. 

## 11.4 Final Remarks

We conclude this chapter with some informal remarks on possible ways in which models of the structure of bond prices can be built. This is a complex area and all we can do here is to make some general comments. 

As we have seen, the theory of interest rates is more complicated than the theory of stock prices. In order to be able to price interest rate derivatives, we need a model of possible movements of bond prices for each maturity. The bond prices with diferent maturities have to be consistent with each other. As we have seen above, the specification of 

a) a model of possible short rates, 

b) a model of possible values of a bond with the longest maturity (consistent with the initial term structure) 

determines the structure of possible prices of all bonds maturing earlier. An alternative approach is to specify 

a) a model of possible short rates, 

b) the probabilities at each state, 

and, taking these probabilities as risk-neutral ones, to compute the prices of all bonds for all maturities. The latter method is conceptually simpler, especially if we take the same probability in each state. The flexibility of short rate mod elling allows us to obtain suficiently many models consistent with the initial term structure. 

If so, the simplest choice of probability $1 / 2$ at each state of the binomial tree appears to be as good as any, and we can focus on constructing short rate models so that their parameters are consistent with historical data. A general short-rate model in discrete time can be described as follows. Let $t _ { n } ~ = ~ n \tau$ Then the following relations specify a tree of the rate movements 

$$
r (t _ {n + 1}) - r (t _ {n}) = \mu (t _ {n}, r (t _ {n})) \tau + \sigma (t _ {n}, r (t _ {n})) \xi_ {n}
$$

where $\xi _ { n } ~ = ~ \pm 1$ with probability $1 / 2$ each, and $\mu ( t , r ) , \ \sigma ( t , r )$ are suitably chosen functions. In the continuous time limit (in the spirit of Section 3.3.2) these relations lead to a stochastic diferential equation of the form 

$$
\mathrm{d} r (t) = \mu (t, r (t)) \mathrm{d} t + \sigma (t, r (t)) \mathrm{d} w (t).
$$

There are many ways in which the functions $\mu$ and $\sigma$ can be specified, but none of them is universally accepted. Here are just a few examples: $\mu ( t , r ) = b - a r _ { \mathrm { : } }$ $\sigma ( t , r ) = \sigma$ (Vasiˇcek model), $\mu ( t , r ) = a ( b - r ) , \sigma ( t , r ) = \sigma \sqrt { r }$ (Cox–Ingersoll– Ross model), or $\mu ( t , r ) = \theta ( t ) r , \sigma ( t , r ) = \sigma r$ (Black–Derman–Toy model). 

Given the short-rates, the next step is to compute the bond prices. These will depend on the functions $\mu$ and $\sigma .$ . Two problems may be encountered: 

1. The model is too crude, for example these functions are just constants. Then we may not be able to adjust them so that the resulting bond prices agree with the initial term structure. 

2. The model is too complicated, for example we take absolutely general functions $\mu , \sigma .$ . Fitting the initial term structure imposes some constraints on the parameters, but many are left free and the result is too general to be of any practical use. 

These problems can be avoided if some middle-of-the-road solution is adopted. 

Yet another alternative is to specify the dynamics of the entire curve of for ward rates. This determines the time evolution of the term structure, with the initial term structure playing the role of initial data. This sounds conceptually simple, but the model (the Heath–Jarrow–Morton model in continuous time setting) is mathematically complex. 

The literature on the subject is vast and expanding. We recommend that the reader interested in pursuing this topic should look, for example, a Pliska (1997), and Jarrow (1995) for the discrete time setting, or Bj¨ork (1998) and Chen (1996) for continuous time models. 

This page intentionally left blank 

## Chapter 1

1.1 The value of the portfolio at time 0 is 

$$
V (0) = x S (0) + y A (0) = 1, 6 0 0
$$

dollars. The value of the portfolio at time 1 will be 

$$
V (1) = x S (1) + y A (1) = \left\{ \begin{array}{l l} 1, 8 0 0 & \text { if   stock   goes   up }, \\ 1, 7 0 0 & \text { if   stock   goes   down }. \end{array} \right.
$$

Hence, the return on the portfolio will be 

$$
K _ {V} = \frac {V (1) - V (0)}{V (0)} = \left\{ \begin{array}{l l} 0. 1 2 5 0 & \text {if stock goes up,} \\ 0. 0 6 2 5 & \text {if stock goes down,} \end{array} \right.
$$

that is, either 12.5% or 6.25%. 

1.2 Given the same bond and stock prices as in Exercise 1.1, the value of a portfolio $( x , y )$ at time 1 will be 

$$
V (1) = \left\{ \begin{array}{l l} x 3 0 + y 1 0 0 & \text {if stock goes up,} \\ x 2 0 + y 1 0 0 & \text {if stock goes down.} \end{array} \right.
$$

Thus, we obtain a system of equations 

$$
\left\{ \begin{array}{l l} x 3 0 + y 1 0 0 = 1, 1 6 0, \\ x 2 0 + y 1 0 0 = 1, 0 4 0. \end{array} \right.
$$

The solution is $x = 1 2$ and $y = 8$ . A portfolio with 12 shares of stock and 8 bonds will produce the desired value at time 1. The time 0 value of this portfolio is 

$$
V (0) = 1 2 \times 2 5 + 8 \times 9 0 = 1, 0 2 0
$$

dollars. 

1.3 An arbitrage opportunity can be realised as follows: 

Use dealer A to change 1 dollar into $\textstyle { \frac { 1 } { 1 . 5 8 4 4 } } \cong 0 . 6 3 1 2$ pounds. 

Use dealer B to change 0.6312 pounds into $\frac { 0 . 6 3 1 2 } { 0 . 6 4 0 1 } \cong 0 . 9 8 6 1$ euros. 

Use dealer A to change 0.9861 euros into $0 . 9 8 \ddot { 6 } 1 \times 1 . 0 2 0 2 \cong 1 . 0 0 6 0$ dollars. 

The arbitrage gain will be about 0.0060 dollars. 

1.4 We want both xS(0) and $y A ( 0 )$ to be equal to a half of the initial wealth. This gives $x 8 0 = 5 , 0 0 0$ and $y 1 0 0 = 5$ , 000, so $x = 6 2 . 5$ and $y = 5 0$ . The value of this portfolio at time 1 will be 

$$
V (1) = 6 2. 5 S (1) + 5 0 A (1) = \left\{ \begin{array}{c l} 1 1, 7 5 0 & \text {if stock goes up,} \\ 9, 2 5 0 & \text {if stock goes down,} \end{array} \right.
$$

and hence the return on this portfolio will be 

$$
K _ {V} = \left\{ \begin{array}{r l} 0. 1 7 5 & \text { if   stock   goes   up }, \\ - 0. 0 7 5 & \text { if   stock   goes   down }. \end{array} \right.
$$

Now we can compute the expected return 

$$
E (K _ {V}) = 0. 1 7 5 \times 0. 8 - 0. 0 7 5 \times 0. 2 = 0. 1 2 5,
$$

which is 12.5%, and the risk 

$$
\sigma_ {V} = \sqrt {(0 . 1 7 5 - 0 . 1 2 5) ^ {2} \times 0 . 8 + (- 0 . 0 7 5 - 0 . 1 2 5) ^ {2} \times 0 . 2} = 0. 1,
$$

that is, 10%. 

1.5 The following strategy will realise an arbitrage opportunity. At time 0: 

Borrow $34. 

Buy a share of stock for $34. 

Enter into a short forward contract with forward price $38.60 and delivery date 1. 

At time 1: 

Sell the stock for $38.60, closing the short forward position. 

Pay $3 4 \times 1 . 1 2 = 3 8 . 0 8$ dollars to clear the loan with interest. 

The balance of $3 8 . 6 0 - 3 8 . 0 8 = 0 . 5 2$ dollars will be your arbitrage profit. 

1.6 Suppose that a sterling bond promising to pay £100 at time 1 is selling for x pounds at time 0. To find x consider the following strategy. At time 0: 

Borrow 1.6x dollars and change the sum into x pounds. 

Purchase a sterling bond for x pounds. 

Take a short forward position to sell £100 for $1.50 to a pound with delivery date 1. 

Then, at time 1: 

Cash the bond, collecting £100. 

Close the short forward position by selling £100 for $150. 

Repay the cash loan with interest, that is, 1.68x dollars in total. 

The balance of all these transactions is $1 5 0 - 1 . 6 8 x$ dollars, which must be equal to zero or else an arbitrage opportunity would arise. It follows that a sterling bond promising to pay £100 at time 1 must sell for $\textstyle x = { \frac { 1 5 0 } { 1 . 6 8 } } \cong 8 9 . 2 9$ pounds at time 0. 

1.7 a) The payof of a call option with strike price $90 will be 

$$
C (1) = \left\{ \begin{array}{c l} 3 0 & \text {if stock goes up,} \\ 0 & \text {if stock goes down.} \end{array} \right.
$$

The replicating investment into x shares and y bonds satisfies the system of equations 

$$
\left\{ \begin{array}{r l} x 1 2 0 + y 1 1 0 & = 3 0, \\ x 8 0 + y 1 1 0 & = 0. \end{array} \right.
$$

The solution is $\textstyle x = { \frac { 3 } { 4 } }$ and $\begin{array} { r } { y = - \frac { 6 } { 1 1 } } \end{array}$ . Hence the price of the option must be 

$$
C (0) = \frac {3}{4} \times 1 0 0 - \frac {6}{1 1} \times 1 0 0 \cong 2 0. 4 5
$$

dollars. 

b) The payof of a call option with strike price $110 will be 

$$
C (1) = \left\{ \begin{array}{c l} 1 0 & \text {if stock goes up,} \\ 0 & \text {if stock goes down.} \end{array} \right.
$$

The replicating investment into x shares and y bonds satisfies 

$$
\left\{ \begin{array}{r l} x 1 2 0 + y 1 1 0 & = 1 0, \\ x 8 0 + y 1 1 0 & = 0. \end{array} \right.
$$

Solving this system of equations, we find that $\textstyle x = { \frac { 1 } { 4 } }$ and $\begin{array} { r } { y = - \frac { 2 } { 1 1 } } \end{array}$ . Hence the price of the option is 

$$
C (0) = \frac {1}{4} \times 1 0 0 - \frac {2}{1 1} \times 1 0 0 \cong 6. 8 2
$$

dollars. 

1.8 a) The replicating investment into x shares and y bonds satisfies the system of equations 

$$
\left\{ \begin{array}{r l} x 1 2 0 + y 1 0 5 & = 2 0, \\ x 8 0 + y 1 0 5 & = 0, \end{array} \right.
$$

which gives $\textstyle x = { \frac { 1 } { 2 } }$ and $\begin{array} { r } { y = - \frac { 8 } { 2 1 } } \end{array}$ . Hence 

$$
C (0) = \frac {1}{2} \times 1 0 0 - \frac {8}{2 1} \times 1 0 0 \cong 1 1. 9 1
$$

dollars. 

b) In this case the replicating investment into x shares and y bonds satisfies 

$$
\left\{ \begin{array}{r l} x 1 2 0 + y 1 1 5 & = 2 0, \\ x 8 0 + y 1 1 5 & = 0, \end{array} \right.
$$

so $\begin{array} { r } { x = \frac { 1 } { 2 } } \end{array}$ and $\begin{array} { r } { y = - \frac { 8 } { 2 3 } } \end{array}$ . It follows that 

$$
C (0) = \frac {1}{2} \times 1 0 0 - \frac {8}{2 3} \times 1 0 0 \cong 1 5. 2 2
$$

dollars. 

1.9 We need to find an investment into x shares and y bonds replicating the pu option, that is, such that $x S ( 1 ) + y A ( 1 ) = P ( 1 )$ , no matter whether the stock price goes up or down. This leads to the system of equations 

$$
\left\{ \begin{array}{c} x 1 2 0 + y 1 1 0 = 0, \\ x 8 0 + y 1 1 0 = 2 0. \end{array} \right.
$$

The solution is $\begin{array} { r } { x = - \frac { 1 } { 2 } } \end{array}$ and $\begin{array} { r } { y = \frac { 6 } { 1 1 } } \end{array}$ . To replicate the put option we need to take a short position of $\textstyle { \frac { 1 } { 2 } }$ a share in stock and to buy $\frac { 6 } { 1 1 }$ of a bond. The value of this investment at time 0 is 

$$
x S (0) + y A (0) = - \frac {1}{2} \times 1 0 0 + \frac {6}{1 1} \times 1 0 0 \cong 4. 5 5
$$

dollars. By a similar argument as in Proposition 1.3, it follows that $x S ( 0 ) +$ $y A ( 0 ) = P ( 0 )$ , or else an arbitrage opportunity would arise. Therefore, the price of the put must be $P ( 0 ) \cong 4 . 5 5$ dollars. 

1.10 The investor will buy $\frac { 5 0 0 } { 1 0 0 } = 5$ shares and $\textstyle { \frac { 5 0 0 } { 1 3 . 6 3 6 4 } } \cong 3 6 . 6 6 6 7$ options. Her final wealth will then be $5 \times { \overset { \circ } { S } } ( 1 ) + 3 6 . 6 6 6 7 \times C ( { \overset { \cdot } { 1 } } )$ , that is, $5 \times 1 2 0 + 3 6 . 6 6 6 7 \times 2 0 \cong$ 1, 333.33 dollars if the price of stock goes up to $120, or $5 \times 8 0 + 3 6 . 6 6 6 7 \times 0 \cong$ 400.00 dollars if it drops to $80. 

1.11 a) If $p = 0 . 2 5$ , then the standard deviation of the return is about 52% when no option is purchased and about 26% with the option. 

b) $\mathrm { I f } \ p = 0 . 5$ , then the standard deviation of the return is about 60% and 30%, respectively. 

c) For $p = 0 . 7 5$ the standard deviation of the return is about 52% and 26%, respectively. 

1.12 The standard deviation of a random variable taking values a and b with probabilities p and $1 - p$ , respectively, is $| a - b | \sqrt { p ( 1 - p ) }$ . If no option is in-<sub>volved, then the return on stock will be 60% or 60%, depending on whether</sub> stock goes up or down. In this case $| a - b | = | 6 0 \% - ( - 6 0 \% ) | = 1 2 0 \%$ . If one option is purchased, then the return on the investment will be 35% or $- 2 5 \%$ , and $| a ^ { - } b | = | 3 5 \% - ( - 2 5 \% ) | = 6 0 \%$ . Clearly, the standard deviation $| a - b | \sqrt { p ( 1 - p ) }$ will be reduced by a half, no matter what $p$ is. 

## Chapter 2

2.1 The rate r satisfies 

$$
\left(1 + \frac {6 1}{3 6 5} \times r\right) \times 9, 0 0 0 = 9, 0 2 0.
$$

This gives $r \cong 0 . 0 1 3 3$ , that is, about 1.33%. The return on this investment will be 

$$
K (0, \frac {6 1}{3 6 5}) = \frac {9 , 0 2 0 - 9 , 0 0 0}{9 , 0 0 0} \cong 0. 0 0 2 2,
$$

that is, about 0.22%. 

2.2 Denote the amount to be paid today by P. Then the return will be 

$$
\frac {1 , 0 0 0 - P}{P} = 0. 0 2.
$$

The solution is $P \cong 9 8 0 . 3 9$ dollars. 

## 2.3 The time t satisfies

$$
(1 + t \times 0. 0 9) \times 8 0 0 = 8 3 0,
$$

which gives $t \cong 0 . 4 1 6 7$ years, that is, $0 . 4 1 6 7 \times 3 6 5 \cong 1 5 2 . 0 8$ days. The return will be 

$$
K (0, t) = \frac {8 3 0 - 8 0 0}{8 0 0} = 0. 0 3 7 5,
$$

that is, 3.75%. 

2.4 The principal P to be invested satisfies 

$$
\left(1 + \frac {9 1}{3 6 5} \times 0. 0 8\right) \times P = 1, 0 0 0,
$$

which gives P ∼= 980.44 dollars. 

2.5 The time t when the future value will be double the initial principal satisfies the equation 

$$
\left(1 + \frac {0 . 0 6}{3 6 5}\right) ^ {3 6 5 t} = 2.
$$

The solution is $t \cong 1 1 . 5 5 3 4$ years. Because no interest will be paid for a fraction of the last day, this needs to be rounded up to a whole number of days, which gives 11 years and 202 days. (We disregard leap years and assume for simplicity that each year has 365 days.) 

2.6 The interest rate r satisfies the equation 

$$
(1 + r) ^ {1 0} = 2,
$$

which gives $r \cong 0 . 0 7 1 8$ , that is, about 7.18%. 

2.7 a) In the case of annual compounding the value after two years will be 

$$
V (2) = \left(1 + \frac {0 . 1}{1}\right) ^ {2 \times 1} 1 0 0 = 1 2 1. 0 0
$$

dollars. 

b) Under semi-annual compounding the value will be 

$$
V (2) = \left(1 + \frac {0 . 1}{2}\right) ^ {2 \times 2} 1 0 0 \cong 1 2 1. 5 5
$$

dollars, which is clearly greater than in case a). 

2.8 At 15% compounded daily the deposit will grow to 

$$
\left(1 + \frac {0 . 1 5}{3 6 5}\right) ^ {1 \times 3 6 5} 1, 0 0 0 \cong 1, 1 6 1. 8 0
$$

dollars after one year. If interest is compounded semi-annually at 15.5%, the value after one year will be 

$$
\left(1 + \frac {0 . 1 5 5}{2}\right) ^ {1 \times 2} 1, 0 0 0 \cong 1, 1 6 1. 0 1
$$

dollars, which is less than in the former case. 

2.9 The initial principal P satisfies the equation 

$$
(1 + 0. 1 2) ^ {2} P = 1, 0 0 0.
$$

It follows that $P \cong 7 9 7 . 1 9$ dollars. 

2.10 a) Under daily compounding the present value is 

$$
1 0 0, 0 0 0 \left(1 + \frac {0 . 0 5}{3 6 5}\right) ^ {- 1 0 0 \times 3 6 5} \cong 6 7 4. 0 3
$$

dollars. 

b) If annual compounding applies, then the present value is 

$$
1 0 0, 0 0 0 (1 + 0. 0 5) ^ {- 1 0 0} \cong 7 6 0. 4 5
$$

dollars. 

2.11 The return will be 

$$
K (0, 1) = \left(1 + \frac {0 . 1}{1 2}\right) ^ {1 2} - 1 \cong 0. 1 0 4 7,
$$

that is, about 10.47%. 

2.12 Using the binomial formula to expand the mth power, we obtain 

$$
\begin{array}{l} K (0, 1) = (1 + \frac {r}{m}) ^ {m} - 1 \\ \qquad = 1 + r + \frac {(1 - \frac {1}{m})}{2 !} r ^ {2} + \dots + \frac {(1 - \frac {m - 1}{m})}{m !} r ^ {m} - 1 > r \end{array}
$$

if m is an integer greater than 1. 

2.13 Denote the interest rate by r, the amount borrowed by $P$ and the amount of each instalment by C, 

$$
C = \frac {P}{\mathrm{PA} (r , 5)} = \frac {P r}{1 - (1 + r) ^ {- 5}},
$$

see Example 2.4. Let $n = 1$ , 2, 3, 4 or 5. The present value of the outstanding balance after $n - 1$ instalments are paid is equal to the amount borrowed reduced by the present value of the first $n - 1$ instalments: 

$$
P - \frac {C}{1 + r} - \dots - \frac {C}{(1 + r) ^ {n - 1}} = P \frac {(1 + r) ^ {6 - n} - 1}{(1 + r) ^ {5} - 1}.
$$

The actual outstanding balance remaining after $n - 1$ instalments are paid can be found by dividing the above by the discount factor $( 1 + r ) ^ { - ( n - 1 ) }$ , which gives 

$$
P \frac {(1 + r) ^ {5} - (1 + r) ^ {n - 1}}{(1 + r) ^ {5} - 1}.\tag{S.1}
$$

The interest included in the nth instalment is, therefore, 

$$
P \frac {(1 + r) ^ {5} - (1 + r) ^ {n - 1}}{(1 + r) ^ {5} - 1} r.\tag{S.2}
$$

The capital repaid as part of the nth instalment is the diference between the outstanding balance of the loan after the $( n - 1 )$ )st and after the nth instalment. By (S.1) this diference is equal to 

$$
P \frac {(1 + r) ^ {n} - (1 + r) ^ {n - 1}}{(1 + r) ^ {5} - 1} = P \frac {r (1 + r) ^ {n - 1}}{(1 + r) ^ {5} - 1}.\tag{S.3}
$$

Putting P to be $1, 000 and r to be 15% in (S.1), (S.2) and (S.3), we can compute the figures collected in the table: 

<table><tr><td>t (years)</td><td>interest paid ($)</td><td>capital repaid ($)</td><td>outstanding balance ($)</td></tr><tr><td>0</td><td>—</td><td>—</td><td>1,000.00</td></tr><tr><td>1</td><td>150.00</td><td>148.32</td><td>851.68</td></tr><tr><td>2</td><td>127.75</td><td>170.56</td><td>681.12</td></tr><tr><td>3</td><td>102.17</td><td>196.15</td><td>484.97</td></tr><tr><td>4</td><td>72.75</td><td>225.57</td><td>259.40</td></tr><tr><td>5</td><td>38.91</td><td>259.40</td><td>0.00</td></tr></table>

2.14 The amount you can aford to borrow is 

$$
\mathrm{PA} (18\%, 10) \times 10,000 = \frac {1 - (1 + 0.18)^{-10}}{0.18} \times 10,000 \cong 44,941
$$

dollars. 

2.15 The present value of the balance after 40 years is 

$$
\mathrm{PA} (5 \%, 4 0) \times 1, 2 0 0 = \frac {1 - (1 + 0 . 0 5) ^ {- 4 0}}{0 . 0 5} \times 1, 2 0 0 \cong 2 0, 5 9 1
$$

dollars. Dividing by the discount factor $( 1 + 0 . 0 5 ) ^ { - 4 0 }$ , we find that the actual balance after 40 years will be 

$$
\frac {2 0 , 5 9 1}{(1 + 0 . 0 5) ^ {- 4 0}} \cong 1 4 4, 9 6 0
$$

dollars. 

2.16 The annual payments will amount to 

$$
C = \frac {1 0 0 , 0 0 0}{P A (6 \%, 1 0)} \cong 1 3, 5 8 6. 8 0
$$

dollars each. The outstanding balance to be paid to clear the mortgage after 8 years (once the 8th annual payment is made) will be 

$$
\mathrm{PA} (6 \%, 2) \times C \cong 24,909.93
$$

dollars. 

2.17 Suppose that payments $C , C ( 1 + g ) , C ( 1 + g ) ^ { 2 } , . .$ . are made after 1 year, 2 years, 3 years, and so on. If the interest rate is constant and equal to $r ,$ then the present values of these payments are $C \left( 1 + r \right) ^ { - 1 } , C ( 1 + \dot { g } ) \left( 1 + r \right) ^ { - 2 } , C ( 1 +$ $g ) ^ { 2 } \left( 1 + r \right) ^ { - 3 } , \ldots .$ . The present value of the infinite stream of payments is, therefore, 

$$
{\frac {C}{1 + r}} + {\frac {C (1 + g)}{(1 + r) ^ {2}}} + {\frac {C (1 + g) ^ {2}}{(1 + r) ^ {3}}} + \ldots = {\frac {C}{r - g}}.
$$

The condition $g < r$ must be satisfied or otherwise the series will be divergent. Using this formula and the tail-cutting procedure, we can find that for a stream of n payments 

$$
{\frac {C}{r - g}} - {\frac {C (1 + g) ^ {n}}{r - g}} {\frac {1}{(1 + r) ^ {n}}} = C {\frac {1 - \left({\frac {1 + g}{1 + r}}\right) ^ {n}}{r - g}}.
$$

2.18 The time t it will take to earn $1 in interest satisfies 

$$
\mathrm{e} ^ {0. 1 t} \times 1, 0 0 0, 0 0 0 \cong 1, 0 0 0, 0 0 1.
$$

This gives $t \cong 0 . 0 0 0 0 1$ years, that is, 315.36 seconds. 

2.19 a) The value in year 2000 of the sum of $24 for which Manhattan was bough in 1626 would be 

$$
2 4 \mathrm{e} ^ {(2 0 0 0 - 1 6 2 6) \times 0. 0 5} \cong 3, 1 7 3, 3 5 0, 5 7 5
$$

dollars, assuming continuous compounding at $5 \%$ 

b) The same amount compounded at 5% annually would be worth 

$$
2 4 (1 + 0. 0 5) ^ {2 0 0 0 - 1 6 2 6} \cong 2, 0 1 8, 4 0 8, 6 2 8
$$

dollars in year 2000. 

2.20 $100 deposited at 10% compounded continuously will become 

$$
1 0 0 \mathrm{e} ^ {0. 1} \cong 1 1 0. 5 2
$$

dollars after one year. The same amount deposited at 10% compounded monthly will become 

$$
1 0 0 \left(1 + \frac {0 . 1}{1 2}\right) ^ {1 2} \cong 1 1 0. 4 7
$$

dollars. The diference is about $0.05. 

If the diference is to be less than $0.01, the compounding frequency m should satisfy 

$$
1 0 0 \left(1 + \frac {0 . 1}{m}\right) ^ {m} > 1 1 0. 5 1.
$$

This means that m should be greater than about 55.19. 

2.21 The present value is 

$$
1, 0 0 0, 0 0 0 \mathrm{e} ^ {- 2 0 \times 0. 0 6} \cong 3 0 1, 1 9 4
$$

dollars. 

2.22 The rate r satisfies 

$$
9 5 0 \mathrm{e} ^ {0. 5 r} = 1, 0 0 0.
$$

It follows that 

$$
r = \frac {1}{0 . 5} \ln \frac {1 , 0 0 0}{9 5 0} \cong 0. 1 0 2 6,
$$

that is, about 10.26%. 

2.23 The interest rate is 

$$
r = \frac {0 . 0 3}{2 / 1 2} = 0. 1 8,
$$

that is, 18%. 

2.24 The rate r satisfies 

$$
\mathrm{e} ^ {r} = \left(1 + \frac {0 . 1 2}{1 2}\right) ^ {1 2}.
$$

The solution is $r \cong 0 . 1 1 9 4$ , about 11.94%. 

2.25 The frequency m satisfies 

$$
\left(1 + \frac {0 . 2}{m}\right) ^ {m} = 1 + 0. 2 1.
$$

Whence $m = 2 . 0$ 

2.26 If monthly compounding at a rate r applies, then $\begin{array} { r } { \left( 1 + \frac { r } { 1 2 } \right) ^ { 1 2 } = 1 + r _ { \mathrm { e } } } \end{array}$ and the present value of the annuity is 

$$
\begin{array}{l} V (0) = \frac {C}{1 + \frac {r}{1 2}} + \frac {C}{\left(1 + \frac {r}{1 2}\right) ^ {2}} + \dots + \frac {C}{\left(1 + \frac {r}{1 2}\right) ^ {1 2 n}} \\ \qquad = \frac {C}{\left(1 + r _ {\mathrm{e}}\right) ^ {1 / 1 2}} + \frac {C}{\left(1 + r _ {\mathrm{e}}\right) ^ {2 / 1 2}} + \dots + \frac {C}{\left(1 + r _ {\mathrm{e}}\right) ^ {n}} \\ \qquad = C \frac {1 - \left(1 + r _ {\mathrm{e}}\right) ^ {- n}}{\left(1 + r _ {\mathrm{e}}\right) ^ {1 / 1 2} - 1}. \end{array}
$$

2.27 If bimonthly compounding at a rate r applies, then $\textstyle \left( 1 + { \frac { r } { 6 } } \right) ^ { 6 } = 1 + r _ { \mathrm { e } }$ and the present value of the perpetuity is 

$$
\begin{array}{l} V (0) = \frac {C}{1 + \frac {r}{6}} + \frac {C}{\left(1 + \frac {r}{6}\right) ^ {2}} + \frac {C}{\left(1 + \frac {r}{6}\right) ^ {3}} + \dots \\ \qquad = \frac {C}{\left(1 + r _ {\mathrm{e}}\right) ^ {1 / 6}} + \frac {C}{\left(1 + r _ {\mathrm{e}}\right) ^ {2 / 6}} + \frac {C}{\left(1 + r _ {\mathrm{e}}\right) ^ {3 / 6}} + \dots \\ \qquad = C \frac {1}{\left(1 + r _ {\mathrm{e}}\right) ^ {1 / 6} - 1}. \end{array}
$$

2.28 We solve the equation 

$$
1 0 0 = 9 5 (1 + r) ^ {\frac {1}{2}}
$$

for $r$ to find the implied efective rate to be about 10.80%. If this rate remains constant, then the bond price will reach $99 at a time t such that 

$$
1 0 0 = 9 9 (1 + r) ^ {\left(\frac {1}{2} - t\right)}.
$$

The solution is $t \cong 0 . 4 0 2$ years, that is, about $0 . 4 0 2 \times 3 6 5 \cong 1 4 6 . 7 3$ days. The bond price will reach $99 on day 147. 

2.29 The interest rate for annual compounding implied by the bond can be found by solving the equation 

$$
(1 + r) ^ {- (1 - 0. 5)} = 0. 9 4 5 5
$$

for $r _ { \cdot }$ . The solution is about 11.86%. By solving the equation 

$$
\left(1 + \frac {r}{2}\right) ^ {- 2 (1 - 0. 5)} = 0. 9 4 5 5,
$$

we obtain the semi-annual rate of about 11.53%, and solving 

$$
\mathrm{e} ^ {- r (1 - 0. 5)} = 0. 9 4 5 5,
$$

we find the continuous rate to be about 11.21%. 

2.30 a) If the continuous compounding rate is 8%, then the price of the bond will be 

$$
5 \mathrm{e} ^ {- 0. 0 8} + 5 \mathrm{e} ^ {- 2 \times 0. 0 8} + 5 \mathrm{e} ^ {- 3 \times 0. 0 8} + 1 0 5 \mathrm{e} ^ {- 4 \times 0. 0 8} \cong 8 9. 0 6
$$

dollars. 

b) If the rate is 5%, then the price of the bond will be 

$$
5 \mathrm{e} ^ {- 0. 0 5} + 5 \mathrm{e} ^ {- 2 \times 0. 0 5} + 5 \mathrm{e} ^ {- 3 \times 0. 0 5} + 1 0 5 \mathrm{e} ^ {- 4 \times 0. 0 5} \cong 9 9. 5 5
$$

dollars. 

2.31 The price of the bond as a function of the continuous compounding rate r can be expressed as $\mathrm { 5 e } ^ { - r } + \mathrm { 5 e } ^ { - 2 r } + \mathrm { 5 e } ^ { - 3 r } + 1 0 5 \mathrm { e } ^ { - 4 r }$ . The graph of this function is shown in Figure S.1. When $r \searrow 0$ , the price approaches $5 + 5 + 5 + 1 0 5 = 1 2 0$ dollars. In the limit as $r \nearrow \infty$ the price tends to zero. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/63cf03214b234fc57ffd3f16c94a1f6e1c658e5dc982733822c4166d467361eb.jpg)



Figure S.1 Bond price versus interest rate in Exercise 2.31


2.32 The time t price of the coupon bond in Examples 2.9 and 2.10 is 

$$
\begin{array}{r l} 1 0 \mathrm{e} ^ {r (t - 1)} + 1 0 \mathrm{e} ^ {r (t - 2)} + 1 0 \mathrm{e} ^ {r (t - 3)} + 1 0 \mathrm{e} ^ {r (t - 4)} + 1 1 0 \mathrm{e} ^ {r (t - 5)} & \text {if} \quad 0 \leq t <   1, \\ 1 0 \mathrm{e} ^ {r (t - 2)} + 1 0 \mathrm{e} ^ {r (t - 3)} + 1 0 \mathrm{e} ^ {r (t - 4)} + 1 1 0 \mathrm{e} ^ {r (t - 5)} & \text {if} \quad 1 \leq t <   2, \\ 1 0 \mathrm{e} ^ {r (t - 3)} + 1 0 \mathrm{e} ^ {r (t - 4)} + 1 1 0 \mathrm{e} ^ {r (t - 5)} & \text {if} \quad 2 \leq t <   3, \\ 1 0 \mathrm{e} ^ {r (t - 4)} + 1 1 0 \mathrm{e} ^ {r (t - 5)} & \text {if} \quad 3 \leq t <   4, \\ 1 1 0 \mathrm{e} ^ {r (t - 5)} & \text {if} \quad 4 \leq t <   5. \end{array}
$$

The graph is shown in Figure S.2. 

2.33 In Figure S.2 we can see that the bond price will reach $95 for the first time during year one, when the bond price is given by $1 0 \mathrm { e } ^ { r ( t - 1 ) } + 1 0 \mathrm { e } ^ { r ( t - 2 ) } + 1 0 \mathrm { e } ^ { r ( t - 3 ) } +$ $1 0 \mathrm { { e } } ^ { r ( t - 4 ) } + \mathrm { { i } } 1 0 \mathrm { { e } } ^ { r ( t - 5 ) }$ . Putting $r = 0 . 1 2$ , we can find the desired time t when the price will reach $95 by solving the equation 

$$
1 0 \mathrm{e} ^ {r (t - 1)} + 1 0 \mathrm{e} ^ {r (t - 2)} + 1 0 \mathrm{e} ^ {r (t - 3)} + 1 0 \mathrm{e} ^ {r (t - 4)} + 1 1 0 \mathrm{e} ^ {r (t - 5)} = 9 5.
$$

This gives $t \cong 0$ .4257 years or 155.4 days. 

2.34 Since the bond is trading at par, its initial price is the same as the face value $F = 1 0 0$ . The implied continuous compounding rate r can be found by solving the equation 

$$
8 \mathrm{e} ^ {- r} + 8 \mathrm{e} ^ {- 2 r} + 1 0 8 \mathrm{e} ^ {- 3 r} = 1 0 0.
$$

This gives $r \cong 0 . 0 7 7 0$ or 7.70%. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/9d106ddaa8ca41df7efeda284c7352e025b56786e1d8271b272617dea15bc42e.jpg)



Figure S.2 Coupon bond price versus time in Exercise 2.32


## 2.35 By solving the equation

$$
(1 + r) ^ {- 1} = 0. 8 9
$$

we find that $r \cong 0 . 1 2 3 6$ , that is, the efective rate implied by the bond is about 12.36%. The price of the bond after 75 days will be 

$$
B (7 5 / 3 6 5, 1) = B (0, 1) (1 + r) ^ {\frac {7 5}{3 6 5}} = 0. 8 9 (1 + 0. 1 2 3 6) ^ {\frac {7 5}{3 6 5}} \cong 0. 9 1 1 5
$$

and the return will be 

$$
K (0, 7 5 / 3 6 5) = \frac {B (7 5 / 3 6 5 , 1) - B (0 , 1)}{B (0 , 1)} \cong \frac {0 . 9 1 1 5 - 0 . 8 9}{0 . 8 9} \cong 0. 0 2 4 2,
$$

about 2.42%. 

2.36 The initial price of a six-month unit bond is $\mathrm { e } ^ { - 0 . 5 r }$ , where r denotes the implied continuous rate. If the bond is to produce a 7% return over six months, then 

$$
\frac {1 - \mathrm{e} ^ {- 0 . 5 r}}{\mathrm{e} ^ {- 0 . 5 r}} = 0. 0 7,
$$

which gives $r \cong 0 . 1 3 5 3$ , or 13.53%. 

2.37 The continuous rate implied by the bond satisfies 

$$
\mathrm{e} ^ {- r} = 0. 9 2.
$$

The solution is $r \cong 0 . 0 8 3 4$ . At time t the bond will be worth $0 . 9 2 \mathrm { e } ^ { r t }$ . It will produce a 5% return at a time t such that 

$$
\frac {0 . 9 2 \mathrm{e} ^ {r t} - 0 . 9 2}{0 . 9 2} = 0. 0 5,
$$

which gives $t \cong 0 . 5 8 5 1$ years or 213.6 days. 

2.38 At time 0 we buy $1 / B ( 0 , 1 ) = \mathbf { e } ^ { r }$ bonds, at time 1 we increase our holdings to $\mathrm { e } ^ { r } / B ( 1 , 2 ) = \mathrm { e } ^ { 2 r }$ bonds, and generally at time n we purchase $\mathrm { e } ^ { ( n + 1 ) r }$ one-year bonds. 

2.39 Because the bond is trading at par and the interest rates remain constant, the price of the bond at the beginning of each year will be $100. The sum of $1, 000 will buy 10 bonds at the beginning of year one. At the end of the year the coupons will pay $1 0 \times 8 = 8 0$ dollars, enough to buy 0.8 bonds at $100 each. As a result, the investor will be holding $1 \bar { 0 } + 0 . 8 \overset { \cdot } { = } 1 0 . 8$ bonds in year two. At the end of that year the coupons will pay $1 0 . 8 \times 8 = 8 6 . 4$ dollars and 0.864 additional bonds will be purchased at $100 each. The number of bonds held in year three will be $1 0 . 8 \dot { + } 0 . 8 6 4 = 1 1 . 6 6 4$ , and so on. 

In general, the number of bonds held in year n will be 

$$
1 0 \left(1 + \frac {8}{1 0 0}\right) ^ {n - 1},
$$

which gives 10.0000, 10.8000, 11.6640, 12.5971, 13.6049 bonds held in years one to five. 

## Chapter 3

3.1 The tree representing the scenarios and price movements in Example 3.1 is shown in Figure S.3. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/3bb4576ae89f26a1933ed81f079aec23469b498997f9d39f968166ebf1ea58b3.jpg)



Figure S.3 Tree of price movements in Example 3.1


3.2 The tree representing the scenarios and price movements is shown in Fig ure S.4. There are altogether eight scenarios represented by the paths through the tree leading from the ‘root’ on the left towards the rightmost branch tips. 


3.3 We can use (3.1) to find


<table><tr><td>Scenario</td><td><eq>S(0)</eq></td><td><eq>S(1)</eq></td><td><eq>S(2)</eq></td><td><eq>S(3)</eq></td></tr><tr><td><eq>\omega_1</eq></td><td>45.00</td><td>49.50</td><td>51.98</td><td>46.78</td></tr><tr><td><eq>\omega_2</eq></td><td>45.00</td><td>47.25</td><td>51.98</td><td>57.17</td></tr><tr><td><eq>\omega_3</eq></td><td>45.00</td><td>47.25</td><td>42.53</td><td>46.78</td></tr></table>

The tree is shown in Figure S.5. 

3.4 When dividends are payable, formula (3.1) becomes 

$$
S (n) = S (n - 1) (1 + K (n)) - \operatorname{div} (n),
$$

which gives 

<table><tr><td>Scenario</td><td><eq>S(0)</eq></td><td><eq>S(1)</eq></td><td><eq>S(2)</eq></td><td><eq>S(3)</eq></td></tr><tr><td><eq>\omega_1</eq></td><td>45.00</td><td>48.50</td><td>49.93</td><td>43.93</td></tr><tr><td><eq>\omega_2</eq></td><td>45.00</td><td>46.25</td><td>49.88</td><td>53.86</td></tr><tr><td><eq>\omega_3</eq></td><td>45.00</td><td>46.25</td><td>40.63</td><td>43.69</td></tr></table>

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/520ae8de5ead89b2657e7877731a2a9423b83669e66315f5ec04b94f896e5c46.jpg)



Figure S.4 Tree of price movements in Exercise 3.2


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/b86b05403cb8fdd776bb521b5c94c99e6ddbe3cb594efe523def8c210300ba10.jpg)



Figure S.5 Tree of price movements in Exercise 3.3


3.5 The return over two time steps as compared to the sum of one-step returns can take the following values: 

<table><tr><td>Scenario</td><td><eq>K(0,2)</eq></td><td><eq>K(1)+K(2)</eq></td></tr><tr><td><eq>\omega_1</eq></td><td>15.50%</td><td>15.00%</td></tr><tr><td><eq>\omega_2</eq></td><td>15.50%</td><td>15.00%</td></tr><tr><td><eq>\omega_3</eq></td><td>-5.50%</td><td>-5.00%</td></tr></table>

Over three time steps we have 

$$
\begin{array}{c c c} \text {Scenario} & K (0, 3) & K (1) + K (2) + K (3) \\ \omega_ {1} & 3.95\% & 5.00\% \\ \omega_ {2} & 27.05\% & 25.00\% \\ \omega_ {3} & 3.95\% & 5.00\% \end{array}
$$

The sum of one-step returns tends to be larger then the return over the total interval if the sign of one-step returns alternates. 

3.6 First find $K ( 0 , 2 )$ and then the one-step returns $K ( 1 ) = K ( 2 ) = K$ from the 

relation $1 + K ( 0 , 2 ) = ( 1 + K ) ^ { 2 } $ (assuming that $1 + K > 0 )$ : 

$$
\begin{array}{c c c} \text {Scenario} & K (0, 2) & K (1) = K (2) \\ \omega_ {1} & 17.14\% & 8.23\% \\ \omega_ {2} & -8.57\% & -4.38\% \\ \omega_ {3} & -20.00\% & -10.56\% \end{array}
$$

## 3.7 The formula

$$
1 + K (0, 2) = (1 + K (1)) (1 + K (2))
$$

can be used to find K(2). For example, the following scenarios and values of K(2) are consistent with the conditions of Exercise 3.7: 

<table><tr><td>Scenario</td><td><eq>K(0,2)</eq></td><td><eq>K(1)</eq></td><td><eq>K(2)</eq></td></tr><tr><td><eq>\omega_{1}</eq></td><td>21.00%</td><td>10.00%</td><td>10.00%</td></tr><tr><td><eq>\omega_{2}</eq></td><td>10.00%</td><td>10.00%</td><td>0.00%</td></tr><tr><td><eq>\omega_{3}</eq></td><td>-1.00%</td><td>-10.00%</td><td>10.00%</td></tr></table>

This is not the only possible solution. Another one can be obtained from the above by changing scenario $\omega _ { 2 }$ to 

$$
\begin{array}{c c c c} \text {Scenario} & K (0, 2) & K (1) & K (2) \\ \omega_ {2} & 10.00\% & -10.00\% & 22.22\% \end{array}
$$

with the other two scenarios unaltered. 

3.8 For the three scenarios in Example 3.2 we find 

$$
\begin{array}{cccc} \text{Scenario} & k(1) & k(2) & k(0,2)\\ \omega_{1} & 5.31\% & 3.39\% & 8.70\% \\ \omega_{2} & 5.31\% & -10.92\% & -5.61\% \\ \omega_{3} & -5.61\% & 1.90\% & -3.70\% \end{array}
$$

In all three cases $k ( 0 , 2 ) = k ( 1 ) + k ( 2 )$ 

3.9 Let K denote the return in the third scenario. If the expected return is equal to 6%, then 

$$
\frac {1}{2} \times (- 5 \%) + \frac {1}{4} \times 6 \% + \frac {1}{4} \times K = 6 \%.
$$

Solving for K, we find that the return in the third scenario must be 28%. 

3.10 First, compute the returns K(1), K(2) and $K ( 0 , 2 )$ in each scenario: 

<table><tr><td>Scenario</td><td><eq>K(1)</eq></td><td><eq>K(2)</eq></td><td><eq>K(0,2)</eq></td></tr><tr><td><eq>\omega_{1}</eq></td><td>10.00%</td><td>9.09%</td><td>20.00%</td></tr><tr><td><eq>\omega_{2}</eq></td><td>5.00%</td><td>-4.76%</td><td>0.00%</td></tr><tr><td><eq>\omega_{3}</eq></td><td>-10.00%</td><td>11.11%</td><td>0.00%</td></tr></table>

It follows that 

$$
E (K (1)) \cong 0. 2 5 \times 1 0. 0 0 \% + 0. 2 5 \times 5. 0 0 \% - 0. 5 \times 1 0. 0 0 \% \cong - 1. 2 5 \%,
$$

$$
E (K (2)) \cong 0. 2 5 \times 9. 0 9 \% - 0. 2 5 \times 4. 7 6 \% + 0. 5 \times 1 1. 1 1 \% \cong 6. 6 4 \%,
$$

$$
E (K (0, 2)) \cong 0. 2 5 \times 2 0. 0 0 \% + 0. 2 5 \times 0. 0 0 \% + 0. 5 \times 0. 0 0 \% \cong 5. 0 0 \%.
$$

Clearly, 

$$
(1 + E (K (1))) (1 + E (K (2))) \cong 1. 0 5 3 0 \neq 1. 0 5 0 0 \cong 1 + E (K (0, 2)).
$$

3.11 Since the quarterly returns $K ( 1 ) , K ( 2 ) , K ( 3 ) , K ( 4 )$ are independent and iden tically distributed, 

$$
E (K (1)) = E (K (2)) = E (K (3)) = E (K (4))
$$

and 

$$
\begin{array}{l} 1 + E (K (0, 3)) = (1 + E (K (1)) ^ {3}, \\ 1 + E (K (0, 4)) = (1 + E (K (1)) ^ {4}. \end{array}
$$

Thus, if $E ( K ( 0 , 3 ) ) = 1 2 \%$ , then the expected quarterly return $E ( K ( 1 ) ) \cong$ 3.85% and the expected annual return $E \big ( K ( 0 , 4 ) \big ) \cong 1 6 . \dot { 3 } 1 \%$ 

3.12 By Condition 3.1 the random variables 

$$
\frac {S (1)}{S (0)} = 1 + K (1), \quad \frac {S (2)}{S (1)} = 1 + K (2), \quad \frac {S (3)}{S (2)} = 1 + K (3)\tag{S.4}
$$

are independent, each taking two values $1 + d$ and $_ { 1 + u }$ with probabilities $p$ and $1 - p ,$ respectively. 

The price $S ( 2 )$ , which is the product of $S ( 0 )$ and the first two of these random variables, takes up to four values corresponding to the four price movement scenarios, that is, paths through the two-step tree of stock prices shown in Figure 3.3 (in which $S ( 0 ) = 1 $ for simplicity). Among these four values of $S ( 2 )$ there are in fact only three diferent ones, 

$$
S (2) = \left\{ \begin{array}{l l} S (0) (1 + u) ^ {2} & \text { with   probability } p ^ {2}, \\ S (0) (1 + u) (1 + d) & \text { with   probability } 2 p (1 - p), \\ S (0) (1 + d) ^ {2} & \text { with   probability } (1 - p) ^ {2}. \end{array} \right.
$$

The price $S ( 3 )$ , which is the product of $S ( 0 )$ and the three independent random variables in (S.4), takes up to eight values corresponding to the eight price movement scenarios, that is, paths through the three-step tree of stock prices in Figure 3.4 (with $S ( 0 ) = 1$ for simplicity). Among these eight values of S(3) there are only four diferent ones, 

$$
S (3) = \left\{ \begin{array}{l l} S (0) (1 + u) ^ {3} & \text {with probability p^{3}}, \\ S (0) (1 + u) ^ {2} (1 + d) & \text {with probability 3p^{2}} (1 - p), \\ S (0) (1 + u) (1 + d) ^ {2} & \text {with probability 3p(1 - p)^{2}}, \\ S (0) (1 + d) ^ {3} & \text {with probability (1 - p)^{3}}. \end{array} \right.
$$

3.13 The top values of S(1) and S(2) can be used to find u: 

$$
u = \frac {9 2 - 8 7}{8 7} \cong 0. 0 5 7 5.
$$

Next, u and the top value of S(1) give the value of $S ( 0 )$ : 

$$
S (0) \cong \frac {8 7}{1 + 0 . 0 5 7 5} \cong 8 2. 2 7
$$

dollars. Finally, d is determined by S(0) and the bottom value of $S ( 1 )$ 

$$
d \cong \frac {7 6 - 8 2 . 2 7}{8 2 . 2 7} \cong - 0. 0 7 6 2.
$$

3.14 Given the continuous risk-free rate of $1 4 \%$ and the time step $\tau = 1 / 1 2$ , we find the one-step return 

$$
r = \mathrm{e} ^ {0. 1 4 / 1 2} - 1 \cong 0. 0 1 1 7.
$$

By Condition 3.2, $u > r \cong 0 . 0 1 1 7 .$ . This means that the middle value $S ( 0 ) ( 1 +$ $u ) ( 1 + d )$ of $S ( 2 )$ must be no less than about $2 2 ( 1 + 0 . 0 1 1 7 ) ( 1 - 0 . 0 1 ) \tilde { \cong } 2 2 . 0 4$ dollars. 

3.15 Consider the system of equations 

$$
\begin{array}{r} S (0) (1 + u) ^ {2} = 3 2, \\ S (0) (1 + u) (1 + d) = 2 8, \\ S (0) (1 + d) ^ {2} = x. \end{array}
$$

It follows that 

$$
\frac {3 2}{2 8} = \frac {1 + u}{1 + d} = \frac {2 8}{x}
$$

and $x = 2 8 ^ { 2 } / 3 2 = 2 4 . 5 0$ dollars. However, the tree cannot be reconstructed uniquely. For any value $S ( 0 ) > 0$ one can find u and d consistent with the data. 

3.16 The values of u and d can be found by solving the equations 

$$
\begin{array}{r} S (0) (1 + u) ^ {2} = 1 2 1, \\ S (0) (1 + d) ^ {2} = 1 0 0, \end{array}
$$

and selecting those solutions that satisfy 1+u > 0 and $1 + d > 0$ . If $S ( 0 ) = 1 0 0$ , then $u = 0 . 1$ and $d = 0$ . If $S ( 0 ) = 1 0 4$ , then $u \cong 0 . 0 7 8 6$ and $d \cong - 0 . 0 1 9 4$ 

3.17 We only need to consider the values of d between 1 and r, that is, $- 1 < d <$ $1 / 1 0 . { \dot { \mathrm { A s } } }$ d increases between these two bounds, $p _ { * }$ decreases from 11/13 to 0. The dependence of $p _ { * }$ on d is shown in Figure S.6. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/d911791a116f37d60a4c300d6d4d0465a240b73e15b6535abf80a1bdf7807433.jpg)



Figure S.6 The risk-neural probability $p _ { * }$ as a function of d


3.18 By (3.4) the condition d $< r < u$ is equivalent to d $< p _ { * } u + ( 1 - p _ { * } ) d < u$ . This, in turn, can be written as $0 < p _ { * } ( u - d ) < u -$ d or, equivalently, $0 < p _ { * } < 1$ 3.19 By Proposition 3.5 

$$
E _ {*} (S (3) | S (2) = 1 1 0) = 1 1 0 (1 + r) = 1 1 0 (1 + 0. 2) = 1 3 2
$$

dollars. 

3.20 By Condition 3.3 the random variables $S ( 1 ) / S ( 0 ) = 1 + K ( 1 )$ and $S ( 2 ) / S ( 1 ) =$ $1 + K ( 2 )$ are independent, each taking three values $1 + d , 1 + n$ and $_ { 1 + u }$ with probabilities $p , \ q$ and $1 - p - q ,$ , respectively. Therefore $S ( 2 )$ , which is the product of these two random variables and the number $S ( 0 )$ , takes up to nine values. Among these nine values there are only six diferent ones, 

$$
S (2) = \left\{ \begin{array}{l l} S (0) (1 + u) ^ {2} & \text {with probability p^{2}}, \\ S (0) (1 + n) ^ {2} & \text {with probability q^{2}}, \\ S (0) (1 + d) ^ {2} & \text {with probability (1 - p - q)^{2}}, \\ S (0) (1 + u) (1 + n) & \text {with probability 2pq}, \\ S (0) (1 + u) (1 + d) & \text {with probability 2p(1 - p - q)}, \\ S (0) (1 + n) (1 + d) & \text {with probability 2q(1 - p - q)}. \end{array} \right.
$$

3.21 Let $p _ { * } , q _ { * } , 1 - p _ { * } - q _ { * }$ be the probabilities of upward, middle and downward price movements, respectively. Condition (3.6) implies that $0 . 2 p _ { * } - 0 . 1 ( 1 - p _ { * } - q _ { * } ) =$ 0, that is, $q _ { * } = 1 \_ 3 p .$ and $1 - p _ { * } - q _ { * } = 2 p _ { * }$ . Observe that $p _ { * } , 1 - 3 p _ { * } , 2 p _ { * } \in [ 0 , 1 ]$ if and only if $p _ { * } \in [ 0 , 1 / 3 ]$ . It follows that $p _ { * } , q _ { * } , 1 - p _ { * } - q \mathopen { }$ are risk-neutral probabilities if and only if $q _ { * } = 1 - 3 p$ p and $p _ { * } \in [ 0 , 1 / 3 ]$ 

3.22 Solving the system of equations 

$$
\begin{array}{r} \ln (1 + u) = m \tau + \sigma \sqrt {\tau}, \\ \ln (1 + d) = m \tau - \sigma \sqrt {\tau}, \end{array}
$$

we find $\sigma \cong 0 . 0 5 2$ and $m \cong 0 . 0 5 9$ 

3.23 Since $p = 1 / 2$ and $\xi ( n ) ^ { 2 } = \tau$ 

$$
\begin{array}{c} {E (\xi (n)) = \frac {1}{2} \sqrt {\tau} - \frac {1}{2} \sqrt {\tau} = 0,} \\ {\mathrm{Var} (\xi (n)) = E (\xi (n) ^ {2}) - E (\xi (n)) ^ {2} = \frac {1}{2} \tau + \frac {1}{2} \tau = \tau ,} \\ {E (k (n)) = m \tau + \sigma E (\xi (n)) = m \tau ,} \\ {\mathrm{Var} (k (n)) = \sigma^ {2} \mathrm{Var} (\xi (n)) = \sigma^ {2} \tau .} \end{array}
$$

3.24 By (3.2) 

$$
\begin{array}{l} S (1) = S (0) \mathrm{e} ^ {k (1)} = S (0) \mathrm{e} ^ {m \tau + \sigma \xi (1)}, \\ S (2) = S (0) \mathrm{e} ^ {k (1) + k (2)} = S (0) \mathrm{e} ^ {2 m \tau + \sigma (\xi (1) + \xi (2))}. \end{array}
$$

3.25 Let $\begin{array} { r } { t = \frac { n } { N } } \end{array}$ . Because the $\xi _ { N } ( i )$ are independent, $E ( \xi _ { N } ( i ) ) = 0 \mathrm { a n d } \mathrm { V a r } ( \xi _ { N } ( i ) ) =$ $\textstyle { \frac { 1 } { N } }$ for each $i = 1 , 2 , \dots ,$ , it follows that 

$$
\begin{array}{c} E (w _ {N} (t)) = E (\xi_ {N} (1) + \dots + \xi_ {N} (n)) \\ = E (\xi_ {N} (1)) + \dots + E (\xi_ {N} (n)) = 0, \\ \operatorname{Var} (w _ {N} (t)) = \operatorname{Var} (\xi_ {N} (1) + \dots + \xi_ {N} (n)) \\ = \operatorname{Var} (\xi_ {N} (1)) + \dots + \operatorname{Var} (\xi_ {N} (1)) = \frac {n}{N} = t. \end{array}
$$

## Chapter 4

4.1 We can use the formulae in the proof of Proposition 4.1 to find 

$$
y (1) = \frac {2 0 0 - 3 5 . 2 4 \times 6 0 - 2 4 . 1 8 \times 2 0}{1 0 0} \cong - 2 3. 9 8,
$$

$$
V (1) \cong 3 5. 2 4 \times 6 5 + 2 4. 1 8 \times 1 5 - 2 3. 9 8 \times 1 1 0 \cong 1 5. 5 0,
$$

$$
y (2) = \frac {1 5 . 5 0 + 4 0 . 5 0 \times 6 5 - 1 0 . 1 3 \times 1 5}{1 1 0} \cong 2 2. 6 9,
$$

$$
V (2) \cong - 4 0. 5 0 \times 7 5 + 1 0. 1 3 \times 2 5 + 2 2. 6 9 \times 1 2 1 \cong - 3 8. 6 0.
$$

4.2 For a one-step strategy admissibility reduces to a couple of inequalities, $V ( 0 ) \geq$ 0 and $V ( 1 ) \bar { \geq } 0$ . The first inequality can be written as 

$$
1 0 x + 1 0 y \geq 0.
$$

The second inequality means that both values of the random variable $V ( 1 )$ should be non-negative, which gives two more inequalities to be satisfied by x and $_ { y , }$ 

$$
\begin{array}{c} 1 3 x + 1 1 y \geq 0, \\ 9 x + 1 1 y \geq 0. \end{array}
$$

The set of portfolios $( x , y )$ satisfying all these inequalities is shown in Fig ure S.7. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/1a3cb6813da4691da34373d0a235858ffd41fbff261c9fe9d1e75366fc5a5823.jpg)



Figure S.7 Admissible portfolios in Exercise 4.2


4.3 Suppose that there is a self-financing predictable strategy with initial value $V ( 0 ) = 0$ and final value $0 \neq V ( 2 ) \geq 0$ , such that $V ( 1 ) < 0$ with positive probability. The last inequality means that this strategy is not admissible, but we shall construct an admissible one that violates the No-Arbitrage Principle. Here is how to proceed to achieve arbitrage: 

Do not invest at all at time 0. 

At time 1 check whether the value $V ( 1 )$ of the non-admissible strategy is negative or not. If $V ( 1 ) \geq 0$ , then refrain from investing at all once again. However, if $V ( 1 ) < 0$ , then take the same position in stock as in the nonadmissible strategy and a risk-free position that is lower by $- V ( 1 )$ than that in the non-admissible strategy. 

This defines a predictable self-financing strategy. Its time 0 and time 1 value is 0. The value at time 2 will be 

$$
\left\{ \begin{array}{c l} 0 & \text {if V(1)\geq 0}, \\ V (2) - V (1) > 0 & \text {if V(1) <   0}. \end{array} \right.
$$

This is, therefore, an admissible strategy realising an arbitrage opportunity. 

4.4 If you happen to know that an increase in stock price will be followed by a fall at the next step, then adopt this strategy: 

At time 0 do not invest in either asset. 

At time 1 check whether the stock has gone up or down. If down, then again do not invest in either asset. But if stock has gone up, then sell short one share for $S ( 0 ) u ,$ , investing the proceeds risk-free. 

Clearly, the time 0 and time 1 value of this strategy is $V ( 0 ) = V ( 1 ) = 0$ . If stock goes down at the first step, then the value at time 2 will be $\overset { \cdot } { V } ( 2 ) = 0$ But if stock goes up at the first step, then it will go down at the second step and $V ( 2 ) = S ( 0 ) u ( r - d )$ will be positive, as required, since $u > r > d .$ . (The notation is as in Section 3.2.) 

Clearly, this is not a predictable strategy, which means that no arbitrage has been achieved. 

4.5 a) If there are no short-selling restrictions, then the following strategy will realise an arbitrage opportunity: 

At time 0 do not invest at all. 

At time 1 check the price S(1). If $S ( 1 ) = 1 2 0$ dollars, then once again do not invest at all. But if $S ( 1 ) = 9 0 $ dollars, then sell short one share of the risky asset and invest the proceeds risk-free. 

The time 0 and time 1 value of this admissible strategy is 0. The value at time 2 will be 

0 in scenarios $\omega _ { 1 }$ and $\omega _ { 2 }$ , 

 <sub>3</sub> <sub>in</sub> <sub>scenario</sub> <sub>ω3,</sub> 

which means that arbitrage can be achieved. 

b) In a) above arbitrage has been achieved by utilising the behaviour of stock prices at the second step in scenario $\omega _ { 2 } \mathrm { : }$ : The return on the risky asset is lower than the risk-free return. Thus, shorting the risky asset and investing the proceeds risk-free creates arbitrage. However, when short selling of risky assets is disallowed, then this arbitrage opportunity will be beyond the reach of investors. 

4.6 The arbitrage strategy described in Solution 4.5 involves buying a fraction of a bond. If $\bar { S } ( 1 ) = 9 \bar { 0 }$ dollars, then one share of stock should be shorted and $\frac { 9 } { 1 1 }$ of a bond purchased at time 1. To obtain an arbitrage strategy involving an integer number of units of each asset, multiply these quantities by 11, that is, short sell 11 shares of stock and buy 9 bonds. 

4.7 Suppose that transaction costs of 5% apply whenever stock is bought or sold. An investor who tried to follow the strategy in Solution 4.5, short selling one share of stock at time 1 if $S ( 1 ) = 9 0 $ dollars, would have to pay transaction costs of $9 0 \times 5 \% = 4 . 5 0$ dollars. If the remaining amount of $9 0 - 4 . 5 0 = 8 5 . 5 0$ dollars were invested risk-free, it would be worth ${ 8 5 . 5 \times { \frac { 1 2 1 } { 1 1 0 } } = 9 4 . 0 5 ~ \mathrm { d o l l } }$ ars at time 2. But closing the short position in stock would cost $96, making the final wealth negative. As a result, there is no arbitrage strategy. 

4.8 The put option gives the right (but no obligation) to sell one share of stock for the strike price $X = 1 1 0$ dollars at time 2. We consider an extended mode with three assets, the stock, the money market, and the option. The unit prices of these assets are $S ( n ) , A ( n ) , P ^ { \mathrm { E } } ( n )$ , where $\dot { P } ^ { \mathrm { E } } ( n )$ is the market price of the put option at time $n = 0 , 1 , 2$ . The time 2 price of the put option is 

$$
P ^ {\mathrm{E}} (2) = \max \{X - S (2), 0 \}.
$$

According to the Fundamental Theorem of Asset Pricing, the discounted stock and option prices $\widetilde { S } ( n ) = S ( n ) / A ( n )$ and $\widetilde { P } ^ { \mathrm { E } } ( n ) = P ^ { \mathrm { E } } ( n ) / A ( n )$ should form a martingale under some probability measure $P _ { * } , \mathrm { o r }$ else an arbitrage opportunity would arise. From Example 4.5 we know that there is only one probability $P _ { * }$ turning $\widetilde { S } ( n )$ into a martingale. Because of this, $\widetilde { P } ^ { \mathrm { E } } ( n )$ must be a martin gale under the same probability $P _ { * }$ . It follows that 

$$
P ^ {\mathrm{E}} (1) = \frac {A (1)}{A (2)} E _ {*} (P ^ {\mathrm{E}} (2) | S (1)) \quad \text { and } \quad P ^ {\mathrm{E}} (0) = \frac {A (0)}{A (1)} E _ {*} (P ^ {\mathrm{E}} (1)).
$$

Using the values of $P _ { * }$ for each scenario found in Example 4.5, we can compute $P ^ { \mathrm { E } } ( \vec { 1 } )$ and $P ^ { \mathrm { E } } ( 0 )$ . For example 

$$
\begin{array}{c} P ^ {\mathrm{E}} (1, \omega_ {3}) = P ^ {\mathrm{E}} (1, \omega_ {4}) = \frac {A (1)}{A (2)} \frac {P _ {*} (\omega_ {3}) P ^ {\mathrm{E}} (2 , \omega_ {3}) + P _ {*} (\omega_ {4}) P ^ {\mathrm{E}} (2 , \omega_ {4})}{P _ {*} (\omega_ {3}) + P _ {*} (\omega_ {4})} \\ = \frac {1 1 0}{1 2 1} \frac {\frac {1}{2 5} \times 2 0 + \frac {1}{1 0 0} \times 3 0}{\frac {1}{2 5} + \frac {1}{1 0 0}} \cong 2 0. 0 0 \end{array}
$$

dollars. In this manner, we obtain 

$$
\begin{array}{c c c c} \text {Scenario} & P ^ {\mathrm{E}} (0) & P ^ {\mathrm{E}} (1) & P ^ {\mathrm{E}} (2) \\ \omega_ {1} & 1. 9 6 & 1. 2 1 & 0. 0 0 \\ \omega_ {2} & 1. 9 6 & 1. 2 1 & 4. 0 0 \\ \omega_ {3} & 1. 9 6 & 2 0. 0 0 & 2 0. 0 0 \\ \omega_ {4} & 1. 9 6 & 2 0. 0 0 & 3 0. 0 0 \end{array}
$$

## Chapter 5

5.1 In the first investment project 

$$
E (K _ {1}) = 0. 1 2 \times 0. 2 5 + 0. 1 2 \times 0. 7 5 = 0. 1 2,
$$

$$
\mathrm{Var} (K _ {1}) = (0. 1 2 - 0. 1 2) ^ {2} \times 0. 2 5 + (0. 1 2 - 0. 1 2) ^ {2} \times 0. 7 5 = 0.
$$

In the second project 

$$
E (K _ {2}) = 0. 1 1 \times 0. 2 5 + 0. 1 3 \times 0. 7 5 = 0. 1 2 5,
$$

$$
\operatorname{Var} \left(K _ {2}\right) = (0. 1 1 - 0. 1 2 5) ^ {2} \times 0. 2 5 + (0. 1 3 - 0. 1 2 5) ^ {2} \times 0. 7 5 = 0. 0 0 0 0 7 5.
$$

Finally, in the third project 

$$
E (K _ {3}) = 0. 0 2 \times 0. 2 5 + 0. 2 2 \times 0. 7 5 = 0. 1 7,
$$

$$
\operatorname{Var} (K _ {3}) = (0. 0 2 - 0. 1 7) ^ {2} \times 0. 2 5 + (0. 2 2 - 0. 1 7) ^ {2} \times 0. 7 5 = 0. 0 0 7 5.
$$

The first project is the least risky one, in fact, it is risk-free. The third project involves the highest risk. 

5.2 First we put $K _ { 2 } ( \omega _ { 2 } ) = x$ and compute 

$$
\begin{array}{l} \operatorname{Var} (K _ {1}) = 0. 0 0 1 8 7 5, \\ \operatorname{Var} (K _ {2}) = 0. 1 8 7   5 x ^ {2} + 0. 0 1 5 x + 0. 0 0 0 3. \end{array}
$$

The two securities will have the same risk if $\operatorname { V a r } ( K _ { 1 } ) = \operatorname { V a r } ( K _ { 2 } )$ . This gives the following equation 

$$
0. 0 0 0 3 + 0. 1 8 7 5 x ^ {2} + 0. 0 1 5 x = 0. 0 0 1 8 7 5
$$

with two solutions x = 0.14 or 0.06. This means that $K _ { 2 } ( \omega _ { 2 } ) = - 1 4 \%$ or $6 \%$ 

5.3 First we use the formula $\mathrm { e } ^ { k _ { i } } = 1 + K _ { i }$ for $i = 1 , 2$ to compute the logarithmic returns and then work out the variance of each return: 

<table><tr><td>Scenario</td><td>Probability</td><td><eq>K_{1}</eq></td><td><eq>K_{2}</eq></td><td><eq>k_{1}</eq></td><td><eq>k_{2}</eq></td></tr><tr><td><eq>\omega_{1}</eq></td><td>0.5</td><td>10.53%</td><td>7.23%</td><td>10.01%</td><td>6.98%</td></tr><tr><td><eq>\omega_{2}</eq></td><td>0.5</td><td>13.89%</td><td>10.55%</td><td>13.01%</td><td>10.03%</td></tr><tr><td>Variance</td><td></td><td>0.000282</td><td>0.000276</td><td>0.000224</td><td>0.000232</td></tr></table>

We find that Var $( K _ { 1 } ) > \mathrm { V a r } ( K _ { 2 } )$ , whereas $\mathrm { V a r } ( k _ { 1 } ) < \mathrm { V a r } ( k _ { 2 } )$ 

This is an interesting observation because it shows that greater risk as measured by Var(K) does not necessarily mean greater risk in the sense of Var(k). Nevertheless, when the rates of return are of the order of 10% or lower, the diferences between these two measures of risk are tiny and can simply be ignored in financial practice. This is because the errors due to inaccurate estimation of the parameters (the probabilities and values of return rates in diferent scenarios) are typically greater than these diferences. 

5.4 Let $x _ { 1 }$ and $x _ { 2 }$ be the number of shares of type 1 and 2 in the portfolio. Then 

$$
\begin{array}{l} V (1) = x _ {1} S _ {1} (1) + x _ {2} S _ {2} (1) = V (0) \left(w _ {1} \frac {S _ {1} (1)}{S _ {1} (0)} + w _ {2} \frac {S _ {2} (1)}{S _ {2} (0)}\right) \\ = 1 0 0 \left(0. 2 5 \times \frac {4 8}{4 5} + 0. 7 5 \times \frac {3 2}{3 3}\right) = 9 9. 3 9 4. \end{array}
$$

5.5 The return on the portfolio is $K _ { V } = w _ { 1 } K _ { 1 } + w _ { 2 } K _ { 2 }$ . This gives 

$$
\begin{array}{l l} K _ {V} = 0. 3 0 \times 12 \% - 0. 7 \times 4 \% = 0. 8 \% & \text {in scenario} \omega_ {1}, \\ K _ {V} = 0. 3 0 \times 10 \% + 0. 7 \times 7 \% = 7. 9 \% & \text {in scenario} \omega_ {2}. \end{array}
$$

5.6 The initial and final values of the portfolio are 

$$
\begin{array}{c} V (0) = x _ {1} S _ {1} (0) + x _ {2} S _ {2} (0), \\ V (1) = x _ {1} S _ {1} (0) \mathrm{e} ^ {k _ {1}} + x _ {2} S _ {2} (0) \mathrm{e} ^ {k _ {2}} \\ = V (0) \left(w _ {1} \mathrm{e} ^ {k _ {1}} + w _ {2} \mathrm{e} ^ {k _ {2}}\right). \end{array}
$$

As a result, the return on the portfolio is 

$$
\mathrm{e} ^ {k _ {V}} = \frac {V (1)}{V (0)} = w _ {1} \mathrm{e} ^ {k _ {1}} + w _ {2} \mathrm{e} ^ {k _ {2}}.
$$

5.7 First we find $E ( K _ { 1 } ) = 7 \%$ and $E ( K _ { 2 } ) = 2 3 \%$ . If the expected return on the portfolio is to be $\dot { E } ( K _ { V } ) = 2 0 \%$ , then by (5.4) and (5.1) the weights must satisfy the system of equations 

$$
\begin{array}{c} {7 w _ {1} + 2 3 w _ {2} = 2 0,} \\ {w _ {1} + w _ {2} = 1.} \end{array}
$$

The solution is $w _ { 1 } = 1 8 . 7 5 \%$ and $w _ { 2 } = 8 1 . 2 5 \%$ 

5.8 First, we find compute $\mu _ { 1 } = 4 \%$ and $\mu _ { 2 } = 1 6 \%$ from the data in Example 5.6. Next, (5.7) and (5.1) give the system of equations 

$$
\begin{array}{c} 4 w _ {1} + 1 4 w _ {2} = 4 6, \\ w _ {1} + w _ {2} = 1, \end{array}
$$

for the weights $w _ { 1 }$ and $w _ { 2 }$ . The solution is $w _ { 1 } = - 3 . 2$ and $w _ { 2 } = 4 . 2$ . Finally, we use $\left( 5 . 7 \right)$ with the values $\sigma _ { 1 } ^ { 2 } \cong 0 . 0 1 8 4 , \sigma _ { 2 } ^ { 2 } \cong 0 . 0 0 2 4$ and $\rho _ { 1 2 } \cong - 0 . 9 6 3 0 9$ computed in Example 5.6 to find the risk of the portfolio: 

$$
\begin{array}{r l} & {\sigma_ {V} ^ {2} \cong (- 3. 2) ^ {2} \times 0. 0 1 8 4 + (4. 2) ^ {2} \times 0. 0 0 2 4} \\ & {\qquad + 2 \times (- 3. 2) \times 4. 2 \times (- 0. 9 6 3 0 9) \times \sqrt {0 . 0 1 8 4} \times \sqrt {0 . 0 0 2 4}} \\ & {\qquad \cong 0. 4 0 2 7 8.} \end{array}
$$

5.9 The returns on risky securities are non-constant random variables, that is, $K _ { 1 } ( \omega _ { 1 } ) \neq K _ { 1 } ( \omega _ { 2 } )$ and $K _ { 2 } ( \omega _ { 1 } ) \neq K _ { 2 } ( \omega _ { 2 } )$ . Because of this, the system of equa tions 

$$
\begin{array}{l} K _ {1} (\omega_ {1}) = a K _ {2} (\omega_ {1}) + b, \\ K _ {1} (\omega_ {2}) = a K _ {2} (\omega_ {2}) + b, \end{array}
$$

must have a solution $a \neq 0$ and b. It follows that $ K _ { 1 } = a K _ { 2 } + b .$ 

Now, use the properties of covariance and variance to compute 

$$
\begin{array}{c} \operatorname{Cov} (K _ {1}, K _ {2}) = \operatorname{Cov} (a K _ {2} + b, K _ {2}) = a \operatorname{Cov} (K _ {2}, K _ {2}) = a \operatorname{Var} (K _ {2}) = a \sigma_ {2} ^ {2}, \\ \sigma_ {1} ^ {2} = \operatorname{Var} (K _ {1}) = \operatorname{Var} (a K _ {2} + b) = a ^ {2} \operatorname{Var} (K _ {2}) = a ^ {2} \sigma_ {2} ^ {2}. \end{array}
$$

It follows that $\sigma _ { 1 } = \left| a \right| \sigma _ { 2 }$ and 

$$
\rho_ {1 2} = \frac {\mathrm{Cov} (K _ {1} , K _ {2})}{\sigma_ {1} \sigma_ {2}} = \frac {a \sigma_ {2} ^ {2}}{| a | \sigma_ {2} ^ {2}} = \pm 1.
$$

5.10 Using the values $\sigma _ { 1 } ^ { 2 } \cong 0 . 0 1 8 4 , \sigma _ { 2 } ^ { 2 } \cong 0 . 0 0 2 4$ and $\rho _ { 1 2 } \cong - 0 . 9 6 3 0 9$ computed in Example 5.6, we find $s _ { 0 }$ from (5.13): 

$$
s _ {0} = \frac {\sigma_ {1} ^ {2} - \rho_ {1 2} \sigma_ {1} \sigma_ {2}}{\sigma_ {1} ^ {2} + \sigma_ {2} ^ {2} - 2 \rho_ {1 2} \sigma_ {1} \sigma_ {2}} \cong 0. 7 3 8 0 9.
$$

This means that the weights in the portfolio with minimum risk are $w _ { 1 } =$ 0.73809 and $w _ { 2 } = 0 . 2 6 1 9 1$ and it involves no short selling. 

5.11 $\mu _ { V } = 0 . 0 6 , \sigma _ { V } \cong 1 . 0 1 3 .$ 

5.12 The weights of the three securities in the minimum variance portfolio are w $\cong$ $\left[ \begin{array} { l l } { 0 . 3 1 4 } & { 0 . 1 4 8 } & { 0 . 5 3 8 } \end{array} \right]$ , the expected return on the portfolio is $\mu _ { V } \cong 0 . 1 7 3$ and the standard deviation is $\sigma _ { V } \cong 0 . 1 5 1$ 

5.13 The weights in the portfolio with the minimum variance among all attainable portfolios with expected return $\mu _ { V } = 2 0 \%$ are $\pmb { w } \cong \left[ \begin{array} { l l l } { 0 . 6 7 2 } & { - 0 . 2 4 6 } & { 0 . 5 7 4 } \end{array} \right]$ The standard deviation of this portfolio is $\sigma _ { V } \cong 0 . { \dot { 1 } } 9 2$ 

5.14 The weights and standard deviations of portfolios along the minimum variance line, parametrised by the expected return $\mu _ { V }$ , are 

$$
\boldsymbol {w} \cong \left[ \begin{array}{c c c} - 2. 0 2 7 + 1 3. 4 9 2 \mu_ {V} & 2. 7 2 8 - 1 4. 8 7 0 \mu_ {V} & 0. 2 9 8 + 1. 3 7 6 \mu_ {V} \end{array} \right],
$$

$$
\sigma_ {V} = \sqrt {0 . 6 2 5 - 6 . 9 4 6 \mu_ {V} + 2 0 . 0 1 8 \mu_ {V} ^ {2}}.
$$

This minimum variance line is presented in Figure S.8, along with the set of attainable portfolios with short selling (light shading) and without (darker shading). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/0a1b33519361ebd91d7fdd6a9b7981fac9cf07de80471a7e51ed743b732a0c06.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/c4ccada68d6a346cf5e9dc942037b3b1c52a0d828162124466fe0f887f4555fd.jpg)



Figure S.8 Minimum variance line and attainable portfilios on the $w _ { 2 } , w _ { 3 }$ and $\sigma , \mu$ planes


5.15 Let m be the one-row matrix formed by the expected returns of the three securities. By multiplying the $\gamma \pmb { w } \pmb { C } = \pmb { m } - \mu \pmb { u }$ equality by ${ \boldsymbol { C } } ^ { - 1 } { \boldsymbol { u } } ^ { T }$ and, respectively, $\check { C } ^ { - 1 } m ^ { T }$ , we get 

$$
\mu_ {V} (\boldsymbol {m} - \mu \boldsymbol {u}) \boldsymbol {C} ^ {- 1} \boldsymbol {u} ^ {T} = (\boldsymbol {m} - \mu \boldsymbol {u}) \boldsymbol {C} ^ {- 1} \boldsymbol {m} ^ {T},
$$

since ${ \boldsymbol { w } } { \boldsymbol { u } } ^ { T } = 1$ and $\boldsymbol { w m } ^ { T } = \mu \boldsymbol { V }$ . This can be solved for $\mu$ to get 

$$
\mu = \frac {\boldsymbol {m} \boldsymbol {C} ^ {- 1} (\boldsymbol {m} ^ {T} - \mu_ {V} \boldsymbol {u} ^ {T})}{\boldsymbol {u} \boldsymbol {C} ^ {- 1} (\boldsymbol {m} ^ {T} - \mu_ {V} \boldsymbol {u} ^ {T})} \cong 0. 1 4 2.
$$

Then, $\gamma$ can be computed as follows: 

$$
\gamma = (\boldsymbol {m} - \mu \boldsymbol {u}) \boldsymbol {C} ^ {- 1} \boldsymbol {u} ^ {T} \cong 1. 3 6 7.
$$

5.16 The market portfolio weights are ${ \pmb w } \cong \left[ \begin{array} { l l l } { 0 . 4 3 8 } & { 0 . 0 1 2 } & { 0 . 5 5 0 } \end{array} \right]$ . The expected return on this portfolio is $\mu _ { M } \cong 0 . 1 8 \mathrm { 3 }$ <sub>and the standard deviation is</sub> $\sigma _ { M } \cong$ 0.156. 

5.17 $\beta _ { V } \cong 0 . 8 5 7$ $\alpha _ { V } \cong - 0 . 1 0 2$ 

5.18 The expected return on the portfolio can be expressed as $K _ { V } = w _ { 1 } K _ { 1 } + \cdot \cdot \cdot +$ $w _ { n } K _ { n }$ in terms of the expected returns on the individual securities. Because covariance is linear in each of its arguments, 

$$
\begin{array}{l} \beta_ {V} = \frac {\operatorname{Cov} (K _ {V} , K _ {M})}{\sigma_ {M} ^ {2}} = w _ {1} \frac {\operatorname{Cov} (K _ {1} , K _ {M})}{\sigma_ {M} ^ {2}} + \dots + w _ {n} \frac {\operatorname{Cov} (K _ {n} , K _ {M})}{\sigma_ {M} ^ {2}} \\ \qquad = w _ {1} \beta_ {1} + \dots + w _ {n} \beta_ {n}. \end{array}
$$

5.19 The equation of the characteristic line is $y = \beta _ { V } x + \alpha _ { V }$ , where $\beta _ { V }$ is the beta factor of that security and $\alpha _ { V } = \mu _ { V } - \beta _ { V } \mu _ { M }$ . In the CAPM the equation $\mu _ { V } = r _ { F } + ( \mu _ { M } - r _ { F } ) \beta _ { V }$ of the security market line holds. Substitution into the formula for α gives $_ { \mathcal { X } V } = r _ { F } - r _ { F } \beta _ { V }$ , so the equation of the characteristic line becomes $y = \beta _ { V } ( x - r _ { F } ) + r _ { F }$ . Clearly, the characteristic line of any security will pass through the point with coordinates $r _ { F } , r _ { F }$ 

## Chapter 6

6.1 Yes, there is an arbitrage opportunity. We enter into a long forward contract and sell short one share, investing 70% of the proceeds at 8% and paying the remaining 30% as a security deposit to attract interest at 4%. At the time of delivery the cash investments plus interest will be worth about $18.20, out of which $18 will need to be paid for one share to close out the short position in stock. This leaves a $0.20 arbitrage profit. 

The rates d for the security deposit such that there is no arbitrage opportunity satisfy $3 0 \% \times 1 7 \times \mathrm { e } ^ { d } + 7 0 \% \times 1 7 \times \mathrm { e } ^ { 8 \% } \leq 1 8$ . The highest such rate is $d \cong 0 . 1 7 4 0 \%$ 

6.2 We take 1 January 2000 to be time 0. By (6.2) 

$$
F (0, 3 / 4) = S (0) \mathrm{e} ^ {0. 0 6 \times \frac {3}{4}}, \qquad F (1 / 4, 3 / 4) = 0. 9 S (0) \mathrm{e} ^ {0. 0 6 \times \frac {2}{4}}.
$$

It follows that the forward price drops by 

$$
\frac {F (0 , 3 / 4) - F (1 / 4 , 3 / 4)}{F (0 , 3 / 4)} = \frac {\mathrm{e} ^ {\frac {3}{4} \times 6 \%} - 0 . 9 \mathrm{e} ^ {\frac {1}{2} \times 6 \%}}{\mathrm{e} ^ {\frac {3}{4} \times 6 \%}} \cong 11.34 \%.
$$

6.3 The present value of the dividends is 

$$
\mathrm{div} _ {0} = 1 \mathrm{e} ^ {- \frac {6}{12} \times 12 \%} + 2 \mathrm{e} ^ {- \frac {9}{12} \times 12 \%} \cong 2. 7 7
$$

dollars. The right-hand side of (6.4) is equal to 

$$
[ S (0) - \mathrm{div} _ {0} ] \mathrm{e} ^ {r T} \cong (1 2 0 - 2. 7 7) \mathrm{e} ^ {\frac {1 0}{1 2} \times 12 \%} \cong 1 2 9. 5 6
$$

dollars, which is less than the quoted forward price of $131. As a result, there will be an arbitrage opportunity, which can be realised as follows: 

on 1 January 2000 enter into a short forward position and borrow $120 to buy stock; 

on 1 July 2000 collect the first dividend of $1 and invest risk-free; 

on 1 October 2000 collect the second dividend of $2 and invest risk-free; 

on 1 November 2000 close out all positions. 

You will be left with an arbitrage profit of 

$$
131 - 120\mathrm{e}^{\frac{10}{12}\times 12\%} + 1\mathrm{e}^{\frac{4}{12}\times 12\%} + 2\mathrm{e}^{\frac{1}{12}\times 12\%}\cong 1.44
$$

dollars. 

6.4 No arbitrage profit can be realised in these circumstances. Though the theoretical no-arbitrage forward price is about $87.83, the first strategy in the proof of Proposition 6.2 brings a loss of $8 9 - 8 3 \mathrm { { e } ^ { 1 0 \% } + 2 \mathrm { { e } ^ { 0 . 5 \times 7 \% } \cong - 0 . 6 6 } }$ dollars and the second one results in a loss of $- 8 9 + 8 3 \mathrm { e } ^ { 7 \% } - 2 \mathrm { e } ^ { 0 . 5 \times 1 0 \% } \cong - 2 . 0 8$ dollars. 

6.5 The euro plays the role of the underlying asset with dividend yield 3%. Hence the forward price (the exchange rate) is 

$$
F (0, 1 / 2) = 0. 9 8 3 4 \mathrm{e} ^ {0. 5 (4 \% - 3 \%)} \cong 0. 9 8 8 3
$$

euros to a dollar. 

6.6 At time t 

borrow and pay (or receive and invest, if negative) the amount $V ( t )$ to acquire a short forward contract with forward price $F ( 0 , T )$ and delivery date $T ,$ 

initiate a new long forward contact with forward price $F ( t , T )$ at no cost. Then at time $T$ 

close out both forward contracts receiving (or paying, if negative) the amounts $S ( T ) - F ( 0 , T )$ and $S ( T ) - F ( t , \bar { T } )$ , respectively; 

collect $V ( t ) \mathrm { e } ^ { r ( T - t ) }$ from the risk-free investment, with interest. 

The final balance $V ( t ) \mathrm { e } ^ { r ( T - t ) } - [ F ( t , T ) - F ( 0 , T ) ] > 0$ will be your arbitrage profit. 

6.7 By (6.3) the initial forward price is $F ( 0 , 1 ) \cong 4 5 . 7 2$ dollars. This takes into account the dividend paid at time $1 / 2 .$ 

a) If $S ( 9 / 1 2 ) = 4 9 $ dollars, then $F ( 9 / 1 2 , 1 ) \cong 4 9 . 7 4$ dollars by (6.2). It follows by (6.8) that $V ( 9 / 1 2 ) \cong 3 . 9 6$ dollars. 

b) If $S ( 9 / 1 2 ) = 5 1 $ dollars, then $F ( 9 / 1 2 ) \cong 5 1 . 7 7$ dollars and $V ( 9 / 1 2 ) \cong$ 5.96 dollars. 

6.8 Let $t = 1 / 3 6 5 , T = 1 / 4$ . We apply the formula (6.11) to get 

$$
f (t, T) - f (0, T) = S (t) \mathrm{e} ^ {r (T - t)} + S (0) \mathrm{e} ^ {r T} = 0
$$

if $S ( t ) = S ( 0 ) \mathrm { e } ^ { r t }$ , that is, if the stock grows at the risk-free rate. 

6.9 Since $f ( t , T ) = S ( t ) \mathrm { e } ^ { r ( T - t ) }$ , the random variables $S ( t )$ and $f ( t , T )$ are perfectly correlated with $\rho _ { S ( t ) f ( t , T ) } = 1$ and $\sigma _ { f ( t , T ) } = \mathrm { e } ^ { r ( T - t ) } \sigma _ { S ( t ) }$ . It follows that $N =$ $\mathrm { e } ^ { - r ( T - t ) }$ 

6.10 Observe that Theorem 6.5 on the equality of futures and forward prices applies also in the case of an asset with dividends paid continuously. We can, therefore, use (6.6) to obtain 

$$
r _ {\mathrm{div}} = 8 \% - \frac {1}{0 . 7 5} \ln \frac {1 4 , 1 0 0}{1 3 , 5 0 0} \cong 2. 2 0 \%.
$$

6.11 The return on the index will be 3.37%. For $r _ { F } = 1 \%$ this gives the futures prices $f ( 0 , 3 ) \cong 9 1 6 . 9 7$ and $f ( 1 , 3 ) \cong 9 3 8 . 4 9$ . If the beta coeficient for a portfolio is $\beta _ { V } = 1 . 5$ , then the expected return on this portfolio will be $\mu _ { V } \cong 4 . 5 6 \%$ To construct a portfolio with $\beta _ { \widetilde { V } } = 0$ and initial value $V ( 0 ) = 1 0 0 $ dollars, supplement the original portfolio with $N \cong 0 . 1 6 5 2$ short futures contracts (observe that N is the same as in Example 6.4). 

If the actual return on the original portfolio during the first time step happens to be equal to the expected return, then its value after one step will be $V ( 1 ) \cong 1 0 4 . 5 6$ dollars. Marking to market requires the holder of $N \cong 0 . 1 6 5 2$ short forward contracts to pay $3.56. As a result, after one step the value of the portfolio with forward contracts will be $\widetilde { V } ( 1 ) \cong 1 0 4 . 5 6 - 3 . 5 6 = 1 0 1 . 0 0$ dollars, once again matching the risk-free growth. 

## Chapter 7

7.1 The investment will bring a profit of 

$$
(3 6 - S (T)) ^ {+} - 4. 5 0 \mathrm{e} ^ {0. 1 2 \times \frac {3}{1 2}} = 3,
$$

where $S ( T )$ is the stock price on the exercise date. This gives $S ( T ) \cong 2 8 . 3 6$ dollars. 

7.2 $E ( ( S ( T ) - 9 0 ) ^ { + } - 8 \mathrm { e } ^ { 0 . 0 9 \times \frac { 6 } { 1 2 } } ) \cong - 5 . 3 7$ dollars. 

7.3 By put-call parity $2 . 8 3 - P ^ { \mathrm { E } } = 1 5 . 6 0 - 1 5 . 0 0 \mathrm { e } ^ { - \frac { 3 } { 1 2 } \times 0 . 0 6 7 2 }$ <sup>2</sup>, so $P ^ { \mathrm { E } } \cong 1$ . 98 dollars. 

7.4 Put-call parity is violated, $5 . 0 9 - 7 . 7 8 > 2 0 . 3 7 - 2 4 e ^ { - 0 . 0 7 4 8 \times \frac { 6 } { 1 2 } }$ . Arbitrage can be realised as in the first part of the proof of Theorem 7.1: 

Buy a share for $20.37; 

Buy a put option for $7.78; 

Write and sell a call option for $5.09; 

Borrow $23.06 at the interest rate of 7.48%. 

The balance of these transactions is zero. After six months 

Sell one share for $24 by exercising the put option or settling the short position in calls, depending on whether the share price turns out to be below or above the strike price; 

Repay the loan with interest, amounting to $2 3 . 0 6 e ^ { \frac { 1 } { 2 } \times 0 . 0 7 4 8 } \cong 2 3 . 9 4$ dollars in total. 

The balance of $2 4 - 2 3 . 9 6 = 0 . 0 6$ dollars will be your arbitrage profit. 

7.5 If $C ^ { \mathrm { E } } - P ^ { \mathrm { E } } > S ( 0 ) - \mathrm { d i v } _ { 0 } - X \mathrm { e } ^ { - r T }$ , then at time 0 buy a share and a put option, write and sell a call option, and invest (or borrow, if negative) the balance on the money market at the interest rate r. As soon as you receive the dividend, invest it at the rate r. At the exercise time $T$ close the money market investment and sell the share for X, either by exercising the put if $S ( T ) < X$ , or by settling the call if $S ( T ) \geq X$ . The final balance $\overline { { ( C ^ { \textnormal { E } } - P ^ { \textnormal { E } } } } -$ $S ( 0 ) + \mathrm { d i v } _ { 0 } ) \mathrm { e } ^ { r T } + X > 0$ will be your arbitrage profit. 

On the other hand, if $\begin{array} { r } { C ^ { \mathrm { E } } - P ^ { \mathrm { E } } < S ( 0 ) - \mathrm { d i v } _ { 0 } - X \mathrm { e } ^ { - r T } } \end{array}$ , then at time 0 sell short a share, write and sell a put, and buy a call option, investing the balance on the money market. When a dividend becomes due on the shorted share, borrow the amount and pay it to the owner of the stock. At time $T$ close the money market position, buy a share for X by exercising the call if $S ( T ) > X$ or settling the put if $S ( T ) \leq X$ , and close the short position in stock. Your arbitrage profit will be $\begin{array} { r } { ( - C ^ { \mathrm { E } } + P ^ { \mathrm { E } } + S ( 0 ) - \mathrm { d i v } _ { 0 } ) \mathrm { e } ^ { r T } - X > 0 } \end{array}$ 

7.6 If $C ^ { \mathrm { E } } - P ^ { \mathrm { E } } < S ( 0 ) \mathrm { e } ^ { - r _ { \mathrm { d i v } } T } - X \mathrm { e } ^ { - r T }$ , then at time 0 sell short $\mathbf { e } ^ { - r _ { \mathrm { { d i v } } } T }$ of $\mathrm { a }$ share, write and sell a put, and buy a call option, investing the balance at the rate $^ r .$ . Between time 0 and $T$ pay dividends to the stock owner, raising cash by shorting the stock. This will lead to one shorted share held at time $T .$ If the put option is exercised at time $T ,$ , you will have to buy a share for $X$ Use this share to close the short position in stock. You will be left with a cal option and a positive amount $( { - \dot { C } ^ { \mathrm { E } } + P ^ { \mathrm { E } } + S ( 0 } ) { \mathrm { e } } ^ { - r _ { \mathrm { d i v } } T } - X { \mathrm { e } } ^ { - r T } ) { \mathrm { e } } ^ { r T } > 0$ . If the put option is not exercised at all, then you can use the call to buy a share for X at time $T$ , closing the short position in stock. You will also be left with a positive final balance $\dot { ( } - C ^ { \mathrm { E } } + P ^ { \dot { \mathrm { E } } } + S ( 0 ) \mathrm { e } ^ { - r _ { \mathrm { d i v } } T } - X \mathrm { e } ^ { - r T } ) \mathrm { e } ^ { r T } > 0 .$ 

On the other hand, if $C ^ { \mathrm { E } } - P ^ { \mathrm { E } } > S ( 0 ) \mathrm { e } ^ { - r _ { \mathrm { d i v } } T } - X \mathrm { e } ^ { - r T }$ , then the opposite strategy will also lead to arbitrage. 

7.7 The strike price is equal to the forward price (more precisely, the exchange rate) of 0.9883 euros to a dollar computed in Solution 6.5. 

7.8 If $S ( 0 ) - X \mathrm { e } ^ { - r T } < C ^ { \mathrm { A } } - P ^ { \mathrm { A } }$ , then write and sell a call, buy a put, and buy a share, investing (or borrowing, if negative) the balance at the rate $^ r .$ . Now the same argument as in the first part of the proof of Theorem 7.2 applies, except that the arbitrage profit may also include the dividend if the call i exercised after the dividend becomes due. (Nevertheless, the dividend cannot be included in this inequality because the option may be exercised and the share sold before the dividend is due.) 

If $C ^ { \mathrm { A } } - P ^ { \mathrm { A } } < S ( 0 ) - \mathrm { d i v } _ { 0 } - X$ , then at time 0 sell short a share, write and sell a put, and buy a call option, investing the balance at the rate r. If the put is exercised at time $t < T$ , you will have to buy a share for $X$ , borrowing the amount at the rate r. As the dividend becomes due, borrow the amount at the rate r and pay it to the owner of the share. At time $T$ return the share to the owner, closing the short sale. You will be left with the call option and a positive amount $( S ( 0 ) + P ^ { \mathrm { A } } - C ^ { \mathrm { A } } - \mathrm { d i v } _ { 0 } ) \mathrm { e } ^ { r T } - X \mathrm { e } ^ { r ( T - t ) } > X \mathrm { e } ^ { r T } - X \mathrm { e } ^ { r ( T - t ) } \geq 0$ . (If the put is exercised before the dividend becomes due, you can increase your arbitrage profit by closing out the short position in stock immediately, in which case you would not have to pay the dividend.) If the put is not exercised before expiry $T$ , then the second part of Solution 7.5 applies. 

7.9 If $S ( 0 ) - X \mathrm { e } ^ { - r T } < C ^ { \mathrm { A } } - P ^ { \mathrm { A } }$ , then use the same strategy as in the first part of the proof of Theorem 7.2. The resulting arbitrage profit will in fact be increased by the dividends accumulated up to the time when the call option is exercised. 

If $C ^ { \mathrm { A } } - P ^ { \mathrm { A } } < S ( 0 ) \mathrm { e } ^ { - r _ { \mathrm { d i v } } T } - X$ , then at time 0 sell short $\mathbf { e } ^ { - r _ { \mathrm { { d i v } } } T }$ of $\mathrm { a }$ share, write and sell a put, and buy a call option, investing the balance at the rate r. Between time 0 and $T$ pay dividends to the stock owner, raising cash by shorting the stock. This will lead to one shorted share held at time T. If the put option is exercised at time $t \leq T$ , you will have to buy a share for $X$ borrowing this amount at the rate r. At time $T$ use this share to close the short position in stock. You will be left with a call option and a positive amount $( - C ^ { \mathrm { A } } + P ^ { \mathrm { A } } + S ( 0 ) \mathrm { e } ^ { - r _ { \mathrm { d i v } } T } ) \mathrm { e } ^ { r T } - X \mathrm { e } ^ { r ( T - t ) } \geq ( - C ^ { \mathrm { A } } + P ^ { \mathrm { A } } + S ( 0 ) \mathrm { e } ^ { - r _ { \mathrm { d i v } } T } - C ( 0 ) \mathrm { e } ^ { r ( T - t ) } )$ $X ) \mathrm { e } ^ { r T } > 0$ plus any dividends accumulated since the share was bought at time t. If the put option is not exercised at all, then you can use the call to buy a share for X at time $T$ , closing the short position in stock. You will also be left with a positive final balance $( - C ^ { \mathrm { \scriptscriptstyle A } } + \mathrm { \Large ~ \bar { P } ^ { \mathrm { \scriptscriptstyle A } } ~ } + S ( 0 ) { \mathrm e } ^ { - r _ { \mathrm { d i v } } T } ) { \mathrm e } ^ { r T } - X >$ $( - C ^ { \mathrm { A } } + P ^ { \mathrm { A } } + S ( 0 ) \mathrm { e } ^ { - r _ { \mathrm { d i v } } T } - X ) \mathrm { e } ^ { r T } > 0 .$ 

7.10 If $C ^ { \mathrm { E } } > C ^ { \mathrm { A } } ,$ , then write and sell a European call and purchase an American call. The diference $C ^ { \mathrm { E } } - C ^ { \mathrm { A } }$ will be your arbitrage income. To keep it, do not exercise the American option until expiry, when either both options will turn out worthless, or the loss from settling the European call will be recovered by exercising the American call. The argument for put options is similar. 

7.11 Suppose that $C ^ { \mathrm { E } } \geq S ( 0 ) - \mathrm { d i v } _ { 0 }$ . In this case write and sell a call option and buy stock, investing the balance on the money market. As soon as you receive the dividends, also invest them on the money market. On the exercise date you can sell the stock for at least min $( S ( T ) , \bar { X } )$ , settling the call option. Your final wealth will be positive, $( C ^ { \mathrm { E } } - S ( \dot { 0 } ) + \mathrm { d i v } _ { 0 } ) \mathbf { e } ^ { r T } + \operatorname* { m i n } ( S ( T ) , X ) > 0$ . This proves that $C ^ { \mathrm { E } } < S ( 0 ) - \mathrm { d i v } _ { 0 }$ 

The remaining bounds follow by the put-call parity relation (7.5) for dividend-paying stock: $\begin{array} { r } { S ( 0 ) - \mathrm { { d i v } } _ { 0 } - X \mathrm { e } ^ { - r T } \le C ^ { \mathrm { { E } } } , } \end{array}$ since $P ^ { \mathrm { E } } \ge 0 ; - S ( 0 ) +$ 0 $\mathrm { 4 i v } _ { 0 } + X \mathrm { e } ^ { - \bar { r } T } \leq P ^ { \mathrm { E } }$ , since $C ^ { \mathrm { E } } \geq 0 ;$ and $P ^ { \mathrm { E } } < X \mathrm { e } ^ { - r T }$ , since $C ^ { \mathrm { E } } < S ( 0 ) - \mathrm { d i v } _ { 0 }$ 

7.12 For dividend-paying stock the regions determined by the bounds on call and put prices in Proposition 7.3 are shown as shaded areas in Figure S.9. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/9dccfaaa5e9833d63a3d3af88f8578969cfc52cdfead96b940b7ff1c687daf10.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/d7c97f80-0af5-4c7b-b9b4-fcc26bb20c77/52a92ed9baa60d683a30c3e64e19e58991426a5ede216a98834de2681ff6ab4c.jpg)



Figure S.9 Bounds on European call and put prices for dividend-paying stock


7.13 If ${ \cal C } ^ { \mathrm { A } } \ge { \cal S } ( 0 )$ , then buy a share, write and sell an American call and invest the balance $C ^ { \mathrm { A } } - S ( 0 )$ without risk. If the option is exercised before or at expiry, then settle your obligation by selling the share for X. If the option is not exercised at all, you will end up with the share worth $S ( T )$ at expiry. In either case the final cash value of this strategy will be positive. The final balance will in fact also include the dividend collected, unless the option is exercised before the dividend becomes due. 

7.14 Suppose that $X ^ { \prime } \ < \ X ^ { \prime \prime }$ , but $C ^ { \mathrm { E } } ( X ^ { \prime } ) \ \leq \ C ^ { \mathrm { E } } ( X ^ { \prime \prime } )$ . We can write and sell a call with strike price $X ^ { \prime \prime }$ and buy a call with strike price $X ^ { \prime }$ , investing the diference $C ^ { \mathrm { E } } ( X ^ { ' \prime } ) - C ^ { \mathrm { E } } ( X ^ { \prime } )$ without risk. If the option with strike price $X ^ { \prime \prime }$ is exercised at expiry, we will need to pay $( S ( T ) - X ^ { \prime \prime } ) ^ { + }$ . This amount can be raised by exercising the option with strike price $X ^ { \prime }$ and cashing the payof $( S ( T ) - X ^ { \prime } ) ^ { + }$ . Because $X ^ { \prime } < X ^ { \prime \prime }$ and $( S ( T ) - X ^ { \prime } ) ^ { + } \ : \ge \ : ( S ( T ) - X ^ { \prime \prime } ) ^ { + }$ with strict inequality whenever $X ^ { \prime } < S ( t )$ , it follows that an arbitrage profit will be realised. 

The inequality for puts follows by a similar arbitrage argument. 

7.15 Consider four cases: 

1) If $S ( T ) \leq X ^ { \prime } < X < X ^ { \prime \prime }$ , then (7.9) reduces to $0 \leq 0$ 

2) If $X ^ { \prime } < S ( T ) \leq X < X ^ { \prime \prime }$ , then (7.9) becomes $0 \le \alpha \left( S ( T ) - X ^ { \prime } \right)$ obviously satisfied for $X ^ { \prime } < \mathop { S } ( T )$ 

3) If $X ^ { \prime } < X < S ( T ) \leq X ^ { \prime \prime }$ , then (7.9) can be written as $S ( T ) - X \leq$ $\alpha \left( S ( T ) - X ^ { \prime } \right)$ . This holds because $X = \alpha X ^ { \prime } + ( 1 - \alpha ) X ^ { \prime \prime }$ and $S ( T ) \leq$ $X ^ { \dag \prime }$ 

4) Finally, if $X ^ { \prime } < X < X ^ { \prime \prime } < S ( T )$ , then $( 7 . 9 )$ becomes an equality, $S ( T ) { \overset { . . . } { - } } X = \alpha \left( S ( T ) - X ^ { \prime } \right) + \left( 1 - \alpha \right) \left( S ( T ) - { \overset { . . . } { X ^ { \prime \prime } } } \right)$ because $X = \alpha X ^ { \prime } +$ $( 1 - \alpha ) X ^ { \prime \prime } .$ 

7.16 Suppose that $P ^ { \mathrm { E } } ( S ^ { \prime } ) \le P ^ { \mathrm { E } } ( S ^ { \prime \prime } )$ for some $S ^ { \prime } < S ^ { \prime \prime }$ , where $S ^ { \prime } = x ^ { \prime } S ( 0 )$ and $S ^ { \prime \prime } \bar { = } x ^ { \prime \prime } S ( 0 )$ . Write and sell a put option on a portfolio with $x ^ { \prime \prime }$ shares and buy a put option on a portfolio with $x ^ { \prime }$ shares, investing the balance $P ^ { \mathrm { E } } ( S ^ { \prime \prime } ) -$ $P ^ { \mathrm { E } } ( S ^ { \prime } )$ without risk. If the written option is exercised at time $T _ { \mathbf { \delta } }$ , then the liability can be met by exercising the other option. Since $x ^ { \prime } < x ^ { \prime \prime }$ , the payof satisfy $( X - x ^ { \prime } S ( T ) ) ^ { + } \geq ( X - x ^ { \prime \prime } S ( T ) ) ^ { + }$ with strict inequality whenever $X \geq$ $x ^ { \prime } S ( \bar { T } )$ . It follows that this is an arbitrage strategy. 

7.17 Suppose that $X ^ { \prime } < X ^ { \prime \prime } .$ , but $C ^ { \mathrm { A } } ( X ^ { \prime } ) \le C ^ { \mathrm { A } } ( X ^ { \prime \prime } )$ . We can write and sell the call with strike price $X ^ { \prime \prime }$ and purchase the call with strike price $X ^ { \prime }$ , investing the balance $C ^ { \mathrm { { A } } } \bar { ( } X ^ { \prime \prime } ) - C ^ { \mathrm { { A } } } ( X ^ { \prime } \bar { ) }$ without risk. If the written option is exercised at time $t \leq T$ , we will have to pay $( S ( t ) - X ^ { \prime \prime } ) ^ { + }$ . This liability can be met by exercising the other option immediately, receiving the payof $( S ( t ) - X ^ { \prime } ) ^ { + }$ Since $( S ( t ) - X ^ { \prime \prime } ) ^ { + } \leq ( S ( t ) - X ^ { \prime } ) ^ { + }$ with strict inequality whenever $X ^ { \prime } < S ( t )$ , this strategy leads to arbitrage. 

The inequality for put options can be proved in a similar manner. 

7.18 We shall prove Proposition 7.19 for American put options. The argument for European puts is similar. By Proposition $7 . 1 5 { \bar { \cal P } } ^ { \mathrm { A } } ( { \bar { \cal S } } )$ is a decreasing function of S. When $S \geq X$ , the intrinsic value of a put option is zero, and so the time value, being equal to $P ^ { \mathrm { { A } } } ( S )$ , is also a decreasing function of S. On the other hand, $P ^ { \mathrm { A } } ( S ^ { \prime } ) - P ^ { \mathrm { A } } ( S ^ { \prime \prime } ) \stackrel { . } { \leq } S ^ { \prime \prime } - S ^ { \prime }$ for any $S ^ { \prime } < S ^ { \prime \prime }$ by Proposition 7.16. This implies that $P ^ { \mathrm { A } } ( S ^ { \prime } ) - ( X - S ^ { \prime } ) ^ { + } \le P ^ { \mathrm { A } } ( S ^ { \prime \prime } ) - ( X - S ^ { \prime \prime } ) ^ { + } \mathrm { ~ i f ~ } S ^ { \prime } < S ^ { \prime \prime } \le X$ , so the time value is an increasing function of $S$ for $S \leq X$ . As a result, the time value has a maximum at $S = X$ 

## Chapter 8

8.1 Let us compute the derivative of the price $C ^ { \mathrm { E } } ( 0 )$ of a call option with respect to u. The formula for the price, assuming that $S ^ { \mathrm { d } } < X < S ^ { \mathrm { u } }$ , is 

$$
C ^ {\mathrm{E}} (0) = \frac {1}{1 + r} \frac {r - d}{u - d} [ S (0) (1 + u) - X ].
$$

The derivative with respect to u is equal to 

$$
\frac {(r - d) [ X - S (0) (1 + d) ]}{(1 + r) (u - d) ^ {2}} = \frac {(r - d) [ X - S ^ {\mathrm{d}} ]}{(1 + r) (u - d) ^ {2}}.
$$

This is positive in our situation, since $r > d$ and $X > S ^ { \mathrm { d } }$ , so $C ^ { \mathrm { E } } ( 0 )$ increases as u increases. 

The derivative of $C ^ { \mathrm { E } } ( 0 )$ with respect to d is equal to 

$$
- \frac {(u - r) [ S (0) (1 + u) - X ]}{(1 + r) (u - d) ^ {2}} = - \frac {(u - r) [ S ^ {\mathrm{u}} - X ]}{(1 + r) (u - d) ^ {2}},
$$

which is negative, since $r < u$ and $X < S ^ { \mathrm { u } }$ . The option price decreases as $d$ increases. 

8.2 If $r = 0$ and $S ( 0 ) = X = 1$ , then $\begin{array} { r } { C ^ { \mathrm { E } } ( 0 ) = \frac { - u d } { u - d } } \end{array}$ . For $u = 0 . 0 5$ and $d = - 0 . 0 5$ we have $u - d = 0 . 1$ and $C ^ { \mathrm { E } } ( 0 ) = 0 . 0 2 5$ dollars. However, if $u = 0 . 0 1$ and $d = - 0 . 1 9$ , then $u - d = 0 . 2$ . The variance of the return on stock is equal to $( u - d ) ^ { 2 } p ( 1 - p )$ and is higher in the latter case, but the option price is lower: $C ^ { \mathrm { E } } ( 0 ) = 0 . 0 0 9 5$ dollars. 

8.3 To replicate a call option the writer needs to buy stock initially and sell it when the option is exercised. The following system of equations needs to be solved to find the replicating portfolio: 

$$
\left\{ \begin{array}{l l} 1 1 0 (1 - c) x + 1. 0 5 y = 1 0, \\ 9 0 (1 - c) x + 1. 0 5 y = 0. \end{array} \right.
$$

For $c = 2 \%$ we obtain $x \cong 0 . 5 1 0 2$ and $y \cong - 4 2 . 8 4 7 1$ , so the initial value of the replicating portfolio will be 100x + $y \cong 8 . 1 6 3 3$ dollars. If $c = 0$ , then the replicating portfolio will be worth 7.1429 dollars. Note that the money marke position $_ y$ is the same for each c. 

8.4 The borrowing rate should be used to replicate a call, since the money market position will be negative. This gives $x ( 1 ) \cong 0 . 6 6 6 7$ and $y ( 1 ) \cong - 4 0 . 1 7 8 6 .$ , so the replicating portfolio value is 9.8214 dollars. For a put we obtain ${ \mathfrak { c } } ( 1 ) \cong - 0$ .3333 and $y ( 1 ) \cong \mathsf { 2 7 } . 7 7 7 8$ using the rate for deposits, so the replicating portfolio will be worth 2.7778 dollars initially. 

The results are consistent with the put and call prices obtained from (8.3) with the appropriate risk-neutral probability (computed using the correspond ing interest rate), $p _ { * } \cong 0 . 7 3 3 3$ for a call and $p _ { * } \cong 0 . 6$ for a put. 

8.5 The option price at time 0 is 22.92 dollars. In addition to this amount, the option writer should borrow 74.05 dollars and buy 0.8081 of a share. At time 1, if $S ( 1 ) = 1 4 4$ , then the amount of stock held should be increased to 1 share, the purchase being financed by borrowing a further 27.64 dollars, increasing the total amount of money owed to 109.09 dollars. If, on the other hand, $S ( 1 ) = 1 0 8$ dollars at time 1, then some stock should be sold to reduce the number of shares held to 0.2963, and 55.27 dollars should be repaid, reducing the amount owed to 26.18 dollars. (In either case the amount owed at time 1 includes interest of 7.40 dollars on the amount borrowed at time 0.) 

8.6 At time 1 the stock prices $S ^ { \mathrm { u } } = 1 4 4 ~ { \mathrm { a n d } } ~ S ^ { \mathrm { d } } = 1 0 8 $ dollars (the so-called cum dividend prices) drop by the amount of the dividend to 129 and 93 dollars (the so-called ex-dividend prices). These prices generate the prices at time $^ { 2 , }$ hence $S ^ { \mathrm { u u } } = 1 5 4 . 8 0 , S ^ { \mathrm { u d } } = 1 1 6 . 1 0 , S ^ { \mathrm { d u } } = 1 1 1 . 6 0 \mathrm { a n d } S ^ { \mathrm { d d } } = 8 3 . 7 0$ dollars. The option will be exercised with payof 34.80 dollars if the stock goes up twice. In the remaining scenarios the payof will be zero. The option value at time 1 will be 21.09 dollars in the up state and zero dollars in the down state. The replicating portfolio constructed at time 1 and based on ex-dividend prices consists of 0.8992 shares and a loan of 94.91 dollars in the up state, and no shares and no money market position in the down state. The option price at time 0 is 12.78 dollars. Replication (based on the cum-dividend prices at time 1, since the dividend is available to the owner of the stock purchased at time 0) involves buying 0.5859 shares and borrowing 57.52 dollars. 

8.7 From the Cox–Ross–Rubinstein formula $C ^ { \mathrm { E } } ( 0 ) \cong 5 . 9 3$ dollars, $P ^ { \mathrm { E } } ( 0 ) \cong 7 . 7 6$ dollars. 

8.8 The least integer m such that $S ( 0 ) ( 1 + u ) ^ { m } ( 1 + d ) ^ { N - m } \ > \ X$ is $m \ : = \ : 3 5$ From the Cox–Ross–Rubinstein formula we obtain $C ^ { \mathrm { E } } ( 0 ) ~ \cong ~ 3 . 4 6 6 1$ dollars and $x ( 1 ) = [ 1 - \varPhi ( m - 1 , N , q ) ] \cong 0 . 8 5 1 9 6$ shares. 

8.9 The delta of a European call becomes equal to 1 at the first step n such that the option will be in the money independently of whether the stock goes up or down at the next step, that is, $\bar { S } ( 0 ) ( 1 + \bar { u } ) ^ { n } ( 1 + d ) > X$ (in this case $S ( 0 ) ( 1 + u ) ^ { n + 1 } > X$ as well). This gives 

$$
n > \frac {\ln X - \ln S (0) - \ln (1 + d)}{\ln (1 + u)}.
$$

8.10 The stock values are 

<table><tr><td>n</td><td colspan="2">0</td><td colspan="2">1</td><td colspan="2">2</td><td>3</td></tr><tr><td rowspan="4">S(n)</td><td rowspan="4">60.00</td><td rowspan="4">&lt;</td><td rowspan="2">66.00</td><td rowspan="2">&lt;</td><td rowspan="2">72.60</td><td rowspan="2">&lt;</td><td>79.86</td></tr><tr><td>68.97</td></tr><tr><td rowspan="2">57.00</td><td rowspan="2">&lt;</td><td>62.70</td><td>&lt;</td><td>59.57</td></tr><tr><td>54.15</td><td>&lt;</td><td>51.44</td></tr></table>

The American put prices are 

$$
\begin{array}{c c c c c c c} n & 0 & & 1 & & 2 & & 3 \\ \hline & & & & & & 0. 0 0 \\ P ^ {\mathrm{A}} (n) & 2. 5 2 & <   & 0. 5 0 & <   & 0. 0 0 & <   \\ & & & \mathbf {5 . 0 0} & <   & 1. 1 0 & <   \\ & & & & & \mathbf {7 . 8 5} & <   \\ & & & & & & 1 0. 5 6 \end{array}
$$

The option will be exercised early in the d node at time 1 or in the dd node at time 2 (bold figures). 

8.11 The values of the European and American calls are the same, 

$$
\begin{array}{c c c c c} n & 0 & 1 & 2 \\ \hline & & & 5 2. 8 0 \\ C ^ {\mathrm{E}} (n) = C ^ {\mathrm{A}} (n) & 2 2. 9 2 & <   & 3 4. 9 1 & <   \\ & & 5. 8 2 & <   & 9. 6 0 \\ & & & & 0. 0 0 \end{array}
$$

At time 2 both options have, of course, the same payof. At time 1 the American call will not be exercised in the up state, as this would bring only 24 dollars, which less than the value of holding the option until expiry. In the down state the American call will be out of the money and will not be exercised either. Similarly, it will not be exercised at time 0. As a result, the American call is equivalent to its European counterpart. 

## 8.12 The ex-dividend stock prices are

<table><tr><td>n</td><td>0</td><td>1</td><td>2</td></tr><tr><td></td><td></td><td>11.20</td><td>&lt; 12.32</td></tr><tr><td rowspan="3">S(n)ex-div</td><td rowspan="3">12.00</td><td>/</td><td>10.64</td></tr><tr><td>\</td><td>10.34</td></tr><tr><td>9.40</td><td>&lt; 8.93</td></tr></table>

The corresponding European and American put prices will be 

<table><tr><td>n</td><td>0</td><td>1</td><td>2</td></tr><tr><td></td><td></td><td></td><td>1.68</td></tr><tr><td></td><td></td><td></td><td>1.68</td></tr><tr><td></td><td></td><td>2.53</td><td rowspan="2">&lt;</td></tr><tr><td></td><td></td><td>2.80</td></tr><tr><td></td><td></td><td>/</td><td>3.36</td></tr><tr><td></td><td></td><td></td><td>3.36</td></tr><tr><td><eq>P^{\text{E}}(n)</eq></td><td>3.42</td><td></td><td></td></tr><tr><td><eq>P^{\text{A}}(n)</eq></td><td>3.69</td><td></td><td></td></tr><tr><td></td><td></td><td>\</td><td>3.66</td></tr><tr><td></td><td></td><td></td><td>3.66</td></tr><tr><td></td><td></td><td>4.33</td><td rowspan="2">&lt;</td></tr><tr><td></td><td></td><td>4.60</td></tr><tr><td></td><td></td><td></td><td>5.07</td></tr><tr><td></td><td></td><td></td><td>5.07</td></tr></table>

At time 1 the payof of the American put option in both the up and down states will be higher than the value of holding the option to expiry, so the option should be exercised in these states (indicated by bold figures). 

8.13 Take b such that $S ( 0 ) \mathrm { e } ^ { \sigma b + r u - { \frac { 1 } { 2 } } \sigma ^ { 2 } u } = a$ and put $\begin{array} { r } { V ( t ) = W ( t ) + \left( m - r + \frac { 1 } { 2 } \sigma ^ { 2 } \right) \frac { t } { \sigma } } \end{array}$ for any $t \geq 0$ , which is a Wiener process under $P _ { * }$ <sub>. In particular,</sub> $V ( u )$ <sub>is nor-</sub> mally distributed under $P _ { * }$ with mean 0 and variance $u .$ . The right-hand side of (8.8) is therefore equal to 

$$
\begin{array}{l} E _ {*} \big (\mathrm{e} ^ {- r u} S (u) 1 _ {S (u) <   a} \big) = S (0) E _ {*} \Big (\mathrm{e} ^ {\sigma V (u) - \frac {1}{2} \sigma^ {2} u} 1 _ {V (u) <   b} \Big) \\ \qquad = S (0) \int_ {- \infty} ^ {b} \mathrm{e} ^ {\sigma x - \frac {1}{2} \sigma^ {2} u} \frac {1}{\sqrt {2 \pi t}} \mathrm{e} ^ {- \frac {x ^ {2}}{2 u}} \mathrm{d} x \\ \qquad = S (0) \int_ {- \infty} ^ {b} \frac {1}{\sqrt {2 \pi t}} \mathrm{e} ^ {- \frac {(x - \sigma u) ^ {2}}{2 u}} \mathrm{d} x. \end{array}
$$

Now observe that, since $V ( t )$ is a Wiener process under $P _ { * }$ , the random vari ables $V ( u )$ and $V ( t ) - V ( \dot { u } )$ are independent and normally distributed with mean 0 and variance u and $t - u$ , respectively. As a result, their joint density is $\textstyle { \frac { 1 } { 2 \pi t } } \mathrm { e } ^ { - { \frac { y ^ { 2 } } { 2 ( t - u ) } } - { \frac { x ^ { 2 } } { 2 u } } }$ . This enables us to compute the left-hand side of (8.8), 

$$
\begin{array}{l} E _ {*} \left(\mathrm{e} ^ {- r t} S (t) 1 _ {S (u) <   a}\right) = S (0) E _ {*} \Big (\mathrm{e} ^ {\sigma V (t) - \frac {1}{2} \sigma^ {2} u} 1 _ {V (u) <   b} \Big) \\ \qquad = S (0) E _ {*} \Big (\mathrm{e} ^ {\sigma (V (t) - V (u)) + \sigma V (u) - \frac {1}{2} \sigma^ {2} u} 1 _ {V (u) <   b} \Big) \\ \qquad = S (0) \int_ {- \infty} ^ {b} \left(\int_ {- \infty} ^ {\infty} \mathrm{e} ^ {\sigma y + \sigma x - \frac {1}{2} \sigma^ {2} t} \frac {1}{2 \pi t} \mathrm{e} ^ {- \frac {y ^ {2}}{2 (t - u)} - \frac {x ^ {2}}{2 u}} \mathrm{d} y\right) \mathrm{d} x \\ \qquad = S (0) \int_ {- \infty} ^ {b} \left(\int_ {- \infty} ^ {\infty} \frac {1}{2 \pi t} \mathrm{e} ^ {- \frac {(y - \sigma (t - u)) ^ {2}}{2 (t - u)} - \frac {(x - \sigma u) ^ {2}}{2 u}} \mathrm{d} y\right) \mathrm{d} x \\ \qquad = S (0) \int_ {- \infty} ^ {b} \frac {1}{\sqrt {2 \pi t}} \mathrm{e} ^ {- \frac {(x - \sigma u) ^ {2}}{2 u}} \mathrm{d} x \end{array}
$$

We can now see that the two sides of (8.8) are equal to one another. 

8.14 Consider the distribution function 

$$
\begin{array}{l} F (x) = P _ {*} \left\{W (t) <   x \right\} = P _ {*} \left\{V (t) <   x + \left(m - r + \frac {1}{2} \sigma^ {2}\right) \frac {t}{\sigma} \right\} \\ = \int_ {- \infty} ^ {x + \left(m - r + \frac {1}{2} \sigma^ {2}\right) \frac {t}{\sigma}} \frac {1}{\sqrt {2 \pi}} \mathrm{e} ^ {- \frac {y ^ {2}}{2}} \mathrm{d} y, \end{array}
$$

where $\begin{array} { r } { V ( t ) = W ( t ) + \left( m - r + \frac { 1 } { 2 } \sigma ^ { 2 } \right) \frac { t } { \sigma } } \end{array}$ is normally distributed under $P * \mathrm { . \ A s }$ a result, the density of $\mathbf { \dot { \boldsymbol { W } } } ( t )$ under ${ \dot { P } } _ { * }$ is 

$$
\frac {d F (x)}{d x} = \frac {1}{\sqrt {2 \pi}} \mathrm{e} ^ {- \frac {1}{2} \left(x + \left(m - r + \frac {1}{2} \sigma^ {2}\right) \frac {t}{\sigma}\right) ^ {2}}.
$$

8.15 By put-call parity, for $t = 0$ 

$$
\begin{array}{r l} P ^ {\mathrm{E}} (0) & = C ^ {\mathrm{E}} (0) - S (0) + X \mathrm{e} ^ {- r T} \\ & = S (0) (N (d _ {1}) - 1) - X \mathrm{e} ^ {- r T} (N (d _ {2}) - 1) \\ & = - S (0) N (- d _ {1}) + X \mathrm{e} ^ {- r T} N (- d _ {2}). \end{array}
$$

Now, by substituting t for 0 and $T - t$ for $T _ { i }$ , we obtain the Black–Scholes formula for $P ^ { \mathrm { E } } ( t )$ 

## Chapter 9

9.1 By put-call parity (7.1) 

$$
\frac {\mathrm{d}}{\mathrm{d} S} P ^ {\mathrm{E}} (S) = \frac {\mathrm{d}}{\mathrm{d} S} C ^ {\mathrm{E}} (S) - 1 = N (d _ {1}) - 1 = - (1 - N (d _ {1})) = - N (- d _ {1}),
$$

where $d _ { 1 }$ is given by (8.9). The delta of a put option is negative, consistently with the fact that the value of a put option decreases as the price of the underlying asset increases. 

9.2 We maximise 581 $. 9 6 \times S - 3 0 , 7 7 9 . 6 2 - 1 , 0 0 0 \times C ^ { \mathrm { E } } ( S , \frac { 1 } { 3 6 5 } )$ , where $S$ stands for the stock price after one day, and $C ^ { \mathrm { E } } ( S , t )$ is the price of a call at time $t ,$ one day in our case, with 89 days to maturity, and where $\sigma = 3 0 \%$ and $r = 8 \%$ as before. Equating the derivative with respect to $S$ to zero, we infer that the delta of the option after one day should be the same as the delta on day zero, $\textstyle { \frac { \mathrm { d } } { \mathrm { d } S } } C ^ { \mathrm { E } } ( S , { \frac { 1 } { 3 6 5 } } ) ^ { \bullet } = 0 . 5 8 1 9 6$ . This gives the following condition for the stock price (after inverting the normal distribution function): 

$$
\frac {\ln \frac {S}{6 0} + (r + \frac {1}{2} \sigma^ {2}) \times \frac {8 9}{3 6 5}}{\sigma \sqrt {\frac {8 9}{3 6 5}}} = \frac {\ln \frac {6 0}{6 0} + (r + \frac {1}{2} \sigma^ {2}) \times \frac {9 0}{3 6 5}}{\sigma \sqrt {\frac {9 0}{3 6 5}}}.
$$

The result is $S \cong 6 0 . 0 1 0 4$ dollars. 

9.3 The premium for a single put is 0.031648 dollars (from the Black–Scholes formula), so the bank will receive 1, 582.40 dollars by writing and selling 50, 000 puts. The delta of a single put is 0.355300, so the delta-hedging portfolio requires shorting 17, 765.00 shares, which will raise 32, 332.29 dollars. This gives a total of 33, 914.69 dollars received to be invested at 5%. The value of the delta neutral portfolio consisting of the shored stock, invested cash and sold options will be $- 3 2 , 3 3 2 . 2 9 + 3 3 , 9 1 4 . 6 9 - 1 , 5 8 2 . 4 0 = 0 . 0 0$ dollars. 

One day later the shorted shares will be worth $1 7 , 7 6 5 \times 1 . 8 1 = 3 2 , 1 5 4 . 6 4$ dollars, whereas the cash investment will grow to $3 3 , 9 1 4 . 6 9 \mathrm { e } ^ { 0 . 0 5 / 3 6 5 } \cong 3 3 , 9 1 9 . 3 4$ dollars. The put price will increase to 0.035182 dollars, so the price of 50, 000 puts will be 1, 759.11 dollars. The value of the delta neutral portfolio will be $- 3 2 , 1 5 4 . 6 4 + 3 3 , 9 1 9 . 3 4 - 1 , 7 5 9 . 1 1 \cong 5 . 5 9$ dollars. 

9.4 The price of a single put after one day will now be 0.038885 dollars, the 50, 000 options sold will therefore be worth 1944.26 dollars, the stock and cash deposit positions remaining as in Solution 9.3. The delta neutral portfolio will bring a loss of 179.56 dollars. 

9.5 If the stock price does not change, $S ( t ) = S ( 0 ) = S ($ , then the value of the portfolio after time t will be given by 

$$
V (t) = S N (d _ {1}) - X \mathrm{e} ^ {r t} \mathrm{e} ^ {- r T} N (d _ {2}) - C ^ {\mathrm{E}} (S, t),
$$

where $C ^ { \mathrm { E } } ( S , t )$ is given by the Black–Scholes formula and $d _ { 1 } , d _ { 2 }$ by (8.9). Then 

$$
\begin{array}{r l} & {\frac {\mathrm{d}}{\mathrm{d} t} V (t) \bigg | _ {t = 0} = - r X \mathrm{e} ^ {- r T} N (d _ {2}) - \left. \frac {\mathrm{d}}{\mathrm{d} t} C ^ {\mathrm{E}} (S, t) \right| _ {t = 0}} \\ & {\qquad = - r X \mathrm{e} ^ {- r T} N (d _ {2}) - \mathrm{theta} _ {C ^ {\mathrm{E}}}} \\ & {\qquad = \frac {\sigma S}{2 \sqrt {2 \pi T}} \mathrm{e} ^ {- d _ {1} ^ {2} / 2},} \end{array}
$$

which is positive. 

9.6 Using put-call parity and the Greek parameters for a call, we can find those for a put: 

$$
\begin{array}{r l} & {\mathrm{delta} _ {P \mathrm{E}} = N (d _ {1}) - 1 = \mathrm{delta} _ {C \mathrm{E}} - 1 = - N (- d _ {1}),} \\ & {\mathrm{gamma} _ {P \mathrm{E}} = \mathrm{gamma} _ {C \mathrm{E}},} \\ & {\mathrm{theta} _ {P \mathrm{E}} = - \frac {S \sigma}{2 \sqrt {2 \pi T}} \mathrm{e} ^ {- \frac {d _ {1} ^ {2}}{2}} + r X \mathrm{e} ^ {- r T} N (- d _ {2}),} \\ & {\mathrm{vega} _ {P \mathrm{E}} = \mathrm{vega} _ {C \mathrm{E}},} \\ & {\mathrm{rho} _ {P \mathrm{E}} = - T X \mathrm{e} ^ {- r T} N (- d _ {2}).} \end{array}
$$

(The Greek parameters are computed at time $t = 0 . )$ These equalities can also be verified directly by diferentiating the Black–Scholes formula for the put price. 

9.7 The rho of the original option is 7.5878, the delta of the additional option is 0.4104 and the rho is 7.1844. The delta-rho neutral portfolio requires buying approximately 148.48 shares of stock and 1, 056.14 additional options, while borrowing $7, 693.22. The position after one day is presented in the following table, in which we also recall the results of the delta hedge: 

<table><tr><td rowspan="2"><eq>S(\frac{1}{365})</eq></td><td colspan="3">delta-rho</td><td>delta</td></tr><tr><td>r=8%</td><td>r=9%</td><td>r=15%</td><td>r=9%</td></tr><tr><td>58.00</td><td>-7.30</td><td>-9.65</td><td>-26.14</td><td>-133.72</td></tr><tr><td>58.50</td><td>-2.71</td><td>-4.63</td><td>-17.95</td><td>-97.22</td></tr><tr><td>59.00</td><td>0.18</td><td>-1.23</td><td>-10.93</td><td>-72.19</td></tr><tr><td>59.50</td><td>1.59</td><td>0.77</td><td>-4.85</td><td>-58.50</td></tr><tr><td>60.00</td><td>1.76</td><td>1.60</td><td>0.52</td><td>-55.96</td></tr><tr><td>60.50</td><td>0.92</td><td>1.50</td><td>5.45</td><td>-64.38</td></tr><tr><td>61.00</td><td>-0.68</td><td>0.72</td><td>10.16</td><td>-83.51</td></tr><tr><td>61.50</td><td>-2.78</td><td>-0.47</td><td>14.90</td><td>-113.07</td></tr><tr><td>62.00</td><td>-5.13</td><td>-1.84</td><td>19.91</td><td>-152.78</td></tr></table>

9.8 With 95% probability the logarithmic return on the exchange rate satisfies $k > m + x \sigma \cong - 2 3 . 6 8 \%$ , where $x \cong - 1 . 6 4 5$ , so that $N ( x ) \cong { \mathrm { 5 \% } }$ . The 1, 000 dollars converted into euros, invested without risk at the rate rEUR, and converted back into dollars after one year, will give $1 , 0 0 0 \mathrm { e } ^ { r _ { \mathrm { E U R } } } \mathrm { e } ^ { k }$ dollars. With probability 95% this amount will satisfy 

$$
1, 0 0 0 \mathrm{e} ^ {r _ {\mathrm{EUR}}} \mathrm{e} ^ {k} > 1, 0 0 0 \mathrm{e} ^ {r _ {\mathrm{EUR}}} \mathrm{e} ^ {m + x \sigma} \cong 8 2 1. 4 0 \text { dollars }.
$$

On the other hand, 1, 000 dollars invested at the rate rUSD would have grown to $1 , 0 0 0 \mathrm { e } ^ { r \mathrm { U S D } } \cong 1$ , 051.27 dollars. As a result, 

$$
\mathrm{VaR} = 1, 0 0 0 \mathrm{e} ^ {r _ {\mathrm{USD}}} - 1, 0 0 0 \mathrm{e} ^ {r _ {\mathrm{EUR}}} \mathrm{e} ^ {m + x \sigma} \cong 2 2 9. 8 8 \text { dollars }.
$$

9.9 A single call costs $21.634. We purchase approximately 46.22 options. With probability 5% the stock price will be less than $49.74. We shall still be able to exercise the options, cashing $450.18 in the borderline case. The alternative risk-free investment of $1, 000 at 8% would grow to $1, 040.81. Hence VaR ∼= 590.63 dollars. If the stock grows at the expected rate, reaching $63.71, then we shall obtain $1, 095.88 when the options are exercised. With $5 \%$ probability the stock price will be above $81.6 and then our options will be worth at leas $1, 922.75. 

9.10 The cost of a single bull spread is $0.8585, with expected return 29.6523%, standard deviation 99.169%, and VaR equal to $15, 000 (at 74.03% confidence level). If 92.95% of the capital is invested without risk and the remainder in the bull spread, then the expected return will the same as on stock, with risk of 6.9957% and VaR equal to $650. 

9.11 A put with strike price $56 costs $0.426. A put with strike price $58 costs $0.9282. The expected return on the bear spread is 111.4635%, the risk reaching 177.2334%. The worst case scenario (among those admitted by the analyst) is when the stock price drops to $58.59. In this scenario, which will happen with conditional probability 0.3901, the investor will lose everything, so $\mathrm { \bar { V a R } } = 1 5 , 0 0 0$ dollars at 60.99% confidence level. 

## Chapter 10

10.1 The yields are $y ( 0 ) \cong 1 4 . 0 8 \%$ and $y ( 3 ) \cong 1 3 . 6 3 \%$ . Thus $B ( 0 , 3 ) = \mathrm { e } ^ { - 3 \tau y ( 0 ) } \cong$ 0.9654 dollars. Arbitrage can be achieved as follows: 

At time 0 buy a 6-month bond for $B ( 0 , 6 ) = 0 . 9 3 2 0$ dollars, raising the money by issuing 0.9654 of a 3-month bond, which sells at $B ( 0 , 3 ) \cong 0 . 9 6 5 4$ dollars. 

At time 3 (after 3 months) issue 0.9989 of a 3-month bond, which sells at $B ( 3 , 6 ) \stackrel { \cdot } { = } 0 . 9 6 6 5$ dollars, and use the proceeds of $0.9654 to settle the fraction of a 3-month bond issued at time 0. 

At time 6 (after half a year) the 6-month bond bought at time 0 will pay $1, out of which $0.9989 will settle the fraction of a 3-month bond issued at time 3. 

The balance of $0.0011 will be the arbitrage profit. 

10.2 The implied rates are $y ( 0 ) \cong 1 2 . 3 8 \%$ and $y ( 6 ) \cong 1 3 . 0 6 \%$ . Investing $100, we can buy 106.38 bonds now and 113.56 after six months. The logarithmic return over one year is ln $( 1 1 3 . 5 6 / 1 0 0 ) \cong 1 2 . 7 2 \%$ , the arithmetic mean of the semi-annual returns. 

10.3 To achieve a return of $1 4 \%$ , we would have to sell the bond for $0 . 8 7 0 0 \mathrm { e } ^ { 1 4 \% } \cong$ 1.0007 dollars, which is impossible. (A zero-coupon bond can never fetch a price higher than its face value.) 

In general, we have to solve the equation $B ( 0 , 1 2 ) \mathrm { e } ^ { k } = \mathrm { e } ^ { - \tau y ( 6 ) }$ to find $y ( 6 )$ , where k is the prescribed logarithmic return. The left-hand side must be smaller than 1. 

10.4 During the first six months the rate is $y ( n ) ~ \cong ~ 8 . 3 4 \%$ , for $n = 0 , \ldots , 1 7 9 .$ and during the rest of the year $y ( n ) \cong 1 0 . 3 4 \%$ , for $n = 1 8 0 , \ldots , 3 6 0$ . The bond should be sold for $0 . 9 2 \mathrm { e } ^ { 4 . 8 8 \% } \cong 0 . 9 6 6 0$ dollars or more. This cannot be achieved during the first six months, since the highest price before the rate changes is $B ( \breve { 1 } 7 9 , 3 6 0 ) \cong 0 . 9 5 8 9$ dollars. On the day of the rate change $B ( 1 8 0 , 3 6 0 ) \cong 0 . 9 4 9 6$ dollars, and we have to wait until day $n = 2 4 0$ , on which the bond price will exceed the required $0.9660 for the first time. 

10.5 The rate can be found by using a spreadsheet with goal seek facility to solve the equation 

$$
1 0. 8 9 6 \times \left(1 0 + 1 0 \mathrm{e} ^ {- y (1)} + 1 0 \mathrm{e} ^ {- 2 y (1)} + 1 1 0 \mathrm{e} ^ {- 3 y (1)}\right) = 1, 0 0 0 \mathrm{e} ^ {k}.
$$

This gives $y ( 1 ) \cong 1 2 . 0 0 \%$ for $k = 1 2 \%$ in case a), $y ( 1 ) \cong 1 2 . 8 1 \%$ for $k = 1 0 \%$ in case b) and $y ( 1 ) \cong 1 1 . 1 9 \%$ for $k = 1 4 \%$ in case c). 

10.6 The numbers were found using an Excel spreadsheet with accuracy highe than the displayed 2 decimal points. 

10.7 Scenario 1: $1, 427.10; Scenario 2: $1, 439.69. 

10.8 Formula (10.2) can be applied directly to find $D \cong 1 . 6 8 4 6$ 

10.9 The duration is equal to 4 if the face value is $73.97. The smallest possible duration, which corresponds to face value $F = \$ 80$ , is about 2.80 years. For very high face values $F$ the duration is close to 5, approaching this number as $F$ goes to infinity. 

When $F = 1 0 0$ , the coupon value $C \cong 1 3 . 5 2$ gives duration of 4 years. If the coupon value is zero, then the duration is 5 years. For very high coupon values $\hat { C }$ tending to infinity the duration approaches about 2.80 years. 

10.10 Since the second derivative of $P ( y )$ is positive, 

$$
\begin{array}{l} \frac {\mathrm{d} ^ {2}}{\mathrm{d} y ^ {2}} P (y) = (\tau n _ {1}) ^ {2} C _ {1} \mathrm{e} ^ {- \tau n _ {1} y} + (\tau n _ {2}) ^ {2} C _ {2} \mathrm{e} ^ {- \tau n _ {2} y} + \dots + (\tau n _ {N}) ^ {2} (C _ {N} + F) \mathrm{e} ^ {- \tau n _ {N} y} \\ > 0, \end{array}
$$

P is a convex function of $y .$ 

10.11 Solving the system $6 = 2 w _ { A } + 3 . 4 w _ { B } , w _ { A } + w _ { B } = 1$ , we find $w _ { A } \cong - 1 . 8 5 7 1$ and $w _ { B } \cong 2 . 8 5 7 1$ . As a result, we invest $14, 285.71 to buy 14, 005.60 bonds B, raising the shortfall of $9, 285.71 by issuing 9, 475.22 bonds A. 

10.12 The yield on the coupon bond A is about 13.37%, so the price of the zerocoupon bond B is $87.48. The coupon bond has duration 3.29 and we find the weights to be $w _ { A } \cong 0 . 4 3 6 6$ and $w _ { B } \cong 0 . 5 6 3 4$ . This means that we invest $436.59 to buy 4.2802 bonds A and $563.41 to buy 6.4403 bonds B. 

10.13 Directly from the definition (10.2) of duration we compute the duration $D _ { t }$ at 

time t (note that the bond price grows by a factor of $\mathrm { e } ^ { y t } )$ ), 

$$
\begin{array}{l} D _ {t} = \frac {1}{\mathrm{e} ^ {y t} P (y)} \left((\tau n _ {1} - t) C _ {1} \mathrm{e} ^ {- y (\tau n _ {1} - t)} + \dots + (\tau n _ {N} - t) (C _ {N} + F) \mathrm{e} ^ {- y (\tau n _ {N} - t)}\right) \\ = \frac {1}{P (y)} \left((\tau n _ {1} - t) C _ {1} \mathrm{e} ^ {- \tau n _ {1} y} + \dots + (\tau n _ {N} - t) (C _ {N} + F) \mathrm{e} ^ {- \tau n _ {N} y}\right) \\ = D _ {0} - t, \end{array}
$$

since the weights $C _ { 1 } \mathrm { e } ^ { - \tau n _ { 1 } y } / P ( y ) , C _ { 2 } \mathrm { e } ^ { - \tau n _ { 2 } y } / P ( y ) , \dots , ( C _ { N } + F ) \mathrm { e } ^ { - \tau n _ { N } y } / P ( y )$ add up to one. 

10.14 Denote the annual payments by $C _ { 1 } , C _ { 2 }$ and the face value by F, so that 

$$
\begin{array}{l} {P (y) = C _ {1} \mathrm{e} ^ {- y} + (C _ {2} + F) \mathrm{e} ^ {- 2 y},} \\ {D (y) = \frac {C _ {1} \mathrm{e} ^ {- y} + 2 (C _ {2} + F) \mathrm{e} ^ {- 2 y}}{P (y)}.} \end{array}
$$

Compute the derivative of $D ( y )$ to see that it is negative: 

$$
\frac {\mathrm{d}}{\mathrm{d} y} D (y) = \frac {- C _ {1} (C _ {2} + F) \mathrm{e} ^ {- 3 y}}{P (y) ^ {2}} <   0.
$$

10.15 We first find the prices and durations of the bonds: $P _ { A } ( y ) \cong 1 2 0 . 7 2 , P _ { B } ( y ) \cong$ 434.95, $D _ { A } ( y ) \cong 1 . 8 4 7 1$ $D _ { B } ( y ) \cong 1 . 9 8 9 4$ . The weights w 7.46%, $w _ { B } \cong$ 107.46% give duration 2, which means that we have to buy 49.41 bonds B and issue 12.35 bonds A. After one year we shall receive $247.05 from the coupons of B and will have to pay the same amount for the coupons of A. Our final amount will be $23, 470.22, exactly equal to the future value of $20, 000 at 8%, independently of any rate changes. 

10.16 If the term structure is to be flat, then the yield $y ( 0 , 6 ) = 8 . 1 6 \%$ applies to any other maturity, which gives $B ( 0 , 3 ) = 0 . 9 7 9 8$ dollars and $B ( 0 , 9 ) = 0 . 9 4 0 6$ dollars. 

10.17 Issue and sell 500 bonds maturing in 6 months with $100 face value, obtaining $48, 522.28. Use this sum to buy 520.4054 one-year bonds. After 6 months settle the bonds issued by paying $50, 000. After one year cash the face value of the bonds purchased. The resulting rate is 8%. 

10.18 You need to deposit $1 0 0 , 0 0 0 \mathrm { { e } ^ { - 8 . 4 1 \% / 1 2 } \cong 9 9 , 3 0 1 . 6 2 }$ dollars for one month, which will grow to the desired level of $100, 000, and borrow the same amount for 6 months at 9.54%. Your customer will receive $100, 000 after 1 month and will have to pay 99, $3 0 1 . 6 2 \mathrm { e } ^ { 9 . 5 4 \% / 2 } \cong 1 0 4 , 1 5 3 . 0 9$ dollars after 6 months, which implies a forward rate of 9.77%. (The rate can be obtained directly from (10.5).) 

The rate for a 4-month loan starting in 2 months is 

$$
f (0, 2, 6) = \frac {6 \times 9.35\% - 2 \times 8.64\%}{4} \cong 10.09\% ,
$$

so a deposit at 10.23% would give an arbitrage opportunity. 

10.19 To see that the forward rates $f ( n , N )$ may be negative, let us analyse the case with $n = 0$ for simplicity. Then 

$$
f (0, N) = (N + 1) y (0, N + 1) - N y (0, N)
$$

and $f ( 0 , N ) < 0$ requires that $( N + 1 ) y ( 0 , N + 1 ) < N y ( 0 , N )$ . The border case is when $\begin{array} { r } { y ( 0 , N + 1 ) = \frac { N } { N + 1 } y ( 0 , N ) } \end{array}$ , which enables us to find a numerical example. For instance, for $N = 8$ and $y ( 0 , 8 ) = 9 \%$ a negative value $f ( 0 , 8 )$ will be obtained if $\begin{array} { r } { y ( 0 , 9 ) < \frac { 8 } { 9 } \times 9 \% = 8 \% } \end{array}$ 

10.20 Suppose that $f ( n , N )$ increases with N. We want to show that the same is true for 

$$
y (n, N) = \frac {f (n , n) + f (n , n + 1) + \cdots + f (n , N - 1)}{N - n}.
$$

This follows from the fact that if a sequence $a _ { n }$ increases, then so does the sequence of averages $\begin{array} { r } { S _ { n } = \frac { a _ { 1 } + \cdots + a _ { n } } { \infty } } \end{array}$ . To see this multiply the target inequality $S _ { n + 1 } > S _ { n }$ by $n ( n + 1 )$ to get (after cancellations) $n a _ { n + 1 } > a _ { 1 } + \cdot \cdot \cdot + a _ { n }$ . The latter is true, since $a _ { n + 1 } > a _ { i }$ for all $i = 1 , \ldots , n .$ 

10.21 The values of $B ( 0 , 2 ) , B ( 0 , 3 ) , B ( 1 , 3 )$ have no efect on the values of the money market account. 

10.22 a) For an investment of $100 in zero-coupon bonds, divide the initial cash by the price of the bond $B ( 0 , 3 )$ to get the number of bonds held, 102.82, which gives final wealth of $102.82. The logarithmic return is 2.78%. b) For an investment of $100 in single-period zero-coupon bonds, compute the number of bonds maturing at time 1 as $1 0 0 / B ( 0 , 1 ) \stackrel { \textstyle \circ } { \cong } 1 0 0 . 9 9$ . Then, at time 1 find the number of bonds maturing at time 2 in a similar $\mathrm { w a y } , 1 0 0 . 9 9 / B ( 1 , 2 ) \cong 1 0 1 . 5 4$ Finally, we arrive at $1 0 1 . 5 4 / B ( 2 , 3 ) \cong 1 0 2 . 5 1$ bonds, each giving a dollar at time 3. The logarithmic return is 2.48%. c) An investment of $100 in the money market account, for which we receive $1 0 0 A ( 3 ) \cong 1 0 2 . 5 1$ at time 3, produce the same logarithmic return of 2.48% as in b). 

## Chapter 11

11.1 We begin from the right, that is, from the face values of the bonds, first computing the values of $B ( 2 , 3 )$ in all states. These numbers together with the known returns give B(1, 3; u) and $B ( 1 , 3 ; { \mathrm { d } } )$ . These, in turn, determine the missing returns $k ( 2 , 3 ; \mathrm { u d } ) = 0 . 2 0 \% \ \mathrm { a n d } \ k ( 2 , 3 ; \mathrm { d d } ) = 0 . 1 6 \%$ . The same is done for the first step, resulting in $k ( 1 , 3 ; \mathrm { d } ) = 0 . 2 3 \%$ . The bond prices are given in Figure S.10. 

$$
B (0, 3) = 0. 9 9 3 6 \begin{array}{l} B (1, 3; u) = 0. 9 9 6 2 \\ B (1, 3; d) = 0. 9 9 5 9 \end{array} \begin{array}{l} B (2, 3; u u) = 0. 9 9 8 4 \\ B (2, 3; u d) = 0. 9 9 8 2 \\ B (2, 3; d u) = 0. 9 9 7 9 \\ B (2, 3; d d) = 0. 9 9 7 5 \end{array}
$$

Figure S.10 Bond prices in Solution 11.1 

11.2 Because of the additivity of the logarithmic returns, $k ( 1 , 3 ; \mathrm { u } ) + k ( 2 , 3 ; \mathrm { u u } ) +$ $k ( 3 , 3 ; \mathrm { u u u } ) = 0 . 6 4 \%$ gives the return in the period of three weeks. To obtain the yield we have to rescale it to the whole year by multiplying by 52/3, hence $y ( 0 , 3 ) = 1 1 . 0 9 \%$ . Note that we must have $\bar { k ( 1 , 3 ; \mathrm { u } ) } + \bar { k ( 2 , 3 ; \mathrm { u d } ) } + \bar { k } ( 3 , 3 ; \mathrm { u d u } ) =$ 

0.64% which allows us to find $k ( 2 , 3 ; \mathrm { u d } ) = 0 . 2 0 \%$ . The other missing returns can be computed in a similar manner, first $k ( 1 , 3 ; \mathrm { d } )$ ), then $k ( 2 , 3 ; \mathrm { d d } )$ 

11.3 The bond prices are given in Figure S.11. 

$$
\begin{array}{c} B (0, 1) = 0. 9 9 2 3 \\ B (0, 2) = 0. 9 8 4 5 \\ B (0, 3) = 0. 9 7 7 6 \end{array} \begin{array}{c} B (1, 2; u) = 0. 9 9 3 4 \\ B (1, 3; u) = 0. 9 8 3 2 \end{array} \begin{array}{c} B (2, 3; u u) = 0. 9 9 1 1 \\ B (2, 3; u d) = 0. 9 8 8 3 \end{array}
$$

Figure S.11 Bond prices in Solution 11.3 

11.4 The money market account is given in Figure S.12. Note that the values for the ‘up’ movements are lower than for the ‘down’ movements. This is related to the fact that the yield decreases as the bond price increases, and our trees are based on bond price movements. 

$$
A (0) = 1. 0 0 7 8 \begin{array}{c} A (1; u) = 1. 0 1 4 5 \\ A (1; d) = 1. 0 1 7 7 \end{array} \begin{array}{c} A (2; u u) = 1. 0 2 3 6 \\ A (2; u d) = 1. 0 2 6 5 \\ A (2; d u) = 1. 0 2 6 8 \\ A (2; d d) = 1. 0 2 8 1 \end{array}
$$

Figure S.12 Money market account in Solution 11.4 

11.5 The prices $B ( 1 , 2 ; \mathrm { u } ) = 0 . 9 9 8 0$ and $B ( 1 , 2 ; \mathrm { d } ) = 0 . 9 9 7 5$ are found by discounting the face value 1 to be received at time 2, using the short rates $r ( 1 ; \mathrm { u } )$ and $r ( 1 ; \mathrm { d } )$ . The price $B ( 0 , 2 ) = 0 . 9 9 4 4$ can be found by the replication procedure. 

11.6 At time 2 the coupons are 0.5227 or 0.8776, depending on whether we are in the up or down state at time 1. At time 1 the coupon is 0.9999. 

11.7 At time 1 we find $1 8 . 0 6 4 7 = ( 0 . 8 1 5 9 \times 2 0 + 0 . 1 8 4 1 \times 1 0 ) / 1 . 0 0 5 2$ in the up state and 1 $. 7 9 5 1 = ( 0 . 1 8 1 1 \times 1 0 + 0 . 8 1 8 9 \times 0 ) / 1 . 0 0 8 8 \mathrm { { i n } }$ the down state. Next, applying the same formula again, we obtain $7 . 9 1 8 8 \ : = \ : ( 0 . 3 8 1 3 \times 1 8 . 3 9 2 8 +$ $0 . 6 1 8 7 \times 1 . 7 9 5 1 ) / 1 . 0 1$ 

11.8 There is an arbitrage opportunity at time 1 in the up state. The price $B ( 1 , 2 ; { \mathrm { u } } ) = 0 . 9 9 2 4$ implies that the growth factor in the money market is 1.00766, whereas the prices of the bond maturing at time 3 imply growth factors 1.01159 and 1.00783. To realise arbitrage, bonds with maturity 3 should be bought, the purchase financed by a loan in the money market. 

11.9 Using formula (11.5) and the short rates given, we find the following structure of bond prices: 

$$
B (0, 3) = 0. 9 7 7 3 \begin{array}{c c c c} & B (1, 3; \mathrm{u}) = 0. 9 8 5 9 & <   & B (2, 3; \mathrm{uu}) = 0. 9 9 3 1 \\ / & & & B (2, 3; \mathrm{ud}) = 0. 9 9 2 6 \\ \backslash & & & B (2, 3; \mathrm{du}) = 0. 9 9 2 4 \\ & B (1, 3; \mathrm{d}) = 0. 9 8 4 3 & <   & B (2, 3; \mathrm{dd}) = 0. 9 9 2 3 \end{array}
$$

11.10 It is best to compute the risk-neutral probabilities. The probability at time 1 of the up movement based on the bond maturing at time 3 is 0.76, whereas the probability based on the bond maturing at time 2 is 0.61. The present price of the bond maturing at time 2 computed using the prices of the bond maturing at time 3 and the risk-neutral probabilities computed from these prices is 0.9867. So, shorting at time 0 the bond maturing at time 3 and buying the bond maturing at time 2 will give an arbitrage profit. 

11.11 At time 2 the option is worthless. At time 1 we evaluate the bond prices by adding the coupon to the discounted final payment of 101.00 at the appropriate (monthly) money market rate: 0.521% in the up state and 0.874% in the down state. The results are 101.4748 and 101.1213, respectively. The option can be exercised at that time in the up state, so the cash flow is 0.1748 and 0, respectively. Expectation with respect to the risk-neutral probabilities of the discounted cash flow gives the initial value 0.06598 of the option. 

11.12 The coupons of the bond with the floor provision difer from the par bond at time 2 in the up state: 0.66889 instead of 0.52272. This results in the following bond prices at time 1: 101.14531 in the up state and 100.9999 in the down state. (The latter is the same as for the par bond.) Expectation with respect to the risk-neutral probability gives the initial bond price 100.05489, so the floor is worth 0.05489. 

## Background Reading: Probability and Stochastic Processes

Ash, R. B. (1970), Basic Probability Theory, John Wiley & Sons, New York. 



Brze´zniak, Z. and Zastawniak, T. (1999), Basic Stochastic Processes, Springer Undergraduate Mathematics Series, Springer-Verlag, London. 



Capi´nski, M. and Kopp, P. E. (1999), Measure, Integral and Probability, Springer Undergraduate Mathematics Series, Springer-Verlag, London. 

Capi´nski, M. and Zastawniak, T. (2001), Probability Through Problems, Springer-Verlag, New York. 



Chung, K. L. (1974), A Course in Probability Theory, Academic Press, New York. 





Stirzaker, D. (1999), Probability and Random Variables. A Beginner’s Guide, Cambridge University Press, Cambridge. 



## Background Reading: Calculus and Linear Algebra



Blyth, T. S. and Robertson, E. F. (1998), Basic Linear Algebra, Springer Undergraduate Mathematics Series, Springer-Verlag, London. 





Jordan, D. W. and Smith, P.(2002), Mathematical Techniques, Oxford University Press, Oxford. 





Stewart, J. (1999), Calculus, Brooks Cole, Pacific Grove, California. 



## Further Reading: Mathematical Finance

Baxter, M. W. and Rennie, A. J. O. (1996), Financial Calculus, Cambridge University Press, Cambridge. 



Benninga, S. and Czaczkes, B. (1997), Financial Modeling, MIT Press, Cambridge, Mass. 





Bingham, N. H. and Kiesel, R. (1998), Risk-Neutral Valuation: Pricing and Hedging of Financial Derivatives, Springer-Verlag, Berlin. 





Bj¨ork, T. (1998), Arbitrage Theory in Continuous Time, Oxford University Press, Oxford. 





Chen, L. (1996), Interest Rate Dynamics, Derivatives Pricing, and Risk Management, Lecture Notes in Econom. and Math. Systems 435, Springer-Verlag, New York. 





Elliott, R. J. and Kopp, P. E. (1998), Mathematics of Financial Markets, Springer-Verlag, New York. 





Elton, E. J. and Gruber, M. J. (1995), Modern Portfolio Theory and Investment Analysis, John Wiley & Sons, New York. 





Haugen, R. A. (1993), Modern Investment Theory, Prentice Hall, Englewood Clifs, N.J. 





Hull, J. (2000), Options, Futures and Other Derivatives, Prentice Hall, Upper Saddle River, N.J. 





Jarrow, R. A. (1995), Modelling Fixed Income Securities and Interest Rate Options, McGraw-Hill, New York. 





Jarrow, R. A. and Turnbull, S. M., Derivative Securities, South-Western Col lege, Cincinnati, Ohio. 





Karatzas, I. and Shreve, S. (1998), Methods ofMathematical Finance, Springer-Verlag, Berlin. 





Korn, R. (1997), Optimal Portfolios, World Scientific, Singapore. 





Lamberton, D. and Lapeyre, B. (1996), Introduction to Stochastic Calculus Applied to Finance, Chapman and Hall, London. 





Musiela, M. and Rutkowski, M. (1997), Martingale Methods in Financial Modelling, Springer-Verlag, Berlin. 





Pliska, S. R. (1997), Introduction to Mathematical Finance: Discrete Time Models, Blackwell, Maldon, Mass. 





Wilmott, P. (2001), Paul Wilmott Introduces Quantitative Finance, John Wiley & Sons, Chichester. 





Wilmott, P., Howison, S. and Dewynne, J. (1995), The Mathematics of Financial Derivatives: A Student Introduction, Cambridge University Press, Cambridge. 



## Glossary of Symbols

$A$ fixed income (risk free) security price; money market account $B$ bond price $\beta$ beta factor $c$ covariance $C$ call price; coupon value $C$ covariance matrix $C ^ { \mathrm { A } }$ American call price $C ^ { \mathrm { E } }$ European call price $\widetilde { C } ^ { \mathrm { E } }$ discounted European call price Cov covariance delta Greek parameter delta $\operatorname { d i v }$ dividend $\mathrm { d i v _ { 0 } }$ present value of dividends $D$ derivative security price; duration $\widetilde { D }$ discounted derivative security price $D ^ { \mathrm { A } }$ price of an American type derivative security $E$ expectation $E _ { * }$ risk-neutral expectation $f$ futures price; payof of an option; forward rate $F$ forward price; future value; face value gamma Greek parameter gamma $\varPhi$ cumulative binomial distribution $k$ logarithmic return $K$ return $i$ coupon rate m compounding frequency; expected logarithmic return 

M market portfolio m expected returns as a row matrix $\mu$ expected return $N$ cumulative normal distribution $\binom { N } { k }$ the number of k-element combinations out of N elements $\omega$ scenario $\varOmega$ probability space $p$ branching probability in a binomial tree $p _ { * }$ risk-neutral probability $P$ put price; principal $P ^ { \mathrm { A } }$ American put price $P ^ { \mathrm { E } }$ European put price $\widetilde { P } ^ { \mathrm { E } }$ discounted European put price $\mathrm { P A }$ present value factor of an annuity $r$ interest rate $r _ { \mathrm { d i v } }$ dividend yield $r _ { \mathrm { e } }$ efective rate $r _ { F }$ risk-free return rho Greek parameter rho $\rho$ correlation $S$ risky security (stock) price $\widetilde { S }$ discounted risky security (stock) price $\sigma$ standard deviation: risk: volatility $t$ current time $T$ maturity time; expiry time; exercise time; delivery time $\tau$ time step theta Greek parameter theta u row matrix with all entries 1 $V$ portfolio value; forward contract value, futures contract value Var variance VaR value at risk vega Greek parameter vega w symmetric random walk; weights in a portfolio w weights in a portfolio as a row matrix $W$ Wiener process, Brownian motion x position in a risky security $X$ strike price y position in a fixed income (risk free) security; yield of a bond z position in a derivative security 

admissible – portfolio 5 – strategy 79, 88 American – call option 147 – derivative security 183 – put option 147 amortised loan 30 annuity 29 arbitrage 7 at the money 169 attainable – portfolio 107 – set 107 basis – of a forward contract 128 – of a futures contract 140 basis point 218 bear spread 208 beta factor 121 binomial – distribution 57, 180 – tree model 7, 55, 81, 174, 238 Black–Derman–Toy model 260 Black-Scholes – equation 198 – formula 188 bond – at par 42, 249 – callable 255 – face value 39 – fixed-coupon 255 – floating-coupon 255 – maturity date 39 

– stripped 230 – unit 39 – with coupons 41 – zero-coupon 39 Brownian motion 69 bull spread 208 butterfly 208 – reversed 209 call option 13, 181 – American 147 – European 147, 188 callable bond 255 cap 258 Capital Asset Pricing Model 118 capital market line 118 caplet 258 CAPM 118 Central Limit Theorem 70 characteristic line 120 compounding – continuous 32 – discrete 25 – equivalent 36 – periodic 25 – preferable 36 conditional expectation 62 contingent claim 18, 85, 148 – American 183 – European 173 continuous compounding 32 continuous time limit 66 correlation coeficient 99 coupon bond 41 coupon rate 249 

covariance matrix 107 Cox–Ingersoll–Ross model 260 Cox–Ross–Rubinstein formula 181 cum-dividend price 292 delta 174, 192, 193, 197 delta hedging 192 delta neutral portfolio 192 delta-gamma hedging 199 delta-gamma neutral portfolio 198 delta-vega hedging 200 delta-vega neutral portfolio 198 derivative security 18, 85, 253 – American 183 – European 173 discount factor 24, 27, 33 discounted stock price 63 discounted value 24, 27 discrete compounding 25 distribution – binomial 57, 180 – log normal 71, 186 – normal 70, 186 diversifiable risk 122 dividend yield 131 divisibility 4, 74, 76, 87 duration 222 dynamic hedging 226 efective rate 36 eficient – frontier 115 – portfolio 115 equivalent compounding 36 European – call option 147, 181, 188 – derivative security 173 – put option 147, 181, 189 ex-coupon price 248 ex-dividend price 292 exercise price 13, 147 time 13, 147 expected return 10, 53, 97, 108 expiry time 147 face value 39 fixed interest 255 fixed-coupon bond 255 flat term structure 229 floating interest 255 floating-coupon bond 255 floor 259 floorlet 259 

forward – contract 11, 125 – price 11, 125 – rate 233 fundamental theorem of asset pricing 83, 88 future value 22, 25 futures – contract 134 – price 134 gamma 197 Girsanov theorem 187 Greek parameters 197 growth factor 22, 25, 32 Heath–Jarrow–Morton model 261 hedging – delta 192 – delta-gamma 199 – delta-vega 200 – dynamic 226 in the money 169 initial – forward rate 232 – margin 135 – term structure 229 instantaneous forward rate 233 interest – compounded 25, 32 – fixed 255 – floating 255 – simple 22 – variable 255 interest rate 22 interest rate option 254 interest rate swap 255 LIBID 232 LIBOR 232 line of best fit 120 liquidity 4, 74, 77, 87 log normal distribution 71, 186 logarithmic return 34, 52 long forward position 11, 125 maintenance margin 135 margin call 135 market portfolio 119 market price of risk 212 marking to market 134 Markowitz bullet 113 martingale 63, 83 

martingale probability 63, 250 maturity date 39 minimum variance – line 109 – portfolio 108 money market 43, 235 

option – American 183 – at the money 169 – call 13, 147, 181, 188 – European 173, 181 – in the money 169 – interest rate 254 – intrinsic value 169 – out of the money 169 – payof 173 – put 18, 147, 181, 189 – time value 170 out of the money 169 

par, bond trading at 42, 249 payof 148, 173 periodic compounding 25 perpetuity 24, 30 portfolio 76, 87 – admissible 5 – attainable 107 – delta neutral 192 – delta-gamma neutral 198 – delta-vega neutral 198 expected return 108 – market 119 – variance 108 – vega neutral 197 positive part 148 predictable strategy 77, 88 preferable compounding 36 present value 24, 27 principal 22 put option 18, 181 – American 147 – European 147, 189 put-call parity 150 estimates 153 random interest rates 237 random walk 67 rate – coupon 249 – efective 36 

– forward 233 initial 232 instantaneous 233 – of interest 22 – of return 1, 49 – spot 229 regression line 120 residual random variable 121 residual variance 122 return 1, 49 – expected 53 – including dividends 50 – logarithmic 34, 52 reversed butterfly 209 rho 197 risk 10, 91 – diversifiable 122 – market price of 212 – systematic 122 – undiversifiable 122 risk premium 119, 123 risk-neutral – expectation 60, 83 market 60 – probability 60, 83, 250 

trinomial tree model 64 

underlying 85, 147 undiversifiable risk 122 unit bond 39 

value at risk 202 value of a portfolio 2 value of a strategy 76, 87 VaR 202 variable interest 255 Vasiˇcek model 260 

vega 197 vega neutral portfolio 197 volatility 71 

weights in a portfolio 94 Wiener process 69 

yield 216 yield to maturity 229 

zero-coupon bond 39 