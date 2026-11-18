

<!-- === Source: MinerU_markdown_Rishi_Narang_-_Inside_the_Black_Box_1_2122156029113376770.md (Page 1) === -->

Copyright © 2009 by Rishi K Narang. All rights reserved. 

Published by John Wiley & Sons, Inc., Hoboken, New Jersey. Published simultaneously in Canada. 

No part of this publication may be reproduced, stored in a retrieval system, or transmitted in any form or by any means, electronic, mechanical, photocopying, recording, scanning, or otherwise, except as permitted under Section 107 or 108 of the 1976 United States Copyright Act, without either the prior written permission of the Publisher, or authorization through payment of the appropriate per-copy fee to the Copyright Clearance Center, Inc., 222 Rosewood Drive, Danvers, MA 01923, (978) 750-8400, fax (978) 646-8600, or on the web at www.copyright.com. Requests to the Publisher for permission should be addressed to the Permissions Department, John Wiley & Sons, Inc., 111 River Street, Hoboken, NJ 07030, (201) 748-6011, fax (201) 748-6008, or online at http://www.wiley.com/go/permissions. 

Limit of Liability/Disclaimer of Warranty: While the publisher and author have used their best efforts in preparing this book, they make no representations or warranties with respect to the accuracy or completeness of the contents of this book and specifically disclaim any implied warranties of merchantability or fitness for a particular purpose. No warranty may be created or extended by sales representatives or written sales materials. The advice and strategies contained herein may not be suitable for your situation. You should consult with a professional where appropriate. Neither the publisher nor author shall be liable for any loss of profit or any other commercial damages, including but not limited to special, incidental, consequential, or other damages. 

For general information on our other products and services or for technical support, please contact our Customer Care Department within the United States at (800) 762-2974, outside the United States at (317) 572-3993 or fax (317) 572-4002. 

Wiley also publishes its books in a variety of electronic formats. Some content that appears in print may not be available in electronic books. For more information about Wiley products, visit our web site at www.wiley.com. 

Library of Congress Cataloging-in-Publication Data: 

Narang, Rishi K, 1974-
Inside the black box: the simple truth about quantitative trading /
Rishi K Narang.
p. cm. – (Wiley finance series)
Includes bibliographical references and index.
ISBN 978-0-470-43206-8 (cloth)
1. Portfolio management–Mathematical models. 2. Investment analysis–Mathematical models. 3. Stocks–Mathematical models. I. Title.
HG4529.5.N37 2009
332.64'2-dc22 

2009010579 

Printed in the United States of America 

10 9 8 7 6 5 4 3 2 1 

TRADING SOFTWARE 

FOR SALE & EXCHANGE 

# www.trading-software-collection.com

Mirrors: 

www.forex-warez.com 

www.traders-software.com 

www.trading-software-download.com 

Join My Mailing List 

This book is dedicated to my father and mother, Thakur and Krishna Narang, to whom I owe so much, and to my wife and partner of many years, Carolyn Wong, whose love and support make a hell of a lot of things really a lot better. 

## Contents

Preface xi
Acknowledgments xv
PART ONE
The Quant Universe
CHAPTER 1
Why Does Quant Trading Matter? 3
The Benefit of Deep Thought 7
The Measurement and Mismeasurement of Risk 8
Disciplined Implementation 10
Summary 10
CHAPTER 2
An Introduction to Quantitative Trading 11
What Is a Quant? 12
What Is the Typical Structure of a Quantitative Trading System? 14
Summary 17
PART TWO
Inside the Black Box
CHAPTER 3
Alpha Models: How Quants Make Money 21
Types of Alpha Models: Theory Driven and Data Driven 22
Theory-Driven Alpha Models 24
Data-Driven Alpha Models 37
Implementing the Strategies 38 

Blending Alpha Models 48
Summary 53
CHAPTER 4
Risk Models 55
Limiting the Amount of Risk 57
Limiting the Types of Risk 60
Summary 64
CHAPTER 5
Transaction Cost Models 67
Defining Transaction Costs 68
Types of Transaction Cost Models 72
Summary 77
CHAPTER 6
Portfolio Construction Models 79
Rule-Based Portfolio Construction Models 80
Portfolio Optimizers 85
Output of Portfolio Construction Models 95
How Quants Choose a Portfolio Construction Model 96
Summary 96
CHAPTER 7
Execution 99
Order Execution Algorithms 100
High-Frequency Trading: Blurring the Line between Alpha and Execution 105
Trading Infrastructure 107
Summary 108
CHAPTER 8
Data 111
The Importance of Data 111
Types of Data 113
Sources of Data 115
Cleaning Data 117
Storing Data 122
Summary 124 

CHAPTER 9
Research 125
Blueprint for Research: The Scientific Method 125
Idea Generation 127
Testing 129
Summary 145

PART THREE
A Practical Guide for Investors in Quantitative Strategies
CHAPTER 10
Risks Inherent to Quant Strategies 149
Model Risk 150
Regime Change Risk 154
Exogenous Shock Risk 158
Contagion, or Common Investor, Risk 159
How Quants Monitor Risk 166
Summary 168

CHAPTER 11
Criticisms of Quant Trading: Setting the Record Straight 169
Trading Is an Art, Not a Science 169
Quants Cause More Market Volatility by Underestimating Risk 171
Quants Cannot Handle Unusual Events or Rapid Changes in Market Conditions 174
Quants Are All the Same 176
Only a Few Large Quants Can Thrive in the Long Run 178
Quants Are Guilty of Data Mining 179
Summary 182

CHAPTER 12
Evaluating Quants and Quant Strategies 185
Gathering Information 186
Evaluating a Quantitative Trading Strategy 188
Evaluating the Acumen of Quantitative Traders 191
The Edge 193
Evaluating Integrity 196
How Quants Fit into a Portfolio 198
Summary 201 

CHAPTER 13
Looking to the Future of Quant Trading 203
Notes 207
About the Author 212
Index 213 

# Preface

An unnecessary opaqueness surrounds quantitative trading strategies (known to many as black boxes), despite their importance to the capital markets and the sensational, widely known examples of their successes and failures. This opaqueness, which quants themselves frequently perpetuate, exacerbates an already widespread misunderstanding of quantitative trading in the broader investment community. 

This book takes you on a tour through the black box, inside and out. It sheds light on the work that quants do, lifting the veil of mystery that surrounds quantitative trading and allowing those interested in doing so to evaluate quants and their strategies. 

The first thing that should be made clear is that people, not machines, are responsible for most of the interesting aspects of quantitative trading. Quantitative trading can be defined as the systematic implementation of trading strategies that human beings create through rigorous research. In this context, systematic is defined as a disciplined, methodological, and automated approach. Despite this talk of automation and systematization, people conduct the research and decide what the strategies will be, people select the universe of securities for the system to trade, and people choose what data to procure and how to clean those data for use in a systematic context, among a great many other things. These people, the ones behind quant trading strategies, are commonly referred to as quants or quant traders. 

Quants employ the scientific method in their research. Though this research is aided by technology and involves mathematics and formulae, the research process is thoroughly dependent on human decision making. In fact, human decisions pervade nearly every aspect of the design, implementation, and monitoring of quant trading strategies. As it turns out, quant strategies and traditional discretionary investment strategies, which rely on human decision makers to manage portfolios day to day, are rather similar in what they do. 

The differences between a quant strategy and a discretionary strategy can be seen in how the strategy is created and in how it is implemented. By carefully researching their strategies, quants are able to assess their ideas the same way that scientists test theories. Furthermore, by utilizing a computerized, systematic implementation, quants eliminate the arbitrariness that pervades so many discretionary trading strategies. In essence, decisions driven by emotion, indiscipline, passion, greed, and fear—what many consider the key pratfalls of “playing the market”—are eliminated from the quant’s investment process. They are replaced by an analytical and systematic approach that borrows from the lessons learned in so many other fields: If something needs to be done repeatedly and with a great deal of discipline, computers will virtually always outshine humans. We simply aren’t cut out for repetition in the way that computers are, and there’s nothing wrong with that. Computers, after all, aren’t cut out for creativity the way we are; without humans telling computers what to do, computers wouldn’t do much of anything. The differences in how a strategy is designed and implemented play a large part in the consistent, favorable risk/reward profile a well-run quant strategy enjoys relative to most discretionary strategies. 

To clarify the scope of this book, it is important to note that I focus on “alpha”-oriented strategies and largely ignore quantitative index traders or other implementations of “beta” strategies. Alpha strategies attempt to generate returns by skillfully timing the selection and/or sizing of various portfolio holdings; beta strategies mimick or slightly improve on the performance of an index, such as the S&P 500. Though quantitative index fund management is a large industry, it requires little explanation. Neither do I spend much time on the field of financial engineering, which typically plays a role in creating or managing new financial products (e.g., CDOs). Nor do I address quantitative analysis, which typically supports discretionary investment decisions. Both of these are interesting subjects, but they are so different from quant trading as to be deserving of their own, separate discussions carried out by experts in those fields. 

This book is divided into three parts. Part One (Chapters 1 and 2) provides a general but useful background on quantitative trading. Part Two (Chapters 3 through 9) details the contents of the black box. Part Three (Chapters 10 through 13) provides an analysis of quant trading and techniques that may be useful in assessing quant traders and their strategies. 

It is my aspiration to explain quant trading in an intuitive manner. I describe what quants do and how they do it by drawing on the economic rationale for their strategies and the theoretical basis for their techniques. Equations are avoided, and the use of jargon is limited and explained, when required at all. My aim is to demonstrate that what many call a black box is in fact transparent, intuitively sensible, and readily understandable. I also explore the lessons that can be learned from quant trading about investing in general and how to evaluate quant trading strategies and their practitioners. As a result, Inside the Black Box may be useful for a variety of participants in and commentators on the capital markets. For portfolio managers, analysts, and traders, whether quantitative or discretionary, this book will help contextualize what quants do, how they do it, and why. For investors, the financial media, or anyone with a reasonable knowledge of capital markets in general, this book will engender a deeper understanding of this niche. 

RISHI K NARANG 

# Acknowledgments

This book would not be readable without the untiring editing of Arzhang Kamarei. My colleagues at Telesis Capital, Myong Han and Yimin Guo, similarly read through countless revisions of this text and offered many invaluable and timely suggestions. I am grateful to Sudhir Chhikara, one of the brightest quants I know, for taking the time to read Inside the Black Box and provide many constructive criticisms. I'd also like to thank Aaron and Sandor Straus of Merfin LLC for their help with the Data chapter. 

I am indebted to my brother, Manoj Narang, from whom I have learned so much. Vijay Prabhakar provided many helpful suggestions and answers to questions related to machine learning, as Rick Durand did with the subject of optimization. 

I am grateful to Steve Drobny for being hugely helpful and an enabler in the infancy of this project and for coming up with its title. Without him, it is extraordinarily unlikely I would ever have started. John Bonaccolta, too, was there in the earliest days, providing suggestions and encouragement when it was greatly needed. 

Similarly, I must acknowledge the help of the rest of my partners at Telesis Capital: R. Alexander Burns, Julie Wilson, Eric Cressman, and John Cutsinger. Richard Vigilante offered a few extremely important criticisms early on, which helped shape the book. 

For their help with getting some metrics on the size of the quant trading universe, I'd like to thank Keith Johnson and Ryan Duncan of Newedge, Greg Lindstrom and Matthew Rothman of Barclays, Dan Kenna of Morgan Stanley, Markus Gsell and Albert Menkveld, the TABB group, Sang Lee of the Aite Group, and the Barclay Group. Underlying data, where necessary, were downloaded from Yahoo! Finance or Bloomberg, unless otherwise noted. 

The Quant Universe 

# Why Does Quant Trading Matter?

Look into their minds, at what wise men do and don't.
—Marcus Aurelius, Meditations 

John is a quant trader running a midsized hedge fund. He completed an undergraduate degree in mathematics and computer science at a top school in the early 1990s. John immediately started working on Wall Street trading desks, eager to capitalize on his quantitative background. After seven years on the Street in various quant-oriented roles, John decided to start his own hedge fund. With partners handling business and operations, John was able to create a quant strategy that recently was trading over $1.5 billion per day in equity volume. More relevant to his investors, the strategy made money on 60 percent of days and 85 percent of months—a rather impressive accomplishment. 

Despite trading billions of dollars of stock every day, there is no shouting at John's hedge fund, no orders being given over the phone, and no drama in the air; in fact, the only sign that there is any trading going on at all is the large flat-screen television in John's office that shows the strategy's performance throughout the day and its trading volume. John can't give you a fantastically interesting story about why his strategy is long this stock or short that one. While he is monitoring his universe of thousands of stocks for events that might require intervention, for the most part he lets the automated trading strategy do the hard work. What John monitors quite carefully, however, is the health of his strategy and the market environment's impact on it. He is aggressive about conducting research on an ongoing basis to adjust his models for changes in the market that would impact him. 

Across from John sits Mark, a recently hired partner of the fund who is researching high-frequency trading. Unlike the firm's first strategy, which only makes money on 6 out of 10 days, the high-frequency efforts Mark and 

John are working on target a much more ambitious task: looking for smaller opportunities that can make money every day. Mark's first attempt at high-frequency strategies already makes money nearly 95 percent the time. In fact, their target for this high-frequency business is even loftier: They want to replicate the success of those firms whose trading strategies make money every hour, maybe even every minute, of every day. Such high-frequency strategies can't accommodate large investments, because the opportunities they find are small, fleeting. Nonetheless, they are highly attractive for whatever capital they can accommodate. Within their high-frequency trading business, John and Mark expect their strategy to generate at least 200 percent a year, possibly much more. 

There are many relatively small quant trading boutiques that go about their business quietly, as John and Mark's firm does, but that have demonstrated top-notch results over reasonably long periods. For example, Quantitative Investment Management of Charlottesville, Virginia, averaged over 20 percent per year for the 2002–2008 period—a track record that many discretionary managers would envy. $^{1}$ 

On the opposite end of the spectrum from these small quant shops are the giants of quant investing, with which many investors are already quite familiar. Of the many impressive and successful quantitative firms in this category, the one widely regarded as the best is Renaissance Technologies. Renaissance, the most famous of all quant funds, is famed for its 35 percent average yearly returns (after exceptionally high fees), with extremely low risk, since 1990. In 2008, a year in which many hedge funds struggled mightily, Renaissance's flagship Medallion Fund gained approximately 80 percent. $^{2}$ I am personally familiar with the fund's track record, and it's actually gotten better as time has passed—despite the increased competition and potential for models to “stop working.” 

Not all quants are successful, however. It seems that once every decade or so, quant traders cause—or at least are perceived to cause—markets to move dramatically because of their failures. The most famous case by far is, of course, Long Term Capital Management (LTCM), which nearly (but for the intervention of Federal Reserve banking officials and a consortium of Wall Street banks) brought the financial world to its knees. Although the world markets survived, LTCM itself was not as lucky. The firm, which averaged 30 percent returns after fees for four years, lost nearly 100 percent of its capital in the debacle of August–October 1998 and left many investors both skeptical and afraid of quant traders (although it is debatable whether this was a quant trading failure or a failure of human judgment in risk management, and it’s questionable whether LTCM was even a quant trading firm at all). 

Not only have quants been widely panned because of LTCM, but they have also been blamed (probably unfairly) for the crash of 1987 and (quite 

TRADING SOFTWARE 

FOR SALE & EXCHANGE 

# www.trading-software-collection.com

Mirrors: 

www.forex-warez.com 

www.traders-software.com 

www.trading-software-download.com 

Join My Mailing List 

fairly) for the eponymous quant liquidation of 2007, the latter having severely impacted many quant shops. Even some of the largest names in quant trading suffered through August 2007's quant liquidation. For instance, Goldman Sachs' largely quantitative Global Alpha Fund was down an estimated 40 percent in 2007 after posting a 6 percent loss in 2006. $^{3}$ In less than a week during August 2007, many quant traders lost between 10 and 40 percent in a few days, though some of them rebounded strongly for the remainder of the month. 

Spectacular success and failure aside, there is no doubt that quants cast an enormous shadow on the trading marketplace virtually every trading day. Across U.S. equity markets, a significant, and rapidly growing, proportion of all trading is done through algorithmic execution, one footprint of quant strategies. (Algorithmic execution is the use of computer software to manage and “work” an investor’s buy and sell orders in electronic markets.) Although this automated execution technology is not the exclusive domain of quant strategies—any trade that needs to be done, whether by an index fund or a discretionary macro trader, can be worked using execution algorithms—certainly a substantial portion of all algorithmic trades are done by quants. Furthermore, quants were both the inventors of, and primary innovators of, algorithmic trading engines. A mere five such quant traders account for about 1 billion shares of volume per day, in aggregate, in the United States alone. It is worth noting that not one of these is well known to the broader investing public. The TABB Group, a research and advisory firm focused exclusively on the capital markets, estimates that, in 2008, approximately 58 percent of all buy-side orders were algorithmically traded. TABB also estimates that this figure has grown some 37 percent per year, compounded, since 2005. More directly, the Aite Group published a study in early 2009 indicating that more than 60 percent of all US equity transactions are attributable to short term quant traders. $^{4}$ These statistics hold true in non-U.S. markets as well. Black-box trading accounted for 45 percent of the volume on the European Xetra electronic order-matching system in the first quarter of 2008, which is 36 percent more than it represented a year earlier. $^{5}$ 

The large presence of quants is not limited to equities. In futures and foreign exchange markets, the domain of commodity trading advisors (CTAs), there is a significant presence of quants. The Barclay Group, proprietor of the most comprehensive commercially available database of CTAs and CTA performance, estimates that well over 85 percent of the assets under management among all CTAs are managed by quantitative trading firms. Although a great many of the largest and most established CTAs (and hedge funds generally) do not report their assets under management or performance statistics to any database, a substantial portion of these firms are actually quants also, and it is likely that the “real” figure is still over 75 percent. As of the end of the third quarter of 2008, the amount of quantitative futures money under management, including only the firms that report to Barclay, was $227.0 billion. 

It is clear that the magnitude of quant trading among hedge funds is substantial. Hedge funds are private investment pools that are accessible only to sophisticated, wealthy individual or institutional clients. They can pursue virtually any investment mandate one can dream up, and they are allowed to keep a portion of the profits they generate for their clients. But this is only one of several arenas in which quant trading is widespread. Proprietary trading desks at the various banks, boutique proprietary trading firms, and various “multistrategy” hedge fund managers who utilize quantitative trading for a portion of their overall business each contribute to a much larger estimate of the size of the quant trading universe. 

With such size and extremes of success and failure, it is not surprising that quants take their share of headlines in the financial press. And though most press coverage of quants seems to be markedly negative, this is not always the case. In fact, not only have many quant funds been praised for their steady returns (a hallmark of their disciplined implementation process), but some experts have even argued that the existence of successful quant strategies improves the marketplace for all investors, regardless of their style. For instance, Reto Francioni (chief executive of Deutsche Boerse AG, which runs the Frankfurt Stock Exchange) said in a speech that algorithmic trading “benefits all market participants through positive effects on liquidity.” Francioni went on to reference a recent academic study showing “a positive causal relationship between algo trading and liquidity.” $^{6}$ Indeed, this is almost guaranteed to be true. Quant traders, using execution algorithms (hence, “algo trading”), typically slice their orders into many small pieces to improve both the cost and efficiency of the execution process. As mentioned before, although originally developed by quant funds, these algorithms have been adopted by the broader investment community. By placing many small orders, other investors who might have different views or needs can also get their own executions improved. 

Quants typically make markets more efficient for other participants by providing liquidity when other traders' needs cause a temporary imbalance in the supply and demand for a security. These imbalances are known as "inefficiencies," after the economic concept of "efficient markets." True inefficiencies (such as an index's price being different from the weighted basket of the constituents of the same index) represent rare, fleeting opportunities for riskless profit. But riskless profit, or arbitrage, is not the only—or even primary—way in which quants improve efficiency. The main inefficiencies quants eliminate (and, thereby, profit from) are not absolute and unassailable but rather probabilistic and requiring risk taking. 

A classic example of this is a strategy called statistical arbitrage, and a classic statistical arbitrage example is a pairs trade. Imagine two stocks with similar market capitalizations from the same industry and with similar business models and financial status. For whatever reason, Company A is included in a major market index, an index that many large index funds are tracking. Meanwhile, Company B is not included in any major index. It is likely that Company A's stock will subsequently outperform shares of Company B simply due to a greater demand for the shares of Company A from index funds, which are compelled to buy this new constituent in order to track the index. This outperformance will in turn cause a higher P/E multiple on Company A than on Company B, which is a subtle kind of inefficiency. After all, nothing in the fundamentals has changed—only the nature of supply and demand for the common shares. Statistical arbitrageurs may step in to sell shares of Company A and buy shares of Company B, thereby preventing the divergence between these two fundamentally similar companies from getting out of hand while improving efficiency in market pricing. 

This is not to say that quants are the only players who attempt to profit by removing market inefficiencies. Indeed, it is likely that any alpha-oriented trader is seeking similar sorts of dislocations as sources of profit. And of course, there are times, such as August 2007, when quants actually cause the markets to be less efficient. Nonetheless, especially in smaller, less liquid, and more neglected stocks, statistical arbitrage players are often major providers of market liquidity and help establish efficient price discovery for all market participants. 

So, what can we learn from a quant's approach to markets? The three answers that follow represent important lessons that quants can teach us—lessons that can be applied by any investment manager. 

## THE BENEFIT OF DEEP THOUGHT

According to James Simons, the founder of the legendary Renaissance Technologies, one of the greatest advantages quants bring to the investment process is their systematic approach to problem solving. As Dr. Simons puts it, “The advantage scientists bring into the game is less their mathematical or computational skills than their ability to think scientifically.” $^{7}$ 

The first reason it is useful to study quants is that they are forced to think deeply about many aspects of their strategy that are taken for granted by nonquant investors. Why does this happen? Computers are obviously powerful tools, but without absolutely precise instruction, they can achieve nothing. So, to make a computer implement a “black-box trading strategy” requires an enormous amount of effort on the part of the developer. You can't tell a computer to "find cheap stocks." You have to specify what find means, what cheap means, and what stocks are. For example, finding might involve searching a database with information about stocks and then ranking the stocks within a market sector (based on some classification of stocks into sectors). Cheap might mean P/E ratios, though one must specify both the metric of cheapness and what level will be considered cheap. As such, the quant can build his system so that cheapness is indicated by a 10 P/E or by those P/Es that rank in the bottom decile of those in their sector. And stocks, the universe of the model, might be all U.S. stocks, all global stocks, all large cap stocks in Europe, or whatever other group the quant wants to trade. 

All this defining leads to a lot of deep thought about exactly what one's strategy is, how to implement it, and so on. In the preceding example, the quant doesn't have to choose to rank stocks within their sectors. Instead, stocks can be compared to their industry peers, to the market overall, or to any other reasonable group. But the point is that the quant is encouraged to be intentional about these decisions by virtue of the fact that the computer will not fill in any of these blanks on its own. 

The benefit of this should be self-evident. Deep thought about a strategy is usually a good thing. Even better, this kind of detailed and rigorous working out of how to divide and conquer the problem of conceptualizing, defining, and implementing an investment strategy is useful to quants and discretionary traders alike. These benefits largely accrue from thoroughness, which is generally held to be a key ingredient to investment or trading success. By contrast, many (though certainly not all) discretionary traders, because they are not forced to be so precise in the specification of their strategy and its implementation, seem to take a great many decisions in an ad hoc manner. I have been in countless meetings with discretionary traders who, when I asked them how they decided on the sizes of their positions, responded with variations on the theme of, “Whatever seemed reasonable.” This is by no means a damnation of discretionary investment styles. I merely point out that precision and deep thought about many details, in addition to the bigger-picture aspects of a strategy, can be a good thing, and this lesson can be learned from quants. 

## THE MEASUREMENT AND MISMEASUREMENT OF RISK

As mentioned earlier in this chapter, the history of LTCM is a lesson in the dangers of mismeasuring risk. Quants are naturally predisposed toward conducting all sorts of measurements, including of risk exposure. This activity itself has potential benefits and downsides. On the plus side, there is a certain intentionality of risk taking that a well-conceived quant strategy encourages. Rather than accepting accidental risks, the disciplined quant attempts to isolate exactly what his edge is and focus his risk taking on those areas that isolate this edge. To root out these risks, the quant must first have an idea of what these risk are and how measure them. For example, most quant equity traders, recognizing that they do not have sufficient capabilities in forecasting the direction of the market itself, measure their exposure to the market (using their net dollar or beta exposure, commonly) and actively seek to limit this exposure to a trivially small level by balancing their long portfolios against their short portfolios. On the other hand, there are very valid concerns about false precision, measurement error, and incorrect sets of assumptions that can plague attempts to measure risk and manage it quantitatively. 

All the blowups we have mentioned, and most of those we haven't, stem in one way or another from this overreliance on flawed risk measurement techniques. In the case of LTCM, for example, historical data showed that certain scenarios were likely, others unlikely, and still others had simply never occurred. At that time, most market participants did not expect that a country of Russia's importance, with a substantial supply of nuclear weapons and materials, would go bankrupt. Nothing like this had ever happened before. Nevertheless, Russia indeed defaulted on its debt in the summer of 1998, sending the world's markets into a frenzy and rendering useless any measurement of risk. The naïve overreliance on quantitative measures of risk, in this case, led to the near-collapse of the financial markets in the autumn of 1998. But for a rescue orchestrated by the U.S. government and agreed on by most of the powerhouse banks on Wall Street, we would have seen a very different path unfold for the capital markets and all aspects of financial life. 

Indeed, the credit debacle that began to overwhelm markets in 2007 and 2008, too, was likely avoidable. Banks relied on credit risk models that simply were unable to capture the risks correctly and in many cases seem to have done so knowingly, because it enabled them greedily to pursue outsized short-term profits (and, of course, bonuses for themselves). It should be said that most of these mismeasurements could have been avoided, or at least the resulting problems mitigated, by the application of better judgment on the part of the practitioners who relied on them. Just as one cannot justifiably blame weather-forecasting models for the way that New Orleans was impacted by Hurricane Katrina in 2005, it would not make sense to blame quantitative risk models for the failures of those who created and use them. Traders can benefit from engaging in the exercise of understanding and measuring risk, so long as they are not seduced into taking ill-advised actions as a result. 

## DISCIPLINED IMPLEMENTATION

Perhaps the most obvious lesson we can learn from quants comes from the discipline inherent to their approach. Upon designing and rigorously testing a strategy that makes economic sense and seems to “work,” a properly run quant shop simply tends to let the models run without unnecessary, arbitrary interference. In many areas of life, from sports to science, the human ability to extrapolate, infer, assume, create, and learn from the past is beneficial in the planning stages of an activity. But execution of the resulting plan is also critical, and it is here that humans frequently are found to be lacking. A significant driver of failure is a lack of discipline. 

Many successful traders subscribe to the old trading adage, “Cut losers and ride winners.” However, discretionary investors often find it very difficult to realize losses, whereas they are quick to realize gains. This is a well-documented behavioral bias known as the disposition effect. $^{8}$ Computers, however, are not subject to this bias. As a result, a trader who subscribes to the aforementioned adage can easily program his trading system to behave in accordance with it every time. This is not because the systematic trader is somehow a better person than the discretionary trader, but rather because the systematic trader is able to make this “rational” decision at a time when there is no pressure, thereby obviating the need to exercise discipline at a time when most people would find it extraordinarily challenging. Discretionary investors can learn something about discipline from those who make it their business. 

## SUMMARY

Quant traders are a diverse and large portion of the global investment universe. They are found in both large and small trading shops and traffic in multiple asset classes and geographical markets. As is obvious from the magnitude of success and failure that is possible in quant trading, this niche can also teach a great deal to any curious investor. Most traders would be well served to work with the same kind of thoroughness and rigor as is required to properly specify and implement a quant trading strategy. Just as useful is the quant's proclivity to measure risk and exposure to various market dynamics, though this activity must be undergone with great care to avoid its flaws. Finally, the discipline and consistency of implementation that exemplifies quant trading is something from which all decision makers can learn a great deal. 

# An Introduction to Quantitative Trading

You see, wire telegraph is a kind of a very, very long cat. You pull his tail in New York and his head is meowing in Los Angeles. Do you understand this? And radio operates exactly the same way: you send signals here, they receive them there. The only difference is that there is no cat. 

—Attributed to Albert Einstein, when asked to explain the radio 

The term black box conjures up images of a Rube Goldberg device wherein some simple input is rigorously tortured to arrive at a mysterious and distant output. Webster's Third New International Dictionary defines a Rube Goldberg device as "accomplishing by extremely complex roundabout means what actually or seemingly could be done simply." Many observers in both the press and industry use markedly similar verbiage to describe quants. One Washington Post article, "For Wall Street's Math Brains, Miscalculations; Complex Formulas Used by 'Quant' Funds Didn't Add Up in Market Downturn," contains the following definition: "... a quant fund is a hedge fund that relies on complex and sophisticated mathematical algorithms to search for anomalies and non-obvious patterns in the markets."¹ In the New York Post's "Not So Smart Now," we learn that "Quant funds run computer programs that buy and sell hundreds and sometimes thousands of stocks simultaneously based on complex mathematical ratios ..."² Perhaps most revealing, this view is held even by some of the world's best-respected investors. David Swensen, the renowned chief investment officer of the $17 billion Yale University endowment fund and author of Pioneering Portfolio Management, said in an interview with Fortune/CNN Money, "We also don't invest in quantitative-black box models because we simply don't know what they're doing."3 

The term black box itself has somewhat mysterious origins. From what I can tell, its first known use was in 1915 in a sci-fi serial called The Black Box, starring Herbert Rawlinson. The program was about a criminologist named Sanford Quest who invented devices (which themselves were placed inside a black box) to help him solve crimes. Universal Studios, which produced the serial, offered cash prizes to those who could guess the contents of the black box. $^{4}$ 

This connotation of opaqueness still persists today whenever the term black box is used. Most commonly in the sciences and in finance, a black box refers to any system that is fed inputs and produces outputs, but whose inner workings are either unknown or unknowable. Appropriately, two favorite descriptors for quant strategies are complex and secretive. However, by the end of this book I think it will be reasonably obvious to readers that, for the most part, quantitative trading strategies are in fact clear boxes that are far easier to understand in most respects than the caprice inherent to most human decision making. 

For example, an esoteric-sounding strategy called statistical arbitrage is in fact simple and easily understood. Statistical arbitrage is based on the theory that similar instruments (imagine two stocks, such as Exxon Mobil and Chevron) should behave similarly. If their relative prices diverge over the short run, they are likely to converge again. So long as the stocks are still similar, the divergence is more likely due to a short-term imbalance between the people buying and selling the instruments rather than any meaningful fundamental change that would warrant a divergence in prices. This is a clear and straightforward premise, and it drives billions of dollars' worth of trading volumes daily. It also happens to be a strategy that discretionary traders use, though it is usually called pairs trading. But whereas the discretionary trader is frequently unable to provide a curious investor with a consistent and coherent framework for determining when two instruments are similar or what constitutes a divergence, these are questions that the quant has likely researched and can address in great detail. 

## WHAT IS A QUANT?

A quant systematically applies an alpha-seeking investment strategy that was specified based on exhaustive research. What makes a quant a quant, in other words, almost always lies in how an investment strategy is conceived and implemented. It is rarely the case that quants are different from discretionary traders in what their strategies are actually doing, as illustrated by the earlier example of pairs trading and statistical arbitrage. There is almost never any attempt to eliminate human contributions to the investment process; after all, we are talking about quants, not robots. As previously mentioned, though quants apply a systematic approach to a wide variety of strategies, whether a fund designed to track the S&P 500 or to trade exotic options strategies, this book will remain focused on quants who pursue alpha, or returns that are independent of the direction of any market in the long run. 

Besides conceiving and researching the core investment strategy, humans also design and build the software and systems used to automate the implementation of their ideas. But once the system “goes live,” human judgment is generally limited in the day-to-day management of a portfolio. Still, the importance of human discretion in such a setup should not be understated. Good judgment is actually what separates the best quants from the mediocre. The kinds of issues listed in the stat arb example are just a small subset of the kinds of decisions that quants almost always have to make, and these fundamental decisions, above all else, drive the strategy’s behavior from that time forward. As such, good and bad judgments are multiplied over and over through time as the computer faithfully implements exactly what it was told to do. This is no different than many other fields. Imagine a guided missile system. If the engineers make bad judgments in the way they design these systems, there can be disastrous results, which are multiplied as more missiles are fired using the faulty guidance systems. 

To understand the systematic nature of quants better, it can be helpful to examine the frontiers of the systematic approach—in other words, the situations in which quants have to abandon a systematic approach for a discretionary one. When a quant intervenes with the execution of her strategy, it is most commonly to mitigate problems caused by information that drives market behavior but that cannot be processed by the model. For example, the 2008 merger between Merrill Lynch and Bank of America, which caused Merrill's price to skyrocket, might have led a naïve quant strategy to draw the conclusion that Merrill had suddenly become drastically overpriced relative to other banks and was therefore an attractive candidate to be sold short. But this conclusion would have been flawed because there was information that justified the spike in Merrill's price and would not seem to a reasonable person to lead to a short sale. As such, a human can step in and simply remove Merrill from the universe that the computer models see, thereby eliminating the risk that, in this case anyway, the model will make decisions based on bad information. In a sense, this is merely an application of the principle of "garbage in, garbage out." If a portfolio manager at a quant trading shop is concerned that the model is making trading decisions based on inaccurate, incomplete, or irrelevant information, she may decide to reduce risk by eliminating trading in the instruments affected by this information. 

Note that in this example, the news of the merger would already have been announced before the quant decides to override the system. Some shops are more aggressive, preemptively pulling names off the list of tradable securities at the first sign of credible rumors. By contrast, some quants do not remove names under any circumstances. Many quants reserve the right to reduce the overall size of the portfolio (and therefore leverage) if, in their discretion, the markets appear too risky. For example, after the attacks of September 11, 2001, many quants reduced their leverage in the wake of a massive event that would have unknowable repercussions on capital markets. Once things seemed to be operating more normally in the markets, they increased their leverage again to normal levels. 

Though the operating definition of quants at the beginning of this section is useful, there is a full spectrum between fully discretionary strategies and fully systematic (or fully automated) strategies. The key determination that puts quants on one side of this spectrum and everyone else on the other is whether daily decisions about the selection and sizing of portfolio positions are made systematically (allowing for the exceptions of “emergency” overrides such as those just described) or discretionarily. If both the question of what positions to own and how much of each to own are usually answered systematically, that’s a quant. If either one is answered by a human as standard operating procedure, that’s not a quant. 

It is interesting to note that, alongside the growth in quantitative trading, there are also a growing number of quasi-quant traders. For instance, some of these traders utilize automated systems to screen for potential investment opportunities, thereby winnowing a large number of potential choices down to a much smaller, more manageable list. From there, human discretion kicks in again, doing some amount of “fundamental” work to determine which names selected by the computer are actually worth owning and which are not. Less commonly, some traders leave the sourcing and selection of trades entirely up to humans, instead using computers to optimize and implement portfolios and to manage risk. Still more rarely, a few traders allow the computer to pick all the trades, while the human trader decides how to allocate among these trades. These quasi-quants make use of a subset of the tools in a proper quant’s toolbox, so we will cover their use of these techniques implicitly. 

## WHAT IS THE TYPICAL STRUCTURE OF A QUANTITATIVE TRADING SYSTEM?

The best way to understand both quants and their black boxes is to examine the components of a quant trading system; this is the structure we will use for the remainder of the book. Exhibit 2.1 shows a schematic of a typical quantitative trading system. This diagram portrays the components of a live, “production” trading strategy (e.g., the components that decide which securities to buy and sell, how much, and when) but does not include everything necessary to create the strategy in the first place (e.g., research tools for designing a trading system). 

The trading system has three modules—an alpha model, a risk model, and a transaction cost model—which feed into a portfolio construction model, which in turn interacts with the execution model. The alpha model is designed to predict the future of the instruments the quant wants to consider trading for the purpose of generating returns. For example, in a trend-following strategy in the futures markets, the alpha model is designed to forecast the direction of whatever futures markets the quant has decided to include in his strategy. 

Risk models, by contrast, are designed to help limit the amount of exposure the quant has to those factors that are unlikely to generate returns but could drive losses. For example, the trend follower could choose to limit his directional exposure to a given asset class, such as commodities, because of concerns that too many forecasts he follows could line up in the same direction, leading to excess risk; the risk model would contain the levels for these commodity exposure limits. 

The Transaction cost model, which is shown in the box to the right of the risk model in Exhibit 2.1, is used to help determine the cost of whatever trades are needed to migrate from the current portfolio to whatever new portfolio is desirable to the portfolio construction model. Almost any trading transaction costs money, whether the trader expects to profit greatly or a little from the trade. Staying with the example of the trend follower, if a trend is expected to be small and last only a short while, the transaction cost model might indicate that the cost of entering and exiting the trade is greater than the expected profits from the trend. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/148e0d39981734f0da7c9c9e17d6bf72990be0e2fca19e9065709ce956c3854a.jpg)



EXHIBIT 2.1 Basic Structure of a Quant Trading Strategy


The alpha, risk, and transaction cost models then feed into a portfolio construction model, which balances the tradeoffs presented by the pursuit of profits, the limiting of risk, and the costs associated with both, thereby determining the best portfolio to hold. Having made this determination, the system can compare the current portfolio to the new target portfolio, with the differences between the current portfolio and the target portfolio representing the trades that need to be executed. Exhibit 2.2 illustrates an example of this process. 

The current portfolio reflects the positions the quant trader currently owns. After running the portfolio construction model, the quant trader generates the new target portfolio weights, shown in the New Target Portfolio column. The difference between the two indicates the trades that now need to be executed, which is the job of the execution algorithm. The execution algorithm takes the required trades and, using various other inputs such as the urgency with which the trades need to be executed and the dynamics of the liquidity in the markets, executes trades in an efficient and low-cost manner. 

The structure shown in Exhibit 2.1 is by no means universal. For example, many quant strategies are run without a transaction cost model, a portfolio construction model, or an execution model. Others combine various components of these models. One can build whatever risk requirements and constraints considered necessary into the alpha model itself. Another variation is to create more recursive connections among the pieces. Some traders capture data about their actual executions and utilize these data to improve their transaction cost models. However, the diagram is useful because, for the most part, it captures the various discrete functions within a quant trading system, regardless of whether they are organized precisely in this manner. 


EXHIBIT 2.2 Moving from an Existing Portfolio to a New Target Portfolio


<table><tr><td></td><td>Current Portfolio</td><td>New Target Portfolio</td><td>Trades to Execute</td></tr><tr><td>S&amp;P500 Index</td><td>Short 30%</td><td>Short 25%</td><td>Buy to Cover 5%</td></tr><tr><td>EUROSTOXX Index</td><td>Long 20%</td><td>Long 25%</td><td>Buy 5%</td></tr><tr><td>U.S. 10-Year Treasury Notes</td><td>Long 40%</td><td>Long 25%</td><td>Sell 15%</td></tr><tr><td>German 10-Year Bunds</td><td>Short 10%</td><td>Short 25%</td><td>Sell Short 15%</td></tr></table>

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/f0eaeddba82a2ba64569f91d519ca58ca21a74eecdb4e7c380621c53798cb351.jpg)



EXHIBIT 2.3 The Black Box Revealed


Exhibit 2.1 captures only part of the work of the quant trader because it considers only the live production trading system and ignores two key pieces required to build it and run it: data and research. Black boxes are inert and useless without data—accurate data, moreover. Quant traders generally build input/output models that take inputs (data), make some calculations about these data, and then process trading decisions. For example, a trader utilizing a trend-following strategy usually requires price data to determine what the trend is. Without data he would have nothing to do, because he'd never be able to identify the trends he intends to follow. As such, data are the lifeblood of a quant and determine much about their strategies. Given data, quants can perform research, which usually involves some form of testing or simulation. Through research, the quant can ascertain whether and how a quant strategy works. We also note that each of the other modules in our schematic, when built correctly, usually requires a great deal of research. We can therefore redraw our diagram to include these other critical pieces, as shown in Exhibit 2.3. 

## SUMMARY

Quants are perhaps not so mysterious as is generally supposed. They tend to start with ideas that any reasonable observer of the markets might also have, but rather than using anecdotal, experiential evidence—or worse, simply assuming that these ideas are true—quants use market data to feed a research process to determine whether their ideas in fact hold true over time. Once they have arrived at a satisfactory strategy, they build their strategy into a quant system. These systems take the emotion out of investing and instead impose a disciplined implementation of the idea that was tested. But this should not be read as minimizing the importance of human beings in the quant trading process. They come up with ideas, test strategies, and decide which ones to use, what kinds of instruments to trade, at what speed, and so on. Humans also tend to control a “panic button,” which allows them to reduce risk if they determine that markets are behaving in some way that is outside the scope of their models’ capabilities. 

Quant strategies are widely ignored by investors as being opaque and incomprehensible. Even those who do focus on this niche tend to spend most of their time understanding the core of the strategy, its alpha model. But we contend that there are many other parts of the quant trading process that deserve to be understood and evaluated. Transaction cost models help determine the correct turnover rate for a strategy and risk models help keep the strategy from betting on the wrong exposures. Portfolio construction models balance the conflicting desires to generate returns, expend the right on transaction costs, manage risk, and deliver a target portfolio to execution models, which implement the portfolio model's decisions. All this activity is fed by data and driven by research. From afar, we have begun to shed light on the black box. 

Next, in Part Two, we will dissect each of these modules, making our way methodically through the inside of the black box. At the end of each of these chapters, as a reminder of the structure of a quant system and of our progress, we will indicate the topic just completed by removing the shading from it. 

Inside the Black Box 

# Alpha Models: How Quants Make Money

Prediction is very difficult, especially about the future.
—Niels Bohr 

Having surveyed it from the outside, we begin our journey through the black box by understanding the heart of the actual trading systems that quants use. This first piece of a quant trading system is its alpha model, which is the part of the model that is looking to make money and is where much of the research process is focused. Alpha, the spelled-out version of the Greek letter $\alpha$ , generally is used as a way to quantify the skill of an investor or the return she delivers independently of the moves in the broader market. By conventional definition, alpha is the portion of the investor's return not due to the market benchmark, or, in other words, the value added (or lost) solely because of the manager. For instance, if a manager is up 12 percent and her respective benchmark is up only 10 percent, a quick back-of-the-envelope analysis would show that her alpha, or value added, is +2 percent. This value added could be a result of luck, or it could be because of skill. Alpha models are therefore the quant's approach to adding skill to the investment process in order to make profits. For example, a trend-following trader's ability to identify trends that will persist into the future represents one type of skill that can generate profits. 

What is common to all pursuits of alpha is that they are in essence designed to time the selection and/or sizing of portfolio holdings. They hold as a core premise that no instrument is inherently good or bad, and therefore no instrument is worth always owning or perpetually ignoring. So again, the trend follower determines when to buy and sell various instruments, as does the value trader. Each of these is a type of alpha. In the first case, alpha is generated from the skill in identifying trends, which allows the trend follower to know when it is good to be long or short a given instrument. The instrument itself is neither good nor bad, neither always worth being long nor always warranting a short position. The key for the trend follower is to determine when to be long or short. Similarly, a value trader does not say that a given stock is cheap now and therefore is worth owning in perpetuity. In fact, if a stock is always cheap, it is almost certainly not worth owning, because its valuation never improves for the investor. Instead, the idea behind value investing is to buy a stock when it is undervalued and to sell it when it is fairly valued or overvalued. Again, this represents an effort to time the stock. 

The software that a quant builds and uses to conduct this timing is known as an alpha model, though there are many synonyms for this term: forecasts, factors, alphas, models, strategies, estimators, or predictors. All successful alpha models are designed to have some “edge,” which allows them to anticipate the future with enough accuracy that, after allowing for them being wrong at least sometimes and for the cost of trading, they can still make money. In a sense, of the various parts of a quant strategy, the alpha model is the optimist, focused on making money by predicting the future. 

To make money, generally some risk, or exposure, must be accepted. By utilizing a strategy, we directly run the risk of losing money when the environment for that strategy is adverse. For example, Warren Buffett has beaten the market over the long term, and this differential is a measure of his alpha. But there have been times when he struggled to add value, as he did during the dot-com bubble of the late 1990s. His strategy was out of favor, and his underperformance during this period reflected this fact. This chapter will address the kinds of alpha models (also known as exposures) that exist and the ways that quants actually use the forecasts their models make. 

## TYPES OF ALPHA MODELS: THEORY DRIVEN AND DATA DRIVEN

An important and not widely understood fact is that there are only a small number of trading strategies that exist for someone seeking alpha. But these basic strategies can be implemented in many ways, making it possible to create an incredible diversity of strategies from a limited set of core ideas. The first key to understanding quant trading strategies is to understand the perspectives quants take on science. 

Because most quants are trained first in the sciences and only later in finance, quants' scientific backgrounds frequently determine the approach they take to trading over their entire careers. The two major branches of science, which also serve as a helpful way to differentiate scientists, are theoretical and empirical. Theoretical scientists try to make sense of the world around them by hypothesizing why it is the way it is. This is the kind of science with which people are most familiar and interact most. For example, viable, controllable, long-distance airplanes exist largely because engineers apply theories of aerodynamics. Empirical scientists believe that enough observations of the world can allow them to predict future patterns of behavior, even if there is no hypothesis to rationalize the behavior in an intuitive way. In other words, knowledge comes from experience. The Human Genome Project is one of many important examples of the applications of empirical science, mapping human traits to the sequences of chemical base pairs that make up human DNA. 

The distinction between theoretical and empirical science is germane to quantitative trading in that there are also two kinds of quant traders. The first, and by far the more common, are theory driven. They start with observations of the markets, think of a generalized theory that could explain the observed behavior, then rigorously test it with market data to see if the theory is shown to be either untrue or supported by the outcome of the test. In quant trading, most of these theories are things that would make sense to you or me and that seem sensible when explained to friends at cocktail parties. For example, “cheap stocks outperform expensive stocks” is a theory that many people hold. This explains the existence of countless “value” funds. Once precisely defined, this theory can be tested. 

The second kind of scientist, by far in the minority, believes that correctly performed empirical observation and analysis of the data can obviate the need for theory. Such a scientist's theory, in short, is that there are recognizable patterns in the data that can be detected with careful application of the right techniques. Again, the example of the Human Genome Project is instructive. The scientists in the Human Genome Project did not believe that it was necessary to theorize what genes were responsible for particular human traits. Rather, scientists merely theorized that the relationships between genes and traits can be mapped using statistical techniques, and they proceeded to do exactly that. Empirical scientists are sometimes derisively (and sometimes just as a matter of fact) labeled data miners. They don't especially care if they can name their theories and instead attempt to use data analysis techniques to uncover behaviors in the market that aren't intuitively obvious. 

It is worthwhile to note that theory-driven scientists (and quants) are also reliant on observations (data) to derive theories in the first place. Just like the empiricists, they, too, believe that something one can observe in the data will be repeatable in the future. Empiricists, however, are less sensitive to whether their human minds can synthesize a “story” to explain the data even if, in the process, they risk finding relationships or patterns in the data that are entirely spurious. 

## THEORY-DRIVEN ALPHA MODELS

Most quants you will come across are theory driven. They start with some economically feasible explanation of why the markets behave in a certain way and test these theories to see whether they can be used to predict the future with any success. Many quants think that their theories are somewhat unique to them, which is part of why so many of them are so secretive. But this turns out, almost always, to be a delusion. Meanwhile, many outside the quant trading world believe that the kinds of strategies quants use are complex and based on complicated mathematical formulae. But this generally also turns out to be false. 

In fact—and in defiance of both the presumed need for secrecy and the claims that what quants do cannot be understood by those without doctoral degrees—most of what theory-driven quants do can be relatively easily fit into one of five categories of phenomena: trend, reversion, value/yield, growth, and quality. It is worth noting that the kinds of strategies that quants utilize are actually exactly the same as those that can be utilized by discretionary traders seeking alpha. These five categories can be further understood by examining the data that they use: price-related data and fundamental data. As we will see throughout this book, understanding the inputs to a strategy is extremely important to understanding the strategy itself. The first two categories of strategies, trend and mean reversion, are based on price-related data. The remaining three strategies, value/yield, growth, and quality, are based on fundamental data. 

Many successful quants utilize more than one type of alpha model in conjunction, but to gain a proper understanding of these strategies, we will first break them down individually and discuss the combining of them afterward. Exhibit 3.1 provides a summary and outline for understanding the types of alpha models that quants use. 

## Strategies Utilizing Price-Related Data

First we will focus on alpha models that utilize price-related data, which is mostly about the prices of various instruments or other information that generally comes from an exchange (such as trading volume). Quants who seek to forecast prices and to profit from such forecasts are likely to be exploiting one of two kinds of phenomena. The first is that an established trend will continue, and the second is that the trend will reverse. In other words, the price can either keep going in the direction it was going already, or it can go in the opposite direction. We call the first idea trend following or momentum, and we call the second idea counter-trend or mean reversion. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/1a7060a12fdc6c205a593b2635817312a791a6aca059efc51dc7b60fbeaad2aa.jpg)



EXHIBIT 3.1 A Taxonomy of Theory-Driven Alpha Models


Trend Following Trend following is based on the theory that markets sometimes move for long enough in a given direction that one can identify this trend and ride it. The economic rationale for the existence of trends is based on the idea of consensus-building among market participants. Imagine that there is uncertainty about the medium-term outlook for the U.S. economy. The labor picture looks fine, but inflation is running rampant and trade deficits are blooming. On the other hand, consumers are still spending and housing is strong. This conflicting information is a regular state of affairs for economies and markets so that some of the information available appears favorable and some unfavorable. In our example, let's further imagine that the bears have it right—that in fact inflation will get out of control and cause problems for the economy. The earliest adopters of this idea place their trades in accordance with it by, for example, selling bonds short. As more and more data come out to support their thesis and as a growing mass of market participants adopts the same thesis, the price of U.S. bonds may take a considerable amount of time to move to its new “equilibrium,” and this slow migration from one equilibrium to the next is the core opportunity that the trend follower looks to capture. 

It bears mentioning that there is an alternate explanation of why trends happen; it is affectionately known as the greater fools theory. The idea here is that, because people believe in trends, they tend to start buying anything that's been going up and selling anything that's been going down, which itself perpetuates the trend. The key is always to sell your position to someone more "foolish," and thereby to avoid being the last fool. Either theoretical explanation, coupled with the evidence in markets, seems a valid enough reason to believe in trends. 

Trend followers typically look for a “significant” move in a given direction in an instrument. They bet that, once a significant move has occurred, it will persist because this significant move is a likely sign of a growing consensus (or a parade of fools). There are many ways of defining what kind of move is significant, but the idea is the same regardless. Perhaps the most obvious and well-known example of a strategy that depends on trends is in the world of futures trading, or commodities trading advisors (CTAs). Exhibit 3.2 illustrates the downward trend in equities that began in the fourth quarter of 2007. One way to define a trend for trading purposes, known as a moving average crossover indicator, is to compare the average price of the index over a shorter time period (e.g., 60 days) to that of a longer time period (e.g., 200 days). When the shorter-term average price is below the longer-term average price, the index is said to be in a negative trend, and when the shorter-term average price is above the longer-term average, the index is in a positive trend. As such, a trend follower using this kind of strategy might have gotten short the S&P Index around the end of 2007, as indicated by the point at which the two moving averages cross over each other, and remained short for most or all of 2008. 


S&P 500 Index,
October 3, 2007–December 9, 2008


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/58390978788288f2ae4000cb48e1af6e3c113f6384cbd750b8ade50731848717.jpg)



EXHIBIT 3.2 S&P 500 Trend


Some of the largest quantitative asset managers engage in trend following in futures markets, which also happens to be the oldest of all quant trading strategies, as far as I can tell. Ed Seykota built the first computerized version of the mechanical trend-following strategy that Richard Donchian created some years earlier, utilizing punch cards on an IBM mainframe in 1970, a year after he graduated from MIT. He was a strong believer in doing ongoing research, and over the course his first 12 years, he turned $5000 into $15,000,000. He went on to a highly successful three-decades-long career, over which he annualized some 60 percent returns. $^{1}$ 

Larry Hite represents another interesting example of an early practitioner of trend following. Previously, Hite was a rock promoter in New York who, after experiencing three separate nightclub shootings on a single night, decided a change of career was in order. In 1972, he coauthored a paper that suggested how game theory could be used to trade the futures markets using quantitative systems. $^{2}$ After turning his attention to trend following, he created Mint Investments in 1981 with two partners; it became the first hedge fund to manage $1 billion and the first fund to partner with the Man Group, which effectively put Man into the hedge fund business. Mint annualized north of 30 percent per year, net of fees, for its investors over the 13 years it existed under Hite's stewardship. Notably, Mint made some 60 percent in 1987, in no small part by being on the right side of the crash that October. $^{3}$ 

Lest it seem like this is an overly rosy picture of trend following, it should be stated clearly: These strategies come with a great deal of risk alongside their lofty returns. The typical successful trend follower earns less than one point of return for every point of downside risk delivered. In other words, to earn 50 percent per year, the investor must be prepared to suffer a loss greater than 50 percent at some point. In short, the returns of this strategy are streaky and highly variable. 

This is not only true of trend following. Indeed, each of the major classes of alpha described in this chapter is subject to relatively long periods of poor returns. This is because the behaviors they seek to profit from in the markets are not ever-present but rather are unstable and episodic. The idea is to make enough money in the good times and manage the downside well enough in the bad times to make the whole exercise worthwhile. 

Perhaps quant trading's most important trend follower in terms of lasting impact was a firm called Axcom, which later became Renaissance Technologies. Elwyn Berlekamp, a Ph.D. in engineering from MIT, in 1986 began to consult for Axcom regarding strategy development. Axcom had been struggling during those years, and Berlekamp bought a controlling interest. In 1989, after doing considerable research, Axcom resumed trading with a new and improved strategy. For its first year, the firm was up 55 percent after charging 5 percent management fees and 20 percent incentive fees. At the end of 1990, Berlekamp sold his interest to Jim Simons for a sixfold profit, which might have been one of the worst trades in history. Renaissance, as the firm was called by then, is now the most successful quant trading firm and probably the most impressive trading firm of any kind. It has evolved a great deal from the trend-following strategies it used in the mid-1980s and even from the more sophisticated futures strategies it employed in the early 1990s. It stopped accepting new money with less than $300 million in 1992 and went on to compound this money to approximately $5.5 billion some 10 years later, despite eye-popping 5 percent management fees and 44 percent incentive fees. They have annualized approximately 35 percent per year net of these fees, from 1989 onward, and perhaps most astonishingly, have gotten better over the years, despite the increased competition in the space and the significantly larger capital base. $^{4}$ 

It is worth pointing out that quants are not the only ones who have a fondness for trend-following strategies. It has always been and will likely remain one of the more important ways in which traders of all stripes go about their business. One can find trend following in the roots of the infamous tulip mania of the Dutch in the seventeenth century, or in the dot-com bubble of the late twentieth century, neither of which is likely to have been caused by quants. And, of course, many discretionary traders have a strong preference to buy what's been "hot" and sell what's been "cold." 

Mean Reversion When prices move, as we have already said, they move in either the same direction they've been going or in the opposite. We have just described trend following, which bets on the former. Now we turn our attention to mean reversion strategies, which bet on prices moving in the opposite direction than that which had been the prevailing trend. 

The theory behind mean reversion strategies is that there exists a center of gravity around which prices fluctuate, and it is possible to identify both this center of gravity and what fluctuation is sufficient to warrant making a trade. The rationale behind this theory can be found in a few ways. First, there are sometimes short-term imbalances among buyers and sellers due simply to liquidity that leads to an instrument being “over-bought” or “oversold.” To return to the example mentioned earlier, imagine that a stock has been added to a well-followed index, such as the S&P 500. This forces any fund that is attempting to track the index to run out and buy the stock, and, in the short term, there might not be enough sellers at the old price to accommodate them. Therefore, the price moves up somewhat abruptly, which increases the probability that the price will reverse again at some point, when the excess demand from index buyers has subsided. Another rationale to explain the existence of mean-reverting behavior is that market participants are not all aware of each other's views and actions, and as they each place orders that drive a price toward its new equilibrium level, the price can overshoot due to excess supply or demand at any given time. Regardless of the cause of the short-term imbalance between supply and demand, mean reversion traders are frequently being paid to provide liquidity because they are bucking current trends and can therefore often buy on the bid and sell on the offer, thereby capturing the bid/ask spread. 

Interestingly, trend and mean reversion strategies are not necessarily at odds with each other. Longer-term trends can occur, even as smaller oscillations around these trends occur in the shorter term. In fact, some quants use both of these strategies in conjunction. Mean reversion traders must identify the current “mean” or “equilibrium” and then must determine what amount of divergence from that equilibrium is sufficient to warrant a trade. As in the case of trend following, there are a large number of ways of defining the “mean” and the reversal. It is worth noting that when discretionary traders implement mean reversion strategies, they are typically known as contrarians. 

Perhaps the best-known strategy based on the mean reversion concept is known as statistical arbitrage (stat arb, for short), which bets on the convergence of the prices of similar stocks whose prices have diverged. While Ed Thorp, founder of Princeton/Newport Partners was probably one of the earliest quantitative equity traders, the trading desk of Nunzio Tartaglia at Morgan Stanley was a pioneer of stat arb and would prove to have lasting impact on the world of finance. Tartaglia's team included scientists like Gerry Bamberger and David Shaw, and together they developed and evolved a strategy that was based on the relative prices of similar stocks. Stat arb ushered in an important change in world view, one that focused on whether company A was over- or undervalued relative to company B rather than whether company A was simply cheap or expensive in itself. This important evolution would lead to the creation of many strategies based on forecasts of relative attractiveness, which is a topic we will address in greater detail shortly. 

Exhibit 3.3 shows a simplified example of the mean-reverting behavior evident between similar instruments, in this case Merrill Lynch (MER) and Charles Schwab (SCHW). As you can see, the spread between these two companies oscillates rather consistently in a reasonably narrow range for long periods. This effect allows a trader to wait for significant divergences and then bet on a reversion back to the equilibrium level. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/519d97e4cdecabf3092a39417a697e6d34d40db6ba782d344d0d532d83f79975.jpg)



EXHIBIT 3.3 Mean Reversion Between SCHW and MER


Trend and mean reversion strategies represent a large portion of all quant trading. After all, price data are plentiful and always changing, presenting the quant with many opportunities to trade. It may be interesting to note that trend and mean reversion, though they are theoretically opposite ideas, both seem to work. How is this possible? Largely, it's possible because of different timeframes. It is obviously correct that both strategies can't possibly be made to be exactly opposite while both making money at the same time. However, there is no reason to create both strategies to be exactly the same. Trends tend to occur over longer time horizons, whereas reversions tend to happen over shorter-term time horizons. Exhibit 3.4 shows this effect in action. You can see that there are indeed longer-term trends and shorter-term mean reversions that take place. In fact, you can also see that the strategies are likely to work well at different times. From 2000 to 2002 and again in 2008, a trend strategy likely exhibits better performance, since the markets were trending very strongly during these periods. From 2003 to 2007, mean-reverting behavior was more prevalent. Yet both strategies are likely to have made money for the period as a whole. 

## Strategies Utilizing Fundamental Data

Most strategies utilizing fundamental data in their alpha models can be easily classified into one of three groups: value/yield, growth, or quality. 


Trend in the S&P 500 Index


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/9b89071d63c3289145c2692856104d8364e9163f5ec60942095d422680281868.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/60e3cd7852e5ddead1177a3d7291631d7af706d95cc1e94030f3f3d531f186e2.jpg)



EXHIBIT 3.4 Trend and Reversion Coexisting


Though these ideas are frequently associated with the analysis of equities, it turns out that one can apply the exact same logic to any kind of instrument. A bond, a currency, a commodity, an option, or a piece of real estate can be bought or sold because it offers attractive value, growth, or quality characteristics. While fundamentals have long been part of the discretionary trader's repertoire, quantitative fundamental strategies are relatively young. 

In quantitative equity trading and in some forms of quantitative futures or macro trading, much is owed to Eugene Fama and Kenneth French (known better collectively as Fama-French). In the early 1990s, they produced a series of papers that got quants thinking about kinds of factors that quants frequently use in strategies utilizing fundamental data. In particular, “The Cross Section of Expected Stock Returns” coalesced more than a decade of prior work in the area of using quantitative fundamental factors to predict stock prices and advanced the field dramatically. $^{5}$ Fama and French found, simply, that stocks’ betas to the market are not sufficient to explain the differences in the returns of various stocks. Rather, combining betas with historical data about the book-to-price ratio and the market capitalization of the stocks was a better determinant of future returns. 

It is somewhat ironic that an entire domain of quantitative alpha trading owes so much to Eugene Fama, because Fama's most famous work advanced the idea that markets are efficient. But if markets are in fact efficient, alpha should be impossible over the long haul. 

Value/Yield Value strategies are well known and are usually associated with equity trading, though such strategies can be used in other markets as well. There are many metrics that people use to describe value in various asset classes, but most of them end up being ratios of some fundamental factor versus the price of the instrument, such as the price-to-earnings (P/E) ratio. Quants tend to invert such ratios, keeping prices in the denominator. An inverted P/E ratio, or an E/P ratio, is also known as earnings yield. Note that investors traditionally already do this with dividends, hence the dividend yield, another commonly used measure of value. The basic concept of value strategies is that the higher the yield, the cheaper the instrument. The benefit of the conversion of ratios to yields is that it allows for much easier and more consistent analysis. 

Let's take earnings as an example: Earnings can (and frequently do) range from large negative numbers to large positive numbers and everywhere in between. If we take two stocks that are both priced at $20, but one has $1 of earnings while the other has $2 of earnings, it's easy to see that the first has a 20 P/E and the second has a 10 P/E, so the second looks cheaper on this metric. But imagine instead that the first has -$1 in earnings, whereas the second has -$2 in earnings. Now, these stocks have P/Es of -20 and -10, and -20 sounds worse than -10. But it's clearly better to only have $1 of negative earnings than $2. In the case that a company happens to have produced exactly $0 in earnings, the P/E ratio is simply undefined, since we would be dividing by $0. Because ratios with price in the numerator and some fundamental figure in the denominator exhibit of this sort of misbehavior, quants tend to use the inverted yield forms of these same ratios. This idea is demonstrated in Exhibit 3.5, which shows that the E/P ratio is well behaved for any level of earnings per share for a hypothetical stock with a price greater than $1 (in the example, we used $20 per share as the stock price). By contrast, the P/E ratio is rather poorly behaved and does not lend itself well to analysis and is not even properly defined when earnings per share are zero. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/88b48fd559c3c5df2f77b42dbd2fad47f7ebab216da65a2a1120b5e6b2f769a0.jpg)



EXHIBIT 3.5 P/E versus E/P ("Earnings Yield")


Most often, value is thought of as a strategy that is defined by “buying cheap.” But this strikes me as being too shallow a definition. In reality, the idea behind value investing is that markets tend to overestimate the risk in risky instruments and possibly to underestimate the risk in less risky ones. Therefore, it can pay off to own the more risky asset and/or sell the less risky asset. The argument for this theory is that sometimes instruments have a higher yield than is justified by their fundamentals simply because the market is requiring a high yield for that kind of instrument at the moment. An investor who can purchase this instrument while it has a high yield can profit from the movement over time to a more efficient, “fair” price. Ray Ball, a professor of accounting at the University of Chicago’s Booth School of Business, wrote a paper, Anomalies in Relationships Between Securities’ Yields and Yield-Surrogates, which echoes the idea that higher-yielding stocks—those with higher earnings yields—are likely those for which investors expect to receive higher returns and greater risks. $^{6}$ 

When done on a relative basis, that is, buying the undervalued security and selling the overvalued one against it, this strategy is also known as a carry trade. One receives a higher yield from the long position and finances this with the short position, on which a lower yield must be paid. The spread between the yield received and the yield paid is the carry. For instance, one could sell short $1,000,000 of U.S. bonds and use the proceeds to buy $1,000,000 of higher-yielding Mexican bonds. Graham and Dodd, in their landmark book Security Analysis, propose that value trading offers investors a margin of safety. In many respects, this margin of safety can be seen clearly in the concept of carry. If nothing else happens, a carry trade offers an investor a baseline rate of return, which acts as the margin of safety Graham and Dodd were talking about. 

Carry trading is an enormously popular kind of strategy for quants (and discretionary traders) in currencies, where the currency of a country with higher short-term yields is purchased against a short position in the currency of a country with relatively low short-term yields. For example, if the European Central Bank's target interest rate is set at 4.25 percent, whereas the U.S. Federal Reserve has set the Fed Funds rate at 2 percent, a carry trade would be to buy Euros against the U.S. dollar. This is a classic value trade because the net yield is 2.25 percent (4.25 percent gained on the Euro position, less 2 percent paid in U.S. interest), and this provides a margin of safety. If the trade doesn't work, the first 2.25 percent of the loss on it is eliminated by the positive carry. 

Another important example of value trading is in equities, where many kinds of traders seek to define metrics of “cheapness,” such as earnings before interest, taxes, depreciation, and amortization (EBITDA) versus enterprise value (EV) or book value to price. Book value per share versus price (book yield or book-to-price) is also a fairly common factor, as it has been among quants since Fama and French popularized it in their papers. Most quant equity traders who use value strategies are seeking relative value rather than simply making an assessment of whether a given stock is cheap or expensive. This strategy is commonly known as quant long/short (QLS). QLS traders tend to rank stocks according to their attractiveness based on various factors, such as value, and then buy the higher-ranked stocks while selling short the lower-ranked ones. For example, assume that we ranked the major integrated oil companies by the following hypothetical book-to-price ratios: 

<table><tr><td>Company</td><td>Book-to-Price Ratio (Hypothetical)</td></tr><tr><td>Marathon Oil (MRO)</td><td>95.2%</td></tr><tr><td>ConocoPhillips (COP)</td><td>91.7%</td></tr><tr><td>Chevron Corp. (CVX)</td><td>65.4%</td></tr><tr><td>Exxon Mobil Corp. (XOM)</td><td>33.9%</td></tr></table>

According to this metric, the higher-ranked stocks might be candidates for long positions, whereas the lower-ranked might be candidates for short positions. The presumption is that a stock with a higher book-to-price ratio might outperform stocks with lower book-to-price ratios over the coming quarters. 

Growth Growth strategies seek to make predictions based on the asset in question's expected or historically observed level of economic growth. Some examples of such ideas could be gross domestic product (GDP) growth or earnings growth. That a given stock is a growth asset implies nothing about its valuation or yield. The theory here is that, all else equal, it is better to buy assets that are experiencing rapid economic growth and/or to sell assets that are experiencing slow or negative growth. Some growth metrics, like the price/earnings-to-growth (PEG) ratio (PE ratio vs. EPS growth rate), are basically a forward-looking concept of value, that is, they compare growth expectations to value expectations to see whether a given instrument is fairly pricing in the positive or negative growth that the trader believes the asset will likely experience. If you expect an asset to grow rapidly but the market has already priced the asset to account for that growth, there is no growth trade to be made. In fact, if the market has priced in a great deal more growth than you expect, it might even be reasonable to short the instrument. But certainly many forms of growth trading are simply focused on buying rapidly growing assets regardless of price and selling assets with stagnant or negative growth, even if they are very cheap (or offer high yields) already. 

The justification for growth investing is that growth is typically experienced in a trending manner, and the strongest growers are typically becoming more dominant relative to their competitors. In the case of a company, you could see the case being made that a strong grower is quite likely to be in the process of winning market share from its weaker-growing competitors. Growth investors try to be early in the process of identifying growth and, hence, early in capturing the implied increase in the future stature of a company. We can see examples of both macroeconomic growth strategies and microeconomic growth strategies in the quant trading world. At the macro level, some foreign exchange trading concepts are predicated on the idea that it is good to be long currencies of countries that are experiencing relatively strong growth, because it is likely that these will have higher relative interest rates in the future than weaker-growth or recession economies, which makes this a sort of forward-looking carry trade. 

In the quant equity world, the QLS community frequently also utilizes signals relating to growth to help diversify their alpha models. Note that an important variant of growth trading utilized by a wide variety of quant and discretionary equity traders focuses on analysts' earnings estimate revisions. 

Sell-side analysts working at various brokerage houses publish their estimates and release occasional reports about the companies they cover. The thesis is identical to any other growth strategy, but the idea is to try to get an early glimpse of a company's growth by using the analysts' expectations rather than simply waiting for the company itself to report its official earnings results. Because this strategy depends on the views of market analysts or economists, it is called a sentiment-based strategy (as opposed to fundamental strategies that use official releases by corporations or governments). The quant community does not universally agree that sentiment-based strategies, such as the estimate revision idea just mentioned, are nothing more than variants of growth strategies, but it is my experience that these two are highly enough correlated in practice to warrant their being treated as close cousins. After all, too often Wall Street analysts' future estimates of growth look a lot like extrapolations of recent historical growth. 

Quality The final kind of theory-driven fundamental alpha is what I call quality. A quality investor believes that, all else being equal, it is better to own instruments that are of high quality and better to sell or be short instruments of poor quality. The justification for this strategy is that capital safety is important, and neither growth nor value strategies really capture this concept. A strategy focused on owning higher-quality instruments may help protect an investor, particularly in a stressful market environment. Not co- incidentally, these are frequently termed flight-to-quality environments. This kind of strategy is easily found in quant equity trading but not as commonly in macroeconomic types of quant trading, for reasons that are unknown to me. A typical kind of QLS signal focused on quality might look at the debt-to-equity ratios of stocks to help determine which ones to buy, the idea being that less-leveraged companies are considered higher quality than more-leveraged companies, all else equal. Another example is an earnings quality signal, which attempts to measure how close are a company's true economic earnings (as measured by, say, the free cash flow) to the reported earnings-per-share numbers. Such strategies especially gained prominence in the wake of the accounting scandals of 2001 and 2002 (Enron and WorldCom, for example), which highlighted that sometimes publicly traded companies are run by folks who are trying harder manage their financial statements than manage their companies. Some quality signals focus on the diversification of a company's sources of earnings (or of the drivers of GDP growth for an economy), with the idea being that higher-quality companies will have more diversified earnings sources. Recently, quality has been a particularly important issue, and a particularly successful factor, in predicting the relative prices of banking stocks, probably because of the credit crisis-roiled markets in 2008. In particular, some quality factors helped traders detect, avoid, and/or sell short those banks with the most leverage or the most exposure to mortgage-related businesses, thereby allowing these traders to avoid or even profit from the 2008 credit crisis. 

We now have a summary of the ways that theory-driven, alpha-focused traders (including quants) can make money. To recap, price information can be used for trend or mean reversion strategies, whereas fundamental information can be used for yield (better known as value), growth, or quality strategies. This is a useful framework for understanding quant strategies but also for understanding all alpha-seeking trading strategies. The framework proposed herein provides a menu of sorts, from which we can ascertain which items have been ordered by a particular quant in creating his strategy. It is also useful framework for quants themselves and can help them rationalize and group the signals they use into families. Sometimes quants can even fool themselves into thinking that there are a broader array of core alpha concepts than there really are. 

## DATA-DRIVEN ALPHA MODELS

We now turn our attention to data-driven strategies, which were not included in the taxonomy shown in Exhibit 3.1. These strategies are far less widely practiced for a variety of reasons, one of which is that they are significantly more difficult to understand and the mathematics are far more complicated. Data mining, when done well, is based on the premise that the data tell you what is likely to happen next, based on some patterns that are recognizable using certain analytical techniques. When used as alpha models, the inputs are usually sourced from exchanges (mostly prices), and these strategies typically seek to identify patterns that have some explanatory power about the future. 

There are two advantages to these approaches. First, compared with theory-driven strategies, data mining is considerably more technically challenging and far less widely practiced. This means that there are fewer competitors, which is helpful. Because theory-driven strategies are usually easy to understand and the math involved in building the relevant models is usually not very advanced, the barriers to entry are naturally lower. Neither condition exists in the case of data-driven strategies, which discourages entry into this space. Second, data-driven strategies are able to discern behaviors whether they have been already named under the banner of some theory or not, which allows them to discover that something happens without having to understand why. By contrast, theory-driven strategies capture the kinds of behavior that humans have identified and named already, which may limit them to the five categories described earlier in this section. 

For example, many high-frequency traders favor an entirely empirical, data-mining approach when designing their short-term trading strategies for equity, futures and foreign exchange markets. These data-mining strategies may be more successful in high frequency because, if designed well, they are able to discern how the market behaves without having to worry about the economic theory or rationalization behind this behavior. Since there is not much good literature at this time about the theoretical underpinnings of human and computerized trading behaviors at very short-term time horizons (i.e., minutes or less), an empirical approach may actually be able to outperform a theoretical approach at this timescale. Furthermore, at this timescale there is so much more data to work with that the empirical researcher has a better chance of finding statistically significant results in his testing. 

However, data-mining strategies also have many shortcomings. The researcher must decide what data to feed the model. If he allows the model to use data that have little or no connection to what he is trying to forecast—for example, the historical phases of the moon for every day over the past 50 years—he may find results that are seemingly significant but are in reality entirely spurious. Furthermore, if the researcher chooses the set of all data generally thought to be useful in predicting markets, the amount of searching the algorithms must conduct is so enormous as to be entirely impractical. To run a relatively thorough searching algorithm over, say, two years of intraday tick data, with a handful of inputs, might take a single computer processor about three months of continuous processing before it finds the combinations of data that have predictive power. If this was not difficult enough, whatever strategies are found in this manner require the past to look at least reasonably like the future, although the future doesn't tend to cooperate with this plan very often or for very long. To adjust for this problem, the data-mining strategy requires nearly constant adjustment to keep up with the changes going on in markets, an activity that has many risks in itself. 

A second problem is that generating alphas using solely data-mining algorithms is a somewhat dubious exercise. The inputs are noisy, containing a great number of false signals that act like traps for data miners. In general, strategies that use data-mining techniques to forecast markets do not work, though there are a few exceptions. It is worth noting that the strategies employed by most successful data miners end up looking a lot like trending or reverting strategies. 

## IMPLEMENTING THE STRATEGIES

There are not many ways for alpha-focused traders to make money, whether they are quants or not. But the limited selection of sources of alpha does not imply that all quants choose one of a handful of phenomena and then have a peer group to which they are substantively identical. There is in fact considerable diversity among alpha traders, far more so than may be evident at first glance. 

This diversity stems from the way quants implement their strategies, and it is to this subject that we now turn our attention. There are many characteristics of an implementation approach that bear discussion, including the forecast target, time horizon, bet structure, investment universe, model specification, and run frequency. 

## Forecast Target

The first key component of implementation is to understand exactly what the model is trying to forecast. Models can forecast the direction, magnitude, and/or duration of a move and furthermore can include an assignment of confidence or probability for their forecasts. Many models forecast direction only, most notably the majority of trend-following strategies in futures markets. They seek to predict whether an asset price will rise or fall, and nothing more. Still others have specific forecasts of the size of a move, either in the form of an expected return or a price target. Some models, though they are far less common, also seek to identify how long a move might take. If the forecasted behavior is not exhibited within the defined time window, the trade is considered a failure and is exited. 

Finally, the signal strength is an important (but not ubiquitous) aspect of the quant model. Signal strength is defined by a larger expected return and/or by a higher likelihood of a return. The larger the expected return (i.e., the further the price target is from the current price), the greater the strength of the signal, holding confidence levels constant. Similarly, the more confidence in a signal, the greater the signal strength, holding expected returns constant. In general, though certainly not always, a higher level of signal strength results in a bigger bet being taken on a position. This is only rational. Imagine that you believe two stocks, Exxon Mobil (XOM) and Chevron (CVX), both will go up, but you have either a higher degree of confidence or a larger expected return in the forecast for XOM. It stands to reason that you will generally be willing to take a bigger bet on XOM than on CVX because XOM offers a more certain and/or larger potential return. The same holds for quant models, which generally give greater credence to a forecast made with a relatively high degree of confidence or large expected return. 

## Time Horizon

The next key component to understanding implementation of the alpha model is time horizon. Some quant models try to forecast literally microseconds into the future; others attempt to predict behavior a year or more ahead. Most quant strategies have forecast horizons that fall in the range of a few days to several months. Notably, a strategy applied to the very short term can look quite different than it would if the exact same idea was applied to the very long term, as illustrated by Exhibit 3.6. As you can see, a “medium-term” version of the moving-average-based following strategy would have been short the S&P 500 index during the entirety of April and May 2008 because of the downtrend in the markets that began in October 2007. By contrast, as shown in the lower graph in Exhibit 3.6, a shorter-term version of the same strategy would have been long on the S&P for all but three days in mid-April and for the last days of May. This exhibit illustrates that the same strategy, applied over different time horizons, can produce markedly different—even opposite—positions. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/380a1fb725e858e1427c80229ea837a48abaf1581319730901329f892cd67aa1.jpg)



EXHIBIT 3.6 Same Strategy on Different Time Horizons


In general, there is more variability between the returns of a one-minute strategy and a one-hour strategy than between a three-month and a six-month strategy, even though the interval between the latter pair is significantly longer than that between the first pair. This general rule especially holds true in more risky environments. This happens because the shorter-term strategies are making very large numbers of trades compared to the longer-term versions of the same strategies. Even a small difference in the time horizon of a strategy, when it is being run at a short time scale, can be amplified across tens of thousands of trades per day and in the millions per year. By contrast, three- and six-month versions of the same strategy are simply making a lot fewer trades, so the difference in time horizon does not get amplified. So, for example, a 150-day moving average versus a 300-day moving average trend-following strategy would produce the exact same constant short position in the S&P 500 during April and May as the trend-following strategy that uses 60- and 100-day moving averages. By contrast, taking merely 10 days off of the longer moving average from the shorter-term system so that it now uses 5- and 10-day moving averages causes the system to be short the S&P for several extra days in mid-April and to add another short trade in mid-May that the 5-/20-day version would not have done. Instead of being short the S&P for eight trading days out of the total of 43 during these two months, the 5-/10-day version would be short for 15 out of the 43 days. 

The choice of time horizon is made from a spectrum with a literally infinite number of choices, that is, forecasts can be made for two weeks into the future, or for two weeks and 30 seconds, or for two weeks and 31 seconds, and so on. Yet adding 30 or 31 seconds to a forecast of two weeks might not cause a great deal of differentiation. Along this line of thinking, a classification may be helpful in understanding the distinctions among quant trading strategies by time horizon. High-frequency strategies are the fastest, making forecasts that go no further than the end of the current trading day. Short-term strategies, the second category, tend to hold positions from one day to two weeks. Medium-term strategies make forecasts anywhere from a few weeks to a few months ahead. Finally, long-term strategies hold positions for several months or longer. The lines of demarcation between these groups are not firm, but this shorthand can be helpful in thinking about how various quant strategies might compare with one another. 

## Bet Structure

The next key component of an alpha model is bet structure, which, in turn, is based on how the alpha model generates its forecast. Models can be made to forecast either an instrument in itself or an instrument relative to others. For example, a model could forecast that gold is cheap and its price is likely to rise or that gold is cheap relative to silver, and that gold is therefore likely to outperform silver. When looking at relative forecasts, one can forecast the behavior of smaller clusters (e.g., pairs) or larger clusters (e.g., sectors). Smaller clusters have the advantage of being easier to understand and analyze. In particular, pairs are primarily attractive because, in theory, one can carefully select instruments that are directly comparable. 

However, pairs have several comparative disadvantages. Very few assets can actually be compared so precisely and directly with one other instrument, rendering a major benefit of pairs trading impracticable. Two Internet companies might each depend significantly on revenues from their respective search engines, but they may differ along other lines. One could have more of a content-driven business while the other uses advertising to supplement the search engine revenues. Meanwhile, one could find other companies with strong advertising or content businesses, each of which shares some characteristics and sector-effects with the first pair. Here the trader is presented with a dilemma: which pairs are actually the best to use? Or to put it another way, how should the trader's pairs best be structured? 

Another approach is to make bets based on larger clusters or groups. Researchers group securities together primarily in an effort to isolate and eliminate common effects among the group. A large part of the point of grouping stocks within their market sector, for example, is to eliminate the impact of a general movement of the sector and thereby focus on the relative movement of stocks within the sector. It turns out to be extremely difficult to isolate group effects with a group size of merely two. On the other hand, larger clusters allow for a cleaner distinction between group behavior and idiosyncratic behavior, which is beneficial for many quant strategies. As a result, most quants who trade in groups tend to use larger groups than simply pairs when they make relative bets. 

Researchers also must choose how they create these clusters, either using statistical techniques or using heuristics (e.g., fundamentally defined industry groups). There are many statistical techniques aimed at discerning when things are similar to each other or when they belong together as a group. However, statistical models can be fooled by the data, leading to bad groupings. For example, there may be periods during which the prices of Internet stocks behave like the price of corn. This may cause the statistical model to group them together, but Internet stocks and corn are ultimately more different than they are similar, and most fundamental grouping approaches would never put them together. Furthermore, any time that the market regime changes, the relationships among instruments frequently also change, which can lead the system to mistakenly group things together that no longer will behave like each other. 

Alternatively, groups can be defined heuristically. Asset classes, sectors, and industries are common examples of heuristically defined groups. They have the advantage of making sense and being defensible theoretically, but they are also imprecise (for instance, to what industry does a conglomerate such as General Electric belong?) and possibly too rigid. Rigidity in particular can be a problem because over time, similarities among instruments change. Sometimes stocks and bonds move in opposite directions, and sometimes they move in the same direction. Because the correlation between these two asset classes moves in phases, it can be very tricky to analyze the relationship theoretically and make a static, unchanging declaration that they belong in the same group or in different groups. As a result, most grouping techniques (and by extension, most strategies that are based on relative forecasts), whether statistically driven or human-made, suffer from changes in market regime that cause drastic changes in the relationships among instruments. 

In evaluating alpha-oriented strategies, this distinction among bet structures, most notably between intrinsic (single security) bets versus relative (multi-security) bets, is rather important. The behavior of a given type of alpha model is very different if it is implemented on an instrument by itself than it would be if implemented on a group of instruments relative to each other. It is critical to balance the risks and benefits of the various approaches to grouping. In general, relative alpha strategies tend to exhibit smoother returns during normal times than intrinsic alpha strategies, but they can also experience unique problems related to incorrect groupings during stressful periods. Some quants attempt to mitigate the problems associated with any particular grouping technique by utilizing several grouping techniques in concert. For example, one could first group stocks by their sectors but then refine these groupings using a more dynamic statistical approach that reflects recent correlations among the stocks. 

Also, it is worth clarifying one piece of particularly unhelpful, but widely used, hedge fund industry jargon: relative value. This term refers to strategies that utilize a relative bet structure, but the value part of the term is actually not useful. Certainly strategies that make forecasts based on a notion of the relative valuation of instruments are quite common. However, most strategies called relative value have little to do with value investing. Relative mean reversion strategies, relative momentum strategies, and other kinds of relative fundamental strategies are all commonly referred to as relative value. 

## Investment Universe

A given strategy can be implemented in a variety of instruments, and the quant must choose which ones to include or exclude. The first significant choice a quant makes about the investment universe is geography. A short-term relative mean reversion strategy traded on stocks in the United States might not behave similarly to the same strategy applied to stocks in Hong Kong. The researcher must decide where to apply the strategy. The second significant choice a quant makes about the investment universe relates to its asset class. A growth strategy applied to foreign exchange markets might behave differently than one applied to equity indices. The quant must decide what asset classes to trade with each strategy. A third significant choice a quant must make about the investment universe relates to the instrument class. Equity indices, as accessed through the futures markets, behave differently than single stocks, even though both belong to the equity asset class. Also, the liquidity characteristics and nature of the other participants in a given market differ from one instrument class to another, and these are some of the considerations quants must make regarding what kinds of instruments to trade. Finally, in some cases, quants may include or exclude specific groups of instruments for a variety of reasons. 

The choice of an investment universe is dependent on several strong preferences that quants tend to have. First, the quant generally prefers liquidity in the underlying instruments so that estimations of transactions costs are reliable. Second, quants generally require large quantities of high-quality data. In general, such data can be found in highly liquid and developed markets. Third, quants tend to prefer instruments that behave in a manner conducive to being predicted by systematic models. Returning to the example of biotechnology stocks, some quants exclude them because they are subject to sudden, violent price changes based on events such as government approval or rejection of their latest drug. Although physician with a biotech specialization may have some intuitions on this subject, it's simply not something that most quants can model. As a result of these preferences, the most typical asset classes and instruments in which one can find quants participating are common stocks, futures (especially on bonds and equity indices), and foreign exchange markets. Some strategies might trade the fixed income asset class using instruments other than futures (e.g., swaps or cash bonds), though these are significantly less common today than they were in the middle or late 1990s. Geographically, the bulk of quant trading occurs in the United States, developed Europe, and Japan, with lesser amounts done in other parts of North America and developed Asia. Quants are almost completely absent from illiquid instruments, or those traded “over the counter” (OTC), such as corporate or convertible bonds, and are rarely found in emerging markets. 

This last fact may change going forward as OTC markets become better regulated and electronic. But that also implies that the liquidity of these markets will improve. As such, this notion of liquidity is perhaps the simplest way to summarize in one dimension the salient characteristics of the trading universe for a strategy. After all, more liquid instruments also tend to offer more high-quality data and to be more conducive to being forecast, on average. 

## Model Specification

It is all well and good to come up with an idea for a trading strategy, but the quant must specifically define every aspect of the strategy before it is usable. Furthermore, any differences in the way a quant chooses to specify or define an idea for her strategy might lead it to behave quite differently than other choices would have. For example, there could be multiple ways to define a trend. Some simply compute the total return of an instrument over some historical period, and if that number is positive, a positive trend is identified (a negative return would constitute a negative trend). Other trend traders use moving average approaches, such as the ones illustrated in Exhibits 3.1, 3.3, and 3.4, to look for prices to rise above or below recent average prices and so determine the presence of a trend. Still other trend strategies seek to identify the breakout of the very early stages of a trend, found using specific price patterns they believe are present in this critical phase, but they do not attempt to determine whether a long-term trend is actually in place or not. 

These are but a few of the more common ways a trend can be defined. Just so, each kind of alpha strategy can be defined in various ways, and it is a significant part of the quant's job to decide precisely how to specify the strategy mathematically. This is an area for an investor in quant trading to study carefully because it is often a source of differentiation—and potentially of comparative advantage—for a quant. In the “Time Horizon” section of this chapter, we saw that even a specification about the time horizon of a strategy for timing the stock market can have dramatic impact on whether it is long or short at a given point in time. Given the importance of time horizon, it is easy to understand the impact of using an entirely different definition of the strategy on its behavior. However, it may be challenging to get a quant to share with an outsider details on exactly how his model is specified. For the nonquant, then, model specification may remain a more opaque aspect of the black box, but exploring this idea as much as possible with a quant trader could, in fact, highlight the reasons for differences in performance that are observed versus the quant's peer group. 

The specification of the details of a model is also an area in which some quants utilize machine learning or data-mining techniques. In the section "Data-Driven Alpha Models," we mentioned the idea of fitting models to the data and setting parameter values. This is a problem to which machine learning techniques, which I described earlier as being neither easily nor commonly applied to the problem of finding alpha, are better suited and more widely used. In essence, machine learning techniques are applied to determine the optimal set of specifications for a quant model. Machine learning algorithms are designed to provide an intelligent and scientifically valid way of testing many potential sets of specifications without overfitting. 

A subset of the problem of specifying a model relates to how often the models themselves are adjusted for more recent data. This process is known as refitting because some of the same work that goes on in the original research process is repeated in live trading in an attempt to refresh the model and make it as adaptive as possible to current market conditions. Because this can be a computationally intensive process, sometimes involving millions or even billions of calculations, many quants refit their models infrequently or not at all. Refitting also leads to a greater risk of overfitting, a very treacherous problem indeed, since spurious and fleeting relationships may be mistaken for valid, lasting ones. 

## Run Frequency

A final component of building a given alpha model is determining the run frequency, or the frequency with which the model is actually run to seek new trading ideas. Some quants run their models relatively infrequently—for example, once per month. At the other extreme, some run their models more or less continuously, in real time. There is an interesting tradeoff that quants must manage here. Specifically, increasing the frequency of model runs usually leads to a greater number of transactions, which means more commissions paid to brokers and higher transaction costs. Also, more frequent model runs lead to a greater probability that the model is moving the portfolio around based on noisy data that doesn't actually mean that much. This, in turn, would mean that the increased transaction costs would cause little or no incremental improvement in the alpha generated by the strategy and would thereby reduce its overall profitability. 

On the other hand, less frequent model runs lead to a smaller number of larger-sized trades. These are expensive in a different way, namely in terms of the impact these trades can have on the marketplace. If models are run too infrequently, then at those times when they are run they could want to make very significant changes to the currently held portfolio. This would mean transacting larger blocks of trades, which would likely cost more in terms of "moving the market." Less frequent model runs are also prone to problems associated with the moment of observation of markets. If a strategy is run once a month, it could miss opportunities to trade at more favorable prices that occur during the month while the model is dormant. Alternatively, the model may attempt in vain to trade at attractive, but quickly fleeting, prices that occur if there has been some aberration just around the time of the model being run. Whether more frequent or less frequent model runs are better depends on many other aspects of the strategy, most especially the time horizon of the forecast and the kinds of inputs. In the end, most quants run their models no less than once a week, and many run continuously throughout the day. The slower-moving the strategy, obviously, the more leeway there is, whereas shorter-term strategies tend toward continuous, real-time runs. 

## An Explosion of Diversity

We have described a few of the kinds of important decisions that quants must make in building a given alpha model. To succeed in quant trading, each of these decisions requires good judgment on the part of the quant. In short, successful quants are characterized in part by an incredible attention to detail and tirelessness in seeking the right questions to ask and the best solutions to address them. Nevertheless, for those who do not build quant trading systems but who are interested in understanding them, the kinds of issues discussed in this section are straightforward to understand and provide a useful way to distinguish one quant from another. 

A final, important implication of these details of implementation is that they lead to an explosion in the variety of quant trading strategies that actually exist. You can easily see that the number of permutations of a strategy focused on the concept of “value,” for example, is enormous when accounting for differences in the type, time horizon, bet structure, investable universe, specification, and frequency of model run. Just taking the first four types of implementation details listed here and using the simplifying categories we described in this section, there are two types of forecasts (direction and magnitude), four types of time horizon (high frequency, short term, medium term, and long term), two types of bet structures (intrinsic and relative), and four asset classes (stocks, bonds, currencies, and commodities). Therefore one could build 64 different value models $2 \times 4 \times 2 \times 4 = 64$ permutations), and this excludes the question of how many ways one can define the idea of value and how often one can look for value. This number might seem daunting at first glance, but the framework established here can help anyone interested in understanding what's inside a black box. Exhibit 3.7 revisits the taxonomy of alpha models, expanding it to include the implementation approaches discussed here. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/01339c0e11cb4538bd0406d068356d28168c118b13ee564087cf5fecbd094599.jpg)



EXHIBIT 3.7 Taxonomy of Theory-Driven Alpha Models


## BLENDING ALPHA MODELS

Each of the decisions a quant makes in defining a trading strategy is an important driver of its behavior. But there is another extremely important set of choices the quant must make in constructing a trading strategy. Specifically, the quant is not limited to choosing just one approach to a given alpha model. Instead, he is equally free to choose to employ multiple types of alpha models. Even the method used to combine these alpha models is an arena rich with possibilities. The most sophisticated and successful quants tend to utilize several kinds of alpha strategies, including trend and reversion, and various kinds of fundamental approaches across a variety of time horizons, trade structures, instruments, and geographies. Such quants benefit from alpha diversification in exactly the same way that diversification is helpful in so many other aspects of financial life. 

Blending or mixing alpha signals has many analogues in discretionary trading (and decision making) in general. Imagine a mutual fund portfolio manager who has two analysts covering XOM. One analyst, focused on fundamental value in the classic Graham and Dodd sense, expects XOM to rise by 50 percent over the next year. The other analyst, taking a momentum approach, thinks XOM is likely to be flat over the next year. What is the net expectation the portfolio manager should have of the price of XOM, given the two analysts' predictions? This is the core problem that is addressed by blending alpha models, each of which can be likened to an analyst. 

The three most common quant approaches to blending forecasts are via linear models, nonlinear models, and machine learning models. There is also a significant fourth school of thought that believes that alpha models should not be combined at all. Instead, several portfolios are constructed, each based on the output from a given alpha model. These factor portfolios are then combined using any of the portfolio construction techniques discussed in Chapter 7. 

Each of these four approaches to signal mixing has its disciples, and as with most everything else we've discussed, the best way to blend alphas depends on the model. In general, as in the case of an alpha model, the purpose of a method of mixing alpha models is to find the combination of them that best predicts the future. All other things being equal, it is very likely that any reasonably intelligent combination of alphas will do a better job together than any one of them could do individually over time. Consider Exhibit 3.8. Here we can see that Forecasts A and B each occasionally predicts future events correctly. This is illustrated in that there is some overlap between Forecast A and the actual outcome and between Forecast B and the actual outcome. But each forecast has only a small amount of success in predicting the future. However, together, Forecasts A and B are about twice as likely to be correct about the future outcomes as either is separately. 

Linear models are by far the most common way in which quants combine alpha factors to construct a composite forecast. A linear model is a reasonable facsimile for one of the more common ways that humans normally think about cause-and-effect relationships. In linear models, the inclusion of one factor is independent of the inclusion of other factors, and each factor is expected to be additive, independently of the other factors that might be included or excluded. For example, for a high school student trying to get into a good university, she can think of her grades, standardized test scores, extracurricular activities, recommendations, and essays as being these independent factors in the linear model that predicts her odds of gaining admission. Regardless of the other factors, grades are always important, as is each other factor. As such, a linear model is relevant. If, on the other hand, it was the case that, with high enough test scores, her essays wouldn't matter, a linear model is no longer the correct way to predict her chances of getting in. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/7a1a0027aede84d0cdd96fc41cd4776d84a1a925391f40096f8ee8d2cf9c4453.jpg)



EXHIBIT 3.8 A Visualization of Multiple Forecasts


The first step in using a linear model in this way is to assign a weight to each alpha factor. To return to our example, if we were trying to predict university admissions, this step would require us to define the relative importance of grades versus, say, test scores. This is typically done using a technique known as multiple regression, which is aimed at finding the combination of alpha factors that explains the maximum amount of the historical behavior of the instruments being traded. The presumption is that, if a model reasonably explains the past, it has a reasonable chance of explaining the future well enough to make a profit. These weights are then applied to the outputs of their respective alpha factors, which are usually a forecast or score of some kind. The weighted sum of these multiple forecasts gives us a combined forecast. Or, to be more specific, by summing the products of the weights of each factor and the outputs of each factor, we arrive at a composite forecast or score. This composite can then be used to help determine the target portfolio. 

Imagine a trading system with two alpha factors. One of the alpha factors focuses on E/P ratios (and is therefore a yield model), and the other focuses on price trends (and is therefore a trend model). The yield factor forecasts a return of +20 percent over the next 12 months for XOM, whereas the trend factor forecasts a return of -10 percent for XOM over the next 12 months. Based on a historical regression, the models are weighted 70 percent toward the yield factor and 30 percent toward the trend factor. Taking their scores and weights together, the total 12-month return forecast of our two-factor model is computed as follows: 

70% weight × 20% return forecast for the yield factor comes to +14%. 

30% weight × -10% return forecast for the trend factor comes to -3%. 

The sum of these two products comes to +11 percent, which is the total expected 12-month return for XOM using the example above. 

A special case of linear models is the equal-weighted model. Though not highly quantitative, equal-weighting methods abound among quant traders. The general idea behind equal weighting is that the trader has no confidence in his ability to define more accurate weights and therefore decides to give all the alpha factors equal importance. A variant of this approach gives each factor an “equal risk” weighting, which incorporates the concept that giving a dollar to a highly risky strategy is not the same as giving a dollar to a less risky strategy. In Chapter 6 we cover both these approaches in more detail as they apply to portfolio construction. 

There are many forms of nonlinear models that can be used to combine alpha factors with each other. In contrast to linear models, nonlinear models are based on the premise that the relationship between the variables used to make forecasts either is not independent (i.e., each variable is not expected to add value independently of the others), or else the relationship changes over time. As such, the two main types of nonlinear models are conditional models and rotation models. Conditional models base the weight of one alpha factor on the reading of another factor. Using the same two factors as earlier, a conditional model might indicate that E/P yields should drive forecasts, but only when the price trends are in agreement with the E/P yields. In other words, the highest-yielding stocks would be candidates to be bought only if the price trends of these stocks were also positive. The lowest-yielding stocks would be candidates to be sold short, but only if the price trends of these stocks were also negative. When the agreement condition is met, the yield factor entirely drives the forecast. But if the price trend doesn't confirm the E/P yield signal, the yield signal is ignored entirely. Revisiting the linear factor combination demonstrated earlier, our conditional model would generate no signal for XOM because the price trend forecast a negative return, whereas the yield factor forecast a positive return. If, instead, XOM had a positive return forecast from the trend factor, the combined nonlinear model would have a targeted return of +20 percent over the next 12 months for that stock because this is the return expected by the value factor, which now has been “activated” by its agreement with the trend factor. An example of a conditional model is shown in Exhibit 3.9. 

The second nonlinear way to blend alphas uses a rotation approach. Rather than following trends in markets themselves, this type of model follows trends in the performance of the alpha models. These are similar to linear models except that the weights of factors fluctuate over time based on updated calculations of the various signals' weights. As time passes, the more recent data are used to determine weighting schemes in the hope that the model's weights are more relevant to current market conditions. This method usually results in giving higher weights to the factors that have performed better recently. As such, this is a form of trend following in the timing of alpha factors. 

Machine learning models are also sometimes used by quants to determine the optimal weights of various alpha factors. As in the case of determining optimal parameters, machine learning techniques applied to the mixing of alpha factors are both more common and more successful than machine learning approaches used to forecast markets themselves. These techniques algorithmically determine the mix of alpha factors that best explains the past, with the presumption that a good mix in the past is likely to be a good mix in the future. As in the case of rotational models, many machine learning approaches to mixing alpha factors periodically update the optimal weights based on the ever-changing and ever-growing set of data available. 

<table><tr><td>Value and Momentum Disagree</td><td>ValueLong</td><td>MomentumShort</td><td>SignalNone</td></tr><tr><td>Value and Momentum Agree</td><td>ValueLong</td><td>MomentumLong</td><td>SignalLong</td></tr></table>


EXHIBIT 3.9 A Simple Conditional (Nonlinear) Model for Blending Alphas


Unlike the example of using machine learning for the generation of actual alpha signals, applying machine learning to determine the weights of various alpha forecasts is more common and significantly more successful. Nevertheless, machine learning remains less widely used than the other techniques for blending alphas described here, and only a relatively small proportion of the universe of quant traders employ these methods. 

We have briefly summarized common approaches to mixing signals, or combining alpha forecasts. This is a part of the quant trading process that has received precious little attention in the academic literature and trade press, but personally I find it one of the most fascinating questions about quant trading—or any trading. It is exactly the same problem any decision maker faces when looking at a variety of sources of information and opinions: What is the best way to synthesize all available and relevant information into a sensible decision? 

It is worth noting that signal mixing shares some similarities with portfolio construction. Both are questions of sizing and combining, after all. However, they are mostly distinct and separate processes. Signal-mixing models size multiple alpha signals to arrive at one composite forecast per security, which is then used in portfolio construction. Portfolio construction models take multiple kinds of signals as inputs, including alpha signals, risk models and transaction cost models (which we cover in the next two chapters), and attempt to size individual positions correctly, given these inputs. 

## SUMMARY

Having made so many decisions about what sort of alpha should be pursued, how to specify and implement it, and how to combine this alpha with others, the quant is left with an output. The output is typically either a return forecast (expected return = X percent) or a directional forecast (expected direction = up, down, or flat). Sometimes quants add elements of time (expected return over the next Y days) and/or probability (Z percent likelihood of expected return) to help utilize the output effectively in trading decisions. See Exhibit 3.10 for a recap of the structure of a quant trading system. As we continue our progress through the black box, we will highlight the components discussed. 

I am consistently amazed by the juxtaposition of the simplicity and relatively small number of concepts used to manage money quantitatively and the incredible diversity of quant trading strategies as applied in the real world. The decisions quants make in the areas discussed in this chapter are major sources of the significant differences in the returns of traders who may be pursuing the same sources of alpha. Those evaluating quant traders (or quants who are evaluating trading strategies of their own) can use the framework provided in this chapter to help determine the nature of the strategies being traded. We now turn our attention to risk modeling, another key component of a quant trading strategy. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/3ef04dd24a8c333cd3704ad952d558cbf2d76f32b7733fef8fc1d5ab8c62fbe2.jpg)



EXHIBIT 3.10 Schematic of the Black Box


## Risk Models

The market can remain irrational longer than you can remain solvent. 

—John Maynard Keynes 

Risk management should not be thought of solely as the avoidance of risk or reduction of loss. It is about the intentional selection and sizing of exposures to improve the quality and consistency of returns. In Chapter 3, we defined alpha as a type of exposure from which a quant trader expects to profit. But we also noted that, from time to time, there can be downside to accepting this exposure. This is not what we classify as risk per se. By pursuing a specific kind of alpha, we are explicitly saying that we want to be invested in the ups and downs of that exposure because we believe we will profit from it in the long run. Though it would be great fun to accept only the upside of a given alpha strategy and reject the losses that can be associated with it, sadly, that is not possible. However, there are other exposures that are frequently linked to the pursuit of some kind of alpha. These other exposures are not expected to make us any money, but they frequently accompany the return-driving exposure. These exposures are risks. 

Risk exposures generally will not produce profits over the long haul, but they can impact the returns of a strategy day to day. More important still, the quant is not attempting to forecast these exposures, usually because he cannot do so successfully. But the fact remains that one of the great strengths of quant trading is to be able to measure various exposures and to be intentional about the selection of such exposures. This chapter deals with how quants define, measure, and control risks. 

Imagine a relative alpha strategy that focuses on the value (yield) of various stocks, buying higher-yielding stocks and selling short lower-yielding stocks. This strategy clearly can lose money if “cheap” (higher-yield) stocks underperform “expensive” (lower-yield) stocks, according to whatever definition the quant chooses for “cheapness” (or yield). That risk is inherent to the pursuit of a value strategy, even if the quant has reason to believe that value strategies should make money in the long term. However, a value strategy without further specification can end up taking significant sector bets in addition to the intentional bet on value. After all, it’s easy to see that stocks within a sector tend to move together. So if one technology stock has gotten very cheap, there’s a reasonable chance that many other technology stocks have also gotten cheap. This means that an unconstrained value-hunting strategy is likely to end up with a net long position in the technology sector. But there is no evidence that there exists a long-term benefit of overweighting one industry or sector versus another. 

More important, assume that the strategy has neither the intention nor the capability to forecast the performance of various sectors. Therefore, sector exposure would be considered a form of risk in our framework, because sector performance is not being intentionally forecast, but having net exposure to various sectors can alter the strategy's results day to day. So the key to understanding risk exposures as they relate to quant trading strategies is that risk exposures are those that are not intentionally sought out by the nature of whatever forecast the quant is making in the alpha model. 

If alpha models are like optimists, risk models are like pessimists. Risk models exist largely to control the size of desirable exposures or to deal with undesirable types of exposures. Their job is to raise hell about things that can cause losses or uncertainty, particularly those bets that are unintentionally made or are incidental byproducts of the alpha model. It both highlights and attempts to remove undesirable exposures from a portfolio. 

There are, however, only a few things you can do with a given type of exposure, aside from simply accepting it outright. Mostly you can limit its size or eliminate it altogether. The function of risk management in the investment process is to determine which of these courses of action is most prudent for each kind of exposure and to provide that input to the portfolio construction model. In general, risk models reduce the amount of money a quant can make, but this is a tradeoff many quants are willing to accept. Managing risk has the day-to-day benefit of reducing the volatility of a strategy's returns. But it also has the far more important benefit of reducing the likelihood of large losses. In many ways, the failures of quants, as in the cases of both LTCM in 1998 and the August 2007 quant liquidation, are usually precipitated by failures to manage risk. 

## LIMITING THE AMOUNT OF RISK

Size limiting is an important form of risk management. It is easy to imagine having a tremendously good trading idea, seemingly a “sure thing,” but without some sense of risk management, there can be a temptation to put all one’s capital into this single trade. This is almost always a bad idea. Why? Because, empirically, a sure thing rarely exists, so the correct way to size a trade in general is certainly not to put all your chips on it. Otherwise it is likely that in the process of “going all in,” at some point the trader will go bankrupt. In other words, it is prudent to take just as much exposure to a trade as is warranted by the considerations of the opportunity (alpha) and the downside (risk). Quantitative risk models focused on limiting the size of bets are common, and many are quite simple. The following sections explain how they work. 

There are several kinds of quantitative risk models that limit size, and they vary in three primary ways: 

1. The manner in which size is limited 

2. How risk is measured 

3. What is having its size limited 

## Limiting by Constraint or Penalty

Approaches to the size limits come in two main forms: hard constraints and penalties. Hard constraints are set to “draw a line” in terms of risk. For instance, imagine a position limit that dictates that no position will be larger than 3 percent of the portfolio, no matter how strong the signal. However, this hard limit may be somewhat arbitrary (e.g., imagine a 3.00 percent position size limit; why is a 3.01 percent position so much worse?), so quants sometimes build penalty functions that allow a position to increase beyond the “limit” level, but only if the alpha model expects a significantly larger return (i.e., a much larger expected return than was required to allow the position merely to reach the limit size in the first place). The penalty functions work so that the further past the limit level we go, the more difficult it becomes to increase the position size additionally. So, using our example, it would be far easier to see a 3.01 percent position than to see a 6 percent position, because the latter is further from the limit than the former. 

In this way, the model attempts to address the idea that an opportunity can sometimes be so good as to warrant an “exception” to the rule. In a sense, penalty functions for size limits can be thought of as making rules to govern exceptions. 

The levels of limits and/or penalties can be determined in the same ways as most other things in the quant world, namely either from theory or from the data (the latter via data-mining approaches). Theory-driven approaches mostly look like an arbitrary level that is set, tested, and, if needed, adjusted until it produces an acceptable outcome. So, to return to the earlier example of a 3 percent limit on position sizes, the quant researcher could have started with a risk limit of 5 percent. But through testing and simulating the historical results of this strategy, he could have come to realize that a far more appropriate level is 3 percent, which better balances the ability to make sizeable bets when attractive opportunities appear against the necessity of recognizing that any given trade could easily go wrong. Data-driven approaches are more varied and can include machine learning techniques to test many combinations of limits or simply testing various limit levels and letting the historical data empirically determine the final outcome. Either way, these levels and the severity of any penalty functions are parameters of the risk model that the quant must set, based on either research or heuristics. 

## Measuring the Amount of Risk

There are two generally accepted ways of measuring the amount of risk in the marketplace. The first is longitudinal and measures risk by computing the standard deviation of the returns of various instruments over time, which is a way of getting at the concept of uncertainty. In finance circles, this concept is usually referred to as volatility. The more volatility, the more risk is said to be present in the markets. $^{1}$ 

The second way to measure risk is to measure the level of similarity in the behavior of the various instruments within a given investment universe. This is frequently calculated by taking the cross-sectional standard deviation of all the relevant instruments for a given period. The larger the standard deviation, the more varied the underlying instruments are behaving. This means that the market is less risky because the portfolio can be made of a larger number of diversified bets. This can be seen easily at the extreme: If all the instruments in a portfolio are perfectly correlated, then as one bet goes, so go all the other bets. This concept is known among quants as dispersion. Dispersion can also be measured by the correlation or covariance among the instruments in a given universe. Here, too, the more similarly the instruments are behaving, the more risky the market is said to be. 

## Where Limits Can Be Applied

Size-limiting models such as these can be used to govern many kinds of exposures. One can limit the size of single positions and/or groups of positions, such as sectors or asset classes. Alternatively, one can limit the size of exposure to various types of risks. For example, in equity trading, one can limit the exposure of a model to market bets (such as a $+/-5$ percent net exposure limit) or to market capitalization bets. In general, risks that are subjected to limits or penalties are those that are not being forecast explicitly by the alpha model. If an alpha model attempts to forecast individual stocks but makes no attempt to forecast the stock market as a whole, it may be prudent to constrain the size of the bet that the portfolio can ultimately take on the stock market. 

Still another component of a risk model may be to govern the amount of overall portfolio leverage. Leverage can be controlled in a variety of ways. For example, one can manage money under the premise that when opportunities abound, more leverage is desirable, whereas when fewer opportunities are present, less leverage is desirable. Alternatively, many quants attempt to offer their investors or bosses a relatively constant level of risk. Using volatility and dispersion as proxies for risk, quants can measure the amount of risk in markets and vary their leverage accordingly to produce a more stable level of risk. The most common tool used for this purpose is known as a value at risk (VaR) model, but there are others that are similar philosophically. These models typically consider the dollar amount of exposures in a portfolio and, based on current levels of volatility, forecast how much the portfolio can be expected to gain or lose within a given confidence interval. For instance, most VaR models calculate what a daily single standard deviation move in portfolio returns will be, based on current volatility levels. The way that these models control risk in the face of rising volatility is to reduce leverage. Therefore, in general, the higher the reading of risk in a VaR model, the lower the level prescribed for leverage. 

In Chapter 10, we will discuss some of the significant problems with these kinds of risk models. For now I will simply point out that the core purpose of such risk models seems to me to be flawed. Other kinds of investments, such as stocks, bonds, mutual funds, private equity, or fine wine, do not attempt to offer fixed levels of volatility. Why should quants want to manage risk in this manner, or be asked to do so? Furthermore, if a quant is good at forecasting volatility or dispersion, there are far more interesting and productive ways to utilize these forecasts (for example, in the options markets) than there are in a risk model that governs leverage. These kinds of models often cause traders to take too little risk in more normal times and too much risk in very turbulent times. Nevertheless, they are wildly popular. 

A more theoretically sound approach, though substantially harder to implement practically, seeks to increase leverage when the strategy has better odds of winning and to decrease risk when the strategy has worse odds. The trick, of course, is to know when the odds are on one's side. Some quants solve this problem by allowing the level of leverage to vary with the overall strength and certainty of the predictions from the alpha model, which seems to be a reasonable approach. $^{2}$ 

## LIMITING THE TYPES OF RISK

Though limiting the amount of an exposure is important, some approaches to risk modeling focus on eliminating whole types of exposure entirely. Imagine that an investor's analysis indicates that CVX is likely to outperform XOM. But the trade the investor makes is simply to go long CVX while ignoring XOM. If the market drops precipitously afterward, it is likely that the investor will lose money on the trade, even if his original thesis proves correct. This is because the investor is exposed to market directional risk, even though he didn't have any particular foresight as to where the market was going. The investor could have substantially eliminated the unintentional or accidental market direction risk if he had expressed his analysis by buying CVX and shorting an equivalent amount of XOM. This way, whether the market rises, falls, or does nothing, he is indifferent. He is only affected by being right or wrong that CVX would outperform XOM. 

As a general rule, it is always better to eliminate any unintentional exposures, since there should be no expectation of being compensated sufficiently for accepting them. Quantitative risk models designed to eliminate undesired exposures come in two familiar flavors: theoretical and empirical. Each is discussed in detail later in this chapter. 

It is also worth noting that alpha models can (and often do) incorporate risk management concepts. Let's assume that a quant is building a relative alpha strategy. A significant amount of work is required to match what "relative" means to the exposures he intends to take or hedge. Revisiting an earlier example, if the quant is building a relative alpha strategy to forecast equities, he might not believe he has a valid way to forecast the sectors to which equities belong. In this case, the quant may design his bet structures so that he is making forecasts of stocks relative to their sectors, which means that he never has a bet on the direction of the sector itself, only which stocks will outperform and which stocks will underperform the sector. This, in turn, helps him eliminate sector bets, which is clearly a risk management exercise as much as it is alpha generation. As such, it is theoretically possible (and occasionally seen in practice) to incorporate all the needed components of his risk model fully into his alpha model by specifying the alpha model such that it only forecasts exactly the exposures from which it expects to make money and structures its bets to avoid exposure to nonforecasted factors. Although not all quant strategies do this, it is worth remembering to look inside the alpha model for elements of risk management, especially for those evaluating a quant. 

## Theory-Driven Risk Models

Theory-driven risk modeling typically focuses on named or systematic risk factors. Just as in the case of theory-driven alpha models, systematic risks that are derived from theory are those for which the quant can make a reasonable, economic argument. Theory-driven risk modeling uses a set of pre-defined systematic risks, which enables the quant to measure and calibrate a given portfolio's exposures. 

It is important to note that the use of the term systematic in defining risk is completely different from the use of the term systematic in describing quant strategies. Systematic risks are those that cannot be diversified away. In the world of single stocks, the market itself is a systematic risk because no amount of diversification among various single stocks eliminates an investor's exposure to the performance of the market itself. If the market is up a lot, it is extremely likely that a portfolio that is long stocks is also going to be up. If the market is down a lot, it is extremely likely that a portfolio that is long stocks will be down. Sector risk is another example of systematic risk, as is market capitalization risk (i.e., small caps versus large caps). A practical example of such a problem, and one that has been well documented by the hedge fund replication crowd, is that an unconstrained market neutral value model will very likely be making a bet on small caps outperforming large caps. $^{3}$ 

The world of fixed income, similarly, contains a host of systematic risks. For example, whether one owns corporate bonds or government bonds, owners of these bonds are all subject to interest rate risk, that is, the risk that rates go up, regardless of the level of diversification of the actual portfolio of bonds. Similar examples can be found in any asset class and frequently also across asset classes. Any economically valid grouping of instruments, in other words, can be said to share one or more common systematic risk factors. An investor who traffics in any of those instruments, then, should be aware of this risk factor and should be either making intentional bets on it or eliminating his exposure. 

## Empirical Risk Models

Empirical risk models are based on the same premise as theory-driven models, namely that systematic risks should be measured and mitigated. However, the empirical approach uses historical data to determine what these risks are and how exposed a given portfolio is to them. Using statistical techniques such as principal component analysis (PCA), a quant is able to use historical data to discern systematic risks that don't have names but that may well correspond to named risk factors. $^{4}$ For example, a PCA run on bond market data using Treasury bonds across various maturities usually shows that the first (most important) risk factor statistically corresponds to the level of interest rates, or what a theory-driven risk model might call interest rate risk. PCA and other statistical models are commonly used in equity markets as well, and these models typically find that the market itself is the first, most important driver of returns for a given stock, usually followed by its sector. These statistical risk models are most commonly found among statistical arbitrage traders, who are betting on exactly that component of an individual stock's returns that is not explained by systematic risks. It is important to note that such statistical methods may discover entirely new systematic risk factors, which a reasonably observer might be inclined to acknowledge exist but for which names have not been assigned. On the other hand, statistical risk models are subject to being “fooled” by the data into finding a risk factor that will not persist for any useful amount of time into the future. It is also possible for a statistical risk model to find spurious exposures, which are just coincidences and not indicative of any real risk in the marketplace. This is a delicate problem for the researcher. 

## How Quants Choose a Risk Model

Quants are attracted to theory-driven risk models because the risk factors they encapsulate make sense. It is hard to make the argument that market risk does not exist as a strong systematic risk factor in equities. Note that this is much the same reasoning that supports theoretical approaches to alpha modeling: Any reasonable person can understand the theory and see that it is likely to be true. This in turn can give the quant faith in the models when it isn't performing very well. Warren Buffett, for example, didn't change his stripes just because he dramatically underperformed the stock market during the Internet bubble. He was able to "keep the faith" in no small part because his approach to markets has very strong theoretical underpinnings. 

Quants that choose empirical risk models typically seek the benefits of adaptiveness. Theoretical risk models are relatively rigid, meaning that the risk factors are not altered often (otherwise the theory would not have been very strong in the first place). Yet the factors that drive markets do change over time. For awhile in early 2003, daily reports about the prospect, and later the progress, of the U.S. invasion of Iraq drove stock, bond, currency, and commodity markets almost singlehandedly. More recently, in early 2008, commodity prices were a significant factor. At other times, expectations of how much the Federal Reserve might cut or raise rates are the key drivers of market behavior. As markets evolve, the data that the markets produce reflect this evolution, and these data drive empirical risk models. For these reasons, an empirical model may be more adaptive to ever-changing market conditions by detecting through new data whatever factors are implicitly driving markets. There are two stages to this adaptation. During the early phases of a market regime change (for example, when equity investors rapidly change their behavior from risk seeking to risk aversion), the quant is using now irrelevant historical data to determine relationships and measure risk factors. Thus, during this phase, the empirical risk model will be modeling market risks incorrectly. Later, if the new behavior persists, the empirical risk model eventually will catch up to the newly prevailing theme driving markets and all will be well again. 

Besides exhibiting a weakness during a regime change, a basic understanding of statistics reveals another problem with empirical risk models. To achieve statistical significance and reduce the potential for measurement error in computing relationships among various instruments, empirical risk models require a rather large amount of data. But this leads to a tradeoff that could squelch most of the adaptiveness benefits of empirical risk models. The more data that are used, i.e., the further back into history we must look, the less adaptive a model can be, because each new data point is but one of a very large number. If we use two years' worth of rolling daily data, or approximately 520 trading days, each new day adds a new data point and causes the oldest one to fall out of the sample. So for every day that passes, only two days' data have changed out of 520. It will therefore take a long time to "turn the ship" and have the empirical model find the new drivers of risk from the data. However, if the quant attempts to improve adaptiveness by shortening the historical window used, the power of the statistics diminishes significantly so that there cannot be sufficient confidence in the measurements to act on them. 

Still, there may be benefits to empirical risk models. If the theoretical risk models are any good at being right, an empirical model should capture these effects without having to know the names of the factors beforehand. If market risk is indeed a big driver of stock prices, an empirical model should pick this up from the data. If the data don't bear it out, what good is the theory? Furthermore, the competing objectives of statistical significance and adaptiveness can be dealt with in part by using intraday data. For example, if a quant uses one-minute intraday snapshots of price activities instead of simply a single closing price for each day, he is able to extract almost 400 data points for each day in his sample, which allows him to use far fewer days to achieve the same statistical significance as another quant using a single data point for each day (the closing price). 

Ultimately, because of the comfort level with the concepts involved in theory-driven risk modeling, most quants tend to use theory-driven risk models rather than empirical risk models. It is worth noting that these two kinds of risk models are not mutually exclusive. Quants may perfectly reasonably use a combination of both, if they deem it appropriate. A small minority of managers also attempt to use their judgment and discretion to monitor market behavior and, should it become clear to them—for example, from the way that the financial media and their peers in the business are behaving—that there is a “new” risk factor that is driving markets, they jump into action and build a “made-to-order” risk factor to measure this temporary phenomenon. When they see that the new driver has faded in importance, they can remove it from the risk model, again using their judgment. 

It is worth mentioning that quants have the option, as is the case with most of the modules of the black box, to build their own risk model or to purchase one that is “off the shelf.” Most premade risk models are not of the empirical variety because empirical solutions require a specifically set universe of instruments, and the analytical techniques are usually relatively easy to implement with simple price data. Also, the vast majority of premade risk models are useful only for equity trading strategies. Several purveyors of risk models—such as BARRA, Northfield and Quantal—have made a healthy business of licensing their software to quant traders. The advantage of buying risk models is that they are premade and usually at least reasonably well thought through. However, they are also by nature somewhat generic. There are advantages to building risk models as well, primarily because they can be customized to the specific needs of the particular quant trader. 

## SUMMARY

Risk management is frequently misunderstood to be an exercise designed to reduce risk. It is really about the selection and sizing of exposures, to maximize returns for a given level of risk. After all, reducing risk almost always comes at the cost of reducing return. So, risk management activities must focus on eliminating or reducing exposure to unnecessary risks but also on taking risks that are expected to offer attractive payoffs. This is true whether one uses a systematic investment process or a discretionary one. The main difference between the two is that quants typically use software to manage risk, whereas discretionary traders, if they use software in the risk management process at all, primarily attempt merely to measure risk in some way, without any systematic process for adjusting their positions in accordance with predefined guidelines. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/f30f2512fc5bf742d481ebb1c65a124fe3bbbb655b94e28af09a0a6e5dd22504.jpg)



EXHIBIT 4.1 Schematic of the Black Box


Whether a quant uses a theoretical or empirical risk model or some hybrid thereof, the goal is the same: The quant wants to identify what systematic exposures are being taken, measure the amount of each exposure in a portfolio, and then make some determination about whether these risks are acceptable. What is good about these kinds of analyses, along with many of the other quantitative risk-modeling approaches, is that they require the quant to be intentional about risk-taking, rather than slapping together some positions that seem like good trades and more or less ignoring the incidental exposures these trades may share. For example, if oil prices become a dominant theme in investors' sentiment about the markets, positions across a variety of sectors and asset classes can be driven by oil. This can lead to significant downside if a longstanding trend in the price of oil reverses. A risk model may allow the quant to see this kind of exposure and make a choice about whether or not to do something about it. This is an important point. Quantitative approaches to risk management, by virtue of seeking to measure and make explicit what exposures are driving a portfolio, put the power into the hands of the portfolio manager to make rational, intentional decisions. Of course, whether this intentionality is helpful or hurtful depends on the judgment of the portfolio manager, even among quants. But at least quantitative risk management techniques offer the opportunity to see what risks are present in a portfolio and to what extent. 

In the next chapter, we examine transaction cost models, which are the final providers of input to help determine the most desirable target portfolio for a quant. Before doing so, let's look at Exhibit 4.1 to examine our progress through this journey inside the black box. 

# Transaction Cost Models

Without frugality, none can be rich, and with it, very few would be poor. 

—Samuel Johnson 

So far we have examined alpha models and risk models, both critical elements of the black box. The alpha model plays the role of the starry-eyed optimist, and the risk model plays the role of the nervous worrier. In this little play, transaction cost models would be the frugal accountant. 

The idea behind transaction cost models is that it costs money to trade, which means that one should not trade unless there is a very good reason to do so. This is not an overly draconian view of trading costs. Many highly successful quants estimate that their transaction costs eat away between 20 and 50 percent of their returns. 

In the world of quant trading, there are only two reasons to make a trade: first, if it improves the odds or magnitude of making money (as indicated by the alpha model), or second, if it reduces the odds or magnitude of losing money (as indicated by the risk model). These reasons, however, are subject to a caveat: A tiny, incremental improvement in the reward or risk prospects of a portfolio might not be sufficient to overcome the cost of trading. In other words, the benefits of the trade need to clear the hurdle of the cost of transacting. Neither the market nor your broker care what the benefits of a trade are. Rather, making a given trade utilizes services that cost the same regardless of the purpose or value the trade holds for the trader. A transaction cost model is a way of quantifying the cost of making a trade of a given size so that this information can be used in conjunction with the alpha and risk models to determine the best portfolio to hold. 

Note that transaction cost models are not designed to minimize the cost of trading, only to inform the portfolio construction engine of the costs of making any given trade. The part of the black box that minimizes costs is the execution algorithm, which we discuss at length in Chapter 7. It is less glamorous to describe costs than it is to minimize them, but the former remains critically important. If a trader underestimates the cost of transacting, this can lead to the system making too many trades that have insufficient benefit, which in turn leads to a problem of “bleeding” losses as a result of the constant acceptance of trading costs. If the trader overestimates the cost of transacting, this can lead to too little trading, which usually results in holding positions too long. Either way, the trader ends up with suboptimal performance, which highlights the importance of correctly estimating transaction costs. But there is also a tradeoff between using more complex models that more accurately describe transaction costs and using less complex models that are faster and less computationally burdensome. 

## DEFINING TRANSACTION COSTS

It is useful to understand what the costs of trading actually are, since we are describing ways to model them. Transaction costs have three major components: commissions and fees, slippage, and market impact. 

## Commissions and Fees

Commissions and fees, the first kind of transaction costs, are paid to brokerages, exchanges and regulators for the services they provide, namely access to other market participants, improved security of transacting, and operational infrastructure. For many quants, brokerage commission costs are rather small on a per-trade basis. Quant traders typically do not utilize many of the services and personnel of the bank but instead use only the bank's infrastructure to go directly to the market. The incremental cost of a trade to a bank is therefore very small, and even very low commissions can be profitable. Given the volume of trading that quants do, they can be extremely profitable clients for the brokerages, despite the diminutive commissions they pay. Some quants utilize significantly less of the bank's infrastructure and therefore pay even lower commission rates than others who use more and pay higher rates. 

Commissions are not the only costs charged by brokerages and exchanges. Brokers charge fees (which are usually a component of the commissions) for services known as clearing and settlement. Clearing involves regulatory reporting and monitoring, tax handling, and handling failure, all of which are activities that must take place in advance of settlement. Settlement is the delivery of securities in exchange for payment in full, which is the final step in the life of a trading transaction and fulfills the obligations of both parties involved in the transaction. These services take effort and therefore cost money. And, given that many quants are doing tens of thousands of trades each day, there can be a significant amount of work involved. 

Exchanges and electronic matching networks provide a different kind of service from brokers, namely access to pools of liquidity. Exchanges must attract traders to their floors for trading, and this trading volume then attracts other traders who are seeking liquidity. Exchanges, too, have some operational effort to make by virtue of their roles, and they also guarantee that both counterparties in a given trade uphold their contractual responsibilities. As such, exchanges also charge small fees for each transaction to cover their costs and risks (and, of course, to profit as a business). 

## Slippage

Commissions and fees certainly are not negligible. But neither are they the dominant part of transaction costs for most quants. They are also basically fixed, which makes them easy to model. If the all-in commissions and fees add up to, say, $0.001 per share, the quant must simply know that the trade in question is worth more in terms of alpha generation or risk reduction than this $0.001 per-share hurdle. On the other hand, slippage and market impact are considerably trickier to measure, model, and manage. 

Slippage is the change in the price between the time a trader (or quant system) decides to transact and the time when the order is actually at the exchange for execution. The market is constantly moving, but a trading decision is made as of a specific point in time. As time passes between the decision being made and the trade being executed, the instrument being forecast is likely to be moving away from the price at which it was quoted when the forecast was made. In fact, the more accurate the forecast, the more likely it is that the price of the instrument being forecast is actually going toward the expected price as more time passes. But the instrument makes this move without the trader benefiting, because he has not yet gotten his trade to market. Imagine a trader decides to sell 100 shares of CVX while the price is at $100.00 per share. When the trader finally gets the order through his broker and to the exchange, the price has gone down to $99.90 per share, for a decline of $0.10 per share. This $0.10 per share is a cost of the transaction because the trader intended to sell at $100.00, but in fact the price had already moved down to $99.90. In the event that the price actually moves up from $100.00 to $100.10, the trader gets to sell at a higher price, which means that slippage can sometimes be a source of positive return. 

Strategies that tend to suffer most from slippage are those that pursue trend-following strategies, because they are seeking to buy and sell instruments that are already moving in the desired direction. Strategies that tend to suffer least from slippage, and for which slippage can sometimes be a positive, are those that are mean reverting in orientation, because these strategies are usually trying to buy and sell instruments that are moving against them when the order is placed. A quant trader's latency or speed to market has a large effect on the level of slippage his strategy will experience over time. This is because slippage is a function of the amount of time that passes between the order being decided and the order reaching the market for execution. The more latency in a trader's system or communications with the marketplace, the more time passes before her order gets to the market and the further the price of an instrument is likely to have moved away from the price when the decision was made. Worse still, the more accurate a forecast, particularly in the near term, the more damaging slippage will be. 

In addition to time, slippage is also a function of the volatility of the instrument being forecast. If we are forecasting 90-day Treasury bills, which tend to move very slowly throughout the day and which can go some weeks without much movement at all, it is likely that slippage is not a major factor. On the other hand, if we are forecasting a high-volatility Internet stock, slippage can be a major issue. Google, Inc. (GOOG), has had an average daily range of 2.6 percent of its opening price, which is about 16 times larger than its average move from one day to the next. Clearly, slippage makes a huge difference if you're trading GOOG. 

## Market Impact

Market impact, the third and final major component of transaction costs, is perhaps the most important for quants. The basic problem described by market impact is that, when a trader goes to buy an instrument, the price of the instrument tends to go up, partly as a result of the trader's order. If the trader sells, the price goes down. At small order sizes, this price movement usually bounces between the current best bid and offer. However, for larger orders, the price move can be substantial, ranging in the extremes, even to several percentage points. Market impact, then, is a measurement of how much a given order "moves" the market by its demand for liquidity. Market impact is normally defined as the difference between the price at the time a market order enters the exchange and the price at which the trade is actually executed. 

The basic idea behind market impact is simple enough and is based on the ubiquitous principle of supply and demand. When a trader goes to market to execute a trade for some size, someone has to be willing to “take the other side,” or supply the size he is looking to trade. The bigger the size of the demand by a trader, the more expensive the trade will be because the 

TRADING SOFTWARE 

FOR SALE & EXCHANGE 

# www.trading-software-collection.com

Mirrors: 

www.forex-warez.com 

www.traders-software.com 

www.trading-software-download.com 

Join My Mailing List 

trader must access more of the supply. As simple as the idea of market impact is, quantifying it is actually not so straightforward. One doesn't know how much a particular trade impacts the market until the trade has already been completed, which may be too late to be useful. Also, there are many other factors that can drive a given observation of market impact and that can complicate its measurement. For example, the number of other trades that are being made in the same direction at the same time or whether news in the stock is causing impact to behave differently than normal are both issues that would affect measurements of market impact and are nontrivial to quantify. These other factors are also usually impossible to predict, much less control. Therefore, market impact as used in transaction cost modeling usually does not account for these factors but rather focuses on the size of the order relative to the liquidity present at the time. Liquidity can be defined in a number of ways, whether by the size available at the bid or offer or by measurements of the “depth of book,” which relate to those bids or offers that have been placed away from the best bid/offer prices. 

In addition, there could be some interaction between slippage and market impact that makes it tricky to segregate these two concepts in a model. A stock might be trending upward while a trader is trying to sell it, for example. In this case, both slippage and impact could look like negative numbers. In other words, the trader might deduce that he was actually paid, not charged, to sell the stock. For instance, assume that a trader decides to enter a market order to sell a stock he owns, and at that moment, the stock's price happens to be $100.00. But by the time his order hits the market, the stock, continuing its trend upward, is now trading at $100.05. Slippage is actually negative $0.05 because his order entered the marketplace at a more favorable price than the one at which he decided to sell. But now assume that the price continues to drift upward as his order makes its way to the front of the line of sale orders, simply because the marketplace's demand to buy the shares might simply overwhelm the orders, including his, to sell it. The trader ultimately sells his stock at $100.20, generating negative market impact of $0.15 on top of the negative slippage of $0.05. Clearly, entering sell orders does not usually make stocks go up, but in this case, it might not be possible to differentiate impact from slippage or either concept from the move the stock was making independently of the trader's order. Did his sell order slow the rise of the stock somewhat, and if so, by how much? These are the kinds of complications that traders must account for in building transaction cost models. 

Some kinds of trades further complicate the measurement of transaction costs. We have discussed trades that demand liquidity from the marketplace, and these behave as one might expect intuitively: If a trader demands liquidity, there is a cost charged by those providing it. Looking at this from the opposite perspective, someone gets paid to supply liquidity. Historically, the party that supplied liquidity was a market maker or specialist whose job it was to make sure that traders can execute an order when they want to. More recently, volumes across many electronically tradable instruments have increased sufficiently to allow for well-functioning marketplaces without the presence of a market maker in the middle. 

Electronic Communication Networks (ECNs) are examples of platforms for customers to trade directly with one another. The main jobs of ECNs are to attract enough customers so that there is abundant liquidity in their exchange and to provide robust technology so that their exchange can continue to function without disruption. To attract providers of liquidity, ECNs have established methods to pay traders who provide liquidity and take payment from traders who demand liquidity. It might cost something like three-tenths of a penny per share for a trader who buys shares at the offer or sells shares at the bid, whereas those providing the bids and offers that are getting “hit” are earning closer to two-tenths of a penny. The ECN keeps the difference, around one-tenth of a penny per share, as its source of revenue. Some kinds of trading strategies (usually mean reversion strategies) actually call for a mostly passive execution approach in which this act of providing liquidity is modeled as a source of profit due to the rebate programs that ECNs put in place to attract liquidity providers. 

## TYPES OF TRANSACTION COST MODELS

There are four basic types of transaction cost models—flat, linear, piecewise-linear, and quadratic—all of which are trying to solve the basic problem of how much it will cost to transact a given trade. Some of these costs are fixed and known—for example, commissions and fees. Models of transaction costs use these fixed costs as a baseline, below which the cost of trading cannot go. Other costs, such as slippage and impact, are variable and cannot be known precisely until they have been incurred. Slippage is affected by a number of factors, such as the volatility of the instrument in question (i.e., the higher the volatility, the greater the expectation of slippage) or its prevailing trend (i.e., the stronger the trend, the more slippage is likely to cost if one attempts to transact in the direction of the trend). Impact also has many drivers, including the size of the order being executed, the amount of liquidity that happens to be available to absorb the order, and imbalances between supply and demand for the instrument at the moment. Traders use transaction cost models in an attempt to develop reasonable expectations for the cost of an order of various sizes for each name they trade. 

It is worth mentioning that each instrument has its own unique characteristics based on the investor base that tends to transact in it and the amount of liquidity and volatility present in the instrument over time. GOOG doesn't trade exactly like Amazon (AMZN), and CVX doesn't trade exactly like XOM. As a result, in an effort to constantly improve their estimates of transaction costs, many quants build separate models for transaction costs for each instrument in their portfolios and allow each of these models to evolve over time based on the trading data the quant collects from his execution systems. In other words, many transaction cost models are highly empirical, allowing the actual, observable, recorded transaction data from a quant's own strategy to drive and evolve the model over time. 

The total cost of transactions for an instrument, holding all else (such as liquidity, trend or volatility) constant, can be visualized as a graph with the size of the order (in terms of dollars, shares, contracts, or the like) on the x-axis and the cost of trading on the y-axis. It is generally accepted by the quant community that the shape of this curve is quadratic, which means that the cost gets higher ever more quickly as the size of the trade gets larger (due to market impact). Certainly many quants do model transaction costs as a quadratic function of the size of the trade (more on this later). However, modeling transaction costs this way can be more complicated and computationally intensive, whereas the other choices of modeling transaction costs are simpler and less intensive. 

With advances in computer hardware and processors, the extra computational burdens are now rather easily managed, but that does not alter the fact that a proper quadratic cost function is inherently more complicated. These functions, from the simplest to most complex, are described in the following sections. 

## Flat Transaction Cost Models

The first kind of transaction cost model is a flat model, which means that the cost of trading is the same, regardless of the size of the order. This is extremely straightforward computationally, but it is rarely correct and is not widely used. A graph of a flat transaction cost model is shown in Exhibit 5.1. 

As you can see, this graph models the cost of a trade as being fixed, regardless of the size of the trade, which is an assumption that seems obviously incorrect in most circumstances. The main circumstance in which such a model is reasonable is if the size being traded is nearly always about the same and liquidity remains sufficiently constant. In this case, one can simply figure out the total cost of such a trade and assume that it will always cost the same. This assumption is wrong, but its being wrong has no consequence because the size of the trade is always the same. Note that where the solid line crosses the dashed line, the model is “close” to a correct estimate of transaction costs. So, if this point of intersection corresponds to the size of trading normally done, and if the range of that trade size is within the region where the flat line is close to the curved line, a flat t-cost model may not be so problematic. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/04995df1b599d28823cff9ef8ab8c2482e18a9e7fe72da0cbe567c465c581eb3.jpg)



EXHIBIT 5.1 Flat Transaction Cost Function


## Linear Transaction Cost Models

The second kind of transaction cost model is linear, which means that the cost of a transaction gets larger with a constant slope as the size of the transaction grows larger, as shown in Exhibit 5.2. This is a better fit relative to the true transaction cost, but it is still mostly useful as a shortcut to building a proper model. 

As you can see, the linear transaction cost model must trade off overestimating costs at smaller trade sizes with underestimating costs at larger trade sizes. Here, again, the model is correct where the solid line crosses the dashed line and is “close to correct” in the immediate vicinity of that intersection. As such, as with the flat t-cost model, if the trades being done are always within that region, a linear t-cost model is reasonable. In any case, across the curve, it appears to be a better estimator of the real transaction cost than is given by the flat transaction cost model. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/4ab178fe0380f2fc55b985cac4365c2f865a16f75caf726f276ac3905152aa2d.jpg)



EXHIBIT 5.2 Linear Transaction Cost Function


## Piecewise-Linear Transaction Cost Models

Piecewise-linear transaction cost models are used to help with precision while using reasonably simple formulas to do so. The idea of a piecewise-linear transaction cost model is that, in certain ranges, a linear estimate is about right, but at some point, the curvature of the quadratic estimator causes a significant enough rise in the slope of the real transaction cost line that it is worthwhile to use a new line from that point on. This concept is illustrated in Exhibit 5.3. 

As you can see, the accuracy of this type of model is significantly better than what can be achieved with flat or linear models across a much wider range of trading sizes; as a result, this model is rather popular among quants as a happy medium between simplicity and accuracy. 

## Quadratic Transaction Cost Models

Finally, quants can build quadratic models of transaction costs. These are computationally the most intensive because the function involved is not nearly as simple as what is used for a linear model, or even for a piecewise-linear model. It has multiple terms, exponents, and generally is a pain to build. A plot of a quadratic transaction cost model is shown in Exhibit 5.4. 

This is clearly the most “accurate” estimate we have seen of transaction costs. And yet it is not perfect, and it is significantly more difficult to build and utilize than a linear or piecewise linear model. You might be wondering how it is that we have estimated a quadratic function using a quadratic function and still ended up with a less than perfect estimate of the true transaction cost. The reason is that the solid line reflects what is expected, whereas the dotted line reflects what is actually observed after the fact. This is a significant difference because the solid line must be specified before one trades, whereas the dotted line is what is observed empirically after one trades. Because the actual transaction cost is an empirically observable fact and any estimation of transaction costs is a prediction, the prediction is unlikely to be perfect. Causes of differences between estimated and realized transaction costs might include changes in liquidity or volatility in the instrument over time or changes in the types of traders (e.g., market makers, hedge funds, mutual funds, or retail investors) who are transacting in the same stock over time. Of course, the quant is trying as hard as possible to make good forecasts, but given that it is known that the forecast is very unlikely to be perfect and that speed and simplicity are both also desirable, the tradeoff between accuracy and simplicity is one which requires the judgment of the quant. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/124f6f3ecc397ce156f80191b3fc9a430aa4bd631b52072affeea3f514389b61.jpg)



EXHIBIT 5.3 Piecewise-Linear Transaction Cost Function


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/04c4fc482a8b5a12be3194d4aebbdcba8d05e5cb64b3e5f153d19bba3432f8db.jpg)



EXHIBIT 5.4 Quadratic Transaction Cost Function


Regardless of the type of model used, the quant must describe the cost of trading each instrument in her universe. After all, a less liquid small cap stock is likely to be more expensive to trade than a more liquid mega cap stock, and that must be a factor in deciding how much of each to trade. Furthermore, the quant should refresh empirical estimations of transaction costs both to keep the model current with the prevailing market conditions as well as to indicate when more research is required to improve the model itself. 

## SUMMARY

The role of transaction cost models is simply to advise the portfolio construction model how much it might cost to transact. Its job is not to minimize the cost of trading, just as the job of the alpha model is not to generate returns but rather to make forecasts and to provide these forecasts to the portfolio construction model. Cost minimization happens in two phases. First, the portfolio construction model, using the input provided by the transaction cost model, accounts for cost in generating a target portfolio. Second, the target portfolio is passed along to the execution algorithms, which explicitly attempt to transact the desired portfolio as cheaply as possible. 

There are several kinds of transaction model, ranging from extremely simple to rather complex. The simpler models are useful for traders who either do trades of roughly the same size in a given instrument all the time or who trade in such small size that they can simply assume a modest cost and be close to correct most of the time. The more complex models are useful for quants who have the potential to trade significant, or significantly variable, quantities of a given instrument in a short period. Any of the four models described here can be valid in the right set of circumstances. The question to consider is whether the model chosen fits the application and facts of the situation. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/6eee73be80f09a76fcac4e4ded33b81d3298d4ee12a173694e893cf9abda5603.jpg)



EXHIBIT 5.5 Schematic of the Black Box


We turn our attention next to portfolio construction models, which utilize the inputs provided by the alpha, risk, and transaction cost models described over the past three chapters, and come up with a target portfolio designed to maximize returns relative to risk. But first we check our progress on the map of the black box in Exhibit 5.5. 

# Portfolio Construction Models

No sensible decision can be made any longer without taking into account not only the world as it is, but the world as it will be.
—Isaac Asimov 

The goal of a portfolio construction model is to determine what portfolio the quant wants to own. The model acts like an arbitrator, hearing the arguments of the optimist (alpha model), the pessimist (risk model), and the cost-conscious accountant (transaction cost model) and then making a decision about how to proceed. The decision to allocate this or that amount to the various holdings in a portfolio is mostly based on a balancing of considerations of expected return, risk, and transaction costs. Too much emphasis on the opportunity can lead to ruin by ignoring risk. Too much emphasis on the risk can lead to underperformance by ignoring the opportunity. Too much emphasis on transaction costs can lead to paralysis because this will tend to cause the trader to hold positions indefinitely instead of taking on the cost of refreshing the portfolio. 

Quantitative portfolio construction models come in two major forms. The first family is rule based. Rule-based portfolio construction models are based on heuristics defined by the quant trader and can be exceedingly simple or rather complex. The heuristics that are used are generally rules that are derived from human experience, such as by trial and error. 

The second family of quantitative portfolio construction models is optimized. Optimizers utilize algorithms—step-by-step sets of rules designed to get the user from a starting point to a desired ending point—to seek the best way to reach a goal that the quant defines. This goal is known as an objective function, and the canonical example of an objective function for an optimizer is to seek the portfolio that generates the highest possible return for a unit of risk. By their nature, optimizers can be more difficult to understand at a great level of detail, but they are straightforward conceptually. 

As in the case of blending alpha models, discussed in Chapter 3, portfolio construction models are a fascinating area to study. Furthermore, portfolio construction turns out to be a critical component of the investment process. If a trader has a variety of investment ideas of varying quality but allocates the most money to the worst ideas and the least money to the best ideas, it is not hard to imagine this trader delivering poor results over time. At a minimum, his results would be greatly improved if he could improve his approach to portfolio construction. And yet actual solutions to the problem of how to allocate assets across the various positions in a portfolio are not exceedingly common. This subject receives rather a lot less time and space in the academic journals and in practitioners' minds than ways to make a new alpha model, for example. This chapter will give you the ability to understand how most quant practitioners tackle this problem. 

## RULE-BASED PORTFOLIO CONSTRUCTION MODELS

There are four types of rule-based portfolio construction models: equal position weighting, equal risk weighting, alpha-driven weighting, and decision-tree weighting. The first two are the simplest and have at their core a philosophy of equal weighting; they differ only in what specifically is being equally weighted. Alpha-driven portfolio construction models mainly rely on the alpha model for guidance on the correct position sizing and portfolio construction. Decision-tree approaches, which look at a defined set of rules in a particular order to determine position sizing, can be rather simple or amazingly complex. I describe these approaches from simplest to most complex. 

## Equal Position Weighting

Equal position-weighted models are surprisingly common. These models are used by those who implicitly (or explicitly) believe that if a position looks good enough to own, no other information is needed (or even helpful) in determining its size. The notion of the strength of a signal, which, as already discussed, is related to the size of a forecast for a given instrument, is ignored except insofar as the signal is strong enough to be worthy of a position at all. At first glance, this might seem like an oversimplification of the problem. However, some serious quants have arrived at this conclusion. The basic premise behind an equal-weighting model is that any attempt to differentiate one position from another has two potentially adverse consequences, which ultimately outweigh any potential benefit from an unequal weighting. In other words, they choose an equal-weighting model because of the many disadvantages they see in unequal weighting. 

The first potential problem with unequal weighting is that it assumes implicitly that there is sufficient statistical strength and power to predict not only the direction of a position in the future but also the magnitude and/or probability of its move relative to the other forecasts in the portfolio. Quants utilizing equal-weighting schemes believe, instead, that the alpha model is only to be trusted enough to forecast direction, and as long as the forecast of direction is sufficiently large to justify trading the instrument at all, it is worth trading at the same size as any other position. 

The second potential problem with unequal weighting of a portfolio is that it generally leads to a willingness to take a few large bets on the "best" forecasts and many smaller bets on the less dramatic forecasts. This weighting disparity, however, may lead to the strategy taking excess risk of some idiosyncratic event in a seemingly attractive position. This can be the case regardless of the type of alpha used to make a forecast. For instance, in momentum-oriented strategies, many of the strongest signals are those for which the underlying instrument has already moved the most (i.e., has showed the strongest trending behavior). In other words, it might be too late, and the trader risks getting his strongest signals at the peak of the trend, just as it reverses. Similarly, for mean reversion-oriented strategies, many of the largest signals are also for those instruments that have already moved the most and are now expected to snap back aggressively. But frequently, large moves happen because there is real information in the marketplace that leads to a prolonged or extended trend. This phenomenon is known to statisticians as adverse selection bias. Mean reversion bets in these situations are characterized as "picking up nickels in front of a steamroller," which is a colorful way of saying that betting on a reversal against a very strong trend leads to being run over if the trend continues, which it sometimes does. Analogous arguments can be made for almost all alpha strategies, making it easy to construct good arguments against unequal-weighting positions. Therefore, the basic argument in favor of an equal-weighted approach is one of mitigating risk by diversifying bets across the largest useful number of positions. It is worth mentioning that equal weights are sometimes subject to constraints of liquidity, in that a position is weighted as close to equally as its liquidity will allow. Such liquidity considerations can be applied to each of the other rule-based allocation methodologies discussed in this chapter. 

## Equal Risk Weighting

Equal risk weighting adjusts position sizes inversely to their volatilities (or whatever other measure of risk, such as drawdown, is preferred). More volatile positions are given smaller allocations, and less volatile positions are given larger allocations. In this way, each position is equalized in the portfolio, not by the size of the allocation but rather by the amount of risk that the allocation contributes to the portfolio. An example is shown in Exhibit 6.1, which shows an example of a two-stock portfolio. As you can see, the more volatile stock (GOOG) gets a smaller allocation in the portfolio than the less volatile stock (XOM). 


EXHIBIT 6.1 A Simple Equal-Risk Weighted Portfolio


<table><tr><td></td><td>Equal Weight</td><td>Volatility</td><td>Volatility-Adjusted Weight</td></tr><tr><td>GOOG</td><td>50%</td><td>2.5%</td><td>39%</td></tr><tr><td>XOM</td><td>50%</td><td>2.0%</td><td>61%</td></tr></table>

The rationale is straightforward. A small-cap stock with a significant amount of price volatility might not deserve quite the same allocation as a mega cap stock with substantially less volatility. Putting an equal number of dollars into these two positions might in fact be taking a much larger and inadvertent real bet on the small cap stock. This is because the small cap stock is much more volatile, and therefore every dollar allocated to that stock would move the portfolio more than the same dollars allocated to the larger cap (and, likely, less volatile) position. As such, some quants who believe that equal weighting is the most appropriate method will utilize an equal risk-weighting approach in an effort to improve the true diversification achieved. 

However, the equal risk-weighting approach also has its shortcomings. Whatever unit of risk is equalized, it is almost always a backward-looking measurement, such as volatility. Instruments with higher volatilities would have smaller allocations, whereas lower-volatility instruments would have larger allocations. But what if the less volatile instruments suddenly became the more volatile? This is not merely a hypothetical question. For many years, bank stocks were very stable. Then, in 2008, they suddenly became highly volatile, more so even than many technology stocks. Any backward-looking analysis of the volatility of stocks that didn't emphasize the last debacle among financial stocks (10 years earlier, in 1998) would likely have been misled by the steady behavior of these stocks for the several years prior to 2008, and therefore an equal-risk model is likely to have held much larger positions in banks than were warranted once volatility spiked in 2008. 

## Alpha-Driven Weighting

A third approach to rule-based portfolio construction determines position sizes based primarily on the alpha model. The idea here is that the alpha model dictates how attractive a position is likely to be, and this signal is the best way to size the position correctly. Still, most quants who utilize this approach would not allow the size of the largest position to be unlimited. As such, they would use the risk model to provide a maximum size limit for a single position. Given the limit, the strength of the signal determines how close to the maximum the position can actually be. This is much like grading on a curve, where the “best score” receives the largest position size, and the scores below the best receive smaller sizes. 

The types of constraints used with this approach to portfolio construction can also include limits on the size of the total bet on a group (e.g., sector or asset class). For example, one could constrain individual positions to be less than 3 percent of the portfolio and each sector to be less than 20 percent. There still needs to be a function that relates the magnitude of the forecast to the size of the position, but these functions can generally be straightforward, and in general, the bigger the forecast, the larger the position. Alpha weighting is favored by some quants because it emphasizes making money, which is after all the goal of the whole exercise. However, quant strategies, such as futures trend following, that utilize this method can suffer sharp drawdowns relatively frequently. This is because these models usually have the largest signals when a price trend is already well established. As the trend proceeds, the size of the position grows, but this will often leave the trader with his largest position just when the trend reverses. Caution is therefore advisable when utilizing an alpha-driven portfolio construction algorithm, because such an approach causes a heavy reliance on the alpha model being right—not only about its forecast of the direction of an instrument but also about the size of the move the instrument will make. 

## Decision-Tree Models

The fourth rule-based approach to portfolio construction is known as a decision tree. It might be easiest to explain a decision-tree portfolio allocation model by example. Imagine an alpha model based on trend following that outputs +1 if it is expecting an instrument's price to rise, 0 if it is expecting no significant change in price, and -1 if it is expecting a decline in the instrument's price. Now imagine we want to incorporate a second type of alpha model—say, a value strategy, which provides the same format of output as we just described for the trend model (i.e., +1, 0, or -1). Assume further that we have three assets: Asset A is a very low-risk asset, Asset B is a medium-risk asset, and Asset C is also a medium-risk asset but with less liquidity than Asset B. As the final output of our model, we want to know the percentage of our portfolio to allocate to each asset (i.e., the position size for each asset in percentage terms). A decision-tree allocation system for this framework might look like Exhibit 6.2. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/2fdb7cb6becebb6e55af307e3e417285a1790e7d12a7cc4a2615ab24c69e4d5d.jpg)



EXHIBIT 6.2 Example of a Decision-Tree Portfolio Construction Model


In this example, we see that there is a decision path to arrive at the percentage allocation for a given instrument, depending on what the alpha models (trend and value) are forecasting and what instrument it is (A, B, or C). To illustrate how to read the tree, assume that Asset A got a trend score of +1 and a value score of 0, meaning that the trend model predicted Asset A would go up and the value model predicted Asset A to be unchanged. How much of Asset A should we have in our portfolio? The answer is 5 percent, and it comes from following the +1 branch of the trend alpha, then the 0 branch of the value alpha, and then finding the target size of Asset A at 5 percent. 

It is worth noting that the percentage limits themselves can be functions of the risk model and/or transaction cost model. For example, Asset A might be the least risky and most liquid, but an unconstrained tree may have wanted to give it a 15 percent allocation in the case that both the value and trend models had the same scores. But if we assume that the risk model constrains the largest position of any security to be not more than 7 percent of the portfolio, regardless of its merits, the position is limited to 7 percent instead of 15 percent. Or imagine the case where Asset C and Asset B are equally volatile but Asset C is less liquid than Asset B. In this scenario, the transaction cost model might constrain the maximum size held in Asset C, because larger position sizes in less liquid names imply larger transactions costs from increased market impact. 

This example was a fairly simple portfolio construction decision tree with merely two alpha models and three types of assets. You can easily imagine that the number of outcomes can grow dramatically if we include more alpha models or more types of positions. It is impossible, given the variety of decision-tree algorithms that can be imagined and effectively used, to give a broad judgment as to their strengths or weaknesses. Certainly there are tradeoffs to consider between simpler trees, which may oversimplify the problem of portfolio construction, and more complex trees, which may be very difficult to troubleshoot or even build correctly. 

## Summary of Rule-Based Portfolio Construction Models

Regardless of which type of rule-based portfolio construction model is used, the alpha model, risk model, and t-cost model can be incorporated in portfolio building. In an equal-weighted model, for example, constraints on the equal weighting can exist because certain instruments are too expensive to transact in, according to the transaction cost model. Obviously, the exact nature of the interaction between the other components of the black box and the portfolio construction model depends entirely on the type of portfolio construction model. For example, a decision-tree model may make use of a risk model in an entirely different way than a portfolio construction model that relies primarily on the alpha model, subject to constraints from the risk model. 

To summarize, rule-based portfolio construction models can be extremely simple (as in the case of an equal-weighted portfolio) or rather complex (in the case of a decision tree with many layers). The challenge common to all of them is to make the rules that drive them rational and well reasoned. We will discuss more about the way quants choose portfolio construction methods later in this chapter. 

## PORTFOLIO OPTIMIZERS

Portfolio optimization is one of the most important topics in quantitative finance. This is one of the first areas in quant finance to receive the attention of serious academic work; in fact, the case could easily be made that the father of quantitative analysis is Harry Markowitz, who published a landmark paper entitled “Portfolio Selection.” $^{1}$ He invented a technique known as mean variance optimization, which is still ubiquitous today, though much sophistication has been built around its core. In 1990, he shared a Nobel Prize with William Sharpe for both their contributions to the understanding of the quantitative analysis of portfolio construction. 

Portfolio optimizers are based on the principles of modern portfolio theory (MPT), which are canonical in the asset management industry. The core tenet of MPT is that investors are inherently risk averse, meaning that if two assets offer the same return but different levels of risk, investors will prefer the less risky asset. A corollary is that investors will take on extra risk only if they expect to receive extra return as compensation. This introduced the concept of risk-adjusted return. Mean variance optimization is a formal way of building portfolios based on MPT. Mean and variance are two of the inputs to the optimizer, and the output is a set of portfolios that have the highest return at each level of risk. The mean in question is the average expected return of each asset being evaluated. Variance is a proxy for the expected risk of each asset and is computed as the standard deviation of the returns of the various assets one is considering owning. A third input to the optimizer is the expected correlation matrix of these same assets. Using these inputs, the optimizer delivers a set of portfolios that offer the highest possible return for various levels of risk, known as the efficient frontier. Several other inputs are utilized by quants in real trading applications, including (a) the size of the portfolio in currency terms; (b) the desired risk level (usually measured in terms of volatility or expected drawdown); and (c) any other constraints, such as a “hard to borrow” list provided by a prime broker in equity trading, which reduces the size of the universe with which the optimizer can work. These inputs are not required by the optimizer, and the first two are also mostly arbitrary, but they help yield a portfolio that is practical and useful to the quant trader. 

The reason these strategies are called optimizers is that they are seeking to find the maximum (optimal) value of a function that has been specified by the researcher. This function is known as the objective function, where objective is used in the sense of goal. The optimizer seeks this goal by an algorithm that conducts a directed search among the various combinations of instruments available to it. As it examines the return and risk characteristics of a given combination, it compares this with previously examined combinations and detects what seems to cause the portfolio's behavior to improve or degrade. By this method, the optimizer is able to rapidly locate a series of optimal portfolios, which are those for which returns cannot be bested by those of any other portfolio at a given level of risk. What is allowed or disallowed is determined by the alpha model, risk model, and transaction cost model. The objective function that many quants use is the same as the original: maximizing the return of a portfolio relative to the volatility of the portfolio's returns. However, an infinite array of objective functions can be used. For example, one could specify an objective function that will cause the optimizer to maximize portfolio return relative to peak-to-valley drawdown instead of return volatility. The use of return versus risk is itself entirely optional, and one could very easily optimize an objective function focused entirely on the total expected return of a portfolio. 

## Inputs to Optimization

The inputs required for an optimizer, as already mentioned, are expected returns, expected volatility, and a correlation matrix of the various instruments to be considered for the portfolio. It is worth understanding where practitioners get the estimates and expectations used in optimization from, since they are critical to the model itself. We consider each of the aforementioned inputs in order. 

Expected Return In more traditional finance, such as private wealth management, expected returns are usually set to equal very long-term historical returns because usually the goal is to create a strategic asset allocation that won't need to be dynamically readjusted. By contrast, quants tend to use their alpha models to drive expected return. As we mentioned in our discussion of alpha models, the output of the alpha model typically includes an expected return and/or an expected direction. Forecasts of direction can be used as forecasts of return simply by making all positive forecasts equal and all negative forecasts equal. 

Expected Volatility Many practitioners, whether in traditional finance or in quant trading, tend to use historical measures for the second input to the optimizer, namely volatility. Some, however, develop and use their own forecasts of volatility. The most common approaches to forecasting volatility utilize stochastic volatility models. Stochastic, in Greek, means random. In statistics, a stochastic process is one that is somewhat predictable but that has some element of unpredictability or randomness built in. The basic idea behind the stochastic family of volatility forecasting methods is that volatility goes through phases in which it is at high levels, followed by periods in which it is at low levels (i.e., the somewhat predictable phases of the volatility cycle), with occasional jumps (the somewhat random and unpredictable part). The most widely used such technique is called Generalized Autoregressive Conditional Heteroskedasticity (GARCH), which was proposed in 1986 in the Journal of Econometrics by the Danish econometrician Tim Bollerslev. $^{2}$ Other approaches to stochastic volatility modeling and variants of the original GARCH forecast abound. All these techniques basically share the notion that volatility goes through clustered periods of relative calm, followed by periods of swings, followed by a return to calm, and so forth. This can be seen in Exhibit 6.3 as being a relatively useful way to describe market volatility. From 2000 to 2003, the S&P 500 was rather volatile. This was followed by a period of calm from mid-2003 to mid-2007, and after that by another period of extreme volatility from mid-2007 through 2008. Even during the relatively calm period, short, seemingly periodic bursts in volatility occurred. GARCH types of models do a reasonable job of forecasting volatility in this sort of pattern. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/687d7161199f86b4e7fa0e540638bff839fd5426ed87574546495030a68ebe35.jpg)



EXHIBIT 6.3 Historical S&P 500 Volatility


Indeed, there exist many other approaches to forecasting volatility, and they can be understood in much the same way that we evaluated strategies for forecasting price. They tend to make forecasts based on ideas of trend, reversion, or some fundamental model of volatility; they can be made over various time horizons; they can forecast either the volatility of a single instrument or the relative volatility of more than one instrument, and so forth. GARCH forecasts, for example, combine elements of trend and mean reversion in forecasting volatility. 

Expected Correlation The third input to the optimizer is the correlation matrix, which offers researchers few approaches to computing or forecasting it. Correlation is at heart a measure of the similarity of the movements of two instruments, expressed in a number between -1 and +1. A +1 correlation implies exact similarity, whereas a -1 correlation implies that the two instruments are exactly opposite, or anti-correlated. A 0 correlation is perfect non-correlation and implies that the two instruments are entirely dissimilar but not opposite. 

There are a number of problems with using standard correlation measures in quant trading, most of which we will address at various points later. Most relevant for the moment, the measurement of the relationships between two instruments can be very unstable over time. They can even be unreliable over long time periods. For example, imagine a portfolio with two investments: one in the S&P 500 and one in the Nikkei 225. Taking the data on both since January 1984, we can see that these two indices correlate at a level of 0.37 since inception. The range of correlations observed using weekly returns over any consecutive 365 calendar days (a rolling year) is shown in Exhibit 6.4. 

You can see that the level of correlation observed between the S&P 500 and the Nikkei 225 depends quite a lot on exactly when it is measured. Indeed, this correlation reaches the lowest point in the sample (+0.01) in October 1989 and by mid-2008 was at its highest point (+0.66). What's worse, the correlation between these indices went from +0.02 to +0.58, and then back to +0.01 all during the course of about four years, from November 1985 until October 1989. Even using a rolling five-year window, the range is +0.21 to +0.57. 

If the strategy specifies appropriate groupings of instruments, as in our earlier example of industry groups, the stability of the correlations over time improves. This specification can be made either in the definition of relative in a relative alpha strategy and/or in the specification of the risk model. So, for example, if the model groups together companies such as XOM and CVX, this can be seen as reasonable, because these two companies have much in common. Both have market capitalizations on the same general scale, both are oil companies, both are based in the United States and have global operations, and so on. Meanwhile, a comparison between CVX and Sun Microsystems (JAVA) might be less defensible based on fundamental factors, such as the fact that JAVA isn't an oil company but is a much smaller capitalization company in the technology sector. Somewhat predictably, this theoretical difference in the comparability between these two pairs of stocks (XOM vs. CVX, CVX vs. JAVA) also bears out in the data, as shown in Exhibit 6.5. 


1/1984–8/2008 (Weekly returns)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/e66a61bf0ee88d2274861902319d6b9f328f923b4fda50ddc79ab3c394edfa33.jpg)



EXHIBIT 6.4 Rolling Yearly Correlation Between S&P 500 and Nikkei 225


As you can see, CVX and XOM correlate relatively well over the entire 20+-year period shown. The lowest correlation level observed between this pair is approximately 0.40, and the highest is 0.89. The correlation over the entire period is 0.70. Meanwhile, CVX and JAVA correlate poorly, at a level of only 0.14 over the whole sample, with a minimum two-year correlation of -0.14 and a maximum of 0.36. Furthermore, the correlation between CVX and XOM changes more smoothly over time than that between CVX and JAVA. Though both pairs can be said to be somewhat unstable, it is quite clear that grouping CVX with XOM is less likely to be problematic than grouping CVX with JAVA. To be clear, the instability of correlations among financial instruments is more or less a fact of the world. It is not the fault of optimizers, nor of correlation as a statistic, that this happens to be the case in the finance industry. 


Rolling Two-Year Correlation, March 1987–March 2008


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/b049d3324889f0c7e3d9d25d2d2b6fd4fd3a8418cc7aaecea78bd38287bba56d.jpg)



EXHIBIT 6.5 Correlation Over Time Between Similar and Dissimilar Instruments


## Optimization Techniques

There are many types of optimizers. They range from basic copies of Markowitz's original specification in 1952 to sophisticated machine learning techniques. This section provides an overview of the most common of these approaches. 

Unconstrained Optimization The most basic form of an optimizer is one that has no constraints; for example, it can suggest putting 100 percent of a portfolio in a single instrument if it wants. Indeed, it is a quirk of unconstrained optimizers that they often do exactly that: propose a single-instrument portfolio, where all the money would be invested in the instrument with the highest risk-adjusted return. 

Constrained Optimization To address this problem, quants figured out how to add constraints and penalties in the optimization process, which forces more “reasonable” solutions. Constraints can include position limits (e.g., not more than 3 percent of the portfolio can be allocated to a given position) or limits on various groupings of instruments (e.g., not more than 20 percent of the portfolio can be invested in any sector). An interesting conundrum for the quant, however, is that, if the unconstrained optimizer would tend to choose unacceptable solutions, to the extent that constraints are applied it can become the case that the constraints drive the portfolio construction more than the optimizer. For example, imagine a portfolio of 100 instruments, with the optimizer limited to allocating no more than 1.5 percent to any single position. The average position is naturally 1 percent (1/100 of the portfolio). So, the very best positions (according to the alpha model) are only 1.5 times the average position, which is relatively close to equal-weighted. This is fine, but it somewhat defeats the purpose of optimizing. 

Black-Litterman Optimization Fischer Black, of Black-Scholes fame, and Bob Litterman, of Goldman Sachs, in 1990 produced a new optimization method that was first introduced in an internal memo at Goldman but was later published in 1992 in the Financial Analysts Journal. $^{3}$ Their Black-Litterman optimizer addresses some of the problems associated with errors in the measurement of inputs to an optimizer. Most important, they proposed a method of blending an investor's expectations with a degree of confidence about those expectations, and these with the historical precedent evident in the data. For example, imagine that CVX and XOM correlate at 0.7 historically, but going forward, a trader's alpha model forecasts that XOM will rally while CVX will fall. In this case, the correlation between CVX and XOM over the period being forecast may be quite low, perhaps even negative, despite the evidence from history. Black-Litterman provided a way to adjust historically observed correlation levels by utilizing the investor's forecasts of return for the various instruments in question. Furthermore, to the extent that the investor has greater confidence in some forecasts and less in others, this fact can be incorporated. If the investor forecasts significant divergence between instruments that historically have correlated at a high level but has a low level of confidence in the forecast, something much closer to the historical level of correlation is used. To the extent that the investor has greater confidence, the forecast returns play a more important role in determining the correlation coefficient utilized by the Black-Litterman optimizer. Some quants prefer this method of optimization because it allows for a more holistic approach to combining the alpha model with the other inputs to optimization. 

Grinold and Kahn's Approach: Optimizing Factor Portfolios Another kind of optimizer that bears mentioning is described in Grinold and Kahn's seminal Active Portfolio Management.⁴ This kind of portfolio optimization technique is directly aimed at building a portfolio of signals, whereas most optimizers try to size positions. The method of optimizing proposed by Grinold and Kahn is fairly widely used. The idea of this approach is to build factor portfolios, each of which are usually rule-based (in fact, very often equal-weighted or equal risk-weighted) portfolios based on a single type of alpha forecast. So, for example, one could imagine building a momentum portfolio, a value portfolio, and a growth portfolio. Each of these portfolios is in turn simulated historically, as though it were making stock picks through the past. For instance, the value factor's portfolio would look back at the historical data and simulate the results it would have achieved by buying undervalued instruments and shorting overvalued instruments through this historical sample, as though it were reliving the past. In this way, a time series of the returns of these simulated factor portfolios is generated. These simulated factor portfolio returns are then treated as the instruments of a portfolio by the optimizer. 

One benefit of this approach is that the number of factor portfolios is typically much more manageable, usually not more than about 20, corresponding to the number of individual factors. What is therefore being optimized is not a portfolio of thousands of instruments but rather the mixing of a handful of factor portfolios. This is certainly an easier hurdle to clear in terms of the amount of data needed. Factor portfolio optimization allows for the inclusion of the risk model, transaction cost model, portfolio size, and risk target as inputs, in much the same way as described for other optimizers. 

Given the weight of each model, we ultimately need to ascertain the weight of each position. The way that each position's weight is computed in this approach is perhaps easiest to understand by example. Imagine we have two alpha factors, both of which yield only a directional forecast (i.e., +1 for a buy signal or -1 for a sell signal). We have 100 stocks in the factor portfolios, which are equally weighted for simplicity's sake. This means that each stock is 1 percent of each factor portfolio. Let's assume that the factor optimization procedure dictated that we should have a 60 percent weight on the first factor portfolio and a 40 percent weight on the second. The allocation to any stock in this example is 1 percent (the weight of each name in each factor portfolio) times the signal given by that factor (i.e., long or short) times the weight of each factor portfolio. Let's say that the first alpha factor's forecast for a given company is +1, and the second is -1. So the total allocation to the company is $[(1\%) * (+1) * (60\%)] + [(1\%) * (-1) * (40\%)] = +0.2\%$ , meaning that we would be long 0.2 percent of our portfolio in this company. 

Resampled Efficiency In Efficient Asset Management, Richard Michaud proposed yet another approach to portfolio construction models. $^{5}$ Rather than proposing a new type of optimization, however, Michaud sought to improve the inputs to optimization. His “Resampled Efficiency” technique may address oversensitivity to estimation error. Michaud argues that this is in fact the single greatest problem with optimizers. Earlier, we gave the example of the instability of the correlation between the S&P 500 and Nikkei 225. This implied that, if we used the past to set expectations for the future—in other words, to estimate the correlation between these two instruments going forward—we are reasonably likely to have the wrong estimate at any given time, relative to the actual correlation that will be observed in the future. A quant will have such estimation errors in the alpha forecasts, in the volatility forecasts, and in the correlation estimates. It turns out that mean variance optimizers are extremely sensitive to these kinds of errors in that even small differences in expectations lead to large changes in the recommended portfolios. 

Michaud proposes to resample the data using a technique called Monte Carlo simulation to reduce the estimation error inherent in the inputs to the optimizer. A Monte Carlo simulation reorders the actually observed results many times, thereby creating a large number of time series all based on the same underlying observations. For example, imagine we are testing a trend-following strategy that is based on the closing prices of the S&P 500 from 1982 through 2008. But now we want to get a sense of how robust the strategy might be if the future doesn't look exactly like the past. So, we can take the return distribution of the S&P 500, which tells us how often the S&P gains or loses various amounts, and use it to create a large number of alternate histories for the index. By reshuffling the returns in this way, we have less dependence on the past looking just like the future, because we now have thousands of "pasts" over which to test our strategy. Interestingly, the average return and the volatility of returns will remain the same across all these alternate histories because they are based on the same underlying return distribution. But now we can see how often our strategy performs well or poorly across all these hypothetical scenarios and therefore how likely it is to work well or poorly in a future that might not resemble the past precisely. This technique is thought to produce more robust predictions than are possible from simply using only the actual sequence of returns the instrument exhibited, in that the researcher is capturing more aspects of the behavior of the instrument. It is this intuition that is at the heart of Monte Carlo simulations. 

Data-Mining Approaches to Optimization As a final note on the types of optimizers, we turn our attention briefly to data-mining approaches applied to portfolio construction models. Some quants use machine learning techniques, such as supervised learning or genetic algorithms, to help with the problem of optimization. The argument in favor of machine learning techniques in portfolio construction is that mean variance optimization is a form of data mining in that it involves searching many possible portfolios and attempting to find the ones that exhibited the best characteristics, as specified by the objective function of the optimizer. But the field of machine learning aims to do much the same thing, and it is a field that has received more rigorous scientific attention in a wide variety of disciplines than portfolio optimization, which is almost exclusively a financial topic. As such, there may be good arguments for considering machine learning approaches to finding the optimal portfolio, especially due to the quality of those algorithms relative to the mean variance optimization technique. 

## Final Thoughts on Optimization

One interesting byproduct of portfolio optimization is that there are instances in which an instrument that is forecast to have a positive return in the future by the alpha model might end up as a short position in the final portfolio (or vice versa). How can this happen? Imagine we are trading a group of equities in the United States and that one of the constraints imposed on the optimization by the risk model is that the portfolio must be neutral to each industry group. In other words, for every dollar of long positions within, say, the software industry, we must have a corresponding dollar of short positions within the same industry (to create a zero net position in the software industry). But what if we have positive return expectations for every stock in the software industry? The optimizer would likely be long those software companies with the highest positive return expectations and short those software companies with the lowest positive return expectations. 

Certainly, among sophisticated quants that use optimizers to build their portfolios, the most simplistic optimization techniques (particularly unconstrained) are in the minority. Still, though the intuition behind optimization is sound, the technique itself is perhaps the most properly labeled “black box” part of the quant trading system. The output is sometimes confusing relative to the inputs because of the complexity of the interactions among an alpha model, a risk model, and a transaction cost model, along with the constraints of size and desired risk level. Compounding the complexity, we have to consider the interaction among various kinds of alpha factors within the alpha model. That said, it is highly likely that the larger positions in the portfolio are those with the strongest expected returns. The strange behavior described here—having a position in the opposite direction as the alpha model’s forecast—is observable mainly with the smaller positions in the portfolio because it is among these that the expected returns can be overcome by transaction cost or risk management considerations. 

## OUTPUT OF PORTFOLIO CONSTRUCTION MODELS

Regardless of the type of portfolio construction approach used, the output of the quantitative portfolio construction model is a targeted portfolio: the desirable individual positions and the targeted sizes of each. This target portfolio is compared to the current portfolio, and the differences are the trades that need to be done. In the case that a brand-new portfolio is being built from scratch, all the positions recommended by the portfolio construction model will need to be executed. If, instead, the quant is rerunning the portfolio construction model as she would do periodically in the normal course of business, she would need to do only the incremental trades that close the gap between the newly recommended portfolio and the existing portfolio she holds. It is, as you have guessed by now, also interesting to consider how often the quant reoptimizes her portfolio. 

## HOW QUANTS CHOOSE A PORTFOLIO CONSTRUCTION MODEL

I have observed that the significant majority of quants using rule-based allocation systems seem to take an “intrinsic” alpha approach (i.e., they forecast individual instruments rather than forecasting instruments relative to each other). Most, but not all, of these are actually futures traders. Meanwhile, quants utilizing optimizers tend to be focused on a “relative” alpha approach, most typically found among equity market neutral strategies. There is no obvious reason for the difference in the preferred portfolio construction approach for relative and intrinsic traders. However, it is likely that quants that use relative alpha strategies already believe implicitly in the stability of the relationships among their instruments. After all, in a relative alpha paradigm, the forecast for a given instrument is as much a function of that instrument’s behavior as it is about the behavior of the other instruments, to which the first is being compared. If these relationships are unstable, the strategy is doomed to start with, because its first premise is that certain comparisons can be made reliably. If the relationships are stable, however, it is entirely logical and consistent that the quant can rely on them for portfolio construction as well. 

Meanwhile, if a quant takes an intrinsic alpha approach, he is making an implicit statement that his portfolio is largely made up of a series of independent bets, so relying on a correlation matrix (one of the key inputs to the optimizer) might not be very useful. Instead, this kind of quant would focus efforts more directly on risk limits and alpha forecasts subject to transaction costs. This more direct approach to portfolio construction is usually best implemented with a rule-based model. It is interesting to note that the kind of alpha model a quant builds is likely to impact the choice of portfolio construction model that makes the most sense to use. 

## SUMMARY

We have described the two major families of portfolio construction models. Rule-based models take a heuristic approach, whereas portfolio optimizers utilize logic rooted in modern portfolio theory. Within each family are numerous techniques and, along with these, numerous challenges. How does the practitioner taking a rule-based approach justify the arbitrariness of the rules he chooses? How does the practitioner utilizing optimization address the myriad issues associated with estimating volatility and correlation? In choosing the “correct” portfolio construction technique, the quant must judge the problems and advantages of each and determine which is most suitable, given the type of alpha, risk, and transaction cost models being used. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/960c35449991c75b97dc441c94a37ec18cc4de6d5966b68ca19b9b5fe4b27f52.jpg)



EXHIBIT 6.6 Schematic of the Black Box


We have completed the penultimate stop on the trip through the inside of the black box, as seen on our roadmap (Exhibit 6.6). Next we will see how quants actually implement the portfolios that they derived using their portfolio construction models. 

# Execution

Quality is never an accident; it is always the result of high intention, sincere effort, intelligent direction and skillful execution.
—William A. Foster 

So far in our tour through the black box, we have seen how quants determine what portfolio they want to own. Quants build alpha models, risk models, and transaction cost models. These modules are fed into a portfolio construction model, which determines a target portfolio. But having a target portfolio on a piece of paper or computer screen is considerably different than actually owning that portfolio. The final part of the black box itself is to implement the portfolio decisions made by the portfolio construction model. 

There are two basic ways to execute a trade: The first is electronic, the second is through a human intermediary (e.g., a broker). Most quants elect to utilize the electronic method, because the number of transactions is frequently so large that it would be unreasonable and unnecessary to expect people to succeed at it. Electronic execution is accomplished through direct market access (DMA), which allows traders to utilize the infrastructure and exchange connectivity of their brokerage firms to trade directly on electronic markets such as ECNs. 

Several points bear clarification. First, DMA is available to any trader, whether quant or discretionary, and in fact, many discretionary traders also utilize DMA platforms offered by their brokers to execute trades. Trades submitted via DMA can still be done manually if so desired, but they are manually entered into computer software, which then directly communicates with the electronic exchanges. In the past, traders would call their brokers, who would “work” orders, which meant the latter trying to pick the best times, sizes, and prices or occasionally contacting other counterparties to negotiate a better price on a larger block trade. Now, particularly on electronic exchanges, execution algorithms are far more commonly responsible for working orders. 

One can acquire execution algorithms in one of three ways: build them, use the broker's, or use a third-party software vendor's. This chapter will, in part, detail the kinds of things execution algorithms are designed to handle. A brief overview of high-frequency trading follows thereafter. We will then discuss more recent developments related to the infrastructure quants utilize to execute trades. 

Though most orders executed by quants are algorithmic, traders occasionally utilize a service most brokerages offer, namely, portfolio bidding. I describe this idea only briefly, since it is not a particularly quantitative way to execute trades. In a portfolio bid, a “blind” portfolio that the trader wants to transact is described by its characteristics in terms such as the valuation ratios of the longs and shorts, the sector breakdown, market capitalizations, and the like. Based on these characteristics, brokers quote a fee, usually in terms of the number of basis points (100 basis points = 1 percent) of the gross market value of the portfolio being traded. In exchange for this cost, a guaranteed price is given to do the transaction. The quant using this arrangement, in other words, is buying certainty of the prices of his trades and in exchange is paying the broker for providing that certainty. Once an agreement is reached between the broker and the quant, he receives the transactions from the broker at the pre-agreed price, and the broker receives his fee for the service and assumes the risk of trading out of the portfolio at future market prices, which may be better or worse than the prices they have guaranteed. “Human” execution of quant portfolios generally looks like a portfolio bid rather than a series of individual orders being worked. 

## ORDER EXECUTION ALGORITHMS

Order execution algorithms determine the way in which systematic execution of a portfolio is actually done. We can examine the kinds of decisions the algorithms must make in real time in much the same framework in which we'd think about how discretionary traders implement their orders. The kinds of considerations are the same in both cases, and as has been the theme throughout this book, we find that quants differ here from their discretionary counterparts principally in the mechanics and not so much in the ideas. The principal goal of execution algorithms, and the function of most execution desks in general, is to minimize the cost of trading into and out of portfolios. 

As a quick refresher, there are two kinds of orders one can use: market orders and limit orders. A market order is submitted to the marketplace and is generally unconditional, but it must be filled. It can be filled in pieces or in full at whatever price prevails at the market at the time the order's turn to be executed arrives. In contrast, limit orders allow the trader to control the worst price at which he is willing to transact, but the trader must accept that his order might not get executed at all or that only a part of it might be executed. Various versions of these orders, such as market-on-close orders or stop-limit orders, exist. There are also modifiers to orders, such as "fill or kill," "all or none," and "good till cancelled." A fill-or-kill order is a limit order in which all the shares for the order must be filled immediately or the order is automatically cancelled. An all-or-none order is like a fill-or-kill order without the cancellation feature, so if an order is not immediately completed in its full size, it remains untouched. A good-till-cancelled order is a limit order that is not automatically cancelled at the end of the day but remains in effect for days or weeks, until explicitly cancelled by the trader. 

In the process of executing orders, the quant must determine the kind of orders that will be used in various circumstances. The main benefit of market orders is that they are likely to be executed very quickly and, in any case, are virtually certain to be executed at some price. However, the price received is variable and cannot be controlled. On the other hand, the main benefit of limit orders is that the trader has control over the worst price at which he is willing to transact, but there is no guarantee that the order will get executed at all, because the price the trader specifies might not be competitive relative to what others are bidding and offering in the marketplace. 

The collection of all available bids and offers for a given security is known as the limit order book, which can be thought of as a queue of limit orders to buy and sell. In electronic markets, each order that is placed on the exchange is prioritized. Highest priority is given to orders at the best prices (the best bids for buy orders and the best offers for sell orders), whereas lower priority is given to those who are bidding or offering worse prices. For two traders offering the same price, traders who show their orders are given higher priority than those who hide them (more on this shortly), and for traders who are still tied, the tiebreaker is, not surprisingly, which one came first. $^{1}$ 

## Aggressive versus Passive

The first kind of decision an execution algorithm must make is how passive or aggressive to be. Passivity and aggression represent how immediately a trader wants to do a trade. Market orders are considered aggressive, because the trader is saying to the market that he just wants his order filled immediately, at whatever the prevailing market price is. As such, a market order to buy is likely to pay at least the offer, whereas a market order to sell is likely to receive, at most, the current best bid. If the order size is larger in share size than the current best bid and offer, the transaction will take out multiple bids and offers at increasingly adverse prices. Paying this kind of cost to transact might be worthwhile if the trader really wants the trade done immediately. But if not, this much aggressiveness in the order placement might not be necessary, and the transaction can be executed in a different manner. 

Limit orders can be placed at differing levels of aggressiveness as well. For example, a limit order to buy at the current best offer is a fairly aggressive limit order because at any time there could be some sellers in the market who might be willing to sell at the (lower) bid price. However, this kind of order immediately attempts to transact at the higher “sellers’ price” and is in that sense an aggressive limit order. By contrast, a limit order to buy well below the current bid is passive because the trader is effectively saying he is fine with the low probability of being executed, but if he does execute, he is at least only paying the price he’s specified. 

To complicate matters further, as we discussed in the discussion of transaction cost models, many exchanges actually pay providers of liquidity for placing passive orders while they charge traders for using liquidity being provided. To phrase it another way, orders that cross the spread (orders to buy that are executed at the offer, or orders to sell that are executed at the bid) are using, or “taking,” liquidity in that each share or contract executed in this manner is taking out a passive order that’s been placed by another trader, which reduces the liquidity available. The practice of paying for liquidity sweetens the deal for a passive order, but only if the order is actually executed. Not only does the passive trader get a better transaction price, but he also receives a commission rebate from the exchange (typically on the order of two-tenths of a cent per share). But again, the tradeoff is a reduction in certainty of being filled. It is generally true that alpha strategies that are based on a concept of momentum will be paired with execution strategies that are more aggressive, because the market can tend to run away from the trader if he is not aggressive. It is also generally the case that mean reversion strategies utilize more passive execution strategies because they are taking the risk that the prevailing trend persists, and at least by executing at a better price, this mitigates the downside risk of “standing in front of the bulldozer.” 

Another factor driving the use of passive or aggressive execution strategies is the strength of the signal and the model's confidence level in the signal. A stronger, more certain signal probably will be executed with greater aggressiveness than a weaker or less certain signal. This idea is easily demonstrated by extreme examples. If you had inside information that a stock was going to double in the next day because of a merger, and if trading on inside information was legal (which it, of course, is not), you should be perfectly happy to pay a lot of money to the marketplace to fill a large order to buy this stock. It would be illogical to fret over a few pennies per share when many dollars are the upside. On the other hand, if you have no view on a stock but were being asked what you'd be willing to pay for it by someone who wants to sell it, you are likely to offer a low enough price that there is some margin of safety. 

A fairly common “middle ground” is to put out limit orders somewhere between the best current bid and offer. This way, the trader jumps to the front of the queue for executions, and though he pays a bit more than he would have to if he simply waits for his order to get executed passively, the limit order caps the amount by which he is worse off. At the same time, he has a higher probability of execution than he would if he simply added his order to the current best bid or offer. In market parlance, adding an order to the best bid or offer is known as joining it; placing an order that constitutes a new best bid or offer is known as improving. 

To summarize, the first characteristic of an order execution algorithm is its level of aggressiveness, and this can be thought of as a spectrum. At the most aggressive end of the spectrum are market orders; at the least aggressive end of the spectrum are limit orders with prices that are far away from the current market. The level of aggressiveness is usually a function of the type of strategy being employed and depends on the strength of the signal and the system's confidence in that signal. 

## Large Order versus Small Order

Whether for market orders or limit orders, the quant has to determine how much of a total order to send at a time. Recall from our discussion of transaction cost models that a large order costs a lot more to execute than a small order because demand for liquidity starts eating into more and more expensive supplies of liquidity. As such, a popular technique for automated execution involves taking a large transaction for, say, 100,000 shares of a stock, breaking it into 1,000 orders of 100 shares each, and spreading the orders out over a window of time. Of course, by spreading the order out over time, the trader runs the risk that the price moves more while the order is being spread out than it would have if it had been executed right away, even with the extra cost of market impact. Generally, however, it is agreed that spreading out trades is a useful way to reduce the cost of transacting, and this is an extremely common feature in execution algorithms. The exact size of the chunks that are sent to market to be executed depends on the transaction cost model's estimate of the transaction cost of variously sized orders for the instrument in question. The determination of the size of each order is related to the analysis of the correct level of aggressiveness. Again, a highly attractive trade warrants taking on more of it quickly than a trade that is relatively less appealing. 

## Hidden Order versus Visible Order

Hidden orders are a way of masking one's limit orders from the market at the cost of losing priority versus visible orders at the same price. The goal here is to "hide one's hand" in terms of buy/sell intentions from other market players while still being able to trade. Any time a trader puts into the queue a visible order—that is, an order that he has allowed the rest of the market to see—he gives away a bit of information. If many units are already being bought, and another trader submits another order to buy, you can imagine a scenario where the price goes up quickly and results in the transaction costing a significant amount more. In other words, the marketplace has a broad-based sense of market impact, based on the total imbalance between the buyers and sellers at the moment. Placing a hidden order provides no information to the market, which helps stave off these imbalances. However, it reduces the priority of the trade in the queue, leading to a lower probability of execution. 

One algorithmic trading technique that utilizes hidden orders is known as iceberging, which takes a single large order and chops it into many smaller orders, most of which are posted to the order book as hidden orders. In this way, the bulk of the order is hidden from other traders, just as only the tip of an iceberg is visible above sea level. It is worth noting that not all exchanges allow hidden orders. 

## Where to Send an Order

In some markets, there are several pools of liquidity for the same instruments. For example, Island and Archipelago are currently two alternative pools of liquidity for trading U.S. stocks. There is a whole field of work in the area of smart order routing, which involves determining to which pool of liquidity it is best to send a given order at the current moment. Typically, the determination itself is straightforward. If one pool of liquidity has the units of a security you want for a better price than another pool of liquidity, you route the order to the first pool. More recently, U.S. regulators have attempted to mitigate the perceived problem of having different “best” prices for a given stock in different pools of liquidity. One of the consequences of this rule is that the best bid and offer for a stock across any valid pool of liquidity must be displayed by all pools of liquidity concurrently. This somewhat mitigates the purpose of smart order routing, but there remain differences (for example, in the depth of liquidity for a given name on various ECNs or connectivity speeds), so intelligence still needs to be applied even in this circumstance. 

In other markets that continue to be accessible via multiple, somewhat independent pools of liquidity for the same exact instruments, smart routing continues to be an interesting area of work. 

## Cancelling and Replacing Orders

Traders have every right to cancel orders if they are unfilled. This leads to all sorts of shenanigans among quants. Some will intentionally place large numbers of orders they have no intent of ever seeing executed, then rapidly cancel them and replace them with other orders. This can be done to gain information about how the market responds to the changing depth of the book, which can provide more information about how to profit from that pattern of reaction. It also masks the true intentions of the trader who is looking to transact. If a trader is trying to buy a large number of shares, it might make sense to also enter a large number of small orders to sell the same shares, further away from the market, because he can cancel those quickly while improving the market's perception of the overall balance between buys and sells. It should be noted that for a variety of reasons, many exchanges do not like to have orders canceled and replaced and therefore can penalize traders whose cancellation rates are high. 

# HIGH-FREQUENCY TRADING: BLURRING THE LINE BETWEEN ALPHA AND EXECUTION

Some quants attempt to make extremely near-term bets (e.g., seconds or less into the future) about markets. The alphas that drive these strategies are typically called microstructure alphas and focus on liquidity patterns in the order book for both the target instrument and related securities. Larger quants also use these microstructure forecasts to guide their execution models, thereby improving their costs of entering trades that their portfolio construction model has deemed necessary. For example, if two trades are equally appealing over the expected life of the trade, but one is significantly more appealing in the extremely short term, this can lead to greater aggressiveness in the more appealing name and more passivity in the less appealing one. 

This kind of nuance can make a small difference in a given trade, but in the long run, these savings can add up to a significant improvement in long-term performance. Some quants actually trade these microstructure alphas as independent high-frequency strategies, which are characterized by very small, short-term, high-probability bets. To do so, they must be prepared to invest rather substantially in infrastructure and research while only being able to manage small sums due to the problems presented by market impact. 

In other words, if a high-frequency strategy is too large, it will begin to move the market so much that the prices at which it finally executes trades are so close to the forecast prices that there is no room left for any actual profit from the trade. 

Often, high-frequency forecasts are not so different from the ones used on longer timescales, especially momentum or mean reversion. However, some researchers who specialize in this area have ideas that are somewhat different than typical momentum or mean reversion concepts. High-frequency trading strategies are a sort of cutting-edge computer game in which the algorithms have names like guerilla, sniper, and shark. For instance, the shark strategy is designed to detect the presence of a large order that has been iceberged and hidden. It works by sending a series of very small trades. If the result is that each of those small orders gets filled quickly, this may be the sign of a large and iceberged order. To take advantage of this discovery, the shark can simply front-run this large, hidden order by placing visible trades, which will pop in front of the hidden iceberged order with preferable queue placement (because of exchange priority rules). To fill itself, the iceberging strategy will then have to push prices up (for a buy order; down for a sell) to get sufficient supply for the rest of its trade to be executed. Meanwhile, the shark keeps bidding ahead of the iceberged order and then rides on its coattails, hoping to build a small position as the price trends. When the large iceberged order is finally complete, it will have pushed prices favorably for the shark, which can then exit the position with a quick and relatively riskless profit. 

Still other high-frequency traders utilize machine learning techniques to discern patterns in the execution of other players' orders in the market. Because execution algorithms tend to repeat their behavior over and over, they may leave behind a footprint that can be detected by a machine learning technique. The more inferior the execution models, the more easily they are found out. And once patterns are uncovered, the machine learning strategy can profit from a continuance of these patterns in the future. 

Machine learning techniques have been applied more successfully in the high-frequency trading arena than in the longer-term space. One probable reason for this better success is that the amount of data available is massive for a high-frequency trader utilizing intraday ticks and order book data. Another reason is that the kinds of behaviors that are exhibited in the very short term are less easily captured by ideas such as momentum and mean reversion. Furthermore, as already mentioned, the patterns of behavior at this timescale are somewhat stable due to the fact that they are driven by computer algorithms. Indeed, so much of the broader market's decision making in the timeframe of milliseconds is done by machines (other participants' execution models) that statistical learning algorithms may actually be well suited to figure out the best way of profiting in this space. 

All of the above might sound like a robot war game, with slower-moving or more conventional robots (such as icebergs) being preyed upon by sharks and spied upon by machine learning agents. It sounds that way because it basically is that way. High-frequency trading has often been labeled an “arms race,” where the ability to shave off a handful of microseconds constitutes an enormous edge, at least until a competitor shaves off a handful more. 

## TRADING INFRASTRUCTURE

We have already mentioned that to execute and process electronic trades, connectivity needs to be set up between the trader on one end and the exchange on the other. Furthermore, a protocol for messages between these two parties is required. The hardware and software quants utilize in implementing their trading strategies are the final pieces of infrastructure. As in most things, quants face a choice between building or buying infrastructure in all three of these areas. Due to regulatory and other constraints, most traders utilize the services of independent brokerage firms that act as the trading agents for their strategies. One of the benefits of using a broker is that the infrastructure requirements are handled by that broker, and this infrastructure can be costly to replicate. 

The most common type of exchange connectivity offered to a trader is, as already discussed, DMA access. This involves using the broker's servers and routing orders through them to the various pools of liquidity being traded. However, some quants, especially those engaged in high-frequency strategies, utilize a more recently available form of connectivity called colocation or sponsored access. Brokers offer easy access to markets through DMA platforms, but they add a fair amount of latency to the process. Quant strategies that are sensitive to this latency utilize the colocation option as a way of improving their executions. In a colocation setup, the trader attempts to place his trading servers as physically close to the exchange as possible. In many cases, this means hosting servers in the same exact data centers as those of the exchange. The reason for the desire for proximity is quite literally to cut down to as short as possible the distance that the order must travel—at the speed of light—over the communication lines between the quant's server and the exchange. A typical and relatively high-quality DMA platform tends to cause between 10 and 30 milliseconds of delay between the time the order is sent from the quant's server and the time the order it reaches the exchange. By contrast, a well-designed colocation solution can have an order travel from the quant's server to the exchange in about a quarter of a millisecond (250 microseconds) or even less. In the arms race that is high-speed trading, this can be a useful improvement. 

In terms of communication, the most important piece of infrastructure in electronic trading is known as the Financial Information eXchange (FIX) protocol. The FIX protocol began in 1992 as a communications framework between Fidelity Investments and Salomon Brothers and has grown to become the method of choice for real-time electronic communication among most of the world's banks, money managers using electronic executions, and exchanges offering electronic equities or futures trading. The FIX protocol is a standardized way for various participants in the trading process to communicate information. Considering that the number of FIX messages is measured in billions per day, it is obviously critical to have a standard format for these communications. The software that implements the FIX protocol, which itself is free and open source, is known as a FIX engine. Quants must choose whether to build or buy such engines, and a fair number of quants land in each camp. In general, quants who are extremely sensitive to latency, such as high-frequency microstructure traders, will likely build their own customized FIX engines to ensure optimal speeds. 

The final component of trading infrastructure relates to the hardware and software used. Again, quants can choose to build or to buy various solutions. For example, it is easy to buy computers using extant hardware (such as microchips, data storage, etc.), order management systems (which process and manage trades), or third-party execution algorithms. On the other hand, I know of several examples of quant firms that have developed their own microchips to perform specialized trading functions with greater speed than conventional, commercially available chips. Beyond this, quants attempt to make their algorithms, databases, and execution software leaner, to reduce the internal latency of processing market data and sending an order out to the market. While writing this very chapter, by coincidence, I received a white paper regarding programming methods that can optimize the computing performance of multicore processors. Even the most fundamental choices about computers—for example, the operating system of choice—are considered. For instance, most quants use either Linux or UNIX operating systems because they are more efficient and therefore provide better computing performance than a PC/Windows configuration. 

## SUMMARY



We have detailed a variety of issues related to the execution of orders for a quant trading strategy. The very first choice the quant must make is whether 



![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/2d1d7acbfed6274a39d532efd75399f1c343e351f72b21791e138f5bc0b066fd.jpg)



EXHIBIT 7.1 Schematic of the Black Box


to build or buy a trading solution. The technical expertise and cost of building a world-class execution infrastructure lead many quants, especially those utilizing longer-term trading strategies or those trading smaller portfolios, to choose the route of buying these services, either from brokers or execution service providers. Both brokers and execution vendors do, in fact, charge for the service of providing execution algorithms and connectivity. This charge normally is made by increasing commission costs. It can often cost five or more times as much per share to trade through a third party's algorithms than to trade using one's own. On the other hand, for traders who have expertise in this area and for those managing significant sums, it can be worthwhile to build custom execution models and infrastructure. 

Execution is where the rubber meets the road for a quant system and how the quant interacts with the rest of the marketplace. This continues to be a fruitful area of research, as it has been for the past several years. It is, however, an arms race, and a player who is the best in the world today and spends millions per year to get that way can be toppled by the next great technology or software innovation. Nevertheless, this is clearly an important part of the quant trading system. 

This chapter concludes our stroll through inside of the black box, as we can see from Exhibit 7.1. We turn our attention now to understanding the data that feeds quant trading strategies. 

I'd sell you my kids before I'd sell you my data, and I'm not selling you my kids. 

—Anonymous quantitative futures trader 

Most quants utilize some form of input/output model, which is a term that comes from computer science (and that has been borrowed by econometricians). It refers to the way in which information processors (such as computers) communicate with the world around them. One of the things we love about input/output models is that if you provide the same input a million times, the output should be consistent every time. The process that transforms an input into an output is typically the part that people call the black box in quant trading, and we have seen the inside of this box in the preceding chapters. In this chapter, we will examine the inputs of quant trading models, namely, the data they depend on. 

Mechanically, data reach the black box through data servers, which are connected to one or more data sources. On receipt of these data, the black box processes them for use by the alpha, risk, transaction cost, portfolio construction, and execution models that constitute the internal organs of the quant trading machine. These data servers usually process data using software some quants call data feed handlers, which are designed to convert the data to a form in which they can be stored and utilized the modules of the quant system. 

## THE IMPORTANCE OF DATA

It is difficult to overstate the importance of data, and it can be seen from many perspectives. First, data, as we know, are the inputs to quant trading systems. It turns out that the nature of the inputs to a system dictates what you can do with the system itself. For example, if you were handed a lot of lettuce, tomatoes, and cucumbers, it would be very difficult to build, say, a jet engine. Instead, you might decide that these inputs are most suited for making a salad. To make a jet engine, you more or less need jet engine parts, or at least materials that can handle high velocities and acceleration, high altitude and a wide range of temperatures. The same is true with quant systems. To the extent that you are given data that focus on macroeconomic activity, it is extremely difficult to build a useful model that doesn't somehow reflect macroeconomic concepts. 

Frequently, many details of the model itself are driven by characteristics of the inputs that are used. Refining our example, imagine that you are given slow-moving macroeconomic data, such as quarterly U.S. GDP figures; furthermore, you receive them only a week after they are released to the public. In this situation, it is unlikely that you can build a very fast trading model that looks to hold positions for only a few minutes. Furthermore, note that the U.S. data you get might be useful for predicting bonds or currency relationships, but they might not be sufficient to build a helpful model of equity markets. U.S. GDP data will also tell you little about what is happening in Uruguay or Poland in any of their securities markets. 

The nature of the data you are using is also an important determinant of the database technology you would rationally choose for storage and retrieval, a subject we will discuss in greater detail later in this chapter. Data sometimes even drive decisions about what types of hardware and software make the most sense. Again and again, we see that the nature of data—and even how they are delivered—determines a great deal about what can be done and how one would actually go about doing it. 

Still another perspective on the importance of data can be understood by examining the consequences of not doing a good job of gathering and handling data. Returning to the idea that quant trading systems are input/output models, if you feed the model bad data, it has little hope of producing accurate or even usable results. A stunning example of this concept can be seen in the Mars Climate Orbiter (MCO). The $200 million satellite was destroyed by atmospheric friction because one team of software engineers programmed the software that controlled the craft's thrusters to expect metric units of force (Newtons) while another team programmed the data delivered to the satellite to be in English units (pound-force). The software model that controlled the satellite's thrusters ran faithfully, but because the data were in the wrong units (causing them to be off by a factor of almost 4.5 times), the satellite drifted off course, fell too close to Mars' surface, and ended up being destroyed. In the aftermath, National Aeronautic and Space Administration (NASA) management did not blame the software error but rather the process used to check and recheck the software and the data being fed to it. $^{1}$ 

Problems, however, can be easy to miss. After all, the results frequently are numbers that can be seen to as many decimal places as you care to see. But this is false precision. This effect is often summarized succinctly as garbage in, garbage out. Because the kind of trading with which we are concerned is all about timing, timeliness is critical. If you build a fantastic model to forecast the price of a stock over the next day, but you don't provide it data until a week later, what good is the model? This is an extreme example, but it is almost exclusively the case that the faster you can get information into a good model, the better off you'll be, at least if succeeding is part of your plan. 

Bad data can also lead to countless hours of squandered hours in research and, in extreme cases, even to invalid theorization. Data are generally required to develop a theory about the markets or anything else in science. After all, scientists utilize their observations of the world to generate their theories. So, if we provide the scientist with incorrect information without his knowledge, he is likely to develop theories that are incorrect when applied to the real world. Bad data lead to bad outcomes. If the data have serious problems, it will be impossible to tell whether a system being tested, no matter how sophisticated the testing nor how elegant the model, is good or bad. 

Many quant trading firms recognize this point in their behavior. Most of the best firms collect their own data from primary sources rather than purchasing it from data vendors. They also expend significant resources in the effort to speed up their access to data, to clean data, and even to develop better ways of storing data. Some firms have dozens or even hundreds of employees dedicated exclusively to capturing, cleaning, and storing data optimally. 

## TYPES OF DATA

There are basically two kinds of data: price data and fundamental data. Price data is actually not solely related to the prices of instruments; it includes other information got or derived from exchanges or transactions. Other examples of price data are the trading volumes for stocks or the time and size of each trade. Indeed, the entire “order book,” which shows a continuous series of all bids and offers for a given instrument throughout the course of a day as well as the amounts of each, would be considered price-related data. Furthermore, we would place anything that can be derived from the levels of various indices (e.g., percent changes computed from the daily values of the S&P 500 index) in the price-related data category, even if the index itself is not a traded instrument. 

There is a rather broad variety of fundamental data, which can make it difficult to categorize effectively. In a sense, fundamental data relate to anything besides prices. However, what all types of data have in common is that they are expected to hold some usefulness in helping to determine the price of an instrument in the future, or at least to describe the instrument in the present. Also, we can do a bit more to create a reasonable taxonomy of fundamental data. The most common kinds of fundamental data are financial health, financial performance, financial worth, and sentiment. For single stocks, for example, a company's balance sheet is mostly used to indicate the financial health of the company. Meanwhile, for macroeconomic securities (e.g., government bonds or currencies), budget or trade deficits, or personal savings, data might serve to indicate the financial health of a nation. Portions of the income and cash-flow statements (e.g., total net profits or free cash flow) are used to determine financial performance; other portions are used to indicate financial health (e.g., ratios of accruals to total revenue or cash flow to earnings). Similarly, the U.S. GDP figure might be an example of macroeconomic financial performance data, whereas the trade balances figure is an example of macroeconomic financial health data. The third type of fundamental data is about what a financial instrument is worth. Some common examples of this kind of data in the equities world are the book value or the amount of cash on hand. The last common type of fundamental data is sentiment. How analysts rate a stock or the buying and selling activity of company insiders are examples of sentiment data for stocks; economists' forecasts for GDP growth for next quarter are an example of macroeconomic sentiment data. 

We don't want to oversimplify the matter. Clever researchers are constantly looking for new and innovative sources of information that might not be used by other players. Technology advances in the broader marketplace have greatly aided this kind of activity. For example, recently some firms (and now even some data vendors) have been quantitatively analyzing news stories written in plain English. Quants can systematically parse these stories, extract quantifiable information, and build strategies around this type of data. However, this remains largely an exercise in getting faster and more robust indicators of sentiment (or other types of fundamentals already described), so we believe that sources such as this are still fundamental in nature. In a still newer and more interesting development, we know of at least one company that is attempting to use aggregated global positioning system (GPS) data to determine the level of various types of economic activity more quickly and accurately than is possible using government-reported statistics. But this too seems to be a potential improvement (even a revolution) in the approach to collecting such data; the nature of the fundamental information being sought is by no means different than it was. 

This is not to diminish the ingenuity of those who developed such ideas. We simply point out that, for better or worse, our classification scheme seems to do a reasonable job of explaining the kinds of data that exist. 

An interesting pattern has emerged in our discussion of data. Much of what we saw in the price category of data tended to focus on shorter time scales. We spoke about daily values and even continuous intraday values. Meanwhile, in the fundamental category, we tend to see new information released on the scale of weeks, months, or quarters. One implication we can immediately discern from these differing periodicities is that, in general, trading strategies utilizing price-related information have the option to be much faster than those utilizing primarily fundamental information. Again, this is simply because the information we have about the securities is refreshed more frequently with price-related information than it usually is with fundamental data. This statement is not universal, since some fundamental strategies, especially those focused on changes in fundamentals or sentiment, can be very short-term oriented. However, this statement holds most of the time and is a handy rule of thumb to bear in mind when looking at a quant strategy. 

## SOURCES OF DATA

One can get data from many sources. Most direct, but also perhaps most challenging, is to get raw data from the primary sources. In other words, a quant would get price data for stocks traded on the New York Stock Exchange directly from the NYSE. This has the benefit of allowing the quant maximum control over the cleaning and storing of data, and it can also have significant benefits in terms of speed. However, there is also a massive cost to doing things this way. It would require building connectivity to every primary source, and if we are speaking about trading multiple types of instruments (e.g., stocks and futures) across multiple geographical markets and exchanges, the number of data sources can explode. With each, software must be built to translate the primary sources' unique formats into something usable by the quant's trading systems. 

Examples of the kinds of primary sources and data types include these: 

■ Exchanges. Prices, volumes, timestamps, open interest, short interest, order book data. 

■ Regulators. Financial statements from individual companies, filings related to large owners of individual stocks as well as insider buying and selling activities. 

■ Governments. Macroeconomic data, such as employment, inflation, or GDP data. 

■ Corporations. Announcements of financial results and other relevant developments (e.g., changes in dividends). 

■ News agencies. Press releases or news articles. 

■ Proprietary data vendors (or data generators). House-created data that might be of interest. For example, brokerage firms frequently issue reports about companies, and some firms track and license investment funds-flow data. 

Because of the scope of the work involved in accessing data directly from primary sources, many firms use secondary data vendors to solve some aspects of the data problem. For example, some data vendors take financial statement data from regulatory filings around the world and create quantified databases that they then license to quant traders. In this example, the data vendor is being paid for having solved the problem of building a consistent framework to house and categorize data from many direct sources. But imagine that the quant firm wants to collect both price and fundamental data about companies around the world. It is frequently the case that entirely different companies provide each of these types of data. For instance, for a given stock, there may be one data vendor providing price data and a completely different one providing fundamental data. These data vendors may also differ in the way they identify stocks. One might use the ticker; another might use a SEDOL code or some other identifier. $^{2}$ With two or more different data sets regarding the same security, the quant will have to find a way to ensure that all the data ultimately find their way into the same company's record in its internal database. The tool used to help with this is frequently called a security master in that it is the master file mapping the various ways that data vendors identify stocks to a single, unique identifier method that the quant will use in her trading system. 

As you might have guessed, still other firms have cropped up to provide unified databases across many types of vendors and data types. These we can call tertiary data vendors, and they are paid to make data easy to access for the quant. They establish connections with many primary and secondary data vendors, build and maintain security masters, and even perform some data-cleaning activities (a subject we will discuss in more detail presently). As a result, they are immensely popular among many firms. However, we should make it clear that as much benefit as they offer in terms of ease, tertiary data vendors do add another layer between the quant and the original data. This layer can result in loss of speed and possibly in less control over the methods used to clean, store, or access data on an ongoing basis. 

## CLEANING DATA

Having established the types and importance of data, we now turn to the kinds of problems quants face in managing these raw materials and how they handle such flaws. Despite the efforts of primary, secondary, and sometimes even tertiary data vendors, data are often either missing or incorrect in some way. If ignored, this problem can lead to disastrous consequences for the quant. This section addresses some of the common problems found with errors and some of the better-known approaches used to deal with these challenges. It's worth noting that although some of the following data problems seem egregious or obvious to a human, it can be challenging to notice such problems in a trading system that is processing millions of data points hourly (or even within one minute, as in the case of high-frequency traders). 

The first common type of data problem is missing data, as we alluded to. Missing data occur when a piece of information existed in reality but for some reason was not provided by the data supplier. This is obviously an issue because without data, the system has nothing to go on. Worse still, by withholding just some portion of the data, systems can make erroneous computations. Two common approaches are used to solve the problem of missing data. The first is to build the system so that it “understands” that data can in fact go missing, in which case the system doesn’t act rashly when there are no data over some limited time period. For example, many databases automatically assign a value of zero to a data point that is missing. After all, zero and nothing have a lot in common. However, there is a very different implication to the model thinking the price is now zero (for example, if we were long the instrument, we’d be showing a 100 percent loss on the position) versus thinking that the price is unknown at the moment. 

To fix this problem, many quants program their database and trading systems to recognize the difference between zero and blank. This frequently means simply using the last known price until a new one is available. The second approach is to try to interpolate what a reasonable value might be in place of the missing data. This is particularly useful for historical data rather than real-time data, but a variation of the method described here can be used for real-time data as well. 

Let's take an example of a semiconductor company in stocks. Imagine that we know the price of a semiconductor stock immediately before and immediately after the missing data point (this is why this technique is mainly useful to back-fill missing data points in a database). We could simply interpolate the price of the stock as being midway between the price immediately before and immediately after the gap. Imagine further that we know how the stock index, the tech sector, the semiconductor industry, and some close competitors performed for the period that is missing. By combining information about the periods around the missing point and the action of related things during the missing period, it is possible to compute a sensible value for the stock's missing data point. Though we aren't guaranteed and in fact aren't terribly likely to get the number exactly right, at least we have something reasonable that won't cause our systems problems. 

A second type of data problem is the presence of incorrect values. For instance, decimal errors are a common problem. To take the example of U.K. stocks, they are sometimes quoted in pounds and sometimes in pence. Obviously, if a system is expecting to receive a figure in pounds and it receives a number that doesn't advertise itself as being anything other than pounds, problems can abound. Instead of being quoted as, say, £10, it is quoted as 1000, i.e., 1000 pence. This can result in the model being told that the price has spiked dramatically upward, which can cause all sorts of other mayhem. Alternatively, a price might simply be wrong. Exchanges and other sources of data frequently put out bad prints, which are data points that simply never happened at all or at least didn't happen the way the data source indicates. 

By far the most common type of tool used to help address this issue is something we call a spike filter. Spike filters look for abnormally large, sudden moves in prices and either smooth these out or eliminate them altogether. Further complicating the matter, it should be noted that sometimes spikes really do happen. In these circumstances, a spike filter may reject a value that is valid, either ignoring it or replacing it with an erroneous value. An interesting example of this is shown in Exhibit 8.1. In this case, during the trading day of July 15, 2008, the U.S. dollar's exchange rate with the Mexican peso quickly fell about 3 percent, then regained virtually all that ground in a matter of seconds. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/cc0a39e2570f977f3bc06e410b8a05486d2c0ec69845262939366d851d53c7d3.jpg)



EXHIBIT 8.1 September 2008 Mexican Peso Futures Contract on July 15, 2008


This behavior is not reserved for less commonly traded instruments, however. The 10-year German bund, one of the more liquid futures contracts in the world, dropped about 1.4 percent in a few seconds during the day of March 28, 2008, only to recover immediately (see Exhibit 8.2). 

A spike filter might well have called this a bad print, but it really happened. To reduce the impact of this problem, some quants use spike filters to alert a human supervisor to look into the matter further, and the human can then decide, based on what he sees as the facts, on what to do about the strange price. Still another common approach, though useful only if there is more than one source for a given piece of data, is to cross-check a data set given by one provider against one provided by a second source. If they match, it is more likely to be a correct price. If they do not match, one or both of them must be wrong. Of course, what to do when two vendors don't match each other is a whole other ball of wax. A final common approach to cleaning data problems is to utilize the same approach as described earlier in addressing the problem of missing data by looking to the points before and after the "bad" data point and/or by looking to the behavior of related instruments to interpolate an approximate value. 

Another very common type of data error relates to corporate actions such as splits and dividends. Imagine a ticker that splits 3:1. Generally, the price drops by about two-thirds to offset the threefold increase in the number of shares. $^{3}$ Imagine that the data vendor doesn't record this as a split, and therefore doesn't adjust the back-history to reflect this corporate action. In this scenario, the quant trader's system may be misled to believe that the stock simply dropped 67 percent overnight. This is generally handled by independently tracking corporate actions, together with the human-oversight version of a spike filter, described previously. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/eaa563a7ed20abdaa38d4c60710cbae406a710e68142296ad466a7a21c5eaf6d.jpg)



EXHIBIT 8.2 June 2008 German Bund Futures Contract on March 28, 2008


Another frustrating problem is that the data sometimes contain incorrect timestamps. This is generally a problem with intraday or real-time data, but it has been known to be an issue with other data as well. This is also one of the tougher problems to solve. Obviously, the path of a time series is fairly important, especially since the goal of the quant trader focused on alpha is to figure out when to be long, short, or out of a given security. As such, if the time series is shuffled because of an error in the data source, it can result in all sorts of problems. A quant researcher could believe his system works when in reality it doesn't, $^{4}$ or he could believe his system doesn't work when in reality it does. $^{5}$ If the quant trading firm stores its own data in real time, it can track timestamps received versus the internal clocks of the machines doing the storing and ensure that there are correct timestamps, which is perhaps the most effective way of addressing this issue. But to do so requires storing one's own data reliably in real time and writing software to check the timestamp of each and every data point against a system clock in a way that doesn't slow the system down too much, making this a difficult problem to address. 

Finally, a more subtle type of data challenge bears mentioning here. This is known as look-ahead bias and is a subject to which we will devote attention several times in this book. Look-ahead bias refers to the problem of wrongly assuming that you could have known something before it would have been possible to know it. Another way to phrase this is “getting yesterday’s news the day before yesterday.” We will examine look-ahead bias in the chapter on research, but for now, let’s examine a particular form of this bias that comes from the data. Specifically, it derives from asynchronicity in the data. 

A common example of asynchronicity can be found in the regulatory filings of financial statements (known as 10-Qs) made by companies each quarter in the United States. Companies report their financial statements as of each quarter end. However, these reports are usually released four to eight weeks after the end of the quarter. Let's imagine the first quarter of 2010 has just ended. On May 1, 2010, Acme Concrete Inc. reports that its first-quarter earnings were $1 per share as of March 31 and furthermore that the general analyst community was expecting only $0.50 per share, making the result a strongly positive surprise. Once the data point is available, most data vendors will report that Acme's earnings per share were $1 per share as of March 31, even though the number wasn't released until May 1. 

Three years later, a quant is testing a strategy that uses earnings data from this vendor. The data indicate that that Acme's earnings were $1 per share for the quarter ending March 31, and his model assumes this to be true, even though in reality he would never have been able to know this until the estimate was released a month later, on May 1. In the back-test, he sees that his model buys Acme in April because its P/E ratio looks appealing from April 1 onward, given the $1-per-share earnings result, even though the model would not have known about the $1 earnings figure until May 1 if he had been trading back then. Suddenly the strategy makes a huge profit on the position in early May, when the world, and his model, actually would have found out about the earnings surprise. This kind of problem also happens with macroeconomic data (such as the unemployment rate), which frequently get revised some months after their initial release. Without careful tracking of the revision history for such data, the quant can be left with the same issue as demonstrated in the equity example: believing that he could have had revised data in the past when in fact he would only have had the less accurate initial data release. 

If the quant ignores this data error, he can end up making a Type I error again: believing that his strategy is profitable and sound, even though it may in fact only look that way because he's made a substantial data error. To address look-ahead bias in the data, quants can record the date at which new information is actually made available and only make the data available for testing at the appropriate time. In addition, quants can put an artificial lag on the data they are concerned about so that the model's awareness of this information is delayed sufficiently to overcome the look-ahead bias issues. Note that look-ahead issues with regard to data are specific to research, which we will discuss further in the next chapter. In live trading, there is no such thing as look-ahead bias, and in fact quants would want all relevant data to be available to their systems as immediately as possible. 

Another type of look-ahead bias stemming from asynchronicity in the data is a result of the various closing times of markets around the world. The SPY (the ETF tracking the S&P 500) trades until 4:15 P.M., whereas the stocks that comprise the S&P 500 index stop trading at 4:00 P.M. European stock markets close from 11:00 A.M. to 12:00 P.M., New York time. Asian markets are already closed on a given day by the time New York opens. In many cases, the considerable impact that U.S. news and trading activity have on European or Asian markets cannot be felt until the next trading day. 

On Friday, October 10, 2008, for example, the Nikkei 225 fell more than 9 percent for the day. But it was already closed by the time New York opened. European markets closed down between 7 and 10 percent for the same day. At the time of Europe's closing, the S&P 500 was down about 6 percent for the day. Suddenly, however, just after 2:00 P.M. EST on the 10th, with two hours remaining in U.S. trading but the rest of the world already gone for the weekend, the S&P 500 rallied, closing down just over 1 percent. Monday the 13th was a market holiday in Japan. Europe tried to make up ground that Monday, with the key markets closing up over 11 percent but the U.S. market up "only" about 6 percent by midday in New 

York. However, by the end of the trading day, the U.S. market closed up over 11 percent as well, leaving the European markets behind again. The Nikkei reopened on the $14^{\text{th}}$ and ended up 14 percent. European markets closed up about 3 percent, whereas the U.S. market was down slightly by the end of its own trading day. Ignoring this kind of asynchronicity can be extremely problematic for analyses of closing price data because these closing prices occur at different times on the same day. 

These are but a few examples of the many subtle ways in which look-ahead bias seeps into the process of research and money management, even for discretionary traders. A key challenge for the quant is deciding how to manage this problem in its myriad forms. 

## STORING DATA

Databases are used to store collected data for later use, and they come in several varieties. The first type of database is known as the flat file. Flat files are two-dimensional databases, much like an ordinary spreadsheet. Flat file databases are loved for their leanness, because there is very little baggage or overhead to slow them down. It is a simple file structure that can be searched very easily, usually in a sequential manner (i.e., from the first row of data onward to the last). However, you can easily imagine that searching for a data point near the bottom row of a very large flat file with millions of rows may take rather a long time. To help with this problem, many quants use indexed flat files, which add an extra step but which can make searching large files easier. The index gives the computer a sort of “cheat sheet,” providing an algorithm to search large sets of data more intelligently than a sequential search. 

A second important type of data storage is a relational database. Relational databases allow for more complex relationships among the data set. For example, imagine that we want to keep track of stocks not just on their own but also as part of industry groups, as part of sectors, as part of broader indices for the countries of their domicile, and as part of the universe of stocks overall. This is a fairly routine thing to want to do. With flat files, we would have to construct these groups each as separate tables. This is fine if nothing ever changes with the constituents of each table. But in reality, every time there is a corporate action, a merger, or any other event that would cause us to want to modify the record for a single stock in any one of these tables, we have to remember to update all of them. Instead, in the world of relational databases, we can simply create a database table that contains attributes of each stock—for example, the industry, sector, market, and universe it is in. Given this table, we can simply manage the table of information for the stock itself and for its attributes. From there, the database will take care of the rest based on the established relationship. Though relational databases allow for powerful searches, they can also be slow and cumbersome because their searches can span many tables as well as the meta tables that establish the relationships among the data tables. 

An important type of relational database is known as a data cube, a label I have borrowed from Sudhir Chhikara, the former head of quantitative trading at Stark Investments. Data cubes force consistency into a relational database by keeping all the values for all the attributes of all instruments in a single, three-dimensional table. For a given date, then, all instruments would be listed in one axis of this table. A second axis would store all the values for a given attribute (e.g., closing price for that date) across the various instruments. The third axis would store other attributes (e.g., earnings per share as of that date). This method has the benefit of simplifying the relationships in a way that is rather useful. In other words, it hardwires certain relationships; furthermore, by keeping all attributes of each instrument available every day, there is no need to search for the last available data point for a given attribute and security. For every day, a data cube is created to store all the relevant data. This approach, too, has its potential disadvantages. Hardwiring the relationships leads to inflexibility, so if the nature of the relationships or the method of querying the data changes, it can be problematic. 

Each of these data storage approaches has advantages and disadvantages. It would be easy to make some assumptions and declare one the "best," but the reality is that the best technique is dependent on the problem that needs to be solved. Here, as in so many other parts of the black box, the quant's judgment determines success or failure. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/8239567fe7aae7d8d09faece03cf43072c6d7ffbe288b68a98b91bc1fa745064.jpg)



EXHIBIT 8.3 Schematic of the Black Box


## SUMMARY

In this chapter, we explained some of the basic concepts of data for use by quant trading systems. Though data are scarcely the most exciting part of a quant strategy, they are so integral and critical to everything quants do and inform so much of how to think about a given quant system that they are well worth understanding. 

Next we will dive into the research process as our final stop in the exploration of the black box (Exhibit 8.3). 

# Research

Everything should be made as simple as possible, but not simpler.
—Albert Einstein 

Research is the heart of quant trading. It is in large part because of a well-designed, rigorous, and tireless research program that the best quants earn their laurels. This chapter gives an overview of what research really means for black-box traders. It focuses mostly on research targeted at developing the alpha models of trading strategies. Research is also done with regard to risk models, transaction cost models, portfolio construction models, execution algorithms, and monitoring tools. Relevant research topics in these other areas will be mentioned as necessary, but the general principles from this section hold true throughout the black box. 

The purpose of research is to scrutinize a well-conceived investment strategy. A strategy is a long-term course of action designed to achieve an objective, usually success or victory. In most applied settings, strategies are chosen from a limitless number of alternatives. One can find interesting examples in nearly every field: curing cancer, a baseball game, a war, a court case, or financial planning. In each case, one has many choices of strategy; so how is one chosen? In the case of quant trading, a strategy is chosen based on research, which has its roots in the natural sciences. 

## BLUEPRINT FOR RESEARCH: THE SCIENTIFIC METHOD

A characteristic shared among well-behaved quants is their adherence to the scientific method in conducting research, which is of course the way science is done in every other field of study. This is critical because it forces rigor and discipline into the single most judgment-driven portion of the entire quant trading process. Without such rigor, quants could easily be led astray by wishful thinking and emotion rather than the logic and consistency that make scientists useful to the world in so many other disciplines. 

The scientific method begins with the scientist observing something in the world that might be explainable. Put differently, the scientist sees a pattern in her observations. For example, in most circumstances, if something is above the ground and is left unsupported, it falls towards the ground. Second, the scientist forms a theory to explain the observations. Sticking with the same theme in our examples, the scientist can theorize that there is something inherent in all things that cause them to move toward each other. This is better known as the theory of gravity. Third, the scientist must deduce consequences of the theory. If gravity exists, the orbits of planets should be predictable using the consequences of the theory of gravity. Fourth comes the all-important testing of the theory. But rather than looking to “prove” a theory, properly done science seeks to find the opposite of the consequences deduced, which would therefore disprove the theory. In the case of gravity, Newton’s theory was used to predict the existence of Neptune, based on motions in the orbit of Uranus that could not be explained by other then-known celestial bodies. But this success could at best provide support for Newton’s theory and could never actually prove it. Karl Popper, the eminent philosopher of science, labeled this technique falsification. A theory that has not yet been disproved can be accepted as true for the moment. But we can never be certain that the next observation we make of the theory will not falsify it. Indeed, Newton’s theory of gravity has never been “proven” and in fact was superseded by Einstein’s general relativity theory. The latter also has not been proven, and alternatives have been proposed to help explain problems (such as the accelerating expansion of the universe or the unexpectedly high velocities of stars in the outskirts of galaxies) that neither Newton’s laws nor Einstein’s relativity address in their current form. 

Looking at the markets, it is easy to see the parallels with the way quants conduct research. First, let's imagine that a quant researcher observes that the various markets go through phases in which they tend to rise for extended periods, followed by phases in which they tend to fall for awhile. She theorizes that a phenomenon called a trend exists, which, for whatever reason, causes the future performance of a market to be in the same direction as its recent historical performance. The consequence of this theory would be that she should be able to achieve a better-than-random forecast of how markets will perform, given only information on how these markets have performed before. So, she sets out to test the theory, and lo and behold, she finds that the evidence does not contradict her theory. Using some metric to define the historical trend (such as the moving average crossover example we used in Chapter 3), she sees that she can indeed forecast markets better than random chance is likely to allow. But she can never be sure. At best, she can have enough confidence that her tests were rigorous that she finds it worth risking some capital on the validity of this theory. 

One important distinction, however, exists between quants and scientists. Scientists conduct research for many purposes, including learning the truth that drives the natural world. In science, a good theory, one that is well supported by the evidence and is widely useful in a variety of practical applications (e.g., Einstein's relativity), does not require modification to continue to be valid. Quant researchers, by contrast, have no choice but to conduct ongoing research and to take every measure to ensure that their research output is prolific. This is because, though nature is relatively stable, the markets are not. Whether from regulatory changes, the changing whims of the aggregate psychology of investors and traders, the constant competition for alpha among traders, or whatever other phenomena, the markets are in fact highly dynamic processes. For this reason, quant traders must constantly research so that they can evolve with as much rigor and forethought as they used in developing their original strategies. 

## IDEA GENERATION

Ideally, quants follow the scientific method in their research. In this regard the development of theories (or theoretically sound approaches to data mining) is the first key step in the research process. We find four common sources of ideas to be observations of the markets, academic literature, migration, and lessons from the activities of discretionary traders. 

The main way that quants come up with their own ideas is by watching the markets. This approach most embodies the spirit of the scientific method. An excellent example comes from the history of the oldest of quant trading strategies: trend following in futures contracts. Richard Donchian is the father of trend following. He originally traded stocks, but in 1948, he created Futures, Inc., the first publicly held commodity fund. In December 1960, he published his philosophy toward trading in his newsletter, Commodity Trend Timing. $^{1}$ He observed that there are sweeping moves in many markets that folks tend to call bull or bear markets; he postulated that one could build a system that would detect that these trends had begun and then ride the wave. He translated his philosophy into the following strategy: If a given market's price is above the highest closing price over the past two weeks, buy that market. If its price goes below the lowest closing price over the past two weeks, sell that market short. In the meantime, hold whatever position you have in that market. Using this incredibly simple system, from 1950 to 

1970 he built a successful track record and spawned an industry that now manages tens of billions of dollars of client capital. 

The academic literature in quantitative finance, and finance more generally, is replete with papers on a massive array of topics of interest to quant researchers. For example, many finance papers have been written on clever ways in which corporate chief finance officers (CFOs) attempt to “fudge” their companies’ earnings and other financial figures to retain the confidence of shareholders. Quant firms have taken note, and several now have strategies in their arsenal that look for the kinds of behaviors described in the academic literature for trading opportunities. Many quant firms spend significant time scouring academic journals, working papers, and conference presentations to glean ideas that can be tested using the scientific method. Such a quant could find papers on topics such as the management of financial statements and could test ideas learned from these papers. Perhaps the most classic example of an academic paper that made massive waves in the quant trading community is Harry Markowitz’s paper, modestly entitled Portfolio Selection. As discussed in Chapter 6, in “Portfolio Selection,” Dr. Markowitz proposed an algorithm to compute the “optimal” portfolio using a technique called mean variance optimization. For all the research that has been done on portfolio construction over the decades since Dr. Markowitz’s paper was published, his technique and variants of it remain key tools in the toolbox of quant trading. Aside from the literature in finance, quants also frequently utilize the literature from other scientific fields—such as astronomy, physics, or psychology—for ideas that might be applicable to quant finance problems. 

Another common source of new ideas is via the migration of a researcher or portfolio manager from one quant shop to the next. Though many firms attempt to make this more difficult via noncompete and nondisclosure agreements, at some point the quant can usually take ideas from one place to another, and this is to be expected. Any rational quant would want to know what the competition are doing, particularly those who are successful. At least part of the attraction of a potential new hire who has worked elsewhere must be the prospect of learning about the activities, and maybe even some secrets, of competitors. There are countless examples of this sort of thing. Goldman Sachs gave birth to AQR's quantitative approach to global tactical asset allocation and global equity market-neutral trading. Richard Dennis trained a group of new traders called the Turtles, none of whom had any trading experience, in trend following as a social experiment and to settle a bet with his friend William Eckhardt. D. E. Shaw was created after its founder cut his teeth at Morgan Stanley's statistical arbitrage prop trading desk and has itself spawned several successful alumni, including Two Sigma and Highbridge's quantitative equity manager. In a fascinating case, Renaissance Technologies, famous for its ability to retain talent partly by having its researchers sign iron-clad noncompete agreements, once lost two of its researchers to Millennium Partners. Renaissance sued Millennium over the incident, and it turned out that the researchers had somehow managed not to sign the noncompete agreements while at Renaissance. Nonetheless, the traders were ultimately terminated by Millennium, who simply decided that retaining them was more trouble than it was worth. Sometimes, investors who have peeked behind the curtains as part of their assessment of a given quant shop, and then shared what they've seen with others, act as the carriers of ideas from one quant shop to the next. 

Finally, quants learn lessons from the behavior of successful discretionary traders. For example, an old adage among successful traders is, "Ride winners and cut losers." This idea can easily be formalized and tested and has come to be known as a stop-loss policy, which involves systematically realizing losses on positions that are not working out. There are many examples of quants working closely with successful discretionary traders in an attempt to codify aspects of the latter's behavior into a trading system. Not all are necessarily bound for success. Technical trader is the label applied to a trader who subjectively analyzes graphs of market prices and makes decisions based on "rules" about the implications of various shapes of such graphs. These shapes are given names such as a head and shoulders pattern or an upward triangle pattern. Many quant funds have come (and mostly gone) that have attempted to recreate such patterns into systematic trading rules. This could be because the idea itself is not based on valid theory, or it might be because the human version is ultimately less rule based, as one might like to believe, condemning a truly systematic implementation to be unsuccessful. However, even here valuable lessons can be learned: Not all successful traders have skill, and a helpful way to begin figuring out what really works and doesn't is to put an idea through the grinder of a research process and see if it's still alive at the end. 

## TESTING

The process of testing is central to research. At first glance, the most common version of this process looks fairly simple. First, build a model and train it on some subset of the data available (the in-sample period). Then test it on another subset of the data to see if it is profitable (the out-of-sample period). However, research is an activity that is fraught with peril. The researcher is constantly offered opportunities to forego rigor in favor of wishful thinking. In this section, we address some of the work and challenges inherent in the research process. 

## In-Sample Testing, a.k.a. Training

In quant trading, models are approximations of the world. They are used to predict the future using data as inputs. The first part of the testing process is to “train” a model by finding optimal parameters over an in-sample period. That sounds rather like a mouthful of marbles, so let’s walk through it term by term. 

Let's imagine that we want to test the idea that cheap stocks outperform expensive stocks. We even theorize that the metric we will use to define cheapness is the earnings yield (earnings/price), such that a higher earnings yield implies a cheaper stock. But what level of yield is sufficiently low to cause us to think that the stock will outperform? And what level of earnings yield is sufficiently high to imply that a stock is expensive and is likely to underperform? These levels are parameters. In general the parameters of a model are quantities that define some aspect of a model and can affect its performance. These are variables that can be set at whatever level one chooses, and by varying these levels, the model itself is altered and will provide different results. 

Imagine that you hire a consultant to help you buy the ideal “optimal” house. The consultant lists all the relevant variables that might factor into your decision, things like the size of the house, its condition at the time of purchase, and the location and school district. If you do not tell him the “perfect” levels for each of these variables, he can deduce them by observing your reaction to various houses. A big house in a poor neighborhood might generate a lukewarm reaction, whereas a smaller house in a good neighborhood might generate a higher degree of interest for you. In this way, the consultant can deduce that you dislike the first neighborhood and prefer the second, and furthermore that the neighborhood might be more important to you than the size of the house. If he is able to repeat these “experiments,” he can continue to fine-tune the choices he presents to you until he finds the house that matches your desires optimally. To the extent he succeeds in this endeavor, he has performed well. 

In this way, optimal parameters in a quant model are those that lead to the best performance based on whatever metrics one chooses to use to measure goodness. Training a model involves simply finding the optimal parameter set, which is usually accomplished by trying a number of them and hoping that at least one set comes out looking appealing. What constitutes appeal is a matter we will discuss in some detail forthwith, but first we consider some other aspects of in-sample research. 

In-sample research is, in a sense, fun for a quant. In the real world, the quant's model is constantly buffeted by new information and unpredictable events. But the historical data from the in-sample period are known to the model in their entirety, and nothing about them needs to be predicted. The in-sample period is like the answer key to a test in grade school. It is the model's best chance to work, because it doesn't have to predict anything. The model simply has to do a reasonable job of explaining the in-sample period after the fact, with the whole picture. This is the one part of the research process in which there is a high degree of hope. 

An important decision lies in the process of in-sample testing: What exactly constitutes the sample chosen for fitting the model? A sample is characterized by two things: its breadth and its length. Imagine that a researcher plans to build a strategy to trade the approximately 5000 listed U.S. stocks and that she has at her disposal data starting in 1990 and ending now. As far as breadth, the researcher must choose how many of the stocks to use and decide how to choose the ones that are used. Should she use a broad cross-section of stocks across sectors and capitalization levels? Should she use a narrower cross-section, or should she choose all the stocks? As to length of time, the researcher must consider what window of data will be available to use for fitting the model. Will it be the most recent data or the oldest data? Will it be a random set of smaller time windows or the entire set of data from 1990 onward? The most common preference among quants would be to use all the instruments for some subset of the time, but this is by no means universal, since there is a tradeoff here to consider. 

By using more data, the quant has a broader array of scenarios and market events that the model has to fit itself to, which can help make it more robust. By the time it has to succeed in real conditions, it has already “seen” and been adapted to the scenarios and environments found in the large in-sample period. On the other hand, the more data the model is allowed to see while it is being tuned, the greater the risk of creating a model that is nothing more than a good explanation of the past. For this reason, many quants utilize a reasonable cross-section of the data for the purpose of in-sample testing and model fitting. 

## What Constitutes a "Good" Model?

Quants utilize a wide variety of metrics to determine the “goodness” of a model. This is true for both the in-sample part of the process and the out-of-sample part of the process, the latter of which we will discuss in the next section. I include here a number of statistics (and other output) that quants may use. I illustrate these metrics using a strategy for forecasting the S&P 500. It has a one-day horizon for its forecast, and it uses an adjustment to a well-known idea known as the equity risk premium, which is calculated by taking the difference between the earnings yield of the S&P 500 and the 10-year Treasury note each day. If the S&P’s yield is higher than the bond’s, this is viewed as a signal to be long stocks. If the S&P's yield is lower than the bond's, this is a signal to be short stocks. I built this strategy back in the mid-1990s for tactical asset allocation purposes, but I have never traded it, for reasons that will be obvious after we assess it using these metrics. The results I show for the strategy are based on daily closing prices from June 1982 through December 2000. 

Graph of the Cumulative Profits Over Time A graph indicating the cumulative profits over time is one of the most powerful pieces of output in a testing process because, as they say, one picture is worth a thousand words. From a graph of cumulative profits, you can see whether the strategy would have made money, how smoothly, and with what sort of downside risk, just to name a few things. As you can see in Exhibit 9.1, the S&P strategy shows as being profitable over the test period, but it is a very “lumpy” return stream, characterized by long periods of inactivity (several years, in some cases), some sharp losses, and some very steep gains. Immediately a researcher can see that this strategy has some real problems. Is it realistic to want to sit on the sidelines making almost no trades, and certainly no profits, from late 1989 until early 1995? 

Average Rate of Return The average rate of return indicates how well the strategy actually worked (i.e., how much it might have made) in the past. If it didn't work in the testing phase, it's very unlikely to work in real life. As we will see later, testing offers many opportunities for the researcher to believe that making money in trading is a trivially easy exercise. Sadly, this misperception is mainly due to a wide variety of deadly traps. In our S&P 500 example, the total cumulative profits in the simulation were 746 percent, which comes to an average annual rate of return of 12.1 percent before any transaction costs or fees. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/5917af9dccec055796a0d36f941386916c27f348c135c97e753f3dfce9c29d65.jpg)



EXHIBIT 9.1 Back-Tested Cumulative Profits of the S&P 500 Strategy


Variability of Returns Over Time The variability of returns over time, which describes the uncertainty around the average returns, is helpful in deciding whether the strategy is worth owning. In general, the less the variability for a given level of returns, the better a strategy is considered to be. For example, if a strategy averages 20 percent returns per year, with an annual standard deviation of 2 percent (i.e., 67 percent of the time, the annual rate of return should fall within $+/-2$ percent of the average 20 percent figure, or between 18 and 22 percent), this would be a better outcome than if the same 20 percent average annual return came with 20 percent annual standard deviation (i.e., 67 percent of the time, returns are within 0 and 40 percent). The idea is that one can have more confidence in a given return if the uncertainty around it is low, and more confidence is a good thing. 

At my shop, we look at a statistic we dubbed lumpiness, which is the portion of a strategy's total return that comes from periods that are significantly above average. This is another way of measuring consistency of returns. Despite the importance of this metric, it is not always the case that consistency should be a primary goal. Nevertheless, it is good to know what to expect as an investor in or practitioner of a strategy, if for no other reason than to discern when the strategy's behavior is changing. In our S&P 500 strategy, the annualized standard deviation of its daily returns over the entire test period was 21.2 percent. 

Worst Peak-to-Valley Drawdown(s) This metric measures the maximum decline from any cumulative peak in the profit curve. If a strategy makes 10 percent, then declines 15 percent, then makes another 15 percent, the total compounded return for this period is about +7.5 percent. However, the peak-to-valley drawdown is -15 percent. Another way of stating this is that the investor had to risk 15 percent to make 7.5 percent. The lower the drawdown of a strategy, the better. Many quants measure not just one drawdown but several, to get a sense of both the extreme and more routine downside historical risks of their strategies. It is also typical to measure recovery times after drawdowns, which give the researcher a sense of the model's behavior after it's done poorly. Long recovery times are generally disliked because they imply that the strategy will remain in negative territory for quite a while if it does go into a large drawdown at some point. The S&P 500 strategy's worst peak-to-valley drawdown in the back-test was -39.7 percent, and it came from being short the S&P 500 in the summer of 1987, before the crash in October actually made that trade look good. 

Predictive Power A statistic known as the R-squared (R²) shows how much of the variability of the thing being predicted can be accounted for by the thing you're using to predict it, or, in other words, how much of the variability in the target is explained by the signal. Its value ranges from 0 to 1, and in general it can be computed simply by squaring the correlation coefficient. A value of 1 implies that the predictor is explaining 100 percent of the variability of the thing being predicted. In case it's not already clear, when we talk about "the thing being predicted," we are of course referring to a stock or a futures contract or some other financial instrument that we want to trade. In quant finance, since we're literally trying to predict the future prices of such instruments, a value of 1 is never seen unless methodological errors are being made. In fact, an excitingly high R² in our industry is usually 0.05 (out of sample, to be discussed later in this chapter). A former employee of mine once said, "If you see an R² above 0.15 and it's not because you made a mistake, run the other way, because the SEC will arrest you for insider trading if you use it." Note that an R² of 0.15 implies that some predictor describes 15 percent of the future volatility of the thing being forecast. As another quant trader put it, "People have gotten rich off a 0.02 R²." Exhibit 9.2 shows that the R² of the S&P 500 strategy was less than 0.01 from 1982 through 2000. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/018c2d5ef02d07a7fb84d4a1a6240b3333845327123d972cc5c9eaee0116f58e.jpg)



EXHIBIT 9.2 R² of the S&P 500 Strategy


Quants frequently utilize an additional approach to ascertaining predictive power. This approach involves bucketing the returns of the instruments included in the test by the deciles (or any other quantile preferred by the researcher) of the underlying forecasts. In general, a model with reliable predictive power is one that demonstrates that the worst returns are found in the bucket for which the worst returns are expected, with each successive bucket of improving expected returns in fact performing better than the prior bucket. If the returns of the instruments being forecast are not monotonically improving with the forecast of them, it could be an indication that the strategy is working purely by accident. 

A bar chart showing the quintile study for the S&P 500 strategy is shown in Exhibit 9.3. As you can see, in this study at least, the strategy looks reasonable. The leftmost bucket of signals averages -2.35 percent, and indeed, the S&P's average return on the day after such a signal is received is the worst of any of the buckets. The second bucket from the left shows that the S&P 500 strategy's second most bearish group of forecasts for the S&P averages -0.19 percent. As we move to increasingly bullish signals, the S&P's returns continue to improve in accordance with the bullishness of the forecasts, which is what one would hope for. The fact that each bucket's average return is better than the one previous to it is said to imply a monotonic relationship between our alpha signal (the modified equity risk premium signal described earlier) and the target of our forecasts (the S&P 500 index's return over the next day). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/6e525a59d62ff9e20719a21cda194264b6d707fc3cf0040a19bcfc546f2c9df7.jpg)



EXHIBIT 9.3 Quintile Study of S&P 500 Strategy's Signals vs. S&P 500 Returns


Percentage Winning Trades or Winning Time Periods This percentage is another measure of consistency. It tells the researcher whether the system tends to make its profits from a small portion of the trades that happened to do very well or from a large number of trades, each of which might contribute only modestly to the bottom line. Similarly, one can easily measure the total number of winning (positive) periods versus the total number of periods. (This is most often measured by percentage winning, or profitable, days.) In both cases, one tends to have more confidence in strategies with greater consistency. In the S&P strategy, the results of this study are somewhat unusual in that the strategy is not designed to produce a signal every day but instead only when the model perceives that the opportunity is sufficiently attractive to warrant trading at all. As such, the model produces a zero signal 65 percent of the time. It produces winning trades about 19 percent of the time and losing trades about 16 percent of the time. Of the days it actually has a nonzero signal, it wins approximately 54 percent of the time. This, too, is not a terrible outcome for a strategy. 

Various Ratios of Return versus Risk A great many statistics have been proposed as useful measures of risk-adjusted return, which are generally all attempts to measure the “cost” (in terms of risk) of achieving some return. The canonical example is the Sharpe ratio, named after William Sharpe (mentioned earlier in connection with the Nobel Prize in Economics he shared with Harry Markowitz in 1990). The Sharpe ratio is computed by taking the average periodic return above the risk-free rate and dividing this quantity by the periodic variability of returns. The higher the Sharpe ratio, the better. Quants (and many in the investment management business) have shortened this moniker by dropping the word ratio. A strategy with a 2 Sharpe is a strategy that delivers two percentage points of return (above the risk-free rate) for each point of variability (and this is a rather good Sharpe, if you can get it). 

A close cousin of the Sharpe ratio is the information ratio, which is different from the Sharpe only in that it eliminates the risk-free rate from the formula. The information ratio of the S&P 500 strategy is a mere 0.57 meaning that the investor receives 0.57 percent in return for every 1 percent in risk taken (again, before transaction costs and before any other fees or costs of implementing the strategy). The Sterling ratio (average return/variability of below-average returns), the Calmar ratio (average return/worst peak-to-valley drawdown), and the Omega ratio (the sum of all positive returns/the sum of all negative returns) are also widely used among a number of other risk-adjusted return metrics. The S&P 500 strategy from 1982 through 2000 displayed a Sterling ratio of 0.87, a Calmar ratio of 0.31, and an Omega ratio of 1.26. Of these ratios, the most discouraging is the low Calmar ratio, which indicates that the strategy generated only 0.31 percent in returns for every 1 percent of drawdown it experienced. 

Relationship with Other Strategies Many quants utilize several kinds of strategies at once. As such, the quant is effectively managing a portfolio of strategies, which can be thought of much like any other kind of portfolio in that diversification is desirable. As a result, the quant frequently measures how a proposed new idea will fit in with other, already utilized, ideas, to ensure that the new strategy is in fact adding value. After all, a good idea that doesn't improve a portfolio is not ultimately useful. Though it is common to compute a correlation coefficient between the new idea and the existing portfolio of strategies, many quants measure the value-added of a new strategy by comparing the results of the existing strategy with and without the new idea. A significant improvement in the results indicates that there is a synergistic relationship between the new idea and the existing strategy. 

Time Decay In testing a strategy, one interesting question to ask is, how sensitive is this strategy to getting information in a timely manner, and for how long is the forecast effect sustained in the marketplace? Many quants will seek to understand what their strategies' returns would be if they must initiate trades on a lagged basis after they receive a trading signal. In other words, if a strategy initiated a signal to sell Microsoft (MSFT) on April 28, 2006, the quant can see what the performance of his strategy would be in MSFT if it was not allowed to sell MSFT for one day, two days, three days, and so on. In this way, he can determine his strategy's sensitivity to the timeliness with which information is received, and he can also gain some information about how crowded the strategy is (because more crowding would mean sharper movements to a new equilibrium, i.e., faster degradation of profit potential). Imagine that a researcher develops a strategy to trade stocks in response to changes in recommendations by Wall Street analysts. Increases in the level of analysts' consensus recommendations for a company lead to a targeted long position in that company, whereas a deterioration in the aggregate recommendation level would lead to a targeted short position in the company. This strategy is popular and followed by many quants (and discretionary traders). However, its effects are very short-lived and are very sensitive to the timing of the information received. 

An example of this phenomenon is shown in Exhibit 9.4, using MSFT from April through October 2006. As you can see, there were five downgrades on April 28, which caused MSFT to underperform the S&P 500 by about 11.4 percent on the day the downgrades were announced. In fact, the opening price of MSFT on the $28^{\text{th}}$ was already down about 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/208b2475bb80516cf952a3cd805cdda0c75392ced98d302e70310eea3bcc1341.jpg)



EXHIBIT 9.4 Illustration of Time Decay of Alpha


11.1 percent because the downgrades all took place before the market opened. As such, the quant trader must be careful not to allow his simulation to assume that he was able to transact in MSFT early enough to capture any of the 11.1 percent change. Instead, to be conservative, he can test what his, say, two-week performance on the trade would have been if he initiated the trade on various days after the initial ratings change. 

If he did this, what he would find is that if he sold MSFT at any time after the close of April 27 (the night before the recommendation changes were announced), his trade would have actually been pretty mediocre. He would have made money selling MSFT on at the close on April 28, May 1 (the next business day), or May 2, but from May 3 through May 12 the trade would have been unprofitable. This illustrates the importance of stress-testing a strategy's dependence on timely information, which might not always be available. 

Interestingly, delaying the signal's implementation does not always result in a negative outcome. For example, our S&P strategy tends to be "early" on its trades, that is, it tends to be short too early and long too early, even though the market subsequently does move in the direction forecast, on average. As such, delaying its entry by merely one day dramatically improves the total return of the strategy, from 746 percent total (12.1 percent annualized) to 870 percent total (12.9 percent annualized). This does not necessarily bode well for the use of such a strategy. In general, it is not comforting to know that you get a signal from your trading strategy that you not only can go without implementing for a little while (which would be the better result) but that you actually are better off ignoring for at least a full day after you get the signal. 

Sensitivity to Specific Parameters It was mentioned earlier that parameters can be varied, and by varying them, differing outcomes are likely. But much can be learned about the quality of a strategy based on how much the outcomes vary based on small changes in the parameters. Let's use our P/E-based strategy from earlier as an example. Imagine that we think that any P/E ratio that is either above 50 or negative (because of negative earnings) should be considered expensive. Meanwhile, we presume that any P/E ratio below 12 is cheap. Assume we test the strategy according to the previously discussed metrics and find that a low P/E strategy with these parameters ( $\geq 50$ implies expensive, $\leq 12$ implies cheap) delivers a 10 percent annual return and 15 percent annual variability. 

Now imagine that we vary the parameters only slightly so that any stock with a P/E ratio below 11 is cheap and any with a P/E ratio that is negative or above 49 is expensive. If this version of the strategy, with slightly differing parameters, results in a significantly different outcome than the first example, we should mistrust both results and use neither in our model. This is because the model has proven to be overly sensitive to a small change in the values of the parameters, which makes little real-world sense. Should there be any great difference between a 10 P/E and an 11 P/E, or between a 50 P/E and a 49 P/E? What many researchers look for is smoothness of the goodness of outcomes with respect to parameter values. Near-neighboring sets of parameters should result in fairly similar results, and if they don't, a researcher should be a bit suspicious about them, because such results may indicate overfitting. 

## Overfitting

## Consider Exhibit 9.5.

Which of these points would you guess is the best choice for a parameter value? Choice A doesn't look so good, because the strategy seems to do poorly when using such a parameter value. Choice C looks enticing because it is the highest point of a broad plateau. But it is so near a cliff's edge that we cannot be sure whether we're at risk of picking unwisely. Choice D seems to have the best outcome, but it is also fairly unreliable, since its near neighbors are universally poor. This leaves Choice B as the best. Even though we haven't picked the highest point on the plateau, we've picked one with a margin of safety around it on both sides. It bears discussing a bit about why this margin of safety is so important. 


Outcome as a Function of Parameter Value


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/21e57c5339d4325a9ed37e22671d93d85295cee6f3977509e3312547505b412a.jpg)



EXHIBIT 9.5 Choosing the Right Parameter Values


When we see a lonely peak like the one represented by Point D in Exhibit 9.5, it is likely that our testing has uncovered some spurious coincidence in the fitting period that makes it especially favorable for that single parameter value. Unfortunately, it is likely that this coincidence will not persist into the future. By selecting Point D, in other words, we are implicitly betting that the future will look exactly like the past. You might be familiar with the standard performance disclaimer: "Past performance is not an indication of future results." Yet we all tend to judge the success of a trader at least partly by performance, which is a way of saying that we think the past might actually be some indication of the future. Similarly, and based on the premises of scientific research in general, all quant trading (and indeed, all science) assumes implicitly that the past can have some value in helping us understand the future. This is why the scientific method starts with observations of the world that can be generalized into a theory. But the appropriate way to think about the past is as a general guide to the future, not as an exact copy. Quants would refer to Point B as being more "robust" than Point D because Point B has a better chance of being good, but not solely as a result of some accident of the sample data used to find it. Any model that explains the past well but is so closely modeled to it that it might be useless for predicting the future has a problem known as overfitting, an issue that we will discuss further in Chapter 11. 

The previously described metrics represent a sampling of the kinds that quants use to determine whether a given model is good. These metrics are used to judge the quality of a model, both while it is being created and when it is being used. Indeed, many hedge fund investors look at the majority of these metrics as ways of gauging the performance of various traders. 

There remains, however, one more extremely important guiding principle in determining the goodness of a quant strategy, and this is known as parsimony. Parsimony is derived from the Latin word parsimonia, meaning sparingness and frugality. Among quants, parsimony implies caution in arriving at a hypothesis. This concept is absolutely central to the research process in quant trading. Models that are parsimonious utilize as few assumptions and as much simplicity as possible in attempting to explain the future. As such, models with large numbers of parameters or trading signals are generally to be viewed with skepticism, especially given the risks of overfitting. 

Parsimony has its roots in a famous principle of a Franciscan friar and logician, William of Occam, known as Occam's razor. Occam's razor is roughly translated from the original Latin as follows: Entities must not be multiplied beyond necessity. In science, this has been understood to mean that it is better to use as few assumptions, and as simple a theory, as possible to explain the observations. Karl Popper pointed out in 1992 that simpler theories are better because they are more easily tested, which means that they contain more empirical value. All around, scientists agree that parsimony, the stripping away of unnecessary assumptions and complexity, is simply better science. Einstein's saying, quoted at the beginning of this chapter, adds an important caveat, which is that oversimplifying an explanation is not helpful either. Looking again at our example of the consultant hired to help you buy a house, if he adds a large number of factors to the mix, such as the color of the guest bathroom tiles or the type of roofing material, given that there is no reason to believe ex ante that such factors are top priorities for you as his client, his analysis would become muddled and confused. But if he uses only two factors, the size of the house and its school district, though both of these may be important, this model might not do a good job of predicting your preferences. Similarly, an important part of the quant researcher's job is balancing on the tightrope between trying to explain the past too perfectly and trying to explain it too little. To one side is failure due to overcomplicating the model and to the other is failure due to oversimplifying it. 

Quant researchers must evaluate the theories they are testing. This is done using a wide array of measurements and techniques, but ultimately, a significant amount of discretion is used. It is unquestionably the case that what separates a successful researcher from the rest is good judgment about the kinds of issues raised in this chapter. As a general principle, we may note that good researchers must possess sufficient confidence and skill to believe that theories can be developed or improved on. At least as important, researchers must also be skeptical and humble enough to know, and be entirely at peace with the fact, that most ideas simply don't work. 

## Out-of-Sample Testing

Out-of-sample testing, the second half of the testing process, is designed to tell the researcher whether her formalized theory actually works in real life, without the benefit of seeing the “cheat sheet” provided during in-sample testing. The model’s parameters have by now been fixed using a different set of data (from the in-sample testing period), and it’s simply a question of whether the parameters really work in an environment that the model has not seen before or, in other words, in a new, “out-of-sample” data set. Many of the same kinds of statistics as described in in this chapter are utilized to make this judgment. 

One additional statistic many quants use is the ratio of the $R^{2}$ in the out-of-sample test to the $R^{2}$ in the in-sample test. This ratio is another way for the researcher to obtain a sense of the robustness of the model. If the out-of-sample $R^{2}$ is relatively close to the in-sample $R^{2}$ (i.e., if the ratio is about half or better), that is considered a good thing. If it is significantly smaller, the researcher must be suspicious about the prospects for his model's success. 

There are many approaches to out-of-sample testing. The simplest utilizes all the data that was set aside from the in-sample test. Some researchers utilize a rolling out-of-sample technique in which the single oldest data point is discarded and one new data point is added to both the fitting (in-sample) and testing (out-of-sample) period. This process is repeated through the entire available sample of data. The rolling out-of-sample technique is thought to help refresh the model over time so that it does not depend on a single set of tests that might have been run some years previously. However, depending on the circumstances, this approach can have the weakness of giving the model the benefit of constant knowledge of the recent past, which could reduce its robustness. This tradeoff is extremely subtle and can be debated in any individual instance, rendering impractical any general judgment about its effectiveness. Still another approach utilizes an ever-growing window of data for ongoing out-of-sample testing as time passes and more data is collected. 

Though the objective of out-of-sample testing is clearly a valid and necessary component of research, it turns out to be a rather tricky thing to do correctly. Imagine a researcher who completes the model fitting over the in-sample data. Then, having a model that seems robust, the researcher tests it over the out-of-sample data. But the model fails to deliver a good result on this new data set. The researcher, already having invested a lot of time on the model, decides to examine the reasons for the model's failure over the out-of-sample period and discovers that the environment changed between the in- and out-of-sample periods in such a way that the model was making losing trades during the latter. Having learned a useful lesson, the researcher goes back to the model and alters it to account for this new information. He refits the model in sample, and then retests it out of sample. And, lo and behold, it works much better. 

Before we break out the champagne, however, we should consider what the researcher has just done. By learning from the out-of-sample data and using that information to train the model anew, he has effectively used up his out-of-sample data and has caused them effectively to become part of the in-sample data set. In general, going back and forth between the in- and out-of-sample data is a terrible idea. This brings up a still more subtle issue, but one that is closely related. 

Often we know enough about that happens in the capital markets during the out-of-sample period that we tend to build models and select parameter sets that we believe are likely to work out of sample anyway. This sullies the purpose of an out-of-sample test because we are, in many respects, looking ahead. For example, we can look back on the Internet bubble of the late 1990s and know that the world and the economy in fact did not change and that negative earnings should not be wildly rewarded in the long run. If we build a strategy today, we can know that it is possible for the Internet bubble to happen but that it eventually bursts. However, we could not have known this with certainty in 1999. 

The world finds new and interesting ways to confound our understanding. As such, to test our current best thinking against competition that existed in the past is a form of wishful thinking. This is a subtle and nefarious form of look-ahead bias, which is a critical problem in research. As researchers become more and more familiar with the out-of-sample periods they use to test their ideas' validity, it becomes more likely that they are implicitly assuming they would have known more about the future than in fact they would have known had they been asking the same questions historically. This practice is called burning data by some quants. 

To mitigate the data-burning form of look-ahead bias, some quant shops take reasonably drastic measures, separating the strategy research function from the strategy selection function and withholding a significant portion of the entire database from the researchers. In this way, the researcher, in theory, cannot even see what data he has and doesn't have, making it much more difficult for him to engage in look-ahead activities. Less draconian, the researcher might simply not be allowed to know or see what data are used for the out-of-sample period, or the portions of data used for in- and out-of-sample testing might be varied randomly or without informing the researcher. Regardless, as you can easily see, the problem of doing testing is tricky and requires great forethought if there is to be any hope of success. 

## Assumptions of Testing

Another component in the testing process revolves around the assumptions one makes about trading a strategy that is being tested historically. We discuss two examples here: transaction costs and (for equity market-neutral or long/short strategies) short availability. 

We have already discussed transaction costs, of which there are several components: commissions and fees, slippage, and market impact. Interestingly, during the research process there is no empirical evidence of what a trading strategy would actually have cost to implement in the past. This is because the trading strategy wasn't actually active in the past but is being researched in the present using historical market data. Therefore, the researcher must make some assumption(s) about how much his order would really have cost in terms of market impact. 

These assumptions can prove critical in determining whether a strategy is good or bad. Let's again look at an extreme case to understand why. Imagine that we assume that transactions are entirely costless. This might make a very high-frequency trading strategy extremely appealing because, as long as it accurately predicts any movement in price, no matter how small, it will seem to have been worthwhile to trade. Imagine that a model is correct 55 percent of the time and makes $0.01 per share when it is correct. It loses 45 percent of the time and loses $0.01 per share when it is wrong. So, for every 100 shares it trades, it could be expected to generate $0.10. But when it is implemented, it turns out that transactions actually cost $0.01 per share across all the components of cost, on average. This would imply that the strategy is actually breakeven on 55 percent of its trades (theoretical profit of $0.01 per share, less the cost of transacting each share of $0.01) and loses $0.02 per share on 45 percent of its trades. 

As a result, rather than making $0.10 per 100 shares, it is in fact losing $0.90, which is obviously a poor outcome. Stated generally, overestimating transaction costs will cause a quant to hold positions for longer than is likely optimal, whereas underestimating transaction costs will cause a quant to turn over his portfolio too quickly and therefore to bleed from the excess costs of transactions. If we have to err in this regard, it makes more sense to overestimate cost than to underestimate, but it is always preferable to get the cost-estimation approximately right. 

The second kind of assumption a quant must make in testing a market-neutral or long/short strategy in equities relates to the availability of short positions. Imagine a U.S. market-neutral quant trader who, by design, holds a short portfolio that is roughly equal in size to the long portfolio. Over time, the short portfolio adds a significant amount of value by finding overpriced stocks and by making money when the stock market tumbles, thereby reducing the risk inherent in the strategy. However, it turns out that the names the strategy wants to short, and in particular, the most successful short picks, are on hard-to-borrow lists. Hard-to-borrow lists are those stocks that are generally restricted from shorting by the broker, because the broker cannot mechanically locate shares to borrow, which is required in the act of shorting. If the shares cannot be located, the trade would be considered a naked short sale, which is illegal in the United States. Therefore, the trade wouldn't have been executed as expected by the back-test. If the model is ignorant of hard-to-borrow issues (and making a model aware of this issue in the past is not trivial, since such historical data is hard to come by), the researcher can easily be fooled into thinking that the short portfolio will be able to deliver value that is, in reality, nonexistent. This is because when he goes to implement the live portfolio, he finds that he is unable to put on the best short trades and is forced to replace these with inferior short trades instead. 

## SUMMARY

We have only scratched the surface of the work that a quant must do in research, and must do well, to succeed over time. Research is a highly sensitive area within the quant's process. It is where her judgment is most obviously and significantly impactful. Researchers must therefore go about their research with great care because this is the formative stage of a strategy's life. Mistakes made during research become baked into a strategy for its lifetime, and then the systematic implementation of this error can become devastating. Moreover, the research effort is not a one-time affair. Rather, the quant must continually conduct a vigorous and prolific research program to produce profits consistently over time. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/38df256e6fecde2951c52a9e57ef5e74d3605548963c554430a88b5ab2b89f8d.jpg)



EXHIBIT 9.6 Schematic of the Black Box


We have now completed our tour through the black box (see Exhibit 9.6), both its component models and the key elements—data and research—that drive it. The coming chapters will focus on the evaluation of quant traders and their strategies. 

Three 

# A Practical Guide for Investors in Quantitative Strategies

# Risks Inherent to Quant Strategies

Torture numbers, and they'll confess to anything. 

—Gregg Easterbrook 

We have defined two broad classes of exposures: those that generate returns in the long run (alpha and beta) and are intentionally accepted and those that do not generate long-term returns (risks) or are incidental to the strategy. For the kind of quant traders that are the subject of this book, beta exposures are generally avoided (because they can be easily obtained by generic, low-cost index instruments), and therefore we can focus on alpha and risk exposures. 

As we have already stressed, the kinds of alpha exposures quants seek to capture are generally exactly the same as those that are sought by discretionary managers. However, with any strategy there is always the possibility that the exposure from which returns are generated is not being rewarded by the marketplace at a given point in time. This risk of “out-of-favor” exposure is shared by both quants and discretionary traders alike. 

This chapter will help an investor understand the types of risks that are either unique to quant trading or at least more applicable to quant trading. In a sense, we also are providing a framework for investors to design their own risk models that can be used to help determine how to use quant trading as part of a portfolio of strategies. The latter is a topic we will address again in Chapter 12. 

## MODEL RISK

Model risk is the most basic form of risk any quant system brings to an investor. Models are approximations of the real world. If the researcher does a poor job of modeling a particular phenomenon—for example, momentum—the strategy might not be profitable, even in a benign environment for momentum in general. In other words, model risk is the risk that the strategy does not accurately describe, match, or predict the real-world phenomenon it is attempting to exploit. Worse still, model risk need not be evident right away. Sometimes small errors in specification or software engineering lead to problems that accumulate very slowly over time, then suddenly explode on a busy trading day. Additionally, model risk can come from several sources. The most common are the inapplicability of modeling, model misspecification, and implementation errors. It bears mentioning that all types of model risk can occur not only in the alpha model but also from errors in any of the other parts of the strategy. Back-testing software, data feed handlers, alpha models, risk models, transaction cost models, portfolio construction models, and execution algorithms can all have model risk in them. 

## Inapplicability of Modeling

Inapplicability of modeling is a fundamental error that comes in two forms. The first is the mistaken use of quantitative modeling to a given problem. For example, trying to model the quality of a musician is simply the wrong idea from the start. One could conceive of some relevant factors that correlate with skill in musicianship, such as the source and duration of training. But ultimately, the goodness of a musician is not a question that can be answered with mathematics or computer models. It is an inherently subjective question, and to apply computer models to it is an error. 

Mathematical models can lull practitioners into feeling safe because of the precision of their computations. But this feeling is illusory. Indeed, one of the most important tasks of any quant is to sort out what questions he can actually ask using historical data and computer models. The global market turmoil in 2008, which was fueled in part by the securitized mortgage business, could be an example of the problem of the inapplicability of quantitative modeling to a problem. Though these securitized mortgages were not in any way like quant trading strategies, part of their rise to prominence owed to the quantitative modeling work done by various structured products desks at a wide variety of banks around the world. They modeled what would happen in various scenarios, and on the back of the comfort gained in the output of these models, they issued AAA-rated bonds backed by instruments that, each on its own, were toxic. It appears that a fundamental error was made (or ignored to rationalize massive greed) in the conceptualization of the problem. 

A second type of inapplicability is subtler and, probably because of this subtlety, more common among quant traders. It is the error of misapplication of an otherwise valid technique to a given problem. One example of this type of error, which we have already touched on in the section on risk modeling, is the widespread use of value at risk (VaR). VaR uses correlation matrices and historical volatility to determine the amount of risk in a given portfolio at a point in time. However, there are many assumptions inherent in the use of VaR that are invalid. For example, the use of both correlation matrices and historical volatility (defined as the standard deviation of returns) assumes that the underlying distributions that describe the various elements in a portfolio are normal. But in fact, market data often exhibits fat tails. In other words, there are significantly more observations of extreme values than one would expect from a normal bell-curve distribution. A specific example of this situation can be seen with data on the S&P 500. Based on the daily historical index data (excluding dividends) from January 3, 2000 through November 30, 2008, a -4 standard deviation day is one on which the S&P posts a return worse than -5.35 percent. A 4 standard deviation event should occur once every 33,333 trading days (approximately every 128 years, assuming 260 trading days per year) if the S&P's returns are normally distributed. In fact, the S&P has posted a return this poor on average once per 13 months, or 119 times more frequently than you'd be led to believe from a normal distribution. 

Furthermore, correlation coefficients (a key ingredient in the computation of VaR measurements) should be used only when a linear relationship exists between the two things being correlated. Instead, many instruments are not linearly related to each other. Exhibit 10.1 shows an interesting contrast between two relationships. 

As you can see from the charts, the relationship between XOM and JAVA is not linear. Note that the best day for XOM is actually a fairly poor day (-5 percent or so) for JAVA. Likewise, the best day for JAVA is also a nearly -5 percent loss for XOM. A line that best fits this relationship would look more like the Gateway Arch in St. Louis than a straight line. By contrast, the relationship between XOM and CVX does appear to be reasonably linear. A researcher using correlation to examine the relationship between JAVA and XOM would likely be making a model inapplicability error because the relationship is nonlinear in the first place. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/b89ce6e6a6e43cd5dab3dda2c11d64dcbb93059dd32c7c2b704bbf758bb45d72.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/f9cb31790ca7d34a1882fe5d32e82d28d7771c6eb5f6a7e85c4beb8ff199dcd7.jpg)



EXHIBIT 10.1 A Demonstration of Nonlinear and Linear Relationships


## Model Misspecification

The second kind of model risk is misspecification. Model misspecification basically means that the researcher has built a model that badly describes the real world. Practically speaking, a model that doesn't fit the real world at all is unlikely ever to make money and therefore is unlikely to be observable for very long before being shut down. As such, the more prevalent misspecification errors relate to events that are uncommon. These models work fine most of the time, but they fail when an extreme event occurs. A recent example of this situation can be seen in the aftermath of August 2007, when many quants concluded that they had done a bad job of modeling liquidity risk in large capitalization U.S. stocks. This is because they looked at only the liquidity risk associated with their own holdings in these names. What they learned, however, was that if many large traders liquidate similar holdings at the same time, the aggregate size of these positions matters more than the size any individual trader holds. 

As a direct result of this event, some quants discovered risk model or transaction cost model misspecifications and have begun to attempt to correct these flaws. But again, the rarity and unique nature of such events makes them extremely difficult to model. 

## Implementation Errors

The third and perhaps most common variety of model risk is from errors in implementation. All quant trading strategies ultimately are pieces of software residing in hardware and network architectures. Implementation errors, or errors in programming or architecting systems, can cause serious risk for the quant trader. For example, imagine that a quant means to have his execution software buy the bid and sell the offer price using limit orders. But he programs his execution software with the signs reversed so that it buys at the offer and sells at the bid. Because of this error, he is now paying the bid/offer spread on every trade—the exact reverse of his intention. This is an example of a programming error. 

Or, for instance, one successful quant trading firm made an architectural error. The firm has separate servers for alpha models and the execution engine (we'll ignore the other pieces, such as risk models and portfolio construction models, because they are irrelevant at the moment). As we discussed earlier, the portfolio construction model looks to the alpha model for information on what positions it should execute on both the long and short sides. At some point during one trading day, there was a need to reboot the servers for the system. But when the servers were restarted, the execution server came online first, and a few minutes later, the alpha model was restored to service. The execution model, seeing that it had no signals whatsoever from the alpha model, rapidly and automatically began liquidating the portfolio of positions in order to eliminate risk. In the few moments before the alpha server came back online, 80 percent of the firm's portfolio was sold off and then had to be reacquired again. There was no warning that this error existed until it manifested itself in this unfortunate manner. The strategy was making perfectly good returns but suddenly broke down due to a combination of a specific quirky error and the circumstances of the situation. Given the massive quantities of code that go into a quant trading strategy, such software and architectural errors are unfortunately the most common, but usually least painful, types of errors. 

## REGIME CHANGE RISK

Most quant models are based on historical data. Even those using analysts' forecasts or other "sentiment" signals turn out to depend heavily on the past because sentiment usually is biased in the direction of historical trends. Regardless of the type of model, quants use past relationships and behavior to develop theories and build models to help predict the future. If markets have behaved in a particular way for awhile, quants will come to depend on that behavior persisting. If there is a regime change, the quant will typically suffer because the relationships and behavior he is counting on are altered, at least temporarily. 

Dependence on the past is certainly one of the more interesting problems to consider in analyzing quant strategies and determining how to use them. In some cases, dependence on the persistence of historical behavior is blatant, as in the case of trend-following strategies. Note that this isn't necessarily an indictment of these strategies. Indeed, such strategies have made money for decades and have exhibited better risk-adjusted returns than the stock market by far. However, if an established trend reverses, the trend follower will almost certainly lose money. Ironically, mean reversion-focused quants may also suffer during a large trend reversal, particularly if they are engaged in a relative mean reversion strategy. We might expect that if a reversal of trend occurs, this should be good for the mean reversion trader, since he bets against trends. However, if the reversal is also associated with the breakdown of established relationships, this can be quite painful because of the relative part of the strategy. Exhibit 10.2 illustrates this point. 

As you can see, there are four distinct phases in the relationship between Charles Schwab (SCHW) and Merrill Lynch (MER). From early 1996 until the end of 1997, the stocks were reasonably correlated and showed similar trends. From early 1998 until early 2001, on the other hand, the stocks behaved very differently from one another, and SCHW in particular began to exhibit substantially greater volatility than it had earlier or than it would again later. The Internet bubble appears to be the cause of this shift, during which investors began to treat SCHW as an online broker, and its shares rose and fell with the likes of Ameritrade and E*Trade instead of its more traditional peer, MER. Upon the bursting of the Internet bubble, SCHW reverted uncannily to MER's level and tracked it very closely for some time, from early 2001 until early 2007. Then, in early 2007, you can see another sharp change in the relationship, with MER dramatically underperforming SCHW. This, of course, is due to the banking and credit crisis that traces its roots to early 2007. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/5c9f0b156125e01c65d0824d49f948f7584714ce5ed6ccd72629630da0d761a8.jpg)



EXHIBIT 10.2 Regime Changes in a Relationship between Two Stocks


A quant betting on this relationship's persistence would have suffered through two reasonably significant periods in the past 10 years in which the relationship did not hold up at all. Whether these stocks have permanently decoupled or will revert again at some point in the future is a matter that is beyond my ability to forecast. But this is precisely what regime change risk is about: A structural shift in the markets causes historical behavior of an instrument or the relationships between instruments to change dramatically and quickly. 

Another example of this kind of structural shift can be seen in the relationship between “value” stocks and “growth” stocks, as measured by the IVE and IVW ETFs, which represent S&P 500 Value and S&P 500 Growth, respectively. The historical spread between these two ETFs is illustrated in Exhibit 10.3. 

This figure shows that the S&P Value index outperformed the S&P Growth index by some 29 percent from the start of 2004 until mid-May 2007. The spread then trended a bit lower until mid-July and then rapidly fell as quants unwound their portfolios, which clearly had been betting on Value to outperform Growth. This unwind, combined with the macroeconomic environment, $^{1}$ set off a massive rebound in Growth relative to Value. 

Note that there are two substantial, short-term reversals of this more recent trend, one in January 2008 and one in July through September 2008, both of which are circled in the figure. These moves are incredibly sharp, actually representing the biggest and fastest moves in this spread in a very long time (certainly going back further than this analysis). In 16 trading days, from January 9 through 31 of 2008, the Value index recovered more than half the underperformance it had experienced in the 160 trading days prior to that point. In other words, the reversal was five times faster than the trend that preceded it. This was another rather painful experience for quants, though not on the order of what was felt in the summer of 2007. Over the subsequent 115 trading days, the Value/Growth spread reversed over 22 percent, all the way back to breakeven, until mid-July 2008. At that point, another brief but violent six-trading-day period saw the spread recover almost 40 percent of the lost ground. In other words, the reversal was almost eight times faster than the trend that preceded it. From late August through early September, the spread recovered another 36 percent of its lost ground, and over the 39-day period from mid-July through early September the recovery was more than 50 percent in total. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/e06499acc84e00194b8b9ba861879643dd92282bad6c543484fac72ad195624a.jpg)



EXHIBIT 10.3 Value/Growth Spread, 2003–2008


What's worse, such sharp reversals frequently cause many other types of relationships to falter. For example, the sectors that had been underperforming (such as financial companies or homebuilders) become the new outperformers, while those that had been outperforming (such as technology companies) tend to become the new laggards. Currencies and bonds also tend to reverse, as do commodities (especially over the past five years). An illustration of this last point is shown in Exhibit 10.4. 

Note that the OIL ETF moves as almost the mirror image of the Value/Growth spread, experiencing mirroring reversals in early January and mid-July 2008 (again, indicated by the circled periods on the graph) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/4a5c34b336db2f91913af2dff4ecf646962b533fb4974bb219b5b899d4f9771c.jpg)



EXHIBIT 10.4 Value/Growth Spreads versus Oil Prices, Normalized to August 16, 2006


and mirroring trends in between. It is for this reason that regime changes are especially painful for quants: They tend to occur across many levels simultaneously. 

## EXOGENOUS SHOCK RISK

The third in the family of quant-specific risks comes from exogenous shocks. I refer to them as exogenous because they are typically driven by information that is not internal to the market. Terrorist attacks, the beginning of a new war, and regulatory intervention are all examples of exogenous shocks. Because quant models utilize market data to generate their forecasts, when nonmarket information begins to drive prices, quant strategies typically suffer. This is especially true because such shocks usually also result in larger-than-normal moves. So, in situations of exogenous shock, we have big moves that aren't explainable by a reasonable model using market data but rather by information that is entirely external to the markets (see Exhibit 10.5). 

The first circled period in the S&P 500 chart in Exhibit 10.5 represents the terrorist attacks on New York and Washington, D.C., on September 11, 2001. The market was closed for almost a week, and when it reopened, it dropped precipitously, only to recover much of that ground rather quickly. Ignoring the obviously horrible nature of the attack on civilians, the downward move in markets was actually a continuation of the downward trend in stocks that had begun in March 2000 and therefore benefited trend-following strategies. However, many mean reversion strategies and relative-alpha strategies suffered in September 2001 as nonmarket information dramatically and briefly changed the way markets behaved. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/9e582a1350a2bf37168f393fe1423b794d90598be20267e26d562d694a6fc673.jpg)



EXHIBIT 10.5 S&P 500 Price Index, December 1999–December 2008


A similarly difficult situation was observable with the start of the Iraq war in early 2003, which is the second circled period. Suddenly global stock, bond, currency, and commodity markets began moving in lockstep with each other, all driven by news reports of the U.S. armed forces' progress through Iraq. This, too, resulted in losses for many quants, including trend followers, since the move resulted in a reversal of the prior trend across several asset classes simultaneously. 

The third circled period follows the bailout of Bear Stearns in mid-March 2008. This period was negative for many quant strategies because it was a sharp trend reversal that was caused by information that could not be anticipated by machines. Indeed, even the collapse of Bear might well have been the result of nonmarket “information,” and as of this writing, the SEC is supposed to be investigating potential wrongdoing in the rumors that were spread about Bear just in advance of (and which likely contributed to) its collapse. 

The final circled period represents another rally in the financial sector in equities, this one set off by the SEC's change in shorting rules, which made it much harder to short battered financial stocks. Though one can argue about whether an SEC intervention or a rumor-based collapse and government-brokered buyout of a major financial institution are endogenous or exogenous to the market, it is unassailably true that the kind of information these events presented to market participants was both unquantifiable and unusual. As such, exogenous shock risk is a significant byproduct of quant investing, one that it is difficult to do anything about (other than with discretionary overrides). 

## CONTAGION, OR COMMON INVESTOR, RISK

The newest member of the quant-specific risk family is contagion, or common investor, risk. By this we mean that we experience risk not because of the strategy itself but because other investors hold the same strategies. In many cases the other investors hold these strategies as part of a portfolio that contains other investments that tend to blow up periodically. The first part of this risk factor relates to how crowded the quant strategy in question is. 

A second part relates to what else is held by other investors that could force them to exit the quant strategy in a panic, sometimes called the ATM effect. In an ATM effect, significant losses in one strategy cause liquidation of a different, totally unrelated strategy. This happens because investors who have exposures to both, especially if highly levered, reduce their liquid holdings in the face of financial distress and margin calls, since their illiquid holdings are usually impossible to sell at such times. In essence, the good, liquid strategy is exited to raise cash to cover the losses of the bad, illiquid strategy. 

This is a particularly challenging type of risk that is certainly not exclusive to quants. However, the clarity with which this risk expressed itself in both August 1998 (easily argued not to be a quant event) and August 2007 (clearly a quant event) demands specific attention. In August 1998, it was not quant trading that suffered but other strategies such as merger arbitrage. We will discuss both of these events in greater detail later, but for the moment, it bears mentioning that there is one striking similarity between the two: In both cases, a credit crisis leading to illiquidity in credit instruments sparked a forced sale of more liquid assets that had nothing to do with the credit crisis. 

In 1998, many relative value equity arbitrage positions, which bet on convergence of share prices between stocks that are either dually listed or else are merging, suffered dramatically as an indirect result of the Russian government's defaulting on its debt obligations. The famous example used by Lowenstein in When Genius Failed was Royal Dutch and Shell, a dual-listed company. Royal Dutch had been trading at an 8 to 10 percent premium to Shell, and the bet was that the two stocks should eventually converge, eliminating the premium. In hopes of this, Long Term Capital Management, or LTCM, (and many others) had long positions in Shell and short positions in Royal Dutch. After all, there was no rational economic reason that a European listing of a given company should outperform a U.S. listing of the same company. Yet because LTCM had to vacate this position at a time when there was little liquidity, the spread widened from 8 to 10 percent to over 20 percent by the time LTCM was trading out of it. The reason that this position had to be sold is that LTCM also had massive losses on its positions in Russian debt. The Russian bond holdings were part of a relative yield trade that paired a long position in high-yield Russian debt and a short position in lower-yielding U.S. debt (which was a hedge against interest rates moving higher globally and which financed the long Russian position). When Russia defaulted, no one particularly wanted to buy the billions of dollars of their debt that LTCM was stuck with. And so, LTCM was forced to liquidate equity positions such as Royal Dutch and Shell to raise cash in a panic. $^{2}$ 

It is inaccurate to call the LTCM crisis a quant blowup. To be sure, some of those who worked at LTCM were quite good at math. But ultimately, the strategies in which they were engaged, in particular the ones that caused the most trouble, were not quant trading strategies. They were engaged in a very broad, cross-border and cross-asset class yield game in which they constantly sought to own risky assets and sell safer ones against them. It was, in most respects, a highly leveraged, one-way bet on ongoing stability and improvement in emerging markets and the markets in general. 

August 2007 was a far different affair and much closer to home for most quant funds. Several drivers coincided, leading to disastrous performance among relative value-oriented quant strategies. The causes were the size and popularity of certain quant strategies, the somewhat poor performance of these strategies for the period leading up to August 2007, the cross-ownership of these strategies with far less liquid ones by many players, and the widespread use of VaR-like models to target constant volatility. 

The first driver of the quant liquidation crisis of 2007 was the size and popularity of quantitative long/short trading strategies. From 2004 to 2007, many blue-chip managers launched quant long/short strategies targeted at attracting large pools of investor capital, either large institutions or individual retail investors. The firms launching these products were attracted by the low turnover and longer-term investment horizons of long/short strategies, both of which are necessary for the placement of large sums of capital. Investors were also attracted by the positive returns in quant long/short products from 2004 through the early part of 2007 and by the blue-chip brand-name managers launching the products. In aggregate, it is likely that hundreds of billions in cash was invested in quantitative long/short funds and bank proprietary trading desks, and with leverage, quant long-short traders likely controlled about $1 trillion in gross positions (the value of longs and absolute value of shorts added together). The vast majority of these positions were held in larger-capitalization U.S. securities because the large numbers of deeply liquid stocks allowed for sufficient diversification and size of assets under management to accommodate both the managers' and investors' needs. Even though there was actually a great deal of diversity in the underlying models of the various firms launching these products, enough of them had sufficient overlap to make individual trades get very crowded. 

The second driver of the debacle was that many of these operators had already begun to suffer subpar returns for a period leading up to the summer of 2007. Many big-name funds with a U.S. focus were flat or negative year to date before August. This is partly because “value” had underperformed “growth” since at least the end of May 2007, after several years of outperforming growth, as discussed earlier in this chapter. Many multistrategy and prop-trading desks also tend to chase recent performance, adding capital to whatever has been doing well and reducing whatever has been doing poorly. This tendency, coupled with the weak results of quant long/short trading strategies for the few months leading up to summer 2007, is likely to have contributed to especially itchy trigger fingers for risk managers who already felt the need to reduce risk in their broader portfolios. 

A third cause, and in my view a critically important one, was the widespread practice, especially among banks' proprietary trading desks and multistrategy hedge funds, of either explicitly or implicitly cross-collateralizing many strategies against each other. The huge profits enjoyed by hedge funds and prop-trading desks before this summer attest to their exposure to credit spreads that kept narrowing in early 2008. These credit-based strategies have historically proven to be far less liquid in a crisis than they appear during “normal market conditions,” and in July 2007 some credit managers experienced spectacular and sudden losses. This, in turn, drove them to seek to raise cash by selling whatever strategies were still liquid. This ATM effect is the main similarity between the 2007 meltdown and the 1998 situation described earlier. 

The fourth factor leading up to the liquidation was risk targeting (which we discussed in Chapter 7), whereby risk managers target a specific level of volatility for their funds or strategies. They hope to achieve this “constant risk” by adjusting leverage inversely with the amount of risk their portfolios are taking. The most common tool for measuring the amount of risk in a portfolio is VaR. As already discussed, VaR measures the risk of individual instruments (using the variability of their returns over time) and combines this with how similarly they are trading to each other (a correlation matrix). With models such as these, risk is computed to be higher when market volatility is higher and/or when correlations among individual instruments are higher. However, note that these two phenomena can be causally linked in that markets tend can become more volatile precisely because they are being driven by a risk factor that also leads to higher-than-normal correlation among individual instruments. In other words, both inputs to a VaR risk model can rise simultaneously, and these increases can be driven by the same underlying causes. As a consequence of using such risk measurement tools, the amount of leverage in a wide variety of strategies had risen dramatically in the few years prior to 2007, since market volatility had fallen to historic lows over that same period. However, in summer 2007, particularly in late July, volatility began to spike dramatically as the credit crisis began in earnest. This led to a requirement for many players to reduce leverage simultaneously because their VaR models reacted very negatively to the simultaneous jumps in correlations and volatility. 

To review, there were four main drivers of the crisis quants faced in August 2007: (1) large sums of money invested in value-based quant strategies with at least some similarity to each other, in other words, the “crowded trade" effect; (2) poor year-to-date performance in quant long/short trading in the United States; (3) cross-ownership of illiquid credit-based strategies that were experiencing large losses alongside more liquid quant strategies, causing the latter to be used as an ATM in a time of crisis; and (4) the use of VaR-based volatility targeting and leverage adjustments. It appears that the crisis started when several large multistrategy hedge funds and/or proprietary trading desks began to deleverage their portfolios in response to poor performance in credit-oriented strategies. In addition, market volatility was rising, leading to higher VaR levels and therefore lower leverage targets. The deleveraging began with quant/long/short trading in the United States, the most liquid strategy at hand, which also happened to have been underperforming. Managers sold off their longs and covered their shorts, causing substantial market impact. The stocks that had been long positions experienced substantial, fundamentally inexplicable price declines while the stocks that had been short positions experienced similarly violent price increases. This meant that anyone holding any of those stocks in the same direction as they had been held by the liquidators saw large, adverse performance as a result. In many cases, stocks were moving at incredible speed on massively increased volume as quants had to unwind their holdings. 

For example, one crowded short trade was in Pulte Homes (NYSE: PHM). Exhibit 10.6 illustrates the issue. 

This table contains several fascinating pieces of data. Note that PHM was declining through the early part of the summer on an average volume of 3.5 million shares per day. Then, on July 24, which appears to have been the earliest days of large-scale liquidation, the volume spiked to 7.2 million. However, this doubling in volume did not cause the stock price to change direction. In fact, it accelerated a bit. It is likely that the short-covering by quant long/short traders was being offset in the initial days of the liquidation by the short-selling of the exact same shares by mean reversion-oriented strategies such as statistical arbitrage. Over the next four trading days, volumes increased another 50 percent, but in this case there was a huge reversal in the stock, which recovered about half its 44-day decline in four days (i.e., the stock was moving about 20 times faster than it had been previously). This also happens to be an interesting illustration of the quadratic nature of market impact. The first 100 percent increase in volume was absorbed by the marketplace without a measurable change in the stock's behavior. But the next 50 percent increase seemed to be on the wrong side of a tipping point in the market's supply of buyers, and indeed, a trader covering a short position on August 9 was paying as much as 15 percent in market impact, many hundreds of times the average cost to liquidate. As soon as the liquidation pressure subsided, which by all accounts was during the afternoon of August 9, the stock resumed its downward march, falling almost 23 percent on volumes much closer to the average prior to the quant liquidation. 


EXHIBIT 10.6 Pulte Homes, Inc. (NYSE: PHM), May 31–August 31, 2007


<table><tr><td>PHM, Summer 2007</td><td>Price Change (%)</td><td>Average Daily Volume</td></tr><tr><td>May 31–July 23</td><td>-22.0</td><td>3.5 million</td></tr><tr><td>July 24–August 3</td><td>-12.5</td><td>7.2 million</td></tr><tr><td>August 6–August 9</td><td>+15.6</td><td>10.4 million</td></tr><tr><td>August 10–August 31</td><td>-22.6</td><td>5.7 million</td></tr></table>

We mentioned that other types of quant traders, such as statistical arbitrageurs, seemed to provide the necessary liquidity to quant long/short players in late July. Statistical arbitrageurs usually feast on environments like this, and no doubt many were happy to provide liquidity as they bet that prices would eventually converge. Many long positions with relatively attractive valuation characteristics were being sold at extremely depressed levels while expensive, poorer-quality short positions were reaching ever higher prices as a result of the quant long/short liquidations. These stocks had diverged from their peers so significantly that they must have appeared to be excellent trading opportunities to the average stat arb trader, who bets that such stocks will converge again to a “fair” relative value. But at some point, the stat arb traders had their fill and could not continue providing liquidity, whereas the quant long/short traders still had much more to cover. Indeed, as stat arb traders began to experience losses from having acquired these positions, they, too, became anxious to go to cash, adding fuel to the fire. 

This was likely the tipping point just mentioned, and suddenly both stat arb traders and quant long/short traders began to experience significant losses that weren't explained at all by fundamentals but purely by a lack of sufficient liquidity. Thus, by August 7 the situation was starting to get very troubling. A broader set of strategies, such as statistical arbitrage, was losing money at breakneck speed and beginning to liquidate alongside the quant long/short traders. Finally, the dam broke on August 8, with huge losses across many types of strategies and with these strategies responding by suddenly liquidating in an effort to preserve capital. Losses began to spread from U.S. strategies to international strategies, especially those implemented in Japan (the most popular non-U.S. market for quant long/short and statistical arbitrage trading). 

A wide range of fundamental signals began to lose money as the overlap between the aggregate of all liquidating managers began to overwhelm virtually any level of differentiation between managers. For the first time during this crisis, even growth-based and momentum-oriented factors began to lose money rapidly. Note that these strategies usually hold opposite positions from the value-oriented and mean reversion-oriented strategies. Thursday, August 9, was pure bedlam in quant-land. An enormous cross-section of strategies, many of which were extremely far removed from the original losers, began to bleed money. Intraday P&L charts started negative in the morning and literally every minute of the day ticked lower and lower as a huge variety and number of quant equity funds liquidated positions. Whereas a few signals had still been working on the August 8, in quant equity trading it was hard to find anything except cash that made money on August 9. It appears that any stock that was attractive for any reason was being sold down, whereas any stock that was unattractive for any reason was running up. In short, most quant equity traders had the worst day in their history, and a great many reduced leverage to extremely low levels, with many shops going completely to cash. 

A bit more should be mentioned about why so many managers reacted in the same way, namely by deleveraging and liquidating positions. Early August was a period of exceedingly perverse behavior. Not only were tried-and-true factors not working, they were actually working negatively. And because the primary discretion employed by a great many quant managers is the decision to unwind positions in the event that the models are behaving badly, quant managers did exactly that, leading other managers with any overlap experiencing losses and doing exactly the same thing in response. The losses incurred, it is important to note, were solely the result of market impact. 

One of the clearest proofs of this point is that one large, well-known quant firm was suffering like everyone else in early August. On August 9, in a panic, the firm tried to convene its investment committee to determine what to do. But several members of the committee were on their summer holidays, so a meeting was scheduled for Monday, August 13, and in the meantime the lieutenants managing the portfolio day to day kept the fund fully invested. As shown earlier in Exhibit 10.6, prices returned to their previous trends fairly quickly when the liquidations stopped. (PHM, for example, was down about 12.3 percent by the close of business on Monday, August 13, merely two trading days later.) As such, by the time the investment committee met, its fund had recovered a huge proportion of its losses, and the committee elected to hold the course. 

Perhaps the greatest irony of the broader situation in August 2007 was that smaller, more boutique quant traders, engaged in less commonplace strategies that had minimal overlap with the more conventional and larger-scale institutional quants, ended up experiencing losses and liquidating their portfolios only very late in the game. As alluded to earlier, managers whose losses began to accumulate only in the middle of the second week of August ended up needing liquidity at the tail end of an already massive deleveraging. 

This forced them to pay incredible transaction costs (all from market impact) to reduce their leverage. Reports of losses at extremely prestigious funds abounded. The range of losses was wide, from -5 percent to -45 percent, but few equity traders emerged unscathed from this event. 

What separated August 2007 from prior market crises, even from the great crash of 1987, was that there was no general market panic during this period. U.S. stocks were approximately flat for the first 10 days of August, whereas stocks internationally were down in the small single digits. What we witnessed in this period was nothing short of a liquidity crisis in the most liquid stocks in the world, driven by market-neutral investors whose hundreds of billions of dollars of position selling led not to a market collapse but to almost no change at all in equity index values. This situation illustrated for the first time that contagion/common investor risk can appear in liquid quant strategies almost as much as in illiquid or discretionary strategies. For the first time, crowding became a risk of quant trading strategies. 

## HOW QUANTS MONITOR RISK

Any discussion of quant-specific risks also merits a discussion of quant-specific tools used to target those risks. Chapter 7 described risk models at some length as models that seek to eliminate or control the size of exposures in a portfolio. But quants also utilize various pieces of software to monitor these exposures, their systems, and the kinds of “quant-specific” risks we have discussed in this chapter. There are several types of monitoring tools, most notably exposure monitoring, profit and loss monitoring, execution monitoring, and systems performance monitoring. 

Exposure monitoring tools are straightforward enough. They start with the current positions held and then group and/or analyze these positions for whatever exposures the manager is concerned about. For example, in a futures portfolio, if the manager wants to see how much of his portfolio he has invested in the various asset classes (equities, bonds, currencies, and commodities), this is something he can do with exposure monitoring software. Similarly, one can group instruments by any other sets of characteristics that are of interest, such as their valuation, the level of momentum they have exhibited, their volatility, and so on. Many equity traders (using either proprietary tools or off-the-shelf software such as BARRA or Northfield) monitor their gross and net exposure to various sectors and industries, to various buckets of market capitalizations, and to various style factors such as value and growth. The tools are straightforward, but the art is in how to use them. Experienced managers can discern from the exposures in their portfolios whether the model is behaving as it should be. If exposures are out of line based on either limits or expectations, this can be an early warning that there is a problem with the model or else problematic market conditions. 

Profit and loss monitors are similarly straightforward. They also start with the current portfolio, but they then look at the prices at which the portfolio's positions closed the previous day and compare those to the current market prices for the same instruments. Many managers look at charts of the intraday performance of their strategies to determine quickly and visually how the day is going. These tools are also important in watching out for several types of model risk. If the strategy appears to be performing in an unexpected manner, either making money when it should be losing or vice versa, the manager can check into the reasons for this anomalous behavior. Or alternatively, the manager can see patterns in his performance that can alert him to problems. We alluded to this idea in discussing the performance of various quant strategies during August 2007, when the intraday performance charts were showing deterioration in the performance with nearly every passing tick. We know of at least one manager who noticed this intraday pattern and, as a result, quickly conducted research that enabled him to reduce his risk much earlier than most, thereby saving him much of the loss experienced by other traders who only sold later. 

Other types of profit and loss monitors look at how money is being made or lost rather than whether money is being made or lost. For example, quants can analyze the realized and unrealized gains and losses of their strategies. Many strategies are constructed to cut losing positions quickly and ride winning positions longer. But if a quant sees that her strategy is holding losers for longer than usual or selling winners more quickly than usual, this can be an indicator that something is wrong and needs to be corrected. This kind of tool also frequently tracks a hit rate, which is the percentage of the time that the strategy makes money on a given position. Again, the designer of a strategy usually understands what the hit rate of a trading strategy should look like, and substantial deviations from the norm in this metric can be important indicators of problems. 

Execution monitoring tools are usually designed to show the quant trader the progress of his executions. They typically show what orders are currently being worked and which ones recently were completed, along with the sizes of the transactions and prices. Fill rates for limit orders are also tracked to help monitor the execution algorithms' performance, particularly for more passive execution strategies. Some managers specifically measure and monitor slippage and market impact in their order execution monitoring software, which allows them to see whether they are getting the kinds of results from their execution strategies that they would expect. 

Finally, systems performance monitors are used largely to check for software and infrastructure errors. Quant traders can monitor any aspect of their technology, from the performance of CPUs or the speed of various stages of their automated processes to latency in the communication of messages to and from the exchanges. This kind of monitoring is perhaps the most important for sniffing out systems errors and some types of model risk. 

## SUMMARY

Quant trading offers many potential benefits to investors and practitioners. The discipline, computing power, and scientific rigor brought to bear on the challenge of making money in a highly competitive marketplace certainly pay dividends overall. However, quants have their own sets of problems to deal with. Some of these problems are unique to quants (e.g., model risk), but most are simply more significant for a quant strategy than for a discretionary one (e.g., common investor or contagion risk, exogenous shock risk, and regime change risk). Quants utilize various types of tools to monitor their systems and risk, which can help mitigate the downside associated with the risks of quant trading. 

Having discussed at length the challenges facing a quant trader and how the quant faces these challenges, we turn our attention to various criticisms of quant trading that are widely espoused in the marketplace. 

# Criticisms of Quant Trading Setting the Record Straight

Computers are useless. They can only give you answers. 

—Pablo Picasso 

Recently, and periodically in the past, people have loved to hate quants. In 1987, a quant strategy known as portfolio insurance was blamed for the crash that occurred that October. In 1998, people blamed quant models for the LTCM crisis and the near-collapse of financial markets. In the summer of 2007, though, it might well be that the tide of public opinion turned from leery and suspicious to overtly negative. There could be many and various reasons for this sentiment. Some of the predilection is likely owed to widespread hatred of math classes in grade school, some of it to fear of the unknown, and some to occasional and sensational blowups by one or several black boxes. But as is the case with many things that are not widely understood, the arguments against quant trading range from entirely valid to utterly ridiculous. It is worth noting that almost every type of trading in capital markets faces valid criticisms. In other words, quant trading, like any other type of trading, has its pluses and minuses. 

This chapter addresses many of the most common criticisms of quant trading and some of my own. Where relevant, I also present counterpoints in defense of quants. 

## TRADING IS AN ART, NOT A SCIENCE

The markets are largely driven by humans' responses to the information they receive. Not all this information is understandable systematically. 

Furthermore, the process by which different people interpret the same piece of information is not systematic. If the CEO of a company is fired, is that good news or bad news? One trader might argue that it shows instability at the highest levels of office and is therefore terrible news. Another might say that the CEO deserved to have been fired, it was a situation well handled by the board of directors, and the company is far better off now. Neither can be proven right ex ante. So, critics of quant trading claim, how can anyone believe that you can really model the markets? Their critique is that markets are ultimately driven by humans, and human behavior can't be modeled. 

This criticism of quant trading is rather backward, reminiscent of the persecution of scientists such as Galileo and Copernicus for proposing ideas that challenged human authority. Humans have successfully automated and systematized many processes that used to be done by hand, from manufacturing automobiles and flying planes to making markets in stocks. Yes, of course there is still room for humans to make or do various products or services by hand, but when commerce is the main objective, we typically see that the efficiency and consistency of automated processes outweigh the benefit and cachet of doing things manually. 

The idea that human behavior cannot be modeled is a bit less easily dismissed, but it is also unlikely to be true. Consider that quantitative techniques are extraordinarily successful for determining what books you might like at Amazon.com, in mining data in customer relationship management software, and in human resources departments seeking to determine which universities produce the best employees. Obviously, as we have already discussed, there is always the risk of trying to get computers to answer questions that shouldn't have been asked of them and of building models that are not good representations of the real world. But in many cases, quant trading included, it is entirely feasible to demonstrate that something humans do with mixed results can be done just as well by computers: to profit from trading the markets. 

Indeed, when done well, computerized trading strategies have tended to be exceptional performers over very long periods, as demonstrated by the examples we've used so far (Ed Seykota, Renaissance, Princeton-Newport Partners, D. E. Shaw, and Two Sigma). In the best cases, models are merely simulations of the real world, not replications. So we cannot expect a quant's models to be perfect, just as we cannot expect Amazon.com to recommend exactly the right book every time. However, over time, a well-designed quant strategy can predict enough of the behavior of the markets to generate substantial profit for practitioners, as evidenced by the results of some of the quant firms we highlighted in Chapter 2. 

## QUANTS CAUSE MORE MARKET VOLATILITY BY UNDERESTIMATING RISK

This criticism contains components of truth and of falsehood. Many managers, quants included, are subject to a fundamental type of model risk we discussed in the last chapter, namely asking the wrong questions and using the wrong techniques. Techniques such as VaR, for example, make numerous wrong assumptions about the market in an effort to distill the concept of risk down to a single number, which is a goal that seems mostly pointless. Furthermore, as illustrated by the August 2007 quant liquidation crisis, quants have underestimated the downside risk of being involved in large-scale, crowded trading strategies. This, too, stems from a fundamental flaw of quantitative trading. Computers can be given a problem that is badly framed or makes too many assumptions, and they can come up with an answer that is both highly precise and entirely wrong. For example, I can drum up a model of my wealth that assumes that this book will sell 50 million copies, that I will receive 50 percent of the proceeds, and that I can then invest the proceeds into a vehicle that will earn 100 percent per year, compounded, forever. With this model I can get precise answers to the question of my earnings as far into the future as I want. However, all my assumptions are highly suspect, at best. 

The computer's job is not to judge my assumptions, so this kind of error is ultimately attributable to my poor judgment. Similarly, some quants can be blamed for using quantitative models that are either inappropriate or badly designed to measure risk. That said, they are scarcely alone in making these errors. Indeed, VaR itself was developed to appease risk managers and banking regulators who were interested in having a single number to summarize downside risk, rather than do the difficult and nuanced work of understanding risk from many perspectives. So, though we accept the criticism that quants can underestimate risk or measure it wrongly, it is worth understanding that they are not alone. Decision makers in almost every field commonly manage to underestimate worst-case scenarios, and when they do not, it is usually to overestimate risk in the aftermath of a disastrous event. This is largely because extreme risks are so rare that it is very difficult to ascertain their probability or the damage they can cause. So, we find that the statement that quants underestimate risk is likely to be true, but we also find this to be due more to human nature and the circumstances of rare events than to something specific in quant trading. 

The idea that this underestimation of risk on the part of quants is somehow responsible for an increase in market volatility is, however, plainly ridiculous. First, we have already shown in Chapter 2 that quants tend to reduce market volatility and inefficiency during normal times. Regardless of what happens in abnormal, chaotic times, this fact should not be simply discounted. Second, extreme events have been happening since people could trade with each other. Preliminarily, we can look at extreme events in stocks and other asset classes. There were five distinct drawdowns in the Dow Jones Industrial Average that were worse than 40 percent before quant trading existed (indeed, before there were computers in general use). The worst of these occurred during the Great Depression, which brought with it a drawdown of almost 90 percent in the Dow and which took until 1954 to recover. The last drawdown in stocks before quant trading became a significant force began in January 1973, reached a nadir of -45 percent in December 1974, and was not fully recovered until November 1982. The next severe drawdown in stocks since then was the bear market of March 2000 through October 2002, which was set off by the bursting of the dot-com bubble. It is ridiculous to claim that a single one of these events of extreme volatility or prolonged pain were owed to quant traders. The same analysis holds for other asset classes. The worst event in recent history in bonds was Russia's default in 1998. This impacted some "quant" firms (though, as mentioned in the last chapter, I reject wholesale the idea that LTCM was actually a quant trading firm) but was certainly not caused by quants. The currency problems in Mexico and Asia in 1995 and 1997, respectively, were also not the result of quants' activities. In fact, at the time a rather famous discretionary macro trader, George Soros, was widely (though not necessarily correctly) blamed by Asian governments for triggering the latter event. 

We can also look at the broader question of how quants are related to market crises from the opposite perspective. How does a crisis in quant trading relate to changes in or levels of market volatility? Since we so far have only one example to work from, we will focus on the events of August 2007. The Dow Jones Industrial Average's historical volatility did move up during the two-week period in which quants were experiencing pain that summer. However, the Dow's realized volatility moved from a significantly below-average level to a level that is equal to the average volatility since 1900. From the close of trading on August 3 through August 9, 2007, certainly the worst part of the quant liquidation crisis, the Dow was actually up an estimated 1.1 percent—scarcely cause for alarm. Implied volatility, as measured by the VIX index, moved up during this period, from 25.16 to 26.48, but this is by no means a significant change in its level over a four-day period. It would be an impressive stretch of the imagination to attribute any change in market volatility to quant traders. Indeed, of infinitely greater importance to downside risk in markets and upside swings in volatility levels are policymakers' decisions, exogenous shocks (e.g., wars or terrorist attacks), basic economic cycles, and run-of-the-mill manias and panics. With that, I believe that the extraordinary events of 2008 bear discussion. 

## The Market Turmoil of 2008

As I write this book, the financial world is suffering through its most challenging environment since the Great Depression. Stocks have endured their second distinct 40-plus percent decline in a single decade, and dozens of banks around the world have either gone bankrupt or have been nationalized, including two of the five largest U.S. investment banks. Real estate prices have crashed in many parts of the world. Several money-market funds have lost all or most of their value. Several of the largest insurance and mortgage companies in the United States were nationalized or required rescuing. The nation of Iceland was effectively bankrupted and actually went to Russia to seek a loan. Record-setting bailout packages and unprecedented, multinational government-backing measures have been enacted in an attempt to stabilize the financial system, which U.S. Secretary of the Treasury Henry Paulson reportedly told the U.S. Congress was “days from a complete meltdown.” Most forms of financial activity, in particular credit, were frozen almost entirely. I raise this contemporary example of market turmoil for two reasons: (1) to evaluate whether quants can be blamed for it and (2) to discuss how quants have fared. 

It remains to be seen whether the market declines that began in October 2007 and accelerated in the fall of 2008 will ultimately rival those of the Great Depression. Regardless, we can understand a fair amount about what brought us to this position: It was caused by irresponsible banks that lent money without proper diligence to unqualified consumers who acted with total disregard to reality; enabled by ratings agencies that had lost all sense of independence and objectivity; and then the situation was ignored and/or exacerbated by regulators. Dodgy accounting practices, incredible amounts of leverage, extreme greed and recklessness among people who should know better, skewed compensation practices, and lofty egos also played significant roles. 

Short sellers and hedge funds were widely blamed for causing the crisis, and indeed, it does appear possible that irresponsible rumor mongering on the Internet might have been partially to blame. (Though I have not seen anyone propose banning the Internet or the kinds of sites that give rumors such wide audiences.) There is no acceptable excuse for those who spread such rumors. But let us be clear and explicit: This was an equally irresponsible attempt to divert attention from the real causes and culprits, many of whom were loudly lobbying for banning short sales and hedge funds. 

The facts are unchanged, despite the attempted smokescreen: Many banks did in fact have toxic balance sheets, uncounted and untold billions in losses, and no way to solve the problem. The bailout package passed by Congress in 2008 approved $700 billion of rescue money, which is, according to most experts, only big enough to solve one-third of the problem. In other words, this is one hell of a very real mess, not just a rumor-driven illusion. To appease those railing against hedge funds and short sellers, the U.S. SEC banned all short sales of 799 financial stocks from September 19 to October 8, 2008. During this time, the Financial Select Sector SPDR (AMEX: XLF), an ETF tracking the financial sector, fell another 23 percent (slightly worse, if we exclude a roughly 1 percent dividend issued during this period). By contrast, one week after the ban was lifted and financial companies were again allowed to be sold short, XLF gained slightly versus its closing price on October 8. 

How have quants fared through this market trauma? Better than most. In 2008 many quantitative equity firms struggled, posting losses in the -10 percent range for the year. But a great many quants, using statistical arbitrage, short term trading and even some longer-term trading strategies, actually made substantial gains. And in other fields of quant trading, 2008 was a banner year. Quantitative CTAs and short term traders in various asset classes, in particular, have done rather well through the crisis. But even if -10 percent was the norm, why should this considered a particularly bad outcome, especially compared to the alternatives? Stocks have cut investors' money in half twice in the past decade. Many large, storied money market funds have gone bust. To my way of thinking, these are examples of extremely risky investments, not quant hedge funds. And as just mentioned, it is categorically untrue that quants in general struggled in 2008. 

This is also not the first time that quants have demonstrated good performance in turbulent times. In the last two severe market dislocations, in the summer of 1998 and in the bear market of 2000 to 2002, quants again proved to be outperformers. Both periods, in fact, were quite good for a great many quants, with some having the best results in their histories during these times. Even in the crash of October 1987, most quantitative trend-following CTAs posted tremendously strong returns. This isn't to say that they are immune from losses or unaffected by market turmoil. The point is that there seems to be an immense double standard applied to quants compared with more traditional markets and even other hedge funds in terms of what is considered risky. 

## QUANTS CANNOT HANDLE UNUSUAL EVENTS OR RAPID CHANGES IN MARKET CONDITIONS

This is perhaps the most valid criticism of quant trading so far. Quants must rely on historical data to make predictions about the future. As a result of this dependency, it is likely that quants will suffer any time there is a significant and sudden change in the way markets behave. It bears repeating and emphasizing that, in order for the event to be of importance to a quant, the regime change must be both large and without much warning. Perhaps the most challenging time for quant trading in its known history has been the period from late July 2007 through August 2008. Over this roughly 13-month window, quants faced the liquidity crisis and at least three separate episodes of substantial pain. You can see this illustrated in part in Exhibit 11.1. 

As you can see from this figure, Value outperformed Growth from mid-2004 through early 2007. There was a reversal of this trend beginning in mid-May 2007, which accelerated aggressively in late July 2007 and was a likely cause of the poor performance among quants that contributed to their liquidation. The trend favoring growth over value from May 2007 to January 2008 is easily seen to be sharper than that which favored value before May 2007. Many quant strategies had adapted to this new regime by the middle of the fall of 2007, leading to strong performance in the later part of that year. But two other periods catch the eye: one in January 2008, and the other in July 2008, both of which are circled in the chart. These two events were rather violent reversals of the strong trend favoring growth that began in May 2007. These reversals were among the sharpest in the history of this spread, and both were substantial periods of downside risk for many quant traders, particularly those in equities. This is because the prevailing pattern of behavior, on which the quant bases forecasts of future behavior, becomes inverted at such times. 


Value-Growth Spread, December 2003 – December 2008


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/795fb498-d6a9-4662-ac88-5c846830c491/f7a9921c0e4b57638bf3d4902ba90c003d81845064764140a64c211eadc5fda6.jpg)



EXHIBIT 11.1 Regime Changes, as Indicated by the Value/Growth Spread


It is worth mentioning that although the significant majority of quant strategies are negatively impacted by regime changes, a small minority are able to successfully navigate these periods. Some shorter-term strategies specifically seek to profit from short reversals of longer-term trends and the resumption of such longer-term trends. These counter-trend traders have been able to profit in many of the most difficult periods for quants (but certainly not all of them). Others sit on the sidelines during normal times, waiting for large dislocations to signal the beginning of a potentially profitable trading period. This kind of trading is known as breakout trading. Both of these styles can be found in any asset class or instrument class but are most generally done with futures instruments in the most liquid markets. 

## QUANTS ARE ALL THE SAME

This argument, too, has been widely held to be true, particularly in the wake of the disastrous performance of many quants in August 2007. However, it is a patently false claim, and this I can state with both vehemence and certainty. We will focus again on both theoretical and empirical evidence of this truth, starting with the former. 

This book has outlined many of the kinds of decisions each quant must make in the process of building a quant strategy. These decisions include the kinds of instruments and asset classes to trade, the sources of data one will use and how these should be cleaned, ways to research and develop trading strategies, the kinds of phenomena are being traded, how these phenomena are specified, ways in which various forecasts are combined, how far into the future forecasts are being made, how bets are structured, ways in which risk is defined and managed, how transactions costs are modeled, how portfolios are constructed, and how trades are executed. The number of degrees of freedom for a quant in building a trading strategy is, in other words, very large. Though the kinds of phenomena are not very numerous, all the other considerations are ways the quant can differentiate his approach from those of others who are ostensibly looking for the same types of anomalies. Depending on the time horizon of the strategy and number of positions it takes, the number of trades per year can easily get into the millions. I know many traders who execute 10,000 to 100,000 trades each trading day. As you can imagine, small differences in how one arrives at a single trade are amplified when millions of trades are made in a year. 

The empirical evidence is abundant and covers both position data and return information. At my firm, we have separately managed accounts with both quant and discretionary equity firms. On an average day, 30 percent of the quants' positions are held in opposite directions on the exact same names. This belies the premise that quants are all the same, especially since only about 75 percent of their positions are even in the same country. In other words, of the positions held in the same country, about 40 percent are held in opposite directions by various quant traders. As the number of traders is increased, this ratio naturally also increases. This has been confirmed by several studies. In 2008 Matthew Rothman, then of Lehman Brothers (and now of Barclays Capital), produced a study of 25 of the largest quant equity market neutral traders and found that approximately 30 percent of their positions were held in directions opposite those of someone else in the group, on average, using portfolio data spanning over a year. Among smaller firms, the differences are even more noticeable. With a third to half of all potentially overlapping positions held in opposite directions, it is difficult to accept an argument that quants are all the same. If they were, one quant's long would not be so likely to be another quant's short. 

Return data confirm what we see in the position data. I have a sample of a couple of dozen quant managers' daily returns (some going back as far as 1997), and the average correlation of these managers to each other is 0.03. There are only nine pairs of correlations that exceed 0.20, out of 252 pairs in total. And during the heart of the crisis, from September through November 2008, this correlation was merely 0.05. By contrast, the eight HFRX hedge fund indices that have daily returns (i.e., ranging from convertibles to risk arb and macro strategies) correlate at an average of 0.21 to each other, and 11 of the 28 pairs correlate at greater than 0.20. Five of the 28 correlate at greater than 0.40, and the maximum correlation is 0.81, between the equity hedge and event-driven styles. 

The same basic story is told by monthly return data. Measuring the correlations of some 53 quant equity market neutral traders with at least 25 months of return history, we find that the average correlation among them is 0.13. Note that we did not even include quantitative futures trading, which would reduce the correlation still further. By contrast, 22 HFRI hedge fund-style indices (excluding the broader HFRI hedge fund and fund of funds indices and excluding the short-selling managers) correlate at an average of 0.48 to each other, and these span styles as diverse as macro and distressed debt. The data are strongly in opposition to the idea that all quants are the same, confirming what we would expect, given a basic understanding of how quant trading strategies are actually developed. 

## ONLY A FEW LARGE QUANTS CAN THRIVE IN THE LONG RUN

I've heard this criticism repeated countless times by various observers of the quant trading world. The argument is reasonable enough at first glance, and it goes something like this: The largest and best-funded quants can throw the most and best resources at every aspect of the black box, from data to execution algorithms, and can negotiate better terms with their service providers. Based on this premise, it is reasonable to expect that, in the long run, they will outperform their smaller cousins. Ultimately, smaller quant firms will fall by the wayside due to either underperformance or investor attrition. The best shops, furthermore, are so good that they ultimately replace their investors' capital with their own, leaving the investor who desires to invest in quant trading in a quandary: Should she select smaller, inferior shops and be able to keep money with them until they go out of business? Is it better to invest in a handful of the biggest quants while that is still possible, and if they kick out their investors later, so be it? Or is it best to simply avoid this space altogether, since the two other options are unattractive? 

This criticism and its corollaries are interesting theoretically but ignore many important facts about quant trading and therefore draw an incorrect conclusion. First, as evidenced very clearly in August 2007 and throughout 2008, having a large amount of money to manage is not always good, because readjustments to such large portfolios can be extremely costly in times of stress. In other words, one sacrifices nimbleness while gaining size. 

Second, whole classes of very appealing strategies are made impossible or impractical for the largest quants because the amount of money that can be effectively managed in those strategies is too small to be worth the effort. For example, large quants rarely engage in statistical arbitrage in markets such as Australia or Hong Kong because they cannot put enough money to work there. High-frequency trading in any market has very limited capacity and is therefore a very uncommon component of a large quant trader's portfolio. 

Third, there is reasonable evidence that smaller hedge funds actually outperform larger funds. $^{1}$ Some observers believe this is partly because smaller shops are headed by entrepreneurs who are hungry to succeed rather than already successful managers who can become complacent or uninvolved. Regardless, there isn’t a particularly good reason to believe that the lack of resources any small trader faces, relative to those who are much larger and trade similar strategies, is any more an impediment for quants than for discretionary traders. As one small discretionary trader put it, “It’s not like I’m going to get the first call when a broker has useful information about a company. I just have to work harder and find things on my own.” In other words, though there is evidence that smaller managers outperform larger ones, there is no reason to distinguish smaller quants from smaller discretionary shops. Both face challenges that larger shops don't, and both must find ways to cope with them. 

Fourth, smaller managers tend to focus on the kinds of things they know and understand best, whereas larger managers need to diversify into areas that are increasingly far from their core expertise in order to grow to such large size. Most very successful trading strategies have somewhat limited capacity for capital under management. As such, to build on success, a larger trader must incorporate other strategies, which might not be at all similar to the ones in which the original success was achieved. This was certainly the case with LTCM and Amaranth; it is also the case with more successful large hedge funds such as D. E. Shaw, Caxton, and Citadel. Some of these have managed a wide diversity of strategies better than others, but the evidence in favor of large multistrategy hedge funds is mixed at best. 

Fifth and finally, the vast majority of the quality of a quant strategy is determined by the good judgment and sound research process of the people in charge. Therefore, it is absolutely the case that one good quant, with significant applied science and/or trading experience and sound judgment, is worth dozens of Ph.D.s who lack these traits. This is a topic we will save for the next chapter. 

I have certainly seen firsthand reasonably compelling evidence that a portfolio of boutique quant traders can be built that is productive and competes favorably with a single, larger quant manager. There are also a large number of quants who are not among the largest but who certainly have sufficient resources to tackle many of the same advanced problems that the largest shops can consider. For example, the smallest firms almost always rely on data vendors, but some boutiques actually collect and clean their own data, something that it is widely assumed that only the largest firms can do. Both theoretically and empirically, there is little evidence to support the idea that there are only the largest quants can survive. 

This is not to say that the largest firms are without their advantages. Those pluses outlined at the beginning of this section are certainly valid, for example. But the case in favor of larger quants is far from airtight, and equally strong arguments can be made for boutiques. The good news is that there are many hundreds of them from which to choose. 

## QUANTS ARE GUILTY OF DATA MINING

Data mining is given a fairly bad name in financial circles. It is used interchangeably with another term that is actually deserving of such negative judgment: overfitting. Data mining is an empirical science, to borrow again from the framework of the two major kinds of science we discussed in Chapter 6. Data-mining techniques are generally understood to use large sets of data for the purpose of deriving information about what happens without worrying about why it happens. This is the biggest difference between data mining and theory-driven science: Theorists are interested in understanding why something happens in order to believe that they can correctly forecast what will happen. However, as we already learned, theorists, too, look to historical data for cues about what kinds of theories might explain what has happened. This is a fine line—fine enough that it is not entirely clear that there is a valid difference between well-done empirical science and well-done theoretical science. The only discernable difference is that, in theoretical science, a human is expected to derive an explanation that seems reasonable to other people, whereas in empirical science, the method of analyzing data is the primary subject of scrutiny. In other words, nearly everyone mines data, even if only loosely. This is not problematic. We would not have heard that cheap stocks outperform expensive ones unless someone had some data to support the idea. If the data were overwhelmingly opposed to such a statement, no one would espouse it as a valid approach to investing. 

Data mining is very successfully used in many industries in the broader economy and society. In the defense industry, data mining is widely used in terrorism prevention. No doubt you have heard of the U.S. government's efforts to scan millions of phone calls and e-mails for information to help predict and therefore help stop terrorist attacks. The government does not have individuals sitting on phones listening into each conversation or at computer terminals reading e-mails. Rather, computer algorithms are used to discern defined patterns that are expected to be fruitful in rooting out potential terrorist activities. 

We have already given several other examples of successful data mining in this chapter. Amazon.com uses data mining to advise you of what kinds of books you might like, given what you've purchased and viewed. Analytical CRM software packages help businesses maximize profit per contact by mining data on these contacts, to allow sales personnel to focus on the most lucrative clients and spend less time on less lucrative prospects. Human resources departments use data-mining tools to discern which universities produce the best employees (the "goodness" of an employee is based on measures of her productivity and quality). Scientists, too, are heavy users of data-mining techniques. This is particularly evident in the field of genomics, where patterns of genetic information lead to linkages between specific genes and human health and behavior. So, it might not be entirely fair to claim that data-mining techniques cannot be used on market data, given their wide use and success in so many social and hard sciences. 

Overfitting is another story entirely. Overfitting a model implies that the researcher has attempted to extract too much information from the data. With a sufficiently complex model, it is possible to explain the past perfectly. But what is the likelihood that a perfect explanation of the past, using an overly complex model, will have any relevance to the future? It turns out that the answer is, not bloody likely. Imagine that we find out that the S&P 500 dropped an average of 1 percent anytime the Federal Reserve announced a decision during some period. But we have only a handful of observations of the Fed making announcements, and all their announcements during the historical period were of the Fed announcing rate hikes. We could, if we were overfitting, draw a conclusion that Fed announcements are always bad, and this conclusion would be successful so long as future Fed announcements are met with the same reaction as past announcements. But what happens if the next Fed announcement is of a lowering of interest rates? It's very likely the strategy would lose money because it was fitted to a sample that primarily included rate hikes. Therefore, we should be concerned about overfitting the data. 

As an experiment, I set up a new Amazon.com account and idly clicked on a handful of books of interest to me. The recommendations that came back were not nearly as good as those that I'm given from my main Amazon.com account, since my main account is based on a lot of real data, whereas the new account is based on information from fewer than 20 observations of my clicking on various titles. The recommendations in my new account are likely to be overfitted, whereas those in my old account are less likely to be overfitted. 

To estimate a given parameter of a model, one needs rather a lot of data. Overfitting ignores this basic fact and burdens a limited supply of data too much, asking it to explain more than is realistic, given the amount of data. These models are finely tuned to the past, but the moment that the future is out of step with the past, the model breaks down. In quant finance, the inevitable outcome of overfitting is losing money. There is no question that, when it is found, overfitting should be eliminated. But it is a gross and incorrect generalization that all quants overfit their models. Those most likely to be guilty of overfitting are data-mining quants. And among data-mining strategies, I find that a useful rule of thumb is that shorter time scales tend to be more amenable to data mining than longer time scales. 

First, this might be due to the fact that there are so many more observations of trades at short time horizons, and therefore the amount of data available for analysis are increased. If a strategy holds positions for a year, on average, it would take hundreds of years to be comfortable with any substantial statistical analysis of the strategy's returns, because the number of betting periods is so small. If, by contrast, a strategy trading U.S. stocks holds its positions for one minute, there are 390 trading periods per day (because there are 390 minutes per trading day) and about 100,000 trading periods per year (because there are 250 to 260 trading days per year and 390 minutes per trading day) per stock. If 1000 stocks are traded, there are about 100 million trading periods per year to observe, yielding a great deal more data that can be mined. Remember, the problem of overfitting arises when the model is too complicated for the amount of data available. The more data are made available, the less likely it is that overfitting has occurred for a given level of model complexity. 

Second, at very short time scales it is not clear that theoretical scientists have yet come up with useful explanations of behavior. A practical guideline is that, for strategies with holding periods of less than a day, data-mining strategies might be fairly useful. For strategies with holding periods on the order of a week, a hybrid approach that combines data-mining techniques and sound market theory can be useful. Finally, strategies that expect to hold positions for months or years are not likely to work if they rely on data-mining techniques. 

Over-fitting models is not only possible, it actually happens among some quant traders. But just as we do not reject analysis because some people are prone to overanalyzing things, we should not so quickly dismiss quantitative modeling (even data mining) just because it is possible (or even easy) for some people to do it badly. 

## SUMMARY

Quant trading is no elixir, and certainly there are quants who are guilty of each or all of the criticisms discussed in this chapter. Some do bad science, underestimate risk, and lose money when market conditions change suddenly. Some implement strategies that are commonplace and crowded, and some overfit their models to limited amounts of data. But most of these criticisms are equally applicable to discretionary traders. Done well, quant trading can produce superior risk-adjusted returns and substantial diversification benefits. 

So, what does it mean to do quant trading well? We will cover this topic in depth in the next chapter, but let's recap some salient points from this chapter: Quants must be concerned with falling prey to the temptation of false precision, particularly in risk management. A printout with a risk number on it does not imply that the number is accurate or has been properly derived. Quants must also remain aware of relationships within the market and must have a detailed understanding of the kinds of bets they are making and how they are expressing these bets in their portfolios, allowing them to navigate violent regime changes. Quants must conduct innovative research in alpha modeling and across the entire spectrum of the black box, to reduce the risk that there is substantial overlap between their models and those of their peers. Finally, to the extent that data mining is explicitly utilized, it should be done in a manner that does not express overconfidence in the amount and predictive power of historical data. 

<!-- === Source: MinerU_markdown_Rishi_Narang_-_Inside_the_Black_Box_201_2122156029113376771.md (Page 201) === -->

# Evaluating Quants and Quant Strategies

The avocation of assessing the failures of better men can be turned into a comfortable livelihood, providing you can back it up with a Ph.D. 

—Nelson Algren 

In this chapter we discuss methods of assessing quant strategies and practitioners to separate the good from the mediocre and the mediocre from the poor. As I have said throughout this book, a great deal of the work that quants do has very natural analogues in discretionary trading. There are also significant parallels in the work of a quant trader to the work of a corporate CEO or any other person involved in the allocation of resources. In this regard, the framework presented in this chapter can be used successfully to judge the work of such decision makers. Indeed, one person I trained in this method of assessing quants has adapted it for trading credit markets and now uses the same method to provide a framework for judging the merit of various corporate bond offerings and the companies behind them. 

The first challenge an evaluator of quants faces is to pierce the walls of secrecy that quants build around their methods. Though it is fair to say that quants are often secretive, I have had a rather different experience. The vast majority of quants I have evaluated—and there have been many hundreds of them—have been willing to answer most or all of my innumerable questions. The difference is due, at least in part, to the questions we ask at my firm. It also owes to how we ask these questions and how we handle the information we learn from quants. In the next section I describe the principles of my approach to interviewing quants. 

Armed with the techniques described in this chapter, the evaluator of a quant has two goals. The first is to understand the strategy itself, including the kinds of risks it is taking and from what sources its returns are generated. This is important because it tells the investor what she owns when she is investing in a given quant strategy. The second goal in the evaluation of a quant is to judge how good the practitioners themselves are. In many respects, a quant trading team is much like an engineering team at an automobile manufacturer. It is fine for the team to build one great engine, but over time, that engine must be improved. As times change, the engine might even need to be redesigned entirely, or other types of engines might need to be designed for other vehicles. It is critical to ascertain whether the quant team is skilled at designing engines, evolving them, and designing new types of engines over time. All these components of the analysis of a quant ultimately serve to help the evaluator answer perhaps the most central question in the evaluation of any kind of trader: Why should I believe that this particular team, utilizing this particular strategy, is actually likely to make money in the future? In hedge fund parlance, what is this manager's "edge"? 

Assuming that the investor finds a team and strategy worthy of investment, he must ascertain the integrity of the people involved. After all, skill is a good thing only if it is in the hands of good people. Here I briefly address some thoughts on how to judge the integrity of a trader, although this is not central to quantitative trading. Finally, I provide a few brief thoughts on portfolio construction using the frameworks provided in this book. 

## GATHERING INFORMATION

How does one actually go about finding out what a particular quant does? Quants are notorious for their secrecy and paranoia. And this is not without reason. Much of the skill of quant trading comes from experience and knowhow, not from raw mathematical superiority. There is an excellent book called The Interrogator, by Raymond Toliver, from which many useful lessons can be learned on how to get information from a quant. $^{1}$ The book's subject is Hanns Joachim Scharff, a former World War II Luftwaffe interrogator who succeeded at gathering information from downed Allied pilots without the use of any physical force or psychologically stressful techniques. Instead, Scharff used three major tools: trust building, domain knowledge, and an organized system for tracking and retrieving information. 

Before detailing Scharff's techniques, I want to stress that I am no fan of wars or interrogations, nor does the relationship between investor and quant manager closely resemble the relationship between interrogator and prisoner. But there is one similarity, I believe, that allows lessons from the latter to be useful in the former: In both cases, information that one party is reluctant to provide is needed by the other. 

The first technique Scharff used is also the most obvious: He built trust with the pilots he was interviewing. In fact, Scharff remained friends with a great many of them after the war, and they seemed universally to respect and like him. Turning to the quant, trust comes in part from building relationships, but a big chunk of it relates to the behavior of the interviewer. If an investor asks a quant for sensitive information and has either a reputation for talking, or an actual propensity to talk about what other quants do, it is less likely that the quant will or should trust this investor. After all, whatever the quant tells him is likely to get spread around the industry. At my firm, we hold quant managers' strategies in the strictest confidence. Often a quant will ask us what some other quant does. Our answer is universally and always that we will not discuss what others do, just as we do not discuss what the quant who asked us does. However, we've heard numerous stories and witnessed numerous firsthand examples of investors or managers passing along even reasonably proprietary bits and pieces of a quant's strategy to the industry. This is an ugly practice. 

The second lesson from The Interrogator is that it is hard to feel particularly justified in being secretive with information if the person asking questions already knows most of the possible answers. For example, Scharff knew the name of the pet dog at the home base of one pilot and the names of most of the pilot's colleagues. His goal in a given interview was to learn just a little bit more about his prisoners and their activities. They were frequently lulled into thinking that there was no point in keeping secrets, since their captor knew so much already. Though this never led to blatant "tell-all" behavior, it certainly allowed the interrogator to amass huge amounts of value from the interviews, a little at a time. It is possible to learn a similarly voluminous amount about quant trading without asking any particular quant to teach it to you in a meeting. This is helped along by the fact that most of what an investor needs to understand about a quant can be learned without compromising proprietary information. In this book, for example, we have outlined a great majority of the kinds of approaches quants use. None of this information is especially proprietary to any trader. A quant with any hope of being successful knows most of the material in this book already. In a sense, this book provides you with a great portion of the menu available to a quant. There aren't many dishes he can choose that aren't on this menu, which obviates the need for most of the secrecy. The investor can, in this way, learn about the specific items on the menu that the quant being interviewed has chosen and why these choices were made. For instance, understanding the kinds of alpha models the quant is using, whether they are relative or intrinsic, how fast he trades, and in what instruments and geographies tells the investor a great deal about what risks are being taken. This information is necessary for building a diversified portfolio and is largely sufficient for that exercise. 

The third and final lesson of The Interrogator is to be organized in the management of information when it is gathered. This greatly supports efforts to get new information but is also useful in ongoing evaluations of the quality of a given practitioner. Scharff's group developed a sophisticated, almost relational database system using index cards and a card catalogue file. (Remember, this was before the computer was invented.) As they got new information, they would organize it by linking it to other relevant cards in the file. For example, if they found out the name of another pilot from a given American base, they would tag that card with references to all the other information, including other pilots, from that base. This way, as they were interviewing a given pilot, they had a dossier that contained an impressive and extensive array of details, well organized and easy to access. These days we have powerful computers and databases to rely on, making such a job easier. 

Keeping information organized furthers the goal of developing deep domain knowledge, but it is also quite useful in ascertaining the “goodness” of a quant team over time. If every three months you ask a quant, for example, what types of research projects he is working on and what new pieces he has added to the model over the past three months, you should see a rational life cycle that repeatedly takes a robust research pipeline and turns it into implemented improvements to the strategy over time. If the quant has a process wherein modules that were not part of the research list from the past suddenly appear in production, this could be evidence of sloppiness in the research process. When visiting a quant’s office, it is useful to ask to see firsthand some of the various tools and software that the quant claimed to use or have developed in previous discussions. But, to be aware that you should be asking to see something specific, you had to have carefully managed the information about the nature of these tools and software to begin with. 

## EVALUATING A QUANTITATIVE TRADING STRATEGY

In my years of evaluating and creating quant trading strategies, I have noted an extraordinarily interesting fact: The work that a quant does is, in most ways, identical to the work that any portfolio manager, any CEO, or any other allocator of resources must perform. After all, these resources (e.g., time or money) are limited and must be invested in a way that results in maximum benefit. The process used to invest resources—the investment process—contains six major components: 

1. Research and strategy development 

2. Data sourcing, gathering, cleaning, and management 

3. Investment selection and structuring 

4. Portfolio construction 

5. Execution 

6. Risk management and monitoring 

You may note that these activities are closely parallel to the modules of the black box and the activities in and around its construction and management. This is because all these areas must be addressed in order for a quant trading program to function properly over time. One fact about computers, which we've addressed already, is that they do not do a good job of thinking about things you might have missed. As quant trading programs have evolved over time, they have had to address the myriad decisions that any portfolio manager must address. Too often, in discretionary management activities, important aspects of this process are left without sufficient analysis, and an ad hoc approach is taken. I've interviewed scores of discretionary stock pickers who can spin tremendous yarns about why they are long this stock or short another. But when asked how they decide how to size these positions in their portfolios, the answers are often vacuous, given without deep thought or analysis. 

Those charged with evaluating managers must thoroughly examine each of these areas. And quants, in general, should be willing to answer questions about each. A few examples of the kinds of questions I ask a quant follow: 

■ Research and strategy development 

■ How do you come up with new ideas for trading strategies? 

■ How do you test these ideas? 

■ What kinds of things are you looking for to determine whether a strategy works or not? 

■ Data sourcing, gathering, cleaning, and management 

■ What data are you using? 

■ How do you store the data, and why that way? 

■ How do you clean the data? 

■ Investment selection and structuring 

■ Are your alpha models theory driven or data driven? 

■ Which alpha strategies are you using (e.g., trend, reversion, value/yield, growth, or quality)? 

■ Are you making relative bets or a bunch of individual bets? 

■ If relative, what does relative mean, exactly? 

■ Over what time horizon, and in what investment universe? 

■ How are you mixing your various alpha models? 

■ Portfolio construction 

■ How do you do portfolio construction? 

■ What are your limits, and why did you set them there? 

■ What are the inputs to your portfolio construction? 

- What are you trying to achieve with portfolio construction (i.e., what is your “objective function”)? 

■ Execution 

■ What kind of transaction cost model are you using, and why did you choose to model transaction costs the way you did? 

■ How are you executing trades—manually or algorithmically? 

■ Tell me about your order execution algorithms: What kinds of things did you build into them (e.g., hidden vs. visible, or active vs. passive)? 

■ Risk management and monitoring 

■ What does your risk model account for, and why those things? 

■ What are your various risk limits, and why did you set them where you did? 

■ Under what circumstances would you ever intervene with your model? 

■ What are you monitoring on an ongoing basis? 

This is but a small sampling of the hundreds of questions I ask a quant. If he claims that the answers to such questions are proprietary, I do not simply accept that response. Rather, I try to ascertain why he thinks the answers are proprietary and try to make him understand why I need to know. Most quants I have met are sympathetic to the goals of an investor trying to understand a portfolio's exposures and whether the quant is skilled at his work. It comes back to building trust, having domain knowledge, and being organized in terms of the management of information. As I've said, the menu of things that quants can choose to do is reasonably easy to know. It is largely laid out in this book, and I am certain I've revealed nothing proprietary. A quant generally should not claim that he cannot disclose which items he has chosen from this menu. 

The investor has one more tool available for understanding a quant strategy, and that is the footprint left behind by the strategy: its return history. Imagine that an investor learns, by asking many questions such as those I've listed, that a quant is using a trend-following strategy on various individual instruments, with a six-month average holding period. When long-term trends are present, the strategy should do well. When longer-term trends reverse, the investor should see the strategy do poorly. In other words, the strategy's return pattern should corroborate the fundamental understanding that the investor has gained by asking many questions. 

# EVALUATING THE ACUMEN OF QUANTITATIVE TRADERS

If I have tried to stress anything in this book, it is that the judgment of a quant trader pervades the strategy she builds. So, an evaluation of the quant's skill and experience in the fields relevant to the trading strategy is obviously important, but it is also easier said than done. This section outlines a few tools that can be used to determine the skill level of quant traders. 

The people developing and managing quant strategies should be well trained in the methods they use. At least some members of the team should have substantial live experience in areas of quant trading relevant to the strategy they are currently pursuing. Experience helps drive good judgment, especially in light of the massive array of subtleties and traps inherent in the process of research and trading. From a dispositional standpoint, quants should be careful and cautious in their analysis, and they must be humble about their ability to predict the future. There are considerable hurdles to doing quant trading well, such as polluted data and constantly improving competition. A good quant does not underestimate such challenges. The reality is, however, that evaluating whether scientists know what they are talking about at a deep level is not the easiest task for someone who is not technically proficient. As such, to make a judgment, one may have to rely on the quant's qualifications and experience, reputation, history of success, and analyses of the investment process. Although this is a lot of work, the task is doable for those who want to undertake it. 

One of the handiest tricks I know of to evaluate a quant's skill is to dig deeply into the details in a few areas of her process. Why? The difference between success and failure is very commonly found in a large number of highly detailed decisions. If the mechanism used to make these decisions is flawed, the manager has little hope of success in the long run. Thus, an analysis of the investment process, and by extension its six major components, is focused on understanding what a quant does and, just as important, why the quant does it. As we discussed throughout this book, a number of approaches to quant trading can work. Momentum and mean reversion strategies can both work, even though they are opposites. Both intrinsic alphas and relative alphas can work. So it is important to understand what a trader does, but why she does it tells you about her judgment, her process, and her potential for future success. 

Each decision a quant makes in how she builds a strategy represents a source of potential differentiation from other traders, but also of potential success or failure. And it makes sense that this is the case. Many quants have large numbers of positions, frequently in the thousands, and most engage in strategies that turn these positions over relatively frequently—from once every few minutes to once every few months. If 5000 positions are turned over once a week, for example, this represents about 260,000 individual bets per year. Now imagine two equity traders, Trader A and Trader B. They have remarkably similar strategies, even in the details, and they each manage $500 million. For each dollar managed, they put on $2 of long positions and $2 of short positions so that each trader has a portfolio of $2 billion. Each turns over about 20 percent of her portfolio per day, or $400 million in dollar volume each day. They each average 10 percent returns per year. If Trader A is later able to optimize her executions such that she makes 0.01 percent more per dollar trades than she used to, either by being faster or improving transaction costs or the alpha model, this results in Trader A's annual return improving to 12 percent per year. This is 20 percent, or $10 million per year in profits, better than the result generated by Trader B, which is an enormous difference when compounded over time. Though some quants certainly do things that are plainly incorrect at a high level, the judgment of the quality of a given quant most often comes down to his decisions at a fairly detailed level. 

Another reason that the details matter so much is that there is really only a tiny amount of predictability in all the movements of the market. Quants usually depend on being right only slightly more often than they are wrong and/or on making only slightly more on winning trades than they lose on losing trades in order to generate profits. As such, small decisions that affect the probability of winning only slightly or those that skew the size of winning trades versus losing trades slightly can dramatically impact the outcome over time. 

Finally, if the quant has given deep and well-grounded thought to the details of the few areas that you spot-check, it is more likely that she has given deep thought to other areas of the quant trading process. This, too, improves her probability of success in the future, since we have shown that rigor is a key component of success in quant trading. Though it is likely obvious enough already, I want to make it clear that the fact that a quant has a Ph.D. in physics (or anything else) is no indication of quality or skill. Some of the brightest and most successful quants have no advanced degrees, and some of the biggest failures in quant trading have won Nobel Prizes. 

The flaw in focusing on the details of a quant strategy is that such details are less likely to be revealed to an investor during due diligence. Though the higher-level topics discussed in the section entitled “Evaluating a 

Quantitative Trading Strategy" might be relatively uncontroversial to discuss, the details are not. As I mentioned earlier, it is frequently the details that separate the best traders from the mediocre ones, and these details often boil down to knowhow more than, say, better math skills. So, quants are and probably should be somewhat more reticent to provide such details. Even if they were to provide details, the investor would have to be knowledgeable and proficient enough to pass judgment on them. In other words, to try to divine the quality of a quant's system from clues about such details requires significant experience on the part of the quant investor. After all, just as I require experience in my traders, I also benefit from experience in judging them. A great many things that seem plausible enough at first glance simply don't work. For example, just because a quant pays a lot of money to a data vendor for clean data, it doesn't mean that the quant should actually rely on the cleanliness of that data. The saving grace for the nonquantitative investor seeking to evaluate a quant is thoroughness and strong information management in the assessment and due-diligence process. 

## THE EDGE

In assessing a portfolio manager, including a quant, a key issue to focus on is the idea of an edge. We define an edge as that which puts the odds in favor of the portfolio manager succeeding. An edge can come from three sources, listed here in order of commonness: the investment process, a lack of competition or something structural. In investing and trading, an edge is not the same thing as a competitive edge. A trader might have absolutely no competitors, yet still manage to lose money. I've seen it more than once. An investment edge is thus more intrinsic than comparative. Still, competition does matter: A valid idea with a valid implementation might make little or no money if there is too much competition, whereas a mediocre strategy might make money if there is none. As such, one must ascertain the sustainability of a given trader's edge. The odds might be in the trader's favor today but against him tomorrow as the world changes or as competition increases, if the trader does not evolve. 

An investment process edge must come from one or more of the six components of the investment process we just outlined. Too often, when asking a discretionary stock picker what his edge is, we hear him say, "Stock picking." But this is merely a description of the activity, not evidence that the trader is any good at it. One must dig further into the reason that the trader claims to have an edge in any of these activities. For quant traders, most often an investment edge comes from experience and skill in conducting research and/or the acquisition or cleaning of data. This is because the goodness of the models for investment selection and structuring, portfolio construction, execution, and risk management is usually determined by the quality of the research and development process that created them. If some modules have not been particularly well researched, there is almost no chance that the trader will have an edge in these areas. An edge in research can derive from superiority in talent or process, but actual experience in conducting successful research in the financial markets is usually critical. In other words, one must have better people and/or a better process to put around these people, but in either case experience is needed. 

I have already described a bit about how to assess the people at a quant shop, but one more point bears mentioning. How a quant deals with adversity is critical to understanding his edge and its sustainability. There are times when the model simply doesn't make money. Knowing how and when to react to these episodes is critical. Too often quants react in a suboptimal manner to losses in their funds, and a knee-jerk reaction can often ruin whatever edge the strategy itself has. A sound approach to managing adversity starts with good monitoring tools, which allow the quant to pinpoint problems and work to solve them rather than panicking. It is unlikely that a trader has an edge because of monitoring, but it is easy to throw away a potential edge through insufficient or badly conceived monitoring processes. 

In terms of research, there are several hallmarks of a high-quality process. The process should be vigorous and prolific, and there must be an ability to translate models efficiently from research into production. This is because most quant models eventually decay into mediocrity, and successful ongoing research must be implemented in live trading strategies to stay ahead of this decay. The research process should also deal with issues such as overfitting and look-ahead bias, and the evaluator should ascertain exactly how the quant thinks about and deals with these critical issues. Finally, the process should at least largely follow the scientific method. In evaluating a quant trader, it is useful to ask many questions about how and why various elements of their strategy are the way they are. If a manager says he will close a position if it has moved 10 percent against him, ask him how and why he decided on 10 percent rather than 5 percent or 50 percent. If the quant says he is running a trend-following strategy in certain markets, find out why he picked a trend-following strategy, how he defines the strategy, and why he is using the markets he's using rather than other or simply more markets. These kinds of details will give you insight into the care with which a manager has developed the entirety of an investment strategy. 

A data edge can come from having proprietary access to some sort of data. Earlier in the book we gave the example of a company that uses geolocational data derived from GPS signals on cell phones to aggregate more real-time macroeconomic indicators. If, in fact, these data prove useful, they might be able to trade using this information, and they might then have a data edge. But in this era of technology and regulation, it is difficult to find sustainable data advantages. It is also possible to build a data edge through superior data gathering, cleaning, and storage techniques. Again, an interviewer should ask questions about where a trader gets his data, what work is done to clean the data, and how and why the data are stored in a certain way. Some answers will be thoughtful; others could indicate carelessness. 

This kind of data edge is quite similar to a lack-of-competition edge. But lack of competition is not a long-term plan. It is a truism in economics that, if higher-than-average profit margins can be had in some activity, more and more players will compete until the margins compress and normalize at levels more typical in the broader marketplace. This is likely to have happened already in at least two quant trading spaces: quant long/short and statistical arbitrage. However, once they become more competitive they also become more cyclical, and there are periods when players vacate the space because it offers too little reward, leaving more of the pie (and therefore better margins again) for the fewer players who remain. It is also important to ascertain why there is a lack of competition, when this is found. Some strategies are inherently more difficult for new entrants; others simply have not yet attracted the attention of new entrants. An example of the former, at least historically, can be found in purely quantitative options trading. This is not widely pursued because there are significant challenges associated with acquiring and cleaning data, structuring trades, and modeling the liquidity of options contracts. But this by no means implies that it cannot later become a crowded strategy with many competing firms chasing an ever-shrinking pie. 

As an example of the second option, I remember an experienced team that formed a hedge fund to trade corporate credit in Asia back in 2002. They had successfully carried out this strategy as proprietary traders at a bank for several years previously. They had few, if any, competitors, and their early years were very strong. Then, as time passed and more entrants to their niche crowded the field, they had to branch into other areas that were less appealing. Over time their edge, which was largely related to a lack of competition, was eroded. Ultimately the new areas into which competition forced them to participate caused a massive drawdown in their fund. The lack of competition was really due to a lack of discovery of their niche, and these are among the most fleeting kinds of edges. 

Structural edges generally relate to something in the market structure that puts the wind in the sails of a market participant. These are usually caused and removed by regulation. I once knew a trader in the pits of the New York Mercantile Exchange who ran a hedge fund that relied on his short-term discretionary trading. Because of his status on the exchange, he was able to supplement a reasonable investment edge with a structural edge that allowed him to transact very cheaply and extremely quickly. Over time, however, his markets went from being pit-traded to electronic, and his structural edge vanished. In quant trading, the most common sort of structural edge comes from liquidity provision, or the rebate, on ECNs. ECNs actually pay market participants for market-making activities by providing commission rebates. In certain cases I have seen the act of transacting become a profitable exercise for the trader, and this too is a structural edge. It is possible that, over time, payments by ECNs for order flow will dwindle, and this edge, too, will be eradicated. 

## EVALUATING INTEGRITY

Most quants, and most traders in general, are honest and ethical. Therefore, it is entirely reasonable to work with them on a “trust, but verify” basis. In other words, for most of the evaluation process it is reasonable to assume that the trader went to school where she claims, got whatever degree(s) she claims, and is generally not a criminal. But before making an investment, most observers would agree that to the extent possible, it’s worth verifying a quant’s ethics. 

Here we have a few tools at our disposal. First, do background checks, education verifications, and reference checks. In the case of backgrounds and education verifications, serious problems in a trader's personal or professional history should probably serve as a red flag. Of course, this is a tricky proposition. The investor must determine whether the mistakes or misdeeds in a quant's past served to "teach her a lesson," or whether they indicate a likely pattern of behavior that will repeat, even if not in exactly the same way. That judgment cannot be made universally for all cases. But I encourage the investor to consider this question only from one specific angle, which might help drive the answer: The job of the investor is not to judge the quant as a person but rather as a potential fiduciary, acting on behalf of the investor. Fiduciaries are bound to act in their clients' best interest and to be very open and up front about any potential conflicts of interest or anything else that could impede their fulfilling their duties to investors. Using the mentality of the fiduciary as a compass is something I have found helpful in a great many difficult circumstances. 

When performing reference checks, I find it useful to request references from existing investors whenever possible and to ask them not only why they like the manager but also what they think her weaknesses are. More helpful still is to seek out references that the manager did not provide herself. It is relatively easy for any trader to find a few people to say something nice about her. But it is much better if the trader is known by others, and those others are likely to provide much more useful input than the references a trader provides for herself. If you cannot locate such references in your own network, it sometimes helps to ask the references provided by the manager whether they know anyone else you can contact. 

It turns out that getting into details with quants helps demonstrate their integrity as well. Though even less skilled quants might have answers at hand for higher-level questions about their strategies and process, even someone intent on deceiving rarely thinks through low-level details sufficiently to be facile in answering questions about them. This is a common and successful interrogation technique in law enforcement. If you ask a suspected criminal where he was last night, it's not surprising to hear him quickly and convincingly provide an alibi, such as "at my girlfriend's house." But if you follow up by asking what time he arrived, how long he stayed, what movie he watched, what he ate and drank while he was there, and so on, he will have to make up answers to these questions he likely has not rehearsed beforehand. 

A quant who is lying to cover up a lack of skill would have to be an expert at making up answers to questions about details on the fly to keep up with questions about the details of her strategy. And some people are very good liars, to be sure. However, these answers also have to be able to stand up on their own. Answers that reveal a lack of understanding of the subject matter or answers that are internally inconsistent or are deficient in other ways should not be ignored. They might not lead you to conclude that the manager lacks integrity, but they should be sufficient to conclude that she isn't very good, which is itself sufficient for the purpose of avoiding hiring her. What's more, you can use the same technique of looking for details in assessing a quant's background as in assessing her strategy. If a quant says she completed her Ph.D. at Harvard, you can follow up by asking where she lived while she was there, what her favorite restaurants were, who her dissertation committee included, what her dissertation's title was, how many pages it ended up being, and so on. And again, many of these details should be verifiable with her alma mater. 

It is worth mentioning one more point about selecting managers, whether quant or not: Almost no trader is so special that it is worth investing in her strategy without gaining a reasonably deep understanding of it. It should not take much to say “no,” in other words, whereas it should take an incredible amount of confidence to say “yes.” Seeing a long and attractive track record should never be sufficient. In fact, I would put forth that it is significantly more important to get good answers to good questions than to see a long track record. If Bernie Madoff and the other scandals that have been announced on a nearly weekly basis since late 2008 provide any sort of lesson to investors, it must be that reputation and track record are not enough. 

No investor can validly claim that they understood how Madoff could have made such consistently positive returns based on the strategy he is said to have employed. Madoff never addressed questions, maintaining that his strategy (which was discretionary, not systematic) was too proprietary. Though insufficient to uncover all potentially fraudulent (or simply unprofitable) investments, the tools provided in this chapter can certainly help eliminate a great majority of them. These techniques should be used in conjunction with an equally rigorous operational due diligence process to further reduce the possibility of being victimized by fraud, malfeasance, or other misbehavior on the part of traders. 

## HOW QUANTS FIT INTO A PORTFOLIO

Assuming that you find a quant that is worth hiring or investing in, you have to decide how to allocate to this trader. To make this determination, you have to understand how the strategy fits in with the rest of your portfolio. This is largely a question of balancing the levels of various types of exposures. This section details some of the more important kinds of exposures associated with quant investing. 

## A Portfolio of Alphas

First, it is worth remembering that portfolio construction is about allocating to exposures. A portfolio that contains more kinds of exposures is more diversified than one that is concentrated among a smaller number of exposures. Investors must seek out the appropriate balance of trend, reversion, value/yield, growth, and quality to achieve optimal diversification. A quant doing trend following is not likely to be so incredibly different, from a portfolio construction viewpoint, than a discretionary trader who is seeking to identify trends. To be sure, the tireless vigilance of a computerized trading strategy might find opportunities that the human trader misses. In addition, the human trader might avoid some bad trades that are taken on by the computerized strategy out of naivete. But, as trend following in general goes, so it is likely that the human and computerized trader both go. So, at a primary level, the investor must diversify among various alpha exposures. In the evaluation process, the investor should be able to ascertain at least roughly the underlying alpha exposures of the various strategies in a portfolio. Using this information, the investor can allocate capital such that the blended allocations to various types of alpha are in line with the levels that the investor has determined are desirable. 

## Bet Structures

The second consideration relevant to portfolio construction is bet structure, as described in Chapter 3. Relative bets can behave very differently from single-instrument bets, particularly when these bet structures are used with different types of alpha models. When a quant strategy makes relative bets, it is inherently counting on the stability of the relationships among the instruments that are grouped together. This makes bet structure itself a source of risk in such strategies, and this risk becomes evident when the relationship between the instruments changes. In such environments, for example, relative mean reversion strategies are prone to losses. On the other hand, single-instrument mean reversion frequently benefits from large regime changes. This is because this strategy tends to bet against the prevailing trend while remaining indifferent to the destabilizing effects of a large trend reversal on the relationships depended on by a relative alpha strategy. This is but one example of how bet structures can impact results and, as a result, the investor's portfolio. In short, it is worthwhile to diversify across various bet structures as well, even within the same domain of alpha exposure (e.g., relative and intrinsic mean reversion). 

## Time Horizon Diversification

Finally, the investor must balance her exposure across time horizons. In general, it is my experience that longer-horizon quant strategies—those that hold positions for more than a week or so—tend to go through longer and streakier performance cycles. They can outperform or underperform for several quarters on end, and it can take several years to evaluate whether there is really a problem with the manager. Some longer-term strategies also demonstrated conclusively that they are subject to crowding risk, as seen so vividly in August 1998 and August 2007. While this might make them a bit less desirable, one can manage significantly more money in such strategies, which is sometimes a practical necessity. 

Short-term strategies, by contrast, tend to be very consistent performers, but they cannot handle much capital. They are therefore very desirable but also not always practical. Furthermore, when one does find a good short-term trader to invest in, it is not clear that the trader will remain small enough to be effective on short time scales. Many traders are tempted to grow their assets when assets are available, and this demands attention on the part of the investor. 

## Summary of Portfolio Considerations

Quants can be valuable components of a portfolio. The investor must realize that quants are ultimately not so different than their discretionary counterparts and therefore that the list of things that matter to building a portfolio that includes quants isn't much different than it would be without quants. As with all things related to portfolios, the key is to build a diversified portfolio that considers three important elements: 

1. Various types of alpha exposures 

2. Various bet structures 

3. Various time horizons 

It is interesting to note that these considerations closely mirror the taxonomy of theory-driven alphas, presented here again as Exhibit 12.1. Equally interesting, I do not believe that the investment universe (asset class, instrument class, or geography) nor various other subtleties about the models (e.g., model specification or run frequency) are particularly impactful in portfolio construction. These variations add a great deal of diversity when markets are behaving normally, but in stressful times they simply matter a lot less than distinctions along the lines of the three portfolio considerations listed here. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-16/b74d9460-d262-40b2-8f52-997285641037/c08fb019759248311cb726fd7e77072123e346ba5acbdb5ea619b706baad1d29.jpg)



EXHIBIT 12.1 Taxonomy of Theory-Driven Alpha Strategies and Implementation Approaches


## SUMMARY

To assess a quant trader and a quant strategy, one must understand the strategy being implemented and the quality and vigor of the process that generates strategies. To do this, the investor has three weapons at her disposal: building trust, gaining as much knowledge as possible about quant trading, and keeping information he learns as organized as possible. These tools can be used to extract and piece together information on a given quant, and on quant trading generally. 

Ultimately, an investor has to determine whether a quant has an edge, what the sources of this edge are, how sustainable the edge is, and what could threaten it in the future. Edges come from people and/or processes, and it is in these areas that the evaluation of a quant must focus. Once quants have been vetted, they should be thoughtfully included in a portfolio. It is important to diversify across different approaches to alpha generation, different time horizons, and bet structures to complement best the other components of the investor's portfolio. 

I remember once interviewing a senior employee at one of the best quant shops in the world. I asked him how on earth they had done so well, which of course was a sort of stupid question. His answer, however, was both concise and seemingly on target. To quote him, loosely: "There is no secret sauce. We are constantly working to improve every area of our strategy. Our data is constantly being improved, our execution models are constantly being improved, our portfolio construction algorithms are constantly being improved ... everything can always be better. We hire the right kinds of people, and we give them an environment in which they can relentlessly work to improve everything we do, little by little." 

# Looking to the Future of Quant Trading

All evolution in thought and conduct must at first appear as heresy and misconduct. 

—George Bernard Shaw 

The black-box trading strategy has existed for over three decades. This book has provided you with the tools necessary to understand this niche of the investment community, perhaps for the first time. From its earliest days in trend-following applications to the most recent and state-of-the-art high-frequency machine learning strategies, the field of quant trading has evolved considerably since its early days. Yet recently it is hard to ignore the travails the quant trading field, particularly in equity market-neutral strategies, has undergone. Starting in July 2007 and sporadically again in 2008, large swaths of the quant trading universe have delivered poor results, unprecedented downside risk, and easy headlines for those who love to hate them. 

Regardless, other niches within the domain of quant trading—and even some of the types of quants whose peers have done poorly—have thrived. Assets have flowed vigorously into systematic futures trading strategies, which outperformed during the aforementioned tumult of mid-2007 through late-2008, having benefited from the price trends that formed the bear market in equities. High-frequency equity traders have profited from increased volatility and liquidity in the markets. Even some that share a label with the statistical arbitrage and quantitative long/short practitioners who have suffered the most still, nonetheless, have managed to deliver solid returns with limited risk. Overall, it is safe to say that quants, whether in futures, equities, or options, are among the star performers of the 2008 credit crisis. 

Yet, the need for quant traders to evolve remains as great as ever. In fact, given the speed with which technology and markets are changing, it is likely that the need to evolve has never been greater. Most quants spend a disproportionate amount of time on their alpha models. This is understandable; these models are indeed the engine of success for a quant strategy. Yet so much of the theory-driven alpha space is already so well understood that little progress is likely to be made in this arena. Perhaps for a short while, the application of relatively standard alpha models to new markets, such as the smaller developed markets in Asia and Europe, or even to developing markets around the world, can bear fruit. But there are few barriers to entry to running a strategy in another country or asset class. Some interesting research is being done in pockets around the industry to uncover new and untapped approaches to alpha generation. Perhaps new forms of alpha can be invented and exploited. But these, too, are likely to be somewhat readily accessible to others. 

The rest of the black box, however, has been comparatively neglected by most researchers in the industry. Relatively naive, frequently ineffective approaches are used to blend alpha models together, to size positions correctly and to manage risk. These are fields of research in which little useful literature has been published, and the landscape is currently wide open for innovation. And some fields of study within the quant trading industry have been ignored almost entirely. Analysis of self-generated data—such as transaction data that captures the behavior of markets just before, during, and just after one trades—can be fruitful but is very rarely done. It is possible to learn a great deal about what works and what doesn't by objectively analyzing one's own track record. Models that predict whether certain strategies are likely to perform well or poorly in the future are also somewhat uncommon, outside of very naive performance-chasing algorithms that increase allocations to strategies that have done well recently. In short, all the myriad decisions a quant must make in building a system should be made with the benefit of more research and study than has been done by most firms so far. 

The manner in which quant trading systems are used, too, can evolve. There are already examples of hybrid quant-discretionary strategies, which utilize quant systems to screen for opportunities while allowing discretion to rule the rest of the process. But more work can be done to ascertain whether certain other parts of the investment process can combine human subjectivity with the objectivity and consistency of machines. For example, it is easy to imagine analysts inputting their views into a computer system and allowing the system to determine the portfolio. In other words, instead of using machines to support human decisions, human input could support systematic decisions. 

Finally, the structure of firms that utilize quant trading strategies can evolve. Historically, firms that have amassed working capital have provided a place for a quant to interact with other quants in building trading strategies, to take orders from a secretive central officer on specific projects that hide the strategy's full scope even from the employees, or simply to use the firm's capital to run a strategy that was developed previously and elsewhere. Meanwhile, smaller boutiques have toiled away in small offices around the world, rarely having any contact with others. There appears to be room for a "quant collective" structure, which would offer the economies of scale afforded by larger shops, such as clean data, fast and reliable market connectivity, and powerful and fast research tools. Meanwhile, such collectives in theory could offer more autonomy and upside potential for the individual quant than a more traditional structure. This structure also may align quants sufficiently that they are encouraged to seek help from their fellow members on subjects in which they may be less strong while keeping proprietary those elements of their own strategy that are most unique. 

In addition to the general requirement to evolve in order to survive, great challenges face the quant trader today. Regulations are becoming increasingly hostile as both quant trading and hedge funds are demonized in the popular press. Government interventions, rare events (such as the credit crisis that began in mid-2007), and geopolitical events that impact the markets have all presented significant difficulties for many quants, since these events typically cause past behavior to cease to explain future behavior. Many alternative investment professionals are turning away from quant trading in disgust after more than a year of repeated “once-in-a-lifetime” events. For quants, this may be a period of “natural selection,” in which the weaker or less lucky firms are forced out of the business while the stronger or luckier firms can survive only if they evolve. 

So, the need to evolve is clear. But given both the difficulty of the market environment over the past few years and the (absolutely misplaced) negativity surrounding hedge funds in general and quant funds in particular, there might never have been a time more critical than this in which to differentiate good quant traders from bad ones. The good news for those who are looking is that there are more than a few good ones out there to be found. With the framework provided in this book, the job of understanding what quant traders do, discerning which ones are more likely to succeed, and ascertaining how to use them in a portfolio is hopefully a bit easier. 

## CHAPTER 1 Why Does Quant Trading Matter?

1. "Hot Models Rev Up Returns," M. Corey Goldman, HFMWeek.com, April 17, 2007; "Goldman Sachs, AQR Hedge Funds Fell 6% in November (Update3)," Jenny Strasburg and Katherine Burton, Bloomberg.com, December 7, 2007. 

2. "Renaissance Waives Fees on Fund That Gave Up 12%," Gregory Zuckerman, Jenny Strasburg, and Peter Lattman, Wall Street Journal Online, January 5, 2009. 

3. "Goldman Sachs Paydays Suffer on Lost Leverage with Fed Scrutiny," Lisa Kasse-naar and Christine Harper, Bloomberg.com, October 21, 2008. 

4. "New World Order: The High Frequency Trading Community and Its Impact on Market Structure," Sang Lee, The Aite Group, February 2009. 

5. "Black Box Trading Has Huge Potential—D. Boerse," Peter Starck, Reuters.com, June 13, 2008. 

6. "Does Algorithmic Trading Improve Liquidity?" Terry Hendershott, Charles M. Jones, and Albert J. Menkveld, April 26, 2008. 

7. www.turtletrader.com/trader-simons.html. 

8. "The Disposition to Sell Winners Too Early and Ride Losers Too Long: Theory and Evidence," Hersh Shefrin and Meir Statman, The Journal of Finance, Volume XL, No. 3, July 1985. 

## CHAPTER 2 An Introduction to Quantitative Trading

1. "For Wall Street's Math Brains, Miscalculations," Frank Ahrens, Washington-Post.com, August 21, 2007, p. A01. 

2. "Not So Smart Now," Roddy Boyd, New York Post.com, August 19, 2007. 

3. "The Swensen Plan," Marcia Vickers, Money.CNN.com, February 24, 2009. 

4. Famous Movie Detectives III, Michael R. Pitts, Scarecrow Press, 2004, p. 265. 

## CHAPTER 3 How Do Quants Make Money? Answer: Alpha Models

1. www.turtletrader.com/trader-seykota.html. 

2. "Game Theory Applications," Larry Hite and Steven Feldman, The Commodity Journal, May–June 1972. 

3. "Making a Mint: How a Scientist, Statistician and Businessman Mixed," Ginger Szala, Futures, March 1, 1989. 



4. “Renaissance Man: James Simons Does the Math on Fund,” Gregory Zuckerman, The Wall Street Journal, July 1, 2005. 



5. "The Cross Section of Expected Stock Returns," Eugene Fama and Kenneth French, Journal of Finance, June 1992, Vol. XLVII, p. 427. 



6. "Anomalies in Relationships Between Securities' Yields and Yield-Surrogates," Ray Ball, Journal of Financial Economics, 1978, Vol. 6, Issue 2–3, pp. 103–126. 



## CHAPTER 4 Risk Models

1. Uncertainty has broadly been adopted as being synonymous with risk. There is usually not much justification for its use, other than expediency for the purposes of relatively easy computations to answer the question, How much risk is there? However, it seems clear that variability is more than acceptable when it is positive, though not desirable when it is negative. Some have therefore proposed to use the negative deviation, which computes the volatility only of the negative returns in a time series, but this strikes me as plainly silly. Standard deviations should be used only when the distribution of the values is expected to be normal, or at least symmetric around the mean. Negative returns almost never meet this criterion. Furthermore, the variability of negative returns is not the same thing as negative variability, and it is only the latter that really characterizes risk. Focusing on the measurement of the variability of negative returns, for example, could lead an investor to love a strategy that loses 100 percent of your money any time it loses at all. Yes, there is no variability among the losers in such a system. But how is that helpful? Instead, the likelihood of losing significant sums (what I called negative variability) of money actually matters, whether the losses are spread across a wide spectrum or levels or are concentrated at a particularly unappetizing level with no variability. 

To address this point, there are various measures of downside risk, such as maximum peak-to-valley drawdown, but these measures have weaknesses too. First, they are not defined by fixed periods and therefore do not work well in most linear statistical frameworks. Some strategies can have very sharp drawdowns that occur over a small number of days. Others can have protracted periods of losses, where the amount lost on any day might not be large, but over the course of a year the losses add up to a large number. This implies that they are less convenient to use in a great many computational exercises, because most analyses of data series are based on the presumption that each point in the data series represents the same amount of time as each other data point. There are only a few techniques that allow an analyst to compare a single day with an entire year, for example. Second, having a valid and useful drawdown statistic depends on having enough of a data set that you are confident you have seen the outer limits of the strategy's risk. 

2. This concept was formalized in the Kelly criterion, in a paper by John L. Kelly, Jr., in the Bell System Technical Journal in 1956. The Kelly criterion provides a systematic way of sizing the risk taken on each of a series of bets based on the bettor's edge, which maximizes the expected gains by the end of the series of bets. The edge is defined as a combination of the payoff for winning and the odds of winning. This concept has been widely applied in gambling and somewhat in investing. The noted quant Edward Thorp is credited with first applying the Kelly criterion to trading strategies. However, some critics of the Kelly betting strategy point out that a critical assumption of this criterion is that each bet is expected to be independent of the next, which is true in many forms of gambling, for example. However, in investing, bets can be serially correlated, which is to say that returns to investment strategies tend to be streaky. As such, in general many investors who believe in the concept of the Kelly criterion use a derivative version of the strategy, such as "half Kelly," to bet less than Kelly suggests. Useful background on Kelly and the criterion can be found on William Poundstone's web site or in his book about Kelly, called Fortune's Formula. 

3. This phenomenon exists, if for no other reason, because the value investor tends to buy stocks that have fallen in price, which tend therefore to have experienced a shrinkage in their market capitalization. A market-neutral value investor would also tend to sell expensive stocks, which are likely to have rallied and therefore will have experienced market capitalization appreciation as well. 

4. Principal components analysis (PCA) is a statistical technique used to reduce the complexity of a set of instruments down to a manageable set of "risk factors," each of which is called a vector. Each vector represents a statistically derived systematic risk among the instruments and is derived by analyzing the historical relationships among all the instruments in the set. 

## CHAPTER 6 Portfolio Construction Models



1. "Portfolio Selection," Harry Markowitz, The Journal of Finance, Vol. 7, No. 1, March 1952, pp. 77–91. 





2. "Generalized Autoregressive Conditional Heteroskedasticity," Tim Bollerslev, Journal of Econometrics, Vol. 31, June 1986, pp. 307–327. 





3. "Global Portfolio Optimization," Fischer Black and Robert Litterman, Financial Analysts Journal, September–October 1982, pp. 28–43. 





4. Active Portfolio Management: A Quantitative Approach for Producing Superior Returns and Controlling Risk, Richard Grinold and Ronald Kahn, McGraw-Hill, 1999. 





5. Efficient Asset Management: A Practical Guide to Stock Portfolio Optimization and Asset Allocation, Richard Michaud, Oxford University Press, 2001. 



## CHAPTER 7 Execution

1. Not all exchanges work exactly this way. For example, some legacy equity option exchanges prorate executions among all option orders at the same price and give better priority to customers versus market makers—although these rules are undergoing review for possible change. Furthermore, quants rarely transact in such markets, and if they do, it does not usually involve utilizing systematic execution engines such as those described in this book. 

## CHAPTER 8 Data

1. "Navigation Team Was Unfamiliar with Mars Climate Orbiter," Greg Clark and Alex Canizares, Space.com, November 10, 1999. 

2. SEDOL stands for Stock Exchange Daily Official List, which is a list of ostensibly unique security identifiers for stocks in the United Kingdom and Ireland. Other common security identifiers in equity markets are the International Securities Identification Number (ISIN) or Committee on Uniform Security Identification Procedures (CUSIP) number. CUSIPs are primarily relevant for U.S. and Canadian stocks. Many data vendors utilize their own proprietary security identifiers as well. 

3. For the sake of simplicity, we are ignoring any “split effect,” which many people believe exists; this theory states that stocks tend not to fall as much as expected based on the size of the split because people like to buy nominally lower-priced stocks. 

4. In science, this is known as a Type I error, which is to accept a false-positive result in testing a hypothesis. This is the error of believing a hypothesis is true when in fact it is false. 

5. In science, this is known as a Type II error, which is to accept a falsely negative result in the outcome of a test. This is the error of believing a hypothesis is false when in fact it is true. 

## CHAPTER 9 Research

1. From Richard Donchian's Foundation web site: www.foundationservices.cc/RDD2/. 

## CHAPTER 10 Risks Inherent to Quant Strategies

1. The macroeconomic environment around this time, and for some time thereafter, favored companies that are in “growth” industries. During this period, that meant those positively linked to commodity prices, such as oil companies or gold-mining companies, and those in businesses that are less dependent on economic cycles, such as telecommunications firms. 

2. When Genius Failed, Roger Lowenstein, Random House Inc., 2000. 

## CHAPTER 11 Criticisms of Quant Trading

1. A study by Pertrac, the hedge fund industry's leading database and performance analytics provider, was cited by the Medill Reports' John Detrixhe on August 14, 

2008. The article can be found at http://news.medill.northwestern.edu/washington/news.aspx?id=97223. 

CHAPTER 12 Evaluating Quants and Quant Strategies 

1. The Interrogator: The Story of Hanns Scharff, Luftwaffe's Master Interrogator, Raymond F. Toliver, AERO Publishers, 1978; Schiffer Publishing, 1997. 

# About the Author

Rishi K Narang is the founder and portfolio manager of Telesis Capital LLC, a boutique alternative investment manager specializing in short-term quantitative alpha strategies. He has been involved in the hedge fund industry variously as an investor in and practitioner of quantitative trading strategies for over 13 years. 

When he isn't working, Rishi enjoys playing his guitar, writing essays and poems, making pencil sketches, arguing with people, playing tennis and hiking. Rishi completed his undergraduate degree in Economics at the University of California at Berkeley. He lives in Los Angeles with his wife, Dr. Carolyn Wong. 

Academic literature, 127–128
Accidental risks, 9
Accounting scandals, 36
Active Portfolio Management (Grinold/Kahn), 92
Adaptiveness, empirical risk models, 63
Aggressive orders, 101–103, 105, 190
Aite Group, 5
Algorithmic execution, 5
Algorithmic trading, 6, 201
Algorithms, types of:
learning/genetic, 46, 94
machine learning, 46
order execution, 16, 100–105
All-or-none orders, 101
Alpha, generally:
defined, 55
exposure, 149
forecasts, 93
models, see Alpha model(s)
portfolio, 198, 200–201
signal, 135
time decay of, 137–138
Alpha model(s):
applications of, generally, 21–22, 54
blending, 48–54
characteristics of, 15–16, 21–22, 67
data-driven, 37–38
forecasting, 92
information processing, 111
model risk, 150, 153
portfolio optimization, 87, 92–93, 95–96
risk management, 60–61
significance of, 203
strategy implementation, 38–48
theory-driven, 24–37, 48
types of, 22–24, 187
Alpha-oriented strategies, xiv, 7, 13
Amaranth, 179 

Amazon.com, 180–181
Ameritrade, 155
Analyst(s):
expectations, 36
functions of, 204
recommendations, 137
sell-side, 36
Annual/annualized returns, 4, 139
Anti-correlated instruments, 89
Arbitrage, types of, 6–7, 12, 62, 129, 160, 164, 179, 195, 203
Arbitrageurs, 7, 164
Architectural errors, 153–154
Arms race. See High-frequency trading
Art/science debate, 169–170
Asian currency crisis, 172
Asset allocation, 80
Asset classes, 15, 43–44, 59, 65, 61, 159, 166, 172, 176, 201, 203
Asset management, 5
ATM effect, 160, 162–163
Australia, 178
Automated trading:
benefits of, xiii, 170
execution of, 5, 16
functions of, 3
Average rate of return, 132–133
Axcom, 27–28 

Back-history, 119, 121
Back-of-the-envelope analysis, 21
Backtesting, 120–121, 132
Bad prints, 118
Bailout packages, 173–174
Balance sheets, 114, 173
Ball, Ray, 33
Bamberger, Gerry, 29
Banking industry, credit risk model, 9
Bank of America, 13–14
Bankruptcy, 173 

Bank stocks, 36, 82
Bar charts, 135
Barclay Group, 5–6
BARRA, 166
Basis points, 100
Bear markets, 127, 174, 203
Bear Stearns, 159
Benchmarks, 21
Berlekamp, Elwyn, 27–28
Beta:
    exposure, 149
    implications of, 32
    strategies, characteristics of, xiv
Bet shops, 178
Bet structure:
    characteristics of, 39, 42–44, 47
    high-probability, 105
    importance of, 199–201
    limitations, 57–59
    risk exposure, 56
Bid/ask spread, 29
Bid/offer prices, 71, 101–103, 153
Biotechnology stocks, 44
Black, Fischer, 91
Black box, see Black box schematics;
    Black-box trading strategy
    alpha models, 21–54
    defined, 17, 111
    risk models, 55–65
Black box schematics:
    alpha model, 53
    data, 123
    execution model, 109
    portfolio construction model, 96
    research, 145
    risk model, 65
    transaction cost model, 78
Black-box trading strategy:
    characteristics of, 5, 13
    implementation of, 7
    origins of, 12, 203
    schematics, see Black box schematics
Black-Litterman optimization, 91–92
Bond market:
    alpha model applications, 47
    influential factors, 25, 34, 44, 62, 157
    risk management, 59, 61–62
Book value, 114
Book value per share, 34
Book-to-price ratio, 32, 34 

Boutique quant traders, 4, 6, 165, 178–179, 205
Breakout, trend strategies, 45
Brokerage houses, 36. See also Brokers
Brokers:
    commissions/fees, 46, 68–69, 100
    functions of, 99–100, 178–179
    online, 155
    trading infrastructure, 107
Buffett, Warren, 22, 62
Bull markets, 127
Burning data, 143
Buy orders, 5, 101
Buy strategies, 29

Calmar ratio, 136–137
Cancelled orders, 105
Capital markets, xiii, 5, 9, 14, 143, 169
Carry trades, 33–34
Cash bonds, 44
Cash-flow statement, 114
Cause-and-effect relationships, 50
Caxton, 179
CDOs, xiv
Charles Schwab (SCHW), 29–30, 154–155
Charts/charting:
    risk monitoring, 167
    test model metrics, 132
Cheap stocks, 8, 22, 56, 130, 180
Chhikara, Sudhir, 123
Citadel, 179
Clearing process, 68–69
Closing price, 63
Colocation, 107
Commissions, 15, 46, 68–69, 144
Commodities trading advisors (CTAs), 26, 174
Commodity market, 62, 157
Commodity trading, 47
Commodity trading advisors (CTAs), 5
Common investor risk, 159–166, 168
Comparative advantage, 45
Competition, significance of, 37, 193, 195
Complex quantitative trading strategies, 12
Compounded returns, 133
Computer(s):
    automated trading, xiii, 3, 5, 16, 170
    electronic market, 5, 45
    hardware systems, 108
    software, see Software programs 

Computerized trading strategies, 170. See also Software programs
Conditional models, blending alphas, 51–52
Confidence intervals, 59
Consensus building, 25
Consumer spending, 25
Contagion risk, 159–166, 168
Contrarians, 29
Convertible bonds, 45
Corporate bonds, 45, 61
Corporation, as data source, 116
Correlation coefficients, 135, 151
Correlations, portfolio construction, 43, 58, 87–91, 93, 162, 177
Cost minimization, 77, 100
Countertrends, 25, 176
Covariance, 58
Credit crisis of 2008, 9, 36–37, 160, 173, 203
Credit spreads, 162
Criticisms of quant trading:
art/science debate, 169–170
data mining, 179–182
handling market changes, 174–176
large quants can thrive in long run, 178–179
underestimating risk, 171–174
similarities/differences in quants, 176–177
Cross-asset yield, 161
Cross-border yield, 161
Cross the spread orders, 102
Crowded trade effect, 162–163
Cumulative profits, 132
Currency exchange, 118–119
Currency market, influential factors, 62, 157
Currency trading, 5, 47, 114

Daily volume, influential factors, 12
Data:
asynchronicity, 120–121
cleaning, 117–122, 189, 195
collection methods, 114
importance of, 111–113
incorrect, 113, 117–122
management of, 189
missing, 117–118
nature of, 112
sources of, 115–116
storage, 112, 122–123
types of, 113–115 

Database, as information resource. See Data
Data cube, 123
Data-driven alpha model:
    applications, 37–38
    blending with theory-driven model, 48–53
    implementation of, 38–48
    theory-based alpha model compared with, 37–38
Data-driven risk models, 58
Data edge, 194–195
Data feed handlers, 111, 150
Data miners/mining, 23, 38, 46, 58, 94, 170, 179–182, 189
Data sourcing, 189
Debt crisis, historical 9
Decision makers, evaluation of, 185
Decision trees, 83–85
Deleveraging, 165
Dennis, Richard, 128
D. E. Shaw, 128, 170, 179
Developing markets, 203
Directional forecast, 54, 93
Direct market access (DMA), 99–100, 107
Discretionary investment style, 8, 10, 12–13, 204
Discretionary traders, characteristics of, 24, 28–29, 31, 35, 100, 129, 172, 182, 199–200
Discretionary trading, 185, 204
Dispersion, risk model, 58–59
Disposition effect, 10
Diversity/diversification:
    alpha models, 39, 47–49, 54, 137, 161
    importance of, 199–201
    risk models, 61
Dividends, 119
Dividend yield, 32
Dodd, David, 34, 49
Donchain, Richard, 27, 127
Dot-com bubble, 22, 28, 173
Dow Jones Industrial Average, 172
Downtrends, 41
Drawdowns, 81, 83, 87, 133–134, 136–137, 172–173, 195
Due diligence, 193

Earnings before interest, taxes, depreciation, and amortization (EBITDA), 34
Earnings per share (EPS), 35–36
Earnings quality, 36 

Earnings yield (E/P), 32–33, 51, 130–131
Eckhardt, William, 128
Economic cycles, 172
Edge:
data, 194–195
defined, 193
identification of, 201
lack-of-competition, 195
monitoring and, 194
structural, 195–196
Efficient Asset Management (Michaud), 93
Efficient frontier, 86
Efficient markets, 6
Einstein, Albert, 126–127, 141
Electronic Communication Networks (ECNs), 72, 99, 104, 196
Electronic markets, 5, 45
Electronic matching networks, 69
Electronic trading, 99–100, 108
Emerging markets, 45, 161
Empirical risk models, 61–65
Empirical scientists, 23–24
Enron, 36
Enterprise value (EV), 34
Equal risk, 51
Equal-weighting, 51, 93
Equilibrium, 25, 29
Equity indices, 44
Equity investments, see Equity trading growth strategies, 35–36
value trades, 34
Equity market-neutral strategies, 96, 144–145
Equity market-neutral traders, 177, 203
Equity markets, 5
Equity risk premium, 11, 135
Equity traders, 9, 29, 166, 203. See also Equity market-neutral traders
Equity trading:
elements of, 59, 114
portfolio optimization, 95
risk management, 59
risk models, 63
volume and, 3
E*Trade, 155
Europe:
quant trades/trading, 8, 45
stock market hours, 121
European Central Bank, 34 

European Xetra electronic order-matching system, 5
EUROSTXX Index, 16
Excess risk, 15
Exchange-traded funds (ETFs), 156
Exchanges:
as data source, 115
fees, 69
order execution, 101–102
Execution:
components of, 99–100, 109, 189
high-frequency trading, 105–107
model risk, 150, 153–154
monitoring, 166–167
order execution algorithms, 16, 100–105
trading infrastructure, 107–109
Exogenous shock risk, 158–159, 168, 172
Exotic options, 13
Expectations, analyst, 36
Expected correlation/correlation matrix, 86, 88–91
Expected returns, 39, 54, 57, 87, 95
Expected volatility, 87
Expensive stocks, 56, 130, 180
Exposure monitoring tools, 166
Factor portfolios, optimization strategies, 92–93
Failed quants, 4, 6
False signals, 38
Falsification, 126
Fama, Eugene, 31–32, 34
Fama-French three factor model, 32, 34
Fat tails, 151
Federal Reserve, 4, 34, 63, 181
Fed funds rate, 4
Fees, types of, 4, 28, 68–69, 100, 144
Fidelity Investments, 108
Fiduciaries, 196
Filled orders, 100–101
Fill rate, 167
Fill-or-kill orders, 101
Finance industry, 91
Financial distress, 160
Financial Information eXchange (FIX) protocol, 108
Financial market, near-collapse in 1998, 9
Financial Select Sector SPDR, 174
Financial statements, 114, 116, 120
Financial stocks, 174 

FIX engine, 108
Fixed income securities, 44, 61
Flat file databases, 122
Flat transaction cost models, 73–74
Flight-to-quality investments, 36
Forecasting:
alpha model approaches, 25, 39, 42–44, 47, 49–51
data mining, 180
equity trading, 60
high-frequency, 59
implications of, 9, 15, 29, 38, 45
risk models, 59
scientific method applications, 126–127
Foreign exchange markets, 5, 38, 44
Foreign exchange trading, 35
Francioni, Reto, 6
Free cash flow, 36
French, Kenneth, 31–32, 34
Fundamental data:
growth, 30, 35–36
overview, 30–32
quality, 30, 36–37
sources of, 113–114, 116
value/yield, 30, 32–35
Fundamental strategies, 7, 36
Futures contracts, 118–119
Futures market, 15, 27, 38, 44
Futures trading, 5–6, 26, 31, 203
Game theory, 27
Generalized autoregressive conditional heteroskedasticity (GARCH), 87–88
General relativity theory, 126–127
Geography, investment universe, 44, 188, 201
German bund, 119
German 10-Year Bonds, 16
Global Alpha Fund, 5
Global market, 150
Global stocks, 8
Going long, 60. See also Long/short strategies
Gold, 42
Goldman Sachs, 5, 128
Good-till-cancelled orders, 101
Government, generally:
bonds, 61, 114
as data source, 116
Graham, Benjamin, 34, 49 

Great Depression, 172–173
Greater fools theory, 26
Greed, 173
Gross domestic product (GDP), 35–36, 112, 114
Grouping techniques:
alpha model, 42–43
risk model, 58–59, 61
Growth investing, 24, 35–36, 164–165
Growth stocks, 156–157, 161, 175–176
Guerilla strategy, 106

Hard-to-borrow lists, 144
Head and shoulders pattern, 129
Hedge funds, 3, 5–6, 27, 43, 77, 162, 174, 177, 179, 195, 205
Hedging, 60
Heuristics, 42–43, 79
Hidden orders, 104, 106, 190
Highbridge, 128
High-frequency traders/trading, 3–4, 38, 41, 47, 105–107, 117, 144, 203
High-quality companies, 36
High-rank stocks, 34–35
High-yield stocks, 33, 51, 55–56
Historical data, 32, 36, 61, 92, 117, 130, 145, 151, 154, 174, 180, 183
Historical regression, 50–51
Historical trends, 126–127
Historical volatility, 87–88
Hite, Larry, 27
Hit rate, 167
Holding periods, 181–182
Hong Kong, 44, 178
Housing market, 25. See also Mortgage industry; Real estate
Human behavior, 170
Human discretion/judgment, 13–14, 17, 64–65, 191
Human Genome Project, 23

Iceberging, 104, 106–107
Iceland, 173
Idea generation, 127–129
Illiquidity, 45, 160
Implementation programs, 6, 10, 18
Implied volatility, 172
Improving, 103
Incentive fees, 28
Income statement, 114 

Index funds, 7
Indexed flat files, 122
Individual investors, 161
Industry groups, 42–43, 89, 122
Inflation, 25
Information, see Data gathering, 189 management, 193 ratio, 136
Infrastructure: errors, 167–168 trade execution, 107–109
Input/output model, 111
In-sample testing, 129–131, 142–144
Insider information, 102
Institutional investors, 161
Instrument class, 44, 188, 201
Insurance industry, 173
Interest rate risk, 61
Interest rates, 34–35, 181
Internet bubble, 62, 143, 155
Internet stocks, 70. See also Technology stocks
Interrogator, The (Toliver), 186–188
Intraday, generally: data, 38, 63, 120 ticks, 38, 106
Intrinsic alpha, 96, 187, 191
Intrinsic bets, 43
Investment decisions: alpha forecast applications, 21–54 based on inaccurate information, 13 influential factors, xiv, 10, 17 systematic approach to, 13–14
Investment horizon, 161. See also Time horizon
Investment strategy: conception of, 12–13 influential factors, 8
Investment universe, 39, 44–47, 53, 190, 201
Investor(s): attrition, 178 capital, 161 individual, 166 institutional, 166 market-neutral, 166 nonquant, 7, 46 quality, 24, 36–37 

retail, 77, 161
systematic, 10
Iraq War, economic impact of, 62, 159

Japan, quant trading in, 45, 164
Joining, 103

Lack-of-competition edge, 195
Large-cap securities, 8, 61, 77, 153, 161
Leverage, 14, 7, 37, 59–60, 160–163, 173
Limit order book, 101
Limit orders, 101–104, 15, 167
Linear forecasting, 49–51
Linear relationship, 151–152
Linear transaction cost models, 74–75, 77
Liquidation crisis (August 2007), 5, 7, 56,
153, 161–167, 171, 175
Liquidity:
implications of, 16, 28, 44–45, 71–73, 77,
102, 104, 160, 164
pools, 104–105
Liquid quant strategies, 166
Live production trading system, 17
Long position, 61, 163
Long/short strategies, 144–145, 161,
163–164, 203
Long Term Capital Management (LTCM), 4,
8–9, 56, 160–161, 169, 172, 179
Long-term strategies, 41
Look-ahead bias, 120–121, 143, 195
Losing trades, 56, 68, 192
Low-rank stocks, 34–35
Low-yielding stock, 51, 55–56
Lumpiness, test model metric, 132–133

Machine learning:
algorithms, 46
characteristics of, 94, 203
forecasting model, 49–50, 52
techniques, 46, 106
Macroeconomics, 35, 112, 114, 121, 195
Macro traders/trading, 5, 31
"Made-to-order" risk factor, 64
Madoff, Bernie, 197–198
Management fees, 28
Manias, 28, 172
Margin calls, 160
Market capitalization, 32, 90, 166
Market capitalization risk, 61 

Market conditions:
impact of, 3, 46, 77, 162
risk models and, 62–63
transaction cost models, 77
Market conditions, changes in, 174–176,
182. See also Regime changes
Market direction risk, 60, 71
Market dislocations, 174–176
Market exposure, measurement of, 9
Market inefficiencies, 6–7
Market liquidity, 7. See also Liquidity
Market makers, 73, 77
Market-neutral investors, 166
Market neutral trading, 128
Market neutral value model, 61
Market-on-close order, 101
Market orders, 71, 100–101, 103
Market pricing, 7
Market risk, 63
Market timing, 45
Markowitz, Harry, 85, 128, 136
Mars Climate Orbiter (MCO), 112
Mathematical models, 150
Mean reversion:
implications of, 43, 70, 106
trading strategies, 28–31, 37, 72, 81, 154,
159, 191
Mean variance optimization, 86, 128
Medallion Fund, 4
Medium-term strategies, 41, 47
Merger arbitrage, 160
Mergers, 13–14
Merrill Lynch (MER), 13–14, 29–30,
154–155
Mexican bonds, 34
Mexican currency crisis, 118, 172
Microeconomic growth strategy, 35
Microsoft (MSFT), 137–138
Microstructure alphas, 105
Millennium Partners, 129
Mint Investments, 27
Misspecification, 153
Model risk:
defined, 150
implementation errors, 150, 153–154
inapplicability of modeling, 150–152
model misspecification, 150, 153
Modern portfolio theory (MPT), 86
Momentum portfolio, 92 

Momentum strategies, 25, 106, 164–165, 191
Money market funds, 173–174
Monte Carlo simulation, 93–94
Mortgage industry, 173
Mortgage-related businesses, 37
Moving average:
characteristics of, 45
crossover, 26–27, 126–127
trend following strategy, 40–41
Moving the market, 45–46, 70
Multi-security bets, 43
Multiple regression, 50
Multistrategy hedge funds, 162, 179
Mutual funds, 49, 59, 77 

Naked short sale, 145
Natural selection, 205
Negative market impact, 71
Negative trends, 26, 45
News agencies, as data source, 116
Newton, Isaac, gravity theory, 126
New York Stock Exchange (NYSE), 115
Nikkei 225, 89, 93, 121–122
Nonlinear forecasting, 49–51
Nonlinear relationship, 151–152
Nonquant investors, 7, 46
Normal distribution, 151
Northfield, 166 

Objective function, 79, 86–87, 94, 190
Occam's razor, 141
Oil prices, 65
Omega ratio, 136
100-day moving average, 41
Opaqueness, 12, 18, 46
Opening price, 137
Optimization, see Portfolio optimizers/optimization constrained, 91
unconstrained, 91, 95
Optimizers, in portfolio construction, 79
Options trading, 13, 195, 203
Order books, 101, 106
Order execution algorithms:
aggressive vs. passive, 101–103, 105, 190
cancelling orders, 105 

Order execution algorithms (Continued)
    characteristics of, 29, 100–101
    hidden order vs. visible order, 104, 106, 190
    large order vs. small order, 103
    replacing orders, 105
    where to send orders, 104–105
Order management system, 108
Order placement. See Order execution algorithms
Out-of-favor exposure, 149
Out-of-sample testing, 129, 142–144
Outperformance, 7, 60–61, 130, 157, 178, 180, 199
Over-the-counter (OTC) market, 45
Overbought/oversold securities, 28
Overfitting, 46, 139–142, 181–182
Overvaluation, 34, 92

Pairs trading, 7, 12–13, 42
Panics, 172
Parsimony, 141
Passive orders, 101–103, 190
Paulson, Henry, 173
Penalty functions, size of position, 57–58
Percentage winning trades, 136
Performance statistics, 5
Permutations, 47
Piecewise-linear transaction cost models, 75–76
Playing the market, xiv
Popper, Karl, 126, 141
Portfolio bidding, 100
Portfolio construction:
    elements of, 53, 188
    importance of, 80, 204
    model, see Portfolio construction model quantitative analysis of, 86
    risk exposure and, 56
    size of portfolio, 21, 189
    techniques, 49
    transaction costs, 67–73
Portfolio construction model:
    balance considerations, 79
    elements of, 15, 18
    goal of, 79
    information processing, 111
    model risk, 150, 153
    optimizers, 79–80, 85–95 

output of, 95
quantitative, 79
rule-based, 79–85, 97
run frequency, 201
selection factors, 96–97, 189
specification of, 201
transaction costs, impact of, see
Transaction costs
Portfolio insurance, 169
Portfolio management, day-to-day, 13
Portfolio of strategies, 137
Portfolio optimizers/optimization:
byproducts of, 94–95
inputs to optimization, 87–94
objective function, 86–87
theoretical influences, 85–86, 91–93
Position limits, constraints and penalty, 57–59
Positive carry, 34
Positive market impact, 71
Positive trend, 27
Predictive power, 133–135, 183
Price data:
defined, 113
sources of, 115–116
Price discovery, 7
Price/earnings-to-growth (PEG) ratio, 35
Price target, 39
Price-to-earnings (P/E) ratio, 7–8, 32–33, 139
Primary data vendors, 115–117
Princeton/Newport Partners, 29, 170
Principal component analysis (PCA), 62
Private equity, 59
Profitability, 46
Profit and loss monitoring, 166–167
Profit curve, 133
Profit margins, 195
Programming errors, 153–154
Proprietary data vendors/generators, 116
Proprietary information, 187
Proprietary trading desk, 3, 6, 161–162
Publicly traded companies, 36
Pulte Homes (PHM), 163, 165 

Quadratic curve, 73
Quadratic transaction cost models, 75–77
Quality:
investors, 24, 36–37
significance of, 30 

Quant(s), generally:
    characteristics of, 12–14, 17–18
    collective structure, 205
    defined, xiii
    equity investments, 35–36
    evaluation methods,
    information-gathering, 186–188
    funds, 11, 205
    future directions for, 203–205
    trading strategies, see Quant strategies evaluation
Quant long/short (QLS), 34–36
Quant strategies evaluation:
    benefits of, 185–186
    components of, 188–191
    edge, 193–196
Quant trader(s):
    characteristics of, 10
    defined, xiii
    evaluation of, see Quant trader evaluation reference checks, 196–197
    success factors, 10, 191–193, 196–198
Quant trader evaluation:
    acumen, 191–193
    edge, 193–196, 201
    integrity, 196–198
    portfolio fit, 198–201
    questions to ask, 189–190
Quantitative Investment Management, 4
Quantitative risk models, 57
Quantitative trading system:
    benefits of, 7–8, 55
    conception of 12–13
    high-frequency of, 3
    implementation of, 6, 10, 18
    long/short positions, 34–36
    performance of, 3–4
    risk measurement/mismeasurement, 8–10
    strategy evaluation, see Quant strategies evaluation
    typical structure of, 14–18
    volume per day, 5
Quasi-quant traders, 14

Ratings agencies, 173
Real estate, 173
Real-time data, 117, 120
Real-time runs, 47
Rebate programs, 72 

Recession economy, 35
Refitting, 46
Regime change:
impact of, 182–183
risk, 154–158, 168, 174–176
Regulations, importance of, 205
Regulators, as data source, 115
Relational database, 122–123, 188
Relative alpha strategy, 43, 55–56, 60, 90, 159, 187, 191
Relative bets, 43
Relative mean reversion strategy, 154
Relative value, 43–44, 164
Relative value equity arbitrage, 160
Renaissance Technologies, 4, 7, 27, 128–129, 170
Resampled efficiency, 93–94
Research:
constant, 127
evaluation methods, 194–195
idea generation, 127–129
importance of, 3, 14–15, 17–18, 38, 46, 58, 125, 146
mistakes in, 146
organization of, 188, 201
scientific method, 125–127, 140, 195
strategy development and, 189
testing strategies, 129–145
Researchers, success factors, 142
Resource allocation, 185
Retail investors, 77, 161
Return vs. risk ratios, 136–137
Returns:
expected, 39, 54, 57, 87, 95
risk-adjusted, 86, 136, 154, 182
risk vs., ratios of, 136–137
total, 45, 139
variability of, 133, 136
Risk, generally:
aversion, 63, 86
exposure to, see Risk exposure
management, 13–14, 17–18, 33, 55, 182, 204
measurement, 58, 81, 162
mitigation, 61
model of, see Risk models
monitoring, 166–168, 189
-taking strategies, 6, 65
targeting, 162
underestimation of, 171–174 

Risk exposure:
common investor risk, 159–166, 168
contagion risk, 159–166, 168
exogenous shock risk, 158–159, 168
impact of, 8, 15, 22, 55–56, 60, 65,
regime change risk, 154–158, 168,
174–176
types of, 149, 168
Risk models:
amount of risk, limitations of, 57–60
characteristics of, 15–16, 18, 56, 67, 153
information processing, 111
types of risk, limitations of, 60–64
Risk-adjusted return, 86, 136, 154, 182
Risk-adjusted returns, 86
Risk-free rate, 136
Riskless profit, 6
Rolling out-of-sample technique, 142
Rolling yearly correlation, 89
Rotation models, blending alphas, 51–52
Rothman, Matthew, 177
Royal Dutch, 160
R-squared (R²), 135, 142
Rube Goldberg device, 11
Rule-based portfolio construction models:
alpha-driven weighting, 82–83, 95
decision-tree models, 83–85
equal position weighting, 80–81, 93
equal risk weighting, 81–82, 95
overview of, 80, 85, 97
Rumors, economic impact of, 14, 159
Run frequency, 39, 46–47, 201
Russian debt crisis, 9, 160, 172
Salomon Brothers, 108
S&P 500, xiv, 13, 16, 26–27, 28, 31, 40–41,
88–89, 94, 121, 131–135, 138–139,
151, 158, 181
S&P Growth index, 156–157
S&P Value index, 156–157
Scientific method, 125–127, 140, 195
Scientists, types of, 23
Secondary data vendors, 115–117
Secretive quantitative trading strategies, 12
Sector:
bets, 56, 60
defined, 122
risk, 61
Securities and Exchange Commission (SEC),
159, 174 

Securitized mortgages, 150–151
Security Analysis (Graham/Dodd), 34
Security master, 116
SEDOL code, 116
Sell orders, 5, 71, 101
Sell strategies, 29
Sensitivity, 139
Sentiment-based strategy, 36, 154–158
Sentiment data, 114
Settlement, 68–69
Seykota, Ed, 27, 170
Shark strategy, 106
Sharpe, William, 86, 136
Sharpe ratio, 136
Shaw, David, 29
Shell, 160
Short positions, 34, 164
Short selling, 13, 25, 37, 51, 55, 60, 144, 163, 174
Short-term strategies, 41, 47
Short-term traders, 174
Signal-mixing models, of alphas, 53
Signal strength, 39
Silver, 42
Simons, James, 7, 28
Simulation, 92. See also Monte Carlo simulation
Size-limited models, 58–59
60-day moving average, 41
Size of position:
limiting, 57
market impact and, 70–71, 167
significance of, 189
transaction costs, 77–78
Slippage, 69–72, 144, 167
Slow-moving strategies, 47
Small-cap stocks, 61, 77, 82
Smart order routing, 104–105
Sniper strategy, 106
Software programs:
alpha model, see Alpha model(s)
back-testing, 150
checking data errors, 120
CRM, 180
FIX protocol, 108
implementation errors, 153–154
risk exposure monitoring, 166
risk models, 64
transaction cost estimates, 73
Soros, George, 172 

Specialists/specialization, 44, 47, 73  
Spike filters, 118–119  
Sponsored access, 107  
SPY, 121  
Standard deviation, 58, 133, 151  
Standard operating procedures, 14  
Statistical arbitrage (stat arb), 7, 12, 29, 164, 178, 195, 203  
Statistical learning algorithms, 107  
Statistical significance, 63  
Statistical techniques, 42–43, 61–62  
Sterling ratio, 136  
Stochastic volatility modeling, 87  
Stock market crash, of 1987, 4–5, 174  
Stock/stock investment, ranking of, 34–35  
Stock/stock market: alpha model applications, 47  
asynchronicity, 121–122  
decline in 2008, 173, 177  
fundamental data, 114  
influential factors, 8, 62–63  
risk management, 59  
stock picking, 189  
stock splits, 119  
Stop-limit orders, 101  
Stop-loss policy, 129  
Structural edges, 195–196  
Supply and demand, 6, 29, 70–72  
Swaps, 44  
Swensen, David, 11–12  
Systematic approach: abandonment of, 13  
alpha model, 44  
defined, xiii  
frontiers of, 13  
futures trading, 20  
to problem solving, 7  
trading rules, 129  
Systematic decisions, 204  
Systematic investors, 10  
Systematic risk, 61–62, 64  
Systems performance monitoring, 166–168  

TABB Group, 5  
Tartaglia, Nunzio, 29  
Technical traders, 129  
Technological advances, economic impact of, 114  
Technology sector, 90  
Technology stocks, 56, 82 

10-Qs, 120
Terrorist attacks, economic impact of, 14, 158–159, 172, 180
Tertiary data vendors, 116–117
Testing, in research:
assumptions of, 144–145
"good" model, 131–139
importance of, 129
in-sample, 129–131, 142–144
out-of-sample, 129, 142–144
overfitting, 139–142
Theoretical scientists, 23–24
Theory development. See Idea generation
Theory-driven alpha model:
applications of, 22–24
blending with data-driven model, 48–53
fundamental data, 30–37
implementation of, 38–48, 200, 204
price-related data, 24–30
taxonomy of, 25, 48, 200
Theory-driven approaches. See Theory-driven alpha model;
Theory-driven risk models
Theory of gravity, 126
Thorp, Ed, 29
Time decay, 137–139, 195
Time horizon, 30, 38–42, 45, 47, 176, 181, 190, 199–201
Time period, winning, 133
Timestamps, 120
Total return, 45, 139
Trade deficits, 25
Trading desk. See Proprietary trading desk
Trade execution. See Execution
Trading periods, amount of, 181–182
Transaction cost:
commissions, 68–69
defined, 68
determination of, 190
estimation of, 73–75, 77, 144–145
execution and, 101–102
fees, 69, 100, 144
graphs, 73–76
high-frequency trading, 105–107, 144
influential factors, 166
market impact, 44, 46, 53, 70–72, 144, 167
minimization of, 68, 77, 101
models, see Transaction cost models slippage, 69–72, 144, 167 

Transaction cost models:
    construction considerations, 71
    elements of, 15–16, 187
    information processing, 111
    model risk, 150
    overview of costs, 68–72
    role of, 67–68, 77
    types of, 72–77
Transaction data, 204
Trend following:
    development of, 127
    evaluation of, 194
    exogenous shock risk, 158–159
    futures market, 15
    implications of, 15–17, 21–22, 25–28, 39
    moving average and, 40–41
    slippage, 69–70
Trend indentification, 22
Trend model, 51
Trend reversals, 81, 154, 157–159, 176, 199
Trust-building, 186–187, 201
Tulip mania, 28
Turnover rate, 18
Turtles program, 128
Two Sigma, 128, 170

Uncertainty, 25, 56, 58, 133
Underperformance, 22, 60, 79, 130, 157,
    178, 199
Undervaluation, 22, 29, 33–34
Unequal weighting, 80–81
U.S. Treasuries:
    Treasury bills, 70
    Treasury bonds, 62
    Treasury notes, 131
    10-year Treasury Notes, 16
Unwinding positions, 165
Uptrends, 71
Upward triangle pattern, 129

Valuation ratios, 100
Value at risk (VaR), 59, 151, 161–163, 171
Value funds, 23
Value/Growth spread, 156–158, 175–176 

Value-hunting strategy, 56
Value investing, 22, 30–35, 43, 55–56
Value stocks, 156–157, 161, 175–176
Variability of returns, testing metric, 133, 136
Variance, 86
Visible orders, 104, 190
VIX, 172
Volatility:
day-to-day management of, 56
defined, 58
forecasts, 93
historical, 172
impact of, 162–163
portfolio construction and, 82, 86–88, 97
prediction of, 135
risk model, 59
risk underestimation and, 171–172
significance of, 72
transaction costs and, 73, 77
Volume, significance of, 3, 5, 12, 113

Wall Street, 9
War, economic impact of, 62, 159, 172
Weak-growth economy, 35
Weighting:
impact of, 51–52
in portfolio construction, 80–83
portfolio optimization, 92–93
White paper, 108
William of Occam, 141
Winning trades:
characteristics of, 192
testing metric, 136
Working capital, 205
WorldCom, 36
World markets, 4
Worst-case scenarios, 171
Worst peak-to-valley drawdown(s), 133–134, 136

Yield:
implications of, 30–35
model, 51–52 