

<!-- === Source: MinerU_markdown_Following_the_Trend－_Diversified_Managed_Futures_Trading._Andreas_Clenow_2013_1_2122155849542639629.md (Page 1) === -->

# Following the Trend

Diversified Managed Futures Trading 

Andreas F. Clenow 

Andreas F. Clenow 

WWW.FOLLOWINGTHETREND.COM 

WILEY 

A John Wiley & Sons, Ltd., Publication 

Registered office John Wiley & Sons Ltd, The Atrium, Southern Gate, Chichester, West Sussex, PO19 8SQ, United Kingdom 

For details of our global editorial offices, for customer services and for information about how to apply for permission to reuse the copyright material in this book please see our website at www.wiley.com. 

The right of the author to be identified as the author of this work has been asserted in accordance with the Copyright, Designs and Patents Act 1988 

All rights reserved. No part of this publication may be reproduced, stored in a retrieval system, or transmitted, in any form or by any means, electronic, mechanical, photocopying, recording or otherwise, except as permitted by the UK Copyright, Designs and Patents Act 1988, without the prior permission of the publisher. 

Wiley publishes in a variety of print and electronic formats and by print-on-demand. Some material included with standard print versions of this book may not be included in e-books or in print-on-demand. If this book refers to media such as a CD or DVD that is not included in the version you purchased, you may download this material at http://booksupport.wiley.com. For more information about Wiley products, visit www.wiley.com. 

Designations used by companies to distinguish their products are often claimed as trademarks. All brand names and product names used in this book are trade names, service marks, trademarks or registered trademarks of their respective owners. The publisher is not associated with any product or vendor mentioned in this book. 

Limit of Liability/Disclaimer of Warranty: While the publisher and author have used their best efforts in preparing this book, they make no representations or warranties with the respect to the accuracy or completeness of the contents of this book and specifically disclaim any implied warranties of merchantability or fitness for a particular purpose. It is sold on the understanding that the publisher is not engaged in rendering professional services and neither the publisher nor the author shall be liable for damages arising herefrom. If professional advice or other expert assistance is required, the services of a competent professional should be sought. 

Library of Congress Cataloging-in-Publication Data is available 

A catalogue record for this book is available from the British Library. 

ISBN 978-1-118-41085-1 (hbk) ISBN 978-1-118-41082-0 (ebk) ISBN 978-1-118-41083-7 (ebk) ISBN 978-1-118-41084-4 (ebk) 

To my wonderful wife Eng Cheng and my son Brandon for their love and patience 

## Table of Contents

Foreword....3
Preface....4
Acknowledgements....6
1....6
Cross-Asset Trend Following with Futures....6
2....18
Futures Data and Tools....18
3....41
Constructing Diversified Futures Trading Strategies....41
4....53
Two Basic Trend-Following Strategies....53
5....76
In-Depth Analysis of Trend-Following Performance....76
6....92
Year by Year Review....92
7....198
Reverse Engineering the Competition....198
8....215
Tweaks and Improvements....215
9....224
Practicalities of Futures Trading....224
10....229
Final Words of Caution....229
Bibliography....233
BOOKS....234
Index....234 

## Foreword

This book is an excellent training manual for anyone interested in learning how to make money as a trend follower. 

I know a bit about trend following because I was part of the famous Turtle experiment in the 1980s when Richard Dennis, the Prince of the Pits, showed the world that trading could be taught and that people with the right sort of training and perspective could make consistent returns that far exceeded normal investments. Ultimately, that ordinary people could learn to trade like the most successful hedge funds. I started as a 19-year-old kid and by the time I was 24 in 1987, I took home $8 million, which was my cut of the $31.5 million I earned for Richard Dennis as a trend follower. 

I even wrote a book about it, Way of the Turtle. It became a bestseller because many traders wanted to know the secrets of our success and to hear about the story first-hand which had been kept secret because of confidentiality agreements and our loyalty to Richard Dennis, a great man and a trading legend. 

I’d thought about writing a follow-on book a few times in the intervening years; something meatier and with more detail. My book was part-story and part-trading manual and I thought about writing a book tha was all trading manual. 

In Following the Trend, Andreas Clenow has written a trend-following trading manual I would be proud to put my own name on. I’m very picky too, so I don’t say this lightly. 

Very few trading books are worthy of an endorsement of any sort. Too many are filled with tips and tricks that don’t stand the test of the markets, let alone the test of time. Too many are written by those who are trying to sell you something like a course, or their seminars. Too many want your money more than they want to create an excellent book. 

That’s why I don’t often speak at conferences and you won’t see me endorsing many books. There is too much self-serving propaganda in the trading industry that makes its money by fleecing the unsuspecting newcomers; too many lies designed to rope in the neophytes with promises of easy profits and quick money that will never pan out. 

## Following the Trend is different.

It is solid, clearly written, covers all the basics, and it doesn’t promise you anything that you can’t actually get as a trend follower. 

If you want to be a trend follower, first, read Reminiscences of a Stock Operator to learn from Jesse Livermore. Then, buy Jack Schwager’s Market Wizards books to learn about the great traders who have been trend followers, like Richard Dennis my trading mentor, Ed Seykota, Bill Dunn, John W. Henry, and Richard Donchian. They will get you excited about the possibilities but leave you wondering how; how can you too learn to be a trend follower? 

Then, when you are ready to move from desire to reality. When you are ready to do it yourself. To make your own mark. 

Read Following the Trend. 

Curtis Faith 

Savannah, GA U.S.A. 

## Preface

This book is in essence about a single trading strategy based on a concept that has been publically known for at least two decades. It is a strategy that has worked remarkably well for over 30 years with a large number of hedge funds employing it. This strategy has been given much attention over the past few years and in particular after the dramatically positive returns it generated in 2008, but it seems nevertheless to be constantly misunderstood, misinterpreted and misused. Even worse, various flawed and overly complicated iterations of it are all too often sold for large amounts of money by people who have never even traded them in a professional environment. The strategy I am alluding to goes by many names but it is in essence the same strategy that most trend-following futures managers (or CTAs for Commodity Trading Advisors if you prefer) have been trading for many years. 

This book differs in many ways from the more traditional way in which trading literature tends to approach the subject of trend-following strategies. My primary reason for writing this book is to fill a gap in that literature and to make publicly available analyses and information that is already known by successful diversified trend followers, but understood by few not already in this very specialised part of the business. It is my belief that most books and therefore most people aspiring to get into this business are focusing on the wrong things, such as entry and exit rules, and missing the important aspects. This is likely related to the fact that many authors don’t actually design or trade these strategies for a living. 

There have been many famous star traders in this particular part of the industry and some of them have been raised to almost mythical status and seen as kinds of deities in the business. These people have my highest respect for their success and pioneer work in our field, but this book is not about hero worship and it does not dwell on strategies that worked in the 1970s but might be financial suicide to run in the same shape today. The market has changed and even more so the hedge-fund industry and I intend to focus on what I see as viable strategies in the current financial marketplace. 

This is not a text book where every possible strategy and indicator is explored in depth with comparisons of the pros and cons of exponential moving average to simple moving average, to adaptive moving average and so on. I don’t describe every trading indicator I can think of or invent new ones and name them after myself. You don’t need a whole bag of technical indicators to construct a solid trend-following strategy and it certainly does not add anything to the field if I change a few details of some formula and call the new one by my own name, although I have to admit that ‘The Clenow Oscillator’ does have a certain ring to it. Indicators are not important and focusing on these details is likely to be the easiest way to miss the whole plot and get stuck in nonsense curve fitting and over-optimisations. I intend to do the absolute opposite and use only the most basic methods and indicators to show how you can construct strategies good enough to use in professional hedge funds without having unnecessary complexity. The buy and sell rules are the least important part of a strategy and focusing on them would serve only to distract from where the real value comes. 

Also, this is not a get-rich-quick book. If you are looking for a quick and easy way to get rich you need to look elsewhere. One of my main points in this book is that it is not terribly difficult to create a trading strategy that can rival many large futures hedge funds but that absolutely does not mean that this is an easy business. Creating a trading strategy is only one step out of many and I even provide trading rules in this book that perform very well over time and have return profiles that are marketable to seasoned institutional investors. That is only part of the work though and if you don’t do your homework properly you will most likely end up either not getting any investments in the first place or blowing up your own and your investors’ money at the first sign of market trouble. 

To be able to use the knowledge I pass on here, you need to put in some really hard work. Don’t take anyone’s word when it comes to trading strategies, not even mine. You need to invest in a good market data infrastructure including effective simulation software and study a proper programming language if you don’t already know one. Then you can start replicating the strategies I describe here and make up your own mind about their usefulness, and I hope find ways to improve them and adapt to your own desired level of risk and return. Using someone else’s method out of the box is rarely a good idea and you need to make the strategies your own in order to really know and trust them. 

Even after you reach that stage, you have most of the work ahead of you. Trading these strategies on a daily basis is a lot tougher than most people expect, not least from a psychological point of view. Add the task of finding investors, launching a fund or managed accounts setup, running the business side, reporting, mid office and so on, and you soon realise that this is not a get-rich-quick scheme. It is certainly a highly rewarding business to be in if you are good at what you do, but that does not mean it is either easy or quick. 

So despite the stated fact that this book is essentially about a single strategy, I will demonstrate that this one strategy is sufficient to replicate the top trend-following hedge funds of the world, when you fully understand it. 

## WHY WRITE A BOOK?

Practically no managed futures funds will reveal their trading rules and they tend to treat their proprietary strategy as if they were blueprints for nuclear weapons. They do so for good reason but not necessarily for the reason most people would assume. The most important rationale for the whole secrecy business is likely tied to marketing, and the perception of a fund manager possessing the secret formula to make gold out of stone will certainly help to sell the fund as a unique opportunity. The fact of the matter is that although most professional trend followers have their proprietary tweaks, the core strategies used don’t differ very much in this business. That might sound like an odd statement, since I have obviously not been privy to the source code of all the managed futures funds out there and because they sometimes show quite different return profiles it would seem as if they are doing very different things. However, by using very simplistic methods one can replicate very closely the returns of many CTA funds and by tweaking the time horizons, risk factor and investment universe one can replicate most of them. 

This is not to say that these funds are not good or that they don’t have their own valuable proprietary algorithms. The point is merely that the specific tweaks used by each shop are only a small factor and that the bulk of the returns come from fairly simple models. Early on in this book I show two basic strategies and how even these highly simplistic models are able to explain a large part of CTA returns, and I then go on to refine these two strategies into one strategy that can compete well with the big established futures funds. I show all the details of how this is done, enabling the reader to replicate the same strategies. These strategies are tradable with quite attractive return profiles just as they are and I show in subsequent chapters how to improve upon them further. I intend to show not just simple examples but complete strategies that can be used straight away for institutional money management. 

And why would I go and tell you all of this? Wouldn’t the spread of this knowledge cause all trendfollowing strategies to cease functioning; free money would be given to the unwashed masses instead of the secret guild of hedge-fund managers and make the earth suddenly stop revolving and fling us all out into space? Well, there are many reasons quantitative traders give to justify their secrecy and keep the mystique up and a few of them are even valid, but in the case of trend-following futures I don’t see too much of a downside in letting others in on the game. The trend-following game is currently dominated by a group of massive funds with assets in the order of US$5–25 billion, which they leverage many times over to play futures all over the world. These fund managers know everything I write in this book and plenty more. The idea that me writing this book may cause so many people to go into the trend-following futures business that their trades would somehow overshadow the big players and destroy the investment opportunities is a nice one for my ego, but not a very probable one. What I describe here is already done on a massive scale and if a few of my readers decide to go into this field, good for them and I wish them the best of luck. 

What we are talking about here are simply methods to locate medium- to long-term trends typically caused by real economic developments and to systematically make money from them over time. Having more people doing the same will hardly change the real economic behaviour of humankind that is ultimately behind the price action. One could of course argue that a significant increase in assets in this game could make the exact entries and exits more of a problem, causing big moves when the crowd enters or exits at the same time. That is a concern for sure, but not a major one. Overcoming these kinds of problems resides in the small details of the strategies and will have little impact over the long run. 

There are other types of quantitative strategies that neither I nor anyone else trading them would write books about. These are usually very short-term strategies or strategies with low capacity that would suffer or cease to be profitable if more capital comes into the same game. Medium- to long-term trend following however has massive liquidity and is very scalable, so it is not subject to these concerns. 

Then there is another reason for me to write about these strategies. I am not a believer in the black-box approach in which you ask your clients for blind trust without giving any meaningful information about how you achieve your returns. Even if you know everything that this book aims to teach, it is still hard work to run a trend-following futures business and most people will not go out and start their own hedge fund simply because they now understand how the mechanics work. Some probably will and if you end up being one of them, please drop me an email to let me know how it all works out. Either way, I would like to think that I can add value with my own investment vehicles and that this book will not in any way hurt my business. 

## Acknowledgements

I had plenty of help in writing this book, both in terms of inspiration and support, and in reviewing and correcting my mistakes. I would especially like to thank the following people who provided invaluable feedback and advice: Thomas Hackl, Erk Subasi, PhD, Max Wong, Werner Trabesinger, PhD, Tony Ugrina, Raphael Rutz, Frederick Barnard and Nitin Gupta. 

1 

## Cross-Asset Trend Following with Futures

There is a group of hedge funds and professional asset managers who have shown a remarkable performance for over 30 years, consistently outperforming conventional strategies in both bull and bear markets, and during the 2008 credit crunch crisis showing truly spectacular returns. These traders are highly secretive about what they do and how they do it. They often employ large quant teams staffed with top-level PhDs from the best schools in the world, adding to the mystique surrounding their seemingly 

amazing long-term track records. Yet, as this book shows, it is possible to replicate their returns by using fairly simple systematic trading models, revealing that not only are they essentially doing the same thing, but also that it is not terribly complex and within the reach of most of us to replicate. 

This group of funds and traders goes by several names and they are often referred to as CTAs (for Commodity Trading Advisors), trend followers or managed futures traders. It matters little which term you prefer because there really are no standardised rules or definitions involved. What they all have in common is that their primary trading strategy is to capture lasting price moves in either direction in global markets across many asset classes, attempting to ride positions as long as possible when they start moving. In practice most futures managers do the same thing they have been doing since the 1970s: trend following. Conceptually the core idea is very simple. Use computer software to identify trends in a large set of different futures markets and attempt to enter into trends and follow them for as long as they last. By following a large number of markets covering all asset classes, both long and short, you can make money in both bull and bear markets and be sure to capture any lasting trend in the financial markets, regardless of asset class. 

This book shows all the details about what this group does in reality and how the members do it. 

The truth is that almost all of these funds are just following trends and there are not a whole lot of ways that this can be done. They all have their own proprietary tweaks, bells and whistles, but in the end the difference achieved by these is marginal in the grand scheme of things. This book sheds some light on what the large institutional trend-following futures traders do and how the results are created. The strategies as such are relatively simple and not terribly difficult to replicate in theory, but that in no way means that it is easy to replicate them in reality and to follow through. The difficulty of managed futures trading is largely misunderstood and those trying to replicate what we do usually spend too much time looking at the wrong things and not even realising the actual difficulties until it is too late. Strategies are easy. Sticking with them in reality is a whole different ball game. That may sound clichéd but come back to that statement after you finish reading this book and see if you still believe it is just a cliché. 

There are many names given to the strategies and the business that this book is about and, although they are often used interchangeably, in practice they can sometimes mean slightly different things and cause all kinds of confusion. The most commonly-used term by industry professionals is simply CTA (Commodity Trading Advisor) and though I admit that I tend to use this term myself it is in fact a misnomer in this case. CTA is a US regulatory term defined by the National Futures Association (NFA) and it has little to do with most so-called CTA funds or CTA managers today. This label is a legacy from the days when those running these types of strategies were US-based individuals or small companies regulated onshore by the NFA, which is not necessarily the case today. If you live in the UK and have your advisory company in London, set up an asset-management company in the British Virgin Islands and a hedge fund in the Caymans (which is in fact a more common setup than one would think) you are in no way affected by the NFA and therefore not a CTA from their point of view, even if you manage futures in large scale. 

## DIVERSIFIED TREND FOLLOWING IN A NUTSHELL

The very concept of trend following means that you will never buy at the bottom and you will never sell at the top. This is not about buying low and selling high, but rather about buying high and selling higher or shorting low and covering lower. These strategies will always arrive late at the party and overstay their welcome, but they always enjoy the fun in-between. All trend-following strategies are the same in concept and the underlying core idea is that the financial markets tend to move in trends, up, down or sideways, fo extended periods of time. Perhaps not all the time and perhaps not even most of the time, but the critical assumption is that there will always be periods where markets continue to move in the same direction for long enough periods of time to pay for the losing trades and have money left over. It is in these periods and only in these periods that trend-following strategies will make money. When the market is moving sideways, which is the case more often than one might think, these strategies are just not profitable. 

Figure 1.1 shows the type of trades we are looking for, which all boils down to waiting until the market has made a significant move in one direction, putting on a bet that the price will continue in the same direction and holding that position until the trend has seized. Note the two phases in the figure separated by a vertical line. Up until April there was no money to be made in following the trends of the NZ Dollar, simply because there were no trends around. Many trend followers would have attempted entries both on the long and short side and lost money, but the emerging trend from April onwards should have paid for it and then some. 


Figure 1.1 Phases of trend following


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/a18c272a4da2c1e0580425455f82a4027fadc851533378a38b1a7fcd2222c973.jpg)


If you look at a single market at any given time, there is a very high likelihood that no trend exists at the moment. That not only means that there are no profits for the trend-following strategies, but can also mean that loss after loss is realised as the strategy enters position after position only to see prices fall back into the old range. Trend-following trading on a single instrument is not terribly difficult but quite often a futile exercise, not to mention a very expensive one. Any single instrument or even asset class can have very long periods where this approach simply does not work and to keep losing over and over again, watching the portfolio value shrinking each time can be a horrible experience as well as financially disastrous. Those who trade only a single or a few markets also have a higher tendency of taking too large bets to make sure the bottom line of the portfolio will get a significant impact of each trade and that is also an excellent method of going bankrupt. 

With a diversified futures strategy you have a large basket of instruments to trade covering all major asset classes, making each single bet by itself almost insignificant to the overall performance. Most trendfollowing futures strategies do in fact lose on over half of all trades entered and sometimes as much as 70%, but the trick is to gain much more on the good ones than you lose on the bad and to do enough trades for the law of big numbers to start kicking in. 

For a truly diversified futures manager it really does not matter if we trade the S&P 500 Index, rough rice, bonds, gold or even live hogs. They are all just futures which can be treated in exactly the same way. Using historical data for long enough time periods we can analyse the behaviour of each market and have our strategy adapt to the volatility and characteristics of each market, making sure we build a robust and truly diversified portfolio. 

# THE TRADITIONAL INVESTMENT APPROACH

The most widely held asset class, in particular among the general public, is equities; that is, shares of corporations trading on stock exchanges. The academic community along with most large banks and financial institutions have long told the public that buying and holding equities over long periods of time is a safe and prudent method of investing and this has created a huge market for equity mutual funds. These funds are generally seen as responsible long-term investments that always go up in the long run, and there is a good chance that even a large part of your pension plan is invested in equity mutual funds for that very reason. The ubiquitous advice from banks is that you should hold a combination of equity mutual funds and bond mutual funds and that the younger you are, the larger the weight of the equity funds should be. The reason for the last part is that, although equities do tend to go up in the long run, they are more volatile than bonds and you should take higher financial risks when you are younger since you have time to make your losses back. Furthermore, the advice is generally that you should prefer equity mutual funds over buying single stocks to make sure that you get sufficient diversification and you participate in the overal market instead of taking bets on individual companies which may run into unexpected trouble down the road. 

This all sounds very reasonable and makes for a good sales pitch, at least if the core assumption of equities always appreciating over time holds up in reality. The idea of diversifying by holding many stocks instead of just a few companies also sounds very reasonable, given that the assumption holds up that the correlation between stocks is low enough to provide the desired diversification benefits of lower risk at equal or higher returns. Of course, if either of these assumptions turn out to be disappointing in reality, the whole strategy risks falling like a proverbial house of cards. 

In reality, equities as an asset class has a very high internal correlation compared to most other types of instruments. The prices of stocks tend to move together up and down on the same days and while there are large differences in overall returns between a good stock and a bad one, over longer time horizons the timing of their positive and negative days are often highly related even in normal markets. If you hold a large basket of stocks in many different countries and sectors, you still just hold stocks and the extent of your diversification is very much limited. The larger problem with the diversification starts creeping up in times of market distress or when there is a single fundamental theme that drives the market as a whole. This could be a longer-term event such as a dot com bubble and crash, a banking sector meltdown and so on, or it can be a shorter-term shock event like an earthquake or a surprise breakout of war. When the market gets single-minded, the correlations between stocks quickly approach one as everyone panic sells at the same time and then re-buys on the same euphoria when the problems are perceived to be lessened. In these markets it matters little what stocks you hold and the diversification of your portfolio will turn out to be a very expensive illusion. 

Then again, if stocks always go up in the long run the correlations should be of lesser importance since you would always make the money back again if you just sit on the stocks and wait a little bit longer. This is absolutely true and if you are a very patient person you are very likely to make money from the stock markets by just buying and holding. From 1976 to 2011 the MSCI World Index rose by 1,300%, so in 35 years you would have made over ten times your initial investment. Of course, if you translate that into annual compound return you will see that this means a yield of just around 8% per year. If you had been so unlucky as to invest in 1999 instead, you would still hold a loss 13 years later of over 20%. Had you invested in 2007 your loss would be even greater. Although equities do tend to move up in the long run, most of us cannot afford to lose a large part of our capital and wait for a half a lifetime to get our money back. If you are lucky and invest in a good year or even a good decade, the buy-and-hold strategy may work out but it can also turn out to be a really bumpy ride for quite a low return in the end. Going back to the 1,000% or so made on an investment from 1976 to 2011, the largest drawdown during this period was 55%. Looking at the buy-and-hold strategy from a long-term return to risk perspective, that means that in order to get your 8% or so return per year, you must accept a risk of losing more than half of your capital, which would translate to close to seven years of average return. 

You may say that the 55% loss represents only one extreme event, the 2008 credit meltdown, and that such scenarios are unlikely to repeat, but this is not at all the case. Let’s just look at the fairly recent history of these so-called once-in-a-lifetime events. In 1974 the Dow Jones Industrial average hit a drawdown of 40%, which took over six years to recover. In 1978 the same index fell 27% in a little over a year. The same thing happened again in 1982 when the losses amounted to 25% in about a year. From the peak in August 1987 to the bottom in October the index lost over 40%. Despite the bull market of the 1990s, there were several 15–20% loss periods and when the markets turned down in 2000 the index had lost about 40% before hitting the bottom. What you need to ask yourself is just how high an expected compound return you need to compensate for the high risks of the stock markets, and whether you are happy with single digit returns for that level of volatility. 

If you do choose to participate in the stock markets through an equity mutual fund you have one more factor to consider, and that is whether or not the mutual fund can match or beat the index it is supposed to be tracking. A mutual-fund manager, as opposed to a hedge-fund manager, is tasked with trying to beat a specific index and in the case of an equity fund that index would be something like the S&P 500, FTSE 100, MSCI World or similar. It can be a broad country index, international index, sector index or any other kind of equity index, but the task is to follow the designated index and attempt to beat it. Most mutual-fund managers have very little leeway in their investment approach and they are not allowed to deviate much from their index. Methods to attempt to beat the index could involve slight over- or under-weights in stocks that the manager believes will perform better or worse than the index, or to hold a little more cash during perceived bad markets. The really big difference between a mutual-fund manager and a hedge-fund manager or absolute-return trader is that the mutual-fund manager’s job is to follow the index, whether it goes up or down. That person’s job is not to make money for the client but rather to attempt to make sure that the client gets the return of the index and it is hoped slightly more. If the S&P 500 index declines by 30% in a year, and a mutual fund using that index as a benchmark loses only 25% of the clients’ money, that is a big achievement and the fund manager has done a very good job. 

There are of course fees to be paid, including a management fee and sometimes a performance fee for the fund as well as administration fees, custody fees, commissions and so on, which is the reason why very few mutual funds manage to beat their index or even match it. According to Standard & Poor’s Indices Versus Active Funds Scorecard (SPIVA) 2011 report, the percentage of US domestic equity funds that outperformed the benchmark in 2011 was less than 16%. Worst that year were the large-cap growth funds where over 95% failed to beat their benchmark. Looking over a period of five years, from 2006 to 2011, 62% of all US domestic funds failed to beat their benchmarks. Worst in that five-year period was the midcap growth funds where less than 10% reached their targets. The picture that the S&P reports paint is devastating for the mutual-fund business. If active mutual funds have consistently proved to underperform their benchmarks year after year, there is little reason to think that this is about to change any time soon. 

There are times when it’s a good idea to participate in the general equity markets by buying and holding for extended periods of time, but then you need to have a strategy for when to get out of the markets when the big declines come along, because they will come along. It makes sense to have a portion of your money in equities one way or another as long as you step out of that market during the extremely volatile and troublesome years, but I’m personally not entirely convinced about the wisdom of putting the bulk of your hard-earned cash into this asset class and just holding onto it in up and down markets, hoping for the best. For participating in these markets, you may also want to consider investing in passive exchangetraded funds (ETFs) as an alternative to classic mutual funds, because the index-tracking ETFs hold the exact stocks of the index at all times and have substantially lower fees, making them track and match the index with a very high degree of precision. They are also very easy and cheap to buy and sell as they are directly traded on an exchange with up-to-the-second pricing. 

# THE CASE FOR DIVERSIFIED MANAGED FUTURES

There are many viable investment strategies that tend to outperform buy-and-hold equities on a volatility adjusted basis and I employ several of them. One of the top strategies is trend-following managed futures for its consistent long-term track record of providing a very good return-to-risk ratio during both bull and bear years. A solid managed futures strategy has a reasonably high expected yearly return, acceptable drawdown in relation to the yearly return and lack of significant correlation to world equity markets, and preferably slightly negative correlation. 

The list of successful traders and hedge funds operating in the trend-following managed futures markets is quite long and many of them have been around for decades, some even from the 1970s. The very fact that so many trend traders have managed not only to stay in business for this long period, but to also make consistently impressive returns, should in itself prove that these strategies work. 

Table 1.1 shows a brief comparison between the performances of some futures managers to that of the world equity markets. As mentioned, MSCI World has shown a long-term yield of 8% with a maximum drawdown (DD) of 55%, which would mean that over seven normal years of performance were given up in that decline. This could be compared with funds like Millburn, which over the same period had a return of 17% and only gave up 26% at the most, or the equivalent of one and a half years only. Transtrend gave up even less of its return and even Dunn, which after a stellar track record suffered a setback a few years ago, only lost four years of performance and still holds a much higher compound rate of return than the equity index. 


Table 1.1 Performance comparison


<table><tr><td></td><td>Ann. compound return (%)</td><td>Max DD (%)</td><td>Correlation to MSCI World</td><td>Starting date</td></tr><tr><td>MSCI World Total Return</td><td>8.0</td><td>-55.0</td><td></td><td>Feb-77</td></tr><tr><td>Millburn Multi Markets</td><td>16.6</td><td>-25.6</td><td>-0.01</td><td>Feb-77</td></tr><tr><td>Dunn World Monetary and Agriculture</td><td>14.4</td><td>-60.3</td><td>-0.03</td><td>Nov-84</td></tr><tr><td>Hyman Beck Global Portfolio</td><td>11.1</td><td>-29.3</td><td>-0.10</td><td>Apr-91</td></tr><tr><td>SuperFund Green Q AG</td><td>12.1</td><td>-32.8</td><td>-0.05</td><td>Mar-96</td></tr><tr><td>Mulvaney Global Markets Fund</td><td>15.4</td><td>-41.3</td><td>-0.16</td><td>May-99</td></tr><tr><td>Transtrend Standard Risk</td><td>9.8</td><td>-10.9</td><td>-0.05</td><td>Jun-92</td></tr><tr><td>Sunrise Expanded Diversified</td><td>11.9</td><td>-19.9</td><td>-0.13</td><td>Jan-96</td></tr><tr><td>Winton Futures Fund B</td><td>16.2</td><td>-25.6</td><td>0.00</td><td>Oct-97</td></tr><tr><td>Rabar Market Research Diversified Program</td><td>12.9</td><td>-29.8</td><td>0.01</td><td>Jan-89</td></tr><tr><td>Clarke Capital Management Worldwide</td><td>13.8</td><td>-26.6</td><td>-0.11</td><td>Jan-96</td></tr><tr><td>Chesapeake Capital Diversified</td><td>12.8</td><td>-27.8</td><td>0.15</td><td>Feb-88</td></tr><tr><td>Abraham Trading Company Diversified Program</td><td>18.7</td><td>-32.0</td><td>-0.08</td><td>Jan-88</td></tr><tr><td>Estlander &amp; Partners, Alpha Trend</td><td>12.1</td><td>-16.5</td><td>0.08</td><td>Oct-91</td></tr></table>

Looking at the funds’ correlation to MSCI World you should notice that none of them have any significant correlation at all. This means that with such a strategy, you really don’t have to worry about whether the world equity markets are going up or down since it makes little difference to your returns. It does not mean that all years are positive for diversified futures strategies, only that the timing of the positive and negative returns is, over time, unrelated to those of the equity market. The observant reader might be asking if that does not make these strategies a very good complement to an equity portfolio, and the answer is that it absolutely does, but we are getting ahead of ourselves here. 

## CRITICISM OF TREND-FOLLOWING STRATEGIES

Although certain criticisms of trend-following trading have some validity, there are other commonly recurring arguments that may be a little less thought through. One somewhat valid criticism is that there is a survival bias in the numbers reported by the industry. The argument is that the funds that are part of the relevant indices and comparisons are only there because they did well and the funds that did not do well are either out of business or too small to be part of the indices, and that this effect makes the indices have a positive bias. This is of course a factor, much the same way as a stock can be knocked out of the S&P 500 Index after it had bad performance and its market capitalisation shrunk. Survival bias is a fact of life with all indices and it makes them all look a little better than reality would dictate. This is not an asset class specific problem. Anyhow, the arguments made in this book regarding the performance of diversified futures strategies are not dependent on the performance of indices; the comparisons asset managers included consist of a broad range of big players, some of which had some really difficult periods in their track records. There are some excellent aspects of these strategies and there are some serious pitfalls and potential problems that you need to be aware of. I deal with all of these in this book and have no intention of painting a rosier picture of the real situation than my experience reflects. Doing so would be both counterproductive and also, quite frankly, unnecessary. 

Another common argument is that the high leverage makes the strategy too risky. This is mostly based on a lack of understanding of the two concepts of leverage and risk, which are not necessarily related. Defining leverage is a tricky thing when you deal with cross-asset futures strategies and simply adding up notional contract values and dividing with the capital base simply does not cut it. As I demonstrate and explain further on, having a million pounds’ worth of exposure to gold and having a million pounds’ worth of exposure to the Euribor is a world apart in terms of actual risk. While gold often moves several per cent in a day, a normal move in the Euribor would be a couple of basis points. Sure, these futures strategies may have quite high notional contract exposures but don’t go confusing that with risk. To be sure, these strategies can be risky, but buying and holding a portfolio of stocks is not necessarily less risky. 

Most trend-following futures strategies will need to sell short quite often, and often as much as you buy long. Critics would highlight that when you are short you have an unlimited potential risk, which again is a misunderstanding of how markets work. Just as with equities, you risk losing what you put on the table but not more than that. While the pay-out diagram for a futures contract in theory has an unlimited loss, unless you have an unlimited amount of margin capital in your account this is simply not the case in reality. In my experience, it is harder to trade on the short side than the long side, but that does not necessarily make it riskier, in particular when done in the context of a large diversified portfolio. Rather, on the contrary, the ability to go short tends to provide a higher skew of the return distributions and thereby increase the attractiveness as a hedging strategy. 

Managed futures funds sometimes have large and long-lasting drawdowns. This is an absolutely valid criticism and something you need to be very aware of before setting out on this path. People like to hear percentage numbers, such as a common drawdown is 20% for example, but this is not really helpful since you can tweak the risk factor up and down as you please by adjusting position sizes, as I explain in detail in later chapters. The question should rather be whether the long-term return numbers compensate for the worst drawdown scenarios and in this case it is hard to argue with the numbers. Drawdowns are painful when they occur but to say that they are worse than for the classic buy-and-hold equity alternative would be untrue. At the bottom of the equity bear market of 2008, based on MSCI World, you would have lost 55% from the peak and gone back to the levels of the mid-1990s. Losing almost 15 years of accumulated gains is practically unheard of for diversified futures strategies, yet the buy-and-hold strategy is considered by many the safer alternative. 

Of course, just because a strategy worked for the past 30 to 40 years does not necessarily mean it has to work in the next decade or two. We are not dealing with mathematical certainties here and we are not trying to predict the future. What we are doing is try to tilt the probabilities slightly in our favour and then repeat the same thing over and over a large number of times. There will be years that are very bad for trend followers and there will be very good years. Over time the strategy is highly likely to produce strong absolute returns and to outperform traditional investment methods, but we are dealing in probabilities and not in certainties. There are no guarantees in this business, regardless of what strategy you choose. I don’t expect any major problems that would end the profitable reign of trend-following futures trading, but it would be arrogant not to admit that the dinosaurs probably did not expect a huge stone to fall from the sky and end their party either. Neither event is very likely but both are quite possible. 

## MANAGED FUTURES AS A BUSINESS

This book primarily deals with how to trade trend-following futures strategies as a money manager, trading other people’s money, and it would be fair to wonder why one would want to share the profits with others. Some would take the view that once you have a good strategy with dependable long-term results, you should keep it to yourself and only trade your own money. There are instances where this may be true, in particular with strategies that are not scalable and have to be traded in low volume. For a truly scalable strategy, however, there is no real downside to sharing the spoils and quite a bit to be gained. 

For starters, you need a large capital base to trade trend-following futures with sufficient diversification and reasonably low volatility, and even if you master the trading side you may not have the couple of million pounds required to achieve a high level of diversification with acceptable risk. Pooling your money with that of other people would then make perfect sense. Given that you can charge other people for managing their money along with your own makes the prospect even more appealing, because it gives you an income while you do the same work you might have done yourself anyhow, and apart from your own gains you participate in your clients’ trading gains as well. 

If you go the hedge-fund route and accept external money to be pooled with your own and traded like a single account, the overall workload increase is quite minor on a daily basis but your earning potential dramatically goes up. If you choose to manage individual accounts you may get a little higher workload on the admin side but a quicker and cheaper start-up phase and the economic upside is essentially the same. For starters you will have a reasonably stable income from the management fee which allows you to focus on long-term results. This strategy requires patience and if you feel economic pressure to achieve profitable trading each month, this will not work out. There can be long periods of sideways or negative trading and you need to be able to stick it out in those periods. Your incentive should always be towards long-term strong positive returns while keeping drawdowns at acceptable levels. As you get a percentage of the profits created on behalf of external investors, the earning potential in good years vastly exceeds what you could achieve with your own money alone. 

If you have US$100,000 and make a 20% return one year you just made US$20,000, which is great for sure. But if you also have US$1 million of external investor money in the pot and charge a management fee of 1.5% and a performance fee of 15%, you just made another US$30,000 in performance fee as well as over US$15,000 in management fee. By doing the same trades on a larger portfolio you make 

US$65,000 instead of US$20,000, and the beauty of managed futures trend following is that it is very scalable and you can keep piling up very large sums of external money and still trade basically the same way with very little additional work. 

Managing external money means that you have a fiduciary responsibility not only to stick strictly to the strategy you have been given the mandate to trade, but also to create relevant reports and analyses and keep proper paperwork. This may seem like a chore but the added required diligence should be a good thing and ensure that you act in a professional manner at all times. 

The negative part with managing other people’s money is that you have a little less freedom, because you need to stick to the plans and principles that you have sold to your investors. You likely need to take lower risk than you would have done with your own account as well. Some traders who just manage their own money may be fine with the prospect of losing 60–70% of the capital base in return for potential tripledigit annual returns, but this is a very tough sell for a professional money manager. Investors, and in particular institutional investors with deep pockets, tend to prefer lower returns with lower risks. 

The business of managing futures can be a highly profitable one if done carefully and with proper planning. There are a large number of famous traders who have achieved remarkable results in this field since the 1970s and the number of public funds in this space keeps increasing. 

From a business point of view the deal is quite straightforward compared to most other types of enterprises. A little simplified, it could be described in these steps: 

1. Find clients to invest money with you. 

2. Trade futures on their behalf. 

3. Charge clients a yearly fixed fee for managing their money, usually 1–2%. 

4. Charge clients a yearly performance fee if you make money for them, usually 10–20% of the profits. 

The nicest part of this business model is that it is no more difficult to manage US$20 million than to manage US$10 million; your cost base would be more or less the same but your revenues would double. This business model is very scalable and until you reach a very large asset base you can use the same strategies in the same manner and just adjust your position sizes. Once you reach US$500 million to US$1 billion, you will for sure get a whole new set of problems when it comes to asset allocation and liquidity, but that is rather a pleasant problem to have. 

When first starting out most of us discover that the biggest problem we have is finding clients to invest in a brand new manager with a brand new product. Unless your rich uncle Bob just retired and has got a few millions he does not mind investing with you, it may be an uphill battle to get that first seed money to get started. Before you start approaching potential clients you need to have a solid product to sell them, that is, your investment strategy along with your abilities to execute it, and be able to show them that you know what you are talking about. Designing an investment strategy is where this book comes in and I hope you will have a good platform to build upon once you reach the end. 

There are two main paths for building a futures-trading business, as opposed to just trading your own money: 

Managed accounts: This is the traditional approach, where clients have accounts in their own names and give a power of attorney to the trader to be able to execute trades directly on their behalves. This is quite a simple approach in terms of setup and legal structures and it provides the client with a high level of flexibility and security. Each account is different, and so the client may have special wishes in terms of risk and such which the trader is usually able to accommodate. If this is not a desired feature and you wish to simplify trading, you can also get onto a managedaccounts platform for a bank or prime broker where you essentially trade one account and have 

trades automatically pro rata split on the individual client accounts. Since the money is in the client’s own account, the individual has the added flexibility of being able to view the account status at any time or to pull the plug on the trading without any notices or otherwise intervene. The client does not need to worry about dealing with a possible new Madoff, because there are no middle men and the bank reports the account status directly to the client. For the money manager, the managed-account solution can mean a little more administrative work at times than if a hedgefund type structure is employed. 

Hedge fund: With this approach, there is one big account for all clients. Well, in practice there may be several accounts at several banks, but the point is that all money from all clients is pooled together in one pile and traded together. This greatly simplifies the business side when it comes to handling client reporting and paperwork, but it requires a more complex legal structure, sometimes with a combination of onshore and offshore companies. 

Regardless of which of these two main paths you decide to take, you need to do some proper homework on the pros and cons of either solution. More and more professional investors have a preference for managed accounts because they reduce legal risks, but for most managed-account setups you need larger amounts from each client than you would need for a hedge-fund setup. The situation also varies a lot depending on where you and your potential clients are domiciled. Look into the applicable legal situation and be sure to check what, if any, regulations apply. You may need licences from the local regulators and breaching such requirements could quickly end your trading reign. 

## DIFFERENCES BETWEEN RUNNING A TRADING BUSINESS AND PERSONAL TRADING

The most important difference in managing a private account and a hedge fund or other professional asset management is the importance of volatility. If your volatility is too high your investors are not likely to stay with you. A temporary drawdown of 50% for a small private account might be acceptable, depending on your risk appetite and expected rate of return, but it is not an easy sell to an external investor. 

## Marketability of your strategy

When you trade your own account, and sometimes even manage accounts for trusted people, you can trade on pretty much anything you think makes sense without having to convince anyone of how good your ideas are. If you are truly a very strong trader and you have a stellar track record, you may be able to do the same thing for a hedge fund or professional managed accounts, but the days of the black box funds are mostly in the past. Simply telling prospective clients to just trust you and only hinting at how your strategies work no longer makes for a good sales pitch. If you are dependent on raising assets for your new fund, as most of us are, you need a good story to be able to paint a clear picture of what your fund does and why it can make a big difference. This does not mean that you need to disclose all your mathematics and hand over source code for your programs, but the principal idea of what your strategy is about, what kind of market phenomenon you are trying to exploit and how you intend to do so, needs to be clear and explainable. You also need to be able to explain how your risk and return profile will look, what kind of return you are targeting and at what kind of volatility level. Even if you have a good story for these aspects, you still need to be able to explain why your product is unique and why the prospective client should not just go and buy another similar fund or hand money to a different futures manager with a successful track record of many years. 

You need to work on presentation and marketing. If you have solid simulations for your strategies, use the charts and data in your material. Make professional-looking fact sheets that describe your philosophy and strategy, showing exactly why your product is so well positioned for this particular market and why your strategy is stronger than the established competitors. 

Don’t underestimate the difficulty and the amount of work needed to raise the initial seed money for your business. This can be a colossal task that can make or break your whole project. It often comes down to connections and friends in the market who can help you by putting up some initial cash and if you lack such connections you may find yourself having tough time. Even if you have a great strategy, a proven track record with individual accounts and a strong personal reputation in the markets, you are still very vulnerable in this phase and you may be forced to make deals against better judgment, such as paying a yearly fee for referred funds, in order to secure enough seed capital to make a fund launch possible. 

## Volatility profile

Volatility is the currency used to buy performance. If customers don’t get what they pay for, they will leave very quickly. There simply is no loyalty in this business and that is probably a good thing in a strictly Darwinian sense. An old adage states that there is no such thing as a third bad year for a hedge fund; after the second bad year all the investors are gone and the fund is out of business. 

In your strategy simulations as well as in your live trading, you need to pay attention not only to the overall return numbers but also to the drawdowns and volatility. Try to simulate realistically what your maximum drawdown would have been trading with the same strategy for the past 30 years, and then assume that something much worse will happen after your fund or trading product is launched. Drawdown is defined as your current loss from the highest historical reading of the fund or strategy. If you gain 20% in the first three months of the year, and then back down to +10% on the year in the next three months, you are in an 8.3% drawdown despite being up 10% year to date. 

You need to be aware what magnitudes of drawdowns are normal for your strategy and how long it normally takes to recover, and of course what the longest recovery time was in the simulations. Even if your drawdown was not big, it is hard to retain clients if it takes years to reach a new peak. Remember that investors may come in at any time during the year, normally at the start of any month. Even if the investor who bought in at a lower price might be okay with a bit of a drawdown, the one who bought at the top may be a little grumpier. 

Managed-accounts clients are generally stickier, as the industry term goes, than hedge-fund clients. This refers to the notion that the managed-account clients tend to stay longer with a manager and it takes more for them to close the relationship than for a hedge-fund client. This is largely due to the fact that the manager has much more personal interaction with a managed-account client than with a hedge-fund client, who is often completely anonymous to the manager. On the flipside, it is generally more difficult to find managed-accounts clients in the first place and they require more admin and relationship management. 

A common concept in measuring risk-to-return profile is the Sharpe ratio. This ratio measures return above risk-free interest rate, divided by the standard deviation of the returns. For systematic strategies, anything above 0.5 is normally considered acceptable, and the higher the better of course. A fair case can be made against the use of Sharpe ratio for these kinds of strategies, however, because it penalises both upside and downside volatility where only one of them is negative to an investor. The Sharpe ratio is very well known, easily explainable to clients and comparable across funds and so it does have some merits, but a good complement to use is the Sortino ratio. This is a very similar concept but punishes volatility only on the downside, or below a required rate of return. 

When analysing your strategies potential drawdowns and recovery times, you also need to consider the crasser factor of your own profitability. Although you should target to be able to at least break even on the management fee alone, all hedge-fund and futures account managers are, sometimes painfully, aware of the fact that the real money comes from performance fees. If you are in a drawdown for two years, you 

don’t get paid any performance fees for two years and that could mean a very large difference in your own bottom line. After all, you are still running a business. 

## Subscriptions and redemptions

Client money inflow and outflow can create a headache for many money managers. You need to have a clear plan for how to handle this aspect and what to do when money comes in or goes out. This is a larger problem that it might sound and can have a significant effect on the return. When you get money coming in, do you simply add to all positions at the same ratio, increase selectively, open new positions for that money or leave it in cash? If you are still a fairly small fund and have a large diversified portfolio of futures, you might find yourself having three to four contracts of some futures and if you get subscriptions increasing your assets under management by 15% you just cannot increase your positions proportionally. The same naturally goes for an equivalent redemption. 

If you get 15% new money coming in and you decide it’s too little to increase position sizes, you effectively dilute the returns for everyone who has already invested. The correct thing to do is to adjust every single position pro rata according to the subscriptions and redemptions coming in, but for a smaller portfolio you will need manual intervention. If you only hold a few contracts of some assets, that is likely to mean that you already have a rounding error in your position size and you could use the subscriptions and redemptions to attempt to balance these rounding errors out. If you have new subscriptions, you could selectively increase the positions where you are slightly underweight due to previous rounding errors and vice versa. Unless you have a large enough capital base, some discretionary decisions will be needed in these cases. 

One nice thing about futures strategies compared to other more cash-instrument-based strategies such as equity funds is that you will always have enough cash on the accounts to pay for normal redemptions. You probably don’t need to liquidate anything to meet the payments for clients who want to exit or decrease their stake, as long as the amounts are not too large a part of the total capital base. 

## Psychological difference

When you review your simulation data and look at a 15% drawdown, it might not sound so bad but the first time you lose a million pounds, things will feel quite different. The added stress of watching the net asset value of your fund ticking in front of you in real-time will further assault your mental health. It takes a tremendous amount of discipline to sit tight and follow a predetermined path of action when a bad day comes along and you see a wildly ticking red number in front of you, losing tens of thousands by the second. Making rash decisions in this situation is rarely a good idea and you need to have a plan in advance for how to react to any given situation. If your simulation tells you that 5% down days are possible but far out on the tail, you cannot pull the plug on the strategy and step to the side if it suddenly occurs in front of your eyes, no matter how painful it might be. 

This type of advice is easy to give but very hard to follow. It is obvious common sense but most people need to go through some really tough market periods and probably several times before this starts becoming less difficult. The temptation to override your strategy when it does badly will always be there and you need to have a rule in advance about whether you are allowed to override, and if so under what conditions and in what manner. Never make the decision on the stressful bad day, just follow your predetermined plan. 

To attempt to maintain your sanity, it might help to try to distance yourself from the monetary numbers. Try not to view the fund’s assets as real money but merely a way of keeping score in the game, like Monopoly money. If you start thinking about what the million you just lost could have bought in the real world, you lose your perspective and risk further losses or missing out on the rebound. Even worse, never calculate what the recent loss means in terms of your own management fee or performance fee and what you would have done with that money. After all, it’s just Monopoly money. 

An unwritten rule says that hedge-fund managers should have a large part of their net worth in their own fund. There are, however, two sides of that coin. The common argument is that having your own money in the fund ensures that your financial interests are aligned with your investors, so that if they lose you lose as well and vice versa. This is of course true, but on the other hand as manager you make most of your money on the performance fee of the fund and so the interest should already be aligned. There is then the added psychological stress of having your own money in the fund. It is certainly a lot harder to look at the fund as Monopoly money if you have a large part of your own money in it. Many investors will see that as a good thing, forgetting that if managers can distance themselves from the asset values and take a more rational perspective on the strategy, the performance might in fact be better. Emotions and investment decisions make a very bad mix. 

2 

## Futures Data and Tools

## FUTURES AS AN ASSET CLASS

Futures is really a type of instrument and not a type of asset. I still call it an asset class for the simple reason that you can treat it like one. The most interesting feature of these instruments is that they are standardised and exchange listed, so you can trade practically all asset classes in a single coherent manner without caring about what the actual underlying asset is, and therefore you can view futures itself as a single asset class. Futures can offer many advantages for the systematic trader and of course some unique challenges as well. With futures strategies you can cover everything from equities to bonds, metals, grains and even meats, with standardised instruments following the same basic characteristics. If you are looking to build portfolio strategies that make full use of diversification effects, this is a dream. You need not worry about whether the underlying is the S&P 500 Index, gold, corn or livestock; they can all be treated the same way. They are of course likely to have very different volatility profiles and that is something you need to address in your core strategy. 

From a technical point of view, a futures contract is an obligation to conduct a transaction at a specific future date. The buyer of the contract is obligated to buy the underlying asset at the end of the contract life and the seller is obligated to sell the same underlying asset at the same time and the same price. The original idea behind futures was for hedging purposes, where a corn farmer who knows that he will have ten tons of corn to sell in two months wants to lock in the price to avoid the risk of adverse price changes until his crop is ready to be sold. You could also imagine a US company expecting to receive 10 million euros in revenue six months from now who wants to avoid taking currency risk and uses futures to secure the price in advance. The key thing with futures is that they are standardised and exchange traded. This means that all detailed specifications about deliveries and so on are detailed in advance and thereby the obligation can be transferred, that is, an offsetting position can be taken to get out of the obligation. If you buy gold futures, that does not mean you have to take delivery of the bars later on, you just need to sell gold futures in the same delivery month on the same exchange before the contract goes to delivery. In reality an overwhelming majority of all futures trading is done by speculators who have no actual interest in the underlying asset itself. These contracts never go to delivery because the speculators make an offsetting trade before the end of the contract’s life. 

So for the purposes of a speculator, and in that group I include you dear reader, you can view futures contracts in a simpler way. If you believe the price of an asset is likely to go up, you buy the futures contract. If you believe it will go down, you sell the contract short. When you buy stocks you generally have to pay up the whole amount right away, or at least three days after the purchase, but not so for futures. All you need to put up is the initial margin specified by the exchange and this is usually just a fraction of the total underlying amount. This means of course that you can trade on margin and achieve a high leverage, if you so please. Doing that could mean large risks if you are not careful, but if you use that leverage to achieve proper diversification it does not necessarily equal higher risks. 

Futures exchanges use so-called mark-to-market accounting that requires that the gains and losses for each day be settled at the end of that day. Gains or losses on the contracts are not allowed to be accumulated from day to day, but are settled in cash at the end of each trading day on your cash accounts. If you are long ten gold contracts and yesterday’s closing price of gold was US$1,650 and today it ended at US$1,652 you have a day gain of US$2 per ounce. Since each contract represents 100 ounces, you have a total gain of US$2,000 and this amount will then be credited to your account by the day’s end, even if your position remains open. 

The notional amount, or face value exposure, on that same position is easily calculated. Multiply the contract price of US$1,652 by the contract size of 100 and by the ten contracts you hold and you arrive at US$1,652,000. This by no means implies that you need to have that amount of money on your account; all you need is a fraction of this, called the margin. The initial margin requirement varies greatly between different markets and as a general rule, the less volatile the instrument, the less the margin requirement is. Typically the initial margin requirement is around 10%, but it can go both higher and lower for some assets and normally varies 5–15%. The margin requirement for each asset is subject to exchange regulation and may change at any time. Be sure you are up to date with the margin requirements of instruments you trade and make sure you have sufficient capital in your accounts. 

If your account drops in value and no longer amounts to the required margin, you will need to add money to bring the account up to the required level or be forced to unwind positions. This is referred to as the maintenance margin. 

Suppose that you want to buy five contracts of sugar and the price at the moment is 24.82 US cents. Each contract is for 112,000 lbs., making for a notional amount of a little less than US$28,000 per contract and about US$140,000 for the five contracts. Further suppose that the initial margin requirement at the time is US$2,030 per contract and a maintenance margin of US$1,450. So instead of requiring US$140,000 on your account, all you need is US$10,150, or about 7.3% of the notional amount, but you need to make sure you don’t go below the maintenance requirement of US$7,250. If your account drops below that, you have the choice of shutting your position down or adding enough money to bring it back up to the initial requirement of US$10,150. 

A critical difference between cash instruments such as stocks and derivatives such as futures is the limited lifetime of the latter. Each futures contract has an expiry date when it ceases to exist, which means that you have the added practical hassle of keeping track of when you need to roll your position from one month to another. 

As far as derivatives go though, futures are quite simple instruments. There are a few basic properties of each contract you need to be aware of and the most important ones are listed in Table 2.1, with the delivery codes in Table 2.2. 

Table 2.1 Some properties of futures 

<table><tr><td>Property</td><td>Description</td></tr><tr><td>Ticker</td><td>The base code of the futures contract: for example, GC for Comex Gold. This is unfortunately not standardised and different data vendors can use different tickers for the same contract. If you use multiple market data vendors, it may be worth building your own lookup table to be able to translate easily between the different code schemes.</td></tr><tr><td>Month</td><td>The delivery month is expressed as a single letter, and here thankfully the nomenclature is the same for all vendors. As Table 2.2 confirms, January to December are designated, in order, by the letters F, G, H, J, K, M, N, Q, U, V, X and Z.</td></tr><tr><td>Year</td><td>A single digit denotes delivery year and the assumption is of course that it is the next possible matching year, if not current.</td></tr><tr><td>Code</td><td>The full code is the combination of the three properties above. So Comex Gold with delivery month June 2012 would usually be designated GCM2.</td></tr><tr><td>Expiry</td><td>The exact date when the contract expires to either financial settlement or actual delivery. For a trader, this date is only relevant for financial futures, not for commodities or anything that is actually deliverable. For deliverable contracts you need to be out much earlier.</td></tr><tr><td>Last trading day</td><td>This is the date you need to pay attention to. The rules are different for different markets and they may use slightly different terminology for this date (first notice day and so on), but all futures contracts have a predetermined last day of trading for speculators. For physically deliverable contracts, you risk being forced to take or make delivery if you hold beyond this point. In practice this is not likely to happen though, as most brokers will not allow you to enter delivery and they will shut down your position forcefully on this day unless you do first. You don’t want that to happen though, so you better make sure that you shut down or roll your position in time.</td></tr><tr><td>Contract size</td><td>This tells you what one contract represents in real world terms. As an example, the Nymex Light Crude Oil represents 1,000 barrels worth, while the Swiss franc (CHF) currency future on the ICE represents 125,000 CHF.</td></tr><tr><td>Point value</td><td>For most futures contracts, the contract size and the point value is exactly the same. When you deal with cross-asset futures though, you will run into some exceptions to this rule and that necessitates a standard way to calculate your profit and loss, risk and so on. You need a way of knowing exactly how much the profit or loss would be if the futures contract moves one full point. For bond futures the answer is usually the contract size divided by 100. With money-market futures you need to both divide by 100 and adjust for the duration. So the 3-month Eurodollar future with a contract size of one million ends up with a point value of 2,500 (1,000,000/100/4). Make sure you have a proper lookup table for point value for all contracts you want to trade. Some data vendors tend to confuse this by mixing up tick value and point value, but I stick to the definition of profit variation per full point move, not single tick move.</td></tr><tr><td>Currency</td><td>For the point value to make sense you need to know what currency the future is traded in and then translate it to your portfolio base currency.</td></tr><tr><td>Initial margin</td><td>The initial margin is determined by the exchange and tells you exactly how much cash you need to put up as collateral for each contract of a certain future. If the position goes against you, however, you need to put up more margin and so you had better not sail too close to the wind here. Your broker will shut down your position if you fail to maintain enough collateral in your account.</td></tr><tr><td>Maintenance margin</td><td>The amount of money needed on your account to hold on to a contract. If your account drops below this amount you are required to either close the position or replenish funds in your account.</td></tr><tr><td>Open interest</td><td>Most financial instruments share the historical data fields open, high, low, close and volume, but the open interest is unique to derivatives. This tells you how many open contracts are currently held by market participants. Futures being a zero sum game, someone is always short what someone else is long, but each contract is counted only once.</td></tr><tr><td>Sector (asset class)</td><td>Although there are many ways of dividing futures into sectors, I use a broad scheme in this book which makes a lot of sense for our needs. I divide the futures markets into currencies, equities, rates, agricultural commodities and non-agricultural commodities.</td></tr></table>


Table 2.2 Futures delivery codes


<table><tr><td>Month</td><td>Code</td></tr><tr><td>January</td><td>F</td></tr><tr><td>February</td><td>G</td></tr><tr><td>March</td><td>H</td></tr><tr><td>April</td><td>J</td></tr><tr><td>May</td><td>K</td></tr><tr><td>June</td><td>M</td></tr><tr><td>July</td><td>N</td></tr><tr><td>August</td><td>Q</td></tr><tr><td>September</td><td>U</td></tr><tr><td>October</td><td>V</td></tr><tr><td>November</td><td>X</td></tr><tr><td>December</td><td>Z</td></tr></table>

## Futures exchanges

There are quite a few futures exchanges around the world although a few large exchanges in the US are the most important for the typical diversified futures manager. Most exchanges have excellent web pages with tons of useful information about the products they offer and they are worth having a read through. The exchanges that I list in Table 2.3 are the ones I primarily use for the futures markets in this book. 


Table 2.3 Futures exchanges


<table><tr><td>Short</td><td>Name</td><td>Website</td><td>Comments</td></tr><tr><td>ASX</td><td>Australian Securities Exchange</td><td>www.asx.com.au</td><td></td></tr><tr><td>CBOT</td><td>Chicago Board of Trade</td><td>www.cbot.com</td><td></td></tr><tr><td>CME</td><td>Chicago Mercantile Exchange</td><td>www.cme.com</td><td></td></tr><tr><td>COMEX</td><td>Commodity Exchange Inc.</td><td>www.comex.com</td><td>Metals division of NYMEX.</td></tr><tr><td>ICE Futures US</td><td>Intercontinental Exchange</td><td>www.theice.com</td><td>Previously known as NYBOT.</td></tr><tr><td>EUREX</td><td>Eurexchange</td><td>www.eurexchange.com</td><td></td></tr><tr><td>Euronext</td><td>Euronext</td><td>www.euronext.com</td><td></td></tr><tr><td>HKEX</td><td>Hong Kong Exchange and Clearing</td><td>www.hkex.com.hk</td><td></td></tr><tr><td>ME</td><td>Montréal Exchange</td><td>www.m-x.ca</td><td></td></tr><tr><td>MEFF</td><td>Mercado Español de Futuros Financieros</td><td>www.meff.es</td><td></td></tr><tr><td>NYMEX</td><td>New York Mercantile Exchange</td><td>www.cme.com</td><td>Now a division of the CME.</td></tr><tr><td>SGX</td><td>Singapore Exchange</td><td>www.sgx.com</td><td></td></tr><tr><td>TGE</td><td>Tokyo Grains Exchange</td><td>www.tge.or.pj</td><td></td></tr><tr><td>TOCOM</td><td>Tokyo Commodity Exchange</td><td>www.tocom.or.jp</td><td></td></tr><tr><td>TSE</td><td>Tokyo Stock Exchange</td><td>www.tse.or.jp</td><td></td></tr><tr><td>WCE</td><td>ICE Futures Canada</td><td>www.theice.com/clear_canada.jhtml</td><td>Previously Winnipeg Commodity Exchange</td></tr><tr><td>CSCE</td><td>Coffee, Sugar and Cocoa Exchange</td><td>www.theice.com</td><td>Now a division of ICE.</td></tr><tr><td>NYCE</td><td>New York Cotton Exchange</td><td>www.theice.com</td><td>Now a division of ICE.</td></tr></table>

## Futures and currency exposure

If you are an international investor or trader and mostly used to cash instruments such as stocks, the concept of currency exposure when it comes to futures will be quite different from what you are used to. With cash instruments the currency exposure is always very clear and straightforward but that is not necessarily the case with futures. If you are a Swiss-based investor buying a US$100,000 worth of IBM in New York, you also need to buy the dollars to pay for it, at least if for a moment we disregard Lombard financing and such. That means that after the transaction you have US$100,000 exposure to the stock price of IBM and at the same time US$100,000 worth of exposure to the US dollar (USD) against the Swissie (CHF). This exposure can have a major impact on the return of your investment and is a major factor in any quantitative analysis of the trade. Consider the following example: 

• You are a Swiss-based investor buying 1,000 shares of IBM in May 2007 at exactly US$100 each. 

• The exchange rate is about 1.21, so you have to exchange 121,000 CHF to pay for the purchase. 

• Three and a half years later the price of IBM is up to 122 and you would like to sell and take home your 22% gain. 

• The exchange rate now is about 1.01. 

• When you sell your IBM stocks for US$122,000 and then exchange it back to Swissie, you only have 123,000 Swissie left, leaving barely enough to pay for commissions. 

This is an age-old problem with cash equities strategies where one needs a strategy for whether to hedge all currency risks, run an overlay currency trading on top of the strategy or simply accept all currency exposure. With futures the situation is quite different. 

When you open a futures position, no money actually changes hands except from your commission fees. What you opened is just a commitment to buy or sell something at a future time. As mentioned, an overwhelming majority of all futures contracts are of course closed out by taking an offsetting position before it is time to buy or sell, but that is beside the point here. The fact that no money changes hands on initiation of the position means that you have much less foreign exchange risk than you do with cash instruments. Consider a similar example to the IBM trade above: 

• You are a UK-based investor buying 10 contracts of the big Nasdaq futures at the price of US$2,000. The exchange rate at the time of purchase is 1.56, but that is in fact almost irrelevant. 

• You close the position by selling offsetting contracts at the price of US$1,834 just a few weeks later. 

Now your loss is US$166,000, which you calculate by taking the price difference of 166 points, multiplying by the point value (which in the case of the Nasdaq contract is 100) and finally multiplying by the number of contracts held, to end up at US$166,000. 

The exchange rate at the time of closing the position is 1.44 and so your loss in your own currency ends up at more or less £115,300, and the exchange rate at the time of opening the position has no actual bearing on this number. 

As seen here, the only exchange rate that has any bearing on the final settlement of the position is that of the closing day, or rather when you bring the resulting profit or loss back to your own base currency, but don’t let that lead you to believe that exchange-rate fluctuations have no bearing on your futures profits and losses. You certainly have to have an exposure to currencies with futures, just not on the notional amount as you do with cash instruments. Your exposure is instead on the profit and loss (P&L), and so only your current profits or losses are subject to currency risk. You therefore have a very dynamic currency exposure and the extent of it varies day by day and even hour by hour as your positions move. This is a much smaller factor than what you have to deal with in cash-instrument strategies, but a much more difficult one to hedge. You may also need to keep some cash in various currencies with your broker just to make sure you don’t get charged fees unnecessarily for overdrawing accounts when you make losses. 

The important point is to understand that you always have a currency risk on your futures P&L and it requires additional care to manage. 

# FUTURES DATA

When dealing with quantitative strategies, the most crucial building block is always the data itself. Everything else you do will be based on that data and if you have even a small problem with your data, your calculations and algorithms may all be for nothing and your actual trading results may differ substantially from what your simulations had you predict. The real complication in terms of time series analysis for futures, compared to cash instruments such as stocks, is the fact that futures have a limited life span. For each asset, S&P 500, silver, corn and so on, there will always be many contracts traded at any given time, each with a different expiry month, and they are normally traded at different prices. To be able to do longer-term simulations and test strategies we desperately need long-term data series to work with, which are by default missing in the futures world. All we have is a large number of discrete time series covering only part of the time we need, and it is up to us as traders/analysts to construct usable long-term series out of this. 

## Dealing with limited life span

When trading commences for a new contract there is usually quite a long time left to the expiry date and very little trading activity to be seen. Few people are interested in trading wheat with a delivery several years from now and as such the contract will remain relatively illiquid until it gets closer to expiry. At any given time, there will be one contract in each market, corn, orange juice, gold and so on, which is the most liquid and the contract that almost everyone is trading at the moment. This can sometimes be the contract that is closest to the expiry date, but this is far from certain and there are no firm rules for when the liquidity switches to another contract or even which contract it switches to. For some markets this is very predictable and very straightforward, such as for equity index futures and currency futures, where the most liquid contract with a high degree of certainty is simply the one that has the least time left to expiry and the switch happens on the expiry date itself or just one or two days before it. In some commodity markets both the timing of the switchover and the selection of the next active contract is completely unpredictable. 

For someone focused just on a single market, it is possible to stay close enough to that market to be aware right away when the attention of the traders switch from one contract to another, but as a systematic trader covering a large number of markets you need to find a way to automatically detect such changes. From the perspective of the typical trader, the most liquid contract is the only one that really matters. Although there are CTA managers exploiting pricing differences between different delivery months in the same market, the most common strategies focus solely on the most heavily traded delivery month. 

Figure 2.1 shows the open interest for the S&P 500 futures for three delivery months in 2011. This particular market offers only contracts for March, June, September and December so when the March moves to expiry the trading will normally move to the June contract and so on. The June contract expires on June 16 and shortly before that the open interest starts moving down for that contract while moving up in the next. At the same time, Figure 2.2 shows that the volume spikes up sharply in both the June and the September contract around this time as well. Remember that the open interest will tell you how many contracts are outstanding, that is how many are still uncovered in that particular delivery month. If you buy one S&P contract you will add one to this number, and when you sell it you will decrease this number, and the same is true for the reversed trade of course. 


Figure 2.1 Open interest moving from month to month


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/fa27759dd7db18faac41ecaba3879f9bd8f6bb9986e3096d97b6dd4b4e800416.jpg)



Figure 2.2 Volume spiking at rollover times


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/69f88fff464a80806a71eae4fdb6a1059f0631ca3d688492cbf939e1da54e0b0.jpg)


The reason that the volume goes up while the open interest rolls to the next delivery is that everyone is busy rolling their position, switching out of the June contract and into the September and thereby generating a lot of trade tickets. Since this is a non-deliverable financial future, you could in theory stay with it all the way until it expires, but as you can see in these figures, very few people ever do that. If your desire is to maintain your position in the underlying asset, in this case the S&P Index, you will want to have control over your rollover and buy one month and sell the other at the same time, so that you don’t have any open price risk between closing one contract and opening the other or vice versa. 

What you need is a clear method for when to switch from one contract to another and a notification of when you need to do the rollover. Common methods are to use the volume, the open interest or both in combination and then roll when a new contract has higher open interest and/or volume. Some prefer to require a couple of consecutive days or higher values before rolling, whereas some roll on the first day one contract exceeds another. In the end, this does not make a huge difference as long as you make sure you stay with a highly liquid contract and are aware of how and when to roll. 

## Term structure

The term structure, or yield curve, of a futures market refers to the shape of the curve you get if you plot the price of each successive delivery month in a graph, such as in the heating oil example in Figure 2.3 and Table 2.4. The price of an asset to be delivered in one month is generally quite different from the price of the same asset to be delivered in six months and the overview graph of how these prices change for different delivery dates is called the term structure. 

Figure 2.3 Term structure of heating oil 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/1e8d1345808b2435aa7ac8a213d7be2084b383c0200b6410301bb6eefd60bdfa.jpg)



Table 2.4 Term structure table


<table><tr><td>Ticker</td><td>Name</td><td>Last</td></tr><tr><td>HOH2</td><td>Heating Oil March 2012</td><td>3.2367</td></tr><tr><td>HOJ2</td><td>Heating Oil April 2012</td><td>3.2499</td></tr><tr><td>HOK2</td><td>Heating Oil May 2012</td><td>3.2598</td></tr><tr><td>HOM2</td><td>Heating Oil June 2012</td><td>3.2690</td></tr><tr><td>HON2</td><td>Heating Oil July 2012</td><td>3.2771</td></tr><tr><td>HOQ2</td><td>Heating Oil August 2012</td><td>3.2835</td></tr></table>

In this example, the price level of heating oil for each successive month is going up, which is the normal case. A term structure chart that slopes upwards such as this one is said to be in contango. In some instances the term structure can take on a downward slope and such a situation is called backwardation. These two words are the legacy of a system of deferring payments for stocks on the London Stock Exchange in the mid-19th century, which may explain the rather esoteric terminology. 

To understand why the prices are usually higher further in the future, you need to think of the cost of hedging the position. The fair price of any position is the cost of hedging it, so if you can hedge something you can also price it. If someone sells open 100 gold contracts with delivery one year from now, the way to hedge this would be to buy 10,000 ounces (283 kilograms) worth of physical gold in the spot market now and store it until the time of delivery. Storage of gold is not entirely free unless you really want to keep it in your basement and you would be locking up cash during this year, which you could have received interest on or otherwise used. You would of course need to be compensated for this or the position is not worth taking. 

For financial futures such as equity index futures and bond futures, the interest rate is the main driver of the term structure shape because there is no physical storage required for hedging; you just need to deliver the cash upfront. Therefore, you see less of a steep curve for financial futures than for deliverable ones. On the other hand, there are commodities with severe storage cost where this is the overwhelming factor in the term structure shape. Natural gas for instance is very expensive to store and it therefore tends to show very steep contango. 

Backwardation, or downwards-sloping term structure, is less common but not an anomaly. Backwardation can be caused by seasonality, interest rate conditions or unusual storage cost situations and is not uncommon for softs and perishable commodities. 

## Basis gaps

The current price of two contracts with the same underlying but different delivery months will always be different and this is reflected in the term structure. The April gold contract will be traded at a different price than the December gold contract for the same year, and the same logic goes for any other market as well. Usually the price of the December contract will be higher than the April contract of the same year, in which case we have a contango situation, and this has nothing to do with the expectations of gold price changes. It may be intuitive to think that the higher price of the December contract reflects traders’ view that the gold spot price should move up, but this is not at all the case. Instead the hedging cost, or carry cost if you will, is the core factor in play. The difference in base price between two contracts becomes acutely important when the currently traded contract comes to its end of life and you need to roll to the next. 

Figure 2.4 shows the May and July 2012 rough rice where the July contract is the lighter, broken line. Note that the July is consistently more expensive than the May. This is the normal case but there are times when the relationship can reverse as well and the longer contract can be cheaper than the shorter. 


Figure 2.4 Rough rice basis gap


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/4cf7d5cd1ece1dd191a0c430cd7390dce382ea4ad7149630acab0aaef146de68.jpg)


The reason for this price discrepancy should now be clear: it’s primarily related to hedging or carry costs. The problem that this creates for us is that when creating a continuous time series for long-term simulations, we cannot simply put one contract’s price series after another. Doing so would introduce artificial gaps in the data where there really are no gaps in the actual market. What is required to do proper back-testing simulations is a continuous time series that reflects the actual market behaviour, which does not necessarily mean that it reflects the actual prices at the time. Consider the time series in Figure 2.5, which is a completely unadjusted time series where contract after contract has just been put back to back. The closest contract has always been selected and held until expiry, when the next contract has taken over. This is the default way of looking at continuous futures time series in many market data applications and if you, for instance, chart the c1 codes in Reuters this is what you get. In this example it is easy to see right away when the contract rollovers occurred, even without the circles that I put in. The seemingly erratic 

behaviour of the price during these periods does not at all reflect the actual market conditions at the time and basing your simulations on such data will produce nonsense results. 


Figure 2.5 Unadjusted time series for rough rice


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/576b8b67cb4a05402052d506ed3321d4c01aa3276869ca77929a0e84e4dc39a2.jpg)



Now compare this with the more normal looking price curve in Figure 2.6. Notice how it is no longer possible to see where the contract rollovers occurred and the artificial gaps have been removed. If you look even closer, you will notice that while the final price is the same in the end, there are significant price differences between the two series on the left-hand side of the x-axis. Whereas the peak reading in October was about 17.3, the adjusted chart shows a peak of over 18. The difference can occur in either direction, depending on whether there is a positive or negative basis gap at the time of the roll.



Figure 2.6 Properly adjusted time series for rough rice


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/d04ebf7e36e48810fce841b253505de45a641ae98d52d1c4eee9d71bc91e08e8.jpg)



The reason for this price discrepancy in the past prices is that I use back-adjusted price charts here. For a back-adjusted chart, the current price is always correct at the right-hand side of the series, but all previous


contracts will have a mismatch. When the roll occurs, the back-adjusted series will adjust all series back in time and remove the artificial gap. This means that the whole time series back in time will have to be shifted up or down to match the new series. 

There are several possible ways to achieve this adjustment and most good market data applications offer a choice in this regard, but it does not make a huge difference for the bigger picture which exact method you choose. My preferred method is to identify the liquid contract based on open interest and to link the contracts together so that the old contract’s close matches the new contract’s close on the rollover date, keeping any actual gaps on that day and back adjusting the entire time series all the way from the start of the data. So if you look at the adjusted time series after to see the exact price of corn in June of 1985, it will be very different from what the actual price was at the time since there have been countless adjustments done with all the rollovers that occurred since. However, the real trends of the price series over time have been properly preserved and the most recent price in the series represents the actual price in the market. 

Other methods of adjusting prices can involve using ratios of two contracts, forward adjusting and different methods of using volume and open interest to find the most liquid issue. These are details which are not too important for the long-term strategy but worth experimenting with if you want to look at the finer details. For a comprehensive look at rollover methods, see Jack Schwager’s 1995 book Schwager on Futures: Technical Analysis. 

## FUTURES SECTORS

In comparison to the equities world, you will find that there is a much more limited set of instruments for futures traders although this is not necessarily a drawback. Everyone knows, or should know, that diversification is a good thing and can potentially help improve volatility adjusted results. One might think that given the overwhelming amount of available stocks to trade in the equity universe diversification potential would make for a massive advantage. As it turns out, however, the internal correlation between stocks regardless of sector or region is very high. Even with a highly diversified equity portfolio, you are still just holding equities and they tend to move together even in normal market times; when there is a stress event hitting the markets the correlations quickly approach one. It does of course help to own several stocks over holding one single stock, but the effect is quite limited compared to holding a cross-asset portfolio. 

In contrast, with futures markets you have all kinds of highly different asset classes at your disposal with very different driving factors. You can trade anything from the S&P 500 index to bonds, oil, corn and even livestock. The correlations between some instruments are higher than others and the correlations tend to vary over time, but there is no question that you can get a substantially better diversification effect trading cross-asset futures than you can trading a single asset class such as stocks. It is therefore imperative that you don’t skip any asset classes and make sure that your strategy covers a wide range of markets across all available markets, or you simply miss the plot of diversified futures trading and most likely blow up sooner or later. The inclusion of a wide set of instruments is critical to the long-term stability of the strategies described in this book. 

For the purpose of analysis and allocation, it is useful to divide investment universes into sectors. In the equity world there are many more or less official sector schemes, such as the GICS scheme, FTSE scheme and various local varieties. In the futures world there are several ways to sort the instruments into sector buckets as well, but you will find the schemes less standardised and the chosen method should depend more on what is useful for your purpose. In our case, we just need a practical way to make a distinction between instruments of similar characteristics and underlying instruments. I use a crude but pragmatic scheme consisting of only five sectors: agricultural commodities, non-agricultural commodities, currencies, equities and rates. 

I introduce each of these sectors as well as a selection of important markets within each sector which we will use for the strategies in this book. 

## Agricultural commodities

Purists may take issue with my definition of agricultural commodities, because I include softs, grains, fibres, meats and so on in this sector, but I prefer a practical and pragmatic sector definition to a textbook definition. There is nothing wrong with subdividing this sector into all those components, but it does not add value in this context. 

The agricultural sector might start feeling slightly comical for traders who are used to dealing with stocks, currencies and bonds. In the agricultural space there are quite a few different futures markets where everything from coffee and cotton to lean hogs and livestock can be traded, making it a veritable supermarket. This is, in a way, an excellent sector because the internal correlation between these different markets is not particularly high. Although it never hurts knowing a little bit about what you trade, you can essentially treat each market as just pure numbers, without having to care about what the market driver for, say, wheat demand really is. 

Most agricultural futures are traded in Chicago or New York, but you also find some interesting markets in Tokyo, London and even Winnipeg. The variety of available instruments in this sector is a dream for the diversified futures manager, such as coffee, cocoa, cotton, orange juice, sugar, corn, wheat, lumber, rubber, oats, rice, soybeans, soybean meal, soybean oil, live cattle and lean hogs. They are all affected by inflation to some degree as well as by the US dollar, but these tend to be of lesser importance over the long run and the individual markets show their own clear trends. It is certainly no coincidence that the business of diversified futures started within the commodity sector, and even still retains its name from those days: commodity trading advisors (CTAs). 

The volatility of the different markets in this sector can vary significantly. The contracts in this sector are highly driven by fundamental developments specific to the commodity in question, such as adverse weather in an important production region, crop results and inventory reports. When significant news comes out, there may be substantial moves not only on the day in question, but also for a prolonged period of time. This can be very nice when the move is in your favour, but make sure you are able to take the pain when the moves go against you. Seasonality is also a factor to consider in some of these commodities where cyclical demand or supply can affect the price patterns. 

The exchanges often have so-called limit rules on these markets, meaning that there is a maximum amount the price is allowed to move in a single day. When the price has moved the maximum amount and buyers and sellers agree that the fair price lies beyond, the trading comes to a halt and is said to be in limit lock. The following day the price can move the same amount again, or less if the participants have calmed down by then. 

In this sector all futures are in theory deliverable, which means that if you hold a contract, long or short, past the critical date you may be forced to take or make delivery of the underlying asset. For all deliverable futures contracts, such as gold, live cattle, corn and so on, you need to close out your position long before the actual expiry date. The market conventions and terminology vary between markets, but usually you need to be out before the so-called first notice day. After that day, you could be called upon to make good on your commitment, which means either deliver or take delivery of the underlying. I don’t know about you, but nothing ruins my day like a truckload of live cows parked outside my office. 

For most traders this is only an amusing theoretical scenario with no actual risk, because most brokers will not allow these contracts to go to delivery and therefore shut them down for you in case you had forgotten and could not be reached, but this is not something you want to happen either. Make sure you are always aware of when you should close or roll a position or there will be negative consequences. 

The units used for agricultural commodities are usually a mass unit such as pounds or a volume unit such as bushels, but with various exceptions such as feet for lumber (see Table 2.5 for all the details). 


Table 2.5 Agricultural commodity futures


<table><tr><td>Name</td><td>Point value</td><td>Unit</td><td>Currency</td><td>Exchange</td></tr><tr><td>Azuki red beans</td><td>2,400</td><td>KG</td><td>JPY</td><td>TGE</td></tr><tr><td>Coffee</td><td>37,500</td><td>Lbs</td><td>USc</td><td>CSCE</td></tr><tr><td>Corn</td><td>5,000</td><td>Bsh</td><td>USc</td><td>CBOT</td></tr><tr><td>Cotton</td><td>50,000</td><td>Lbs</td><td>USc</td><td>NYCE</td></tr><tr><td>Lean hogs</td><td>40,000</td><td>Lbs</td><td>USc</td><td>CME</td></tr><tr><td>Live cattle</td><td>40,000</td><td>Lbs</td><td>USc</td><td>CME</td></tr><tr><td>Lumber</td><td>110,000</td><td>Feet</td><td>USD</td><td>CME</td></tr><tr><td>Oats</td><td>5,000</td><td>Bsh</td><td>USc</td><td>CBOT</td></tr><tr><td>Orange juice</td><td>15,000</td><td>Lbs</td><td>USc</td><td>NYCE</td></tr><tr><td>Canola</td><td>20</td><td>Tons</td><td>CAD</td><td>WCE</td></tr><tr><td>Rough rice</td><td>2,000</td><td>Cwt</td><td>USc</td><td>CBOT</td></tr><tr><td>Rubber</td><td>10,000</td><td>KG</td><td>JPY</td><td>TOCOM</td></tr><tr><td>Soybean meal</td><td>100</td><td>Tons</td><td>USD</td><td>CBOT</td></tr><tr><td>Soybeans</td><td>5,000</td><td>Bsh</td><td>USc</td><td>CBOT</td></tr><tr><td>Sugar</td><td>112,000</td><td>Lbs</td><td>USc</td><td>CSCE</td></tr><tr><td>Wheat</td><td>5,000</td><td>Bsh</td><td>USc</td><td>CBOT</td></tr></table>

In the agricultural commodities sector the small player has a clear advantage in that there are a large number of less liquid instruments available with low correlation to other assets. They are liquid enough for trading accounts of a few tens of million dollars, perhaps even over a hundred million, but the big players in the field simply cannot get any useful profits out of them because of their size. It simply is not possible to trade huge amounts of Japanese rubber or European potatoes and this keeps the huge CTA funds away. If you manage reasonably small accounts, this is the sector where you can go nuts and add all kinds of obscure markets to help improve your risk-adjusted returns. The relatively low internal correlation in this sector means that you can get significant diversification benefits from adding more markets. 

## Non-agricultural commodities

This is again a pragmatic sector definition, which you are unlikely to find in more purist literature on the subject. I have mixed energies and metals into one sector because they fit more together with each other than they do with the agricultural commodities (see Table 2.6). 


Table 2.6 Non-agricultural commodity futures


<table><tr><td>Name</td><td>Point value</td><td>Unit</td><td>Currency</td><td>Exchange</td></tr><tr><td>Gasoil</td><td>100</td><td>Tonne</td><td>USD</td><td>NYMEX</td></tr><tr><td>Crude oil</td><td>1,000</td><td>Barrels</td><td>USD</td><td>NYMEX</td></tr><tr><td>Heating oil</td><td>42,000</td><td>Gallons</td><td>USD</td><td>NYMEX</td></tr><tr><td>Natural gas (HH)</td><td>10,000</td><td>mmBTU</td><td>USD</td><td>NYMEX</td></tr><tr><td>Gasoline</td><td>42,000</td><td>Gallons</td><td>USD</td><td>NYMEX</td></tr><tr><td>Gold</td><td>100</td><td>Troy Ounces</td><td>USD</td><td>COMEX</td></tr><tr><td>Copper</td><td>25,000</td><td>Pounds</td><td>USc</td><td>COMEX</td></tr><tr><td>Palladium</td><td>100</td><td>Troy Ounces</td><td>USD</td><td>NYMEX</td></tr><tr><td>Platinum</td><td>50</td><td>Troy Ounces</td><td>USD</td><td>NYMEX</td></tr><tr><td>Silver</td><td>5,000</td><td>Troy Ounces</td><td>USc</td><td>COMEX</td></tr></table>

The energy group is a bit limited in terms of instruments, but offers some interesting opportunities. The dominating theme in this sector is oil and its different products, where light sweet crude oil forms the core. This is essentially the product they pump out of the ground in various regions of the world with horrible climates and extremist leaders, such as Saudi Arabia, Texas and Alaska. The main products from crude oil are heating oil, gasoil and gasoline, all tradable and highly liquid in the futures market. These four markets usually have a fairly high correlation to each other, but at times the driving factors behind them work independently and their trends can decouple for extended periods. They are all very prone to long-term trends and well suited for a diversified futures trend-following method. 

There is another highly interesting instrument within the energy sector as well, which is usually not very correlated to the oil theme, and that is the Henry Hub (HH) natural gas. This is a bit of a special animal and rather unique in its behaviour. Natural gas is mainly used for power generation and is pumped out of the ground chiefly in Russia and the US. The unique property of this particular commodity is its persistently sharp contango, which means that the prices of contracts deliverable further in the future are more expensive than contracts that expire sooner, and that the term structure chart thereby is sloping upwards. Most commodities display somewhat of a contango due to the cost of hedging the position as explained earlier (the main reasons being cost of storage and opportunity cost of capital although for some markets seasonality holds a large part of the explanation as well). 

For natural gas, the contango is very large and for good reason. This particular commodity has a very low density, which makes storage extremely expensive. The method of hedging a short futures contract of natural gas would be in theory to buy it today, store it in huge domes or silos that are often located underground, and then deliver it against the contract upon expiry (or of course to just let it stay in the ground and take it up later on instead). As a futures trader, of course, you are not concerned with dealing with the actual physical commodity, but the hedging method is still theoretically valid for pricing and you need to understand why the term structure chart looks the way it does, and how it can work in your favour. The cost-of-carry hedging model applies mainly to commodities that can be stored and for assets such as oil this is the core driver of the term structure shape. For natural gas, with its highly complicated and nigh impossible storage situation, the curve is also in large part driven by the seasonal demand patterns for the underlying asset (Figure 2.7). 


Figure 2.7 Term structure of natural gas


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/b8989fb539e355b7c7267a0e7f2fc6ab0e5640ba7e05dbacda9ca442033df3f7.jpg)



At the time of writing, the price difference in the May contract and the September 2012 contract is nearly 5%. The actual price by expiry is often quite stable while the futures contracts are traded much higher,


depending on how far out they are. This means that the points on the term structure curve tend to slowly move down while they are moving left, which is where the profit opportunity lies; commodities with sharp persistent contango trend strongly downwards and the money is on the short side of the game as long as the shape persists. 

Sharp contango situations, as well as backwardation, can offer great opportunities but also require that you really take care of the problem of obtaining corrected time series. The trend in something like natural gas will look highly different if you simply paste one futures contract after the next as opposed to adjusting properly for basis gaps when they are spliced together. Figure 2.8 illustrates the problem, where the lighter line lacks any adjustment and simply displays the actual prices of each contract followed by the next contract upon expiry, while the second one uses a back-adjustment method as described earlier. So did the actual price move up or down? It depends on your point of view, but for a futures trader it absolutely collapsed and there was a ton of money being made on staying short. The spot price did not change anywhere near as much and actually went up over time, but if you traded the futures that is completely irrelevant because the contango effect overshadowed the spot price moves over time. 


Figure 2.8 Adjusted versus unadjusted data for natural gas


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/0ee70c34693844a9736ebd2c745bd5e575b1b8008e6aa00e52cc1bb09b6a39d7.jpg)


Then we have the metals where you find both the base metals and the more shiny kind. There are only four precious metals of interest for a trader because there are no liquid markets in ruthenium, osmium and other more obscure precious metals. The elephant in this sector is naturally gold, which has a dual use as a shiny status symbol and as a psychological protection against inflation and various end-of-the-world scenarios. The value of gold is largely psychological and somewhat political because the industrial use of it is limited, but one should never underestimate the madness of large groups of people. Gold tends to be seen as a store of value and a protection against inflation, deflation, wars, riots and zombie attacks. It does have these properties in some sense, but only because a lot of people have agreed on this logic. If the state of the world turns ugly in a serious way and the chanting crowds with the pitchforks are approaching your house, you are probably better off with canned food and a shotgun than with gold bars. Still, gold shows excellent long-term trending patterns and certainly should be included in a diversified futures strategy. 

Often seen as the little brother of gold, silver has a fairly high correlation to gold, but it has its own merits as well. This metal has more industrial use and in many respects different drivers of performance. Apart from these two well-known precious metals, there is also platinum and palladium, which both at times can show truly excellent trending patterns. These two metals are less liquid than gold and silver but for a small- to medium-sized managed futures fund, they are absolutely liquid enough. 

The most common futures market in base metals is copper, traded in Chicago. Most other base metals are primarily traded in London on the London Metal Exchange (LME), and are not in fact futures but forward contracts. In that exchange you can find the less exciting sounding metals such as zinc, aluminium, lead and so on. They can be traded on the same principles as their futures brethren and the differences between the futures and forwards markets are not that significant. 

# Currencies

If you are not used to trading currencies you may need some time to get used to the concept. A Euro-based investor who buys a contract of the German MDAX future is doing something very straightforward: buying a basket of stocks traded in her own currency. If the same investor buys gold futures, she is buying gold against the US dollar, which is still fairly straightforward, but when the same person buys the Mexican peso contract she is long peso against dollar and is taking a bet on two completely different currencies. Trading currencies makes it more important to understand that in every single position, regardless of asset class or sector, you are always long something and short something. If you buy IBM shares, you are long IBM and short dollar and so on. Yes, you might already have the cash dollars to pay with, but the acquisition of those dollars belongs to a different position with its own long and short leg. 

In the same way, when you enter a currency future you are long one currency and short the other. There are many available currency futures and quite a few of them are very liquid. The spreads are very tight and often better than on the forwards. The currency markets are the most liquid in the world and the spot market can swallow just about any volume. This is highly useful for very large CTA funds that tend to trade a large portion of their funds in currencies when they get so big that it is getting difficult and expensive to move positions in many other markets. If you study the asset allocation of the extremely large trend followers with assets in the billions, you will find that they have the bulk of their money in the currency markets. 

Many currency futures are crosses against the USD and if only one currency is named, it is implied that it is against the USD (see Table 2.7). Therefore the CHF future is a bet on the exchange rate between the CHF and the USD. There are also a growing number of non-USD crosses, such as the Euro/Yen future and so on. This sector offers some interesting diversification possibilities if you use these types of crosses. Always be aware of the danger of stacking up USD risk and be sure to monitor the risk you are taking here. If you are long the euro future, long the CHF future, the yen future, the British pound future and the Aussie future, you are really just short dollar and when the dollar recovers, you get hit on all positions at once. Taking these positions may still at times be a good idea, just as long as you are aware of the risk and model it properly so you know what to expect when things turn against you. 

Table 2.7 Currency futures 

<table><tr><td>Name</td><td>Point value</td><td>Unit</td><td>Currency</td><td>Exchange</td></tr><tr><td>AUD/USD</td><td>100,000</td><td>AUD</td><td>USD</td><td>CME</td></tr><tr><td>GBP/USD</td><td>62,500</td><td>GBP</td><td>USD</td><td>CME</td></tr><tr><td>EUR/USD</td><td>125,000</td><td>EUR</td><td>USD</td><td>CME</td></tr><tr><td>CAD/USD</td><td>100,000</td><td>CAD</td><td>USD</td><td>CME</td></tr><tr><td>JPY/USD</td><td>1,250</td><td>Million JPY</td><td>USc</td><td>CME</td></tr><tr><td>NZD/USD</td><td>100,000</td><td>NZD</td><td>USD</td><td>CME</td></tr><tr><td>NOK/USD</td><td>200,000</td><td>NOK</td><td>USD</td><td>CME</td></tr><tr><td>ZAR/USD</td><td>500,000</td><td>RND</td><td>USD</td><td>CME</td></tr><tr><td>SEK/USD</td><td>200,000</td><td>SEK</td><td>USD</td><td>CME</td></tr><tr><td>CHF/USD</td><td>125,000</td><td>CHF</td><td>USD</td><td>CME</td></tr><tr><td>EUR/CHF</td><td>125,000</td><td>EUR</td><td>CHF</td><td>CME</td></tr><tr><td>EUR/GBP</td><td>125,000</td><td>EUR</td><td>GBP</td><td>CME</td></tr><tr><td>EUR/JPY</td><td>125,000</td><td>CHF</td><td>JPY</td><td>CME</td></tr></table>

## Equities

This is the largest futures sector in terms of amount of available instruments and the easiest for most people to relate to. Buying a basket of stocks in a well-defined market is a very straightforward concept and understanding the potential risk and reward of such a trade is fairly intuitive. The percentage moves of the underlying indices are published daily on news websites, TV screens and newspapers. We are only dealing in equity index futures in this book and not with single stock futures and the reason for this is not just simplification as one might think, but rather that I find single stock futures of much less interest and they are just not terribly helpful in diversified futures strategies. 

Just as single cash equities have high internal correlation, so of course do equity futures. It can be very tempting to include a large number of equity futures in your strategy because there are so many to pick from, but I would advise against allocating too high a risk to this sector, as it can easily put you in a corner portfolio with the illusion of diversification when you are in fact just putting on massive bets on equity beta. Nevertheless, equity futures do have a place in a diversified futures strategy and representative contracts from several different geographical markets should be included. As Table 2.8 shows, I include the large US futures such as the S&P 500 and the Nasdaq 100 as well as European representatives such as the EuroStoxx 50, FTSE 100, GDAX and CAC40 and a few Asians such as Hang Seng and Nikkei 225. In Asia you also have some interesting Chinese exposure opportunities by including the Hang Seng China Enterprises and the MSCI Taiwan. 

Table 2.8 Equity futures 

<table><tr><td>Name</td><td>Point value</td><td>Unit</td><td>Currency</td><td>Exchange</td></tr><tr><td>CAC 40</td><td>10</td><td>Index points</td><td>EUR</td><td>Euronext</td></tr><tr><td>DAX</td><td>25</td><td>Index points</td><td>EUR</td><td>EUREX</td></tr><tr><td>EuroStoxx</td><td>10</td><td>Index points</td><td>EUR</td><td>Euronext</td></tr><tr><td>FTSE 100</td><td>10</td><td>Index points</td><td>GBP</td><td>Euronext</td></tr><tr><td>Hang Seng</td><td>50</td><td>Index points</td><td>HKD</td><td>HKEX</td></tr><tr><td>Hang Seng China Enterprises</td><td>50</td><td>Index points</td><td>HKD</td><td>HKEX</td></tr><tr><td>IBEX 35</td><td>10</td><td>Index points</td><td>EUR</td><td>MEFF</td></tr><tr><td>MSCI Taiwan</td><td>100</td><td>Index points</td><td>USD</td><td>SGX</td></tr><tr><td>Nasdaq 100</td><td>100</td><td>Index points</td><td>USD</td><td>CME</td></tr><tr><td>Nikkei 225</td><td>5</td><td>Index points</td><td>USD</td><td>CME</td></tr><tr><td>S&amp;P 500</td><td>250</td><td>Index points</td><td>USD</td><td>CME</td></tr><tr><td>S&amp;P 60</td><td>200</td><td>Index points</td><td>CAD</td><td>ME</td></tr><tr><td>SPI 200</td><td>25</td><td>Index points</td><td>USD</td><td>ASX</td></tr></table>

One thing to keep in mind here is that most diversified futures strategies go both long and short and tha the short side of equities usually has a very different profile from the long side. When equities are in a bul market, they can move slowly upwards in an orderly fashion for long periods of time, compounding gains week after week and be highly profitable. On the downside, equity moves tend to be swifter and more violent. Sharp drop-downs followed by v-shaped reversals create a very dangerous trading environment. Many strong diversified futures programmes struggle on the equity sector and it is not uncommon even for good systems to lose money consistently over time on that game. Even so, I would not recommend that you cut out short equity futures from your trading universe. You are likely to end up without significant profits in the long run, perhaps even in a loss, but in the shorter run it provides a very valuable diversification and can smooth out returns. When the bad years for the equity markets come along, the short side of your equity trades can make very good money and help you recover from what otherwise might be a very bad year for you. 

The unit used for equity index futures is simply points on the relevant index, which makes this a very simple calculation in terms of profit and loss. For example, if you buy five contracts at 100 and sell them at 110 and the point value for this particular contract is 10, your gain is $( ( 1 1 0 - 1 0 0 ) \times 5 \times 1 0 \times 1 ) = 5 0 0$ of the currency in question. 

## Rates

In this sector I include practically everything on the yield curve, from the far left to the far right. The behaviour of instruments very far apart on this scale can seem like very dissimilar instruments in that the level of volatility will be extremely different and that has to be taken into account for position sizing. The far left of the yield curve always has a much lower volatility than the far right since these instruments have much lower duration and therefore a much lower interest rate risk, but going into the finer points of fixed income mathematics is far outside the scope of this book. You don’t need to have read all Fabozzi’s books on the subject to be able to trade bond futures but it does not hurt to get a little basic knowledge. The key point to understand is that volatility decreases drastically on the far left side and it goes up the farther on the right you move. 

Take a look at Figure 2.9. Starting on the left end we have the short-term interest rate futures, often based on loans of 30 or 90 days. These futures, often shorted down to just STIRs, are bets on changes in interest rates on the left side of the curve. The major difference between this sector and the bond futures is the aforementioned massive difference in potential price moves on the left and the right side of the curve. If the 30-year US Bond moves 1% in a day that is a slightly larger than normal move, but nothing to write home about; a 1% move in a STIR future on the other hand would take a cataclysmic world event. The 

quick conclusion from this should be that one needs to take massive leverage in STIRs to get any form of profit or loss that actually matters, as scary as that might sound. 


Figure 2.9 US benchmark yield curve


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/fd17d4492301ffcb28b79b0e4ec0178cfbf95429998dbf848cac589f67ef29a9.jpg)


Also be careful to get the underlying contract value and the point value right since this works a little differently than for other sectors. Let’s take the Eurodollar as an example, which is based on the three months US Dollar LIBOR – although don’t confuse this with the currency rate Euro/Dollar which is something utterly different. The term Eurodollar was coined long before the European currency was conceived and refers to the interest rate of time deposits in USD outside the United States. The notional underlying of this contract is US$1 million and quoted as 100 minus the annual three months LIBOR rate. To get to the point value you therefore need to first divide the notional by 100, just like you would with bond futures, but you also need to divide again by four because the contract is for the quarterly rate and not the annual, despite being quoted as such. So if the Eurodollar contract moves from 98 to 99 the profit or loss impact on one contract is then US$2,500. Of course, a full point move in such an instrument does not exactly happen overnight. 

Short-term interest futures often scare people away because you need to take on what feels like a massive position to get any sort of real profit or loss out of it. As you will find, in a diversified futures portfolio the notional underlying exposure of the fund is completely dominated by this sector for that very reason. Comparing with gold as an example, you often need to take on up to 50 times the notional amount to get to the same level of risk, if normalised for volatility, or rather for potential price fluctuations to be more accurate. Most people might be okay with holding US$1 million worth of gold in a US$5 million portfolio, but would you sleep easily at night if you also held a US$50 million position in the Eurodollar in the same portfolio? Nevertheless, this is essentially a fallacy to avoid and you should be concerned with actual risk and not with notional amounts. 

From about year 2 on the curve we have the bond futures where there is an actual underlying bond to be delivered at expiry. Bond futures are quoted in per cent of par, just as a normal bond. That means of course that as yields move up, bond futures moves down and vice versa. Each bond futures contract has certain specifications, such as maturity, coupon, issuer and so on, and in theory there are often several different actual bonds that could be delivered against the contact upon expiry. In reality, however, only one bond will be cheapest to deliver and that is the one that will change hands between those who choose to keep their contracts open to the end. As a trader, you don’t want to keep your contracts open until expiry though, as you would then have to deal with the actual bonds. The most liquid and therefore most interesting bond futures are those on bonds issued by the respective governments of the USA, Germany, the UK, Australia, Canada and Japan although other countries’ debt may also be of interest to you should you want to expand in this sector. 

A bond future is tied to a certain, although often approximate, maturity. For the US for instance, the contracts of interest are the 2-year note, the 5-year note, the 10-year note and the 30-year t-bond. In Germany the terminology is less straightforward, where the longest-term contract is called the Buxl and represents a German government debt with a remaining term of 24–35 years. There is also the Bund with a duration of 8.5–10.5 years, the Bobl with 4.5–5.5 years and the Schatz with 1.75–2.25 years (see Table 2.9). 


Table 2.9 Rates futures


<table><tr><td>Name</td><td>Point value</td><td>Unit</td><td>Currency</td><td>Exchange</td></tr><tr><td>AU 10Y</td><td>1,000</td><td>Bond price</td><td>AUD</td><td>ASX</td></tr><tr><td>AU 3Y</td><td>1,000</td><td>Bond price</td><td>AUD</td><td>ASX</td></tr><tr><td>AU 90 Day</td><td>2,500</td><td>Price</td><td>AUD</td><td>ASX</td></tr><tr><td>Bobl</td><td>1,000</td><td>Bond price</td><td>EUR</td><td>Euronext</td></tr><tr><td>Bund</td><td>1,000</td><td>Bond price</td><td>EUR</td><td>Euronext</td></tr><tr><td>CD 10Y</td><td>1,000</td><td>Bond price</td><td>CAD</td><td>ME</td></tr><tr><td>CD 90 Day</td><td>2,500</td><td>Price</td><td>CAD</td><td>ME</td></tr><tr><td>Euribor</td><td>2,500</td><td>1 million EUR</td><td>EUR</td><td>Euronext</td></tr><tr><td>Euroswiss</td><td>2,500</td><td>1 million CHF</td><td>CHF</td><td>Euronext</td></tr><tr><td>JP 10Y</td><td>1,000</td><td>Bond price</td><td>JPY</td><td>TSE</td></tr><tr><td>Long gilt</td><td>1,000</td><td>Bond price</td><td>GBP</td><td>Euronext</td></tr><tr><td>Schatz</td><td>1,000</td><td>Bond price</td><td>EUR</td><td>Euronext</td></tr><tr><td>Short sterling</td><td>1,250</td><td>£500,000</td><td>GBP</td><td>Euronext</td></tr><tr><td>US 10Y</td><td>1,000</td><td>Bond price</td><td>USD</td><td>CME</td></tr><tr><td>US 2Y</td><td>2,000</td><td>Bond price</td><td>USD</td><td>CME</td></tr><tr><td>US 5Y</td><td>1,000</td><td>Bond price</td><td>USD</td><td>CME</td></tr></table>

The price moves in the bond futures depend on the interest rate changes, which in turn is a factor of many things from inflation to investors’ propensity to take risk and the perceived solvency of the issuer. 

The contract value of bond futures is normally 100,000 of the currency in question, although as the pricing is in percentage terms this need to be divided by 100 to arrive at the most common point value for bond futures of 1,000. As a futures trader, the point value is always more important for you to know than the actual contract value. They may often be the same but when they differ, focus on the point value. 

Bond futures as a group have a fairly low level of volatility; however, the longer durations always have a greater volatility than the shorter ones. The longer ones have a higher sensitivity to changes in interest rates and the prices will move much quicker. They are still slower than most other sectors, but there is a very large difference in volatility between a 10-year note and a 2-year note. 

## REQUIRED TOOLS

Before you can start trading, you need to model and test your strategies. For that you will require lots of data, applications for testing strategies and possibly your own database solution. If you are new to programming, I strongly advise that you pick a relevant computer language and start studying. 

## A word about programming

A quantitative trader does need at least a basic understanding of programming or else you are quite helpless in this business. It does not matter if you have never done any programming before or you feel that this is not your main area of expertise. Since you are reading this book I am going to go ahead and assume that you have a certain degree of determination to either get into this business or become better at it. Understanding programming is a vital part of that process and something you need to face. Even if you have access to a team of propeller heads who can build to your specifications, you are still seriously disadvantaged by not understanding the details and not being able to tweak and innovate on your own. Having a secretary does not negate the need for the ability to type. Point and click system building and simplified scripting languages are for consumers and we are shooting for the big leagues here so buckle down, buy a programming book and learn how to write some code. 

## Development environment

The next thing you need is to settle on a primary environment for developing your strategies. Be careful in screening the available software packages and make sure you pick a platform that is really up for the task. Most of the big name software packages for charting and trading systems development are more simplistic and limited than their marketing material may suggest. These packages are often aimed at the consumer retail market and whereas a few professionals might use them as well, that is not their primary purpose and it shows quickly once you try to build something more complex. 

There are a few very good software environments out there though. By good, I mean environments that can be customised to the extreme. The problem with many charting environments is that they are primarily charting applications and not serious strategy development environments. They are made for a very specific and very narrow purpose and if you start going outside of the box that the software designers intended, you find yourself stuck in a corner very quickly. They use their own proprietary scripting languages, which is highly limiting, and they draw a very small box within which you have to try to make do. A good environment is one that allows you to do just about anything, even things the developer of the application never imagined. It also needs to be able to handle very large data amounts and very memoryintensive portfolio strategies and it should preferably use a standard computer programming language as well as allow you to plug in new functionality in the form of DLLs or similar. If the application is just open enough, you can fill any gaps you may find in its functionality. For crunching the amount of data you need in these simulations, a 32-bit program is not good enough and you should make sure that both your operating system and software package are x64 to make full use of the memory in your (I hope) very powerful workstation. 

Two applications I like are WealthLab.Net and RightEdge. They are both based on Microsoft’s Common Language Runtime (CLR) and use C# as their primary strategy-building language. They are very open and one can construct custom DLLs in Visual Studio to augment functionality. WealthLab is definitely easier to learn and use than RightEdge, but the latter has an even higher degree of flexibility and is great for more complex strategy modelling. Another good option is to build in MatLab, should you already be familiar with this environment. Be aware of course that this book is written in 2012 and depending on when you read it, the situation regarding software packages and languages may have changed. 

If you have no set language preference, I recommend studying C# and starting out with modelling in WealthLab. It is a useful language to know and a reasonably friendly environment to start out with. The more advanced programmer may want to look into RightEdge or MatLab instead. For most strategies the differences don’t matter all that much. 

Teaching programming is beyond the scope of this book and I have intentionally avoided printing any programming code. The type of code you need to build to mimic the strategies I explain is not very 

complex and understanding the ideas of what needs to be built is what really matters. Make no mistake though, you do need to understand programming if you want to be in this business. Perhaps you don’t have to be the best programmer in the world, but if you intend to use drag and drop software or some simplistic scripting apps, you might as well find an easier business to be in. 

Whatever environment you settle on, it is possible that you have to construct your own data provider plugin for it. The data provider plug-in is the interface between the application you want to use and your data. Depending on how you store your data and what vendor it comes from, you may need to build your own DLL to plug into the application so that it can read directly from your source. This is usually a quite simple task though and if you are lucky someone may have already created the interface you need and made it available on the Internet. 

## Data vendors

If you deal only in equity strategies with a limited market set, such as only the US stock market, you can easily find free online data sources of a decent quality that a systematic trader on a tight budget can use. For futures, however, things are a little more complicated. Getting hold of the individual time series for each futures contract, like the December 2005 soybeans, is not difficult, but then you need to adjust and maintain your own data, which can be both time-consuming and error prone. Luckily there are good data providers who can supply the daily adjusted data for a reasonable cost, such as CSI Data and similar. You can also export quality data from some general market data software packages such as Bloomberg, but tha of course comes with a very different price tag. 

Investigate potential data vendors and make sure they cover all markets you are interested in. They need to be able to adjust automatically the data in the way you prefer to receive it and optimally they should allow great flexibility for you to set your own rules so you can experiment with different methods. The data needs to be delivered automatically each day in a format that suits your needs and fits your chosen simulation software. Also don’t underestimate the value of metadata. It helps greatly to have easy access to metadata for each market you cover, such as point value, currency, sector, trading hours, margin requirements and so on. 

While I am mentioning products and companies by name, I should point out that I don’t get paid by any of them, nor do I have any discounts or other benefits from any, and I’m willing to switch to different vendors if a better product comes around. 

## Data storage

You have two main ways you can go in terms of data storage: either you can rely completely on your chosen data provider and let your strategy modelling software and tools work directly against this source, or you can create your own local database. If your software talks directly to your vendor’s database you will be a little more vulnerable and if its source happens to be down while you need to work that can cause a bit of a problem. Some vendors shut down for maintenance on weekends for instance and perhaps you need access to the data then. Other vendors will automatically send you text files with data on a daily basis, which counters the risk of server downtime on their side but still makes you very dependent on their technical formats and standards. This is very much a matter of preference, but I like to create generic database solutions in-house, so that the critical part of the business is always shielded from the particulars of any individual data provider. This makes it easier to switch provider if needed or mix data from severa providers and in general gives you much more freedom and control over your own data. Setting up a MySql database or similar and having your strategy modelling software speak directly to that is both inexpensive and easily done. 

# Constructing Diversified Futures Trading Strategies

In this chapter and the next two, I demonstrate how extremely simple strategies can be used to achieve results very close to what the big managed futures managers display. Some large futures funds treat their proprietary strategies as if they are photos of the Roswell alien landing and like to talk about how they have vast staffs of PhDs and massive research budgets, and in most cases this is true. The question you should ask, however, is just how big a difference this really makes. Once you reach the size of having a few hundred million under management, hiring a staff of researchers to improve details is a good idea, but in fact a single person can replicate the bulk of the returns with some decent software and a bit of hard work. 

I describe two very basic trend-following strategies using the most common approaches to capturing trends. I then make some slight adjustments to these strategies and combine them into a single, and more realistic, strategy. I analyse the resulting strategy in detail and compare it with the results of the big-name futures funds. 

Through this exercise I intend to show that you don’t need complicated mathematics to construct a working trend-following portfolio strategy and that the exact buy-and-sell rules are largely irrelevant. The concept is important but the common focus on entry and exit rules is misguided. 

## THEY ARE ALL DOING THE SAME THING

I make the somewhat bold claim in this book that the trend-following futures managers out there are more or less doing the same thing and that this is not a very complicated thing to replicate. I have to admit that part of the reason I make this claim is that the controversy of the statement itself should catch your eye and if you are still reading this book I have probably succeeded so far, but I am serious in my statement and I intend to prove it. Of course many funds have their own clever little tweaks which may make a substantial performance difference over time and my statement is in no way intended to belittle the successful futures managers in this field, rather the contrary. There is a clear difference between understanding how to construct a successful strategy and having the ability, drive and willpower to make it happen in reality. That is the tough part that can never be properly taught. The entrepreneurs who started the funds I mention in this book have achieved incredible success and should receive their proper credit for it. 

The first chart I show (in Figure 3.1) is not so much for comparison purposes but to provide an overview of the performance profile for this type of fund. The table shows you a number of funds in this field and how they have performed since their inception and because they all have different dates of inception the starting point will be different for them. Millburn is the one with the longest official track record and I include both old legendary funds and newer and less known funds. These funds have different volatility profiles and different investment universes, but if you look closely you can see that they quite often show peaks and troughs at the same time. We can also see that a few of the funds with very strong long-term track records had really bad starts but picked themselves up and moved on, something that is extremely hard to do in reality. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/7d1aedb58ca4daf13dfc89ef820d7a13bb154916fc6a9d4af982a96464172f25.jpg)


To better put the numbers into context, consider Table 3.1 with the basic performance data. The compound annualised return of these funds is not only high, it is quite remarkably high, and in combination with the drawdown numbers and volatility figures they look even better. The lowest annualised return of these funds is still in the double digits while the stock market in the long run comes nowhere close to that. Since 1977 when the oldest fund in our example list, Millburn, was founded, the MSCI World Index has yielded a compound annual return of 8%. To further put these numbers into perspective, the world stock market had an annualised standard deviation of 15% and a maximum drawdown (DD) of 55%, making it a highly inferior investment vehicle any way you look at it. 

Table 3.1 Trend-followers’ performance 

<table><tr><td></td><td>Ann. compound return (%)</td><td>Max DD (%)</td><td>Correlation to MSCI World</td><td>Starting date</td></tr><tr><td>MSCI World Total Return</td><td>8.0</td><td>-55.0</td><td></td><td>Feb-77</td></tr><tr><td>Millburn Multi Markets</td><td>16.6</td><td>-25.6</td><td>-0.01</td><td>Feb-7/</td></tr><tr><td>Dunn World Monetary and Agriculture</td><td>14.4</td><td>-60.3</td><td>-0.03</td><td>Nov-84</td></tr><tr><td>Hyman Beck Global Portfolio</td><td>11.1</td><td>-29.3</td><td>-0.10</td><td>Apr-91</td></tr><tr><td>SuperFund Green Q AG</td><td>12.1</td><td>-32.8</td><td>-0.05</td><td>Mar-96</td></tr><tr><td>Mulvaney Global Markets Fund</td><td>15.4</td><td>-41.3</td><td>-0.16</td><td>May-99</td></tr><tr><td>Transtrend Standard Risk</td><td>9.8</td><td>-10.9</td><td>-0.05</td><td>Jun-92</td></tr><tr><td>Sunrise Expanded Diversified</td><td>11.9</td><td>-19.9</td><td>-0.13</td><td>Jan-96</td></tr><tr><td>Winton Futures Fund B</td><td>16.2</td><td>-25.6</td><td>0.00</td><td>Oct-97</td></tr><tr><td>Rabar Market Research Diversified Program</td><td>12.9</td><td>-29.8</td><td>0.01</td><td>Jan-89</td></tr><tr><td>Clarke Capital Management Worldwide</td><td>13.8</td><td>-26.6</td><td>-0.11</td><td>Jan-96</td></tr><tr><td>Chesapeake Capital Diversified</td><td>12.8</td><td>-27.8</td><td>0.15</td><td>Feb-88</td></tr><tr><td>Abraham Trading Company Diversified Program</td><td>18.7</td><td>-32.0</td><td>-0.08</td><td>Jan-88</td></tr><tr><td>Estlander &amp; Partners, Alpha Trend</td><td>12.1</td><td>-16.5</td><td>0.08</td><td>Oct-91</td></tr></table>


Obviously these strategies have very different risk profiles because their annualised return numbers and risk numbers come out quite far apart, and so you may be wondering where I am going with this argument about them all doing almost the same thing. Have a look at Figures 3.2 and 3.3, which should help prove my point. Figure 3.2 shows the performance of a representative group of futures funds rebased to 100 in 2004. The data is the pure track record of each fund and as you can see they don’t look too similar at first glance except that almost all were profitable in this period. The similarities are not that large until you start digging into the details. Don’t worry about identifying which line is for which fund, that’s not important to the point I am making, which is why I removed the legend. It is the same set of funds shown in Table 3.1 and the important point here is to observe the similarities. 


Figure 3.2 Performance comparison of futures funds since 2004: unadjusted 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/3af61b05c04e405867f61a6ec2fd28a27c0950d7a46c3f8cd590faff5a205f80.jpg)



Figure 3.3 shows the exact same funds and more importantly the exact same y-axis scale. The only difference is that the return of each fund has been adjusted based on the standard deviation of its returns. In essence, I have merely normalised the returns for volatility to compare them on an equal footing. Naturally you can still see some difference between the funds, but the notion that they are all working with the same base concepts should be very clear from this picture. Some perform better than others but they all react at the same time to the same events. The main differences between these funds are what investment universe they use, more specifically how their sector allocation looks, what time frame they primarily operate on and what risk level they are using.



Figure 3.3 Performance comparison of futures funds since 2004: normalised for volatility


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/e58cddac6aa489d9394a1ad825ebd7aa1ae859a7b5d4bee2aac5d47527a50dbb.jpg)



The correlation in Table 3.2 is based on monthly log return numbers and shows that none of these funds have any correlation to the world equity markets to speak of, but they do have quite high correlation to each other. Some funds have as high a correlation coefficient as 0.8 making them more or less identical funds. This does not in any way mean that these funds are bad and their return numbers alone show that they are clearly creating great value for their customers; but the point remains that they are all diversified futures trend followers and there are not a whole lot of different ways this can be done.



Table 3.2 Correlation between futures funds


<table><tr><td></td><td>MSCI World</td><td>Millburn Multi Markets</td><td>Dunn World Monetary and Agriculture</td><td>Hyman Beck Global Portfolio</td><td>SuperFund Green Q AG</td><td>Mulvaney Global Markets Fund</td><td>Transtrend Standard Risk</td><td>Sunrise Expanded Diversified</td><td>Campbell Composite</td><td>Winton Futures Fund B</td><td>Eckhardt Trading Company Standard Plus</td><td>Rabar Market Research Diversified Program</td><td>Clarke Capital Management Worldwide</td><td>Chesapeake Capital Diversified</td><td>Abraham Trading Company Diversified Program</td><td>Estlander &amp; Partners, Alpha Trend</td></tr><tr><td>MSCI World</td><td></td><td>-0.01</td><td>-0.03</td><td>-0.19</td><td>-0.11</td><td>-0.16</td><td>-0.04</td><td>-0.14</td><td>-0.02</td><td>0.01</td><td>0.06</td><td>0.22</td><td>-0.12</td><td>0.20</td><td>-0.10</td><td>0.07</td></tr><tr><td>Millburn Multi Markets</td><td>-0.01</td><td></td><td>0.78</td><td>0.67</td><td>0.78</td><td>0.62</td><td>0.75</td><td>0.74</td><td>0.69</td><td>0.66</td><td>0.53</td><td>0.77</td><td>0.49</td><td>0.68</td><td>0.52</td><td>0.56</td></tr><tr><td>Dunn World Monetary and Agriculture</td><td>-0.03</td><td>0.78</td><td></td><td>0.64</td><td>0.67</td><td>0.60</td><td>0.63</td><td>0.73</td><td>0.67</td><td>0.63</td><td>0.57</td><td>0.67</td><td>0.51</td><td>0.62</td><td>0.47</td><td>0.54</td></tr><tr><td>Hyman Beck Global Portfolio</td><td>-0.19</td><td>0.67</td><td>0.64</td><td></td><td>0.62</td><td>0.65</td><td>0.62</td><td>0.73</td><td>0.59</td><td>0.55</td><td>0.41</td><td>0.62</td><td>0.54</td><td>0.52</td><td>0.56</td><td>0.62</td></tr><tr><td>SuperFund Green Q AG</td><td>-0.11</td><td>0.78</td><td>0.67</td><td>0.62</td><td></td><td>0.67</td><td>0.77</td><td>0.77</td><td>0.70</td><td>0.72</td><td>0.50</td><td>0.73</td><td>0.52</td><td>0.73</td><td>0.62</td><td>0.60</td></tr><tr><td>Mulvaney Global Markets Fund</td><td>-0.16</td><td>0.62</td><td>0.60</td><td>0.65</td><td>0.67</td><td></td><td>0.59</td><td>0.70</td><td>0.54</td><td>0.47</td><td>0.41</td><td>0.60</td><td>0.48</td><td>0.71</td><td>0.55</td><td>0.58</td></tr></table>

<table><tr><td>Transtrend Standard Risk</td><td>-0.04</td><td>0.75</td><td>0.63</td><td>0.62</td><td>0.77</td><td>0.59</td><td></td><td>0.70</td><td>0.70</td><td>0.65</td><td>0.55</td><td>0.73</td><td>0.51</td><td>0.64</td><td>0.55</td><td>0.58</td></tr><tr><td>Sunrise Expanded Diversified</td><td>-0.14</td><td>0.74</td><td>0.73</td><td>0.73</td><td>0.77</td><td>0.70</td><td>0.70</td><td></td><td>0.65</td><td>0.61</td><td>0.47</td><td>0.69</td><td>0.54</td><td>0.72</td><td>0.66</td><td>0.62</td></tr><tr><td>Campbell Composite</td><td>-0.02</td><td>0.69</td><td>0.67</td><td>0.59</td><td>0.70</td><td>0.54</td><td>0.70</td><td>0.65</td><td></td><td>0.56</td><td>0.44</td><td>0.69</td><td>0.39</td><td>0.63</td><td>0.52</td><td>0.48</td></tr><tr><td>Winton Futures Fund B</td><td>0.01</td><td>0.66</td><td>0.63</td><td>0.55</td><td>0.72</td><td>0.47</td><td>0.65</td><td>0.61</td><td>0.56</td><td></td><td>0.53</td><td>0.69</td><td>0.54</td><td>0.62</td><td>0.58</td><td>0.65</td></tr><tr><td>Eckhardt Trading Company Standard Plus</td><td>0.06</td><td>0.53</td><td>0.57</td><td>0.41</td><td>0.50</td><td>0.41</td><td>0.55</td><td>0.47</td><td>0.44</td><td>0.53</td><td></td><td>0.60</td><td>0.60</td><td>0.46</td><td>0.38</td><td>0.48</td></tr><tr><td>Rabar Market Research Diversified Program</td><td>0.22</td><td>0.77</td><td>0.67</td><td>0.62</td><td>0.73</td><td>0.60</td><td>0.73</td><td>0.69</td><td>0.69</td><td>0.69</td><td>0.60</td><td></td><td>0.57</td><td>0.76</td><td>0.51</td><td>0.69</td></tr><tr><td>Clarke Capital Management Worldwide</td><td>-0.12</td><td>0.49</td><td>0.51</td><td>0.54</td><td>0.52</td><td>0.48</td><td>0.51</td><td>0.54</td><td>0.39</td><td>0.54</td><td>0.60</td><td>0.57</td><td></td><td>0.38</td><td>0.46</td><td>0.62</td></tr><tr><td>Chesapeake Capital Diversified</td><td>0.20</td><td>0.68</td><td>0.62</td><td>0.52</td><td>0.73</td><td>0.71</td><td>0.64</td><td>0.72</td><td>0.63</td><td>0.62</td><td>0.46</td><td>0.76</td><td>0.38</td><td></td><td>0.56</td><td>0.59</td></tr><tr><td>Abraham Trading Company Diversified Program</td><td>-0.10</td><td>0.52</td><td>0.47</td><td>0.56</td><td>0.62</td><td>0.55</td><td>0.55</td><td>0.66</td><td>0.52</td><td>0.58</td><td>0.38</td><td>0.51</td><td>0.46</td><td>0.56</td><td></td><td>0.49</td></tr><tr><td>Estlander &amp; Partners, Alpha Trend</td><td>0.07</td><td>0.56</td><td>0.54</td><td>0.62</td><td>0.60</td><td>0.58</td><td>0.58</td><td>0.62</td><td>0.48</td><td>0.65</td><td>0.48</td><td>0.69</td><td>0.62</td><td>0.59</td><td>0.49</td><td></td></tr></table>

It is my intention in this book to dig into the gritty details of what these funds actually are and how they are creating these superior results. As you will see, the underlying methods need not be overly complex and it is absolutely possible for any determined individual to get into this business and compete with the big players. 

# CRACKING OPEN THE MAGIC TREND-FOLLOWING BLACK BOX

Contrary to popular beliefs and widespread myths, trend following is not a terribly complex subject. It is all about waiting for a price to make a move up or down, taking a bet that it will continue in the same direction for a while and sitting on that bet until the price moves enough against you that you conclude that the trend is over. The reason most people still fail at something that seems so simple is that they focus on the wrong things while missing the really important factors. It seems as if too many people spend all their time and effort wondering whether they should use an exponential moving average or a simple one, RSI or Stochastics, combining different indicators, making new indicators, tweaking parameter inputs, adding filters and so on. There are plenty of books around dealing in these tiny differences between a large number of ways of doing the same thing and as much fun as this may sound, it is probably the best way of simply missing the whole plot. 

The core idea of trend following is extremely simple and there is no point trying to make it seem complicated. Wait for momentum to build in one direction and get on the bandwagon. Expect to lose about two thirds of the time and so make sure your winners can pay for the losers and leave enough over to cover the rent. Of course there are a million different ways the details of this strategy can be varied, but most of them don’t make for any material difference. 

There are a few items that do make a real difference, however, and this is what you need to be very aware of. Instead of running thousands of simulations of different ways to measure a breakout or on variations of moving averages and so on, spending your time on the following items will prove a much more productive use of your time: 

• Diversification: How you choose to diversify is the single most important factor to influence the overall long-term results. Which instruments are included in the universe and the weighting of different sectors will have a massive impact. 

• Position sizing: Finding a way to properly calculate position sizes based on the volatility of each instrument is paramount, but the good news is that this does not have to be overly complicated. 

Time horizon: You need to decide what length of trends to follow: for example, if you want to be in the 1–2 week trends, 5–8 week trends and so on. At times this will make a substantial difference in performance. 

Risk level: There will always be a trade-off between risk and return and the higher risk you are willing to take, the more return you should be getting. Find a level both you and your investors can be comfortable with. 

Single or multiple strategy: Although long-term results tend to be similar, running the same strategy on multiple time frames or several similar trend-following strategies at the same time can help to smooth out volatility in the shorter term. 

## Investment universe

To achieve long-term success with a diversified futures strategy, you must cover multiple markets and multiple instruments per market. Running a trend-following strategy like these ones on a single market or a single asset class is at best plain silly and at worst suicidal. If you take these strategies and then go and trade only the Nasdaq 100 with it, don’t come blaming me when that margin call comes along. And when I say you need multiple markets, I don’t just mean that you need both the S&P 500 and the NDX. If you don’t include a large variety of futures markets in different asset classes, you should not do this in the first place. Sometimes there are several years in a row when a single market or even a whole asset class just keeps losing and losing, and then some years later that turns out to be the big winner. The whole point here is that you trade everything, even if you keep losing on some markets. As long as the winners pay for the 

losers, it is worth having these markets in for diversification. You never know when the market regime switches and the losing market becomes the winner. I cannot stress enough the importance of multiple markets. Using a single strategy on a single instrument is for people with either extreme skill or for those who simply have a death wish. 

There is often a trade-off between number of markets and complexity of the strategy. More markets can increase diversification and create more trading opportunities but adding too many will complicate your strategy and your operational side. The exact number you settle on should be a result of your own simulations and matching your risk acceptance. I will start out with a fairly broad universe in these simulations, although very good results can be achieved with fewer markets as well. 

For each of the sectors I mention in Chapter 2, I take ten instruments and include them in the initial investment universe for this chapter (see Table 3.3). It is no accident that I pick the same number in each sector. This is for demonstration purposes, to give each sector a theoretical equal chance at impacting our strategies so that we can fairly analyse sector attribution over time. In a real-life strategy, there is rarely good cause for equal-weighted universes like this, but it should help demonstrate some learning points and enable you to make intelligent decisions about your real investment universe later on. 


Table 3.3 Equal-weighted investment universe


<table><tr><td>Agricultural</td><td>Non-agricultural</td><td>Currencies</td><td>Equities</td><td>Rates</td></tr><tr><td>Cotton</td><td>Gasoil</td><td>AUD/USD</td><td>CAC 40</td><td>Bunt</td></tr><tr><td>Corn</td><td>Crude oil</td><td>GBP/USD</td><td>DAX</td><td>Schatz</td></tr><tr><td>Lumber</td><td>Heating oil</td><td>EUR/USD</td><td>FTSE 100</td><td>Long gilt</td></tr><tr><td>Live cattle</td><td>Natural gas (HH)</td><td>JPY/USD</td><td>HS China Enterprises</td><td>Canadian Bankers&#x27; Acceptance</td></tr><tr><td>Lean hogs</td><td>Gasoline</td><td>NZD/USD</td><td>Hang Seng</td><td>US 2-year note</td></tr><tr><td>Oats</td><td>Gold</td><td>EUR/CHF</td><td>Nasdaq 100</td><td>US 10-year note</td></tr><tr><td>Rough rice</td><td>Copper</td><td>EUR/GBP</td><td>Nikkei 225</td><td>Eurodollar</td></tr><tr><td>Soybeans</td><td>Palladium</td><td>EUR/JPY</td><td>S&amp;P 500</td><td>Euroswiss</td></tr><tr><td>Sugar</td><td>Platinum</td><td>CHF/USD</td><td>EuroStoxx 50</td><td>Euribor</td></tr><tr><td>Wheat</td><td>Silver</td><td>CAD/USD</td><td>Russell 2000</td><td>Short sterling</td></tr></table>

Why these particular markets? They are all highly liquid and easily tradable, but other than that they are fairly random. The typical trend-following futures fund would use around 100 different contracts and some make artificial markets by trading spreads between for instance gold and silver. 

I use daily data only, not just to simplify but also because you can successfully run these types of strategies without bothering with intraday data. Since this is futures data, you need to make sure that the data is properly adjusted, as I discuss in Chapter 2. Don’t skip or underestimate the importance of this detail. If your futures data is not properly adjusted you are simply wasting your time building strategies and will be wasting your money trading them later on. 

## Position sizing

Without a decent position-sizing formula it really does not matter how good the trading rules are. The instruments included in our portfolio above show very different volatility profiles, not to say extremely different volatility profiles. The term volatility is admittedly used loosely here and what we are concerned with is the potential price fluctuations of different instruments based on their recent past. 

Although the EuroStoxx 50 index can easily move 1–2% in a day and sometimes even 4–5% in a very eventful day, a move of just 0.5% in a day would be practically unheard of for Eurodollar. So if we were simply to put the same notional dollar amount in each trade, the portfolio would immediately be dominated by the volatile instruments and not much impact at all would come from the less volatile. This is not what we want to do, so instead we need to find ways to take the volatility of each instrument into account when deciding how many contracts to buy or sell in each market. There are several variations on how to do this: some prefer to base it on average true range, others on standard deviation and some may prefer to make their own formulas. In essence, the methodologies used by most CTAs are more or less the same, the principle being that you take larger sizes of less volatile instruments with the aim of having each position theoretically capable of making the same bottom line profit or loss impact on the overall strategy. 

For our strategies in this book I use a method based on so-called average true range, which has been widely known for a long time and used for at least four decades. It aims to measure how big a normal daily move is for each instrument and then use that as a basis for position sizes. The true range refers to the price span in which the instrument was traded for one day based on the high, low and close values. The formula for the true range for day t is: 

$$
T R _ {t} = \max (H, C _ {t - 1}) - \min (L, C _ {t - 1})
$$

The lowest price of today’s low and yesterday’s close is subtracted from the highest of today’s high and yesterday’s close, and we arrive at the range in which we have been trading for today. To get to the average true range (ATR), you just need to take an average of these numbers. I use an exponential moving average to arrive at the normal trading range for each instrument over time. You may see other smoothing methods for the ATR in other books, but it usually matters very little which one you use. 

The point with using the ATR as volatility estimation is that it provides not only a comparable number that we can use to standardise position sizes, but also an estimation of how large a move we can expect on any given normal day. We can use this information to set a target impact of the position on the portfolio as a whole. This target impact number will in turn act as a kind of leverage factor which could be scaled up or down to shift the risk level of the strategy up or down. 

For our initial strategies we use a risk factor of 20 basis points, so the theoretical average daily impact on the portfolio for each position should be 0.2%. Imagine the current portfolio as a whole is worth US$1 million. Since we want each position to have a theoretical impact of 20 basis points that translates to US$2,000. We get a buy signal in gold and the ATR of this instrument happens to be exactly US$10 at that time, and because we know that the Comex Gold contract has a point value of 100, each contract we buy has a theoretical impact of US$1,000. So we buy two of them. 

The reason I keep using the phrase ‘theoretical impact’ is that you must always be aware that volatility is not stationary and can change dramatically over the course of a position’s lifetime. This position-sizing method does not depend on a stationary volatility, it just uses the ATR at the time of position entry as a reasonable estimation of potential price moves. The position size is kept constant through the life of the position and not increased or reduced over time. The last part is something you may or may not want to tweak in your final strategy. 

The formula employed here is: 

$$
\text { Contracts } = \frac {0 . 0 0 2 \times \text { Equity }}{\left(\text { ATR } _ {1 0 0} \times \text { PointValue }\right)}
$$

Equity is the full value of the account being traded, or the amount of the account allocated to the strategy in question, and I discuss the ATR above (if you are not aware of what point value is, read up on it in Chapter 2). The denominator of this equation is the normal daily move in the instrument, should volatility remain on the same level. Note that if you are dealing with futures denominated in different currencies, this number must be converted to the same currency as the account equity; also remember that the point value is not always the same as the underlying amount of the contract. We can, of course, only buy whole contracts and not fractions of a contract, so the number is rounded down to make sure we err on the conservative side. 

The magic value here is the Figure 0.002, or 0.2%, which I refer to as our risk factor. This is a more or less arbitrary number and changing it can scale the risk of your strategy up or down very quickly. I suggest you experiment with the outcomes of simulations and find a risk factor that you are comfortable with. A lower number gives you lower returns and lower risk, while a higher number gives you higher risk and higher returns. 

I use the ATR method for position sizing because it is the simplest to explain and does the job well enough. There are several similar approaches possible, all striving to adjust the size of the position to the expected price moves of the instrument so that you get a common risk basis. Another popular method is to use standard deviation instead of ATR. Note that if you use this approach, you need to calculate the standard deviation of the daily returns and not on the prices themselves. 

Although I have always shied away from it myself, I know of futures hedge funds with excellent results that use only margin to equity as their position sizing and risk measurement. This is a different approach than using historical volatility estimations but aims to accomplish the same thing. The exchanges set the margins of each futures market based primarily on their view on volatility to minimise the risk of defaults by market participants. By trusting that the margins accurately reflect the risk of the instrument you could use this as a basis, for example always taking 0.5% margin to equity risk of each position, where equity represents your full account value. This method has always made me wary of the somewhat subjective part in the exchanges’ decisions for setting the margin and the history of sudden and unexpected changes in margin requirements in some markets. It is also tricky to simulate results back in time because it can be hard to get hold of accurate historical data for margin requirements. Still, there are large funds using this concept with very strong results and so I don’t write it off. 

## Slippage, commission and other costs

Underestimating the effect of costs is generally a bad idea. It makes your simulations look nice, but when the rubber meets the road you will feel the pain of the mistake. In this chapter I assume US$20 per futures contract round trip and market specific realistic slippage. It’s not a perfect estimation but it should be conservative enough to err on the side of caution. 

When you plan for your trading business you also need to count in your management fee, performance fee, custody fee, administration fee, auditor fee and whatever else you might need to load the fund or client accounts with. In order to show realistic numbers and not just some wishful thinking, I have taken these fees into account by assuming a 1.5% management fee, 0.5% for various fixed costs such as administration and custody, as well as a 15% performance fee. 

## Interest on liquidity

One unique feature of futures strategies compared with cash equities and similar is that they are not very cash intensive. These instruments allow for very high leverage and in theory you need only enough cash to cover the initial margins and make sure you don’t get killed by margin calls. That approach is more akin to gambling though and it is not how a professional CTA manager operates. In reality most CTAs have a huge amount of cash that is not needed as margin collateral for the near future. Keeping cash on the books is not desirable for many reasons, not least because it creates an unnecessary counter party risk against your prime broker while giving close to 0% interest rate. Should your broker default you will likely lose any cash that’s being held on your behalf, but securities are normally segregated and will be returned to you. 

The obvious solution to this problem is to buy sovereign government debt with the excess cash, because there is no point in taking additional risk by going to riskier debt instruments. Depending on the state of the interest rate curves in the world at any given time, this method is not only safer than cash but can also have a welcome contribution to the bottom line returns of the fund. At the time of writing, the interest income a CTA can earn from excess cash is negligible, but at other points in recent history this can be a significant performance contributor. 

The effect of the interest on excess cash holdings has been accounted for in all simulations in this book unless stated otherwise to provide as realistic results as possible. 

## Strategy personality

There is an old industry adage that the way to make money from the markets is to buy low and sell high. This is certainly not how trend-following futures traders operate and you need to get comfortable with a very different way of working. As a trend follower, you will be buying high and selling higher as well as selling low and buying back lower. You will often take positions that seem crazy, such as buying an instrument that already went up 20% in a month and just had a massive spike up, showing extreme overbought readings. When everyone else thinks something has gone so far that it just has to stop and reverse, that is often when you enter. 

Trend-following strategies look easy and highly profitable when you look at long-term return charts, but you need to study the shorter term down to daily variations and trades to be able to judge whether you can really follow the strategy in real life. It’s a matter of your own personality and whether you could and want to trade in the style that the strategy dictates, and the matter of how your clients will see the results. Many of these strategies have drawdowns of up to 30% and can sometimes take a year or more to recover. If you launch your trading product just before a larger drawdown occurs and you are sitting there half a year later trying to explain to a client why he still has a substantial loss on his investment, you might wish you had chosen a different strategy or a different risk level. But certainly, the more volatile strategies are also the most profitable in the long run and it’s all a matter of how much you and your clients can stomach. 

In Chapter 4 I describe two trend-following methodologies that are deliberately picked because of their simplicity and widespread usage. These strategies form a good starting point for getting familiar with the principles of trend-following futures trading and although they are profitable over time, I don’t recommend using them in their original form. Don’t worry though; I am not going to play the usual trick of describing simple models that cannot be used in real life. As the book progresses, we will improve upon these strategies and arrive at methods that are perfectly usable in a real-life hedge fund. 

## Anatomy of a trend-following strategy

The aim of trend-following strategies is to enter into a trend that is already under way and then stick with the trend until it makes a move against you and is likely to turn. That means that you are targeting the middle of a trend, deliberately forsaking the beginning and the end. The underlying principle involved here is that markets tend to move in extended trends. For the most part, any given instrument lacks a real trend to exploit and trend followers either stay out or keep losing over and over by trying to enter into potential new trends that don’t materialise. Any single instrument might stay in such a non-trending mode for a very long time, perhaps even years. It is therefore crucial that the serious trend-following trader systematically trades many different instruments in many different sectors. If your intention is to run these types of strategies on a single instrument or perhaps just a few of them, you might as well go buy a lottery ticket. 

Often books on this subject spend too much time talking about entry rules while often neglecting the really important aspects of a strategy. In reality, the buy and sell rules are far subordinate in importance to position sizing and diversification. Non-professionals tend to spend an excess of time and energy on the 

buy and sell rules and neglect the infinitely more important aspects of diversification and risk. For a trend following strategy, it is quite possible to have flawed entry and exit rules in combination with good diversification and risk rules and still be profitable, but the other way around is a recipe for disaster. 

Looking at classic futures trending systems, some of which have published or otherwise disclosed, there are two main methods commonly used by these traders. The first method is to buy positive breakouts and to short negative breakouts, which means you need to find a good way to define a breakout (see Figure 3.4). 


Figure 3.4 Buying positive breakout in rough rice


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/55907246388bcc415e70b95e2cf223dffb22fb9d438505378fabeb1478a28b8c.jpg)


The second main method is to use some classic trending indicator, such as a moving average, and enter on various crossover rules (see Figure 3.5). The simplest example would be to plot a moving average over a price chart and buy whenever the price crosses above it and short whenever the price crosses below. 


Figure 3.5 Reversing position on moving average cross in the Nasdaq


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/97b5f15e390659ee2df5b88f7acf5928291e0b1123534f3b545a2cdf2da93edd.jpg)


As stated, entry rules are the least important part of a trading strategy and accordingly you should spend the least amount of time on them. That does not mean they are irrelevant and should be skipped over, but the other components are very much more important to your actual trading results over time. 

Often a filter rule accompanies the trending rules, making sure that buys only occur when the market is in a bullish phase and vice versa for shorts. Many trend followers would want to avoid accidentally going against a strong trend just because there was a short-term counter move, and a good filter rule can help you with that. An easy method is to use two layers of trend measurement of different time horizon, such as a 200-day moving average for a long-term trend filter and a shorter moving average for trend-entry signals. Requiring both indicators to agree ensures that you only enter into trades in the direction of the longer term predominate trend. For the initial strategies presented in this section of the book, I don’t employ a trend filter. The point of doing so is just to keep the models as simple as possible for the first demonstration, and then I will add more features to them later to see how the results are impacted. 

4 

## Two Basic Trend-Following Strategies

Instead of lingering too long on the theoretical aspects of constructing trading strategies, in this chapter I use examples that you can replicate and test yourself, so that you can make up your own mind about what works and what does not. I start by introducing two very basic trend-following methods, which have been used at least since the 1970s and perhaps even earlier. These particular methods have been chosen for their simplicity and widespread use, in order to make a point. I intend to demonstrate that these very simple and well known strategies, even without any complex modifications, can achieve results comparable with many of the professional trend-following funds out there. I describe the details of these strategies along with a common position-sizing formula they both use as well as the diversification plan; then we can see how well these strategies perform over time and how they measure up against the competition in the hedge-fund world. 

The first strategy we investigate is a real classic and very easy to model and trade. The basis of the strategy is the moving average, that is, the average price for the past X number of days. In this variant of the strategy two moving averages are used with a different number of days used for the look-back period, so that we have one fast-moving average and one slow-moving average. To start off with, let’s use the fairly arbitrary values 10 for the fast-moving average and 100 for the slow-moving average (see Figure 4.1). Just how much these numbers matter is investigated later on in this chapter. 

Figure 4.1 Standard moving average crossover strategy 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/be153c91dc7c4b47eb8690ab54eb3891cb6e3fe5fef381ae07c3669612b887a4.jpg)


This strategy trades both on the long and short side of all instruments and it will always be in the market, which means that for each futures contract we include in the strategy universe we always have a position, long or short. As soon as we get a stop from the long strategy, we immediately open a short position and vice versa. No trend filter or similar is employed at this stage, so we simply follow the moving average cross signals as they come along. The strategy is being run on daily data and always trades the day after a signal. The last part is a safeguard to prevent so-called data snooping, a common mistake of modelling strategies that trade on data that may not be available in reality at the time of the trade. If a signal is generated on a Tuesday, the strategy simulation assumes that we buy on Wednesday morning and that we get a generally bad entry price with the slippage and commission assumptions mentioned in Chapter 3. 

The logic of the strategy is very simple. If the faster-moving average is above the slower-moving average that means that the trend of the instrument is up. Since the trend is up, we buy with the assumption that if the price moves against us we will get stopped out fairly soon with a small loss, whereas if the price continues up we have a theoretically unlimited upside. 

Our second strategy attempts to enter into new trends and stay with them as long as possible. The rules are again very simple: if today’s close is higher or equal to the highest close in the past 50 days, we buy tomorrow; if the close is below or equal to the lowest close for the past 50 days, we sell open tomorrow and go short. A similar logic is used to get out of positions, where a long trade is sold when the close reaches the lowest point in 25 days and a short trade is covered when the price makes a 25-day high (see Figure 4.2). Analytics is done on daily closing prices and trades are always taken one day after the signal. 

Figure 4.2 Standard breakout strategy 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/257e6ab9f68ce608171333f0ebdfb1dac0d599301c5cf60553d8246d2a52dfa7.jpg)



As opposed to the moving average cross strategy, the breakout strategy does not have to be in the market the whole time. After a position is stopped out, it can be out for some time before the next signal comes along.


## STRATEGY PERFORMANCE

It is important to view the performance of any strategy in the proper context. Simply looking at the compounded annual return number does not tell you much about whether the strategy is viable or not, or even whether it is better or worse than another strategy. To figure out which strategy is preferable over another, you need to look at various risk measurements but also study the equity curve of the strategy in detail to see whether it is something you can realistically live with or not. Some highly profitable strategies have very scary periods and if you cannot stomach them, you should find a different strategy that fits you and your investors. 

The equity curve in Figure 4.3 tells us that both strategies seem to be profitable over longer-time spans, but it is easy to fall into the trap of making premature assumptions. A simple visual inspection of such a longterm equity curve would not make it easy to judge whether the moving average strategy is in reality a better strategy than the breakout, for instance. In this time span you would have made more money with the former, but seeing which one would be better from a volatility adjusted point of view is not easy. Note that the y-axis uses a logarithmic scale to make the chart more readable. With the large percentage moves over time that we see here, a linear chart would just look plain silly, to use the technical term for it, and for that reason practically all charts in this book employ the same scale. 

Figure 4.3 Moving average and breakout strategies 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/b9c6480399b747383ff9ec99e7a41a46599209dbffe82e2be2190f05a4c7cb39.jpg)


To put the long-term performance of the basic strategies into context, I include four comparison items, or benchmarks if you will. The first is simply MSCI World, which is a common benchmark for world equity performance because it covers over a thousand stocks in many regions, and the second is Barclay BTOP 50, an index that seeks to replicate the overall composition of the managed-futures industry (see Figure 4.4). I also include (in Figure 4.5) the Millburn Diversified Futures Program and the Dunn World Monetary and Agricultural Program. Millburn is one of the pioneers in the business and it has been running a highly successful business since the 1970s, making it an excellent benchmark for performance. As with Millburn, Dunn is a very successful long-term performer and one of the legends of the business. These two funds are chosen to represent the industry because they both have long official track records available and show very respectable performance. 


Figure 4.4 Core strategies compared to benchmarks


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/7345ec2bf95af57d2d21af6f3cc94915b4c51e71b503b81277af5b0bd650f793.jpg)



Figure 4.5 Core strategies compared to cta funds


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/afd29349257ace5e702a2ce97ebc3c563747e88c0e2a8e55f1d67fe0e3ec6d88.jpg)


We can see from these figures and the summarised data in Table 4.1 that the most basic strategies, which have been published over and over again for decades, outperform traditional investments in a big way. Start by considering the long-term performance of equities. In the 22 years covered by the simulation, world equities had an annualised performance of 4.7%, which is barely above the so-called risk-free rate you could have received from the government. Still there is a perception among the public that equities always go up and that one always has to be invested in this asset class. For some periods in history this has been true, but for the past couple of decades things don’t look very good for stocks. If you invested US$100 at the start of January of 1990, you would now have a whopping US$276 after 22 years. Almost triple your money sounds good, right? Of course, you only need about 3.2% annual return to double your money in 22 years and around 5.1% to triple it. Also note that the worst loss the stock index suffered, measured from the high to the low, was 57.5%. So at one point you would have lost over half your money. There are plenty of severe drawdowns in recent history for the equity markets and the returns are not anywhere near enough to compensate for them. 


Table 4.1 Simple strategies compared to benchmarks and competition


<table><tr><td>All data from Jan 1990 to Dec 2011</td><td>MA Cross 10 × 100, 0.2% risk</td><td>Breakout 25 × 50, 0.2% risk</td><td>MSCI World total return (US$)</td><td>Barclay BTOP 50 index</td><td>Millburn Multi Market</td><td>Dunn Monetary and Agriculture</td></tr><tr><td>Compounded annual return</td><td>28.9%</td><td>19.4%</td><td>4.7%</td><td>7.3%</td><td>11.5%</td><td>15.9%</td></tr><tr><td>Worst drawdown</td><td>-48%</td><td>-32.2%</td><td>-57.5%</td><td>-13.3%</td><td>-22.8%</td><td>-60.3%</td></tr><tr><td>Drawdown/annualised return</td><td>-1.66</td><td>-1.66</td><td>-11.36</td><td>-1.81</td><td>-1.99</td><td>-3.78</td></tr><tr><td>Percentage profitable months</td><td>65%</td><td>60%</td><td>62%</td><td>60%</td><td>62%</td><td>58%</td></tr><tr><td>Best month</td><td>57.9%</td><td>56.8%</td><td>11.3%</td><td>10.6%</td><td>17.7%</td><td>31.2%</td></tr><tr><td>Worst month</td><td>-30.3%</td><td>-32.2%</td><td>-18.9%</td><td>-7.0%</td><td>-11.1%</td><td>-23.5%</td></tr><tr><td>Sharpe, RF: 2.5%</td><td>0.89</td><td>0.68</td><td>0.22</td><td>0.54</td><td>0.68</td><td>0.53</td></tr><tr><td>Sortino ratio</td><td>1.84</td><td>1.36</td><td>0.01</td><td>0.87</td><td>1.09</td><td>0.79</td></tr></table>

The astute reader might at this point ask about the dividends you would have received on the stocks if you bought and held the index constituents for this time, and whether this would not make up for the difference. 

The answer is simple; no. The MSCI World data I present here is the total return series, and so the dividend effect is already included. If not for the dividends, you would only have received 3.4% annua return. 

So let’s look at the second index, Barclay’s BTOP 50. This shows a very solid long-term performance, which speaks in favour of these types of strategies of course. It compounds at a respectable 7.3%, which would have made that same US$100 into almost US$500 in the same period. The worst drawdown suffered was a little over 13%, which seems quite reasonable given the annual return number. Keep in mind of course that this is an index consisting of the performance of many diversified futures traders and so the volatility is naturally lower than most of the individual constituents. Compare the return profile of the BTOP and the MSCI indices in Figure 4.4 and you can see that the managed-futures index provides a much smoother return, which remains stable through good and bad years for the stock market. It is not prone to the large declines as the equity index is. 

To compare against the big guys in the business, I include two managed-futures houses that have been around for decades and are highly respected in the business. Millburn had a compounded annualised return since inception of around 17% since 1977, which would make US$100 into US$23,000 and beat pretty much any benchmark you throw at it. Dunn has been around since 1984 and compounded around 15% since then. There are many top-notch trend-following managers out there, and we’ll look closer at them later on, but for now these two will have to represent the competition in our initial comparisons. For full disclosure, I don’t get paid, directly or indirectly, by any fund or similar to say nice things in this book. 

So, how did our two test strategies fare against the indices and the big competitors? The moving average strategy compounded at 28.9% with a worst drawdown of 48% and the breakout strategy yielded 19.4% annualised while having a max drawdown of 32.2%. Obviously our two strategies are more volatile than the benchmarks and show larger numbers for both return and risk. In the current shape they may seem a bit overly volatile but as long as the profits are strong in relation to the risk taken, there is no need for concern. The volatility level itself is not a problem, because it can be dialled back and forth very easily by modifying our position-sizing factor and thereby simultaneously decreasing risk and return at the same time. The details of how this works are explored in detail in Chapter 5. Therefore, the ratio between the two is of much more importance than the absolute return and drawdown numbers. 

A common way to compare strategies of different volatility is the Sharpe ratio. It is often seen as a universal way to rank strategies where you simply choose the one with the highest ratio. Before I explain why this is a bad idea, let me briefly explain what the Sharpe ratio is. The formula as such is quite simple: take the annualised historic return, deduct the so-called risk-free return and then divide the result by the standard deviation of the strategy’s return. 

The real problem with this ratio is in how it reacts to volatility. Since we have volatility, in the shape of standard deviation of the returns in the denominator, the formula is of the distinct opinion that volatility is always bad and should be severely punished. The core idea is not wrong and it is certainly better to have smooth returns than volatile returns, but the way in which the standard Sharpe ratio is calculated makes no real sense for evaluating different styles of trading. The standard deviation formula is based on a theoretical mean return and whenever actual returns are far away from this, the deviation rises and causes a negative impact on your Sharpe ratio. Note that the standard deviation treats both positive and negative deviation equally, so if your strategy has a very strong run up, such as occurred for most trend-following strategies during the second half of 2008, you may have excellent returns but your Sharpe might not look so great. 

Another reason why Sharpe ratio is a bad idea for our kind of strategies is that we are essentially dealing with highly leveraged trading. Exactly how leveraged we are is a matter of debate when you deal in crossasset strategies and many traditional measures of leverage may not make much sense in this context, but we are certainly leveraged. If you study the position-sizing formula presented earlier, you find that it has a key input number that can be raised and lowered depending on how large a position you want and by extension how much risk you want on your strategy. By lowering this number you get lower return numbers, lower drawdowns and lower standard deviation, and vice versa if you raise the number. You are still however deducting the same risk-free rate from your returns, and so if you lower your number you get a lower standard deviation but lose a much larger part of your return in the numerator of the Sharpe equation. 

What should matter is how much return you can make and what level of risk you need to take to get there. This is presumably what Sharpe originally intended, but I take issue with the way his formula defines risk in this context. 

Although far from perfect, the Sortino ratio can be more helpful than Sharpe for us. The principle for the Sortino ratio is the same as for the Sharpe ratio, but only downside volatility is measured so that a strategy is not punished for moves in the right direction. 

If we divide the worst drawdown by the annualised return we can get a feel for how big the largest drawdown really is in comparison to a normal year for the strategy. For both the moving average strategy and the breakout strategy, the maximum drawdown was 1.66 normal years, while MSCI World lost 11.36 years at the most. The BTOP 50 index had a drawdown of 1.81 years while Millburn and Dunn lost 1.99 years and 3.78 years respectively. How large a drawdown in relation to return you are willing to accept should be something you need to think over. Remember that even if your strategy is sound and will recover over time, you may lose your investors if you have too large drawdown in relation to your return profile. All the futures strategies here have reasonable numbers but giving up almost eleven and a half years’ performance on the equity markets seems a little steep. 

## Correlations between strategies

What we are looking at here are monthly return correlations; that is, how closely the returns of one strategy are related to another. Be careful when you calculate your correlations and avoid the rookie errors that are still so common. The most common mistake made by people not used to calculating correlations is to simply make a column in Excel with all the monthly returns, and then run the built-in Correl() function on it, which is likely to produce flawed data. Another mistake is to take price series, NAV of a fund, price of a futures contract and so on, and then use the same Correl() function, which would give you even worse nonsense data. The problem is not the aforementioned Excel function, which is perfectly usable for this purpose, but that you need to have the right input data. The proper way to do it is to run the correlation on the natural log returns, not on the percentage returns and definitely not on the price. 

To calculate the log returns, use the formula: 

$$
R _ {i} = L n \left(\frac {P _ {i}}{P _ {i - 1}}\right)
$$

where Pi is the price or value of your time series at point i in time, Pi–1 would then be the price of the same time series one day earlier and the resulting Ri is your natural log return for data point i. If you are using Excel to do this, just put all your time series price data in a row and make a row next to it where you use the built-in Ln() function to calculate a new column with all the log returns. Then use the Correl() function on two sets of log returns and you are done. 

The correlation coefficient itself will have a value between –1 and 1, which describes the nature of the relationship between the two series being compared. A value of 1 means that they are identical and move exactly the same, while –1 implies that they move exactly inversely to each other. Zero means that they are completely unrelated. 

The correlation matrix in Table 4.2 demonstrates a few interesting points. First note how our two initial trending strategies are very highly correlated: with an almost 0.9 correlation coefficient, the strategies are practically identical. This confirms that the exact buy and sell rules did not matter very much. The core concept remained the same and the portfolios will for most of the time have a very similar composition. The second interesting part is that our strategies are negatively correlated to the world index, but not strongly negatively correlated. This means that they would work well as a complement to an equity portfolio, because they have positive return expectations and negative correlation to the market that would both improve return and reduce risk if held as part of a portfolio of stocks. In fact, all the diversified futures strategies here, including the Barclay index, have a slight negative correlation to world equities The diversification effects of having vehicles in your portfolio that have a zero to slight negative correlation and still strong positive expectations can be huge. 


Table 4.2 Correlation comparison


<table><tr><td></td><td>MA Cross strategy</td><td>Breakout strategy</td><td>MSCI World total return</td><td>BTOP 50</td><td>Millburn Multi Market</td><td>Dunn Monetary and Agricultural</td></tr><tr><td>MA Cross strategy</td><td></td><td>0.89</td><td>-0.17</td><td>0.64</td><td>0.61</td><td>0.60</td></tr><tr><td>Breakout strategy</td><td>0.89</td><td></td><td>-0.23</td><td>0.66</td><td>0.63</td><td>0.59</td></tr><tr><td>MSCI World total return</td><td>-0.17</td><td>-0.23</td><td></td><td>-0.09</td><td>-0.01</td><td>-0.03</td></tr><tr><td>BTOP 50</td><td>0.64</td><td>0.66</td><td>-0.09</td><td></td><td>0.84</td><td>0.81</td></tr><tr><td>Millburn Multi Market</td><td>0.61</td><td>0.63</td><td>-0.01</td><td>0.84</td><td></td><td>0.71</td></tr><tr><td>Dunn Monetary and Agricultural</td><td>0.60</td><td>0.59</td><td>-0.03</td><td>0.81</td><td>0.71</td><td></td></tr></table>

Our correlation to the BTOP 50 index is high, but not extremely high. About 65% of our returns can be explained by this index, which may seem low but our current choice of risk level and asset universe likely differs from most funds and we are still using very basic strategies without any bells and whistles. Also note that the two competitors both have a very high correlation to the BTOP index as well as to each other. 

One major reason why our strategies don’t have a higher correlation to the big funds is the asset class mix. We allocate equally to the five sectors as defined above, which is not a common method in reality. For now we deal in an equal-weighted universe for educational purposes and we’ll switch to more realistic asset mixes later on. 

Having a small set of equal-weighted markets can be easy to do if you are small enough, whether it’s a good idea or not. But when you reach the size of these funds and have several billion dollars to manage on a highly leverage basis, there are many markets you simply cannot trade, at least not in a size that really matters. When liquidity becomes a real issue, funds tend to get more longer term in their trend analysis and they tend to increase allocation to currencies and rates where the liquidity is considerably higher than with commodities, as well as increasing the number of instruments in their universe greatly. There are, of course, highly liquid contracts in the commodity space as well, but you have far fewer to choose from. 

## Parameter stability

At this point, you might be thinking that I deliberately picked parameters for these strategies to make sure that they look good in the end. This is a reasonable assumption, and so let’s see if I can dispel it. I will now use the exact same strategies again, but make a shorter term and a longer term version of the same thing. For the moving average strategy that originally used 10 and 100 day analytics, I use 5 and 50 on the short term and 20 and 200 on the long term (see Figure 4.6). The breakout strategy’s original 25 and 50 days are supplemented with a 15/30 short term as well as a 50/100-day long-term iteration (see Figure 4.7). 


Figure 4.6 Parameter stability of moving average strategy


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/481fdaba856d55bd0b7a3193e2f821453a76141fac3db0dca2cfc937a86b77da.jpg)



Figure 4.7 Parameter stability of breakout strategy


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/7af88d9942bad72be1476ea5c5bce37f9ae2060ed53c4567e30460aeae238865.jpg)


Pure visual inspection of the comparison charts shows us that the return profiles look practically identical with the moving average strategy and quite close for the breakout strategy. For the latter, the longer-time horizon clearly does better than the shorter. In reality it makes quite a bit of difference over time depending on which one you pick, but all of these show significantly better return profiles than the equity markets and most of them could be used to manage money on a professional basis. They could, of course, be improved upon without too much effort, which I intend to demonstrate shortly, so don’t start trading just yet. 

Looking at Table 4.3 we can see that all the strategies have nice positive returns but the return number by itself means very little without putting it into a volatility context. The compound returns and the 

drawdowns vary with very similar amounts so there is no big change in the drawdown to annualised return ratio, with the exception of the short-term breakout strategy. Short-term strategies are often more tricky and usually require a little bit more sophistication on the risk side than the medium-term strategies because you have a greater risk of getting whipsawed in and out of positions. Still, the numbers even for the shortterm breakout strategy, which clearly is the worst performer in this comparison, are good enough to stand up to most benchmarks. 

## Table 4.3 Parameter stability comparison

<table><tr><td>All data from Jan 1990 to Dec 2011</td><td>MA Cross 10 × 100, 0.2%</td><td>MA Cross 5 × 50, 0.2%</td><td>MA Cross 20 × 200, 0.2%</td><td>Breakout 25 × 50, 0.2%</td><td>Breakout 15 × 30, 0.2%</td><td>Breakout 50 × 100, 0.2%</td></tr><tr><td>Compounded annual return</td><td>28.9%</td><td>22.2%</td><td>25.7%</td><td>19.4%</td><td>15.5%</td><td>25.0%</td></tr><tr><td>Worst drawdown</td><td>-48.0%</td><td>-40.8%</td><td>-33.6%</td><td>-32.2%</td><td>-38.9%</td><td>-36.4%</td></tr><tr><td>Drawdown/ annualised return</td><td>-1.66</td><td>-1.84</td><td>-1.31</td><td>-1.66</td><td>-2.51</td><td>-1.45</td></tr><tr><td>Percentage profitable months</td><td>65%</td><td>63%</td><td>58%</td><td>60%</td><td>60%</td><td>63%</td></tr><tr><td>Best month</td><td>57.9%</td><td>52.8%</td><td>50.1%</td><td>56.8%</td><td>53.1%</td><td>60.5%</td></tr><tr><td>Worst month</td><td>-30.3%</td><td>-20.2%</td><td>-23.5%</td><td>-21.6%</td><td>-16.2%</td><td>-25.9%</td></tr><tr><td>Sharpe, RF: 2.5%</td><td>0.89</td><td>0.72</td><td>0.86</td><td>0.68</td><td>0.59</td><td>0.81</td></tr><tr><td>Sortino ratio:</td><td>1.84</td><td>1.38</td><td>2.07</td><td>1.36</td><td>1.16</td><td>1.67</td></tr></table>

In some periods the returns are offset slightly and one time frame beats another, but over time we can see that all these iterations are viable and produce strong results. The time frame parameter would therefore seem fairly stable and although they would produce slightly different returns over time, there is no real firm answer as to which of them is the best going forward. 

## Conclusions from the basic strategies

What we have established so far in this chapter is that even the simplest trend-following strategies can perform remarkably well over time. The point of this exercise was to demonstrate that the choice of trendfollowing method is not as important at people seem to think. It helps to have good buy and sell rules, but you can still achieve very good results using the most basic methods available to the public for decades. The secret sauce is not in the buy and sell rules. 

## IMPROVING THE STRATEGIES

The two strategies used so far demonstrate that we can get very strong results from very simple strategies, but they could use some modifications to perform better. In this section I add a few simple but important features to our strategies and combine them into one single strategy, which we can use for further analysing the returns of diversified futures programmes. Let’s start by looking at the problems the current strategies have and how we can address them. 

Despite their apparent profitability, there are several problems with our initial strategies that need to be addressed. They both perform well enough over the long run, but show too high a volatility for most investors to bear and they result in many trades that are very difficult to deal with from a trader’s psychological perspective. The last bit may sound a bit odd, but it is a factor you should take into consideration before deciding on a trading strategy. As an example, if your strategy is profitable over the long run, but only wins on 30% of the trades and tends to get kicked in and out of positions each day, it will be very difficult to keep pulling the trigger and keep on trading. Most people would sooner or later start thinking that because 70% of all trades are losses, perhaps they will just skip one or two once in a while. If you then skip the one that was going to be profitable enough to pay for all the losers, your whole performance year may be ruined. It is quite normal for a diversified futures strategy to lose on 60% to 70% of all trades and that is one of the most difficult aspects of this trading style to deal with and the reason many traders start doubting their own strategy and end up overriding at the wrong time. 

We need to make our strategies a little less risky, easier to trade and hopefully a little more profitable as well. I will make it a point to keep our strategy simple but realistic. I am not going to add 10 different oscillators and some neural-network machine-learning doodads, just some small improvements that make the strategy a whole lot more viable in an institutional-trading environment. More complexity does not necessarily make a strategy better and it is my experience that simple trend-following strategies perform better in real life than those with highly complex maths and large numbers of rules. 

## Trend filter

Our two strategies each have a unique problem, and these are in fact quite related and can be addressed by the same means. The moving average strategy’s biggest problem is that it is always in the market, even if there is really no trend at the moment. When there is a sideways movement in the market, this strategy tends to enter and exit time after time, losing on each turn. This is not only unprofitable, but also highly annoying, demoralising and it makes little sense. Figure 4.8 shows this behaviour during a sideways phase of the mid-2000 in the S&P 500. What is missing here is some sort of trend filter to make sure that the strategy does not buy or sell when there is no trend available to profit from. 


Figure 4.8 Moving average strategy overtrading without trend filter


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/dadf79b8c925ecc7c7b8a49a3728c2bdbfa1a3e0aa9cde172aa6c0940a962491.jpg)


The breakout strategy does not have exactly the same problem, because it is not always in the market and only enters after a price breakout, but it does suffer from a similar symptom. Since the breakout will enter a long trade after seeing the highest price in a certain number of days and enter a short trade when a new low for the same number of days is made, it has a tendency to go against the main market trend at times. If there has been a very strong market trend for a while, it is not unusual to see a bit of a pullback. Such a pullback may for some strategies be a good place to take the profits and exit, but it is rarely a good point to enter a reverse position. 

Figure 4.9 shows the breakout strategy in a strongly trending period of the S&P 500 at the height of the dot com bubble. Two things should be clear just from a quick glance: the strategy enters into shorts in a strong bull market, which does not make sense, and it over-trades, taking too many positions back and forth in a strong trending market. 


Figure 4.9 Breakout strategy without trend filter


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/e014ecd4df80447b931e01c9a6bcb90c56fb2f8c189002fc97c8974695db5660.jpg)


The remedy for both these situations is to add a trend filter, which makes sure that we only trade in the direction of the main trend and that we don’t get whipsawed by going in and out of positions every couple of days. The moving average strategy does in fact make for a pretty good trend filter by itself, at least if we make it a little slower so that we can measure the direction of the medium-term trend with it. I stick to round and fairly arbitrary numbers to show that there is no optimisation or other shenanigans going on here. The concept is what matters rather than the exact details. 

Figure 4.10 shows crude oil during a bull market phase followed by a bear market phase. The method used to determine which market regime we are in is a combination of two moving average lines, where the solid line is the slower 100-days moving average and the lighter line is the faster-reacting 50 days. Here the moving average lines are not used for trading signals because it was in one of our initial strategies, but just as a filter to see what market direction is dominating. If we set a criterion for our strategy that we are only allowed to buy when the overall market is in an uptrend and vice versa, we are likely to get two effects: the number of trades is reduced and there is a higher percentage of winners. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/e16f368b826da7c10cf7ec05ccf34fafde5ab905ecc3f6fe09342eb655501e7f.jpg)



In Table 4.4 we can see that the standard breakout strategy has significantly improved by using a simple trend filter. The annualised returns are up while the maximum drawdown and volatility are down. The number of positive months increased and the worst month is not as bad as before. Most importantly, the maximum drawdown has decreased significantly. We now only have a maximum historic loss of 1.16 times an average year’s earnings and our simple strategy is starting to shape up quite a bit (see Figure 4.11).



Figure 4.11 Effect of trend filter


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/7890d195ce4e863afd9d2f54e0966078e3e9d9b6b6a8f009d17d1a4640a6302a.jpg)



Table 4.4 Adding trend filter


<table><tr><td>All data from Jan 1990 to Dec 2011</td><td>Breakout 25 × 50</td><td>Breakout with filter 25 × 50</td></tr><tr><td>Compounded annual return</td><td>19.4%</td><td>22.4%</td></tr><tr><td>Worst drawdown</td><td>-32.2%</td><td>-26.0%</td></tr><tr><td>Drawdown/annualised return</td><td>-1.66</td><td>-1.16</td></tr><tr><td>Percentage profitable months</td><td>60%</td><td>63%</td></tr><tr><td>Best month</td><td>56.8%</td><td>56.8%</td></tr><tr><td>Worst month</td><td>-21.6%</td><td>-18.6%</td></tr><tr><td>Sharpe, RF: 2.5%</td><td>0.68</td><td>0.80</td></tr><tr><td>Sortino ratio:</td><td>1.58</td><td>1.77</td></tr></table>

## An improved stop loss mechanism

Using the breakout method for entries and exits, we are left without detailed knowledge of how much each trade can cost us until we hit the stop point. Remember that the stop is triggered when the price makes a new 25-day low, and just how far down it is to making a new 25-day low can vary massively between different situations. One potential problem is when we have bought something that takes off in a very strong way, making a parabolic move to the upside. When this move turns back down, it is a very long drop down to making a new 25-day low and we risk giving up all our profits. On the other hand, if the trend levels out slowly and moves sideways for a couple of months, the distance to the stop would be very close. This method for stops can be psychologically difficult to follow because it would often mean giving up very large portions of your best positions before getting out. I prefer to add some more predictability to our stops. 

Remember how I used the average true range (ATR) method for position sizing in Chapter 3? Well, I am going to use the same concept for our stops and show how the position sizing and stops can work together to make our portfolio behaviour a little more predictable. To save you from flipping back and checking the formula, here it is again: 

$$
T R _ {t} = \max (H, C _ {t - 1}) - \min (L, C _ {t - 1})
$$

$$
A T R _ {t} = \frac {\sum_ {j = 0} ^ {n = 1} T R _ {t - j}}{n}
$$

$$
\text { Contracts } = \frac {0 . 0 0 2 \times \text { Equity }}{\left(\text { ATR } _ {1 0 0} \times \text { PointValue }\right)}
$$

As fun as equations can be, this is easier explained in plain text: 

• The true range is the daily trading range, or how many dollars the instrument moved in a particular day. 

• The average true range is an average of the true range over a set number of days, in our case 100 days. 

If we multiply the average true range by the point value of the futures contract in question, we get a figure for how much profit or loss to expect from a normal day’s intraday movements in that contract. 

Setting the risk factor to 0.002 means we are willing to get an impact of 0.2% on our portfolio, and so we need to multiply the risk factor with the portfolio value, or equity, to arrive at our desired daily impact in dollars. 

• Dividing this by the expected average impact of each contract gives us the number of contracts to buy, after rounding it down of course. 

It should be clear to any trader who deals in assets of varying volatility that setting stops in terms of percentage moves is a very bad idea. However, there is nothing to prevent us from using the ATR instead. This number is already adjusted for volatility, and so we can use it straight away. Let’s keep it simple, and set our stops trailing, always 3 ATR units away from the best point the position has seen since we opened it. So for long positions, the stop is always 3 ATR units down from the highest high since we bought and for shorts it is 3 units above the lowest low. 

The nice part here is that we know our theoretical maximum cost per position. With a risk unit of 0.2% per ATR unit and our stop 3 units away, the stop should cost us 60 basis points. Never forget however that volatility is not stationary and I will keep repeating that point because it is very important. The logic with the ATR units, as well as for any similar methodology, is just an estimation based on the recent past. In your simulations and planning, always take into account that volatility has a nasty tendency of changing in ways that end up hurting your bottom line. This is a decent approximation method but you should never relax and think that it is a sure thing. 

I will also not use intraday stops for this strategy, and so we always trade on the open the day after a signal. At times the price may drop very far through the stop point before the trade is closed the day after, and that is also something that needs to be taken into account. 

As Table 4.5 and Figure 4.12 show, the effect of adding these more realistic stop points is a decreased profitability but also a reduced risk. Some of the more extreme behaviour of the strategy during strong trending markets is lessened and we get a somewhat smoother ride. We are now down to a maximum historical drawdown of 20% on a strategy that yields 18% compounded, and that is something most professional investors can live with. 


Figure 4.12 Effect of stop technique


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/f019a8681e6a18dc34ce53cee33f7982f8cd21ec08318359ebcc3fe8a57e15c0.jpg)



Table 4.5 Volatility based stops


<table><tr><td>All data from Jan 1990 to Dec 2011</td><td>Breakout 25 × 50</td><td>Breakout with filter 25 × 50</td><td>Breakout with filter and ATR Stops 25 × 50, 0.2%</td></tr><tr><td>Compounded annual return</td><td>19.4%</td><td>22.4%</td><td>17.9%</td></tr><tr><td>Worst drawdown</td><td>-32.2%</td><td>-26.0%</td><td>-20.2%</td></tr><tr><td>Drawdown/annualised return</td><td>-1.66</td><td>-1.16</td><td>-1.13</td></tr><tr><td>Percentage profitable months</td><td>60%</td><td>63%</td><td>63%</td></tr><tr><td>Best month</td><td>56.8%</td><td>56.8%</td><td>41.3%</td></tr><tr><td>Worst month</td><td>-21.6%</td><td>-18.6%</td><td>-14.7%</td></tr><tr><td>Sharpe, RF: 2.5%</td><td>0.68</td><td>0.80</td><td>0.74</td></tr><tr><td>Sortino ratio</td><td>1.36</td><td>1.77</td><td>1.57</td></tr></table>

The year by year performance is shown in Figure 4.14 for comparison. Note that when the equity markets had a bad year the futures strategies tended to have very good years, but there are plenty of years where the equity markets did well and the futures also had a good run. 

Going back to our benchmark comparison, our new champion strategy is holding up quite well against the competition (see Figure 4.13). Comparing equity indices such as the MSCI World to diversified futures strategies is a bit like kicking a dead horse, but I do so anyhow to show just how far behind the traditional investment choice is. In comparison to our two legendary futures funds, Dunn and Millburn, is our strategy clearly better than theirs? No, not really. But on the other hand, their strategies are not clearly better than ours either. What should be very clear is that our simple strategy can stand up to the big boys of the business and produce very respectable volatility adjusted results. 


Figure 4.13 Comparing with the competition and benchmarks


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/7e206760ab2cff2d10f1700fd0b0667c5aca332c9a3fc64f15f82c125b9db1ca.jpg)



Figure 4.14 Year by year comparison


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/39c12474f004a1cf63eece09685e5472221c9b10293bf9eb5c9fd127bcdb043e.jpg)


One of the bigger problems left with our strategy is the tremendous performance seen in 2008, when it more than doubled the money. This may not seem like a problem at first glance, but the daily volatility the strategy experienced during the second half of that year was truly scary to go through and very few futures managers stuck to their guns and let the strategy run free. Whether the overriding that many did that year was prudent or not is hard to say even in hindsight. Those who overrode their strategies and decreased risk ended up making less money than they in theory should have, but they also reduced the risks of getting caught in a massive loss that could easily have happened with that unprecedented level of volatility that the markets were experiencing. Our strategy came out ahead in the end with very nice results, but at the expense of many sleepless nights for the manager. 

## Controlling the risk level

Perhaps you feel that the strategy I show here is too risky, or perhaps you feel that it does not yield high enough annual return numbers. There is a very easy solution to these concerns. Remember how we used a risk factor variable in our position-sizing formula? If you want to gear the risk level of the strategy up or down, all you need to do is to modify this input value. The risk factor governs how much each position, in theory, should affect the bottom line of the portfolio on a day to day basis and how much damage or profit the position can potentially do to the portfolio as a whole. 

In our original position-sizing formula, I used 0.2% as our risk factor, making each position in theory have a 0.2% bottom-line impact on our whole portfolio on an average day. We don’t change position sizes over time, but the risk changes naturally both by volatility contraction and expansion in the instrument itself or by large price moves. A commodity that is traded around US$100 and has an average true range of US$2 when we buy it is likely to have a very different average true range when we have held it for half a year and the price is now around US$200. Risk will naturally expand with success for long positions but the flipside of this is that the opposite can happen on the short side, as the position grows smaller with increasing success. 

The point is that since our position sizes and stop points depend completely upon this risk factor, toggling it up or down can have dramatic effects. Figure 4.15 shows the exact same strategy as before, but with four different risk factors. I keep the original 0.2% factor for comparison and add one higher risk iteration and two lower risk versions, of 0.25%, 0.15% and 0.1% respectively. 


Figure 4.15 Changing the risk level


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/fbf139ffd322f1b3dfd31d0b1e7ddc08fb035116c373d18553b260ecf0671253.jpg)


Note that the overall profile of the returns is pretty much the same, but the magnitude of the moves varies accordingly. There are many reasons why the 0.2% version is not simply double the return from the 0.1% version, and most of them are likely already clear to the reader. Management fee will be a constant percentage and performance fee impact will vary but most importantly is the effect of leverage itself, which can work some funny illusions at times. 

The common mistake when thinking about leverage strategies is that people miss the effect of the compounding. Consider a theoretical instrument with the monthly returns as shown in Table 4.6. If the percentage returns stay the same for the basic, unleveraged investment, the leveraged investment will behave quite differently and despite the leverage version having double risk from the standard, they can end up at very different numbers. 

## Table 4.6 Effect of leverage

<table><tr><td>Month</td><td>Monthly return (%)</td><td>Unleveraged</td><td>Double leveraged</td></tr><tr><td></td><td></td><td>100.0</td><td>100.0</td></tr><tr><td>January</td><td>-5</td><td>105.0</td><td>110.0</td></tr><tr><td>February</td><td>+5</td><td>99.8</td><td>99.0</td></tr><tr><td>March</td><td>+10</td><td>109.7</td><td>118.8</td></tr><tr><td>April</td><td>-10</td><td>98.75</td><td>95.0</td></tr></table>

Comparing the statistics for the four variations shown in Figure 4.15, we end up with Table 4.7. It shows just how easy it is to flip the risk level up or down on your strategy. 


Table 4.7 Comparing strategy iterations


<table><tr><td>All data from Jan 1990 to Dec 2011</td><td>Breakout with filter and ATR stops <eq>{25} \times {50}</eq> 0.2%</td><td>Breakout with filter and ATR stops <eq>{25} \times {50}</eq> 0.15%</td><td>Breakout with filter and ATR stops <eq>{25} \times {50}</eq> 0.10%</td><td>Breakout with filter and ATR stops <eq>{25} \times {50}</eq> 0.25%</td></tr><tr><td>Compounded annual return</td><td>17.9%</td><td>13.7%</td><td>9.4%</td><td>22.0%</td></tr><tr><td>Worst drawdown</td><td>-20.2%</td><td>-15.6%</td><td>-10.8%</td><td>-24.5%</td></tr><tr><td>Drawdown/ annualised return</td><td>-1.13</td><td>-1.14</td><td>-1.15</td><td>-1.11</td></tr><tr><td>Percentage profitable months</td><td>63%</td><td>63%</td><td>63%</td><td>63%</td></tr><tr><td>Best month</td><td>41.3%</td><td>30.0%</td><td>19.4%</td><td>53.4%</td></tr><tr><td>Worst month</td><td>-14.7%</td><td>-11.1%</td><td>-7.5%</td><td>-18.2%</td></tr><tr><td>Sharpe, RF: 2.5%</td><td>0.74</td><td>0.71</td><td>0.64</td><td>0.76</td></tr><tr><td>Sortino ratio</td><td>1.57</td><td>1.48</td><td>1.25</td><td>1.61</td></tr></table>

Armed with these variations, you can choose your risk level and which of our benchmarks you want to compete with. If you prefer to play things safe and try to more or less opt for the low volatility of the BTOP 50 index, your best bet is the 0.1% risk version. That risk level was a good fit for the BTOP 50 index throughout the 1990s, although in the past decade it would seem as if the volatility of the index has gone down even further, along with its returns of course (see Figure 4.16). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/e1952cd9ad3c398467db2fdf756870c353afa718e1dea37860a376f414433f1b.jpg)


Figure 4.17 is a year by year comparison of the results of the 0.1% version of our strategy to that of the BTOP 50 index. What we see here is that in most years the results are pretty close but we do have some larger divergences. In 1994 our strategy took a beating while the benchmark index was hugging the zero line and in 1996 and 1997 we lost to the benchmark, although gained in absolute terms. 1998 to 2001 showed quite large outperformance and it is clear that the volatility of the index went down while the strategy volatility went up. The massive difference however is in 2008 when our strategy more than doubled the return of the index. I dig into this exceptional year in detail in Chapter 6, but the main effect comes from the fact that our strategy lets profits run wild and does not take money off the table until the signal comes to close the trade. In a year with such extreme trends as 2008, most futures managers overrode their strategies and decreased risk as volatility of their strategies rose to unprecedented levels. This was likely a good business decision to make, for reasons I demonstrate in Chapter 6, but it did hurt their end of year absolute performance figure. The same way, it is likely that many managers manually decreased risk during 1994 when their performance started to suffer. 


Figure 4.17 Year by year comparison of core strategy with 0.1% risk to BTOP 50


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/350bb0abba9554958306ecfa0262e7cd9801cfc88797c023445236af27706764.jpg)


If you prefer to take on a bit more risk to get to the really juicy returns, by all means go for the 0.25% version (see Figure 4.18). This higher risk iteration tracked our two benchmark funds quite closely for some time, but lately it has started outperforming more and more. This is only natural because as these funds grow larger they are unable to take the same amount of risk as previously and many less liquid markets become closed to them. Multi-billion dollar futures funds cannot place bets in smaller commodity markets of any size that would be meaningful, because these markets are not liquid enough to handle the kind of money these funds need to invest. 


Figure 4.18 Comparison of core strategy with 0.25% risk and two large futures funds


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/d849bf441d6cd0b3c7efb4245d0ec46802e136a75228dff3087e1ea268d9a706.jpg)



Could you argue that our simulated returns are highly unrealistic for that same reason, that if you get these types of returns in a real fund, there will be so much assets coming into the fund that you are finally unable to continue to produce such high return numbers? Absolutely, but if you find yourself managing a US$5 billion futures fund, your biggest concern in life is no longer achieving 25% compound return figures! In Tables 4.8 and 4.9 you can also compare the results of our four iterations to those of the benchmarks used earlier.


Table 4.8 Yearly returns for core strategy and benchmarks (%) 

<table><tr><td></td><td>Core strategy, 0.1%</td><td>Core strategy, 0.15%</td><td>Core strategy, 0.2%</td><td>Core strategy, 0.25%</td><td>MSCI World</td><td>BTOP 50</td><td>Millburn</td><td>Dunn</td></tr><tr><td>1990</td><td>15.9</td><td>22.7</td><td>29.6</td><td>36.7</td><td>-18.7</td><td>15.2</td><td>50.4</td><td>51.6</td></tr><tr><td>1991</td><td>12.7</td><td>18.2</td><td>23.8</td><td>29.3</td><td>16.0</td><td>14.7</td><td>8.2</td><td>16.9</td></tr><tr><td>1992</td><td>3.2</td><td>4.6</td><td>6.0</td><td>7.3</td><td>-7.1</td><td>2.5</td><td>18.7</td><td>-21.8</td></tr><tr><td>1993</td><td>17.1</td><td>26.4</td><td>36.3</td><td>46.9</td><td>20.4</td><td>13.4</td><td>12.1</td><td>60.2</td></tr><tr><td>1994</td><td>-7.4</td><td>-11.5</td><td>-15.4</td><td>-19.2</td><td>3.4</td><td>-0.2</td><td>11.7</td><td>-19.3</td></tr><tr><td>1995</td><td>15.0</td><td>21.9</td><td>28.8</td><td>35.7</td><td>18.7</td><td>14.0</td><td>30.3</td><td>98.7</td></tr><tr><td>1996</td><td>10.9</td><td>15.7</td><td>20.6</td><td>25.5</td><td>11.7</td><td>12.9</td><td>19.0</td><td>58.2</td></tr><tr><td>1997</td><td>5.1</td><td>6.6</td><td>8.0</td><td>9.2</td><td>14.2</td><td>12.0</td><td>14.9</td><td>44.6</td></tr><tr><td>1998</td><td>22.2</td><td>33.7</td><td>46.2</td><td>59.6</td><td>22.8</td><td>12.4</td><td>8.4</td><td>13.7</td></tr><tr><td>1999</td><td>4.6</td><td>6.0</td><td>7.3</td><td>8.4</td><td>25.3</td><td>1.6</td><td>0.4</td><td>13.3</td></tr><tr><td>2000</td><td>8.3</td><td>11.3</td><td>14.2</td><td>17.0</td><td>-13.0</td><td>6.6</td><td>14.4</td><td>13.1</td></tr><tr><td>2001</td><td>18.2</td><td>27.2</td><td>36.2</td><td>45.2</td><td>-16.8</td><td>3.8</td><td>-3.8</td><td>1.1</td></tr><tr><td>2002</td><td>13.5</td><td>20.5</td><td>27.4</td><td>34.2</td><td>-19.4</td><td>13.7</td><td>24.9</td><td>54.0</td></tr><tr><td>2003</td><td>13.2</td><td>20.8</td><td>28.7</td><td>37.0</td><td>33.7</td><td>15.5</td><td>4.0</td><td>-13.4</td></tr><tr><td>2004</td><td>1.4</td><td>2.3</td><td>3.1</td><td>3.7</td><td>15.2</td><td>0.9</td><td>-0.4</td><td>-16.7</td></tr><tr><td>2005</td><td>2.7</td><td>3.7</td><td>4.6</td><td>5.4</td><td>10.0</td><td>2.4</td><td>6.2</td><td>-16.4</td></tr><tr><td>2006</td><td>10.9</td><td>15.7</td><td>20.5</td><td>25.3</td><td>20.6</td><td>5.6</td><td>9.2</td><td>3.1</td></tr><tr><td>2007</td><td>5.6</td><td>7.3</td><td>8.6</td><td>9.5</td><td>9.6</td><td>7.6</td><td>14.4</td><td>7.6</td></tr><tr><td>2008</td><td>45.6</td><td>73.5</td><td>104.9</td><td>140.1</td><td>-40.4</td><td>13.6</td><td>22.4</td><td>51.4</td></tr><tr><td>2009</td><td>-3.9</td><td>-5.6</td><td>-7.5</td><td>-9.7</td><td>30.7</td><td>-4.8</td><td>-7.4</td><td>-0.6</td></tr><tr><td>2010</td><td>6.3</td><td>10.3</td><td>14.3</td><td>18.4</td><td>12.3</td><td>6.4</td><td>12.6</td><td>30.7</td></tr><tr><td>2011</td><td>-4.0</td><td>-5.3</td><td>-7.0</td><td>-8.8</td><td>-4.9</td><td>-4.3</td><td>-3.5</td><td>6.4</td></tr></table>


Table 4.9 Monthly returns, core strategy 0.2% 


<table><tr><td></td><td>Jan (%)</td><td>Feb (%)</td><td>Mar (%)</td><td>Apr (%)</td><td>May (%)</td><td>Jun (%)</td><td>Jul (%)</td><td>Aug (%)</td><td>Sep (%)</td><td>Oct (%)</td><td>Nov (%)</td><td>Dec (%)</td><td>Year (%)</td></tr><tr><td>1990</td><td>-1.6</td><td>2.5</td><td>7.6</td><td>5.6</td><td>-6.5</td><td>3.4</td><td>6.2</td><td>9.6</td><td>6.3</td><td>-8.3</td><td>1.4</td><td>1.5</td><td>29.58</td></tr><tr><td>1991</td><td>0.7</td><td>1.1</td><td>0.6</td><td>-4.6</td><td>1.1</td><td>0.1</td><td>-3.3</td><td>1.1</td><td>3.9</td><td>4.3</td><td>1.2</td><td>16.8</td><td>23.78</td></tr><tr><td>1992</td><td>-4.9</td><td>1.6</td><td>0.3</td><td>-2.4</td><td>4.3</td><td>1.5</td><td>7.2</td><td>6.0</td><td>-6.0</td><td>-3.4</td><td>2.7</td><td>-0.2</td><td>5.96</td></tr><tr><td>1993</td><td>1.6</td><td>9.9</td><td>0.6</td><td>-0.2</td><td>2.9</td><td>0.2</td><td>5.1</td><td>-2.7</td><td>-5.4</td><td>5.2</td><td>2.1</td><td>13.4</td><td>36.35</td></tr><tr><td>1994</td><td>-6.7</td><td>-5.0</td><td>5.1</td><td>-2.6</td><td>4.1</td><td>-1.4</td><td>-3.2</td><td>-4.2</td><td>0.4</td><td>-4.0</td><td>6.1</td><td>-4.2</td><td>-15.41</td></tr><tr><td>1995</td><td>-1.3</td><td>2.5</td><td>9.2</td><td>1.2</td><td>5.9</td><td>-1.1</td><td>-2.6</td><td>-3.0</td><td>2.0</td><td>-1.2</td><td>1.5</td><td>13.8</td><td>28.76</td></tr><tr><td>1996</td><td>-0.7</td><td>-8.3</td><td>5.9</td><td>10.0</td><td>-3.2</td><td>2.0</td><td>-6.6</td><td>3.3</td><td>7.9</td><td>7.6</td><td>10.2</td><td>-6.6</td><td>20.57</td></tr><tr><td>1997</td><td>9.2</td><td>2.8</td><td>-3.7</td><td>-5.0</td><td>-2.6</td><td>-0.4</td><td>11.4</td><td>-11.0</td><td>-0.2</td><td>-2.6</td><td>1.8</td><td>10.5</td><td>7.98</td></tr><tr><td>1998</td><td>0.7</td><td>5.7</td><td>2.5</td><td>-1.4</td><td>4.8</td><td>2.2</td><td>5.2</td><td>15.4</td><td>-0.5</td><td>-0.9</td><td>2.1</td><td>3.6</td><td>46.19</td></tr><tr><td>1999</td><td>2.1</td><td>3.2</td><td>-5.1</td><td>2.2</td><td>-8.3</td><td>4.4</td><td>2.4</td><td>0.5</td><td>1.5</td><td>-10.4</td><td>6.8</td><td>9.5</td><td>7.28</td></tr><tr><td>2000</td><td>-7.2</td><td>3.7</td><td>-7.8</td><td>3.3</td><td>4.4</td><td>2.9</td><td>-0.3</td><td>8.0</td><td>-4.1</td><td>-2.7</td><td>2.8</td><td>12.4</td><td>14.19</td></tr><tr><td>2001</td><td>-0.1</td><td>0.8</td><td>13.3</td><td>-11.6</td><td>2.2</td><td>-1.3</td><td>0.5</td><td>6.3</td><td>22.1</td><td>6.8</td><td>-4.2</td><td>0.3</td><td>36.19</td></tr><tr><td>2002</td><td>-4.8</td><td>-1.0</td><td>-4.2</td><td>-2.6</td><td>7.2</td><td>11.1</td><td>11.9</td><td>3.1</td><td>8.1</td><td>-9.6</td><td>-1.0</td><td>9.1</td><td>27.40</td></tr><tr><td>2003</td><td>8.6</td><td>7.3</td><td>-7.4</td><td>8.4</td><td>6.6</td><td>-6.0</td><td>4.5</td><td>3.0</td><td>-3.9</td><td>3.1</td><td>-4.7</td><td>7.9</td><td>28.72</td></tr><tr><td>2004</td><td>3.2</td><td>10.4</td><td>1.3</td><td>-9.1</td><td>-4.4</td><td>-3.0</td><td>-0.5</td><td>-4.8</td><td>1.3</td><td>1.5</td><td>9.8</td><td>-0.8</td><td>3.11</td></tr><tr><td>2005</td><td>-4.4</td><td>0.3</td><td>-4.0</td><td>-2.3</td><td>1.1</td><td>2.3</td><td>2.4</td><td>-0.8</td><td>-1.1</td><td>2.1</td><td>10.1</td><td>-0.4</td><td>4.57</td></tr><tr><td>2006</td><td>9.1</td><td>-4.2</td><td>9.7</td><td>7.3</td><td>-6.6</td><td>-3.7</td><td>-4.5</td><td>3.8</td><td>-0.8</td><td>5.8</td><td>3.1</td><td>1.4</td><td>20.49</td></tr><tr><td>2007</td><td>2.4</td><td>-9.1</td><td>-3.0</td><td>7.7</td><td>10.6</td><td>6.1</td><td>-8.0</td><td>-7.0</td><td>8.2</td><td>7.4</td><td>-3.7</td><td>-0.7</td><td>8.57</td></tr><tr><td>2008</td><td>8.9</td><td>22.4</td><td>-5.1</td><td>-3.1</td><td>5.6</td><td>2.6</td><td>-11.7</td><td>0.5</td><td>5.9</td><td>41.3</td><td>6.6</td><td>9.0</td><td>104.91</td></tr><tr><td>2009</td><td>-2.1</td><td>0.7</td><td>-11.1</td><td>-2.5</td><td>4.5</td><td>-4.4</td><td>3.0</td><td>4.8</td><td>3.3</td><td>-3.4</td><td>7.7</td><td>-6.7</td><td>-7.52</td></tr><tr><td>2010</td><td>-3.4</td><td>1.7</td><td>3.6</td><td>1.4</td><td>-3.3</td><td>0.7</td><td>-5.3</td><td>2.3</td><td>3.4</td><td>10.6</td><td>-3.1</td><td>6.0</td><td>14.28</td></tr><tr><td>2011</td><td>-1.1</td><td>3.2</td><td>-2.7</td><td>9.9</td><td>-9.1</td><td>-4.6</td><td>2.8</td><td>11.1</td><td>5.0</td><td>-14.7</td><td>-3.5</td><td>-0.6</td><td>-6.97</td></tr></table>


Parameter stability check


As we now have a slightly different strategy than the previous ones, it may be worth doing a sanity check on the base parameter, in this case the number of days used for the breakout logic. Since the strategy uses 50 days at the moment, let’s do a quick check to see whether it performs more or less the same using 25 days and 100 days. One might wonder why I don’t just run an optimisation and pick the perfect number, but it is the wrong question to ask. Optimisations are plain and simple evil and out to kill you, and if you ever catch one stomp on it hard and make sure it does not get away. There is no need to use the optimisation features built into your off-the-shelf software; in fact, there are many reasons why it can be really harmful and lull you into a false sense of security while only serving to curve-fit historical data with little to no bearing on reality. 

It is, however, sensible to make a few similar iterations of your strategy with the key parameters changed up and down a bit, just to make sure the results show up as would be expected. That does not mean that the annualised return should be the same, just that the overall concept should still work. If it does not, you need to ask yourself why that is, and decide whether there is a good reason why your strategy does not work on other time frames and so on or whether your first iteration was just a curve fit that is useless in real life. 

In Table 4.10 we see the result of a quick parameter stability check, using our original 50-day strategy compared to 25- and 100-day iterations. The shorter-term breakout strategy shows higher yearly results but at the cost of deeper drawdowns and higher volatility. They are quite similar in terms of winning versus losing months, skew and other parameters. Looking at the drawdown to annualised return, you end up with 1.37 years for the 25-day iteration, 1.13 years for the original 50-day version and 1.06 years again for 100 days. 

<table><tr><td>All data from Jan 1990 to Dec 2011</td><td>Breakout with filter and ATR stops 50 days</td><td>Breakout with filter and ATR stops 25 days</td><td>Breakout with filter and ATR stops 100 days</td></tr><tr><td>Compounded annual return</td><td>17.9%</td><td>21.5%</td><td>17.7%</td></tr><tr><td>Worst drawdown</td><td>-20.2%</td><td>-29.3%</td><td>-18.8%</td></tr><tr><td>Drawdown/annualised return</td><td>-1.13</td><td>-1.37</td><td>-1.06</td></tr><tr><td>Percentage profitable months</td><td>63%</td><td>62%</td><td>64%</td></tr><tr><td>Best month</td><td>41.3%</td><td>41.6%</td><td>41.0%</td></tr><tr><td>Worst month</td><td>-14.7%</td><td>-15.7%</td><td>-14.6%</td></tr><tr><td>Sharpe, RF: 2.5%</td><td>0.74</td><td>0.85</td><td>0.76</td></tr><tr><td>Sortino ratio:</td><td>1.57</td><td>1.93</td><td>1.61</td></tr></table>


The conclusion is that although the 25-day iteration is a little more volatile, the concept is stable across all three time frames and our strategy thereby holds up to the test (see Figure 4.19). 



Figure 4.19 Core strategy parameter stability


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/025888f4563738c9d64254c75061612c7d6755d7e08a89771834fe3fc76ab9a3.jpg)


## A solid foundation for futures trading

The strategy you have in front of you now is solid, realistic and fully usable for institutional money management. For my investors and myself I use several systematic trading strategies, and though none are identical to this one, some are close enough. If you are serious about trading a strategy like this, you now need to do the hard work of making the strategy your own. Get the software and the data, code the strategies described here and test them hard. Review the small details and make your own modifications to get the strategy to behave the way it fits your own style. If you are not intimately familiar with the strategy you trade, you always end up second guessing it and probably overriding it at the worst possible moment. 

## Core strategy rules

Let’s review the rules of the strategy we now have before us. This is still a fairly simple breakout strategy with only a few bells and whistles added on top of it but used correctly it works very well: 

• Long entries are only allowed if the 50-day moving average is above the 100-day moving average. 

• Short entries are only allowed if the 50-day moving average is below the 100-day moving average. 

• If today’s closing price is the highest close in the past 50 days, we buy. 

• If today’s closing price is the lowest close in the past 50 days, we sell. 

• Position sizing is volatility adjusted according to the ATR-based formula previously shown, with a risk factor of 20 basis points. 

• A long position is closed when it has moved three ATR units down from its highest closing price since the position was opened. 

• A short position is closed when it has moved three ATR units up from its lowest closing price since the position was opened. 

• The investment universe consists of five sectors with 10 markets in each. 

## 5

## In-Depth Analysis of Trend-Following Performance

This chapter uses the core strategy outlined in Chapter 4 to conduct an in-depth analysis into where the profit and loss in this type of strategy comes from. I dig deeper into sector attribution and long versus short attribution and explain the consequences of the resulting analysis. 

## STRATEGY BEHAVIOUR

The strategy we now have in our hands seems to perform quite well over time, but before trading real money you need to be fully aware of how the strategy makes, and loses, money. To manage such a strategy you need to be very familiar with its characteristics before launching or else you will certainly get cold feet at the first sign of trouble and start overriding the rules. Too many strategy developers rely only on the overview statistics generated by their back-testing software to understand the strategy behaviour, and therefore I go in much deeper and show year by year how the sausage is really made. The statistics from your average back-testing software have their value too, at least some of them, but they only tell a very small part of the story. I start by giving you some general statistics on this strategy and then take a look at the real details. 

The average holding period for a position is six weeks and four days where profitable trades average ten weeks and three days holding and the losing trades only two weeks. This is not so strange because winning trades are held onto for as long as they are not giving back too much profit, while the losing trades tend to be cut out quite fast. An average holding period of around six to seven weeks is a fairly common mediumterm trend-following time horizon. Note also that I don’t count rollovers as new positions but rather the same as the already held position. On average, about three trades per week are generated with this strategy, again not counting rolls. 

The strategy wins on 42% of all trades and thereby, of course, loses on the remaining 58%. If you have not been trading trend-following strategies it may sound odd that you are losing over half of the time, but I assure you that this is completely normal. I have seen very profitable trend-following strategies that lose on over 70% of all trades and the reason is, of course, that the winners on average gain much more than the losers lose. It is not easy to keep taking all new trade signals when you know that the trade you are 

entering will most likely fail and this is one of the toughest parts of trading trend-following futures strategies. 

The histogram of the trade result distribution in Figure 5.1 helps paint a clearer picture. You can see that the highest frequency outcome is a loss of between 0.5% and 0.75% on the portfolio and that makes a lot of sense. The theoretical stop point is at 60 basis points loss and with the added slippage and gaps that may occur many losses were even larger than this, which is to be expected. Out of all trades, 40% end up in the region between –0.25% and +0.25% and a whopping 70% end up between –0.5% and +0.5%, telling us that most trades are just not moving very much. That’s okay though, given the overall distribution properties. The term ‘fat tails’ is often used with a negative connotation in finance, often referring to the propensity of the market to experience negative outliers; or in plain English, to hit you with unexpected losses that no normal distribution shape could have predicted. In this case though, the fat tails work in your favour and that is the real beauty of the diversified trend-following approach. 


Figure 5.1 Distribution of trade results


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/726022128decaaba0d7f69c2ee027bd121e13d8c47c55c6821b80d59e6790f59.jpg)


The distribution diagram for the trades has quite a high positive skew of 2.1. This means that the overall tilt of the distribution is heavily to the right. There are no trades in our 22-year simulation that lost more than 2%, but 15 trades by themselves yielded 5% or more. The important part is that while an overwhelming majority of all trades end up as either small losses or small gains, some 5–10% of your trades are home-runs that generate big profits. 

The maximum number of winning trades in a row was 14 and after such a good run you will feel pretty good with yourself. But then again, after the maximum number of losses in a row that totalled 24 you will feel ready to switch career after that hit, at least if you were not previously aware that this can happen with this strategy. 

I could tell you more standard statistics that are normally displayed in the back-testing software packages but frankly I feel that most of it is of little value in general and for this type of strategy in particular. If I were to tell you that the average loss is 2.93%, it does not say anything useful because a 2.93% loss on palladium has a very different impact to a 2.93% loss in the Bund and percentages in this context only serve to obfuscate reality. It is an infinitely more enlightening process to break up the equity curve into sectors, longs, shorts and any other way that might make sense for a particular strategy and then go over it with a huge metaphorical magnifying glass to study carefully the details of the performance attribution. Only in this way can you learn about the personality of a trading strategy before you put real money at risk. 

# AS A COMPLEMENT TO AN EQUITY PORTFOLIO

Most investors, institutional as well as individual, prefer to hold a large part of their money in the equities market, that is, they want to be long stocks for the long term. I attribute this attitude mostly to the indoctrination from schools and governments about the conventional wisdom that ‘the equity markets always go up in the long run’, which in a manner of speaking is absolutely true. Of course, as John Maynard Keynes astutely pointed out, ‘in the long run we are all dead’. I showed earlier how in the 22- year time span covered by the strategy analyses in this book starting in 1990 and ending in 2011, the MSCI World Total Return Index yielded 4.7% annual compounded return and had a maximum drawdown of 57.5%. So if you happen to buy at the peak just before that drawdown, you can expect over a decade to recover your initial investment. To add insult to injury, if you had your money invested with an indexed mutual fund, you would with overwhelming probability end up with an even lower annual return while you pay the bank to keep underperforming. 

Now, before I get beaten over the head with a stick for writing off a whole asset class, let me explain my position a bit further. I have nothing against stocks and in fact I trade several profitable stock strategies and even some that are long only. My objection is only to the standard approach to the stock market of buying a basket of stocks, most likely whatever happens to be in a specific index, and just holding it for year after year. This is indeed a very risky strategy which can easily be seen from the numbers just mentioned, but the marketing effort of certain universities, governments and banks has been massively successful and people seem quite content to get their 4–5% return for taking the risk of losing over half their assets. There are many viable strategies for participating in the long-term bull markets in equities, which tend to be very profitable when they come along, but simply buying and sitting on stocks for decades does not make much sense to me. Still, many investors like doing this and so let’s have a closer look at how their overall returns can be improved by holding part of their money in the equities market and part of it in a strategy such as the ones I discuss in this book. 

The question that we need to ask here, and which ultimately we would like our potential investors to ask themselves, is ‘can a standard long only equity portfolio be improved by adding managed futures to the mix?’. This problem could be approached from a strict Markowitz methodology of building covariance matrices, Lagrange multipliers and other equally fun things to arrive at an exact optimal asset mix to the tenth decimal, but frankly I find this a waste of everyone’s time including the valued reader of this book. There are many interesting concepts coming out of Modern Portfolio Theory, but the vast majority of the methods have absolutely no bearing on reality and should probably not be used very much outside of classrooms. 

Still, the core concept of the Efficient Frontier is reasonably valid, even though some assumptions and methods surrounding it may not be, so I’m going to make a very simplified variant just to prove my point regarding diversification. In the following analysis, I have two assets to choose from: one is our core trendfollowing futures strategy, using equal weighted sectors, 20 basis points risk factor and including all costs; and the other is the MSCI World Total Return Index net of dividends. The question is how much we should buy of each to get the best volatility adjusted results for the overall portfolio. 

To test this I have made nine different mixes of these two assets with 10% increments, as well as the two alternatives of keeping all the assets in either strategy. The rebalancing is done monthly to make sure that the much higher long-term yield of the futures strategy does not result in an overwhelming amount of the assets in that strategy after a good period. 

We already know that the futures strategy has a much higher expected return, so there is no surprise that the highest returns are achieved with a maximum allocation to futures, but that is not what we are looking for here. Figure 5.2 shows the equivalent of a so-called efficient frontier for the two assets in our portfolio, with annual compound return on the y-axis and standard deviation, as a proxy of risk, on the x-axis. The idea is simple; we want to achieve as high an annual return as possible at the expense of as low a volatility as we can. The volatility is essentially the currency in which we pay for returns. 


Figure 5.2 Diversified futures as an enhancement to an equity portfolio


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/9e2c570894faac77b241933fe90e7bd5a7561da9005f0b6e88a77329ed12dbcc.jpg)



Figure 5.2 tells us right away that if we start with a portfolio of only the stock index and keep gradually adding allocation to the futures strategy, we get a lower and lower standard deviation while at the same time the annual compound return rises. The obvious conclusion from a quick inspection of this chart is that it does not make sense to have less than 30–40% futures and the remaining part in equities, because anything less means a lower return at a higher or equal risk level.


Table 5.1 shows the same data as in Figure 5.2 but it also has an additional column with the maximum drawdown numbers for each point in the curve. Even though 100% allocation to the futures gives the best overall return, the drawdown of the portfolio can actually be reduced by adding stocks to the mix. 


Table 5.1 Adding diversified futures to an equity portfolio


<table><tr><td>Percentage futures</td><td>Standard deviation (%)</td><td>Annual return (%)</td><td>Max drawdown (%)</td></tr><tr><td>0</td><td>4.5</td><td>4.0</td><td>55.4</td></tr><tr><td>10</td><td>4.0</td><td>5.7</td><td>46.5</td></tr><tr><td>20</td><td>3.6</td><td>7.5</td><td>36.4</td></tr><tr><td>30</td><td>3.4</td><td>9.1</td><td>26.3</td></tr><tr><td>40</td><td>3.4</td><td>10.7</td><td>16.7</td></tr><tr><td>50</td><td>3.6</td><td>12.2</td><td>12.8</td></tr><tr><td>60</td><td>4.0</td><td>13.7</td><td>14.8</td></tr><tr><td>70</td><td>4.5</td><td>15.0</td><td>16.7</td></tr><tr><td>80</td><td>5.1</td><td>16.3</td><td>18.5</td></tr><tr><td>90</td><td>5.7</td><td>17.5</td><td>20.4</td></tr><tr><td>100</td><td>6.4</td><td>18.7</td><td>22.2</td></tr></table>

Naturally, in a real world scenario you have more than two assets to choose from and there are other reallife complications as well, which makes it tricky to determine an exact optimal amount to buy of each asset class. Therefore, view this as a guideline approach and a way of demonstrating a concept more than exact numbers. 

# TRADING DIRECTION

The strategy we have arrived at is direction agnostic, using symmetrical rules for longs and shorts both in terms of entry and exit and in position sizing. So far we have only looked at the overview aggregated results and they seem to hold up well against the benchmarks, but we have not dug into the details of performance attribution yet. The first part we need to look into is how the long and the short side fare against each other and whether there are any differences between the two. For those who previously have not done these simulations themselves, the result of such an investigation may be a bit of a shocker. My recommendations on how to handle that result may be even more surprising. 

The short side of trend-following strategies is quite a problem to deal with and it requires some counter intuitive thinking to tackle. To start by demonstrating the problem, I present in Table 5.2 the results of using the same core strategy that we have arrived at so far when trading both sides, taking only the long trades and taking only the short trades. 


Table 5.2 Long versus short


<table><tr><td>All data from Jan 1990 to Dec 2011</td><td>Breakout with filter and ATR stops 50 days – long and short</td><td>Breakout with filter and ATR stops 50 days – just long</td><td>Breakout with filter and ATR stops 50 days – just short</td></tr><tr><td>Compounded annual return</td><td>17.9%</td><td>15.5%</td><td>2.5%</td></tr><tr><td>Worst drawdown</td><td>-20.2%</td><td>-14.7%</td><td>-32.4%</td></tr><tr><td>Drawdown/ annualised return</td><td>-1.13</td><td>-0.95</td><td>-12.9</td></tr><tr><td>Percentage profitable months</td><td>63%</td><td>59%</td><td>49%</td></tr><tr><td>Best month</td><td>41.3%</td><td>24.2%</td><td>31.6%</td></tr><tr><td>Worst month</td><td>-14.7%</td><td>-10.0%</td><td>-12.1%</td></tr><tr><td>Sharpe, RF: 2.5%</td><td>0.74</td><td>0.78</td><td>0.06</td></tr><tr><td>Sortino ratio</td><td>1.57</td><td>1.74</td><td>-0.61</td></tr></table>

The compound return on the short side of 2.5% is not a typo. Neither is the almost 13 years of maximum drawdown in relation to compound return. This tells us that the short side of the strategy, at least as a stand-alone strategy, looks quite abysmal. If we wanted to risk a drawdown of 13 years performance, we might as well go with the buy and hold equity strategy, right? One thing is certain; trading the short side only is a very bad idea. It may seem as if the obvious conclusion is to trade only the long side, but things are not as simple as they seem here. For the long only version, you would have made a return of 15.5% for a maximum drawdown of 14.7%, making for the best drawdown to return ratio we have seen so far. Looking at standard optimisation techniques, it would appear as if the long only strategy is the most desirable, with higher Sharpe ratio, higher Sortino ratio and so on. But standard optimisation techniques more often than not lead to strategies that fail in reality, so don’t stop analysing the results just because a couple of ratios ended up marginally higher. 

Looking at Figure 5.3 shows that the long only version moves up in a reasonable smooth pattern, trailing behind the long and short combined but showing solid results. The short only strategy has an odder pattern and does not move up anywhere near as much as the long version. This distinction is not the important piece of information, however, which comes when you compare the results of the short only strategy to 

that of the MSCI World Index. Note that when the world equity markets suffer, the short side of the strategy tends to do very well. Don’t underestimate the value of this effect. During equity bear markets very few strategies do well and the help that the short side of this strategy can provide during these times makes a big difference. Even more importantly though, during the times of serious market distress, when things are getting really scary for most market participants and there are few places to hide, the short side of the strategy tends to spike up and show excellent profits. It is not necessarily short equity index futures that yield the big profits in these bearish years, it may also be short energies and similar. The rather extreme performance of trend-following futures in 2008 was in a large part accomplished by the short side and those managers who had chosen to forgo the shorts only had long rates left to save the year. 


Figure 5.3 Comparing long versus short


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/9c4bf38999acb09468d111a9a9bdc1a5bcd7d4c8bb2ee324229355e1c0cf5c9b.jpg)


It is tempting for a strategy developer to follow the easy path and just ‘optimise’ the short side away. It looks like a no-brainer, giving higher volatility adjusted ratios, decreasing trading and lowering overall exposure. Still, you should take some more time to think through whether you do want to cut out the short side: it may make your strategy less competitive and may create some major problems for you in the case of a volatile financial environment. 

The reason it may decrease the competitiveness of your strategy is simple. The more you lean towards long only, even if you still trade all asset classes, the higher the correlation is to the world stock markets. One of the core benefits of managed futures is the ability to decouple from the stock markets and make money in up and down years, regardless of the equity crowd’s mood swings. To be an attractive complement to the ubiquitous equity portfolio, our managed futures strategy should have clear positive expected returns while having low to slightly negative correlations to the world stock markets. If we can achieve that, there are great diversification gains for a stock market investor to buy our product and that is a key sales argument. The reason is that with low or negative correlation along with positive returns we would push the investor’s overall portfolio to a more attractive point on the efficient frontier curve. 

The symmetrical long/short trend strategy we have used so far fulfils this requirement. The long only version does show nice yearly returns at attractively small drawdowns, but the correlation against the stock markets has changed for the worse. The original symmetrical strategy had a negative correlation of –0.16 but once the short side was excluded the correlation went up to +0.18. This may not sound like much but it can have quite a large impact on how your portfolio performs in relation to the world equities, and thereby to most other strategies. Having a positive correlation to the equity markets makes your product less 

desirable as a diversified for someone who already owns an equity portfolio, and let’s face it, most people own an equity portfolio. 

Figure 5.4 shows the same efficient frontier curve as in the earlier Figure 5.2, along with the new efficient frontier after we exclude the short side of the futures strategy (in grey). Note that the whole curve shifts to the right. For each point of annualised return on the y-axis, we now have to pay more in terms of higher volatility. The point of this analysis is naturally to find out how we can get the highest possible return at the lowest possible volatility and with that perspective it makes little sense to exclude the short side. 


Figure 5.4 Efficient frontier shift with long only futures


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/b53994b35c9e78b3edb0c8a65bea8486f0b099d2dc46f9e3422c241a94d9231a.jpg)


## SECTOR IMPACT

When doing the attribution calculations in this section, I ignore the effects of management fees and performance fees, because it would make little sense in breaking it down on the sectors. The information we are looking for here is the relative performance of the subcomponents of our strategy and for this purpose the fund fees are not terribly helpful. I use the same core strategy as before, with a 0.2% risk factor as per our original strategy. We know already that this basic strategy can produce pretty good return numbers, but so far we don’t really know where they come from. That is what we aim to uncover in this section. 

Table 5.3 shows yearly average returns for the different sectors, breaking down the long and short attribution. Note that these are average returns before fees and therefore slightly higher than the compound returns after all fees. The table tells us that over the long run the rates sector has been by far the most profitable sector. This is in no way an indication that rates will continue to be the most profitable sector going forward, or even that it will stay profitable at all. The long rates have been the big contributors simply because we have had a period of several decades of falling yields and thereby raising bond prices. Given the yield levels in most of the developed world at the moment, there are likely to be limited possibilities in long rates for a while. After all, bond yields are not likely to move south of zero. 

Table 5.3 Sector comparison – arithmetic average yearly returns before tees 

<table><tr><td></td><td>All sectors (%)</td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td></tr><tr><td>Long</td><td>18.8</td><td>2.8</td><td>2.6</td><td>2.2</td><td>2.2</td><td>8.9</td></tr><tr><td>Short</td><td>3.9</td><td>0.7</td><td>2.4</td><td>1.3</td><td>-0.2</td><td>-0.3</td></tr><tr><td>Total</td><td>22.7</td><td>3.5</td><td>5.1</td><td>3.5</td><td>2.0</td><td>8.6</td></tr></table>

Both the commodity buckets do well over time, gaining fairly evenly on longs and shorts. As usual we see a little less gain on the short side but that is quite normal for trending strategies. The currencies show an even higher tilt towards the long side although the short side still makes a small contribution. 

It may seem surprising that the equity futures are making so little compared to the rest and that in fact we are losing money over time on the short equity futures. Equities used to be much easier for these types of strategies a decade or two ago and one can only speculate about what, if anything, made the equity markets change and become more erratic and less prone to sustained trending. What comes to mind of course would be not only the increased amount of electronic trading and high frequency algorithmic trading, but also the increasingly globalised world in which all equity futures across the world tend to see a remarkably high level of correlation to each other. In particular when the markets are experiencing high levels of fear, such as the crises during 2000, 2008 and 2011, the correlation between indices with seemingly very different sector or geographic compositions quickly approaches one. High correlation between instruments in our investment universe is undesirable and although it sometimes means quick profits, it more often than not means sudden and simultaneous reversals in a large number of positions, causing painful losses in a very short time. 

As usual the yearly charts get distorted by the outsized returns in 2008 but try to look beyond that. The extreme profitability, along with the equally extreme volatility that year seem to be somewhat of an anomaly and not very likely to be repeated anytime soon. Still, these figures with the average sector returns for the strategy, along with the long and short side should help clarify where the profits and losses come from. 

The long and the short side of our strategy tend to behave quite differently, with the long side showing a smoother upwards profile and the short side a more dynamic burst-style return. The short side is far less profitable and in fact often ends up losing money for extended periods of time; but it still adds value by acting as a volatility stabiliser as well as providing substantial gain in extreme market situations. The trading results for each direction vary a great deal from sector to sector, and so it is important to look into the details of how each sector tends to behave on the long and the short side. 

Looking at the combined long and short results in Figure 5.5, the following can be observed: 

Figure 5.5 Average sector contribution per year 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/a7416ba4d2c7b90f220e4181f18ebce1bfe3340c40170a02feefd6aff5d46246.jpg)


• Rates show an overwhelming amount of positive years and quite a few outsized returns on the positive side. 

• Equities have a mediocre showing with many years near zero or negative and it also displays a few large negative years. The most eye catching year for equities should be 2008, which I will return to later. 

• Non-agricultural commodities had one extremely bad year but otherwise it performed fine. It also had an outsized performance in 2008. 

• Agricultural commodities sector is nearly always positive and it has several large positive return years while showing no significant negative years. 

• Currencies rarely makes big waves and has about half of the years in the black, but tends to win more on good years than it loses in bad years. 

In Figure 5.6, you see the profit and loss from just the long side of the trades, displayed in the same manner as in Figure 5.5. The sum of each bar therefore adds up to the yearly contribution of all long trades for all sectors in the strategy, which may be higher or lower than the total return on the strategy depending on how the short side performs the same year. The most important point to notice here is how this graph differs from the previous one. 

Figure 5.6 Average sector contribution, long side 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/d24ef860899744873c36d2dc0c7139f021b7b121a2fb0a78c87dda39ee8b0719.jpg)



Here is what stands out:


The overwhelmingly large positive returns of the long rates sector. It is positive a little more than half of the years, but the good years are a great deal larger than the bad ones. Many years are completely dominated by the long rates returns. 

• Long only equities look slightly better, with a few more positive years and a little larger gains but it is still not a major contributor to long-term profit and loss. 

• The long side of non-agricultural commodities keeps ticking in profits, slowly but surely. The contributions are not huge, but they are fairly steady. 

• Long agricultural commodities shows an even more steady smooth profile than the non-agricultural commodities, with almost no real loss year to speak of. 

• The long currencies, which may seem like an oxymoron, is not showing anything significantly different than in the combined long and short chart in Figure 5.5. 

Finally we have the short only numbers in Figure 5.7, otherwise composed in the same manner as those above. The first thing that should hit you when you see this chart is how relatively small most bars are and how many of them are negative: 

Figure 5.7 Average sector contribution, short side 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/4819b4c141a0cf3286aefe119183d8b8f23f69fa18f51824ad32b9bbe408a357.jpg)


• For short rates, almost no year has a significant positive impact on the portfolio. 

Short equities lose on a majority of the years although they have a large positive impact during the dot com crash of 2001. The shocker to the observant reader should be that short equities had a negative performance in 2008. 

• The non-agricultural short trades have a much smaller percentage of profitable years, but the profit years are generally larger than the loss years. 

• Agricultural commodity shorts have several large positive return years and only three negative years large enough to speak of. 

• Currencies again perform quite similarly on the long and short side, if you can even speak of a long and short side for this asset class. 

To paint a much clearer picture of what happened throughout this period, we need to go even deeper. We need to look at year by year to see how the profit and loss was really generated so that you get a feeling for what it is like to operate a diversified trend-following strategy in real life, and that is exactly what I do in Chapter 6. 

## CASH MANAGEMENT AND THE EFFECT OF FREE GOVERNMENT MONEY

Keep in mind that when we are dealing in futures we don’t need to pay cash for our positions the way that you normally would when buying stocks. All we need is to have enough cash on the books to cover the initial margin and enough to avoid risking margin calls in case the position goes against us. If the only position in the portfolio happens to be 10 contracts of wheat and the position was just opened at a price of 800 cents per bushel, we do in fact have a nominal exposure of US$400,000 worth of this particular grain, but that does not mean we need to have anywhere near as much money in our account. Exactly how much we need to hold in cash will vary based on the margin requirements on this commodity, which is set by the exchange where it is traded. 

At the time of writing, the initial margin per wheat contract is about US$3,000, and so we would at least need to have US$30,000 to cover the 10 contracts just bought. The wheat contract has a maintenance margin of about US$2,250 at this time, which means that we need to make sure that there is at least that much cash per contract available on our account at all times, after any unrealised losses. If the price now drops to 780 cents we have an unrealised loss on the position of US$1,000 per contract, given that the 

point value is US$5,000 and that the price quote is in cents. That means we just lost US$10,000 on the account on our 10 contracts and if we only have the minimum required US$30,000 on the account, we now get a margin call, because the cash on the account is not enough for the minimum US$2,250 per contract maintenance margin. 

The margin call requires us to top up the account to US$30,000 or the position will be forcefully shut down. A margin call is not something that you want happening to you and proper cash management will prevent that from ruining your day. Don’t ever put yourself in a situation where you may receive an unexpected margin call. Keep enough cash on the account to cover even quite large swings against you. 

If you have a mandate or fund denominated in US dollars and you only trade on American exchanges, the cash situation is very straightforward. Of course, for most of us this is just not the case and you are likely to find yourself involved in five to ten currencies depending on how many countries you want to trade in. You then face the added practical task of making sure each current account is properly funded as well as managing the currency exposure that this may entail. 

But then again, no one is saying that you should keep all your cash laying around on some brokerage account. This is both a waste of money and an unnecessary risk. The risk here can be summarised in a single word: Lehman. Although that unfortunate investment bank was the most spectacular, the same thing has happened to many others before and after. Many otherwise successful futures trading houses got burned in a big way on the MF Global implosion and there are no reasons to believe that these large blowups were the only ones masking horribly irresponsible companies behind smoke and mirrors. More spectacular failures of banks and brokerage houses are likely to come and it is not easy to predict who they will be. 

If you hold stocks or bonds with a bank or broker when it suddenly goes bankrupt it will be a messy and painful experience, but you and your investors will most likely get the stocks and bonds back in the end, because they are held directly under the account holder’s name. When it comes to cash, however, the story is quite different. I am sure that if you have made it this far you are already quite aware of how fractional reserve banking works and why the money you think you have in your bank is not actually there. The details of this system and its merits and hazards are not a topic in this book, but the short and simplified story is that all cash coming into a bank goes into the same big old pile of money as everyone else’s, to be lent out to people who go and buy things from people who put the money back into the bank to be lent out again. 

Imagine that you find US$1,000 hidden in a mattress and you go to your local bank and deposit it to your savings account. The bank then keeps a fraction of that money in the bank, as required by law, and lends the rest out to someone. Now assume it lends out US$900 of your money to someone who goes to buy a used car. The person who sells the car deposits the money in his savings account at the same bank and all of a sudden there is US$1,900 in the bank, while the bank is just in the middle of lending out another US$1,710 to start the cycle again. If we for ease of calculation assume that the bank needs to hold a 10% reserve on deposits, your US$1,000 adds US$10,000 to the monetary system by the magic of banking. 

In the end, everyone thinks that they have money in the bank but it’s all the same money, and the illusion only works until everyone wants to get their money out at the same time. This of course never happens, unless the bank is about to go bankrupt or there is a perception that the bank might go bankrupt, in which case it becomes a self-fulfilling prophecy. What you need to understand about this is just that cash held with a bank is not secure and will be exposed to counter party risk against said bank. If the bank goes belly-up, you will probably lose all your cash. Still, you do need some cash on the books and a reasonable amount of counter party risk is the cost of doing business, but you should pick your broker well and not keep too much cash lying around for no reason. 

A second reason not to keep all the money lying around in cash is that you receive little to no interest on it. Granted that as of writing this in 2012 the government yields are on a level where the interest income is almost insignificant, but at least you still get a little bit of free money while at the same time reducing risks. The core strategy described in this book normally operates at between 10% to 20% margin to equity ratio, so we have quite large amounts of money that will never be used. For a US$10 million fund running this strategy, you can easily keep US$6 million in government debt securities and probably even more. 

Exactly how you keep this excess cash is something you need to think through and plan. I recommend sticking only to government debt with top tier countries, preferably in your base currency, because it is not worth increasing risk to get a few extra basis points from lesser creditors. If you place the money only with the government who controls your fund’s base currency, or in the case of the Euro the most trusted of the member nations, your risk level is almost nonexistent. Regardless of the state of a nation’s economy, a G7 nation will pay back debts in its own currency, because they own the printing presses. The exception is of course the Eurozone, but the strongest nations are still considered quite safe. 

It is practical to pick a mix of varying durations to have different dates of expiry and keep rolling. Holding some in shorter-term papers and the bulk in 1–3 year securities is a common practice. Over time, the effect of proper cash management can be quite large, or at least it has been in the past. 

I am sure by now that many readers have been wondering why I have barely mentioned the effects of interest income up until now. This is after all a huge factor for managed-futures returns and it can have an extremely large impact on overall results. Well, the reason is that this has been a major factor in the past but there is nothing to indicate that it will remain an important factor in the future, at least not anywhere near as important as it was in the 1980s and 1990s. The truth is that a significant part of the returns from many managed-futures strategies in the past 30 years has simply been free money from the government and this is a phenomenon we need to explore further. 

Let’s go back to our core strategy and look at the difference in returns if we keep all excess funds in cash versus allocating it sensibly to government securities. I make the simplified but reasonable assumption that on average we have 65% of the asset base in US debt instruments with an average duration of two years. 

As Table 5.4 shows, the effect of the interest on excess cash has gradually decreased and is currently (in 2012) very low. The impact of this factor is going down because yields across the board have been decreasing for decades. There are two sides of that coin: on the one hand we get less risk-free return on our excess cash, but at the same time the strategy has been long bond futures the whole time and making a killing on the same falling yields. 

## Table 5.4 Effect of interest on free cash

<table><tr><td></td><td>Without interest (%)</td><td>With interest (%)</td><td>Impact (%)</td></tr><tr><td>1990</td><td>30.4</td><td>37.1</td><td>6.6</td></tr><tr><td>1991</td><td>25.6</td><td>30.2</td><td>4.6</td></tr><tr><td>1992</td><td>6.3</td><td>9.1</td><td>2.7</td></tr><tr><td>1993</td><td>42.5</td><td>45.2</td><td>2.7</td></tr><tr><td>1994</td><td>-16.5</td><td>-13.5</td><td>2.9</td></tr><tr><td>1995</td><td>28.1</td><td>32.9</td><td>4.8</td></tr><tr><td>1996</td><td>22.2</td><td>26.4</td><td>4.2</td></tr><tr><td>1997</td><td>7.4</td><td>11.5</td><td>4.1</td></tr><tr><td>1998</td><td>51.9</td><td>56.8</td><td>4.9</td></tr><tr><td>1999</td><td>6.8</td><td>10.6</td><td>3.8</td></tr><tr><td>2000</td><td>14.0</td><td>18.8</td><td>4.8</td></tr><tr><td>2001</td><td>41.8</td><td>45.0</td><td>3.1</td></tr><tr><td>2002</td><td>33.1</td><td>34.6</td><td>1.4</td></tr><tr><td>2003</td><td>35.2</td><td>36.2</td><td>1.0</td></tr><tr><td>2004</td><td>4.6</td><td>5.7</td><td>1.1</td></tr><tr><td>2005</td><td>5.0</td><td>7.4</td><td>2.5</td></tr><tr><td>2006</td><td>22.3</td><td>26.3</td><td>4.0</td></tr><tr><td>2007</td><td>8.4</td><td>12.2</td><td>3.8</td></tr><tr><td>2008</td><td>123.9</td><td>126.7</td><td>2.9</td></tr><tr><td>2009</td><td>-5.8</td><td>-5.5</td><td>0.2</td></tr><tr><td>2010</td><td>17.4</td><td>17.6</td><td>0.2</td></tr><tr><td>2011</td><td>-5.1</td><td>-5</td><td>0.2</td></tr></table>

The 1980s and 1990s were truly the golden years for a futures manager, where you could get 5% or more absolutely free, and still get a performance fee on it. Even though this extra side income is essentially free money from the government, the futures manager still gets paid for it. Always keep this in mind when analysing a futures manager’s long-term track record. A significant factor in the diminishing returns we have been seeing for the managed-futures industry is of course related to the low interest rate environment and it should be expected that results looked better a decade or two ago. 

Even without the impact of the interest income the returns of trend-following futures have been quite attractive over the long run, showing a more healthy returnto risk ratio than most traditional investment strategies such as mutual funds. Looking another decade back, into the 1980s, the interest income effect was much greater still. In such an environment managing futures is very much easier than it is in the current climate. Just consider the seemingly odd situation of a futures manager who ended a year like 1985 flat, making or losing nothing on the trading, but gaining 7% on holding US government debt for the lion share of the account. He would then be paid a performance fee on this 7%, despite a failed trading year. Don’t expect this easy-money environment to come back anytime soon. Odds are that interests will stay low for some time and competition in our field will only increase. 

## PUTTING LEVERAGE INTO CONTEXT

That trend-following futures trading need to be leveraged is hardly a shocking revelation, but you may perhaps wonder just how leveraged we have to be. Both mainstream and financial media like to use leverage terminology to make a point about how risky a fund or other investment is and you often hear outsized numbers about how leveraged traders are. The problem is that leverage and risk are two completely different concepts and they are not necessarily related. A higher leverage could mean higher risk but it by no means has to imply this. Of course, if you only hold one asset such as stocks in IBM, then your risk is double if you have US$100,000 exposure compared to having US$50,000 exposure, but when dealing with derivatives and cross-asset instruments the picture is not that simple. 

To put leverage into proper context and perspective, let’s take a look at a typical portfolio for our core strategy. If you have an account size of about US$5 million and trade the core strategy with a risk factor of 0.2% as described above, your portfolio would hold 19 positions covering all sectors on 21 May 2009. This date is chosen rather arbitrarily, and for the point I am making here pretty much any randomly chosen date would be just fine. Let’s start with the funny number and then I demonstrate why this seemingly ridiculous number is of little to no value to us: the portfolio value is as stated US$5,000,000 and our total notional exposure is US$55,300,000. We are not 100% exposed, or 150% exposed, but rather 1,100%: 11 to 1 leverage. This is a rather typical portfolio but at times the exposure can be more than double this. Crazy, you say? 

Table 5.5 has the full portfolio for the date in question with all positions, sectors, exact number of contracts held, how long they have been held and so on. You can also see the portfolio impact, that is, the profit or loss on the position in terms of effect on the overall portfolio. The exposure is the face value of the contracts, and so just the number of contracts multiplied by the contract size and price and then translated to US dollars. The exposure is also shown as a percentage of the total portfolio value. The final field is the cost to the stop, that is, how much you would lose on the position if it turned around right now and went down to its stop point. 


Table 5.5 Portfolio composition, 21 May 2009


<table><tr><td>Position</td><td>Sector</td><td>Contracts held</td><td>Days held</td><td>Portfolio impact (%)</td><td>Notional exposure dollar</td><td>Notional exposure (%)</td><td>Cost to stop</td></tr><tr><td>Australian Dollar</td><td>Currencies</td><td>6</td><td>15</td><td>0.61</td><td>389,280</td><td>7.79</td><td>-29,280</td></tr><tr><td>Canadian Bankers&#x27; Acceptance</td><td>Rates</td><td>30</td><td>156</td><td>2.64</td><td>7,353,496</td><td>147.07</td><td>-15,766</td></tr><tr><td>Canadian Dollar</td><td>Currencies</td><td>7</td><td>1</td><td>0.01</td><td>604,100</td><td>12.08</td><td>-19,600</td></tr><tr><td>Cotton</td><td>Agricultural</td><td>11</td><td>9</td><td>-0.35</td><td>127,655</td><td>2.55</td><td>-8,910</td></tr><tr><td>Euro</td><td>Currencies</td><td>4</td><td>1</td><td>0.13</td><td>691,350</td><td>13.83</td><td>-26,350</td></tr><tr><td>Eurodollar 3M</td><td>Rates</td><td>31</td><td>31</td><td>0.68</td><td>7,578,338</td><td>151.57</td><td>-20,538</td></tr><tr><td>Euribor 3M</td><td>Rates</td><td>35</td><td>158</td><td>6.11</td><td>11,337,779</td><td>226.76</td><td>-9,243</td></tr><tr><td>Euroswiss 3M</td><td>Rates</td><td>51</td><td>158</td><td>5.23</td><td>13,835,671</td><td>276.71</td><td>-14,671</td></tr><tr><td>Short Sterling 3M</td><td>Rates</td><td>41</td><td>29</td><td>0.68</td><td>7,853,534</td><td>157.07</td><td>-26,738</td></tr><tr><td>Hang Seng China Enterprises</td><td>Equities</td><td>3</td><td>13</td><td>0.06</td><td>181,175</td><td>3.62</td><td>-18,929</td></tr><tr><td>Hang Seng</td><td>Equities</td><td>2</td><td>11</td><td>0.05</td><td>201,572</td><td>4.03</td><td>-16,881</td></tr><tr><td>Nasdaq 100</td><td>Equities</td><td>2</td><td>16</td><td>-0.05</td><td>261,798</td><td>5.24</td><td>-15,998</td></tr><tr><td>New Zealand Dollar</td><td>Currencies</td><td>7</td><td>9</td><td>0.04</td><td>380,800</td><td>7.62</td><td>-18,200</td></tr><tr><td>Gasoline</td><td>Non-agricultural</td><td>4</td><td>1</td><td>0.05</td><td>274,714</td><td>5.49</td><td>-31,114</td></tr><tr><td>Soybeans</td><td>Agricultural</td><td>5</td><td>15</td><td>0.62</td><td>261,000</td><td>5.22</td><td>-26,000</td></tr><tr><td>Sugar</td><td>Agricultural</td><td>20</td><td>14</td><td>0.28</td><td>210,112</td><td>4.20</td><td>-28,000</td></tr><tr><td>Swiss Franc</td><td>Currencies</td><td>5</td><td>5</td><td>0.11</td><td>585,438</td><td>11.71</td><td>-20,125</td></tr><tr><td>Silver</td><td>Non-agricultural</td><td>3</td><td>10</td><td>0.18</td><td>224,670</td><td>4.49</td><td>-22,170</td></tr><tr><td>US 2Y Note</td><td>Rates</td><td>14</td><td>157</td><td>1.46</td><td>2,945,636</td><td>58.91</td><td>-18,516</td></tr></table>

If you look more closely at the table, you can see that there is a large difference in the exposure for different sectors. The rates sector seems always to have a much larger exposure and this is not a coincidence. All positions are volatility adjusted with the idea of allocating approximately equal risk to each position. That would imply that a more volatile asset gets a much smaller allocation in terms of exposure while a less volatile instrument is given a larger weight. Relatively speaking, rates are very low volatility instruments compared to equities, commodities and so on and as a general rule the shorter the duration the lower the volatility. This is the reason that out of the 1,100% exposure, about 960% comes from short-term money market futures. Does this mean that our portfolio is entirely driven by the rates and the impact of equities, commodities and currencies really does not matter? Certainly not. Out of 19 positions, 6 are in rates and that means that approximately one third of the risk at the moment is in rates. 

Much more relevant here is the distance to the stop, that is, how much it would cost us if the position went in the wrong direction until it hits our stop point. As you can see from Table 5.5, the cost to the stop points is not greater for the rates sector than for any other asset class. The stop is calculated the same for each instrument; from the peak positive reading for the open position, a maximum damage of 3 × risk factor is allowed on the portfolio as a whole. For a US$5 million portfolio that means that the giveback is theoretically capped at US$30,000. Of course this does not count slippage and potential adverse gaps, and so in your worst case scenario calculations you need to assume something very bad and highly unexpected will happen sooner or later and make sure you can deal with it. 

The total notional exposure of the long and short rates futures is over 10 times of our account size by itself. Someone might ask what happens if the rates markets move 10% against us in one day; would that not wipe out our account instantly? Well, the maths is simple – of course it would. Just like a giant meteor from the sky hitting our building is quite likely to put an end to the trading as well, but let’s put things into context here. I am not worried about a 10% intraday move in the short-term rates market, but rather a 0.5% move. Well, let’s go nuts and say that even a full 1% move is worth being worried about, even though it has never happened in the money markets so far. But worrying about a 10% day in the money markets is like worrying that the S&P 500 will hit zero before the closing bell. If an event like that happens, you are way beyond being concerned about your trading account. You are even way beyond being concerned about holding physical gold in your basement. The concern you are likely to have if something like that happens is how much canned food you have and how well armed you are, because it would take a world altering event for this to happen. 

Don’t get me wrong. Highly improbable events can and will happen and some suit on TV will keep referring to these events as five standard deviation events or whatever the number of the day is. Odd events happen much more often than any normal bell curve would suggest and that we have to deal with, but these kinds of risks apply equally to all sectors because they all have their weaknesses. There could be a 1% move in the Eurodollar in a day just as there could be a 25% move in the Nasdaq 100 in one day. Look back in history at the worst case scenarios and assume something much worse will happen in the next five years and be prepared for it, but don’t let notional exposure bother you just because they look like big scary numbers. 

# Year by Year Review

The strategy we have arrived at is already on a par with what most CTA funds and futures managers are able to produce. In its current shape it is quite usable for managing money, although it is certainly possible to improve upon it further. What we have now is a core strategy that is very similar to the base strategy of most trend-following managed futures funds and as such it has its merits. To be able to make intelligent decisions regarding what should be further enhanced with this strategy you need to properly understand how it really behaves and this is an extremely tough insight to build. There is no substitute for experience in this regard and having seen a strategy perform in the wild is the only way to gain a complete understanding of what it is capable of. But in lieu of that, in this chapter I try to paint as clear a picture as I can of what it would have been like to manage this strategy as it stands over a longer period of time. 

It is clear that certain years are more interesting than others. Some years everything is just plain old business as usual with not much action going on, but in other years there may be large swings and important analytical conclusions to be drawn. I go over the 22 years from 1990 to 2011 and explain what happened, what went right and what went wrong. If things looked easy when you saw the overview simulation data in the previous chapters, this chapter will highlight where the difficulties can come in. 

In the following analyses I always take commissions and slippage into account to keep things realistic and I assume a 1.5% management fee and 15% performance fee, both payable yearly in arrears. In reality the management fee is often paid monthly or quarterly and some funds charge performance fees intra-year as well, but it would not add much to the analytical points to model these details here. 

As a general market comparison, I use the global equity index MSCI World Total Return, which includes reinvested dividends. This is certainly not a strategy that attempts to mimic or beat the equity indices and as a benchmark it is not really a fair comparison because they are very different animals, but it is my experience that investors, individual and institutional alike are very focused on the overall state of the equity market and that the pressure on a futures manager thereby goes up as equities go up and declines when equity markets are doing poorly. Even if your strategy is completely unrelated to equities, this tends to be the case. The only explanation I can offer is that it is human nature to want to gain when everyone else is gaining and that a loss does not feel so bad when everyone else is also losing. For most investors, a loss hurts much more if their neighbours are gaining at the same time. This phenomenon never ceases to amaze me, but it seems a fact of life for our industry. 

## HOW TO READ THIS CHAPTER

This is the longest chapter of the book and as it goes through the behaviour and performance of the strategy over the course of 22 years, it may feel like ancient history and cause you to wonder whether this is just a page filler. I can assure you that nothing is further from the truth. In my view, this chapter is by far the most valuable learning opportunity in the book and if you want to understand trend trading in depth, you should reflect on each year, looking at the details in the performance charts and trying to imagine what life is like for a professional trend trader. 

What you are normally told in books and marketing material is that trend trading is easy and highly profitable. The study of the year by year behaviour and breakdowns on sectors and directions shows that although it is profitable in the long run and the trading rules are theoretically simple, it is far from easy to accomplish the results in real life. See this chapter as a reality check. It is my way of showing the real side of this business, the good and the bad, without overselling or overhyping. If you want to enter into the field of trend trading, read the book through once first. Then go back and study the details of this chapter again. 

When you have settled on your own trading strategy, whether by constructing your own or modifying my core strategy, make realistic simulations and compare the details to this chapter, year by year and month by month, to see how your strategy would have handled things differently and whether it is still a viable way forward. 

You simply cannot base your strategy-selection process just on simulation summary statistics or a longterm equity curve. 

After this year by year review, in the next chapters I look more closely at how to replicate and reverse engineer existing futures hedge funds as well as how to further improve upon the core strategy. 

## 1990

So, imagine that we are back in late 1989: Bon Jovi was selling LPs like crazy, the Chinese were rolling tanks into Tiananmen Square and the pastel-coloured 1980s were slowly starting to fade. You were in luck because you had just received US$10 million committed from investors for your new managed futures fund and you had all your infrastructure set up, ready to go. 

On the morning of 2 January 1990 you ran your strategy simulation on your computer and a list of long and short futures came up on your screen for you to enter as a starting portfolio. The number of positions at any given time can vary greatly, depending on how many interesting trends are available for your strategy to enter. In this case, your first portfolio of futures contracts was larger than average, since there were many good trends to play at this time. 

The important thing to remember is that all position sizes are adjusted for volatility, so that in theory they have the same approximate daily impact on the bottom line of our whole strategy. You can find the details of this process in previous chapters, but the importance of taking that part seriously cannot be overstressed. Without proper position sizing, your strategy will fail. 

The initial portfolio for this strategy at the start of January 1990 is shown in Table 6.1. 

Table 6.1 Initial portfolio 1990 

<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Lumber</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Live cattle</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Oats</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Soybeans</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Swiss franc</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Australian dollar</td><td>Long</td><td>Currencies</td></tr><tr><td>British pound</td><td>Long</td><td>Currencies</td></tr><tr><td>Canadian dollar</td><td>Long</td><td>Currencies</td></tr><tr><td>Euro/USD (ECU)</td><td>Long</td><td>Currencies</td></tr><tr><td>Japanese yen</td><td>Short</td><td>Currencies</td></tr><tr><td>CAC 40</td><td>Long</td><td>Equities</td></tr><tr><td>FTSE 100</td><td>Long</td><td>Equities</td></tr><tr><td>Hang Seng Index</td><td>Long</td><td>Equities</td></tr><tr><td>Crude oil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Copper</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Heating oil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Palladium</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoline</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Canadian Bankers’ Acceptance</td><td>Short</td><td>Rates</td></tr><tr><td>Eurodollar</td><td>Long</td><td>Rates</td></tr><tr><td>Short sterling</td><td>Short</td><td>Rates</td></tr><tr><td>US 10-year note</td><td>Long</td><td>Rates</td></tr></table>


Table 6.2 Initial sector allocation 1990


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>4</td><td>1</td><td>5</td></tr><tr><td>Agricultural commodities</td><td>3</td><td>2</td><td>5</td></tr><tr><td>Non-agricultural commodities</td><td>4</td><td>2</td><td>6</td></tr><tr><td>Equities</td><td>3</td><td>0</td><td>3</td></tr><tr><td>Rates</td><td>2</td><td>2</td><td>4</td></tr><tr><td>Total</td><td>16</td><td>7</td><td>23</td></tr></table>

Given that each position has the same volatility adjusted size, we can easily sum up each sector to see how the overall allocation of the fund looked (see Table 6.2). This is naturally always an approximation, because the volatility adjusting sizing relies on the flawed assumption that the volatility of the respective instruments will remain constant. As the pie chart in Figure 6.1 shows, our initial portfolio seemed quite well balanced between sectors. Commodities, both agricultural and non-agricultural, held the lion share but the currencies and rates baskets were fairly large as well. Equities held the smallest part, but still a 13% stake. We can also quickly see that in the equity sector we held only longs, in the rates we were long in Canadian and US rates and short British, metals were short, energy long and agriculturals mixed. That should make for an interesting portfolio to start off with. 

## Figure 6.1 Sector allocation 1990

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/6198a75270d77da5ef7fed6c361f46279489030b86491b4cc0b70d8271e9f4bc.jpg)



Non-Agricultural Commodities, 26%


The first year of the 1990s was a turbulent one that saw global equity prices shed over 25% of their values. We had just left the roaring 1980s and a rebound of some sort was overdue. It was hardly a smooth ride down though as the year began with a bear market move of 18%, followed by 15% rebound to the upside, another 22% down and then a slow recovery of 9% before the year ended. In such a market it is very difficult to make money with normal equity strategies and it makes for a good example of how diversified futures strategies can provide value. 

Figure 6.2 shows how our strategy performed compared to MSCI World this year. Early on in the year the strategy was struggling sideways with a maximum loss on the year of 3% before slowly moving upwards. The upward move got stronger and stronger while the MSCI World stock index kept falling and at this time our initial long equity bias had naturally shifted into a short bias. In May both our strategy and the index started reversing and moving more or less sideways during the middle of summer until they both continued their trends in August, when the index started losing and we started gaining. The peak of our strategy was in September when we see a rather large spike upwards in our profits which lasts very briefly before we move sideways to downwards for the remainder of the year. Our maximum gain over the year was over 45% but we closed at 30% up. 


Figure 6.2 Strategy performance 1990


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/53813235ee82c9b52fd690f1c69cbfeb7fdbae5c66bd4ddcdba6ba6cf7e98865.jpg)


Compare also in Figures 6.3 to 6.5 how the sectors and the long versus short positions behaved. In this year the short strategy showed a smoother return and despite going sideways for some months it ended up with a higher return than the long side. This is actually unusual for this type of strategy and normally you will find that the short side of the strategy is choppier, less predictable as well as less profitable. 


Figure 6.3 Sector performance 1990


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/fd062f135339e5ebfa62a214c1c24b7faa0dbc73591e9ab57eb05679dfb4a122.jpg)



Figure 6.4 Long sector performance 1990


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/9cab3ee5ed7a598d35bd3f4a9010f4914db58113bead11c7793e2e479d987af3.jpg)



Figure 6.5 Short sector performance 1990


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/3a3e7d1a64466464c6b9e62140e750e23a546117e6f7a788b693a1c4dc02bb53.jpg)


This might look like a very nice year for the strategy with the end result being a gain of almost 30%, but it was a difficult year from a psychological perspective and that should not be underestimated. If we started the year with US$10 million under management, this would mean that at the peak our account was up to US$14.5 million and at that time you would probably be ecstatic and thrilled by the enormous trading success. Most likely you expected the current angle of ascent to continue and did the maths over and over again on how much money the fund would make at the end of the year if this angle continued, not to mention how much money you would make in performance fee and what a hero you would be to your investors. This is human psychology and very hard to avoid, but never forget that diversified trend following is prone to extreme periods of success followed by sharp declines and sideways choppy markets. This is part of the game and nigh impossible to avoid. 

After drinking the premature champagne in late August, the setbacks started coming in. Although the short side of the strategy kept moving smoothly, the long side took a big and sudden hit, pushing our account value down US$1.5 million dollars in a matter of days. That was a hard hit to take at that moment, although the year looks good overall in retrospect. After this, the rest of the year was very frustrating for the manager. The last four months of the year the fund value bobbed up and down in a slowly declining path and we never returned to the high of the year. 

Some investors are very short-sighted and you may have had redemptions from disgruntled clients who started expecting that the month of August would be the norm and who felt that the last four months of the year represented a significant enough losing streak that their confident in you as a manager started dwindling. Also don’t forget that an investor who entered the fund at the end of August would have lost 10% by the end of the year and that person was unlikely to be a happy camper. 

The sector leadership changed over the year as can be seen in Figure 6.3 and the big driving force in the first quarter of the year was clearly rates. Up until May this sector was completely dominating the profit and loss (P&L) of the fund and after that it slowly started trending down for the remainder of the year, still leaving a profit at the end of the day. This is again a typical behaviour that can be frustrating when it happens but should be seen as the cost of doing business in this very specialised part of the industry. The profits on the rates were mainly on the short side as Figure 6.5 shows and much of it came from the UK and Canadian instruments. The agricultural commodities sector was a very stable earner this year and kept moving up at a nice and smooth pace and here as well we were making the bulk of the money on the short side. The non-agricultural commodities sector had a highly volatile year and it was clearly responsible for that big spike in the overall performance in August we saw earlier. Up until the end of July this sector had a negative performance and was not doing anything worth writing home about. It took loss after loss and seemed doomed to have a very uninteresting and unprofitable year. But then suddenly in August, there was a massive spike up in the profits of the non-agricultural sector. In fact, the spike was so large that something significant must have occurred in the market. Let’s see, what could possibly have happened in August of 1990 that would be worth remembering? 

If you said the Gulf War, full marks; those who guessed on the solar eclipse that same month get to stand in the corner for the rest of the chapter and think about what they have done! Our strategy was already long several oil-related markets when the Iraqi tanks rolled into Kuwait and the massive price spike that followed in crude and other oil markets generated huge profits for us, some of which were given up as oil dropped again following the start of Operation Desert Shield. One of these trades was the gasoline in Figure 6.6. The two solid lines above and below the price plot are the 50-day high and 50-day low, showing where the strategy would enter a new trade on a breakout if the overall trend was in the same direction. The dots below each daily price candle show where the stop point is located for that day. Remember that this is an end of day stop, and so we need a close beyond this dot to exit the position the following day. 

Figure 6.6 Gasoline around the time of Gulf War I 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/4011b1f4c3474a27f8d19eba8f6ff0befdf09c725fde03346f9b2a96bb5ccef4.jpg)



For equities, this was an absolutely boring year with several trades in and out of the market with most of them ending up as small losses. This sector was under water for most of the year and clearly taking the back seat in terms of P&L. Finally, the currencies were marginally profitable up until June but then took off, creating large and more importantly consistent gains throughout the remainder of the year.


At the end of the year we were left holding a nice gain, the bulk of which came from long currencies and short agricultural commodities, with some contribution from the non-agricultural commodities as well as from the rates. The end of year breakdown is shown in Table 6.3. 


Table 6.3 Sector results 1990


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>10.2</td><td>1.9</td><td>-0.8</td><td>-0.5</td><td>-1.7</td><td>9.0</td></tr><tr><td>Short</td><td>0.5</td><td>8.7</td><td>6.7</td><td>0.0</td><td>5.4</td><td>21.4</td></tr><tr><td>All</td><td>10.7</td><td>10.6</td><td>5.9</td><td>-0.5</td><td>3.8</td><td>30.4</td></tr></table>

These numbers are all in terms of impact on the portfolio, net of commissions and slippage but before external fees and interest income. Table 6.4 shows how the net results of the year look including these items as well. Note that the fee calculations are slightly simplified in this table and meant to demonstrate the broad strokes, not to train you to become a fund administrator. Luckily there are companies who provide those services for reasonable fees. The result before any fees was 30.4%, but that was not the number your investors saw. In the 1990s interest rates were quite high and we could therefore get quite a large contribution from Uncle Sam, the Queen or other applicable government personifications in your country. The effect of this money, which is explained in more detail in Chapter 5, was quite extreme in this era and it goes to show how much easier it was to manage futures funds in the days of high inflation. 


Table 6.4 Results 1990


<table><tr><td>Year</td><td>1990</td></tr><tr><td>Starting Net Asset Value (NAV)</td><td>100</td></tr><tr><td>Trading result</td><td>30.4%</td></tr><tr><td>Interest income</td><td>6.6%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.8%</td></tr><tr><td>Performance fee</td><td>-5.2%</td></tr><tr><td>Net result</td><td>29.5%</td></tr><tr><td>Ending NAV</td><td>129.5</td></tr></table>

There were also bills to be paid of course, and I assume fixed external costs of 0.5% for admin, custody and so on, as well as a management fee of 1.5%. The management fee was calculated on average fund value and therefore may end up higher or lower than 1.5% of the initial money under management. If we do well, which we certainly did this year, we also get a performance fee of 15% of the profits after all other costs have been paid. The percentage number in Table 6.4 shows how large the performance fee was in relation to the initial asset base at the beginning of the year. 

## 1991

Going into 1991, the initial portfolio looked quite a bit different from last year, which is often the case (see Table 6.5). Last year we entered with 23 positions whereas this year started with only 14 (as shown in Table 6.6). Remember that in theory each position represents approximately equal risk. Strictly speaking this is of course not true, or at least the word approximate has been stretched a bit, but the concept should be clear to you at this point. When positions are opened, they are volatility adjusted so that they represent equal theoretical risk based on the past 100 days of fluctuation, which is a good enough estimator for our purposes. The actual risk will change as the position grows or declines as the price moves up and down and also as volatility itself changes. Still, the portfolio we entered this year with was clearly less risky than the one that started 1990. 


Table 6.5 Initial portfolio 1991


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Corn</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Cotton</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Live cattle</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Oats</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Soybeans</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Wheat</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Australian dollar</td><td>Short</td><td>Currencies</td></tr><tr><td>Canadian dollar</td><td>Long</td><td>Currencies</td></tr><tr><td>CAC 40 Index</td><td>Short</td><td>Equities</td></tr><tr><td>Natural gas</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Palladium</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Euribor</td><td>Short</td><td>Rates</td></tr><tr><td>Eurodollar</td><td>Long</td><td>Rates</td></tr><tr><td>US 2-year T-note</td><td>Long</td><td>Rates</td></tr></table>


Table 6.6 Initial sector allocation 1991


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>1</td><td>1</td><td>2</td></tr><tr><td>Agricultural commodities</td><td>2</td><td>4</td><td>6</td></tr><tr><td>Non-agricultural commodities</td><td>0</td><td>2</td><td>2</td></tr><tr><td>Equities</td><td>0</td><td>1</td><td>1</td></tr><tr><td>Rates</td><td>2</td><td>1</td><td>3</td></tr><tr><td>Total</td><td>5</td><td>9</td><td>14</td></tr></table>

This January we had the bulk of our risk in commodities and in particular on the agricultural ones. As the pie chart in Figure 6.7 shows, the two types of commodities together represented close to 60% of the risk in this initial portfolio whereas equities was put on the back burner with only 7% and just a single position in the short CAC 40. 


Figure 6.7 Sector allocation 1991


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/f472b741fbf0ec09b64f2d85977981c5bd7af611d7329d39429716b5bb86ab03.jpg)


Take a good look at Figure 6.8 showing the profit and loss development over the course of 1991 and think through whether you would have been able to execute that strategy or if you would have been likely to override or quit. Having had a successful 1990 behind you helps, but if you started out like this year it would have been easy to throw in the towel before year end. Up until October you had nine long months where almost nothing happened at all despite plenty of trades being entered and exited. So for the better part of a year you kept working hard, taking trade after trade, but you kept ending up at more or less the same numbers and far below what the equity market returned. The reality is that at the start of October this year, anyone would have been sick and tired of the strategy and contemplating all kinds of changes and tweaks. The rewards however tend to come to those who stick to their rules and follow the game plan. If your strategy begins doing things that are very unexpected you should start looking for what is wrong and whether you need to fix something, but the type of behaviour seen in 1991 is not that uncommon and, as annoying as it is when it happens, you need to just keep swimming and not start messing with any parameters. 

Figure 6.8 Strategy performance 1991 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/58569c38c54f0649558534276a5aa9be5febf462bc0d78cc97e635ec0322db22.jpg)



If you are wondering whether I seem to have a data spike error in August in the MSCI World, I suggest you carry out an Internet search for ‘Soviet Union coup d’état’ and see what comes up. For our strategy, however, this event did not have a noticeable impact.


The sector overview chart in Figure 6.9 tells pretty much the same story about a long, boring three quarters of a year where no sector was really gaining or losing much. Then by the end the rates started shooting up and they kept moving up smoothly for the remainder of the year. Clearly something was going on here. In Figures 6.10 and 6.11 you can compare the long and the short side and quickly see that the long side of the rates game was responsible for the excellent comeback this year, albeit with a little help from the short non-agricultural commodities. As the Soviet Union crumbled, the yields in the Western economies started moving steadily down with our long bond futures thereby gaining nicely (see Figure 6.12). 


Figure 6.9 Sector performance 1991


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/e2fc2d9a45f451a3b97aeb749df7389d66f161e1b4ddf1f39d3d24f24218d070.jpg)



Figure 6.10 Long sector performance 1991


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/ffe4264248ad11d68966ac7b34a4c2bd6eb2ed1aae0f4ebe5bdaafbae9c08e42.jpg)



Figure 6.11 Short sector performance 1991


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/b653e46fb98617e914caa7fe87f126bbe7d91858c722539665da794889b435d5.jpg)



Figure 6.12 S&P 500 during the Soviet coup


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/6d4898de2dc3b8ca799865c1183d6cb4bda53be8190f827ffb60bfbd3df6f041.jpg)


Luckily for us, the strategy was not much into equities at the time of the Soviet coup or it might have been a costly experience. We did however enter on the strong recovery in the days following and though those trades ended up losing, they were quite orderly. 

Before fees we produced a result of +25.6%, which would have to be seen as a very strong year (see Table 6.7). The fact that we received another 5% less change for free in interest income was a very nice extra benefit of having a futures strategy in this monetary climate (see Table 6.8). After all fees we showed the investors a return on their money of just under 24%, clearly beating the equity market and most other benchmarks. 

Table 6.7 Sector results 1991 

<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>4.3%</td><td>2.7%</td><td>-4.9%</td><td>0.5%</td><td>17.9%</td><td>20.5%</td></tr><tr><td>Short</td><td>-2.3%</td><td>-0.7%</td><td>8.2%</td><td>-1.5%</td><td>1.5%</td><td>5.1%</td></tr><tr><td>All</td><td>2.0%</td><td>2.0%</td><td>3.3%</td><td>-1.0%</td><td>19.4%</td><td>25.6%</td></tr></table>


Table 6.8 Results 1991


<table><tr><td>Year</td><td>1991</td></tr><tr><td>Starting NAV</td><td>129.5</td></tr><tr><td>Trading result</td><td>25.6%</td></tr><tr><td>Interest income</td><td>4.6%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.7%</td></tr><tr><td>Performance fee</td><td>-4.2%</td></tr><tr><td>Net result</td><td>23.7%</td></tr><tr><td>Ending NAV</td><td>160.3</td></tr></table>

## 1992

The risk level of the initial 1992 portfolio was fairly high, holding a full 29 positions with the largest concentration being in short non-agricultural commodities as well as short agricultural commodities (see Table 6.9). This was a somewhat unusual portfolio because there were several direct bets against the US dollar while at the same time plenty of short commodity positions. Generally speaking, commodities tend to do better when the dollar is trending down so it would go against conventional wisdom to be short both the dollar and the commodities. There are of course no fixed rules in the marketplace and just about anything is possible, at least for a limited period of time. 


Table 6.9 Initial portfolio 1992


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Corn</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Cotton</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Lumber</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Lean hogs</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Soybeans</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Wheat</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>British pound</td><td>Long</td><td>Currencies</td></tr><tr><td>Euro (ECU at this time)</td><td>Long</td><td>Currencies</td></tr><tr><td>Japanese yen</td><td>Long</td><td>Currencies</td></tr><tr><td>Swiss franc</td><td>Long</td><td>Currencies</td></tr><tr><td>DAX Index</td><td>Short</td><td>Equities</td></tr><tr><td>Hang Seng Index</td><td>Long</td><td>Equities</td></tr><tr><td>S&amp;P 500 Index</td><td>Long</td><td>Equities</td></tr><tr><td>Crude oil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gold</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoline</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Heating oil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Natural gas</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Palladium</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Platinum</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Silver</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Canadian Bankers’ Acceptance</td><td>Long</td><td>Rates</td></tr><tr><td>German Bund</td><td>Long</td><td>Rates</td></tr><tr><td>Eurodollar</td><td>Long</td><td>Rates</td></tr><tr><td>Euribor</td><td>Short</td><td>Rates</td></tr><tr><td>Short sterling</td><td>Short</td><td>Rates</td></tr><tr><td>US 2-year note</td><td>Long</td><td>Rates</td></tr><tr><td>US 10-year note</td><td>Long</td><td>Rates</td></tr></table>

Table 6.10 and Figure 6.13 show that the bets in the equity markets were very small with two longs and one short, and so no big stake there. On the rates side we were leaning towards the long side, with five long positions and two shorts. 


Figure 6.13 Sector allocation 1992


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/0eb23f29d61bad22cf196030340541012e1c026f616f04dd11a0cf0e42089a1d.jpg)



Table 6.10 Initial sector allocation 1992


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>4</td><td>0</td><td>4</td></tr><tr><td>Agricultural commodities</td><td>1</td><td>5</td><td>6</td></tr><tr><td>Non-agricultural commodities</td><td>0</td><td>9</td><td>9</td></tr><tr><td>Equities</td><td>2</td><td>1</td><td>3</td></tr><tr><td>Rates</td><td>5</td><td>2</td><td>7</td></tr><tr><td>Total</td><td>12</td><td>17</td><td>29</td></tr></table>

As Figure 6.14 shows, the start of the year was quite rocky and would certainly take its toll on the fund manager. After gaining 3% in a matter of days, the fund slipped back 8%, down to –5% on the year before the end of January. The fund struggled slowly upwards for several months before finally being almost back at the zero line in April when it got smacked down hard to a new year low of –7%. Even after some recovery back in June, we were still in the negative and investors were probably calling more and more frequently to ask what was going on and whether the strategy had simply stopped working. Lucky for us, the world stock markets were also down and since investors in general are more patient with losses if they occur when everyone is also losing, we probably did not have too many problems with redemptions. 


Figure 6.14 Strategy performance 1992


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/257c6a262997f10304d352515a2bc4eb3dcca45fe1b6b8ac383ddb60140129db.jpg)


In July we were finally rewarded for the difficult first half of the year when both the long and the short side of the strategy started kicking in at the same time and we moved up to a year high of +15% in just a few months. As is so often the case with this strategy, a big chunk of the profits were then given up again as trends reversed and in early October we were back to nail-biting mode again, but still holding on to 5% of profits in a choppy sideways market for the remainder of the year. 

Looking at the sector return charts in Figures 6.15 to 6.17, we can clearly see that the sudden drop in January was caused by the long rates, long currencies and short non-agricultural commodities. Many of the positions that reversed at the start of the year had been held for some time and were quite profitable since entered, but all that is seen on this particular year of course is the reversal and thereby the loss. One month into the year the number of positions was cut down to a third as stop after stop was hit. 

Figure 6.15 Sector performance 1992 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/14e988594e60f133c207bc1b5afe4ce52a439df0641ea2c9e345b02e4a692324.jpg)



Figure 6.16 Long sector performance 1992


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/118c49e9f1d60d97d1bcda366a6d567f23029f37ea1c80eb71120dde78643cec.jpg)



Figure 6.17 Short sector performance 1992


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/0156951a81c16f630d5eedcf129ce68f1ae8238eb1cc58e9d8ab344e5949e423.jpg)


The equity side of the strategy in fact did very well this year and showed quite remarkably stable returns given the spotty performance of the global stock indices. Our strategy held both long and short equity 

index futures for much of the year, which is unusual because the correlation between different geographical stock markets tends to be quite high, often leading the strategy to pick either the long or the short side, but in this year some markets did very well while others lost. The Hong Kong stock market had a very nice run up even though the European and American markets fell and since Japan was in full economic crisis mode, there was plenty of money to be made on being short on the Nikkei. 

Several currency futures were hit on the September dollar rebound, but most of them already had some profits on the books and cashed out on them. The Euro chart in Figure 6.18 shows the gap move that contributed to the losses for the strategy during this month. 


Figure 6.18 Euro (ECU) Futures 1992


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/6863cbcd34ba4880c90a927e01cc82fa700adf217ae213c90a66d37fe256e044.jpg)



Most of the sectors had quite a mediocre showing this year and the non-agricultural commodities were in particular disappointing, but none of the sectors racked up any sizable losses.


All in all Tables 6.11 and 6.12 show that 1992 was not a very good year, but we did manage to land on the positive side of the fence. The gross result was 6.3% and the net effect of interest income and costs were now getting to be about even, landing the fund at a result of 5.9% net of everything. This was a tough year for everyone and the equity markets, which most investors use consciously or not as their benchmark, lost about 7% and so overall in the light of the environment this was a bad year but not a terrible year. Of course, after 12 months of hard work with very little to show for it, you might not have agreed at the time. 


Table 6.11 Sector performance 1992


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>2.1</td><td>-0.7</td><td>-0.3</td><td>3.3</td><td>5.3</td><td>9.7</td></tr><tr><td>Short</td><td>-1.1</td><td>4.0</td><td>-2.8</td><td>2.2</td><td>-5.8</td><td>-3.3</td></tr><tr><td>All</td><td>1.0</td><td>3.3</td><td>-3.1</td><td>5.6</td><td>-0.5</td><td>6.3</td></tr></table>


Table 6.12 Results 1992


<table><tr><td>Year</td><td>1992</td></tr><tr><td>Starting NAV</td><td>160.3</td></tr><tr><td>Trading result</td><td>6.3%</td></tr><tr><td>Interest income</td><td>2.7%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.6%</td></tr><tr><td>Performance fee</td><td>-1.0%</td></tr><tr><td>Net result</td><td>5.9%</td></tr><tr><td>Ending NAV</td><td>169.8</td></tr></table>

## 1993

We entered into 1993 with 16 positions open, and about medium risk level for the strategy (see Tables 6.13 and 6.14 and Figure 6.19). The portfolio was quite well diversified with a slight tilt towards long agricultural commodities but no really big bets in any single theme. At the end of last year the P&L curve had been moving sideways for some time and there was a general lack of strong trends in the marketplace, which explained why there were no significant bets on at the start of 1993. 


Figure 6.19 Sector allocation 1993


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/9b4ca70c5d64a268974a22c6ded8dbb997d0712bb5c028f9aa5c10f74e1ac64e.jpg)



Non-Agricultural Commodities, 13%



Table 6.13 Initial portfolio 1993


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Lean hogs</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Live cattle</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Lumber</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Oats</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Rough rice</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Sugar</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>British pound</td><td>Long</td><td>Currencies</td></tr><tr><td>Euro</td><td>Short</td><td>Currencies</td></tr><tr><td>Swiss franc</td><td>Short</td><td>Currencies</td></tr><tr><td>FTSE 100 Index</td><td>Long</td><td>Equities</td></tr><tr><td>S&amp;P 500 Index</td><td>Long</td><td>Equities</td></tr><tr><td>Gasoil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Silver</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>German Bund</td><td>Short</td><td>Rates</td></tr><tr><td>US 10-year note</td><td>Short</td><td>Rates</td></tr><tr><td>US 2-year note</td><td>Long</td><td>Rates</td></tr></table>


Table 6.14 Initial portfolio allocation 1993


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>1</td><td>2</td><td>3</td></tr><tr><td>Agricultural commodities</td><td>4</td><td>2</td><td>6</td></tr><tr><td>Non-agricultural commodities</td><td>1</td><td>1</td><td>2</td></tr><tr><td>Equities</td><td>2</td><td>0</td><td>2</td></tr><tr><td>Rates</td><td>1</td><td>2</td><td>3</td></tr><tr><td>Total</td><td>9</td><td>7</td><td>16</td></tr></table>

As Figure 6.20 reveals, the first month was quite uneventful with a slight gain that was quickly lost, but after that the exciting times started when our profits suddenly took off in a serious way and hit a 20% profit level in just over a month. We then saw a choppy sideways development for some time, but the slight tilt to the upside was always with us and by the end of the year our performance spiked up again to end at a year high of almost +40%. This was an excellent year, one of those rare ones with no real difficult periods. 


Figure 6.20 Strategy performance 1993


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/74d12d7e4aa13bc63ef438371c11a6b0566cbbb34f5ba5c2f94eec8743af5f3f.jpg)


The profits all came from the long side while the short side was idling along the zero line for most of the time and even hanging out below it for several months. This is quite common and the bulk of the profits tend to come from the long side. Still, the short side is a much needed stabiliser over time and tends to perform very well when the global marketplace is experiencing some larger crisis. 

The big run-up early in the year was caused mainly by agricultural commodities with some help along the way from the rates sector (see Figures 6.21 and 6.22). The initial gain in the agricultural commodities was a combination of the long and short sides where both gained at the same time, showing the strength of a truly diversified strategy. The short agriculturals (Figure 6.23) lost their gains later in the year whereas the long side not only kept them but also added significantly to them late in the year. 


Figure 6.21 Sector performance 1993


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/f8fd5d3398ddc009cf4f94b397af2607a9b6f5e8793a6fa8c98bd65b2b249242.jpg)



Figure 6.22 Long sector performance 1993


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/6f4b585b9367145c31baa51ce3e948ac785e488bbadc9f700a1150d8e4640d34.jpg)



Figure 6.23 Short sector performance 1993


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/563c22ffe28a3f4689e9f110fa229a09bf8fa93fd48880725913bb7cff4f6e0b.jpg)


Given that the return curve of our fund followed that of the MSCI World quite closely, as you can see from Figure 6.20, you might think that we made the bulk of the profits on long equities, but nothing could be farther from the truth. The equity side of the strategy performed quite poorly, both on the long and the short side, and at the end of December it showed only a very marginal gain. Instead the theme of this year was commodities, with long agriculturals being the main driver for most of the year and short nonagriculturals shooting up in December to provide a sizable overall contribution in the end. 

Despite the lack of action for some months, overall this was a fun year to be a trend-following futures manager, perhaps with the exception of the months of the turbulence in the fall. Even though the bottom line of the fund itself was held up due to the effective diversification, the losses incurred on the nonagricultural commodities on 5 August and following days were very painful at the time and left a bad taste in the mouth for quite a while after. On a single day the whole sector experienced a shock with all trends reversing suddenly and very strongly. The strategy was long metals and short energies when suddenly gold and other metals fell many times below their theoretical stop points racking up big losses and at the same time the energy futures all spiked up dramatically causing equally large losses. These types of events often feel like the end of the world when they occur but the fact of the matter is that the world very rarely ends and these days are simply the cost of doing business in the very profitable industry of diversified futures trading. 

The year ended at over 40% up with the bulk of the profits coming from the agricultural commodities, having had some contributions from non-agriculturals and rates. The currency side ended in the negative as the only sector to do so. 

The lean hogs trade (Figure 6.24) was not alone, but it certainly had a helping hand in the profitability of the agricultural sector this year. The position was already opened as we entered the year although it was just humming along sideways until February. After the sudden break to the upside two months into the year, the price skyrocketed and two months later the pigs were sold with a tidy profit. Note how close the price was to the dotted stop loss points at times and it was just ticks from being stopped out. 


Figure 6.24 Lean hogs long position 1993


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/e7075a86dc4cf6f1b46dd067964391f6ce9ce20a245ccf35ae2eef9118e1ad3c.jpg)



After all fees, there was still over 36% for the investors and with the performance fee the manager received, it would be a fair assumption to say that both parties were quite happy after this year (see Tables 6.15 and 6.16).



Table 6.15 Sector performance 1993


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>-1.7</td><td>21.2</td><td>3.7</td><td>4.2</td><td>11.7</td><td>39.1</td></tr><tr><td>Short</td><td>-2.9</td><td>-1.2</td><td>9.0</td><td>1.0</td><td>-2.6</td><td>3.3</td></tr><tr><td>All</td><td>-4.6</td><td>20.0</td><td>12.8</td><td>5.2</td><td>9.0</td><td>42.5</td></tr></table>


Table 6.16 Results 1993


<table><tr><td>Year</td><td>1993</td></tr><tr><td>Starting NAV</td><td>169.8</td></tr><tr><td>Trading result</td><td>42.5%</td></tr><tr><td>Interest income</td><td>2.7%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.8%</td></tr><tr><td>Performance fee</td><td>-6.4%</td></tr><tr><td>Net result</td><td>36.3%</td></tr><tr><td>Ending NAV</td><td>231.5</td></tr></table>

## 1994

The initial portfolio this year held a higher than average risk with 28 opened positions at the start of January (see Tables 6.17 and 6.18). As Figure 6.25 shows, half of the portfolio was in commodities, with one quarter each in agricultural and non-agricultural and the remainder spread quite evenly between equities, currencies and rates. We were long precious metals, short energies, long equities, mainly long rates and mixed agricultural exposure. This made for quite a diversified portfolio with many bets and a high likelihood of showing low internal correlation. 


Table 6.17 Initial portfolio 1994


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Wheat</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Corn</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Soybeans</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Cotton</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Lumber</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Oats</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Lean hogs</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Canadian Bankers’ Acceptance</td><td>Long</td><td>Currencies</td></tr><tr><td>Australian dollar</td><td>Long</td><td>Currencies</td></tr><tr><td>British pound</td><td>Short</td><td>Currencies</td></tr><tr><td>Euro</td><td>Short</td><td>Currencies</td></tr><tr><td>Japanese yen</td><td>Short</td><td>Currencies</td></tr><tr><td>FTSE 100 Index</td><td>Long</td><td>Equities</td></tr><tr><td>Dax</td><td>Long</td><td>Equities</td></tr><tr><td>Hang Seng</td><td>Long</td><td>Equities</td></tr><tr><td>S&amp;P 500 Index</td><td>Long</td><td>Equities</td></tr><tr><td>CAC 40 Index</td><td>Long</td><td>Equities</td></tr><tr><td>Gold</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Silver</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Platinum</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoline</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Heating oil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Crude oil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Long gilt</td><td>Long</td><td>Rates</td></tr><tr><td>Short sterling</td><td>Long</td><td>Rates</td></tr><tr><td>German Bund</td><td>Long</td><td>Rates</td></tr><tr><td>Euribor</td><td>Short</td><td>Rates</td></tr></table>


Table 6.18 Initial sector allocation 1994


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>2</td><td>3</td><td>5</td></tr><tr><td>Agricultural commodities</td><td>5</td><td>2</td><td>7</td></tr><tr><td>Non-agricultural commodities</td><td>3</td><td>4</td><td>7</td></tr><tr><td>Equities</td><td>5</td><td>0</td><td>5</td></tr><tr><td>Rates</td><td>3</td><td>1</td><td>4</td></tr><tr><td>Total</td><td>18</td><td>10</td><td>28</td></tr></table>


Figure 6.25 Sector allocation 1994


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/5a9f3faf778ca5272529d1be1c0dc2b8756761e4e3885eb6e50f3ef554dc73ea.jpg)


Little could we have known at the time that this portfolio, which seemed so well rounded at the start of January, would turn out to be a disaster and that we were in for the worst year in decades. 1994 was one of those years where you end up wishing you had gone to dentist school instead of wasting your days losing money day after day and getting yelled at by understandably upset clients. 

Before the first week of January was up, the fund had lost 5% and the nightmare was far from over as Figure 6.26 reveals. Although the short side of the strategy had a mediocre but okay performance, the long side absolutely killed us this year. By the end of February the fund was down 13% and the zero line far out of reach. In November the low watermark of –20% was set and investors who came in at the start of the year needed to see a 25% increase in the NAV just to get their initial money back, and I can assure you that they were not happy. 


Figure 6.26 Strategy performance 1994


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/67c612815481688c5a93b4cd057db0967421f06098230856e3eba49861b865cd.jpg)


After a small move to the upside the year closed at almost –17% with most of the damage caused by the long positions. Looking at the sector attributions in Figures 6.27 to 6.29, no sector did very well but the pain came from two in particular: non-agricultural commodities and equities. The precious metals positions had all been entered just before the New Year and they were all stopped out early in January. For the energies, most of them were stopped out in the first few days, but they were re-entered again in February and stopped out again, compounding the losses. Many trends reversed early in the year and position after position was stopped out after taking losses. The year continued to be bad for the metals and energies and the short profitable summer in this sector was quickly replaced by further losses. 


Figure 6.27 Sector performance 1994


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/d3bc9a210086f99b66a1ce46c287f06cf2ed4dc19bc225cfddb461ae94379261.jpg)



Figure 6.28 Long sector performance 1994


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/cd2b459cbf2517b524322d0fca940738c65248648dc32e0d109437590d45a491.jpg)



Figure 6.29 Short sector performance 1994


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/2bf391224e6a68e5d646c00672770c390c25e31e6d7d64a61d934362a17e63ba.jpg)


The equities fared no better and many equity positions were entered throughout the year, both on the long and the short side, but the lack of overall trends in the equity markets caused nigh on all of them to end up in the red. This was a very frustrating year; even if you had had several good years behind you, this kind of year can cause you to question your strategy and in the worst cases even start making modifications to your strategy to better fit this particular type of year. To change the rules based on a bad year is a mistake however, and if the overall long-term strategy still seems sound a year like this should only make you more confident that the good times are near again. That is, however, much easier to write in a book than to do in reality, and there is no substitute for experience with these things. I can tell you for sure though, that if you have gone through a horrible year like this and managed to execute every trade, not changing any trading rules along the way, and then managed to fight back into profit the next year, you will have a whole new confidence in your strategy and your abilities and have moved a long way towards becoming a master of the trade. 

At the end of the year the long side had lost 12% and the short side 5% with the losses mainly being in the non-agricultural and the equity sector (see Figures 6.26 and 6.27). The agricultural sector and the rates managed to end in the positive, but too marginally for it really to matter. Fixed fees on the fund of course had to be paid, including paying the manager of the fund despite the bad results, but no performance fee. After the fixed fees the return for the investor was a whopping –16.5%, which was sure to cause some very angry and very worried phone calls. With the world equity markets up a few per cent while you were down over 16%, people started to ask questions. As long as you are making money, investors tend not to bother with the details about how you are making it, but once you have losses you notice who had properly understood the risks of the vehicle they had invested in and who had not. 

Personally I prefer to communicate often with my investors in good and bad months, making sure that they are aware of the overall strategy, risk level, positioning and attributions. A well-informed client is likely to stick with you after a drawdown such as this one, although no one is really happy here. But the client who had made lots of money on earlier years without properly understanding why and how is more likely to leave your fund before a year like 1994 is up. 

The year was full of false breakout signals in particular in the non-agricultural sector. The gold chart in Figure 6.30 shows how a typical trade looked in that sector. A short trade signal came along and we sold on what turned out to be practically the low before prices quickly moved up to the stop. 


Figure 6.30 Gold false breakout in 1994


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/b55c393b5bc82c5621662e665de7ae376da7e2d6c4b7ed0551d58ca21e4eeec5.jpg)



For this horrible year we naturally did not get any performance fee and so the costs of the fund were automatically lower than in the profitable years (see Tables 6.19 and 6.20). The net effect of interest income and costs was slightly positive and in the end the investors lost 15.4% in 1994.



Table 6.19 Sector performance 1994


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>0.2</td><td>1.1</td><td>-4.9</td><td>-4.8</td><td>-3.5</td><td>-11.8</td></tr><tr><td>Short</td><td>-1.3</td><td>0.8</td><td>-7.0</td><td>-3.2</td><td>6.1</td><td>-4.6</td></tr><tr><td>All</td><td>-1.1</td><td>1.9</td><td>-11.9</td><td>-8.0</td><td>2.6</td><td>-16.5</td></tr></table>


Table 6.20 Results 1994


<table><tr><td>Year</td><td>1994</td></tr><tr><td>Starting NAV</td><td>231.5</td></tr><tr><td>Trading result</td><td>-16.5%</td></tr><tr><td>Interest income</td><td>2.9%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.4%</td></tr><tr><td>Performance fee</td><td>0.0%</td></tr><tr><td>Net result</td><td>-15.4%</td></tr><tr><td>Ending NAV</td><td>195.9</td></tr></table>

## 1995

As we entered into the year in which Nick Leeson blew up Barings Bank and O.J. Simpson was set free to go and search for the real killer of his wife, the pressure was high having sustained significant losses of our investors’ money in the past 12 months. After being whipsawed time after time the portfolio had been decimated and there were not many surviving positions. All in all we now held 13 positions, 60% of which were in commodities and not a single equity position (see Tables 6.21 and 6.22 and Figure 6.31). 


Figure 6.31 Sector allocation 1995


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/5cad165517657a392e7c6cfaecd596baf7bedab57a8ba3c1cb4a48f03f8eb698.jpg)



Table 6.21 Initial portfolio 1995


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Cotton</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Lumber</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Australian dollar</td><td>Long</td><td>Currencies</td></tr><tr><td>Canadian dollar</td><td>Short</td><td>Currencies</td></tr><tr><td>Japanese yen</td><td>Short</td><td>Currencies</td></tr><tr><td>Copper</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Gold</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Silver</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Crude oil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Natural gas</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>US 2-year note</td><td>Short</td><td>Rates</td></tr><tr><td>Short sterling</td><td>Short</td><td>Rates</td></tr></table>


Table 6.22 Initial sector allocation 1995


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>1</td><td>2</td><td>3</td></tr><tr><td>Agricultural commodities</td><td>1</td><td>1</td><td>2</td></tr><tr><td>Non-agricultural commodities</td><td>1</td><td>5</td><td>6</td></tr><tr><td>Equities</td><td>0</td><td>0</td><td>0</td></tr><tr><td>Rates</td><td>0</td><td>2</td><td>2</td></tr><tr><td>Total</td><td>3</td><td>10</td><td>13</td></tr></table>

As Figure 6.32 shows, the year started rather uneventfully and after two months the return on the year was still hugging the zero line. Then there was a brief dip almost hitting –6% on the year and as this was just after the horrible 1994, you can be sure this was quite a white-knuckle ride. Then in March you finally got your reward for sticking to the strategy when the year returns not only hit the zero line again but also kept moving up month after month. The peak was hit in July when the fund had generated 25% since the start of the year and the investors who came in early 1994 had finally made their money back. Part of this return, however, was lost in the following months but the fund stayed around the +10% level until December when it made another mad dash to the upside, finally ending the year at +28.1% before fees. 


Figure 6.32 Strategy performance 1995


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/0dd67560678086a6b74dd343b1208bc08a876fa20b10cba0f4db64e99ab23e26.jpg)


The dip in February was caused in its entirety by the short side of the strategy with equities leading the losses, but that is not the most interesting observation to make for this year (see Figures 6.33 to 6.35 for the sector data). This was an unusual year in a way, because the profits and losses were driven completely by a single factor over the whole year. The only thing that really mattered this year was the long rates side. All other trades show negligible effect on the overall strategy. While the overall stock markets as measured by MSCI World had quite a good year, moving steadily and ending at a respectable +18%, there was not much money made by the long equity futures. 

Figure 6.33 Sector performance 1995 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/f2f054e47fb21c23d29a4219b23c5390442691904314c0757e77cd882d8313c0.jpg)



Figure 6.34 Long sector performance 1995


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/41f23890340c02df37accfba0071a9a653e5f270eaf4d6fc7293193728c92ea4.jpg)



Figure 6.35 Short sector performance 1995


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/d3c8fdfb34d86f940a386c76c257d0b3315bcf1a0036e0d9a4c9fc407534488d.jpg)


The fact of the matter is that practically all the returns this year came from being long rates. Everything from 3 month Eurodollar to 30 year US bonds were held and it paid off in spades. The other sectors more or less returned a net of zero, with no sector showing any significant gain or loss. 

This year shows the importance of having a strategy that has guaranteed entry into any important world trend. If you deal only in commodities or only in currencies, this would have been a flat year but since the strategy keeps trying everything, something is bound to work and the sectors that don’t tend to keep losses in acceptable ranges. Despite this being a very profitable year, it was at the same time a remarkably uneventful year. This may sound boring if you have not yet started trading diversified trend-following strategies, but after a few years you wish that a year like this would come along. 

The upwards trends in the fixed-income markets in 1995 were lasting and solid. As Figure 6.36 shows, some trades just kept ticking in money for over half a year at a time, constantly rising. 

## Figure 6.36 Long rates in 1995 – US 10 Year

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/7e6a5981847743c5447a85bb6d7adfbcad7e8567ab8975a7129b29cf61325d07.jpg)



Take a look at Tables 6.23 and 6.24. Perhaps you think that the performance fee in the latter table seems a little low for such a stellar year; that is absolutely so and by design. This is the effect of the high watermark rule which practically all hedge funds and other absolute return managers apply. We only get a performance fee when we hit new highs of the fund after all fees. This aligns the incentives of the hedgefund manager with the interests of the investor, or at least that is the theory. One could of course argue that it incentivises the fund manager to take on outsized risks, especially when he is in a drawdown, but I leave that debate alone here. Anyhow, because we had a big loss year in 1994, we needed to make that money back before we got paid any performance fees and in this year we just barely hit that mark and so the fees paid were quite modest.



Table 6.23 Sector performance 1995


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>1.4</td><td>8.2</td><td>3.5</td><td>3.7</td><td>26.9</td><td>43.7</td></tr><tr><td>Short</td><td>-3.3</td><td>-3.2</td><td>-4.4</td><td>-2.8</td><td>-2.1</td><td>-15.6</td></tr><tr><td>All</td><td>-1.9</td><td>5.0</td><td>-0.8</td><td>1.0</td><td>24.8</td><td>28.1</td></tr></table>


Table 6.24 Results 1995


<table><tr><td>Year</td><td>1995</td></tr></table>

Non-Agricultural Commodities, 26% 

<table><tr><td>Starting NAV</td><td>195.9</td></tr><tr><td>Trading result</td><td>28.1%</td></tr><tr><td>Interest income</td><td>4.8%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.7%</td></tr><tr><td>Performance fee</td><td>-1.9%</td></tr><tr><td>Net result</td><td>28.7%</td></tr><tr><td>Ending NAV</td><td>252.0</td></tr></table>

## 1996

The initial portfolio of 1996 was quite an aggressive one with 27 positions all in all and with a clear weighting towards long rates, long commodities and long dollar at the same time. Note that in the nonagricultural sector we were long energies and short metals though. We were also long equities, which should not be a big surprise given that we were now in the early Internet bubble stage of that segment of the markets (see Tables 6.25 and 6.26 and Figure 6.37). 


Figure 6.37 Sector allocation 1996


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/d13de89e0d8544415df43f34eec2838b4cb74961e13855c3d2a4f78a5e48ddf8.jpg)



Table 6.25 Initial portfolio 1996


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Corn</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Lean hogs</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Soybeans</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Sugar</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Wheat</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>British pound</td><td>Short</td><td>Currencies</td></tr><tr><td>Euro</td><td>Short</td><td>Currencies</td></tr><tr><td>Japanese yen</td><td>Short</td><td>Currencies</td></tr><tr><td>Dax</td><td>Long</td><td>Equities</td></tr><tr><td>Hang Seng</td><td>Long</td><td>Equities</td></tr><tr><td>Nikkei 225</td><td>Long</td><td>Equities</td></tr><tr><td>Crude oil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Heating oil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Palladium</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Platinum</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoline</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Silver</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Canadian Bankers’ Acceptance</td><td>Long</td><td>Rates</td></tr><tr><td>German Bund</td><td>Long</td><td>Rates</td></tr><tr><td>Eurodollar</td><td>Long</td><td>Rates</td></tr><tr><td>Euribor</td><td>Long</td><td>Rates</td></tr><tr><td>Euroswiss</td><td>Long</td><td>Rates</td></tr><tr><td>Long gilt</td><td>Long</td><td>Rates</td></tr><tr><td>Short sterling</td><td>Long</td><td>Rates</td></tr><tr><td>US 2-year note</td><td>Long</td><td>Rates</td></tr><tr><td>US 10-year note</td><td>Long</td><td>Rates</td></tr></table>


Table 6.26 Sector allocation 1996


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>0</td><td>3</td><td>3</td></tr><tr><td>Agricultural commodities</td><td>5</td><td>0</td><td>5</td></tr><tr><td>Non-agricultural commodities</td><td>4</td><td>3</td><td>7</td></tr><tr><td>Equities</td><td>3</td><td>0</td><td>3</td></tr><tr><td>Rates</td><td>9</td><td>0</td><td>9</td></tr><tr><td>Total</td><td>21</td><td>6</td><td>27</td></tr></table>

This was another tough year from a psychological point of view, marked by many frustrating situations. It was one of those years where it takes strong will power to keep running the strategy and not to make the mistake of overruling it. The first thing that happened was a sharp drop in January, down to –6% before even a full month had passed (see Figure 6.38). There is nothing to knock the wind out of you like getting 6% in the face in the first few weeks. Then when things started looking a little better in February and we were almost back to the zero line, another big drop came along and by mid-March we were down 10% on the year. At the same time the stock market was up a few per cent and the situation started to look worrying. 

Figure 6.38 Strategy performance 1996 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/c6fbfcc86657c205da50a033b294c7ddf0a9144d79658b63639686776047c5ce.jpg)


At this point, however, things started turning for us and in May we saw a spike up all the way to +12%, but the victory was short lived. After a quick fall down to +5% we moved sideways for a few months before falling back down under the zero line in August. At this point you were likely to feel the frustration of having worked so hard, having fought back from the depths of –10% all the way up to +12% only to lose it all and be back under the water again. 

As so often happens with trend-following strategies, when things look bleak the rescue is not far away. In September the trends finally kicked in and we got a nice smooth ride all the way up to +30%, which was of course a tremendous move in such short time. A sudden drop in the price in December still left 20% left on the table at year-end. 

Take a look at the sector numbers in Figures 6.39 to 6.41. The initial losses were driven by the commodities, both the agricultural and the non-agricultural ones and on the long side in particular. During the first month the long rates and equities in combination with the long dollar bets, or short bets on other currencies against the dollar if you will, managed to counteract the losses by the commodities to some extent and these sectors were responsible for the brief rebound in February. After these sectors also started suffering in late February and early March though, the whole fund received a hit and was pushed down to –10%. After the long rates took a beating in early March they were stopped out and remained out for much of the year. 


Figure 6.39 Sector performance 1996


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/ab7260d35882202a912ea58a2a77bcf3db1a03d427d844f5047d61312bdae6db.jpg)



Figure 6.40 Long sector performance 1996


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/90d272df8cfe61e436509070594e2834fb12378b9d812ac97d2a4e4b0ef1560f.jpg)



Figure 6.41 Short sector performance 1996


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/7e74b8db236de5506a30a98315611728ec8508dceb18bb56a1260b01c86cb47f.jpg)



The rough rice, along with several other agricultural commodities, had a nice run during late 1995 and early 1996 (see Figure 6.42). The trend accelerated quickly on the upside, adding up to a large part of the strategy’s profits during this time until the sharp reversal occurred, hitting its stops and exiting.


## Figure 6.42 Rough rice in 1996

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/81eb7fba2902c0de68acbf2763ac987d43c415b7ee0f909ec4403fc8c2cdfefe.jpg)


The rescue operation from these depths was led by the commodities and when this group got going, they really knew how to move. In April they all took off more or less at once: oil-based energies that were long went skyrocketing; metals that were short fell hard. At the same time the agricultural longs, from corn to rice to lumber all took off in a sharp rally and built quick profits for us. The peak of this run in the commodities was in May (see Figure 6.40) when most of them turned against us and stop after stop was hit, although the bulk of the profits was kept. 

The choppy sideways movement from May to July was a function of a lack of trends across sectors and the environment for trend-following profit making was simply not present. After having been up at double digit returns on the year and lost it all again, the trends finally returned to save the day. Two sectors led the assault on the upside: long non-agricultural commodities and long rates. After some time they also received backup from the long equities sector as the stock market picked up more and more. From being under the waterline in August, the bottom line of the fund rallied quickly on these three sectors and at the start of December we saw an astonishing 30% positive return on the year. 

The very design of this strategy, however, means that there will often be a big giveback of profits after a strong run, when the strongest sectors start reversing all at once. The exact same three sectors that led the rise all started losing their trends in December and before they hit their stops and were cut out the fund was down to +22.2% on the year (see Tables 6.27 and 6.28). Still, this should be considered a successful year and quite an exciting one at that. 


Table 6.27 Sector performance 1996


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>2.8</td><td>0.4</td><td>4.8</td><td>6.3</td><td>7.2</td><td>21.5</td></tr><tr><td>Short</td><td>2.4</td><td>-1.2</td><td>3.0</td><td>-0.1</td><td>-3.3</td><td>0.7</td></tr><tr><td>All</td><td>5.2</td><td>-0.8</td><td>7.8</td><td>6.2</td><td>3.8</td><td>22.2</td></tr></table>


Table 6.28 Results 1996


<table><tr><td>Year</td><td>1996</td></tr><tr><td>Starting NAV</td><td>252.0</td></tr><tr><td>Trading result</td><td>22.2%</td></tr><tr><td>Interest income</td><td>4.2%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.7%</td></tr><tr><td>Performance fee</td><td>-3.6%</td></tr><tr><td>Net result</td><td>20.5%</td></tr><tr><td>Ending NAV</td><td>303.8</td></tr></table>

So now after seven years of operation we have finally managed to triple the money of the initial investors and we have about 18% compound annual return. Investors who got in from the start and stuck with the fund should at this time be quite happy and the 20.5% return this year should give them confidence in the strategy. This was well needed, because unknown to you or your investors, you were both in for a very rocky year that would put your faith in the strategy to the test. 

## 1997

This year was smack in the middle of the biggest bubble period since the South Sea, with the financial community running all over each other to try to throw as much money as possible at teenagers who had found new clever ways to lose money on websites, and so one would be forgiven for thinking that this should be a great time for any trend follower. The fact of the matter is that although Internet stocks showed amazing trends, most other financial instruments lacked really clear trends to play and the volatility was quite high. The starting portfolio of 1997 was one of medium risk, holding 19 positions with quite a broad mix of sectors. Currencies and commodities were the highest weighted but the distribution between longs and shorts was quite even and the portfolio construction indicated a lack of strong market drivers (see Tables 6.29 and 6.30 and Figure 6.43). 


Figure 6.43 Sector allocation 1997


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/1054702854d433bf696ab668e0c1102af887d63b4552cd604f6100ffee049ab3.jpg)



Table 6.29 Initial portfolio allocation 1997


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Corn</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Live cattle</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Lean hogs</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Oats</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Rough rice</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>British pound</td><td>Long</td><td>Currencies</td></tr><tr><td>Canadian dollar</td><td>Short</td><td>Currencies</td></tr><tr><td>Euro</td><td>Short</td><td>Currencies</td></tr><tr><td>Japanese yen</td><td>Short</td><td>Currencies</td></tr><tr><td>Swiss franc</td><td>Short</td><td>Currencies</td></tr><tr><td>FTSE 100</td><td>Long</td><td>Equities</td></tr><tr><td>Nikkei 225</td><td>Short</td><td>Equities</td></tr><tr><td>Crude oil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Gold</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Platinum</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoline</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Silver</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Eurodollar</td><td>Long</td><td>Rates</td></tr><tr><td>Euribor</td><td>Long</td><td>Rates</td></tr></table>


Table 6.30 Initial sector allocation 1997


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>1</td><td>4</td><td>5</td></tr><tr><td>Agricultural commodities</td><td>3</td><td>2</td><td>5</td></tr><tr><td>Non-agricultural commodities</td><td>2</td><td>3</td><td>5</td></tr><tr><td>Equities</td><td>1</td><td>1</td><td>2</td></tr><tr><td>Rates</td><td>2</td><td>0</td><td>2</td></tr><tr><td>Total</td><td>9</td><td>10</td><td>19</td></tr></table>

This year was certainly not a fun year to be a futures manager and even though the year ended in positive territory, the path to get there was a tough one and sure to have taken its toll on the manager’s night sleep. Up until March things looked just dandy with long equities and long dollar bets driving the portfolio up 15% in the first three months (see Figure 6.44). So far there was no problem and everyone was smiling and doing the maths over and over again on how much the performance fee would be if the remaining three quarters also yielded 15% each. 

Figure 6.44 Strategy performance 1997 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/cbfb23d80db4251ff2e4015189855fa697e02ca92bfd642ace26d7030b08f95f.jpg)



In late March, the roller coaster of death started and we were quickly plunged down from +15% to +5% and then down to 0% before heading down to a few per cent in the minus. Some might say that having had profits and losing them is worse than never having had them at all. Having lost a year profit of 15% was a tough thing to bear and by mid-year we had nothing at all to show for our hard work. The next couple of months chugged along sideways around the zero line before the profits finally came in again, courtesy of the long equity futures.


Unfortunately the party did not last long and the hangover was even harsher this time. Having finally clawed our way back up to reach +10%, the drop-down was fast and hard as equities corrected down and already in September we were down 5% year to date again and not a smile in the house. It got even worse by November, when a sudden drop in rates and non-agricultural commodities pushed the fund all the way down to –6.5% on the year, which was of course over 20% away from where we had been back in March. Lucky for us, the strength of the US dollar came to the rescue and our short currency futures started kicking in big time. At the same time the trends turned in our favour for both agricultural and nonagricultural commodities and after a quick rush to the upside we finished the year at about +6.4%. Sure, it was a positive year in the end but a mere 6% and change was clearly insufficient reward to pay for the volatility we saw throughout this horrible year. 

At the end of the day the bulk of the profits was created by the short currency futures, which in essence translated to long dollar bets as most of the currency futures trade against the dollar. We did make money on being long equities in the roaring bull market but not enough to pay for the losses in the commodities and rates sectors (see Figures 6.45 to 6.47). 

Figure 6.45 Sector performance 1997 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/9c03c445d61041c0106fedc26ef988d515ae61327c9f5e867f96af822355d5f5.jpg)



Figure 6.46 Long sector performance 1997


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/d3391234031d18ee1806d6d81faf57fc0317f234d10da949de6c22f8980fe50d.jpg)



Figure 6.47 Short sector performance 1997


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/ac6dd90c79a6ee51cfad326267145a8eceb200453bcccc9d8ad2a039b3993149.jpg)


One of the currency trades that saved the performance by the end of the year was the short Japanese Yen (see Figure 6.48). Entered in early September, the Yen trade went mostly sideways for a couple of months before it started generating real profits. This and similar short currency bets ended up making the big difference in the final months of the year. 


Figure 6.48 Short Japanese yen in 1997


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/b07cd8a23a9dbe5f29f49b6b71eaabb6a6789059aae579cbf4939db87a34bd2b.jpg)



As Tables 6.31 and 6.32 state, the profits ended at around 7.4%, which became 11.5% after interest income was counted in. But someone had to pay for the lights in the office and the food the manager ate, and after all costs including performance fee were taken care of there was only 8.0% remaining for our esteemed investors and half of that was interest income that they could have received taking much lower risks given the interest-rate climate. The chances that they were very happy with this gain were not great, and so we had to pick up the performance a bit or the redemptions forms would have started filling up the mailbox.



Table 6.31 Sector performance 1997


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>-1.8</td><td>-3.9</td><td>-2.2</td><td>5.5</td><td>-1.2</td><td>-3.5</td></tr><tr><td>Short</td><td>11.4</td><td>-0.7</td><td>-0.5</td><td>2.8</td><td>-2.2</td><td>10.9</td></tr><tr><td>All</td><td>9.6</td><td>-4.5</td><td>-2.6</td><td>8.4</td><td>-3.4</td><td>7.4</td></tr></table>


Table 6.32 Results 1997


<table><tr><td>Year</td><td>1997</td></tr><tr><td>Starting NAV</td><td>303.8</td></tr><tr><td>Trading result</td><td>7.4%</td></tr><tr><td>Interest income</td><td>4.1%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.6%</td></tr><tr><td>Performance fee</td><td>-1.4%</td></tr><tr><td>Net result</td><td>8.0%</td></tr><tr><td>Ending NAV</td><td>328.0</td></tr></table>

## 1998

The pressure was on as 1998 started because we had just left a year that we cannot honestly be satisfied with. The initial portfolio consisted of 25 positions across all sectors with a clear tilt toward the short side, with the exception of the rates sector (see Tables 6.33 and 6.34 and Figure 6.49). We were short several currency futures, which translates as saying that we were still long the dollar as we were during 1997. At the same time we were short both agricultural commodities and energies and net short equities as well. The last part might seem odd and even more odd that we were short the Nasdaq during the 1990s, but there was a period in late 1997 when even this market had not only slowed down but also even reversed enough to trigger a short trade. 

## Figure 6.49 Sector allocation 1998

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/eb4af8c69ea4ae80987a29673ddbd33c2dc5bf1c47cd85e9ed7cb2f54410e890.jpg)



Table 6.33 Initial portfolio 1998


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Cotton</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Lumber</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Live cattle</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Lean hogs</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Oats</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Wheat</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Australian dollar</td><td>Short</td><td>Currencies</td></tr><tr><td>Canadian dollar</td><td>Short</td><td>Currencies</td></tr><tr><td>Euro</td><td>Short</td><td>Currencies</td></tr><tr><td>Japanese yen</td><td>Short</td><td>Currencies</td></tr><tr><td>DAX</td><td>Long</td><td>Equities</td></tr><tr><td>Nasdaq 100</td><td>Short</td><td>Equities</td></tr><tr><td>Nikkei 225</td><td>Short</td><td>Equities</td></tr><tr><td>Crude oil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Copper</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Heating oil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Natural gas</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>German Bund</td><td>Long</td><td>Rates</td></tr><tr><td>German Schatz</td><td>Long</td><td>Rates</td></tr><tr><td>Euroswiss</td><td>Long</td><td>Rates</td></tr><tr><td>Long gilt</td><td>Long</td><td>Rates</td></tr><tr><td>Short sterling</td><td>Short</td><td>Rates</td></tr><tr><td>US 2-year note</td><td>Long</td><td>Rates</td></tr><tr><td>US 10-year note</td><td>Long</td><td>Rates</td></tr></table>


Table 6.34 Initial sector allocation 1998


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>0</td><td>4</td><td>4</td></tr><tr><td>Agricultural commodities</td><td>0</td><td>6</td><td>6</td></tr><tr><td>Non-agricultural commodities</td><td>0</td><td>5</td><td>5</td></tr><tr><td>Equities</td><td>1</td><td>2</td><td>3</td></tr><tr><td>Rates</td><td>6</td><td>1</td><td>7</td></tr><tr><td>Total</td><td>7</td><td>18</td><td>25</td></tr></table>

The second to last year of the 1990s was a very interesting one for several reasons, not least of which being the bankruptcy of a former world super power and the spectacular implosion of a massive hedge fund run by a bunch of people who won Nobel Prizes for supposedly figuring out how the markets really work. 

The first little shake early in the year felt pretty bad at the time, but in the context of the year it was hardly worth remembering (see Figure 6.50). In January the profits ran up to +7.5% in a couple of weeks, only to give it all back again; these things are always very tough when they happen, especially after a bad run like the previous year. After that however, the real fun began. The year 1998 was one of those incredible years that come along once a decade or so for trend followers and this was a year to remember for a long time. From zero in February, the fund went in a smooth line up slightly above 10%, sideways choppy for a few months and then a spike up to +30%. When the profits started dropping soon after that the painful memories from last year’s giveback periods were sure to come up but this one was not quite as dramatic. The trends gained strength again after the pullback, moving smoothly back up to +30% before making another crazy acceleration all the way up to +42% in a matter of days. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/83b2ee09f1aaff2575722b45790bd6fca96cc7002f5a97ad6bdacb40fae0a091.jpg)


Again the decline halted after giving up only 10% and the rally continued once more. A third insane dash upwards started in October and peaked at +53%, at which point anyone would be tempted to close or reduce positions to make sure the big gain was not given back before year end. These overrides are rarely a good idea though and if you had stuck to the strategy, you would see that it took care of itself. We again gave up a little more than 10%, but the ensuing rally pushed the performance for the fund back up to the 50% line before the year was finished. This was truly an amazing year and even though it was highly profitable it was still a very mentally exhausting year and the sharp reversals wreaked havoc on most people’s nerves. 

Figures 6.51 to 6.53 show that although there were many contributors to the positive end of year result, the long rates and the short agricultural commodities were together responsible for 42% of the total 52% and thereby completely dominated the year. 


Figure 6.51 Sector performance 1998


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/2df6e4816ae933d30617eb907e55ed315f334ccd93588cda02878d5bff3e0190.jpg)



Figure 6.52 Long sector performance 1998


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/350a2afd37b4af962e4dd1e90a20ed700da6fdbe44e3a2b28cb86252e613f4c1.jpg)



Figure 6.53 Short sector performance 1998


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/395e3573993733e83e05d89185bf1ee0143381651573b8b965b416997a65307f.jpg)


The short oats was one of several very profitable trades in the agricultural sector this year (see Figure 6.54). The trade was entered in December of 1997 and continued to trend firmly down until the trend acceleration in April. As the prices moved quickly in our favour, the stop point moved in closer and on the rebound the position was exited. This is the safety mechanism to make sure we don’t give back too much profit when the trends do turn. In this case, the trend continued down and after having missed out on a few days decline, we re-entered the short trade and rode it successfully all the way to October. 

Figure 6.54 Short oats in 1998 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/f4d765e966b4f32b7cd97c5c0adeba715d7421ce4b5e2543998dedf6a2f67fcc.jpg)


After such an amazing year the manager got a pretty nice piece of the overall pie (see Tables 6.35 and 6.36). The combined management and performance fee received for this year was equivalent of almost 9% of the initial assets and while that may seem excessive to some, remember that this is a function of the extreme success seen this particular year and that as of this year an investor who came in at the start of 1990 with US$100,000 now had US$500,000 worth of the fund. 


Table 6.35 Sector performance 1998


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>-1.6</td><td>-3.1</td><td>2.0</td><td>10.3</td><td>26.7</td><td>34.2</td></tr><tr><td>Short</td><td>1.0</td><td>15.1</td><td>3.7</td><td>-0.6</td><td>-1.4</td><td>17.7</td></tr><tr><td>All</td><td>-0.6</td><td>12.0</td><td>5.7</td><td>9.6</td><td>25.3</td><td>51.9</td></tr></table>


Table 6.36 Results 1998


<table><tr><td>Year</td><td>1998</td></tr><tr><td>Starting NAV</td><td>328.0</td></tr><tr><td>Trading result</td><td>51.9%</td></tr><tr><td>Interest income</td><td>4.9%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.9%</td></tr><tr><td>Performance fee</td><td>-8.1%</td></tr><tr><td>Net result</td><td>46.1%</td></tr><tr><td>Ending NAV</td><td>479.3</td></tr></table>

## 1999

Closing a stellar year like 1998 is always a great feeling, and the memories of the horrible 1997 experience were long gone. The initial portfolio looked as one might expect after seeing the results of late 1998, with the sectors that carried the profits that period being the heaviest weights going into this year (as shown in 

Tables 6.37 and 6.38 and Figure 6.55). We were long rates, short commodities and long equities in a very clear portfolio. Note that the long rates were concentrated in Europe and that the short commodities were across the board, with everything from corn to crude to gold being held short. 


Figure 6.55 Sector allocation 1999


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/6797d47bf4533a81c8f1b33586f0fccf74194689b4ebcdcbce987097d31e0d56.jpg)



Table 6.37 Initial portfolio 1999


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Corn</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Cotton</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Lumber</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Oats</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Rough rice</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Soybeans</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Sugar</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Wheat</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Canadian dollar</td><td>Short</td><td>Currencies</td></tr><tr><td>Japanese yen</td><td>Long</td><td>Currencies</td></tr><tr><td>CAC 40</td><td>Long</td><td>Equities</td></tr><tr><td>FTSE 100</td><td>Long</td><td>Equities</td></tr><tr><td>Nasdaq 100</td><td>Long</td><td>Equities</td></tr><tr><td>S&amp;P 500</td><td>Long</td><td>Equities</td></tr><tr><td>Crude oil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gold</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Copper</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Natural gas</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Palladium</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoline</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>German Bund</td><td>Long</td><td>Rates</td></tr><tr><td>German Schatz</td><td>Long</td><td>Rates</td></tr><tr><td>Euribor</td><td>Long</td><td>Rates</td></tr><tr><td>Long gilt</td><td>Long</td><td>Rates</td></tr><tr><td>Short sterling</td><td>Long</td><td>Rates</td></tr></table>


Table 6.38 Initial sector allocation 1999


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>1</td><td>1</td><td>2</td></tr><tr><td>Agricultural commodities</td><td>1</td><td>7</td><td>8</td></tr><tr><td>Non-agricultural commodities</td><td>1</td><td>6</td><td>7</td></tr><tr><td>Equities</td><td>4</td><td>0</td><td>4</td></tr><tr><td>Rates</td><td>5</td><td>0</td><td>5</td></tr><tr><td>Total</td><td>12</td><td>14</td><td>26</td></tr></table>

The last year of the 1990s was a very tough one for our trend-following approach and another one of those years where you had plenty of time to ponder your career choice. The first quarter of the year was more or less sideways within the range of plus/minus about 4% (see Figure 6.56). Then in late May the fund took quite a big and sudden hit, falling down to –8% on the year before slowly starting to regain ground. By July a short burst in the profits managed to get the fund back up above the zero line and all the way up to +6% but this was a short-lived victory. The dropdown again was hard and brutal and in a matter of days the fund had lost almost 10%. At this time the mood around the office was not too good and in the next few months the equity curve just bobbed up and down over the zero line, which created constant hope of recovery followed by fear of big losses. 


Figure 6.56 Strategy performance 1999


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/164bf8ad731462d54e77ee7c025fc29f3ad804d09a9625e6a3086681861e6993.jpg)


In early October you had no profits on the books at all and a volatile nine months behind you and just as things felt like they could not get much worse, they did. The losses started mounting up and after week after week of losing money you found yourself at –10% in November and the situation looked dire. The year was almost over, you had had a roller coaster up and down and the only thing you had to show for it was a big hole in the pocket. The year was not over though and by mid-November the losses started decreasing steadily and finally hit the zero line again in December. But it did not stop there and before the year finished the fund managed to close at +5% on the year. A return of 5% after such a volatile ride, and when the world stock market just made a 25% profit year, was almost an insult, but at least we made the money back for the investors. 

Figures 6.57 to 6.59 contain the sector data. The only sector that did well throughout the year was the short agricultural commodities, which is why this year ultimately ended in positive territory and the reason behind the sudden gains by mid-year. The non-agricultural commodities, however, had a pretty bad year, especially on the short side. 


Figure 6.57 Sector performance 1999


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/ff5848d7875980d9b20416629e37d7be3b9e7db8f3fb4bd7300c8a143326d2d7.jpg)



Figure 6.58 Long sector performance 1999


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/4628e26866674b0289bf17167e308f0ea7a215cfdaac099a81683ba5026c8b30.jpg)



Figure 6.59 Short sector performance 1999


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/db2f6a1741501fceda667078f5afaa8b7b96cabf3308d00c89d9003b46618237.jpg)



The only other sector that had a positive contribution this year was the end of year rally in the equity markets. The other sectors were mostly bad throughout the year with some showing temporary profits that had evaporated before the end of December.


Most people remember the last year of the 1990s for the final push of the incredible tech boom, but in fact (as Figure 6.60 shows) most of that year showed little to no real usable trend in the Nasdaq. The final rally that started in October was very profitable, but before that the price moves were choppy and hard to make money from. The tech index had many false breakouts followed by sharp corrections, which triggered exit signals and the strategy ended up overtrading and mostly losing money up until that final big move up. 


Figure 6.60 Nasdaq trades during 1999


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/a63b94f5a8f4461d76d3925267cf2ef8cc9e41f290a710f15edfd193f0cf5622.jpg)



A bad year to be sure, but the end result after all fees was still about 7.3% (see Tables 6.39 and 6.40). Although this was still in positive territory, investors may not feel that this was enough reward for the volatility they suffered and not in such a high-interest rate environment. The fact that the world stock markets were up almost 25% certainly does not mitigate their concerns. This was at the height of the tech bubble and it was a hard sale to explain why investors should stay with you and not put all their money in Internet stocks.



Table 6.39 Sector performance 1999


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>-6.4</td><td>1.1</td><td>0.7</td><td>11.4</td><td>-3.3</td><td>3.5</td></tr><tr><td>Short</td><td>3.1</td><td>6.8</td><td>-3.7</td><td>-3.2</td><td>0.3</td><td>3.3</td></tr><tr><td>All</td><td>-3.3</td><td>7.8</td><td>-3.0</td><td>8.3</td><td>-3.0</td><td>6.8</td></tr></table>


Table 6.40 Results 1999


<table><tr><td>Year</td><td>1999</td></tr><tr><td>Starting NAV</td><td>479.3</td></tr><tr><td>Trading result</td><td>6.8%</td></tr><tr><td>Interest income</td><td>3.8%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.6%</td></tr><tr><td>Performance fee</td><td>-1.3%</td></tr><tr><td>Net result</td><td>7.3%</td></tr><tr><td>Ending NAV</td><td>514.1</td></tr></table>


2000


Despite all the doomsday warnings, not much happened when the computer clocks flipped over from 1999 to 2000 on New Year’s Eve. We entered the year with a risk portfolio holding 32 positions spread out quite evenly on all sectors (see Tables 6.41 and 6.42 and Figure 6.61). The bet taken on by the strategy was historically high and if you break it down to the basics, the bet this year was short agricultural commodities, long non-agricultural commodities and long equities. The rates and currency positions were not as one-sided but with the two commodity sectors and the equities were very clear outright bets. Now what could possibly go wrong with being heavily long equities at the start of 2000? 


Figure 6.61 Sector allocation 2000


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/3206d2cc63415ee67c628bbcd9eb67513667429e1be74293f7872421ce436e37.jpg)



Table 6.41 Initial portfolio 2000


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Corn</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Cotton</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Lean hogs</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Oats</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Rough rice</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Soybeans</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Sugar</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Wheat</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Canadian dollar</td><td>Long</td><td>Currencies</td></tr><tr><td>Euro</td><td>Short</td><td>Currencies</td></tr><tr><td>Japanese yen</td><td>Long</td><td>Currencies</td></tr><tr><td>Euro/Pound</td><td>Short</td><td>Currencies</td></tr><tr><td>EUR/JPY</td><td>Short</td><td>Currencies</td></tr><tr><td>Swiss franc</td><td>Short</td><td>Currencies</td></tr><tr><td>CAC 40</td><td>Long</td><td>Equities</td></tr><tr><td>DAX</td><td>Long</td><td>Equities</td></tr><tr><td>FTSE 100</td><td>Long</td><td>Equities</td></tr><tr><td>Hang Seng</td><td>Long</td><td>Equities</td></tr><tr><td>Nasdaq 100</td><td>Long</td><td>Equities</td></tr><tr><td>S&amp;P 500</td><td>Long</td><td>Equities</td></tr><tr><td>EuroStoxx 50</td><td>Long</td><td>Equities</td></tr><tr><td>Crude oil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Copper</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Heating oil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Palladium</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Platinum</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoline</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Eurodollar</td><td>Short</td><td>Rates</td></tr><tr><td>Euroswiss</td><td>Long</td><td>Rates</td></tr><tr><td>US 10-year note</td><td>Short</td><td>Rates</td></tr><tr><td>US 2-year note</td><td>Short</td><td>Rates</td></tr></table>


Table 6.42 Initial sector allocation 2000


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>2</td><td>4</td><td>6</td></tr><tr><td>Agricultural commodities</td><td>1</td><td>7</td><td>8</td></tr><tr><td>Non-agricultural commodities</td><td>7</td><td>0</td><td>7</td></tr><tr><td>Equities</td><td>7</td><td>0</td><td>7</td></tr><tr><td>Rates</td><td>1</td><td>3</td><td>4</td></tr><tr><td>Total</td><td>18</td><td>14</td><td>32</td></tr></table>

As you have made it this far into the book, I doubt you will be surprised that 2000 turned out to be a very eventful year (see Figure 6.62). The horror started on the second day of trading when the fund suddenly found it had lost 6% even before the hangover from the New Year’s Eve party had subdued. A week into the New Year and the loss had risen to 12% and now it was no longer any fun. The big hit was of course in the long equity portfolio with our seven positions in that theme taking a beating at the same time. Most sectors have a tendency to build high internal correlations during market turbulence but the equity sector tends to reach far more extreme levels, which is when you get these kinds of hits in that particular sector. 


Figure 6.62 Strategy performance 2000


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/06f2c114fa52c5cb0392b162741cab1e4246b4cde05037d92fe1a495a56b62c8.jpg)


For the remainder of the first quarter the fund slowly regained its losses, much to the credit of the long non-agricultural commodities, and by the middle of March we finally reached that coveted zero line again. But 2000 was no ordinary year and another sharp decline in the equity markets sent our fund plummeting down to –15% on the year, and this was at a time when the world equity markets were only marginally down on the year. As we were stopped out of most long equity positions and the currency bets took over the driver seat, we started regaining ground again in May, peaking up above the zero line briefly before falling back down to –10% in June. 

After this the short agricultural commodities kicked in and with the help of the currencies and nonagricultural commodities we managed to reach marginally into the double digit profits at +11% in September, but the victory was not long lasting. In two sharp moves down, fuelled by long equity positions as well as profit givebacks in the commodities, the fund hit a low of –5% in November and again we found ourselves in a position of having a negative performance number with only one month to go. This year we were saved by the long rates, and as the equity markets started falling hard after our exposure to that sector was already closed, we gained big on our long rates positions and the year ended at a respectable +14%, leaving the equity market very far behind. 

The equities trading ended up losing on both longs and shorts in a very volatile year and the total loss on this sector turned out to be a rather dramatic 18.5% on the whole fund (see Figure 6.63). At the same time all other sectors ended the year in positive territory and thanks to the strong results of the non-agricultural commodities and the rates (see Figure 6.64) we can still show the investors a good return on the year. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/74c930b33fcdf47ca42feee85be1d2fba69a3195041ed007ad95667620d1591c.jpg)



Figure 6.64 Long sector performance 2000


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/87f4f21800d387964ad9c744862fd913a35d3bca1627926bbc89242f5e28916b.jpg)


For most of 2000 the dollar rallied strongly and that meant we were generally short foreign currency futures against the US dollar (see Figure 6.65). The Cable, British pound against the dollar, was one of the highly profitable trades during this period (as shown in Figure 6.66). 


Figure 6.65 Short sector performance 2000


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/63e6ba64089f0b55767a98957d9d7a1a221ff81a9217a93e77639220ae978a64.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/4c32e99707a98547213d93c134f80465dc259349183b5178ead4e4c09631bb34.jpg)


After all fees the net result for the fund’s investors landed at 14.2%, shy of 15% even, but in a year like 2000 you were not likely to get many complaints. As stated, most investors tend to compare returns to the stock markets and the average investor in that market just lost 15% while the people who held onto tech stocks lost substantially more, and so these results don’t look too bad after all (see Tables 6.43 and 6.44). 


Table 6.43 Sector performance 2000


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>-2.5</td><td>0.0</td><td>13.2</td><td>-15.3</td><td>12.7</td><td>8.1</td></tr><tr><td>Short</td><td>7.5</td><td>3.1</td><td>0.0</td><td>-3.2</td><td>-1.4</td><td>5.9</td></tr><tr><td>All</td><td>5.0</td><td>3.1</td><td>13.2</td><td>-18.5</td><td>11.3</td><td>14.0</td></tr></table>


Table 6.44 Results 2000


<table><tr><td>Year</td><td>2000</td></tr><tr><td>Starting NAV</td><td>514.1</td></tr><tr><td>Trading result</td><td>14.0%</td></tr><tr><td>Interest income</td><td>4.8%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.6%</td></tr><tr><td>Performance fee</td><td>-2.5%</td></tr><tr><td>Net result</td><td>14.2%</td></tr><tr><td>Ending NAV</td><td>586.9</td></tr></table>

## 2001

As in the previous year, the starting portfolio of 2001 was quite a risky one with 33 positions in total. It is very clear from just a quick overview how this portfolio was tilted (see Tables 6.45 and 46 and Figure 

6.67). The equity and rates exposure should speak a clear message about the state of the global markets in 2001. There were seven short equity positions and no longs and at the same time we held eight long rates positions with no shorts. This was an aggressive bear market portfolio that potentially could lose big, if the market turned to the upside. The currency bets were reasonably spread and not too concentrated and the two agricultural sectors held various side bets to the big theme of the global bear market, providing some much needed diversification. 


Figure 6.67 Sector allocation 2001


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/1fa54f75056b5e03ffe7568eb8ab5716d886587c924ed3872b58e91d65c51f36.jpg)



Table 6.45 Initial portfolio 2001


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Soybeans</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Wheat</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Corn</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Cotton</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Rough rice</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Oats</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Lumber</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Live cattle</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Swiss franc</td><td>Long</td><td>Currencies</td></tr><tr><td>EUR/GBP</td><td>Long</td><td>Currencies</td></tr><tr><td>Japanese yen</td><td>Short</td><td>Currencies</td></tr><tr><td>EUR/JPY</td><td>Long</td><td>Currencies</td></tr><tr><td>EuroStoxx 50</td><td>Short</td><td>Equities</td></tr><tr><td>FTSE 100</td><td>Short</td><td>Equities</td></tr><tr><td>DAX</td><td>Short</td><td>Equities</td></tr><tr><td>Nikkei 225</td><td>Short</td><td>Equities</td></tr><tr><td>S&amp;P 500</td><td>Short</td><td>Equities</td></tr><tr><td>CAC 40</td><td>Short</td><td>Equities</td></tr><tr><td>Nasdaq 100</td><td>Short</td><td>Equities</td></tr><tr><td>Natural gas</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Platinum</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Silver</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Palladium</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Long gilt</td><td>Long</td><td>Rates</td></tr><tr><td>German Bund</td><td>Long</td><td>Rates</td></tr><tr><td>Euribor</td><td>Long</td><td>Rates</td></tr><tr><td>Euroswiss</td><td>Long</td><td>Rates</td></tr><tr><td>German Schatz</td><td>Long</td><td>Rates</td></tr><tr><td>Canadian Bankers’ Acceptance</td><td>Long</td><td>Rates</td></tr><tr><td>US 10-year note</td><td>Long</td><td>Rates</td></tr><tr><td>Short sterling</td><td>Long</td><td>Rates</td></tr><tr><td>US 2-year note</td><td>Long</td><td>Rates</td></tr><tr><td>Eurodollar</td><td>Long</td><td>Rates</td></tr></table>


Table 6.46 Initial sector allocation 2001


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>3</td><td>1</td><td>4</td></tr><tr><td>Agricultural commodities</td><td>3</td><td>5</td><td>8</td></tr><tr><td>Non-agricultural commodities</td><td>3</td><td>1</td><td>4</td></tr><tr><td>Equities</td><td>0</td><td>7</td><td>7</td></tr><tr><td>Rates</td><td>10</td><td>0</td><td>10</td></tr><tr><td>Total</td><td>19</td><td>14</td><td>33</td></tr></table>

The first quarter of 2001 seemed eventful at the time but few would really remember those months if asked a year later. The fund was up 5% at first, then turning down to stay at around –5% for a couple of months (as Figure 6.68 shows). April saw a short-lived burst in profits where the year-to-date return rose to +10% before it was lost a month later. In fact, all the way up to September of this year things seemed rather mediocre. Having had two bad years behind us, the pressure to perform was high and being in the ninth month of the year without any profits again was enough to shake the steadiest nerves. This is exactly the reason why there are not more long-lasting, successful trend-following futures funds. If you are persistent and trust your strategy you will make very good returns over the long run, but you need to endure these kinds of periods where it is very easy to start doubting, overriding or losing enough clients to be forced to shut down. 

## Figure 6.68 Strategy performance 2001

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/5834babb4c861877f2f8dcaa30fe2e647300c94a33c3774b4bfffa9bd0d6c357.jpg)


The only redeeming factor this year up until September was that the world equity markets were down quite a bit and our strategy was still around zero. The fact of the matter is that we had at that time made very good money on being short equity markets as well as on the short agricultural commodities, but it was all eaten up by the other sectors. But then in September, the long rates finally took off in a big way, sending the fund on an amazing ride up to +30% in just weeks. After a short breather we even saw +50% on the year in November before backing down a little to end at around +42%. The pullback by the end of the year was caused by the year-end rally, which caused losses on the short equities and long rates and triggered many stop losses. 

This is, as I am sure you have seen by now, a common way in which trend-following futures make money. You get a long period of mediocre returns at high volatility and then suddenly huge bursts of profits that make up for the dull periods. As I have tried to show, this game is not for everyone, despite the fact that it is not terribly difficult from a purely technical perspective. 

Although the net of what I would classify as side bets in the two commodity sectors and the currencies did pay off with about 3%, this year the performance was completely driven by the large bear market bets (see Figures 6.69 to 6.71). Given how strong the bear market was at this time that is not very surprising. Of course, what you need to be aware of is that when trends grow this strong, the strategy will pile up quite a large amount of risk on bets related to the same theme and build a corner portfolio. This is how the big profits are made but it also means that when things turn it will be painful very quickly. This is all part of the game. 


Figure 6.69 Sector performance 2001


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/193dc2448a4d2e01f6bb31250b7327caf4b7e45ec13a8c6e6394e5fe373aa64a.jpg)



Figure 6.70 Long sector performance 2001


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/27f1375a10646c6a6fbe6b8eb7ea3655099dbbd279c0bf6b73c3b37d2bc15208.jpg)



Figure 6.71 Short sector performance 2001


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/0020c8bc28f3a031d876f2a338272cd3bfcf6b0fa548fde72f366031e3b60654.jpg)



The German Bund trade (shown in Figure 6.72) was typical for the rates sector this year and demonstrates what happens when prices gap far below your stop point. Having been in the position for some time, the profits were adding up to large amounts by November after the yields were hitting the lows. As the whole rates sector had a shock reversal in mid-November, the prices quickly fell and gapped down far below our theoretical stop point. As we only trade on end of day data, this had to be accounted for and the position was not closed until the following day at even lower prices. In the short run these situations are highly frustrating but the position was still closed with a good profit.


Figure 6.72 German Bund experiencing a quick reversal in 2001 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/661d43e3413dafd03f198aa0d2f610b89c126aef52b60b7b6f7eb1186e5850ac.jpg)



This was indeed a very profitable year, both for the investors who got a return of 36.2% after all costs and for the fund manager who received a substantial remuneration (see Tables 6.47 and 6.48). The performance fee of 15% of all profits after costs turned out to be a total of almost 6.5% of the initial money under management as of start of the year. This may sound very steep but those are the rules of the game and when clients receive such a stellar return in a year when most people lost large amounts, they are probably not in the mood to make complaint phone calls.



Table 6.47 Sector performance 2001


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>-1.9</td><td>-2.2</td><td>-5.0</td><td>0.0</td><td>20.0</td><td>10.9</td></tr><tr><td>Short</td><td>1.5</td><td>11.0</td><td>0.6</td><td>18.3</td><td>-0.5</td><td>31.0</td></tr><tr><td>All</td><td>-0.3</td><td>8.7</td><td>-4.4</td><td>18.3</td><td>19.5</td><td>41.8</td></tr></table>


Table 6.48 Results 2001


<table><tr><td>Year</td><td>2001</td></tr><tr><td>Starting NAV</td><td>586.9</td></tr><tr><td>Trading result</td><td>41.8%</td></tr><tr><td>Interest income</td><td>3.1%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.8%</td></tr><tr><td>Performance fee</td><td>-6.4%</td></tr><tr><td>Net result</td><td>36.2%</td></tr><tr><td>Ending NAV</td><td>799.1</td></tr></table>

Take note of how the interest income has gone down from the previous years, because the money market yields were falling and becoming less profitable for us. But then again, as long as the performance is as good as this year, it should not matter much, right? Well, let’s see about that. 

## 2002

It may seem surprising to see how small the initial portfolio of 2002 was given how it had looked entering the past few years. We had only nine positions left and the reason was that during the last couple of months of 2001 a large number of stop losses were triggered, causing the fund to lose some performance but also drastically reduce risk (see Tables 6.49 and 6.50 and Figure 6.73). We had no equity positions at all left in the fund and only two long rates futures, and so in essence our bear market portfolio was liquidated and we now held a small portfolio of various side bets. 


Figure 6.73 Sector allocation 2002


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/8e9ff85800f9aa41958b6f7c3570c9bc8450d7ca4a580a1033bdbeae9afbd89a.jpg)



Table 6.49 Initial portfolio 2002


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Soybeans</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Corn</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>EUR/GBP</td><td>Short</td><td>Currencies</td></tr><tr><td>Japanese yen</td><td>Short</td><td>Currencies</td></tr><tr><td>EUR/JPY</td><td>Long</td><td>Currencies</td></tr><tr><td>Gold</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Natural gas</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Canadian Bankers’ Acceptance</td><td>Long</td><td>Rates</td></tr><tr><td>Eurodollar</td><td>Long</td><td>Rates</td></tr></table>


Table 6.50 Initial sector allocation 2002


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>1</td><td>2</td><td>3</td></tr><tr><td>Agricultural commodities</td><td>0</td><td>2</td><td>2</td></tr><tr><td>Non-agricultural commodities</td><td>0</td><td>2</td><td>2</td></tr><tr><td>Equities</td><td>0</td><td>0</td><td>0</td></tr><tr><td>Rates</td><td>2</td><td>0</td><td>2</td></tr><tr><td>Total</td><td>3</td><td>6</td><td>9</td></tr></table>

After the rather dramatic performance of the end of the previous year this year may at first seem a bit on the slow side. The performance fell below the surface quite soon after the year began and slowly kept moving down more and more until early summer (check out Figure 6.74). At the worst point we saw a drawdown on the year of –12%, which was not exactly good but after the stellar performance of last year not horrible either. 


Figure 6.74 Strategy performance 2002


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/cc87af03c8b75c7b5a0d0b3a959cb13cbd6f9def28de5daa8515deae9aef642f.jpg)


In early June, however, something started happening. The rally that closed 2001 was over by January of 2002 and the markets turned down again, but it always takes a while for our trend-following strategy to kick in and join the crowd. In June we really moved back into the bear market portfolio in scale and the profits were not far behind. From being at double digit negative performance on the year the fund started trending upwards in a nice smooth ascent driven by long rates, long currencies and short equities (see Figures 6.75 to 6.77), and month after month we set new highs. By August the performance year to date was already +30% and in October we almost reached +40%. The sharp rally in October caused some damage and the fund quickly fell back from that level to only having 20% profit on the year. This may sound almost trivial in the context but a loss of 20% performance in a couple of weeks is no laughing matter when it happens. Despite the profits still held, it can cause both you as the manager and your clients to start doubting the process and wondering whether something had changed in the markets that could have caused the strategy to cease working. The fact is that this is a rather normal behaviour and the cost of doing business in this field. 

## Figure 6.75 Sector performance 2002

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/3725b3900e140310e7fabc16e73b8130d8c8c2221d33d8c18a0573553830561f.jpg)



Figure 6.76 Long sector performance 2002


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/94837c989ab31b350119a697180dcc2ce6e12226e0a6d05779bcabfddf00a575.jpg)



Figure 6.77 Short sector performance 2002


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/eb9e2d8c5617795412f2489393f18c426f78280a6e7bce5c65b6b947d035cac8.jpg)


Having been knocked out of many positions not much happened to the portfolio for a couple of months until December when rates and currencies with some assistance from the non-agricultural commodities made a dash up and the fund ended a little over 30% in the positive. 

The big factors this year were clearly the rates and the currencies. Rates futures went up most of the year as yields came under pressure during the bear market so the profits were just made on the long side. In the currency sector the money was made on essentially being short the US dollar against all kinds of other currencies. 

The dollar weakness was one of the major themes in 2002 and Figure 6.78 displaying the Euro future shows just how friendly this trend was. The dollar index fell almost constantly throughout the year and there were long and profitable trades in practically all currency futures. 


Figure 6.78 Euro rising against Dollar during 2002


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/c6ae2e5f9f57132d2836077094f1fb4b697fba1c30c1f583be481003f3f09e9f.jpg)



Tables 6.51 and 6.52 contain the sector performance and results for this year. In earlier years we were getting free government money to the tune of 5–6% per year, but in 2002 we received less than 1.5% for helping the politicians out with their bills. This was not good for our business and something to keep an eye on. Before fees the result was 33% but after fees the number that the investors saw was closer to 27.4%. With the low government yields, the interest income failed to absorb much of the costs. Still, this was a year when the stock market lost over 20% and saw several very scary free fall declines and our results have to be considered very good in this environment.



Table 6.51 Sector performance 2002


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>16.0</td><td>2.8</td><td>-4.2</td><td>-1.1</td><td>18.2</td><td>31.8</td></tr><tr><td>Short</td><td>-4.6</td><td>2.7</td><td>-1.2</td><td>5.9</td><td>-1.4</td><td>1.3</td></tr><tr><td>All</td><td>11.4</td><td>5.5</td><td>-5.4</td><td>4.8</td><td>16.8</td><td>33.1</td></tr></table>


Table 6.52 Results 2002


<table><tr><td>Year</td><td>2002</td></tr><tr><td>Starting NAV</td><td>799.1</td></tr><tr><td>Trading result</td><td>33.1%</td></tr><tr><td>Interest income</td><td>1.4%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.8%</td></tr><tr><td>Performance fee</td><td>-4.8%</td></tr><tr><td>Net result</td><td>27.4%</td></tr><tr><td>Ending NAV</td><td>1018.0</td></tr></table>

## 2003

The initial portfolio of 2003 was quite dramatically different from that of the previous year. Last year we started off with just nine positions but now the portfolio consisted of 37 holdings across all sectors (see Tables 6.53 and 6.54 and Figure 6.79). Just like at the start of 2001 we had a clear bear market portfolio and an even more aggressive one than that year. We were short six different equity markets and long ten rates futures, making us very sensitive to the overall risk appetite of the world’s investors. As they ran scared we gained on both those legs and if they regained confidence we quickly lost. We were also very exposed to counter dollar bets, which in many ways is a related theme in this market. This was a period of falling dollar, falling equities and falling yields and these markets were strongly interrelated and driven by the same base factors. This was clearly a corner portfolio and a very scary one to be sitting on. You don’t need expensive risk-management software to see that this was a very risky and very concentrated portfolio, but that is part of running a trend-following futures portfolio. You may still want to get that expensive riskmanagement software, however, to figure out just how risky it was. 


Figure 6.79 Sector allocation 2003


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/e3c134ddaac412d51653d3934bcb945f296ee7c55f417c198a6b78a251ad08ff.jpg)



Table 6.53 Initial portfolio 2003


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Lumber</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Sugar</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Wheat</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Corn</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Soybeans</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Cotton</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Live cattle</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Rough rice</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Japanese yen</td><td>Long</td><td>Currencies</td></tr><tr><td>British pound</td><td>Long</td><td>Currencies</td></tr><tr><td>Swiss franc</td><td>Long</td><td>Currencies</td></tr><tr><td>Australian dollar</td><td>Long</td><td>Currencies</td></tr><tr><td>Euro</td><td>Long</td><td>Currencies</td></tr><tr><td>EUR/GBP</td><td>Long</td><td>Currencies</td></tr><tr><td>NZ dollar</td><td>Long</td><td>Currencies</td></tr><tr><td>Nikkei 225</td><td>Short</td><td>Equities</td></tr><tr><td>Dax</td><td>Short</td><td>Equities</td></tr><tr><td>S&amp;P 500</td><td>Short</td><td>Equities</td></tr><tr><td>EuroStoxx 50</td><td>Short</td><td>Equities</td></tr><tr><td>FTSE 100</td><td>Short</td><td>Equities</td></tr><tr><td>Hang Seng</td><td>Short</td><td>Equities</td></tr><tr><td>Gasoil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Heating oil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Crude oil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoline</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Gold</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Palladium</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Short sterling</td><td>Long</td><td>Rates</td></tr><tr><td>US 10-year note</td><td>Long</td><td>Rates</td></tr><tr><td>German Bund</td><td>Long</td><td>Rates</td></tr><tr><td>Long gilt</td><td>Long</td><td>Rates</td></tr><tr><td>US 2-year note</td><td>Long</td><td>Rates</td></tr><tr><td>Canadian Bankers’ Acceptance</td><td>Long</td><td>Rates</td></tr><tr><td>Euribor</td><td>Long</td><td>Rates</td></tr><tr><td>Eurodollar</td><td>Long</td><td>Rates</td></tr><tr><td>Euroswiss</td><td>Long</td><td>Rates</td></tr><tr><td>German Schatz</td><td>Long</td><td>Rates</td></tr></table>


Table 6.54 Initial sector allocation 2003


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>7</td><td>0</td><td>7</td></tr><tr><td>Agricultural commodities</td><td>4</td><td>4</td><td>8</td></tr><tr><td>Non-agricultural commodities</td><td>5</td><td>1</td><td>6</td></tr><tr><td>Equities</td><td>0</td><td>6</td><td>6</td></tr><tr><td>Rates</td><td>10</td><td>0</td><td>10</td></tr><tr><td>Total</td><td>26</td><td>11</td><td>37</td></tr></table>

The commodity bets were again somewhat side bets. We had some longs and some shorts and many of them had very low correlation to the main bear theme of the markets. 

One thing you can be sure about when you hold this sort of high risk on a portfolio is that you are about to see some action. You can never be sure whether the action will be on the upside or downside but a sideways move in the portfolio value with this amount of risk piled up is highly unlikely. 

For a couple of weeks in the beginning of the year things looked fairly calm but this changed very soon and before we entered February we already had a double digit profit on the books (see Figure 6.80). The zero line was left behind and not seen again for the rest of the year. Right from January, all our bets paid off at the same time and this is the true beauty of systematic trend-following futures strategies; when it rains, it pours. The long rates, long non-agriculturals and currencies were building profits very fast in the first quarter and the short equity side was having a strong contribution as well. In early March the fund was already at +25% while the MSCI World index was in double digit negative. This was one of those years where you were happy you did not go to dentist school after all. 


Figure 6.80 Strategy performance 2003


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/26170cd11630abf92a39235abff66cfeef919e84a1964f2a14d120b3f067dc9d.jpg)


The sharp decline by the end of March was surely a setback but by now you should be used to these occasional slaps in the face by our dear friend Mr Market. Going from +25% to +7% in a couple of weeks was very painful and as always hard to explain properly to the investors, but it is certainly easier when you are still in positive mode. The sudden giveback was caused by the turn in the market and risk appetite of the participants. The equity markets turned to the upside and the short equity bets gave up most of their year-to-date performance before they were stopped out. As so often happens during bear phases, many markets and sectors became increasingly correlated and when the equities turned up, all other major trends were turned upside down as well, which resulted in this rather large drawdown in March. 

The drawdown did not last long this time though and already in April we started climbing upwards again. The counter dollar bet was the big ticket item but we also got help from the long agricultural commodities and to some degree the short non-agriculturals. The performance year to date reached +30% by mid-year and although there was a brief period of volatility in July caused by failed bets on long rates, the fund stayed around the 25–30% level for the remainder of the year, until it made a push to the upside just in time for Christmas and ended up at +35%. Not a bad year at all. 

This year is often remembered for the turnaround in the equity markets, but the big story for trend followers was the decline of the US dollar. The lion’s share of the profits made this year was on being long other currencies against the US dollar (as Figures 6.81 and 6.82 show). Money was made on equities, both on the long and the short side (see Figure 6.83 for the latter), but the contribution from that sector was merely half of what the currencies gave us. The other sectors, the two commodity buckets and the rates, were all rounding errors in comparison to what the currencies and equities gave us and mere sideshows for a trend follower in 2003. 


Figure 6.81 Sector performance 2003


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/ebcbf1483a7b7ed1e75478f8ab18ae6e68ceb6d0320e7d816a9f53175f4156c3.jpg)



Figure 6.82 Long sector performance 2003


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/b0fa7929328d2031340b46b76f001f54af1dd5cca389ccddc11b8471ed437016.jpg)



Figure 6.83 Short sector performance 2003


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/06813106099b408b1f6ef848b8fe1919f8d50a7115b00e7ce62d28daccbfd0aa.jpg)


We entered into 2003 with several short positions in equities, following the bear market trend down. This turned out to be an overall good trade although in the short run it hit the portfolio because all these positions reversed at more or less the same time. The EuroStoxx 50 chart (Figure 6.84) is a good example of what happened. After a big blowout on the downside, there was a sudden and sharp move up in March, quickly hitting stops on all equity positions. 


Figure 6.84 End of the bear market


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/b0ee11ce51c56b0244ec9997834262c931d4ae47041b3e907c95c83c9b2ebc1e.jpg)



A year with performance as good as this (see Table 6.55) means lots of money to go round for everyone involved. The investors got 28.7% after costs and the manager received an obscene amount of dough for creating these profits. The interest on free cash hardly contributed at all this year and so the performance was all done with the trend-following futures strategy. All in all, the fund manager received over 6.5% of the initial money that was in the fund at the start of the year (see Table 6.56).



Table 6.55 Sector performance 2003


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>27.9</td><td>8.0</td><td>3.8</td><td>11.0</td><td>-2.0</td><td>48.7</td></tr><tr><td>Short</td><td>-3.7</td><td>-5.9</td><td>-1.1</td><td>0.5</td><td>-3.3</td><td>-13.5</td></tr><tr><td>All</td><td>24.2</td><td>2.1</td><td>2.7</td><td>11.5</td><td>-5.3</td><td>35.2</td></tr></table>


Table 6.56 Results 2003


<table><tr><td>Year</td><td>2003</td></tr><tr><td>Starting NAV</td><td>1,018</td></tr><tr><td>Trading result</td><td>35.2%</td></tr><tr><td>Interest income</td><td>1.0%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.8%</td></tr><tr><td>Performance fee</td><td>-5.1%</td></tr><tr><td>Net result</td><td>28.7%</td></tr></table>

## 2004

The January portfolio of 2004 held a couple of interrelated themes and if you look carefully at the data in Tables 6.57 and 6.58 you can see that this was a very decisive portfolio, with clear convictions on the markets. You don’t find balanced and measured allocations with both longs and shorts across all sectors as some years can show. This year the strategy had taken quite large bets on concentrated themes. The first theme was the weakness of the US dollar and this is clear from all the long currency futures, most of which were against the dollar. The second theme was that there were eight long positions in equities, making for a big bet on a continued bull market. Although conventional wisdom often states that fixed income and equities have an inverse correlation, this is not always the case and here we were also long the rates sector. On the non-agricultural side we held longs in metals and energies while the agriculturals were all short. This portfolio was very consistent with the main theme at the time: a bull market with a falling US dollar. You can see the sector percentages in Figure 6.85. 


Figure 6.85 Sector allocation 2004


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/b6a0a27a2fe43fc96649efe063eefdcf0faae12887a1b1e335449aae16d94a5f.jpg)



Table 6.57 Initial portfolio 2004


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Sugar</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Oats</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Lean hogs</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Canadian dollar</td><td>Long</td><td>Currencies</td></tr><tr><td>EUR/JPY</td><td>Long</td><td>Currencies</td></tr><tr><td>Swiss franc</td><td>Long</td><td>Currencies</td></tr><tr><td>Euro</td><td>Long</td><td>Currencies</td></tr><tr><td>Japanese yen</td><td>Long</td><td>Currencies</td></tr><tr><td>British pound</td><td>Long</td><td>Currencies</td></tr><tr><td>NZ dollar</td><td>Long</td><td>Currencies</td></tr><tr><td>Australian dollar</td><td>Long</td><td>Currencies</td></tr><tr><td>Russell 2000</td><td>Long</td><td>Equities</td></tr><tr><td>Hang Seng</td><td>Long</td><td>Equities</td></tr><tr><td>EuroStoxx 50</td><td>Long</td><td>Equities</td></tr><tr><td>DAX</td><td>Long</td><td>Equities</td></tr><tr><td>CAC 40</td><td>Long</td><td>Equities</td></tr><tr><td>FTSE 100</td><td>Long</td><td>Equities</td></tr><tr><td>Nasdaq 100</td><td>Long</td><td>Equities</td></tr><tr><td>S&amp;P 500</td><td>Long</td><td>Equities</td></tr><tr><td>Gasoline</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Crude oil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Heating oil</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Copper</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Silver</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Gold</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>German Schatz</td><td>Long</td><td>Rates</td></tr><tr><td>Euroswiss</td><td>Long</td><td>Rates</td></tr><tr><td>US 10-year note</td><td>Long</td><td>Rates</td></tr><tr><td>US 2-year note</td><td>Long</td><td>Rates</td></tr><tr><td>Canadian Bankers’ Acceptance</td><td>Long</td><td>Rates</td></tr><tr><td>Eurodollar</td><td>Long</td><td>Rates</td></tr></table>


Table 6.58 Initial sector allocation 2004


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>8</td><td>0</td><td>8</td></tr><tr><td>Agricultural commodities</td><td>0</td><td>3</td><td>3</td></tr><tr><td>Non-agricultural commodities</td><td>7</td><td>0</td><td>7</td></tr><tr><td>Equities</td><td>8</td><td>0</td><td>8</td></tr><tr><td>Rates</td><td>6</td><td>0</td><td>6</td></tr><tr><td>Total</td><td>29</td><td>3</td><td>32</td></tr></table>

As Figure 6.86 reveals, 2004 turned out to be an emotional roller coaster and the relatively easy times of the last three years were nowhere to be seen. 2004 saw very high volatility and it did not give much reward for the risk taken. The year started well enough with a steep ascent to +12% two weeks into January. After a volatile few weeks, the fund was back at the zero line in February before taking off on the upside to hit +16% by the end of the first quarter. So far the volatility had been a nail-biter for investors and manager alike, but the real problems of this year had not really begun. From the peak of +16% the fund plummeted down hard, first to +3%, then to zero, then down to –5% and by September we hit a low of –9.5%. Being at a profit of 16% in March and finding yourself down at –10% in September could cause nervous breakdowns in the best of us. Losing over 25 percentage points was a tough experience. The initial decline from the positive numbers back to neutral was caused by a multitude of sectors, in which many previously profitable sectors such as rates and non-agriculturals gave back most of their performance, while the long equity bets were constantly suffering at the same time. The sharp acceleration on the downside was fuelled by short rates bets taken on during the year together with currency losses. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/afc490ba2382d1384b0f22737125e8f2d5b07f14dc91950cd21cc43b080e08fd.jpg)


From these lows, the profits slowly started climbing up again and by the end of the year we finished at less than 5% up. At the same time, the world stock markets could show a return in the double digits and at less volatility to boot. It is not easy to explain such a year to investors especially if they don’t have full insight into and understanding of the fund’s strategy. 

What made the difference at the end of the year were the long metals and energies: the non-agricultural sector was the only one with any profits to speak of. Despite the fact that the global equity markets did quite well, we lost over 4% on the equity futures. 

As you can see in the sector charts (Figures 6.87 to 6.89), there was a rather large giveback of profits in the long rates sector in late March and the long gilt market was partly to blame (see Figure 6.90). All our long rates positions at this time suddenly reversed course and went off a cliff, hitting stops in rapid succession. The long gilt was an unfortunate trade because most other rates positions already held nice profits and only gave back parts of them, whereas this particular market entered into a long trade just before the plunge. 


Figure 6.87 Sector performance 2004


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/a112e4c184b581c5c7ee303e11ccf866a85e6a36adadad2dc334de5f859004fb.jpg)



Figure 6.88 Long sector performance 2004


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/7918c03653b6019147d6541205a78a659c45bd7e0f8ee9673e007e050622fd9e.jpg)



Figure 6.89 Short sector performance 2004


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/368b88fb0fe1402960486424a66489e89548068b6a208c0d42a2f30edfd9741c.jpg)



Figure 6.90 Costly trade in long gilt


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/291cec09997ad743bc5fe3266278b7c88af03c95669a3c4886ba9bf4ac0becf8.jpg)


After a year like this, you’d feel ashamed to take a performance fee (see Tables 6.59 and 6.60). Not that it would be much money, but still. After all the bills were paid there was only a 3% return left for the investors, with which they were sure to be unhappy and with full right. A few measly per cent was no way to compensate for the volatility we saw this year. The pressure was on to make sure that we could show investors some profits soon or else redemptions would be coming in. 


Table 6.59 Sector performance 2004


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>4.2</td><td>-1.2</td><td>5.9</td><td>-0.8</td><td>4.5</td><td>12.5</td></tr><tr><td>Short</td><td>-4.2</td><td>2.5</td><td>0.6</td><td>-3.1</td><td>-3.7</td><td>-7.9</td></tr><tr><td>All</td><td>-0.1</td><td>1.2</td><td>6.5</td><td>-3.9</td><td>0.8</td><td>4.6</td></tr></table>


Table 6.60 Results 2004


<table><tr><td>Year</td><td>2004</td></tr><tr><td>Starting NAV</td><td>1310.4</td></tr><tr><td>Trading result</td><td>4.6%</td></tr><tr><td>Interest income</td><td>1.1%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.5%</td></tr><tr><td>Performance fee</td><td>-0.6%</td></tr><tr><td>Net result</td><td>3.1%</td></tr><tr><td>Ending NAV</td><td>1351.4</td></tr></table>


2005


With 30 positions we had another year starting out with quite a high risk level (see Tables 6.61 and 6.62 and Figure 6.91). During bad periods the number of positions tends to decrease to a very small amount, as stop after stop is triggered and positions are closed down. The same thing happened during 2004, but after the strong finish of last year we again had a large portfolio of instruments. The rally was still on in the equity markets and we had nine long positions in that sector. We also still had large counter dollar bets against several different world currencies. Apart from that, the bets were rather spread out and not very theme concentrated. Still, with a portfolio this size some moves were certain and after 2004 we needed some performance. 

Figure 6.91 Sector allocation 2005 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/4b1e75a1d95d14b210fae00c61a282d9d97e2072c9e9da9cb659ba234937bfdb.jpg)



Table 6.61 Initial portfolio 2005


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Sugar</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Oats</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Cotton</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Corn</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Wheat</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>EUR/GBP</td><td>Long</td><td>Currencies</td></tr><tr><td>EUR/CHF</td><td>Long</td><td>Currencies</td></tr><tr><td>EUR/JPY</td><td>Long</td><td>Currencies</td></tr><tr><td>Canadian Bankers’ Acceptance</td><td>Long</td><td>Currencies</td></tr><tr><td>British pound</td><td>Long</td><td>Currencies</td></tr><tr><td>Swiss franc</td><td>Long</td><td>Currencies</td></tr><tr><td>Euro</td><td>Long</td><td>Currencies</td></tr><tr><td>NZ dollar</td><td>Long</td><td>Currencies</td></tr><tr><td>Hang Seng China Enterprises</td><td>Long</td><td>Equities</td></tr><tr><td>CAC 40</td><td>Long</td><td>Equities</td></tr><tr><td>DAX</td><td>Long</td><td>Equities</td></tr><tr><td>FTSE 100</td><td>Long</td><td>Equities</td></tr><tr><td>Hang Seng</td><td>Long</td><td>Equities</td></tr><tr><td>S&amp;P 500</td><td>Long</td><td>Equities</td></tr><tr><td>Nasdaq 100</td><td>Long</td><td>Equities</td></tr><tr><td>EuroStoxx 50</td><td>Long</td><td>Equities</td></tr><tr><td>Russell 2000</td><td>Long</td><td>Equities</td></tr><tr><td>Copper</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoline</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Natural gas</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Palladium</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Euroswiss</td><td>Long</td><td>Rates</td></tr><tr><td>Eurodollar</td><td>Short</td><td>Rates</td></tr><tr><td>Short sterling</td><td>Long</td><td>Rates</td></tr><tr><td>Long gilt</td><td>Long</td><td>Rates</td></tr></table>


Table 6.62 Initial sector allocation 2005


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>8</td><td>0</td><td>8</td></tr><tr><td>Agricultural commodities</td><td>2</td><td>3</td><td>5</td></tr><tr><td>Non-agricultural commodities</td><td>1</td><td>3</td><td>4</td></tr><tr><td>Equities</td><td>9</td><td>0</td><td>9</td></tr><tr><td>Rates</td><td>3</td><td>1</td><td>4</td></tr><tr><td>Total</td><td>23</td><td>7</td><td>30</td></tr></table>

Unfortunately for us, the year could not have started worse. In the first couple of days of the year we quickly lost over 6%, and although much of this was recovered by February, the declines continued and there was another very sharp push down in late March, which saw the fund reaching into the negative double digits (check out Figure 6.92). The big decline early on in the year was caused primarily by the long equity positions, which all suffered at the same time when the market turned down. This is the big danger with this particular sector: that the internal correlation tends to be much higher than in other sectors and in particular when the market turns sharply down. It is easy to fall into the trap of believing that you are diversified just because you hold long equities in many countries or sectors, but when things turn down they all move down together. The second sharp downturn also owed much to the same sector but it also got some help from the currencies and commodities. 


Figure 6.92 Strategy performance 2005


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/6cc9efb4e7259f6ab0eaec0815a6524b68b8fe3721d03a0697a29f828688f300.jpg)



In early June we were still at –10% but started to move slowly upwards courtesy of the long equity positions and the long rates. Having almost reached the zero line again in August, the fund dropped down hard and touched the double digits. Again we found ourselves having a big loss on the books late in the year and in these situations things can feel rather hopeless. What you always need to remember is that this is a statistical game with a slight tilt in your favour and that you just have to keep throwing the dice long enough to get the law of big numbers on your side.


In late October the curves finally started pointing up again and as the long non-agricultural commodities, long equities and short rates all kicked in at the same time, we finished the year in almost the same manner as in 2004; first peaking above +10% and then falling back to about 5% in the positive. 

The positions betting on a weak dollar clearly did not pan out and we ended up with the biggest loss in the currency sector (see Figures 6.93 and 6.94). The only sectors that had a sizable overall contribution were the equities and the rates. The non-agricultural commodities show that there was potential on the long side but that the short side ate up most of the profits (see Figures 6.95). 


Figure 6.93 Sector performance 2005


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/1ac1a9833ac84885691518167b6537bb9861e38cb62d378d0120d96d08ffb1c3.jpg)



Figure 6.94 Long sector performance 2005


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/7219e2353b1dcbae065fe8e4a3aeca72243f2d1ccd59e100837b275a15e6c2db.jpg)



Figure 6.95 Short sector performance 2005


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/9938d18a235bbb279f875328a7faa98a9fdc49c65513b1719be392da2db423c6.jpg)


The Nikkei trade in 2005 shows the kind of trend you really want to find: a nice smooth ascent followed by a reasonably orderly pullback to let us exit (see Figure 6.96). After a brief sideways movement of the market, we re-entered and were treated to the same comfortable ride up once more before stepping out. Unfortunately, this kind of trade was rare in 2005. 


Figure 6.96 Japan joining the bull market


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/088beeb3706a1c22d5bc11f619c128f877f231284d4d8076b693752bee1f74f0.jpg)



Table 6.63 Sector performance 2005


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>-6.9</td><td>1.6</td><td>6.3</td><td>6.8</td><td>-0.3</td><td>7.4</td></tr><tr><td>Short</td><td>0.5</td><td>-2.4</td><td>-4.2</td><td>-0.7</td><td>4.4</td><td>-2.4</td></tr><tr><td>All</td><td>-6.4</td><td>-0.9</td><td>2.1</td><td>6.1</td><td>4.1</td><td>5.0</td></tr></table>


Table 6.64 Results 2005


<table><tr><td>Year</td><td>2005</td></tr><tr><td>Starting NAV</td><td>1351.4</td></tr><tr><td>Trading result</td><td>5.0%</td></tr><tr><td>Interest income</td><td>2.5%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.6%</td></tr><tr><td>Performance fee</td><td>-0.8%</td></tr><tr><td>Net result</td><td>4.6%</td></tr><tr><td>Ending NAV</td><td>1413.1</td></tr></table>

2005 was again a year in which it felt like you did not deserve that performance fee (see Tables 6.63 and 6.64). Even if that fee seemed small in comparison to the fund size, it showed a side of the business that may surprise people unfamiliar with the hedge-fund and absolute-return mandate industry. Managing a fund of 10 million or 100 million does not make too big a difference in terms of effort, but if the fund had 100 million at the start of this year, the manager would have made almost a million on performance fee, despite the fact that this year by any objective standards must be seen as a failure. The investors were left just 5%, and the only reason it was that much was because the money market yields went up enough to give 2.5% return to the fund, on which the manager of course received a performance fee as well. 

## 2006

The bull market in equities was still in effect in early 2006 and the strategy saw fit to take on maximum risk in this sector. Remember that we had 10 markets included in each sector and going into January 2006 we were long all 10 equity markets (see Tables 6.65 and 6.66). There was also a clear bet on downwards trending oil prices, with four different oil-related markets held short. The remaining bets were spread out and reasonably diversified across longs and shorts in the other sectors. Such a large bet in the equity markets should rightfully make you a little nervous, given the high propensity of internal correlation that this sector tends to display. With two tough years behind us, this year was critical to investor confidence, not to mention the manager’s. The sector percentages are shown in Figure 6.97. 


Figure 6.97 Sector allocation 2006


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/d9c92845ef47e6a32ca530ed94218fce0da35cf5f434102a989a41af74ee6844.jpg)


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Lumber</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Rough rice</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Cotton</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Sugar</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Live cattle</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Australian collar</td><td>Short</td><td>Currencies</td></tr><tr><td>EUR/CHF</td><td>Long</td><td>Currencies</td></tr><tr><td>Canadian collar</td><td>Long</td><td>Currencies</td></tr><tr><td>Euro</td><td>Short</td><td>Currencies</td></tr><tr><td>Swiss franc</td><td>Short</td><td>Currencies</td></tr><tr><td>Nikkei 225</td><td>Long</td><td>Equities</td></tr><tr><td>Hang Seng</td><td>Long</td><td>Equities</td></tr><tr><td>Hang Seng China Enterprises</td><td>Long</td><td>Equities</td></tr><tr><td>CAC 40</td><td>Long</td><td>Equities</td></tr><tr><td>FTSE 100</td><td>Long</td><td>Equities</td></tr><tr><td>EuroStoxx 50</td><td>Long</td><td>Equities</td></tr><tr><td>Russell 2000</td><td>Long</td><td>Equities</td></tr><tr><td>DAX</td><td>Long</td><td>Equities</td></tr><tr><td>S&amp;P 500</td><td>Long</td><td>Equities</td></tr><tr><td>Nasdaq 100</td><td>Long</td><td>Equities</td></tr><tr><td>Heating oil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoline</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Crude oil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Copper</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Long gilt</td><td>Long</td><td>Rates</td></tr><tr><td>US 2-year note</td><td>Short</td><td>Rates</td></tr><tr><td>Canadian Bankers’ Acceptance</td><td>Short</td><td>Rates</td></tr></table>


Table 6.66 Initial sector allocation 2006


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>2</td><td>3</td><td>5</td></tr><tr><td>Agricultural commodities</td><td>4</td><td>1</td><td>5</td></tr><tr><td>Non-agricultural commodities</td><td>1</td><td>4</td><td>5</td></tr><tr><td>Equities</td><td>10</td><td>0</td><td>10</td></tr><tr><td>Rates</td><td>1</td><td>2</td><td>3</td></tr><tr><td>Total</td><td>18</td><td>10</td><td>28</td></tr></table>

The year started off with a large advance in the equity markets, quickly sending the fund up over 5%, followed by a move in the commodities that pushed the fund up into the double digits positive in just the second month of the year (see Figure 6.98). Half of this move was quickly lost again in February but as the commodities started contributing in a big way in March and April the fund ascended rapidly in an almost parabolic manner. The short energies did not work out so well but as the fund shifted into long metals the profits were racked up very quickly. During April and part of May 2006 both precious and base metals 

went skyrocketing and at the same time short agricultural commodities and rates had a nice contribution as well, making the fund attain the amazing number of +36% in late May. 


Figure 6.98 Strategy performance 2006


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/6ad3d4815ea9c7094b756f859319276fe42d5a08d42628d59e7eb7750bee2abb.jpg)


As I am sure you are painfully aware by now, the weakness of this strategy in its current shape is that at times it exhibits excess volatility and often gives back large parts of gains very quickly when the trends turn. This again happened here and from being at +35% the drop-down was even faster than the parabolic ascent seen in May. The first thing that happened was that the equity market rebounded to the downside and lost the whole year’s performance during May and June and at that same time the rates futures reversed as well as they normally do in these situations. The bear market was not over yet, but the rebound was strong enough to trigger stops in all our 10 long equity markets. Once the equity markets took off in bull mode again in July, we no longer had a stake in that sector and were left to watch the rally without making any money from it. 

The fund struggled for several months after this because there was a lack of real trends in any sector and the fund continued slowly down, finally reaching the low of +5% year to date, having lost 30 percentage points from the top. After the past two bad years, this was a tough one to bear. At this point the long equity positions started building up again, and along with short positions in energies this helped to regain some performance. The year finally ended at a little over 20% up, which had to be seen as an acceptable result despite the high volatility during this year. 

Years like 2006 are extremely different to live through and in fact trade compared to looking at a simulation. It would be easy to look simply at the yearly or even monthly result and think it was a very good and easy year, but going through the ups and down in reality was quite a different matter and cannot be properly taught in any other way than by personal experience. 

All sectors but the rates ended up positive and three of them with quite respectable numbers, making this year look quite successful in retrospect, despite the nerve-wracking ride (see Figures 6.99 to 6.101). In the non-agricultural sector we made money on both long metals and short energies and the profits were fairly evenly distributed in the agricultural bucket as well, showing that the diversification themes worked well here. The equities and rates, however, had a much larger correlation this year, both internally and against each other, and although they both ended up profitable their respective profits and losses throughout the year were timed very similarly, showing that we held a very high risk concentration to a single theme and that was ultimately the cause of the excessive volatility in 2006. 

Figure 6.99 Sector performance 2006 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/8ab249962a9ae346325623b5ad40d355eace10e5436b1613ca4c56224422f6a0.jpg)



Figure 6.100 Long sector performance 2006


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/ea3de9f149426005a61803c4a0d8913c575ca8c1df2f7faa3bceaa81bb2a87a4.jpg)



Figure 6.101 Short sector performance 2006


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/3bc8b46ae69792958b24f129e1731a143a0e1fc2dc7e66355fa711266d079a6a.jpg)


Even though the equities made up for it in the end, the sector saw some sharp declines late in the second quarter. It was the most profitable sector this year despite the high internal correlations and choppy moves. 


Trading profits were over 22% before the performance fee ate up quite a large chunk of the pie, but the days of high-interest payments were back for now and we got a whole 4% on our deposits with the government (see Tables 6.67 and 6.68). After the costs were loaded onto the fund the remaining yield for customers was still a respectable 20.5%.


In some of markets, such as the Nasdaq shown in Figure 6.102, the strategy took on short positions soon after the longs were stopped out, joining the bear market side. 


Figure 6.102 Bear phase of 2006


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/d80e1295eb536e68eaf0c652233df17bbebd165e60e89795c19839a57bf17136.jpg)



Table 6.67 Sector performance 2006


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>2.7</td><td>2.5</td><td>5.2</td><td>12.6</td><td>-6.9</td><td>16.1</td></tr><tr><td>Short</td><td>-1.5</td><td>3.9</td><td>4.2</td><td>-1.4</td><td>1.0</td><td>6.2</td></tr><tr><td>All</td><td>1.2</td><td>6.4</td><td>9.5</td><td>11.2</td><td>-5.9</td><td>22.3</td></tr></table>


Table 6.68 Results 2006


<table><tr><td>Year</td><td>2006</td></tr><tr><td>Starting NAV</td><td>1413.1</td></tr><tr><td>Trading result</td><td>22.3%</td></tr><tr><td>Interest income</td><td>4.0%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.7%</td></tr><tr><td>Performance fee</td><td>-3.6%</td></tr><tr><td>Net result</td><td>20.5%</td></tr><tr><td>Ending NAV</td><td>1702.3</td></tr></table>

## 2007

Just like the previous year we had a portfolio geared for a bull market on our hands. With eight long equity positions and six short rates markets, this was a very concentrated portfolio betting on a continuation of the on-going rally (see Tables 6.69 and 6.70 and Figure 6.103). There was also a concentration of currency positions that would all gain if the US dollar declined. In combination with being short three oil-related markets, this made for a high risk portfolio. We should have expected this portfolio to make some moves, but the direction of those moves remained to be seen. 


Figure 6.103 Sector allocation 2007


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/e9fd477e124f7b9bf439458588ad27969d1e5f8f7e749b4384f4242f73498391.jpg)



Table 6.69 Initial portfolio 2007


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Rough rice</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>EUR/JPY</td><td>Long</td><td>Currencies</td></tr><tr><td>NZ dollar</td><td>Long</td><td>Currencies</td></tr><tr><td>British pound</td><td>Long</td><td>Currencies</td></tr><tr><td>EUR/CHF</td><td>Long</td><td>Currencies</td></tr><tr><td>Euro</td><td>Long</td><td>Currencies</td></tr><tr><td>Australian dollar</td><td>Long</td><td>Currencies</td></tr><tr><td>Canadian dollar</td><td>Short</td><td>Currencies</td></tr><tr><td>Japanese yen</td><td>Short</td><td>Currencies</td></tr><tr><td>EUR/GBP</td><td>Short</td><td>Currencies</td></tr><tr><td>Hang Seng China Enterprises</td><td>Long</td><td>Equities</td></tr><tr><td>Hang Seng</td><td>Long</td><td>Equities</td></tr><tr><td>S&amp;P 500</td><td>Long</td><td>Equities</td></tr><tr><td>Mini Russell 2000</td><td>Long</td><td>Equities</td></tr><tr><td>DAX</td><td>Long</td><td>Equities</td></tr><tr><td>Nikkei 225</td><td>Long</td><td>Equities</td></tr><tr><td>CAC 40</td><td>Long</td><td>Equities</td></tr><tr><td>EuroStoxx 50</td><td>Long</td><td>Equities</td></tr><tr><td>Heating oil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Crude oil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Copper</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Natural gas</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Short sterling</td><td>Short</td><td>Rates</td></tr><tr><td>German Schatz</td><td>Short</td><td>Rates</td></tr><tr><td>Eurodollar</td><td>Short</td><td>Rates</td></tr><tr><td>Euroswiss</td><td>Short</td><td>Rates</td></tr><tr><td>Long gilt</td><td>Short</td><td>Rates</td></tr><tr><td>Euribor</td><td>Short</td><td>Rates</td></tr></table>


Table 6.70 Initial sector allocation 2007


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>6</td><td>3</td><td>9</td></tr><tr><td>Agricultural commodities</td><td>1</td><td>0</td><td>1</td></tr><tr><td>Non-agricultural commodities</td><td>0</td><td>5</td><td>5</td></tr><tr><td>Equities</td><td>8</td><td>0</td><td>8</td></tr><tr><td>Rates</td><td>0</td><td>6</td><td>6</td></tr><tr><td>Total</td><td>15</td><td>14</td><td>29</td></tr></table>

The first couple of months of the year were quite calm with modest profits and gains in different sectors cancelling each other out, but in February something rather dramatic happened (see Figure 6.104). On 27 February the Chinese market dropped almost 10% in a day, sending shockwaves throughout the world’s equity markets. This was a completely outsized move in the wrong direction for us and the fund took very large losses literarily overnight. All long equity positions hit their stops in a single day, losing over 7% on the fund in a day on that sector. The fund as a whole lost over 15% in a couple of days and after this most positions were stopped out, meaning that it would not be easy to fight our way back up. Being stuck at – 15% with very few positions still held meant that there would be no real moves in the portfolio until new trends emerged and we could rebuild a proper portfolio. At least the risk level was low for the moment and further sharp declines were not likely any time soon. 


Figure 6.104 Strategy performance 2007


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/7a8f6dbb8e25c0ce5289aa7d6651ed160d5ab8046513b5ac07d8fadc47bed59f.jpg)


After the Chinese correction, or crash if you really want to use that word, the markets recovered very quickly but without our participation because our stops had already triggered. The long equity positions were not re-entered until late April and so most of the recovery was missed. The fund did manage to recover during the summer and reached a peak of +20% in July courtesy of long rates, equities and currencies. Unfortunately, by then we had just managed to build up a new concentrated equity portfolio just before the next correction came along and the fund again lost on all equity futures, sending the fund’s year to date performance down to –3% in September and making this another extreme roller coaster year. 

In this line of business, help often comes from the most unexpected source and suddenly both the agricultural and non-agricultural sector started taking over the driver seat, adding up enough gains for the fund to end at more than 8% up. 

This was a very bad year for the equity sector, which had a negative contribution of 7% and lost on both longs and shorts (see Figures 6.105 to 6.107). If not for the commodities, in particular the agricultural ones, this would have been a real disaster year, showing again the strength of proper diversification. 


Figure 6.105 Sector performance 2007


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/4378e169a11775ee5382d7d4517a15151cf4c9ac13ce99b218c922724f53012d.jpg)



Figure 6.106 Long sector performance 2007


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/629d931f8d71da786b0bae41626f631486d25dbcadc2a0302c7e822f829b0f7a.jpg)



Figure 6.107 Short sector performance 2007


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/6029a19065352ee65e29b712ed68e9b47883fc46cbd9e2514958619e96d4af1b.jpg)



One of the agricultural positions that helped greatly to save this year was the soybeans and the rally it experienced late in the year (see Figure 6.108). Entered in late October and held a couple of months into the following year, this was a very profitable transaction.



Figure 6.108 Soybean rally of 2007


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/b947aa8cb079a3761273f05262df4ced2aef7c704787c355e973cf1794486bce.jpg)



As we have seen before, with low yearly returns such as this a large chunk of the profits were eaten up by the fees (see Tables 6.71 and 6.72). The saviour here was the relatively high return on the cash, which contributed almost 4% to the bottom line. This effect managed to more or less cancel out the fees and the official end of year number landed at +8.5%.



Table 6.71 Sector performance 2007


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>2.7</td><td>5.9</td><td>5.5</td><td>-0.8</td><td>-3.4</td><td>9.8</td></tr><tr><td>Short</td><td>-0.4</td><td>0.9</td><td>-1.9</td><td>-6.2</td><td>6.2</td><td>-1.4</td></tr><tr><td>All</td><td>2.3</td><td>6.8</td><td>3.6</td><td>-7.0</td><td>2.7</td><td>8.4</td></tr></table>

<table><tr><td>Year</td><td>2007</td></tr><tr><td>Starting NAV</td><td>1702.3</td></tr><tr><td>Trading result</td><td>8.4%</td></tr><tr><td>Interest income</td><td>3.8%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.6%</td></tr><tr><td>Performance fee</td><td>-1.5%</td></tr><tr><td>Net result</td><td>8.5%</td></tr><tr><td>Ending NAV</td><td>1847.7</td></tr></table>


2008


After some tough years behind us, and of course unknown to us at the time, we were about to enter into the most exciting year in the history of trend-following strategies. 2008 was truly a year like no other. 

The initial portfolio was nothing to write home about; it was quite a small one consisting mostly of commodity bets with no equities and very little exposure to rates and currencies (see Tables 6.73 and 6.74 and Figure 6.109). With this portfolio we would not expect any large swings in the portfolio value, unless of course strong trends emerged and we started building up new positions. 


Figure 6.109 Portfolio allocation 2008


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/8178f27616de973f41af4bc95f37fd5df4bf6c28e7af2c8eac89a2be5a3f5ef7.jpg)



Table 6.73 Initial portfolio allocation 2008


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Rough rice</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Soybeans</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Corn</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Live cattle</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Lumber</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Lean hogs</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Sugar</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>EUR/GBP</td><td>Long</td><td>Currencies</td></tr><tr><td>EUR/JPY</td><td>Long</td><td>Currencies</td></tr><tr><td>Platinum</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoline</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Copper</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Natural gas</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Euribor</td><td>Short</td><td>Rates</td></tr><tr><td>Short sterling</td><td>Long</td><td>Rates</td></tr></table>


Table 6.74 Initial sector allocation 2008


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>2</td><td>0</td><td>2</td></tr><tr><td>Agricultural commodities</td><td>4</td><td>3</td><td>7</td></tr><tr><td>Non-agricultural Commodities</td><td>2</td><td>2</td><td>4</td></tr><tr><td>Equities</td><td>0</td><td>0</td><td>0</td></tr><tr><td>Rates</td><td>1</td><td>1</td><td>2</td></tr><tr><td>Total</td><td>9</td><td>6</td><td>15</td></tr></table>

Take a look at the y-axis scale of Figure 6.110 before we start reviewing the performance over the year. The scale is dramatically different from the previous years, both on the positive and negative side. The year of 2008 saw some of the most extreme moves in the financial markets since the crash of 1929 and while the world equity markets lost about half of their value, it was a stellar year for trend followers albeit still not an entirely easy one. 


Figure 6.110 Strategy performance 2008


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/d2b9239f3de750f224806a43a87c7e6b5a474937039f9d8b4fb1d247ce38fe70.jpg)


The modest portfolio initially held was augmented quite swiftly in the first few weeks of the year as more and more trends developed and the risk level was successively increased. In late January the fund had gains of over 10%, but in a remarkable year such as 2008 this is barely worth mentioning. In February and March both of the commodity sectors started going crazy on the long side, racking up large profits in a very short period, and as the short equities gained at the same time the fund reached an amazing +40% before the end of the first quarter. The following period between March and September was the calm 

before the storm, in a manner of speaking. The profits went up and down a bit, but stayed between +20% and +40% most of the time as the profits and losses of various sectors cancelled each other out over time. 

2008 will always be remembered as the year when the global financial system was on the brink of total collapse and bailout after bailout did not seem to halt the never-ending financial crises. Bear Sterns and Lehman Brothers went bankrupt, AIG was barely saved and all the largest banks in the world had to get government help to survive the year. This was a time of extreme fear and equally extreme market volatility. It was also a time of extreme trends and the payout for those who followed the strategy was, for lack of a better word, even more extreme. 

In October the rocket ship took off and it hit terminal velocity before the passengers had time to say ‘Credit Crunch’. From being at +30% in early October, the fund had hit an unprecedented +80% on the year before the month was over and in the next months the returns reached into the triple digits. It started with oil going into a strong bear trend, then our short equities kicked in with big profits at the same time as short commodities and long dollar bets all made huge profits. All these factors made big contributions, but the massive contributor was the long rates futures which built up profits to the tune of 40% on the fund in a matter of two months. 

This was a six standard deviation year that occurs once in a hundred years. Of course, in that context you need to be aware that 85% of all statistics are made up on the spot. What we can assert, however, is that this type of year has only happened once in the 30–40 years when it was possible to trade diversified futures and the reasonable conclusion is that such a perfect storm is not likely to happen again anytime soon. If it still does happen, your strategy should be prepared for it and able to handle it. 

This year may seem like a dream year for a trend-following trader but there were many things that could go wrong and most managers of this type of strategies ended up overriding trades or reducing the risk of their strategies. The first thing to remember is that when you see Bear Sterns, Lehman Brothers and the rest blowing up and taking the money of their clients with them, you need to be extraordinarily careful with your counterparty risk. If your prime broker goes the way of the dodo, you can realistically expect that all cash on the books will be gone in the same instance and in the worst case scenario you will also be unable to liquidate your futures positions for days or perhaps weeks. This would mean the end of your fund, your business and possibly of your clients’ assets. 

This is a good reminder that you need to do proper due diligence on your broker and find one that is financially sound. This can prove difficult because some of the failed brokers looked good from the outside until the very end. If in any doubt whatsoever, pick a safer broker – preferably one that does nothing but brokerage and takes no proprietary risks. You may also need several brokers, to be able to move your cash and positions quickly to another counterpart should one of them start having problems. It is also important to keep as little cash as possible on the accounts. Put as much as you can in government debt with short duration, not as much for the yield (which in 2012 is so close to zero that it hardly covers commissions) but rather to safeguard it against the failure of a counterpart. 

The other concern with the development of late 2008 was the excessive volatility to which the strategy was subjected. There were many days when you saw swings of 15–20% of the fund value, in a single day. This is not what the strategy was designed for, and even though everything ended up marvellously if you closed your eyes and let the strategy run, the danger level was clearly above our plans. The question of whether or not you should override the strategy in this type of market is a difficult one. I know of some large funds that simply decided to cut all positions in half when volatility reached uncomfortable levels and I know of funds that just went full speed ahead. My take is that if you have profits in the 50–70% range and start seeing 10–20% moves in single days, it may make sense to conclude that the market is out of its mind and that anything can happen and that you subsequently should reduce your exposure. Live to fight another day and all of that. 

It was practically impossible to predict that a year like this would come along and therefore it was not strange that most funds did not have proper rules for how to handle it. Now we have seen 2008, however, and rules can be made in advance for how to handle the positions, should such a year happen again. 

The result by the end of this dramatic year landed at +124% and I doubt that many futures managers got much sleep in the last quarter of the year. 

The real eye opener when you look at the sector results in Figures 6.111 to 6.113 should be that the equity sector, even the short side, actually lost money during a year when the bear trend was so strong. As we have seen before, the problem is that equity markets across the world have a bad habit of reaching a near perfect 1 correlation during times of distress, and so although it looks like we have 10 different positions, they will all go up and down in identical patterns during these kinds of years. This results in quick profits being built up, which are then quickly lost as all equity markets pull back on the same day. 


Figure 6.111 Sector performance 2008


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/18b922cbfa89cbd17cd104e926aea6be162eb5631167dcf9eaca0bfdc13983cc.jpg)



Figure 6.112 Long sector performance 2008


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/8702c7f0de2b646e8f14fbb1712af07beb3efe69ea617a9cead359b073193824.jpg)



Figure 6.113 Short sector performance 2008


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/4f1cc571a8906906823260c120fa86658da4d4c53a71ce66ad90a4379ae3ce8f.jpg)



The rates sector was the absolute star this year and being long bonds from all over the world was the key position. As investors ran for cover to move their money from equity markets to safer alternatives, these bonds rallied and so did our profits.


As the sky was falling in the autumn of 2008, bond futures took off. The rally in the bond markets in this period was nothing short of amazing. The German Schatz (see Figure 6.114) was just one of many highly profitable trades in this sector. The long bonds generated an incredible 40% on the bottom line during the last few months of the year while most of the world’s investors were losing on the same scale. 


Figure 6.114 Extreme trend in German Schatz


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/59e053921db63df72380be5fdaac447fd56d1d28861843a543d8d98536e105a0.jpg)



The fact that we failed to make money on equity futures in the strongest bear market in recent history begs the question as to what went wrong. Figure 6.115 shines some light on this problem. What may appear visually as small counter moves that kicked out our positions were in reality huge swings. Among other failed trades in the equity sector during this time, we entered into a short EuroStoxx 50 position in early October, after which the market quickly dropped 20% in just a few days. However, in the following week and a half, the same index gained 25%, triggering our stops before dropping down 25% to new lows. This kind of volatility is unprecedented and extremely scary, for lack of a better word. The money this year was not in the equity trend and we should be glad that sector only ended up with small losses for us.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/39d373db8bce88d62376e10f5d056a8e25ebf7a7903e6d5390df3c66176cc779.jpg)



Before this year we had gained almost 2,000% since the inception of our strategy in 1990, but given the extreme performance we were now up to almost 4,000% (see Tables 6.75 and 6.76). With the year’s extreme performance followed extreme rewards. In this remarkable year, the total fees collected by the manager amounted to a whopping 21% of the initial money in the fund at the start of the year. Of course, investors were probably not complaining either, having seen that most people in the world lost half their wealth in the stock market while they doubled their money in your fund.



Table 6.75 Sector performance 2008


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>7.4</td><td>6.8</td><td>12.4</td><td>-0.9</td><td>41.6</td><td>67.4</td></tr><tr><td>Short</td><td>15.0</td><td>15.5</td><td>25.0</td><td>-1.8</td><td>2.8</td><td>56.5</td></tr><tr><td>All</td><td>22.4</td><td>22.3</td><td>37.4</td><td>-2.7</td><td>44.4</td><td>123.9</td></tr></table>


Table 6.76 Results 2008


<table><tr><td>Year</td><td>2008</td></tr><tr><td>Starting NAV</td><td>1847.7</td></tr><tr><td>Trading result</td><td>123.9%</td></tr><tr><td>Interest income</td><td>2.9%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-2.5%</td></tr><tr><td>Performance fee</td><td>-18.5%</td></tr><tr><td>Net result</td><td>105.0%</td></tr><tr><td>Ending NAV</td><td>3787.1</td></tr></table>


2009


The spectacular end of 2008 was driven primarily by the long rates sector, and so we still held a very large exposure to this sector going into 2009. At the same time we had a short bias on the equity markets, but only three positions and so not a very large bet. The commodities were more interesting, where we were essentially short across the board on everything from oil to platinum to lean hogs (see Tables 6.77 and 6.78 and Figure 6.116). 


Figure 6.116 Sector allocation 2009


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/7bfa046ee36d310d1d8cbc632f1f3338748afabb038eccf5b7d0fd543bb6da6a.jpg)



Table 6.77 Initial portfolio 2009


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Lean hogs</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Sugar</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>Oats</td><td>Short</td><td>Agricultural commodities</td></tr><tr><td>EUR/GBP</td><td>Long</td><td>Currencies</td></tr><tr><td>Japanese yen</td><td>Long</td><td>Currencies</td></tr><tr><td>British pound</td><td>Short</td><td>Currencies</td></tr><tr><td>Canadian Bankers’ Acceptance</td><td>Long</td><td>Currencies</td></tr><tr><td>EuroStoxx 50</td><td>Short</td><td>Equities</td></tr><tr><td>FTSE 100</td><td>Short</td><td>Equities</td></tr><tr><td>CAC 40</td><td>Short</td><td>Equities</td></tr><tr><td>Palladium</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Copper</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Crude oil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Gasoline</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Heating oil</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Natural gas</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>Platinum</td><td>Short</td><td>Non-agricultural commodities</td></tr><tr><td>German Bund</td><td>Long</td><td>Rates</td></tr><tr><td>US 10-year note</td><td>Long</td><td>Rates</td></tr><tr><td>Long gilt</td><td>Long</td><td>Rates</td></tr><tr><td>Eurodollar</td><td>Long</td><td>Rates</td></tr><tr><td>German Schatz</td><td>Long</td><td>Rates</td></tr><tr><td>Euribor</td><td>Long</td><td>Rates</td></tr><tr><td>Euroswiss</td><td>Long</td><td>Rates</td></tr><tr><td>US 2-year note</td><td>Long</td><td>Rates</td></tr><tr><td>Short sterling</td><td>Long</td><td>Rates</td></tr></table>


Table 6.78 Initial sector allocation 2009


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>3</td><td>1</td><td>4</td></tr><tr><td>Agricultural commodities</td><td>0</td><td>3</td><td>3</td></tr><tr><td>Non-agricultural commodities</td><td>0</td><td>8</td><td>8</td></tr><tr><td>Equities</td><td>0</td><td>3</td><td>3</td></tr><tr><td>Rates</td><td>9</td><td>0</td><td>9</td></tr><tr><td>Total</td><td>12</td><td>15</td><td>27</td></tr></table>

After the excitement we witnessed in 2008 it was just as well that this year started off rather undramatically. Up until March there were hardly any movements at all in the fund and we did not see either +5% or –5% (as Figure 6.117 shows). At the same time the global stock markets continued to fall and lost almost 30% from the start of the year. The grace period unfortunately ended at the start of the second quarter and a group of currency bets that were sensitive towards a strong US currency all fell back down hard along with the dollar. The fund went below –10% in late March and most positions were stopped out, leaving a low risk portfolio with little chance of coming back up until new trends emerged. These trends did not come around until July and August in the shape of long equities, long rates and antidollar positions. Together these sectors helped the fund to reach up to the zero line again in October and it stayed around this line under quite low volatility for most of the year, but fell back down to –5.8% in December where it finally ended the year. 


Figure 6.117 Strategy performance 2009


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/04fd0ff843c75a928279bc52d50fee5e191daec88561e29a1d8b1b1b96af6dd2.jpg)



All in all, 2009 was a really slow and uneventful year, at least in comparison to what we had just gone through. With the strong equity rebound, the results unfortunately looked quite bad in comparison although the properly informed investor should not expect you to beat the equity indices in a rebound market.


The only significant number in this year’s roundup (in Figures 6.118 to 6.120) was the loss on the short currencies, which for the most part meant long US dollar bets. With the large swings in the dollar index this particular year, that was not completely surprising though. Small gains were seen in equities and rates but they were eaten up by the currencies and commodities. All in all, quite an uneventful year. 


Figure 6.118 Sector performance 2009


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/42efd8f3eff3a3ad48f7e72997656b81a38e7e6ce62b03cefe0454e89efd0bcf.jpg)



Figure 6.119 Long sector performance 2009


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/796e42a0bdad78fff19addbda149907d423bbe9f65d06a4f7a1fd2b882d06187.jpg)



Figure 6.120 Short sector performance 2009


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/25f073284b1da49c38b0bf4edab4b5d381b5ec3428208393cf445bb0e195f18b.jpg)


The live cattle situation was emblematic of the trendless markets we experienced across all markets in 2009 (see Figure 6.121). The strategy tried several entries, both on the long and short side, and most of them ended up hitting their stop points soon after. It can be difficult to keep taking the trades in situations like this, when you have just lost five times in a row on the same market and you see a completely trendless choppy market in front of you. It is imperative, however, that you keep on following the original plan. If you go off the reservation and selectively skip some trades, sooner or later you will end up skipping that one trade that would have made up for the whole losing streak. 


Figure 6.121 Lack of trends in live cattle in 2009


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/49b71880129f1f1e4d96fca56886c91b3c402c2e6d3217ada4e1360a9e90b80b.jpg)



Having lost money for our clients this year, there was no performance fee paid to the manager (see Tables 6.79 and 6.80). You should always make sure that you budget for this scenario and that you are able to cover all costs and salaries even without a performance fee.


Table 6.79 Sector performance 2009 

<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>-0.1</td><td>1.0</td><td>-0.4</td><td>5.6</td><td>3.3</td><td>9.4</td></tr><tr><td>Short</td><td>-5.6</td><td>-4.0</td><td>-1.4</td><td>-3.3</td><td>-0.8</td><td>-15.2</td></tr><tr><td>All</td><td>-5.8</td><td>-3.1</td><td>-1.8</td><td>2.3</td><td>2.5</td><td>-5.8</td></tr></table>

Table 6.80 Results 2009 

<table><tr><td>Year</td><td>2009</td></tr><tr><td>Starting NAV</td><td>3787.1</td></tr><tr><td>Trading result</td><td>-5.8%</td></tr><tr><td>Interest income</td><td>0.2%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.5%</td></tr><tr><td>Performance fee</td><td>0.0%</td></tr><tr><td>Net result</td><td>-7.5%</td></tr><tr><td>Ending NAV</td><td>3504.2</td></tr></table>

As the other fund costs have to be paid even in a losing year, the loss to the clients was increased even further and the final number they saw in their account statements was –7.5% and the interest income that helped us so many times before was nowhere to be seen. The yields dropped like a stone around this time and you got almost nothing at all for lending out your money anymore. The only reason to keep doing so with these yield levels was that the cash was safer with the government than with your prime broker. 

Not a very good year, and we hope our clients were still happy with the memory of the 2008 performance. You may be surprised over how short a time some clients remember good performance and how long they remember the bad. Constant communication and openness about the investment process helps in setting proper expectations and is likely to make the clients more inclined to stay with you during bad periods like this. 

## 2010

After the equity rally in 2009 we had built up a large portfolio of instruments in that sector and it was now the largest sector holding in our portfolio with longs primarily in Europe and the US (see Tables 6.81 and 6.82 and Figure 6.122). We also still held a fairly large bet that yields would continue down, but the remaining positions were more scattered. There were longs in various commodities from lean hogs to palladium, but they did not represent as large a risk factor as the equity and rates positions. 

Figure 6.122 Sector allocation 2010 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/e2fe18db8bd00398cc399b84ca8ecec040a4a1a31f1148525a83eb09cd288d3b.jpg)



Table 6.81 Initial portfolio 2010


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Lean hogs</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Soybeans</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Sugar</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Cotton</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>EUR/JPY</td><td>Short</td><td>Currencies</td></tr><tr><td>EUR/CHF</td><td>Short</td><td>Currencies</td></tr><tr><td>EuroStoxx 50</td><td>Long</td><td>Equities</td></tr><tr><td>Russell 2000</td><td>Long</td><td>Equities</td></tr><tr><td>Nikkei 225</td><td>Long</td><td>Equities</td></tr><tr><td>DAX</td><td>Long</td><td>Equities</td></tr><tr><td>CAC 40</td><td>Long</td><td>Equities</td></tr><tr><td>S&amp;P 500</td><td>Long</td><td>Equities</td></tr><tr><td>FTSE 100</td><td>Long</td><td>Equities</td></tr><tr><td>Nasdaq 100</td><td>Long</td><td>Equities</td></tr><tr><td>Palladium</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Copper</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Euribor</td><td>Long</td><td>Rates</td></tr><tr><td>German Schatz</td><td>Long</td><td>Rates</td></tr><tr><td>Short sterling</td><td>Long</td><td>Rates</td></tr><tr><td>Eurodollar</td><td>Long</td><td>Rates</td></tr><tr><td>Euroswiss</td><td>Long</td><td>Rates</td></tr></table>


Table 6.82 Initial sector allocation 2010


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>0</td><td>2</td><td>2</td></tr><tr><td>Agricultural commodities</td><td>4</td><td>0</td><td>4</td></tr><tr><td>Non-agricultural commodities</td><td>2</td><td>0</td><td>2</td></tr><tr><td>Equities</td><td>8</td><td>0</td><td>8</td></tr><tr><td>Rates</td><td>5</td><td>0</td><td>5</td></tr><tr><td>Total</td><td>19</td><td>2</td><td>21</td></tr></table>

2010 started off a bit on the rocky side with a loss of over 5% in February when the equity markets turned down, bringing our futures in that sector down too (see Figure 6.123). The commodities also reversed trend at the same time, adding to the losses. Rates on the other hand just kept ticking on up and together with currency futures and some short commodities managed to bring the fund up to +5% early in the second quarter of the year. The shaky equity markets, however, managed to rain on the parade again and after some losses the fund found itself back at –5% in the third quarter. After this the commodity sectors took control of the performance generation almost completely and in a very short time the fund moved from –5% all the way up to +28% before falling back down to +10% after taking some stops. 


Figure 6.123 Strategy performance 2010


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/8557c1d9b7a4a5042fbadc14bf07c91a349792df7f98c88fb2fef890926d918d.jpg)


This can seem like a rather large giveback and the reason for it was the increasing correlation between the equities, agricultural commodities and non-agricultural commodities, which started building up in the third quarter. This phenomenon happens from time to time and usually leads to quick losses followed by sharp givebacks before stops are triggered. The strategy in its current form does not take these correlations into account when sizing positions, and therefore it can carry rather large risks at times. A bit of a rocky year then, but in the end the result stopped just above 17%, providing much needed relief after 2009. 

Equities ended up having another poor showing while the other sectors did okay (see Figures 6.124 to 6.126). The non-agricultural commodities landed at about zero but at least did not do any damage and all other sectors had quite nice returns. Losing 7% on equities was not very good but the year ended up double digits positive anyway. 

Figure 6.124 Sector performance 2010 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/2e037c0d62325bac551b8e1df0bef3cefa0f0a1746ce26425e2f961b709c0b7e.jpg)



Figure 6.125 Long sector performance 2010


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/40c8b4ff7b0fc62384da6af913c1a404adbecf76a9c8dc0388529d99f2cd3908.jpg)



Figure 6.126 Short sector performance 2010


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/0bc6ba50b39a0329d64e43c52f3889b8587f8de496543fcccf84846d652c95cc.jpg)


The rally in the agricultural sector was quite remarkable in the second half of the year and although as a group it did end up giving back some profits in November, it still had a very large positive contribution over this period. The sugar rally is a good example of what happened in this sector and it showed some very welcome profits for us. Notice in Figure 6.127 that because of our trend filter we were quite slow to get into the trade, but once we were in it we stayed until the trend was over. We got a bit lucky on this trade because we were extremely close to being stopped out in October. The stop point was penetrated intraday but we never saw a close on the wrong side. 


Figure 6.127 Sugar rally of 2010


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/8f073427433bfc8426a06c3397d888c4db79f82174b6fa547bbfc5fa146f8bda.jpg)



Remember that last year had a negative return, and so the performance fee for this year is calculated from the highest point at which the performance fee was last paid, which was at the end of 2008. We don’t get any performance fee simply for making up for the loss in 2009. The positive result of almost 17.5% was reduced to 14.3% after all costs, with almost no contribution from the money market yields this year but clearly beating equities and similar benchmarks, which should have left the customers reasonably satisfied (see Tables 6.83 and 6.84).



Table 6.83 Sector performance 2010


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>0.2</td><td>8.9</td><td>4.1</td><td>-1.8</td><td>9.5</td><td>20.9</td></tr><tr><td>Short</td><td>5.5</td><td>0.5</td><td>-3.2</td><td>-4.7</td><td>-1.6</td><td>-3.5</td></tr><tr><td>All</td><td>5.6</td><td>9.5</td><td>0.8</td><td>-6.5</td><td>7.9</td><td>17.4</td></tr></table>


Table 6.84 Results 2010


<table><tr><td>Year</td><td>2010</td></tr><tr><td>Starting NAV</td><td>3504.2</td></tr><tr><td>Trading result</td><td>17.4%</td></tr><tr><td>Interest income</td><td>0.2%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.6%</td></tr><tr><td>Performance fee</td><td>-1.1%</td></tr><tr><td>Net result</td><td>14.3%</td></tr></table>

## 2011

The final year to review started out with 21 positions and the largest theme was still the bull markets in the equity world. Some stops had been taken in the rates sector during the last half of 2010 as the bonds fell back on the equity rally, but a few of them were still in the portfolio (see Tables 6.85 and 6.86 and Figure 6.128). 


Figure 6.128 Sector allocation 2011


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/eaf8383b18be1e194f2c93b453bb05cfcca573f0de375e9c55d5d0025b31c776.jpg)



Table 6.85 Initial portfolio allocation 2011


<table><tr><td>Market</td><td>Direction</td><td>Sector</td></tr><tr><td>Lean hogs</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Soybeans</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Sugar</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>Cotton</td><td>Long</td><td>Agricultural commodities</td></tr><tr><td>EUR/JPY</td><td>Short</td><td>Currencies</td></tr><tr><td>EUR/CHF</td><td>Short</td><td>Currencies</td></tr><tr><td>EuroStoxx 50</td><td>Long</td><td>Equities</td></tr><tr><td>Russell 2000</td><td>Long</td><td>Equities</td></tr><tr><td>Nikkei 225</td><td>Long</td><td>Equities</td></tr><tr><td>DAX</td><td>Long</td><td>Equities</td></tr><tr><td>CAC 40</td><td>Long</td><td>Equities</td></tr><tr><td>S&amp;P 500</td><td>Long</td><td>Equities</td></tr><tr><td>FTSE 100</td><td>Long</td><td>Equities</td></tr><tr><td>Nasdaq 100</td><td>Long</td><td>Equities</td></tr><tr><td>Palladium</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Copper</td><td>Long</td><td>Non-agricultural commodities</td></tr><tr><td>Euribor</td><td>Long</td><td>Rates</td></tr><tr><td>German Schatz</td><td>Long</td><td>Rates</td></tr><tr><td>Short sterling</td><td>Long</td><td>Rates</td></tr><tr><td>Eurodollar</td><td>Long</td><td>Rates</td></tr><tr><td>Euroswiss</td><td>Long</td><td>Rates</td></tr></table>


Table 6.86 Initial sector allocation 2011


<table><tr><td></td><td>Long</td><td>Short</td><td>Total</td></tr><tr><td>Currencies</td><td>0</td><td>2</td><td>2</td></tr><tr><td>Agricultural commodities</td><td>4</td><td>0</td><td>4</td></tr><tr><td>Non-agricultural commodities</td><td>2</td><td>0</td><td>2</td></tr><tr><td>Equities</td><td>8</td><td>0</td><td>8</td></tr><tr><td>Rates</td><td>5</td><td>0</td><td>5</td></tr><tr><td>Total</td><td>19</td><td>2</td><td>21</td></tr></table>

The first couple of months of 2011 were relatively eventless. The long equity positions were ticking in money on the continuing rally while currency positions got stopped out early. The first scare of this year came in March, when the Japanese disaster hit: an earthquake, followed by a massive tsunami wave, followed by a nuclear disaster threatening Tokyo. This horrible disaster sent fear throughout the world and naturally triggered a large amount of panic selloffs. The fund lost about 4% in a day and a little more in the following days, and our equity positions were quickly sold. Having seen gains of almost 7%, the fund lost 10% from that peak in early March (see Figure 6.129). 


Figure 6.129 Strategy performance 2011


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/c8b990f21e88f7a3eced336f655fe2c976b6c4dfe3f95e67b70655a48b2de238.jpg)


In April the equity curve started climbing again, driven mainly by oil-related futures. The heating oil in particular had been a very profitable position for some time and we also held long positions in crude oil, gasoline and gasoil. This was when the second setback of 2011 hit us. A surprise margin requirement increase from the exchanges in these energy futures caused a sudden and violent move to the downside as speculators trading on thin margins were forced to cover their positions. The move in heating oil was the worst with an unprecedented move of over 8% in a single day (see Figure 6.130). This highlights a potential weakness of the robust but simple strategy rules we were working with at this point. The day before this outsized move, the stop point for heating oil was almost hit, only a few cents away. As the 

strategy operates only on a closing basis in its current shape, the actual stop was not taken until the day after the large drop and by that point the real damage was almost three times as large as the theoretical stop. 

Figure 6.130 Heating oil gapping far below stop point 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/30be8a1671fa4302f01a86560d3383202c399a8bd25280b39ed1872ede56c1b7.jpg)


During the summer months the fund stayed mostly under the waterline, briefly seeing small profits but quickly losing them again. The worst reading of the year came in late July, at almost 8% down. August, however, turned out much better because we now had time to build up bear positions again as the European Union’s financial situations deteriorated and the equity declines continued. The profits in short equity futures and long rates futures paid off very quickly during August and continued to do well in September, making the fund reach a high of nearly 20% year to date by the end of that month. 

As so often happens in sharp bear markets, there was a sudden and strong reversal starting in October of 2011. Our short equity futures were closed out after losing part of their profits and most of the long rates closed out soon after. Our portfolio of 30 positions was reduced to a mere eight in a matter of weeks, all of them taking losses during this time. The correlations between sectors grew very high at this point and essentially all sectors contributed to the hard landing in late October. The remainder of the year was relatively trendless, with losses taken on several sectors while attempting to enter potential new trends that never materialised. 

In the end, only the rates sector ended up making money in 2011; the currencies netted zero and all other sectors lost (see Figures 6.131 to 6.133). The largest loss was in the long equities positions that were held early in the year and we failed to exploit the bear market, which was considerably shorter than the one seen in 2008. 

Figure 6.131 Sector performance 2011 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/417a2ed3efa33799dc4658a556f6f8f61d12cb10f84c06bd984b714680843be4.jpg)



Figure 6.132 Long sector performance 2011


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/ca7c949382008a2a7c597647e352b39ffcf33d8156cbde334a2eb2123f33d17a.jpg)



Figure 6.133 Short sector performance 2011


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/5f0d025a711e7e3970627190b14a5b743ab2a3f16c1442e7aaef18d7c922a743.jpg)


There were many highly profitable positions in the long rates sector during 2011 but none were as eventful as the Euroswiss trade, as Figure 6.134 illustrates. Again, this is the three months money market rate we are talking about here and not the EUR/CHF currency cross. Already in July the futures indicated a rate so close to zero that there should be very little possible theoretical profits in being long in it. Then during the height of the European Union crisis in August, money kept pouring into the safe haven Swissie currency and the short-term rates markets go absolutely crazy. For a couple of weeks, this market experienced unprecedented daily price moves, shooting up to levels that made absolutely no sense, but they did it anyhow. As the price moved up above 100, the implication was that banks were willing to pay for the privilege to lend out money to each other on an unsecured basis. This was of course nuts and the situation did not last long. Still, our trending strategy made very welcome profits on this position before getting out after the huge spike up. 


Figure 6.134 Euroswiss goes ballistic in 2011


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/879fac13-6dc3-4c09-9bac-038398b89275/40ccc8a10a6ae56ad207f6dd42ebb80d8ac3d870770dda3962717e09e3eb26e7.jpg)


It may seem like an unhappy ending to leave off with a bad year like 2011 (check out the numbers in Tables 6.87 and 6.88). Another way to look at it is, of course, that there are not usually many bad years in a row and this may prove to be a good time to get into the trend-following futures business. 


Table 6.87 Sector performance 2011


<table><tr><td></td><td>Currencies (%)</td><td>Agricultural commodities (%)</td><td>Non-agricultural commodities (%)</td><td>Equities (%)</td><td>Rates (%)</td><td>Total (%)</td></tr><tr><td>Long</td><td>1.7</td><td>-4.8</td><td>0.4</td><td>-6.3</td><td>13.6</td><td>4.6</td></tr><tr><td>Short</td><td>-1.7</td><td>-2.4</td><td>-1.7</td><td>0.9</td><td>-4.8</td><td>-9.7</td></tr><tr><td>All</td><td>0.0</td><td>-7.2</td><td>-1.3</td><td>-5.4</td><td>8.8</td><td>-5.1</td></tr></table>


Table 6.88 Results 2011


<table><tr><td>Year</td><td>2011</td></tr><tr><td>Starting NAV</td><td>4004.8</td></tr><tr><td>Trading result</td><td>-5.1%</td></tr><tr><td>Interest income</td><td>0.2%</td></tr><tr><td>Misc. fees</td><td>-0.5%</td></tr><tr><td>Management fee</td><td>-1.5%</td></tr><tr><td>Performance fee</td><td>0.0%</td></tr><tr><td>Net result</td><td>-6.9%</td></tr><tr><td>Ending NAV</td><td>3728.3</td></tr></table>

All in all, an investor who joined in the beginning of 1990 with an investment of US$10,000 and stayed throughout the whole ride would now have close to US$400,000 worth of shares in the fund. This translates to an annual compounded return of almost 18% and this is during a period when the world stock markets returned less than 5% per annum. The traditional equity investor would also have seen maximum losses of almost 60% while the ones who invested in this futures strategy saw only a little over 20% loss as the worst. 

It has been a tough ride with many scary years, but I am quite sure that it was scarier for those who stayed long equities, and who ended up making much less money for it. 

## CONCLUSIONS OF YEAR BY YEAR REVIEW

I spent many pages going over each year in this chapter to make sure anyone starting out with this trading style fully understood the true price of the returns in terms of volatility, drawdowns and long periods of sleepless nights. When looking at simulation reports and long-term equity curves, everything looks very nice and perhaps overly so. Even when you look back at some years of monthly figures for your actual trading results, it could look really nice and not even hint at how tough it was to stick with the strategy during that time. This is also what you see when you look at the track record of a futures fund. You see the nice-looking summary, but these guys likely had some tough times in the meanwhile. 

Look again at the monthly and yearly returns for the strategy over these years in Table 6.89. This information should now look much more scary than it did before you read this chapter. The next time you look through the track record of a CTA fund or analyse the results from your simulations, you should be able to relate to the different years and figure out what might have happened to create the results, good or bad. 

Table 6.89 Monthly returns for the core strategy 

<table><tr><td></td><td>Jan (%)</td><td>Feb (%)</td><td>Mar (%)</td><td>Apr (%)</td><td>May (%)</td><td>Jun (%)</td><td>Jul (%)</td><td>Aug (%)</td><td>Sep (%)</td><td>Oct (%)</td><td>Nov (%)</td><td>Dec (%)</td><td>Year (%)</td></tr><tr><td>1990</td><td>-1.6</td><td>2.5</td><td>7.6</td><td>5.6</td><td>-6.5</td><td>3.4</td><td>6.2</td><td>9.6</td><td>6.3</td><td>-8.3</td><td>1.4</td><td>1.5</td><td>29.6</td></tr><tr><td>1991</td><td>0.7</td><td>1.1</td><td>0.6</td><td>-4.6</td><td>1.1</td><td>0.1</td><td>-3.3</td><td>1.1</td><td>3.9</td><td>4.3</td><td>1.2</td><td>16.8</td><td>23.8</td></tr><tr><td>1992</td><td>-4.9</td><td>1.6</td><td>0.3</td><td>-2.4</td><td>4.3</td><td>1.5</td><td>7.2</td><td>6.0</td><td>-6.0</td><td>-3.4</td><td>2.7</td><td>-0.2</td><td>6.0</td></tr><tr><td>1993</td><td>1.6</td><td>9.9</td><td>0.6</td><td>-0.2</td><td>2.9</td><td>0.2</td><td>5.1</td><td>-2.7</td><td>-5.4</td><td>5.2</td><td>2.1</td><td>13.4</td><td>36.3</td></tr><tr><td>1994</td><td>-6.7</td><td>-5.0</td><td>5.1</td><td>-2.6</td><td>4.1</td><td>-1.4</td><td>-3.2</td><td>-4.2</td><td>0.4</td><td>-4.0</td><td>6.1</td><td>-4.2</td><td>-15.4</td></tr><tr><td>1995</td><td>-1.3</td><td>2.5</td><td>9.2</td><td>1.2</td><td>5.9</td><td>-1.1</td><td>-2.6</td><td>-3.0</td><td>2.0</td><td>-1.2</td><td>1.5</td><td>13.8</td><td>28.8</td></tr><tr><td>1996</td><td>-0.7</td><td>-8.3</td><td>5.9</td><td>10.0</td><td>-3.2</td><td>2.0</td><td>-6.6</td><td>3.3</td><td>7.9</td><td>7.6</td><td>10.2</td><td>-6.6</td><td>20.6</td></tr><tr><td>1997</td><td>9.2</td><td>2.8</td><td>-3.7</td><td>-5.0</td><td>-2.6</td><td>-0.4</td><td>11.4</td><td>-11.0</td><td>-0.2</td><td>-2.6</td><td>1.8</td><td>10.5</td><td>8.0</td></tr><tr><td>1998</td><td>0.7</td><td>5.7</td><td>2.5</td><td>-1.4</td><td>4.8</td><td>2.2</td><td>5.2</td><td>15.4</td><td>-0.5</td><td>-0.9</td><td>2.1</td><td>3.6</td><td>46.2</td></tr><tr><td>1999</td><td>2.1</td><td>3.2</td><td>-5.1</td><td>2.2</td><td>-8.3</td><td>4.4</td><td>2.4</td><td>0.5</td><td>1.5</td><td>-10.4</td><td>6.8</td><td>9.5</td><td>7.3</td></tr><tr><td>2000</td><td>-7.2</td><td>3.7</td><td>-7.8</td><td>3.3</td><td>4.4</td><td>2.9</td><td>-0.3</td><td>8.0</td><td>-4.1</td><td>-2.7</td><td>2.8</td><td>12.4</td><td>14.2</td></tr><tr><td>2001</td><td>-0.1</td><td>0.8</td><td>13.3</td><td>-11.6</td><td>2.2</td><td>-1.3</td><td>0.5</td><td>6.3</td><td>22.1</td><td>6.8</td><td>-4.2</td><td>0.3</td><td>36.2</td></tr><tr><td>2002</td><td>-4.8</td><td>-1.0</td><td>-4.2</td><td>-2.6</td><td>7.2</td><td>11.1</td><td>11.9</td><td>3.1</td><td>8.1</td><td>-9.6</td><td>-1.0</td><td>9.1</td><td>27.4</td></tr><tr><td>2003</td><td>8.6</td><td>7.3</td><td>-7.4</td><td>8.4</td><td>6.6</td><td>-6.0</td><td>4.5</td><td>3.0</td><td>-3.9</td><td>3.1</td><td>-4.7</td><td>7.9</td><td>28.7</td></tr><tr><td>2004</td><td>3.2</td><td>10.4</td><td>1.3</td><td>-9.1</td><td>-4.4</td><td>-3.0</td><td>-0.5</td><td>-4.8</td><td>1.3</td><td>1.5</td><td>9.8</td><td>-0.8</td><td>3.1</td></tr><tr><td>2005</td><td>-4.4</td><td>0.3</td><td>-4.0</td><td>-2.3</td><td>1.1</td><td>2.3</td><td>2.4</td><td>-0.8</td><td>-1.1</td><td>2.1</td><td>10.1</td><td>-0.4</td><td>4.6</td></tr><tr><td>2006</td><td>9.1</td><td>-4.2</td><td>9.7</td><td>7.3</td><td>-6.6</td><td>-3.7</td><td>-4.5</td><td>3.8</td><td>-0.8</td><td>5.8</td><td>3.1</td><td>1.4</td><td>20.5</td></tr><tr><td>2007</td><td>2.4</td><td>-9.1</td><td>-3.0</td><td>7.7</td><td>10.6</td><td>6.1</td><td>-8.0</td><td>-7.0</td><td>8.2</td><td>7.4</td><td>-3.7</td><td>-0.7</td><td>8.6</td></tr><tr><td>2008</td><td>8.9</td><td>22.4</td><td>-5.1</td><td>-3.1</td><td>5.6</td><td>2.6</td><td>-11.7</td><td>0.5</td><td>5.9</td><td>41.3</td><td>6.6</td><td>9.0</td><td>104.9</td></tr><tr><td>2009</td><td>-2.1</td><td>0.7</td><td>-11.1</td><td>-2.5</td><td>4.5</td><td>-4.4</td><td>3.0</td><td>4.8</td><td>3.3</td><td>-3.4</td><td>7.7</td><td>-6.7</td><td>-7.5</td></tr><tr><td>2010</td><td>-3.4</td><td>1.7</td><td>3.6</td><td>1.4</td><td>-3.3</td><td>0.7</td><td>-5.3</td><td>2.3</td><td>3.4</td><td>10.6</td><td>-3.1</td><td>6.0</td><td>14.3</td></tr><tr><td>2011</td><td>-1.1</td><td>3.2</td><td>-2.7</td><td>9.9</td><td>-9.1</td><td>-4.6</td><td>2.8</td><td>11.1</td><td>5.0</td><td>-14.7</td><td>-3.5</td><td>-0.6</td><td>-7.0</td></tr></table>

7 

# Reverse Engineering the Competition

So far we have seen that if you are prepared to accept volatile performance with large swings in a short amount of time, you can receive very strong long-term results as a reward. The volatility in some years may seem excessive to many people and some may be quick to rule these strategies as simply too risky to be practical. At the same time, we can also show that as volatile as trend-following futures trading can be, you are likely to get even higher volatility if you just buy and hold equities and that alternative gives you significantly lower returns. I am sure there are readers who are a little sceptical at this point, wondering whether you can run such a rocket ship of a strategy in real life and whether it is plausible that the large futures hedge funds are doing these things. Surely they must be doing something tremendously more complex, given their massive research budgets and enormous profitability? 

The short answer to that is: not really. Most of them do what I describe in this book, with only minor variations. By this I don’t mean that they are using the exact rules I present or that they trade only one simple model in this manner. The point is that their returns can be replicated quite closely by using the model from this book. Any variations, tweaks and combinations of models that they may be using are not enough to differentiate them significantly from simple trend-following models such as our core strategy. 

<!-- === Source: MinerU_markdown_Following_the_Trend－_Diversified_Managed_Futures_Trading._Andreas_Clenow_2013_201_2122155849542639630.md (Page 201) === -->

There are not a whole lot of different ways that trend following can be done and whatever the actual rules these funds use, they are close enough that our core strategy can be used as an approximation. 

In this chapter I start by making a few minor variations to the core strategy that we have been using so far and then I demonstrate how each of these variations correspond to different actual futures hedge funds. By simply matching the output of our strategy with those of the established funds, we can reverse engineer them and find out what their core strategy is about and how it differs from ours. There is no point in trying to get an exact match because they all have various tweaks that are impossible to replicate with precision and many of them also run multiple time frames or other variations. It is also a reasonable assumption that they have changed or evolved their strategy over the years. We can still get close enough with our model though. 

## INVESTMENT UNIVERSES

The simplified investment universe we have used up to this point is the largest differentiator between us and actual CTA hedge funds. In order to model and reverse engineer these funds properly we must first create a few additional variants of investment universes that are more realistic and more likely to resemble what these funds actually use. 

The result over time of a trend-following strategy is very much dependent on its mix of markets in the investment universe. The investment universe we used so far is quite small and designed to have equal weights of each sector. If there is no clear reason otherwise, it is preferable to have a larger investment universe and thereby more opportunities to find trends and to diversify. The rational for keeping the investment universe small is when you have a very limited amount of assets under management. Doubling the number of markets in the investment universe roughly doubles the amount of risk on your strategy, so in order to keep risk level steady you need to cut the risk factor in the position-sizing formula in half. If you have only, say, US$2 million under management, however, you may find yourself getting trade signals to buy or sell fractions of contracts and if you round off the size, the error factor will be significant. If you start off very small, look for mini contracts to trade instead of the big contracts, but be careful to verify that they are liquid enough. 

As a reminder, Table 7.1 shows the original investment universe we have used up to this point. This was deliberately chosen as an equal-weighted universe with the same amount of contracts in each market, not because this necessarily gives the best results but because it makes it easier to see the effect of sector performance over the years in Chapter 6. 


Table 7.1 Equal-Weighted Investment Universe


<table><tr><td>Agricultural</td><td>Non-agricultural</td><td>Currencies</td><td>Equities</td><td>Rates</td></tr><tr><td>Cotton</td><td>Gasoil</td><td>AUD/USD</td><td>CAC 40</td><td>Bunt</td></tr><tr><td>Corn</td><td>Crude oil</td><td>GBP/USD</td><td>DAX</td><td>Schatz</td></tr><tr><td>Lumber</td><td>Heating oil</td><td>EUR/USD</td><td>FTSE 100</td><td>Long gilt</td></tr><tr><td>Live Cattle</td><td>Natural gas</td><td>JPY/USD</td><td>HS China Enterprises</td><td>Canadian Bankers&#x27; Acceptance</td></tr><tr><td>Lean hogs</td><td>Gasoline</td><td>NZD/USD</td><td>Hang Seng</td><td>US 2-year note</td></tr><tr><td>Oats</td><td>Gold</td><td>EUR/CHF</td><td>Nasdaq 100</td><td>US 10-year note</td></tr><tr><td>Rough rice</td><td>Copper</td><td>EUR/GBP</td><td>Nikkei 225</td><td>Eurodollar</td></tr><tr><td>Soybeans</td><td>Palladium</td><td>EUR/JPY</td><td>S&amp;P 500</td><td>Euroswiss</td></tr><tr><td>Sugar</td><td>Platinum</td><td>CHF/USD</td><td>EuroStoxx 50</td><td>Euribor</td></tr><tr><td>Wheat</td><td>Silver</td><td>CAD/USD</td><td>Russell 2000</td><td>Short sterling</td></tr></table>

Although it is a safe bet that there are a plethora of market combinations traded by futures funds, I construct four sets of investment universes (in addition to the equal-weighted version we have used so far), which I believe is enough to approximate what most funds use. Using easy to remember names, I simply call the first one the Large Universe (see Table 7.2). It contains 68 markets all in all, holding the largest weights in commodities and rates. Using this amount of markets we should get a high degree of diversification and well-rounded exposure to all sectors. 


Table 7.2 Large Universe


<table><tr><td>Agricultural</td><td>Non-agricultural</td><td>Currencies</td><td>Equities</td><td>Rates</td></tr><tr><td>Azuki red beans</td><td>Copper</td><td>AUD/USD</td><td>CAC 40</td><td>AU 10Y</td></tr><tr><td>Coffee</td><td>Crude oil</td><td>CAD/USD</td><td>DAX</td><td>AU 3Y</td></tr><tr><td>Corn</td><td>Gasoil</td><td>CHF/USD</td><td>EuroStoxx</td><td>AU 90 Day</td></tr><tr><td>Cotton</td><td>Gasoline</td><td>EUR/USD</td><td>FTSE 100</td><td>Bobl</td></tr><tr><td>Lean hogs</td><td>Gold</td><td>GBP/USD</td><td>Hang Seng</td><td>Bund</td></tr><tr><td>Live cattle</td><td>Heating oil</td><td>JPY/USD</td><td>HS China Enterprises</td><td>CD 10Y</td></tr><tr><td>Lumber</td><td>Natural gas</td><td>MXN/USD</td><td>IBEX 35</td><td>Canadian Bankers&#x27; Acceptance</td></tr><tr><td>Oats</td><td>Palladium</td><td>NOK/USD</td><td>MSCI Taiwan</td><td>Euribor</td></tr><tr><td>Orange juice</td><td>Platinum</td><td>NZD/USD</td><td>Nasdaq 100</td><td>Eurodollar</td></tr><tr><td>Rapeseed</td><td>Silver</td><td>SEK/USD</td><td>Nikkei 225</td><td>Euroswiss</td></tr><tr><td>Rough rice</td><td></td><td>ZAR/USD</td><td>S&amp;P 500</td><td>JP 10Y</td></tr><tr><td>Rubber</td><td></td><td></td><td>S&amp;P 60</td><td>Long gilt</td></tr><tr><td>Soybean meal</td><td></td><td></td><td>SPI 200</td><td>Schatz</td></tr><tr><td>Soybeans</td><td></td><td></td><td></td><td>Short sterling</td></tr><tr><td>Sugar</td><td></td><td></td><td></td><td>US 10Y</td></tr><tr><td>Wheat</td><td></td><td></td><td></td><td>US 2Y</td></tr><tr><td></td><td></td><td></td><td></td><td>US 30Y</td></tr><tr><td></td><td></td><td></td><td></td><td>US 5Y</td></tr></table>

As I hope you noticed in the year by year review in Chapter 6, the equity sector can be particularly problematic when it comes to diversification. In a normal, orderly market you may get reasonable diversification from trading multiple-equity markets but the crux is that once the markets come under pressure and the trends reverse, the correlation between individual equity markets quickly approaches 1. This phenomenon can happen in other sectors as well although the problem is by far the most severe in this equity sector. It may be wise to avoid risk concentrations in this sector and one way of doing that is simply to reduce the number of markets included in this category. The second investment universe with its 62 markets is therefore the same as the Large Universe, with the exception that it has less equity markets, and therefore it is called the Large Universe, Reduced Equities (see Table 7.3). 

Table 7.3 Large Universe, Reduced Equities 

<table><tr><td>Agricultural</td><td>Non-agricultural</td><td>Currencies</td><td>Equities</td><td>Rates</td></tr><tr><td>Azuki red beans</td><td>Copper</td><td>AUD/USD</td><td>DAX</td><td>AU 10Y</td></tr><tr><td>Coffee</td><td>Crude oil</td><td>CAD/USD</td><td>EuroStoxx</td><td>AU 3Y</td></tr><tr><td>Corn</td><td>Gasoil</td><td>CHF/USD</td><td>Hang Seng</td><td>AU 90 day</td></tr><tr><td>Cotton</td><td>Gasoline</td><td>EUR/USD</td><td>MSCI Taiwan</td><td>Bobl</td></tr><tr><td>Lean hogs</td><td>Gold</td><td>GBP/USD</td><td>Nasdaq 100</td><td>Bund</td></tr><tr><td>Live cattle</td><td>Heating oil</td><td>JPY/USD</td><td>Nikkei 225</td><td>Canadian Bankers&#x27; Acceptance</td></tr><tr><td>Lumber</td><td>Natural gas</td><td>MXN/USD</td><td>S&amp;P 500</td><td>CD 10Y</td></tr><tr><td>Oats</td><td>Palladium</td><td>NOK/USD</td><td></td><td>Euribor</td></tr><tr><td>Orange juice</td><td>Platinum</td><td>NZD/USD</td><td></td><td>Eurodollar</td></tr><tr><td>Rapeseed</td><td>Silver</td><td>SEK/USD</td><td></td><td>Euroswiss</td></tr><tr><td>Rough rice</td><td></td><td>ZAR/USD</td><td></td><td>JP 10Y</td></tr><tr><td>Rubber</td><td></td><td></td><td></td><td>Long gilt</td></tr><tr><td>Soybean meal</td><td></td><td></td><td></td><td>Schatz</td></tr><tr><td>Soybeans</td><td></td><td></td><td></td><td>Short sterling</td></tr><tr><td>Sugar</td><td></td><td></td><td></td><td>US 10Y</td></tr><tr><td>Wheat</td><td></td><td></td><td></td><td>US 2Y</td></tr><tr><td></td><td></td><td></td><td></td><td>US 30Y</td></tr><tr><td></td><td></td><td></td><td></td><td>US 5Y</td></tr></table>

When funds become very large they often struggle with liquidity, which means that they have such large positions that they will make too big a footprint in many markets. When you hold a position representing 5% of a normal trading day’s volume, it will be difficult to get out of it without causing an adverse price move. As a result, many larger funds concentrate their trading on the financial futures where the liquidity is the highest. In currencies and rates you can move extremely large amounts with little to no footprint and therefore a very large fund may need an investment universe geared to these sectors. You will find the worst liquidity in the commodity sector and in particular in the agricultural part of it, and so we reduce that allocation in this Financially Heavy Investment Universe set (see Table 7.4). 

## Table 7.4 Financially Heavy Investment Universe

<table><tr><td>Agricultural</td><td>Non-agricultural</td><td>Currencies</td><td>Equities</td><td>Rates</td></tr><tr><td>Coffee</td><td>Copper</td><td>AUD/USD</td><td>CAC 40</td><td>AU 10Y</td></tr><tr><td>Corn</td><td>Crude oil</td><td>CAD/USD</td><td>DAX</td><td>AU 3Y</td></tr><tr><td>Cotton</td><td>Gasoil</td><td>CHF/USD</td><td>EuroStoxx</td><td>AU 90 Day</td></tr><tr><td>Lean hogs</td><td>Gasoline</td><td>EUR/USD</td><td>FTSE 100</td><td>Bobl</td></tr><tr><td>Live cattle</td><td>Gold</td><td>GBP/USD</td><td>Hang Seng</td><td>Bund</td></tr><tr><td>Soybean meal</td><td>Heating oil</td><td>JPY/USD</td><td>IBEX 35</td><td>Canadian Bankers&#x27; Acceptance</td></tr><tr><td>Soybean oil</td><td>Natural gas</td><td>MXN/USD</td><td>MSCI Taiwan</td><td>CD 10Y</td></tr><tr><td>Soybeans</td><td>Platinum</td><td>NOK/USD</td><td>Nasdaq 100</td><td>Euribor</td></tr><tr><td>Sugar</td><td>Silver</td><td>NZD/USD</td><td>Nikkei 225</td><td>Eurodollar</td></tr><tr><td>Wheat</td><td></td><td>SEK/USD</td><td>S&amp;P 500</td><td>Euroswiss</td></tr><tr><td></td><td></td><td>ZAR/USD</td><td>S&amp;P 60</td><td>JP 10Y</td></tr><tr><td></td><td></td><td></td><td>SPI 200</td><td>Long gilt</td></tr><tr><td></td><td></td><td></td><td></td><td>Schatz</td></tr><tr><td></td><td></td><td></td><td></td><td>Short sterling</td></tr><tr><td></td><td></td><td></td><td></td><td>US 10Y</td></tr><tr><td></td><td></td><td></td><td></td><td>US 2Y</td></tr><tr><td></td><td></td><td></td><td></td><td>US 30Y</td></tr><tr><td></td><td></td><td></td><td></td><td>US 5Y</td></tr></table>

Finally, we need an investment universe tilted more towards the commodities sectors because this is a popular theme among futures traders (see Table 7.5). The agricultural sector in particular is very interesting for diversified futures traders since it contains a large number of markets that have quite a low internal correlation. This provides many opportunities to get diversification effects and improve both profitability and risk. This kind of universe is difficult to trade for funds with over US$1 billion under management, but for a small-to-medium sized player this is an excellent sector to concentrate on. 


Table 7.5 Commodity Heavy Investment Universe


<table><tr><td>Agricultural</td><td>Non-agricultural</td><td>Currencies</td><td>Equities</td><td>Rates</td></tr><tr><td>Azuki Red Beans</td><td>Copper</td><td>AUD/USD</td><td>EuroStoxx 50</td><td>Bund</td></tr><tr><td>Coffee</td><td>Crude oil</td><td>CAD/USD</td><td>Hang Seng</td><td>Canadian Bankers&#x27; Acceptance</td></tr><tr><td>Corn</td><td>Gasoline</td><td>EUR/USD</td><td>Nasdaq 100</td><td>Eurodollar</td></tr><tr><td>Cotton</td><td>Gold</td><td>GBP/USD</td><td>Nikkei 225</td><td>Long gilt</td></tr><tr><td>Lean hogs</td><td>Heating oil</td><td>JPY/USD</td><td>S&amp;P 500</td><td>US 10-year note</td></tr><tr><td>Live cattle</td><td>Natural gas</td><td></td><td></td><td></td></tr><tr><td>Lumber</td><td>Palladium</td><td></td><td></td><td></td></tr><tr><td>Oats</td><td>Platinum</td><td></td><td></td><td></td></tr><tr><td>Orange juice</td><td>Silver</td><td></td><td></td><td></td></tr><tr><td>Rapeseed</td><td></td><td></td><td></td><td></td></tr><tr><td>Rough rice</td><td></td><td></td><td></td><td></td></tr><tr><td>Rubber</td><td></td><td></td><td></td><td></td></tr><tr><td>Soybean meal</td><td></td><td></td><td></td><td></td></tr><tr><td>Soybeans</td><td></td><td></td><td></td><td></td></tr><tr><td>Sugar</td><td></td><td></td><td></td><td></td></tr><tr><td>Wheat</td><td></td><td></td><td></td><td></td></tr></table>

COMPARING THE INVESTMENT UNIVERSES 

The five sets of market combinations in Tables 7.1 to 7.5 show a similar profile over a long enough time although for any given month or even year there may be a significant difference. As seen in the year by year review in Chapter 6, some years are completely driven by one or two sectors and having a smaller or larger weight of that sector can have a massive impact on the bottom line. Also bear in mind that the number of markets in each is not equal and that if everything else is held constant, the more markets we include in the investment universe, the higher the risk of the strategy and therefore all performance numbers will move up or down as well. It is therefore natural for a set with higher number instruments, such as our Large Universe, to have the highest return and the highest volatility. This is not really a problem because the overall risk level can be adjusted in the position-sizing formula to normalise the volatility, should you so desire. 

Comparing the five different investment universes, using the exact same strategy and risk factor, we find that they have very similar return profiles, although the larger sets tend to show higher numbers for the reasons just mentioned (see Table 7.6 and Figure 7.1). Note that if you compare the large set with the reduced equities, where the only difference is that less equity markets are included in the latter, the volatility adjusted performance goes up. This is an effect of the high internal correlation of the equity sector and the difficulty of getting sufficient diversifications out of it. It can be safely concluded that all these sets of markets are viable for trading a trend-following strategy on and there is no real right or wrong answer as to which is the best. 


Table 7.6 Comparing the investment universes


<table><tr><td>All data from Jan 1990 to Dec 2011</td><td>Equal-weighted investment universe</td><td>Large universe</td><td>Large universe, reduced equities</td><td>Commodity heavy investment universe</td><td>Financially heavy investment universe</td></tr><tr><td>Compounded annual return</td><td>17.9%</td><td>25.9%</td><td>24.9%</td><td>14.6%</td><td>21.9%</td></tr><tr><td>Worst drawdown</td><td>-20.2%</td><td>-29.2%</td><td>-25.4%</td><td>-19.2%</td><td>-27.9%</td></tr><tr><td>Drawdown/annualised return</td><td>-1.13</td><td>-1.13</td><td>-1.02</td><td>-1.38</td><td>-1.27</td></tr><tr><td>Percentage profitable months</td><td>63%</td><td>63%</td><td>63%</td><td>63%</td><td>64%</td></tr><tr><td>Best month</td><td>41.3%</td><td>45.8%</td><td>42.3%</td><td>28.1%</td><td>43.1%</td></tr><tr><td>Worst month</td><td>-14.7%</td><td>-18.4%</td><td>-16.7%</td><td>-12.0%</td><td>-17.5%</td></tr><tr><td>Sharpe, RF: 2.5%</td><td>0.74</td><td>0.87</td><td>0.88</td><td>0.70</td><td>0.78</td></tr><tr><td>Sortino ratio:</td><td>1.57</td><td>1.92</td><td>2.0</td><td>1.43</td><td>1.63</td></tr></table>


Figure 7.1 Performance comparison of the investment universes


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/71769a0a8ee9474eeb5cabe9acb1d7e9b7e25019b31eb29da6be1795d176df98.jpg)


Selecting the mix of markets to be traded is very much a matter of meeting individual tastes and the needs of the fund. Before starting to trade you need to spend much time analysing the implications of your choice of asset mix and be sure to select a combination that you are comfortable with. It is a very bad idea to start meddling with the investment universe once the fund is launched, at least unless it is done very carefully and for very good reasons. The risk is that you have a bad streak and decide to cut out markets based on a bad few months, only to miss the profits when the next few months turn out to be driven by the instruments you took out. Changing long-term strategy based on short-term results is a real danger that many traders fall into. 

## REPLICATING EXISTING FUNDS

When looking at the long-term track records of existing futures funds, it is clear that their strategies have changed over the course of the years. This evolution is both a natural process and in some ways also a necessary one. One reason to adapt strategy is simply that the initial success and capital appreciation will sooner or later start creating liquidity concerns. As the assets under management grow, it will be more and more difficult to trade some less-liquid markets and the fund manager needs to find ways around this problem. The obvious solutions are to add more markets to the investment universe in order to reduce the necessary size in each, to downsize or cut out markets with insufficient liquidity, to spread trades out over several days or to dedicate a large weight of the fund to the super liquid sectors such as currencies and rates. 

Another natural reason for modifying the strategy is that with success comes profit and that means larger research budgets, hiring of quant staff, inclusion of multiple strategy iterations, time frames and so on. These efforts will in most cases, if successful, result in lowering the volatility of the strategy slightly but not enough to make a massive impact. Still, if the fund is large enough it is still worth the effort and clients should be happy that they are spending some of the profits to help improve the results. Some funds though, as we will see later in this chapter, made changes that in retrospect do not appear to have panned out as planned. 

Then there may be cases where you are forced to make changes, such as when many European currency markets were merged into the Euro, and you could no longer trade the Deutsche mark futures. Looking back in the past 20 years there are several times when the asset mixes needed to be changed due to availability of markets, such as the fading volume and subsequent delisting of the pork belly futures. 

It is therefore unrealistic to expect a single strategy such as ours, using a single set of markets across the whole period, to match closely the entire history of an existing fund. What we can do, however, is to try to find a match for a prolonged period, to show what the fund was doing at that period, or to find a way to get a reasonable but less exact match for the whole period. In replicating the big name funds in this chapter, I use the exact same strategy that we have been using up until now, the very same used for the year by year analysis in the previous chapter. 

The point of this exercise is to demonstrate that many stellar futures funds with ‘Wizard’ status can in fact be replicated using a single simple trading strategy. They all add their own proprietary flair and an exact replication is not possible without risking extensive curve fitting and I doubt that would be very useful here. For this reason, I allow only three variables to be changed in our core strategy to try to match the results of these funds: 

• Investment universe: The five different sets of markets described above will be used and for each fund I pick the investment universe that seems to match the closest. 

Risk factor: The volatility of each fund can show significant variations compared to each other and to our core strategy. In order to replicate a fund, the risk factor in the position-sizing formula must be changed to match the volatility level of the fund. 

Time frame: Many funds trade multiple time frames but I stick to a single time frame in the replication. As some funds concentrate on the longer-term trends and others on the shorter term, I either pick the default time period, a shorter version or a longer version in order to match the results as closely as possible. 

## Campbell Composite

The Campbell Composite is not actually a fund but a composite index of accounts managed by Campbell & Company, who have been in the business since the early 1970s and done very well over the long run. The company manages a large number of individual accounts as well as funds and its official track record is a composite of all accounts it traded, net of all fees. It is therefore not the result of a single account but rather like an index of all the company’s accounts. It can be assumed that the firm does not do exactly the same for all accounts, but its business is trend-following futures and the difference between accounts is likely to be related to sector weighting and risk level more than the core strategy. Either way, it should even out when all accounts are mashed into a composite such as this one. 

With over US$2 billion under management, Campbell is one of the giants of the business. Their compounded annual returns are around 14% and they had only four losing years in the 22 years between 1990 and 2011 (see Table 7.7), not counting the flat 2008. That should be a tough player to beat. 

Table 7.7 Campbell Composite monthly returns 

<table><tr><td></td><td>Jan (%)</td><td>Feb (%)</td><td>Mar (%)</td><td>Apr (%)</td><td>May (%)</td><td>Jun (%)</td><td>Jul (%)</td><td>Aug (%)</td><td>Sep (%)</td><td>Oct (%)</td><td>Nov (%)</td><td>Dec (%)</td><td>Year (%)</td></tr><tr><td>1990</td><td>3.70</td><td>0.44</td><td>3.86</td><td>5.44</td><td>-11.69</td><td>7.08</td><td>8.58</td><td>11.33</td><td>2.19</td><td>1.64</td><td>-1.25</td><td>-0.81</td><td>32.65</td></tr><tr><td>1991</td><td>-8.05</td><td>-2.28</td><td>19.78</td><td>-1.99</td><td>2.75</td><td>2.32</td><td>-8.46</td><td>2.56</td><td>5.51</td><td>0.54</td><td>-2.12</td><td>17.07</td><td>26.56</td></tr><tr><td>1992</td><td>-5.53</td><td>-3.88</td><td>0.52</td><td>-2.71</td><td>0.80</td><td>10.72</td><td>10.23</td><td>4.93</td><td>-2.42</td><td>-3.66</td><td>5.97</td><td>-0.95</td><td>13.11</td></tr><tr><td>1993</td><td>-1.23</td><td>13.90</td><td>-5.74</td><td>2.96</td><td>2.76</td><td>2.81</td><td>5.47</td><td>-4.85</td><td>-5.06</td><td>-6.59</td><td>-0.18</td><td>-0.29</td><td>2.17</td></tr><tr><td>1994</td><td>-4.59</td><td>-6.86</td><td>6.02</td><td>-2.20</td><td>-2.80</td><td>5.92</td><td>-3.24</td><td>-4.14</td><td>6.67</td><td>0.57</td><td>-6.55</td><td>-5.03</td><td>-16.23</td></tr><tr><td>1995</td><td>-4.48</td><td>5.64</td><td>9.45</td><td>1.80</td><td>0.17</td><td>-1.07</td><td>-3.83</td><td>6.04</td><td>-3.62</td><td>1.10</td><td>-0.16</td><td>6.80</td><td>18.05</td></tr><tr><td>1996</td><td>5.74</td><td>-5.69</td><td>5.31</td><td>3.53</td><td>-1.81</td><td>1.26</td><td>-0.19</td><td>1.93</td><td>2.36</td><td>12.19</td><td>12.07</td><td>-4.27</td><td>35.50</td></tr><tr><td>1997</td><td>5.05</td><td>2.15</td><td>-2.05</td><td>-3.38</td><td>-1.91</td><td>2.38</td><td>8.97</td><td>-5.19</td><td>4.17</td><td>2.28</td><td>0.60</td><td>4.92</td><td>18.49</td></tr><tr><td>1998</td><td>3.14</td><td>-2.39</td><td>4.97</td><td>-5.89</td><td>4.25</td><td>1.93</td><td>-3.70</td><td>9.13</td><td>2.88</td><td>4.50</td><td>-0.57</td><td>0.68</td><td>19.53</td></tr><tr><td>1999</td><td>-4.83</td><td>1.52</td><td>0.84</td><td>5.51</td><td>-3.26</td><td>4.63</td><td>-0.14</td><td>1.18</td><td>1.72</td><td>-4.24</td><td>0.68</td><td>3.49</td><td>6.70</td></tr><tr><td>2000</td><td>3.63</td><td>-0.35</td><td>-2.10</td><td>-1.83</td><td>2.59</td><td>1.85</td><td>-1.87</td><td>3.03</td><td>-3.26</td><td>3.19</td><td>5.91</td><td>2.49</td><td>13.61</td></tr><tr><td>2001</td><td>-1.10</td><td>0.69</td><td>6.92</td><td>-8.05</td><td>1.21</td><td>-1.74</td><td>1.41</td><td>2.05</td><td>6.90</td><td>4.91</td><td>-9.63</td><td>3.71</td><td>5.91</td></tr><tr><td>2002</td><td>-0.71</td><td>-1.99</td><td>-1.63</td><td>-4.01</td><td>4.09</td><td>7.75</td><td>7.55</td><td>3.58</td><td>3.85</td><td>-4.71</td><td>-1.30</td><td>3.64</td><td>16.22</td></tr><tr><td>2003</td><td>7.71</td><td>7.68</td><td>-4.37</td><td>2.77</td><td>2.10</td><td>-0.77</td><td>-4.63</td><td>2.42</td><td>-1.15</td><td>2.88</td><td>0.80</td><td>4.31</td><td>20.62</td></tr><tr><td>2004</td><td>2.44</td><td>10.65</td><td>0.87</td><td>-6.66</td><td>-0.59</td><td>-3.15</td><td>-0.57</td><td>-1.13</td><td>-1.50</td><td>2.43</td><td>4.06</td><td>0.79</td><td>6.89</td></tr><tr><td>2005</td><td>-2.17</td><td>-1.10</td><td>0.11</td><td>0.51</td><td>4.99</td><td>6.22</td><td>1.04</td><td>-5.32</td><td>3.78</td><td>3.81</td><td>2.12</td><td>-2.72</td><td>11.16</td></tr><tr><td>2006</td><td>2.01</td><td>-1.55</td><td>4.21</td><td>-2.76</td><td>-2.77</td><td>-0.40</td><td>-0.08</td><td>-0.36</td><td>-2.77</td><td>1.79</td><td>0.83</td><td>7.82</td><td>5.57</td></tr><tr><td>2007</td><td>2.49</td><td>-5.57</td><td>-3.20</td><td>2.16</td><td>5.71</td><td>4.16</td><td>-10.79</td><td>-6.73</td><td>1.94</td><td>5.59</td><td>-6.13</td><td>-2.15</td><td>-13.31</td></tr><tr><td>2008</td><td>-0.38</td><td>1.55</td><td>-0.20</td><td>-2.54</td><td>2.09</td><td>5.45</td><td>-1.28</td><td>-1.45</td><td>-1.24</td><td>-0.96</td><td>-1.41</td><td>0.53</td><td>-0.09</td></tr><tr><td>2009</td><td>0.09</td><td>1.03</td><td>-2.09</td><td>-4.60</td><td>-0.63</td><td>-2.20</td><td>0.17</td><td>-1.06</td><td>3.87</td><td>-1.38</td><td>3.41</td><td>-3.60</td><td>-7.10</td></tr><tr><td>2010</td><td>-7.12</td><td>1.48</td><td>2.16</td><td>2.45</td><td>-2.93</td><td>-0.52</td><td>-1.59</td><td>5.11</td><td>4.62</td><td>4.11</td><td>-1.54</td><td>4.99</td><td>10.95</td></tr><tr><td>2011</td><td>-1.12</td><td>2.52</td><td>-6.47</td><td>6.86</td><td>-3.2</td><td>-4.03</td><td>9.13</td><td>0.41</td><td>-5.01</td><td>-4.48</td><td>-1.24</td><td>3.01</td><td>-4.80</td></tr></table>

Since the company manages a huge amount of money, it would be a fair assumption that it uses a large universe of markets to trade. As an approximation therefore, I use the Large Universe that I defined earlier in this chapter (in Table 7.2). Next, the Campbell Composite results (see Figure 7.2) show us that it is operating on a lower volatility level than our core strategy, with both lower returns and lower drawdowns. To compensate for this I use a risk factor of 9 basis points (bp) in the position-sizing algorithm. I leave the time frame at the default speed of medium-term trading. 


Figure 7.2 Replicating Campbell 1990 to 2010


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/510d39328a42f02db0ed4794b960105e74fbf943867cb0d69c09e22b4e021d79.jpg)


The result of this minor change to our core strategy when compared to the Campbell method is rather striking. In 1990 its volatility level was higher than the core strategy, which likely means that it was taking more risk and trading fewer markets than in the following decade. In relation to our strategy, this paid off for Campbell from 1990 to 1993 but it lost that advantage in 1993 to 1995. It is in the period from 1997 to 2007 that our simple comparison strategy has a very good fit and this shows that during this period Campbell’s core strategy was probably not very different from the one described in this book. Again, all simulations shown in this book take commission, slippage, management fee, admin fees and performance fees into account; otherwise it would not be a fair comparison. The month by month returns from 1997 to 2007 are close to identical, and so the probability of Campbell doing something very different and by pure coincidence happening to land on the same return numbers is not exactly overwhelming. The monthly return correlation for the whole period was 0.72 and during some years substantially higher. 

What is really interesting is what happened to Campbell in 2007 and the following years. This is when practically all trend-following strategies were having their best performances ever, but the Campbell Composite turned down. This should not be possible with a trend-following strategy and the only explanation for this is that the company started changing its formula. Campbell was probably trying out new systematic strategies, adding carry trade strategies, options or other new factors that took over the driver seat of the NAV and caused it to lose money when it should have been making huge amounts had it only stuck to the original strategy. Looking at the results from 2010 onwards, it would appear as if classic trend following is again driving Campbell’s bottom line and so I have high hopes for it making a good comeback. The missing 2008 profits will of course mean that it will remain far behind most competitors for some time in the longer-term comparisons. 

## Sunrise Capital Diversified

Sunrise Capital is another giant of the industry that has been around since the mid-1990s and has almost US$750 million under management. It is a classic trend-following futures manager with fairly low volatility compared with our core strategy and a compounded annual return of around 12% (see Table 7.8 for its monthly results). Since its inception it has outperformed pretty much any benchmark you can throw at it, despite having a risk level significantly lower than our core strategy. According to its own marketing material, it seems to have a heavier weighting towards financial futures and especially interest rates and currencies. For this reason I use the Financially Heavy Investment Universe (from the earlier Table 7.4) to try to replicate what it does. A quick visual inspection of its long-term track record does not show any signs of larger deviation from what would be expected from a medium-term trend-following strategy, and so it should be safe enough to use our core strategy with the same time frame parameters. Its volatility is slightly more than half of the core strategy though, so that will have to be compensated for in the position sizing. 

## Table 7.8 Sunrise Capital Diversified monthly results

<table><tr><td></td><td>Jan (%)</td><td>Feb (%)</td><td>Mar (%)</td><td>Apr (%)</td><td>May (%)</td><td>Jun (%)</td><td>Jul (%)</td><td>Aug (%)</td><td>Sep (%)</td><td>Oct (%)</td><td>Nov (%)</td><td>Dec (%)</td><td>Year (%)</td></tr><tr><td>1998</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-0.1</td><td>-2.3</td><td>1.0</td><td>-1.4</td></tr><tr><td>1999</td><td>-1.7</td><td>4.0</td><td>0.4</td><td>3.6</td><td>0.7</td><td>1.9</td><td>-1.0</td><td>-0.7</td><td>0.4</td><td>-4.2</td><td>4.6</td><td>-2.0</td><td>5.8</td></tr><tr><td>2000</td><td>5.2</td><td>-4.4</td><td>-1.6</td><td>-2.6</td><td>0.2</td><td>-2.8</td><td>1.7</td><td>3.9</td><td>0.1</td><td>0.0</td><td>5.6</td><td>7.1</td><td>12.3</td></tr><tr><td>2001</td><td>3.2</td><td>4.4</td><td>6.7</td><td>-6.2</td><td>1.9</td><td>-0.6</td><td>-0.2</td><td>2.7</td><td>7.4</td><td>8.4</td><td>-13.9</td><td>-1.3</td><td>10.8</td></tr><tr><td>2002</td><td>-1.2</td><td>-2.0</td><td>-1.5</td><td>1.6</td><td>4.6</td><td>10.8</td><td>3.6</td><td>0.8</td><td>5.6</td><td>-6.3</td><td>-7.5</td><td>9.8</td><td>17.9</td></tr><tr><td>2003</td><td>9.8</td><td>3.3</td><td>-6.2</td><td>0.5</td><td>5.6</td><td>-3.1</td><td>-2.8</td><td>0.5</td><td>-5.2</td><td>7.0</td><td>-2.4</td><td>7.7</td><td>14.0</td></tr><tr><td>2004</td><td>3.1</td><td>7.9</td><td>1.7</td><td>-4.4</td><td>-2.1</td><td>-2.1</td><td>-1.0</td><td>-5.2</td><td>0.8</td><td>4.0</td><td>5.4</td><td>2.1</td><td>9.8</td></tr><tr><td>2005</td><td>-6.2</td><td>-0.2</td><td>-0.3</td><td>-2.4</td><td>0.5</td><td>1.4</td><td>-1.0</td><td>-1.1</td><td>-1.4</td><td>-0.1</td><td>6.5</td><td>1.9</td><td>-2.8</td></tr><tr><td>2006</td><td>0.7</td><td>0.2</td><td>2.7</td><td>3.4</td><td>0.1</td><td>-1.6</td><td>-4.2</td><td>-0.6</td><td>0.0</td><td>3.9</td><td>1.7</td><td>2.0</td><td>8.3</td></tr><tr><td>2007</td><td>4.5</td><td>-3.4</td><td>-6.8</td><td>6.6</td><td>2.6</td><td>0.5</td><td>-6.2</td><td>-9.4</td><td>5.5</td><td>8.1</td><td>3.4</td><td>2.3</td><td>6.0</td></tr><tr><td>2008</td><td>6.4</td><td>8.7</td><td>-1.1</td><td>-3.4</td><td>3.4</td><td>2.4</td><td>-4.6</td><td>-2.9</td><td>3.1</td><td>13.8</td><td>4.2</td><td>1.8</td><td>34.9</td></tr><tr><td>2009</td><td>-1.8</td><td>-0.5</td><td>-2.1</td><td>-1.6</td><td>3.0</td><td>-0.5</td><td>3.0</td><td>2.6</td><td>0.6</td><td>-0.3</td><td>4.9</td><td>-2.1</td><td>5.1</td></tr><tr><td>2010</td><td>-4.4</td><td>-0.5</td><td>2.5</td><td>0.1</td><td>-13.1</td><td>-0.8</td><td>-3.3</td><td>2.0</td><td>3.3</td><td>6.5</td><td>-1.7</td><td>5.3</td><td>-5.5</td></tr><tr><td>2011</td><td>0.7</td><td>3.5</td><td>-1.1</td><td>4.3</td><td>-4.9</td><td>-1.9</td><td>0.2</td><td>0.8</td><td>5.6</td><td>-7.0</td><td>2.5</td><td>0.5</td><td>2.3</td></tr></table>

Using the core strategy with the Financially Heavy Investment Universe on a medium-term time frame and 11 bp risk, we arrive at a pretty good fit with a correlation of 0.73. The month by month correlation between 1997 and 2004 was extremely high and even after the divergence that started at that point the monthly correlations remain very high. There are two notable single-month divergences that can be seen in Figure 7.3, in August 2007 and May 2010 where Sunrise had individual bad months and our strategy did not. In August of 2007 there were two sector-driving losses for most futures traders, the first of which was the sharp rebound in the downwards trend of the dollar. The trend continued after the counter move, bu many trend-following strategies were knocked out of their positions after taking heavy losses. Since Sunrise is heavily geared towards this sector, it likely had many counter dollar bets going against it that month. The other factor for that month was the sudden reversal of the equity bear trend, which also triggered many stops for our colleagues out there. 


Figure 7.3 Replicating Sunrise Capital Diversified


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/3bcb64c53f128fc360f685127f143328b4c0abbbf505ee949603d4af5f26d2e8.jpg)


The situation in 2010 was similar but this time the interest-rate sector was the more likely culprit. A trend follower would have been short rates in the US and Canada, in particular in May of 2010 when the yields dropped quickly and the prices shot up. Our strategy got lucky with the timing and closed out a couple of days before larger moves in the adverse direction in the Canadian Bankers’ Acceptance, Eurodollar and Tbills. Sunrise did however manage to catch up with our strategy remarkably quickly after both events. 

## Palm Trend Fund

The Palm Trend Fund is a commodity trend following managed by Beach Horizon and it has shown a compound annual return of about 15%, maximum drawdown of around 25% with 54% positive months, 72% positive rolling 12-month periods. Having commenced managed account trading in 2005, it launched the Palm Trend Fund in 2010. The monthly return numbers presented in Table 7.9 are a combination of this fund and the pro forma adjusted track record of its managed account trading based on the same strategy, as provided by the manager. This particular fund has a clear focus on commodities and states that it has close to 60% in this sector and the rest diversified across other asset classes. That gives us a good starting point to reverse engineer its strategy and it implies that we should be using the Commodity Heavy Investment Universe (see the earlier Table 7.5). 


Table 7.9 Palm Trend Fund D monthly results


<table><tr><td></td><td>Jan(%)</td><td>Feb(%)</td><td>Mar(%)</td><td>Apr(%)</td><td>May(%)</td><td>Jun(%)</td><td>Jul(%)</td><td>Aug(%)</td><td>Sep(%)</td><td>Oct(%)</td><td>Nov(%)</td><td>Dec(%)</td><td>Year(%)</td></tr><tr><td>2005</td><td>-</td><td>-</td><td>-</td><td>-</td><td>6.42</td><td>4.44</td><td>-4.12</td><td>5.66</td><td>1.91</td><td>-4.67</td><td>14.35</td><td>0.82</td><td>26.1</td></tr><tr><td>2006</td><td>8.63</td><td>-6.08</td><td>9.28</td><td>13.45</td><td>-2.94</td><td>-5.66</td><td>-8.74</td><td>1.14</td><td>-4.81</td><td>6.14</td><td>0.87</td><td>2.76</td><td>12.0</td></tr><tr><td>2007</td><td>2.45</td><td>-4.69</td><td>-3.94</td><td>7.22</td><td>6.93</td><td>5.69</td><td>-10.50</td><td>-14.26</td><td>11.55</td><td>14.13</td><td>-3.86</td><td>8.41</td><td>15.7</td></tr><tr><td>2008</td><td>13.56</td><td>28.41</td><td>-3.78</td><td>-5.98</td><td>3.49</td><td>8.55</td><td>-16.74</td><td>-6.36</td><td>9.99</td><td>25.51</td><td>8.80</td><td>6.56</td><td>84.9</td></tr><tr><td>2009</td><td>0.82</td><td>0.99</td><td>-5.63</td><td>-4.52</td><td>-2.27</td><td>-3.92</td><td>-1.97</td><td>5.34</td><td>2.74</td><td>-6.71</td><td>11.17</td><td>-3.50</td><td>-8.5</td></tr><tr><td>2010</td><td>-6.40</td><td>-0.34</td><td>7.29</td><td>3.66</td><td>-13.28</td><td>-0.85</td><td>-7.79</td><td>6.04</td><td>3.24</td><td>11.75</td><td>-6.37</td><td>17.02</td><td>10.3</td></tr></table>

Overlaying our core strategy with the Commodity Heavy Investment Universe and 25 bp risk, the similarities are quite striking and the correlation is a whopping 0.86. Starting from 2005 we see a close tracking month by month and years later the two strategies still show almost exactly the same values (see Figure 7.4). There is not much to say about discrepancies between the strategies because they are more or less the same. Whatever strategy and investment universe the guys and gals over at Beach Horizon may be using it would appear probable that its secret formula is quite close to what we are doing in this book. 


Figure 7.4 Replicating Palm Trend Fund


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/499551ab0849f8122492fe56f8938539abb160af66a8ebe9d44395dd5085e436.jpg)


## Transtrend Standard Risk Program

Based in the relatively small port town of Rotterdam, Holland, this company has shown very consistent results in its trend-following strategy for the past two decades. The company was founded in 1991 as a traditional CTA-style trend-following futures manager mainly focusing on individual managed accounts. The company’s official track record on its Diversified Trend Program goes back to 1992 (see the monthly results in Table 7.10) and it offers various enhanced (that is, increased) risk versions as well. Transtrend prides itself on being extremely diversified and trading more markets than the competition, and it trades outright markets as well as the trends in spreads between related markets in order to increase the diversification effects. Being a very large house with assets in the order of US$10 billion, it would, of course, need to be extremely diversified in order to be able to move its massive orders in the market. 


Table 7.10 Transtrend Standard Risk monthly results


<table><tr><td></td><td>Jan (%)</td><td>Feb (%)</td><td>Mar (%)</td><td>Apr (%)</td><td>May (%)</td><td>Jun (%)</td><td>Jul (%)</td><td>Aug (%)</td><td>Sep (%)</td><td>Oct (%)</td><td>Nov (%)</td><td>Dec (%)</td><td>Year (%)</td></tr><tr><td>1992</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>3.15</td><td>4.26</td><td>0.95</td><td>-1.17</td><td>-1.62</td><td>1.71</td><td>-0.85</td><td>6.44</td></tr><tr><td>1993</td><td>-5.24</td><td>5.35</td><td>-0.48</td><td>4.25</td><td>-1.79</td><td>1.59</td><td>4.79</td><td>-2.91</td><td>-0.19</td><td>-0.39</td><td>0.97</td><td>4.92</td><td>10.71</td></tr><tr><td>1994</td><td>1.12</td><td>1.17</td><td>6.35</td><td>-0.05</td><td>1.57</td><td>0.92</td><td>-2.64</td><td>-3.72</td><td>1.37</td><td>-1.29</td><td>6.02</td><td>-0.49</td><td>10.28</td></tr><tr><td>1995</td><td>-3.83</td><td>6.16</td><td>7.52</td><td>-0.22</td><td>4.21</td><td>2.63</td><td>-1.18</td><td>-0.41</td><td>0.54</td><td>-1.26</td><td>1.73</td><td>3.95</td><td>21.01</td></tr><tr><td>1996</td><td>2.53</td><td>-3.80</td><td>0.08</td><td>5.48</td><td>-1.88</td><td>-0.09</td><td>2.03</td><td>4.27</td><td>4.30</td><td>4.71</td><td>0.72</td><td>-1.93</td><td>17.13</td></tr><tr><td>1997</td><td>4.99</td><td>3.73</td><td>-1.16</td><td>-2.24</td><td>-0.31</td><td>0.65</td><td>9.78</td><td>-0.15</td><td>1.28</td><td>-5.83</td><td>3.88</td><td>5.61</td><td>21.11</td></tr><tr><td>1998</td><td>1.14</td><td>0.10</td><td>2.16</td><td>-3.39</td><td>2.42</td><td>0.62</td><td>-2.21</td><td>12.73</td><td>1.87</td><td>-0.15</td><td>-0.38</td><td>1.19</td><td>16.38</td></tr><tr><td>1999</td><td>-2.32</td><td>0.99</td><td>-1.56</td><td>2.03</td><td>-1.79</td><td>3.10</td><td>1.06</td><td>-1.67</td><td>0.48</td><td>-4.86</td><td>1.61</td><td>2.83</td><td>-0.42</td></tr><tr><td>2000</td><td>1.17</td><td>-1.18</td><td>-1.64</td><td>-0.06</td><td>1.85</td><td>-1.63</td><td>-0.31</td><td>1.42</td><td>0.72</td><td>1.98</td><td>3.52</td><td>2.90</td><td>8.93</td></tr><tr><td>2001</td><td>0.19</td><td>0.89</td><td>4.25</td><td>-1.13</td><td>0.91</td><td>-0.49</td><td>3.23</td><td>1.67</td><td>5.09</td><td>0.72</td><td>-1.84</td><td>3.11</td><td>17.63</td></tr><tr><td>2002</td><td>-0.81</td><td>-0.59</td><td>1.01</td><td>-0.91</td><td>1.18</td><td>4.91</td><td>3.82</td><td>2.09</td><td>2.16</td><td>-1.71</td><td>-1.02</td><td>4.44</td><td>15.23</td></tr><tr><td>2003</td><td>3.23</td><td>2.66</td><td>-3.37</td><td>2.53</td><td>3.75</td><td>-1.62</td><td>-1.73</td><td>-0.18</td><td>-1.32</td><td>1.59</td><td>-0.47</td><td>-0.13</td><td>4.75</td></tr><tr><td>2004</td><td>1.53</td><td>3.44</td><td>-1.11</td><td>-2.16</td><td>-0.16</td><td>-1.51</td><td>-0.92</td><td>-0.35</td><td>0.99</td><td>1.86</td><td>5.67</td><td>1.12</td><td>8.43</td></tr><tr><td>2005</td><td>-3.07</td><td>1.73</td><td>1.50</td><td>-2.18</td><td>0.95</td><td>2.62</td><td>1.86</td><td>-0.24</td><td>1.09</td><td>-0.15</td><td>2.36</td><td>-1.80</td><td>4.57</td></tr><tr><td>2006</td><td>1.08</td><td>-1.65</td><td>0.79</td><td>1.33</td><td>-1.94</td><td>-0.71</td><td>-2.40</td><td>3.35</td><td>0.41</td><td>3.08</td><td>2.40</td><td>3.52</td><td>9.41</td></tr><tr><td>2007</td><td>1.02</td><td>-2.61</td><td>-1.95</td><td>3.80</td><td>4.21</td><td>2.48</td><td>-1.59</td><td>-1.59</td><td>4.91</td><td>5.82</td><td>-1.40</td><td>0.97</td><td>14.46</td></tr><tr><td>2008</td><td>-0.32</td><td>3.97</td><td>0.74</td><td>0.43</td><td>2.14</td><td>2.00</td><td>-1.97</td><td>-0.92</td><td>3.65</td><td>4.93</td><td>1.67</td><td>1.41</td><td>18.98</td></tr><tr><td>2009</td><td>-0.24</td><td>0.40</td><td>-2.39</td><td>-0.11</td><td>0.85</td><td>-0.73</td><td>-1.71</td><td>0.36</td><td>-0.68</td><td>-2.51</td><td>1.38</td><td>-3.21</td><td>-8.36</td></tr><tr><td>2010</td><td>-2.63</td><td>0.73</td><td>5.50</td><td>0.95</td><td>-2.97</td><td>-0.18</td><td>-0.75</td><td>1.82</td><td>2.07</td><td>2.72</td><td>-0.66</td><td>2.21</td><td>8.84</td></tr></table>

Using our core strategy with the default time frame and expanding the investment universe to the Large Universe (see the earlier Table 7.2), we get a pretty good fit for this futures manager. The volatility level of its Standard Risk Program is less than half our default setting but using 8 bp in the position sizing does the trick and we arrive at the results in Figure 7.5, where already we have quite an okay fit. Interestingly, Transtrend seems to have slightly higher volatility than our 8 bp model in the first half of the chart while their volatility level is lower than the model’s in the next final decade. It is quite common to see that large managers that have been operating for a long time tend to decrease their volatility levels, and with them the returns of course. When the assets under management grow into the billions it becomes very difficult to continue getting the same level of returns out and the success of this manager may have ended up hampering its result. 

Figure 7.5 Replicating Transtrend Standard Risk 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/608ff56cadbfdfd80eb3b85ed530f1d72b9531b9e6e4eec2892bc4b12ae2b49f.jpg)


Compare Figure 7.6 where the core strategy is exactly the same except that a different risk level has been used up to the year 2000 than for the years following it. From 1992 to 1999 I use a risk level of 9 bp and after that reduce it to just 6 bp. The trading rules and everything else are, of course, kept constant. It is likely that the actual risk reduction in the Transtrend trading strategy was gradual and not cut at a single point in time as this simplified example shows, but we still get a very close fit using this approximation. The conclusion is that the company is using quite standard trending models, just like most other futures managers do. 


Figure 7.6 Transtrend Replication with Risk Reduction from 2000


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/fe6d51ef64e094a1d55668f429b8b972dc18e0a56ba7a59b167b977360663511.jpg)



Mulvaney Capital Management Global Markets Fund


This UK-based investment manager takes a significantly longer-term view on trend following than most of its peers. This longer-term time horizon means that it needs much wider stop loss distances than our default strategy and so it could have sharper drawdowns in bad periods. On the other hand, it also means that it does not get knocked out of trends as quickly and it is more likely to stay in during a trend correction. This approach often yields higher overall returns at the expense of larger losses when the trends actually turn around. The time horizon is its main differentiator against other funds. Founded by a former Merrill Lynch options trader in 1999, the fund has shown very strong results with only three real negative years and it more than doubled its investors’ money in 2008. It has around US$200 million under management and so it is still small enough to be able to trade most markets. 

The months from August 2001 to February 2002 lack a track record because the fund was temporarily closed during a migration to a different structure (see Table 7.11). In accordance, the replication simulation uses a zero return for these months as well. 


Table 7.11 Mulvaney Global Markets Fund monthly returns


<table><tr><td></td><td>Jan (%)</td><td>Feb (%)</td><td>Mar (%)</td><td>Apr (%)</td><td>May (%)</td><td>Jun (%)</td><td>Jul (%)</td><td>Aug (%)</td><td>Sep (%)</td><td>Oct (%)</td><td>Nov (%)</td><td>Dec (%)</td><td>Year (%)</td></tr><tr><td>1999</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-0.3</td><td>-0.1</td><td>-2.2</td><td>2.1</td><td>-4.8</td><td>-4.8</td><td>7.0</td><td>4.8</td><td>1.1</td></tr><tr><td>2000</td><td>-5.0</td><td>2.5</td><td>-8.4</td><td>-0.3</td><td>7.0</td><td>1.6</td><td>-1.3</td><td>12.7</td><td>-4.4</td><td>2.0</td><td>9.1</td><td>8.9</td><td>24.5</td></tr><tr><td>2001</td><td>-9.6</td><td>18.8</td><td>13.5</td><td>-15.3</td><td>-0.7</td><td>5.4</td><td>-1.3</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>6.7</td></tr><tr><td>2002</td><td>-</td><td>-</td><td>-7.5</td><td>1.6</td><td>6.8</td><td>7.4</td><td>6.0</td><td>5.4</td><td>5.1</td><td>-7.7</td><td>-5.1</td><td>7.8</td><td>19.4</td></tr><tr><td>2003</td><td>13.2</td><td>7.2</td><td>-12.8</td><td>1.5</td><td>7.6</td><td>-7.6</td><td>-6.3</td><td>0.1</td><td>6.7</td><td>15.3</td><td>-0.3</td><td>5.4</td><td>29.3</td></tr><tr><td>2004</td><td>4.2</td><td>8.5</td><td>2.4</td><td>-11.5</td><td>-7.0</td><td>-0.7</td><td>-0.4</td><td>-6.2</td><td>7.8</td><td>0.8</td><td>9.6</td><td>-4.9</td><td>-0.1</td></tr><tr><td>2005</td><td>-4.3</td><td>0.5</td><td>2.3</td><td>-9.3</td><td>-4.1</td><td>5.3</td><td>6.6</td><td>2.8</td><td>13.6</td><td>-5.6</td><td>15.3</td><td>8.4</td><td>32.3</td></tr><tr><td>2006</td><td>11.1</td><td>-2.7</td><td>13.1</td><td>11.5</td><td>-4.3</td><td>-6.1</td><td>-5.2</td><td>2.0</td><td>1.0</td><td>-0.1</td><td>0.6</td><td>1.6</td><td>21.9</td></tr><tr><td>2007</td><td>0.6</td><td>-5.2</td><td>-8.8</td><td>2.6</td><td>4.7</td><td>4.9</td><td>-16.9</td><td>-19.4</td><td>3.9</td><td>13.7</td><td>-8.6</td><td>8.5</td><td>-23.1</td></tr><tr><td>2008</td><td>21.7</td><td>28.9</td><td>-8.0</td><td>-8.6</td><td>5.4</td><td>8.5</td><td>-18.8</td><td>-6.7</td><td>11.6</td><td>45.5</td><td>7.0</td><td>5.3</td><td>108.9</td></tr><tr><td>2009</td><td>1.6</td><td>0.0</td><td>-3.4</td><td>-5.5</td><td>-1.3</td><td>-6.8</td><td>-0.5</td><td>10.9</td><td>1.3</td><td>-7.9</td><td>10.7</td><td>-3.2</td><td>-5.9</td></tr><tr><td>2010</td><td>-3.8</td><td>-7.2</td><td>-5.2</td><td>2.0</td><td>-8.8</td><td>0.5</td><td>-12.0</td><td>14.6</td><td>16.5</td><td>22.3</td><td>-5.4</td><td>25.3</td><td>34.9</td></tr><tr><td>2011</td><td>2.1</td><td>9.8</td><td>-4.6</td><td>6.1</td><td>-11.8</td><td>-7.4</td><td>11.2</td><td>1.6</td><td>-4.2</td><td>-14.1</td><td>12.1</td><td>-1.6</td><td>-5.3</td></tr></table>

The Large Universe fits reasonably well to the Mulvaney profile, but the Commodity Heavy Universe (see the earlier Table 7.5) shows even higher correlations so that’s the one used here. One reason why the Commodity Heavy version works well could be that the company is small enough to be able to allocate more to this sector, something that becomes increasingly difficult north of US$500 million under management. To mimic its longer-term profile I widen the stops from the default of 3 to 6 risk units, as defined in Chapter 3.In order to match its chosen volatility structure, I also had to lower the risk factor in the position-sizing formula from 20 to 15 bp. With these small changes to the core strategy, we end up with a correlation of 0.86 against the Mulvaney Global Markets Fund and there is only really one period where our results differ. During late 2005 it had quite a large outperformance against our strategy, which it ended up losing quite quickly in 2007 (as Figure 7.7 shows). 

Figure 7.7 Replicating Mulvaney Global Markets Fund 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/a9dca83d9d476a65911d34e33e1c9a9fb13ed1ef637d2a56f58b71f48e68776a.jpg)



More funds



Still not convinced that the big boys of the business are using essentially the same model as our core strategy? Fine, let’s replicate some more of them. In Figures 7.8 to 7.11 you find replication charts of Abraham, Eckhardt, Conquest, and ISAM along with the specifications used for the model strategy.



Figure 7.8 Replicating Abraham Trading Company Diversified Program


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/9c0503f79d3c846899e58dc6abe718d555afadf1c0827b6b6aec83c97d2ad838.jpg)



Figure 7.9 Replicating Eckhardt Trading Company Standard Plus


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/d9f257a4d33594979801e9b17b227c449b64297fb6bcd96b3ee5ec552af42a50.jpg)



Figure 7.10 Replicating Conquest Managed Futures Select


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/95fdb0c4fa3279f60117f8288c612d2aac2f64d94c8dc9c06511298649718426.jpg)



Figure 7.11 Replicating ISAM Systematic Fund Classic A


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/c0667820451a7ad6e6e8bbba72e37787c59cc618ca17c85df581a94a53a5c268.jpg)


## CONCLUSIONS

Not all futures funds are easy to replicate with simple models but with a little work you should be able to figure out the core strategies of the majority of CTA funds. This does not mean that there is something wrong with the funds or that you should necessarily favour funds that you cannot manage to reverse engineer. At the end of the day, a nice positive return is still a nice positive return and the funds discussed in this chapter have provided very attractive returns for their investors over the long run. What this method of reverse engineering can do for you is to show what each fund does and how the funds differ from each other. You could also use it as a benchmark, ranking funds on a volatility equalised basis to see which ones add value. Most importantly of course if you want to get into the business of managing futures, you can use this information to develop and improve your strategies and to benchmark your own results. 

The fact that it is relatively easy to build a systematic strategy that can replicate large funds does not in any way mean that it is as easy to accomplish in reality. It can be done with plenty of hard work, however, and that is what the investors are paying the funds for. If you do your own homework and put some hard work into it, perhaps investors will be paying you to do it as well. 

8 

## Tweaks and Improvements

In this chapter I provide some ideas on the type of improvements that may prove beneficial to our core strategy. There are several possible objectives when it comes to tweaking a strategy such as this one, and whilst not necessarily the most important, increased profitability is only one. If increasing the annual compounded return is the only objective, all you need to do is increase the leverage to just slightly shy of risking a complete blow-up. This is, of course, just stretching the theoretical arguments and not how reality looks. It is important to be able to achieve a high enough annualised return for the strategy to be of interest to investors and worth the time and effort involved in achieving it, but in reality it is much more important, and difficult, to reduce volatility and correlations to similar products. 

If you can reduce your drawdowns, lower the volatility levels and achieve a slightly different return profile from the average CTA product, you will find your product much easier to sell. Most of these subjects would require a book all by themselves to analyse properly and my intention in this chapter is only to point you in the right direction for further research on these topics. After all, in order to really trust and trade strategies with a potential 1,000 to 1 leverage, you need to do some serious research either way. 

## TRADING MULTIPLE TIME FRAMES

One of the most common and also one of the easier ways to increase the volatility adjusted returns is to trade the same strategy on multiple time frames. To change the core strategy to trade shorter- or longerterm trends with a minimum of modification you could adjust the trend filter settings, the breakout period and/or the stop distance. If you double the distance to the tops, the strategy will stay in trades longer and quite often will benefit from keeping a position during times when others get whipsawed in and out of it. On the downside of course when the trend actually turns, the hit comes much harder. By halving the distance to the stops you get out much faster when the trend turns and take your profits home much faster, but you also risk increased whipsawing during trendless periods. Either approach is fine as long as you are fully aware of the consequences. Generally speaking, the longer-term strategies can be more profitable in terms of compound annual return but they tend to suffer from worse skews, which could mean some nasty surprises in extreme markets, as well as higher correlations to traditional investments. 

To demonstrate how a combination of different time horizons can provide benefits, I use three simulated strategies all based on the same core strategy as before, and all using the large investment universe from Chapter 7. The first one keeps the standard 3 unit stop distance as the original core strategy while the second uses 1.5 units and the final iteration 6 units. Although the longer-term strategies are clearly more volatile than the shorter, and also more profitable, I keep this example simple by assigning them equal weights in our portfolio. They all get to trade on 0.06% risk. 

In a long-term chart such as Figure 8.1 the result of combining multiple time frames may seem negligible but this is not the case. You need to dig down deeper into the details to see the pleasant improvements. While the original strategy showed an annual yield of 25.9% with a maximum drawdown of 29.2%, the mix of the three strategies shows about the same return of 25.7% but a maximum drawdown of only 26.9%. If you prefer to keep the drawdown level constant and raise your returns, you could let the three strategies run at 0.066% risk each and end up with annualised returns of 28.5% with a maximum drawdown of 29.5%. 

Figure 8.1 Mixing time frames 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/ce6ab16a5aaaca949dfffe800d1635d30a1bcb04fc7581057957d79ad0c28e13.jpg)


The three strategies obviously have very high correlations to each other because they are based on the same principles of trading, but even with the fairly small differences they yield over time it is enough to provide a slight diversification effect and get some more profit out per volatility unit. If you have a sufficient capital base, it can provide some much needed smoothing effects. The downside is that if your capital base is low, especially if you are below US$1 million, you may find yourself already struggling to achieve sufficient diversification without taking on too much risk because some contracts are rather large. 

## TRADING SYNTHETIC CONTRACTS

Do you sometimes get the feeling that trading all asset classes on all the world’s exchanges is not enough diversification? This can at times be very true and if you are looking for ways to achieve uncorrelated returns and separate yourself from the pack of trend followers, you may need to look beyond just trading single markets. One way to do this is to construct synthetic contracts, or spreads if you prefer, and treat them just like they were a normal futures market. The idea is that you take two or more contracts that are in some way related, make a new time series showing the difference between the prices of the two markets, and then apply standard trend-following strategies on this. When you trade it, you will always have a long leg and a short leg of the trade, theoretically cancelling out the commonalities of the markets involved and trading only the differences. 

A simple example is the classic gold against silver trade. At times silver may show stronger relative performance than gold during prolonged periods, whereas the opposite may be true at other times. By treating the difference in the two prices as a time series all by itself, measuring trends and breakouts as we do for all other markets, you can trade this practically the same way by going long one of them and short the other. There are a couple of differences, however, that are important to remember. First, if you start off with two equally balanced legs of the trade and successfully hold onto it for some time you may find yourself with a very mismatched position. As the long leg increases in price, that position grows larger. If the short position decreases, it grows smaller. You need to keep an eye on this and make sure your position remains roughly balanced. A second concern is that the volatility of spreads such as this is usually much lower than that of the individual contracts. As gold and silver commonly move up and down on the same days but in different degrees, you need to take on much larger notional positions in each asset to get sufficient profit potential. This means a potentially greater risk, but it can also mean much higher margin requirements, depending on how your broker views this kind of trade and how it calculates the combined margins of these trades. Some brokers simply add the margins up, which would make these spreads practically impossible to fund. 

Besides gold to silver, there are many popular spreads to use for this purpose, not least in the energy space. The crack spread as an example refers to the theoretical profit margin of an oil refinery, that is, the difference between the crude oil price and the petroleum products that are extracted from it. A common way to trade this is to have the crude on one leg and gasoline and heating oil on the other, usually in a ratio of 3:2:1. You can essentially make up any sort of spread combination you like, but do ensure that the contracts have a real-world connection and reason why they move in similar ways. If you pick contracts that just happened to have similar return profiles for a while but could potentially decouple, you may end up taking a larger risk than you bargained for. 

## ADDING A COUNTER-TREND COMPONENT

A common and often very effective method of smoothing returns of a trend-following futures strategy is simply to add a counter-trend strategy to it. Does that sound like a big contradiction in terms? It may seem odd, but this is something that works very well for some of the best trend-following futures managers. The big money is in following the trends and that is where the main action should always be, but by adding a taste of a shorter-term counter strategy you may achieve equal or even higher returns with lower volatility. A counter trend strategy has a very different personality to our core strategy. This type of strategy is usually based on taking the opposite side once a market has made an extreme move in either direction, keeping the stops very tight and taking profits early. Think of the counter strategy as more of a hit-and-run tactic in which you are fighting against the stream, and so once you have a profit you need to take it off the table and wait for the next opportunity. 

Generally speaking, most counter-trend strategies have a higher hit ratio than their trend-following counterparts. That means that you win on a higher percentage of the trades you make, but on the other hand your gains are smaller in relation to your losses than for the trend followers. You rarely see countertrend strategies that stay long with a position. They tend to hit their stops fast and get out or move to their profit targets and get out quite soon after entry. The desired properties of such a strategy in this context are positive expected returns in combinations with low or negative correlation to the trending strategy. If you can achieve that, you can use it to smooth out the return profile of your core strategy without compromising the potential yield. 

Some futures managers run up to 50/50 of counter-trend versus trending strategies in their funds or managed accounts while most let the trend-following part dominate and only add enough counter-trend trading to give a bit of a relief in the periods when trend following suffers. 

Of the profitable counter-trend strategies I have developed, most fall into one of two categories. There are the ones that go against the overall dominating trend of the markets, essentially trading directly against the trend-following strategy during extreme periods and thereby essentially work as risk-reduction mechanisms, and there are the ones that trade in the direction of the dominating trend, but waiting for outsized moves against that trend before entering. Both these methods have their own merits and they are both good complements to the core strategy. 

The first category inevitably lowers the potential returns of a trend-following strategy because it takes off risk in extreme runs in the trending direction. When the huge trends come around – think autumn 2008 – a counter-trend strategy of this type reduces the risk on the trending strategy during the most profitable times. On the other hand, during normal or sideways markets, you may find that it gives you smoother returns and higher probabilities of making positive numbers. 

The other category usually enters a position after the core trend strategy has taken its stop and exited, but before the overall trend filter signals a shift in the major trend. For instance, if there is a strong bull market in equities going on but a correction phase kicked your position out of the market, this type of counter 

strategy would be designed to attempt a re-entry of that same position at much lower prices, holding it for just a brief period of time and exiting before the core trend strategy would re-enter. 

Of the available toolkit for improving a trend-following strategy, adding a counter-trend component is in my view the most effective. 

The reason I don’t discuss scaling in and out of positions using multiple entries and exits for the core strategy is simply that I prefer to view that as a separate, albeit related strategy. It’s a matter of semantics really. Instead of having a rule to reduce positions in extreme situations, to take one example, I prefer to view it as a separate strategy taking an opposing trade in such situations. 

## INTRADAY STOPS

The core strategy used in this book only trades the day after a signal comes in, and so regardless of what happens on any given day, no action is taken until the following day. This can at times be very frustrating, in particular when there is a large adverse move in an asset and your rules don’t allow you to close your position. It is tempting to experiment with hard stops in the market and if done right it may help results as well. Just be aware that it typically also leads you to get kicked out of good positions more often because the price dips below your hard stop and comes back up again. 

The heating oil trade in 2011 is a good example of the kind of situation that can create a great deal of frustration in the short run. On 4 May the price closed very near our stop loss point, in fact only a few cents away (as Figure 8.2 shows). 5 May was a very bad day for this asset, because the exchange raised the margin requirements unexpectedly and the price fell hard throughout the day. With the default end-of-day data rules, we would need to wait until 6 May before closing down this position and by that time the damage done is three times the theoretical maximum loss from the peak. In this particular example a hard stop in the market would have been useful, but bear in mind that on a very large number of occasions the prices dip below the theoretical stop point intraday, only to continue in the trending direction soon after. Note that with a hard stop rule in this case, we would have already been out of the position in mid-April. 


Figure 8.2 Heating oil dropping far below stop


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/09e69c27ba4aa840c559a8f22579441d0cb73d0ae2b7477f17fcc91d4afed3ae.jpg)



There are two main ways to implement hard stops. The first one is to take away the previous rule about trading the following day after a certain price correction and replace it with a firm intraday stop. If you go


with this approach, you may want to move the stop a little further away than with the end-of-day stop or you risk getting too many false exits. Figure 8.3 and Table 8.1 show a quick comparison between the original approach and hard stops, at the same 3 units distance as the core strategy uses and another version that moves the stop to 4 units. The default equal-weighted investment universe has been used for all three simulations. 


Figure 8.3 Using intraday hard stops


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/4b043375dc9cf2e8d2025b83b9797620f5f8e05386be7738431f9298a99652b4.jpg)



Table 8.1 Comparing intraday stop methods


<table><tr><td>All data from Jan 1990 to Dec 2011</td><td>Core strategy</td><td>Core strategy, hard stops at 3 units</td><td>Core strategy, hard stops at 4 units</td></tr><tr><td>Compounded annual return</td><td>17.9%</td><td>12.5%</td><td>19.6%</td></tr><tr><td>Worst drawdown</td><td>-20.2%</td><td>-20.9%</td><td>-21.1%</td></tr><tr><td>Drawdown/annualised return</td><td>-1.13</td><td>-1.68</td><td>-1.07</td></tr><tr><td>Percentage profitable months</td><td>63%</td><td>62%</td><td>63%</td></tr><tr><td>Best month</td><td>41.3%</td><td>26.3%</td><td>37.3%</td></tr><tr><td>Worst month</td><td>-14.7%</td><td>-13.2%</td><td>-18.0%</td></tr><tr><td>Sharpe, RF: 2.5%</td><td>0.74</td><td>0.6</td><td>0.79</td></tr><tr><td>Sortino ratio</td><td>1.57</td><td>1.12</td><td>1.68</td></tr></table>

The default stop distance of 3 units clearly seems too tight for firm stops and that should not be very surprising. Using a little wider stop, however, shows potential. It is not easy from this data alone to say that having intraday stops is better than daily stops and be sure to look at all the details. Note the –18% as the worst month for the last simulation. That occurred in the notoriously bad month of October 2011, and so it’s a very recent event. Incidentally, the other two variations also had their worst month at the same time. This was a fairly unusual month, but there is nothing to say this cannot happen a few more times in the near future. Normally the intraday stop method seems to win over time, but a few hits like that particular month and the score can quickly change. 

The second method of implementing intraday stops is to use them as a failsafe only. That means that you keep the original rule of taking stops based on yesterday’s closing price, but add a firm intraday stop as well. The intraday stop should then be a bit further away and act only in case of a larger adverse move. This would be a protection mechanism to prevent outsized short-term losses. 

## CORRELATION MATRICES, POSITION SIZING AND RISK

If you are serious about the field of managed futures and trend following, this is an area in which you may need to do some hard work. After you have replicated and fully understood all other aspects of diversified trend following, this is likely to be the area where you need to spend the most time to perfect your strategy design. 

If anyone asked me what the single biggest flaw is in the core strategy we have used up to this point, my answer would be that the strategy treats every position completely independently and does not take into account how related they are to each other. The position sizing and risk management is therefore done on a position level and not on a portfolio level. There are two main reasons why I have let this flaw remain in the core strategy. First, it works quite well without it, showing strong results at acceptable volatility and drawdowns. Second, the topic is complex enough to warrant another few hundred pages to treat properly. 

Consider a situation where there has been one overwhelming theme dominating the real-world developments for some time. Perhaps there is a serious bear market in equities, primarily driven by negative European Union developments as in 2011/2012. This may have caused most bond futures to trend up for a prolonged period of time while the dollar gained strength and commodities moved down. So we have a fully invested portfolio with long bonds, short equities, short currencies against dollar and short commodities. The question then is: do we have many different trades or one single bet on the same theme? It may be fine that we just have a concentrated bet, because that is how the strategy is designed and what happens in some markets, but the risk level will be very high and the more these positions go in our favour, the larger the difference will be in the risk level intended by our position-sizing formula and the actual risk level. With such a portfolio, we need to be very aware that if the underlying economic and political situations suddenly change, all our positions are likely to move violently against us at the same time. Whether it is still a profitable trade or not depends on how much profit we managed to build up before the inevitable reversal. 

Two things about our existing positions change when they are held for a longer period of time, which will affect their potential impact on the portfolio. Long positions going in our favour will by definition grow larger while short positions moving down will shrink in size. Furthermore, the volatility level that each market had at the time of position entry, on which the sizing was based, will change over time. This is not taken into account at all at the moment and neither is the fact that many of our positions may in some market conditions show practically identical daily moves. 

Using the ATR method for judging volatility and as proxy for risk is a decent estimator but a highly simplified concept compared to what most futures managers would do in reality. Most of us would use Value at Risk (VaR) or similar concepts instead and some stick to the good old margin-to-equity ratio. 

You can use VaR for risk reporting, risk management and risk control and once you have large enough assets under management it makes sense to implement such a system. VaR methodology takes into account how each position is related to each other, that is, their covariance against each other. This has the added benefit of being able to run pre-trade simulations such as calculating the incremental VaR on your portfolio, should you take on a new position. The possibilities this opens in terms of risk control on a portfolio level are quite vast and potentially very valuable if you are looking for risk reduction and return smoothing. 

If you don’t have the possibility of implementing a full VaR system, you should at least be aware of the relationship between the markets you trade and look for methods to use this information in your risk management. The first thing you should do is to build a correlation matrix of the instruments you are looking to trade, or a covariance matrix if you so prefer. Make the table dynamic so that you are able to analyse the relationship between the markets over many different time periods. What you are likely to find is that at times the overall covariance between most markets in diverse asset classes goes up dramatically. These periods are often very profitable but also highly risky. 

When you build a correlation matrix there are a few things to keep in mind. First and foremost, you want to use the log returns as your basis of calculation and never the actual prices to get data. This is not at all difficult but very necessary if you don’t want to end up with nonsense data. The basic formula to get the log returns for one period is simply ln(Pt/Pt–1). However, when you are dealing with daily correlation data for global futures you have another problem to take into account and that is the different closing times of the different markets. Using one-day returns may be counterproductive if you are trading futures across the globe. If the S&P makes a big move in the afternoon in New York the Nikkei is likely to make a big move the next day and you end up with a date mismatch. The most common solution to this problem is to use a return over several days instead of just one. For instance, if you use a rolling 10-day return, ln(Pt/Pt–10), as your basis of calculations you have smoothed this issue out and made it but a rounding error. 

There are many ways to implement a risk-management strategy for a futures strategy by taking these relationships into account and this is an area where you may want to spend some time thinking things through before going live. 

## THE ROLLOVER EFFECT

The rollover effect is an interesting phenomenon that can work in your favour or to your disadvantage. If you are not aware of it and have no plan for it, the impact will be rather random and you will just be drifting in the wind hoping it all works out. This is an effect that has the biggest impact on commodities and the gist of it is that the front contract, or rather the most liquid one, has a tendency of coming under unwarranted negative pressure during the last few days of its effective life. 

There are many huge long-only commodity funds, which are essentially the commodity world equivalent of mutual funds. These funds, often managing massive amounts of money, simply buy baskets of predefined percentages of all kinds of commodities and hold them for the long run. The exact weights are usually dependent on some commodity index, just as a normal mutual fund invests according to an equity index. The big difference is that while an equity mutual fund buys stocks, the commodity fund does not buy the physical commodities. If it did, it would have to get massive warehouses, silos, vaults and so on, and operate a vast transport and storage business with all that that would entail. Instead they just buy the most liquid futures contract for each commodity and sit on it until another contract becomes more liquid, at which point they roll to the next one. These funds commonly stay long in all commodities at all times with the same percentage weights. The performance of most such funds is quite bad and if you compare their results with the spot commodity prices they seem to have rather severe underperformance. The reason for this is that most commodities are normally in a state of contango, and so these funds buy high up on the right-hand side of the yield curve and sell lower down on the left side, always having the term structure working against them. 

Since we have these huge behemoth funds that always have large speculative long positions, we know that they have a very limited time period during which they need to roll their positions. As the volume spikes up near the end of a contract’s life, these funds need to sell their positions and buy new positions further out on the curve. This creates an artificial, and measurable, negative effect on the front contract price in relation to the other points on the curve. Note that this does not mean that the price necessarily falls in the last few days, only that the relative price moves of the front contract to those of the other months tend to be slightly worse. 

One approach to this phenomenon is simply to stay out of their way by making sure you roll your long commodity positions a little earlier. By predicting when the big boys start rolling their positions, you can start your rolling a few days before and avoid risking a negative impact by their actions. The other approach is to attempt to profit directly from their predicament by trading calendar spreads. The latter option is certainly more tricky, but with some proper planning and analysis it can be done by putting on calendar spreads in the final week, but that is quite a large topic all by itself. 

## OPTIMISATION AND ITS DISCONTENTS

Modern software can easily run through a few tens of thousands of iterations of our core strategy and tell us exactly which parameters would have been the best in the past few decades. It may be tempting to let your workstation go nuts and run through every possible permutation of the strategy to make sure you get the very best possible parameters. Unfortunately, this is another one of those potentially very expensive illusions. 

Don’t lose track of what we are really doing here. We are trading a concept, a general idea. What we need to know is whether that concept would have worked reasonably well in the past and then we need to make up our minds whether we believe that this same concept is likely to work well in the future. We need to stay objective in the evaluation process and look into all the details on what went well and what did not in the past simulated results. The optimisation process does just the opposite. It hides the potential problems and lulls you into a false sense of safety. 

Perhaps your optimisation process tells you that you should run the core strategy with a 57-day breakout period, a stop of 4.17 on the long side and 2.78 on the short side. I did not bother to run this optimisation, and so those numbers are completely made up. Whatever they end up being, consider the reasons for showing the best results. If you look into the details you are likely to find that this set of numbers worked best because they managed to avoid a few really bad losses by a hairline. They had their stops just that one day before a big loss or they did not enter just before that major correction that hit the other iterations. 

If you want to push optimisation even further, why not let it use different parameters for different years? You may come to the conclusion that if you put stops very tight every second year that gives better results. I think you see the point here. Optimisation will produce so many nonsense results that it is not worth bothering with. 

Look at the broad concepts instead. Make a few different versions of the strategy, representing different conceptual ideas and test them against each other. Find out which concepts work and you get some real value out of your testing, instead of being told if you should have a stop of 3.15 units instead of 3. 

## Practicalities of Futures Trading

The work does not stop after you have designed a robust-trading strategy, rather the contrary; this is when things really begin. Now you need to deal with all the little practical details of the implementation of your strategy and if you have not traded global futures before, you may be in for a few surprises if you are not prepared for them. 

## REQUIRED ASSET BASE

Whether you opt to trade diversified futures for your own account, for managed client accounts or as a hedge fund, you need make sure you have a capital base sufficiently large enough to make full use of the diversification effects without taking on unhealthy levels of risk. If there is a catch to diversified futures trend trading, this would be it. For stock traders the capital base is not a big concern, because their position sizes are divisible into very small amounts and you can easily have 40 open positions in a US$1,000 account and get the same diversification as a fund of a US$100 million. Futures are not divisible in the same way, however, and if your capital base is not large enough you cannot take on many positions without racking up the risks higher than the desired level. In this strategy, positions are sized so that they will target a desired daily average impact on the overall portfolio and if you have an insufficient asset base that formula will indicate that you should buy only a fraction of a contract, which means that you should not buy at all. To illustrate the problem, say you have an account of US$150,000 and you get a buy signa in live cattle. This contract has a size of 40,000 lbs and the ATR at the time of the trade signal was US$0.017. Using the risk factor 0.2%, you would then end up with the following formula for your position size: 

$$
\text { TradeSize } = \frac {1 5 0 , 0 0 0 \times 0 . 0 0 2}{0 . 0 1 7 \times 4 0 , 0 0 0}
$$

The formula would arrive at a trade size of less than half a contract and then you obviously have a problem. To trade diversified futures with too small an asset base would force you to increase the risk factor and if your asset base is significantly smaller than what is required, you will leave the field of professional trading and enter the field of gambling. Trend trading with an asset base of less than US$1 million is in my opinion a bit on the reckless side and even with that amount it can be a bit of a stretch and you may have to make some compromises. I am, of course, aware of stories of people who started trading these strategies on margin accounts of US$10,000 and made millions, and if you feel extremely lucky you could try it out. If 1,000 readers of this book do so, my bet is that about 998 of them wipe out their money in a matter of weeks or months, while two of them make huge returns in a short time before they either end up wiping out as well or are smart enough to quit or reduce risk once they have won their first jackpot. But this book is not about gambling strategies and I strongly recommend against anyone entering this field with less than US$1 million to back them up. 

Trading mini contracts can help a little if you are low on base assets but the availability is not great and the liquidity in some can be low. In the equity world there is an abundance of mini contracts but for some sectors they are hard to come by. In particular in the very important rates sector there is a clear lack of 

proper mini coverage. The agricultural sector has some minis but they are limited and often illiquid with spreads that are too expensive. 

Even if you have US$1 million, you sometimes get trading signals of 1.5 contracts or 0.7 contracts and so on, and you need to decide in advance what to do with such signals. The prudent course of action is of course to round down, but you also want to avoid ending up with too few positions. With a smaller asset base in the range US$1–5 million, you may also need to be more restrictive with your investment universe. As we have seen, increasing the investment universe while keeping all else equal directly increases the risk of the overall strategy, we hope, along with the expected return. You could therefore decrease the number of instruments in the universe to decrease risk, but if you trade too small a number of markets your diversification effects will get too small. There is no easy way to trade diversified futures with smaller assets, but if you do attempt it be sure to do your maths well so that you are aware of the risks involved. 

## GOING LIVE

So the day has come for you to go live. All testing has been done, you are comfortable with the strategy choices you have made, your accounts are opened, the structures are in place and clients’ assets are on the accounts. Excellent, but now the hard part starts. A common question that is often not thought of until quite close to the go-live date is what exactly is to be done on day one. Should you immediately enter all positions that your back-test simulation currently has open or should you wait and just enter into new signals as they come along and slowly build up a portfolio? 

For other types of strategies that answer might not be as clear but in this context there is only one correct choice. You absolutely need to enter into all positions on the first day or you will get a return curve that may look very different from what you expect. You need to calculate the position size for each open position in the simulation based on the day when the trade signal came in, not on the day when you go live, and then enter into the positions when your trading goes live. So if you go live on 2 January and your simulated strategy would have entered into a long soybean trade on 10 December the previous year, you need to calculate the theoretical size that you would have held if you had been trading on 10 December, using the volatility numbers from back then. The reason is, of course, that you want to make sure that your real results match your simulation. 

If you don’t enter into all positions right away, you will not get the same return curve as your simulations predict and you would simply be taking a gamble that the discretionary override, which is what the approach of only taking new signals would really constitute, will tip in your favour. 

You may see situations that look scary on the first day and it may be difficult to enter into them: perhaps a long position that already has a much higher profit than the statistical average and just had two weeks of shooting up like a rocket. The problem is that if you don’t buy it now, when will you? Perhaps it falls back down a little, perhaps not. Perhaps it continues for a year before being stopped out. If you don’t enter all positions right away it will take quite a while before you achieve any meaningful diversification and even longer before your live track record is in sync with simulations. If you happen to go live just before a very profitable phase of the strategy it may take longer to recover the underperformance. Perhaps you start just before a bad period too but that is impossible to predict, and therefore the wise decision is to just stick with the programme. 

## EXECUTION

A practicality you need to think about before commencing trading operations is just how you are going handle the executions when new trade signals are generated. Our strategy in this book assumes that you place market orders before each exchange is open and get the stated open price with a realistic slippage, but this is of course a simplification of reality. The exchange openings can be at very different times of the day and perhaps in the middle of the night for you. Some markets have several trading sessions that you need to take into account and others are practically traded 24 hours a day, making the definition of ‘open’ a little fuzzy. There is also the question of liquidity of course, where in particular some commodity markets can be quite illiquid part of the day, making market orders at those times subject to higher spread costs. 

From my own experience as well as that of colleagues at other futures management companies, I can say for sure that there is a wide range of opinions and different approaches on this subject. Some of the traders have everything automated, with their analytical software sending orders directly to the exchange using pre-programmed algorithms for when and how to execute each market. Other funds have large staffs of execution traders who sometimes are given as much as a week to enter or exit after a signal has been given by the analytical software. For a large fund that could potentially make a significant market footprint when they enter and exit, it makes sense to give execution traders discretion of spreading the trade over a few days but there are also larger funds that use automatic programs to achieve the same thing. For a smaller fund or trader it is of course possible to set defined times of the day when trades are made for different markets and then use a bit of common sense whether to enter a market order or limit order. 

If you do decide to trade in manually to try to get a better price, make sure you measure the result compared to theoretical market orders over time. A good execution trader can beat the average market order but most people cannot do that over time and the core business here is the longer-term trade and not the relatively small difference made by minor variations in the execution price. If it takes a lot of time or costs a lot of money and makes little difference, or even has negative impact, there is little point in keeping up the manual work. Your decision on this aspect is a matter of preference and highly subject to your own skills as an execution trader. 

Depending on your geographical location as well as on your sleep cycle, if you trade global futures you are not likely to be awake at all times when the strategy wants to trade. Assuming you trade only in the opening as the core strategy in this book does, you have quite a bit of time difference between the opening of Japan, Hong Kong, Singapore, Europe and North America. 

If you execute each transaction manually, you are likely not to be around for the opening of each market and thereby your entry price may differ significantly from what your simulation predicts. One way to counter this is to put in market-at-open orders before going to sleep, but if something big happens overnight you may have a problem. 

Another simple way to counter this discrepancy between simulated and actual executions is to make your simulations aware of the problem. If you live in Europe and know that you will not be awake for the opening of Japan, Singapore and Hong Kong, you could simply build into the simulation software that trades are taken at the close for these markets instead of at the open, or even delay execution one day. Try it out in your simulation and see whether it makes a difference to the results or not. 

## CASH MANAGEMENT

One thing you never really see in your simulations is the practicality of cash management. This is just one of those things that are simplified and ignored in most simulation software and although it is not terribly complicated, it is still something you want to be familiar with before starting to trade futures. 

When you open your trading account, whether it is for your own money, a hedge fund or for a client account, you have to decide on the base currency of that account. This is the main currency in which all performance will be calculated. Your account can also have one or more sub-accounts in different currencies, which is what you as a futures trader need. What you want to do is to make sure you have a sub-account for each currency of the futures in your universe. The instruments covered by this book, which are likely to cover what you need, are traded in USD, CHF, EUR, GBP, HKD, JPY and CAD, so these are the accounts you need to set up from day one. When you take on a new position you need to have enough collateral in your account and you should make sure that you always have much more than you need in terms of collateral. Some brokers may require you to post collateral in the same currency while others are happy with the equivalent in another currency, which would likely be your account base currency. 

Futures contracts are marked to market on a daily basis and the daily gain or loss is settled through the clearing house at end of business. So if you have your accounts all set up, put US$1 million in your base USD account and happen to lose £2,000 on long gilts today, you will find yourself in the red on the Sterling account. Note that this is regardless of whether or not your long gilt position is still open. The net gains or losses are always settled daily and the balance shows up on your profit and loss cash accounts. Now you have a choice of doing a spot currency transaction to cover the negative balance on your Sterling or to ignore it and pay the interest rate on the overdraft. 

To avoid this problem, you could transfer an initial amount to each account to cover potential losses. This would mean that you open a currency exposure for those currencies you may not want. This currency exposure is not likely to be very large in terms of per cent of the whole account, so again this leaves you with the choice of leaving it as it is and calling it a rounding error or hedging it away. Unless your account is very small, currency futures make for excellent hedging vehicles. They are cheaper and easier to trade than currency forwards and the spreads are much tighter. The only real negative aspect of using currency futures for hedging is that you cannot trade exact amounts, only multiples of the contract value, which is usually around US$100,000–US$150,000 equivalent for the big contracts. Minis are normally available and liquid enough in this sector though. 

The picture I am trying to paint here is that cash management and its implications is not an exact science and that there are no easy answers on the best course of action. Some might transfer a few hundred thousand to each account and ignore the relatively minor currency exposures, others have great deals on the rates and leave the negative balance as it is, and some may transfer enough money and maintain currency hedges on it. It will not make much difference to the bottom line at the end of the year either way, but it is still a practical detail that needs to be addressed. Table 9.1 shows an example of some subaccounts. 


Table 9.1 Sub-accounts overview example


<table><tr><td>Account</td><td>Currency</td><td>Cash available</td><td>Unrealised P&amp;L</td><td>Account value</td></tr><tr><td>5611.77512-124/U</td><td>USD</td><td>34,124,566.86</td><td>-131,548.22</td><td>33,993,018.64</td></tr><tr><td>5611.77512-124/E</td><td>EUR</td><td>124,886.12</td><td>146,324.87</td><td>271,210.99</td></tr><tr><td>5611.77512-124/C</td><td>CHF</td><td>-12,781.20</td><td>34,819.15</td><td>22,037.95</td></tr><tr><td>5611.77512-124/G</td><td>GBP</td><td>14,379.08</td><td>-2,674.00</td><td>11,705.08</td></tr><tr><td>5611.77512-124/H</td><td>HKD</td><td>14,721,927.45</td><td>2,456,874.23</td><td>17,178,801.68</td></tr><tr><td>5611.77512-124/J</td><td>JPY</td><td>-132,453.00</td><td>278,226.00</td><td>145,773.00</td></tr><tr><td>5611.77512-124/C</td><td>CAD</td><td>74,558.98</td><td>-4,235.73</td><td>70,323.25</td></tr></table>

A certain amount of cash is always needed on your accounts to pay for the settlements of futures and to use as collateral. You may be able to use bonds or similar instruments as collateral as well, depending on your broker and your negotiation position, but having some liquidity on the books cannot be completely avoided. Make sure you have enough to settle your losses and that you are able to pay up for any potential investor redemption. If you have to sell off bonds that you intended to keep to maturity because of unexpected investor fund outflows then something has gone wrong in your cash planning. 

Having said that, it is of course in your interest to keep the cash to a minimum while at the same time at safe enough levels to be able to settle the said expenses and outflows. There are two reasons why you want to minimise the cash on the books and though one of them is well known, the other is increasing in importance these days. The more widely understood reason is the additional interest income you can get from placing excess liquidity with the government, and even though the yields these days are far from what they used to be there is still validity to that argument. Even if you manage to get only 0.25% on the portfolio in a year, it is still free money and while the risk-free moniker can be discussed, it is as close as you get. 

The other reason is that any cash held by your bank or broker will evaporate into thin air if they go bankrupt. I don’t much care if a broker claims that accounts are segregated and that there is no risk, because we have all seen that this is not always the case in real life. All it takes is a former senator with apparent gambling problems as CEO and a billion bucks of customer money can vanish in no time. No matter how much reassurance you get, the truth is that any cash you have on your accounts is likely to either disappear or be locked up in limbo for years if your broker suddenly goes belly up, whereas security holdings such as government debt should be returned to you intact. 

## HIGHER VOLATILITY IN DRAWDOWN MODE

A factor that is easy to forget is that your volatility will be significantly higher whenever you are in a drawdown. When you are having a good year and making good money and new highs your overall performance moves slower than when you just had a bad period. This may sound a bit odd, but take a moment to think about it. The reason for the slower moves in good times has nothing to do with market climate or the strategy as such and this phenomenon is true for practically all hedge funds, managed accounts and similar structures as long as they charge a performance fee. 

When your current result is better than at the last time the performance fee was settled, part of your profits will be offset to account for the accrued performance fee. The money is not physically removed from your account but the accrued liability will be accounted for in the performance calculations. If you charge 15% performance fee on a managed account or fund and you gain 10% from the recent highs, your track record will reflect a gain of only 8.5%. On the other hand, if you are in a profit since the last performance fee settlement and you suffer a loss, the same percentage of the loss will be absorbed by the decrease in the performance fee liability. 

Performance fee therefore works as a stabiliser, dampening both the positive and negative moves in the fund or account as long as you hold a profit since the last high watermark. On the flipside of that, your volatility is higher as a result when you are in a drawdown since there is no performance fee stabiliser anymore. This can work in your favour, helping you regain to the old high watermark quicker, but it can of course also accelerate steep losses if you are not careful. 

## PORTFOLIO MONITORING

Having your fund NAV and the intraday profits and losses ticking in real-time in front of you is a mixed blessing. It is certainly convenient and reassuring to be able to follow your positions intraday. It lets you stay current with the developments in the markets and how your fund responds to it and it gives you a good feel for your portfolio composition and return profile. This type of monitoring is usually available from most futures brokers and if it does not suit your needs you could use your Reuters, Bloomberg or whatever market data system you have and build your own Excel monitoring screen that calculates the P&L for you. 

The question is, of course, whether intraday, tick-by-tick monitoring contributes anything positive. Having the real-time values ticking in front of you does not help your trading and if you have a strategy that just trades on end of day values anyhow, it serves only to increase your stress level and distract your attention from more important tasks. There is very little rational reason why you would want to stare at a ticking portfolio screen during the day if you run a strategy such as the one in this book. 

Of course, despite having said this, I have to confess that I spend much more time that I should watching said screen and I know just how addictive it can be. 

## STRATEGY FOLLOW-UP

Once you are up and running, trading live money and I hope showing good results, the actual work is far from over. One of the most important tasks going forward is to benchmark your actual results with the expected results from your simulations as well as to other futures managers. If you spent all this time developing a solid trading strategy and it turns out that your returns are not closely tracking the expected simulated returns, you need to figure out what is wrong. There will, of course, always be smaller discrepancies between simulations and reality but they should be within a reasonable range and random, and not systematic. If you are a little worse one month and a little better another that is not a big deal, but if you are always a little bit worse then there is a risk that you missed something in your modelling of the strategy and you may find that the negative bias will continue over time. I advise that you err on the side of caution and make sure from the start that the assumptions in your simulations are conservative. Add higher slippage and commissions than you believe you will see in reality. 

Set up a spreadsheet where you do daily calculations of your trading result, net of all fees including accrual management and performance fees as well as all other external costs, and compare this each day with the predicted simulation results. Track closely any trend in the divergence and attempt to locate where it comes from. If you realise that there is a systematic difference between your results and the simulations, you have a real problem and you had better figure out where it comes from before things get worse. 

It helps getting to the details if you calculate daily profits and losses per instrument, both for your actual trading and for your simulations. Most simulation software does not have such an option built in, but if you get one that has an open enough architecture you can just add this yourself. It is not too difficult and you don’t need to be a master programmer to build a plug-in to your analytical software and augment the functionality a little. 

Having the best simulated results possible is a poor comfort if you find your real trading failing to replicate it. 

## 10

## Final Words of Caution

This book deals in highly leveraged derivatives strategies and as such it is wise to dedicate the final chapter to the risks and problems that may arise. 

## DIMINISHING RETURNS OF FUTURES FUNDS

The trend-following business used to be much easier and it is getting tougher and tougher to achieve the big number returns. In the 1980s and 1990s most managers in this business had stellar compound returns with hardly any lasting drawdowns, but those days seem to have been replaced with higher volatility and more uncertain results. The core trend-following strategies are still profitable given enough time, but the return profiles have clearly changed in the past decade. To demonstrate the effect, I have made a composite out of a large number of trend-following futures funds where each fund has an equal weight. Figure 10.1 demonstrates how the returns have changed over the years by showing the 12 months rolling returns for the composite over time. The volatility was certainly larger in the good old days but so was the profitability. Even the superb year of 2008 did not make the composite go flying off the chart as happened back in 1990. 


Figure 10.1 Rolling 12-month compounded return for CTA composite


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/5bc887e1-710a-4041-81ee-b683143d4ddd/87643eb818402b1febcc096942e2de2b6a4fb249a5345b718dfea9bd536a506c.jpg)


There are two main factors driving the diminishing returns in our sector. The first factor was touched upon in Chapter 5, and that is the effect of the free contribution of money from your friendly local government. At any given time, a typical futures manager would have most of the assets under management in government debt, both to earn interest on excess capital and to shield it from counter party risks. During the 1980s and 1990s the income earned from this activity was substantial and served to shift the entire track record of any given manager some per cent up, at times as much as 5–6% on the yearly return. With the current interest levels in 2012, the effect hardly even amounts to a rounding error. Having lost this relatively safe income, the strategy relies solely on its own trading results and the returns automatically shift slightly downwards. 

One can only speculate about whether the extreme low-rates environment we are currently living in will last or things will return to the good old days. Sooner or later rates are likely to come back up to levels where it starts paying off to hand your hard-earned cash over to Big Brother for safe keeping, but this may be far off in the future. It is surely an odd world where interest levels keep going down and closing in on the zero line when at the same time we see so many problems with the large Western governments finances. Normally when borrowers get their credit ratings downgraded, the cost to borrow more rises, but when the United States got downgraded by the S&P in 2011 the yields on US debt fell. The world’s largest rating house points out that the finances of the United States might not be as rosy as everyone thought, and the reaction of people is to buy more of that debt at higher prices. A similar phenomenon is going on in Europe where German debt is seen as all powerful despite the fact that they may end up having to issue 

Eurobonds and back the debt of the Mediterranean countries as well. The Swiss interest rates futures even went into negative territory for a short while in 2011. 

As systematic traders, it is not our job to bet against the madness of crowds, but rather to run alongside the crazies for as long as it lasts and try to get out in time when things turn. This too goes for the yield situation and though we have gained for many years on the constantly shrinking yields, we are now approaching levels where things cannot go much further. The best we can hope for is a long-term reversal, that bonds trend down and yields up for some years, creating both trading profits and higher returns on excess capital. But we may also be looking at a prolonged period with more or less stationary rates at very low levels and that would not be very positive for futures managers. 

The second factor driving diminishing returns is that the behaviour of the markets appears to have changed somewhat. It is said that the most famous last words in the markets are ‘this time it’s different’, and so I tread carefully here. The changes that seem to have occurred over time are mostly related to an increased trading activity and increased volatility. Whereas many markets showed longer and more lasting trends a couple of decades ago we are now experiencing shorter cycles and more violent counter reactions. It is possible that these developments are a result of increased assets available to alternative strategies and the various algorithmic-trading strategies employed by that segment. Incidents such as the 2010 flash crash for instance can be lethal to a leveraged trend follower and until recently these events were practically unheard of. The increasing amount of money managed by trend followers is by itself a possible reason for diminishing returns. When a market starts moving, everyone gets on the bandwagon and propels the price even further, which is all well for us. But when the prices start turning, everyone starts taking their stops at around the same time and what might otherwise have just been a small counter move can turn into a violent adverse price move. 

The effect of these changes has so far not been severe enough to risk compromising the competitiveness of class trend following, but there is nothing to say that the day might come when the core trending models will not be enough. For now it still works, but keep an eye on developments and never stop analysing the markets. 

## ENDING UP IN THE SOUP BOWL

By now you should be very aware of the fact that even in a successful trend-following strategy, most trades end up losing money. The principle is that the ratio between your average gain and average loss is such that the 30–40% of trades that do end up gaining are able to pay for the losing trades and then some. The fact that up to 70% of trades with this strategy fail is very useful information for someone who wishes to construct a counter-trend strategy. 

When a market has been experiencing a range-bound sideways movement and then starts to break out, there will be plenty of initial buying pressure from people like us who are betting that the breakout is real and that a new trend will emerge. This can temporarily push prices in the breakout direction, further than what was justified, and there are several interesting strategies published for how one could take advantage of this phenomenon to take the opposite trade for a short-term profit at the expense of us trend followers. This is all fair of course, but it can be costly if you happen to trade at the same time as the crowd, and if this seems a problem in your back tests you may want to look into different entry tactics. Instead of blindly buying the breakout, you could enter in several steps, wait for a breakout, or manually trade into each position over a few days. Just be aware that sharks are out there who are aware of your type of strategies and anticipating your entries. Linda Raschke and Laurence Connors’ excellent book from 1996, Street Smarts: High Probability Short-Term Strategies, details methods that a short-term operator could use to gain at the expense of trend followers. 

# SETTING THE INITIAL RISK LEVEL

One of the most important decisions you need to make before starting actual trading is what risk level to aim for. Setting your position sizes is the key control factor for setting the risk and if you set it too low you will not be able to get enough returns to attract capital, but if you set it too high you risk having the kind of drawdowns that scare investors off. 

When you are making this call, keep in mind that the maximum drawdown will probably be higher than what your simulations predict and perhaps it will happen soon after your launch. The fact of the matter is that this happens more often than one might think. The very reason that a new fund starts with this type of strategy and finds sufficient initial investors for it may be that trend-following strategies just had a very good run and got plenty of attention. This is exactly what happened to so many new funds after 2008. This strategy absolutely dominated the headlines and massively outperformed practically all other strategies, except of course those who were massively betting against the Credit Default Swaps markets. It is much easier to find traction for a venture like this after a very good return period and investors tend to come into these funds after these good years. The problem is that they will come in with an expectation that the good times will continue in the near future and as we have seen in this book, this is not often the case. After a very strong performance period, we are likely to see some troubled times, large drawdowns, volatile years of sideways or losing results. 

Funds that launched just after 2008, or after other good periods as well for that matter, found themselves in a very dangerous position. If you invested in a typical trend-following futures fund at the start of 2009, after having read all about the strategy that beat the markets in the otherwise disaster year that just passed, you would be in for a very tough ride. Most trend followers had large losses in 2009, many over 20% drawdowns during that year. Plenty of the new capital that came into trend-following funds in early 2009 had already left by the end of that year as investors got scared over the difference in what they thought they would get and what reality looked like. For those who stayed in, 2010 was for the most part a bad year as well. In the last half of 2010 the profitable trends came back and started making the money back for the patient investors. 

So if you had launched a new fund in early 2009, you would find yourself over a year and a half later with a likely drawdown of 20–25%, perhaps more. A fund that had been in business a couple of decades longer with good track record could survive this, but a new fund would likely not. 

What I want to say about this is, be very careful when you start out. If you set a high risk level you may perhaps look like a hero if you get lucky and get some good trends soon after the launch, but if you are unlucky and get a bad year or two, you are out of business. Survival must always be the first priority and this means starting out in a comfortable scale, making sure you are able to handle a bad period, even if it happens to come along at the very start. 

I hope my attempts at giving a fair and balanced picture of the reality that faces a trend-following futures manager has not discouraged you from getting into the business. For all the possible pitfalls, this is still a very good business to be in and even with the diminishing returns of the past years there are no real signs that cross-asset trend following should not be profitable in the future. 

# OFFICIAL BOOK WEBSITE

www.followingthetrend.com 

# RESEARCH PAPERS, ARTICLES AND WEBSITES

Absolute Returns, www.absolutereturns.com (accessed 24 August 2012) 

Automated Trading System, www.automated-trading-system.com (accessed 24 August 2012) 

Barclay Hedge, www.barclayhedge.com (accessed 24 August 2012) 

Basu, Devraj, ‘Capturing Commodity Backwardation’, Futures magazine, May 2011 

Basu, Devraj and Stremme, Alexander, ‘The Economic Value of Linkage between Spot and Futures Market’, February 2009 

Burghardt, Galen and Walls, Brian, ‘Two Benchmarks for Momentum Trading’, NewEdge AlternativeEdge Research, 2010 

Cooper, Tony, ‘Alpha Generation and Risk Smoothing using Managed Volatility’, August 2010 

Faith, Curtis, ‘The Original Turtle Trading Rules’, 2003, http://www.benvanvliet.net/Downloads/turtlerules.pdf (accessed 24 August 2012) 

IASG Managed Futures Database, www.iasg.com (accessed 24 August 2012) 

Kaminski, Kathryn and Lo, Andrew W., ‘When Do Stop-Loss Rules Stop Losses?’, January 2007 

Koulajian, Nigol and Czkwianianc, Paul, ‘Black Box Trend Following – Lifting the Veil’, 2010 

Koulajian, Nigol and Czkwianianc, Paul, ‘Know your Skew’, 2011 

National Futures Association, www.nfa.futures.org (accessed 24 August 2012) 

Standard and Poor’s, ‘Standard and Poor’s Indices Versus Active (SPIVA)’, www.standardandpoors.com/indices/spiva/en/us (accessed 24 August 2012) 

Wilkes, Thomas and Fletcher, Laurence, ‘Special Report: The Algorithmic Arms Race’, Reuters 2012 

## BOOKS

Chande, Tushar, Beyond Technical Analysis, John Wiley & Sons Inc., Hoboken, 2001 

Covel, Michael, Trend Following, FT Press, 2009 

Fabozzi, Frank, The Handbook of Fixed Income Securities, McGraw-Hill, 2005 

Faith, Curtis, Way of the Turtle: The Secret Methods that Turned Ordinary People into Legendary Traders, McGraw-Hill, 1997 

Gyllenram, Carl, Trading with Crowd Psychology, John Wiley & Sons Inc., Hoboken, 2000 

Ineichen, Alexander, Absolute Returns, John Wiley & Sons Inc., Hoboken, 2003 

Ineichen, Alexander, Asymmetric Returns, John Wiley & Sons Inc., Hoboken, 2007 

Leeson, Nick, Rogue Trader, Warner, 1997 

Lefèvre, Edwin, Reminiscences of a Stock Operator, John Wiley & Sons Inc., Hoboken, 1923 

McCrary, Stuart, How to Create and Manage a Hedge Fund, John Wiley & Sons Inc., Hoboken, 2002 

Raschke, Linda and Connors, Laurence, Street Smarts: High Probability Short-Term Strategies, M. Gordon Publishing Group 1996 

Rogers, Jim, Hot Commodities: How Anyone Can Invest Profitably in the World’s Best Market, John Wiley & Sons Ltd, Chichester, 2004 

Schwager, Jack, Market Wizards: Interviews with Top Traders, Harper, 1992 

Schwager, Jack, Schwager on Futures: Fundamental Analysis, John Wiley & Sons Inc., Hoboken, 1998 

Schwager, Jack, Schwager on Futures: Technical Analysis, John Wiley & Sons Inc., Hoboken, 1995 

Ugrina, Tony and Gyllenram, Carl, En Aktiespekulants Psykologi, Liber AB, 2004 

Wong, Max, Bubble Value at Risk: Extremistan and Procyclicality, Immanuel Consulting PTE, 2011 

## Index

Abraham Trading Company Diversified Program 

agriculture 

asset base requirements 

ATR see average true range automatic trading average holding periods average true range (ATR) method back-adjusted charts backwardation banking Barclay’s BTOP basic strategies basis gaps beginning trading behaviour, strategy benchmark generation benchmark performance, mutual funds bond futures bonds BP see British Pounds breakouts detection filters overtrading performance standard strategies 

management forms psychological preparedness redemptions seed funds subscriptions volatility profiles 

buy-and-hold strategies
calendar spreads
Campbell Composite
cash management
CLR see Common Language Runtime
coding of contracts
commission
commodities
agricultural/non-agricultural CTAs
Heavy Investment Universe rollover effect
commodity trading advisors (CTAs)
Common Language Runtime (CLR)
competition
competitiveness
Conquest Managed Futures Select
contango
contract sizes
core strategy
trading rules
year by year reviews
correlations
futures funds
matrices
trading strategies
costs
counter-trend strategies
credit crunch
credit meltdowns 

basis gaps correlation natural log returns open interest storage term structures vendors 

futures concepts traditional investment approach 

dollar see Eurodollar; US Dollar vs Euro 

drawdowns (DD) 

Dunn World Monetary and Agricultural Program 

Eckhardt Trading Company Standard Plus 

efficient frontiers 

energy sector 

entry rules 

Equal-Weighted Investment Universe 

equal weighting 

equities 

complementary diversified futures futures mutual funds real-world performance rollover effect traditional investment approach 

equity-reduced large investment universes 

ETFs see exchange-traded funds 

Eurodollar 

Euro futures 1992 

EuroStoxx 

2003 2008-9 

EuroSwiss performance 2011 

Euro vs US Dollar 2002 

excess cash 

exchange rates 

exchanges, futures 

Campbell Composite Mulvaney Capital Management Global Markets Fund Palm Trend Fund Sunrise Capital Diversified Transtrend Standard Risk Program 

as asset class complementary equity portfolios concept cross-asset trend following data basis gaps open interest term structures definition delivery codes diversified strategies Euro futures exchanges initial margins lifetimes performance vs equities properties 

sectors
tools
trend-follower performance
see also diversified managed futures

gasoline prices

German Bund 2001

German Schatz

gilts

going live

gold

government debt securities

Gulf War 1

hard stops

heating oil

hedge funds

Henry Hub national gas

holding periods

improvements

correlation matrices
counter-trend components
multiple time frames
optimization
parameter stability checks
position sizing
risk control
rollover effect
stops mechanisms
synthetic contracts
trend filters

in-depth performance analysis

behaviour analysis
cash management
equity/futures mixes
leverage
sector impact
trading direction index-linked funds
initial margins
initial risk levels
interest
cash management
liquidity
STIRS
internal correlation, equities
intraday stops
investment universes
Commodity Heavy
comparison
Equal-Weighted
Financially Heavy
Large
liquidity
ISAM Systematic Fund Classic A
Japanese disaster 2011
Large Investment Universe
last trading days
launching fund
leverage
LIBOR
lifetimes
cash
futures
limited
multiple time frames
rollover effect
liquidity
live cattle trends 2009
LME see London Metal Exchange log returns
London Metal Exchange (LME)
long trades
sectors
trading direction
losing/winning phases
maintenance margins
managed funds
manual trading
margins
margin-to-equity position sizing
marketability
market behaviour
market footprint
mark-to-market accounting
metals
Milburn Diversified Futures Program
mini contracts
monitoring portfolios
monthly returns
correlations
risk control
strategy simulation
months, delivery codes
moving average cross strategies
filters
overtrading
performance
principles 

Mulvaney Capital Management Global Markets Fund Nasdaq 1999 2006 natural gas natural log returns negative market correlation non-agricultural commodities oats 1998 open interest Operation Desert Shield optimization overtrading palladium Palm Trend Fund parameter stability performance Abraham Trading Company Diversified Program benchmark generation Campbell Composite cash management Conquest Managed Futures Select Eckhardt Trading Company Standard Plus equities equity/futures mixes evaluation existing funds since 1977 follow-up strategy reviews futures investment universe comparison ISAM Systematic Fund Classic A Mulvaney Capital Management Global Markets Fund Palm Trend Fund portfolio monitoring result distributions rollover effect Sunrise Capital Diversified 

personality of strategies platinum point values portfolios diversification equities monitoring position sizing practicalities prices profitability programming psychological preparedness rates realtime monitoring redemptions required asset base reverse engineering existing fund replication investment universes reviews see year by year reviews RightEdge 

risk 

drawdown volatility improvements initial levels investment universes managed futures short selling 

Transtrend Standard Risk Program
rollover effects
rough rice basis gap
sales pitches
scalability
sectors
agricultural commodities
energy
long trades
non-agricultural commodities
performance analysis
seed funds
Sharpe ratio
short selling
short-term interest rate futures (STIRs)
short-term operators
silver
single-instrument trend following
slippage
smoothing
Sortino ratio
sovereign debt
Soviet Union coup d’état’
Soybeans in 2007
spreads, synthetic contracts
starting up
stationarity
STIRs see short-term interest rate futures
stops average true range methods intraday storage, data strategy behaviour subscriptions Sunrise Capital Diversified survival bias synthetic contracts term structures ticker code time horizons tools tracker funds trade signals trading direction trading strategies basic strategies behaviour analysis benchmark generation breakout strategies construction core rules correlations costs counter-trends direction diversification efficient frontiers equity/futures mixes essential considerations execution existing funds filters follow-up improvements initial risk intraday stops investment universes 

moving average cross strategies multiple time frames optimization parameter stability performance personality portfolio monitoring position sizing principles risk levels sector impact stop loss reduction stops, intraday synthetic contracts volatility 

traditional investment approach 

Transtrend Standard Risk Program 

trend filters 

trend following 

phases rules strategies words of caution year by year reviews 

US Dollar vs Euro 2002 

value-at-risk (VaR) 

volatility 

bond futures Campbell Composite drawdowns equities evaluation future profiles stop rule adjustment 

volume spiking WealthLab.net whipsawing winning/losing phases 