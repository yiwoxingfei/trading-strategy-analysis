

<!-- === Source: MinerU_markdown_Baddeley_M.C.,_Barrowclough_D.V._-_Running_Regressions__A_Practical_Guide_to_Quantitative_Research_in_Economics_._-CUP_(2009)_1_2122707855927779340.md (Page 1) === -->

RUNNING REGRESSIONS 

A Practical Guide to Quantitative Research in Economics, Finance and Development Studies 

M.C.BADDELEY aNd D.V.BARROWCLOUGH 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/70d5bdb412953019f7c84a8bfcd668836ba9cfc3ab8a54f65d8a2777599e9c21.jpg)


‘This book shows how econometrics can be of real value to understanding major global problems such as violent conflict and poverty. With an easily readable style, the book encourages everyone to try their hand at running regressions. 

## Professor Anthony Addison

Executive Director, Brooks World Poverty Institute, University of Manchester 

‘Running Regressions … combines statistical analysis with the relevant theories and their economic policy implications. [It] encourages the reader to see the relevance and importance of empirical analysis, and also allows the reader to see the links between theory and empirical analysis in a clear and consistent way. The writing and presentation style is very user-friendly and accessible. 

## Professor Philip Arestis

University of Cambridge 

‘Michelle Baddeley and Diana Barrowclough have written an outstanding book for undergraduate economists. It offers a well-structured introduction to econometric models via a series of illuminating applications. Readers see not only the statistical tools themselves, but also how they can be used to address important questions in economics. Students will welcome the seamless integration ofeconomic and statistical theory in an accessible manner, and teachers will appreciate how effectively the book shows the relevance of econometrics to economics. 

## Dr Nicholas Fawcett

University of Oxford 

‘This is an exceptionally readable and interesting book. Students now have an econometrics text that they will enjoy. It shows, by way of example, the power and usefulness of econometric analysis. 

## Professor Bernard Fingleton

University of Strathclyde 

‘For students of politics and international relations, Running Regressions demystifies an often daunting set of analytical tools and provides practical, critical advice on how to use them. 

## Dr Carolyn Deere

Global Economic Governance Programme, University College, Oxford 

## Running Regressions

A Practical Guide to Quantitative Research in Economics, Finance and Development Studies 

Running Regressions introduces social science undergraduates, particularly those studying economics and business, to the practical aspects of regression analysis, without adopting an esoteric, mathematical approach. It shows that statistical analysis can be simultaneously straightforward, useful and interesting, and can deal with topical, real-world issues. Each chapter introduces an economic theory or idea by relating it to an issue of topical interest, and explains how data and econometric analysis can be used to test it. The book can be used as a self-standing text or to supplement conventional econometric texts. It is also ideally suited as a guide to essays and project work. 

Michelle Baddeley is Director of Studies (Economics), Fellow and College Lecturer at Gonville and Caius College, Cambridge. She is the author ofInvestment: Theories and Analysis (2003). 

Diana Barrowclough is a senior economist, Office of the Secretary General, United Nations Conference for Trade and Development (UNCTAD). She formerly lectured economics at the University of Cambridge, where she was a fellow of St John’s College. 

A Practical Guide to Quantitative Research in Economics, Finance and Development Studies 

Michelle Baddeley 

Gonville and Caius College, Cambridge 

Diana Barrowclough 

United Nations Conference for Trade and Development (UNCTAD) 

cambridge university press Cambridge, New York, Melbourne, Madrid, Cape Town, Singapore, São Paulo, Delhi Cambridge University Press The Edinburgh Building, Cambridge CB2 8RU, UK 

Published in the United States of America by Cambridge University Press, New York 

www.cambridge.org Information on this title: www.cambridge.org/9780521603089 

© M. C. Baddeley and D. V. Barrowclough 2009 

The right of M. C. Baddeley and D. V. Barrowclough to be identified as the author of this work has been asserted by them in accordance with the Copyright, Designs & Patents Act, 1988. 

This publication is in copyright. Subject to statutory exception and to the provisions of relevant collective licensing agreements, no reproduction of any part may take place without the written permission of Cambridge University Press. 

First published 2009 

Printed in the United Kingdom at the University Press, Cambridge 

A catalogue recordfor this publication is available from the British Library 

Library ofCongress Cataloguing in Publication Data Baddeley, Michelle, 1962– Running regressions : a practical introduction to OLS in economics, finance and development studies / by Michelle Baddeley & Diane Barrowclough p. cm. Includes index. ISBN 978-0-521-84211-2 (hdbk.) – ISBN 978-0-521-60308-9 (pbk.) 1. Econometrics. 2. Least squares 3. Regression analysis. I. Barrowclough, Diana. II. Title. HB139.B34 2009 330.01<sup>0</sup>519536–dc22 

2009007332 

ISBN 978-0-521-84211-2 hardback ISBN 978-0-521-60308-9 paperback 

Cambridge University Press has no responsibility for the persistence or accuracy of URLs for external or third-party internet websites referred to in this publication, and does not guarantee that any content on such websites is, or will remain, accurate or appropriate. 

This work represents the personal views of the authors and is not the official view of the United Nations or its member states. 

To my parents (M.C.B.) 

To my family (D.V.B.) 

## Contents

List of figures page xi
List of tables xiii
List of boxes xv
Acknowledgements xvii
List of acronyms xviii
How to use this book 1
Part I Simple regression and data analysis 9
1 An introduction to Ordinary Least Squares 11
2 Running simple regressions: Global poverty and economic growth 36
3 Using logs and estimating elasticities: Demand for air travel 64
4 Hypothesis testing: Health expenditure and the quality of life 86
Part II Multiple regression and diagnostic testing 107
5 Multiple regression analysis: Housing demand in the UK 109
6 Heteroscedasticity: R&D, invention and innovation 133
7 Autocorrelation: Tourism and the environment 157
8 Model misspecification: Tobin's q and investment in the USA 178 

Part III Time-series econometrics 199
9 Structural breaks, non-stationarity and spurious regressions: Venture capital and computing investment in the USA 201
10 Error correction models: Consumption and the multiplier in the UK 225
Part IV Advanced topics 247
11 Panel estimation: Divorce and income 249
12 Binary dependent variables: War and poverty 264
Index 280 

## Figures

1.1 Line of best fit page 17
1.2 Sampling distributions for unbiased estimator A and biased estimator B 23
1.3 Sampling distributions showing minimum variance estimator $\hat{\beta}_{A}$ 23
1.4 Sampling distributions for a consistent estimator 24
2.1 Poverty and growth 45
2.2 Line of best fit 48
3.1 Elasticity varies along a linear demand curve 71
3.2 Constant elasticity of demand curve: linear vs. logged scales 72
3.3 Rising global air travel, 1991–2004: rising demand and falling price 80
3.4 Scatter plot of air travel demand (in passenger miles) suggesting constant elasticity of demand for air travel 80
4.1 Health interventions in Tanzania: money spent did not match health needs 91
4.2 Life expectancy for a cross-section of countries, 1999 94
4.3 Health spending for a cross-section of countries, 1998 97
4.4 Longer life expectancy associated with larger health expenditures 100
5.1 UK house prices and mortgage lending, 1975Q1 to 2008Q1 116
5.2 Actual vs. fitted values from estimation of Equation (5.3a) 126
6.1 Invention vs. innovation: the pyramid of innovative activities 135
6.2 Summary Innovation Index, 2004 138
6.3 Patents by country, ranked by R&D expenditure 143
6.4 Actual and fitted values from estimation of Equation (6.2) 144
6.5 Actual vs. fitted values from Equation (6.2) for observations 1–20 145
6.6 Actual vs. fitted values from transformed model (Equation (6.11)) 153 

7.1 International aviation emissions and international tourist arrivals, 1971–2003 163
7.2 EViews plot of residuals from estimation of Equation (7.2) 167
8.1 Adjustment costs and optimal investment 180
8.2 Corporate investment and Tobin's q, USA 1987–2004 186
8.3a lin-log specification 189
8.3b log-log specification 189
8.3c lin-lin specification 189
9.1 Computing investment vs. venture capital disbursements, USA 1980–2004 208
9.2 Actual vs. fitted computing investment, 1980–2004 210
9.3 Parameter shifts across a sample 211
9.4 Venn diagram of non-stationary processes 216
10.1 Real consumption and real disposable income – UK 1979–2005 233
10.2 Aggregate average propensity to consume (APC), UK 1979–2005 233
10.3 Scatter plot of consumption against income, UK data 234
11.1 Scatter plot of divorce rates vs. personal income, USA 2002–4 254
12.1 Conflicts and wars, 1992–2003 268
12.2 Involvement in armed conflict, by income category 268
12.3 Calculating the Gini coefficient 270
12.4 Logit function 274 

## Tables

2.1 Relative incomes of rich and poor page 40
2.2 Changing poverty (Y) and GDP growth (X): regression by hand 47
2.3 Measuring the sums of squares to estimate $R^2$ 55
2.4 A development target and its indicators 59
2.5 Different indicators reveal a different picture 62
2.6 Change in poverty, exports of goods and services, and investment 63
3.1 Elastic demand from leisure travellers, inelastic from business 75
3.2 Data on aviation demand and revenue 76
3.3 Example of an Excel output table 81
4.1 Infant mortality, life expectancy, and public expenditure on health 93
4.2 Excel output table 100
5.1 Summary of EViews printout 123
6.1 EViews output table: OLS regression 140
6.2 EViews output table: White's heteroscedasticity test 148
6.3 EViews output table: model with homoscedastic errors 153
7.1 EViews output table: OLS estimation 164
7.2 Decision rules for the Durbin–Watson (DW) test 168
7.3 Breusch–Godfrey LM tests from EViews 171
7.4a GLS estimation of tourism arrivals and aviation emissions (Cochrane–Orcutt procedure) 174
7.4b Breusch–Godfrey LM test 174
8.1 Summary of EViews output tables from estimations of Equations (8.4), (8.5) and (8.6) 191
9.1 Unit root tests (with constant and linear trend) 221
9.2 Summary of EViews printout 222
10.1 Illustrating the multiplier effect 227
10.2 Differing estimates of MPC and the multiplier 229 

10.3 Augmented Dickey-Fuller unit root tests 235  
10.4 EViews output: Keynesian consumption function 236  
10.5 EViews output: Friedman's permanent income model 237  
10.6a EViews output: ARDL Model 242  
10.6b EViews output: error correction model (ECM) 242  
11.1 EViews output from the pooled estimation 255  
11.2 EViews output from fixed effects estimation using dummy variables 260  
12.1 EViews output from estimation of the linear probability model 272  
12.2 EViews output from estimation of the logit model 276 

## Boxes

1.1 Types of data page 13
1.2 Calculating variances and standard errors 19
1.3 Statistical indicators of reliability 22
1.4 Gauss–Markov assumptions – mathematical notation 26
2.1 The Millennium Development Goals (MDGs) 37
2.2 ‘Doing’ development economics 38
2.3 Poverty and development: the record so far 41
2.4 The standard errors of the parameter estimates 50
3.1 Types of goods: Normal versus inferior, ordinary versus Giffen 68
3.2 Own-price elasticities of demand 70
3.3 Logs and elasticities, model specification 72
3.4 Existing evidence shows heterogeneity in patterns of demand for air travel 74
4.1 Health surveys in Tanzania: information as the best medicine 91
4.2 Measuring healthiness: The Quality of Life Index and the Human Development Index 96
4.3 The F test of explanatory power 102
5.1 House price indices and hedonic pricing 115
5.2 Using seasonal dummies to capture seasonality 118
5.3 Multiple regression analysis (MRA) 121
5.4 Joint hypothesis tests 128
6.1 Mirror mirror on the wall, who is most innovative of all ... 137
6.2 Correcting heteroscedasticity 149
7.1 Measuring the environment 162
7.2 Generalised least squares (GLS) to correct autocorrelation 171
8.1 Measuring market value and efficient markets 182
8.2 Incentives to invest: $q_{\text{M}}$ and $q_{\text{A}}$ 184 

8.3 Model misspecification errors 187  
8.4 Detecting model misspecification using Ramsey's RESET test 190  
8.5 Inefficient markets and behavioural economics 194  
9.1 Structural breaks, parameter instability and Chow tests 211  
9.2 Unit roots and non-stationarity 215  
9.3 Testing for non-stationarity 218  
10.1 Using lags 230  
10.2 The link between an ARDL and an ECM 239  
11.1 Economics and happiness 251  
12.1 Game theory and the strategy of conflict 266  
12.2 Measuring inequality: Gini coefficients and Lorenz curves 270  
12.3 Logit and Probit 273 

# Acknowledgements

Any imprecision and all mistakes/omissions remain our own. However, we do gratefully acknowledge the help of numerous people from Cambridge University Press: including Liz Davey, Lynn Dunlop, Phil Good, Chris Harrison and Pat Maurice. Thank you also to Fran Robinson for compiling the index, and to our copy editor – Jon Billam. We have also benefited from helpful substantive comments from various readers including Peter Batchelor (UNDP), Tony Addison and Charles Gore (UNCTAD) as well as anonymous reviewers. We would like to thank Chez Hall (Department of Engineering, Cambridge University) for his invaluable advice in our research into aircraft emissions, and the International Civil Aviation Authority for data on airline passengers and revenues. 

We also thank the generations of Cambridge University undergraduates whom we have had the pleasure to know and to teach; and whose curiosity and enthusiasm inspired us to write this book. The ‘toolbox’ outlined in Running Regressions offers a fascinating and increasingly relevant way to improve our understanding of topical world issues, and we hope that these pages will continue to spark our students’ (and graduates’) interest. Some who helped directly by commenting on early drafts of chapters included Arun Advani, Philomena Aw, Bruce Chen, Nicholas Fawcett, Oliver de Groot, Heather Katsonga Phiri, Dominique Lam, Nathan Lang, Raymond Lung, Adrian McMullan, Sarah Miller, Sarah Murphy, Natasha Prasad, Stefanie Stantchev, Daniel Thomas, Jon Waters, Hai Li Wu and Sophie Yu. 

Finally, warm gratitude is owed also to our families and friends for their patient and seemingly endless support and encouragement during the long (and sometimes arduous!) process of writing and producing this book. 

## Acronyms

ADF Augmented Dickey Fuller test APC Average Propensity to Consume BEA Bureau of Economic Analysis (US) BG Breusch–Godfrey LM test for Serial Correlation CI Confidence Interval CIA Central Intelligence Agency CLT Central Limit Theorem CML Council of Mortgage Lenders (UK) df Degrees of freedom DF Dickey–Fuller Test DGP Data generating process DW Durbin–Watson test ESS Explained sum of squares GDP Gross Domestic Product GLS Generalised Least Squares GM Gauss–Markov GQ Goldfeld–Quandt test HDI Human Development Index HPI Human Poverty Index IBRD International Bank for Reconstruction and Development ICT Information and Communication Technologies IDA International Development Association IEA International Energy Agency IMF International Monetary Fund IPCC Intergovernmental Panel on Climate Change IT Information Technology LDC Least Developed Country LPM Linear Probability Model LRE Long Run Elasticity MDG Millennium Development Goal 

xviii 

MLE Maximum Likelihood Estimation MPC Marginal Propensity to Consume MPC-UK Monetary Policy Committee (UK) MRA Multiple Regression Analysis NCHS US National Center for Health Statistics NGO Non Governmental Organisation OLS Ordinary Least Squares ONS Office of National Statistics (UK) PDI Personal Disposable Income QLI Quality of Life Index R&D Research and Development RSS Residual sum of squares SME Small/Medium Sized Enterprise SML Survey of Mortgage Lenders SRA Simple Regression Analysis SRF Sample Regression function TSS Total Sum of Squares UNCTAD United Nations Conference for Trade and Development UNDP United Nations Development Program UNWTO United Nations World Tourism Organisation WLS Weighted Least Squares 

# How to use this book …

A minority of students relish the prospect of studying econometrics, as many are deterred perhaps by the technical jargon e.g. ‘autocorrelated disturbances’, ‘heteroscedasticity’ and ‘identification problems’. The aim of Running Regressions is to apply the practical aspects of elementary regression analysis to some interesting issues and without adopting an excessively esoteric and/or mathematical approach. Running Regressions shows that statistics and econometrics can be straightforward, useful and interesting. 

## A view to the real world

Running Regressions focuses on some topical, real-world issues. Econometric analyses may not seem to be the focus of articles in The Economist, the front page of the Financial Times, New York Times or in OXFAM’s latest newsletter. But the professional application of econometric techniques underlies the insights expressed in the business press. Applied econometrics can earn you a living and win you arguments; it gives empirical ‘flesh’ to what might otherwise be dismissed as subjective opinion or abstract theory. Econometric analysis is used by policy-makers in deciding how much of the budget to devote to health or education, and/or what the tax rate should be. It is used by central bankers deciding whether to raise or lower interest rates. It is used by non-governmental organisations (NGOs) in illustrating the benefits of debt relief and/or how world trade rules can be designed better to advance the interests of developing countries. And it is used by hedge fund analysts to forecast stock market movements and currency fluctuations. Applied econometrics is relevant to every part of economics, finance and development studies and the topics selected for analysis in Running Regressions are chosen accordingly; for example, we have including chapters on international relations (world poverty and armed conflict), local and personal issues (housing, divorce) and cutting-edge fields such as behavioural economics. 

## Use it simply

The book is not about excessively complex econometric techniques. Our present goal is to explain economic phenomenon using elementary econometric techniques of the ‘plain vanilla’ variety – one at a time to highlight the key aspects. Good econometricians will focus on parsimony: they will attempt to abstract from the complexity to strip theoretical models to their bare essentials. In selecting techniques, the best techniques will be the most straightforward and intuitive as long as these techniques are also relatively reliable and accurate. Adopting a relatively simple approach does not reduce the power of the analysis. Simplicity is often very effective. So the aim of Running Regressions is to present analyses in which there is clear connection between the phenomenon observed, the underlying theory, the raw data and the econometric techniques. 

## Use it with versatility: econometrics for the social sciences

The econometric tools outlined in Running Regressions can be used to analyse a wide range of issues from economics, finance, business studies and the other social sciences. Social scientists examine complex aspects of human decisionmaking and so the methods of pure science cannot be adopted without adaptation. Good applied econometrics requires a judicious mix of sound economic theory, reliable data and correctly applied statistical techniques. These ingredients do not always readily combine. Finding the data with which to examine theory is usually the hardest part, in practical terms. Social scientists do not deal with a purely physical world and we rarely have laboratories in which we can run controlled, replicable experiments to generate reliable data sets. We may not have data that is directly related to the phenomenon we want to study. It is so often as if we had started off with the plan to make duck à l’orange for dinner, only to discover that there is no duck and we must substitute chicken; that we have only lemon rind when orange is called for; parsley in place offines herbes and so on. This does not mean that the analysis is going to be a flop – indeed, if we select our techniques carefully we will come up with useful insights as long as we realise that we may be able only roughly to approximate the reality we want to understand. 

It follows from this that applied econometrics involves some subjective judgements. Which elements of the real world should we include and highlight? Which should we subdue or leave out entirely? This decision will be influenced by preference and perception. Just as Monet’s representation of exactly the same tree would be different from, say, Vincent van Gogh’s, so two econometricians can differ in their representation of social science. Different features of reality can be emphasised or downplayed according to the perspective that seems most relevant, topical or exciting – or which best fits a view of the world. It is this aspect ofdiscretion and personal choice that contributes to making econometrics as much an art as it is a science. It is useful to remember, when carrying out one’s own analysis or interpreting the work of others, that there are many different ways of approaching the same question. 

## Use it frequently

We toyed with the idea of calling this book An Econometrician’s Toolbox because the methods presented in this book are used regularly by social scientists using applied econometric techniques. Whether one works in business (estimating the demand curve for airline ticket sales), in development (estimating the effectiveness of various policies on poverty reduction), in law (fighting a monopoly pricing suit, or trying to prove unfair business practices) … the applications are as infinite as the questions that social scientists set out to answer. Of course it is rare that one would run regressions every single day of the week, but the point remains that researchers are required most days to give empirical evidence to back up their arguments and to persuade colleagues as well as critics. Not least, applied econometrics is about providing empirical examples that support (or refute) hypotheses, illustrate trends and allow us to draw inferences about relationships between phenomena. Even if working life consists more of reading the results of studies conducted by others, we must nonetheless understand the implications ofwhat went into the models (and what was left out) and be able to judge whether or not the conclusions are robust. Why was one theory chosen over another? Why those variables selected and not others? Does the data used adequately represent the problem at hand? Has the appropriate yardstick been chosen to assess statistical significance? We need to understand the mechanics and implications of all these elements. 

## Use it as a complement to other texts, or by itself

The advantage of Running Regressions is that it blends a practical approach with a holistic perspective. So Running Regressions is an ideal complement to mainstream econometrics texts because it illustrates a wide range of commonly taught techniques using topical and thought-provoking examples soundly based in elementary economic theory. Alternatively, it does cover all the basic econometric techniques and so it could be used as the main text for introductory applied econometrics and/or research methods courses. 

## The structure of Running Regressions and its chapters

You can read Running Regressions from start-to-finish, or take the à la carte approach, selecting each chapter from the menu of contents, according to particular need or interest. Running Regressions is unusual in that it incorporates two titles for each chapter: a main title referring to an econometric technique and a sub-title referring to an economic issue or theory. This division of the titles reflects Running Regressions’ marriage of theory and applied econometrics. Both titles are listed in the table of contents. So if you are selecting on a chapter-by-chapter basis, you need to decide whether to select either from the list of econometric techniques or from the list of theoretical concepts. This might depend on whether your goal is to prepare for project work/class assignments, to refresh your understanding of a particular theory, to find out more about a particular data issue or to learn about an econometric technique via an interesting illustration of how it works. This unconventional combination of the disparate elements of econometrics into a cohesive whole was one of the book’s primary goals, based on the numerous requests from students for a ‘roadmap’ of econometrics. 

If your aim is to read a general overview of econometrics, we recommend starting at the beginning and working your way through. The book opens with fundamental principles of econometrics and concludes with more complex examples. (The last few chapters, for example would not usually be covered in first-year undergraduate courses.) Running Regressions covers a variety of methods – starting at the most basic (running a regression by hand using a hand-held calculator), moving through the statistical tools available via Excel and then focussing on a widely used tailor-made econometrics package – EViews. In early chapters, data sets are available to allow our readers to try the techniques themselves; in later chapters website links are provided. If you use our data then there may be slight variations in the estimates you get – reflecting rounding differences or specific features of the various programmes but your results should be much the same as the ones we got ourselves. 

If you are reading Running Regressions for guidance about how to do a research report or project in an area covered by this book then follow the ‘Table of Contents’ for guidance about the relevant theories and models. Core theories and their contenders are described, along with a reading list for further and more specialised reading. 

## How to get started

Each of the chapters in Running Regressions goes through a systematic series of steps to show how data and econometric analysis can be used to test a theory. So each chapter is roughly set out in the format that is conventionally expected in applied economic analysis: a theoretical model is developed, the data is presented and analysed and models are estimated and assessed. (Alternatively, one could say that each chapter introduces a different theoretical issue, and then uses an econometric analysis to illustrate it.) For each chapter, the argument will be built up as follows: 

## 1. The issue

In this preliminary section, the basic theoretical ideas, data and econometric approaches are briefly introduced. 

## 2. The theory

We set out the underlying theory or hypothesis, on the basis of existing literature. We then analyse the theory using econometrics but modifying the theory ifthe econometric evidence suggests that the real world does not conform to the theory. We express this theory as an econometric model. This means simplifying the hypothesis into a simple testable assertion and then re-working it into a form that can be analysed using the available data. 

## 3. Data

Each chapter will go into important details about using data. One can learn a great deal simply by evaluating and describing the empirical landscape that a dataset presents. Descriptive analysis is an oft under-estimated, critical step in the whole exercise. So data plots should be examined carefully: chart variables over time and against each other. Look for obvious trends and patterns. 

## 4. Empirical results and interpretation

The next step is to obtain numerical values, or estimates, of the relationships between the variables in the model, from the data available. In this book, we do this through regression analysis, usually using Ordinary Least Squares (OLS), as explained in Chapter 1. In explaining the detail of OLS techniques, we have kept things simple by concentrating on one set of econometric issues per chapter. But in real-world analysis, it is important to remember that we will usually have more than one step in our estimation procedure and so for your own investigations you may have to combine econometric techniques from two or more chapters. Usually a model will need improving. So it is important to consider what could be done to make the model better. Sometimes this means additional work to extend the theoretical model. Sometimes it will involve finding more appropriate or precise data. At other times it may be a matter of using more reliable and accurate econometric techniques. 

It is also important to interpret our results in the light of theoretical issues. Do the findings confirm our theoretical hypotheses or not? What do our econometric results tell us about the relationship between the variables of our model? Are the relationships between variables positive or negative; are the impacts large or small? In order to assess this we test the statistical significance of our estimates using hypothesis tests such as Student’s t-test and/or F tests. What do the tests mean in terms ofthe underlying phenomena studied, and in terms ofour understanding of the theory? Do they allow us to make some forecasts about the future? Of course, just as a defendant in a courtroom can only be declared ‘not guilty’ rather than ‘innocent’, the results can only provide support (or not) to a hypothesis. We can never ‘prove’ a hypothesis. This is why econometricians are cautious with their language, sometimes the statistical linguistic style is necessarily unwieldy: hypotheses are not ‘accepted’; at best they are ‘not rejected’. This is because the empirical findings are by their nature probabilistic: unlikely outcomes are always possible and evidence appearing to support a hypothesis may just be a coincidence. 

## 5. Policy implications and conclusions

It is not enough just to present results and state whether or not they confirm a theory. Good applied econometrics provides practical answers and policy guidance. So we need to set out our conclusions clearly but also to think about the policy implications suggested by our results. This may be where advocacy comes in, for example if an NGO wants to support arguments for policy change; or if Treasury or central bank officials see a case for financial reform during a credit crunch; or funds managers see a warning to overhaul their corporate policy on portfolio allocations. 

## 6. Further reading

We have included further reading for readers who would like to follow-up on the intricacies of the issues we explore. We have referred to a range of readings from textbooks, journal articles and policy reports but these references are just a taster of the range of readings available. We have selected the ones that are relatively straightforward, particularly relevant and/or readily accessible. Intentionally, we have kept these further reading lists relatively brief and we haven’t been able to discuss in detail every relevant reference or reading. For further ideas on readings, don’t forget to do further searches using JSTOR, Google and/or Wikipedia, or just by browsing through economics collections in libraries. The Journal of Economic Literature can be a good source of summary articles. Many topical economic and financial issues are the focus of articles and/or surveys in The Economist and so this magazine is also a useful starting point in a quest to understand topical world issues. 

## 7. Chapter exercises

For most chapters, we have provided some exercises for students who would like to explore the data and/or test and techniques in more detail. 

## Going on from here …

Where possible, each chapter gives references to institutions that are associated with the topic examined or to ongoing research programmes. Our goal is to stimulate readers to realise that applied econometrics can be relevant, fun, and an essential beginning in a journey of understanding the economic, financial and social world around us … 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/1ba90dd8d679565798f2b1859e7b4600eabda52fcff86794be579b5154e14efc.jpg)


# Simple regression and data analysis

In this part we outline some basic econometric techniques, including running regressions by hand using Ordinary Least Squares (OLS) estimation techniques. We focus on simple regressions, i.e. regressions on models with just one explanatory variable. 

We also introduce Microsoft’s Excel as a user-friendly spreadsheet package for running simple regressions. 

Running regressions on models with more than one explanatory variable – Multiple Regression Analysis (MRA), will be analysed from Part II onwards. 

# An introduction to Ordinary Least Squares

This chapter provides a brief and intuitive summary of the econometric theory that underlies OLS estimation, including: 

 The data generating process and sample regression functions 

 Types of data 

 Ordinary Least Squares (OLS) estimation 

 Measuring correlation and goodness of fit 

 The Gauss–Markov theorem 

 Properties of estimators 

 Hypothesis testing 

## 1.1 Introduction

Running Regressions is about the quantitative analysis ofobserved behaviours and phenomena using economic theory, probability and statistics. By bringing these different elements together we can improve our understanding of people, firms and countries – in the past, the present and the future. For those readers who approach the subject with trepidation, it may be worth remembering this practical goal. 

The skills that are required are not intrinsically difficult if a systematic approach is followed. Not least, our intention in Running Regressions is to illustrate commonly used techniques in an imaginative and interesting way. This chapter provides a brief introduction to concepts and techniques that are then worked through as practical examples in the following chapters. 

Finally, whilst we focus on economics, finance and development studies in our selection of topics, the approach can be used in analysing a wide range of all real-world situations. The techniques can be, and are, used in all the social and natural sciences. 

## 1.2 Models and data

The aim ofeconometric analysis is to understand the data generating processes (DGPs) that underlie economic systems and human behaviour. These DGPs are like the engines in a car and they propel socio-economic actions and events. For example, the interaction between income and consumption is determined by a DGP. This DGP causes consumption and income to rise together and these rises will be transmitted into the recorded data on income and consumption. Unfortunately, an econometrician rarely has direct knowledge of DGPs and so he/she has to draw inferences about it from samples of data. For a briefanalysis of the types of data used in econometric analyses, see Box 1.1. 

To capture how DGPs operate an econometrician will use socio-economic and/or financial theory as an initial guide, building up a testable model from previous knowledge about a process or system. Once a testable empirical model has been devised, the econometrician will proceed to estimate the parameters of their model. As explained below, estimating parameters is one of the aims in applied econometrics because the parameters ofa model capture the magnitude and direction ofinteractions between the variables ofthe model. Another aim is to use econometric evidence for forecasting the future and parameter estimates are used in constructing these forecasts. Either way, estimating parameters accurately and reliably is the essence of an applied econometrician’s task. 

## 1.3 Constructing empirical models

Theoretical ideas are translated into empirical hypotheses via some assumptions about the DGP. The DGP is expressed as a mathematical function linking a dependent variable – the variable that the econometrician is trying to ‘explain’ (sometimes called the regressand); and the explanatory variables (sometimes called regressors or independent variables). For a lot of econometrics, the selection of a variable as the independent variable is complicated by the fact that causality may not be unidirectional, e.g. for the example used in this chapter: poverty might cause low growth; low growth might cause poverty; they may both affect each other (i.e. there may be a simultaneous relationship between them) and/or a third factor may be generating changes in both. 

## Box 1.1 Types of data

When gathering data we should try to ensure that our data sample is representative of the data generating process (DGP). We do not gather data on average height by measuring only world-class basketball players and we do not conduct household surveys at times of the day when people in formal employment are out and so those at home are a biased subset of the total. 

## Data dimensions

Three types of datasets are used in this book: time series; cross-sectional and pooled/panel datasets. 

Time-series data are data collected over the temporal dimension to capture the evolution of variables over time. For example, we might be tracking national GDP trends, analysing one country’s performance over time. Time-series data can be collected at any sort of frequency, e.g. monthly, quarterly, weekly, daily or more frequently; for example, high-frequency data (available at intervals as short as every minute or every second) is sometimes useful in the analysis of financial markets. 

Cross-sectionaldata are collected over the spatial dimension and they provide a snapshot of a cross-sectional pattern at one point in time. Cross-sectional data can be captured at many levels of disaggregation. For example, the Population Census in the UK surveys a sample of households at one point in time. In microeconometric analyses household or employer/worker survey data is used; in macroeconometric analyses, international, national and regional data is used. 

Pooledandpaneldata sets combine cross-sectional and time-series data, for example by gathering data on the same sample of families, firms or countries, every year over a number of years. Special techniques may be needed in analysing these types of data, as is explained in Chapter 11. 

## The nature of data

Broadly speaking, the nature of data collected can be categorised according to how the phenomena under investigation are measured. 

Quantitative data capture things that are measurable using an objective, cardinal scale. Cardinal measurement involves calculating ‘how many’ and requires clear units of measurement. For example, to measure unemployment we count how many people are without a job; to measure GDP we count how many currency units of output have been produced. Other quantitative data are calculated using indices based around units of measurement, for example price indices are calculated from prices of goods measured in currency units. 

Qualitative data cannot be counted. There are no objective units of measurement for qualitative data and so assigning these data numbers must necessarily embed some sort of subjective judgement. This subjective judgement will emerge either in the method of measurement or in the system of weighting different components of a phenomena. For example the United Nations Development Programme (UNDP) Human Development Indicator (HDI) is calculated using infant mortality rates, GDP per capita and literacy rates. Each of these components is captured using different units of measurement and to sum them together is like counting apples and eggs. In practice, the HDI index is constructed giving indices of these components an equal weighting; but even the decision to assign different components equal weights is in essence a subjective judgement. Why should literacy be as important as infant mortality? Why should GDP per capita be as important as literacy? For business confidence surveys, respondents are asked to give subjective scores using an ordinal system of measurement, i.e. they are asked to rank alternatives according to their subjective assessments and individual preferences. 

We have divided quantitative and qualitative data starkly but it is important to remember that there is fuzziness at the boundary between them. For example, defining and measuring variables such as prices, unemployment and GDP is rarely completely straightforward; information uncertainty (the uncertainty associated with data constraints and measurement problems) and potential for measurement error should always be acknowledged in empirical analysis. Also, in many areas of social sciences, e.g. psychology and behavioural economics, data are collected based on observed behaviour, often in a binary form as dummy variables (e.g. D= 1 if the experimental subject did perform a specific action; D= 0 if they didn’t). So it is possible to count the number of people performing an action even though the data is reflecting a subjective decision-making process. 

In practice, many studies will use both quantitative and qualitative data. In Britain for example, the UK’s Monetary Policy Committee (MPC-UK) sets central bank interest rates to moderate inflationary pressures using a variety of indicators. Given the uncertainties surrounding accurate measurement and forecasting of the variables affecting inflation etc. these procedures cannot be mechanical; the final decision of the MPC will, inevitably, have qualitative/subjective elements. Nonetheless statistical information will be very useful to the members of the MPC-UK in forming their judgements. 

In devising a model, it is important to remember that econometrics is about using, testing and developing economic theories. It is not about the mindless churning of data. For research to be useful as well as interesting, socio-economic and financial theories should always be the starting point. 

In this discussion we are confining our discussion to linear models.<sup>1</sup> In a linear world the dependent variable is a linear (i.e. additive) function of explanatory variables and can be represented as a simple linear equation. For example, if an econometrician hypothesises that a linear relationship exists between poverty and GDP growth per capita then he/she will formulate the following: 

$$
Y _ {i} = \alpha + \beta X _ {i} + \varepsilon_ {i}\tag{1.1}
$$

where $Y _ { i }$ represents the average change in the poverty rate in the ith country and $X _ { i }$ represents the growth in GDP per capita in the ith country. 

There are two main components to this model: a deterministic component and a random or ‘stochastic’ component. 

The deterministic component is represented by $\alpha + \beta X _ { i }$ , which is an amalgam of parameters (α and $\beta \mathrm { s } )$ and explanatory variables. We hypothesise that these parameters represent properties inherent to a ‘population’ of data. But what is $\alpha ?$ What is $\beta \ ?$ The parameters α and $\beta$ are the unknowns of the system and the essence of the applied econometrician’s task is to identify them. A good econometrician is looking for reliable and accurate information about the magnitude and sign of these parameters. 

The stochastic component is represented by ε, which is commonly called the error term or disturbance term. The error term captures all the excluded (and by assumption unimportant) influences on the dependent variable. It also captures the inherent randomness within the DGP. The existence of this randomness means that there will always be a probabilistic element within econometric analysis. The world ofstatistics and econometrics is a world ofprobability and chance; anything can happen. So the econometrician must (usually) concentrate on what is most likely to be true rather than what is exactly true. 

## 1.4 The sample regression function (SRF)

Econometricians cannot usually see the DGP (unless they artificially create one for themselves using Monte Carlo experiments) and so they have to make inferences about the population from a sample of data. The model estimated using sample data is sometimes referred to as the sample regression function (SRF). This is because even if an econometrician knows what population they should be using to get their data sample (in a cross-sectional context for example, it might be the population of the US) it will be infeasible and/or too costly for them to collect and analyse information on all US citizens. It is even more complicated in a time series context where it is not intuitively clear what the population of data actually is. All the data used in Running 

Regressions is sample data; we don’t have observations for every member of the population under investigation. But because we’re not using whole populations we rarely know the true values of the parameters α and $\beta .$ We have to make educated guesses and for this to work well we have to select our sample carefully to ensure that it is representative and to avoid sample selection bias. A biased sample will not be representative of a population; for example an internet survey of favourite foods/drinks conducted via facebook will give a sample of data biased in favour of younger age groups and/or those who are relatively technically literate; this sample would not be representative of people of all age groups, 

For the poverty example above, we could collect a sample of cross-sectional data on Y and X for i different countries. Then we would construct the following SRF: 

$$
Y _ {i} = \hat {\alpha} + \hat {\beta} X _ {i} + \hat {\varepsilon} _ {i}\tag{1.2}
$$

You will notice that this SRF looks very similar to (1.1) except $\hat { \alpha }$ and $\hat { \beta }$ are the sample estimates of α and $\beta$ not the population values. The term $\hat { \varepsilon } _ { i }$ is the sample residual, which is the estimate ofthe error term. As is explained below, we assume that the expected value or mean ofthis error is zero, i.e. we assume that $E ( \varepsilon _ { i } ) = 0$ 

Using an example that is explained more fully in Chapter 2, our working hypothesis is that changes in poverty vary as growth rates vary. To assess this hypothesis we derive estimates of changes in poverty for a given growth rate, i.e. our expected value of $Y _ { i }$ conditional upon a given $X _ { i } - E ( Y _ { i } | X _ { i } )$ , using parameter estimates and observations on Y and X as follows: 

$$
\hat {Y} _ {i} = \hat {\alpha} + \hat {\beta} X _ {i}\tag{1.3}
$$

where ${ \hat { Y } } _ { i }$ is an estimate of Y given X. The estimate of Y may also be referred to as the predicted value or fitted value of Y. 

Linking these ideas into our example from above, if $\hat { \beta }$ is negative and ‘significantly’ different from zero (i.e. relatively large) then it may suggest that countries with higher growth rates have reduced poverty more rapidly than countries with lower growth rates. So if we want a more equitable world, then one policy possibility is to encourage GDP growth. 

But in order to make these inferences, we need some accurate and reliable information about the parameter estimates α^ and ${ \hat { \boldsymbol { \beta } } } .$ How can we get this information? A simple and (often) reliable method is Ordinary Least Squares (OLS). 

## 1.5 Ordinary Least Squares (OLS)

In the previous section we explained that estimates of the parameters describing a DGP are derived from sample data and that these parameter estimates can be used to derive an estimate of dependent variable conditional upon each value of an explanatory variable. But how do we calculate parameter estimates? There are a large number of different estimation techniques, many of which can give reliable answers. But in this book we are concentrating on the simplest of them – Ordinary Least Squares (OLS). 

OLS involves estimating the line of best fit or regression line through the observations on Y and X. For our example of poverty and GDP growth, Figure 1.1 depicts the line of best fit. With GDP growth on the horizontal axis and average change in poverty on the vertical axis, the pairs ofobservations on Y and X for each country are represented as dots. The line that fits these observed values best will pass through the means for both the dependent and the explanatory variable and it will minimise the spread of observations around the line. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/430104c4543253809520295a6d2a4b8a6c18d162db8c176bf16b67fba46fad1b.jpg)



Figure 1.1 Line of best fit


What do we mean by minimising the spread of observations? For OLS, we are minimising the spread of sample residuals (^ε ), where the residuals are the vertical distances between the observed value and the predicted value: 

$$
\hat {\varepsilon} _ {i} = Y _ {i} - \hat {Y} _ {i} = Y _ {i} - \hat {\alpha} - \hat {\beta} X _ {i}\tag{1.4}
$$

Spread is captured statistically as squared deviations from means and, because the mean of residuals is zero, the residual spread is measured as the sum of squared residuals (RSS). 

In practice, OLS involves using differential calculus to identify the parameter estimates that minimise this sum of squared residuals: 

$$
R S S = \sum_ {i = 1} ^ {n} \hat {\varepsilon} _ {i} ^ {2} = \sum \left(Y _ {i} - \hat {Y} _ {i}\right) ^ {2}\tag{1.5}
$$

When we minimise RSS, we get the normal equations and solve to give the following formulae for the parameter estimates: 

$$
\hat {\beta} = \frac {\operatorname{cov} (X , Y)}{\operatorname{var} (X)} = \frac {\sum \left(X _ {i} - \bar {X}\right) \left(Y _ {i} - \bar {Y}\right)}{\sum \left(X _ {i} - \bar {X}\right) ^ {2}}\tag{1.6}
$$

$$
\hat {\alpha} = \bar {Y} - \hat {\beta} \bar {X}\tag{1.7}
$$

where cov(X, Y) is the covariance between our explanatory variable, and X<sup>-</sup> and Y<sup>-</sup> are the sample means for the variables X and Y respectively. 

Covariance captures the extent to which two variables ‘co-vary’. To explain covariance: it is measured using the products ofdeviations from means; iftwo variables (in this case X and Y) are deviating from their means in a similar way, then the covariance between them will be large in absolute terms. So if we have a large covariance then (all things being equal) this will generate a $\beta$ that is large in absolute terms – we will be picking up a strong association between the variables. In the denominator of (1.6) we have var(X) – the variance of X. The variance of a variable is measured by summing the squared deviations of a variable from its mean, giving a measure of spread or dispersion. If a variable has a tendency to deviate widely from its mean, then the variance will be large. 

Measures of variance and spread are also important in assessing the accuracy of our estimation procedure. Minimising the RSS in OLS is equivalent to minimising the residual variance. (The definitions and formulae for residual variance and the variances of our parameter estimates are explained in Box 1.2.) With OLS, the expected value (i.e. the mean) of residuals will be 

## Box 1.2 Calculating variances and standard errors

As explained above, OLS involves minimising the spread of observations around the line of best fit. For OLS, we are minimising this spread by minimising RSS so we will also be minimising the residual variance, defined as: 

$$
\hat {\sigma} _ {i} ^ {2} = \frac {1}{n - k - 1} \sum_ {i} ^ {n} \hat {\varepsilon} _ {i} ^ {2} = \frac {R S S}{n - k - 1}\tag{1.8}
$$

where k is the number of explanatory variables in our model (in this chapter’s example, we have one explanatory variable and so we would have $\boldsymbol { \eta } - \boldsymbol { 2 }$ in our denominator). 

We can use this information to calculate the variances and standard errors of each parameter estimate as follows: 

$$
\operatorname{var} (\hat {\beta}) = \frac {\sigma^ {2}}{\sum (X _ {i} - \bar {X}) ^ {2}}
$$

$$
s e (\hat {\beta}) = \sqrt {\frac {\hat {\sigma} ^ {2}}{\sum (X _ {i} - \bar {X}) ^ {2}}}\tag{1.9}
$$

where $s e \left( { \hat { \beta } } \right)$ is the standard error of ${ \hat { \beta } } .$ 

Similarly the variance and standard error of the intercept parameter are: 

$$
\operatorname{var} (\hat {a}) = \left\{\frac {\sum X _ {i} ^ {2}}{n \sum (X _ {i} - \bar {X}) ^ {2}} \right\} \times \sigma^ {2}\tag{1.10}
$$

$$
s e (\hat {a}) = \sqrt {\left\{\frac {\sum X _ {i} ^ {2}}{n \sum (X _ {i} - \bar {X}) ^ {2}} \times \hat {\sigma} ^ {2} \right.}
$$

Note that in the above formulae for the variances of the parameter estimates ^α and ${ \hat { \beta } } ,$ the true error variance $( \sigma ^ { 2 } )$ is used; in the real world, however, we will not know this true error variance and so in calculating the standard errors for our parameter estimates we must use the sample estimate of the error variance i.e. the residual variance $\hat { \sigma } ^ { 2 }$ . Also, it is important to note that these variances and standard errors are calculated assuming homoscedasticity, i.e. that the error variance is constant across all observations. If this assumption is violated, i.e. if there is heteroscedasticity, then heteroscedasticity robust variances and standard errors should be used. The homoscedasticity assumption is explained below and the heteroscedasticity problem is explored in detail in Chapter 6. 

zero, i.e. $E ( \varepsilon _ { i } | X _ { i } ) = 0$ but the spread of the residuals (the residual variance) may still be large. A model with a relatively large residual variance will not fit the observed data very well and our next step will be to assess how well our estimated model is fitting the observed data. 

## Goodness of fit and the coefficient of determination

## The correlation coefficient

Econometric analysis often starts with an investigation of correlation, which is the degree of linear association between two variables; OLS estimation is essentially a sophisticated form of correlation analysis. In assessing the results from an OLS regression we will need an objective measure of the nature of clustering in a scatter plot of Y against X; this is captured in its simplest form by the correlation coefficient which captures the relative magnitude of the linear association between two variables and thus is a simple measure of statistical ‘dependence’. 

The first step in calculating the correlation coefficient involves measuring the extent to which the two series co-vary using covariance (as explained above). The extent to which one variable covaries with another gives a usefu clue about correlation because if variables are correlated then the covariance between them will be relatively large in comparison with the variances. The correlation coefficient is calculated from the covariances and variances as follows: 

$$
r _ {X Y} = \frac {\sum (X _ {i} - \bar {X}) (Y _ {i} - \bar {Y})}{\sqrt {\sum (X _ {i} - \bar {X}) ^ {2} \sum (Y _ {i} - \bar {Y}) ^ {2}}} = \frac {\operatorname{cov} (X , Y)}{\sqrt {\operatorname{var} (X) \times \operatorname{var} (Y)}}\tag{1.11}
$$

where $r _ { X Y }$ is the correlation coefficient between X and Y. 

This correlation coefficient is a ‘normalised’ covariance: the association between deviations from means for Y and X is normalised to lie between ± 1. A correlation coefficient of + 1 implies that the variables are moving together completely. A correlation coefficient of –1 implies that they are mirroring each other (i.e. moving in opposite directions but completely in tandem). A correlation coefficient of 0 implies that there is no systematic (linear) association between the variables. 

Note that in calculating the correlation coefficient, no distinction is made between a dependent and an explanatory variable. This is because the correlation coefficient is just a measure of linear association. It tells us nothing about which variable causes the other; in fact, some third variable might be causing both. It is very important to remember that a statistical correlation does not necessarily imply an underlying causal mechanism. 

## Goodness of fit

As explained above, Figure 1.1 presents a visual impression of how well our estimated line fits the observations. But we can capture how neatly our estimated line for Y fits the spread of observed values on Y more precisely by measuring the goodness of fit. The goodness of fit captures the extent to which our line of best fit neatly fits the pairs of observations on Y and X. This can be measured by calculating the ratio of ‘explained’ variance to unexplained variance as follows: 

1. For each observation we calculate the difference between the estimate of Y (calculated using Equation (1.3)) and the sample mean ${ \bar { Y } } .$ . We sum these deviations together across all our observations to give the explained sum of squares (ESS). 

2. Similarly, we calculate the sum of deviations of each observed value of Y from the sample mean Y<sup>-</sup>. This is the total sum of squares (TSS). 

3. We take the ratio of the ESS to the TSS. This ratio is $R ^ { 2 } -$ the coefficient of determination: 

$$
R ^ {2} = \frac {E S S}{T S S} = \frac {\sum (\hat {Y} - \bar {Y}) ^ {2}}{\sum (Y _ {i} - \bar {Y}) ^ {2}}\tag{1.12}
$$

The intuition underlying $R ^ { 2 }$ is that it gives a relative measure of the proportion of the total variability in Y that is ‘explained’ by the model, i.e. that is captured by the line of best fit. 

In the two-dimensional world of simple regression analysis (SRA), i.e. for regressions on just one explanatory variable, there is no essential difference between the correlation coefficient (r) and the goodness of fit. In SRA, $R ^ { 2 } = r ^ { 2 }$ ; the coefficient of determination is just the square of the correlation coefficient. But, as explained in Chapter 5, the relationship becomes more complex in multiple regression analysis (MRA). 

## 1.6 The Gauss–Markov Theorem

Now that we’ve explained the mechanics of OLS we need to explain why OLS is so commonly used. OLS is a popular technique because, given some assumptions (as explained below), OLS estimators will reliable and accurate. This justification for the OLS method is captured by the Gauss– Markov Theorem, which states that if the Gauss–Markov assumptions are satisfied then the OLS parameter estimators will be BLUE (Best Linear Unbiased Estimators). BLUEness is associated with reliability and accuracy and the technical definitions of these terms are explained in Box 1.3. 

## Box 1.3 Statistical indicators of reliability

In assessing how well an estimation technique such as OLS is working, performance is judged in terms of the desirable properties of estimators. Desirability reflects the fact that we would like our estimators to be as simple, accurate and reliable as possible. BLUEness is about these desirable properties of estimators. The main desirable small sample properties are unbiasedness (= accuracy), minimum variance (= reliability) and linearity (associated with simplicity). 

Unbiasedness is associated with accuracy. For example, if an estimate of the slope parameter $\beta$ is unbiased, this means that if lots of samples of data are taken and each is used to get an estimate ${ \hat { \beta } } ,$ then the average $\hat { \beta }$ from all the samples will be equal to the true value in the population $\beta .$ In mathematical notation: $\begin{array} { r } { E ( \hat { \boldsymbol { \beta } } ) = \boldsymbol { \beta } , } \end{array}$ , where $E ( { \hat { \beta } } )$ is the expected value (i.e. average) of ${ \hat { \beta } } .$ . The property of unbiasedness is shown visually in Figure 1.2. Each panel of this diagram shows sampling distributions for two estimation procedures A and B, and captures the probability of getting each value of ${ \hat { \beta } } .$ If we were to take repeated samples and estimate the parameter $\beta$ from all these samples of data, then the sample parameter estimate $\hat { \beta }$ will take a range of values because it is a random variable. If our estimator is unbiased then the average of these values will be the correct value. For example, Figure 1.2 shows that the sampling distribution for A is centred around the true value $\beta .$ . Over many samples, on average $\hat { \beta } _ { A }$ is equal to the true value $\beta$ i.e. $\mathinner { E \mathopen { \left( \hat { \beta } _ { A } \right) } } = \beta$ so A is an unbiased estimator of $\beta .$ For estimator $\mathsf { B } ,$ , over many samples the most likely estimate is not centred around the true value $\beta$ so $\textstyle E ( { \hat { \beta } } _ { B } ) \neq \beta$ and $\hat { \beta } _ { B }$ is a biased estimator of $\beta$ 

Minimum variance is associated with reliability. The minimum variance estimator will be the estimator with the smallest variance of its sampling distribution for ${ \hat { \beta } } .$ From Figure 1.3, you can see that both sampling distributions for $\hat { \beta }$ are symmetrically distributed around the true value $\beta$ and both have the same area of $1 . ^ { 2 }$ But the left-hand sampling distribution for $\hat { \beta } _ { A }$ is taller and narrower than that for $\hat { \beta } _ { B }$ showing that the spread of estimates around the true value $\beta$ is smaller for the $\hat { \beta } _ { A }$ sampling distribution than for the ${ \hat { \beta } } _ { B }$ sampling distribution. So A is the minimum variance estimator in this case. 

Linearity is associated with linear (i.e. additive) calculation rather than multiplicative, non-linear calculation. OLS estimators are derived from the linear summing of random variables and this means that OLS estimates can be calculated relatively easily. In some cases, if a model is just non-linear in the variables but linear in the parameters, then OLS techniques can still be used on a transformed model. For example, a production function of form $\begin{array} { r } { Y = A K ^ { \gamma } L ^ { \beta } } \end{array}$ is a non-linear, multiplicative combination of the variables 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/e6701d9215c0bcdb1d2c0a5307cbde08c5257fec02461b6517c8da4e14cbe9ac.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/2a720246702a3fa7c8099b332c9bc42beebee33d17256f8b56c22e1467afa8ea.jpg)



Figure 1.2 Sampling distributions for unbiased estimator A and biased estimator B


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/31f374e68ffd1351b1892ffd5de7be5c4a241397c3194cad5ac3ef0c28370923.jpg)



Figure 1.3 Sampling distributions showing minimum variance estimator $\hat { \beta } _ { A }$


Kand $L ;$ but it can be simplified to a form in which it is an additive function of the logged variables as follows: ln Y ¼ ln A þ γ ln K þ β ln L. OLS can be used to estimate this logged function because this function is linear in the parameters (which in this case are $\gamma , \beta$ and ln $A ) .$ 

This property is important in justifying the use of OLS because OLS is not the only accurate and/or reliable estimation technique; there are many others, for example Maximum Likelihood Estimation $( M L E ) ^ { 3 }$ . Whilst MLE is not always unbiased it is efficient in large samples (i.e. it is ‘asymptotically efficient’ and ‘consistent’, properties that are explained below). But calculating MLE parameter estimates involves complicated non-linear techniques. The linearity property of OLS gives it an advantage over MLE in terms of relative simplicity. With modern econometrics software however this ease of OLS estimation is of less importance than when the churning of numbers necessary to running a regression was a relatively laborious, human-error prone process. 

## Asymptotic properties and the Central Limit Theorem (CLT)

As you will see in the chapters that follow, common violations of the Gauss–Markov assumptions mean that we rarely see a full set of desirable properties in small samples. 

But if an econometrician has a large sample of data with a large number of observations then they may not need to worry if their estimators are not BLUE as long as they have other desirable properties. One of the advantages of large samples is that estimators that do not work well in small samples may possess desirable asymptotic (large sample) properties instead and these asymptotic properties emerge as $n {  } \infty$ . So provided your sample is large enough, then lack of BLUEness does not necessarily create insurmountable problems. 

This is because, for very large samples of data, we can invoke the law of large numbers: when large numbers of variables are averaged, errors will cancel out and estimates are more likely to be unbiased. More specifically, given the Central Limit Theorem (CLT), random variables will approximate the standard normal distribution in large samples. (The standard normal distribution is a probability distribution used widely in statistics; it is a symmetric distribution with a mean of zero and a variance of 1.) 

Most of the asymptotic properties are corollaries of the properties associated with BLUEness, e.g. two important asymptotic properties are asymptotic unbiasedness and asymptotic efficiency. For example, an estimator may be biased in small samples but as the sample size increases, i.e. as $n {  } \infty$ , the bias is eliminated and we can therefore say that the estimator is asymptotically unbiased. One of the most important asymptotic properties is consistency. For a consistent estimator, its sampling distribution shrinks in spread as n increases until ‘at the limit’, i.e. as $n {  } \infty$ , bias and variance go to zero. As illustrated in Figure 1.4, the sampling distribution for the parameter estimate collapses to an infinitely tall vertical line (the variance around a line is zero) at the true value of the population parameter. 

Consistency is an important property in practice because, as explained below, OLS is only BLUE given certain assumptions (i.e. the Gauss Markov assumptions). For some violations of these assumptions BLUEness is lost, but consistency remains. So, as long as our sample size is large enough, OLS will still giving reliable and accurate estimates. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/2d6438e14da2e5c29a6bd8e8233ed700381d07fe53c74da5af2af37122398b1a.jpg)



Figure 1.4 Sampling distributions for a consistent estimator


In claiming on these asymptotic properties we need a large sample of data. But when is our sample big enough for us to start claiming on asymptotic properties? Asking this question is a bit like asking ‘How long is a piece of string?’ For some models very large sample sizes are needed for asymptotic statistics to be a reasonable approximation. It depends on the size of the population of data and a range of other factors, e.g. the complexity of the model. As a minimum, you should generally aim to have sample sizes of 50 observations or so. 

As explained above, OLS will only work well if the Gauss Markov assumptions are satisfied. 

We will focus on some key assumptions including the following: 

1. The mean of the error terms is zero. 

2. No autocorrelation – the covariance between error terms is zero. 

3. Homoscedasticity: the variance of the error is constant across all observations. 

4. The model is correctly specified, including all relevant explanatory variables, no unnecessary ones and represented using the correct functional form. 

5. Exogeneity: the error term and explanatory variables are independently distributed, i.e. are not correlated with each other. 

6. Linearity in the parameters: The model capturing the DGP must be linear in the parameters because OLS is a linear estimation technique. 

Some ofthe Gauss–Markov assumptions can be represented more quickly and easily in mathematical notation, as shown in Box 1.4. 

Different textbooks present Gauss–Markov assumptions (also known as Gaussian assumptions) in different ways. For example, some textbooks also include assumptions such as perfect multicollinearity (no perfect linear association between explanatory variables) and non-zero variance of explanatory variables; violating these assumptions will prevent the mathematical identification of the parameters. We are not focussing on these assumptions here because if a model is properly formulated and based on a sensible interpretation of underlying theories, then these problems will not occur. 

As will be explained in the subsequent chapters, from estimating an SRF we can infer whether or not our hypotheses about the DGP are accurately capturing reality. From looking at the sample parameter estimates, the econometrician can make inferences about the parameters underlying the DGP. But if we want specifically to test whether or not these inferences are accurate, then we have to add in the normality assumption i.e. we have to assume that our error terms are normally distributed. As explained above, in large samples the normality assumption is justified by the CLT and the law oflarge numbers. 

Box 1.4 Gauss–Markov assumptions – mathematical notation
1. The mean or expected value of $\varepsilon_{i}$ , the error term is zero: $E(\varepsilon_{i}) = 0$ .
2. No autocorrelation, i.e. a zero covariance between error term for observation i and the error term for observation j: $\mathbf{cov}(\varepsilon_{i}, \varepsilon_{j}) = 0$ 3. Homoscedasticity, the variance of the error term, i.e. $\text{var}(\varepsilon_{ij})$ , is a constant: $\text{var}(\varepsilon_{i}) = \sigma^{2}$ , where $\sigma^{2}$ is a constant.
4. Exogeneity: $\mathbf{cov}(\varepsilon_{i}, X_{i}) = 0$ where X is the explanatory variable. 

It is important to remember that the Gauss–Markov assumptions are neither independent nor mutually exclusive and just because one assumption is violated does not mean that another assumption can’t be violated too. In fact, sometimes the violations of groups of assumptions can give a clue as to what might be wrong with a model – for example any sort of systematic pattern in residuals may be a sign that the model econometric is misspecified. 

The problem for OLS estimation is that whilst it is a simple technique, its underlying assumptions are often violated. So the popularity of OLS as an estimation technique is not always justified. In order to establish whether or not OLS is working, diagnostic tests must be used to test the Gauss–Markov (GM) assumptions. Ifthese tests are failed, then the techniques can sometimes be adapted to resolve the problem. Alternatively, other estimation techniques may be needed. 

In some of the subsequent chapters of this book, we examine the key GM assumptions and illustrate some of the diagnostic tests used to test whether or not these GM assumptions are satisfied. We explain the consequences of violating these Gauss Markov assumptions and we outline some of the corrective procedures designed to allow the econometrician to return to a BLUE(ish) world. 

## 1.7 Drawing inferences and hypothesis tests

What is the difference between our parameter estimates $\hat { \alpha }$ and $\hat { \beta }$ and the underlying ‘true’ values of α and $\beta \mathfrak { Q }$ If we want specifically to test whether or not these inferences are accurate, we will use hypothesis tests: hypothesis tests are a way to draw statistical inferences from our results. Of course we do not know the true value for the coefficients because we have a random sample and there is always a probability that our random sample is not at all representative of the DGP and/or population as a whole. Unless we have created our own dataset we will never know whether or not our parameter estimates match the true values. But, using a statistical/probability distribution as a benchmark, we can investigate the statistical significance of the difference between our parameter estimates and a null hypothesis about the true value(s). 

## Hypothesis tests: General principles

The first step in hypothesis testing is to set-up the null hypothesis $\left( H _ { 0 } \right)$ and alternative hypothesis $\left( H _ { 1 } \right)$ . Null hypotheses are usually constructed around a ‘conventional wisdom’ representing the consensus of opinion on an issue. As will be seen below, this ensures that the null is relatively difficult to reject. In principle at least, we should be prepared to reject the null (and disregard existing information and/or judgements about a phenomenon) only ifwe have results that are extremely different from our null. 

The next step is to use our sample data to construct a test statistic. Test statistics are constructed around estimates from a sample of data. Remembering that sample estimates are random variables, test statistics will also be random variables following some statistical distribution. The test statistics used in this book (i.e. the t and F tests) are relatively simple and widely known; statisticians have established that they will fall within wellknown probability distributions, i.e. the t and F distributions (variants of the standard normal distribution). Essentially we investigate whether or not our test statistics fall in the tails of these distributions; if they do, then we will infer that our null is relatively unlikely and we reject it. If our test statistic falls in the middle of the relevant distribution then we ‘do not reject’ the null. This rather unwieldy and pedantic language reflects the fact that, for statistical analysis, we are in a world of induction (not deduction) and so we can never ‘prove’ anything. Statisticians/econometricians are cautious people. They are very aware of the distinction between extremely unlikely and impossible. Statisticians do not ‘accept’ anything; they prefer to say that they ‘do not reject’ it. 

In deciding whether or not to reject a null hypothesis, we use a decision rule. We will discuss decision rules based around critical values and decision rules based around probability values $( p$ values). 

The critical value of a test statistic marks the boundary between rejection and non-rejection of our null and, using significance levels and degrees of freedom, we can find critical values in the statistical tables for t and F distributions. 

But what do we mean by a significance level? Significance levels determine critical values and thus what we do with our null hypothesis. For example, if a critical value of a test statistic is selected using a 5% significance level, this means that we would expect to see a test statistic more extreme than the critical value in only 5% of samples. We go on to infer that it is unlikely that we would see such extreme values if our null were true and so we reject our null. This doesn’t mean that our null is wrong; it just means that it doesn’t seem very probable given the results from our sample of data. 

It is important to remember that the selection of the significance level does introduce some arbitrariness into hypothesis testing. Also, selection of significance levels will affect the chances of making a Type I error (the error of incorrectly rejecting a true $\mathrm { H } _ { 0 } )$ versus a Type II error (the error of not rejecting a false null). For most econometric analysis we won’t know whether or not we are making these mistakes because the whole point is that we don’t know what’s true. If we did then perhaps we wouldn’t have to bother with running regressions! Significance levels will directly determine the probability of Type I error, i.e. a significance level of 5% implies that the probability of a Type I error is 5%. Significance levels will also affect the power of hypothesis tests (the power ofa test is 1 minus the probability ofType II error). The tradeoffs between Type I and Type II errors raise a whole range ofinteresting issues beyond the scope of this text but addressed in detail in any good text on statistical theory. We abstract from these complexities by using conventional significance levels, i.e. 1%, 5% and 10%. 

The critical values for the t and F tests used in this book will also be determined by the degrees of freedom in our model. Degrees of freedom give us statistical ‘room for manoeuvre’; if we have many degrees of freedom then we can more accurately estimate the parameters of an empirical model. In running a regression, we lose one degree of freedom for each parameter estimated. In SRA we will lose one degree of freedom (df) in estimating the slope and another in estimating the intercept. This gives $d f = n - k - l = n - 2 .$ In multiple regression, more parameters must be estimated and so more degrees of freedom will be lost in calculating these parameters, e.g. the degrees of freedom in a model with $k = 5 ;$ , i.e. with five explanatory variables is $d f = n - 5 - 1 = n - 6 .$ 

An alternative to using critical values is to use p values (probability values). These give an exact significance level, i.e. the significance level at which we would reject our null. So a relatively low $\boldsymbol { p }$ value would suggest that we should reject our null and a relatively high $\boldsymbol { p }$ value would suggest that we should retain it. If we are using a 5% significance level, then our $\boldsymbol { p }$ value decision rule would be: 

If $\textstyle p > 0 . 0 5$ (i.e. 5%), then do not reject $H _ { 0 } ;$ if $\hbar < 0 . 0 5$ then reject $H _ { 0 }$ . 

These $\boldsymbol { p }$ values can be used for any sort of hypothesis test, including t tests, F tests (and other hypothesis tests) and are now widely reported in most statistical and econometrics packages (including Excel and EViews). Using $\boldsymbol { p }$ values saves the time and trouble involved in looking up statistical tables. 

## Tests of individual significance – Student’s t test

For our tests of the individual significance of specific parameter estimates, we use Student’s t test. The $H _ { 0 }$ and $H _ { 1 }$ for the t tests can be constructed in two ways depending on whether we are using a one-tailed test or a two-tailed test. With one-tailed tests we construct an asymmetric $H _ { 1 }$ implying that the parameter of interest will deviate from the null in one direction only. We use a one-tailed test when we have some prior information about the sign of our parameters. One-tailed tests are more powerful because the rejection region is concentrated in one tail of the t distribution. One-tailed t tests are illustrated in Chapter 3. 

For two-tailed tests, the $H _ { 1 }$ is constructed to allow deviations from the null in either direction. To illustrate the procedures for a two-tailed t test on a slope parameter of our model in Equation (1.1), our null and alternatives would be 

$$
\begin{array}{l} H _ {0}: \beta = 0 \\ H _ {1}: \beta \neq 0 \end{array}
$$

The test statistic for the Student’s t test is: 

$$
\hat {t} = \frac {\hat {\beta} - \beta_ {H _ {0}}}{s e (\hat {\beta})}\tag{1.13}
$$

where $\beta _ { H _ { 0 } }$ is the value of $\dot { \boldsymbol { \beta } }$ hypothesized within our null, $\hat { \beta }$ is our estimate of $\beta$ and $s e ( \hat { \beta } )$ is the standard error of our estimate of $\beta .$ . 

Our decision rule will be to reject $H _ { 0 }$ if the absolute value of the t statistic is ‘significantly greater’ than 0 with a 5% significance level and constructing this decision rule around critical values gives: 

$I f - t _ { \mathrm { c r i t } } < \hat { t } < + t _ { \mathrm { c r i t } }$ then do not reject $H _ { 0 }$ ; but $i f | \hat { t } | < t _ { \mathrm { c r i t } }$ ; then reject $H _ { 0 }$ where $t _ { \mathrm { c r i t } }$ is the critical value of our test statistic. 

A rejection of $H _ { 0 }$ implies that the slope parameter is significantly different from zero and therefore suggests a systematic association between Y and X. 

## Confidence intervals

We can turn the t testing procedure on its head to give an alternative way of drawing inferences about our $H _ { 0 }$ by constructing a confidence interval (CI). CIs give the numerical region in which we would have some degree of confidence that our null is true, i.e. they capture the region in which our null would not be rejected. The formula for the confidence interval is given by: 

$$
\left| \hat {\beta} \right| \pm s e (\hat {\beta}) \times t _ {\text { crit }}\tag{1.14}
$$

<sub>If</sub> $H _ { 0 }$ falls within the CI then we would not reject $H _ { 0 }$ but if $H _ { 0 }$ falls outside the CI we would conclude that it is relatively unlikely and so would reject $H _ { 0 }$ . An example of the construction of confidence intervals is illustrated in Chapter 2. 

## Tests of joint significance – The F test of explanatory power

For simple regression analysis (SRA) we are interested in testing hypotheses about a single slope parameter. In MRA we have more than one explanatory variable and so we will need to use joint tests of significance if we want to draw inferences about parameters on groups of variables. For example if we want to establish whether or not all the explanatory variables in our model are statistically associated with our dependent variable, then we can test whether or not the slope parameter(s) are jointly equal to 0 using an F test of explanatory power. To conduct this test on a model with k explanatory variables (and so with k slope parameters), our hypotheses will be: 

$$
H _ {0}: \beta_ {1} = \beta_ {2} = \dots = \beta_ {k} = 0
$$

$H _ { 1 } { \mathrm { : } }$ at least one of these parameters is not equal to zero 

The formula for the F test of explanatory power is: 

$$
F _ {k, n - k - 1} = \frac {R ^ {2} / k}{(1 - R ^ {2}) / n - k - 1}\tag{1.15}
$$

Decision rule: If $F > F _ { \mathrm { c r i t } } ,$ then reject $H _ { 0 }$ . 

In essence, the F test ofexplanatory power captures the relative magnitude of $R ^ { 2 } ;$ if $R ^ { 2 }$ is relatively large, then F is more likely to exceed $F _ { \mathrm { c r i t } }$ and the null of parameter values of zero on all the explanatory variables (i.e. of no association between the dependent variable and explanatory variables) will be rejected. 

In SRA, this F test statistic will be equal to the square of a Student’s t test statistic on $H _ { 0 } : \beta _ { 1 } = 0$ . But in MRA, the relationship becomes more complex and this relationship between t and F will break down. 

This section has illustrated the basic principles of hypothesis testing but we will use many other hypothesis tests in Running Regressions, for example another F test – the F test of restrictions (explained in detail in Chapter 5). 

## 1.8 What’s next?

Now that we have introduced the basic concepts underlying OLS regression analysis, we are ready to apply the principles to a range of real-world examples. To ensure that the econometric analysis is ‘digestibile’, we will introduce the tests and techniques one-by-one. For quick reference, the Gauss–Markov assumptions and basic formulae essential to running regressions are summarised in the Appendix to this chapter. For further details on the techniques, we have also suggested some relatively easy econometrics references in the section on further reading. 

Some good news about applied econometrics – an econometrician rarely has to do all the computational work him/herself. There are a variety of econometrics packages on the market with various pros and cons. In addition, regressions can be run relatively easily using most popular spreadsheet packages, e.g. running regressions in Excel can be done using the option ‘Data Analysis – Regression’ (usually accessible via ‘Tools’ in the Excel toolbar). In Chapter 2 ofthis book we do illustrate how you could run a regression ‘by hand (i.e. using a handheld calculator) to estimate a simple line of best fit because this illustrates the principles and procedures underlying OLS. For the remainder of the book, the models will be estimated either using a spreadsheet package (we use Excel) or a specialised econometric package (we use EViews). 

## 1.9 Further reading

This econometric introduction provides just a very brief and relatively intuitive summary of the econometric theory that underlies OLS because we want to concentrate on the interesting business of using the techniques to explain how socio-economic processes work. All of econometrics becomes a lot easier if you have a good understanding of the basic statistical concepts. The readings that follow represent good textbook introductions to various aspects of statistical and econometric theory. Most of these are printed in new editions every few years. 

## Introductory

Damodar N. Gujarati, Essentials ofEconometrics, New York: McGraw-Hill. 

Damodar N. Gujarati, Basic Econometrics, New York: McGraw-Hill. 

## Intuitive

Peter Kennedy, Guide to Econometrics, Oxford: Blackwell. 

## Good overall coverage

Christopher Dougherty, Introduction to Econometrics, Oxford: Oxford University Press. 

William H. Greene, Econometric Analysis, Upper Saddle River, NJ: Prentice-Hall. 

James H. Stock and Mark W. Watson, Introduction to Econometrics, Harlow: Pearson Education/Addison-Wesley. 

## Time series econometrics

R. L. Thomas, Modern Econometrics – An Introduction, Harlow: Addison-Wesley. 

Cross-sectional analysis and ‘microeconometrics 

Jeffrey M. Wooldridge, Introductory Econometrics – A Modern Approach, Thomson South-Western. 

## Appendix – Summary of assumptions and tests

## A.1 The Gauss–Markov Theorem

For OLS to give the Best Linear Unbiased Estimators (BLUE) in small samples, the following Gauss–Markov assumptions must be true: 

1. The mean or expected value of $\varepsilon _ { i } ,$ the error term, is zero: $E ( \varepsilon _ { i } ) = 0$ 

2. No autocorrelation in the errors, i.e. a zero covariance between error term for observation i and the error term for observation $j \colon \mathrm { c o v } ( \varepsilon _ { i } , \varepsilon _ { j } ) = 0$ 

3. Homoscedasticity, the variance of the error term, i.e. $\mathrm { v a r } ( \varepsilon _ { i } )$ , is a constant: $\mathrm { v a r } ( \varepsilon _ { i } ) = \sigma ^ { 2 }$ , where $\sigma ^ { 2 }$ is a constant. 

4. Exogeneity: $\mathrm { c o v } ( \varepsilon _ { i } , X _ { i } ) = 0$ where X is an explanatory variable. 

## A.2 Running regressions checklist

In general, the following steps should form the basis of any regression analysis: 

1. In constructing an empirical model carefully investigate the relevant theory and previous empirical research and specify your model accordingly. For example: if you are estimating a demand function then you will need to take the natural logs of your variables (see Chapter 3); for binary dependent variables, you will be estimating probabilities so you will need to use logit or probit techniques (see Chapter 12). 

2. Test hypotheses about individual significance (e.g. using Student’s t test) and joint significance (e.g. using F tests) explicitly stating your null and alternative hypotheses and decision rules. Remember that decision rules can be constructed around critical values or $\boldsymbol { p }$ values (see Chapters 2–4). 

3. Assess the goodness of fit as captured by $R ^ { 2 }$ in SRA (see Chapter 2) or $\bar { R } ^ { 2 }$ in MRA (see Chapter 5). 

4. Use F tests ofexplanatory power statistically to test the goodness offit (see Chapter 4). 

5. Visually inspect residuals to check for heteroscedasticity and autocorrelation (see Chapters 6 and 7). 

6. Conduct diagnostic tests for heteroscedasticity and autocorrelation (see Chapters 6 and 7). 

7. Conduct diagnostic tests for model misspecification e.g. Ramsey’s RESET test (see Chapter 8). 

8. If you do not have many observations, consider combining cross-sectional and time-series data in conducting a panel estimation (see Chapter 11). 

More specifically for time-series data, you will need to: 

9. Identify an appropriate lag structure (see Chapter 10). 

10. Check for structural breaks (see Chapter 9). 

11. Check for deterministic and stochastic trends (see Chapter 9). 

12. If variables are non-stationary, take differences until you identify a stationary form of the variables. Alternatively, check to see if non-stationary variables are cointegrated (see Chapters 9 and 10). 

## A.3 Essential formulae

## A.3.1 Residual sum of squares (RSS) and residual variance

$$
R S S = \sum \hat {\varepsilon} _ {i} ^ {2} = \sum \left(Y _ {i} - \hat {Y} _ {i}\right) ^ {2}
$$

$$
\hat {\sigma} _ {i} ^ {2} = \frac {R S S}{n - k - 1}
$$

A.3.2 Parameter estimates, variances and standard errors Slope 

$$
\hat {\beta} = \frac {\operatorname{cov} (X , Y)}{\operatorname{var} (X)} = \frac {\sum \left(X _ {i} - \bar {X}\right) \left(Y _ {i} - \bar {Y}\right)}{\sum \left(X _ {i} - \bar {X}\right) ^ {2}}
$$

$$
\operatorname{var} (\hat {\beta}) = \frac {\sigma^ {2}}{\sum (X _ {i} - \bar {X}) ^ {2}}
$$

$$
s e (\hat {\beta}) = \sqrt {\frac {\hat {\sigma} ^ {2}}{\sum (X _ {i} - \bar {X}) ^ {2}}}
$$

Intercept 

$$
\hat {\alpha} = \bar {Y} - \hat {\beta} \bar {X}
$$

$$
\operatorname{var} (\hat {\alpha}) = \left\{\frac {\sum X _ {i} ^ {2}}{n \sum (X _ {i} - \bar {X}) ^ {2}} \right\} \times \sigma^ {2}
$$

$$
s e (\hat {\alpha}) = \sqrt {\left\{\frac {\sum X _ {i} ^ {2}}{n \sum (X _ {i} - \bar {X}) ^ {2}} \times \hat {\sigma} ^ {2} \right.}\tag{1.10}
$$

A.3.3 Hypothesis tests and confidence intervals Student’s t test (two-tailed) 

$$
H _ {0}: \beta_ {1} = 0
$$

$$
H _ {1}: \beta_ {1} \neq 0
$$

$\hat { t } = \frac { \hat { \beta } - 0 } { s e ( \widehat { \beta } ) }$ ; i E ti ð1:14Þ 

Decision rule: if $| \hat { t } | < | t _ { \mathrm { c r i t } } |$ , then reject $\mathrm { H } _ { 0 }$ . If $- t _ { \mathrm { c r i t } } < \hat { t } < + t _ { \mathrm { c r i t } }$ then do not reject $H _ { 0 }$ 

## Confidence interval

The confidence interval is given by: 

$$
\left| \hat {\beta} \right| \pm s e (\hat {\beta}) \times t _ {\text { crit }}
$$

## A.3.4 Correlation and goodness of fit

$$
r _ {x y} = \frac {\sum (X _ {i} - \bar {X}) (Y _ {i} - \bar {Y})}{\sqrt {\sum (X _ {i} - \bar {X}) ^ {2} \sum (Y _ {i} - \bar {Y}) ^ {2}}} = \frac {\operatorname{cov} (X , Y)}{\sqrt {\operatorname{var} (X) \times \operatorname{var} (Y)}}
$$

$$
R ^ {2} = \frac {E S S}{T S S} = \frac {\sum (\hat {Y} - \bar {Y}) ^ {2}}{\sum (Y _ {i} - \bar {Y}) ^ {2}}
$$

Adjusted $R ^ { 2 }$ 

$$
\bar {R} ^ {2} = 1 - \left[ (1 - R ^ {2}) \times \frac {n - 1}{n - k - 1} \right]
$$

F test of explanatory power 

$$
H _ {0}: \beta_ {1} = \beta_ {2} = \dots = \beta_ {k} = 0
$$

$$
F _ {k, n - k - 1} = \frac {R ^ {2} / k}{(1 - R ^ {2}) / n - k - 1}
$$

Decision rule: If $F > F _ { \mathrm { c r i t } }$ , then reject $H _ { 0 }$ . 

# Running simple regressions Global poverty and economic growth

The test ofour progress is not whether we add to the abundance ofthose who have much; it is whether we provide enough for those who have too little. 

US President Franklin D. Roosevelt, 2nd inaugural address, 1937. 

Economic issues include: 

 Poverty reduction – the role of investment and trade 

 Millennium Development Goals (MDGs) 

 Development economics and development institutions 

Econometric issues include: 

 Correlation coefficients 

 Running OLS regressions ‘by hand 

 Single hypothesis tests: Student’s t test 

 Point estimates and confidence intervals 

 Goodness of fit and the coefficient of determination 

Data issues include: 

 Quantitative indicators of development 

 A qualitative indicator – the Human Poverty Index 

## 2.1 The issue

How can we reduce poverty and improve living standards for the poor? There are no easy answers and in addressing the problems of global poverty, the world’s heads ofstate met in September 2000 to discuss a universal framework for development, agreeing on targets to promote development. The then 189 UN member states agreed to the eight Millennium Development Goals (MDGs) listed in Box 2.1. Poverty reduction was one ofthese primary goals and the UN member states pledged to halve world poverty by 2015. These goals were 

## Box 2.1 The Millennium Development Goals (MDGs)

 Eradicate extreme poverty and hunger 

 Achieve universal primary education 

 Promote gender equality and empower women 

 Reduce child mortality 

 Improve maternal health 

 Combat HIV/AIDS, malaria and other diseases 

 Ensure environmental sustainability 

 Develop a global partnership for development 

Source: www.un.org/millenniumgoals/ 

reaffirmed at the World Summit held in September 2005, and the issue has been kept alive ever since by a number of high-profile awareness-raising and fund-raising events, backed by a diverse range of people – rockstars included. 

There is therefore a clear consensus on the importance of the MDGs themselves but little agreement about how to achieve them. The target date of 2015 is now not far away and there is a lot left to do. Many fear that the first decade ofthe new millennium will be marked down as one of lost opportunities, rather than improvements. In devising strategies, policies and initiatives to achieve the MDG of poverty reduction it is important for policy makers to have a good understanding ofhow poverty evolves in the first place. In this chapter, we make a start in analysing poverty by examining some simple statistical evidence about the relationship between poverty and economic growth. 

The problem of poverty amidst wealth and abundance has long concerned economists in both the developing and the developed world. There are many competing views and prescriptions about what to do about it and analysis of these is the focus of development economics, an area of economics that is of enormous interest to national governments, international organisations (such as the UN and its sister organisations), as well as to non-governmental organisations. In Box 2.2 there is a quick summary of the practical aspects of development economics as well as a list of some of the organisations particularly interested in analysing the process of development. 

## Defining poverty

In this chapter we explain the distinction between relative poverty and absolute poverty. Relative poverty is manifested in inequalities of income 

## Box 2.2 ‘Doing’ development economics

In one sense, almost all economists are interested in the topic of development, in that we strive for ways to better understand and to improve human welfare and economic life. However a number of individuals and institutions focus in particular on these challenges in the more extreme context of developing countries, or in the pockets of under-development that exist within countries that are otherwise rich and ‘developed’. The topic is increasing in popularity, at both the theoretical and the practical level, perhaps as a response to concerns that so much remains to be done but also with the increasing recognition that problems that do not initially appear to be economic in nature often have underlying economic causes and solutions. For example, the 1998 Nobel laureate, Amartya Sen, used the tools of economics to challenge the conventional assumption that starvation was caused by food shortages, droughts and famines. His 1981 book Poverty and Famines showed that many recent famines had occurred when there was no significant shortage of food arguing that institutional constraints and other economic features are the cause of starvation so institutional reform should be central to policy solutions. Increasingly development economists today are focussing on institutional features relating to poverty and under-development, including the role of ‘good government’; failures of international and national capital markets; and the importance of international trade rules, rather than focussing on inherent features of the natural world. 

Readers who are interested in learning more about the scale and scope of practical development economics can view the wide range of current initiatives being conducted by economists (and lawyers, social scientists, health professionals etc.) in the small selection of websites of development organisations listed below. Many of the better-known agencies, institutions and non-governmental organisations (NGOs) also offer internships (paid or voluntary) and interesting full or part-time careers. Most universities also offer courses in development economics at the graduate level, in addition to introductory courses at the undergraduate level. 

Some interesting websites 

<table><tr><td colspan="2">Governmental organisations</td></tr><tr><td>United Nations Development Programme</td><td>www.undp.org</td></tr><tr><td>World Health Organisation</td><td>www.who.org</td></tr><tr><td>International Monetary Fund</td><td>www.imf.org</td></tr><tr><td>UN Research Institute for Social Development</td><td>www.unrisd.org</td></tr><tr><td>Asian Development Bank</td><td>www.adb.org</td></tr><tr><td>African Development Bank</td><td>www.afdb.org</td></tr><tr><td>Inter-American Development Bank</td><td>www.iadb.org</td></tr><tr><td>UN Economic Commission for Europe</td><td>www.unece.org</td></tr><tr><td>UN Food and Agriculture Organisation</td><td>www.fao.org</td></tr><tr><td>UN Conference for Trade and Development</td><td>www.unctad.org</td></tr><tr><td>UN University World Institute for Economic Development Research</td><td>www.wider.un.edu</td></tr><tr><td>World Bank</td><td>www.worldbank.org</td></tr><tr><td>Organisation for Economic Cooperation and Development</td><td>www.oecd.org</td></tr><tr><td>International Labour Organisation</td><td>www.ilo.org</td></tr><tr><td>Australian Government Overseas Aid</td><td>www.ausaid.gov.au</td></tr><tr><td>International Development Research Centre (Canada)</td><td>www.idrc.ca</td></tr><tr><td>UK Department for International Development</td><td>www.dfid.gov.uk</td></tr><tr><td>US Agency for International Development</td><td>www.usaid.gov</td></tr><tr><td>International jobs in development economics</td><td>www.devnetjobs.org</td></tr><tr><td>Non-governmental organisations</td><td></td></tr><tr><td>Oxfam</td><td>www.oxfam.org</td></tr><tr><td>World Vision</td><td>www.worldvision.org</td></tr><tr><td>Care</td><td>www.care.org</td></tr></table>

and wealth. Relative poverty is the focus of a particular and special intensity in the modern world but concerns about people’s relative positions in an economy are not new. As early as 400 BC the Greek philosopher Plato had advised that the gap between the richest and the poorest citizens should never be greater than a factor of four – i.e. that the richest should be no more than four times wealthier than the poorest. Plato argued that this 4:1 ratio was necessary not only for ethical and moral reasons, but also for practical and pragmatic ones: greater inequality could fuel civil violence or even war. At the 2001 World Economic Forum meeting, held in New York in the aftermath of the September 11 tragedy, UN Secretary General, Kofi Annan likened the world’s rich and poor to fellow passengers on an unstable boat: 

None of us can afford to ignore the condition of our fellow passengers on this little boat. If they are sick, all of us risk infection. And if they are angry, all of us can easily get hurt. 

How does the modern world match-up in terms of Plato’s ideal? Table 2.1 shows the relationship between relative incomes in a selection of countries and reveals some stark differences. In Argentina for example, the richest decile (i.e. the richest 10% of the population) received an income that was on average 40 times higher than the country’s poorest decile. In Brazil the gap between the top and bottom decile was even greater. At the global level, the richest decile of the world’s population (who live for the most part in North America, Europe and parts of Asia) had income levels that were more than 100 times higher than the poorest 10% – who live, for the most part, in the Least Developed Countries (LDCs). Table 2.1 also shows that richer, more developed countries can also have large gaps between their richest and poorest decile. In the United States, for example, the richest decile earned 16 times as much as the poorest decile . Plato’s four-fold ratio clearly fails to hold today; in 2005, only Japan was close to Plato’s ideal ratio. Furthermore, research by World Bank economists Ravallion, Chen and Sangraula (2008) suggests that relative poverty has been worsening in the developing world in recent years. 


Table 2.1 Relative incomes of rich and poor<sup>1</sup>


<table><tr><td colspan="2">On average, how many times as much income do the richest 10% earn relative to the poorest 10%? Factor differences in income between richest and poorest deciles:</td></tr><tr><td>Argentina</td><td>40</td></tr><tr><td>Brazil</td><td>94</td></tr><tr><td>Japan</td><td>4.5</td></tr><tr><td>Switzerland</td><td>10</td></tr><tr><td>United States</td><td>16</td></tr><tr><td>The world</td><td>103</td></tr></table>


Source: UNDP 2005. 


While inequality is clearly a major aspect of poverty, recent approaches to the subject have tended to focus less on relative poverty, and more on absolute poverty. This is reflected in the use of benchmarks, capturing a ‘breadline’ of decent living below which society should not allow households to slip. At the national level, different countries use different definitions of their breadline, depending on national income, and on national perceptions of what constitutes their society’s minimum bundle of goods and capabilities. At the global level, this approach has culminated in a concrete, quantitative definition of poverty as the condition affecting people trying to live on less than $1 per day. This defines a global ‘social floor’ that makes it easy to see first, how countries perform relative to each other and second, if there have been improvements 

Source: United Nations Development Program (UNDP), Human Development Report 2005. 


Box 2.3 Poverty and development: the record so far



Development record of the last decade:


<table><tr><td>The positives</td><td>The negatives</td></tr><tr><td>130 million people were lifted out of extreme poverty</td><td>2.5 billion people still live on less than $2 a day</td></tr><tr><td>2 million fewer child deaths a year</td><td>10 million preventable child deaths a year</td></tr><tr><td>30 million more children are in school</td><td>115 million children are still out of school – especially girls</td></tr><tr><td>1.2 billion people gained access to clean water</td><td>More than 1 billion people still have no access to safe water</td></tr><tr><td></td><td>2.6 billion lack access to sanitation</td></tr></table>

over time. It is easier to reduce absolute poverty (e.g. through cash transfer programmes) than to reduce inequality (redistribution of assets via land reform is problematic in countries where inequality has been embedded for centuries). 

Box 2.3 summarises the development record from the last decade and illustrates that whilst much has been achieved, much remains to be done. 

## 2.2 The theory

Abstracting from the complexity ofissues relevant to development economics, the particular economic theory tested in this chapter is that the key to poverty reduction is rapid and sustained economic growth. The idea is that, if incomes and wealth are growing in one sector of the economy, then the benefits of growth will ‘trickle down’ to poorer groups. This is of course an extremely simplistic way to phrase trickle-down theory, and nobody thinks that growth is the only factor affecting poverty, but the core of this view is widely supported. Most undergraduate texts in economics take it as given that growth will moderate poverty – for example Lipsey and Chrystal (2007) summarise a vast literature on growth, development and poverty by concluding that ‘economic growth is the economy’s most powerful engine for generating longterm increases in living standards’. Even those with opposing views are likely to agree that it is easier to slice and re-distribute an expanding cake, rather than a shrinking one. The real controversy lies in answering the prior question of how to achieve growth in the first place. There are many competing theories on this subject, some of which arise in subsequent chapters of this book. Keynesian models, for example, emphasise the role of household consumption; others have focused on the role of labour productivity. More recently writers have emphasised the role of factors such as savings and investment (e.g. Swan, 1956, Solow, 1956) and human capital effects gained through education and human capital formation (e.g. Mankiw, Romer and Weil, 1992). An excellent overview of the subject is given by Thirlwall (2005) in the introductory textbook Growth and Development. 

As described more fully by United Nations Conference for Trade and Development in its Least Developed Countries Report 2002 (UNCTAD, 2002), economic growth enables LDCs to reduce domestic poverty because of its impact upon household income and consumption. UNCTAD’s story is an extension of earlier arguments by Rodrik (1999), who asserted that countries that had had rapid growth alongside rapid poverty reductions had also directed more and more oftheir domestic production towards export markets. And this trend was particularly pronounced amongst low-income countries. The UNCTAD Report describes a cycle where LDCs experience a process of ‘late industrialisation’, brought about by increases in investment. This investment enables sectors of the economy that were previously marginal (e.g. subsistence agriculture) to become productive. New investment leads to the construction of factories, transport and communications networks, which allow modern industrial manufacturing processes to replace traditional agricultural and pre-industrial systems. Resources are gradually shifted away from the traditional activities and into higher technology and capital-intensive industries. New products are created which can be exported to global markets that pay higher prices than local markets. As the share ofdomestic production geared towards exports increases, wages rise and job opportunities are increased. Incomes rise, household consumption rises, and poverty levels fall through a series of trickle-down effects. 

This chapter provides some data that can be used in testing some assertions from the UNCTAD report. There are two sets of simple and readily testable theories/assumptions that can be explored: 

(a) economic growth affects poverty, 

(b) increased investment and exports lead to economic growth. 

Below, we test hypothesis (a) via a cross-sectional analysis comparing the relative performance of 31 LDCs over a period of twelve years. We predict that countries with higher levels of growth were more able to reduce poverty than countries with lower growth. For hypothesis (b) we would expect that countries with higher levels of investment and increased export orientation will have experienced faster growth than countries without increased investments or exports.<sup>2</sup> 

## 2.3 The data

The data used in this chapter is taken from UNCTAD (2002) but comparable data is readily available elsewhere, including for example the IMF, World Bank, UN WIDER inequality and poverty database and national accounts. In all cases we look at the data in terms of the change in the indicators, over the years from 1987 to 1999. We do this primarily because our focus is on the extent to which poverty levels have worsened or improved rather than absolute poverty levels (which will be affected by many other factors in addition to economic growth). (see e.g. poverty studies network www.chronicpoverty.org.) 

It is helpful in research analyses to present a detailed ‘descriptive analysis’ of the data before going on to regression analysis, to tease out the broad patterns. The data set presented in Annex 2.2 – Table 2.6 focusses on the following variables: change in absolute poverty, measured as the percentage change in the proportion of the population living on $1 per day or less; annual average GDP growth per capita; % change in exports as a share of GDP; and investment, measured as the growth in gross capital formation (GCF). 

In column 1 of Table 2.6 we have our dependent variable – poverty. Over the period 1987–1999 this indicator ranged from an increase in poverty of 37.2% (Sierra Leone) to a decrease in poverty of20.4% (Malawi). The mean or average for the sample reflected a slight increase in poverty (of + 1.63%) but there was considerable variance across the individual countries in the sample. 

In column 2 we have our explanatory variable: economic growth. This is measured as the rate of change in GDP per capita. Over the years studied, this ranged from + 3.5% (Lao Peoples’ Democratic Republic) to –5.7% (Sierra Leone). The average was slightly negative at –0.2%. 

The change in exports as a share of GDP is in column 3. This also varied considerably from country to country, around an average increase of 4.7%. Angola scored particularly highly with an export growth rate of 23.6% per annum, reflecting sales of natural resources such as oil and diamonds; 

but incomes from these commodity sales were accrued by a small fraction of Angola’s population and/or spent on imports and so would not necessarily foster improved living standards amongst Angola’s poorest. 

In column 4, we have investment growth, measured as the rate of change of Gross Capital Formation (GCF); GCF measures the change in the capital stock i.e. the accumulation ofphysical capital including factories, plant and machinery. This was slow – increasing by an average of only 1.6% over the sample period, perhaps reflecting the relatively stagnant rates of economic growth mentioned above. 

Focussing just on the associations between poverty and GDP growth: of the 31 countries in our sample, 16 countries experienced rising GDP per capita. For most of these 16 countries this was associated with reduced poverty but the two exceptions were Lesotho and Mali. Of the declining growth countries, Sierra Leone quite spectacularly exhibited what we expected, with GDP falling by 5.7% and poverty levels rising sharply by 37.2%. 

## Empirical results and interpretation

We can test the accuracy of this verbal description of the data by using some simple techniques. We start with correlation analysis and by running a regression – statistically to capture the degree of association between changing poverty and growth in GDP per capita. 

The following pages work through the hypothesis that growth in GDP is associated with reductions in poverty using the same data set and techniques introduced in Chapter 1. As explained in Chapter 1, the first step in statistical analysis is to start with an empirical hypothesis and construct an empirical model around it. This empirical model should capture the hypothesised data generating process (DGP). Our hypothesis is that GDP growth is negatively associated with changing poverty and that this association takes a linear form, so this hypothesis can be expressed mathematically as follows: 

$$
Y _ {i} = \alpha + \beta X _ {i} + \varepsilon_ {i} \quad \beta <   0\tag{2.1}
$$

where $Y _ { i } = \mathrm { c h a n g e }$ in proportion ofpopulation living on $1/day for country for the 31 countries in our sample (from Lao PDR, i = 1, to Sierra Leone, i = 31) 

$X _ { i } = \mathrm { c h a n g e }$ in average annual GDP per capita (also for each country i) 

α = intercept parameter 

β = slope parameter (capturing the change in Y for a unit change in X) 

ε = stochastic (i.e. random) error term 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/1557394eaad6ddb6ca3c32ec1b82eed756bf93926efe9ba2432dda39bb9aa064.jpg)



Figure 2.1 Poverty and growth


A good starting point in any empirical analysis is to have a look at some plots of the data. This sort of visual inspection can reveal some of the broad and/or stark patterns in the data. It’s also a good way to check that there aren’t any obvious problems with data. 

Focussing on poverty and growth, we can have a look at the data to see if the inverse association between economic growth and poverty predicted by our theory is a realistic hypothesis. Figure 2.1 shows a simple scatter plot showing for each country the pairs of observations on the dependent variable Y (change in poverty) and the explanatory variable X (GDP growth per capita). 

Our data sample of observations on changing poverty and GDP growth are presented in Figure 2.1. The two ‘centres of gravity’ created by the two sample averages or means are depicted by a dotted vertical line at the mean GDP growth rate change of −0.2; and a dotted horizontal line at the mean poverty change of 1.63. 

Most countries are either in the SE quadrant with a (−,+) association between poverty changes and GDP growth, or in the NW quadrant with a (+,−) association for each pair of observations. 

So there is a negatively sloped clustering running from the north-west (NW), top left-hand side of the graph to the south-east (SE) corner of the graph. 

Specifically the north-west (NW) quadrant of Figure 2.1 contains countries whose poverty levels worsened and whose GDP growth slowed – i.e. $Y _ { i } > \bar { Y }$ and $X _ { i } { < } \bar { X }$ . More specifically in the NW corner, Sierra Leone is a particularly extreme example ofa country in which growth was low and poverty worsened. 

The SE quadrant contains countries whose poverty levels were falling by more than the mean, and whose GDP was growing fast – i.e. $Y _ { i } < \bar { Y }$ and $X _ { i } { > } \bar { X }$ Uganda stands out as an example here. 

Countries in the NE quadrant are characterised by a (+,+) relationship reflecting disproportionate rises in poverty in spite ofrelatively fast growth (i.e $Y _ { i } > \bar { Y }$ and $X _ { i } > { \bar { X } } )$ ; only Mali and Lesotho appear in this quadrant. In the SW quadrant are the countries that experienced a $( - , - )$ relationship with lower than average GDP growth but also a lower than average worsening ofpoverty – i.e. $Y _ { i } < \bar { Y }$ and $X _ { i } < \bar { X }$ . Gambia, Togo and Angola are in this quadrant. 

But these countries are in a clear minority. On balance the sample is dominated by countries which, one way or the other, are characterised by an inverse association between changing poverty and GDP growth. So our initial inspection of the data verifies the basic hypothesis: the scatter plot in Fig. 2.1. is consistent with our basic hypothesis that poverty reduction is associated with GDP growth. We further verify this pattern when we measure the correlation coefficient and run a regression. 

## Capturing correlation

In getting a more objective measure of the nature of clustering in the scatter plot we can measure the correlation between the two variables – i.e. the extent of linear association or statistical dependence between two variables. As explained in Chapter 1, the first step in assessing correlation involves measuring the extent to which the two series ‘co-vary’. Mathematically, covariances are the product of deviations from means. The measure of movements between two variables relative to their respective means in a given sample of data is the sample covariance. Some of the data transformations needed to measure this covariance are summarised in Table 2.2. 

As explained in Chapter 1, the correlation coefficient is a ‘normalised’ measure of the linear association between two variables and the range of possible values is $- 1 \le r _ { X Y } \le + 1$ . Using variable transformations shown in columns 5, 6 and 8 of Table 2.2 and the method for calculating correlation coefficients outlined in Chapter 1 gives: 

$$
\begin{array}{l} r _ {X Y} = \frac {\sum (X _ {i} - \bar {X}) (Y _ {i} - \bar {Y})}{\sqrt {\sum (X _ {i} - \bar {X}) ^ {2} \sum (Y _ {i} - \bar {Y}) ^ {2}}} = \frac {\operatorname{cov} (X , Y)}{\sqrt {\operatorname{var} (X) \times \operatorname{var} (Y)}} \\ = \frac {- 6 6 3 . 8}{\sqrt {1 7 9 . 3 \times 5 5 4 0 . 5}} = - 0. 6 6 \end{array}\tag{2.2}
$$


Table 2.2 Changing poverty (Y) and GDP growth (X ): regression by hand


<table><tr><td rowspan="2"></td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>7</td><td>8</td></tr><tr><td><eq>Y_i</eq></td><td><eq>X_i</eq></td><td><eq>X_i - \bar{X}</eq></td><td><eq>Y_i - \bar{Y}</eq></td><td><eq>(X_i - \bar{X})(Y - \bar{Y})</eq></td><td><eq>(X_i - \bar{X})^2</eq></td><td><eq>X_i^2</eq></td><td><eq>(Y_i - \bar{Y})^2</eq></td></tr><tr><td>Lao PDR</td><td>-2</td><td>3.5</td><td>3.7</td><td>-3.6</td><td>-13.4</td><td>13.7</td><td>12.3</td><td>13.2</td></tr><tr><td>Bangladesh</td><td>-3.4</td><td>3.3</td><td>3.5</td><td>-5.0</td><td>-17.6</td><td>12.3</td><td>10.9</td><td>25.3</td></tr><tr><td>Uganda</td><td>-16.1</td><td>3.1</td><td>3.30</td><td>-17.7</td><td>-58.5</td><td>10.9</td><td>9.6</td><td>314.4</td></tr><tr><td>Bhutan</td><td>-19.2</td><td>3</td><td>3.20</td><td>-20.8</td><td>-66.7</td><td>10.2</td><td>9.00</td><td>433.9</td></tr><tr><td>Cape Verde</td><td>-6.3</td><td>2.9</td><td>3.1</td><td>-7.9</td><td>-24.6</td><td>9.6</td><td>8.4</td><td>62.9</td></tr><tr><td>Mozambique</td><td>-3.6</td><td>2.5</td><td>2.7</td><td>-5.2</td><td>-14.1</td><td>7.3</td><td>6.3</td><td>27.4</td></tr><tr><td>Nepal</td><td>-14.3</td><td>2.4</td><td>2.6</td><td>-15.9</td><td>-41.4</td><td>6.8</td><td>5.8</td><td>253.8</td></tr><tr><td>Solomon Is</td><td>-4.1</td><td>1.4</td><td>1.6</td><td>-5.7</td><td>-9.2</td><td>2.6</td><td>2.0</td><td>32.8</td></tr><tr><td>Benin</td><td>-6.1</td><td>1</td><td>1.2</td><td>-7.7</td><td>-9.3</td><td>1.4</td><td>1.00</td><td>59.8</td></tr><tr><td>Malawi</td><td>-20.4</td><td>0.9</td><td>1.1</td><td>-22.0</td><td>-24.2</td><td>1.2</td><td>0.8</td><td>485.3</td></tr><tr><td>Ethiopia</td><td>-1.2</td><td>0.8</td><td>1.0</td><td>-2.83</td><td>-2.8</td><td>1.0</td><td>0.6</td><td>8.0</td></tr><tr><td>Lesotho</td><td>22.3</td><td>0.7</td><td>0.9</td><td>20.7</td><td>18.6</td><td>0.8</td><td>0.5</td><td>427.2</td></tr><tr><td>Burkina Faso</td><td>-6.5</td><td>0.4</td><td>0.6</td><td>-8.1</td><td>-4.9</td><td>0.4</td><td>0.2</td><td>66.1</td></tr><tr><td>Mali</td><td>8.7</td><td>0.1</td><td>0.3</td><td>7.1</td><td>2.1</td><td>0.1</td><td>0.0</td><td>50.0</td></tr><tr><td>Senegal</td><td>0.8</td><td>0</td><td>0.2</td><td>-0.8</td><td>-0.2</td><td>0.0</td><td>0.0</td><td>0.7</td></tr><tr><td>Central African Republic</td><td>23.3</td><td>-0.8</td><td>-0.6</td><td>21.7</td><td>-13.0</td><td>0.4</td><td>0.6</td><td>469.6</td></tr><tr><td>Chad</td><td>2.5</td><td>-1.3</td><td>-1.1</td><td>0.9</td><td>-1.0</td><td>1.2</td><td>1.7</td><td>0.8</td></tr><tr><td>Vanuatu</td><td>3.5</td><td>-1.3</td><td>-1.1</td><td>1.9</td><td>-2.1</td><td>1.2</td><td>1.7</td><td>3.5</td></tr><tr><td>Guinea-Bissau</td><td>25</td><td>-1.6</td><td>-1.4</td><td>23.4</td><td>-32.7</td><td>2.0</td><td>2.6</td><td>546.2</td></tr><tr><td>Madagascar</td><td>4.5</td><td>-1.8</td><td>-1.6</td><td>2.9</td><td>-4.6</td><td>2.6</td><td>3.2</td><td>8.2</td></tr><tr><td>Comoros</td><td>11.8</td><td>-3.5</td><td>-3.3</td><td>10.2</td><td>-33.6</td><td>10.9</td><td>12.3</td><td>103.4</td></tr><tr><td>Angola</td><td>1.5</td><td>-3.8</td><td>-3.6</td><td>-0.1</td><td>0.5</td><td>13.0</td><td>14.4</td><td>0.0</td></tr><tr><td>Mauritania</td><td>-6.2</td><td>1.6</td><td>1.8</td><td>-7.8</td><td>-14.1</td><td>3.2</td><td>2.6</td><td>61.3</td></tr><tr><td>Guinea</td><td>-7.4</td><td>0.8</td><td>1</td><td>-9.0</td><td>-9.0</td><td>1.0</td><td>0.6</td><td>81.5</td></tr><tr><td>Gambia</td><td>-16.3</td><td>-0.9</td><td>-0.7</td><td>-17.9</td><td>12.6</td><td>0.5</td><td>0.8</td><td>321.5</td></tr><tr><td>Togo</td><td>-1.7</td><td>-2</td><td>-1.8</td><td>-3.3</td><td>6.0</td><td>3.2</td><td>4.0</td><td>11.1</td></tr><tr><td>Niger</td><td>5.1</td><td>-2</td><td>-1.80</td><td>3.5</td><td>-6.2</td><td>3.2</td><td>4.0</td><td>12.0</td></tr><tr><td>Rwanda</td><td>13.1</td><td>-2.9</td><td>-2.7</td><td>11.5</td><td>-31.0</td><td>7.3</td><td>8.4</td><td>131.6</td></tr><tr><td>Burundi</td><td>11</td><td>-3.4</td><td>-3.20</td><td>9.4</td><td>-30.0</td><td>10.2</td><td>11.6</td><td>87.8</td></tr><tr><td>Haiti</td><td>14.9</td><td>-3.5</td><td>-3.3</td><td>13.3</td><td>-43.8</td><td>10.9</td><td>12.3</td><td>176.1</td></tr><tr><td>Sierra Leone</td><td>37.2</td><td>-5.7</td><td>-5.5</td><td>35.6</td><td>-195.6</td><td>30.3</td><td>32.5</td><td>1265.2</td></tr><tr><td>Mean</td><td>1.63</td><td>-0.20</td><td></td><td></td><td>-21.4</td><td></td><td></td><td></td></tr><tr><td>Total</td><td></td><td></td><td></td><td></td><td>-663.8</td><td>179.3</td><td>180.5</td><td>5540.5</td></tr></table>

This indicates that there is a strongly negative statistical association between the variables Y and X of −0.66. Note that, in a two-variable context, the calculation of the correlation coefficient is not affected by which variable is the dependent variable and which variable is the explanatory variable. (It becomes more complex when there are more variables because there may be indirect effects.) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/b305ef9d3ea5d0f4852347cf1d57a6b30794dbf6b027a11adb45ed7fab2ce589.jpg)



Figure 2.2 Line of best fit


Overall $r { = } { - } 0 . 6 6$ is consistent both with our initial hypothesis and with our visual inspection of the scatter plot. This high and negative correlation between changing poverty and GDP growth per capita is encouraging for our initial hypothesis. 

## Running a regression

From the correlation coefficient we have some information about the direction and magnitude of linear association between Y and X. To get more information about the form of the correlation, we can use OLS to estimate the parameters of a model. As explained in Chapter 1, econometric analysis often starts with an estimation of a line of best fit or a ‘regression’ line. In this section we will investigate simple regression analysis (i.e. a regression on just one explanatory variable). Multiple regression analysis, when more than one explanatory variable is used, is explored from Chapter 5 onwards. 

The concept of a line of best fit can be understood visually by imagining how to place the line so that it fits the observations neatly with a small spread of observations around the line (see Figure 2.2). 

When we run our regression, the extent to which the two series co-vary together will be manifested in estimates for coefficients α and $\beta ,$ , their standard errors and the estimate of the sample variance $\hat { \sigma } ^ { 2 }$ 

## Parameter estimates

Using the formulae outlined in Chapter 1, the parameter estimates can be calculated by plugging the numbers from Table 2.2 into the following formulae: 

$$
\hat {\beta} = \frac {\operatorname{cov} (X , Y)}{\operatorname{var} (X)} = \frac {\sum \left(X _ {i} - \bar {X}\right) \left(Y _ {i} - \bar {Y}\right)}{\sum \left(X _ {i} - \bar {X}\right) ^ {2}} = \frac {- 6 6 3 . 8}{1 7 9 . 3} = - 3. 7 0\tag{2.3}
$$

and 

$$
\hat {\alpha} = \bar {Y} - \hat {\beta} \bar {X} = 1. 6 3 - (- 3. 7 0 \times - 0. 2 0) = 0. 8 9\tag{2.4}
$$

So our estimated line of best fit is: 

$$
\hat {Y} _ {i} = 0. 8 9 - (3. 7 0 \times X _ {i})\tag{2.5}
$$

The result that $\hat { \beta } \ = - 3 . 7 0$ confirms that the association between GDP growth and poverty change is negative, i.e. $\hat { \beta }$ has the negative sign expected by our theory and suggests that there is a strong negative association between changing poverty and GDP growth. For this sample of data, a 1% increase in GDP growth is associated with a 3.7% decrease in the proportion of people living on $1/day. 

## Drawing inferences and constructing hypothesis tests

There does seem to be an association but what can we infer from it? Perhaps the negative association is not a robust measure of a real association. We need a benchmark to decide how large or small our parameter estimates are relative to our initial hypothesis. To establish this we use a hypothesis test to test how statistically significant is the difference between our parameter estimates (which took the values 0.89 and –3.70 respectively) and the benchmark null hypothesis. 

In this case we are testing a single hypothesis about the relationship between poverty and GDP growth. So the null and alternative hypotheses are as follows: 

$$
\begin{array}{l l} \text {Null hypothesis} & H _ {0} \colon \beta = 0 \\ \text {alternative hypothesis} & H _ {1} \colon \beta \neq 0. \end{array}
$$

When the alternative hypothesis is true, i.e. when $\beta \neq 0 ;$ , GDP growth does have an impact on poverty. 

If we wanted to be more precise we could test $H _ { 0 }$ against $H _ { 1 } \colon \beta < 0$ using a one-tailed test but, in the interests of simplicity, we are using a two-tailed test in this chapter; one-tailed hypothesis tests are illustrated in Chapter 3. 

As explained in Chapter 1, to test this sort of single hypothesis we can use Student’s t test to estimate a t statistic. As is shown below, to calculate Student’s t test we need measures of the standard errors of the parameter estimates, and the procedure for calculating these is explained in Box 2.4. 

## Box 2.4 The standard errors of the parameter estimates

The starting point in calculating the standard error of the parameter estimates is to get an estimate of the variance of the sample estimate $( \hat { \sigma } ^ { 2 } )$ . This is found using the residual sum of squares (RSS) and dividing through by degrees of freedom, as explained in Chapter 1. The residual sum of squares has been calculated in column 7 of Table 2.3 using the following formula: 

$$
R S S = \Sigma \hat {\varepsilon} _ {i} ^ {2} = \sum (Y _ {i} - \hat {Y} _ {i}) ^ {2}\tag{2.6}
$$

Then the RSS is divided by the degrees of freedom $( = n { - } k { - } 1 )$ where k is the number of explanatory variables. We have 31 observations so $\eta = 3 1 ; k = 1$ so we lose one degree of freedom in estimating the slope parameter and another from estimating the intercept parameters. So the degrees of freedom are $3 1 - 2 = 2 9 .$ 

Using the RSS and degrees of freedom (df) we can calculate the variance of the estimate as follows: 

$$
\hat {\sigma} ^ {2} = \frac {\sum \hat {\varepsilon} _ {i} ^ {2}}{(n - k - 1)} = \frac {3 0 8 2 . 8}{3 1 - 2} = 1 0 6. 3\tag{2.7}
$$

where $\Sigma \hat { \varepsilon } _ { i } ^ { 2 }$ is the residual sum of squares (RSS) and $d f = \eta - k - 1$ 

We are now ready to find the standard errors of each of the two estimated coefficients using the method explained in Chapter 1.<sup>3</sup> All the information needed has already been calculated above and in Table 2.3 so plugging these numbers in gives: 

$$
s e (\hat {\beta}) = \sqrt {\frac {\hat {\sigma} ^ {2}}{\sum (X _ {i} - \bar {X}) ^ {2}}} = \sqrt {\frac {1 0 6 . 3}{1 7 9 . 3}} = 0. 7 7\tag{2.8}
$$

Similarly the standard error of the intercept parameter can be calculated following the procedure outlined in Chapter 1: 

$$
s e (\hat {a}) = \sqrt {\frac {\sum X _ {i} ^ {2}}{n \sum (X _ {i} - \bar {X}) ^ {2}} \times \hat {\sigma} ^ {2}} = \sqrt {\frac {1 8 0 . 5 \times 1 0 6 . 3}{3 1 \times 1 7 9 . 3}} = 1. 8 6\tag{2.9}
$$

Using the parameter estimates and their associated standard errors, a Student’s t test on our point estimate of $\hat { \boldsymbol { \beta } }$ can be calculated as follows: 

$$
\hat {t} = \frac {\hat {\beta} - \beta_ {H _ {0}}}{s e (\hat {\beta})} = \frac {- 3 . 7 0}{0 . 7 7} = - 4. 8 1\tag{2.10}
$$

where $\beta _ { H _ { 0 } }$ is the value of $\beta$ hypothesised within our null, $\hat { \beta }$ is our point estimate of $\beta$ and $s e ( \hat { \beta } )$ is the standard error of ${ \bf \ddot { \boldsymbol { \beta } } } .$ 

Similarly the t test for the intercept parameter $\hat { \alpha }$ gives: 

$$
\hat {t} = \frac {\hat {\alpha} - \alpha_ {H _ {0}}}{s e (\hat {\alpha})} = \frac {0 . 8 9}{1 . 8 6} = 0. 4 8\tag{2.11}
$$

The next step is to find out whether or not these estimates of the t statistics are significantly different from the null hypothesis. 

Concentrating on the slope parameter, the alternative hypothesis is that $\beta$ is not equal to zero so we will be assessing whether or not the estimated t statistic is more extreme than the critical value using a two-tailed t test. The critical value of a test statistic marks the boundary between relatively likely and relatively unlikely, as we will illustrate below. Our decision rule will be to reject $H _ { 0 }$ if the absolute value of the t statistic is ‘significantly greater’ than 0 at a 5% significance level. 

But what do we mean by a significance level? As explained in Chapter 1, critical values are determined by the significance level. If a critical value of a test statistic (e.g. a t statistic) is selected using a 5% significance level, this means that we would expect to see an estimated t value more extreme than the critical value in only 5% of samples, i.e. it is quite unlikely that we would see such extreme t values ifthe null were true. Therefore, ifour estimated t is more extreme than our critical value, then it follows that we will reject our null hypothesis. This doesn’t mean that our null is wrong; it just means that it doesn’t seem very probable for the sample of data that we’re using. 

It is important to remember that the selection of the significance level does introduce some arbitrariness into hypothesis testing. However, there are conventions – i.e. 1%, 5% and 10% significance levels are commonly used in statistical analysis.<sup>4</sup> 

For our analysis of the relationship between poverty and GDP growth, we select a 5% significance level. With df= 29 and two-tailed test, the critical value of our t statistic will be $t _ { \mathrm { c r i t } } = 2 . 0 4$ where $t _ { \mathrm { c r i t } }$ is the ‘critical value’. So our decision rule is: if $| \hat { t } | > | t _ { \mathrm { c r i t } } |$ , then reject $H _ { 0 }$ . $\mathrm { I f } - t _ { \mathrm { c r i t } } < \hat { t } < + \ t _ { \mathrm { c r i t } }$ then do not reject $H _ { 0 }$ . 

So, with a 5% significance level, we reject our null and conclude that $\hat { \beta }$ is statistically ‘significant’. This is shorthand (in a two-tailed test context) for saying that $\hat { \beta }$ is statistically significantly different from the null $( H _ { 0 } \colon \beta = 0 )$ so we can reject the null hypothesis and verify the alternative hypothesis. We have evidence confirming a significant association between falling poverty rates and rising GDP growth per capita. If we wanted a more powerful test of this, we could use a one-tailed test but, as noted above, we are using two-tailed tests to keep the analysis simple. But once you have read the illustration of one-tailed hypothesis tests, outlined in Chapter 3, you could try a one-tailed test on this example. 

Comparing a point estimate oft statistic against the relevant critical value is just one way of assessing a hypothesis. But, as explained in Chapter 1, another way to assess hypotheses is to use confidence intervals. In this case we will use a 95% confidence interval; this should capture the true value of $\beta$ in 95% of samples. It is important to remember first, that we are using just one sample of data; and second, that there is always a 5% probability that the true value of $\beta$ is not captured within our confidence interval. For this reason, we cannot prove anything about the value of $\dot { \boldsymbol { \beta } } ;$ we can only make inferences about what is likely given our evidence. 

That said, the formula for the confidence interval in this case is: 

$$
\left| \hat {\beta} \right| \pm s e (\hat {\beta}) \times t _ {\text { crit }}\tag{2.12}
$$

So our confidence interval for $\beta$ is: 

$$
\begin{array}{l}- 3. 7 0 - (0. 7 7 \times 2. 0 4) <   \beta <   - 3. 7 0 + (0. 7 7 \times 2. 0 4)\\\rightarrow - 5. 2 7 <   \beta <   - 2. 1 3\end{array}
$$

Our value of $\beta$ postulated within our $H _ { 0 } ,$ i.e. of $\beta = 0$ , does not fall within our confidence interval and therefore we can reject $H _ { 0 }$ . This finding is completely consistent with the t test on the point estimate ${ \hat { \boldsymbol { \beta } } } ,$ , outlined above. 

To summarise our findings from estimating the line of best fit, the parameter estimates and associated standard errors can be summarised as follows: 

$$
\begin{array}{c c} Y _ {i} = 0. 8 9 & - 3. 7 0 X _ {i} \\ (1. 8 6) & (0. 7 7) \\ t = - 0. 4 8 & t = 4. 8 1 \end{array}\tag{2.13}
$$

with the standard errors in brackets. 

These results confirm the findings from our visual inspection of the scatter plot and from our estimate of the parameters of the line of best fit. There is an assocation between rising poverty and falling GDP growth which is statistically significantly different from zero at a 5% significance level. 

## $R ^ { 2 }$ and goodness of fit

In looking at the overall performance of our OLS estimation we need to ask: how well does our regression line fit the observed data? To capture this, we can calculate the coefficient of determination – a measure of the goodness of fit (i.e. the extent to which the estimated line neatly fits the pairs of observations on Y and X for each country). This is easy to do using the transformations summarised in Table 2.3. 

The first step in finding $R ^ { 2 }$ is to calculate the difference between the observed values for each country (Y ) and the estimates of $\hat { Y } _ { i }$ (i.e. the fitted or predicted values for the poverty variable). This vertical distance between the observed and predicted values gives the sample residual. The sum of these residuals across the sample is the residual sum ofsquares (RSS). We can get the predictions for Y for each country taking advantage of our new information that: 

$$
\hat {Y} _ {i} = 0. 8 9 - 3. 7 0 \mathrm{X} _ {\mathrm{i}}\tag{2.14}
$$

For example the predicted values of Y for various countries in the sample can be calculated as follows: 

$$
\hat {Y} _ {\mathrm{Lao}} = 0. 8 9 + (- 3. 7 0 \times 3. 5) = - 1 2. 1
$$

$$
\hat {Y} _ {\text { Bangladesh }} = 0. 8 9 + (- 3. 7 0 \times 3. 3) = - 1 1. 3
$$

$$
\hat {Y} _ {\mathrm{Uganda}} = 0. 8 9 + (- 3. 7 0 \times 3. 1) = - 1 0. 6\tag{2.15}
$$

and so on. 

The predicted values for all the countries in this sample are listed in column 1 ofTable 2.3, and the extent to which they differ from the observed value ofY is shown in column 6. As we would expect from our initial graph, because our sample captures such a diverse range of experiences, our regression estimates are very different from the actual/observed $Y _ { i }$ in some countries. This was particularly apparent in the case of Sierra Leone, Malawi, Lesotho, Central African Republic and Gambia. But although these may seem like big errors, OLS methodology is already giving us the smallest error possible consistent with identifying a line that fits all the data points as neatly as possible. 

To measure goodness of fit, we look at the total variability in Y and assess how much of this is ‘explained’ by the model and how much is caught in the residuals. This variability is measured using sums of squared deviations. To calculate the total sum of squares (TSS), we measure the deviation of the observed value from the mean $Y - { \bar { Y _ { i } } }$ , square these and then sum across all observations to give $\mathrm { T S S } = 5 5 4 0 . 5$ . These calculations are shown in columns 2 and 3 of Table 2.3. Similarly, as shown in columns 4 and 5, for the explained sum of squares (ESS), we measure the deviations between the predicted values $\hat { Y } _ { i }$ and the overall mean ${ \bar { Y } } _ { i { \mathrm { : } } }$ then we square these and sum across all observations to give $\mathrm { E S S } = 2 4 5 4 . 2$ . Finally, as shown in columns 6 and 7, we measure the residual sum of squares (RSS) by calculating the residual $( Y _ { i } - { \hat { Y } } _ { i } )$ squaring and summing this to give $\mathrm { R S S } = 3 0 8 2 . 8$ 

$R ^ { 2 }$ is measured by calculating the ratio of explained sum of squares (ESS) to total sum of squares (TSS). This formula can be applied here as follows: 

$$
R ^ {2} = \frac {E S S}{T S S} = \frac {\sum (\hat {Y} - \bar {Y}) ^ {2}}{\sum (Y _ {i} - \bar {Y}) ^ {2}} = \frac {2 4 5 4 . 2}{5 5 4 0 . 5} = 0. 4 4\tag{2.16}
$$

In simple regression analysis (SRA) the coefficient of determination is also easy to calculate using the correlation coefficient because it is just $r ^ { 2 } ;$ , i.e. the square of the correlation coefficient. We’ve already calculated $r = - 0 . 6 6$ so $r ^ { 2 } = 0 . 4 4$ . This verifies our calculation from above, i.e. $R ^ { 2 }$ is the square of the correlation coefficient $\left( r = - 0 . 6 6 \right)$ 

But this simple relationship between $r ^ { 2 }$ and $R ^ { 2 }$ holds only for SRA. In multiple regression analysis (MRA), i.e. when two or more explanatory variables are involved, measuring goodness of fit is more complicated than simply squaring the correlation coefficient. But the formula in Equation (2.16) can be applied in MRA too because it abstracts from the contribution of individual explanatory variables and instead focusses on the overall relationship between predicted and observed values of a single dependent variable. Measuring goodness of fit in MRA is explained in more detail in Chapter 5. 

As shown above, our calculation of the coefficient of determination indicates that 44% of the variability in poverty changes can be captured by the variability in GDP growth. So the results suggest a good fit between growing GDP and falling poverty. But with econometrics it is important to think of caveats, conditions and qualifying factors. This result may be misleading if it indirectly reflects other factors relevant to poverty changes, such as whether the country is a democracy or not; whether it has social policies aimed at the poor, and so on. If we leave these factors out of our simple regression we could generate omitted variable bias (a problem explained in Chapter 8). Many economic factors are affected by more than one explanatory variable and for this reason a lot of econometric analysis does tend to focus on MRA. 


Table 2.3 Measuring the sums of squares to estimate $R ^ { 2 }$


<table><tr><td rowspan="2"></td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>7</td></tr><tr><td><eq>\hat{Y}_{i}</eq></td><td><eq>(Y_{i}-\bar{Y})</eq></td><td><eq>(Y_{i}-\bar{Y})^{2}</eq></td><td><eq>(\hat{Y}_{i}-\bar{Y})</eq></td><td><eq>(\hat{Y}_{i}-\bar{Y})^{2}</eq></td><td><eq>(Y_{i}-\hat{Y}_{i})</eq></td><td><eq>(Y_{i}-\hat{Y}_{i})^{2}</eq></td></tr><tr><td>Lao PDR</td><td>-12.1</td><td>-3.6</td><td>13.2</td><td>-13.7</td><td>186.6</td><td>10.1</td><td>101.2</td></tr><tr><td>Bangladesh</td><td>-11.3</td><td>-5.0</td><td>25.3</td><td>-12.9</td><td>166.9</td><td>7.9</td><td>62.7</td></tr><tr><td>Uganda</td><td>-10.6</td><td>-17.7</td><td>314.4</td><td>-12.2</td><td>148.4</td><td>-5.5</td><td>30.5</td></tr><tr><td>Bhutan</td><td>-10.2</td><td>-20.8</td><td>433.9</td><td>-11.8</td><td>139.5</td><td>-9.0</td><td>80.8</td></tr><tr><td>Cape Verde</td><td>-9.8</td><td>-7.9</td><td>62.9</td><td>-11.4</td><td>130.9</td><td>3.5</td><td>12.5</td></tr><tr><td>Mozambique</td><td>-8.4</td><td>-5.2</td><td>27.4</td><td>-10.0</td><td>99.2</td><td>4.8</td><td>22.7</td></tr><tr><td>Nepal</td><td>-8.0</td><td>-15.9</td><td>253.8</td><td>-9.6</td><td>92.0</td><td>-6.3</td><td>39.8</td></tr><tr><td>Solomon Is</td><td>-4.3</td><td>-5.7</td><td>32.8</td><td>-5.9</td><td>34.7</td><td>0.2</td><td>0.0</td></tr><tr><td>Benin</td><td>-2.8</td><td>-7.7</td><td>59.8</td><td>-4.4</td><td>19.4</td><td>-3.3</td><td>10.8</td></tr><tr><td>Malawi</td><td>-2.4</td><td>-22.0</td><td>485.3</td><td>-4.0</td><td>16.3</td><td>-18.0</td><td>322.6</td></tr><tr><td>Ethiopia</td><td>-2.1</td><td>-2.8</td><td>8.0</td><td>-3.7</td><td>13.5</td><td>0.9</td><td>0.8</td></tr><tr><td>Lesotho</td><td>-1.7</td><td>20.7</td><td>427.2</td><td>-3.3</td><td>10.9</td><td>24.0</td><td>576.0</td></tr><tr><td>Burkina Faso</td><td>-0.6</td><td>-8.1</td><td>66.1</td><td>-2.2</td><td>4.8</td><td>-5.9</td><td>34.9</td></tr><tr><td>Mali</td><td>0.5</td><td>7.1</td><td>50.0</td><td>-1.1</td><td>1.2</td><td>8.2</td><td>66.9</td></tr><tr><td>Senegal</td><td>0.9</td><td>-0.8</td><td>0.7</td><td>-0.7</td><td>0.5</td><td>-0.1</td><td>0.0</td></tr><tr><td>Central African Republic</td><td>3.9</td><td>21.7</td><td>469.6</td><td>2.3</td><td>5.1</td><td>19.5</td><td>378.3</td></tr><tr><td>Chad</td><td>5.7</td><td>0.9</td><td>0.8</td><td>4.1</td><td>16.8</td><td>-3.2</td><td>10.2</td></tr><tr><td>Vanuatu</td><td>5.7</td><td>1.9</td><td>3.5</td><td>4.1</td><td>16.8</td><td>-2.2</td><td>4.8</td></tr><tr><td>Guinea-Bissau</td><td>6.8</td><td>23.4</td><td>546.2</td><td>5.2</td><td>27.1</td><td>18.2</td><td>330.9</td></tr><tr><td>Madagascar</td><td>7.6</td><td>2.9</td><td>8.2</td><td>6.0</td><td>35.4</td><td>-3.1</td><td>9.3</td></tr><tr><td>Comoros</td><td>13.8</td><td>10.2</td><td>103.4</td><td>12.2</td><td>149.8</td><td>-2.0</td><td>4.2</td></tr><tr><td>Angola</td><td>15.0</td><td>-0.1</td><td>0.0</td><td>13.4</td><td>178.2</td><td>-13.5</td><td>180.9</td></tr><tr><td>Mauritania</td><td>-5.0</td><td>-7.8</td><td>61.3</td><td>-6.6</td><td>44.0</td><td>-1.2</td><td>1.4</td></tr><tr><td>Guinea</td><td>-2.1</td><td>-9.0</td><td>81.5</td><td>-3.7</td><td>13.5</td><td>-5.3</td><td>28.4</td></tr><tr><td>Gambia</td><td>4.2</td><td>-17.9</td><td>321.5</td><td>2.6</td><td>6.9</td><td>-20.5</td><td>421.1</td></tr><tr><td>Togo</td><td>8.3</td><td>-3.3</td><td>11.1</td><td>6.7</td><td>44.8</td><td>-10.0</td><td>99.8</td></tr><tr><td>Niger</td><td>8.3</td><td>3.5</td><td>12.0</td><td>6.7</td><td>44.8</td><td>-3.2</td><td>10.2</td></tr><tr><td>Rwanda</td><td>11.6</td><td>11.5</td><td>131.6</td><td>10.0</td><td>100.4</td><td>1.5</td><td>2.2</td></tr><tr><td>Burundi</td><td>13.5</td><td>9.4</td><td>87.8</td><td>11.9</td><td>140.9</td><td>-2.5</td><td>6.1</td></tr><tr><td>Haiti</td><td>13.8</td><td>13.3</td><td>176.1</td><td>12.2</td><td>149.8</td><td>1.1</td><td>1.1</td></tr><tr><td>Sierra Leone</td><td>22.0</td><td>35.6</td><td>1265.2</td><td>20.4</td><td>415.3</td><td>15.2</td><td>231.6</td></tr><tr><td>Sums of Squares</td><td></td><td colspan="2">TSS = 5540.5</td><td colspan="2">ESS = 2454.2</td><td colspan="2">RSS = 3082.8</td></tr></table>

This chapter focusses on calculation by hand but most spreadsheet and econometric packages (including Excel and EViews) will perform the necessary calculations with a click of a mouse, as will be shown in the following chapters. Some of the output produced by these packages will include the predicted values for the dependent variable as well as the residuals. Both can also be generated in graphical form. Analysis of the residuals and/or predicted values is an important step in assessing whether or not OLS is working properly; this information can be used to test whether or not it is valid to make the assumptions about BLUEness outlined in Chapter 1. The practical aspects testing for BLUEness are analysed in subsequent chapters of this book. 

Overall, we have shown some empirical support for the ‘trickle-down assertion that rapid growth is associated with poverty reduction. But our evidence does not prove that the relationship is robust and we’d be well advised to explore further. More detailed evidence could be found perhaps by examining a single country’s experience over time, using time-series data for the last 20 years or more. (Not least, we might want to explore some of the confounding countries, such as Angola, which had extremely high increases in investment and exports, but negative growth and minimal improvement in poverty.) We might also develop richer measurements ofpoverty, for example incorporating qualitative aspects of inequality and participation, as well as daily consumption. (See Annex 2.1 for some ideas about alternative poverty measures.) Perhaps our sample is not representative in which case a larger sample set might prove to be more representative of LDCs as a whole. Most importantly, we should allow for the possibility that our theory is flawed, and go back to the drawing board! 

## 2.4 Implications and conclusions

Our results have supported the trickle-down hypothesis: growth does seem to be associated with falling poverty. But what are the policy implications? One obvious way to reduce world poverty would be for the rich to make an immense lump-sum payment to the poor to enable them to invest and grow. Such a transfer would certainly change the income (and possibly wealth) distribution profile. However it is unlikely to be politically acceptable, to the rich at least; and moreover it would not necessarily guarantee sustainable improvements in the long run either. Philanthropy and aid is ofcourse vital to developing countries, especially for health, education and other forms of public investment. But few, if any, would claim that aid alone will forge a lasting path out of poverty. Aid does not ensure that poor societies have the tools, the technologies and the resources that will help them to create sustainable economic futures (UNCTAD, 2008); and there is no guarantee that the rich will continue to feel philanthropic, or even to be as productive, in the long run. 

As you might expect, there is no monopoly of prescriptions to reduce poverty and in fact there are a myriad of theories from which to choose. This is not surprising, given that poverty is a multi-faceted problem and there will be more than one way of contributing to its reduction. However, one widely held view is that sustainable poverty reduction requires a combination of massive public investment alongside private sector investment, in order to create jobs and income-generating opportunities that can help the poor to become masters of their own destinies. These arguments became more pressing in 2008, in debates about how to cope with global recession. Enabling all countries easy access to global export markets can be encouraged via fair trade rules. These points are for the most part widely accepted. The contention lies rather in the details: what is the sequencing ofevents required to get economies moving? How can public and private investment be harnessed most effectively together? What priorities are most important; what constitutes fair trade? Econometric analysis can give us small clues about past patterns and whilst statistical evidence cannot provide answers to these complex questions, it can at least give us a starting point in enhancing our understanding of the links between variables. 

## 2.5 Further reading

## Books



Addison, A., Hulme, D. and Kanbur, R. (2008) Poverty Dynamics, Oxford: Oxford University Press. 





Lipsey, R. and Chrystal, A. (2007) Economics (11th edition), Oxford: Oxford University Press. Chapters 33–34. 





Sen, A. (1981) Poverty and Famines, Oxford: Oxford University Press. 





Thirlwall, A. P. (2005) Growth and development (8th edition), London: Macmillan. Chapters 1, 2 and 16. 



## Academic articles and working papers



Asian Development Bank (ADB) (2008), ‘Special chapter: Comparing poverty across countries: the role of purchasing power parities’, in Key Indicators for Asia and the Pacific 2008, Manila: ADB, pp. 3–54. 





Atkinson, A. B. (1987) ‘On the measurement of poverty’, Econometrica vol. 55, no. 4, 749–64. 





Chen, S. and Ravallion, M. (2000) How Did the World’s Poor Fare in the 1990s, Washington: World Bank. 





Collier, P. and Dollar, D. (2001) ‘Can the world cut poverty in half? How policy reform and effective aid can meet International Development Goals, World Development, vol. 29, no. 11, 1727–802. 





Mankiw, G., Romer, D. and Weil, D. (1992) A Contribution to the Empirics of Economic Growth, NBER Working Paper, No. 3541. 





Ravallion, M., Chen, S. and Sangraula, P. (2008), A Dollar a Day Revisited, World Bank Policy Research Working Paper No. 4620, Washington: World Bank. 





Rodrik, D. (1999) The New Global Economy, Making Openness Work, Policy Essay No. 24, Overseas Development Council, Washington D.C. 





Solow, R. (1956) ‘A contribution to the theory of economic growth’, Quarterly Journal of Economics, vol. 70, 65–94. 





Swan, T. (1956) ‘Economic growth and capital accumulation’, Economic Record, vol. 32, no. 2, 334–61. 



## Policy reports

UN Millennium Development Goals Report 2007, Geneva: United Nations. 

UNCTAD (2008) Least Developed Countries Report, Geneva and New York: United Nations. UNDP (annual), Human Development Report, Geneva: United Nations Development Program. World Bank (annual), World Development Report, Washington: World Bank Group. 

## 2.6 Chapter exercises

1. Using the data provided in Annex 2.2 – Table 2.6: 

(a) Assess the impact on GDP growth of export orientation by analysing the statistical associations between these variables. 

(b) Using your calculator, estimate a line of best fit and discuss your findings. 

(c) What are the implications of your findings for economic development policies? 

2. Using the data provided in Annex 2.2 – Table 2.6: 

(a) Construct scatter plots of the change in poverty against 

i. growth in GDP per capita 

ii. share of exports in GDP 

iii. rate of growth in gross capital formation. 

(b) Construct a matrix of correlation coefficients to show the associations between change in poverty, growth in GDP per capita, share ofexports in GDP and rate of growth in gross capital formation. 

(c) What are some theoretical and statistical implications of the correlations between these variables that should be kept in mind when devising policies to reduce poverty? 

## Annex 2.1 – Data focus: Quantitative and qualitative measurements of poverty

Sound measurements of poverty are important if we care about who is poor, for example whether the incidence is mostly in the young or the old; in racial minorities; women more than men; or those living in particular regions. We may be concerned that poverty is path-dependent in the sense that poor children are more likely to become poor adults, and so on. Another reason is to assess the progress of anti-poverty strategies and on these grounds alone poverty measurement is likely to become a particularly topical subject over the next decade, given the targets contained in the MDGs. As explained at the beginning of this chapter, the first of the eight MDGs is to eradicate extreme poverty. Other goals and targets, which are also for the most part poverty related, include reducing hunger, achieving universal primary education, and improving health. As donor countries and NGOs are committing billions of dollars and effort to achieving these goals – not to mention being genuinely concerned about human suffering – the way poverty is measured will become increasingly important. Table 2.4 shows an example of a MDG for which the target can be measured using both monetary and qualitative/non-monetary indicators of poverty. 

Each type of indicator will have advantages and disadvantages, some of which are described below. 

## Monetary indicators

Monetary indicators of poverty are usually based around a poverty line, expressed in US dollars or national currency. This describes a critical threshold below which one cannot have a minimum nutritionally adequate diet, or essential non-food requirements (such as housing). In developing countries, the bundle of goods and services that comprises these minimum requirements is derived using a variety of methods, including an approach based on defining basic human needs, or an approach based on a minimum level of‘food energy’. Once the bundle has been established, it is given a monetary value. 


Table 2.4 A development target and its indicators


<table><tr><td>MDG Target 1 → Eradicate extreme poverty and hunger</td><td>Indicators of progress</td></tr><tr><td>Between 1990 and 2015, halve the proportion of people whose income is less than $1/day.</td><td>1. Proportion of population below $1 (PPP) a day.2. Poverty gap ratio (incidence × depth of poverty).3. Share of poorest quintile (20%) in national consumption.</td></tr></table>

The $1 a day per person poverty line used in this chapter is a commonly used international indicator introduced by the World Bank in 1990. Some researchers have adjusted this benchmark upwards e.g. a new international poverty line at $1.25 has been advocated by Ravallion, Chen and Sangraula (2008); and the Asian Development Bank has suggested a special Asian Poverty Line at about $1.35 a day (ADB, 2008) after surveys in a number of countries indicated that it was an appropriate level for both national and intercountry comparisons. (Later, an additional $2 benchmark line was also introduced; and typically in developed countries significantly higher benchmarks are used.) In order to know how many people live below the benchmark, household surveys are conducted in each country, asking questions about sources of income and spending patterns. (This is of course a simplification of issues. Readers interested in the properties and criteria that income-based poverty indices should meet could start with Atkinson (1987), for an excellent overview, and Chen and Ravallion (2000), Ravallion, Chen and Sangraula (2008) for the World Bank view.) 

Limitations to this approach include the following: 

 Different households may have different preferences, so necessities for one household may be less important in another. 

 Different prices can be charged for the same goods: e.g. prices are cheaper in cities compared to rural areas; bulk purchases are cheaper than small ones.<sup>5</sup> 

 Average figures assume that resources are shared evenly within the household, but studies show that women and girls receive less of everything than boys and men. 

 Poverty levels can be overstated if non-monetary benefits are left out. 

 Inflation distorts things: poverty lines are not re-measured every year even if prices have changed by double-digits. 

 People may overstate their poverty if there are financial or other benefits arising from being identified as poor, or they may understate long-distant and forgotten sufferings. 

 A person surviving on $1.05 a day may be little better off than another living on $0.95, but the former may be categorised as ‘non-poor’. 

 A slight increase in the number of people living under the poverty line may slightly raise the percentage of people defined as “poor” while masking a dramatic worsening of conditions for the worst off. 

 Translating from $ prices to national currencies introduces problems. Between 1999 and 2000, South Africa saw the number of people living on less than $1 day fall from 24% to just 12%, while Turkmenistan went from 5% to 21%. But both changes were largely due to revised estimates of the purchasing power of the national currencies – where purchasing power is the measure of the value of a currency in terms of the amount of goods and services it can buy. 

Given these limitations, why are these indicators so widely used? Firstly, they are simple, easily interpreted, and readily incorporated into international, inter-regional or inter-temporal studies. They are intuitively appealing, and their eye-catching nature makes them a powerful tool for advocacy purposes – it is easier to imagine life on $1 a day than it is to conceptualise complex subjective indexes comprised of many different components. 

Secondly, the information is relatively easy to obtain. Even the poorest countries regularly conduct household and income surveys, so the data exists. Finally, the use of monetary measures enables comparison with other monetary variables, such as income, GDP, or foreign aid flows. However, given their limitations, readers will not be surprised to know there is an ongoing search for new and better indicators. 

## Non-monetary indicators

The Human Poverty Index (HPI), developed in 1977 by the UNDP, captures poverty not just in terms of lack of income but in a much broader way, as being the denial of a person’s capabilities and opportunities in life. It draws heavily on the conceptual framework of Amartya Sen, bringing together in a composite index a number of the various features of deprivation that characterise the lives of the poor. The index is made up of three components: 

i. longevity – the percentage of people who do not live to 40 years 

ii. knowledge deprivation – the percentage of people who are illiterate 


Table 2.5 Different indicators reveal a different picture


<table><tr><td>Country</td><td>% living on $1 day</td><td>% living on $2 day</td><td>HPI index</td><td>GDP $/person</td></tr><tr><td>Venezuela</td><td>15</td><td>32</td><td>11</td><td>5,380</td></tr><tr><td>Columbia</td><td>8.2</td><td>22.6</td><td>10</td><td>6,370</td></tr><tr><td>Philippines</td><td>14.6</td><td>46.4</td><td>28</td><td>4,170</td></tr><tr><td>Peru</td><td>18.1</td><td>37.7</td><td>23</td><td>5,010</td></tr><tr><td>China</td><td>16.6</td><td>46.7</td><td>24</td><td>4,580</td></tr><tr><td>South Africa</td><td>7.1</td><td>23.8</td><td>52</td><td>10,070</td></tr><tr><td>India</td><td>34.7</td><td>79.9</td><td>48</td><td>2,670</td></tr><tr><td>Zimbabwe</td><td>36</td><td>64.2</td><td>91</td><td>2,400</td></tr><tr><td>Ethiopia</td><td>37.9</td><td>78.4</td><td>89</td><td>780</td></tr><tr><td>Mali</td><td>72.8</td><td>90.6</td><td>93</td><td>930</td></tr></table>


Source: UNDP, Human Development Report 2004. 


iii. deprivations in the standard ofliving, measured as: 

(a) the percentage of people without access to health services, 

(b) the percentage without guaranteed access to safe water and 

(c) the percentage of malnourished children under the age of five. There are other non-monetary indicators of development, for example the Human Development Index (HDI). The advantage of the HPI over indicators such as the HDI<sup>6</sup> is that it focusses squarely on the experience of poverty, and does not take into account monetary variables at all. 

To illustrate the fact that one measure will rarely capture the full picture, Table 2.5 summarises some data on a range of different countries and indicators. This shows, for example, that South Africa has high GDP per person compared to a number of other developing countries (at $10,070). 

However ‘GDP per capita’ is simply a measure of total GDP divided by the population – it does not mean that wealth is shared equally. In fact, despite its high GDP per capita, South Africa scored worse in terms ofthe HPI than China, Peru, Philippines, Columbia and Venezuela. On the other hand, with the exception of Columbia, South Africa had a smaller proportion of people living on less than $2 and $1 per day. This could reflect the fact that South Africa offers targeted income support to its very poorest (through for example its policy of paying a pension to all elderly people) but nonetheless, South Africa performs less well on broader targets such as literacy, longevity and access to water. 

## Annex 2.2 – Raw data


Table 2.6 Change in poverty, exports of goods and services, and investment


<table><tr><td rowspan="2"></td><td>1</td><td>2</td><td>3</td><td>4</td></tr><tr><td>% change in proportion of population living on $1/day</td><td>Annual average GDP growth per capita</td><td>% change exports</td><td>Investment: % change GCF</td></tr><tr><td>Lao PDR</td><td>-2</td><td>3.5</td><td>19.8</td><td>15</td></tr><tr><td>Bangladesh</td><td>-3.4</td><td>3.3</td><td>7.2</td><td>4.6</td></tr><tr><td>Uganda</td><td>-16.1</td><td>3.1</td><td>3.6</td><td>5.3</td></tr><tr><td>Bhutan</td><td>-19.2</td><td>3</td><td>5.1</td><td>15.3</td></tr><tr><td>Cape Verde</td><td>-6.3</td><td>2.9</td><td>9.1</td><td>12.6</td></tr><tr><td>Mozambique</td><td>-3.6</td><td>2.5</td><td>3.4</td><td>11.1</td></tr><tr><td>Nepal</td><td>-14.3</td><td>2.4</td><td>12.7</td><td>2.8</td></tr><tr><td>Solomon Islands</td><td>-4.1</td><td>1.4</td><td>18.2</td><td>-</td></tr><tr><td>Benin</td><td>-6.1</td><td>1</td><td>2.6</td><td>4.2</td></tr><tr><td>Malawi</td><td>-20.4</td><td>0.9</td><td>4.3</td><td>-5.4</td></tr><tr><td>Ethiopia</td><td>-1.2</td><td>0.8</td><td>6.6</td><td>1.6</td></tr><tr><td>Lesotho</td><td>22.3</td><td>0.7</td><td>9.5</td><td>6.1</td></tr><tr><td>Burkina Faso</td><td>-6.5</td><td>0.4</td><td>1.5</td><td>7.5</td></tr><tr><td>Mali</td><td>8.7</td><td>0.1</td><td>8.6</td><td>-0.4</td></tr><tr><td>Senegal</td><td>0.8</td><td>0</td><td>8.7</td><td>6.2</td></tr><tr><td>Central African Republic</td><td>23.3</td><td>-0.8</td><td>1.4</td><td>0.9</td></tr><tr><td>Chad</td><td>2.5</td><td>-1.3</td><td>3.5</td><td>5.8</td></tr><tr><td>Vanuatu</td><td>3.5</td><td>-1.3</td><td>15.8</td><td>-0.7</td></tr><tr><td>Guinea-Bissau</td><td>25</td><td>-1.6</td><td>9.8</td><td>-22.6</td></tr><tr><td>Madagascar</td><td>4.5</td><td>-1.8</td><td>5.6</td><td>0.2</td></tr><tr><td>Comoros</td><td>11.8</td><td>-3.5</td><td>7.5</td><td>-5.9</td></tr><tr><td>Angola</td><td>1.5</td><td>-3.8</td><td>23.6</td><td>10.8</td></tr><tr><td>Mauritania</td><td>-6.2</td><td>1.6</td><td>-10.5</td><td>-6.8</td></tr><tr><td>Guinea</td><td>-7.4</td><td>0.8</td><td>-9.1</td><td>1.2</td></tr><tr><td>Gambia</td><td>-16.3</td><td>-0.9</td><td>-2.9</td><td>-0.2</td></tr><tr><td>Togo</td><td>-1.7</td><td>-2</td><td>-9.8</td><td>-2.7</td></tr><tr><td>Niger</td><td>5.1</td><td>-2</td><td>-1.9</td><td>-4.1</td></tr><tr><td>Rwanda</td><td>13.1</td><td>-2.9</td><td>-0.5</td><td>0.5</td></tr><tr><td>Burundi</td><td>11</td><td>-3.4</td><td>-1.7</td><td>-9.5</td></tr><tr><td>Haiti</td><td>14.9</td><td>-3.5</td><td>-4</td><td>-3.3</td></tr><tr><td>Sierra Leone</td><td>37.2</td><td>-5.7</td><td>-2.2</td><td>-5.8</td></tr><tr><td>Minimum</td><td>-20.4</td><td>-5.7</td><td>-10.5</td><td>-22.6</td></tr><tr><td>Maximum</td><td>37.2</td><td>3.5</td><td>23.6</td><td>15.3</td></tr><tr><td>Mean</td><td>1.63</td><td>-0.20</td><td>4.7</td><td>1.6</td></tr></table>

# Using logs and estimating elasticities Demand for air travel

Economic issues include: 

 Inverse demand curves 

 Elasticities 

 Income and substitution effects 

 Normal, inferior and Giffen goods 

Econometric issues include: 

 Model specification: using logs to estimate elasticities 

 Running regressions using Excel 

 Hypothesis testing: one-tailed t tests 

Data issues include: 

 Data constraints 

 Proxy variables 

## 3.1 The issue

If you were the manager of the London Underground or American Airlines would you raise ticket prices, or drop them? Which strategy would maximise your firm’s profits? The ‘law of demand’ states that if prices are lowered then there will be rises in demand. But this doesn’t necessarily mean that a firm should just lower prices if it wants to boost revenue. Other effects operate too and the net result will depend on how sensitive consumers are to changes in price. If for some reason consumers are determined to have only a certain amount of a particular good or service then lowering prices may make little difference to the amount demanded and so a firm’s revenues might fall because they are selling similar quantities but at lower prices. For example, if you manage an airline and your consumers don’t care much about price; if they are not motivated to travel more even when flights are cheaper, then total revenues would fall, perhaps so much that costs could not be covered (and you would probably be looking for a new career). The question of pricing is therefore critical – whether one is a private firm trying to maximise profits, or a government agency trying to provide public transport. 

But some producers have more control over prices than others. For producers of tomatoes, wheat or other goods and services for which there are many sellers and buyers: products are fairly homogeneous, and markets more closely approximate perfect competition. In these markets, each producer must set prices no higher than anyone else’s, or they will lose their customers. However when firms have a degree of monopoly power the question of what price to charge, and to whom, is critical. For the transport industries, there may be limited competition – for example the London Underground competes only against other forms of transport; there is no other underground train service in London and so if buses are not good substitutes for tube trains, then London Underground will have a lot of control over the price. But they will still need to judge pricing decisions carefully. If prices are too low, they will fail to cover costs and may go bust, particularly if the government is unwilling to bail them out! 

In this chapter, we examine these issues using the example of transport pricing in the airlines industry; we introduce the theoretical concepts of an ‘inverse’ demand curve, income/substitution effects and elasticities; and we show how econometric analysis can be used empirically to model the price elasticity of demand for air travel. 

## 3.2 The theory

For our analysis of air travel, we expect consumers to be price-responsive; we expect the demand for air travel to rise as prices fall, either because more people buy flights when prices are lower, or because the same people fly further and more often when prices are lower. 

In understanding more deeply why quantity demanded ofany good usually rises as prices fall, we need to make distinctions between effects that are subtle. When a price changes, there are two effects: the substitution effect and the income effect. 

The substitution effect captures the way that a consumer alters his or her purchasing decisions on the basis of the change in relative price (i.e. one good’s price in comparison with other goods). For example, as airline travel becomes relatively cheaper compared to other goods and services, we expect consumers to substitute their purchases towards more airline travel, and away from other goods and services. 

Price changes will also have knock-on income effects. Lowering the price of one good or service will lead to a rise in effective income or purchasing power. For example, if we have an income of £100 per week and we want to buy a plane ticket costing £20, we’ll have £80 left to buy other things; but if there’s a 50% cut in plane fares and we only have to spend £10 on our plane fare, then we will have £90 left to buy other things. Assuming that the prices of other things remain unchanged, we’ll be able to afford more ofeverything. We would be able to have the same ‘basket’ of the other goods that we had before but with some extra income to spend because air travel is cheaper. If relative prices had not changed, the only way this would have been possible would have been via a rise in income. So even though our take-home pay of £100 hasn’t changed, the purchasing power of our income has changed via this income effect. 

But the impact of the income effect is more complicated than that of the substitution effect. We don’t necessarily increase our demand for everything as our incomes rise; there are some things we prefer to stop consuming as our purchasing power increases; for example perhaps we would be able to afford to give up eating bread, or potatoes or tripe. This is the difference between a normal good and an inferior good. For normal goods quantity demanded rises as income rises. By comparison, for inferior goods, quantity demanded falls as income rises – if people tend to eat less bread when income rises because they can afford cake, then bread is an inferior good. 

In assessing the net impact of price changes we need to think carefully about the balance of the income effect and substitution effect, keeping in mind whether we are considering normal goods or inferior goods. For normal goods, the income and substitution effects will reinforce each other because they will move in the same direction. A fall in the price ofsomething will make it relatively cheaper and so we will demand more of it. Unsurprisingly, there will be a negative substitution effect: prices decrease, demand rises. The falling price will also release income increasing our ability to consume and our demand for a normal good will increase with this overall increase in purchasing power. So there will be a negative income effect too: prices fall, effective purchasing power of income rises and demand rises too. Overall, there will be an unequivocal increase in the quantity demanded. 

But for inferior goods, the net impact of the substitution effect and income effect is more complex. The substitution effect will work in exactly the same way as for a normal good, i.e. a fall in the relative price ofa good will encourage increasing demand for that good. Again, there will be a negative substitution effect. But the freeing up of income allowed by the fall in price will discourage consumption of inferior goods: the income effect on its own will encourage falling demand and there will be a positive relationship: the income effect will generate a tendency for decreased demand. This creates a trade-off because the income effect operates in the opposite direction to the substitution effect; and the precise outcome will depend on the relative magnitude of these separate effects. Ifthe income effect is large enough then it may entirely cancel out the substitution effect. 

How likely is it that the income effect will overwhelm the substitution effect? Most goods are ordinary goods: with ordinary goods, demand increases as prices fall. As explained above, all normal goods are ordinary goods because there is no trade-offbetween the income and substitution effects for normal goods. But there are two sorts ofinferior goods: ordinary goods and Giffen goods. For ordinary inferior goods the perverse income effect explained in the last paragraph is not sufficient to overwhelm the substitution effect. 

Giffen goods are an extreme type of inferior goods for which the income effect is enough to overwhelm the substitution effect and so a fall in prices is associated with a fall in demand. To explain why this happens: the price fall makes the Giffen good relatively cheaper so demand rises via the substitution effect. But this effect is not as strong as the income effect; via the income effect the price fall releases purchasing power and effective income allowing the consumer to buy a lot less of the inferior good. Overall, the perverse income effect has overwhelmed the substitution effect. So for Giffen goods: a fall in price leads to decreases in the quantity demanded first, because the income and subsitution effects are operating in opposite directions and second, because the income effect is larger than the substitution effect. Examples of Giffen goods are rare but one often-cited example is potatoes during the Irish famine: as the price ofpotatoes rose, purchasing power fell and demand for potatoes rose because consumers could no longer afford more expensive staples. 

In Box 3.1 the different types of goods are illustrated to emphasise the difference between normal goods, inferior ordinary goods and Giffen goods. 

It is not always easy to predict the net effect of the substitution effect and income effect in advance. Applying these concepts to our chapter example, the airline industry: the intensity of the effects will vary from case to case, depending on the reason people are travelling, and whether distances travelled are short or long. But here we will keep things simple by assuming that air travel is a normal good: people will want to consume more of it when their income rises. Price falls will release purchasing power and, because we are assuming that air travel is a normal good, this positive income will reinforce the substitution effect. Unequivocally, price falls will lead to increases in demand. So overall we expect that air travel will have a conventional looking downward sloping demand curve. 

<table><tr><td>Substitution effect (SE)</td><td>Income effect (IE)</td><td>IE vs SE</td><td>Net effect</td></tr><tr><td>Normal goods<eq>\downarrow P \rightarrow \uparrow Q</eq>→ All normal goods are ordinaryInferior goods:Ordinary inferior<eq>\downarrow P \rightarrow \uparrow \uparrow Q</eq>Giffen (inferior) goods<eq>\downarrow P \rightarrow \uparrow Q</eq></td><td><eq>\downarrow P \rightarrow \uparrow Q</eq><eq>\downarrow P \rightarrow \downarrow Q</eq><eq>\downarrow P \rightarrow \downarrow \downarrow Q</eq></td><td>IE reinforces SE</td><td><eq>\downarrow P \rightarrow \uparrow Q</eq><eq>\downarrow P \rightarrow \uparrow Q</eq><eq>\downarrow P \rightarrow \downarrow Q</eq><eq>\downarrow P \rightarrow \downarrow Q</eq></td></tr></table>

A downward sloping demand curve is called the inverse demand curve. Why? Mathematically, it is conventional to put the dependent variable on the vertical axis and the explanatory variable on the horizontal axis. Yet economists usually depict the relationship between price (P) and quantity demanded (Q) using (for ordinary goods) a downward sloping demand curve – with P on the vertical axis and Q on the horizontal axis, even though demand is the dependent variable. However, P is the dependent variable for supply relationships (i.e. all things being equal a rising price encourages increased production) so to make the demand function consistent with this, it must be mathematically inverted to give an ‘inverse’ demand curve with the dependent variable (Q) on the horizontal axis. 

Another issue to consider is the shape of our demand function. Mathematically, the shape of a demand curve will be determined by the elasticity of a consumer’s response to price changes. Elasticity is a very general concept. There are all sorts of elasticities in economics: the elasticity of output with respect to inputs of labour; the elasticity of imports and exports to currency fluctuations. And there are elasticities in other subjects (in fact the term elasticity has its origins in physics, which defines elasticity as the ability of a solid to recover its shape when an external force is removed). Here we will concentrate on price elasticities and in particular on two types of price elasticity: the own-price elasticity of demand, as explained in Box 3.2, and the cross-price elasticity of demand. 

The cross-price elasticity of demand is the change in quantity demanded for one good in response to a change in the price of another. If two goods or services, for example planes and trains, are close substitutes, then a fall in the price of trains will lead to a fall in demand for planes. In this case the formula for the cross price elasticity of demand will be: 

$$
\eta_ {\text { Planes,   Trains }} = \frac {\Delta Q _ {\text { Planes }}}{\Delta P _ {\text { Trains }}}. \frac {P _ {\text { Trains }}}{Q _ {\text { Planes }}}\tag{3.1}
$$

Price elasticities of demand will depend on the absolute and relative magnitudes of the income and substitution effects. Similarly, elasticities will also vary depending on whether a good is a necessity or a luxury. Demand for necessities (such as drinking water) is likely to be highly inelastic; demand for luxury goods tends to be relatively elastic. Certain types of travel (for example supersonic or zero gravity flights) are likely to be luxury goods. 

Elasticities also have implications for the revenue generated (or not) by a change in prices. Revenue is price paid multiplied by quantity sold. Ifthe ownprice elasticity is greater than 1, i.e. if demand is elastic, then a fall in price will lead to a greater proportionate rise in quantity demanded and so revenue will increase. Total revenues accrued to a firm facing this kind of demand will rise if they push down prices (assuming no changes to the firm’s costs). On the other hand, if the consumer response is inelastic, the rise in consumption will be relatively small in comparison with the falling price. And so total revenue will fall as prices fall. 

<table><tr><td colspan="3">Box 3.2 Own-price elasticities of demand</td></tr><tr><td colspan="3">The own-price elasticity of demand measures the relative sensitivity of demand to changes in price. It is measured as the percentage change in quantity demanded resulting from a given percentage change in price. For example, if a 1% increase in price leads to a 1.5% fall in quantity demanded, then the own-price elasticity is 1.5. This is an elastic response, i.e. the proportional change in quantity demanded is larger in absolute terms than the proportional change in price. If, on the other hand, the 1% rise in price had led to only a 0.5% reduction in quantity demanded, then this would be an inelastic response: the consumers&#x27; proportionate response in terms of quantity demanded is relatively small (in absolute terms) in comparison with the proportionate change in price.Mathematically, this means that the own price elasticity is defined as the ratio of percentage change in quantity demanded to percentage change in price:η = ΔQ/Q/ΔP/P = ΔQ/ΔP·P/Q(3.2)</td></tr><tr><td colspan="3">where P and Q represent the price and quantity demanded respectively and ΔQ and ΔP represent the change in quantity and price demanded.The various scenarios for own price elasticities are shown below:</td></tr><tr><td>Terminology</td><td>Numerical measure</td><td>Definition</td></tr><tr><td>Perfectly or completely inelastic</td><td>|η| = 0</td><td>Quantity demanded does not change as price changes.</td></tr><tr><td>Inelastic</td><td>0 &lt; |η| &lt; 1</td><td>Quantity demanded changes by a smaller percentage than the price.</td></tr><tr><td>Unit elasticity</td><td>|η| = 1</td><td>Quantity demanded changes by exactly the same percentage as the price.</td></tr><tr><td>Elastic</td><td>1 &lt; |η| &lt; ∞</td><td>Quantity demanded changes by a larger percentage than the price.</td></tr><tr><td>Perfectly or completely elastic</td><td>|η| → ∞</td><td>Consumers are prepared to buy all they can get at one price, but none at all at a different price.</td></tr><tr><td colspan="3">Practical examples of these measures of elasticity are shown in Box 3.4.</td></tr></table>

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/1cb3b6d74f674899c0a9f29e540e37406596a31016b6b7a5550fa2dc7badd1be.jpg)



Figure 3.1 Elasticity varies along a linear demand curve


What is the relationship between elasticities and inverse demand functions? As explained above, the formula for the own-price elasticity of demand is given by Equation (3.3): 

$$
\eta = \frac {\Delta Q}{\Delta P} \cdot \frac {P}{Q}\tag{3.3}
$$

What happens to this elasticity along a linear demand function, such as the one depicted in Figure 3.1? 

From Equation (3.2) you can see that the elasticity (η) will vary along a linear demand function. The slope of a line is constant i.e. $\Delta Q / \Delta P$ does not change along the line. But the ratio of price to quantity (P/Q) will vary along the line: at the top left of this line, the ratio P/Q will be relatively high and so η will be relatively large in absolute terms (i.e. elastic); in the bottom righthand corner P/Q will be relatively small and so $\eta$ will be too (i.e. the price elasticity of demand will be inelastic). 

In economic analysis we often want to concentrate on constant elasticity ofdemand functions. These take the following non-linear form: 

$$
Q = A P ^ {\eta}\tag{3.4}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/f112895fbda897d53078f1c1a0849d469b7ec9a39816ed2fe516b4866b0bf0a3.jpg)



Figure 3.2 Constant elasticity of demand curve: linear vs. logged scales


where η is the elasticity of demand. This type of demand function is depicted in Figure 3.2 – in the first panel using a linear scale. The elasticity is constant for this sort of function because, moving towards the bottom right, the slope of the curve will flatten and $\Delta P / \Delta Q$ will fall $( \mathrm { i } . \mathrm { e } . \ \Delta Q / \Delta P$ will rise) and, at the same time, P/Q will fall. Thus the changes in the slope are being balanced by changes in the price-quantity ratio and so the elasticity remains constant. 

Constant elasticity demand curves of the form (3.4) will exhibit a nonlinear, logarithmic relationship. We can capture this by taking the natural log of both sides of the equality from Equation (3.4): 

$$
\ln (Q) = \ln A + \eta \ln (P)\tag{3.5}
$$

So the plot of $\textit { p } \left( = \ln P \right)$ against $q \ ( = \ln Q )$ will be linear. This logged transformation of (3.2) is depicted in the second panel of Figure 3.2. (Also see Box 3.3 for a fuller explanation of the elasticities and the logarithmic functional form.) 

## Box 3.3 Logs and elasticities, model specification

As explained in Chapter 1, Ordinary Least Squares (OLS) is a linear estimation technique and therefore will only work properly if we can assume linearity in the parameters. This does not necessarily mean that non-linearity in the variables is a problem because we may be able to transform our model into a form that is linear in the parameters. We can do this for our example of air travel, as follows. 

Equation (3.4) shows a constant elasticity of demand function: 

$$
Q = A P ^ {\eta}\tag{3.4}
$$

Equation (3.4) is a non-linear function; it is not linear in the variables because, in its untransformed form, it is not an additive function; the various components are not being added together. Rather it is a multiplicative function in which the variables are being multiplied by each other. So what can we do? We can take natural logs, as we did to get Equation (3.5), and this specification is linear in the parameters: 

$$
\ln (Q) = \ln A + \eta \ln (P) \quad \rightarrow q _ {t} = a + \eta p _ {t}\tag{3.6}
$$

$$
\text { where } q = \ln (Q), p = \ln (P) \text { and } a = \ln (A)
$$

This sort of function can be estimated effectively using OLS because it is an additive function and so satisfies the Gauss–Markov assumption of linearity in the parameters. 

We can also show that the slope parameter on ln(P), i.e. η is the own-price elasticity of demand using a little bit of differential calculus. Following from Equation (3.1): 

$$
\eta = \frac {d Q}{d P} \cdot \frac {P}{Q}
$$

$$
\frac {d Q}{d P} = \eta A P ^ {\eta - 1} = \eta \frac {Q}{P} \text { because } A P ^ {\eta - 1} = \frac {Q}{P}
$$

$$
\mathrm{so} \frac {d Q}{d P} \cdot \frac {P}{Q} = \eta\tag{3.7}
$$

## Functional forms: lin-lin, log-log, log-lin or lin-log?

This illustrates the difference between lin-lin, log-log, log-lin and lin-log models. The model that we are using in Equation (3.6) is a log-log model or double-log model – we’ve logged both the dependent and explanatory variables. We explained that the slope parameter on ln(P), i.e. η is the own-price elasticity of demand. 

A lin-lin model is one in which the dependent and explanatory variables are not logged, i.e. are left in their linear form. 

Other forms of log relationships include semi-log models. There are two basic types of semi-log models: in log-lin models only the dependent variable is logged and the slope coefficient measures the relative change in Y for a given absolute change in X. This is often used when the explanatory variable is a time trend. For example, in the model ln $( Y ) = a + \beta t ,$ t is a deterministic time trend changing by one unit as each year passes, and the coefficient $\beta$ simply measures the rate of growth over a year. This sort of log-lin model is sometimes called the constant growth model. 

Another form is the lin-log model, where only the explanatory variable is logged. In this case the slope coefficient measures the absolute change in Yfor a relative change in X. 

Log-log, log-lin and lin-log forms are used frequently in applied economics because we are often interested in elasticities and proportional responses rather than absolute responses. For example as we’ve shown in this chapter, with a log-log model we are capturing an elasticity – the % change in one variable relative to the % change in another variable. With logged models, we can abstract from the units of measurement used and so we can interpret results more easily. Using logs can also help to moderate some econometric problems, e.g. heteroscedasticity, explored in Chapter 6. 

In our empirical section, we will illustrate how these exponential/logarithmic relationships can be used in practice when estimating the price elasticity of demand for air travel. This will illustrate some very important points about how correctly to specify an empirical model, particularly when, as in much of economics, you’re interested in unit-free elasticities of response rather than absolute responses. 

But before moving onto our own empirical analysis, we should conclude this section by examining existing evidence. In any research project it is useful to have a look at the methods and findings of other researchers and in Box 3.4 we summarise some empirical evidence relevant to estimating own-price elasticities of demand for air travel. 

## Box 3.4 Existing evidence shows heterogeneity in patterns of demand for air travel

Demand for any good or service depends on a variety of factors, including tastes, income, price and quality, the price of other goods, especially substitutes, and any number of other factors. We must assume that these other influences remain constant when estimating demand elasticity – which is more easily said than done in practice. One example is given by a recent Canadian government survey of 21 domestic and international air travel demand studies (Canadian Department of Finance 2003), see Table 3.1. This study separated the findings into six distinct market segments each of which were influenced by very different sets of non-price factors. For example, business travellers are less flexible about dates or routes than are leisure travellers; and long-haul business travellers do not have substitute options, such as going by car or train. 

As expected, this ‘meta’ study found that long-haul business travellers were much less responsive to price changes than all other types of consumers. This is evident not only in the average elasticity but also in the range of estimates. For long-haul international business travellers these range from + 0.19 (perhaps long-haul air travel is an inferior good for some business travellers if richer companies can afford video-conferencing facilities?) to –0.48, with a median of − 0.26. In contrast, the estimates for international leisure travellers ranged from –0.56 to –1.7, with a median of –1.04, and short-haul domestic leisure travellers, who could just as easily go by bus, car or train, were the most responsive to price changes. The lesson from this is that an airline wishing to boost its total revenues should seek means of raising prices for business travellers (particularly long-haul), and lowering them for holidaymakers (particularly short-haul). 

These on average negative estimates of the own-price elasticity of demand confirm that air travel is a normal (and therefore ordinary) good. Ranking these sample estimates against the continuum of definitions of elasticity shown below and including the sign, we see that business travel (both short haul and international) is inelastic, meaning that its elasticity was less than zero but greater than –1 $( - 1 < \eta < 0 )$ , i.e. the responsiveness of quantity demanded was less than the responsiveness of price. Demand in all the other market segments was elastic with respect to price, with estimates that were less than –1 but greater than (negative) infinity $( - \infty < \eta < - 1 )$ . We can show these estimates on the continuum of own-price elasticity of demand as follows: 


Table 3.1 Elastic demand from leisure travellers, inelastic from business


<table><tr><td>Market segment</td><td></td><td>Median own-price elasticity</td></tr><tr><td>Short-haul leisure</td><td>(SHL)</td><td>-1.52</td></tr><tr><td>Long-haul domestic business</td><td>(LHDB)</td><td>-1.15</td></tr><tr><td>Long-haul domestic leisure</td><td>(LHDL)</td><td>-1.10</td></tr><tr><td>Long-haul international leisure</td><td>(LHIL)</td><td>-1.04</td></tr><tr><td>Short-haul business</td><td>(SHB)</td><td>-0.70</td></tr><tr><td>Long-haul international business</td><td>(LHIB)</td><td>-0.26</td></tr></table>


Source: Derived from Department of Finance, Canada 2003. 


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/09e8dca7a67be454c3498ad42230eac37fdaa6f55e3da4a3decde90d1d44b843.jpg)


## 3.3 The data

In this chapter we want to investigate how consumers change their demand for air travel as the price of air travel changes and in this section we explain how we selected the data and some of the data constraints that we faced. 

## Broad trends

For our analysis we have used International Civil Aviation Organisation (ICAO) data on number of passengers worldwide travelling on scheduled national and international flights as a measure of demand and revenue per passenger km as a proxy for price, as shown in Table 3.2. (We will say more about proxies in the following section on data constraints.) 


Table 3.2 Data on aviation demand and revenue


<table><tr><td rowspan="2"></td><td colspan="2">International Civil Aviation Raw Data</td><td colspan="2">Data transformed into natural logs</td></tr><tr><td>Number of passengers (millions)</td><td>Revenue per passenger-km US cents</td><td>Number of passengers</td><td>Revenue per passenger-km</td></tr><tr><td>1991</td><td>1135</td><td>9.60</td><td>7.03</td><td>2.26</td></tr><tr><td>1992</td><td>1146</td><td>9.20</td><td>7.04</td><td>2.22</td></tr><tr><td>1993</td><td>1142</td><td>9.20</td><td>7.04</td><td>2.22</td></tr><tr><td>1994</td><td>1233</td><td>9.20</td><td>7.12</td><td>2.22</td></tr><tr><td>1995</td><td>1304</td><td>9.40</td><td>7.17</td><td>2.24</td></tr><tr><td>1996</td><td>1391</td><td>9.10</td><td>7.24</td><td>2.21</td></tr><tr><td>1997</td><td>1457</td><td>8.80</td><td>7.28</td><td>2.17</td></tr><tr><td>1998</td><td>1471</td><td>8.60</td><td>7.29</td><td>2.15</td></tr><tr><td>1999</td><td>1562</td><td>8.30</td><td>7.35</td><td>2.12</td></tr><tr><td>2000</td><td>1672</td><td>8.30</td><td>7.42</td><td>2.12</td></tr><tr><td>2001</td><td>1640</td><td>7.90</td><td>7.40</td><td>2.07</td></tr><tr><td>2002</td><td>1639</td><td>7.80</td><td>7.40</td><td>2.05</td></tr><tr><td>2003</td><td>1691</td><td>8.00</td><td>7.43</td><td>2.08</td></tr><tr><td>2004</td><td>1887</td><td>8.20</td><td>7.54</td><td>2.10</td></tr><tr><td>Change</td><td>0.66</td><td>-0.15</td><td></td><td></td></tr></table>

Demand, as measured by passenger numbers, increased over the years from 1991 to 2004. The total number of passengers in 2004 was estimated to be 1,887 million, up from 1,135 million in 1991, a 66% increase. There was a fall in passenger numbers at the end of 2001, reflecting increased caution following the terrorist attacks of 11 September 2001 but even this fall proved to be short-lived. With the increasing dominance of the budget airlines, it is expected that future trends will reflect ever more growth, in spite of potentially severe impacts on the environment (an issue to be examined in Chapter 7). 

For the price proxy, overall there was a 15% drop in revenue per passenger km over the years 1991 to 2004. There was a slight increase (with fuel price rises) in 2004 but overall our measure of demand (passenger numbers) and our proxy for price (revenue per passenger km) have moved in opposite directions, suggesting that there is an inverse relationship consistent with an inverse demand curve. 

## Dealing with data constraints

In conducting empirical analyses, data limitations are often an important constraint and it is important to acknowledge and justify these constraints from the outset. 

One major constraint emerges from a sampling bias: we are interested in demand for air travel from all consumers everywhere but our data is only capturing travel on scheduled flights; it excludes chartered flights, flights on private jets etc. The exclusion of particular categories of flights may distort our results. Also, even without potential sampling bias, the data just for passengers on scheduled flights may not fully capture demand. Did two passengers travel 50 miles each, or was it one passenger travelling 100 miles? Were they business or holiday travellers? Did they travel to capital cities or to small local airports? Did they travel first or economy class? And so on. We have lumped everyone together into a crude measure of ‘passenger kilometres’ but this does not allow us to distinguish between short trips and long ones. 

For the analysis in this chapter, we have an additional set of constraints because one of our aims is simply to illustrate OLS for simple regression analysis, i.e. using one explanatory variable. This focus on just one explanatory variable can be justified by assuming ceteris paribus (all things being equal) but if we did want to analyse a wider range of influences on demand for air travel, we might have problems collecting data on the many other influential variables, e.g. income trends, airline loyalty schemes, prices of substitutes and complements to air travel, costs of carbon offsetting etc. etc. A more detailed study would require us to gather price and quantity demanded data for a single carrier, over a single route, for a single class, and perhaps even with the same booking conditions. 

What about the data on prices? Passengers can pay different prices to travel exactly the same number of miles, depending on the airline with which they are flying, what class ticket they bought, whether they booked on the Internet or through a travel agent, and whether they booked weeks or just hours in advance. In fact, it is difficult to collect any sort of data specifically on prices. It is a common problem in statistical analysis that the phenomenon an econometrician would like to analyse is not easily measurable. One solution is to use a proxy variable. A good proxy will be strongly correlated with the missing variable but uncorrelated with the error term of our regression. What’s a good proxy for price in this example? As noted above, we have used ICAO on revenue per passenger per kilometre as a proxy; we would expect revenue per passenger km to be strongly correlated with prices. Again to keep things simple, we will also assume that revenue per passenger km is uncorrelated with the error term.<sup>1</sup> Using this proxy will also allow us to abstract from the complexities of routes and distances. On the other hand, price could have stayed the same, while passenger numbers could have increased for some other reason unrelated to price (e.g. rising incomes) and these two factors together would be manifested as falling revenue per passenger km. So overall, is it feasible to use revenue per passenger km as a proxy for prices? For our purposes we can justify the use ofthis variable on the basis that industry studies confirm that it is a good proxy but nonetheless we should acknowledge that measurement errors associated with using an imperfect proxy may affect our results. 

Another problem for our data set is the small sample size – we have just 14 annual observations from 1991 to 2004. It would be better, for example, if we had evidence from the 1960s and 1970s to extend the data set but we do not have easy access to a longer set of time-series data and the accuracy of our empirical results will be compromised by the limited information in our small sample. We are using annual data because we are trying to capture long-term patterns and estimates of long-run elasticities. These are of more interest to policymakers and company accountants because data gathered over 12 full months reflects the time that consumers have to change their behavioural patterns, towards or away from air travel compared to choices that might be more rigid in the shorter term. But the small sample size will probably affect the accuracy of our estimations.<sup>2</sup> 

One solution, if we were particularly interested in short-term elasticities, would be to search for data gathered more frequently. Another solution would be to create larger data sets, e.g. panel data sets that combine crosssectional and time series data. Panel estimation requires more complex techniques specifically designed simultaneously to capture spatial and temporal effects. 

## 3.4 Empirical methods and results

In setting up our empirical model of the data-generating process (DGP) for demand for air travel we have to think carefully about the specification of our model. We assume that air travel is a normal good and therefore we expect that the income effect and substitution effect will reinforce each other; there should be an unequivocally negative relationship between the price and quantity. In capturing these assumptions we need to select the correct functional form of our regression model. The issue of correct model specification is extremely important because, with a misspecified model, our OLS estimates will not be BLUE.<sup>4</sup> 

For our example ofdemand for air travel we must consider whether to use a linear functional form (i.e. using unlogged variables) or a logarithmic functional form (i.e. using the natural logs of our variables). We are assuming that the own-price elasticity of demand is constant, implying that airline passengers are equally responsive to changes in the price of very low-priced tickets (say, for short flights), as they are to changes in the price of high-priced tickets (say for round-the-world tickets.). As explained in Section 3.2, this is not consistent with a function that is linear in the variables. A log-log model will fit best with our underlying theory because it will embed a constant elasticity (see Box 3.3). 

Assuming a log-log specification, gives us the following model of the (DGP): 

$$
q _ {t} = \alpha + \eta p _ {t} + \varepsilon_ {t}\tag{3.8}
$$

where $q = \ln ( Q )$ and $\scriptstyle p = \ln ( P )$ and $\eta$ is the own price elasticity of demand for air travel. (We have transformed our raw data into natural logs in the final two columns of Table 3.2.) So we will be estimating the following sample regression function (SRF): 

$$
q _ {t} = \hat {\alpha} + \hat {\eta} p _ {t} + \hat {\varepsilon} _ {t}\tag{3.9}
$$

If we run a regression of $q$ on $\boldsymbol { p }$ then our slope parameter estimate $\hat { \eta }$ will be an estimate of the elasticity of the air-travel demand with respect to our price proxy; it will show us the percentage change in Q for a percentage change in P. What magnitude would we expect $\hat { \eta }$ to take? For most of us, air travel is a luxury. So we would expect its own-price elasticity to be relatively high, i. $\mathrm { e . ~ } - \infty < \eta < - 1$ , i.e. the response of quantity demanded to changing price should be relatively elastic so the parameter on price will be more negative than –1. 

In a preliminary assessment of our model we plot demand for air travel against our proxy for price over the period 1991 to 2004 (see Figure 3.3). This illustrates that passenger numbers have been rising whilst revenues have been falling, providing initial support for our hypothesis of an inverse relationship between demand and price. 

Are we correct in assuming that this is consistent with a downward sloping demand curve such as the one depicted in Figure 3.2? Figure 3.4 shows a scatter plot of air travel demand (logged) against the proxy (logged) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/fa96f44fa38e7d6140dfaef2d4dcac7f343f3978efbbb68a45cc96afd3aa8e68.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/03a48811eaeb4e85c8846317557ceb28bed5cc45d6d1cbd56727af8fa95dfbb9.jpg)



Figure 3.3 Rising global air travel, 1991–2004: rising demand and falling price


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/af7131d3951874887f6df5a486200ec8a046c00fef185eae10ba0a688b74f849.jpg)



Figure 3.4 Scatter plot of air travel demand (in passenger miles) suggesting constant elasticity of demand for air travel



Table 3.3 Example of an Excel output table Summary output log-log Model


<table><tr><td colspan="7">Regression Statistics</td></tr><tr><td>R Squared</td><td></td><td></td><td></td><td></td><td></td><td>0.79</td></tr><tr><td>Adjusted R Squared</td><td></td><td></td><td></td><td></td><td></td><td>0.77</td></tr><tr><td>Standard Error</td><td></td><td></td><td></td><td></td><td></td><td>0.08</td></tr><tr><td>Observations</td><td></td><td></td><td></td><td></td><td></td><td>14</td></tr><tr><td colspan="7">ANOVA</td></tr><tr><td></td><td>df</td><td>SS</td><td>MS</td><td>F</td><td></td><td>Significance F</td></tr><tr><td>Regression</td><td>1</td><td>0.28</td><td>0.28</td><td>45.71</td><td></td><td>0.00</td></tr><tr><td>Residual</td><td>12</td><td>0.07</td><td>0.01</td><td></td><td></td><td></td></tr><tr><td>Total</td><td>13</td><td>0.36</td><td></td><td></td><td></td><td></td></tr><tr><td></td><td>Coefficients</td><td>Standard Error</td><td>t Stat</td><td>P-value</td><td>Lower 95%</td><td>Upper 95%</td></tr><tr><td>Intercept</td><td>11.85</td><td>0.68</td><td>17.48</td><td>0.00</td><td>10.37</td><td>13.33</td></tr><tr><td>P</td><td>-2.12</td><td>0.31</td><td>-6.76</td><td>0.00</td><td>-2.80</td><td>-1.44</td></tr></table>

capturing the constant elasticity of demand relationship implied by our SRF (Equation (3.9)). 

This is consistent with a logarithmic specification ofthe demand function for air travel and also suggests that there is a constant price elasticity of demand for air travel. 

We can explore this pattern more rigorously by running an OLS regression using Excel’s analysis tool: ‘Regression’. When we use Excel’s regression tool, we get the Excel output table (Table 3.3) when we estimate the SRF from Equation (3.9). 

We have included the whole table so you can see an example of an Excel output table. But there is a lot of extra information in the table that we will leave for subsequent chapters. 

To summarise the essential information for this chapter, estimating our log-log model using Excel gives the following result: 

$$
Y = \begin{array}{l l l} 1 1. 8 5 & - 2. 1 2 X & + \hat {\varepsilon} _ {t} \\ (0. 6 8) & (0. 3 1) \\ t = 1 7. 4 8 & t = - 6. 7 6 \end{array}\tag{3.10}
$$

$$
R ^ {2} = 0. 7 9
$$

The numbers in brackets are the standard errors for the parameter estimates. 

We have a negative slope as expected, and the estimate of the own-price elasticity of demand indicates that the quantity of travel demanded increases by 2.12%, for a 1% fall in prices. As explained in Box 3.4, the estimate of $\eta = - 2 . 1 2$ is described as an elastic response: in percentage terms, the demand for air travel has risen by a greater proportion than the percentage fall in the price of air travel. 

To establish whether or not the inverse relationship between demand for air travel and our price proxy is statistically significant, we will test the hypothesis using a one-tailed t test. As explained in Chapter 1, we use a one-tailed test when we have some prior information about the sign of our parameters. In this case, we would expect our parameter to be less than zero; it is extremely unlikely that it would be more than zero because this would imply that air travel is a Giffen good, which is not a plausible hypothesis. So we set up the null and alternative hypotheses as follows: 

$$
H _ {0} \colon \eta = 0
$$

$$
H _ {1} \colon \eta <   0
$$

For a one-tailed test, our decision rule is modified because we are concentrating on one tail of the t distribution. As explained in Chapter 1, as long as the one-tailed test is justified on the basis of prior information, a one-tailed test will have more power than a two-tailed test: the probability of Type II error (of incorrectly retaining $H _ { 0 } )$ will be lower because the rejection region associated with the 5% significance level will all be in one tail. 

From statistical tables, a one-tailed test with a 5% significance level and degrees of freedom of $d f = n - k - 1 = 1 4 - 1 - 1 = 1 2 { \mathrm { ~ g i v e s } } - 1 . 7 8 2$ . So our decision rule will be: if $\hat { t } < - 1 . 7 8 2$ then reject $H _ { 0 } .$ . So, given our t value of –6.76, we can reject $H _ { 0 }$ and conclude that our estimate of the own-price elasticity of demand for air travel is significantly less than zero at a 5% significance level. 

We have tested a null that the elasticity is negative but we may also be interested in testing hypotheses about the absolute magnitude of the elasticity, e.g. that the absolute value ofthe elasticity is unitary, i.e. equal to 1 (see Chapter Exercise 3.7.1). 

Our estimate is larger than the estimates reported in previous research (as summarised in Box 3.4). This may reflect data constraints, sampling bias, our small sample size and/or omissions from our model. As explained in the section on data constraints, we have made a number of assumptions so that we can illustrate some introductory statistical techniques. In a more rigorous multiple regression analysis (MRA) we would use the techniques explained in Part II of this book. More specifically, we would include additional explanatory variables to overcome any biases that are emerging because important explanatory variables have been left out. What sort of extra variables would we add in capturing demand for air travel? One possibility is an income variable. The observations on quantity and the price proxy used in this chapter do not allow us to distinguish between movements along the demand curve versus shifts of the demand curve. With a positive income elasticity for air travel (assuming that it is a normal good), and increasing per capita real income (as seen in most developed countries over the period) a regression omitting an income variable may have led to a distortion of the absolute price elasticity of demand. 

What other variables could be used? The exclusion of prices of substitutes (e.g. prices of car travel) may also have biased the estimate of elasticity of demand for air travel. This omission might have particularly important consequences for the comparative analysis of short-haul travel versus longhaul travel so we could collect some data about the relative contribution of short-haul flights, compared to long-haul ones. We could also try to distinguish between leisure and business travellers given that previous studies have suggested that demand for leisure travel is more elastic than demand for business travel. Also, we have simplified by concentrating on the demand side and abstracting from the cost side. Some cost-side factors that may be relevant include fuel and security costs, changes in the airline industry (e.g. reflecting the entry of the budget airlines), changes to aviation taxation policies etc. etc. If we were to conduct a really robust econometric analysis taking full account of the supply side as well as the demand side, then we could use simultaneous equation estimation techniques. These techniques are beyond the scope of this book but some related issues are touched upon in Chapter 8. 

These caveats allowing, we can conclude by saying that our evidence suggests that the demand for air travel is elastic. It is also broadly consistent with the much more detailed and sophisticated studies summarised in Box 3.4 (for leisure travel at least). This finding is good news for the airlines because an elastic response implies that a fall in price will lead to a larger rise in revenue: the distances travelled by air-travellers have risen by a greater proportion than the fall in the price of travel. 

## 3.5 Implications and conclusions

The concepts analysed in this chapter have relevance to a range of policy issues. The microeconomic concepts will inform the marketing strategies of individual airline operators, explaining the many ‘two for the price of one’ or ‘half-price weekend’ deals that we frequently see advertised. Similar pricing deals operate in other industries – e.g. mobile phone companies. Discount deals such as these are not intended to be gifts or to comfort homesick expatriates – they are a sophisticated effort to map the demand schedule, and to discover the prices that will maximise corporate revenues. The evidence presented here suggests that, from the demand side at least, a strategy of lowering ticket prices would appear to be a profitable strategy. But for a fuller exploration of this issue we could look at the supply side too because pricing policies will depend also on the cost of running an airline. 

More broadly, concepts of price elasticity are also important for macroeconomic policy. Elasticity analysis is used in the formulation of fiscal policy, e.g. in designing taxation strategies. Governments may want to tax some goods and services to raise revenue and/or to dampen consumer demand. Increasing taxation on goods for which consumers have inelastic demand may have positive fiscal and social benefits: for example, if the demand for tobacco/alcohol is inelastic then policy-makers can generate substantial tax revenues by introducing tobacco taxes and duties on alcohol, and some of this revenue can be earmarked for public health expenditure. Overall, the precise impact of such policies will depend on the own-price elasticity of demand for alcohol and cigarettes. 

## 3.6 Further reading

## Textbooks



Grant, S. and Bamford, C. (2006) Transport Economics (4th edition), Oxford: Heinemann Educational Publishers. 





Varian, H. (2006) Intermediate Microeconomics (7th edition), London: W. W. Norton & Co. Chapters 5–6 and 15. 



## Journal articles



Brons, M., Pels, E., Nijkamp P. and Rietveld P. (2002) ‘Price elasticities ofdemand for passenger air travel: a meta-analysis’, Journal ofAir Transport Management, vol. 8, no. 3, 165–75. 





Ito, H. and Lee D. (2005) ‘Assessing the impact ofthe September 11 terrorist attacks on the U.S. airline demand’, Journal ofEconomics and Business, vol. 57, issue 1, 75–95. 





Verleger, P. K. (1972) ‘Models of the demand for air transportation’, Bell Journal ofEconomics and Management Science, vol. 3, no. 2, 437–457. 



## Policy reports



Gillen, D. W., Morrison W. G. and Stewart, C. (2003) Air Travel Demand Elasticities: Concepts, Issues and Measurement, Department of Finance, Canada. See www.fin.gc.ca/consultresp/ Airtravel/airtravStdy_1e.html 



## 3.7

## Chapter exercises

1. In this chapter we have established that the estimate ofthe price elasticity of demand for air travel is significantly less than zero at a 5% significance level. But we might want to know whether or not there is an elastic response (rather than no response at all). Using the data provided in this chapter, test whether or not the demand for air travel is elastic by: 

(a) Reformulating the hypotheses and decision rules to test that the elasticity is less than or equal to unity in absolute value terms. 

(b) Calculate the t test accordingly. 

(c) Interpret your findings. 

2. Using the data provided in Table 3.2: 

(a) Estimate (e.g. using Excel’s ‘Regression’ tool) the relationship between passenger miles and the price proxy assuming a linear specification, i.e. a lin-lin specification. (Hint: run the regression on unlogged variables.) 

(b) What are the parameter estimates from this regression capturing? 

(c) Discuss your results focussing on the parameter estimates. 

(d) What differences do you notice between the results from your lin-lin estimation and the log-log specification estimated in this chapter? (Hint: have a look at your t tests and $R ^ { 2 } .$ .) Explain the differences. 

(e) Which specification is preferable? Why? 

# Hypothesis testing Health expenditure and quality of life

Economic issues include: 

 Public goods and externalities 

 Asymmetric information and adverse selection 

Econometric issues include: 

 Hypothesis testing: using p values 

 The F test of explanatory power 

Data issues include: 

 Household survey data 

 Qualitative indexes 

## 4.1 The issue

How much should the State spend on health? One might doubt this is a question for economists – perhaps medical professionals should decide on patients’ needs and treatment costs or politicians should be asked about the desires of the electorate and its taxpayers. But economists can offer helpful tools with which to debate questions of this nature. No country has a blank chequebook, and public budgeting is a tense business of allocating scarce resources amongst competing needs. Economists can contribute helpfully to the debate on how resources might be best used by showing the relative costs and benefits of different strategies. This can help to reconcile, or at least to prioritise, diverse and sometimes conflicting objectives. Moreover, the question ofhow much governments should spend on health care is usually nested within the wider debate to which economists have long been central – namely, to what extent should the State be involved in the economy at all. In most countries this topic can be relied upon to produce heated argument from all ends of the political spectrum, in tones that are often highly ideological, and polemical. Our aim in this chapter is to shed some light on the heat by showing how empirical analysis can help raise the level of debate. 

## 4.2 The theory

Most industrialised countries have seen government spending rise over the last century, as have many developing countries. Even in the USA, with its strong private sector ethos, government real expenditure increased from 2.5% of GDP in 1870 to over 20% by the end of the twentieth century; and in most countries the levels are much higher. Typically much of the spending goes to defence (often as much as half the total), followed by health, education, and infrastructure; and the figure would double if subsidies and transfer payments (such as unemployment benefits, pension payments and so on) were also included. Its rationale is usually the public good argument, that the State provides services that benefit everyone because services will not be properly provided by the market alone. State intervention is also justified by the need to compensate for negative externalities and to subsidise positive ones that the market would fail to address; or to ensure social equity. This was most dramatically marked in many leading economies during 2008, as governments nationalised banks and bailed out ailing industries in an attempt to contain the effects of the global credit crunch. 

In the health sector, examples of these arguments include the public good aspect of vaccination against infectious diseases (where the vaccinations provide a non-rival and non-excludable benefit to the unvaccinated, by reducing the likelihood oftheir being exposed to disease). More recently, it is also argued that free and universal access to health care is a fundamental human right 

These ideas have a relatively long historical pedigree: Bismarck introduced public health insurance into Europe in 1883, and the idea spread so that by 1975 between 70 and 100 per cent of Europe’s total labour force was covered. The USA developed a different tradition, with public insurance being directed only to the poor and the elderly, with the rest of the population insured privately. But both continents saw government spending on health increase, in both absolute terms and as a share ofGDP. Expenditure slowed in the 1980s alongside a variety of attempts to reform the public sector and to control costs and amid fears that government failure was worse than the market failures it aimed to rectify. Critics doubted that the welfare state had added much to social or economic welfare, and thought that public spending could be cut without sacrificing important policy objectives. These challenges are reflected in the flurry of health-sector reforms that most countries have experienced since the 1970s, including deregulation, the introduction of quasi-markets, (public sector institutions designed to incorporate market features to promote economic efficiency) or even full privatisation. 

The debate is still on with no country confident it has found the best means to provide the right quality and quantity of health services to its people. Moreover, costs are likely to keep rising as more sophisticated treatments are developed and our steadily increasing life expectancy and ageing population fuels demand. Public money generally predominates in the financing of health care and this strains government budgets for health services. Public health and prevention programmes, which are especially cost effective, account for on average only a small percentage of health-care spending (usually less than five per cent). 

More controversially, turning to markets and market-based ‘user pays health services do not necessarily help solve the problem. Private sector insurers not only exclude those who cannot pay; they also exclude people who can pay but who have predictable or costly problems. Unless countries are willing to see these people abandoned by the health system completely, the State must step in. Congenital illnesses and pregnancy for example are often not covered by private insurers. Market-oriented health care is also criticised for inducing wasteful expenditures, including supply-induced-demand (feepaid doctors may encourage patients to consume excessive amounts of care). There is also myopia: people may not purchase health insurance because they underestimate their future health costs. 

One of the critical sources of market failure affecting the health sector is asymmetric information, creating many problems and inequities. Asymmetric information is a particular type of imperfect information in which one signatory to a contract has more information than another. Asymmetric information problems are very common in economics, as we will see in later chapters. One type of asymmetric information problem is moral hazard. This is a problem of‘hidden action’: after contracts have been signed the beneficiaries of a contract may have an incentive to cheat on the contract. In a health-care setting this would be associated with patients trying to get the most ofout their health insurance premium by over-consuming health-care services – they may continue to smoke without telling their health insurer for example. 

Another asymmetric information problem is adverse selection. This is a pre-contractual problem of ‘hidden attributes’: before a contract is signed, signatories to a contract may be able to conceal relevant characteristics about themselves because those characteristics are not readily observable, e.g. to a health insurer. Akerlof(1970) illustrates the consequences ofadverse selection problems using his lemons principle: in used car markets, average car prices will be pulled down by the quality of the ‘lemons’ until the market disappears completely. 

The lemons principle can be applied to health insurance markets: adverse selection problems will mean that health insurance companies cannot distinguish between the healthy and the unhealthy. The more unhealthy people, who realise that they may need health care services in the future, will have a greater incentive to sign up to health insurance contracts; the most-healthy people will not and, because health insurers cannot easily tell the difference, they will set their premiums to match average healthiness. This premium will deter the relatively healthy from taking out health insurance contracts so they will leave the health insurance market. So average healthiness will fall and premiums will rise. This will deter the next-most-healthy group of potential customers; they too will leave the health insurance market, average health will fall again, premiums will rise again and so the process continues. Premiums will rise and there will never be enough relatively healthy members to keep the premium low unless mechanisms are put in place to reduce the asymmetric information (e.g. health screening by insurance companies, healthy people signalling that they’re healthy via their lifestyle choices etc.). 

In the extreme, this process will continue indefinitely until the market for health insurance disappears. On the other hand, forcing symmetric information might be considered unethical. So some countries have implemented a solution whereby health insurers are not allowed to exclude anyone, and can differentiate premiums only on the basis of age or gender, not by individual patient characteristics; in such systems all individuals are required to take insurance. 

Overall the problems outlined above suggest that market solutions may not provide the best way either to finance or provide health care. But public health care is not perfect either. In developed countries, it is often criticised for being of poor quality and for relying excessively on rationing by queuing, where those with urgent problems are treated immediately. Those with minor problems have to wait a long time – sometimes so long that the minor problems become major problems. It is not always clear that tax-payers get value for money, or that the funds are used efficiently, let alone equitably. Under-investment in public health over a long period of time can create problems of poor infrastructure or lack of skilled professionals making it extremely difficult to boost quality and services, even if funds are eventually forthcoming. 

The arguments are less heated in developing countries, where medical services are provided at a lower level of technology, lower costs and much lowered expectations about the quality of public health care. Much of the public expenditure in these countries is aimed at public health problems that the industrialised world resolved in the nineteenth century – with the very important exception of HIV/AIDS. 

Does it matter whether the provision of health services is publicly or privately funded? The arguments above imply that higher public contributions to the total health budget encourage better health outcomes because, even in a country with high levels of expenditure overall, there are some sorts of services that private insurers will never cover, e.g. preventative health programmes and health education; these expenditures are typically the domain of the public sector. In this chapter we will focus on the impact of public health provision and statistically assess the relationships between healthiness and health expenditure across a cross-section of developed and developing countries. 

## 4.3 The data

Collecting data on health and health expenditures is not straightforward because the value of healthiness is not easily measured in monetary terms. One approach is to use survey data. An example, from Tanzania, of the benefits of using appropriate survey data to examine and to guide health expenditure is described in Box 4.1. 

The key to the success of the Tanzanian exercise was the careful collection of relevant data, and these data were then used strategically to guide the efficient spending of a limited health budget. This sort of data collection exercise can present special challenges in developing countries. Panel data household surveys (interviewing the same family on regular intervals) in Nairobi slums, for example, are affected by the fact that houses can disappear overnight. On the other hand, the benefits that can be achieved when we have better information about needs and priorities clearly make the effort worthwhile. 

But a major problem for surveys is that they are prone to sampling bias, especially if a researcher is not careful to select a sample that is representative of the relevant population. Identifying representative households involves 

## Box 4.1 Health surveys in Tanzania: information as the best medicine

The benefits of data collection and analysis have been made strikingly clear in two poor, rural regions of Tanzania, where infant mortality fell by almost half in just six years following an innovative study into the causes of death. The results have been so dramatic that the data collection methodology is now being rolled out across the whole country. 

One in ten children were dying before they reached their first birthday. So the Tanzania Ministry of Health began working with the Canadian aid agency, the International Development Research Centre (IDRC), to look for ways to improve the impact of their health expenditure. Together they searched for information about the causes of death, so that priority could be given to treatments that saved more lives at lower cost, and less priority given to treatments that saved few lives, at higher cost. This seems obvious now, but very few developing countries would readily have the information to ascertain this. Not least, most people die in their homes so very little information reaches the health planning authorities. 

The project focussed on health outcomes in two rural districts over the period 1997 to 2003, to the south and east of the largest city, Dar es Salaam. Researchers on bicycles carried out door-to-door surveys, asking representative households whether any family member had died or been ill lately, and with what symptoms. 

Figure 4.1 shows that there was no clear relationship between health expenditure priorities and the prevalence of disease. For example, malaria accounted for 30% of the years of lives lost in one region, but only 5% of the budget. A number of ‘childhood problems such as pneumonia, diarrhoea, malnutrition and measles claimed 28% of the life years lost, but got only 13% of the health budget. At the other extreme, 22% of the budget was directed 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/a2d0d14cb3f5a8af852e63c449bda07ec03b34c1cd06e0e9fec4804ec6ae24cf.jpg)


% health budget % lives lost 


Figure 4.1 Health interventions in Tanzania: money spent did not match health needs


towards tuberculosis, which accounted for only 4% of deaths in the sample. The interpretation was not that the tuberculosis vaccination programme should be stopped: falls in the tuberculosis death rate no doubt reflected the success of the vaccination programmes. But in terms of future spending strategies, the falling tuberculosis death-rate was consistent with plans to lower expenditures on vaccination programmes. 

The new information meant that medical efforts could be concentrated more effectively, and health status indicators improved as a consequence: the early results of better matching between health needs and health spending were staggering, with infant mortality dropping by 28% in just one year. Over six years of the mapping exercises, infant mortality dropped by 43% in one region, and 46% in the other. 

The tragedy of the lives lost before this programme is that some of the most effective early treatments are not costly: for example, oral rehydration salts for children with diarrhoea cost only a few cents. Other more pricey treatments have been shown to be so effective that even poor households try to pay the cost. Insecticide impregnated mosquito nets, for example, seem expensive at $3 each but not in terms of the life years saved. Moreover, as families are able to stay healthy longer, they can also become less poor. Families that used to suffer malaria fevers every few months could stay well for a whole year, and even accumulate extra food and cash over that period. 

Sources: Tanzania Essential Health Interventions Project, IDRC, Canada. 

seeking information from particular households, rather than a random ‘doorknock’, in an effort to obtain a picture that is representative of the entire population. Calling on households at random could generate non-random results if, for example, the only people home to answer the survey were the unemployed, the aged, or the infirm. 

For our quantitative assessment of the links between healthiness and health expenditure, we are examining healthiness at a broader scale. We examine the assertion that ifone country spends more on health care than another, then its people should enjoy a healthier life and live longer and its babies should have a sturdier start in life. 

Whilst it is relatively easy to make cross-country comparisons of health budgets using government health expenditure, survey data of the type used in Tanzania are not usually available for cross-country comparisons of healthiness. So how do we measure improvements in average health across countries? In this chapter we explore the relationships between healthiness and health expenditure using a sample of 24 high and low income countries. 


Table 4.1 Infant mortality, life expectancy, and public expenditure on health


<table><tr><td></td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>7</td></tr><tr><td></td><td>Life expectancy (average in years)</td><td colspan="3">Infant mortality (deaths per 1000 live births)</td><td colspan="3">Public health expenditure (% of GDP)</td></tr><tr><td></td><td>1999</td><td>1960</td><td>1999</td><td>Change (%)</td><td>1960</td><td>1998</td><td>Change (%)</td></tr><tr><td>Australia</td><td>78.78</td><td>20.20</td><td>4.90</td><td>-75.7%</td><td>2.40</td><td>5.90</td><td>145.8%</td></tr><tr><td>Austria</td><td>77.93</td><td>37.50</td><td>4.40</td><td>-88.3%</td><td>3.10</td><td>5.80</td><td>87.1%</td></tr><tr><td>Belgium</td><td>78.03</td><td>31.20</td><td>5.38</td><td>-82.8%</td><td>2.10</td><td>7.90</td><td>276.2%</td></tr><tr><td>Canada</td><td>79.03</td><td>27.30</td><td>5.30</td><td>-80.6%</td><td>2.30</td><td>6.40</td><td>178.3%</td></tr><tr><td>France</td><td>78.51</td><td>27.40</td><td>4.80</td><td>-82.5%</td><td>2.50</td><td>7.30</td><td>192.0%</td></tr><tr><td>Germany</td><td>76.99</td><td>35.00</td><td>4.83</td><td>-86.2%</td><td>3.20</td><td>7.90</td><td>146.9%</td></tr><tr><td>Ireland</td><td>76.12</td><td>29.30</td><td>5.50</td><td>-81.2%</td><td>3.00</td><td>4.70</td><td>56.7%</td></tr><tr><td>Italy</td><td>78.29</td><td>43.90</td><td>5.43</td><td>-87.6%</td><td>3.00</td><td>5.60</td><td>86.7%</td></tr><tr><td>Japan</td><td>80.63</td><td>30.40</td><td>3.60</td><td>-88.2%</td><td>1.80</td><td>5.90</td><td>227.8%</td></tr><tr><td>Netherlands</td><td>77.65</td><td>17.90</td><td>5.10</td><td>-71.5%</td><td>1.30</td><td>6.00</td><td>361.5%</td></tr><tr><td>New Zealand</td><td>77.39</td><td>22.60</td><td>5.23</td><td>-76.9%</td><td>3.50</td><td>6.20</td><td>77.1%</td></tr><tr><td>Norway</td><td>78.48</td><td>18.90</td><td>4.02</td><td>-78.7%</td><td>2.60</td><td>7.40</td><td>184.6%</td></tr><tr><td>Spain</td><td>77.91</td><td>43.70</td><td>5.30</td><td>-87.9%</td><td>0.90</td><td>5.40</td><td>500.0%</td></tr><tr><td>Sweden</td><td>79.26</td><td>16.60</td><td>3.60</td><td>-78.3%</td><td>3.40</td><td>6.70</td><td>97.1%</td></tr><tr><td>Switzerland</td><td>79.56</td><td>21.10</td><td>4.56</td><td>-78.4%</td><td>2.00</td><td>7.60</td><td>280.0%</td></tr><tr><td>UK</td><td>77.25</td><td>22.50</td><td>5.70</td><td>-74.7%</td><td>3.30</td><td>5.60</td><td>69.7%</td></tr><tr><td>USA</td><td>76.91</td><td>26.00</td><td>6.90</td><td>-73.5%</td><td>1.30</td><td>5.80</td><td>346.2%</td></tr><tr><td>Denmark</td><td>75.87</td><td>21.50</td><td>4.65</td><td>-78.4%</td><td>3.20</td><td>6.80</td><td>112.5%</td></tr><tr><td>Finland</td><td>77.26</td><td>21.40</td><td>4.08</td><td>-81.0%</td><td>2.30</td><td>5.20</td><td>126.1%</td></tr><tr><td>South Africa</td><td>48.47</td><td>88.60</td><td>61.52</td><td>-30.6%</td><td>...</td><td>3.30</td><td>...</td></tr><tr><td>Singapore</td><td>77.55</td><td>34.80</td><td>3.20</td><td>-90.8%</td><td>...</td><td>1.20</td><td>...</td></tr><tr><td>Malaysia</td><td>72.34</td><td>70.60</td><td>7.90</td><td>-88.8%</td><td>...</td><td>1.40</td><td>...</td></tr><tr><td>Indonesia</td><td>65.72</td><td>137.80</td><td>41.92</td><td>-69.6%</td><td>...</td><td>0.70</td><td>...</td></tr><tr><td>Bangladesh</td><td>60.74</td><td>154.80</td><td>61.20</td><td>-60.5%</td><td>...</td><td>1.70</td><td>...</td></tr><tr><td>Mean</td><td>75.28</td><td>41.71</td><td>11.21</td><td>-78.0%</td><td>...</td><td>5.40</td><td>...</td></tr></table>


Sources: World Bank World Development Indicators, OECD Social Expenditure Database: 1980/1998. 


These data are summarised in Table 4.1 and were gathered from the following sources: 

World Bank World Development Indicators: www.worldbank.org 

OECD Social Expenditure Database: 1980/1998: www.oecd.org 

Other potential sources of data include the World Health Organisation (WHO), United Nations Development Programme (UNDP) and the national accounts of individual countries. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/ba78a7a90156966f5cff2f9f65dff230a383fa7d62225b6ebf3247702a46fe86.jpg)



Figure 4.2 Life expectancy for a cross-section of countries, 1999


## Indicators of health

The measure of healthiness that we use here is life expectancy, a frequently used indicator of national health standards. There are other ways to measure healthiness: another possibility is the infant mortality rate – the number of infant deaths per 1,000 live births. 

The life expectancy data (column 1 of Table 4.1) shows a wide range of outcomes across the sample with a relatively short average lifespan (of just over 48 years) in South Africa but a relatively long average lifespan (of almost 81 years) in Japan. 

These data are plotted in Figure 4.2 to give a visual impression of the spread of life expectancy outcomes. This plot shows that there is a clear division between the performance of the rich, developed countries – all of which have approximately similar average life expectancies of between 76 years and 81 years and the poorer less-developed countries, which experienced average life expectancies ranging between 48 and 72 years. 

Infant mortality rates are another measure of the healthiness of a nation and data on infant mortality in 1999 relative to infant mortality in 1960 are shown in Table 4.1 (columns 2 to 4). In general, infant mortality has improved over the past 40 or so years, even in countries that still have a relatively high number of infant deaths. Bangladesh recorded 61 infant deaths per 1,000 live births in 1999, compared to 155 in 1960. Developed countries such as the USA and UK registered even greater improvements, despite their better baseline (relative improvements are harder when performance is already good!). 

There may be other aspects of healthiness captured neither by life expectancy measures nor by infant mortality measures. For this reason, qualitative and composite indicators may also be helpful (see Box 4.2 for an outline of quality of life indicators). 

## Measuring health expenditure

To capture health expenditure in this analysis we use OECD data on public expenditure on health as a percentage ofGDP (see columns 5 and 6, Table 4.1). Expenditure is measured relative to GDP to control for the economic size of the countries in our sample. It would be distorting to compare the absolute expenditures of large countries such as the USA with the absolute expenditures of smaller countries with otherwise similar health-related factors (e.g. similar levels of development, education or life-styles etc.) Just to focus on absolute figures would capture neither the relative commitments of governments to health expenditure nor the relative demands on health services given the economic or demographic size of a country. For example, the UNDP Human Development Report reveals that 2002 health expenditure in the USA amounted to $1,545 billion but the UK spent $128 billion in the same year. This doesn’t mean that the UK government had less of a commitment to health than the US government; it reflects that fact that the UK is a smaller economy. So we can ‘weight’ each country’s expenditure by expressing expenditure as a proportion of GDP. 

Also, when comparing health expenditure between countries (or even within one country over time), we cannot say that $1 worth of health care bought the same quality of services in all situations. There is no readily available equivalent to indices of purchasing power parity (PPP) i.e. measures of the value of a currency in terms of the value of goods and services it can buy. PPP measures can provide a very useful means to compare the real purchasing power of different currencies but economists have struggled to develop reliable PPP indicators for health services. 

By comparing the performance in 1960 (column 5, Table 4.1) and 1998 (column 6, Table 4.1) we can calculate the % change in expenditure (column 7, Table 4.1). These data reveal a sustained increase in governments’ commitment to public health expenditure: health expenditure increased from a mean 

## Box 4.2 Measuring healthiness: The Quality of Life Index and the Human Development Index

How should we decide on priorities for health spending? As described above, once a policy maker decides that a health budget should be set at some fixed amount, then priorities for spending have to be determined. One way to decide is on the basis of the benefits of various treatments. But defining and measuring these is extremely difficult, particularly because it involves making inter-personal comparisons or aggregating effects over a large number of individuals. It is not obvious how to compare the benefit of the same operation given to two different patients – for example, the benefit of a heart transplant to an otherwise healthy person, compared with the benefit to another patient with additional confounding health problems; or the benefit to a young person compared to an old one. And it is even more difficult to compare the benefits of different operations between different people – even if all the operations cost the same price. Measuring benefits in terms of their effect on labour productivity is one approach, but it is a very narrow definition of ‘benefit’; moreover it is biased against elderly or low paid individuals. 

Another method involves the use of Quality of Life Index (QLIs), which ranks different health states, so one can compare the benefits to different patients of different sorts of treatments. Ranking patients’ health status according to this scale produces a relatively objective measure of the benefits of various treatment options (McGuire etal. 1987). For example, physicians studying quality of life for people suffering from the inherited disease phenylketonuria (PKU) ranked 15 different health states, ranging between ‘death’ (=0.00) and ‘no symptoms’ (=1.00), and including: (a) confined to house, walking freely and able to care for oneself but not doing any major activities (=0.435), and (b) in hospital, walking freely but requiring assistance with self-care (=0.165). 

The Human Development Index (HDI) is an example of a composite index that measures a country’s performance across three areas of human development; life expectancy, literacy and standard of living (as measured by GDP per capita). This index allows us to rank countries that may have very similar levels of income but different outcomes in terms of infant survival rates and/or educational attainment. The United States, for example, ranked 6th on the 2002 HD (scoring 0.939) while the United Kingdom ranked 13th (at 0.928). By comparison, Germany ranked 17th (0.925), South Africa ranked 107th (0.695), Bangladesh was 145th (0.478), and Sierra Leone was ranked lowest – in 173rd place (0.275). 

The approach used in constructing the HDI can also be extended to measure poverty, capturing impacts that go far beyond simplistic income measures. For example, the Human Poverty Index (HPI), which was introduced in Chapter 2, includes the proportion of the population in each country with access to safe water supplies. The Gender-Related Development Index (GDI) adjusts for gender inequalities, to compare the positions of men and women between different countries. Sweden, which ranked 2nd in terms of the 2002 HDI, fell to 5th position in its GDI; the USA rose to 4th place in the GDI, and the UK rose to 12th place. 

Source: http://hdr.undp.org/statistics 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/8b72a57a6744fe2ad7069aacc4b0fc93ae873af9d1f0fecdaff44ae7fbc5c4d3.jpg)



Figure 4.3 Health spending for a cross-section of countries, 1998


across this sample ofonly 2.5% ofGDP in the 1960s to over 5.4% by 1998. The USA and Spain in particular recorded substantial increases of346% and 500% respectively. 

We plot 1998 health expenditure data in Figure 4.3 revealing again a broad division between the poorer, developing countries with health expenditures between 0.7% to 3.3% of GDP and the richer developed countries with health expenditures upwards of 4.7% of GDP. 

Note that this broad pattern ofhealth expenditure mirrors the pattern oflife expectancies shown in Figure 4.2: the countries with longer life expectancies are the countries with higher health expenditures and this supports our hypothesis about a link between public health spending and healthiness. But it is important also to emphasise: firstly that a correlation between variables does not necessarily imply a causal mechanism and, secondly that there may be limitations on our data, as discussed below. 

## Data limitations

Before proceeding with a statistical analysis of these data, we should explore the limitations of our dataset. Firstly, a comparison of the life expectancy and infant mortality data illustrates that life expectancy may be an imperfect measure of a nation’s healthiness. There are significant divergences between some countries’ performance in terms of life expectancy versus infant mortality: for example, Canada had one of the highest life expectancies but alongside a relatively high infant mortality rate. Conversely, Singapore had a relatively low life expectancy but the best outcome across the sample in terms of low levels of infant mortality. In these cases, which measure more accurately captures healthiness? Probably neither or both! 

Further biases are revealed in the life expectancy data. Figure 4.2 reveals that South Africa is a significant outlier (with a very low life expectancy) and the remaining developing countries in our sample (namely Malaysia, Indonesia and Bangladesh) have also experienced low life expectancies. Also, in terms of our analysis of the impact of health expenditure the clear divide between rich and poor countries captured in Figure 4.2 is likely to be a reflection of a complex range of factors some of which will be unrelated to our explanatory variable – public health expenditure. 

In assessing our data we must keep in mind the constraints on crosssectional comparisons. In analysing phenomena in poorer countries for example, missing data can be a common problem. Richer countries are more likely to have good data collection and they are probably also committed to relatively high levels of health expenditure. This sample is strongly skewed in favour of rich countries. This may create sampling bias so we need to keep in mind that the findings established in this chapter may not be robust in the countries which are poor. 

Overall, it is important to recognise that our data may not perfectly measure the phenomena in which we are interested and so the results from our statistical analyses may not be completely reliable. We could perhaps perfectly measure our variables if we had populations of identical people, living identical lifestyles, with some spending a little on health care and others spending a great deal, to buy variable quantities of identical quality services. Such a data series would of course be impossible to find. Imperfect data series and impure associations are a fact of life in economics but hopefully we can find good proxies for the effects that we want to understand. 

In this chapter we are illustrating some straightforward regression techniques and so we will assume away these complexities for the moment (though we will explore these problems in detail in later chapters). 

## 4.4 Empirical methods and results

In this chapter, we are analysing the relationship between healthiness and health expenditure. As we are still focussing on simple regression analysis, we have to confine ourselves to one explanatory variable. It is important to remember that this may make our model vulnerable to omitted variable bias – a particular type of model misspecification bias occurring when OLS estimates of parameters are biased by the influences of excluded explanatory variables.<sup>1</sup> We assume that there is a linear relationship between the dependent variable and the explanatory variable and so the empirical model we are testing is: 

$$
Y _ {i} = \alpha + \beta X _ {i} + \varepsilon_ {i}\tag{4.1}
$$

where Y is healthiness measured as average life expectancy in 1999, X is public health expenditure as a proportion of GDP in 1998 and $\varepsilon _ { i }$ is a random error term. Note that we have used a lag on the explanatory variable. This is because we would not expect instantaneous effects of health expenditure on healthiness. Using the data from Table 4.1, we estimate an econometric model for a cross-sectional sample of 24 countries using the following SRF: 

$$
Y _ {i} = \hat {\alpha} + \hat {\beta} X _ {i} + \hat {\varepsilon} _ {i}\tag{4.2}
$$

Before running this regression we can draw some broad inferences about the plausibility of our model by inspecting the scatter plot in Figure 4.4. This shows a broadly positive association between life expectancy and health expenditure. But it is important to remember that not all observations in a sample will fit the broad pattern: here for example, Indonesia had the lowest spending but not the lowest life-expectancy; South Africa spent a relatively large amount on public health, but life expectancy was extremely low, at 48.5 years. 

For our other measure of healthiness – infant mortality – low expenditure on public health was also associated with higher infant mortality rates: countries with higher spending tended also to have reduced infant mortality. But we cannot make clear cross-country comparisons. For example, although the USA had the second highest increase in spending over the 40 years, it still had the fifth highest infant mortality rate. We won’t analyse the link between infant mortality and health expenditure in any more detail here because we have left that for one of the chapter exercises . . . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/47425ab61254fa6efcf6b648e5fbc59209da8855e65e1408d355ca030e2e46c4.jpg)



Figure 4.4 Longer life expectancy associated with larger health expenditures


Table 4.2 shows the Excel output table from running a regression of life expectancy on public health expenditure using our sample of 24 countries: 


Table 4.2 Excel output table Summary output


<table><tr><td colspan="7">Regression Statistics</td></tr><tr><td>R Squared</td><td></td><td></td><td></td><td></td><td></td><td>0.35</td></tr><tr><td>Adjusted R Squared</td><td></td><td></td><td></td><td></td><td></td><td>0.32</td></tr><tr><td>Standard Error</td><td></td><td></td><td></td><td></td><td></td><td>5.98</td></tr><tr><td>Observations</td><td></td><td></td><td></td><td></td><td></td><td>24</td></tr><tr><td colspan="7">ANOVA</td></tr><tr><td></td><td>df</td><td>SS</td><td>MS</td><td>F</td><td colspan="2">Significance F</td></tr><tr><td>Regression</td><td>1</td><td>414.31</td><td>414.31</td><td>11.60</td><td>0.00</td><td></td></tr><tr><td>Residual</td><td>22</td><td>785.90</td><td>35.72</td><td></td><td></td><td></td></tr><tr><td>Total</td><td>23</td><td>1200.21</td><td></td><td></td><td></td><td></td></tr><tr><td></td><td>Coefficients</td><td>Standard Error</td><td>t Stat</td><td>P-value</td><td>Lower 95%</td><td>Upper 95%</td></tr><tr><td>Intercept</td><td>64.69</td><td>3.34</td><td>19.37</td><td>0.00</td><td>57.77</td><td>71.62</td></tr><tr><td>Health Expenditure</td><td>1.98</td><td>0.58</td><td>3.41</td><td>0.00</td><td>0.77</td><td>3.18</td></tr></table>

These results can be summarised as follows: 

$$
\begin{array}{l l} \hat {Y} _ {i} = & 6 4. 6 9 + \\ & (3. 3 4) \\ & t = 1 9. 3 7 \\ & p = 0. 0 0 \end{array} \quad \begin{array}{l l} 1. 9 8 X _ {i} \\ (0. 5 8) \\ t = 3. 4 1 \\ p = 0. 0 0 \end{array}
$$

Standard errors are in brackets and we’ve also reported the p-values. We will explain these in more detail below. 

The estimate of $\hat { \beta }$ suggests that a 1 point increase in the share of GDP devoted to public health is associated with an extension of life expectancy of just under 2 years. But is this finding statistically significant? We assess at a 5% significance level using a two-tailed t test with the following hypotheses and decision rules: 

$$
\begin{array}{l l} H _ {0}: \alpha = 0 & H _ {1}: \beta \neq 0 \\ H _ {1}: \alpha \neq 0 & H _ {0}: \beta = 0 \end{array}
$$

We have 22 degrees of freedom $( n = 2 4$ and we lose one degree of freedom in estimating our intercept and another degree of freedom estimating the slope parameter on health expenditure). So for a 5% significance level and a twotailed test, $t _ { \mathrm { c r i t } } = 2 . 0 7$ and our decision rule will be: if $| \hat { t } | < t _ { \mathrm { c r i t } }$ then do not reject $H _ { 0 }$ but if $| \hat { t } | > t _ { \mathrm { c r i t } }$ then reject $H _ { 0 }$ . For ${ \hat { \alpha } } ; \mathrm { t } = 1 9 . 3 7 > 2 . 0 7 ;$ ; for $\beta \mathrm { : } \operatorname { t } = 3 . 4 1 > 2 . 0 7$ and so in both cases we reject $H _ { 0 }$ 

Focussing on ${ \hat { \beta } } ,$ we can conclude that there is a positive association between life expectancy and health expenditure that is statistically significant at the 5% level. This confirms the patterns from our more casual inspection of the data in Section 4.3. For this sample of countries, countries that are spending more on public health have a healthier population. 

There is another, quicker way to formulate decision rules – by using the probability values $( \pmb { p }$ values) mentioned above. Notice that these are reported in the Excel Output Table to the right of the t statistics. As explained in Chapter 1, decision rules can be constructed around $\boldsymbol { p }$ values because they give us an exact significance level, capturing the boundary significance level at which we will start rejecting our null. They allow us to reformulate our decision rule in a very straightforward way. For example if we are using a 5% significance level our decision rule becomes: if $ { p } > 0 . 0 5$ , do not reject $H _ { 0 } ;$ if $\textstyle p < 0 . 0 5$ reject $H _ { 0 }$ 

For the results in this chapter, the $\boldsymbol { p }$ value on our t test of the null that the parameter on health expenditure is zero, i.e. $H _ { 0 } : \beta = 0$ , gives $\mathtt { p } = 0 . 0 0$ which is less than 0.05 and so we can reject $H _ { 0 } .$ . Similarly we can reject the null that the intercept parameter is equal to zero $( \mathrm { i . e . } H _ { 0 } : \alpha = 0 )$ because the p value for this parameter estimate is also 0.00. 

The p values can be used for any sort of hypothesis test, including t tests, F tests and others. They are now widely reported in most statistical and econometrics packages. Using p values saves the time and trouble involved in looking up statistical tables but it is important to remember that they are formulated around a specific null hypothesis and this is usually the simplest possible null, e.g. that a parameter is equal to zero. 

As is explained in detail in Chapters 1 and 2, $R ^ { 2 }$ is the coefficient ofdetermination and measures the ‘goodness offit’ ofour estimated regression line. Here $R ^ { 2 } =$ 0.35 which indicates that 35% of the variability in life expectancy is captured by variability in health expenditure. But how can we judge this outcome? Is 35% too high, too low, or just right? We cannot say without a proper statistical test and to assess this question, we can use an F test ofexplanatory power, as outlined in Box 4.3. The result calculated there indicates that our $R ^ { 2 }$ is relatively high and our statistical model does capture a statistically significant proportion of the variability in life expectancy for our sample of countries. But it is important to remember (particularly as we are using simple regression analysis) that there will be many other factors influencing life expectancy apart from public health expenditure. Further analyses could focus on identifying the other determinants of life expectancy not only in a cross-sectional context but also in a time-series context. 

## Box 4.3 The F test of explanatory power

As explained in earlier chapters, when we want to test a single hypothesis, then one possibility is to use the Student’s t test. But when we want to draw inferences about the overall explanatory power of a model, e.g. as captured by $R ^ { 2 }$ , we can use the F test of explanatory power. As explained in Chapter 1, $R ^ { 2 }$ measures the proportion of the variability in the dependent variable that can be captured by the variability in the explanatory variables. So if we want to draw inferences about whether or not our $R ^ { 2 }$ is significantly different from zero, then we can test whether or not the slope parameter(s) are jointly equal to 0 using the F test of explanatory power.<sup>2</sup> 

The formula for the F test of explanatory power is: 

$$
F _ {k, n - k - 1} = \frac {R ^ {2} / k}{(1 - R ^ {2}) / (n - k - 1)}
$$

where k is the number of explanatory variables and n is the number of observations in our sample. For the model in this chapter, we have just one slope parameter (k= 1) but in its general formulation the F test of explanatory power tests the following null and alternative hypotheses for the slope parameters in a model with k explanatory variables: 

$$
H _ {0}: \beta_ {1} = \beta_ {2} = \dots = \beta_ {k} = 0
$$

$H _ { 1 } \colon$ at least one of the parameters is not equal to zero 

Decision rule: If $\tilde { F } { > } F _ { \mathrm { c r i t } } ,$ then reject $H _ { 0 } .$ 

This Ftest of explanatory power is known as a joint hypothesis test because it is testing the overall explanatory power contributed by all the explanatory variables in the model. This and other F tests are particularly important to estimating models with more than one explanatory variable i.e. for multiple regression analysis (MRA) and so this and other F tests will be discussed more extensively in Part II of this book. 

For simple regression analysis (SRA) the terminology above may seem confusing because of course we just have one explanatory variable and so just one slope parameter is included in our $H _ { 0 } .$ For the simple regression model in this chapter, $R ^ { 2 }$ is measuring the proportion of the variability in Y that can be captured by the one explanatory variable X. If we want to test whether or not our model overall captures a significant proportion of the variability in life expectancy, i.e. if we want to test whether or not the $R ^ { 2 }$ of 0.35 is significantly different from zero, then we can use the F test of explanatory power in the following way: 

$$
H _ {0}: \beta = 0
$$

$$
H _ {1}: \beta \neq 0
$$

Decision rule: If $\bar { F } { > } \bar { F } _ { \mathrm { c r i t } }$ , then reject $H _ { 0 } .$ 

$$
\begin{array}{r l} F _ {k, n - k - 1} & F _ {1, 2 2} = \frac {R ^ {2} / k}{(1 - R ^ {2}) / n - k - 1} \\ & = \frac {0 . 3 5 / 1}{(1 - 0 . 3 5) / (2 4 - 1 - 1)} = \frac {0 . 3 5}{0 . 0 3} = 1 1. 6 7 \end{array}
$$

You may have noticed that this F test result is also reported in the Excel output table as 11.60 (the very slight difference between these figures reflects rounding differences). Using our decision rule and a 5% significance level (i.e. with a 95% confidence interval), $\boldsymbol { F _ { \mathrm { c r i t } } }$ $( 1 , 2 2 ) = 4 . 3 0$ . So $F > F _ { \mathrm { c r i t } }$ . Therefore we can reject $H _ { 0 }$ and conclude that the model overall does capture a significant proportion of the variability in Y. This result verifies the result from our ttest. In fact, in the SRA case the Ftest is just the square of the ttest and (again allowing for rounding differences) $t = 3 . 4 1  t ^ { 2 } = 1 1 . 6 3$ which is approximately equal to the F of 11.67 calculated above. 

## 4.5 Implications and conclusions

The regressions in this chapter indicate that relatively high expenditures on public health are associated with longer life expectancies. Does this mean that governments should spend more? The simple answer may be ‘yes’ if we agree that a change in health expenditure can be compared on the same terms as a change in health outcomes. However before we can translate our findings into robust policy implications, more detailed work must be done. 

Our empirical results may not be as clear-cut as implied above because several problems are likely to muddy our data and confound our results. Not least, our regression is a crude tool that compares broadly defined, total public health expenditure on the one hand, with a precise and narrowly defined healthiness indicator on the other. We may have overestimated the importance of public health expenditure – public funds are spent on many health services completely unrelated to the mortality chances of new-born babies, such as adult cancer treatment, heart disease and hip replacements (all of which absorb large proportions of public health expenditure in many countries). We do not have information about the amounts devoted to infant or maternal care over the period studied. Finding more about these patterns of spending could also have important implications for the results. 

Other problems may lie in the specification of our model. For this chapter we have been using simple regression analysis to estimate the impact of just one explanatory variable and this may generate biases in our estimation procedure. We will introduce multiple regression analysis (MRA) in the next chapter but, in the meantime, we should be cautious in the interpretation of results from a model with just one explanatory variable. 

Last but not least, an extremely important question to consider is the issue of correlation versus causation: it is difficult, if not impossible, to separate correlation from causation. This is a key problem for most econometric analyses. In the context of healthiness, it could be that the causality operates in the opposite direction (people who live longer will demand more healthcare); or another variable may be affecting both health expenditure and life expectancy (e.g. effective governments are seen in countries at higher levels of development). Income may also have an impact, particularly in LDCs where higher incomes are associated with better health because of better sanitation, less starvation and so on. 

Other factors such as diet, income, social status, genetic inheritance, education, and lifestyle choices (such as to smoke or not) may be as important as the quality and quantity of health care available. For infant mortality, the nutrition of both mother and infant will have critical impacts, as will water quality, sanitation and hygiene. In nineteenth-century Europe, for example, improvements in the quality of water supplies and sewage disposal, as well as the sterilisation, bottling and safe transport of milk, sharply reduced infant mortality; and the same is likely to be the case in the world’s LDCs. The World Health Organisation (2008) has reported that there are important social determinants of health and these are captured by a social gradient: healthiness rises not only with income but also with relative social standing. So improving healthiness depends not only upon growing income but also upon a more equitable income distribution both within and across nations. Public policy will also have an effect: regulations requiring seatbelts to be worn in cars, or helmets to be worn when cycling, have a large impact on mortality and life expectancy even though such policies are not financed via public health expenditure. So even if we do find highly significant correlations between variables, we cannot assume that this reflects a causal link between the variables. 

## 4.6

## Further reading

## Textbooks and lectures



Atkinson, A. B. and Stiglitz, J. (1980) Lectures on Public Economics, New York: McGraw-Hill. 





Auerbach, A. J. and Feldstein, M. (eds.) (2002) Handbook ofPublic Economics, Amsterdam: Elsevier. 





McGuire, A., Henderson, J. and Mooney, G. (1987) The Economics of Health Care, London: Routledge. 





Stiglitz, J. (2000) Economics of the Public Sector, 3rd edition, London: W.W. Norton & Co., Chapter 12. 



## Journal articles



Akerlof, G. (1970) ‘The market for lemons: quality, uncertainty, and the market mechanism’, Quarterly Journal ofEconomics, vol. 84, no. 3, 488–500. 





Arrow, K. (1963) ‘The welfare economics ofmedical care’, American Economic Review, vol. 53, no. 5. Cutler, D. (2002) ‘Equality, efficiency and market fundamentals – the dynamics ofinternational medical care reform’, Journal ofEconomic Literature, vol. 40, no. 3, 881–906. 



## Policy Reports

OECD (1985) Social Expenditure 1960–1990: Problems of Growth and Control, Paris: Organisation for Economic Cooperation and Development. UNDP (annual) Human Development Report, Geneva: United Nations Development Programme. 

World Bank (annual), World Development Report, Washington: World Bank Group. 

World Health Organisation (WHO) (annual) World Health Report, Geneva: World Health Organisation. 

World Health Organisation (WHO) (2008), Closing the Gap in a Generation: Health Equity through Action on the Social Determinants of Health, WHO Commission on Social Determinants of Health, Geneva: World Health Organisation. 

## 4.7 Chapter exercises

1. In this chapter we have examined the relationship between health expenditure and life expectancy. Using the data from Table 4.1, analyse the relationship between infant mortality and health expenditure as follows: 

(a) Generate a scatter plot of infant mortality against health expenditure. 

(b) Estimate a line of best fit using the Excel Regression tool. 

(c) Discuss the findings from the hypothesis tests including 

i. t tests of single hypotheses 

ii. the F test of explanatory power. 

(d) For these hypothesis tests construct decision rules using 

i. p values 

ii. critical values from statistical tables. 

(e) Interpret your findings – is there an association between health expenditure and infant mortality? Is the association significant? 

(f) What are the limitations of your analysis? 

2. In this chapter we’ve been using simple regression analysis on one explanatory variable. Other variables will have an impact on life expectancy. 

(a) Using some of the data sources outlined in this chapter, e.g. the World Bank’s website, www.worldbank.org, collect some data on variables that you think may be important determinants of a nation’s healthiness. 

(b) Set out an empirical model including more than one explanatory variable. 

(c) Using the Excel Regression tool, estimate your empirical model of healthiness using multiple regression analysis (MRA). (HINT: this is just a matter of incorporating extra columns within the “Input X Range” of the Excel ‘Data Analysis – Regression’ tool.) 

(d) What do you think might be some of the statistical and theoretical implications of using MRA rather than SRA? 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/a19225bc553aab0cd920e511e08b1a10670d5832df3a710cf21dd62b6b7ecadf.jpg)


# Multiple regression and diagnostic testing

In Chapters 2–4, we introduced the basic OLS techniques associated with simple regression analysis (SRA). But, as explained in Chapter 1, OLS is the Best Linear Unbiased Estimator (BLUE) – i.e. the most reliable and accurate estimator of parameters – only when the Gauss–Markov (GM) assumptions are satisfied. In many cases, GM assumptions will be violated and OLS will be inadequately simple; for example the omission of important variables will generate biases in SRA. And there may be other econometric problems further compromising the BLUEness of OLS. 

In Part II we introduce multiple regression analysis (MRA), i.e. regressions on models with more than one explanatory variable. We also outline some commonly used econometric tests and procedures, for example the diagnostic tests used to discover violations of the GM assumptions. We will also introduce some procedures for correcting violations of GM assumptions. 

# Multiple regression analysis Housing demand in the UK

Economic issues include: 

 Durable consumption goods 

 Credit constraints and gearing 

Econometric issues include: 

 OLS using EViews 

 Multiple regression analysis (MRA) 

 F tests of restrictions 

Data issues include: 

 Hedonic pricing 

 Capturing seasonality using dummy variables 

 Dummy variable trap 

## 5.1 The issue

Developments in housing markets have wide-ranging implications for the macro-economy. Increases in house prices will boost household wealth, thereby boosting consumption and fostering increases in aggregate demand. Increases in house prices may also affect consumer confidence and expectations, increasing general optimism within the economy. On the other hand, rigidities in housing markets have crucial implications for labour mobility, employment and unemployment. For example, housing market volatility will limit the ability ofpeople to move in search of better jobs: Oswald (1997) observed that countries with fastest growth in home ownership in the 1980s and 1990s had the fastest growth in unemployment and attributed this to the labour immobility of owner occupiers in depressed housing markets, particularly those home owners who face negative equity (a situation which occurs when mortgage borrowings on a property exceed the value of the mortgaged property). 

The affordability of housing will also affect householders’ decisions to invest in housing: as house prices rise and incomes fall, people will choose other alternatives (e.g. renting, living with family) and cannot afford to enter the housing market either because their incomes are too low and/or because they cannot get easy access to mortgage credit. For many people in the UK and other OECD countries, declining affordability has meant that younger, poorer people have to wait a long time before becoming homeowners; in the meantime, the older/richer people who were able to afford housing a decade ago will have benefited from the spectacular rises in house prices that occurred from the late 1990s until 2007; they will have accrued an increased share ofthe stock of household wealth. In this way, volatile housing markets will have contributed to wealth inequalities. 

House prices are affected by a wide range of other variables including the stock of housing, population growth and changing demographic patterns, government regulation and fiscal incentives/disincentives for owner occupation (e.g. stamp duty in the UK). House prices can also be volatile because of supply constraints; with inelastic supply, the price effects of shifts in demand are amplified. For new housing in particular, the supply of housing stock is inelastic in both the short term and the long term; firstly, because of the lags involved with housing construction and secondly, because the supply of land available for new housing is constrained, particularly in the UK. This shortage of housing land is one reason that governments may encourage the use of urban ‘brownfield’ sites for new housing developments. 

More specifically, the UK housing market has experienced a lot of instability in the past few decades – particularly during the 1980s, with a sharp resurgence in volatility in 2007/8. This volatility may have its roots in the moves towards the deregulation of the UK’s financial markets that started in the 1980s. Prior to 1981, the building societies were the key mortgage lenders, and they used the savings deposits of one set of customers to finance the mortgages of another set of customers. But from 1981 onwards, other lenders entered the mortgage market, including high street banks and other financial institutions. Other sources of credit were tapped, not only depositor savings but also short-term money markets. The increased volumes of mortgage lending enabled larger numbers of households to become homeowners; home-ownership was not as dependent on existing wealth/past savings as it had been in the past. In the 1980s and from the late 1990s onwards, increased liquidity in mortgage markets initially fuelled housing market bubbles, but then housing busts were precipitated in the early 1990s and again in 2007/8 as lending institutions became worried about the sustainability of high volumes ofmortgage lending. During the 2007/8 credit crunch in particular, these fears were exarcerbated by concerns about UK banks’ excessive exposure to risky and unbalanced sub-prime mortgage lending (the relatively risky lending to borrowers who are more likely to default on their loans because of their straitened financial circumstances). Poor credit market conditions precipitated increasing pessimism amongst mortgage lenders, risk premiums on mortgage lending were increased and/or more stringent lending criteria were adopted thus constraining the availability of mortgage credit and magnifying house price falls. 

Volatility is also affected by the sensitivity of UK mortgage markets to interest rate changes. A lot ofEuropean countries use fixed rate mortgages and so interest costs on mortgage borrowing change infrequently; in contrast, the high proportion of variable rate mortgages in the UK means that interest costs can change relatively rapidly and this makes UK mortgage holders more sensitive to changes in interest rates overall. UK housing markets were particularly affected by rises in interest rates in the late 1980s, when interest rates were raised in order to curb inflationary pressures throughout the macroeconomy; these rises fed through into higher mortgage rates, stalling housing demand and contributing to large falls in house prices from the early 1990s onwards. Interest rate costs have less relevance for the 2008 housing credit crunch because the Bank of England’s base rate was relatively low and then fell dramatically, though lending pessimism did contribute to relatively large risk premiums on mortgage lending. 

The aim of this chapter is to assess the various determinants of fluctuations in UK housing demand, focussing in particular on credit constraints – including the cost and availability of mortgage financing. But to begin with, we will examine some of the theory explaining owner occupation, i.e. why people choose to buy their own houses to live in, rather than renting. 

## 5.2 The theory

Why do people buy houses? There is the obvious answer: because it’s somewhere to live. But why not just rent? People buy houses ifthey expect their house to gain value over time and/or if living in their own house is cheaper than renting. One of the factors affecting this decision is the affordability of houses. Affordability can be captured by the ratio of average incomes to average house prices but income is not the only financial constraint on home-ownership; credit constraints are also important, as explained below. 

Owner-occupiers face a complex set of decisions when they buy and sell their houses. On the consumption side, houses are durable goods and so exhibit lumpiness: lumpy goods are not easily divisible into small, easily traded quantities. So buying a house involves a once-off purchase of a large ‘bundle’ of services associated not only with shelter but also with a complex mix of necessities and luxuries. Houses are also goods that people expect to consume throughout their lives delivering utility over a long time-horizon. 

The ownership of housing assets is also a key source of household wealth and, similarly mortgage borrowings are a key source of household debt. In accumulating housing wealth, owner-occupiers will try to maximise the capital gains of owning housing assets by timing their housing purchases carefully to take advantage of rises and falls in house prices, hopefully maximising speculative gains. But households face credit constraints: most households do not have sufficient current income and accumulated savings to cover the high cost of housing assets that will deliver utility and returns over a long time-horizon. So financial markets will play an important role in filling the shortfall because households can use borrowings to leverage the purchase of assets that they could not otherwise afford. So for most owner-occupiers, buying a house will accompany a significant set of decisions, i.e. the financial decisions associated with getting a mortgage. 

The extent to which a household is dependent on mortgage borrowings can be measured by the gearing ratio: this captures the proportion of the housing purchase that is funded via mortgage borrowings rather than a household’s income and savings: ifyou want to buy something that costs £100 but you only have £20, then you may be able to borrow £80; in this case your gearing ratio will be four – your borrowings will be four times as much as your own contribution. Gearing means that the purchase of an asset is not constrained by a person’s current income or wealth. 

The extent to which households use their own savings as opposed to gearing their purchases will affect their own stake or ‘equity’ in their housing assets, but it will also have wider implications in terms of housing market volatility. For example, if a house buyer is buying a house for £100,000 and if a building society or bank is prepared to give them a 100% mortgage (i.e. lend them the full £100,000) then the house buyer will have used none ofhis/her own savings and is therefore holding zero equity in the house. In this case, any house price appreciation will come at zero cost (assuming no transactions costs); if the house appreciates and is sold for £120,000, then the home-owner will not have had to use any of their own cash to make the gain; they’ll have £20,000 of pure profit. But gearing purchases is a risky strategy because what happens if house prices fall? Capital gains from house price appreciation will be eroded by house price falls; if a home owner has borrowed £100,000 to buy a house that a year later is worth £80,000 then they’re facing £20,000 of pure loss (excepting any gains made because they haven’t had to pay rent). This situation of negative equity occurs when borrowings exceed the value of an asset. 

Highly geared housing purchases may also have implications if the cost of borrowing rises because, as interest rates rise, an increasing proportion of households will be unable to afford their mortgages and ifthey default on their payments then their houses may be repossessed. These events will have implications for other borrowers too because mortgage lenders will respond to the instability created by negative equity and rising levels of default and repossession by increasing risk premiums on mortgage lending, contributing to further volatility and instability. 

Minsky (1964) analysed the role played by financial constraints in propelling boom–bust cycles and put forward the financial fragility hypothesis, arguing that optimism during expansionary phases contributes to financial bubbles by encouraging excessive lending; however, this excessive lending will also plant the seeds of eventual crisis because, as lending increases to unsustainable levels, defaults will increase concomitantly, triggering pessimism amongst lenders. Risk premiums will also rise and credit constraints will intensify thus precipitating credit crunches and financial crisis. These ideas have much relevance for today’s housing market volatility. 

Muellbauer and Murphy (1997) also analyse the role of financial factors in arguing that, during the UK housing boom of the 1980s, high gearing ratios were more important than the low interest rates. The financial deregulation of mortgage markets had affected gearing ratios by allowing easier access to mortgage financing. With more competition in mortgage lending markets, accompanying increases in the volume of mortgage finance encouraged mortgage lenders to take greater risks in order to attract customers. 100% mortgages based on large multiples of borrowers’ incomes were not uncommon. So households’ equity in their houses decreased and gearing ratios increased. Whilst house prices were rising, homeowners who had high gearing rates on their housing purchases benefited from house price appreciation but for some homeowners those benefits were short-lived; by the 1990s, a large number of unlucky home owners were saddled with negative equity. And rapid house price falls in the UK following the 2007/8 credit crunch contributed to a resurgence of negative equity from 2008 onwards. 

## 5.3 Data

In this chapter we are going to examine the impact of financial factors such as lending and interest rates on housing demand. Using house price growth as our dependent variable, we will regress this on mortgage rates and the growth in mortgage lending. We will also assess the impact of seasonal factors using dummy variables, as will be explained below. 

But where does housing market data come from? Housing market data for a range of countries are published by the OECD (www.oecd.org). For the UK, some housing market data are available via the Office of National Statistics (ONS) website (www.statistics.gov.uk). The building societies are also useful sources of house price data and in our analysis we use house price data from the Nationwide building society to calculate house price growth (see www.nationwide.co.uk). For the financial variables used in this chapter, we have collected data on volumes of mortgage lending from the Council of Mortgage Lenders (CML) (www.cml.org.uk/cml/statistics). Data on mortgage rates comes from the Office of National Statistics (ONS) (www. statistics.gov.uk). 

There are a number of limitations for these data. For the UK overall, it is important to remember that housing markets in England and Wales operate in a different way from housing markets in Scotland and so a lot of British housing market data is really data just for England and Wales. 

Measuring house prices is further complicated by the fact that not all houses are of the same quality. Houses are not homogenous: they are heterogenous goods, i.e. they are essentially different objects of mixed quality. Even houses in the same area may be different things; for example if Mr Bloggs buys a house in the same street as Mr Jones, he may be prepared to pay a lot more for his house if it has a loft conversion or a modern bathroom or kitchen. But he will also have to pay more if Mr Jones bought his house during a depressed period whilst Mr Bloggs bought his house during a boom. House price indices abstract from heterogeneity. This creates measurement errors in housing data. It will also be difficult to separate the impact of general house price inflation from specific increases in the quality ofhousing services reflecting renovations etc. The building societies in particular have recognised this problem and in recent years have started to adopt hedonic pricing methods (Wood, 2005). Hedonic pricing and some of the measurement issues that emerge from the heterogeneity of housing goods are explained in Box 5.1. 

<table><tr><td colspan="2">Box 5.1 House price indices and hedonic pricing</td></tr><tr><td colspan="2">Sources of house price data</td></tr><tr><td colspan="2">Wood (2005) has identified at least seven main house price indices for the UK:The Land Registry collects statistics on:</td></tr><tr><td colspan="2">1. average prices from records on all completed house sales.Mortgage lenders also collect data on house prices from the mortgage applications of their customers. The Office of the Deputy Prime Minister collates these house price data from its Survey of Mortgage Lenders (SML) to construct two indices including:</td></tr><tr><td colspan="2">2. a simple average index; and</td></tr><tr><td colspan="2">3. a mix-adjusted index – which is a weighted average of house prices from a representative selection of house sales.Building societies collect house price data too, for example:</td></tr><tr><td colspan="2">4. the Halifax index; and</td></tr><tr><td colspan="2">5. the Nationwide index.Building societies data are collected from mortgage lending records but building society survey data was more representative 25 years ago than it is today because, as explained above, building societies are no longer the only major mortgage lenders. Today, many other types of financial institution are involved with mortgage lending and if there are significant differences in the profiles of the average bank mortgage-holder versus the average building society mortgage-holder, then the building society data will suffer from sampling bias.House price indices are also generated by real estate agents including the:</td></tr><tr><td colspan="2">6. Hometrack index; and</td></tr><tr><td colspan="2">7. Rightmove index.</td></tr><tr><td colspan="2">Hedonic pricing</td></tr><tr><td colspan="2">The collection of these house price data is complicated by the fact that houses are heterogeneous. So how do economists separate the influences of quality difference from house prices inflation? One way is to usehedonic pricingmethodologies to compile house price data controlling for quality improvements. Hedonic pricing builds upon the idea that different characteristics of a good or service impact differently on the pleasure of consumption. For housing it involves econometric analysis to assess the value of certain property characteristics (e.g. a large garden, a modern kitchen). Prices are then adjusted to remove the idiosyncratic influence of these sources of heterogeneity to give an unbiased estimate of the ‘raw’ price. In theFinancial Times(30 June 2004), hedonic prices are described which show that whilst the price of shelter rose from the late 1990s,</td></tr></table>

the price of desirable attributes did not. This suggests that general house prices inflation had a greater impact on house prices than quality improvements. 


Summary of some web links for housing market data:


<table><tr><td>Council of Mortgage Lenders (CML)</td><td>www.cml.org.uk</td></tr><tr><td>Land Registry</td><td>www.landreg.gov.uk</td></tr><tr><td>Office of the Deputy Prime Minister (ODPM)</td><td>www.odpm.gov.uk</td></tr><tr><td>Office of National Statistics (ONS)</td><td>www.statistics.gov.uk</td></tr><tr><td>Nationwide</td><td>www.nationwide.co.uk/hpi/</td></tr></table>

What do the data show about housing demand in the UK? Figure 5.1 plots Nationwide data on UK house prices alongside data on mortgage lending from the CML over the period 1975Q1 to 2008Q1. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/15ed3ca6b7ef27fca61566d70ad0e9b66e95351537c99506417657e2cb51bc7c.jpg)



Source: Nationwide Building Society, CML.



Figure 5.1 UK house prices and mortgage lending, 1975Q1 to 2008Q1


Figure 5.1 shows that there has been a sustained upward trend in house prices from the 1970s through to early 2008; this is matched by exponential rises in mortgage lending suggesting that house prices are positively associated with mortgage lending. At the end of the period, there were strong signs that these trends were reversing from 2008 onwards. 

Using these data patterns as a basis for our empirical model, we will assess the relationship between house prices, mortgage lending growth and mortgage rates using the following data: 

<table><tr><td>Variable</td><td>Source</td><td>Website</td></tr><tr><td>House prices</td><td>Average Price for ‘All Houses’ (from mortgage application records)</td><td>www.nationwide.co.uk/hpi/downloads/UK_house_price_since_1952.xls</td></tr><tr><td>Mortgage lending</td><td>ONS data on composite Banks and Building Societies mortgage rate. From Economic Trends Annual Supplement (AJVT)</td><td>www.statistics.gov.uk</td></tr><tr><td>Mortgage rates</td><td>All loans for house purchases by mortgage lenders</td><td>www.cml.org.uk/cml/statistics</td></tr></table>


The house price and mortgage lending variables have been deflated using the consumer price index from the ONS (Economic Trends Annual Supplement’s Table 3.2, variable D7BT). We will also use dummy variables to capture seasonal influences, as explained below. 


## 5.4 Empirical methods and results

In this empirical section we analyse some of the factors influencing UK housing demand, as measured by house prices. In the theoretical section we explained that housing demand is determined by a number of potential explanatory variables. The rise in house prices depicted in Figure 5.1 has outstripped rises in household disposable incomes and has coincided with the declining affordability of housing. So rises in affordability do not fully explain the pronounced boom–bust cycles in UK house prices since the 1980s. 

In exploring these boom–bust cycles, as is common in econometric analysis, we will have to abstract from the complexity of relevant factors to concentrate on what we judge to be the most important factors. Building upon some of the theoretical ideas outlined above, we will examine the role of credit constraints and mortgage lending. Financial deregulation from the 1980s onwards boosted gearing ratios and led to increased mortgage lending on riskier terms; the increased risk may have translated in a greater probability of default. More recently, deregulated financial markets and the growth of complex financial products again encouraged lenders to engage in risky over-lending, encouraging house prices to accelerate at unprecedented rates throughout the late 1990s through to the 2000s only to collapse in the early 1990s and from 2008 onwards. These factors may help to explain destabilising boom–bust cycles in house prices. 

Specifically to assess the impact of financial factors, we collected 45 quarterly observations for the UK between 1995Q1 and 2006Q1 using the data sources outlined above and we use these data to estimate the following empirical model: 

$$
h _ {t} = \alpha + \beta_ {1} l _ {t} + \beta_ {2} r _ {t} + \beta_ {3} Q 1 _ {t} + \beta_ {4} Q 2 _ {t} + \beta_ {5} Q 3 _ {t} + \varepsilon_ {t}\tag{5.1}
$$

where h is house prices (logged); l is mortgage lending (logged); r is the mortgage rate; Q1, Q2 and Q3 are dummy variables (capturing shifts in means for the Winter, Spring and Summer quarters respectively), and ε is a random error term. 

Our SRF will be: 

$$
h _ {t} = \hat {\alpha} + \hat {\beta} _ {1} l _ {t} + \hat {\beta} _ {2} r _ {t} + \hat {\beta} _ {3} Q 1 _ {t} + \hat {\beta} _ {4} Q 2 _ {t} + \hat {\beta} _ {5} Q 3 _ {t} + \hat {\varepsilon} _ {t}\tag{5.2}
$$

In addition to the financial factors discussed above, we have also introduced seasonality into our model and this is captured using seasonal dummy variables, as explained in Box 5.2. 

## Box 5.2 Using seasonal dummies to capture seasonality

Dummy variables are categorical variables and are often used to capture non-measurable influences, for example the effect of seasonal factors on housing demand. Dummy variables are binary – they take the value 1 if something is true and the value 0 if something is false. For example, in the model below Q1 will capture differences in house prices in the winter quarter. We introduce a winter quarter dummy variable and ask the question for each observation in our data set: is this observation in the winter quarter? If the observation is in the winter quarter then we set Q1 = 1; if not, we set Q1 = 0. So for all observations taken from winter quarters Q1 = 1 and for spring, summer and autumn quarters Q1 = 0. 

The following extract from our data file shows how the dummy variables are constructed in practice. 

<table><tr><td></td><td>Q1</td><td>Q2</td><td>Q3</td><td>Q4</td></tr><tr><td>1975 Q1</td><td>1</td><td>0</td><td>0</td><td>0</td></tr><tr><td>1975 Q2</td><td>0</td><td>1</td><td>0</td><td>0</td></tr><tr><td>1975 Q3</td><td>0</td><td>0</td><td>1</td><td>0</td></tr><tr><td>1975 Q4</td><td>0</td><td>0</td><td>0</td><td>1</td></tr><tr><td>1976 Q1</td><td>1</td><td>0</td><td>0</td><td>0</td></tr><tr><td>1976 Q2</td><td>0</td><td>1</td><td>0</td><td>0</td></tr><tr><td>1976 Q3</td><td>0</td><td>0</td><td>1</td><td>0</td></tr><tr><td>1976 Q4</td><td>0</td><td>0</td><td>0</td><td>1</td></tr><tr><td>1977 Q1</td><td>1</td><td>0</td><td>0</td><td>0</td></tr><tr><td colspan="5">etc. etc.</td></tr></table>

With dummy variables it is easy to fall into the dummy variable trap. Imagine that we had included all four seasonal dummies as well as an intercept into the SRF set out in Equation (5.2). The most obvious problem is one of interpretation. What would the parameters on Q1, Q2, Q3 and Q4 mean? These parameters are designed to capture all the constant factors affecting house prices in a given quarter. So what is the intercept capturing if we have four quarterly dummies in our model? More importantly, if we include all of the seasonal dummies then we will have a perfect correlation of +1 between the intercept and the sum of the dummies. To explain this: the intercept in a regression model is always a constant. The four quarterly dummy variables will always sum to 1 because the seasonal categories are mutually exclusive and exhaustive. (Ignoring the weather, officially it is always eithe winter or spring or summer or autumn; it is never more than one of these at once.) So the sum of the dummies will be a constant; because the intercept is also a constant, the correlation coefficient between them will be exactly equal to +1. This means that it will be impossible empirically to separate the influences of the intercept and dummies. 

In statistical terms, the dummy variable trap emerges because of perfect multicollinearity between the intercept and the sum of the four quarterly dummies. Multicollinearity is the general term for the existence of linear associations between explanatory variables. With imperfect multicollinearity the correlation coefficients between variables are high but less than 1 in absolute terms. With imperfect multicollinearity estimation will be less accurate and this may affect our inferences. Perfect multicollinearity is the extreme version of multicollinearity and occurs when there are perfect linear associations between explanatory variables and/or groups of explanatory variables, i.e. when the correlation coefficients between them are exactly equal to ±1. With perfect multicollinearity (e.g. in the case of the dummy variable trap), OLS will not work at all because when there is a perfect linear association between groups of explanatory variables it is impossible to separate their influences: variances will be infinitely large and confidence intervals will be infinitely wide. And your econometrics software will give you an error message! 

To escape this dummy variable trap for this analysis, we will have to drop one dummy variable and use its corresponding set of observations as our reference category. For our estimations we will use Q4 (autumn) as the reference category. The intercept then captures the impact of constant factors in autumn. The parameter estimates on the other dummies will represent shifts in the intercepts for other seasons. Another solution could be to drop the intercept and have four quarterly dummies, with the parameters on each representing the intercept for the relevant quarter, but this would complicate the interpretation of $R ^ { 2 }$ and for this reason it is better to keep one category as a reference category. 

What does this imply for our model? We are estimating the following model: 

$$
h _ {t} = a + \beta_ {1} I _ {t} + \beta_ {2} r _ {t} + \beta_ {3} Q 1 _ {t} + \beta_ {4} Q 2 _ {t} + \beta_ {5} Q 3 _ {t} + \varepsilon_ {t}\tag{5.1}
$$

where h is house prices (logged), l is mortgage lending (logged), r is the mortgage rate, Q1, Q2 and Q3 are dummy variables (capturing shifts in means for the Winter, Spring and Summer quarters respectively), and ε is a random error term. 

As explained above, we are using Q4 as our reference category and so the intercept from the model is capturing the constant factors in Q4. Different combinations of values on the dummy variables will affect the intercept of this model as follows: When it’s autumn, i.e. when $\mathtt { Q 1 } = \mathtt { Q 2 } = \mathtt { Q 3 } = 0$ 

$$
\rightarrow h _ {t} = a + \beta_ {1} I _ {t} + \beta_ {2} r _ {t} + \varepsilon_ {t}\tag{5.1a}
$$

When it’s winter, i.e. when Q1 = 1 and Q2 = Q3 = 0: 

$$
\rightarrow h _ {t} = (a + \beta_ {3}) + \beta_ {1} I _ {t} + \beta_ {2} r _ {t} + \varepsilon_ {t}\tag{5.1b}
$$

When it’s spring, i.e. when Q2 = 1 and Q1 = Q3 = 0 

$$
\rightarrow h _ {t} = (a + \beta_ {4}) + \beta_ {1} I _ {t} + \beta_ {2} r _ {t} + \varepsilon_ {t}\tag{5.1c}
$$

When it’s summer, i.e. when Q3 = 1 and Q1 = Q2 = 0 

$$
\rightarrow h _ {t} = (a + \beta_ {5}) + \beta_ {1} I _ {t} + \beta_ {2} r _ {t} + \varepsilon_ {t}\tag{5.1d}
$$

So we’ve estimated four different models in one go! 

Notice that the intercept is being augmented in each case – the parameters on the dummy variables are shifting the intercept upwards. We aren’t trying to capture shifts in slopes in this example and the mean of the product of the slope parameter estimates and the explanatory variables is constant across all seasons.<sup>1</sup> The average for a given season, e.g. winter is given by: 

$$
h _ {t} = (\bar {a} + \bar {\beta} _ {3}) + \beta_ {1} \bar {I} _ {t} + \beta_ {2} \bar {r} _ {t} + \varepsilon_ {t}\tag{5.3a}
$$

The mean of a constant is just that constant, and this will be the same for all four seasons. It follows that the mean of the parameter on an additive dummy is just that parameter. The mean of the error is zero and so for winter we can capture the difference between winter’s mean and the overall means as follows: 

$$
h _ {t} - a - \beta_ {1} \bar {l} _ {t} - \beta_ {2} \bar {r} _ {t} = \beta_ {3}\tag{5.3b}
$$

In this way, the seasonal dummies are capturing the shifts in the means of house prices as the seasons change. To summarise: the additive dummy variables are capturing the differences in group means across the four seasons. 

The main innovation of this chapter is, for the first time in this book, we have more than one explanatory variable; in fact we have five explanatory variables (k = 5). This means that we will have to use multiple regression analysis (MRA) to analyse house prices. One of the main advantages of MRA is that it allows us to avoid omitted variable bias by specifying our empirical models to include as many variables as are indicated by the relevant theory. This is useful in the context of our model of house prices because we have identified a number of explanatory variables that might capture house price fluctuations. 

MRA also involves an extension of the various tests and measures used for SRA and so the coefficient of determination, our measure of the goodness of fit, must be adapted to account for the presence of more than one explanatory variable, as explained in Box 5.3. 

## Box 5.3 Multiple regression analysis (MRA)

Multiple regression analysis (MRA) involves the extension of the OLS techniques out lined in previous chapters to empirical models that have more than one explanatory variable. This means that we can separate out the influences of different explanatory variables; the parameter on one explanatory variable will be capturing the impact of that variable holding the other explanatory variables constant. This allows us to capture the direct effect of each explanatory variable more effectively; we are controlling for the influences of the other explanatory variables included in the model. Whilst the mathematics of multiple regression are more complex than for simple regression, in practice the techniques are much the same and the computer packages are programmed do all the extra work. It’s not a good idea to try to do multiple regressions “by hand” unless you have lots of spare time! 

## Measuring goodness of fit

In simple regression we were using just one explanatory variable. In multiple regression we may use many more. What implications does this have for the coefficient of determination – our measure of goodness of fit? As explained in Chapter 1, in simple regression analysis there is a straightforward association between the correlation coefficient – r and the coefficient of determination – $R ^ { 2 }$ . For MRA, this relationship is more complex and $R ^ { 2 } \neq r ^ { 2 } :$ r will just capture the two-way correlation between Y and one explanatory variable; r will not control for the indirect influences of other explanatory variables. On the other hand, $R ^ { 2 }$ is capturing the collective association between Y and all the explanatory variables. So, whilst $R ^ { 2 } \neq r ^ { 2 }$ it can still be calculated using the following formula: 

$$
R ^ {2} = \frac {E S S}{T S S} = \frac {\sum (\hat {Y} - \bar {Y}) ^ {2}}{\sum (Y _ {i} - \bar {Y}) ^ {2}}\tag{1.12 from Chapter 1}
$$

Another complication that applies to MRA is that each time we add a new explanatory variable, our goodness of fit necessarily increases because we are adding in an additional source of ‘explained’ variance and so $R ^ { 2 }$ will inevitably increase. This means that, all things being equal, $R ^ { 2 }$ in models with lots of explanatory variables will be greater than the $R ^ { 2 }$ in models with few explanatory variables, even though the latter may have more real substance. At the extreme (degrees of freedom permitting) that might tempt us into data mining i.e. just adding in as many variables as possible without much consideration of their theoretical underpinnings. One way to correct for the ‘size’ of a model is to use $\bar { R } ^ { 2 }$ (the adjusted $R ^ { 2 } )$ . This is an adjustment using degrees of freedom as follows: 

$$
\bar {R} ^ {2} = 1 - \left[ (1 - R ^ {2}) \times \frac {n - 1}{n - k - 1} \right]\tag{5.4}
$$

where k is the number of explanatory variables and n is the number of observations in the sample. This formula ensures that, in a model with many explanatory variables (and lots of slope parameters), the $R ^ { 2 }$ will be adjusted downwards accordingly; in this way $\bar { R } ^ { 2 }$ penalises the inclusion of ‘trash’ variables. 

In the preceding chapters on simple regressions, we used either the relatively unwieldy method of running regressions using Excel or the definitely unwieldy method of running regressions by hand. But for multiple regression analysis it is quicker and easier to use tailor-made econometrics packages. With these packages, running a regression just involves typing a list ofvariable codes and clicking on a couple of buttons. The package automatically produces a table of estimation results together with a wide range of accompanying statistics that can be cut-and-pasted directly into your various documents. Another key advantage of such packages is the detail and sophistication of the econometric techniques embedded within them, including a wide range of diagnostic and corrective tools that are not available via spreadsheet packages. 

In this chapter we introduce running regressions using the econometrics package EViews. With EViews, there are a number of data input options including typing the data in by hand, but the easiest method is probably to collect data in Excel and then cut and paste across into EViews. Running our estimation of Equation (5.3a) using EViews gives results as summarised in Table 5.1 – a summary of the EViews printout. 


Table 5.1 Summary of EViews printout


<table><tr><td colspan="5">Dependent Variable: Real house prices (logged)</td></tr><tr><td colspan="5">Method: Least Squares</td></tr><tr><td colspan="5">Sample: 1995Q1 2006Q1</td></tr><tr><td colspan="5">Included observations: 45</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>2.880</td><td>1.076</td><td>2.675</td><td>0.011</td></tr><tr><td>Mortgage lending (logged)</td><td>0.854</td><td>0.089</td><td>9.650</td><td>0.000</td></tr><tr><td>Mortgage rate</td><td>-0.004</td><td>0.033</td><td>-0.112</td><td>0.912</td></tr><tr><td>Q1</td><td>0.203</td><td>0.062</td><td>3.283</td><td>0.002</td></tr><tr><td>Q2</td><td>-0.080</td><td>0.061</td><td>-1.311</td><td>0.197</td></tr><tr><td>Q3</td><td>0.009</td><td>0.060</td><td>0.145</td><td>0.886</td></tr><tr><td>R-squared</td><td>0.86</td><td>F-statistic</td><td></td><td>47.74</td></tr><tr><td>Adjusted R-squared</td><td>0.84</td><td>Prob(F-statistic)</td><td></td><td>0.00</td></tr><tr><td>Sum Squared residuals</td><td>0.76</td><td></td><td></td><td></td></tr></table>

You will notice that there is a lot of detail in this table. For the moment, we are just going to concentrate on the t tests, the adjusted $R ^ { 2 }$ (explained above) and some related statistics.<sup>2</sup> But the results from the estimation of the SRF can be summarised by the following equation: 

$$
\begin{array}{r l r l r l r} \hat {h} _ {t} = & 2. 8 8 0 & + 0. 8 5 4 l & - 0. 0 0 4 r & + 0. 2 0 3 Q 1 & - 0. 0 8 0 Q 2 & + 0. 0 0 9 Q 3 \\ & (1. 0 7 6) & (0. 0 8 9) & (0. 0 3 3) & (0. 0 6 2) & (0. 0 6 1) & (0. 0 6 0) \\ & t = 2. 6 7 5 & t = 9. 6 5 0 & t = - 0. 1 1 2 & t = 3. 2 8 3 & t = - 1. 3 1 1 & t = 0. 1 4 5 \\ & p = 0. 0 1 1 & 0. 0 0 0 & 0. 9 1 2 & 0. 0 0 2 & 0. 1 9 7 & 0. 8 8 6 \end{array}\tag{5.5}
$$

## Single hypothesis test

Here we will use a two-tailed t test to test the nulls that the parameter on the intercept is equal to zero, i.e.: 

$$
\begin{array}{l} H _ {0}: \alpha = 0 \\ H _ {1}: \alpha \neq 0 \end{array}
$$

and for the slope parameters that each individual parameter on each explanatory variable is equal to zero, i.e.: 

$$
\begin{array}{l l l l l} H _ {0}: \beta_ {1} = 0 & H _ {0}: \beta_ {2} = 0 & H _ {0}: \beta_ {3} = 0 & H _ {0}: \beta_ {4} = 0 & H _ {0}: \beta_ {5} = 0 \\ H _ {1}: \beta_ {1} \neq 0 & H _ {1}: \beta_ {2} \neq 0 & H _ {1}: \beta_ {3} \neq 0 & H _ {1}: \beta_ {4} \neq 0 & H _ {1}: \beta_ {5} \neq 0 \end{array}
$$

These hypotheses for the slope parameters can be summarised as: 

$$
H _ {0}: \beta_ {k} = 0
$$

$$
H _ {1}: \beta_ {k} \neq 0\tag{5.6}
$$

We have 39 degrees of freedom in our t test $\left( n - k - 1 = 4 5 - 5 - 1 \right)$ and from statistical tables we get the critical values for t at a 5% significance level of $t _ { \mathrm { c r i t } } \approx 2 . 0 2$ . So our decision rule is: 

$i f \left| \hat { t } \right| > 2 . 0 2 ,$ , then reject H<sub>0</sub>; $i f \left| \hat { t } \right| < 2 . 0 2$ then do not reject $H _ { 0 }$ 

A quicker alternative would be to use a decision rule based around the $\boldsymbol { p }$ values, as explained in Chapters 1 and 4. Our decision rule for a 5% significance level is: 

$f p < 0 . 0 5 ,$ , then reject $H _ { 0 } ; i f p > 0 . 0 5$ then do not reject $H _ { 0 }$ 

This is equivalent to rejecting the null $\mathrm { i f } \ \lvert \hat { t } \rvert > t _ { \mathrm { c r i t } } ( 5 \% ) . ^ { 3 }$ Using these decision rules: for the intercept, mortgage lending and the winter dummy, we can reject $H _ { 0 } ;$ for the parameters on the mortgage rate and the other seasonal dummies, we cannot reject $H _ { 0 }$ 

How do our statistical findings link with our theoretical analysis? For mortgage lending there is a positive and significant association: rising house prices are associated with rises in mortgage lending. This is consistent with the assertion that increases in mortgage lending will foster house price bubbles and conversely, that credit constraints will precipitate house price slumps. This may reflect the gearing and credit constraints explained in the theoretical section: higher volumes of lending allow owner-occupiers to gear-up their property purchases and this fuels rising house prices and house price bubbles. For mortgage rates, there is a negative association – as hypothesised but this is insignificantly different from zero at a 5% significance level (i.e. with a 95% confidence interval). This is consistent with our theoretical analysis to the extent that rising mortgage rates are associated with dampened demand for housing but the effect is not large. 

As for the dummy variables, the parameter on Q1 is positive and significantly different from zero at a 5% significance level and this suggests that the mean house price in Q1 is significantly higher, at a 5% significance level, than the mean house price in the other quarters. For the other quarters, there are no significant differences in the group means. 

## Testing for a unitary elasticity

The t tests discussed above are testing the null hypothesis that mortgage financing has no effect on house prices. However, if we want to make more specific hypotheses about the magnitude of responses, we can adapt the hypotheses within our t tests. We have logged both the house price and mortgage lending variable $\mathbf { s o } ,$ as explained in Chapter 3, this means that our parameter on the mortgage lending variable is capturing the elasticity of house prices with respect to mortgage lending. It will capture the percentage increase in house prices associated with a percentage increase in mortgage lending. If we want to find out whether or not this is a unitary elasticity (an elasticity equal to one), i.e. whether or not a 1% rise in mortgage lending is associated with a proportional 1% rise in house prices, then we can test this using a one-tailed t test as follows: 

$$
\begin{array}{l}H _ {0}: \beta_ {1} = 1\\H _ {1}: \beta_ {1} <   1\\\rightarrow \hat {t} = \frac {\hat {\beta} - 1}{s e (\hat {\beta})} = \frac {0 . 8 5 4 - 1}{0 . 0 8 9} = - 1. 6 4\end{array}\tag{5.7}
$$

For a one-tailed t test with a 5% significance level $( d f { = } 3 9 ) , t _ { \mathrm { c r i t } } { \approx } - 1 . 6 8$ . So we do not reject $H _ { 0 }$ and conclude that whilst there is a significant association between house prices and mortgage lending the elasticity is insignificantly different from one. This suggests that there may be an elastic response of house prices to mortgage lending but the decision is marginal; note that with a different significance level, the inferences would be different, e.g. with a 10% significance level (i.e. a 90% confidence interval) $t _ { \mathrm { c r i t } } { \approx } - 1 . 3 0$ and we would reject $H _ { 0 } .$ . In this case, our inferences are sensitive to the significance level used. This underscores the fact that, in any interpretation of statistical results, the researcher must remember the trade-offs between Type I and Type II errors (as summarised in Chapter 1). 

## Goodness of fit

With MRA analysis our individual t tests, being single hypothesis tests, cannot give us information about the contribution ofall our explanatory variables as a group and so assessing goodness of fit becomes slightly more complicated. Also individual scatter plots of our dependent variable against each of our explanatory variables would be unwieldy and in any case would not control for the contribution ofother explanatory variables. So in MRA it is more usual to get a visual impression about the $\operatorname { \mathrm { \Sigma } } _ { \mathrm { f i t } } ^ { \mathrm { \Sigma } } ,$ of our model by plotting actual (i.e. observed) values against our predicted or fitted values from the multiple regression model. Figure 5.2 shows the plot of actual versus fitted values for our SRF as summarised in Equation (5.3a). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/d58cc439137acf0ea32d47ed9e3907c51e04f7a2c7c91728c93ea2a0d7646d33.jpg)



Figure 5.2 Actual vs. fitted values from estimation of Equation (5.3a)


This plot suggests a broad correspondence between observed and predicted house prices but there are a number of periods when our estimated model is consistently under-predicting or over-predicting house prices; we seem to have some systematic patterns in our residuals. This reflects a problem of autocorrelation. Exploring autocorrelation in depth is beyond the scope of this chapter.<sup>4</sup> 

As for the goodness of fit, if we want an objective measure of goodness of fit in multiple regression analysis we use the $\bar { R } ^ { 2 }$ – the adjusted $R ^ { 2 }$ . As explained in Box 5.3, $\bar { R } ^ { 2 }$ is weighted to take account of the number of explanatory variables in an empirical model, ensuring that a model with lots ofexplanatory variables does not necessarily give a better goodness of fit than a model with very few explanatory variables. Applying the formula for $\bar { R } ^ { 2 }$ from (5.3a) to our model gives: 

$$
\begin{array}{r l} & {\bar {R} ^ {2} = 1 - (1 - R ^ {2}) \times \frac {n - 1}{n - k - 1}} \\ & {\qquad = 1 - \left[ (1 - 0. 8 6) \times \frac {4 5 - 1}{4 5 - 5 - 1} \right] = 0. 8 4} \end{array}\tag{5.8}
$$

This is consistent with the $\bar { R } ^ { 2 }$ recorded underneath the ordinary $R ^ { 2 }$ in Table 5.1 – the EViews results table. It indicates that, after adjusting for the contribution of all the explanatory variables, about 84% of the variability in real house prices can be captured by the variability in the explanatory variables together. 

Putting together the high adjusted $R ^ { 2 }$ and the fact that some of the slope parameters are significantly different from zero indicates that house prices and the various explanatory variables are varying together; there is some sort of statistical relationship between the variables. 

But what if the researcher wants to find out if this overall relationship is significant? In this case, he/she will use the F test of overall explanatory power, as explained in Box 5.4. We can also test hypotheses about sub-groups of variables (in this case we will try the parameters on the dummy variables), using the F test of restrictions. This is also explained in Box 5.4. 

Overall, our results do confirm that there is a significantly positive relationship between house prices and mortgage lending, though the impact of mortgage rates seems to be less important. There are however important caveats. The systematic pattern in the residuals, as noted above, may be a sign of potentially serious problems with the specification of our model. 

There are some specific disadvantages of MRA that emerge because we are estimating more parameters than we would in a SRA. One problem, mentioned above, is imperfect multicollinearity. As explained above, imperfect multicollinearity occurs when the correlation coefficients are relatively high but less than 1 in absolute value terms. Imperfect multicollinearity is not a violation ofa Gauss–Markov condition. Our OLS estimators will still be BLUE but the overall accuracy of estimation procedures will be compromised. OLS will give us definite results; but these results may not be very accurate because we will be estimating our parameters less precisely: the variances and standard errors of our parameter estimates will be higher, our confidence intervals will be wider and we will be more likely to retain a false $H _ { 0 } ,$ i.e. we will be more prone to Type II errors. 

A related problem is the problem of (imperfect) micronumerosity. Micronumerosity is the problem of having a relatively small number of degrees of freedom; for example if we have 10 observations and 6 explanatory 

## Box 5.4 Joint hypothesis tests

Building up from earlier discussions of Ftests in Chapters 1 and 4, the F test of explanatory power can be conducted using the following null and alternative: 

$$
H _ {0}: \beta_ {1} = \beta_ {2} = \beta_ {3} = \beta_ {4} = \beta_ {5} = 0
$$

$H _ { 1 } \colon$ At least one of the slope parameters is not equal to zero 

The F test of explanatory power (introduced in Chapters 1 and 4) tests the joint restrictions that all slope parameters are jointly equal to zero. The formula is used in this example as follows: 

$$
F (k, n - k - 1) = \frac {(R ^ {2} / k)}{(1 - R ^ {2}) / (n - k - 1)} = \frac {(0 . 8 6 0 / 5)}{(1 - 0 . 8 6 0) / (4 5 - 5 - 1)} = 4 7. 9 1\tag{5.9}
$$

where k is the number of explanatory variables and n = number of observations. Broadly the same result is reported in Table 5.1 – EViews printout as the ‘F-statistic’, with its associated $p$ value of 0.00 (discrepancies reflect rounding differences). Given that $p { < } 0 . 0 0$ we can reject $H _ { 0 }$ at a 5% significance level and conclude that there is a significant association between house prices and all our explanatory variables, i.e. our model as a whole. The variability captured by our explanatory variables is a statistically significant proportion of total variability in our house price variable. We would come to the same conclusion if we looked up our critical value for the F statistic using statistical tables. From these tables (using a 5% significance level), $F _ { \mathrm { c r i t } } ( 5 , 3 9 ) \approx 2 . 4 5$ . This is less than 47.91 so, again, we reject ${ \sf H } _ { 0 }$ 

## The F test of restrictions

We can also use F tests to test sub-sets of restrictions, for example if we wanted to test the importance of groups of variables. The formula for the F test of restrictions is: 

$$
F (d, n - k _ {\mathrm{u}} - 1) = \frac {(R S S _ {\mathrm{r}} - R S S _ {\mathrm{u}}) / d}{R S S _ {\mathrm{u}} / (n - k _ {\mathrm{u}} - 1)}\tag{5.10}
$$

where the subscripts r and u denote the restricted and unrestricted models respectively, kis the number of explanatory variables, n is the number of observations and dis the number of parameters restricted. 

To explain this formula intuitively: it is capturing changes in RSS – the residual sum of squares. When we ‘restrict’ a model, i.e. by imposing restrictions upon the estimates of parameters within our model, then our estimations are less likely to fit the real world neatly. Statistically, this translates into a fall in our goodness of fit and a rise in our residuals and thus an increase in the RSS. The F test of restrictions is designed to capture the relative size of this increase in RSS by comparing the RSS in the ‘unrestricted’ model with the RSS in the‘restricted’ version; the restricted model will incorporate the null hypothesis about the parameter values. 

Using the example in this chapter to illustrate, if we wanted to test that the seasonal influences were zero, i.e. that the constant factors were more or less the same for all quarters, we could use an $F$ test of restrictions to compare the $R S S _ { \mathrm { u } }$ (RSS from the unrestricted model with the seasonal dummies in) with the RSS (RSS from a restricted model with the dummies out). If the RSS increases by a significant amount when the dummies are ignored, then this suggests the dummies are important variables and should be left in. On the other hand if the increase in the RSS is insignificant when the dummies are ignored, then this suggests that the dummies do not add explanatory power and could be left out. 

To illustrate, we will test a null that incorporates our restriction that the parameters on the dummies are jointly equal to zero i.e.: 

$$
H _ {0}: \beta_ {3} = \beta_ {4} = \beta_ {5} = 0
$$

$H _ { 1 } \colon$ At least one of the parameters on the seasonal dummies is not equal to zero 

When we impose the restriction that the parameters on the dummies are jointly equal to zero we will estimate a restricted model of the following form: 

$$
h _ {t} = a + \beta_ {1} I _ {t} + \beta_ {2} r _ {t} + \varepsilon_ {t}\tag{5.11}
$$

Our unrestricted model, in which the parameters on the dummies can take whatever values fit the data best, is Equation (5.3a). 

Estimating Equation (5.11) using EViews we get $R S S _ { \mathrm { r } } { } = 1 . 1 4 5$ . We have already run Equation (5.3a) above and the $R S S _ { \mathrm u }$ from this is recorded in Table 5.1 as ‘Sum squared residuals’ so $R S S _ { \mathrm { u } } = 0 . 7 6 2$ . We have restricted three parameter values and so $d { \boldsymbol { = } } 3$ Incorporating these numbers into our formula we calculate: 

$$
F (d, n - k _ {\mathrm{u}} - 1) = \frac {(R S S _ {\mathrm{r}} - R S S _ {\mathrm{u}}) / d}{(R S S _ {\mathrm{u}}) / (n - k _ {\mathrm{u}} - 1)} = \frac {(1 . 1 4 5 - 0 . 7 6 2) / 3}{0 . 7 6 2 / (4 5 - 5 - 1)} = 6. 5 3\tag{5.12}
$$

In practice, EViews will do all the mathematical work for us. We can estimate the unrestricted model by using the EViews toolbar to click through ‘View – Coefficient Tests – Redundant Variables’, inputting Q1, Q2 and Q3 as our ‘redundant variables’. Then EViews will show an output table with the estimated F together with its associated p value. The Fwill be more-or-less the same as the one calculated in Equation (5.12) (any small discrepancies will reflect rounding differences). So from EViews we get the p value from the F test in Equation (5.12), i.e. $p { = } 0 . 0 0 1$ . So $p { < } 0 . 0 5$ and we can reject $H _ { 0 } .$ At a 5% significance level, the dummy variables as a group are contributing significant explanatory power to our model of house prices. 

This result implies that the residuals do increase markedly when the seasonal dummies are dropped: the increase in the RSS is relatively large when we impose the restriction that the parameters on the seasonal dummies are zero, and our t tests of individual significance suggest that this mainly reflects the influence of shifting house prices in Q1. 

variables (6 slope parameters and 1 intercept parameter to estimate), then we will have only 3 degrees of freedom left (i.e. not many).<sup>5</sup> Imperfect micronumerosity has much the same consequences as imperfect multicollinearity: variances and standard errors are larger, confidence intervals are wider and our hypothesis testing is more prone to Type II errors. 

Just as there is an extreme version ofmulticollinearity (perfect multicollinearity) so there is an extreme version of micronumerosity: perfect micronumerosity. This occurs when we have fewer observations than parameters to estimate and so we have no degrees of freedom. With perfect micronumerosity, as with perfect multicollinearity, there will be no solution using OLS estimation. Again our software will send us an error message to remind us to check our data set! 

## 5.5 Implications and conclusions

It is important in any empirical analysis to state the limitations of the findings. This is just our first illustration of MRA and so we have kept it simple by focussing on just a sub-set of possible explanatory variables. We have also neglected the influence of lags and in the chapter exercises we make some suggestions about how to introduce lags into an empirical model. There may be other important variables, for example changes in disposable income, demographic factors, government policy etc. etc. Furthermore, findings for other countries and/or time periods might be different, reflecting institutional differences and structural changes. 

An additional technical issue to keep in mind is that we haven’t tested for violations of the Gauss–Markov assumptions outlined in Chapter 1. Until we have done these tests, we cannot be sure that our OLS estimations are giving reliable and accurate results. For this analysis, there were hints of a potential problem with our residuals when we plotted our actual versus fitted values (see Figure 5.2). How to detect and correct potential violations of Gauss– Markov assumptions is explained in more detail in the following chapters. 

These caveats stated, overall the results from this chapter suggest that there was a significant positive association between mortgage lending and house prices in the UK over the period 1995 to 2006. We identified an elastic response with rises in mortgage rates matched by proportionate rises in house prices. The impact of seasonal changes also had an impact. On the other hand, the impact of fluctuations in mortgage rates was insignificant. 

Overall, if these findings are robust, then there are some important policy implications. The fact that mortgage rates have an insignificant impact suggests that more emphasis could be placed on constraining lending excesses during boom periods in order to avoid credit crunches and housing crashes when those boom periods end. Financial deregulation during the 1980s means that mortgage lenders are now more ‘self-regulating’ than they were in the 1970s; but, as the 2007/8 sub-prime mortgage crisis has amply illustrated, private financial institutions do not always have the incentives or information to manage their lending policies prudently. Public institutions can play an important role in smoothing volatility. 

In containing the UK credit crunch of2007/8 for example, the Bank ofEngland responded by providing facilities to swap risky mortgages for Treasury bonds, in this way injecting liquidity into the system. Regulatory authorities also have the potential to play a key role in the management of financial crises. The UK’s Financial Services Authority (FSA) – a non-governmental institution given statutory powers to regulate the financial services industry including mortgage lenders via the Financial Services and Markets Act 2000 – responded to the 2007 Northern Rock banking run by recognising that the UK’s deposit protection policies were inadequate and had the potential to trigger banking runs. So the FSA focussed on devising a robust system of deposit insurance to sustain public confidence in the banking system. These examples illustrate that a combination of more prudent mortgage lending and a more effective monetary policy institutional framework are important in moderating boom–bust cycles in the future. 

## 5.6

## Further reading

Academic articles and working papers 

Baddeley, M. C. (2005) ‘Housing bubbles, herds and frenzies: Evidence from British Housing Markets’, CCEPP Policy Brief No. 02–05, Cambridge Centre for Economic and Public Policy, Cambridge, UK. See www.landecon.cam.ac.uk/ 



Helbling, T. F. (2005) ‘House price bubbles – a tale based on housing price booms and busts’, BIS Papers No. 21 – Real Estate Indicators and Financial Stability, Bank for International Settlements, 30–41. 





Minsky, H. P. (1964) ‘Longer waves in financial relations: financial factors in the more severe depressions’, American Economic Review, vol. 54, no. 3, 324–35. 





Muellbauer, J. and Murphy, A. (1997) ‘Booms and busts in the UK housing market’, Economic Journal, vol. 107, no. 445, 1701–27. 





Oswald, A. J. (1997) ‘The missing piece of the unemployment puzzle’, Inaugural Lecture, University of Warwick. 





Wood, R. (2005) ‘A comparison ofUK residential house price indices’, BIS Papers No. 21 – Real Estate Indicators and Financial Stability, Bank for International Settlements, 212–27. 



## Policy reports and newspaper articles

Andre, C., Catte, P., Girouard, N. and Price, R. (2004) ‘Housing markets, wealth and the business cycle’, OECD Economics Department Working Papers, No. 394, Paris: OECD Publishing. The Economist (2005) ‘The global housing boom: in come the waves’, 16 June 2005. Financial Times (2004) ‘Every house price index tells its own story’, 30 June 2004. 

## 5.7 Chapter exercises

1. For the model in this chapter, we have implicitly assumed that mortgage lending and mortgage rates have immediate impacts on house prices. Using the data from the websites mentioned in the data section, assess this assumption as follows: 

(a) Adapting Equation (5.2), estimate a model of house prices that also includes lags (ofup to 4 quarters) on mortgage rates and mortgage lending. 

(b) Using t tests and p values, statistically assess the individual significance of the parameter estimates. 

(c) Use an F test of restrictions, assess whether or not lags on the explanatory variables are jointly associated with fluctuations in house prices. 

2. Housing demand is affected by the cost ofhousing. In this chapter, we have assessed one aspect of housing costs, i.e. borrowing costs as measured by mortgage rates, but personal incomes will also be important. 

(a) Using the ONS website (www.statistics.gov.uk) collect data on personal disposable income (PDI). 

(b) Incorporate current and lagged PDI (in logged form) into an extension of the house price model estimated in this chapter. 

(c) Assess the statistical significance oflogged PDI using t tests and F tests. 

(d) Interpret your findings. What are the policy implications? 

# Heteroscedasticity R&D, invention and innovation

Economic issues include: 

 Invention versus innovation 

 Role of technology 

Econometric issues include: 

 Homoscedasticity and heteroscedasticity 

 Heteroscedasticity tests: the Goldfield–Quandt test, White’s test 

 Weighted Least Squares (WLS) 

Data issues include: 

 Measuring innovation and knowledge: an innovativeness index 

 Working with outliers 

## 6.1 The issue

Innovation is essential for economic growth and development, whether for countries that are technological leaders at the frontier of knowledge or for countries that are ‘latecomers’, catching up on technical advances made elsewhere. Globalisation has interacted with rapid technological change and trade has become increasingly open and competitive, transport costs have fallen, and capital and labour have become more and more mobile. International competitive pressures have become more pronounced and all countries, rich and poor, have had to innovate constantly. 

Innovation can also involve finding new ways to do the same old things – for example in introducing new processes that can reduce the price and/or raise the quality of traditional products – such as wine. Overall, being innovative is important everywhere; it has important implications for developing countries as well as developed ones (UNCTAD, 2007); it is as important to individual firms as it is to nations as a whole. It is also important to individual people – we need to keep investing in and refreshing our personal human capital; in modern economies for example, there are many good reasons (social as well as professional) to be computer literate, i.e. to ‘invest’ in our human computing capital. 

In this chapter we will analyse the relationships between inputs into the innovative process (measured as R&D expenditure) and outputs (measured as number of patents) across a sample of countries. We will illustrate that, in getting accurate statistical information about the relationship between these inputs and outputs, we have to account for the specific econometric problem of heteroscedasticity. 

## 6.2 The theory

What is the difference between invention and innovation? Invention is about new ideas and technologies; innovation is about turning those new technologies into products and processes, i.e. it is about introducing new inventions into production. So invention is just the first stage in a long process. Figure 6.1 illustrates the pyramid of activities that mark progress from invention to innovation: invention is at the top of the pyramid (there can be no innovation without some inventions to precede it); the next segment of Figure 6.1 illustrates that inventions are then improved in a way that will boost productivity and competitiveness; then, as shown in the next segment, new technologies are adapted to fit in with existing productive processes; the final segment of the pyramid illustrates the final stage in which workers and managers are trained to use these new technologies in their everyday activities. 

The nature ofinvention and innovation can vary immensely according to its function and according to the capabilities and capacities that are required to do it. Countries (and firms) that are more innovative will have a better economic performance than those that are not: they will be quicker to pick up the latest technologies; they will be faster to bring new products to the market; they will be more competitive; and they will gain market share. Linked with these benefits should be sustainable job creation and increased economic growth. But before any of this can start, a country or a firm must decide to devote resources to the innovative process and this is where research and development (R&D) comes in. R&D is not the only element in the innovative process, but it is an essential one. Also, R&D expenditure is the most widely available and best-developed statistical indicator of inputs into the process of innovation activities. According to international guidelines, R&D comprises creative work undertaken systematically to increase the stock of knowledge and used for devising new processes (OECD, 2002). It includes basic research – research that advances scientific knowledge but has no specific immediate commercial applications; applied research – which has specific commercial objectives with respect to products, processes or services; and finally development – which involves systematically applying research knowledge to the production of prototype goods and services, new materials, and new methods, etc. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/da757c839138312f39f482326ad9ce0b1bfaf95d52ce491c83b283286ae04eba.jpg)



Figure 6.1 Invention vs. innovation: the pyramid of innovative activities


The theory tested in this chapter is that investing more in R&D increases a country’s innovativeness. Whilst we are not focussing specifically on the relationship between R&D, innovation and economic growth, our findings will have implications for the economic growth because R&D will contribute to innovation and innovation boosts economic growth. Here we will focus on this very first stage of the innovative process by asking: How can we boost a country’s performance in terms of innovation? What is the relationship between inputs and outputs into the innovative process? Framing the questions in this way will give us some hooks onto which policy initiatives can eventually be attached. 

## 6.3 The data

How can we measure innovation? A number of benchmarking exercises have been carried out, as many countries are concerned about their innovation capacities and performance. For example, Box 6.1 summarises proxies for both inputs and outputs used by Innovation Policy in Europe in its calculation ofthe Summary Innovation Index (SII) (see Figure 6.2), a measure of the relative innovativeness of a sample of countries over time. Other widely used measures include the Technological Activity Index (TAI) and the Human Capital Index (HCI). 

The SII gives a useful picture ofinnovation for a selection ofcountries but it is not a widely available or widely tested measure of innovation across all nations. Also, it combines both inputs and outputs into the innovative process. 

For our analysis we will assess whether input of R&D expenditure is associated with innovative output in terms of patents and, to do this, we will separate inputs and outputs, using patents granted in 2001 as our measure of innovative output (our dependent variable) and R&D expenditure in 2000 as our explanatory variable (input into innovation). Also, in order to illustrate the problem of heteroscedasticity (the econometric focus in this chapter) we will use two measures of R&D: total R&D expenditure and R&D intensity (i.e. R&D as a proportion of GDP). 

The sources for these data are as follows: 

<table><tr><td>Variable</td><td>Source</td><td>Website</td></tr><tr><td>Number of patents</td><td>US Patents Office</td><td>www.uspto.gov/</td></tr><tr><td>Real R&amp;D expenditure</td><td>OECD (2004) Science and Technology Industry Outlook</td><td>www.oecd.org</td></tr></table>

As discussed in previous chapters, it is important to state from the outset any potential problems with our data. Firstly, data on these issues is not yet widely published and so we have a cross-sectional data set that includes only 29 observations: this will generate two potential problems: sampling bias (a problem introduced in Chapter 4) and imperfect micronumerosity (explained in Chapter 5). Unfortunately we cannot do much about these problems 

## Box 6.1 Mirror mirror on the wall, who is most innovative of all …

The Summary Innovation Index (SII) is an index of innovative activity and has been calculated for a range of countries. This index has been constructed using the following indicators of innovation: 

## 1. Human resources

(a) Science and engineering graduates (% of 20–29 years age cohort) 

(b) Population with tertiary education 

(c) Participation in life-long learning 

(d) Employment in medium-tech and high-tech manufacturing 

(e) Employment in high-tech services 

## 2. Knowledge creation

(a) Public R&D expenditures 

(b) Business expenditures on R&D as % GDP 

(c) European Patent Office high-tech and general patent applications 

(d) United States Patent Office high-tech and general patent applications 

## 3. Transmission and application ofknowledge

(a) Small and medium sized enterprises (SMEs) innovating in-house (% of all SMEs) 

(b) SMEs involved in innovation co-operation 

(c) Innovation expenditures (% of total turnover) 

(d) SMEs using non-technological change 

## 4. Innovation finance output and markets

(a) Share of high-tech venture capital investment 

(b) Share of early stage venture capital in GDP 

(c) Sales of ‘new to market’ products 

(d) Sales of ‘new to the firm but not new to the market’ products 

(e) ICT expenditures (% of GDP) 

(f) Share of manufacturing value-added in high-tech sectors 

As Figure 6.2 shows, according to the SII, Sweden and Finland remain the innovation leaders within the European Union, ranking below Japan and above the United States in terms of global innovation levels. 

because the data just isn’t there (yet). But we should be careful to interpret our findings cautiously and hope that future studies (based on improved data) will confirm our findings. 

There are some more specific data problems too. For innovative output, patent data is not a perfect measure, not least because many innovations are not patented. In addition, knowledge can be created and transferred tacitly, in which case there will be no tangible measure of it. Also, some countries are new to the patent process and so will not put the same emphasis on patenting their innovations as countries that are not necessarily more innovative in real terms. Patenting is a costly exercise, and some countries may do less of it than others because of the administrative or legal costs involved. Finally, we can measure only the number of patents taken, not their value, either in terms of potential revenue streams, or in terms of their contribution to knowledge and innovation. Much valuable R&D that is conducted in the public sector, in universities and R&D institutions, is not patented; sometimes because it does not have a ready business application, although it may contribute to many subsequent valuable applications. In some countries, individuals working in university labs or faculties are not allowed to patent their work. Nonetheless, patents are one of the most frequently used measures of innovation mainly because the data are readily available. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/f3ef94e4c95121116cbaae0001d8df77bbf4f575eb3f7062938bd8e5255e5ad4.jpg)



Source: http://trendchart.cordis.lu/scoreboards/scoreboard2004/indicators.cfma



Figure 6.2 Summary Innovation Index, 2004


For R&D expenditure – it is the most frequently used measure of inputs into the innovation process but many developing countries may not collect or publish R&D data and, even if they do, the information may be outdated. Not all countries use the same definitions of R&D; and in some countries, firms have tax incentives to report activities as R&D when perhaps, under other circumstances, they would not be defined as such. For the purposes of industrial innovation and activities that are likely to result in patents, an important measure is likely to be Business Enterprise R&D (BERD), but data on this component of R&D is scarce so we use total R&D as a proxy. 

## Empirical results and interpretation

As explained above, we will be investigating the link between inputs into the innovative process (R&D expenditure) and innovative output (measured as number of patents) using 2000 and 2001 data. We might expect to find that higher levels of R&D expenditure in 2000 will result in larger numbers of patents in 2001. To assess this assertion we investigate the following model: 

$$
Y _ {i, t} = \alpha + \beta X _ {i, t - 1} + \varepsilon_ {i, t}\tag{6.1}
$$

where Y = number of patents granted for country i in year t, and X = general expenditure on R&D for country i in year t − 1, and $\varepsilon _ { i }$ is the random error term. The SRF will be: 

$$
Y _ {i, t} = \hat {\alpha} + \hat {\beta} X _ {i, t - 1} + \hat {\varepsilon} _ {i, t}\tag{6.2}
$$

The explanatory variable X is lagged because investing inputs of R&D expenditure will not immediately generate patents; the lag is included in the recognition that the process will take time. 

Our basic hypotheses will be that there is a significant association between R&D and patents granted in the following year: 

$$
\begin{array}{l} H _ {0}: \beta = 0 \\ H _ {1}: \beta \neq 0 \end{array}
$$

Table 6.1 shows the results from estimating the SRF using a cross-section of 29 countries with 2001 data on patents and 2000 data on R&D. From Table 6.1, these results can be summarised as follows: 

$$
\begin{array}{l l l} \hat {Y} _ {i} = & - 8 2 6. 2 3 & 0. 3 1 X \\ & (3 5 8. 2 4) & (0. 0 1) \\ & t = - 2. 3 1 & t = 4 2. 4 2 \\ & p = 0. 0 3 & p = 0. 0 0 \\ & R ^ {2} = 0. 9 9 \end{array}\tag{6.3}
$$

(Standard errors in brackets) 


Table 6.1 EViews output table: OLS regression


<table><tr><td colspan="5">Dependent Variable: Number of patents</td></tr><tr><td colspan="5">Method: Least Squares</td></tr><tr><td colspan="5">Sample: 1 29</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>-826.23</td><td>358.24</td><td>-2.31</td><td>0.03</td></tr><tr><td>General expenditure on R&amp;D</td><td>0.31</td><td>0.01</td><td>42.42</td><td>0.00</td></tr><tr><td>R-Squared</td><td>0.99</td><td>Mean dependent variable</td><td></td><td>4800.00</td></tr><tr><td>Sum squared residuals</td><td>86712468.00</td><td>F-statistic</td><td></td><td>1799.31</td></tr><tr><td></td><td></td><td>Prob(F-statistic)</td><td></td><td>0.00</td></tr></table>

These results suggest a positive and significant (at 5%) association between patents granted and R&D expenditure: with a $\boldsymbol { p }$ value of 0.00 on our t test, we can reject our null that the parameter on R&D is insignificantly different from zero at a 5% significance level. 

This is confirmed by our $R ^ { 2 }$ of 0.99 which suggests that 99% of the variability in patents granted is captured by variability in R&D expenditure. The F test of explanatory power (the F-statistic in the output table) also suggests a positive and highly significant relationship. So on first inspection our results look good (suspiciously good in fact!) but are they reliable? 

## The problem of heteroscedasticity

When we run a regression we need to think about whether or not the Gauss– Markov assumptions (outlined in Chapter 1) have been satisfied. In a full analysis of an empirical model, it is important to assess a range of potential violations of the Gauss–Markov assumptions but one of the aims of this book is to explain tests and techniques one at a time, with one problem as the focus of each chapter. For this chapter we will investigate heteroscedasticity. 

Heteroscedasticity is an extremely common problem in applied econometrics. It is particularly characteristic of cross-sectional data, but can also occur in time-series data. Heteroscedasticity literally refers to ‘differently dispersed’ errors, and as such it violates one of the Gauss–Markov assumptions introduced in Chapter 1. Specifically, it violates the assumption of homoscedasticity i.e. that errors are ‘similarly dispersed’. As explained in Chapter 1, OLS estimates are only BLUE ifthe error term is homoscedastic i.e. if var $\left( \varepsilon _ { i } \right) = \sigma ^ { 2 }$ where $\sigma ^ { 2 }$ is a constant. This constancy of variance means that if we were to take repeated samples ofdata, the error variance for each observation would be the same as the error variance for all the other observations. This is difficult to conceptualise in economics because we usually have only one sample of data and it may be difficult to see how we can infer anything at all about the error variance for each observation if we have just one set of observations. One way to conceptualise homoscedasticity is to think about the conditional value of the error variance, i.e. $\varepsilon _ { i }$ ‘conditioned’ on a particular value of X. With homoscedasticity, we would not expect the error variance to vary systematically with our explanatory variables, i.e. the conditional variance should be constant across all realisations of $X ,$ i.e. va $\cdot ( \varepsilon _ { i } \mid X _ { i } ) = \sigma ^ { 2 }$ . If we violate this assumption of homoscedasticity then we will have a heteroscedastic error term i.e. var $\left( \varepsilon _ { i } \mid X _ { i } \right) = \sigma _ { i } ^ { 2 }$ – the conditional variance of the error term will vary across observations as our explanatory variable varies. 

In a sample context, homoscedasticity requires that the residual variance be constant across all observations in the sample, i.e. it should not vary as X varies. As explained in Chapter 1, variance is a measure of spread and is calculated by squaring deviations from means. The expected value of a residual is zero so the residual variance can be calculated just by squaring the residuals, adding them together and dividing by the degrees of freedom, as explained in Chapter 1. In a sample context, the actual value of the residual can be positive, or negative, relatively close to 0 and relatively far from 0, but the point is that it should be random; the residual and residual variance should not be systematically associated with the explanatory variable X. We do not want the spread of residuals to increase as X increases. 

This can be explained intuitively using an example. If we are analysing consumption and expenditure patterns across households, then it is likely that we will find a greater dispersion of the kinds of choices made by wealthy households compared to poor households. When incomes are low, there can be little room for discretion on how to allocate one’s money: we pay the rent, buy food and other essentials. Most other poor households do exactly the same. By comparison, rich households can exercise more choice over how to allocate their money: choosing between spending on holidays, original art, second homes, or various forms of savings and investments. The variability of choices made by rich households will be much larger than poorer households. 

This will show up in a regression as a larger residual for observations on rich households than for observations on poor households. 

## Consequences of heteroscedasticity

With heteroscedasticity, our OLS parameter estimates will remain unbiased and consistent (as long as no other Gauss–Markov assumptions are violated) but they will not be minimum variance and other estimation methods will be needed to give us efficient parameter estimates – with smaller variances and narrower confidence intervals. In addition, the usual OLS formulae for variances and standard errors will be biased in the presence of heteroscedasticity and ifwe want to ensure that our hypothesis tests are correctly calculated, then we will have to use formulae for variances and standard errors that are adjusted to allow for heteroscedastic errors. 

Most estimation packages (including EViews) will report heteroscedasticityrobust standard errors for the parameter estimates and so, with large samples of data, OLS may give accurate estimates and inferences as long as hypothesis tests are constructed using these robust standard errors (and as long as the heteroscedasticity isn’t just a symptom ofa more serious problem such as model misspecification). It is important to remember that the default option for calculation of the variances in EViews assumes homoscedasticity but it is easy to get results that include the robust standard errors by ticking the option for ‘Heteroskedasticity Consistent Coefficient Covariance’ in the EViews ‘Equation Estimation’ window. 

What are the potential implications of heteroscedasticity for our analysis of innovation? Large economies will inevitably have larger absolute magnitudes ofR&D expenditure. So as R&D expenditure is incorporated in absolute terms into our regression of (6.2), we may be picking-up systematic differences in R&D expenditure rather than a robust association between R&D and patents. Our residual variance may be varying systematically reflecting this. It is also possible that large or rich countries will have different patenting behaviours than small or poor countries. For example, it could be that rich countries have developed the infrastructure to specialise in R&D; economies of scale and scope may enable them to produce more patents per unit ofR&D expenditure than poorer countries (even when R&D is measured in relative terms e.g. as a proportion of GDP). R&D may be more diversified in richer countries because their industrial structure has been adapted to R&D activities, particularly if large companies are trying to sustain monopoly advantages. Barriers to entry may prevent poor countries from using R&D expenditure to produce patentable inventions and innovations. In this case, our regression results may be distorted by the exceptional patent production of the richest countries, and our residual variance may be varying systematically reflecting these influences. 

## Diagnosing heteroscedasticity

Before we can use our OLS results to justify increased public or private R&D expenditure, we need to check whether or not our errors are heteroscedastic. How do we do this? As explained above, if our error variance is conditional upon the value of our explanatory variables, then we will have an heteroscedastic error term. So in a sample context, methods for detecting heteroscedasticity often focus on identifying systematic associations between the residual variance and the explanatory variables, including visual inspection and diagnostic tests – i.e. tests to diagnose specific violations ofGauss–Markov assumptions. 

## Visual inspection

The first and easiest thing to do is to inspect our data to look for systematic patterns in our residuals and residual variance. Figure 6.3 shows patents by country, ranked according to R&D expenditure; there is a clear non-linear relationship suggesting an exponential relationship between patents and R&D expenditure. In particular, Figure 6.3 shows extremely large patent outputs for the top R&D spenders i.e. for Sweden and the former G7 countries (USA, 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/d431c0bffd4f47eb09907a9fcb428cc372aae076996b8234e9c8c1831050da90.jpg)



R&D Expenditure (US$ millions, 1995 prices)



Figure 6.3 Patents by country, ranked by R&D expenditure


Japan, Germany, France, the UK, Canada and Italy).<sup>2</sup> These observations may distort our residual variance, particularly if we run a regression without controlling for units ofmeasurement. In addition, these last eight observations are not particularly representative of the whole sample and yet could be influential observations given our small sample size of 29 observations. In particular, we would be concerned about the last two observations (which are for Japan and the USA) because they are quite clearly outliers – i.e. extreme observations. Given this asymmetry in our data set, we would not be surprised to see our residual variance rising for observations on countries with particularly large R&D expenditures. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/80f92494c55d2fcdb3d626af1019019e67eb363941c583b9e8705278d48c856e.jpg)



Figure 6.4 Actual and fitted values from estimation of Equation (6.2)


We can also look at the plots of actual versus fitted values because the spread ofobserved values around the fitted line will give us a visual impression of the residual variance and so will capture the accuracy of our estimation. Figure 6.4 shows the plot of actual and fitted values from the estimation of Equation (6.2). On first inspection, there does seem to be a good fit but it is difficult to see what’s happening for the more average countries in the sample; in fact, for some countries in our sample, our initial model is generating negative fitted values for patents, which is a ridiculous result. So what’s happening in this plot? One of the problems with our initial model is that, because we have not (yet!) weighted or transformed our variables, we are not getting a clear impression of the patterns for countries with relatively low levels of R&D expenditure: the absolute magnitude of the residuals for these observations is small when plotted on a scale that captures the very large number of patents produced by the countries with very large number of patents (and high levels of R&D expenditure). So it is difficult to infer what might be happening with the residual variance for the smaller economies. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/fe2cbf9d86c589c4a863cb65c043a53d702f67e17e02c48065c22a8d618b6c42.jpg)



Figure 6.5 Actual vs. fitted values from Equation (6.2) for observations 1–20


To give a clearer impression, in Figure 6.5 we have plotted the actual and fitted values just for the more representative countries (excluding the eight countries with the very highest patents output) to illustrate how the unadjusted inclusion of these eight extreme observations is distorting the predicted values for patents for countries with more average R&D expenditure (i.e. most of the countries in our sample). 

This figure suggests that the accuracy of the patent estimates as captured by the fitted line is limited for the smaller countries but for most of the big R&D spenders the accuracy of the estimation improves: there is a clear systematic pattern and from this we could infer that the residual variance is not constant. Our visual inspection of this data suggests that we cannot assume that our errors are homoscedastic. 

## Diagnostic tests

Above we have shown a fairly clear pattern of heteroscedasticity in our plots of actual and fitted values. But patterns of heteroscedasticity are not always so easy to detect via visual inspection and so it is always a good idea to conduct some diagnostic tests. EViews (and most other econometrics packages) will report tests specifically designed to detect heteroscedasticity. There are many tests for heteroscedasticity and they revolve around identifying a systematic association between the residual variance and the explanatory variable(s). Here we will focus on just two tests: the Goldfeld–Quandt test and White’s test. 

The Goldfeld–Quandt (GQ) test can be used when one, rather than several, of the explanatory variables is suspected as the heteroscedasticity culprit. In multiple regression analysis, conducting the GQ test would involve constructing a new test for each explanatory variable but here our task will be relatively straightforward because we have only one explanatory variable – R&D expenditure. The intuition underlying the GQ test is that if the residual variance is changing as the explanatory variable changes, then we would expect to see a residual sum of squares (RSS) from the ‘top’ end of the sample (i.e. with the high values on X) that is significantly different from the RSS at the bottom end. So the GQ test involves calculating the ratio of the RSSs. 

The GQ test tests the following null and alternative hypotheses: 

$H _ { 0 } \colon \operatorname { v a r } ( \varepsilon _ { i } \mid X _ { i } ) = \sigma ^ { 2 }$ i:e: a homoscedastic error 

$H _ { 1 } \colon \mathrm { v a r } ( \varepsilon _ { i } \mid X _ { i } ) = \sigma _ { i } ^ { 2 }$ i: : h t d ti 

The construction of the GQ test involves the following stages: 

Step One: Rank the raw data according to ascending values of X. 

Step Two: Cut out a number of the central observations, breaking the data set into two distinct sets: one with low values of X and one with high values. One ofthe problems with the GQ test is that there is no clear rule about how many observations to delete and this means that there will always be an element ofsubjectivity to the GQ test. The general advice is to delete around 10–20% of observations – e.g. delete 4 observations for a sample size of 30 and delete 10 observations for a sample size of 60. 

Step Three: Run the regression for the first set of observations, to obtain RSS . Step Four: Run the regression for the second set of observations, to obtain ${ \mathrm { R S } } S _ { 2 } .$ 

Step Five: Calculate the F ratio of RSSs as follows: 

$$
F \left(n _ {1} - k - 1, n _ {2} - k - 1\right) = \frac {R S S _ {1} / \left(n _ {1} - k - 1\right)}{R S S _ {2} / \left(n _ {2} - k - 1\right)}\tag{6.4}
$$

In deciding how to split our sample, we have followed Thomas (1997) in deleting 4 central observations from our sample size of approximately 30 observations (Thomas 1997, p. 287). We will also incorporate an asymmetric split because our plot of actual versus fitted values indicates that the pattern changes for our eight top R&D spenders and we want to see how the residual variance differs for these top eight observations. So we will calculate RSS from a regression on the first 17 observations, delete the next 4 observations and then calculate ${ \mathrm { R S } } { \mathrm { S } } _ { 2 }$ from a regression on the last 8 observations. 

Running the regressions on observations 1 to 17 gives $\mathrm { R S S } _ { 1 } = 6 5 6 6 6 6 5 0 ;$ running another regression on observations 22 to 29 gives $\mathrm { R S S } _ { 2 } = 9 1 2 9 4 5 2$ so we calculate the F test as follows: 

$$
\begin{array}{r l}F (n _ {1} - k - 1, n _ {2} - k - 1)&= \frac {R S S _ {1} / (n _ {1} - k - 1)}{R S S _ {2} / (n _ {2} - k - 1)}\\&\rightarrow F (1 5, 6) = \frac {6 5 6 6 6 6 5 0 / 1 5}{9 1 2 9 4 5 2 / 6} = 2. 8 8\end{array}\tag{6.5}
$$

From statistical tables, $F _ { \mathrm { c r i t , ~ } 5 \% } ( 1 5 , 6 ) \approx 2 . 7 9$ and so we reject the null and, on the evidence of the GQ test, conclude that there is significant evidence of heteroscedasticity at a 5% significance level. 

We have rejected the null of homoscedasticity but with only a narrow margin. This may reflect the fact that the GQ test is not a powerful test (it has a relatively high probability of Type II error, i.e. of falsely retaining the null of homoscedasticity). This lack of power may emerge because, by deleting central observations, we are losing degrees of freedom and therefore potentially valuable information. There are other problems with the GQ test: the intuition underlying the deletion of the central observations is that it will accentuate the differences in the RSSs but there are no clear rules about how many central observations to delete and this introduces an element of subjectivity into the GQ test. Also, the GQ is sensitive to differences in the way the sample is split (this problem is illustrated in the chapter exercises). Also, in a multiple regression context, the test would have to be run a number of times using each explanatory variable. Finally, it is important to remember always to put the larger residual variance in the numerator otherwise the test will have no power at all! (If we calculate the GQ test the wrong way round then F will always be less than 1; always less than the relevant critical value and so the null of homoscedasticity would be retained even for very large and systematic changes in the residual variance.) 

Luckily, there are newer and more powerful heteroscedasticity tests, for example White’s test. The intuition underlying White’s test is much the same as the basic intuition underlying the GQ test: it focusses on identifying systematic patterns between the residual variance, the explanatory variable(s) and the square of the explanatory variable(s). It is relatively straightforward to perform and one variant can be constructed as follows: 

1. Save $\hat { \varepsilon } _ { i }$ i.e. the residuals from the initial SRF (Equation (6.2)). 

2. Square the explanatory variable. 

3. Run an auxiliary regression (i.e. a regression using output from the estimation of the SRF) by regressing the squared residuals on the level and square of the explanatory variable: 

$$
\hat {\varepsilon} _ {i} ^ {2} = \phi + \gamma_ {1} X _ {i} + \gamma_ {2} X _ {i} ^ {2}\tag{6.6}
$$

where $\hat { \varepsilon } _ { i } ^ { 2 }$ is the squared residual for each observation i, ϕ is the intercept for the auxiliary regression and $\gamma _ { 1 }$ and $\gamma _ { 2 }$ are the parameters on the explanatory variable and its square. 

4. Conduct an F test of explanatory power to give White’s test statistic. 

5. If $F > F _ { \mathrm { c r i t } }$ then reject the null of homoscedasticity, i.e. reject $H _ { 0 } { \mathrm { : } }$ var $\cdot ( \varepsilon _ { i } \mid X _ { i } ) = \sigma ^ { 2 }$ 

The intuition underlying this procedure is that if there is a systematic association between the residual variance and X, then the $R ^ { 2 }$ from this auxiliary regression will be relatively high. 

White’s test has a number of advantages over the GQ test, most of which centre around the fact that less subjectivity is involved in the testing procedure: there is no room for error in selecting an explanatory variable to capture the heteroscedasticity because all explanatory variables are included (degrees of freedom permitting); and there are no decisions to be made about how many central observations to exclude. All information is used which makes it, ceteris paribus, a more powerful test than the GQ test. 

It has the added practical advantage that it is calculated automatically by EViews. For our example, see Table 6.2 for the EViews output table which records White’s F test and its associated p value: because $\textstyle p < 0 . 0 5$ we can reject $H _ { 0 }$ at a 5% significance level (and at much lower significance levels too). Thus White’s test result suggests that there is strongly significant evidence of heteroscedasticity for our initial estimation, a result that is consistent with the GQ test and our visual inspection of actual versus fitted values. 


Table 6.2 EViews output table: White’s heteroscedasticity test


<table><tr><td colspan="5">White&#x27;s Heteroscedasticity Test:</td></tr><tr><td>F-statistic</td><td>43.48</td><td>Probability</td><td>0.00</td><td></td></tr><tr><td>Obs*R-squared</td><td>22.33</td><td>Probability</td><td>0.00</td><td></td></tr><tr><td>Test Equation:Dependent Variable: RESID^2 (= squared residuals)Method: Least SquaresSample: 1 29Variable</td><td>Coefficient</td><td>Std.Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>-1986402.00</td><td>967760.60</td><td>-2.05</td><td>0.05</td></tr><tr><td>R&amp;D expenditure</td><td>583.79</td><td>62.90</td><td>9.28</td><td>0.00</td></tr><tr><td>R&amp;D expenditure squared</td><td>0.00</td><td>0.00</td><td>-8.68</td><td>0.00</td></tr></table>

## Remedial measures

Visual inspections of the data and both the GQ and White’s tests have indicated a problem with heteroscedastic errors for our estimation of (6.2). So our initial OLS results will not be giving us the most accurate impression of the relationship between patents and R&D expenditure. Heteroscedasticity means that our OLS estimators are no longer efficient, which undermines the usual hypothesis-testing procedures. What can we do about it? Luckily there is a range of possible solutions though a process of trial and error is often needed in identifying the best solution. Some potential solutions are outlined in Box 6.2. 

## Box 6.2 Correcting heteroscedasticity

Heteroscedasticity can emerge for a number of reasons and, in the context of a sample, identifying a solution often involves a process of trial and error. For regressions of linear models, one quick and simple approach is to transform the data into logs, because this compresses the scales in which variables are measured. For example if we had used levels data: the raw value of real USA expenditure on R&D in 2000 at US$243,271 million is more than a thousand times larger than the US$207 million spent by Iceland. When transformed to natural logs the differences between them are sharply compressed to 12.4 (United States) and 5.33 (Iceland). Estimating log-log models may also have theoretical plausibility if we want estimates of unit-free elasticities to capture the percentage changes in Y associated with a given percentage change in X. (Elasticities and log-log models were introduced in Chapter 3.) 

If heteroscedasticity is a symptom of the influence of an outlier or small groups of outliers then, given the central limit theorem (discussed in Chapter 1), the problem may become unimportant in large samples. Note from above that OLS is still consistent in large samples even though it is inefficient (but unbiased) in small samples. So we may be able to reduce the problem by increasing our sample size. We could also delete the outlier observations but this would involve a loss of degrees of freedom. It will also involve a willing abandonment of potentially important information: those apparent outliers may in fact give some important clues about our empirical model. 

If justifiable in terms of the relevant economic theory, we can transform our model and ‘normalise’ the data to minimise the likelihood of heteroscedasticity; for example we could transform data by expressing data per capita or as a proportion of GDP. This sort of informal weighting process can also eliminate outliers without abandoning observations. 

Alternatively, we can use more rigorous estimation procedures specifically designed to ‘homogenise’ our sample variance. If we had information about the error variance from the relevant population, then we could use weighted least squares (WLS) a type of generalised least squares (GLS) procedure.<sup>3</sup> In the rare case when we know exactly the underlying error variance, we can use this information in transforming our model. To illustrate this, we start with the following model: 

$$
Y _ {i} = a + \beta X _ {i} + u _ {i}\tag{6.7}
$$

Let’s pretend that we know that the error variance (conditional on the value of $\textstyle \chi _ { j } )$ takes the following form: 

$$
\operatorname{Var} \left(u _ {i} \mid X _ {i}\right) = \sigma^ {2} X _ {i} ^ {2} \text { where } \sigma^ {2} \text { is   constant }\tag{6.8}
$$

Then we can divide both sides of (6.7) by X to give: 

$$
Y _ {i} / X _ {i} = \left(a / X _ {i}\right) + \beta \left(X _ {i} / X _ {i}\right) + \left(u _ {i} / X _ {i}\right) = a \left(\frac {1}{X _ {i}}\right) + \beta + \varepsilon_ {i}\tag{6.9}
$$

Notice that the error in (6.9) has been transformed into $\varepsilon _ { i } = \frac { U _ { i } } { \chi _ { i } }$ 

Next we must assume that our explanatory variable is non-stochastic for a given observation i (i.e. even though the explanatory variable must vary within a sample, the value of each individual observation on the explanatory variable will be a constant across samples). This means that the value of X will be fixed for each observation i. This is difficult to conceptualise with only one sample of data but it means that the Xvalues be fixed across all samples; if this is true, then the value of X for each individualobservation $i ,$ will be a constant and so we can take $\chi _ { \mathrm { i } }$ outside the variance expression, squaring it as we go (following the mathematical rules of variance). So the variance of $\varepsilon _ { j }$ becomes: 

$$
\operatorname{var} \left(\varepsilon_ {i}\right) = \operatorname{var} \left(\frac {u _ {i}}{X _ {i}}\right) = \frac {1}{X _ {i} ^ {2}} \operatorname{var} \left(u _ {i}\right)\tag{6.10}
$$

From Equation (6.8), we incorporate the expression for ${ \mathsf { v a r } } ( U _ { i } )$ as follows: 

$$
\operatorname{var} \left(\varepsilon_ {i}\right) = \frac {\operatorname{var} \left(u _ {i}\right)}{\chi_ {i} ^ {2}} = \frac {\sigma^ {2} \times \chi_ {i} ^ {2}}{\chi_ {i} ^ {2}} = \sigma^ {2}\tag{6.11}
$$

and so $\varepsilon _ { j }$ is equal to the constant $\sigma ^ { 2 } ;$ it is homoscedastic. 

Our WLS estimation will give accurate and reliable estimates (provided all the other Gauss–Markov assumptions are satisfied too) and WLS will be a BLUE estimation technique. This illustrates that sometimes (not always!) when Gauss–Markov assumptions are violated, the least squares principle can be adapted to give GLS estimators; these estimators will be consistent and efficient even when OLS is not. 

So, in theory at least (and given our assumptions), we could get a model with a homoscedastic error simply by regressing Y/X on 1/X, though care is needed in interpreting parameter estimates from WLS. Notice in the transformed model set out in Equation (6.9) that the constant from (6.7) is being estimated by the slope parameter on 1/Xin Equation (6.9); and the slope parameter on X is being estimated by the intercept from this transformed model. 

There are some problems with taking this approach to a sample context and we will explain these below. But first we will explain the intuition underlying this sort of weighting procedure assuming that we can easily use this solution in samples of data. In a sample, if the residual variance is increasing as X increases, then fitted values associated with high values of X will be less reliable than fitted values associated with low values of X (the residuals and residual variance will be larger; there will be a larger divergence between observed values and fitted values). In dividing through each observation by Xwe are giving a greater weight to observations associated with low values of X(i.e. the observations that are bein estimated more accuratel and a lesser wei ht to observations associated with hi h values of X (which are being estimated less accurately). So we are weighting observations according to reliability and the overall accuracy of our estimation will improve accordingly. 

The main problem with WLS is that when we are working in the realm of social, rather than physical, science it is extremely unlikely that we will have much information at all about the hypothetical error variance – we have at best a large and representative sample. For this reason the above procedure is sometimes known as infeasible WLS: it’s not a feasible procedure when (as is usually the case) we don’t know the exact form of the heteroscedasticity. 

But understanding the basic intuition underlying this infeasible WLS procedure is important because the same intuition underlies other GLS procedures. But when we don’t know the error variance we need to select appropriate weights carefully. For example, take the case where the residual variance increases as the explanatory variable X increases; this implies that the accuracy of the model is decreasing as we get larger and larger values of the explanatory variable and so dividing through by X would not work. 

One way to identify appropriate weights is to estimate the unknown population variance using our sample data. To do this, we would take the residuals from the OLS estimation, and square them. Then we could estimate the conditional residual variance by regressing the squared residuals on some function of the explanatory variable. We would take the square root of this conditional residual variance for each observation and use it to weight each observation (i.e. we would divide each observation by the square root of the conditional residual variance). This procedure is known as feasible WLS (FLS). FLS will not be unbiased in small samples and the residual variance will not be an unbiased estimator of the error variance but FLS will be consistent so may work effectively with large samples of data. 

OLS is consistent too so why bother with FLS? Remember from our discussion of consequences that the OLS formulae for standard errors and variances will be biased in the presence of heteroscedasticity and FLS does not suffer from this disadvantage. 

For our analysis ofinnovation we tried various combinations ofthe solutions outlined in Box 6.2. One option would be to exclude the outliers but in doing this we would be ignoring observations that might convey valuable information about R&D (we do not want to lose USA and Japan and the lessons that their story might tell us). We tried estimating a log-log model to pick up an exponential relationship between R&D and patents; this did reduce the problem of heteroscedasticity but we were still forced to reject the null of homoscedasticity at a 5% significance level. The log-log model did not effectively control for the extremely large observations on real R&D expenditure for the G7 countries and Sweden. We considered expressing all the variables as ratios ofGDP. Whilst this would be appropriate for R&D expenditure, expressing patents as a ratio of GDP would be problematic because patents as a proportion ofGDP has no clear economic meaning and so interpreting results would be difficult. So finally we combined the solutions and identified the following model: 

$$
y _ {i, t} = \theta + \lambda x _ {i, t - 1} + \xi_ {i, t}\tag{6.12}
$$

where y is patents (logged), x is R&D intensity (real R&D expenditure as a proportion of GDP); θ is the intercept, λ is the slope parameter and $\xi$ is the error term. 

From this we estimate the following SRF: 

$$
\hat {y} _ {i, t} = \hat {\theta} + \hat {\lambda} \hat {x} _ {i, t - 1}\tag{6.13}
$$

The results from the estimation of this model (including the White’s test result) are reported in Table 6.3. 

These results suggest a positive and significant relationship between patents and R&D intensity: with a p value of 0.00 on our t test, we can reject our null that the parameter on R&D is insignificantly different from zero. Given that patents is now logged, the parameter estimate suggests that an increase in R&D of 1% of GDP is associated with a 1.93% increase in patents granted the following year. The overall association between these variables is confirmed by our $R ^ { 2 }$ of 0.43; 43% of the variability in patents (logged) is captured by variability in R&D intensity. The F test of explanatory power confirms that there is a highly significant relationship: we can reject the null hypothesis of no association between patents and R&D intensity at very low significance levels. A visual inspection ofactual and predicted values (see Figure 6.6) suggests that the residuals and residual variance do not seem to be exhibiting systematic patterns. 


Table 6.3 EViews output table: model with homoscedastic errors


<table><tr><td colspan="5">Dependent variable: Patents (logged)</td></tr><tr><td>Method: Least SquaresSample: 1 29Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>2.48</td><td>0.82</td><td>3.04</td><td>0.01</td></tr><tr><td>R&amp;D intensity</td><td>1.93</td><td>0.43</td><td>4.52</td><td>0.00</td></tr><tr><td>R-squared</td><td>0.43</td><td>F-statistic</td><td></td><td>20.42</td></tr><tr><td>Sum squared residuals</td><td>109.41</td><td>Prob(F-statistic)</td><td></td><td>0.00</td></tr><tr><td colspan="5">White Heteroscedasticity Test:</td></tr><tr><td>F-statistic</td><td>1.36</td><td>Probability</td><td></td><td>0.27</td></tr><tr><td>Obs*R-squared</td><td>2.75</td><td>Probability</td><td></td><td>0.25</td></tr><tr><td colspan="5">Dependent Variable: RESID^2</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>2.90</td><td>3.86</td><td>0.75</td><td>0.46</td></tr><tr><td>R&amp;D intensity</td><td>-1.02</td><td>4.58</td><td>-0.22</td><td>0.83</td></tr><tr><td>R&amp;D intensity squared</td><td>0.71</td><td>1.18</td><td>0.60</td><td>0.55</td></tr></table>

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/4aa6e1341c14eaa5f60ce2bfd00e5c9cc90c05b319f6e32e6b3a6786a7c85440.jpg)



Figure 6.6 Actual vs. fitted values from transformed model (Equation (6.11))


Most importantly, our White’s test result suggests that we can retain our null hypothesis of homoscedasticity at 5% and at 10% and in fact at significance levels up to 27%. 

Why has this transformation worked so well? Dividing R&D by GDP to give a measure of R&D intensity reduced the association between the residual variance and explanatory variable; it has also reduced the distorting impact of the outliers. Logging the patents variable enabled us to capture the exponential relationship between patents and R&D expenditure as initially identified from an inspection of Figure 6.3. Overall, we have reliable evidence that there is a significantly positive association between R&D intensity in 2000 and patents in 2001 for the 29 countries in our sample. 

## Policy implications and conclusions

The empirical evidence of a positive association between inputs into the innovative process (as measured by R&D intensity) and innovative outputs (as measured by patents granted) suggests that boosting R&D intensity can have beneficial impacts in terms of innovative activity. But what policies can be put in place to boost R&D spending and thus encourage innovative activity? 

In some countries and/or industries, particularly less-developed countries and industries, innovative activities are undertaken informally, without the trappings of formal R&D departments. As countries mature however, R&D begins to appear as a distinct activity. As firms tackle increasingly significant technological improvements, and as consumer demand for new products grows, firms will want to introduce new product and process innovations and so the role offormal R&D will become increasingly important. Firms may set up specialised units to monitor new developments, to adapt and improve on existing technologies, and/or to develop something completely new. R&D can also be conducted in low-tech and medium-tech sectors as much as in the high-tech sectors with which one usually associates R&D – in Italy for example, most business-related R&D takes place in the textiles and manufacturing sectors, i.e. in traditional sectors but ones in which Italy has created a strong comparative advantage. 

There is evidence that R&D activity can generate increasing returns; as innovation opens up new industries, there may be special and widespread benefits particularly if innovation enables local people in LDCs to build-up their human capital in acquiring technological knowledge. In China and 

India, massive amounts of R&D are being undertaken as a principal activity, reflecting China and India’s comparative advantage in terms of endowments of large numbers of highly skilled scientists and engineers. In India, technological changes associated with computerisation have allowed her to become a global leader in software technology and innovations in telecommunications have allowed her to take advantage of the demand for call-centre outsourcing, with substantial benefits for the wider economy. 

In the fast-moving, highly competitive and technologically advanced globalised world, maintaining innovative advantages will be essential for economic growth and progression and, in promoting innovation, governments can play a crucial role particularly for economies that do not have a well-established tradition of innovation within the private sector. Formal R&D is an essential part of the technological learning process but in countries without an established R&D tradition and/or where private firms are not willing or able to undertake R&D expenditure, governments can play a leading role. 

## 6.6

## Further reading

## Textbooks



Fagerberg, J., Mowery, D. and Nelson R. (eds.) (2004) The Oxford Handbook of Innovation, Oxford: Oxford University Press. 





Link, A. N. and Scherer, F. M. (eds.) (2006) The Economics of R&D, Innovation, and Technological Change: Essays in Honor ofEdwin Mansfield, New York: Springer-Verlag. 





Stock, J. H. and Watson, M. W. (2000) Introduction to Econometrics, Harlow: Pearson Education/Addison-Wesley, Chapter 4. 





Thomas, R. L. (1997) Modern Econometrics: An Introduction, Harlow: Addison-Wesley, Chapter 10. 





Wooldridge, J. M. (2003) Introductory Econometrics: A Modern Approach (2nd edition), Thomson South-Western, Chapter 8. 



## Academic articles and working papers

Klette J. and Kortum S. (2004) ‘Innovating firms and aggregate innovation’, Journal ofPolitical Economy, vol. 112, no. 5, 986–1018. 

## Policy Reports

OECD (2002), OECD Science, Technology and Industry Outlook 2002, Paris: Organisation for Economic Cooperation and Development. Published annually. 

UNCTAD (2005), ‘World Investment Report 2005 – Transnational Corporations and the Internationalization of R&D’. New York and Geneva: United Nations Conference on Trade and Development. www.unctad.org/en/docs/wir2005overview_end.pdf 

UNCTAD (2007), Knowledge, Technological Learning and Innovation for Development, Least Developed Countries Report, Geneva and New York: United Nations. 

## 6.7

## Chapter exercises

1. For the Goldfeld–Quandt (GQ) test estimated in this chapter, we have incorporated an asymmetric division of the sample. Using the data sources outlined in the data section: 

(a) Construct your own GQ test for heteroscedasticity by dividing the sample symmetrically, using RSS<sub>1</sub> from a regression on the first 12 observations and ${ \mathrm { R S } } { \mathrm { S } } _ { 2 }$ from a regression on the last 12 observations. Discuss your result. 

(b) What can you say about the power of this form of the GQ test? 

(c) Explain the divergence between your result and the result from the GQ test conducted in this chapter. 

2. Using the data sources outlined in the data section: 

(a) Estimate a log-log model of the relationship between patents and R&D expenditure and discuss your results. 

(b) Construct two plots of your actual and predicted values – one for the whole sample and the other for the first 20 observations (i.e. excluding the G7 and Sweden). What do these plots suggest about the nature of the residual variance in your estimation? 

(c) Using EViews, conduct White’s test for your log-log model. Explain why your results differ from the estimation of equation 6.13. 

# Autocorrelation Tourism and the environment

Economic issues include: 

 Tragedy of the commons and environmental externalities 

 Game theory and the Prisoner’s Dilemma 

 Tourism life-cycles and sustainable development 

Econometric issues include: 

 Breusch–Godfrey LM and Durbin–Watson tests for autocorrelation 

 Generalised Least Squares (GLS) and the Cochrane–Orcutt procedure 

Data issues include: 

 Measuring the environment 

## 7.1 The issue

The tourism industry has great potential to boost incomes, growth and development in poorer countries. World Travel and Tourism Council (WTTC) estimates of the economic contribution made by tourism in 2005 include revenues of$6201.5 billion, employment of221.6 million workers and an 8.3% share ofGDP. For the Caribbean alone, a region heavily dependent on its tourism industry, 2005 estimates indicate that tourism has contributed 15% of GDP, 15% of jobs and $45.5 billion of revenue. 

This growth in the tourism industry has not come without a cost. Iftourism is not carefully planned then there will be negative consequences for the natural environment and for socio-economic and cultural institutions more generally. Even when judged in terms of prospects for the tourism industry alone, if the environmental resources on which tourism depends are exploited and destroyed by rapid growth in tourism demand then the contribution of tourism to sustainable development in the long term will be limited. 

In managing a tourism industry that will be sustainable in the future, policy makers need to take account of the environmental consequences. So there are a lot of difficult issues confronting policy makers in those countries that are promoting sustainable development via their tourism industries. 

## 7.2 The theory

In assessing the relationships between tourism, the environment and sustainable development, a number of theoretical issues are important. In this chapter we focus on analyses ofthe ‘tragedy ofthe commons’ and the relationships between tourism life cycles and sustainable development. 

## The tragedy of the commons

The tragedy of the commons is a problem that emerges from the over-use of natural resources held in common ownership. Hardin (1968) described this problem as emerging in the use of common grazing land before the English parliamentary enclosures movement of the eighteenth century. (See also The Economist (2008) for a modern analysis ofthe problem.) According to Hardin, when land was commonly owned, local villagers had an incentive to have more cows grazing on the land than was economically efficient. This was because each villager always had an incentive to put more cows on the land as long as they could afford it because if they didn’t make use of the land with their own cows, then the other villagers would use the land instead. The parliamentary enclosures movement provided a solution to this problem by creating a system of private property rights; these encouraged each property owner to consider the efficient and sustainable use of their own land, consequently reducing the over-grazing problem. 

This tragedy of the commons principle can be applied to the use of environmental resources in a modern context too. Modern tragedies of the commons exist when environmental resources are over-used by tourism industries. The essence of the problem can be explained using concepts from game theory. Game theory involves the analysis of strategic interactions between small groups of ‘players’. In its simplest form, game theory focusses on interactions in 2-player games. The over-use of natural resources illustrates a commonly observed game: the Prisoner’s Dilemma (PD). In PD games the market mechanism does not operate efficiently to coordinate individuals’ self-interested actions and Adam Smith’s Invisible Hand goes into reverse: players pursuing their own self-interest will generate a suboptimal social outcome. 

The PD game can be used to illustrate the tragedy of the commons and here we apply the ideas to analyse environmental impacts of tourism. Imagine that there are two hotels in Goa: the Taj Mahal Hotel and the Amber Palace Hotel. An environmental resource on which they will both depend is a clean sea. If there is sewage in the sea then customers will stay away and each hotel will lose revenue. We begin by assuming that, for each hotel, tourism revenues will fall by 3.5 million rupees for the number ofhotels without a sewage plant. So ifone has a sewage plant and the other doesn’t, each hotel’s revenues will fall by 3.5m rupees. Ifneither have a sewage plant, then their revenues will fall by 7m rupees each. On the other hand, ifa hotel wants to build a sewage plant then it will cost them RS5m. These figures can be incorporated into a pay-off matrix which shows the financial consequences of the hotels’ strategies, see below noting that we have negative pay-offs in this matrix because we are examining the costs. 

<table><tr><td></td><td>Taj Mahal Sewage into sea</td><td>Taj Mahal Buy sewage plant</td></tr><tr><td rowspan="2">Amber Palace Sewage into sea</td><td>Amber Palace: -7m rupees</td><td>Amber Palace: -3.5m rupees</td></tr><tr><td>Taj Mahal: -7m rupees</td><td>Taj Mahal: -8.5m rupees</td></tr><tr><td rowspan="2">Amber Palace Buy sewage plant</td><td>Amber Palace: -8.5m rupees</td><td>Amber Palace: -5m rupees</td></tr><tr><td>Taj Mahal: -3.5m rupees</td><td>Taj Mahal: -5m rupees</td></tr></table>

If you imagine that you are managing the Taj Mahal Hotel, you will see that your costs will be minimised if you pump your sewage into the sea. This is the dominant strategy, i.e. the best strategy regardless of the actions of the other player. The game is symmetrical, i.e. the same strategy will work for the Amber Palace Hotel. So the net result is that both hotels will pump sewage into the sea incurring 7m rupees in lost revenue for each hotel, a total loss for the industry of 14m rupees. This is the Nash equilibrium of the game. The Nash equilibrium is a game’s point of stability, i.e. the point at which there is no incentive for either player to change their strategy. But in terms of the Pareto optimal strategy: if both hotels had bought sewage plants, then their total losses would have been 10m rupees – the best overall outcome even when judged just in terms ofthe two hotels’ costs. In terms of the broader environmental impacts, the social benefits would have been even greater. But each hotel had no guarantee that the other hotel would buy a sewage plant so there was no incentive for either of them individually to pursue the socially desirable strategy. 

The essence of this tragedy of the commons idea is that the use of natural resources in common ownership creates negative externalities: exploiting natural resources may benefit private individuals but if no-one is taking responsibility for maintaining those resources (because those resources are in common ownership), then the use ofnatural resources will not take account of the total social costs. 

The social costs of environmental change will impact in a number of ways: environmental change may limit the future viability of the tourism industry, particularly for countries dependent upon an abundance of natural resources. Environmental change will also have global impacts e.g. in terms ofclimate change. 

## Environmental impacts on tourism in LDCs

These negative externalities have implications for the length of tourism lifecycles. The tourism life cycle describes the stages of growth and decline in tourism production. The tourism life-cycle concept illustrates how the tourism industry goes through a cycle of growth and decline in response to different motivators of demand. In the early stage, facilities for tourists are limited but as tourism demand grows, external economies develop. External economies emerge when the economic activities undertaken by an individual person/business benefit all people/businesses within an industry or area. For our example of tourism development, external economies take hold and so the construction of some infrastructure encourages the creation of more infrastructure; new hotels have to construct roads, lighting, drainage etc. and the presence of these services encourages the building of more new hotels. The tourism industry will grow rapidly until it reaches a peak. Then, particularly given the fashions and fads in tourism demand, resorts will lose their novelty appeal. Overcrowding and congestion will discourage tourists from returning. Some tourists will in any case only want to re-visit a resort once. Once these negative factors take hold, the resort will head into decline (Baddeley, 2004). 

The tourism life-cycle hypothesis illustrates that many of the negative environmental impacts emerging from the development of tourism resorts emerge only over a relatively long time horizon. In poorer countries, the focus is by necessity often on the short term. When there are mouths to feed today it doesn’t make much sense to worry about the long-term profitability of tourism resorts let alone environmental sustainability more generally. If the tourism industry is to provide a long-term development solution, some of the problems outlined above must be resolved. Tourist areas should be encouraged to develop in a way that provides local incomes allowing local infrastructure to develop but in a way that is sustainable – both in terms of prolonging the life-cycle of tourism resources but also in a way that preserves the environment. 

## Global environmental impacts: climate change

Above we have outlined some ofthe issues affecting the development oftourism in particular areas. There are also significant global implications. Clear air and clean seas are natural resources in common ownership and so private incentives will not automatically ensure that these resources are maintained. This has created particular problems in the last few decades. Growing demand for international tourism has led to rapid rises in demand for air travel (an issue that was also addressed in Chapter 3). In particular, with more and more tourists flying to more exotic locations, the demand for air travel has increased with significant implications for climate change. The Stern Review (Stern 2006) gave an extensive assessment of the future environmental and economic consequences of human-made environmental change, advocating that governments invest now to ameliorate environmental damage in the future. The implications of aircraft emissions for the global environment have also been the focus for recent policy reports from groups such as the Intergovernmental Panel on Climate Change (IPCC) and the UN Framework Convention on Climate Change (UNFCCC). For example a recent IPCC report has highlighted the impact of international aviation on climate change; this report notes that international passenger traffic has grown by approximately 9% per year since 1960 – exceeding growth in GDP by a factor of 2.4. (Penner et al., 1999, p. 23) Technological improvements and improved operational procedures have mitigated the impacts of this growing demand for aviation but nonetheless, reductions in emissions from these changes have not kept pace with the rises in aviation emissions from increased demand for air transport. Penner et al. also project that future rises in passenger traffic will exceed future growth in GDP. 

In this chapter we explore some of the impacts of tourism on the environment by analysing the relationship between international tourist traffic and aircraft emissions using the data described in the following section. 

## 7.3

## The data

In this chapter, we use time-series data to investigate the relationship between aviation emissions and international flows oftourists. It is important to remember that aviation emissions, and emissions more generally, are just one factor affecting the environment. Some of the broader issues involved in measuring the environment and environmental resources are outlined in Box 7.1. 

## Box 7.1 Measuring the environment

Measuring the environment is difficult because there is no single measurable objective factor that defines the environment. Some traditional indicators have focussed on the categories of economic, social and biophysical environmental aspects but it is difficult objectively to rank and/ or select the individual criteria that define these categories. In terms of environment sustainability, e.g. of tourism developments, indicators such as the Index of Sustainable Economic Welfare (ISEW), the Environmental Pressure Index (EPI) and Genuine Progress Indicator (GPI) have been devised to give a general, broad picture of environment impact. However, there can be no completely objective criterion for assigning appropriate weights to the various components of these indicators. The Barometer of Sustainability (BS) gives equal weights to human well-being and eco-system ‘well-being’ but the judgement to weight equally involves some subjectivism; some might argue that human well-being should have a greater weight; others might think that homo sapiens is only one species and therefore assigning human and ecosystem well-being equal weights involves an implicit over-estimation of human priorities. Approaches such as the Ecological Footprint (EF) methodology involve assuming that all space is equal in quality and importance. But again, is it appropriate to assume that all people should be entitled to the same environmental resources? Different people/organisations create different externalities, both positive and negative, in terms of their economic and social activities. Should a brothel have the same entitlement to land as a university? Also, all space is not equal in usefulness to people: many people would probably value an acre in Sydney more highly than 100 acres in the Simpson Desert. 

For all indicators of environmental quality and impact, measurement will be particularly difficult for LDCs because collecting, harmonising and disaggregating data will be a difficult task. This all suggests that adopting a more disaggregated and partial approach to environmental assessment is a necessary compromise in a less than ideal world. 


Our dependent variable is aircraft emissions and our explanatory variable is tourism flows and the data is collected from the following sources:


<table><tr><td>Variable</td><td>Source</td><td>Website</td></tr><tr><td><eq>CO_{2}</eq> emissions from international aviation bunkers</td><td><eq>CO_{2}</eq> Emissions from Fuel Combustion, International Energy Agency (IEA)</td><td>www.iea.org</td></tr><tr><td>International Tourism Arrivals</td><td>Tourism Market Trends – Statistical Annex, UN World Trade Organisation (UNWTO)</td><td>www.unwto.org</td></tr></table>


Figure 7.1 shows the time-plots of data on emissions and tourism arrivals between 1971 and 2003.


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/f57ec49a3badc03b3c4bac6b3a8ac4f22923dd8c922110482b02dd86f1937305.jpg)



Figure 7.1 International aviation emissions and international tourist arrivals, 1971–2003


An initial inspection of these data suggests that aviation emissions increase with tourism arrivals and provide preliminary evidence in support ofour hypothesis that there is a positive assocation between tourism demand and aircraft pollution. As always however, it is important to acknowledge the limitations of our data set. The emissions data is derived from records of fossil fuel used by the aviation industry. There are other measures of emissions. The UN Framework Convention on Climate Change (UNFCCC) requires countries to submit audits of $\mathrm { C O } _ { 2 }$ emissions but whilst the UNFCCC embeds a common reporting format for all countries, its geographical coverage is limited. Also, there are other types of aviation emissions and we have concentrated just on $\mathrm { C O } _ { 2 }$ emissions as they are relatively easy to measure. As for the tourism data, these will proxy for the growth in demand for international aviation from tourists. However, it is important to remember that tourists are not responsible for all aviation emissions and also, some tourists will use other forms of transport; the emissions from these alternative forms of transport will not be captured in aviation emissions data. 

## 7.4 Empirical methods and results

Our overall hypothesis is that international tourism will generate negative environmental consequences. In particular, the increased aviation traffic required to service rising demand for international tourism will generate $\mathrm { C O } _ { 2 }$ emissions with negative implications for climate change. To confirm this hypothesis we will estimate the following model (with lower case letters used to denote logged variables): 


Table 7.1 EViews output table: OLS estimation


<table><tr><td colspan="5">Dependent Variable: Aircraft emissions (logged)</td></tr><tr><td colspan="5">Method: Least Squares</td></tr><tr><td colspan="5">Sample: 1971 2003</td></tr><tr><td colspan="5">Included observations: 33</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>2.30</td><td>0.12</td><td>19.94</td><td>0.00</td></tr><tr><td>Tourist arrivals (logged)</td><td>0.54</td><td>0.02</td><td>27.90</td><td>0.00</td></tr><tr><td>R-squared</td><td>0.96</td><td colspan="2">Mean dependent variable</td><td>5.50</td></tr><tr><td>Adjusted R-squared</td><td>0.96</td><td colspan="2">F-statistic</td><td>778.16</td></tr><tr><td>Sum squared residuals</td><td>0.07</td><td colspan="2">Prob(F-statistic)</td><td>0.00</td></tr><tr><td>Durbin-Watson statistic</td><td>0.74</td><td></td><td></td><td></td></tr></table>

$$
y _ {t} = \alpha + \beta x _ {t} + \varepsilon_ {t}\tag{7.1}
$$

where y is aviation emissions (logged) and x is tourism arrivals (logged). 

Using this model we estimate the following SRF using time-series data from 1971 to 2003 (n = 33): 

$$
y _ {t} = \hat {\alpha} + \hat {\beta} x _ {t} + \hat {\varepsilon} _ {t}\tag{7.2}
$$

Table 7.2 shows the EViews output table from the estimation of (7.2). 

The results from the estimation of (7.2) can be summarised as follows: 

$$
\begin{array}{l l} \hat {y} _ {t} & = \\ & (0. 1 2) \\ & t = 1 9. 9 4 \\ & p = 0. 0 0 \\ R ^ {2} = 0. 9 6 \end{array} \qquad \begin{array}{l l} 2. 3 0 & + 0. 5 4 x _ {t} \\ (0. 1 2) & (0. 0 2) \\ & t = 2 7. 9 0 \\ & p = 0. 0 0 \end{array}
$$

Durbin–Watson test = 0.74 

Initially, these results look good and confirm our assertion that aviation emissions are associated with rises in international tourist traffic. Our t test on $H _ { 0 } \colon \beta = 0$ versus $H _ { 1 } \colon \beta \neq 0$ , gives $p { = } 0 . 0 0$ and, at a 5% significance level, we can safely reject the null hypothesis of no association between y and x. The $R ^ { 2 }$ suggests that 96% of the variability in y is captured by variability in x – a high degree of ‘explanatory’ power and this is confirmed by the F test of explanatory power. The EViews printout also contains a statistic for a test not yet mentioned – the Durbin–Watson test which will be explained in detail below. 

As emphasised in the preceding chapter, we cannot assume that these are reliable results until we have established that the Gauss–Markov assumptions underlying OLS estimation have been satisfied. In this chapter, we will focus on the problem of autocorrelation or serial correlation and we will explore this assumption in assessing our regression results. 

## What is autocorrelation?

To define autocorrelation mathematically and in terms of the Gauss–Markov theorem: it involves the violation of the Gauss–Markov assumption that $\operatorname { c o v } ( \varepsilon _ { i } , \varepsilon _ { j } ) = 0 , i \neq j .$ . In words, autocorrelation is the violation of the assumption that the covariance between error terms is zero. For OLS to work effectively, the residuals from our regression should only capture random and excluded unimportant factors. Autocorrelation (in the residuals) is a problem that occurs when residuals from a sample regression are not random because they correlate with each other either over time or over space. If we have any sort of systematic pattern between our residuals, then some of the systematic influences that should be captured by the deterministic part of our model may be mistakenly picked up by the residual and OLS will be less accurate as a consequence. Whilst autocorrelation is commonly a time-series problem it can exist in crosssectional datasets too. In a cross-sectional context, spatial autocorrelation may occur if neighbouring countries have similar conditions and institutional structures; also there may be spillover effects between countries that are close in terms of geography because those countries may also be similar in terms of socio-economic and cultural conditions. 

It is important to note that the key symptom of autocorrelation is systematic patterns in the residuals and these can be a symptom of something other than pure autocorrelation, for example one or more of the following problems: 

 heteroscedasticity (explained in Chapter 6) 

 model misspecification (explained in Chapter 8) 

 endogeneity (explained in Chapter 9) 

 structural breaks (explained in Chapter 9) 

 non-stationarity (explained in Chapter 10) 

When systematic patterns in residuals are reflecting these more complex problems, the consequences may be more severe and the solutions more complicated. So it is important to spend some time identifying the exact cause of the autocorrelation in residuals before deciding what to do next. 

## Consequences of autocorrelation

When the ‘no autocorrelation’ assumption is violated, OLS will no longer be BLUE. OLS estimators will remain unbiased and consistent (as long as nothing more sinister is happening) but they will not be BLUE because they will not be the minimum variance unbiased estimator. (These consequences are similar to the consequences from heteroscedasticity, outlined in Chapter 6, because both are about systematic patterns in the random error term.) For OLS estimation in the presence of autocorrelation, the variances and standard errors will be larger and confidence intervals wider. This is because not all systematic information is being captured by the deterministic part of the regression model; instead, some of it is being mistakenly attributed to the residual. 

## Detecting autocorrelation

As explained above, autocorrelation is a problem that manifests itself via systematic patterns in the residuals from a regression. So the simplest method for identifying autocorrelation is a visual inspection of plots of residuals. In addition, various diagnostic tests exist which, in essence, quantify these systematic residual patterns. There are a number of different autocorrelation tests and here we will explain two common tests: the Durbin–Watson test and the Breusch–Godfrey LM test. 

## Visual inspection

Figure 7.2 is an EViews plot of the actual and fitted values from the OLS regression together with a plot ofthe residuals. (As explained in Chapter 1, the residual for each observation is the vertical distance between the observed value and the fitted value.) Visual inspection ofthese plots is often the first and quickest way to spot a potential problem. 

What are we looking for? In Figure 7.2, you may notice that there are relatively long runs of initially negative but then positive gaps between actual and observed values; the residuals are not spread randomly across the sample, suggesting that there is some systematic positive correlation between residuals. These systematic waves ofpositive and then negative residuals suggest a problem of positive autocorrelation, which occurs when one residual is a positive function of its predecessor. (It is also possible to have negative autocorrelation; in this case one residual will be a negative function of its predecessor and the residuals would zig-zag up and down more frequently than randomly generated residuals. Whilst negative autocorrelation is a less common problem and has different underlying causes, nonetheless it will generate similar problems and consequences to positive autocorrelation.) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/52a0d8e2-947d-4664-8ec8-aaf319076755/ac4a7e907e866cf428a912ecacbf13869a30882a623727162421ee8c808e024c.jpg)



Figure 7.2 EViews plot of residuals from estimation of Equation (7.2)


## Diagnostic tests

Visual patterns can be difficult to detect and will inevitably involve some degree of subjectivity, particularly in borderline cases. So there are many autocorrelation tests designed to pick up correlations between residuals. The classic test for autocorrelation is the Durbin–Watson (DW) test, routinely reported by most econometrics packages. We explain this test here because it is so widely known and used but it is important to remember that the DW test suffers from a number of limitations, and these are discussed in more detail below. 

The DW test is designed to pick up autocorrelation of the following form: 

$$
\varepsilon_ {t} = \rho \varepsilon_ {t - 1} + v _ {t}\tag{7.3}
$$

where $\varepsilon _ { t }$ is the error term and $\upsilon _ { t }$ is a stochastic error term. (A stochastic error is a randomly generated error process with a mean of zero and is sometimes referred to as a white noise error process.) The model in (7.4) focusses on the association between the error and one lag of itself, i.e. it is a first-order autoregressive process. In technical notation, it is an AR(1) process, i.e. a process in which a variable is a function of just one lag of itself (auto = self; regressive = related to the past). The DW test is designed to pick up AR(1) autocorrelation and so tests the following null and alternative hypotheses: 

$$
H _ {0} \colon \operatorname{cov} (\varepsilon_ {t}, \varepsilon_ {t - 1}) = 0\tag{7.4}
$$

$$
H _ {1} \colon \operatorname{cov} (\varepsilon_ {t}, \varepsilon_ {t - 1}) \neq 0
$$

The Durbin–Watson statistic is constructed around the sum of squared differences between successive residuals expressed as a ratio of the residual variance and can be calculated using the following formula: 

$$
\hat {d} = \frac {\sum (\hat {\varepsilon} _ {t} - \hat {\varepsilon} _ {t - 1}) ^ {2}}{\sum \hat {\varepsilon} _ {t} ^ {2}}\tag{7.5}
$$

If there is negative autocorrelation then the squared differences between successive residuals will be relatively large and d will be relatively large too, with an upper bound of 4. If there is positive autocorrelation then the squared differences between successive residuals will be relatively small and d will tend towards zero. 

If there is no autocorrelation: the differences will be random and then d will fall between 0 and 4, i.e. somewhere around 2. 

One of the limitations of the DW test lies in the complexity of its decision rules. In deciding whether or not the DW test result is revealing autocorrelation, the critical values for DW are found using k (the number of explanatory variables) and n (the number of observations). DW tables give two critical values each time, an upper value $( d _ { \mathrm { U } } )$ and a lower value $( d _ { \mathrm { L } } )$ . The decision rules given these critical values are summarised in Table 7.2. 

For our estimation, we have $\hat { d } = 0 . 7 4$ (see Table 7.1). From the DW tables (we have $k = 1$ and $n = 3 3 )$ using a 5% significance level, we get $d _ { \mathrm { U } } = 1 . 5 1$ and $d _ { \mathrm { L } } \mathrm { = } 1 . 3 8$ . Following the decision rules summarised in Table 7.2, since $\hat { d } < d _ { \mathrm { L } }$ we must reject $H _ { 0 }$ and conclude that there is significant evidence of positive serial correlation in the residuals from our estimation of Equation (7.2). 


Table 7.2 Decision rules for the Durbin–Watson (DW) test


<table><tr><td>If →</td><td>0 &lt; d̂ &lt; dL</td><td>dL &lt; d̂ &lt; dU</td><td>dU &lt; d̂ &lt; 4 - dU</td><td>4 - dU &lt; d̂ &lt; 4 - dL</td><td>4 - dL &lt; d̂ &lt; 4</td></tr><tr><td>Then →</td><td>Reject H0</td><td>No decision possible</td><td>Do not reject H0</td><td>No decision possible</td><td>Reject H0</td></tr><tr><td>Inference →</td><td>Positive serial correlation</td><td>?</td><td>No significant serial correlation</td><td>?</td><td>Negative serial correlation</td></tr></table>

## Problems with the DW test

There are a number of problems with the Durbin–Watson test. It is a clumsy test to use because, as noted above and in Table 7.2, there are two zones of indecision between the values $d _ { \mathrm { L } } { < } \hat { d } { < } d _ { \mathrm { U } }$ and $4 - d _ { \mathrm { U } } < \hat { d } < 4 - d _ { \mathrm { L } }$ . In these zones no conclusions can be drawn at all. Also as mentioned above, the DW will only pick up AR(1) autocorrelation i.e. correlation between successive residuals; it won’t automatically pick-up correlations with residuals that are more than one ‘step’ behind; for example in quarterly data we may expect that residuals in one period are correlated with residuals a year ago, i.e. four steps behind and the DW test will not capture this form of autocorrelation. Also, DW will not work when there’s a lagged dependent variable in the model: in this case $\hat { d }$ will be biased towards 2 and so will not be a powerful test of our $H _ { 0 }$ . This is because the probability of Type II error (incorrectly retaining the false null of no autocorrelation) will be relatively high when $\hat { d }$ is close to 2 and so we will be more likely wrongly to conclude that there is no significant autocorrelation. This last problem can be addressed by adapting the procedure to derive Durbin’s h test; Durbin’s h test is a relatively powerful test for autocorrelation in the presence of a lagged dependent variable and it is easier to interpret because it follows a standard normal distribution. But, like the DW test, it will only pick up AR(1) autocorrelation. 

Given the problems with DW, it is generally a good idea to conduct additional tests for autocorrelation. There are many alternatives to the DW test but a widely used test is the Breusch–Godfrey Lagrange Multiplier test (BG test). This test can pick up higher-order autocorrelation and can be calculated by many econometrics packages, including EViews. It is also a more powerful test than the DW because it isn’t biased towards a nonrejection of the null when a lagged dependent variable is included. This test is constructed by saving the residuals from the original regression and then conducting an auxiliary regression to estimate the relationship between a given residual and various lags of itself. Whilst the BG test can be constructed to detect higher-order autocorrelation we will first illustrate the AR(1) case, in which the form of this auxiliary regression would be: 

$$
\hat {\varepsilon} _ {t} = \phi + \gamma x _ {t} + \rho_ {1} \hat {\varepsilon} _ {t - 1} + v _ {t}\tag{7.6}
$$

where $\phi$ is the intercept in the auxiliary regression, x is the explanatory variable from the original model, γ is the slope parameter on x and $\rho$ is the parameter on the lagged residuals. An F version of this test can be constructed by comparing the RSS from Equation (7.6) with the RSS from a restricted version of Equation (7.6) which excludes the lagged residual: 

$$
\hat {\varepsilon} _ {t} = \phi + \gamma x _ {t} + v _ {t}\tag{7.7}
$$

The RSS from (7.6) and (7.7) are compared using an F test of restrictions (this test is explained in Chapter 5). The degrees of freedom on this F test will be F $( r , n - k - 1 - r )$ where r is the order of autocorrelation encapsulated within the unrestricted auxiliary equation. In the case of a test for AR(1) autocorrelation in an estimation with one explanatory variable and n = 33, the degrees of freedom will be F(1,30). 

Significant differences between the RSSs in the unrestricted and restricted models will be associated with large, significant F values. So the decision rule on the BG test is: if $F > F _ { \mathrm { c r i t } }$ then reject $H _ { 0 }$ 

The intuition underlying this test is that if there is a systematic pattern in the residuals then there will be statistically significant associations between residuals in time t and lagged residuals. So the RSS from the auxiliary regression will increase significantly when lagged residuals are dropped in a restricted version of (7.7); F will be greater than $F _ { \mathrm { c r i t } } .$ 

As mentioned above, the BG test can also be tailored to pick up higherorder autocorrelation. For example if we wanted to investigate the possibility of AR(5) autocorrelation, the unrestricted auxiliary regression would be: 

$$
\hat {\varepsilon} _ {t} = \phi + \gamma x _ {t} + \rho_ {1} \hat {\varepsilon} _ {t - 1} + \rho_ {2} \hat {\varepsilon} _ {t - 2} + \rho_ {3} \hat {\varepsilon} _ {t - 3} + \rho_ {4} \hat {\varepsilon} _ {t - 4} + \rho_ {5} \hat {\varepsilon} _ {t - 5} + v _ {t}\tag{7.8}
$$

The restricted version would be the same as for the AR(1) version, as outlined in Equation (7.7). For a sample of 33 observations with one explanatory variable, the degrees of freedom on the test would be F(5, 26). 

EViews will do BG tests and for our example we use EViews to test for AR(5) autocorrelation in our estimation of international aircraft emissions. The results from this EViews test are summarised in Table 7.3. 

Given $\hbar < 0 . 0 5$ we can reject the null of no autocorrelation. There is a significant problem of serial correlation in this sample and this result confirms the findings from the visual inspection and the Durbin–Watson test. The EViews BG tables also give more detailed information about the impact of lagged residuals. The results from the estimation of the auxiliary regression are summarised in Table 7.3 under ‘Test equation’. Although this information does not give a very rigorous test for the detailed nature of the associations between residuals and their lags, the fact that the only significant parameter is the one on the first lag of the residuals, may suggest that the autocorrelation we are detecting in our model of aircraft emissions is AR(1) 


Table 7.3 Breusch–Godfrey LM tests from EViews


<table><tr><td>F-statistic</td><td>3.92</td><td>Probability</td><td></td><td>0.01</td></tr><tr><td>Obs*R-squared</td><td>14.19</td><td>Probability</td><td></td><td>0.01</td></tr><tr><td colspan="5">Test Equation:Dependent Variable: RESID = residualsMethod: Least Squares</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>-0.01</td><td>0.10</td><td>-0.10</td><td>0.92</td></tr><tr><td>Tourist arrivals (logged)</td><td>0.00</td><td>0.02</td><td>0.11</td><td>0.91</td></tr><tr><td>RESID(-1)</td><td>0.73</td><td>0.20</td><td>3.70</td><td>0.00</td></tr><tr><td>RESID(-2)</td><td>-0.20</td><td>0.24</td><td>-0.82</td><td>0.42</td></tr><tr><td>RESID(-3)</td><td>0.19</td><td>0.25</td><td>0.77</td><td>0.45</td></tr><tr><td>RESID(-4)</td><td>-0.17</td><td>0.26</td><td>-0.66</td><td>0.52</td></tr><tr><td>RESID(-5)</td><td>-0.05</td><td>0.24</td><td>-0.21</td><td>0.84</td></tr><tr><td>R-squared</td><td>0.43</td><td>Sum squared residuals</td><td></td><td>0.04</td></tr><tr><td>Adjusted R-squared</td><td>0.30</td><td>F-statistic</td><td></td><td>3.27</td></tr><tr><td>Durbin-Watson statistic</td><td>2.01</td><td>Prob(F-statistic)</td><td></td><td>0.02</td></tr></table>

autocorrelation. (As we will show below, the fact that a corrective procedure based around an assumption of AR(1) correlation eliminates the problem from our estimation does suggest that our tentative inference about AR(1) autocorrelation has some basis.) 

## Correcting autocorrelation

We have emphasised that it is important to think about the various possible reasons for the symptom of correlated residuals but assuming that the autocorrelation detected in our SRF is not a sign either of model misspecification, structural breaks and/or non-stationarity (problems which are explained in subsequent chapters), we will illustrate a classic solution to autocorrelation based around a Generalised Least Squares (GLS) procedure – as explained in Box 7.2. 

## Box 7.2 Generalised least squares (GLS) to correct autocorrelation

As its name suggests, GLS is a generalisation of the least squares principle and was introduced in Chapter 6 in the context of heteroscedasticity. In the context of autocorrelation, GLS is adapted to extract out the systematic patterns in the autocorrelated errors in the following way: 

Taking an empirical model of the form: 

$$
y _ {t} = a + \beta x _ {t} + \varepsilon_ {t}\tag{7.9}
$$

If successive errors are correlated then: 

$$
\varepsilon_ {t} = \rho \varepsilon_ {t - 1} + v _ {t}\tag{7.10}
$$

where $\upsilon _ { t }$ is a stochastic, white noise error term with a mean of zero. 

This autocorrelation will generate inefficiency in OLS: OLS will not be estimated as accurately as possible because it is not capturing the systematic pattern in the error ε. In addition, the standard errors will be estimated wrongly and so the t tests from the original regression will be incorrectly calculated. 

To correct this problem we need to incorporate all the systematic information into the deterministic component of our regression model in order to create a model with a white noise error $\boldsymbol { \upsilon } _ { t }$ 

Using the information from Equation (7.10) we can transform our model by lagging Equation (7.9), multiplying it by $\rho$ to give: 

$$
\rho y _ {t - 1} = \rho a + \rho \beta x _ {t - 1} + \rho \varepsilon_ {t - 1}\tag{7.11}
$$

Subtracting (7.11) from (7.9) gives: 

$$
y _ {t} - \rho y _ {t - 1} = (1 - \rho) a + \beta (x _ {t} - \rho x _ {t - 1}) + (\varepsilon_ {t} - \rho \varepsilon_ {t - 1})\tag{7.12}
$$

$$
\mathsf {S o} \quad y _ {t} ^ {*} = \varphi + \beta x _ {t} ^ {*} + (\varepsilon_ {t} - \rho \varepsilon_ {t - 1})\tag{7.13}
$$

where 

$$
y _ {t} ^ {*} = y _ {t} - \rho y _ {t - 1}, x _ {t} ^ {*} = x _ {t} - \rho x _ {t - 1} \text { and } \varphi = (1 - \rho) a\tag{7.14}
$$

Remember that $\xi _ { t } = \rho \varepsilon _ { t - 1 } + \upsilon _ { t }$ (from Equation (7.10)) which can be rearranged to show that the stochastic error in (7.13) is given by the random white noise error term, $\upsilon _ { t }$ i.e. $\varepsilon _ { t } - \rho \varepsilon _ { t - 1 } = U _ { t } .$ All systematic influences are now captured within the deterministic portion of the model. In this case, OLS will be consistent. It will also be BLUE in small samples if x is strictly exogenous, i.e. if x exhibits no correlation with the error (Stock and Watson, 2003, p. 514). However, we will lose one degree of freedom in transforming our variables. Furthermore, the inclusion of the lagged dependent variable will create problems for linear estimation of (7.12) but these difficulties are beyond the scope of this chapter. 

In a sample context we can ‘clean $\mathsf { u p ^ { \prime } }$ the autocorrelated residuals using this approach. But to do this we need an estimate of the autocorrelation paramete ${ \cdot } \hat { \rho } .$ There are many ways to get an estimate of ${ \hat { \rho } } .$ One method is a grid search procedure, i.e. experimenting with different values of $\hat { \rho }$ to see which gives the best $R ^ { 2 }$ . Another way is to make some assumptions about $\hat { \rho } -$ for example by using information from previous analyses. One of the most famous methods for getting an estimate of $\rho$ is the Cochrane–Orcutt (C–O) 

procedure. This involves running the OLS regression, saving the residuals and running an auxiliary regression of the residuals on the residuals as follows: 

$$
\hat {\varepsilon} _ {t} = \hat {\rho} \hat {\varepsilon} _ {t - 1}\tag{7.15}
$$

The parameter on the lagged residual will give an estimate of $\rho .$ Below, this procedure is applied to our emissions–tourism example. It is important to remember that this C–O procedure suffers from the limitations outlined above. It is also important to remember that it will only work for AR(1) autocorrelation and the procedure would have to be extended for higher orders of autocorrelation. 

## The Cochrane–Orcutt (C–O) two stage procedure

The C–O procedure can be performed in complex ways (e.g. by using iterative solutions to identify $\hat { \rho } )$ but the simplest version, the C–O two stage procedure, can be used to correct the problem of autocorrelation in our estimation of (7.2) as follows:. 

1. Run an OLS regression on (7.2) and save the residuals, $\widehat { \varepsilon } _ { t }$ 

2. Run an auxiliary regression of the residuals in period t on the residuals in period t − 1. For our data, this auxiliary regression gave the following result: 

$$
\hat {\varepsilon} _ {i} = 0. 6 3 \hat {\varepsilon} _ {i - 1} + \hat {v} _ {t} \quad \rightarrow \hat {\rho} = 0. 6 3\tag{7.16}
$$

3. Using $\hat { \rho } = 0 . 6 3$ as identified in step (2), we transform our variables as follows: 

$$
y _ {t} ^ {*} = y _ {t} - 0. 6 3 y _ {t - 1}\tag{7.17a}
$$

$$
x _ {t} ^ {*} = x _ {t} - 0. 6 3 x _ {t - 1}\tag{7.17b}
$$

4. Then we run a regression of $y ^ { * }$ on $x ^ { * }$ , noting that (7.14) implies a new intercept term in our transformed model; however this intercept will still be a constant (as it is an amalgam of constants itself) and so the change in the intercept will have no specific implications for our new estimation. 

The results from the estimation of this transformed model (including diagnostic tests) are summarised in Table 7.4a. Overall, our corrective GLS procedure appears to have worked well and for our final regression the Breusch–Godfrey test indicates that any inefficiency in OLS estimation created by an autocorrelation problem has been eliminated by using the GLS estimator. The results from the BG test for higher-order autocorrelation (shown in Table 7.4b) indicate that, even at very low significance levels, we can retain the null of no AR(5) autocorrelation. 


Table 7.4a GLS estimation of tourism arrivals and aviation emissions (Cochrane–Orcutt procedure)


<table><tr><td colspan="5">Dependent Variable: y*</td></tr><tr><td colspan="5">Method: Least Squares</td></tr><tr><td colspan="5">Sample (adjusted): 1972 2003</td></tr><tr><td colspan="5">Included observations: 32 after adjustments</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>0.84</td><td>0.10</td><td>8.56</td><td>0.00</td></tr><tr><td>x*</td><td>0.55</td><td>0.04</td><td>12.33</td><td>0.00</td></tr><tr><td>R-squared</td><td>0.84</td><td colspan="2">Mean dependent variable</td><td>2.06</td></tr><tr><td>Adjusted R-squared</td><td>0.83</td><td colspan="2">F-statistic</td><td>152.06</td></tr><tr><td>Sum squared residuals</td><td>0.04</td><td colspan="2">Prob(F-statistic)</td><td>0.00</td></tr><tr><td>Durbin-Watson statistic</td><td>1.82</td><td></td><td></td><td></td></tr></table>


Table 7.4b Breusch–Godfrey LM test


<table><tr><td>F-statistic</td><td>0.21</td><td>Probability</td><td></td><td>0.95</td></tr><tr><td>Obs*R-squared</td><td>1.31</td><td>Probability</td><td></td><td>0.93</td></tr><tr><td colspan="5">Test Equation:Dependent Variable: RESID</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>0.00</td><td>0.11</td><td>0.00</td><td>1.00</td></tr><tr><td><eq>x^*</eq></td><td>0.00</td><td>0.05</td><td>-0.01</td><td>1.00</td></tr><tr><td>RESID(-1)</td><td>0.11</td><td>0.20</td><td>0.56</td><td>0.58</td></tr><tr><td>RESID(-2)</td><td>-0.14</td><td>0.20</td><td>-0.67</td><td>0.51</td></tr><tr><td>RESID(-3)</td><td>0.12</td><td>0.21</td><td>0.57</td><td>0.57</td></tr><tr><td>RESID(-4)</td><td>-0.12</td><td>0.23</td><td>-0.52</td><td>0.61</td></tr><tr><td>RESID(-5)</td><td>-0.01</td><td>0.27</td><td>-0.04</td><td>0.97</td></tr><tr><td>R-squared</td><td>0.04</td><td colspan="2">Mean dependent variable</td><td>0.00</td></tr><tr><td>Adjusted R-squared</td><td>-0.19</td><td colspan="2">F-statistic</td><td>0.18</td></tr><tr><td>Sum squared residuals</td><td>0.04</td><td colspan="2">Prob(F-statistic)</td><td>0.98</td></tr><tr><td>Durbin-Watson statistic</td><td>1.98</td><td></td><td></td><td></td></tr></table>

Note that all we have done here is transform our variables to allow more efficient estimation of our parameters. We are still estimating the α, β and γ from Equation (7.2); we’re just doing it more efficiently and accurately because we’ve incorporated information about the form ofthe autocorrelation into our estimation procedure. 

The results from our GLS C–O estimation are broadly similar to the results from the initial OLS estimation: our t test of $H _ { 0 } \colon \beta = 0$ against $H _ { 1 } \colon \beta \neq 0$ , gives $p { = } 0 . 0 0$ and so we can still safely reject $H _ { 0 }$ at a 5% significance level. There is a statistically significant, positive association between y and x: our results suggest that a 1% rise in international tourist arrivals will be associated with a 0.55% rise in international aircraft emissions. 

The F test of explanatory power also indicates that, even with very low significance levels, we can reject $H _ { 0 } \colon \beta = 0$ . For the $R ^ { 2 } { \mathrm { ; } }$ , 84% of the variability in $y ^ { * }$ is captured by variability in $x ^ { * }$ again confirming that the model overall has a high degree of ‘explanatory’ power. Using the Breusch–Godfrey test and a 5% significance level we can retain the null of no AR(5) autocorrelation in the residuals. Whilst the basic results from our GLS estimation are similar to the results from the OLS estimation, they are in fact a lot more plausible because we have adapted our technique to match the Gauss–Markov assumption of no autocorrelation in the errors. 

We have identified a positive and significant relationship between international aircraft emissions and international tourist arrivals. But whilst our initial findings do suggest that controlling international tourist traffic may be crucial in moderating aviation emissions, statistically it is important to note that, whilst we have addressed the problem of autocorrelation, there may be other, more complex problems with our statistical analysis, e.g. nonstationarity. These problems are explored in subsequent chapters. 

## 7.5 Implications and conclusions

Ifour empirical results are robust, then they suggest a worrying future for climate change. With increasing numbers ofdeveloping countries building prospects for growth around their tourism industries, and with rising incomes in the developed world, it seems likely that international tourist traffic will continue to rise in the future. Similarly the growth of the cheap airline industry in many OECD countries will do little to reverse the growth in international tourism. The results from this chapter suggest that these increasing flows of tourists are likely to be associated with significant increases in international aircraft emissions. 

Drawing a parallel with the Prisoner’s Dilemma problem outlined in the theory section, there will be no market incentive for any given individual to moderate their own international travel if others are continuing to travel. Although public awareness of environmental change has been increasing, the focus on sustainable tourism and ecotourism may do little to moderate climate change emerging from aviation because many ecotourism resorts and activities are concentrated in exotic destinations, far away from the homes of the tourist customers. 

In terms ofsolutions to the problem, the growth of‘carbon offset’ and ‘carbon balancing’ schemes may do something to reduce the impact of tourism on climate change – if airlines and tourists can be persuaded to compensate for negative environmental externalities generated from aviation emissions by charging and paying higher prices for air travel. As for government policy: in moderating the extent of climate change governments may have to include measures to quell the demand for international tourism. Some policy solutions include fuel taxes, tradeable emissions permits, landing charges and arrival/ departure taxes. All these measures would raise the relative cost ofinternational tourism. However, these sort of policies require international co-operation because the Prisoner’s Dilemma may operate on an international scale: individual countries are unlikely unilaterally to impose new taxes and charges on their own tourism industries in the hopes ofsaving the environment ifthe most likely outcome is that tourists will just go somewhere cheaper for their annual holiday. 

## 7.6

## Further reading

## Textbooks



Holden, A. (2000) Environment and Tourism, London: Routledge. 





Opperman, M. and Chon, K-S. (1997) Tourism in Developing Countries, Thomson Business Press. 





Stock, J. H. and Watson, M. W (2003) Introduction to Econometrics, Harlow: Pearson Education Addison-Wesley. 





Varian, H. (2006) Intermediate Microeconomics 7th edition, London: W. W. Norton & Co. Chapter 34 (on the tragedy of the commons and environmental externalities). 



## Academic articles and working papers



Baddeley, M. (2004) ‘Are tourists willing to pay for aesthetic quality? An empirical assessment from Krabi Province, Thailand, Tourism Economics, vol. 10, no. 1, 45–61. Reprinted in T. Hybers (ed.) (2007), Economics and Management of Tourism 2 – Tourism in Developing Countries, Cheltenham: Edward Elgar, pp. 608–24. 





Hardin, G. (1968) ‘The Tragedy of the Commons’, Science, vol. 162, no. 3859, 1243–7. 



## Newspaper articles

The Economist (2008) ‘Commons sense: Why it still pays to study medieval English landholding and Sahelian nomadism’, 31 July 2008. 

## Policy reports



Penner, J. E., Lister, D. H., Griggs, D. J., Dokken, D. J. and Mcfarland, M. (1999) Aviation and the Global Atmosphere – Summaryforpolicy makers, Intergovernmental Panel on Climate Change: Cambridge: Cambridge University Press. Downloadable from www.ipcc.ch/pdf/ special-reports/spm/av-en.pdf 





Roe, D., Ashley, C., Page, S. and Meyer, D. (2004) Tourism and the Poor: Analysing and Interpreting Tourism Statistics from a Poverty Perspective, ProPoor Tourism Working Paper No. 16, March, London: Pro Poor Tourism (PPT). 





Stern, N. (2006) The Stern Review Report on the Economics ofClimate Change, Cabinet Office – HM Treasury/Cambridge University Press, Cambridge UK. 





UNWTO (annual) Tourism Market Trends, Madrid: UN World Tourism Organisation. 



## 7.7

## Chapter exercises

1. Using the data sources outlined above, collect data on aircraft emissions and tourist arrivals and then: 

(a) Estimate an autoregressive distributed lag (ARDL) model of aircraft emissions of the following form: $y _ { t } = \alpha + \lambda y _ { t - 1 } + \beta _ { 1 } x _ { t } + \beta _ { 2 } x _ { t - 1 } + \varepsilon _ { t }$ 

(b) Test for AR(1) autocorrelation in the errors explaining which test(s) you’ve used and why you’ve used them. 

(c) Test for AR(5) autocorrelation in the errors explaining which test(s) you’ve used and why you’ve used them 

(d) What do the tests for autocorrelated residuals reveal? 

(e) Explain how and why the ARDL estimation has/hasn’t worked. 

2. In the discussion of autocorrelation, we outlined a number of explanations for systematic patterns. Discuss the plausibility of these explanations in the context of the relationship between aviation emissions and tourist arrivals as analysed in this chapter. 

# Model misspecification Tobin’s q and investment in the USA

Economic issues include: 

 Tobin’s q theory 

 The Efficient Markets Hypothesis 

 Psychology, behavioural economics and neuroeconomics 

Econometric issues include: 

 Identifying correct functional form 

 Model misspecification errors 

 Ramsey’s RESET tests for model misspecfication 

Data issues include: 

 Measuring stock market value 

 Measurement error 

## 8.1 The issue

In this chapter, stock market valuation methods of investment appraisal are introduced and applied to US fixed asset investment data. In a simple world, business entrepreneurs use two factors of production when they are producing their goods and services: capital and labour. Fixed asset investment is about the first. As businesses invest in new plant, machinery and equipment they generate a flow of new capital goods into the stock of capital. This capital stock (when combined with labour inputs) will determine the future productive capacity both of the firm at a microeconomic level and of the macro-economy as a whole. 

Some early investment theories focused on investment as the outcome of firms balancing the marginal benefits and marginal costs of buying units of new capital but these theories could not easily explain the timing of investment decisions. Also, they neglected the role of expectations and uncertainty. 

<!-- === Source: MinerU_markdown_Baddeley_M.C.,_Barrowclough_D.V._-_Running_Regressions__A_Practical_Guide_to_Quantitative_Research_in_Economics_._-CUP_(2009)_201_2122707855927779341.md (Page 201) === -->

This was an important omission because investment is all about planning for the future: expectations and uncertainty have crucial impacts on entrepreneurial decision-making. The problem is that expectations are not observable and so one solution is to use stock market data on market capitalisations to capture investors’ expectations about the future, as explained below. This approach forms the basis of Tobin’s $q$ theories of investment and in this chapter we investigate variants of $q$ theory to assess their empirical performance in capturing aggregate investment in the USA from 1987 to 2004. 

## 8.2 The theory

Lots of investment theories have evolved over the years.<sup>1</sup> Early accelerator theories focussed on explaining investment as a process of capital stock adjustment, asserting that entrepreneurs invest to build up their capital stock to meet future sales demand and using past output growth to proxy future sales demand. This capital stock adjustment approach was developed in Jorgenson’s influential neo-classical investment theory (Jorgenson, 1963) but, according to Jorgenson, investment is also a function of the user cost of capital – a measure of the opportunity costs of spending money on investment projects. The user cost includes interest costs, depreciation from wear-and-tear, and the capital gains or losses from changes in the value of capital goods. It is defined as: 

$$
c = r + \delta - \dot {p} _ {k}\tag{8.1}
$$

where r = the real interest rate; $\delta$ is the depreciation rate on capital equipment and $\dot { p } _ { k }$ captures capital appreciation from relative changes in the value of capital goods. Note that capital appreciation will reduce the opportunity costs of investment and so the sign on $\dot { P } k$ is negative. 

There are two main shortcomings with Jorgenson’s theory. First, it assumes static, unchanging expectations. Second, it assumes that there are no adjustment costs but if there are no adjustment costs then the rate of investment over time will be undefined. Tobin’s q theory addresses some ofthe limitations in Jorgenson’s theory by incorporating adjustment costs into the investment decision-making process, focussing in particular on internal adjustment costs. Internal adjustment costs emerge from disruptions to the production process as new capital goods are ‘broken-in’ and workers are re-trained. With increasing investment more workers are needed to ‘bolt-down’ new equipment and there are increasing demands on managerial time. This means that adjustment costs will be a convex function of new investment, i.e. adjustment costs will increase at an increasing rate as investment increases. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/84d7ab0b57876b490efc30c3fb9c45d22e69a38c0dbdf6a971cf8444831a6013.jpg)



Figure 8.1 Adjustment costs and optimal investment


Figure 8.1 illustrates the basic concepts of adjustment cost theory and shows that optimal investment and maximum profits will occur at the point where expected marginal revenue balances all the marginal costs, including the adjustment costs. The total revenue curve shows expected revenues increasing but at a decreasing rate reflecting the diminishing marginal productivity of new investment; the slope is decreasing as new investment increases. The convexity of adjustment costs can be seen in the shape of the adjustment costs curve: the slope is increasing because marginal adjustment costs increase as new investment increases. The user cost line has a constant slope: unlike adjustment costs, the first unit of new investment is affected by the same user costs (interest, appreciation and changes in the value of capital goods) as the last unit of new investment. The total costs curve is the vertical sum of the user cost and adjustment cost curves and so it will be convex because the adjustment costs curve is convex. Profits from new investments will be maximised when the marginal benefits of investment (in terms of expected revenues) are balanced by the marginal costs. It is important to note that the marginal benefits of investment are marginal revenues and so are captured by the slope on the expected revenue curve; the marginal costs are captured by the slope on the total costs curve; when these two slopes are equal, i.e. when the lines are parallel, marginal benefits and marginal costs will be equal and profits will be maximised. This occurs at I*, which is the optimal level of investment. 

The q theorists explain this balancing of benefits and costs using the concept of marginal q $( q _ { \mathrm { M } } )$ , which is the shadow price of investment – in this case the increment to total revenue expected from a unit increase in the marginal costs. In other words, it is the ratio of the marginal benefits in terms of revenue (MB) and marginal costs (MC) including user cost and marginal adjustment costs. At the point of optimal investment, ${ \mathrm { M B } } = { \mathrm { M C } }$ and $q _ { \mathrm { M } } = 1$ At this point no new investments would be profitable (apart from replacement investment to replace worn-out plant and equipment etc.). When $\mathrm { M B } > \mathrm { M C } , q _ { \mathrm { M } }$ will be greater than 1 and firms should increase their capital stock by investing more: if a firm was to buy another unit of new investment then they would increase their profits (because the marginal benefits exceed the marginal costs). On the other hand, if ${ \mathrm { M B } } < { \mathrm { M C } }$ and $q _ { \mathrm { M } } < 1$ , then costs exceed benefits and so the firm should decrease its investment – if it can. But disinvestment is limited by the fact that it is difficult to sell second-hand investment goods given asset specificity (plant and equipment is not easy to re-sell if it is designed for a very specific purpose) and/or adverse selection (a type of asymmetric information which occurs when buyers are reluctant to buy second-hand goods because they cannot observe the hidden attributes of these goods). 

What use is $q _ { \mathrm { M } }$ in practice? It is not observable because the firm is assumed to be a ‘black box’ – its internal workings cannot be seen i.e. a firm’s managers cannot see the incremental output from each individual unit of capital, they see only the total output, inputs and costs. So because $q _ { \mathrm { M } }$ is unobservable a proxy is needed. Average $q \ ( q _ { \mathrm { A } } )$ can be used as a proxy. Average ${ \mathfrak { q } } \left( q _ { \mathrm { A } } \right)$ is the ratio of total benefits (TB) expected by a firm (from its production and investment) to the total cost (TC) that would be incurred if it had to replace its entire capital stock. If TB > TC then $q _ { \mathrm { A } } > 1$ and net investment should take place. The capital stock will increase from inflows of new investment but, because of the diminishing marginal productivity of capital, TC will increase at a decreasing rate until $\mathrm { T B } = \mathrm { T C } .$ . At this point the capital stock will be at its optimal level, $q _ { \mathrm { A } }$ will equal $q _ { \mathrm { M } }$ and both will be equal to unity. 

But profit-maximising firms operate at the margin, at least in theory, so what use is an average concept? This problem can be answered by assuming homogeneity of the capital stock and constant returns to scale, in which case marginal and average costs and benefits will be equal (Hayashi 1982). So although $q _ { \mathrm { M } }$ is unobservable, $q _ { \mathrm { A } }$ may be a good proxy and firms will respond to $q _ { \mathrm { A } }$ as if they know $q _ { \mathrm { M } }$ . In other words, even though $q _ { \mathrm { M } }$ is unobservable, $q _ { \mathrm { A } }$ will give a quantifiable measure of the incentive to invest. 

How do we measure $q _ { \mathrm { A } } { \mathrm { ? } }$ In this chapter we focus on one solution: Tobin’s q theory. Tobin’s $q$ is the ratio of the stock market valuation of a firm (MV) to the current replacement cost (CRC) of its capital stock. As explained in Box 8.1, MV will be a good proxy for firms’ expectations of future revenue from current investments assuming that share prices are a good signal of the profit expectations of entrepreneurs. CRC is the accounting or ‘book’ cost of firms’ existing productive capacity; for example, if a firm’s capital stock is ten sewing machines and each sewing machine costs $100 at current market prices, then the $\mathrm { C R C } = \$ 1000$ . Using these measures of MV and CRC, Tobin’s $q$ is calculated as: 

T bi ’ $q = { \frac { M V } { C R C } }$ 

(8:2) 

## Box 8.1 Measuring market value and efficient markets

A share in a company is like a little piece of that company. So the market value of the firm is just a firm’s share price multiplied by the number of issued shares. This gives a measure of the market valuation of an individual firm. For example, if Rolls Royce shares are trading at £5 each on the London Stock Exchange (LSE) and there are 1.8 billion shares in the company, then the market capitalisation for Rolls Royce will be £9 billion. 

Most world stock exchanges report their total market capitalisations. These are calculated simply by adding together the market capitalisations for all the firms listed on a stock exchange. For example, in 2007 there were 1139 firms listed on the main market of the LSE and the total market capitalisation of these companies was over £2 trillion (trillion = a million millions). In 2007 there were more than 2600 companies listed on the New York Stock Exchange (NYSE), with a total market capitalisation of US$22.6 trillion. 

Tobin’s q theory is based around the rational expectations hypothesis (REH) and the related efficient markets hypothesis (EMH). The REH is usually attributed to Muth who asserted that ‘expectations, since they are informed predictions of future events, are essentially the same as the predictions of the relevant economic theory’ (Muth 1961, p. 316). The EMH incorporates the REH in hypothesising that financial markets are ‘informationally efficient’, i.e. they ensure that share prices listed on stock exchanges fully reflect all relevant information available to rational investors. If financial markets are informationally efficient, then share prices will fluctuate completely and instantaneously to incorporate any informative news. If new information affecting the future prospects of a firm arrives, then the relative demand and supply for the shares of that firm will adjust instantaneously via arbitrage. For example if there is bad news about a company and its future profitability prospects look less impressive as a consequence, then demand for shares in that company will fall and more people will try to sell its shares as rational traders will adjust their willingness to pay downwards. So the share price will fall. In this way, share prices will adjust to reflect the fundamental value of a firm, i.e. the discounted stream of expected future profits or dividends emerging from the firm’s future production. Overall, REH and EMH together predict that share prices will provide an unbiased indicator of rational investors’ expectations of future profitability. 

If the efficient markets assumption is true, then it follows that the rational traders expectations about the future value of firms will be captured by the stock market capitalisation of the firm. Tobin’s q theorists argue that these stock market valuations will give an unbiased estimate of the future value of a firm’s production and investment. 

The ratio of total value and total costs gives a measure of average contribution of all new investment to total revenue: MV is capturing the total value and CRC is capturing the total cost and so Tobin’s q measures $q _ { \mathrm { A } }$ 

This theory follows Tobin’s interpretation of Keynes’s (1936) ideas about the role of the stock market in providing a measure of expectations about the expected future profits from new investments. (It is important to emphasise that Tobin’s q theory is based upon just one interpretation of Keynes; some economists argue that Keynes’s emphasis on crowd psychology and herd behaviour in financial markets is not consistent with Tobin’s q theories of investment because Tobin’s interpretation relies on assumptions of rational expectations and efficient markets, as also explained in Box 8.1.) 

As explained above, whilst $q _ { \mathrm { M } }$ is about the impacts of marginal additions to the capital stock via new investment it can be proxied by $q _ { \mathrm { A } }$ . Tobin’s q measures this average and so can be used to give investment decision rules, as outlined in Box 8.2. 

So far we have concentrated on the microeconomic aspects of investor decision-making but Tobin’s q theory can be transformed into an aggregate theory of macroeconomic investment by adopting a representative agent hypothesis, i.e. by assuming that all firms behave in the same way. If this is true then we can describe the aggregate behaviour of all firms by describing the behaviour of one representative firm. In the macroeconomic versions of Tobin’s $q$ theory, this means that the ratio of the stock market capitalisation for all listed companies on an exchange (as explained in Box 8.1) to the overall current replacement cost of all these companies’ capital stocks will give a measure of aggregate average q. In this chapter we will assess these aggregate versions of Tobin’s $q$ model of investment using US data to analyse the relationships between the rate of investment and Tobin’s measure of $q _ { \mathrm { A } } ,$ , as explained below. 


Box 8.2 Incentives to invest: $q _ { \mathsf { M } }$ and $q _ { \mathsf { A } }$


<table><tr><td><eq>q_{M}</eq></td><td><eq>q_{A}</eq> as a proxy for <eq>q_{M}</eq></td><td>Optimal choice</td></tr><tr><td><eq>q_{M} = \frac{MB}{MC} &gt; 1</eq></td><td><eq>q_{A} = \frac{MV}{CRC} = \frac{TB}{TC} &gt; 1</eq></td><td>→ increase investment</td></tr><tr><td><eq>q_{M} = \frac{MB}{MC} = 1</eq></td><td><eq>q_{A} = \frac{MV}{CRC} = \frac{TB}{TC} = 1</eq></td><td>→ replacement investment only</td></tr><tr><td><eq>q_{M} = \frac{MB}{MC} &lt; 1</eq></td><td><eq>q_{A} = \frac{MV}{CRC} = \frac{TB}{TC} &lt; 1</eq></td><td>→ disinvest (if possible)</td></tr></table>

## 8.3

## The data

The dependent variable used in this analysis will be the investment rate $\frac { I } { K } ,$ where I is corporate investment in the US (net of replacement investment) and K is the US corporate capital stock as measured by its current replacement cost. 

Tobin’s q is used as an explanatory variable in our investment models. As explained above, the essence of Tobin’s $q$ is that it is a measure of $q _ { \mathrm { A } }$ and so can be used as a proxy for $q _ { \mathrm { M } }$ . Tobin’s q model of investment rests on the assumption that stock market valuations capture the expected future profitability of companies’ capital stocks and so will determine investment activity. Following Equation (8.2): 

Tobin’s $q = { \frac { M V } { C R C } }$ 

(8:2) 

Calculating a simple version of Tobin’s q is relatively straightforward, though more complex versions do incorporate adjustments for taxation and depreciation. 


We collected data from the following sources:


<table><tr><td>Variable</td><td>Source</td><td>Website</td></tr><tr><td rowspan="2">Tobin&#x27;s q</td><td>Smithers and Wright (2000)</td><td>www.valuingwallstreet.com/</td></tr><tr><td>New York Stock Exchange</td><td>www.nyse.com</td></tr><tr><td>Investment rate (I/K)</td><td>Derived from National Income and Product (NIPA) accounts, US Bureau of Economic Analysis</td><td>www.bea.gov</td></tr></table>

The $q$ data from Smithers and Wright (2000) are based on stock market capitalisations on the New York Stock Exchange. Similar data on stock markets and investment for the UK can be collected via the LSE (www. londonstockexchange.com) and the Office of National Statistics (ONS) (www.statistics.gov.uk). 

In assessing the reliability of our data, it is important to note that we only have 18 observations and the very small size of our sample will limit the accuracy of our estimations. That said, we are forced to use a small number of observations because the data on Tobin’s $q$ is not very rich and detailed. Also, it is important to emphasise that not all firms are listed on the NYSE and so there will not be a match between the market capitalisation element of $q$ and the investment rate. But we will assume for simplicity that stock market capitalisations act as a signal to all firms planning to buy some new productive capacity, whether or not they are listed on the NYSE. 

Another issue to remember is that the true incentive to invest is given by $q _ { \mathrm { M } } ,$ an unobservable variable. As explained in Chapter 3, when data on a specific variable are unavailable (perhaps because the variable is unobservable and/or un-measurable), a proxy can be used in its place. A good proxy will be strongly correlated with the missing variable but uncorrelated with the error term of our regression. The rationale underlying Tobin’s $q$ models is that, given some assumptions, $q _ { \mathrm { A } }$ will be a good proxy for $q _ { \mathrm { M } } .$ . But proxy variables may still create problems because they will introduce measurement error into empirical models: the proxy is not the true explanatory variable and so cannot be perfectly correlated with it. Measurement error may emerge from using proxies for other reasons (e.g. unreliable statistical collection methods). In general, if measurement error affects the explanatory variable then it may create the problem ofendogeneity – a violation ofGauss–Markov assumptions which occurs when the explanatory variable is correlated with the error term. When the explanatory variable and error are correlated, OLS parameter estimates will pick up some of the influence of the errors and OLS 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/1c6340fb058f4bd3fc8ba86a3302ec831bf680c103adde3f958ab9eb18cdfda5.jpg)



Sources: BEA, Smithers and Wright (2000).


Figure 8.2 Corporate investment and Tobin’s q, USA 1987–2004 

estimation will be both biased and inconsistent. Issues of endogeneity are beyond the scope of this book but see Wooldridge (2003) for a thorough analysis of these issues. Putting these complexities to one side, we will start by looking at our data for our dependent variable (I/K) and explanatory variable (q). 

In Figure 8.2 the changes in the US corporate investment rate and Tobin’s q are plotted to depict the broad trends between q and investment during the years 1987–2004. Figure 8.2 shows that, whilst there are some periods of volatility in Tobin’s q (perhaps reflecting the dotcom boom of the early 1990s and the busts early in the new millennium), overall the series are fluctuating in similar ways. On the other hand, there are long periods in which Tobin’s q is above or below 1 suggesting that entrepreneurs are taking time to adjust their capital stocks in response to changes in market valuations. (The issue of lags is not explicitly addressed in this chapter but is covered in the chapter exercises.) In analysing whether or not these patterns translate into a robust relationship between the investment rate and Tobin’s q, we will run a regression of the investment rate on q, as outlined in the empirical section below. 

## 8.4 Empirical methods and results

Does Tobin’s $q$ theory capture the empirical evidence on aggregate investment? In this chapter we will answer this question by analysing the relationship between the investment rate (I/K) and Tobin’s $q \ ( q )$ using the following general model: 

$$
\frac {I _ {t}}{K _ {t}} = f (q _ {t})\tag{8.3}
$$

The issue that we will investigate in this chapter is the identification of the functional form of the relationship between the dependent and explanatory variables. This functional form captures the nature of the mathematical relationship between the dependent and explanatory variables. We need to decide is it linear or non-linear? If it’s non-linear, then what form does the non-linearity take? As explained in Box 8.3, identifying the correct functional form is important. Incorrect functional form is a type of model misspecification error and can have crucial implications for the applicability of OLS estimation. 

## Box 8.3 Model misspecification errors

Model misspecification bias occurs when an empirical model is constructed the wrong way. There are three main types of model misspecification error, all of which distort the relationship between observed data and their fitted values: 

1. Incorrect functional form: for example, using OLS works well if a model is linear but if there is a non-linear relationship between the dependent and explanatory variables then OLS will be biased and inconsistent 

2. Omitted variable bias: this occurs when important explanatory variables have been left out of the regression. When we leave an important variable out of an empirical model (either unintentionally or because we can’t measure it) then OLS estimates may be biased and inconsistent. 

3. Irrelevant variables: a less serious form of model misspecification occurs when irrelevant variables are included. This leads to a loss of efficiency because degrees of freedom are ‘wasted’ in unnecessarily estimating irrelevant parameters. 

What are the solutions? Hypothesis tests (such as Student’s t test) will give us information about whether or not an explanatory variable is irrelevant. The first two types of model misspecification (along with measurement error) are trickier to resolve even though they can be major sources of endogeneity, as mentioned above. 

More generally, to protect against model misspecification problems, it is important to use economic theory and previous research as a guide in constructing an appropriate functiona form and in selecting appropriate explanatory variables. For unmeasurable variables there are two main solutions: using a proxy (as discussed above) or using ‘instrumental variable (IV)’ estimation. IV estimation is beyond the scope of this book but see Wooldridge (2003) for a thorough analysis. 

We will explore a number of possible forms, including lin-log, log-log and lin-lin specifications.<sup>2</sup> In establishing which of these specifications is most appropriate, a good first step is to look at the scatter plot ofour variables around the trend line, as shown in Figures 8.3a–c. The observations seem to be more evenly dispersed around the trend line in the lin-lin specification. However, it is difficult to form a clear impression ofthe patterns because the inspection ofany visual plot of data is susceptible to some degree of subjectivity. 

To gather some more objective information about the functional form of the relationship between investment and Tobin’s $q ,$ we will estimate the following three forms of Equation (8.3): 

$$
\text { lin - log   specification }: \quad i _ {t} = \alpha_ {1} + \beta_ {1} \ln q _ {t} + \varepsilon_ {1 t}\tag{8.4}
$$

$$
\text { log - log   specification }: \quad \ln i _ {t} = \alpha_ {2} + \beta_ {2} \ln q _ {t} + \varepsilon_ {2 t}\tag{8.5}
$$

$$
\text { lin - lin   specification }: \quad i _ {t} = \alpha_ {3} + \beta_ {3} q _ {t} + \varepsilon_ {3 t}\tag{8.6}
$$

where $i _ { t } = \frac { I _ { t } } { K _ { t } }$ and $\varepsilon _ { 1 t } , \varepsilon _ { 2 t }$ and $\varepsilon _ { 3 t }$ are the stochastic error terms from (8.4), (8.5) and (8.6) respectively. From the SRFs, we will test each model for incorrect functional form using Ramsey’s RESET test, which is explained in Box 8.4. 

The EViews output tables for the estimations of the SRFs for Equations (8.4) (lin-log), (8.5) (log-log) and (8.6) (lin-lin) are summarised in Table 8.1. For the estimations of (8.4) (lin-log) and (8.5) (log-log), there are initial signs of model misspecification; the null of no AR(4) autocorrelation in the errors from the F version of the BG test is rejected at a 5% significance level. This suggests a systematic pattern in the residuals from these regressions and, as explained above, one explanation for this is some form of model misspecification error. 

We also have the RR test results from EViews. To show how this RR test was calculated, using the results from the estimation of (8.4), we follow the steps outlined in Box 8.4 as follows (on page 192): 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/c4db917c961d4e20ac45a00e50ad68df32c68e727dd282d2523c93f327c18b55.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/e71b4e33d12e64698a4d8af2567dd327e4ba24a62ba8d5a44cdfbd1caba0a024.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/5bab0dfb80e4a4433e16e153d4ce792e461001e3626658c986f7f2516935307f.jpg)



Figure 8.3 (a) lin-log specification (b) log-log specification (c) lin-lin specification


## Box 8.4 Detecting model misspecification using Ramsey’s RESET test

In Chapter 7 we explained that systematic patterns in the residuals may be a symptom of other problems one of which is model misspecification. So our diagnostic tests for autocorrelation, i.e. the Breusch–Godfrey (BG) test (explained in Chapter 7) will also pick up systematic patterns in the residuals emerging because of model misspecification. There are also tests designed specifically to identify problems of incorrect functional form and one of the most widely used functional form tests is Ramsey’s RESET (RR) test. RR tests come in many forms; for example if you are trying to estimate a logarithmic relationship using levels, then the RR test will pick this up. 

The RR test is constructed in three stages. 

1. Estimate the SRF and save the fitted values. 

2. Transform the fitted values to generate a variable which can capture omitted influences. The most common method is to use a quadratic transformation by squaring the fitted values, though it is possible also to include higher-order polynomial terms e.g. cubic transformations of the fitted values. 

3. Run an auxiliary regression of the dependent variable on the explanatory variable and the squared fitted values. 

4. Conduct hypotheses tests on the parameters for the transformed fitted values using an $F$ test of restrictions. 

For example, if our dependent variable is Y and our explanatory variable is $\chi ,$ then the auxiliary regression for the RR test would be: 

$$
\hat {Y} _ {i} = \hat {a} + \hat {\beta} X _ {i} + \hat {\phi} \left[ \hat {Y} _ {i} ^ {2} \right]\tag{8.7}
$$

The RR test is testing the following null and alternative hypotheses: 

$$
H _ {0}: \phi = 0
$$

$$
H _ {1}: \phi \neq 0
$$

The intuition underlying the Ramsey RESET test is that if the original model is complete, then including $\hat { Y } _ { j } ^ { 2 }$ in the auxiliary regression will make very little difference to the goodness of fit and the F test of restrictions will not allow the rejection of $H _ { 0 } .$ . On the other hand, if the original model suffers from the problem of incorrect functional form, then $\hat { Y } _ { j } ^ { 2 }$ will pick up something of what is missing. Including $\hat { Y } _ { j } ^ { 2 }$ will lead to a relatively large fall in the RSS relative to the RSS in the original model and the F test will allow a rejection of $H _ { 0 } .$ . We will conclude that the square of the fitted value is picking up something that has been omitted from the original model. 

Most econometrics packages, including EViews, will report variants of the RR test. We illustrate an example of the RR test below. 


<sub>p</sub>l<sub>e:</sub> <sub>19</sub>8<sup>7</sup> <sup>20</sup> <sub>mary</sub> <sub>of</sub> <sub>EV</sub>i<sub>ews</sub> <sub>output</sub> t<sup>ab</sup>l<sup>es</sup> <sup>from</sup> <sup>est</sup>i<sup>mat</sup>i<sup>ons</sup> <sup>of</sup> <sup>Equat</sup>i<sup>ons</sup> <sup>(8.4)</sup>


<table><tr><td colspan="4">LINLOG MODEL</td><td colspan="4">LOGLOG MODEL</td><td colspan="4">LINLIN MODEL</td></tr><tr><td colspan="4">Dependent Variable: Investment Rate</td><td colspan="4">Dependent Variable: Investment Rate (logged)</td><td colspan="4">Dependent Variable: Investment Rate</td></tr><tr><td>Variable</td><td>Coefficient</td><td>t-Statistic</td><td>Prob.</td><td>Variable</td><td>Coefficient</td><td>t-Statistic</td><td>Prob.</td><td>Variable</td><td>Coefficient</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>0.11</td><td>62.37</td><td>0.00</td><td>Intercept</td><td>-2.23</td><td>-141.29</td><td>0.00</td><td>Intercept</td><td>0.08</td><td>17.09</td><td>0.00</td></tr><tr><td>q (logged)</td><td>0.02</td><td>4.48</td><td>0.00</td><td>q (logged)</td><td>0.20</td><td>4.43</td><td>0.00</td><td>q</td><td>0.02</td><td>5.44</td><td>0.00</td></tr><tr><td>R-squared</td><td></td><td>0.56</td><td></td><td>R-squared</td><td></td><td>0.55</td><td></td><td>R-squared</td><td></td><td>0.65</td><td></td></tr><tr><td>Adjusted</td><td></td><td>0.53</td><td></td><td>Adjusted</td><td></td><td>0.52</td><td></td><td>Adjusted</td><td></td><td>0.63</td><td></td></tr><tr><td>R-squared</td><td></td><td></td><td></td><td>R-squared</td><td></td><td></td><td></td><td>R-squared</td><td></td><td></td><td></td></tr><tr><td>Sum squared</td><td></td><td>0.000849</td><td></td><td>Sum squared</td><td></td><td>0.0714</td><td></td><td>Sum squared</td><td></td><td>0.000672</td><td></td></tr><tr><td>residuals</td><td></td><td></td><td></td><td>residuals</td><td></td><td></td><td></td><td>residuals</td><td></td><td></td><td></td></tr><tr><td>F-statistic</td><td></td><td>20.05</td><td></td><td>F-statistic</td><td></td><td>19.66</td><td></td><td>F-statistic</td><td></td><td>29.55</td><td></td></tr><tr><td>Prob(F-statistic)</td><td></td><td>0.00</td><td></td><td>Prob(F-statistic)</td><td></td><td>0.00</td><td></td><td>Prob(F-statistic)</td><td></td><td>0.00</td><td></td></tr><tr><td colspan="4">Breusch-Godfrey LM Tests:</td><td colspan="4"></td><td colspan="4"></td></tr><tr><td>F-statistic</td><td>3.88</td><td></td><td></td><td>F-statistic</td><td>3.88</td><td></td><td></td><td>F-statistic</td><td>1.92</td><td></td><td></td></tr><tr><td>Probability</td><td>0.03</td><td></td><td></td><td>Probability</td><td>0.03</td><td></td><td></td><td>Probability</td><td>0.17</td><td></td><td></td></tr><tr><td colspan="4">Ramsey RESET Tests and Auxiliary Regressions:</td><td colspan="4"></td><td colspan="4"></td></tr><tr><td>F-statistic</td><td>8.5</td><td></td><td></td><td>F-statistic</td><td>7.9</td><td></td><td></td><td>F-statistic</td><td>1.1</td><td></td><td></td></tr><tr><td>Probability</td><td>0.01</td><td></td><td></td><td>Probability</td><td>0.01</td><td></td><td></td><td>Probability</td><td>0.30</td><td></td><td></td></tr><tr><td colspan="4">Test Equation from Auxiliary Regressions:</td><td colspan="4">Test Equation:</td><td colspan="4">Test Equation:</td></tr><tr><td>Variable</td><td>Coefficient</td><td>t-Statistic</td><td>Prob.</td><td>Variable</td><td>Coefficient</td><td>t-Statistic</td><td>Prob.</td><td>Variable</td><td>Coefficient</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>C</td><td>-0.63</td><td>-2.49</td><td>0.03</td><td>C</td><td>-36.83</td><td>-2.98</td><td>0.01</td><td>C</td><td>-0.03</td><td>-0.30</td><td>0.77</td></tr><tr><td>q (logged)</td><td>-0.27</td><td>-2.69</td><td>0.02</td><td>q (logged)</td><td>6.37</td><td>2.89</td><td>0.01</td><td>q</td><td>-0.07</td><td>-0.80</td><td>0.44</td></tr><tr><td><eq>FITTED^2</eq></td><td>63.81</td><td>2.91</td><td>0.01</td><td><eq>FITTED^2</eq></td><td>6.92</td><td>2.80</td><td>0.01</td><td><eq>FITTED^2</eq></td><td>18.59</td><td>1.07</td><td>0.30</td></tr><tr><td>R-squared</td><td></td><td>0.72</td><td></td><td>R-squared</td><td></td><td>0.71</td><td></td><td>R-squared</td><td></td><td>0.67</td><td></td></tr><tr><td>Adjusted</td><td></td><td>0.68</td><td></td><td>Adjusted</td><td></td><td>0.67</td><td></td><td>Adjusted</td><td></td><td>0.63</td><td></td></tr><tr><td>R-squared</td><td></td><td></td><td></td><td>R-squared</td><td></td><td></td><td></td><td>R-squared</td><td></td><td></td><td></td></tr><tr><td>Sum squared</td><td></td><td>0.000542</td><td></td><td>Sum squared</td><td></td><td>0.0469</td><td></td><td>Sum squared</td><td></td><td>0.000624</td><td></td></tr><tr><td>residuals</td><td></td><td></td><td></td><td>residuals</td><td></td><td></td><td></td><td>residuals</td><td></td><td></td><td></td></tr><tr><td>F-statistic</td><td></td><td>18.95</td><td></td><td>F-statistic</td><td></td><td>17.98</td><td></td><td>F-statistic</td><td></td><td>15.47</td><td></td></tr><tr><td>Prob(F-statistic)</td><td></td><td>0.00</td><td></td><td>Prob(F-statistic)</td><td></td><td>0.00</td><td></td><td>Prob(F-statistic)</td><td></td><td>0.00</td><td></td></tr></table>

1. Estimate the SRF, saving the fitted values. This is the restricted model for the purposes of the RR test so $R S S _ { \mathrm { r } } = 0 . 0 0 0 8 4 9$ 

2. Square the fitted values from step 1 to give ‘FITTED $\wedge _ { 2 } \cdot$ 

3. Run an auxiliary regression by regressing the investment rate on logged q and ‘FITTED^2’. This gives us the unrestricted model for F version of the RR test and so $R S S _ { \mathrm { u } } = 0 . 0 0 0 5 4 2$ 

4. We construct the RR version of the F test of restrictions as follows. (There is one restriction, i.e. that the parameter on $\mathrm { { } ^ { c } F I T T E D } \Lambda 2 ^ { \prime }$ is equal to zero, so $d = 1 ; n = 1 8$ and k =1.) 

$$
\begin{array}{r l} F (d, n - k _ {u} - 1 - d) & = \frac {(R S S _ {r} - R S S _ {u}) / d}{(R S S _ {u}) / (n - k _ {u} - 1 - d)} \\ & = \frac {0 . 0 0 0 8 4 9 - 0 . 0 0 0 5 4 2}{(0 . 0 0 0 5 4 2) / (1 8 - 2 - 1)} = 8. 5 0 \end{array}\tag{8.8}
$$

Following this procedure we can reject the null that the parameter on FITTED^2 is equal to zero at a 5% significance level. This is consistent with the result from a t test that the parameter on FITTED^2 is equal to zero. It is also consistent with our BG test. So we can conclude that there are significant signs of model misspecification. Similarly, you will see from Table 8.1 that there are signs of model misspecification in the estimation of (8.5) (the log-log model). 

For the estimation of (8.6) (the lin-lin model) however, the F version of the RR test gives $p = 0 . 3 0$ so $\textstyle p > 0 . 0 5$ and so we cannot reject the null that the parameter on FITTED^2 is equal to zero. In addition, the F version of the AR(4) BG test gives a p value of 0.17; $\textstyle p > 0 . 0 5$ and so, with a 5% significance level, we do not reject the null of no autocorrelation in the errors. Again this suggests that there are no significant signs of incorrect functional form in the estimation of (8.6). We can conclude that the results from the lin-lin model seem to be relatively reliable. 

The results from the estimation of the lin-lin model can be summarised as follows: 

$$
\begin{array}{r l r} \hat {i} _ {t} = & 0. 0 8 & + 0. 0 2 q _ {t} \\ & (0. 0 0 4 8) & (0. 0 0 4 4) \\ & t = 1 7. 0 9 & t = 5. 4 4 \\ & p = 0. 0 0 & p = 0. 0 0 \end{array}\tag{8.9}
$$

$$
R ^ {2} = 0. 6 5
$$

$$
F (1, 1 6) = 2 9. 5 5 [ P = 0. 0 0 ]
$$

Overall, the significant t test results on the parameter estimates for (8.6) (the lin-lin model) allow us to reject the nulls that the intercept and slope parameters are equal to zero. An initial inspection suggests that there is a significant positive relationship between investment and $q _ { \mathrm { A } } ,$ , as predicted by Tobin’s $q$ theory. For our data on US investment 1987–2004, an increase in $q _ { \mathrm { A } }$ is associated with increases in the investment rate. The $R ^ { 2 }$ suggests that 65% of the variability in the investment rate is captured by variability in q and the F test of explanatory power confirms that the overall goodness of fit of the model is relatively high and we can reject the null of no association between the dependent and explanatory variables. We have identified a significant association between q and the investment rate. 

These results seem to confirm the theory. If our findings are robust then this suggests that, if a buoyant stock market generates rises in market capitalisation that outstrip increases in the current replacement cost of the capital stock, then this will generate rises in the investment rate. It is important however to note the shortcomings of our analysis. Empirically, we have identified a positive association between investment and $q \colon$ as q rises, the investment rate (as a proportion of the capital stock) rises with it. However, as mentioned above, this finding is based on results from a very small sample. There are also problems with simple specifications of q theory. Lags are excluded even though in reality investment decisions will not be implemented instantaneously. Delays affect almost every stage of investment decision-making: there are lags between decision-making, expenditure, ordering, delivery and installation. So actual investment expenditure in the current period will reflect decisions taken some time ago. Including just current q when its lags may have more impact may have affected the reliability of our results. 

Also Tobin’s q models are based on assumptions of rational expectations and efficient financial markets. Are these assumptions valid? There is a growing literature asserting that stock market valuations will not reflect rational expectations of the future potential of current investments. This is because share prices reflect a range of other factors and will fluctuate in response to crowd psychology, herd behaviour, speculative bubbles, irrational exuberance and short-termism. With inefficient financial markets, market valuations will not be a reliable indicator of the future profitability prospects of current investments. This issue has been the focus of a lot of recent research and this research into inefficient markets is summarised in Box 8.5. 

## Box 8.5 Inefficient markets and behavioural economics

Hypotheses about efficient markets and rational agents look weak when confronted by the large number of historical examples of speculative bubbles. A speculative bubble occurs when an asset price deviates from its fundamental value. One of the most spectacular historical examples of a speculative bubble was Tulipmania, which happened during the 1630s in Holland. During this time, there was a very rare bulb that could grow into a beautiful tulip; it was called the Semper Augustus and, at the height of Tulipmania, it was selling for as much as a three-storey house in central Amsterdam. But when the bubble burst, within weeks the Semper Augustus bulb became relatively worthless. There are many more recent examples of speculative bubbles, for example the dotcom bubble of the late 1990s – the impact of which can be seen in Figure 8.2 as an upward blip in Tobin’s q ratio reflecting a jump in market valuations because of speculative trading in dotcom shares. Speculative bubbles in housing and commodity markets constituted to significant instability from 2008 onwards. 

Keynes (1936) was one of the first economists to focus on the irrational triggers of financial market movements, analysing the role of factors such as crowd psychology, herding and market conventions. More recently, economists such as Shiller and Shleifer have focussed on irrational forces in financial markets, developing the arguments of Federal Reserve governor Alan Greenspan (who coined the term irrational exuberance in response to the dotcom bubble of the late 1990s). Also, building upon the work of the George Katona, recent Nobel Prize winner Daniel Kahneman (a psychologist) and Kahneman’s colleague Amos Tversky (who was an economist), behavioural economists and economic psychologists are putting to one side assumptions about rational expectations and efficient markets to concentrate on the psychology of economic and financial decision-making. 

One of the more novel aspects of this literature is the research into the relationship between psychological factors and financial activity. This draws upon Jevons’ sunspot theory, a nineteenth-century model of the economy focussing on the impact of cosmic rays and sunspots on the weather. Jevons argued that the consequent impacts of weather on agricultural production would spread to the macroeconomy more generally. Whilst these ideas were ridiculed at the time, the focus on weather is now being revived in a number of ways. In financial derivatives markets new instruments are being devised to hedge against weather risks using weather derivatives: for example natural catastrophe bonds (cat bonds) are instruments designed to protect agricultural firms from natural catastrophes such as hurricanes (The Economist, 2005). 

In explaining the wider psychological impacts of the weather on financial markets, Hirschleifer and Shumway (2003) have analysed the relationships between mood, sunlight and financial trading activity and Kamstra, Kramer and Levi (2003) have identified a positive relationship between seasonal depression (a.k.a. Seasonal Affective Disorder – SAD) and subdued stock market activity. 

Ideas about inefficient financial markets are also taken further in a new sub-discipline of economics called neuroeconomics. Neuroeconomists work with experimental psychologists, neurophysiologists and neuroanatomists using various experimental techniques to capture how and why the brain is involved in financial decision-making, particularly risktaking and impulsive behaviour. A range of neuroeconomic techniques is outlined in Camerer, Loewenstein and Prelec (2005). Some examples of neuroeconomic techniques include functional magnetic resonance imaging (fMRI) – which involves taking detailed ‘pictures’ of the brain to assess oxygen flows to particular areas; single neuron experiments to monitor the neurotransmitters that operate at the synapses of neurons (e.g. dopamine); monitoring of levels of hormones such as testosterone and cortisol using saliva and blood tests; studying the behaviour of patients with lesions located in particular areas of their brains to assess whether or not such impairments affect economic behaviour; as well as psychometric testing to control for the role of various personality traits in economic decisionmaking etc. 

Neuroeconomists investigate financial market behaviour by assessing how financial traders’ brains respond when traders are making risky decisions. Ultimately, if they can show that people do not necessarily use objective information in a systematic way then rational expectations and efficient markets will no longer be at the core of theoretical analyses of financial markets. On the other hand, if the behavioural economists and neuroeconomists can show that economic and financial decision-making is associated with logical, rational cognitive responses, then we could conclude that the emphasis on rationality and market efficiency in models such as Tobin’s q theory may be justifiable, at least as an approximation. 

## Implications and conclusions

In this chapter, we have analysed the impact of stock market activity on fixed asset investment by estimating Tobin’s q model of investment in the USA 1987–2004. In terms of policy, the positive association between Tobin’s q and investment suggests that stock market volatility will have implications for investment and capital accumulation more generally. Therefore, measures to stabilise stock markets, e.g. taxes on speculative trades (known as Tobin taxes reflecting Tobin’s other research), may generate wider benefits in terms of stabilising productive activity overall. Taxes on financial transactions might moderate some ofthe sources ofmacroeoconomic instability but there may be political constraints on implementing new taxes and regulations. Such policy changes are unlikely to be popular, particularly within the financial services sector, though instability in global financial markets has increased pressure to implement regulatory reforms. 

Overall, Tobin’s q provides a neat theoretical solution to the problem of measuring investors’ expectations of the future potential of their current investment decisions. And q models capture the investment process more effectively than Jorgenson’s early theory because they incorporate expectations, forward-looking behaviour and adjustment costs. However, if agents do not form rational expectations and/or if financial markets are not efficient, then the theoretical underpinnings of q models of investment will have to be rethought. 

## 8.6

## Further reading

## Textbooks



Baddeley, M. C. (2003) Investment: Theories and Analysis, London: Palgrave Macmillan. 





Keynes, J. M. (1936) The General Theory of Employment, Interest and Money, London: Macmillan. 





NYSE (2006) A Guide to the NYSE Market Place, New York: New York Stock Exchange. 





Shiller, R. (2001) Irrational Exuberance, Princeton: Princeton University Press. 





Shleifer, A. (2000) Inefficient Markets: An Introduction to Behavioral Finance, Oxford: Oxford University Press. 





Smithers, A. S. and Wright, S. (2000) Valuing Wall Street, New York: McGraw Hill. 





Wooldridge, J. M. (2003) Introductory Econometrics – A Modern Approach (2nd edition), Thomson South-Western. See Chapter 9 on model misspecification and measurement error; see Chapter 15 for corrective procedures including instrumental variable (IV) estimation. 



## Academic articles and working papers



Camerer, C. F., Loewenstein, G. and Prelec, D. (2005) ‘Neuroeconomics: how neuroscience can inform economics’, Journal ofEconomic Literature, vol. 43 no. 1, 9–64. 





Hayashi, F. (1982) ‘Tobin’s marginal q and average q: a neoclassical interpretation’, Econometrica, vol. 50, no. 1, 213–24. 





Hirschleifer, D. and Shumway, T. (2003) ‘Good day sunshine: stock returns and the weather’, Journal ofFinance, vol. LVIII, no. 3, 1009–32. 





Jorgenson, D. W. (1963) ‘Capital theory and investment behaviour’, American Economic Review, vol. 53, no. 2, 247–59. 





Kamstra, M. J., Kramer, L. A. and Levi, M. D. (2003) ‘Winter blues: a SAD stock market cycle’, American Economic Review, vol. 93, no. 1, 324–43. 





Muth, J. F. (1961) ‘Rational expectations and the theory of price movements’, Econometrica, vol. 29, no. 3, 315–55. 



## Policy briefs and newspaper articles

Bond, S., Klemm, A., Newton-Smith, R., Syed, M. and Vlieghe, G. (2004) ‘The roles of profitability, Tobin’s Q and cash flow in econometric models of company investment’, Bank of England Working Paper No. 222, London: Bank of England. 

The Economist (2005) ‘Weather risk: natural hedge’, 1 October 2005, p. 84. 

## 8.7 Chapter exercises

1. In this chapter we noted that the estimation of Tobin’s q models might have suffered econometrically from the exclusion of lags. Re-estimate the models from this chapter using the data sources outlined in Section 8.3 and check for signs of model misspecification. Discuss your results. 

2. As explained in Section 8.3, accelerator theories of investment use past output growth as a proxy for expectations of future sales. Using the data sources outlined in Section 8.3: 

(a) Construct an empirical model of accelerator theory using output growth as an explanatory variable. 

(b) Assess your results including the diagnostic test results. 

(c) Discuss the relative empirical performance of your model and the q models from this chapter. 

# Time-series econometrics

In the previous parts, we have applied econometric techniques to both crosssectional data and time-series data. Cross-sectional data has a spatial dimension and can be collected at different levels of disaggregation. It gives a ‘snapshot view from one point in time and will include observations for a number of different individuals, households, firms, regions or countries. 

Conversely, time-series analysis focusses on one spatial ‘entity’ (e.g. a firm, a country or the world) and investigates how the behaviour of that entity changes over time. Time-series observations can be of any ‘periodicity’. The most commonly used are annual, quarterly, monthly or daily. In financial markets intra-day ‘high-frequency’ data is also collected, e.g. to record how asset prices change even from one second to the next. 

Apart from the usual econometric problems discussed in Part II, the analysis of time-series data can be complicated by lags and structural breaks. There may also be time trends – both ‘deterministic’ (predictable) and ‘stochastic (random). These trends will generate the problem of ‘non-stationarity’. 

In this part, we will investigate some of these complications. We will also introduce some econometric procedures designed specifically for the analysis of time-series data. 

# Structural breaks, non-stationarity and spurious regressions Venture capital and computing investment in the USA

Economic issues include: 

 The New Economy 

 Investment in computing 

 Venture capital funding 

Econometric issues include: 

 Structural breaks 

 Unit roots, non-stationarity and spurious regressions 

Data issues include: 

 Measuring the New Economy 

## 9.1 The issue

In this chapter we will look at the relationship between computing investment and venture capital financing in the New Economy. Computing investment has been essential to the growth of the New Economy: Yang and Brynjolfsson (2001) argue that computerisation is the most pervasive technological change this era. IT (information technology) investments promoted improved macroeconomic performance, culminating from large increases in productivity and growth in the 1990s onwards, particularly in the US. Increasing GDP growth was accompanied by reduced volatility in GDP. This is because IT innovations played a key role in promoting greater flexibility; for example, innovations such as price comparison sites (e.g. dealtime.com and 

## transparency.

The New Economy grew rapidly from the 1990s onwards and its growth was enabled by venture capital injections. Venture capital is of particular importance because young entrepreneurs are responsible for a substantial proportion of the innovative New Economy investments. These entrepreneurs do not have profits retained from existing production. So venture capital funds are important in providing them finance for their new investments. 

In this chapter we will explore the relationship between New Economy investment and venture capital funding. We will focus in particular on IT in the New Economy by examining the relationships between venture capital funds and investment in computing software in the US 1980–2004. We will also use this data set to illustrate the econometric implications of structural breaks, non-stationary variables and spurious regressions. 

## 9.2 The theory

These days it seems that everyone’s talking about the New Economy. But what is it? There is no universally accepted definition of the New Economy but the term is generally used to refer to the development of new high-tech knowledge-based industries, particularly those associated with IT. The New Economy also includes industries associated with biotechnology (biotech) but the IT sector has been particularly influential. 

The growth of the New Economy and particularly the development of the Internet, have made physical location and resources less important. This is because one of the key characteristics of the technological changes in IT are that they are knowledge-driven and therefore aspatial. They are knowledgedriven because brain-power, research and innovation play a more important role than they do in traditional industries, for which physical location and local resources (e.g. plentiful labour) are important. Knowledge-driven technologies and industries are also aspatial because they do not rely on physical assets fixed in particular locations. This means that knowledge-driven industries can transcend national/regional boundaries more easily. For example, computing innovations such as email and the Internet mean that geographical divisions are not as important as they once were. Developments in the New Economy have progressed in tandem with the process of globalisation; for example, different people in different parts ofthe world can communicate and trade almost instantaneously because of IT innovations particularly those based on Internet and mobile technologies. So these technologies have had enormous implications for global economic activity and trade. 

What is the history of the IT Revolution? Widespread computerisation of economic activity began in 1971 when Intel marketed its first microprocessor chip, allowing the development of powerful personal computers (PCs). During the 1970s, news of these innovations spread and new ITrelated products and services evolved, starting with basic computerisation of business activities (e.g. word-processing, spreadsheet and accounting packages). Computerisation eventually affected almost every aspect of modern economic life with the development of innovations associated with computer networking and the Internet, mobile phone technologies and computer-based financial innovations (for example Electronic Funds Transfer at Point of Sale (EFTPOS), and Automated Clearing House (ACH) systems). 

This diffusion of computer technologies is described via Moore’s Law: the power ofmicroprocessors doubles every 18 months. Moore’s Law operates because technological developments have allowed an increasing number of transistors to be built into each individual microprocessor increasing their power: the transistor count in the average microprocessor rose from just above 1,000 transistors in 1971 to close on 100 million transistors in 2001. This exponential growth in electronic transistors translated into a rapid growth of computing power, in turn fostering rapid falls in the cost of computing equipment. These falls in computing costs allowed technological changes from the IT sector to spread rapidly through the economy, particularly for innovations that overlap industries. For example, recent innovators in the high-tech sector have been developing mobile wallets, which allow people to store and use money via their mobile phones. Mobile wallets link together IT technologies from the computing and telecommunications industry and from the financial sector. 

Computing innovations have had significant impacts on the broader economy. The US Department of Commerce estimates that high-tech industry accounted for more than one third of GDP growth between 1995 and 1999. Gordon (2000) and Whelan (2002) also provide evidence about the impacts of the IT Revolution on increasing trend growth rates in real GDP and productivity. In addition, Landefeld and Fraumeni (2000) estimate that, between 1995 and 1999, the contribution of high-tech products to real GDP growth was 24%; they also observe that difficulties measuring the impacts ofhigh-tech investments mean that this is likely to be an under estimate. 

IT developments have affected productivity, real wages and unemployment too. Plants using computer-aided manufacturing paid workers two-thirds more than traditional plants in the same industry (Dunne, 1991). Output growth in the computing industries has been associated with declines in UK unemployment (Baddeley, 2008). The IT Revolution promoted increasing international trade in computers, semi-conductors and other high-tech goods and household wealth increased in parallel: US household wealth doubled in the 1990s, reflecting increases in share prices – particularly in the IT sector – in turn fostering income growth and growing consumer confidence (Landefeld & Fraumeni, 2000). 

However, not all commentators agree about the revolutionary impact ofthe IT Revolution. Many assert that the IT Revolution is not a unique event, and it is neither a new phenomenon nor qualitatively different from other technological revolutions, e.g. those that accompanied the Industrial Revolution. Some of the pessimism about the IT Revolution emerged because computerisation’s contribution to productivity and economic growth was not immediately obvious. This was the essence of Solow’s Computer Paradox (SCP): many people had expected computerisation to boost labour and capital productivity a lot more quickly – but between the 1970s and the 1990s, productivity actually slowed despite widespread computerisation. Solow (1987) famously observed that computerisation can be seen everywhere, except in the productivity statistics. But productivity gains did eventually emerge, suggesting that the SCP may have reflected lags in investment decision-making, slow diffusion of innovations, substantial adjustment costs involved in adopting innovative technologies and/or problems of measurement. Specifically, measurement problems will occur because computerisation involves intangible investments (e.g. in computing skills, R&D etc.) and focusses on the provision of services rather than the production of goods; conventional productivity statistics do not effectively capture these factors. 

Even so, these benefits did not last forever. Following the NASDAQ crash in mid 2001 surplus computers stockpiled because access to cheap finance had encouraged an unsustainable over-investment in computing resources (Cecchetti, 2002). But IT innovations may have made economies naturally more resilient and flexible, for example new innovations in inventory control allowed firms to respond relatively quickly to changes in economic conditions; for example, Cecchetti (2002) observes that the 2000–2001 slowdown in the US was remarkably subdued and short-lived because computerisation had increased macroeconomic flexibility. Economies were also far more resilient in the aftermath of the September 2001 terrorist attacks than was initially predicted. US Bureau of Economic Analysis (BEA) data show that although US annual real GDP growth slowed to 1.7% in the last quarter of 2001, in the first quarter of 2002, it recovered to 5.6%. Hopeful commentators might also predict that the flexibility engendered by computerisation of economic activity may also moderate the recessionary impacts of the 2007/8 credit crunch. 

What are the limits to growth in the New Economy? Have economies had their New Economy ‘burst’ or can we expect technological progress to continue at its current pace? Will new technologies continue to develop and spread? According to some observers, the rise and fall of the dot coms and the accompanying boom–bust investment cycle suggests that perhaps the processes of invention and innovation will falter until the next technological revolution. Furthermore, some economists believe that technological developments are a key factor in explaining the ups and downs of business cycles. Schumpeter (1939) analysed technological booms associated with the telephone, railways and electrification and his ideas can be extended to investment in the New Economy. Schumpeter argued that innovative industries emerge from a process of ‘creative destruction’ with oligopolistic firms competing technologically (rather than via price competition) and creating cyclical instability as a consequence. The clumping of innovations leads to ‘bursts’ of entrepreneurship; bandwagon effects encourage herds of entrepreneurs to copy innovative entrepreneurs in exploiting new innovations. But as more and more entrepreneurs try to exploit the diffusion of technological innovations, profits will be eroded. Financing new innovations will become more and more difficult, contributing to an ebbing of confidence in innovative industries. So downswings are the inevitable consequence of the innovative phases that generate the upswing. 

A key factor affecting technological cycles is the availability of finance. The process of investing in new types of plant, machinery and equipment ensures that technological innovation diffuses through the economy allowing people and businesses to learn about new innovations. But, even if an entrepreneur has a brilliant idea, the success or failure of his/her business venture will still depend upon whether or not funds are available to finance the costs of establishing a new business. All fixed investments, whether innovative or not, depend on finance so innovative activity will slow as financing constraints emerge. 

In innovative phases, specific types of funding may be necessary. One way to fund investment is via retained profits from existing production but the established firms that are likely to have these retained profits may initially be resistant to technological change. The technological leaders are more likely to be young entrepreneurs with great new ideas but no existing business to provide them with retained profits for new investments. Famous examples of businesses started by young entrepreneurs include Mark Zuckerberg (who founded Facebook) and Larry Page and Sergey Brin (who founded Google) – all were under 26 years old when they founded their businesses. Without a fund of retained profits young entrepreneurs often have to rely on specific types of financial backing including venture capital funds or angel investors. 

Venture capital funds represent a pool of funds managed for a group of financial investors. Angel investors are individuals providing finance from their own resources. Venture capitalists and angel investors will provide financial backing for new businesses and, in return, will either charge interest or retain equity in the entrepreneur’s firm (i.e. they will own some proportion of the firm’s assets). The interest rate charged on lending will usually be relatively high – reflecting the fact that the lending is very risky. On the other hand, the maximum returns may also be very high: angel investors and venture capitalists often have a large number of firms on their books but the success ofjust one ofthose firms may deliver a profit large enough to cover the failure of a number of the other firms that they’re backing. 

In this chapter we will explore the links between computing investment and venture capital funding. We choose computing investment because computerisation is an essential aspect of the growth of the New Economy. We focus on venture capital funds because innovative entrepreneurs do not usually have their own sources offunds to finance investment projects and the success or failure of innovations will therefore depend upon whether or not venture capitalists are prepared to fund innovative production. In our empirical analysis, we will not specifically address the impact of angel investment because data on angel investors are scare and venture capital funds play a more significant role. 

So the theoretical model that we will estimate in this chapter is: 

$$
c i _ {t} = \alpha + \beta v c _ {t} + \gamma T i m e _ {t} + \varepsilon_ {t}\tag{9.1}
$$

where $c i _ { t }$ is the natural log of computing investment; $\nu c _ { t }$ is the natural log of venture capital funds and Time is a deterministic trend. Deterministic trend variables are included to capture stable proportionate increases in a variable over time, e.g. reflecting factors such as technological progress and GDP growth. 

For the parameters, α is the intercept parameter, $\beta$ is the elasticity of computing investment with respect to venture capital funding, γ is the parameter on the deterministic trend and $\varepsilon _ { t }$ is the error term. Our variables are logged because we are interested in the elasticity of computing investment with respect to venture capital funding. 

## 9.3 The data


In this analysis, we are examining the links between computing investment and venture capital funding. How do we measure this relationship between computing investment and venture capital financing? Our data sources are:


<table><tr><td>Variable</td><td>Source</td><td>Website</td></tr><tr><td>Computing Investment (software)</td><td>Bureau of Economic Analysis (BEA), US National Income and Product Accounts (NIPA)</td><td>www.bea.gov/national/nipaweb/</td></tr><tr><td>Venture capital disbursements (software)</td><td>National Science Foundation (NSF), Science and Engineering Indicators 2006</td><td>www.nsf.gov/statistics</td></tr></table>

The BEA data is expressed in real terms – as a quantity index. We transform the venture capital data into real terms by deflating venture capital disbursements using the US GDP deflator from the IMF’s World Economic Outlook Database (www.imf.org/external/pubs/ft/weo/2008/01/weodata). 

Figure 9.1 plots computing investment and venture capital disbursements over the period 1980 to 2004. This figure captures the changing patterns in computing investment and venture capital disbursements. Until about 1994, there was no clear association between computing investment and venture capital: growth in venture capital was relatively stagnant until about 1995 suggesting that computing investment was propelled by other factors during this early period. From 1995 onwards a positive association between computing investment and venture capital emerged alongside considerable volatility in venture capital disbursements. Venture capital disbursements shot up during the 1999–2001 dotcom bubble but collapsed again with the dotcom crash in 2001. This instability did not strongly impact on computing investment, perhaps because the long lags on investment decisions enabled a smoothing of the path of computing investment. 

There are two key features to the patterns depicted in Figure 9.1: firstly, the relationship between computing investment and venture capital does not have a stable form; and secondly, both series of data are exhibiting some instability over time: they do not have a stable mean and variance. These features will complicate our econometric analysis and will be explored further in Section 9.4. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/5019d51240c3ddc1b550c95297eebd6f29b4e8e4546f44d4842fb0c18809fa67.jpg)



Figure 9.1 Computing investment vs. venture capital disbursements, USA 1980–2004


Before beginning an econometric analysis, it is important to examine some of the limitations of the data set. The growth of high-tech industry is a relatively recent development and for many countries the range of detailed data on hign-tech production and investment is limited, although more efforts have been made recently to collect and standardise data particularly in the USA. The BEA computing investment data are provided in real terms (as a quantity index). Whilst quantity measures do, in theory at least, abstract from price effects, they will not capture the substantial improvements in computing quality that have occurred over time (e.g. via the operation of Moore’s Law). Ideally, hedonic price measures are needed effectively to capture these quality improvements but hedonic price measures for IT are not yet widely available.<sup>1</sup> 

We have focussed specifically on computing investments in software because the BEA data on computing investments in other categories is not disaggregated in the same way as the NSF data on venture capital disbursements into computing. This may introduce a selection bias into our analysis and our results from an analysis of software investment may not be representative of all computing investment. 

Also, we have only 25 observations and so our analysis might suffer from the consequences ofmicronumerosity (i.e. a small sample size), particularly as micronumerosity will reduce the accuracy of our estimation and compromise the power of our hypothesis tests. 

Finally, as mentioned above, we may have reason to be concerned about the stability of our data series; for example, the large fluctuations in venture capital disbursements may have implications for the reliability of our results. In assessing this issue, in this chapter we emphasise the impacts of structural breaks and non-stationarity on the stability ofour data and these problems are defined and assessed in more detail in Section 9.4. 

## 9.4 Empirical methods and results

When we run a regression on Equation (9.1), we get the following estimated equation for computing investment (standard errors are in brackets): 

$$
\begin{array}{l l l l l} c i _ {t} = & 2. 1 2 & + 0. 0 7 4 v c _ {t} & + 0. 1 3 3 T i m e & + \hat {\varepsilon} _ {t} \\ & (0. 1 0 7) & (0. 0 4 0 1) & (0. 0 0 7 7 9) \\ & t = 1 9. 9 & t = 1. 8 2 & t = 1 7. 0 \\ & p = 0. 0 0 0 & p = 0. 0 8 2 & p = 0. 0 0 0 \\ & \bar {R} ^ {2} = 0. 9 8 6 & \mathrm{DW} = 0. 2 5 6 \end{array}\tag{9.2}
$$

On first inspection at least, our results look good: our adjusted $R ^ { 2 }$ is high suggesting that about 98% of the variability in computing investment is captured by variability in venture capital disbursements. If we test the $H _ { 0 } { \mathrm { : } }$ $\beta = 0$ , we find that $\beta ,$ the coefficient capturing the elasticity of computing investment spending with respect to venture capital disbursements, is significantly different from 0 at a 10% significance level though not at a 5% significance level. 

But there are signs of a problem as can be seen from an inspection of the actual versus fitted values for computing investment – plotted in Figure 9.2. 

The vertical distances between the actual and fitted values are the residuals and these are are exhibiting wave-like patterns. In the early period there is a run of negative residuals but from 1990 until about 2001 there is a long run of mostly positive residuals. As explained in Chapter 7, wave-like patterns are a sign of positive autocorrelation and the presence of this problem is confirmed by the DW statistic $\hat { d } = 0 . 2 5 6 < d _ { L } ( n = 2 5 , k = 2 ) =$ $\bar { 1 } . 2 1 . ^ { 2 }$ It is important to remember that the DW statistic is not the most powerful autocorrelation test but it is routinely reported in many econometrics packages and does provide a quick ‘at a glance’ indicator of potential problems before more rigorous investigations proceed. Also, as explained in Chapter 7, finding autocorrelation may indicate that an econometric model suffers from more serious problems such as, for example, structural breaks and non-stationary variables, as explained below. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/d840e8f14ca32eef87e9ab646881435d931a9cb27dfa2e91e0c84bef583c14f9.jpg)



Figure 9.2 Actual vs. fitted computing investment, 1980–2004


## Structural breaks

One of the explanations for this residual correlation may be that there is a structural break in the relationship between computing investment and venture capital disbursements. Structural breaks can be captured using a Chow test for a structural break and the methodology underlying this test is explained in Box 9.1. 

## Box 9.1 Structural breaks, parameter instability and Chow tests

One of the assumptions made when running a regression is that parameters are stable over the entire period sampled. This may not be a valid assumption because structural breaks are common in a lot of econometric analysis. 

To illustrate: Figure 9.3 below shows two sets of observations over time – the dotted lines depict the lines of best fit just for the sub-sets of observations. Clearly, the slope and intercept for these two sub-samples of data are different. The solid line depicts what would happen if you tried to treat these two sub-sets of observations as identical, i.e. if you were to assume that the slope and intercept parameters were the same for both sub-sets. In this case, vertical distances between the dots and crosses and straight line would be relatively large and this would be picked up in a relatively high residual sum of squares (RSS). 

If there have been structural shifts in the parameters of the model then we can test for these using Chow’s structural break test. Whilst we show how to do this ‘by hand’, most statistical packages, including EViews, are programmed to calculate Chow tests. 

## Calculating the Chow structural break test

Constructing the Chow test involves running a series of regressions to capture shifts across two (or more) subperiods of data to allow a comparison of the unrestricted RSS (when you allow the parameters to shift across your sample) with the restricted RSS (when you force the parameters to be the same across your sample). When you impose a restriction upon a model, the RSS will necessarily increase and this can be measured using an adaptation of the F test of restrictions explained in Chapter 5. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/e890d87d32a1c1d54afd7a41a209ed7ff4ad79aba50463f98e701f664b3d04ee.jpg)



Figure 9.3 Parameter shifts across a sample


To illustrate, if we are regressing y on x: 

$$
y _ {t} = a + \theta x _ {t} + \varepsilon_ {t}\tag{9.3}
$$

We will be testing the following hypotheses: 

$$
H _ {0}: a _ {1} = a _ {2}; \theta_ {1} = \theta_ {2}
$$

$$
H _ {0}: a _ {1} \neq a _ {2}; \theta_ {1} \neq \theta_ {2}\tag{9.4}
$$

where subscript 1 denotes Period 1 and subscript 2 denotes Period 2. 

We estimate the restricted model over the whole sample of data – thereby forcing the parameters to be the same throughout. This restricted regression gives the RSS . There are as many restrictions as there are parameters in the theoretical model, i.e. two in this case (one intercept parameter and one slope parameter). 

The next step is to see what happens to the RSS if we allow the parameters to change – by estimating two separate regressions for the sub-samples of data and calculating the unrestricted RSS as the sum of the RSSs from the sub-sample regressions, i.e. $\begin{array} { r } { R S S _ { \mathrm { u } } { = } R S S _ { \mathrm { 1 } } + R S S _ { \mathrm { 2 } } . } \end{array}$ . The RSS and $R S S _ { \mathrm { u } }$ are then incorporated into the following formula: 

$$
F (k, n _ {1} + n _ {2} - 2 k - 2) = \frac {(R S S _ {\mathrm{r}} - R S S _ {\mathrm{u}}) / k}{R S S _ {\mathrm{u}} / (n _ {1} + n _ {2} - 2 k - 2)}\tag{9.5}
$$

The degrees of freedom in the numerator are the number of restrictions imposed in the restricted model: in this case it will be k+1 – the number of parameters in our model. For model (9.3) we estimate one intercept and one slope parameter. 

The degrees of freedom in the denominator capture the degrees of freedom in the unrestricted model. In this case $\mathsf { w e v e }$ had to estimate Equation (9.3) twice – once for the early period and once for the later period. There are $( \boldsymbol { { \eta } } _ { 1 } + \boldsymbol { { \eta } } _ { 2 } )$ observations but 2(k+1) degrees of freedom will be lost because each set of parameters is estimated twice and this leaves $\begin{array} { r } { \eta _ { 1 } + \eta _ { 2 } - 2 k - 2 } \end{array}$ degrees of freedom in the denominator. 

If the Fvalue from the Chow test is relatively large (i.e. if $F { > } F _ { \mathrm { c r i t } } )$ then this suggests that the RSS increases significantly when we force the parameters to be the same over the entire period; the goodness of fit has declined. This would suggest that the assumption of parameter stability is not a valid assumption and so $H _ { 0 }$ would be rejected. On the other hand, if $F { < } F _ { \mathrm { c r i t } } ,$ then imposing the restriction of parameter stability has not made much difference to the goodness of fit and has not increased the RSS significantly. This would suggest that the restriction of parameter stability, i.e. that the parameters are the same across both sub-samples, is mirrored in the data and it would be valid to retain $H _ { 0 }$ 

If a break is identified, how can it be modelled? Dummy variables may be useful. As explained in Chapter 5, dummy variables can be used to capture effects that can only be categorised and cannot be measured in the ordinary way. In Chapter 5, we discussed their use in the context of seasonal effects but dummies can also be used to capture the impacts of other non-measurable forms of change, for example structural breaks. Using dummies to capture breaks in Equation (9.4), if we want to control for simple shifts in the intercept, then we can introduce an additive dummy variable taking the value 1 after the break and the value zero before it. This will shift the intercept for periods after the break by an amount captured by the estimated parameter γ on the dummy variable $D _ { * }$ 

$$
y _ {t} = (a + \gamma D) + \theta \cdot x _ {t} + \varepsilon_ {t}\tag{9.6}
$$

Note that before the break $D = 0$ and so the additive dummy disappears from the equation, and we are left with our original specification. 

Shifts in slope can be captured using a multiplicative dummy; in this case constructed by multiplying D by the explanatory variable x to give: 

$$
u _ {t} = (a + \gamma D) + (\theta + \varphi D) \cdot x _ {t} + \varepsilon_ {t}\tag{9.7}
$$

where φ captures the shift in slope when $D = 1$ 

Constructing models that include these additive and multiplicative dummy variables can also give us an alternative to the conventional Chow test for a structural break if we conduct an Ftest of restrictions to test $H _ { 0 } ; \gamma = \varphi = 0$ The restricted model would exclude the dummies, the unrestricted model would include them. If the F test of restrictions indicates that RSS is not significantly greater than $R S S _ { \mathrm { u } } ,$ then we would conclude that parameters on the additive and multiplicative dummies are jointly equal to zero. We would not reject our $H _ { 0 }$ above and this would be exactly equivalent to not rejecting the $H _ { 0 } ; a _ { 1 } = a _ { 2 } ; \theta _ { 1 } = \theta _ { 2 }$ from Equation (9.3). 

One problem for structural break tests is in identifying the timing of breaks. Relatively sophisticated methods exist to ‘endogenously’ identify the timing of a break by testing all possibilities for the start of the break. At a more elementary level, a good understanding of the underlying economic/political trends will help to inform hypotheses about the timing of breaks. Also, structural break tests can be designed to capture more than one break and this issue is explored in the chapter exercises. 

Using the methodology outlined in Box 9.1, we can perform a structural break test on our model as follows: 

Step 1: Estimate the model over the entire period 1980–2004 to get $R S S _ { \mathrm { r } } .$ . For this estimation the parameters are restricted to be the same over the entire period. For this dataset, EViews gives $R S S _ { \mathrm { r } } = 0 . 3 6 1 8 .$ 

Step 2: Estimate the model separately over two sub-periods (1980– 1994 and 1995–2004) to give $R S S _ { \mathrm { u } } { = } R S S _ { 1 } { + } R S S _ { 2 }$ . For this data set, EViews gives: $\mathrm { R S S _ { u } } \mathrm { = } R S S _ { 1 } \mathrm { + } R S S _ { 2 } \mathrm { = } 0 . 0 2 7 9 \mathrm { + } 0 . 0 2 2 5 \mathrm { = } 0 . 0 5 0 4$ 

Step 3: For the degrees of freedom, we are imposing three restrictions (i.e. that the intercept, the slope on the venture capital variable and the slope on the time trend are the same in the second period as in the first period) so we have three degrees offreedom in our numerator. In our unrestricted model we have used observations for the whole period of data $( n _ { 1 } + n _ { 2 } = 1 5 + 1 0 = 2 5 )$ and we have estimated two sets of parameters – one set for the first period and another set for the second period so $2 ( \mathrm { k } { + } 1 ) = 6$ and the remaining degrees of freedom in the denominator is 19. 

Step 4: Incorporating these numbers into our formula for the F test of restrictions gives: 

$$
\begin{array}{r l} F (k, n _ {1} + n _ {2} - 2 k - 2) & = \frac {(R S S _ {\mathrm{r}} - R S S _ {\mathrm{u}}) / k + 1}{R S S _ {\mathrm{u}} / (n _ {1} + n _ {2} - 2 k - 2)} \\ & = \frac {(0 . 3 6 1 8 - 0 . 0 5 0 4) / 3}{0 . 0 5 0 4 / 1 9} = 3 9. 1 3 \end{array}
$$

EViews will calculate this test automatically and you can verify this result using EViews as follows: in the Equation output box, pull down Stability Tests from the View menu, pull across to Chow Breakpoint test, then input 1995. Click on OK and you have your Chow test result of $F = 3 9 . 1 3 \ [ p = 0 . 0 0 0 ]$ 

Given this result, we reject the null that the parameters are stable throughout the period: even at very low significance levels there is evidence of a significant shift in the parameters of our model. This is unsurprising given the patterns from Figure 9.1: these show that there is a far stronger correlation in venture capital disbursements after 1995 than before 1995. 

## Non-stationarity

As noted above, our initial regression indicated that there are systematic patterns in our residuals i.e. there is residual autocorrelation in our model. Above we have explored the possibility that this residual autocorrelation reflects a structural break in the relationship between computing investment and venture capital. Another possibility is that our variables have unstable properties: it is possible that we have non-stationary variables and a symptom of non-stationarity is autocorrelation in the residuals. Non-stationarity in variables will also mean that the variances of our variables will be unbounded, compromising OLS estimation. Non-stationarity may also generate a spurious regression, i.e. a regression with a misleadingly high degree of explanatory power. For example, iftwo variables, by coincidence, are exhibiting common upward trends, then the covariance between them will be high and $\hat { \beta } _ { O L S }$ – the OLS estimate of the slope parameter – will be inflated accordingly. A detailed explanation of non-stationarity is provided in Box 9.2. 

## Box 9.2 Unit roots and non-stationarity

For our regressions to be estimated accurately and reliably the variables used must be well behaved, i.e. the variables must be stable over time with constant means, variances and autocovariances (the autocovariance is the covariance of a variable between itself and its own lagged values). Usually, OLS estimation procedures will only work properly if all the variables (dependent and explanatory) are stationary. 

A non-stationary variable is a variable with a changing mean, variance or autocovariance. Non-stationarity is caused by trends in variables and there are two broad types of trends: deterministic trends and stochastic trends. A deterministic trend is a systematic, stable upward movement in a variable and can be captured using a deterministic time trend variable. 

A stochastic trend emerges as a consequence of randomness in variables. Stochastic trends can be illustrated using some simple stochastic processes: the unit root processes. There are various types of unit root processes but two common forms are random walks and random walks with drift. If we are looking at the relationship between a variable y<sub>t</sub> and its own lagged value $y _ { t - 1 } .$ 

$$
y _ {t} = \rho y _ {t - 1} + \varepsilon_ {t}\tag{9.8}
$$

ywill have a unit root if $\rho = 1$ , i.e. if the parameter on the lag is exactly equal to one. In other words, if we have a unit root process then: 

$$
y _ {t} = y _ {t - 1} + \varepsilon_ {t}\tag{9.9}
$$

For this simple form of unit root process subtracting $y _ { t - 1 }$ from both sides gives: 

$$
\Delta y _ {t} = \varepsilon_ {t}\tag{9.10}
$$

Thus, when $\rho = 1 \ \Delta y _ { \mathrm { t } }$ follows a completely random pattern, i.e. its movements will be determined by $\varepsilon _ { t } { : } y$ will be changing or ‘walking’ in a random way. For this reason this form of non-stationarity is called a random walk. This is a simple example of a stochastic trend because the trends in y are generated by the stochastic, random element, i.e. $\boldsymbol { \varepsilon } _ { t }$ 

A more complex unit root process is the random walk with drift where a ‘drift’ or intercept term α is affecting the random walk process: 

$$
y _ {t} = a + y _ {t - 1} + \varepsilon_ {t}\tag{9.11}
$$

To illustrate how non-stationarity emerges with the random walk with drift, assume that we start in period 1 with $y = y _ { 0 }$ . If y is a random walk with drift then it will evolve in the following way: 

$$
y _ {1} = a + y _ {0} + \varepsilon_ {1}\tag{9.12}
$$

$$
y _ {2} = a + y _ {1} + \varepsilon_ {2} = a + (a + y _ {0} + \varepsilon_ {1}) + \varepsilon_ {2} = 2 a + y _ {0} + \varepsilon_ {1} + \varepsilon_ {2}\tag{9.13}
$$

So it follows that: 

$$
y _ {3} = a + y _ {2} + \varepsilon_ {3} = 3 a + y _ {0} + \varepsilon_ {1} + \varepsilon_ {2} + \varepsilon_ {3}\tag{9.14}
$$

In Equations (9.6)–(9.8) the drift terms and errors are adding up because of the unit root. Past errors and drift terms are always being multiplied by 1 and so their impact will never diminish. This means that the mean of y will increase over time because of the build-up of drift terms α. The variance will also be increasing over time because of the build-up of random error terms $\boldsymbol { \varepsilon } _ { t }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/739aa0607920f852c7239cc12661eb3252fc76a42de6c77a92d2e4163d60d9e5.jpg)



Figure 9.4 Venn diagram of non-stationary processes


It is easy to confuse the different types ofnon-stationarity and so in Figure 9.4 the various possibilities for stochastic trends are depicted using a Venn diagram. This shows that random walks and random walks with drift are subsets of unit root processes and unit root processes are a subset of non-stationary processes. So in some cases, non-stationarity, unit roots and random walks are all the same thing. (Note that we have not shown deterministic trends in the diagram, although these are also in the set of non-stationary processes.) 

Why is non-stationarity a problem? It is a problem because, when nonstationary variables are regressed on non-stationary variables, this can create a spurious regression, i.e. a model that has a misleadingly high degree of explanatory power.<sup>3</sup> Looking at Figure 9.1 you will notice that computing investment and venture capital disbursements show trend increases over time. This may be because there is a causal relationship between these two variables but perhaps these variables are rising together by coincidence e.g. because the general economy is in a boom phase or because these variables are rising with GDP growth. Either way, the fact that the variables are exhibiting common trends means that they will be highly correlated: when we regress one of these non-stationary variables on the other the covariance between them is high so we will get a high $R ^ { 2 }$ , but not necessarily because we’ve detected any real relationship between the variables. Ice-cream sales also exhibit a common upward trend and so we’d also get a high $R ^ { 2 }$ if we regressed computing investment on ice-cream sales but of course there can be no (obvious) meaningful causal relationship between ice-cream and computing investment. 

As mentioned above, one classic sign ofa spurious regression is a systematic pattern in the residuals: there may be strong correlations between variables exhibiting common time trends but the model as a whole will be misspecified and the systematic pattern in the residuals will capture divergences in the upward trends for the dependent versus explanatory variables. So a high $R ^ { 2 }$ and a significant autocorrelation test together can be a sign that nonstationarity in the variables is generating a spurious result. Engle and Granger used this insight to construct the Engle–Granger rule of thumb and they observe that when $R ^ { 2 } > D W$ this may be a sign of a spurious regression reflecting non-stationarity in the variables. This is just a simple rule of thumb and, as with using the DW for a quick indicator of autocorrelation, more rigorous investigations should follow, as explained below. 

What can we say about the evidence for a spurious regression in our estimation of (9.2)? Our results reveal that $R ^ { 2 } = 0 . 9 8 4 > \mathrm { D W } = 0 . 2 5 6$ . So, using the Engle–Granger rule of thumb, we can conclude that there may be signs of a spurious regression. Therefore we should carefully explore the possibility that we are using non-stationary variables, e.g. by using the Dickey–Fuller (DF) and Augmented Dickey–Fuller (ADF) unit root tests outlined in Box 9.3. 

The DF and ADF tests for non-stationarity can easily be found using EViews by clicking on the variable name. Then pull down Unit Root Test from the View menu and click the appropriate boxes depending on whether you want to test that the level, first difference or second difference of the 

## Box 9.3 Testing for non-stationarity

Given the possibility of non-stationarity in time-series data, it is important to test for nonstationarity in all variables (dependent and explanatory) before running a regression. The most famous tests for non-stationarity are the Dickey–Fuller (DF) and Augmented Dickey– Fuller (ADF) unit root tests (there are other tests too). Both the DF and ADF test involve testing the $H _ { 0 }$ that a variable has a unit root. From Box 9.2: 

$$
y _ {t} = \rho y _ {t - 1} + \varepsilon_ {t}\tag{9.8}
$$

and a unit root process occurs when $\rho = 1$ . A simple example of a unit root process is: 

$$
y _ {t} = y _ {t - 1} + \varepsilon_ {t}\tag{9.9}
$$

In constructing DF/ADF tests, non-stationarity in y will affect the accuracy of a straightforward regression of (9.3). For this reason the DF/ADF tests are reformulated from (9.3) by subtracting $y _ { t - 1 }$ from both sides to give: 

$$
\Delta y _ {t} = \delta y _ {t - 1} + \varepsilon_ {t} \quad \text { where } \delta = \rho - 1\tag{9.15}
$$

The following hypotheses are then assessed using a one-tailed test: $H _ { 0 } : \rho = 1 , \delta = 0 ,$ $H _ { 1 } : \rho < 1 , \delta < 0$ . The $H _ { 0 }$ is that the variable is stationary and the $H _ { 1 }$ is that the variable is non-stationary. The DF/ADF tests involve constructing a τ (tau) test statistic calculated as: 

$$
\hat {\tau} = \frac {\hat {\delta}}{s e (\hat {\delta})}\tag{9.16}
$$

Whilst this looks like the formula for the conventional t test, it is important to remember that the potential non-stationarity in the variables generates a bias in small samples and affects the distribution of Student’s t test statistic. For this reason special Dickey–Fuller tables must be used to construct decision rules for the DF and ADF tests. Using the special DF tables, the decision rule is: 

$$
\text { if } | \hat {\tau} | > | \tau_ {\text { crit }} | \text { then   reject } H _ {0} \text { but   if } | \hat {\tau} | <   | \tau_ {\text { crit }} | \text { then   do   not   reject } H _ {0}.
$$

The DF test can be constructed using different specifications to control for other forms of trend apart from the stochastic trend generated by the unit root process. Other specifications incorporate intercepts to capture drift and/or time trend variables to capture deterministic trends. The three key specifications are of a simple random walk as described above (with no trend, no intercept), a random walk with drift (including an intercept term to capture the drift) and random walk with drift and trend (including an intercept term and a time trend to capture a deterministic trend). The DF Tables include three sets of critical values to cover these three groups of specification. The appropriate specification to use will depend on the characteristics of a given variable and the simplest way to judge the appropriate specification of the DF test involves inspecting plots of the variable over time, though model comparison tests will provide a more objective measure, as explained below. 

What about econometric problems with the DF test? When the DF test is characterised b autocorrelation in the residuals then the results are unreliable and so ADF tests must be used instead. The ADF test is much the same as the DF test but lagged Δys are included as well, to ‘mop-up’ any autocorrelation in the DF test. The simplest form of ADF test is an ADF(1) which incorporates one lag on $\Delta y _ { t - 1 }$ 

$$
\Delta y _ {t} = \delta y _ {t - 1} + \phi \Delta y _ {t - 1} + \varepsilon_ {t}\tag{9.17}
$$

It is important to remember that we will still be constructing the test statistic using (9.6) and using the accompanying decision rule as outlined above. The variable $\Delta y _ { t - 1 }$ has been included just to resolve the autocorrelation problem. For the ADF tests, the DF tables are used and, as for DF tests, the ADF test can be expanded to control for drifts and deterministic trends. 

In this example, we have included only one lag on the dependent variable in order to keep things simple. But in reality, as many lagged variables as are necessary to eliminate the autocorrelation should be included in the ADF tests. Deciding how many lags to include in the ADF tests will depend on how many lags are needed to remove significant autocorrelation in the residuals of the DF/ADF tests. In practice, econometrics packages will automatically report the best specification by using some general model comparison tests to identify the relative explanatory power of the various forms of the test. Some of the model comparison tests used include Akaike’s Information Criterion and the Schwartz Information Criterion. A detailed explanation of these model comparison tests is beyond the scope of this book but in essence they are based around the RSS and so are capturing the residual variance of the different specifications. 

variable has a unit root. You will also have to make a choice about whether to include either just an intercept or an intercept plus trend (as explained in Box 9.3, an inspection ofa time-plot ofthe variable is a simple way to decide which of the specifications is appropriate). Then click on OK and EViews will report the results from the best specification of the DF/ADF test (and the judgement about the best specification is made using model comparison tests, also explained in Box 9.3). 

For the variables in our model, Figure 9.1 suggests that both variables are drifting upwards over time at an increasing rate. We control for these factors by including an intercept and a deterministic trend in our specifications of the 

DF/ADF tests. For $^ { c i , }$ the ADF(1) test includes one lag on $\Delta c \dot { \boldsymbol { \imath } } _ { t }$ giving the following estimated equation: 

$$
\begin{array}{r l r l r l} \Delta c i _ {t} & = 0. 6 4 1 & - 0. 2 6 2 c i _ {t - 1} & + 0. 7 9 1 \Delta c i _ {t - 1} & + 0. 0 3 7 3 T i m e & + \hat {\varepsilon} _ {t} \\ t & = 2. 4 6 1 & \tau & = - 2. 0 8 7 & t & = 3. 4 5 7 \\ p & = 0. 0 2 3 6 & p & = 0. 0 5 1 & p & = 0. 0 0 2 6 \\ R ^ {2} & = 0. 5 3 7 & \bar {R} ^ {2} & = 0. 4 6 4 & D W & = 1. 8 1 0 \end{array} \tag {9.1}\tag{9.18}
$$

As explained in Box 9.3, for the test on computing investment, we are focussing on the parameter estimates on $c i _ { t - I }$ . EViews has selected ADF(1) as the best specification of the DF/ADF test. Using a 5% significance level (remembering that special of tables must be used, as explained in Box 9.3), $p = 0 . 0 5 1 > 0 . 0 5$ so we do not reject $H _ { 0 }$ and can conclude that ci is non-stationary and does have a unit root, though this decision is borderline. The fact that the parameters on the intercept and drift terms are significantly different from zero at a 10% significance level suggests that there is some evidence supporting the existence of a drift and deterministic trend in our specification of this unit root test. 

We get similar results for vc and both sets of results are summarised in Table 9.1. The key difference between the test of ci and the test on vc is that EViews selects ADF(4) as the best specification for testing vc; this is an ADF test with 4 lags on $\Delta c \dot { \boldsymbol { \imath } } _ { t }$ . The probability value for this ADF(4) test is $p { = } 0 . 1 2$ and so $\textstyle p > 0 . 0 5$ . We do not reject $H _ { 0 }$ and we conclude that vc is also a nonstationary unit root process. 

What do we do if we have non-stationary variables? Unless the variables are cointegrated (a relatively complex issue that will be introduced in Chapter 10) then we must use the variables in stationary form. Non-stationarity can be eliminated by differencing the variables and to establish whether or not these first differences are themselves stationary they are tested for a unit root using the DF/ADF tests. Ifthe first differences are also non-stationary then they should be differenced again to give the second differences which again should tested for unit roots etc. etc: this process continues for as long as it takes to reject the $H _ { 0 }$ of a unit root. The number of times that the variables must be differenced to make it stationary is the order of integration of the variable, with the order of integration indicated by the notation $I ( q )$ , where $q$ is the order of integration. 

From Table 9.1, we can see that both our variables ci and vc are stationary in first differences, i.e. $\Delta c \dot { \boldsymbol { \imath } } _ { t }$ and $\Delta \nu c _ { t }$ are I(0); $c i _ { t }$ and $\nu c _ { t }$ are I(1) and so a regression on first differences should remove the non-stationarity and should give a non-spurious regression result. 


Table 9.1 Unit root tests (with constant and linear trend)


<table><tr><td></td><td>Lag length</td><td><eq>\hat{\tau}</eq></td><td>Probability value</td><td>5% critical value from DF tables</td><td>Inference</td></tr><tr><td colspan="6">Computing investment - logged (ci)</td></tr><tr><td>Level</td><td>1</td><td>-2.09</td><td>0.53</td><td>-3.62</td><td>Do not reject <eq>H_0 \rightarrow</eq> non-stationary</td></tr><tr><td>First difference</td><td>5</td><td>-4.16</td><td>0.02</td><td>-3.69</td><td>Reject <eq>H_0 \rightarrow</eq> stationary</td></tr><tr><td colspan="6">Venture capital disbursements - logged (vc)</td></tr><tr><td>Level</td><td>4</td><td>-3.16</td><td>0.12</td><td>-3.66</td><td>Do not reject <eq>H_0 \rightarrow</eq> non-stationary</td></tr><tr><td>First difference</td><td>0</td><td>-4.00</td><td>0.02</td><td>-3.62</td><td>Reject <eq>H_0 \rightarrow</eq> stationary</td></tr></table>

This all suggests, not necessarily that venture capital is unimportant to computing investment, but that the determinants of computing investment are more complex than we initially postulated. So we cannot trust the results from our initial regression summarised in Equation (9.2). The next step would be to ensure that we include stationary versions of our variables in the model – see chapter exercises. 

## Structural breaks and non-stationarity

So far we have treated structural breaks and non-stationarity as separate issues but it is possible that both problems are occurring in the same data set. It is also possible that the presence of one of these problems will reduce the power of tests for the other; for example, the presence ofstructural breaks will reduce the power of the DF/ADF tests because if a break is not controlled for then the DF/ADF tests will pick up its influence. 

For our investigation of the links between computing investment and venture capital we have shown that there is significant evidence of a structural break. There is also significant evidence of a unit root in the computing investment and venture capital variables. In estimating our model we can incorporate both possibilities. Table 9.2 shows the results from a regression on the first differences of computing investment and venture capital (as we showed above, these first differences are the stationary, I(0) forms of our variables). We have also incorporated additive and multiplicative dummies to control for parameter shifts from 1995 onwards (using dummies to capture parameter shifts is explained in Box 9.1). 

The results from this final estimation are a lot more promising than our earlier regressions. There are no immediate signs of a spurious regression because $\mathrm { D W } > R ^ { 2 }$ . We have also conducted a BG test for residual autocorrelation (the methodology for the BG test is explained in Chapter 7) giving $F { = } 1 . 9 2 5$ $[ p = 0 . 1 7 5 ] ;$ so with $ { p } > 0 . 0 5$ we can retain the $H _ { 0 }$ of no autocorrelation at a 5% significance level (and in fact at any significance level up to 17.5%). 


Table 9.2 Summary of EViews printout Estimation on I(0) variables, with structural break in 1995


<table><tr><td colspan="5">Dependent Variable: ΔLCIMethod: Least SquaresSample (adjusted): 1981 2004</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>0.157</td><td>0.016</td><td>9.832</td><td>0.000</td></tr><tr><td>ΔVC</td><td>-0.002</td><td>0.032</td><td>-0.070</td><td>0.945</td></tr><tr><td>D</td><td>-0.068</td><td>0.024</td><td>-2.862</td><td>0.010</td></tr><tr><td>D.ΔVC</td><td>0.127</td><td>0.045</td><td>2.809</td><td>0.011</td></tr><tr><td>R-squared</td><td>0.500</td><td>F-statistic</td><td></td><td>6.657</td></tr><tr><td>Adjusted R-squared</td><td>0.425</td><td>Prob(F-statistic)</td><td></td><td>0.003</td></tr><tr><td>Durbin-Watson statistic</td><td>1.456</td><td></td><td></td><td></td></tr></table>

The parameter estimates also confirm our initial judgements about the relationships between computing investment and venture capital as outlined in Section 9.3: there is a clear association between computing investment and venture capital only from 1995 onwards and this is reflected in the statistically significant parameter estimate on the additive dummy D and the multiplicative dummy $D \cdot \nu c _ { t }$ 

## 9.5 Implications and conclusions

Our empirical analysis has shown that the relationship between computing investment and venture capital funding is affected by structural breaks and non-stationary variables. So we tested and corrected for non-stationarity and controlled for structural breaks. Our preferred estimation suggested that parameter shifts affected the interaction between growth in computing investment and venture capital funding. Our results indicate firstly, that there is a significant upward shift in computing investment from 1995 onwards and secondly, that growth in computing investment was associated with growth in venture capital funding from 1995 onwards but not before. Growth in venture capital funding only had a significant impact on growth in computing investment from 1995 onwards. This latter finding may suggest that it takes time to build up momentum in the financing of innovative investments – perhaps because venture capitalists need clear evidence that an innovative burst will be sustained before they are prepared to commit their money to risky innovative ventures. 

In terms of policy implications, if our finding about delays in the provision ofventure capital funds is robust, then it suggests that governments could play a role in ensuring that funds are available to subsidise innovative new industries (e.g. see UNCTAD, 2008). This may be particularly important for computing innovations given the evidence about the economic benefits of computerisation. Also, the considerable volatility in venture capital funding, as captured by the spike in venture capital disbursements in Figure 9.1, suggests that trends in private venture capital disbursements can be unstable, e.g. as shown during the 1999–2001 period of the dotcom bubble and subsequent bust. Volatility in private venture capital financing has the potential to create significant instability in the macroeconomy and so financial policies could be implemented to manage this instability. Overall, governments may have a role to play both in supporting innovative investment and in managing the volatility that emerges via the private financing of innovative investments. 

## Further reading

## Text books



Schumpeter, J. A. (1939) Business Cycles: A Theoretical, Historical and Statistical Analysis ofthe Capitalist Process, New York: McGraw-Hill. 





Thomas, R. L. (1997) Modern Econometrics – An Introduction, Harlow: Addison-Wesley, Chapters 13 and 14. 



## Academic articles and working papers



Baddeley, M. (2008) ‘Structural shifts in UK unemployment: the twin impacts of financial deregulation and computerisation’, Bulletin of Economic Research, vol. 60, no. 2 (April), 123–57. 





Cecchetti, S. G. (2002) The New Economy and Challenges for Macroeconomic Policy, National Bureau of Economic Research Working Paper No. 8935, National Bureau of Economic Research. 





Gordon, R. J. (2000) ‘Does the “New Economy” measure up to the great inventions ofthe past?’, Journal ofEconomic Perspectives, vol. 14, 49–74. 





Whelan, K. (2002) ‘Computers, obsolescence and productivity’, Review of Economics and Statistics, vol. 84, no. 3, 445–61. 





Yang, S. and Brynjolfsson, E. (2001) ‘Intangible Assets and Growth Accounting: Evidence from Computer Investments’, Massachusetts Institute of Technology, downloaded from http:// ebusiness.mit.edu/erik/itg01-05-30.pdf. 



Policy briefs and newspaper articles 



Dunne, T. (1991) Technology Usage in US Manufacturing Industries, Washington D.C.: US Census Economic Studies. 



Landefeld, J. S. and Fraumeni, B. M. (2000) ‘Measuring the New Economy’, US Bureau of Economic Analysis Advisory Committee Meeting. 



Solow, R. M. (1987) ‘We’d better watch out’, New York Times Book Review, 12 July 1987, 36. 



UNCTAD (2008) Science and Technology for Development: the New Paradigm of ICT, Geneva and New York: United Nations. 

## 9.7

## Chapter exercises

1. Using the methodology outlined in Box 9.1 and the data sources outlined in Section 9.3, extend the Chow testing methodology to construct your own test for two structural breaks, i.e. a first break in 1995 and a second break in 2000. (Hint: this will involve an unrestricted model estimated for three separate subperiods rather than two.) Verify the results of your test using EViews. 

2. In the final version of our computing investment model we ran regressions on a hybrid model that simultaneously addressed problems of nonstationarity and parameter instability. Estimate a computing investment model that incorporates only stationary variables (i.e. estimate a model that does not control for structural breaks). Discuss your results commenting in particular on whether the regression on stationary variables has, by itself, resolved the problems identified in the initial estimations ofEquation (9.2). 

# Error correction models Consumption and the multiplier in the UK

Economic issues include: 

 Marginal and average propensities to consume 

 The multiplier 

 Permanent income hypothesis and life-cycle hypothesis Econometric issues include: 

 Autoregressive distributed lag (ARDL) models 

 Error correction models (ECMs) and cointegration 

 Granger causality tests 

Data issues include: 

 Using lags 

## 10.1 The issue

When income rises do we spend more or save more? This question most famously excited the interest of the British economist, John Maynard Keynes (1883–1946) during the depression years of the 1930s, but it is of equal importance today. Consumption is the single largest element in household spending and has significant implications for demand and the subsequent health of the economy. Recognition of this role of household spending was evident in the flurry of newspaper articles in late 2001 and early 2002, when many commentators feared the world was headed for recession, if not a complete depression. ‘The shoppers who saved the nation’ was a typical headline in 2005: journalists who had previously expressed shock at the high debt held at stores and on credit cards by the average household, now applauded the fact they were continuing to spend and thereby maintaining the multiplier effects that might ward off the nation’s – and indeed the world’s – slide into recession. Policy-makers struggled to estimate precisely the extent to which an extra dollar’s spending would trickle through the economy to keep the country’s producers, manufacturers and retailers afloat. 

What explains these rises in consumption? Across the OECD, spending patterns have been changing in response firstly to the loosening of consumer credit controls following financial deregulation, and secondly to the more fluid flows of foreign finance encouraged by globalisation. But if too much money is being pumped into consumption in the current period then it means that not enough will be saved to spend on investment in future productive capacity. 

In this chapter we explore one of the factors affecting consumption by analysing the relationships between income and consumption. We examine two important theoretical consumption models: the Keynesian consumption function and Friedman’s consumption function. In the empirical estimations, we analyse these models empirically for the UK 1979 to 2005. We use the hypothesis of a stable average propensity to consume (APC) to construct an error correction model (ECM) – an empirical specification that enables us simultaneously to capture long-run equilibrium and short-run ‘out-ofequilibrium’ dynamics. 

## 10.2 The theory

In analysing consumption theory we start with Keynes’s analysis of consumption (Keynes, 1936, 1937). The marginal propensity to consume (MPC) lies at the core ofKeynes’s analysis and reflects specific assumptions about human nature and about our psychological motivations. Keynes asserted that: 

… the prevailing psychological law seems to be that when aggregate income increases, consumption-expenditure will also increase but to a somewhat lesser extent. (Keynes, 1937, p. 219) 

That is, we will spend more when our income rises, but not by as much as our increase in income. Technically speaking, the marginal propensity to consume is positive but less than 1: consumption rises as income rises but by a lesser proportion. The MPC is central to Keynes’s macroeconomic analysis because it drives the multiplier effect. Multiplier effects emerge because various spillover effects are generated by each spending transaction. As we spend more on consumer goods, shops employ more sales staff to cope with the increased demand; factories employ more staff to meet the increased demand from the shops; suppliers boost their production capacity to cope with the increased demand for their inputs. More truck drivers and perhaps more trucks are needed to ferry the goods from supplier to factory to warehouse to shop. And so on. Sales assistants, factory workers and truck drivers will each have more income to spend spurring more and more consumption spending. Via these multiplier effects, household consumption decisions permeate through to all the corners of the economy. 

We can analyse the impact of these multiplier effects mathematically. Assuming a closed economy with no trade and no government, the simplest form of the multiplier is: 

$$
\mathrm{Multiplier} = \frac {1}{1 - M P C}\tag{10.1}
$$

For example, if the estimate of MPC was 0.8, this means that a £1 increase in income will produce a £0.80 increase in spending for each individual and the multiplier will be 5: 

$$
\mathrm{Multiplier} = \frac {1}{1 - 0 . 8} = 5\tag{10.2}
$$

This captures the fact that each 80% increase in household spending trickles down through all the various sectors of the economy generating £5 of total income per £1 of initial income. 

This can be shown with a simple arithmetic example. Let’s assume that everyone has the same MPC of0.8, i.e. they spend 80% oftheir current income on consumption. To keep it simple, we will also assume that the prices are net of production costs such as the price of raw materials etc. As shown in Table 10.1, imagine that Bob gets an extra £10 in his pay-packet and spends 80% of it (i.e. £8) buying beer from Sally. So Sally’s income has increased by £8. Sally uses 80% of this £8 (i.e. £6.40) to buy some cherries from Sanjeev. Sanjeev uses 80% ofhis income of£6.40 (i.e. £5.12) to buy pencils from Joshua. Joshua uses 80% of his £5.12 income to buy chocolate from Maya. Maya buys £3.28 of bread from Lee; Lee buys £2.62 of nuts from Abdul; Abdul buys £2.10 of milk from Theo. And so the process continues until the increments to further spending become too small to measure. From the table you can see that the initial £10 that Bob earned has been multiplied up to generate a total extra income of more than £40 for them all. 


Table 10.1 Illustrating the multiplier effect


<table><tr><td></td><td>Bob</td><td>Sally</td><td>Sanjeev</td><td>Joshua</td><td>Maya</td><td>Lee</td><td>Abdul</td><td>Theo</td><td>Total</td></tr><tr><td>MPC</td><td>0.8</td><td>0.8</td><td>0.8</td><td>0.8</td><td>0.8</td><td>0.8</td><td>0.8</td><td>0.8</td><td></td></tr><tr><td>Income</td><td>£10</td><td>£8</td><td>£6.40</td><td>£5.12</td><td>£4.10</td><td>£3.28</td><td>£2.62</td><td>£2.10</td><td>£41.62</td></tr><tr><td>Consumption</td><td>£8</td><td>£6.40</td><td>£5.12</td><td>£4.10</td><td>£3.28</td><td>£2.62</td><td>£2.10</td><td>£1.68</td><td>£33.3</td></tr></table>

This is an example of a geometric progression – a type of mathematical series which determines how an initial value (of£10 in this case) increases over time and it can be summarised as: 

$$
\begin{array}{l} \sum_ {n = 1} ^ {\infty} (\mathfrak {E} 1 0 \times 0. 8 ^ {n}) = (\mathfrak {E} 1 0 \times 0. 8 ^ {0}) + (\mathfrak {E} 1 0 \times 0. 8 ^ {1}) + (\mathfrak {E} 1 0 \times 0. 8 ^ {2}) \dots (\mathfrak {E} 1 0 \times 0. 8 ^ {n}) \\ = \mathfrak {E} 1 0 + (\mathfrak {E} 1 0 \times 0. 8) + (\mathfrak {E} 1 0 \times 0. 8 \times 0. 8) + (\mathfrak {E} 1 0 \times 0. 8 \times 0. 8 \times 0. 8) + \dots e t c. \end{array}\tag{10.3}
$$

If this process were to continue ad infinitum (i.e. beyond Theo’s spending) until, for the last person, income earned is negligible, everyone together would have earned a total of £50, i.e.: 

$$
M u l t i p l i e r = \frac {1}{1 - M P C} = \frac {1}{1 - 0 . 8} = 5\tag{10.4}
$$

Research into the relationship between the MPC and the multiplier has taken many forms, with writers focussing on different countries, different periods of history, different occupational groups, and even different forms of incomes; for example, most studies measure income by using measures of aggregate income, but some have narrowed the focus down to look specifically at income effects that are created by rising equity markets, or rising house prices. An eclectic sample of these is shown in Table 10.2 to illustrate the importance of context: the MPC will vary geographically and across occupations. 

Each diverse sample noted in Table 10.2 reveals an interesting insight. The 1951 study by Jan Tinbergen compared the multiplier effects created by the spending habits of different occupational groups – and found that manual workers created more spillover benefits than farmers for example. Tinbergen also compared the MPC of different countries. More recently, researchers at the Bank ofEngland examined consumption patterns ofdifferent countries, focussing only on the behaviour of people who owned shares, but looking at income in aggregate measures rather than equity income (Norman et al., 2002). They found that as the value of share portfolios increased, greater multiplier effects were generated; for example, American households generate greater multiplier effects through their spending patterns than German or French households because they hold more equity. 


Table 10.2 Differing estimates of MPC and the multiplier


<table><tr><td>Studies included:</td><td>Estimated MPC</td><td>Implied Multiplier</td></tr><tr><td colspan="3">National occupational groups (Tinbergen, 1951)</td></tr><tr><td>manual workers</td><td>0.83</td><td>5.88</td></tr><tr><td>‘brain workers’</td><td>0.82</td><td>5.56</td></tr><tr><td>agricultural workers</td><td>0.70</td><td>4.76</td></tr><tr><td>farmers</td><td>0.44</td><td>1.78</td></tr><tr><td colspan="3">Countries (aggregate income) (Tinbergen, 1951)</td></tr><tr><td>Germany</td><td>0.42</td><td>1.72</td></tr><tr><td>Britain</td><td>0.52</td><td>2.08</td></tr><tr><td>Sweden</td><td>0.60</td><td>2.50</td></tr><tr><td>Poland</td><td>0.71</td><td>3.44</td></tr><tr><td>United States</td><td>0.75</td><td>4.00</td></tr><tr><td colspan="3">Countries – equities income (Source: Norman et al., 2002)</td></tr><tr><td>United States</td><td>0.80</td><td>5.0</td></tr><tr><td>Germany</td><td>0.50</td><td>2.0</td></tr><tr><td>France</td><td>0.60</td><td>2.5</td></tr></table>

But how does the empirical evidence fit Keynes’s theory? The shiftfrom-thrift arguments outlined above imply that the average propensity to consume (APC) will fall as income rises. This can be shown as follows: 

$$
A P C = \frac {C}{Y} = \frac {\alpha + \beta Y}{Y} = \frac {\alpha}{Y} + \beta\tag{10.5}
$$

where $\beta$ is the MPC (and is assumed to be a constant) and α is autonomous consumption; both α and $\beta$ are constants and so the APC should fall as Y rises because as Y is increasing, $\frac { \alpha } { Y }$ will necessarily get smaller as Y gets larger (given that α is a constant). 

There has been substantial empirical debate about whether or not it is defensible to assume a falling APC. Historical evidence from Kuznets (1946) shows that, historically, the APC has been stable and this does appear to undermine Keynes’s specification of the consumption function. Also, theoretical critics of Keynes’s theory argued that Keynesian consumers are a bit simple-minded. Their decision to spend or save depends only on their current income: ifincome rises one week, they will spend more; ifit falls the next week, they will spend less. Lags may be important, as explained in Box 10.1. Also, can we really aggregate to an entire nation made up of diverse peoples, of different ages and tastes for example, from such a simplistic vision of a household? 

## Box 10.1 Using lags

In the Keynesian model of consumption, current consumption is expressed as a function of current income. In practice this means (for example) that consumption in 1980 is determined by income in 1980; consumption in 1981 is set against 1981’s income and so on. The implicit assumption here is that people can observe a change in their real disposable incomes and respond very quickly – there is no lag between an increase in wages (or a fall in taxes, or inflation) and corresponding increases in consumption expenditure. This implies either that people are responding to current income or that, even though current consumption is not a direct function of current income, current income is acting as a proxy for future expected income. 

Generally there may be many reasons to expect lagged effects i.e. that a change in the explanatory variable in one year will take time to feed through to a change in the dependent variable. For example, lags are particularly important in agricultural markets. When the price of wool increases (P), we expect farmers will not be able to increase their supply of wool (S) for at least one year (assuming they had no wool stockpiled from previous years and so needed to breed more sheep). In this case, the model specification should be $S _ { t } =$ $a + \beta P _ { t - 1 } + \varepsilon _ { t } ,$ . If the lag was as long as two years, we would write the equation as $S _ { t } { = } a +$ $\beta _ { 1 } P _ { t - 1 } + \beta _ { 2 } P _ { t - 2 } + \varepsilon _ { t } .$ 

More complex lag structures exist, ranging from the relatively straight-forward distributedlag specification where the lag effect is spread out over a number of time periods e.g. $S _ { t } =$ $a + \beta _ { 0 } P _ { t } + \beta _ { 1 } P _ { t - 1 } + \beta _ { 2 } P _ { t - 2 } + \beta _ { 3 } P _ { t - 3 } + \varepsilon ;$ to more complex models such as Median and Mean lag models, and models incorporating partial adjustment and adaptive expectations, such as the Koyck model.<sup>1</sup> 

Choosing which lag structure to use depends on the reason a delay is expected. Lags may be institutional (e.g. students need time to finish their degrees before they can respond to new employment opportunities; homeowners need to sit out fixed duration mortgage contracts before they can respond to cuts in interest rates); technological (sheep still take at least half a year to grow a new woollen coat and a year to reproduce themselves); or psychological (habit and addiction make us slow to change; as does the belief that something is a ‘one-off’ and will not be repeated). More generally, technological progress may reduce lags by speeding up production and distribution processes. The development of new technologies and use of flexible employment or financial contracts has hastened the rate with which we can respond to unexpected events. It may also be that we can learn from past experiences (and economic research!). 

Keynesian theory is a demand-led theory built in a world ofexcess capacity, where the economy is below full employment. Other theories, such as Friedman’s and Modigliani’s focus more on the supply-side and on future expectations of future income (rather than current income) as determinants of current consumption. These ideas underlie more sophisticated postulates about human behaviour, including the argument that people’s spending decisions in the present are based on their expectations about the future generating consumption smoothing. Milton Friedman argues that it is not current income that determines how you spend or save, but your expected permanent income. Ifwe get a wage rise but expect it to be short-term, lasting only a year for example, it may not be sensible just to increase our spending. Rather, we might save the extra money, seeing it as a one-off bonus. But if we expect a permanent wage rise, then we would increase our spending accordingly. This is the essence of the permanent income hypothesis (PIH). 

Friedman’s model is describing microeconomic decisions and applying them to a macroeconomic context so it is a micro-founded macroeconomic theory. Micro-founded theories are built around the representative agents hypothesis (first introduced in Chapter 8). This hypothesis asserts that if we describe the behaviour ofone representative household then, assuming that all households behave in the same way as the representative agent (at least on average), this representative behaviour captures aggregate macroeconomic behaviour too. 

Another consumption-smoothing theory of consumption is the life-cycle theory, formulated by Franco Modigliani. He suggests that rather than follow the reflex response implied by Keynes, we intelligently calculate our expected income stream over our entire lives, and spend in each year that amount which would enable us to ‘break even’ in our (predicted) year of death. So we spend more than we earn when we are young (e.g. when we are students), less than we earn when we are older and more again when we retire. 

More recently, behavioural economists have investigated whether or not the consumption-smoothing approaches are consistent with real-world behaviour. At a microeconomic level, Veblen effects may operate: we may consume something because we see our neighbours consuming it. Past experiences and past expectations will have an impact; consumption may reflect ingrained habits rather than sensible choices. People may have relatively short time horizons and their preferences may shift over time. This will mean that consumption behaviour is not necessarily rational and sensible in the ways envisaged by Friedman and Modigliani. 

None ofthe theories outlined in this theory section can offer a single, perfect, explanation. Modigliani’s life-cycle consumers may find that no matter how accurate are their forecasts oftomorrow’s income, the bank will not grant them the loan they need today and so liquidity constraints will mean that people don’t have the necessary cash that they need to buy something that they want today because they cannot borrow money. 

In this chapter, we investigate these issues in analysing the relationships between consumption and income in the UK 1979 to 2005. We will analyse two specifications of the consumption function: the Keynesian consumption function and Friedman’s PIH consumption function. 

## 10.3 The data


The data used in this chapter is published by the UK’s Office of National Statistics (ONS). Consumption and income incorporated in real terms using the following data sources:


<table><tr><td>Variable</td><td>Source</td><td>Website</td></tr><tr><td>Final Consumption Expenditure – current prices (RPQM) deflated using the RPI (CZBH)</td><td>UK ONS, Economic Trends Annual Supplement (ETAS)</td><td>www.statistics.gov.uk</td></tr><tr><td>Real household disposable income (OSXS)</td><td>UK ONS, Economic Trends Annual Supplement (ETAS)</td><td>www.statistics.gov.uk</td></tr></table>

In assessing the relationships between consumption and income we will examine evidence for some of the theoretical predictions outlined in Section 10.2. As mentioned above, Kuznets (1946) presented evidence showing that the APC was stable over time and this result is inconsistent with Keynes’s specification of the consumption function. In reassessing Kuznets’s evidence about a stable APC we can inspect the raw data: Figure 10.1 plots consumption and real disposable income over time revealing a relatively steady relationship between the two, though there are some short-term fluctuations. 

Figure 10.2 plots the APC over time using annual data and whilst there are episodes where the APC has been relatively high or relatively low, overall it does seem to be steady at around 0.70, again suggesting that the APC is stable. 

Together our data show that Kuznets’s early finding is being mirrored in recent data. This stable pattern suggests that changes in income are being matched by equivalent changes in consumption. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/54d80f0842fff780c2e3e638a21c18a4a37415d655d73bf729d38d9eb92a90ac.jpg)



Figure 10.1 Real consumption and real disposable income – UK 1979–2005


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/01b9a628442e79d2526ca845eb107789a08672b082c3190c29db324b1c67604b.jpg)



Figure 10.2 Aggregate average propensity to consume (APC), UK 1979–2005


In the following empirical section we will assess the Keynesian consumption function and Friedman’s consumption function, keeping in mind that a stable APC would be more consistent with the latter functional form. We will also use the evidence about a stable APC to build an error correction model (ECM) of the relationship between consumption and income, as will be explained below. 

## 10.4 Empirical methods and results

In this section we will estimate Keynes’s consumption function and Friedman’s consumption function. Our empirical models will be as follows. 

## Keynesian consumption function

To recap on the key theoretical postulates, Keynes (1936) assumed a stable marginal propensity to consume and so the Keynesian empirical model is ofthis form: 

$$
C _ {t} = \alpha + \beta Y _ {t} + \varepsilon_ {t}\tag{10.6}
$$

where $0 < \beta < 1$ 

As shown above in Equation (10.5), this mathematical relationship implies a stable MPC. It also implies that the APC is declining. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/e76ddc819e3273df5522081759d252557ecdd57226ca06e7ee072a66e3260dae.jpg)



Figure 10.3 Scatter plot of consumption against income, UK data


To capture the patterns between consumption and income, we show a scatter plot in Figure 10.3. This scatter plot reveals a relatively steady positive relationship between consumption and income and the trend line captures a linear pattern consistent with the Keynesian specification of the consumption function. However there is some evidence that the relationship is not completely robust: some of the observations on consumption (those associated with low to middling levels of income) are relatively far away from the trend line. 

## Friedman’s permanent income hypothesis (PIH)

As explained in Section 10.2 Friedman’s permanent income hypothesis is based around rational, forward-looking consumption-smoothing behaviour. Friedman constructs a consumption function around a multiplicative function form as follows: 

$$
C _ {t} = \alpha Y _ {t} ^ {\mathrm{P}} v _ {t}\tag{10.7}
$$

where $Y ^ { \mathrm { p } }$ is permanent income and $v _ { t }$ is a stochastic error term with a mean of zero. Permanent income is assumed, on average, equal to total income. (Shocks to consumption are assumed to be random with a mean of zero.) With this multiplicative form ofconsumption function, the elasticity is unitary and the APC will be constant: as Ygoes up, C goes up by a proportional amount and so the APC is unchanging.<sup>2</sup> Here we have a model that is non-linear in the variables but by taking logs we get the following model (which is linear in the parameters, thus satisfying one of the Gauss–Markov assumptions explained in chapter 1): 

$$
c _ {t} = \ln \alpha + \beta y _ {t} + \varepsilon_ {t}\tag{10.8}
$$

where $c$ is logged consumption, y is logged income and $\varepsilon = \ln ( \upsilon )$ . To be consistent with (10.7) and the unitary long-run elasticity explained above, we assume that $\beta = 1$ 

Before estimating the models, we establish the orders of integration of each variable using Augmented Dickey–Fuller tests (as explained in Chapter 9 – see Table 10.3). 


Table 10.3 Augmented Dickey–Fuller unit root tests


<table><tr><td rowspan="2"></td><td colspan="3">Levels</td><td colspan="3">First Difference</td></tr><tr><td>t-Statistic</td><td>Prob.*</td><td>Critical value 5% level</td><td>t-Statistic</td><td>Prob.*</td><td>Critical value 5% level</td></tr><tr><td>Consumption (C)</td><td>1.34</td><td>1.00</td><td>-2.98</td><td>-3.38</td><td>0.02</td><td>-2.99</td></tr><tr><td>Income (Y)</td><td>2.21</td><td>1.00</td><td>-2.98</td><td>-3.32</td><td>0.02</td><td>-2.99</td></tr><tr><td>Logged consumption (c)</td><td>-1.13</td><td>0.68</td><td>-3.02</td><td>-4.06</td><td>0.01</td><td>-3.02</td></tr><tr><td>Logged income (y)</td><td>0.55</td><td>0.99</td><td>-2.98</td><td>-3.54</td><td>0.02</td><td>-2.99</td></tr><tr><td>Error Correction Term (EC)</td><td>-3.27</td><td>0.03</td><td>-2.99</td><td>n/a</td><td>n/a</td><td>n/a</td></tr></table>

Using a 5% significance level, these tests indicate that consumption, income, logged consumption and logged income are I(1). We have also constructed an error correction term variable. The meaning and usefulness of this variable will be explained below but note for the moment just that this error correction term is I(0). (We have also tested the variables for structural breaks and have found no significant evidence of breaks at a 5% significance level.) 

The EViews output from the estimation of (10.6) (the Keynesian consumption function) is summarised in Table 10.4. Note that this estimation (and the subsequent ones too) include a deterministic trend term (‘Time’) to capture systematic upward trends over time. (Deterministic trends were explained in Chapter 9.) 


Table 10.4 EViews output: Keynesian consumption function


<table><tr><td colspan="5">Dependent Variable: Consumption (C)</td></tr><tr><td colspan="5">Sample: 1979 2005</td></tr><tr><td colspan="5">Included observations: 27</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>-5.21</td><td>1.69</td><td>-3.08</td><td>0.01</td></tr><tr><td>Income (Y)</td><td>0.90</td><td>0.16</td><td>5.57</td><td>0.00</td></tr><tr><td>Time</td><td>0.30</td><td>0.34</td><td>0.89</td><td>0.38</td></tr><tr><td>R-squared</td><td>0.99</td><td>F-statistic</td><td></td><td>1432.91</td></tr><tr><td>Adjusted R-squared</td><td>0.99</td><td>Prob(F-statistic)</td><td></td><td>0.00</td></tr><tr><td>DW</td><td>0.75</td><td></td><td></td><td></td></tr><tr><td colspan="5">Diagnostic Tests</td></tr><tr><td colspan="5">Breusch-Godfrey Serial Correlation LM Test:</td></tr><tr><td></td><td>F-statistic</td><td>10.20</td><td>Probability</td><td>0.00</td></tr><tr><td colspan="5">Ramsey RESET Test:</td></tr><tr><td></td><td>F-statistic</td><td>0.47</td><td>Probability</td><td>0.50</td></tr></table>

An initial inspection of these results from the estimation of the Keynesian consumption function suggest that the null that the parameter on income is equal to zero can be rejected at a 5% significance level. Also, the F test of explanatory power indicates that the null of no association between the dependent variable and explanatory variable can be rejected at a 5% significance level. However, these results are unlikely to be reliable; the Breusch–Godfrey test (conducted here as an AR(4) version) indicates that the null of no autocorrelation in the errors must be rejected with a 5% significance level. 

From Chapter 9 (and our unit root test results as summarised in Table 10.3), you will probably guess that non-stationarity in our variables is generating spurious regression results; and adopting the Engle–Granger Rule of Thumb (explained in Chapter 9) we can provisionally infer that there is evidence of a spurious regression because $R ^ { 2 } { > } \mathrm { D W } .$ So non-stationarity in our variables is creating a problem but (as also explained in Chapter 9) this can be resolved by differencing our variables. 


Table 10.5 EViews output: Friedman’s permanent income model


<table><tr><td colspan="5">Dependent Variable: Consumption (logged) (c)</td></tr><tr><td colspan="5">Sample: 1979 2005</td></tr><tr><td colspan="5">Included observations: 27</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>9.33</td><td>0.79</td><td>11.76</td><td>0.00</td></tr><tr><td>Income (logged) (y)</td><td>0.83</td><td>0.25</td><td>3.39</td><td>0.00</td></tr><tr><td>Time</td><td>0.01</td><td>0.01</td><td>0.95</td><td>0.35</td></tr><tr><td>R-squared</td><td>0.99</td><td>F-statistic</td><td></td><td>1176.22</td></tr><tr><td>Adjusted R-squared</td><td>0.99</td><td>Prob(F-statistic)</td><td></td><td>0.00</td></tr><tr><td colspan="5">Diagnostic tests</td></tr><tr><td colspan="5">Breusch-Godfrey LM Test:</td></tr><tr><td></td><td>F-statistic</td><td>5.73</td><td>Probability</td><td>0.00</td></tr><tr><td colspan="5">Ramsey RESET Test:</td></tr><tr><td></td><td>F-statistic</td><td>0.70</td><td>Probability</td><td>0.41</td></tr></table>

Turning to our second hypothesis, the EViews output from the estimation of equation (10.8) (Friedman’s permanent income consumption function) is summarised in Table 10.5. 

On initial inspection, these results are similar to the results from the estimation of the Keynesian consumption function: the $R ^ { 2 }$ is high and there is a highly significant relationship between logged consumption and logged income. But examining these results more carefully reveals that the Breusch– Godfrey LM test is significant, again indicating problems of non-stationarity, spurious regression and/or omitted variable bias. 

As explained in Chapter 9, when our variables are non-stationary we should difference them until we have identified a stationary transformation ofour original variable. The unit root tests summarised in Table 10.3 suggest that our consumption and income variables are I(1). In the last chapter we discussed the implications ofusing I(1) variables but in this chapter we introduce the possibility ofcointegration. Cointegration occurs when a linear combination ofnon-stationary variables is stationary. For example, the I(1) variables consumption and income will be cointegrated if a linear combination of them is I(0). With cointegration, OLS estimators exhibit the property of super consistency. This means that as the sample size increases the sampling distribution of the OLS estimators collapses more rapidly onto the true parameter value.<sup>4</sup> 

We test for cointegration by doing a unit test on the residuals from our ARDL: this is called an Engle–Granger test and involves applying the DF/ADF testing methodology to the residuals and the null will be that there is a unit root in the errors. The Engle–Granger test on the model reported in Table 10.5 gives $\hat { \tau } = - 4 . 2 8 0 ( \mathrm { p } = 0 . 0 0 3 )$ and so we can reject the null ofa unit root and conclude that our residuals are stationary. This suggests that logged consumption and logged income are cointegrated. 

Cointegration is important to the construction of error correction models. For our example, the error correction term (ECT) is a linear combination of consumption (logged) and income (logged) because it is constructed as follows: 

$$
E C T _ {t} = \ln \left[ \frac {C _ {t}}{Y _ {y}} \right] = c _ {t} - y _ {t}\tag{10.9}
$$

The unit root tests noted in Table 10.3 indicated that the null of a unit root in ECM could be rejected with a 5% significance level so ECT is I(0) even though $c _ { t }$ and $\gamma _ { t }$ are themselves I(1). So there is some evidence that our consumption and income are cointegrated. We can use the information to construct an error correction model (ECM) as we explain below. 

## Autoregressive distributed lag (ARDL) and error correction models (ECMs)

An error correction model incorporates some assumption about a long-run equilibrium relationship between two variables. The first step in constructing an ECM is to gather some information about the long-run patterns. The evidence outlined above suggests that there is a stable long-run equilibrium relationship between C and $Y ,$ i.e. there is a constant APC. We will use this insight to construct an ECM using the constant APC to capture the long-run equilibrium path. A constant APC implies that (at least in the long-run) the elasticity of C with respect to Y is unitary (i.e. equal to 1). This is what will ensure a constant APC: with a unitary elasticity, a 1% rise in income will be matched by a 1% rise in consumption and so overall APC (the ratio of consumption to income) will remain constant. 

Long-run elasticities can be calculated from autoregressive distributed lag (ARDL) models. Autoregressive (AR) means that the variable is related to past lags of itself; as explained in Box 10.1 a distributed lag (DL) is a lag structure in which the impact of the explanatory variables is distributed over more than one period. An ARDL model combines lags on both the dependent and explanatory variable(s). In the case of consumption functions, this means that a simple ARDL (1,1), i.e. an ARDL with one lag each on the dependent and explanatory variables, will look like this: 

$$
c _ {t} = \alpha + \lambda c _ {t - 1} + \beta_ {1} y _ {t} + \beta_ {2} y _ {t - 1} + \varepsilon_ {t}\tag{10.10}
$$

For an explanation of the relationships between long-run elasticities, ARDLs and ECMs, see Box 10.2. 

## Box 10.2 The link between an ARDL and an ECM

An Error Correction Model (ECM) is a restricted version of an Autoregressive Distributed Lag (ARDL) model incorporating some assumption about a constant long-run relationship between a dependent variable and its explanatory variable(s). In this case we are looking at a very simple sort of ECM incorporating a unitary long-run elasticity (of 1) between income and consumption. (Note that a unitary elasticity does not imply that income and consumption are the same, just that they change in the same way.) 

We can show how the ARDL can be restricted to give an ECM by starting with our ARDL (1,1) specification: 

$$
c _ {t} = a + \lambda c _ {t - 1} + \beta_ {1} y _ {t} + \beta_ {2} y _ {t - 1} + \varepsilon_ {t}\tag{10.10}
$$

Adapting the ECM methodology outlined in Thomas (1997) to derive the restricted ECM version of the ARDL model first we need to ‘re-parameterise’ (10.10) by subtracting $c _ { t - 1 }$ from both sides: 

$$
c _ {t} - c _ {t - 1} = \Delta c _ {t} = a + \beta_ {1} y _ {t} + \beta_ {2} y _ {t - 1} + (\lambda - 1) c _ {t - 1} + \varepsilon_ {t}\tag{10.11}
$$

Then we add and subtract $\beta _ { 1 } y _ { t - 1 }$ from the right-hand side to give: 

$$
\Delta c _ {t} = a + \beta_ {1} \Delta y _ {t} + (\beta_ {1} + \beta_ {2}) y _ {t - 1} + (\lambda - 1) c _ {t - 1} + \varepsilon_ {t}\tag{10.12}
$$

Now that the ARDL has been re-parameterised, we can impose a restriction that the long-run elasticity is equal to one. As we’ve explained above, the stable APC justifies imposing a unitary long-run elasticity on the ARDL because for the APC to remain stable the elasticity of consumption with respect to income must be unitary. We can get an expression for the longrun elasticity by constructing a long-run model in which $c _ { t } = c _ { t - 1 } = c ^ { \star }$ and $y _ { t } = y _ { t - 1 } = y ^ { \star }$ which when incorporated into (10.10) gives: 

$$
c ^ {*} = a + \lambda c ^ {*} + \beta_ {1} y ^ {*} + \beta_ {2} y ^ {*}\tag{10.13}
$$

Rearranging this to collect $c ^ { \star }$ on the righthand side and $y ^ { \star }$ on the left-hand side gives: 

$$
c ^ {*} = \frac {a}{1 - \lambda} + \left[ \frac {\beta_ {1} + \beta_ {2}}{1 - \lambda} \right] y ^ {*}\tag{10.14}
$$

The parameter on $y ^ { \star }$ is the long-run elasticity (LRE) which is equal to: 

$$
L R E = \frac {\beta_ {1} + \beta_ {2}}{(1 - \lambda)}\tag{10.15}
$$

$$
\mathrm{if} L R E = 1, \mathrm{then}
$$

$$
\beta_ {1} + \beta_ {2} = 1 - \lambda\tag{10.16}
$$

If this is true then the parameter on $c _ { t - 1 }$ in (10.12) will be equal but of opposite sign to the parameter on $y _ { t - 1 }$ and so we can restrict our ARDL to give: 

$$
\Delta c _ {t} = a + \beta_ {1} \Delta y _ {t} + (1 - \lambda) y _ {t - 1} + (\lambda - 1) c _ {t - 1} + \varepsilon_ {t}\tag{10.17}
$$

Collecting together $c _ { t - 1 }$ and $y _ { t - 1 }$ whilst remembering that their parameters are equal but opposite sign gives: 

$$
\Delta c _ {t} = a + \beta_ {1} \Delta y _ {t} + (\lambda - 1) [ c _ {t - 1} - y _ {t - 1} ] + \varepsilon_ {t}\tag{10.18}
$$

This is the error correction model (ECM) specification. Note that as the variables are in natural logs so $\Delta c _ { t }$ is the growth rate in consumption and $\Delta y _ { t }$ is the growth rate in income. On the long-run equilibrium path (given $L R E = 1 )$ , consumption and income will rise in proportion and will grow at the same rate. But if the consumption should move above the long-run equilibrium path, then the lagged error correction term $( \mathsf E \mathsf C \mathsf T _ { t - 1 } = \mathsf C _ { t - 1 } - y _ { t - 1 } )$ will be above average and, assuming $( \lambda - 1 ) < 0$ , then growth in consumption will be negatively related to excessive consumption growth in the previous period. In other words, growth in consumption above the long-run equilibrium path (described by a constant APC) will be ‘corrected’ by a fall in consumption growth in the subsequent period; given the negative parameter on the error correction term, consumption growth will fall in the subsequent period. 

Overall, one of the interesting things about ECMs is that they have a clear intuition that fits into the concepts of equilibrium that are so common in economics. We can illustrate this link between long-run equilibrium and short-run disequilibrium dynamics using the consumption example. We’re approximately regressing consumption growth on income growth and whilst these variables are moving in proportion, the economy will be on its long-run equilibrium path of the constant APC. In disequilibrium however, if consumption grows relatively rapidly in comparison with income growth, then the negative effect of the EC term will pull consumption growth down in the next period. On the other hand if consumption is growing too slowly relative to income, then consumption will be below its long-run equilibrium path. Again the negative sign on the ECT parameter will pull growth in consumption in the opposite direction; and in the subsequent period consumption will grow more rapidly. In other words, the system will adjust to errors away from long-run equilibrium. Thus the ECT term captures corrections to consumption in disequilibrium and ensures that consumption and income return to the long-run equilibrium path given by a constant APC. 

In estimating ARDL and ECM models, it is important to conduct Granger Causality tests. Granger causality tests involve establishing whether or not a variable ‘Granger causes another variable; a variable Granger causes another if it ‘leads’ the other variable and F tests of restrictions are used to assess the contribution of lags on one variable to the variability in the other. If lags on $\boldsymbol { \chi } _ { t }$ capture a significant proportion of the variability in $y _ { t }$ then $x _ { t }$ ‘Granger causes’ $y _ { t } ;$ if lags on $y _ { t }$ capture a significant proportion of the variability in $x _ { t }$ then $y _ { t }$ Granger causes $x _ { t } ;$ if a significant proportion of the variability in both variables are captured by lags on the other variable, then they Granger cause each other and this suggests that there may be simultaneity (i.e. feedback effects). If there is no correlation at all between the variables and the lags, then neither variable ‘Granger causes’ the other. Granger causality may mean very little in terms of a real causal link between variables; as emphasised in earlier chapters, in statistical analysis correlation does not imply causation and this is particularly true for regression analysis in economics because people’s expectations complicate the timing of events – for example, Christmas cards do not cause Christmas, they merely ‘Granger cause’ Christmas. 

As explained in Box 10.2, when we impose the restriction of a constant APC and therefore a unitary long-run elasticity of consumption with respect to income, then the unrestricted ARDL model is transformed into a restricted ECM. The EViews output from the estimation of these models is summarised in Table 10.6. 

Note that there is less evidence of a spurious regression in these regressions that in the earlier regressions and, using the Breusch–Godfrey test we can retain the null ofno autocorrelation at a 10% significance level, though we would have to reject this null at 5% (The DW test cannot be used in this case because it is invalidated by the presence of a lagged dependent variable.) The results have improved because, as explained in Chapter 9, spurious regressions are the outcome ofnon-stationary variables and for the ARDL and ECM specifications we have used the following stationary variables: Δc (the first difference in logged consumption – approximately equal to consumption growth), Δy (the first difference in logged income – approximately income growth) and EC (the error correction term). As noted above and shown in Table 10.3 we can reject the $H _ { 0 }$ of a unit root for all these variables at a 5% significance level and so all the variables in our regression are I(0), i.e. are stationary. 

We can also test the statistical merit of the ECM transformation incorporating a long-run elasticity of 1 using an F test of restrictions. As explained in Chapter 5, the intuition underlying these tests is that if the parameters in a model are restricted, then the restricted RSS will increase: if it increases by a small amount then this suggests that the restriction is mirrored in the real 

## Table 10.6a EViews output: ARDL Model

<table><tr><td colspan="5">Dependent Variable: logged consumption (<eq>c_t</eq>)Sample (adjusted): 1980 2005Included observations: 26 after adjustments</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>4.27</td><td>1.58</td><td>2.70</td><td>0.01</td></tr><tr><td>logged consumption lagged <eq>c_{t-1}</eq></td><td>0.74</td><td>0.18</td><td>4.11</td><td>0.00</td></tr><tr><td>logged income (<eq>y_t</eq>)</td><td>0.45</td><td>0.36</td><td>1.25</td><td>0.23</td></tr><tr><td>logged income, lagged (<eq>y_{t-1}</eq>)</td><td>-0.81</td><td>0.25</td><td>-3.24</td><td>0.00</td></tr><tr><td>Time</td><td>0.02</td><td>0.01</td><td>3.12</td><td>0.01</td></tr><tr><td>R-squared</td><td>0.99</td><td>F-statistic</td><td></td><td>1124.22</td></tr><tr><td>Adjusted R-squared</td><td>0.99</td><td>Prob(F-statistic)</td><td></td><td>0.00</td></tr><tr><td>Sum squared residuals</td><td>0.006339</td><td></td><td></td><td></td></tr><tr><td colspan="5">Diagnostic tests</td></tr><tr><td colspan="5">Breusch-Godfrey Serial Correlation LM Test:</td></tr><tr><td></td><td>F-statistic</td><td>2.53</td><td>Probability</td><td>0.08</td></tr><tr><td colspan="5">Ramsey RESET Test:</td></tr><tr><td></td><td>F-statistic</td><td>2.21</td><td>Probability</td><td>0.15</td></tr></table>


Table 10.6b EViews output: error correction model (ECM)


<table><tr><td colspan="5">Dependent Variable: Change in logged consumption (<eq>\Delta c_t</eq>)</td></tr><tr><td colspan="5">Sample (adjusted): 1980 2005</td></tr><tr><td colspan="5">Included observations: 26 after adjustments</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>3.33</td><td>1.81</td><td>1.84</td><td>0.08</td></tr><tr><td>Change in logged income (<eq>\Delta y_t</eq>)</td><td>1.03</td><td>0.36</td><td>2.88</td><td>0.01</td></tr><tr><td>Time</td><td>0.00</td><td>0.00</td><td>1.17</td><td>0.25</td></tr><tr><td>ECT(-1)</td><td>-0.38</td><td>0.21</td><td>-1.84</td><td>0.08</td></tr><tr><td>R-squared</td><td>0.28</td><td>F-statistic</td><td></td><td>2.88</td></tr><tr><td>Adjusted R-squared</td><td>0.18</td><td>Prob(F-statistic)</td><td></td><td>0.06</td></tr><tr><td>Sum squared residuals</td><td>0.009068</td><td></td><td></td><td></td></tr><tr><td colspan="5">Diagnostic tests</td></tr><tr><td colspan="5">Breusch-Godfrey LM Test:</td></tr><tr><td></td><td>F-statistic</td><td>2.49</td><td>Probability</td><td>0.08</td></tr><tr><td colspan="5">Ramsey RESET Test:</td></tr><tr><td></td><td>F-statistic</td><td>0.75</td><td>Probability</td><td>0.40</td></tr></table>

data, we therefore infer that the restriction has empirical support and we do not reject it. However if the RSS increases significantly when we restrict a model, then we infer that the restriction does not fit the data well and so we reject the restriction. Here we will use the F test of restrictions to test the following null: 

$$
\begin{array}{c} H _ {0}: \frac {\beta_ {1} + \beta_ {2}}{(1 - \lambda)} = 1 \\ \therefore \beta_ {1} + \beta_ {2} = 1 - \lambda \end{array}
$$

The ECM is the restricted model (it incorporates the restriction that the longrun elasticity is unitary); the ARDL is the unrestricted model. This gives the following working for the F test of restrictions: 

$$
F (1, 2 1) = \frac {\left(R S S _ {\mathrm{r}} - R S S _ {\mathrm{u}}\right) / d}{\left(R S S _ {\mathrm{u}}\right) / \left(n - k _ {\mathrm{u}} - 1\right)} = \frac {(0 . 0 0 9 0 6 8 - 0 . 0 0 6 3 3 9) / 1}{0 . 0 0 6 3 3 9 / (2 6 - 4 - 1)} = 9. 0 4
$$

At a 5% significance level, $F _ { \mathrm { c r i t } } ( 1 , 2 1 ) = 4 . 3 2$ , and since $F > F _ { \mathrm { c r i t } } ,$ we reject $H _ { 0 }$ and conclude that our results unfortunately do not confirm the ECM incorporating a unitary long-run elasticity. 

Overall, we have outlined some of the mechanics involved in constructing ARDL and ECM specifications of the relationship between consumption and income. We found some evidence that logged consumption and logged income are cointegrated but the imposition ofa unitary long-run elasticity was not justified at a 5% significance level. This is a disappointing finding and may reflect our small sample size so one solution might be to collect more data and hope for more reliable results with a larger sample. Also whilst it is possible that another assumption about the elasticity could generate a more robust ECM, this would not be consistent with the constant APC identified by Kuznets and adopted by Friedman and Modigliani. For the data here, our main evidence about a constant APC came from a visual inspection of our data; graphs and charts cannot give us definitive answers about the precise magnitude of parameters and in this sense the finding from the F test of restrictions is more objective. There are however other ways of testing particular assumptions about long-run elasticities (see Thomas, 1997) and further investigations could focus on uncovering more evidence about the long-run relationship between consumption and income. 

Another issue to keep in mind is that, whilst the diagnostic test results allowed us to retain a null of no autocorrelation in the errors at a 5% significance level, this finding was borderline and the autocorrelation in the residuals may be a sign of omitted variable bias, in which case our OLS estimations will be biased and inconsistent. So further investigations could focus on analysing the influence of other factors apart from income; it is important to remember that consumption will also be affected by other variables, for example by interest rates, liquidity constraints and wealth. 

## 10.5 Implications and conclusions

The policy implications and strategies that stem from the analysis of consumption functions focus on government initiatives to stimulate consumer demand by lowering tax and interest rates, and/or by employing large numbers ofpeople on infrastructure and other public works projects. On these grounds, UK Prime Minister Gordon Brown and US Presidents Kennedy, Clinton and Bush could all be described as Keynesian policy makers even though they are not from the same political party. President Bush’s tax cuts in late 2001 and, in 2008, expansionary policies across the OECD introduced as recession-fighting tools, were – political motivations aside – an attempt to keep households spending their money, in the hope this would prevent the economy from stalling or, worse, free-falling, in the aftermath of numerous financial and political shocks. Also, the low spending in Japanese households from the 1990s onwards had been considered partly to blame for Japan’s failure to lift itself out of economic slump. Unless households buy more, factories cannot increase their produc tion, and the economy cannot grow. Consumption is by far the largest component of aggregate demand in most national economies and policy-makers need to be able to estimate its determinants reasonably accurately in order to predict the likely impact on the economy as a whole. 

## 10.6 Further reading

## Textbooks



Friedman, M. (1957) A Theory ofthe Consumption Function, Princeton: Princeton University Press. 





Griffiths, A. and Wall, S. (1997) Applied Economics, An Introductory Course (7th edition), Harlow: Longman, Chapter 13, pp. 312–17. 





Keynes, J. M. (1936) General Theory ofEmployment, Interest and Money, London: Macmillan. Chapters 8–10. 





Mankiw, G. (2006) Macroeconomics (5th edition), New York: Worth, Chapter 10. 





Thomas, R. L. (1997) Modern Econometrics – An Introduction, Harlow: Addison-Wesley. Chapter 11 (on lag structure); Chapter 15 (on ECMs), Chapter 16 (Granger causality tests). 





Tinbergen, J. (1951) Business Cycles in the United Kingdom, 1870–1914, Amsterdam: North-Holland. 



## Academic articles



Keynes, J. M. (1937) ‘The general theory of employment’, Quarterly Journal of Economics, vol. 51, 209–23. 





Kuznets, S. (1946) National Product Since 1869 (assisted by L. Epstein and E. Zenks), New York: National Bureau of Economic Research, 1946. 





Tinbergen, J. (1942) ‘Does Consumption Lag Behind Incomes?’ Review ofEconomic Statistics, vol. 24, No. 1, 1–8. 



## Policy briefs and newspaper articles

The Economist (2005), ‘How to tame the thrift shift’, 22 September 2005. 

Norman, B., Sebastia-Barriel, M. and Weeden, O. (2002), ‘Equity, wealth and consumption – the experience of Germany, France and Italy in an international context’, Bank ofEngland Quarterly Journal, vol. 42, Spring, 78–85. 

## 10.7 Chapter exercises

1. In this chapter, we have estimated an error correction model (ECM) using logs of consumption and income. Estimate a linear ECM model of consumption following the procedures outlined in this chapter, i.e.: 

(a) Test consumption and income for unit roots and establish the order of integration of these variables; 

(b) Generate an EC variable and use unit root tests to establish its order of integration; 

(c) Estimate the ECM and discuss your results. Does the ECM modelling strategy work when the variables are in levels? 

(d) What are the policy implications of Keynesian consumption theories? 

2. In this chapter we explained the importance of Granger causality tests. Conduct some Granger causality tests on logged consumption and logged income to establish whether these variables Granger cause each other. Discuss the implications of your findings for the estimation of the ARDL and ECM models in this chapter. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/6b9d8b0fed55a08ab00a6412d652333daa34c8c329a3a1724da074426a4216ba.jpg)


# Advanced topics

In this section, we introduce some relatively advanced econometric topics: panel estimation and logit/probit. 

In the previous sections we have treated cross-sectional data and time-series data as separate but it is possible to combine these data sets, either by pooling or via panel estimation. We illustrate these techniques in the chapter on marriage and divorce. 

Until now, we have focussed on linear estimation techniques. With ‘binary dependent variables, we estimate the probability of finding a particular characteristic. Linear estimation techniques may not work well when estimating probabilities. So, in the chapter on war and poverty, we introduce some non-linear techniques for the estimation of probabilities: logit and probit. 

# Panel estimation Divorce and income

Economic issues include: 

 Rational choice theory 

 Economics and happiness 

Econometric issues include: 

 Heterogeneity bias 

 Pooling and panel estimation 

Data issues include: 

 Combining cross-sectional and time-series data 

## 11.1 The issue

Economic analysis is not confined to the study of money and finance. Some economists use their tools for ‘theoretical imperialism’ – i.e. to analyse issues affecting human happiness and welfare that are usually the focus of sociological and/or psychological analysis. How is such an economic approach justified? Economic imperialists take the basic economic principle of balancing benefits and costs and apply it to some of the decisions that people make every day, e.g. choices about drug use, criminal behaviour, decisions to get married and/or divorced etc. The idea is that people engage in certain behaviours, even ostensibly anti-social or destructive behaviours, because the benefits outweigh the costs. This is the essence of the rational choice theory made famous by Gary Becker. 

Other economists have also used economic tools to illuminate social issues and problems. In this chapter we illustrate how economics and econometrics can be used to illuminate an area offamily life that has been the focus of many analyses by economists: marriage and divorce. In this chapter, we focus on divorce data from 45 US states over the period 2002–4 so our data set has both a spatial/geographical dimension and a temporal dimension. When cross-sectional and time-series data are combined, particular techniques may be needed and in this chapter we illustrate panel estimation techniques – techniques designed simultaneously to capture both a spatial dimension and a temporal dimension. 

## 11.2 The theory

Gary Becker popularised (and won the Nobel prize) for rational choice theory – an approach that applies economic principles to a wide range of social and psychological behaviours. Becker asserts that we are economisers not only when it comes to incomes and money but in other areas of our lives too. So economic theory can be helpful in understanding relationship decisions as well as financial and economic decisions. 

In A Treatise on the Family (1991), Becker applies rational choice principles to family life asserting that decisions about marriage and divorce reflect a rational, maximising approach to life. People marry and divorce when they perceive that the overall benefits from entering into or breaking the marriage contract outweigh the costs. 

Some economists confront these rational choice principles in arguing that people are not maximisers: anti-social and self-destructive behaviours may be the product of a complex range of motivations, including behaviours that are associated with irrational and/or ill-informed decision-making. For example, Daniel Kahneman (another Nobel laureate) and Amos Tversky approached socio-economic problems from the opposite direction: they argued that the psychological underpinnings of people’s life experiences are as important as an economic analysis of the benefits and costs and their ideas triggered the development of hedonic psychology, as outlined in Box 11.1. 

Rowthorn (1999) analyses marital decisions using a hybrid approach. He uses economic principles to draw parallels between economic investments and relationship-specific investments (such as marriage) requiring mutual levels of trust, describing marriage as a joint project in which the two partners pool and share resources and assets: marriage has an important economic dimension. But Rowthorn, captures some of the insights of the hedonic psychologists when he observes that contagion effects will operate – attitudes and expectations will influence the likelihood ofdivorce. So it is not only about benefits and costs; it is also about social and psychological factors too. 

## Box 11.1 Economics and happiness

Kahneman and Tversky (1979) introduced psychological factors into modern economic analysis via prospect theory. Prospect theory is not based on strict assumptions of rational and consistent behaviour. Instead it assumes that people operating in a risky world will assess the likely prospects of a range of different behaviours. Rather than balancing benefits and costs in a symmetric and systematic way, people will prefer avoiding losses to making gains, and happiness will be affected by changing situations not the status quo. 

Tversky and Kahneman (1986) also argue that people are not necessarily very good at judging the probabilities of various events and will often misjudge future prospects, with statistical errors emerging because of cognitive biases such as anchoring effects and framing effects. Anchoring effects operate when people’s decisions and choices reflect what they have experienced already: if they are happy with a given situation then they will anchor their expectations of the future to what they are currently experiencing. Framing effects focus on the psychological context of people’s reported perceptions of personal issues: when researchers asked students two questions: “Are you happy?” “Did you have a date last night?” the students’ answers were affected both by which question is asked first and by how things had gone the night before. For a good introduction to some of the main findings from this research into prospect theory and other research into aspects of behavioural economics see Lunn (2008). 

Kahneman and Tversky’s research propelled a whole new approach to economics – hedonic psychology – the psychology of well-being.<sup>1</sup> In one sense hedonic psychology is a modern development of utilitarianism – a moral doctrine, associated with the English economist and philosopher Jeremy Bentham, asserting that actions should be assessed according to their impact on utility i.e. on pleasure, satisfaction and happiness. The hedonic psychologists argue that we are not necessarily strictly rational in our decision-making and our subjective judgements of our own satisfaction, e.g. in the context of decisions such as to marry or divorce, may not necessarily tie in with monetary measures. So economics should be extended to analyse not only monetary measures of utility but also measures of experienced happiness: our own experiences of psychological well-being are as important as monetary measures of benefits and costs. Because the hedonic psychologists focus on experienced happiness, their empirical analyses tend to concentrate on survey data and related reports of individuals’ reported levels of happiness. 

These ideas are applied to the assessment of marriage and divorce by focussing on the insight that it is change that affects people’s perceptions of their own welfare. People will judge their own happiness against a benchmark of what they’ve experienced in the past. For married couples, their experience of marriage and divorce is determined by the recent past. 

Happiness peaks at the point of marriage but falls rapidly until after (on average) two years of marriage it stabilises at a level equivalent (and sometimes below) pre-marital happiness levels (Layard 2005). Stutzer and Frey (2006) develop these ideas analysing marriage using German survey evidence: their analysis suggests that happy singles are more likely to select into marriage and unhappy people are likely to self-select into divorce. These findings remain preliminary because most economists have only recently developed an interest in analysing social and psychological issues; the evidence is relatively sparse. But a large volume of research is in progress from which we can anticipate fascinating new insights. 

Economists have also analysed broader issues relating to marriage and divorce. Wilson and Oswald (2005) analyse the relationships between marriage and health (both physical and psychological) identifying health gains from being married. Edland (2005) focusses on the impact ofmarital decisions on labour mobility and migration and hypothesises that females will move to urban areas because they are attracted by the higher incomes of the richer urban men. Gautier, Svarer and Teulings (2005) assert that singles are more likely to pay higher property prices in cities because of better marriage markets in cities. 

In this chapter we will build on Rowthorn’s idea that marriage is a joint economic contract by exploring the relationship between divorce and economic conditions. We assume that when disposable incomes are relatively low, people will experience financial pressures and these will increase the economic and psychological costs of partnership thereby increasing the likelihood of divorce. Hypotheses about a negative association between income and divorce are emerging in the academic literature and in the mainstream press – for example Burgess, Propper and Aassve (2003) examine the relationships between income and divorce finding negative correlations for men; and The Economist has highlighted debates about the impact of recessions on divorce (The Economist, 2008). In this chapter we investigate these assertions by analysing the associations between divorce rates and personal income across the different states of the USA over the period 2002–2004. 

## 11.3 Data

The theoretical hypothesis outlined in Section 11.2 is that macroeconomic conditions affect divorce rates and we assess this hypothesis using divorce 


statistics for 45 US states over the period 2002 to 2004. Our data comes from the following sources:


<table><tr><td>Variable</td><td>Source</td><td>Website</td></tr><tr><td>Divorce rate per 1000 inhabitants, by state</td><td>US National Center for Health Statistics (NCHS)</td><td>www.cdc.gov/nchs/data/nvss/divorce90_04.pdf</td></tr><tr><td>Personal disposable income per capita, by state</td><td>US Bureau of Economic Analysis (BEA)</td><td>www.bea.gov/regional/spi/drill.cfm</td></tr></table>

The divorce rate is measured using data on the divorces from household health surveys conducted and analysed by the NCHS. Income is measured as average annual personal disposable income (PDI) per capita by state, collected from the BEA’s regional income and product accounts. 

In assessing our data, the key limitations will be that PDI does not completely capture the full range of macroeconomic conditions affecting marital pressures – for example mortgage and housing markets are likely to have an impact on the stability of relationships particularly if the family home is threatened by repossession. Also, our data is focussing closely on macroeconomic factors and this abstracts from the social and psychological pressures on family life. 

Given these caveats, we show a scatter plot of divorce rates and PDI in Figure 11.1. This preliminary assessment of the data reveals that there is a negative association between divorce rates and personal income, confirming our hypothesis that difficult economic conditions are associated with higher divorce rates, though there is also a lot of variability across the data set. 

## 11.4 Empirical methods and results

In exploring the relationship between incomes and divorce across the US states more thoroughly, we will estimate the following model: 

$$
d _ {i, t} = \alpha + \beta y _ {i, t} + u _ {i, t}\tag{11.1}
$$

d is the divorce rate and y is PDI per capita. Note that we have two subscripts on each variable. This is because we have two dimensions to our data set: we have data for i individual states (45 states in the sample) over t different time periods (3 years in this analysis). The intercept term is included to capture all the constant factors that might affect the divorce rate, for example social conventions and attitudes. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/9a0b2709afd9ce443507599e48a85e12389f31cb76a1fbd2d3de343cad89be92.jpg)



Figure 11.1 Scatter plot of divorce rates vs. personal income, USA 2002–4


There are two econometric approaches to combining cross-sectional and time-series observations: pooling and panel estimation. 

## Pooled estimation

Pooling is the simple combining of cross-sectional and time-series data without adjustment. A pooled regression would be a regression on our 135 pairs of observations (45 states × 3 years) without making any allowance for factors specific to each individual state. If we were to look at just one year of data, we’d have just 45 observations but with 3 years of data we have 135 observations. This may increase the accuracy of our estimation because if we have a problem of micronumerosity (which, as explained in Chapter 5, is the technical term to describe a sample with few degrees of freedom, i.e. a sample in which the number of observations is small relative to the number of parameters to be estimated) then OLS estimates will not be so precise. The standard errors on the OLS parameter estimates will be larger and confidence intervals will be wider. 

For some samples ofdata it may be appropriate just to pool the observations in this simple way. If the samples are randomly selected from each point in time, then there will be no systematic cross-sectional specific effects to affect the parameter estimates – for example, if we were taking three different random samples of 1000 households three times across three years from a population of 30 million households, then it is very unlikely that the same households would be selected more than once; the households sampled in each year would be different and so household-specific effects are unlikely to be important. In this case simple pooling will be valid. 


Table 11.1 EViews output from the pooled estimation


<table><tr><td colspan="5">Dependent Variable: Divorce rateMethod: Least SquaresSample: 1 135</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>7.055</td><td>0.445</td><td>15.854</td><td>0.000</td></tr><tr><td>PDI per capita</td><td>-0.099</td><td>0.014</td><td>-7.004</td><td>0.000</td></tr><tr><td>R-squared</td><td>0.269</td><td></td><td></td><td></td></tr><tr><td>Adjusted R-squared</td><td colspan="3">0.264 Prob(F-statistic)</td><td>0.000</td></tr><tr><td>Sum squared residuals</td><td>94.061</td><td></td><td></td><td></td></tr><tr><td>Durbin-Watson statistic</td><td>0.536</td><td></td><td></td><td></td></tr><tr><td colspan="5">Breusch-Godfrey Serial Correlation LM Test:</td></tr><tr><td>F-statistic</td><td>77.393</td><td>Probability</td><td></td><td>0.000</td></tr></table>

We run a simple pooling regression on our data set and the results are shown in Table 11.1. 

These results do capture a strong association between divorce rates and PDI: for a t test of the null that the parameter on logged income is equal to zero, we can reject the null at a 5% significance level $\left( p < 0 . 0 5 \right)$ . The $R ^ { 2 }$ indicates that variability in PDI captures 26.9% of the variability in divorce rates and the F test of explanatory power confirms that the overall goodness of fit is relatively high. 

However, looking at the results more carefully there are signs that OLS may not be working well because Gauss–Markov assumptions are violated. For example the DW statistic is low and close to zero suggesting that autocorrelation may be a problem and this is confirmed by the results from the BG test – which indicates that the null of no autocorrelation must be rejected even at very low significance levels. 

So what is happening with this data set? The autocorrelation problem may be emerging because in our data set we have ordered our data set so that the three years of data for each state follow from each other. We might expect that each state is affected by some factors that are constant but specific to an individual state, but do not affect the other states. These state-specific constant factors will not vary over time and the BG and DW tests are picking up the correlations between these state-specific constant factors over the three consecutive years of data for each state. 

This illustrates the essential problem of a simple pooling procedure: pooling is only valid ifall the parameters ofthe model are constant across space. So a simple pooling of our data procedure is unlikely to be valid for our sample because we have some fixed effects i.e. state-specific effects which are time invariant but unobservable. Unless we control for these fixed effects we will generate biases in our estimation and to show how these biases are created when we ignore regionspecific fixed effects we start with our empirical model from (11.1): 

$$
d _ {i, t} = \alpha + \beta y _ {i, t} + u _ {i, t}\tag{11.1}
$$

We extend this model by including a deterministic time trend (T) as follows: 

$$
d _ {i, t} = \alpha + \beta y _ {i, t} + \phi T _ {t} + u _ {i, t}\tag{11.2}
$$

(This time trend is constant across the states hence there is no subscript i.) If we ignore the state-specific fixed effects then these will be left in the error term as follows: 

$$
u _ {i, t} = a _ {i} + \varepsilon_ {i, t}\tag{11.3}
$$

where $a _ { i }$ is the fixed effect specific to each state i. 

Putting (11.2) and (11.3) together we have: 

$$
d _ {i, t} = \alpha + \beta y _ {i, t} + \phi T _ {t} + (a _ {i} + \varepsilon_ {i, t})\tag{11.4}
$$

The problem with this model is that the state-specific effects have been left in the error term of the model even though they may be exerting a systematic influence on the divorce rate; the error term is meant to capture truly random factors. To illustrate what is happening by linking into some of the theoretical ideas outlined above: if Rowthorn’s contagion effects are operating, then variations in attitudes and expectations across the states may mean that divorce is regarded as being more socially acceptable in some states than others and the $a _ { i }$ for each individual state will capture these (and other) differences across the states. But if $a _ { i }$ is left in the error then the deterministic part of the model won’t properly capture all systematic influences. 

If these fixed effects are ignored then this generates heterogeneity bias. Heterogeneity bias occurs because the time invariant fixed effects influencing individual cross-sectional units have have been left out of the deterministic part of the model so in essence heterogeneity bias is a form of omitted variable bias. As explained in Chapter 8, omitted variable bias is a potentially serious type of model misspecification. At the least it will generate autocorrelated errors, again because an important systematic influence has been left out of the deterministic part of the empirical model and is being captured in the error term. For our analysis, heterogeneity bias explains our significant DW and BG tests. More seriously, if there is a correlation between the state-specific effects $a _ { i }$ and the explanatory variable(s) then heterogeneity bias will create the problem of endogeneity (also introduced in Chapter 8), i.e. the explanatory variable and error will be correlated and OLS estimators will be biased and inconsistent. So simple pooling in the presence of heterogeneity bias is likely severely to compromise the efficiency of OLS estimation. 

## Panel estimation

In the presence of cross-section specific fixed effects, before drawing any firm conclusions from our estimations it will be important either to capture or to remove the fixed effects and thus eliminate potential heterogeneity bias. One solution to heterogeneity bias is to use panel estimation techniques. These allow us to combine the advantages of pooling as outlined above (i.e. efficiency gains from reducing micronumerosity) with techniques to control for heterogeneity bias. 

We outline two ways of removing time constant cross-section specific effects – the difference estimator and fixed effects estimation. A further method, the random effects estimator model, is beyond the scope of this book but see Wooldridge (2003) for a detailed explanation. 

## The difference estimator

The difference estimator eliminates the heterogeneity bias by differencing it away over time as follows. Starting with (Equation (11.4)): 

$$
d _ {i, t} = \alpha + \beta y _ {i, t} + \phi T _ {t} + (a _ {i} + \varepsilon_ {i, t})\tag{11.4}
$$

Lag (11.4) by one time period to give: 

$$
d _ {i, t - 1} = \alpha + \beta y _ {i, t - 1} + \phi T _ {t - 1} + (a _ {i} + \varepsilon_ {i, t - 1})\tag{11.5}
$$

Then subtract (11.5) from (11.4) Remembering that $\Delta T _ { t } = 1$ , $a _ { i }$ is constant over time and so $\Delta a _ { i } = 0$ , this gives: 

$$
\Delta d _ {i, t} = \beta \Delta y _ {i, t} + \phi + \Delta \varepsilon_ {i, t}\tag{11.6}
$$

The $a _ { i }$ has been differenced away and subtracted out, removing the potential source of heterogeneity bias. Note that the parameter $\phi$ has become our new intercept in the differenced model because $\Delta T _ { t } = 1$ 

The difference estimator has removed the heterogeneity bias but suffers from the following limitations: 

– we may want to retain levels information in our model e.g. if we are more interested in the levels variables rather than changes; 

– by differencing our explanatory variables we reduce their variability, we will not have such a strong source of explained variance and this lower ‘explanatory’ power will be associated with a lower $R ^ { 2 }$ ; 

– by differencing our model we lose degrees of freedom and the accuracy of our estimation will decline accordingly; 

– in differencing the error term we may create problems with our errors, e.g in Equation (11.6) our error is a moving average $( \Delta \varepsilon _ { i , t } = \varepsilon _ { i , t } - \varepsilon _ { i , t - 1 } )$ i.e. it is an average of successive values of $\varepsilon _ { i \cdot }$ . 

## The fixed effects estimator

Another approach to dealing with cross-section specific effects in panel estimation is to use the fixed effects estimator, which involves a within transformation: i.e. the observations within each cross-sectional subgroup are demeaned to remove the unobservable fixed effects (see also Wooldridge 2003). To illustrate these concepts, demeaning involves subtracting the mean for each subgroup from each observation in that subgroup. For our chapter example, ifwe want to demean the Florida observations on d and $y ,$ then we subtract the mean for Florida over the period 2002–4 from each of the Florida observations. 

We can show how and why the demeaning procedure works by starting again with Equations (11.1) and (11.3): 

$$
d _ {i, t} = \alpha + \beta y _ {i, t} + (a _ {i} + \varepsilon_ {i, t})\tag{11.1}
$$

$$
u _ {i, t} = a _ {i} + \varepsilon_ {i, t}\tag{11.3}
$$

Taking the mean for d for each subgroup i gives 

$$
\bar {d} _ {i} = \bar {\alpha} + \beta \bar {y} _ {i} + \bar {a} _ {i} + E (\varepsilon_ {i})\tag{11.7}
$$

Demeaning involves subtracting this subgroup mean from each observation to give: 

$$
d _ {i, t} - \bar {d} _ {i} = (\alpha - \bar {\alpha}) + \beta (y _ {i, t} - \bar {y} _ {i}) + (a _ {i} - \bar {a} _ {i}) + \varepsilon_ {i, t} - E (\varepsilon_ {i})\tag{11.8}
$$

This can be simplified because the mean of a constant is just that constant and the mean of the error is zero i.e. $\bar { a } _ { i } = a _ { i } , \bar { \alpha } = \alpha$ and $E ( \varepsilon _ { i } ) = 0$ giving: 

$$
\left(d _ {i, t} - \bar {d} _ {i}\right) = \beta \left(y _ {i, t} - \bar {y} _ {i}\right) + \varepsilon_ {i, t}\tag{11.9}
$$

In this way, the fixed effects have been demeaned away. 

A directly equivalent procedure to demeaning is to use dummy variables to control for the cross-section specific fixed effects. A dummy variable can be used to bring the $a _ { i }$ out of the error $( u _ { i , t } )$ into the parameter estimate on the dummy variable. If we create a dummy variable $D _ { i }$ for each cross-sectional unit i, then we have: 

$$
d _ {i, t} = \alpha + \beta y _ {i, t} + \sum_ {i = 1} ^ {4 4} a _ {i} D _ {i} + \varepsilon_ {i, t}\tag{11.10}
$$

To illustrate – we create a dummy variable for Florida called $D _ { \mathrm { F l o r i d a } } ,$ which is equal to one for the three years of Florida data and equal to zero for all observations referring to other states. When $D _ { \mathrm { F l o r i d a } } = 1$ all the other $D _ { i } s$ are zero, we have the following: 

$$
\begin{array}{r l} d _ {\text { Florida }, t} & = \alpha + \beta y _ {\text { Florida }, t} + a _ {\text { Florida }} D _ {\text { Florida }} + \varepsilon_ {\text { Florida }, t} \\ & = (\alpha + a _ {\text { Florida }}) + \beta y _ {\text { Florida }, t} + \varepsilon_ {\text { Florida }, t} \end{array}\tag{11.11}
$$

In this way, the parameter on each dummy variable will pick up the $a _ { i }$ for each cross-section – e.g. the parameter on Florida’s dummy has shifted the intercept to capture the cross-sectional fixed effects that apply only to Florida. This gives the same result as demeaning. 

For our data set we create similar dummy variables for all the 45 states in our sample and include all the state-specific dummies in our model to capture state-specific effects. We use Alabama as the reference category i.e. Alabama is the state to which the conventional intercept refers. 

Alternatively we could have dropped the intercept because the dummy variables will be capturing all the constant factors for each state but dropping the intercept complicates interpretation of adjusted $R ^ { 2 }$ . We couldn’t do both (i.e. include the Alabama dummy as well as the conventional intercept) because this would create perfect multicollinearity and we’d be in a dummy variable trap (as explained in Chapter 5). 

The fixed effects estimation with dummy variables is reported in Table 11.2. 

This estimation procedure has worked relatively well; the $R ^ { 2 }$ is high and the F test of explanatory power allows rejection ofthe null that the parameters on the explanatory variables are jointly equal to zero even at low significance levels. 

In testing for individual significance, the parameter on PDI is still significantly different from zero even at low significance levels. The t tests on the parameters on the state dummies are, at 10% significance levels and lower, significantly different from zero for all states except Colorado, Connecticut, Florida, Idaho, Kentucky, Tennessee and Washington State. However, the significance of the parameters on the fixed effects dummies for Florida, Connecticut and Kentucky is borderline – these parameters are significantly different from zero at significance levels just about 10%. An F test of joint restrictions for the remaining four states with fixed effects parameters more clearly insignificantly different from zero confirms the t test results: the null that the parameters on the dummy variables for those four states are equal to zero is not rejected even at high significance levels $- \ F ( 4 , 8 8 ) = 0 . 1 9 5 \ [ p = 0 . 9 4 1 ]$ 


<sub>V</sub>i<sub>ews</sub> <sub>output</sub> <sub>from</sub> <sub>f</sub>i<sub>xed</sub> <sub>ef</sub>f<sup>ects</sup> <sup>est</sup>i<sup>mat</sup>i<sup>on</sup> <sup>us</sup>i<sup>ng</sup> <sup>dum</sup>


<table><tr><td colspan="10">Dependent Variable: DIVORCEMethod: Least SquaresSample: 1 135</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td><td></td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>7.675</td><td>0.310</td><td>24.767</td><td>0.000</td><td></td><td></td><td></td><td></td><td></td></tr><tr><td>PDI per capita</td><td>-0.094</td><td>0.011</td><td>-8.392</td><td>0.000</td><td></td><td></td><td></td><td></td><td></td></tr><tr><td>Dummy variables</td><td></td><td></td><td></td><td></td><td>Dummy variables</td><td></td><td></td><td></td><td></td></tr><tr><td>Alaska</td><td>-0.308</td><td>0.135</td><td>-2.273</td><td>0.025</td><td>Nevada</td><td>2.305</td><td>0.132</td><td>17.453</td><td>0.000</td></tr><tr><td>Arizona</td><td>-0.827</td><td>0.116</td><td>-7.141</td><td>0.000</td><td>New Hampshire</td><td>-0.272</td><td>0.149</td><td>-1.823</td><td>0.072</td></tr><tr><td>Arkansas</td><td>0.738</td><td>0.118</td><td>6.262</td><td>0.000</td><td>New Jersey</td><td>-0.670</td><td>0.193</td><td>-3.476</td><td>0.001</td></tr><tr><td>Colorado</td><td>0.009</td><td>0.145</td><td>0.063</td><td>0.950</td><td>New Mexico</td><td>-0.567</td><td>0.117</td><td>-4.867</td><td>0.000</td></tr><tr><td>Connecticut</td><td>-0.353</td><td>0.224</td><td>-1.575</td><td>0.119</td><td>New York</td><td>-1.021</td><td>0.161</td><td>-6.325</td><td>0.000</td></tr><tr><td>Delaware</td><td>-0.771</td><td>0.142</td><td>-5.424</td><td>0.000</td><td>North Carolina</td><td>-0.711</td><td>0.117</td><td>-6.085</td><td>0.000</td></tr><tr><td>District of Columbia</td><td>-1.095</td><td>0.258</td><td>-4.243</td><td>0.000</td><td>North Dakota</td><td>-2.023</td><td>0.117</td><td>-17.337</td><td>0.000</td></tr><tr><td>Florida</td><td>0.203</td><td>0.125</td><td>1.626</td><td>0.108</td><td>Ohio</td><td>-1.088</td><td>0.121</td><td>-8.974</td><td>0.000</td></tr><tr><td>Idaho</td><td>-0.054</td><td>0.116</td><td>-0.471</td><td>0.639</td><td>Oregon</td><td>-0.542</td><td>0.121</td><td>-4.494</td><td>0.000</td></tr><tr><td>Illinois</td><td>-1.743</td><td>0.142</td><td>-12.296</td><td>0.000</td><td>Pennsylvania</td><td>-1.575</td><td>0.131</td><td>-12.002</td><td>0.000</td></tr><tr><td>Iowa</td><td>-2.029</td><td>0.119</td><td>-17.074</td><td>0.000</td><td>Rhode Island</td><td>-1.479</td><td>0.135</td><td>-10.954</td><td>0.000</td></tr><tr><td>Kansas</td><td>-1.454</td><td>0.121</td><td>-11.991</td><td>0.000</td><td>South Carolina</td><td>-1.917</td><td>0.116</td><td>-16.583</td><td>0.000</td></tr><tr><td>Kentucky</td><td>-0.183</td><td>0.116</td><td>-1.582</td><td>0.117</td><td>South Dakota</td><td>-1.807</td><td>0.119</td><td>-15.246</td><td>0.000</td></tr><tr><td>Maine</td><td>-0.515</td><td>0.118</td><td>-4.354</td><td>0.000</td><td>Tennessee</td><td>0.003</td><td>0.117</td><td>0.024</td><td>0.981</td></tr><tr><td>Maryland</td><td>-0.833</td><td>0.172</td><td>-4.852</td><td>0.000</td><td>Texas</td><td>-1.106</td><td>0.121</td><td>-9.171</td><td>0.000</td></tr><tr><td>Massachusetts</td><td>-1.512</td><td>0.189</td><td>-8.008</td><td>0.000</td><td>Utah</td><td>-1.218</td><td>0.116</td><td>-10.475</td><td>0.000</td></tr><tr><td>Michigan</td><td>-1.190</td><td>0.125</td><td>-9.496</td><td>0.000</td><td>Vermont</td><td>-0.763</td><td>0.124</td><td>-6.176</td><td>0.000</td></tr><tr><td>Minnesota</td><td>-1.449</td><td>0.146</td><td>-9.920</td><td>0.000</td><td>Virginia</td><td>-0.409</td><td>0.144</td><td>-2.842</td><td>0.006</td></tr><tr><td>Mississippi</td><td>-0.821</td><td>0.122</td><td>-6.748</td><td>0.000</td><td>Washington</td><td>-0.068</td><td>0.140</td><td>-0.482</td><td>0.631</td></tr><tr><td>Missouri</td><td>-1.017</td><td>0.119</td><td>-8.536</td><td>0.000</td><td>West Virginia</td><td>-0.227</td><td>0.118</td><td>-1.925</td><td>0.058</td></tr><tr><td>Montana</td><td>-1.284</td><td>0.115</td><td>-11.124</td><td>0.000</td><td>Wisconsin</td><td>-1.672</td><td>0.125</td><td>-13.415</td><td>0.000</td></tr><tr><td>Nebraska</td><td>-1.325</td><td>0.124</td><td>-10.708</td><td>0.000</td><td>Wyoming</td><td>0.777</td><td>0.136</td><td>5.695</td><td>0.000</td></tr><tr><td>R-squared</td><td>0.986</td><td colspan="3">Sum squared residuals</td><td>1.779</td><td></td><td>F-statistic</td><td></td><td>141.162</td></tr><tr><td>Adjusted R-squared</td><td>0.979</td><td colspan="3">Durbin-Watson statistic</td><td>2.871</td><td></td><td>Prob(F-statistic)</td><td></td><td>0.000</td></tr></table>

For the 41 remaining states, the statistical significance of the state-specific fixed effects suggests that divorce rates are affected by factors specific to each state as well as by PDI. Some state-specific factors that might be captured by these fixed effect dummies include financial constraints, mortgage defaults and repossessions, unemployment (assuming that it is relatively constant over short time spans) and possibly a number of non-economic factors, such as psychological health and social factors. 

## 11.5 Implications and conclusions

In terms of econometric techniques, this chapter has shown that econometric results can be affected profoundly by whether or not the correct techniques have been used. For example, as illustrated in this chapter, a naïve pooling of the data on divorce rates and PDI may generate misleading conclusions and panel estimation techniques will more efficiently control for time invariant fixed effects. 

If our empirical findings about the negative association between divorce and PDI across the US states between 2001 and 2004 are robust, then this suggests that government policies to improve economic performance may have some positive social effects in moderating family breakdown. However, the fact that cross-section specific fixed effects are also significant suggests, unsurprisingly, that other factors are important. Other economic factors such as financial instability and unemployment will affect divorce rates too, but whilst economic factors may have some impact on social phenomena such as divorce, psychological characteristics, social attitudes and expectations will play a central role. In the future, interdisciplinary research involving not only appropriate econometric techniques but also more suitable, disaggregated sources of data (e.g. survey data used to capture the likelihood of divorce at a household level) may more effectively capture the complex effects of economic, social and psychological factors on divorce rates. 

## 11.6 Further reading

## Books



Becker, G. (1991) A Treatise on the Family, Cambridge MA: Harvard University Press. 





Kahneman, D., Diener, E. and Schwarz, N. (2003) Well-Being: Foundations ofHedonic Psychology, New York: Russell Sage Foundation. 





Layard, R. (2005) Happiness: Lessons from a New Science, London: Allen Lane/Penguin. 





Lunn, P. (2008) Basic Instincts: Human Nature and the New Economics, London: Marshall Cavendish Business. 





Wooldridge, J. M. (2003) Introductory Econometrics – A Modern Approach (2nd edition), Thomson South-Western, Chapters 7 and 14. 



## Academic articles and working papers



Burgess, S., Propper, C. and Aassve, A. (2003) ‘The role of income in marriage and divorce transitions among young Americans’, Population Economics, vol. 16, no. 3, 455–75. 





Edlund L. (2005) ‘Sex and the City’, Scandinavian Journal of Economics, vol. 107, no. 1, 25–44. 





Gautier, P. A., Svarer, M. and Teulings, C. N. (2005) ‘Marriage and the City’, CEPR Discussion Paper No. 4939, Centre for Economic Policy Research, London. 





Kahneman, D. and Tversky, A. (1979) ‘Prospect theory – an analysis of decision under risk’, Econometrica, vol. 47, no. 2, 263–92. 





Rowthorn, R. (1999) ‘Marriage and trust: some lessons from economics’, Cambridge Journal of Economics, vol. 23, no. 5, 661–91. 





Stutzer, A. and Frey, B. S. (2006) ‘Does marriage make people happy, or do happy people get married?’ Journal ofSocio-Economics, vol. 35, no. 2, 326–47. 





Tversky, A. and Kahneman, D. (1986) ‘Rational choice and the framing ofdecisions’, Journal of Business, vol. 59, no. 4, 251–78. 





Wilson, C. M. and Oswald, A. J. (2005) ‘How does marriage affect physical and psychological health, a survey of longitudinal evidence’, Institute for the Study of Labour Discussion Paper, IZA Discussion Paper No. 1619. 



## Newspaper articles

The Economist (2008) ‘Divorce and economic growth: negatively correlated’, 24 July 2008. 

## 11.7 Chapter exercises

1. Using the data sources outlined in Section 11.3, use the difference estimator to analyse the relationship between the divorce rate and personal disposable income per capita across the US states. Interpret your findings. How do your results differ from the results reported in this chapter? 

2. Using the data sources outlined in Section 11.3, perform a ‘within transformation’ by subtracting the relevant cross-sectional means away from each observation (e.g. for the Florida observations, subtract the Florida mean). Confirm that this demeaning procedure gives the same result as for fixed effects estimation. 

# Binary dependent variables War and poverty

Economic issues include: 

 Conflict and inequality 

 Institutions and development 

Econometric issues include: 

 Binary dependent variable estimation 

 Logit and probit 

Data issues include: 

 The Gini coefficient 

## 12.1 The issue

Poverty and armed conflict are the norm for a large proportion of the world’s poor. In moderating the socio-economic impacts of these conflicts, the military as an institution plays a complex role. It may bestow some benefits in countries with institutions that are otherwise underdeveloped and perhaps it is not surprising that a well-organised and powerful public institution, when engaged in peaceful activity, should have positive impacts in countries with otherwise underdeveloped institutions. A lot ofempirical work has been done, following Benoit (1978), to show that defence spending necessitated by real or potential armed conflicts encourages the development of human skills and essential infrastructure within poor economies, thus alleviating poverty. Benoit’s study led to a range of further studies, some of which questioned Benoit’s methodology and findings, and others which investigated the relationship between defence and economic growth using different methodologies.<sup>1</sup> 

Whilst the military as an institution may have a positive impact in peacetime, what about the direct impacts of war and conflict? What are its causes and consequences? In this chapter we will start to illuminate these questions by assessing evidence about the relationship between the incidence of war and relative poverty. To do this we will estimate the probability of conflict in a binary response model i.e. in a model in which the dependent variable takes one of two discrete values: 0 or 1. OLS estimation is not the most effective estimation method for binary response models and special binary estimation techniques are usually needed. In this chapter, we will introduce some relatively simple binary estimation techniques: Logit and Probit. 

## 12.2 The theory

Given the destruction of life and resources that accompanies violent conflict, why would a government want to go to war? Analyses of the political and strategic motivations affecting governments’ decisions to engage in armed conflict (or not) have been analysed by Nobel laureate Thomas Schelling (1958, 1960) using game theory concepts, as is explained in Box 12.1 

In this chapter we will focus on one of the explanations for civil war – the political control of social unrest amongst poorer groups, and we will analyse the probability of war using poverty as an explanatory variable. 

In assessing the specific impact of poverty and inequality on the probability of war, a range of issues must be considered. Many armed conflicts are the product of local socio-economic conditions rather than territorial motivations. Poverty and discrimination can be particularly prevalent in dual economies: economies characterised by a sharp divide between a globalised, industrialised urban sector and a poorer, more traditional, rural sector. In dual economies, political and economic leaders may have incentives to protect their economic and financial interests using violent techniques, increasing susceptibility to civil war. This hypothesis forms the basis of greed and grievance theory. In greed and grievance theory poverty and underdevelopment contribute to social unrest, generating feelings of political insecurity amongst the local elite groups. Rich elites have an incentive to use violent methods to protect their political and economic interests and so respond by increasing security expenditure on both the police and defence forces thus fostering the conditions for armed conflict. So according to the greed and grievance theorists, the probability of conflict is positively 

## Box 12.1 Game theory and the strategy of conflict

In The Strategy ofConflict (1960), Thomas Schelling uses game theory concepts to analyse military strategies (see also Schelling, 1958). As explained in Chapter 7, game theory is used to examine the bargaining behaviour of a small number of players devising their own strategies based on the potential strategies of the other players. Schelling argues that conflict situations can often be described as strategic bargaining situations: countries are concerned not so much with the application of force as with the exploitation of potentia force. For example, during the Cold War, the US and USSR accumulated arms including nuclear weapons to prevent not encourage conflict. So it could be argued that the Arms Race was about deterrence not conflict. Schelling uses these ideas to devise the concept of limited war, i.e. strategic manoeuvres that can stabilise conflicts without resulting in actua armed engagement. Limited war will result in wasteful expenditures: nations will accumulate weapons just because they expect other countries to do so, generating a spiralling of armament accumulation, yet these weapons are accumulated in the hope that they will never be used. War breaks out when the strategies fail so actual conflict emerges from failed bargains. These ideas have been extended more recently, e.g. by Jackson and Morelli (2005), who argue that asymmetric information and political bias (i.e. bias away from democracy) increase the probability that peace bargains fail. 

In this chapter we are concentrating on a specific type of armed conflict, i.e. civil war in developing countries. In this situation military strategies are moulded by a different set of goals and constraints, partly reflecting the fact that civil wars are not often games played between two equally powerful players. Nonetheless the concepts of game theory can still be applied and the strategy of deterrence can be a useful one for incumbent governments if a visible military presence acts as a deterrent to civil uprisings. 

related to the extent of poverty and socio-economic tensions within poor countries (Collier and Hoeffler, 2004). Interactions between poverty and conflict will have other consequences too – for example undermining financial stability and financial wellbeing (Baddeley, 2008). 

In this chapter we will develop some of these ideas by simplifying greed and grievance theory and concentrating on one dimension of the relationship between poverty and conflict: the impact of relative poverty on the probability of armed conflict. It is important to note that feedback effects will probably exist between poverty and conflict because the causality may run both ways – conflict may generate poverty e.g. if military expenditure crowds out social expenditure. If vicious circles are operating to increase poverty and armed conflict, feeding into each other, reinforcing destabilising political, socioeconomic and financial effects then the simple unidirectional model estimated in this chapter is unlikely to pick up all the interactions. This reverse causality will be manifested as simultaneity in the relationship between war and poverty, creating endogeneity (first introduced in Chapter 8). This may bias our OLS results. One solution would be to use simultaneous equation estimation – i.e. estimating more than one regression equation at a time. However, these techniques are beyond the scope of this book though further details can be found in Wooldridge (2003). In this chapter we will keep things simple by illustrating the principles of binary estimation assuming that there is no simultaneity. 

## 12.3 The data

As explained above, we are examining the impact ofpoverty on the probability ofarmed conflict. To do this, we have collected two sets ofdata: data on armed conflict and data on poverty. As explained in the theory section, there will be many more factors affecting the probability ofwar but here we are deliberately focussing on a simple model so that we can illustrate binary estimation techniques as clearly as possible. 

## Data on conflict

Overall, measuring conflict is not straightforward and there are a lot of data available – on the types of conflict (civil versus international) and the length/severity of conflicts. Conflict data are collected by a number of institutions including the Stockholm International Peace Research Institute (www.sipri.org/), the US Arms Control and Disarmament Agency (http:// dosfan.lib.uic.edu/acda/) and Uppsala Conflict Database (www.ucdp.uu.se/ database). Data from the Uppsala Universitet Conflict Database are captured in Figure 12.1 and show that, numerically, the incidence of war and conflict has subsided over the period 1992 to 2003, with the number of conflicts decreasing from 36 in 1992 to 29 in 2003. The severity of conflicts was also diminishing over this period with 16 full-scale wars in 1992 decreasing to 5 in 2003. 

Using World Bank data to sort the countries identified in the Uppsala database into income groups reveals that, between 1992 and 2003, 64% of low income countries (LICs); 37% of lower middle income countries (LMICs); 8% 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/56c237ef131d6d1db6be038f3052a0aedbb7d278947de90b6cf88210e2e3eb72.jpg)



Figure 12.1 Conflicts and wars, 1992–2003


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/8e3c01587e807ae84fe951ec50d522424edf9ea96b463f747d32db17169ad435.jpg)


Lower income Lower middle income Upper middle income Higher income 


Figure 12.2 Involvement in armed conflict, by income category


of upper middle income countries (UMICs) and 7% of upper income countries (UICs) were involved in conflicts. 

As a proportion of total numbers of conflicts, the incidence of conflict in each of these income categories is shown in Figure 12.2: of the 67 countries engaged in conflict during the period 1992 to 2003, 59% were low income countries; only 6% were the high income countries. So conflict is most common in the poorest countries and this finding adds weight to our broad hypothesis that there is a positive relationship between poverty and the incidence of war/armed conflict so it is the poorest countries that are likely to experience the devastating consequences. 

## Data on poverty and development

There are also many measures of poverty. As discussed in Chapters 2 and 4, data on levels of development, poverty and inequality are collected by a number of UN agencies and by other organisations such as the CIA. These include the UN Development Program (UNDP http://www.undp.org/) and the organisations within the World Bank group including the International Bank for Reconstruction and Development (IBRD) and the International Development Association (IDA). The World Bank co-ordinates these data collection tasks in collating a comprehensive collection of data on the international patterns of poverty and development, covering the various facets of poverty both absolute and relative. 

As explained in Chapter 2, absolute poverty captures the proportion of a population earning below the national/international poverty lines – where poverty lines are defined in terms of basic needs (such as for food, shelter, health care etc.) and broad indicators of human welfare can be captured by looking at life expectancy, literacy, infant mortality etc. 

In this chapter we will examine the relationships between war and relative poverty. Relative poverty is about inequalities in the distribution of income (or wealth). In a population in which everyone has access to plentiful food, shelter etc. there may still be relative poverty if the richest groups have a lot more than the poorest groups. 

Relative poverty can be measured by examining the proportion ofeconomic activity taking place amongst the richest versus poorest groups in a population and the commonest way to do this is to calculate the Gini index, as explained in Box 12.2. 

We use some of these data sources to analyse the impact of poverty on conflict across a sample of 50 countries. We construct our dependent variable (W= War) as follows: for a given country, if intrastate conflicts were active i.e. if there were 25 or more deaths from civil conflicts in at least one of the years between 2004 and 2006, then W= 1; if not, then W= 0. 

We use the Gini index to capture relative poverty, our explanatory variable. Unfortunately, annual data on Gini indexes are not readily available so we are forced to use different years of data for different countries; however, it is probably justifiable to assume that the extent of relative poverty does not change very rapidly within a given country, so we use the latest Gini coefficient available over the period 2000–4. We have used the period preceding 2004–6 for measuring poverty because our simple starting hypothesis is that poverty generates civil unrest, i.e. relative poverty is our leading 

## Box 12.2 Measuring inequality: Gini coefficients and Lorenz curves

The Gini coefficient was developed by an Italian statistician, Corrado Gini in 1912 as a measure of relative poverty. We use the Gini coefficient and index to capture income inequality but it can also be used to measure inequality in the wealth distribution. 

An essential building block in calculating the Gini coefficient is the Lorenz curve. The Lorenz curve traces out the cumulative proportions of income earned by cumulative proportions of the population, as shown in Figure 12.3. The Lorenz curve is ‘benchmarked against the perfect equality case, i.e. when each percentile of the population earns an equivalent percentile of the national income – as captured by the 45 degree line. 

The Gini coefficient measures the difference between the perfect equality scenario and the Lorenz curve and it is calculated using the areas under the 45 degree line. If the area between the line of perfect equality and Lorenz curve is A, and the area underneath the Lorenz curve is B, then the Gini coefficient is calculated as $\mathsf { A } / ( \mathsf { A } { + } \mathsf { B } )$ and will take a value between 0 and 1, where 0 indicates perfect equality (everyone has the same income) and 1 indicates perfect inequality (one person has all the income). 

If the Lorenz curve is not very far from the 45 degree line (i.e. in a situation of relative equality e.g. when the richest 1% would earn not much more than 1% of the national income), then the area A will be small and the Gini coefficient will be close to zero. On the other hand, if there is a lot of inequality, then the Lorenz curve will be bent away from the 45 degree line and the area A will be large: for example, in a relatively (economically) unequal population the richest 10% might earn 90% of the national income and in this case the Gini coefficient will be closer to 1. The Gini index is just the Gini coefficient as a percentage, i.e. is calculated by multiplying the Gini coefficient by 100. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/62e83c2fb392e1f398f706c1b8cf1325fd23b287bda3117be0806ef92584b2c5.jpg)



Figure 12.3 Calculating the Gini coefficient


variable. Data on the Gini index is published frequently in the UNDP’s Human Development Report (and other UN publications) but here we have used the CIA’s World Factbook because this publication provides more detailed information about the year to which their data applies. 


To summarise, the data sources are as follows:


<table><tr><td>Variable</td><td>Source</td><td>Website</td></tr><tr><td>W = War (W = 1 if &gt;25 deaths in civil conflicts, 2004–6)</td><td>Uppsala Conflict Database (UCDP)</td><td>www.ucdp.uu.se/database</td></tr><tr><td>G = Gini coefficient</td><td>CIA World Factbook</td><td>www.cia.gov/library/publications/the-world-factbook/</td></tr></table>

Given the patterns described in Figures 12.1 and 12.2 it would be easy to conclude that there is a causal link but it is important to remember that correlation does not equal causation so whilst here we are investigating the role of poverty in creating conflict there are other possibilities, e.g. either that conflict is creating the poverty and/or some third variable is the fundamental cause of both. 

## 12.4 Empirical methods and results

In this chapter, one of our aims is to illustrate binary estimation techniques and so we will draw a sharp dividing line – using a very simple measure of conflict, just to capture whether or not it happened in a given country over the period 2004 to 2006, as explained above. More specifically, we are trying to capture $P _ { i } { = } \operatorname* { P r } ( W { = } 1 | G _ { i } )$ – which is the probability of war conditioned on the degree ofinequality, i.e. dependent on G. The function that we’re estimating is: 

$$
P _ {i} = \operatorname * {P r} (W = 1 | G _ {i}) = F (Z _ {i}) \text {   where   } Z = \alpha + \beta G _ {i} + \varepsilon_ {i}\tag{12.1}
$$

The function outlined in Equation (12.1) describes a binary response model, i.e. our dependent variable is a binary variable – it covers just two mutually exclusive and exhaustive possibilities so it takes one of two possible values: 0 or 1. Binary variables are essentially dummy variables but the key difference in comparison with the dependent variables in previous chapters is that they are being used on the left-hand side as a dependent variable rather than on the right-hand side as an explanatory variable. 

Binary response models enable us to estimate the probability of war given the extent of relative poverty, i.e. the probability that W = 1 conditioned on 


Table 12.1 EViews output from estimation of the linear probability model


<table><tr><td colspan="5">Dependent Variable: WMethod: Least SquaresSample: 1 50</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>-0.414</td><td>0.366</td><td>-1.133</td><td>0.263</td></tr><tr><td>G</td><td>0.0182</td><td>0.0092</td><td>1.983</td><td>0.053</td></tr><tr><td>R-squared</td><td>0.08</td><td colspan="2">Mean dependent variable</td><td>0.30</td></tr><tr><td>F-statistic</td><td>3.93</td><td></td><td></td><td></td></tr><tr><td>Prob(F-statistic)</td><td>0.05</td><td></td><td></td><td></td></tr></table>

G: $\operatorname* { P r } ( W = 1 | G )$ . This latter part is important: if all we want to estimate is the probability ofconflict and we aren’t interested in the specific impact ofpoverty then we need nothing more than a calculator: the overall probability of conflict in this sample is 30%: i.e. 15 of the 50 countries in our sample have a $W = 1$ ; and 35 of these countries have $W { = } 0$ so the probability of peace is 70%. 

F (Z ) in Equation (12.1) is a link function i.e. it links the binary variable to a linear functional form. The simplest thing that we can do is to use the linear probability model i.e. estimate the probability of war using OLS. In this case the link function and the estimated function would both be linear and: 

$$
P _ {i} = \operatorname * {P r} (W = 1 | G _ {i}) = \alpha + \beta G _ {i} + \varepsilon_ {i}\tag{12.2}
$$

In Table 12.1 we have summarised the EViews output table for the OLS estimation of the LPM. These results suggest that there is a statistically significant relationship between W and G: the t test on the poverty parameter is significantly different from zero at a 10% significance level $\left( \mathinner { p \mathopen { = } 0 . 0 5 3 } \right)$ and we can reject the null that the parameter on G is zero. This finding is confirmed by the F test of explanatory power. However, $R ^ { 2 }$ is not much more than zero (for reasons explained below). 

We should anyway be cautious in our interpretation because we have imposed a linear world onto the estimation of non-linear probabilities and, potentially, we have misspecified our model. To explain: OLS is a linear technique – it involves estimating a line of best fit. In using OLS, we have implicitly assumed that there is a constant relationship between the probability of war and the extent of inequality. Lines are unbounded functions with a constant slope – they extend up and down without limit. But probabilities aren’t linear: they are bounded by the values 1 (i.e. a certain outcome) and 0 (i.e. an impossible outcome). As OLS estimates are not similarly bounded, OLS estimation is not always the best technique to use with binary dependent variables (though it may work well as an approximation for certain data sets). 

There are some complications with the use of the LPM to estimated probabilities. Firstly, in using a linear link function, it is possible that we will predict probabilities for a given values of the explanatory variable that are more than 1 or less than zero – either of which would be nonsensical results. Secondly, the error variances in the LPM will be heteroscedastic though this problem can be addressed using variants of the weighting procedures outlined in Chapter 6. 

Given these limitations of the LPM we may prefer to use a non-linear link function. As explained in Box 12.3, we can express the probability of war as a non-linear function of $Z _ { i }$ even though Z itself is a linear function of our explanatory variable G. This will ensure that our estimates ofthe probability of war will be bounded between 0 and 1. 

## Box 12.3 Logit and Probit

For binary variables, the probabilities of each outcome sum to 1 as the two possible events are mutually exclusive and exhaustive; there is either war or peace so the probability of one is 1 minus the probability of the other. When estimating probabilities the LPM has a number of limitations, one of which is the assumption of a constant slope on the explanatory variables. There are two non-linear functions that are commonly used to overcome this problem: logit and probit. For both these functions, the marginal effects of the explanatory variables on $P _ { j }$ will change as the explanatory variables change – the marginal effects are not constant.<sup>2</sup> 

## Logit

Logit is the log of the odds ratio, where the odds ratio is $P _ { i } / ( 1 - P _ { i } )$ . The log of the odds ratio will be linear: 

$$
\log \left(\frac {P _ {i}}{1 - P _ {i}}\right) = \log [ P _ {i} ] - \log [ 1 - P _ {i} ] = a + \beta G _ {i} + \varepsilon_ {i}\tag{12.3a}
$$

$$
\text { where } P _ {i} = \frac {\exp (a + \beta G _ {i} + \varepsilon_ {i})}{1 + \exp (a + \beta G _ {i} + \varepsilon_ {i})}\tag{12.3b}
$$

Mathematically it can be shown that the logit will have the ‘sigmoid’ shape depicted in Figure 12.4 – the slope is not constant and the function flattens as it asymptotically approaches the bounds of 0 and 1: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2b3ed4b2-4b4b-4aa5-8dff-598fb84dae4b/9dc624a5b3f061f1f0f3541c76f3e45372453989177ac241a34dde4a9c2f0798.jpg)



Figure 12.4 Logit function


## Probit

Probit is the cumulative density function from the standard normal distribution. This means that it is capturing what happens to $P _ { j }$ as $\chi _ { j }$ increases – $P _ { j }$ for a given $\textstyle \chi _ { j }$ is measured by taking the area underneath the standard normal distribution up to $\textstyle \chi _ { j }$ . Mathematically, it is derived by integrating the standard normal distribution to give the cumulative density function. The shape of the probit function is broadly similar to the shape of the logit function. See Wooldridge (2003) for further details. 

As explained above, the key advantage of using logit and probit is that they are non-linear functions and so the marginal effects of the explanatory variables on $P _ { j }$ are not constant. As they are non-linear functions, logit and probit cannot be estimated using linear estimation techniques. Instead they can be estimated using Maximum Likelihood Estimation (MLE). MLE involves identifying values of the unknown parameters (the constant and slope) that maximise the likelihood function capturing the probability of getting the values of the variables observed in the sample of data. A detailed explanation is beyond the scope of this book but see Wooldridge (2003) and Thomas (1997) for further details. 

## Log likelihood function

MLE is based around assessing the likelihood of the dependent variable conditional upon a link function and so measuring the empirical ‘fit’ of a model involves assessing the log of the likelihood function derived via MLE. For the model in this chapter, the log likelihood function is given by: 

$$
L = \sum_ {i = 1} ^ {1 5} \left\{W _ {i} \cdot \ln (P _ {i}) \right\} + \sum_ {i = 1 6} ^ {5 0} \left\{(1 - W _ {i}) \cdot \ln (1 - P _ {i}) \right\}\tag{12.4}
$$

For logit and probit the log likelihood function will always be negative because the probabilities are bounded between 0 and 1 and so the logs of the probabilities will be negative. If the likelihood function is relatively close to zero then the empirical model is working relatively well. 

The most restricted version of the log-likelihood function contains only the intercept. The restricted log likelihood function for the example in this chapter can easily be calculated as follows: 

1. The probability of war $( W = 1 )$ is given by $P _ { i } = 0 . 3 0 , \mathsf { I n } ( 0 . 3 0 ) = - 1 . 2 0 4$ . The probability of peace $( W = 0 )$ is given by $( 1 - P _ { i } ) { = } 0 . 7 0$ and $\mathsf { l n } ( 0 . 7 0 ) = - 0 . 3 5 7 .$ 

2. For 15 of our observations $W = 1$ and adding these together gives $1 5 \times - 1 . 2 0 4$ 

3. For 35 of our observations $W { = } 0$ and adding these together gives $3 5 \times - 0 . 3 5 7$ 

4. The restricted log likelihood function is calculated by applying Equation (12.4) as follows: 

$$
L = \sum_ {i = 1} ^ {1 5} \left\{W _ {i} \cdot \ln (P _ {i}) \right\} + \sum_ {i = 1 6} ^ {5 0} \left\{(1 - W _ {i}) \cdot (1 - P _ {i}) \right\}\tag{12.5}
$$

$$
= \{1 5 \times - 1. 2 0 4 \} + \{3 5 \times - 0. 3 5 7 \} = - 3 0. 5 5
$$

## Likelihood ratio (LR) test

We can use a restricted log-likelihood function to assess the contribution of our explanatory variables by comparing the log likelihoods in restricted and unrestricted models. Thus the LR test is like a non-linear equivalent of the F test of restrictions and it is calculated using the following formula: 

$$
L R = 2 (L _ {u} - L _ {r})\tag{12.6}
$$

This test follows a $\chi ^ { 2 }$ distribution with ${ \mathsf { d } } { \mathsf { f } } = d$ where d is the number of restrictions embedded within the restricted model. 

As explained in Box 12.3 two non-linear techniques commonly used to estimate probabilities are logit and probit. In capturing W as a non-linear function of G, we have used logit estimation. We have selected logit because it has a clear conceptual basis. However, probit is also very commonly used and we have designed a chapter exercise around probit estimation; for the empirical model in this chapter, the results from logit and probit estimations are very similar. The output from the EViews estimation of the logit model is summarised in Table 12.2. 

For our EViews output table, the sample statistics provided are z scores calculated from standard normal distributions. This is because, as explained in Box 12.3, logit estimation requires MLE techniques – asymptotic techniques that assume a large sample. As Student’s t distribution is a small sample approximation of the standard normal distribution, t statistics are not reported. 


Table 12.2 EViews output from estimation of the logit model


<table><tr><td colspan="5">Dependent Variable: WSample: 150</td></tr><tr><td>Variable</td><td>Coefficient</td><td>Std. Error</td><td>t-Statistic</td><td>Prob.</td></tr><tr><td>Intercept</td><td>-4.46</td><td>1.95</td><td>-2.29</td><td>0.02</td></tr><tr><td>G</td><td>0.09</td><td>0.05</td><td>1.92</td><td>0.05</td></tr><tr><td>Log likelihood</td><td></td><td>-28.63</td><td>LR statistic (1 df)</td><td>3.84</td></tr><tr><td>Restr. log likelihood</td><td></td><td>-30.54</td><td>Probability (LR stat)</td><td>0.05</td></tr><tr><td>Obs with Dep = 0</td><td></td><td>35</td><td>Total observations</td><td>50</td></tr><tr><td>Obs with Dep = 1</td><td></td><td>15</td><td></td><td></td></tr></table>

Note that the parameter estimate on G (0.09) is capturing the average marginal effect. It’s important to re-emphasise that for logit (and probit) estimation the slopes are varying and the marginal effects will be conditional upon a particular value of the explanatory variable. The observed responsiveness for any given observation will be conditional upon the magnitude of the explanatory variable. 

These results from the logit estimation are similar to the results from the estimation of the LPM; the null that the parameter on the Gini coefficient is equal to zero can be rejected at a 10% significance level. EViews does not provide $R ^ { 2 }$ for logit and probit estimations because $R ^ { 2 }$ is not particularly meaningful: it captures the goodness of fit in linear estimation and we are using logit – a non-linear estimation technique. As explained in Box 12.3, for non-linear models the log likelihood function is more meaningful than $R ^ { 2 }$ in measuring the relative ‘fit’ of the model. As shown in Box 12.3, calculating the log likelihood function involves summing together the log likelihoods across the sample and for the estimation of Equation (12.7) the restricted log likelihood is −30.55. This restricted log likelihood incorporates the restriction that the parameters on an explanatory variable are jointly equal to zero and so this statistic can also be calculated using EViews by regressing W just on the constant term. Notice also that this restricted log likelihood is approximately equal to the natural log of the estimated intercept in the LPM (see Table 12.1). 

We can calculate the relative contribution of G to the model by comparing log likelihoods from the restricted and unrestricted versions (where the unrestricted model is the model including all the explanatory variables as well as the constant) using a Likelihood Ratio test as explained in Box 12.3. 

Applying the LR test to our example this gives the following (the probability value is from EViews): 

$$
L R = 2 \left(L _ {U R} - L _ {R}\right) = 2 \times (- 2 8. 6 3 + 3 0. 5 5) = 3. 8 4 [ p = 0. 0 5 ]\tag{12.7}
$$

With $\scriptstyle { p > 0 . 0 5 }$ we can reject the null that the slope parameter on G is insignificantly different from zero at a 5% significance level. We can conclude that there is a statistically significant relationship between W and G and this confirms the findings from our $Z$ test – in this sample ofdata there is a positive association between conflict and poverty. 

How do these results differ from our LPM estimated using OLS? With the logit estimation, the estimates of the probability of war are bounded between 1 and 0 for all possible values of G. This is because the slope parameter, which captures the marginal effect ofG on $P _ { i } ,$ is not constant but is itselfa function of $G _ { i \cdot }$ At extreme values of $G _ { i }$ the change in the probability of war for a given change in $G _ { i }$ is very small but, for average values of $G _ { i } ,$ the change in the probability of war for a given change in $G _ { i }$ is relatively large. These changes in the marginal effects are what ensure that the logistic function has the sigmoid shape described in Box 12.3. 

The results from the estimation of the logit function seem plausible. But further investigations are needed to establish the directions of causality and possible simultaneity. There may also be other variables that are important, for example financial instability. A more thorough investigation ofthese issues would require a combination of techniques, for example logit/probit techniques to capture probabilities, combined with simultaneous equation estimation techniques to capture simultaneity. As mentioned above, simultaneous estimation is beyond the scope of this chapter but refer to Wooldridge (2003) for further guidance. 

## 12.5 Implications and conclusions

The results from this chapter suggest that there is a positive relationship between poverty and conflict. If further studies establish that this positive association is robust, then strategies to promote peace should concentrate (amongst other things) upon ensuring a more equitable distribution of income and resources within economies. 

More detailed analyses would have to take into account a range of other variables and in understanding conflict in poor countries it is important not only to examine the causes of war but also the consequences. Feedback effects may affect the relationship between poverty and conflict: just as poverty encourages conflict so conflict will exacerbate poverty. Collier and Hoeffler (2004) observe that conflicts will encourage opportunistic behaviour and weaken the institutions that usually provide low cost services and/or facilitate the smooth operation of the market mechanism, thus exacerbating poverty. This explains why conflict and inequality are so common in poor countries with abundant natural resources such as diamonds and oil (Collier, 2008). 

During civil war, the ratio of military expenditure to GDP rises sharply, ‘crowding out’ social expenditures that could be used to promote broadly based development. So the poorest groups will suffer the most if economic decisions reflect military and political goals. Overall there will be the potential for a significant peace dividend when conflicts end not only in terms of economic growth but also in terms of a less impoverished society. 

There may be other implications too: if arms are being imported (as they often are), then this may create external problems of balance of payments crisis and excessive foreign debt burdens. These will contribute to financial instability and will retard/reverse the evolution of modern financial institutions, creating substantial and prolonged constraints on the availability of finance. 

## 12.6 Further reading

## Textbooks and monographs



Collier, P. (2008) The Bottom Billion, Oxford: Oxford University Press. 





Sandler, T. and Hartley, K. (1995) The Economics of Defense, New York: Cambridge University Press. 





Schelling, T. (1960) The Strategy of Conflict, Cambridge, MA: Harvard University Press. 





Thomas, R. L. (1997) Modern Econometrics – An Introduction, Harlow: Addison-Wesley, pp. 469–77. 





Wooldridge, J. M. (2003) Introductory Econometrics (2nd edition), Thomson South-Western, Chapters 7 and 17. 



## Academic articles and working papers



Baddeley, M. C. (2008) ‘Poverty, armed conflict and financial instability’, Cambridge Working Papers in Economics No. 0857, Faculty ofEconomics, University of Cambridge. 





Benoit, E. (1978) ‘Growth and defense in developing countries’, Economic Development and Cultural Change, vol. 26, 271–80. 





Collier, P. and Hoeffler, A. (2004) ‘Greed and grievance in civil wars’, Oxford Economic Papers, vol. 56, 563–95. 





Fitzgerald, E. V. K. (1997) ‘Paying for the war: macroeconomic stabilization in poor countries under conflict conditions’, Oxford Development Studies, 25(1), 43–65. 





Schelling, T. (1958) ‘The strategy of conflict – prospectus for a reorientation of Game Theory’, The Journal ofConflict Resolution, vol. 2, no. 3 (September), 203–64. 



## Policy briefs

Jackson, M. O. and Morelli, M. (2005) ‘War, Transfers, and Political Bias’, http://economics.sbs. ohio-state.edu/morelli/warbias4.pdf. 

UN Millennium Development Goals Report 2007, Geneva: United Nations. 

UNDP, Human Development Report, Geneva: United Nations, various years. 

World Bank, World Development Report, World Bank, Washington, various years. 

## 12.7 Chapter exercises

1. Estimate a Probit version of Equation (12.1) using the data provided. Briefly explain the method and check your results against the results from this chapter. 

2. In this chapter, we have focussed on only one of the potential determinants of conflict, i.e. poverty. Using the data sources cited in this chapter: 

(a) Collect your own data focussing on the variables that you think might be important determinants of armed conflict. 

(b) Construct an empirical model of conflict. 

(c) Estimate your model using binary estimation techniques. 

(d) Interpret your results and assess the policy implications. 

## Index

absolute poverty 269 measurement of 40 accelerator theories, of investment 179 additive dummy variable 213 additive function 72 adjustment costs curve 180 adverse selection 88–9, 181 agricultural markets, importance of lags 230 aid, to developing countries 56–7 air travel, income and substitution effects 67, 161 data on 75–6 elasticitiy of 75, 83 heterogeneity 74 marketing strategies 83 model specification 79–81 exclusion of substitutes 83 functional forms 73 income variables 83 logs and elasticities 72–3 price data 77 sample size 78 sampling bias 77 Akaike's Information Criterion 219 Akerlof, G., lemons principle 89, 105 anchoring effects 251 Andre, C. 132 angel investors 206 Annan, Kofi 39 AR(1) error process 167, 169, 170, 173 arbitrage, and efficient markets 183 Arrow, K. 105 Ashley, C. 177 asset specificity 181 asymmetric information 88–9 asymptotic properties 23–5 Atkinson, A. B. 60, 105 Auerbach 105 Augmented Dickey – Fuller (ADF) unit root tests 217, 219 on consumption model 235 and structural breaks 221 

autocorrelation 25, 33, 35, 126, 165, 257 Breusch–Godfrey Lagrange Multiplier test 169–71 Cochrane–Orcutt two stage procedure 173–5 Durbin – Watson test 167–8, 169 and OLS 166 visual detection of 166–7 autocovariance 215 Automated Clearing House (ACH) systems 203 autoregressive distributed lag (ARDL) model 238–43 link with ECM 239–40 auxiliary regression 148 average propensity to consume, stability of 229, 232, 243 and error correction models 238 in Friedman’s work 235 in Keynes's work 234 average q 181, 184 proxy for marginal q 185 see also Tobin’s q aviation emissions, and international flows of tourists 161-5, 175 Baddeley, M. 131, 160, 176, 179, 196, 204. 223, 278 Bamford, C. 84 Bank of England consumption patterns 228 response to credit crunch 131 Barometer of Sustainability (BS) 162 basic human needs, definition of 60 Becker, Gary, rational choice theory 249–50, 262 behavioural economics 194–5 Benoit, E. 264, 278 Bentham, Jeremy, and utilitarianism 25 Best Linear Unbiased Estimators (BLUE) 21, 22, 24, 32 binary dependent variable estimation 272–3 binary estimation technique see logit estimation binary response model 271-2 biotechnology, and New Economy 202 Bismarck, and public health insurance 87 black box, firm as a 181–2 

Bond, S. 197 Breusch–Godfrey Lagrange Multiplier (BG) test 169–71, 174, 191, 221 Friedman’s permanent income hypothesis 237 Keynes’s consumption function 236 model misspecification 190, 192 Brin, Sergey, and Google 206 Brons, M. 84 Brown, Gordon, PM 244 Brynjolfsson, E. 201, 223 Bush, President George W. 244 business confidence surveys 14 Business Enterprise R&D (BERD) 139 Camerer, C. F. 195, 196 Canadian Department of Finance 74, 75 capital stock adjustment see accelerator theories carbon offset/balancing schemes 176 cardinal measurement 13 cat bonds 194 Catte, P. 132 Cecchetti, S. G. 204, 223 Central Limit Theorem 24, 149 Chon, K.-S. 176 Chow test 210, 211–13 Chrystal, A. 41 civil war, explanation for 265 and game theory 266 climate change, impact of air travel 161, 175–6 Clinton, President Bill 244 CO emissions audits of 163 and rising demand for tourism 163–5 Cochrane–Orcutt (C–O) two stage procedure 172 173–5 coefficient of determination (R<sup>2</sup>) 21, 53, 54 adaptation for MRA 121, 122, 126–7 of life expectancy and health expenditure 102, 103 and sum of squares 55 cognitive bias 251 cointegration 237–8 and error correction term 238 Collier, P., greed and grievance theory 265, 266, 278 computerisation, growth of 203 see also computing investment computing investment 201 data for 207 limitations of 208–9 and NASDAQ crash 204 and venture capital financing 206–8, 209–10, 217 DF/ADF tests 219–20, 221, 222–3 

confidence interval 30, 34 conflict availability of finance for 278 data on 267–8 and inequality 264–8, 277–8 binary response model 271–2 linear probability model 272, 273 political motivation for 265 see also conflict data, greed and grievance theory; logit estimation; poverty, data consistency 24 constant elasticity of demand 71, 81 constant growth model 73 consumption, relationship with income data for 232 policy implications 244 rise in 225–6 see also ARDL model, consumption function, ECM model; lags consumption function Friedman’s theory 231, 234–5, 237, 243 Keynes’s theory 229–31, 232, 233–4, 236, 237 consumption smoothing 231 see also life-cycle theory; permanent income hypothesis; Veblen effects correlation coefficient 20 correlation versus causation, importance in healthcare model 104–5 Council of Mortgage Lenders 114, 116–17 covariance 18 credit crunch 111, 131 credit restraints 112–13 and house price slumps 124 see also gearing ratio critical value 27, 28 cross-price elasticity of demand 69, 70 cross-sectional data 13, 199 and time-series data 250 see also panel estimation; pooling current replacement cost 182 Cutler, D. 105 Darling, Alistair, MP 244 data constraints 77–8, 82 data mining 122 decision rule 27 defence spending and alleviation of poverty 264 effect on social expenditure 278 demeaning 258–9 dependent variable/regressand 12, 14 deterministic and stochastic trends 33, 215 diagnostic tests 26, 145– 

Dickey-Fuller (DF) unit root tests 217, 218-19 and structural breaks 221 see also Augmented Dickey–Fuller Diener, E. 251, 262 difference estimator 257–8 distributed lag specification 230 divorce data 249, 253 limitations to 253 divorce, effect of economic conditions on 252, 253 and government policy 261 model of 261 need for interdisciplinary research 261 and rational choice theory 250 dominant strategy 159 dotcom bubble 194 irrational exuberance 194 and venture capital 207 double-log model 73 Dougherty, C. 32 dual economies, and civil war 265 dummy variable trap 119, 259 and multicollinearity 119 and reference category 119–20 dummy variables 14 and cross-section specific fixed effects 259 and structural breaks 212 Dunne, T. 204, 224 durable consumption goods, lumpiness 112 Durbin-Watson test for autocorrelation 164, 167–8 limitations of 168 problems with 169 Durbin’s h test 169 Ecological Footprint methodology 162 econometric analysis, use of 1–2, 3, 11–12, 32–3 econometrics packages 31 and social sciences 2–3 Economist, The 132, 194, 197, 245 Edlund, L., marriage and labour mobility 252, 262 efficient markets hypothesis 182 and Tobin’s q theory 182, 183, 193 elasticities 69–71, 75 relationship with inverse demand functions 71–2 use of logs for estimation 72 see also own-price elasticity of demand Electronic Funds Transfer at Point of Sale (EFTPOS) 203 endogeneity 141, 165, 185, 257 and simultaneity 267 Engle–Granger rule of thumb 217, 236, 238 entrepreneurship, funding of 206 

environment, global issues 161 impact of tourism 157, 158, 163–5 measurement of 157–62 social costs of change 160 see also aviation emissions; Tragedy of the Commons Environmental Pressure Index (EPI) 162 equilibrium, and ECMs 240 error correction model (ECM) 238, 242 link with ARDL 239–40 error variance, see heteroscedasticity; homoscedasticity error/disturbance term 15 expected value 16 in Gauss–Markov theory 25, 107 sample residual 16, 18 EViews ARDL model 242 and BG tests 170 Chow test 214 DF/ADF test 217–19 divorce data, fixed effects estimation with dummy variables 260 pooled estimation 255 ECM model 242 Friedman’s permanent income hypothesis 237 and heteroscedasticity 142, 145 OLS regression 140 White’s test 148 and homoscedastic errors 153 Keynesian consumption function 235, 236 Likelihood Ratio test 277 linear probability model 272 logit model 276 use in running regressions 81 exogeneity, in Gauss–Markov theory 25 expectations and consumption 231 role in investment theory 178, 193 and stock market 183 expected revenue curve 180 experienced happiness measures 25 explained sum of squares (ESS) 21, 54, 55 export growth, and poverty 43, 63 external economies 160 externalities, and state intervention 87 extreme value estimation 273 

F test 27 and critical values 28 F test of explanatory power 30–1, 33, 102–3, 127, 128, 175 

F test of restrictions 127, 128–30, 170 in ARDL model 243 and Chow test 212 in ECM 241–3 and Granger causality 241 and Ramsey’s RESET test 192 Fagerberg, J. 155 fair trade rules 57 feasible WLS (FLS) 151–2 Feldstein, M. 105 financial deregulation and credit control 226 effect on housing market 110–11, 113, 117 self-regulation 131 financial markets, inefficiency 193, 194–5 Financial Services Authority (FSA), and Northern Rock crisis 131 Financial Times, The 115, 132 financial transactions, taxes on 195 fitted/predicted values 53 Fitzgerald, E. V. K. 279 fixed asset investment 178 fixed effects estimation 258–9 and pooling 256 framing effects 251 Fraumeni, B. M. 203, 204, 224 Frey, B. S. 252, 262 Friedman, M. 244 see also consumption function functional form 73, 79, 187, 188–93 identification of 187–8 linearity 187 model misspecification error 187, 190, 192 functional magnetic resonance imaging (fMRI) 195 fundamental value, of firm 183 game theory 158 and military strategy 266 Gauss–Markov assumptions 24, 25, 26, 127,140 diagnostic tests 143, 145–9 and least squares 151 see also autocorrelation Gautier, P. A., and marriage 252, 262 GDP growth, and poverty reduction 41, 42, 44 achievement of 41–2 theory testing correlation coefficient 46–8 data analysis 43–4 empirical analysis 44 sample covariance 46 

simple regression analysis 48–56 visual inspection of data 45–6 see also growth and poverty regression analysis gearing ratio 112, 113, 117 Gender-Related Development Index (GDI) 96 Generalised Least Squares (GLS) 161 solution to autocorrelation 171–3, 174, 175 Genuine Progress Indicator (GPI) 162 geometric progression 228 Giffen goods and air travel 82 income and substitution effect 67, 68 Gillen, D. W. 84 Gini coefficient 269–71 Girouard, N. 132 global poverty, UN meeting 36 globalisation, and foreign finance 226 Goldfield–Quandt test 146–7 goodness of fit 53 in MRA 121–2, 125 autocorrelation 126 see also coefficient of determination Gordon, R. G. 203, 223 government policy, on climate change 176 government spending 87 Granger causality tests 241 Grant, S. 84 greed and grievance theory 265 Greene, W. H. 32 Greenspan, Alan 194 grid search procedure 172 Griffiths, A. 244 gross capital formation (GCF), and investment growth 44 growth, and poverty regression analysis data, 47 hypothesis testing 49 coefficient of determination 53, 54 confidence intervals 52 critical value 51 goodness of fit 53 significance level 51–2 Student's t-test 49–51 parameter estimates 48–9, 53 calculating standard error 50 Gujurati, D. N. 32 Halifax index 115 Hardin, G. 158, 176 Hartley, K. 264, 278 Hayashi, F. 182, 196 

health expenditure market-based services 88, 90 measurement of 95 per cent change in expenditure 95 purchasing power parity (PPP) 95 by state 86–8, 90, 104 see also asymmetric information health indicators data limitations 97–8 differences between rich and poor 94, 97 health sector reforms 88 health, social determinants of 105 healthiness, link with health expenditure data collection 92–3 measurement of 96 regression model 99, 100 hedonic pricing 114, 115–16 hedonic psychology 250, 251–2 Helbling, T. F. 132 Henderson, J. 96, 105 heterogeneity bias and panel estimation 257 and pooling 256–7 see also difference estimator heteroscedasticity 73, 136, 140, 165 diagnostic tests for 145–9 implications for analysis of innovation 142 solutions to 149–54 visual inspection 143–5 see also weighted least squares high frequency data 13, 199 Hirschleifer, D. 194, 196 Hoeffler, A., greed and grievance theory 265, 266, 278 Holden, A. 176 Hometrack index 115 homoscedasticity 25, 33, 140–1 house prices and affordability 110, 111, 117 association with mortgage lending 124, 131 indices 115 measurement of 114 volatililty 110 see also Minsky household spending, and recession 225 see also consumption housing data, limitations of 114 see also hedonic pricing housing demand implications for macroeconomy 109–11 model assessment 118 limitations of findings 130–1 multiple regression analysis 121–30 trends in 116–17 

housing wealth, and credit constraints 112 Human Capital Index (HCI) 136 Human Development Index (HDI) 96 Human Poverty Index (HPI) 96 hypothesis tests alternative hypothesis 49 null hypothesis 27, 49 test statistic 27 Type I and II error 28, 29, 78, 82 see also F test, F test of explanatory power, F test of restrictions, p values, Students t-test IMF World Economic Outlook Database 207 imperfect micronumerosity, data on R&D 136 income and consumption 12 measurement 228 income effect and price change 66 and price elasticities of demand 69 independent variables/regressors 12 Index of Sustainable Economic Welfare (ISEW) 162 infant mortality rate 94 data limitations 97 and expenditure on public health 93 infeasible WLS 151 inferior goods income and substitution effect 66, 67, 68 see also Giffen goods information technology (IT) diffusion and finance 205–6 and GDP growth 20 investment and macroeconomic performance 201, 204–5 knowledge-driven technological change 202–3 revolution in 203–4 economic flexibility 204–5 see also computing investment, Solow, Computer Paradox information uncertainty 14 innovation, and economic performance 134, 154 formal role of R&D 154 and LDCs 154 measurement of 136 necessity for 133–4 see also R&D expenditure Innovation Policy in Europe, Summary Innovation Index (SII) 136, 137 institutional lags 230 institutions, impact of conflict on 278 instrumental variable (IV) estimation 188 Intel, microprocessor chip 203 interest rates, effect on UK mortgage markets 111 

Intergovernmental Panel on Climate Change (IPCC) 161, 177 internal adjustment costs 179–81 International Bank for Reconstruction and Development (IBRD) 269 International Civil Aviation Organisation (ICAO) 75 International Development Association (IDA) 269 International Development Research Centre (IDRC) 91 International Energy Agency (IEA) 162 Internet, and New Economy 202 invention versus innovation 134 inverse demand curves 68 and air travel 76, 82 investment growth, and poverty 42, 44, 57, 63 in housing 110 rate relationship with Tobin’s q 186, 187, 188–93, 195–6 functional form 188–93 lags 193 theory 178, 179 see also Tobin’s q irrelevant variables 187 Ito, H. 84 Jackson, M. O. 266, 279 Jevons’s sunspot theory 194 joint hypothesis test 103 Jorgenson, D. W., neo-classical investment theory 179, 196 Kahneman, Daniel 194 and hedonic psychology 250, 251, 262 Kamstra, M. J. 194, 196 Katona, G. 194 Kennedy, P. 32 Kennedy, President John F. 244 Keynes, J. M. on consumption 225, 226, 244 and financial markets 194 and Tobin’s q theory 183, 196 see also consumption function Keynesian models of growth 42 Klemm, A. 197 Klette, J. 155 Kortum, S. 155 Koyck model 230 Kramer, L.A. 194, 196 Kuznets, S. 229, 232, 243, 245 lag structure, identification of 33 lags, use of, and consumption function 229, 230 see also ARDL mode 

Land Registry 115, 116 Landefeld, J. S. 203, 204, 224 law of large numbers 24 Layard, R. 252, 262 LDCs, environmental sustainability and tourism 160, 175 measurement of 162 Lee, D. 84 leverage 112 Levi, M. D. 194, 196 life expectancy 94 and expenditure on health 93, 97, 99 cross-sectional sampling bias 98 data limitations 97 life-cycle hypothesis 231 Likelihood Ratio (LR) test 275, 276 limited war 266 line of best fit/regression line 17, 48–9 linear models 14, 25 linear probability model 272 complications with 273 linearity 22–3 link function 272 Link, A. N. 155 lin-lin specification 73, 188–92 lin-log specification 188–92 Lipsey, R. 41 liquidity constraints, and consumption theory 232 Loewenstein, G. 195, 196 log likelihood function 274–5, 276 logit estimation 273, 274, 275–6, 277 see also log likelihood functior log-log specification 73, 79, 81, 188–92 and heteroscedasticity 149, 152 London Stock Exchange 185 long-run elasticities 238–43 unitary 239 Lorenz curve 270 lumpiness, of durable goods 112 

Mankiw, G. 42, 244 marginal propensity to consume 226–8, 233 marginal q 181, 184 marriage and health 252 and rational choice theory 250 Maximum Likelihood Estimation (MLE) 23. 274, 275 and log likelihood function 274 McGuire, A. 96, 105 measurement error 14, 185 and proxy variables 78 Median and Mean lag models 230 Meyer, D. 177 

micro-founded macroeconomic theory 231 micronumerosity 78, 127–30, 209 and pooling 254 military, institutional role of 264 Millennium Development Goals (MDGs) 36–7, 59 minimum variance 22 Minsky, H. P., financial fragility hypothesis 113, 132 mobile wallets 203 model misspecification 99, 165, 187, 192 see also Breusch–Godfrey test; Ramsey’s RESET test model parameters 12, 15 correct specification in GM theory 25 degrees of freedom 28 estimates of 34, 48–9 Modigliani, consumption theory 231, 232, 235, 243 Monetary Policy Committee 14 Monte Carlo experiments 15 Mooney, G. 96, 105 Moore’s Law 203, 208 moral hazard 88 Morelli, M. 266, 279 Morrison, W. G. 84 mortgage lending association with house prices 123–4, 127, 131 and unitary elasticity 125 excessive 113 liquidity of market 110 rates and demand for housing 124, 13 sensitivity to interest rate changes 111 see also gearing ratio moving average error 258 Mowery, D. 155 Muellbauer, J., and gearing ratios 113, 132 multicollinearity 25, 119, 127 multiple regression analysis (MRA) 121–2 disadvantages of 127 use of econometric packages 122 EViews 122, 128, 129 see also housing demand multiplicative dummy variable 213 multiplicative function 73 multiplier effect 226–8, 229 different forms of relationship 228 Murphy, A., and gearing ratios 113, 132 Muth, J. F. 182, 196 NASDAQ crash 204 Nash equilibrium 159 National Science Foundation 207, 208 Nationwide building society, house price data 114, 115, 116–17 negative autocorrelation 166, 168 

negative equity 109, 113 negative externalities 159 Nelson, R. 155 neuroeconomics 195 New Economy, growth in 202, 205 see also computing investment New York Stock Exchange (NYSE) 182, 196 Newton-Smith, R. 197 Nijkamp, P. 84 non-stationarity 165, 214–16 elimination of 220 and structural breaks 221–2 see also DF tests; spurious regressions non-stationarity, in permanent income hypothesis 237 normal equations 18 normal goods, income and substitution effect 66, 68 normalisation of data, and heteroscedasticity 149 normality assumption 25 Norman, B. 228, 229, 245 odds ratio 273 OECD 135 housing market data 114 Science and Technology Industry Outlook 136, 155 Social Expenditure Database 93, 95, 105 Office for National Statistics (ONS) 185, 232, 253 housing market data 114, 116, 117 Office of the Deputy Prime Minister (ODPM), Survey of Mortgage Lenders (SML) 115, 116 omitted variable bias 54, 99, 121, 187 in consumption-income model 243 and pooling 256 one-tailed t test 29, 82 and unitary elasticity 125 Opperman, M. 176 order of integration, of variable 220 Ordinary Least Squares (OLS) models 107 calculation of 17–19 data generating process 12–15 estimation 12 Gauss–Markov theorem 21–6, 32 and heteroscedasticity 152 hypothesis testing 26–31, 33, 49 measuring correlation 20 and goodness of fit 20–1, 33, 35 and misspecification error 187 properties of estimators 21–6 sample regression function (SRF) 15–16 types of data 13–14 

Oswald, A. J. 109, 132 marriage and health 252, 262 outliers 144 and problems of heteroscedasticity 82, 149 own-price elasticity ofdemand 69, 70, 71, 75, 79, 80, 82 Page, Larry, and Google 206 Page, S. 177 panel estimation 33, 250, 257 data sets 13, 78 household surveys, problems of 90 parameter instability 211, 212 parameter linearity, and OLS technique 72 Pareto optimal strategy 159 patents, number of 134 data problems 137–8 and R&D expenditure 136 model of 139–40, 142–3, 152 pay-off matrix 159 Pels, E. 84 permanent income hypothesis 231, 234–5, 237 Plato 39–40 political bias 266 pooling 13, 254–6 problems with 256–7, 26 Population Census 13 positive autocorrelation 166, 168 poverty data on 269–71 and institutional reform 38 and investment 57 reduction of 36, 41 see also conflict, inequality; GDP growth, and poverty reduction; trickle down theory poverty line 59 poverty measurement 59 monetary indicators 59–60, 62 limitations to 60–1 use of 61 non-monetary indicators 61-2 see also Gini coefficient Prelec, D. 195, 196 Price, R. 132 price changes, balance of income and substitution effect 66 price elasticity, and fiscal policy 84 price transparency 202 pricing 64–5 and monopoly power 65 and perfect competition 65 Prisoner's Dilemma (PD) 158–9, 175, 176 

privatisation, of health care 88 and exclusion 88 see also adverse selection probability (p) values 28, 101–2 probit estimation 274, 275, 276 see also log likelihood function productivity, and IT development 204 prospect theory 251 proxy variables 77–8 psychological lags 230 psychology of economic and financial decision making 194 psychometric testing 195 public goods 87 public health care 89–90 public health insurance 87 purchasing power parity (PPP) 95 qualitative data 13 Ouality Adjusted Life Years (OUALYs) 96 Quality of Life Index (QLIs) 96 quantitative data 13 quasi-markets, in health sector 88 R&D expenditure 134 and heteroscedasticity 142–3, 145–9 and increase in innovativeness 135 model of 139–40, 152 policy implications 154–5 problems with data 138–9 R&D intensity 136 and heteroscedasticity 152, 154 Ramsey’s RESET test 33, 188, 190, 191 random effects estimator model 257 random walks 215, 216 with drift 215-16 see also DF tests rational choice theory 249–50 rational expectations, and Tobin’s q 182, 183, 193, 196 real wages, and IT development 204 relative poverty 37–40, 269 reliability indicators 22 replacement investment 181 repossession 113 representative agent hypothesis 183 residual autocorrelation 209 see also non-stationarity; structural breaks residual sum of squares (RSS) 18, 33, 50, 53, 54, 55 and Chow test 211 and F test of restrictions 128-30 residual variance 18, 19, 141–2 actual versus fitted values 144–5 Rietveld, P. 84 

Rightmove index 115 Rodrik, D. 42 Roe, D. 177 Romer, D. 42 Roosevelt, President Franklin D. 36 Rowthorn, R. 250, 256, 262 RSS comparisons 170 sample estimates 16 sample residual 53 sample size 78 sampling bias 16, 90, 98 data on R&D 136 Sandler, T. 264, 278 Schelling, Thomas 265, 266, 278, 279 Scherer, F. M. 155 Schumpeter, J.A., and creative destruction 205, 22 Schwartz Information Criterion 219 Schwarz, N. 251, 262 Seasonal Affective Disorder (SAD) and stock market activity 194 seasonality, and use of dummy variables 117, 118–20 see also dummy variable trap Sebastia-Barriel, M. 229, 245 semi-log model 73 serial correlation, see autocorrelation shadow price 181 Shiller, R. 194, 196 Shleifer, A. 194, 196 Shumway, T. 194, 196 significance level 28, 33 and critical value 51–2 exact 28 and p values 101 Types I and II error 28 simultaneity 12, 241 in relationship between war and poverty 267 simultaneous equation estimation 267 single neuron experiments 195 Smith, Adam, Invisible Hand 158 Smithers, A. S. 185, 196 social benefits, of fiscal policies 84 social determinants of health 105 social gradient 105 Solow, R. M. 42 and Computer Paradox 204, 224 speculative bubbles 194 spread of observations 18 spurious regressions 215, 216–17 in ARDL and ECM models 241 Engle–Granger rule of thumb 217 standard errors 19 and heteroscedasticity 142 

standard normal distribution 24 stationarity of variables 33 Stern, N., The Stern Review 161, 177 Stewart, C. 84 Stiglitz, J. 105 stochastic error 167 stochastic trends 215–16 stock market values 182 rational expectations 193 stock market volatility, implications for investmen and capital accumulation 195–6 Stock, J. H. 32, 155, 172 Stockholm International Peace Research Institute 267 structural breaks 33, 165, 210–14 and F test of restrictions 213 and non-stationarity 221–2 see also Chow test Student’s t-test 27, 29–30, 33, 34, 49–51, 187 and critical values 28 Stutzer, A. 252, 262 sub-prime mortgage lending 11 substitution effect 65 and price elasticities of demand 69 super consistency 237 supply, of housing 110 supply-induced demand 88 Svarer, M., marriage 252, 262 Swan, T. 42 Syed, M. 197 systematic patterns in residuals, causes of 165 

Tanzania, data collection on health 90, 91–2 Technological Activity Index (TAI) 136 technological change implications for global economic activity 202–3 lags 230 Teulings, C. N., marriage 252, 262 theoretical imperialism 249 Thirlwall, A.P. 42 Thomas, R. L. 32, 146, 155, 223, 230, 243, 244, 274, 278 Time-series data 13 combined with cross-sectional data 250 see also panel estimation, pooling Tinbergen, J., multiplier effects 228, 229, 245 Tobin’s q 179, 182–3, 184, 196 data collection 184–6 exclusion of lags 193 macroeconomic version of 183 rational expectations 193 total costs curve, in adjustment cost theory 180 total market capitalisation 182 total sum of squares (TSS) 21, 54, 55 

tourism, economic contribution of 157 and environmental change 160, 163–5 tourism life-cycles 160 and sustainability 160 Tragedy of the Commons 158–60 trickle-down theory 41, 42, 56 policy implications 56 Tulipmania 194 Tversky, Amos, and hedonic psychology 194, 250, 251, 262 two-tailed t test 29 and critical value 51 on housing demand model 123–4 Type II error and DW test 169 and GQ test 147 and multiple regression analysis 127 

UN Conference on Trade and Development 42,43 World Investment Report 156 UN Development Program (UNDP) 93, 95, 105, 269 Human Development Indicator (HDI) 14 UN Framework Convention on Climate Change (UNFCCC) 161, 163 UN Millennium Development Goals 279 UN World Trade Organisation (UNWTO) 162, 177 unbiasedness 22–3 uncertainty, role in investment theory 178 unemployment effect of housing market on 109 and IT development 204 unit roots 215–16, 221 see also DF tests unitary elasticity 125 Uppsala Conflict Database 267, 271 US Arms Control and Disarmament Agency 267 US Bureau of Economic Analysis (BEA) 185, 205, 207,208,253 US National Center for Health Statistics (NCHS) 253 US Patents Office 136 user cost of capital 179, 180 utilitarianism 251 

Varian, H. 84, 176 variance 18 allowance for heteroscedasticity 142 calculation of 19 ratio of explained to unexplained 21 visual inspection 143–5 Veblen effects 231 venture capital funding 206 data for 207, 208 and growth of New Economy 202 role of government 223 see also computing investment Verleger, P. K. 84 Vlieghe, G. 197 

Wall, S. 244 war, probability of, see conflict, and inequality Watson, M. W. 155, 172, 203 wealth inequalities, and housing market 110 weather, psychological impacts on financial markets 194 weather derivatives 194 Weeden, O. 229, 245 weighted least squares (WLS) 150–1 problems with 151–2 Weil, D. 42 Whelan, K. 203, 223 white noise, see stochastic error White’s test 147–9, 154 Wilson, C. M., marriage and health 257, 262 within transformation 258 Wood, R., hedonic pricing 114, 115, 132 Wooldridge, J.M. 32, 155, 186, 188, 196, 257, 258, 262, 267, 273, 274, 277, 278 World Bank 279 data on income groups 267, 271 poverty indicator 60 World Development Indicators 93, 106 World Economic Forum, and global poverty 39 World Health Organisation (WHO) 93, 106 World Travel and Tourism Council (WTTC) 157 Wright, S. 185, 196 

Yang, S. 201, 223 

zones of indecision 169 Zuckerberg, Mark, and Facebook 206 