

<!-- === Source: MinerU_markdown_Analysis_I_-_By_Terence_Tao_1_2122707919320489999.md (Page 1) === -->

# Terence Tao

## Analysis I

Third Edition 

# Texts and Readings in Mathematics

Volume 37 

Advisory Editor 

C.S. Seshadri, Chennai Mathematical Institute, Chennai 

Managing Editor 

Rajendra Bhatia, Indian Statistical Institute, New Delhi 

## Editor

Manindra Agrawal, Indian Institute of Technology Kanpur, Kanpur 

V. Balaji, Chennai Mathematical Institute, Chennai 

R.B. Bapat, Indian Statistical Institute, New Delhi 

V.S. Borkar, Indian Institute of Technology Bombay, Mumbai 

T.R. Ramadas, Chennai Mathematical Institute, Chennai 

V. Srinivas, Tata Institute of Fundamental Research, Mumba 

The Texts and Readings in Mathematics series publishes high-quality textbooks, research-level monographs, lecture notes and contributed volumes. Undergraduate and graduate students of mathematics, research scholars, and teachers would find this book series useful. The volumes are carefully written as teaching aids and highlight characteristic features of the theory. The books in this series are co-published with Hindustan Book Agency, New Delhi, India. 

More information about this series at http://www.springer.com/series/15141 

Terence Tao 

Analysis I 

Third Edition 

Terence Tao Department of Mathematics University of California, Los Angeles Los Angeles, CA USA 

This work is a co-publication with Hindustan Book Agency, New Delhi, licensed for sale in all countries in electronic form only. Sold and distributed in print across the world by Hindustan Book Agency, P-19 Green Park Extension, New Delhi 110016, India. ISBN: 978-93-80250-64-9 © Hindustan Book Agency 2015. 

ISSN 2366-8725 (electronic) Texts and Readings in Mathematics ISBN 978-981-10-1789-6 (eBook) DQI 10.1007/978-981-10-1789-6 

Library of Congress Control Number: 2016940817 

© Springer Science+Business Media Singapore 2016 and Hindustan Book Agency 2015 

This work is subject to copyright. All rights are reserved by the Publishers, whether the whole or part of the material is concerned, specifically the rights of translation, reprinting, reuse of illustrations, recitation, broadcasting, reproduction on microfilms or in any other physical way, and transmission or information storage and retrieval, electronic adaptation, computer software, or by similar or dissimilar methodology now known or hereafter developed. 

The use of general descriptive names, registered names, trademarks, service marks, etc. in this publication does not imply, even in the absence of a specific statement, that such names are exempt from the relevant protective laws and regulations and therefore free for general use. 

The publishers, the authors and the editors are safe to assume that the advice and information in this book are believed to be true and accurate at the date of publication. Neither the publishers nor the authors or the editors give a warranty, express or implied, with respect to the material contained herein or for any errors or omissions that may have been made. 

This Springer imprint is published by Springer Nature 

The registered company is Springer Science+Business Media Singapore Pte Ltd. 

To my parents, for everything 

## Contents

Preface to the second and third editions xi  
Preface to the first edition xiii  
About the Author xix  
1 Introduction 1  
1.1 What is analysis? 1  
1.2 Why do analysis? 2  
2 Starting at the beginning: the natural numbers 13  
2.1 The Peano axioms 15  
2.2 Addition 24  
2.3 Multiplication 29  
3 Set theory 33  
3.1 Fundamentals 33  
3.2 Russell's paradox (Optional) 46  
3.3 Functions 49  
3.4 Images and inverse images 56  
3.5 Cartesian products 62  
3.6 Cardinality of sets 67  
4 Integers and rationals 74  
4.1 The integers 74  
4.2 The rationals 81  
4.3 Absolute value and exponentiation 86  
4.4 Gaps in the rational numbers 90  
5 The real numbers 94  
5.1 Cauchy sequences 96  
5.2 Equivalent Cauchy sequences 100  
5.3 The construction of the real numbers 102  
5.4 Ordering the reals 111 

5.5 The least upper bound property . . . . . . . . . . . . . . . . . . . . . 116
5.6 Real exponentiation, part I . . . . . . . . . . . . . . . . . . . 121

6 Limits of sequences 126
6.1 Convergence and limit laws . . . . . . . . . . . . . . . . . . 126
6.2 The Extended real number system . . . . . . . . . . . . . . 133
6.3 Suprema and Infima of sequences . . . . . . . . . . . . . 137
6.4 Limsup, Liminf, and limit points . . . . . . . . . 139
6.5 Some standard limits . . . . . . . . . . . 148
6.6 Subsequences . . . . . . . 149
6.7 Real exponentiation, part II 152

7 Series 155
7.1 Finite series 155
7.2 Infinite series 164
7.3 Sums of non-negative numbers 170
7.4 Rearrangement of series 174
7.5 The root and ratio tests 178

8 Infinite sets 181
8.1 Countability 181
8.2 Summation on infinite sets 188
8.3 Uncountable sets 195
8.4 The axiom of choice 198
8.5 Ordered sets 202

9 Continuous functions on R 211
9.1 Subsets of the real line 211
9.2 The algebra of real-valued functions 217
9.3 Limiting values of functions 220
9.4 Continuous functions 227
9.5 Left and right limits 231
9.6 The maximum principle 234
9.7 The intermediate value theorem 238
9.8 Monotonic functions 241
9.9 Uniform continuity 243
9.10 Limits at infinity 249

10 Differentiation of functions 251
10.1 Basic definitions 251 

10.2 Local maxima, local minima, and derivatives . . . . . . . 257
10.3 Monotone functions and derivatives . . . . . . . . . 260
10.4 Inverse functions and derivatives . . . . . . . . . . 261
10.5 L'Hôpital's rule . . . . . . . . . . . . . . 264

11 The Riemann integral 267
11.1 Partitions . . . . . . . . . . . . . . 268
11.2 Piecewise constant functions . . . . . . . . . . 272
11.3 Upper and lower Riemann integrals . . . . . . . . 276
11.4 Basic properties of the Riemann integral . . . . . . 280
11.5 Riemann integrability of continuous functions . . . . 285
11.6 Riemann integrability of monotone functions . . . . 289
11.7 A non-Riemann integrable function . . . . 291
11.8 The Riemann-Stieltjes integral . . . . 292
11.9 The two fundamental theorems of calculus . 295
11.10 Consequences of the fundamental theorems . 300

A Appendix: the basics of mathematical logic 305
A.1 Mathematical statements . 306
A.2 Implication . 312
A.3 The structure of proofs . 317
A.4 Variables and quantifiers . 320
A.5 Nested quantifiers . 324
A.6 Some examples of proofs and quantifiers . 327
A.7 Equality . 329

B Appendix: the decimal system 331
B.1 The decimal representation of natural numbers . 332
B.2 The decimal representation of real numbers . 335

Index 339

Texts and Readings in Mathematics 349 

# Preface to the second and third editions

Since the publication of the first edition, many students and lecturers have communicated a number of minor typos and other corrections to me. There was also some demand for a hardcover edition of the texts. Because of this, the publishers and I have decided to incorporate the corrections and issue a hardcover second edition of the textbooks. The layout, page numbering, and indexing of the texts have also been changed; in particular the two volumes are now numbered and indexed separately. However, the chapter and exercise numbering, as well as the mathematical content, remains the same as the first edition, and so the two editions can be used more or less interchangeably for homework and study purposes. 

The third edition contains a number of corrections that were reported for the second edition, together with a few new exercises, but is otherwise essentially the same text. 

# Preface to the first edition

This text originated from the lecture notes I gave teaching the honours undergraduate-level real analysis sequence at the University of California, Los Angeles, in 2003. Among the undergraduates here, real analysis was viewed as being one of the most dificult courses to learn, not only because of the abstract concepts being introduced for the first time (e.g., topology, limits, measurability, etc.), but also because of the level of rigour and proof demanded of the course. Because of this perception of dificulty, one was often faced with the dificult choice of either reducing the level of rigour in the course in order to make it easier, or to maintain strict standards and face the prospect of many undergraduates, even many of the bright and enthusiastic ones, struggling with the course material. 

Faced with this dilemma, I tried a somewhat unusual approach to the subject. Typically, an introductory sequence in real analysis assumes that the students are already familiar with the real numbers, with mathematical induction, with elementary calculus, and with the basics of set theory, and then quickly launches into the heart of the subject, for instance the concept of a limit. Normally, students entering this sequence do indeed have a fair bit of exposure to these prerequisite topics, though in most cases the material is not covered in a thorough manner. For instance, very few students were able to actually define a real number, or even an integer, properly, even though they could visualize these numbers intuitively and manipulate them algebraically. This seemed to me to be a missed opportunity. Real analysis is one of the first subjects (together with linear algebra and abstract algebra) that a student encounters, in which one truly has to grapple with the subtleties of a truly rigorous mathematical proof. As such, the course ofered an excellent chance to go back to the foundations of mathematics, and in particular the opportunity to do a proper and thorough construction of the real numbers. 

Thus the course was structured as follows. In the first week, I described some well-known “paradoxes” in analysis, in which standard laws of the subject (e.g., interchange of limits and sums, or sums and integrals) were applied in a non-rigorous way to give nonsensical results such $\mathrm { a s } 0 = 1$ . This motivated the need to go back to the very beginning of the subject, even to the very definition of the natural numbers, and check all the foundations from scratch. For instance, one of the first homework assignments was to check (using only the Peano axioms) that addition was associative for natural numbers (i.e., that $( a + b ) + c = a + ( b + c )$ for all natural numbers $a , b , c \mathrm { : }$ see Exercise 2.2.1). Thus even in the first week, the students had to write rigorous proofs using mathematical induction. After we had derived all the basic properties of the natural numbers, we then moved on to the integers (initially defined as formal diferences of natural numbers); once the students had verified all the basic properties of the integers, we moved on to the rationals (initially defined as formal quotients of integers); and then from there we moved on (via formal limits of Cauchy sequences) to the reals. Around the same time, we covered the basics of set theory, for instance demonstrating the uncountability of the reals. Only then (after about ten lectures) did we begin what one normally considers the heart of undergraduate real analysis - limits, continuity, diferentiability, and so forth. 

The response to this format was quite interesting. In the first few weeks, the students found the material very easy on a conceptual level, as we were dealing only with the basic properties of the standard number systems. But on an intellectual level it was very challenging, as one was analyzing these number systems from a foundational viewpoint, in order to rigorously derive the more advanced facts about these number systems from the more primitive ones. One student told me how dificult it was to explain to his friends in the non-honours real analysis sequence (a) why he was still learning how to show why all rational numbers are either positive, negative, or zero (Exercise 4.2.4), while the nonhonours sequence was already distinguishing absolutely convergent and conditionally convergent series, and (b) why, despite this, he thought his homework was significantly harder than that of his friends. Another student commented to me, quite wryly, that while she could obviously see why one could always divide a natural number n into a positive integer $q$ to give a quotient a and a remainder r less than $q$ (Exercise 2.3.5), she still had, to her frustration, much dificulty in writing down a proof of this fact. (I told her that later in the course she would have to prove statements for which it would not be as obvious to see that the statements were true; she did not seem to be particularly consoled by this.) Nevertheless, these students greatly enjoyed the homework, as when they did perservere and obtain a rigorous proof of an intuitive fact, it solidified the link in their minds between the abstract manipulations of formal mathematics and their informal intuition of mathematics (and of the real world), often in a very satisfying way. By the time they were assigned the task of giving the infamous “epsilon and delta” proofs in real analysis, they had already had so much experience with formalizing intuition, and in discerning the subtleties of mathematical logic (such as the distinction between the “for all” quantifier and the “there exists” quantifier), that the transition to these proofs was fairly smooth, and we were able to cover material both thoroughly and rapidly. By the tenth week, we had caught up with the non-honours class, and the students were verifying the change of variables formula for Riemann-Stieltjes integrals, and showing that piecewise continuous functions were Riemann integrable. By the conclusion of the sequence in the twentieth week, we had covered (both in lecture and in homework) the convergence theory of Taylor and Fourier series, the inverse and implicit function theorem for continuously diferentiable functions of several variables, and established the dominated convergence theorem for the Lebesgue integral. 

In order to cover this much material, many of the key foundational results were left to the student to prove as homework; indeed, this was an essential aspect of the course, as it ensured the students truly appreciated the concepts as they were being introduced. This format has been retained in this text; the majority of the exercises consist of proving lemmas, propositions and theorems in the main text. Indeed, I would strongly recommend that one do as many of these exercises as possible - and this includes those exercises proving “obvious” statements - if one wishes to use this text to learn real analysis; this is not a subject whose subtleties are easily appreciated just from passive reading. Most of the chapter sections have a number of exercises, which are listed at the end of the section. 

To the expert mathematician, the pace of this book may seem somewhat slow, especially in early chapters, as there is a heavy emphasis on rigour (except for those discussions explicitly marked “Informal”), and justifying many steps that would ordinarily be quickly passed over as being self-evident. The first few chapters develop (in painful detail) many of the “obvious” properties of the standard number systems, for instance that the sum of two positive real numbers is again positive (Exercise 5.4.1), or that given any two distinct real numbers, one can find rational number between them (Exercise 5.4.5). In these foundationa chapters, there is also an emphasis on non-circularity - not using later, more advanced results to prove earlier, more primitive ones. In particular, the usual laws of algebra are not used until they are derived (and they have to be derived separately for the natural numbers, integers, rationals, and reals). The reason for this is that it allows the students to learn the art of abstract reasoning, deducing true facts from a limited set of assumptions, in the friendly and intuitive setting of number systems; the payof for this practice comes later, when one has to utilize the same type of reasoning techniques to grapple with more advanced concepts (e.g., the Lebesgue integral). 

The text here evolved from my lecture notes on the subject, and thus is very much oriented towards a pedagogical perspective; much of the key material is contained inside exercises, and in many cases I have chosen to give a lengthy and tedious, but instructive, proof instead of a slick abstract proof. In more advanced textbooks, the student will see shorter and more conceptually coherent treatments of this material, and with more emphasis on intuition than on rigour; however, I feel it is important to know how to do analysis rigorously and “by hand” first, in order to truly appreciate the more modern, intuitive and abstract approach to analysis that one uses at the graduate level and beyond. 

The exposition in this book heavily emphasizes rigour and formalism; however this does not necessarily mean that lectures based on this book have to proceed the same way. Indeed, in my own teaching I have used the lecture time to present the intuition behind the concepts (drawing many informal pictures and giving examples), thus providing a complementary viewpoint to the formal presentation in the text. The exercises assigned as homework provide an essential bridge between the two, requiring the student to combine both intuition and formal understanding together in order to locate correct proofs for a problem. This I found to be the most dificult task for the students, as it requires the subject to be genuinely learnt, rather than merely memorized or vaguely absorbed. Nevertheless, the feedback I received from the students was that the homework, while very demanding for this reason, was also very rewarding, as it allowed them to connect the rather abstract manipulations of formal mathematics with their innate intuition on such basic concepts as numbers, sets, and functions. Of course, the aid of a good teaching assistant is invaluable in achieving this connection. 

With regard to examinations for a course based on this text, I would recommend either an open-book, open-notes examination with problems similar to the exercises given in the text (but perhaps shorter, with no unusual trickery involved), or else a take-home examination that involves problems comparable to the more intricate exercises in the text. The subject matter is too vast to force the students to memorize the definitions and theorems, so I would not recommend a closed-book examination, or an examination based on regurgitating extracts from the book. (Indeed, in my own examinations I gave a supplemental sheet listing the key definitions and theorems which were relevant to the examination problems.) Making the examinations similar to the homework assigned in the course will also help motivate the students to work through and understand their homework problems as thoroughly as possible (as opposed to, say, using flash cards or other such devices to memorize material), which is good preparation not only for examinations but for doing mathematics in general. 

Some of the material in this textbook is somewhat peripheral to the main theme and may be omitted for reasons of time constraints. For instance, as set theory is not as fundamental to analysis as are the number systems, the chapters on set theory (Chapters 3, 8) can be covered more quickly and with substantially less rigour, or be given as reading assignments. The appendices on logic and the decimal system are intended as optional or supplemental reading and would probably not be covered in the main course lectures; the appendix on logic is particularly suitable for reading concurrently with the first few chapters. Also, Chapter 11.27 (on Fourier series) is not needed elsewhere in the text and can be omitted. 

For reasons of length, this textbook has been split into two volumes. The first volume is slightly longer, but can be covered in about thirty lectures if the peripheral material is omitted or abridged. The second volume refers at times to the first, but can also be taught to students who have had a first course in analysis from other sources. It also takes about thirty lectures to cover. 

I am deeply indebted to my students, who over the progression of the real analysis course corrected several errors in the lectures notes from which this text is derived, and gave other valuable feedback. I am also very grateful to the many anonymous referees who made several corrections and suggested many important improvements to the text. 



I also thank Biswaranjan Behera, Tai-Danae Bradley, Brian, Eduardo Buscicchio, Carlos, EO, Florian, G¨okhan G¨u¸cl¨u, Evangelos Georgiadis, Ulrich Groh, Bart Kleijngeld, Erik Koelink, Wang Kuyyang, Matthis Lehmk¨uhler, Percy Li, Ming Li, Jason M., Manoranjan Majji, Geof Mess, Pieter Naaijkens, Vineet Nair, Cristina Pereyra, David Radnell, Tim Reijnders, Pieter Rofelsen, Luke Rogers, Marc Schoolderman, Kent Van Vels, Daan Wanrooy, Yandong Xiao, Sam Xu, Luqing Ye, and the students of Math 401/501 and Math 402/502 at the University of New Mexico for corrections to the first and second editions. 



Terence Tao 

## About the Author

Terence Tao, FAA FRS, is an Australian mathematician. His areas of interests are in harmonic analysis, partial differential equations, algebraic combinatorics, arithmetic combinatorics, geometric combinatorics, compressed sensing and analytic number theory. As of 2015, he holds the James and Carol Collins chair in mathematics at the University of California, Los Angeles. Professor Tao is a co-recipient of the 2006 Fields Medal and the 2014 Breakthrough Prize in Mathematics. He maintains a personal mathematics blog, which has been described by Timothy Gowers as “the undisputed king of all mathematics blogs”. 

## Chapter 1

## Introduction

## 1.1 What is analysis?

This text is an honours-level undergraduate introduction to real analysis: the analysis of the real numbers, sequences and series of real numbers, and real-valued functions. This is related to, but is distinct from, complex analysis, which concerns the analysis of the complex numbers and complex functions, harmonic analysis, which concerns the analysis of harmonics (waves) such as sine waves, and how they synthesize other functions via the Fourier transform, functional analysis, which focuses much more heavily on functions (and how they form things like vector spaces), and so forth. Analysis is the rigorous study of such objects, with a focus on trying to pin down precisely and accurately the qualitative and quantitative behavior of these objects. Real analysis is the theoretical foundation which underlies calculus, which is the collection of computational algorithms which one uses to manipulate functions. 

In this text we will be studying many objects which will be familiar to you from freshman calculus: numbers, sequences, series, limits, functions, definite integrals, derivatives, and so forth. You already have a great deal of experience of computing with these objects; however here we will be focused more on the underlying theory for these objects. We will be concerned with questions such as the following: 

1. What is a real number? Is there a largest real number? After 0, what is the “next” real number (i.e., what is the smallest positive real number)? Can you cut a real number into pieces infinitely many times? Why does a number such as 2 have a square root, while a number such as -2 does not? If there are infinitely many reals and infinitely many rationals, how come there are “more” real numbers than rational numbers? 

2. How do you take the limit of a sequence of real numbers? Which sequences have limits and which ones don’t? If you can stop a sequence from escaping to infinity, does this mean that it must eventually settle down and converge? Can you add infinitely many real numbers together and still get a finite real number? Can you add infinitely many rational numbers together and end up with a non-rational number? If you rearrange the elements of an infinite sum, is the sum still the same? 

3. What is a function? What does it mean for a function to be continuous? diferentiable? integrable? bounded? Can you add infinitely many functions together? What about taking limits of sequences of functions? Can you diferentiate an infinite series of functions? What about integrating? If a function f(x) takes the value 3 when $x = 0$ and 5 when x = 1 (i.e., $f ( 0 ) = 3$ and $f ( 1 ) = 5 )$ , does it have to take every intermediate value between 3 and 5 when x goes between 0 and 1? Why? 

You may already know how to answer some of these questions from your calculus classes, but most likely these sorts of issues were only of secondary importance to those courses; the emphasis was on getting you to perform computations, such as computing the integral of x sin $( x ^ { 2 } )$ from x = 0 to x = 1. But now that you are comfortable with these objects and already know how to do all the computations, we will go back to the theory and try to really understand what is going on. 

## 1.2 Why do analysis?

It is a fair question to ask, “why bother?”, when it comes to analysis. There is a certain philosophical satisfaction in knowing why things work, but a pragmatic person may argue that one only needs to know how things work to do real-life problems. The calculus training you receive in introductory classes is certainly adequate for you to begin solving many problems in physics, chemistry, biology, economics, computer science, finance, engineering, or whatever else you end up doing - and you can certainly use things like the chain rule, L’Hˆopital’s rule, or integration by parts without knowing why these rules work, or whether there are any exceptions to these rules. However, one can get into trouble if 

## 1.2. Why do analysis?

one applies rules without knowing where they came from and what the limits of their applicability are. Let me give some examples in which several of these familiar rules, if applied blindly without knowledge of the underlying analysis, can lead to disaster. 

Example 1.2.1 (Division by zero). This is a very familiar one to you: the cancellation law $a c = b c \implies a = b$ does not work when $c = 0$ . For instance, the identity $1 \times 0 = 2 \times 0$ is true, but if one blindly cancels the 0 then one obtains $1 = 2$ , which is false. In this case it was obvious that one was dividing by zero; but in other cases it can be more hidden. 

Example 1.2.2 (Divergent series). You have probably seen geometric series such as the infinite sum 

$$
S = 1 + \frac {1}{2} + \frac {1}{4} + \frac {1}{8} + \frac {1}{1 6} + \dots .
$$

You have probably seen the following trick to sum this series: if we call the above sum S, then if we multiply both sides by 2, we obtain 

$$
2 S = 2 + 1 + \frac {1}{2} + \frac {1}{4} + \frac {1}{8} + \dots = 2 + S
$$

and hence $S = 2$ , so the series sums to 2. However, if you apply the same trick to the series 

$$
S = 1 + 2 + 4 + 8 + 1 6 + \ldots
$$

one gets nonsensical results: 

$$
2 S = 2 + 4 + 8 + 1 6 + \dots = S - 1 \implies S = - 1.
$$

So the same reasoning that shows that $1 + { \textstyle { \frac { 1 } { 2 } } } + { \textstyle { \frac { 1 } { 4 } } } + \dots = 2$ also gives that $1 + 2 + 4 + 8 + \ldots = - 1$ . Why is it that we trust the first equation but not the second? A similar example arises with the series 

$$
S = 1 - 1 + 1 - 1 + 1 - 1 + \ldots ;
$$

we can write 

$$
S = 1 - (1 - 1 + 1 - 1 + \dots) = 1 - S
$$

and hence that $S = 1 / 2$ ; or instead we can write 

$$
S = (1 - 1) + (1 - 1) + (1 - 1) + \dots = 0 + 0 + \dots
$$

and hence that $S = 0 ;$ or instead we can write 

$$
S = 1 + (- 1 + 1) + (- 1 + 1) + \dots = 1 + 0 + 0 + \dots
$$

and hence that $S = 1$ . Which one is correct? (See Exercise 7.2.1 for an answer.) 

Example 1.2.3 (Divergent sequences). Here is a slight variation of the previous example. Let x be a real number, and let $L$ be the limit 

$$
L = \lim _ {n \to \infty} x ^ {n}.
$$

Changing variables $n = m + 1$ , we have 

$$
L = \lim _ {m + 1 \to \infty} x ^ {m + 1} = \lim _ {m + 1 \to \infty} x \times x ^ {m} = x \lim _ {m + 1 \to \infty} x ^ {m}.
$$

But if $m + 1  \infty$ , then $m \to \infty$ , thus 

$$
\lim _ {m + 1 \to \infty} x ^ {m} = \lim _ {m \to \infty} x ^ {m} = \lim _ {n \to \infty} x ^ {n} = L,
$$

and thus 

$$
x L = L.
$$

At this point we could cancel the $L \mathrm { { s } }$ and conclude that $x = 1$ for an arbitrary real number $x ,$ , which is absurd. But since we are already aware of the division by zero problem, we could be a little smarter and conclude instead that either $x = 1$ , or $L = 0$ . In particular we seem to have shown that 

$$
\lim _ {n \to \infty} x ^ {n} = 0 \mathrm{forall} x \neq 1.
$$

But this conclusion is absurd if we apply it to certain values of $x ,$ , for instance by specializing to the case $x = 2$ we could conclude that the sequence $1 , 2 , 4 , 8 , \ldots$ converges to zero, and by specializing to the case $x = - 1$ we conclude that the sequence $1 , - 1 , 1 , - 1 , \ldots$ . also converges to zero. These conclusions appear to be absurd; what is the problem with the above argument? (See Exercise 6.3.4 for an answer.) 

Example 1.2.4 (Limiting values of functions). Start with the expression $\scriptstyle \operatorname* { l i m } _ { x \to \infty } \sin ( x )$ , make the change of variable $x = y + \pi$ and recall that sin $( y + \pi ) = - \sin ( y )$ to obtain 

$$
\lim _ {x \to \infty} \sin (x) = \lim _ {y + \pi \to \infty} \sin (y + \pi) = \lim _ {y \to \infty} (- \sin (y)) = - \lim _ {y \to \infty} \sin (y).
$$

## 1.2. Why do analysis?

Since $\begin{array} { r } { \operatorname* { l i m } _ { x  \infty } \sin ( x ) = \operatorname* { l i m } _ { y  \infty } \sin ( y ) } \end{array}$ we thus have 

$$
\lim _ {x \to \infty} \sin (x) = - \lim _ {x \to \infty} \sin (x)
$$

and hence 

$$
\lim _ {x \to \infty} \sin (x) = 0.
$$

If we then make the change of variables $x = \pi / 2 + z$ and recall that sin $( \pi / 2 + z ) = \cos ( z )$ we conclude that 

$$
\lim _ {x \to \infty} \cos (x) = 0.
$$

Squaring both of these limits and adding we see that 

$$
\lim _ {x \to \infty} (\sin^ {2} (x) + \cos^ {2} (x)) = 0 ^ {2} + 0 ^ {2} = 0.
$$

On the other hand, we have si $\mathrm { n } ^ { 2 } ( x ) + \cos ^ { 2 } ( x ) = 1$ for all x. Thus we have shown that 1 = 0! What is the dificulty here? 

Example 1.2.5 (Interchanging sums). Consider the following fact of arithmetic. Consider any matrix of numbers, e.g. 

$$
\left( \begin{array}{c c c} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{array} \right)
$$

and compute the sums of all the rows and the sums of all the columns, and then total all the row sums and total all the column sums. In both cases you will get the same number - the total sum of all the entries in the matrix: 

$$
\left( \begin{array}{c c c} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \\ 1 2 & 1 5 & 1 8 \end{array} \right) \quad \begin{array}{c} 6 \\ 1 5 \\ 2 4 \\ 4 5 \end{array}
$$

To put it another way, if you want to add all the entries in an $m \times n$ matrix together, it doesn’t matter whether you sum the rows first or sum the columns first, you end up with the same answer. (Before the invention of computers, accountants and book-keepers would use this fact to guard against making errors when balancing their books.) In series notation, this fact would be expressed as 

$$
\sum_ {i = 1} ^ {m} \sum_ {j = 1} ^ {n} a _ {i j} = \sum_ {j = 1} ^ {n} \sum_ {i = 1} ^ {m} a _ {i j},
$$

if $a _ { i j }$ denoted the entry in the $i ^ { t h }$ row and $j ^ { t h }$ column of the matrix. 

Now one might think that this rule should extend easily to infinite series: 

$$
\sum_ {i = 1} ^ {\infty} \sum_ {j = 1} ^ {\infty} a _ {i j} = \sum_ {j = 1} ^ {\infty} \sum_ {i = 1} ^ {\infty} a _ {i j}.
$$

Indeed, if you use infinite series a lot in your work, you will find yourself having to switch summations like this fairly often. Another way of saying this fact is that in an infinite matrix, the sum of the row-totals should equal the sum of the column-totals. However, despite the reasonableness of this statement, it is actually false! Here is a counterexample: 

$$
\left( \begin{array}{c c c c c} 1 & 0 & 0 & 0 & \ldots \\ - 1 & 1 & 0 & 0 & \ldots \\ 0 & - 1 & 1 & 0 & \ldots \\ 0 & 0 & - 1 & 1 & \ldots \\ 0 & 0 & 0 & - 1 & \ldots \\ \vdots & \vdots & \vdots & \vdots & \ddots \end{array} \right).
$$

If you sum up all the rows, and then add up all the row totals, you get 1; but if you sum up all the columns, and add up all the column totals, you get 0! So, does this mean that summations for infinite series should not be swapped, and that any argument using such a swapping should be distrusted? (See Theorem 8.2.2 for an answer.) 

Example 1.2.6 (Interchanging integrals). The interchanging of integrals is a trick which occurs in mathematics just as commonly as the interchanging of sums. Suppose one wants to compute the volume under a surface $z = f ( x , y )$ (let us ignore the limits of integration for the moment). One can do it by slicing parallel to the x-axis: for each fixed value of $y ,$ we can compute an area $\textstyle \int f ( x , y )$ dx, and then we integrate the area in the $y$ variable to obtain the volume 

$$
V = \int \int f (x, y) d x d y.
$$

Or we could slice parallel to the y-axis for each fixed x and compute an area $\textit { \textbf { f } } f ( x , y ) \ d y$ , and then integrate in the x-axis to obtain 

$$
V = \int \int f (x, y) d y d x.
$$

This seems to suggest that one should always be able to swap integral signs: 

$$
\int \int f (x, y) d x d y = \int \int f (x, y) d y d x.
$$

And indeed, people swap integral signs all the time, because sometimes one variable is easier to integrate in first than the other. However, just as infinite sums sometimes cannot be swapped, integrals are also sometimes dangerous to swap. An example is with the integrand $e ^ { - x y } - x y e ^ { - x y }$ Suppose we believe that we can swap the integrals: 

$$
\int_ {0} ^ {\infty} \int_ {0} ^ {1} (e ^ {- x y} - x y e ^ {- x y}) d y d x = \int_ {0} ^ {1} \int_ {0} ^ {\infty} (e ^ {- x y} - x y e ^ {- x y}) d x d y.\tag{1.1}
$$

Since 

$$
\int_ {0} ^ {1} \left(e ^ {- x y} - x y e ^ {- x y}\right) d y = y e ^ {- x y} | _ {y = 0} ^ {y = 1} = e ^ {- x},
$$

the left-hand side of (1.1) is $\begin{array} { r } { \int _ { 0 } ^ { \infty } e ^ { - x } \ d x = - e ^ { - x } | _ { 0 } ^ { \infty } = 1 } \end{array}$ . But since 

$$
\int_ {0} ^ {\infty} \left(e ^ {- x y} - x y e ^ {- x y}\right) d x = x e ^ {- x y} | _ {x = 0} ^ {x = \infty} = 0,
$$

the right-hand side of (1.1) is $\textstyle \int _ { 0 } ^ { 1 } 0 \ d x = 0$ . Clearly $1 \neq 0$ , so there is an error somewhere; but you won’t find one anywhere except in the step where we interchanged the integrals. So how do we know when to trust the interchange of integrals? (See Theorem 11.50.1 for a partial answer.) 

Example 1.2.7 (Interchanging limits). Suppose we start with the plausible looking statement 

$$
\lim _ {x \to 0} \lim _ {y \to 0} \frac {x ^ {2}}{x ^ {2} + y ^ {2}} = \lim _ {y \to 0} \lim _ {x \to 0} \frac {x ^ {2}}{x ^ {2} + y ^ {2}}.\tag{1.2}
$$

But we have 

$$
\lim _ {y \to 0} \frac {x ^ {2}}{x ^ {2} + y ^ {2}} = \frac {x ^ {2}}{x ^ {2} + 0 ^ {2}} = 1,
$$

so the left-hand side of (1.2) is 1; on the other hand, we have 

$$
\lim _ {x \to 0} \frac {x ^ {2}}{x ^ {2} + y ^ {2}} = \frac {0 ^ {2}}{0 ^ {2} + y ^ {2}} = 0,
$$

so the right-hand side of (1.2) is 0. Since 1 is clearly not equal to zero, this suggests that interchange of limits is untrustworthy. But are there any other circumstances in which the interchange of limits is legitimate? (See Exercise 11.9.9 for a partial answer.) 

Example 1.2.8 (Interchanging limits, again). Consider the plausible looking statement 

$$
\lim _ {x \to 1 ^ {-}} \lim _ {n \to \infty} x ^ {n} = \lim _ {n \to \infty} \lim _ {x \to 1 ^ {-}} x ^ {n}
$$

where the notation $x  1 ^ { - }$ means that $x$ is approaching 1 from the left. When x is to the left of 1, then $\scriptstyle \operatorname* { l i m } _ { n \to \infty } x ^ { n } = 0$ , and hence the left-hand side is zero. But we also have $\scriptstyle \operatorname* { l i m } _ { x \to 1 ^ { - } } x ^ { n } = 1$ for all $n _ { \mathrm { : } }$ , and so the right-hand side limit is 1. Does this demonstrate that this type of limit interchange is always untrustworthy? (See Proposition 11.15.3 for an answer.) 

Example 1.2.9 (Interchanging limits and integrals). For any real number $y ,$ we have 

$$
\int_ {- \infty} ^ {\infty} \frac {1}{1 + (x - y) ^ {2}} d x = \arctan (x - y) | _ {x = - \infty} ^ {\infty} = \frac {\pi}{2} - \left(- \frac {\pi}{2}\right) = \pi .
$$

Taking limits as $y  \infty$ , we should obtain 

$$
\int_ {- \infty} ^ {\infty} \lim _ {y \to \infty} \frac {1}{1 + (x - y) ^ {2}} d x = \lim _ {y \to \infty} \int_ {- \infty} ^ {\infty} \frac {1}{1 + (x - y) ^ {2}} d x = \pi .
$$

But for every x, we have lim<sub>y</sub> $\not { D } \to \infty \ \frac { 1 } { 1 + ( x - y ) ^ { 2 } } \ = \ 0$ . So we seem to have concluded that $0 = \pi$ . What was the problem with the above argument? Should one abandon the (very useful) technique of interchanging limits and integrals? (See Theorem 11.18.1 for a partial answer.) 

Example 1.2.10 (Interchanging limits and derivatives). Observe that if $\varepsilon > 0$ , then 

$$
{\frac {d}{d x}} \left({\frac {x ^ {3}}{\varepsilon^ {2} + x ^ {2}}}\right) = {\frac {3 x ^ {2} (\varepsilon^ {2} + x ^ {2}) - 2 x ^ {4}}{(\varepsilon^ {2} + x ^ {2}) ^ {2}}}
$$

## 1.2. Why do analysis?

and in particular that 

$$
\frac {d}{d x} \left(\frac {x ^ {3}}{\varepsilon^ {2} + x ^ {2}}\right) | _ {x = 0} = 0.
$$

Taking limits as $\varepsilon \to 0$ , one might then expect that 

$$
{\frac {d}{d x}} \left({\frac {x ^ {3}}{0 + x ^ {2}}}\right) | _ {x = 0} = 0.
$$

But the right-hand side is $\begin{array} { r } { \frac { d } { d x } x = 1 } \end{array}$ . Does this mean that it is always illegitimate to interchange limits and derivatives? (See Theorem 11.19.1 for an answer.) 

Example 1.2.11 (Interchanging derivatives). Let<sup>1</sup> $f ( x , y )$ be the function $\begin{array} { r } { f ( x , y ) : = \frac { x y ^ { 3 } } { x ^ { 2 } + y ^ { 2 } } } \end{array}$ . A common maneuvre in analysis is to interchange two partial derivatives, thus one expects 

$$
\frac {\partial^ {2} f}{\partial x \partial y} (0, 0) = \frac {\partial^ {2} f}{\partial y \partial x} (0, 0).
$$

But from the quotient rule we have 

$$
{\frac {\partial f}{\partial y}} (x, y) = {\frac {3 x y ^ {2}}{x ^ {2} + y ^ {2}}} - {\frac {2 x y ^ {4}}{(x ^ {2} + y ^ {2}) ^ {2}}}
$$

and in particular 

$$
{\frac {\partial f}{\partial y}} (x, 0) = {\frac {0}{x ^ {2}}} - {\frac {0}{x ^ {4}}} = 0.
$$

Thus 

$$
\frac {\partial^ {2} f}{\partial x \partial y} (0, 0) = 0.
$$

On the other hand, from the quotient rule again we have 

$$
{\frac {\partial f}{\partial x}} (x, y) = {\frac {y ^ {3}}{x ^ {2} + y ^ {2}}} - {\frac {2 x ^ {2} y ^ {3}}{(x ^ {2} + y ^ {2}) ^ {2}}}
$$

and hence 

$$
{\frac {\partial f}{\partial x}} (0, y) = {\frac {y ^ {3}}{y ^ {2}}} - {\frac {0}{y ^ {4}}} = y.
$$

Thus 

$$
\frac {\partial^ {2} f}{\partial y \partial x} (0, 0) = 1.
$$

Since $1 \neq 0$ , we thus seem to have shown that interchange of derivatives is untrustworthy. But are there any other circumstances in which the interchange of derivatives is legitimate? (See Theorem 11.37.4 and Exercise 11.37.1 for some answers.) 

Example 1.2.12 (L’Hˆopital’s rule). We are all familiar with the beautifully simple L’Hˆopital’s rule 

$$
\lim _ {x \to x _ {0}} \frac {f (x)}{g (x)} = \lim _ {x \to x _ {0}} \frac {f ^ {\prime} (x)}{g ^ {\prime} (x)},
$$

but one can still get led to incorrect conclusions if one applies it incorrectly. For instance, applying it to $f ( x ) : = x , g ( x ) : = 1 + x$ , and $x _ { 0 } : = 0$ we would obtain 

$$
\lim _ {x \to 0} \frac {x}{1 + x} = \lim _ {x \to 0} \frac {1}{1} = 1,
$$

but this is the incorrect answer, since lim $\textstyle 1 _ { x \to 0 } { \frac { x } { 1 + x } } = { \frac { 0 } { 1 + 0 } } = 0$ . Of course, all that is going on here is that L’Hˆopital’s rule is only applicable when both $f ( x )$ and $g ( x )$ go to zero as $x  x _ { 0 }$ , a condition which was violated in the above example. But even when $f ( x )$ and $g ( x )$ do go to zero as $x  x _ { 0 }$ there is still a possibility for an incorrect conclusion. For instance, consider the limit 

$$
\lim _ {x \to 0} \frac {x ^ {2} \sin (x ^ {- 4})}{x}.
$$

Both numerator and denominator go to zero as $x \to 0$ , so it seems pretty safe to apply L’Hˆopital’s rule, to obtain 

$$
\begin{array}{r l} \lim _ {x \to 0} \frac {x ^ {2} \sin (x ^ {- 4})}{x} & = \lim _ {x \to 0} \frac {2 x \sin (x ^ {- 4}) - 4 x ^ {- 3} \cos (x ^ {- 4})}{1} \\ & = \lim _ {x \to 0} 2 x \sin (x ^ {- 4}) - \lim _ {x \to 0} 4 x ^ {- 3} \cos (x ^ {- 4}). \end{array}
$$

The first limit converges to zero by the squeeze test (since the function $2 x \sin ( x ^ { - 4 } )$ is bounded above by $2 | x |$ and below by $- 2 | x |$ , both of which go to zero at 0). But the second limit is divergent (because $x ^ { - 3 }$ goes to infinity as $x \to 0$ , and $\cos ( x ^ { - 4 } )$ does not go to zero). So the limit $\begin{array} { r } { \operatorname* { l i m } _ { x \to 0 } \frac { 2 \bar { x } \sin ( x ^ { - 4 } ) - 4 x ^ { - 2 } \cos ( x ^ { - 4 } ) } { 1 } } \end{array}$ diverges. One might then conclude using L’Hˆopital’s rule that $\begin{array} { r } { \operatorname* { l i m } _ { x \to 0 } { \frac { x ^ { 2 } \sin ( x ^ { - 4 } ) } { x } } } \end{array}$ also diverges; however we can 

## 1.2. Why do analysis?

clearly rewrite this limit as $\begin{array} { r } { \operatorname* { l i m } _ { x \to 0 } x \sin ( x ^ { - 4 } ) } \end{array}$ , which goes to zero when $x \to 0$ by the squeeze test again. This does not show that L’Hˆopital’s rule is untrustworthy (indeed, it is quite rigorous; see Section 10.5), but it still requires some care when applied. 

Example 1.2.13 (Limits and lengths). When you learn about integration and how it relates to the area under a curve, you were probably presented with some picture in which the area under the curve was approximated by a bunch of rectangles, whose area was given by a Riemann sum, and then one somehow “took limits” to replace that Riemann sum with an integral, which then presumably matched the actual area under the curve. Perhaps a little later, you learnt how to compute the length of a curve by a similar method - approximate the curve by a bunch of line segments, compute the length of all the line segments, then take limits again to see what you get. 

However, it should come as no surprise by now that this approach also can lead to nonsense if used incorrectly. Consider the right-angled triangle with vertices $( 0 , 0 ) , ( 1 , 0 )$ , and (0, 1), and suppose we wanted to compute the length of the hypotenuse of this triangle. Pythagoras theorem tells us that this hypotenuse has length ${ \sqrt { 2 } } .$ , but suppose for some reason that we did not know about Pythagoras’ theorem, and wanted to compute the length using calculus methods. Well, one way to do so is to approximate the hypotenuse by horizontal and vertica edges. Pick a large number N, and approximate the hypotenuse by a “staircase” consisting of N horizontal edges of equal length, alternating with N vertical edges of equal length. Clearly these edges all have length $1 / N$ , so the total length of the staircase is $2 N / N = 2$ . If one takes limits as N goes to infinity, the staircase clearly approaches the hypotenuse, and so in the limit we should get the length of the hypotenuse. However, as $N \to \infty$ , the limit of 2N/N is 2, not ${ \sqrt { 2 } } .$ , so we have an incorrect value for the length of the hypotenuse. How did this happen? 

The analysis you learn in this text will help you resolve these questions, and will let you know when these rules (and others) are justified, and when they are illegal, thus separating the useful applications of these rules from the nonsense. Thus they can prevent you from making mistakes, and can help you place these rules in a wider context. Moreover, as you learn analysis you will develop an “analytical way of thinking”, which will help you whenever you come into contact with any new rules of mathematics, or when dealing with situations which are not quite covered by the standard rules, For instance, what if your functions are complex-valued instead of real-valued? What if you are working on the sphere instead of the plane? What if your functions are not continuous, but are instead things like square waves and delta functions? What if your functions, or limits of integration, or limits of summation, are occasionally infinite? You will develop a sense of why a rule in mathematics (e.g., the chain rule) works, how to adapt it to new situations, and what its limitations (if any) are; this will allow you to apply the mathematics you have already learnt more confidently and correctly. 

## Chapter 2

## Starting at the beginning: the natural numbers

In this text, we will review the material you have learnt in high schoo and in elementary calculus classes, but as rigorously as possible. To do so we will have to begin at the very basics - indeed, we will go back to the concept of numbers and what their properties are. Of course, you have dealt with numbers for over ten years and you know how to manipulate the rules of algebra to simplify any expression involving numbers, but we will now turn to a more fundamental issue, which is: why do the rules of algebra work at all? For instance, why is it true that $a ( b + c )$ is equal to $a b + a c$ for any three numbers $a , b , c ?$ This is not an arbitrary choice of rule; it can be proven from more primitive, and more fundamental, properties of the number system. This will teach you a new skill - how to prove complicated properties from simpler ones. You will find that even though a statement may be “obvious”, it may not be easy to prove; the material here will give you plenty of practice in doing so, and in the process will lead you to think about why an obvious statement really is obvious. One skill in particular that you will pick up here is the use of mathematical induction, which is a basic tool in proving things in many areas of mathematics. 

So in the first few chapters we will re-acquaint you with various number systems that are used in real analysis. In increasing order of sophistication, they are the natural numbers N; the integers Z; the rationals Q, and the real numbers R. (There are other number systems such as the complex numbers C, but we will not study them until Section 11.26.) The natural numbers $\{ 0 , 1 , 2 , \ldots \}$ are the most primitive of the number systems, but they are used to build the integers, which in turn are used to build the rationals. Furthermore, the rationals are used to build the real numbers, which are in turn used to build the complex numbers. Thus to begin at the very beginning, we must look at the natural numbers. We will consider the following question: how does one actually define the natural numbers? (This is a very diferent question from how to use the natural numbers, which is something you of course know how to do very well. It’s like the diference between knowing how to use, say, a computer, versus knowing how to build that computer.) 

This question is more dificult to answer than it looks. The basic problem is that you have used the natural numbers for so long that they are embedded deeply into your mathematical thinking, and you can make various implicit assumptions about these numbers (e.g., that $a + b$ is always equal to $b + a )$ without even aware that you are doing so; it is dificult to let go and try to inspect this number system as if it is the first time you have seen it. So in what follows I will have to ask you to perform a rather dificult task: try to set aside, for the moment, everything you know about the natural numbers; forget that you know how to count, to add, to multiply, to manipulate the rules of algebra, etc. We will try to introduce these concepts one at a time and identify explicitly what our assumptions are as we go along - and not allow ourselves to use more “advanced” tricks such as the rules of algebra until we have actually proven them. This may seem like an irritating constraint, especially as we will spend a lot of time proving statements which are “obvious”, but it is necessary to do this suspension of known facts to avoid circularity (e.g., using an advanced fact to prove a more elementary fact, and then later using the elementary fact to prove the advanced fact). Also, this exercise will be an excellent way to afirm the foundations of your mathematical knowledge. Furthermore, practicing your proofs and abstract thinking here will be invaluable when we move on to more advanced concepts, such as real numbers, functions, sequences and series, diferentials and integrals, and so forth. In short, the results here may seem trivial, but the journey is much more important than the destination, for now. (Once the number systems are constructed properly, we can resume using the laws of algebra etc. without having to rederive them each time.) 

We will also forget that we know the decimal system, which of course is an extremely convenient way to manipulate numbers, but it is not something which is fundamental to what numbers are. (For instance, one could use an octal or binary system instead of the decimal system, or even the Roman numeral system, and still get exactly the same set of numbers.) Besides, if one tries to fully explain what the decimal number system is, it isn’t as natural as you might think. Why is 00423 the same number as 423, but 32400 isn’t the same number as 324? Why is 123.4444 . . . a real number, while . . . 444.321 is not? And why do we have to carry of digits when adding or multiplying? Why is 0.999 . . . the same number as 1? What is the smallest positive real number? Isn’t it just 0.00 . . . 001? So to set aside these problems, we will not try to assume any knowledge of the decimal system, though we will of course still refer to numbers by their familiar names such as 1,2,3, etc. instead of using other notation such as I,II,III or 0++, (0++)++, ((0++)++)++ (see below) so as not to be needlessly artificial. For completeness, we review the decimal system in an Appendix ( B). 

## 2.1 The Peano axioms

We now present one standard way to define the natural numbers, in terms of the Peano axioms, which were first laid out by Guiseppe Peano (1858–1932). This is not the only way to define the natural numbers. For instance, another approach is to talk about the cardinality of finite sets, for instance one could take a set of five elements and define 5 to be the number of elements in that set. We shall discuss this alternate approach in Section 3.6. However, we shall stick with the Peano axiomatic approach for now. 

How are we to define what the natural numbers are? Informally, we could say 

Definition 2.1.1. (Informal) A natural number is any element of the set 

$$
\mathbf {N} := \{0, 1, 2, 3, 4, \dots \},
$$

which is the set of all the numbers created by starting with 0 and then counting forward indefinitely. We call N the set of natural numbers. 

Remark 2.1.2. In some texts the natural numbers start at 1 instead of 0, but this is a matter of notational convention more than anything else. In this text we shall refer to the set 1, 2, 3, . . . as the positive integers $\mathbf { Z } ^ { + }$ rather than the natural numbers. Natural numbers are sometimes also known as whole numbers. 

In a sense, this definition solves the problem of what the natural numbers are: a natural number is any element of the set<sup>1</sup> N. However, it is not really that satisfactory, because it begs the question of what N is. This definition of “start at 0 and count indefinitely” seems like an intuitive enough definition of N, but it is not entirely acceptable, because it leaves many questions unanswered. For instance: how do we know we can keep counting indefinitely, without cycling back to $0 ?$ Also, how do you perform operations such as addition, multiplication, or exponentiation? 

We can answer the latter question first: we can define complicated operations in terms of simpler operations. Exponentiation is nothing more than repeated multiplication: $5 ^ { 3 }$ is nothing more than three fives multiplied together. Multiplication is nothing more than repeated addition; $5 \times 3$ is nothing more than three fives added together. (Subtraction and division will not be covered here, because they are not operations which are well-suited to the natural numbers; they will have to wait for the integers and rationals, respectively.) And addition? It is nothing more than the repeated operation of counting forward, or incrementing. If you add three to five, what you are doing is incrementing five three times. On the other hand, incrementing seems to be a fundamental operation, not reducible to any simpler operation; indeed, it is the first operation one learns on numbers, even before learning to add. 

Thus, to define the natural numbers, we will use two fundamental concepts: the zero number 0, and the increment operation. In deference to modern computer languages, we will use n++ to denote the increment or successor of $n .$ , thus for instance $3 + 1 = 4 , ( 3 { + } + ) { + } = 5$ , etc. This is a slightly diferent usage from that in computer languages such as $C _ { i }$ where n++ actually redefines the value of n to be its successor; however in mathematics we try not to define a variable more than once in any given setting, as it can often lead to confusion; many of the statements which were true for the old value of the variable can now become false, and vice versa. 

So, it seems like we want to say that N consists of 0 and everything which can be obtained from 0 by incrementing: N should consist of the objects 

$$
0, 0 + +, (0 + +) + +, ((0 + +) + +) + +, \text { etc. }
$$

If we start writing down what this means about the natural numbers, we thus see that we should have the following axioms concerning 0 and the increment operation ++: 

Axiom 2.1. 0 is a natural number. 

Axiom 2.2. If n is a natural number, then n++ is also a natural number. 

Thus for instance, from Axiom 2.1 and two applications of Axiom 2.2, we see that (0++)++ is a natural number. Of course, this notation wil begin to get unwieldy, so we adopt a convention to write these numbers in more familiar notation: 

Definition 2.1.3. We define 1 to be the number 0++, 2 to be the number (0++)++, 3 to be the number $( ( 0 + + ) + + ) + +$ , etc. (In other words, $1 : = 0 + + , 2 : = 1 + + , 3 : = 2 + +$ , etc. In this text I use $^ { 6 } x : = y ^ { \dag }$ to denote the statement that x is defined to equal y.) 

Thus for instance, we have 

Proposition 2.1.4. 3 is a natural number. 

Proof. By Axiom 2.1, 0 is a natural number. By Axiom 2.2, 0++ = 1 is a natural number. By Axiom 2.2 again, $1 + + = 2$ is a natural number. By Axiom 2.2 again, $2 { \ + } + = 3$ is a natural number. □ 

It may seem that this is enough to describe the natural numbers. However, we have not pinned down completely the behavior of N: 

Example 2.1.5. Consider a number system which consists of the numbers 0, 1, 2, 3, in which the increment operation wraps back from 3 to 0. More precisely 0++ is equal to 1, 1++ is equal to 2, 2++ is equa to 3, but 3++ is equal to 0 (and also equal to 4, by definition of 4). This type of thing actually happens in real life, when one uses a computer to try to store a natural number: if one starts at 0 and performs the increment operation repeatedly, eventually the computer will overflow its memory and the number will wrap around back to 0 (though this may take quite a large number of incrementation operations, for instance a two-byte representation of an integer will wrap around only after 65, 536 increments). Note that this type of number system obeys Axiom 2.1 and Axiom 2.2, even though it clearly does not correspond to what we intuitively believe the natural numbers to be like. 

To prevent this sort of “wrap-around issue” we will impose another axiom: 

Axiom 2.3. 0 is not the successor of any natural number; i.e., we have $n { + } + \neq 0$ for every natural number n. 

Now we can show that certain types of wrap-around do not occur: for instance we can now rule out the type of behavior in Example 2.1.5 using 

Proposition 2.1.6. 4 is not equal to 0. 

Don’t laugh! Because of the way we have defined 4 - it is the increment of the increment of the increment of the increment of 0 - it is not necessarily true a priori that this number is not the same as zero, even if it is “obvious”. (“a priori” is Latin for “beforehand” - it refers to what one already knows or assumes to be true before one begins a proof or argument. The opposite is “a posteriori” - what one knows to be true after the proof or argument is concluded.) Note for instance that in Example 2.1.5, 4 was indeed equal to 0, and that in a standard twobyte computer representation of a natural number, for instance, 65536 is equal to 0 (using our definition of 65536 as equal to 0 incremented sixty-five thousand, five hundred and thirty-six times). 

Proof. By definition, 4 = 3++. By Axioms 2.1 and 2.2, 3 is a natural number. Thus by Axiom 2.3, 3++ = 0, i.e., 4 = 0. □ 

However, even with our new axiom, it is still possible that our number system behaves in other pathological ways: 

Example 2.1.7. Consider a number system consisting of five numbers 0,1,2,3,4, in which the increment operation hits a “ceiling” at 4. More precisely, suppose that 0++ = 1, 1++ = 2, 2++ = 3, 3++ = 4, but 4++ = 4 (or in other words that 5 = 4, and hence 6 = 4, 7 = 4, etc.). This does not contradict Axioms 2.1,2.2,2.3. Another number system with a similar problem is one in which incrementation wraps around, but not to zero, e.g. suppose that 4++ = 1 (so that 5 = 1, then 6 = 2, etc.). 

There are many ways to prohibit the above types of behavior from happening, but one of the simplest is to assume the following axiom: 

Axiom 2.4. Diferent natural numbers must have diferent successors; i.e., if n, m are natural numbers and n $\neq m$ , then $n { + } + \neq m { + } +$ . Equivalently<sup>2</sup>, if $n { \ + } = m { \ + } +$ , then we must have $n = m$ 

## 2.1. The Peano axioms

Thus, for instance, we have 

Proposition 2.1.8. 6 is not equal to 2. 

Proof. Suppose for sake of contradiction that 6 = 2. Then $5 { + } + = 1 { + } +$ so by Axiom 2.4 we have $5 = 1$ , so that 4++ = 0++. By Axiom 2.4 again we then have 4 = 0, which contradicts our previous proposition. □ 

As one can see from this proposition, it now looks like we can keep all of the natural numbers distinct from each other. There is however still one more problem: while the axioms (particularly Axioms 2.1 and 2.2) allow us to confirm that 0, 1, 2, 3, . . . are distinct elements of N, there is the problem that there may be other “rogue” elements in our number system which are not of this form: 

Example 2.1.9. (Informal) Suppose that our number system N consisted of the following collection of integers and half-integers: 

$$
\mathbf {N} := \{0, 0. 5, 1, 1. 5, 2, 2. 5, 3, 3. 5, \dots \}.
$$

(This example is marked “informal” since we are using real numbers, which we’re not supposed to use yet.) One can check that Axioms 2.1- 2.4 are still satisfied for this set. 

What we want is some axiom which says that the only numbers in N are those which can be obtained from 0 and the increment operation - in order to exclude elements such as 0.5. But it is dificult to quantify what we mean by “can be obtained from” without already using the natural numbers, which we are trying to define. Fortunately, there is an ingenious solution to try to capture this fact: 

Axiom 2.5 (Principle of mathematical induction). Let $P ( n )$ be any property pertaining to a natural number n. Suppose that P(0) is true, and suppose that whenever $P ( n )$ is true, $P ( n { \ + } { + } )$ is also true. Then $P ( n )$ is true for every natural number n. 

Remark 2.1.10. We are a little vague on what “property” means at this point, but some possible examples of $P ( n )$ might be $^ { 6 6 } n$ is even”; “n is equal to 3”; “n solves the equation $( n + 1 ) ^ { 2 } = n ^ { 2 } + 2 n + 1 "$ ; and so forth. Of course we haven’t defined many of these concepts yet, but when we do, Axiom 2.5 will apply to these properties. (A logical remark: Because this axiom refers not just to variables, but also properties, it is of a diferent nature than the other four axioms; indeed, Axiom 2.5 should technically be called an axiom schema rather than an axiom - it is a template for producing an (infinite) number of axioms, rather than being a single axiom in its own right. To discuss this distinction further is far beyond the scope of this text, though, and falls in the realm of logic.) 

The informal intuition behind this axiom is the following. Suppose $P ( n )$ is such that $P ( 0 )$ is true, and such that whenever $P ( n )$ is true, then $P ( n { + } { + } )$ is true. Then since $P ( 0 )$ is true, $P ( 0 + + ) = P ( 1 )$ is true. Since $P ( 1 )$ is true, $P ( 1 + + ) = P ( 2 )$ is true. Repeating this indefinite $\cdot \mathrm { y } ,$ we see that $P ( 0 )$ , P(1), P(2), P(3), etc. are all true - however this line of reasoning will never let us conclude that $P ( 0 . 5 )$ , for instance, is true. Thus Axiom 2.5 should not hold for number systems which contain “unnecessary” elements such as 0.5. (Indeed, one can give a $\mathrm { \ " { p r o o f } } \ '$ of this fact. Apply Axiom 2.5 to the property $P ( n ) = n$ “is not a halfinteger”, i.e., an integer plus 0.5. Then $P ( 0 )$ is true, and if $P ( n )$ is true, then $P ( n { \ + } { + } )$ is true. Thus Axiom 2.5 asserts that $P ( n )$ is true for all natural numbers $n _ { ; }$ i.e., no natural number can be a half-integer. In particular, 0.5 cannot be a natural number. This “proof” is not quite genuine, because we have not defined such notions as “integer”, “halfinteger”, and $^ { 6 6 } 0 . 5 ^ { 5 }$ yet, but it should give you some idea as to how the principle of induction is supposed to prohibit any numbers other than the “true” natural numbers from appearing in N.) 

The principle of induction gives us a way to prove that a property $P ( n )$ is true for every natural number n. Thus in the rest of this text we will see many proofs which have a form like this: 

Proposition 2.1.11. A certain property $P ( n )$ is true for every natural number n. 

Proof. We use induction. We first verify the base case $n = 0 , \mathrm { i . e . }$ ., we prove $P ( 0 )$ . (Insert proof of $P ( 0 )$ here). Now suppose inductively that $n$ is a natural number, and $P ( n )$ has already been proven. We now prove $P ( n { \ + } { + } )$ . (Insert proof of $P ( n { \ + } { + } )$ , assuming that $P ( n )$ is true, here). This closes the induction, and thus $P ( n )$ is true for all numbers n. 

Of course we will not necessarily use the exact template, wording, or order in the above type of proof, but the proofs using induction will generally be something like the above form. There are also some other variants of induction which we shall encounter later, such as backwards induction (Exercise 2.2.6), strong induction (Proposition 2.2.14), and transfinite induction (Lemma 8.5.15). 

Axioms 2.1-2.5 are known as the Peano axioms for the natural numbers. They are all very plausible, and so we shall make 

Assumption 2.6. (Informal) There exists a number system N, whose elements we will call natural numbers, for which Axioms 2.1-2.5 are true. 

We will make this assumption a bit more precise once we have laid down our notation for sets and functions in the next chapter. 

Remark 2.1.12. We will refer to this number system N as the natural number system. One could of course consider the possibility that there is more than one natural number system, e.g., we could have the Hindu-Arabic number system $\{ 0 , 1 , 2 , 3 , . . . \}$ and the Roman number system $\{ O , I , I I , I I I , I V , V , V I , . . . \}$ , and if we really wanted to be annoying we could view these number systems as diferent. But these number systems are clearly equivalent (the technical term is isomorphic), because one can create a one-to-one correspondence $0  O , 1  I , 2  I I$ , etc. which maps the zero of the Hindu-Arabic system with the zero of the Roman system, and which is preserved by the increment operation (e.g., if 2 corresponds to II, then 2++ will correspond to II++). For a more precise statement of this type of equivalence, see Exercise 3.5.13. Since all versions of the natural number system are equivalent, there is no point in having distinct natural number systems, and we will just use a single natural number system to do mathematics. 

We will not prove Assumption 2.6 (though we will eventually include it in our axioms for set theory, see Axiom 3.7), and it will be the only assumption we will ever make about our numbers. A remarkable accomplishment of modern analysis is that just by starting from these five very primitive axioms, and some additional axioms from set theory, we can build all the other number systems, create functions, and do all the algebra and calculus that we are used to. 

Remark 2.1.13. (Informal) One interesting feature about the natural numbers is that while each individual natural number is finite, the set of natural numbers is infinite; i.e., N is infinite but consists of individually finite elements. (The whole is greater than any of its parts.) There are no infinite natural numbers; one can even prove this using Axiom 2.5, provided one is comfortable with the notions of finite and infinite. (Clearly 0 is finite. Also, if n is finite, then clearly n++ is also finite. Hence by Axiom 2.5, all natural numbers are finite.) So the natura numbers can approach infinity, but never actually reach it; infinity is not one of the natural numbers. (There are other number systems which admit “infinite” numbers, such as the cardinals, ordinals, and p-adics, but they do not obey the principle of induction, and in any event are beyond the scope of this text.) 

Remark 2.1.14. Note that our definition of the natural numbers is axiomatic rather than constructive. We have not told you what the natural numbers are (so we do not address such questions as what the numbers are made of, are they physical objects, what do they measure, etc.) - we have only listed some things you can do with them (in fact, the only operation we have defined on them right now is the increment one) and some of the properties that they have. This is how mathematics works - it treats its objects abstractly, caring only about what properties the objects have, not what the objects are or what they mean. If one wants to do mathematics, it does not matter whether a natural number means a certain arrangement of beads on an abacus, or a certain organization of bits in a computer’s memory, or some more abstract concept with no physical substance; as long as you can increment them, see if two of them are equal, and later on do other arithmetic operations such as add and multiply, they qualify as numbers for mathematical purposes (provided they obey the requisite axioms, of course). It is possible to construct the natural numbers from other mathematical objects - from sets, for instance - but there are multiple ways to construct a working model of the natural numbers, and it is pointless, at least from a mathematician’s standpoint, as to argue about which model is the “true” one - as long as it obeys all the axioms and does all the right things, that’s good enough to do maths. 

Remark 2.1.15. Historically, the realization that numbers could be treated axiomatically is very recent, not much more than a hundred years old. Before then, numbers were generally understood to be inextricably connected to some external concept, such as counting the cardinality of a set, measuring the length of a line segment, or the mass of a physical object, etc. This worked reasonably well, until one was forced to move from one number system to another; for instance, understanding numbers in terms of counting beads, for instance, is great for conceptualizing the numbers 3 and 5, but doesn’t work so well for 3 or $1 / 3$ or $\sqrt { 2 }$ or $3 + 4 i$ ; thus each great advance in the theory of numbers - negative numbers, irrational numbers, complex numbers, even the number zero - led to a lot of unnecessary philosophical anguish. 

The great discovery of the late nineteenth century was that numbers can be understood abstractly via axioms, without necessarily needing a concrete model; of course a mathematician can use any of these models when it is convenient, to aid his or her intuition and understanding, but they can also be just as easily discarded when they begin to get in the way. 

One consequence of the axioms is that we can now define sequences recursively. Suppose we want to build a sequence $a _ { 0 } , a _ { 1 } , a _ { 2 } , . . .$ . of numbers by first defining $a _ { 0 }$ to be some base value, $\mathrm { e . g . } , a _ { 0 } : = c$ for some number $c ,$ and then by letting $a _ { 1 }$ be some function of $a _ { 0 } , a _ { 1 } : = f _ { 0 } ( a _ { 0 } )$ 2 $a _ { 2 }$ be some function of $a _ { 1 } , a _ { 2 } : = f _ { 1 } ( a _ { 1 } )$ , and so forth. In general, we set $a _ { n + 1 } : = f _ { n } ( a _ { n } )$ for some function $f _ { n }$ from N to N. By using all the axioms together we will now conclude that this procedure will give a single value to the sequence element $a _ { n }$ for each natural number n. More precisely<sup>3</sup>: 

Proposition 2.1.16 (Recursive definitions). Suppose for each natural number n, we have some function $f _ { n } : \mathbf { N }  \mathbf { N }$ from the natural numbers to the natural numbers. Let c be a natural number. Then we can assign a unique natural number $a _ { n }$ to each natural number n, such that $a _ { 0 } = c$ and $a _ { n + 1 } = f _ { n } ( a _ { n } )$ for each natural number n. 

Proof. (Informal) We use induction. We first observe that this procedure gives a single value to $a _ { 0 }$ , namely $c .$ (None of the other definitions $a _ { n + 1 } : = f _ { n } ( a _ { n } )$ will redefine the value of $a _ { 0 }$ , because of Axiom 2.3.) Now suppose inductively that the procedure gives a single value to $a _ { n }$ . Then it gives a single value to $a _ { n + + }$ , namely $a _ { n + 1 } : = f _ { n } ( a _ { n } )$ (None of the other definitions $a _ { m + 1 } : = f _ { m } ( a _ { m } )$ will redefine the value of $a _ { n + 1 }$ , because of Axiom 2.4.) This completes the induction, and so $a _ { n }$ is defined for each natural number $n .$ , with a single value assigned to each $a _ { n }$ □ 

Note how all of the axioms had to be used here. In a system which had some sort of wrap-around, recursive definitions would not work because some elements of the sequence would constantly be redefined. For instance, in Example 2.1.5, in which $3 { \ + } + = 0$ , then there would be (at least) two conflicting definitions for $a _ { 0 }$ , either c or $f _ { 3 } ( { a } _ { 3 } ) )$ . In a system which had superfluous elements such as 0.5, the element a<sub>0.5</sub> would never be defined. 

Recursive definitions are very powerful; for instance, we can use them to define addition and multiplication, to which we now turn. 

## 2.2 Addition

The natural number system is very bare right now: we have only one operation - increment - and a handful of axioms. But now we can build up more complex operations, such as addition. 

The way it works is the following. To add three to five should be the same as incrementing five three times - this is one increment more than adding two to five, which is one increment more than adding one to five, which is one increment more than adding zero to five, which should just give five. So we give a recursive definition for addition as follows. 

Definition 2.2.1 (Addition of natural numbers). Let m be a natural number. To add zero to $m ,$ we define $0 + m : = m$ . Now suppose inductively that we have defined how to add n to m. Then we can add n++ to m by defining $( n + + ) + m : = ( n + m ) + 1$ 

Thus $0 + m { \mathrm { ~ i s ~ } } m , 1 + m = ( 0 + + ) + m { \mathrm { ~ i s ~ } } m + + ; 2 + m = ( 1 + + ) + m = 0$ $( m + + ) + + ;$ and so forth; for instance we have $2 + 3 = ( 3 + + ) + + =$ $4 + + \ = \ 5 .$ . From our discussion of recursion in the previous section we see that we have defined $n + m$ for every natural number n. Here we are specializing the previous general discussion to the setting where $a _ { n } = n + m$ and $f _ { n } ( a _ { n } ) = a _ { n } + +$ . Note that this definition is asymmetric: $3 + 5$ is incrementing 5 three times, while 5 + 3 is incrementing 3 five times. Of course, they both yield the same value of 8. More generally, it is a fact (which we shall prove shortly) that $a + b = b + a$ for all natural numbers a, b, although this is not immediately clear from the definition. 

Notice that we can prove easily, using Axioms 2.1, 2.2, and induction (Axiom 2.5), that the sum of two natural numbers is again a natural number (why?). 

Right now we only have two facts about addition: that $0 + m = m$ 4 and that $( n + + ) + m = ( n + m ) + +$ . Remarkably, this turns out to be enough to deduce everything else we know about addition. We begin with some basic lemmas<sup>4</sup>. 

Lemma 2.2.2. For any natural number n, $n + 0 = n$ 

Note that we cannot deduce this immediately from $0 + m = m$ because we do not know yet that $a + b = b + a$ 

Proof. We use induction. The base case $0 + 0 = 0$ follows since we know that $0 + m = m$ for every natural number m, and 0 is a natural number. Now suppose inductively that $n + 0 = n .$ . We wish to show that $( n + + ) + 0 = n + +$ . But by definition of addition, $( n { + } + ) { + } 0$ is equal to $( n + 0 ) \mathcal { H }$ , which is equal to n++ since $n + 0 = n$ . This closes the induction. □ 

Lemma 2.2.3. For any natural numbers n and m, $n + ( m + 1 + ) = ( n +$ $m ) { + } +$ 

Again, we cannot deduce this yet from $( n + + ) + m = ( n + m ) + +$ because we do not know yet that $a + b = b + a $ 

Proof. We induct on n (keeping m fixed). We first consider the base case $n = 0$ . In this case we have to prove $0 + ( m { + } + ) = ( 0 + m ) + 1$ But by definition of addition, $0 + ( m { + } + ) = m { + } + { \mathrm { ~ a n d ~ } } 0 + m = m$ , so both sides are equal to m++ and are thus equal to each other. Now we assume inductively that $n + ( m { + } 1 ) = ( n + m ) { + } 1 ;$ ; we now have to show that $\left( n { + } + \right) + \left( m { + } + \right) = \left( \left( n { + } + \right) { + } m \right) { + } +$ . The left-hand side is $( n +$ $( m + + ) ) + +$ by definition of addition, which is equal to $( ( n + m ) { + } + ) { + } +$ by the inductive hypothesis. Similarly, we have $( n + + ) + m = ( n + m ) + 1$ by the definition of addition, and so the right-hand side is also equal to $( ( n + m ) { + } + ) { + } +$ . Thus both sides are equal to each other, and we have closed the induction. □ 

As a particular corollary of Lemma 2.2.2 and Lemma 2.2.3 we see that $n { \mathrel { + } } + = n + 1 \ \mathrm { ( w h y ? ) }$ 

As promised earlier, we can now prove that $a + b = b + a .$ 

Proposition 2.2.4 (Addition is commutative). For any natural numbers n and m, $n + m = m + n$ 

Proof. We shall use induction on n (keeping m fixed). First we do the base case $n = 0$ , i.e., we show $0 + m = m + 0$ . By the definition of addition, $0 + m = m$ , while by Lemma 2.2.2, $m + 0 = m$ . Thus the base case is done. Now suppose inductively that $n + m = m + n$ , now we have to prove that $( n + + ) + m = m + ( n + )$ to close the induction. By the definition of addition, $( n + + ) + m = ( n + m ) + +$ . By Lemma $2 . 2 . 3 , m + ( n + 1 ) = ( m + n ) + 1$ , but this is equal to $( n + m ) { \ + } +$ by the inductive hypothesis $n + m = m + n$ . Thus $( n + + ) + m = m + ( n { + } + )$ and we have closed the induction. □ 

Proposition 2.2.5 (Addition is associative). For any natural numbers $a , b , c ,$ we have $( a + b ) + c = a + ( b + c )$ 

Proof. See Exercise 2.2.1. 

Because of this associativity we can write sums such as $a + b + c$ without having to worry about which order the numbers are being added together. 

Now we develop a cancellation law. 

Proposition 2.2.6 (Cancellation law). Let $a , b , c$ be natural numbers such that $a + b = a + c$ . Then we have $b = c$ 

Note that we cannot use subtraction or negative numbers yet to prove this proposition, because we have not developed these concepts yet. In fact, this cancellation law is crucial in letting us define subtraction (and the integers) later on in this text, because it allows for a sort of “virtual subtraction” even before subtraction is oficially defined. 

Proof. We prove this by induction on a. First consider the base case $a = 0$ . Then we have $0 + b = 0 + c ,$ , which by definition of addition implies that $b = c$ as desired. Now suppose inductively that we have the cancellation law for a (so that $a + b = a + c$ implies $b = c )$ ; we now have to prove the cancellation law for $a { \mathrel { + { + } } }$ . In other words, we assume that $( a + + ) + b = ( a + + ) + c$ and need to show that $b = c .$ . By the definition of addition, $( a + + ) + b = ( a + b ) + { \mathrm { ~ a n d ~ } } ( a + + ) + c = ( a + c ) + +$ and so we have $( a + b ) \substack { + + } = ( a + c ) \tgroup + +$ . By Axiom 2.4, we have $a + b = a + c .$ Since we already have the cancellation law for a, we thus have $b = c$ as desired. This closes the induction. □ 

We now discuss how addition interacts with positivity. 

Definition 2.2.7 (Positive natural numbers). A natural number n is said to be positive if it is not equal to $0 . ~ ( ^ { 6 4 } \mathrm { f f } ^ { \prime } )$ is shorthand for “if and only $\mathrm { i f ~ ^ { 9 } ~ - ~ s e e }$ Section A.1). 

Proposition 2.2.8. If a is positive and b is a natural number, then $a + b$ is positive (and hence $b + a$ is also, by Proposition $\it 2 . 2 . 4 )$ 

Proof. We use induction on b. If $b = 0$ , then $a + b = a + 0 = a$ , which is positive, so this proves the base case. Now suppose inductively that $a + b$ is positive. Then $a + ( b + 1 + ) = ( a + b ) + 1$ , which cannot be zero by Axiom 2.3, and is hence positive. This closes the induction. □ 

Corollary 2.2.9. If a and b are natural numbers such that $a + b = 0$ then $a = 0$ and $b = 0$ 

Proof. Suppose for sake of contradiction that $a \neq 0$ or $b \neq 0$ . If $a \neq 0$ then a is positive, and hence $a + b = 0$ is positive by Proposition 2.2.8, a contradiction. Similarly if $b \neq 0$ then b is positive, and again $a + b = 0$ is positive by Proposition 2.2.8, a contradiction. Thus a and b must both be zero. □ 

Lemma 2.2.10. Let a be a positive number. Then there exists exactly one natural number b such that $b { + } { + } = a$ 

Proof. See Exercise 2.2.2. 

Once we have a notion of addition, we can begin defining a notion of order. 

Definition 2.2.11 (Ordering of the natural numbers). Let n and m be natural numbers. We say that n is greater than or equal to $m ,$ and write $n \geq m { \mathrm { ~ o r ~ } } m \leq n$ , if we have $n = m + a$ for some natural number a. We say that n is strictly greater than m, and write $n > m { \mathrm { ~ o r ~ } } m < n$ , if $n \geq m$ and $n \neq m$ 

Thus for instance $8 > 5$ , because $8 = 5 + 3$ and $8 \neq 5$ . Also note that $n { \mathrel { + } } + > n$ for any n; thus there is no largest natural number n, because the next number $^ { n + + }$ is always larger still. 

Proposition 2.2.12 (Basic properties of order for natural numbers). Let a, b, c be natural numbers. Then 

(a) (Order is reflexive) $a \geq a$ 

(b) (Order is transitive) If $a \geq b$ and $b \geq c _ { i }$ , then $a \geq c$ 

(c) (Order is anti-symmetric) If $a \geq b$ and $b \geq a$ , then $a = b$ 

(d) (Addition preserves order) $a \geq b$ if and only if $a + c \geq b + c .$ 

(e) $a < b$ if and only if $a + + \leq b$ 

(f ) $a < b$ if and only if $b = a + a$ for some positive number d. 

Proof. See Exercise 2.2.3. 

Proposition 2.2.13 (Trichotomy of order for natural numbers). Let a and b be natural numbers. Then exactly one of the following statements is true: $a < b , a = b , o r a > b$ 

Proof. This is only a sketch of the proof; the gaps will be filled in Exercise 2.2.4. 

First we show that we cannot have more than one of the statements $a < b , a = b , a > b$ holding at the same time. If $a < b$ then $a \neq b$ by definition, and if $a > b$ then $a \neq b$ by definition. If $a > b$ and $a < b$ then by Proposition 2.2.12 we have $a = b .$ , a contradiction. Thus no more than one of the statements is true. 

Now we show that at least one of the statements is true. We keep b fixed and induct on a. When $a = 0$ we have $0 \leq b$ for all $b \ \mathrm { ( w h y ? ) }$ , so we have either $0 = b \ { \mathrm { o r } } \ 0 < b .$ , which proves the base case. Now suppose we have proven the proposition for a, and now we prove the proposition for $a { \mathrel { + { + } } }$ . From the trichotomy for a, there are three cases: $a < b , a = b ,$ and $a > b$ . If $a > b$ , then $a \mathrm { + + } > b ~ \mathrm { ( w h y ? ) }$ . If $a = b ,$ , then $a \mathrm { + } \mathrm { + } \mathrm { > } b$ (why?). Now suppose that $a < b$ . Then by Proposition 2.2.12, we have $a + + \leq b$ . Thus either $a \mathrm { + } \mathrm { + } = b \mathrm { ~ o r ~ } a \mathrm { + } \mathrm { + } < b$ , and in either case we are done. This closes the induction. □ 

The properties of order allow one to obtain a stronger version of the principle of induction: 

Proposition 2.2.14 (Strong principle of induction). Let $m _ { 0 }$ be a natural number, and let $P ( m )$ be a property pertaining to an arbitrary natural 

## 2.3. Multiplication

number m. Suppose that for each $m \geq m _ { 0 }$ , we have the following implication: if $P ( m ^ { \prime } )$ is true for all natural numbers $m _ { 0 } \le m ^ { \prime } < m$ , then $P ( m )$ is also true. (In particular, this means that $P ( m _ { 0 } )$ is true, since in this case the hypothesis is vacuous.) Then we can conclude that $P ( m )$ is true for all natural numbers $m \geq m _ { 0 }$ 

Remark 2.2.15. In applications we usually use this principle with $m _ { 0 } =$ 0 or $m _ { 0 } = 1$ 

Proof. See Exercise 2.2.5. 

— Exercises — 

Exercise 2.2.1. Prove Proposition 2.2.5. (Hint: fix two of the variables and induct on the third.) 

Exercise 2.2.2. Prove Lemma 2.2.10. (Hint: use induction.) 

Exercise 2.2.3. Prove Proposition 2.2.12. (Hint: you will need many of the preceding propositions, corollaries, and lemmas.) 

Exercise 2.2.4. Justify the three statements marked $\mathrm { ( w h y ? ) }$ in the proof of Proposition 2.2.13. 

Exercise 2.2.5. Prove Proposition 2.2.14. (Hint: define $Q ( n )$ to be the property that $P ( m )$ is true for all $m _ { 0 } \leq m < n ;$ note that $Q ( n )$ is vacuously true when $n < m _ { 0 } . )$ 

Exercise 2.2.6. Let n be a natural number, and let $P ( m )$ be a property pertaining to the natural numbers such that whenever $P ( m { + } { + } )$ is true, then $P ( m )$ is true. Suppose that $P ( n )$ is also true. Prove that $P ( m )$ is true for all natura numbers $m \leq n ;$ this is known as the principle of backwards induction. (Hint: apply induction to the variable n.) 

## 2.3 Multiplication

In the previous section we have proven all the basic facts that we know to be true about addition and order. To save space and to avoid belaboring the obvious, we will now allow ourselves to use all the rules of algebra concerning addition and order that we are familiar with, without further comment. Thus for instance we may write things like $a + b + c = c +$ $b + a$ without supplying any further justification. Now we introduce multiplication. Just as addition is the iterated increment operation, multiplication is iterated addition: 

Definition 2.3.1 (Multiplication of natural numbers). Let m be a natural number. To multiply zero to m, we define $0 \times m : = 0$ . Now suppose inductively that we have defined how to multiply n to m. Then we can multiply $n { \mathrm { + } } + { \mathrm { ~ t o ~ } } m$ by defining $( n { + } + ) \times m : = ( n \times m ) + m$ 

Thus for instance $0 \times m = 0 , 1 \times m = 0 + m , 2 \times m = 0 + m + m ,$ etc. By induction one can easily verify that the product of two natura numbers is a natural number. 

Lemma 2.3.2 (Multiplication is commutative). Let n, m be natural numbers. Then $n \times m = m \times n$ 

Proof. See Exercise 2.3.1. 

We will now abbreviate $n \times m$ as nm, and use the usual convention that multiplication takes precedence over addition, thus for instance $a b + c$ means $( a \times b ) + c$ , not $a \times ( b + c )$ . (We will also use the usual notational conventions of precedence for the other arithmetic operations when they are defined later, to save on using parentheses all the time.) 

Lemma 2.3.3 (Positive natural numbers have no zero divisors). Let n, m be natural numbers. Then $n \times m = 0$ if and only if at least one of n, m is equal to zero. In particular, if n and m are both positive, then nm is also positive. 

Proof. See Exercise 2.3.2. 

Proposition 2.3.4 (Distributive law). For any natural numbers $a , b , c ,$ we have $a ( b + c ) = a b + a c \ a n d \ ( b + c ) a = b a + c a$ 

Proof. Since multiplication is commutative we only need to show the first identity $a ( b + c ) = a b + a c .$ . We keep a and b fixed, and use induction on c. Let’s prove the base case $c = 0 , \mathrm { i . e . , } a ( b + 0 ) = a b + a 0$ The left-hand side is $a b .$ , while the right-hand side is $a b + 0 = a b .$ , so we are done with the base case. Now let us suppose inductively that $a ( b + c ) =$ $a b + a c ,$ and let us prove that $a ( b + ( c + 1 ) ) = a b + a ( c + 1 )$ . The lefthand side is $a ( ( b + c ) + + ) = a ( b + c ) + a$ , while the right-hand side is $a b + a c + a = a ( b + c ) + a$ by the induction hypothesis, and so we can close the induction. □ 

Proposition 2.3.5 (Multiplication is associative). For any natural numbers $a , b , c ,$ , we have $( a \times b ) \times c = a \times ( b \times c )$ 

Proof. See Exercise 2.3.3. 

Proposition 2.3.6 (Multiplication preserves order). If a, b are natural numbers such that $a < b$ , and c is positive, then $a c < b c ,$ 

Proof. Since $a < b ,$ , we have $b = a + d$ for some positive d. Multiplying by c and using the distributive law we obtain $b c = a c + d c$ . Since d is positive, and c is positive, dc is positive, and hence $a c < b c$ as desired. □ 

Corollary 2.3.7 (Cancellation law). Let a, b, c be natural numbers such that $a c = b c$ and c is non-zero. Then $a = b$ 

Remark 2.3.8. Just as Proposition 2.2.6 will allow for a “virtual subtraction” which will eventually let us define genuine subtraction, this corollary provides a “virtual division” which will be needed to define genuine division later on. 

Proof. By the trichotomy of order (Proposition 2.2.13), we have three cases: $a < b , a = b , a > b .$ . Suppose first that $a < b ,$ , then by Proposition 2.3.6 we have $a c < b c ,$ a contradiction. We can obtain a similar contradiction when $a > b$ . Thus the only possibility is that $a = b$ , as desired. □ 

With these propositions it is easy to deduce all the familiar rules of algebra involving addition and multiplication, see for instance Exercise 2.3.4. 

Now that we have the familiar operations of addition and multiplication, the more primitive notion of increment will begin to fall by the wayside, and we will see it rarely from now on. In any event we can always use addition to describe incrementation, since $n \mathrm { + } + = n \mathrm { + } 1$ 

Proposition 2.3.9 (Euclidean algorithm). Let n be a natural number, and let q be a positive number. Then there exist natural numbers m, r such that $0 \leq r < q$ and $n = m q + r$ 

Remark 2.3.10. In other words, we can divide a natural number n by a positive number q to obtain a quotient m (which is another natural number) and a remainder r (which is less than $q )$ . This algorithm marks the beginning of number theory, which is a beautiful and important subject but one which is beyond the scope of this text. 

Proof. See Exercise 2.3.5. 

Just like one uses the increment operation to recursively define addition, and addition to recursively define multiplication, one can use multiplication to recursively define exponentiation: 

Definition 2.3.11 (Exponentiation for natural numbers). Let m be a natural number. To raise m to the power 0, we define $m ^ { 0 } : = 1$ ; in particular, we define $0 ^ { 0 } : = 1$ . Now suppose recursively that $m ^ { n }$ has been defined for some natural number n, then we define $m ^ { n + + } : = m ^ { n } \times m$ 

Examples 2.3.12. Thus for instance $x ^ { 1 } = x ^ { 0 } \times x = 1 \times x = x ; x ^ { 2 } =$ $x ^ { 1 } \times x = x \times x ; x ^ { 3 } = x ^ { 2 } \times x = x \times x \times x ;$ and so forth. By induction we see that this recursive definition defines $x ^ { n }$ for all natural numbers n. 

We will not develop the theory of exponentiation too deeply here, but instead wait until after we have defined the integers and rational numbers; see in particular Proposition 4.3.10. 

— Exercises — 



Exercise 2.3.1. Prove Lemma 2.3.2. (Hint: modify the proofs of Lemmas 2.2.2, 2.2.3 and Proposition 2.2.4.) 



Exercise 2.3.2. Prove Lemma 2.3.3. (Hint: prove the second statement first.) 



Exercise 2.3.3. Prove Proposition 2.3.5. (Hint: modify the proof of Proposition 2.2.5 and use the distributive law.) 



Exercise 2.3.4. Prove the identity $( a + b ) ^ { 2 } = a ^ { 2 } + 2 a b + b ^ { 2 }$ for all natural numbers a, b. 



Exercise 2.3.5. Prove Proposition 2.3.9. (Hint: fix q and induct on n.) 



## Chapter 3

## Set theory

Modern analysis, like most of modern mathematics, is concerned with numbers, sets, and geometry. We have already introduced one type of number system, the natural numbers. We will introduce the other number systems shortly, but for now we pause to introduce the concepts and notation of set theory, as they will be used increasingly heavily in later chapters. (We will not pursue a rigorous description of Euclidean geometry in this text, preferring instead to describe that geometry in terms of the real number system by means of the Cartesian co-ordinate system.) 

While set theory is not the main focus of this text, almost every other branch of mathematics relies on set theory as part of its foundation, so it is important to get at least some grounding in set theory before doing other advanced areas of mathematics. In this chapter we present the more elementary aspects of axiomatic set theory, leaving more advanced topics such as a discussion of infinite sets and the axiom of choice to Chapter 8. A full treatment of the finer subtleties of set theory (of which there are many!) is unfortunately well beyond the scope of this text. 

## 3.1 Fundamentals

In this section we shall set out some axioms for sets, just as we did for the natural numbers. For pedagogical reasons, we will use a somewhat overcomplete list of axioms for set theory, in the sense that some of the axioms can be used to deduce others, but there is no real harm in doing this. We begin with an informal description of what sets should be. 

Definition 3.1.1. (Informal) We define a set A to be any unordered collection of objects, e.g., 3, 8, 5, 2 is a set. If x is an object, we say that x is an element of A or $x \in A$ if x lies in the collection; otherwise we say that $x \not \in A$ . For instance, $3 \in \{ 1 , 2 , 3 , 4 , 5 \}$ but $7 \notin \{ 1 , 2 , 3 , 4 , 5 \}$ 

This definition is intuitive enough, but it doesn’t answer a number of questions, such as which collections of objects are considered to be sets, which sets are equal to other sets, and how one defines operations on sets $( \mathrm { e . g . }$ , unions, intersections, etc.). Also, we have no axioms yet on what sets do, or what their elements do. Obtaining these axioms and defining these operations will be the purpose of the remainder of this section. 

We first clarify one point: we consider sets themselves to be a type of object. 

Axiom 3.1 (Sets are objects). If A is a set, then A is also an object. In particular, given two sets A and B, it is meaningful to ask whether A is also an element of B. 

Example 3.1.2. (Informal) The set $\{ 3 , \{ 3 , 4 \} , 4 \}$ is a set of three distinct elements, one of which happens to itself be a set of two elements. See Example 3.1.10 for a more formal version of this example. However, not all objects are sets; for instance, we typically do not consider a natural number such as 3 to be a set. (The more accurate statement is that natural numbers can be the cardinalities of sets, rather than necessarily being sets themselves. See Section 3.6.) 

Remark 3.1.3. There is a special case of set theory, called “pure set theory”, in which all objects are sets; for instance the number 0 might be identified with the empty set $\varnothing = \{ \}$ , the number 1 might be identified with $\{ 0 \} = \{ \{ \} \}$ , the number 2 might be identified with $\{ 0 , 1 \} = \{ \{ \} , \{ \{ \} \} \}$ , and so forth. From a logical point of view, pure set theory is a simpler theory, since one only has to deal with sets and not with objects; however, from a conceptual point of view it is often easier to deal with impure set theories in which some objects are not considered to be sets. The two types of theories are more or less equivalent for the purposes of doing mathematics, and so we shall take an agnostic position as to whether all objects are sets or not. 

To summarize so far, among all the objects studied in mathematics, some of the objects happen to be sets; and if x is an object and A is a set, then either $x \in A$ is true or $x \in A$ is false. (If A is not a set, we leave the statement $x \in A$ undefined; for instance, we consider the statement $3 \in 4$ to neither be true or false, but simply meaningless, since 4 is not a set.) 

Next, we define the notion of equality: when are two sets considered to be equal? We do not consider the order of the elements inside a set to be important; thus we think of 3, 8, 5, 2 and 2, 3, 5, 8 as the same set. On the other hand, 3, 8, 5, 2 and 3, 8, 5, 2, 1 are diferent sets, because the latter set contains an element that the former one does not, namely the element 1. For similar reasons 3, 8, 5, 2 and 3, 8, 5 are diferent sets. We formalize this as a definition: 

Definition 3.1.4 (Equality of sets). Two sets A and B are equal, $A = B$ , if every element of A is an element of B and vice versa. To put it another way, $A = B$ if and only if every element x of A belongs also to B, and every element y of B belongs also to A. 

Example 3.1.5. Thus, for instance, 1, 2, 3, 4, 5 and 3, 4, 2, 1, 5 are the same set, since they contain exactly the same elements. (The set 3, 3, 1, 5, 2, 4, 2 is also equal to 1, 2, 3, 4, 5 ; the repetition of 3 and 2 is irrelevant as it does not further change the status of 2 and 3 being elements of the set.) 

One can easily verify that this notion of equality is reflexive, symmetric, and transitive (Exercise 3.1.1). Observe that if $x \in A$ and $A = B$ , then $x \in B$ , by Definition 3.1.4. Thus the “is an element of” relation obeys the axiom of substitution (see Section A.7). Because of this, any new operation we define on sets will also obey the axiom of substitution, as long as we can define that operation purely in terms of the relation . This is for instance the case for the remaining definitions in this section. (On the other hand, we cannot use the notion of the “first” or “last” element in a set in a well-defined manner, because this would not respect the axiom of substitution; for instance the sets 1, 2, 3, 4, 5 and 3, 4, 2, 1, 5 are the same set, but have diferent first elements.) 

Next, we turn to the issue of exactly which objects are sets and which objects are not. The situation is analogous to how we defined the natural numbers in the previous chapter; we started with a single natural number, 0, and started building more numbers out of 0 using the increment operation. We will try something similar here, starting with a single set, the empty set, and building more sets out of the empty set by various operations. We begin by postulating the existence of the empty set. 

Axiom 3.2 (Empty set). There exists a set $\varnothing _ { i }$ , known as the empty set, which contains no elements, i.e., for every object x we have x $\notin \emptyset$ 

The empty set is also denoted $\{ \}$ . Note that there can only be one empty set; if there were two sets $\varnothing$ and $\varnothing ^ { \prime }$ which were both empty, then by Definition 3.1.4 they would be equal to each other (why?). 

If a set is not equal to the empty set, we call it non-empty. The following statement is very simple, but worth stating nevertheless: 

Lemma 3.1.6 (Single choice). Let A be a non-empty set. Then there exists an object x such that $x \in A$ 

Proof. We prove by contradiction. Suppose there does not exist any object x such that $x \in A$ . Then for all objects x, we have $x \not \in A$ . Also, by Axiom 3.2 we have $x \notin \varnothing$ . Thus $x \in A \iff x \in \emptyset$ (both statements are equally false), and so $A = \emptyset$ by Definition 3.1.4, a contradiction. 

Remark 3.1.7. The above Lemma asserts that given any non-empty set A, we are allowed to “choose” an element x of A which demonstrates this non-emptyness. Later on (in Lemma 3.5.12) we will show that given any finite number of non-empty sets, say $A _ { 1 } , \ldots , A _ { n }$ , it is possible to choose one element $x _ { 1 } , \ldots , x _ { n }$ from each set $A _ { 1 } , \ldots , A _ { n } ;$ this is known as “finite choice”. However, in order to choose elements from an infinite number of sets, we need an additional axiom, the axiom of choice, which we wil discuss in Section 8.4. 

Remark 3.1.8. Note that the empty set is not the same thing as the natural number 0. One is a set; the other is a number. However, it is true that the cardinality of the empty set is 0; see Section 3.6. 

If Axiom 3.2 was the only axiom that set theory had, then set theory could be quite boring, as there might be just a single set in existence, the empty set. We now present further axioms to enrich the class of sets available. 

Axiom 3.3 (Singleton sets and pair sets). If a is an object, then there exists a set $\{ a \}$ whose only element is a, i.e., for every object y, we have $y \in \{ a \}$ if and only if $y = a ,$ ; we refer to $\{ a \}$ as the singleton set whose element is a. Furthermore, if a and b are objects, then there exists a set $\{ a , b \}$ whose only elements are a and b; i.e., for every object y, we have $y \in \{ a , b \}$ if and only if $y = a o r y = b $ ; we refer to this set as the pair set formed by a and b. 

## 3.1. Fundamentals

Remarks 3.1.9. Just as there is only one empty set, there is only one singleton set for each object $^ { a , }$ thanks to Definition 3.1.4 (why?). Similarly, given any two objects a and $b ,$ there is only one pair set formed by $a$ and b. Also, Definition 3.1.4 also ensures that $\{ a , b \} = \{ b , a \}$ (why?) and $\{ a , a \} = \{ a \} ~ ( \mathrm { w h y ? } )$ . Thus the singleton set axiom is in fact redundant, being a consequence of the pair set axiom. Conversely, the pair set axiom will follow from the singleton set axiom and the pairwise union axiom below (see Lemma 3.1.13). One may wonder why we $\mathrm { d o n ^ { \prime } t }$ $_ \mathrm { g o }$ further and create triplet axioms, quadruplet axioms, etc.; however there will be no need for this once we introduce the pairwise union axiom below. 

Examples 3.1.10. Since $\varnothing$ is a set (and hence an object), so is singleton set , i.e., the set whose only element is $\varnothing .$ , is a set (and it is not the same set as $\emptyset , \ \{ \emptyset \} \neq \emptyset \ ( \mathrm { w h y ? } ) )$ . Similarly, the singleton set $\{ \{ \emptyset \} \}$ and the pair set $\{ \emptyset , \{ \emptyset \} \}$ are also sets. These three sets are not equal to each other (Exercise 3.1.2). 

As the above examples show, we can now create quite a few sets; however, the sets we make are still fairly small (each set that we can build consists of no more than two elements, so far). The next axiom allows us to build somewhat larger sets than before. 

Axiom 3.4 (Pairwise union). Given any two sets A, B, there exists a set $A \cup B$ , called the union $A \cup B$ of A and B, whose elements consists of all the elements which belong to A or B or both. In other words, for any object x, 

$$
x \in A \cup B \iff (x \in A o r x \in B).
$$

Recall that $^ { 6 6 } \mathrm { o r } ^ { 9 9 }$ refers by default in mathematics to inclusive or: $^ { 6 6 } X$ or Y is true” means that “either X is true, or Y is true, or both are $\mathrm { t r u e } ^ { \dag }$ . See Section A.1. 

Example 3.1.11. The set $\{ 1 , 2 \} \cup \{ 2 , 3 \}$ consists of those elements which either lie on 1, 2 or in 2, 3 or in both, or in other words the elements of this set are simply 1, 2, and 3. Because of this, we denote this set as $\{ 1 , 2 \} \cup \{ 2 , 3 \} = \{ 1 , 2 , 3 \}$ 

Remark 3.1.12. If A, B, A are sets, and A is equal to $A ^ { \prime } .$ , then $A \cup B$ is equal to $A ^ { \prime } \cup B$ (why? One needs to use Axiom 3.4 and Definition 3.1.4). Similarly if $B ^ { \prime }$ is a set which is equal to B, then $A \cup B$ is equal to $A \cup B ^ { \prime }$ . Thus the operation of union obeys the axiom of substitution, and is thus well-defined on sets. 

We now give some basic properties of unions. 

Lemma 3.1.13. If a and b are objects, then $\{ a , b \} = \{ a \} \cup \{ b \}$ . If $A , B , C$ are sets, then the union operation is commutative $( i . e . , A \cup B =$ $B \cup A )$ and associative $( i . e . , ( A \cup B ) \cup C = A \cup ( B \cup C ) )$ . Also, we have $A \cup A = A \cup \emptyset = \emptyset \cup A = A$ 

Proof. We prove just the associativity identity $( A \cup B ) \cup C = A \cup ( B \cup C )$ and leave the remaining claims to Exercise 3.1.3. By Definition 3.1.4,we need to show that every element x of $( A \cup B ) \cup C$ is an element of$A \cup ( B \cup C )$ , and vice versa. So suppose first that x is an element of$( A \cup B ) \cup C$ . By Axiom 3.4, this means that at least one of $x \in A \cup B$ or$x \in C$ is true. We now divide into two cases. If $x \in C$ , then by Axiom 3.4again $x \in B \cup C$ , and so by Axiom 3.4 again we have $x \in A \cup ( B \cup C )$ Now suppose instead $x \in A \cup B$ , then by Axiom 3.4 again $x \in A$ or$x \in B$ . If $x \in A$ then $x \in A \cup ( B \cup C )$ by Axiom 3.4, while if $x \in B$ then by consecutive applications of Axiom 3.4 we have $x \in B \cup C$ andhence $x \in A \cup ( B \cup C )$ Thus in all cases we see that every element of$( A \cup B ) \cup C$ lies in $A \cup ( B \cup C )$ . A similar argument shows that everyelement of $A \cup ( B \cup C )$ lies in $( A \cup B ) \cup C$ , and so $( A \cup B ) \cup C = A \cup ( B \cup C )$ as desired. 厂

Because of the above lemma, we do not need to use parentheses to denote multiple unions, thus for instance we can write $A \cup B \cup C$ instead of $( A \cup B ) \cup C$ or $A \cup ( B \cup C )$ . Similarly for unions of four sets, $A \cup B \cup C \cup D .$ , etc. 

Remark 3.1.14. While the operation of union has some similarities with addition, the two operations are not identical. For instance, $\{ 2 \} \cup$ $\{ 3 \} = \{ 2 , 3 \}$ and $2 + 3 = 5$ , whereas $\{ 2 \} + \{ 3 \}$ is meaningless (addition pertains to numbers, not sets) and $2 \cup 3$ is also meaningless (union pertains to sets, not numbers). 

This axiom allows us to define triplet sets, quadruplet sets, and so forth: if $a , b , c$ are three objects, we define $\{ a , b , c \} : = \{ a \} \cup \{ b \} \cup \{ c \}$ ; if $a , b , c ,$ d are four objects, then we define $\{ a , b , c , d \} : = \{ a \} \cup \{ b \} \cup \{ c \} \cup \{ d \}$ and so forth. On the other hand, we are not yet in a position to define sets consisting of n objects for any given natural number n; this would require iterating the above construction $^ { 6 6 } n$ times”, but the concept of $n { \mathrm { - f o l d } }$ iteration has not yet been rigorously defined. For similar reasons, we cannot yet define sets consisting of infinitely many objects, because that would require iterating the axiom of pairwise union infinitely often, and it is not clear at this stage that one can do this rigorously. Later on, we will introduce other axioms of set theory which allow one to construct arbitrarily large, and even infinite, sets. 

Clearly, some sets seem to be larger than others. One way to formalize this concept is through the notion of a subset. 

Definition 3.1.15 (Subsets). Let $A , B$ be sets. We say that A is a subset of B, denoted $A \subseteq B$ , if every element of A is also an element of B, i.e. 

$$
\text { For   any   object } x, \quad x \in A \quad \implies \quad x \in B.
$$

We say that A is a proper subset of B, denoted $A \subsetneq B ,$ , if $A \subseteq B$ and $A \neq B$ 

Remark 3.1.16. Because these definitions involve only the notions of equality and the “is an element of” relation, both of which already obey the axiom of substitution, the notion of subset also automatically obeys the axiom of substitution. Thus for instance if $A \subseteq B$ and $A = A ^ { \prime }$ , then $A ^ { \prime } \subseteq B$ 

Examples 3.1.17. We have $\{ 1 , 2 , 4 \} \subseteq \{ 1 , 2 , 3 , 4 , 5 \}$ , because every element of $\{ 1 , 2 , 4 \}$ is also an element of $\{ 1 , 2 , 3 , 4 , 5 \}$ . In fact we also have $\{ 1 , 2 , 4 \} \subsetneq \{ 1 , 2 , 3 , 4 , 5 \}$ , since the two sets 1, 2, 4 and 1, 2, 3, 4, 5 are not equal. Given any set A, we always have $A \subseteq A { \mathrm { ~ ( w h y ? ) } }$ and $\varnothing \subseteq A$ (why?). 

The notion of subset in set theory is similar to the notion of “less than or equal $\mathrm { t o } ^ { \dag }$ for numbers, as the following Proposition demonstrates (for a more precise statement, see Definition 8.5.1): 

Proposition 3.1.18 (Sets are partially ordered by set inclusion). Let $A , B , C$ be sets. If $A \subseteq B$ and $B \subseteq C$ then $A \subseteq C$ . If $A \subseteq B$ and $B \subseteq A$ , then $A = B$ . Finally, if $A \subsetneq B$ and $B \subsetneq C$ then $A \subsetneq C$ 

Proof. We shall just prove the first claim. Suppose that $A \subseteq B$ and $B \subseteq C$ . To prove that $A \subseteq C$ , we have to prove that every element of A is an element of C. So, let us pick an arbitrary element x of A. Then, since $A \subseteq B$ , x must then be an element of B. But then since $B \subseteq C$ , x is an element of C. Thus every element of A is indeed an element of $C ,$ as claimed. □ 

Remark 3.1.19. There is a relationship between subsets and unions: see for instance Exercise 3.1.7. 

Remark 3.1.20. There is one important diference between the subset relation $\subsetneq$ and the less than relation $<$ . Given any two distinct natural numbers $n , m ,$ we know that one of them is smaller than the other (Proposition 2.2.13); however, given two distinct sets, it is not in general true that one of them is a subset of the other. For instance, take $A : =$ $\{ 2 n : n \in \mathbf { N } \}$ to be the set of even natural numbers, and $B : = \{ 2 n + 1 :$ $n \in \mathbf { N } \}$ to be the set of odd natural numbers. Then neither set is a subset of the other. This is why we say that sets are only partially ordered, whereas the natural numbers are totally ordered (see Definitions 8.5.1, 8.5.3). 

Remark 3.1.21. We should also caution that the subset relation $\subseteq$ is not the same as the element relation $\in .$ . The number 2 is an element of $\{ 1 , 2 , 3 \}$ but not a subset; thus $2 \in \{ 1 , 2 , 3 \}$ , but $2 \not \subseteq \{ 1 , 2 , 3 \}$ . Indeed, 2 is not even a set. Conversely, while 2 is a subset of $\{ 1 , 2 , 3 \}$ , it is not an element; thus $\{ 2 \} \subseteq \{ 1 , 2 , 3 \}$ but $\{ 2 \} \not \in \{ 1 , 2 , 3 \}$ . The point is that the number 2 and the set 2 are distinct objects. It is important to distinguish sets from their elements, as they can have diferent properties. For instance, it is possible to have an infinite set consisting of finite numbers (the set N of natural numbers is one such example), and it is also possible to have a finite set consisting of infinite objects (consider for instance the finite set $\{ { \bf N } , { \bf Z } , { \bf Q } , { \bf R } \}$ , which has four elements, all of which are infinite). 

We now give an axiom which easily allows us to create subsets out of larger sets. 

Axiom 3.5 (Axiom of specification). Let A be a set, and for each $x \in$ A, let $P ( x )$ be a property pertaining to ${ \mathrm { ~ ; ~ } } ( i . e . , \ P ( x )$ is either a true statement or a false statement). Then there exists a set, called $\{ x \in A$ : $P ( x )$ is true (or simply $\{ x \in A : P ( x ) \}$ for short), whose elements are precisely the elements x in A for which $P ( x )$ is true. In other words, for any object y, 

$$
y \in \{x \in A: P (x) \text {   is   true } \} \iff (y \in A \text {   and   } P (y) \text {   is   true }).
$$

This axiom is also known as the axiom of separation. Note that $\{ x \in A : P ( x )$ is true is always a subset of $A \ \mathrm { ( w h y ? ) }$ , though it could be as large as $A$ or as small as the empty set. One can verify that the axiom of substitution works for specification, thus if $A = A ^ { \prime }$ then $\{ x \in A : P ( x ) \} = \{ x \in A ^ { \prime } : P ( x ) \} \ ( \mathrm { w h y ? } )$ 

Example 3.1.22. Let $S : = \{ 1 , 2 , 3 , 4 , 5 \}$ . Then the set $\{ n \in S : n < 4 \}$ is the set of those elements n in S for which $n < 4$ is true, i.e., $\{ n \in S$ $n < 4 \} = \{ 1 , 2 , 3 \}$ . Similarly, the set $\{ n \in S : n < 7 \}$ is the same as $S$ itself, while $\{ n \in S : n < 1 \}$ is the empty set. 

We sometimes write $\{ x \in A { \big | } P ( x ) \}$ instead of $\{ x \in A : P ( x ) \}$ ; this is useful when we are using the colon $\stackrel { 6 6 , 9 9 } { : }$ to denote something else, for instance to denote the range and domain of a function $f : X \to Y )$ 

We can use this axiom of specification to define some further operations on sets, namely intersections and diference sets. 

Definition 3.1.23 (Intersections). The intersection $S _ { 1 } \cap S _ { 2 }$ of two sets is defined to be the set 

$$
S _ {1} \cap S _ {2} := \{x \in S _ {1}: x \in S _ {2} \}.
$$

In other words, $S _ { 1 } \cap S _ { 2 }$ consists of all the elements which belong to both $S _ { 1 }$ and $S _ { 2 }$ . Thus, for all objects $x _ { i }$ , 

$$
x \in S _ {1} \cap S _ {2} \iff x \in S _ {1} \text {   and   } x \in S _ {2}.
$$

Remark 3.1.24. Note that this definition is well-defined (i.e., it obeys the axiom of substitution, see Section $\mathrm { A } . 7 )$ because it is defined in terms of more primitive operations which were already known to obey the axiom of substitution. Similar remarks apply to future definitions in this chapter and will usually not be mentioned explicitly again. 

Examples 3.1.25. We have $\{ 1 , 2 , 4 \} \cap \{ 2 , 3 , 4 \} = \{ 2 , 4 \} , \{ 1 , 2 \} \cap \{ 3 , 4 \} =$ $\emptyset , \{ 2 , 3 \} \cup \emptyset = \{ 2 , 3 \}$ , and $\{ 2 , 3 \} \cap \varnothing = \varnothing .$ 

Remark 3.1.26. By the way, one should be careful with the English word “and”: rather confusingly, it can mean either union or intersection, depending on context. For instance, if one talks about a set of “boys and girls”, one means the union of a set of boys with a set of girls, but if one talks about the set of people who are single and male, then one means the intersection of the set of single people with the set of male people. (Can you work out the rule of grammar that determines when “and” means union and when “and” means intersection?) Another problem is that “and” is also used in English to denote addition, thus for instance one could say that $^ { 6 6 } 2$ and 3 is $5 ^ { \mathfrak { s } }$ , while also saying that “the elements of 

2 and the elements of 3 form the set $\{ 2 , 3 \} ^ { \mathfrak { s } }$ and “the elements in 2 and 3 form the set $\varnothing ^ { \mathfrak { s } }$ . This can certainly get confusing! One reason we resort to mathematical symbols instead of English words such as $\mathrm { ^ { 6 6 } a n d ^ { \prime } }$ is that mathematical symbols always have a precise and unambiguous meaning, whereas one must often look very carefully at the context in order to work out what an English word means. 

Two sets $A , B$ are said to be disjoint if $A \cap B = \emptyset$ . Note that this is not the same concept as being distinct, $A \neq B$ . For instance, the sets 1, 2, 3 and 2, 3, 4 are distinct (there are elements of one set which are not elements of the other) but not disjoint (because their intersection is non-empty). Meanwhile, the sets $\varnothing$ and $\varnothing$ are disjoint but not distinct $\mathrm { \left( w h y ? \right) }$ 

Definition 3.1.27 (Diference sets). Given two sets A and B, we define the set $A - B$ or $A \backslash B$ to be the set A with any elements of B removed: 

$$
A \backslash B := \{x \in A: x \notin B \};
$$

for instance, $\{ 1 , 2 , 3 , 4 \} \backslash \{ 2 , 4 , 6 \} = \{ 1 , 3 \}$ . In many cases B will be a subset of A, but not necessarily. 

We now give some basic properties of unions, intersections, and difference sets. 

Proposition 3.1.28 (Sets form a boolean algebra). Let A, B, C be sets, and let X be a set containing $A , B , C$ as subsets. 

(a) (Minimal element) We have $A \cup \varnothing = A$ and $A \cap \emptyset = \emptyset$ 

(b) (Maximal element) We have $A \cup X = X$ and $A \cap X = A$ 

(c) (Identity) We have $A \cap A = A$ and $A \cup A = A$ 

(d) (Commutativity) We have $A \cup B = B \cup A$ and $A \cap B = B \cap A$ 

(e) (Associativity) We have $( A \cup B ) \cup C = A \cup ( B \cup C ) \ a n d ( A \cap B ) \cap C =$ $A \cap ( B \cap C )$ 

(f ) $( D i s t r i b u t i v i t y )$ We have $A \cap ( B \cup C ) = ( A \cap B ) \cup ( A \cap C )$ and $A \cup ( B \cap C ) = ( A \cup B ) \cap ( A \cup C )$ 

(g) (Partition) We have $A \cup ( X \backslash A ) = X \ a n d \ A \cap ( X \backslash A ) = \emptyset .$ 

## 3.1. Fundamentals

(h) (De Morgan laws) We have $X \backslash ( A \cup B ) = ( X \backslash A ) \cap ( X \backslash B )$ and $X \backslash ( A \cap B ) = ( X \backslash A ) \cup ( X \backslash B )$ 

Remark 3.1.29. The de Morgan laws are named after the logician Augustus De Morgan (1806–1871), who identified them as one of the basic laws of set theory. 

Proof. See Exercise 3.1.6. 

Remark 3.1.30. The reader may observe a certain symmetry in the above laws between and , and between X and . This is an example of duality - two distinct properties or objects being dual to each other. In this case, the duality is manifested by the complementation relation $A \mapsto X \backslash A ;$ the de Morgan laws assert that this relation converts unions into intersections and vice versa. (It also interchanges X and the empty set.) The above laws are collectively known as the laws of Boolean algebra, after the mathematician George Boole (1815–1864), and are also applicable to a number of other objects other than sets; it plays a particularly important rˆole in logic. 

We have now accumulated a number of axioms and results about sets, but there are still many things we are not able to do yet. One of the basic things we wish to do with a set is take each of the objects of that set, and somehow transform each such object into a new object; for instance we may wish to start with a set of numbers, say $\{ 3 , 5 , 9 \}$ , and increment each one, creating a new set 4, 6, 10 . This is not something we can do directly using only the axioms we already have, so we need a new axiom: 

Axiom 3.6 (Replacement). Let A be a set. For any object $x \in A$ , and any object y, suppose we have a statement $P ( x , y )$ pertaining to x and y, such that for each $x \in A$ there is at most one y for which $P ( x , y )$ is true. Then there exists a set $\{ y : P ( x , y )$ is true for some $x \in A \}$ , such that for any object z, 

$$
\begin{array}{c} z \in \{y: P (x, y) \text {is true for some} x \in A \} \\ \iff P (x, z) \text {is true for some} x \in A. \end{array}
$$

Example 3.1.31. Let $A : = \{ 3 , 5 , 9 \}$ , and let $P ( x , y )$ be the statement $y = x { + } + , \operatorname { i . e . , } y$ is the successor of x. Observe that for every $x \in A$ , there is exactly one y for which $P ( x , y )$ is true - specifically, the successor of x. Thus the above axiom asserts that the set $\{ y : y = x + +$ for some $x \in$ $\{ 3 , 5 , 9 \} \}$ exists; in this case, it is clearly the same set as $\{ 4 , 6 , 1 0 \} ( \mathrm { { w h y ? } ) }$ 

Example 3.1.32. Let $A \ = \ \{ 3 , 5 , 9 \}$ , and let $P ( x , y )$ be the statement $y = 1$ Then again for every $x \in \ A$ , there is exactly one y for which $P ( x , y )$ is true - specifically, the number 1. In this case $\{ y : y = 1$ for some $x \in \{ 3 , 5 , 9 \} \}$ is just the singleton set 1 ; we have replaced each element 3, 5, 9 of the original set A by the same object, namely 1. Thus this rather silly example shows that the set obtained by the above axiom can be “smaller” than the original set. 

We often abbreviate a set of the form 

$$
\{y: y = f (x) \text {   for   some   } x \in A \}
$$

as $\{ f ( x ) : x \in A \}$ or $\{ f ( x ) { \big \vert } x \in A \}$ . Thus for instance, if $A = \{ 3 , 5 , 9 \}$ , then $\{ x { \mathrm { + } } \colon x \in A \}$ is the set $\{ 4 , 6 , 1 0 \}$ . We can of course combine the axiom of replacement with the axiom of specification, thus for instance we can create sets such as $\{ f ( x ) : x \in A ; P ( x )$ is true by starting with the set A, using the axiom of specification to create the set $\{ x \in A$ $P ( x )$ is true , and then applying the axiom of replacement to create $\{ f ( x ) : x \in A ; P ( x )$ is true . Thus for instance $\{ n + + : n \in \{ 3 , 5 , 9 \} ; n <$ $6 \} = \{ 4 , 6 \}$ 

In many of our examples we have implicitly assumed that natura numbers are in fact objects. Let us formalize this as follows. 

Axiom 3.7 (Infinity). There exists a set N, whose elements are called natural numbers, as well as an object 0 in N, and an object n++ assigned to every natural number $n \in \mathbf N$ , such that the Peano axioms (Axioms $\it { 2 . 1 - 2 . 5 ) }$ hold. 

This is the more formal version of Assumption 2.6. It is called the axiom of infinity because it introduces the most basic example of an infinite set, namely the set of natural numbers N. (We will formalize what finite and infinite mean in Section 3.6.) From the axiom of infinity we see that numbers such as 3, 5, 7, etc. are indeed objects in set theory, and so (from the pair set axiom and pairwise union axiom) we can indeed legitimately construct sets such as 3, 5, 9 as we have been doing in our examples. 

One has to keep the concept of a set distinct from the elements of that set; for instance, the set $\left\{ n + 3 : n \in \mathbf { N } , 0 \leq n \leq 5 \right\}$ is not the same thing as the expression or function $n + 3$ . We emphasize this with an example: 

Example 3.1.33. (Informal) This example requires the notion of subtraction, which has not yet been formally introduced. The following two sets are equal, 

$$
\{n + 3: n \in \mathbf {N}, 0 \leq n \leq 5 \} = \{8 - n: n \in \mathbf {N}, 0 \leq n \leq 5 \},\tag{3.1}
$$

(see below), even though the expressions $n + 3$ and $8 - n$ are never equal to each other for any natural number n. Thus, it is a good idea to remember to use those curly braces when you talk about sets, lest you accidentally confuse a set with its elements. One reason for this counter-intuitive situation is that the letter n is being used in two diferent ways on the two sides of (3.1). To clarify the situation, let us rewrite the set $\left\{ 8 - n : n \in \mathbf { N } , 0 \leq n \leq 5 \right\}$ by replacing the letter n by the letter m, thus giving $\left\{ 8 - m : m \in \mathbf { N } , 0 \leq m \leq 5 \right\}$ . This is exactly the same set as before (why?), so we can rewrite (3.1) as 

$$
\{n + 3: n \in \mathbf {N}, 0 \leq n \leq 5 \} = \{8 - m: m \in \mathbf {N}, 0 \leq m \leq 5 \}.
$$

Now it is easy to see (using (3.1.4)) why this identity is true: every number of the form $n + 3$ , where n is a natural number between 0 and 5, is also of the form 8 m where $m : = 5 - n$ (note that m is therefore also a natural number between 0 and 5); conversely, every number of the form $8 - m$ , where m is a natural number between 0 and 5, is also of the form $n + 3$ , where $n : = 5 - m$ (note that n is therefore a natural number between 0 and 5). Observe how much more confusing the above explanation of (3.1) would have been if we had not changed one of the n’s to an m first! 

## — Exercises —



Exercise 3.1.1. Show that the definition of equality in Definition 3.1.4 is reflexive, symmetric, and transitive. 





Exercise 3.1.2. Using only Definition 3.1.4, Axiom 3.1, Axiom 3.2, and Axiom 3.3, prove that the sets , , , and ,  are all distinct (i.e., no two of them are equal to each other). 





Exercise 3.1.3. Prove the remaining claims in Lemma 3.1.13. 





Exercise 3.1.4. Prove the remaining claims in Proposition 3.1.18. 





Exercise 3.1.5. Let A, B be sets. Show that the three statements $A \subseteq B$ $A \cup B = B , A \cap B = A$ are logically equivalent (any one of them implies the other two). 



Exercise 3.1.6. Prove Proposition 3.1.28. (Hint: one can use some of these claims to prove others. Some of the claims have also appeared previously in Lemma 3.1.13.) 

Exercise 3.1.7. Let $A , B , C$ be sets. Show that $A \cap B \subseteq A$ and $A \cap B \subseteq B$ Furthermore, show that $C \subseteq A$ and $C \subseteq B$ if and only if $C \subseteq A \cap B$ . In a similar spirit, show that $A \subseteq A \cup B$ and $B \subseteq A \cup B$ , and furthermore that $A \subseteq C$ and $B \subseteq C$ if and only if $A \cup B \subseteq C$ 

Exercise 3.1.8. Let $A , B$ be sets. Prove the absorption laws $A \cap ( A \cup B ) = A$ and $A \cup ( A \cap B ) = A$ 

Exercise 3.1.9. Let $A , B , X$ be sets such that $A \cup B = X$ and $A \cap B = \emptyset$ . Show that $A = X \backslash B$ and $B = X \backslash A$ 

Exercise 3.1.10. Let A and B be sets. Show that the three sets $A \backslash B , A \cap B$ , and $B \backslash A$ are disjoint, and that their union is $A \cup B$ 

Exercise 3.1.11. Show that the axiom of replacement implies the axiom of specification. 

## 3.2 Russell’s paradox (Optional)

Many of the axioms introduced in the previous section have a similar flavor: they both allow us to form a set consisting of all the elements which have a certain property. They are both plausible, but one might think that they could be unified, for instance by introducing the following axiom: 

Axiom 3.8 (Universal specification). (Dangerous!) Suppose for every object x we have a property $P ( x )$ pertaining to x (so that for every x, $P ( x )$ is either a true statement or a false statement). Then there exists a set $\{ x : P ( x )$ is true such that for every object y, 

$$
y \in \{x: P (x) i s t r u e \} \iff P (y) i s t r u e.
$$

This axiom is also known as the axiom of comprehension. It asserts that every property corresponds to a set; if we assumed that axiom, we could talk about the set of all blue objects, the set of all natural numbers, the set of all sets, and so forth. This axiom also implies most of the axioms in the previous section (Exercise 3.2.1). Unfortunately, this axiom cannot be introduced into set theory, because it creates a logical contradiction known as Russell’s paradox, discovered by the philosopher and logician Bertrand Russell (1872–1970) in 1901. The paradox runs as follows. Let $P ( x )$ be the statement 

$$
P (x) \iff \text { `` } x \text {   is   a   set,   and   } x \notin x \text { '' };
$$

i.e., $P ( x )$ is true only when x is a set which does not contain itself. For instance, $P ( \{ 2 , 3 , 4 \} )$ is true, since the set $\{ 2 , 3 , 4 \}$ is not one of the three elements 2, 3, 4 of $\{ 2 , 3 , 4 \}$ . On the other hand, if we let $S$ be the set of all sets (which we would know to exist from the axiom of universal specification), then since S is itself a set, it is an element of $S ,$ , and so $P ( S )$ is false. Now use the axiom of universal specification to create the set 

$$
\Omega := \{x: P (x) \text {   is   true } \} = \{x: x \text {   is   a   set   and   } x \not \in x \},
$$

i.e., the set of all sets which do not contain themselves. Now ask the question: does Ω contain itself, i.e. is $\Omega \in \Omega ?$ If Ω did contain itself, then by definition this means that $P ( \Omega )$ is true, i.e., Ω is a set and $\Omega \not \in \Omega$ . On the other hand, if Ω did not contain itself, then $P ( \Omega )$ would be true, and hence $\Omega \in \Omega$ . Thus in either case we have both $\Omega \in \Omega$ and $\Omega \not \in \Omega$ , which is absurd. 

The problem with the above axiom is that it creates sets which are far too “large” - for instance, we can use that axiom to talk about the set of all objects (a so-called “universal set”). Since sets are themselves objects (Axiom 3.1), this means that sets are allowed to contain themselves, which is a somewhat silly state of afairs. One way to informally resolve this issue is to think of objects as being arranged in a hierarchy. At the bottom of the hierarchy are the primitive objects - the objects that are not $\mathrm { s e t s } ^ { 1 }$ , such as the natural number 37. Then on the next rung of the hierarchy there are sets whose elements consist only of primitive objects, such as 3, 4, 7 or the empty set ; let’s call these “primitive sets” for now. Then there are sets whose elements consist only of primitive objects and primitive sets, such as $\{ 3 , 4 , 7 , \{ 3 , 4 , 7 \} \}$ . Then we can form sets out of these objects, and so forth. The point is that at each stage of the hierarchy we only see sets whose elements consist of objects at lower stages of the hierarchy, and so at no stage do we ever construct a set which contains itself. 

To actually formalize the above intuition of a hierarchy of objects is actually rather complicated, and we will not do so here. Instead, we shall simply postulate an axiom which ensures that absurdities such as Russell’s paradox do not occur. 

Axiom 3.9 (Regularity). If A is a non-empty set, then there is at least one element x of A which is either not a set, or is disjoint from A. 

The point of this axiom (which is also known as the axiom of foundation) is that it is asserting that at least one of the elements of A is so low on the hierarchy of objects that it does not contain any of the other elements of A. For instance, if $A = \{ \{ 3 , 4 \} , \{ 3 , 4 , \{ 3 , 4 \} \} \}$ , then the element $\{ 3 , 4 \} \in A$ does not contain any of the elements of A (neither 3 nor 4 lies in A), although the element $\{ 3 , 4 , \{ 3 , 4 \} \}$ , being somewhat higher in the hierarchy, does contain an element of A, namely 3, 4 . One particular consequence of this axiom is that sets are no longer allowed to contain themselves (Exercise 3.2.2). 

One can legitimately ask whether we really need this axiom in our set theory, as it is certainly less intuitive than our other axioms. For the purposes of doing analysis, it turns out in fact that this axiom is never needed; all the sets we consider in analysis are typically very low on the hierarchy of objects, for instance being sets of primitive objects, or sets of sets of primitive objects, or at worst sets of sets of sets of primitive objects. However it is necessary to include this axiom in order to perform more advanced set theory, and so we have included this axiom in the text (but in an optional section) for sake of completeness. 

## — Exercises —

Exercise 3.2.1. Show that the universal specification axiom, Axiom 3.8, if assumed to be true, would imply Axioms 3.2, 3.3, 3.4, 3.5, and 3.6. (If we assume that all natural numbers are objects, we also obtain Axiom 3.7.) Thus, this axiom, if permitted, would simplify the foundations of set theory tremendously (and can be viewed as one basis for an intuitive model of set theory known as “naive set theory”). Unfortunately, as we have seen, Axiom 3.8 is “too good to be true”! 

Exercise 3.2.2. Use the axiom of regularity (and the singleton set axiom) to show that if A is a set, then A A. Furthermore, show that if A and B are two sets, then either A B or B A (or both). 

Exercise 3.2.3. Show (assuming the other axioms of set theory) that the universal specification axiom, Axiom 3.8, is equivalent to an axiom postulating the existence of a “universal set” Ω consisting of all objects (i.e., for all objects x, we have $x \in \Omega )$ . In other words, if Axiom 3.8 is true, then a universal set exists, and conversely, if a universal set exists, then Axiom 3.8 is true. (This may explain why Axiom 3.8 is called the axiom of universal specification). Note that if a universal set Ω existed, then we would have $\Omega \in \Omega$ by Axiom 3.1, contradicting Exercise 3.2.2. Thus the axiom of foundation specifically rules out the axiom of universal specification. 

## 3.3 Functions

In order to do analysis, it is not particularly useful to just have the notion of a set; we also need the notion of a function from one set to another. Informally, a function $f : X \to Y$ from one set $X$ to another set $Y$ is an operation which assigns to each element $( \mathrm { o r } \ \mathrm { \ddot { \ s i n p u t { \vec { \nu } } } } )$ x in $X$ , a single element $( \mathrm { o r \ o u t p u t ^ { \prime \prime } } ) \ f ( x )$ in $Y ;$ ; we have already used this informal concept in the previous chapter when we discussed the natural numbers. The formal definition is as follows. 

Definition 3.3.1 (Functions). Let X, Y be sets, and let $P ( x , y )$ be a property pertaining to an object $x \in X$ and an object $y \in Y$ , such that for every $x \in X$ , there is exactly one $y \in Y$ for which $P ( x , y )$ is true (this is sometimes known as the vertical line test). Then we define the function $f : X \to Y$ defined by $P$ on the domain X and range $Y$ to be the object which, given any input $x \in X$ , assigns an output $f ( x ) \in Y$ 4 defined to be the unique object $f ( x )$ for which $P ( x , f ( x ) )$ is true. Thus, for any $x \in X$ and $y \in Y$ 2 

$$
y = f (x) \iff P (x, y) \text {   is   true. }
$$

Functions are also referred to as maps or transformations, depending on the context. They are also sometimes called morphisms, although to be more precise, a morphism refers to a more general class of object, which may or may not correspond to actual functions, depending on the context. 

Example 3.3.2. Let $X = \mathbf { N } , Y = \mathbf { N }$ , and let $P ( x , y )$ be the property that $y = x { + } +$ . Then for each $x \in \mathbf { N }$ there is exactly one y for which $P ( x , y )$ is true, namely $y = x { + } +$ . Thus we can define a function $f : \mathbf { N } $ N associated to this property, so that $f ( x ) = x { \mathrel { + } } +$ for all $x ;$ this is the increment function on N, which takes a natural number as input and returns its increment as output. Thus for instance $f ( 4 ) = 5 , f ( 2 n + 3 ) =$ $2 n + 4$ and so forth. One might also hope to define a decrement function $g : \mathbf { N }  \mathbf { N }$ associated to the property $P ( x , y )$ defined by $y + + = x , \mathrm { i . e . }$ $g ( x )$ would be the number whose increment is x. Unfortunately this does not define a function, because when $x = 0$ there is no natural number y whose increment is equal to $x$ (Axiom 2.3). On the other hand, we can legitimately define a decrement function $h : \mathbb { N } \backslash \{ 0 \}  \mathbb { N }$ associated to the property $P ( x , y )$ defined by $y + + = x$ , because when $x \in \mathbf { N } \backslash \{ 0 \}$ there is indeed exactly one natural number y such that $y + + = x$ , thanks to Lemma 2.2.10. Thus for instance $h ( 4 ) = 3$ and $h ( 2 n + 3 ) = 2 n + 2$ 4 but $h ( 0 )$ is undefined since 0 is not in the domain $\mathbf { N } \backslash \{ 0 \}$ 

Example 3.3.3. (Informal) This example requires the real numbers R, which we will define in Chapter 5. One could try to define a square root function $\surd : \mathbf { R }  \mathbf { R }$ by associating it to the property $P ( x , y )$ defined by $y ^ { 2 } = x$ , i.e., we would want $\sqrt { x }$ to be the number y such that $y ^ { 2 } = x$ Unfortunately there are two problems which prohibit this definition from actually creating a function. The first is that there exist real numbers x for which $P ( x , y )$ is never true, for instance if $x = - 1$ then there is no real number y such that $y ^ { 2 } = x$ . This problem however can be solved by restricting the domain from R to the right half-line $[ 0 , + \infty )$ . The second problem is that even when $x \in [ 0 , + \infty )$ , it is possible for there to be more than one y in the range R for which $y ^ { 2 } = x .$ , for instance if $x = 4$ then both $y = 2$ and $y = - 2$ obey the property $P ( x , y )$ , i.e., both +2 and 2 are square roots of 4. This problem can however be solved by restricting the range of R to $[ 0 , + \infty )$ . Once one does this, then one can correctly define a square root function $\surd : [ 0 , + \infty )  [ 0 , + \infty )$ using the relation $y ^ { 2 } = x ,$ , thus $\sqrt { x }$ is the unique number $y \in [ 0 , + \infty )$ such that $y ^ { 2 } = x$ 

One common way to define a function is simply to specify its domain, its range, and how one generates the output $f ( x )$ from each input; this is known as an explicit definition of a function. For instance, the function f in Example 3.3.2 could be defined explicitly by saying that f has domain and range equal to N, and $f ( x ) : = x + +$ for all $x \in \mathbf { N }$ . In other cases we only define a function f by specifying what property $P ( x , y )$ links the input x with the output $f ( x )$ ; this is an implicit definition of a function. For instance, the square root function $\sqrt { x }$ in Example 3.3.3 was defined implicitly by the relation $( { \sqrt { x } } ) ^ { 2 } = x $ . Note that an implicit definition is only valid if we know that for every input there is exactly one output which obeys the implicit relation. In many cases we omit specifying the domain and range of a function for brevity, and thus for instance we could refer to the function $f$ in Example 3.3.2 as “the function $f ( x ) : = x { + } + \cdots$ , “the function $x \mapsto x { \mathrel { + } } + { \mathfrak { s } }$ , “the function $x { \mathrel { + { + } } } ^ { \mathfrak { s } }$ or even the extremely abbreviated $^ { 6 6 } { + + } ^ { , 9 }$ . However, too much of this abbreviation can be dangerous; sometimes it is important to know what the domain and range of the function is. 

We observe that functions obey the axiom of substitution: if $x = x ^ { \prime }$ 4 then $f ( x ) = f ( x ^ { \prime } ) ~ \mathrm { ( w h y ? ) }$ . In other words, equal inputs imply equal outputs. On the other hand, unequal inputs do not necessarily ensure unequal outputs, as the following example shows: 

Example 3.3.4. Let $X = \mathbf { N } , Y = \mathbf { N }$ , and let $P ( x , y )$ be the property that $y = 7 .$ Then certainly for every $x \in \textbf { N }$ there is exactly one y for which $P ( x , y )$ is true, namely the number 7. Thus we can create a function $f : \mathbf { N }  \mathbf { N }$ associated to this property; it is simply the constant function which assigns the output of $f ( x ) = 7$ to each input $x \in \mathbf { N }$ . Thus it is certainly possible for diferent inputs to generate the same output. 

Remark 3.3.5. We are now using parentheses () to denote several different things in mathematics; on one hand, we are using them to clarify the order of operations (compare for instance $2 + ( 3 \times 4 ) = 1 4$ with $( 2 + 3 ) \times 4 = 2 0 )$ , but on the other hand we also use parentheses to enclose the argument $f ( x )$ of a function or of a property such as $P ( x )$ However, the two usages of parentheses usually are unambiguous from context. For instance, if a is a number, then $a ( b + c )$ denotes the expression $a \times ( b + c )$ , whereas if $f$ is a function, then $f ( b + c )$ denotes the output of $f$ when the input is $b + c .$ Sometimes the argument of a function is denoted by subscripting instead of parentheses; for instance, a sequence of natural numbers $a _ { 0 } , a _ { 1 } , a _ { 2 } , a _ { 3 } , \dots .$ is, strictly speaking, a function from N to N, but is denoted by $n \mapsto a _ { n }$ rather than $n \mapsto a ( n )$ 

Remark 3.3.6. Strictly speaking, functions are not sets, and sets are not functions; it does not make sense to ask whether an object x is an element of a function $f ,$ , and it does not make sense to apply a set A to an input x to create an output $A ( x )$ On the other hand, it is possible to start with a function $f : X \to Y$ and construct its graph $\{ ( x , f ( x ) ) : x \in X \}$ , which describes the function completely: see Section 3.5. 

We now define some basic concepts and notions for functions. The first notion is that of equality. 

Definition 3.3.7 (Equality of functions). Two functions $f : X \to Y$ 2 $g : X \to Y$ with the same domain and range are said to be equal, $f = g$ if and only if $f ( x ) = g ( x )$ for all $x \in X$ . (If f(x) and $g ( x )$ agree for some values of $x ,$ but not others, then we do not consider f and $g$ to be $\mathrm { \ e q u a l ^ { 2 } }$ .) 

Example 3.3.8. The functions $x \mapsto x ^ { 2 } + 2 x + 1$ and $x \mapsto ( x + 1 ) ^ { 2 }$ are equal on the domain R. The functions $x \mapsto x$ and $x \mapsto | x |$ are equal on the positive real axis, but are not equal on $\mathbf { R } ;$ thus the concept of equality of functions can depend on the choice of domain. 

Example 3.3.9. A rather boring example of a function is the empty function $f : \varnothing \to X$ from the empty set to an arbitrary set $X$ . Since the empty set has no elements, we do not need to specify what f does to any input. Nevertheless, just as the empty set is a set, the empty function is a function, albeit not a particularly interesting one. Note that for each set X, there is only one function from $\varnothing$ to $X$ , since Definition 3.3.7 asserts that all functions from $\varnothing$ to $X$ are equal (why?). 

This notion of equality obeys the usual axioms (Exercise 3.3.1). 

A fundamental operation available for functions is composition. 

Definition 3.3.10 (Composition). Let $f : X \to Y$ and $g : Y  Z$ be two functions, such that the range of f is the same set as the domain of $g .$ We then define the composition $g \circ f : X \to Z$ of the two functions g and $f$ to be the function defined explicitly by the formula 

$$
(g \circ f) (x) := g (f (x)).
$$

If the range of $f$ does not match the domain of $g _ { \colon }$ , we leave the composition $g \circ f$ undefined. 

It is easy to check that composition obeys the axiom of substitution (Exercise 3.3.1). 

Example 3.3.11. Let $f : \mathbf { N }  \mathbf { N }$ be the function $f ( n ) : = 2 n$ , and let $g : \mathbf { N }  \mathbf { N }$ be the function $g ( n ) : = n + 3$ . Then $g \circ f$ is the function 

$$
g \circ f (n) = g (f (n)) = g (2 n) = 2 n + 3,
$$

thus for instance $g \circ f ( 1 ) = 5 , g \circ f ( 2 ) = 7$ , and so forth. Meanwhile, $f \circ g$ is the function 

$$
f \circ g (n) = f (g (n)) = f (n + 3) = 2 (n + 3) = 2 n + 6,
$$

thus for instance $f \circ g ( 1 ) = 8 , f \circ g ( 2 ) = 1 0$ , and so forth. 

## 3.3. Functions

The above example shows that composition is not commutative: f g and $g \circ f$ are not necessarily the same function. However, composition is still associative: 

Lemma 3.3.12 (Composition is associative). Let $f : Z \to W , g : Y \to$ $Z ,$ and $h : X \to Y$ be functions. Then $f \circ ( g \circ h ) = ( f \circ g ) \circ h$ 

Proof. Since $g \circ h$ is a function from X to $Z , f \circ ( g \circ h )$ is a function from X to W. Similarly $f \circ g$ is a function from Y to W, and hence $( f \circ g ) \circ h$ is a function from X to W. Thus $f \circ ( g \circ h )$ and $( f \circ g ) \circ h$ have the same domain and range. In order to check that they are equal, we see from Definition 3.3.7 that we have to verify that $( f \circ ( g \circ h ) ) ( x ) = ( ( f \circ g ) \circ h ) ( x )$ for all $x \in X$ . But by Definition 3.3.10 

$$
\begin{array}{r l} (f \circ (g \circ h)) (x) & = f ((g \circ h) (x)) \\ & = f (g (h (x)) \\ & = (f \circ g) (h (x)) \\ & = ((f \circ g) \circ h) (x) \end{array}
$$

as desired. 

Remark 3.3.13. Note that while g appears to the left of f in the expression $g \circ f .$ , the function $g \circ f$ applies the right-most function f first, before applying $g .$ . This is often confusing at first; it arises because we traditionally place a function f to the left of its input x rather than to the right. (There are some alternate mathematical notations in which the function is placed to the right of the input, thus we would write xf instead of $f ( x )$ , but this notation has often proven to be more confusing than clarifying, and has not as yet become particularly popular.) 

We now describe certain special types of functions: one-to-one functions, onto functions, and invertible functions. 

Definition 3.3.14 (One-to-one functions). A function $f$ is one-to-one (or injective) if diferent elements map to diferent elements: 

$$
x \neq x ^ {\prime} \quad \Longrightarrow \quad f (x) \neq f (x ^ {\prime}).
$$

Equivalently, a function is one-to-one if 

$$
f (x) = f \left(x ^ {\prime}\right) \quad \Longrightarrow \quad x = x ^ {\prime}.
$$

Example 3.3.15. (Informal) The function $f : \textbf { Z } \to \textbf { Z }$ defined by $f ( n ) : = n ^ { 2 }$ is not one-to-one because the distinct elements 1, 1 map to the same element 1. On the other hand, if we restrict this function to the natural numbers, defining the function $g : \mathbf { N }  \mathbf { Z }$ by $g ( n ) : = n ^ { 2 }$ , then $g$ is now a one-to-one function. Thus the notion of a one-to-one function depends not just on what the function does, but also what its domain is. 

Remark 3.3.16. If a function $f : X \to Y$ is not one-to-one, then one can find distinct $x$ and $x ^ { \prime }$ in the domain X such that $f ( x ) = f ( x ^ { \prime } )$ , thus one can find two inputs which map to one output. Because of this, we say that $f$ is two-to-one instead of one-to-one. 

Definition 3.3.17 (Onto functions). A function f is onto (or surjective) if $f ( X ) = Y , \operatorname { i . e . }$ , every element in Y comes from applying $f$ to some element in X: 

For every $y \in Y ,$ , there exists $x \in X$ such that $f ( x ) = y$ 

Example 3.3.18. (Informal) The function $f : \textbf { Z } \to \textbf { Z }$ defined by $f ( n ) : = n ^ { 2 }$ is not onto because the negative numbers are not in the image of $f$ . However, if we restrict the range Z to the set $A : = \{ n ^ { 2 } : n \in \mathbf { Z } \}$ of square numbers, then the function $g : \mathbf { Z }  A$ defined by $g ( n ) : = n ^ { 2 }$ is now onto. Thus the notion of an onto function depends not just on what the function does, but also what its range is. 

Remark 3.3.19. The concepts of injectivity and surjectivity are in many ways dual to each other; see Exercises 3.3.2, 3.3.4, 3.3.5 for some evidence of this. 

Definition 3.3.20 (Bijective functions). Functions $f : X \to Y$ which are both one-to-one and onto are also called bijective or invertible. 

Example 3.3.21. Let $f : \{ 0 , 1 , 2 \}  \{ 3 , 4 \}$ be the function $f ( 0 ) : = 3$ $f ( 1 ) : = 3 , f ( 2 ) : = 4$ . This function is not bijective because if we set $y = 3$ , then there is more than one x in 0, 1, 2 such that $f ( x ) = y$ (this is a failure of injectivity). Now let $g : \{ 0 , 1 \}  \{ 2 , 3 , 4 \}$ be the function $g ( 0 ) : = 2 , g ( 1 ) : = 3 ;$ then g is not bijective because if we set $y = 4$ , then there is no x for which $g ( x ) = y$ (this is a failure of surjectivity). Now let $h : \{ 0 , 1 , 2 \}  \{ 3 , 4 , 5 \}$ be the function $h ( 0 ) : = 3 , h ( 1 ) : = 4$ , $h ( 2 ) : = 5$ . Then h is bijective, because each of the elements 3, 4, 5 comes from exactly one element from 0, 1, 2. 

Example 3.3.22. The function $f : \mathbf { N }  \mathbf { N } \backslash \{ 0 \}$ defined by $f ( n ) : =$ $^ { n + + }$ is a bijection (in fact, this fact is simply restating Axioms 2.2, 2.3, 2.4). On the other hand, the function $g : \mathbf { N }  \mathbf { N }$ defined by the same definition $g ( n ) : = n { + } +$ is not a bijection. Thus the notion of a bijective function depends not just on what the function does, but also what its range (and domain) are. 

Remark 3.3.23. If a function $x \mapsto f ( x )$ is bijective, then we sometimes call f a perfect matching or a one-to-one correspondence (not to be confused with the notion of a one-to-one function), and denote the action of f using the notation $x  f ( x )$ instead of $x \mapsto f ( x )$ . Thus for instance the function h in the above example is the one-to-one correspondence $0  3 , 1  4 , 2  5$ 

Remark 3.3.24. A common error is to say that a function $f : X \to Y$ is bijective if “for every x in X, there is exactly one y in $Y$ such that $y = f ( x ) .$ .” This is not what it means for f to be bijective; rather, this is merely stating what it means for f to be a function. A function cannot map one element to two diferent elements, for instance one cannot have a function f for which $f ( 0 ) = 1$ and also $f ( 0 ) = 2$ . The functions f, g given in the previous example are not bijective, but they are still functions, since each input still gives exactly one output. 

If f is bijective, then for every $y \in Y$ , there is exactly one x such that $f ( x ) = y$ (there is at least one because of surjectivity, and at most one because of injectivity). This value of x is denoted $f ^ { - 1 } ( y )$ ; thus $f ^ { - 1 }$ is a function from Y to X. We call $f ^ { - 1 }$ the inverse of $f$ . 

$$
- \text { Exercises } -
$$

Exercise 3.3.1. Show that the definition of equality in Definition 3.3.7 is reflexive, symmetric, and transitive. Also verify the substitution property: if $f , { \tilde { f } } : X \to Y$ and $g , \tilde { g } : Y \to Z$ are functions such that $f = { \tilde { f } }$ and $g = \tilde { g }$ , then $g \circ f = \tilde { g } \circ \tilde { f }$ 

Exercise 3.3.2. Let $f : X \to Y$ and $g : Y  Z$ be functions. Show that if f and g are both injective, then so is $g \circ f$ ; similarly, show that if $f$ and $g$ are both surjective, then so is $g \circ f$ 

Exercise 3.3.3. When is the empty function injective? surjective? bijective? 

Exercise 3.3.4. In this section we give some cancellation laws for composition. Let $f : X \to Y , \tilde { f } : X \to Y , g : Y \to Z$ , and ${ \tilde { g } } : Y \to Z$ be functions. Show that if $g \circ f = g \circ { \tilde { f } }$ and $g$ is injective, then $f = { \tilde { f } }$ . Is the same statement true if g is not injective? Show that if $g \circ f = \tilde { g } \circ f$ and $f$ is surjective, then $g = \tilde { g }$ Is the same statement true if $f$ is not surjective? 

Exercise 3.3.5. Let $f : X \to Y$ and $g : Y  Z$ be functions. Show that if $g \circ f$ is injective, then $f$ must be injective. Is it true that $g$ must also be injective? Show that if $g \circ f$ is surjective, then $g$ must be surjective. Is it true that $f$ must also be surjective? 

Exercise 3.3.6. Let $f : X \to Y$ be a bijective function, and let $f ^ { - 1 } : Y \to X$ be its inverse. Verify the cancellation laws $f ^ { - 1 } ( f ( x ) ) = x$ for all $x \in X$ and $f ( f ^ { - 1 } ( y ) ) = y$ for all $y \in Y$ . Conclude that $f ^ { - 1 }$ is also invertible, and has $f$ as its inverse (thus $( f ^ { - 1 } ) ^ { - 1 } = f )$ 

Exercise 3.3.7. Let $f : X \to Y$ and $g : Y  Z$ be functions. Show that if $f$ and g are bijective, then so is $g \circ f .$ , and we have $( g \circ f ) ^ { - 1 } = f ^ { - 1 } \circ g ^ { - 1 }$ 

Exercise 3.3.8. If X is a subset of Y, let $\iota _ { X  Y } : X  Y$ be the inclusion map from X to Y, defined by mapping $x \mapsto x$ for all $x \in X , { \mathrm { i . e . , ~ } } \iota _ { X  Y } ( x ) : = x$ for all $x \in X$ . The map $\ell X {  } X$ is in particular called the identity map on $X$ 

(a) Show that if $X \subseteq Y \subseteq Z$ then $\iota _ { Y  Z } \circ \iota _ { X  Y } = \iota _ { X  Z } .$ 

(b) Show that if $f : A  B$ is any function, then $f = f \circ \iota _ { A  A } = \iota _ { B  B } \circ f .$ 

(c) Show that, if $f : A  B$ is a bijective function, then $f \circ f ^ { - 1 } = \iota _ { B \to B }$ and $f ^ { - 1 } \circ f = \iota _ { A  A }$ 

(d) Show that if X and Y are disjoint sets, and $f : X \to Z$ and $g : Y  Z$ are functions, then there is a unique function $h : X \cup Y  Z$ such that $h \circ \iota _ { X  X \cup Y } = f$ and $h \circ \iota _ { Y  X \cup Y } = g .$ 

## 3.4 Images and inverse images

We know that a function $f : X \to Y$ from a set X to a set $Y$ can take individual elements $x \in X$ to elements $f ( x ) \in Y$ . Functions can also take subsets in X to subsets in $Y$ : 

Definition 3.4.1 (Images of sets). If $f : X \to Y$ is a function from X to $Y$ , and S is a set in X, we define $f ( S )$ to be the set 

$$
f (S) := \{f (x): x \in S \};
$$

this set is a subset of $Y$ , and is sometimes called the image of $S$ under the map $f .$ . We sometimes call $f ( S )$ the forward image of $S$ to distinguish it from the concept of the inverse image $f ^ { - 1 } ( S )$ of S, which is defined below. 

Note that the set $f ( S )$ is well-defined thanks to the axiom of replacement (Axiom 3.6). One can also define $f ( S )$ using the axiom of specification (Axiom 3.5) instead of replacement, but we leave this as a challenge to the reader. 

Example 3.4.2. If $f : \mathbf { N }  \mathbf { N }$ is the map $f ( x ) = 2 x$ , then the forward image of 1, 2, 3 is 2, 4, 6 : 

$$
f (\{1, 2, 3 \}) = \{2, 4, 6 \}.
$$

More informally, to compute $f ( S )$ , we take every element x of S, and apply $f$ to each element individually, and then put all the resulting objects together to form a new set. 

In the above example, the image had the same size as the original set. But sometimes the image can be smaller, because $f$ is not one-to-one (see Definition 3.3.14): 

Example 3.4.3. (Informal) Let Z be the set of integers (which we will define rigorously in the next section) and let $f : \mathbf { Z }  \mathbf { Z }$ be the map $f ( x ) = x ^ { 2 }$ , then 

$$
f (\{- 1, 0, 1, 2 \}) = \{0, 1, 4 \}.
$$

Note that $f$ is not one-to-one because $f ( - 1 ) = f ( 1 )$ 

Note that 

$$
x \in S \implies f (x) \in f (S)
$$

but in general 

$$
f (x) \in f (S) \nRightarrow x \in S;
$$

for instance in the above informal example, $f ( - 2 )$ lies in the set $f ( \{ - 1 , 0 , 1 , 2 \} )$ , but 2 is not in $\{ - 1 , 0 , 1 , 2 \}$ . The correct statement is 

$$
y \in f (S) \iff y = f (x) \text {   for   some   } x \in S
$$

(why?). 

Definition 3.4.4 (Inverse images). If U is a subset of $Y$ , we define the set $f ^ { - 1 } ( U )$ to be the set 

$$
f ^ {- 1} (U) := \{x \in X: f (x) \in U \}.
$$

In other words, $f ^ { - 1 } ( U )$ consists of all the elements of X which map into $U$ 

$$
f (x) \in U \iff x \in f ^ {- 1} (U).
$$

We call $f ^ { - 1 } ( U )$ the inverse image of U. 

Example 3.4.5. If $f : \mathbf { N }  \mathbf { N }$ is the map $f ( x ) = 2 x$ , then $f ( \{ 1 , 2 , 3 \} ) =$ $\{ 2 , 4 , 6 \}$ , but $f ^ { - 1 } ( \{ 1 , 2 , 3 \} ) = \{ 1 \}$ . Thus the forward image of $\{ 1 , 2 , 3 \}$ and the backwards image of $\{ 1 , 2 , 3 \}$ are quite diferent sets. Also note that 

$$
f (f ^ {- 1} (\{1, 2, 3 \})) \neq \{1, 2, 3 \}
$$

(why?). 

Example 3.4.6. (Informal) If $f : \mathbf { Z } \to \mathbf { Z }$ is the map $f ( x ) = x ^ { 2 }$ , then 

$$
f ^ {- 1} (\{0, 1, 4 \}) = \{- 2, - 1, 0, 1, 2 \}.
$$

Note that $f$ does not have to be invertible in order for $f ^ { - 1 } ( U )$ to make sense. Also note that images and inverse images do not quite invert each other, for instance we have 

$$
f ^ {- 1} (f (\{- 1, 0, 1, 2 \})) \neq \{- 1, 0, 1, 2 \}
$$

(why?). 

Remark 3.4.7. If $f$ is a bijective function, then we have defined $f ^ { - 1 }$ in two slightly diferent ways, but this is not an issue because both definitions are equivalent (Exercise 3.4.1). 

As remarked earlier, functions are not sets. However, we do consider functions to be a type of object, and in particular we should be able to consider sets of functions. In particular, we should be able to consider the set of $a l l$ functions from a set $X$ to a set Y. To do this we need to introduce another axiom to set theory: 

Axiom 3.10 (Power set axiom). Let X and Y be sets. Then there exists a set, denoted $\dot { Y } ^ { X }$ , which consists of all the functions from X to $Y$ , thus 

$$
f \in Y ^ {X} \iff (f \text {   is   a   function   with   domain   } X \text {   and   range   } Y).
$$

Example 3.4.8. Let $X = \{ 4 , 7 \}$ and ${ \cal Y } = \{ 0 , 1 \}$ . Then the set $Y ^ { X }$ consists of four functions: the function that maps $4 \mapsto 0$ and $7 \mapsto 0 ;$ the function that maps $4 \mapsto 0$ and $^ { 7 } \mapsto 1$ ; the function that maps $4 \mapsto 1$ and $7 \mapsto 0 ;$ and the function that maps $4 \mapsto 1$ and $^ { 7 } \mapsto 1$ . The reason we use the notation $Y ^ { X }$ to denote this set is that if Y has n elements and X has m elements, then one can show that $Y ^ { X }$ has $n ^ { m }$ elements; see Proposition 3.6.14(f). 

One consequence of this axiom is 

## Lemma 3.4.9. Let X be a set. Then the set

## Y : Y is a subset of X

is a set. 

Proof. See Exercise 3.4.6. 

Remark 3.4.10. The set $\{ Y \ : \ Y$ is a subset of X is known as the power set of X and is denoted $2 ^ { X }$ . For instance, if $a , b , c$ are distinct objects, we have 

$$
2 ^ {\{a, b, c \}} = \{\emptyset , \{a \}, \{b \}, \{c \}, \{a, b \}, \{a, c \}, \{b, c \}, \{a, b, c \} \}.
$$

Note that while $\{ a , b , c \}$ has 3 elements, $2 ^ { \{ a , b , c \} }$ has $2 ^ { 3 } = 8$ elements. This gives a hint as to why we refer to the power set of X as $2 ^ { X }$ ; we return to this issue in Chapter 8. 

For sake of completeness, let us now add one further axiom to our set theory, in which we enhance the axiom of pairwise union to allow unions of much larger collections of sets. 

Axiom 3.11 (Union). Let A be a set, all of whose elements are themselves sets. Then there exists a set A whose elements are precisely those objects which are elements of the elements of A, thus for all objects x 

$$
x \in \bigcup A \iff (x \in S f o r s o m e S \in A).
$$

Example 3.4.11. If $A = \{ \{ 2 , 3 \} , \{ 3 , 4 \} , \{ 4 , 5 \} \}$ , then $\bigcup A = \{ 2 , 3 , 4 , 5 \}$ $\mathrm { \left( w h y ? \right) }$ 

The axiom of union, combined with the axiom of pair set, implies the axiom of pairwise union (Exercise 3.4.8). Another important consequence of this axiom is that if one has some set I, and for every element $\alpha \in I$ we have some set $A _ { \alpha }$ , then we can form the union set $\textstyle \bigcup _ { \alpha \in I } A _ { \alpha }$ by defining 

$$
\bigcup_ {\alpha \in I} A _ {\alpha} := \bigcup \{A _ {\alpha}: \alpha \in I \},
$$

which is a set thanks to the axiom of replacement and the axiom of union. Thus for instance, if $I = \{ 1 , 2 , 3 \} , A _ { 1 } : = \{ 2 , 3 \} , A _ { 2 } : = \{ 3 , 4 \}$ , and 

$A _ { 3 } : = \{ 4 , 5 \}$ , then $\textstyle \bigcup _ { \alpha \in \{ 1 , 2 , 3 \} } A _ { \alpha } = \{ 2 , 3 , 4 , 5 \}$ . More generally, we see that for any object $y _ { \mathrm { i } }$ , 

$$
y \in \bigcup_ {\alpha \in I} A _ {\alpha} \iff (y \in A _ {\alpha} \text { for   some } \alpha \in I).\tag{3.2}
$$

In situations like this, we often refer to I as an index set, and the elements α of this index set as labels; the sets $A _ { \alpha }$ are then called a family of sets, and are indexed by the labels $\alpha \in I$ . Note that if I was empty, then $\textstyle \bigcup _ { \alpha \in I } A _ { \alpha }$ would automatically also be empty (why?). 

We can similarly form intersections of families of sets, as long as the index set is non-empty. More specifical $\lfloor \mathrm { y } ,$ given any non-empty set $I ,$ and given an assignment of a set $A _ { \alpha }$ to each $\alpha \in I$ , we can define the intersection $\cap _ { \alpha \in I } A _ { \alpha }$ by first choosing some element $\beta$ of I (which we can do since I is non-empty), and setting 

$$
\bigcap_ {\alpha \in I} A _ {\alpha} := \{x \in A _ {\beta}: x \in A _ {\alpha} \text {for all} \alpha \in I \},\tag{3.3}
$$

which is a set by the axiom of specification. This definition may look like it depends on the choice of $\beta _ { i }$ , but it does not (Exercise 3.4.9). Observe that for any object $y .$ 

$$
y \in \bigcap_ {\alpha \in I} A _ {\alpha} \iff (y \in A _ {\alpha} \text {   for   all   } \alpha \in I)\tag{3.4}
$$

(compare with (3.2)). 

Remark 3.4.12. The axioms of set theory that we have introduced (Axioms 3.1-3.11, excluding the dangerous Axiom 3.8) are known as theZermelo-Fraenkel axioms of set $t h e o r y ^ { 3 }$ , after Ernest Zermelo (1871– 1953) and Abraham Fraenkel (1891–1965). There is one further axiom we will eventually need, the famous axiom of choice (see Section 8.4), giving rise to the Zermelo-Fraenkel-Choice $( Z F C )$ axioms of set theory, but we will not need this axiom for some time. 

$$
- \text { Exercises } -
$$

Exercise 3.4.1. Let $f : X \to Y$ be a bijective function, and let $f ^ { - 1 } : Y \to X$ be its inverse. Let V be any subset of Y. Prove that the forward image of V under $f ^ { - 1 }$ is the same set as the inverse image of V under $f ;$ thus the fact that both sets are denoted by $f ^ { - 1 } ( V )$ will not lead to any inconsistency. 

Exercise 3.4.2. Let $f : X \to Y$ be a function from one set $X$ to another set $Y ,$ let $S$ be a subset of X, and let U be a subset of $Y$ . What, in general, can one say about $f ^ { - 1 } ( f ( S ) )$ and S? What about $f ( f ^ { - 1 } ( U ) )$ and $U ?$ 

Exercise 3.4.3. Let A, B be two subsets of a set $X$ , and let $f : X \to Y$ be a function. Show that $f ( A \cap B ) \subseteq f ( A ) \cap f ( B )$ , that $f ( A ) \backslash f ( B ) \subseteq f ( A \backslash B )$ , $f ( A \cup B ) = f ( A ) \cup f ( B )$ . For the first two statements, is it true that the $\subseteq$ relation can be improved to =? 

Exercise 3.4.4. Let $f : X \to Y$ be a function from one set X to another set $Y$ and let U, V be subsets of Y. Show that $f ^ { - 1 } ( U \cup V ) = f ^ { - 1 } ( U ) \cup f ^ { - 1 } ( V )$ , that $f ^ { - 1 } ( U \cap V ) = f ^ { - 1 } ( U ) \cap f ^ { - 1 } ( V )$ , and that $f ^ { - 1 } ( U \backslash V ) = f ^ { - 1 } ( U ) \backslash f ^ { - 1 } ( V )$ 

Exercise 3.4.5. Let $f : X \to Y$ be a function from one set X to another set $Y$ Show that $f ( f ^ { - 1 } ( S ) ) = S$ for every $S \subseteq Y$ if and only if f is surjective. Show that $f ^ { - 1 } ( f ( S ) ) = { \dot { S } }$ for every $S \subseteq X$ if and only if $f$ is injective. 

Exercise 3.4.6. Prove Lemma 3.4.9. (Hint: start with the set $\{ 0 , 1 \} ^ { X }$ and apply the replacement axiom, replacing each function $f$ with the object $f ^ { - 1 } ( \{ 1 \} ) . )$ See also Exercise 3.5.11. 

Exercise 3.4.7. Let $X , Y$ be sets. Define a partial function from $X$ to $Y$ to be any function $f : X ^ { \prime } \to Y ^ { \prime }$ whose domain $X ^ { \prime }$ is a subset of X, and whose range $Y ^ { \prime }$ is a subset of $Y$ . Show that the collection of all partial functions from X to $Y$ is itself a set. (Hint: use Exercise 3.4.6, the power set axiom, the replacement axiom, and the union axiom.) 

Exercise 3.4.8. Show that Axiom 3.4 can be deduced from Axiom 3.1, Axiom 3.3 and Axiom 3.11. 

Exercise 3.4.9. Show that if $\beta$ and $\beta ^ { \prime }$ are two elements of a set $I ,$ and to each $\alpha \in I$ we assign a set $A _ { \alpha }$ , then 

$$
\{x \in A _ {\beta}: x \in A _ {\alpha} \text {   for   all   } \alpha \in I \} = \{x \in A _ {\beta^ {\prime}}: x \in A _ {\alpha} \text {   for   all   } \alpha \in I \},
$$

and so the definition of $\cap _ { \alpha \in I } A _ { \alpha }$ defined in (3.3) does not depend on $\beta$ . Also explain why (3.4) is true. 

Exercise 3.4.10. Suppose that I and J are two sets, and for all $\alpha \in I \cup J$ let $A _ { \alpha }$ be a set. Show that $\begin{array} { r } { ( \bigcup _ { \alpha \in I } A _ { \alpha } ) \cup ( \bigcup _ { \alpha \in J } A _ { \alpha } ) = \bigcup _ { \alpha \in I \cup J } A _ { \alpha } } \end{array}$ . If I and J are non-empty, show that $\begin{array} { r } { ( \bigcap _ { \alpha \in I } \hat { A } _ { \alpha } ) \cap ( \bigcap _ { \alpha \in J } \hat { A } _ { \alpha } ) = \bigcap _ { \alpha \in I \cup J } A _ { \alpha } . } \end{array}$ 

  <sub>Exercise 3.4.11. Let X be a set, let I be a non-empty set, and for all</sub> $\alpha \in I$ let $A _ { \alpha }$ be a subset of $X$ . Show that 

$$
X \backslash \bigcup_ {\alpha \in I} A _ {\alpha} = \bigcap_ {\alpha \in I} (X \backslash A _ {\alpha})
$$

and 

$$
X \backslash \bigcap_ {\alpha \in I} A _ {\alpha} = \bigcup_ {\alpha \in I} (X \backslash A _ {\alpha}).
$$

This should be compared with de Morgan’s laws in Proposition 3.1.28 (although one cannot derive the above identities directly from de Morgan’s laws, as I could be infinite). 

## 3.5 Cartesian products

In addition to the basic operations of union, intersection, and diferencing, another fundamental operation on sets is that of the Cartesian product. 

Definition 3.5.1 (Ordered pair). If x and $y$ are any objects (possibly equal), we define the ordered pair $( x , y )$ to be a new object, consisting of x as its first component and y as its second component. Two ordered pairs $( x , y )$ and $( x ^ { \prime } , y ^ { \prime } )$ are considered equal if and only if both their components match, i.e. 

$$
(x, y) = (x ^ {\prime}, y ^ {\prime}) \iff (x = x ^ {\prime} \text {   and   } y = y ^ {\prime}).\tag{3.5}
$$

This obeys the usual axioms of equality (Exercise 3.5.3). Thus for instance, the pair $( 3 , 5 )$ is equal to the pair $( 2 + 1 , 3 + 2 )$ , but is distinct from the pairs $( 5 , 3 ) , ( 3 , 3 )$ , and (2, 5). (This is in contrast to sets, where 3, 5 and 5, 3 are equal.) 

Remark 3.5.2. Strictly speaking, this definition is partly an axiom, because we have simply postulated that given any two objects x and $y ,$ that an object of the form $( x , y )$ exists. However, it is possible to define an ordered pair using the axioms of set theory in such a way that we do not need any further postulates (see Exercise 3.5.1). 

Remark 3.5.3. We have now “overloaded” the parenthesis symbols () once again; they now are not only used to denote grouping of operators and arguments of functions, but also to enclose ordered pairs. This is usually not a problem in practice as one can still determine what usage the symbols () were intended for from context. 

Definition 3.5.4 (Cartesian product). If X and $Y$ are sets, then we define the Cartesian product $X \times Y$ to be the collection of ordered pairs, whose first component lies in X and second component lies in $Y$ , thus 

$$
X \times Y = \{(x, y): x \in X, y \in Y \}
$$

or equivalently 

$$
a \in (X \times Y) \iff (a = (x, y) \text {   for   some   } x \in X \text {   and   } y \in Y).
$$

Remark 3.5.5. We shall simply assume that our notion of ordered pair is such that whenever X and $Y$ are sets, the Cartesian product $X \times Y$ is also a set. This is however not a problem in practice; see Exercise 3.5.1. 

Example 3.5.6. If $X : = \{ 1 , 2 \}$ and $Y : = \{ 3 , 4 , 5 \}$ , then 

$$
X \times Y = \{(1, 3), (1, 4), (1, 5), (2, 3), (2, 4), (2, 5) \}
$$

and 

$$
Y \times X = \{(3, 1), (4, 1), (5, 1), (3, 2), (4, 2), (5, 2) \}.
$$

Thus, strictly speaking, $X \times Y$ and $Y \times X$ are diferent sets, although they are very similar. For instance, they always have the same number of elements (Exercise 3.6.5). 

Let $f : X \times Y \to Z$ be a function whose domain $X \times Y$ is a Cartesian product of two other sets $X$ and $Y$ . Then $f$ can either be thought of as a function of one variable, mapping the single input of an ordered pair $( x , y )$ in $X \times Y$ to an output $f ( x , y )$ in $Z .$ , or as a function of two variables, mapping an input $x \in X$ and another input $y \in Y$ to a single output $f ( x , y )$ in $Z .$ . While the two notions are technically diferent, we will not bother to distinguish the two, and think of $f$ simultaneously as a function of one variable with domain $X \times Y$ and as a function of two variables with domains $X$ and $Y$ . Thus for instance the addition operation + on the natural numbers can now be re-interpreted as a function $+ : \mathbf { N } \times \mathbf { N }  \mathbf { N }$ , defined by $( x , y ) \mapsto x + y$ 

One can of course generalize the concept of ordered pairs to ordered triples, ordered quadruples, etc: 

Definition 3.5.7 (Ordered n-tuple and n-fold Cartesian product). Let n be a natural number. An ordered n-tuple $( x _ { i } ) _ { 1 \leq i \leq n }$ (also denoted $( x _ { 1 } , \ldots , x _ { n } ) )$ is a collection of objects $x _ { i } ,$ , one for every natural number i between 1 and $n ;$ we refer to $x _ { i }$ as the $i ^ { t h }$ component of the ordered n-tuple. Two ordered n-tuples $( x _ { i } ) _ { 1 \leq i \leq n }$ and $( y _ { i } ) _ { 1 \leq i \leq n }$ are said to be equal if $x _ { i } = y _ { i }$ for all $1 \leq i \leq n$ . If $( X _ { i } ) _ { 1 \leq i \leq n }$ is an ordered n-tuple of sets, we define their Cartesian product $\textstyle \prod _ { 1 \leq i \leq n } X _ { i }$ (also denoted $\Pi _ { i = 1 } ^ { n } X _ { i }$ or $X _ { 1 } \times \ldots \times X _ { n } )$ by 

$$
\prod_ {1 \leq i \leq n} X _ {i} := \{(x _ {i}) _ {1 \leq i \leq n}: x _ {i} \in X _ {i} \text {   for   all   } 1 \leq i \leq n \}.
$$

Again, this definition simply postulates that an ordered n-tuple and a Cartesian product always exist when needed, but using the axioms of set theory one can explicitly construct these objects (Exercise 3.5.2). 

Remark 3.5.8. One can show that $\textstyle \prod _ { 1 \leq i \leq n } X _ { i }$ is indeed a set. Indeed, from the power set axiom we can consider the set of all functions $i \mapsto x _ { i }$ from the domain $\{ 1 \leq i \leq n \}$ to the range $\textstyle \bigcup _ { 1 \leq i \leq n } X _ { i } .$ , and then we can restrict using the axiom of specification to restrict to those functions $i \mapsto x _ { i }$ for which $x _ { i } \ \in \ X _ { i }$ for all $1 \leq i \leq n$ . One can generalize this construction to infinite Cartesian products, see Definition 8.4.1. 

Example 3.5.9. Let $a _ { 1 } , b _ { 1 } , a _ { 2 } , b _ { 2 } , a _ { 3 } , b _ { 3 }$ be objects, and let $X _ { 1 } : =$ $\{ a _ { 1 } , b _ { 1 } \} , X _ { 2 } : = \{ a _ { 2 } , b _ { 2 } \}$ , and $X _ { 3 } : = \{ a _ { 3 } , b _ { 3 } \}$ . Then we have 

$$
\begin{array}{c} X _ {1} \times X _ {2} \times X _ {3} = \{(a _ {1}, a _ {2}, a _ {3}), (a _ {1}, a _ {2}, b _ {3}), (a _ {1}, b _ {2}, a _ {3}), (a _ {1}, b _ {2}, b _ {3}), \\ (b _ {1}, a _ {2}, a _ {3}), (b _ {1}, a _ {2}, b _ {3}), (b _ {1}, b _ {2}, a _ {3}), (b _ {1}, b _ {2}, b _ {3}) \} \\ (X _ {1} \times X _ {2}) \times X _ {3} = \\ \{(((a _ {1}, a _ {2}), a _ {3}), ((a _ {1}, a _ {2}), b _ {3}), ((a _ {1}, b _ {2}), a _ {3}), ((a _ {1}, b _ {2}), b _ {3}), \\ ((b _ {1}, a _ {2}), a _ {3}), ((b _ {1}, a _ {2}), b _ {3}), ((b _ {1}, b _ {2}), a _ {3}), ((b _ {1}, b _ {2}), b _ {3}) \} \\ X _ {1} \times (X _ {2} \times X _ {3}) = \\ \{(a _ {1}, (a _ {2}, a _ {3})), (a _ {1}, (a _ {2}, b _ {3})), (a _ {1}, (b _ {2}, a _ {3})), (a _ {1}, (b _ {2}, b _ {3})), \\ (b _ {1}, (a _ {2}, a _ {3})), (b _ {1}, (a _ {2}, b _ {3})), (b _ {1}, (b _ {2}, a _ {3})), (b _ {1}, (b _ {2}, b _ {3})) \}. \end{array}
$$

Thus, strictly speaking, the sets $X _ { 1 } \times X _ { 2 } \times X _ { 3 } , ( X _ { 1 } \times X _ { 2 } ) \times X _ { 3 }$ , and $X _ { 1 } \times ( X _ { 2 } \times X _ { 3 } )$ are distinct. However, they are clearly very related to each other (for instance, there are obvious bijections between any two of the three sets), and it is common in practice to neglect the minor distinctions between these sets and pretend that they are in fact equal. Thus a function $f : X _ { 1 } \times X _ { 2 } \times X _ { 3 } \to Y$ can be thought of as a function of one variable $( x _ { 1 } , x _ { 2 } , x _ { 3 } ) \in X _ { 1 } { \times } X _ { 2 } { \times } X _ { 3 }$ , or as a function of three variables $x _ { 1 } \in X _ { 1 } , x _ { 2 } \in X _ { 2 } , x _ { 3 } \in X _ { 3 }$ , or as a function of two variables $x _ { 1 } \in X _ { 1 }$ , $( x _ { 2 } , x _ { 3 } ) \in X _ { 2 } \times X _ { 3 }$ , and so forth; we will not bother to distinguish between these diferent perspectives. 

Remark 3.5.10. An ordered n-tuple $x _ { 1 } , \ldots , x _ { n }$ of objects is also called an ordered sequence of n elements, or a finite sequence for short. In Chapter 5 we shall also introduce the very useful concept of an infinite sequence. 

Example 3.5.11. If x is an object, then (x) is a 1-tuple, which we shall identify with x itself (even though the two are, strictly speaking, not the same object). Then if $X _ { 1 }$ is any set, then the Cartesian product $\Pi _ { 1 < i < 1 } X _ { i }$ is just $X _ { 1 }$ (why?). Also, the empty Cartesian product $\Pi _ { 1 \leq i \leq 0 } { \overline { { X _ { i } } } }$ gives, not the empty set , but rather the singleton set $\{ ( ) \}$ whose only element is the 0-tuple (), also known as the empty tuple. 

## 3.5. Cartesian products

If n is a natural number, we often write $X ^ { n }$ as shorthand for the n-fold Cartesian product $\begin{array} { r } { X ^ { n } : = \prod _ { 1 < i < n } X } \end{array}$ . Thus $X ^ { 1 }$ is essentially the same set as X (if we ignore the distinction between an object x and the 1-tuple $( x ) )$ , while $X ^ { 2 }$ is the Cartesian product $X \times X$ . The set $X ^ { 0 }$ is a singleton set $\mathrm { \small { \left\{ \rho \right\} } \left( w h y ? \right) }$ 

We can now generalize the single choice lemma (Lemma 3.1.6) to allow for multiple (but finite) number of choices. 

Lemma 3.5.12 (Finite choice). Let $n \geq 1$ be a natural number, and for each natural number $1 \leq i \leq n$ , let $X _ { i }$ be a non-empty set. Then there exists an n-tuple $( x _ { i } ) _ { 1 \leq i \leq n }$ such that $x _ { i } \in X _ { i }$ for all $1 \leq i \leq n$ In other words, if each $X _ { i }$ is non-empty, then the set $\prod _ { 1 \leq i \leq n } X _ { i }$ is also non-empty. 

Proof. We induct on n (starting with the base case $n = 1$ ; the claim is also vacuously true with $n = 0$ but is not particularly interesting in that case). When $n = 1$ the claim follows from Lemma 3.1.6 (why?). Now suppose inductively that the claim has already been proven for some $n ;$ we will now prove it for $^ { n + + }$ . Let $X _ { 1 } , \ldots , X _ { n + 1 }$ be a collection of nonempty sets. By induction hypothesis, we can find an n-tuple $( x _ { i } ) _ { 1 \leq i \leq n }$ such that $x _ { i } \in X _ { i }$ for all $1 \leq i \leq n$ . Also, since $X _ { n + + }$ is non-empty, by Lemma 3.1.6 we may find an object a such that $a \in X _ { n + 1 }$ . If we thus define the n++-tuple $( y _ { i } ) _ { 1 \leq i \leq n + 1 }$ by setting $y _ { i } : = x _ { i }$ when $1 \leq i \leq n$ and $y _ { i } : = a$ when $i = n { + } + \mathrm { i t }$ is clear that $y _ { i } \in X _ { i }$ for all $1 \leq i \leq n + + ,$ thus closing the induction. □ 

Remark 3.5.13. It is intuitively plausible that this lemma should be extended to allow for an infinite number of choices, but this cannot be done automatically; it requires an additional axiom, the axiom of choice. See Section 8.4. 

## — Exercises —

Exercise 3.5.1. Suppose we define the ordered pair $( x , y )$ for any objects x and y by the formula $( x , y ) : = \{ \{ x \} , \{ x , y \} \}$ (thus using several applications of Axiom 3.3). Thus for instance (1, 2) is the set $\{ \{ 1 \} , \{ 1 , 2 \} \} , \ ( 2 , 1 )$ is the set $\{ \{ 2 \} , \{ 2 , 1 \} \}$ , and (1, 1) is the set 1 . Show that such a definition indeed obeys the property (3.5), and also whenever X and $Y$ are sets, the Cartesian product $X \times Y$ is also a set. Thus this definition can be validly used as a definition of an ordered pair. For an additional challenge, show that the alternate definition $( x , y ) : = \{ x , \{ x , y \} \}$ also verifies (3.5) and is thus also an acceptable definition of ordered pair. (For this latter task one needs the axiom of regularity, and in particular Exercise 3.2.2.) 

Exercise 3.5.2. Suppose we define an ordered n-tuple to be a surjective function $x : \{ i \in \mathbf { N } : 1 \leq i \leq n \}  X$ whose range is some arbitrary set X (so diferent ordered n-tuples are allowed to have diferent ranges); we then write $x _ { i }$ for $x ( i )$ , and also write x as $( x _ { i } ) _ { 1 \leq i \leq n }$ . Using this definition, verify that we have $( x _ { i } ) _ { 1 \leq i \leq n } = ( y _ { i } ) _ { 1 \leq i \leq n }$ if and only if $x _ { i } = y _ { i }$ for all $1 \leq i \leq n$ . Also, show that if $( X _ { i } ) _ { 1 \leq i \leq n }$ are an ordered n-tuple of sets, then the Cartesian product, as defined in Definition 3.5.7, is indeed a set. (Hint: use Exercise 3.4.7 and the axiom of specification.) 

Exercise 3.5.3. Show that the definitions of equality for ordered pair and ordered n-tuple obey the reflexivity, symmetry, and transitivity axioms. 

Exercise 3.5.4. Let A, B, C be sets. Show that $A \times ( B \cup C ) = ( A \times B ) \cup ( A \times C )$ that $A \times ( B \cap C ) = ( A \times B ) \cap ( A \times C )$ , and that $A \times ( B \backslash C ) = ( A \times B ) \backslash ( A \times C )$ (One can of course prove similar identities in which the rˆoles of the left and right factors of the Cartesian product are reversed.) 

Exercise 3.5.5. Let $A , B , C , D$ be sets. Show that $( A \times B ) \cap ( C \times D ) = ( A \cap$ $C ) \times ( B \cap D )$ . Is it true that $( A \times B ) \cup ( C \times D ) = ( A \cup C ) \times ( B \cup D ) ?$ Is it true that $( A \times B ) \backslash ( C \times D ) = ( A \backslash C ) \times ( B \backslash D ) \}$ 

Exercise 3.5.6. Let $A , B , C , D$ be non-empty sets. Show that $A \times B \subseteq C \times D$ if and only if $A \subseteq C$ and $B \subseteq D$ , and that $A \times B = C \times D$ if and only if $A = C$ and $B = D$ . What happens if the hypotheses that the $A , B , C , D$ are all non-empty are removed? 

Exercise 3.5.7. Let X, Y be sets, and let $\pi _ { X \times Y \to X } : X \times Y \to X$ and $\pi _ { X \times Y \to Y } :$ $X \times Y \to Y$ be the maps $\pi _ { \boldsymbol { X } \times \boldsymbol { Y } \to \boldsymbol { X } } ( x , y ) : = x$ and $\pi _ { \boldsymbol { X } \times \boldsymbol { Y } \to \boldsymbol { Y } } ( x , y ) : = y ;$ these maps are known as the co-ordinate functions on $X \times Y$ . Show that for any functions $f : Z \to X$ and $g : Z \to Y$ , there exists a unique function $h : Z \to$ $X \times Y$ such that $\pi _ { X \times Y \to X } \circ h = f$ and $\pi _ { X \times Y \to Y } \circ h = g$ . (Compare this to the last part of Exercise 3.3.8, and to Exercise 3.1.7.) This function h is known as the direct sum of f and g and is denoted $h = f \oplus g$ 

Exercise 3.5.8. Let $X _ { 1 } , \ldots , X _ { n }$ be sets. Show that the Cartesian product $\textstyle \prod _ { i = 1 } ^ { n } X _ { i }$ is empty if and only if at least one of the $X _ { i }$ is empty. 

Exercise 3.5.9. Suppose that I and J are two sets, and for all $\alpha \in I$ let $A _ { \alpha }$ be a set, and for all $\beta \in J$ let $B _ { \beta }$ be a set. Show that $\begin{array} { r l } { ( \bigcup _ { \alpha \in I } A _ { \alpha } ) \cap ( \bigcup _ { \beta \in J } B _ { \beta } ) = } & { { } } \end{array}$ $\cup _ { ( \alpha , \beta ) \in I \times J } ( A _ { \alpha } \cap B _ { \beta } )$ 

Exercise 3.5.10. If $f : X \to Y$ is a function, define the graph of f to be the subset of $X \times Y$ defined by $\{ ( x , f ( x ) ) : x \in X \}$ . Show that two functions $f : X \to Y , { \tilde { f } } : X \to Y$ are equal if and only if they have the same graph. Conversely, if G is any subset of $X \times Y$ with the property that for each $x \in X$ , the set $\{ y \in Y : ( x , y ) \in G \}$ has exactly one element (or in other words, G obeys the vertical line test), show that there is exactly one function $f : X \to Y$ whose graph is equal to G. 

Exercise 3.5.11. Show that Axiom 3.10 can in fact be deduced from Lemma 3.4.9 and the other axioms of set theory, and thus Lemma 3.4.9 can be used as an alternate formulation of the power set axiom. (Hint: for any two sets X and $Y ,$ , use Lemma 3.4.9 and the axiom of specification to construct the set of all subsets of $X \times Y$ which obey the vertical line test. Then use Exercise 3.5.10 and the axiom of replacement.) 

Exercise 3.5.12. This exercise will establish a rigorous version of Proposition 2.1.16. Let $f : \mathbf { N } \times \mathbf { N }  \mathbf { N }$ be a function, and let c be a natural number. Show that there exists a function $a : \mathbf { N } \to \mathbf { N }$ such that 

$$
a (0) = c
$$

and 

$$
a (n + +) = f (n, a (n)) \text {   for   all   } n \in \mathbf {N},
$$

and furthermore that this function is unique. (Hint: first show inductively, by a modification of the proof of Lemma 3.5.12, that for every natural number $N \in \mathbf { N }$ , there exists a unique function a : $\{ n \in \mathbf { N } : n \leq N \} \to \mathbf { N }$ such that $a _ { N } ( 0 ) = c$ and $a _ { N } ( n { + } + ) = f ( n , a ( n ) )$ for all $n \in \mathbf N$ such that $n < N . )$ For an additional challenge, prove this result without using any properties of the natural numbers other than the Peano axioms directly (in particular, without using the ordering of the natural numbers, and without appealing to Proposition 2.1.16). (Hint: first show inductively, using only the Peano axioms and basic set theory, that for every natural number $N \in \mathbf { N }$ , there exists a unique pair $A _ { N } , B _ { N }$ of subsets of N which obeys the following properties: (a) $A _ { N } \cap B _ { N } = \varnothing$ , (b) $A _ { N } \cup B _ { N } = \mathbf { N }$ $( \mathrm { c } ) \ 0 \ \in \ A _ { N }$ , (d) $N + + \ \in \ B _ { N }$ , (e) Whenever $n \in B _ { N } .$ , we have $n + \mathrm { ~ \in ~ } B _ { N }$ . (f) Whenever $n \in A _ { N }$ and $n \neq N ,$ we have $n { + } + \in A _ { N }$ . Once one obtains these sets, use $A _ { N }$ as a substitute for $\{ n \in \mathbf { N } : n \leq N \}$ in the previous argument.) 

Exercise 3.5.13. The purpose of this exercise is to show that there is essentially only one version of the natural number system in set theory (cf. the discussion in Remark 2.1.12). Suppose we have a set $\mathbf { N } ^ { \prime }$ of “alternative natural numbers”, an “alternative $z \mathrm { e r o } ^ { \prime \prime } \ 0 ^ { \prime } .$ , and an “alternative increment operation” which takes any alternative natural number $n ^ { \prime } \in \mathbf { N } ^ { \prime }$ and returns another alternative natural number $n ^ { \prime } { + } { + } ^ { \prime } \in \mathbf { N } ^ { \prime }$ , such that the Peano axioms (Axioms 2.1-2.5) all hold with the natural numbers, zero, and increment replaced by their alternative counterparts. Show that there exists a bijection $f : \mathbf { N }  \mathbf { N } ^ { \prime }$ from the natural numbers to the alternative natural numbers such that $f ( 0 ) = 0 ^ { \prime }$ , and such that for any $n \in \mathbf N$ and $n ^ { \prime } \in \mathbf { N } ^ { \prime }$ , we have $f ( n ) = n ^ { \prime }$ if and only if $f ( n { + } + ) = n ^ { \prime } { + } + ^ { \prime }$ (Hint: use Exercise 3.5.12.) 

## 3.6 Cardinality of sets

In the previous chapter we defined the natural numbers axiomatically, assuming that they were equipped with a 0 and an increment operation, and assuming five axioms on these numbers. Philosophically, this is quite diferent from one of our main conceptualizations of natural numbers - that of cardinality, or measuring how many elements there are in a set. Indeed, the Peano axiom approach treats natural numbers more like ordinals than cardinals. (The cardinals are One, Two, Three, ..., and are used to count how many things there are in a set. The ordinals are First, Second, Third, ..., and are used to order a sequence of objects. There is a subtle diference between the two, especially when comparing infinite cardinals with infinite ordinals, but this is beyond the scope of this text). We paid a lot of attention to what number came next after a given number n - which is an operation which is quite natura for ordinals, but less so for cardinals - but did not address the issue of whether these numbers could be used to count sets. The purpose of this section is to address this issue by noting that the natural numbers can be used to count the cardinality of sets, as long as the set is finite. 

The first thing is to work out when two sets have the same size: it seems clear that the sets 1, 2, 3 and 4, 5, 6 have the same size, but that both have a diferent size from 8, 9 . One way to define this is to say that two sets have the same size if they have the same number of elements, but we have not yet defined what the “number of elements” in a set is. Besides, this runs into problems when a set is infinite. 

The right way to define the concept of “two sets having the same size” is not immediately obvious, but can be worked out with some thought. One intuitive reason why the sets 1, 2, 3 and 4, 5, 6 have the same size is that one can match the elements of the first set with the elements in the second set in a one-to-one correspondence: $1  4$ $2  5 , 3  6$ . (Indeed, this is how we first learn to count a set: we correspond the set we are trying to count with another set, such as a set of fingers on your hand). We will use this intuitive understanding as our rigorous basis for “having the same size”. 

Definition 3.6.1 (Equal cardinality). We say that two sets X and Y have equal cardinality if there exists a bijection $f : X \to Y$ from X to Y. 

Example 3.6.2. The sets 0, 1, 2 and 3, 4, 5 have equal cardinality, since we can find a bijection between the two sets. Note that we do not yet know whether 0, 1, 2 and 3, 4 have equal cardinality; we know that one of the functions f from 0, 1, 2 to 3, 4 is not a bijection, but we have not proven yet that there might still be some other bijection from one set to the other. (It turns out that they do not have equa cardinality, but we will prove this a little later). Note that this definition 

## 3.6. Cardinality of sets

makes sense regardless of whether X is finite or infinite (in fact, we haven’t even defined what finite means yet). 

Remark 3.6.3. The fact that two sets have equal cardinality does not preclude one of the sets from containing the other. For instance, if X is the set of natural numbers and Y is the set of even natural numbers, then the map $f : X \to Y$ defined by $f ( n ) : = 2 n$ is a bijection from X to $Y \ \mathrm { \left( w h y ? \right) }$ , and so X and Y have equal cardinality, despite Y being a subset of X and seeming intuitively as if it should only have “half” of the elements of X. 

The notion of having equal cardinality is an equivalence relation: 

Proposition 3.6.4. Let X, Y, Z be sets. Then X has equal cardinality with X. If X has equal cardinality with Y, then Y has equal cardinality with X. If X has equal cardinality with Y and Y has equal cardinality with Z, then X has equal cardinality with Z. 

Proof. See Exercise 3.6.1. 

Let n be a natural number. Now we want to say when a set X has n elements. Certainly we want the set $\{ i \in \mathbf { N } : 1 \leq i \leq n \} = \{ 1 , 2 , \ldots , n \}$ to have n elements. (This is true even when $n = 0 \cdot$ ; the set $\{ i \in N : 1 \leq$ $i \leq 0 \}$ is just the empty set.) Using our notion of equal cardinality, we thus define: 

Definition 3.6.5. Let n be a natural number. A set X is said to have cardinality n, if it has equal cardinality with $\{ i \in \mathbf { N } : 1 \leq i \leq n \}$ . We also say that X has n elements if it has cardinality n. 

Remark 3.6.6. One can use the set $\{ i \in \mathbf { N } : i < n \}$ instead of $\{ i \in \mathbf { N }$ $1 \leq i \leq n \}$ , since these two sets clearly have equal cardinality. (Why? What is the bijection?) 

Example 3.6.7. Let $a , b , c ,$ d be distinct objects. Then $\{ a , b , c , d \}$ has the same cardinality as $\{ i \in \mathbf { N } : i < 4 \} = \{ 0 , 1 , 2 , 3 \}$ or $\{ i \in \mathbf { N } : 1 \leq i \leq$ $4 \} = \ \{ 1 , 2 , 3 , 4 \}$ and thus has cardinality 4. Similarly, the set a has cardinality 1. 

There might be one problem with this definition: a set might have two diferent cardinalities. But this is not possible: 

Proposition 3.6.8 (Uniqueness of cardinality). Let X be a set with some cardinality n. Then X cannot have any other cardinality, i.e., X cannot have cardinality m for any m $\neq n$ 

Before we prove this proposition, we need a lemma. 

Lemma 3.6.9. Suppose that $n \geq 1$ , and X has cardinality n. Then X is non-empty, and if x is any element of X, then the set $X - \{ x \} \ ( i . e .$ X with the element x removed) has cardinality<sup>4</sup> $n - 1$ 

Proof. If X is empty then it clearly cannot have the same cardinality as the non-empty set $\{ i \in \mathbf { N } : 1 \leq i \leq n \}$ , as there is no bijection from the empty set to a non-empty set $\mathrm { \left( w h y ? \right) }$ . Now let x be an element of X. Since X has the same cardinality as $\{ i \in \mathbf { N } : 1 \leq i \leq N \}$ , we thus have a bijection f from X to $\{ i \in \mathbf { N } : 1 \leq i \leq N \}$ . In particular, $f ( x )$ is a natural number between 1 and n. Now define the function $g : X - \{ x \}$ to $\{ i \in \mathbf { N } : 1 \leq i \leq n - 1 \}$ by the following rule: for any $y \in X - \{ x \}$ , we define $g ( y ) : = f ( y ) { \mathrm { ~ i f ~ } } f ( y ) < f ( x )$ , and define $g ( y ) : = f ( y ) - 1$ if $f ( y ) > f ( x )$ . (Note that $f ( y )$ cannot equal $f ( x )$ since $y \neq x$ and f is a bijection.) It is easy to check that this map is also a bijection (why?), and so $X - \{ x \}$ has equal cardinality with $\{ i \in \mathbf { N } : 1 \leq i \leq n - 1 \}$ . In particular $X - \{ x \}$ has cardinality $n - 1$ , as desired. □ 

Now we prove the proposition. 

Proof of Proposition 3.6.8. We induct on n. First suppose that $n = 0 .$ Then X must be empty, and so X cannot have any non-zero cardinality. Now suppose that the proposition is already proven for some n; we now prove it for $^ { n + + }$ . Let X have cardinality $n { \mathrel { + { + } } } ;$ and suppose that X also has some other cardinality $m \neq n { + } 1$ . By Lemma 3.6.9, X is non-empty, and if x is any element of X, then $X - \{ x \}$ has cardinality n and also has cardinality $m - 1$ , by Lemma 3.6.9. By induction hypothesis, this means that $n = m - 1$ , which implies that $m = n { + } +$ , a contradiction. This closes the induction. □ 

Thus, for instance, we now know, thanks to Propositions 3.6.4 and 3.6.8, that the sets 0, 1, 2 and $\{ 3 , 4 \}$ do not have equal cardinality, since the first set has cardinality 3 and the second set has cardinality 2. 

Definition 3.6.10 (Finite sets). A set is finite if it has cardinality n for some natural number n; otherwise, the set is called infinite. If X is a finite set, we use $\# ( X )$ to denote the cardinality of X. 

Example 3.6.11. The sets $\{ 0 , 1 , 2 \}$ and 3, 4 are finite, as is the empty set (0 is a natural number), and $\# ( \{ 0 , 1 , 2 \} ) = 3 , \# ( \{ 3 , 4 \} ) = 2$ , and $\# ( \emptyset ) = 0$ 

Now we give an example of an infinite set. 

Theorem 3.6.12. The set of natural numbers N is infinite. 

Proof. Suppose for sake of contradiction that the set of natural numbers N was finite, so it had some cardinality $\# ( \mathbf { N } ) = n$ . Then there is a bijection f from $\{ i \in \mathbf { N } : 1 \leq i \leq n \}$ to N. One can show that the sequence $f ( 1 ) , f ( 2 ) , \dots , f ( n )$ is bounded, or more precisely that there exists a natural number M such that $f ( i ) \ \leq \ M$ for all $1 \leq i \leq n$ (Exercise 3.6.3). But then the natural number $M + 1$ is not equal to any of the f(i), contradicting the hypothesis that f is a bijection. □ 

Remark 3.6.13. One can also use similar arguments to show that any unbounded set is infinite; for instance the rationals Q and the reals R (which we will construct in later chapters) are infinite. However, it is possible for some sets to be “more” infinite than others; see Section 8.3. 

Now we relate cardinality with the arithmetic of natural numbers. 

Proposition 3.6.14 (Cardinal arithmetic). 

(a) Let X be a finite set, and let x be an object which is not an element of X. Then $X \cup \{ x \}$ is finite and $\# ( X \cup \{ x \} ) = \# ( X ) + 1$ 

(b) Let X and Y be finite sets. Then $X \cup Y$ is finite and $\# ( X \cup$ $Y ) \leq \# ( X ) + \# ( Y )$ . If in addition X and Y are disjoint (i.e., $X \cap Y = \varnothing )$ , then $\# ( X \cup Y ) = \# ( X ) + \# ( Y )$ 

(c) Let X be a finite set, and let Y be a subset of X. Then Y is finite, and $\# ( Y ) \leq \# ( X )$ . If in addition $Y \neq X ( i . e . , Y$ is a proper subset of X), then we have $\# ( Y ) < \# ( X )$ 

(d) If X is a finite set, and $f : X \to Y$ is a function, then $f ( X )$ is a finite set with $\# ( f ( X ) ) \leq \# ( X )$ . If in addition f is one-to-one, then $\# ( f ( X ) ) = \# ( X )$ 

(e) Let X and Y be finite sets. Then Cartesian product $X \times Y$ is finite and # $( X \times Y ) = \# ( X ) \times \# ( Y )$ 

(f) Let X and Y be finite sets. Then the set $Y ^ { X }$ (defined in Axiom 3.10) is finite and $\# ( Y ^ { X } ) = \# ( Y ) \# ( X )$ 

Proof. See Exercise 3.6.4. 

Remark 3.6.15. Proposition 3.6.14 suggests that there is another way to define the arithmetic operations of natural numbers; not defined recursively as in Definitions 2.2.1, 2.3.1, 2.3.11, but instead using the notions of union, Cartesian product, and power set. This is the basis of cardinal arithmetic, which is an alternative foundation to arithmetic than the Peano arithmetic we have developed here; we will not develop this arithmetic in this text, but we give some examples of how one would work with this arithmetic in Exercises 3.6.5, 3.6.6. 

This concludes our discussion of finite sets. We shall discuss infinite sets in Chapter 8, once we have constructed a few more examples of infinite sets (such as the integers, rationals and reals). 

— Exercises — 

Exercise 3.6.1. Prove Proposition 3.6.4. 

Exercise 3.6.2. Show that a set X has cardinality 0 if and only if X is the empty set. 

Exercise 3.6.3. Let n be a natural number, and let $f : \{ i \in \mathbf { N } : 1 \leq i \leq n \}  \mathbf { N }$ be a function. Show that there exists a natural number M such that $f ( i ) \leq M$ for all $1 \leq i \leq n$ . (Hint: induct on n. You may also want to peek at Lemma 5.1.14.) Thus finite subsets of the natural numbers are bounded. 

Exercise 3.6.4. Prove Proposition 3.6.14. 

Exercise 3.6.5. Let A and B be sets. Show that $A \times B$ and $B \times A$ have equal cardinality by constructing an explicit bijection between the two sets. Then use Proposition 3.6.14 to conclude an alternate proof of Lemma 2.3.2. 

Exercise 3.6.6. Let A, B, C be sets. Show that the sets $( A ^ { B } ) ^ { C }$ and $A ^ { B \times C }$ have equal cardinality by constructing an explicit bijection between the two sets. Conclude that $( a ^ { b } ) ^ { c } = a ^ { b c }$ for any natural numbers $a , b , c .$ . Use a similar argument to also conclude $a ^ { b } \times a ^ { c } = a ^ { b + c }$ 

Exercise 3.6.7. Let A and B be sets. Let us say that A has lesser or equal cardinality to B if there exists an injection $f : A  B$ from A to B. Show that if A and B are finite sets, then A has lesser or equal cardinality to B if and only if # $\mathsf { \Pi } _ { \mathsf { \Phi } } ^ { L } ( A ) \leq \# ( B )$ 

Exercise 3.6.8. Let A and B be sets such that there exists an injection $f$ : $A  B$ from A to B (i.e., A has lesser or equal cardinality to B). Show that there then exists a surjection $g : B  A$ from B to A. (The converse to this statement requires the axiom of choice; see Exercise 8.4.3.) 

Exercise 3.6.9. Let A and B be finite sets. Show that A B and $A \cap B$ are also finite sets, and that $\# ( A ) + \# ( B ) = \# ( A \cup B ) + \# ( A \cap B )$ 

Exercise 3.6.10. Let $A _ { 1 } , \ldots , A _ { n }$ be finite sets such that # $\textstyle ( \bigcup _ { i \in \{ 1 , . . . , n \} } A _ { i } ) > n$ Show that there exists $i \in \{ 1 , \ldots , n \}$ such that $\# ( A _ { i } ) \geq 2$ . (This is known as the pigeonhole principle.) 

## Chapter 4

## Integers and rationals

## 4.1 The integers

In Chapter 2 we built up most of the basic properties of the natural number system, but we have reached the limits of what one can do with just addition and multiplication. We would now like to introduce a new operation, that of subtraction, but to do that properly we will have to pass from the natural number system to a larger number system, that of the integers. 

Informally, the integers are what you can get by subtracting two natural numbers; for instance, $3 - 5$ should be an integer, as should $6 - 2$ . This is not a complete definition of the integers, because (a) it doesn’t say when two diferences are equal (for instance we should know why $3 - 5$ is equal to $2 - 4$ , but is not equal to $1 - 6 )$ , and (b) it doesn’t say how to do arithmetic on these diferences (how does one add $3 - 5$ to 6 2?). Furthermore, (c) this definition is circular because it requires a notion of subtraction, which we can only adequately define once the integers are constructed. Fortunately, because of our prior experience with integers we know what the answers to these questions should be. To answer (a), we know from our advanced knowledge in algebra that $a - b = c - d$ happens exactly when $a + d = c + b $ , so we can characterize equality of diferences using only the concept of addition. Similarly, to answer (b) we know from algebra that $( a - b ) + ( c - d ) = ( a + c ) - ( b + d )$ and that $( a - b ) ( c - d ) = ( a c + b d ) - ( a d + b c )$ . So we will take advantage of our foreknowledge by building all this into the definition of the integers, as we shall do shortly. 

We still have to resolve (c). To get around this problem we will use the following work-around: we will temporarily write integers not as a diference $a - b .$ but instead use a new notation $a { - } b$ to define integers, where the is a meaningless place-holder, similar to the comma in the Cartesian co-ordinate notation $( x , y )$ for points in the plane. Later when we define subtraction we will see that $a { - } b$ is in fact equal to $a - b ,$ , and so we can discard the notation ; it is only needed right now to avoid circularity. (These devices are similar to the scafolding used to construct a building; they are temporarily essential to make sure the building is built correctly, but once the building is completed they are thrown away and never used again.) This may seem unnecessarily complicated in order to define something that we already are very familiar with, but we will use this device again to construct the rationals, and knowing these kinds of constructions will be very helpful in later chapters. 

Definition 4.1.1 (Integers). An integer is an expression<sup>1</sup> of the form $a { - } b$ , where a and b are natural numbers. Two integers are considered to be equal, $a - b = c - d .$ , if and only if $a + d = c + b$ . We let Z denote the set of all integers. 

Thus for instance 3 5 is an integer, and is equal to 2 4, because $3 + 4 = 2 + 5$ . On the other hand, 3 5 is not equal to 2 3 because $3 + 3 \neq 2 + 5$ . This notation is strange looking, and has a few deficiencies; for instance, 3 is not yet an integer, because it is not of the form $a { \mathrm { - } } b !$ We will rectify these problems later. 

We have to check that this is a legitimate notion of equality. We need to verify the reflexivity, symmetry, transitivity, and substitution axioms (see Section A.7). We leave reflexivity and symmetry to Exercise 4.1.1 and instead verify the transitivity axiom. Suppose we know that $\quad { a { \mathrm { - } } { b } } = { c { \mathrm { - } } { } }$ d and $c - d = e - f$ . Then we have $a + d = c + b$ and $c + f = d + e .$ Adding the two equations together we obtain $a + d + c + f =$ $c + b + d + e$ . By Proposition 2.2.6 we can cancel the c and d, obtaining $a + f = b + e , { \mathrm { ~ i . e . , ~ } } a { \longrightarrow } b = e { \longrightarrow } f$ . Thus the cancellation law was needed to make sure that our notion of equality is sound. As for the substitution axiom, we cannot verify it at this stage because we have not yet defined any operations on the integers. However, when we do define our basic operations on the integers, such as addition, multiplication, and order, we will have to verify the substitution axiom at that time in order to ensure that the definition is valid. (We will only need to do this for the basic operations; more advanced operations on the integers, such as exponentiation, will be defined in terms of the basic ones, and so we do not need to re-verify the substitution axiom for the advanced operations.) 

Now we define two basic arithmetic operations on integers: addition and multiplication. 

Definition 4.1.2. The sum of two integers, $( a { - } { - } b ) + ( c { - } d )$ , is defined by the formula 

$$
(a - b) + (c - d) := (a + c) - (b + d).
$$

The product of two integers, $( a - - b ) \times ( c - d )$ , is defined by 

$$
(a - b) \times (c - d) := (a c + b d) - (a d + b c).
$$

Thus for instance, $( 3 - 5 ) + ( 1 { - } 4 )$ is equal to $( 4 - 9 )$ . There is however one thing we have to check before we can accept these definitions - we have to check that if we replace one of the integers by an equal integer, that the sum or product does not change. For instance, $( 3 \mathrm { - } 5 )$ is equal to $( 2 { - } 4 ) , \mathrm { s o } ( 3 { - } 5 ) + ( 1 { - } 4 )$ ought to have the same value as $( 2 - 4 ) + ( 1 { - } - 4 )$ , otherwise this would not give a consistent definition of addition. Fortunately, this is the case: 

Lemma 4.1.3 (Addition and multiplication are well-defined). Let $a , b , a ^ { \prime } , b ^ { \prime } , c ,$ d be natural numbers. $I f \left( a { - } { - } b \right) = \left( a ^ { \prime } { - } b ^ { \prime } \right)$ , then $( a - b ) +$ $( c { \mathrm { - } } d ) = ( a ^ { \prime } { \mathrm { - } } b ^ { \prime } ) + ( c { \mathrm { - } } d )$ and $( a { \mathrm { -- } } b ) \times ( c { \mathrm { -- } } d ) = ( a ^ { \prime } { \mathrm { -- } } b ^ { \prime } ) \times ( c { \mathrm { -- } } d )$ and also $( c \mathrm { ~ - ~ } d ) + ( a \mathrm { ~ - ~ } b ) = ( c \mathrm { ~ - ~ } d ) + ( a ^ { \prime } \mathrm { ~ - ~ } b ^ { \prime } )$ and $\quad ( c - d ) \times ( a - b ) =$ $( c - d ) \times ( a ^ { \prime } - b ^ { \prime } )$ . Thus addition and multiplication are well-defined operations (equal inputs give equal outputs). 

Proof. To prove that $( a { \mathrm { -- } } b ) + ( c { \mathrm { -- } } d ) = ( a ^ { \prime } { \mathrm { -- } } b ^ { \prime } ) + ( c { \mathrm { -- } } d )$ , we evaluate both sides as $( a + c ) { \longrightarrow } ( b + d )$ and $( a ^ { \prime } + c ) { \textstyle \longrightarrow } ( b ^ { \prime } + d )$ . Thus we need to show that $a + c + b ^ { \prime } + d = a ^ { \prime } + c + b + d .$ . But since $\left( a - b \right) = \left( a ^ { \prime } - b ^ { \prime } \right)$ , we have $a + b ^ { \prime } = a ^ { \prime } + b$ , and so by adding c + d to both sides we obtain the claim. Now we show that $( a { \mathrm { -- } } b ) \times ( c { \mathrm { -- } } d ) = ( a ^ { \prime } { \mathrm { -- } } b ^ { \prime } ) \times ( c { \mathrm { -- } } d )$ . Both sides evaluate to $( a c + b d ) { \longrightarrow } ( a d + b c )$ and $( a ^ { \prime } c + b ^ { \prime } d ) { \mathrm { - } } ( a ^ { \prime } d + b ^ { \prime } c )$ , so we have to show that $a c + b d + a ^ { \prime } d + b ^ { \prime } c = a ^ { \prime } c + b ^ { \prime } d + a d + b c$ . But the left-hand side factors as $c ( a + b ^ { \prime } ) + d ( a ^ { \prime } + b )$ , while the right factors as $c ( a ^ { \prime } + b ) + d ( a + b ^ { \prime } )$ . Since $a + b ^ { \prime } = a ^ { \prime } + b$ , the two sides are equal. The other two identities are proven similarly. □ 

The integers $n { - } 0$ behave in the same way as the natural numbers n; indeed one can check that $( n { \longrightarrow } 0 ) + ( m { \longrightarrow } 0 ) = ( n + m ) { \longrightarrow } 0$ and $( n - \ l - 0 ) \times ( m - \ l - 0 ) = n m - \ l - 0$ . Furthermore, $( n { - } 0 )$ is equal to $( m { - } 0 )$ if and only if $n = m$ . (The mathematical term for this is that there is an isomorphism between the natural numbers n and those integers of the form $n { \mathrm { - } } 0 . )$ Thus we may identify the natural numbers with integers by setting $n \equiv n - 0$ ; this does not afect our definitions of addition or multiplication or equality since they are consistent with each other. For instance the natural number 3 is now considered to be the same as the integer $3 - 0$ , thus $3 = 3 \mathrm { - } 0$ . In particular 0 is equal to $0 { - } 0$ and 1 is equal to $1 - 0$ . Of course, if we set n equal to $n { - } 0$ , then it will also be equal to any other integer which is equal to $n { - } 0$ , for instance 3 is equal not only to $3 - 0$ , but also to $4 - 1 , 5 - 2$ , etc. 

We can now define incrementation on the integers by defining $x { \ + } + : =$ $x + 1$ for any integer $x ;$ this is of course consistent with our definition of the increment operation for natural numbers. However, this is no longer an important operation for us, as it has been now superceded by the more general notion of addition. 

Now we consider some other basic operations on the integers. 

Definition 4.1.4 (Negation of integers). If $\left( a { - } b \right)$ is an integer, we define the negation $- ( a { - } b )$ to be the integer $( b { \mathrm { - } } a )$ . In particular if $n = n { - } 0$ is a positive natural number, we can define its negation $- n = 0 { \overline { { - } } } n$ 

For instance $- ( 3 - 5 ) = ( 5 - 3 )$ . One can check this definition is well-defined (Exercise 4.1.2). 

We can now show that the integers correspond exactly to what we expect. 

Lemma 4.1.5 (Trichotomy of integers). Let x be an integer. Then exactly one of the following three statements is true: (a) x is zero; (b) x is equal to a positive natural number n; or (c) x is the negation $- n$ of a positive natural number n. 

Proof. We first show that at least one of $( \mathrm { a } ) , ( \mathrm { b } ) , ( \mathrm { c } )$ is true. By definition, $x = a - b$ for some natural numbers a, b. We have three cases: $a > b , a = b $ , or $a < b$ . If $a > b$ then $a = b + c$ for some positive natural number $c ,$ which means that $a { \mathrm { - } } - b = c { \mathrm { - } } 0 = c ,$ , which is (b). If $a = b$ then $a { \mathrm { - } } b = a { \mathrm { - } } a = 0 { \mathrm { - } } 0 = 0$ , which is (a). If $a < b ,$ , then $b > a ,$ , so that $b { \underline { { - a } } } = n$ for some natural number n by the previous reasoning, and thus $\displaystyle a - b = - n ,$ , which is (c). 

Now we show that no more than one of $\mathrm { ( a ) , ( b ) , ( c ) }$ can hold at a time. By definition, a positive natural number is non-zero, so (a) and (b) cannot simultaneously be true. If (a) and (c) were simultaneously true, then $0 = - n$ for some positive natural $n ;$ thus $( 0 { \ - } - 0 ) = ( 0 { \ - } - n )$ so that $0 + n = 0 + 0$ , so that $n = 0$ , a contradiction. If (b) and (c) were simultaneously true, then $n = - m$ for some positive $n , m ,$ , so that $( n { \mathrm { - } } \quad 0 ) = ( 0 { \mathrm { - } } m )$ , so that $n + m = 0 + 0$ , which contradicts Proposition 2.2.8. Thus exactly one of (a), (b), (c) is true for any integer x. □ 

If n is a positive natural number, we call n a negative integer. Thus every integer is positive, zero, or negative, but not more than one of these at a time. 

One could well ask why we don’t use Lemma 4.1.5 to define the integers; i.e., why didn’t we just say an integer is anything which is either a positive natural number, zero, or the negative of a natural number. The reason is that if we did so, the rules for adding and multiplying integers would split into many diferent cases (e.g., negative times positive equals positive; negative plus positive is either negative, positive, or zero, depending on which term is larger, etc.) and to verify all the properties would end up being much messier. 

We now summarize the algebraic properties of the integers. 

Proposition 4.1.6 (Laws of algebra for integers). Let x, y, z be integers. Then we have 

$$
\begin{array}{c} x + y = y + x \\ (x + y) + z = x + (y + z) \\ x + 0 = 0 + x = x \\ x + (- x) = (- x) + x = 0 \\ x y = y x \\ (x y) z = x (y z) \\ x 1 = 1 x = x \\ x (y + z) = x y + x z \\ (y + z) x = y x + z x. \end{array}
$$

Remark 4.1.7. The above set of nine identities have a name; they are asserting that the integers form a commutative ring. (If one deleted the identity $x y = y x$ , then they would only assert that the integers form a $r i n g )$ . Note that some of these identities were already proven for the natural numbers, but this does not automatically mean that they also hold for the integers because the integers are a larger set than the natural numbers. On the other hand, this proposition supercedes many of the propositions derived earlier for natural numbers. 

Proof. There are two ways to prove these identities. One is to use Lemma 4.1.5 and split into a lot of cases depending on whether $x , y , z$ are zero, positive, or negative. This becomes very messy. A shorter way is to write $x = ( a { \longrightarrow } b ) , \ y = ( c { \longrightarrow } d )$ , and $z = ( e - f )$ for some natural numbers $a , b , c , d , e , f $ , and expand these identities in terms of $a , b , c , d , e , f$ and use the algebra of the natural numbers. This allows each identity to be proven in a few lines. We shall just prove the longest one, namely $( x y ) z = x ( y z )$ 

$$
\begin{array}{r l} (x y) z & = ((a - b) (c - d)) (e - f) \\ & = ((a c + b d) - (a d + b c)) (e - f) \\ & = ((a c e + b d e + a d f + b c f) - (a c f + b d f + a d e + b c e)); \\ x (y z) & = (a - b) ((c - d) (e - f)) \\ & = (a - b) ((c e + d f) - (c f + d e)) \\ & = ((a c e + a d f + b c f + b d e) - (a c f + a d e + b c e + b d f)) \end{array}
$$

and so one can see that $( x y ) z { \mathrm { ~ a n d ~ } } x ( y z )$ are equal. The other identities are proven in a similar fashion; see Exercise 4.1.4. □ 

We now define the operation of subtraction $x - y$ of two integers by the formula 

$$
x - y := x + (- y).
$$

We do not need to verify the substitution axiom for this operation, since we have defined subtraction in terms of two other operations on integers, namely addition and negation, and we have already verified that those operations are well-defined. 

One can easily check now that if a and b are natural numbers, then 

$$
a - b = a + - b = (a - 0) + (0 - b) = a - b,
$$

and so $a { \mathrm { - } } b$ is just the same thing as $a - b$ . Because of this we can now discard the notation, and use the familiar operation of subtraction instead. (As remarked before, we could not use subtraction immediately because it would be circular.) 

We can now generalize Lemma 2.3.3 and Corollary 2.3.7 from the natural numbers to the integers: 

Proposition 4.1.8 (Integers have no zero divisors). Let a and b be integers such that $a b = 0$ . Then either $a = 0 ~ o r ~ b = 0 ~ ( o r ~ b o t h )$ 

Proof. See Exercise 4.1.5. 

Corollary 4.1.9 (Cancellation law for integers). If a, b, c are integers such that $a c = b c$ and c is non-zero, then $a = b$ 

Proof. See Exercise 4.1.6. 

We now extend the notion of order, which was defined on the natural numbers, to the integers by repeating the definition verbatim: 

Definition 4.1.10 (Ordering of the integers). Let n and m be integers. We say that n is greater than or equal to m, and write $n \geq m$ or $m \leq n ,$ if we have $n = m + a$ for some natural number a. We say that n is strictly greater than m, and write $n > m$ or $m \ < \ n .$ , if $n \geq m$ and $n \neq m$ 

Thus for instance $5 > - 3$ , because $5 = - 3 + 8$ and $5 \neq - 3$ . Clearly this definition is consistent with the notion of order on the natural numbers, since we are using the same definition. 

Using the laws of algebra in Proposition 4.1.6 it is not hard to show the following properties of order: 

Lemma 4.1.11 (Properties of order). Let $a , b , c$ be integers. 

(a) $a > b$ if and only if $a - b$ is a positive natural number. 

(b) (Addition preserves order) If $a > b$ , then $a + c > b + c$ 

(c) (Positive multiplication preserves order) If $a > b$ and c is positive, then $a c > b c$ 

(d) (Negation reverses order) If $a > b$ , then $- a < - b$ 

(e) (Order is transitive) If $a > b$ and $b > c _ { i }$ , then $a > c$ 

## 4.2. The rationals

(f) (Order trichotomy) Exactly one of the statements $a > b , a < b ,$ , or $a = b$ is true. 

Proof. See Exercise 4.1.7. 

— Exercises — 

Exercise 4.1.1. Verify that the definition of equality on the integers is both reflexive and symmetric. 

Exercise 4.1.2. Show that the definition of negation on the integers is welldefined in the sense that if $\left( a - b \right) = \left( a ^ { \prime } - b ^ { \prime } \right)$ , then $- ( a { \longrightarrow } b ) = - ( a ^ { \prime } { \longrightarrow } b ^ { \prime } )$ (so equal integers have equal negations). 

Exercise 4.1.3. Show that $( - 1 ) \times a = - a$ for every integer a. 

Exercise 4.1.4. Prove the remaining identities in Proposition 4.1.6. (Hint: one can save some work by using some identities to prove others. For instance, once you know that $x y = y x$ , you get for free that $x 1 = 1 x$ , and once you also prove $x ( y + z ) = x y + x z$ , you automatically get $( y + z ) x = y x + z x { \mathrm { ~ f o r ~ f r e e . } } )$ 

Exercise 4.1.5. Prove Proposition 4.1.8. (Hint: while this proposition is not quite the same as Lemma 2.3.3, it is certainly legitimate to use Lemma 2.3.3 in the course of proving Proposition 4.1.8.) 

Exercise 4.1.6. Prove Corollary 4.1.9. (Hint: there are two ways to do this. One is to use Proposition 4.1.8 to conclude that $a - b$ must be zero. Another way is to combine Corollary 2.3.7 with Lemma 4.1.5.) 

Exercise 4.1.7. Prove Lemma 4.1.11. (Hint: use the first part of this lemma to prove all the others.) 

Exercise 4.1.8. Show that the principle of induction (Axiom 2.5) does not apply directly to the integers. More precisely, give an example of a property $P ( n )$ pertaining to an integer n such that $P ( 0 )$ is true, and that $P ( n )$ implies $P ( n { + } { + } )$ for all integers n, but that $P ( n )$ is not true for all integers n. Thus induction is not as useful a tool for dealing with the integers as it is with the natural numbers. (The situation becomes even worse with the rational and rea numbers, which we shall define shortly.) 

## 4.2 The rationals

We have now constructed the integers, with the operations of addition, subtraction, multiplication, and order and verified all the expected algebraic and order-theoretic properties. Now we will use a similar construction to build the rationals, adding division to our mix of operations. 

Just like the integers were constructed by subtracting two natural numbers, the rationals can be constructed by dividing two integers, though of course we have to make the usual caveat that the denominator should be non-zero<sup>2</sup>. Of course, just as two diferences $a - b$ and $c - d$ can be equal if $a + d = c + b$ , we know (from more advanced knowledge) that two quotients $a / b$ and $c / d$ can be equal if $a d = b c$ . Thus, in analogy with the integers, we create a new meaningless symbol $/ /$ (which will eventually be superceded by division), and define 

Definition 4.2.1. A rational number is an expression of the form $a / / b .$ where a and b are integers and b is non-zero; $a / / 0$ is not considered to be a rational number. Two rational numbers are considered to be equal, $a / / b = c / / d$ , if and only if $a d = c b$ . The set of all rational numbers is denoted Q. 

Thus for instance $3 / / 4 = 6 / / 8 = - 3 / / - 4$ , but $3 / / 4 \neq 4 / / 3$ . This is a valid definition of equality (Exercise 4.2.1). Now we need a notion of addition, multiplication, and negation. Again, we will take advantage of our pre-existing knowledge, which tells us that $a / b + c / d$ should equal $( a d + b c ) / ( b d )$ and that $a / b { * c } / d$ should equal $a c / b d .$ , while $- ( a / b )$ equals $( - a ) / b .$ . Motivated by this foreknowledge, we define 

Definition 4.2.2. If $a / / b$ and $c / d$ are rational numbers, we define their sum 

$$
(a / / b) + (c / / d) := (a d + b c) / / (b d)
$$

their product 

$$
(a / / b) * (c / / d) := (a c) / / (b d)
$$

and the negation 

$$
- (a / / b) := (- a) / / b.
$$

Note that if b and d are non-zero, then bd is also non-zero, by Proposition 4.1.8, so the sum or product of two rational numbers remains a rational number. 

Lemma 4.2.3. The sum, product, and negation operations on rational numbers are well-defined, in the sense that if one replaces $a / / b$ with another rational number $a ^ { \prime } / / b ^ { \prime }$ which is equal to $a / / b$ , then the output of the above operations remains unchanged, and similarly for $c / d$ 

Proof. We just verify this for addition; we leave the remaining claims to Exercise 4.2.2. Suppose $a / / b = a ^ { \prime } / / b ^ { \prime }$ , so that b and $b ^ { \prime }$ are non-zero and $a b ^ { \prime } = a ^ { \prime } b$ . We now show that $a / / b + c / / d = a ^ { \prime } / / b ^ { \prime } + c / / d .$ . By definition, the left-hand side is $( a d + b c ) / / b d$ and the right-hand side is $( a ^ { \prime } d + b ^ { \prime } c ) / / b ^ { \prime } d .$ , so we have to show that 

$$
(a d + b c) b ^ {\prime} d = (a ^ {\prime} d + b ^ {\prime} c) b d,
$$

which expands to 

$$
a b ^ {\prime} d ^ {2} + b b ^ {\prime} c d = a ^ {\prime} b d ^ {2} + b b ^ {\prime} c d.
$$

But since $a b ^ { \prime } = a ^ { \prime } b$ , the claim follows. Similarly if one replaces $c / d$ by $c ^ { \prime } / / d ^ { \prime }$ □ 

We note that the rational numbers $a / / 1$ behave in a manner identical to the integers a: 

$$
\begin{array}{c} (a / / 1) + (b / / 1) = (a + b) / / 1; \\ (a / / 1) \times (b / / 1) = (a b / / 1); \\ - (a / / 1) = (- a) / / 1. \end{array}
$$

Also, $a / / 1$ and $b / / 1$ are only equal when a and b are equal. Because of this, we will identify a with $a / / 1$ for each integer a: $a \equiv a / / 1$ ; the above identities then guarantee that the arithmetic of the integers is consistent with the arithmetic of the rationals. Thus just as we embedded the natural numbers inside the integers, we embed the integers inside the rational numbers. In particular, all natural numbers are rational numbers, for instance 0 is equal to $0 / / 1$ and 1 is equal to $1 / / 1$ 

Observe that a rational number $a / / b$ is equal to $0 = 0 / / 1$ if and only if $a \times 1 = b \times 0$ , i.e., if the numerator a is equal to 0. Thus if a and b are non-zero then so is $a / / b$ 

We now define a new operation on the rationals: reciprocal. If $x =$ $a / / b$ is a non-zero rational (so that $a , b \neq 0 )$ then we define the reciprocal $x ^ { - 1 }$ of $x$ to be the rational number $x ^ { - 1 } : = b / / a$ . It is easy to check that this operation is consistent with our notion of equality: if two rational numbers $a / / b , \ a ^ { \prime } / / b ^ { \prime }$ are equal, then their reciprocals are also equal. (In contrast, an operation such as “numerator” is not well-defined: the rationals $3 / / 4$ and $6 / / 8$ are equal, but have unequal numerators, so we have to be careful when referring to such terms as “the numerator of $x ^ { \prime \prime } . \big )$ ) We however leave the reciprocal of 0 undefined. 

We now summarize the algebraic properties of the rationals. 

Proposition 4.2.4 (Laws of algebra for rationals). Let $x , y , z$ be rationals. Then the following laws of algebra hold: 

$$
\begin{array}{c} {x + y = y + x} \\ {(x + y) + z = x + (y + z)} \\ {x + 0 = 0 + x = x} \\ {x + (- x) = (- x) + x = 0} \\ {x y = y x} \\ {(x y) z = x (y z)} \\ {x 1 = 1 x = x} \\ {x (y + z) = x y + x z} \\ {(y + z) x = y x + z x.} \end{array}
$$

If x is non-zero, we also have 

$$
x x ^ {- 1} = x ^ {- 1} x = 1.
$$

Remark 4.2.5. The above set of ten identities have a name; they are asserting that the rationals Q form a field. This is better than being a commutative ring because of the tenth identity $x x ^ { - 1 } = x ^ { - 1 } x = 1$ . Note that this proposition supercedes Proposition 4.1.6. 

Proof. To prove this identity, one writes $x = a / / b , y = c / / d , z = e / / f$ for some integers $a , c , e$ and non-zero integers $b , d , f .$ , and verifies each identity in turn using the algebra of the integers. We shall just prove the longest one, namely $( x + y ) + z = x + ( y + z )$ 

$$
\begin{array}{r l} (x + y) + z & = ((a / / b) + (c / / d)) + (e / / f) \\ & = ((a d + b c) / / b d) + (e / / f) \\ & = (a d f + b c f + b d e) / / b d f; \\ x + (y + z) & = (a / / b) + ((c / / d) + (e / / f)) \\ & = (a / / b) + ((c f + d e) / / d f) \\ & = (a d f + b c f + b d e) / / b d f \end{array}
$$

and so one can see that $( x + y ) + z { \mathrm { ~ a n d ~ } } x + ( y + z )$ are equal. The other identities are proven in a similar fashion and are left to Exercise 4.2.3. □ 

We can now define the quotient $x / y$ of two rational numbers x and y, provided that y is non-zero, by the formula 

$$
x / y := x \times y ^ {- 1}.
$$

Thus, for instance 

$$
(3 / / 4) / (5 / / 6) = (3 / / 4) \times (6 / / 5) = (1 8 / / 2 0) = (9 / / 1 0).
$$

Using this formula, it is easy to see that $a / b = a / / b$ for every integer a and every non-zero integer b. Thus we can now discard the $/ /$ notation, and use the more customary $a / b$ instead of $a / / b$ 

In a similar spirit, we define subtraction on the rationals by the formula 

$$
x - y := x + (- y),
$$

just as we did with the integers. 

Proposition 4.2.4 allows us to use all the normal rules of algebra; we will now proceed to do so without further comment. 

In the previous section we organized the integers into positive, zero, and negative numbers. We now do the same for the rationals. 

Definition 4.2.6. A rational number x is said to be positive if we have $x = a / b$ for some positive integers a and b. It is said to be negative if we have $x = - y$ for some positive rational y $( { \mathrm { i . e . , ~ } } x = ( - a ) / b$ for some positive integers a and b). 

Thus for instance, every positive integer is a positive rational number, and every negative integer is a negative rational number, so our new definition is consistent with our old one. 

Lemma 4.2.7 (Trichotomy of rationals). Let x be a rational number. Then exactly one of the following three statements is true: (a) x is equal to $\theta . \quad ( b )$ x is a positive rational number. (c) x is a negative rational number. 

Proof. See Exercise 4.2.4. 

Definition 4.2.8 (Ordering of the rationals). Let x and y be rational numbers. We say that $x > y$ if $x - y$ is a positive rational number, and $x < y { \mathrm { ~ i f f ~ } } x - y$ is a negative rational number. We write $x \geq y$ if either $x > y { \mathrm { ~ o r ~ } } x = y$ , and similarly define $x \leq y$ 

Proposition 4.2.9 (Basic properties of order on the rationals). Let $x , y , z$ be rational numbers. Then the following properties hold. 

(a) (Order trichotomy) Exactly one of the three statements $x \ = \ y$ , $x < y$ , or $x > y$ is true. 

(b) (Order is anti-symmetric) One has $x < y$ if and only if $y > x$ 

(c) (Order is transitive) If $x < y$ and $y < z$ , then $x < z$ 

(d) (Addition preserves order) If $x < y$ , then $x + z < y + z .$ 

(e) (Positive multiplication preserves order) If $x < y$ and z is positive, then $x z < y z$ 

Proof. See Exercise 4.2.5. 

Remark 4.2.10. The above five properties in Proposition 4.2.9, combined with the field axioms in Proposition 4.2.4, have a name: they assert that the rationals Q form an ordered field. It is important to keep in mind that Proposition 4.2.9(e) only works when z is positive, see Exercise 4.2.6. 

## — Exercises —

Exercise 4.2.1. Show that the definition of equality for the rational numbers is reflexive, symmetric, and transitive. (Hint: for transitivity, use Corollary 4.1.9.) 

Exercise 4.2.2. Prove the remaining components of Lemma 4.2.3. 

Exercise 4.2.3. Prove the remaining components of Proposition 4.2.4. (Hint: as with Proposition 4.1.6, you can save some work by using some identities to prove others.) 

Exercise 4.2.4. Prove Lemma 4.2.7. (Note that, as in Proposition 2.2.13, you have to prove two diferent things: firstly, that at least one of (a), (b), (c) is true; and secondly, that at most one of (a), (b), (c) is true.) 

Exercise 4.2.5. Prove Proposition 4.2.9. 

Exercise 4.2.6. Show that if x, $y , z$ are rational numbers such that $x < y$ and z is negative, then $x z > y z$ 

## 4.3 Absolute value and exponentiation

We have already introduced the four basic arithmetic operations of addition, subtraction, multiplication, and division on the rationals. (Recall that subtraction and division came from the more primitive notions of negation and reciprocal by the formulae $x - y : = x + ( - y )$ and $x / y : = x \times y ^ { - 1 } . )$ We also have a notion of order <, and have organized the rationals into the positive rationals, the negative rationals, and zero. In short, we have shown that the rationals Q form an ordered field. 

One can now use these basic operations to construct more operations. There are many such operations we can construct, but we shall just introduce two particularly useful ones: absolute value and exponentiation. 

Definition 4.3.1 (Absolute value). If x is a rational number, the absolute value x of x is defined as follows. If x is positive, then $| x | : = x$ . If x is negative, then $| x | : = - x$ . If x is zero, then $| x | : = 0$ 

Definition 4.3.2 (Distance). Let x and y be rational numbers. The quantity $| x - y |$ is called the distance between x and y and is sometimes denoted $d ( x , y )$ , thus $d ( x , y ) : = | x - y |$ . For instance, $d ( 3 , 5 ) = 2$ 

Proposition 4.3.3 (Basic properties of absolute value and distance). Let $x , y , z$ be rational numbers. 

(a) (Non-degeneracy of absolute value) We have $| x | \geq 0$ . Also, $| x | = 0$ if and only if x is 0. 

(b) (Triangle inequality for absolute value) We have $| x + y | \leq | x | + | y |$ 

(c) We have the inequalities $- y \leq x \leq y$ if and only if $y \geq | x |$ . In particular, we have $- | x | \leq x \leq | x |$ 

(d) (Multiplicativity of absolute value) We have $| x y | \ = \ | x | \ | y |$ . In particular, $| - x | = | x |$ 

(e) (Non-degeneracy of distance) We have $d ( x , y ) \geq 0$ . Also, $d ( x , y ) =$ 0 if and only if $x = y$ 

(f) (Symmetry of distance) $d ( x , y ) = d ( y , x )$ 

(g) (Triangle inequality for distance) $d ( x , z ) \leq d ( x , y ) + d ( y , z )$ 

Proof. See Exercise 4.3.1. 

Absolute value is useful for measuring how “close” two numbers are. Let us make a somewhat artificial definition: 

Definition 4.3.4 (ε-closeness). Let $\varepsilon > 0$ be a rational number, and let $x , y$ be rational numbers. We say that y is ε-close to x if we have $d ( y , x ) \leq \varepsilon$ 

Remark 4.3.5. This definition is not standard in mathematics textbooks; we will use it as “scafolding” to construct the more important notions of limits (and of Cauchy sequences) later on, and once we have those more advanced notions we will discard the notion of ε-close. 

Examples 4.3.6. The numbers 0.99 and 1.01 are 0.1-close, but they are not 0.01 close, because $d ( 0 . 9 9 , 1 . 0 1 ) = \lvert 0 . 9 9 - 1 . 0 1 \rvert = 0 . 0 2$ is larger than 0.01. The numbers 2 and 2 are ε-close for every positive ε. 

We do not bother defining a notion of ε-close when ε is zero or negative, because if ε is zero then x and y are only ε-close when they are equal, and when ε is negative then x and y are never ε-close. (In any event it is a long-standing tradition in analysis that the Greek letters ε, δ should only denote small positive numbers.) 

Some basic properties of ε-closeness are the following. 

Proposition 4.3.7. Let $x , y , z .$ , w be rational numbers. 

(a) $I f x = y$ , then x is ε-close to y for every $\varepsilon > 0$ . Conversely, if x is ε-close to y for every $\varepsilon > 0$ , then we have $x = y$ 

(b) Let $\varepsilon > 0$ . If x is ε-close to y, then y is ε-close to x. 

(c) Let $\varepsilon , \delta > 0$ . If x is ε-close to y, and y is δ-close to z, then x and $z \ a r e \ ( \varepsilon + \delta )  – c l o s e .$ 

(d) Let $\varepsilon , \delta > 0$ . If x and y are ε-close, and z and w are δ-close, then x + z and y + w are (ε + δ)-close, and x z and $y - w$ are also $( \varepsilon + \delta ) { - c l o s e . }$ 

(e) Let $\varepsilon > 0$ . If x and y are ε-close, they are also ε-close for every $\varepsilon ^ { \prime } > \varepsilon .$ 

(f) Let $\varepsilon > 0$ . If y and z are both ε-close to x, and w is between y and $z \ ( i . e . , \ y \le w \le z \ o r \ z \le w \le y )$ , then w is also ε-close to x. 

(g) Let $\varepsilon > 0$ . If x and y are ε-close, and z is non-zero, then xz and $y z \ a r e \ \varepsilon | z | - c l o s e .$ 

(h) Let $\varepsilon , \delta > 0$ . If x and y are ε-close, and z and w are δ-close, then xz and yw are $( \varepsilon | z | + \delta | x | + \varepsilon \delta ) { \ - } { - } c l o s e .$ 

Proof. We only prove the most dificult one, (h); we leave $\mathrm { ( a ) \mathrm { - ( g ) } }$ to Exercise 4.3.2. Let $\varepsilon , \delta > 0$ , and suppose that x and y are ε-close. If we write $a : = y - x$ , then we have $y = x + a$ and that $| a | \leq \varepsilon$ . Similarly, if z and w are δ-close, and we define $b : = w - z$ , then $w = z + b$ and $| b | \leq \delta$ 

Since $y = x +$ a and $w = z + b$ , we have 

$$
y w = (x + a) (z + b) = x z + a z + x b + a b.
$$

Thus 

$$
| y w - x z | = | a z + b x + a b | \leq | a z | + | b x | + | a b | = | a | | z | + | b | | x | + | a | | b |.
$$

Since $| a | \leq \varepsilon$ and $| b | \leq \delta$ , we thus have 

$$
| y w - x z | \leq \varepsilon | z | + \delta | x | + \varepsilon \delta
$$

and thus that yw and xz are $( \varepsilon | z | + \delta | x | + \varepsilon \delta )  – \mathrm { c l o s e } .$ 

Remark 4.3.8. One should compare statements $\mathrm { ( a ) - ( c ) }$ of this proposition with the reflexive, symmetric, and transitive axioms of equality. It is often useful to think of the notion of “ε-close” as an approximate substitute for that of equality in analysis. 

Now we recursively define exponentiation for natural number exponents, extending the previous definition in Definition 2.3.11. 

Definition 4.3.9 (Exponentiation to a natural number). Let x be a rational number. To raise x to the power 0, we define $x ^ { 0 } : = 1$ ; in particular we define $0 ^ { 0 } : = 1$ . Now suppose inductively that $x ^ { n }$ has been defined for some natural number n, then we define $x ^ { n + 1 } : = x ^ { n } \times x$ 

Proposition 4.3.10 (Properties of exponentiation, I). Let $x , y$ be rational numbers, and let n, m be natural numbers. 

(a) We have $x ^ { n } x ^ { m } = x ^ { n + m } , ( x ^ { n } ) ^ { m } = x ^ { n m }$ , and $( x y ) ^ { n } = x ^ { n } y ^ { n }$ 

(b) Suppose $n > 0$ . Then we have $x ^ { n } = 0$ if and only if $x = 0$ 

(c) If $x \ge y \ge 0$ , then $x ^ { n } \geq y ^ { n } \geq 0$ . If $x > y \ge 0$ and $n > 0$ , then $x ^ { n } > y ^ { n } \geq 0$ 

(d) We have $| x ^ { n } | = | x | ^ { n }$ 

Proof. See Exercise 4.3.3. 

Now we define exponentiation for negative integer exponents. 

Definition 4.3.11 (Exponentiation to a negative number). Let x be a non-zero rational number. Then for any negative integer $- n ,$ , we define $x ^ { - n } : = 1 / x ^ { n }$ 

Thus for instance $x ^ { - 3 } = 1 / x ^ { 3 } = 1 / ( x \times x \times x )$ . We now have $x ^ { n }$ defined for any integer n, whether n is positive, negative, or zero. Exponentiation with integer exponents has the following properties (which supercede Proposition 4.3.10): 

Proposition 4.3.12 (Properties of exponentiation, II). Let x, y be nonzero rational numbers, and let n, m be integers. 

(a) We have $x ^ { n } x ^ { m } = x ^ { n + m }$ $( x ^ { n } ) ^ { m } = x ^ { n m }$ , and $( x y ) ^ { n } = x ^ { n } y ^ { n }$ 

(b) If $x \ge y > 0$ , then $x ^ { n } \geq y ^ { n } > 0$ if n is positive, and $0 < x ^ { n } \leq y ^ { n }$ if n is negative. 

(c) If $x , y > 0 , n \neq 0$ , and $x ^ { n } = y ^ { n }$ , then $x = y$ 

(d) We have $| x ^ { n } | = | x | ^ { n }$ 

Proof. See Exercise 4.3.4. 

## — Exercises —

Exercise 4.3.1. Prove Proposition 4.3.3. (Hint: while all of these claims can be proven by dividing into cases, such as when x is positive, negative, or zero, several parts of the proposition can be proven without such a tedious division into cases. For instance one can use earlier parts of the proposition to prove later ones.) 

Exercise 4.3.2. Prove the remaining claims in Proposition 4.3.7. 

Exercise 4.3.3. Prove Proposition 4.3.10. (Hint: use induction.) 

Exercise 4.3.4. Prove Proposition 4.3.12. (Hint: induction is not suitable here. Instead, use Proposition 4.3.10.) 

Exercise 4.3.5. Prove that $2 ^ { N } \geq N$ for all positive integers N. (Hint: use induction.) 

## 4.4 Gaps in the rational numbers

Imagine that we arrange the rationals on a line, arranging x to the right of y if $x > y$ . (This is a non-rigorous arrangement, since we have not yet defined the concept of a line, but this discussion is only intended to motivate the more rigorous propositions below.) Inside the rationals we have the integers, which are thus also arranged on the line. Now we work out how the rationals are arranged with respect to the integers. 

Proposition 4.4.1 (Interspersing of integers by rationals). Let x be a rational number. Then there exists an integer n such that $n \leq x < n + 1$ In fact, this integer is unique $( i . e . ,$ for each x there is only one n for which $n \leq x < n + 1 )$ . In particular, there exists a natural number N such that $N > x$ (i.e., there is no such thing as a rational number which is larger than all the natural numbers). 

Remark 4.4.2. The integer n for which $n \leq x < n + 1$ is sometimes referred to as the integer part of x and is sometimes denoted $n = \lfloor x \rfloor$ 

Proof. See Exercise 4.4.1. 

Also, between every two rational numbers there is at least one additional rational: 

Proposition 4.4.3 (Interspersing of rationals by rationals). If x and y are two rationals such that $x < y$ , then there exists a third rational z such that $x < z < y$ 

Proof. We set $z : = ( x + y ) / 2$ . Since $x < y$ , and $1 / 2 = 1 / / 2$ is positive, we have from Proposition 4.2.9 that $x / 2 < y / 2$ . If we add $y / 2$ to both sides using Proposition 4.2.9 we obtain $x / 2 + y / 2 < y / 2 + y / 2 , \mathrm { i . e . , } z < y$ If we instead add $x / 2$ to both sides we obtain $x / 2 + x / 2 < y / 2 + x / 2 .$ i.e., $x < z$ . Thus $x < z < y$ as desired. 

Despite the rationals having this denseness property, they are still incomplete; there are still an infinite number of “gaps” or “holes” between the rationals, although this denseness property does ensure that these holes are in some sense infinitely small. For instance, we will now show that the rational numbers do not contain any square root of two. 

Proposition 4.4.4. There does not exist any rational number x for which $x ^ { 2 } = 2$ 

Proof. We only give a sketch of a proof; the gaps will be filled in Exercise 4.4.3. Suppose for sake of contradiction that we had a rational number x for which $x ^ { 2 } = 2$ . Clearly x is not zero. We may assume that x is positive, for if x were negative then we could just replace x by x (since $x ^ { 2 } = ( - x ) ^ { 2 } )$ . Thus $x = p / q$ for some positive integers p, q, so $( p / q ) ^ { 2 } = 2$ which we can rearrange as $p ^ { 2 } = 2 q ^ { 2 }$ . Define a natural number p to be even if $p = 2 k$ for some natural number k, and odd if $p = 2 k + 1$ for some natural number k. Every natural number is either even or odd, but not both (why?). If p is odd, then $p ^ { 2 }$ is also odd (why?), which contradicts $p ^ { 2 } = 2 q ^ { 2 }$ . Thus p is even, i.e., $p = 2 k$ for some natural number k. Since $p$ is positive, k must also be positive. Inserting $p = 2 k$ into $p ^ { 2 } = 2 q ^ { 2 }$ we obtain $4 k ^ { 2 } = 2 q ^ { 2 }$ , so that $q ^ { 2 } = 2 k ^ { 2 }$ 

To summarize, we started with a pair $( p , q )$ of positive integers such that $p ^ { 2 } = 2 q ^ { 2 }$ , and ended up with a pair $( q , k )$ of positive integers such that $q ^ { 2 } = 2 k ^ { 2 }$ . Since $p ^ { 2 } = 2 q ^ { 2 }$ , we have $q < p \ \mathrm { ( w h y ? ) }$ . If we rewrite $p ^ { \prime } : = q$ and $q ^ { \prime } : = k$ , we thus can pass from one solution $( p , q )$ to the equation $p ^ { 2 } = 2 q ^ { 2 }$ to a new solution $( p ^ { \prime } , q ^ { \prime } )$ to the same equation which has a smaller value of $p .$ . But then we can repeat this procedure again and again, obtaining a sequence $( p ^ { \prime \prime } , q ^ { \prime \prime } ) , ( p ^ { \prime \prime \prime } , q ^ { \prime \prime \prime } )$ , etc. of solutions to $p ^ { 2 } = 2 q ^ { 2 }$ , each one with a smaller value of $p$ than the previous, and each one consisting of positive integers. But this contradicts the principle of infinite descent (see Exercise 4.4.2). This contradiction shows that we could not have had a rational x for which $x ^ { 2 } = 2$ □ 

On the other hand, we can get rational numbers which are arbitrarily close to a square root of 2: 

Proposition 4.4.5. For every rational number $\varepsilon > 0$ , there exists a non-negative rational number x such that $x ^ { 2 } < 2 < ( x + \varepsilon ) ^ { 2 }$ 

Proof. Let $\varepsilon > 0$ be rational. Suppose for sake of contradiction that there is no non-negative rational number x for which $x ^ { 2 } < 2 < ( x + \varepsilon ) ^ { 2 }$ This means that whenever x is non-negative and $x ^ { 2 } < 2$ , we must also have $( x + \varepsilon ) ^ { 2 } < 2$ (note that $( x + \varepsilon ) ^ { 2 }$ cannot equal 2, by Proposition $4 . 4 . 4 )$ . Since $0 ^ { 2 } < 2$ , we thus have $\varepsilon ^ { 2 } < 2$ , which then implies $( 2 \varepsilon ) ^ { 2 } < 2$ 2 and indeed a simple induction shows that $( n \varepsilon ) ^ { 2 } < 2$ for every natural number $n .$ . (Note that $n \varepsilon$ is non-negative for every natural number n - why?) But, by Proposition 4.4.1 we can find an integer n such that $n > 2 / \varepsilon$ , which implies that $n \varepsilon > 2$ , which implies that $( n \varepsilon ) ^ { 2 } > 4 > 2$ 4 contradicting the claim that $( n \varepsilon ) ^ { 2 } < 2$ for all natural numbers n. This contradiction gives the proof. □ 

Example 4.4.6. $\mathrm { I f } ^ { 3 } ~ \varepsilon = 0 . 0 0 1$ , we can take $x = 1 . 4 1 4$ , since $x ^ { 2 } =$ 1.999396 and $( x + \varepsilon ) ^ { 2 } = 2 . 0 0 2 2 2 5$ 

Proposition 4.4.5 indicates that, while the set Q of rationals does not actually have $\sqrt { 2 }$ as a member, we can get as close as we wish to ${ \sqrt { 2 } } .$ . For instance, the sequence of rationals 

1.4, 1.41, 1.414, 1.4142, 1.41421, . . . 

seem to get closer and closer to ${ \sqrt { 2 } } ,$ , as their squares indicate: 

1.96, 1.9881, 1.99396, 1.99996164, 1.9999899241, . . . 

Thus it seems that we can create a square root of 2 by taking a “limit” of a sequence of rationals. This is how we shall construct the real numbers in the next chapter. (There is another way to do so, using something called “Dedekind cuts”, which we will not pursue here. One can also proceed using infinite decimal expansions, but there are some sticky issues when doing so, e.g., one has to make 0.999 . . . equal to 1.000 . . ., and this approach, despite being the most familiar, is actually more complicated than other approaches; see the Appendix B.) 

— Exercises — 

Exercise 4.4.1. Prove Proposition 4.4.1. (Hint: use Proposition 2.3.9.) 

Exercise 4.4.2. A definition: a sequence $a _ { 0 } , a _ { 1 } , a _ { 2 } , \dotsc$ of numbers (natural numbers, integers, rationals, or reals) is said to be in infinite descent if we have $a _ { n } > a _ { n + 1 }$ for all natural numbers n $( { \mathrm { i . e . , ~ } } a _ { 0 } > a _ { 1 } > a _ { 2 } > \ldots { } )$ 

(a) Prove the principle of infinite descent: that it is not possible to have a sequence of natural numbers which is in infinite descent. (Hint: assume for sake of contradiction that you can find a sequence of natural numbers which is in infinite descent. Since all the $a _ { n }$ are natural numbers, you know that $a _ { n } \geq 0$ for all n. Now use induction to show in fact that $a _ { n } \geq k$ for all $k \in \mathbf N$ and all $n \in \mathbf N$ , and obtain a contradiction.) 

(b) Does the principle of infinite descent work if the sequence $a _ { 1 } , a _ { 2 } , a _ { 3 } , \ldots$ is allowed to take integer values instead of natural number values? What about if it is allowed to take positive rational values instead of natura numbers? Explain. 

Exercise 4.4.3. Fill in the gaps marked (why?) in the proof of Proposition 4.4.4. 

## Chapter 5

## The real numbers

To review our progress to date, we have rigorously constructed three fundamental number systems: the natural number system N, the integers Z, and the rationals Q<sup>1</sup>. We defined the natural numbers using the five Peano axioms, and postulated that such a number system existed; this is plausible, since the natural numbers correspond to the very intuitive and fundamental notion of sequential counting. Using that number system one could then recursively define addition and multiplication, and verify that they obeyed the usual laws of algebra. We then constructed the integers by taking formal<sup>2</sup> diferences of the natural numbers, a b. We then constructed the rationals by taking formal quotients of the integers, $a / / b ,$ , although we need to exclude division by zero in order to keep the laws of algebra reasonable. (You are of course free to design your own number system, possibly including one where division by zero is permitted; but you will have to give up one or more of the field axioms from Proposition 4.2.4, among other things, and you will probably get a less useful number system in which to do any real-world problems.) 

The rational system is already suficient to do a lot of mathematics - much of high school algebra, for instance, works just fine if one only knows about the rationals. However, there is a fundamental area of mathematics where the rational number system does not sufice - that of geometry (the study of lengths, areas, etc.). For instance, a right-angled triangle with both sides equal to 1 gives a hypotenuse of ${ \sqrt { 2 } } ,$ which is an irrational number, i.e., not a rational number; see Proposition 4.4.4. Things get even worse when one starts to deal with the sub-field of geometry known as trigonometry, when one sees numbers such as π or cos(1), which turn out to be in some sense “even more” irrational than $\sqrt { 2 }$ . (These numbers are known as transcendental numbers, but to discuss this further would be far beyond the scope of this text.) Thus, in order to have a number system which can adequately describe geometry - or even something as simple as measuring lengths on a line - one needs to replace the rational number system with the real number system. Since diferential and integral calculus is also intimately tied up with geometry - think of slopes of tangents, or areas under a curve - calculus also requires the real number system in order to function properly. 

However, a rigorous way to construct the reals from the rationals turns out to be somewhat dificult - requiring a bit more machinery than what was needed to pass from the naturals to the integers, or the integers to the rationals. In those two constructions, the task was to introduce one more algebraic operation to the number system - e.g., one can get integers from naturals by introducing subtraction, and get the rationals from the integers by introducing division. But to get the reals from the rationals is to pass from a “discrete” system to a “continuous” one, and requires the introduction of a somewhat diferent notion - that of a limit. The limit is a concept which on one level is quite intuitive, but to pin down rigorously turns out to be quite dificult. (Even such great mathematicians as Euler and Newton had dificulty with this concept. It was only in the nineteenth century that mathematicians such as Cauchy and Dedekind figured out how to deal with limits rigorously.) 

In Section 4.4 we explored the “gaps” in the rational numbers; now we shall fill in these gaps using limits to create the real numbers. The real number system will end up being a lot like the rational numbers, but will have some new operations - notably that of supremum, which can then be used to define limits and thence to everything else that calculus needs. 

The procedure we give here of obtaining the real numbers as the limit of sequences of rational numbers may seem rather complicated. However, it is in fact an instance of a very general and useful procedure, that of completing one metric space to form another; see Exercise 11.6.8. 

## 5.1 Cauchy sequences

Our construction of the real numbers shall rely on the concept of a Cauchy sequence. Before we define this notion formally, let us first define the concept of a sequence. 

Definition 5.1.1 (Sequences). Let m be an integer. A sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ of rational numbers is any function from the set $\{ n \in \mathbf { Z } : n \geq$ m to Q, i.e., a mapping which assigns to each integer n greater than or equal to m, a rational number $a _ { n }$ . More informally, a sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ of rational numbers is a collection of rationals $a _ { m } , a _ { m + 1 } , a _ { m + 2 } , . . . .$ 

Example 5.1.2. The sequence $( n ^ { 2 } ) _ { n = 0 } ^ { \infty }$ is the collection 0, 1, 4, 9, . . . of natural numbers; the sequence $( 3 ) _ { n = 0 } ^ { \infty }$ is the collection 3, 3, 3, . . . of natural numbers. These sequences are indexed starting from 0, but we can of course make sequences starting from 1 or any other number; for instance, the sequence $( a _ { n } ) _ { n = 3 } ^ { \infty }$ denotes the sequence $a _ { 3 } , a _ { 4 } , a _ { 5 } , . . . ,$ so $( n ^ { 2 } ) _ { n = 3 } ^ { \infty }$ is the collection 9, 16, 25, . . . of natural numbers. 

We want to define the real numbers as the limits of sequences of rational numbers. To do so, we have to distinguish which sequences of rationals are convergent and which ones are not. For instance, the sequence 

$$
\begin{array}{l} 1. 4, 1. 4 1, 1. 4 1 4, 1. 4 1 4 2, 1. 4 1 4 2 1, \dots \end{array}
$$

looks like it is trying to converge to something, as does 

$$
0. 1, 0. 0 1, 0. 0 0 1, 0. 0 0 0 1, \dots
$$

while other sequences such as 

$$
1, 2, 4, 8, 1 6, \ldots
$$

or 

$$
1, 0, 1, 0, 1, \ldots
$$

do not. To do this we use the definition of ε-closeness defined earlier. Recall from Definition 4.3.4 that two rational numbers x, y are ε-close if $d ( x , y ) = | x - y | \leq \varepsilon$ 

Definition 5.1.3 (ε-steadiness). Let $\varepsilon > 0$ . A sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ is said to be ε-steady if each pair $a _ { j } , ~ a _ { k }$ of sequence elements is ε-close for every natural number $j , k$ . In other words, the sequence $a _ { 0 } , a _ { 1 } , a _ { 2 } , . . .$ . is ε-steady if $d ( a _ { j } , a _ { k } ) \leq \varepsilon$ for all $j , k$ 

## 5.1. Cauchy sequences

Remark 5.1.4. This definition is not standard in the literature; we wil not need it outside of this section; similarly for the concept of “eventual ε-steadiness” below. We have defined ε-steadiness for sequences whose index starts at 0, but clearly we can make a similar notion for sequences whose indices start from any other number: a sequence $a _ { N } , a _ { N + 1 } , \dotsc$ is ε-steady if one has $d ( a _ { j } , a _ { k } ) \leq \varepsilon { \mathrm { ~ f o r } }$ all j, $k \geq N$ 

Example 5.1.5. The sequence 1, 0, 1, 0, 1, . . . is 1-steady, but is not $1 / 2 \AA$ steady. The sequence 0.1, 0.01, 0.001, 0.0001, . . . is 0.1-steady, but is not 0.01-steady (why?). The sequence 1, 2, 4, 8, 16, . . . is not ε-steady for any $\varepsilon \ \mathrm { ( w h y ? ) }$ . The sequence 2, 2, 2, 2, . . . is ε-steady for every $\varepsilon > 0$ 

The notion of ε-steadiness of a sequence is simple, but does not really capture the limiting behavior of a sequence, because it is too sensitive to the initial members of the sequence. For instance, the sequence 

$$
1 0, 0, 0, 0, 0, 0, \ldots
$$

is 10-steady, but is not ε-steady for any smaller value of $\varepsilon ,$ despite the sequence converging almost immediately to zero. So we need a more robust notion of steadiness that does not care about the initial members of a sequence. 

Definition 5.1.6 (Eventual ε-steadiness). Let $\varepsilon \quad > \quad 0 .$ A sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ is said to be eventually ε-steady if the sequence $a _ { N } , a _ { N + 1 } , a _ { N + 2 } , . . .$ is ε-steady for some natural number $N \geq 0$ . In other words, the sequence $a _ { 0 } , a _ { 1 } , a _ { 2 } , \dotsc$ . is eventually ε-steady if there exists an $N \geq 0$ such that $d ( a _ { j } , a _ { k } ) \leq \varepsilon$ for all $j , k \geq N$ 

Example 5.1.7. The sequence $a _ { 1 } , a _ { 2 } , \dotsc .$ . defined by $a _ { n } : = 1 / n , \mathrm { ( i . e . }$ the sequence $1 , 1 / 2 , 1 / 3 , 1 / 4 , \ldots )$ is not 0.1-steady, but is eventually 0.1- steady, because the sequence $a _ { 1 0 } , a _ { 1 1 } , a _ { 1 2 } , . . . \ ( \mathrm { i . e . , ~ } 1 / 1 0 , 1 / 1 1 , 1 / 1 2 , . . . )$ is 0.1-steady. The sequence $1 0 , 0 , 0 , 0 , 0 , . . .$ . is not ε-steady for any ε less than 10, but it is eventually ε-steady for every $\varepsilon > 0 \ \mathrm { ( w h y ? ) }$ 

Now we can finally define the correct notion of what it means for a sequence of rationals to “want” to converge. 

Definition 5.1.8 (Cauchy sequences). A sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ of rational numbers is said to be a Cauchy sequence if for every rational $\varepsilon > 0$ , the sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ is eventually ε-steady. In other words, the sequence $a _ { 0 } , a _ { 1 } , a _ { 2 } , \dotsc$ is a Cauchy sequence if for every $\varepsilon > 0$ , there exists an $N \geq 0$ such that $d ( a _ { j } , a _ { k } ) \leq \varepsilon$ for all $j , k \geq N$ 

Remark 5.1.9. At present, the parameter ε is restricted to be a positive rational; we cannot take ε to be an arbitrary positive real number, because the real numbers have not yet been constructed. However, once we do construct the real numbers, we shall see that the above definition will not change if we require ε to be real instead of rational (Proposition 6.1.4). In other words, we will eventually prove that a sequence is eventually ε-steady for every rational $\varepsilon > 0$ if and only if it is eventually ε-steady for every real $\varepsilon > 0$ ; see Proposition 6.1.4. This rather subtle distinction between a rational ε and a real ε turns out not to be very important in the long run, and the reader is advised not to pay too much attention as to what type of number $\varepsilon$ should be. 

Example 5.1.10. (Informal) Consider the sequence 

$$
1. 4, 1. 4 1, 1. 4 1 4, 1. 4 1 4 2, \dots
$$

mentioned earlier. This sequence is already 1-steady. If one discards the first element 1.4, then the remaining sequence 

$$
1. 4 1, 1. 4 1 4, 1. 4 1 4 2, \dots
$$

is now 0.1-steady, which means that the original sequence was eventually 0.1-steady. Discarding the next element gives the 0.01-steady sequence 1.414, 1.4142, . . .; thus the original sequence was eventually 0.01- steady. Continuing in this way it seems plausible that this sequence is in fact ε-steady for every $\varepsilon > 0$ , which seems to suggest that this is a Cauchy sequence. However, this discussion is not rigorous for several reasons, for instance we have not precisely defined what this sequence 1.4, 1.41, 1.414, . . . really is. An example of a rigorous treatment follows next. 

Proposition 5.1.11. The sequence $a _ { 1 } , a _ { 2 } , a _ { 3 } , . . .$ . defined by $a _ { n } : = 1 / n$ (i.e., the sequence $1 , 1 / 2 , 1 / 3 , \ldots )$ is a Cauchy sequence. 

Proof. We have to show that for every $\varepsilon > 0$ , the sequence $a _ { 1 } , a _ { 2 } , \dotsc$ . is eventually ε-steady. So let $\varepsilon > 0$ be arbitrary. We now have to find a number $N \geq 1$ such that the sequence $a _ { N } , a _ { N + 1 } , . . .$ . is ε-steady. Let us see what this means. This means that $d ( a _ { j } , a _ { k } ) \leq \varepsilon$ for every $j , k \geq N$ , i.e. 

$$
\left| 1 / j - 1 / k \right| \leq \varepsilon \text {   for   every   } j, k \geq N.
$$

Now since $j , k \geq N$ , we know that $0 < 1 / j , 1 / k \le 1 / N$ , so that $| 1 / j -$ $1 / k | \leq 1 / N$ . So in order to force $| 1 / j - 1 / k |$ to be less than or equal to ε, it would be suficient for $1 / N$ to be less than $\varepsilon .$ . So all we need to do is choose an N such that $1 / N$ is less than $\varepsilon ,$ , or in other words that N is greater than $1 / \varepsilon$ . But this can be done thanks to Proposition 4.4.1. 

As you can see, verifying from first principles (i.e., without using any of the machinery of limits, etc.) that a sequence is a Cauchy sequence requires some efort, even for a sequence as simple as $1 / n$ . The part about selecting an N can be particularly dificult for beginners - one has to think in reverse, working out what conditions on N would sufice to force the sequence $a _ { N } , a _ { N + 1 } , a _ { N + 2 } , . . .$ to be ε-steady, and then finding an N which obeys those conditions. Later we will develop some limit laws which allow us to determine when a sequence is Cauchy more easily. 

We now relate the notion of a Cauchy sequence to another basic notion, that of a bounded sequence. 

Definition 5.1.12 (Bounded sequences). Let $M \geq 0$ be rational. A finite sequence $a _ { 1 } , a _ { 2 } , \ldots , a _ { n }$ is bounded by M if $| a _ { i } | \leq M$ for all $1 \leq$ $i \leq n$ . An infinite sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is bounded by M if $| a _ { i } | \leq M$ for all $i \geq 1$ . A sequence is said to be bounded if it is bounded by M for some rational $M \geq 0$ 

Example 5.1.13. The finite sequence $1 , - 2 , 3 , - 4$ is bounded (in this case, it is bounded by 4, or indeed by any M greater than or equal to 4). But the infinite sequence $1 , - 2 , 3 , - 4 , 5 , - 6 , . .$ . is unbounded. (Can you prove this? Use Proposition 4.4.1.) The sequence $1 , - 1 , 1 , - 1 , . .$ . is bounded (e.g., by 1), but is not a Cauchy sequence. 

Lemma 5.1.14 (Finite sequences are bounded). Every finite sequence $a _ { 1 } , a _ { 2 } , \ldots , a _ { n }$ is bounded. 

Proof. We prove this by induction on n. When $n = 1$ the sequence $a _ { 1 }$ is clearly bounded, for if we choose $M : = | a _ { 1 } |$ then clearly we have $| a _ { i } | \leq M$ for all $1 \leq i \leq n$ . Now suppose that we have already proved the lemma for some $n \geq 1$ ; we now prove it for $n + 1 , \mathrm { i . e . }$ , we prove every sequence $a _ { 1 } , a _ { 2 } , \ldots , a _ { n + 1 }$ is bounded. By the induction hypothesis we know that $a _ { 1 } , a _ { 2 } , \ldots , a _ { n }$ is bounded by some $M \ \geq \ 0 ;$ ; in particular, it must be bounded by $\boldsymbol { M } + | a _ { n + 1 } |$ . On the other hand, $a _ { n + 1 }$ is also bounded by $\textstyle M + | a _ { n + 1 } |$ . Thus $a _ { 1 } , a _ { 2 } , \ldots , a _ { n } , a _ { n + 1 }$ is bounded by $\textstyle M + | a _ { n + 1 } |$ , and is hence bounded. This closes the induction. □ 

Note that while this argument shows that every finite sequence is bounded, no matter how long the finite sequence is, it does not say anything about whether an infinite sequence is bounded or not; infinity is not a natural number. However, we have 

Lemma 5.1.15 (Cauchy sequences are bounded). Every Cauchy sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is bounded. 

Proof. See Exercise 5.1.1. 

— Exercises — 

Exercise 5.1.1. Prove Lemma 5.1.15. (Hint: use the fact that $a _ { n }$ is eventually 1-steady, and thus can be split into a finite sequence and a 1-steady sequence. Then use Lemma 5.1.14 for the finite part. Note there is nothing special about the number 1 used here; any other positive number would have suficed.) 

## 5.2 Equivalent Cauchy sequences

Consider the two Cauchy sequences of rational numbers: 

1.4, 1.41, 1.414, 1.4142, 1.41421, . . . 

and 

$$
1. 5, 1. 4 2, 1. 4 1 5, 1. 4 1 4 3, 1. 4 1 4 2 2, \ldots
$$

Informally, both of these sequences seem to be converging to the same number, the square root ${ \sqrt { 2 } } = 1 . 4 1 4 2 1 \ldots$ . (though this statement is not yet rigorous because we have not defined real numbers yet). If we are to define the real numbers from the rationals as limits of Cauchy sequences, we have to know when two Cauchy sequences of rationals give the same limit, without first defining a real number (since that would be circular). To do this we use a similar set of definitions to those used to define a Cauchy sequence in the first place. 

Definition 5.2.1 (ε-close sequences). Let $( a _ { n } ) _ { n = 0 } ^ { \infty }$ and $( b _ { n } ) _ { n = 0 } ^ { \infty }$ be two sequences, and let $\varepsilon > 0$ . We say that the sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ is ε-close to $( b _ { n } ) _ { n = 0 } ^ { \infty }$ if $a _ { n }$ is ε-close to $b _ { n }$ for each $n \in \mathbf N$ . In other words, the sequence $a _ { 0 } , a _ { 1 } , a _ { 2 } , \dotsc$ is ε-close to the sequence $b _ { 0 } , b _ { 1 } , b _ { 2 } , \ldots \mathrm { i f f } \ | a _ { n } - b _ { n } | \leq \varepsilon$ for all n = 0, 1, 2, . . .. 

Example 5.2.2. The two sequences 

$$
1, - 1, 1, - 1, 1, \dots
$$

and 

$$
1. 1, - 1. 1, 1. 1, - 1. 1, 1. 1, \ldots
$$

are 0.1-close to each other. (Note however that neither of them are 0.1-steady). 

Definition 5.2.3 (Eventually ε-close sequences). Let $( a _ { n } ) _ { n = 0 } ^ { \infty }$ and $( b _ { n } ) _ { n = 0 } ^ { \infty }$ be two sequences, and let $\varepsilon > 0$ . We say that the sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ is eventually ε-close to $( b _ { n } ) _ { n = 0 } ^ { \infty }$ if there exists an $N \geq 0$ such that the sequences $( a _ { n } ) _ { n = N } ^ { \infty }$ and $( b _ { n } ) _ { n = N } ^ { \infty }$ are ε-close. In other words, $a _ { 0 } , a _ { 1 } , a _ { 2 } , \dotsc$ . is eventually ε-close to $b _ { 0 } , b _ { 1 } , b _ { 2 } , \dotsc$ . if there exists an $N \geq 0$ such that $| a _ { n } - b _ { n } | \leq \varepsilon$ for all $n \geq N$ 

Remark 5.2.4. Again, the notations for ε-close sequences and eventually ε-close sequences are not standard in the literature, and we will not use them outside of this section. 

## Example 5.2.5. The two sequences

$$
1. 1, 1. 0 1, 1. 0 0 1, 1. 0 0 0 1, \dots
$$

and 

$$
0. 9, 0. 9 9, 0. 9 9 9, 0. 9 9 9 9, \dots
$$

are not 0.1-close (because the first elements of both sequences are not 0.1-close to each other). However, the sequences are still eventually 0.1-close, because if we start from the second elements onwards in the sequence, these sequences are 0.1-close. A similar argument shows that the two sequences are eventually 0.01-close (by starting from the third element onwards), and so forth. 

Definition 5.2.6 (Equivalent sequences). Two sequences $( a _ { n } ) _ { n = 0 } ^ { \infty }$ and $( b _ { n } ) _ { n = 0 } ^ { \infty }$ are equivalent if for each rational $\varepsilon > 0$ , the sequences $( a _ { n } ) _ { n = 0 } ^ { \infty }$ and $( b _ { n } ) _ { n = 0 } ^ { \infty }$ are eventually ε-close. In other words, $a _ { 0 } , a _ { 1 } , a _ { 2 } , \dotsc$ . and $b _ { 0 } , b _ { 1 } , b _ { 2 } , \dotsc$ are equivalent if for every rational $\varepsilon > 0$ , there exists an $N \geq 0$ such that $| a _ { n } - b _ { n } | \leq \varepsilon$ for all $n \geq N$ 

Remark 5.2.7. As with Definition 5.1.8, the quantity $\varepsilon > 0$ is currently restricted to be a positive rational, rather than a positive real. However, we shall eventually see that it makes no diference whether ε ranges over the positive rationals or positive reals; see Exercise 6.1.10. 

From Definition 5.2.6 it seems that the two sequences given in Example 5.2.5 appear to be equivalent. We now prove this rigorously. 

Proposition 5.2.8. Let $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ be the sequences $a _ { n } =$ $1 + 1 0 ^ { - n }$ and $b _ { n } = 1 - 1 0 ^ { - n }$ . Then the sequences $a _ { n } , b _ { n }$ are equivalent. 

Remark 5.2.9. This Proposition, in decimal notation, asserts that $1 . 0 0 0 0 \ldots = 0 . 9 9 9 9 \ldots ; . . ;$ see Proposition B.2.3. 

Proof. We need to prove that for every $\varepsilon > 0$ , the two sequences $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ are eventually ε-close to each other. So we fix an $\varepsilon > 0$ We need to find an $N > 0$ such that $( a _ { n } ) _ { n = N } ^ { \infty }$ and $\left( b _ { n } \right) _ { n = N } ^ { \infty }$ are $\varepsilon { \mathrm { - c l o s e } }$ in other words, we need to find an $N > 0$ such that 

$$
\left| a _ {n} - b _ {n} \right| \leq \varepsilon \text {   for   all   } n \geq N.
$$

However, we have 

$$
\left| a _ {n} - b _ {n} \right| = \left| (1 + 1 0 ^ {- n}) - (1 - 1 0 ^ {- n}) \right| = 2 \times 1 0 ^ {- n}.
$$

Since $1 0 ^ { - n }$ is a decreasing function of $n \ ( { \mathrm { i . e . , ~ } } 1 0 ^ { - m } < 1 0 ^ { - n }$ whenever $m > n ;$ this is easily proven by induction), and $n \geq N$ , we have $2 ~ \times$ $1 0 ^ { - n } \leq 2 \times 1 0 ^ { - N }$ . Thus we have 

$$
\left| a _ {n} - b _ {n} \right| \leq 2 \times 1 0 ^ {- N} \text {   for   all   } n \geq N.
$$

Thus in order to obtain $| a _ { n } - b _ { n } | \leq \varepsilon$ for all $n \geq N$ , it will be suficient to choose N so that $2 \times 1 0 ^ { - N } \leq \varepsilon$ . This is easy to do using logarithms, but we have not yet developed logarithms yet, so we will use a cruder method. First, we observe $1 0 ^ { N }$ is always greater than N for any $N \geq 1$ (see Exercise 4.3.5). Thus $1 0 ^ { - N } \le 1 / N$ , and so $2 \times 1 0 ^ { - N } \leq 2 / N$ . Thus to get $2 \times 1 0 ^ { - N } \leq \varepsilon$ , it will sufice to choose N so that $2 / N \le \varepsilon$ , or equivalently that $N \geq 2 / \varepsilon$ . But by Proposition 4.4.1 we can always choose such an N, and the claim follows. □ 

$$
- \text { Exercises } -
$$

Exercise 5.2.1. Show that if $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ are equivalent sequences of rationals, then $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is a Cauchy sequence if and only if $( b _ { n } ) _ { n = 1 } ^ { \infty }$ is a Cauchy sequence. 

Exercise 5.2.2. Let $\varepsilon > 0$ . Show that if $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ are eventually ε-close, then $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is bounded if and only if $( b _ { n } ) _ { n = 1 } ^ { \infty }$ is bounded. 

## 5.3 The construction of the real numbers

We are now ready to construct the real numbers. We shall introduce a new formal symbol LIM, similar to the formal notations and $/ /$ defined earlier; as the notation suggests, this will eventually match the familiar operation of lim, at which point the formal limit symbol can be discarded. 

Definition 5.3.1 (Real numbers). A real number is defined to be an object of the form $\mathrm { L I M } _ { n \to \infty } a _ { n }$ , where $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is a Cauchy sequence of rational numbers. Two real numbers $\mathrm { L I M } _ { n \to \infty } a _ { n }$ and $\mathrm { L I M } _ { n \to \infty } b _ { n }$ are said to be equal if $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ are equivalent Cauchy sequences. The set of all real numbers is denoted R. 

Example 5.3.2. (Informal) Let $a _ { 1 } , a _ { 2 } , a _ { 3 } , . . .$ . denote the sequence 

1.4, 1.41, 1.414, 1.4142, 1.41421, . . . 

and let $b _ { 1 } , b _ { 2 } , b _ { 3 } , \dotsc$ . denote the sequence 

$$
1. 5, 1. 4 2, 1. 4 1 5, 1. 4 1 4 3, 1. 4 1 4 2 2, \dots
$$

then $\mathrm { L I M } _ { n \to \infty } a _ { n }$ is a real number, and is the same real number as $\mathrm { L I M } _ { n \to \infty } b _ { n }$ , because $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ are equivalent Cauchy sequences: $\mathrm { L I M } _ { n \to \infty } a _ { n } = \mathrm { L I M } _ { n \to \infty } b _ { n }$ 

We will refer to $\mathrm { L I M } _ { n \to \infty } a _ { n }$ as the formal limit of the sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ . Later on we will define a genuine notion of limit, and show that the formal limit of a Cauchy sequence is the same as the limit of that sequence; after that, we will not need formal limits ever again. (The situation is much like what we did with formal subtraction and formal division $/ / . )$ 

In order to ensure that this definition is valid, we need to check that the notion of equality in the definition obeys the first three laws of equality: 

Proposition 5.3.3 (Formal limits are well-defined). Let $x \quad =$ $\mathrm { L I M } _ { n \to \infty } a _ { n } , \ y \ = \mathrm { L I M } _ { n \to \infty } b _ { n }$ , and $z \ = \ \mathrm { L I M } _ { n \to \infty } c _ { n }$ be real numbers. Then, with the above definition of equality for real numbers, we have $x = x$ . Also, if $x = y$ , then $y = x$ . Finally, if $x = y$ and $y = z ,$ , then $x = z$ 

Proof. See Exercise 5.3.1. 

Because of this proposition, we know that our definition of equality between two real numbers is legitimate. Of course, when we define other operations on the reals, we have to check that they obey the law of substitution: two real number inputs which are equal should give equa outputs when applied to any operation on the real numbers. 

Now we want to define on the real numbers all the usual arithmetic operations, such as addition and multiplication. We begin with addition. 

Definition 5.3.4 (Addition of reals). Let $x = \mathrm { L I M } _ { n \to \infty } a _ { n }$ and $y =$ $\mathrm { L I M } _ { n \to \infty } b _ { n }$ be real numbers. Then we define the sum $x + y$ to be $x + y : = \mathrm { L I M } _ { n \to \infty } ( a _ { n } + b _ { n } )$ 

Example 5.3.5. The sum of $\mathrm { L I M } _ { n \to \infty } 1 + 1 / n$ and $\mathrm { L I M } _ { n \to \infty } 2 + 3 / n$ is $\mathrm { L I M } _ { n \to \infty } 3 + 4 / n$ 

We now check that this definition is valid. The first thing we need to do is to confirm that the sum of two real numbers is in fact a rea number: 

Lemma 5.3.6 (Sum of Cauchy sequences is Cauchy). Let $x \quad =$ $\mathrm { L I M } _ { n \to \infty } a _ { n }$ and $y = \operatorname { L I M } _ { n \to \infty } b _ { n }$ be real numbers. Then $x + y$ is also a real number $( i . e . , ( a _ { n } + b _ { n } ) _ { n = 1 } ^ { \infty }$ is a Cauchy sequence of rationals ). 

Proof. We need to show that for every $\varepsilon > 0$ , the sequence $( a _ { n } + b _ { n } ) _ { n = 1 } ^ { \infty }$ is eventually ε-steady. Now from hypothesis we know that $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is eventually ε-steady, and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ is eventually ε-steady, but it turns out that this is not quite enough (this can be used to imply that $( a _ { n } + b _ { n } ) _ { n = 1 } ^ { \infty }$ is eventually $2 \varepsilon { \mathrm { - s t e a d y } } .$ , but that’s not what we want). So we need to do a little trick, which is to play with the value of $\varepsilon$ . 

We know that $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is eventually δ-steady for every value of $\delta .$ This implies not only that $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is eventually ε-steady, but it is also eventually $\varepsilon / 2$ -steady. Similarly, the sequence $( b _ { n } ) _ { n = 1 } ^ { \infty }$ is also eventually $\varepsilon / 2 .$ -steady. This will turn out to be enough to conclude that $( a _ { n } + b _ { n } ) _ { n = 1 } ^ { \infty }$ is eventually ε-steady. 

Since $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is eventually $\varepsilon / 2 .$ -steady, we know that there exists an $N \geq 1$ such that $( a _ { n } ) _ { n = N } ^ { \infty }$ is $\varepsilon / 2 .$ -steady, i.e., $a _ { n }$ and $a _ { m }$ are $\varepsilon / 2 .$ -close for $\mathrm { e v e r y } \ n , m \geq N$ . Similarly there exists an $M \geq 1$ such that $( b _ { n } ) _ { n = M } ^ { \infty }$ is $\varepsilon / 2 { \mathrm { - s t e a d y } } , \mathrm { i } . \mathrm { e } . , b _ { n }$ and $b _ { m }$ are $\varepsilon / 2 .$ -close for every $n , m \geq M$ 

Let max(N, M) be the larger of N and M (we know from Proposition 2.2.13 that one has to be greater than or equal to the other). If $n , m \geq$ max(N, M), then we know that $a _ { n }$ and $a _ { m }$ are $\varepsilon / 2 \mathrm { - c l o s e } .$ , and $b _ { n }$ and $b _ { m }$ are $\varepsilon / 2 .$ -close, and so by Proposition 4.3.7 we see that $a _ { n } + b _ { n }$ and $a _ { m } + b _ { m }$ are ε-close for every $n , m \ge \operatorname* { m a x } ( N , M )$ . This implies that the sequence $( a _ { n } + b _ { n } ) _ { n = 1 } ^ { \infty }$ is eventually ε-close, as desired. □ 

The other thing we need to check is the axiom of substitution (see Section A.7): if we replace a real number x by another number equal to x, this should not change the sum $x + y$ (and similarly if we substitute y by another number equal to $y )$ 

Lemma 5.3.7 (Sums of equivalent Cauchy sequences are equivalent). Let $x = \mathrm { L I M } _ { n \to \infty } a _ { n } , y = \mathrm { L I M } _ { n \to \infty } b _ { n }$ , and $x ^ { \prime } = \mathrm { L I M } _ { n \to \infty } a _ { n } ^ { \prime }$ be real numbers. Suppose that $x = x ^ { \prime }$ . Then we have $x + y = x ^ { \prime } + y$ 

Proof. Since x and $x ^ { \prime }$ are equal, we know that the Cauchy sequences $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( a _ { n } ^ { \prime } ) _ { n = 1 } ^ { \infty }$ are equivalent, so in other words they are eventually ε-close for each $\varepsilon > 0$ . We need to show that the sequences $( a _ { n } + b _ { n } ) _ { n = 1 } ^ { \infty }$ and $( a _ { n } ^ { \prime } + b _ { n } ) _ { n = 1 } ^ { \infty }$ are eventually ε-close for each $\varepsilon > 0$ . But we already know that there is an $N \geq 1$ such that $( a _ { n } ) _ { n = N } ^ { \infty }$ and $( a _ { n } ^ { \prime } ) _ { n = N } ^ { \infty }$ are ε-close, $\mathrm { i . e . }$ , that $a _ { n }$ and $a _ { n } ^ { \prime }$ are ε-close for each $n \geq N$ . Since $b _ { n }$ is of course 0- close to $b _ { n }$ , we thus see from Proposition 4.3.7 (extended in the obvious manner to the $\delta = 0 ~ \mathrm { c a s e } )$ that $a _ { n } + b _ { n }$ and $a _ { n } ^ { \prime } + b _ { n }$ are ε-close for each $n \geq N$ . This implies that $( a _ { n } + b _ { n } ) _ { n = 1 } ^ { \infty }$ and $( a _ { n } ^ { \prime } + b _ { n } ) _ { n = 1 } ^ { \infty }$ are eventually ε-close for each $\varepsilon > 0$ , and we are done. □ 

Remark 5.3.8. The above lemma verifies the axiom of substitution for the $^ { 6 6 } x ^ { \prime }$ variable in $x + y .$ , but one can similarly prove the axiom of substitution for the $^ { \ast } y ^ { \ast }$ variable. (A quick way is to observe from the definition of $x + y$ that we certainly have $x + y = y + x$ , since $a _ { n } + b _ { n } = b _ { n } + a _ { n } . )$ 

We can define multiplication of real numbers in a manner similar to that of addition 

Definition 5.3.9 (Multiplication of reals). Let $x = \mathrm { L I M } _ { n \to \infty } a _ { n }$ and $y = \operatorname { L I M } _ { n \to \infty } b _ { n }$ be real numbers. Then we define the product xy to be $x y : = \operatorname { L I M } _ { n \to \infty } a _ { n } b _ { n }$ 

The following Proposition ensures that this definition is valid, and that the product of two real numbers is in fact a real number: 

Proposition 5.3.10 (Multiplication is well defined). Let $x \quad =$ $\mathrm { L I M } _ { n \to \infty } a _ { n } , y = \mathrm { L I M } _ { n \to \infty } b _ { n }$ , and $x ^ { \prime } = \mathrm { L I M } _ { n \to \infty } a _ { n } ^ { \prime }$ be real numbers. Then xy is also a real number. Furthermore, ${ i f } \ x = x ^ { \prime }$ , then $x y = x ^ { \prime } y$ 

Proof. See Exercise 5.3.2. 

Of course we can prove a similar substitution rule when $y$ is replaced by a real number $y ^ { \prime }$ which is equal to $y .$ 

At this point we embed the rationals back into the reals, by equating every rational number $q$ with the real number $\operatorname { L I M } _ { n \to \infty } q .$ . For instance, if $a _ { 1 } , a _ { 2 } , a _ { 3 } , \dots$ . is the sequence 

then we set $\mathrm { L I M } _ { n \to \infty } a _ { n }$ equal to 0.5. This embedding is consistent with our definitions of addition and multiplication, since for any rational numbers $a , b$ we have 

$$
\begin{array}{l} (\operatorname{LIM} _ {n \to \infty} a) + (\operatorname{LIM} _ {n \to \infty} b) = \operatorname{LIM} _ {n \to \infty} (a + b) \text {and} \\ (\operatorname{LIM} _ {n \to \infty} a) \times (\operatorname{LIM} _ {n \to \infty} b) = \operatorname{LIM} _ {n \to \infty} (a b); \end{array}
$$

this means that when one wants to add or multiply two rational numbers a, b it does not matter whether one thinks of these numbers as rationals or as the real numbers $\mathrm { L I M } _ { n \to \infty } a$ , $\mathrm { L I M } _ { n \to \infty } b$ . Also, this identification of rational numbers and real numbers is consistent with our definitions of equality (Exercise 5.3.3). 

We can now easily define negation x for real numbers x by the formula 

$$
- x := (- 1) \times x,
$$

since 1 is a rational number and is hence real. Note that this is clearly consistent with our negation for rational numbers since we have $- q =$ $( - 1 ) \times q$ for all rational numbers q. Also, from our definitions it is clear that 

$$
- \operatorname{LIM} _ {n \to \infty} a _ {n} = \operatorname{LIM} _ {n \to \infty} (- a _ {n})
$$

(why?). Once we have addition and negation, we can define subtraction as usual by 

$$
x - y := x + (- y),
$$

note that this implies 

$$
\operatorname{LIM} _ {n \to \infty} a _ {n} - \operatorname{LIM} _ {n \to \infty} b _ {n} = \operatorname{LIM} _ {n \to \infty} (a _ {n} - b _ {n}).
$$

We can now easily show that the real numbers obey all the usual rules of algebra (except perhaps for the laws involving division, which we shall address shortly): 

Proposition 5.3.11. All the laws of algebra from Proposition 4.1.6 hold not only for the integers, but for the reals as well. 

Proof. We illustrate this with one such rule: $x ( y + z ) = x y + x z$ . Let $x = \mathrm { L I M } _ { n \to \infty } a _ { n } , y = \mathrm { L I M } _ { n \to \infty } b _ { n }$ , and $z = \mathrm { L I M } _ { n \to \infty } c _ { n }$ be real numbers. Then by definition, $x y = \mathrm { L I M } _ { n \to \infty } a _ { n } b _ { n }$ and $x z = \mathrm { L I M } _ { n \to \infty } a _ { n } c _ { n }$ , and so $x y + x z = \mathrm { L I M } _ { n  \infty } ( a _ { n } b _ { n } + a _ { n } c _ { n } )$ . A similar line of reasoning shows that $x ( y + z ) = \mathrm { L I M } _ { n  \infty } a _ { n } ( b _ { n } + c _ { n } )$ . But we already know that $a _ { n } ( b _ { n } + c _ { n } )$ is equal to $a _ { n } b _ { n } + a _ { n } c _ { n }$ for the rational numbers $a _ { n } , b _ { n } , c _ { n }$ , and the claim follows. The other laws of algebra are proven similarly. □ 

The last basic arithmetic operation we need to define is reciprocation: $x \to x ^ { - 1 }$ . This one is a little more subtle. On obvious first guess for how to proceed would be define 

$$
(\mathrm{LIM} _ {n \to \infty} a _ {n}) ^ {- 1} := \mathrm{LIM} _ {n \to \infty} a _ {n} ^ {- 1},
$$

but there are a few problems with this. For instance, let $a _ { 1 } , a _ { 2 } , a _ { 3 } , \ldots$ be the Cauchy sequence 

$$
0. 1, 0. 0 1, 0. 0 0 1, 0. 0 0 0 1, \dots ,
$$

and let $x \ : = \ \mathrm { L I M } _ { n \to \infty } a _ { n }$ Then by this definition, $x ^ { - 1 }$ would be $\mathrm { L I M } _ { n \to \infty } b _ { n }$ , where $b _ { 1 } , b _ { 2 } , b _ { 3 } , \dotsc$ . is the sequence 

$$
1 0, 1 0 0, 1 0 0 0, 1 0 0 0 0, \dots
$$

but this is not a Cauchy sequence (it isn’t even bounded). Of course, the problem here is that our original Cauchy sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ was equivalent to the zero sequence $( 0 ) _ { n = 1 } ^ { \infty } \mathrm { ( w h y ? ) }$ , and hence that our real number x was in fact equal to 0. So we should only allow the operation of reciprocal when x is non-zero. 

However, even when we restrict ourselves to non-zero real numbers, we have a slight problem, because a non-zero real number might be the formal limit of a Cauchy sequence which contains zero elements. For instance, the number 1, which is rational and hence real, is the formal limit $1 = \operatorname { L I M } _ { n \to \infty } a _ { n }$ of the Cauchy sequence 

$$
0, 0. 9, 0. 9 9, 0. 9 9 9, 0. 9 9 9 9, \dots
$$

but using our naive definition of reciprocal, we cannot invert the real number 1, because we can’t invert the first element 0 of this Cauchy sequence! 

To get around these problems we need to keep our Cauchy sequence away from zero. To do this we first need a definition. 

Definition 5.3.12 (Sequences bounded away from zero). A sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ of rational numbers is said to be bounded away from zero if there exists a rational number $c > 0$ such that $\left| a _ { n } \right| \geq c$ for all $n \geq 1$ 

Examples 5.3.13. The sequence $1 , - 1 , 1 , - 1 , 1 , - 1 , 1 , . . .$ . is bounded away from zero (all the coeficients have absolute value at least 1). But the sequence 0.1, 0.01, 0.001, . . . is not bounded away from zero, and neither is 0, 0.9, 0.99, 0.999, 0.9999, . . .. The sequence 10, 100, 1000, . . . is bounded away from zero, but is not bounded. 

We now show that every non-zero real number is the formal limit of a Cauchy sequence bounded away from zero: 

Lemma 5.3.14. Let x be a non-zero real number. Then $x \quad =$ $\mathrm { L I M } _ { n \to \infty } a _ { n }$ for some Cauchy sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ which is bounded away from zero. 

Proof. Since x is real, we know that $x = \mathrm { L I M } _ { n \to \infty } b _ { n }$ for some Cauchy sequence $( b _ { n } ) _ { n = 1 } ^ { \infty }$ . But we are not yet done, because we do not know that $b _ { n }$ is bounded away from zero. On the other hand, we are given that $x \neq 0 = \mathrm { L I M } _ { n  \infty } 0$ , which means that the sequence $( b _ { n } ) _ { n = 1 } ^ { \infty }$ is not equivalent to $( 0 ) _ { n = 1 } ^ { \infty }$ . Thus the sequence $( b _ { n } ) _ { n = 1 } ^ { \infty }$ cannot be eventually ε-close to $( 0 ) _ { n = 1 } ^ { \infty }$ for every $\varepsilon > 0$ . Therefore we can find an $\varepsilon > 0$ such that $( b _ { n } ) _ { n = 1 } ^ { \infty }$ is not eventually ε-close to $( 0 ) _ { n = 1 } ^ { \infty }$ 

Let us fix this ε. We know that $( b _ { n } ) _ { n = 1 } ^ { \infty }$ is a Cauchy sequence, so it is eventually ε-steady. Moreover, it is eventually ε/2-steady, since $\varepsilon / 2 > 0$ Thus there is an $N \geq 1$ such that $| b _ { n } - b _ { m } | \leq \varepsilon / 2$ for all $n , m \geq N$ 

On the other hand, we cannot have $| b _ { n } | \leq \varepsilon$ for all $n \geq N$ , since this would imply that $( b _ { n } ) _ { n = 1 } ^ { \infty }$ is eventually ε-close to $( 0 ) _ { n = 1 } ^ { \infty }$ . Thus there must be some $n _ { 0 } \geq N$ for which $| b _ { n _ { 0 } } | > \varepsilon$ . Since we already know that $| b _ { n 0 } - b _ { n } | \leq \varepsilon / 2$ for all $n \geq N$ , we thus conclude from the triangle inequality (how?) that $| b _ { n } | \geq \varepsilon / 2$ for all $n \geq N$ 

This almost proves that $( b _ { n } ) _ { n = 1 } ^ { \infty }$ is bounded away from zero. Actually, what it does is show that $( b _ { n } ) _ { n = 1 } ^ { \infty }$ is eventually bounded away from zero. But this is easily fixed, by defining a new sequence $a _ { n }$ , by setting $a _ { n } : = \varepsilon / 2$ if $n < N$ and $a _ { n } : = b _ { n }$ if $n \geq N$ . Since $b _ { n }$ is a Cauchy sequence, it is not hard to verify that $a _ { n }$ is also a Cauchy sequence which is equivalent to $b _ { n }$ (because the two sequences are eventually the same), and so $x = \operatorname { L I M } _ { n \to \infty } a _ { n }$ . And since $| b _ { n } | \geq \varepsilon / 2$ for all $n \geq N$ , we know that $| a _ { n } | \geq \varepsilon / 2$ for all $n \geq 1$ (splitting into the two cases $n \geq N$ and $n < N$ separately). Thus we have a Cauchy sequence which is bounded away from zero $( \mathrm { b y } \varepsilon / 2$ instead of $\varepsilon ,$ , but that’s still OK since $\varepsilon / 2 > 0 )$ , and which has x as a formal limit, and so we are done. □ 

Once a sequence is bounded away from zero, we can take its reciprocal without any dificulty: 

Lemma 5.3.15. Suppose that $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is a Cauchy sequence which is bounded away from zero. Then the sequence $( a _ { n } ^ { - 1 } ) _ { n = 1 } ^ { \infty }$ is also a Cauchy sequence. 

Proof. Since $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is bounded away from zero, we know that there is a $c > 0$ such that $\left| a _ { n } \right| \geq c$ for all $n \geq 1$ . Now we need to show that $( a _ { n } ^ { - 1 } ) _ { n = 1 } ^ { \infty }$ is eventually ε-steady for each $\varepsilon > 0$ . Thus let us fix an $\varepsilon > 0$ ; our task is now to find an $N \geq 1$ such that $| a _ { n } ^ { - 1 } - a _ { m } ^ { - 1 } | \leq \varepsilon$ for all $n , m \geq N$ . But 

$$
| a _ {n} ^ {- 1} - a _ {m} ^ {- 1} | = \left| \frac {a _ {m} - a _ {n}}{a _ {m} a _ {n}} \right| \leq \frac {| a _ {m} - a _ {n} |}{c ^ {2}}
$$

(since $\left| a _ { m } \right| , \left| a _ { n } \right| \geq c )$ , and so to make $| a _ { n } ^ { - 1 } - a _ { m } ^ { - 1 } |$ less than or equal to $\varepsilon _ { i }$ , it will sufice to make $\left| a _ { m } - a _ { n } \right|$ less than or equal to $c ^ { 2 } \varepsilon$ . But since $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is a Cauchy sequence, and $c ^ { 2 } \varepsilon > 0$ , we can certainly find an N such that the sequence $( a _ { n } ) _ { n = N } ^ { \infty }$ is $c ^ { 2 } \varepsilon { \mathrm { - s t e a d y } } ,$ , i.e., $| a _ { m } - a _ { n } | \leq c ^ { 2 } \varepsilon$ for all $n \geq N$ . By what we have said above, this shows that $| a _ { n } ^ { - 1 } - a _ { m } ^ { - 1 } | \leq \varepsilon$ for all $m , n \geq N$ , and hence the sequence $( a _ { n } ^ { - 1 } ) _ { n = 1 } ^ { \infty }$ is eventually ε-steady. Since we have proven this for every ε, we have that $( a _ { n } ^ { - 1 } ) _ { n = 1 } ^ { \infty }$ is a Cauchy sequence, as desired. □ 

We are now ready to define reciprocation: 

Definition 5.3.16 (Reciprocals of real numbers). Let x be a non-zero real number. Let $( a _ { n } ) _ { n = 1 } ^ { \infty }$ be a Cauchy sequence bounded away from zero such that $x = \mathrm { L I M } _ { n \to \infty } a _ { n }$ (such a sequence exists by Lemma 5.3.14). Then we define the reciprocal $x ^ { - 1 }$ by the formula x $^ { - 1 } : = \mathrm { L I M } _ { n \to \infty } a _ { n } ^ { - 1 }$ (From Lemma 5.3.15 we know that $x ^ { - 1 }$ is a real number.) 

We need to check one thing before we are sure this definition makes sense: what if there are two diferent Cauchy sequences $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ which have x as their formal limit, $x \ = \ \mathrm { L I M } _ { n \to \infty } a _ { n } \ =$ $\mathrm { L I M } _ { n \to \infty } b _ { n }$ . The above definition might conceivably give two diferent reciprocals $x ^ { - 1 }$ , namely $\mathrm { L I M } _ { n \to \infty } a _ { n } ^ { - 1 }$ and $\mathrm { L I M } _ { n \to \infty } b _ { n } ^ { - 1 }$ . Fortunately, this never happens: 

Lemma 5.3.17 (Reciprocation is well defined). Let $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ be two Cauchy sequences bounded away from zero such that $\mathrm { L I M } _ { n \to \infty } a _ { n } \ = \ \mathrm { L I M } _ { n \to \infty } b _ { n } ( i . e . _ { ; }$ , the two sequences are equivalent). Then $\mathrm { L I M } _ { n \to \infty } a _ { n } ^ { - 1 } = \mathrm { L I M } _ { n \to \infty } b _ { n } ^ { - 1 }$ 

Proof. Consider the following product P of three real numbers: 

$$
P := (\mathrm{LIM} _ {n \to \infty} a _ {n} ^ {- 1}) \times (\mathrm{LIM} _ {n \to \infty} a _ {n}) \times (\mathrm{LIM} _ {n \to \infty} b _ {n} ^ {- 1}).
$$

If we multiply this out, we obtain 

$$
P = \mathrm{LIM} _ {n \to \infty} a _ {n} ^ {- 1} a _ {n} b _ {n} ^ {- 1} = \mathrm{LIM} _ {n \to \infty} b _ {n} ^ {- 1}.
$$

On the other hand, since $\mathrm { L I M } _ { n \to \infty } a _ { n } = \mathrm { L I M } _ { n \to \infty } b _ { n }$ , we can write P in another way as 

$$
P = (\mathrm{LIM} _ {n \to \infty} a _ {n} ^ {- 1}) \times (\mathrm{LIM} _ {n \to \infty} b _ {n}) \times (\mathrm{LIM} _ {n \to \infty} b _ {n} ^ {- 1})
$$

(cf. Proposition 5.3.10). Multiplying things out again, we get 

$$
P = \mathrm{LIM} _ {n \to \infty} a _ {n} ^ {- 1} b _ {n} b _ {n} ^ {- 1} = \mathrm{LIM} _ {n \to \infty} a _ {n} ^ {- 1}.
$$

Comparing our diferent formulae for P we see that $\scriptstyle \mathrm { L I M } _ { n \to \infty } a _ { n } ^ { - 1 } \ =$ $\mathrm { L I M } _ { n \to \infty } b _ { n } ^ { - 1 }$ , as desired. □ 

Thus reciprocal is well-defined (for each non-zero real number $x ,$ we have exactly one definition of the reciprocal $x ^ { - 1 } )$ . Note it is clear from the definition that $x x ^ { - 1 } = x ^ { - 1 } x = 1 \ \mathrm { ( w h y ? ) }$ ; thus all the field axioms (Proposition 4.2.4) apply to the reals as well as to the rationals. We of course cannot give 0 a reciprocal, since 0 multiplied by anything gives 0, not 1. Also note that if $q$ is a non-zero rational, and hence equal to the real number $\mathrm { L I M } _ { n \to \infty } q$ , then the reciprocal of $\mathrm { L I M } _ { n \to \infty } q$ is $\mathrm { L I M } _ { n \to \infty } q ^ { - 1 } = q ^ { - 1 }$ ; thus the operation of reciprocal on real numbers is consistent with the operation of reciprocal on rational numbers. 

Once one has reciprocal, one can define division $x / y$ of two real numbers x, y, provided y is non-zero, by the formula 

$$
x / y := x \times y ^ {- 1},
$$

just as we did with the rationals. In particular, we have the cancellation law: if x, y, z are real numbers such that $x z = y z ,$ , and z is non-zero, then by dividing by z we conclude that $x = y$ . Note that this cancellation law does not work when z is zero. 

We now have all four of the basic arithmetic operations on the reals: addition, subtraction, multiplication, and division, with all the usual rules of algebra. Next we turn to the notion of order on the reals. 

— Exercises — 

Exercise 5.3.1. Prove Proposition 5.3.3. (Hint: you may find Proposition 4.3.7 to be useful.) 

Exercise 5.3.2. Prove Proposition 5.3.10. (Hint: again, Proposition 4.3.7 may be useful.) 

Exercise 5.3.3. Let a, b be rational numbers. Show that $a = b$ if and only if $\mathrm { L I M } _ { n \to \infty } a = \mathrm { L I M } _ { n \to \infty } b ( \mathrm { i . e . }$ , the Cauchy sequences $a , a , a , a , \ldots$ . and $b , b , b , b \dots$ equivalent if and only if $a = b )$ . This allows us to embed the rational numbers inside the real numbers in a well-defined manner. 

Exercise 5.3.4. Let $( a _ { n } ) _ { n = 0 } ^ { \infty }$ be a sequence of rational numbers which is bounded. Let $( b _ { n } ) _ { n = 0 } ^ { \infty }$ be another sequence of rational numbers which is equivalent to $( a _ { n } ) _ { n = 0 } ^ { \infty }$ . Show that $( b _ { n } ) _ { n = 0 } ^ { \infty }$ is also bounded. (Hint: use Exercise 5.2.2.) 

Exercise 5.3.5. Show that $\mathrm { L I M } _ { n \to \infty } 1 / n = 0$ 

## 5.4 Ordering the reals

We know that every rational number is positive, negative, or zero. We now want to say the same thing for the reals: each real number should be positive, negative, or zero. Since a real number x is just a formal limit of rationals $a _ { n }$ , it is tempting to make the following definition: a real number $x = \operatorname { L I M } _ { n \to \infty } a _ { n }$ is positive if all of the $a _ { n }$ are positive, and negative if all of the $a _ { n }$ are negative (and zero if all of the $a _ { n }$ are zero). However, one soon realizes some problems with this definition. For instance, the sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ defined by $a _ { n } : = 1 0 ^ { - n }$ , thus 

$$
0. 1, 0. 0 1, 0. 0 0 1, 0. 0 0 0 1, \dots
$$

consists entirely of positive numbers, but this sequence is equivalent to the zero sequence $0 , 0 , 0 , 0 , \ldots$ and thus $\mathrm { L I M } _ { n \to \infty } a _ { n } = 0$ . Thus even though all the rationals were positive, the real formal limit of these rationals was zero rather than positive. Another example is 

$$
0. 1, - 0. 0 1, 0. 0 0 1, - 0. 0 0 0 1, \dots ;
$$

this sequence is a hybrid of positive and negative numbers, but again the formal limit is zero. 

The trick, as with the reciprocals in the previous section, is to limit one’s attention to sequences which are bounded away from zero. 

Definition 5.4.1. Let $( a _ { n } ) _ { n = 1 } ^ { \infty }$ be a sequence of rationals. We say that this sequence is positively bounded away from zero if we have a positive rational $c > 0$ such that $a _ { n } \geq c$ for all $n \geq 1$ (in particular, the sequence is entirely positive). The sequence is negatively bounded away from zero if we have a negative rational $- c < 0$ such that $a _ { n } \leq - c$ for all $n \geq 1$ (in particular, the sequence is entirely negative). 

Examples 5.4.2. The sequence 1.1, 1.01, 1.001, 1.0001, . . . is positively bounded away from zero (all terms are greater than or equal to 1). The sequence $- 1 . 1 , - 1 . 0 1 , - 1 . 0 0 1 , - 1 . 0 0 0 1 , . . .$ is negatively bounded away from zero. The sequence 1, 1, 1, 1, 1, 1, . . . is bounded away from zero, but is neither positively bounded away from zero nor negatively bounded away from zero. 

It is clear that any sequence which is positively or negatively bounded away from zero, is bounded away from zero. Also, a sequence cannot be both positively bounded away from zero and negatively bounded away from zero at the same time. 

Definition 5.4.3. A real number x is said to be positive if it can be written as $x = \operatorname { L I M } _ { n \to \infty } a _ { n }$ for some Cauchy sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ which is positively bounded away from zero. x is said to be negative if it can be written as $x = \operatorname { L I M } _ { n \to \infty } a _ { n }$ for some sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ which is negatively bounded away from zero. 

Proposition 5.4.4 (Basic properties of positive reals). For every real number x, exactly one of the following three statements is true: (a) x is zero; (b) x is positive; (c) x is negative. A real number x is negative if and only $_ { i f - x }$ is positive. If x and y are positive, then so are $x + y$ and xy. 

Proof. See Exercise 5.4.1. 

Note that if q is a positive rational number, then the Cauchy sequence $q , q , q , . . .$ . is positively bounded away from zero, and hence $\scriptstyle \mathrm { L I M } _ { n \to \infty } q =$ q is a positive real number. Thus the notion of positivity for rationals is consistent with that for reals. Similarly, the notion of negativity for rationals is consistent with that for reals. 

Once we have defined positive and negative numbers, we can define absolute value and order. 

Definition 5.4.5 (Absolute value). Let x be a real number. We define the absolute value $| x |$ of x to equal x if x is positive, x when x is negative, and 0 when x is zero. 

Definition 5.4.6 (Ordering of the real numbers). Let x and $y$ be real numbers. We say that x is greater than $y ,$ and write $x > y .$ , if $x - y$ is a positive real number, and $x < y$ if $x - y$ is a negative real number. We define $x \geq y { \mathrm { ~ i f f ~ } } x > y { \mathrm { ~ o r ~ } } x = y .$ , and similarly define $x \leq y$ 

Comparing this with the definition of order on the rationals from Definition 4.2.8 we see that order on the reals is consistent with order on the rationals, i.e., if two rational numbers $q , q ^ { \prime }$ are such that $q$ is less than $q ^ { \prime }$ in the rational number system, then $q$ is still less than $q ^ { \prime }$ in the real number system, and similarly for “greater than”. In the same way we see that the definition of absolute value given here is consistent with that in Definition 4.3.1. 

Proposition 5.4.7. All the claims in Proposition 4.2.9 which held for rationals, continue to hold for real numbers. 

Proof. We just prove one of the claims and leave the rest to Exercise 5.4.2. Suppose we have $x < y$ and $z \textrm { a }$ positive real, and want to conclude that $x z < y z$ . Since $x < y , y - x$ is positive, hence by Proposition 5.4.4 we have $( y - x ) z = y z - x z$ is positive, hence $x z < y z$ □ 

As an application of these propositions, we prove 

Proposition 5.4.8. Let x be a positive real number. Then $x ^ { - 1 }$ is also positive. Also, if y is another positive number and $x > y$ , then $x ^ { - 1 } <$ $y ^ { - 1 }$ 

Proof. Let x be positive. Since $x x ^ { - 1 } = 1$ , the real number $x ^ { - 1 }$ cannot be zero (since $x 0 = 0 \neq 1 )$ . Also, from Proposition 5.4.4 it is easy to see that a positive number times a negative number is negative; this shows that $x ^ { - 1 }$ cannot be negative, since this would imply that $x x ^ { - 1 } = 1$ is negative, a contradiction. Thus, by Proposition 5.4.4, the only possibility left is that $x ^ { - 1 }$ is positive. 

Now let y be positive as well, so $x ^ { - 1 }$ and $y ^ { - 1 }$ are also positive. If $x ^ { - 1 } \geq y ^ { - 1 }$ , then by Proposition 5.4.7 we have $x x ^ { - 1 } > y x ^ { - 1 } \geq y y ^ { - 1 }$ thus $1 > 1$ , which is a contradiction. Thus we must have $x ^ { - 1 } < y ^ { - 1 } . \quad \sqcup$ 

Another application is that the laws of exponentiation (Proposition 4.3.12) that were previously proven for rationals, are also true for reals; see Section 5.6. 

We have already seen that the formal limit of positive rationals need not be positive; it could be zero, as the example $0 . 1 , 0 . 0 1 , 0 . 0 0 1 , . . .$ showed. However, the formal limit of non-negative rationals (i.e., rationals that are either positive or zero) is non-negative. 

Proposition 5.4.9 (The non-negative reals are closed). Let $a _ { 1 } , \ a _ { 2 }$ $a _ { 3 } , . . .$ be a Cauchy sequence of non-negative rational numbers. Then $\mathrm { L I M } _ { n \to \infty } a _ { n }$ is a non-negative real number. 

Eventually, we will see a better explanation of this fact: the set of non-negative reals is closed, whereas the set of positive reals is open. See Section 11.4. 

Proof. We argue by contradiction, and suppose that the real number $x : = \mathrm { L I M } _ { n \to \infty } a _ { n }$ is a negative number. Then by definition of negative real number, we have $x = \mathrm { L I M } _ { n \to \infty } b _ { n }$ for some sequence $b _ { n }$ which is negatively bounded away from zero, i.e., there is a negative rational $- c < 0$ such that $b _ { n } \leq - c$ for all $n \geq 1$ . On the other hand, we have $a _ { n } \geq 0$ for all $n \geq 1$ , by hypothesis. Thus the numbers $a _ { n }$ and $b _ { n }$ are never $c / 2 \mathrm { - c l o s e }$ , since $c / 2 < c$ . Thus the sequences $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ are not eventually $c / 2 \mathrm { - c l o s e }$ . Since $c / 2 > 0$ , this implies that $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ are not equivalent. But this contradicts the fact that both these sequences have x as their formal limit. □ 

Corollary 5.4.10. Let $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ be Cauchy sequences of rationals such that $a _ { n } ~ \geq ~ b _ { n }$ for all $n \geq 1$ . Then $\mathrm { L I M } _ { n  \infty } a _ { n } \geq$ $\mathrm { L I M } _ { n \to \infty } b _ { n }$ 

Proof. Apply Proposition 5.4.9 to the sequence $a _ { n } - b _ { n }$ 

Remark 5.4.11. Note that the above Corollary does not work if the $\geq$ signs are replaced by $> :$ for instance if $a _ { n } : = 1 + 1 / n$ and $b _ { n } : = 1 - 1 / n ,$ then $a _ { n }$ is always strictly greater than $b _ { n }$ , but the formal limit of $a _ { n }$ is not greater than the formal limit of $b _ { n }$ , instead they are equal. 

We now define distance $d ( x , y ) : = | x - y |$ just as we did for the rationals. In fact, Propositions 4.3.3 and 4.3.7 hold not only for the rationals, but for the reals; the proof is identical, since the real numbers obey all the laws of algebra and order that the rationals do. 

We now observe that while positive real numbers can be arbitrarily large or small, they cannot be larger than all of the positive integers, or smaller in magnitude than all of the positive rationals: 

Proposition 5.4.12 (Bounding of reals by rationals). Let x be a positive real number. Then there exists a positive rational number q such that $q \leq x$ , and there exists a positive integer N such that $x \leq N$ 

Proof. Since x is a positive real, it is the formal limit of some Cauchy sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ which is positively bounded away from zero. Also, by Lemma 5.1.15, this sequence is bounded. Thus we have rationals $q > 0$ and r such that $q \leq a _ { n } \leq r$ for all $n \geq 1$ . But by Proposition 4.4.1 we know that there is some integer N such that $r \leq N$ ; since q is positive and $q \ \leq \ r \ \leq \ N$ , we see that N is positive. Thus $q \ \leq \ a _ { n } \ \leq \ N$ for all $n \geq 1$ . Applying Corollary 5.4.10 we obtain that $q \leq x \leq N$ , as desired. □ 

Corollary 5.4.13 (Archimedean property). Let x and ε be any positive real numbers. Then there exists a positive integer M such that $M \varepsilon > x$ 

Proof. The number $x / \varepsilon$ is positive, and hence by Proposition 5.4.12 there exists a positive integer N such that $x / \varepsilon \leq N$ . If we set $M : =$ $N + 1$ , then $x / \varepsilon < M$ . Now multiply by ε. □ 

This property is quite important; it says that no matter how large x is and how small ε is, if one keeps adding ε to itself, one will eventually overtake x. 

Proposition 5.4.14. Given any two real numbers $x < y$ , we can find a rational number q such that $x < q < y$ 

Proof. See Exercise 5.4.5. 

We have now completed our construction of the real numbers. This number system contains the rationals, and has almost everything that the rational number system has: the arithmetic operations, the laws of algebra, the laws of order. However, we have not yet demonstrated any advantages that the real numbers have over the rationals; so far, even after much efort, all we have done is shown that they are at least as good as the rational number system. But in the next few sections we show that the real numbers can do more things than rationals: for example, we can take square roots in a real number system. 

Remark 5.4.15. Up until now, we have not addressed the fact that real numbers can be expressed using the decimal system. For instance, the formal limit of 

## 1.4, 1.41, 1.414, 1.4142, 1.41421, . . .

is more conventionally represented as the decimal 1.41421 . . .. We wil address this in an Appendix ( B), but for now let us just remark that there are some subtleties in the decimal system, for instance 0.9999 . . . and 1.000 . . . are in fact the same real number. 

## — Exercises —

Exercise 5.4.1. Prove Proposition 5.4.4. (Hint: if x is not zero, and x is the formal limit of some sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ , then this sequence cannot be eventually ε-close to the zero sequence $( 0 ) _ { n = 1 } ^ { \infty }$ for every single $\varepsilon > 0$ . Use this to show that the sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is eventually either positively bounded away from zero or negatively bounded away from zero.) 

Exercise 5.4.2. Prove the remaining claims in Proposition 5.4.7. 

Exercise 5.4.3. Show that for every real number x there is exactly one integer N such that $N \leq x < N + 1$ . (This integer N is called the integer part of x, and is sometimes denoted $N = \lfloor x \rfloor . )$ 

Exercise 5.4.4. Show that for any positive real number $x > 0$ there exists a positive integer N such that $x > 1 / N > 0$ 

Exercise 5.4.5. Prove Proposition 5.4.14. (Hint: use Exercise 5.4.4. You may also need to argue by contradiction.) 

Exercise 5.4.6. Let x, y be real numbers and let $\varepsilon > 0$ be a positive real. Show that $| x - y | < \varepsilon$ if and only if $y - \varepsilon < x < y + \varepsilon$ , and that $| x - y | \leq \varepsilon { \mathrm { ~ i f ~ } }$ and only if $y - \varepsilon \leq x \leq y + \varepsilon$ 

Exercise 5.4.7. Let x and y be real numbers. Show that $x \leq y + \varepsilon$ for all real numbers $\varepsilon > 0$ if and only if $x \leq y$ . Show that $| x - y | \leq \varepsilon$ for all real numbers $\varepsilon > 0$ if and only if $x = y$ 

Exercise 5.4.8. Let $( a _ { n } ) _ { n = 1 } ^ { \infty }$ be a Cauchy sequence of rationals, and let x be a real number. Show that if $a _ { n } \ \leq \ x$ for all $n \geq 1$ , then $\mathrm { L I M } _ { n \to \infty } a _ { n } \le x$ Similarly, show that if $a _ { n } \geq x$ for all $n \geq 1$ , then $\mathrm { L I M } _ { n \to \infty } a _ { n } \geq x$ . (Hint: prove by contradiction. Use Proposition 5.4.14 to find a rational between $\mathrm { L I M } _ { n \to \infty } a _ { n }$ and x, and then use Proposition 5.4.9 or Corollary 5.4.10.) 

## 5.5 The least upper bound property

We now give one of the most basic advantages of the real numbers over the rationals; one can take the least upper bound sup(E) of any subset E of the real numbers R. 

Definition 5.5.1 (Upper bound). Let E be a subset of R, and let M be a real number. We say that M is an upper bound for E, if we have $x \leq M$ for every element x in E. 

Example 5.5.2. Let E be the interval $E : = \{ x \in \mathbf { R } : 0 \leq x \leq 1 \}$ . Then 1 is an upper bound for E, since every element of E is less than or equal to 1. It is also true that 2 is an upper bound for E, and indeed every number greater or equal to 1 is an upper bound for E. On the other hand, any other number, such as 0.5, is not an upper bound, because 0.5 is not larger than every element in E. (Merely being larger than some elements of E is not necessarily enough to make 0.5 an upper bound.) 

Example 5.5.3. Let $\mathbf { R } ^ { + }$ be the set of positive reals: $\mathbf { R } ^ { + } : = \{ x \in \mathbf { R }$ $x > 0 \}$ . Then $\mathbf { R } ^ { + }$ does not have any upper bounds<sup>3</sup> at all (why?). 

Example 5.5.4. Let $\varnothing$ be the empty set. Then every number M is an upper bound for $\varnothing ,$ , because M is greater than every element of the empty set (this is a vacuously true statement, but still true). 

It is clear that if M is an upper bound of E, then any larger number $M ^ { \prime } \geq M$ is also an upper bound of E. On the other hand, it is not so clear whether it is also possible for any number smaller than M to also be an upper bound of E. This motivates the following definition: 

Definition 5.5.5 (Least upper bound). Let E be a subset of R, and M be a real number. We say that M is a least upper bound for E if (a) M is an upper bound for $E _ { i }$ , and also (b) any other upper bound $M ^ { \prime }$ for E must be larger than or equal to M. 

Example 5.5.6. Let E be the interval $E : = \{ x \in \mathbf { R } : 0 \leq x \leq 1 \}$ Then, as noted before, E has many upper bounds, indeed every number greater than or equal to 1 is an upper bound. But only 1 is the least upper bound; all other upper bounds are larger than 1. 

Example 5.5.7. The empty set does not have a least upper bound (why?). 

Proposition 5.5.8 (Uniqueness of least upper bound). Let E be a subset of R. Then E can have at most one least upper bound. 

Proof. Let $M _ { 1 }$ and $M _ { 2 }$ be two least upper bounds, say $M _ { 1 }$ and $M _ { 2 }$ Since $M _ { 1 }$ is a least upper bound and $M _ { 2 }$ is an upper bound, then by definition of least upper bound we have $M _ { 2 } \geq M _ { 1 }$ . Since $M _ { 2 }$ is a least upper bound and $M _ { 1 }$ is an upper bound, we similarly have $M _ { 1 } \ge M _ { 2 }$ Thus $M _ { 1 } = M _ { 2 }$ . Thus there is at most one least upper bound. □ 

Now we come to an important property of the real numbers: 

Theorem 5.5.9 (Existence of least upper bound). Let E be a nonempty subset of R. If E has an upper bound, (i.e., E has some upper bound M), then it must have exactly one least upper bound. 

Proof. This theorem will take quite a bit of efort to prove, and many of the steps will be left as exercises. 

Let E be a non-empty subset of R with an upper bound M. $\mathrm { B y }$ Proposition 5.5.8, we know that E has at most one least upper bound; we have to show that $E$ has at least one least upper bound. Since $E$ is non-empty, we can choose some element $x _ { 0 }$ in $E$ 

Let $n \geq 1$ be a positive integer. We know that E has an upper bound M. By the Archimedean property (Corollary 5.4.13), we can find an integer K such that $K / n \ge M$ , and hence $K / n$ is also an upper bound for E. By the Archimedean property again, there exists another integer L such that $L / n < x _ { 0 }$ . Since $x _ { 0 }$ lies in $E _ { i }$ , we see that $L / n$ is not an upper bound for $E$ . Since $K / n$ is an upper bound but $L / n$ is not, we see that $K \geq L$ 

Since $K / n$ is an upper bound for E and $L / n$ is not, we can find an integer $L < m _ { n } \leq K$ with the property that $m _ { n } / n$ is an upper bound for $E$ , but $( m _ { n } - 1 ) / n$ is not (see Exercise 5.5.2). In fact, this integer $m _ { n }$ is unique (Exercise 5.5.3). We subscript $m _ { n }$ by n to emphasize the fact that this integer m depends on the choice of $n$ . This gives a well-defined (and unique) sequence $m _ { 1 } , m _ { 2 } , m _ { 3 } , . . .$ of integers, with each of the $m _ { n } / n$ being upper bounds and each of the $( m _ { n } - 1 ) / n$ not being upper bounds. 

Now let $N \geq 1$ be a positive integer, and let $n , n ^ { \prime } \geq N$ be integers larger than or equal to $N$ . Since $m _ { n } / n$ is an upper bound for $E$ and $( m _ { n ^ { \prime } } - 1 ) / n ^ { \prime }$ is not, we must have $m _ { n } / n > ( m _ { n ^ { \prime } } - 1 ) / n ^ { \prime } { \mathrm { ~ ( w h y ? ) } }$ . After a little algebra, this implies that 

$$
\frac {m _ {n}}{n} - \frac {m _ {n ^ {\prime}}}{n ^ {\prime}} > - \frac {1}{n ^ {\prime}} \geq - \frac {1}{N}.
$$

Similarly, since $m _ { n ^ { \prime } } / n ^ { \prime }$ is an upper bound for $E$ and $( m _ { n } - 1 ) / n$ is not, we have $m _ { n ^ { \prime } } / n ^ { \prime } > ( m _ { n } - 1 ) / n$ , and hence 

$$
\frac {m _ {n}}{n} - \frac {m _ {n ^ {\prime}}}{n ^ {\prime}} \leq \frac {1}{n} \leq \frac {1}{N}.
$$

Putting these two bounds together, we see that 

$$
\left| \frac {m _ {n}}{n} - \frac {m _ {n ^ {\prime}}}{n ^ {\prime}} \right| \leq \frac {1}{N} \text {   for   all   } n, n ^ {\prime} \geq N \geq 1.
$$

This implies that $\textstyle { \frac { m _ { n } } { n } }$ is a Cauchy sequence (Exercise 5.5.4). Since the $\textstyle { \frac { m _ { n } } { n } }$ are rational numbers, we can now define the real number S as 

$$
S := \operatorname{LIM} _ {n \to \infty} \frac {m _ {n}}{n}.
$$

From Exercise 5.3.5 we conclude that 

$$
S = \mathrm{LIM} _ {n \to \infty} \frac {m _ {n} - 1}{n}.
$$

To finish the proof of the theorem, we need to show that $S$ is the least upper bound for E. First we show that it is an upper bound. Let x be any element of E. Then, since $m _ { n } / n$ is an upper bound for $E ,$ we have $x \leq m _ { n } / n$ for all $n \geq 1$ . Applying Exercise 5.4.8, we conclude that $x \leq \mathrm { L I M } _ { n  \infty } m _ { n } / n = S$ . Thus S is indeed an upper bound for $E .$ 

Now we show it is a least upper bound. Suppose y is an upper bound for E. Since $( m _ { n } - 1 ) / n$ is not an upper bound, we conclude that $y \ge ( m _ { n } - 1 ) / n$ for all $n \geq 1$ . Applying Exercise 5.4.8, we conclude that $y \geq \mathrm { L I M } _ { n  \infty } ( m _ { n } - 1 ) / n = S$ . Thus the upper bound $S$ is less than or equal to every upper bound of $E _ { \mathrm { { i } } }$ , and $S$ is thus a least upper bound of $E .$ □ 

Definition 5.5.10 (Supremum). Let E be a subset of the real numbers. If E is non-empty and has some upper bound, we define sup(E) to be the least upper bound of $E$ (this is well-defined by Theorem 5.5.9). We introduce two additional symbols, + and . If E is non-empty and has no upper bound, we set sup $( E ) : = + \infty ;$ ; if E is empty, we set $\operatorname* { s u p } ( E ) : = - \infty$ . We refer to $\operatorname { s u p } ( E )$ as the supremum of $E _ { \mathrm { { i } } }$ , and also denote it by sup E. 

Remark 5.5.11. At present, + and are meaningless symbols; we have no operations on them at present, and none of our results involving real numbers apply to + and , because these are not real numbers. In Section 6.2 we add + and to the reals to form the extended real number system, but this system is not as convenient to work with as the real number system, because many of the laws of algebra break down. For instance, it is not a good idea to try to define + + ; setting this equal to 0 causes some problems. 

Now we give an example of how the least upper bound property is useful. 

Proposition 5.5.12. There exists a positive real number x such that $x ^ { 2 } = 2$ 

Remark 5.5.13. Comparing this result with Proposition 4.4.4, we see that certain numbers are real but not rational. The proof of this proposition also shows that the rationals Q do not obey the least upper bound property, otherwise one could use that property to construct a square root of 2, which by Proposition 4.4.4 is not possible. 

Proof. Let E be the set $\{ y \in \mathbf { R } : y \geq 0$ and $y ^ { 2 } < 2 \}$ ; thus E is the set of all non-negative real numbers whose square is less than 2. Observe that E has an upper bound of 2 (because if $y > 2$ , then $y ^ { 2 } > 4 > 2$ and hence $y \notin E )$ . Also, E is non-empty (for instance, 1 is an element of E). Thus by the least upper bound property, we have a real number $x : = \operatorname* { s u p } ( E )$ which is the least upper bound of E. Then x is greater than or equal to 1 (since $1 \in E )$ and less than or equal to 2 (since 2 is an upper bound for E). So x is positive. Now we show that $x ^ { 2 } = 2$ 

We argue this by contradiction. We show that both $x ^ { 2 } < 2$ and $x ^ { 2 } > 2$ lead to contradictions. First suppose that $x ^ { 2 } < 2$ . Let $0 < \varepsilon < 1$ be a small number; then we have 

$$
(x + \varepsilon) ^ {2} = x ^ {2} + 2 \varepsilon x + \varepsilon^ {2} \leq x ^ {2} + 4 \varepsilon + \varepsilon = x ^ {2} + 5 \varepsilon
$$

since $x \le 2$ and $\varepsilon ^ { 2 } \leq \varepsilon$ . Since $x ^ { 2 } < 2$ , we see that we can choose an $0 < \varepsilon < 1$ such that $x ^ { 2 } + 5 \varepsilon < 2$ , thus $( x + \varepsilon ) ^ { 2 } < 2$ . By construction of $E _ { i }$ , this means that $x + \varepsilon \in E$ ; but this contradicts the fact that x is an upper bound of E. 

Now suppose that $x ^ { 2 } > 2$ . Let $0 < \varepsilon < 1$ be a small number; then we have 

$$
(x - \varepsilon) ^ {2} = x ^ {2} - 2 \varepsilon x + \varepsilon^ {2} \geq x ^ {2} - 2 \varepsilon x \geq x ^ {2} - 4 \varepsilon
$$

since $x \leq 2$ and $\varepsilon ^ { 2 } \geq 0$ . Since $x ^ { 2 } > 2$ , we can choose $0 < \varepsilon < 1$ such that $x ^ { 2 } - 4 \varepsilon > 2$ , and thus $( x - \varepsilon ) ^ { 2 } > 2$ . But then this implies that $x - \varepsilon \geq y$ for all $y \in E$ . (Why? If $x - \varepsilon < y$ then $( x - \varepsilon ) ^ { 2 } < y ^ { 2 } \leq 2$ , a contradiction.) Thus $x - \varepsilon$ is an upper bound for E, which contradicts the fact that x is the least upper bound of E. From these two contradictions we see that $x ^ { 2 } = 2$ , as desired. □ 

Remark 5.5.14. In Chapter 6 we will use the least upper bound property to develop the theory of limits, which allows us to do many more things than just take square roots. 

Remark 5.5.15. We can of course talk about lower bounds, and greatest lower bounds, of sets $E ;$ the greatest lower bound of a set E is also known as the $i n f i m u m ^ { 4 }$ of E and is denoted inf(E) or inf E. Everything we say about suprema has a counterpart for infima; we will usually leave such statements to the reader. A precise relationship between the two notions is given by Exercise 5.5.1. See also Section 6.2. 

## — Exercises —

Exercise 5.5.1. Let E be a subset of the real numbers R, and suppose that E has a least upper bound M which is a real number, i.e., $M = \operatorname* { s u p } ( E )$ . Let $- E$ be the set 

$$
- E := \{- x: x \in E \}.
$$

Show that M is the greatest lower bound of $- E , { \mathrm { i . e . , ~ } } - M = { \mathrm { i n f } } ( - E )$ 

Exercise 5.5.2. Let E be a non-empty subset of R, let $n \geq 1$ be an integer, and let $L < K$ be integers. Suppose that $K / n$ is an upper bound for $E ,$ but that $L / n$ is not an upper bound for E. Without using Theorem 5.5.9, show that there exists an integer $L < m \leq K$ such that $m / n$ is an upper bound for E, but that $( m - 1 ) / n$ is not an upper bound for E. (Hint: prove by contradiction, and use induction. It may also help to draw a picture of the situation.) 

Exercise 5.5.3. Let E be a non-empty subset of R, let $n \geq 1$ be an integer, and let $m , m ^ { \prime }$ be integers with the properties that $m / n$ and $m ^ { \prime } / n$ are upper bounds for E, but $( m - 1 ) / n$ and $( m ^ { \prime } - 1 ) / n$ are not upper bounds for E. Show that $m = m ^ { \prime }$ . This shows that the integer m constructed in Exercise 5.5.2 is unique. (Hint: again, drawing a picture will be helpful.) 

Exercise 5.5.4. Let $q _ { 1 } , q _ { 2 } , q _ { 3 } , . . .$ . be a sequence of rational numbers with the property that $\begin{array} { r } { | q _ { n } - q _ { n ^ { \prime } } | \le \frac { 1 } { M } } \end{array}$ whenever $M \geq 1$ is an integer and $n , n ^ { \prime } \geq M$ Show that $q _ { 1 } , q _ { 2 } , q _ { 3 } , . . .$ . is a Cauchy sequence. Furthermore, if $S : = \operatorname { L I M } _ { n \to \infty } q _ { n }$ show that $\begin{array} { r } { | q _ { M } - S | \le \frac 1 { M } } \end{array}$ for every $M \geq 1$ . (Hint: use Exercise 5.4.8.) 

Exercise 5.5.5. Establish an analogue of Proposition 5.4.14, in which “rational” is replaced by “irrational”. 

## 5.6 Real exponentiation, part I

In Section 4.3 we defined exponentiation $x ^ { n }$ when x is rational and n is a natural number, or when x is a non-zero rational and n is an integer. Now that we have all the arithmetic operations on the reals (and Proposition 5.4.7 assures us that the arithmetic properties of the rationals that we are used to, continue to hold for the reals) we can similarly define exponentiation of the reals. 

Definition 5.6.1 (Exponentiating a real by a natural number). Let x be a real number. To raise x to the power 0, we define $x ^ { 0 } : = 1$ . Now suppose recursively that $x ^ { n }$ has been defined for some natural number n, then we define $x ^ { n + 1 } : = x ^ { n } \times x$ 

Definition 5.6.2 (Exponentiating a real by an integer). Let x be a non-zero real number. Then for any negative integer n, we define $x ^ { - n } : = 1 / x ^ { n }$ 

Clearly these definitions are consistent with the definition of rational exponentiation given earlier. We can then assert 

Proposition 5.6.3. All the properties in Propositions 4.3.10 and 4.3.12 remain valid if x and y are assumed to be real numbers instead of rational numbers. 

Instead of giving an actual proof of this proposition, we shall give a meta-proof (an argument appealing to the nature of proofs, rather than the nature of real and rational numbers). 

Meta-proof. If one inspects the proof of Propositions 4.3.10 and 4.3.12 we see that they rely on the laws of algebra and the laws of order for the rationals (Propositions 4.2.4 and 4.2.9). But by Propositions 5.3.11, 5.4.7, and the identity $x x ^ { - 1 } = x ^ { - 1 } x = 1$ we know that all these laws of algebra and order continue to hold for real numbers as well as rationals. Thus we can modify the proof of Proposition 4.3.10 and 4.3.12 to hold in the case when x and y are real. - 

Now we consider exponentiation to exponents which are not integers. We begin with the notion of an $n ^ { \mathrm { t h } }$ root, which we can define using our notion of supremum. 

Definition 5.6.4. Let $x \geq 0$ be a non-negative real, and let $n \geq 1$ be a positive integer. We define $x ^ { 1 / n }$ , also known as the $n ^ { \mathrm { t h } }$ root of x, by the formula 

$$
x ^ {1 / n} := \sup \{y \in \mathbf {R}: y \geq 0 \text {   and   } y ^ {n} \leq x \}.
$$

We often write $\sqrt { x }$ for $x ^ { 1 / 2 }$ 

Note we do not define the $n ^ { \mathrm { t h } }$ root of a negative number. In fact, we will leave the $n ^ { \mathrm { t h } }$ roots of negative numbers undefined for the rest of the text (one can define these $n ^ { \mathrm { t h } }$ roots once one defines the complex numbers, but we shall refrain from doing so). 

Lemma 5.6.5 (Existence of $n ^ { \mathrm { t h } }$ roots). Let $x \ge 0$ be a non-negative real, and let $n \geq 1$ be a positive integer. Then the set $E : = \{ y \in \mathbf { R } : y \geq$ 0 and $y ^ { n } \leq x \}$ is non-empty and is also bounded above. In particular, $x ^ { 1 / n }$ is a real number. 

Proof. The set E contains $0 \ \mathrm { ( w h y ? ) }$ , so it is certainly not empty. Now we show it has an upper bound. We divide into two cases: $x \leq 1$ and $x > 1$ . First suppose that we are in the case where $x \le 1$ . Then we claim that the set E is bounded above by 1. To see this, suppose for sake of contradiction that there was an element $y \in E$ for which $y > 1$ . But then $y ^ { n } > 1 \ \mathrm { ( w h y ? ) }$ , and hence $y ^ { n } > x$ , a contradiction. Thus E has an upper bound. Now suppose that we are in the case where $x > 1$ . Then we claim that the set E is bounded above by x. To see this, suppose for contradiction that there was an element $y \in E$ for which $y > x$ . Since $x > 1$ , we thus have $y > 1$ . Since $y > x$ and $y > 1$ , we have $y ^ { n } > x$ $\mathrm { \left( w h y ? \right) }$ , a contradiction. Thus in both cases E has an upper bound, and so $x ^ { 1 / n }$ is finite. □ 

We list some basic properties of $n ^ { \mathrm { t h } }$ root below. 

Lemma 5.6.6. Let $x , y \geq 0$ be non-negative reals, and let $n , m \geq 1$ be positive integers. 

(a) If $y = x ^ { 1 / n }$ , then $y ^ { n } = x$ 

(b) Conversely, if $y ^ { n } = x$ , then $y = x ^ { 1 / n }$ 

(c) $x ^ { 1 / n }$ is a positive real number. 

(d) We have $x > y$ if and only if $x ^ { 1 / n } > y ^ { 1 / n }$ 

(e) $I f x > 1$ , then $x ^ { 1 / k }$ is a decreasing function of k. If $x < 1$ , then $x ^ { 1 / k }$ is an increasing function of k. If $x = 1$ , then $x ^ { 1 / k } = 1$ for all k. 

(f ) We have $( x y ) ^ { 1 / n } = x ^ { 1 / n } y ^ { 1 / n }$ 

(g) We have $( x ^ { 1 / n } ) ^ { 1 / m } = x ^ { 1 / n m }$ 

Proof. See Exercise 5.6.1. 

The observant reader may note that this definition of $x ^ { 1 / n }$ might possibly be inconsistent with our previous notion of $x ^ { n }$ when $n = 1$ , but it is easy to check that $x ^ { 1 / 1 } = x = x ^ { 1 } \left( \mathrm { w h y ? } \right)$ , so there is no inconsistency. 

One consequence of Lemma $5 . 6 . 6 ( \mathrm { b } )$ is the following cancellation law: if $y$ and $z { \mathrm { ~ a r e } }$ positive and $y ^ { n } = z ^ { n }$ , then $y = z$ . (Why does this follow from Lemma $5 . 6 . 6 ( \mathrm { b } ) ? )$ Note that this only works when $y$ and z are positive; for instance, $( - 3 ) ^ { 2 } = 3 ^ { 2 }$ , but we cannot conclude from this that $- 3 = 3$ 

Now we define how to raise a positive number x to a rational exponent $q .$ 

Definition 5.6.7. Let $x > 0$ be a positive real number, and let $q$ be a rational number. To define $x ^ { q }$ , we write $q = a / b$ for some integer a and positive integer $b ,$ , and define 

$$
x ^ {q} := (x ^ {1 / b}) ^ {a}.
$$

Note that every rational $q ,$ whether positive, negative, or zero, can be written in the form $a / b$ where $a$ is an integer and b is positive $\mathrm { \left( w h y ? \right) }$ However, the rational number $q$ can be expressed in the form $a / b$ in more than one way, for instance $1 / 2$ can also be expressed as $2 / 4$ or $3 / 6$ . So to ensure that this definition is well-defined, we need to check that diferent expressions $a / b$ give the same formula for $x ^ { q }$ : 

Lemma 5.6.8. Let $a , a ^ { \prime }$ be integers and $b , b ^ { \prime }$ be positive integers such that $a / b = a ^ { \prime } / b ^ { \prime }$ , and let x be a positive real number. Then we have $( x ^ { 1 / b ^ { \prime } } ) ^ { \dot { a } ^ { \prime } } = ( x ^ { \dot { 1 / b } } ) ^ { a }$ 

Proof. There are three cases: $a = 0 , a > 0 , a < 0$ . If $a = 0$ , then we must have $a ^ { \prime } = 0 ~ \mathrm { ( w h y ? ) }$ and so both $( x ^ { 1 / b ^ { \prime } } ) ^ { a ^ { \prime } }$ and $( x ^ { 1 / b } ) ^ { a }$ are equal to 1, so we are done. 

Now suppose that $a > 0$ . Then $a ^ { \prime } > 0 \mathrm { ~ ( w h y ? ) }$ , and $a b ^ { \prime } = b a ^ { \prime }$ . Write $y : = x ^ { 1 / ( a \hat { b ^ { \prime } } ) } = x ^ { 1 / ( b a ^ { \prime } ) }$ . By Lemma $5 . 6 . 6 ( \mathrm { g } )$ we have $y ~ = ~ ( x ^ { 1 / b ^ { \prime } } ) ^ { 1 / a }$ and $y = ( x ^ { 1 / b } ) ^ { 1 / a ^ { \prime } } ;$ by Lemma $5 . 6 . 6 ( \mathrm { a } )$ we thus have $y ^ { a } = x ^ { 1 / b ^ { \prime } }$ and $y ^ { a ^ { \prime } } = x ^ { 1 / b }$ . Thus we have 

$$
(x ^ {1 / b ^ {\prime}}) ^ {a ^ {\prime}} = (y ^ {a}) ^ {a ^ {\prime}} = y ^ {a a ^ {\prime}} = (y ^ {a ^ {\prime}}) ^ {a} = (x ^ {1 / b}) ^ {a}
$$

as desired. 

Finally, suppose that $a < 0$ . Then we have $( - a ) / b = ( - a ^ { \prime } ) / b$ . But $- a$ is positive, so the previous case applies and we have $( x ^ { 1 / b ^ { \prime } } ) ^ { - a ^ { \prime } } =$ $( x ^ { 1 / b } ) ^ { - a }$ . Taking the reciprocal of both sides we obtain the result. 

Thus $x ^ { q }$ is well-defined for every rational $q .$ . Note that this new definition is consistent with our old definition for $x ^ { 1 / n } \ \mathrm { \Gamma ( w h y ? ) }$ and is also consistent with our old definition for $x ^ { n } { \mathrm { ~ ( w h y ? ) } }$ 

## 5.6. Real exponentiation, part I

Some basic facts about rational exponentiation: 

Lemma 5.6.9. Let $x , y > 0$ be positive reals, and let $q , r$ be rationals. 

(a) $x ^ { q }$ is a positive real. 

(b) $x ^ { q + r } = x ^ { q } x ^ { r }$ and $( x ^ { q } ) ^ { r } = x ^ { q r }$ 

(c) $x ^ { - q } = 1 / x ^ { q }$ 

(d) $I f q > 0$ , then $x > y$ if and only if $x ^ { q } > y ^ { q }$ 

(e) $I f x > 1$ , then $x ^ { q } > x ^ { r }$ if and only if $q > r$ . If $x < 1$ , then $x ^ { q } > x ^ { r }$ if and only if $q < r$ 

Proof. See Exercise 5.6.2. 

We still have to do real exponentiation; in other words, we still have to define $x ^ { y }$ where $x > 0$ and y is a real number - but we will defer that until Section 6.7, once we have formalized the concept of limit. 

In the rest of the text we shall now just assume the real numbers to obey all the usual laws of algebra, order, and exponentiation. 

— Exercises — 

Exercise 5.6.1. Prove Lemma 5.6.6. (Hints: review the proof of Proposition 5.5.12. Also, you will find proof by contradiction a useful tool, especially when combined with the trichotomy of order in Proposition 5.4.7 and Proposition 5.4.12. The earlier parts of the lemma can be used to prove later parts of the lemma. With part (e), first show that if $x > 1$ then $x ^ { 1 / n } > 1$ , and if $x < 1$ then $x ^ { 1 / n } < 1 . )$ 

Exercise 5.6.2. Prove Lemma 5.6.9. (Hint: you should rely mainly on Lemma 5.6.6 and on algebra.) 

Exercise 5.6.3. If x is a real number, show that $| x | = ( x ^ { 2 } ) ^ { 1 / 2 }$ 

# Chapter 6

## Limits of sequences

## 6.1 Convergence and limit laws

In the previous chapter, we defined the real numbers as formal limits of rational (Cauchy) sequences, and we then defined various operations on the real numbers. However, unlike our work in constructing the integers (where we eventually replaced formal diferences with actual diferences) and rationals (where we eventually replaced formal quotients with actual quotients), we never really finished the job of constructing the real numbers, because we never got around to replacing formal limits $\mathrm { L I M } _ { n \to \infty } a _ { n }$ with actual limits $\operatorname* { l i m } _ { n \to \infty } a _ { n }$ . In fact, we haven’t defined limits at all yet. This will now be rectified. 

We begin by repeating much of the machinery of ε-close sequences, etc. again - but this time, we do it for sequences of real numbers, not rational numbers. Thus this discussion will supercede what we did in the previous chapter. First, we define distance for real numbers: 

Definition 6.1.1 (Distance between two real numbers). Given two real numbers x and y, we define their distance $d ( x , y )$ to be $d ( x , y ) : = | x - y |$ 

Clearly this definition is consistent with Definition 4.3.2. Further, Proposition 4.3.3 works just as well for real numbers as it does for rationals, because the real numbers obey all the rules of algebra that the rationals do. 

Definition 6.1.2 (ε-close real numbers). Let $\varepsilon > 0$ be a real number. We say that two real numbers x, y are ε-close if we have $d ( y , x ) \leq \varepsilon$ 

Again, it is clear that this definition of ε-close is consistent with Definition 4.3.4. 

Now let $( a _ { n } ) _ { n = m } ^ { \infty }$ be a sequence of real numbers; i.e., we assign a real number $a _ { n }$ for every integer $n \geq m$ . The starting index m is some integer; usually this will be 1, but in some cases we will start from some index other than 1. (The choice of label used to index this sequence is unimportant; we could use for instance $\left( a _ { k } \right) _ { k = m } ^ { \infty }$ and this would represent exactly the same sequence as $( a _ { n } ) _ { n = m } ^ { \infty } . )$ We can define the notion of a Cauchy sequence in the same manner as before: 

Definition 6.1.3 (Cauchy sequences of reals). Let $\varepsilon > 0$ be a real number. A sequence $( a _ { n } ) _ { n = N } ^ { \infty }$ of real numbers starting at some integer index N is said to be ε-steady if $a _ { j }$ and $a _ { k }$ are ε-close for every $j , k \geq N$ A sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ starting at some integer index m is said to be eventually ε-steady if there exists an $N \ge m$ such that $( a _ { n } ) _ { n = N } ^ { \infty }$ is ε-steady. We say that $( a _ { n } ) _ { n = m } ^ { \infty }$ is a Cauchy sequence if it is eventually ε-steady for every $\varepsilon > 0$ 

To put it another way, a sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ of real numbers is a Cauchy sequence if, for every real $\varepsilon > 0$ , there exists an $N \geq m$ such that $| a _ { n } - a _ { n ^ { \prime } } | \leq \varepsilon$ for all $n , n ^ { \prime } \geq N$ . These definitions are consistent with the corresponding definitions for rational numbers (Definitions 5.1.3, 5.1.6, 5.1.8), although verifying consistency for Cauchy sequences takes a little bit of care: 

Proposition 6.1.4. Let $( a _ { n } ) _ { n = m } ^ { \infty }$ be a sequence of rational numbers starting at some integer index m. Then $( a _ { n } ) _ { n = m } ^ { \infty }$ is a Cauchy sequence in the sense of Definition 5.1.8 if and only if it is a Cauchy sequence in the sense of Definition 6.1.3. 

Proof. Suppose first that $( a _ { n } ) _ { n = m } ^ { \infty }$ is a Cauchy sequence in the sense of Definition 6.1.3; then it is eventually ε-steady for every real $\varepsilon > 0$ In particular, it is eventually ε-steady for every rational $\varepsilon > 0$ , which makes it a Cauchy sequence in the sense of Definition 5.1.8. 

Now suppose that $( a _ { n } ) _ { n = m } ^ { \infty }$ is a Cauchy sequence in the sense of Definition 5.1.8; then it is eventually ε-steady for every rational $\varepsilon > 0$ If $\varepsilon > 0$ is a real number, then there exists a rational $\varepsilon ^ { \prime } > 0$ which is smaller than $\varepsilon ,$ , by Proposition 5.4.12. Since $\varepsilon ^ { \prime }$ is rational, we know that $( a _ { n } ) _ { n = m } ^ { \infty }$ is eventually $\varepsilon ^ { \prime } { \mathrm { - s t e a d y } } ;$ ; since $\varepsilon ^ { \prime } < \varepsilon$ , this implies that $( a _ { n } ) _ { n = m } ^ { \infty }$ is eventually ε-steady. Since $\varepsilon$ is an arbitrary positive real number, we thus see that $( a _ { n } ) _ { n = m } ^ { \infty }$ is a Cauchy sequence in the sense of Definition 6.1.3. □ 

Because of this proposition, we will no longer care about the distinction between Definition 5.1.8 and Definition 6.1.3, and view the concept of a Cauchy sequence as a single unified concept. 

Now we talk about what it means for a sequence of real numbers to converge to some limit L. 

Definition 6.1.5 (Convergence of sequences). Let $\varepsilon > 0$ be a real number, and let L be a real number. A sequence $( a _ { n } ) _ { n = N } ^ { \infty }$ of real numbers is said to be ε-close to L if $a _ { n }$ is ε-close to L for every $n \geq N$ , i.e., we have $| a _ { n } - L | \leq \varepsilon$ for every $n \geq N$ . We say that a sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ is eventually ε-close to L if there exists an $N \geq m$ such that $( a _ { n } ) _ { n = N } ^ { \infty }$ is ε-close to L. We say that a sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ converges to L if it is eventually ε-close to L for every real $\varepsilon > 0$ 

One can unwrap all the definitions here and write the concept of convergence more directly; see Exercise 6.1.2. 

## Examples 6.1.6. The sequence

$$
0. 9, 0. 9 9, 0. 9 9 9, 0. 9 9 9 9, \dots
$$

is 0.1-close to 1, but is not 0.01-close to 1, because of the first element of the sequence. However, it is eventually 0.01-close to 1. In fact, for every real $\varepsilon > 0$ , this sequence is eventually ε-close to 1, hence is convergent to 1. 

Proposition 6.1.7 (Uniqueness of limits). Let $( a _ { n } ) _ { n = m } ^ { \infty }$ be a real sequence starting at some integer index m, and let $L \neq L ^ { \prime }$ be two distinct real numbers. Then it is not possible for $( a _ { n } ) _ { n = m } ^ { \infty }$ to converge to L while also converging to $L ^ { \prime } .$ 

Proof. Suppose for sake of contradiction that $( a _ { n } ) _ { n = m } ^ { \infty }$ was converging to both L and $L ^ { \prime }$ . Let $\varepsilon = | L - L ^ { \prime } | / 3$ ; note that ε is positive since $L \neq L ^ { \prime }$ Since $( a _ { n } ) _ { n = m } ^ { \infty }$ converges to $L ,$ we know that $( a _ { n } ) _ { n = m } ^ { \infty }$ is eventually $\varepsilon -$ close to $L ;$ thus there is an $N \geq m$ such that $d ( a _ { n } , L ) \leq \varepsilon$ for all $n \geq N$ Similarly, there is an $M \geq m$ such that $d ( a _ { n } , L ^ { \prime } ) \leq \varepsilon$ for all $n \geq M$ In particular, if we set $n : = \operatorname* { m a x } ( N , M )$ , then we have $d ( a _ { n } , L ) ~ \leq ~ \varepsilon$ and $d ( a _ { n } , L ^ { \prime } ) ~ \leq ~ \varepsilon$ , hence by the triangle inequality $d ( L , L ^ { \prime } ) \leq 2 \varepsilon =$ $2 | L - L ^ { \prime } | / 3$ . But then we have $| L - L ^ { \prime } | \leq 2 | L - L ^ { \prime } | / 3$ , which contradicts the fact that $| L - L ^ { \prime } | > 0$ . Thus it is not possible to converge to both L and $L ^ { \prime }$ □ 

## 6.1. Convergence and limit laws

Now that we know limits are unique, we can set up notation to specify them: 

Definition 6.1.8 (Limits of sequences). If a sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ converges to some real number $L ,$ we say that $( a _ { n } ) _ { n = m } ^ { \infty }$ is convergent and that its limit is $L ;$ we write 

$$
L = \lim _ {n \to \infty} a _ {n}
$$

to denote this fact. If a sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ is not converging to any real number $L$ , we say that the sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ is divergent and we leave $\operatorname* { l i m } _ { n \to \infty } a _ { n }$ undefined. 

Note that Proposition 6.1.7 ensures that a sequence can have at most one limit. Thus, if the limit exists, it is a single real number, otherwise it is undefined. 

Remark 6.1.9. The notation $\operatorname* { l i m } _ { n \to \infty } a _ { n }$ does not give any indication about the starting index $m$ of the sequence, but the starting index is irrelevant (Exercise 6.1.3). Thus in the rest of this discussion we shall not be too careful as to where these sequences start, as we shall be mostly focused on their limits. 

We sometimes use the phrase $" a _ { n }  x { \mathrm { ~ a s ~ } } n  \infty "$ as an alternate way of writing the statement $^ { 6 6 } ( a _ { n } ) _ { n = m } ^ { \infty }$ converges to $x '$ . Bear in mind, though, that the individual statements $a _ { n } \to x$ and $n \to \infty$ do not have any rigorous meaning; this phrase is just a convention, though of course a very suggestive one. 

Remark 6.1.10. The exact choice of letter used to denote the index (in this case n) is irrelevant: the phrase $\operatorname* { l i m } _ { n \to \infty } a _ { n }$ has exactly the same meaning as $\operatorname* { l i m } _ { k \to \infty } a _ { k }$ , for instance. Sometimes it will be convenient to change the label of the index to avoid conflicts of notation; for instance, we might want to change n to $k$ because n is simultaneously being used for some other purpose, and we want to reduce confusion. See Exercise 6.1.4. 

As an example of a limit, we present 

## Proposition 6.1.11. We have $\textstyle \operatorname* { l i m } _ { n \to \infty } 1 / n = 0$

Proof. We have to show that the sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ converges to 0, where $a _ { n } : = 1 / n$ . In other words, for every $\varepsilon > 0$ , we need to show that the sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is eventually ε-close to 0. So, let $\varepsilon > 0$ be an arbitrary real number. We have to find an N such that $| a _ { n } - 0 | \leq \varepsilon$ for every $n \geq N$ . But if $n \geq N$ , then 

$$
\left| a _ {n} - 0 \right| = \left| 1 / n - 0 \right| = 1 / n \leq 1 / N.
$$

Thus, if we pick $N > 1 / \varepsilon$ (which we can do by the Archimedean principle), then $1 / N < \varepsilon _ { : }$ , and so $( a _ { n } ) _ { n = N } ^ { \infty }$ is ε-close to 0. Thus $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is eventually ε-close to 0. Since ε was arbitrary, $( a _ { n } ) _ { n = 1 } ^ { \infty }$ converges to 0. □ 

Proposition 6.1.12 (Convergent sequences are Cauchy). Suppose that $( a _ { n } ) _ { n = m } ^ { \infty }$ is a convergent sequence of real numbers. Then $( a _ { n } ) _ { n = m } ^ { \infty }$ is also a Cauchy sequence. 

Proof. See Exercise 6.1.5. 

Example 6.1.13. The sequence $1 , - 1 , 1 , - 1 , 1 , - 1 , . . .$ . is not a Cauchy sequence (because it is not eventually 1-steady), and is hence not a convergent sequence, by Proposition 6.1.12. 

Remark 6.1.14. For a converse to Proposition 6.1.12, see Theorem 6.4.18 below. 

Now we show that formal limits can be superceded by actual limits, just as formal subtraction was superceded by actual subtraction when constructing the integers, and formal division superceded by actual division when constructing the rational numbers. 

Proposition 6.1.15 (Formal limits are genuine limits). Suppose that $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is a Cauchy sequence of rational numbers. Then $( a _ { n } ) _ { n = 1 } ^ { \infty }$ converges to $\mathrm { L I M } _ { n \to \infty } a _ { n }$ , i.e. 

$$
\operatorname{LIM} _ {n \to \infty} a _ {n} = \lim _ {n \to \infty} a _ {n}.
$$

Proof. See Exercise 6.1.6. 

Definition 6.1.16 (Bounded sequences). A sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ of real numbers is bounded by a real number M if we have $| a _ { n } | \leq M$ for all $n \geq m$ . We say that $( a _ { n } ) _ { n = m } ^ { \infty }$ is bounded if it is bounded by M for some real number $M > 0$ 

## 6.1. Convergence and limit laws

This definition is consistent with Definition 5.1.12; see Exercise 6.1.7. 

Recall from Lemma 5.1.15 that every Cauchy sequence of rational numbers is bounded. An inspection of the proof of that Lemma shows that the same argument works for real numbers; every Cauchy sequence of real numbers is bounded. In particular, from Proposition 6.1.12 we see have 

Corollary 6.1.17. Every convergent sequence of real numbers is bounded. 

Example 6.1.18. The sequence 1, 2, 3, 4, 5, . . . is not bounded, and hence is not convergent. 

We can now prove the usual limit laws. 

Theorem 6.1.19 (Limit Laws). Let $( a _ { n } ) _ { n = m } ^ { \infty }$ and $( b _ { n } ) _ { n = m } ^ { \infty }$ be convergent sequences of real numbers, and let x, y be the real numbers $x : = \dim _ { n \to \infty } a _ { n }$ and $y : = \dim _ { n \to \infty } b _ { n }$ 

(a) The sequence $( a _ { n } + b _ { n } ) _ { n = m } ^ { \infty }$ converges to $x + y ;$ in other words, 

$$
\lim _ {n \to \infty} (a _ {n} + b _ {n}) = \lim _ {n \to \infty} a _ {n} + \lim _ {n \to \infty} b _ {n}.
$$

(b) The sequence $( a _ { n } b _ { n } ) _ { n = m } ^ { \infty }$ converges to xy; in other words, 

$$
\lim _ {n \to \infty} (a _ {n} b _ {n}) = (\lim _ {n \to \infty} a _ {n}) (\lim _ {n \to \infty} b _ {n}).
$$

(c) For any real number c, the sequence $( c a _ { n } ) _ { n = m } ^ { \infty }$ converges to cx; in other words, 

$$
\lim _ {n \to \infty} (c a _ {n}) = c \lim _ {n \to \infty} a _ {n}.
$$

(d) The sequence $( a _ { n } - b _ { n } ) _ { n = m } ^ { \infty }$ converges to $x - y ;$ in other words, 

$$
\lim _ {n \to \infty} (a _ {n} - b _ {n}) = \lim _ {n \to \infty} a _ {n} - \lim _ {n \to \infty} b _ {n}.
$$

(e) Suppose that $y \ne 0$ , and that $b _ { n } \neq 0$ for all $n \geq m$ . Then the sequence $( b _ { n } ^ { - 1 } ) _ { n = m } ^ { \infty }$ converges to $y ^ { - 1 }$ ; in other words, 

$$
\lim _ {n \to \infty} b _ {n} ^ {- 1} = (\lim _ {n \to \infty} b _ {n}) ^ {- 1}.
$$

(f) Suppose that $y \ne 0$ , and that $b _ { n } \neq 0$ for all $n \geq m$ . Then the sequence $( a _ { n } / b _ { n } ) _ { n = m } ^ { \infty }$ converges to $x / y ;$ in other words, 

$$
\lim _ {n \to \infty} \frac {a _ {n}}{b _ {n}} = \frac {\lim _ {n \to \infty} a _ {n}}{\lim _ {n \to \infty} b _ {n}}.
$$

(g) The sequence $( \operatorname* { m a x } ( a _ { n } , b _ { n } ) ) _ { n = m } ^ { \infty }$ converges to max $( x , y )$ ; in other words, 

$$
\lim _ {n \to \infty} \max (a _ {n}, b _ {n}) = \max (\lim _ {n \to \infty} a _ {n}, \lim _ {n \to \infty} b _ {n}).
$$

(h) The sequence $( \operatorname* { m i n } ( a _ { n } , b _ { n } ) ) _ { n = m } ^ { \infty }$ converges to min $( x , y )$ ; in other words, 

$$
\lim _ {n \to \infty} \min (a _ {n}, b _ {n}) = \min (\lim _ {n \to \infty} a _ {n}, \lim _ {n \to \infty} b _ {n}).
$$

Proof. See Exercise 6.1.8. 

## — Exercises —

Exercise 6.1.1. Let $( a _ { n } ) _ { n = 0 } ^ { \infty }$ be a sequence of real numbers, such that $a _ { n + 1 } > a _ { n }$ for each natural number n. Prove that whenever n and m are natural numbers such that $m > n ,$ , then we have $a _ { m } \ > \ a _ { n }$ . (We refer to these sequences as increasing sequences.) 

Exercise 6.1.2. Let $( a _ { n } ) _ { n = m } ^ { \infty }$ be a sequence of real numbers, and let L be a real number. Show that $( a _ { n } ) _ { n = m } ^ { \infty }$ converges to L if and only if, given any real $\varepsilon > 0$ , one can find an $N \geq m$ such that $| a _ { n } - L | \leq \varepsilon$ for all $n \geq N$ 

Exercise 6.1.3. Let $( a _ { n } ) _ { n = m } ^ { \infty }$ be a sequence of real numbers, let c be a real number, and let $m ^ { \prime } \geq m$ be an integer. Show that $( a _ { n } ) _ { n = m } ^ { \infty }$ converges to c if and only if $\left( a _ { n } \right) _ { n = m ^ { \prime } } ^ { \infty }$ converges to c. 

Exercise 6.1.4. Let $( a _ { n } ) _ { n = m } ^ { \infty }$ be a sequence of real numbers, let c be a real number, and let $k \geq 0$ be a non-negative integer. Show that $( a _ { n } ) _ { n = m } ^ { \infty }$ converges to c if and only if $( a _ { n + k } ) _ { n = m } ^ { \infty }$ converges to c. 

Exercise 6.1.5. Prove Proposition 6.1.12. (Hint: use the triangle inequality, or Proposition 4.3.7.) 

Exercise 6.1.6. Prove Proposition 6.1.15, using the following outline. Let $( a _ { n } ) _ { n = m } ^ { \infty }$ be a Cauchy sequence of rationals, and write $L : = L I M _ { n \to \infty } a _ { n }$ . We have to show that $( a _ { n } ) _ { n = m } ^ { \infty }$ converges to L. Let $\varepsilon > 0$ . Assume for sake of contradiction that sequence $a _ { n }$ is not eventually ε-close to L. Use this, and the fact that $( a _ { n } ) _ { n = m } ^ { \infty }$ is Cauchy, to show that there is an $N \geq m$ such that either $a _ { n } > L + \varepsilon / 2$ for all $n \geq N$ , or $a _ { n } < L - \varepsilon / 2$ for all $n \geq N$ . Then use Exercise 5.4.8. 

Exercise 6.1.7. Show that Definition 6.1.16 is consistent with Definition 5.1.12 (i.e., prove an analogue of Proposition 6.1.4 for bounded sequences instead of Cauchy sequences). 

Exercise 6.1.8. Prove Theorem 6.1.19. (Hint: you can use some parts of the theorem to prove others, e.g., (b) can be used to prove $( \mathrm { c } ) ; ( \mathrm { a } ) , ( \mathrm { c } )$ can be used to prove (d); and (b), (e) can be used to prove (f). The proofs are similar to those of Lemma 5.3.6, Proposition 5.3.10, and Lemma 5.3.15. For (e), you may need to first prove the auxiliary result that any sequence whose elements are non-zero, and which converges to a non-zero limit, is bounded away from zero.) 

Exercise 6.1.9. Explain why Theorem 6.1.19(f) fails when the limit of the denominator is 0. (To repair that problem requires L’Hˆopital’s rule, see Section 10.5.) 

Exercise 6.1.10. Show that the concept of equivalent Cauchy sequence, as defined in Definition 5.2.6, does not change if ε is required to be positive real instead of positive rational. More precisely, if $( a _ { n } ) _ { n = 0 } ^ { \infty }$ and $( b _ { n } ) _ { n = 0 } ^ { \infty }$ are sequences of reals, show that $( a _ { n } ) _ { n = 0 } ^ { \infty }$ and $( b _ { n } ) _ { n = 0 } ^ { \infty }$ are eventually ε-close for every rational $\varepsilon > 0$ if and only if they are eventually ε-close for every real $\varepsilon > 0$ . (Hint: modify the proof of Proposition 6.1.4.) 

## 6.2 The Extended real number system

There are some sequences which do not converge to any real number, but instead seem to be wanting to converge to + or . For instance, it seems intuitive that the sequence 

$$
1, 2, 3, 4, 5, \ldots
$$

should be converging to + , while 

$$
- 1, - 2, - 3, - 4, - 5, \ldots
$$

should be converging to . Meanwhile, the sequence 

$$
1, - 1, 1, - 1, 1, - 1, \ldots
$$

does not seem to be converging to anything (although we shall see later that it does have +1 and 1 as “limit points” - see below). Similarly the sequence 

$$
1, - 2, 3, - 4, 5, - 6, \ldots
$$

does not converge to any real number, and also does not appear to be converging to + or converging to $- \infty$ . To make this precise we need to talk about something called the extended real number system. 

Definition 6.2.1 (Extended real number system). The extended real number system $\mathbf { R } ^ { * }$ is the real line R with two additional elements attached, called + and . These elements are distinct from each other and also distinct from every real number. An extended real number x is called finite if it is a real number, and infinite if it is equal to + or $- \infty$ . (This definition is not directly related to the notion of finite and infinite sets in Section 3.6, though it is of course similar in spirit.) 

These new symbols, $+ \infty$ and $- \infty$ , at present do not have much meaning, since we have no operations to manipulate them (other than equality = and inequality $\neq )$ . Now we place a few operations on the extended real number system. 

Definition 6.2.2 (Negation of extended reals). The operation of negation $x \mapsto - x$ on R, we now extend to $\mathbf { R } ^ { * }$ by defining $- ( + \infty ) : = - \infty$ and $- ( - \infty ) : = + \infty$ 

Thus every extended real number x has a negation, and $- ( - x )$ is always equal to x. 

Definition 6.2.3 (Ordering of extended reals). Let x and y be extended real numbers. We say that $x \le y$ , i.e., x is less than or equal to y, if one of the following three statements is true: 

(a) x and y are real numbers, and $x \leq y$ as real numbers. 

(b) $y = + \infty .$ 

(c) $x = - \infty .$ 

We say that $x < y$ if we have $x \leq y$ and $x \neq y$ . We sometimes write $x < y$ as $y > x ,$ and $x \leq y$ as $y \geq x$ 

Examples 6.2.4. $3 \leq 5 , 3 < + \infty$ , and $- \infty < + \infty$ , but $3 \nleq - \infty .$ 

Some basic properties of order and negation on the extended real number system: 

Proposition 6.2.5. Let x, $y , \ z$ be extended real numbers. Then the following statements are true: 

(a) (Reflexivity) We have $x \leq x$ 

(b) (Trichotomy) Exactly one of the statements $x < y , x = y , o r x > y$ is true. 

(c) (Transitivity) If $x \leq y$ and $y \le z$ , then $x \le z$ 

(d) (Negation reverses order) $I f x \le y$ , then $- y \leq - x$ 

Proof. See Exercise 6.2.1. 

One could also introduce other operations on the extended real number system, such as addition, multiplication, etc. However, this is somewhat dangerous as these operations will almost certainly fail to obey the familiar rules of algebra. For instance, to define addition it seems reasonable (given one’s intuitive notion of infinity) to set $+ \infty + 5 = + \infty$ and $+ \infty + 3 = + \infty$ , but then this implies that $+ \infty + 5 = + \infty + 3$ , while $5 \neq 3$ . So things like the cancellation law begin to break down once we try to operate involving infinity. To avoid these issues we shall simply not define any arithmetic operations on the extended real number system other than negation and order. 

Remember that we defined the notion of supremum or least upper bound of a set E of reals; this gave an extended real number sup(E), which was either finite or infinite. We now extend this notion slightly. 

Definition 6.2.6 (Supremum of sets of extended reals). Let E be a subset of R∗. Then we define the supremum sup(E) or least upper bound of E by the following rule. 

(a) If E is contained in R (i.e., + and are not elements of E), then we let sup(E) be as defined in Definition 5.5.10. 

(b) If E contains + , then we set $\operatorname* { s u p } ( E ) : = + \infty .$ 

(c) If E does not contain + but does contain , then we set sup $( E ) : = \operatorname* { s u p } ( E \backslash \{ - \infty \} )$ (which is a subset of R and thus falls under case (a)). 

We also define the infimum inf(E) of E (also known as the greatest lower bound of E by the formula 

$$
\inf (E) := - \sup (- E)
$$

where $- E$ is the set $- E : = \{ - x : x \in E \}$ 

Example 6.2.7. Let E be the negative integers, together with : 

$$
E = \{- 1, - 2, - 3, - 4, \dots \} \cup \{- \infty \}.
$$

Then $\operatorname* { s u p } ( E ) = \operatorname* { s u p } ( E \backslash \{ - \infty \} ) = - 1$ , while 

$$
\inf (E) = - \sup (- E) = - (+ \infty) = - \infty .
$$

Example 6.2.8. The set $\{ 0 . 9 , 0 . 9 9 , 0 . 9 9 9 , 0 . 9 9 9 9 , \ldots \}$ has infimum 0.9 and supremum 1. Note that in this case the supremum does not actually belong to the set, but it is in some sense “touching $\mathrm { i t } ^ { \dag }$ from the right. 

Example 6.2.9. The set $\{ 1 , 2 , 3 , 4 , 5 \ldots \}$ has infimum 1 and supremum $+ \infty$ 

Example 6.2.10. Let E be the empty set. Then $\operatorname* { s u p } ( E ) = - \infty$ and inf $( E ) = + \infty \mathrm { ( w h y ? ) }$ . This is the only case in which the supremum can be less than the infimum $\mathrm { ( w h y ? ) }$ 

One can intuitively think of the supremum of E as follows. Imagine the real line with + somehow on the far right, and $- \infty$ on the far left. Imagine a piston at $+ \infty$ moving leftward until it is stopped by the presence of a set $E ;$ the location where it stops is the supremum of E. Similarly if one imagines a piston at $- \infty$ moving rightward until it is stopped by the presence of $E _ { i }$ , the location where it stops is the infimum of $E .$ . In the case when $E$ is the empty set, the pistons pass through each other, the supremum landing at $- \infty$ and the infimum landing at $+ \infty$ 

The following theorem justifies the terminology “least upper bound” and “greatest lower bound”: 

Theorem 6.2.11. Let $E$ be a subset of $\mathbf { R } ^ { * }$ . Then the following statements are true. 

(a) For every $x \in E$ we have $x \leq \operatorname* { s u p } ( E )$ and $x \geq \operatorname { i n f } ( E )$ 

(b) Suppose that $M \in \mathbf { R } ^ { * }$ is an upper bound for $E , i . e . , x \leq M$ for all $x \in E$ . Then we have $\operatorname* { s u p } ( E ) \leq M$ 

(c) Suppose that $M \in \mathbf { R } ^ { * }$ is a lower bound for $E , \ i . e . , x \geq M$ for all $x \in E$ . Then we have in $\operatorname { f } ( E ) \geq M$ 

Proof. See Exercise 6.2.2. 

$$
- \text { Exercises } -
$$

Exercise 6.2.1. Prove Proposition 6.2.5. (Hint: you may need Proposition $5 . 4 . 7 . )$ 

Exercise 6.2.2. Prove Theorem 6.2.11. (Hint: you may need to break into cases depending on whether $+ \infty \ \mathrm { o r \ - \infty }$ belongs to $E .$ . You can of course use Definition 5.5.10, provided that E consists only of real numbers.) 

## 6.3 Suprema and Infima of sequences

Having defined the notion of a supremum and infimum of sets of reals, we can now also talk about the supremum and infimum of sequences. 

Definition 6.3.1 (Sup and inf of sequences). Let $( a _ { n } ) _ { n = m } ^ { \infty }$ be a sequence of real numbers. Then we define s $\textstyle \operatorname { 1 p } ( a _ { n } ) _ { n = m } ^ { \infty }$ to be the supremum of the set $\{ a _ { n } : n \geq m \}$ , and inf $( a _ { n } ) _ { n = m } ^ { \infty }$ to the infimum of the same set $\{ a _ { n } : n \geq m \}$ 

Remark 6.3.2. The quantities $\operatorname* { s u p } ( a _ { n } ) _ { n = m } ^ { \infty }$ and inf $( a _ { n } ) _ { n = m } ^ { \infty }$ are sometimes written as $\operatorname* { s u p } _ { n \geq m } a _ { n }$ and $\operatorname { i n f } _ { n \geq m } a _ { n }$ respectively. 

Example 6.3.3. Let $\begin{array} { l c l } { a _ { n } } & { \mathrel { \mathop : } = } & { ( - 1 ) ^ { n } } \end{array}$ ; thus $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is the sequence $- 1 , 1 , - 1 , 1 , \ldots$ Then the set $\{ a _ { n } : n \geq 1 \}$ is just the two-element set $\{ - 1 , 1 \}$ , and hence sup $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is equal to 1. Similarly inf $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is equal to 1. 

Example 6.3.4. Let $\begin{array} { r c l } { a _ { n } } & { { : = } } & { { 1 / n ; } } \end{array}$ thus $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is the sequence $1 , 1 / 2 , 1 / 3 , \ldots$ Then the set $\{ a _ { n } ~ : ~ n ~ \geq ~ 1 \}$ is the countable set $\{ 1 , 1 / 2 , 1 / 3 , 1 / 4 , . . . \}$ . Thus $\operatorname* { s u p } ( a _ { n } ) _ { n = 1 } ^ { \infty } = 1$ and in $( a _ { n } ) _ { n = 1 } ^ { \infty } = 0$ (Exercise 6.3.1). Notice here that the infimum of the sequence is not actually a member of the sequence, though it becomes very close to the sequence eventually. (So it is a little inaccurate to think of the supremum and infimum as the “largest element of the sequence” and “smallest element of the sequence” respectively.) 

Example 6.3.5. Let $a _ { n } : = n \cdot$ ; thus $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is the sequence 1, 2, 3, 4, . . .. Then the set $\{ a _ { n } : n \geq 1 \}$ is just the positive integers $\{ 1 , 2 , 3 , 4 , \ldots \}$ Then sup $( a _ { n } ) _ { n = 1 } ^ { \infty } = + \infty$ and inf $( a _ { n } ) _ { n = 1 } ^ { \infty } = 1$ 

As the last example shows, it is possible for the supremum or infimum of a sequence to be $+ \infty \ \mathrm { o r \ - \infty }$ However, if a sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ is bounded, say bounded by M, then all the elements $a _ { n }$ of the sequence lie between M and M, so that the set $\{ a _ { n } : n \geq m \}$ has M as an upper bound and M as a lower bound. Since this set is clearly non-empty, we can thus conclude that the supremum and infimum of a bounded sequence are real numbers (i.e., not + and ). 

Proposition 6.3.6 (Least upper bound property). Let $( a _ { n } ) _ { n = m } ^ { \infty }$ be a sequence of real numbers, and let x be the extended real number $x : =$ sup $( a _ { n } ) _ { n = m } ^ { \infty }$ . Then we have $a _ { n } \ \leq \ x$ for all $n \geq m$ . Also, whenever $M \in \mathbf { R } ^ { * }$ is an upper bound for $a _ { n } ( i . e . , a _ { n } \leq M$ for all $n \geq m )$ , we have $x \leq M$ . Finally, for every extended real number y for which $y < x$ there exists at least one $n \geq m$ for which $y < a _ { n } \leq x$ 

Proof. See Exercise 6.3.2. 

Remark 6.3.7. There is a corresponding Proposition for infima, but with all the references to order reversed, e.g., all upper bounds should now be lower bounds, etc. The proof is exactly the same. 

Now we give an application of these concepts of supremum and infimum. In the previous section we saw that all convergent sequences are bounded. It is natural to ask whether the converse is true: are all bounded sequences convergent? The answer is no; for instance, the sequence $1 , - 1 , 1 , - 1 , . .$ . is bounded, but not Cauchy and hence not convergent. However, if we make the sequence both bounded and monotone (i.e., increasing or decreasing), then it is true that it must converge: 

Proposition 6.3.8 (Monotone bounded sequences converge). Let $( a _ { n } ) _ { n = m } ^ { \infty }$ be a sequence of real numbers which has some finite upper bound $M \in \mathbf { R }$ , and which is also increasing $( i . e . , \ a _ { n + 1 } \ \geq \ a _ { n }$ for all $n \geq m )$ Then $( a _ { n } ) _ { n = m } ^ { \infty }$ is convergent, and in fact 

$$
\lim _ {n \to \infty} a _ {n} = \sup (a _ {n}) _ {n = m} ^ {\infty} \leq M.
$$

Proof. See Exercise 6.3.3. 

One can similarly prove that if a sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ is bounded below and decreasing $( { \mathrm { i . e . , } } a _ { n + 1 } \leq a _ { n } )$ , then it is convergent, and that the limit is equal to the infimum. 

A sequence is said to be monotone if it is either increasing or decreasing. From Proposition 6.3.8 and Corollary 6.1.17 we see that a monotone sequence converges if and only if it is bounded. 

Example 6.3.9. The sequence 3, 3.1, 3.14, 3.141, 3.1415, . . . is increasing, and is bounded above by 4. Hence by Proposition 6.3.8 it must have a limit, which is a real number less than or equal to 4. 

Proposition 6.3.8 asserts that the limit of a monotone sequence exists, but does not directly say what that limit is. Nevertheless, with a little extra work one can often find the limit once one is given that the limit does exist. For instance: 

Proposition 6.3.10. Let $0 < x < 1$ . Then we have $\scriptstyle \operatorname* { l i m } _ { n \to \infty } x ^ { n } = 0$ 

Proof. Since $0 \textless x \textless 1$ , one can show that the sequence $( x ^ { n } ) _ { n = 1 } ^ { \infty }$ is decreasing (why?). On the other hand, the sequence $( x ^ { n } ) _ { n = 1 } ^ { \infty }$ has a lower bound of 0. Thus by Proposition 6.3.8 (for infima instead of suprema) the sequence $( x ^ { n } ) _ { n = 1 } ^ { \infty }$ converges to some limit L. Since $\boldsymbol { x } ^ { n + 1 } = \boldsymbol { x } \times \boldsymbol { x } ^ { n }$ , we thus see from the limit laws (Theorem 6.1.19) that $( x ^ { n + 1 } ) _ { n = 1 } ^ { \infty }$ converges to $x L$ . But the sequence $( x ^ { n + 1 } ) _ { n = 1 } ^ { \infty }$ is just the sequence $( x ^ { n } ) _ { n = 2 } ^ { \infty }$ shifted by one, and so they must have the same limits (why?). So $x L = L$ Since $x \neq 1$ , we can solve for L to obtain $L = 0$ . Thus $( x ^ { n } ) _ { n = 1 } ^ { \infty }$ converges to 0. □ 

Note that this proof does not work when $x > 1$ (Exercise 6.3.4). 

$$
- \text { Exercises } -
$$

Exercise 6.3.1. Verify the claim in Example 6.3.4. 

Exercise 6.3.2. Prove Proposition 6.3.6. (Hint: use Theorem 6.2.11.) 

Exercise 6.3.3. Prove Proposition 6.3.8. (Hint: use Proposition 6.3.6, together with the assumption that $a _ { n }$ is increasing, to show that $a _ { n }$ converges to sup $( a _ { n } ) _ { n = m } ^ { \infty } . )$ 

Exercise 6.3.4. Explain why Proposition 6.3.10 fails when $x > 1$ . In fact, show that the sequence $( x ^ { n } ) _ { n = 1 } ^ { \infty }$ diverges when $x > 1$ . (Hint: prove by contradiction and use the identity $( 1 / x ) ^ { n } x ^ { n } = 1$ and the limit laws in Theorem 6.1.19.) Compare this with the argument in Example 1.2.3; can you now explain the flaws in the reasoning in that example? 

## 6.4 Limsup, Liminf, and limit points

Consider the sequence 

$$
1. 1, - 1. 0 1, 1. 0 0 1, - 1. 0 0 0 1, 1. 0 0 0 0 1, \dots
$$

If one plots this sequence, then one sees (informally, of course) that this sequence does not converge; half the time the sequence is getting close to 1, and half the time the sequence is getting close to -1, but it is not converging to either of them; for instance, it never gets eventually 1/2-close to 1, and never gets eventually 1/2-close to -1. However, even though -1 and +1 are not quite limits of this sequence, it does seem that in some vague way they “want” to be limits. To make this notion precise we introduce the notion of a limit point. 

Definition 6.4.1 (Limit points). Let $( a _ { n } ) _ { n = m } ^ { \infty }$ be a sequence of real numbers, let x be a real number, and let $\varepsilon > 0$ be a real number. We say that x is ε-adherent to $( a _ { n } ) _ { n = m } ^ { \infty }$ if there exists an $n \geq m$ such that $a _ { n }$ is ε-close to x. We say that x is continually ε-adherent to $( a _ { n } ) _ { n = m } ^ { \infty }$ if it is ε-adherent to $( a _ { n } ) _ { n = N } ^ { \infty }$ for every $N \geq m$ . We say that x is a limit point or adherent point of $( a _ { n } ) _ { n = m } ^ { \infty }$ if it is continually ε-adherent to $( a _ { n } ) _ { n = m } ^ { \infty }$ for every $\varepsilon > 0$ 

Remark 6.4.2. The verb “to adhere” means much the same as “to stick $\mathrm { t o } ^ { \dag }$ ; hence the term “adhesive”. 

Unwrapping all the definitions, we see that x is a limit point of $( a _ { n } ) _ { n = m } ^ { \infty } { \mathrm { i f } } .$ , for every $\varepsilon > 0$ and every $N \geq m$ , there exists an $n \geq N$ such that $| a _ { n } - x | \leq \varepsilon .$ (Why is this the same definition?) Note the diference between a sequence being ε-close to $L$ (which means that all the elements of the sequence stay within a distance $\varepsilon$ of $L )$ and L being ε-adherent to the sequence (which only needs a single element of the sequence to stay within a distance $\varepsilon$ of $L )$ . Also, for L to be continually ε-adherent to $( a _ { n } ) _ { n = m } ^ { \infty }$ , it has to be ε-adherent to $( a _ { n } ) _ { n = N } ^ { \infty }$ for all $N \geq m$ , whereas for $( a _ { n } ) _ { n = m } ^ { \infty }$ to be eventually ε-close to L, we only need $( a _ { n } ) _ { n = N } ^ { \infty }$ to be ε-close to L for some $N \geq m$ . Thus there are some subtle diferences in quantifiers between limits and limit points. 

Note that limit points are only defined for finite real numbers. It is also possible to rigorously define the concept of $+ \infty \ \mathrm { o r \ - \infty }$ being a limit point; see Exercise 6.4.8. 

Example 6.4.3. Let $( a _ { n } ) _ { n = 1 } ^ { \infty }$ denote the sequence 

$$
\begin{array}{l} 0. 9, 0. 9 9, 0. 9 9 9, 0. 9 9 9 9, 0. 9 9 9 9 9, \dots . \end{array}
$$

The number 0.8 is 0.1-adherent to this sequence, since 0.8 is 0.1-close to 0.9, which is a member of this sequence. However, it is not continually 0.1-adherent to this sequence, since once one discards the first element of this sequence there is no member of the sequence to be 0.1-close to. In particular, 0.8 is not a limit point of this sequence. On the other hand, the number 1 is 0.1-adherent to this sequence, and in fact is continually 0.1-adherent to this sequence, since no matter how many initial members of the sequence one discards, there is still something for 1 to be 0.1-close to. In fact, it is continually ε-adherent for every ε, and is hence a limit point of this sequence. 

Example 6.4.4. Now consider the sequence 

$$
1. 1, - 1. 0 1, 1. 0 0 1, - 1. 0 0 0 1, 1. 0 0 0 0 1, \dots
$$

The number 1 is 0.1-adherent to this sequence; in fact it is continually 0.1-adherent to this sequence, because no matter how many elements of the sequence one discards, there are some elements of the sequence that 1 is 0.1-close to. (As discussed earlier, one does not need all the elements to be 0.1-close to 1, just some; thus 0.1-adherent is weaker than 0.1-close, and continually 0.1-adherent is a diferent notion from eventually 0.1- close.) In fact, for every $\varepsilon > 0$ , the number 1 is continually ε-adherent to this sequence, and is thus a limit point of this sequence. Similarly -1 is a limit point of this sequence; however 0 (say) is not a limit point of this sequence, since it is not continually 0.1-adherent to it. 

Limits are of course a special case of limit points: 

Proposition 6.4.5 (Limits are limit points). Let $( a _ { n } ) _ { n = m } ^ { \infty }$ be a sequence which converges to a real number c. Then c is a limit point of $( a _ { n } ) _ { n = m } ^ { \infty }$ and in fact it is the only limit point of $( a _ { n } ) _ { n = m } ^ { \infty }$ 

Proof. See Exercise 6.4.1. 

Now we will look at two special types of limit points: the limit superior (lim sup) and limit inferior (lim inf). 

Definition 6.4.6 (Limit superior and limit inferior). Suppose that $( a _ { n } ) _ { n = m } ^ { \infty }$ is a sequence. We define a new sequence $( a _ { N } ^ { + } ) _ { N = m } ^ { \infty }$ by the formula 

$$
a _ {N} ^ {+} := \sup (a _ {n}) _ {n = N} ^ {\infty}.
$$

More informally, $a _ { N } ^ { + }$ is the supremum of all the elements in the sequence from $a _ { N }$ onwards. We then define the limit superior of the sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ , denoted lim su ${ \mathrm { p } } _ { n  \infty } a _ { n }$ , by the formula 

$$
\limsup _ {n \to \infty} a _ {n} := \inf (a _ {N} ^ {+}) _ {N = m} ^ {\infty}.
$$

Similarly, we can define 

$$
a _ {N} ^ {-} := \inf (a _ {n}) _ {n = N} ^ {\infty}
$$

and define the limit inferior of the sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ , denoted lim in $\mathbf { f } _ { n  \infty } a _ { n }$ , by the formula 

$$
\liminf _ {n \to \infty} a _ {n} := \sup (a _ {N} ^ {-}) _ {N = m} ^ {\infty}.
$$

Example 6.4.7. Let $a _ { 1 } , a _ { 2 } , a _ { 3 } , . . .$ . denote the sequence 

$$
1. 1, - 1. 0 1, 1. 0 0 1, - 1. 0 0 0 1, 1. 0 0 0 0 1, \dots
$$

Then $a _ { 1 } ^ { + } , a _ { 2 } ^ { + } , a _ { 3 } ^ { + } , \ldots$ . is the sequence 

$$
1. 1, 1. 0 0 1, 1. 0 0 1, 1. 0 0 0 0 1, 1. 0 0 0 0 1, \dots
$$

(why?), and its infimum is 1. Hence the limit superior of this sequence is 1. Similarly, $a _ { 1 } ^ { - } , a _ { 2 } ^ { - } , a _ { 3 } ^ { - } , \ldots$ is the sequence 

$$
- 1. 0 1, - 1. 0 1, - 1. 0 0 0 1, - 1. 0 0 0 1, - 1. 0 0 0 0 0 1, \dots
$$

(why?), and the supremum of this sequence is 1. Hence the limit inferior of this sequence is 1. One should compare this with the supremum and infimum of the sequence, which are 1.1 and 1.01 respectively. 

Example 6.4.8. Let $a _ { 1 } , a _ { 2 } , a _ { 3 } , \dots$ . denote the sequence 

$$
1, - 2, 3, - 4, 5, - 6, 7, - 8, \ldots
$$

Then $a _ { 1 } ^ { + } , a _ { 2 } ^ { + } , \ldots$ is the sequence 

$$
+ \infty , + \infty , + \infty , + \infty , \dots
$$

(why?) and so the limit superior is + . Similarly, $a _ { 1 } ^ { - } , a _ { 2 } ^ { - } , \ldots$ . is the sequence 

$$
- \infty , - \infty , - \infty , - \infty , \dots
$$

and so the limit inferior is $- \infty$ 

Example 6.4.9. Let $a _ { 1 } , a _ { 2 } , a _ { 3 } , . . .$ . denote the sequence 

$$
1, - 1 / 2, 1 / 3, - 1 / 4, 1 / 5, - 1 / 6, \ldots
$$

Then $a _ { 1 } ^ { + } , a _ { 2 } ^ { + } , \ldots$ . is the sequence 

$$
1, 1 / 3, 1 / 3, 1 / 5, 1 / 5, 1 / 7, \dots
$$

which has an infimum of 0 (why?), so the limit superior is 0. Similarly, 

$a _ { 1 } ^ { - } , a _ { 2 } ^ { - } , \ldots$ is the sequence 

$$
- 1 / 2, - 1 / 2, - 1 / 4, - 1 / 4, - 1 / 6, - 1 / 6
$$

which has a supremum of 0. So the limit inferior is also 0. 

Example 6.4.10. Let $a _ { 1 } , a _ { 2 } , a _ { 3 } , \dots$ . denote the sequence 

$$
1, 2, 3, 4, 5, 6, \ldots
$$

Then $a _ { 1 } ^ { + } , a _ { 2 } ^ { + } , \ldots$ is the sequence 

$$
+ \infty , + \infty , + \infty , \dots
$$

so the limit superior is $+ \infty$ . Similarly, $a _ { 1 } ^ { - } , a _ { 2 } ^ { - } , \ldots .$ . is the sequence 

$$
1, 2, 3, 4, 5, \ldots
$$

which has a supremum of $+ \infty$ . So the limit inferior is also $+ \infty$ 

Remark 6.4.11. Some authors use the notation $\scriptstyle \operatorname* { l i m } _ { n \to \infty } a _ { n }$ instead of lim $\operatorname* { s u p } _ { n \to \infty } a _ { n }$ , and $\varinjlim _ { n \to \infty } a _ { n }$ instead of lim $\operatorname* { i n f } _ { n \to \infty } a _ { n }$ . Note that the starting index m of the sequence is irrelevant (see Exercise 6.4.2). 

Returning to the piston analogy, imagine a piston at $+ \infty$ moving leftward until it is stopped by the presence of the sequence $a _ { 1 } , a _ { 2 } , \dotsc$ The place it will stop is the supremum of $a _ { 1 } , a _ { 2 } , a _ { 3 } , . . . ,$ , which in our new notation is $a _ { 1 } ^ { + }$ . Now let us remove the first element $a _ { 1 }$ from the sequence; this may cause our piston to slip leftward, to a new point $a _ { 2 } ^ { + }$ (though in many cases the piston will not move and $a _ { 2 } ^ { + }$ will just be the same as $a _ { 1 } ^ { + } )$ . Then we remove the second element $a _ { 2 }$ , causing the piston to slip a little more. If we keep doing this the piston will keep slipping, but there will be some point where it cannot go any further, and this is the limit superior of the sequence. A similar analogy can describe the limit inferior of the sequence. 

We now describe some basic properties of limit superior and limit inferior. 

Proposition 6.4.12. Let $( a _ { n } ) _ { n = m } ^ { \infty }$ be a sequence of real numbers, let $L ^ { + }$ be the limit superior of this sequence, and let $L ^ { - }$ be the limit inferior of this sequence (thus both $L ^ { + }$ and $L ^ { - }$ are extended real numbers). 

(a) For every $x > L ^ { + }$ , there exists an $N \geq m$ such that $a _ { n } \ < \ x$ for all $n \geq N$ . (In other words, for every $x > L ^ { + }$ , the elements of the sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ are eventually less than x.) Similarly, for every $y < L ^ { - }$ there exists an $N \geq m$ such that $a _ { n } > y$ for all $n \geq N$ 

(b) For every $x < L ^ { + }$ , and every $N \geq m$ , there exists an $n \geq N$ such that $a _ { n } \ > \ x$ . (In other words, for every $x < L ^ { + }$ , the elements of the sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ exceed x infinitely often.) Similarly, for every $y > L ^ { - }$ and every $N \geq m$ , there exists an $n \geq N$ such that $a _ { n } < y$ 

(c) We have inf $\cdot ( a _ { n } ) _ { n = m } ^ { \infty } \leq L ^ { - } \leq L ^ { + } \leq \operatorname* { s u p } ( a _ { n } ) _ { n = m } ^ { \infty }$ 

(d) $\mathit { I f c }$ is any limit point of $( a _ { n } ) _ { n = m } ^ { \infty }$ , then we have $L ^ { - } \leq c \leq L ^ { + }$ 

(e) If $L ^ { + }$ is finite, then it is a limit point of $( a _ { n } ) _ { n = m } ^ { \infty }$ . Similarly, if $L ^ { - }$ is finite, then it is a limit point of $( a _ { n } ) _ { n = m } ^ { \infty }$ 

(f) Let c be a real number. $I f \ ( a _ { n } ) _ { n = m } ^ { \infty }$ converges to $^ { c , }$ then we must have $L ^ { + } = L ^ { - } = c$ . Conversely, if $L ^ { + } = L ^ { - } = c ,$ then $( a _ { n } ) _ { n = m } ^ { \infty }$ converges to c. 

Proof. We shall prove (a) and (b), and leave the remaining parts to the exercises. Suppose first that $x > L ^ { + }$ . Then by definition of $L ^ { + }$ , we have $x > \mathrm { i n f } ( a _ { N } ^ { + } ) _ { N = m } ^ { \infty }$ . By Proposition 6.3.6, there must then exist an integer $N \geq m$ such that $x > a _ { N } ^ { + }$ . By definition of $a _ { N } ^ { + }$ , this means that $x > \operatorname* { s u p } ( a _ { n } ) _ { n = N } ^ { \infty }$ . Thus by Proposition 6.3.6 again, we have $x > a _ { n }$ for all $n \geq N$ , as desired. This proves the first part of (a); the second part of (a) is proven similarly. 

Now we prove (b). Suppose that $x < L ^ { + }$ . Then we have $x \_ <$ inf $( a _ { N } ^ { + } ) _ { N = m } ^ { \infty }$ . If we fix any $N \geq m$ , then by Proposition 6.3.6, we thus have $x < a _ { N } ^ { + }$ . By definition of $a _ { N } ^ { + }$ , this means that $x < \operatorname* { s u p } ( a _ { n } ) _ { n = N } ^ { \infty }$ . By Proposition 6.3.6 again, there must thus exist $n \geq N$ such that $a _ { n } > x ,$ as desired. This proves the first part of (b), the second part of (b) is proven similarly. 

The proofs of $( \mathrm { c } ) , ( \mathrm { d } ) , ( \mathrm { e } ) , ( \mathrm { f } )$ are left to Exercise 6.4.3. 

Parts (c) and (d) of Proposition 6.4.12 say, in particular, that $L ^ { + }$ is the largest limit point of $( a _ { n } ) _ { n = m } ^ { \infty }$ , and $L ^ { - }$ is the smallest limit point (providing that $L ^ { + }$ and $L ^ { - }$ are finite. Proposition 6.4.12 (f) then says that if $L ^ { + }$ and $L ^ { - }$ coincide (so there is only one limit point), then the sequence in fact converges. This gives a way to test if a sequence converges: compute its limit superior and limit inferior, and see if they are equal. 

We now give a basic comparison property of limit superior and limit inferior. 

Lemma 6.4.13 (Comparison principle). Suppose that $( a _ { n } ) _ { n = m } ^ { \infty }$ and $( b _ { n } ) _ { n = m } ^ { \infty }$ are two sequences of real numbers such that $a _ { n } \leq b _ { n }$ for all $n \geq m$ . Then we have the inequalities 

$$
\sup (a _ {n}) _ {n = m} ^ {\infty} \leq \sup (b _ {n}) _ {n = m} ^ {\infty}
$$

$$
\inf (a _ {n}) _ {n = m} ^ {\infty} \leq \inf (b _ {n}) _ {n = m} ^ {\infty}
$$

$$
\limsup _ {n \to \infty} a _ {n} \leq \limsup _ {n \to \infty} b _ {n}
$$

$$
\liminf _ {n \to \infty} a _ {n} \leq \liminf _ {n \to \infty} b _ {n}
$$

Proof. See Exercise 6.4.4. 

Corollary 6.4.14 (Squeeze test). Let $( a _ { n } ) _ { n = m } ^ { \infty } , ( b _ { n } ) _ { n = m } ^ { \infty }$ , and $( c _ { n } ) _ { n = m } ^ { \infty }$ be sequences of real numbers such that 

$$
a _ {n} \leq b _ {n} \leq c _ {n}
$$

for all $n \geq m$ . Suppose also that $( a _ { n } ) _ { n = m } ^ { \infty }$ and $( c _ { n } ) _ { n = m } ^ { \infty }$ both converge to the same limit L. Then $( b _ { n } ) _ { n = m } ^ { \infty }$ is also convergent to L. 

Proof. See Exercise 6.4.5. 

Example 6.4.15. We already know (see Proposition 6.1.11) that $\mathrm { l i m } _ { n \to \infty } 1 / n = 0$ . By the limit laws (Theorem 6.1.19), this also implies that $\mathrm { l i m } _ { n  \infty } 2 / n = 0$ and $\scriptstyle \operatorname* { l i m } _ { n \to \infty } - 2 / n = 0$ . The squeeze test then shows that any sequence $( b _ { n } ) _ { n = 1 } ^ { \infty }$ for which 

$$
- 2 / n \leq b _ {n} \leq 2 / n \text { for   all } n \geq 1
$$

is convergent to 0. For instance, we can use this to show that the sequence $( - 1 ) ^ { n } / n + 1 / n ^ { 2 }$ converges to zero, or that 2−<sup>n</sup> converges to zero. Note one can use induction to show that $0 \leq 2 ^ { - n } \leq 1 / n$ for all $n \geq 1$ 

Remark 6.4.16. The squeeze test, combined with the limit laws and the principle that monotone bounded sequences always have limits, allows to compute a large number of limits. We give some examples in the next chapter. 

One commonly used consequence of the squeeze test is 

Corollary 6.4.17 (Zero test for sequences). Let $( a _ { n } ) _ { n = M } ^ { \infty }$ be a sequence of real numbers. Then the limit $\operatorname* { l i m } _ { n \to \infty } a _ { n }$ exists and is equal to zero if and only if the limit $\scriptstyle \operatorname* { l i m } _ { n \to \infty } \left| a _ { n } \right|$ exists and is equal to zero. 

Proof. See Exercise 6.4.7. 

We close this section with the following improvement to Proposition 6.1.12. 

Theorem 6.4.18 (Completeness of the reals). A sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ of real numbers is a Cauchy sequence if and only if it is convergent. 

Remark 6.4.19. Note that while this is very similar in spirit to Proposition 6.1.15, it is a bit more general, since Proposition 6.1.15 refers to Cauchy sequences of rationals instead of real numbers. 

Proof. Proposition 6.1.12 already tells us that every convergent sequence is Cauchy, so it sufices to show that every Cauchy sequence is convergent. 

Let $( a _ { n } ) _ { n = 1 } ^ { \infty }$ be a Cauchy sequence. We know from Lemma 5.1.15 (or more precisely, from the extension of this lemma to the real numbers, which is proven in exactly the same fashion) that the sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is bounded; by Lemma 6.4.13 (or Proposition 6.4.12(c)) this implies that $L ^ { - } : = \operatorname* { l i m } \operatorname* { i n f } _ { } n \to \infty { } a _ { n }$ and $L ^ { + } : = \operatorname* { l i m } \operatorname* { s u p } _ { n \to \infty } a _ { n }$ of the sequence are both finite. To show that the sequence converges, it will sufice by Proposition 6.4.12(f) to show that $L ^ { - } = L ^ { + }$ 

Now let $\varepsilon \ > \ 0$ be any real number. Since $( a _ { n } ) _ { n = 1 } ^ { \infty }$ is a Cauchy sequence, it must be eventually ε-steady, so in particular there exists an $N \geq 1$ such that the sequence $( a _ { n } ) _ { n = N } ^ { \infty }$ is ε-steady. In particular, we have $a _ { N } - \varepsilon \leq a _ { n } \leq a _ { N } + \varepsilon$ for all $n \geq N$ . By Proposition 6.3.6 (or Lemma 6.4.13) this implies that 

$$
a _ {N} - \varepsilon \leq \inf (a _ {n}) _ {n = N} ^ {\infty} \leq \sup (a _ {n}) _ {n = N} ^ {\infty} \leq a _ {N} + \varepsilon
$$

and hence by the definition of $L ^ { - }$ and $L ^ { + }$ (and Proposition 6.3.6 again) 

$$
a _ {N} - \varepsilon \leq L ^ {-} \leq L ^ {+} \leq a _ {N} + \varepsilon .
$$

Thus we have 

$$
0 \leq L ^ {+} - L ^ {-} \leq 2 \varepsilon .
$$

But this is true for all $\varepsilon > 0$ , and $L ^ { + }$ and $L ^ { - }$ do not depend on $\varepsilon ;$ so we must therefore have $L ^ { + } = L ^ { - } . ( \mathrm { I f } L ^ { + } > L ^ { - }$ then we could set $\varepsilon : = ( L ^ { + } - L ^ { - } ) / 3$ and obtain a contradiction.) By Proposition 6.4.12(f) we thus see that the sequence converges. □ 

Remark 6.4.20. In the language of metric spaces (see Chapter B.2), Theorem 6.4.18 asserts that the real numbers are a complete metric space - that they do not contain “holes” the same way the rationals do. (Certainly the rationals have lots of Cauchy sequences which do not converge to other rationals; take for instance the sequence 1, 1.4, 1.41, 1.414, 1.4142, . . . which converges to the irrational ${ \sqrt { 2 } } . )$ This property is closely related to the least upper bound property (Theorem 5.5.9), and is one of the principal characteristics which make the real numbers superior to the rational numbers for the purposes of doing analysis (taking limits, taking derivatives and integrals, finding zeroes of functions, that kind of thing), as we shall see in later chapters. 

— Exercises — 

Exercise 6.4.1. Prove Proposition 6.4.5. 

Exercise 6.4.2. State and prove analogues of Exercises 6.1.3 and 6.1.4 for limit points, limit superior, and limit inferior. 

Exercise 6.4.3. Prove parts (c),(d),(e),(f) of Proposition 6.4.12. (Hint: you can use earlier parts of the proposition to prove later ones.) 

Exercise 6.4.4. Prove Lemma 6.4.13. 

Exercise 6.4.5. Use Lemma 6.4.13 to prove Corollary 6.4.14. 

Exercise 6.4.6. Give an example of two bounded sequences $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ such that $a _ { n } < b _ { n }$ for all $n \geq 1$ , but that sup $( a _ { n } ) _ { n = 1 } ^ { \infty } \not \prec \operatorname { s u p } ( b _ { n } ) _ { n = 1 } ^ { \infty }$ . Explain why this does not contradict Lemma 6.4.13. 

Exercise 6.4.7. Prove Corollary 6.4.17. Is the corollary still true if we replace zero in the statement of this Corollary by some other number? 

Exercise 6.4.8. Let us say that a sequence $( a _ { n } ) _ { n = M } ^ { \infty }$ of real numbers has + as a limit point if it has no finite upper bound, and that it has as a limit point if it has no finite lower bound. With this definition, show that lim $\operatorname* { s u p } _ { n \to \infty } a _ { n }$ is a limit point of $( a _ { n } ) _ { n = M } ^ { \infty }$ , and furthermore that it is larger than all the other limit points of $( a _ { n } ) _ { n = M } ^ { \infty } ;$ in other words, the limit superior is the largest limit point of a sequence. Similarly, show that the limit inferior is the smallest limit point of a sequence. (One can use Proposition 6.4.12 in the course of the proof.) 

Exercise 6.4.9. Using the definition in Exercise 6.4.8, construct a sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ which has exactly three limit points, at , 0, and + . 

Exercise 6.4.10. Let $( a _ { n } ) _ { n = N } ^ { \infty }$ be a sequence of real numbers, and let $( b _ { m } ) _ { m = M } ^ { \infty }$ be another sequence of real numbers such that each $b _ { m }$ is a limit point of $( a _ { n } ) _ { n = N } ^ { \infty }$ . Let c be a limit point of $( b _ { m } ) _ { m = M } ^ { \infty }$ . Prove that c is also a limit point of $( a _ { n } ) _ { n = N } ^ { \infty }$ . (In other words, limit points of limit points are themselves limit points of the original sequence.) 

## 6.5 Some standard limits

Armed now with the limit laws and the squeeze test, we can now compute a large number of limits. 

A particularly simple limit is that of the constant sequence $c , c , c , c , \ldots ,$ we clearly have 

$$
\lim _ {n \to \infty} c = c
$$

for any constant $c \ \mathrm { ( w h y ? ) }$ 

Also, in Proposition 6.1.11, we proved that $\textstyle \operatorname* { l i m } _ { n \to \infty } 1 / n = 0$ . This now implies 

Corollary 6.5.1. We have $\scriptstyle \operatorname* { l i m } _ { n \to \infty } 1 / n ^ { 1 / k } = 0$ for every integer $k \geq 1$ 

Proof. From Lemma 5.6.6 we know that $1 / n ^ { 1 / k }$ is a decreasing function of $n ,$ while being bounded below by 0. By Proposition 6.3.8 (for decreasing sequences instead of increasing sequences) we thus know that this sequence converges to some limit $L \geq 0$ 

$$
L = \lim _ {n \to \infty} 1 / n ^ {1 / k}.
$$

Raising this to the $k ^ { t h }$ power and using the limit laws (or more precisely, Theorem 6.1.19(b) and induction), we obtain 

$$
L ^ {k} = \lim _ {n \to \infty} 1 / n.
$$

By Proposition 6.1.11 we thus have $L ^ { k } = 0 ;$ but this means that $L$ cannot be positive (else $L ^ { k }$ would be positive), so $L = 0$ , and we are done. □ 

Some other basic limits: 

Lemma 6.5.2. Let x be a real number. Then the limit $\scriptstyle \operatorname* { l i m } _ { n \to \infty } x ^ { n }$ exists and is equal to zero when $| x | < 1$ , exists and is equal to 1 when $x = 1$ , and diverges when $x = - 1$ or when $| x | > 1$ 

Proof. See Exercise 6.5.2. 

Lemma 6.5.3. For any $x > 0$ , we have $\scriptstyle \operatorname* { l i m } _ { n \to \infty } x ^ { 1 / n } = 1$ 

Proof. See Exercise 6.5.3. 

We will derive a few more standard limits later on, once we develop the root and ratio tests for series and for sequences. 

$$
- \text { Exercises } -
$$

Exercise 6.5.1. Show that $\textstyle \operatorname* { l i m } _ { n \to \infty } 1 / n ^ { q } = 0$ for any rational $q > 0$ . (Hint: use Corollary 6.5.1 and the limit laws, Theorem 6.1.19.) Conclude that the limit $\scriptstyle \operatorname* { l i m } _ { n \to \infty } n ^ { q }$ does not exist. (Hint: argue by contradiction using Theorem $6 . 1 . 1 9 ( \mathrm { e } ) . )$ 

Exercise 6.5.2. Prove Lemma 6.5.2. (Hint: use Proposition 6.3.10, Exercise 6.3.4, and the squeeze test.) 

Exercise 6.5.3. Prove Lemma 6.5.3. (Hint: you may need to treat the cases $x \ge 1$ and $x < 1$ separately. You might wish to first use Lemma 6.5.2 to prove the preliminary result that for every $\varepsilon > 0$ and every real number $M > 0$ , there exists an n such that $M ^ { 1 / n } \leq 1 + \bar { \varepsilon } . )$ 

## 6.6 Subsequences

This chapter has been devoted to the study of sequences $( a _ { n } ) _ { n = 1 } ^ { \infty }$ of real numbers, and their limits. Some sequences were convergent to a single limit, while others had multiple limit points. For instance, the sequence 

$$
1. 1, 0. 1, 1. 0 1, 0. 0 1, 1. 0 0 1, 0. 0 0 1, 1. 0 0 0 1, \dots
$$

has two limit points at 0 and 1 (which are incidentally also the lim inf and lim sup respectively), but is not actually convergent (since the lim sup and lim inf are not equal). However, while this sequence is not convergent, it does appear to contain convergent components; it seems to be a mixture of two convergent subsequences, namely 

$$
1. 1, 1. 0 1, 1. 0 0 1, \dots
$$

and 

$$
0. 1, 0. 0 1, 0. 0 0 1, \dots
$$

To make this notion more precise, we need a notion of subsequence. 

Definition 6.6.1 (Subsequences). Let $( a _ { n } ) _ { n = 0 } ^ { \infty }$ and $( b _ { n } ) _ { n = 0 } ^ { \infty }$ be sequences of real numbers. We say that $( b _ { n } ) _ { n = 0 } ^ { \infty }$ is a subsequence of $( a _ { n } ) _ { n = 0 } ^ { \infty }$ if there exists a function $f : \mathbf { N }  \mathbf { N }$ which is strictly increasing (i.e., $f ( n + 1 ) > f ( n )$ for all $n \in \mathbf { N } )$ such that 

$$
b _ {n} = a _ {f (n)} \text {   for   all   } n \in \mathbf {N}.
$$

Example 6.6.2. If $( a _ { n } ) _ { n = 0 } ^ { \infty }$ is a sequence, then $( a _ { 2 n } ) _ { n = 0 } ^ { \infty }$ is a subsequence of $( a _ { n } ) _ { n = 0 } ^ { \infty }$ , since the function $f : \mathbf { N }  \mathbf { N }$ defined by $f ( n ) : = 2 n$ is a strictly increasing function from N to N. Note that we do not assume f to be bijective, although it is necessarily injective (why?). More informally, the sequence 

$$
a _ {0}, a _ {2}, a _ {4}, a _ {6}, \ldots
$$

is a subsequence of 

$$
a _ {0}, a _ {1}, a _ {2}, a _ {3}, a _ {4}, \ldots .
$$

Example 6.6.3. The two sequences 

$$
1. 1, 1. 0 1, 1. 0 0 1, \ldots
$$

and 

$$
0. 1, 0. 0 1, 0. 0 0 1, \ldots
$$

mentioned earlier are both subsequences of 

$$
1. 1, 0. 1, 1. 0 1, 0. 0 1, 1. 0 0 1, 1. 0 0 0 1, \dots
$$

The property of being a subsequence is reflexive and transitive, though not symmetric: 

Lemma 6.6.4. Let $( a _ { n } ) _ { n = 0 } ^ { \infty } , ( b _ { n } ) _ { n = 0 } ^ { \infty }$ , and $( c _ { n } ) _ { n = 0 } ^ { \infty }$ be sequences of real numbers. Then $( a _ { n } ) _ { n = 0 } ^ { \infty }$ is a subsequence of $( a _ { n } ) _ { n = 0 } ^ { \infty }$ . Furthermore, if $( b _ { n } ) _ { n = 0 } ^ { \infty }$ is a subsequence of $( a _ { n } ) _ { n = 0 } ^ { \infty }$ , and $( c _ { n } ) _ { n = 0 } ^ { \infty }$ is a subsequence of $( b _ { n } ) _ { n = 0 } ^ { \infty }$ , then $( c _ { n } ) _ { n = 0 } ^ { \infty }$ is a subsequence of $( a _ { n } ) _ { n = 0 } ^ { \infty }$ 

Proof. See Exercise 6.6.1. 

We now relate the concept of subsequences to the concept of limits and limit points. 

Proposition 6.6.5 (Subsequences related to limits). Let $( a _ { n } ) _ { n = 0 } ^ { \infty }$ be a sequence of real numbers, and let L be a real number. Then the following two statements are logically equivalent (each one implies the other): 

(a) The sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ converges to L. 

(b) Every subsequence of $( a _ { n } ) _ { n = 0 } ^ { \infty }$ converges to $L$ . 

Proof. See Exercise 6.6.4. 

Proposition 6.6.6 (Subsequences related to limit points). Let $( a _ { n } ) _ { n = 0 } ^ { \infty }$ be a sequence of real numbers, and let L be a real number. Then the following two statements are logically equivalent. 

(a) L is a limit point of $( a _ { n } ) _ { n = 0 } ^ { \infty }$ 

(b) There exists a subsequence of $( a _ { n } ) _ { n = 0 } ^ { \infty }$ which converges to L. 

Proof. See Exercise 6.6.5. 

Remark 6.6.7. The above two propositions give a sharp contrast between the notion of a limit, and that of a limit point. When a sequence has a limit L, then all subsequences also converge to L. But when a sequence has L as a limit point, then only some subsequences converge to L. 

We can now prove an important theorem in real analysis, due to Bernard Bolzano (1781–1848) and Karl Weierstrass (1815–1897): every bounded sequence has a convergent subsequence. 

Theorem 6.6.8 (Bolzano-Weierstrass theorem). Let $( a _ { n } ) _ { n = 0 } ^ { \infty }$ be a bounded sequence (i.e., there exists a real number $M \ > \ 0$ such that $\left. a _ { n } \right. \leq$ M for all $n \in \mathbf { N } )$ Then there is at least one subsequence of $( a _ { n } ) _ { n = 0 } ^ { \infty }$ which converges. 

Proof. Let L be the limit superior of the sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ . Since we have $- M \leq a _ { n } \leq M$ for all natural numbers n, it follows from the comparison principle (Lemma 6.4.13) that $- M \leq L \leq M$ . In particular, L is a real number $( \mathrm { n o t + \infty ~ o r ~ } - \infty )$ . By Proposition 6.4.12(e), L is thus a limit point of $( a _ { n } ) _ { n = 0 } ^ { \infty }$ . Thus by Proposition 6.6.6, there exists a subsequence of $( a _ { n } ) _ { n = 0 } ^ { \infty }$ which converges (in fact, it converges to L). □ 

Note that we could as well have used the limit inferior instead of the limit superior in the above argument. 

Remark 6.6.9. The Bolzano-Weierstrass theorem says that if a sequence is bounded, then eventually it has no choice but to converge in some places; it has “no room” to spread out and stop itself from acquiring limit points. It is not true for unbounded sequences; for instance, the sequence 1, 2, 3, . . . has no convergent subsequences whatsoever (why?). In the language of topology, this means that the interval $\left\{ x \in \mathbf { R } : - M \leq x \leq M \right\}$ is compact, whereas an unbounded set such as the real line R is not compact. The distinction between compact sets and non-compact sets will be very important in later chapters - of similar importance to the distinction between finite sets and infinite sets. 

— Exercises — 

Exercise 6.6.1. Prove Lemma 6.6.4. 

Exercise 6.6.2. Can you find two sequences $( a _ { n } ) _ { n = 0 } ^ { \infty }$ and $( b _ { n } ) _ { n = 0 } ^ { \infty }$ which are not the same sequence, but such that each is a subsequence of the other? 

Exercise 6.6.3. Let $( a _ { n } ) _ { n = 0 } ^ { \infty }$ be a sequence which is not bounded. Show that there exists a subsequence $( b _ { n } ) _ { n = 0 } ^ { \infty }$ of $( a _ { n } ) _ { n = 0 } ^ { \infty }$ such that $\scriptstyle \operatorname* { l i m } _ { n \to \infty } 1 / \ b _ { n }$ exists and is equal to zero. (Hint: for each natural number $j .$ , recursively introduce the quantity $n _ { j } : = \mathrm { m i n } \{ n \in \mathbf { N } : | a _ { n } | \geq j ; n > n _ { j - 1 } \}$ (omitting the condition $n > n _ { j - 1 }$ when $j = 0 )$ , first explaining why the set $\left\{ n \in \mathbf { N } : | a _ { n } | \geq j ; n > n _ { j - 1 } \right\}$ is non-empty. Then set $b _ { j } : = a _ { n _ { j } } . )$ 

Exercise 6.6.4. Prove Proposition 6.6.5. (Note that one of the two implications has a very short proof.) 

Exercise 6.6.5. Prove Proposition 6.6.6. (Hint: to show that (a) implies (b), define the numbers $n _ { j }$ for each natural numbers j by the formula $n _ { j } : = \operatorname* { m i n } \{ n >$ $n _ { j - 1 } : | a _ { n } - L | \leq 1 / j \}$ , with the convention $n _ { 0 } : = 0$ , explaining why the set $\{ n > n _ { j - 1 } : | a _ { n } - L | \leq 1 / j \}$ is non-empty. Then consider the sequence $a _ { n _ { j } \cdot } )$ 

## 6.7 Real exponentiation, part II

We finally return to the topic of exponentiation of real numbers that we started in Section 5.6. In that section we defined $x ^ { q }$ for all rational q and positive real numbers x, but we have not yet defined $x ^ { \alpha }$ when α is real. We now rectify this situation using limits (in a similar way as to how we defined all the other standard operations on the real numbers). First, we need a lemma: 

Lemma 6.7.1 (Continuity of exponentiation). Let $x > 0$ , and let α be a real number. Let $( q _ { n } ) _ { n = 1 } ^ { \infty }$ be any sequence of rational numbers converging to α. Then $( x ^ { q _ { n } } ) _ { n = 1 } ^ { \infty }$ is also a convergent sequence. Furthermore, if $( q _ { n } ^ { \prime } ) _ { n = 1 } ^ { \infty }$ is any other sequence of rational numbers converging to α, then $( x ^ { q _ { n } ^ { \prime } } ) _ { n = 1 } ^ { \infty }$ has the same limit as $( x ^ { q _ { n } } ) _ { n = 1 } ^ { \infty }$ 

$$
\lim _ {n \to \infty} x ^ {q _ {n}} = \lim _ {n \to \infty} x ^ {q _ {n} ^ {\prime}}.
$$

Proof. There are three cases: $x < 1 , x = 1$ , and $x > 1$ . The case $x = 1$ is rather easy (because then $x ^ { q } = 1$ for all rational $q )$ . We shall just do the case $x > 1$ , and leave the case $x < 1$ (which is very similar) to the reader. 

Let us first prove that $( x ^ { q _ { n } } ) _ { n = 1 } ^ { \infty }$ converges. By Proposition 6.4.18 it is enough to show that $( x ^ { q _ { n } } ) _ { n = 1 } ^ { \infty }$ is a Cauchy sequence. 

To do this, we need to estimate the distance between $x ^ { q _ { n } }$ and $x ^ { q m }$ ; let us say for the time being that $q _ { n } \geq q _ { m }$ , so that $x ^ { q _ { n } } \geq x ^ { q _ { m } }$ (since $x > 1 )$ . We have 

$$
d (x ^ {q _ {n}}, x ^ {q _ {m}}) = x ^ {q _ {n}} - x ^ {q _ {m}} = x ^ {q _ {m}} \big (x ^ {q _ {n} - q _ {m}} - 1 \big).
$$

Since $( q _ { n } ) _ { n = 1 } ^ { \infty }$ is a convergent sequence, it has some upper bound M; since $x > 1$ , we have $x ^ { q _ { m } } \leq x ^ { M }$ . Thus 

$$
d \left(x ^ {q _ {n}}, x ^ {q _ {m}}\right) = \left| x ^ {q _ {n}} - x ^ {q _ {m}} \right| \leq x ^ {M} \left(x ^ {q _ {n} - q _ {m}} - 1\right).
$$

Now let $\varepsilon > 0$ . We know by Lemma 6.5.3 that the sequence $( x ^ { 1 / k } ) _ { k = 1 } ^ { \infty }$ is eventually εx−<sup>M</sup>-close to 1. Thus there exists some $K \geq 1$ such that 

$$
| x ^ {1 / K} - 1 | \leq \varepsilon x ^ {- M}.
$$

Now since $( q _ { n } ) _ { n = 1 } ^ { \infty }$ is convergent, it is a Cauchy sequence, and so there is an $N \geq 1$ such that $q _ { n }$ and $q _ { m }$ are $1 / K \mathrm { - c l o s e }$ for all $n , m \geq N$ . Thus we have 

$$
d (x ^ {q _ {n}}, x ^ {q _ {m}}) = x ^ {M} (x ^ {q _ {n} - q _ {m}} - 1) \leq x ^ {M} (x ^ {1 / K} - 1) \leq x ^ {M} \varepsilon x ^ {- M} = \varepsilon
$$

for every $n , m \geq N$ such that $q _ { n } \geq q _ { m }$ . By symmetry we also have this bound when $n , m \geq N$ and $q _ { n } \leq q _ { m }$ . Thus the sequence $( x ^ { q _ { n } } ) _ { n = N } ^ { \infty }$ is $\varepsilon -$ steady. Thus the sequence $( x ^ { q _ { n } } ) _ { n = 1 } ^ { \infty }$ is eventually ε-steady for every $\varepsilon >$ 0, and is thus a Cauchy sequence as desired. This proves the convergence of $( x ^ { q _ { n } } ) _ { n = 1 } ^ { \infty }$ 

Now we prove the second claim. It will sufice to show that 

$$
\lim _ {n \to \infty} x ^ {q _ {n} - q _ {n} ^ {\prime}} = 1,
$$

since the claim would then follow from limit laws (since $\begin{array} { r l } { x ^ { q n } } & { { } = } \end{array}$ $x ^ { q _ { n } - q _ { n } ^ { \prime } } x ^ { q _ { n } ^ { \prime } } )$ 

Write $r _ { n } : = q _ { n } - q _ { n } ^ { \prime }$ ; by limit laws we know that $( r _ { n } ) _ { n = 1 } ^ { \infty }$ converges to 0. We have to show that for every $\varepsilon > 0$ , the sequence $( x ^ { r _ { n } } ) _ { n = 1 } ^ { \infty }$ is eventually ε-close to 1. But from Lemma 6.5.3 we know that the sequence $( x ^ { 1 / k } ) _ { k = 1 } ^ { \infty }$ is eventually ε-close to 1. Since l $\scriptstyle \operatorname* { m } _ { k \to \infty } x ^ { - 1 / k }$ is also equal to 1 by Lemma 6.5.3, we know that $( x ^ { - 1 / k } ) _ { k = 1 } ^ { \infty }$ is also eventually ε-close to 1. Thus we can find a K such that $x ^ { 1 / K }$ and $x ^ { - 1 / K }$ are both $\varepsilon -$ close to 1. But since $( r _ { n } ) _ { n = 1 } ^ { \infty }$ is convergent to 0, it is eventually 1/K-close to 0, so that eventually $- 1 / K \le r _ { n } \le 1 / K$ , and thus $x ^ { - 1 / K } \leq x ^ { r _ { n } } \leq$ $x ^ { 1 / K }$ . In particular $x ^ { r _ { n } }$ is also eventually ε-close to 1 (see Proposition $4 . 3 . 7 ( \mathrm { f } ) )$ , as desired. □ 

We may now make the following definition. 

Definition 6.7.2 (Exponentiation to a real exponent). Let $x > 0$ be real, and let α be a real number. We define the quantity $x ^ { \alpha }$ by the formula $x ^ { \alpha } = \operatorname* { l i m } _ { n \to \infty } x ^ { q _ { n } }$ , where $( q _ { n } ) _ { n = 1 } ^ { \infty }$ is any sequence of rational numbers converging to α. 

Let us check that this definition is well-defined. First of all, given any real number α we always have at least one sequence $( q _ { n } ) _ { n = 1 } ^ { \infty }$ of rational numbers converging to α, by the definition of real numbers (and Proposition 6.1.15). Secondly, given any such sequence $( q _ { n } ) _ { n = 1 } ^ { \infty } .$ the limit $\scriptstyle \operatorname* { l i m } _ { n \to \infty } x ^ { q _ { n } }$ exists by Lemma 6.7.1. Finally, even though there can be multiple choices for the sequence $( q _ { n } ) _ { n = 1 } ^ { \infty }$ , they all give the same limit by Lemma 6.7.1. Thus this definition is well-defined. 

If α is not just real but rational, i.e., $\alpha = q$ for some rational $q ,$ then this definition could in principle be inconsistent with our earlier definition of exponentiation in Section $6 . 7 .$ . But in this case α is clearly the limit of the sequence $( q ) _ { n = 1 } ^ { \infty }$ , so by definition $x ^ { \alpha } = \operatorname* { l i m } _ { n \to \infty } x ^ { q } = x ^ { q }$ Thus the new definition of exponentiation is consistent with the old one. 

Proposition 6.7.3. All the results of Lemma 5.6.9, which held for rational numbers $q$ and r, continue to hold for real numbers q and $r _ { \cdot }$ 

Proof. We demonstrate this for the identity $x ^ { q + r } = x ^ { q } x ^ { r }$ (i.e., the first part of Lemma 5.6.9(b)); the other parts are similar and are left to Exercise 6.7.1. The idea is to start with Lemma 5.6.9 for rationals and then take limits to obtain the corresponding results for reals. 

Let q and r be real numbers. Then we can write $q = \operatorname* { l i m } _ { n \to \infty } q _ { n }$ and $r = \operatorname* { l i m } _ { n \to \infty } r _ { n }$ for some sequences $( q _ { n } ) _ { n = 1 } ^ { \infty }$ and $( r _ { n } ) _ { n = 1 } ^ { \infty }$ of rationals, by the definition of real numbers (and Proposition 6.1.15). Then by the limit laws, $q + r$ is the limit of $( q _ { n } + r _ { n } ) _ { n = 1 } ^ { \infty }$ . By definition of rea exponentiation, we have 

$$
x ^ {q + r} = \lim _ {n \to \infty} x ^ {q _ {n} + r _ {n}}; \quad x ^ {q} = \lim _ {n \to \infty} x ^ {q _ {n}}; \quad x ^ {r} = \lim _ {n \to \infty} x ^ {r _ {n}}.
$$

But by Lemma 5.6.9(b) (applied to rational exponents) we have $x ^ { q _ { n } + r _ { n } } = x ^ { q _ { n } } x ^ { r _ { n } }$ . Thus by limit laws we have $x ^ { q + r } = x ^ { q } x ^ { r }$ , as desired. □ 

$$
- \text { Exercises } -
$$

Exercise 6.7.1. Prove the remaining components of Proposition 6.7.3. 

## Chapter 7

Series 

Now that we have developed a reasonable theory of limits of sequences, we will use that theory to develop a theory of infinite series 

$$
\sum_ {n = m} ^ {\infty} a _ {n} = a _ {m} + a _ {m + 1} + a _ {m + 2} + \dots .
$$

But before we develop infinite series, we must first develop the theory of finite series. 

## 7.1 Finite series

Definition 7.1.1 (Finite series). Let m, n be integers, and let $( a _ { i } ) _ { i = m } ^ { n }$ be a finite sequence of real numbers, assigning a real number $a _ { i }$ to each integer i between m and n inclusive $( { \mathrm { i . e . , ~ } } m \leq i \leq n )$ . Then we define the finite sum (or finite series) $\textstyle \sum _ { i = m } ^ { n } a _ { i }$ by the recursive formula 

$$
\sum_ {i = m} ^ {n} a _ {i} := 0 \text { whenever } n <   m;
$$

$$
\sum_ {i = m} ^ {n + 1} a _ {i} := \left(\sum_ {i = m} ^ {n} a _ {i}\right) + a _ {n + 1} \text { whenever } n \geq m - 1.
$$

Thus for instance we have the identities 

$$
\sum_ {i = m} ^ {m - 2} a _ {i} = 0; \quad \sum_ {i = m} ^ {m - 1} a _ {i} = 0; \quad \sum_ {i = m} ^ {m} a _ {i} = a _ {m};
$$

$$
\sum_ {i = m} ^ {m + 1} a _ {i} = a _ {m} + a _ {m + 1}; \quad \sum_ {i = m} ^ {m + 2} a _ {i} = a _ {m} + a _ {m + 1} + a _ {m + 2}
$$

(why?). Because of this, we sometimes express $\textstyle \sum _ { i = m } ^ { n } a _ { i }$ less formally as 

$$
\sum_ {i = m} ^ {n} a _ {i} = a _ {m} + a _ {m + 1} + \ldots + a _ {n}.
$$

Remark 7.1.2. The diference between “sum” and “series” is a subtle linguistic one. Strictly speaking, a series is an expression of the form $\scriptstyle \sum _ { i = m } ^ { n } a _ { i } ;$ this series is mathematically (but not semantically) equal to a real number, which is then the sum of that series. For instance, $1 + 2 +$ $3 + 4 + 5$ is a series, whose sum is 15; if one were to be very picky about semantics, one would not consider 15 a series and one would not consider $1 + 2 + 3 + 4 + 5$ a sum, despite the two expressions having the same value. However, we will not be very careful about this distinction as it is purely linguistic and has no bearing on the mathematics; the expressions $1 + 2 + 3 + 4 + 5$ and 15 are the same number, and thus mathematically interchangeable, in the sense of the axiom of substitution (see Section A.7), even if they are not semantically interchangeable. 

Remark 7.1.3. Note that the variable i (sometimes called the index of summation) is a bound variable (sometimes called a dummy variable); the expression $\scriptstyle \sum _ { i = m } ^ { n } a _ { i }$ does not actually depend on any quantity named i. In particular, one can replace the index of summation i with any other symbol, and obtain the same sum: 

$$
\sum_ {i = m} ^ {n} a _ {i} = \sum_ {j = m} ^ {n} a _ {j}.
$$

We list some basic properties of summation below. 

## Lemma 7.1.4.

(a) Let $m \leq n < p$ be integers, and let $a _ { i }$ be a real number assigned to each integer $m \le i \le p$ . Then we have 

$$
\sum_ {i = m} ^ {n} a _ {i} + \sum_ {i = n + 1} ^ {p} a _ {i} = \sum_ {i = m} ^ {p} a _ {i}.
$$

(b) Let $m \leq n$ be integers, k be another integer, and let $a _ { i }$ be a real number assigned to each integer $m \leq i \leq n$ . Then we have 

$$
\sum_ {i = m} ^ {n} a _ {i} = \sum_ {j = m + k} ^ {n + k} a _ {j - k}.
$$

(c) Let $m \leq n$ be integers, and let $a _ { i } , b _ { i }$ be real numbers assigned to each integer $m \leq i \leq n$ . Then we have 

$$
\sum_ {i = m} ^ {n} (a _ {i} + b _ {i}) = \left(\sum_ {i = m} ^ {n} a _ {i}\right) + \left(\sum_ {i = m} ^ {n} b _ {i}\right).
$$

(d) Let m $\leq n$ be integers, and let $a _ { i }$ be a real number assigned to each integer $m \leq i \leq n$ , and let c be another real number. Then we have 

$$
\sum_ {i = m} ^ {n} (c a _ {i}) = c \left(\sum_ {i = m} ^ {n} a _ {i}\right).
$$

(e) (Triangle inequality for finite series) Let $m \leq n$ be integers, and let $a _ { i }$ be a real number assigned to each integer $m \leq i \leq n$ . Then we have 

$$
\left| \sum_ {i = m} ^ {n} a _ {i} \right| \leq \sum_ {i = m} ^ {n} | a _ {i} |.
$$

(f) (Comparison test for finite series) Let $m \leq n$ be integers, and let $a _ { i } , b _ { i }$ be real numbers assigned to each integer $m \leq i \leq n$ . Suppose that $a _ { i } \leq b _ { i }$ for all $m \leq i \leq n$ . Then we have 

$$
\sum_ {i = m} ^ {n} a _ {i} \leq \sum_ {i = m} ^ {n} b _ {i}.
$$

Proof. See Exercise 7.1.1. 

Remark 7.1.5. In the future we may omit some of the parentheses in series expressions, for instance we may write $\textstyle \sum _ { i = m } ^ { n } ( a _ { i } + b _ { i } )$ simply as $\textstyle \sum _ { i = m } ^ { n } a _ { i } + b _ { i }$ . This is reasonably safe from being mis-interpreted, because the alternative interpretation $\textstyle ( \sum _ { i = m } ^ { n } a _ { i } ) + b _ { i }$ does not make any sense (the index i in $b _ { i }$ is meaningless outside of the summation, since i is only a dummy variable). 

One can use finite series to also define summations over finite sets: 

Definition 7.1.6 (Summations over finite sets). Let X be a finite set with n elements (where $n \in \mathbf { N } )$ , and let $f : X  \mathbf { R }$ be a function from X to the real numbers (i.e., f assigns a real number $f ( x )$ to each element x of X). Then we can define the finite sum $\textstyle \sum _ { x \in X } f ( x )$ as follows. We first select any bijection g from $\{ i \in \mathbf { N } : 1 \leq i \leq n \}$ to X; such a bijection exists since X is assumed to have n elements. We then define 

$$
\sum_ {x \in X} f (x) := \sum_ {i = 1} ^ {n} f (g (i)).
$$

Example 7.1.7. Let X be the three-element set $X : = \{ a , b , c \}$ , where $a , b , c$ are distinct objects, and let $f : X  \mathbf { R }$ be the function $f ( a ) : = 2$ , $f ( b ) : = 5 , f ( c ) : = - 1$ . In order to compute the sum $\textstyle \sum _ { x \in X } f ( x )$ , we select a bijection $g : \{ 1 , 2 , 3 \}  X , { \mathrm { e . g . , ~ } } g ( 1 ) : = a , g ( 2 ) : = \bar { b } , g ( 3 ) : = c .$ We then have 

$$
\sum_ {x \in X} f (x) = \sum_ {i = 1} ^ {3} f (g (i)) = f (a) + f (b) + f (c) = 6.
$$

One could pick another bijection from $\{ 1 , 2 , 3 \}$ to $X , { \mathrm { ~ e . g . } } , h ( 1 ) : = c ,$ $h ( 2 ) : = b , h ( 3 ) = c .$ but the end result is still the same: 

$$
\sum_ {x \in X} f (x) = \sum_ {i = 1} ^ {3} f (h (i)) = f (c) + f (b) + f (a) = 6.
$$

To verify that this definition actually does give a single, well-defined value to $\textstyle \sum _ { x \in X } f ( x )$ , one has to check that diferent bijections g from $\{ i \in \mathbf { N } : 1 \leq \bar { i } \leq n \}$ to X give the same sum. In other words, we must prove 

Proposition 7.1.8 (Finite summations are well-defined). Let X be a finite set with n elements (where $n \in \mathbf { N } )$ , let $f : X  \mathbf { R }$ be a function, and let $g : \{ i \in \mathbf { N } : 1 \leq i \leq n \}  X$ and h : $\{ i \in \mathbf { N } : 1 \leq i \leq n \}  X$ be bijections. Then we have 

$$
\sum_ {i = 1} ^ {n} f (g (i)) = \sum_ {i = 1} ^ {n} f (h (i)).
$$

Remark 7.1.9. The issue is somewhat more complicated when summing over infinite sets; see Section 8.2. 

Proof. We use induction on n; more precisely, we let $P ( n )$ be the assertion that “For any set X of n elements, any function $f : X  \mathbf { R } .$ 7 and any two bijections g, h from $\{ i \in \mathbf { N } : 1 \leq i \leq n \}$ to X, we have $\begin{array} { r } { \sum _ { i = 1 } ^ { n } f ( g ( i ) ) = \sum _ { i = 1 } ^ { n } f ( h ( i ) ) ^ { \prime \prime } } \end{array}$ . (More informally, $P ( n )$ is the assertion that Proposition 7.1.8 is true for that value of $n . )$ We want to prove that $P ( n )$ is true for all natural numbers n. 

We first check the base case $P ( 0 )$ . In this case $\textstyle \sum _ { i = 1 } ^ { 0 } f ( g ( i ) )$ and $\textstyle \sum _ { i = 1 } ^ { 0 } f ( h ( i ) )$ both equal to 0, by definition of finite series, so we are done. 

Now suppose inductively that $P ( n )$ is true; we now prove that $P ( n +$ 1) is true. Thus, let X be a set with $n + 1$ elements, let $f : X  \mathbf { R }$ be a function, and let g and $h$ be bijections from $\{ i \in \mathbf { N } : 1 \leq i \leq n + 1 \}$ to X. We have to prove that 

$$
\sum_ {i = 1} ^ {n + 1} f (g (i)) = \sum_ {i = 1} ^ {n + 1} f (h (i)).\tag{7.1}
$$

Let $x : = g ( n + 1 )$ ; thus x is an element of X. By definition of finite series, we can expand the left-hand side of (7.1) as 

$$
\sum_ {i = 1} ^ {n + 1} f (g (i)) = \left(\sum_ {i = 1} ^ {n} f (g (i))\right) + f (x).
$$

Now let us look at the right-hand side of (7.1). Ideally we would like to have $h ( n + 1 )$ also equal to x - this would allow us to use the inductive hypothesis $P ( n )$ much more easily - but we cannot assume this. However, since h is a bijection, we do know that there is some index $j ,$ , with $1 \leq j \leq n + 1$ , for which $h ( j ) = x$ . We now use Lemma 7.1.4 and the definition of finite series to write 

$$
\begin{array}{l} \sum_ {i = 1} ^ {n + 1} f (h (i)) = \left(\sum_ {i = 1} ^ {j} f (h (i))\right) + \left(\sum_ {i = j + 1} ^ {n + 1} f (h (i))\right) \\ \qquad = \left(\sum_ {i = 1} ^ {j - 1} f (h (i))\right) + f (h (j)) + \left(\sum_ {i = j + 1} ^ {n + 1} f (h (i))\right) \\ \qquad = \left(\sum_ {i = 1} ^ {j - 1} f (h (i))\right) + f (x) + \left(\sum_ {i = j} ^ {n} f (h (i + 1))\right). \end{array}
$$

We now define the function $\tilde { h } : \{ i \in \mathbf { N } : 1 \leq i \leq n \}  X - \{ x \}$ by setting $\tilde { h } ( i ) : = h ( i )$ when $i < j$ and $\tilde { h } ( i ) : = h ( i + 1 )$ when $i \geq j$ . We can thus write the right-hand side of (7.1) as 

$$
= \left(\sum_ {i = 1} ^ {j - 1} f (\tilde {h} (i))\right) + f (x) + \left(\sum_ {i = j} ^ {n} f (\tilde {h} (i))\right) = \left(\sum_ {i = 1} ^ {n} f (\tilde {h} (i))\right) + f (x)
$$

where we have used Lemma 7.1.4 once again. Thus to finish the proof of (7.1) we have to show that 

$$
\sum_ {i = 1} ^ {n} f (g (i)) = \sum_ {i = 1} ^ {n} f (\tilde {h} (i)).\tag{7.2}
$$

But the function g (when restricted to $\{ i \in \mathbf { N } : 1 \leq i \leq n \} )$ is a bijection from $\{ i \in \mathbf { N } : 1 \leq i \leq n \} \to X - \{ x \} \ ( \mathrm { w h y ? } )$ . The function $\tilde { h }$ is also a bijection from $\{ i \in \mathbf { N } : 1 \leq i \leq n \}  X - \{ x \}$ (why? cf. Lemma 3.6.9). Since $X - \{ x \}$ has n elements (by Lemma 3.6.9), the claim 7.2 then follows directly from the induction hypothesis $P ( n )$ □ 

Remark 7.1.10. Suppose that X is a set, that $P ( x )$ is a property pertaining to an element x of X, and $f : \{ y \in X : P ( y )$ is $\operatorname { t r u e } \}  \mathbf { R }$ is a function. Then we will often abbreviate 

$$
\sum_ {x \in \{y \in X: P (y) \text {is true} \}} f (x)
$$

as $\textstyle \sum _ { x \in X : P ( x ) }$ is true $f ( x )$ or even as $\sum _ { P ( x ) }$ is true $f ( x )$ when there is no chance of confusion. For instance, $\textstyle \sum _ { n \in \mathbf { N } : 2 \leq n \leq 4 } f ( x ) { \mathrm { ~ o r ~ } } \sum _ { 2 \leq n \leq 4 } f ( x )$ is short-hand for $\begin{array} { r } { \sum _ { n \in \{ 2 , 3 , 4 \} } f ( x ) = f ( 2 ) + f ( \overline { { 3 } } ) + f ( 4 ) } \end{array}$ 

The following properties of summation on finite sets are fairly obvious, but do require a rigorous proof: 

Proposition 7.1.11 (Basic properties of summation over finite sets). 

(a) If X is empty, and $f : X  \mathbf { R }$ is a function $( i . e . , f$ is the empty function), we have 

$$
\sum_ {x \in X} f (x) = 0.
$$

(b) If X consists of a single element, $X = \{ x _ { 0 } \}$ , and $f : X  \mathbf { R }$ is a function, we have 

$$
\sum_ {x \in X} f (x) = f (x _ {0}).
$$

(c) (Substitution, part I) If X is a finite set, $f : X  \mathbf { R }$ is a function, and $g : Y  X$ is a bijection, then 

$$
\sum_ {x \in X} f (x) = \sum_ {y \in Y} f (g (y)).
$$

(d) (Substitution, part II) Let $n \leq$ m be integers, and let X be the set $X : = \{ i \in \mathbf { Z } : n \leq i \leq m \}$ . If $a _ { i }$ is a real number assigned to each integer $i \in X$ , then we have 

$$
\sum_ {i = n} ^ {m} a _ {i} = \sum_ {i \in X} a _ {i}.
$$

(e) Let X, Y be disjoint finite sets (so $X \cap Y = \emptyset )$ , and $f : X \cup Y  \mathbf { R }$ is a function. Then we have 

$$
\sum_ {z \in X \cup Y} f (z) = \left(\sum_ {x \in X} f (x)\right) + \left(\sum_ {y \in Y} f (y)\right).
$$

(f ) (Linearity, part I) Let X be a finite set, and let $f : X  \mathbf { R }$ and $g : X  \mathbf { R }$ be functions. Then 

$$
\sum_ {x \in X} (f (x) + g (x)) = \sum_ {x \in X} f (x) + \sum_ {x \in X} g (x).
$$

(g) (Linearity, part II) Let X be a finite set, let $f : X \to \mathbf { R }$ be a function, and let c be a real number. Then 

$$
\sum_ {x \in X} c f (x) = c \sum_ {x \in X} f (x).
$$

(h) (Monotonicity) Let X be a finite set, and let $f : X \to \mathbf { R }$ and $g : X  \mathbf { R }$ be functions such that $f ( x ) \leq g ( x )$ for all $x \in X$ Then we have 

$$
\sum_ {x \in X} f (x) \leq \sum_ {x \in X} g (x).
$$

(i) (Triangle inequality) Let X be a finite set, and let $f : X  \mathbf { R }$ be a function, then 

$$
| \sum_ {x \in X} f (x) | \leq \sum_ {x \in X} | f (x) |.
$$

Proof. See Exercise 7.1.2. 

Remark 7.1.12. The substitution rule in Proposition $7 . 1 . 1 1 ( \mathrm { c } )$ can be thought of as making the substitution $x : = g ( y )$ (hence the name). Note that the assumption that g is a bijection is essential; can you see why the rule will fail when g is not one-to-one or not onto? From Proposition 7.1.11(c) and (d) we see that 

$$
\sum_ {i = n} ^ {m} a _ {i} = \sum_ {i = n} ^ {m} a _ {f (i)}
$$

for any bijection f from the set $\{ i \in \mathbf { Z } : n \leq i \leq m \}$ to itself. Informally, this means that we can rearrange the elements of a finite sequence at will and still obtain the same value. 

Now we look at double finite series - finite series of finite series - and how they connect with Cartesian products. 

Lemma 7.1.13. Let $X , Y$ be finite sets, and let $f : X \times Y  \mathbf { R }$ be a function. Then 

$$
\sum_ {x \in X} \left(\sum_ {y \in Y} f (x, y)\right) = \sum_ {(x, y) \in X \times Y} f (x, y).
$$

Proof. Let n be the number of elements in X. We will use induction on n (cf. Proposition 7.1.8); i.e., we let $P ( n )$ be the assertion that Lemma 7.1.13 is true for any set X with n elements, and any finite set $Y$ and any function $f : X \times Y  \mathbf { R }$ . We wish to prove $P ( n )$ for all natural numbers n. 

The base case $P ( 0 )$ is easy, following from Proposition 7.1.11(a) $\mathrm { \left( w h y ? \right) }$ . Now suppose that $P ( n )$ is true; we now show that $P ( n + 1 )$ is true. Let X be a set with $n + 1$ elements. In particular, by Lemma 3.6.9, we can write $X = X ^ { \prime } \cup \{ x _ { 0 } \}$ , where $x _ { 0 }$ is an element of X and $X ^ { \prime } : = X - \{ x _ { 0 } \}$ has n elements. Then by Proposition 7.1.11(e) we have 

$$
\sum_ {x \in X} \left(\sum_ {y \in Y} f (x, y)\right) = (\sum_ {x \in X ^ {\prime}} \left(\sum_ {y \in Y} f (x, y))\right) + \left(\sum_ {y \in Y} f (x _ {0}, y)\right);
$$

by the induction hypothesis this is equal to 

$$
\sum_ {(x, y) \in X ^ {\prime} \times Y} f (x, y) + \left(\sum_ {y \in Y} f (x _ {0}, y)\right).
$$

By Proposition 7.1.11(c) this is equal to 

$$
\sum_ {(x, y) \in X ^ {\prime} \times Y} f (x, y) + \left(\sum_ {(x, y) \in \{x _ {0} \} \times Y} f (x, y)\right).
$$

By Proposition 7.1.11(e) this is equal to 

$$
\sum_ {(x, y) \in X \times Y} f (x, y)
$$

(why?) as desired. 

Corollary 7.1.14 (Fubini’s theorem for finite series). Let X, Y be finite sets, and let $f : X \times Y  \mathbf { R }$ be a function. Then 

$$
\begin{array}{c} \sum_ {x \in X} \left(\sum_ {y \in Y} f (x, y)\right) = \sum_ {(x, y) \in X \times Y} f (x, y) \\ = \sum_ {(y, x) \in Y \times X} f (x, y) \\ = \sum_ {y \in Y} \left(\sum_ {x \in X} f (x, y)\right). \end{array}
$$

Proof. In light of Lemma 7.1.13, it sufices to show that 

$$
\sum_ {(x, y) \in X \times Y} f (x, y) = \sum_ {(y, x) \in Y \times X} f (x, y).
$$

But this follows from Proposition 7.1.11(c) by applying the bijection $h : X \times Y \to Y \times X$ defined by $h ( x , y ) : = ( y , x )$ . (Why is this a bijection, and why does Proposition 7.1.11(c) give us what we want?) □ 

Remark 7.1.15. This should be contrasted with Example 1.2.5; thus we anticipate something interesting to happen when we move from finite sums to infinite sums. However, see Theorem 8.2.2. 

## — Exercises —

Exercise 7.1.1. Prove Lemma 7.1.4. (Hint: you will need to use induction, but the base case might not necessarily be at 0.) 

Exercise 7.1.2. Prove Proposition 7.1.11. (Hint: this is not as lengthy as it may first appear. It is largely a matter of choosing the right bijections to turn these sums over sets into finite series, and then applying Lemma 7.1.4.) 

Exercise 7.1.3. Form a definition for the finite products $\textstyle \prod _ { i = 1 } ^ { n } a _ { i }$ and $\textstyle \prod _ { x \in X } f ( x )$ . Which of the above results for finite series have analogues for finite products? (Note that it is dangerous to apply logarithms because some of the $a _ { i }$ or $f ( x )$ could be zero or negative. Besides, we haven’t defined logarithms yet.) 

Exercise 7.1.4. Define the factorial function n! for natural numbers n by the recursive definition $0 ! : = 1$ and $( n + 1 ) ! : = n ! \times ( n + 1 )$ . If x and y are real numbers, prove the binomial formula 

$$
(x + y) ^ {n} = \sum_ {j = 0} ^ {n} \frac {n !}{j ! (n - j) !} x ^ {j} y ^ {n - j}
$$

for all natural numbers n. (Hint: induct on n.) 

Exercise 7.1.5. Let X be a finite set, let m be an integer, and for each $x \in X$ let $( a _ { n } ( x ) ) _ { n = m } ^ { \infty }$ be a convergent sequence of real numbers. Show that the sequence $\textstyle ( \sum _ { x \in X } a _ { n } ( x ) ) _ { n = m } ^ { \infty }$ is convergent, and 

$$
\lim _ {n \to \infty} \sum_ {x \in X} a _ {n} (x) = \sum_ {x \in X} \lim _ {n \to \infty} a _ {n} (x).
$$

(Hint: induct on the cardinality of X, and use Theorem $6 . 1 . 1 9 ( \mathrm { a } ) . )$ Thus we may always interchange finite sums with convergent limits. Things however get trickier with infinite sums; see Exercise 11.47.11. 

## 7.2 Infinite series

We are now ready to sum infinite series. 

Definition 7.2.1 (Formal infinite series). A (formal) infinite series is any expression of the form 

$$
\sum_ {n = m} ^ {\infty} a _ {n},
$$

where m is an integer, and $a _ { n }$ is a real number for any integer $n \geq m$ We sometimes write this series as 

$$
a _ {m} + a _ {m + 1} + a _ {m + 2} + \dots .
$$

At present, this series is only defined formally; we have not set this sum equal to any real number; the notation $a _ { m } + a _ { m + 1 } + a _ { m + 2 } + . .$ . is of course designed to look very suggestively like a sum, but is not actually a finite sum because of the “. . .” symbol. To rigorously define what the series actually sums to, we need another definition. 

Definition 7.2.2 (Convergence of series). Let $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ be a formal infinite series. For any integer $N \geq m$ , we define the $N ^ { t h }$ partial sum $S _ { N }$ of this series to be $\begin{array} { r } { S _ { N } : = \sum _ { n = m } ^ { N } a _ { n } ; } \end{array}$ of course, $S _ { N }$ is a real number. If the sequence $( S _ { N } ) _ { N = m } ^ { \infty }$ converges to some limit L as $N  \infty$ , then we say that the infinite series $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ is convergent, and converges to $L ;$ we also write $\textstyle L = \sum _ { n = m } ^ { \infty } a _ { n }$ , and say that $L$ is the sum of the infinite series $\textstyle \sum _ { n = m } ^ { \infty } a _ { n } .$ . If the partial sums $S _ { N }$ diverge, then we say that the infinite series $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ is divergent, and we do not assign any real number value to that series. 

Remark 7.2.3. Note that Proposition 6.1.7 shows that if a series converges, then it has a unique sum, so it is safe to talk about the sum $\textstyle L = \sum _ { n = m } ^ { \infty } a _ { n }$ of a convergent series. 

Examples 7.2.4. Consider the formal infinite series 

$$
\sum_ {n = 1} ^ {\infty} 2 ^ {- n} = 2 ^ {- 1} + 2 ^ {- 2} + 2 ^ {- 3} + \dots .
$$

The partial sums can be verified to equal 

$$
S _ {N} = \sum_ {n = 1} ^ {N} 2 ^ {- n} = 1 - 2 ^ {- N}
$$

by an easy induction argument (or by Lemma 7.3.3 below); the sequence $1 - 2 ^ { - N }$ converges to 1 as $N  \infty .$ , and hence we have 

$$
\sum_ {n = 1} ^ {\infty} 2 ^ {- n} = 1.
$$

In particular, this series is convergent. On the other hand, if we consider the series 

$$
\sum_ {n = 1} ^ {\infty} 2 ^ {n} = 2 ^ {1} + 2 ^ {2} + 2 ^ {3} + \ldots
$$

then the partial sums are 

$$
S _ {N} = \sum_ {n = 1} ^ {N} 2 ^ {n} = 2 ^ {N + 1} - 2
$$

and this is easily shown to be an unbounded sequence, and hence divergent. Thus the series $\sum _ { n = 1 } ^ { \infty } 2 ^ { n }$ is divergent. 

Now we address the question of when a series converges. The following proposition shows that a series converges if the “tail” of the sequence is eventually less than ε for any $\varepsilon > 0$ 

Proposition 7.2.5. Let $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ be a formal series of real numbers. Then $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ converges if and only if, for every real number $\varepsilon > 0$ there exists an integer $N \geq m$ such that 

$$
\left| \sum_ {n = p} ^ {q} a _ {n} \right| \leq \varepsilon \text {   for   all   } p, q \geq N.
$$

Proof. See Exercise 7.2.2. 

This Proposition, by itself, is not very handy, because it is not so easy to compute the partial sums $\textstyle \sum _ { n = p } ^ { q } a _ { n }$ in practice. However, it has a number of useful corollaries. For instance: 

Corollary 7.2.6 (Zero test). Let $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ be a convergent series of real numbers. Then we must have $\scriptstyle \operatorname* { l i m } _ { n \to \infty } a _ { n } = 0$ . To put this another way, if $\operatorname* { l i m } _ { n \to \infty } a _ { n }$ is non-zero or divergent, then the series $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ is divergent. 

Proof. See Exercise 7.2.3. 

Example 7.2.7. The sequence $a _ { n } : = 1$ does not converge to 0 as $n $ $\infty ,$ so we know that $\textstyle \sum _ { n = 1 } ^ { \infty } 1$ is a divergent series. (Note however that 1, 1, 1, 1, . . . is a convergent sequence; convergence of series is a diferent notion from convergence of sequences.) Similarly, the sequence $a _ { n } : =$ $( - 1 ) ^ { n }$ diverges, and in particular does not converge to zero; thus the series $\scriptstyle \sum _ { n = 1 } ^ { \infty } ( - 1 ) ^ { n }$ is also divergent. 

If a sequence $( a _ { n } ) _ { n = m } ^ { \infty }$ does converge to zero, then the series $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ may or may not be convergent; it depends on the series. For instance, we will soon see that the series $\textstyle \sum _ { n = 1 } ^ { \infty } 1 / n$ is divergent despite the fact that $1 / n$ converges to 0 as $n \to \infty$ 

Definition 7.2.8 (Absolute convergence). Let $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ be a formal series of real numbers. We say that this series is absolutely convergent if the series $\textstyle \sum _ { n = m } ^ { \infty } \left| a _ { n } \right|$ is convergent. 

In order to distinguish convergence from absolute convergence, we sometimes refer to the former as conditional convergence. 

## 7.2. Infinite series

Proposition 7.2.9 (Absolute convergence test). Let $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ be a for-mal series of real numbers. If this series is absolutely convergent, then it is also conditionally convergent. Furthermore, in this case we have the triangle inequality 

$$
\left| \sum_ {n = m} ^ {\infty} a _ {n} \right| \leq \sum_ {n = m} ^ {\infty} | a _ {n} |.
$$

Proof. See Exercise 7.2.4. 

Remark 7.2.10. The converse to this proposition is not true; there exist series which are conditionally convergent but not absolutely convergent. See Example 7.2.13. 

Remark 7.2.11. We consider the class of conditionally convergent series to include the class of absolutely convergent series as a subclass. Thus when we say a statement such as $\stackrel { \ldots } { \sum } _ { n = m } ^ { \infty } a _ { n }$ is conditionally conver-gent”, this does not automatically mean that $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ is not absolutely convergent. If we wish to say that a series is conditionally convergent but not absolutely convergent, then we will instead use a phrasing such as $\stackrel { \ldots } { \sum } _ { n = m } ^ { \infty } a _ { n }$ is only conditionally convergent”, or $\stackrel { \ldots } { \sum } _ { n = m } ^ { \infty } a _ { n }$ converges conditionally, but not absolutely”. 

Proposition 7.2.12 (Alternating series test). Let $( a _ { n } ) _ { n = m } ^ { \infty }$ be a sequence of real numbers which are non-negative and decreasing, thus $a _ { n } \geq 0$ and $a _ { n } \geq a _ { n + 1 }$ for every $n \geq m$ . Then the series $\scriptstyle \sum _ { n = m } ^ { \infty } ( - 1 ) ^ { n } a _ { n }$ is convergent if and only if the sequence $a _ { n }$ converges to 0 as $n \to \infty$ 

Proof. From the zero test, we know that if $\scriptstyle \sum _ { n = m } ^ { \infty } ( - 1 ) ^ { n } a _ { n }$ is a convergent series, then the sequence $( - 1 ) ^ { n } a _ { n }$ converges to 0, which implies that $a _ { n }$ also converges to 0, since $( - 1 ) ^ { n } a _ { n }$ and $a _ { n }$ have the same distance from 0. 

Now suppose conversely that $a _ { n }$ converges to 0. For each N, let $S _ { N }$ be the partial sum $\begin{array} { r } { S _ { N } : = \sum _ { n = m } ^ { N } ( - 1 ) ^ { n } a _ { n } } \end{array}$ ; our job is to show that $S _ { N }$ converges. Observe that 

$$
\begin{array}{c} {S _ {N + 2} = S _ {N} + (- 1) ^ {N + 1} a _ {N + 1} + (- 1) ^ {N + 2} a _ {N + 2}} \\ {= S _ {N} + (- 1) ^ {N + 1} (a _ {N + 1} - a _ {N + 2}).} \end{array}
$$

But by hypothesis, $\left( a _ { N + 1 } - a _ { N + 2 } \right)$ is non-negative. Thus we have $S _ { N + 2 } \geq$ $S _ { N }$ when N is odd and $S _ { N + 2 } \le S _ { N }$ if N is even. 

Now suppose that N is even. From the above discussion and induction we see that $S _ { N + 2 k } ~ \le ~ S _ { N }$ for all natural numbers $k  { \mathrm { \ : \ : } } \left( \mathrm { w h y ? } \right)$ 

Also we have $S _ { N + 2 k + 1 } \geq S _ { N + 1 } = S _ { N } - a _ { N + 1 }$ (why?). Finally, we have $S _ { N + 2 k + 1 } = S _ { N + 2 k } - a _ { N + 2 k + 1 } \leq S _ { N + 2 k } { \mathrm { ~ ( w h y ? ) } }$ . Thus we have 

$$
S _ {N} - a _ {N + 1} \leq S _ {N + 2 k + 1} \leq S _ {N + 2 k} \leq S _ {N}
$$

for all k. In particular, we have 

$$
S _ {N} - a _ {N + 1} \leq S _ {n} \leq S _ {N} \text {   for   all   } n \geq N
$$

(why?). In particular, the sequence $S _ { n }$ is eventually $a _ { N + 1 } { \mathrm { - s t e a d y } }$ . But the sequence $a N$ converges to 0 as $N \to \infty$ , thus this implies that $S _ { n }$ is eventually ε-steady for every $\varepsilon > 0 \ \mathrm { ( w h y ? ) }$ . Thus $S _ { n }$ converges, and so the series $\scriptstyle \sum _ { n = m } ^ { \infty } ( - 1 ) ^ { n } a _ { n }$ is convergent. □ 

Example 7.2.13. The sequence $( 1 / n ) _ { n = 1 } ^ { \infty }$ is non-negative, decreasing, and converges to zero. Thus $\scriptstyle \sum _ { n = 1 } ^ { \infty } ( - 1 ) ^ { n } / n$ is convergent (but it is not absolutely convergent, because $\textstyle \sum _ { n = 1 } ^ { \infty } 1 / n$ diverges, see Corollary 7.3.7). Thus lack of absolute convergence does not imply lack of conditional convergence, even though absolute convergence implies conditional convergence. 

Some basic identities concerning convergent series are collected below. 

Proposition 7.2.14 (Series laws). 

(a) If $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ is a series of real numbers converging to $x ,$ , and $\scriptstyle \sum _ { n = m } ^ { \infty } b _ { n } i s$ a series of real numbers converging to $y ,$ , then $\scriptstyle \sum _ { n = m } ^ { \infty } ( a _ { n } + b _ { n } )$ is also a convergent series, and converges to $x + y$ In particular, we have 

$$
\sum_ {n = m} ^ {\infty} (a _ {n} + b _ {n}) = \sum_ {n = m} ^ {\infty} a _ {n} + \sum_ {n = m} ^ {\infty} b _ {n}.
$$

(b) $\textstyle I f \sum _ { n = m } ^ { \infty } a _ { n }$ is a series of real numbers converging to $x _ { i }$ , and $c$ is a real number, then $\scriptstyle \sum _ { n = m } ^ { \infty } ( c a _ { n } )$ is also a convergent series, and converges to cx. In particular, we have 

$$
\sum_ {n = m} ^ {\infty} (c a _ {n}) = c \sum_ {n = m} ^ {\infty} a _ {n}.
$$

## 7.2. Infinite series

(c) Let $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ be a series of real numbers, and let $k \geq 0$ be an integer. If one of the two series $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ and $\scriptstyle \sum _ { n = m + k } ^ { \infty } a _ { n }$ are  convergent, then the other one is also, and we have the identity 

$$
\sum_ {n = m} ^ {\infty} a _ {n} = \sum_ {n = m} ^ {m + k - 1} a _ {n} + \sum_ {n = m + k} ^ {\infty} a _ {n}.
$$

(d) Let $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ be a series of real numbers converging to $x ,$ and let k be an integer. Then $\scriptstyle \sum _ { n = m + k } ^ { \infty } a _ { n - k }$ also converges to x. 

Proof. See Exercise 7.2.5. 

From Proposition 7.2.14(c) we see that the convergence of a series does not depend on the first few elements of the series (though of course those elements do influence which value the series converges to). Because of this, we will usually not pay much attention as to what the initial index m of the series is. 

There is one type of series, called telescoping series, which are easy to sum: 

Lemma 7.2.15 (Telescoping series). Let $( a _ { n } ) _ { n = 0 } ^ { \infty }$ be a sequence of real numbers which converge to 0, i.e., $\operatorname* { l i m } _ { n \to \infty } a _ { n } \ = \ 0$ . Then the series $\scriptstyle \sum _ { n = 0 } ^ { \infty } ( a _ { n } - a _ { n + 1 } )$ converges to a . 

Proof. See Exercise 7.2.6. 

$$
- \text { Exercises } -
$$

Exercise 7.2.1. Is the series $\scriptstyle \sum _ { n = 1 } ^ { \infty } ( - 1 ) ^ { n }$ convergent or divergent? Justify your answer. Can you now resolve the dificulty in Example 1.2.2? 



Exercise 7.2.2. Prove Proposition 7.2.5. (Hint: use Proposition 6.1.12 and Theorem 6.4.18.) 



Exercise 7.2.3. Use Proposition 7.2.5 to prove Corollary 7.2.6. 

Exercise 7.2.4. Prove Proposition 7.2.9. (Hint: use Proposition 7.2.5 and Proposition 7.1.4(e).) 

Exercise 7.2.5. Prove Proposition 7.2.14. (Hint: use Theorem 6.1.19.) 

Exercise 7.2.6. Prove Lemma 7.2.15. (Hint: First work out what the partial sums $\scriptstyle \sum _ { n = 0 } ^ { N } ( a _ { n } - a _ { n + 1 } )$ should be, and prove your assertion using induction.) How does the proposition change if we assume that $a _ { n }$ does not converge to zero, but instead converges to some other real number L? 

## 7.3 Sums of non-negative numbers

Now we specialize the preceding discussion in order to consider sums $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ where all the terms $a _ { n }$ are non-negative. This situation comes up, for instance, from the absolute convergence test, since the absolute value $\left| a _ { n } \right|$ of a real number $a _ { n }$ is always non-negative. Note that when all the terms in a series are non-negative, there is no distinction between conditional convergence and absolute convergence. 

Suppose $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ is a series of non-negative numbers. Then the partial sums $\begin{array} { r } { S _ { N } : = \sum _ { n = m } ^ { N } a _ { n } } \end{array}$ are increasing, i.e., $S _ { N + 1 } \geq S _ { N }$ for all $N \ge m \ \mathrm { ( w h y ? ) }$ . From Proposition 6.3.8 and Corollary 6.1.17, we thus see that the sequence $( S _ { N } ) _ { n = m } ^ { \infty }$ is convergent if and only if it has an upper bound M. In other words, we have just shown 

Proposition 7.3.1. Let $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ be a formal series of non-negative real numbers. Then this series is convergent if and only if there is a real number M such that 

$$
\sum_ {n = m} ^ {N} a _ {n} \leq M \text { for all integers } N \geq m.
$$

A simple corollary of this is 

Corollary 7.3.2 (Comparison test). $L e t \sum _ { n = m } ^ { \infty } a _ { n }$ and $\textstyle \sum _ { n = m } ^ { \infty } b _ { n }$ be two formal series of real numbers, and suppose that $| a _ { n } | \leq b _ { n }$ for all $n \geq m$ Then $i f \sum _ { n = m } ^ { \infty } b _ { n }$ is convergent, then $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ is absolutely convergent, and in fact 

$$
\left| \sum_ {n = m} ^ {\infty} a _ {n} \right| \leq \sum_ {n = m} ^ {\infty} | a _ {n} | \leq \sum_ {n = m} ^ {\infty} b _ {n}.
$$

<sub>Proof. See Exercise 7.3.1.</sub> 

We can also run the comparison test in the contrapositive: if we have $| a _ { n } | \leq b _ { n }$ for all $n \geq m$ , and $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ is not absolutely convergent, then $\textstyle \sum _ { n = m } ^ { \infty } b _ { n }$ is not conditionally convergent. (Why does this follow immediately from Corollary 7.3.2?) 

A useful series to use in the comparison test is the geometric series 

$$
\sum_ {n = 0} ^ {\infty} x ^ {n},
$$

where x is some real number: 

Lemma 7.3.3 (Geometric series). Let x be a real number. $I f \left| x \right| \geq 1$ then the series $\scriptstyle \sum _ { n = 0 } ^ { \infty } x ^ { n }$ is divergent. If however $| x | < 1$ , then the series is absolutely convergent and 

$$
\sum_ {n = 0} ^ {\infty} x ^ {n} = 1 / (1 - x).
$$

Proof. See Exercise 7.3.2. 

We now give a useful criterion, known as the Cauchy criterion, to test whether a series of non-negative but decreasing terms is convergent. 

Proposition 7.3.4 (Cauchy criterion). Let $( a _ { n } ) _ { n = 1 } ^ { \infty }$ be a decreasing sequence of non-negative real numbers (so $a _ { n } \geq 0$ and $a _ { n + 1 } \leq a _ { n }$ for all $n \geq 1 )$ . Then the series $\textstyle \sum _ { n = 1 } ^ { \infty } a _ { n }$ is convergent if and only $i f$ the series 

$$
\sum_ {k = 0} ^ {\infty} 2 ^ {k} a _ {2 ^ {k}} = a _ {1} + 2 a _ {2} + 4 a _ {4} + 8 a _ {8} + \dots
$$

is convergent. 

Remark 7.3.5. An interesting feature of this criterion is that it only uses a small number of elements of the sequence $a _ { n }$ (namely, those elements whose index n is a power of 2, $n = 2 ^ { k } )$ in order to determine whether the whole series is convergent or not. 

Proof. Let $\begin{array} { r } { S _ { N } : = \sum _ { n = 1 } ^ { N } a _ { n } } \end{array}$ be the partial sums of $\textstyle \sum _ { n = 1 } ^ { \infty } a _ { n }$ , and let $\textstyle T _ { K } : = \sum _ { k = 0 } ^ { K } 2 ^ { k } a _ { 2 ^ { k } }$ be the partial sums of $\scriptstyle \sum _ { k = 0 } ^ { \infty } 2 ^ { k } a _ { 2 ^ { k } }$ . In light of Propo- sition 7.3.1, our task is to show that the sequence $( S _ { N } ) _ { N = 1 } ^ { \infty }$ is bounded if and only if the sequence $( T _ { K } ) _ { K = 0 } ^ { \infty }$ is bounded. To do this we need the following claim: 

Lemma 7.3.6. For any natural number K, we have $S _ { 2 ^ { K + 1 } - 1 } \leq T _ { K } \leq$ $2 S _ { 2 ^ { K } }$ 

Proof. We use induction on K. First we prove the claim when $K = 0$ i.e. 

$$
S _ {1} \leq T _ {0} \leq 2 S _ {1}.
$$

This becomes 

$$
a _ {1} \leq a _ {1} \leq 2 a _ {1}
$$

which is clearly true, since $a _ { 1 }$ is non-negative. 

Now suppose the claim has been proven for K, and now we try to prove it for $K + 1$ : 

$$
S _ {2 ^ {K + 2} - 1} \leq T _ {K + 1} \leq 2 S _ {2 ^ {K + 1}}.
$$

Clearly we have 

$$
T _ {K + 1} = T _ {K} + 2 ^ {K + 1} a _ {2 ^ {K + 1}}.
$$

Also, we have (using Lemma 7.1.4(a) and (f), and the hypothesis that the $a _ { n }$ are decreasing) 

$$
S _ {2 ^ {K + 1}} = S _ {2 ^ {K}} + \sum_ {n = 2 ^ {K} + 1} ^ {2 ^ {K + 1}} a _ {n} \geq S _ {2 ^ {K}} + \sum_ {n = 2 ^ {K} + 1} ^ {2 ^ {K + 1}} a _ {2 ^ {K + 1}} = S _ {2 ^ {K}} + 2 ^ {K} a _ {2 ^ {K + 1}}
$$

and hence 

$$
2 S _ {2 ^ {K + 1}} \geq 2 S _ {2 ^ {K}} + 2 ^ {K + 1} a _ {2 ^ {K + 1}}.
$$

Similarly we have 

$$
\begin{array}{l} S _ {2 ^ {K + 2} - 1} = S _ {2 ^ {K + 1} - 1} + \sum_ {n = 2 ^ {K + 1}} ^ {2 ^ {K + 2} - 1} a _ {n} \\ \leq S _ {2 ^ {K + 1} - 1} + \sum_ {n = 2 ^ {K + 1}} ^ {2 ^ {K + 2} - 1} a _ {2 ^ {K + 1}} \\ = S _ {2 ^ {K + 1} - 1} + 2 ^ {K + 1} a _ {2 ^ {K + 1}}. \end{array}
$$

Combining these inequalities with the induction hypothesis 

$$
S _ {2 ^ {K + 1} - 1} \leq T _ {K} \leq 2 S _ {2 ^ {K}}
$$

we obtain 

$$
S _ {2 ^ {K + 2} - 1} \leq T _ {K + 1} \leq 2 S _ {2 ^ {K + 1}}
$$

as desired. This proves the claim. 

From this claim we see that if $( S _ { N } ) _ { N = 1 } ^ { \infty }$ is bounded, then $( S _ { 2 ^ { K } } ) _ { K = 0 } ^ { \infty }$ is bounded, and hence $( T _ { K } ) _ { K = 0 } ^ { \infty }$ is bounded. Conversely, if $( T _ { K } ) _ { K = 0 } ^ { \infty }$ is bounded, then the claim implies that $S _ { 2 ^ { K + 1 } - 1 }$ is bounded, i.e., there is an M such that $S _ { 2 ^ { K + 1 } - 1 } \leq M$ for all natural numbers K. But one can easily show (using induction) that $2 ^ { K + 1 } - 1 \ge K + 1$ , and hence that $S _ { K + 1 } \leq M$ for all natural numbers K, hence $( S _ { N } ) _ { N = 1 } ^ { \infty }$ is bounded. 

Corollary 7.3.7. Let $q > 0$ be a rational number. Then the series $\textstyle \sum _ { n = 1 } ^ { \infty } 1 / n ^ { q }$ is convergent when $q > 1$ and divergent when $q \leq 1$ 

Proof. The sequence $( 1 / n ^ { q } ) _ { n = 1 } ^ { \infty }$ is non-negative and decreasing (by Lemma $5 . 6 . 9 ( \mathrm { d } ) )$ , and so the Cauchy criterion applies. Thus this series is convergent if and only if 

$$
\sum_ {k = 0} ^ {\infty} 2 ^ {k} \frac {1}{(2 ^ {k}) ^ {q}}
$$

is convergent. But by the laws of exponentiation (Lemma 5.6.9) we can rewrite this as the geometric series 

$$
\sum_ {k = 0} ^ {\infty} (2 ^ {1 - q}) ^ {k}.
$$

As mentioned earlier, the geometric series $\scriptstyle \sum _ { k = 0 } ^ { \infty } x ^ { k }$ converges if and only if $| x | < 1$ . Thus the series $\textstyle \sum _ { n = 1 } ^ { \infty } 1 / n ^ { q }$ will converge if and only if $| 2 ^ { 1 - q } | < 1$ , which happens if and only if $q > 1$ (why? Try proving it just using Lemma 5.6.9, and without using logarithms). □ 

In particular, the series $\textstyle \sum _ { n = 1 } ^ { \infty } 1 / n$ (also known as the harmonic se-ries) is divergent, as claimed earlier. However, the series $\textstyle \sum _ { n = 1 } ^ { \infty } 1 / n ^ { 2 }$ is convergent. 

Remark 7.3.8. The quantity $\textstyle \sum _ { n = 1 } ^ { \infty } 1 / n ^ { q }$ , when it converges, is called $\zeta ( q )$ , the Riemann-zeta function of q. This function is very important in number theory, and in particular in the distribution of the primes; there is a very famous unsolved problem regarding this function, called the Riemann hypothesis, but to discuss it further is far beyond the scope of this text. I will mention however that there is a US$ 1 million prize - and instant fame among all mathematicians - attached to the solution to this problem. 

— Exercises — 

Exercise 7.3.1. Use Proposition 7.3.1 to prove Corollary 7.3.2. 

Exercise 7.3.2. Prove Lemma 7.3.3. (Hint: for the first part, use the zero test. For the second part, first use induction to establish the geometric series formula 

$$
\sum_ {n = 0} ^ {N} x ^ {n} = (1 - x ^ {N + 1}) / (1 - x)
$$

and then apply Lemma 6.5.2.) 

Exercise 7.3.3. Let $\textstyle \sum _ { n = 0 } ^ { \infty } a _ { n }$ be an absolutely convergent series of real numbers such that $\scriptstyle \sum _ { n = 0 } ^ { \infty } \left| a _ { n } \right| = { \mathrm { 0 } }$ . Show that $a _ { n } = 0$ for every natural number n. 

## 7.4 Rearrangement of series

One feature of finite sums is that no matter how one rearranges the terms in a sequence, the total sum is the same. For instance, 

$$
a _ {1} + a _ {2} + a _ {3} + a _ {4} + a _ {5} = a _ {4} + a _ {3} + a _ {5} + a _ {1} + a _ {2}.
$$

A more rigorous statement of this, involving bijections, has already appeared earlier, see Remark 7.1.12. 

One can ask whether the same thing is true for infinite series. If all the terms are non-negative, the answer is yes: 

Proposition 7.4.1. Let $\textstyle \sum _ { n = 0 } ^ { \infty } a _ { n }$ be a convergent series of non-negative real numbers, and let f : N N be a bijection. Then $\textstyle \sum _ { m = 0 } ^ { \infty } a _ { f ( m ) }$ is also convergent, and has the same sum: 

$$
\sum_ {n = 0} ^ {\infty} a _ {n} = \sum_ {m = 0} ^ {\infty} a _ {f (m)}.
$$

Proof. We introduce the partial sums $\begin{array} { r } { S _ { N } \ : = \ \sum _ { n = 0 } ^ { N } a _ { n } } \end{array}$ and $T _ { M } : =$ $\scriptstyle \sum _ { m = 0 } ^ { M } a _ { f ( m ) }$ . We know that the sequences $( S _ { N } ) _ { n = 0 } ^ { \infty }$ and $( T _ { M } ) _ { m = 0 } ^ { \infty }$ are increasing. Write $L : = \operatorname* { s u p } ( S _ { N } ) _ { n = 0 } ^ { \infty }$ and $L ^ { \prime } : = \operatorname* { s u p } ( T _ { M } ) _ { m = 0 } ^ { \infty }$ . By Proposition 6.3.8 we know that L is finite, and in fact $\textstyle L = \sum _ { n = 0 } ^ { \infty } a _ { n }$ ; by Proposition 6.3.8 again we see that we will thus be done as soon as we can show that $L ^ { \prime } = L$ 

Fix M, and let Y be the set $Y : = \{ m \in \mathbf { N } : m \leq M \}$ . Note that f is a bijection between Y and f(Y). By Proposition 7.1.11, we have 

$$
T _ {M} = \sum_ {m = 0} ^ {M} a _ {f (m)} = \sum_ {m \in Y} a _ {f (m)} = \sum_ {n \in f (Y)} a _ {n}.
$$

The sequence $( f ( m ) ) _ { m = 0 } ^ { M }$ is finite, hence bounded, i.e., there exists an N such that $f ( m ) \leq N$ for all $m \leq N$ . In particular $f ( Y )$ is a subset of $\{ n \ \in \textbf { N } : \ n \ \leq \ N \}$ , and so by Proposition 7.1.11 again (and the assumption that all the $a _ { n }$ are non-negative) 

$$
T _ {M} = \sum_ {n \in f (Y)} a _ {n} \leq \sum_ {n \in \{n \in \mathbf {N}: n \leq N \}} a _ {n} = \sum_ {n = 0} ^ {N} a _ {n} = S _ {N}.
$$

But since $( S _ { N } ) _ { N = 0 } ^ { \infty }$ has a supremum of L, we thus see that $S _ { N } \ \leq \ L$ and hence that $T _ { M } \leq L$ for all M. Since $L ^ { \prime }$ is the least upper bound of $( T _ { M } ) _ { M = 0 } ^ { \infty }$ , this implies that $L ^ { \prime } \leq L$ 

A very similar argument (using the inverse $f ^ { - 1 }$ instead of $f )$ shows that every $S _ { N }$ is bounded above by $L ^ { \prime } { \mathrm { . } }$ , and hence $L \leq L ^ { \prime }$ . Combining these two inequalities we obtain $L = L ^ { \prime }$ , as desired. □ 

Example 7.4.2. From Corollary 7.3.7 we know that the series 

$$
\sum_ {n = 1} ^ {\infty} 1 / n ^ {2} = 1 + 1 / 4 + 1 / 9 + 1 / 1 6 + 1 / 2 5 + 1 / 3 6 + \dots
$$

is convergent. Thus, if we interchange every pair of terms, to obtain 

$$
1 / 4 + 1 + 1 / 1 6 + 1 / 9 + 1 / 3 6 + 1 / 2 5 + \dots
$$

we know that this series is also convergent, and has the same sum. (It turns out that the value of this sum is $\zeta ( 2 ) = \pi ^ { 2 } / 6$ , a fact which we shal prove in Exercise 11.32.2.) 

Now we ask what happens when the series is not non-negative. Then as long as the series is absolutely convergent, we can still do rearrangements: 

Proposition 7.4.3 (Rearrangement of series). Let $\textstyle \sum _ { n = 0 } ^ { \infty } a _ { n }$ be an $a b -$ solutely convergent series of real numbers, and let $f : \mathbf { N }  \mathbf { N }$ be a bijection. Then $\textstyle \sum _ { m = 0 } ^ { \infty } a _ { f ( m ) }$ is also absolutely convergent, and has the same sum: 

$$
\sum_ {n = 0} ^ {\infty} a _ {n} = \sum_ {m = 0} ^ {\infty} a _ {f (m)}.
$$

Proof. (Optional) We apply Proposition 7.4.1 to the infinite series $\textstyle \sum _ { n = 0 } ^ { \infty } | a _ { n } | .$ , which by hypothesis is a convergent series of non-negative numbers. If we write $\begin{array} { r } { L : = \sum _ { n = 0 } ^ { \infty } \left| a _ { n } \right| } \end{array}$ , then by Proposition 7.4.1 we know that $\scriptstyle \sum _ { m = 0 } ^ { \infty } | a _ { f ( m ) } |$ also converges to $L$ . 

Now write $\textstyle L ^ { \prime } : = \sum _ { n = 0 } ^ { \infty } a _ { n }$ . We have to show that $\scriptstyle \sum _ { m = 0 } ^ { \infty } a _ { f ( m ) }$ also converges to $L ^ { \prime }$ . In other words, given any $\varepsilon > 0$ , we have to find an M such that $\scriptstyle \sum _ { m = 0 } ^ { M ^ { \prime } } a _ { f ( m ) }$ is ε-close to $L ^ { \prime }$ for every $M ^ { \prime } \geq M$ 

Since $\textstyle \sum _ { n = 0 } ^ { \infty } \left| a _ { n } \right|$ is convergent, we can use Proposition 7.2.5 and find an $N _ { 1 }$ such that $\textstyle \sum _ { n = p } ^ { q } | a _ { n } | \leq \varepsilon / 2$ for all $p , q \ \geq \ N _ { 1 }$ . Since $\textstyle \sum _ { n = 0 } ^ { \infty } a _ { n }$ converges to $L ^ { \prime } ,$ the partial sums $\textstyle \sum _ { n = 0 } ^ { N } a _ { n }$ also converge to $L ^ { \prime }$ <sub>, and so</sub> there exists $N \geq N _ { 1 }$ such that $\textstyle \sum _ { n = 0 } ^ { N } a _ { n }$ is $\varepsilon / 2 \mathrm { - c l o s e }$ to $L ^ { \prime } .$ 

Now the sequence $( f ^ { - 1 } ( n ) ) _ { n = 0 } ^ { N }$ is finite, hence bounded, so there exists an $M$ such that $f ^ { - 1 } ( n ) \leq M$ for all $0 \leq n \leq N$ . In particular, for any $M ^ { \prime } \geq M$ , the set $\{ f ( m ) : m \in \mathbf { N } ; m \leq M ^ { \prime } \}$ contains $\{ n \in \mathbf { N } : n \leq$ $N \} \mathrm { { ( w h y ? ) } }$ . So by Proposition 7.1.11, for any $M ^ { \prime } \geq M$ 

$$
\sum_ {m = 0} ^ {M ^ {\prime}} a _ {f (m)} = \sum_ {n \in \{f (m): m \in \mathbf {N}; m \leq M ^ {\prime} \}} a _ {n} = \sum_ {n = 0} ^ {N} a _ {n} + \sum_ {n \in X} a _ {n}
$$

where X is the set 

$$
X = \{f (m): m \in \mathbf {N}; m \leq M ^ {\prime} \} \backslash \{n \in \mathbf {N}: n \leq N \}.
$$

The set X is finite, and is therefore bounded by some natural number $q ;$ we must therefore have 

$$
X \subseteq \{n \in \mathbf {N}: N + 1 \leq n \leq q \}
$$

(why?). Thus 

$$
\left| \sum_ {n \in X} a _ {n} \right| \leq \sum_ {n \in X} | a _ {n} | \leq \sum_ {n = N + 1} ^ {q} | a _ {n} | \leq \varepsilon / 2
$$

by our choice of N. Thus $\scriptstyle \sum _ { m = 0 } ^ { M ^ { \prime } } a _ { f ( m ) }$ is $\varepsilon / 2 \mathrm { - c l o s e }$ to $\textstyle \sum _ { n = 0 } ^ { N } a _ { n }$ , which as mentioned before is $\varepsilon / 2$ -close to $L ^ { \prime }$ . Thus $\scriptstyle \sum _ { m = 0 } ^ { M ^ { \prime } } a _ { f ( m ) }$ is ε-close to $L$ for all $M ^ { \prime } \geq M$ , as desired. □ 

Surprisingly, when the series is not absolutely convergent, then the rearrangements are very badly behaved. 

Example 7.4.4. Consider the series 

$$
1 / 3 - 1 / 4 + 1 / 5 - 1 / 6 + 1 / 7 - 1 / 8 + \dots
$$

This series is not absolutely convergent (why?), but is conditionally convergent by the alternating series test, and in fact the sum can be seen to converge to a positive number (in fact, it converges to $\ln ( 2 ) - 1 / 2 = 0 . 1 9 3 1 4 7 . . . ,$ see Example 11.25.7). Basically, the reason why the sum is positive is because the quantities $( 1 / 3 - 1 / 4 ) , ( 1 / 5 - 1 / 6 )$ 1 $( 1 / 7 - 1 / 8 )$ are all positive, which can then be used to show that every partial sum is positive. (Why? you have to break into two cases, depending on whether there are an even or odd number of terms in the partial sum.) 

If, however, we rearrange the series to have two negative terms to each positive term, thus 

$$
1 / 3 - 1 / 4 - 1 / 6 + 1 / 5 - 1 / 8 - 1 / 1 0 + 1 / 7 - 1 / 1 2 - 1 / 1 4 + \dots
$$

then the partial sums quickly become negative (this is because $( 1 / 3 -$ $1 / 4 - 1 / 6 ) , ( 1 / 5 - 1 / 8 - 1 / 9 )$ , and more generally $( 1 / ( 2 n + 1 ) - 1 / 4 n -$ $1 / ( 4 n + 2 ) )$ are all negative), and so this series converges to a negative quantity; in fact, it converges to 

$$
(\ln (2) - 1) / 2 = -. 1 5 3 4 2 6 \dots .
$$

There is in fact a surprising result of Riemann, which shows that a series which is conditionally convergent but not absolutely convergent can in fact be rearranged to converge to any value (or rearranged to diverge, in fact - see Exercise 8.2.6); see Theorem 8.2.8. 

To summarize, rearranging series is safe when the series is absolutely convergent, but is somewhat dangerous otherwise. (This is not to say that rearranging a series that is not absolutely convergent necessarily gives you the wrong answer - for instance, in theoretical physics one often performs similar maneuvres, and one still (usually) obtains a correct answer at the end - but doing so is risky, unless it is backed by a rigorous result such as Proposition 7.4.3.) 

$$
- \mathrm{Exercises} -
$$

Exercise 7.4.1. Let $\textstyle \sum _ { n = 0 } ^ { \infty } a _ { n }$ be an absolutely convergent series of real numbers. Let $f : \mathbf { N }  \mathbf { N }$ be an increasing function $( \mathrm { i . e . , } f ( n + 1 ) > f ( n )$ for all $n \in \mathbf { N } )$ Show that $\textstyle \sum _ { n = 0 } ^ { \infty } a _ { f ( n ) }$ is also an absolutely convergent series. (Hint: try to compare each partial sum of $\textstyle \sum _ { n = 0 } ^ { \infty } a _ { f ( n ) }$ with a (slightly diferent) partial sum of $\textstyle \sum _ { n = 0 } ^ { \infty } a _ { n } . )$ 

## 7.5 The root and ratio tests

Now we can state and prove the famous root and ratio tests for convergence. 

Theorem 7.5.1 (Root test). Let $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ be a series of real numbers, and let $\alpha : = \operatorname* { l i m } \operatorname* { s u p } _ { n \to \infty } | a _ { n } | ^ { 1 / n }$ 

(a) If $\alpha < 1$ , then the series $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ is absolutely convergent (and hence conditionally convergent). 

(b) If $\alpha > 1$ , then the series $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ is not conditionally convergent (and hence cannot be absolutely convergent either). 

(c) $I f \alpha = 1$ , we cannot assert any conclusion. 

Proof. First suppose that $\alpha \ < \ 1$ . Note that we must have $\alpha \geq 0$ since $| a _ { n } | ^ { 1 / n } \geq 0$ for every n. Then we can find an $\varepsilon > 0$ such that $0 < \alpha + \varepsilon < 1$ (for instance, we can set $\varepsilon : = ( 1 - \alpha ) / 2 )$ . By Proposition $6 . 4 . 1 2 ( \mathrm { a } )$ , there exists an $N \ge m$ such that $| a _ { n } | ^ { 1 / n } \leq \alpha + \varepsilon$ for all $n \geq N$ . In other words, we have $| a _ { n } | \leq ( \alpha + \varepsilon ) ^ { n }$ for all $n \geq N$ . But from the geometric series we have that $\scriptstyle \sum _ { n = N } ^ { \infty } ( \alpha + \varepsilon ) ^ { n }$ is absolutely convergent, since $0 < \alpha + \varepsilon < 1$ (note that the fact that we start from N is irrelevant by Proposition $7 . 2 . 1 4 ( \mathrm { c } ) )$ . Thus by the comparison test, we see that $\textstyle \sum _ { n = N } ^ { \infty } a _ { n }$ is absolutely convergent, and thus $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ is absolutely convergent, by Proposition $7 . 2 . 1 4 ( \mathrm { c } )$ again. 

Now suppose that $\alpha > 1$ . Then by Proposition 6.4.12(b), we see that for every $N \ge m$ there exists an $n \geq N$ such that $| a _ { n } | ^ { 1 / n } \geq 1$ and hence that $\left| a _ { n } \right| \geq 1$ . In particular, $( a _ { n } ) _ { n = N } ^ { \infty }$ is not 1-close to 0 for any N, and hence $( a _ { n } ) _ { n = m } ^ { \infty }$ is not eventually 1-close to 0. In particular, $( a _ { n } ) _ { n = m } ^ { \infty }$ does not converge to zero. Thus by the zero test, $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ is not conditionally convergent. 

For $\alpha = 1$ , see Exercise 7.5.3. 

The root test is phrased using the limit superior, but of course if $\scriptstyle \operatorname* { l i m } _ { n \to \infty } | a _ { n } | ^ { 1 / n }$ converges then the limit is the same as the limit superior. Thus one can phrase the root test using the limit instead of the limit superior, but only when the limit exists. 

The root test is sometimes dificult to use; however we can replace roots by ratios using the following lemma. 

Lemma 7.5.2. Let $( c _ { n } ) _ { n = m } ^ { \infty }$ be a sequence of positive numbers. Then we have 

$$
\liminf _ {n \to \infty} \frac {c _ {n + 1}}{c _ {n}} \leq \liminf _ {n \to \infty} c _ {n} ^ {1 / n} \leq \limsup _ {n \to \infty} c _ {n} ^ {1 / n} \leq \limsup _ {n \to \infty} \frac {c _ {n + 1}}{c _ {n}}.
$$

Proof. There are three inequalities to prove here. The middle inequality follows from Proposition $6 . 4 . 1 2 \mathrm { ( c ) }$ . We shall prove the last inequality, and leave the first one to Exercise 7.5.1. 

Write $\begin{array} { r } { L : = \operatorname* { l i m } \operatorname* { s u p } _ { n \to \infty } { \frac { c _ { n + 1 } } { c _ { n } } } } \end{array}$ . If $L = + \infty$ then there is nothing to prove (since $x \leq + \infty$ for every extended real number $x )$ , so we may assume that L is a finite real number. (Note that L cannot equal ; why?). Since $\textstyle { \frac { c _ { n + 1 } } { c _ { n } } }$ is always positive, we know that $L \geq 0$ 

Let $\varepsilon > 0 .$ By Proposition $6 . 4 . 1 2 ( \mathrm { a } )$ , we know that there exists an $N \geq m { \mathrm { ~ s u c h } }$ that $\begin{array} { r } { \frac { c _ { n + 1 } } { c _ { n } } \leq L + \varepsilon } \end{array}$ for all $n \geq N$ . This implies that $c _ { n + 1 } \leq c _ { n } ( L + \varepsilon )$ for all ${ \ddot { n } } \geq N$ . By induction this implies that 

$$
c _ {n} \leq c _ {N} (L + \varepsilon) ^ {n - N} \text { for   all } n \geq N
$$

(why?). If we write $A : = c _ { N } ( L + \varepsilon ) ^ { - N }$ , then we have 

$$
c _ {n} \leq A (L + \varepsilon) ^ {n}
$$

and thus 

$$
c _ {n} ^ {1 / n} \leq A ^ {1 / n} (L + \varepsilon)
$$

for all $n \geq N$ . But we have 

$$
\lim _ {n \to \infty} A ^ {1 / n} (L + \varepsilon) = L + \varepsilon
$$

by the limit laws (Theorem 6.1.19) and Lemma 6.5.3. Thus by the comparison principle (Lemma 6.4.13) we have 

$$
\limsup _ {n \to \infty} c _ {n} ^ {1 / n} \leq L + \varepsilon .
$$

But this is true for all $\varepsilon > 0$ , so this must imply that 

$$
\limsup _ {n \to \infty} c _ {n} ^ {1 / n} \leq L
$$

(why? prove by contradiction), as desired. 

□ 

From Theorem 7.5.1 and Lemma 7.5.2 (and Exercise 7.5.3) we have 

Corollary 7.5.3 (Ratio test). Let $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ be a series of non-zero numbers. (The non-zero hypothesis is required so that the ratios $\left| a _ { n + 1 } \right| / \left| a _ { n } \right|$ appearing below are well-defined.) 

If lim $\begin{array} { r } { \operatorname* { s u p } _ { n \to \infty } \frac { | a _ { n + 1 } | } { | a _ { n } | } < 1 } \end{array}$ , then the series $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ is absolutely convergent (hence conditionally convergent). 

If lim i $\begin{array} { r } { \mathrm { { l f } } _ { n \to \infty } { \frac { | a _ { n + 1 } | } { | a _ { n } | } } > 1 } \end{array}$ , then the series $\textstyle \sum _ { n = m } ^ { \infty } a _ { n }$ is not condi-tionally convergent (and thus cannot be absolutely convergent). 

In the remaining cases, we cannot assert any conclusion. 

Another consequence of Lemma 7.5.2 is the following limit: 

Proposition 7.5.4. We have $\textstyle \operatorname* { l i m } _ { n \to \infty } n ^ { 1 / n } = 1$ 

Proof. By Lemma 7.5.2 we have 

$$
\limsup _ {n \to \infty} n ^ {1 / n} \leq \limsup _ {n \to \infty} (n + 1) / n = \limsup _ {n \to \infty} 1 + 1 / n = 1
$$

by Proposition 6.1.11 and limit laws (Theorem 6.1.19). Similarly we have 

$$
\liminf _ {n \to \infty} n ^ {1 / n} \geq \liminf _ {n \to \infty} (n + 1) / n = \liminf _ {n \to \infty} 1 + 1 / n = 1.
$$

The claim then follows from Proposition 6.4.12(c) and (f). 

Remark 7.5.5. In addition to the ratio and root tests, another very useful convergence test is the integral test, which we will cover in Proposition 11.6.4. 

$$
- \text { Exercises } -
$$

Exercise 7.5.1. Prove the first inequality in Lemma 7.5.2. 

Exercise 7.5.2. Let x be a real number with $| x | < 1$ , and q be a real number. Show that the series $\textstyle \sum _ { n = 1 } ^ { \infty } n ^ { q } x ^ { n }$ is absolutely convergent, and that $\scriptstyle \operatorname* { l i m } _ { n \to \infty } n ^ { q } x ^ { n } = 0$ 

Exercise 7.5.3. Give an example of a divergent series $\textstyle \sum _ { n = 1 } ^ { \infty } a _ { n }$ of positive numbers $a _ { n }$ such that $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } a _ { n + 1 } / a _ { n } \ = \ \operatorname* { l i m } _ { n \to \infty } a _ { n } ^ { 1 / n } \ = \ 1 } \end{array}$ , and give an example of a convergent series $\textstyle \sum _ { n = 1 } ^ { \infty } b _ { n }$ of positive numbers $b _ { n }$ such that $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } b _ { n + 1 } / b _ { n } = \operatorname* { l i m } _ { n \to \infty } b _ { n } ^ { 1 / n } = 1 } \end{array}$ . (Hint: use Corollary 7.3.7.) This shows that the ratio and root tests can be inconclusive even when the summands are positive and all the limits converge. 

## Chapter 8

## Infinite sets

We now return to the study of set theory, and specifically to the study of cardinality of sets which are infinite (i.e., sets which do not have cardinality n for any natural number n), a topic which was initiated in Section 3.6. 

## 8.1 Countability

From Proposition 3.6.14(c) we know that if X is a finite set, and Y is a proper subset of X, then Y does not have equal cardinality with X. However, this is not the case for infinite sets. For instance, from Theorem 3.6.12 we know that the set N of natural numbers is infinite. The set N 0 is also infinite, thanks to Proposition 3.6.14(a) (why?), and is a proper subset of N. However, the set N 0 , despite being “smaller” than N, still has the same cardinality as N, because the function f : $\mathbf { N }  \mathbf { N } - \{ 0 \}$ defined by $f ( n ) : = n + 1$ , is a bijection from N to N 0 . (Why?) This is one characteristic of infinite sets; see Exercise 8.1.1. 

We now distinguish two types of infinite sets: the countable sets and the uncountable sets. 

Definition 8.1.1 (Countable sets). A set X is said to be countably infinite (or just countable) if it has equal cardinality with the natural numbers N. A set X is said to be at most countable if it is either countable or finite. We say that a set is uncountable if it is infinite but not countable. 

Remark 8.1.2. Countably infinite sets are also called denumerable sets. 

Examples 8.1.3. From the preceding discussion we see that N is countable, and so is N 0 . Another example of a countable set is the even natural numbers $\{ 2 n : n \in \mathbf { N } \}$ , since the function $f ( n ) : = 2 n$ provides a bijection between N and the even natural numbers $\mathrm { ( w h y ? ) }$ 

Let X be a countable set. Then, by definition, we know that there exists a bijection $f : \mathbf { N }  X$ . Thus, every element of X can be written in the form $f ( n )$ for exactly one natural number n. Informally, we thus have 

$$
X = \{f (0), f (1), f (2), f (3), \dots \}.
$$

Thus, a countable set can be arranged in a sequence, so that we have a zeroth element $f ( 0 )$ , followed by a first element $f ( 1 )$ , then a second element $f ( 2 )$ , and so forth, in such a way that all these elements $f ( 0 ) , f ( 1 ) , f ( 2 ) , . . .$ . are all distinct, and together they fill out all of X. (This is why these sets are called countable; because we can literally count them one by one, starting from $f ( 0 )$ , then $f ( 1 )$ , and so forth.) 

Viewed in this way, it is clear why the natural numbers 

$$
\mathbf {N} = \{0, 1, 2, 3, \dots \},
$$

the positive integers 

$$
\mathbf {N} - \{0 \} = \{1, 2, 3, \ldots \},
$$

and the even natural numbers 

$$
\{0, 2, 4, 6, 8, \ldots \}
$$

are countable. However, it is not as obvious whether the integers 

$$
\mathbf {Z} = \{\dots , - 3, - 2, - 1, 0, 1, 2, 3, \dots \}
$$

or the rationals 

$$
\mathbf {Q} = \{0, 1 / 4, - 2 / 3, \dots \}
$$

or the reals 

$$
\mathbf {R} = \{0, \sqrt {2}, - \pi , 2. 5, \ldots \}
$$

are countable or not; for instance, it is not yet clear whether we can arrange the real numbers in a sequence $f ( 0 ) , f ( 1 ) , f ( 2 ) , . . . .$ We will answer these questions shortly. 

From Proposition 3.6.4 and Theorem 3.6.12, we know that countable sets are infinite; however it is not so clear whether all infinite sets are countable. Again, we will answer those questions shortly. We first need the following important principle. 

## 8.1. Countability

Proposition 8.1.4 (Well ordering principle). Let X be a non-empty subset of the natural numbers N. Then there exists exactly one element $n \in X$ such that $n \leq m$ for all $m \in X$ . In other words, every non-empty set of natural numbers has a minimum element. 

Proof. See Exercise 8.1.2. 

We will refer to the element n given by the well-ordering principle as the minimum of X, and write it as min(X). Thus for instance the minimum of the set $\{ 2 , 4 , 6 , 8 , \ldots \}$ is 2. This minimum is clearly the same as the infimum of X, as defined in Definition 5.5.10 (why?). 

Proposition 8.1.5. Let X be an infinite subset of the natural numbers N. Then there exists a unique bijection $f : \mathbf { N }  X$ which is increasing, in the sense that $f ( n + 1 ) > f ( n )$ for all $n \in \mathbf N$ . In particular, X has equal cardinality with N and is hence countable. 

Proof. We will give an incomplete sketch of the proof, with some gaps marked by a question mark (?); these gaps will be filled in Exercise 8.1.3. 

We now define a sequence $a _ { 0 } , a _ { 1 } , a _ { 2 } , \dotsc$ of natural numbers recursively by the formula 

$$
a _ {n} := \min \{x \in X: x \neq a _ {m} \text {   for   all   } m <   n \}.
$$

Intuitively speaking, $a _ { 0 }$ is the smallest element of $X ; ~ a _ { 1 }$ is the second smallest element of X, i.e., the smallest element of X once $a _ { 0 }$ is removed; $a _ { 2 }$ is the third smallest element of X; and so forth. Observe that in order to define $a _ { n } .$ , one only needs to know the values of $a _ { m }$ for all $m < n ,$ , so this definition is recursive. Also, since X is infinite, the set $\{ x \in X$ : $x \neq a _ { m }$ for all $m < n \}$ is infinite(?), hence non-empty. Thus by the wellordering principle, the minimum, min $\{ x \in X : x \neq a _ { m }$ for all $m < n \}$ is always well-defined. 

One can show(?) that $a _ { n }$ is an increasing sequence, i.e. 

$$
a _ {0} <   a _ {1} <   a _ {2} <   \dots
$$

and in particular that(?) $a _ { n } \neq a _ { m }$ for all $n \neq m$ . Also, we have(?) $a _ { n } \in X$ for each natural number n. 

Now define the function $f : \mathbf { N }  X$ by $f ( n ) \ : = \ a _ { n }$ . From the previous paragraph we know that f is one-to-one. Now we show that f is onto. In other words, we claim that for every $x \in X$ , there exists an n such that $a _ { n } = x$ 

<!-- === Source: MinerU_markdown_Analysis_I_-_By_Terence_Tao_201_2122707919320490000.md (Page 201) === -->

Let $x \in X$ . Suppose for sake of contradiction that $a _ { n } \neq x$ for every natural number n. Then this implies(?) that x is an element of the set $\{ x \in X : x \neq a _ { m }$ for all $m \ : < \ : n \}$ for all n. By definition of ${ \boldsymbol { a } } _ { n } ,$ this implies that $x \geq a _ { n }$ for every natural number n. However, since $a _ { n }$ is an increasing sequence, we have $a _ { n } \geq n \ ( ? )$ , and hence $x \geq n$ for every natural number n. In particular we have $x \geq x + 1$ , which is a contradiction. Thus we must have $a _ { n } = x$ for some natural number n, and hence f is onto. 

Since $f : \mathbf { N }  X$ is both one-to-one and onto, it is a bijection. We have thus found at least one increasing bijection f from N to X. Now suppose for sake of contradiction that there was at least one other increasing bijection g from N to X which was not equal to $f .$ Then the set $\{ n \in \mathbf { N } : g ( n ) \neq f ( n ) \}$ is non-empty, and define m $: = \operatorname* { m i n } \{ n \in \mathbf { N }$ $g ( n ) \neq f ( n ) \}$ , thus in particular $g ( m ) \neq f ( m ) = a _ { m }$ , and $g ( n ) = f ( n ) =$ $a _ { n }$ for all $n < m$ . But we then must have(?) 

$$
g (m) = \min \{x \in X: x \neq a _ {t} \text { for   all } t <   m \} = a _ {m},
$$

a contradiction. Thus there is no other increasing bijection from N to X other than $f .$ □ 

Since finite sets are at most countable by definition, we thus have 

Corollary 8.1.6. All subsets of the natural numbers are at most countable. 

Corollary 8.1.7. If X is an at most countable set, and Y is a subset of X, then Y is at most countable. 

Proof. If X is finite then this follows from Proposition $3 . 6 . 1 4 ( \mathrm { c } )$ , so assume X is countable. Then there is a bijection $f : X \to$ N between X and N. Since Y is a subset of X, and f is a bijection from X and N, then when we restrict f to Y, we obtain a bijection between Y and f(Y). (Why is this a bijection?) Thus $f ( Y )$ has equal cardinality with Y. But $f ( Y )$ is a subset of N, and hence at most countable by Corollary 8.1.6. Hence Y is also at most countable. □ 

Proposition 8.1.8. Let Y be a set, and let $f : \mathbf { N }  Y$ be a function. Then f(N) is at most countable. 

Proof. See Exercise 8.1.4. 

## 8.1. Countability

Corollary 8.1.9. Let X be a countable set, and let $f : X \to Y$ be a function. Then $f ( X )$ is at most countable. 

Proof. See Exercise 8.1.5. 

Proposition 8.1.10. Let X be a countable set, and let Y be a countable set. Then $X \cup Y$ is a countable set. 

Proof. See Exercise 8.1.7. 

To summarize, any subset or image of a countable set is at most countable, and any finite union of countable sets is still countable. We can now establish countability of the integers. 

Corollary 8.1.11. The integers Z are countable. 

Proof. We already know that the set $\mathbf { N } = \{ 0 , 1 , 2 , 3 , . . . \}$ of natural numbers are countable. The set N defined by 

$$
- \mathbf {N} := \{- n: n \in \mathbf {N} \} = \{0, - 1, - 2, - 3, \dots \}
$$

is also countable, since the map $f ( n ) : = - n$ is a bijection between N and this set. Since the integers are the union of N and N, the claim follows from Proposition 8.1.10 □ 

To establish countability of the rationals, we need to relate countability with Cartesian products. In particular, we need to show that the set $\mathbf { N } \times \mathbf { N }$ is countable. We first need a preliminary lemma: 

Lemma 8.1.12. The set 

$$
A := \{(n, m) \in \mathbf {N} \times \mathbf {N}: 0 \leq m \leq n \}
$$

is countable. 

Proof. Define the sequence $a _ { 0 } , a _ { 1 } , a _ { 2 } , . . .$ . recursively by setting $a _ { 0 } : = 0$ , and $a _ { n + 1 } : = a _ { n } + n + 1$ for all natural numbers n. Thus 

$$
a _ {0} = 0; a _ {1} = 0 + 1; a _ {2} = 0 + 1 + 2; a _ {3} = 0 + 1 + 2 + 3; \dots .
$$

By induction one can show that $a _ { n }$ is increasing, i.e., that $a _ { n } \ > \ a _ { m }$ whenever $n > m \mathrm { \ ( w h y ? ) }$ 

Now define the function $f : A  \mathbf { N }$ by 

$$
f (n, m) := a _ {n} + m.
$$

We claim that f is one-to-one. In other words, if $( n , m )$ and $( n ^ { \prime } , m ^ { \prime } )$ are any two distinct elements of A, then we claim that $f ( n , m ) \neq f ( n ^ { \prime } , m ^ { \prime } )$ 

To prove this claim, let $( n , m )$ and $( n ^ { \prime } , m ^ { \prime } )$ be two distinct elements of A. There are three cases: $n ^ { \prime } = n , n ^ { \prime } > n .$ , and $n ^ { \prime } < n$ . First suppose that $n ^ { \prime } = n$ . Then we must have $m \neq m ^ { \prime } .$ , otherwise $( n , m )$ and $( n ^ { \prime } , m ^ { \prime } )$ would not be distinct. Thus $a _ { n } + m \neq a _ { n } + m ^ { \prime }$ , and hence $f ( n , m ) \neq f ( n ^ { \prime } , m ^ { \prime } )$ , as desired. 

Now suppose that $n ^ { \prime } > n$ . Then $n ^ { \prime } \geq n + 1$ , and hence 

$$
f (n ^ {\prime}, m ^ {\prime}) = a _ {n ^ {\prime}} + m ^ {\prime} \geq a _ {n ^ {\prime}} \geq a _ {n + 1} = a _ {n} + n + 1.
$$

But since $( n , m ) \in A$ , we have $m \leq n < n + 1$ , and hence 

$$
f (n ^ {\prime}, m ^ {\prime}) \geq a _ {n} + n + 1 > a _ {n} + m = f (n, m),
$$

and thus $f ( n ^ { \prime } , m ^ { \prime } ) \neq f ( n , m )$ 

The case $n ^ { \prime } < n$ is proven similarly, by switching the rˆoles of n and $n ^ { \prime }$ in the previous argument. Thus we have shown that f is one-to-one. Thus f is a bijection from A to $f ( A )$ , and so A has equal cardinality with $f ( A )$ . But $f ( A )$ is a subset of N, and hence by Corollary 8.1.6 $f ( A )$ is at most countable. Therefore A is at most countable. But, A is clearly not finite. (Why? Hint: if A was finite, then every subset of A would be finite, and in particular $\{ ( n , 0 ) : n \in \mathbf { N } \}$ would be finite, but this is clearly countably infinite, a contradiction.) Thus, A must be countable. □ 

Corollary 8.1.13. The set $\mathbf N \times \mathbf N$ is countable. 

Proof. We already know that the set 

$$
A := \{(n, m) \in \mathbf {N} \times \mathbf {N}: 0 \leq m \leq n \}
$$

is countable. This implies that the set 

$$
B := \{(n, m) \in \mathbf {N} \times \mathbf {N}: 0 \leq n \leq m \}
$$

is also countable, since the map $f : A  B$ given by $f ( n , m ) : = ( m , n )$ is a bijection from A to $B  { \mathrm { \ : \left( w h y ? \right) } }$ . But since $\mathbf { N } \times \mathbf { N }$ is the union of A and B (why?), the claim then follows from Proposition 8.1.10. □ 

Corollary 8.1.14. If X and Y are countable, then $X \times Y$ is countable. 

Proof. See Exercise 8.1.8. 

## 8.1. Countability

Corollary 8.1.15. The rationals Q are countable. 

Proof. We already know that the integers Z are countable, which implies that the non-zero integers ${ \bf Z } - \{ 0 \}$ are countable (why?). By Corollary 8.1.14, the set 

$$
\mathbf {Z} \times (\mathbf {Z} - \{0 \}) = \{(a, b): a, b \in \mathbf {Z}, b \neq 0 \}
$$

is thus countable. If one lets $f : { \bf Z } \times ( { \bf Z } - \{ 0 \} ) \to { \bf Q }$ be the function $f ( a , b ) : = a / b$ (note that f is well-defined since we prohibit b from being equal to 0), we see from Corollary 8.1.9 that $f ( \mathbf { Z } \times ( \mathbf { Z } - \{ 0 \} ) )$ is at most countable. But we have $f ( \mathbf { Z } \times ( \mathbf { Z } - \{ 0 \} ) ) = \mathbf { Q }$ (why? This is basically the definition of the rationals Q). Thus Q is at most countable. However, Q cannot be finite, since it contains the infinite set N. Thus Q is countable. □ 

Remark 8.1.16. Because the rationals are countable, we know in principle that it is possible to arrange the rational numbers as a sequence: 

$$
\mathbf {Q} = \{a _ {0}, a _ {1}, a _ {2}, a _ {3}, \ldots \}
$$

such that every element of the sequence is diferent from every other element, and that the elements of the sequence exhaust Q (i.e., every rational number turns up as one of the elements $a _ { n }$ of the sequence). However, it is quite dificult (though not impossible) to actually try and come up with an explicit sequence $a _ { 0 } , a _ { 1 } , . . .$ . which does this; see Exercise 8.1.10. 

## — Exercises —

Exercise 8.1.1. Let X be a set. Show that X is infinite if and only if there exists a proper subset $Y \subsetneq X$ of X which has the same cardinality as X. (This exercise requires the axiom of choice, Axiom 8.1) 

Exercise 8.1.2. Prove Proposition 8.1.4. (Hint: you can either use induction, or use the principle of infinite descent, Exercise 4.4.2, or use the least upper bound (or greatest lower bound) principle, Theorem 5.5.9.) Does the wellordering principle work if we replace the natural numbers by the integers? What if we replace the natural numbers by the positive rationals? Explain. 

Exercise 8.1.3. Fill in the gaps marked (?) in Proposition 8.1.5. 

Exercise 8.1.4. Prove Proposition 8.1.8. (Hint: the basic problem here is that f is not assumed to be one-to-one. Define A to be the set 

$$
A := \{n \in \mathbf {N}: f (m) \neq f (n) \text {   for   all   } 0 \leq m <   n \};
$$

informally speaking, A is the set of natural numbers n for which $f ( n )$ does not appear in the sequence $f ( 0 ) , f ( 1 ) , \dots f ( n - 1 )$ . Prove that when f is restricted to $A .$ , it becomes a bijection from A to $f ( \mathbf { N } )$ . Then use Proposition 8.1.5.) 

Exercise 8.1.5. Use Proposition 8.1.8 to prove Corollary 8.1.9. 

Exercise 8.1.6. Let A be a set. Show that A is at most countable if and only if there exists an injective map $f : A  \mathbf { N }$ from A to N. 

Exercise 8.1.7. Prove Proposition 8.1.10. (Hint: by hypothesis, we have a bijection $f : \mathbf { N }  X$ , and a bijection $g : \mathbf { N }  Y$ . Now define $h : \mathbf { N }  X \cup Y$ by setting $h ( 2 n ) : = f ( n )$ and $h ( 2 n + 1 ) : = g ( n )$ for every natural number n, and show that $h ( \mathbf { N } ) = X \cup Y$ . Then use Corollary 8.1.9, and show that $X \cup Y$ cannot possibly be finite.) 

Exercise 8.1.8. Use Corollary 8.1.13 to prove Corollary 8.1.14. 

Exercise 8.1.9. Suppose that I is an at most countable set, and for each $\alpha \in I$ let $A _ { \alpha }$ be an at most countable set. Show that the set $\textstyle \bigcup _ { \alpha \in I } A _ { \alpha }$ is also at most countable. In particular, countable unions of countable sets are countable. (This exercise requires the axiom of choice, see Section 8.4.) 

Exercise 8.1.10. Find a bijection $f : \mathbf { N }  \mathbf { Q }$ from the natural numbers to the rationals. (Warning: this is actually rather tricky to do explicitly; it is dificult to get f to be simultaneously injective and surjective.) 

## 8.2 Summation on infinite sets

We now introduce the concept of summation on countable sets, which will be well-defined provided that the sum is absolutely convergent. 

Definition 8.2.1 (Series on countable sets). Let X be a countable set, and let $f : X \to \mathbf { R }$ be a function. We say that the series $\textstyle \sum _ { x \in X } f ( x )$ is absolutely convergent if for some bijection $g : \textbf { N } \to X$ , the sum $\scriptstyle \sum _ { n = 0 } ^ { \infty } f ( g ( n ) )$ is absolutely convergent. We then define the sum of $\textstyle \sum _ { x \in X } f ( x )$ by the formula 

$$
\sum_ {x \in X} f (x) = \sum_ {n = 0} ^ {\infty} f (g (n)).
$$

From Proposition 7.4.3 (and Proposition 3.6.4), one can show that these definitions do not depend on the choice of $^ { g , }$ , and so are well defined. 

We can now give an important theorem about double summations. 

Theorem 8.2.2 (Fubini’s theorem for infinite sums). Let $f : \mathbf { N } \times \mathbf { N } $ R be a function such that $\scriptstyle \sum _ { ( n , m ) \in \mathbf { N } \times \mathbf { N } } f ( n , m )$ is absolutely convergent. 

## 8.2. Summation on infinite sets

Then we have 

$$
\begin{array}{c} \sum_ {n = 0} ^ {\infty} \left(\sum_ {m = 0} ^ {\infty} f (n, m)\right) = \sum_ {(n, m) \in \mathbf {N} \times \mathbf {N}} f (n, m) \\ = \sum_ {(m, n) \in \mathbf {N} \times \mathbf {N}} f (n, m) \\ = \sum_ {m = 0} ^ {\infty} \left(\sum_ {n = 0} ^ {\infty} f (n, m)\right). \end{array}
$$

In other words, we can switch the order of infinite sums provided that the entire sum is absolutely convergent. You should go back and compare this with Example 1.2.5. 

Proof. (A sketch only; this proof is considerably more complex than the other proofs, and is optional reading.) The second equality follows easily from Proposition 7.4.3 (and Proposition 3.6.4). We shall just prove the first equality, as the third is very similar (basically one switches the rˆole of n and m). 

Let us first consider the case when $f ( n , m )$ is always non-negative (we will deal with the general case later). Write 

$$
L := \sum_ {(n, m) \in \mathbf {N} \times \mathbf {N}} f (n, m);
$$

our task is to show that the series $\scriptstyle \sum _ { n = 0 } ^ { \infty } ( \sum _ { m = 0 } ^ { \infty } f ( n , m ) )$ converges to L. 

One can easily show that $\sum _ { ( n , m ) \in X } f ( n , m ) \leq L$ for all finite sets $X \subset \mathbf { N } \times \mathbf { N }$ . (Why? Use a bijection g between N N and N, and then use the fact that $g ( X )$ is finite, hence bounded.) In particular, for every $n \in \mathbf N$ and $M \in \mathbf { N }$ we have $\textstyle \sum _ { m = 0 } ^ { M } f ( n , m ) \leq L$ , which implies by Proposition 6.3.8 that $\textstyle \sum _ { m = 0 } ^ { \infty } f ( n , m )$ is convergent for each m. Similarly, for any $N \in \mathbf { N }$ and $M \in \mathbf { N }$ we have (by Corollary 7.1.14) 

$$
\sum_ {n = 0} ^ {N} \sum_ {m = 0} ^ {M} f (n, m) \leq \sum_ {(n, m) \in X} f (n, m) \leq L
$$

where X is the set $\{ ( n , m ) \in \mathbf { N } \times \mathbf { N } : n \leq N , m \leq M \}$ which is finite by Proposition 3.6.14. Taking suprema of this as $M \to \infty$ we have (by 

limit laws, and an induction on N) 

$$
\sum_ {n = 0} ^ {N} \sum_ {m = 0} ^ {\infty} f (n, m) \leq L.
$$

By Proposition 6.3.8, this implies that $\scriptstyle \sum _ { n = 0 } ^ { \infty } \sum _ { m = 0 } ^ { \infty } f ( n , m )$ converges, and 

$$
\sum_ {n = 0} ^ {\infty} \sum_ {m = 0} ^ {\infty} f (n, m) \leq L.
$$

To finish the proof, it will sufice to show that 

$$
\sum_ {n = 0} ^ {\infty} \sum_ {m = 0} ^ {\infty} f (n, m) \geq L - \varepsilon
$$

for every $\varepsilon > 0$ . (Why will this be enough? Prove by contradiction.) ${ \mathrm { S o } } ,$ let $\varepsilon > 0$ . By definition of $L ,$ , we can then find a finite set $X \subseteq \mathbf { N } \times \mathbf { N }$ such that $\sum _ { ( n , m ) \in X } f ( n , m ) \geq L - \varepsilon .$ . (Why?) This set, being finite, must be contained in some set of the form $Y : = \{ ( n , m ) \in \mathbf { N } \times \mathbf { N } : n \leq$ $N ; m \leq M \}$ . (Why? use induction.) Thus by Corollary 7.1.14 

$$
\sum_ {n = 0} ^ {N} \sum_ {m = 0} ^ {M} f (n, m) = \sum_ {(n, m) \in Y} f (n, m) \geq \sum_ {(n, m) \in X} f (n, m) \geq L - \varepsilon
$$

and hence 

$$
\sum_ {n = 0} ^ {\infty} \sum_ {m = 0} ^ {\infty} f (n, m) \geq \sum_ {n = 0} ^ {N} \sum_ {m = 0} ^ {\infty} f (n, m) \geq \sum_ {n = 0} ^ {N} \sum_ {m = 0} ^ {M} f (n, m) \geq L - \varepsilon
$$

as desired. 

This proves the claim when the $f ( n , m )$ are all non-negative. A similar argument works when the $f ( n , m )$ are all non-positive (in fact, one can simply apply the result just obtained to the function $- f ( n , m )$ and then use limit laws to remove the . For the general case, note that any function $f ( n , m )$ can be written $\mathrm { ( w h y ? ) }$ as $f _ { + } ( n , m ) + f _ { - } ( n , m )$ • where $f _ { + } ( n , m )$ is the positive part of $f ( n , m ) \ { \mathrm { ~ ( i . e . } }$ , it equals $f ( n , m )$ when $f ( n , m )$ is positive, and 0 otherwise), and $f _ { - }$ is the negative part of $f ( n , m )$ (it equals $f ( n , m )$ when $f ( n , m )$ is negative, and 0 otherwise). It is easy to show that if $\scriptstyle \sum _ { ( n , m ) \in \mathbf { N } \times \mathbf { N } } f ( n , m )$ is absolutely convergent, then so are $\scriptstyle \sum _ { ( n , m ) \in \mathbf { N } \times \mathbf { N } } f _ { + } ( { \overset { \prime } { n } } , { \overset { \prime } { m } } )$ and $\scriptstyle \sum _ { ( n , m ) \in \mathbf { N } \times \mathbf { N } } f _ { - } ( n , m )$ . So now one applies the results just obtained to $f _ { + }$ and to $f _ { - }$ and adds them together using limit laws to obtain the result for a general $f .$ □ 

There is another characterization of absolutely convergent series. 

Lemma 8.2.3. Let X be an at most countable set, and let $f : X  \mathbf { R }$ be a function. Then the series $\textstyle \sum _ { x \in X } f ( x )$ is absolutely convergent if and only if 

$$
\sup \left\{\sum_ {x \in A} | f (x) |: A \subseteq X, A \text {   finite } \right\} <   \infty .
$$

Proof. See Exercise 8.2.1. 

Inspired by this lemma, we may now define the concept of an absolutely convergent series even when the set X could be uncountable. (We give some examples of uncountable sets in the next section.) 

Definition 8.2.4. Let X be a set (which could be uncountable), and let $f : X \to \mathbf { R }$ be a function. We say that the series $\textstyle \sum _ { x \in X } f ( x )$ is absolutely convergent if 

$$
\sup \left\{\sum_ {x \in A} | f (x) |: A \subseteq X, A \text {   finite } \right\} <   \infty .
$$

Note that we have not yet said what the series $\textstyle \sum _ { x \in X } f ( x )$ is equal to. This shall be accomplished by the following lemma. 

Lemma 8.2.5. Let X be a set (which could be uncountable), and let $f : X  \mathbf { R }$ be a function such that the series $\textstyle \sum _ { x \in X } f ( x )$ is absolutely convergent. Then the set $\{ x \in X : f ( x ) \neq 0 \}$ is at most countable. (This result requires the axiom of choice, see Section 8.4.) 

Proof. See Exercise 8.2.2. 

Because of this, we can define the value of $\textstyle \sum _ { x \in X } f ( x )$ for any abso-lutely convergent series on an uncountable set X by the formula 

$$
\sum_ {x \in X} f (x) := \sum_ {x \in X: f (x) \neq 0} f (x),
$$

since we have replaced a sum on an uncountable set X by a sum on the countable set $\{ x \in X : f ( x ) \neq 0 \}$ . (Note that if the former sum is absolutely convergent, then the latter one is also.) Note also that this definition is consistent with the definitions we already have for series on countable sets. 

We give some laws for absolutely convergent series on arbitrary sets. 

Proposition 8.2.6 (Absolutely convergent series laws). Let X be an arbitrary set (possibly uncountable), and let $f : X  \mathbf { R }$ and $g : X  \mathbf { R }$ be functions such that the series $\textstyle \sum _ { x \in X } f ( x )$ and $\textstyle \sum _ { x \in X } g ( x )$ are both absolutely convergent. 

(a) The series $\textstyle \sum _ { x \in X } ( f ( x ) + g ( x ) )$ is absolutely convergent, and 

$$
\sum_ {x \in X} (f (x) + g (x)) = \sum_ {x \in X} f (x) + \sum_ {x \in X} g (x).
$$

(b) If c is a real number, then $\textstyle \sum _ { x \in X } c f ( x )$ is absolutely convergent, and 

$$
\sum_ {x \in X} c f (x) = c \sum_ {x \in X} f (x).
$$

(c) If $X = X _ { 1 } \cup X _ { 2 }$ for some disjoint sets $X _ { 1 }$ and $X _ { 2 }$ , then $\textstyle \sum _ { x \in X _ { 1 } } f ( x )$ and $\textstyle \sum _ { x \in X _ { 2 } } f ( x )$ are absolutely convergent, and 

$$
\sum_ {x \in X _ {1} \cup X _ {2}} f (x) = \sum_ {x \in X _ {1}} f (x) + \sum_ {x \in X _ {2}} f (x).
$$

Conversely, if $h \ : \ X \ \to \ \mathbf { R }$ is such that $\textstyle \sum _ { x \in X _ { 1 } } h ( x )$ and $\textstyle \sum _ { x \in X _ { 2 } } h ( x )$ are absolutely convergent, then $\textstyle \sum _ { x \in X _ { 1 } \cup X _ { 2 } } { \bar { h } } ( x )$ is also absolutely convergent, and 

$$
\sum_ {x \in X _ {1} \cup X _ {2}} h (x) = \sum_ {x \in X _ {1}} h (x) + \sum_ {x \in X _ {2}} h (x).
$$

(d) If Y is another set, and $\phi ~ : ~ Y ~ \to ~ X$ is a bijection, then $\textstyle \sum _ { y \in Y } f ( \phi ( y ) )$ is absolutely convergent, and 

$$
\sum_ {y \in Y} f (\phi (y)) = \sum_ {x \in X} f (x).
$$

(This result requires the axiom of choice when X is uncountable, see Section $8 . 4 \cdot \ j$ 

Proof. See Exercise 8.2.3. 

Recall in Example 7.4.4 that if a series was conditionally convergent, but not absolutely convergent, then its behaviour with respect to rearrangements was bad. We now analyze this phenomenon further. 

Lemma 8.2.7. Let $\textstyle \sum _ { n = 0 } ^ { \infty } a _ { n }$ be a series of real numbers which is con-ditionally convergent, but not absolutely convergent. Define the sets $A _ { + } ~ : = ~ \{ n ~ \in \textbf { N } : ~ a _ { n } ~ \geq ~ 0 \}$ and $A _ { - } \ : = \ \{ n \in \textbf { N } : \ a _ { n } \ < \ 0 \}$ , thus $A _ { + } \cup A _ { - } = \mathbf { N }$ and $A _ { + } \cap A _ { - } = \varnothing$ . Then both of the series $\textstyle \sum _ { n \in A _ { + } } a _ { n }$ and $\textstyle \sum _ { n \in A _ { - } } a _ { n }$ are not conditionally convergent (and thus not absolutely convergent). 

Proof. See Exercise 8.2.4. 

We are now ready to present a remarkable theorem of Georg Riemann (1826–1866), which asserts that a series which converges conditionally but not absolutely can be rearranged to converge to any value one pleases! 

Theorem 8.2.8. Let $\textstyle \sum _ { n = 0 } ^ { \infty } a _ { n }$ be a series which is conditionally conver-gent, but not absolutely convergent, and let L be any real number. Then there exists a bijection $f : \mathbf { N }  \mathbf { N }$ such that $\textstyle \sum _ { m = 0 } ^ { \infty } a _ { f ( m ) }$ converges conditionally to L. 

Proof. (Optional) We give a sketch of the proof, leaving the details to be filled in in Exercise 8.2.5. Let $A _ { + }$ and A be the sets in Lemma 8.2.7; from that lemma we know that $\textstyle \sum _ { n \in A _ { + } } a _ { n }$ and $\textstyle \sum _ { n \in A _ { - } } a _ { n }$ both fail to be absolutely convergent. In particular $A _ { + }$ and $A _ { - }$ <sup>−</sup> are infinite (why?). By Proposition 8.1.5 we can then find increasing bijections $f _ { + } : \mathbf { N }  A _ { + }$ and $f _ { - } : \mathbf { N }  A .$ . Thus the sums $\scriptstyle \sum _ { m = 0 } ^ { \infty } a _ { f _ { + } ( m ) }$ and $\scriptstyle \sum _ { m = 0 } ^ { \infty } a _ { f _ { - } ( m ) }$ both  fail to be absolutely convergent (why?). The plan shall be to select terms from the divergent series $\scriptstyle \sum _ { m = 0 } ^ { \infty } a _ { f _ { + } ( m ) }$ and $\scriptstyle \sum _ { m = 0 } ^ { \infty } a _ { f _ { - } ( m ) }$ in a well-chosen  order in order to keep their diference converging towards $L$ 

We define the sequence $n _ { 0 } , n _ { 1 } , n _ { 2 } , . . .$ of natural numbers recursively as follows. Suppose that j is a natural number, and that $n _ { i }$ has already been defined for all $i < j$ (this is vacuously true if $j = 0 )$ . We then define $n _ { j }$ by the following rule: 

(I) If $\textstyle \sum _ { 0 \leq i < j } a _ { n _ { i } } < L$ , then we set 

$$
n _ {j} := \min \{n \in A _ {+}: n \neq n _ {i} \text {   for   all   } i <   j \}.
$$

(II) If instead $\textstyle \sum _ { 0 \leq i < j } a _ { n _ { i } } \geq L$ , then we set 

$$
n _ {j} := \min \{n \in A _ {-}: n \neq n _ {i} \text {   for   all   } i <   j \}.
$$

Note that this recursive definition is well-defined because $A _ { + }$ and $A _ { - }$ are infinite, and so the sets $\{ n \in A _ { + } : n \neq n _ { i }$ for all $i < j \}$ and $n _ { j } : = \operatorname* { m i n } \{ n \in A _ { - } : n \neq n _ { i }$ for all $i < j \}$ are never empty. (Intuitively, we add a non-negative number to the series whenever the partial sum is too low, and add a negative number when the sum is too high.) One can then verify the following claims: 

The map $j \mapsto n _ { j }$ is injective. (Why?) 

Case I occurs an infinite number of times, and Case II also occurs an infinite number of times. (Why? prove by contradiction.) 

The map $j \mapsto n _ { j }$ is surjective. (Why?) 

We have $\operatorname* { l i m } _ { j \to \infty } a _ { n _ { j } } = 0$ . (Why? Note from Corollary 7.2.6 that $\scriptstyle \operatorname* { l i m } _ { n \to \infty } a _ { n } = 0 . )$ 

We have lim $\begin{array} { r } { \mathfrak { 1 } _ { j  \infty } \sum _ { 0 \leq i < j } a _ { n _ { i } } = L . ~ ( \mathrm { W h y ? } ) } \end{array}$ 

The claim then follows by setting $f ( i ) : = n _ { i }$ for all i. 

$$
- \text { Exercises } -
$$

Exercise 8.2.1. Prove Lemma 8.2.3. (Hint: you may find Exercise 3.6.3 to be useful.) 

Exercise 8.2.2. Prove Lemma 8.2.5. (Hint: first show if M is the quantity 

$$
M := \sup \left\{\sum_ {x \in A} | f (x) |: A \subseteq X, A \text {   finite } \right\}
$$

then the sets $\{ x \in X : | f ( x ) | > 1 / n \}$ are finite with cardinality at most Mn for every positive integer n. Then use Exercise 8.1.9 (which uses the axiom of choice, see Section 8.4).) 

Exercise 8.2.3. Prove Proposition 8.2.6. (Hint: you may of course use all the results from Chapter 7 to do this.) 

Exercise 8.2.4. Prove Lemma 8.2.7. (Hint: prove by contradiction, and use limit laws.) 

Exercise 8.2.5. Explain the gaps marked (why?) in the proof of Theorem 8.2.8. 

Exercise 8.2.6. Let $\textstyle \sum _ { n = 0 } ^ { \infty } a _ { n }$ be a series which is conditionally convergent, but not absolutely convergent. Show that there exists a bijection $f : \mathbf { N }  \mathbf { N }$ such that $\textstyle \sum _ { m = 0 } ^ { \infty } a _ { f ( m ) }$ diverges to + , or more precisely that 

$$
\liminf _ {N \to \infty} \sum_ {m = N} ^ {\infty} a _ {f (m)} = \limsup _ {N \to \infty} \sum_ {m = N} ^ {\infty} a _ {f (m)} = + \infty .
$$

(Of course, a similar statement holds with + replaced by $- \infty . )$ 

## 8.3 Uncountable sets

We have just shown that a lot of infinite sets are countable - even such sets as the rationals, for which it is not obvious how to arrange as a sequence. After such examples, one may begin to hope that other infinite sets, such as the real numbers, are also countable - after all, the real numbers are nothing more than (formal) limits of the rationals, and we’ve already shown the rationals are countable, so it seems plausible that the reals are also countable. 

It was thus a great shock when Georg Cantor (1845–1918) showed in 1873 that certain sets - including the real numbers R are in fact uncountable - no matter how hard you try, you cannot arrange the real numbers R as a sequence $a _ { 0 } , a _ { 1 } , a _ { 2 } , \dotsc$ (Of course, the real numbers R can contain many infinite sequences, e.g., the sequence 0, 1, 2, 3, 4, . . .. However, what Cantor proved is that no such sequence can ever exhaust the real numbers; no matter what sequence of real numbers you choose, there will always be some real numbers that are not covered by that sequence.) 

Recall from Remark 3.4.10 that if X is a set, then the power set of X, denoted $2 ^ { X } : = \{ A : A \subseteq X \}$ , is the set of all subsets of X. Thus for instance $2 ^ { \{ 1 , 2 \} } = \{ \stackrel { \cdot } { \varnothing } , \{ 1 \} , \{ 2 \} , \{ 1 , 2 \} \}$ . The reason for the notation $2 ^ { X }$ is given in Exercise 8.3.1. 

Theorem 8.3.1 (Cantor’s theorem). Let X be an arbitrary set (finite or infinite). Then the sets X and $2 ^ { X }$ cannot have equal cardinality. 

Proof. Suppose for sake of contradiction that the sets X and $2 ^ { X }$ had equal cardinality. Then there exists a bijection $f : X \to 2 ^ { X }$ between X and the power set of X. Now consider the set 

$$
A := \{x \in X: x \not \in f (x) \}.
$$

Note that this set is well-defined since $f ( x )$ is an element of $2 ^ { X }$ and is hence a subset of X. Clearly A is a subset of $X$ , hence is an element of $2 ^ { X }$ . Since $f$ is a bijection, there must therefore exist $x \in X$ such that $f ( x ) = A$ . There are now two cases, depending on whether $x \in A$ or $x \not \in A$ . If $x \in A$ , then by definition of A we have $x \not \in f ( x )$ , hence $x \not \in A .$ , a contradiction. But if $x \not \in A$ , then $x \not \in f ( x )$ , hence by definition of A we have $x \in A$ , a contradiction. Thus in either case we have a contradiction. □ 

Remark 8.3.2. The reader should compare the proof of Cantor’s theorem with the statement of Russell’s paradox (Section 3.2). The point is that a bijection between X and $2 ^ { X }$ would come dangerously close to the concept of a set X “containing itself”. 

Corollary 8.3.3. $2 ^ { \mathbf { N } }$ is uncountable. 

Proof. By Theorem 8.3.1, $2 ^ { \mathbf { N } }$ cannot have equal cardinality with N, hence is either uncountable or finite. However, $2 ^ { \mathbf { N } }$ contains as a subset the set of singletons $\{ \{ n \} : n \in \mathbf { N } \} .$ , which is clearly bijective to N and hence countably infinite. Thus $2 ^ { \mathbf { \hat { N } } }$ cannot be finite (by Proposition 3.6.14), and is hence uncountable. □ 

Cantor’s theorem has the following important (and unintuitive) consequence. 

Corollary 8.3.4. R is uncountable. 

Proof. Let us define the map $f : 2 ^ { \mathbf { N } }  \mathbf { R }$ by the formula 

$$
f (A) := \sum_ {n \in A} 1 0 ^ {- n}.
$$

Observe that since $\scriptstyle \sum _ { n = 0 } ^ { \infty } 1 0 ^ { - n }$ is an absolutely convergent series (by Lemma 7.3.3), the series $\textstyle \sum _ { n \in A } 1 0 ^ { - n }$ is also absolutely convergent (by Proposition $8 . 2 . 6 ( \mathrm { c } ) )$ . Thus the map $f$ is well defined. We now claim that $f$ is injective. Suppose for sake of contradiction that there were two distinct sets A, $B \in 2 ^ { \mathbf { N } }$ such that $f ( A ) = f ( B )$ . Since $A \neq B$ , the set $( A \backslash B ) \cup ( B \backslash A )$ is a non-empty subset of N. By the well-ordering principle (Proposition 8.1.4), we can then define the minimum of this set, say $n _ { 0 } : = \operatorname* { m i n } ( A \backslash B ) \cup ( B \backslash A )$ . Thus $n _ { 0 }$ either lies in $A \backslash B$ or $B \backslash A$ By symmetry we may assume it lies in $A \backslash B$ . Then $n _ { 0 } \in A , n _ { 0 } \notin B$ , and for all $n < n _ { 0 }$ we either have $n \in A , B$ or $n \not \in A , B$ . Thus 

$$
\begin{array}{l} 0 = f (A) - f (B) \\ \quad = \sum_ {n \in A} 1 0 ^ {- n} - \sum_ {n \in B} 1 0 ^ {- n} \\ \quad = \left(\sum_ {n <   n _ {0}: n \in A} 1 0 ^ {- n} + 1 0 ^ {- n _ {0}} + \sum_ {n > n _ {0}: n \in A} 1 0 ^ {- n}\right) \\ \quad - \left(\sum_ {n <   n _ {0}: n \in B} 1 0 ^ {- n} + \sum_ {n > n _ {0}: n \in B} 1 0 ^ {- n}\right) \\ \quad = 1 0 ^ {- n _ {0}} + \sum_ {n > n _ {0}: n \in A} 1 0 ^ {- n} - \sum_ {n > n _ {0}: n \in B} 1 0 ^ {- n} \\ \quad \geq 1 0 ^ {- n _ {0}} + 0 - \sum_ {n > n _ {0}} 1 0 ^ {- n} \\ \quad \geq 1 0 ^ {- n _ {0}} - \frac {1}{9} 1 0 ^ {- n _ {0}} \\ \quad > 0, \end{array}
$$

a contradiction, where we have used the geometric series lemma (Lemma 7.3.3) to sum 

$$
\sum_ {n > n _ {0}} 1 0 ^ {- n} = \sum_ {m = 0} ^ {\infty} 1 0 ^ {- (n _ {0} + 1 + m)} = 1 0 ^ {- n _ {0} - 1} \sum_ {m = 0} ^ {\infty} 1 0 ^ {- m} = \frac {1}{9} 1 0 ^ {- n _ {0}}.
$$

Thus $f$ is injective, which means that $f ( 2 ^ { \mathbf { N } } )$ has the same cardinality as $2 ^ { \mathbf { N } }$ and is thus uncountable. Since $f ( 2 ^ { \mathbf { N } } )$ is a subset of R, this forces R to be uncountable also (otherwise this would contradict Corollary 8.1.7), and we are done. □ 

Remark 8.3.5. We will give another proof of this result using measure theory in Exercise 11.42.6. 

Remark 8.3.6. Corollary 8.3.4 shows that the reals have strictly larger cardinality than the natural numbers (in the sense of Exercise 3.6.7). One could ask whether there exist any sets which have strictly larger cardinality than the natural numbers, but strictly smaller cardinality than the reals. The Continuum Hypothesis asserts that no such sets exist. Interestingly, it was shown in separate works of Kurt G¨odel (1906– 1978) and Paul Cohen (1934–2007) that this hypothesis is independent of the other axioms of set theory; it can neither be proved nor disproved in that set of axioms (unless those axioms are inconsistent, which is highly unlikely). 

— Exercises — 

Exercise 8.3.1. Let X be a finite set of cardinality n. Show that $2 ^ { X }$ is a finite set of cardinality 2<sup>n</sup>. (Hint: use induction on n.) 

Exercise 8.3.2. Let A, B, C be sets such that $A \subseteq B \subseteq C$ , and suppose that there is a injection $f : C \to A$ . Define the sets $D _ { 0 } , D _ { 1 } , D _ { 2 } , \ldots$ . recursively by setting $D _ { 0 } : = B \backslash A$ , and then $D _ { n + 1 } : = f ( D _ { n } )$ for all natural numbers n. Prove that the sets $D _ { 0 } , D _ { 1 } , \ldots$ . are all disjoint from each other $( \mathrm { i . e . , ~ } D _ { n } \cap D _ { m } = \emptyset$ whenever $n \neq m )$ . Also show that if $g : A  B$ is the function defined by setting $g ( x ) : = f ^ { - 1 } ( x )$ when $x \in \textstyle \bigcup _ { n = 1 } ^ { \infty } D _ { n }$ , and $g ( x ) : = x$ when $x \notin \mathsf { U } _ { n = 1 } ^ { \infty } D _ { n }$  then g does indeed map A to B and is a bijection between the two. In particular, A and B have the same cardinality. 

Exercise 8.3.3. Recall from Exercise 3.6.7 that a set A is said to have lesser or equal cardinality than a set B if there is an injective map $f : A  B$ from A to B. Using Exercise 8.3.2, show that if A, B are sets such that A has lesser or equal cardinality to B and B has lesser or equal cardinality to A, then A and B have equal cardinality. (This is known as the Schr¨oder-Bernstein theorem, after Ernst Schr¨oder (1841–1902) and Felix Bernstein (1878–1956).) 

Exercise 8.3.4. Let us say that a set A has strictly lesser cardinality than a set B if A has lesser than or equal cardinality to B (in the sense of Exercise 3.6.7) but A does not have equal cardinality to B. Show that for any set X, that X has strictly lesser cardinality than $2 ^ { \check { X } }$ . Also, show that if A has strictly lesser cardinality than B, and B has strictly lesser cardinality than C, then A has strictly lesser cardinality than C. 

Exercise 8.3.5. Show that no power set (i.e., a set of the form $2 ^ { X }$ for some set X) can be countably infinite. 

## 8.4 The axiom of choice

We now discuss the final axiom of the standard Zermelo-Fraenkel-Choice system of set theory, namely the axiom of choice. We have delayed introducing this axiom for a while now, to demonstrate that a large portion of the foundations of analysis can be constructed without appealing to this axiom. However, in many further developments of the theory, it is very convenient (and in some cases even essential) to employ this powerfu axiom. On the other hand, the axiom of choice can lead to a number of unintuitive consequences (for instance the Banach-Tarski paradox, a simplified version of which we will encounter in Section 11.43), and can lead to proofs that are philosophically somewhat unsatisfying. Nevertheless, the axiom is almost universally accepted by mathematicians. One reason for this confidence is a theorem due to the great logician Kurt G¨odel, who showed that a result proven using the axiom of choice will never contradict a result proven without the axiom of choice (unless all the other axioms of set theory are themselves inconsistent, which is highly unlikely). More precisely, G¨odel demonstrated that the axiom of choice is undecidable; it can neither be proved nor disproved from the other axioms of set theory, so long as those axioms are themselves consistent. (From a set of inconsistent axioms one can prove that every statement is both true and false.) In practice, this means that any $^ { 6 \cdot } \mathrm { r e a l - l i f e } ^ { 3 \cdot }$ application of analysis (more precisely, any application involving only “decidable” questions) which can be rigorously supported using the axiom of choice, can also be rigorously supported without the axiom of choice, though in many cases it would take a much more complicated and lengthier argument to do so if one were not allowed to use the axiom of choice. Thus one can view the axiom of choice as a convenient and safe labour-saving device in analysis. In other disciplines of mathematics, notably in set theory in which many of the questions are not decidable, the issue of whether to accept the axiom of choice is more open to debate, and involves some philosophical concerns as well as mathematical and logical ones. However, we will not discuss these issues in this text. 

We begin by generalizing the notion of finite Cartesian products from Definition 3.5.7 to infinite Cartesian products. 

Definition 8.4.1 (Infinite Cartesian products). Let I be a set (possibly infinite), and for each $\alpha \in I$ let $X _ { \alpha }$ be a set. We then define the Cartesian product $\Pi _ { \alpha \in I } X _ { \alpha }$ to be the set 

$$
\prod_ {\alpha \in I} X _ {\alpha} = \left\{(x _ {\alpha}) _ {\alpha \in I} \in (\bigcup_ {\beta \in I} X _ {\beta}) ^ {I}: x _ {\alpha} \in X _ {\alpha} \text {for all} \alpha \in I \right\},
$$

where we recall (from Axiom 3.10) that $( \cup _ { \alpha \in I } X _ { \alpha } ) ^ { I }$ is the set of all functions $( x _ { \alpha } ) _ { \alpha \in I }$ which assign an element $x _ { \alpha } \in \cup _ { \beta \in I } X _ { \beta }$ to each $\alpha \in I$ Thus $\Pi _ { \alpha \in I } X _ { \alpha }$ is a subset of that set of functions, consisting instead of those functions $( x _ { \alpha } ) _ { \alpha \in I }$ which assign an element $x _ { \alpha } \in X _ { \alpha }$ to each $\alpha \in I$ 

Example 8.4.2. For any sets I and X, we have $\begin{array} { r } { \prod _ { \alpha \in I } X = X ^ { I } \ \mathrm { ( w h y ? ) } } \end{array}$ If I is a set of the form $I : = \{ i \in \mathbf { N } : 1 \leq i \leq n \}$  ∈, then $\Pi _ { \alpha \in I } X _ { \alpha }$ is the same set as the set $\Pi _ { 1 \leq i \leq N } X _ { i }$ defined in Definition 3.5.7 (why?). 

Recall from Lemma 3.5.12 that if $X _ { 1 } , \ldots , X _ { n }$ were any finite collection of non-empty sets, then the finite Cartesian product $\prod _ { 1 \leq i \leq n } X _ { i }$ was also non-empty. The axiom of choice asserts that this statement is also true for infinite Cartesian products: 

Axiom 8.1 (Choice). Let I be a set, and for each $\alpha \in I$ , let $X _ { \alpha }$ be a non-empty set. Then $\Pi _ { \alpha \in I } X _ { \alpha }$ is also non-empty. In other words, there exists a function $( x _ { \alpha } ) _ { \alpha \in I }$ which assigns to each $\alpha \in I$ an element $x _ { \alpha } \in X _ { \alpha }$ 

Remark 8.4.3. The intuition behind this axiom is that given a (possibly infinite) collection of non-empty sets $X _ { \alpha }$ , one should be able to choose a single element $x _ { \alpha }$ from each one, and then form the possibly infinite tuple $( x _ { \alpha } ) _ { \alpha \in I }$ from all the choices one has made. On one hand, this is a very intuitively appealing axiom; in some sense one is just applying Lemma 3.1.6 over and over again. On the other hand, the fact that one is making an infinite number of arbitrary choices, with no explicit rule as to how to make these choices, is a little disconcerting. Indeed, there are many theorems proven using the axiom of choice which assert the abstract existence of some object x with certain properties, without saying at all what that object is, or how to construct it. Thus the axiom of choice can lead to proofs which are non-constructive - demonstrating existence of an object without actually constructing the object explicitly. This problem is not unique to the axiom of choice - it already appears for instance in Lemma 3.1.6 - but the objects shown to exist using the axiom of choice tend to be rather extreme in their level of non-constructiveness. However, as long as one is aware of the distinction between a non-constructive existence statement, and a constructive existence statement (with the latter being preferable, but not strictly necessary in many cases), there is no dificulty here, except perhaps on a philosophical level. 

Remark 8.4.4. There are many equivalent formulations of the axiom of choice; we give some of these in the exercises below. 

In analysis one often does not need the full power of the axiom of choice. Instead, one often only needs the axiom of countable choice, which is the same as the axiom of choice but with the index set I restricted to be at most countable. We give a typical example of this below. 

Lemma 8.4.5. Let E be a non-empty subset of the real line with $\operatorname* { s u p } ( E ) < \infty ( i . e . , E$ is bounded from above). Then there exists a sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ whose elements $a _ { n }$ all lie in $E _ { i }$ , such that $\scriptstyle \operatorname* { l i m } _ { n \to \infty } a _ { n } =$ $\operatorname { s u p } ( E )$ 

Proof. For each positive natural number n, let $X _ { n }$ denote the set 

$$
X _ {n} := \{x \in E: \sup (E) - 1 / n \leq x \leq \sup (E) \}.
$$

Since $\operatorname { s u p } ( E )$ is the least upper bound for $E _ { i }$ , then $\operatorname* { s u p } ( E ) - 1 / n$ cannot be an upper bound for $E ,$ and so $X _ { n }$ is non-empty for each n. Using the axiom of choice (or the axiom of countable choice), we can then find a sequence $( a _ { n } ) _ { n = 1 } ^ { \infty }$ such that $a _ { n } \in X _ { n }$ for all $n \geq 1$ . In particular $a _ { n } \in E$ for all n, and $\operatorname* { s u p } ( E ) - 1 / n \leq a _ { n } \leq \operatorname* { s u p } ( E )$ for all n. But then we have $\operatorname* { l i m } _ { n \to \infty } a _ { n } = \operatorname* { s u p } ( E )$ by the squeeze test (Corollary 6.4.14). □ 

Remark 8.4.6. In many special cases, one can obtain the conclusion of this lemma without using the axiom of choice. For instance, if E is a closed set (Definition 11.4.12) then one can define $a _ { n }$ without choice by the formula $a _ { n } : = \operatorname { i n f } ( X _ { n } )$ ; the extra hypothesis that E is closed will ensure that $a _ { n }$ lies in E. 

Another formulation of the axiom of choice is as follows. 

Proposition 8.4.7. Let X and Y be sets, and let $P ( x , y )$ be a property pertaining to an object $x \in X$ and an object $y \in Y$ such that for every $x \in X$ there is at least one $y \in Y$ such that $P ( x , y )$ is true. Then there exists a function $f : X \to Y$ such that $P ( x , f ( x ) )$ is true for all $x \in X$ 

Proof. See Exercise 8.4.1. 

## — Exercises —

Exercise 8.4.1. Show that the axiom of choice implies Proposition 8.4.7. (Hint: consider the sets $Y _ { x } : = \{ y \in Y : P ( x , y )$ is true for each $x \in X . )$ Conversely, show that if Proposition 8.4.7 is true, then the axiom of choice is also true. 

Exercise 8.4.2. Let I be a set, and for each $\alpha \in I$ let $X _ { \alpha }$ be a non-empty set. Suppose that all the sets $X _ { \alpha }$ are disjoint from each other, i.e., $X _ { \alpha } \cap X _ { \beta } = \varnothing$ for all distinct $\alpha , \beta \in I$ . Using the axiom of choice, show that there exists a set Y such that $\# ( Y \cap X _ { \alpha } ) = 1$ for all $\alpha \in I \ ( { \mathrm { i . e . , } } Y$ intersects each $X _ { \alpha }$ in exactly one element). Conversely, show that if the above statement was true for an arbitrary choice of sets I and non-empty disjoint sets $X _ { \alpha }$ , then the axiom of choice is true. (Hint: the problem is that in Axiom 8.1 the sets $X _ { \alpha }$ are not assumed to be disjoint. But this can be fixed by the trick by looking at the sets $\{ \alpha \} \times X _ { \alpha } = \{ ( \alpha , x ) : x \in X _ { \alpha } \}$ instead.) 

Exercise 8.4.3. Let A and B be sets such that there exists a surjection $g \ :$ $B  A .$ . Using the axiom of choice, show that there then exists an injection $f : A  B ;$ in other words A has lesser or equal cardinality to B in the sense of Exercise 3.6.7. (Hint: consider the inverse images $g ^ { - 1 } ( \{ a \} )$ for each $a \in A . )$ Compare this with Exercise 3.6.8. Conversely, show that if the above statement is true for arbitrary sets A, B and surjections $g : B  A$ , then the axiom of choice is true. (Hint: use Exercise 8.4.2.) 

## 8.5 Ordered sets

The axiom of choice is intimately connected to the theory of ordered sets. There are actually many types of ordered sets; we will concern ourselves with three such types, the partially ordered sets, the totally ordered sets, and the well-ordered sets. 

Definition 8.5.1 (Partially ordered sets). A partially ordered set (or poset) is a set X, together<sup>1</sup> with a relation $\leq _ { X }$ on X (thus for any two objects $x , y \in X$ , the statement $x \le _ { X } { \mathrm { ~ y ~ } }$ is either a true statement or a false statement). Furthermore, this relation is assumed to obey the following three properties: 

(Reflexivity) For any $x \in X$ , we have $x \le _ { X } x$ 

(Anti-symmetry) If $x , y \in X$ are such that $x \le _ { X } y$ and $y \le _ { X } ~ x$ 4 then $x = y$ 

(Transitivity) If $x , y , z \in X$ are such that $x \ \leq x \ y$ and $y \le _ { X } z$ , then $x \le _ { X } z$ 

We refer to $\leq _ { X }$ as the ordering relation. In most situations it is understood what the set X is from context, and in those cases we shall simply write $\leq$ instead of $\leq _ { X }$ . We write $x < _ { X } y$ (or $x < y$ for short) if $x \leq \chi$ y and $x \neq y$ 

Examples 8.5.2. The natural numbers N together with the usual lessthan-or-equal-to relation $\leq$ (as defined in Definition 2.2.11) forms a partially ordered set, by Proposition 2.2.12. Similar arguments (using the appropriate definitions and propositions) show that the integers $\mathbf { Z } ,$ the rationals Q, the reals R, and the extended reals $\mathbf { R } ^ { * }$ are also partially ordered sets. Meanwhile, if X is any collection of sets, and one uses the relation of $\mathrm { i s - a - s u b s e t - o f } \subseteq$ (as defined in Definition 3.1.15) for the ordering relation $\leq _ { X }$ , then X is also partially ordered (Proposition 3.1.18). Note that it is certainly possible to give these sets a diferent partial ordering than the standard one; see for instance Exercise 8.5.3. 

Definition 8.5.3 (Totally ordered set). Let X be a partially ordered set with some order relation $\leq _ { X }$ . A subset Y of X is said to be totally ordered if, given any two $y , y ^ { \prime } \in Y$ , we either have $y \le _ { X } y ^ { \prime }$ or $y ^ { \prime } \leq x$ y (or both). If X itself is totally ordered, we say that X is a totally ordered set (or chain) with order relation $\leq { \boldsymbol { X } }$ 

Examples 8.5.4. The natural numbers N, the integers Z, the rationals Q, reals R, and the extended reals $\mathbf { R } ^ { * }$ , all with the usual ordering relation $\leq ,$ are totally ordered (by Proposition 2.2.13, Lemma 4.1.11, Proposition 4.2.9, Proposition 5.4.7, and Proposition 6.2.5 respectively). Also, any subset of a totally ordered set is again totally ordered (why?). On the other hand, a collection of sets with the $\subseteq$ relation is usually not totally ordered. For instance, if X is the set $\{ \{ 1 , 2 \} , \{ 2 \} , \{ 2 , 3 \} , \{ 2 , 3 , 4 \} , \{ 5 \} \}$ , ordered by the set inclusion relation $\subseteq$ , then the elements 1, 2 and 2, 3 of X are not comparable to each other $( { \mathrm { i . e . , ~ } } \{ 1 , 2 \} \not \subseteq \{ 2 , 3 \}$ and $\{ 2 , 3 \} \not \subseteq \{ 1 , 2 \} )$ 

Definition 8.5.5 (Maximal and minimal elements). Let X be a partially ordered set, and let Y be a subset of X. We say that y is a minimal element of Y if $y \in Y$ and there is no element $y ^ { \prime } \in Y$ such that $y ^ { \prime } < y$ We say that y is a maximal element of Y if $y \in Y$ and there is no element $y ^ { \prime } \in Y$ such that $y < y ^ { \prime }$ 

Example 8.5.6. Using the set X from the previous example, 2 is a minimal element, 1, 2 and 2, 3, 4 are maximal elements, 5 is both a minimal and a maximal element, and 2, 3 is neither a minimal nor a maximal element. This example shows that a partially ordered set can have multiple maxima and minima; however, a totally ordered set cannot (Exercise 8.5.7). 

Example 8.5.7. The natural numbers N (ordered by $\leq )$ has a minimal element, namely 0, but no maximal element. The set of integers Z has no maximal and no minimal element. 

Definition 8.5.8 (Well-ordered sets). Let X be a partially ordered set, and let Y be a totally ordered subset of X. We say that Y is well-ordered if every non-empty subset of Y has a minimal element min(Y ). 

Examples 8.5.9. The natural numbers N are well-ordered by Proposition 8.1.4. However, the integers Z, the rationals Q, and the real numbers R are not (see Exercise 8.1.2). Every finite totally ordered set is well-ordered (Exercise 8.5.8). Every subset of a well-ordered set is again well-ordered (why?). 

One advantage of well-ordered sets is that they automatically obey a principle of strong induction (cf. Proposition 2.2.14): 

Proposition 8.5.10 (Principle of strong induction). Let X be a wellordered set with an ordering relation $\leq$ , and let $P ( n )$ be a property pertaining to an element $n \in X$ (i.e., for each $n \in X$ $P ( n )$ is either a true statement or a false statement). Suppose that for every $n \in X$ , we have the following implication: if $P ( m )$ is true for all $m \in X$ with $m < _ { X } n$ then $P ( n )$ is also true. Prove that $P ( n )$ is true for all $n \in X$ 

Remark 8.5.11. It may seem strange that there is no “base” case in strong induction, corresponding to the hypothesis $P ( 0 )$ in Axiom 2.5. However, such a base case is automatically included in the strong induction hypothesis. Indeed, if 0 is the minimal element of X, then by specializing the hypothesis “if $P ( m )$ is true for all $m \in X$ with $m < _ { X } n ,$ then $P ( n )$ is also true” to the $n = 0$ case, we automatically obtain that $P ( 0 )$ is true. (Why?) 

Proof. See Exercise 8.5.10. 

So far we have not seen the axiom of choice play any rˆole. This wil come in once we introduce the notion of an upper bound and a strict upper bound. 

Definition 8.5.12 (Upper bounds and strict upper bounds). Let X be a partially ordered set with ordering relation $\leq ,$ , and let Y be a subset of X. If $x \in X$ , we say that x is an upper bound for Y if $y \leq x$ for all $y \in Y$ . If in addition $x \not \in Y$ , we say that x is a strict upper bound for Y. Equivalently, x is a strict upper bound for Y if $y < x$ for all $y \in Y$ (Why is this equivalent?) 

Example 8.5.13. Let us work in the real number system R with the usual ordering $\leq$ . Then 2 is an upper bound for the set $\{ x \in \mathbf { R } : 1 \leq$ $x \leq 2 \}$ but is not a strict upper bound. The number 3, on the other hand, is a strict upper bound for this set. 

Lemma 8.5.14. Let X be a partially ordered set with ordering relation $\leq$ , and let $x _ { 0 }$ be an element of X. Then there is a well-ordered subset Y of X which has $x _ { 0 }$ as its minimal element, and which has no strict upper bound. 

Proof. The intuition behind this lemma is that one is trying to perform the following algorithm: we initalize $Y : = \{ x _ { 0 } \}$ . If Y has no strict upper bound, then we are done; otherwise, we choose a strict upper bound and add it to $Y .$ . Then we look again to see if Y has a strict upper bound or not. If not, we are done; otherwise we choose another strict upper bound and add it to $Y$ . We continue this algorithm “infinitely often” until we exhaust all the strict upper bounds; the axiom of choice comes in because infinitely many choices are involved. This is however not a rigorous proof because it is quite dificult to precisely pin down what it means to perform an algorithm “infinitely often”. Instead, what we will do is that we will isolate a collection of “partially completed” sets $Y$ which we shall call good sets, and then take the union of all these good sets to obtain a “completed” object $Y _ { \infty }$ which will indeed have no strict upper bound. 

We now begin the rigorous proof. Suppose for sake of contradiction that every well-ordered subset $Y$ of $X$ which has $x _ { 0 }$ as its minimal element has at least one strict upper bound. Using the axiom of choice (in the form of Proposition 8.4.7), we can thus assign a strict upper bound $s ( Y ) \in X$ to each well-ordered subset $Y$ of X which has $x _ { 0 }$ as its minimal element. 

Let us define a special class of subsets $Y$ of X. We say that a subset $Y$ of $X$ is good if it is well-ordered, contains $x _ { 0 }$ as its minimal element, and obeys the property that 

$$
x = s \left(\left\{y \in Y: y <   x \right\}\right) \text {   for   all   } x \in Y \backslash \left\{x _ {0} \right\}.
$$

Note that if $x \in Y \backslash \{ x _ { 0 } \}$ then the set $\{ y \in Y : y < x \}$ is a subset of X which is well-ordered and contains $x _ { 0 }$ as its minimal element. Let $\Omega : = \{ Y \subseteq X : Y$ is good be the collection of all good subsets of $X$ . This collection is not empty, since the subset $\{ x _ { 0 } \}$ of X is clearly good (why?). 

We make the following important observation: if $Y$ and $Y ^ { \prime }$ are two good subsets of $X$ , then every element of $Y ^ { \prime } \backslash Y$ is a strict upper bound for 

$Y ,$ and every element of $Y \backslash Y ^ { \prime }$ is a strict upper bound for $Y ^ { \prime }$ . (Exercise 8.5.13). In particular, given any two good sets Y and $Y ^ { \prime }$ , at least one of $Y ^ { \prime } \backslash Y$ and $Y \backslash Y ^ { \prime }$ must be empty (since they are both strict upper bounds of each other). In other words, Ω is totally ordered by set inclusion: given any two good sets Y and $Y ^ { \prime }$ , either $Y \subseteq Y ^ { \prime }$ or $Y ^ { \prime } \subseteq Y$ 

Let $Y _ { \infty } : = \bigcup \Omega , { \mathrm { i . e . , ~ } } Y _ { \infty }$ is the set of all elements of X which belong to at least one good subset of $X$ . Clearly $x _ { 0 } \in Y _ { \infty }$ . Also, since each good subset of X has $x _ { 0 }$ as its minimal element, the set $Y _ { \infty }$ also has $x _ { 0 }$ as its minimal element (why?). 

Next, we show that $Y _ { \infty }$ is totally ordered. Let $x , x ^ { \prime }$ be two elements of $Y _ { \infty }$ . By definition of $Y _ { \infty }$ , we know that x lies in some good set $Y$ and $x ^ { \prime }$ lies in some good set $Y ^ { \prime }$ . But since Ω is totally ordered, one of these good sets contains the other. Thus $x , x ^ { \prime }$ are contained in a single good set (either Y or $Y ^ { \prime } )$ ; since good sets are totally ordered, we thus see that either $x \leq x ^ { \prime }$ or $x ^ { \prime } \leq x$ as desired. 

Next, we show that $Y _ { \infty }$ is well-ordered. Let A be any non-empty subset of $Y _ { \infty }$ . Then we can pick an element $a \in A$ , which then lies in $Y _ { \infty }$ . Therefore there is a good set $Y$ such that $a \in Y$ . Then $A \cap Y$ is a non-empty subset of $Y ;$ ; since $Y$ is well-ordered, the set $A \cap Y$ thus has a minimal element, call it $b .$ . Now recall that for any other good set $Y ^ { \prime }$ every element of $Y ^ { \prime } \backslash Y$ is a strict upper bound for $Y$ , and in particular is larger than $b .$ Since b is a minimal element of $A \cap Y$ , this implies that b is also a minimal element of $A \cap Y ^ { \prime }$ for any good set $Y ^ { \prime }$ with $A \cap Y ^ { \prime } \neq \emptyset$ (why?). Since every element of A belongs to $Y _ { \infty }$ and hence belongs to at least one good set $Y ^ { \prime }$ , we thus see that b is a minimal element of A. Thus $Y _ { \infty }$ is well-ordered as claimed. 

Since $Y _ { \infty }$ is well-ordered with $x _ { 0 }$ as its minimal element, it has a strict upper bound $s ( Y _ { \infty } )$ . But then $Y _ { \infty } \cup \{ s ( Y _ { \infty } ) \}$ is well-ordered (why? see Exercise 8.5.11) and has $x _ { 0 }$ as its minimal element (why?). Thus this set is good, and must therefore be contained in $Y _ { \infty }$ . But this is a contradiction since $s ( Y _ { \infty } )$ is a strict upper bound for $Y _ { \infty }$ . Thus we have constructed a set with no strict upper bound, as desired. □ 

## The above lemma has the following important consequence:

Lemma 8.5.15 (Zorn’s lemma). Let X be a non-empty partially ordered set, with the property that every totally ordered subset Y of X has an upper bound. Then X contains at least one maximal element. 

Proof. See Exercise 8.5.14. 

We give some applications of Zorn’s lemma (also called the principle of transfinite induction) in the exercises below. 

## — Exercises —

Exercise 8.5.1. Consider the empty set $\varnothing$ with the empty order relation $\leq \varnothing$ (this relation is vacuous because the empty set has no elements). Is this set partially ordered? totally ordered? well-ordered? Explain. 

Exercise 8.5.2. Give examples of a set X and a relation $\leq$ such that 

(a) The relation $\leq$ is reflexive and anti-symmetric, but not transitive; 

(b) The relation $\leq$ is reflexive and transitive, but not anti-symmetric; 

(c) The relation $\leq$ is anti-symmetric and transitive, but not reflexive. 

Exercise 8.5.3. Given two positive integers $n , m \in { \bf N } \backslash \{ 0 \}$ , we say that n divides m, and write $n | m$ , if there exists a positive integer a such that $m = n a$ . Show that the set $\mathbf { N } \backslash \{ 0 \}$ with the ordering relation is a partially ordered set but not a totally ordered one. Note that this is a diferent ordering relation from the usual $\leq$ ordering of $\mathbf { N } \backslash \{ 0 \}$ 

Exercise 8.5.4. Show that the set of positive reals $\mathbf { R } ^ { + } : = \{ x \in \mathbf { R } : x > 0 \}$ have no minimal element. 

Exercise 8.5.5. Let $f : X \to Y$ be a function from one set X to another set $Y$ Suppose that Y is partially ordered with some ordering relation $\leq _ { Y }$ . Define a relation $\leq _ { X }$ on X by defining $x \leq _ { X } x ^ { \prime }$ if and only if $f ( x ) < _ { Y } f ( x ^ { \prime } )$ or $x = x ^ { \prime }$ Show that this relation $\leq _ { X }$ turns X into a partially ordered set. If we know in addition that the relation $\leq _ { Y }$ makes Y totally ordered, does this mean that the relation $\leq _ { X }$ makes X totally ordered also? If not, what additional assumption needs to be made on f in order to ensure that $\leq _ { X }$ makes X totally ordered? 

Exercise 8.5.6. Let X be a partially ordered set. For any x in $X ,$ , define the order ideal $( x ) \subset X$ to be the set $( x ) : = \{ y \in X : y \leq x \}$ . Let $( X ) : = \{ ( x ) : x \in$ $X \}$ be the set of all order ideals, and let $f : X \to ( X )$ be the map $f ( x ) : = ( x )$ that sends every element of x to its order ideal. Show that f is a bijection, and that given any $x , y \in X$ , that $x \le _ { X } y$ if and only if $f ( x ) \subseteq f ( y )$ . This exercise shows that any partially ordered set can be represented by a collection of sets whose ordering relation is given by set inclusion. 

Exercise 8.5.7. Let X be a partially ordered set, and let Y be a totally ordered subset of X. Show that $Y$ can have at most one maximum and at most one minimum. 

Exercise 8.5.8. Show that every finite non-empty subset of a totally ordered set has a minimum and a maximum. (Hint: use induction.) Conclude in particular that every finite totally ordered set is well-ordered. 

Exercise 8.5.9. Let X be a totally ordered set such that every non-empty subset of X has both a minimum and a maximum. Show that X is finite. (Hint: assume for sake of contradiction that X is infinite. Start with the minimal element $x _ { 0 }$ of X and then construct an increasing sequence $x _ { 0 } < x _ { 1 } < . . .$ . in $X . )$ 

Exercise 8.5.10. Prove Proposition 8.5.10, without using the axiom of choice. (Hint: consider the set 

$$
Y := \{n \in X: P (m) \text {   is   false   for   some   } m \in X \text {   with   } m \leq_ {X} n \},
$$

and show that Y being non-empty would lead to a contradiction.) 

Exercise 8.5.11. Let X be a partially ordered set, and let Y and $Y ^ { \prime }$ be wellordered subsets of X. Show that $Y \cup Y ^ { \prime }$ is well-ordered if and only if it is totally ordered. 

Exercise 8.5.12. Let X and Y be partially ordered sets with ordering relations $\leq _ { X }$ and $\leq _ { Y }$ respectively. Define a relation $\le _ { X \times Y }$ on the Cartesian product $X \times Y$ by defining $\left( x , y \right) \leq _ { X \times Y } \left( x ^ { \prime } , y ^ { \prime } \right)$ if $x < _ { X } x ^ { \prime } .$ , or if $x = x ^ { \prime }$ and $y \le _ { Y } y ^ { \prime }$ (This is called the lexicographical ordering on $X \times Y$ , and is similar to the alphabetical ordering of words; a word w appears earlier in a dictionary than another word $w ^ { \prime }$ if the first letter of w is earlier in the alphabet than the first letter of $w ^ { \prime }$ , or if the first letters match and the second letter of $w$ is earlier than the second letter of $w ^ { \prime }$ , and so forth.) Show that $\le x \times Y$ defines a partia ordering on $X \times Y$ . Furthermore, show that if X and $Y$ are totally ordered, then so is $X \times Y$ , and if X and $Y$ are well-ordered, then so is $X \times Y$ 

Exercise 8.5.13. Prove the claim in the proof of Lemma 8.5.14, namely that every element of $Y ^ { \prime } \backslash Y$ is an upper bound for $Y$ and vice versa. (Hint: Show using Proposition 8.5.10 that 

$$
\{y \in Y: y \leq a \} = \{y \in Y ^ {\prime}: y \leq a \} = \{y \in Y \cap Y ^ {\prime}: y \leq a \}
$$

for all $a \in Y \cap Y ^ { \prime }$ . Conclude that $Y \cap Y ^ { \prime }$ is good, and hence $s ( Y \cap Y ^ { \prime } )$ exists. Show that $s ( Y \cap Y ^ { \prime } ) = \operatorname* { m i n } ( Y ^ { \prime } \backslash Y )$ if $Y ^ { \prime } \backslash Y$ is non-empty, and similarly with $Y$ and $Y ^ { \prime }$ interchanged. Since $Y ^ { \prime } \backslash Y$ and $Y \backslash Y ^ { \prime }$ are disjoint, one can then conclude that one of these sets is empty, at which point the claim becomes easy to establish.) 

Exercise 8.5.14. Use Lemma 8.5.14 to prove Lemma 8.5.15. (Hint: first show that if X had no maximal elements, then any subset of X which has an upper bound, also has a strict upper bound.) 

Exercise 8.5.15. Let A and B be two non-empty sets such that A does not have lesser or equal cardinality to B. Using the principle of transfinite induction, prove that B has lesser or equal cardinality to $A .$ . (Hint: for every subset $X \subseteq B$ , let $P ( X )$ denote the property that there exists an injective map from X to A.) This exercise (combined with Exercise 8.3.3) shows that the cardinality of any two sets is comparable, as long as one assumes the axiom of choice. 

Exercise 8.5.16. Let X be a set, and let P be the set of all partial orderings of X. (For instance, if $X : = \mathbf { N } \backslash \{ 0 \}$ , then both the usual partial ordering $\leq$ and the partial ordering in Exercise 8.5.3, are elements of $P . )$ We say that one partial ordering $\le \in { \cal P }$ is coarser than another partial ordering $\leq ^ { \prime } \in \mathcal Ḋ P Ḍ$ if for any $x , y \in P$ , we have the implication $( x \leq y ) \implies ( x \leq ^ { \prime } y )$ . Thus for instance the partial ordering in Exercise 8.5.3 is coarser than the usual ordering $\leq$ . Let us write ${ \le } { \preceq } { \le } { ' } \ \mathrm { i f } \ { \le }$ is coarser than $\leq ^ { \prime }$ . Show that $\preceq$ turns $P$ into a partially ordered set; thus the set of partial orderings on X is itself partially ordered. There is exactly one minimal element of $P ;$ ; what is it? Show that the maximal elements of $P$ are precisely the total orderings of $P$ . Using Zorn’s lemma, show that given any partial ordering $\leq$ of X there exists a total ordering $\leq ^ { \prime }$ such that $\leq$ is coarser than $\leq ^ { \prime }$ 

Exercise 8.5.17. Use Zorn’s lemma to give another proof of the claim in Exercise 8.4.2. (Hint: let Ω be the set of all $Y \subseteq \cup _ { \alpha \in I } X _ { \alpha }$ such that $\# ( Y \cap X _ { \alpha } ) \leq 1$ for all $\alpha \in I$ , i.e., all sets which intersect each $X _ { \alpha }$ in at most one element. Use Zorn’s lemma to locate a maximal element of Ω.) Deduce that Zorn’s lemma and the axiom of choice are in fact logically equivalent (i.e., they can be deduced from each other). 

Exercise 8.5.18. Using Zorn’s lemma, prove Hausdorf’s maximality principle: if X is a partially ordered set, then there exists a totally ordered subset $Y$ of X which is maximal with respect to set inclusion (i.e. there is no other totally ordered subset $Y ^ { \prime }$ of $X$ which contains $Y$ . Conversely, show that if Hausdorf’s maximality principle is true, then Zorn’s lemma is true. Tthus by Exercise 8.5.17, these two statements are logically equivalent to the axiom of choice. 

Exercise 8.5.19. Let X be a set, and let Ω be the space of all pairs $( Y , \leq )$ where $Y$ is a subset of X and $\leq$ is a well-ordering of $Y$ . If $( Y , \leq )$ and $( Y ^ { \prime } , \leq ^ { \prime } )$ are elements of Ω, we say that $( Y , \leq )$ is an initial segment of $( Y ^ { \prime } , \leq ^ { \prime } )$ if there exists an $x \in Y ^ { \prime }$ such that $Y : = \{ y \in Y ^ { \prime } : y < ^ { \prime } x \}$ (so in particular $Y \subsetneq Y ^ { \prime } )$ and for any $y , y ^ { \prime } \in Y , y \leq y ^ { \prime }$ if and only if $y \le ^ { \prime } y ^ { \prime }$ . Define a relation on Ω by defining $( Y , \leq ) \preceq ( Y ^ { \prime } , \leq ^ { \prime } )$ if either $( Y , \leq ) = ( Y ^ { \prime } , \leq ^ { \prime } )$ , or if $( Y , \leq )$ is an initial segment of $( Y ^ { \prime } , \leq ^ { \prime } )$ . Show that $\preceq$ is a partial ordering of Ω. There is exactly one minimal element of $\Omega ;$ what is it? Show that the maximal elements of Ω are precisely the well-orderings $( X , \leq )$ of X. Using Zorn’s lemma, conclude the well ordering principle: every set X has at least one well-ordering. Conversely, use the well-ordering principle to prove the axiom of choice, Axiom 8.1. (Hint: place a well-ordering $\textstyle \leq \operatorname { o n } \bigcup _ { \alpha \in I } X _ { \alpha }$ , and then consider the minimal elements of each $X _ { \alpha } . )$ We thus see that the axiom of choice, Zorn’s lemma, and the well-ordering principle are all logically equivalent to each other. 

Exercise 8.5.20. Let X be a set, and let $\Omega \subset 2 ^ { X }$ be a collection of subsets of $X$ . Assume that $\Omega$ does not contain the empty set . Using Zorn’s lemma, show that there is a subcollection $\Omega ^ { \prime } \subseteq \Omega$ such that all the elements of $\Omega ^ { \prime }$ are disjoint from each other $( { \mathrm { i . e . , ~ } } A \cap B = \varnothing$ whenever A, B are distinct elements of $\Omega ^ { \prime } )$ , but that all the elements of Ω intersect at least one element of $\Omega ^ { \prime } ~ ( \mathrm { i . e . }$ for all $C \in \Omega$ there exists $A \in \Omega ^ { \prime }$ such that $C \cap A \neq \emptyset )$ . (Hint: consider al the subsets of Ω whose elements are all disjoint from each other, and locate a maximal element of this collection.) Conversely, if the above claim is true, show that it implies the claim in Exercise 8.4.2, and thus this is yet another claim which is logically equivalent to the axiom of choice. (Hint: let Ω be the set of all pair sets of the form $\{ ( 0 , \alpha ) , ( 1 , x _ { \alpha } ) \}$ , where $\alpha \in I$ and $x _ { \alpha } \in X _ { \alpha } . )$ 

## Chapter 9

## Continuous functions on R

In previous chapters we have been focusing primarily on sequences. A sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ can be viewed as a function from N to R, i.e., an object which assigns a real number $a _ { n }$ to each natural number n. We then did various things with these functions from N to R, such as take their limit at infinity (if the function was convergent), or form suprema, infima, etc., or computed the sum of all the elements in the sequence (again, assuming the series was convergent). 

Now we will look at functions not on the natural numbers N, which are “discrete”, but instead look at functions on a continuum<sup>1</sup> such as the real line R, or perhaps on an interval such as $\{ x \in \mathbf { R } : a \leq x \leq b \}$ Eventually we will perform a number of operations on these functions, including taking limits, computing derivatives, and evaluating integrals. In this chapter we will focus primarily on limits of functions, and on the closely related concept of a continuous function. 

Before we discuss functions, though, we must first set out some notation for subsets of the real line. 

## 9.1 Subsets of the real line

Very often in analysis we do not work on the whole real line R, but on certain subsets of the real line, such as the positive real axis $\{ x \in$ $\mathbf { R } : x > 0 \}$ . Also, we occasionally work with the extended real line $\mathbf { R } ^ { * }$ defined in Section 6.2, or in subsets of that extended real line. 

There are of course infinitely many subsets of the real line; indeed, Cantor’s theorem (Theorem 8.3.1; see also Exercise 8.3.4) shows that there are even more such sets than there are real numbers. However, there are certain special subsets of the real line (and the extended real line) which arise quite often. One such family of sets are the intervals. 

Definition 9.1.1 (Intervals). Let a, $b \in \mathbf { R } ^ { * }$ be extended real numbers. We define the closed interval [a, b] by 

$$
[ a, b ] := \{x \in \mathbf {R} ^ {*}: a \leq x \leq b \},
$$

the half-open intervals $[ a , b )$ and $( a , b ]$ by 

$$
[ a, b) := \{x \in \mathbf {R} ^ {*}: a \leq x <   b \}; (a, b ] := \{x \in \mathbf {R} ^ {*}: a <   x \leq b \},
$$

and the open intervals $( a , b )$ by 

$$
(a, b) := \{x \in \mathbf {R} ^ {*}: a <   x <   b \}.
$$

We call a the left endpoint of these intervals, and b the right endpoint. 

Remark 9.1.2. Once again, we are overloading the parenthesis notation; for instance, we are now using (2, 3) to denote both an open interval from 2 to 3, as well as an ordered pair in the Cartesian plane $\mathbf { R } ^ { 2 } : = \mathbf { R } \times \mathbf { R }$ . This can cause some genuine ambiguity, but the reader should still be able to resolve which meaning of the parentheses is intended from context. In some texts, this issue is resolved by using reversed brackets instead of parenthesis, thus for instance $[ a , b )$ would now be $[ a , b [ , ( a , b ]$ would be $] a , b ]$ , and $( a , b )$ would be $] a , b [$ 

Examples 9.1.3. If a and b are real numbers (i.e., not equal to + $\mathrm { o r } \mathrm { - } \infty )$ then all of the above intervals are subsets of the real line, for instance $[ 2 , 3 ) = \{ x \in \mathbf { R } : 2 \leq x < 3 \}$ . The positive real axis $\{ x \in$ $\mathbf { R } : x > 0 \}$ is the open interval $( 0 , + \infty )$ , while the non-negative real axis $\{ x \in \mathbf { R } : x \geq 0 \}$ is the half-open interval $[ 0 , + \infty )$ . Similarly, the negative real axis $\{ x \in \mathbf { R } : x < 0 \}$ is $( - \infty , 0 )$ , and the non-positive real axis $\{ x \in \mathbf { R } : x \leq 0 \}$ is $( - \infty , 0 ]$ . Finally, the real line R itself is the open interval $( - \infty , + \infty )$ , while the extended real line $\mathbf { R } ^ { * }$ is the closed interval $[ - \infty , + \infty ]$ . We sometimes refer to an interval in which one endpoint is infinite (either + or ) as half-infinite intervals, and intervals in which both endpoints are infinite as $d o u b l y  – i n f i n i t e$ intervals; all other intervals are bounded intervals. Thus [2, 3) is a bounded interval, the positive and negative real axes are half-infinite intervals, and R and $\mathbf { R } ^ { * }$ are infinite intervals. 

Example 9.1.4. If $a > b$ then all four of the intervals $[ a , b ] , [ a , b ) , ( a , b ]$ and $( a , b )$ are the empty set $\mathrm { \left( w h y ? \right) }$ . If $a = b ,$ , then the three intervals $[ a , b ) , ( a , b ]$ , and $( a , b )$ are the empty set, while $[ a , b ]$ is just the singleton set $\{ a \} ~ ( \mathrm { w h y ? } )$ . Because of this, we call these intervals degenerate; most (but not all) of our analysis will be restricted to non-degenerate intervals. 

Of course intervals are not the only interesting subsets of the real line. Other important examples include the natural numbers N, the integers Z, and the rationals Q. One can form additional sets using such operations as union and intersection (see Section 3.1), for instance one could have a disconnected union of two intervals such as $( 1 , 2 ) \cup [ 3 , 4 ]$ , or one could consider the set $[ - 1 , 1 ] \cap \mathbf { Q }$ of rational numbers between 1 and 1 inclusive. Clearly there are infinitely many possibilities of sets one could create by such operations. 

Just as sequences of real numbers have limit points, sets of real numbers have adherent points, which we now define. 

Definition 9.1.5 (ε-adherent points). Let X be a subset of R, let $\varepsilon > 0$ and let $x \in \mathbf { R }$ . We say that x is ε-adherent to X if there exists a $y \in X$ which is ε-close to x $( { \mathrm { i . e . , ~ } } | x - y | \leq \varepsilon )$ 

Remark 9.1.6. The terminology “ε-adherent” is not standard in the literature. However, we shall shortly use it to define the notion of an adherent point, which is standard. 

Example 9.1.7. The point 1.1 is 0.5-adherent to the open interval (0, 1), but is not 0.1-adherent to this interval (why?). The point 1.1 is 0.5-adherent to the finite set 1, 2, 3 . The point 1 is 0.5-adherent to $\{ 1 , 2 , 3 \} ~ ( \mathrm { w h y ? } )$ 

Definition 9.1.8 (Adherent points). Let X be a subset of R, and let $x \in \mathbf { R }$ . We say that x is an adherent point of X if it is ε-adherent to X for every $\varepsilon > 0$ 

Example 9.1.9. The number 1 is ε-adherent to the open interval (0, 1) for every $\varepsilon > 0 \mathrm { \ : \ : ( w h y ? ) }$ , and is thus an adherent point of $( 0 , 1 )$ . The point 0.5 is similarly an adherent point of (0, 1). However, the number 2 is not 0.5-adherent (for instance) to (0, 1), and is thus not an adherent point to (0, 1). 

Definition 9.1.10 (Closure). Let X be a subset of R. The closure of X, sometimes denoted X is defined to be the set of all the adherent points of X. 

Lemma 9.1.11 (Elementary properties of closures). Let X and Y be arbitrary subsets of R. Then $X \subseteq { \overline { { X } } } , { \overline { { X \cup Y } } } = { \overline { { X } } } \cup { \overline { { Y } } }$ , and ${ \overline { { X \cap Y } } } \subseteq$ $\overline { { X } } \cap \overline { { Y } }$ . If $X \subseteq Y$ , then ${ \overline { { X } } } \subseteq { \overline { { Y } } }$ 

Proof. See Exercise 9.1.2. 

We now compute some closures. 

Lemma 9.1.12 (Closures of intervals). Let $a < b$ be real numbers, and let I be any one of the four intervals $( a , b ) , ( a , b ] , [ a , b )$ , or $[ a , b ]$ . Then the closure of I is $[ a , b ]$ . Similarly, the closure of $( a , \infty )$ or $[ a , \infty )$ is $[ a , \infty )$ , while the closure of $( - \infty , a )$ or $( - \infty , a ]$ is $( - \infty , a ]$ . Finally, the closure of $( - \infty , \infty )$ is $( - \infty , \infty )$ 

Proof. We will just show one of these facts, namely that the closure of $( a , b )$ is $[ a , b ]$ ; the other results are proven similarly (or one can use Exercise 9.1.1). 

First let us show that every element of $[ a , b ]$ is adherent to $( a , b )$ . Let $x \in [ a , b ]$ . If $x \in ( a , b )$ then it is definitely adherent to $( a , b )$ . If $x = b$ then x is also adherent to $( a , b )$ (why?). Similarly when $x = a$ . Thus every point in $[ a , b ]$ is adherent to $( a , b )$ 

Now we show that every point x that is adherent to $( a , b )$ lies in $[ a , b ]$ Suppose for sake of contradiction that x does not lie in $[ a , b ]$ , then either $x > b$ or $x < a$ . If $x > b$ then x is not $( x - b )$ -adherent to $( a , b )$ (why?), and is hence not an adherent point to $( a , b )$ . Similarly, if $x < a$ , then x is not $( a - x )$ -adherent to $( a - b )$ , and is hence not an adherent point to $( a , b )$ . This contradiction shows that x is in fact in $[ a , b ]$ as claimed. 

Lemma 9.1.13. The closure of N is N. The closure of Z is Z. The closure $o f \mathbf { Q }$ is R, and the closure of R is R. The closure of the empty set is . 

Proof. See Exercise 9.1.3. 

The following lemma shows that adherent points of a set X can be obtained as the limit of elements in X: 

Lemma 9.1.14. Let X be a subset of R, and let $x \in \mathbf { R }$ . Then x is an adherent point of X if and only if there exists a sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ , consisting entirely of elements in X, which converges to x. 

Proof. See Exercise 9.1.5. 

Definition 9.1.15. A subset $E \subseteq \mathbf { R }$ is said to be closed if ${ \overline { { E } } } = E$ , or in other words that E contains all of its adherent points. 

Examples 9.1.16. From Lemma 9.1.12 we see that if $a < b$ are real numbers, then $[ a , b ] , [ a , + \infty ) , ( - \infty , a ]$ , and $( - \infty , + \infty )$ are closed, while $( a , b ) , ( a , b ] , [ a , b ) , ( a , + \infty )$ , and $( - \infty , a )$ are not. From Lemma 9.1.13 we see that N, Z, R, are closed, while Q is not. 

From Lemma 9.1.14 we can define closure in terms of sequences: 

Corollary 9.1.17. Let X be a subset of R. If X is closed, and $( a _ { n } ) _ { n = 0 } ^ { \infty }$ is a convergent sequence consisting of elements in X, then $\operatorname* { l i m } _ { n \to \infty } a _ { n }$ also lies in X. Conversely, if it is true that every convergent sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ of elements in X has its limit in X as well, then X is necessarily closed. 

When we study diferentiation in the next chapter, we shall need to replace the concept of an adherent point by the closely related notion of a limit point. 

Definition 9.1.18 (Limit points). Let X be a subset of the real line. We say that x is a limit point (or a cluster point) of X if it is an adherent point of $X \backslash \{ x \}$ . We say that x is an isolated point of X if $x \in X$ and there exists some $\varepsilon > 0$ such that $| x - y | > \varepsilon$ for all $y \in X \backslash \{ x \}$ 

Example 9.1.19. Let X be the set $X = ( 1 , 2 ) \cup \{ 3 \}$ . Then 3 is an adherent point of X, but it is not a limit point of X, since 3 is not adherent to $X - \{ 3 \} = ( 1 , 2 )$ ; instead, 3 is an isolated point of $X , \ \mathrm { O n }$ the other hand, 2 is still a limit point of X, since 2 is adherent to $X - \{ 2 \} = X$ ; but it is not isolated $\mathrm { \left( w h y ? \right) }$ 

Remark 9.1.20. From Lemma 9.1.14 we see that x is a limit point of X if there exists a sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ , consisting entirely of elements in X that are distinct from x, and such that $( a _ { n } ) _ { n = 0 } ^ { \infty }$ converges to x. It turns out that the set of adherent points splits into the set of limit points and the set of isolated points (Exercise 9.1.9). 

Lemma 9.1.21. Let I be an interval (possibly infinite), i.e., I is a set of the form $( a , b ) , ( a , b ] , [ a , b ) , [ a , b ] , ( a , + \infty ) , [ a , + \infty ) , ( - \infty , a )$ , or $( - \infty , a ]$ , with $a < b$ in the first four cases. Then every element of I is a limit point of I. 

Proof. We show this for the case $I = [ a , b ]$ ; the other cases are similar and are left to the reader. Let $x \in I ;$ we have to show that x is a limit point of I. There are three cases: $x = a , a < x < b .$ , and $x = b$ . If $x = a$ then consider the sequence $( x + { \frac { 1 } { n } } ) _ { n = N } ^ { \infty }$ . This sequence converges to x, and will lie inside $I - \{ a \} = ( a , \dot { b } ]$ if N is chosen large enough $\mathrm { \left( w h y ? \right) }$ Thus by Remark 9.1.20 we see that $x = a$ is a limit point of $[ a , b ]$ . A similar argument works when $a < x < b$ . When $x = b$ one has to use the sequence $\textstyle ( x - { \frac { 1 } { n } } ) _ { n = N } ^ { \infty }$ instead (why?) but the argument is otherwise the same. □ 

Next, we define the concept of a bounded set. 

Definition 9.1.22 (Bounded sets). A subset X of the real line is said to be bounded if we have $X \subset [ - M , M ]$ for some real number $M > 0$ 

Example 9.1.23. For any real numbers $a , b ,$ , the interval [a, b] is bounded, because it is contained inside $[ - M , M ]$ where $M : =$ max $( | a | , | b | )$ . However, the half-infinite interval $[ 0 , + \infty )$ is unbounded (why?). In fact, no half-infinite interval or doubly infinite interval can be bounded. The sets N, Z, Q, and R are all unbounded (why?). 

A basic property of closed and bounded sets is the following. 

Theorem 9.1.24 (Heine-Borel theorem for the line). Let X be a subset of R. Then the following two statements are equivalent: 

(a) X is closed and bounded. 

(b) Given any sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ of real numbers which takes values in X $( i . e . , a _ { n } \in X$ for all n), there exists a subsequence $( a _ { n _ { j } } ) _ { j = 0 } ^ { \infty }$ of the original sequence, which converges to some number L in X. 

Proof. See Exercise 9.1.13. 

Remark 9.1.25. This theorem shall play a key rˆole in subsequent sections of this chapter. In the language of metric space topology, it asserts that every subset of the real line which is closed and bounded, is also compact; see Section 11.7. A more general version of this theorem, due to Eduard Heine (1821–1881) and Emile Borel (1871–1956), can be found in Theorem 11.7.7. 

## — Exercises —

Exercise 9.1.1. Let X be any subset of the real line, and let Y be a set such that $X \subseteq Y \subseteq { \overline { { X } } }$ . Show that ${ \overline { { Y } } } = { \overline { { X } } }$ 

Exercise 9.1.2. Prove Lemma 9.1.11. 

Exercise 9.1.3. Prove Lemma 9.1.13. (Hint: for computing the closure of $\mathbf { Q } .$ you will need Proposition 5.4.14.) 

Exercise 9.1.4. Give an example of two subsets X, Y of the real line such that ${ \overline { { X \cap Y } } } \neq { \overline { { X } } } \cap { \overline { { Y } } }$ 

Exercise 9.1.5. Prove Lemma 9.1.14. (Hint: in order to prove one of the two implications here you will need axiom of choice, as in Lemma 8.4.5.) 

Exercise 9.1.6. Let X be a subset of R. Show that $\overline { { X } }$ is closed $( \mathrm { i . e . , } \overline { { X } } = \overline { { X } } )$ Furthermore, show that if Y is any closed set that contains X, then Y also contains X. Thus the closure X of X is the smallest closed set which contains X. 

Exercise 9.1.7. Let $n \geq 1$ be a positive integer, and let $X _ { 1 } , \ldots , X _ { n }$ be closed subsets of R. Show that $X _ { 1 } \cup X _ { 2 } \cup . . . \cup X _ { n }$ is also closed. 

Exercise 9.1.8. Let I be a set (possibly infinite), and for each $\alpha \in I$ let $X _ { \alpha }$ be a closed subset of R. Show that the intersection $\cap _ { \alpha \in I } X _ { \alpha }$ (defined in (3.3)) is also closed. 

Exercise 9.1.9. Let X be a subset of the real line, and x be a real number. Show that every adherent point of X is either a limit point or an isolated point of X, but cannot be both. Conversely, show that every limit point and every isolated point of X is an adherent point of X. 

Exercise 9.1.10. If X is a non-empty subset of R, show that X is bounded if and only if inf(X) and sup(X) are finite. 

Exercise 9.1.11. Show that if X is a bounded subset of R, then the closure X is also bounded. 

Exercise 9.1.12. Show that the union of any finite collection of bounded subsets of R is still a bounded set. Is this conclusion still true if one takes an infinite collection of bounded subsets of R? 

Exercise 9.1.13. Prove Theorem 9.1.24. (Hint: to show (a) implies (b), use the Bolzano-Weierstrass theorem (Theorem 6.6.8) and Corollary 9.1.17. To show (b) implies (a), argue by contradiction, using Corollary 9.1.17 to establish that X is closed. You will need the axiom of choice to show that X is bounded, as in Lemma 8.4.5.) 

Exercise 9.1.14. Show that any finite subset of R is closed and bounded. 

Exercise 9.1.15. Let E be a bounded subset of R, and let $S : = \operatorname* { s u p } ( E )$ be the least upper bound of E. (Note from the least upper bound principle, Theorem 5.5.9, that S is a real number.) Show that S is an adherent point of E, and is also an adherent point of $\mathbf { R } \backslash E$ 

## 9.2 The algebra of real-valued functions

You are familiar with many functions $f : \mathbf { R }  \mathbf { R }$ from the real line to the real line. Some examples are: $f ( x ) : = x ^ { 2 } + 3 x + 5 ; f ( x ) : = 2 ^ { x } / ( x ^ { 2 } + 1 )$ ; 

$f ( x ) : = \sin ( x ) \exp ( x )$ (we will define sin and exp formally in Chapter 11.20). These are functions from R to R since to every real number x they assign a single real number $f ( x )$ . We can also consider more exotic functions, e.g. 

$$
f (x) := \left\{ \begin{array}{l l} 1 & \text { if } x \in \mathbf {Q} \\ 0 & \text { if } x \not \in \mathbf {Q}. \end{array} \right.
$$

This function is not algebraic (i.e., it cannot be expressed in terms of x purely by using the standard algebraic operations of $+ , - , \times , / , \surd ,$ etc.; we will not need this notion in this text), but it is still a function from R to R, because it still assigns a real number $f ( x )$ to each $x \in \mathbf { R }$ 

We can take any one of the previous functions $f : \mathbf { R }  \mathbf { R }$ defined on all of R, and restrict the domain to a smaller set $X \subseteq \mathbf { R }$ , creating a new function, sometimes called $f | _ { X }$ , from X to R. This is the same function as the original function $f ,$ , but is only defined on a smaller domain. (Thus $f | _ { X } ( x ) : = f ( x )$ when $x \in X$ , and $f | _ { X } ( x )$ is undefined when $x \notin X . )$ For instance, we can restrict the function $f ( x ) : = x ^ { 2 }$ , which is initially defined from R to R, to the interval [1, 2], thus creating a new function $f | _ { [ 1 , 2 ] } : [ 1 , 2 ] \to \mathbf { R }$ , which is defined as $f | _ { [ 1 , 2 ] } ( x ) = x ^ { 2 }$ when $x \in [ 1 , 2 ]$ but is undefined elsewhere. 

One could also restrict the range from R to some smaller subset $Y$ of R, provided of course that all the values of $f ( x )$ lie inside $Y$ . For instance, the function $f : \mathbf { R }  \mathbf { R }$ defined by $f ( x ) : = x ^ { 2 }$ could also be thought of as a function from R to $[ 0 , \infty )$ , instead of a function from R to R. Formally, these two functions are diferent functions, but the distinction between them is so minor that we shall often be careless about the range of a function in our discussion. 

Strictly speaking, there is a distinction between a function $f ,$ and its value $f ( x )$ at a point x. f is a function; but $f ( x )$ is a number (which depends on some free variable $x )$ . This distinction is rather subtle and we will not stress it too much, but there are times when one has to distinguish between the two. For instance, if $f : \mathbf { R }  \mathbf { R }$ is the function $f ( x ) : = x ^ { 2 }$ , and $g : = f | _ { [ 1 , 2 ] }$ is the restriction of f to the interval $[ 1 , 2 ]$ then f and g both perform the operation of squaring, i.e., $f ( x ) = x ^ { 2 }$ and $g ( x ) = x ^ { 2 }$ , but the two functions $f$ and $g$ are not considered the same function, $f \neq g$ , because they have diferent domains. Despite this distinction, we shall often be careless, and say things like “consider the function $x ^ { 2 } + 2 x + 3 ^ { \prime \prime }$ when really we should be saying “consider the function $f : \mathbf { R }  \mathbf { R }$ defined by $f ( x ) : = x ^ { 2 } + 2 x + 3 ^ { \mathfrak { V } }$ . (This distinction makes more of a diference when we start doing things like diferentiation. 

For instance, if $f : \mathbf { R }  \mathbf { R }$ is the function $f ( x ) = x ^ { 2 }$ , then of course $f ( 3 ) = 9$ , but the derivative of $f$ at 3 is 6, whereas the derivative of 9 is of course 0, so we cannot simply “diferentiate both sides” of $f ( 3 ) = 9$ and conclude that $6 = 0 . )$ 

If X is a subset of R, and $f : X  \mathbf { R }$ is a function, we can form the graph $\{ ( x , f ( x ) ) : x \in X \}$ of the function $f ;$ this is a subset of $X \times \mathbf { R }$ , and hence a subset of the Euclidean plane $\mathbf { R } ^ { 2 } = \mathbf { R } \times \mathbf { R }$ . One can certainly study a function through its graph, by using the geometry of the plane $\mathbf { R } ^ { 2 } \ ( \mathrm { e . g . }$ , employing such concepts as tangent lines, area, and so forth). We however will pursue a more “analytic” approach, in which we rely instead on the properties of the real numbers to analyze these functions. The two approaches are complementary; the geometric approach ofers more visual intuition, while the analytic approach ofers rigour and precision. Both the geometric intuition and the analytic formalism become useful when extending analysis of functions of one variable to functions of many variables (or possibly even infinitely many variables). 

Just as numbers can be manipulated arithmetically, so can functions: the sum of two functions is a function, the product of two functions is a function, and so forth. 

Definition 9.2.1 (Arithmetic operations on functions). Given two functions $f : X  \mathbf { R }$ and $g : X  \mathbf { R }$ , we can define their sum $f + g : X \to \mathbf { R }$ by the formula 

$$
(f + g) (x) := f (x) + g (x),
$$

their diference $f - g : X \to \mathbf { R }$ by the formula 

$$
(f - g) (x) := f (x) - g (x),
$$

their maximum max $( f , g ) : X \to \mathbf { R }$ by 

$$
\max (f, g) (x) := \max (f (x), g (x)),
$$

their minimum min $( f , g ) : X \to \mathbf { R }$ by 

$$
\min (f, g) (x) := \min (f (x), g (x)),
$$

their product $f g : X \to \mathbf { R } ( \operatorname { o r } f \cdot g : X \to \mathbf { R } )$ by the formula 

$$
(f g) (x) := f (x) g (x),
$$

and (provided that $g ( x ) \neq 0$ for all $x \in X )$ the quotient $f / g : X \to \mathbf { R }$ by the formula 

$$
(f / g) (x) := f (x) / g (x).
$$

Finally, if c is a real number, we can define the function $c f : X \to \mathbf { R }$ (or $c \cdot f : X \to \mathbf { R } )$ by the formula 

$$
(c f) (x) := c \times f (x).
$$

Example 9.2.2. If $f : \mathbf { R }  \mathbf { R }$ is the function $f ( x ) \ : = \ x ^ { 2 }$ , and $_ { \textit { g } : }$ $\mathbf R \to \mathbf R$ is the function $g ( x ) : = 2 x$ , then $f + g : \mathbf { R }  \mathbf { R }$ is the function $( f + g ) ( x ) : = x ^ { 2 } + 2 x$ , while $f g : \mathbf { R }  \mathbf { R }$ is the function $f g ( x ) = 2 x ^ { 3 }$ Similarly $f - g : \mathbf { R }  \mathbf { R }$ is the function $( f - g ) ( x ) : = x ^ { 2 } - 2 x$ , while $6 f : \mathbf { R }  \mathbf { R }$ is the function $( 6 f ) ( x ) = 6 x ^ { 2 }$ Observe that $f g$ is not the same function as $f \circ g .$ , which maps $x \mapsto 4 x ^ { 2 }$ , nor is it the same as $g \circ f$ , which maps $x \mapsto 2 x ^ { 2 } \ \mathrm { ( w h y ? ) }$ . Thus multiplication of functions and composition of functions are two diferent operations. 

## — Exercises —

Exercise 9.2.1. Let $f : \mathbf { R }  \mathbf { R } , g : \mathbf { R }  \mathbf { R } , h : \mathbf { R }  \mathbf { R }$ . Which of the following identities are true, and which ones are false? In the former case, give a proof; in the latter case, give a counterexample. 

$$
\begin{array}{c} (f + g) \circ h = (f \circ h) + (g \circ h) \\ f \circ (g + h) = (f \circ g) + (f \circ h) \\ (f + g) \cdot h = (f \cdot h) + (g \cdot h) \\ f \cdot (g + h) = (f \cdot g) + (f \cdot h) \end{array}
$$

## 9.3 Limiting values of functions

In Chapter 6 we defined what it means for a sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ to converge to a limit L. We now define a similar notion for what it means for a function f defined on the real line, or on some subset of the real line, to converge to some value at a point. Just as we used the notions of ε-closeness and eventual ε-closeness to deal with limits of sequences, we shall need a notion of ε-closeness and local ε-closeness to deal with limits of functions. 

Definition 9.3.1 (ε-closeness). Let X be a subset of R, let $f : X  \mathbf { R }$ be a function, let L be a real number, and let $\varepsilon > 0$ be a real number. We say that the function f is ε-close to L if $f ( x )$ is ε-close to L for every $x \in X$ 

Example 9.3.2. When the function $f ( x ) \ : = \ x ^ { 2 }$ is restricted to the interval [1, 3], then it is 5-close to 4, since when $x \in [ 1 , 3 ]$ then $1 \ \leq$ $f ( x ) \leq 9$ , and hence $| f ( x ) - 4 | \leq 5$ . When instead it is restricted to the smaller interval $[ 1 . 9 , 2 . 1 ]$ , then it is 0.41-close to 4, since if $x \in [ 1 . 9 , 2 . 1 ]$ then $3 . 6 1 \leq f ( x ) \leq 4 . 4 1$ , and hence $| f ( x ) - 4 | \leq 0 . 4 1$ 

Definition 9.3.3 (Local ε-closeness). Let X be a subset of R, let $f$ : $X  \mathbf { R }$ be a function, let L be a real number, $x _ { 0 }$ be an adherent point of X, and $\varepsilon > 0$ be a real number. We say that f is ε-close to L near x if there exists a $\delta > 0$ such that $f$ becomes ε-close to L when restricted to the set $\{ x \in X : | x - x _ { 0 } | < \delta \}$ 

Example 9.3.4. Let $f : [ 1 , 3 ] \to \mathbf { R }$ be the function $f ( x ) : = x ^ { 2 }$ , restricted to the interval [1, 3]. This function is not 0.1-close to 4, since for instance $f ( 1 )$ is not 0.1-close to 4. However, f is 0.1-close to 4 near $2 ,$ since when restricted to the set $\{ x \in [ 1 , 3 ] : | x - 2 | < 0 . 0 1 \}$ , the function f is indeed 0.1-close to 4. This is because when $| x - 2 | < 0 . 0 1$ , we have $1 . 9 9 < x < 2 . 0 1$ , and hence $3 . 9 6 0 1 < f ( x ) < 4 . 0 4 0 1$ , and in particular $f ( x )$ is 0.1-close to 4. 

Example 9.3.5. Continuing with the same function f used in the previous example, we observe that $f$ is not 0.1-close to 9, since for instance $f ( 1 )$ is not 0.1-close to 9. However, f is 0.1-close to 9 near 3, since when restricted to the set $\{ x \in [ 1 , 3 ] : | x - 3 | < 0 . 0 1 \}$ - which is the same as the half-open interval (2.99, 3] (why?), the function $f$ becomes 0.1-close to 9 (since if $2 . 9 9 < x \le 3$ , then $8 . 9 4 0 1 < f ( x ) \le 9$ , and hence $f ( x )$ is 0.1-close to 9). 

Definition 9.3.6 (Convergence of functions at a point). Let X be a subset of R, let $f : X \to \mathbf { R }$ be a function, let E be a subset of $X , x _ { 0 }$ be an adherent point of E, and let L be a real number. We say that f converges to L at $x _ { 0 }$ in E, and write lim $\quad _ { x \to x _ { 0 } ; x \in E } f ( x ) = L$ , if $f ,$ after restricting to $E _ { i }$ , is ε-close to $L$ near $x _ { 0 }$ for every $\varepsilon > 0$ . If f does not converge to any number $L$ at $x _ { 0 }$ , we say that f diverges at $x _ { 0 }$ , and leave $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in E } f ( x )$ undefined. 

In other words, we have $\begin{array} { r } { \operatorname* { l i m } _ { x  x _ { 0 } ; x \in E } f ( x ) = L } \end{array}$ if for every $\varepsilon > 0$ 4 there exists a $\delta > 0$ such that $| f ( x ) - L | \leq \varepsilon$ for all $x \in E$ such that $| x - x _ { 0 } | < \delta$ . (Why is this definition equivalent to the one given above?) 

Remark 9.3.7. In many cases we will omit the set E from the above notation (i.e., we will just say that f converges to L at $x _ { 0 }$ , or that $\begin{array} { r } { \operatorname* { l i m } _ { x  x _ { 0 } } f ( x ) = L ) } \end{array}$ , although this is slightly dangerous. For instance, it sometimes makes a diference whether E actually contains $x _ { 0 }$ or not. To give an example, if $f : \textbf { R } \to \textbf { R }$ is the function defined by setting $f ( x ) ~ = ~ 1$ when $x \ = \ 0$ and $f ( x ) ~ = ~ 0$ when $x \neq 0$ , then one has $\textstyle \operatorname* { l i m } _ { x \to 0 ; x \in \mathbf { R } \backslash \left\{ 0 \right\} } f ( x ) = 0 ,$ , but $\scriptstyle \operatorname* { l i m } _ { x \to 0 ; x \in \mathbf { R } } f ( x )$ is undefined. Some authors only define the limit $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in E } f ( x )$ when $E$ does not contain $x _ { 0 }$ (so that $x _ { 0 }$ is now a limit point of E rather than an adherent point), or would use $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in E } f ( x )$ to denote what we would cal $\begin{array} { r } { \operatorname* { l i m } _ { x \in x _ { 0 } ; x \in E \backslash \{ x _ { 0 } \} } f ( x ) } \end{array}$ , but we have chosen a slightly more general notation, which allows the possibility that E contains $x _ { 0 }$ 

Example 9.3.8. Let $f : [ 1 , 3 ] \to \mathbf { R }$ be the function $f ( x ) : = x ^ { 2 }$ . We have seen before that f is 0.1-close to 4 near 2. A similar argument shows that f is 0.01-close to 4 near 2 (one just has to pick a smaller value of δ). 

Definition 9.3.6 is rather unwieldy. However, we can rewrite this definition in terms of a more familiar one, involving limits of sequences. 

Proposition 9.3.9. Let X be a subset of R, let $f : X \to \mathbf { R }$ be $a$ function, let E be a subset of X, let $x _ { 0 }$ be an adherent point of E, and let L be a real number. Then the following two statements are logically equivalent: 

(a) f converges to L at $x _ { 0 }$ in $E$ . 

(b) For every sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ which consists entirely of elements of E and converges to $x _ { 0 }$ , the sequence $( f ( a _ { n } ) ) _ { n = 0 } ^ { \infty }$ converges to $L$ 

Proof. See Exercise 9.3.1. 

In view of the above proposition, we will sometimes write ${ } ^ { \ 6 } f ( x ) \to L$ as $x  x _ { 0 }$ in $E ^ { \ast }$ or $^ { 6 6 } f$ has a limit L at $x _ { 0 }$ in $E ^ { \ast }$ instead of $^ { 6 6 } f$ converges to L at ${ x _ { 0 } } ^ { , , } , { \mathrm { o r } } \ { } ^ { \ast } { \mathrm { l i m } } _ { x \to x _ { 0 } } f ( x ) = L ^ { , }$ 

Remark 9.3.10. With the notation of Proposition 9.3.9, we have the following corollary: if $\begin{array} { r } { \operatorname* { l i m } _ { x  x _ { 0 } ; x \in E } f ( x ) = L } \end{array}$ , and $\scriptstyle \operatorname* { l i m } _ { n \to \infty } a _ { n } = x _ { 0 }$ , then $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } f ( a _ { n } ) = L } \end{array}$ 

Remark 9.3.11. We only consider limits of a function f at $x _ { 0 }$ in the case when $x _ { 0 }$ is an adherent point of $E .$ . When $x _ { 0 }$ is not an adherent point then it is not worth it to define the concept of a limit. (Can you see why there will be problems?) 

Remark 9.3.12. The variable x used to denote a limit is a dummy variable; we could replace it by any other variable and obtain exactly the same limit. For instance, if $\textstyle \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in E } f ( x ) \ = \ L$ , then $\begin{array} { r } { \operatorname* { l i m } _ { y  x _ { 0 } ; y \in E } f ( y ) = L } \end{array}$ , and conversely (why?). 

Proposition 9.3.9 has some immediate corollaries. For instance, we now know that a function can have at most one limit at each point: 

Corollary 9.3.13. Let X be a subset of R, let E be a subset of $X$ , let $x _ { 0 }$ be an adherent point of $E _ { \perp }$ , and let $f : X \to \mathbf { R }$ be a function. Then f can have at most one limit at $x _ { 0 }$ in $E$ . 

Proof. Suppose for sake of contradiction that there are two distinct numbers $L$ and $L ^ { \prime }$ such that $f$ has a limit $L$ at $x _ { 0 }$ in $E$ , and such that $f$ also has a limit $L ^ { \prime }$ at $x _ { 0 }$ in $E .$ . Since $x _ { 0 }$ is an adherent point of $E .$ , we know by Lemma 9.1.14 that there is a sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ consisting of elements in $E$ which converges to $x _ { 0 }$ . Since f has a limit $L$ at $x _ { 0 }$ in $E$ , we thus see by Proposition 9.3.9, that $( f ( a _ { n } ) ) _ { n = 0 } ^ { \infty }$ converges to $L .$ . But since $f$ also has a limit $L ^ { \prime }$ at $x _ { 0 }$ in $E _ { i }$ , we see that $( f ( a _ { n } ) ) _ { n = 0 } ^ { \infty }$ also converges to $L ^ { \prime }$ But this contradicts the uniqueness of limits of sequences (Proposition 6.1.7). □ 

Using the limit laws for sequences, one can now deduce the limit laws for functions: 

Proposition 9.3.14 (Limit laws for functions). Let X be a subset of R, let $E$ be a subset of X, let $x _ { 0 }$ be an adherent point of $E ,$ , and let $f : X  \mathbf { R }$ and $g : X  \mathbf { R }$ be functions. Suppose that f has a limit $L$ at x in $E ,$ and g has a limit M at $x _ { 0 }$ in E. Then $f + g$ has a limit $L + M$ at $x _ { 0 }$ in $E , f - g$ has a limit $L - M$ at $x _ { 0 }$ in $E ,$ max $( f , g )$ has a limit max(L, M) at $x _ { 0 }$ in $E _ { i }$ , min $( f , g )$ has a limit min(L, M) at $x _ { 0 }$ in E and fg has a limit LM at x in E. If c is a real number, then cf has a limit cL at $x _ { 0 }$ in E. Finally, if g is non-zero on E $( i . e . , g ( x ) \neq 0$ for all $x \in E )$ and M is non-zero, then $f / g$ has a limit $L / M$ at x in E. 

Proof. We just prove the first claim (that $f + g$ has a limit $L + M )$ ; the others are very similar and are left to Exercise 9.3.2. Since $x _ { 0 }$ is an adherent point of $E _ { \mathrm { { i } } }$ , we know by Lemma 9.1.14 that there is a sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ consisting of elements in $E ,$ which converges to $x _ { 0 }$ . Since f has a limit $L$ at $x _ { 0 }$ in $E _ { i }$ , we thus see by Proposition 9.3.9, that $( f ( a _ { n } ) ) _ { n = 0 } ^ { \infty }$ converges to $L$ . Similarly $( g ( a _ { n } ) ) _ { n = 0 } ^ { \infty }$ converges to M. By the limit laws for sequences (Theorem 6.1.19) we conclude that $( ( f + g ) ( a _ { n } ) ) _ { n = 0 } ^ { \infty }$ converges to $L + M$ . By Proposition 9.3.9 again, this implies that $f + g$ has a limit $L + M$ at $x _ { 0 }$ in $E$ as desired (since $( a _ { n } ) _ { n = 0 } ^ { \infty }$ was an arbitrary sequence in E converging to $x _ { 0 } )$ □ 

Remark 9.3.15. One can phrase Proposition 9.3.14 more informally as saying that 

$$
\begin{array}{c} \lim _ {x \to x _ {0}} (f \pm g) (x) = \lim _ {x \to x _ {0}} f (x) \pm \lim _ {x \to x _ {0}} g (x) \\ \lim _ {x \to x _ {0}} \max (f, g) (x) = \max \left(\lim _ {x \to x _ {0}} f (x), \lim _ {x \to x _ {0}} g (x)\right) \\ \lim _ {x \to x _ {0}} \min (f, g) (x) = \min \left(\lim _ {x \to x _ {0}} f (x), \lim _ {x \to x _ {0}} g (x)\right) \\ \lim _ {x \to x _ {0}} (f g) (x) = \lim _ {x \to x _ {0}} f (x) \lim _ {x \to x _ {0}} g (x) \\ \lim _ {x \to x _ {0}} (f / g) (x) = \frac {\lim _ {x \to x _ {0}} f (x)}{\lim _ {x \to x _ {0}} g (x)} \end{array}
$$

(where we have dropped the restriction $x \in E$ for brevity) but bear in mind that these identities are only true when the right-hand side makes sense, and furthermore for the final identity we need g to be nonzero, and also $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } } g ( x )$ to be non-zero. (See Example 1.2.4 for some examples of what goes wrong when limits are manipulated carelessly.) 

Using the limit laws in Proposition 9.3.14 we can already deduce several limits. First of all, it is easy to check the basic limits 

$$
\lim _ {x \to x _ {0}; x \in \mathbf {R}} c = c
$$

and 

$$
\lim _ {x \to x _ {0}; x \in \mathbf {R}} x = x _ {0}
$$

for any real numbers $x _ { 0 }$ and $c .$ (Why? use Proposition 9.3.9.) By the limit laws we can thus conclude that 

$$
\begin{array}{c} \lim _ {x \to x _ {0}; x \in \mathbf {R}} x ^ {2} = x _ {0} ^ {2} \\ \lim _ {x \to x _ {0}; x \in \mathbf {R}} c x = c x _ {0} \\ \lim _ {x \to x _ {0}; x \in \mathbf {R}} x ^ {2} + c x + d = x _ {0} ^ {2} + c x _ {0} + d \end{array}
$$

e $\displaystyle \langle \mathbf { c } . ,$ where $c , d$ are arbitrary real numbers. 

## 9.3. Limiting values of functions

If f converges to $L$ at $x _ { 0 }$ in $X$ , and Y is any subset of X such that $x _ { 0 }$ is still an adherent point of $Y$ , then f will also converge to $L$ at $x _ { 0 }$ in $Y \ \mathrm { \left( w h y ? \right) }$ . Thus convergence on a large set implies convergence on a smaller set. The converse, however, is not true: 

Example 9.3.16. Consider the signum function sgn : $\mathbf R  \mathbf R$ , defined by 

$$
\operatorname{sgn} (x) := \left\{ \begin{array}{l l} 1 & \text {if x > 0} \\ 0 & \text {if x = 0} \\ - 1 & \text {if x <   0} \end{array} \right.
$$

Then $\begin{array} { r } { \operatorname* { l i m } _ { x  0 ; x \in ( 0 , \infty ) } \mathrm { s g n } ( x ) = 1 \ \mathrm { ( w h y ? ) } } \end{array}$ , whereas $\scriptstyle \operatorname* { l i m } _ { x \to 0 ; x \in ( - \infty , 0 ) } = - 1$ $\mathrm { \left( w h y ? \right) }$ and $\scriptstyle \operatorname* { l i m } _ { x \to 0 ; x \in \mathbf { R } } \operatorname { s g n } ( x )$ is undefined $\mathrm { ( w h y ? ) }$ . Thus it is sometimes dangerous to drop the set X from the notation of limit. However, in many cases it is safe to do so; for instance, since we know that $\begin{array} { r } { \operatorname* { l i m } _ { x  x _ { 0 } ; x \in \mathbf { R } } x ^ { 2 } = x _ { 0 } ^ { 2 } } \end{array}$ , we know in fact that $\begin{array} { r } { \operatorname* { l i m } _ { x \in x _ { 0 } ; x \in X } x ^ { 2 } = x _ { 0 } ^ { 2 } } \end{array}$ for any set X with $x _ { 0 }$ as an adherent point (why?). Thus it is safe to write $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } } x ^ { 2 } = x _ { 0 } ^ { 2 }$ 

Example 9.3.17. Let $f ( x )$ be the function 

$$
f (x) := \left\{ \begin{array}{l l} 1 & \text { if } x = 0 \\ 0 & \text { if } x \neq 0. \end{array} \right.
$$

Then $\begin{array} { r } { \operatorname* { l i m } _ { x  0 ; x \in \mathbf { R } - \{ 0 \} } f ( x ) = 0 \ \mathrm { ( w h y ? ) } } \end{array}$ , but $\scriptstyle \operatorname* { l i m } _ { x \to 0 ; x \in \mathbf { R } } f ( x )$ is undefined (why). (When this happens, we say that f has a “removable singularity” or “removable discontinuity” at 0. Because of such singularities, it is sometimes the convention when writing $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } } f ( x )$ to automatically exclude $x _ { 0 }$ from the set; for instance, in the textbook, $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } } f ( x )$ is used as shorthand for $\begin{array} { r } { \operatorname* { l i m } _ { x  x _ { 0 } ; x \in X - \{ x _ { 0 } \} } f ( x ) . ) } \end{array}$ 

On the other hand, the limit at $x _ { 0 }$ should only depend on the values of the function near $x _ { 0 } ;$ the values away from $x _ { 0 }$ are not relevant. The following proposition reflects this intuition: 

Proposition 9.3.18 (Limits are local). Let X be a subset of R, let E be a subset of X, let $x _ { 0 }$ be an adherent point of $E$ , let $f : X  \mathbf { R }$ be a function, and let L be a real number. Let $\delta > 0$ . Then we have 

$$
\lim _ {x \to x _ {0}; x \in E} f (x) = L
$$

if and only if 

$$
\lim _ {x \to x _ {0}; x \in E \cap (x _ {0} - \delta , x _ {0} + \delta)} f (x) = L.
$$

Proof. See Exercise 9.3.3. 

Informally, the above proposition asserts that 

$$
\lim _ {x \to x _ {0}; x \in E} f (x) = \lim _ {x \to x _ {0}; x \in E \cap (x _ {0} - \delta , x _ {0} + \delta)} f (x).
$$

Thus the limit of a function at $x _ { 0 }$ , if it exists, only depends on the values of f near $x _ { 0 } ;$ the values far away do not actually influence the limit. 

We now give a few more examples of limits. 

Example 9.3.19. Consider the functions $f : \mathbf { R }  \mathbf { R }$ and $g : \mathbf { R }  \mathbf { R }$ defined by $f ( x ) : = x + 2$ and $g ( x ) : = x + 1$ . Then $\textstyle \operatorname* { l i m } _ { x \to 2 ; x \in \mathbf { R } } f ( x ) = 4$ and $\scriptstyle \operatorname* { l i m } _ { x \to 2 ; x \in \mathbf { R } } g ( x ) \ = \ 3$ We would like to use the limit laws to conclude that l $\mathrm { m } _ { x \to 2 ; x \in { \bf R } } f ( x ) / g ( x ) \ = \ 4 / 3$ , or in other words that $\begin{array} { r } { \operatorname* { l i m } _ { x  2 ; x \in \mathbf { R } } \frac { x + 2 } { x + 1 } = \frac { 4 } { 3 } } \end{array}$ . Strictly speaking, we cannot use Proposition 9.3.14 to ensure this, because $x + 1$ is zero at $x = - 1$ , and so $f ( x ) / g ( x )$ is not defined. However, this is easily solved, by restricting the domain of f and g from R to a smaller domain, such as $\mathbf { R } - \{ 1 \}$ . Then Proposition 9.3.14 does apply, and we have $\begin{array} { r } { \operatorname* { l i m } _ { x  2 ; x \in { \bf R } - \{ 1 \} } \frac { x + 2 } { x + 1 } = \frac { 4 } { 3 } } \end{array}$ 

Example 9.3.20. Consider the function $f : \mathbf { R } - \{ 1 \} \  \ \mathbf { R }$ defined by $f ( x ) : = ( x ^ { 2 } - 1 ) / ( x - 1 )$ . This function is well-defined for every real number except 1, so f(1) is undefined. However, 1 is still an adherent point of $\mathbf { R } - \{ 1 \} ~ \mathrm { ( w h y ? ) }$ , and the limit $\begin{array} { r } { \operatorname* { l i m } _ { x  1 ; x \in \mathbf { R } - \{ 1 \} } f ( x ) } \end{array}$ is still defined. This is because on the domain $\mathbf { R } - \{ 1 \}$ we have the identity $( x ^ { 2 } - 1 ) / ( x - 1 ) \ = \ ( x + 1 ) ( x - 1 ) / ( x - 1 ) \ = \ x + 1$ , and $\begin{array} { r } { \operatorname* { l i m } _ { x  1 ; x \in \mathbf { R } - \{ 1 \} } x + 1 = 2 . } \end{array}$ 

Example 9.3.21. Let $f : \mathbf { R }  \mathbf { R }$ be the function 

$$
f (x) := \left\{ \begin{array}{l l} 1 & \text { if } x \in \mathbf {Q} \\ 0 & \text { if } x \not \in \mathbf {Q}. \end{array} \right.
$$

We will show that $f ( x )$ has no limit at 0 in R. Suppose for sake of contradiction that $f ( x )$ had some limit L at 0 in R. Then we would have $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } f ( a _ { n } ) \ = \ L } \end{array}$ whenever $( a _ { n } ) _ { n = 0 } ^ { \infty }$ is a sequence of non-zero numbers converging to 0. Since $( 1 / n ) _ { n = 0 } ^ { \infty }$ is such a sequence, we would have 

$$
L = \lim _ {n \to \infty} f (1 / n) = \lim _ {n \to \infty} 1 = 1.
$$

On the other hand, since $( \sqrt { 2 } / n ) _ { n = 0 } ^ { \infty }$ is another sequence of non-zero numbers converging to 0 - but now these numbers are irrational instead 

## 9.4. Continuous functions

of rational - we have 

$$
L = \lim _ {n \to \infty} f (\sqrt {2} / n) = \lim _ {n \to \infty} 0 = 0.
$$

Since $1 \neq 0$ , we have a contradiction. Thus this function does not have a limit at 0. 

— Exercises — 

Exercise 9.3.1. Prove Proposition 9.3.9. 

Exercise 9.3.2. Prove the remaining claims in Proposition 9.3.14. 

Exercise 9.3.3. Prove Lemma 9.3.18. 

Exercise 9.3.4. Propose a definition for limit superior lim $\scriptstyle \operatorname* { s u p } _ { x \to x _ { 0 } ; x \in E } f ( x )$ and limit inferior lim ${ \mathrm { i n f } } _ { x  x _ { 0 } ; x \in E } f ( x )$ , and then propose an analogue of Proposition 9.3.9 for your definition. (For an additional challenge: prove that analogue.) 

Exercise 9.3.5. (Continuous version of squeeze test) Let X be a subset of R, let E be a subset of X, let $x _ { 0 }$ be an adherent point of $E ,$ , and let $f : X \to \mathbf { R }$ , $g : X \to \mathbf { R } , h : X \to \mathbf { R }$ be functions such that $f ( x ) \leq g ( x ) \leq h ( x )$ for all $x \in E$ . If we have $\begin{array} { r } { \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in E } f ( x ) = \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in E } h ( x ) = L } \end{array}$ for some real number $L ,$ show that $\begin{array} { r } { \operatorname* { l i m } _ { x  x _ { 0 } ; x \in E } g ( x ) = L } \end{array}$ 

## 9.4 Continuous functions

We now introduce one of the most fundamental notions in the theory of functions - that of continuity. 

Definition 9.4.1 (Continuity). Let $X$ be a subset of R, and let $f$ : $X  \mathbf { R }$ be a function. Let $x _ { 0 }$ be an element of $X$ . We say that $f$ is continuous at $x _ { 0 }$ if we have 

$$
\lim _ {x \to x _ {0}; x \in X} f (x) = f (x _ {0});
$$

in other words, the limit of $f ( x )$ as x converges to $x _ { 0 }$ in X exists and is equal to $f ( x _ { 0 } )$ . We say that f is continuous on $X$ (or simply continuous) if $f$ is continuous at $x _ { 0 }$ for every $x _ { 0 } \in X$ . We say that $f$ is discontinuous at $x _ { 0 }$ if it is not continuous at $x _ { 0 }$ 

Example 9.4.2. Let c be a real number, and let $f : \mathbf { R }  \mathbf { R }$ be the constant function $f ( x ) : = c $ . Then for every real number $x _ { 0 } \in \mathbf { R }$ , we have 

$$
\lim _ {x \to x _ {0}; x \in \mathbf {R}} f (x) = \lim _ {x \to x _ {0}; x \in \mathbf {R}} c = c = f (x _ {0}),
$$

thus $f$ is continuous at every point $x _ { 0 } \in \mathbf { R }$ , or in other words $f$ is continuous on $\mathbf { R }$ . 

Example 9.4.3. Let $f : \mathbf { R }  \mathbf { R }$ be the identity function $f ( x ) : = x .$ Then for every real number $x _ { 0 } \in \mathbf { R }$ , we have 

$$
\lim _ {x \to x _ {0}; x \in {\bf R}} f (x) = \lim _ {x _ {0} \in x; x \in {\bf R}} x = x _ {0} = f (x _ {0}),
$$

thus $f$ is continuous at every point $x _ { 0 } \in \mathbf { R } .$ , or in other words $f$ is continuous on R. 

Example 9.4.4. Let sgn : $\mathbf { \partial } \cdot \mathbf { R }  \mathbf { R } \quad$ be the signum function defined in Example 9.3.16. Then sgn(x) is continuous at every non-zero value of $x ;$ for instance, at 1, we have (using Proposition 9.3.18) 

$$
\begin{array}{l} \lim _ {x \to 1; x \in \mathbf {R}} \operatorname{sgn} (x) = \lim _ {x \to 1; x \in (0. 9, 1. 1)} \operatorname{sgn} (x) \\ \qquad = \lim _ {x \to 1; x \in (0. 9, 1. 1)} 1 \\ \qquad = 1 \\ \qquad = \operatorname{sgn} (1). \end{array}
$$

On the other hand, sgn is not continuous at 0, since the limit $\scriptstyle \operatorname* { l i m } _ { x \to 0 ; x \in \mathbf { R } } \operatorname { s g n } ( x )$ does not exist. 

Example 9.4.5. Let $f : \mathbf { R }  \mathbf { R }$ be the function 

$$
f (x) := \left\{ \begin{array}{l l} 1 & \text { if } x \in \mathbf {Q} \\ 0 & \text { if } x \not \in \mathbf {Q}. \end{array} \right.
$$

Then by the discussion in the previous section, f is not continuous at 0. In fact, it turns out that $f$ is not continuous at any real number $x _ { 0 }$ (can you see why?). 

Example 9.4.6. Let $f : \mathbf { R }  \mathbf { R }$ be the function 

$$
f (x) := \left\{ \begin{array}{l l} 1 & \text { if } x \geq 0 \\ 0 & \text { if } x <   0. \end{array} \right.
$$

Then $f$ is continuous at every non-zero real number (why?), but is not continuous at 0. However, if we restrict f to the right-hand line $[ 0 , \infty )$ then the resulting function ${ f | } _ { [ 0 , \infty ) }$ now becomes continuous everywhere in its domain, including 0. Thus restricting the domain of a function can make a discontinuous function continuous again. 

## 9.4. Continuous functions

There are several ways to phrase the statement that $^ { 6 6 } f$ is continuous at $\boldsymbol { x } _ { 0 } \boldsymbol { ^ { \flat } }$ : 

Proposition 9.4.7 (Equivalent formulations of continuity). Let X be a subset of R, let $f : X \to \mathbf { R }$ be a function, and let $x _ { 0 }$ be an element of X. Then the following four statements are logically equivalent: 

(a) f is continuous at $x _ { 0 }$ . 

(b) For every sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ consisting of elements of X with $\scriptstyle \operatorname* { l i m } _ { n \to \infty } a _ { n } = x _ { 0 }$ , we have $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } f ( a _ { n } ) = f ( x _ { 0 } ) } \end{array}$ 

(c) For every $\varepsilon > 0$ , there exists a $\delta > 0$ such that $| f ( x ) - f ( x _ { 0 } ) | < \varepsilon$ for all $x \in X$ with $| x - x _ { 0 } | < \delta$ 

(d) For every $\varepsilon > 0$ , there exists a $\delta > 0$ such that $| f ( x ) - f ( x _ { 0 } ) | \leq \varepsilon$ for all $x \in X$ with $| x - x _ { 0 } | \leq \delta$ 

Proof. See Exercise 9.4.1. 

Remark 9.4.8. A particularly useful consequence of Proposition 9.4.7 is the following: if f is continuous at $x _ { 0 }$ , and $a _ { n } \to x _ { 0 }$ as $n \to \infty$ , then $f ( a _ { n } ) \to f ( x _ { 0 } )$ as $n \to \infty$ (provided that all the elements of the sequence $( a _ { n } ) _ { n = 0 } ^ { \infty }$ lie in the domain of $f ,$ of course). Thus continuous functions are very useful in computing limits. 

The limit laws in Proposition 9.3.14, combined with the definition of continuity in Definition 9.4.1, immediately imply 

Proposition 9.4.9 (Arithmetic preserves continuity). Let X be a subset of R, and let $f : X \to \mathbf { R }$ and $g : X  \mathbf { R }$ be functions. Let $x _ { 0 } \in X$ Then if f and g are both continuous at $x _ { 0 }$ , then the functions $f + g _ { i }$ $f - g , \operatorname* { m a x } ( f , g )$ , $\operatorname* { m i n } ( f , g )$ and fg are also continuous at $x _ { 0 }$ . If g is non-zero on X, then $f / g$ is also continuous at $x _ { 0 }$ 

In particular, the sum, diference, maximum, minimum, and product of continuous functions are continuous; and the quotient of two continuous functions is continuous as long as the denominator does not become zero. 

One can use Proposition 9.4.9 to show that a lot of functions are continuous. For instance, just by starting from the fact that constant functions are continuous, and the identity function $f ( x ) = x$ is continuous (Exercise 9.4.2), one can show that the function $g ( x ) : =$ max $( x ^ { 3 } + 4 x ^ { 2 } + x + 5 , x ^ { 4 } - x ^ { 3 } ) / ( x ^ { 2 } - 4 )$ , for instance, is continuous at every point of R except the two points $x = + 2 , x = - 2$ where the denominator vanishes. 

Some other examples of continuous functions are given below. 

Proposition 9.4.10 (Exponentiation is continuous, I). Let $a > 0$ be a positive real number. Then the function $f : \mathbf { R }  \mathbf { R }$ defined by $f ( x ) : = a ^ { x }$ is continuous. 

Proof. See Exercise 9.4.3. 

Proposition 9.4.11 (Exponentiation is continuous, II). Let p be a real number. Then the function $f : ( 0 , \infty ) \to \mathbf { R }$ defined by $f ( x ) : = x ^ { p }$ is continuous. 

Proof. See Exercise 9.4.4. 

There is a stronger statement than Propositions 9.4.10, 9.4.11, namely that exponentiation is jointly continuous in both the exponent and the base, but this is harder to show; see Exercise 11.25.10. 

Proposition 9.4.12 (Absolute value is continuous). The function f : $\mathbf R \to \mathbf R$ defined by $f ( x ) : = | x |$ is continuous. 

Proof. This follows since $| x | = \operatorname* { m a x } ( x , - x )$ and the functions $x , - x$ are already continuous. □ 

The class of continuous functions is not only closed under addition, subtraction, multiplication, and division, but is also closed under composition: 

Proposition 9.4.13 (Composition preserves continuity). Let X and Y be subsets of R, and let $f : X \to Y$ and $g : Y  \mathbf { R }$ be functions. Let x be a point in X. If f is continuous at $x _ { 0 }$ , and g is continuous at $f ( x _ { 0 } )$ then the composition $g \circ f : X  \mathbf { R }$ is continuous at $x _ { 0 }$ 

Proof. See Exercise 9.4.5. 

Example 9.4.14. Since the function $f ( x ) : = 3 x + 1$ is continuous on al of R, and the function $g ( x ) : = 5 ^ { x }$ is continuous on all of R, the function $g \circ f ( x ) = 5 ^ { 3 x + 1 }$ is continuous on all of R. By several applications of the above propositions, one can show that far more complicated functions, e.g., $h ( x ) : = | x ^ { 2 } - 8 x + 7 | ^ { \sqrt { 2 } } / ( x ^ { 2 } + 1 )$ , are also continuous. (Why is this function continuous?) There are still a few functions though that are not yet easy to test for continuity, such as $k ( x ) : = x ^ { x }$ ; this function can be dealt with more easily once we have the machinery of logarithms, which we will see in Section 11.25. 

— Exercises — 

Exercise 9.4.1. Prove Proposition 9.4.7. (Hint: this can largely be done by applying the previous propositions and lemmas. Note that to prove ${ ( \mathrm { a ) , ( b ) } }$ and (c) are equivalent, you do not have to prove all six equivalences, but you do have to prove at least three; for instance, showing that (a) implies (b), (b) implies (c), and (c) implies (a) will sufice, although this is not necessarily the shortest or simplest way to do this question.) 

Exercise 9.4.2. Let X be a subset of R, and let $c \in \mathbf { R }$ . Show that the constant function $f : X \to \mathbf { R }$ defined by $f ( x ) : = c$ is continuous, and show that the identity function $g : X  \mathbf { R }$ defined by $g ( x ) : = x$ is also continuous. 

Exercise 9.4.3. Prove Proposition 9.4.10. (Hint: you can use Lemma 6.5.3, combined with the squeeze test (Corollary 6.4.14) and Proposition 6.7.3.) 

Exercise 9.4.4. Prove Proposition 9.4.11. (Hint: from limit laws (Proposition 9.3.14) one can show that lim $\operatorname* { l } _ { x \to 1 } x ^ { n } = 1$ for all integers n. From this and the squeeze test (Corollary 6.4.14) deduce that $\scriptstyle \operatorname* { l i m } _ { x \to 1 } x ^ { p } = 1$ for all real numbers p. Finally, apply Proposition 6.7.3.) 

Exercise 9.4.5. Prove Proposition 9.4.13. 

Exercise 9.4.6. Let X be a subset of R, and let $f : X \to \mathbf { R }$ be a continuous function. If Y is a subset of X, show that the restriction $f | _ { Y } : Y  \mathbf { R }$ of $f$ to Y is also a continuous function. (Hint: this is a simple result, but it requires you to follow the definitions carefully.) 

Exercise 9.4.7. Let $n \geq 0$ be an integer, and for each $0 \leq i \leq n$ let $c _ { i }$ be a real number. Let $P : \mathbf { R }  \mathbf { R }$ be the function 

$$
P (x) := \sum_ {i = 0} ^ {n} c _ {i} x ^ {i};
$$

such a function is known as a polynomial of one variable; a typical example is $P ( x ) = 6 x ^ { 4 } - 3 x ^ { 2 } + 4$ . Show that $P$ is continuous. 

## 9.5 Left and right limits

We now introduce the notion of left and right limits, which can be thought of as two seperate “halves” of the complete limit $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in X } f ( x )$ 

Definition 9.5.1 (Left and right limits). Let X be a subset of R, $f$ : $X  \mathbf { R }$ be a function, and let $x _ { 0 }$ be a real number. If $x _ { 0 }$ is an adherent point of $X \cap ( x _ { 0 } , \infty )$ , then we define the right limit $f ( x _ { 0 } + )$ of $f$ at $x _ { 0 }$ by the formula 

$$
f (x _ {0} +) := \lim _ {x \to x _ {0}; x \in X \cap (x _ {0}, \infty)} f (x),
$$

provided of course that this limit exists. Similarly, if $x _ { 0 }$ is an adherent point of $X \cap ( - \infty , x _ { 0 } )$ , then we define the left limit $f ( x _ { 0 } - )$ of $f$ at $x _ { 0 }$ by the formula 

$$
f (x _ {0} -) := \lim _ {x \to x _ {0}; x \in X \cap (- \infty , x _ {0})} f (x),
$$

again provided that the limit exists. (Thus in many cases $f ( x _ { 0 } + )$ and $f ( x _ { 0 } - )$ will not be defined.) 

Sometimes we use the shorthand notations 

$$
\begin{array}{l} \lim _ {x \to x _ {0} +} f (x) := \lim _ {x \to x _ {0}; x \in X \cap (x _ {0}, \infty)} f (x); \\ \lim _ {x \to x _ {0} -} f (x) := \lim _ {x \to x _ {0}; x \in X \cap (- \infty , x _ {0})} f (x) \end{array}
$$

when the domain X of f is clear from context. 

Example 9.5.2. Consider the signum function sgn : $\mathbf R  \mathbf R$ defined in Example 9.3.16. We have 

$$
\operatorname{sgn} (0 +) = \lim _ {x \to x _ {0}; x \in \mathbf {R} \cap (0, \infty)} \operatorname{sgn} (x) = \lim _ {x \to x _ {0}; x \in \mathbf {R} \cap (0, \infty)} 1 = 1
$$

and 

$$
\operatorname{sgn} (0 -) = \lim _ {x \to x _ {0}; x \in \mathbf {R} \cap (- \infty , 0)} \operatorname{sgn} (x) = \lim _ {x \to x _ {0}; x \in \mathbf {R} \cap (- \infty , 0)} - 1 = - 1,
$$

while $\mathrm { s g n } ( 0 ) = 0$ by definition. 

Note that f does not necessarily have to be defined at $x _ { 0 }$ in order for $f ( x _ { 0 } + )$ or $f ( x _ { 0 } - )$ to be defined. For instance, if $f : \mathbf { R } - \{ 0 \}  \mathbf { R }$ is the function $f ( x ) : = x / | x |$ , then $f ( 0 + ) = 1$ and $f ( 0 - ) = - 1 ~ \mathrm { ( w h y ? ) }$ even though $f ( 0 )$ is undefined. 

From Proposition 9.4.7 we see that if the right limit $f ( x _ { 0 } + )$ exists, and $( a _ { n } ) _ { n = 0 } ^ { \infty }$ is a sequence in X converging to $x _ { 0 }$ from the right (i.e., $a _ { n } \ > \ x _ { 0 }$ for all $n \in \mathbf { N } )$ , then $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } f ( a _ { n } ) \ = \ f ( x _ { 0 } + ) } \end{array}$ . Similarly, if $( b _ { n } ) _ { n = 0 } ^ { \infty }$ is a sequence converging to x from the left $( \mathrm { i . e . , } a _ { n } < x _ { 0 }$ for all $n \in \mathbf { N } )$ then $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } f ( a _ { n } ) = f ( x _ { 0 } - ) } \end{array}$ 

Let $x _ { 0 }$ be an adherent point of both $X \cap ( x _ { 0 } , \infty )$ and $X \cap ( - \infty , x _ { 0 } )$ If f is continuous at $x _ { 0 }$ , it is clear from Proposition 9.4.7 that $f ( x _ { 0 } + )$ 

and $f ( x _ { 0 } - )$ both exist and are equal to $f ( x _ { 0 } )$ . (Can you see why?) A converse is also true (compare this with Proposition 6.4.12(f)): 

Proposition 9.5.3. Let X be a subset of R containing a real number x , and suppose that $x _ { 0 }$ is an adherent point of both $X \cap ( x _ { 0 } , \infty )$ and $X \cap ( - \infty , x _ { 0 } )$ . Let $f : X \to \mathbf { R }$ be a function. If $f ( x _ { 0 } + )$ and $f ( x _ { 0 } - )$ both exist and are both equal to $f ( x _ { 0 } )$ , then f is continuous at $x _ { 0 }$ 

Proof. Let us write $L : = f ( x _ { 0 } )$ . Then by hypothesis we have 

$$
\lim _ {x \to x _ {0}; x \in X \cap (x _ {0}, \infty)} f (x) = L\tag{9.1}
$$

and 

$$
\lim _ {x \to x _ {0}; x \in X \cap (- \infty , x _ {0})} f (x) = L.\tag{9.2}
$$

Let $\varepsilon > 0$ be given. From (9.1) and Proposition 9.4.7 (applied to the restriction of f to $X \cap ( x _ { 0 } , + \infty ) )$ , we know that there exists a $\delta _ { + } > 0$ such that $| f ( x ) - L | < \varepsilon$ for all $x \in X \cap ( x _ { 0 } , \infty )$ for which $| x - x _ { 0 } | < \delta _ { + }$ From (9.2) we similarly know that there exists a $\delta _ { - } ~ > ~ 0$ such that $| f ( x ) - L | < \varepsilon$ for all $x \in X \cap ( - \infty , x _ { 0 } )$ for which $| x - x _ { 0 } | < \delta _ { - }$ . Now let $\delta : = \operatorname* { m i n } ( \delta _ { - } , \delta _ { + } )$ ; then $\delta > 0 \mathrm { \ : \ : ( w h y ? ) }$ , and suppose that $x \in X$ is such that $| x - x _ { 0 } | < \delta$ . Then there are three cases: $x > x _ { 0 } , x = x _ { 0 }$ , and $x < x _ { 0 }$ , but in all three cases we know that $| f ( x ) - L | < \varepsilon .$ . (Why? the reason is diferent in each of the three cases.) By Proposition 9.4.7 we thus have that f is continuous at $x _ { 0 }$ , as desired. □ 

As we saw with the signum function in Example 9.3.16, it is possible for the left and right limits $f ( x _ { 0 } - ) , f ( x _ { 0 } + )$ of a function $f$ at a point $x _ { 0 }$ to both exist, but not be equal to each other; when this happens, we say that f has a jump discontinuity at $x _ { 0 }$ . Thus, for instance, the signum function has a jump discontinuity at zero. Also, it is possible for the left and right limits $f ( x _ { 0 } - ) , f ( x _ { 0 } + )$ to exist and be equal each other, but not be equal to $f ( x _ { 0 } )$ ; when this happens we say that f has a removable discontinuity (or removable singularity) at $x _ { 0 }$ . For instance, if we take $f : \mathbf { R }  \mathbf { R }$ to be the function 

$$
f (x) := \left\{ \begin{array}{l l} 1 & \text { if } x = 0 \\ 0 & \text { if } x \neq 0, \end{array} \right.
$$

then $f ( 0 + )$ and $f ( 0 - )$ both exist and equal $0 \ \mathrm { ( w h y ? ) }$ , but $f ( 0 )$ equals 1; thus f has a removable discontinuity at 0. 

Remark 9.5.4. Jump discontinuities and removable discontinuities are not the only way a function can be discontinuous. Another way is for a function to go to infinity at the discontinuity: for instance, the function $f : \mathbf { R } - \{ 0 \}  \mathbf { R }$ defined by $f ( x ) : = 1 / x$ has a discontinuity at 0 which is neither a jump discontinuity or a removable singularity; informally, $f ( x )$ converges to $+ \infty$ when x approaches 0 from the right, and converges to $- \infty$ when x approaches 0 from the left. These types of singularities are sometimes known as asymptotic discontinuities. There are also oscillatory discontinuities, where the function remains bounded but still does not have a limit near $x _ { 0 }$ . For instance, the function $f : \mathbf { R }  \mathbf { R }$ defined by 

$$
f (x) := \left\{ \begin{array}{l l} 1 & \text {if} x \in \mathbf {Q} \\ 0 & \text {if} x \not \in \mathbf {Q} \end{array} \right.
$$

has an oscillatory discontinuity at 0 (and in fact at any other real number also). This is because the function does not have left or right limits at 0, despite the fact that the function is bounded. 

The study of discontinuities (also called singularities) continues further, but is beyond the scope of this text. For instance, singularities play a key rˆole in complex analysis. 

## — Exercises —

Exercise 9.5.1. Let E be a subset of R, let $f : E  \mathbf { R }$ be a function, and let $x _ { 0 }$ be an adherent point of E. Write down a definition of what it would mean for the limit $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in E } f ( x )$ to exist and equal + or . If $f : { \bf R } \backslash \{ 0 \}  { \bf R }$ is the function $f ( x ) : = 1 / x$ , use your definition to conclude $f ( 0 + ) = + \infty$ and $f ( 0 - ) = - \infty$ . Also, state and prove some analogue of Proposition 9.3.9 when $L = + \infty$ or $L = - \infty$ 

## 9.6 The maximum principle

In the previous two sections we saw that a large number of functions were continuous, though certainly not all functions were continuous. We now show that continuous functions enjoy a number of other usefu properties, especially if their domain is a closed interval. It is here that we shall begin exploiting the full power of the Heine-Borel theorem (Theorem 9.1.24). 

Definition 9.6.1. Let X be a subset of R, and let $f : X  \mathbf { R }$ be a function. We say that f is bounded from above if there exists a real number M such that $f ( x ) \leq M$ for all $x \in X$ . We say that f is bounded from below if there exists a real number M such that $f ( x ) \geq - M$ for all $x \in X$ . We say that f is bounded if there exists a real number M such that $| f ( x ) | \leq M$ for all $x \in X$ 

Remark 9.6.2. A function is bounded if and only if it is bounded both from above and below. (Why? Note that one part of the “if and only $\mathrm { i f } ^ { \dag }$ is slightly trickier than the other.) Also, a function $f : X \to \mathbf { R }$ is bounded if and only if its image $f ( X )$ is a bounded set in the sense of Definition 9.1.22 (why?). 

Not all continuous functions are bounded. For instance, the function $f ( x ) : = x$ on the domain R is continuous but unbounded $\mathrm { \left( w h y ? \right) }$ , although it is bounded on some smaller domains, such as [1, 2]. The function $f ( x ) : = 1 / x$ is continuous but unbounded on $( 0 , 1 )  { \mathrm { \Omega } } \left( \mathrm { w h y ? } \right)$ • though it is continuous and bounded on [1, 2] (why?). However, if the domain of the continuous function is a closed and bounded interval, then we do have boundedness: 

Lemma 9.6.3. Let $a < b$ be real numbers, and let $f : [ a , b ]  \mathbf { R }$ be a function continuous on $[ a , b ]$ . Then f is a bounded function. 

Proof. Suppose for sake of contradiction that f is not bounded. Thus for every real number M there exists an element $x \in [ a , b ]$ such that $| f ( x ) | \geq M$ 

In particular, for every natural number $n ,$ the set $\{ x \ \in \ [ a , b ] \ :$ $| f ( x ) | \geq n \}$ is non-empty. We can thus choose<sup>2</sup> a sequence $( x _ { n } ) _ { n = 0 } ^ { \infty }$ in $[ a , b ]$ such that $| f ( x _ { n } ) | \geq n$ for all $n .$ . This sequence lies in $[ a , b ]$ and so by Theorem 9.1.24 there exists a subsequence $( x _ { n _ { j } } ) _ { j = 0 } ^ { \infty }$ which converges to some limit $L \in [ a , b ]$ , where $n _ { 0 } < n _ { 1 } < n _ { 2 } < . . .$ . is an increasing sequence of natural numbers. In particular, we see that $n _ { j } \geq j$ for all $j \in \mathbf { N }$ (why? use induction). 

Since f is continuous on $[ a , b ]$ , it is continuous at L, and in particular we see that 

$$
\lim _ {j \to \infty} f (x _ {n _ {j}}) = f (L).
$$

Thus the sequence $( f ( x _ { n _ { j } } ) ) _ { j = 0 } ^ { \infty }$ is convergent, and hence it is bounded. $\mathrm { O n }$ the other hand, we know from the construction that $| f ( x _ { n _ { j } } ) | \geq$ $n _ { j } \geq j$ for all $j$ , and hence the sequence $( f ( x _ { n _ { j } } ) ) _ { j = 0 } ^ { \infty }$ is not bounded, a contradiction. □ 

Remark 9.6.4. There are two things about this proof that are worth noting. Firstly, it shows how useful the Heine-Borel theorem (Theorem 9.1.24) is. Secondly, it is an indirect proof; it doesn’t say how to find the bound for $f _ { i }$ , but it shows that having $f$ unbounded leads to a contradiction. 

We now improve Lemma 9.6.3 to say something more. 

Definition 9.6.5 (Maxima and minima). Let $f : X \to \mathbf { R }$ be a function, and let $x _ { 0 } \in X$ . We say that f attains its maximum at $x _ { 0 }$ if we have $f ( x _ { 0 } ) \geq f ( x )$ for all $x \in X \ { \mathrm { ( i . e . } }$ , the value of f at the point $x _ { 0 }$ is larger than or equal to the value of $f$ at any other point in X). We say that $f$ attains its minimum at $x _ { 0 }$ if we have $f ( x _ { 0 } ) \leq f ( x )$ 

Remark 9.6.6. If a function attains its maximum somewhere, then it must be bounded from above $\mathrm { \left( w h y ? \right) }$ . Similarly if it attains its minimum somewhere, then it must be bounded from below. These notions of maxima and minima are global; local versions will be defined in Definition 10.2.1. 

Proposition 9.6.7 (Maximum principle). Let $a < b$ be real numbers, and let $f : [ a , b ]  \mathbf { R }$ be a function continuous on $[ a , b ]$ . Then f attains its maximum at some point $x _ { m a x } \in [ a , b ]$ , and also attains its minimum at some point $x _ { m i n } \in [ a , b ]$ 

Remark 9.6.8. Strictly speaking, “maximum principle” is a misnomer, since the principle also concerns the minimum. Perhaps a more precise name would have been “extremum principle”; the word “extremum” is used to denote either a maximum or a minimum. 

Proof. We shall just show that f attains its maximum somewhere; the proof that it attains its minimum also is similar but is left to the reader. 

From Lemma 9.6.3 we know that f is bounded, thus there exists an M such that $- M \leq f ( x ) \leq M$ for each $x \in [ a , b ]$ . Now let E denote the set 

$$
E := \{f (x): x \in [ a, b ] \}.
$$

(In other words, $E : = f ( [ a , b ] ) . )$ By what we just said, this set is a subset of $[ - M , M ]$ . It is also non-empty, since it contains for instance the point $f ( a )$ . Hence by the least upper bound principle, it has a supremum sup(E) which is a real number. 

Write $m : = \operatorname* { s u p } ( E )$ . By definition of supremum, we know that $y \le m$ for all $y \in E ;$ by definition of $E .$ , this means that $f ( x ) \ \leq \ m$ for all $x \in [ a , b ]$ . Thus to show that f attains its maximum somewhere, it will sufice to find an $x _ { m a x } \in [ a , b ]$ such that $f ( x _ { m a x } ) = m$ . (Why will this sufice?) 

Let $n \geq 1$ be any integer. Then $m - { \frac { 1 } { n } } < m = \operatorname* { s u p } ( E )$ . As $\operatorname { s u p } ( E )$ is the least upper bound for E, $\textstyle m - { \frac { 1 } { n } }$ cannot be an upper bound for $E ,$ thus there exists a $y \in E$ such that $\begin{array} { r } { m - \frac { 1 } { n } < y } \end{array}$ . By definition of $E$ , this implies that there exists an $x \in [ a , b ]$ such that $\textstyle m - { \frac { 1 } { n } } < f ( x )$ 

We now choose a sequence $( x _ { n } ) _ { n = 1 } ^ { \infty }$ by choosing, for each $n , x _ { n }$ to be an element of $[ a , b ]$ such that $\begin{array} { r } { m - \frac { 1 } { n } < f ( x _ { n } ) } \end{array}$ . (Again, this requires the axiom of choice; however it is possible to prove this principle without the axiom of choice. For instance, you will see a better proof of this proposition using the notion of compactness in Proposition 11.10.2.) This is a sequence in $[ a , b ]$ ; by the Heine-Borel theorem (Theorem 9.1.24), we can thus find a subsequence $( x _ { n _ { j } } ) _ { j = 1 } ^ { \infty }$ , where $n _ { 1 } < n _ { 2 } < . . . ,$ which converges to some limit $x _ { m a x } \in [ a , b ]$ . Since $( x _ { n _ { j } } ) _ { j = 1 } ^ { \infty }$ converges to $x _ { m a x } .$ and $f$ is continuous at $x _ { m a x }$ , we have as before that 

$$
\lim _ {j \to \infty} f (x _ {n _ {j}}) = f (x _ {m a x}).
$$

$\mathrm { O n }$ the other hand, by construction we know that 

$$
f (x _ {n _ {j}}) > m - \frac {1}{n _ {j}} \geq m - \frac {1}{j},
$$

and so by taking limits of both sides we see that 

$$
f (x _ {m a x}) = \lim _ {j \to \infty} f (x _ {n _ {j}}) \geq \lim _ {j \to \infty} m - \frac {1}{j} = m.
$$

On the other hand, we know that $f ( x ) \leq m$ for all $x \in [ a , b ]$ , so in particular $f ( x _ { m a x } ) \leq m$ . Combining these two inequalities we see that $f ( x _ { m a x } ) = m$ as desired. □ 

Note that the maximum principle does not prevent a function from attaining its maximum or minimum at more than one point. For instance, the function $f ( x ) : = x ^ { 2 }$ on the interval [ 2, 2] attains its maximum at two diferent points, at 2 and at 2. 

Let us write $\operatorname* { s u p } _ { x \in [ a , b ] } f ( x )$ as short-hand for sup $\{ f ( x ) : x \in [ a , b ] \}$ and similarly define inf $\dot { x } \in [ a , b ] ~ f ( x )$ . The maximum principle thus asserts that $m : = \operatorname* { s u p } _ { x \in [ a , b ] } f ( x )$ is a real number and is the maximum value of f on $[ a , b ]$ , i.e., there is at least one point $x _ { m a x }$ in $[ a , b ]$ for which $f ( x _ { m a x } ) = m$ , and for every other $x \in [ a , b ] , f ( x )$ is less than or equal to m. Similarly $\operatorname* { i n f } _ { x \in [ a , b ] } f ( x )$ is the minimum value of $f$ on $[ a , b ]$ 

We now know that on a closed interval, every continuous function is bounded and attains its maximum at least once and minimum at least once. The same is not true for open or infinite intervals; see Exercise 9.6.1. 

Remark 9.6.9. You may encounter a rather diferent “maximum principle” in complex analysis or partial diferential equations, involving analytic functions and harmonic functions respectively, instead of continuous functions. Those maximum principles are not directly related to this one (though they are also concerned with whether maxima exist, and where the maxima are located). 

## — Exercises —

Exercise 9.6.1. Give examples of 

(a) a function $f : ( 1 , 2 ) $ R which is continuous and bounded, attains its minimum somewhere, but does not attain its maximum anywhere; 

(b) a function $f : [ 0 , \infty ) \to \mathbf { R }$ which is continuous, bounded, attains its maximum somewhere, but does not attain its minimum anywhere; 

(c) a function $f : [ - 1 , 1 ] \to \mathbf { R }$ which is bounded but does not attain its minimum anywhere or its maximum anywhere. 

(d) a function $f : [ - 1 , 1 ] \to \mathbf { R }$ which has no upper bound and no lower bound. 

Explain why none of the examples you construct violate the maximum principle. (Note: read the assumptions carefully!) 

## 9.7 The intermediate value theorem

We have just shown that a continuous function attains both its maximum value and its minimum value. We now show that f also attains every value in between. To do this, we first prove a very intuitive theorem: 

Theorem 9.7.1 (Intermediate value theorem). Let $a < b$ , and let $f$ : $[ a , b ]  \mathbf { R }$ be a continuous function on $[ a , b ]$ . Let y be a real number between $f ( a )$ and $f ( b ) , i . e .$ , either $f ( a ) \leq y \leq f ( b ) o r f ( a ) \geq y \geq f ( b )$ Then there exists $c \in [ a , b ]$ such that $f ( c ) = y$ 

Proof. We have two cases: $f ( a ) \leq y \leq f ( b ) { \mathrm { ~ o r ~ } } f ( a ) \geq y \geq f ( b )$ . We will assume the former, that $f ( a ) \leq y \leq f ( b )$ ; the latter is proven similarly and is left to the reader. 

If $y = f ( a )$ or $y = f ( b )$ then the claim is easy, as one can simply set $c = a { \mathrm { ~ o r ~ } } c = b .$ , so we will assume that $f ( a ) < y < f ( b )$ . Let $E$ denote the set 

$$
E := \{x \in [ a, b ]: f (x) <   y \}.
$$

Clearly E is a subset of $[ a , b ]$ , and is hence bounded. Also, since $f ( a ) < y$ we see that a is an element of $E _ { \mathrm { { i } } }$ so $E$ is non-empty. By the least upper bound principle, the supremum 

$$
c := \sup (E)
$$

is thus finite. Since E is bounded by b, we know that $c \leq b ;$ since E contains $^ { a , }$ we know that $c \geq a$ . Thus we have $c \in [ a , b ]$ ]. To complete the proof we now show that $f ( c ) = y$ . The idea is to work from the left of c to show that $f ( c ) \leq y$ , and to work from the right of c to show that $f ( c ) \geq y$ 

Let $n \geq 1$ be an integer. The number $\textstyle c - { \frac { 1 } { n } }$ is less than $c = \operatorname* { s u p } ( E )$ and hence cannot be an upper bound for E. Thus there exists a point, call it $x _ { n }$ , which lies in E and which is greater than $\textstyle c - { \frac { 1 } { n } }$ . Also $x _ { n } \leq c$ since c is an upper bound for E. Thus 

$$
c - \frac {1}{n} \leq x _ {n} \leq c.
$$

By the squeeze test (Corollary 6.4.14) we thus have li $\quad \ m _ { n \to \infty } x _ { n } \ = \ c $ Since $f$ is continuous at $c ,$ this implies that l $\begin{array} { r } { \operatorname* { i m } _ { n \to \infty } f ( x _ { n } ) = f ( c ) } \end{array}$ . But since $x _ { n }$ lies in $E$ for every n, we have $f ( x _ { n } ) \ < \ y$ for every n. By the comparison principle (Lemma 6.4.13) we thus have $f ( c ) \leq y$ . Since $f ( b ) > f ( c )$ , we conclude $c \neq b$ 

Since $c \neq$ b and $c \in [ a , b ]$ , we must have $c < b$ . In particular there is an $N > 0$ such that $\begin{array} { r } { c + \frac { 1 } { n } < b } \end{array}$ for all $n > N$ (since $\textstyle c + { \frac { 1 } { n } }$ converges to c as $n  \infty )$ Since c is the supremum of E and $c + { \frac { 1 } { n } } > c ,$ we thus have $c + { \textstyle { \frac { 1 } { n } } } \not \in E$ for all $n > N$ . Since $c + { \textstyle \frac { 1 } { n } } \in [ a , b ]$ , we thus have $\textstyle f ( c + { \frac { 1 } { n } } ) \geq y$ for all $n \geq N$ . But $c + { \frac { 1 } { n } }$ converges to c, and f is continuous at c, thus $f ( c ) \geq y$ . But we already knew that $f ( c ) \leq y _ { : }$ , thus $f ( c ) = y .$ 7 as desired. □ 

The intermediate value theorem says that if f takes the values $f ( a )$ and $f ( b )$ , then it must also take all the values in between. Note that if f is not assumed to be continuous, then the intermediate value theorem no longer applies. For instance, if $f : [ - 1 , 1 ] \to \mathbf { R }$ is the function 

$$
f (x) := \left\{ \begin{array}{l l} - 1 & \text { if } x \leq 0 \\ 1 & \text { if } x > 0 \end{array} \right.
$$

then $f ( - 1 ) = - 1$ , and $f ( 1 ) = 1$ , but there is no $c \in [ - 1 , 1 ]$ for which $f ( c ) = 0$ . Thus if a function is discontinuous, it can $\mathrm {  { ~ \mathrm { \hat { j } u m p } ^ { \prime } } }$ past intermediate values; however continuous functions cannot do so. 

Remark 9.7.2. A continuous function may take an intermediate value multiple times. For instance, if $f : [ - 2 , 2 ]  \mathbf { R }$ is the function $f ( x ) : =$ $x ^ { 3 } - x$ , then $f ( - 2 ) = - 6$ and $f ( 2 ) = 6 { \mathrm { : } }$ , so we know that there exists a $c \in [ - 2 , 2 ]$ for which $f ( c ) = 0$ . In fact, in this case there exists three such values of c: we have $f ( - 1 ) = f ( 0 ) = f ( 1 ) = 0$ 

Remark 9.7.3. The intermediate value theorem gives another way to show that one can take $n ^ { t h }$ roots of a number. For instance, to construct the square root of 2, consider the function $f : [ 0 , 2 ] \to \mathbf { R }$ defined by $f ( x ) = x ^ { 2 }$ . This function is continuous, with $f ( 0 ) = 0$ and $f ( 2 ) = 4$ Thus there exists a $c \in [ 0 , 2 ]$ such that $f ( c ) = 2 , \mathrm { i . e . , } c ^ { 2 } = 2 .$ . (This argument does not show that there is just one square root of 2, but it does prove that there is at least one square root of 2.) 

Corollary 9.7.4 (Images of continuous functions). Let $a < b$ , and let $f : [ a , b ]  \mathbf { R }$ be a continuous function on $[ a , b ]$ . Let M $\scriptstyle : = \operatorname* { s u p } _ { x \in [ a , b ] } f ( x )$ be the maximum value of f, and let $m : = \operatorname* { i n f } _ { x \in [ a , b ] } f ( x )$ be the minimum value. Let y be a real number between m and M $( i . e . , \ m \leq y \leq M )$ Then there exists a $c \in [ a , b ]$ such that $f ( c ) = y$ . Furthermore, we have $f ( [ a , b ] ) = [ m , M ]$ 

Proof. See Exercise 9.7.1. 

$$
- \text { Exercises } -
$$

Exercise 9.7.1. Prove Corollary 9.7.4. (Hint: you may need Exercise 9.4.6 in addition to the intermediate value theorem.) 

Exercise 9.7.2. Let $f : [ 0 , 1 ] \to [ 0 , 1 ]$ be a continuous function. Show that there exists a real number x in [0, 1] such that $f ( x ) = x$ . (Hint: apply the intermediate value theorem to the function $f ( x ) - x . )$ This point x is known as a fixed point of f, and this result is a basic example of a fixed point theorem, which play an important rˆole in certain types of analysis. 

## 9.8 Monotonic functions

We now discuss a class of functions which is distinct from the class of continuous functions, but has somewhat similar properties: the class of monotone (or monotonic) functions. 

Definition 9.8.1 (Monotonic functions). Let X be a subset of R, and let $f : X \to \mathbf { R }$ be a function. We say that f is monotone increasing if $f ( y ) \geq f ( x )$ whenever $x , y \in X$ and $y > x$ . We say that f is strictly monotone increasing if $f ( y ) > f ( x )$ whenever $x , y \in X$ and $y \ > \ x$ Similarly, we say f is monotone decreasing if $f ( y ) \leq f ( x )$ whenever $x , y \in X$ and $y > x ,$ , and strictly monotone decreasing if $f ( y ) < f ( x )$ whenever $x , y \in X$ and $y \ > \ x$ . We say that f is monotone if it is monotone increasing or monotone decreasing, and strictly monotone if it is strictly monotone increasing or strictly monotone decreasing. 

Examples 9.8.2. The function $f ( x ) : = x ^ { 2 }$ , when restricted to the domain $[ 0 , \infty )$ , is strictly monotone increasing (why?), but when restricted instead to the domain $( - \infty , 0 ]$ , is strictly monotone decreasing (why?). Thus the function is strictly monotone on both $( - \infty , 0 ]$ and $[ 0 , \infty )$ , but is not strictly monotone (or monotone) on the full real line $( - \infty , \infty )$ Note that if a function is strictly monotone on a domain X, it is automatically monotone as well on the same domain X. The constant function $f ( x ) : = 6$ , when restricted to an arbitrary domain $X \subseteq \mathbf { R } ,$ is both monotone increasing and monotone decreasing, but is not strictly monotone (unless X consists of at most one point - why?). 

Continuous functions are not necessarily monotone (consider for instance the function $f ( x ) = x ^ { 2 }$ on R), and monotone functions are not necessarily continuous; for instance, consider the function $f : [ - 1 , 1 ] \to$ R defined earlier by 

$$
f (x) := \left\{ \begin{array}{l l} - 1 & \text { if } x \leq 0 \\ 1 & \text { if } x > 0. \end{array} \right.
$$

Monotone functions obey the maximum principle (Exercise 9.8.1), but not the intermediate value principle (Exercise 9.8.2). On the other hand, it is possible for a monotone function to have many, many discontinuities (Exercise 9.8.5). 

If a function is both strictly monotone and continuous, then it has many nice properties. In particular, it is invertible: 

Proposition 9.8.3. Let $a < b$ be real numbers, and let $f : [ a , b ]  \mathbf { R }$ be a function which is both continuous and strictly monotone increasing. Then f is a bijection from $[ a , b ]$ to $[ f ( a ) , f ( b ) ]$ , and the inverse $f ^ { - 1 }$ $[ f ( a ) , f ( b ) ] \to [ a , b ]$ is also continuous and strictly monotone increasing. 

Proof. See Exercise 9.8.4. 

There is a similar Proposition for functions which are strictly monotone decreasing; see Exercise 9.8.4. 

Example 9.8.4. Let n be a positive integer and $R > 0$ . Since the function $f ( x ) : = x ^ { n }$ is strictly increasing on the interval $[ 0 , R ]$ , we see from Proposition 9.8.3 that this function is a bijection from $[ 0 , R ]$ to $[ 0 , R ^ { n } ]$ , and hence there is an inverse from $[ 0 , R ^ { n } ]$ to [0, R]. This can be used to give an alternate means to construct the $n ^ { t h }$ root $x ^ { 1 / n }$ of a number $x \in [ 0 , R ]$ than what was done in Lemma 5.6.5. 

## — Exercises —

Exercise 9.8.1. Explain why the maximum principle remains true if the hypothesis that f is continuous is replaced with f being monotone, or with f being strictly monotone. (You can use the same explanation for both cases.) 

Exercise 9.8.2. Give an example to show that the intermediate value theorem becomes false if the hypothesis that f is continuous is replaced with f being monotone, or with f being strictly monotone. (You can use the same counterexample for both cases.) 

Exercise 9.8.3. Let $a < b$ be real numbers, and let $f : [ a , b ]  \mathbf { R }$ be a function which is both continuous and one-to-one. Show that f is strictly monotone. (Hint: divide into the three cases $f ( a ) < f ( b ) , f ( a ) = f ( b ) , f ( a ) > f ( b )$ . The second case leads directly to a contradiction. In the first case, use contradiction and the intermediate value theorem to show that f is strictly monotone increasing; in the third case, argue similarly to show f is strictly monotone decreasing.) 

Exercise 9.8.4. Prove Proposition 9.8.3. (Hint: to show that $f ^ { - 1 }$ is continuous, it is easiest to use the “epsilon-delta” definition of continuity, Proposition $9 . 4 . 7 ( \mathrm { c } ) . )$ Is the proposition still true if the continuity assumption is dropped, or if strict monotonicity is replaced just by monotonicity? How should one modify the proposition to deal with strictly monotone decreasing functions instead of strictly monotone increasing functions? 

Exercise 9.8.5. In this exercise we give an example of a function which has a discontinuity at every rational point, but is continuous at every irrational. Since 

## 9.9. Uniform continuity

the rationals are countable, we can write them as $\mathbf { Q } = \{ q ( 0 ) , q ( 1 ) , q ( 2 ) , . . . \} .$ where $q : \mathbf { N }  \mathbf { Q }$ is a bijection from N to $\mathbf { Q }$ . Now define a function $g : { \bf Q }  { \bf R }$ by setting $g ( q ( n ) ) : = 2 ^ { - n }$ for each natural number $n ;$ thus $g$ maps $q ( 0 )$ to 1, q(1) to $2 ^ { - 1 }$ , etc. Since $\textstyle \sum _ { n = 0 } ^ { \infty } 2 ^ { - n }$ is absolutely convergent, we see that $\textstyle \sum _ { r \in \mathbf { Q } } g ( r )$ is also absolutely convergent. Now define the function $f : \mathbf { R }  \mathbf { R }$ by 

$$
f (x) := \sum_ {r \in \mathbf {Q}: r <   x} g (r).
$$

Since $\textstyle \sum _ { r \in \mathbf { Q } } g ( r )$ is absolutely convergent, we know that $f ( x )$ is well-defined for every real number x. 

(a) Show that f is strictly monotone increasing. (Hint: you will need Proposition 5.4.14.) 

(b) Show that for every rational number r, f is discontinuous at $r .$ . (Hint: since $r$ is rational, $r \ = \ q ( n )$ for some natural number n. Show that $f ( x ) \geq f ( r ) + 2 ^ { - n }$ for all $x > r . )$ 

(c) Show that for every irrational number $x , f$ is continuous at x. (Hint: first demonstrate that the functions 

$$
f _ {n} (x) := \sum_ {r \in \mathbf {Q}: r <   x, g (r) \geq 2 ^ {- n}} g (r)
$$

are continuous at x, and that $| f ( x ) - f _ { n } ( x ) | \leq 2 ^ { - n } . )$ 

## 9.9 Uniform continuity

We know that a continuous function on a closed interval $[ a , b ]$ remains bounded (and in fact attains its maximum and minimum, by the maximum principle). However, if we replace the closed interval by an open interval, then continuous functions need not be bounded any more. An example is the function $f : ( 0 , 2 ) \to \mathbf { R }$ defined by $f ( x ) : = 1 / x$ . This function is continuous at every point in (0, 2), and is hence continuous at (0, 2), but is not bounded. Informally speaking, the problem here is that while the function is indeed continuous at every point in the open interval (0, 2), it becomes “less and less” continuous as one approaches the endpoint 0. 

Let us analyze this phenomenon further, using the “epsilon-delta” definition of continuity - Proposition $9 . 4 . 7 ( \mathrm { c } )$ . We know that if $f : X \to$ R is continuous at a point $x _ { 0 }$ , then for every $\varepsilon > 0$ there exists a $\delta$ such that $f ( x )$ will be ε-close to $f ( x _ { 0 } )$ whenever $x \in X$ is δ-close to $x _ { 0 }$ . In other words, we can force $f ( x )$ to be ε-close to $f ( x _ { 0 } )$ if we ensure that x is suficiently close to $x _ { 0 }$ . One way of thinking about this is that around every point $x _ { 0 }$ there is an “island of stability” $( x _ { 0 } - \delta , x _ { 0 } + \delta )$ , where the function $f ( x )$ doesn’t stray by more than $\varepsilon$ from $f ( x _ { 0 } )$ 

Example 9.9.1. Take the function $f ( x ) : = 1 / x$ mentioned above at the point $x _ { 0 } = 1$ . In order to ensure that $f ( x )$ is 0.1-close to $f ( x _ { 0 } )$ , it sufices to take $x$ to be 1/11-close to $x _ { 0 }$ , since if $x$ is 1/11-close to $x _ { 0 }$ then $1 0 / 1 1 < x < 1 2 / 1 1$ , and so $1 1 / 1 2 < f ( x ) < 1 1 / 1 0 .$ , and so $f ( x )$ is 0.1-close to $f ( x _ { 0 } )$ . Thus the $^ { 6 6 } \delta ^ { 9 }$ one needs to make f(x) 0.1-close to $f ( x _ { 0 } )$ is about 1/11 or so, at the point $x _ { 0 } = 1$ 

Now let us look instead at the point $x _ { 0 } = 0 . 1$ . The function $f ( x ) =$ $1 / x$ is still continuous here, but we shall see the continuity is much worse. In order to ensure that $f ( x )$ is 0.1-close to $f ( x _ { 0 } )$ , we need $x$ to be 1/1010-close to $x _ { 0 }$ . Indeed, if x is $1 / 1 0 1 0$ close to $x _ { 0 }$ , then $1 0 / 1 0 1 <$ $x < 1 0 2 / 1 0 1 0$ , and so $9 . 9 0 1 < f ( x ) < 1 0 . 1$ , so $f ( x )$ is 0.1-close to $f ( x _ { 0 } )$ Thus one needs a much smaller $^ { 6 6 } \delta ^ { 9 }$ for the same value of $\varepsilon \mathrm { ~ - ~ i . e . , ~ } f ( x )$ is much more “unstable” near 0.1 than it is near 1, in the sense that there is a much smaller “island of stability” around 0.1 as there is around 1 (if one is interested in keeping $f ( x ) \ 0 . 1 – \mathrm { s t a b l e } )$ 

On the other hand, there are other continuous functions which do not exhibit this behavior. Consider the function $g : ( 0 , 2 )  \mathbf { R }$ defined by $g ( x ) : = 2 x$ . Let us fix $\varepsilon = 0 . 1$ as before, and investigate the island of stability around $x _ { 0 } = 1$ . It is clear that if $x$ is 0.05-close to $x _ { 0 } .$ , then $g ( x )$ is 0.1-close to $g ( x _ { 0 } )$ ; in this case we can take $\delta$ to be 0.05 at $x _ { 0 } = 1$ And if we move x around, say if we set $x _ { 0 }$ to 0.1 instead, the $\delta$ does not change - even when $x _ { 0 }$ is set to 0.1 instead of 1, we see that $g ( x )$ will stay 0.1-close to $g ( x _ { 0 } )$ whenever x is 0.05-close to $x _ { 0 }$ . Indeed, the same $\delta$ works for every $x _ { 0 }$ . When this happens, we say that the function $g$ is uniformly continuous. More precisely: 

Definition 9.9.2 (Uniform continuity). Let X be a subset of $\mathbf { R } ,$ , and let $f : X \to \mathbf { R }$ be a function. We say that $f$ is uniformly continuous if, for every $\varepsilon > 0$ , there exists a $\delta > 0$ such that $f ( x )$ and $f ( x _ { 0 } )$ are ε-close whenever $x , x _ { 0 } \in X$ are two points in X which are δ-close. 

Remark 9.9.3. This definition should be compared with the notion of continuity. From Proposition $9 . 4 . 7 ( \mathrm { c } )$ , we know that a function $f$ is continuous if for every $\varepsilon > 0$ , and every $x _ { 0 } \in X$ , there is a $\delta > 0$ such that $f ( x )$ and $f ( x _ { 0 } )$ are ε-close whenever $x \in X$ is δ-close to $x _ { 0 }$ . The diference between uniform continuity and continuity is that in uniform continuity one can take a single $\delta$ which works for all $x _ { 0 } ~ \in ~ X$ ; for ordinary continuity, each $x _ { 0 } \in X$ might use a diferent $\delta .$ . Thus every uniformly continuous function is continuous, but not conversely. 

Example 9.9.4. (Informal) The function $f : ( 0 , 2 ) \to \mathbf { R }$ defined by $f ( x ) : = 1 / x$ is continuous on (0, 2), but not uniformly continuous, because the continuity (or more precisely, the dependence of $\delta \ \mathrm { o n } \ \varepsilon )$ becomes worse and worse as $x \to 0$ . (We will make this more precise in Example 9.9.10.) 

Recall that the notions of adherent point and of continuous function had several equivalent formulations; both had “epsilon-delta” type formulations (involving the notion of ε-closeness), and both had “sequential” formulations (involving the convergence of sequences); see Lemma 9.1.14 and Proposition 9.3.9. The concept of uniform continuity can similarly be phrased in a sequential formulation, this time using the concept of equivalent sequences (cf. Definition 5.2.6, but we now generalize to sequences of real numbers instead of rationals, and no longer require the sequences to be Cauchy): 

Definition 9.9.5 (Equivalent sequences). Let m be an integer, let $( a _ { n } ) _ { n = m } ^ { \infty }$ and $( b _ { n } ) _ { n = m } ^ { \infty }$ be two sequences of real numbers, and let $\varepsilon > 0$ be given. We say that $( a _ { n } ) _ { n = m } ^ { \infty }$ is ε-close to $( b _ { n } ) _ { n = m } ^ { \infty }$ if $a _ { n }$ is ε-close to $b _ { n }$ for each $n \geq m$ . We say that $( a _ { n } ) _ { n = m } ^ { \infty }$ is eventually ε-close to $( b _ { n } ) _ { n = m } ^ { \infty }$ if there exists an $N \geq m$ such that the sequences $( a _ { n } ) _ { n = N } ^ { \infty }$ and $( b _ { n } ) _ { n = N } ^ { \infty }$ are ε-close. Two sequences $( a _ { n } ) _ { n = m } ^ { \infty }$ and $( b _ { n } ) _ { n = m } ^ { \infty }$ are equivalent if for each $\varepsilon > 0$ , the sequences $( a _ { n } ) _ { n = m } ^ { \infty }$ and $( b _ { n } ) _ { n = m } ^ { \infty }$ are eventually ε-close. 

Remark 9.9.6. One could debate whether ε should be assumed to be rational or real, but a minor modification of Proposition 6.1.4 shows that this does not make any diference to the above definitions. 

The notion of equivalence can be phrased more succinctly using our language of limits: 

Lemma 9.9.7. Let $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ be sequences of real numbers (not necessarily bounded or convergent). Then $( a _ { n } ) _ { n = 1 } ^ { \infty }$ and $( b _ { n } ) _ { n = 1 } ^ { \infty }$ are equivalent if and only if $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } ( a _ { n } - b _ { n } ) = 0 } \end{array}$ 

Proof. See Exercise 9.9.1. 

Meanwhile, the notion of uniform continuity can be phrased using equivalent sequences: 

Proposition 9.9.8. Let X be a subset of R, and let $f : X  \mathbf { R }$ be a function. Then the following two statements are logically equivalent: 

(a) f is uniformly continuous on $X$ 

(b) Whenever $( x _ { n } ) _ { n = 0 } ^ { \infty }$ and $( y _ { n } ) _ { n = 0 } ^ { \infty }$ are two equivalent sequences consisting of elements of X, the sequences $( f ( x _ { n } ) ) _ { n = 0 } ^ { \infty }$ and $( f ( y _ { n } ) ) _ { n = 0 } ^ { \infty }$ are also equivalent. 

Proof. See Exercise 9.9.2. 

Remark 9.9.9. The reader should compare this with Proposition 9.3.9. Proposition 9.3.9 asserted that if f was continuous, then f maps convergent sequences to convergent sequences. In contrast, Proposition 9.9.8 asserts that if $f$ is uniformly continuous, then $f$ maps equivalent pairs of sequences to equivalent pairs of sequences. To see how the two Propositions are connected, observe from Lemma 9.9.7 that $( x _ { n } ) _ { n = 0 } ^ { \infty }$ will converge to $x _ { * }$ if and only if the sequences $( x _ { n } ) _ { n = 0 } ^ { \infty }$ and $( x _ { * } ) _ { n = 0 } ^ { \infty }$ are equivalent. 

Example 9.9.10. Consider the function $f : ( 0 , 2 ) \  \ \mathbf { R }$ defined by $f ( x ) : = 1 / x$ considered earlier. From Lemma 9.9.7 we see that the sequence $( 1 / n ) _ { n = 1 } ^ { \infty }$ and $( 1 / 2 n ) _ { n = 1 } ^ { \infty }$ are equivalent sequences in (0, 2). However, the sequences $( f ( 1 / n ) ) _ { n = 1 } ^ { \infty }$ and $( f ( 1 / 2 n ) ) _ { n = 1 } ^ { \infty }$ are not equivalent (why? Use Lemma 9.9.7 again). So by Proposition 9.9.8, f is not uniformly continuous. (These sequences start at 1 instead of 0, but the reader can easily see that this makes no diference to the above discussion.) 

Example 9.9.11. Consider the function $f : \textbf { R } \to \textbf { R }$ defined by $f ( x ) : = x ^ { 2 }$ . This is a continuous function on R, but it turns out not to be uniformly continuous; in some sense the continuity gets “worse and worse” as one approaches infinity. One way to quantify this is via Proposition 9.9.8. Consider the sequences $( n ) _ { n = 1 } ^ { \infty }$ and $\textstyle ( n + { \frac { 1 } { n } } ) _ { n = 1 } ^ { \infty } .$ By Lemma 9.9.7, these sequences are equivalent. But the sequences $( f ( n ) ) _ { n = 1 } ^ { \infty }$ and $( f ( n + \textstyle { \frac { 1 } { n } } ) ) _ { n = 1 } ^ { \infty }$ are not equivalent, since $f ( n + { \frac { 1 } { n } } ) \ =$ $\begin{array} { r } { n ^ { 2 } + 2 + \frac { 1 } { n ^ { 2 } } = f ( n ) + \ddot { 2 } + \frac { 1 } { n ^ { 2 } } } \end{array}$ does not become eventually 2-close to $f ( n )$ . By Proposition 9.9.8 we can thus conclude that f is not uniformly continuous. 

## 9.9. Uniform continuity

Another property of uniformly continuous functions is that they map Cauchy sequences to Cauchy sequences. 

Proposition 9.9.12. Let X be a subset of R, and let $f : X \to \mathbf { R }$ be a uniformly continuous function. Let $( x _ { n } ) _ { n = 0 } ^ { \infty }$ be a Cauchy sequence consisting entirely of elements in X. Then $( f ( x _ { n } ) ) _ { n = 0 } ^ { \infty }$ is also a Cauchy sequence. 

Proof. See Exercise 9.9.3. 

Example 9.9.13. Once again, we demonstrate that the function f : $( 0 , 2 )  \mathbf { R }$ defined by $f ( x ) : = 1 / x$ is not uniformly continuous. The sequence $( 1 / n ) _ { n = 1 } ^ { \infty }$ is a Cauchy sequence in (0, 2), but the sequence $( f ( 1 / n ) ) _ { n = 1 } ^ { \infty }$ is not a Cauchy sequence (why?). Thus by Proposition 9.9.12, f is not uniformly continuous. 

Corollary 9.9.14. Let X be a subset of R, let $f : X  \mathbf { R }$ be a uniformly continuous function, and let x be an adherent point ofX. Then the limit $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in X } f ( x )$ exists (in particular, it is a real number). 

Proof. See Exercise 9.9.4. 

We now show that a uniformly continuous function will map bounded sets to bounded sets. 

Proposition 9.9.15. Let X be a subset of R, and let $f : X  \mathbf { R }$ be a uniformly continuous function. Suppose that E is a bounded subset of X. Then $f ( E )$ is also bounded. 

Proof. See Exercise 9.9.5. 

As we have just seen repeatedly, not all continuous functions are uniformly continuous. However, if the domain of the function is a closed interval, then continuous functions are in fact uniformly continuous: 

Theorem 9.9.16. Let $a \textless b$ be real numbers, and let $f : [ a , b ]  \mathbf { R }$ be a function which is continuous on [a, b]. Then f is also uniformly continuous. 

Proof. Suppose for sake of contradiction that f is not uniformly continuous. By Proposition 9.9.8, there must therefore exist two equivalent sequences $( x _ { n } ) _ { n = 0 } ^ { \infty }$ and $( y _ { n } ) _ { n = 0 } ^ { \infty }$ in $[ a , b ]$ such that the sequences $( f ( x _ { n } ) ) _ { n = 0 } ^ { \infty }$ and $( f ( y _ { n } ) ) _ { n = 0 } ^ { \infty }$ are not equivalent. In particular, we can find an $\varepsilon > 0$ such that $( f ( x _ { n } ) ) _ { n = 0 } ^ { \infty }$ and $( f ( y _ { n } ) ) _ { n = 0 } ^ { \infty }$ are not eventually ε-close. 

Fix this value of ε, and let E be the set 

$$
E := \{n \in N: f (x _ {n}) \text {   and   } f (y _ {n}) \text {   are   not   } \varepsilon \text {-close} \}.
$$

We must have E infinite, since if E were finite then $( f ( x _ { n } ) ) _ { n = 0 } ^ { \infty }$ and $( f ( y _ { n } ) ) _ { n = 0 } ^ { \infty }$ would be eventually ε-close (why?). By Proposition 8.1.5, E is countable; in fact from the proof of that proposition we see that we can find an infinite sequence 

$$
n _ {0} <   n _ {1} <   n _ {2} <   \ldots
$$

consisting entirely of elements in E. In particular, we have 

$$
\left| f \left(x _ {n _ {j}}\right) - f \left(y _ {n _ {j}}\right) \right| > \varepsilon \text { for   all } j \in \mathbf {N}.\tag{9.3}
$$

On the other hand, the sequence $( x _ { n _ { j } } ) _ { j = 0 } ^ { \infty }$ is a sequence in $[ a , b ]$ , and so by the Heine-Borel theorem (Theorem 9.1.24) there must be a subsequence $( x _ { n _ { j _ { k } } } ) _ { k = 0 } ^ { \infty }$ which converges to some limit L in $[ a , b ]$ . In particular, $f$ is continuous at L, and so by Proposition 9.4.7, 

$$
\lim _ {k \to \infty} f (x _ {n _ {j _ {k}}}) = f (L).\tag{9.4}
$$

Note that $( x _ { n _ { j _ { k } } } ) _ { k = 0 } ^ { \infty }$ is a subsequence of $( x _ { n } ) _ { n = 0 } ^ { \infty }$ , and $( y _ { n _ { j _ { k } } } ) _ { k = 0 } ^ { \infty }$ is a subsequence of $( y _ { n } ) _ { n = 0 } ^ { \infty }$ , by Lemma 6.6.4. On the other hand, from Lemma 9.9.7 we have 

$$
\lim _ {n \to \infty} (x _ {n} - y _ {n}) = 0.
$$

By Proposition 6.6.5, we thus have 

$$
\lim _ {k \to \infty} (x _ {n _ {j _ {k}}} - y _ {n _ {j _ {k}}}) = 0.
$$

Since $x _ { n _ { j _ { k } } }$ converges to L as $k \to \infty$ , we thus have by limit laws 

$$
\lim _ {k \to \infty} y _ {n _ {j _ {k}}} = L
$$

and hence by continuity of f at L 

$$
\lim _ {k \to \infty} f (y _ {n _ {j _ {k}}}) = f (L).
$$

Subtracting this from (9.4) using limit laws, we obtain 

$$
\lim _ {k \to \infty} (f (x _ {n _ {j _ {k}}}) - f (y _ {n _ {j _ {k}}})) = 0.
$$

But this contradicts (9.3) (why?). From this contradiction we conclude that f is in fact uniformly continuous. □ 

Remark 9.9.17. One should compare Lemma 9.6.3, Proposition 9.9.15, and Theorem 9.9.16 with each other. No two of these results imply the third, but they are all consistent with each other. 

## — Exercises —

Exercise 9.9.1. Prove Lemma 9.9.7. 

Exercise 9.9.2. Prove Proposition 9.9.8. (Hint: you should avoid Lemma 9.9.7, and instead go back to the definition of equivalent sequences in Definition 9.9.5.) Exercise 9.9.3. Prove Proposition 9.9.12. (Hint: use Definition 9.9.2 directly.) Exercise 9.9.4. Use Proposition 9.9.12 to prove Corollary 9.9.14. Use this corollary to give an alternate demonstration of the results in Example 9.9.10. Exercise 9.9.5. Prove Proposition 9.9.15. (Hint: mimic the proof of Lemma 9.6.3. At some point you will need either Proposition 9.9.12 or Corollary 9.9.14.) 

Exercise 9.9.6. Let X, Y, Z be subsets of R. Let $f : X \to Y$ be a function which is uniformly continuous on X, and let $g : Y  Z$ be a function which is uniformly continuous on Y. Show that the function $g \circ f : X \to Z$ is uniformly continuous on X. 

## 9.10 Limits at infinity

Until now, we have discussed what it means for a function $f : X  \mathbf { R }$ to have a limit as $x  x _ { 0 }$ as long as $x _ { 0 }$ is a real number. We now briefly discuss what it would mean to take limits when $x _ { 0 }$ is equal to + or $- \infty$ . (This is part of a more general theory of continuous functions on a topological space; see Section 11.12.) 

First, we need a notion of what it means for $+ \infty \mathrm { o r } \mathrm { - } \infty$ to be adherent to a set. 

Definition 9.10.1 (Infinite adherent points). Let X be a subset of R. We say that + is adherent to X if for every $M \in \mathbf { R }$ there exists an $x \in X$ such that $x > M ;$ we say that $- \infty$ is adherent to X if for every $M \in \mathbf { R }$ there exists an $x \in X$ such that $x < M$ 

In other words, + is adherent to X if X has no upper bound, or equivalently if $\operatorname* { s u p } ( X ) = + \infty$ . Similarly is adherent to X if X has no lower bound, or if inf $( X ) = - \infty$ . Thus a set is bounded if and only $\mathrm { i f } + \infty \ \mathrm { a n d \ - } \infty$ are not adherent points. 

Remark 9.10.2. This definition may seem rather diferent from Definition 9.1.8, but can be unified using the topological structure of the extended real line $\mathbf { R } ^ { * }$ , which we will not discuss here. 

Definition 9.10.3 (Limits at infinity). Let X be a subset of R with + as an adherent point, and let $f : X \to \mathbf { R }$ be a function. We say that $f ( x )$ converges to L as $x \to + \infty$ in X, and write $\begin{array} { r } { \operatorname* { l i m } _ { x  + \infty ; x \in X } f ( x ) = L . } \end{array}$ if for every $\varepsilon > 0$ there exists an M such that f is ε-close to L on $X \cap ( M , + \infty ) { \mathrm { ~ ( i . e . , ~ } } | f ( x ) - L | \leq \varepsilon$ for all $x \in X$ such that $x > M )$ Similarly we say that $f ( x )$ converges to L as $x \to - \infty$ if for every $\varepsilon > 0$ there exists an M such that f is ε-close to L on $X \cap ( - \infty , M )$ 

Example 9.10.4. Let $f : ( 0 , \infty ) \to \mathbf { R }$ be the function $f ( x ) : = 1 / x .$ Then we have $\mathrm { l i m } _ { x  + \infty ; x \in ( 0 , \infty ) } 1 / x = 0$ . (Can you see why, from the definition?) 

One can do many of the same things with these limits at infinity as we have been doing with limits at other points $x _ { 0 } ;$ for instance, it turns out that all of the limit laws continue to hold. However, as we will not be using these limits much in this text, we will not devote much attention to these matters. We will note though that this definition is consistent with the notion of a limit $\operatorname* { l i m } _ { n \to \infty } a _ { n }$ of a sequence (Exercise 9.10.1). 

$$
- \text { Exercises } -
$$

Exercise 9.10.1. Let $( a _ { n } ) _ { n = 0 } ^ { \infty }$ be a sequence of real numbers, then $a _ { n }$ can also be thought of as a function from N to R, which takes each natural number n to a real number $a _ { n }$ . Show that 

$$
\lim _ {n \to + \infty ; n \in {\bf N}} a _ {n} = \lim _ {n \to \infty} a _ {n}
$$

where the left-hand limit is defined by Definition 9.10.3 and the right-hand limit is defined by Definition 6.1.8. More precisely, show that if one of the above two limits exists then so does the other, and then they both have the same value. Thus the two notions of limit here are compatible. 

## Chapter 10

## Diferentiation of functions

## 10.1 Basic definitions

We can now begin the rigorous treatment of calculus in earnest, starting with the notion of a derivative. We can now define derivatives analytically, using limits, in contrast to the geometric definition of derivatives, which uses tangents. The advantage of working analytically is that (a) we do not need to know the axioms of geometry, and (b) these definitions can be modified to handle functions of several variables, or functions whose values are vectors instead of scalar. Furthermore, one’s geometric intuition becomes dificult to rely on once one has more than three dimensions in play. (Conversely, one can use one’s experience in analytic rigour to extend one’s geometric intuition to such abstract settings; as mentioned earlier, the two viewpoints complement rather than oppose each other.) 

Definition 10.1.1 (Diferentiability at a point). Let X be a subset of R, and let $x _ { 0 } \in X$ be an element of X which is also a limit point of X. Let $f : X  \mathbf { R }$ be a function. If the limit 

$$
\lim _ {x \to x _ {0}; x \in X - \{x _ {0} \}} \frac {f (x) - f (x _ {0})}{x - x _ {0}}
$$

converges to some real number $L$ , then we say that f is diferentiable at $x _ { 0 }$ on X with derivative $L$ , and write $f ^ { \prime } ( x _ { 0 } ) : = L$ . If the limit does not exist, or if $x _ { 0 }$ is not an element of X or not a limit point of $X$ , we leave $f ^ { \prime } ( x _ { 0 } )$ undefined, and say that f is not diferentiable at $x _ { 0 }$ on $X$ . 

Remark 10.1.2. Note that we need $x _ { 0 }$ to be a limit point in order for $x _ { 0 }$ to be adherent to $X - \{ x _ { 0 } \}$ , otherwise the limit 

$$
\lim _ {x \to x _ {0}; x \in X - \{x _ {0} \}} \frac {f (x) - f (x _ {0})}{x - x _ {0}}
$$

would automatically be undefined. In particular, we do not define the derivative of a function at an isolated point; for instance, if one restricts the function $f : \mathbf { R }  \mathbf { R }$ defined by $f ( x ) : = x ^ { 2 }$ to the domain $X : =$ $[ 1 , 2 ] \cup \{ 3 \}$ , then the restriction of the function ceases to be diferentiable at 3. (See however Exercise 10.1.1 below.) In practice, the domain X will almost always be an interval, and so by Lemma 9.1.21 all elements $x _ { 0 }$ of X will automatically be limit points and we will not have to care much about these issues. 

Example 10.1.3. Let $f : \mathbf { R }  \mathbf { R }$ be the function $f ( x ) : = x ^ { 2 }$ , and let $x _ { 0 }$ be any real number. To see whether $f$ is diferentiable at $x _ { 0 }$ on $\mathbf { R }$ we compute the limit 

$$
\lim _ {x \to x _ {0}; x \in \mathbf {R} - \{x _ {0} \}} \frac {f (x) - f (x _ {0})}{x - x _ {0}} = \lim _ {x \to x _ {0}; x \in \mathbf {R} - \{x _ {0} \}} \frac {x ^ {2} - x _ {0} ^ {2}}{x - x _ {0}}.
$$

We can factor the numerator as $( x ^ { 2 } - x _ { 0 } ^ { 2 } ) = ( x - x _ { 0 } ) ( x + x _ { 0 } )$ . Since $x \in \mathbf { R } - \{ x _ { 0 } \}$ , we may legitimately cancel the factors of $x - x _ { 0 }$ and write the above limit as 

$$
\lim _ {x \to x _ {0}; x \in \mathbf {R} - \{x _ {0} \}} x + x _ {0}
$$

which by limit laws is equal to $2 x _ { 0 }$ . Thus the function $f ( x )$ is diferentiable at $x _ { 0 }$ and its derivative there is $2 x _ { 0 }$ 

Remark 10.1.4. This point is trivial, but it is worth mentioning: if $f : X \to \mathbf { R }$ is diferentiable at $x _ { 0 }$ , and $g \ : \ X \ \to \ \mathbf { R }$ is equal to $f$ $( { \mathrm { i . e . , ~ } } g ( x ) = f ( x )$ for all $x \in X )$ , then $g$ is also diferentiable at $x _ { 0 }$ and $g ^ { \prime } ( x _ { 0 } ) = f ^ { \prime } ( x _ { 0 } ) \ \mathrm { ( w h y ? ) }$ . However, if two functions $f$ and $g$ merely have the same value at x , i.e., $g ( x _ { 0 } ) = f ( x _ { 0 } )$ , this does not imply that $g ^ { \prime } ( x _ { 0 } ) = f ^ { \prime } ( x _ { 0 } )$ . (Can you see a counterexample?) Thus there is a big diference between two functions being equal on their whole domain, and merely being equal at one point. 

Remark 10.1.5. One sometimes writes $\textstyle { \frac { d f } { d x } }$ instead of $f ^ { \prime }$ . This notation is of course very familiar and convenient, but one has to be a little careful, because it is only safe to use as long as x is the only variable used to represent the input for $f ;$ otherwise one can get into all sorts of trouble. For instance, the function $f : \mathbf { R }  \mathbf { R }$ defined by $f ( x ) : = x ^ { 2 }$ has derivative $\begin{array} { r } { \frac { d f } { d x } = 2 x } \end{array}$ , but the function $g : \mathbf { R }  \mathbf { R }$ defined by $g ( y ) : =$ $y ^ { 2 }$ would seem to have derivative $\begin{array} { r } { \frac { d g } { d x } = 0 \mathrm { ~ i f ~ } y } \end{array}$ and x are independent variables, despite the fact that g and f are exactly the same function. Because of this possible source of confusion, we will refrain from using the notation $\textstyle { \frac { d f } { d x } }$ whenever it could possibly lead to confusion. (This confusion becomes even worse in the calculus of several variables, and the standard notation of $\textstyle { \frac { \partial f } { \partial x } }$ can lead to some serious ambiguities. There are ways to resolve these ambiguities, most notably by introducing the notion of diferentiation along vector fields, but this is beyond the scope of this text.) 

Example 10.1.6. Let $f : \mathbf { R }  \mathbf { R }$ be the function $f ( x ) : = | x |$ , and let $x _ { 0 } = 0$ . To see whether f is diferentiable at 0 on R, we compute the limit 

$$
\lim _ {x \to 0; x \in {\bf R} - \{0 \}} \frac {f (x) - f (0)}{x - 0} = \lim _ {x \to 0; x \in {\bf R} - \{0 \}} \frac {| x |}{x}.
$$

Now we take left limits and right limits. The right limit is 

$$
\lim _ {x \to 0; x \in (0, \infty)} \frac {| x |}{x} = \lim _ {x \to 0; x \in (0, \infty)} \frac {x}{x} = \lim _ {x \to 0; x \in (0, \infty)} 1 = 1,
$$

while the left limit is 

$$
\lim _ {x \to 0; x \in (- \infty , 0)} \frac {| x |}{x} = \lim _ {x \to 0; x \in (0, \infty)} \frac {- x}{x} = \lim _ {x \to 0; x \in (0, \infty)} - 1 = - 1,
$$

and these limits do not match. Thus $\begin{array} { r } { \operatorname* { l i m } _ { x  0 ; x \in \mathbf { R } - \{ 0 \} } \frac { | x | } { x } } \end{array}$ does not exist, and f is not diferentiable at 0 on R. However, if one restricts f to $[ 0 , \infty )$ , then the restricted function $f | _ { [ 0 , \infty ) }$ is diferentiable at 0 on $[ 0 , \infty )$ , with derivative 1: 

$$
\lim _ {x \to 0; x \in [ 0, \infty) - \{0 \}} \frac {f (x) - f (0)}{x - 0} = \lim _ {x \to 0; x \in (0, \infty)} \frac {| x |}{x} = 1.
$$

Similarly, when one restricts f to $( - \infty , 0 ]$ , the restricted function $f | _ { ( - \infty , 0 ] }$ is diferentiable at 0 on $( - \infty , 0 ]$ , with derivative 1. Thus even when a function is not diferentiable, it is sometimes possible to restore the diferentiability by restricting the domain of the function. 

If a function is diferentiable at $x _ { 0 }$ , then it is approximately linear near x : 

Proposition 10.1.7 (Newton’s approximation). Let X be a subset of R, let $x _ { 0 } \in X$ be a limit point of X, let $f : X \to \mathbf { R }$ be a function, and let L be a real number. Then the following statements are logically equivalent: 

(a) f is diferentiable at x on X with derivative L. 

(b) For every $\varepsilon > 0$ , there exists a $\delta > 0$ such that $f ( x )$ is $\varepsilon | x - x _ { 0 } | -$ close to $f ( x _ { 0 } ) + L ( x - x _ { 0 } )$ whenever $x \in X$ is δ-close to x , i.e., we have 

$$
| f (x) - (f (x _ {0}) + L (x - x _ {0})) | \leq \varepsilon | x - x _ {0} |
$$

whenever $x \in X$ and $| x - x _ { 0 } | \leq \delta$ 

Remark 10.1.8. Newton’s approximation is of course named after the great scientist and mathematician Isaac Newton (1642–1727), one of the founders of diferential and integral calculus. 

Proof. See Exercise 10.1.2. 

Remark 10.1.9. We can phrase Proposition 10.1.7 in a more informa way: if f is diferentiable at $x _ { 0 }$ , then one has the approximation $f ( x ) \approx$ $f ( x _ { 0 } ) + f ^ { \prime } ( x _ { 0 } ) ( x - x _ { 0 } )$ , and conversely. 

As the example of the function $f : \mathbf { R }  \mathbf { R }$ defined by $f ( x ) : = | x |$ shows, a function can be continuous at a point without being diferentiable at that point. However, the converse is true: 

Proposition 10.1.10 (Diferentiability implies continuity). Let X be a subset of R, let $x _ { 0 } \in X$ be a limit point of X, and let $f : X  \mathbf { R }$ be a function. If f is diferentiable at $x _ { 0 }$ , then f is also continuous at x . 

Proof. See Exercise 10.1.3. 

Definition 10.1.11 (Diferentiability on a domain). Let X be a subset of R, and let $f : X  \mathbf { R }$ be a function. We say that f is diferentiable on X if, for every limit point $x _ { 0 } \in X$ , the function f is diferentiable at x on X. 

From Proposition 10.1.10 and the above definition we have an immediate corollary: 

Corollary 10.1.12. Let X be a subset of R, and let $f : X  \mathbf { R }$ be a function which is diferentiable on X. Then f is also continuous on X. 

## 10.1. Basic definitions

Now we state the basic properties of derivatives which you are all familiar with. 

Theorem 10.1.13 (Diferential calculus). Let X be a subset of R, let $x _ { 0 } \in X$ be a limit point of X, and let $f : X \to \mathbf { R }$ and $g : X  \mathbf { R }$ be functions. 

(a) If f is a constant function, i.e., there exists a real number c such that $f ( x ) = c$ for all $x \in X$ , then f is diferentiable at $x _ { 0 }$ and $f ^ { \prime } ( x _ { 0 } ) = 0$ 

(b) If f is the identity function, i.e., $f ( x ) = x$ for all $x \in X$ , then f is diferentiable at x and $f ^ { \prime } ( x _ { 0 } ) = 1$ 

(c) (Sum rule) If f and g are diferentiable at x<sub>0</sub>, then $f + g$ is also diferentiable at x , and $( f + g ) ^ { \prime } ( x _ { 0 } ) = f ^ { \prime } ( x _ { 0 } ) + g ^ { \prime } ( x _ { 0 } )$ 

(d) (Product rule) If f and g are diferentiable at x , then fg is also diferentiable at x<sub>0</sub>, and $( f g ) ^ { \prime } ( x _ { 0 } ) = f ^ { \prime } ( x _ { 0 } ) g ( x _ { 0 } ) + f ( x _ { 0 } ) g ^ { \prime } ( x _ { 0 } )$ 

(e) If f is diferentiable at x and c is a real number, then cf is also diferentiable at x , and $( c f ) ^ { \prime } ( x _ { 0 } ) = c f ^ { \prime } ( x _ { 0 } )$ 

(f) (Diference rule) If f and g are diferentiable at x , then $f - g$ is also diferentiable at x , and $( f - g ) ^ { \prime } ( x _ { 0 } ) = f ^ { \prime } ( x _ { 0 } ) - g ^ { \prime } ( x _ { 0 } )$ 

(g) If g is diferentiable at x , and g is non-zero on X $( i . e . , g ( x ) \neq 0$ for all $x \in X )$ , then 1/g is also diferentiable at x<sub>0</sub>, and $\begin{array} { r l } {  { \big ( \frac { 1 } { g } \big ) ^ { \prime } \big ( x _ { 0 } \big ) = } } \end{array}$ $\frac { g ^ { \prime } ( x _ { 0 } ) } { g ( x _ { 0 } ) ^ { 2 } }$ 

(h) (Quotient rule) If f and g are diferentiable at x , and g is nonzero on X, then f/g is also diferentiable at x , and 

$$
(\frac {f}{g}) ^ {\prime} (x _ {0}) = \frac {f ^ {\prime} (x _ {0}) g (x _ {0}) - f (x _ {0}) g ^ {\prime} (x _ {0})}{g (x _ {0}) ^ {2}}.
$$

Remark 10.1.14. The product rule is also known as the Leibniz rule, after Gottfried Leibniz (1646–1716), who was the other founder of differential and integral calculus besides Newton. 

Proof. See Exercise 10.1.4. 

As you are well aware, the above rules allow one to compute many derivatives easily. For instance, if $f : \mathbf { R } - \{ 1 \}  \mathbf { R }$ is the function $\textstyle f ( x ) : = { \frac { x - 2 } { x - 1 } }$ , then it is easy to use the above rules to show that $f ^ { \prime } ( x _ { 0 } ) =$ $\frac { 1 } { ( x _ { 0 } - 1 ) ^ { 2 } }$ for all $x _ { 0 } \in \mathbf { R } - \{ 1 \}$ . (Why? Note that every point $x _ { 0 }$ in $\mathbf { R } - \{ 1 \}$ is a limit point of $\mathbf { R } - \{ 1 \} . )$ 

Another fundamental property of diferentiable functions is the following: 

Theorem 10.1.15 (Chain rule). Let X, Y be subsets of R, let $x _ { 0 } \in X$ be a limit point of X, and let $y _ { 0 } \in Y$ be a limit point of Y. Let $f : X \to Y$ be a function such that $f ( x _ { 0 } ) = y _ { 0 }$ , and such that f is diferentiable at $x _ { 0 }$ . Suppose that $g : Y  \mathbf { R }$ is a function which is diferentiable at $y _ { 0 }$ Then the function $g \circ f : X  \mathbf { R }$ is diferentiable at $x _ { 0 }$ , and 

$$
(g \circ f) ^ {\prime} (x _ {0}) = g ^ {\prime} (y _ {0}) f ^ {\prime} (x _ {0}).
$$

Proof. See Exercise 10.1.7. 

Example 10.1.16. If $f : \mathbf { R } - \{ 1 \}  \mathbf { R }$ is the function $\textstyle f ( x ) : = { \frac { x - 2 } { x - 1 } }$ • and $g : \mathbf { R }  \mathbf { R }$ is the function $g ( y ) : = y ^ { 2 }$ , then $\textstyle g \circ f ( x ) = ( { \frac { x - 2 } { x - 1 } } ) ^ { 2 }$ , and the chain rule gives 

$$
(g \circ f) ^ {\prime} (x _ {0}) = 2 \left(\frac {x _ {0} - 2}{x _ {0} - 1}\right) \frac {1}{(x _ {0} - 1) ^ {2}}.
$$

Remark 10.1.17. If one writes y for $f ( x )$ , and $z$ for $g ( y )$ , then the chain rule can be written in the more visually appealing manner $\begin{array} { r } { \frac { d z } { d x } = } \end{array}$ $\frac { d z } { d y } \frac { d y } { d x }$ . However, this notation can be misleading (for instance it blurs the distinction between dependent variable and independent variable, especially for $y )$ , and leads one to believe that the quantities $d z , d y$ , dx can be manipulated like real numbers. However, these quantities are not real numbers (in fact, we have not assigned any meaning to them at all), and treating them as such can lead to problems in the future. For instance, if f depends on $x _ { 1 }$ and $x _ { 2 }$ , which depend on $t ,$ then chain rule for several variables asserts that $\begin{array} { r } { \frac { d f } { d t } = \frac { \partial f } { \partial x _ { 1 } } \frac { d x _ { 1 } } { d t } + \frac { \partial f } { \partial x _ { 2 } } \frac { d x _ { 2 } } { d t } } \end{array}$ , but this rule might seem suspect if one treated $d f$ , dt, etc. as real numbers. It is possible to think of $d y , d x$ , etc. as “infinitesimal real numbers” if one knows what one is doing, but for those just starting out in analysis, I would not recommend this approach, especially if one wishes to work rigorously. (There is a way to make all of this rigorous, even for the calculus of several variables, but it requires the notion of a tangent vector, and the derivative map, both of which are beyond the scope of this text.) 

— Exercises — 

Exercise 10.1.1. Suppose that X is a subset of $\mathbf { R } , x _ { 0 }$ is a limit point of $X$ , and $f : X \to \mathbf { R }$ is a function which is diferentiable at $x _ { 0 }$ . Let $Y \subset X$ be such that $x _ { 0 } \in Y$ , and $x _ { 0 }$ is also a limit point of $Y$ . Prove that the restricted function $f | _ { Y } : Y  \mathbf { R }$ is also diferentiable at $x _ { 0 }$ , and has the same derivative as f at $x _ { 0 }$ . Explain why this does not contradict the discussion in Remark 10.1.2. 

Exercise 10.1.2. Prove Proposition 10.1.7. (Hint: the cases $x = x _ { 0 }$ and $x \neq x _ { 0 }$ have to be treated separately.) 

Exercise 10.1.3. Prove Proposition 10.1.10. (Hint: either use the limit laws (Proposition 9.3.14), or use Proposition 10.1.7.) 

Exercise 10.1.4. Prove Theorem 10.1.13. (Hint: use the limit laws in Proposition 9.3.14. Use earlier parts of this theorem to prove the latter. For the product rule, use the identity 

$$
\begin{array}{r l} & f (x) g (x) - f (x _ {0}) g (x _ {0}) \\ & \quad = f (x) g (x) - f (x) g (x _ {0}) + f (x) g (x _ {0}) - f (x _ {0}) g (x _ {0}) \\ & \quad = f (x) (g (x) - g (x _ {0})) + (f (x) - f (x _ {0})) g (x _ {0}); \end{array}
$$

this trick of adding and subtracting an intermediate term is sometimes known as the “middle-man trick” and is very useful in analysis.) 

Exercise 10.1.5. Let n be a natural number, and let $f : \mathbf { R }  \mathbf { R }$ be the function $f ( x ) \ : = \ x ^ { n }$ . Show that f is diferentiable on R and $f ^ { \prime } ( x ) \ = \ n x ^ { n - 1 }$ for all $x \in \mathbf { R }$ . (Hint: use Theorem 10.1.13 and induction.) 

Exercise 10.1.6. Let n be a negative integer, and let $f : \mathbf { R } - \{ 0 \}  { \mathbf { R } }$ be the function $f ( x ) : = x ^ { n }$ . Show that f is diferentiable on R and $f ^ { \prime } ( x ) = n x ^ { n - 1 }$ for all $x \in \mathbf { R } - \{ 0 \}$ . (Hint: use Theorem 10.1.13 and Exercise 10.1.5.) 

Exercise 10.1.7. Prove Theorem 10.1.15. (Hint: one way to do this is via Newton’s approximation, Proposition 10.1.7. Another way is to use Proposition 9.3.9 and Proposition 10.1.10 to convert this problem into one involving limits of sequences, however with the latter strategy one has to treat the case $f ^ { \prime } ( x _ { 0 } ) = 0$ separately, as some division-by-zero subtleties can occur in that case.) 

## 10.2 Local maxima, local minima, and derivatives

As you learnt in your basic calculus courses, one very common application of using derivatives is to locate maxima and minima. We now present this material again, but this time in a rigorous manner. 

The notion of a function $f : X  \mathbf { R }$ attaining a maximum or minimum at a point $x _ { 0 } \in X$ was defined in Definition 9.6.5. We now localize this definition: 

Definition 10.2.1 (Local maxima and minima). Let $f : X \to \mathbf { R }$ be a function, and let $x _ { 0 } \in X$ . We say that $f$ attains a local maximum at $x _ { 0 }$ if there exists $\mathrm { ~ a ~ } \delta > 0$ such that the restriction $f | _ { X \cap ( x _ { 0 } - \delta , x _ { 0 } + \delta ) }$ of $f$ to $X \cap ( x _ { 0 } - \delta , x _ { 0 } + \delta )$ attains a maximum at $x _ { 0 }$ . We say that $f$ attains a local minimum at $x _ { 0 }$ if there exists a $\delta > 0$ such that the restriction $f | _ { X \cap ( x _ { 0 } - \delta , x _ { 0 } + \delta ) }$ of $f$ to $X \cap ( x _ { 0 } - \delta , x _ { 0 } + \delta )$ attains a minimum at $x _ { 0 }$ 

Remark 10.2.2. If $f$ attains a maximum at $x _ { 0 }$ , we sometimes say that $f$ attains a global maximum at $x _ { 0 }$ , in order to distinguish it from the local maxima defined here. Note that if $f$ attains a global maximum at $x _ { 0 }$ , then it certainly also attains a local maximum at this $x _ { 0 }$ , and similarly for minima. 

Example 10.2.3. Let $f : \mathbf { R }  \mathbf { R }$ denote the function $f ( x ) : = x ^ { 2 } - x ^ { 4 }$ This function does not attain a global minimum at $0 ,$ , since for example $f ( 2 ) = - 1 2 < 0 = f ( 0 )$ , however it does attain a local minimum, for if we choose $\delta : = 1$ and restrict $f$ to the interval $( - 1 , 1 )$ , then for all $x \in ( - 1 , 1 )$ we have $x ^ { 4 } \leq x ^ { 2 }$ and thus $f ( x ) = x ^ { 2 } - x ^ { 4 } \geq 0 = f ( 0 )$ , and so $f | _ { ( - 1 , 1 ) }$ has a local minimum at 0. 

Example 10.2.4. Let $f : \mathbf { Z }  \mathbf { R }$ be the function $f ( x ) = x ,$ , defined on the integers only. Then f has no global maximum or global minimum $\mathrm { \left( w h y ? \right) }$ , but attains both a local maximum and local minimum at every integer $n \ \mathrm { ( w h y ? ) }$ 

Remark 10.2.5. If $f : X  \mathbf { R }$ attains a local maximum at a point $x _ { 0 }$ in $X$ , and $Y \subset X$ is a subset of X which contains $x _ { 0 }$ , then the restriction $f | _ { Y } : Y  \mathbf { R }$ also attains a local maximum at $x _ { 0 } \ \mathrm { ( w h y ? ) }$ . Similarly for minima. 

The connection between local maxima, minima and derivatives is the following. 

Proposition 10.2.6 (Local extrema are stationary). Let $a < b$ be real numbers, and let $f : ( a , b )  \mathbf { R }$ be a function. If $x _ { 0 } \in ( a , b )$ , f is diferentiable at $x _ { 0 }$ , and f attains either a local maximum or local minimum at $x _ { 0 }$ , then $f ^ { \prime } ( x _ { 0 } ) = 0$ 

Proof. See Exercise 10.2.1. 

Note that f must be diferentiable for this proposition to work; see Exercise 10.2.2. Also, this proposition does not work if the open interval $( a , b )$ is replaced by a closed interval $[ a , b ]$ . For instance, the function $f : [ 1 , 2 ]  \mathbf { R }$ defined by $f ( x ) : = x$ has a local maximum at $x _ { 0 } = 2$ and a local minimum $x _ { 0 } = 1$ (in fact, these local extrema are global extrema), but at both points the derivative is $f ^ { \prime } ( x _ { 0 } ) = 1$ , not $f ^ { \prime } ( x _ { 0 } ) = 0$ . Thus the endpoints of an interval can be local maxima or minima even if the derivative is not zero there. Finally, the converse of this proposition is false (Exercise 10.2.3). 

By combining Proposition 10.2.6 with the maximum principle, one can obtain 

Theorem 10.2.7 (Rolle’s theorem). Let $a < b$ be real numbers, and let $g : [ a , b ]  \mathbf { R }$ be a continuous function which is diferentiable on $( a , b )$ Suppose also that $g ( a ) = g ( b )$ . Then there exists an $x \in ( a , b )$ such that $g ^ { \prime } ( x ) = 0$ 

Proof. See Exercise 10.2.4. 

Remark 10.2.8. Note that we only assume f is diferentiable on the open interval $( a , b )$ , though of course the theorem also holds if we assume f is diferentiable on the closed interval $[ a , b ]$ , since this is larger than $( a , b )$ 

Rolle’s theorem has an important corollary. 

Corollary 10.2.9 (Mean value theorem). Let $a < b$ be real numbers, and let $f : [ a , b ]  \mathbf { R }$ be a function which is continuous on $[ a , b ]$ and diferentiable on $( a , b )$ . Then there exists an $x \in ( a , b )$ such that $f ^ { \prime } ( x ) =$ $\frac { f ( \bar { b } ) - f ( a ) } { b - a }$ 

Proof. See Exercise 10.2.5. 

— Exercises — 

Exercise 10.2.1. Prove Proposition 10.2.6. 

Exercise 10.2.2. Give an example of a function $f : ( - 1 , 1 ) \  \ \mathbf { R }$ which is continuous and attains a global maximum at 0, but which is not diferentiable at 0. Explain why this does not contradict Proposition 10.2.6. 

Exercise 10.2.3. Give an example of a function $f : ( - 1 , 1 ) \  \ \mathbf { R }$ which is diferentiable, and whose derivative equals 0 at 0, but such that 0 is neither a local minimum nor a local maximum. Explain why this does not contradict Proposition 10.2.6. 

Exercise 10.2.4. Prove Theorem 10.2.7. (Hint: use Corollary 10.1.12 and the maximum principle, Proposition 9.6.7, followed by Proposition 10.2.6. Note that the maximum principle does not tell you whether the maximum or minimum is in the open interval $( a , b )$ or is one of the boundary points $a , b ,$ so you have to divide into cases and use the hypothesis $g ( a ) = g ( b )$ somehow.) 

Exercise 10.2.5. Use Theorem 10.2.7 to prove Corollary 10.2.9. (Hint: consider a function of the form $f ( x ) - c x$ for some carefully chosen real number c.) 

Exercise 10.2.6. Let $M > 0$ , and let $f : [ a , b ]  \mathbf { R }$ be a function which is continuous on $[ a , b ]$ and diferentiable on $( a , b )$ , and such that $| f ^ { \prime } ( x ) | \leq M$ for all $x \in ( a , b )$ (i.e., the derivative of f is bounded). Show that for any $x , y \in [ a , b ]$ we have the inequality $| f ( x ) - f ( y ) | \leq M | x - y |$ . (Hint: apply the mean value theorem (Corollary 10.2.9) to a suitable restriction of $f . )$ Functions which obey the bound $| f ( x ) - f ( y ) | \leq M | x - y |$ are known as Lipschitz continuous functions with Lipschitz constant $M ;$ thus this exercise shows that functions with bounded derivative are Lipschitz continuous. 

Exercise 10.2.7. Let $f : \textbf { R }  \textbf { R }$ be a diferentiable function such that $f ^ { \prime }$ is bounded. Show that $f$ is uniformly continuous. (Hint: use the preceding exercise.) 

## 10.3 Monotone functions and derivatives

In your elementary calculus courses, you may have come across the assertion that a positive derivative meant an increasing function, and a negative derivative meant a decreasing function. This statement is not completely accurate, but it is pretty close; we now give the precise version of these statements below. 

Proposition 10.3.1. Let X be a subset of R, let $x _ { 0 } \in X$ be a limit point of X, and let $f : X \to \mathbf { R }$ be a function. If f is monotone increasing and f is diferentiable at $x _ { 0 }$ , then $f ^ { \prime } ( x _ { 0 } ) \geq 0$ . If f is monotone decreasing and $f$ is diferentiable at x , then $f ^ { \prime } ( x _ { 0 } ) \leq 0$ 

Proof. See Exercise 10.3.1. 

Remark 10.3.2. We have to assume that $f$ is diferentiable at $x _ { 0 } ;$ There exist monotone functions which are not always diferentiable (see Exercise 10.3.2), and of course if f is not diferentiable at $x _ { 0 }$ we cannot possibly conclude that $f ^ { \prime } ( x _ { 0 } ) \geq 0 \mathrm { ~ o r ~ } f ^ { \prime } ( x _ { 0 } ) \leq 0$ 

One might naively guess that if f were strictly monotone increasing, and f was diferentiable at $x _ { 0 }$ , then the derivative $f ^ { \prime } ( x _ { 0 } )$ would be strictly positive instead of merely non-negative. Unfortunately, this is not always the case (Exercise 10.3.3). 

On the other hand, we do have a converse result: if function has strictly positive derivative, then it must be strictly monotone increasing: 

Proposition 10.3.3. Let $a < b _ { : }$ , and let $f : [ a , b ]  \mathbf { R }$ be a diferentiable function. If $f ^ { \prime } ( x ) > 0$ for all $x \in [ a , b ]$ , then f is strictly monotone increasing. If $f ^ { \prime } ( x ) < 0$ for all $x \in [ a , b ]$ , then f is strictly monotone decreasing. $I f ^ { \prime } f ^ { \prime } ( x ) = 0$ for all $x \in [ a , b ]$ , then f is a constant function. 

Proof. See Exercise 10.3.4. 

— Exercises — 

Exercise 10.3.1. Prove Proposition 10.3.1. 

Exercise 10.3.2. Give an example of a function $f : ( - 1 , 1 ) \to \mathbf { R }$ which is continuous and monotone increasing, but which is not diferentiable at 0. Explain why this does not contradict Proposition 10.3.1. 

Exercise 10.3.3. Give an example of a function $f : \mathbf { R }  \mathbf { R }$ which is strictly monotone increasing and diferentiable, but whose derivative at 0 is zero. Explain why this does not contradict Proposition 10.3.1 or Proposition 10.3.3. (Hint: look at Exercise 10.2.3.) 

Exercise 10.3.4. Prove Proposition 10.3.3. (Hint: you do not have integrals or the fundamental theorem of calculus yet, so these tools cannot be used. However, one can proceed via the mean-value theorem, Corollary 10.2.9.) 

Exercise 10.3.5. Give an example of a subset $X \subset \mathbf { R }$ and a function $f : X  \mathbf { R }$ which is diferentiable on X, is such that $f ^ { \prime } ( x ) > 0$ for all $x \in X$ , but f is not strictly monotone increasing. (Hint: the conditions here are subtly diferent from those in Proposition 10.3.3. What is the diference, and how can one exploit that diference to obtain the example?) 

## 10.4 Inverse functions and derivatives

We now ask the following question: if we know that a function $f :$ $X  Y$ is diferentiable, and it has an inverse $f ^ { - 1 } : Y \to X$ , what can we say about the diferentiability of $f ^ { - 1 } \ ?$ This will be useful for many applications, for instance if we want to diferentiate the function $f ( x ) : = x ^ { 1 / n }$ 

We begin with a preliminary result. 

Lemma 10.4.1. Let $f : X \to Y$ be an invertible function, with inverse $f ^ { - 1 } : Y \to X$ . Suppose that $x _ { 0 } \in X$ and $y _ { 0 } \in Y$ are such that $y _ { 0 } = f ( x _ { 0 } )$ (which also implies that $x _ { 0 } = f ^ { - 1 } ( y _ { 0 } ) )$ . If f is diferentiable at $x _ { 0 }$ , and $f ^ { - 1 }$ is diferentiable at $y _ { 0 }$ , then 

$$
(f ^ {- 1}) ^ {\prime} (y _ {0}) = \frac {1}{f ^ {\prime} (x _ {0})}.
$$

Proof. From the chain rule (Theorem 10.1.15) we have 

$$
(f ^ {- 1} \circ f) ^ {\prime} (x _ {0}) = (f ^ {- 1}) ^ {\prime} (y _ {0}) f ^ {\prime} (x _ {0}).
$$

But $f ^ { - 1 } \circ f$ is the identity function on $X .$ , and hence by Theorem $1 0 . 1 . 1 3 ( \mathrm { b } ) ~ ( f ^ { - 1 } \circ f ) ^ { \prime } ( x _ { 0 } ) = 1$ . The claim follows. □ 

As a particular corollary of Lemma 10.4.1, we see that if f is differentiable at $x _ { 0 }$ with $f ^ { \prime } ( x _ { 0 } ) = 0$ , then $f ^ { - 1 }$ cannot be diferentiable at $y _ { 0 } = f ( x _ { 0 } )$ , since $1 / f ^ { \prime } ( x _ { 0 } )$ is undefined in that case. Thus for instance, the function $g : [ 0 , \infty ) \to [ 0 , \infty )$ defined by $g ( y ) : = y ^ { 1 / 3 }$ cannot be diferentiable at 0, since this function is the inverse $g = f ^ { - 1 }$ of the function $f : [ 0 , \infty ) \to [ 0 , \infty )$ defined by $f ( x ) \ : = \ x ^ { 3 }$ , and this function has a derivative of 0 at $f ^ { - 1 } ( 0 ) = 0$ 

If one writes $y \ = \ f ( x )$ , so that $x = f ^ { - 1 } ( y )$ , then one can write the conclusion of Lemma 10.4.1 in the more appealing form $d x / d y =$ $1 / ( d y / d x )$ . However, as mentioned before, this way of writing things, while very convenient and easy to remember, can be misleading and cause errors if applied too carelessly (especially when one begins to work in the calculus of several variables). 

Lemma 10.4.1 seems to answer the question of how to diferentiate the inverse of a function, however it has one significant drawback: the lemma only works if one assumes a priori that $f ^ { - 1 }$ is diferentiable. Thus, if one does not already know that $f ^ { - 1 }$ is diferentiable, one cannot use Lemma 10.4.1 to compute the derivative of $f ^ { - 1 }$ 

However, the following improved version of Lemma 10.4.1 will compensate for this fact, by relaxing the requirement on $f ^ { - 1 }$ from diferentiability to continuity. 

Theorem 10.4.2 (Inverse function theorem). Let $f : X \to Y$ be an invertible function, with inverse $f ^ { - 1 } : Y \to X$ . Suppose that $x _ { 0 } \in X$ and $y _ { 0 } \in Y$ are such that $f ( x _ { 0 } ) = y _ { 0 }$ . If f is diferentiable at $x _ { 0 } , f ^ { - 1 }$ is continuous at $y _ { 0 }$ , and $f ^ { \prime } ( x _ { 0 } ) \neq 0$ , then $f ^ { - 1 }$ is diferentiable at $y _ { 0 }$ and 

$$
(f ^ {- 1}) ^ {\prime} (y _ {0}) = \frac {1}{f ^ {\prime} (x _ {0})}.
$$

Proof. We have to show that 

$$
\lim _ {y \to y _ {0}; y \in Y - \{y _ {0} \}} \frac {f ^ {- 1} (y) - f ^ {- 1} (y _ {0})}{y - y _ {0}} = \frac {1}{f ^ {\prime} (x _ {0})}.
$$

By Proposition 9.3.9, it sufices to show that 

$$
\lim _ {n \to \infty} \frac {f ^ {- 1} (y _ {n}) - f ^ {- 1} (y _ {0})}{y _ {n} - y _ {0}} = \frac {1}{f ^ {\prime} (x _ {0})}
$$

for any sequence $( y _ { n } ) _ { n = 1 } ^ { \infty }$ of elements in $Y - \{ y _ { 0 } \}$ which converge to $y _ { 0 }$ 

To prove this, we set $x _ { n } : = f ^ { - 1 } ( y _ { n } )$ . Then $( x _ { n } ) _ { n = 1 } ^ { \infty }$ is a sequence of elements in $X - \{ x _ { 0 } \}$ . (Why? Note that $f ^ { - 1 }$ is a bijection) Since $f ^ { - 1 }$ is continuous by assumption, we know that $x _ { n } = f ^ { - 1 } ( y _ { n } )$ converges to $f ^ { - 1 } ( y _ { 0 } ) = x _ { 0 }$ as $n \to \infty$ . Thus, since $f$ is diferentiable at $x _ { 0 }$ , we have (by Proposition 9.3.9 again) 

$$
\lim _ {n \to \infty} \frac {f (x _ {n}) - f (x _ {0})}{x _ {n} - x _ {0}} = f ^ {\prime} (x _ {0}).
$$

But since $x _ { n } \neq x _ { 0 }$ and $f$ is a bijection, the fraction $\frac { f ( x _ { n } ) - f ( x _ { 0 } ) } { x _ { n } - x _ { 0 } }$ is nonzero. Also, by hypothesis $f ^ { \prime } ( x _ { 0 } )$ is non-zero. So by limit laws 

$$
\lim _ {n \to \infty} \frac {x _ {n} - x _ {0}}{f (x _ {n}) - f (x _ {0})} = \frac {1}{f ^ {\prime} (x _ {0})}.
$$

But since $x _ { n } = f ^ { - 1 } ( y _ { n } )$ and $x _ { 0 } = f ^ { - 1 } ( y _ { 0 } )$ , we thus have 

$$
\lim _ {n \to \infty} \frac {f ^ {- 1} (y _ {n}) - f ^ {- 1} (y _ {0})}{y _ {n} - y _ {0}} = \frac {1}{f ^ {\prime} (x _ {0})}
$$

as desired. 

□ 

We give some applications of the inverse function theorem in the exercises below. 

— Exercises — 

Exercise 10.4.1. Let $n \geq 1$ be a natural number, and let $g : ( 0 , \infty ) \to ( 0 , \infty )$ be the function $g ( x ) : = x ^ { 1 / n }$ 

(a) Show that g is continuous on $( 0 , \infty )$ . (Hint: use Proposition 9.8.3.) 

(b) Show that g is diferentiable on $( 0 , \infty )$ , and that $\begin{array} { r } { g ^ { \prime } ( x ) = \frac { 1 } { n } x ^ { \frac { 1 } { n } - 1 } } \end{array}$ for all $x \in ( 0 , \infty )$ . (Hint: use the inverse function theorem and (a).) 

Exercise 10.4.2. Let q be a rational number, and let $f : ( 0 , \infty ) \to \mathbf { R }$ be the function $f ( x ) = x ^ { q }$ 

(a) Show that f is diferentiable on $( 0 , \infty )$ and that $f ^ { \prime } ( x ) = q x ^ { q - 1 }$ . (Hint: use Exercise 10.4.1 and the laws of diferential calculus in Theorem 10.1.13 and Theorem 10.1.15.) 

(b) Show that $\begin{array} { r } { \operatorname* { l i m } _ { x \to 1 ; x \in ( 0 , \infty ) } \frac { x ^ { q } - 1 } { x - 1 } = q } \end{array}$ for every rational number q. (Hint: use part (a) and Definition 10.1.1. An alternate route is to apply L’Hˆopital’s rule from the next section.) 

Exercise 10.4.3. Let α be a real number, and let $f : ( 0 , \infty ) \to \mathbf { R }$ be the function $f ( x ) = x ^ { \alpha }$ 

(a) Show that $\begin{array} { r } { \operatorname* { l i m } _ { x \to 1 ; x \in ( 0 , \infty ) \backslash \{ 1 \} } \frac { f ( x ) - f ( 1 ) } { x - 1 } = \alpha . } \end{array}$ . (Hint: use Exercise 10.4.2 and the comparison principle; you may need to consider right and left limits separately. Proposition 5.4.14 may also be helpful.) 

(b) Show that f is diferentiable on $( 0 , \infty )$ and that $f ^ { \prime } ( x ) = \alpha x ^ { \alpha - 1 }$ . (Hint: use (a), exponent laws (Proposition 6.7.3), and Definition 10.1.1.) 

## 10.5 L’Hˆopital’s rule

Finally, we present a version of a rule you are all familiar with. 

Proposition 10.5.1 (L’Hˆopital’s rule I). Let X be a subset of R, let $f : X \to \mathbf { R }$ and $g : X  \mathbf { R }$ be functions, and let $x _ { 0 } \in X$ be a limit point of X. Suppose that $f ( x _ { 0 } ) = g ( x _ { 0 } ) = 0 \quad$ , that f and g are both diferentiable at $x _ { 0 }$ , but $g ^ { \prime } ( x _ { 0 } ) \neq 0$ . Then there exists a $\delta > 0$ such that $g ( x ) \neq 0$ for all $x \in ( X \cap ( x _ { 0 } - \delta , x _ { 0 } + \delta ) ) - \{ x _ { 0 } \}$ , and 

$$
\lim _ {x \to x _ {0}; x \in (X \cap (x _ {0} - \delta , x _ {0} + \delta)) - \{x _ {0} \}} \frac {f (x)}{g (x)} = \frac {f ^ {\prime} (x _ {0})}{g ^ {\prime} (x _ {0})}.
$$

Proof. See Exercise 10.5.1. 

The presence of the δ here may seem somewhat strange, but is needed because $g ( x )$ might vanish at some points other than $x _ { 0 }$ , which would imply that quotient $\textstyle { \frac { f ( x ) } { g ( x ) } }$ is not necessarily defined at all points in $X -$ $\{ x _ { 0 } \}$ 

A more sophisticated version of L’Hˆopital’s rule is the following. 

Proposition 10.5.2 (L’Hˆopital’s rule II). Let $a < b$ be real numbers, let $f : [ a , b ]  \mathbf { R }$ and $g : [ a , b ]  \mathbf { R }$ be functions which are diferentiable on $[ a , b ]$ . Suppose that $f ( a ) = g ( a ) = 0$ , that $g ^ { \prime }$ is non-zero on $\left[ a , b \right] \left( i . e . \right.$ $g ^ { \prime } ( x ) \neq 0$ for all $x \in [ a , b ] )$ , and $\begin{array} { r } { \operatorname* { l i m } _ { x \to a ; x \in ( a , b ] } \frac { f ^ { \prime } ( x ) } { g ^ { \prime } ( x ) } } \end{array}$ exists and equals $L$ Then $g ( x ) \neq 0$ for all $x \in ( a , b ]$ , and $\begin{array} { r } { \operatorname* { l i m } _ { x \to a ; x \in ( a , b ] } \frac { f ( x ) } { g ( x ) } } \end{array}$ exists and equals $L .$ 

Remark 10.5.3. This proposition only considers limits to the right of $^ { a , }$ but one can easily state and prove a similar proposition for limits to the left of $^ { a , }$ or around both sides of $a .$ . Speaking very informally, the proposition states that 

$$
\lim _ {x \to a} \frac {f (x)}{g (x)} = \lim _ {x \to a} \frac {f ^ {\prime} (x)}{g ^ {\prime} (x)},
$$

though one has to ensure all of the conditions of the proposition hold (in particular, that $f ( a ) = g ( a ) = 0$ , and that the right-hand limit exists), before one can apply L’Hˆopital’s rule. 

Proof. (Optional) We first show that $g ( x ) \neq 0$ for all $x \in ( a , b ]$ . Suppose for sake of contradiction that $g ( x ) = 0$ for some $x \in ( a , b ]$ . But since $g ( a )$ is also zero, we can apply Rolle’s theorem to obtain $g ^ { \prime } ( y ) = 0$ for some $a < y < x$ , but this contradicts the hypothesis that $g ^ { \prime }$ is non-zero on $[ a , b ]$ 

Now we show that $\begin{array} { r } { \operatorname* { l i m } _ { x \to a ; x \in ( a , b ] } { \frac { f ( x ) } { g ( x ) } } = L } \end{array}$ . By Proposition 9.3.9, it will sufice to show that 

$$
\lim _ {n \to \infty} \frac {f (x _ {n})}{g (x _ {n})} = L
$$

for any sequence $( x _ { n } ) _ { n = 1 } ^ { \infty }$ taking values in $( a , b ]$ which converges to x. 

Consider a single $x _ { n }$ , and consider the function $h _ { n } : [ a , x _ { n } ] \to \mathbf { R }$ defined by 

$$
h _ {n} (x) := f (x) g \left(x _ {n}\right) - g (x) f \left(x _ {n}\right).
$$

Observe that $h _ { n }$ is continuous on $[ a , x _ { n } ]$ and equals 0 at both a and $x _ { n }$ , and is diferentiable on $( a , x _ { n } )$ with derivative $h _ { n } ^ { \prime } ( x ) = f ^ { \prime } ( x ) g ( x _ { n } ) -$ $g ^ { \prime } ( x ) f ( x _ { n } )$ . (Note that $f ( x _ { n } )$ and $g ( x _ { n } )$ are constants with respect to x.) By Rolle’s theorem (Theorem 10.2.7), we can thus find $y _ { n } \in \left( a , x _ { n } \right)$ such that $h _ { n } ^ { \prime } ( y _ { n } ) = 0$ , which implies that 

$$
\frac {f (x _ {n})}{g (x _ {n})} = \frac {f ^ {\prime} (y _ {n})}{g ^ {\prime} (y _ {n})}.
$$

Since $y _ { n } \in ( a , x _ { n } )$ for all n, and $x _ { n }$ converges to a as $n  \infty$ , we see from the squeeze test (Corollary 6.4.14) that $y _ { n }$ also converges to a as $n \to \infty$ . Thus $\frac { f ^ { \prime } ( y _ { n } ) } { g ^ { \prime } ( y _ { n } ) }$ converges to L, and thus $\textstyle { \frac { f ( x _ { n } ) } { g ( x _ { n } ) } }$ also converges to $L _ { ; }$ as desired. □ 

## — Exercises —

Exercise 10.5.1. Prove Proposition 10.5.1. (Hint: to show that $g ( x ) \neq 0$ near $x _ { 0 }$ , you may wish to use Newton’s approximation (Proposition 10.1.7). For the rest of the proposition, use limit laws, Proposition 9.3.14.) 

Exercise 10.5.2. Explain why Exercise 1.2.12 does not contradict either of the propositions in this section. 

## Chapter 11

## The Riemann integral

In the previous chapter we reviewed diferentiation - one of the two pillars of single variable calculus. The other pillar is, of course, integration, which is the focus of the current chapter. More precisely, we will turn to the definite integral, the integral of a function on a fixed interval, as opposed to the indefinite integral, otherwise known as the antiderivative. These two are of course linked by the Fundamental theorem of calculus, of which more will be said later. 

For us, the study of the definite integral will start with an interval I which could be open, closed, or half-open, and a function $f : I  \mathbf { R }$ , and will lead us to a number $\textstyle \int _ { I } f ;$ we can write this integral as $\textstyle \int _ { I } f ( x )$ dx (of course, we could replace x by any other dummy variable), or if I has endpoints a and b, we shall also write this integral as $\textstyle \int _ { a } ^ { b } f$ or $\textstyle \int _ { a } ^ { b } f ( x ) d x$ 

To actually define this integral $\textstyle \int _ { I } f$ is somewhat delicate (especially if one does not want to assume any axioms concerning geometric notions such as area), and not all functions f are integrable. It turns out that there are at least two ways to define this integral: the Riemann integral, named after Georg Riemann (1826–1866), which we will do here and which sufices for most applications, and the Lebesgue integral, named after Henri Lebesgue (1875–1941), which supercedes the Riemann integral and works for a much larger class of functions. The Lebesgue integral will be constructed in Chapter 11.45. There is also the Riemann-Steiltjes integral $\textstyle \int _ { I } f ( x ) \ d \alpha ( x )$ , a generalization of the Riemann integral due to Thomas Stieltjes (1856–1894), which we will discuss in Section 11.8. 

Our strategy in defining the Riemann integral is as follows. We begin by first defining a notion of integration on a very simple class of functions - the piecewise constant functions. These functions are quite primitive, but their advantage is that integration is very easy for these functions, as is verifying all the usual properties. Then, we handle more general functions by approximating them by piecewise constant functions. 

## 11.1 Partitions

Before we can introduce the concept of an integral, we need to describe how one can partition a large interval into smaller intervals. In this chapter, all intervals will be bounded intervals (as opposed to the more general intervals defined in Definition 9.1.1). 

Definition 11.1.1. Let X be a subset of R. We say that X is connected if the following property is true: whenever x, y are elements in X such that $x \ < \ y .$ , the bounded interval [x, y] is a subset of X (i.e., every number between x and y is also in X). 

Remark 11.1.2. Later on, in Section 11.11 we will define a more general notion of connectedness, which applies to any metric space. 

Examples 11.1.3. The set [1, 2] is connected, because if $x < y$ both lie in [1, 2], then $1 \leq x < y \leq 2$ , and so every element between x and y also lies in [1, 2]. A similar argument shows that the set (1, 2) is connected. However, the set $[ 1 , 2 ] \cup [ 3 , 4 ]$ is not connected (why?). The real line is connected (why?). The empty set, as well as singleton sets such as 3 , are connected, but for rather trivial reasons (these sets do not contain two elements x, y for which $x < y )$ 

Lemma 11.1.4. Let X be a subset of the real line. Then the following two statements are logically equivalent: 

(a) X is bounded and connected. 

(b) X is a bounded interval. 

Proof. See Exercise 11.1.1. 

Remark 11.1.5. Recall that intervals are allowed to be singleton points (e.g., the degenerate interval $[ 2 , 2 ] = \{ 2 \} )$ , or even the empty set. 

Corollary 11.1.6. If I and J are bounded intervals, then the intersection $I \cap J$ is also a bounded interval. 

Proof. See Exercise 11.1.2. 

Example 11.1.7. The intersection of the bounded intervals $[ 2 , 4 ]$ and [4, 6] is 4 , which is also a bounded interval. The intersection of (2, 4) and (4, 6) is . 

We now give each bounded interval a length. 

Definition 11.1.8 (Length of intervals). If I is a bounded interval, we define the length of I, denoted I as follows. If I is one of the intervals $[ a , b ] , ( a , b ) , [ a , b )$ , or $( a , b ]$ for some real numbers $a < b ,$ then we define $| I | : = b - a$ . Otherwise, if I is a point or the empty set, we define $| I | = 0$ 

Example 11.1.9. For instance, the length of [3, 5] is 2, as is the length of (3, 5); meanwhile, the length of 5 or the empty set is 0. 

Definition 11.1.10 (Partitions). Let I be a bounded interval. A partition of I is a finite set P of bounded intervals contained in I, such that every x in I lies in exactly one of the bounded intervals J in P. 

Remark 11.1.11. Note that a partition is a set of intervals, while each interval is itself a set of real numbers. Thus a partition is a set consisting of other sets. 

Examples 11.1.12. The set $\textbf { P } = \{ \{ 1 \} , ( 1 , 3 ) , [ 3 , 5 ) , \{ 5 \} , ( 5 , 8 ] , \emptyset \}$ of bounded intervals is a partition of [1, 8], because all the intervals in P lie in [1, 8], and each element of [1, 8] lies in exactly one interval in P. Note that one could have removed the empty set from P and still obtain a partition. However, the set $\{ [ 1 , 4 ] , [ 3 , 5 ] \}$ is not a partition of [1, 5] because some elements of [1, 5] are included in more than one interval in the set. The set $\{ ( 1 , 3 ) , ( 3 , 5 ) \}$ is not a partition of (1, 5) because some elements of (1, 5) are not included in any interval in the set. The set $\{ ( 0 , 3 ) , [ 3 , 5 ) \}$ is not a partition of (1, 5) because some intervals in the set are not contained in (1, 5). 

Now we come to a basic property about length: 

Theorem 11.1.13 (Length is finitely additive). Let I be a bounded interval, n be a natural number, and let P be a partition of I of cardinality n. Then 

$$
| I | = \sum_ {J \in \mathbf {P}} | J |.
$$

Proof. We prove this by induction on n. More precisely, we let $P ( n )$ be the property that whenever I is a bounded interval, and whenever P is a partition of I with cardinality n, that $\begin{array} { r } { | I | = \sum _ { J \in \mathbf { P } } | J | } \end{array}$ 

The base case $P ( 0 )$ is trivial; the only way that I can be partitioned into an empty partition is if I is itself empty $\mathrm { \left( w h y ? \right) }$ , at which point the claim is easy. The case $P ( 1 )$ is also very easy; the only way that I can be partitioned into a singleton set $\{ J \}$ is if $J = I \ \mathrm { ( w h y ? ) }$ , at which point the claim is again very easy. 

Now suppose inductively that $P ( n )$ is true for some $n \geq 1$ , and now we prove $P ( n + 1 )$ . Let I be a bounded interval, and let P be a partition of I of cardinality $n + 1$ 

If I is the empty set or a point, then all the intervals in P must also be either the empty set or a point $\mathrm { ( w h y ? ) }$ , and so every interval has length zero and the claim is trivial. Thus we will assume that I is an interval of the form $( a , b ) , ( a , b ] , [ a , b )$ , or $[ a , b ]$ 

Let us first suppose that $b \in I , \mathrm { i . e . , } I$ is either $( a , b ] { \mathrm { ~ o r ~ } } [ a , b ]$ . Since $b \in I$ , we know that one of the intervals K in P contains b. Since K is contained in $I ,$ it must therefore be of the form $( c , b ] , [ c , b ]$ , or b for some real number $c ,$ with $a \leq c \leq b$ (in the latter case of $K = \{ b \}$ we set $c : = b )$ . In particular, this means that the set $I - K$ is also an interval of the form $[ a , c ] , ( a , c ) , ( a , c ] , [ a , c )$ when $c > a ,$ , or a point or empty set when $a = c$ . Either way, we easily see that 

$$
| I | = | K | + | I - K |.
$$

$\mathrm { O n }$ the other hand, since P forms a partition of $I ,$ we see that $\mathbf { P } - \{ K \}$ forms a partition of $I - K \ \mathrm { ( w h y ? ) }$ . By the induction hypothesis, we thus have 

$$
| I - K | = \sum_ {J \in \mathbf {P} - \{K \}} | J |.
$$

Combining these two identities (and using the laws of addition for finite sets, see Proposition 7.1.11) we obtain 

$$
| I | = \sum_ {J \in \mathbf {P}} | J |
$$

as desired. 

Now suppose that $b \not \in I , \mathrm { i . e . }$ , I is either $( a , b )$ or $[ a , b )$ . Then one of the intervals K also is of the form $( c , b )$ or $[ c , b )$ (see Exercise 11.1.3). In particular, this means that the set $I - K$ is also an interval of the form $[ a , c ] , ( a , c ) , ( a , c ] , [ a , c )$ when $c > a$ , or a point or empty set when $a = c .$ The rest of the argument then proceeds as above. □ 

There are two more things we need to do with partitions. One is to say when one partition is finer than another, and the other is to talk about the common refinement of two partitions. 

Definition 11.1.14 (Finer and coarser partitions). Let I be a bounded interval, and let P and $\mathbf { P ^ { \prime } }$ be two partitions of I. We say that $\mathbf { P } ^ { \prime }$ is finer than P (or equivalently, that P is coarser than P) if for every J in $\mathbf { P } ^ { \prime }$ there exists a K in P such that $J \subseteq K$ 

Example 11.1.15. The partition $\{ [ 1 , 2 ) , \{ 2 \} , ( 2 , 3 ) , [ 3 , 4 ] \}$ is finer than [1, 2], (2, 4] (why?). Both partitions are finer than [1, 4] , which is the coarsest possible partition of [1, 4]. Note that there is no such thing as a “finest” partition of [1, 4]. (Why? recall all partitions are assumed to be finite.) We do not compare partitions of diferent intervals, for instance if P is a partition of [1, 4] and $\mathbf { P ^ { \prime } }$ is a partition of [2, 5] then we would not say that P is coarser or finer than $\mathbf { P ^ { \prime } }$ 

Definition 11.1.16 (Common refinement). Let I be a bounded interval, and let P and $\mathbf { P ^ { \prime } }$ be two partitions of I. We define the common refinement $\mathbf { P \# P ^ { \prime } }$ of P and $\mathbf { P } ^ { \prime }$ to be the set 

$$
\mathbf {P} \# \mathbf {P} ^ {\prime} := \{K \cap J: K \in \mathbf {P} \text {   and   } J \in \mathbf {P} ^ {\prime} \}.
$$

Example 11.1.17. Let ${ \bf P } : = \{ [ 1 , 3 ) , ~ [ 3 , 4 ] \}$ and ${ \bf P } ^ { \prime } : = \{ [ 1 , 2 ] , ~ ( 2 , 4 ] \}$ be two partitions of [1, 4]. Then $\mathbf { P \# P ^ { \prime } }$ is the set $\{ [ 1 , 2 ] , ( 2 , 3 ) , [ 3 , 4 ] , \emptyset \}$ (why?). 

Lemma 11.1.18. Let I be a bounded interval, and let P and $\mathbf { P ^ { \prime } }$ be two partitions of I. Then $\mathbf { P \# P ^ { \prime } }$ is also a partition of I, and is both finer than P and finer than $\mathbf { P ^ { \prime } }$ 

Proof. See Exercise 11.1.4. 

## — Exercises —

Exercise 11.1.1. Prove Lemma 11.1.4. (Hint: in order to show that (a) implies (b) in the case when X is non-empty, consider the supremum and infimum of X.) 

Exercise 11.1.2. Prove Corollary 11.1.6. (Hint: use Lemma 11.1.4, and explain why the intersection of two bounded sets is automatically bounded, and why the intersection of two connected sets is automatically connected.) 

Exercise 11.1.3. Let I be a bounded interval of the form $\boldsymbol { I } = \left( a , b \right)$ or $I = [ a , b )$ for some real numbers $a < b$ . Let $I _ { 1 } , \ldots , I _ { n }$ be a partition of I. Prove that one of the intervals $I _ { j }$ in this partition is of the form $I _ { j } = \left( c , b \right)$ or $I _ { j } = [ c , b )$ for some $a \leq c \leq b$ . (Hint: prove by contradiction. First show that if $I _ { j }$ is not of the form (c, b) or [c, b) for any $a \leq c \leq b$ , then sup $I _ { j }$ is strictly less than b.) Exercise 11.1.4. Prove Lemma 11.1.18. 

## 11.2 Piecewise constant functions

We can now describe the class of “simple” functions which we can integrate very easily. 

Definition 11.2.1 (Constant functions). Let X be a subset of R, and let $f : X \to \mathbf { R }$ be a function. We say that f is constant if there exists a real number c such that $f ( x ) = c$ for all $x \in X$ . If E is a subset of X, we say that f is constant on E if the restriction $f | _ { E }$ of f to E is constant, in other words there exists a real number c such that $f ( x ) = c$ for all $x \in E$ . We refer to c as the constant value of f on E. 

Remark 11.2.2. If E is a non-empty set, then a function f which is constant on $E$ can have only one constant value; it is not possible for a function to always equal 3 on E while simultaneously always equalling 4. However, if E is empty, every real number c is a constant value for f on $E \ \mathrm { ( w h y ? ) }$ 

Definition 11.2.3 (Piecewise constant functions I). Let I be a bounded interval, let $f : I  \mathbf { R }$ be a function, and let P be a partition of I. We say that f is piecewise constant with respect to P if for every $J \in \mathbf { P }$ , f is constant on J. 

Example 11.2.4. The function $f : [ 1 , 6 ] \to \mathbf { R }$ defined by 

$$
f (x) = \left\{ \begin{array}{l l} 7 & \text { if } 1 \leq x <   3 \\ 4 & \text { if } x = 3 \\ 5 & \text { if } 3 <   x <   6 \\ 2 & \text { if } x = 6 \end{array} \right.
$$

is piecewise constant with respect to the partition $\{ [ 1 , 3 ) , \ \{ 3 \} , \ ( 3 , 6 )$ $\{ 6 \} \}$ of [1, 6]. Note that it is also piecewise constant with respect to some other partitions as well; for instance, it is piecewise constant with respect to the partition $\{ [ 1 , 2 ) , \{ 2 \} , ( 2 , 3 ) , \{ 3 \} , ( 3 , 5 ) , [ 5 , 6 ) , \{ 6 \} , \emptyset \}$ 

Definition 11.2.5 (Piecewise constant functions II). Let I be a bounded interval, and let $f : I  \mathbf { R }$ be a function. We say that f is piecewise constant on I if there exists a partition P of I such that f is piecewise constant with respect to $\mathbf { P }$ 

Example 11.2.6. The function used in the previous example is piecewise constant on [1, 6]. Also, every constant function on a bounded interval I is automatically piecewise constant (why?). 

Lemma 11.2.7. Let I be a bounded interval, let P be a partition of I, and let $f : I  \mathbf { R }$ be a function which is piecewise constant with respect to P. Let $\mathbf { P ^ { \prime } }$ be a partition of I which is finer than P. Then f is also piecewise constant with respect to $\mathbf { P ^ { \prime } }$ 

Proof. See Exercise 11.2.1. 

The space of piecewise constant functions is closed under algebraic operations: 

Lemma 11.2.8. Let I be a bounded interval, and let $f : I  \mathbf { R }$ and $g : I  \mathbf { R }$ be piecewise constant functions on I. Then the functions $f + g , f - g$ $\operatorname* { m a x } ( f , g )$ and fg are also piecewise constant functions on I. Here of course max $( f , g ) : I \to \mathbf { R }$ is the function max $( f , g ) ( x ) : =$ max $( f ( x ) , g ( x ) )$ . If g does not vanish anywhere on I $( i . e . , g ( x ) \neq 0$ for all $x \in I )$ then $f / g$ is also a piecewise constant function on I. 

Proof. See Exercise 11.2.2. 

We are now ready to integrate piecewise constant functions. We begin with a temporary definition of an integral with respect to a partition. 

Definition 11.2.9 (Piecewise constant integral I). Let I be a bounded interval, let P be a partition of I. Let $f : I  \mathbf { R }$ be a function which is piecewise constant with respect to P. Then we define the piecewise constant integral $p . c . \int _ { [ \mathbf { P } ] } f$ of f with respect to the partition P by the formula 

$$
p. c. \int_ {[ \mathbf {P} ]} f := \sum_ {J \in \mathbf {P}} c _ {J} | J |,
$$

where for each J in P, we let $c _ { J }$ be the constant value of f on J. 

Remark 11.2.10. This definition seems like it could be ill-defined, because if J is empty then every number $c _ { J }$ can be the constant value of f on J, but fortunately in such cases $| J |$ is zero and so the choice of $c J$ is irrelevant. The notation $p . c . \int _ { [ \mathbf { P } ] } f$ is rather artificial, but we shal only need it temporaril $\cdot \mathrm { y } ,$ en route to a more useful definition. Note that since P is finite, the sum $\sum { _ { J \in \mathbf { P } } c _ { J } | J | }$ is always well-defined (it is never divergent or infinite). 

Remark 11.2.11. The piecewise constant integral corresponds intuitively to one’s notion of area, given that the area of a rectangle ought to be the product of the lengths of the sides. (Of course, if f is negative somewhere, then the “area” $c _ { J } | J |$ would also be negative.) 

Example 11.2.12. Let $f : [ 1 , 4 ] \to \mathbf { R }$ be the function 

$$
f (x) = \left\{ \begin{array}{l l} 2 & \text { if } 1 \leq x <   3 \\ 4 & \text { if } x = 3 \\ 6 & \text { if } 3 <   x \leq 4 \end{array} \right.
$$

and let $\mathbf { P } : = \{ [ 1 , 3 ) , \{ 3 \} , ( 3 , 4 ] \}$ . Then 

$$
\begin{array}{r l} & p. c. \int_ {[ \mathbf {P} ]} f = c _ {[ 1, 3)} | [ 1, 3) | + c _ {\{3 \}} | \{3 \} | + c _ {(3, 4 ]} | (3, 4) | \\ & \qquad = 2 \times 2 + 4 \times 0 + 6 \times 1 \\ & \qquad = 1 0. \end{array}
$$

Alternatively, if we let $\mathbf { P } ^ { \prime } : = \{ [ 1 , 2 ) , [ 2 , 3 ) , \{ 3 \} , ( 3 , 4 ] , \emptyset \}$ then 

$$
\begin{array}{r l} & p. c. \int_ {[ \mathbf {P} ^ {\prime} ]} f = c _ {[ 1, 2)} | [ 1, 2) | + c _ {[ 2, 3)} | [ 2, 3) | + c _ {\{3 \}} | \{3 \} | \\ & \qquad + c _ {(3, 4 ]} | (3, 4 ] | + c _ {\emptyset} | \emptyset | \\ & \qquad = 2 \times 1 + 2 \times 1 + 4 \times 0 + 6 \times 1 + c _ {\emptyset} \times 0 \\ & \qquad = 1 0. \end{array}
$$

This example suggests that this integral does not really depend on what partition you pick, so long as your function is piecewise constant with respect to that partition. That is indeed true: 

Proposition 11.2.13 (Piecewise constant integral is independent of partition). Let I be a bounded interval, and let $f : I  \mathbf { R }$ be a function. Suppose that P and $\mathbf { P } ^ { \prime }$ are partitions of I such that f is piecewise constant both with respect to P and with respect to $\mathbf { P } ^ { \prime }$ . Then $\textstyle p . c . \int _ { [ \mathbf { P } ] } f = p . c . \int _ { [ \mathbf { P ^ { \prime } } ] } f$ 

Proof. See Exercise 11.2.3. 

Because of this proposition, we can now make the following definition: 

Definition 11.2.14 (Piecewise constant integral II). Let I be a bounded interval, and let $f : I  \mathbf { R }$ be a piecewise constant function on I. We define the piecewise constant integral $p . c . \int _ { I } f$ by the formula 

$$
p. c. \int_ {I} f := p. c. \int_ {[ \mathbf {P} ]} f,
$$

where P is any partition of I with respect to which f is piecewise constant. (Note that Proposition 11.2.13 tells us that the precise choice of this partition is irrelevant.) 

Example 11.2.15. If f is the function given in Example 11.2.12, then $\begin{array} { r } { p . c . \int _ { [ 1 , 4 ] } f = 1 0 } \end{array}$ 

We now give some basic properties of the piecewise constant integral. These laws will eventually be superceded by the corresponding laws for the Riemann integral (Theorem 11.4.1). 

Theorem 11.2.16 (Laws of integration). Let I be a bounded interval, and let $f : I  \mathbf { R }$ and $g : I  \mathbf { R }$ be piecewise constant functions on I. 

(a) We have p.c. $\begin{array} { r } { \int _ { I } ( f + g ) = p . c . \int _ { I } f + p . c . \int _ { I } g . } \end{array}$ 

(b) For any real number c, we have p.c. $\textstyle { \int _ { I } ( c f ) = c ( p . c . \int _ { I } f ) }$ 

(c) We have p.c. $\begin{array} { r } { \int _ { I } ( f - g ) = p . c . \int _ { I } f - p . c . \int _ { I } g . } \end{array}$ 

(d) If $f ( x ) \geq 0$ for all $x \in I$ , then p.c. $\textstyle \int _ { I } f \geq 0$ 

(e) $I f f ( x ) \geq g ( x )$ for all $x \in I$ , then p.c. $\textstyle \int _ { I } f \geq p . c . \int _ { I } g .$ 

(f ) $I f f$ is the constant function $f ( x ) = c$ for all x in I, then $\textstyle p . c . \int _ { I } f =$ $c | I |$ 

(g) Let J be a bounded interval containing $I \ ( i . e . , \ I \ \subseteq \ J )$ , and let $F : J  \mathbf { R }$ be the function 

$$
F (x) := \left\{ \begin{array}{l l} f (x) & \text { if } x \in I \\ 0 & \text { if } x \not \in I \end{array} \right.
$$

Then F is piecewise constant on J, and $\textstyle p . c . \int _ { J } F = p . c . \int _ { I } f .$ 

(h) Suppose that $\{ J , K \}$ is a partition of I into two intervals J and K. Then the functions $f | _ { J } : J \to \mathbf { R }$ and $f | _ { K } : K  \mathbf { R }$ are piecewise constant on J and K respectively, and we have 

$$
p. c. \int_ {I} f = p. c. \int_ {J} f | _ {J} + p. c. \int_ {K} f | _ {K}.
$$

Proof. See Exercise 11.2.4. 

This concludes our integration of piecewise constant functions. We now turn to the question of how to integrate bounded functions. 

— Exercises — 

Exercise 11.2.1. Prove Lemma 11.2.7. 

Exercise 11.2.2. Prove Lemma 11.2.8. (Hint: use Lemmas 11.1.18 and 11.2.7 to make f and g piecewise constant with respect to the same partition of I.) 

Exercise 11.2.3. Prove Proposition 11.2.13. (Hint: first use Theorem 11.1.13 to show that both integrals are equal to $p . c . \int _ { [ \mathbf { P } \# \mathbf { P ^ { \prime } } ] } f . )$ 

Exercise 11.2.4. Prove Theorem 11.2.16. (Hint: you can use earlier parts of the theorem to prove some of the later parts of the theorem. See also the hint to Exercise 11.2.2.) 

## 11.3 Upper and lower Riemann integrals

Now let $f : I  \mathbf { R }$ be a bounded function defined on a bounded interval I. We want to define the Riemann integral $\textstyle \int _ { I } f .$ . To do this we first need to define the notion of upper and lower Riemann integrals $\overline { { \int } } _ { I } f$ and $\underline { { \boldsymbol { \int } } } _ { I } \boldsymbol { f } .$ These notions are related to the Riemann integral in much the same way that the lim sup and lim inf of a sequence are related to the limit of that sequence. 

Definition 11.3.1 (Majorization of functions). Let $f : I  \mathbf { R }$ and $g : I  \mathbf { R }$ . We say that g majorizes f on I if we have $g ( x ) \geq f ( x )$ for all $x \in I$ , and that g minorizes f on I if $g ( x ) \leq f ( x )$ for all $x \in I$ 

The idea of the Riemann integral is to try to integrate a function by first majorizing or minorizing that function by a piecewise constant function (which we already know how to integrate). 

Definition 11.3.2 (Upper and lower Riemann integrals). Let $f : I  \mathbf { R }$ be a bounded function defined on a bounded interval I. We define the upper Riemann integral $\overline { { \int } } _ { I } f$ by the formula 

${ \overline { { \int } } } _ { I } f : = \operatorname* { i n f } \{ p . c . \int _ { I } g : g$ is a p.c. function on I which majorizes f 

and the lower Riemann integral $\underline { { \boldsymbol { \int } } } _ { I } \boldsymbol { f }$ by the formula 

$\underline { { { \int } } } _ { I } f : = \operatorname* { s u p } \{ p . c . \int _ { I } g : g$ is a p.c. function on I which minorizes $f \}$ 

We give a crude but useful bound on the lower and upper integral: 

Lemma 11.3.3. Let $f : I  \mathbf { R }$ be a function on a bounded interval I which is bounded by some real number M, $i . e . , - M \leq f ( x ) \leq M$ for all $x \in I$ . Then we have 

$$
- M | I | \leq \underline {{\int}} _ {I} f \leq \overline {{\int}} _ {I} f \leq M | I |.
$$

In particular, both the lower and upper Riemann integrals are real numbers $( i . e .$ , they are not infinite). 

Proof. The function $g : I  \mathbf { R }$ defined by $g ( x ) = M$ is constant, hence piecewise constant, and majorizes $f ;$ thus $\begin{array} { r } { \overline { { \int } } _ { I } f \le p . c . \int _ { I } g = M | I | } \end{array}$ by definition of the upper Riemann integral. A similar argument gives $\begin{array} { r } { - M | I | \le \underline { { \int } } _ { I } f } \end{array}$ . Finally, we have to show that $\textstyle \int _ { r } f \leq { \overline { { \int _ { I } } } } f$ . Let $g$ be any piecewise constant function majorizing $f _ { : }$ , and let h be any piecewise constant function minorizing $f .$ . Then g majorizes $h ,$ and hence p.c. $\begin{array} { r } { \int _ { I } h \le p . c . \int _ { I } g } \end{array}$ . Taking suprema in h, we obtain that $\underline { { \boldsymbol { \int } } } _ { I } f \le p . c . \int _ { I } g .$ Taking infima in $g ,$ we thus obtain $\underline { { \boldsymbol { \int } } } _ { I } \boldsymbol { f } \le \overline { { \boldsymbol { \int } } } _ { I } \boldsymbol { g }$ , as desired. □ 

We now know that the upper Riemann integral is always at least as large as the lower Riemann integral. If the two integrals match, then we can define the Riemann integral: 

Definition 11.3.4 (Riemann integral). Let $f : I  \mathbf { R }$ be a bounded function on a bounded interval I. If $\textstyle \int _ { I } f = { \overline { { \int } } } _ { I } f$ , then we say that f is Riemann integrable on I and define 

$$
\int_ {I} f := \underline {{\int}} _ {I} f = \overline {{\int}} _ {I} f.
$$

If the upper and lower Riemann integrals are unequal, we say that f is not Riemann integrable. 

Remark 11.3.5. Compare this definition to the relationship between the lim sup, lim inf, and limit of a sequence $a _ { n }$ that was established in Proposition 6.4.12(f); the lim sup is always greater than or equal to the lim inf, but they are only equal when the sequence converges, and in this case they are both equal to the limit of the sequence. The definition given above may difer from the definition you may have encountered in your calculus courses, based on Riemann sums. However, the two definitions turn out to be equivalent; this is the purpose of the next section. 

Remark 11.3.6. Note that we do not consider unbounded functions to be Riemann integrable; an integral involving such functions is known as an improper integral. It is possible to still evaluate such integrals using more sophisticated integration methods (such as the Lebesgue integral); we shall do this in Chapter 11.45. 

The Riemann integral is consistent with (and supercedes) the piecewise constant integral: 

Lemma 11.3.7. Let f : I R be a piecewise constant function on a bounded interval I. Then f is Riemann integrable, and $\textstyle \int _ { I } f = p . c . \int _ { I } f$ 

Proof. See Exercise 11.3.3. 

Remark 11.3.8. Because of this lemma, we will not refer to the piecewise constant integral p.c. $\scriptstyle \int _ { I }$ again, and just use the Riemann integral $\scriptstyle \int _ { I }$ throughout (until this integral is itself superceded by the Lebesgue integral in Chapter 11.45). We observe one special case of Lemma 11.3.7: if I is a point or the empty set, then $\textstyle \int _ { I } f = 0$ for all functions $f : I  \mathbf { R }$ (Note that all such functions are automatically constant.) 

We have just shown that every piecewise constant function is Riemann integrable. However, the Riemann integral is more general, and can integrate a wider class of functions; we shall see this shortly. For now, we connect the Riemann integral we have just defined to the concept of a Riemann sum, which you may have seen in other treatments of the Riemann integral. 

Definition 11.3.9 (Riemann sums). Let $f : I  \mathbf { R }$ be a bounded function on a bounded interval I, and let P be a partition of I. We define the upper Riemann sum $U ( f , \mathbf { P } )$ and the lower Riemann sum $L ( f , \mathbf { P } )$ by 

$$
U (f, \mathbf {P}) := \sum_ {J \in \mathbf {P}: J \neq \emptyset} (\sup _ {x \in J} f (x)) | J |
$$

and 

$$
L (f, \mathbf {P}) := \sum_ {J \in \mathbf {P}: J \neq \emptyset} (\inf _ {x \in J} f (x)) | J |.
$$

Remark 11.3.10. The restriction $J \neq \emptyset$ is required because the quantities in $\operatorname { f } _ { x \in J } f ( x )$ and $\operatorname { s u p } _ { x \in J } f ( x )$ are infinite (or negative infinite) if J is empty. 

We now connect these Riemann sums to the upper and lower Riemann integral. 

Lemma 11.3.11. Let $f : I  \mathbf { R }$ be a bounded function on a bounded interval I, and let g be a function which majorizes f and which is piecewise constant with respect to some partition P of I. Then 

$$
p. c. \int_ {I} g \geq U (f, \mathbf {P}).
$$

Similarly, if h is a function which minorizes f and is piecewise constant with respect to P, then 

$$
p. c. \int_ {I} h \leq L (f, \mathbf {P}).
$$

Proof. See Exercise 11.3.4. 

Proposition 11.3.12. Let $f : I  \mathbf { R }$ be a bounded function on a bounded interval I. Then 

$$
\overline {{\int}} _ {I} f = \inf \{U (f, \mathbf {P}): \mathbf {P} i s a p a r t i t i o n o f I \}
$$

and 

$$
\int_ {\underline {{I}}} f = \sup \{L (f, \mathbf {P}): \mathbf {P} \text {   is   a   partition   of   } I \}
$$

Proof. See Exercise 11.3.5. 

— Exercises — 

Exercise 11.3.1. Let $f : I  \mathbf { R } , g : I  \mathbf { R }$ , and $h : I  \mathbf { R }$ be functions. Show that if f majorizes g and g majorizes h, then f majorizes h. Show that if f and g majorize each other, then they must be equal. 

Exercise 11.3.2. Let $f : I  \mathbf { R } , g : I  \mathbf { R } ,$ and $h : I  \mathbf { R }$ be functions. If f majorizes g, is it true that $f + h$ majorizes $g + h ?$ Is it true that $f \cdot h$ majorizes $g \cdot h ?$ If c is a real number, is it true that cf majorizes $c g \smash { ? }$ 

Exercise 11.3.3. Prove Lemma 11.3.7. 

Exercise 11.3.4. Prove Lemma 11.3.11. 

Exercise 11.3.5. Prove Proposition 11.3.12. (Hint: you will need Lemma 11.3.11, even though this Lemma will only do half of the job.) 

## 11.4 Basic properties of the Riemann integral

Just as we did with limits, series, and derivatives, we now give the basic laws for manipulating the Riemann integral. These laws will eventually be superceded by the corresponding laws for the Lebesgue integral (Proposition 11.48.3). 

Theorem 11.4.1 (Laws of Riemann integration). Let I be a bounded interval, and let $f : I  \mathbf { R }$ and $g : I  \mathbf { R }$ be Riemann integrable functions on I. 

(a) The function $f + g$ is Riemann integrable, and we have $\textstyle \int _ { I } ( f + g ) =$ $\textstyle { \int _ { I } f + \int _ { I } g . }$ 

(b) For any real number c, the function cf is Riemann integrable, and we have $\textstyle { \int _ { I } ( c f ) = c ( \int _ { I } f ) }$ 

(c) The function $f - g$ is Riemann integrable, and we have $\textstyle \int _ { I } ( f - g ) =$ $\textstyle \int _ { I } f - \int _ { I } g$ 

(d) If $f ( x ) \geq 0$ for all $x \in I$ , then $\textstyle \int _ { I } f \geq 0$ 

(e) $I f f ( x ) \geq g ( x )$ for all $x \in I$ , then $\textstyle { \int _ { I } f \geq \int _ { I } g }$ 

(f ) $_ { I f f }$ is the constant function $f ( x ) = c$ for all x in I, then $\textstyle \int _ { I } f =$ $c | I |$ 

(g) Let J be a bounded interval containing $I \ ( i . e . , \ I \ \subseteq \ J )$ , and let $F : J  \mathbf { R }$ be the function 

$$
F (x) := \left\{ \begin{array}{l l} f (x) & \text { if } x \in I \\ 0 & \text { if } x \not \in I \end{array} \right.
$$

Then F is Riemann integrable on J, and $\textstyle \int _ { J } F = \int _ { I } f$ 

(h) Suppose that $\{ J , K \}$ is a partition of I into two intervals J and K. Then the functions $f | _ { J } : J \to \mathbf { R }$ and $f | _ { K } : K  \mathbf { R }$ are Riemann integrable on J and K respectively, and we have 

$$
\int_ {I} f = \int_ {J} f | _ {J} + \int_ {K} f | _ {K}.
$$

Proof. See Exercise 11.4.1. 

Remark 11.4.2. We often abbreviate $\int _ { J } f { \big \vert } _ { J }$ as $\textstyle \int _ { J } f $ , even though f is really defined on a larger domain than just J. 

Theorem 11.4.1 asserts that the sum or diference of any two Riemann integrable functions is Riemann integrable, as is any scalar multiple $c f$ of a Riemann integrable function $f .$ . We now give some further ways to create Riemann integrable functions. 

Theorem 11.4.3 (Max and min preserve integrability). Let I be a bounded interval, and let $f : I  \mathbf { R }$ and $g \ : \ I \  \ \mathbf { R }$ be a Riemann integrable function. Then the functions max $( f , g ) : I \to \mathbf { R }$ and min $( f , g ) \ : \ I \ \to \ \mathbf { R }$ defined by max $( f , g ) ( x ) : = \operatorname* { m a x } ( f ( x ) , g ( x ) )$ and min $( f , g ) ( x ) : = \operatorname* { m i n } ( f ( x ) , g ( x ) )$ are also Riemann integrable. 

Proof. We shall just prove the claim for $\operatorname* { m a x } ( f , g )$ , the case of min $( f , g )$ being similar. First note that since f and g are bounded, then max $( f , g )$ is also bounded. 

Let $\varepsilon \ > \ 0$ . Since $\textstyle \int _ { I } f \ = \ \underline { { \int } } _ { I } f .$ , there exists a piecewise constant function $\underline { { f } } : I  \mathbf { R }$ which minorizes f on I such that 

$$
\int_ {I} \underline {{f}} \geq \int_ {I} f - \varepsilon .
$$

Similarly we can find a piecewise constant $g : I  \mathbf { R }$ which minorizes g on I such that 

$$
\int_ {I} \underline {{g}} \geq \int_ {I} g - \varepsilon ,
$$

and we can find piecewise functions ${ \overline { { f } } } , { \overline { { g } } }$ which majorize $f , g$ respectively on I such that 

$$
\int_ {I} \overline {{f}} \leq \int_ {I} f + \varepsilon
$$

and 

$$
\int_ {I} \overline {{g}} \leq \int_ {I} g + \varepsilon .
$$

In particular, if $h : I  \mathbf { R }$ denotes the function 

$$
h := (\overline {{f}} - \underline {{f}}) + (\overline {{g}} - \underline {{g}})
$$

we have 

$$
\int_ {I} h \leq 4 \varepsilon .
$$

On the other hand, $\operatorname* { m a x } ( \underline { { f } } , \underline { { g } } )$ is a piecewise constant function on I $\mathrm { \left( w h y ? \right) }$ which minorizes max $\left( f , g \right) { \mathrm { ~ ( w h y ? ) ~ } }$ , while $\operatorname* { m a x } ( \overline { { f } } , \overline { { g } } )$ is similarly a piecewise constant function on I which majorizes $\operatorname* { m a x } ( f , g )$ . Thus 

$$
\int_ {I} \max (\underline {{f}}, \underline {{g}}) \leq \int_ {\underline {{I}}} \max (f, g) \leq \overline {{\int}} _ {I} \max (f, g) \leq \int_ {I} \max (\overline {{f}}, \overline {{g}}),
$$

and so 

$$
0 \leq \overline {{\int}} _ {I} \max (f, g) - \underline {{\int}} _ {I} \max (f, g) \leq \int_ {I} \max (\overline {{f}}, \overline {{g}}) - \max (\underline {{f}}, \underline {{g}}).
$$

But we have 

$$
\overline {{{f}}} (x) = \underline {{{f}}} (x) + (\overline {{{f}}} - \underline {{{f}}}) (x) \leq \underline {{{f}}} (x) + h (x)
$$

and similarly 

$$
\overline {{g}} (x) = \underline {{g}} (x) + (\overline {{g}} - \underline {{g}}) (x) \leq \underline {{g}} (x) + h (x)
$$

and thus 

$$
\max (\overline {{f}} (x), \overline {{g}} (x)) \leq \max (\underline {{f}} (x), \underline {{g}} (x)) + h (x).
$$

Inserting this into the previous inequality, we obtain 

$$
0 \leq \overline {{\int}} _ {I} \max (f, g) - \underline {{\int}} _ {I} \max (f, g) \leq \int_ {I} h \leq 4 \varepsilon .
$$

To summarize, we have shown that 

$$
0 \leq \overline {{\int}} _ {I} \max (f, g) - \underline {{\int}} _ {I} \max (f, g) \leq 4 \varepsilon
$$

for every ε. Since $\begin{array} { r } { \overline { { \int } } _ { I } \operatorname* { m a x } ( f , g ) - \underline { { \int } } _ { I } \operatorname* { m a x } ( f , g ) } \end{array}$ does not depend on $\varepsilon ,$ we thus see that 

$$
\overline {{\int}} _ {I} \max (f, g) - \underline {{\int}} _ {I} \max (f, g) = 0
$$

and hence that $\operatorname* { m a x } ( f , g )$ is Riemann integrable. 

Corollary 11.4.4 (Absolute values preserve Riemann integrability). Let I be a bounded interval. If $f : I  \mathbf { R }$ is a Riemann integrable function, then the positive part $f _ { + } : = \operatorname* { m a x } ( f , 0 )$ and the negative part $f _ { - } : = \operatorname* { m i n } ( f , 0 )$ are also Riemann integrable on I. Also, the absolute value $| f | = f _ { + } - f _ { - }$ is also Riemann integrable on I. 

Theorem 11.4.5 (Products preserve Riemann integrability). Let I be a bounded interval. If $f : I  \mathbf { R }$ and $g : I  \mathbf { R }$ are Riemann integrable, then $f g : I  \mathbf { R }$ is also Riemann integrable. 

Proof. This one is a little trickier. We split $f = f _ { + } + f _ { - }$ and $g = g _ { + } + g _ { - }$ into positive and negative parts; by Corollary 11.4.4, the functions $f _ { + }$ $f _ { - } , g _ { + } , g _ { - }$ are Riemann integrable. Since 

$$
f g = f _ {+} g _ {+} + f _ {+} g _ {-} + f _ {-} g _ {+} + f _ {-} g _ {-}
$$

then it sufices to show that the functions $f _ { + } g _ { + } , f _ { + } g _ { - } , \ f _ { - } g _ { + } , \ f _ { - } g _ { - }$ are individually Riemann integrable. We will just show this for $f _ { + } g _ { + } ;$ the other three are similar. 

Since $f _ { + }$ and $g _ { + }$ are bounded and positive, there are $M _ { 1 } , M _ { 2 } > 0$ such that 

$$
0 \leq f _ {+} (x) \leq M _ {1} \mathrm{and} 0 \leq g _ {+} (x) \leq M _ {2}
$$

for all $x \in I$ . Now let $\varepsilon > 0$ be arbitrary. Then, as in the proof of Theorem 11.4.3, we can find a piecewise constant function $f _ { \pm }$ minorizing $f _ { + }$ on I, and a piecewise constant function $\overline { { f _ { + } } }$ majorizing $f _ { + }$ on $I ,$ such that 

$$
\int_ {I} \overline {{f _ {+}}} \leq \int_ {I} f _ {+} + \varepsilon
$$

and 

$$
\int_ {I} \underline {{f _ {+}}} \geq \int_ {I} f _ {+} - \varepsilon .
$$

Note that $f _ { + }$ may be negative at places, but we can fix this by replacing $f _ { + }$ by $\operatorname* { m a x } ( \overline { { f } } _ { + } , 0 )$ , since this still minorizes $f _ { + } ^ { } \mathrm { ( w h y ? ) }$ and still has integral greater than or equal to $\begin{array} { r } { \int _ { I } f _ { + } - \varepsilon \ \left( \mathrm { w h y ? } \right) } \end{array}$ . So without loss of generality we may assume that $f _ { + } ( x ) \geq 0$ for all $x \in I$ . Similarly we may assume that $\overline { { f _ { + } } } ( x ) \leq M _ { 1 }$ for all $x \in I ;$ ; thus 

$$
0 \leq \underline {{f _ {+}}} (x) \leq f _ {+} (x) \leq \overline {{f _ {+}}} (x) \leq M _ {1}
$$

for all $x \in I$ 

Similar reasoning allows us to find piecewise constant $g _ { \pm }$ minorizing $g _ { + }$ , and $\overline { { g _ { + } } }$ majorizing $g _ { + }$ , such that 

$$
\int_ {I} \overline {{g _ {+}}} \leq \int_ {I} g _ {+} + \varepsilon
$$

and 

$$
\int_ {I} \underline {{g _ {+}}} \geq \int_ {I} g _ {+} - \varepsilon ,
$$

and 

$$
0 \leq \underline {{g _ {+}}} (x) \leq g _ {+} (x) \leq \overline {{g _ {+}}} (x) \leq M _ {2}
$$

for all $x \in I$ 

Notice that $f _ { + } g _ { + }$ is piecewise constant and minorizes $f _ { + } g _ { + }$ , while $\overline { { f _ { + } } } \overline { { g _ { + } } }$ is piecewise constant and majorizes $f _ { + } g _ { + }$ . Thus 

$$
0 \leq \overline {{\int}} _ {I} f _ {+} g _ {+} - \underline {{\int}} _ {I} f _ {+} g _ {+} \leq \int_ {I} \overline {{f _ {+}}} \overline {{g _ {+}}} - \underline {{f _ {+} g _ {+}}}.
$$

However, we have 

$$
\begin{array}{c} \overline {{f _ {+}}} (x) \overline {{g _ {+}}} (x) - \underline {{f _ {+}}} (x) \underline {{g _ {+}}} (x) = \overline {{f _ {+}}} (x) (\overline {{g _ {+}}} - \underline {{g _ {+}}}) (x) + \underline {{g _ {+}}} (x) (\overline {{f _ {+}}} - \underline {{f _ {+}}} (x)) \\ \leq M _ {1} (\overline {{g _ {+}}} - \underline {{g _ {+}}}) (x) + M _ {2} (\overline {{f _ {+}}} - \underline {{f _ {+}}} (x)) \end{array}
$$

for all $x \in I$ , and thus 

$$
\begin{array}{c} 0 \leq \overline {{\int}} _ {I} f _ {+} g _ {+} - \underline {{\int}} _ {I} f _ {+} g _ {+} \leq M _ {1} \int_ {I} (\overline {{g _ {+}}} - \underline {{g _ {+}}}) + M _ {2} \int_ {I} (\overline {{f _ {+}}} - \underline {{f _ {+}}}) \\ \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \leq M _ {1} (2 \varepsilon) + M _ {2} (2 \varepsilon). \end{array}
$$

Again, since $\varepsilon$ was arbitrary, we can conclude that $f _ { + } g _ { + }$ is Riemann integrable, as before. Similar argument show that $f _ { + } g _ { - } , \ f _ { - } g _ { + } , \ f _ { - } g _ { - }$ are Riemann integrable; combining them we obtain that $f g$ is Riemann integrable. □ 

— Exercises — 

Exercise 11.4.1. Prove Theorem 11.4.1. (Hint: you may find Theorem 11.2.16 to be useful. For part (b): First do the case $c > 0$ . Then do the case $c = - 1$ and $c = 0$ separately. Using these cases, deduce the case of $c < 0$ . You can use earlier parts of the theorem to prove later ones.) 

Exercise 11.4.2. Let $a \ < \ b$ be real numbers, and let $f : [ a , b ] \ \to \ \mathbf { R }$ be a continuous, non-negative function (so $f ( x ) \geq 0$ for all $x \in [ a , b ] )$ . Suppose that $\textstyle \int _ { [ a , b ] } f = 0$ . Show that $f ( x ) = 0$ for all $x \in [ a , b ]$ . (Hint: argue by <sub>contradiction.)</sub> 

Exercise 11.4.3. Let I be a bounded interval, let $f : I  \mathbf { R }$ be a Riemann integrable function, and let P be a partition of I. Show that 

$$
\int_ {I} f = \sum_ {J \in {\bf P}} \int_ {J} f.
$$

Exercise 11.4.4. Without repeating all the computations in the above proofs, give a short explanation as to why the remaining cases of Theorem 11.4.3 and Theorem 11.4.5 follow automatically from the cases presented in the text. (Hint: from Theorem 11.4.1 we know that if f is Riemann integrable, then so is $- f . )$ 

## 11.5 Riemann integrability of continuous functions

We have already said a lot about Riemann integrable functions so far, but we have not yet actually produced any such functions other than the piecewise constant ones. Now we rectify this by showing that a large class of useful functions are Riemann integrable. We begin with the uniformly continuous functions. 

Theorem 11.5.1. Let I be a bounded interval, and let f be a function which is uniformly continuous on I. Then f is Riemann integrable. 

Proof. From Proposition 9.9.15 we see that f is bounded. Now we have to show that $\textstyle \underline { { \int } } _ { I } f = { \overline { { \int } } } _ { I } f$ 

If I is a point or the empty set then the theorem is trivial, so let us assume that I is one of the four intervals $[ a , b ] , ( a , b ) , ( a , b ]$ , or [a, b) for some real numbers $a < b$ 

Let $\varepsilon > 0$ be arbitrary. By uniform continuity, there exists a $\delta > 0$ such that $| f ( x ) - f ( y ) | < \varepsilon$ whenever x, $y \in I$ are such that $| x - y | < \delta$ By the Archimedean principle, there exists an integer $N > 0$ such that $( b - a ) / N < \delta$ 

Note that we can partition I into N intervals $J _ { 1 } , \ldots , J _ { N }$ , each of length $( b - a ) / N$ . (How? One has to treat each of the cases $[ a , b ] , ( a , b )$ , $( a , b ] , [ a , b )$ slightly diferently.) By Proposition 11.3.12, we thus have 

$$
\overline {{\int}} _ {I} f \leq \sum_ {k = 1} ^ {N} (\sup _ {x \in J _ {k}} f (x)) | J _ {k} |
$$

and 

$$
\int_ {\underline {{I}}} f \geq \sum_ {k = 1} ^ {N} (\inf _ {x \in J _ {k}} f (x)) | J _ {k} |
$$

so in particular 

$$
\overline {{\int}} _ {I} f - \underline {{\int}} _ {- I} f \leq \sum_ {k = 1} ^ {N} (\sup _ {x \in J _ {k}} f (x) - \inf _ {x \in J _ {k}} f (x)) | J _ {k} |.
$$

However, we have $| f ( x ) - f ( y ) | < \varepsilon$ for all $x , y \in J _ { k }$ , since $| J _ { k } | =$ $( b - a ) / N < \delta$ . In particular we have 

$$
f (x) <   f (y) + \varepsilon \text {   for   all   } x, y \in J _ {k}.
$$

Taking suprema in $x ,$ we obtain 

$$
\sup _ {x \in J _ {k}} f (x) \leq f (y) + \varepsilon \text {   for   all   } y \in J _ {k},
$$

and then taking infima in y we obtain 

$$
\sup _ {x \in J _ {k}} f (x) \leq \inf _ {y \in J _ {k}} f (y) + \varepsilon .
$$

Inserting this bound into our previous inequality, we obtain 

$$
\overline {{\int}} _ {I} f - \underline {{\int}} _ {I} f \leq \sum_ {k = 1} ^ {N} \varepsilon | J _ {k} |,
$$

but by Theorem 11.1.13 we thus have 

$$
\overline {{\int}} _ {I} f - \underline {{\int}} _ {I} f \leq \varepsilon (b - a).
$$

But $\varepsilon > 0$ was arbitrary, while $( b - a )$ is fixed. Thus ${ \overline { { \int } } } _ { I } f - \underline { { \int } } _ { I } f$ cannot be positive. By Lemma 11.3.3 and the definition of Riemann integrability we thus have that $f$ is Riemann integrable. □ 

Combining Theorem 11.5.1 with Theorem 9.9.16, we thus obtain 

Corollary 11.5.2. Let $[ a , b ]$ be a closed interval, and let $f : [ a , b ]  \mathbf { R }$ be continuous. Then f is Riemann integrable. 

Note that this Corollary is not true if $[ a , b ]$ is replaced by any other sort of interval, since it is not even guaranteed then that continuous functions are bounded. For instance, the function $f : ( 0 , 1 )  \mathbf { R }$ defined by $f ( x ) : = 1 / x$ is continuous but not Riemann integrable. However, if we assume that a function is both continuous and bounded, we can recover Riemann integrability: 

Proposition 11.5.3. Let I be a bounded interval, and let $f : I  \mathbf { R }$ be both continuous and bounded. Then f is Riemann integrable on I. 

Proof. If I is a point or an empty set then the claim is trivial; if I is a closed interval the claim follows from Corollary 11.5.2. So let us assume that I is of the form $( a , b ] , ( a , b )$ , or $[ a , b )$ for some $a < b$ 

We have a bound M for f, so $\operatorname { t h a t } - M \leq f ( x ) \leq M$ for all $x \in I .$ Now let $0 < \varepsilon < ( b - a ) / 2$ be a small number. The function $f$ when restricted to the interval $[ a + \varepsilon , b - \varepsilon ]$ is continuous, and hence Riemann integrable by Corollary 11.5.2. In particular, we can find a piecewise constant function $h : [ a + \varepsilon , b - \varepsilon ] \to \mathbf { R }$ which majorizes $f$ on $[ a + \varepsilon , b - \varepsilon ]$ such that 

$$
\int_ {[ a + \varepsilon , b - \varepsilon ]} h \leq \int_ {[ a + \varepsilon , b - \varepsilon ]} f + \varepsilon .
$$

Define $\tilde { h } : I  \mathbf { R }$ by 

$$
\tilde {h} (x) := \left\{ \begin{array}{l l} h (x) & \text {if} x \in [ a + \varepsilon , b - \varepsilon ] \\ M & \text {if} x \in I \backslash [ a + \varepsilon , b - \varepsilon ] \end{array} \right.
$$

Clearly $\tilde { h }$ is piecewise constant on I and majorizes $f ;$ by Theorem 11.2.16 we have 

$$
\int_ {I} \tilde {h} = \varepsilon M + \int_ {[ a + \varepsilon , b - \varepsilon ]} h + \varepsilon M \leq \int_ {[ a + \varepsilon , b - \varepsilon ]} f + (2 M + 1) \varepsilon .
$$

In particular we have 

$$
\overline {{\int}} _ {I} f \leq \int_ {[ a + \varepsilon , b - \varepsilon ]} f + (2 M + 1) \varepsilon .
$$

A similar argument gives 

$$
\int_ {\underline {{I}}} f \geq \int_ {[ a + \varepsilon , b - \varepsilon ]} f - (2 M + 1) \varepsilon
$$

and hence 

$$
\overline {{\int}} _ {I} f - \underline {{\int}} _ {I} f \leq (4 M + 2) \varepsilon .
$$

But $\varepsilon$ is arbitrary, and so we can argue as in the proof of Theorem 11.5.1 to conclude Riemann integrability. □ 

This gives a large class of Riemann integrable functions already; the bounded continuous functions. But we can expand this class a little more, to include the bounded piecewise continuous functions. 

Definition 11.5.4. Let I be a bounded interval, and let $f : I  \mathbf { R }$ We say that $f$ is piecewise continuous on I if there exists a partition P of I such that $f | _ { J }$ is continuous on J for all $J \in \mathbf { P }$ 

Example 11.5.5. The function $f : [ 1 , 3 ] \to \mathbf { R }$ defined by 

$$
F (x) := \left\{ \begin{array}{l l} x ^ {2} & \text { if } 1 \leq x <   2 \\ 7 & \text { if } x = 2 \\ x ^ {3} & \text { if } 2 <   x \leq 3 \end{array} \right.
$$

is not continuous on [1, 3], but it is piecewise continuous on [1, 3] (since it is continuous when restricted to [1, 2) or 2 or (2, 3], and those three intervals partition [1, 3]). 

Proposition 11.5.6. Let I be a bounded interval, and let $f : I  \mathbf { R }$ be both piecewise continuous and bounded. Then f is Riemann integrable. 

Proof. See Exercise 11.5.1. 

— Exercises — 

Exercise 11.5.1. Prove Proposition 11.5.6. (Hint: use Theorem 11.4.1(a) and (h).) 

## 11.6 Riemann integrability of monotone functions

In addition to piecewise continuous functions, another wide class of functions is Riemann integrable, namely the monotone functions. We give two instances of this: 

Proposition 11.6.1. Let $[ a , b ]$ be a closed and bounded interval and let $f : [ a , b ]  \mathbf { R }$ be a monotone function. Then f is Riemann integrable on $[ a , b ]$ 

Remark 11.6.2. From Exercise 9.8.5 we know that there exist monotone functions which are not piecewise continuous, so this proposition is not subsumed by Proposition 11.5.6. 

Proof. Without loss of generality we may take f to be monotone increasing (instead of monotone decreasing). From Exercise 9.8.1 we know that f is bounded. Now let $N > 0$ be an integer, and partition $[ a , b ]$ into N half-open intervals $\begin{array} { r } { \{ [ a + \frac { b - a } { N } j , a + \frac { b - a } { N } ( j + 1 ) ) : 0 \leq j \leq N - 1 \} } \end{array}$ of length $( b - a ) / N$ , together with the point $\{ b \}$ . Then by Proposition 11.3.12 we have 

$$
\overline {{\int}} _ {I} f \leq \sum_ {j = 0} ^ {N - 1} \left(\sup _ {x \in [ a + \frac {b - a}{N} j, a + \frac {b - a}{N} (j + 1))} f (x)\right) \frac {b - a}{N},
$$

(the point $\{ b \}$ clearly giving only a zero contribution). Since f is monotone increasing, we thus have 

$$
\overline {{\int}} _ {I} f \leq \sum_ {j = 0} ^ {N - 1} f \left(a + \frac {b - a}{N} (j + 1)\right) \frac {b - a}{N}.
$$

Similarly we have 

$$
\int_ {\underline {{I}}} f \geq \sum_ {j = 0} ^ {N - 1} f \left(a + \frac {b - a}{N} j\right) \frac {b - a}{N}.
$$

Thus we have 

$$
\overline {{\int}} _ {I} f - \underline {{\int}} _ {I} f \leq \sum_ {j = 0} ^ {N - 1} \left(f \left(a + \frac {b - a}{N} (j + 1)\right) - f \left(a + \frac {b - a}{N} j\right)\right) \frac {b - a}{N}.
$$

Using telescoping series (Lemma 7.2.15) we thus have 

$$
\begin{array}{c} \overline {{\int}} _ {I} f - \underline {{\int}} _ {I} f \leq \left(f \left(a + \frac {b - a}{N} (N)\right) - f \left(a + \frac {b - a}{N} 0\right)\right) \frac {b - a}{N} \\ = (f (b) - f (a)) \frac {b - a}{N}. \end{array}
$$

But N was arbitrary, so we can conclude as in the proof of Theorem 11.5.1 that f is Riemann integrable. □ 

Corollary 11.6.3. Let I be a bounded interval, and let $f : I  \mathbf { R }$ be both monotone and bounded. Then f is Riemann integrable on I. 

Proof. See Exercise 11.6.1. 

We now give the famous integral test for determining convergence of monotone decreasing series. 

Proposition 11.6.4 (Integral test). Let $f : [ 0 , \infty )  \mathbf { R }$ be a monotone decreasing function which is non-negative $( i . e . , f ( x ) \geq 0$ for all $x \geq 0 )$ Then the sum $\textstyle \sum _ { n = 0 } ^ { \infty } f ( n )$ is convergent if and only if $\scriptstyle \operatorname* { s u p } _ { N > 0 } \int _ { [ 0 , N ] } f$ is finite. 

Proof. See Exercise 11.6.3. 

Corollary 11.6.5. Let p be a real number. Then $\textstyle \sum _ { n = 1 } ^ { \infty } { \frac { 1 } { n ^ { p } } }$ converges absolutely when $p > 1$ and diverges when $p \leq 1$ 

Proof. See Exercise 11.6.5. 

— Exercises — 

Exercise 11.6.1. Use Proposition 11.6.1 to prove Corollary 11.6.3. (Hint: adapt the proof of Proposition 11.5.3.) 

Exercise 11.6.2. Formulate a reasonable notion of a piecewise monotone function, and then show that all bounded piecewise monotone functions are Riemann integrable. 

Exercise 11.6.3. Prove Proposition 11.6.4. (Hint: what is the relationship between the sum $\textstyle \sum _ { n = 1 } ^ { N } f ( n )$ , the sum $\textstyle \sum _ { n = 0 } ^ { N - 1 } { f ( n ) }$ , and the integral $\int _ { [ 0 , N ] } f ( \underline { { \tau } } )$ 

Exercise 11.6.4. Give examples to show that both directions of the integral test break down if f is not assumed to be monotone decreasing. 

Exercise 11.6.5. Use Proposition 11.6.4 to prove Corollary 11.6.5. 

## 11.7 A non-Riemann integrable function

We have shown that there are large classes of bounded functions which are Riemann integrable. Unfortunately, there do exist bounded functions which are not Riemann integrable: 

Proposition 11.7.1. Let $f : [ 0 , 1 ] \to \mathbf { R }$ be the discontinuous function 

$$
f (x) := \left\{ \begin{array}{l l} 1 & \text {if} x \in \mathbf {Q} \\ 0 & \text {if} x \not \in \mathbf {Q} \end{array} \right.
$$

considered in Example 9.3.21. Then f is bounded but not Riemann integrable. 

Proof. It is clear that f is bounded, so let us show that it is not Riemann integrable. 

Let P be any partition of [0, 1]. For any $J \in \mathbf { P }$ , observe that if J is not a point or the empty set, then 

$$
\sup _ {x \in J} f (x) = 1
$$

(by Proposition 5.4.14). In particular we have 

$$
\left(\sup _ {x \in J} f (x)\right) | J | = | J |.
$$

(Note this is also true when J is a point, since both sides are zero.) In particular we see that 

$$
U (f, \mathbf {P}) = \sum_ {J \in \mathbf {P}: J \neq \emptyset} | J | = | [ 0, 1 ] | = 1
$$

by Theorem 11.1.13; note that the empty set does not contribute anything to the total length. In particular we have $\begin{array} { r } { \overline { { \int } } _ { [ 0 , 1 ] } f = 1 } \end{array}$ , by Proposition 11.3.12. 

A similar argument gives that 

$$
\inf _ {x \in J} f (x) = 0
$$

for all J (other than points or the empty set), and so 

$$
L (f, \mathbf {P}) = \sum_ {J \in \mathbf {P}: J \neq \emptyset} 0 = 0.
$$

In particular we have $\underline { { \boldsymbol { f } } } _ { [ 0 , 1 ] } f = 0$ , by Proposition 11.3.12. Thus the upper and lower Riemann integrals do not match, and so this function is not Riemann integrable. □ 

Remark 11.7.2. As you can see, it is only rather “artificial” bounded functions which are not Riemann integrable. Because of this, the Riemann integral is good enough for a large majority of cases. There are ways to generalize or improve this integral, though. One of these is the Lebesgue integral, which we will define in Chapter 11.45. Another is the Riemann-Stieltjes integral $\textstyle \int _ { I } f d \alpha$ , where $\alpha : I  \mathbf { R }$ is a monotone increasing function, which we define in the next section. 

## 11.8 The Riemann-Stieltjes integral

Let I be a bounded interval, let $\alpha : I  \mathbf { R }$ be a monotone increasing function, and let $f : I  \mathbf { R }$ be a function. Then there is a generalization of the Riemann integral, known as the Riemann-Stieltjes integral. This integral is defined just like the Riemann integral, but with one twist: instead of taking the length J of intervals J, we take the α-length $\alpha [ J ]$ , defined as follows. If J is a point or the empty set, then $\alpha [ J ] : = 0$ If J is an interval of the form $[ a , b ] , ( a , b ) , ( a , b ] , \mathrm { o r } [ a , b )$ , then $\alpha [ J ] : =$ $\alpha ( b ) - \alpha ( a )$ . Note that in the special case where α is the identity function $\alpha ( x ) : = x$ , then $\alpha [ J ]$ is just the same as J . However, for more general monotone functions α, the α-length $\alpha [ J ]$ is a diferent quantity from J . Nevertheless, it turns out one can still do much of the above theory, but replacing J by $\alpha [ J ]$ throughout. 

Definition 11.8.1 (α-length). Let I be a bounded interval, and let $\alpha : X  \mathbf { R }$ be a function defined on some domain X which contains I. Then we define the α-length $\alpha [ I ]$ of I as follows. If I is a point or the empty set, we set $\alpha [ I ] = 0$ . If I is an interval of the form $[ a , b ] , [ a , b )$ $( a , b ]$ , or $( a , b )$ for some $b > a ,$ , then we set $\alpha [ I ] = \alpha ( b ) - \alpha ( a )$ 

Example 11.8.2. Let $\alpha : \mathbf { R }  \mathbf { R }$ be the function $\alpha ( x ) : = x ^ { 2 }$ . Then $\alpha [ [ 2 , 3 ] ] = \alpha ( 3 ) - \alpha ( 2 ) = 9 - 4 = 5$ , while $\alpha [ ( - 3 , - 2 ) ] = - 5$ . Meanwhile $\alpha [ \{ 2 \} ] = 0$ and $\alpha [ \varnothing ] = 0$ 

Example 11.8.3. Let $\alpha : \mathbf { R }  \mathbf { R }$ be the identity function $\alpha ( x ) : = x$ Then $\alpha [ I ] = | I |$ for all bounded intervals I (why?) Thus the notion of length is a special case of the notion of α-length. 

We sometimes write $\alpha | _ { a } ^ { b }$ or $\alpha ( x ) | _ { x = a } ^ { x = b }$ instead of $\alpha [ [ a , b ] ]$ 

One of the key theorems for the theory of the Riemann integra was Theorem 11.1.13, which concerned length and partitions, and in particular showed that $\begin{array} { r } { | I | = \sum _ { J \in \mathbf { P } } | J | } \end{array}$ whenever P was a partition of I. We now generalize this slightly. 

Lemma 11.8.4. Let I be a bounded interval, let $\alpha : X  \mathbf { R }$ be a function defined on some domain X which contains I, and let P be $a$ partition of I. Then we have 

$$
\alpha [ I ] = \sum_ {J \in \mathbf {P}} \alpha [ J ].
$$

Proof. See Exercise 11.8.1. 

□ 

We can now define a generalization of Definition 11.2.9. 

Definition 11.8.5 (P.c. Riemann-Stieltjes integral). Let I be a bounded interval, and let P be a partition of I. Let $\alpha : X  \mathbf { R }$ be a function defined on some domain X which contains I, and let $f : I  \mathbf { R }$ be a function which is piecewise constant with respect to P. Then we define 

$$
p. c. \int_ {[ \mathbf {P} ]} f d \alpha := \sum_ {J \in \mathbf {P}} c _ {J} \alpha [ J ]
$$

where $c _ { J }$ is the constant value of f on $J .$ 

Example 11.8.6. Let $f : [ 1 , 3 ] \to \mathbf { R }$ be the function 

$$
f (x) = \left\{ \begin{array}{l l} 4 & \text {when x\in [1,2)} \\ 2 & \text {when x\in [2,3]}, \end{array} \right.
$$

let $\alpha : \mathbf { R }  \mathbf { R }$ be the function $\alpha ( x ) : = x ^ { 2 }$ , and let P be the partition ${ \bf P } : = \{ [ 1 , 2 ) , [ 2 , 3 ] \}$ . Then 

$$
\begin{array}{l} p. c. \int_ {[ \mathbf {P} ]} f d \alpha = c _ {[ 1, 2)} \alpha [ [ 1, 2) ] + c _ {[ 2, 3 ]} \alpha [ [ 2, 3 ] ] \\ = 4 (\alpha (2) - \alpha (1)) + 2 (\alpha (3) - \alpha (2)) = 4 \times 3 + 2 \times 5 = 2 2. \end{array}
$$

Example 11.8.7. Let $\alpha : \mathbf { R }  \mathbf { R }$ be the identity function $\alpha ( x ) : = x$ Then for any bounded interval I, any partition P of I, and any function f that is piecewise constant with respect to P, we have $\begin{array} { r } { p . c . \int _ { [ \mathbf { P } ] } f \ d \alpha = } \end{array}$ $p . c . \int _ { [ \mathbf { P } ] } f \ ( \mathrm { w h y ? } )$ 

We can obtain an exact analogue of Proposition 11.2.13 by replacing all the integrals $p . c . \int _ { [ \mathbf { P } ] } f$ in the proposition with $p . c . \int _ { [ \mathbf { P } ] } f$ dα (Exercise 11.8.2). We can thus define $p . c . \int _ { I } f$ dα for any piecewise constant function $f : I  \mathbf { R }$ and any α $: X  \mathbf { R }$ defined on a domain containing I, in analogy to before, by the formula 

$$
p. c. \int_ {I} f d \alpha := p. c. \int_ {[ \mathbf {P} ]} f d \alpha
$$

for any partition P on I with respect to which f is piecewise constant. 

Up until now, our function $\alpha : \mathbf { R }  \mathbf { R }$ could have been arbitrary. Let us now assume that α is monotone increasing, i.e., $\alpha ( y ) \ge \alpha ( x )$ whenever $x , y \in X$ are such that $y \geq x$ . This implies that $\alpha ( I ) \geq 0$ for all intervals in X (why?). From this one can easily verify that all the results from Theorem 11.2.16 continue to hold when the integrals $p . c . \int _ { I } f$ are replaced by $p . c . \int _ { I } f$ dα, and the lengths $| I |$ are replaced by the α-lengths $\alpha ( I )$ ; see Exercise 11.8.3. 

We can then define upper and lower Riemann-Stieltjes integrals $\overline { { \int } } _ { I } f$ dα and $\underline { { \boldsymbol { \int } } } _ { I } \boldsymbol { f }$ dα whenever $f : I  \mathbf { R }$ is bounded and α is defined on a domain containing I, by the usual formulae 

$$
\overline {{\int}} _ {I} f d \alpha := \inf \{p. c. \int_ {I} g d \alpha : g \text {is p.c. on I and majorizes} f \}
$$

and 

$$
\underline {{\int}} _ {I} f d \alpha := \sup \{p. c. \int_ {I} g d \alpha : g \text {is p.c. on I and minorizes} f \}.
$$

We then say that f is Riemann-Stieltjes integrable on I with respect to α if the upper and lower Riemann-Stieltjes integrals match, in which case we set 

$$
\int_ {I} f d \alpha := \overline {{\int}} _ {I} f d \alpha = \underline {{\int}} _ {I} f d \alpha .
$$

As before, when α is the identity function $\alpha ( x ) \ : = \ x$ then the Riemann-Stieltjes integral is identical to the Riemann integral; thus the Riemann-Stieltjes integral is a generalization of the Riemann integral. 

(We shall see another comparison between the two integrals a little later, in Corollary 11.10.3.) Because of this, we sometimes write $\textstyle \int _ { I } f$ as $\textstyle \int _ { I } f$ dx or $\textstyle \int _ { I } f ( x )$ dx. 

Most (but not all) of the remaining theory of the Riemann integral then can be carried over without dificulty, replacing Riemann integrals with Riemann-Stieltjes integrals and lengths with α-lengths. There are a couple results which break down; Theorem 11.4.1(g), Proposition 11.5.3, and Proposition 11.5.6 are not necessarily true when α is discontinuous at key places $( \mathrm { e . g . }$ , if f and α are both discontinuous at the same point, then $\textstyle \int _ { I } f$ dα is unlikely to be defined. However, Theorem 11.5.1 is still true (Exercise 11.8.4). 

## — Exercises —

Exercise 11.8.1. Prove Lemma 11.8.4. (Hint: modify the proof of Theorem 11.1.13.) 

Exercise 11.8.2. State and prove a version of Proposition 11.2.13 for the Riemann-Stieltjes integral. 

Exercise 11.8.3. State and prove a version of Theorem 11.2.16 for the Riemann-Stieltjes integral. 

Exercise 11.8.4. State and prove a version of Theorem 11.5.1 for the Riemann-Stieltjes integral. (Hint: one has to be careful with the proof; the problem here is that some of the references to the length of $| J _ { k } |$ should remain unchanged, and other references to the length of $| J _ { k } |$ should be changed to the α-length $\alpha ( J _ { k } )$ - basically, all of the occurrences of $| J _ { k } |$ which appear inside a summation should be replaced with $\alpha ( J _ { k } )$ , but the rest should be unchanged.) 

Exercise 11.8.5. Let sgn : $\mathbf R \to \mathbf R$ be the signum function 

$$
\operatorname{sgn} (x) := \left\{ \begin{array}{l l} 1 & \text {when x > 0} \\ 0 & \text {when x = 0} \\ - 1 & \text {when x <   0}. \end{array} \right.
$$

Let $f : [ - 1 , 1 ] \to \mathbf { R }$ be a continuous function. Show that f is Riemann-Stieltjes integrable with respect to sgn, and that 

$$
\int_ {[ - 1, 1 ]} f d \mathrm{sgn} = 2 f (0).
$$

(Hint: for every $\varepsilon > 0$ , find piecewise constant functions majorizing and minorizing f whose Riemann-Stieltjes integral is ε-close to $2 f ( 0 ) . )$ ) 

## 11.9 The two fundamental theorems of calculus

We now have enough machinery to connect integration and diferentiation via the familiar fundamental theorem of calculus. Actually, there are two such theorems, one involving the derivative of the integral, and the other involving the integral of the derivative. 

Theorem 11.9.1 (First Fundamental Theorem of Calculus). Let $a < b$ be real numbers, and let $f : [ a , b ]  \mathbf { R }$ be a Riemann integrable function. Let $F : [ a , b ] \to \mathbf { R }$ be the function 

$$
F (x) := \int_ {[ a, x ]} f.
$$

Then F is continuous. Furthermore, if $x _ { 0 } \in [ a , b ]$ and f is continuous at $x _ { 0 }$ , then F is diferentiable at $x _ { 0 }$ , and $F ^ { \prime } ( x _ { 0 } ) = f ( x _ { 0 } )$ 

Proof. Since f is Riemann integrable, it is bounded (by Definition 11.3.4). Thus we have some real number M such that $- M \leq f ( x ) \leq M$ for all $x \in [ a , b ]$ 

Now let $x < y$ be two elements of $[ a , b ]$ . Then notice that 

$$
F (y) - F (x) = \int_ {[ a, y ]} f - \int_ {[ a, x ]} f = \int_ {[ x, y ]} f
$$

by Theorem 11.4.1(h). By Theorem 11.4.1(e) we thus have 

$$
\int_ {[ x, y ]} f \leq \int_ {[ x, y ]} M = p. c. \int_ {[ x, y ]} M = M (y - x)
$$

and 

$$
\int_ {[ x, y ]} f \geq \int_ {[ x, y ]} - M = p. c. \int_ {[ x, y ]} - M = - M (y - x)
$$

and thus 

$$
| F (y) - F (x) | \leq M (y - x).
$$

This is for $y > x$ . By interchanging x and y we thus see that 

$$
| F (y) - F (x) | \leq M (x - y)
$$

when $x > y$ . Also, we have $F ( y ) - F ( x ) = 0$ when $x = y$ . Thus in all three cases we have 

$$
| F (y) - F (x) | \leq M | x - y |.
$$

Now let $x \in [ a , b ]$ , and let $( x _ { n } ) _ { n = 0 } ^ { \infty }$ be any sequence in $[ a , b ]$ converging to x. Then we have 

$$
- M | x _ {n} - x | \leq F (x _ {n}) - F (x) \leq M | x _ {n} - x |
$$

for each n. But $- M | x _ { n } - x |$ and $M | x _ { n } - x |$ both converge to 0 as $n \to \infty$ • so by the squeeze test $F ( x _ { n } ) - F ( x )$ converges to 0 as $n \to \infty$ , and thus $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } F ( x _ { n } ) = F ( x ) } \end{array}$ . Since this is true for all sequences $x _ { n } \in [ a , b ]$ converging to $x ,$ we thus see that $F$ is continuous at $x .$ . Since x was an arbitrary element of $[ a , b ]$ , we thus see that $F$ is continuous. 

Now suppose that $x _ { 0 } \in [ a , b ]$ , and f is continuous at $x _ { 0 }$ . Choose any $\varepsilon > 0$ . Then by continuity, we can find $\mathrm { ~ a ~ } \delta > 0$ such that $| f ( x ) - f ( x _ { 0 } ) | \leq$ $\varepsilon$ for all $x$ in the interval $I : = [ x _ { 0 } - \delta , x _ { 0 } + \delta ] \cap [ a , b ]$ , or in other words 

$$
f (x _ {0}) - \varepsilon \leq f (x) \leq f (x _ {0}) + \varepsilon \text {   for   all   } x \in I.
$$

We now show that 

$$
| F (y) - F (x _ {0}) - f (x _ {0}) (y - x _ {0}) | \leq \varepsilon | y - x _ {0} |
$$

for all $y \in I$ , since Proposition 10.1.7 will then imply that $F$ is diferentiable at $x _ { 0 }$ with derivative $F ^ { \prime } ( x _ { 0 } ) = f ( x _ { 0 } )$ as desired. 

Now fix $y \in I$ . There are three cases. If $y = x _ { 0 }$ , then $F ( y ) - F ( x _ { 0 } ) -$ $f ( x _ { 0 } ) ( y - x _ { 0 } ) = 0$ and so the claim is obvious. If $y > x _ { 0 }$ , then 

$$
F (y) - F (x _ {0}) = \int_ {[ x _ {0}, y ]} f.
$$

Since $x _ { 0 } , y \in I$ , and I is a connected set, then $[ x _ { 0 } , y ]$ is a subset of $I ,$ and thus we have 

$$
f (x _ {0}) - \varepsilon \leq f (x) \leq f (x _ {0}) + \varepsilon \text {   for   all   } x \in [ x _ {0}, y ],
$$

and thus 

$$
(f (x _ {0}) - \varepsilon) (y - x _ {0}) \leq \int_ {[ x _ {0}, y ]} f \leq (f (x _ {0}) + \varepsilon) (y - x _ {0})
$$

and so in particular 

$$
| F (y) - F (x _ {0}) - f (x _ {0}) (y - x _ {0}) | \leq \varepsilon | y - x _ {0} |
$$

as desired. The case $y < x _ { 0 }$ is similar and is left to the reader. 

Example 11.9.2. Recall in Exercise 9.8.5 that we constructed a monotone function $f : \mathbf { R }  \mathbf { R }$ which was discontinuous at every rational and continuous everywhere else. By Proposition 11.6.1, this monotone function is Riemann integrable on [0, 1]. If we define $F : [ 0 , 1 ] \to \mathbf { R }$ by $\begin{array} { r } { F ( x ) : = \int _ { [ 0 , x ] } f } \end{array}$ , then $F$ is a continuous function which is diferentiable at every irrational number. On the other hand, $F$ is non-diferentiable at every rational number; see Exercise 11.9.1. 

Informally, the first fundamental theorem of calculus asserts that 

$$
\left(\int_ {[ a, x ]} f\right) ^ {\prime} (x) = f (x)
$$

given a certain number of assumptions on $f .$ Roughly, this means that the derivative of an integral recovers the original function. Now we show the reverse, that the integral of a derivative recovers the origina function. 

Definition 11.9.3 (Antiderivatives). Let I be a bounded interval, and let $f : I  \mathbf { R }$ be a function. We say that a function $F : I  \mathbf { R }$ is an antiderivative of f if $F$ is diferentiable on I and $F ^ { \prime } ( x ) = f ( x )$ for all $x \in I$ 

Theorem 11.9.4 (Second Fundamental Theorem of Calculus). Let $a < b$ be real numbers, and let $f : [ a , b ]  \mathbf { R }$ be a Riemann integrable function. If $F : [ a , b ]  \mathbf { R }$ is an antiderivative of $f _ { i }$ , then 

$$
\int_ {[ a, b ]} f = F (b) - F (a).
$$

Proof. We will use Riemann sums. The idea is to show that 

$$
U (f, \mathbf {P}) \geq F (b) - F (a) \geq L (f, \mathbf {P})
$$

for every partition P of $[ a , b ]$ . The left inequality asserts that $F ( b ) { - } F ( a )$ is a lower bound for $\{ U ( f , { \mathbf { P } } ) : { \mathbf { P } }$ is a partition of $[ a , b ] \}$ , while the right inequality asserts that $F ( b ) - F ( a )$ is an upper bound for $\{ L ( f , \mathbf { P } ) : \mathbf { P }$ is a partition of $[ a , b ] \}$ . But by Proposition 11.3.12, this means that 

$$
\overline {{\int}} _ {[ a, b ]} f \geq F (b) - F (a) \geq \underline {{\int}} _ {[ a, b ]} f,
$$

but since $f$ is assumed to be Riemann integrable, both the upper and lower Riemann integral equal $\int _ { [ a , b ] } f$ . The claim follows. 

<sub>We have to show the bound</sub> $\dot { U } ( f , { \mathbf { P } } ) \ge F ( b ) - F ( a ) \ge L ( f , { \mathbf { P } } )$ . We shall just show the first inequality $U ( f , \mathbf { P } ) \geq F ( b ) - F ( a )$ ; the other inequality is similar. 

Let P be a partition of $[ a , b ]$ . From Lemma 11.8.4 we have 

$$
F (b) - F (a) = \sum_ {J \in \mathbf {P}} F [ J ] = \sum_ {J \in \mathbf {P}: J \neq \emptyset} F [ J ],
$$

while from definition we have 

$$
U (f, \mathbf {P}) = \sum_ {J \in \mathbf {P}: J \neq \emptyset} \sup _ {x \in J} f (x) | J |.
$$

Thus it will sufice to show that 

$$
F [ J ] \leq \sup _ {x \in J} f (x) | J |
$$

for all $J \in \mathbf { P }$ (other than the empty set). 

When J is a point then the claim is clear, since both sides are zero. Now suppose that $J = [ c , d ] , ( c , d ] , [ c , d )$ , or $( c , d )$ for some $c < d$ . Then the left-hand side is $F [ J ] = F ( d ) - F ( c )$ . By the mean-value theorem, this is equal to $( d - c ) F ^ { \prime } ( e )$ for some $e \in J$ . But since $F ^ { \prime } ( e ) = f ( e )$ , we thus have 

$$
F [ J ] = (d - c) f (e) = f (e) | J | \leq \sup _ {x \in J} f (x) | J |
$$

as desired. 

□ 

Of course, as you are all aware, one can use the second fundamental theorem of calculus to compute integrals relatively easily provided that you can find an anti-derivative of the integrand $f .$ . Note that the first fundamental theorem of calculus ensures that every continuous Riemann integrable function has an anti-derivative. For discontinuous functions, the situation is more complicated, and is $\mathrm { a }$ graduate-level real analysis topic which will not be discussed here. Also, not every function with an anti-derivative is Riemann integrable; as an example, consider the function $F : [ - 1 , 1 ] \to \mathbf { R }$ defined by $F ( x ) : = x ^ { 2 } \sin ( 1 / x ^ { 3 } )$ when $x \neq 0$ 2 and $F ( 0 ) : = 0$ . Then $F$ is diferentiable everywhere (why?), so $F ^ { \prime }$ has an antiderivative, but $F ^ { \prime }$ is unbounded $\mathrm { \left( w h y ? \right) }$ , and so is not Riemann integrable. 

We now pause to mention the infamous $^ { 6 6 } + C ^ { 9 9 }$ ambiguity in antiderivatives: 

Lemma 11.9.5. Let I be a bounded interval, and let $f : I  \mathbf { R }$ be a function. Let $F : I  \mathbf { R }$ and $G : I  \mathbf { R }$ be two antiderivatives of $f .$ Then there exists a real number $C$ such that $F ( x ) = G ( x ) + C$ for all $x \in I$ 

Proof. See Exercise 11.9.2. 

— Exercises — 

Exercise 11.9.1. Let $f : [ 0 , 1 ] \to \mathbf { R }$ be the function in Exercise 9.8.5. Show that for every rational number $q \in \mathbf { Q } \cap [ 0 , 1 ]$ , the function $F : [ 0 , 1 ]  \mathbf { R }$ defined by the formula $\begin{array} { r } { F ( x ) : = \int _ { 0 } ^ { x } f ( \bar { y } ) } \end{array}$ dy is not diferentiable at $q .$ 

Exercise 11.9.2. Prove Lemma 11.9.5. (Hint: apply the mean-value theorem, Corollary 10.2.9, to the function $F - G$ . One can also prove this lemma using the second Fundamental theorem of calculus (how?), but one has to be careful since we do not assume f to be Riemann integrable.) 

Exercise 11.9.3. Let $a \ < \ b$ be real numbers, and let $f : [ a , b ] \ \to \ \mathbf { R }$ be a monotone increasing function. Let $F : [ a , b ] \to \mathbf { R }$ be the function $F ( x ) : =$ $\int _ { [ a , x ] } f .$ . Let $x _ { 0 }$ be an element of $[ a , b ]$ . Show that $F$ is diferentiable at $x _ { 0 }$ if <sub>and only if</sub> $f$ is continuous at $x _ { 0 }$ . (Hint: one direction is taken care of by one of the fundamental theorems of calculus. For the other, consider left and right limits of $f$ and argue by contradiction.) 

## 11.10 Consequences of the fundamental theorems

We can now give a number of useful consequences of the fundamental theorems of calculus (beyond the obvious application, that one can now compute any integral for which an anti-derivative is known). The first application is the familiar integration by parts formula. 

Proposition 11.10.1 (Integration by parts formula). Let $I = [ a , b ]$ , and let $F : [ a , b ] \to \mathbf { R }$ and $G : [ a , b ] \to \mathbf { R }$ be diferentiable functions on $[ a , b ]$ such that $F ^ { \prime }$ and $G ^ { \prime }$ are Riemann integrable on I. Then we have 

$$
\int_ {[ a, b ]} F G ^ {\prime} = F (b) G (b) - F (a) G (a) - \int_ {[ a, b ]} F ^ {\prime} G.
$$

Proof. See Exercise 11.10.1. 

Next, we show that under certain circumstances, one can write a Riemann-Stieltjes integral as a Riemann integral. We begin with piecewise constant functions. 

Theorem 11.10.2. Let $\alpha : [ a , b ]  \mathbf { R }$ be a monotone increasing function, and suppose that α is also diferentiable on $[ a , b ]$ , with α being Riemann integrable. Let $f : [ a , b ]  \mathbf { R }$ be a piecewise constant function on $[ a , b ]$ . Then $f \alpha ^ { \prime }$ is Riemann integrable on $[ a , b ]$ , and 

$$
\int_ {[ a, b ]} f d \alpha = \int_ {[ a, b ]} f \alpha^ {\prime}.
$$

Proof. Since f is piecewise constant, it is Riemann integrable, and since $\alpha ^ { \prime }$ is also Riemann integrable, then $f \alpha ^ { \prime }$ is Riemann integrable by Theorem 11.4.5. 

Suppose that f is piecewise constant with respect to some partition P of $[ a , b ]$ ; without loss of generality we may assume that P does not contain the empty set. Then we have 

$$
\int_ {[ a, b ]} f d \alpha = p. c. \int_ {[ \mathbf {P} ]} f d \alpha = \sum_ {J \in \mathbf {P}} c _ {J} \alpha [ J ]
$$

where $c _ { J }$ is the constant value of f on J. On the other hand, from Theorem 11.2.16(h) (generalized to partitions of arbitrary length - why is this generalization true?) we have 

$$
\int_ {[ a, b ]} f \alpha^ {\prime} = \sum_ {J \in \mathbf {P}} \int_ {J} f \alpha^ {\prime} = \sum_ {J \in \mathbf {P}} \int_ {J} c _ {J} \alpha^ {\prime} = \sum_ {J \in \mathbf {P}} c _ {J} \int_ {J} \alpha^ {\prime}.
$$

But by the second fundamental theorem of calculus (Theorem 11.9.4), $\begin{array} { r } { \int _ { J } \alpha ^ { \prime } = \alpha [ J ] } \end{array}$ , and the claim follows. □ 

Corollary 11.10.3. Let $\alpha : [ a , b ]  \mathbf { R }$ be a monotone increasing function, and suppose that α is also diferentiable on $[ a , b ]$ , with $\alpha ^ { \prime }$ being Riemann integrable. Let $f : [ a , b ]  \mathbf { R }$ be a function which is Riemann-Stieltjes integrable with respect to α on $[ a , b ]$ . Then $f \alpha ^ { \prime }$ is Riemann integrable on $[ a , b ]$ , and 

$$
\int_ {[ a, b ]} f d \alpha = \int_ {[ a, b ]} f \alpha^ {\prime}.
$$

Proof. Note that since f and $\alpha ^ { \prime }$ are bounded, then $f \alpha ^ { \prime }$ must also be bounded. Also, since α is monotone increasing and diferentable, $\alpha ^ { \prime }$ is non-negative. 

Let $\varepsilon > 0$ . Then, we can find a piecewise constant function $\overline { { f } }$ majorizing f on $[ a , b ]$ , and a piecewise constant function $\underline { { f } }$ minorizing $f$ on $[ a , b ]$ , such that 

$$
\int_ {[ a, b ]} f d \alpha - \varepsilon \leq \int_ {[ a, b ]} \underline {{f}} d \alpha \leq \int_ {[ a, b ]} \overline {{f}} d \alpha \leq \int_ {[ a, b ]} f d \alpha + \varepsilon .
$$

Applying Theorem 11.10.2, we obtain 

$$
\int_ {[ a, b ]} f d \alpha - \varepsilon \leq \int_ {[ a, b ]} \underline {{f}} \alpha^ {\prime} \leq \int_ {[ a, b ]} \overline {{f}} \alpha^ {\prime} \leq \int_ {[ a, b ]} f d \alpha + \varepsilon .
$$

Since $\alpha ^ { \prime }$ is non-negative and $\underline { { f } }$ minorizes f, then $f \alpha ^ { \prime }$ minorizes $f \alpha ^ { \prime }$ Thus $\underline { { { \int } } } _ { [ a , b ] } \underline { { { f } } } \alpha ^ { \prime } \le \underline { { { \int } } } _ { [ a , b ] } f \alpha ^ { \prime }$ (why?). Thus 

$$
\int_ {[ a, b ]} f d \alpha - \varepsilon \leq \int_ {\underline {{\quad}} [ a, b ]} f \alpha^ {\prime}.
$$

Similarly we have 

$$
\overline {{\int}} _ {[ a, b ]} f \alpha^ {\prime} \leq \int_ {[ a, b ]} f d \alpha + \varepsilon .
$$

Since these statements are true for any $\varepsilon > 0$ , we must have 

$$
\int_ {[ a, b ]} f d \alpha \leq \underline {{\int_ {[ a , b ]}}} f \alpha^ {\prime} \leq \overline {{\int_ {[ a , b ]}}} f \alpha^ {\prime} \leq \int_ {[ a, b ]} f d \alpha
$$

and the claim follows. 

□ 

Remark 11.10.4. Informally, Corollary 11.10.3 asserts that f dα is essentially equivalent to $\textstyle f { \frac { d \alpha } { d x } } d x$ , when α is diferentiable. However, the advantage of the Riemann-Stieltjes integral is that it still makes sense even when α is not diferentiable. 

We now build up to the familiar change of variables formula. We first need a preliminary lemma. 

Lemma 11.10.5 (Change of variables formula I). Let $[ a , b ]$ be a closed interval, and let $\phi : [ a , b ]  [ \phi ( a ) , \phi ( b ) ]$ be a continuous monotone increasing function. Let $f : [ \phi ( a ) , \phi ( b ) ] \to \mathbf { R }$ be a piecewise constant function on $[ \phi ( a ) , \phi ( b ) ]$ . Then $f \circ \phi : [ a , b ]  \mathbf { R }$ is also piecewise constant on $[ a , b ]$ , and 

$$
\int_ {[ a, b ]} f \circ \phi d \phi = \int_ {[ \phi (a), \phi (b) ]} f.
$$

Proof. We give a sketch of the proof, leaving the gaps to be filled in Exercise 11.10.2. Let P be a partition of $[ \phi ( a ) , \phi ( b ) ]$ such that f is piecewise constant with respect to P; we may assume that P does not contain the empty set. For each $J \in \mathbf { P }$ , let $c _ { J }$ be the constant value of $f$ on J, thus 

$$
\int_ {[ \phi (a), \phi (b) ]} f = \sum_ {J \in \mathbf {P}} c _ {J} | J |.
$$

For each interval $J ,$ let $\phi ^ { - 1 } ( J )$ be the set $\phi ^ { - 1 } ( J ) : = \{ x \in [ a , b ] : \phi ( x ) \in$ $J \}$ . Then $\phi ^ { - 1 } ( J )$ is connected $\mathrm { \left( w h y ? \right) }$ , and is thus an interval. Furthermore, $c J$ is the constant value of $f \circ \phi$ on $\phi ^ { - 1 } ( J ) \ \mathrm { ( w h y ? ) }$ . Thus, if we define $\mathbf { Q } : = \{ \phi ^ { - 1 } ( J ) : J \in \mathbf { P } \}$ (ignoring the fact that Q has been used to represent the rational numbers), then $\mathbf { Q }$ partitions $[ a , b ] \ \mathrm { ( w h y ? ) }$ , and $f \circ \phi$ is piecewise constant with respect to $\textbf { Q } ( \mathrm { w h y ? } )$ . Thus 

$$
\int_ {[ a, b ]} f \circ \phi d \phi = \int_ {[ \mathbf {Q} ]} f \circ \phi d \phi = \sum_ {J \in \mathbf {P}} c _ {J} \phi [ \phi^ {- 1} (J) ].
$$

But $\phi [ \phi ^ { - 1 } ( J ) ] = | J | \ ( \mathrm { w h y ? } )$ , and the claim follows. 

Proposition 11.10.6 (Change of variables formula II). Let $[ a , b ]$ be a closed interval, and let $\phi : [ a , b ]  [ \phi ( a ) , \phi ( b ) ]$ be a continuous monotone increasing function. Let $f : [ \phi ( a ) , \phi ( b ) ] \to \mathbf { R }$ be a Riemann integrable function on $[ \phi ( a ) , \phi ( b ) ]$ . Then $f \circ \phi : [ a , b ]  \mathbf { R }$ is Riemann-Stieltjes integrable with respect to φ on $[ a , b ]$ , and 

$$
\int_ {[ a, b ]} f \circ \phi d \phi = \int_ {[ \phi (a), \phi (b) ]} f.
$$

Proof. This will be obtained from Lemma 11.10.5 in a similar manner to how Corollary 11.10.3 was obtained from Theorem 11.10.2. First observe that since f is Riemann integrable, it is bounded, and then $f \circ \phi$ must also be bounded $\mathrm { ( w h y ? ) }$ 

Let $\varepsilon > 0$ . Then, we can find a piecewise constant function $\overline { { f } }$ majorizing f on $[ \phi ( a ) , \phi ( b ) ]$ , and a piecewise constant function $\underline { { f } }$ minorizing $f$ on $[ \phi ( a ) , \phi ( b ) ]$ , such that 

$$
\int_ {[ \phi (a), \phi (b) ]} f - \varepsilon \leq \int_ {[ \phi (a), \phi (b) ]} \underline {{f}} \leq \int_ {[ \phi (a), \phi (b) ]} \overline {{f}} \leq \int_ {[ \phi (a), \phi (b) ]} f + \varepsilon .
$$

Applying Lemma 11.10.5, we obtain 

$$
\int_ {[ \phi (a), \phi (b) ]} f - \varepsilon \leq \int_ {[ a, b ]} \underline {{f}} \circ \phi d \phi \leq \int_ {[ a, b ]} \overline {{f}} \circ \phi d \phi \leq \int_ {[ \phi (a), \phi (b) ]} f + \varepsilon .
$$

Since $f \circ \phi$ is piecewise constant and minorizes $f \circ \phi$ , we have 

$$
\int_ {[ a, b ]} \underline {{f}} \circ \phi d \phi \leq \int_ {\underline {{\quad [ a, b ]}}} f \circ \phi d \phi
$$

while similarly we have 

$$
\int_ {[ a, b ]} \overline {{f}} \circ \phi d \phi \geq \overline {{\int_ {[ a , b ]}}} f \circ \phi d \phi .
$$

Thus 

$$
\int_ {[ \phi (a), \phi (b) ]} f - \varepsilon \leq \underline {{\int}} _ {[ a, b ]} f \circ \phi d \phi \leq \overline {{\int}} _ {[ a, b ]} f \circ \phi d \phi \leq \int_ {[ \phi (a), \phi (b) ]} f + \varepsilon .
$$

Since $\varepsilon > 0$ was arbitrary, this implies that 

$$
\int_ {[ \phi (a), \phi (b) ]} f \leq \underline {{\int_ {[ a , b ]}}} f \circ \phi d \phi \leq \overline {{\int_ {[ a , b ]}}} f \circ \phi d \phi \leq \int_ {[ \phi (a), \phi (b) ]} f
$$

and the claim follows. 

□ 

Combining this formula with Corollary 11.10.3, one immediately obtains the following familiar formula: 

Proposition 11.10.7 (Change of variables formula III). Let $[ a , b ]$ be $a$ closed interval, and let $\phi : [ a , b ]  [ \phi ( a ) , \phi ( b ) ]$ be a diferentiable monotone increasing function such that φ is Riemann integrable. Let $f : [ \phi ( a ) , \phi ( b ) ] \to \mathbf { R }$ be a Riemann integrable function on $[ \phi ( a ) , \phi ( b ) ]$ Then $( f \circ \phi ) \phi ^ { \prime } : [ a , b ]  \mathbf { R }$ is Riemann integrable on $[ a , b ]$ , and 

$$
\int_ {[ a, b ]} (f \circ \phi) \phi^ {\prime} = \int_ {[ \phi (a), \phi (b) ]} f.
$$

— Exercises — 

Exercise 11.10.1. Prove Proposition 11.10.1. (Hint: first use Corollary 11.5.2 and Theorem 11.4.5 to show that $F G ^ { \prime }$ and $F ^ { \prime } G$ are Riemann integrable. Then use the product rule (Theorem $\mathrm { 1 0 . 1 . 1 3 ( d ) . ) }$ 

Exercise 11.10.2. Fill in the gaps marked (why?) in the proof of Lemma 11.10.5. 

Exercise 11.10.3. Let $a \ < \ b$ be real numbers, and let $f : [ a , b ]  \mathbf { R }$ be a Riemann integrable function. Let $g : [ - b , - a ]  \mathbf { R }$ be defined by $g ( x ) : =$ $f ( - x )$ . Show that $g$ is also Riemann integrable, and $\begin{array} { r } { \int _ { [ - b , - a ] } g = \int _ { [ a , b ] } f } \end{array}$ 

Exercise 11.10.4. What is the analogue of Proposition 11.10.7 when $\phi$ is monotone decreasing instead of monotone increasing? (When $\phi$ is neither monotone increasing or monotone decreasing, the situation becomes significantly more complicated.) 

## Chapter A

# Appendix: the basics of mathematical logic

The purpose of this appendix is to give a quick introduction to mathematical logic, which is the language one uses to conduct rigorous mathematical proofs. Knowing how mathematical logic works is also very helpful for understanding the mathematical way of thinking, which once mastered allows you to approach mathematical concepts and problems in a clear and confident way - including many of the proof-type questions in this text. 

Writing logically is a very useful skill. It is somewhat related to, but not the same as, writing clearly, or eficiently, or convincingly, or informatively; ideally one would want to do all of these at once, but sometimes one has to make compromises, though with practice you’l be able to achieve more of your writing objectives concurrently. Thus a logical argument may sometimes look unwieldy, excessively complicated, or otherwise appear unconvincing. The big advantage of writing logically, however, is that one can be absolutely sure that your conclusion will be correct, as long as all your hypotheses were correct and your steps were logical; using other styles of writing one can be reasonably convinced that something is true, but there is a diference between being convinced and being sure. 

Being logical is not the only desirable trait in writing, and in fact sometimes it gets in the way; mathematicians for instance often resort to short informal arguments which are not logically rigorous when they want to convince other mathematicians of a statement without going through all of the long details, and the same is true of course for nonmathematicians as well. So saying that a statement or argument is “not logical” is not necessarily a bad thing; there are often many situations when one has good reasons not to be emphatic about being logical. However, one should be aware of the distinction between logical reasoning and more informal means of argument, and not try to pass of an illogical argument as being logically rigorous. In particular, if an exercise is asking for a proof, then it is expecting you to be logical in your answer. 

Logic is a skill that needs to be learnt like any other, but this skil is also innate to all of you - indeed, you probably use the laws of logic unconsciously in your everyday speech and in your own internal (nonmathematical) reasoning. However, it does take a bit of training and practice to recognize this innate skill and to apply it to abstract situations such as those encountered in mathematical proofs. Because logic is innate, the laws of logic that you learn should make sense - if you find yourself having to memorize one of the principles or laws of logic here, without feeling a mental “click” or comprehending why that law should work, then you will probably not be able to use that law of logic correctly and efectively in practice. So, please don’t study this appendix the way you might cram before a final - that is going to be useless. Instead, put away your highlighter pen, and read and understand this appendix rather than merely studying it! 

## A.1 Mathematical statements

Any mathematical argument proceeds in a sequence of mathematical statements. These are precise statements concerning various mathematical objects (numbers, vectors, functions, etc.) and relations between them (addition, equality, diferentiation, etc.). These objects can either be constants or variables; more on this later. Statements<sup>1</sup> are either true or false. 

Example A.1.1. 2 + 2 = 4 is a true statement; 2 + 2 = 5 is a false statement. 

Not every combination of mathematical symbols is a statement. For instance, 

$$
= 2 + + 4 = - = 2
$$

is not a statement; we sometimes call it ill-formed or ill-defined. The statements in the previous example are well-formed or well-defined. Thus well-formed statements can be either true or false; ill-formed statements are considered to be neither true nor false (in fact, they are usually not considered statements at all). A more subtle example of an 

ill-formed statement is 

$$
0 / 0 = 1;
$$

division by zero is undefined, and so the above statement is ill-formed. A logical argument should not contain any ill-formed statements, thus for instance if an argument uses a statement such as $x / y = z$ , it needs to first ensure that y is not equal to zero. Many purported proofs of $\mathrm { \Delta ^ { 6 } 0 = 1 \ ' }$ or other false statements rely on overlooking this “statements must be well-formed” criterion. 

Many of you have probably written ill-formed or otherwise inaccurate statements in your mathematical work, while intending to mean some other, well-formed and accurate statement. To a certain extent this is permissible - it is similar to misspelling some words in a sentence, or using a slightly inaccurate or ungrammatical word in place of a correct one (“She ran good” instead of “She ran well”). In many cases, the reader (or grader) can detect this mis-step and correct for it. However, it looks unprofessional and suggests that you may not know what you are talking about. And if indeed you actually do not know what you are talking about, and are applying mathematical or logical rules blindly, then writing an ill-formed statement can quickly confuse you into writing more and more nonsense - usually of the sort which receives no credit in grading. So it is important, especially when just learning a subject, to take care in keeping statements well-formed and precise. Once you have more skill and confidence, of course you can aford once again to speak loosely, because you will know what you are doing and won’t be in as much danger of veering of into nonsense. 

One of the basic axioms of mathematical logic is that every wellformed statement is either true or false, but not both. (Though if there are free variables, the truth of a statement may depend on the values of these variables. More on this later.) Furthermore, the truth or falsity of a statement is intrinsic to the statement, and does not depend on the opinion of the person viewing the statement (as long as all the definitions and notations are agreed upon, of course). So to prove that a statement is true, it sufices to show that it is not false, while to show that a statement is false, it sufices to show that it is not true; this is the principle underlying the powerful technique of proof by contradiction, which we discuss later. This axiom is viable as long as one is working with precise concepts, for which the truth or falsity can be determined (at least in principle) in an objective and consistent manner. However, if one is working in very non-mathematical situations, then this axiom becomes much more dubious, and so it can be a mistake to apply mathematical logic to non-mathematical situations. (For instance, a statement such as “this rock weighs 52 pounds” is reasonably precise and objective, and so it is fairly safe to use mathematical reasoning to manipulate it, whereas vague statements such as “this rock is heavy”, “this piece of music is beautiful” or “God exists” are much more problematic. So while mathematical logic is a very useful and powerful tool, it still does have some limitations of applicability.) One can still attempt to apply logic (or principles similar to logic) in these cases (for instance, by creating a mathematical model of a real-life phenomenon), but this is now science or philosophy, not mathematics, and we will not discuss it further here. 

Remark A.1.2. There are other models of logic which attempt to deal with statements that are not definitely true or definitely false, such as modal logic, intuitionist logic, or fuzzy logic, but these are well beyond the scope of this text. 

Being true is diferent from being useful or eficient. For instance, the statement 

$$
2 = 2
$$

is true but unlikely to be very useful. The statement 

$$
4 \leq 4
$$

is also true, but not very eficient (the statement 4 = 4 is more precise). It may also be that a statement may be false yet still be useful, for instance 

$$
\pi = 2 2 / 7
$$

is false, but is still useful as a first approximation. In mathematical reasoning, we only concern ourselves with truth rather than usefulness or eficiency; the reason is that truth is objective (everybody can agree on it) and we can deduce true statements from precise rules, whereas usefulness and eficiency are to some extent matters of opinion, and do not follow precise rules. Also, even if some of the individual steps in an argument may not seem very useful or eficient, it is still possible (indeed, quite common) for the final conclusion to be quite non-trivial (i.e., not obviously true) and useful. 

Statements are diferent from expressions. Statements are true or false; expressions are a sequence of mathematical symbols which produces some mathematical object (a number, matrix, function, set, etc.) 

as its value. For instance 

$$
2 + 3 * 5
$$

is an expression, not a statement; it produces a number as its value. Meanwhile, 

$$
2 + 3 * 5 = 1 7
$$

is a statement, not an expression. Thus it does not make any sense to ask whether $2 + 3 * 5$ is true or false. As with statements, expressions can be well-defined or ill-defined; $2 + 3 / 0$ , for instance, is ill-defined. More subtle examples of ill-defined expressions arise when, for instance, attempting to add a vector to a matrix, or evaluating a function outside of its domain, e.g., $\sin ^ { - 1 } ( 2 )$ 

One can make statements out of expressions by using relations such $\mathrm { a s } = , < , \geq , \in , \subset$ etc. or by using properties (such as “is prime”, “is continuous”, “is invertible”, etc.) For instance, $^ { 6 6 } 3 0 + 5$ is prime” is a statement, as is $^ { \mathrm { 4 4 } } 3 0 + 5 \leq 4 2 - 7 ^ { \mathrm { 9 } }$ . Note that mathematical statements are allowed to contain English words. 

One can make a compound statement from more primitive statements by using logical connectives such as and, or, not, if-then, if-and-only-if, and so forth. We give some examples below, in decreasing order of intuitiveness. 

Conjunction. If X is a statement and Y is a statement, the statement $^ { 6 6 } X$ and $Y ^ { \dag }$ is true if X and $Y$ are both true, and is false otherwise. For instance, $^ { 6 6 } 2 + 2 = 4$ and $3 + 3 = 6 ^ { 3 }$ is true, while $^ { 6 6 } 2 + 2 = 4$ and $3 + 3 = 5 ^ { \mathfrak { N } }$ is not. Another example: $^ { 6 6 } 2 + 2 = 4$ and $2 + 2 = 4 ^ { \mathfrak { s } }$ is true, even if it is a bit redundant; logic is concerned with truth, not eficiency. 

Due to the expressiveness of the English language, one can reword the statement $^ { 6 6 } X$ and $Y ^ { \dag }$ in many ways, $\mathrm { e . g . , } \ ^ { 6 } X$ and also $Y ^ { \dag }$ , or “Both X and Y are true”, etc. Interestingly, the statement $^ { 6 6 } X$ , but $Y ^ { \dag }$ is logically the same statement as $^ { 6 6 } X$ and $Y ^ { \dag }$ , but they have diferent connotations (both statements afirm that X and $Y$ are both true, but the first version suggests that X and $Y$ are in contrast to each other, while the second version suggests that X and Y support each other). Again, logic is about truth, not about connotations or suggestions. 

Disjunction. If X is a statement and Y is a statement, the statement “X or $Y ^ { \dag }$ is true if either X or Y is true, or both. For instance, $^ { 6 6 } 2 + 2 = 4$ or $3 + 3 = 5 ^ { \mathfrak { N } }$ is true, but $^ { 6 6 } 2 + 2 = 5$ or $3 + 3 = 5 ^ { \mathfrak { N } }$ is not. Also $^ { 6 6 } 2 + 2 = 4$ or $3 + 3 = 6 ^ { 3 }$ is true (even if it is a bit ineficient; it would be a stronger statement to say $^ { 6 6 } 2 + 2 = 4$ and $3 + 3 = 6 ^ { 3 } )$ . Thus by default, the word $^ { 6 6 } \mathrm { o r } ^ { 9 9 }$ in mathematical logic defaults to inclusive or. The reason we do this is that with inclusive or, to verify $^ { 6 6 } X$ or $Y ^ { \dag }$ , it sufices to verify that just one of X or Y is true; we don’t need to show that the other one is false. So we know, for instance, that $^ { 6 6 } 2 + 2 = 4$ or $2 3 5 3 + 5 9 3 1 = 7 2 8 4 ^ { \mathfrak { 3 } }$ is true without having to look at the second equation. As in the previous discussion, the statement $\mathit { \Omega } ^ {  } 2 + 2 = 4 \mathrm { ~ o r ~ } 2 + 2 = 4 ^ { \prime \prime }$ is true, even if it is highly ineficient. 

If one really does want to use exclusive or, use a statement such as “Either X or Y is true, but not both” or “Exactly one of X or Y is true”. Exclusive or does come up in mathematics, but nowhere near as often as inclusive or. 

Negation. The statement “X is not true” or “X is false”, or $^ { 6 6 } \mathrm { { I t } }$ is not the case that $X ^ { \dag }$ , is called the negation of X, and is true if and only if X is false, and is false if and only if X is true. For instance, the statement “It is not the case that $2 + 2 = 5 ^ { , }$ is a true statement. Of course we could abbreviate this statement to $^ { 6 6 } 2 + 2 \neq 5 ^ { , }$ 

Negations convert “and” into “or”. For instance, the negation of “Jane Doe has black hair and Jane Doe has blue eyes” is “Jane Doe doesn’t have black hair or doesn’t have blue eyes”, not “Jane Doe doesn’t have black hair and doesn’t have blue eyes” (can you see why?). Similarly, if x is an integer, the negation of $^ { 6 6 } x$ is even and non-negative” is “x is odd or negative”, not $^ { 6 6 } x$ is odd and negative”. (Note how it is important here that or is inclusive rather than exclusive.) Or the negation of $^ { \ast } x \geq 2$ and $x \le 6 ^ { \ ' } \ ( \mathrm { i . e . , \ } ^ { \thickspace } 2 \le x \le 6 ^ { \ ' } )$ is $^ { 6 } x < 2$ or $x > 6 ^ { \mathfrak { g } }$ , not $^ { 6 } x < 2$ and $x > 6 ^ { \mathfrak { g } }$ or $^ { 6 6 } 2 < x > 6 . ^ { 9 9 }$ 

Similarly, negations convert “or” into “and”. The negation of “John Doe has brown hair or black hair” is “John Doe does not have brown hair and does not have black hair”, or equivalently “John Doe has neither brown nor black hair”. If x is a real number, the negation of $^ { 6 } x \geq 1$ or $x \leq - 1 ^ { \mathfrak { N } } { \mathrm { ~ i s ~ } } ^ { \mathfrak { Q } } x < 1$ and $x > - 1 ^ { \mathfrak { P } } \ ( { \mathrm { i . e . , } } - 1 < x < 1 )$ 

It is quite possible that a negation of a statement will produce a statement which could not possibly be true. For instance, if x is an integer, the negation of $^ { 6 6 } x$ is either even or odd” is $^ { 6 6 } x$ is neither even nor odd”, which cannot possibly be true. Remember, though, that even if a statement is false, it is still a statement, and it is definitely possible to arrive at a true statement using an argument which at times involves false statements. (Proofs by contradiction, for instance, fall into this category. Another example is proof by dividing into cases. If one divides into three mutually exclusive cases, Case 1, Case 2, and Case 3, then at any given time two of the cases will be false and only one will be true, however this does not necessarily mean that the proof as a whole is incorrect or that the conclusion is false.) 

Negations are sometimes unintuitive to work with, especially if there are multiple negations; a statement such as “It is not the case that either x is not odd, or x is not larger than or equal to 3, but not both” is not particularly pleasant to use. Fortunately, one rarely has to work with more than one or two negations at a time, since often negations cancel each other. For instance, the negation of “X is not true” is just “X is true”, or more succinctly just $^ { 6 6 } X ^ { 9 9 }$ . Of course one should be careful when negating more complicated expressions because of the switching of “and” and “or”, and similar issues. 

If and only if (if). If X is a statement, and Y is a statement, we say that “X is true if and only if Y is true”, whenever X is true, Y has to be also, and whenever Y is true, X has to be also (i.e., X and Y are “equally true”). Other ways of saying the same thing are “X and Y are logically equivalent statements”, or “X is true if Y is true”, or $^ { 6 6 } X  Y ^ { 5 9 }$ . Thus for instance, if x is a real number, then the statement $^ { 6 } x = 3$ if and only if $2 x = 6 ^ { \mathfrak { s } }$ is true: this means that whenever x = 3 is true, then $2 x = 6$ is true, and whenever $2 x = 6$ is true, then x = 3 is true. On the other hand, the statement $^ { 6 } x = 3$ if and only if $x ^ { 2 } = 9 "$ is false; while it is true that whenever x = 3 is true, $x ^ { 2 } = 9$ is also true, it is not the case that whenever $x ^ { 2 } = 9$ is true, that $x = 3$ is also automatically true (think of what happens when $x = - 3 )$ 

Statements that are equally true, are also equally false: if X and Y are logically equivalent, and X is false, then Y has to be false also (because if Y were true, then X would also have to be true). Conversely, any two statements which are equally false will also be logically equivalent. Thus for instance $2 + 2 = 5$ if and only if $4 + 4 = 1 0$ 

Sometimes it is of interest to show that more than two statements are logically equivalent; for instance, one might want to assert that three statements X, Y, and Z are all logically equivalent. This means whenever one of the statements is true, then all of the statements are true; and it also means that if one of the statements is false, then all of the statements are false. This may seem like a lot of logical implications to prove, but in practice, once one demonstrates enough logical implications between X, Y, and Z, one can often conclude all the others and conclude that they are all logicallly equivalent. See for instance Exercises A.1.5, A.1.6. 

— Exercises — 

Exercise A.1.1. What is the negation of the statement “either X is true, or Y is true, but not both”? 

Exercise A.1.2. What is the negation of the statement “X is true if and only if Y is true”? (There may be multiple ways to phrase this negation). 

Exercise A.1.3. Suppose that you have shown that whenever X is true, then Y is true, and whenever X is false, then Y is false. Have you now demonstrated that X and Y are logically equivalent? Explain. 

Exercise A.1.4. Suppose that you have shown that whenever X is true, then Y is true, and whenever Y is false, then X is false. Have you now demonstrated that X is true if and only if Y is true? Explain. 

Exercise A.1.5. Suppose you know that X is true if and only if Y is true, and you know that Y is true if and only if Z is true. Is this enough to show that $X , Y , Z$ are all logically equivalent? Explain. 

Exercise A.1.6. Suppose you know that whenever X is true, then Y is true; that whenever Y is true, then Z is true; and whenever Z is true, then X is true. Is this enough to show that X, Y, Z are all logically equivalent? Explain. 

## A.2 Implication

Now we come to the least intuitive of the commonly used logical connectives - implication. If X is a statement, and Y is a statement, then “if X, then $Y ^ { \dag }$ is the implication from X to Y; it is also written “when X is true, Y is true”, or “X implies $Y ^ { \dag }$ or $^ { 6 6 } Y$ is true when $X \ \mathrm { i s } ^ { \mathrm { \prime \prime } }$ or $^ { 6 6 } X$ is true only if Y is true” (this last one takes a bit of mental efort to see). What this statement “if X, then $Y ^ { \dag }$ means depends on whether X is true or false. If X is true, then “if X, then $Y ^ { \mathfrak { s } }$ is true when $Y$ is true, and false when $Y$ is false. If however X is false, then “if X, then $Y ^ { \dag }$ is always true, regardless of whether Y is true or false! To put it another way, when X is true, the statement “if X, then $Y ^ { \dag }$ implies that Y is true. But when X is false, the statement “if X, then $Y ^ { \dag }$ ofers no information about whether Y is true or not; the statement is true, but vacuous (i.e., does not convey any new information beyond the fact that the hypothesis is false). 

Examples A.2.1. If x is an integer, then the statement “If x = 2, then $x ^ { 2 } = 4 "$ is true, regardless of whether x is actually equal to 2 or not (though this statement is only likely to be useful when x is equal to 2). This statement does not assert that x is equal to 2, and does not assert that $x ^ { 2 }$ is equal to 4, but it does assert that when and if x is equal to 2, 

## A.2. Implication

then $x ^ { 2 }$ is equal to 4. If x is not equal to 2, the statement is still true but ofers no conclusion on x or $x ^ { 2 }$ 

Some special cases of the above implication: the implication ${ } ^ { 6 } \mathrm { f f ~ 2 = }$ 2, then $2 ^ { 2 } = 4 ^ { \prime \prime }$ is true (true implies true). The implication ${ } ^ { 6 6 } \mathrm { I f } \ 3 = 2$ then $3 ^ { 2 } = 4 "$ is true (false implies false). The implication ${ } ^ { 6 } \mathrm { f f } - 2 = 2$ then $( - 2 ) ^ { 2 } = 4 ^ { \mathfrak { n } }$ is true (false implies true). The latter two implications are considered vacuous - they do not ofer any new information since their hypothesis is false. (Nevertheless, it is still possible to employ vacuous implications to good efect in a proof - a vacously true statement is still true. We shall see one such example shortly.) 

As we see, the falsity of the hypothesis does not destroy the truth of an implication, in fact it is just the opposite! (When a hypothesis is false, the implication is automatically true.) The only way to disprove an implication is to show that the hypothesis is true while the conclusion is false. Thus $\scriptscriptstyle { ^ { 6 4 } \mathrm { I f } ~ 2 + 2 } = 4$ , then $4 + 4 = 2 "$ is a false implication. (True does not imply false.) 

One can also think of the statement “if X, then $Y ^ { \dag }$ as $^ { 6 6 } Y$ is at least as true as $X ^ { \mathfrak { N } } \mathfrak { - } \mathrm { i f } \ X$ is true, then Y also has to be true, but if X is false, Y could be as false as X, but it could also be true. This should be compared with $^ { 6 6 } X$ if and only if $Y ^ { \dag }$ , which asserts that X and $Y$ are equally true. 

Vacuously true implications are often used in ordinary speech, sometimes without knowing that the implication is vacuous. A somewhat frivolous example is “If wishes were wings, then pigs would $\mathrm { { f l y } ^ { \mathrm { { \ ' } } } }$ . (The statement “hell freezes over” is also a popular choice for a false hypothesis.) A more serious one is “If John had left work at 5pm, then he would be here by now.” This kind of statement is often used in a situation in which the conclusion and hypothesis are both false; but the implication is still true regardless. This statement, by the way, can be used to illustrate the technique of proof by contradiction: if you believe that “If John had left work at 5pm, then he would be here by now”, and you also know that “John is not here by now”, then you can conclude that “John did not leave work at 5pm”, because John leaving work at 5pm would lead to a contradiction. Note how a vacuous implication can be used to derive a useful truth. 

To summarize, implications are sometimes vacuous, but this is not actually a problem in logic, since these implications are still true, and vacuous implications can still be useful in logical arguments. In particular, one can safely use statements like “If X, then $Y ^ { \dag }$ without necessarily having to worry about whether the hypothesis X is actually true or not (i.e., whether the implication is vacuous or not). 

Implications can also be true even when there is no causal link between the hypothesis and conclusion. The statement $^ { 6 } \mathrm { T f } 1 + 1 = 2$ , then Washington D.C. is the capital of the United States” is true (true implies true), although rather odd; the statement $\scriptscriptstyle \mathrm { ~ \sp { 6 6 } I f ~ 2 + 2 = 3 ~ }$ , then New York is the capital of the United States” is similarly true (false implies false). Of course, such a statement may be unstable (the capital of the United States may one day change, while 1 + 1 will always remain equal to 2) but it is true, at least for the moment. While it is possible to use acausal implications in a logical argument, it is not recommended as it can cause unneeded confusion. (Thus, for instance, while it is true that a false statement can be used to imply any other statement, true or false, doing so arbitrarily would probably not be helpful to the reader.) 

To prove an implication “If X, then Y”, the usual way to do this is to first assume that X is true, and use this (together with whatever other facts and hypotheses you have) to deduce Y. This is still a valid procedure even if X later turns out to be false; the implication does not guarantee anything about the truth of X, and only guarantees the truth of Y conditionally on X first being true. For instance, the following is a valid proof of a true proposition, even though both hypothesis and conclusion of the proposition are false: 

Proposition A.2.2. If $2 + 2 = 5 , t h e n 4 = 1 0 - 4 .$ 

Proof. Assume $2 + 2 = 5$ . Multiplying both sides by 2, we obtain $4 + 4 =$ 10. Subtracting 4 from both sides, we obtain $4 = 1 0 - 4$ as desired. 

On the other hand, a common error is to prove an implication by first assuming the conclusion and then arriving at the hypothesis. For instance, the following Proposition is correct, but the proof is not: 

Proposition A.2.3. Suppose that $2 x + 3 = 7$ . Show that $x = 2$ 

Proof. (Incorrect) x = 2; so 2x = 4; so 2x + 3 = 7. 

When doing proofs, it is important that you are able to distinguish the hypothesis from the conclusion; there is a danger of getting hopelessly confused if this distinction is not clear. 

Here is a short proof which uses implications which are possibly vacuous. 

Theorem A.2.4. Suppose that n is an integer. Then $n ( n + 1 )$ is an even integer. 

Proof. Since n is an integer, n is even or odd. If n is even, then $n ( n + 1 )$ is also even, since any multiple of an even number is even. If n is odd, then $n + 1$ is even, which again implies that $n ( n + 1 )$ is even. Thus in either case $n ( n + 1 )$ is even, and we are done. □ 

Note that this proof relied on two implications: “if n is even, then $n ( n + 1 )$ is $\mathrm { e v e n } ^ { \mathfrak { N } }$ , and “if n is odd, then $n ( n + 1 )$ is even”. Since n cannot be both odd and even, at least one of these implications has a false hypothesis and is therefore vacuous. Nevertheless, both these implications are true, and one needs both of them in order to prove the theorem, because we don’t know in advance whether n is even or odd. And even if we did, it might not be worth the trouble to check it. For instance, as a special case of this theorem we immediately know 

Corollary A.2.5. Let $n = ( 2 5 3 + 1 4 2 ) * 1 2 3 - ( 4 2 3 + 1 9 8 ) ^ { 3 4 2 } + 5 3 8 - 2 1 3 .$ Then $n ( n + 1 )$ is an even integer. 

In this particular case, one can work out exactly which parity n is - even or odd - and then use only one of the two implications in the above Theorem, discarding the vacuous one. This may seem like it is more eficient, but it is a false economy, because one then has to determine what parity n is, and this requires a bit of efort - more efort than it would take if we had just left both implications, including the vacuous one, in the argument. So, somewhat paradoxically, the inclusion of vacuous, false, or otherwise “useless” statements in an argument can actually save you efort in the long run! (I’m not suggesting, of course, that you ought to pack your proofs with lots of time-wasting and irrelevant statements; all I’m saying here is that you need not be unduly concerned that some hypotheses in your argument might not be correct, as long as your argument is still structured to give the correct conclusion regardless of whether those hypotheses were true or false.) 

The statement “If X, then $Y ^ { \dag }$ is not the same as “If Y, then $X ^ { \dag }$ ; for instance, while $^ { \mathrm { ~ 6 ~ } } \mathrm { I f } \ x = 2$ , then $x ^ { 2 } = 4 "$ is true, “If $x ^ { 2 } = 4$ , then $x = 2 ^ { \mathfrak { g } }$ can be false if x is equal to 2. These two statements are called converses of each other; thus the converse of a true implication is not necessarily another true implication. We use the statement “X if and only if $Y ^ { \dag }$ to denote the statement that “If X, then $Y ;$ and if Y, then $X ^ { \dag }$ . Thus for instance, we can say that $x = 2$ if and only if $2 x = 4$ , because if $x = 2$ then $2 x = 4$ , while if $2 x = 4$ then $x = 2$ . One way of thinking about an if-and-only-if statement is to view “X if and only if $Y ^ { \dag }$ as saying that X is just as true as $Y ;$ if one is true then so is the other, and if one is false, then so is the other. For instance, the statement $\mathrm { ^ 6 4 } \mathrm { ~ f ~ f ~ 3 ~ = ~ 2 ~ }$ , then $6 = 4 ^ { \mathfrak { s } }$ is true, since both hypothesis and conclusion are false. (Under this view, “If X, then $Y ^ { \dag }$ can be viewed as a statement that Y is at least as true as X.) Thus one could say “X and Y are equally true” instead of “X if and only if $Y ^ { \dag }$ 

Similarly, the statement “If X is true, then Y is true” is not the same as “If X is false, then Y is false”. Saying that ${ \mathfrak { s e } } _ { \mathrm { i f } } \ { \boldsymbol { x } } = \ 2$ , then $x ^ { 2 } = 4 "$ does not imply that “if $x \neq 2$ , then $x ^ { 2 } \neq 4 ^ { , }$ , and indeed we have $x = - 2$ as a counterexample in this case. If-then statements are not the same as if-and-only-if statements. (If we knew that “X is true if and only if Y is true”, then we would also know that “X is false if and only if Y is false”.) The statement “If X is false, then Y is false” is sometimes called the inverse of “If X is true, then Y is true”; thus the inverse of a true implication is not necessarily a true implication. 

If you know that “If X is true, then Y is true”, then it is also true that “If Y is false, then X is false” (because if Y is false, then X can’t be true, since that would imply Y is true, a contradiction). For instance, if we knew that “If $x = 2$ , then $x ^ { 2 } = 4 "$ , then we also know that “If $x ^ { 2 } \neq 4$ , then $x \ne 2 ^ { \mathfrak { r } }$ . Or if we knew “If John had left work at 5pm, he would be here by now”, then we also know “If John isn’t here now, then he could not have left work at 5pm”. The statement “If Y is false, then X is false” is known as the contrapositive of “If X, then $Y ^ { \dag }$ and both statements are equally true. 

In particular, if you know that X implies something which is known to be false, then X itself must be false. This is the idea behind proof by contradiction or reductio ad absurdum: to show something must be false, assume first that it is true, and show that this implies something which you know to be false (e.g., that a statement is simultaneously true and not true). For instance: 

Proposition A.2.6. Suppose that x be a positive number such that sin(x) = 1. Then $x \ge \pi / 2$ 

Proof. Suppose for sake of contradiction that $x \ < \ \pi / 2$ . Since x is positive, we thus have $0 < x < \pi / 2$ Since sin(x) is increasing for $0 ~ < ~ x ~ < ~ \pi / 2$ , and sin $( 0 ) ~ = ~ 0$ and sin $( \pi / 2 ) ~ = ~ 1$ , we thus have $0 < \sin ( x ) < 1$ . But this contradicts the hypothesis that sin $( x ) = 1$ Hence $x \ge \pi / 2$ □ 

## A.3. The structure of proofs

Note that one feature of proof by contradiction is that at some point in the proof you assume a hypothesis (in this case, that $x < \pi / 2 )$ which later turns out to be false. Note however that this does not alter the fact that the argument remains valid, and that the conclusion is true; this is because the ultimate conclusion does not rely on that hypothesis being true (indeed, it relies instead on it being false!). 

Proof by contradiction is particularly useful for showing “negative” statements - that X is false, that a is not equal to b, that kind of thing. But the line between positive and negative statements is sort of blurry. (Is the statement $x \ge 2$ a positive or negative statement? What about its negation, that $x < 2 ? )$ So this is not a hard and fast rule. 

Logicians often use special symbols to denote logical connectives; for instance $^ { 6 6 } X$ implies $Y ^ { \dag }$ can be written $^ {  } X \implies Y ^ {  }$ , “X is not true” can be written ${ } ^ { \mathfrak { a } } \sim X ^ { \mathfrak { n } } , { } ^ { \mathfrak { a } } ! X ^ { \mathfrak { n } } , \mathrm { o r } \ { } ^ { \mathfrak { a } } \neg X ^ { \mathfrak { n } }$ , “X and $Y ^ { \dag }$ can be written $^ { 6 6 } X \wedge Y ^ { 5 }$ or $^ { 6 6 } X \& Y ^ { 9 }$ , and so forth. But for general-purpose mathematics, these symbols are not often used; English words are often more readable, and don’t take up much more space. Also, using these symbols tends to blur the line between expressions and statements; it’s not as easy to understand ${ } ^ { \mathfrak { c } } ( ( x = 3 ) \wedge ( y = 5 ) ) \implies ( x + y = 8 ) ^ { \mathfrak { n } }$ as $\mathrm { { ^ 6 4 } I f } \ x = 3$ and $y = 5$ , then $x + y = 8 ^ { \prime \prime }$ . So in general I would not recommend using these symbols (except possibly for $\Longrightarrow$ , which is a very intuitive symbol). 

## A.3 The structure of proofs

To prove a statement, one often starts by assuming the hypothesis and working one’s way toward a conclusion; this is the direct approach to proving a statement. Such a proof might look something like the following: 

## Proposition A.3.1. A implies B.

Proof. Assume A is true. Since A is true, C is true. Since C is true, D is true. Since D is true, B is true, as desired. □ 

An example of such a direct approach is 

Proposition A.3.2. If $x = \pi$ , then sin $( x / 2 ) + 1 = 2$ 

Proof. Let $x = \pi$ . Since $x = \pi$ , we have $x / 2 = \pi / 2$ . Since $x / 2 = \pi / 2$ 4 we have sin $( x / 2 ) = 1$ . Since sin $( x / 2 ) = 1$ , we have sin $( x / 2 ) + 1 = 2$ □ 

In the above proof, we started at the hypothesis and moved steadily from there toward a conclusion. It is also possible to work backwards from the conclusion and seeing what it would take to imply it. For instance, a typical proof of Proposition A.3.1 of this sort might look like the following: 

Proof. To show B, it would sufice to show D. Since C implies D, we just need to show C. But C follows from A. □ 

As an example of this, we give another proof of Proposition A.3.2: 

Proof. To show sin $( x / 2 ) + 1 = 2$ , it would sufice to show that sin $( x / 2 ) =$ 1. Since $x / 2 = \pi / 2$ would imply sin $( x / 2 ) = 1$ , we just need to show that $x / 2 = \pi / 2$ . But this follows since $x = \pi$ □ 

Logically speaking, the above two proofs of Proposition A.3.2 are the same, just arranged diferently. Note how this proof style is diferent from the (incorrect) approach of starting with the conclusion and seeing what it would imply (as in Proposition A.2.3); instead, we start with the conclusion and see what would imply it. 

Another example of a proof written in this backwards style is the following: 

Proposition A.3.3. Let $0 < r < 1$ be a real number. Then the series $\textstyle \sum _ { n = 1 } ^ { \infty } n r ^ { n }$ is convergent. 

Proof. To show this series is convergent, it sufices by the ratio test to show that the ratio 

$$
\left| \frac {r ^ {n + 1} (n + 1)}{r ^ {n} n} \right| = r \frac {n + 1}{n}
$$

 converges to something less than 1 as $n  \infty$ . Since r is already less than 1, it will be enough to show that $\textstyle { \frac { n + 1 } { n } }$ converges to 1. But since $\textstyle { \frac { n + 1 } { n } } \ = 1 + { \frac { 1 } { n } }$ , it sufices to show that $\textstyle { \frac { 1 } { n } } \to 0$ . But this is clear since $n \to \infty$ □ 

One could also do any combination of moving forwards from the hypothesis and backwards from the conclusion. For instance, the following would be a valid proof of Proposition A.3.1: 

Proof. To show B, it would sufice to show D. So now let us show $D$ Since we have A by hypothesis, we have C. Since C implies D, we thus have D as desired. □ 

Again, from a logical point of view this is exactly the same proof as before. Thus there are many ways to write the same proof down; how you do so is up to you, but certain ways of writing proofs are more readable and natural than others, and diferent arrangements tend to emphasize diferent parts of the argument. (Of course, when you are just starting out doing mathematical proofs, you’re generally happy to get some proof of a result, and don’t care so much about getting the “best” arrangement of that proof; but the point here is that a proof can take many diferent forms.) 

The above proofs were pretty simple because there was just one hypothesis and one conclusion. When there are multiple hypotheses and conclusions, and the proof splits into cases, then proofs can get more complicated. For instance a proof might look as tortuous as this: 

Proposition A.3.4. Suppose that A and B are true. Then C and D are true. 

Proof. Since A is true, E is true. From E and B we know that F is true. Also, in light of A, to show D it sufices to show G. There are now two cases: H and I. If H is true, then from F and H we obtain C, and from A and H we obtain G. If instead I is true, then from I we have G, and from I and G we obtain C. Thus in both cases we obtain both C and G, and hence C and D. □ 

Incidentally, the above proof could be rearranged into a much tidier manner, but you at least get the idea of how complicated a proof could become. To show an implication there are several ways to proceed: you can work forward from the hypothesis; you can work backward from the conclusion; or you can divide into cases in the hope to split the problem into several easier sub-problems. Another is to argue by contradiction, for instance you can have an argument of the form 

## Proposition A.3.5. Suppose that A is true. Then B is false.

Proof. Suppose for sake of contradiction that B is true. This would imply that C is true. But since A is true, this implies that D is true; which contradicts C. Thus B must be false. □ 

As you can see, there are several things to try when attempting a proof. With experience, it will become clearer which approaches are likely to work easily, which ones will probably work but require much efort, and which ones are probably going to fail. In many cases there is really only one obvious way to proceed. Of course, there may definitely be multiple ways to approach a problem, so if you see more than one way to begin a problem, you can just try whichever one looks the easiest, but be prepared to switch to another approach if it begins to look hopeless. 

Also, it helps when doing a proof to keep track of which statements are known (either as hypotheses, or deduced from the hypotheses, or coming from other theorems and results), and which statements are desired (either the conclusion, or something which would imply the conclusion, or some intermediate claim or lemma which will be useful in eventually obtaining the conclusion). Mixing the two up is almost always a bad idea, and can lead to one getting hopelessly lost in a proof. 

## A.4 Variables and quantifiers

One can get quite far in logic just by starting with primitive statements (such as $^ { 6 6 } 2 + 2 = 4 ^ { 5 }$ or “John has black hair”), then forming compound statements using logical connectives, and then using various laws of logic to pass from one’s hypotheses to one’s conclusions; this is known as propositional logic or Boolean logic. (It is possible to list a dozen or so such laws of propositional logic, which are suficient to do everything one wants to do, but I have deliberately chosen not to do so here, because you might then be tempted to memorize that list, and that is not how one should learn how to do logic, unless one happens to be a computer or some other non-thinking device. However, if you really are curious as to what the formal laws of logic are, look up “laws of propositional logic” or something similar in the library or on the internet.) 

However, to do mathematics, this level of logic is insuficient, because it does not incorporate the fundamental concept of variables - those familiar symbols such as x or n which denote various quantities which are unknown, or set to some value, or assumed to obey some property. Indeed we have already sneaked in some of these variables in order to illustrate some of the concepts in propositional logic (mainly because it gets boring after a while to talk endlessly about variable-free statements such as $2 + 2 = 4 { \mathrm { ~ o r } }$ “Jane has black hair”). Mathematical logic is thus the same as propositional logic but with the additional ingredient of variables added. 

A variable is a symbol, such as n or x, which denotes a certain type of mathematical object - an integer, a vector, a matrix, that kind of thing. In almost all circumstances, the type of object that the variable represents should be declared, otherwise it will be dificult to make wellformed statements using it. (There are very few true statements that one can make about variables without knowing the type of variables involved. For instance, given a variable x of any type whatsoever, it is true that $x = x$ , and if we also know that $x = y$ , then we can conclude that $y = x$ . But one cannot say, for instance, that $x + y = y + x$ , until we know what type of objects x and y are and whether they support the operation of addition; for instance, the above statement is ill-formed if x is a matrix and y is a vector. Thus if one actually wants to do some useful mathematics, then every variable should have an explicit type.) 

One can form expressions and statements involving variables, for instance, if x is a real variable (i.e., a variable which is a real number), $x + 3$ is an expression, and $x + 3 = 5$ is a statement. But now the truth of a statement may depend on the value of the variables involved; for instance the statement $x + 3 = 5$ is true if x is equal to 2, but is false if x is not equal to 2. Thus the truth of a statement involving a variable may depend on the context of the statement - in this case, it depends on what x is supposed to be. (This is a modification of the rule for propositional logic, in which all statements have a definite truth value.) 

Sometimes we do not set a variable to be anything (other than specifying its type). Thus, we could consider the statement $x + 3 = 5$ where x is an unspecified real number. In such a case we call this variable a free variable; thus we are considering $x + 3 = 5$ with x a free variable. Statements with free variables might not have a definite truth value, as they depend on an unspecified variable. For instance, we have already remarked that $x + 3 = 5$ does not have a definite truth value if x is a free real variable, though of course for each given value of x the statement is either true or false. On the other hand, the statement $( x + 1 ) ^ { 2 } = x ^ { 2 } + 2 x + 1$ is true for every real number x, and so we can regard this as a true statement even when x is a free variable. 

At other times, we set a variable to equal a fixed value, by using a statement such as “Let $x = 2 ^ { \mathfrak { g } }$ or “Set x equal to $2 ^ { \mathfrak { g } }$ . In this case, the variable is known as a bound variable, and statements involving only bound variables and no free variables do have a definite truth value. For instance, if we set $x = 3 4 2$ , then the statement ${ } ^ { 4 4 } x + 1 3 5 = 4 7 7 { } ^ { 3 }$ now has a definite truth value, whereas if x is a free real variable then ${ } ^ { 4 } x + 1 3 5 = 4 7 7 { } ^ { 3 }$ could be either true or false, depending on what x is. Thus, as we have said before, the truth of a statement such as ${ } ^ { 4 5 } x + 1 3 5 = 4 7 7 { } ^ { 3 5 }$ depends on the context - whether x is free or bound, and if it is bound, what it is bound to. 

One can also turn a free variable into a bound variable by using the quantifiers “for $\mathrm { a l l } ^ { \dag }$ or “for some”. For instance, the statement 

$$
(x + 1) ^ {2} = x ^ {2} + 2 x + 1
$$

is a statement with one free variable x, and need not have a definite truth value, but the statement 

$$
(x + 1) ^ {2} = x ^ {2} + 2 x + 1 \mathrm{forallrealnumbers} x
$$

is a statement with one bound variable x, and now has a definite truth value (in this case, the statement is true). Similarly, the statement 

$$
x + 3 = 5
$$

has one free variable, and does not have a definite truth value, but the statement 

$$
x + 3 = 5 \mathrm{forsomerealnumber} x
$$

is true, since it is true for $x = 2$ . On the other hand, the statement 

$$
x + 3 = 5 \mathrm{forallrealnumbers} x
$$

is false, because there are some (indeed, there are many) real numbers x for which $x + 3$ is not equal to 5. 

Universal quantifiers. Let $P ( x )$ be some statement depending on a free variable x. The statement ${ } ^ { 6 6 } P ( x )$ is true for all x of type $T ^ { \mathfrak { s } }$ means that given any x of type $T ,$ the statement $P ( x )$ is true regardless of what the exact value of x is. In other words, the statement is the same as saying “if x is of type $T$ , then $P ( x )$ is true”. Thus the usual way to prove such a statement is to let x be a free variable of type $T$ (by saying something like “Let x be any object of type $T ^ { \dag } )$ , and then proving $P ( x )$ for that object. The statement becomes false if one can produce even a single counterexample, i.e., an element x which lies in $T$ but for which $P ( x )$ is false. For instance, the statement $^ { 6 6 } x ^ { 2 }$ is greater than $x$ for all positive $x '$ can be shown to be false by producing a single example, such as $x = 1$ or $x = 1 / 2$ , where $x ^ { 2 }$ is not greater than x. 

On the other hand, producing a single example where $P ( x )$ is true will not show that $P ( x )$ is true for all x. For instance, just because the equation $x + 3 = 5$ has a solution when $x = 2$ does not imply that $x + 3 = 5$ for all real numbers $x ;$ it only shows that $x + 3 = 5$ is true for some real number x. (This is the source of the often-quoted, though somewhat inaccurate, slogan “One cannot prove a statement just by giving an example”. The more precise statement is that one cannot prove a “for all” statement by examples, though one can certainly prove “for some” statements this way, and one can also disprove “for $\mathrm { a l l } ^ { \dag }$ statements by a single counterexample.) 

It occasionally happens that there are in fact no variables x of type T. In that case the statement ${ } ^ { \ 6 } P ( x )$ is true for all x of type $T ^ { \mathfrak { s } }$ is vacuously true - it is true but has no content, similar to a vacuous implication. For instance, the statement 

$$
6 <   2 x <   4 \mathrm{forall} 3 <   x <   2
$$

is true, and easily proven, but is vacuous. (Such a vacuously true statement can still be useful in an argument, though this doesn’t happen very often.) 

One can use phrases such as “For every” or “For each” instead of “For all”, e.g., one can rephrase $\ ^ { \mathfrak { s } } ( x + 1 ) ^ { 2 } = x ^ { 2 } + 2 x + 1$ for all real numbers $x '$ as ${ } ^ { 6 6 } \mathrm { F o r }$ each real number $x , ( x + 1 ) ^ { 2 }$ is equal to $x ^ { 2 } + 2 x + 1 ^ { \mathfrak { n } }$ For the purposes of logic these rephrasings are equivalent. The symbol $\forall$ can be used instead of “For all”, thus for instance ${ } ^ { \mathfrak { s e } } \forall x \in X : P ( x )$ is true” or ${ } ^ { \ 6 \cdot } P ( x )$ is true $\forall x \in X ^ { \prime }$ is synonymous with ${ } ^ { \ 6 } P ( x )$ is true for all $x \in X ^ { \prime }$ 

Existential quantifiers. The statement ${ } ^ { \ 6 } P ( x )$ is true for some x of type $T ^ { \mathfrak { s } }$ means that there exists at least one x of type $T$ for which $P ( x )$ is true, although it may be that there is more than one such x. (One would use a quantifier such as “for exactly one $x '$ instead of “for some $x '$ if one wanted both existence and uniqueness of such an $x . )$ To prove such a statement it sufices to provide a single example of such an x. For instance, to show that 

$$
x ^ {2} + 2 x - 8 = 0 \mathrm{forsomerealnumber} x
$$

all one needs to do is find a single real number x for which $x ^ { 2 } + 2 x - 8 = 0$ for instance $x \ = \ 2$ will do. (One could also use $x \ = \ - 4$ , but one doesn’t need to use both.) Note that one has the freedom to select x to be anything one wants when proving a for-some statement; this is in contrast to proving a for-all statement, where one has to let x be arbitrary. (One can compare the two statements by thinking of two games between you and an opponent. In the first game, the opponent gets to pick what x is, and then you have to prove $P ( x )$ ; if you can always win this game, then you have proven that $P ( x )$ is true for all x. In the second game, you get to choose what x is, and then you prove $P ( x )$ ; if you can win this game, you have proven that $P ( x )$ is true for some x.) 

Usually, saying something is true for all x is much stronger than just saying it is true for some x. There is one exception though, if the condition on x is impossible to satisfy, then the for-all statement is vacuously true, but the for-some statement is false. For instance 

$$
6 <   2 x <   4 \mathrm{forall} 3 <   x <   2
$$

is true, but 

$$
6 <   2 x <   4 \mathrm{forsome} 3 <   x <   2
$$

is false. 

One can use phrases such as “For at least one” or “There exists . . . such that” instead of “For some”. For instance, one can rephrase $\begin{array} { r } { \ddot { } x ^ { 2 } + 2 x - 8 = 0 } \end{array}$ for some real number $x '$ as “There exists a real number x such that $x ^ { 2 } + 2 x - 8 = 0 ^ { , , }$ . The symbol can be used instead of “There exists . . . such that”, thus for instance $\ast \exists x \in X : P ( x )$ is true” is synonymous with ${ } ^ { \mathfrak { s } } P ( x )$ is true for some $x \in X ^ { \prime }$ 

## A.5 Nested quantifiers

One can nest two or more quantifiers together. For instance, consider the statement 

$$
\mathrm{Foreachverypositivenumber} x, \mathrm{thereexistsa}
$$

$$
\text { positive   number } y \text { such   that } y ^ {2} = x.
$$

What does this statement mean? It means that for each positive number x, the statement 

There exists a positive number y such that $y ^ { 2 } = x$ 

is true. In other words, one can find a positive square root of x for each positive number x. So the statement is saying that every positive number has a positive square root. 

To continue the gaming metaphor, suppose you play a game where your opponent first picks a positive number x, and then you pick a positive number y. You win the game if $y ^ { 2 } = x$ . If you can always win the game regardless of what your opponent does, then you have proven that for every positive x, there exists a positive y such that $y ^ { 2 } = x$ 

Negating a universal statement produces an existential statement. The negation of $^ { 6 6 } \mathrm { A l l }$ swans are white” is not “All swans are not white”, but rather “There is some swan which is not white”. Similarly, the negation of “For every $0 < x < \pi / 2$ , we have $\cos ( x ) \geq 0 ^ { \mathfrak { n } }$ is “For some $0 < x < \pi / 2$ , we have cos $( x ) < 0$ , not “For every $0 < x < \pi / 2$ , we have cos $( x ) < 0 ^ { \mathfrak { n } }$ 

Negating an existential statement produces a universal statement. The negation of “There exists a black swan” is not “There exists a swan which is non-black”, but rather “All swans are non-black”. Similarly, the negation of “There exists a real number x such that $x ^ { 2 } + x + 1 = 0 ^ { , }$ is “For every real number x, $x ^ { 2 } + x + 1 \neq 0 ^ { , }$ , not “There exists a real number x such that $x ^ { 2 } + x + 1 \neq 0 ^ { , }$ . (The situation here is very similar to how “and” and $^ { 6 6 } \mathrm { o r } ^ { 9 9 }$ behave with respect to negations.) 

If you know that a statement $P ( x )$ is true for all x, then you can set x to be anything you want, and $P ( x )$ will be true for that value of x; this is what “for all” means. Thus for instance if you know that 

$$
(x + 1) ^ {2} = x ^ {2} + 2 x + 1 \text { for   all   real   numbers } x,
$$

then you can conclude for instance that 

$$
(\pi + 1) ^ {2} = \pi^ {2} + 2 \pi + 1,
$$

or for instance that 

$$
(\cos (y) + 1) ^ {2} = \cos (y) ^ {2} + 2 \cos (y) + 1 \text { for all real numbers } y
$$

(because if y is real, then cos(y) is also real), and so forth. Thus universal statements are very versatile in their applicability - you can get $P ( x )$ to hold for whatever x you wish. Existential statements, by contrast, are more limited; if you know that 

$$
x ^ {2} + 2 x - 8 = 0 \mathrm{forsomerealnumber} x
$$

then you cannot simply substitute in any real number you wish, $\mathrm { e . g . , \pi }$ 4 and conclude that $\pi ^ { 2 } + 2 \pi - 8 = 0$ . However, you can of course still conclude that $x ^ { 2 } + 2 x - 8 = 0$ for some real number x, it’s just that you don’t get to pick which x it is. (To continue the gaming metaphor, you can make $P ( x )$ hold, but your opponent gets to pick x for you, you don’t get to choose for yourself.) 

Remark A.5.1. In the history of logic, quantifiers were formally studied thousands of years before Boolean logic was. Indeed, Aristotlean logic, developed of course by Aristotle (384BC – 322BC) and his school, deals with objects, their properties, and quantifiers such as “for all” and “for some”. A typical line of reasoning (or syllogism) in Aristotlean logic goes like this: “All men are mortal. Socrates is a man. Hence, Socrates is mortal”. Aristotlean logic is a subset of mathematical logic, but is not as expressive because it lacks the concept of logical connectives such as and, or, or if-then (although “not” is allowed), and also lacks the concept of a binary relation such as $= \mathrm { o r } <$ 

Swapping the order of two quantifiers may or may not make a difference to the truth of a statement. Swapping two “for all” quantifiers is harmless: a statement such as 

For all real numbers $^ { a , }$ and for all real numbers $b ,$ 

$$
\text { we   have } (a + b) ^ {2} = a ^ {2} + 2 a b + b ^ {2}
$$

is logically equivalent to the statement 

For all real numbers $b ,$ and for all real numbers $^ { a , }$ 

$$
\mathrm{wehave} (a + b) ^ {2} = a ^ {2} + 2 a b + b ^ {2}
$$

(why? The reason has nothing to do with whether the identity $( a + b ) ^ { 2 } =$ $a ^ { 2 } + 2 a b + b ^ { 2 }$ is actually true or not). Similarly, swapping two “there exists” quantifiers has no efect: 

There exists a real number $^ { a , }$ and there exists a real number $b ,$ 

$$
\mathrm{suchthat} a ^ {2} + b ^ {2} = 0
$$

is logically equivalent to 

There exists a real number $b ,$ and there exists a real number $a ,$ 

$$
\mathrm{suchthat} a ^ {2} + b ^ {2} = 0.
$$

However, swapping a “for all” with a “there exists” makes a lot of diference. Consider the following two statements: 

(a) For every integer $n ,$ , there exists an integer m which is larger than n. 

(b) There exists an integer m such that m is larger than n for every integer n. 

Statement (a) is obviously true: if your opponent hands you an integer n, you can always find an integer m which is larger than n. But Statement (b) is false: if you choose m first, then you cannot ensure that m is larger than every integer n; your opponent can easily pick a number n bigger than m to defeat that. The crucial diference between the two statements is that in Statement (a), the integer n was chosen $\mathit { f i r s t } ,$ and integer m could then be chosen in a manner depending on n; but in Statement (b), one was forced to choose m first, without knowing in advance what n is going to be. In short, the reason why the order of quantifiers is important is that the inner variables may possibly depend on the outer variables, but not vice versa. 

## — Exercises —

Exercise A.5.1. What does each of the following statements mean, and which of them are true? Can you find gaming metaphors for each of these statements? 

(a) For every positive number x, and every positive number y, we have $y ^ { 2 } =$ x. 

(b) There exists a positive number x such that for every positive number $y _ { \mathrm { { i } } }$ we have $y ^ { 2 } = x$ 

(c) There exists a positive number x, and there exists a positive number $y ,$ such that $y ^ { 2 } = x$ 

(d) For every positive number y, there exists a positive number x such that $y ^ { 2 } = x$ 

(e) There exists a positive number y such that for every positive number $x ,$ we have $y ^ { 2 } = x$ 

## A.6 Some examples of proofs and quantifiers

Here we give some simple examples of proofs involving the “for all” and “there exists” quantifiers. The results themselves are simple, but you should pay attention instead to how the quantifiers are arranged and how the proofs are structured. 

Proposition A.6.1. For every $\varepsilon > 0$ there exists a $\delta > 0$ such that $2 \delta < \varepsilon$ 

Proof. Let $\varepsilon > 0$ be arbitrary. We have to show that there exists a $\delta > 0$ such that $2 \delta < \varepsilon$ . We only need to pick one such $\delta ;$ choosing $\delta : = \varepsilon / 3$ will work, since one then has $2 \delta = 2 \varepsilon / 3 < \varepsilon$ □ 

Notice how $\varepsilon$ has to be arbitrary, because we are proving something for every $\varepsilon ;$ on the other hand, $\delta$ can be chosen as you wish, because you only need to show that there exists a $\delta$ which does what you want. Note also that $\delta$ can depend on $\varepsilon ,$ , because the δ-quantifier is nested inside the ε-quantifier. If the quantifiers were reversed, i.e., if you were asked to prove “There exists a $\delta > 0$ such that for every $\varepsilon > 0 , 2 \delta < \varepsilon ^ { \prime \prime }$ , then you would have to select δ first before being given $\varepsilon .$ In this case it is impossible to prove the statement, because it is false (why?). 

Normally, when one has to prove a “There exists...” statement, e.g., “Prove that there exists an $\varepsilon > 0$ such that X is true”, one proceeds by selecting $\varepsilon { \mathrm { ~ c a r e f u l l y } } ,$ and then showing that X is true for that $\varepsilon .$ However, this sometimes requires a lot of foresight, and it is legitimate to defer the selection of $\varepsilon$ until later in the argument, when it becomes clearer what properties $\varepsilon$ needs to satisfy. The only thing to watch out for is to make sure that $\varepsilon$ does not depend on any of the bound variables nested inside X. For instance: 

Proposition A.6.2. There exists $a n \ \varepsilon > 0$ such that sin $( x ) > x / 2$ for all $0 < x < \varepsilon$ 

Proof. We pick $\varepsilon > 0$ to be chosen later, and let $0 < x < \varepsilon$ . Since the derivative of sin(x) is cos(x), we see from the mean-value theorem we have 

$$
{\frac {\sin (x)}{x}} = {\frac {\sin (x) - \sin (0)}{x - 0}} = \cos (y)
$$

for some $0 \leq y \leq x$ . Thus in order to ensure that sin $( x ) > x / 2$ , it would sufice to ensure that cos $( y ) > 1 / 2$ . To do this, it would sufice to ensure that $0 \leq y < \pi / 3$ (since the cosine function takes the value of 1 at 0, takes the value of $1 / 2$ at $\pi / 3$ , and is decreasing in between). Since $0 \leq y \leq x$ and $0 < x < \varepsilon$ , we see that $0 \leq y < \varepsilon$ . Thus if we pick $\varepsilon : = \pi / 3$ , then we have $0 \leq y < \pi / 3$ as desired, and so we can ensure that $\sin ( x ) > x / 2$ for all $0 < x < \varepsilon$ □ 

Note that the value of ε that we picked at the end did not depend on the nested variables x and $y .$ . This makes the above argument legitimate. Indeed, we can rearrange it so that we don’t have to postpone anything: 

Proof. We choose $\varepsilon : = \pi / 3 ;$ ; clearly $\varepsilon > 0$ . Now we have to show that for all $0 < x < \pi / 3$ , we have sin $( x ) > x / 2$ . So let $0 < x < \pi / 3$ be arbitrary. By the mean-value theorem we have 

$$
{\frac {\sin (x)}{x}} = {\frac {\sin (x) - \sin (0)}{x - 0}} = \cos (y)
$$

for some $0 \leq y \leq x$ . Since $0 \leq y \leq x$ and $0 < x < \pi / 3$ , we have $0 \leq$ $y < \pi / 3$ . Thus $\cos ( y ) > \cos ( \pi / 3 ) = 1 / 2$ , since cos is decreasing on the interval $[ 0 , \pi / 3 ]$ . Thus we have sin $( x ) / x > 1 / 2$ and hence sin $( x ) > x / 2$ as desired. □ 

If we had chosen $\varepsilon$ to depend on x and y then the argument would not be valid, because $\varepsilon$ is the outer variable and $x , y$ are nested inside it. 

## A.7 Equality

As mentioned before, one can create statements by starting with expressions (such as $2 \times 3 + 5 )$ and then asking whether an expression obeys a certain property, or whether two expressions are related by some sort of relation $( = , \leq , \in , \mathrm { e t c . } )$ . There are many relations, but the most important one is equality, and it is worth spending a little time reviewing this concept. 

Equality is a relation linking two objects $x , y$ of the same type $T$ $\mathrm { ( e . g . , }$ two integers, or two matrices, or two vectors, etc.). Given two such objects $x$ and $y ,$ the statement $x = y$ may or may not be true; it depends on the value of x and y and also on how equality is defined for the class of objects under consideration. For instance, as real numbers, the two numbers 0.9999 . . . and 1 are equal. In modular arithmetic with modulus 10 (in which numbers are considered equal to their remainders modulo 10), the numbers 12 and 2 are considered equal, $1 2 = 2$ , even though this is not the case in ordinary arithmetic. 

How equality is defined depends on the class $T$ of objects under consideration, and to some extent is just a matter of definition. However, for the purposes of logic we require that equality obeys the following four axioms of equality: 

(Reflexive axiom). Given any object x, we have $x = x$ 

(Symmetry axiom). Given any two objects x and y of the same type, if $x = y$ , then $y = x$ 

(Transitive axiom). Given any three objects $x , y , z$ of the same type, if $x = y$ and $y = z$ , then $x = z$ 

(Substitution axiom). Given any two objects x and y of the same type, if $x = y$ , then $f ( x ) = f ( y )$ for all functions or operations $f .$ 

Similarly, for any property $P ( x )$ depending on x, if $x = y$ , then $P ( x )$ and $P ( y )$ are equivalent statements. 

The first three axioms are clear, together, they assert that equality is an equivalence relation. To illustrate the substitution we give some examples. 

Example A.7.1. Let x and y be real numbers. If $x = y$ , then $2 x = 2 y$ and sin $( x ) = \sin ( y )$ . Furthermore, $x + z = y + z$ for any real number z. 

Example A.7.2. Let n and m be integers. If n is odd and $n = m$ , then m must also be odd. If we have a third integer k, and we know that $n > k$ and $n = m$ , then we also know that $m > k$ 

Example A.7.3. Let x, $y , z$ be real numbers. If we know that $x = \sin ( y )$ and $y = z ^ { 2 }$ , then (by the substitution axiom) we have sin $( y ) = \sin ( z ^ { 2 } )$ • and hence (by the transitive axiom) we have $x = \sin ( z ^ { 2 } )$ 

Thus, from the point of view of logic, we can define equality on a class of objects however we please, so long as it obeys the reflexive, symmetry, and transitive axioms, and is consistent with all other operations on the class of objects under discussion in the sense that the substitution axiom was true for all of those operations. For instance, if we decided one day to modify the integers so that 12 was now equal to 2, one could only do so if one also made sure that 2 was now equal to 12, and that $f ( 2 ) = f ( 1 2 )$ for any operation f on these modified integers. For instance, we now need $2 + 5$ to be equal to $1 2 + 5$ . (In this case, pursuing this line of reasoning will eventually lead to modular arithmetic with modulus 10.) 

## — Exercises —

Exercise A.7.1. Suppose you have four real numbers $a , b , c , d$ and you know that $a = b$ and $c = d .$ . Use the above four axioms to deduce that $a + d = b + c$ 

## Chapter B

# Appendix: the decimal system

In Chapters 2, 4, 5 we painstakingly constructed the basic number systems of mathematics: the natural numbers, integers, rationals, and reals. Natural numbers were simply postulated to exist, and to obey five axioms; the integers then came via (formal) diferences of the natural numbers; the rationals then came from (formal) quotients of the integers, and the reals then came from (formal) limits of the rationals. 

This is all very well and good, but it does seem somewhat alien to one’s prior experience with these numbers. In particular, very little use was made of the decimal system, in which the digits 0, 1, 2, 3, 4, 5, 6, 7, 8, 9 are combined to represent these numbers. Indeed, except for a number of examples which were not essential to the main construction, the only decimals we really used were the numbers 0, 1, and 2, and the latter two can be rewritten as 0++ and (0++)++. 

The basic reason for this is that the decimal system itself is not essential to mathematics. It is very convenient for computations, and we have grown accustomed to it thanks to a thousand years of use, but in the history of mathematics it is actually a comparatively recent invention. Numbers have been around for about ten thousand years (starting from scratch marks on cave walls), but the modern Hindu-Arabic base 10 system for representing numbers only dates from the 11th century or so. Some early civilizations relied on other bases; for instance the Babylonians used a base 60 system (which still survives in our time system of hours, minutes, and seconds, and in our angular system of degrees, minutes, and seconds). And the ancient Greeks were able to do quite advanced mathematics, despite the fact that the most advanced number representation system available to them was the Roman numeral system I, II, III, IV, . . ., which was horrendous for computations of even two-digit numbers. And of course modern computing relies on binary, hexadecimal, or byte-based (base 256) arithmetic instead of decimal, while analog computers such as the slide rule do not really rely on any number representation system at all. In fact, now that computers can do the menial work of number-crunching, there is very little use for decimals in modern mathematics. Indeed, we rarely use any numbers other than one-digit numbers or one-digit fractions (as well as $e , \pi , i )$ explicitly in modern mathematical work; any more complicated numbers usually get called more generic names such as n. 

Nevertheless, the subject of decimals does deserve an appendix, because it is so integral to the way we use mathematics in our everyday life, and also because we do want to use such notation as $3 . 1 4 1 5 9 \ldots$ to refer to real numbers, as opposed to the far clunkier ${ } ^ { 6 \cdot } \mathrm { L I M } _ { n \to \infty } a _ { n }$ 4 where $a _ { 1 } = 3 . 1 , a _ { 2 } : = 3 . 1 4 , a _ { 3 } : = 3 . 1 4 1 , . . . ^ { \cdot }$ 

We begin by reviewing how the decimal system works for the positive integers, and then turn to the reals. Note that in this discussion we shall freely use all the results from earlier chapters. 

## B.1 The decimal representation of natural numbers

In this section we will avoid the usual convention of abbreviating $a \times b$ as $a b .$ since this would mean that decimals such as 34 might be misconstrued as $3 \times 4$ 

Definition B.1.1 (Digits). A digit is any one of the ten symbols $\mathbf { 0 , 1 , 2 , 3 , . . . , 9 }$ . We equate these digits with natural numbers by the formulae $0 \equiv 0 , 1 \equiv 0 { + } { + } , 2 \equiv 1 { + } { + }$ , etc. all the way up to $9 \equiv 8 + +$ We also define the number ten by the formula ten $: = 9 + +$ . (We cannot use the decimal notation 10 to denote ten yet, because that presumes knowledge of the decimal system and would be circular.) 

Definition B.1.2 (Positive integer decimals). A positive integer decimal is any string $a _ { n } a _ { n - 1 } \ldots a _ { 0 }$ of digits, where $n \geq 0$ is a natural number, and the first digit $a _ { n }$ is non-zero. Thus, for instance, 3049 is a positive integer decimal, but 0493 or 0 is not. We equate each positive integer decimal with a positive integer by the formula 

$$
a _ {n} a _ {n - 1} \dots a _ {0} \equiv \sum_ {i = 0} ^ {n} a _ {i} \times \mathrm{ten} ^ {i}.
$$

Remark B.1.3. Note in particular that this definition implies that 

$$
1 0 = 0 \times \mathrm{ten} ^ {0} + 1 \times \mathrm{ten} ^ {1} = \mathrm{ten}
$$

and thus we can write ten as the more familiar 10. Also, a single digit integer decimal is exactly equal to that digit itself, e.g., the decimal 3 by the above definition is equal to 

$$
3 = 3 \times \mathrm{ten} ^ {0} = 3
$$

so there is no possibility of confusion between a single digit, and a single digit decimal. (This is a subtle distinction, and not one which is worth losing much sleep over.) 

Now we show that this decimal system indeed represents the positive integers. It is clear from the definition that every positive decimal representation gives a positive integer, since the sum consists entirely of natural numbers, and the last term $a _ { n } \tan ^ { n }$ is non-zero by definition. 

Theorem B.1.4 (Uniqueness and existence of decimal representations). Every positive integer m is equal to exactly one positive integer decimal. 

Proof. We shall use the principle of strong induction (Proposition 2.2.14, with $m _ { 0 } : = 1 )$ . For any positive integer $m ,$ let $P ( m )$ denote the statement $^ { 6 6 } m$ is equal to exactly one positive integer decimal”. Suppose we already know $P ( m ^ { \prime } )$ is true for all positive integers $m ^ { \prime } < m ;$ we now wish to prove $P ( m )$ 

First observe that either $m \ \geq \ \mathrm { t e n }$ or $m \in \{ 1 , 2 , 3 , 4 , 5 , 6 , 7 , 8 , 9 \}$ (This is easily proved by ordinary induction.) Suppose first that $m \in \{ 1 , 2 , 3 , 4 , 5 , 6 , 7 , 8 , 9 \}$ . Then $m$ clearly is equal to a positive integer decimal consisting of a single digit, and there is only one single-digit decimal which is equal to $m$ . Furthermore, no decimal consisting of two or more digits can equal m, since if $a _ { n } \ldots a _ { 0 }$ is such a decimal (with $n > 0 )$ we have 

$$
a _ {n} \dots a _ {0} = \sum_ {i = 0} ^ {n} a _ {i} \times \mathrm{ten} ^ {i} \geq a _ {n} \times \mathrm{ten} ^ {n} \geq \mathrm{ten} > m.
$$

Now suppose that $m \ \geq \ \mathrm { t e n }$ . Then by the Euclidean algorithm (Proposition 2.3.9) we can write 

$$
m = s \times \mathrm{ten} + r
$$

where $s$ is a positive integer, and $r \in \{ 0 , 1 , 2 , 3 , 4 , 5 , 6 , 7 , 8 , 9 \}$ . Since 

$$
s <   s \times \mathrm{ten} \leq s \times \mathrm{ten} + r = m
$$

we can use the strong induction hypothesis and conclude that $P ( s )$ is true. In particular, s has a decimal representation 

$$
s = b _ {p} \ldots b _ {0} = \sum_ {i = 0} ^ {p} b _ {i} \times \mathrm{ten} ^ {i}.
$$

Multiplying by ten, we see that 

$$
s \times \mathrm{ten} = \sum_ {i = 0} ^ {p} b _ {i} \times \mathrm{ten} ^ {i + 1} = b _ {p} \dots b _ {0} 0,
$$

and then adding r we see that 

$$
m = s \times \mathrm{ten} + r = \sum_ {i = 0} ^ {p} b _ {i} \times \mathrm{ten} ^ {i + 1} + r = b _ {p} \dots b _ {0} r.
$$

Thus m has at least one decimal representation. Now we need to show that m has at most one decimal representation. Suppose for sake of contradiction that we have at least two diferent representations 

$$
m = a _ {n} \ldots a _ {0} = a _ {n ^ {\prime}} ^ {\prime} \ldots a _ {0} ^ {\prime}.
$$

First observe by the previous computation that 

$$
a _ {n} \ldots a _ {0} = (a _ {n} \ldots a _ {1}) \times \mathrm{ten} + a _ {0}
$$

and 

$$
a _ {n ^ {\prime}} ^ {\prime} \dots a _ {0} ^ {\prime} = (a _ {n ^ {\prime}} ^ {\prime} \dots a _ {1} ^ {\prime}) \times \mathrm{ten} + a _ {0} ^ {\prime}
$$

and so after some algebra we obtain 

$$
a _ {0} ^ {\prime} - a _ {0} = (a _ {n} \dots a _ {1} - a _ {n ^ {\prime}} ^ {\prime} \dots a _ {1} ^ {\prime}) \times \mathrm{ten}.
$$

The right-hand side is a multiple of ten, while the left-hand side lies strictly between ten and + ten. Thus both sides must be equal to 0. This means that $a _ { 0 } = a _ { 0 } ^ { \prime }$ and $a _ { n } \ldots a _ { 1 } = a _ { n ^ { \prime } } ^ { \prime } \ldots a _ { 1 } ^ { \prime }$ . But by previous arguments, we know that $a _ { n } \ldots a _ { 1 }$ is a smaller integer than $a _ { n } \ldots a _ { 0 }$ Thus by the strong induction hypothesis, the number $a _ { n } \ldots a _ { 0 }$ has only one decimal representation, which means that $n ^ { \prime }$ must equal n and $a _ { i } ^ { \prime }$ must equal $a _ { i }$ for all $i = 1 , \ldots , n$ Thus the decimals $a _ { n } \ldots a _ { 0 }$ and $a _ { n ^ { \prime } } ^ { \prime } \ldots a _ { 0 } ^ { \prime }$ are in fact identical, contradicting the assumption that they were diferent. □ 

We refer to the decimal given by the above theorem as the decimal representation of m. Once one has this decimal representation, one can then derive the usual laws of long addition and long multiplication to connect the decimal representation of $x + y { \mathrm { ~ o r ~ } } x \times y$ to that of x or y (Exercise B.1.1). 

Once one has decimal representation of positive integers, one can of course represent negative integers decimally as well by using the sign. Finally, we let 0 be a decimal as well. This gives decimal representations of all integers. Every rational is then the ratio of two decimals, e.g., $3 3 5 / 1 1 3 \mathrm { \ o r \ - 1 / 2 }$ (with the denominator required to be non-zero, of course), though there may be more than one way to represent a rational as such a ratio, e.g., $6 / 4 = 3 / 2$ 

Since $\tan = 1 0 ,$ , we will now use 10 instead of ten throughout, as is customary. 

## — Exercises —

Exercise B.1.1. The purpose of this exercise is to demonstrate that the procedure of long addition taught to you in elementary school is actually valid. Let $A = a _ { n } \ldots a _ { 0 }$ and $B = \boldsymbol { b _ { m } } \ldots \boldsymbol { b _ { 0 } }$ be positive integer decimals. Let us adopt the convention that $a _ { i } = 0$ when $i > n$ , and $b _ { i } = 0$ when $i > m ;$ ; for instance, if $A = 3 7 2$ , then $a _ { 0 } = 2 , a _ { 1 } = 7 , a _ { 2 } = 3 , a _ { 3 } = 0 , a _ { 4 } = 0$ , and so forth. Define the numbers $c _ { 0 } , c _ { 1 } , \ldots$ . and $\varepsilon _ { 0 } , \varepsilon _ { 1 } , \ldots$ . recursively by the following long addition algorithm. 

We set $\varepsilon _ { 0 } : = 0$ 

Now suppose that $\varepsilon _ { i }$ has already been defined for some $i \geq 0$ . If $a _ { i } +$ $b _ { i } + \varepsilon _ { i } < 1 0$ , we set $c _ { i } : = a _ { i } + b _ { i } + \varepsilon _ { i }$ and $\varepsilon _ { i + 1 } : = 0 ;$ otherwise, if $a _ { i } + b _ { i } + \varepsilon _ { i } \geq 1 0$ , we set $c _ { i } : = a _ { i } + b _ { i } + \varepsilon _ { i } - 1 0$ and $\varepsilon _ { i + 1 } = 1$ . (The number $\varepsilon _ { i + 1 }$ is the “carry digit” from the $i ^ { t h }$ decimal place to the $( i + 1 ) ^ { t h }$ decimal place.) 

Prove that the numbers $c _ { 0 } , c _ { 1 } , \ldots .$ . are all digits, and that there exists an l such that $c _ { l } \neq 0$ and $c _ { i } = 0$ for all $i > l$ . Then show that $c _ { l } c _ { l - 1 } \ldots c _ { 1 } c _ { 0 }$ is the decimal representation of $A + B$ 

Note that one could in fact use this algorithm to define addition, but it would look extremely complicated, and to prove even such simple facts as $( a + b ) + c = a + ( b + c )$ would be rather dificult. This is one of the reasons why we have avoided the decimal system in our construction of the natural numbers. The procedure for long multiplication (or long subtraction, or long division) is even worse to lay out rigorously; we will not do so here. 

## B.2 The decimal representation of real numbers

We need a new symbol: the decimal point $^ { 6 6 } \cdot ^ { 5 9 }$ 

Definition B.2.1 (Real decimals). A real decimal is any sequence of digits, and a decimal point, arranged as 

$$
\pm a _ {n} \dots a _ {0}. a _ {- 1} a _ {- 2} \dots
$$

which is finite to the left of the decimal point (so n is a natural number), but infinite to the right of the decimal point, where is either + or , and $a _ { n } \ldots a _ { 0 }$ is a natural number decimal (i.e., either a positive integer decimal, or 0). This decimal is equated to the real number 

$$
\pm a _ {n} \dots a _ {0}. a _ {- 1} a _ {- 2} \dots \equiv \pm 1 \times \sum_ {i = - \infty} ^ {n} a _ {i} \times 1 0 ^ {i}.
$$

The series is always convergent (Exercise B.2.1). Next, we show that every real number has at least one decimal representation: 

Theorem B.2.2 (Existence of decimal representations). Every real number x has at least one decimal representation 

$$
x = \pm a _ {n} \dots a _ {0}. a _ {- 1} a _ {- 2} \dots .
$$

Proof. We first note that $x = 0$ has the decimal representation 0.000 . . .. Also, once we find a decimal representation for x, we automatically get a decimal representation for x by changing the sign . Thus it sufices to prove the theorem for positive real numbers x (by Proposition 5.4.4). 

Let $n \geq 0$ be any natural number. From the Archimedean property (Corollary 5.4.13) we know that there is a natural number M such that $M \times 1 0 ^ { - n } > x$ . Since $0 \times 1 0 ^ { - n } \leq x .$ , we thus see that there must exist a natural number $s _ { n }$ such that $s _ { n } \times 1 0 ^ { - n } \leq x$ and $s _ { n } + + \times 1 0 ^ { - n } > x$ . (If no such natural number existed, one could use induction to conclude that $s \times 1 0 ^ { - n } \leq x$ for all natural numbers s, contradicting the Archimedean property.) 

Now consider the sequence $s _ { 0 } , s _ { 1 } , s _ { 2 } , \ldots$ Since we have 

$$
s _ {n} \times 1 0 ^ {- n} \leq x <   (s _ {n} + 1) \times 1 0 ^ {- n}
$$

we thus have 

$$
(1 0 \times s _ {n}) \times 1 0 ^ {- (n + +)} \leq x <   (1 0 \times s _ {n} + 1 0) \times 1 0 ^ {- (n + +)}.
$$

On the other hand, we have 

$$
s _ {n + 1} \times 1 0 ^ {- (n + 1)} \leq x <   (s _ {n + 1} + 1) \times 1 0 ^ {- (n + 1)}
$$

and hence we have 

$$
1 0 \times s _ {n} <   s _ {n + 1} + 1 \mathrm{and} s _ {n + 1} <   1 0 \times s _ {n} + 1 0.
$$

From these two inequalities we see that we have 

$$
1 0 \times s _ {n} \leq s _ {n + 1} \leq 1 0 \times s _ {n} + 9
$$

and hence we can find a digit $a _ { n + 1 }$ such that 

$$
s _ {n + 1} = 1 0 \times s _ {n} + a _ {n + 1}
$$

and hence 

$$
s _ {n + 1} \times 1 0 ^ {- (n + 1)} = s _ {n} \times 1 0 ^ {- n} + a _ {n + 1} \times 1 0 ^ {- (n + 1)}.
$$

From this identity and induction, we can obtain the formula 

$$
s _ {n} \times 1 0 ^ {- n} = s _ {0} + \sum_ {i = 0} ^ {n} a _ {i} \times 1 0 ^ {- i}.
$$

Now we take limits of both sides (using Exercise B.2.1) to obtain 

$$
\lim _ {n \to \infty} s _ {n} \times 1 0 ^ {- n} = s _ {0} + \sum_ {i = 0} ^ {\infty} a _ {i} \times 1 0 ^ {- i}.
$$

On the other hand, we have 

$$
x - 1 0 ^ {- n} \leq s _ {n} \times 1 0 ^ {- n} \leq x
$$

for all $n ,$ so by the squeeze test (Corollary 6.4.14) we have 

$$
\lim _ {n \to \infty} s _ {n} \times 1 0 ^ {- n} = x.
$$

Thus we have 

$$
x = s _ {0} + \sum_ {i = 0} ^ {\infty} a _ {i} \times 1 0 ^ {- i}.
$$

Since $s _ { 0 }$ already has a positive integer decimal representation by Theorem B.1.4, we thus see that x has a decimal representation as desired. 

There is however one slight flaw with the decimal system: it is possible for one real number to have two decimal representations. 

Proposition B.2.3 (Failure of uniqueness of decimal representations). The number 1 has two diferent decimal representations: 1.000 . . . and 0.999 . . .. 

Proof. The representation $1 = 1 . 0 0 0 \ldots$ is clear. Now let’s compute 0.999 . . .. By definition, this is the limit of the Cauchy sequence 

$$
0. 9, 0. 9 9, 0. 9 9 9, 0. 9 9 9 9, \dots .
$$

But this sequence has 1 as a formal limit by Proposition 5.2.8. □ 

It turns out that these are the only two decimal representations of 1 (Exercise B.2.2). In fact, as it turns out, all real numbers have either one or two decimal representations - two if the real is a terminating decimal, and one otherwise (Exercise B.2.3). 

$$
- \text { Exercises } -
$$

Exercise B.2.1. If $a _ { n } \cdot \cdot \cdot a _ { 0 } . a _ { - 1 } a _ { - 2 } \cdot \cdot \cdot$ . is a real decimal, show that the series $\scriptstyle \sum _ { i = - \infty } ^ { n } a _ { i } \times 1 0 ^ { i }$ is absolutely convergent. 

Exercise B.2.2. Show that the only decimal representations 

$$
1 = \pm a _ {n} \dots a _ {0}. a _ {- 1} a _ {- 2} \dots
$$

of 1 are $1 = 1 . 0 0 0 . .$ . and $1 = 0 . 9 9 9 \ldots$ 

Exercise B.2.3. A real number x is said to be a terminating decimal if we have $x = n / 1 0 ^ { - m }$ for some integers n, m. Show that if x is a terminating decimal, then x has exactly two decimal representations, while if x is not at terminating decimal, then x has exactly one decimal representation. 

Exercise B.2.4. Rewrite the proof of Corollary 8.3.4 using the decimal system. 

## Index

++ (increment), 16, 49 on integers, 77 +C, 299 α-length, 292 ε-adherent, 140, 213 continually ε-adherent, 140 ε-close eventual, 101 functions, 220 local, 220 rationals, 87 reals, 126 sequences, 101, 128 ε-steady, 96, 127 eventually ε-steady, 97, 127 a posteriori, 18 a priori, 18 absolute convergence for series, 166, 191 test, 167 absolute value for rationals, 86 for reals, 112 absorption laws, 46 abstraction, 21–22 addition long, 335 of cardinals, 72 of functions, 219 

of integers, 76 of natural numbers, 24 of rationals, 81 of reals, 104 adherent point infinite, 249 of sequences: see limit point of sequences of sets, 213 alternating series test, 167 analysis, 1 and: see conjunction antiderivative, 298 Archimedian property, 115 Aristotlean logic, 326 associativity of addition in N, 26 of composition, 52, 53 of multiplication in N, 30 see also:, ring, field, laws of algebra asymptotic discontinuity, 234 Axiom(s) in mathematics, 21–22 of choice, 36, 65, 200 of comprehension: see Axiom of universal specification of countable choice, 200 of equality, 329 

of foundation: see Axiom of regularity of induction: see principle of mathematical induction of infinity, 44 of natural numbers: see Peano axioms of pairwise union, 37 of power set, 58 of reflexivity, 329 of regularity, 47 of replacement, 43 of separation, 40 of set theory, 34, 36–37, 40, 43–44, 48, 58 of singleton sets and pair sets, 36 of specification, 40 of substitution, 50, 329 of symmetry, 329 of the empty set, 36 of transitivity, 329 of union, 59 of universal specification, 46 bijection, 54 binomial formula, 164 Bolzano-Weierstrass theorem, 151 Boolean algebra, 42 Boolean logic, 320 bound variable, 156, 321, 328 bounded from above and below, 235 function, 234 interval, 212 sequence, 99, 130 

sequence away from zero, 107, 111 set, 216 cancellation law of addition in N, 26 of multiplication in N, 31 of multiplication in R, 110 of multiplication in Z, 80 Cantor’s theorem, 195 cardinality arithmetic of, 71 of finite sets, 70 uniqueness of, 70 Cartesian product, 62 infinite, 199, 200 Cauchy criterion, 171 Cauchy sequence, 97, 127 chain rule, 256 chain: see totally ordered set change of variables formula, 302–312 choice arbitrary, 200 countable, 200 finite, 65 single, 36 closed interval, 212 closure, 213 cluster point: see limit point common refinement, 271 commutativity of addition in N, 26 of multiplication in N, 30 comparison principle (or test) for finite series, 157 for infinite series, 170 for sequences, 145 completeness 

of the reals, 146 composition of functions, 52 conjunction (and), 309 connectedness, 268 constant function, 51, 272 sequence, 148 continuity, 227 and convergence, 222 continuum, 211 hypothesis, 197 contrapositive, 316 convergence of a function at a point, 221 of sequences, 128 of series, 165 converse, 315 corollary, 25 countability, 181 of the integers, 185 of the rationals, 187 de Morgan laws, 43 decimal negative integer, 335 non-uniqueness of representation, 338 point, 335 positive integer, 335 real, 336 denumerable: see countable derivative, 251 diference rule, 255 diference set, 42 diferentiability at a point, 251 digit, 332 direct sum of functions, 63 discontinuity: see singularity 

disjoint sets, 42 disjunction (or), 309 inclusive vs. exclusive, 310 distance in Q, 87 in R, 126 distributive law for natural numbers, 30 see also:, laws of algebra divergence of sequences, 4 of series, 3, 165 ,see also: convergence divisibility, 207 division by zero, 3 formal (//), 82 of functions, 219 of rationals, 85 domain, 49 dominate: see majorize dominated convergence: see Lebesgue dominated convergence theorem doubly infinite, 212 dummy variable: see bound variable empty Cartesian product, 64 function, 52 sequence, 64 series, 160 set, 36 equality, 329 for functions, 51 for sets, 35 of cardinality, 68 equivalence of sequences, 101, 245 

relation, 330 Euclidean algorithm, 31 exponentiation of cardinals, 71 with base and exponent in N, 32 with base in Q and exponent in Z, 89, 90 with base in R and exponent in Z, 122 with base in R<sup>+</sup> and exponent in Q, 124 with base in R<sup>+</sup> and exponent in R, 154 expression, 308 extended real number system R∗, 119, 133 extremum: see maximum, minimum factorial, 164 family, 60 field, 84 ordered, 86 finite set, 70 fixed point theorem, 241 forward image: see image free variable, 321 Fubini’s theorem for finite series, 163 for infinite series, 188 see also:, interchanging integrals/sums with integrals/sums function, 49 implicit definition, 50 fundamental theorems of calculus, 296, 298 geometric series, 165, 171 

formula, 171, 174 graph, 51, 66, 219 greatest lower bound: see least upper bound half-infinite, 212 half-open, 212 harmonic series, 173 Hausdorf maximality principle, 209 Heine-Borel theorem for the real line, 216 identity map (or operator), 56 if: see implication if (if and only if), 27 ill-defined, 306, 309 image inverse image, 56 of sets, 56 implication (if), 312 improper integral, 278 inclusion map, 56 inconsistent, 198, 199 index of summation: see dummy variable index set, 60 induction: see Principle of mathematical induction infimum: see supremum infinite interval, 212 set, 70 injection: see one-to-one function integer part, 91, 116 integers Z definition, 74 

identification with rationals, 83 interspersing with rationals, 91 integral test, 290 integration by parts, 300–302 laws, 275, 280 piecewise constant, 273, 274 Riemann: see Riemann integral interchanging derivatives with derivatives, 9 finite sums with finite sums, 162, 163 integrals with integrals, 1 limits with derivatives, 8 limits with integrals, 8 limits with length, 11 limits with limits, 7, 8 sums with sums, 5, 188 intermediate value theorem, 238 intersection pairwise, 41 interval, 212 inverse function theorem, 262 image, 56 in logic, 316 of functions, 55 irrationality, 95 <sub>of</sub> √<sub>2, 91, 120</sub> isolated point, 215 jump discontinuity, 233 l<sup>1</sup>, l<sup>2</sup>, l∞, L<sup>1</sup>, L<sup>2</sup>, L∞ ,see also: supremum as norm 

L’Hˆopital’s rule, 10, 264 label, 60 laws of algebra for integers, 78 for rationals, 84 for reals, 106 laws of exponentiation, 89, 90, 122, 125 least upper bound, 117 least upper bound property, 117, 137 see also:, supremum Leibniz rule, 255 lemma, 25 length of interval, 269 limit at infinity, 250 formal (LIM), 103, 130 laws, 131, 223 left and right, 231 limiting values of functions, 4, 220 of sequences, 129 uniqueness of, 128, 223 limit inferior, see limit superior limit point of sequences, 139 of sets, 215 limit superior, 141 linearity of finite series, 161 of infinite series, 168 of integration, 274, 280 of limits, 131 Lipschitz constant, 260 Lipschitz continuous, 260 logical connective, 309 lower bound: see upper bound majorize, 276 

maximum, 203, 258 local, 258 of functions, 219, 236 principle, 236 mean value theorem, 259 meta-proof, 122 metric ,see also: distance minimum, 203, 258 local, 258 of a set of natural numbers, 183 of functions, 219, 236 minorize: see majorize monotone (increasing or decreasing) function, 241, 294 sequence, 138 morphism: see function multiplication of cardinals, 71 of functions, 220 of integers, 76 of natural numbers, 29 of rationals, 82 of reals, 105 Natural numbers N are infinite, 70 axioms: see Peano axioms identification with integers, 77 in set theory: see Axiom of infinity informal definition, 15 uniqueness of, 67 negation in logic, 310 of extended reals, 134 of integers, 77 

of rationals, 82 of reals, 106 negative: see negation, positive Newton’s approximation, 253 non-constructive, 200 objects, 34 primitive, 47 one-to-one correspondence: see bijection one-to-one function, 54 onto, 54 open interval, 212 or: see disjunction order ideal, 207 ordered n-tuple, 62 ordered pair, 62 construction of, 65 ordering lexicographical, 208 of cardinals, 198 of orderings, 209 of partitions, 270 of sets, 203 of the extended reals, 134 of the integers, 80 of the natural numbers, 27 of the rationals, 85 of the reals, 112 oscillatory discontinuity, 234 pair set, 36 partial function, 61 partial sum, 165 partially ordered set, 40, 202 partition, 269 Peano axioms, 16–19, 21 perfect matching: see bijection piecewise 

constant, 272 constant Riemann-Stieltjes integral, 293 continuous, 288 pigeonhole principle, 73 polynomial, 231 positive integer, 77 natural number, 27 rational, 85 real, 112 power set, 58 principle of infinite descent, 93 principle of mathematical induction, 19 backwards induction, 29 strong induction, 28, 204 transfinite, 207 product rule, see Leibniz rule proof abstract examples, 317–320, 327–328 by contradiction, 307, 316 proper subset, 39 property, 309 proposition, 25 propositional logic, 320 quantifier, 322 existential (for some), 323 negation of, 325 nested, 324 universal (for all), 322 Quotient rule, 255 Quotient: see division range, 49 ratio test, 180 rational numbers Q definition, 82 

identification with reals, 106 interspersing with rationals, 91 interspersing with reals, 115 real numbers R definition, 103 rearrangement of absolutely convergent series, 175 of divergent series, 176, 193 of finite series, 160 of non-negative series, 174 reciprocal of rationals, 84 of reals, 109 recursive definitions, 23, 67 reductio ad absurdum: see proof by contradiction removable discontinuity: see removable singularity removable singularity, 225, 233 restriction of functions, 218 Riemann hypothesis, 173 Riemann integrability, 277 closure properties, 280–285 failure of, 291 of bounded continuous functions, 287 of continuous functions on compacta, 287 of monotone functions, 289 of piecewise continuous bounded functions, 288 of uniformly continuous functions, 285 Riemann integral, 277 upper and lower, 277 

Riemann sums (upper and lower), 280 Riemann zeta function, 173 Riemann-Stieltjes integral, 294 ring, 78 commutative, 78 Rolle’s theorem, 259 root, 122 test, 178 Russell’s paradox, 46 scalar multiplication of functions, 220 Schr¨oder-Bernstein theorem, 198 sequence, 96 finite, 64 series finite, 155, 157 formal infinite, 164 laws, 168, 192 on arbitrary sets, 192 on countable sets, 188 vs. sum, 156 set axioms: see axioms of set theory informal definition, 34 signum function, 225 singleton set, 36 singularity, 234 square root, 50 Squeeze test for sequences, 145 statement, 306 strict upper bound, 204 subsequence, 149 subset, 39 substitution: see rearrangement subtraction formal ( ), 76 of functions, 220 of integers, 80 sum rule, 255 supremum (and infimum) of a set of extended reals, 136, 137 of a set of reals, 119, 121 of sequences of reals, 137 surjection: see onto tangent: see trigonometric function telescoping series, 169 ten, 332 theorem, 25 totally ordered set, 40, 203 transformation: see function triangle inequality for finite series, 157, 161 in R, 87 trichotomy of order for integers, 81 for natural numbers, 27 for rationals, 85 for reals, 112 of extended reals, 135 two-to-one function, 54 uncountability, 181 of the reals, 196 undecidable, 199 uniform continuity, 244 union, 59 pairwise, 37 universal set, 47 upper bound of a partially ordered set, 204 

Index 

of a set of reals, 116 ,see also: least upper bound 

variable, 320 vertical line test, 49, 66 

well ordering principle for arbitrary sets, 210 for natural numbers, 183 

well-defined, 306 

well-ordered sets, 204 

Zermelo-Fraenkel(-Choice) axioms, 61 see also:, axioms of set theory 

zero test for sequences, 145 for series, 166 

Zorn’s lemma, 206 

## Texts and Readings in Mathematics



1. R. B. Bapat: Linear Algebra and Linear Models (Third Edition) 





2. Rajendra Bhatia: Fourier Series (Second Edition) 





3. C. Musili: Representations of Finite Groups 





4. H. Helson: Linear Algebra (Second Edition) 





5. D. Sarason: Complex Function Theory (Second Edition) 





6. M. G. Nadkarni: Basic Ergodic Theory (Third Edition) 





7. H. Helson: Harmonic Analysis (Second Edition) 





8. K. Chandrasekharan: A Course on Integration Theory 





9. K. Chandrasekharan: A Course on Topological Groups 





10. R. Bhatia (ed.): Analysis, Geometry and Probability 





11. K. R. Davidson: C* – Algebras by Example (Reprint) 





12. M. Bhattacharjee et al.: Notes on Infinite Permutation Groups 





13. V. S. Sunder: Functional Analysis — Spectral Theory 





14. V. S. Varadarajan: Algebra in Ancient and Modern Times 





15. M. G. Nadkarni: Spectral Theory of Dynamical Systems 





16. A. Borel: Semisimple Groups and Riemannian Symmetric Spaces 





17. M. Marcolli: Seiberg – Witten Gauge Theory 





18. A. Bottcher and S. M. Grudsky: Toeplitz Matrices, Asymptotic Linear Algebra and Functional Analysis 





19. A. R. Rao and P. Bhimasankaram: Linear Algebra (Second Edition) 





20. C. Musili: Algebraic Geometry for Beginners 





21. A. R. Rajwade: Convex Polyhedra with Regularity Conditions and Hilbert's Third Problem 





22. S. Kumaresan: A Course in Differential Geometry and Lie Groups 





23. Stef Tijs: Introduction to Game Theory 





24. B. Sury: The Congruence Subgroup Problem 





25. R. Bhatia (ed.): Connected at Infinity 





26. K. Mukherjea: Differential Calculus in Normed Linear Spaces (Second Edition) 





27. Satya Deo: Algebraic Topology: A Primer (Corrected Reprint) 





28. S. Kesavan: Nonlinear Functional Analysis: A First Course 





29. S. Szabó: Topics in Factorization of Abelian Groups 





30. S. Kumaresan and G. Santhanam: An Expedition to Geometry 





31. D. Mumford: Lectures on Curves on an Algebraic Surface (Reprint) 





32. J. W. Milnor and J. D. Stasheff: Characteristic Classes (Reprint) 





33. K. R. Parthasarathy: Introduction to Probability and Measure (Corrected Reprint) 





34. Amiya Mukherjee: Topics in Differential Topology 





35. K. R. Parthasarathy: Mathematical Foundations of Quantum Mechanics 





36. K. B. Athreya and S. N. Lahiri: Measure Theory 





37. Terence Tao: Analysis I (Third Edition) 





38. Terence Tao: Analysis II (Second Edition) 





39. W. Decker and C. Lossen: Computing in Algebraic Geometry 





40. A. Goswami and B. V. Rao: A Course in Applied Stochastic Processes 





41. K. B. Athreya and S. N. Lahiri: Probability Theory 





42. A. R. Rajwade and A. K. Bhandari: Surprises and Counterexamples in Real Function Theory 





43. G. H. Golub and C. F. Van Loan: Matrix Computations (Reprint of the Third Edition) 





44. Rajendra Bhatia: Positive Definite Matrices 





45. K. R. Parthasarathy: Coding Theorems of Classical and Quantum Information Theory 





46. C. S. Seshadri: Introduction to the Theory of Standard Monomials (Second Edition) 





47. Alain Connes and Matilde Marcolli: Noncommutative Geometry, Quantum Fields and Motives 





48. Vivek S. Borkar: Stochastic Approximation: A Dynamical Systems Viewpoint 





49. B. J. Venkatachala: Inequalities: An Approach Through Problems 





50. Rajendra Bhatia: Notes on Functional Analysis 





52. S. Kesavan: Functional Analysis 





51. A. Clebsch (ed.): Jacobi's Lectures on Dynamics (Second Revised Edition) 





53. V. Lakshmibai and Justin Brown: Flag Varieties: An Interplay of Geometry, Combinatorics, and Representation Theory 





54. S. Ramasubramanian: Lectures on Insurance Models 





55. Sebastian M. Cioaba and M. Ram Murty: A First Course in Graph Theory and Combinatorics 





56. Bamdad R. Yahaghi: Iranian Mathematics Competitions, 1973-2007 





57. Aloke Dey: Incomplete Block Designs 





58 R. B. Bapat: Graphs and Matrices 





59. Hermann Weyl: Algebraic Theory of Numbers (Reprint) 





60. Carl Ludwig Siegel: Transcendental Numbers (Reprint) 





61. Steven J. Miller and Ramin Takloo-Bighash: An Invitation to Number Theory (Reprint) 





62. John Milnor: Dynamics in One Complex Variable (Reprint) 





63. R. P. Pakshirajan: Probability Theory: A Foundational Course 





64. Sharad S. Sane: Combinatorial Techniques 





65. Hermann Weyl: The Classical Groups: Their Invariants and Representations (Reprint) 





66. John Milnor: Morse Theory (Reprint) 





67. R. Bhatia (ed.): Connected at Infinity II 





68. Donald Passman: A Course in Ring Theory 





69. Amiya Mukherjee: Atiyah-Singer Index Theorem: An Introduction 





70. Fumio Hiai and Dénes Petz: Introduction to Matrix Analysis and Applications 

