

<!-- === Source: MinerU_markdown_Analysis_II_Third_Edition_-_By_Terence_Tao_1_2122707919320490001.md (Page 1) === -->

# Terence Tao

## Analysis II

Third Edition 

# Texts and Readings in Mathematics

Volume 38 

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

Analysis II 

Third Edition 

This work is a co-publication with Hindustan Book Agency, New Delhi, licensed for sale in all countries in electronic form only. Sold and distributed in print across the world by Hindustan Book Agency, P-19 Green Park Extension, New Delhi 110016, India. ISBN: 978-93-80250-65-6 © Hindustan Book Agency 2015. 

ISSN 2366-8725 (electronic) Texts and Readings in Mathematics ISBN 978-981-10-1804-6 (eBook) DQI 10.1007/978-981-10-1804-6 

Library of Congress Control Number: 2016940817 

© Springer Science+Business Media Singapore 2016 and Hindustan Book Agency 2015 

This work is subject to copyright. All rights are reserved by the Publishers, whether the whole or part of the material is concerned, specifically the rights of translation, reprinting, reuse of illustrations, recitation, broadcasting, reproduction on microfilms or in any other physical way, and transmission or information storage and retrieval, electronic adaptation, computer software, or by similar or dissimilar methodology now known or hereafter developed. 

The use of general descriptive names, registered names, trademarks, service marks, etc. in this publication does not imply, even in the absence of a specific statement, that such names are exempt from the relevant protective laws and regulations and therefore free for general use. 

The publishers, the authors and the editors are safe to assume that the advice and information in this book are believed to be true and accurate at the date of publication. Neither the publishers nor the authors or the editors give a warranty, express or implied, with respect to the material contained herein or for any errors or omissions that may have been made. 

This Springer imprint is published by Springer Nature 

The registered company is Springer Science+Business Media Singapore Pte Ltd. 

To my parents, for everything 

## Contents

Preface to the second and third editions ix
Preface to the first edition xi
About the Author xvii
1 Metric spaces 1
1.1 Definitions and examples . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
1.2 Some point-set topology of metric spaces . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
1.3 Relative topology . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 15
1.4 Cauchy sequences and complete metric spaces 17
1.5 Compact metric spaces 21
2 Continuous functions on metric spaces 28
2.1 Continuous functions 28
2.2 Continuity and product spaces 31
2.3 Continuity and compactness 34
2.4 Continuity and connectedness 36
2.5 Topological spaces (Optional) 39
3 Uniform convergence 45
3.1 Limiting values of functions 46
3.2 Pointwise and uniform convergence 48
3.3 Uniform convergence and continuity 53
3.4 The metric of uniform convergence 56
3.5 Series of functions; the Weierstrass M-test 58
3.6 Uniform convergence and integration 61
3.7 Uniform convergence and derivatives 63
3.8 Uniform approximation by polynomials 66
4 Power series 75
4.1 Formal power series 75
4.2 Real analytic functions 78 

4.3 Abel's theorem . . . . . . . . . . . . . . . . . . . . . . . . 83
4.4 Multiplication of power series . . . . . . . . . . . . . . . . . 87
4.5 The exponential and logarithm functions . . . . . . . . 90
4.6 A digression on complex numbers . . . . . . . . . . . 93
4.7 Trigonometric functions . . . . . . . . . . . . 101

5 Fourier series 107
5.1 Periodic functions . . . . . . . . . . . . 108
5.2 Inner products on periodic functions . . . . . . . 110
5.3 Trigonometric polynomials . . . . . . 114
5.4 Periodic convolutions . . . . 116
5.5 The Fourier and Plancherel theorems 121

6 Several variable differential calculus 127
6.1 Linear transformations 127
6.2 Derivatives in several variable calculus 134
6.3 Partial and directional derivatives 137
6.4 The several variable calculus chain rule 144
6.5 Double derivatives and Clairaut's theorem 147
6.6 The contraction mapping theorem 149
6.7 The inverse function theorem in several variable calculus 152
6.8 The implicit function theorem 157

7 Lebesgue measure 162
7.1 The goal: Lebesgue measure 164
7.2 First attempt: Outer measure 166
7.3 Outer measure is not additive 174
7.4 Measurable sets 176
7.5 Measurable functions 183

8 Lebesgue integration 187
8.1 Simple functions 187
8.2 Integration of non-negative measurable functions 193
8.3 Integration of absolutely integrable functions 201
8.4 Comparison with the Riemann integral 205
8.5 Fubini's theorem 207

Index 213
Texts and Readings in Mathematics 219 

# Preface to the second and third editions

Since the publication of the first edition, many students and lecturers have communicated a number of minor typos and other corrections to me. There was also some demand for a hardcover edition of the texts. Because of this, the publishers and I have decided to incorporate the corrections and issue a hardcover second edition of the textbooks. The layout, page numbering, and indexing of the texts have also been changed; in particular the two volumes are now numbered and indexed separately. However, the chapter and exercise numbering, as well as the mathematical content, remains the same as the first edition, and so the two editions can be used more or less interchangeably for homework and study purposes. 

The third edition contains a number of corrections that were reported for the second edition, together with a few new exercises, but is otherwise essentially the same text. 

## Preface to the first edition

This text originated from the lecture notes I gave teaching the honours undergraduate-level real analysis sequence at the University of California, Los Angeles, in 2003. Among the undergraduates here, real analysis was viewed as being one of the most dificult courses to learn, not only because of the abstract concepts being introduced for the first time (e.g., topology, limits, measurability, etc.), but also because of the level of rigour and proof demanded of the course. Because of this perception of dificulty, one was often faced with the dificult choice of either reducing the level of rigour in the course in order to make it easier, or to maintain strict standards and face the prospect of many undergraduates, even many of the bright and enthusiastic ones, struggling with the course material. 

Faced with this dilemma, I tried a somewhat unusual approach to the subject. Typically, an introductory sequence in real analysis assumes that the students are already familiar with the real numbers, with mathematical induction, with elementary calculus, and with the basics of set theory, and then quickly launches into the heart of the subject, for instance the concept of a limit. Normally, students entering this sequence do indeed have a fair bit of exposure to these prerequisite topics, though in most cases the material is not covered in a thorough manner. For instance, very few students were able to actually define a real number, or even an integer, properly, even though they could visualize these numbers intuitively and manipulate them algebraically. This seemed to me to be a missed opportunity. Real analysis is one of the first subjects (together with linear algebra and abstract algebra) that a student encounters, in which one truly has to grapple with the subtleties of a truly rigorous mathematical proof. As such, the course ofered an excellent chance to go back to the foundations of mathematics, and in particular the opportunity to do a proper and thorough construction of the real numbers. 

Thus the course was structured as follows. In the first week, I described some well-known “paradoxes” in analysis, in which standard laws of the subject (e.g., interchange of limits and sums, or sums and integrals) were applied in a non-rigorous way to give nonsensical results such $\mathrm { a s } 0 = 1$ . This motivated the need to go back to the very beginning of the subject, even to the very definition of the natural numbers, and check all the foundations from scratch. For instance, one of the first homework assignments was to check (using only the Peano axioms) that addition was associative for natural numbers (i.e., that $( a + b ) + c = a + ( b + c )$ for all natural numbers $a , b , c \mathrm { : }$ see Exercise 2.2.1). Thus even in the first week, the students had to write rigorous proofs using mathematical induction. After we had derived all the basic properties of the natural numbers, we then moved on to the integers (initially defined as formal diferences of natural numbers); once the students had verified all the basic properties of the integers, we moved on to the rationals (initially defined as formal quotients of integers); and then from there we moved on (via formal limits of Cauchy sequences) to the reals. Around the same time, we covered the basics of set theory, for instance demonstrating the uncountability of the reals. Only then (after about ten lectures) did we begin what one normally considers the heart of undergraduate real analysis - limits, continuity, diferentiability, and so forth. 

The response to this format was quite interesting. In the first few weeks, the students found the material very easy on a conceptual level, as we were dealing only with the basic properties of the standard number systems. But on an intellectual level it was very challenging, as one was analyzing these number systems from a foundational viewpoint, in order to rigorously derive the more advanced facts about these number systems from the more primitive ones. One student told me how dificult it was to explain to his friends in the non-honours real analysis sequence (a) why he was still learning how to show why all rational numbers are either positive, negative, or zero (Exercise 4.2.4), while the nonhonours sequence was already distinguishing absolutely convergent and conditionally convergent series, and (b) why, despite this, he thought his homework was significantly harder than that of his friends. Another student commented to me, quite wryly, that while she could obviously see why one could always divide a natural number n into a positive integer $q$ to give a quotient a and a remainder r less than $q$ (Exercise 2.3.5), she still had, to her frustration, much dificulty in writing down a proof of this fact. (I told her that later in the course she would have to prove statements for which it would not be as obvious to see that the statements were true; she did not seem to be particularly consoled by this.) Nevertheless, these students greatly enjoyed the homework, as when they did perservere and obtain a rigorous proof of an intuitive fact, it solidified the link in their minds between the abstract manipulations of formal mathematics and their informal intuition of mathematics (and of the real world), often in a very satisfying way. By the time they were assigned the task of giving the infamous “epsilon and delta” proofs in real analysis, they had already had so much experience with formalizing intuition, and in discerning the subtleties of mathematical logic (such as the distinction between the “for all” quantifier and the “there exists” quantifier), that the transition to these proofs was fairly smooth, and we were able to cover material both thoroughly and rapidly. By the tenth week, we had caught up with the non-honours class, and the students were verifying the change of variables formula for Riemann-Stieltjes integrals, and showing that piecewise continuous functions were Riemann integrable. By the conclusion of the sequence in the twentieth week, we had covered (both in lecture and in homework) the convergence theory of Taylor and Fourier series, the inverse and implicit function theorem for continuously diferentiable functions of several variables, and established the dominated convergence theorem for the Lebesgue integral. 

In order to cover this much material, many of the key foundational results were left to the student to prove as homework; indeed, this was an essential aspect of the course, as it ensured the students truly appreciated the concepts as they were being introduced. This format has been retained in this text; the majority of the exercises consist of proving lemmas, propositions and theorems in the main text. Indeed, I would strongly recommend that one do as many of these exercises as possible - and this includes those exercises proving “obvious” statements - if one wishes to use this text to learn real analysis; this is not a subject whose subtleties are easily appreciated just from passive reading. Most of the chapter sections have a number of exercises, which are listed at the end of the section. 

To the expert mathematician, the pace of this book may seem somewhat slow, especially in early chapters, as there is a heavy emphasis on rigour (except for those discussions explicitly marked “Informal”), and justifying many steps that would ordinarily be quickly passed over as being self-evident. The first few chapters develop (in painful detail) many of the “obvious” properties of the standard number systems, for instance that the sum of two positive real numbers is again positive (Exercise 5.4.1), or that given any two distinct real numbers, one can find rational number between them (Exercise 5.4.5). In these foundationa chapters, there is also an emphasis on non-circularity - not using later, more advanced results to prove earlier, more primitive ones. In particular, the usual laws of algebra are not used until they are derived (and they have to be derived separately for the natural numbers, integers, rationals, and reals). The reason for this is that it allows the students to learn the art of abstract reasoning, deducing true facts from a limited set of assumptions, in the friendly and intuitive setting of number systems; the payof for this practice comes later, when one has to utilize the same type of reasoning techniques to grapple with more advanced concepts (e.g., the Lebesgue integral). 

The text here evolved from my lecture notes on the subject, and thus is very much oriented towards a pedagogical perspective; much of the key material is contained inside exercises, and in many cases I have chosen to give a lengthy and tedious, but instructive, proof instead of a slick abstract proof. In more advanced textbooks, the student will see shorter and more conceptually coherent treatments of this material, and with more emphasis on intuition than on rigour; however, I feel it is important to know how to do analysis rigorously and “by hand” first, in order to truly appreciate the more modern, intuitive and abstract approach to analysis that one uses at the graduate level and beyond. 

The exposition in this book heavily emphasizes rigour and formalism; however this does not necessarily mean that lectures based on this book have to proceed the same way. Indeed, in my own teaching I have used the lecture time to present the intuition behind the concepts (drawing many informal pictures and giving examples), thus providing a complementary viewpoint to the formal presentation in the text. The exercises assigned as homework provide an essential bridge between the two, requiring the student to combine both intuition and formal understanding together in order to locate correct proofs for a problem. This I found to be the most dificult task for the students, as it requires the subject to be genuinely learnt, rather than merely memorized or vaguely absorbed. Nevertheless, the feedback I received from the students was that the homework, while very demanding for this reason, was also very rewarding, as it allowed them to connect the rather abstract manipulations of formal mathematics with their innate intuition on such basic concepts as numbers, sets, and functions. Of course, the aid of a good teaching assistant is invaluable in achieving this connection. 

With regard to examinations for a course based on this text, I would recommend either an open-book, open-notes examination with problems similar to the exercises given in the text (but perhaps shorter, with no unusual trickery involved), or else a take-home examination that involves problems comparable to the more intricate exercises in the text. The subject matter is too vast to force the students to memorize the definitions and theorems, so I would not recommend a closed-book examination, or an examination based on regurgitating extracts from the book. (Indeed, in my own examinations I gave a supplemental sheet listing the key definitions and theorems which were relevant to the examination problems.) Making the examinations similar to the homework assigned in the course will also help motivate the students to work through and understand their homework problems as thoroughly as possible (as opposed to, say, using flash cards or other such devices to memorize material), which is good preparation not only for examinations but for doing mathematics in general. 

Some of the material in this textbook is somewhat peripheral to the main theme and may be omitted for reasons of time constraints. For instance, as set theory is not as fundamental to analysis as are the number systems, the chapters on set theory (Chapters 3, 8) can be covered more quickly and with substantially less rigour, or be given as reading assignments. The appendices on logic and the decimal system are intended as optional or supplemental reading and would probably not be covered in the main course lectures; the appendix on logic is particularly suitable for reading concurrently with the first few chapters. Also, Chapter 5 (on Fourier series) is not needed elsewhere in the text and can be omitted. 

For reasons of length, this textbook has been split into two volumes. The first volume is slightly longer, but can be covered in about thirty lectures if the peripheral material is omitted or abridged. The second volume refers at times to the first, but can also be taught to students who have had a first course in analysis from other sources. It also takes about thirty lectures to cover. 

I am deeply indebted to my students, who over the progression of the real analysis course corrected several errors in the lectures notes from which this text is derived, and gave other valuable feedback. I am also very grateful to the many anonymous referees who made several corrections and suggested many important improvements to the text. 



I also thank Biswaranjan Behera, Tai-Danae Bradley, Brian, Eduardo Buscicchio, Carlos, EO, Florian, G¨okhan G¨u¸cl¨u, Evangelos Georgiadis, Ulrich Groh, Bart Kleijngeld, Erik Koelink, Wang Kuyyang, Matthis Lehmk¨uhler, Percy Li, Ming Li, Jason M., Manoranjan Majji, Geof Mess, Pieter Naaijkens, Vineet Nair, Cristina Pereyra, David Radnell, Tim Reijnders, Pieter Rofelsen, Luke Rogers, Marc Schoolderman, Kent Van Vels, Daan Wanrooy, Yandong Xiao, Sam Xu, Luqing Ye, and the students of Math 401/501 and Math 402/502 at the University of New Mexico for corrections to the first and second editions. 



Terence Tao 

## About the Author

Terence Tao, FAA FRS, is an Australian mathematician. His areas of interests are in harmonic analysis, partial differential equations, algebraic combinatorics, arithmetic combinatorics, geometric combinatorics, compressed sensing and analytic number theory. As of 2015, he holds the James and Carol Collins chair in mathematics at the University of California, Los Angeles. Professor Tao is a co-recipient of the 2006 Fields Medal and the 2014 Breakthrough Prize in Mathematics. He maintains a personal mathematics blog, which has been described by Timothy Gowers as “the undisputed king of all mathematics blogs”. 

# Chapter 1

## Metric spaces

## 1.1 Definitions and examples

In Definition 6.1.5 we defined what it meant for a sequence $( x _ { n } ) _ { n = m } ^ { \infty }$ of real numbers to converge to another real number $x ;$ indeed, this meant that for every $\varepsilon > 0$ , there exists an $N \geq m$ such that $| x - x _ { n } | \leq \varepsilon$ for all $n \geq N$ . When this is the case, we write $\scriptstyle \operatorname* { l i m } _ { n \to \infty } x _ { n } = x$ 

Intuitively, when a sequence $( x _ { n } ) _ { n = m } ^ { \infty }$ converges to a limit $x ,$ , this means that somehow the elements $x _ { n }$ of that sequence will eventually be as close to x as one pleases. One way to phrase this more precisely is to introduce the distance function $d ( x , y )$ between two real numbers by $d ( x , y ) : = | x - y |$ . (Thus for instance $d ( 3 , 5 ) = 2 , d ( 5 , 3 ) = 2$ , and $d ( 3 , 3 ) = 0 . )$ Then we have 

Lemma 1.1.1. Let $( x _ { n } ) _ { n = m } ^ { \infty }$ be a sequence of real numbers, and let x be another real number. Then $( x _ { n } ) _ { n = m } ^ { \infty }$ converges to x if and only if $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } d ( x _ { n } , x ) = 0 } \end{array}$ 

Proof. See Exercise 1.1.1. 

One would now like to generalize this notion of convergence, so that one can take limits not just of sequences of real numbers, but also sequences of complex numbers, or sequences of vectors, or sequences of matrices, or sequences of functions, even sequences of sequences. One way to do this is to redefine the notion of convergence each time we deal with a new type of object. As you can guess, this will quickly get tedious. A more eficient way is to work abstractly, defining a very general class of spaces - which includes such standard spaces as the real numbers, complex numbers, vectors, etc. - and define the notion of convergence on this entire class of spaces at once. (A space is just the set of all objects of a certain type - the space of all real numbers, the space of all $3 \times 3$ matrices, etc. Mathematically, there is not much distinction between a space and a set, except that spaces tend to have much more structure than what a random set would have. For instance, the space of real numbers comes with operations such as addition and multiplication, while a general set would not.) 

It turns out that there are two very useful classes of spaces which do the job. The first class is that of metric spaces, which we will study here. There is a more general class of spaces, called topological spaces, which is also very important, but we will only deal with this generalization briefly, in Section 2.5. 

Roughly speaking, a metric space is any space X which has a concept of distance $d ( x , y )$ - and this distance should behave in a reasonable manner. More precisely, we have 

Definition 1.1.2 (Metric spaces). A metric space $( X , d )$ is a space X of objects (called points), together with a distance function or metric $d : X \times X \to [ 0 , + \infty )$ , which associates to each pair $x , y$ of points in X a non-negative real number $d ( x , y ) \geq 0$ . Furthermore, the metric must satisfy the following four axioms: 

(a) For any $x \in X$ , we have $d ( x , x ) = 0$ 

(b) (Positivity) For any distinct $x , y \in X$ , we have $d ( x , y ) > 0$ 

(c) (Symmetry) For any $x , y \in X$ , we have $d ( x , y ) = d ( y , x )$ 

(d) (Triangle inequality) For any $x , y , z \in \ X$ , we have $d ( x , z ) \ \leq$ $d ( x , y ) + d ( y , z )$ 

In many cases it will be clear what the metric d is, and we shall abbreviate $( X , d )$ as just X. 

Remark 1.1.3. The conditions (a) and (b) can be rephrased as follows: for any $x , y \in X$ we have $d ( x , y ) = 0$ if and only if $x = y$ . (Why is this equivalent to (a) and (b)?) 

Example 1.1.4 (The real line). Let R be the real numbers, and let d : $\mathbf { R } \times \mathbf { R } \to [ 0 , \infty )$ be the metric $d ( x , y ) : = | x - y |$ mentioned earlier. Then $( \mathbf { R } , d )$ is a metric space (Exercise 1.1.2). We refer to d as the standard metric on R, and if we refer to R as a metric space, we assume that the metric is given by the standard metric d unless otherwise specified. 

## 1.1. Definitions and examples

Example 1.1.5 (Induced metric spaces). Let $( X , d )$ be any metric space, and let Y be a subset of $X$ . Then we can restrict the metric function $d : X \times X \to [ 0 , + \infty )$ to the subset $Y \times Y$ of $X \times X$ to create a restricted metric function $d | _ { Y \times Y } : Y \times Y \to [ 0 , + \infty )$ of $Y ;$ this is known as the metric on $Y$ induced by the metric d on $X$ . The pair $( Y , d | _ { Y \times Y } )$ is a metric space (Exercise 1.1.4) and is known the subspace of $( X , d )$ induced by $Y .$ . Thus for instance the metric on the real line in the previous example induces a metric space structure on any subset of the reals, such as the integers $\mathbf { Z } ,$ , or an interval $[ a , b ]$ , etc. 

Example 1.1.6 (Euclidean spaces). Let $n \geq 1$ be a natural number, and let $\mathbf { R } ^ { n }$ be the space of n-tuples of real numbers: 

$$
\mathbf {R} ^ {n} = \{(x _ {1}, x _ {2}, \dots , x _ {n}): x _ {1}, \dots , x _ {n} \in \mathbf {R} \}.
$$

We define the Euclidean metric (also called the $l ^ { 2 }$ metric) $d _ { l ^ { 2 } } : \mathbf { R } ^ { n } \times$ $\mathbf { R } ^ { n } \to \mathbf { R }$ by 

$$
\begin{array}{c} d _ {l ^ {2}} ((x _ {1}, \ldots , x _ {n}), (y _ {1}, \ldots , y _ {n})) := \sqrt {(x _ {1} - y _ {1}) ^ {2} + \ldots + (x _ {n} - y _ {n}) ^ {2}} \\ = \left(\sum_ {i = 1} ^ {n} (x _ {i} - y _ {i}) ^ {2}\right) ^ {1 / 2}. \end{array}
$$

Thus for instance, if $n = 2$ , then $d _ { l ^ { 2 } } ( ( 1 , 6 ) , ( 4 , 2 ) ) = \sqrt { 3 ^ { 2 } + 4 ^ { 2 } } = 5$ . This metric corresponds to the geometric distance between the two points $( x _ { 1 } , x _ { 2 } , \ldots , x _ { n } ) , ( y _ { 1 } , y _ { 2 } , \ldots , y _ { n } )$ as given by Pythagoras’ theorem. (We remark however that while geometry does give some very important examples of metric spaces, it is possible to have metric spaces which have no obvious geometry whatsoever. Some examples are given below.) The verification that $( \mathbf { R } ^ { n } , d )$ is indeed a metric space can be seen geometrically (for instance, the triangle inequality now asserts that the length of one side of a triangle is always less than or equal to the sum of the lengths of the other two sides), but can also be proven algebraically (see Exercise 1.1.6). We refer to $( \mathbf { R } ^ { n } , d _ { l ^ { 2 } } )$ as the Euclidean space of dimension n. Extending the convention from Example 1.1.4, if we refer to $\mathbf { R } ^ { n }$ as a metric space, we assume that the metric is given by the Euclidean metric unless otherwise specified. 

Example 1.1.7 (Taxi-cab metric). Again let $n \geq 1$ , and let $\mathbf { R } ^ { n }$ be as before. But now we use a diferent metric $d _ { l ^ { 1 } }$ , the so-called taxicab 

metric (or $l ^ { 1 }$ metric), defined by 

$$
\begin{array}{c} d _ {l ^ {1}} ((x _ {1}, x _ {2}, \ldots , x _ {n}), (y _ {1}, y _ {2}, \ldots , y _ {n})) := | x _ {1} - y _ {1} | + \ldots + | x _ {n} - y _ {n} | \\ = \sum_ {i = 1} ^ {n} | x _ {i} - y _ {i} |. \end{array}
$$

Thus for instance, if $n = 2$ , then $d _ { l ^ { 1 } } ( ( 1 , 6 ) , ( 4 , 2 ) ) = 3 + 4 = 7$ . This metric is called the taxi-cab metric, because it models the distance a taxi-cab would have to traverse to get from one point to another if the cab was only allowed to move in cardinal directions (north, south, east, west) and not diagonally. As such it is always at least as large as the Euclidean metric, which measures distance “as the crow flies”, as it were. We claim that the space $( \mathbf { R } ^ { n } , d _ { l ^ { 1 } } )$ is also a metric space (Exercise 1.1.7). The metrics are not quite the same, but we do have the inequalities 

$$
d _ {l ^ {2}} (x, y) \leq d _ {l ^ {1}} (x, y) \leq \sqrt {n} d _ {l ^ {2}} (x, y)\tag{1.1}
$$

for all $x , y$ (see Exercise 1.1.8). 

Remark 1.1.8. The taxi-cab metric is useful in several places, for instance in the theory of error correcting codes. A string of n binary digits can be thought of as an element of $\mathbf { R } ^ { n }$ , for instance the binary string 10010 can be thought of as the point $( 1 , 0 , 0 , 1 , 0 )$ in $\mathbf { R } ^ { 5 }$ . The taxi-cab distance between two binary strings is then the number of bits in the two strings which do not match, for instance $d _ { l ^ { 1 } } ( 1 0 0 1 0 , 1 0 1 0 1 ) = 3$ . The goal of error-correcting codes is to encode each piece of information (e.g., a letter of the alphabet) as a binary string in such a way that all the binary strings are as far away in the taxicab metric from each other as possible; this minimizes the chance that any distortion of the bits due to random noise can accidentally change one of the coded binary strings to another, and also maximizes the chance that any such distortion can be detected and correctly repaired. 

Example 1.1.9 (Sup norm metric). Again let $n \geq 1$ , and let $\mathbf { R } ^ { n }$ be as before. But now we use a diferent metric $d _ { l ^ { \infty } }$ , the so-called sup norm metric (or $l ^ { \infty }$ metric), defined by 

$$
d _ {l \infty} ((x _ {1}, x _ {2}, \dots , x _ {n}), (y _ {1}, y _ {2}, \dots , y _ {n})) := \sup \{| x _ {i} - y _ {i} |: 1 \leq i \leq n \}.
$$

Thus for instance, if $n = 2$ , then $d _ { l ^ { \infty } } ( ( 1 , 6 ) , ( 4 , 2 ) ) = \operatorname* { s u p } ( 3 , 4 ) = 4$ . The space $( \mathbf { R } ^ { n } , d _ { l ^ { \infty } } )$ is also a metric space (Exercise 1.1.9), and is related to 

## 1.1. Definitions and examples

the $l ^ { 2 }$ metric by the inequalities 

$$
\frac {1}{\sqrt {n}} d _ {l ^ {2}} (x, y) \leq d _ {l ^ {\infty}} (x, y) \leq d _ {l ^ {2}} (x, y)\tag{1.2}
$$

for all $x , y$ (see Exercise 1.1.10). 

Remark 1.1.10. The $l ^ { 1 } , l ^ { 2 }$ , and $l ^ { \infty }$ metrics are special cases of the more general $l ^ { p }$ metrics, where $p \in [ 1 , + \infty ]$ , but we will not discuss these more general metrics in this text. 

Example 1.1.11 (Discrete metric). Let X be an arbitrary set (finite or infinite), and define the discrete metric $d _ { \mathrm { d i s c } }$ by setting $d _ { \mathrm { d i s c } } ( x , y ) : = 0$ when $x \ : = \ : y .$ , and $d _ { \mathrm { d i s c } } ( x , y ) : = 1$ when $x \neq y .$ . Thus, in this metric, all points are equally far apart. The space $( X , d _ { \mathrm { d i s c } } )$ is a metric space (Exercise 1.1.11). Thus every set X has at least one metric on it. 

Example 1.1.12 (Geodesics). (Informal) Let X be the sphere $\{ ( x , y , z ) \in \mathbf { R } ^ { 3 } : x ^ { 2 } + y ^ { 2 } + z ^ { 2 } = 1 \}$ , and let $d ( ( x , y , z ) , ( x ^ { \prime } , y ^ { \prime } , z ^ { \prime } ) )$ be the length of the shortest curve in X which starts at $( x , y , z )$ and ends at $( x ^ { \prime } , y ^ { \prime } , z ^ { \prime } )$ . (This curve turns out to be an arc of a great circle; we will not prove this here, as it requires calculus of variations, which is beyond the scope of this text.) This makes X into a metric space; the reader should be able to verify (without using any geometry of the sphere) that the triangle inequality is more or less automatic from the definition. 

Example 1.1.13 (Shortest paths). (Informal) Examples of metric spaces occur all the time in real life. For instance, X could be all the computers currently connected to the internet, and $d ( x , y )$ is the shortest number of connections it would take for a packet to travel from computer x to computer $y ;$ for instance, if x and y are not directly connected, but are both connected to $z ,$ then $d ( x , y ) = 2$ . Assuming that all computers in the internet can ultimately be connected to all other computers (so that $d ( x , y )$ is always finite), then $( X , d )$ is a metric space (why?). Games such as “six degrees of separation” are also taking place in a similar metric space (what is the space, and what is the metric, in this case?). $\operatorname { O r } , X$ could be a major city, and $d ( x , y )$ could be the shortest time it takes to drive from x to $y$ (although this space might not satisfy axiom (c) in real life!). 

Now that we have metric spaces, we can define convergence in these spaces. 

Definition 1.1.14 (Convergence of sequences in metric spaces). Let m be an integer, $( X , d )$ be a metric space and let $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ be a sequence of points in X (i.e., for every natural number $n \geq m$ , we assume that $x ^ { ( n ) }$ is an element of X). Let x be a point in X. We say that $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ converges to $x$ with respect to the metric $d ,$ if and only if the limit $\scriptstyle \operatorname* { l i m } _ { n \to \infty } d ( x ^ { ( n ) } , x )$ exists and is equal to 0. In other words, $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ converges to x with respect to d if and only if for every $\varepsilon > 0$ , there exists an $N \geq m$ such that $d ( x ^ { ( n ) } , x ) \leq \varepsilon$ for all $n \geq N$ . (Why are these two definitions equivalent?) 

Remark 1.1.15. In view of Lemma 1.1.1 we see that this definition generalizes our existing notion of convergence of sequences of real numbers. In many cases, it is obvious what the metric d is, and so we shall often just say $^ { 6 6 } ( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ converges to $x '$ instead of $^ { 6 6 } ( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ converges to x with respect to the metric $d ^ { \ast }$ when there is no chance of confusion. We also sometimes write $^ { \mathfrak { s } } x ^ { ( n ) } \to x$ as $n  \infty ^ { \mathfrak { N } }$ instead. 

Remark 1.1.16. There is nothing special about the superscript n in the above definition; it is a dummy variable. Saying that $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ converges to $x$ is exactly the same statement as saying that $( x ^ { ( k ) } ) _ { k = m } ^ { \infty }$ converges to $x ,$ for example; and sometimes it is convenient to change superscripts, for instance if the variable n is already being used for some other purpose. Similarly, it is not necessary for the sequence $x ^ { ( n ) }$ to be denoted using the superscript (n); the above definition is also valid for sequences $x _ { n }$ , or functions $f ( n )$ , or indeed of any expression which depends on n and takes values in X. Finally, from Exercises 6.1.3, 6.1.4 we see that the starting point m of the sequence is unimportant for the purposes of taking limits; if $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ converges to $x ,$ , then $( x ^ { ( n ) } ) _ { n = m ^ { \prime } } ^ { \infty }$ also converges to x for any $m ^ { \prime } \geq m$ 

Example 1.1.17. We work in the Euclidean space $\mathbf { R } ^ { 2 }$ with the standard Euclidean metric $d _ { l ^ { 2 } }$ Let $( x ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ denote the sequence $x ^ { ( n ) } : = ( 1 / n , 1 / n )$ in $\mathbf { R } ^ { 2 }$ , i.e., we are considering the sequence $( 1 , 1 ) , ( 1 / 2 , 1 / 2 ) , ( 1 / 3 , 1 / 3 ) , . . . .$ Then this sequence converges to (0, 0) with respect to the Euclidean metric $d _ { l ^ { 2 } }$ , since 

$$
\lim _ {n \to \infty} d _ {l ^ {2}} (x ^ {(n)}, (0, 0)) = \lim _ {n \to \infty} \sqrt {\frac {1}{n ^ {2}} + \frac {1}{n ^ {2}}} = \lim _ {n \to \infty} \frac {\sqrt {2}}{n} = 0.
$$

The sequence $( x ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ also converges to (0, 0) with respect to the taxicab metric $d _ { l ^ { 1 } }$ , since 

$$
\lim _ {n \to \infty} d _ {l ^ {1}} (x ^ {(n)}, (0, 0)) = \lim _ {n \to \infty} \frac {1}{n} + \frac {1}{n} = \lim _ {n \to \infty} \frac {2}{n} = 0.
$$

## 1.1. Definitions and examples

Similarly the sequence converges to $( 0 , 0 )$ in the sup norm metric $d _ { l ^ { \infty } }$ (why?). However, the sequence $( x ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ does not converge to $( 0 , 0 )$ in the discrete metric $d _ { \mathrm { d i s c } } ,$ , since 

$$
\lim _ {n \to \infty} d _ {\mathrm{disc}} (x ^ {(n)}, (0, 0)) = \lim _ {n \to \infty} 1 = 1 \neq 0.
$$

Thus the convergence of a sequence can depend on what metric one uses<sup>1</sup>. 

In the case of the above four metrics - Euclidean, taxi-cab, sup norm, and discrete - it is in fact rather easy to test for convergence. 

Proposition 1.1.18 (Equivalence of $l ^ { 1 } , l ^ { 2 } , l ^ { \infty } )$ . Let $\mathbf { R } ^ { n }$ be a Euclidean space, and let $( x ^ { ( k ) } ) _ { k = m } ^ { \infty }$ be a sequence of points in $\mathbf { R } ^ { n }$ . We write $x ^ { ( k ) } =$ $( x _ { 1 } ^ { ( k ) } , x _ { 2 } ^ { ( k ) } , \dots , x _ { n } ^ { ( k ) } )$ , i.e., for $j = 1 , 2 , \dotsc , n , \ x _ { j } ^ { ( k ) } \ \in \ \mathbf { R }$ is the $j ^ { t h }$ coordinate of $x ^ { ( k ) } \in \mathbf { R } ^ { n }$ . Let $x = ( x _ { 1 } , \ldots , x _ { n } )$ be a point in $\mathbf { R } ^ { n }$ . Then the following four statements are equivalent: 

(a) $( x ^ { ( k ) } ) _ { k = m } ^ { \infty }$ converges to x with respect to the Euclidean metric $d _ { l ^ { 2 } }$ 

(b) $( x ^ { ( k ) } ) _ { k = m } ^ { \infty }$ converges to x with respect to the taxi-cab metric $d _ { l ^ { 1 } }$ 

(c) $( x ^ { ( k ) } ) _ { k = m } ^ { \infty }$ converges to x with respect to the sup norm metric $d _ { l ^ { \infty } }$ 

(d) For every $1 \ \leq \ j \ \leq \ n$ , the sequence $( x _ { j } ^ { ( k ) } ) _ { k = m } ^ { \infty }$ converges to $x _ { j }$ (Notice that this is a sequence of real numbers, not of points in R<sup>n</sup>.) 

Proof. See Exercise 1.1.12. 

In other words, a sequence converges in the Euclidean, taxi-cab, or sup norm metric if and only if each of its components converges individually. Because of the equivalence of (a), (b) and (c), we say that the Euclidean, taxicab, and sup norm metrics on $\mathbf { R } ^ { n }$ are equivalent. (There are infinite-dimensional analogues of the Euclidean, taxicab, and sup norm metrics which are not equivalent, see for instance Exercise 1.1.15.) 

For the discrete metric, convergence is much rarer: the sequence must be eventually constant in order to converge. 

Proposition 1.1.19 (Convergence in the discrete metric). Let X be any set, and let $d _ { \mathrm { d i s c } }$ be the discrete metric on X. Let $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ be a sequence of points in X, and let x be a point in X. Then $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ converges to x with respect to the discrete metric $d _ { \mathrm { d i s c } }$ if and only if there exists an $N \geq m$ such that $x ^ { ( n ) } = x$ for all $n \geq N$ 

Proof. See Exercise 1.1.13. 

We now prove a basic fact about converging sequences; they can only converge to at most one point at a time. 

Proposition 1.1.20 (Uniqueness of limits). Let $( X , d )$ be a metric space, and let $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ be a sequence in X. Suppose that there are two points $x , x ^ { \prime } \in X$ such that $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ converges to x with respect to $d ,$ and $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ also converges to $x ^ { \prime }$ with respect to d. Then we have $x = x ^ { \prime }$ 

Proof. See Exercise 1.1.14. 

Because of the above Proposition, it is safe to introduce the following notation: if $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ converges to x in the metric $d ,$ then we write $d - \operatorname* { l i m } _ { n \to \infty } x ^ { ( n ) } = x ,$ or simply $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } x ^ { ( n ) } = x } \end{array}$ when there is no confusion as to what d is. For instance, in the example of $\textstyle { \left( { \frac { 1 } { n } } , { \frac { 1 } { n } } \right) }$ , we have 

$$
d _ {l ^ {2}} - \lim _ {n \rightarrow \infty} \left(\frac {1}{n}, \frac {1}{n}\right) = d _ {l ^ {1}} - \lim _ {n \rightarrow \infty} \left(\frac {1}{n}, \frac {1}{n}\right) = (0, 0),
$$

but $\begin{array} { r } { d _ { \mathrm { d i s c } } \ - \ \operatorname* { l i m } _ { n \to \infty } ( { \frac { 1 } { n } } , { \frac { 1 } { n } } ) } \end{array}$ is undefined. Thus the meaning of $d -$ $\scriptstyle \operatorname* { l i m } _ { n \to \infty } x ^ { ( n ) }$ can depend on what d is; however Proposition 1.1.20 assures us that once d is fixed, there can be at most one value of $d - \operatorname* { l i m } _ { n \to \infty } x ^ { ( n ) }$ (Of course, it is still possible that this limit does not exist; some sequences are not convergent.) Note that by Lemma 1.1.1, this definition of limit generalizes the notion of limit in Definition 6.1.8. 

Remark 1.1.21. It is possible for a sequence to converge to one point using one metric, and another point using a diferent metric, although such examples are usually quite artificial. For instance, let $X : = [ 0 , 1 ]$ , the closed interval from 0 to 1. Using the usual metric d, we have $\begin{array} { r } { d - \operatorname* { l i m } _ { n \to \infty } \frac { 1 } { n } = 0 } \end{array}$ . But now suppose we “swap” the points 0 and 1 in the following manner. Let $f : [ 0 , 1 ]  [ 0 , 1 ]$ be the function defined by $f ( 0 ) : = 1 , f ( 1 ) : = 0$ , and $f ( x ) : = x$ for all $x \in ( 0 , 1 )$ , and then define 

## 1.1. Definitions and examples

$d ^ { \prime } ( x , y ) : = d ( f ( x ) , f ( y ) )$ . Then $( X , d ^ { \prime } )$ is still a metric space (why?), but now $\begin{array} { r } { d ^ { \prime } - \operatorname* { l i m } _ { n \to \infty } \frac { 1 } { n } = 1 } \end{array}$ . Thus changing the metric on a space can greatly afect the nature of convergence (also called the topology) on that space; see Section 2.5 for a further discussion of topology. 

## — Exercises —

Exercise 1.1.1. Prove Lemma 1.1.1. 

Exercise 1.1.2. Show that the real line with the metric $d ( x , y ) : = | x - y |$ is indeed a metric space. (Hint: you may wish to review your proof of Proposition 4.3.3.) 

Exercise 1.1.3. Let X be a set, and let $d : X \times X \to [ 0 , \infty )$ be a function. 

(a) Give an example of a pair (X, d) which obeys axioms (bcd) of Definition 1.1.2, but not (a). (Hint: modify the discrete metric.) 

(b) Give an example of a pair (X, d) which obeys axioms (acd) of Definition 1.1.2, but not (b). 

(c) Give an example of a pair (X, d) which obeys axioms (abd) of Definition 1.1.2, but not (c). 

(d) Give an example of a pair (X, d) which obeys axioms (abc) of Definition 1.1.2, but not (d). (Hint: try examples where X is a finite set.) 

Exercise 1.1.4. Show that the pair $( Y , d | _ { Y \times Y } )$ defined in Example 1.1.5 is indeed a metric space. 

Exercise 1.1.5. Let $n \geq 1$ , and let $a _ { 1 } , a _ { 2 } , \ldots , a _ { n }$ and $b _ { 1 } , b _ { 2 } , \ldots , b _ { n }$ be real numbers. Verify the identity 

$$
\left(\sum_ {i = 1} ^ {n} a _ {i} b _ {i}\right) ^ {2} + \frac {1}{2} \sum_ {i = 1} ^ {n} \sum_ {j = 1} ^ {n} (a _ {i} b _ {j} - a _ {j} b _ {i}) ^ {2} = \left(\sum_ {i = 1} ^ {n} a _ {i} ^ {2}\right) \left(\sum_ {j = 1} ^ {n} b _ {j} ^ {2}\right),
$$

and conclude the Cauchy-Schwarz inequality 

$$
\left| \sum_ {i = 1} ^ {n} a _ {i} b _ {i} \right| \leq \left(\sum_ {i = 1} ^ {n} a _ {i} ^ {2}\right) ^ {1 / 2} \left(\sum_ {j = 1} ^ {n} b _ {j} ^ {2}\right) ^ {1 / 2}.\tag{1.3}
$$

Then use the Cauchy-Schwarz inequality to prove the triangle inequality 

$$
\left(\sum_ {i = 1} ^ {n} \left(a _ {i} + b _ {i}\right) ^ {2}\right) ^ {1 / 2} \leq \left(\sum_ {i = 1} ^ {n} a _ {i} ^ {2}\right) ^ {1 / 2} + \left(\sum_ {j = 1} ^ {n} b _ {j} ^ {2}\right) ^ {1 / 2}.
$$

Exercise 1.1.6. Show that $( \mathbf { R } ^ { n } , d _ { l ^ { 2 } } )$ in Example 1.1.6 is indeed a metric space. (Hint: use Exercise 1.1.5.) 

Exercise 1.1.7. Show that the pair $( \mathbf { R } ^ { n } , d _ { l ^ { 1 } } )$ in Example 1.1.7 is indeed a metric space. 

Exercise 1.1.8. Prove the two inequalities in (1.1). (For the first inequality, square both sides. For the second inequality, use Exercise (1.1.5). 

Exercise 1.1.9. Show that the pair $( \mathbf { R } ^ { n } , d _ { l ^ { \infty } } )$ in Example 1.1.9 is indeed a metric space. 

Exercise 1.1.10. Prove the two inequalities in (1.2). 

Exercise 1.1.11. Show that the discrete metric $\left( \mathbf { R } ^ { n } , d _ { \mathrm { d i s c } } \right)$ in Example 1.1.11 is indeed a metric space. 

Exercise 1.1.12. Prove Proposition 1.1.18. 

Exercise 1.1.13. Prove Proposition 1.1.19. 

Exercise 1.1.14. Prove Proposition 1.1.20. (Hint: modify the proof of Proposition 6.1.7.) 

Exercise 1.1.15. Let 

$$
X := \left\{(a _ {n}) _ {n = 0} ^ {\infty}: \sum_ {n = 0} ^ {\infty} | a _ {n} | <   \infty \right\}
$$

be the space of absolutely convergent sequences. Define the $l ^ { 1 }$ and $l ^ { \infty }$ metrics on this space by 

$$
d _ {l ^ {1}} \big ((a _ {n}) _ {n = 0} ^ {\infty}, (b _ {n}) _ {n = 0} ^ {\infty} \big) := \sum_ {n = 0} ^ {\infty} | a _ {n} - b _ {n} |;
$$

$$
d _ {l ^ {\infty}} ((a _ {n}) _ {n = 0} ^ {\infty}, (b _ {n}) _ {n = 0} ^ {\infty}) := \sup _ {n \in \mathbf {N}} | a _ {n} - b _ {n} |.
$$

Show that these are both metrics on $X$ , but show that there exist sequences $x ^ { ( 1 ) } , x ^ { ( 2 ) } , . . .$ . of elements of X (i.e., sequences of sequences) which are convergent with respect to the $d _ { l ^ { \infty } }$ metric but not with respect to the $d _ { l ^ { 1 } }$ metric. Conversely, show that any sequence which converges in the $d _ { l ^ { 1 } }$ metric automatically converges in the $d _ { l ^ { \infty } }$ metric. 

Exercise 1.1.16. Let $( x _ { n } ) _ { n = 1 } ^ { \infty }$ and $( y _ { n } ) _ { n = 1 } ^ { \infty }$ be two sequences in a metric space $( X , d )$ . Suppose that $( x _ { n } ) _ { n = 1 } ^ { \infty }$ converges to a point $x \in X$ , and $( y _ { n } ) _ { n = 1 } ^ { \infty }$ converges to a point $y \in X$ . Show that $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } d ( x _ { n } , y _ { n } ) = d ( x , y ) } \end{array}$ . (Hint: use the triangle inequality several times.) 

## 1.2 Some point-set topology of metric spaces

Having defined the operation of convergence on metric spaces, we now define a couple other related notions, including that of open set, closed set, interior, exterior, boundary, and adherent point. The study of such notions is known as point-set topology, which we shall return to in Section 2.5. 

We first need the notion of a metric ball, or more simply a ball. 

Definition 1.2.1 (Balls). Let $( X , d )$ be a metric space, let $x _ { 0 }$ be a point in $X$ , and let $r > 0$ . We define the ball $B _ { ( X , d ) } ( x _ { 0 } , r )$ in $X$ , centered at $x _ { 0 }$ , and with radius $r _ { \mathrm { : } }$ , in the metric $d ,$ to be the set 

$$
B _ {(X, d)} (x _ {0}, r) := \{x \in X: d (x, x _ {0}) <   r \}.
$$

When it is clear what the metric space $( X , d )$ is, we shall abbreviate $B _ { ( X , d ) } ( x _ { 0 } , r )$ as just $B ( x _ { 0 } , r )$ 

Example 1.2.2. In $\mathbf { R } ^ { 2 }$ with the Euclidean metric $d _ { l ^ { 2 } }$ , the ball $B _ { ( \mathbf { R } ^ { 2 } , d _ { l ^ { 2 } } ) } ( ( 0 , 0 ) , 1 )$ is the open disc 

$$
B _ {(\mathbf {R} ^ {2}, d _ {l 2})} ((0, 0), 1) = \{(x, y) \in \mathbf {R} ^ {2}: x ^ {2} + y ^ {2} <   1 \}.
$$

However, if one uses the taxi-cab metric $d _ { l ^ { 1 } }$ instead, then we obtain a diamond: 

$$
B _ {(\mathbf {R} ^ {2}, d _ {l 1})} ((0, 0), 1) = \{(x, y) \in \mathbf {R} ^ {2}: | x | + | y | <   1 \}.
$$

If we use the discrete metric, the ball is now reduced to a single point: 

$$
B _ {(\mathbf {R} ^ {2}, d _ {\mathrm{disc}})} ((0, 0), 1) = \{(0, 0) \},
$$

although if one increases the radius to be larger than 1, then the bal now encompasses all of $\mathbf { R } ^ { 2 }$ . (Why?) 

Example 1.2.3. In R with the usual metric $d ,$ the open interval $( 3 , 7 )$ is also the metric bal $B _ { ( \mathbf { R } , d ) } ( 5 , 2 )$ 

Remark 1.2.4. Note that the smaller the radius $^ { r , }$ the smaller the ball $B ( x _ { 0 } , r )$ . However, $B ( x _ { 0 } , r )$ always contains at least one point, namely the center $x _ { 0 }$ , as long as $r$ stays positive, thanks to Definition 1.1.2(a). (We don’t consider balls of zero radius or negative radius since they are rather boring, being just the empty set.) 

Using metric balls, one can now take a set $E$ in a metric space $X$ and classify three types of points in $X$ : interior, exterior, and boundary points of $E$ 

Definition 1.2.5 (Interior, exterior, boundary). Let $( X , d )$ be a metric space, let $E$ be a subset of $X ,$ and let $x _ { 0 }$ be a point in X. We say that $x _ { 0 }$ is an interior point of E if there exists a radius $r > 0$ such that $B ( x _ { 0 } , r ) \subseteq E$ . We say that $x _ { 0 }$ is an exterior point of E if there exists a radius $r > 0$ such that $B ( x _ { 0 } , r ) \cap E = \varnothing$ . We say that $x _ { 0 }$ is a boundary point of E if it is neither an interior point nor an exterior point of $E$ 

The set of all interior points of $E$ is called the interior of $E$ and is sometimes denoted int $( E )$ . The set of exterior points of $E$ is called the exterior of $E$ and is sometimes denoted $\operatorname { e x t } ( E )$ . The set of boundary points of $E$ is called the boundary of E and is sometimes denoted $\partial E$ 

Remark 1.2.6. If $x _ { 0 }$ is an interior point of $E ,$ , then $x _ { 0 }$ must actually be an element of $E ,$ since balls $B ( x _ { 0 } , r )$ always contain their center $x _ { 0 }$ Conversely, if $x _ { 0 }$ is an exterior point of $E$ , then $x _ { 0 }$ cannot be an element of $E .$ . In particular it is not possible for $x _ { 0 }$ to simultaneously be an interior and an exterior point of $E .$ . If $x _ { 0 }$ is a boundary point of $E _ { \mathrm { { i } } }$ , then it could be an element of $E _ { \mathrm { { i } } }$ but it could also not lie in $E ;$ we give some examples below. 

Example 1.2.7. We work on the real line R with the standard metric $d .$ Let E be the half-open interval $E = [ 1 , 2 )$ . The point 1.5 is an interior point of $E ,$ since one can find a ball (for instance $B ( 1 . 5 , 0 . 1 ) )$ centered at 1.5 which lies in $E .$ . The point 3 is an exterior point of $E ,$ since one can find a ball (for instance $B ( 3 , 0 . 1 ) )$ centered at 3 which is disjoint from $E .$ . The points 1 and 2 however, are neither interior points nor exterior points of $E _ { i }$ , and are thus boundary points of $E .$ . Thus in this case int $( E ) = ( 1 , 2 )$ , ext $\left( E \right) = \left( - \infty , 1 \right) \cup \left( 2 , \infty \right)$ , and $\partial E = \{ 1 , 2 \}$ . Note that in this case one of the boundary points is an element of $E$ , while the other is not. 

Example 1.2.8. When we give a set X the discrete metric $d _ { \mathrm { d i s c } }$ , and $E$ is any subset of $X$ , then every element of $E$ is an interior point of $E _ { i }$ every point not contained in $E$ is an exterior point of $E$ , and there are no boundary points; see Exercise 1.2.1. 

Definition 1.2.9 (Closure). Let $( X , d )$ be a metric space, let $E$ be a subset of $X$ , and let $x _ { 0 }$ be a point in $X$ . We say that $x _ { 0 }$ is an adherent point of $E$ if for every radius $r > 0$ , the ball $B ( x _ { 0 } , r )$ has a non-empty intersection with E. The set of all adherent points of $E$ is called the closure of E and is denoted $\overline { E }$ 

Note that these notions are consistent with the corresponding notions on the real line defined in Definitions 9.1.8, 9.1.10 $\mathrm { ( w h y ? ) }$ 

The following proposition links the notions of adherent point with interior and boundary point, and also to that of convergence. 

Proposition 1.2.10. Let $( X , d )$ be a metric space, let E be a subset of X, and let x<sub>0</sub> be a point in X. Then the following statements are logically equivalent. 

(a) $x _ { 0 }$ is an adherent point of E. 

(b) $x _ { 0 }$ is either an interior point or a boundary point of E. 

(c) There exists a sequence $( x _ { n } ) _ { n = 1 } ^ { \infty }$ in $E$ which converges to $x _ { 0 }$ with respect to the metric d. 

Proof. See Exercise 1.2.2. 

From the equivalence of Proposition 1.2.10(a) and (b) we obtain an immediate corollary: 

Corollary 1.2.11. Let $( X , d )$ be a metric space, and let E be a subset of X. Then ${ \overline { { E } } } = \operatorname { i n t } ( E ) \cup \partial E = X \backslash \operatorname { e x t } ( E )$ 

As remarked earlier, the boundary of a set E may or may not lie in E. Depending on how the boundary is situated, we may call a set open, closed, or neither: 

Definition 1.2.12 (Open and closed sets). Let $( X , d )$ be a metric space, and let E be a subset of X. We say that E is closed if it contains all of its boundary points, i.e., $\partial E \subseteq E$ . We say that E is open if it contains none of its boundary points, i.e., $\partial E \cap E = \emptyset$ . If E contains some of its boundary points but not others, then it is neither open nor closed. 

Example 1.2.13. We work in the real line R with the standard metric d. The set (1, 2) does not contain either of its boundary points 1, 2 and is hence open. The set [1, 2] contains both of its boundary points 1, 2 and is hence closed. The set [1, 2) contains one of its boundary points 1, but does not contain the other boundary point 2, so is neither open nor closed. 

Remark 1.2.14. It is possible for a set to be simultaneously open and closed, if it has no boundary. For instance, in a metric space $( X , d )$ , the whole space X has no boundary (every point in X is an interior point - why?), and so X is both open and closed. The empty set also has no boundary (every point in X is an exterior point - why?), and so is both open and closed. In many cases these are the only sets that are simultaneously open and closed, but there are exceptions. For instance, using the discrete metric $d _ { \mathrm { d i s c } }$ , every set is both open and closed! (why?) 

From the above two remarks we see that the notions of being open and being closed are not negations of each other; there are sets that are both open and closed, and there are sets which are neither open nor closed. Thus, if one knew for instance that E was not an open set, it would be erroneous to conclude from this that E was a closed set, and similarly with the rˆoles of open and closed reversed. The correct relationship between open and closed sets is given by Proposition 1.2.15(e) below. 

Now we list some more properties of open and closed sets. 

Proposition 1.2.15 (Basic properties of open and closed sets). Let $( X , d )$ be a metric space. 

(a) Let E be a subset of X. Then E is open if and only if $E = \operatorname { i n t } ( E )$ In other words, E is open if and only if for every $x \in E$ , there exists an $r > 0$ such that $B ( x , r ) \subseteq E$ 

(b) Let E be a subset of X. Then E is closed if and only if E contains all its adherent points. In other words, E is closed if and only if for every convergent sequence $( x _ { n } ) _ { n = m } ^ { \infty }$ in E, the limit $\scriptstyle \operatorname* { l i m } _ { n \to \infty } x _ { n }$ of that sequence also lies in E. 

(c) For any $x _ { 0 } ~ \in ~ X$ and $r \ > \ 0$ , then the ball $B ( x _ { 0 } , r )$ is an open set. The set $\{ x \in X : d ( x , x _ { 0 } ) \leq r \}$ is a closed set. (This set is sometimes called the closed ball of radius r centered at $x _ { 0 } . \big )$ 

(d) Any singleton set $\{ x _ { 0 } \}$ , where $x _ { 0 } \in X$ , is automatically closed. 

(e) If E is a subset of X, then E is open if and only if the complement $X \backslash E : = \{ x \in X : x \not \in E \}$ is closed. 

(f ) If $E _ { 1 } , \ldots , E _ { n }$ are a finite collection of open sets in X, then $E _ { 1 } \cap$ $E _ { 2 } \cap \ldots \cap E _ { n }$ is also open. If $F _ { 1 } , \ldots , F _ { n }$ is a finite collection of closed sets in X, then $F _ { 1 } \cup F _ { 2 } \cup . . . \cup F _ { n }$ is also closed. 

(g) If $\{ E _ { \alpha } \} _ { \alpha \in I }$ is a collection of open sets in X (where the index set I could be finite, countable, or uncountable), then the union $\textstyle \bigcup _ { \alpha \in I } E _ { \alpha } : = \{ x \in X : x \in E _ { \alpha }$ for some $\alpha \in I \}$ is also open. If $\{ F _ { \alpha } \} _ { \alpha \in I }$ is a collection of closed sets in X, then the intersection $\bigcap _ { \alpha \in I } F _ { \alpha } : = \{ x \in X : x \in F _ { \alpha }$ for all $\alpha \in I \}$ is also closed. 

(h) If E is any subset of X, then int(E) is the largest open set which is contained in E; in other words, int(E) is open, and given any 

## 1.3. Relative topology

other open set $V \subseteq E$ , we have $V \subseteq \operatorname { i n t } ( E )$ . Similarly $\overline { E }$ is $t h e$ smallest closed set which contains $E ;$ in other words, $\overline { E }$ is closed, and given any other closed set $K \supset E , K \supset { \overline { { E } } }$ 

Proof. See Exercise 1.2.3. 

— Exercises — 

Exercise 1.2.1. Verify the claims in Example 1.2.8. 

Exercise 1.2.2. Prove Proposition 1.2.10. (Hint: for some of the implications one will need the axiom of choice, as in Lemma 8.4.5.) 

Exercise 1.2.3. Prove Proposition 1.2.15. (Hint: you can use earlier parts of the proposition to prove later ones.) 

Exercise 1.2.4. Let $( X , d )$ be a metric space, x<sub>0</sub> be a point in $X$ , and $r > 0$ Let B be the open ball $B : = B ( x _ { 0 } , r ) = \{ x \in X : d ( x , x _ { 0 } ) < r \}$ , and let C be the closed ball $C : = \{ x \in X : d ( x , x _ { 0 } ) \leq r \}$ 

(a) Show that ${ \overline { { B } } } \subseteq C $ 

(b) Give an example of a metric space $( X , d )$ , a point $x _ { 0 }$ , and a radius $r > 0$ such that B is not equal to C. 

## 1.3 Relative topology

When we defined notions such as open and closed sets, we mentioned that such concepts depended on the choice of metric one uses. For instance, on the real line R, if one uses the usual metric $d ( x , y ) = | x - y |$ • then the set 1 is not open, however if instead one uses the discrete metric $d _ { \mathrm { d i s c } }$ , then 1 is now an open set (why?). 

However, it is not just the choice of metric which determines what is open and what is not - it is also the choice of ambient space X. Here are some examples. 

Example 1.3.1. Consider the plane $\mathbf { R } ^ { 2 }$ with the Euclidean metric $d _ { l ^ { 2 } }$ Inside the plane, we can find the x-axis $X : = \{ ( x , 0 ) : x \in \mathbf { R } \}$ The metric $d _ { l ^ { 2 } }$ can be restricted to X, creating a subspace $\left( X , d _ { l ^ { 2 } } | _ { X \times X } \right)$ of $( \mathbf { R } ^ { 2 } , d _ { l ^ { 2 } } )$ . (This subspace is essentially the same as the real line $( \mathbf { R } , d )$ with the usual metric; the precise way of stating this is that $\left( X , d _ { l ^ { 2 } } | _ { X \times X } \right)$ is isometric to $( \mathbf { R } , d )$ . We will not pursue this concept further in this text, however.) Now consider the set 

$$
E := \{(x, 0): - 1 <   x <   1 \}
$$

which is both a subset of X and of $\mathbf { R } ^ { 2 }$ . Viewed as a subset of $\mathbf { R } ^ { 2 }$ , it is not open, because the point 0, for instance, lies in E but is not an interior point of E. (Any ball $B _ { \mathbf { R } ^ { 2 } , d _ { l ^ { 2 } } } ( 0 , r )$ will contain at least one point that lies outside of the x-axis, and hence outside of E. On the other hand, if viewed as a subset of X, it is open; every point of E is an interior point of $E$ with respect to the metric space $\left( X , d _ { l ^ { 2 } } | _ { X \times X } \right)$ . For instance, the point 0 is now an interior point of E, because the ball $B _ { X , d _ { l ^ { 2 } } | _ { X \times X } } ( 0 , 1 )$ is contained in E (in fact, in this case it is E.) 

Example 1.3.2. Consider the real line R with the standard metric $d ,$ and let X be the interval $X : = ( - 1 , 1 )$ contained inside $\mathbf { R } ;$ ; we can then restrict the metric d to X, creating a subspace $( X , d | _ { X \times X } )$ of $( \mathbf { R } , d )$ Now consider the set [0, 1). This set is not closed in R, because the point 1 is adherent to [0, 1) but is not contained in [0, 1). However, when considered as a subset of X, the set [0, 1) now becomes closed; the point 1 is not an element of X and so is no longer considered an adherent point of [0, 1), and so now [0, 1) contains all of its adherent points. 

To clarify this distinction, we make a definition. 

Definition 1.3.3 (Relative topology). Let $( X , d )$ be a metric space, let Y be a subset of X, and let $E$ be a subset of Y. We say that $E$ is relatively open with respect to Y if it is open in the metric subspace $( Y , d | _ { Y \times Y } )$ . Similarly, we say that E is relatively closed with respect to Y if it is closed in the metric space $( Y , d | _ { Y \times Y } )$ 

The relationship between open (or closed) sets in X, and relatively open (or relatively closed) sets in Y, is the following. 

Proposition 1.3.4. Let $( X , d )$ be a metric space, let Y be a subset of X, and let E be a subset of Y. 

(a) E is relatively open with respect to Y if and only if $E = V \cap Y$ for some set $V \subseteq X$ which is open in X. 

(b) E is relatively closed with respect to Y if and only if $E = K \cap Y$ for some set $K \subseteq X$ which is closed in X. 

Proof. We just prove (a), and leave (b) to Exercise 1.3.1. First suppose that E is relatively open with respect to Y. Then, E is open in the metric space $( Y , d | _ { Y \times Y } )$ . Thus, for every $x \in E$ , there exists a radius $r > 0$ such that the ball $B _ { ( Y , d | _ { Y \times Y } ) } ( x , r )$ is contained in $E$ . This radius r depends on $x ;$ to emphasize this we write $r _ { x }$ instead of $^ { r , }$ thus for every $x \in E$ the ball $B _ { ( Y , d | _ { Y \times Y } ) } ( x , r _ { x } )$ is contained in $E .$ . (Note that we have used the axiom of choice, Proposition 8.4.7, to do this.) 

Now consider the set 

$$
V := \bigcup_ {x \in E} B _ {(X, d)} (x, r _ {x}).
$$

This is a subset of X. By Proposition 1.2.15(c) and (g), V is open. Now we prove that $E = V \cap Y$ . Certainly any point $x$ in E lies in $V \cap Y$ 4 since it lies in Y and it also lies in $B _ { ( X , d ) } ( x , r _ { x } )$ , and hence in V. Now suppose that $y$ is a point in $V \cap Y$ . Then $y \in V$ , which implies that there exists an $x \in E$ such that $y \in B _ { ( X , d ) } ( x , r _ { x } )$ . But since $y$ is also in $Y$ , this implies that $y \in B _ { ( Y , d | _ { Y \times Y } ) } ( x , r _ { x } )$ . But by definition of $r _ { x } ,$ , this means that $y \in E$ , as desired. Thus we have found an open set $V$ for which $E = V \cap Y$ as desired. 

Now we do the converse. Suppose that $E = V \cap Y$ for some open set $V ;$ we have to show that E is relatively open with respect to $Y$ . Let x be any point in $E ;$ ; we have to show that x is an interior point of $E$ in the metric space $( Y , d | _ { Y \times Y } )$ . Since $x \in E$ , we know $x \in V$ . Since V is open in $X .$ , we know that there is a radius $r > 0$ such that $B _ { ( X , d ) } ( x , r )$ is contained in $V .$ . Strictly speaking, r depends on $x ,$ , and so we could write $r _ { x }$ instead of $^ { r , }$ but for this argument we will only use a single choice of $x$ (as opposed to the argument in the previous paragraph) and so we will not bother to subscript r here. Since $E = V \cap Y$ , this means that $B _ { ( X , d ) } ( x , r ) \cap Y$ is contained in E. But $B _ { ( X , d ) } ( x , r ) \cap Y$ is exactly the same as $B _ { ( Y , d | _ { Y \times Y } ) } ( x , r ) ~ ( \mathrm { w h y ? } )$ , and so $B _ { ( Y , d | _ { Y \times Y } ) } ( x , r )$ is contained in $E$ . Thus x is an interior point of $E$ in the metric space $( Y , d | _ { Y \times Y } )$ , as desired. □ 

— Exercises — 

Exercise 1.3.1. Prove Proposition 1.3.4(b). 

## 1.4 Cauchy sequences and complete metric spaces

We now generalize much of the theory of limits of sequences from Chapter $6$ to the setting of general metric spaces. We begin by generalizing the notion of a subsequence from Definition 6.6.1: 

Definition 1.4.1 (Subsequences). Suppose that $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ is a sequence of points in a metric space $( X , d )$ . Suppose that $n _ { 1 } , n _ { 2 } , n _ { 3 } , . . . .$ is an increasing sequence of integers which are at least as large as m, thus 

$$
m \leq n _ {1} <   n _ {2} <   n _ {3} <   \dots .
$$

Then we call the sequence $( x ^ { ( n _ { j } ) } ) _ { j = 1 } ^ { \infty }$ a subsequence of the original sequence $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ 

Examples 1.4.2. the sequence $\textstyle \big ( \big ( \frac { 1 } { j ^ { 2 } } , \frac { 1 } { j ^ { 2 } } \big ) \big ) _ { j = 1 } ^ { \infty }$ in $\mathbf { R } ^ { 2 }$ is a subsequence of the sequence $\textstyle { \bigl ( } { \bigl ( } { \frac { 1 } { n } } , { \frac { 1 } { n } } { \bigr ) } { \bigr ) } _ { n = 1 } ^ { \infty }$ (in this case, $n _ { j } : = j ^ { 2 } )$ . The sequence $1 , 1 , 1 , 1 , \ldots$ is a subsequence of 1, 0, 1, 0, 1, . . .. 

If a sequence converges, then so do all of its subsequences: 

Lemma 1.4.3. Let $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ be a sequence in $( X , d )$ which converges to some limit $x _ { 0 }$ . Then every subsequence $( x ^ { ( n _ { j } ) } ) _ { j = 1 } ^ { \infty }$ of that sequence also converges to $x _ { 0 }$ . 

Proof. See Exercise 1.4.3. 

On the other hand, it is possible for a subsequence to be convergent without the sequence as a whole being convergent. For example, the sequence $1 , 0 , 1 , 0 , 1 , \ldots$ is not convergent, even though certain subsequences of it (such as $1 , 1 , 1 , \ldots )$ converge. To quantify this phenomenon, we generalize Definition 6.4.1 as follows: 

Definition 1.4.4 (Limit points). Suppose that $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ is a sequence of points in a metric space $( X , d )$ , and let $L \in X$ . We say that L is a limit point of $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ if for every $N \geq m$ and $\varepsilon > 0$ there exists an $n \geq N$ such that $d ( x ^ { ( n ) } , L ) \leq \varepsilon$ 

Proposition 1.4.5. Let $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ be a sequence of points in a metric space $( X , d )$ , and let $L \in X$ . Then the following are equivalent: 

L is a limit point of $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ 

There exists a subsequence $( x ^ { ( n _ { j } ) } ) _ { j = 1 } ^ { \infty }$ of the original sequence $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ which converges to L. 

Proof. See Exercise 1.4.2. 

Next, we review the notion of a Cauchy sequence from Definition 6.1.3 (see also Definition 5.1.8). 

Definition 1.4.6 (Cauchy sequences). Let $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ be a sequence of points in a metric space $( X , d )$ . We say that this sequence is a Cauchy sequence if for every $\varepsilon > 0$ , there exists an $N \geq m$ such that $d ( x ^ { ( j ) } , x ^ { ( k ) } ) < \varepsilon$ for all $j , k \geq N$ 

Lemma 1.4.7 (Convergent sequences are Cauchy sequences). Let $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ be a sequence in $( X , d )$ which converges to some limit $x _ { 0 }$ . Then $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ is also a Cauchy sequence. 

Proof. See Exercise 1.4.3. 

It is also easy to check that subsequence of a Cauchy sequence is also a Cauchy sequence (why)? However, not every Cauchy sequence converges: 

Example 1.4.8. (Informal) Consider the sequence 

3, 3.1, 3.14, 3.141, 3.1415, . . . 

in the metric space $( \mathbf { Q } , d )$ (the rationals Q with the usual metric $d ( x , y ) : = | x - y | )$ . While this sequence is convergent in R (it converges to π), it does not converge in Q (since $\pi \not \in \mathbf { Q }$ , and a sequence cannot converge to two diferent limits). 

So in certain metric spaces, Cauchy sequences do not necessarily converge. However, if even part of a Cauchy sequence converges, then the entire Cauchy sequence must converge (to the same limit): 

Lemma 1.4.9. Let $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ be a Cauchy sequence in $( X , d )$ . Suppose that there is some subsequence $( x ^ { ( n _ { j } ) } ) _ { j = 1 } ^ { \infty }$ of this sequence which converges to a limit x<sub>0</sub> in X. Then the original sequence $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ also converges to $x _ { 0 }$ 

Proof. See Exercise 1.4.4. 

In Example 1.4.8 we saw an example of a metric space which contained Cauchy sequences which did not converge. However, in Theorem 6.4.18 we saw that in the metric space $( \mathbf { R } , d )$ , every Cauchy sequence did have a limit. This motivates the following definition. 

Definition 1.4.10 (Complete metric spaces). A metric space $( X , d )$ is said to be complete if every Cauchy sequence in $( X , d )$ is in fact convergent in $( X , d )$ 

Example 1.4.11. By Theorem 6.4.18, the reals $( \mathbf { R } , d )$ are complete; by Example 1.4.8, the rationals $( \mathbf { Q } , d )$ , on the other hand, are not complete. 

Complete metric spaces have some nice properties. For instance, they are intrinsically closed: no matter what space one places them in, they are always closed sets. More precisely: 

Proposition 1.4.12. (a) Let $( X , d )$ be a metric space, and let $( Y , d | _ { Y \times Y } )$ be a subspace of (X, d). $I f \left( Y , d | _ { Y \times Y } \right)$ is complete, then Y must be closed in X. 

(b) Conversely, suppose that $( X , d )$ is a complete metric space, and Y is a closed subset of X. Then the subspace $( Y , d | _ { Y \times Y } )$ is also complete. 

Proof. See Exercise 1.4.7. 

In contrast, an incomplete metric space such as $( \mathbf { Q } , d )$ may be considered closed in some spaces (for instance, Q is closed in Q) but not in others (for instance, Q is not closed in R). Indeed, it turns out that given any incomplete metric space $( X , d )$ , there exists a completion $( \overline { { X } } , \overline { { d } } )$ , which is a larger metric space containing $( X , d )$ which is complete, and such that X is not closed in X (indeed, the closure of X in $( \overline { { X } } , \overline { { d } } )$ will be all of $\overline { { \boldsymbol X } } )$ ; see Exercise 1.4.8. For instance, one possible completion of Q is R. 

## — Exercises —



Exercise 1.4.1. Prove Lemma 1.4.3. (Hint: review your proof of Proposition 6.6.5.) 





Exercise 1.4.2. Prove Proposition 1.4.5. (Hint: review your proof of Proposition 6.6.6.) 





Exercise 1.4.3. Prove Lemma 1.4.7. (Hint: review your proof of Proposition 6.1.12.) 





Exercise 1.4.4. Prove Lemma 1.4.9. 



Exercise 1.4.5. Let $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ be a sequence of points in a metric space $( X , d )$ , and let $L \in X$ . Show that if L is a limit point of the sequence $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ , then L is an adherent point of the set $\{ x ^ { ( n ) } : { \bar { n } } \geq m \}$ . Is the converse true? 

Exercise 1.4.6. Show that every Cauchy sequence can have at most one limit point. 



Exercise 1.4.7. Prove Proposition 1.4.12. 



## 1.5. Compact metric spaces

Exercise 1.4.8. The following construction generalizes the construction of the reals from the rationals in Chapter 5, allowing one to view any metric space as a subspace of a complete metric space. In what follows we let $( X , d )$ be a metric space. 

(a) Given any Cauchy sequence $( x _ { n } ) _ { n = 1 } ^ { \infty }$ in X, we introduce the formal limit $\mathrm { L I M } _ { n \to \infty } x _ { n }$ . We say that two formal limits $\mathrm { L I M } _ { n \to \infty } x _ { n }$ and $\operatorname { L I M } _ { n \to \infty } y _ { n }$ are equal if $\scriptstyle \operatorname* { l i m } _ { n \to \infty } d ( x _ { n } , y _ { n } )$ is equal to zero. Show that this equality relation obeys the reflexive, symmetry, and transitive axioms. 

(b) Let X be the space of all formal limits of Cauchy sequences in X, with the above equality relation. Define a metric $d _ { \overline { { X } } } : \dot { \overline { { X } } } \times \bar { \overline { { X } } }  \mathbf { R } ^ { + }$ by setting 

$$
d _ {\overline {{X}}} (\mathrm{LIM} _ {n \to \infty}   x _ {n}, \mathrm{LIM} _ {n \to \infty}   y _ {n}) := \lim _ {n \to \infty} d (x _ {n}, y _ {n}).
$$

Show that this function is well-defined (this means not only that the limit $\scriptstyle \operatorname* { l i m } _ { n \to \infty } d ( x _ { n } , y _ { n } )$ exists, but also that the axiom of substitution is obeyed; cf. Lemma 5.3.7), and gives X the structure of a metric space. 

(c) Show that the metric space $( { \overline { { X } } } , d _ { \overline { { X } } } )$ is complete. 

(d) We identify an element $x \in X$ with the corresponding formal limit $\mathrm { L I M } _ { n \to \infty } x$ in ${ \overline { { X } } } ;$ show that this is legitimate by verifying that $x =$ $y \iff \operatorname { L I M } _ { n \to \infty } x = \operatorname { L I M } _ { n \to \infty } y$ . With this identification, show that $d ( x , y ) = d _ { \overline { { X } } } ( x , y )$ , and thus $( X , d )$ can now be thought of as a subspace of $( { \overline { { X } } } , d _ { \overline { { X } } } )$ 

(e) Show that the closure of X in X is X (which explains the choice of notation X). 

(f) Show that the formal limit agrees with the actual limit, thus if $( x _ { n } ) _ { n = 1 } ^ { \infty }$ is any Cauchy sequence in X, then we have $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } x _ { n } = \mathrm { L I M } _ { n \to \infty } x _ { n } } \end{array}$ in X. 

## 1.5 Compact metric spaces

We now come to one of the most useful notions in point set topology, that of compactness. Recall the Heine-Borel theorem (Theorem 9.1.24), which asserted that every sequence in a closed and bounded subset X of the real line R had a convergent subsequence whose limit was also in X. Conversely, only the closed and bounded sets have this property. This property turns out to be so useful that we give it a name. 

Definition 1.5.1 (Compactness). A metric space $( X , d )$ is said to be compact if every sequence in $( X , d )$ has at least one convergent subsequence. A subset Y of a metric space X is said to be compact if the subspace $( Y , d | _ { Y \times Y } )$ is compact. 

Remark 1.5.2. The notion of a set Y being compact is intrinsic, in the sense that it only depends on the metric function $d | _ { Y \times Y }$ restricted to Y, and not on the choice of the ambient space X. The notions of completeness in Definition 1.4.10, and of boundedness below in Definition 1.5.3, are also intrinsic, but the notions of open and closed are not (see the discussion in Section 1.3). 

Thus, Theorem 9.1.24 shows that in the real line R with the usual metric, every closed and bounded set is compact, and conversely every compact set is closed and bounded. 

Now we investigate how the Heine-Borel extends to other metric spaces. 

Definition 1.5.3 (Bounded sets). Let $( X , d )$ be a metric space, and let Y be a subset of X. We say that Y is bounded if there exists a ball $B ( x , r )$ in X which contains Y. 

Remark 1.5.4. This definition is compatible with the definition of a bounded set in Definition 9.1.22 (Exercise 1.5.1). 

Proposition 1.5.5. Let $( X , d )$ be a compact metric space. Then $( X , d )$ is both complete and bounded. 

Proof. See Exercise 1.5.2. 

From this proposition and Proposition 1.4.12(a) we obtain one half of the Heine-Borel theorem for general metric spaces: 

Corollary 1.5.6 (Compact sets are closed and bounded). Let $( X , d )$ be a metric space, and let Y be a compact subset of X. Then Y is closed and bounded. 

The other half of the Heine-Borel theorem is true in Euclidean spaces: 

Theorem 1.5.7 (Heine-Borel theorem). Let $( \mathbf { R } ^ { n } , d )$ be a Euclidean space with either the Euclidean metric, the taxicab metric, or the sup norm metric. Let E be a subset of $\mathbf { R } ^ { n }$ . Then E is compact if and only if it is closed and bounded. 

Proof. See Exercise 1.5.3. 

However, the Heine-Borel theorem is not true for more general metrics. For instance, the integers Z with the discrete metric is closed (indeed, it is complete) and bounded, but not compact, since the sequence 

1, 2, 3, 4, . . . is in Z but has no convergent subsequence $\mathrm { \left( w h y ? \right) }$ . Another example is in Exercise 1.5.8. However, a version of the Heine-Borel theorem is available if one is willing to replace closedness with the stronger notion of completeness, and boundedness with the stronger notion of total boundedness; see Exercise 1.5.10. 

One can characterize compactness topologically via the following, rather strange-sounding statement: every open cover of a compact set has a finite subcover. 

Theorem 1.5.8. Let $( X , d )$ be a metric space, and let Y be a compact subset of X. Let $( V _ { \alpha } ) _ { \alpha \in I }$ be a collection of open sets in X, and suppose that 

$$
Y \subseteq \bigcup_ {\alpha \in I} V _ {\alpha}.
$$

$( i . e .$ , the collection $( V _ { \alpha } ) _ { \alpha \in I }$ covers Y). Then there exists a finite subset F of I such that 

$$
Y \subseteq \bigcup_ {\alpha \in F} V _ {\alpha}.
$$

Proof. We assume for sake of contradiction that there does not exist any finite subset F of A for which $Y \subset \bigcup _ { \alpha \in F } V _ { \alpha }$ 

Let y be any element of Y. Then y must lie in at least one of the sets $V _ { \alpha }$ . Since each $V _ { \alpha }$ is open, there must therefore be an $r > 0$ such that $B _ { ( X , d ) } ( y , r ) \subseteq V _ { \alpha }$ . Now let $r ( y )$ denote the quantity 

$$
r (y) := \sup \{r \in (0, \infty): B _ {(X, d)} (y, r) \subseteq V _ {\alpha} \text {   for   some   } \alpha \in A \}.
$$

By the above discussion, we know that $r ( y ) > 0$ for all $y \in Y$ . Now, let $r _ { 0 }$ denote the quantity 

$$
r _ {0} := \inf \{r (y): y \in Y \}.
$$

Since $r ( y ) > 0$ for all $y \in Y$ , we have $r _ { 0 } \geq 0$ . There are two cases: $r _ { 0 } = 0$ and $r _ { 0 } > 0$ 

Case 1: $r _ { 0 } = 0$ . Then for every integer $n \geq 1$ , there is at least one point y in Y such that $r ( y ) < 1 / n { \mathrm { ~ ( w h y ? ) } }$ . We thus choose, for each $n \geq 1$ , a point $y ^ { ( n ) }$ in Y such that $r ( y ^ { ( n ) } ) < 1 / n$ (we can do this because of the axiom of choice, see Proposition 8.4.7). In particular we have l $\begin{array} { r } { \operatorname* { i m } _ { n \to \infty } r ( y ^ { ( n ) } ) = 0 } \end{array}$ , by the squeeze test. The sequence $( y ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ is a sequence in $Y ;$ since $Y$ is compact, we can thus find a subsequence $( y ^ { ( n _ { j } ) } ) _ { j = 1 } ^ { \infty }$ which converges to a point $y _ { 0 } \in Y$ 

As before, we know that there exists some $\alpha \in A$ such that $y _ { 0 } \in V _ { \alpha }$ and hence (since $V _ { \alpha }$ is open) there exists some $\varepsilon > 0$ such that $B ( y _ { 0 } , \varepsilon ) \subseteq V _ { \alpha }$ . Since $y ^ { ( n _ { j } ) }$ converges to $y _ { 0 }$ , there must exist an $N \geq 1$ such that $y ^ { ( n _ { j } ) } \in B ( y _ { 0 } , \varepsilon / 2 )$ for all $n \geq N$ . In particular, by the triangle inequality we have $B ( y ^ { ( n _ { j } ) } , \varepsilon / 2 ) \ \subseteq \ B ( y _ { 0 } , \varepsilon )$ , and thus $B ( y ^ { ( n _ { j } ) } , \varepsilon / 2 ) \ \subseteq \ V _ { \alpha }$ . By definition of $r ( y ^ { ( n _ { j } ) } )$ , this implies that $r ( y ^ { ( n _ { j } ) } ) \ge \varepsilon / 2$ for all $n \geq N$ . But this contradicts the fact that $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } r ( y ^ { ( n ) } ) = 0 } \end{array}$ 

Case 2: $r _ { 0 } > 0 .$ . In this case we now have $r ( y ) > r _ { 0 } / 2$ for all $y \in Y$ . This implies that for every $y \in Y$ there exists an $\alpha \in A$ such that $B ( y , r _ { 0 } / 2 ) \in V _ { \alpha } \mathrm { ~ ( w h y ? ) ~ }$ 

We now construct a sequence $y ^ { ( 1 ) } , y ^ { ( 2 ) } , . .$ . by the following recursive procedure. We let $y ^ { ( 1 ) }$ be any point in $Y$ . The ball $B ( y ^ { ( 1 ) } , r _ { 0 } / 2 )$ is contained in one of the $V _ { \alpha }$ and thus cannot cover all of $Y$ , since we would then obtain a finite cover, a contradiction. Thus there exists a point $y ^ { ( 2 ) }$ which does not lie in $B ( y ^ { ( 1 ) } , r _ { 0 } / 2 )$ 2 so in particular $d ( y ^ { ( 2 ) } , y ^ { ( 1 ) } ) \geq r _ { 0 } / 2$ . Choose such a point $y ^ { ( 2 ) }$ . The set $B ( y ^ { ( 1 ) } , r _ { 0 } / 2 ) \cup B ( y ^ { ( 2 ) } , r _ { 0 } / 2 )$ cannot cover all of $Y ,$ since we would then obtain two sets $V _ { \alpha _ { 1 } }$ and $V _ { \alpha _ { 2 } }$ which covered ${ \mathit { Y } } ,$ a contradiction again. So we can choose a point $y ^ { ( 3 ) }$ which does not lie in $B ( y ^ { ( 1 ) } , r _ { 0 } / 2 ) \cup B ( y ^ { ( 2 ) } , r _ { 0 } / 2 )$ , so in particular $d ( y ^ { ( 3 ) } , y ^ { ( 1 ) } ) \geq r _ { 0 } / 2$ and $d ( y ^ { ( 3 ) } , y ^ { ( 2 ) } ) \geq r _ { 0 } / 2$ . Continuing in this fashion we obtain a sequence $( y ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ in $Y$ with the property that $d ( y ^ { ( k ) } , y ^ { ( j ) } ) \geq r _ { 0 } / 2$ for all $k > j$ . In particular the sequence $( y ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ is not a Cauchy sequence, and in fact no subsequence of $( y ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ can be a Cauchy sequence either. But this contradicts the assumption that $Y$ is compact (by Lemma 1.4.7). 

It turns out that Theorem 1.5.8 has a converse: if Y has the property that every open cover has a finite sub-cover, then it is compact (Exercise 1.5.11). In fact, this property is often considered the more fundamental notion of compactness than the sequence-based one. (For metric spaces, the two notions, that of compactness and sequential compactness, are equivalent, but for more general topological spaces, the two notions are slightly diferent; see Exercise 2.5.8.) 

## 1.5. Compact metric spaces

Theorem 1.5.8 has an important corollary: that every nested sequence of non-empty compact sets is still non-empty. 

Corollary 1.5.9. Let $( X , d )$ be a metric space, and let $K _ { 1 } , K _ { 2 } , K _ { 3 } , \ldots$ be a sequence of non-empty compact subsets of X such that 

$$
K _ {1} \supset K _ {2} \supset K _ {3} \supset \dots .
$$

Then the intersection $\cap _ { n = 1 } ^ { \infty } K _ { n }$ is non-empty. 

Proof. See Exercise 1.5.6. 

We close this section by listing some miscellaneous properties of compact sets. 

Theorem 1.5.10. Let $( X , d )$ be a metric space. 

(a) If Y is a compact subset of X, and $Z \subseteq Y$ , then Z is compact if and only if Z is closed. 

(b) If $Y _ { 1 } , \dots , Y _ { n }$ are a finite collection of compact subsets of X, then their union $Y _ { 1 } \cup \ldots \cup Y _ { n }$ is also compact. 

(c) Every finite subset of X (including the empty set) is compact. 

Proof. See Exercise 1.5.7. 

$$
- \text { Exercises } -
$$

Exercise 1.5.1. Show that Definitions 9.1.22 and 1.5.3 match when talking about subsets of the real line with the standard metric. 

Exercise 1.5.2. Prove Proposition 1.5.5. (Hint: prove the completeness and boundedness separately. For both claims, use proof by contradiction. You wil need the axiom of choice, as in Lemma 8.4.5.) 

Exercise 1.5.3. Prove Theorem 1.5.7. (Hint: use Proposition 1.1.18 and Theorem 9.1.24.) 

Exercise 1.5.4. Let $( \mathbf { R } , d )$ be the real line with the standard metric. Give an example of a continuous function $f : \mathbf { R }  \mathbf { R }$ , and an open set $V \subseteq \mathbf { R }$ , such that the image $f ( V ) : = \{ f ( x ) : x \in V \}$ of V is not open. 

Exercise 1.5.5. Let $( \mathbf { R } , d )$ be the real line with the standard metric. Give an example of a continuous function $f : \mathbf { R }  \mathbf { R }$ , and a closed set $F \subseteq \mathbf { R }$ , such that $f ( F )$ is not closed. 

Exercise 1.5.6. Prove Corollary 1.5.9. (Hint: work in the compact metric space $( K _ { 1 } , d \vert _ { K _ { 1 } \times K _ { 1 } } )$ , and consider the sets $V _ { n } : = K _ { 1 } \backslash K _ { n }$ , which are open on $K _ { 1 }$ Assume for sake of contradiction that $\textstyle \bigcap _ { n = 1 } ^ { \infty } K _ { n } = \varnothing$ , and then apply Theorem 1.5.8.) 

Exercise 1.5.7. Prove Theorem 1.5.10. (Hint: for part (c), you may wish to use (b), and first prove that every singleton set is compact.) 

Exercise 1.5.8. Let $( X , d _ { l ^ { 1 } } )$ be the metric space from Exercise 1.1.15. For each natural number n, let $e ^ { ( n ) } = ( e _ { j } ^ { ( n ) } ) _ { j = 0 } ^ { \infty }$ be the sequence in X such that $e _ { j } ^ { ( n ) } : = 1$ when $n = j$ and $e _ { j } ^ { ( n ) } : = 0$ when $n \neq j$ . Show that the set $\{ e ^ { ( n ) } : n \in \mathbf { N } \}$ is a closed and bounded subset of X, but is not compact. (This is despite the fact that $( X , d _ { l ^ { 1 } } )$ is even a complete metric space - a fact which we will not prove here. The problem is that not that X is incomplete, but rather that it is “infinite-dimensional”, in a sense that we will not discuss here.) 

Exercise 1.5.9. Show that a metric space $( X , d )$ is compact if and only if every sequence in X has at least one limit point. 

Exercise 1.5.10. A metric space $( X , d )$ is called totally bounded if for every $\varepsilon \ > \ 0$ , there exists a positive integer n and a finite number of balls $\bar { B ( x ^ { ( 1 ) } , \varepsilon ) } , \dots , B ( x ^ { ( n ) } , \varepsilon )$ which cover X $\textstyle ( { \mathrm { i . e . , ~ } } X = \bigcup _ { i = 1 } ^ { n } B ( x ^ { ( i ) } , \varepsilon )$ 

(a) Show that every totally bounded space is bounded. 

(b) Show the following stronger version of Proposition 1.5.5: if $( X , d )$ is compact, then complete and totally bounded. (Hint: if X is not totally bounded, then there is some $\varepsilon > 0$ such that X cannot be covered by finitely many ε-balls. Then use Exercise 8.5.20 to find an infinite sequence of balls $B ( x ^ { ( n ) } , \varepsilon / 2 )$ which are disjoint from each other. Use this to then construct a sequence which has no convergent subsequence.) 

(c) Conversely, show that if X is complete and totally bounded, then X is compact. (Hint: if $( x ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ is a sequence in X, use the total boundedness hypothesis to recursively construct a sequence of subsequences $( x ^ { ( n ; j ) } ) _ { n = 1 } ^ { \infty }$ of $( x ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ for each positive integer j, such that for each $j ,$ the elements of the sequence $( x ^ { ( n ; j ) } ) _ { n = 1 } ^ { \infty }$ are contained in a single ball of radius $1 / j$ , and also that each sequence $( x ^ { ( n ; j + 1 ) } ) _ { n = 1 } ^ { \infty }$ is a subsequence of the previous one $( x ^ { ( n ; j ) } ) _ { n = 1 } ^ { \infty }$ . Then show that the “diagonal” sequence $( x ^ { ( n ; n ) } ) _ { n = 1 } ^ { \infty }$ is a Cauchy sequence, and then use the completeness hypothesis.) 

Exercise 1.5.11. Let $( X , d )$ have the property that every open cover of X has a finite subcover. Show that X is compact. (Hint: if X is not compact, then by Exercise 1.5.9, there is a sequence $( x ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ with no limit points. Then for every $x \in X$ there exists a ball $B ( x , \varepsilon )$ containing x which contains at most finitely many elements of this sequence. Now use the hypothesis.) 

Exercise 1.5.12. Let $( X , d _ { \mathrm { d i s c } } )$ be a metric space with the discrete metric $d _ { \mathrm { d i s c } }$ 

(a) Show that X is always complete. 

(b) When is X compact, and when is X not compact? Prove your claim. (Hint: the Heine-Borel theorem will be useless here since that only applies to Euclidean spaces.) 

Exercise 1.5.13. Let E and F be two compact subsets of R (with the standard metric $d ( x , y ) = | x - y | )$ . Show that the Cartesian product $E \times F : = \{ ( x , y )$ : $x \in E , y \in F { \big \} }$ is a compact subset of $\mathbf { R } ^ { 2 }$ (with the Euclidean metric $d _ { l ^ { 2 } } )$ 

Exercise 1.5.14. Let $( X , d )$ be a metric space, let E be a non-empty compact subset of $X$ , and let $x _ { 0 }$ be a point in X. Show that there exists a point $x \in E$ such that 

$$
d (x _ {0}, x) = \inf \{d (x _ {0}, y): y \in E \},
$$

$_ \mathrm { i . e . , \textit { x } }$ is the closest point in $E$ to $x _ { 0 }$ . (Hint: let R be the quantity $R : = \operatorname* { i n f } \{ d ( x _ { 0 } , y ) : y \in E \}$ . Construct a sequence $( x ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ in $E$ such that $\begin{array} { r } { d ( x _ { 0 } , x ^ { ( n ) } ) \leq R + \frac { 1 } { n } } \end{array}$ , and then use the compactness of E.) 

Exercise 1.5.15. Let $( X , d )$ be a compact metric space. Suppose that $( K _ { \alpha } ) _ { \alpha \in I }$ is a collection of closed sets in X with the property that any finite subcollection of these sets necessarily has non-empty intersection, thus $\cap _ { \alpha \in F } K _ { \alpha } \neq \emptyset$ for all finite $F \subseteq I$ . (This property is known as the finite intersection property.) Show that the entire collection has non-empty intersection, thus $\cap _ { \alpha \in I } K _ { \alpha } \neq \emptyset$ . Show by counterexample that this statement fails if X is not compact. 

## Chapter 2

## Continuous functions on metric spaces

## 2.1 Continuous functions

In the previous chapter we studied a single metric space $( X , d )$ , and the various types of sets one could find in that space. While this is already quite a rich subject, the theory of metric spaces becomes even richer, and of more importance to analysis, when one considers not just a single metric space, but rather pairs $( X , d _ { X } )$ and $( Y , d _ { Y } )$ of metric spaces, as well as continuous functions $f : X \to Y$ between such spaces. To define this concept, we generalize Definition 9.4.1 as follows: 

Definition 2.1.1 (Continuous functions). Let $( X , d _ { X } )$ be a metric space, and let $( Y , d _ { Y } )$ be another metric space, and let $f : X \to Y$ be a function. If $x _ { 0 } \in X$ , we say that f is continuous at $x _ { 0 }$ if for every $\varepsilon > 0$ , there exists a $\delta > 0$ such that $d _ { Y } ( f ( x ) , f ( x _ { 0 } ) ) < \varepsilon$ whenever $d _ { X } ( x , x _ { 0 } ) < \delta$ . We say that f is continuous if it is continuous at every point $x \in X$ 

Remark 2.1.2. Continuous functions are also sometimes called continuous maps. Mathematically, there is no distinction between the two terminologies. 

Remark 2.1.3. If $f : X \to Y$ is continuous, and K is any subset of X, then the restriction $f | _ { K } : K \to Y$ of f to K is also continuous (why?). 

We now generalize much of the discussion in Chapter 9. We first observe that continuous functions preserve convergence: 

Theorem 2.1.4 (Continuity preserves convergence). Suppose that $( X , d _ { X } )$ and $( Y , d _ { Y } )$ are metric spaces. Let $f : X \to Y$ be a function, 

## 2.1. Continuous functions

and let $x _ { 0 } \in X$ be a point in X. Then the following three statements are logically equivalent: 

(a) f is continuous at $x _ { 0 }$ . 

(b) Whenever $( x ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ is a sequence in X which converges to $x _ { 0 }$ with respect to the metric $d _ { X }$ , the sequence $( f ( x ^ { ( n ) } ) ) _ { n = 1 } ^ { \infty }$ converges to $f ( x _ { 0 } )$ with respect to the metric $d _ { Y }$ 

(c) For every open set $V \subset Y$ that contains $f ( x _ { 0 } )$ , there exists an open set $U \subset X$ containing x such that $f ( U ) \subseteq V$ 

Proof. See Exercise 2.1.1. 

Another important characterization of continuous functions involves open sets. 

Theorem 2.1.5. Let $( X , d _ { X } )$ be a metric space, and let $( Y , d _ { Y } )$ be another metric space. Let $f : X \to Y$ be a function. Then the following four statements are equivalent: 

(a) f is continuous. 

(b) Whenever $( x ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ is a sequence in X which converges to some point $x _ { 0 } \in \ X$ with respect to the metric $d _ { X }$ , the sequence $( f ( x ^ { ( n ) } ) ) _ { n = 1 } ^ { \infty }$ converges to $f ( x _ { 0 } )$ with respect to the metric $d _ { Y }$ 

(c) Whenever V is an open set in Y, the set $f ^ { - 1 } ( V ) : = \{ x \in X$ $f ( x ) \in V \}$ is an open set in X. 

(d) Whenever F is a closed set in Y, the set $f ^ { - 1 } ( F ) : = \{ x \in X$ $f ( x ) \in F \}$ is a closed set in X. 

## Proof. See Exercise 2.1.2.

Remark 2.1.6. It may seem strange that continuity ensures that the inverse image of an open set is open. One may guess instead that the reverse should be true, that the forward image of an open set is open; but this is not true; see Exercises 1.5.4, 1.5.5. 

As a quick corollary of the above two Theorems we obtain 

Corollary 2.1.7 (Continuity preserved by composition). Let $( X , d _ { X } )$ $( Y , d _ { Y } )$ , and $( Z , d _ { Z } )$ be metric spaces. 

(a) If $f : X \to Y$ is continuous at a point $x _ { 0 } \in X$ , and $g : Y  Z$ is continuous at $f ( x _ { 0 } )$ , then the composition $g \circ f : X \to Z$ , defined by $g \circ f ( x ) : = g ( f ( x ) )$ , is continuous at $x _ { 0 }$ 

(b) If $f : X \to Y$ is continuous, and $g : Y  Z$ is continuous, then $g \circ f : X \to Z$ is also continuous. 

Proof. See Exercise 2.1.3. 

Example 2.1.8. If $f : X  \mathbf { R }$ is a continuous function, then the function $f ^ { 2 } : X \to \mathbf { R }$ defined by $f ^ { 2 } ( x ) : = f ( x ) ^ { 2 }$ is automatically continuous also. This is because we have $f ^ { 2 } = g \circ f$ , where $g : \mathbf { R }  \mathbf { R }$ is the squaring function $g ( x ) : = x ^ { 2 }$ , and $g$ is a continuous function. 

— Exercises — 

Exercise 2.1.1. Prove Theorem 2.1.4. (Hint: review your proof of Proposition $9 . 4 . 7 . ) $ 

Exercise 2.1.2. Prove Theorem 2.1.5. (Hint: Theorem 2.1.4 already shows that (a) and (b) are equivalent.) 

Exercise 2.1.3. Use Theorem 2.1.4 and Theorem 2.1.5 to prove Corollary 2.1.7. 

Exercise 2.1.4. Give an example of functions $f : \mathbf { R }  \mathbf { R }$ and $g : \mathbf { R }  \mathbf { R }$ such that 

(a) f is not continuous, but g and $g \circ f$ are continuous; 

(b) g is not continuous, but f and $g \circ f$ are continuous; 

(c) f and g are not continuous, but $g \circ f$ is continuous. 

Explain briefly why these examples do not contradict Corollary 2.1.7. 

Exercise 2.1.5. Let $( X , d )$ be a metric space, and let $( E , d | _ { E \times E } )$ be a subspace of $( X , d )$ . Let $\iota _ { E  X } : E  X$ be the inclusion map, defined by setting $\iota _ { E \to X } ( x ) : = x$ for all $x \in E$ . Show that $\iota E {  } X$ is continuous. 

Exercise 2.1.6. Let $f : X \to Y$ be a function from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ . Let E be a subset of X (which we give the induced metric $d _ { X } | _ { E \times E } )$ , and let $f | _ { E } : E \to Y$ be the restriction of $f$ to $E$ , thus $f | _ { E } ( x ) : = f ( x )$ when $x \in E$ . If $x _ { 0 } ~ \in ~ E$ and $f$ is continuous at $x _ { 0 }$ , show that $f | _ { E }$ is also continuous at $x _ { 0 }$ . (Is the converse of this statement true? Explain.) Conclude that if $f$ is continuous, then $f | _ { E }$ is continuous. Thus restriction of the domain of a function does not destroy continuity. (Hint: use Exercise 2.1.5.) 

Exercise 2.1.7. Let $f : X \to Y$ be a function from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ . Suppose that the image $f ( X )$ of $X$ is contained in some subset $E \subset Y$ of $Y$ . Let $g : X \to E$ be the function which is the same as $f$ but with the range restricted from Y to $E$ , thus $g ( x ) = f ( x )$ for all $x \in X$ . We give $E$ the metric $d _ { Y } { \big | } _ { E \times E }$ induced from $Y$ . Show that for any $x _ { 0 } \in X$ , that $f$ is continuous at $x _ { 0 }$ if and only if $g$ is continuous at $x _ { 0 }$ . Conclude that $f$ is continuous if and only if $g$ is continuous. (Thus the notion of continuity is not afected if one restricts the range of the function.) 

## 2.2 Continuity and product spaces

Given two functions $f : X \to Y$ and $g : X \to Z$ , one can define their direct sum $f \oplus g : X \to Y \times Z$ defined by $f \oplus g ( x ) : = ( f ( x ) , g ( x ) )$ 4 i.e., this is the function taking values in the Cartesian product $Y \times Z$ whose first co-ordinate is $f ( x )$ and whose second co-ordinate is g(x) (cf. Exercise 3.5.7). For instance, if $f : \mathbf { R }  \mathbf { R }$ is the function $f ( x ) : = x ^ { 2 } + 3$ , and $g : \mathbf { R }  \mathbf { R }$ is the function $g ( x ) = 4 x$ , then $f \oplus g : \mathbf { R } \to \mathbf { R } ^ { 2 }$ is the function $f \oplus g ( x ) : = ( x ^ { 2 } + 3 , 4 x )$ . The direct sum operation preserves continuity: 

Lemma 2.2.1. Let $f : X \to \mathbf { R }$ and $g : X  \mathbf { R }$ be functions, and let $f \oplus g : X \to \mathbf { R } ^ { 2 }$ be their direct sum. We give $\mathbf { R } ^ { 2 }$ the Euclidean metric. 

(a) If $x _ { 0 } \in X$ , then f and g are both continuous at $x _ { 0 }$ if and only if $f \oplus g$ is continuous at x<sub>0</sub>. 

(b) f and g are both continuous if and only if f g is continuous. 

Proof. See Exercise 2.2.1. 

To use this, we first need another continuity result: 

Lemma 2.2.2. The addition function $( x , y ) \mapsto x + y$ , the subtraction function $( x , y ) \mapsto x - y$ , the multiplication function $( x , y ) \mapsto x y .$ the maximum function $( x , y ) \ \mapsto \ \operatorname* { m a x } ( x , y )$ , and the minimum function $( x , y ) \mapsto \operatorname* { m i n } ( x , y )$ , are all continuous functions from $\mathbf { R } ^ { 2 }$ to R. $T h e d i v i s i o n f u n c t i o n ( x , y ) \mapsto x / y$ is a continuous function from $\mathbf { R } \times ( \mathbf { R } \backslash \{ 0 \} ) = \{ ( x , y ) \in \mathbf { R } ^ { 2 } : y \neq 0 \}$ to R. For any real number c, the function x cx is a continuous function from R to R. 

Proof. See Exercise 2.2.2. 

Combining these lemmas we obtain 

Corollary 2.2.3. Let $( X , d )$ be a metric space, let $f : X \to \mathbf { R }$ and $g : X  \mathbf { R }$ be functions. Let c be a real number. 

(a) If $x _ { 0 } \in X$ and f and g are continuous at x<sub>0</sub>, then the functions $f + g : X \to \mathbf { R } , \ f - g : X \to \mathbf { R } , \ f g : X \to \mathbf { R } , \operatorname* { m a x } ( f , g ) : X \to \mathbf { R }$ min $( f , g ) : X \to \mathbf { R }$ , and $c f : X \to \mathbf { R }$ (see Definition 9.2.1 for definitions) are also continuous at x . If $g ( x ) \neq 0$ for all $x \in X$ then $f / g : X \to \mathbf { R }$ is also continuous at x<sub>0</sub>. 

(b) If f and g are continuous, then the functions $f + g : X \to \mathbf { R }$ $f - g : X \to \mathbf { R } , f g : X \to \mathbf { R }$ , max $( f , g ) : X \to \mathbf { R }$ , min $( f , g ) : X \to$ $\mathbf { R } ,$ and $c f : X \to \mathbf { R }$ are also continuous at x . If $g ( x ) \neq 0$ for all $x \in X$ , then $f / g : X \to \mathbf { R }$ is also continuous at $x _ { 0 }$ 

Proof. We first prove (a). Since f and g are continuous at $x _ { 0 }$ , then by Lemma 2.2.1 f $g : X \to \mathbf { R } ^ { 2 }$ is also continuous at $x _ { 0 }$ . On the other hand, from Lemma 2.2.2 the function $( x , y ) \mapsto x + y$ is continuous at every point in $\mathbf { R } ^ { 2 }$ , and in particular is continuous at $f \oplus g ( x _ { 0 } )$ . If we then compose these two functions using Corollary 2.1.7 we conclude that $f + g : X \to \mathbf { R }$ is continuous. A similar argument gives the continuity of $f - g , f g , \operatorname* { m a x } ( f , g )$ , min $( f , g )$ and $c f$ . To prove the claim for $f / g$ , we first use Exercise 2.1.7 to restrict the range of $g$ from R to $\mathbf { R } \backslash \{ 0 \}$ , and then one can argue as before. The claim (b) follows immediately from (a). □ 

This corollary allows us to demonstrate the continuity of a large class of functions; we give some examples below. 

## — Exercises —

Exercise 2.2.1. Prove Lemma 2.2.1. (Hint: use Proposition 1.1.18 and Theorem 2.1.4.) 

Exercise 2.2.2. Prove Lemma 2.2.2. (Hint: use Theorem 2.1.5 and limit laws (Theorem 6.1.19).) 

Exercise 2.2.3. Show that if $f : X \to \mathbf { R }$ is a continuous function, so is the function $| f | : X \to \mathbf { R }$ defined by $| f | ( x ) : = | f ( x ) |$ 

Exercise 2.2.4. Let $\pi _ { 1 } : \mathbf { R } ^ { 2 }  \mathbf { R }$ and $\pi _ { 2 } : \mathbf { R } ^ { 2 }  \mathbf { R }$ be the functions $\pi _ { 1 } ( x , y ) : =$ x and $\pi _ { 2 } ( x , y ) : = y$ (these two functions are sometimes called the co-ordinate functions on $\mathbf { R } ^ { 2 } )$ . Show that $\pi _ { 1 }$ and $\pi _ { 2 }$ are continuous. Conclude that if $f : \mathbf { R }  X$ is any continuous function into a metric space $( X , d )$ , then the functions $g _ { 1 } : \mathbf { R } ^ { 2 }  X$ and $g _ { 2 } : \mathbf { R } ^ { 2 }  X$ defined by $g _ { 1 } ( x , y ) : = f ( x )$ and $g _ { 2 } ( x , y ) : = f ( y )$ are also continuous. 

Exercise 2.2.5. Let $n , m \geq 0$ be integers. Suppose that for every $0 \leq i \leq n$ and $0 \leq j \leq m$ we have a real number $c _ { i j }$ . Form the function $P : \mathbf { R } ^ { 2 }  \mathbf { R }$ defined by 

$$
P (x, y) := \sum_ {i = 0} ^ {n} \sum_ {j = 0} ^ {m} c _ {i j} x ^ {i} y ^ {j}.
$$

(Such a function is known as a polynomial of two variables; a typical example of such a polynomial is $P ( x , y ) = x ^ { 3 } + 2 x y ^ { 2 } - x ^ { 2 } + 3 y + 6 . )$ Show that $P$ is continuous. (Hint: use Exercise 2.2.4 and Corollary 2.2.3.) Conclude that if $f : X \to \mathbf { R }$ and $g : X  \mathbf { R }$ are continuous functions, then the function $P ( f , g ) : X \to \mathbf { R }$ defined by $P ( f , g ) ( x ) : = P ( f ( x ) , g ( x ) )$ is also continuous. 

Exercise 2.2.6. Let $\mathbf { R } ^ { m }$ and $\mathbf { R } ^ { n }$ be Euclidean spaces. If $f : X \to \mathbf { R } ^ { m }$ and $g : X \to \mathbf { R } ^ { n }$ are continuous functions, show that $f \oplus g : X \to \mathbf { R } ^ { m + n }$ is also continuous, where we have identified $\mathbf { R } ^ { m } \times \mathbf { R } ^ { n }$ with $\mathbf { R } ^ { m + n }$ in the obvious manner. Is the converse statement true? 

Exercise 2.2.7. Let $k \geq 1$ , let I be a finite subset of $\mathbf { N } ^ { k }$ , and let $c : I  \mathbf { R }$ be a function. Form the function $P : \mathbf { R } ^ { k }  \mathbf { R }$ defined by 

$$
P (x _ {1}, \ldots , x _ {k}) := \sum_ {(i _ {1}, \ldots , i _ {k}) \in I} c (i _ {1}, \ldots , i _ {k}) x _ {1} ^ {i _ {1}} \ldots x _ {k} ^ {i _ {k}}.
$$

(Such a function is known as a polynomial of k variables; a typical example of such a polynomial is $P ( x _ { 1 } , x _ { 2 } , x _ { 3 } ) = 3 x _ { 1 } ^ { 3 } x _ { 2 } x _ { 3 } ^ { 2 } - x _ { 2 } x _ { 3 } ^ { 2 } + x _ { 1 } + 5 . )$ Show that P is continuous. (Hint: use induction on k, Exercise 2.2.6, and either Exercise 2.2.5 or Lemma 2.2.2.) 

Exercise 2.2.8. Let $( X , d _ { X } )$ and $( Y , d _ { Y } )$ be metric spaces. Define the metric $d _ { X \times Y } : ( X \times Y ) \times ( X \times Y ) \to [ 0 , \infty )$ by the formula 

$$
d _ {X \times Y} ((x, y), (x ^ {\prime}, y ^ {\prime})) := d _ {X} (x, x ^ {\prime}) + d _ {Y} (y, y ^ {\prime}).
$$

Show that $( X \times Y , d _ { X \times Y } )$ is a metric space, and deduce an analogue of Proposition 1.1.18 and Lemma 2.2.1. 

Exercise 2.2.9. Let $f : \mathbf { R } ^ { 2 } $ R be a function from $\mathbf { R } ^ { 2 }$ to R. Let $( x _ { 0 } , y _ { 0 } )$ be a point in $\mathbf { R } ^ { 2 }$ . If $f$ is continuous at $( x _ { 0 } , y _ { 0 } )$ , show that 

$$
\lim _ {x \to x _ {0}} \operatorname * {l i m s u p} _ {y \to y _ {0}} f (x, y) = \lim _ {y \to y _ {0}} \operatorname * {l i m s u p} _ {x \to x _ {0}} f (x, y) = f (x _ {0}, y _ {0})
$$

and 

$$
\lim _ {x \to x _ {0}} \operatorname * {l i m i n f} _ {y \to y _ {0}} f (x, y) = \lim _ {y \to y _ {0}} \operatorname * {l i m i n f} _ {x \to x _ {0}} f (x, y) = f (x _ {0}, y _ {0}).
$$

$\begin{array} { r l r } { \mathrm { ( R e c a l l ~ t h a t ~ \operatorname* { l i m } s u p } _ { x \to x _ { 0 } } f ( x ) } & { : = } & { \operatorname* { i n f } _ { r > 0 } \operatorname* { s u p } _ { | x - x _ { 0 } | < r } f ( x ) } \end{array}$ and lim ${ \mathrm { i n f } } _ { x \to x _ { 0 } }$ $\begin{array} { r } { f ( x ) : = \operatorname* { s u p } _ { r > 0 } \operatorname* { i n f } _ { | x - x _ { 0 } | < r } f ( x ) . \ ) } \end{array}$ In particular, we have 

$$
\lim _ {x \to x _ {0}} \lim _ {y \to y _ {0}} f (x, y) = \lim _ {y \to y _ {0}} \lim _ {x \to x _ {0}} f (x, y)
$$

whenever the limits on both sides exist. (Note that the limits do not necessarily exist in general; consider for instance the function $f : { \bf R } ^ { 2 }  { \bf R }$ such that $\begin{array} { r } { f ( x , y ) = y \sin { \frac { 1 } { x } } } \end{array}$ when xy $\neq 0$ and $f ( x , y ) = 0$ otherwise.) Discuss the comparison between this result and Example 1.2.7. 

Exercise 2.2.10. Let $f : { \bf R } ^ { 2 }  { \bf R }$ be a continuous function. Show that for each $x \in \mathbf { R }$ , the function $y \mapsto f ( x , y )$ is continuous on R, and for each $y \in \mathbf { R }$ the function $x \mapsto f ( x , y )$ is continuous on R. Thus a function $f ( x , y )$ which is jointly continuous in $( x , y )$ is also continuous in each variable $x , y$ separately. Exercise 2.2.11. Let $f : { \mathbf { R } } ^ { 2 }  { \mathbf { R } }$ be the function defined by $\textstyle f ( x , y ) : = { \frac { x y } { x ^ { 2 } + y ^ { 2 } } }$ when $( x , y ) \neq ( 0 , 0 )$ , and $f ( x , y ) = 0$ otherwise. Show that for each fixed $x \in \mathbf { R } .$ the function $y \mapsto f ( x , y )$ is continuous on R, and that for each fixed $y \in \mathbf { R }$ , the function $x \mapsto f ( x , y )$ is continuous on R, but that the function $f : { \mathbf { R } } ^ { 2 }  { \mathbf { R } }$ is not continuous on $\mathbf { R } ^ { 2 }$ . This shows that the converse to Exercise 2.2.10 fails; it is possible to be continuous in each variable separately without being jointly continuous. 

## 2.3 Continuity and compactness

Continuous functions interact well with the concept of compact sets defined in Definition 1.5.1. 

Theorem 2.3.1 (Continuous maps preserve compactness). Let f : $X \  \ Y$ be a continuous map from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ . Let $K \subseteq X$ be any compact subset of X. Then the image $f ( K ) : = \{ f ( x ) : x \in K \}$ of K is also compact. 

Proof. See Exercise 2.3.1. 

This theorem has an important consequence. Recall from Definition 9.6.5 the notion of a function $f : X \to \mathbf { R }$ attaining a maximum or minimum at a point. We may generalize Proposition 9.6.7 as follows: 

Proposition 2.3.2 (Maximum principle). Let $( X , d )$ be a compact metric space, and let $f : X \to \mathbf { R }$ be a continuous function. Then f is bounded. Furthermore, f attains its maximum at some point $x _ { m a x } \in X$ and also attains its minimum at some point $x _ { m i n } \in X$ 

Proof. See Exercise 2.3.2. 

Remark 2.3.3. As was already noted in Exercise 9.6.1, this principle can fail if X is not compact. This proposition should be compared with Lemma 9.6.3 and Proposition 9.6.7. 

Another advantage of continuous functions on compact sets is that they are uniformly continuous. We generalize Definition 9.9.2 as follows: 

Definition 2.3.4 (Uniform continuity). Let $f : X \to Y$ be a map from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ . We say that $f$ is uniformly continuous if, for every $\varepsilon > 0$ , there exists a $\delta > 0$ such that $d _ { Y } ( f ( x ) , f ( x ^ { \prime } ) ) < \varepsilon$ whenever $x , x ^ { \prime } \in X$ are such that $d _ { X } ( x , x ^ { \prime } ) < \delta$ 

Every uniformly continuous function is continuous, but not conversely (Exercise 2.3.3). But if the domain X is compact, then the two notions are equivalent: 

Theorem 2.3.5. Let $( X , d _ { X } )$ and $( Y , d _ { Y } )$ be metric spaces, and suppose that $( X , d _ { X } )$ is compact. If $f : X \to Y$ is function, then f is continuous $i f$ and only if it is uniformly continuous. 

Proof. If f is uniformly continuous then it is also continuous by Exercise 2.3.3. Now suppose that $f$ is continuous. Fix $\varepsilon > 0$ . For every $x _ { 0 } \in X$ , the function $f$ is continuous at $x _ { 0 }$ . Thus there exists a $\delta ( x _ { 0 } ) > 0 $ , depending on $x _ { 0 }$ , such that $d _ { Y } ( f ( x ) , f ( x _ { 0 } ) ) < \varepsilon / 2$ whenever $d _ { X } ( x , x _ { 0 } ) < \delta ( x _ { 0 } )$ . In particular, by the triangle inequality this implies that $d _ { Y } ( f ( x ) , f ( x ^ { \prime } ) ) < \varepsilon$ whenever $x \in B _ { ( X , d _ { X } ) } ( x _ { 0 } , \delta ( x _ { 0 } ) / 2 )$ and $d _ { X } ( x ^ { \prime } , x ) < \delta ( x _ { 0 } ) / 2 \ ( \mathrm { w h y ? } )$ 

Now consider the (possibly infinite) collection of balls 

$$
\{B _ {(X, d _ {X})} (x _ {0}, \delta (x _ {0}) / 2): x _ {0} \in X \}.
$$

Each ball in this collection is of course open, and the union of all these balls covers $X$ , since each point $x _ { 0 }$ in $X$ is contained in its own ball $B _ { ( X , d _ { X } ) } ( x _ { 0 } , \delta ( x _ { 0 } ) / 2 )$ . Hence, by Theorem 1.5.8, there exist a finite number of points $x _ { 1 } , \ldots , x _ { n }$ such that the balls $B _ { ( X , d _ { X } ) } ( x _ { j } , \delta ( x _ { j } ) / 2 )$ for $j = 1 , \dotsc , n$ cover $X$ : 

$$
X \subseteq \bigcup_ {j = 1} ^ {n} B _ {(X, d _ {X})} (x _ {j}, \delta (x _ {j}) / 2).
$$

Now let $\delta : = \mathrm { \ m i n } _ { i = 1 } ^ { n } \delta ( x _ { j } ) / 2$ . Since each of the $\delta ( x _ { j } )$ are positive, and there are only a finite number of $j$ , we see that $\delta \ > \ 0$ . Now let $x , x ^ { \prime }$ be any two points in $X$ such that $d _ { X } ( x , x ^ { \prime } ) ~ < ~ \delta$ Since the balls $B _ { ( X , d _ { X } ) } ( x _ { j } , \delta ( x _ { j } ) / 2 )$ cover $X$ , we see that there must exist $1 \leq j \leq n$ such that $x \in B _ { ( X , d _ { X } ) } ( x _ { j } , \delta ( x _ { j } ) / 2 )$ . Since $d _ { X } ( x , x ^ { \prime } ) < \delta$ , we have $d _ { X } ( x , x ^ { \prime } ) < \delta ( x _ { j } ) / 2$ , and so by the previous discussion we have $d _ { Y } ( f ( x ) , f ( x ^ { \prime } ) ) < \varepsilon$ . We have thus found a $\delta$ such that $d _ { Y } ( f ( x ) , f ( x ^ { \prime } ) ) <$ $\varepsilon$ whenever $d ( x , x ^ { \prime } ) ~ < ~ \delta$ , and this proves uniform continuity as desired. □ 

— Exercises — 

Exercise 2.3.1. Prove Theorem 2.3.1. 

Exercise 2.3.2. Prove Proposition 2.3.2. (Hint: modify the proof of Proposition $9 . 6 . 7 . ) $ 

Exercise 2.3.3. Show that every uniformly continuous function is continuous, but give an example that shows that not every continuous function is uniformly continuous. 

Exercise 2.3.4. Let $( X , d _ { X } ) , \ ( Y , d _ { Y } ) , \ ( Z , d _ { Z } )$ be metric spaces, and let $f :$ $X  Y$ and $g : Y  Z$ be two uniformly continuous functions. Show that $g \circ f : X \to Z$ is also uniformly continuous. 

Exercise 2.3.5. Let $( X , d _ { X } )$ be a metric space, and let $f : X \to \mathbf { R }$ and $g : X \to$ R be uniformly continuous functions. Show that the direct sum $f \oplus g : X \to \mathbf { R } ^ { 2 }$ defined by $f \oplus g ( x ) : = ( f ( x ) , g ( x ) )$ is uniformly continuous. 

Exercise 2.3.6. Show that the addition function $( x , y ) \mapsto x + y$ and the subtraction function $( x , y ) \mapsto x - y$ are uniformly continuous from $\mathbf { R } ^ { 2 }$ to R, but the multiplication function $( x , y ) \mapsto x y$ is not. Conclude that if $f : X \to \mathbf { R }$ and $g : X  \mathbf { R }$ are uniformly continuous functions on a metric space $( X , d )$ then $f + g : X \to \mathbf { R }$ and $f - g : X \to \mathbf { R }$ are also uniformly continuous. Give an example to show that $f g : X \to \mathbf { R }$ need not be uniformly continuous. What is the situation for max $( f , g )$ , min $( f , g ) , f / g$ , and $c f$ for a real number $c ?$ 

## 2.4 Continuity and connectedness

We now describe another important concept in metric spaces, that of connectedness. 

Definition 2.4.1 (Connected spaces). Let $( X , d )$ be a metric space. We say that X is disconnected if there exist disjoint non-empty open sets V and W in X such that $V \cup W = X$ . (Equivalently, X is disconnected if and only if X contains a non-empty proper subset which is simultaneously closed and open.) We say that X is connected if it is non-empty and not disconnected. 

We declare the empty set $\varnothing$ as being special - it is neither connected nor disconnected; one could think of the empty set as “unconnected”. 

Example 2.4.2. Consider the set $X : = [ 1 , 2 ] \cup [ 3 , 4 ]$ , with the usual metric. This set is disconnected because the sets [1, 2] and $[ 3 , 4 ]$ are open relative to X (why?). 

Intuitively, a disconnected set is one which can be separated into two disjoint open sets; a connected set is one which cannot be separated in this manner. We defined what it means for a metric space to be connected; we can also define what it means for a set to be connected. 

Definition 2.4.3 (Connected sets). Let $( X , d )$ be a metric space, and let Y be a subset of X. We say that Y is connected if the metric space $( Y , d | _ { Y \times Y } )$ is connected, and we say that Y is disconnected if the metric space $( Y , d | _ { Y \times Y } )$ is disconnected. 

Remark 2.4.4. This definition is intrinsic; whether a set Y is connected or not depends only on what the metric is doing on $Y$ , but not on what ambient space X one placing $Y$ in. 

On the real line, connected sets are easy to describe. 

Theorem 2.4.5. Let X be a subset ofthe real line R. Then the following statements are equivalent. 

(a) X is connected. 

(b) Whenever x, $y \in X$ and $x < y$ , the interval $[ x , y ]$ is also contained in X. 

(c) X is an interval (in the sense of Definition 9.1.1). 

Proof. First we show that (a) implies (b). Suppose that X is connected, and suppose for sake of contradiction that we could find points $x \ : < y$ in X such that $[ x , y ]$ is not contained in X. Then there exists a real number $x < z < y$ such that $z \not \in X$ . Thus the sets $( - \infty , z ) \cap X$ and $( z , \infty ) \cap X$ will cover X. But these sets are non-empty (because they contain x and y respectively) and are open relative to X, and so X is disconnected, a contradiction. 

Now we show that (b) implies (a). Let X be a set obeying the property (b). Suppose for sake of contradiction that X is disconnected. Then there exist disjoint non-empty sets V, W which are open relative to X, such that $V \cup W = X$ . Since V and W are non-empty, we may choose an $x \in V$ and $y \in W$ . Since V and W are disjoint, we have $x \neq y ;$ without loss of generality we may assume $x \ : < y$ . By property (b), we know that the entire interval $[ x , y ]$ is contained in X. 

Now consider the set $[ x , y ] \cap V$ . This set is both bounded and nonempty (because it contains x). Thus it has a supremum 

$$
z := \sup ([ x, y ] \cap V).
$$

Clearly $z \in [ x , y ]$ , and hence $z \in X$ . Thus either $z \in V$ or $z \in W$ Suppose first that $z \in V$ . Then $z \neq y$ (since $y \in W$ and V is disjoint from W). But V is open relative to X, which contains $[ x , y ]$ , so there is some ball $B _ { ( [ x , y ] , d ) } ( z , r )$ which is contained in V. But this contradicts the fact that z is the supremum of $[ x , y ] \cap V$ . Now suppose that $z \in W$ Then $z \neq x$ (since $x \in V$ and V is disjoint from W). But W is open relative to X, which contains $[ x , y ]$ , so there is some ball $B _ { ( [ x , y ] , d ) } ( z , r )$ which is contained in W. But this again contradicts the fact that z is the supremum of $[ x , y ] \cap V$ . Thus in either case we obtain a contradiction, which means that X cannot be disconnected, and must therefore be connected. 

It remains to show that (b) and (c) are equivalent; we leave this to Exercise 2.4.3. □ 

Continuous functions map connected sets to connected sets: 

Theorem 2.4.6 (Continuity preserves connectedness). Let $f : X \to Y$ be a continuous map from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ Let E be any connected subset of X. Then f(E) is also connected. 

Proof. See Exercise 2.4.4. 

An important corollary of this result is the intermediate value theorem, generalizing Theorem 9.7.1. 

Corollary 2.4.7 (Intermediate value theorem). Let $f : X \to \mathbf { R }$ be a continuous map from one metric space $( X , d _ { X } )$ to the real line. Let E be any connected subset of X, and let a, b be any two elements of E. Let y be a real number between $f ( a )$ and f(b), i.e., either $f ( a ) \leq y \leq f ( b )$ or $f ( a ) \geq y \geq f ( b )$ . Then there exists $c \in E$ such that $f ( c ) = y$ 

Proof. See Exercise 2.4.5. 

— Exercises — 

Exercise 2.4.1. Let $( X , d _ { d i s c } )$ be a metric space with the discrete metric. Let E be a subset of X which contains at least two elements. Show that E is disconnected. 

Exercise 2.4.2. Let $f : X \to Y$ be a function from a connected metric space $( X , d )$ to a metric space $( Y , d _ { d i s c } )$ with the discrete metric. Show that f is continuous if and only if it is constant. (Hint: use Exercise 2.4.1.) 

Exercise 2.4.3. Prove the equivalence of statements (b) and (c) in Theorem 2.4.5. 

Exercise 2.4.4. Prove Theorem 2.4.6. (Hint: the formulation of continuity in Theorem 2.1.5(c) is the most convenient to use.) 

Exercise 2.4.5. Use Theorem 2.4.6 to prove Corollary 2.4.7. 

Exercise 2.4.6. Let $( X , d )$ be a metric space, and let $( E _ { \alpha } ) _ { \alpha \in I }$ be a collection of connected sets in X. Suppose also that $\cap _ { \alpha \in I } E _ { \alpha }$ is non-empty. Show that $\textstyle \bigcup _ { \alpha \in I } E _ { \alpha }$ is connected. 

Exercise 2.4.7. Let $( X , d )$ be a metric space, and let E be a subset of X. We say that E is path-connected if, for every $x , y \in E$ , there exists a continuous function $\gamma : [ 0 , 1 ] \to E$ from the unit interval [0, 1] to E such that $\gamma ( 0 ) = x$ and $\gamma ( 1 ) = y .$ . Show that every path-connected set is connected. (The converse is false, but is a bit tricky to show and will not be detailed here.) 

Exercise 2.4.8. Let $( X , d )$ be a metric space, and let E be a subset of X. Show that if $E$ is connected, then the closure $\overline { E }$ of $E$ is also connected. Is the converse true? 

Exercise 2.4.9. Let $( X , d )$ be a metric space. Let us define a relation $x \sim y$ on X by declaring $x \sim y$ if there exists a connected subset of X which contains both x and $y .$ Show that this is an equivalence relation (i.e., it obeys the reflexive, symmetric, and transitive axioms). Also, show that the equivalence classes of this relation (i.e., the sets of the form $\{ y \in X : y \sim x \}$ for some $x \in X )$ are all closed and connected. (Hint: use Exercise 2.4.6 and Exercise 2.4.8.) These sets are known as the connected components of X. 

Exercise 2.4.10. Combine Proposition 2.3.2 and Corollary 2.4.7 to deduce a theorem for continuous functions on a compact connected domain which generalizes Corollary 9.7.4. 

## 2.5 Topological spaces (Optional)

The concept of a metric space can be generalized to that of a topological space. The idea here is not to view the metric d as the fundamental object; indeed, in a general topological space there is no metric at all. Instead, it is the collection of open sets which is the fundamental concept. Thus, whereas in a metric space one introduces the metric d first, and then uses the metric to define first the concept of an open ball and then the concept of an open set, in a topological space one starts just with the notion of an open set. As it turns out, starting from the open sets, one cannot necessarily reconstruct a usable notion of a ball or metric (thus not all topological spaces will be metric spaces), but remarkably one can still define many of the concepts in the preceding sections. 

We will not use topological spaces at all in this text, and so we shall be rather brief in our treatment of them here. A more complete study of these spaces can of course be found in any topology textbook, or a more advanced analysis text. 

Definition 2.5.1 (Topological spaces). A topological space is a pair $( X , { \mathcal { F } } )$ , where X is a set, and ${ \mathcal { F } } \subset 2 ^ { X }$ is a collection of subsets of $X$ whose elements are referred to as open sets. Furthermore, the collection $\mathcal { F }$ must obey the following properties: 

The empty set and the whole set X are open; in other words, $\varnothing \in { \mathcal { F } }$ and $X \in { \mathcal { F } }$ 

Any finite intersection of open sets is open. In other words, if $V _ { 1 } , \ldots , V _ { n }$ are elements of $\mathcal { F }$ , then $V _ { 1 } \cap \ldots \cap V _ { n }$ is also in $\mathcal { F }$ 

Any arbitrary union of open sets is open (including infinite unions). In other words, if $( V _ { \alpha } ) _ { \alpha \in I }$ is a family of sets in $\mathcal { F }$ , then $\textstyle \bigcup _ { \alpha \in I } V _ { \alpha }$ is also in $\mathcal { F }$ 

In many cases, the collection $\mathcal { F }$ of open sets can be deduced from context, and we shall refer to the topological space $( X , { \mathcal { F } } )$ simply as $X$ . 

From Proposition 1.2.15 we see that every metric space $( X , d )$ is automatically also a topological space (if we set $\mathcal { F }$ equal to the collection of sets which are open in $( X , d )$ . However, there do exist topological spaces which do not arise from metric spaces (see Exercise 2.5.1, 2.5.6). 

We now develop the analogues of various notions in this chapter and the previous chapter for topological spaces. The notion of a ball must be replaced by the notion of a neighbourhood. 

Definition 2.5.2 (Neighbourhoods). Let $( X , { \mathcal { F } } )$ be a topological space, and let $x \in X$ . A neighbourhood of x is defined to be any open set in $\mathcal { F }$ which contains x. 

Example 2.5.3. If $( X , d )$ is a metric space, $x \in X$ , and $r > 0$ , then $B ( x , r )$ is a neighbourhood of x. 

Definition 2.5.4 (Topological convergence). Let $m$ be an integer, $( X , { \mathcal { F } } )$ be a topological space and let $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ be a sequence of points in X. Let x be a point in X. We say that $( x ^ { ( n ) } ) _ { n = m } ^ { \infty }$ converges to x if and only if, for every neighbourhood $V$ of $x .$ , there exists an $N \geq m$ such that $x ^ { ( n ) } \in V$ for all $n \geq N$ 

This notion is consistent with that of convergence in metric spaces (Exercise 2.5.2). One can then ask whether one has the basic property of uniqueness of limits (Proposition 1.1.20). The answer turns out to usually be yes - if the topological space has an additional property known as the Hausdorfproperty - but the answer can be no for other topologies; see Exercise 2.5.4. 

Definition 2.5.5 (Interior, exterior, boundary). Let $( X , { \mathcal { F } } )$ be a topological space, let $E$ be a subset of $X$ , and let $x _ { 0 }$ be a point in $X$ . We say that $x _ { 0 }$ is an interior point of E if there exists a neighbourhood V of $x _ { 0 }$ such that $V \subseteq E$ . We say that $x _ { 0 }$ is an exterior point of $E$ if there exists a neighbourhood $V$ of $x _ { 0 }$ such that $V \cap E = \emptyset$ . We say that $x _ { 0 }$ 

## 2.5. Topological spaces (Optional)

is a boundary point of E if it is neither an interior point nor an exterior point of E. 

This definition is consistent with the corresponding notion for metric spaces (Exercise 2.5.3). 

Definition 2.5.6 (Closure). Let $( X , { \mathcal { F } } )$ be a topological space, let E be a subset of X, and let $x _ { 0 }$ be a point in $X$ . We say that $x _ { 0 }$ is an adherent point of $E$ if every neighbourhood V of $x _ { 0 }$ has a non-empty intersection with $E .$ . The set of all adherent points of $E$ is called the closure of $E$ and is denoted $\overline { E }$ 

There is a partial analogue of Theorem 1.2.10, see Exercise 2.5.10. 

We define a set K in a topological space $( X , { \mathcal { F } } )$ to be closed if its complement $X \backslash K$ is open; this is consistent with the metric space definition, thanks to Proposition 1.2.15(e). Some partial analogues of that Proposition are true (see Exercise 2.5.11). 

To define the notion of a relative topology, we cannot use Definition 1.3.3 as this requires a metric function. However, we can instead use Proposition 1.3.4 as our starting point: 

Definition 2.5.7 (Relative topology). Let $( X , { \mathcal { F } } )$ be a topological space, and Y be a subset of X. Then we define ${ \mathcal { F } } _ { Y } : = \{ V \cap Y : V \in { \mathcal { F } } \}$ and refer this as the topology on Y induced by $( X , { \mathcal { F } } )$ . We call $( Y , { \mathcal { F } } _ { Y } )$ a topological subspace of $( X , { \mathcal { F } } )$ . This is indeed a topological space, see Exercise 2.5.12. 

From Proposition 1.3.4 we see that this notion is compatible with the one for metric spaces. 

Next we define the notion of continuity. 

Definition 2.5.8 (Continuous functions). Let $( X , { \mathcal { F } } _ { X } )$ and $( Y , { \mathcal { F } } _ { Y } )$ be topological spaces, and let $f : X \to Y$ be a function. If $x _ { 0 } \in X$ , we say that $f$ is continuous at $x _ { 0 }$ if for every neighbourhood V of $f ( x _ { 0 } )$ , there exists a neighbourhood $U$ of $x _ { 0 }$ such that $f ( U ) \subseteq V$ . We say that $f$ is continuous if it is continuous at every point $x \in X$ 

This definition is consistent with that in Definition 2.1.1 (Exercise 2.5.15). Partial analogues of Theorems 2.1.4 and 2.1.5 are available (Exercise 2.5.16). In particular, a function is continuous if the preimages of every open set is open. 

There is unfortunately no notion of a Cauchy sequence, a complete space, or a bounded space, for topological spaces. However, there is certainly a notion of a compact space, as we can see by taking Theorem 1.5.8 as our starting point: 

Definition 2.5.9 (Compact topological spaces). Let $( X , { \mathcal { F } } )$ be a topological space. We say that this space is compact if every open cover of X has a finite subcover. If Y is a subset of X, we say that Y is compact if the topological space on Y induced by $( X , { \mathcal { F } } )$ is compact. 

Many basic facts about compact metric spaces continue to hold true for compact topological spaces, notably Theorem 2.3.1 and Proposition 2.3.2 (Exercise 2.5.17). However, there is no notion of uniform continuity, and so there is no analogue of Theorem 2.3.5. 

We can also define the notion of connectedness by repeating Definition 2.4.1 verbatim, and also repeating Definition 2.4.3 (but with Definition 2.5.7 instead of Definition 1.3.3). Many of the results and exercises in Section 2.4 continue to hold for topological spaces (with almost no changes to any of the proofs!). 

## — Exercises —

Exercise 2.5.1. Let X be an arbitrary set, and let ${ \mathcal F } : = \{ \emptyset , X \}$ . Show that (X, ) is a topology (called the trivial topology on X). If X contains more than one element, show that the trivial topology cannot be obtained from by placing a metric d on X. Show that this topological space is both compact and connected. 

Exercise 2.5.2. Let (X, d) be a metric space (and hence a topological space). Show that the two notions of convergence of sequences in Definition 1.1.14 and Definition 2.5.4 coincide. 

Exercise 2.5.3. Let (X, d) be a metric space (and hence a topological space). Show that the two notions of interior, exterior, and boundary in Definition 1.2.5 and Definition 2.5.5 coincide. 

Exercise 2.5.4. A topological space (X, ) is said to be Hausdorf if given any two distinct points x, $y \in X$ , there exists a neighbourhood V of x and a neighbourhood $W$ of y such that $V \cap W = \emptyset$ . Show that any topological space coming from a metric space is Hausdorf, and show that the trivial topology is not Hausdorf. Show that the analogue of Proposition 1.1.20 holds for Hausdorf topological spaces, but give an example of a non-Hausdorf topological space in which Proposition 1.1.20 fails. (In practice, most topological spaces one works with are Hausdorf; non-Hausdorf topological spaces tend to be so pathologica that it is not very profitable to work with them.) 

Exercise 2.5.5. Given any totally ordered set X with order relation $\leq$ , declare a set $V \subset X$ to be open if for every $x \in V$ there exists a set I which is an interval $\{ y \in X : a < y < b \}$ for some $a , b \in X$ , a ray $\{ y \in X : a < y \}$ for some $a \in X$ , the ray $\{ y \in X : y < b \}$ for some $b \in X$ , or the whole space $X .$ , which contains $x$ and is contained in V. Let $\mathcal { F }$ be the set of all open subsets of $X$ . Show that $( X , { \mathcal { F } } )$ is a topology (this is the order topology on the totally ordered set $( X , \leq ) )$ which is Hausdorf in the sense of Exercise 2.5.4. Show that on the real line R (with the standard ordering ), the order topology matches the standard topology (i.e., the topology arising from the standard metric). If instead one applies this to the extended real line $\mathbf { R } ^ { * }$ , show that R is an open set with boundary $\{ - \infty , + \infty \}$ . If $( x _ { n } ) _ { n = 1 } ^ { \infty }$ is a sequence of numbers in R (and hence in $\mathbf { R } ^ { * } )$ , show that $x _ { n }$ converges to + if and only if lim in $\dot { \bar { \iota } } _ { n \to \infty } x _ { n } = + \infty$ , and $x _ { n }$ converges to $- \infty$ if and only if lim $\operatorname* { s u p } _ { n \to \infty } x _ { n } = - \infty$ 

Exercise 2.5.6. Let X be an uncountable set, and let $\mathcal { F }$ be the collection of all subsets E in X which are either empty or co-finite (which means that $X \backslash E$ is finite). Show that $( X , { \mathcal { F } } )$ is a topology (this is called the cofinite topology on X) which is not Hausdorf in the sense of Exercise 2.5.4, and is compact and connected. Also, show that if $x \in X \ ( V _ { n } ) _ { n = 1 } ^ { \infty }$ is any countable collection of open sets containing $x ,$ then $\textstyle \bigcap _ { n = 1 } ^ { \infty } V _ { n } \neq \{ x \}$ . Use this to show that the cofinite topology cannot be obtained by placing a metric d on $X$ . (Hint: what is the set $\textstyle \bigcap _ { n = 1 } ^ { \infty } B ( x , 1 / n )$ equal to in a metric space?) 

Exercise 2.5.7. Let X be an uncountable set, and let $\mathcal { F }$ be the collection of all subsets E in X which are either empty or co-countable (which means that $X \backslash E$ is at most countable). Show that $( X , { \mathcal { F } } )$ is a topology (this is called the cocountable topology on X) which is not Hausdorf in the sense of Exercise 2.5.4, and connected, but cannot arise from a metric space and is not compact. 

Exercise 2.5.8. Show that there exists an uncountable well-ordered set $\omega _ { 1 } + 1$ that has a maximal element , and such that the initial segments $\{ x \in \omega _ { 1 } + 1 :$ $x < y \}$ are countable for all $y \in \omega _ { 1 } { + } 1 \backslash \{ \infty \}$ . (Hint: Well-order the real numbers using Exercise 8.5.19, take the union of all the countable initial segments, and then adjoin a maximal element .) If we give $\omega _ { 1 } + 1$ the order topology (Exercise 2.5.5), show that $\omega _ { 1 } + 1$ is compact; however, show that not every sequence has a convergent subsequence. 

Exercise 2.5.9. Let $( X , { \mathcal { F } } )$ be a compact topological space. Assume that this space is first countable, which means that for every $x \in X$ there exists a countable collection $V _ { 1 } , V _ { 2 } , \dots$ . of neighbourhoods of $x ,$ such that every neighbourhood of $x$ contains one of the $V _ { n }$ . Show that every sequence in X has a convergent subsequence, by modifying Exercise 1.5.11. Explain why this does not contradict Exercise 2.5.8. 

Exercise 2.5.10. Prove the following partial analogue of Proposition 1.2.10 for topological spaces: (c) implies both (a) and (b), which are equivalent to each other. Show that in the co-countable topology in Exercise 2.5.7, it is possible for (a) and (b) to hold without (c) holding. 

Exercise 2.5.11. Let E be a subset of a topological space $( X , { \mathcal { F } } )$ . Show that E is open if and only if every element of E is an interior point, and show that E is closed if and only if E contains all of its adherent points. Prove analogues of Proposition $1 . 2 . 1 5 ( \mathrm { e } ) \mathrm { - ( h ) }$ (some of these are automatic by definition). If we assume in addition that X is Hausdorf, prove an analogue of Proposition 1.2.15(d) also, but give an example to show that (d) can fail when X is not Hausdorf. 

Exercise 2.5.12. Show that the pair $( Y , { \mathcal { F } } _ { Y } )$ defined in Definition 2.5.7 is indeed a topological space. 

Exercise 2.5.13. Generalize Corollary 1.5.9 to compact sets in a topological space. 

Exercise 2.5.14. Generalize Theorem 1.5.10 to compact sets in a topological space. 

Exercise 2.5.15. Let $( X , d _ { X } )$ and $( Y , d _ { Y } )$ be metric spaces (and hence a topological space). Show that the two notions continuity (both at a point, and on the whole domain) of a function $f : X \to Y$ in Definition 2.1.1 and Definition 2.5.8 coincide. 

Exercise 2.5.16. Show that when Theorem 2.1.4 is extended to topological spaces, that (a) implies (b). (The converse is false, but constructing an example is dificult.) Show that when Theorem 2.1.5 is extended to topological spaces, that (a), (c), (d) are all equivalent to each other, and imply (b). (Again, the converse implications are false, but dificult to prove.) 

Exercise 2.5.17. Generalize both Theorem 2.3.1 and Proposition 2.3.2 to compact sets in a topological space. 

## Chapter 3

## Uniform convergence

In the previous two chapters we have seen what it means for a sequence $( x ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ of points in a metric space $( X , d _ { X } )$ to converge to a limit $x ;$ it means that lim $i _ { n  \infty } d _ { X } ( x ^ { ( n ) } , x ) = 0$ , or equivalently that for every $\varepsilon > 0$ there exists an $N > 0$ such that $d _ { X } ( x ^ { ( n ) } , x ) < \varepsilon$ for all $n > N$ . (We have also generalized the notion of convergence to topological spaces $( X , { \mathcal { F } } )$ 1 but in this chapter we will focus on metric spaces.) 

In this chapter, we consider what it means for a sequence of functions $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ to converge. In other words, we have a sequence of functions $f ^ { ( 1 ) } , f ^ { ( 2 ) } , \ldots$ , with each function $f ^ { ( n ) } : X \to Y$ being a function from $X$ to $Y$ , and we ask what it means for this sequence of functions to converge to some limiting function $f$ . 

It turns out that there are several diferent concepts of convergence of functions; here we describe the two most important ones, pointwise convergence and uniform convergence. (There are other types of convergence for functions, such as $L ^ { 1 }$ convergence, $L ^ { 2 }$ convergence, convergence in measure, almost everywhere convergence, and so forth, but these are beyond the scope of this text.) The two notions are related, but not identical; the relationship between the two is somewhat analogous to the relationship between continuity and uniform continuity. 

Once we work out what convergence means for functions, and thus can make sense of such statements as $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } f ^ { ( n ) } = f } \end{array}$ , we will then ask how these limits interact with other concepts. For instance, we already have a notion of limiting values of functions: $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in X } f ( x )$ . Can we interchange limits, i.e. 

$$
\lim _ {n \to \infty} \lim _ {x \to x _ {0}; x \in X} f ^ {(n)} (x) = \lim _ {x \to x _ {0}; x \in X} \lim _ {n \to \infty} f ^ {(n)} (x)?
$$

As we shall see, the answer depends on what type of convergence we have for $f ^ { ( n ) }$ . We will also address similar questions involving interchanging limits and integrals, or limits and sums, or sums and integrals. 

## 3.1 Limiting values of functions

Before we talk about limits of sequences of functions, we should first discuss a similar, but distinct, notion, that of limiting values of functions. We shall focus on the situation for metric spaces, but there are similar notions for topological spaces (Exercise 3.1.3). 

Definition 3.1.1 (Limiting value of a function). Let $( X , d _ { X } )$ and $( Y , d _ { Y } )$ be metric spaces, let E be a subset of X, and let $f : X \to Y$ be a function. If $x _ { 0 } \in X$ is an adherent point of E, and $L \in Y$ , we say that $f ( x )$ converges to L in Y as x converges to $x _ { 0 }$ in E, or write $\begin{array} { r } { \operatorname* { l i m } _ { x  x _ { 0 } ; x \in E } f ( x ) = L } \end{array}$ , if for every $\varepsilon > 0$ there exists a $\delta > 0$ such that $d _ { Y } ( f ( x ) , L ) < \varepsilon$ for all $x \in E$ such that $d _ { X } ( x , x _ { 0 } ) < \delta$ 

Remark 3.1.2. Some authors exclude the case $x = x _ { 0 }$ from the above definition, thus requiring $0 < d _ { X } ( x , x _ { 0 } ) < \delta$ . In our current notation, this would correspond to removing x<sub>0</sub> from E, thus one would consider $\begin{array} { r } { \operatorname* { l i m } _ { x  x _ { 0 } ; x \in E \backslash \{ x _ { 0 } \} } f ( x ) } \end{array}$ instead of $\scriptstyle \operatorname* { l i m } _ { x \in x _ { 0 } ; x \in E } f ( x )$ . See Exercise 3.1.1 for a comparison of the two concepts. 

Comparing this with Definition 2.1.1, we see that f is continuous at $x _ { 0 }$ if and only if 

$$
\lim _ {x \to x _ {0}; x \in X} f (x) = f (x _ {0}).
$$

Thus f is continuous on X if we have 

$$
\lim _ {x \to x _ {0}; x \in X} f (x) = f (x _ {0}) \text {   for   all   } x _ {0} \in X.
$$

Example 3.1.3. If $f : \mathbf { R }  \mathbf { R }$ is the function $f ( x ) = x ^ { 2 } - 4$ , then 

$$
\lim _ {x \to 1} f (x) = f (1) = 1 - 4 = - 3
$$

since f is continuous. 

Remark 3.1.4. Often we shall omit the condition $x \in X$ , and abbreviate $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in X } f ( x )$ as simply $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } } f ( x )$ when it is clear what space x will range in. 

## 3.1. Limiting values of functions

One can rephrase Definition 3.1.1 in terms of sequences: 

Proposition 3.1.5. Let $( X , d _ { X } )$ and $( Y , d _ { Y } )$ be metric spaces, let E be a subset of $X$ , and let $f : X \to Y$ be a function. Let $x _ { 0 } \in X$ be an adherent point of $E$ and $L \in Y$ . Then the following four statements are logically equivalent: 

(a) $\begin{array} { r } { \operatorname* { l i m } _ { x  x _ { 0 } ; x \in E } f ( x ) = L . } \end{array}$ 

(b) For every sequence $( x ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ in E which converges to $x _ { 0 }$ with $r e \mathrm { - }$ spect to the metric $d _ { X }$ , the sequence $( f ( x ^ { ( n ) } ) ) _ { n = 1 } ^ { \infty }$ converges to $L$ with respect to the metric $d _ { Y }$ 

(c) For every open set $V \subset Y$ which contains $L ,$ there exists an open set $U \subset X$ containing $x _ { 0 }$ such that $f ( U \cap E ) \subseteq V$ 

(d) Ifone defines the function $g : E \cup \{ x _ { 0 } \}  Y$ by defining $g ( x _ { 0 } ) : = L$ and $g ( x ) : = f ( x ) \ f o r \ x \in E \backslash \{ x _ { 0 } \}$ , then g is continuous at $x _ { 0 }$ Furthermore, if $x _ { 0 } \in E$ , then $f ( x _ { 0 } ) = L$ 

Proof. See Exercise 3.1.2. 

Remark 3.1.6. Observe from Proposition 3.1.5(b) and Proposition 1.1.20 that a function $f ( x )$ can converge to at most one limit $L$ as x converges to $x _ { 0 }$ . In other words, if the limit 

$$
\lim _ {x \to x _ {0}; x \in E} f (x)
$$

exists at all, then it can only take at most one value. 

Remark 3.1.7. The requirement that $x _ { 0 }$ be an adherent point of $E$ is necessary for the concept of limiting value to be useful, otherwise $x _ { 0 }$ will lie in the exterior of $E .$ , the notion that $f ( x )$ converges to $L$ as x converges to $x _ { 0 }$ in $E$ is vacuous (for $\delta$ suficiently small, there are no points $x \in E$ so that $d ( x , x _ { 0 } ) < \delta )$ 

Remark 3.1.8. Strictly speaking, we should write 

$$
d _ {Y} - \lim _ {x \to x _ {0}; x \in E} f (x) \text {   instead   of   } \lim _ {x \to x _ {0}; x \in E} f (x),
$$

since the convergence depends on the metric $d _ { Y }$ . However in practice it will be obvious what the metric $d _ { Y }$ is and so we will omit the $d _ { Y ^ { - } }$ prefix from the notation. 

— Exercises — 

Exercise 3.1.1. Let $( X , d _ { X } )$ and $( Y , d _ { Y } )$ be metric spaces, let $E$ be a subset of X, let $f : E \to Y$ be a function, and let $x _ { 0 }$ be an element of $E .$ . Show that the limit $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in E } f ( x )$ exists if and only if the limit $\begin{array} { r } { \operatorname* { l i m } _ { x  x _ { 0 } ; x \in E \backslash \{ x _ { 0 } \} } f ( x ) } \end{array}$ exists and is equal to $f ( x _ { 0 } )$ . Also, show that if the limit lim ${ } _ { \cdot x \to x _ { 0 } ; x \in E } f ( x )$ exists at all, then it must equal $f ( x _ { 0 } )$ 

Exercise 3.1.2. Prove Proposition 3.1.5. (Hint: review your proof of Theorem 2.1.4.) 

Exercise 3.1.3. Use Proposition 3.1.5(c) to define a notion of a limiting value of a function $f : X \to Y$ from one topological space $( X , { \mathcal { F } } _ { X } )$ to another $( Y , { \mathcal { F } } _ { Y } )$ Then prove the equivalence of Proposition 3.1.5(c) and $3 . 1 . 5 ( \mathrm { d } )$ . If in addition Y is a Hausdorf topological space (see Exercise 2.5.4), prove an analogue of Remark 3.1.6. Is the same statement true if Y is not Hausdorf? 

Exercise 3.1.4. Recall from Exercise 2.5.5 that the extended real line $\mathbf { R } ^ { * }$ comes with a standard topology (the order topology). We view the natural numbers N as a subspace of this topological space, and + as an adherent point of N in $\mathbf { R } ^ { * }$ . Let $( a _ { n } ) _ { n = 0 } ^ { \infty }$ be a sequence taking values in a topological space $( Y , { \mathcal { F } } _ { Y } )$ and let $L \in Y$ . Show that $\begin{array} { r } { \operatorname* { l i m } _ { n  + \infty ; n \in \mathbf { N } } a _ { n } = L } \end{array}$ (in the sense of Exercise 3.1.3) if and only ${ \mathrm { i f ~ l i m } } _ { n  \infty } a _ { n } = L$ (in the sense of Definition 2.5.4). This shows that the notions of limiting values of a sequence, and limiting values of a function, are compatible. 

Exercise 3.1.5. Let $( X , d _ { X } ) , ( Y , d _ { Y } ) , ( Z , d _ { Z } )$ be metric spaces, and let $x _ { 0 } \in X$ , $y _ { 0 } \in Y , z _ { 0 } \in Z$ . Let $f : X \to Y$ and $g : Y  Z$ be functions, and let E be a set. If we have $\begin{array} { r } { \operatorname* { l i m } _ { x  x _ { 0 } ; x \in E } f ( x ) = y _ { 0 } } \end{array}$ and $\begin{array} { r } { \operatorname* { l i m } _ { y \to y _ { 0 } ; y \in f ( E ) } g ( y ) = z _ { 0 } } \end{array}$ , conclude that $\textstyle \operatorname* { l i m } _ { x \in x _ { 0 } ; x \in E } g \circ f ( x ) = z _ { 0 }$ 

Exercise 3.1.6. State and prove an analogue of the limit laws in Proposition 9.3.14 when X is now a metric space rather than a subset of R. (Hint: use Corollary 2.2.3.) 

## 3.2 Pointwise and uniform convergence

The most obvious notion of convergence of functions is pointwise convergence, or convergence at each point of the domain: 

Definition 3.2.1 (Pointwise convergence). Let $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ be a sequence of functions from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ , and let $f : X \to Y$ be another function. We say that $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ converges pointwise to f on X if we have 

$$
\lim _ {n \to \infty} f ^ {(n)} (x) = f (x)
$$

for all $x \in X , \operatorname { i . e }$ 

$$
\lim _ {n \to \infty} d _ {Y} (f ^ {(n)} (x), f (x)) = 0.
$$

Or in other words, for every x and every $\varepsilon > 0$ there exists $N > 0$ such that $d _ { Y } ( f ^ { ( n ) } ( x ) , f ( x ) ) < \varepsilon$ for every $n > N$ . We call the function $f$ the pointwise limit of the functions $f ^ { ( n ) }$ 

Remark 3.2.2. Note that $f ^ { ( n ) } ( x )$ and $f ( x )$ are points in $Y .$ , rather than functions, so we are using our prior notion of convergence in metric spaces to determine convergence of functions. Also note that we are not really using the fact that $( X , d _ { X } )$ is a metric space $( \mathrm { i . e . , }$ we are not using the metric $d _ { X } )$ ; for this definition it would sufice for $X$ to just be a plain old set with no metric structure. However, later on we shall want to restrict our attention to continuous functions from $X$ to $Y$ and in order to do so we need a metric on $X$ (and on Y), or at least a topological structure. Also when we introduce the concept of uniform convergence, then we will definitely need a metric structure on $X$ and $Y ;$ there is no comparable notion for topological spaces. 

Example 3.2.3. Consider the functions $f ^ { ( n ) } : { \textbf { R } } \to { \textbf { R } }$ defined by $f ^ { ( n ) } ( x ) : = x / n$ , while $f : \mathbf { R }  \mathbf { R }$ is the zero function $f ( x ) : = 0$ . Then $f ^ { ( n ) }$ converges pointwise to $f _ { i }$ , since for each fixed real number x we have $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } f ^ { ( n ) } ( x ) = \operatorname* { l i m } _ { n \to \infty } x / n = 0 = f ( x ) } \end{array}$ 

From Proposition 1.1.20 we see that a sequence $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ of functions from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ can have at most one pointwise limit $f$ (this explains why we can refer to $f$ as the pointwise limit). However, it is of course possible for a sequence of functions to have no pointwise limit (can you think of an example?), just as a sequence of points in a metric space do not necessarily have a limit. 

Pointwise convergence is a very natural concept, but it has a number of disadvantages: it does not preserve continuity, derivatives, limits, or integrals, as the following three examples show. 

Example 3.2.4. Consider the functions $f ^ { ( n ) } : [ 0 , 1 ] \to \mathbf { R }$ defined by $f ^ { ( n ) } ( x ) : = x ^ { n }$ , and let $f : [ 0 , 1 ] \to \mathbf { R }$ be the function defined by setting $f ( x ) : = 1$ when $x = 1$ and $f ( x ) : = 0$ when $0 \leq x < 1$ . Then the functions $f ^ { ( n ) }$ are continuous, and converge pointwise to $f$ on [0, 1] (why? treat the cases $x = 1$ and $0 \leq x < 1$ separately), however the limiting function $f$ is not continuous. Note that the same example shows that pointwise convergence does not preserve diferentiability either. 

Example 3.2.5. If lim $. { } ~ . . . . x _ { 0 } ; x { \in } E ^ { \ f ^ { ( n ) } } ( x ) \ = \ L$ for every $n _ { ; }$ , and $f ^ { ( n ) }$ converges pointwise to $f ,$ , we cannot always take limits conclude that $\begin{array} { r } { \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in E } f ( x ) = L } \end{array}$ . The previous example is also a counterexample here: observe that $\begin{array} { r } { \operatorname* { l i m } _ { x \to 1 ; x \in [ 0 , 1 ) } x ^ { n } = 1 } \end{array}$ for every $n ,$ but $x ^ { n }$ converges pointwise to the function $f$ defined in the previous paragraph, and $\textstyle \operatorname* { l i m } _ { x \to 1 ; x \in [ 0 , 1 ) } f ( x ) = 0$ . In particular, we see that 

$$
\lim _ {n \to \infty} \lim _ {x \to x _ {0}; x \in X} f ^ {(n)} (x) \neq \lim _ {x \to x _ {0}; x \in X} \lim _ {n \to \infty} f ^ {(n)} (x).
$$

(cf. Example 1.2.8). Thus pointwise convergence does not preserve limits. 

Example 3.2.6. Suppose that $f ^ { ( n ) } : [ a , b ]  \mathbf { R }$ a sequence of Riemannintegrable functions on the interval $[ a , b ]$ . If $\begin{array} { r } { \int _ { [ a , b ] } f ^ { ( n ) } = L } \end{array}$ for every $n ,$ and $f ^ { ( n ) }$ converges pointwise to some new function $f _ { i }$ , this does not mean that $\int _ { [ a , b ] } f = L$ . An example comes by setting $[ a , b ] : = [ 0 , 1 ]$ , and letting $f ^ { ( n ) }$ be the function $f ^ { ( n ) } ( x ) : = 2 n$ when $x \in [ 1 / 2 n , 1 / n ]$ , and $f ^ { ( n ) } ( x ) : = 0$ for all other values of x. Then $f ^ { ( n ) }$ converges pointwise to the zero function $f ( x ) : = 0 \ \mathrm { ( w h y ? ) }$ . On the other hand, $\begin{array} { r } { \int _ { [ 0 , 1 ] } f ^ { ( n ) } = 1 } \end{array}$ for every n, while $\begin{array} { r } { \int _ { [ 0 , 1 ] } f = 0 } \end{array}$ . In particular, we have an example where 

$$
\lim _ {n \to \infty} \int_ {[ a, b ]} f ^ {(n)} \neq \int_ {[ a, b ]} \lim _ {n \to \infty} f ^ {(n)}.
$$

One may think that this counterexample has something to do with the $f ^ { ( n ) }$ being discontinuous, but one can easily modify this counterexample to make the $f ^ { ( n ) }$ continuous (can you see how?). 

Another example in the same spirit is the “moving bump” example. Let $f ^ { ( n ) } : { \textbf { R } } \to { \textbf { R } }$ be the function defined by $f ^ { ( n ) } ( x ) : = 1$ if $x \in$ $[ n , n + 1 ]$ and $f ^ { ( n ) } ( x ) : = 0$ otherwise. Then $\int _ { \mathbf { R } } { f ^ { ( n ) } } \ = 1$ for every n (where $\scriptstyle \int _ { \mathbf { R } } f$ is defined as the limit of $\int _ { [ - N , N ] } f$ as N goes to infinity). On the other hand, $f ^ { ( n ) }$ converges pointwise to the zero function $0 \ \mathrm { ( w h y ? ) }$ , and $\int _ { \mathbf { R } } 0 \ = \ 0$ . In both of these examples, functions of area 1 have somehow “disappeared” to produce functions of area 0 in the limit. See also Example 1.2.9. 

These examples show that pointwise convergence is too weak a concept to be of much use. The problem is that while $f ^ { ( n ) } ( x )$ converges to $f ( x )$ for each x, the rate of that convergence varies substantially with x. For instance, consider the first example where $f ^ { ( n ) } : [ 0 , 1 ] \to \mathbf { R }$ was the function $f ^ { ( n ) } ( x ) : = x ^ { n }$ , and $f : [ 0 , 1 ] \to \mathbf { R }$ was the function such that $f ( x ) : = 1$ when $x = 1$ , and $f ( x ) : = 0$ otherwise. Then for each x, $f ^ { ( n ) } ( x )$ converges to $f ( x )$ as $n  \infty ;$ ; this is the same as saying that $\scriptstyle \operatorname* { l i m } _ { n \to \infty } x ^ { n } = 0$ when $0 \leq x < 1$ , and that $\scriptstyle \operatorname* { l i m } _ { n \to \infty } x ^ { n } = 1$ when $x = 1$ But the convergence is much slower near 1 than far away from 1. For instance, consider the statement that $\scriptstyle \operatorname* { l i m } _ { n \to \infty } x ^ { n } = 0$ for all $0 \leq x < 1$ This means, for every $0 \leq x < 1$ , that for every $\varepsilon _ { i }$ , there exists an $N \geq 1$ such that $| x ^ { n } | < \varepsilon$ for all $n \geq N \mathrm { ~ - ~ } \mathrm { o r }$ in other words, the sequence $1 , x , x ^ { 2 } , x ^ { 3 } , . . .$ . will eventually get less than $\varepsilon ,$ after passing some finite number N of elements in this sequence. But the number of elements N one needs to go out to depends very much on the location of $x .$ . For instance, take $\varepsilon : = 0 . 1$ . If $x = 0 . 1$ , then we have $| x ^ { n } | < \varepsilon$ for all $n \geq 2 \mathrm { ~ - ~ }$ the sequence gets underneath ε after the second element. But if $x = 0 . 5$ then we only get $| x ^ { n } | < \varepsilon$ for $n \geq 4 ~ \AA ^ { } - { }$ you have to wait until the fourth element to get within $\varepsilon$ of the limit. And if $x = 0 . 9$ , then one only has $| x ^ { n } | < \varepsilon$ when $n \geq 2 2$ . Clearly, the closer x gets to 1, the longer one has to wait until $f ^ { ( n ) } ( x )$ will get within $\varepsilon$ of $f ( x )$ , although it still will get there eventually. (Curiously, however, while the convergence gets worse and worse as x approaches 1, the convergence suddenly becomes perfect when $x = 1 . )$ 

To put things another way, the convergence of $f ^ { ( n ) }$ to f is not uniform in $x \mathrm { ~ - ~ }$ the N that one needs to get $f ^ { ( n ) } ( x )$ within $\varepsilon$ of $f$ depends on x as well as on $\varepsilon .$ . This motivates a stronger notion of convergence. 

Definition 3.2.7 (Uniform convergence). Let $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ be a sequence of functions from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ , and let $f : X \to Y$ be another function. We say that $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ converges uniformly to f on X if for every $\varepsilon > 0$ there exists $N > 0$ such that $d _ { Y } ( f ^ { ( n ) } ( x ) , f ( x ) ) < \varepsilon$ for every $n > N$ and $x \in X$ . We call the function f the uniform limit of the functions $f ^ { ( n ) }$ 

Remark 3.2.8. Note that this definition is subtly diferent from the definition for pointwise convergence in Definition 3.2.1. In the definition of pointwise convergence, N was allowed to depend on x; now it is not. The reader should compare this distinction to the distinction between continuity and uniform continuity (i.e., between Definition 2.1.1 and Definition 2.3.4). A more precise formulation of this analogy is given in Exercise 3.2.1. 

It is easy to see that if $f ^ { ( n ) }$ converges uniformly to $f$ on $X$ , then it also converges pointwise to the same function $f$ (see Exercise 3.2.2); thus when the uniform limit and pointwise limit both exist, then they have to be equal. However, the converse is not true; for instance the functions $f ^ { ( n ) } : [ 0 , 1 ] \to \mathbf { R }$ defined earlier by $f ^ { ( n ) } ( x ) : = x ^ { n }$ converge pointwise, but do not converge uniformly (see Exercise 3.2.2). 

Example 3.2.9. Let $f ^ { ( n ) } : [ 0 , 1 ] \to \mathbf { R }$ be the functions $f ^ { ( n ) } ( x ) : = x / n$ and let $f : [ 0 , 1 ] \to \mathbf { R }$ be the zero function $f ( x ) : = 0$ . Then it is clear that $f ^ { ( n ) }$ converges to f pointwise. Now we show that in fact $f ^ { ( n ) }$ converges to $f$ uniformly. We have to show that for every $\varepsilon > 0$ , there exists an $N$ such that $| f ^ { ( n ) } ( x ) - f ( x ) | < \varepsilon$ for every $x \in [ 0 , 1 ]$ and every $n \geq N$ To show this, let us fix an $\varepsilon > 0$ . Then for any $x \in [ 0 , 1 ]$ and $n \geq N$ , we have 

$$
| f ^ {(n)} (x) - f (x) | = | x / n - 0 | = x / n \leq 1 / n \leq 1 / N.
$$

Thus if we choose N such that $N > 1 / \varepsilon$ (note that this choice of N does not depend on what x is), then we have $| f ^ { ( n ) } ( x ) - f ( x ) | < \varepsilon$ for all $n \geq N$ and $x \in [ 0 , 1 ]$ , as desired. 

We make one trivial remark here: if a sequence $f ^ { ( n ) } : X \to Y$ of functions converges pointwise (or uniformly) to a function $f : X \to Y$ 2 then the restrictions $f ^ { ( n ) } | _ { E } : E \to Y$ of $f ^ { ( n ) }$ to some subset E of X will also converge pointwise (or uniformly) to $f | _ { Y } . \mathrm { \ ( W h y ? ) }$ 

## — Exercises —

Exercise 3.2.1. The purpose of this exercise is to demonstrate a concrete relationship between continuity and pointwise convergence, and between uniform continuity and uniform convergence. Let $f : \mathbf { R }  \mathbf { R }$ be a function. For any $a \in \mathbf { R }$ , let $f _ { a } : \mathbf { R }  \mathbf { R }$ be the shifted function $f _ { a } ( x ) : = f ( x - a )$ 

(a) Show that f is continuous if and only if, whenever $( a _ { n } ) _ { n = 0 } ^ { \infty }$ is a sequence of real numbers which converges to zero, the shifted functions $f _ { a _ { 1 } }$ converge pointwise to $f .$ 

(b) Show that f is uniformly continuous if and only if, whenever $( a _ { n } ) _ { n = 0 } ^ { \infty }$ is a sequence of real numbers which converges to zero, the shifted functions $f _ { a _ { n } }$ converge uniformly to $f .$ 

Exercise 3.2.2. (a) Let $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ be a sequence of functions from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ , and let $f : X \to Y$ be another function from X to Y. Show that if $f ^ { ( n ) }$ converges uniformly to $f _ { i }$ , then $f ^ { ( n ) }$ also converges pointwise to $f .$ 

(b) For each integer $n \geq 1$ , let $f ^ { ( n ) } : ( - 1 , 1 ) \to \mathbf { R }$ be the function $f ^ { ( n ) } ( x ) : =$ $x ^ { n }$ . Prove that $f ^ { ( n ) }$ converges pointwise to the zero function 0, but does not converge uniformly to any function $f : ( - 1 , 1 ) \to \mathbf { R }$ 

(c) Let $g : ( - 1 , 1 )  \mathbf { R }$ be the function $g ( x ) : = x / ( 1 - x )$ . With the notation as in (b), show that the partial sums $\textstyle \sum _ { n = 1 } ^ { N } f ^ { ( n ) }$ converges pointwise as $N \to \infty$ to g, but does not converge uniformly to $g _ { \mathrm { : } }$ , on the open interval $( - 1 , 1 )$ . (Hint: use Lemma 7.3.3.) What would happen if we replaced the open interval ( 1, 1) with the closed interval $[ - 1 , 1 ] ?$ 

Exercise 3.2.3. Let $( X , d _ { X } )$ a metric space, and for every integer $n \geq 1$ , let $f _ { n } : X \to \mathbf { R }$ be a real-valued function. Suppose that $f _ { n }$ converges pointwise to another function $f : X  \mathbf { R }$ on X (in this question we give R the standard metric $d ( x , y ) = | x - y | )$ . Let $h : \mathbf { R }  \mathbf { R }$ be a continuous function. Show that the functions $h \circ f _ { n }$ converge pointwise to $h \circ f$ on X, where $h \circ f _ { n } : X  \mathbf { R }$ is the function $h \circ f _ { n } ( x ) : = h ( f _ { n } ( x ) )$ , and similarly for $h \circ f$ 

Exercise 3.2.4. Let $f _ { n } : X \to Y$ be a sequence of bounded functions from one metric space $( X , d _ { X } )$ to another metric space $( Y , d _ { Y } )$ . Suppose that $f _ { n }$ converges uniformly to another function $f : X \to Y$ . Suppose that f is a bounded function; i.e., there exists a ball $B _ { ( Y , d _ { Y } ) } ( y _ { 0 } , R )$ in $Y$ such that $f ( x ) \in$ $B _ { ( Y , d _ { Y } ) } ( y _ { 0 } , R )$ for all $x \in X$ . Show that the sequence $f _ { n }$ is uniformly bounded; i.e. there exists a ball $B _ { ( Y , d _ { Y } ) } ( y _ { 0 } , R )$ in $Y$ such that $f _ { n } ( x ) \in B _ { ( Y , d _ { Y } ) } ( y _ { 0 } , R )$ for all $x \in X$ and all positive integers n. 

## 3.3 Uniform convergence and continuity

We now give the first demonstration that uniform convergence is significantly better than pointwise convergence. Specifically, we show that the uniform limit of continuous functions is continuous. 

Theorem 3.3.1 (Uniform limits preserve continuity I). Suppose $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ is a sequence of functions from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ , and suppose that this sequence converges uniformly to another function $f : X \to Y$ . Let x<sub>0</sub> be a point in X. If the functions $f ^ { ( n ) }$ are continuous at x<sub>0</sub> for each n, then the limiting function f is also continuous at x . 

Proof. See Exercise 3.3.1. 

This has an immediate corollary: 

Corollary 3.3.2 (Uniform limits preserve continuity II). Let $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ be a sequence of functions from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ , and suppose that this sequence converges uniformly to another function $f : X \to Y$ . If the functions $f ^ { ( n ) }$ are continuous on X for each n, then the limiting function f is also continuous on X. 

This should be contrasted with Example 3.2.4. There is a slight variant of Theorem 3.3.1 which is also useful: 

Proposition 3.3.3 (Interchange of limits and uniform limits). Let $( X , d _ { X } )$ and $( Y , d _ { Y } )$ be metric spaces, with Y complete, and let E be a subset of X. Let $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ be a sequence of functions from E to $Y _ { . }$ and suppose that this sequence converges uniformly in E to some function $f : E \to Y$ . Let $x _ { 0 } \in X$ be an adherent point of E, and suppose that for each n the limit l $\begin{array} { r } { \operatorname* { m } _ { x \to x _ { 0 } ; x \in E } f ^ { ( n ) } ( x ) } \end{array}$ exists. Then the limit $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in E } f ( x )$ also exists, and is equal to the limit of the sequence $( \scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in E } f ^ { ( n ) } ( x ) ) _ { n = 1 } ^ { \infty }$ ; in other words we have the interchange of limits 

$$
\lim _ {n \to \infty} \lim _ {x \to x _ {0}; x \in E} f ^ {(n)} (x) = \lim _ {x \to x _ {0}; x \in E} \lim _ {n \to \infty} f ^ {(n)} (x).
$$

Proof. See Exercise 3.3.2. 

This should be constrasted with Example 3.2.5. Finally, we have a version of these theorems for sequences: 

Proposition 3.3.4. Let $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ be a sequence of continuous functions from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ , and suppose that this sequence converges uniformly to another function $f : X \to Y$ . Let $x ^ { ( n ) }$ be a sequence of points in X which converge to some limit x. Then $f ^ { ( n ) } ( x ^ { ( n ) } )$ converges (in Y) to $f ( x )$ 

Proof. See Exercise 3.3.4. 

A similar result holds for bounded functions: 

Definition 3.3.5 (Bounded functions). A function $f : X \to Y$ from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ is bounded if $f ( X )$ is a bounded set, i.e., there exists a ball $B _ { ( Y , d _ { Y } ) } ( y _ { 0 } , R )$ in $Y$ such that $f ( x ) \in$ $B _ { ( Y , d _ { Y } ) } ( y _ { 0 } , R )$ for all $x \in X$ 

Proposition 3.3.6 (Uniform limits preserve boundedness). Let $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ be a sequence of functions from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ , and suppose that this sequence converges uniformly to another function $f : X \to Y$ . If the functions $f ^ { ( n ) }$ are bounded on X for each n, then the limiting function f is also bounded on X. 

Proof. See Exercise 3.3.6. 

Remark 3.3.7. The above propositions sound very reasonable, but one should caution that it only works if one assumes uniform convergence; pointwise convergence is not enough. (See Exercises 3.3.3, 3.3.5, 3.3.7.) 

— Exercises — 

Exercise 3.3.1. Prove Theorem 3.3.1. Explain briefly why your proof requires uniform convergence, and why pointwise convergence would not sufice. (Hints: it is easiest to use the “epsilon-delta” definition of continuity from Definition 2.1.1. You may find the triangle inequality 

$$
\begin{array}{c} d _ {Y} (f (x), f (x _ {0})) \leq d _ {Y} (f (x), f ^ {(n)} (x)) + d _ {Y} (f ^ {(n)} (x), f ^ {(n)} (x _ {0})) \\ + d _ {Y} (f ^ {(n)} (x _ {0}), f (x _ {0})) \end{array}
$$

useful. Also, you may need to divide $\varepsilon { \mathrm { ~ a s ~ } } \varepsilon = \varepsilon / 3 + \varepsilon / 3 + \varepsilon / 3$ . Finally, it is possible to prove Theorem 3.3.1 from Proposition 3.3.3, but you may find it easier conceptually to prove Theorem 3.3.1 first.) 

Exercise 3.3.2. Prove Proposition 3.3.3. (Hint: this is very similar to Theorem 3.3.1. Theorem 3.3.1 cannot be used to prove Proposition 3.3.3, however it is possible to use Proposition 3.3.3 to prove Theorem 3.3.1.) 

Exercise 3.3.3. Compare Proposition 3.3.3 with Example 1.2.8. Can you now explain why the interchange of limits in Example 1.2.8 led to a false statement, whereas the interchange of limits in Proposition 3.3.3 is justified? 

Exercise 3.3.4. Prove Proposition 3.3.4. (Hint: again, this is similar to Theorem 3.3.1 and Proposition 3.3.3, although the statements are slightly diferent, and one cannot deduce this directly from the other two results.) 

Exercise 3.3.5. Give an example to show that Proposition 3.3.4 fails if the phrase “converges uniformly” is replaced by “converges pointwise”. (Hint: some of the examples already given earlier will already work here.) 

Exercise 3.3.6. Prove Proposition 3.3.6. Discuss how this proposition difers from Exercise 3.2.4. 

Exercise 3.3.7. Give an example to show that Proposition 3.3.6 fails if the phrase “converges uniformly” is replaced by “converges pointwise”. (Hint: some of the examples already given earlier will already work here.) 

Exercise 3.3.8. Let $( X , d )$ be a metric space, and for every positive integer n, let $f _ { n } : X \to \mathbf { R }$ and $g _ { n } : X \to \mathbf { R }$ be functions. Suppose that $( f _ { n } ) _ { n = 1 } ^ { \infty }$ converges uniformly to another function $f : X \to \mathbf { R }$ , and that $( g _ { n } ) _ { n = 1 } ^ { \infty }$ converges uniformly to another function $g : X  \mathbf { R }$ . Suppose also that the functions $( f _ { n } ) _ { n = 1 } ^ { \infty }$ and $( g _ { n } ) _ { n = 1 } ^ { \infty }$ are uniformly bounded, i.e., there exists an $M > 0$ such that $| f _ { n } ( x ) | \leq M$ and $| g _ { n } ( x ) | \leq M$ for all $n \geq 1$ and $x \in X$ . Prove that the functions $f _ { n } g _ { n } : X \to \mathbf { R }$ converge uniformly to $f g : X \to \mathbf { R }$ 

## 3.4 The metric of uniform convergence

We have now developed at least four, apparently separate, notions of limit in this text: 

(a) limits lim $\mathbf { 1 } _ { n \to \infty } x ^ { ( n ) }$ of sequences of points in a metric space (Definition 1.1.14; see also Definition 2.5.4); 

(b) limiting values $\scriptstyle \operatorname* { l i m } _ { x \to x _ { 0 } ; x \in E } f ( x )$ of functions at a point (Definition 3.1.1); 

(c) pointwise limits f of functions $f ^ { ( n ) }$ (Definition 3.2.1; and 

(d) uniform limits f of functions $f ^ { ( n ) }$ (Definition 3.2.7). 

This proliferation of limits may seem rather complicated. However, we can reduce the complexity slightly by observing that (d) can be viewed as a special case of (a), though in doing so it should be cautioned that because we are now dealing with functions instead of points, the convergence is not in X or in Y, but rather in a new space, the space of functions from X to $Y$ 

Remark 3.4.1. If one is willing to work in topological spaces instead of metric spaces, we can also view (b) as a special case of (a), see Exercise 3.1.4, and (c) is also a special case of (a), see Exercise 3.4.4. Thus the notion of convergence in a topological space can be used to unify all the notions of limits we have encountered so far. 

Definition 3.4.2 (Metric space of bounded functions). Suppose $( X , d _ { X } )$ and $( Y , d _ { Y } )$ are metric spaces. We let $B ( X  Y )$ denote the space<sup>1</sup> of bounded functions from X to Y: 

$$
B (X \to Y) := \{f | f: X \to Y \text {   is   a   bounded   function } \}.
$$

We define a metric $d _ { \infty } : B ( X \to Y ) \times B ( X \to Y ) \to \mathbf { R } ^ { + }$ by defining 

$$
d _ {\infty} (f, g) := \sup _ {x \in X} d _ {Y} (f (x), g (x)) = \sup \left\{d _ {Y} (f (x), g (x)): x \in X \right\}
$$

for all $f , g \in B ( X \to Y )$ . This metric is sometimes known as the sup norm metric or the $L ^ { \infty }$ metric. We will also use $d _ { B ( X  Y ) }$ as a synonym for $d _ { \infty }$ 

Notice that the distance $d _ { \infty } ( f , g )$ is always finite because f and g are assumed to be bounded on X. 

Example 3.4.3. Let $X : = [ 0 , 1 ]$ and $Y = \mathbf { R } \quad$ . Let $f : [ 0 , 1 ] \to \mathbf { R }$ and $g : [ 0 , 1 ] \to \mathbf { R }$ be the functions $f ( x ) : = 2 x$ and $g ( x ) : = 3 x$ . Then f and g are both bounded functions and thus live in $B ( [ 0 , 1 ]  \mathbf { R } )$ ). The distance between them is 

$$
d _ {\infty} (f, g) = \sup _ {x \in [ 0, 1 ]} | 2 x - 3 x | = \sup _ {x \in [ 0, 1 ]} | x | = 1.
$$

This space turns out to be a metric space (Exercise 3.4.1). Convergence in this metric turns out to be identical to uniform convergence: 

Proposition 3.4.4. Let $( X , d _ { X } )$ and $( Y , d _ { Y } )$ be metric spaces. Let $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ be a sequence of functions in $B ( X  Y )$ , and let f be another function in $B ( X \to Y ) . T h e n ( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty } $ converges to f in the metric $d _ { B ( X  Y ) }$ if and only if $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ converges uniformly to f. 

Proof. See Exercise 3.4.2. 

Now let $C ( X  Y )$ be the space of bounded continuous functions from X to Y: 

$$
C (X \to Y) := \{f \in B (X \to Y) \Big | f \text {   is   continuous } \}.
$$

This set $C ( X  Y )$ is clearly a subset of $B ( X  Y )$ . Corollary 3.3.2 asserts that this space $C ( X  Y )$ is closed in $B ( X  Y ) ~ \mathrm { ( w h y ? ) }$ Actually, we can say a lot more: 

Theorem 3.4.5 (The space of continuous functions is complete). Let $( X , d _ { X } )$ be a metric space, and let $( Y , d _ { Y } )$ be a complete metric space. The space $( C ( X \to Y ) , d _ { B ( X \to Y ) } | _ { C ( X \to Y ) \times C ( X \to Y ) } )$ is a complete subspace of $( B ( X \to Y ) , d _ { B ( X \to Y ) } )$ . In other words, every Cauchy sequence of functions in $C ( X  Y )$ converges to a function in $C ( X  Y )$ 

Proof. See Exercise 3.4.3. 

$$
- \text { Exercises } -
$$

Exercise 3.4.1. Let $( X , d _ { X } )$ and $( Y , d _ { Y } )$ be metric spaces. Show that the space $B ( X  Y )$ defined in Definition 3.4.2, with the metric $d _ { B ( X  Y ) }$ , is indeed a metric space. 

Exercise 3.4.2. Prove Proposition 3.4.4. 

Exercise 3.4.3. Prove Theorem 3.4.5. (Hint: this is similar, but not identical, to the proof of Theorem 3.3.1). 

Exercise 3.4.4. Let $( X , d _ { X } )$ and $( Y , d _ { Y } )$ be metric spaces, and let $Y ^ { X } : = \{ f { \big | } f$ $X  Y \}$ be the space of all functions from X to $Y$ (cf. Axiom 3.10). If $x _ { 0 } \in X$ and V is an open set in $Y _ { \textrm { : } }$ , let $V ^ { ( x _ { 0 } ) } \subseteq Y ^ { X }$ be the set 

$$
V ^ {(x _ {0})} := \{f \in Y ^ {X}: f (x _ {0}) \in V \}.
$$

If E is a subset of $Y ^ { X }$ , we say that E is open if for every $f \in E .$ , there exists a finite number of points $x _ { 1 } , \ldots , x _ { n } \in X$ and open sets $V _ { 1 } , \ldots , V _ { n } \subseteq Y$ such that 

$$
f \in V _ {1} ^ {(x _ {1})} \cap \ldots \cap V _ {n} ^ {(x _ {n})} \subseteq E.
$$

Show that if $\mathcal { F }$ is the collection of open sets in $Y ^ { X }$ , then $( Y ^ { X } , { \mathcal { F } } )$ is a topological space. 

For each natural number n, let $f ^ { ( n ) } : X \to Y$ be a function from X to $Y$ , and let $f : X \to Y$ be another function from X to Y. Show that $f ^ { ( n ) }$ converges to f in the topology $\mathcal { F }$ (in the sense of Definition 2.5.4) if and only if $f ^ { ( n ) }$ converges to f pointwise (in the sense of Definition 3.2.1). 

The topology $\mathcal { F }$ is known as the topology of pointwise convergence, for obvious reasons; it is also known as the product topology. It shows that the concept of pointwise convergence can be viewed as a special case of the more general concept of convergence in a topological space. 

## 3.5 Series of functions; the Weierstrass M-test

Having discussed sequences of functions, we now discuss infinite series $\textstyle \sum _ { n = 1 } ^ { \infty } f _ { n }$ of functions. Now we shall restrict our attention to functions $f : X \to \mathbf { R }$ from a metric space $( X , d _ { X } )$ to the real line R (which we of course give the standard metric); this is because we know how to add two real numbers, but don’t necessarily know how to add two points in a general metric space Y. Functions whose range is R are sometimes called real-valued functions. 

Finite summation is, of course, easy: given any finite collection $f ^ { ( 1 ) } , \ldots , f ^ { ( N ) }$ of functions from X to R, we can define the finite sum $\sum _ { i = 1 } ^ { N } f ^ { ( i ) } : X \to \mathbf { R }$ by 

$$
\left(\sum_ {i = 1} ^ {N} f ^ {(i)}\right) (x) := \sum_ {i = 1} ^ {N} f ^ {(i)} (x).
$$

Example 3.5.1. If $f ^ { ( 1 ) } : { \bf R }  { \bf R }$ is the function $f ^ { ( 1 ) } ( x ) : = x , f ^ { ( 2 ) }$ $\mathbf R \to \mathbf R$ is the function $f ^ { ( 2 ) } ( x ) : = x ^ { 2 }$ , and $f ^ { ( 3 ) } : { \bf R }  { \bf R }$ is the function $f ^ { ( 3 ) } ( x ) : = x ^ { 3 }$ , then $\textstyle f : = \sum _ { i = 1 } ^ { 3 } f ^ { ( i ) }$ is the function $f : \mathbf { R }  \mathbf { R }$ defined by $f ( x ) : = x + x ^ { 2 } + x ^ { 3 }$ 

It is easy to show that finite sums of bounded functions are bounded, and finite sums of continuous functions are continuous (Exercise 3.5.1). 

Now to add infinite series. 

Definition 3.5.2 (Infinite series). Let $( X , d _ { X } )$ be a metric space. Let $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ be a sequence of functions from X to R, and let $f$ be another function from X to R. If the partial sums $\scriptstyle \sum _ { n = 1 } ^ { N } f ^ { ( n ) }$ converge pointwise to $f$ on $X$ as $N \to \infty$ , we say that the infinite series $\textstyle \sum _ { n = 1 } ^ { \infty } f ^ { ( n ) }$ converges pointwise to $f$ , and write $\textstyle f = \sum _ { n = 1 } ^ { \infty } f ^ { ( n ) }$ . If the partial sums $\textstyle \sum _ { n = 1 } ^ { N } f ^ { ( n ) }$ converge uniformly to $f$ on X as $N \to \infty$ , we say that the infinite series $\scriptstyle \sum _ { n = 1 } ^ { \infty } f ^ { ( n ) }$ converges uniformly to $f _ { i }$ and again write $\textstyle f = \sum _ { n = 1 } ^ { \infty } f ^ { ( n ) }$ (Thus when one sees an expression such as $\textstyle f = \sum _ { n = 1 } ^ { \infty } f ^ { ( n ) }$ , one should look at the context to see in what sense this infinite series converges.) 

Remark 3.5.3. A series $\textstyle \sum _ { n = 1 } ^ { \infty } f ^ { ( n ) }$ converges pointwise to f on X if and only if $\scriptstyle \sum _ { n = 1 } ^ { \infty } f ^ { ( n ) } ( x )$ converges to $f ( x )$ for every $x \in X$ . (Thus if $\textstyle \sum _ { n = 1 } ^ { \infty } f ^ { ( n ) }$ does not converge pointwise to $f$ , this does not mean that it diverges pointwise; it may just be that it converges for some points x but diverges at other points x.) 

If a series $\textstyle \sum _ { n = 1 } ^ { \infty } f ^ { ( n ) }$ converges uniformly to $f ,$ then it also converges pointwise to $f ;$ but not vice versa, as the following example shows. 

Example 3.5.4. Let $f ^ { ( n ) } : ( - 1 , 1 ) \to \mathbf { R }$ be the sequence of functions $f ^ { ( n ) } ( x ) : = x ^ { n }$ . Then $\textstyle \sum _ { n = 1 } ^ { \infty } f ^ { ( n ) }$ converges pointwise, but not uniformly, to the function $x / ( 1 - x )$ (see Exercise 3.2.2 and Example 3.5.8). 

It is not always clear when a series $\textstyle \sum _ { n = 1 } ^ { \infty } f ^ { ( n ) }$ converges or not. However, there is a very useful test that gives at least one test for uniform convergence. 

Definition 3.5.5 (Sup norm). If $f : X \to \mathbf { R }$ is a bounded real-valued function, we define the sup norm $\| f \| _ { \infty }$ of f to be the number 

$$
\| f \| _ {\infty} := \sup \{| f (x) |: x \in X \}.
$$

In other words, $\| f \| _ { \infty } = d _ { \infty } ( f , 0 )$ , where $0 : X  \mathbf { R }$ is the zero function $0 ( x ) : = 0$ , and $d _ { \infty }$ was defined in Definition 3.4.2. (Why is this the case?) 

Example 3.5.6. Thus, for instance, if $f : ( - 2 , 1 ) \to \mathbf { R }$ is the function $f ( x ) : = 2 x$ , then $\| f \| _ { \infty } = \operatorname* { s u p } \{ | 2 x | : x \in ( - 2 , 1 ) \} = 4 { \mathrm { ~ ( w h y ? ) } }$ . Notice that when f is bounded then $\| f \| _ { \infty }$ will always be a non-negative rea number. 

Theorem 3.5.7 (Weierstrass $M { \mathrm { - t e s t } } )$ . Let $( X , d )$ be a metric space, and let $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ be a sequence of bounded real-valued continuous functions on X such that the series $\scriptstyle \sum _ { n = 1 } ^ { \infty } \| f ^ { ( n ) } \| _ { \infty }$ is convergent. (Note that this is a series of plain old real numbers, not of functions.) Then the series $\textstyle \sum _ { n = 1 } ^ { \infty } f ^ { ( n ) }$ converges uniformly to some function f on X, and that function f is also continuous. 

Proof. See Exercise 3.5.2. 

To put the Weierstrass M-test succinctly: absolute convergence of sup norms implies uniform convergence of functions. 

Example 3.5.8. Let $0 < r < 1$ be a real number, and let $f ^ { ( n ) } : [ - r , r ] \to$ R be the series of functions $f ^ { ( n ) } ( x ) : = x ^ { n }$ . Then each $f ^ { ( n ) }$ is continuous and bounded, and $\| f ^ { ( n ) } \| _ { \infty } = r ^ { n }$ (why?). Since the series $\textstyle \sum _ { n = 1 } ^ { \infty } r ^ { n }$ is absolutely convergent (e.g., by the ratio test, Theorem 7.5.1), we thus see that $f ^ { ( n ) }$ converges uniformly in $\left[ - r , r \right]$ to some continuous function; in Exercise $3 . 2 . 2 ( \mathrm { c } )$ we see that this function must in fact be the function $f : [ - r , r ] \to$ R defined by $f ( x ) : = x / ( 1 - x )$ . In other words, the series $\scriptstyle \sum _ { n = 1 } ^ { \infty } x ^ { n }$ is pointwise convergent, but not uniformly convergent, on $( - 1 , 1 )$ , but is uniformly convergent on the smaller interval $[ - r , r ]$ for any $0 < r < 1$ 

The Weierstrass M-test is especially useful in relation to power series, which we will encounter in the next chapter. 

$$
- \text { Exercises } -
$$

Exercise 3.5.1. Let $f ^ { ( 1 ) } , \ldots , f ^ { ( N ) }$ be a finite sequence of bounded functions from a metric space $( X , d _ { X } )$ to R. Show that $\textstyle \sum _ { i = 1 } ^ { N } f ^ { ( i ) }$ is also bounded. Prove a similar claim when “bounded” is replaced by “continuous”. What if “continuous” was replaced by “uniformly continuous”? 

Exercise 3.5.2. Prove Theorem 3.5.7. (Hint: first show that the sequence $\textstyle \sum _ { i = 1 } ^ { N } f ^ { ( i ) }$ is a Cauchy sequence in $C ( X  \mathbf { R } )$ . Then use Theorem 3.4.5.) 

## 3.6 Uniform convergence and integration

We now connect uniform convergence with Riemann integration (which was discussed in Chapter 11), by showing that uniform limits can be safely interchanged with integrals. 

Theorem 3.6.1. Let $[ a , b ]$ be an interval, and for each integer $n \geq 1$ • let $f ^ { ( n ) } : [ a , b ] \to \mathbf { R }$ be a Riemann-integrable function. Suppose $f ^ { ( n ) }$ converges uniformly on $[ a , b ]$ to a function $f : [ a , b ]  \mathbf { R }$ . Then f is also Riemann integrable, and 

$$
\lim _ {n \to \infty} \int_ {[ a, b ]} f ^ {(n)} = \int_ {[ a, b ]} f.
$$

Proof. We first show that $f$ is Riemann integrable on $[ a , b ]$ . This is the same as showing that the upper and lower Riemann integrals of $f$ match: $\underline { { \int } } _ { [ a , b ] } f = \overline { { \int } } _ { [ a , b ] } f .$ 

Let $\varepsilon > 0$ . Since $f ^ { ( n ) }$ converges uniformly to $f ,$ , we see that there exists an $N > 0$ such that $| f ^ { ( n ) } ( x ) - f ( x ) | < \varepsilon$ for all $n > N$ and $x \in [ a , b ]$ . In particular we have 

$$
f ^ {(n)} (x) - \varepsilon <   f (x) <   f ^ {(n)} (x) + \varepsilon
$$

for all $x \in [ a , b ]$ . Integrating this on $[ a , b ]$ we obtain 

$$
\int_ {\underline {{\quad}} [ a, b ]} (f ^ {(n)} - \varepsilon) \leq \int_ {\underline {{\quad}} [ a, b ]} f \leq \overline {{\int}} _ {[ a, b ]} f \leq \overline {{\int}} _ {[ a, b ]} (f ^ {(n)} + \varepsilon).
$$

Since $f ^ { ( n ) }$ is assumed to be Riemann integrable, we thus see 

$$
\left(\int_ {[ a, b ]} f ^ {(n)}\right) - \varepsilon (b - a) \leq \int_ {\underline {{\quad}} [ a, b ]} f \leq \overline {{\int_ {[ a , b ]}}} f \leq \left(\int_ {[ a, b ]} f ^ {(n)}\right) + \varepsilon (b - a).
$$

In particular, we see that 

$$
0 \leq \overline {{\int_ {[ a , b ]}}} f - \underline {{\int_ {[ a , b ]}}} f \leq 2 \varepsilon (b - a).
$$

Since this is true for every $\varepsilon > 0$ , we obtain $\underline { { \int } } _ { [ a , b ] } f = \overline { { \int } } _ { [ a , b ] } f$ as desired. 

The above argument also shows that for every $\varepsilon > 0$ there exists an $N > 0$ such that 

$$
\left| \int_ {[ a, b ]} f ^ {(n)} - \int_ {[ a, b ]} f \right| \leq 2 \varepsilon (b - a)
$$

for all $n \geq N$ . Since $\varepsilon$ is arbitrary, we see that $\begin{array} { r } { \int _ { [ a , b ] } f ^ { ( n ) } } \end{array}$ converges to $\int _ { [ a , b ] } f$ as desired. □ 

To rephrase Theorem 3.6.1: we can rearrange limits and integrals (on compact intervals $[ a , b ] )$ , 

$$
\lim _ {n \to \infty} \int_ {[ a, b ]} f ^ {(n)} = \int_ {[ a, b ]} \lim _ {n \to \infty} f ^ {(n)},
$$

provided that the convergence is uniform. This should be contrasted with Example 3.2.5 and Example 1.2.9. 

There is an analogue of this theorem for series: 

Corollary 3.6.2. Let $[ a , b ]$ be an interval, and let $( f ^ { ( n ) } ) _ { n = 1 } ^ { \infty }$ be a sequence of Riemann integrable functions on $[ a , b ]$ such that the series $\textstyle \sum _ { n = 1 } ^ { \infty } f ^ { ( n ) }$ is uniformly convergent. Then we have 

$$
\sum_ {n = 1} ^ {\infty} \int_ {[ a, b ]} f ^ {(n)} = \int_ {[ a, b ]} \sum_ {n = 1} ^ {\infty} f ^ {(n)}.
$$

Proof. See Exercise 3.6.1. 

This Corollary works particularly well in conjunction with the Weierstrass M-test (Theorem 3.5.7): 

Example 3.6.3. (Informal) From Lemma 7.3.3 we have the geometric series identity 

$$
\sum_ {n = 1} ^ {\infty} x ^ {n} = \frac {x}{1 - x}
$$

for $x \in ( - 1 , 1 )$ , and the convergence is uniform (by the Weierstrass M-test) on $[ - r , r ]$ for any $0 \textless r \textless 1$ . By adding 1 to both sides we obtain 

$$
\sum_ {n = 0} ^ {\infty} x ^ {n} = \frac {1}{1 - x}
$$

and the converge is again uniform. We can thus integrate on $[ 0 , r ]$ and use Corollary 3.6.2 to obtain 

$$
\sum_ {n = 0} ^ {\infty} \int_ {[ 0, r ]} x ^ {n} d x = \int_ {[ 0, r ]} \frac {1}{1 - x} d x.
$$

The left-hand side is $\textstyle \sum _ { n = 0 } ^ { \infty } r ^ { n + 1 } / ( n + 1 )$ . If we accept for now the use of logarithms (we will justify this use in Section 4.5), the anti-derivative of $1 / ( 1 - x ) { \mathrm { ~ i s ~ } } - \log ( 1 - x )$ , and so the right-hand side is $- \log ( 1 - r )$ We thus obtain the formula 

$$
- \log (1 - r) = \sum_ {n = 0} ^ {\infty} r ^ {n + 1} / (n + 1)
$$

for all $0 < r < 1$ 

— Exercises — 

Exercise 3.6.1. Use Theorem 3.6.1 to prove Corollary 3.6.2. 

## 3.7 Uniform convergence and derivatives

We have already seen how uniform convergence interacts well with continuity, with limits, and with integrals. Now we investigate how it interacts with derivatives. 

The first question we can ask is: if $f _ { n }$ converges uniformly to $f ,$ and the functions $f _ { n }$ are diferentiable, does this imply that f is also diferentiable? And does $f _ { n } ^ { \prime }$ also converge to $f ^ { \prime } { \ ? }$ 

The answer to the second question is, unfortunately, no. To see a counterexample, we will use without proof some basic facts about trigonometric functions (which we will make rigorous in Section 4.7). Consider the functions $f _ { n } : [ 0 , 2 \pi ] \to \mathbf { R }$ defined by $f _ { n } ( x ) \ : = \ n ^ { - 1 / 2 } \sin ( n x )$ , and let $f : [ 0 , 2 \pi ] \ \to \ \mathbf { R }$ be the zero function $f ( x ) : = 0$ . Then, since sin takes values between -1 and 1, we have $d _ { \infty } ( f _ { n } , f ) \le n ^ { - 1 / 2 }$ , where we use the uniform metric $d _ { \infty } ( f , g ) : =$ $\textstyle \operatorname* { s u p } _ { x \in [ 0 , 2 \pi ] } | f ( x ) - g ( x ) |$ introduced in Definintion 3.4.2. Since $n ^ { - 1 / 2 }$ converges to 0, we thus see by the squeeze test that $f _ { n }$ converges uniformly to f. On the other hand, $f _ { n } ^ { \prime } ( x ) = n ^ { 1 / 2 } \cos ( n x )$ , and so in particular $| f _ { n } ^ { \prime } ( 0 ) - f ^ { \prime } ( 0 ) | = n ^ { 1 / 2 }$ . Thus $f _ { n } ^ { \prime }$ does not converge pointwise to $f ^ { \prime }$ , and so in particular does not converge uniformly either. In particular we have 

$$
\frac {d}{d x} \lim _ {n \to \infty} f _ {n} (x) \neq \lim _ {n \to \infty} \frac {d}{d x} f _ {n} (x).
$$

The answer to the first question is also no. An example is the sequence of functions $f _ { n } : [ - 1 , 1 ] \to \mathbf { R }$ defined by $\begin{array} { r } { f _ { n } ( x ) : = \sqrt { \frac { 1 } { n ^ { 2 } } + x ^ { 2 } } } \end{array}$ These functions are diferentiable $\mathrm { \left( w h y ? \right) }$ . Also, one can easily check that 

$$
| x | \leq f _ {n} (x) \leq | x | + \frac {1}{n}
$$

for all $x \in [ - 1 , 1 ]$ (why? square both sides), and so by the squeeze test $f _ { n }$ converges uniformly to the absolute value function $f ( x ) : = | x |$ . But this function is not diferentiable at 0 (why?). Thus, the uniform limit of diferentiable functions need not be diferentiable. (See also Example 1.2.10). 

So, in summary, uniform convergence of the functions $f _ { n }$ says nothing about the convergence of the derivatives $f _ { n } ^ { \prime }$ . However, the converse is true, as long as $f _ { n }$ converges at at least one point: 

Theorem 3.7.1. Let $[ a , b ]$ be an interval, and for every integer $n \geq 1$ , let $f _ { n } : [ a , b ] \to \mathbf { R }$ be a diferentiable function whose derivative $f _ { n } ^ { \prime } : [ a , b ] \to$ R is continuous. Suppose that the derivatives $f _ { n } ^ { \prime }$ converge uniformly to a function $g : [ a , b ]  \mathbf { R }$ . Suppose also that there exists a point x<sub>0</sub> such that the limit $\scriptstyle \operatorname* { l i m } _ { n \to \infty } f _ { n } ( x _ { 0 } )$ exists. Then the functions $f _ { n }$ converge uniformly to a diferentiable function $f$ , and the derivative of f equals g. 

Informally, the above theorem says that if $f _ { n } ^ { \prime }$ converges uniformly, and $f _ { n } ( x _ { 0 } )$ converges for some $x _ { 0 }$ , then $f _ { n }$ also converges uniformly, and $\begin{array} { r } { \frac { d } { d x } \operatorname* { l i m } _ { n  \infty } f _ { n } ( x ) = \operatorname* { l i m } _ { n  \infty } \frac { d } { d x } f _ { n } ( x ) } \end{array}$ 

Proof. We only give the beginning of the proof here; the remainder of the proof will be an exercise (Exercise 3.7.1). 

Since $f _ { n } ^ { \prime }$ is continuous, we see from the fundamental theorem of calculus (Theorem 11.9.4) that 

$$
f _ {n} (x) - f _ {n} (x _ {0}) = \int_ {[ x _ {0}, x ]} f _ {n} ^ {\prime}
$$

when $x \in [ x _ { 0 } , b ]$ , and 

$$
f _ {n} (x) - f _ {n} (x _ {0}) = - \int_ {[ x, x _ {0} ]} f _ {n} ^ {\prime}
$$

when $x \in [ a , x _ { 0 } ]$ 

Let L be the limit of $f _ { n } ( x _ { 0 } )$ as $n \to \infty$ 

$$
L := \lim _ {n \to \infty} f _ {n} (x _ {0}).
$$

By hypothesis, L exists. Now, since each $f _ { n } ^ { \prime }$ is continuous on $[ a , b ]$ , and $f _ { n } ^ { \prime }$ converges uniformly to $g ,$ we see by Corollary 3.3.2 that g is also continuous. Now define the function $f : [ a , b ]  \mathbf { R }$ by setting 

$$
f (x) := L - \int_ {[ a, x _ {0} ]} g + \int_ {[ a, x ]} g
$$

for all $x \in [ a , b ]$ . To finish the proof, we have to show that $f _ { n }$ converges uniformly to $f _ { : }$ , and that $f$ is diferentiable with derivative $g ;$ this shall be done in Exercise 3.7.1. □ 

Remark 3.7.2. It turns out that Theorem 3.7.1 is still true when the functions $f _ { n } ^ { \prime }$ are not assumed to be continuous, but the proof is more dificult; see Exercise 3.7.2. 

By combining this theorem with the Weierstrass M-test, we obtain 

Corollary 3.7.3. Let $[ a , b ]$ be an interval, and for every integer $n \geq 1$ , let $f _ { n } : [ a , b ] \to \mathbf { R }$ be a diferentiable function whose derivative $f _ { n } ^ { \prime }$ $[ a , b ] \to \mathbf { R }$ is continuous. Suppose that the series $\scriptstyle \sum _ { n = 1 } ^ { \infty } \| f _ { n } ^ { \prime } \| _ { \infty }$ is absolutely convergent, where 

$$
\| f _ {n} ^ {\prime} \| _ {\infty} := \sup _ {x \in [ a, b ]} | f _ {n} ^ {\prime} (x) |
$$

is the sup norm of $f _ { n } ^ { \prime }$ , as defined in Definition 3.5.5. Suppose also that the series $\scriptstyle \sum _ { n = 1 } ^ { \infty } f _ { n } ( x _ { 0 } )$ is convergent for some $x _ { 0 } ~ \in ~ [ a , b ]$ . Then the series $\textstyle \sum _ { n = 1 } ^ { \infty } { \ddot { f _ { n } } }$ converges uniformly on $[ a , b ]$ to a diferentiable function, and in fact 

$$
{\frac {d}{d x}} \sum_ {n = 1} ^ {\infty} f _ {n} (x) = \sum_ {n = 1} ^ {\infty} {\frac {d}{d x}} f _ {n} (x)
$$

for all $x \in [ a , b ]$ 

Proof. See Exercise 3.7.3. 

We now pause to give an example of a function which is continuous everywhere, but diferentiable nowhere (this particular example was discovered by Weierstrass). Again, we will presume knowledge of the trigonometric functions, which will be covered rigorously in Section 4.7. 

Example 3.7.4. Let $f : \mathbf { R }  \mathbf { R }$ be the function 

$$
f (x) := \sum_ {n = 1} ^ {\infty} 4 ^ {- n} \cos (3 2 ^ {n} \pi x).
$$

Note that this series is uniformly convergent, thanks to the Weierstrass M-test, and since each individual function $4 ^ { - n } \cos ( 3 2 ^ { n } \pi x )$ is continuous, the function f is also continuous. However, it is not diferentiable (Exercise 4.7.10); in fact it is a nowhere diferentiable function, one which is not diferentiable at any point, despite being continuous everywhere! 

— Exercises — 

Exercise 3.7.1. Complete the proof of Theorem 3.7.1. Compare this theorem with Example 1.2.10, and explain why this example does not contradict the theorem. 

Exercise 3.7.2. Prove Theorem 3.7.1 without assuming that $f _ { n } ^ { \prime }$ is continuous. (This means that you cannot use the fundamental theorem of calculus. However, the mean value theorem (Corollary 10.2.9) is still available. Use this to show that if $d _ { \infty } ( f _ { n } ^ { \prime } , f _ { m } ^ { \prime } ) \leq \varepsilon .$ , then $| ( f _ { n } ( x ) - { \dot { f _ { m } } } ( x ) ) - ( f _ { n } ( x _ { 0 } ) - f _ { m } ( x _ { 0 } ) ) | \ \leq$ $\varepsilon | x - x _ { 0 } |$ for all $x \in [ a , b ]$ , and then use this to complete the proof of Theorem 3.7.1.) 

Exercise 3.7.3. Prove Corollary 3.7.3. 

## 3.8 Uniform approximation by polynomials

As we have just seen, continuous functions can be very badly behaved, for instance they can be nowhere diferentiable (Example 3.7.4). On the other hand, functions such as polynomials are always very well behaved, in particular being always diferentiable. Fortunately, while most continuous functions are not as well behaved as polynomials, they can always be uniformly approximated by polynomials; this important (but dificult) result is known as the Weierstrass approximation theorem, and is the subject of this section. 

Definition 3.8.1. Let $[ a , b ]$ be an interval. A polynomial on $[ a , b ]$ is a function $f : [ a , b ]  \mathbf { R }$ of the form $\textstyle f ( x ) : = \sum _ { i = 0 } ^ { n } c _ { j } x ^ { j }$ , where $n \geq 0$ is an integer and $c _ { 0 } , \ldots , c _ { n }$ are real numbers. If $c _ { n } \neq 0$ , then n is called the degree of f. 

Example 3.8.2. The function $f : [ 1 , 2 ]  \mathbf { R }$ defined by $f ( x ) : = 3 x ^ { 4 } + \quad$ $2 x ^ { 3 } - 4 x + 5$ is a polynomial on $[ 1 , 2 ]$ of degree 4. 

Theorem 3.8.3 (Weierstrass approximation theorem). $I f \ [ a , b ]$ is an interval, $f : [ a , b ]  \mathbf { R }$ is a continuous function, and $\varepsilon > 0$ , then there exists a polynomial P on $[ a , b ]$ such that $d _ { \infty } ( P , f ) \leq \varepsilon \ ( i . e . , \ | P ( x ) -$ $f ( x ) | \leq \varepsilon$ for all $x \in [ a , b ] )$ 

Another way of stating this theorem is as follows. Recall that $C ( [ a , b ]  \mathbf { R } )$ was the space of continuous functions from $[ a , b ]$ to R, with the uniform metric $d _ { \infty }$ . Let $P ( [ a , b ] \  \ \mathbf { R } )$ be the space of all polynomials on $[ a , b ]$ ; this is a subspace of $C ( [ a , b ]  \mathbf { R } )$ , since all polynomials are continuous (Exercise 9.4.7). The Weierstrass approximation theorem then asserts that every continuous function is an adherent point of $P ( [ a , b ]  \mathbf { R } )$ ; or in other words, that the closure of the space of polynomials is the space of continuous functions: 

$$
\overline {{P ([ a , b ] \to {\bf R})}} = C ([ a, b ] \to {\bf R}).
$$

In particular, every continuous function on $[ a , b ]$ is the uniform limit of polynomials. Another way of saying this is that the space of polynomials is dense in the space of continuous functions, in the uniform topology. 

The proof of the Weierstrass approximation theorem is somewhat complicated and will be done in stages. We first need the notion of an approximation to the identity. 

Definition 3.8.4 (Compactly supported functions). Let $[ a , b ]$ be an interval. A function $f : \mathbf { R }  \mathbf { R }$ is said to be supported on $[ a , b ]$ if $f ( x ) = 0$ for all $x \not \in [ a , b ]$ . We say that f is compactly supported if it is supported on some interval $[ a , b ]$ . If f is continuous and supported on $[ a , b ]$ , we define the improper integral $\textstyle \int _ { - \infty } ^ { \infty } f$ to be $\textstyle { \int _ { - \infty } ^ { \infty } f : = \int _ { [ a , b ] } f }$ 

Note that a function can be supported on more than one interval, for instance a function which is supported on $[ 3 , 4 ]$ is also automatically supported on [2, 5] (why?). In principle, this might mean that our definition of $\textstyle \int _ { - \infty } ^ { \infty } f$ is not well defined, however this is not the case: 

Lemma 3.8.5. If $f : \mathbf { R }  \mathbf { R }$ is continuous and supported on an interval $[ a , b ]$ , and is also supported on another interval $[ c , d ]$ , then $\begin{array} { r } { \int _ { [ a , b ] } f = } \end{array}$ $\textstyle \int _ { [ c , d ] } f$ 

Proof. See Exercise 3.8.1. 

Definition 3.8.6 (Approximation to the identity). Let $\varepsilon > 0$ and $0 <$ $\delta < 1$ . A function $f : \mathbf { R }  \mathbf { R }$ is said to be an $( \varepsilon , \delta )$ )-approximation to the identity if it obeys the following three properties: 

(a) f is supported on $[ - 1 , 1 ]$ , and $f ( x ) \geq 0$ for all $- 1 \leq x \leq 1$ 

(b) f is continuous, and $\textstyle \int _ { - \infty } ^ { \infty } f = 1$ 

(c) $| f ( x ) | \leq \varepsilon$ for all $\delta \leq | x | \leq 1$ 

Remark 3.8.7. For those of you who are familiar with the Dirac delta function, approximations to the identity are ways to approximate this (very discontinuous) delta function by a continuous function (which is easier to analyze). We will not however discuss the Dirac delta function in this text. 

Our proof of the Weierstrass approximation theorem relies on three key facts. The first fact is that polynomials can be approximations to the identity: 

Lemma 3.8.8 (Polynomials can approximate the identity). For every $\varepsilon > 0$ and $0 < \delta < 1$ there exists an $( \varepsilon , \delta )$ -approximation to the identity which is a polynomial P on $[ - 1 , 1 ]$ 

Proof. See Exercise 3.8.2. 

We will use these polynomial approximations to the identity to approximate continuous functions by polynomials. We will need the following important notion of a convolution. 

Definition 3.8.9 (Convolution). Let $f : \mathbf { R }  \mathbf { R }$ and $g : \mathbf { R }  \mathbf { R }$ be continuous, compactly supported functions. We define the convolution $f * g : \mathbf { R }  \mathbf { R }$ of f and g to be the function 

$$
(f * g) (x) := \int_ {- \infty} ^ {\infty} f (y) g (x - y) d y.
$$

Note that if f and $g$ are continuous and compactly supported, then for each x the function $f ( y ) g ( x - y )$ (thought of as a function of $y )$ is also continuous and compactly supported, so the above definition makes sense. 

Remark 3.8.10. Convolutions play an important rˆole in Fourier analysis and in partial diferential equations (PDE), and are also important in physics, engineering, and signal processing. An in-depth study of convolution is beyond the scope of this text; only a brief treatment will be given here. 

Proposition 3.8.11 (Basic properties of convolution). Let $f : \mathbf { R } $ R, $g : \mathbf { R }  \mathbf { R }$ , and $h : \mathbf { R }  \mathbf { R }$ be continuous, compactly supported functions. Then the following statements are true. 

(a) The convolution $f * g$ is also a continuous, compactly supported function. 

(b) (Convolution is commutative) We have $f { * } g = g { * } f .$ ; in other words 

$$
\begin{array}{c} f * g (x) = \int_ {- \infty} ^ {\infty} f (y) g (x - y) d y \\ = \int_ {- \infty} ^ {\infty} g (y) f (x - y) d y \\ = g * f (x). \end{array}
$$

(c) (Convolution is linear) We have $f * ( g + h ) = f * g + f * h$ . Also, for any real number c, we have $f * ( c g ) = ( c f ) * g = c ( f * g )$ 

Proof. See Exercise 3.8.4. 

Remark 3.8.12. There are many other important properties of convolution, for instance it is associative, $( f * g ) * h = f * ( g * h )$ , and it commutes with derivatives, $( f * g ) ^ { \prime } = f ^ { \prime } * g = f * g ^ { \prime }$ , when f and g are diferentiable. The Dirac delta function δ mentioned earlier is an identity for convolution: $f * \delta = \delta * f = f$ . These results are slightly harder to prove than the ones in Proposition 3.8.11, however, and we will not need them in this text. 

As mentioned earlier, the proof of the Weierstrass approximation theorem relies on three facts. The second key fact is that convolution with polynomials produces another polynomial: 

Lemma 3.8.13. Let $f : \mathbf { R }  \mathbf { R }$ be a continuous function supported on [0, 1], and let $g : \mathbf { R }  \mathbf { R }$ be a continuous function supported on $[ - 1 , 1 ]$ which is a polynomial on $[ - 1 , 1 ]$ . Then f g is a polynomial on [0, 1]. (Note however that it may be non-polynomial outside of $\left[ 0 , 1 \right] . \jmath ^ { }$ 

Proof. Since g is polynomial on $[ - 1 , 1 ]$ , we may find an integer $n \geq 0$ and real numbers $c _ { 0 } , c _ { 1 } , \ldots , c _ { n }$ such that 

$$
g (x) = \sum_ {j = 0} ^ {n} c _ {j} x ^ {j} \text {   for   all   } x \in [ - 1, 1 ].
$$

On the other hand, for all $x \in [ 0 , 1 ]$ , we have 

$$
f * g (x) = \int_ {- \infty} ^ {\infty} f (y) g (x - y) d y = \int_ {[ 0, 1 ]} f (y) g (x - y) d y
$$

since $f$ is supported on [0, 1]. Since $x \in [ 0 , 1 ]$ and the variable of integration y is also in [0, 1], we have $x - y \in [ - 1 , 1 ]$ . Thus we may substitute in our formula for g to obtain 

$$
f * g (x) = \int_ {[ 0, 1 ]} f (y) \sum_ {j = 0} ^ {n} c _ {j} (x - y) ^ {j} d y.
$$

We expand this using the binomial formula (Exercise 7.1.4) to obtain 

$$
f * g (x) = \int_ {[ 0, 1 ]} f (y) \sum_ {j = 0} ^ {n} c _ {j} \sum_ {k = 0} ^ {j} \frac {j !}{k ! (j - k) !} x ^ {k} (- y) ^ {j - k} d y.
$$

We can interchange the two summations (by Corollary 7.1.14) to obtain 

$$
f * g (x) = \int_ {[ 0, 1 ]} f (y) \sum_ {k = 0} ^ {n} \sum_ {j = k} ^ {n} c _ {j} \frac {j !}{k ! (j - k) !} x ^ {k} (- y) ^ {j - k} d y
$$

(why did the limits of summation change? It may help to plot $j$ and k on a graph). Now we interchange the k summation with the integral, and observe that $x ^ { k }$ is independent of $y .$ to obtain 

$$
f * g (x) = \sum_ {k = 0} ^ {n} x ^ {k} \int_ {[ 0, 1 ]} f (y) \sum_ {j = k} ^ {n} c _ {j} \frac {j !}{k ! (j - k) !} (- y) ^ {j - k} d y.
$$

If we thus define 

$$
C _ {k} := \int_ {[ 0, 1 ]} f (y) \sum_ {j = k} ^ {n} c _ {j} \frac {j !}{k ! (j - k) !} (- y) ^ {j - k} d y
$$

for each $k = 0 , \ldots , n$ , then $C _ { k }$ is a number which is independent of $x ,$ and we have 

$$
f * g (x) = \sum_ {k = 0} ^ {n} C _ {k} x ^ {k}
$$

for all $x \in [ 0 , 1 ]$ . Thus $f * g$ is a polynomial on $[ 0 , 1 ]$ 

The third key fact is that if one convolves a uniformly continuous function with an approximation to the identity, we obtain a new function which is close to the original function (which explains the terminology “approximation to the identity”): 

Lemma 3.8.14. Let $f : \mathbf { R }  \mathbf { R }$ be a continuous function supported on $[ 0 , 1 ]$ , which is bounded by some $M > 0 \ ( i . e . , \ | f ( x ) | \leq M$ for all $x \in \mathbf { R } )$ ), and let $\varepsilon > 0$ and $0 < \delta < 1$ be such that one has $| f ( x ) - f ( y ) | < \varepsilon$ whenever $x , y \in \mathbf { R }$ and $| x - y | < \delta$ . Let g be any (ε, δ)-approximation to the identity. Then we have 

$$
| f * g (x) - f (x) | \leq (1 + 4 M) \varepsilon
$$

for all $x \in [ 0 , 1 ]$ 

Proof. See Exercise 3.8.6. 

## 3.8. Uniform approximation by polynomials

Combining these together, we obtain a preliminary version of the Weierstrass approximation theorem: 

Corollary 3.8.15 (Weierstrass approximation theorem I). Let $f : \mathbf { R } $ R be a continuous function supported on [0, 1]. Then for every $\varepsilon > 0$ there exists a function $P : \mathbf { R }  \mathbf { R }$ which is polynomial on [0, 1] and such that $| P ( x ) - f ( x ) | \leq \varepsilon$ for all $x \in [ 0 , 1 ]$ 

Proof. See Exercise 3.8.7. 

Now we perform a series of modifications to convert Corollary 3.8.15 into the actual Weierstrass approximation theorem. We first need a simple lemma. 

Lemma 3.8.16. Let $f : [ 0 , 1 ] \to \mathbf { R }$ be a continuous function which equals 0 on the boundary of [0, 1], i.e., $f ( 0 ) = f ( 1 ) = 0$ . Let $F : \mathbf { R } $ R be the function defined by setting $F ( x ) : = f ( x ) \ f o r \ x \ \in \ [ 0 , 1 ]$ and $F ( x ) : = 0$ for $x \notin [ 0 , 1 ]$ . Then F is also continuous. 

Proof. See Exercise 3.8.9. 

Remark 3.8.17. The function F obtained in Lemma 3.8.16 is sometimes known as the extension of f by zero. 

From Corollary 3.8.15 and Lemma 3.8.16 we immediately obtain 

Corollary 3.8.18 (Weierstrass approximation theorem II). Let $f :$ $[ 0 , 1 ] \  \ \textbf { R }$ be a continuous function supported on [0, 1] such that $f ( 0 ) = f ( 1 ) = 0$ Then for every $\varepsilon \ > \ 0$ there exists a polynomial $P : [ 0 , 1 ]  \mathbf { R }$ such that $| P ( x ) - f ( x ) | \leq \varepsilon$ for all $x \in [ 0 , 1 ]$ 

Now we strengthen Corollary 3.8.18 by removing the assumption that $f ( 0 ) = f ( 1 ) = 0$ 

Corollary 3.8.19 (Weierstrass approximation theorem III). Let f : $[ 0 , 1 ]  \mathbf { R }$ be a continuous function supported on [0, 1]. Then for every $\varepsilon > 0$ there exists a polynomial $P : [ 0 , 1 ] \to \mathbf { R }$ such that $| P ( x ) - f ( x ) | \leq \varepsilon$ for all $x \in [ 0 , 1 ]$ 

Proof. Let $F : [ 0 , 1 ]  \mathbf { R }$ denote the function 

$$
F (x) := f (x) - f (0) - x (f (1) - f (0)).
$$

Observe that $F$ is also continuous $\mathrm { \left( w h y ? \right) }$ , and that $F ( 0 ) = F ( 1 ) = 0$ By Corollary 3.8.18, we can thus find a polynomial $Q : [ 0 , 1 ]  \mathbf { R }$ such that $| Q ( x ) - F ( x ) | \leq \varepsilon$ for all $x \in [ 0 , 1 ]$ . But 

$$
Q (x) - F (x) = Q (x) + f (0) + x (f (1) - f (0)) - f (x),
$$

so the claim follows by setting $P$ to be the polynomial $P ( x ) : = Q ( x ) +$ $f ( 0 ) + x ( f ( 1 ) - f ( 0 ) )$ □ 

Finally, we can prove the full Weierstrass approximation theorem. 

Proof of Theorem 3.8.3. Let $f : [ a , b ]  \mathbf { R }$ be a continuous function on $[ a , b ]$ . Let $g : [ 0 , 1 ]  \mathbf { R }$ denote the function 

$$
g (x) := f (a + (b - a) x) \text {   for   all   } x \in [ 0, 1 ]
$$

Observe then that 

$$
f (y) = g ((y - a) / (b - a)) \text {   for   all   } y \in [ a, b ].
$$

The function $g$ is continuous on $[ 0 , 1 ] \ \mathrm { ( w h y ? ) }$ , and so by Corollary 3.8.19 we may find a polynomial $Q : [ 0 , 1 ]  \mathbf { R }$ such that $| Q ( x ) - g ( x ) | \leq \varepsilon$ for all $x \in [ 0 , 1 ]$ . In particular, for any $y \in [ a , b ]$ , we have 

$$
\left| Q \left(\left(y - a\right) / (b - a)\right) - g \left(\left(y - a\right) / (b - a)\right) \right| \leq \varepsilon .
$$

If we thus set $P ( y ) : = Q ( ( y - a ) / ( b - a ) )$ , then we observe that P is also a polynomial (why?), and so we have $| P ( y ) - f ( y ) | \leq \varepsilon$ for all $y \in [ a , b ]$ , as desired. □ 

Remark 3.8.20. Note that the Weierstrass approximation theorem only works on bounded intervals $[ a , b ]$ ; continuous functions on R cannot be uniformly approximated by polynomials. For instance, the exponential function $f : \mathbf { R }  \mathbf { R }$ defined by $f ( x ) : = e ^ { x }$ (which we shall study rigorously in Section 4.5) cannot be approximated by any polynomial, because exponential functions grow faster than any polynomial (Exercise 4.5.9) and so there is no way one can even make the sup metric between $f$ and a polynomial finite. 

Remark 3.8.21. There is a generalization of the Weierstrass approximation theorem to higher dimensions: if K is any compact subset of $\mathbf { R } ^ { n }$ (with the Euclidean metric $d _ { l ^ { 2 } } )$ , and $f : K  \mathbf { R }$ is a continuous function, then for every $\varepsilon > 0$ there exists a polynomial $P : K  \mathbf { R }$ of n variables $x _ { 1 } , \ldots , x _ { n }$ such that $d _ { \infty } ( f , P ) < \varepsilon$ . This general theorem can be proven by a more complicated variant of the arguments here, but we will not do so. (There is in fact an even more general version of this theorem applicable to an arbitrary metric space, known as the Stone-Weierstrass theorem, but this is beyond the scope of this text.) 

— Exercises — 

Exercise 3.8.1. Prove Lemma 3.8.5. 

Exercise 3.8.2. (a) Prove that for any real number $0 \leq y \leq 1$ and any natural number $n \geq 0$ , that $( 1 - y ) ^ { n } \geq 1 - n y$ . (Hint: induct on n. Alternatively, diferentiate with respect to y.) 

(b) Show that $\textstyle \int _ { - 1 } ^ { 1 } ( 1 - x ^ { 2 } ) ^ { n } \ d x \geq { \frac { 1 } { \sqrt { n } } }$ . (Hint: for $| x | \leq 1 / { \sqrt { n } }$ , use part (a); for $| x | \geq 1 / { \sqrt { n } }$ , just use the fact that $( 1 - x ^ { 2 } )$ is positive. It is also possible to proceed via trigonometric substitution, but I would not recommend this unless you know what you are doing.) 

(c) Prove Lemma 3.8.8. (Hint: choose $f ( x )$ to equal $c ( 1 - x ^ { 2 } ) ^ { N }$ for $x \in [ - 1 , 1 ]$ and to equal zero for $x \notin [ - 1 , 1 ]$ , where N is a large number $N _ { : }$ where c is chosen so that f has integral 1, and use (b).) 

Exercise 3.8.3. Let $f : \mathbf { R }  \mathbf { R }$ be a compactly supported, continuous function. Show that f is bounded and uniformly continuous. (Hint: the idea is to use Proposition 2.3.2 and Theorem 2.3.5, but one must first deal with the issue that the domain R of f is non-compact.) 

Exercise 3.8.4. Prove Proposition 3.8.11. (Hint: to show that f g is continuous, use Exercise 3.8.3.) 

Exercise 3.8.5. Let $f : \mathbf { R }  \mathbf { R }$ and $g : \mathbf { R }  \mathbf { R }$ be continuous, compactly supported functions. Suppose that f is supported on the interval [0, 1], and g is constant on the interval [0, 2] (i.e., there is a real number c such that $g ( x ) = c$ for all $x \in [ 0 , 2 ] )$ . Show that the convolution $f * g$ is constant on the interval [1, 2]. 

Exercise 3.8.6. (a) Let g be an $( \varepsilon , \delta )$ approximation to the identity. Show that $\begin{array} { r } { 1 - 2 \varepsilon \le \int _ { [ - \delta , \delta ] } g \le 1 . } \end{array}$ 

(b) Prove Lemma 3.8.14. (Hint: begin with the identity 

$$
\begin{array}{l} f * g (x) = \int f (x - y) g (y) d y = \int_ {[ - \delta , \delta ]} f (x - y) g (y) d y \\ \qquad + \int_ {[ \delta , 1 ]} f (x - y) g (y) d y + \int_ {[ - 1, - \delta ]} f (x - y) g (y) d y. \end{array}
$$

The idea is to show that the first integral is close to $f ( x )$ , and that the second and third integrals are very small. To achieve the former task, use (a) and the fact that $f ( x )$ and $f ( x - y )$ are within $\varepsilon$ of each other; to achieve the latter task, use property (c) of the approximation to the identity and the fact that $f$ is bounded.) 

Exercise 3.8.7. Prove Corollary 3.8.15. (Hint: combine Exercise 3.8.3, Lemma 3.8.8, Lemma 3.8.13, and Lemma 3.8.14.) 

Exercise 3.8.8. Let $f : [ 0 , 1 ] \to \mathbf { R }$ be a continuous function, and suppose that $\int _ { [ 0 , 1 ] } f ( x ) x ^ { n }$ dx = 0 for all non-negative integers $n = 0 , 1 , 2 , \ldots$ Show that $f$ must be the zero function $f \equiv 0$ . (Hint: first show that $\textstyle \int _ { [ 0 , 1 ] } f ( x ) P ( x ) \ d x = 0$ for all polynomials P. Then, using the Weierstrass approximation theorem, show that $\begin{array} { r } { \int _ { [ 0 , 1 ] } f ( x ) f ( x ) d x = 0 . ) } \end{array}$ 

Exercise 3.8.9. Prove Lemma 3.8.16. 

## Chapter 4

## Power series

## 4.1 Formal power series

We now discuss an important subclass of series of functions, that of power series. As in earlier chapters, we begin by introducing the notion of a formal power series, and then focus in later sections on when the series converges to a meaningful function, and what one can say about the function obtained in this manner. 

Definition 4.1.1 (Formal power series). Let a be a real number. A formal power series centered at a is any series of the form 

$$
\sum_ {n = 0} ^ {\infty} c _ {n} (x - a) ^ {n}
$$

where $c _ { 0 } , c _ { 1 } , \ldots .$ . is a sequence of real numbers (not depending on $x )$ ; we refer to $c _ { n }$ as the $n ^ { t h }$ coeficient of this series. Note that each term $c _ { n } ( x - a ) ^ { n }$ in this series is a function of a real variable x. 

Example 4.1.2. The series $\scriptstyle \sum _ { n = 0 } ^ { \infty } n ! ( x - 2 ) ^ { n }$ is a formal power series centered at 2. The series $\scriptstyle \sum _ { n = 0 } ^ { \infty } 2 ^ { x } ( x - 3 ) ^ { n }$ is not a formal power series, since the coeficients $2 ^ { x }$ depend on x. 

We call these power series formal because we do not yet assume that these series converge for any x. However, these series are automatically guaranteed to converge when $x = a \mathrm { \ ( w h y ? ) }$ . In general, the closer x gets to $^ { a , }$ the easier it is for this series to converge. To make this more precise, we need the following definition. 

Definition 4.1.3 (Radius of convergence). Let $\textstyle \sum _ { n = 0 } ^ { \infty } c _ { n } ( x - a ) ^ { n }$ be a formal power series. We define the radius of convergence R of this series 

to be the quantity 

$$
R := \frac {1}{\limsup _ {n \to \infty} | c _ {n} | ^ {1 / n}}
$$

where we adopt the convention that $\textstyle { \frac { 1 } { 0 } } = + \infty$ and $\begin{array} { r } { \frac { 1 } { + \infty } = 0 } \end{array}$ 

Remark 4.1.4. Each number $| c _ { n } | ^ { 1 / n }$ is non-negative, so the limit lim $\mathrm { s u p } _ { n  \infty } | c _ { n } | ^ { 1 / n }$ can take on any value from $0 ~ \mathrm { t o } + \infty$ , inclusive. Thus R can also take on any value between 0 and + inclusive (in particular it is not necessarily a real number). Note that the radius of convergence always exists, even if the sequence $| c _ { n } | ^ { 1 / n }$ is not convergent, because the lim sup of any sequence always exists (though it might be $+ \infty \ \mathrm { o r \ - \infty } )$ 

Example 4.1.5. The series $\scriptstyle \sum _ { n = 0 } ^ { \infty } n ( - 2 ) ^ { n } ( x - 3 ) ^ { n }$ has radius of convergence 

$$
\frac {1}{\limsup _ {n \to \infty} | n (- 2 ^ {n}) | ^ {1 / n}} = \frac {1}{\limsup _ {n \to \infty} 2 n ^ {1 / n}} = \frac {1}{2}.
$$

The series $\scriptstyle \sum _ { n = 0 } ^ { \infty } 2 ^ { n ^ { 2 } } ( x + 2 ) ^ { n }$ has radius of convergence 

$$
\frac {1}{\limsup _ {n \to \infty} | 2 ^ {n ^ {2}} | ^ {1 / n}} = \frac {1}{\limsup _ {n \to \infty} 2 ^ {n}} = \frac {1}{+ \infty} = 0.
$$

The series $\scriptstyle \sum _ { n = 0 } ^ { \infty } 2 ^ { - n ^ { 2 } } ( x + 2 ) ^ { n }$ has radius of convergence 

$$
\frac {1}{\limsup _ {n \to \infty} | 2 ^ {- n ^ {2}} | ^ {1 / n}} = \frac {1}{\limsup _ {n \to \infty} 2 ^ {- n}} = \frac {1}{0} = + \infty .
$$

The significance of the radius of convergence is the following. 

Theorem 4.1.6. Let $\textstyle \sum _ { n = 0 } ^ { \infty } c _ { n } ( x - a ) ^ { n }$ be a formal power series, and let R be its radius of convergence. 

(a) (Divergence outside of the radius of convergence) If $x \in \mathbf { R }$ is such that $| x - a | > R$ , then the series $\textstyle \sum _ { n = 0 } ^ { \infty } c _ { n } ( x - a ) ^ { n }$ is divergent for that value of x. 

(b) (Convergence inside the radius of convergence) If $x \in \mathbf { R }$ is such that $| x - a | < R$ , then the series $\textstyle \sum _ { n = 0 } ^ { \infty } c _ { n } ( x - a ) ^ { n }$ is absolutely convergent for that value of x. 

For parts $( c ) \ – ( e )$ we assume that $R > 0 \ ( i . e .$ , the series converges at at least one other point than $x = a )$ . Let $f : ( a - R , a + R )  \mathbf { R }$ be the 

## 4.1. Formal power series

function $\textstyle f ( x ) : = \sum _ { n = 0 } ^ { \infty } c _ { n } ( x - a ) ^ { n }$ ; this function is guaranteed to exist by (b). 

(c) (Uniform convergence on compact sets) For any $0 < r < R$ , the series $\textstyle \sum _ { n = 0 } ^ { \infty } c _ { n } ( x - a ) ^ { n }$ converges uniformly to f on the compact interval $[ a - r , a + r ]$ . In particular, f is continuous on $( a - R , a + R )$ 

(d) (Diferentiation of power series) The function f is diferentiable on $( a - R , a + R )$ , and for any $0 < r < R$ , the series $\scriptstyle \sum _ { n = 1 } ^ { \infty } n c _ { n } ( x -$ $a ) ^ { n - 1 }$ converges uniformly to f on the interval $[ \boldsymbol { a } - \boldsymbol { r } , \boldsymbol { a } + \boldsymbol { r } ]$ 

(e) (Integration of power series) For any closed interval $[ y , z ]$ contained in $( a - R , a + R )$ , we have 

$$
\int_ {[ y, z ]} f = \sum_ {n = 0} ^ {\infty} c _ {n} \frac {(z - a) ^ {n + 1} - (y - a) ^ {n + 1}}{n + 1}.
$$

Proof. See Exercise 4.1.1. 

Theorem 4.1.6 (a) and (b) of the above theorem give another way to find the radius of convergence, by using your favorite convergence test to work out the range of x for which the power series converges: 

Example 4.1.7. Consider the power series $\textstyle \sum _ { n = 0 } ^ { \infty } n ( x - 1 ) ^ { n }$ . The ratio test shows that this series converges when $| x - 1 | < 1$ and diverges when $| x - 1 | > 1$ (why?). Thus the only possible value for the radius of convergence is $R = 1 { \mathrm { ~ ( i f ~ } } R < 1$ , then we have contradicted Theorem $4 . 1 . 6 ( \mathrm { a } )$ ; if $R > 1$ , then we have contradicted Theorem 4.1.6(b)). 

Remark 4.1.8. Theorem 4.1.6 is silent on what happens when $| x - a | =$ R, i.e., at the points $a - R$ and $a + R .$ . Indeed, one can have either convergence or divergence at those points; see Exercise 4.1.2. 

Remark 4.1.9. Note that while Theorem 4.1.6 assures us that the power series $\textstyle \sum _ { n = 0 } ^ { \infty } c _ { n } ( x - a ) ^ { n }$ will converge pointwise on the interval $( a - R , a + R )$ , it need not converge uniformly on that interval (see Exercise 4.1.2(e)). On the other hand, Theorem 4.1.6(c) assures us that the power series will converge on any smaller interval $[ \boldsymbol { a } - \boldsymbol { r } , \boldsymbol { a } + \boldsymbol { r } ]$ . In particular, being uniformly convergent on every closed subinterval of $( a - R , a + R )$ is not enough to guarantee being uniformly convergent on all of $( a - R , a + R )$ 

— Exercises — 

Exercise 4.1.1. Prove Theorem 4.1.6. (Hints: for (a) and (b), use the root test (Theorem 7.5.1). For (c), use the Weierstrass M-test (Theorem 3.5.7). For (d), use Theorem 3.7.1. For (e), use Corollary 3.6.2. 

Exercise 4.1.2. Give examples of a formal power series $\scriptstyle \sum _ { n = 0 } ^ { \infty } c _ { n } x ^ { n }$ centered at 0 with radius of convergence 1, which 

(a) diverges at both x = 1 and $x = - 1$ ; 

(b) diverges at $x = 1$ but converges at $x = - 1$ ; 

(c) converges at x = 1 but diverges at $x = - 1 ;$ ; 

(d) converges at both x = 1 and $x = - 1$ 

(e) converges pointwise on ( 1, 1), but does not converge uniformly on ( 1, 1). 

## 4.2 Real analytic functions

A function $f ( x )$ which is lucky enough to be representable as a power series has a special name; it is a real analytic function. 

Definition 4.2.1 (Real analytic functions). Let E be a subset of R, and let $f : E  \mathbf { R }$ be a function. If a is an interior point of E, we say that f is real analytic at a if there exists an open interval $( a - r , a + r )$ in E for some $r > 0$ such that there exists a power series $\textstyle \sum _ { n = 0 } ^ { \infty } c _ { n } ( x - a ) ^ { n }$ centered at a which has a radius of convergence greater than or equal to r, and which converges to f on $( a - r , a + r )$ . If E is an open set, and f is real analytic at every point a of E, we say that f is real analytic on E. 

Example 4.2.2. Consider the function $f : { \bf R } \backslash \{ 1 \} \  \ { \bf R }$ defined by $f ( x ) : = 1 / ( 1 - x )$ . This function is real analytic at 0 because we have a power series $\scriptstyle \sum _ { n = 0 } ^ { \infty } x ^ { n }$ centred at 0 which converges to $1 / ( 1 - x ) =$ $f ( x )$ on the interval ( 1, 1). This function is also real analytic at 2 because we have a power series $\scriptstyle \sum _ { n = 0 } ^ { \infty } ( - 1 ) ^ { n + 1 } ( x - 2 ) ^ { n }$ which converges to $\textstyle { \frac { - 1 } { 1 - ( - ( x - 2 ) ) } } = { \frac { 1 } { 1 - x } } = f ( x )$ on the interval (1, 3) (why? use Lemma 7.3.3). In fact this function is real analytic on all of $\mathbf { R } \backslash \{ 1 \}$ ; see Exercise 4.2.2. 

Remark 4.2.3. The notion of being real analytic is closely related to another notion, that of being complex analytic, but this is a topic for complex analysis, and will not be discussed here. 

## 4.2. Real analytic functions

We now discuss which functions are real analytic. From Theorem $4 . 1 . 6 ( \mathrm { c } )$ and (d) we see that if f is real analytic at a point $^ { a , }$ then $f$ is both continuous and diferentiable on $( a - r , a + r )$ for some $r > 0$ . We can in fact say more: 

Definition 4.2.4 (k-times diferentiability). Let E be a subset of R. We say a function $f : E  \mathbf { R }$ is once diferentiable on E if it is diferentiable. More generally, for any $k \geq 2$ we say that $f : E  \mathbf { R }$ is k times diferentiable on E, or just k times diferentiable, if f is diferentiable, and $f ^ { \prime }$ is $k - 1$ times diferentiable. If f is k times diferentiable, we define the $k ^ { t h }$ derivative $f ^ { ( k ) } : E  \mathbf { R }$ by the recursive rule $f ^ { ( 1 ) } : = f ^ { \prime }$ 2 and $f ^ { ( k ) } = ( f ^ { ( k - 1 ) } ) ^ { \prime }$ for all $k \geq 2$ . We also define $f ^ { ( 0 ) } : = f$ (this is $f$ diferentiated 0 times), and we allow every function to be zero times diferentiable (since clearly $f ^ { ( 0 ) }$ exists for every $f )$ . A function is said to be infinitely diferentiable (or smooth) if it is k times diferentiable for every $k \geq 0$ 

Example 4.2.5. The function $f ( x ) : = | x | ^ { 3 }$ is twice diferentiable on R, but not three times diferentiable (why?). Indeed, $f ^ { ( 2 ) } = f ^ { \prime \prime } = 6 | x |$ • which is not diferentiable, at 0. 

Proposition 4.2.6 (Real analytic functions are k-times diferentiable). Let E be a subset of R, let a be an interior point of $E$ , and and let f be a function which is real analytic at a, thus there is an $r > 0$ for which we have the power series expansion 

$$
f (x) = \sum_ {n = 0} ^ {\infty} c _ {n} (x - a) ^ {n}
$$

for all $x \in ( a - r , a + r )$ . Then for every $k \geq 0$ , the function f is k-times diferentiable on $( a - r , a + r )$ , and for each $k \geq 0$ the $k ^ { t h }$ derivative is given by 

$$
\begin{array}{c} f ^ {(k)} (x) = \sum_ {n = 0} ^ {\infty} c _ {n + k} (n + 1) (n + 2) \ldots (n + k) (x - a) ^ {n} \\ = \sum_ {n = 0} ^ {\infty} c _ {n + k} \frac {(n + k) !}{n !} (x - a) ^ {n} \end{array}
$$

for all $x \in ( a - r , a + r )$ 

Proof. See Exercise 4.2.3. 

Corollary 4.2.7 (Real analytic functions are infinitely diferentiable). Let E be an open subset of R, and let $f : E  \mathbf { R }$ be a real analytic function on E. Then f is infinitely diferentiable on E. Also, all derivatives of f are also real analytic on E. 

Proof. For every point $a \in E$ and $k \geq 0$ , we know from Proposition 4.2.6 that f is k-times diferentiable at a (we will have to apply Exercise 10.1.1 k times here, why?). Thus f is k-times diferentiable on E for every $k \geq 0$ and is hence infinitely diferentiable. Also, from Proposition 4.2.6 we see that each derivative $f ^ { ( k ) }$ of $f$ has a convergent power series expansion at every $x \in E$ and thus $f ^ { ( k ) }$ is real analytic. □ 

Example 4.2.8. Consider the function $f : \mathbf { R }  \mathbf { R }$ defined by $f ( x ) : =$ $| x |$ . This function is not diferentiable at $x = 0$ , and hence cannot be real analytic at $x = 0$ . It is however real analytic at every other point $x \in { \bf R } \backslash \{ 0 \} \ ( \mathrm { w h y ? } )$ 

Remark 4.2.9. The converse statement to Corollary 4.2.7 is not true; there are infinitely diferentiable functions which are not real analytic. See Exercise 4.5.4. 

Proposition 4.2.6 has an important corollary, due to Brook Taylor (1685–1731). 

Corollary 4.2.10 (Taylor’s formula). Let E be a subset of R, let a be an interior point of E, and let $f : E  \mathbf { R }$ be a function which is real analytic at a and has the power series expansion 

$$
f (x) = \sum_ {n = 0} ^ {\infty} c _ {n} (x - a) ^ {n}
$$

for all $x \in ( a - r , a + r )$ and some $r > 0$ . Then for any integer $k \geq 0$ we have 

$$
f ^ {(k)} (a) = k! c _ {k},
$$

where k! $\mathrel { \mathop : } = 1 \times 2 \times \ldots \times k$ (and we adopt the convention that $0 ! = 1 )$ In particular, we have Taylor’s formula 

$$
f (x) = \sum_ {n = 0} ^ {\infty} \frac {f ^ {(n)} (a)}{n !} (x - a) ^ {n}
$$

for all x in $( a - r , a + r )$ 

## 4.2. Real analytic functions

Proof. See Exercise 4.2.4. 

The power series $\scriptstyle \sum _ { n = 0 } ^ { \infty } { \frac { f ^ { ( n ) } ( a ) } { n ! } } ( x - a ) ^ { n }$ is sometimes called the Taylor series of f around a. Taylor’s formula thus asserts that if a function is real analytic, then it is equal to its Taylor series. 

Remark 4.2.11. Note that Taylor’s formula only works for functions which are real analytic; there are examples of functions which are infinitely diferentiable but for which Taylor’s theorem fails (see Exercise 4.5.4). 

Another important corollary of Taylor’s formula is that a real analytic function can have at most one power series at a point: 

Corollary 4.2.12 (Uniqueness of power series). Let E be a subset of R, let a be an interior point of E, and let $f : E  \mathbf { R }$ be a function which is real analytic at a. Suppose that f has two power series expansions 

$$
f (x) = \sum_ {n = 0} ^ {\infty} c _ {n} (x - a) ^ {n}
$$

and 

$$
f (x) = \sum_ {n = 0} ^ {\infty} d _ {n} (x - a) ^ {n}
$$

centered at a, ecah with a non-zero radius of convergence. Then $c _ { n } = d _ { n }$ for all $n \geq 0$ 

Proof. By Corollary 4.2.10, we have $f ^ { ( k ) } ( a ) = k ! c _ { k }$ for all $k \geq 0$ . But we also have $f ^ { ( k ) } ( a ) = k ! d _ { k }$ , by similar reasoning. Since k! is never zero, we can cancel it and obtain $c _ { k } = d _ { k }$ for all $k \geq 0$ , as desired. □ 

Remark 4.2.13. While a real analytic function has a unique power series around any given point, it can certainly have diferent power series at diferent points. For instance, the function $\textstyle f ( x ) : = { \frac { 1 } { 1 - x } }$ , defined on $\mathbf { R } - \{ 1 \}$ , has the power series 

$$
f (x) := \sum_ {n = 0} ^ {\infty} x ^ {n}
$$

around 0, on the interval ( 1, 1), but also has the power series 

$$
\begin{array}{r c l} f (x) & = & \frac {1}{1 - x} = \frac {2}{1 - 2 (x - \frac {1}{2})} \\ & & = \sum_ {n = 0} ^ {\infty} 2 \left(2 \left(x - \frac {1}{2}\right)\right) ^ {n} = \sum_ {n = 0} ^ {\infty} 2 ^ {n + 1} \left(x - \frac {1}{2}\right) ^ {n} \end{array}
$$

around $1 / 2  \it$ , on the interval (0, 1) (note that the above power series has a radius of convergence of $1 / 2$ , thanks to the root test. See also Exercise 4.2.8. 

## — Exercises —

Exercise 4.2.1. Let $n \geq 0$ be an integer, let $c , a$ be real numbers, and let f be the function $f ( x ) : = c ( x - a ) ^ { n }$ . Show that f is infinitely diferentiable, and that $f ^ { ( k ) } ( x ) = c { \frac { n ! } { ( n - k ) ! } } ( x - a ) ^ { n - k }$ for all integers $0 \leq k \leq n$ . What happens when $k > n ?$ 

Exercise 4.2.2. Show that the function f defined in Example 4.2.2 is real analytic on all of $\mathbf { R } \backslash \{ 1 \}$ 

Exercise 4.2.3. Prove Proposition 4.2.6. (Hint: induct on k and use Theorem $4 . 1 . 6 ( \mathrm { d } ) )$ 

Exercise 4.2.4. Use Proposition 4.2.6 and Exercise 4.2.1 to prove Corollary 4.2.10. 

Exercise 4.2.5. Let $a , b$ be real numbers, and let $n \geq 0$ be an integer. Prove the identity 

$$
(x - a) ^ {n} = \sum_ {m = 0} ^ {n} \frac {n !}{m ! (n - m) !} (b - a) ^ {n - m} (x - b) ^ {m}
$$

for any real number x. (Hint: use the binomial formula, Exercise 7.1.4.) Explain why this identity is consistent with Taylor’s theorem and Exercise 4.2.1. (Note however that Taylor’s theorem cannot be rigorously applied until one verifies Exercise 4.2.6 below.) 

Exercise 4.2.6. Using Exercise 4.2.5, show that every polynomial $P ( x )$ of one variable is real analytic on R. 

Exercise 4.2.7. Let $m \geq 0$ be a positive integer, and let $0 < x < r$ be real numbers. Use Lemma 7.3.3 to establish the identity 

$$
{\frac {r}{r - x}} = \sum_ {n = 0} ^ {\infty} x ^ {n} r ^ {- n}
$$

for all $x \in ( - r , r )$ . Using Proposition 4.2.6, conclude the identity 

$$
{\frac {r}{(r - x) ^ {m + 1}}} = \sum_ {n = m} ^ {\infty} {\frac {n !}{m ! (n - m) !}} x ^ {n - m} r ^ {- n}
$$

for all integers $m \geq 0$ and $x \in ( - r , r )$ . Also explain why the series on the right-hand side is absolutely convergent. 

Exercise 4.2.8. Let E be a subset of R, let a be an interior point of $E ,$ and let $f : E  \mathbf { R }$ be a function which is real analytic in $a ,$ and has a power series expansion 

$$
f (x) = \sum_ {n = 0} ^ {\infty} c _ {n} (x - a) ^ {n}
$$

at a which converges on the interval $( a - r , a + r )$ . Let $( b - s , b + s )$ be any sub-interval of $( a - r , a + r )$ for some $s > 0$ 

(a) Prove that $| a - b | \leq r - s$ , so in particular $| a - b | < r$ 

(b) Show that for every $0 < \varepsilon < r .$ , there exists a $C > 0$ such that $\left. c _ { n } \right. \leq$ $C ( r - \varepsilon ) ^ { - n }$ for all integers $n \geq 0$ . (Hint: what do we know about the radius of convergence of the series $\textstyle \sum _ { n = 0 } ^ { \infty } c _ { n } ( x - a ) ^ { n } ? )$ 

(c) Show that the numbers $d _ { 0 } , d _ { 1 } , \ldots$ given by the formula 

$$
d _ {m} := \sum_ {n = m} ^ {\infty} \frac {n !}{m ! (n - m) !} (b - a) ^ {n - m} c _ {n} \text { for all integers } m \geq 0
$$

are well-defined, in the sense that the above series is absolutely convergent. (Hint: use (b) and the comparison test, Corollary 7.3.2, followed by Exercise 4.2.7.) 

(d) Show that for every $0 < \varepsilon < s$ there exists a $C > 0$ such that 

$$
| d _ {m} | \leq C (s - \varepsilon) ^ {- m}
$$

for all integers $m \geq 0$ . (Hint: use the comparison test, and Exercise 4.2.7.) 

(e) Show that the power series $\textstyle \sum _ { m = 0 } ^ { \infty } d _ { m } ( x - b ) ^ { m }$ is absolutely convergent for $x \in ( b - s , b + s )$ and converges to $f ( x )$ . (You may need Fubini’s theorem for infinite series, Theorem 8.2.2, as well as Exercise 4.2.5). 

(f) Conclude that f is real analytic at every point in $( a - r , a + r )$ 

## 4.3 Abel’s theorem

Let $\begin{array} { r } { f ( x ) = \sum _ { n = 0 } ^ { \infty } c _ { n } ( x - a ) ^ { n } } \end{array}$ be a power series centered at $a$ with a radius of convergence $0 < R < \infty$ strictly between 0 and infinity. From Theorem 4.1.6 we know that the power series converges absolutely whenever $| x - a | < R$ , and diverges when $| x - a | > R$ . However, at the boundary $| x - a | = R$ the situation is more complicated; the series may either converge or diverge (see Exercise 4.1.2). However, if the series does converge at the boundary point, then it is reasonably well behaved; in particular, it is continuous at that boundary point. 

Theorem 4.3.1 (Abel’s theorem). Let $\begin{array} { r } { f ( x ) = \sum _ { n = 0 } ^ { \infty } c _ { n } ( x - a ) ^ { n } } \end{array}$ be a power series centered at a with radius of convergence $0 < R < \infty$ . If the power series converges at $a + R _ { i }$ , then f is continuous at $a + R ,$ i.e. 

$$
\lim _ {x \to a + R: x \in (a - R, a + R)} \sum_ {n = 0} ^ {\infty} c _ {n} (x - a) ^ {n} = \sum_ {n = 0} ^ {\infty} c _ {n} R ^ {n}.
$$

Similarly, if the power series converges at $a - R$ , then f is continuous at $a - R$ , i.e. 

$$
\lim _ {x \to a - R: x \in (a - R, a + R)} \sum_ {n = 0} ^ {\infty} c _ {n} (x - a) ^ {n} = \sum_ {n = 0} ^ {\infty} c _ {n} (- R) ^ {n}.
$$

Before we prove Abel’s theorem, we need the following lemma. 

Lemma 4.3.2 (Summation by parts formula). Let $( a _ { n } ) _ { n = 0 } ^ { \infty }$ and $( b _ { n } ) _ { n = 0 } ^ { \infty }$ be sequences of real numbers which converge to limits A and B respectively, i.e., li $\operatorname { n } _ { n \to \infty } a _ { n } = A$ and $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } b _ { n } = B } \end{array}$ . Suppose that the sum $\textstyle \sum _ { n = 0 } ^ { \infty } ( a _ { n + 1 } - a _ { n } ) b _ { n }$ is convergent. Then the sum $\begin{array} { r } { \sum _ { n = 0 } ^ { \infty } a _ { n + 1 } ( b _ { n + 1 } - b _ { n } ) } \end{array}$ is also convergent, and 

$$
\sum_ {n = 0} ^ {\infty} (a _ {n + 1} - a _ {n}) b _ {n} = A B - a _ {0} b _ {0} - \sum_ {n = 0} ^ {\infty} a _ {n + 1} (b _ {n + 1} - b _ {n}).
$$

Proof. See Exercise 4.3.1. 

Remark 4.3.3. One should compare this formula with the more wellknown integration by parts formula 

$$
\int_ {0} ^ {\infty} f ^ {\prime} (x) g (x) d x = f (x) g (x) | _ {0} ^ {\infty} - \int_ {0} ^ {\infty} f (x) g ^ {\prime} (x) d x,
$$

see Proposition 11.10.1. 

Proof of Abel’s theorem. It will sufice to prove the first claim, i.e., that 

$$
\lim _ {x \to a + R: x \in (a - R, a + R)} \sum_ {n = 0} ^ {\infty} c _ {n} (x - a) ^ {n} = \sum_ {n = 0} ^ {\infty} c _ {n} R ^ {n}
$$

whenever the sum $\scriptstyle \sum _ { n = 0 } ^ { \infty } c _ { n } R ^ { n }$ converges; the second claim will then follow $\mathrm { ( w h y ? ) }$ by replacing $c _ { n }$ by $( - 1 ) ^ { n } c _ { n }$ in the above claim. If we 

## 4.3. Abel’s theorem

make the substitutions $d _ { n } : = c _ { n } R ^ { n }$ and $\textstyle y : = { \frac { x - a } { R } } $ , then the above claim can be rewritten as 

$$
\lim _ {y \to 1: y \in (- 1, 1)} \sum_ {n = 0} ^ {\infty} d _ {n} y ^ {n} = \sum_ {n = 0} ^ {\infty} d _ {n}
$$

whenever the sum $\textstyle \sum _ { n = 0 } ^ { \infty } d _ { n }$ converges. (Why is this equivalent to the previous claim?) 

Write $D : = \textstyle \sum _ { n = 0 } ^ { \infty } d _ { n }$ , and for every $N \geq 0$ write 

$$
S _ {N} := \left(\sum_ {n = 0} ^ {N - 1} d _ {n}\right) - D
$$

so in particular $S _ { 0 } = - D$ . Then observe that lim ${ \bf \Gamma } _ { N  \infty } S _ { N } = 0$ , and that $d _ { n } = S _ { n + 1 } - S _ { n }$ . Thus for any $y \in ( - 1 , 1 )$ we have 

$$
\sum_ {n = 0} ^ {\infty} d _ {n} y ^ {n} = \sum_ {n = 0} ^ {\infty} (S _ {n + 1} - S _ {n}) y ^ {n}.
$$

Applying the summation by parts formula (Lemma 4.3.2), and noting that $\scriptstyle \operatorname* { l i m } _ { n \to \infty } y ^ { n } = 0$ , we obtain 

$$
\sum_ {n = 0} ^ {\infty} d _ {n} y ^ {n} = - S _ {0} y ^ {0} - \sum_ {n = 0} ^ {\infty} S _ {n + 1} (y ^ {n + 1} - y ^ {n}).
$$

Observe that $- S _ { 0 } y ^ { 0 } = + D$ . Thus to finish the proof of Abel’s theorem, it will sufice to show that 

$$
\lim _ {y \to 1: y \in (- 1, 1)} \sum_ {n = 0} ^ {\infty} S _ {n + 1} (y ^ {n + 1} - y ^ {n}) = 0.
$$

Since y converges to 1, we may as well restrict $y$ to [0, 1) instead of ( 1, 1); in particular we may take y to be positive. 

From the triangle inequality for series (Proposition 7.2.9), we have 

$$
\begin{array}{c} \left| \sum_ {n = 0} ^ {\infty} S _ {n + 1} (y ^ {n + 1} - y ^ {n}) \right| \leq \sum_ {n = 0} ^ {\infty} | S _ {n + 1} (y ^ {n + 1} - y ^ {n}) | \\ = \sum_ {n = 0} ^ {\infty} | S _ {n + 1} | (y ^ {n} - y ^ {n + 1}), \end{array}
$$

so by the squeeze test (Corollary 6.4.14) it sufices to show that 

$$
\lim _ {y \to 1: y \in [ 0, 1)} \sum_ {n = 0} ^ {\infty} | S _ {n + 1} | (y ^ {n} - y ^ {n + 1}) = 0.
$$

The expression $\scriptstyle \sum _ { n = 0 } ^ { \infty } | S _ { n + 1 } | ( y ^ { n } - y ^ { n + 1 } )$ is clearly non-negative, so it wil sufice to show that 

$$
\limsup _ {y \to 1: y \in [ 0, 1)} \sum_ {n = 0} ^ {\infty} | S _ {n + 1} | (y ^ {n} - y ^ {n + 1}) = 0.
$$

Let $\varepsilon > 0$ . Since $S _ { n }$ converges to 0, there exists an N such that $| S _ { n } | \le \varepsilon$ for all $n > N$ . Thus we have 

$$
\sum_ {n = 0} ^ {\infty} | S _ {n + 1} | (y ^ {n} - y ^ {n + 1}) \leq \sum_ {n = 0} ^ {N} | S _ {n + 1} | (y ^ {n} - y ^ {n + 1}) + \sum_ {n = N + 1} ^ {\infty} \varepsilon (y ^ {n} - y ^ {n + 1}).
$$

The last summation is a telescoping series, which sums to $\varepsilon y ^ { N + 1 }$ (See Lemma 7.2.15, recalling from Lemma 6.5.2 that $y ^ { n } \to 0 \operatorname { a s } n \to \infty )$ , and thus 

$$
\sum_ {n = 0} ^ {\infty} | S _ {n + 1} | (y ^ {n} - y ^ {n + 1}) \leq \sum_ {n = 0} ^ {N} | S _ {n + 1} | (y ^ {n} - y ^ {n + 1}) + \varepsilon y ^ {N + 1}.
$$

Now take limits as $y  1$ . Observe that $y ^ { n } - y ^ { n + 1 } \to 0$ as $y  1$ for every $n \in { 0 , 1 , \ldots , N }$ . Since we can interchange limits and finite sums (Exercise 7.1.5), we thus have 

$$
\limsup _ {n \to \infty} \sum_ {n = 0} ^ {\infty} | S _ {n + 1} | (y ^ {n} - y ^ {n + 1}) \leq \varepsilon .
$$

But $\varepsilon > 0$ was arbitrary, and thus we must have 

$$
\limsup _ {n \to \infty} \sum_ {n = 0} ^ {\infty} | S _ {n + 1} | (y ^ {n} - y ^ {n + 1}) = 0
$$

since the left-hand side must be non-negative. The claim follows. 

$$
- \text { Exercises } -
$$

Exercise 4.3.1. Prove Lemma 4.3.2. (Hint: first work out the relationship between the partial sums $\textstyle \sum _ { n = 0 } ^ { N } ( a _ { n + 1 } - a _ { n } ) b _ { n }$ and $\begin{array} { r } { \sum _ { n = 0 } ^ { N } a _ { n + 1 } ( b _ { n + 1 } - b _ { n } ) . ) } \end{array}$ 

## 4.4 Multiplication of power series

We now show that the product of two real analytic functions is again real analytic. 

Theorem 4.4.1. Let $f : ( a - r , a + r )  \mathbf { R }$ and $g : ( a - r , a + r )  \mathbf { R }$ be functions analytic on $( a - r , a + r )$ , with power series expansions 

$$
f (x) = \sum_ {n = 0} ^ {\infty} c _ {n} (x - a) ^ {n}
$$

and 

$$
g (x) = \sum_ {n = 0} ^ {\infty} d _ {n} (x - a) ^ {n}
$$

respectively. Then $f g : ( a - r , a + r ) \to \mathbf { R }$ is also analytic on $( a - r , a + r )$ with power series expansion 

$$
f (x) g (x) = \sum_ {n = 0} ^ {\infty} e _ {n} (x - a) ^ {n}
$$

where $\begin{array} { r } { e _ { n } : = \sum _ { m = 0 } ^ { n } c _ { m } d _ { n - m } } \end{array}$ 

Remark 4.4.2. The sequence $( e _ { n } ) _ { n = 0 } ^ { \infty }$ is sometimes referred to as the convolution of the sequences $( c _ { n } ) _ { n = 0 } ^ { \infty }$ and $( d _ { n } ) _ { n = 0 } ^ { \infty } ;$ ; it is closely related (though not identical) to the notion of convolution introduced in Definition 3.8.9. 

Proof. We have to show that the series $\textstyle \sum _ { n = 0 } ^ { \infty } e _ { n } ( x - a ) ^ { n }$ converges to $f ( x ) g ( x )$ for all $x \in \left( a { - } r , a { + } r \right)$ . Now fix x to be any point in $( a - r , a + r )$ By Theorem 4.1.6, we see that both f and g have radii of convergence at least r. In particular, the series $\textstyle \sum _ { n = 0 } ^ { \infty } c _ { n } ( x - a ) ^ { n }$ and $\textstyle \sum _ { n = 0 } ^ { \infty } d _ { n } ( x - a ) ^ { n }$ are absolutely convergent. Thus if we define 

$$
C := \sum_ {n = 0} ^ {\infty} | c _ {n} (x - a) ^ {n} |
$$

and 

$$
D := \sum_ {n = 0} ^ {\infty} | d _ {n} (x - a) ^ {n} |
$$

then C and D are both finite. 

For any $N \geq 0$ , consider the partial sum 

$$
\sum_ {n = 0} ^ {N} \sum_ {m = 0} ^ {\infty} | c _ {m} (x - a) ^ {m} d _ {n} (x - a) ^ {n} |.
$$

We can rewrite this as 

$$
\sum_ {n = 0} ^ {N} | d _ {n} (x - a) ^ {n} | \sum_ {m = 0} ^ {\infty} | c _ {m} (x - a) ^ {m} |,
$$

which by definition of C is equal to 

$$
\sum_ {n = 0} ^ {N} | d _ {n} (x - a) ^ {n} | C,
$$

which by definition of D is less than or equal to DC. Thus the above partial sums are bounded by DC for every N. In particular, the series 

$$
\sum_ {n = 0} ^ {\infty} \sum_ {m = 0} ^ {\infty} | c _ {m} (x - a) ^ {m} d _ {n} (x - a) ^ {n} |
$$

is convergent, which means that the sum 

$$
\sum_ {n = 0} ^ {\infty} \sum_ {m = 0} ^ {\infty} c _ {m} (x - a) ^ {m} d _ {n} (x - a) ^ {n}
$$

is absolutely convergent. 

Let us now compute this sum in two ways. First of all, we can pull the $d _ { n } ( x - a ) ^ { n }$ factor out of the $\textstyle \sum _ { m = 0 } ^ { \infty }$ summation, to obtain 

$$
\sum_ {n = 0} ^ {\infty} d _ {n} (x - a) ^ {n} \sum_ {m = 0} ^ {\infty} c _ {m} (x - a) ^ {m}.
$$

By our formula for $f ( x )$ , this is equal to 

$$
\sum_ {n = 0} ^ {\infty} d _ {n} (x - a) ^ {n} f (x);
$$

by our formula for $g ( x )$ , this is equal to $f ( x ) g ( x )$ . Thus 

$$
f (x) g (x) = \sum_ {n = 0} ^ {\infty} \sum_ {m = 0} ^ {\infty} c _ {m} (x - a) ^ {m} d _ {n} (x - a) ^ {n}.
$$

## 4.4. Multiplication of power series

Now we compute this sum in a diferent way. We rewrite it as 

$$
f (x) g (x) = \sum_ {n = 0} ^ {\infty} \sum_ {m = 0} ^ {\infty} c _ {m} d _ {n} (x - a) ^ {n + m}.
$$

By Fubini’s theorem for series (Theorem 8.2.2), because the series was absolutely convergent, we may rewrite it as 

$$
f (x) g (x) = \sum_ {m = 0} ^ {\infty} \sum_ {n = 0} ^ {\infty} c _ {m} d _ {n} (x - a) ^ {n + m}.
$$

Now make the substitution $n ^ { \prime } : = n + m$ , to rewrite this as 

$$
f (x) g (x) = \sum_ {m = 0} ^ {\infty} \sum_ {n ^ {\prime} = m} ^ {\infty} c _ {m} d _ {n ^ {\prime} - m} (x - a) ^ {n ^ {\prime}}.
$$

If we adopt the convention that $d _ { j } = 0$ for all negative $j ,$ , then this is equal to 

$$
f (x) g (x) = \sum_ {m = 0} ^ {\infty} \sum_ {n ^ {\prime} = 0} ^ {\infty} c _ {m} d _ {n ^ {\prime} - m} (x - a) ^ {n ^ {\prime}}.
$$

Applying Fubini’s theorem again, we obtain 

$$
f (x) g (x) = \sum_ {n ^ {\prime} = 0} ^ {\infty} \sum_ {m = 0} ^ {\infty} c _ {m} d _ {n ^ {\prime} - m} (x - a) ^ {n ^ {\prime}},
$$

which we can rewrite as 

$$
f (x) g (x) = \sum_ {n ^ {\prime} = 0} ^ {\infty} (x - a) ^ {n ^ {\prime}} \sum_ {m = 0} ^ {\infty} c _ {m} d _ {n ^ {\prime} - m}.
$$

Since $d _ { j }$ was 0 when j is negative, we can rewrite this as 

$$
f (x) g (x) = \sum_ {n ^ {\prime} = 0} ^ {\infty} (x - a) ^ {n ^ {\prime}} \sum_ {m = 0} ^ {n ^ {\prime}} c _ {m} d _ {n ^ {\prime} - m},
$$

which by definition of $e$ is 

$$
f (x) g (x) = \sum_ {n ^ {\prime} = 0} ^ {\infty} e _ {n ^ {\prime}} (x - a) ^ {n ^ {\prime}},
$$

as desired. 

## 4.5 The exponential and logarithm functions

We can now use the machinery developed in the last few sections to develop a rigorous foundation for many standard functions used in mathematics. We begin with the exponential function. 

Definition 4.5.1 (Exponential function). For every real number x, we define the exponential function $\exp ( x )$ to be the real number 

$$
\exp (x) := \sum_ {n = 0} ^ {\infty} \frac {x ^ {n}}{n !}.
$$

Theorem 4.5.2 (Basic properties of exponential). 

(a) For every real number x, the series $\textstyle \sum _ { n = 0 } ^ { \infty } { \frac { x ^ { n } } { n ! } }$ is absolutely convergent. In particular, exp(x) exists and is real for every $x \in \mathbf { R }$ , the power series $\textstyle \sum _ { n = 0 } ^ { \infty } { \frac { x ^ { n } } { n ! } }$ has an infinite radius of convergence, and exp is a real analytic function on $( - \infty , \infty )$ 

(b) exp is diferentiable on R, and for every $x \in \mathbf { R } , \exp ^ { \prime } ( x ) = \exp ( x )$ 

(c) exp is continuous on R, and for every interval $[ a , b ]$ , we have $\begin{array} { r } { \int _ { [ a , b ] } \exp ( x ) \ d x = \exp ( b ) - \exp ( a ) } \end{array}$ 

(d) For every x, $y \in \mathbf { R }$ , we have exp $( x + y ) = \exp ( x ) \exp ( y )$ 

(e) We have exp $( 0 ) = 1$ . Also, for every $x \in \mathbf { R } , \exp ( x )$ is positive, and $\exp ( - x ) = 1 / \exp ( x )$ 

(f) exp is strictly monotone increasing: in other words, if x, y are real numbers, then we have ex $\mathrm { p } ( y ) > \exp ( x )$ if and only if $y > x$ 

Proof. See Exercise 4.5.1. 

One can write the exponential function in a more compact form, introducing famous Euler’s number $e = 2 . 7 1 8 2 8 1 8 3 \dots$ also known as the base of the natural logarithm: 

Definition 4.5.3 (Euler’s number). The number e is defined to be 

$$
e := \exp (1) = \sum_ {n = 0} ^ {\infty} \frac {1}{n !} = \frac {1}{0 !} + \frac {1}{1 !} + \frac {1}{2 !} + \frac {1}{3 !} + \dots .
$$

Proposition 4.5.4. For every real number x, we have $\exp ( x ) = e ^ { x }$ 

Proof. See Exercise 4.5.3. 

In light of this proposition we can and will use $e ^ { x }$ and $\exp ( x )$ interchangeably. 

Since $e > 1 \ \mathrm { ( w h y ? ) }$ , we see that $e ^ { x } \to + \infty { \mathrm { ~ a s ~ } } x \to + \infty$ , and $e ^ { x } \to 0$ as $x \to - \infty$ . From this and the intermediate value theorem (Theorem 9.7.1) we see that the range of the function exp is $( 0 , \infty )$ . Since exp is increasing, it is injective, and hence exp is a bijection from R to $( 0 , \infty )$ 1 and thus has an inverse from $( 0 , \infty ) \to \mathbf { R }$ . This inverse has a name: 

Definition 4.5.5 (Logarithm). We define the natural logarithm function log ${ \bf \colon } ( 0 , \infty )  { \bf R }$ (also called ln) to be the inverse of the exponential function. Thus $\exp ( \log ( x ) ) = x { \mathrm { ~ a n d ~ } } \log ( \exp ( x ) ) = x .$ 

Since exp is continuous and strictly monotone increasing, we see that log is also continuous and strictly monotone increasing (see Proposition 9.8.3). Since exp is also diferentiable, and the derivative is never zero, we see from the inverse function theorem (Theorem 10.4.2) that log is also diferentiable. We list some other properties of the natural logarithm below. 

Theorem 4.5.6 (Logarithm properties). 

(a) For every $x \in ( 0 , \infty )$ , we have $\begin{array} { r } { \ln ^ { \prime } ( x ) = \frac { 1 } { x } . } \end{array}$ . In particular, by the fundamental theorem of calculus, we have ${ \\begin{array} { r } { \int _ { [ a , b ] } { \frac { 1 } { x } } \ d x = \ln ( b ) - \ln ( a ) } \end{array} }$ for any interval [a, b] in $( 0 , \infty )$ 

(b) We have $\ln ( x y ) = \ln ( x ) + \ln ( y )$ for all x, $y \in ( 0 , \infty )$ 

(c) We have ln(1) = 0 and ln $( 1 / x ) = - \ln ( x )$ for all $x \in ( 0 , \infty )$ 

(d) For any $x \in ( 0 , \infty )$ and $y \in \mathbf { R }$ , we have $\ln ( x ^ { y } ) = y \ln ( x )$ 

(e) For any $x \in ( - 1 , 1 )$ , we have 

$$
\ln (1 - x) = - \sum_ {n = 1} ^ {\infty} \frac {x ^ {n}}{n}.
$$

In particular, ln is analytic at 1, with the power series expansion 

$$
\ln (x) = \sum_ {n = 1} ^ {\infty} \frac {(- 1) ^ {n + 1}}{n} (x - 1) ^ {n}
$$

for $x \in ( 0 , 2 )$ , with radius of convergence 1. 

Proof. See Exercise 4.5.5. 

□ 

Example 4.5.7. We now give a modest application of Abel’s theorem (Theorem 4.3.1): from the alternating series test we see that $\scriptstyle \sum _ { n = 1 } ^ { \infty } { \frac { ( - 1 ) ^ { n + 1 } } { n } }$ is convergent. By Abel’s theorem we thus see that 

$$
\begin{array}{c} \sum_ {n = 1} ^ {\infty} \frac {(- 1) ^ {n + 1}}{n} = \lim _ {x \to 2} \sum_ {n = 1} ^ {\infty} \frac {(- 1) ^ {n + 1}}{n} (x - 1) ^ {n} \\ = \lim _ {x \to 2} \ln (x) = \ln (2), \end{array}
$$

thus we have the formula 

$$
\begin{array}{c} \ln (2) = 1 - \frac {1}{2} + \frac {1}{3} - \frac {1}{4} + \frac {1}{5} - \dots . \\ \text {- Exercises - } \end{array}
$$

Exercise 4.5.1. Prove Theorem 4.5.2. (Hints: for part (a), use the ratio test. For parts (bc), use Theorem 4.1.6. For part (d), use Theorem 4.4.1. For part (e), use part (d). For part (f), use part (d), and prove that $\exp ( x ) > 1$ when x is positive. You may find the binomial formula from Exercise 7.1.4 to be useful. 

Exercise 4.5.2. Show that for every integer $n \geq 3$ , we have 

$$
0 <   \frac {1}{(n + 1) !} + \frac {1}{(n + 2) !} + \dots <   \frac {1}{n !}.
$$

(Hint: first show that $( n + k ) ! > 2 ^ { k } n !$ for all $k = 1 , 2 , 3 , \ldots )$ Conclude that n!e is not an integer for every $n \geq 3$ . Deduce from this that e is irrational. (Hint: prove by contradiction.) 

Exercise 4.5.3. Prove Proposition 4.5.4. (Hint: first prove the claim when x is a natural number. Then prove it when x is an integer. Then prove it when x is a rational number. Then use the fact that real numbers are the limits of rational numbers to prove it for all real numbers. You may find the exponent laws (Proposition 6.7.3) to be useful.) 

Exercise 4.5.4. Let $f : \mathbf { R }  \mathbf { R }$ be the function defined by setting $f ( x ) : =$ $\exp ( - 1 / x )$ when $x > 0$ , and $f ( x ) : = 0$ when $x \leq 0$ . Prove that f is infinitely diferentiable, and $f ^ { ( k ) } ( 0 ) = 0$ for every integer $k \geq 0$ , but that f is not rea analytic at 0. 

Exercise 4.5.5. Prove Theorem 4.5.6. (Hints: for part (a), use the inverse function theorem (Theorem 10.4.2) or the chain rule (Theorem 10.1.15). For parts (bcd), use Theorem 4.5.2 and the exponent laws (Proposition 6.7.3). For part (e), start with the geometric series formula (Lemma 7.3.3) and integrate using Theorem 4.1.6). 

Exercise 4.5.6. Prove that the natural logarithm function is real analytic on $( 0 , + \infty )$ 

Exercise 4.5.7. Let $f : \mathbf { R }  ( 0 , \infty )$ be a positive, real analytic function such that $f ^ { \prime } ( x ) = f ( x )$ for all $x \in \mathbf { R }$ . Show that $f ( x ) = C e ^ { x }$ for some positive constant $C ;$ justify your reasoning. (Hint: there are basically three diferent proofs available. One proof uses the logarithm function, another proof uses the function $e ^ { - x }$ , and a third proof uses power series. Of course, you only need to supply one proof.) 

Exercise 4.5.8. Let $m > 0$ be an integer. Show that 

$$
\lim _ {x \to + \infty} \frac {e ^ {x}}{x ^ {m}} = + \infty .
$$

(Hint: what happens to the ratio between $e ^ { x + 1 } / ( x + 1 ) ^ { m }$ and $e ^ { x } / x ^ { m }$ as $x $ $+ \infty ? )$ 

Exercise 4.5.9. Let $P ( x )$ be a polynomial, and let $c > 0 .$ . Show that there exists a real number $N > 0$ such that $e ^ { c x } > | P ( x ) |$ for all $x > N$ ; thus an exponentially growing function, no matter how small the growth rate $c ,$ will eventually overtake any given polynomial $P ( x )$ , no matter how large. (Hint: use Exercise 4.5.8.) 

Exercise 4.5.10. Let $f \ : \ ( 0 , + \infty ) \times \mathbf { R } \  \ \mathbf { R }$ be the exponential function $f ( x , y ) : = x ^ { y }$ . Show that $f$ is continuous. (Hint: note that Propositions 9.4.10, 9.4.11 only show that f is continuous in each variable, which is insuficient, as Exercise 2.2.11 shows. The easiest way to proceed is to write $f ( x , y ) = \exp ( y \ln x )$ and use the continuity of $\exp ( )$ and $\ln ( )$ . For an extra challenge, try proving this exercise without using the logarithm function.) 

## 4.6 A digression on complex numbers

To proceed further we need the complex number system C, which is an extension of the real number system R. A full discussion of this important number system (and in particular the branch of mathematics known as complex analysis) is beyond the scope of this text; here, we need the system primarily because of a very useful mathematical operation, the complex exponential function $z \mapsto \exp ( z )$ , which generalizes the real exponential function $x \mapsto \exp ( x )$ introduced in the previous section. 

Informally, we could define the complex numbers as 

Definition 4.6.1 (Informal definition of complex numbers). The complex numbers C are the set of all numbers of the form $a + b i$ , where $a , b$ are real numbers and i is a square root of $- 1 , i ^ { 2 } = - 1$ 

However, this definition is a little unsatisfactory as it does not explain how to add, multiply, or compare two complex numbers. To construct the complex numbers rigorously we will first introduce a formal version of the complex number $a + b i$ , which we shall temporarily denote as $( a , b )$ this is similar to how in Chapter 4, when constructing the integers $\mathbf { Z } _ { \mathrm { i } }$ we needed a formal notion of subtraction $a { - } b$ before the actual notion of subtraction $a - b$ could be introduced, or how when constructing the rational numbers, a formal notion of division $a / / b$ was needed before it was superceded by the actual notion $a / b$ of division. It is also similar to how, in the construction of the real numbers, we defined a formal limit $\mathrm { L I M } _ { n \to \infty } a _ { n }$ before we defined a genuine limit $\operatorname* { l i m } _ { n \to \infty } a _ { n }$ 

Definition 4.6.2 (Formal definition of complex numbers). A complex number is any pair of the form $( a , b )$ , where a, b are real numbers, thus for instance $( 2 , 4 )$ is a complex number. Two complex numbers $( a , b ) , ( c , d )$ are said to be equal if $a = c$ and $b = d .$ , thus for instance $( 2 + 1 , 3 + 4 ) =$ $( 3 , 7 )$ , but $( 2 , 1 ) \neq ( 1 , 2 )$ and $( 2 , 4 ) \neq ( 2 , - 4 )$ . The set of all complex numbers is denoted C. 

At this stage the complex numbers C are indistinguishable from the Cartesian product $\mathbf { R } ^ { 2 } = \mathbf { R } \times \mathbf { R }$ (also known as the Cartesian plane). However, we will introduce a number of operations on the complex numbers, notably that of complex multiplication, which are not normally placed on the Cartesian plane $\mathbf { R } ^ { 2 }$ . Thus one can think of the complex number system C as the Cartesian plane $\mathbf { R } ^ { 2 }$ equipped with a number of additional structures. We begin with the notion of addition and negation. Using the informal definition of the complex numbers, we expect 

$$
(a, b) + (c, d) = (a + b i) + (c + d i) = (a + c) + (b + d) i = (a + c, b + d)
$$

and similarly 

$$
- (a, b) = - (a + b i) = (- a) + (- b) i = (- a, - b).
$$

As these derivations used the informal definition of the complex numbers, these identities have not yet been rigorously proven. However we shall simply encode these identities into our complex number system by defining the notion of addition and negation by the above rules: 

Definition 4.6.3 (Complex addition, negation, and zero). $\mathrm { I f } ~ z = ( a , b )$ and $w = ( c , d )$ are two complex numbers, we define their sum $z + w$ to be the complex number $z + w : = ( a + c , b + d )$ . Thus for instance $( 2 , 4 ) + ( 3 , - 1 ) = ( 5 , 3 )$ . We also define the negation $- z \ \mathrm { o f } \ z \ \mathrm { t o }$ be the complex number $- z : = ( - a , - b )$ , thus for instance $- ( 3 , - 1 ) = ( - 3 , 1 )$ We also define the complex zero 0 to be the complex number $0 _ { \mathbf { C } } =$ (0, 0). 

It is easy to see that notion of addition is well-defined in the sense that if $z = z ^ { \prime }$ and $w = w ^ { \prime }$ then $z + w = z ^ { \prime } + w ^ { \prime }$ . Similarly for negation. The complex addition, negation, and zero operations obey the usual laws of arithmetic: 

Lemma 4.6.4 (The complex numbers are an additive group). If z<sub>1</sub>, z<sub>2</sub>, z are complex numbers, then we have the commutative property $z _ { 1 } + z _ { 2 } = z _ { 2 } + z _ { 1 }$ , the associative property $( z _ { 1 } + z _ { 2 } ) + z _ { 3 } = z _ { 1 } + ( z _ { 2 } + z _ { 3 } )$ , $t h e \ i d e n t i t y \ p r o p e r t y \ z _ { 1 } + 0 _ { \mathbf { C } } = 0 _ { \mathbf { C } } + z _ { 1 } = z _ { 1 }$ , and the inverse property $z _ { 1 } + ( - z _ { 1 } ) = ( - z _ { 1 } ) + z _ { 1 } = 0 _ { \mathbf { C } }$ 

Proof. See Exercise 4.6.1. 

Next, we define the notion of complex multiplication and reciprocal. The informal justification of the complex multiplication rule is 

$$
\begin{array}{r l} (a, b) \cdot (c, d) & = (a + b i) (c + d i) \\ & = a c + a d i + b i c + b i d i \\ & = (a c - b d) + (a d + b c) i \\ & = (a c - b d, a d + b c) \end{array}
$$

since $i ^ { 2 }$ is supposed to equal 1. Thus we define 

Definition 4.6.5 (Complex multiplication). $\operatorname { I f } z = ( a , b )$ and $w = ( c , d )$ are complex numbers, then we define their product zw to be the complex number zw $: = ( a c - b d , a d + b c )$ . We also introduce the complex identity $\mathbf { 1 } _ { \mathbf { C } } : = ( 1 , 0 )$ 

This operation is easily seen to be well-defined, and also obeys the usual laws of arithmetic: 

Lemma 4.6.6. If $z _ { 1 } , z _ { 2 } , z _ { 3 }$ are complex numbers, then we have the commutative property $z _ { 1 } z _ { 2 } = z _ { 2 } z _ { 1 }$ , the associative property $( z _ { 1 } z _ { 2 } ) z _ { 3 } =$ $z _ { 1 } ( z _ { 2 } z _ { 3 } )$ , the identity property $z _ { 1 } 1 _ { \mathbf { C } } = 1 _ { \mathbf { C } } z _ { 1 } = z _ { 1 }$ , and the distributivity properties $z _ { 1 } ( z _ { 2 } + z _ { 3 } ) = z _ { 1 } z _ { 2 } + z _ { 1 } z _ { 3 }$ and $( z _ { 2 } + z _ { 3 } ) z _ { 1 } = z _ { 2 } z _ { 1 } + z _ { 3 } z _ { 1 }$ 

Proof. See Exercise 4.6.2. 

The above lemma can also be stated more succinctly, as the assertion that C is a commutative ring. As is usual, we now write $z \textrm { - } w$ as shorthand for $z + ( - w )$ 

We now identify the real numbers R with a subset of the complex numbers C by identifying any real number x with the complex number $( x , 0 )$ , thus $x \equiv ( x , 0 )$ . Note that this identification is consistent with equality (thus $x = y$ if $( x , 0 ) = ( y , 0 ) )$ , with addition $( x _ { 1 } + x _ { 2 } = x _ { 3 }$ if $( x _ { 1 } , 0 ) + ( x _ { 2 } , 0 ) = ( x _ { 3 } , 0 ) )$ , with negation $( x = - y$ if $( x , 0 ) = - ( y , 0 ) )$ and multiplication $( x _ { 1 } x _ { 2 } = x _ { 3 }$ if $( x _ { 1 } , 0 ) ( x _ { 2 } , 0 ) = ( x _ { 3 } , 0 ) )$ , so we will no longer need to distinguish between “real addition” and “complex addition”, and similarly for equality, negation, and multiplication. For instance, we can compute $3 ( 2 , 4 )$ by identifying the real number 3 with the complex number (3, 0) and then computing $( 3 , 0 ) ( 2 , 4 ) = ( 3 \times 2 -$ $0 \times 4 , 3 \times 4 + 0 \times 2 ) = ( 6 , 1 2 )$ . Note also that $0 \equiv 0 \mathbf { c }$ and $1 \equiv 1 _ { \mathbf { C } } .$ , so we can now drop the C subscripts from the zero 0 and the identity 1. 

We now define i to be the complex number $i : = ( 0 , 1 )$ . We can now reconstruct the informal definition of the complex numbers as a lemma: 

Lemma 4.6.7. Every complex number $z \in \mathbf { C }$ can be written as $z = a { + } b i$ for exactly one pair a, b of real numbers. Also, we have $i ^ { 2 } = - 1$ , and $- z = ( - 1 ) z$ 

Proof. See Exercise 4.6.3. 

Because of this lemma, we will now refer to complex numbers in the more usual notation $a + b i$ , and discard the formal notation $( a , b )$ henceforth. 

Definition 4.6.8 (Real and imaginary parts). If z is a complex number with the representation $z = a + b i$ for some real numbers $a , b ,$ we shall call a the real part of z and denote $\Re ( z ) : = a$ , and call b the imaginary part of z and denote ${ \mathfrak { I } } ( z ) : = b ,$ , thus for instance $\Re ( 3 + 4 i ) = 3$ and $\mathbb { S } ( 3 + 4 i ) = 4$ , and in general $z = \Re ( z ) + i \Im ( z )$ . Note that z is real if $\Im ( z ) = 0$ . We say that z is imaginary if $\Re ( z ) = 0$ , thus for instance 4i is imaginary, while $3 + 4 i$ is neither real nor imaginary, and 0 is both real and imaginary. We define the complex conjugate z of z to be the complex number $\overline { { z } } : = \Re ( z ) - i \Im ( z )$ , thus for instance ${ \overline { { 3 + 4 i } } } = 3 - 4 i$ , $\bar { i } = - i$ , and ${ \overline { { 3 } } } = 3$ 

The operation of complex conjugation has several nice properties: 

Lemma 4.6.9 (Complex conjugation is an involution). Let z, w be complex numbers, then $\overline { { z + w } } = \overline { { z } } + \overline { { w } } , \overline { { - z } } = - \overline { { z } }$ , and $\overline { { z w } } = \overline { { z } } \overline { { w } }$ . Also $\overline { { \overline { { z } } } } = z$ 

Finally, we have $\overline { { z } } = \overline { { w } }$ if and only $i f z = w$ , and $\overline { { z } } = z \ i f$ and only $i f z$ is real. 

Proof. See Exercise 4.6.4. 

The notion of absolute value $| x |$ was defined for rational numbers x in Definition 4.3.1, and this definition extends to real numbers in the obvious manner. However, we cannot extend this definition directly to the complex numbers, as most complex numbers are neither positive nor negative. (For instance, we do not classify i as either a positive or negative number; see Exercise 4.6.15 for some reasons why). However, we can still define absolute value by generalizing the formula $| x | = { \sqrt { x ^ { 2 } } }$ from Exercise 5.6.3: 

Definition 4.6.10 (Complex absolute value). If $z = a + b i$ is a complex number, we define the absolute value $| z |$ of $z$ to be the real number $| z | : = { \sqrt { a ^ { 2 } + b ^ { 2 } } } = ( a ^ { 2 } + b ^ { 2 } ) ^ { 1 / 2 }$ 

From Exercise 5.6.3 we see that this notion of absolute value generalizes the notion of real absolute value. The absolute value has a number of other good properties: 

Lemma 4.6.11 (Properties of complex absolute value). Let z, w be complex numbers. Then $| z |$ is a non-negative real number, and $| z | = 0$ if and only $i f z = 0$ . Also we have the identity $z { \overline { { z } } } = | z | ^ { 2 }$ , and so $| z | = { \sqrt { z { \overline { { z } } } } }$ . As a consequence we have $| z w | = | z | | w |$ and $| \overline { { z } } | = | z |$ . Finally, we have the inequalities 

$$
- | z | \leq \Re (z) \leq | z |; - | z | \leq \Im (z) \leq | z |; | z | \leq | \Re (z) | + | \Im (z) |
$$

as well as the triangle inequality $| z + w | \leq | z | + | w |$ 

Proof. See Exercise 4.6.6. 

Using the notion of absolute value, we can define a notion of reciprocal: 

Definition 4.6.12 (Complex reciprocal). If z is a non-zero complex number, we define the reciprocal $z ^ { - 1 }$ of z to be the complex number $z ^ { - 1 } : = | z | ^ { - 2 } \overline { { z } }$ (note that $| z | ^ { - 2 }$ is well-defined as a positive real number because $| z |$ is positive real, thanks to Lemma 4.6.11). Thus for instance $\begin{array} { r } { ( 1 + 2 i ) ^ { - 1 } = | 1 + 2 i | ^ { - 2 } ( 1 - 2 i ) = ( 1 ^ { 2 } + 2 ^ { 2 } ) ^ { - 1 } ( 1 - 2 i ) = \frac { 1 } { 5 } - \frac { 2 } { 5 } i } \end{array}$ . If $z$ is $\mathrm { z e r o } , z = 0$ , we leave the reciprocal $0 ^ { - 1 }$ undefined. 

From the definition and Lemma 4.6.11, we see that 

$$
z z ^ {- 1} = z ^ {- 1} z = | z | ^ {- 2} \overline {{z}} z = | z | ^ {- 2} | z | ^ {2} = 1,
$$

and so $z ^ { - 1 }$ is indeed the reciprocal of z. We can thus define a notion of quotient $z / w$ for any two complex numbers z, w with $w \neq 0$ in the usual manner by the formula $z / w : = z w ^ { - 1 }$ 

The complex numbers can be given a distance by defining $d ( z , w ) =$ $| z - w |$ 

Lemma 4.6.13. The complex numbers C with the distance d form a metric space. ${ \cal I } f \ ( z _ { n } ) _ { n = 1 } ^ { \infty }$ is a sequence of complex numbers, and $z \textit { i s }$ another complex number, then we have $\operatorname* { l i m } _ { n \to \infty } z _ { n } = z \ i n$ this metric space if and only if $\operatorname* { l i m } _ { n \to \infty } \Re ( z _ { n } ) = \Re ( z )$ and $\operatorname* { l i m } _ { n \to \infty } \Im ( z _ { n } ) = \Im ( z )$ 

Proof. See Exercise 4.6.9. 

□ 

This metric space is in fact complete and connected, but not compact: see Exercises 4.6.10, 4.6.12, 4.6.13. We also have the usual limit laws: 

Lemma 4.6.14 (Complex limit laws). Let $( z _ { n } ) _ { n = 1 } ^ { \infty }$ and $( w _ { n } ) _ { n = 1 } ^ { \infty }$ be convergent sequences of complex numbers, and let c be a complex number. Then the sequences $( z _ { n } + w _ { n } ) _ { n = 1 } ^ { \infty } , ( z _ { n } - w _ { n } ) _ { n = 1 } ^ { \infty } , ( c z _ { n } ) _ { n = 1 } ^ { \infty } , ( z _ { n } w _ { n } ) _ { n = 1 } ^ { \infty } ,$ and $( \overline { { z _ { n } } } ) _ { n = 1 } ^ { \infty }$ are also convergent, with 

$$
\lim _ {n \to \infty} z _ {n} + w _ {n} = \lim _ {n \to \infty} z _ {n} + \lim _ {n \to \infty} w _ {n}
$$

$$
\lim _ {n \to \infty} z _ {n} - w _ {n} = \lim _ {n \to \infty} z _ {n} - \lim _ {n \to \infty} w _ {n}
$$

$$
\lim _ {n \to \infty} c z _ {n} = c \lim _ {n \to \infty} z _ {n}
$$

$$
\lim _ {n \to \infty} z _ {n} w _ {n} = \left(\lim _ {n \to \infty} z _ {n}\right) \left(\lim _ {n \to \infty} w _ {n}\right)
$$

$$
\lim _ {n \to \infty} \overline {{z _ {n}}} = \overline {{\lim _ {n \to \infty} z _ {n}}}
$$

Also, if the $w _ { n }$ are all non-zero and $\scriptstyle \operatorname* { l i m } _ { n \to \infty } w _ { n }$ is also non-zero, then $( z _ { n } / w _ { n } ) _ { n = 1 } ^ { \infty }$ is also a convergent sequence, with 

$$
\lim _ {n \to \infty} z _ {n} / w _ {n} = \left(\lim _ {n \to \infty} z _ {n}\right) / \left(\lim _ {n \to \infty} w _ {n}\right).
$$

Proof. See Exercise 4.6.14. 

## 4.6. A digression on complex numbers

Observe that the real and complex number systems are in fact quite similar; they both obey similar laws of arithmetic, and they have similar structure as metric spaces. Indeed many of the results in this textbook that were proven for real-valued functions, are also valid for complex-valued functions, simply by replacing “real” with “complex” in the proofs but otherwise leaving all the other details of the proof unchanged. Alternatively, one can always split a complex-valued function f into real and imaginary parts $\Re ( f ) , \Im ( f )$ , thus $f = \Re ( f ) + i \Im ( f )$ , and then deduce results for the complex-valued function f from the corresponding results for the real-valued functions $\Re ( f ) , \Im ( f )$ . For instance, the theory of pointwise and uniform convergence from Chapter 3, or the theory of power series from this chapter, extends without any dificulty to complex-valued functions. In particular, we can define the complex exponential function in exactly the same manner as for real numbers: 

Definition 4.6.15 (Complex exponential). $\operatorname { I f } { z }$ is a complex number, we define the function $\exp ( z )$ by the formula 

$$
\exp (z) := \sum_ {n = 0} ^ {\infty} \frac {z ^ {n}}{n !}.
$$

One can state and prove the ratio test for complex series and use it to show that $\exp ( z )$ converges for every z. It turns out that many of the properties from Theorem 4.5.2 still hold: we have that $\exp ( z + w ) = \exp ( z ) \exp ( w )$ , for instance; see Exercise 4.6.16. (The other properties require complex diferentiation and complex integration, but these topics are beyond the scope of this text.) Another useful observation is that $\overline { { \exp ( z ) } } = \exp ( \overline { { z } } )$ ; this can be seen by conjugating the partial sums $\textstyle \sum _ { n = 0 } ^ { N } { \frac { z ^ { n } } { n ! } }$ and taking limits as $N \to \infty$ 

The complex logarithm turns out to be somewhat more subtle, mainly because exp is no longer invertible, and also because the various power series for the logarithm only have a finite radius of convergence (unlike exp, which has an infinite radius of convergence). This rather delicate issue is beyond the scope of this text and will not be discussed here. 

— Exercises — 

Exercise 4.6.1. Prove Lemma 4.6.4. 

Exercise 4.6.2. Prove Lemma 4.6.6. 

Exercise 4.6.3. Prove Lemma 4.6.7. 

Exercise 4.6.4. Prove Lemma 4.6.9. 

Exercise 4.6.5. If z is a complex number, show that $\textstyle \Re ( z ) = { \frac { z + { \overline { { z } } } } { 2 } }$ and $\Re ( z ) =$ $\frac { z - { \overline { { z } } } } { 2 i }$ 

Exercise 4.6.6. Prove Lemma 4.6.11. (Hint: to prove the triangle inequality, first prove that $\Re ( z { \overline { { w } } } ) \leq | z | | w |$ , and hence (from Exercise 4.6.5) that $z { \overline { { w } } } + { \overline { { z } } } w \leq$ $2 | z | | w |$ . Then add $| z | ^ { 2 } + | w | ^ { 2 }$ to both sides of this inequality.) 

Exercise 4.6.7. Show that if $z ,$ w are complex numbers with $w \neq 0$ , then $| z / w | =$ $| z | / | w |$ 

Exercise 4.6.8. Let z, w be non-zero complex numbers. Show that $| z + w | =$ $| z | + | w |$ if and only if there exists a positive real number $c > 0$ such that $z = c w$ 

Exercise 4.6.9. Prove Lemma 4.6.13. 

Exercise 4.6.10. Show that the complex numbers C (with the usual metric d) form a complete metric space. 

Exercise 4.6.11. Let $f : { \mathbf { R } } ^ { 2 }  { \mathbf { C } }$ be the map $f ( a , b ) : = a + b i$ . Show that $f$ is a bijection, and that f and $f ^ { - 1 }$ are both continuous maps. 

Exercise 4.6.12. Show that the complex numbers C (with the usual metric d) form a connected metric space. (Hint: first show that C is path connected, as in Exercise 2.4.7.) 

Exercise 4.6.13. Let E be a subset of C. Show that E is compact if and only if E is closed and bounded. (Hint: combine Exercise 4.6.11 with the Heine-Borel theorem, Theorem 1.5.7.) In particular, show that C is not compact. 

Exercise 4.6.14. Prove Lemma 4.6.14. (Hint: split $z _ { n }$ and $w _ { n }$ into real and imaginary parts and use the usual limit laws, Lemma 6.1.19, combined with Lemma 4.6.13.) 

Exercise 4.6.15. The purpose of this exercise is to explain why we do not try to organize the complex numbers into positive and negative parts. Suppose that there was a notion of a “positive complex number” and a “negative complex number” which obeyed the following reasonable axioms (cf. Proposition 4.2.9): 

(Trichotomy) For every complex number $z ,$ exactly one of the following statements is true: $z$ is positive, $z$ is negative, $z$ is zero. 

(Negation) $\operatorname { I f } z$ is a positive complex number, then $- z$ is negative. If $z$ is a negative complex number, then z is positive. 

(Additivity) $\operatorname { I f } z$ and w are positive complex numbers, then $z + w$ is also positive. 

(Multiplicativity) If z and w are positive complex numbers, then $z w$ is also positive. 

Show that these four axioms are inconsistent, i.e., one can use these axioms to deduce a contradiction. (Hints: first use the axioms to deduce that 1 is positive, and then conclude that 1 is negative. Then apply the Trichotomy axiom to $z = i$ and obtain a contradiction in any one of the three cases). 

Exercise 4.6.16. Prove the ratio test for complex series, and use it to show that the series used to define the complex exponential is absolutely convergent. Then prove that $\exp ( z + w ) = \exp ( z ) \exp ( w )$ for all complex numbers z, w. 

## 4.7 Trigonometric functions

We now discuss the next most important class of special functions, after the exponential and logarithmic functions, namely the trigonometric functions. (There are several other useful special functions in mathematics, such as the hyperbolic trigonometric functions and hypergeometric functions, the gamma and zeta functions, and elliptic functions, but they occur more rarely and will not be discussed here.) 

Trigonometric functions are often defined using geometric concepts, notably those of circles, triangles, and angles. However, it is also possible to define them using more analytic concepts, and in particular the (complex) exponential function. 

Definition 4.7.1 (Trigonometric functions). If z is a complex number, then we define 

$$
\cos (z) := \frac {e ^ {i z} + e ^ {- i z}}{2}
$$

and 

$$
\sin (z) := \frac {e ^ {i z} - e ^ {- i z}}{2 i}.
$$

We refer to cos and sin as the cosine and sine functions respectively. 

These formulae were discovered by Leonhard Euler (1707–1783) in 1748, who recognized the link between the complex exponential and the trigonometric functions. Note that since we have defined the sine and cosine for complex numbers z, we automatically have defined them also for real numbers x. In fact in most applications one is only interested in the trigonometric functions when applied to real numbers. 

From the power series definition of exp, we have 

$$
e ^ {i z} = 1 + i z - \frac {z ^ {2}}{2 !} - \frac {i z ^ {3}}{3 !} + \frac {z ^ {4}}{4 !} + \dots
$$

and 

$$
e ^ {- i z} = 1 - i z - \frac {z ^ {2}}{2 !} + \frac {i z ^ {3}}{3 !} + \frac {z ^ {4}}{4 !} - \dots
$$

and so from the above formulae we have 

$$
\cos (z) = 1 - \frac {z ^ {2}}{2 !} + \frac {z ^ {4}}{4 !} - \dots = \sum_ {n = 0} ^ {\infty} \frac {(- 1) ^ {n} z ^ {2 n}}{(2 n) !}
$$

and 

$$
\sin (z) = z - \frac {z ^ {3}}{3 !} + \frac {z ^ {5}}{5 !} - \dots = \sum_ {n = 0} ^ {\infty} \frac {(- 1) ^ {n} z ^ {2 n + 1}}{(2 n + 1) !}.
$$

In particular, cos(x) and sin(x) are always real whenever x is real. From the ratio test we see that the two power series $\scriptstyle \sum _ { n = 0 } ^ { \infty } { \frac { ( - 1 ) ^ { n } x ^ { 2 n } } { ( 2 n ) ! } }$ 2 $\scriptstyle \sum _ { n = 0 } ^ { \infty } { \frac { ( - 1 ) ^ { n } x ^ { 2 n + 1 } } { ( 2 n + 1 ) ! } }$ are absolutely convergent for every x, thus sin(x) and cos(x) are real analytic at 0 with an infinite radius of convergence. From Exercise 4.2.8 we thus see that the sine and cosine functions are real analytic on all of R. (They are also complex analytic on all of C, but we will not pursue this matter in this text). In particular the sine and cosine functions are continuous and diferentiable. 

We list some basic properties of the sine and cosine functions below. 

Theorem 4.7.2 (Trigonometric identities). Let x, y be real numbers. 

(a) We have sin $( x ) ^ { 2 } + \cos ( x ) ^ { 2 } = 1$ . In particular, we have $\sin ( x ) \in$ [ 1, 1] and cos $( x ) \in [ - 1 , 1 ]$ for all $x \in \mathbf { R }$ 

(b) We have $\sin ^ { \prime } ( x ) = \cos ( x )$ and cos(x) = sin(x). 

(c) We have sin( x) = sin(x) and cos( x) = cos(x). 

(d) We have $\cos ( x + y ) = \cos ( x ) \cos ( y ) - \sin ( x ) \sin ( y )$ and $\sin ( x + y ) =$ sin $( x ) \cos ( y ) + \cos ( x ) \sin ( y )$ 

(e) We have sin(0) = 0 and cos(0) = 1. 

(f ) We have $e ^ { i x } = \cos ( x ) + i \sin ( x )$ and $e ^ { - i x } = \cos ( x ) - i \sin ( x )$ . In particular $\cos ( x ) = \Re ( e ^ { i x } )$ and sin $( x ) = \Im ( e ^ { i x } )$ 

Proof. See Exercise 4.7.1. 

Now we describe some other properties of sin and cos. 

Lemma 4.7.3. There exists a positive number x such that sin(x) is equal to 0. 

## 4.7. Trigonometric functions

Proof. Suppose for sake of contradiction that sin $( x ) \neq 0$ for all $x \in$ $( 0 , \infty )$ Observe that this would also imply that $\cos ( x ) ~ \neq ~ 0$ for all $x \in ( 0 , \infty )$ , since if $\cos ( x ) = 0$ then sin $( 2 x ) = 0$ by Theorem $4 . 7 . 2 ( \mathrm { d } )$ $\mathrm { \left( w h y ? \right) }$ . Since $\cos ( 0 ) = 1$ , this implies by the intermediate value theorem (Theorem 9.7.1) that $\cos ( x ) ~ > ~ 0$ for all $x \mathrm { ~ > ~ 0 ~ } \left( \mathrm { w h y ? } \right)$ . Also, since $\sin ( 0 ) = 0$ and $\sin ^ { \prime } ( 0 ) = 1 > 0$ , we see that sin increasing near 0, hence is positive to the right of 0. By the intermediate value theorem again we conclude that sin $( x ) > 0$ for all $x > 0$ (otherwise sin would have a zero on $( 0 , \infty ) )$ . 

In particular if we define the cotangent function cot $( x ) \quad : = { }$ cos $( x ) / \sin ( x )$ , then cot(x) would be positive and diferentiable on all of $( 0 , \infty )$ . From the quotient rule (Theorem $1 0 . 1 . 1 3 ( \mathrm { h } ) )$ and Theorem 4.7.2 we see that the derivative of cot(x) is $- 1 / \sin ( x ) ^ { 2 }$ (why?) In particular, we have $\cot ^ { \prime } ( x ) \leq - 1$ for all $x > 0$ . By the fundamental theorem of calculus (Theorem 11.9.1) this implies that cot $( x + s ) \leq \cot ( x ) - s$ for all $x > 0$ and $s > 0$ . But letting $s \to \infty$ we see that this contradicts our assertion that cot is positive on $( 0 , \infty ) \ \mathrm { ( w h y ? ) }$ □ 

Let E be the set $E : = \{ x \in ( 0 , + \infty ) : \sin ( x ) = 0 \} , { \mathrm { ~ i . e . , ~ } } E$ is the set of roots of sin on $( 0 , + \infty )$ . By Lemma 4.7.3, E is non-empty. Since $\sin ^ { \prime } ( 0 ) > 0$ , there exists a $c > 0$ such that $E \subseteq [ c , + \infty )$ (see Exercise 4.7.2). Also, since sin is continuous in $[ c , + \infty )$ , E is closed in $[ c , + \infty )$ (why? use Theorem $2 . 1 . 5 ( \mathrm { d } ) )$ . Since $[ c , + \infty )$ is closed in R, we conclude that E is closed in R. Thus E contains all its adherent points, and thus contains inf(E). Thus if we make the definition 

Definition 4.7.4. We define π to be the number 

$$
\pi := \inf \{x \in (0, \infty): \sin (x) = 0 \}
$$

then we have $\pi \in E \subseteq [ c , + \infty )$ (so in particular $\pi > 0 )$ and $\sin ( \pi ) =$ 0. By definition of $\pi _ { \ i }$ , sin cannot have any zeroes in $( 0 , \pi )$ , and so in particular must be positive on $( 0 , \pi )$ , (cf. the arguments in Lemma 4.7.3 using the intermediate value theorem). Since $\cos ^ { \prime } ( x ) = - \sin ( x )$ , we thus conclude that $\cos ( x )$ is strictly decreasing on $( 0 , \pi )$ . Since cos $( 0 ) = 1$ this implies in particular that $\cos ( \pi ) < 1$ ; since $\sin ^ { 2 } ( \pi ) + \cos ^ { 2 } ( \pi ) = 1$ and sin $( \pi ) = 0$ , we thus conclude that $\cos ( \pi ) = - 1$ 

In particular we have Euler’s famous formula 

$$
e ^ {\pi i} = \cos (\pi) + i \sin (\pi) = - 1.
$$

We now conclude with some other properties of sine and cosine. 

Theorem 4.7.5 (Periodicity of trigonometric functions). Let x be a real number. 

(a) We have cos $( x + \pi ) = - \cos ( x )$ and sin $( x + \pi ) = - \sin ( x )$ In particular we have $\cos ( x + 2 \pi ) = \cos ( x )$ and sin $( x + 2 \pi ) = \sin ( x )$ $i . e .$ , sin and cos are periodic with period $2 \pi$ 

(b) We have sin $( x ) = 0$ if and only if $x / \pi$ is an integer. 

(c) We have $\cos ( x ) = 0$ if and only if $x / \pi$ is an integer plus $\scriptstyle 1 / 2 .$ 

Proof. See Exercise 4.7.3. 

We can of course define all the other trigonometric functions: tangent, cotangent, secant, and cosecant, and develop all the familiar identities of trigonometry; some examples of this are given in the exercises. 

— Exercises — 

Exercise 4.7.1. Prove Theorem 4.7.2. (Hint: write everything in terms of exponentials whenever possible.) 

Exercise 4.7.2. Let $f : \mathbf { R }  \mathbf { R }$ be a function which is diferentiable at $x _ { 0 }$ , with $f ( x _ { 0 } ) = 0$ and $f ^ { \prime } ( x _ { 0 } ) \neq 0$ . Show that there exists a $c > 0$ such that $f ( y )$ is non-zero whenever $0 < | x _ { 0 } - y | < c .$ . Conclude in particular that there exists a $c > 0$ such that sin $( x ) \neq 0$ for all $0 < x < c$ 

Exercise 4.7.3. Prove Theorem 4.7.5. (Hint: for (c), you may wish to first compute sin $\left( \pi / 2 \right)$ and $\cos ( \pi / 2 )$ , and then link $\cos ( x )$ to sin $( x + \pi / 2 ) . )$ 

Exercise 4.7.4. Let $x , y$ be real numbers such that $x ^ { 2 } + y ^ { 2 } = 1$ . Show that there is exactly one real number $\theta \in ( - \pi , \pi ]$ such that $x = \sin ( \theta )$ and $y = \cos ( \theta )$ (Hint: you may need to divide into cases depending on whether x, y are positive, negative, or zero.) 

Exercise 4.7.5. Show that if $r , s > 0$ are positive real numbers, and $\theta , \alpha$ are real numbers such that $r e ^ { i \theta } = s e ^ { i \alpha }$ , then $r = s$ and $\theta = \alpha + 2 \pi k$ for some integer k. 

Exercise 4.7.6. Let z be a non-zero complex number. Using Exercise 4.7.4, show that there is exactly one pair of real numbers $r , \theta$ such that $r > 0 , \theta \in ( - \pi , \pi ]$ , and $z = r e ^ { i \theta }$ . (This is sometimes known as the standard polar representation of z.) 

Exercise 4.7.7. For any real number θ and integer n, prove the de Moivre identities 

$$
\cos (n \theta) = \Re ((\cos \theta + i \sin \theta) ^ {n}); \quad \sin (n \theta) = \Im ((\cos \theta + i \sin \theta) ^ {n}).
$$

## 4.7. Trigonometric functions

Exercise 4.7.8. Let tan $\mathbf { \varepsilon } : \ ( - \pi / 2 , \pi / 2 ) \ \to \ \mathbf { R }$ be the tangent function $\tan ( x ) : = \sin ( x ) / \cos ( x )$ . Show that tan is diferentiable and monotone increasing, with $\textstyle { \frac { d } { d x } } \tan ( x ) \ = \ 1 + \tan ( x ) ^ { 2 }$ , and that $\mathrm { l i m } _ { x \to \pi / 2 } \tan ( x ) \ = \ + \infty$ and $\begin{array} { r } { \operatorname* { l i m } _ { x \to - \pi / 2 } \tan ( x ) = - \infty } \end{array}$ . Conclude that tan is in fact a bijection from $( - \pi / 2 , \pi / 2 ) \overset { \cdot } {  } { \bf R }$ , and thus has an inverse function $\tan ^ { - 1 } : \mathbf { R }  ( - \pi / 2 , \pi / 2 )$ (this function is called the arctangent function). Show that $\tan ^ { - 1 }$ is diferentiable and $\begin{array} { r } { \frac { d } { d x } \tan ^ { - 1 } ( x ) = \frac { 1 } { 1 + x ^ { 2 } } } \end{array}$ 

Exercise 4.7.9. Recall the arctangent function $\tan ^ { - 1 }$ from Exercise 4.7.8. By modifying the proof of Theorem 4.5.6(e), establish the identity 

$$
\tan^ {- 1} (x) = \sum_ {n = 0} ^ {\infty} \frac {(- 1) ^ {n} x ^ {2 n + 1}}{2 n + 1}
$$

for all $x \in ( - 1 , 1 )$ . Using Abel’s theorem (Theorem 4.3.1) to extend this identity to the case $x = 1$ , conclude in particular the identity 

$$
\pi = 4 - \frac {4}{3} + \frac {4}{5} - \frac {4}{7} + \ldots = 4 \sum_ {n = 0} ^ {\infty} \frac {(- 1) ^ {n}}{2 n + 1}.
$$

(Note that the series converges by the alternating series test, Proposition 7.2.12). Conclude in particular that $4 - { \frac { 4 } { 3 } } < \pi < 4$ . (One can of course compute $\pi = 3 . 1 4 1 5 9 2 6 . .$ . to much higher accuracy, though if one wishes to do so it is advisable to use a diferent formula than the one above, which converges very slowly). 

Exercise 4.7.10. Let $f : \mathbf { R }  \mathbf { R }$ be the function 

$$
f (x) := \sum_ {n = 1} ^ {\infty} 4 ^ {- n} \cos (3 2 ^ {n} \pi x).
$$

(a) Show that this series is uniformly convergent, and that f is continuous. 

(b) Show that for every integer j and every integer $m \geq 1$ , we have 

$$
\left| f \left(\frac {j + 1}{3 2 ^ {m}}\right) - f \left(\frac {j}{3 2 ^ {m}}\right) \right| \geq 4 ^ {- m}.
$$

(Hint: use the identity 

$$
\sum_ {n = 1} ^ {\infty} a _ {n} = \left(\sum_ {n = 1} ^ {m - 1} a _ {n}\right) + a _ {m} + \sum_ {n = m + 1} ^ {\infty} a _ {n}
$$

for certain sequences $a _ { n }$ . Also, use the fact that the cosine function is periodic with period 2π, as well as the geometric series formula $\textstyle \sum _ { n = 0 } ^ { \infty } r ^ { n } = { \frac { 1 } { 1 - r } }$ for any $| r | < 1$ . Finally, you will need the inequal-${ \mathrm { i t y ~ } } | \cos ( x ) - \cos ( y ) | \leq | x - y |$ for any real numbers x and $y ;$ this can be proven by using the mean value theorem (Corollary 10.2.9), or the fundamental theorem of calculus (Theorem 11.9.4).) 

(c) Using ${ \mathrm { ( b ) } }$ , show that for every real number $x _ { 0 }$ , the function $f$ is not diferentiable at $x _ { 0 }$ . (Hint: for every $x _ { 0 }$ and every $m \geq 1$ , there exists an integer $j$ such that $j \leq 3 2 ^ { m } x _ { 0 } \leq j + 1$ , thanks to Exercise 5.4.3.) 

(d) Explain briefly why the result in (c) does not contradict Corollary 3.7.3. 

## Chapter 5

## Fourier series

In the previous two chapters, we discussed the issue of how certain functions (for instance, compactly supported continuous functions) could be approximated by polynomials. Later, we showed how a diferent class of functions (real analytic functions) could be written exactly (not approximately) as an infinite polynomial, or more precisely a power series. 

Power series are already immensely useful, especially when dealing with special functions such as the exponential and trigonometric functions discussed earlier. However, there are some circumstances where power series are not so useful, because one has to deal with functions $( \mathrm { e . g . , ~ } \sqrt { x } )$ which are not real analytic, and so do not have power series. 

Fortunately, there is another type of series expansion, known as Fourier series, which is also a very powerful tool in analysis (though used for slightly diferent purposes). Instead of analyzing compactly supported functions, it instead analyzes periodic functions; instead of decomposing into polynomials, it decomposes into trigonometric polynomials. Roughly speaking, the theory of Fourier series asserts that just about every periodic function can be decomposed as an (infinite) sum of sines and cosines. 

Remark 5.0.6. Jean-Baptiste Fourier (1768-1830) was, among other things, an administrator accompanying Napoleon on his invasion of Egypt, and then a Prefect in France during Napoleons reign. After the Napoleonic wars, he returned to mathematics. He introduced Fourier series in an important 1807 paper in which he used them to solve what is now known as the heat equation. At the time, the claim that every periodic function could be expressed as a sum of sines and cosines was extremely controversial, even such leading mathematicians as Euler declared that it was impossible. Nevertheless, Fourier managed to show that this was indeed the case, although the proof was not completely rigorous and was not totally accepted for almost another hundred years. 

There will be some similarities between the theory of Fourier series and that of power series, but there are also some major diferences. For instance, the convergence of Fourier series is usually not uniform (i.e., not in the $L ^ { \infty }$ metric), but instead we have convergence in a diferent metric, the $L ^ { 2 } { \mathrm { - m e t r i c } }$ . Also, we will need to use complex numbers heavily in our theory, while they played only a tangential rˆole in power series. 

The theory of Fourier series (and of related topics such as Fourier integrals and the Laplace transform) is vast, and deserves an entire course in itself. It has many, many applications, most directly to diferential equations, signal processing, electrical engineering, physics, and analysis, but also to algebra and number theory. We will only give the barest bones of the theory here, however, and almost no applications. 

## 5.1 Periodic functions

The theory of Fourier series has to do with the analysis of periodic functions, which we now define. It turns out to be convenient to work with complex-valued functions rather than real-valued ones. 

Definition 5.1.1. Let $L > 0$ be a real number. A function $f : \mathbf { R }  \mathbf { C }$ is periodic with period L, or L-periodic, if we have $f ( x + L ) = f ( x )$ for every real number x. 

Example 5.1.2. The real-valued functions $f ( x ) = \sin ( x )$ and $f ( x ) =$ $\cos ( x )$ are 2π-periodic, as is the complex-valued function $f ( x ) = e ^ { i x }$ These functions are also 4π-periodic, 6π-periodic, etc. (why?). The function $f ( x ) = x ,$ , however, is not periodic. The constant function $f ( x ) = 1$ is L-periodic for every L. 

Remark 5.1.3. If a function f is L-periodic, then we have $f ( x + k L ) =$ $f ( x )$ for every integer k (why? Use induction for the positive k, and then use a substitution to convert the positive k result to a negative k result. The $k = 0$ case is of course trivial). In particular, if a function f is 1-periodic, then we have $f ( x + k ) = f ( x )$ for every $k \in \mathbf { Z }$ . Because of this, 1-periodic functions are sometimes also called Z-periodic (and L-periodic functions called $L \mathbf { Z } { \mathrm { - p e r i o d i c } } )$ 

Example 5.1.4. For any integer n, the functions cos(2πnx), sin(2πnx), and $e ^ { 2 \pi i n x }$ are all Z-periodic. (What happens when n is not an integer?). 

Another example of a Z-periodic function is the function $f : \mathbf { R }  \mathbf { C }$ defined by $f ( x ) : = 1$ when $x \in [ n , n + \frac { 1 } { 2 } )$ for some integer n, and $f ( x ) : = 0$ when $x \in [ n + \frac { 1 } { 2 } , n + 1 )$ for some integer n. This function is an example of a square wave. 

Henceforth, for simplicity, we shall only deal with functions which are Z-periodic (for the Fourier theory of L-periodic functions, see Exercise 5.5.6). Note that in order to completely specify a Z-periodic function $f : \mathbf { R }  \mathbf { C }$ , one only needs to specify its values on the interval $[ 0 , 1 )$ 1 since this will determine the values of f everywhere else. This is because every real number x can be written in the form $x = k + y$ where k is an integer (called the integer part of $x _ { i }$ , and sometimes denoted $[ x ] )$ and $y \in [ 0 , 1 )$ (this is called the fractional part of $x ,$ , and sometimes denoted $\{ x \} )$ ; see Exercise 5.1.1. Because of this, sometimes when we wish to describe a $\mathbf { Z } { \mathrm { - p e r i o d i c } }$ function f we just describe what it does on the interval [0, 1), and then say that it is extended periodically to all of R. This means that we define $f ( x )$ for any real number x by setting $f ( x ) : = f ( y )$ , where we have decomposed $x = k + y$ as discussed above. (One can in fact replace the interval [0, 1) by any other half-open interval of length 1, but we will not do so here.) 

The space of complex-valued continuous Z-periodic functions is denoted $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ . (The notation $\mathbf { R } / \mathbf { Z }$ comes from algebra, and denotes the quotient group of the additive group R by the additive group $\mathbf { Z } ;$ more information in this can be found in any algebra text.) By “continuous” we mean continuous at all points on $\mathbf { R } ;$ merely being continuous on an interval such as [0, 1] will not sufice, as there may be a discontinuity between the left and right limits at 1 (or at any other integer). Thus for instance, the functions sin(2πnx), cos(2πnx), and $e ^ { 2 \pi i n x }$ are all elements of $C ( { \bf R } / { \bf Z } ; { \bf C } )$ , as are the constant functions, however the square wave function described earlier is not in $C ( { \bf R } / { \bf Z } ; { \bf C } )$ because it is not continuous. Also the function sin(x) would also not qualify to be in $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ since it is not Z-periodic. 

Lemma 5.1.5 (Basic properties of $C ( { \bf R } / { \bf Z } ; { \bf C } ) )$ . 

(a) (Boundedness) If $f \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ , then f is bounded $( i . e .$ , there exists a real number $M > 0$ such that $| f ( x ) | \leq M$ for all $x \in \mathbf { R } )$ 

(b) (Vector space and algebra properties) If $f , g \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ , then the functions $f + g , f - g$ , and fg are also in $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ . Also, if c is any complex number, then the function $c f$ is also in $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ 

(c) (Closure under uniform limits) If $( f _ { n } ) _ { n = 1 } ^ { \infty }$ is a sequence of functions in $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ which converges uniformly to another function $f : \mathbf { R }  \mathbf { C }$ , then f is also in $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ 

Proof. See Exercise 5.1.2. 

One can make $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ into a metric space by re-introducing the now familiar sup-norm metric 

$$
d _ {\infty} (f, g) = \sup _ {x \in \mathbf {R}} | f (x) - g (x) | = \sup _ {x \in [ 0, 1)} | f (x) - g (x) |
$$

of uniform convergence. (Why is the first supremum the same as the second?) See Exercise 5.1.3. 

## — Exercises —

Exercise 5.1.1. Show that every real number x can be written in exactly one way in the form $x = k + y $ , where k is an integer and $y \in [ 0 , 1 )$ . (Hint: to prove existence of such a representation, set $k : = \operatorname* { s u p } \{ l \in \mathbf { Z } : l \leq x \} . )$ 

Exercise 5.1.2. Prove Lemma 5.1.5. (Hint: for (a), first show that f is bounded on $[ 0 , 1 ] . )$ 

Exercise 5.1.3. Show that $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ with the sup-norm metric $d _ { \infty }$ is a metric space. Furthermore, show that this metric space is complete. 

## 5.2 Inner products on periodic functions

From Lemma 5.1.5 we know that we can add, subtract, multiply, and take limits of continuous periodic functions. We will need a couple more operations on the space $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ , though. The first one is that of inner product. 

Definition 5.2.1 (Inner product). If $f , g \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ , we define the inner product $\langle f , g \rangle$ to be the quantity 

$$
\langle f, g \rangle = \int_ {[ 0, 1 ]} f (x) \overline {{g (x)}} d x.
$$

Remark 5.2.2. In order to integrate a complex-valued function, $f ( x ) =$ $g ( x ) + i h ( x )$ , we use the definition that $\begin{array} { r } { \int _ { [ a , b ] } f : = \int _ { [ a , b ] } g + i \int _ { [ a , b ] } h ; \mathrm { i . e . } } \end{array}$ , we integrate the real and imaginary parts of the function separately. Thus for instance $\begin{array} { r } { \int _ { [ 1 , 2 ] } ( 1 + i x ) \ d x = \int _ { [ 1 , 2 ] } 1 \ d x + i \int _ { [ 1 , 2 ] } x \ d x = 1 + \frac { 3 } { 2 } i } \end{array}$ . It is easy to verify that all the standard rules of calculus (integration by parts, fundamental theorem of calculus, substitution, etc.) still hold when the functions are complex-valued instead of real-valued. 

Example 5.2.3. Let f be the constant function $f ( x ) : = 1$ , and let $g ( x )$ be the function $g ( x ) : = e ^ { 2 \pi i x }$ . Then we have 

$$
\begin{array}{r l} \langle f, g \rangle & = \int_ {[ 0, 1 ]} 1 e ^ {\overline {{2 \pi i x}}} d x \\ & = \int_ {[ 0, 1 ]} e ^ {- 2 \pi i x} d x \\ & = \frac {e ^ {- 2 \pi i x}}{- 2 \pi i} | _ {x = 0} ^ {x = 1} \\ & = \frac {e ^ {- 2 \pi i} - e ^ {0}}{- 2 \pi i} \\ & = \frac {1 - 1}{- 2 \pi i} \\ & = 0. \end{array}
$$

Remark 5.2.4. In general, the inner product $\langle f , g \rangle$ will be a complex number. (Note that $f ( x ) { \overline { { g ( x ) } } }$ will be Riemann integrable since both functions are bounded and continuous.) 

Roughly speaking, the inner product $\langle f , g \rangle$ is to the space $C ( { \bf R } / { \bf Z } ; { \bf C } )$ what the dot product $x \cdot y$ is to Euclidean spaces such as $\mathbf { R } ^ { n }$ . We list some basic properties of the inner product below; a more in-depth study of inner products on vector spaces can be found in any linear algebra text but is beyond the scope of this text. 

Lemma 5.2.5. Let $f , g , h \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ 

(a) (Hermitian property) We have $\langle g , f \rangle = { \overline { { \langle f , g \rangle } } }$ 

(b) (Positivity) We have $\langle f , f \rangle \geq 0$ . Furthermore, we have $\langle f , f \rangle = 0$ if and only if $f = 0 \ ( i . e . , f ( x ) = 0$ for all $x \in \mathbf { R } )$ 

(c) (Linearity in the first variable) We have $\langle f + g , h \rangle = \langle f , h \rangle + \langle g , h \rangle$ For any complex number c, we have $\langle c f , g \rangle = c \langle f , g \rangle$ 

(d) (Antilinearity in the second variable) We have $\left. f , g + h \right. = \left. f , g \right. +$ $\langle f , h \rangle$ . For any complex number c, we have $\langle f , c g \rangle = \overline { { c } } \langle f , g \rangle$ 

Proof. See Exercise 5.2.1. 

From the positivity property, it makes sense to define the $L ^ { 2 }$ norm $\| f \| _ { 2 }$ of a function $f \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ by the formula 

$$
\| f \| _ {2} := \sqrt {\langle f , f \rangle} = \left(\int_ {[ 0, 1 ]} f (x) \overline {{f (x)}} d x\right) ^ {1 / 2} = \left(\int_ {[ 0, 1 ]} | f (x) | ^ {2} d x\right) ^ {1 / 2}.
$$

Thus $\| f \| _ { 2 } \geq 0$ for all f. The norm $\| f \| _ { 2 }$ is sometimes called the root mean square of $f$ . 

Example 5.2.6. If $f ( x )$ is the function $e ^ { 2 \pi i x }$ , then 

$$
\| f \| _ {2} = \left(\int_ {[ 0, 1 ]} e ^ {2 \pi i x} e ^ {- 2 \pi i x} d x\right) ^ {1 / 2} = \left(\int_ {[ 0, 1 ]} 1 d x\right) ^ {1 / 2} = 1 ^ {1 / 2} = 1.
$$

This $L ^ { 2 }$ norm is related to, but is distinct from, the $L ^ { \infty }$ norm $\| f \| _ { \infty } : = \operatorname* { s u p } _ { x \in \mathbf { R } } | f ( x ) |$ . For instance, if $f ( x ) = \sin ( x )$ , then $\| f \| _ { \infty } = 1$ but $\begin{array} { r } { \| \boldsymbol { f } \| _ { 2 } = \frac { 1 } { \sqrt { 2 } } . } \end{array}$ . In general, the best one can say is that $0 \leq \| f \| _ { 2 } \leq$ $\| f \| _ { \infty } ;$ ; see Exercise 5.2.3. 

Some basic properties of the $L ^ { 2 }$ norm are given below. 

Lemma 5.2.7. Let $f , g \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ 

(a) (Non-degeneracy) We have $\| f \| _ { 2 } = 0$ if and only if $f = 0$ 

(b) (Cauchy-Schwarz inequality) We have $| \langle f , g \rangle | \leq \| f \| _ { 2 } \| g \| _ { 2 }$ 

(c) (Triangle inequality) We have $\| f + g \| _ { 2 } \leq \| f \| _ { 2 } + \| g \| _ { 2 }$ 

(d) (Pythagoras’ theorem) If $\langle f , g \rangle = 0 _ { ; }$ , then $\lVert f + g \rVert _ { 2 } ^ { 2 } = \lVert f \rVert _ { 2 } ^ { 2 } + \lVert g \rVert _ { 2 } ^ { 2 } \mathrm { . }$ 

(e) (Homogeneity) We have $\| c f \| _ { 2 } = | c | \| f \| _ { 2 }$ for all $c \in \mathbf { C }$ 

Proof. See Exercise 5.2.4. 

In light of Pythagoras’ theorem, we sometimes say that f and g are orthogonal if $\langle f , g \rangle = 0$ 

We can now define the $L ^ { 2 }$ metric $d _ { L ^ { 2 } }$ on $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ by defining 

$$
d _ {L ^ {2}} (f, g) := \| f - g \| _ {2} = \left(\int_ {[ 0, 1 ]} | f (x) - g (x) | ^ {2} d x\right) ^ {1 / 2}.
$$

Remark 5.2.8. One can verify that $d _ { L ^ { 2 } }$ is indeed a metric (Exercise 5.2.2). Indeed, the $L ^ { 2 }$ metric is very similar to the $l ^ { 2 }$ metric on Euclidean spaces $\mathbf { R } ^ { n }$ , which is why the notation is deliberately chosen to be similar; you should compare the two metrics yourself to see the analogy. 

Note that a sequence $f _ { n }$ of functions in $C ( { \bf R } / { \bf Z } ; { \bf C } )$ will converge in the $L ^ { 2 }$ metric to $f \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ if $d _ { L ^ { 2 } } ( f _ { n } , f ) \to 0$ as $n  \infty$ , or in other words that 

$$
\lim _ {n \to \infty} \int_ {[ 0, 1 ]} | f _ {n} (x) - f (x) | ^ {2} d x = 0.
$$

Remark 5.2.9. The notion of convergence in $L ^ { 2 }$ metric is diferent from that of uniform or pointwise convergence; see Exercise 5.2.6. 

Remark 5.2.10. The $L ^ { 2 }$ metric is not as well-behaved as the $L ^ { \infty }$ metric. For instance, it turns out the space $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ is not complete in the $L ^ { 2 }$ metric, despite being complete in the $L ^ { \infty }$ metric; see Exercise 5.2.5. 

— Exercises — 

Exercise 5.2.1. Prove Lemma 5.2.5. (Hint: the last part of (b) is a little tricky. You may need to prove by contradiction, assuming that f is not the zero function, and then show that $\int _ { [ 0 , 1 ] } | f ( x ) | ^ { 2 }$ is strictly positive. You will need to use the fact that $f ,$ and hence ${ \dot { | f | } } .$ is continuous, to do this.) 

Exercise 5.2.2. Prove that the $L ^ { 2 }$ metric $d _ { L ^ { 2 } }$ on $C ( { \bf R } / { \bf Z } ; { \bf C } )$ does indeed turn $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ into a metric space. (cf. Exercise 1.1.6). 

Exercise 5.2.3. If $f \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ is a non-zero function, show that $0 < \| f \| _ { 2 } \leq$ $\| f \| _ { L ^ { \infty } }$ . Conversely, if $0 < A \le$ B are real numbers, so that there exists a non-zero function $f \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ such that $\| f \| _ { 2 } = A$ and $\| f \| _ { \infty } = B .$ . (Hint: let g be a non-constant non-negative real-valued function in $C ( { \bf R } / { \bf Z } ; { \bf C } )$ , and consider functions f of the form $\dot { \boldsymbol { f } } = ( c + d \boldsymbol { g } ) ^ { 1 / 2 }$ for some constant real numbers $c , d > 0 . )$ 

Exercise 5.2.4. Prove Lemma 5.2.7. (Hint: use Lemma 5.2.5 frequently. For the Cauchy-Schwarz inequality, begin with the positivity property $\langle f , f \rangle \geq 0$ , but with $f$ replaced by the function $f \| g \| _ { 2 } ^ { 2 } - \langle f , g \rangle g$ , and then simplify using Lemma 5.2.5. You may have to treat the case $\| g \| _ { 2 } = 0$ separately. Use the Cauchy-Schwarz inequality to prove the triangle inequality.) 

Exercise 5.2.5. Find a sequence of continuous periodic functions which converge in $L ^ { 2 }$ to a discontinuous periodic function. (Hint: try converging to the square wave function.) 

Exercise 5.2.6. Let $f \in C ( \mathbf { R } / \mathbf { Z } , \mathbf { C } )$ , and let $( f _ { n } ) _ { n = 1 } ^ { \infty }$ be a sequence of functions in $C ( { \bf R } / { \bf Z } ; { \bf C } )$ 

(a) Show that if $f _ { n }$ converges uniformly to $f _ { : }$ , then $f _ { n }$ also converges to $f$ in the $L ^ { 2 }$ metric. 

(b) Give an example where $f _ { n }$ converges to f in the $L ^ { 2 }$ metric, but does not converge to $f$ uniformly. (Hint: take $f = 0$ . Try to make the functions $f _ { n }$ large in sup norm.) 

(c) Give an example where $f _ { n }$ converges to f in the $L ^ { 2 }$ metric, but does not converge to $f$ pointwise. (Hint: take $f = 0$ . Try to make the functions $f _ { n }$ large at one point.) 

(d) Give an example where $f _ { n }$ converges to f pointwise, but does not converge to $f$ in the $L ^ { 2 }$ metric. (Hint: take $f = 0$ . Try to make the functions $f _ { n }$ large in $L ^ { 2 }$ norm.) 

## 5.3 Trigonometric polynomials

We now define the concept of a trigonometric polynomial. Just as polynomials are combinations of the functions $x ^ { n }$ (sometimes called monomials), trigonometric polynomials are combinations of the functions e<sup>2πinx</sup> (sometimes called characters). 

Definition 5.3.1 (Characters). For every integer n, we let $\textstyle e _ { n } \in$ $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ denote the function 

$$
e _ {n} (x) := e ^ {2 \pi i n x}.
$$

This is sometimes referred to as the character with frequency n. 

Definition 5.3.2 (Trigonometric polynomials). A function f in $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ is said to be a trigonometric polynomial if we can write $\begin{array} { r } { f = \sum _ { n = - N } ^ { N } c _ { n } e _ { n } } \end{array}$ for some integer $N \geq 0$ and some complex numbers $( c _ { n } ) _ { n = - N } ^ { N }$ 

Example 5.3.3. The function $f = 4 e _ { - 2 } + i e _ { - 1 } - 2 e _ { 0 } + 0 e _ { 1 } - 3 e _ { 2 }$ is a trigonometric polynomial; it can be written more explicitly as 

$$
f (x) = 4 e ^ {- 4 \pi i x} + i e ^ {- 2 \pi i x} - 2 - 3 e ^ {4 \pi i x}.
$$

Example 5.3.4. For any integer n, the function cos(2πnx) is a trigonometric polynomial, since 

$$
\cos (2 \pi n x) = \frac {e ^ {2 \pi i n x} + e ^ {- 2 \pi i n x}}{2} = \frac {1}{2} e _ {- n} + \frac {1}{2} e _ {n}.
$$

Similarly the function $\sin ( 2 \pi n x ) = { \frac { - 1 } { 2 i } } e _ { - n } + { \frac { 1 } { 2 i } } e _ { n }$ is a trigonometric polynomial. In fact, any linear combination of sines and cosines is also a trigonometric polynomial, for instance $3 + i \cos ( 2 \pi x ) + 4 i \sin ( 4 \pi x )$ is a trigonometric polynomial. 

The Fourier theorem will allow us to write any function in $C ( { \bf R } / { \bf Z } ; { \bf C } )$ as a Fourier series, which is to trigonometric polynomials what power series is to polynomials. To do this we will use the inner product structure from the previous section. The key computation is 

Lemma 5.3.5 (Characters are an orthonormal system). For any integers n and m, we have $\langle e _ { n } , e _ { m } \rangle = 1$ when $n = m$ and $\langle e _ { n } , e _ { m } \rangle = 0$ when $n \neq m$ . Also, we have $\| e _ { n } \| = 1$ 

## 5.3. Trigonometric polynomials

Proof. See Exercise 5.3.2. 

As a consequence, we have a formula for the co-eficients of a trigonometric polynomial. 

Corollary 5.3.6. Let $\begin{array} { r } { f = \sum _ { n = - N } ^ { N } c _ { n } e _ { n } } \end{array}$ be a trigonometric polynomial. Then we have the formula 

$$
c _ {n} = \langle f, e _ {n} \rangle
$$

for all integers $- N \leq n \leq N$ . Also, we have $\boldsymbol { 0 } ~ = ~ \langle \boldsymbol { f } , \boldsymbol { e } _ { n } \rangle$ whenever $n > N$ or $n < - N$ . Also, we have the identity 

$$
\| f \| _ {2} ^ {2} = \sum_ {n = - N} ^ {N} | c _ {n} | ^ {2}.
$$

Proof. See Exercise 5.3.3. 

We rewrite the conclusion of this corollary in a diferent way. 

Definition 5.3.7 (Fourier transform). For any function $\qquad f \quad \in \qquad $ $C ( { \bf R } / { \bf Z } ; { \bf R } )$ , and any integer $\mathbf { \psi } _ { n } \in \mathbf { \Xi } \mathbf { Z }$ , we define the $n ^ { t h }$ Fourier coeficient $o f f .$ , denoted ${ \hat { f } } ( n )$ , by the formula 

$$
\hat {f} (n) := \langle f, e _ {n} \rangle = \int_ {[ 0, 1 ]} f (x) e ^ {- 2 \pi i n x} d x.
$$

The function ${ \hat { f } } : \mathbf { Z } \to \mathbf { C }$ is called the Fourier transform of $f .$ . 

From Corollary 5.3.6, we see that whenever $\begin{array} { r } { f = \sum _ { n = - N } ^ { N } c _ { n } e _ { n } } \end{array}$ is a trigonometric polynomial, we have 

$$
f = \sum_ {n = - N} ^ {N} \langle f, e _ {n} \rangle e _ {n} = \sum_ {n = - \infty} ^ {\infty} \langle f, e _ {n} \rangle e _ {n}
$$

and in particular we have the Fourier inversion formula 

$$
f = \sum_ {n = - \infty} ^ {\infty} \hat {f} (n) e _ {n}
$$

or in other words 

$$
f (x) = \sum_ {n = - \infty} ^ {\infty} \hat {f} (n) e ^ {2 \pi i n x}.
$$

The right-hand side is referred to as the Fourier series of f. Also, from the second identity of Corollary 5.3.6 we have the Plancherel formula 

$$
\| f \| _ {2} ^ {2} = \sum_ {n = - \infty} ^ {\infty} | \hat {f} (n) | ^ {2}.
$$

Remark 5.3.8. We stress that at present we have only proven the Fourier inversion and Plancherel formulae in the case when f is a trigonometric polynomial. Note that in this case that the Fourier coefficients ${ \hat { f } } ( n )$ are mostly zero (indeed, they can only be non-zero when $- N \leq n \leq N )$ , and so this infinite sum is really just a finite sum in disguise. In particular there are no issues about what sense the above series converge in; they both converge pointwise, uniformly, and in $L ^ { 2 }$ metric, since they are just finite sums. 

In the next few sections we will extend the Fourier inversion and Plancherel formulae to general functions in $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ , not just trigonometric polynomials. (It is also possible to extend the formula to discontinuous functions such as the square wave, but we will not do so here). To do this we will need a version of the Weierstrass approximation theorem, this time requiring that a continuous periodic function be approximated uniformly by trigonometric polynomials. Just as convolutions were used in the proof of the polynomial Weierstrass approximation theorem, we will also need a notion of convolution tailored for periodic functions. 

$$
- \text { Exercises } -
$$

Exercise 5.3.1. Show that the sum or product of any two trigonometric polynomials is again a trigonometric polynomial. 

Exercise 5.3.2. Prove Lemma 5.3.5. 

Exercise 5.3.3. Prove Corollary 5.3.6. (Hint: use Lemma 5.3.5. For the second identity, either use Pythagoras’ theorem and induction, or substitute $\begin{array} { r } { f = \sum _ { n = - N } ^ { N } c _ { n } e _ { n } } \end{array}$ and expand everything out.) 

## 5.4 Periodic convolutions

The goal of this section is to prove the Weierstrass approximation theorem for trigonometric polynomials: 

Theorem 5.4.1. Let $f \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ , and let $\varepsilon > 0$ . Then there exists a trignometric polynomial P such that $\| f - P \| _ { \infty } \leq \varepsilon$ 

This theorem asserts that any continuous periodic function can be uniformly approximated by trigonometric polynomials. To put it another way, if we let $P ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ denote the space of all trigonometric polynomials, then the closure of $P ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ in the $L ^ { \infty }$ metric is $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ 

It is possible to prove this theorem directly from the Weierstrass approximation theorem for polynomials (Theorem 3.8.3), and both theorems are a special case of a much more general theorem known as the Stone-Weierstrass theorem, which we will not discuss here. However we shall instead prove this theorem from scratch, in order to introduce a couple of interesting notions, notably that of periodic convolution. The proof here, though, should strongly remind you of the arguments used to prove Theorem 3.8.3. 

Definition 5.4.2 (Periodic convolution). Let $f , g \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ . Then we define the periodic convolution $f * g : \mathbf { R }  { \mathbf { C } }$ of f and g by the formula 

$$
f * g (x) := \int_ {[ 0, 1 ]} f (y) g (x - y) d y.
$$

Remark 5.4.3. Note that this formula is slightly diferent from the convolution for compactly supported functions defined in Definition 3.8.9, because we are only integrating over [0, 1] and not on all of R. Thus, in principle we have given the symbol $f * g$ two conflicting meanings. However, in practice there will be no confusion, because it is not possible for a non-zero function to both be periodic and compactly supported (Exercise 5.4.1). 

Lemma 5.4.4 (Basic properties of periodic convolution). Let $f , g , h \in$ $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ 

(a) (Closure) The convolution $f * g$ is continuous and Z-periodic. In other words, $f * g \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ 

(b) (Commutativity) We have $f * g = g * f$ 

(c) (Bilinearity) We have $f * ( g + h ) = f * g + f * h$ and $( f + g ) * h =$ $f * h + g * h$ . For any complex number c, we have $c ( f * g ) =$ $( c f ) * g = f * ( c g )$ 

Proof. See Exercise 5.4.2. 

Now we observe an interesting identity: for any $f \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ and any integer n, we have 

$$
f * e _ {n} = \hat {f} (n) e _ {n}.
$$

To prove this, we compute 

$$
\begin{array}{c} {f * e _ {n} (x) = \int_ {[ 0, 1 ]} f (y) e ^ {2 \pi i n (x - y)} d y} \\ {= e ^ {2 \pi i n x} \int_ {[ 0, 1 ]} f (y) e ^ {- 2 \pi i n y} d y = \hat {f} (n) e ^ {2 \pi i n x} = \hat {f} (n) e _ {n}} \end{array}
$$

as desired. 

More generally, we see from Lemma 5.4.4(iii) that for any trigonometric polynomial $\begin{array} { r } { P = \sum _ { n = - N } ^ { n = N } c _ { n } e _ { n } } \end{array}$ , we have 

$$
f * P = \sum_ {n = - N} ^ {n = N} c _ {n} (f * e _ {n}) = \sum_ {n = - N} ^ {n = N} \hat {f} (n) c _ {n} e _ {n}.
$$

Thus the periodic convolution of any function in $C ( { \bf R } / { \bf Z } ; { \bf C } )$ with a trigonometric polynomial, is again a trigonometric polynomial. (Compare with Lemma 3.8.13.) 

Next, we introduce the periodic analogue of an approximation to the identity. 

Definition 5.4.5 (Periodic approximation to the identity). Let $\varepsilon > 0$ and $0 < \delta < 1 / 2$ . A function $f \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ is said to be a periodic $( \varepsilon , \delta )$ approximation to the identity if the following properties are true: 

(a) $f ( x ) \geq 0$ for all $x \in \mathbf { R }$ , and $\begin{array} { r } { \int _ { [ 0 , 1 ] } f = 1 } \end{array}$ 

(b) We have $f ( x ) < \varepsilon$ for all $\delta \leq | x | \leq 1 - \delta .$ 

Now we have an analogue of Lemma 3.8.8: 

Lemma 5.4.6. For every $\varepsilon > 0$ and $0 < \delta < 1 / 2$ , there exists a trigonometric polynomial P which is an $( \varepsilon , \delta )$ approximation to the identity. 

Proof. We sketch the proof of this lemma here, and leave the completion of it to Exercise 5.4.3. Let $N \geq 1$ be an integer. We define the Fej´er kernel $F _ { N }$ to be the function 

$$
F _ {N} = \sum_ {n = - N} ^ {N} \left(1 - \frac {| n |}{N}\right) e _ {n}.
$$

Clearly $F _ { N }$ is a trigonometric polynomial. We observe the identity 

$$
F _ {N} = \frac {1}{N} \left| \sum_ {n = 0} ^ {N - 1} e _ {n} \right| ^ {2}
$$

(why?). But from the geometric series formula (Lemma 7.3.3) we have 

$$
\sum_ {n = 0} ^ {N - 1} e _ {n} (x) = \frac {e _ {N} - e _ {0}}{e _ {1} - e _ {0}} = \frac {e ^ {\pi i (N - 1) x} \sin (\pi N x)}{\sin (\pi x)}
$$

when x is not an integer, (why?) and hence we have the formula 

$$
F _ {N} (x) = \frac {\sin (\pi N x) ^ {2}}{N \sin (\pi x) ^ {2}}.
$$

When $x$ is an integer, the geometric series formula does not apply, but one has $F _ { N } ( x ) = N$ in that case, as one can see by direct computation. In either case we see that $F _ { N } ( x ) \geq 0$ for any x. Also, we have 

$$
\int_ {[ 0, 1 ]} F _ {N} (x) d x = \sum_ {n = - N} ^ {N} \left(1 - \frac {| n |}{N}\right) \int_ {[ 0, 1 ]} e _ {n} = \left(1 - \frac {| 0 |}{N}\right) 1 = 1
$$

(why?). Finally, since sin $( \pi N x ) \leq 1$ , we have 

$$
F _ {N} (x) \leq \frac {1}{N \sin (\pi x) ^ {2}} \leq \frac {1}{N \sin (\pi \delta) ^ {2}}
$$

whenever $\delta < | x | < 1 - \delta$ (this is because sin is increasing on $[ 0 , \pi / 2 ]$ and decreasing on $[ \pi / 2 , \pi ] )$ . Thus by choosing N large enough, we can make $F _ { N } ( x ) \leq \varepsilon$ for all $\delta < | x | < 1 - \delta$ □ 

Proof of Theorem $5 . 4 . 1$ . Let f be any element of $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ ; we know that f is bounded, so that we have some $M > 0$ such that $| f ( x ) | \leq M$ for all $x \in \mathbf { R }$ 

Let $\varepsilon > 0$ be arbitrary. Since f is uniformly continuous, there exists a $\delta > 0$ such that $| f ( x ) - f ( y ) | \leq \varepsilon$ whenever $| x - y | \le \delta$ . Now use Lemma 5.4.6 to find a trigonometric polynomial P which is a $( \varepsilon , \delta )$ approximation to the identity. Then $f * P$ is also a trigonometric polynomial. We now estimate $\| f - f * P \| _ { \infty }$ 

Let x be any real number. We have 

$$
\begin{array}{l} | f (x) - f * P (x) | = | f (x) - P * f (x) | \\ \qquad = \left| f (x) - \int_ {[ 0, 1 ]} f (x - y) P (y) d y \right| \\ \qquad = \left| \int_ {[ 0, 1 ]} f (x) P (y) d y - \int_ {[ 0, 1 ]} f (x - y) P (y) d y \right| \\ \qquad = \left| \int_ {[ 0, 1 ]} (f (x) - f (x - y)) P (y) d y \right| \\ \qquad \leq \int_ {[ 0, 1 ]} | f (x) - f (x - y) | P (y) d y. \end{array}
$$

The right-hand side can be split as 

$$
\begin{array}{c} \int_ {[ 0, \delta ]} | f (x) - f (x - y) | P (y) d y + \int_ {[ \delta , 1 - \delta ]} | f (x) - f (x - y) | P (y) d y \\ + \int_ {[ 1 - \delta , 1 ]} | f (x) - f (x - y) | P (y) d y \end{array}
$$

which we can bound from above by 

$$
\begin{array}{l} \leq \int_ {[ 0, \delta ]} \varepsilon P (y) d y + \int_ {[ \delta , 1 - \delta ]} 2 M \varepsilon d y \\ \quad + \int_ {[ 1 - \delta , 1 ]} | f (x - 1) - f (x - y) | P (y) d y \\ \leq \int_ {[ 0, \delta ]} \varepsilon P (y) d y + \int_ {[ \delta , 1 - \delta ]} 2 M \varepsilon d y + \int_ {[ 1 - \delta , 1 ]} \varepsilon P (y) d y \\ \leq \varepsilon + 2 M \varepsilon + \varepsilon \\ = (2 M + 2) \varepsilon . \end{array}
$$

Thus we have $\| f - f \ast P \| _ { \infty } \leq ( 2 M + 2 ) \varepsilon$ . Since M is fixed and $\varepsilon$ is arbitrary, we can thus make $f * P$ arbitrarily close to f in sup norm, which proves the periodic Weierstrass approximation theorem. □ 

$$
- \mathrm{Exercises} -
$$

Exercise 5.4.1. Show that if $f : \mathbf { R }  \mathbf { C }$ is both compactly supported and Z-periodic, then it is identically zero. 

Exercise 5.4.2. Prove Lemma 5.4.4. (Hint: to prove that $f * g$ is continuous, you will have to do something like use the fact that f is bounded, and $g$ is uniformly continuous, or vice versa. To prove that $f * g = g * f$ , you will need to use the periodicity to “cut and paste” the interval [0, 1].) 

Exercise 5.4.3. Fill in the gaps marked (why?) in Lemma 5.4.6. (Hint: for the first identity, use the identities $| z | ^ { 2 } = z \overline { { z } } , \overline { { e _ { n } } } = e _ { - n }$ , and $e _ { n } e _ { m } = e _ { n + m } . )$ 

## 5.5 The Fourier and Plancherel theorems

Using the Weierstrass approximation theorem (Theorem 5.4.1), we can now generalize the Fourier and Plancherel identities to arbitrary continuous periodic functions. 

Theorem 5.5.1 (Fourier theorem). For any $f \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ , the series $\textstyle \sum _ { n = - \infty } ^ { \infty } { \hat { f } } ( n ) e _ { n }$ converges in $L ^ { 2 }$ metric to f. In other words, we have 

$$
\lim _ {N \to \infty} \left\| f - \sum_ {n = - N} ^ {N} \hat {f} (n) e _ {n} \right\| _ {2} = 0.
$$

Proof. Let $\varepsilon > 0$ . We have to show that there exists an $N _ { 0 }$ such that $\begin{array} { r } { \| f - \sum _ { n = - N } ^ { N } { \hat { f } } ( n ) e _ { n } \| _ { 2 } \leq \varepsilon } \end{array}$ for all suficiently large N. 

By the Weierstrass approximation theorem (Theorem 5.4.1), we can find a trigonometric polynomial $\begin{array} { r } { P ~ = ~ \sum _ { n = - N _ { 0 } } ^ { N _ { 0 } } c _ { n } e _ { n } } \end{array}$ such that $\| f - P \| _ { \infty } \leq \varepsilon$ , for some $N _ { 0 } > 0$ . In particular we have $\| f - P \| _ { 2 } \leq \varepsilon$ 

Now let $N > N _ { 0 }$ , and let $\begin{array} { r } { F _ { N } : = \sum _ { n = - N } ^ { n = N } \hat { f } ( n ) e _ { n } } \end{array}$ . We claim that $\| f - F _ { N } \| _ { 2 } \leq \varepsilon$ . First observe that for any $| m | \leq N$ , we have 

$$
\langle f - F _ {N}, e _ {m} \rangle = \langle f, e _ {m} \rangle - \sum_ {n = - N} ^ {N} \hat {f} (n) \langle e _ {n}, e _ {m} \rangle = \hat {f} (m) - \hat {f} (m) = 0,
$$

where we have used Lemma 5.3.5. In particular we have 

$$
\langle f - F _ {N}, F _ {N} - P \rangle = 0
$$

since we can write $F _ { N } - P$ as a linear combination of the $e _ { m }$ for which $| m | \leq N$ . By Pythagoras’ theorem we therefore have 

$$
\| f - P \| _ {2} ^ {2} = \| f - F _ {N} \| _ {2} ^ {2} + \| F _ {N} - P \| _ {2} ^ {2}
$$

and in particular 

$$
\| f - F _ {N} \| _ {2} \leq \| f - P \| _ {2} \leq \varepsilon
$$

as desired. 

□ 

Remark 5.5.2. Note that we have only obtained convergence of the Fourier series $\textstyle \sum _ { n = - \infty } ^ { \infty } { \hat { f } } ( n ) e _ { n }$ to $f$ in the $L ^ { 2 }$ metric. One may ask whether one has convergence in the uniform or pointwise sense as well, but it turns out (perhaps somewhat surprisingly) that the answer is no to both of those questions. However, if one assumes that the function f is not only continuous, but is also continuously diferentiable, then one can recover pointwise convergence; if one assumes continuously twice diferentiable, then one gets uniform convergence as well. These results are beyond the scope of this text and will not be proven here. However, we will prove one theorem about when one can improve the $L ^ { 2 }$ convergence to uniform convergence: 

Theorem 5.5.3. Let $f ~ \in ~ { \cal C } ( { \bf R } / { \bf Z } ; { \bf C } )$ , and suppose that the series $\scriptstyle \sum _ { n = - \infty } ^ { \infty } | { \hat { f } } ( n ) |$ is absolutely convergent. Then the series $\textstyle \sum _ { n = - \infty } ^ { \infty } { \hat { f } } ( n ) e _ { n }$ converges uniformly to $f$ . In other words, we have 

$$
\lim _ {N \to \infty} \left\| f - \sum_ {n = - N} ^ {N} \hat {f} (n) e _ {n} \right\| _ {\infty} = 0.
$$

Proof. By the Weierstrass M-test (Theorem 3.5.7), we see that $\textstyle \sum _ { n = - \infty } ^ { \infty } { \hat { f } } ( n ) e _ { n }$ converges to some function F, which by Lemma 5.1.5(iii) is also continuous and Z-periodic. (Strictly speaking, the Weierstrass M test was phrased for series from $n = 1$ to $n = \infty$ , but also works for series from $n = - \infty$ to $n = + \infty$ ; this can be seen by splitting the doubly infinite series into two pieces.) Thus 

$$
\lim _ {N \to \infty} \left\| F - \sum_ {n = - N} ^ {N} \hat {f} (n) e _ {n} \right\| _ {\infty} = 0
$$

which implies that 

$$
\lim _ {N \rightarrow \infty} \left\| F - \sum_ {n = - N} ^ {N} \hat {f} (n) e _ {n} \right\| _ {2} = 0
$$

since the $L ^ { 2 }$ norm is always less than or equal to the $L ^ { \infty }$ norm. But the sequence $\textstyle \sum _ { n = - N } ^ { N } { \hat { f } } ( n ) e _ { n }$ is already converging in $L ^ { 2 }$ metric to f by the 

Fourier theorem, so can only converge in $L ^ { 2 }$ metric to F if $F = f$ (cf. Proposition 1.1.20). Thus $F = f$ , and so we have 

$$
\lim _ {N \to \infty} \left\| f - \sum_ {n = - N} ^ {N} \hat {f} (n) e _ {n} \right\| _ {\infty} = 0
$$

as desired. 

□ 

As a corollary of the Fourier theorem, we obtain 

Theorem 5.5.4 (Plancherel theorem). For any $f \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ , the series $\scriptstyle \sum _ { n = - \infty } ^ { \infty } | { \hat { f } } ( n ) | ^ { 2 }$ is absolutely convergent, and 

$$
\| f \| _ {2} ^ {2} = \sum_ {n = - \infty} ^ {\infty} | \hat {f} (n) | ^ {2}.
$$

This theorem is also known as Parseval’s theorem. 

Proof. Let $\varepsilon > 0$ . By the Fourier theorem we know that 

$$
\left\| f - \sum_ {n = - N} ^ {N} \hat {f} (n) e _ {n} \right\| _ {2} \leq \varepsilon
$$

if N is large enough (depending on $\varepsilon )$ . In particular, by the triangle inequality this implies that 

$$
\| f \| _ {2} - \varepsilon \leq \left\| \sum_ {n = - N} ^ {N} \hat {f} (n) e _ {n} \right\| _ {2} \leq \| f \| _ {2} + \varepsilon .
$$

On the other hand, by Corollary 5 we have 

$$
\left\| \sum_ {n = - N} ^ {N} \hat {f} (n) e _ {n} \right\| _ {2} = \left(\sum_ {n = - N} ^ {N} | \hat {f} (n) | ^ {2}\right) ^ {1 / 2}
$$

and hence 

$$
(\| f \| _ {2} - \varepsilon) ^ {2} \leq \sum_ {n = - N} ^ {N} | \hat {f} (n) | ^ {2} \leq (\| f \| _ {2} + \varepsilon) ^ {2}.
$$

Taking lim sup, we obtain 

$$
(\| f \| _ {2} - \varepsilon) ^ {2} \leq \limsup _ {N \to \infty} \sum_ {n = - N} ^ {N} | \hat {f} (n) | ^ {2} \leq (\| f \| _ {2} + \varepsilon) ^ {2}.
$$

Since $\varepsilon$ is arbitrary, we thus obtain by the squeeze test that 

$$
\limsup _ {N \to \infty} \sum_ {n = - N} ^ {N} | \hat {f} (n) | ^ {2} = \| f \| _ {2} ^ {2}
$$

and the claim follows. 

There are many other properties of the Fourier transform, but we will not develop them here. In the exercises you will see a small number of applications of the Fourier and Plancherel theorems. 

— Exercises — 

Exercise 5.5.1. Let $f$ be a function in $C ( { \bf R } / { \bf Z } ; { \bf C } )$ , and define the trigonometric Fourier coeficients $a _ { n } , b _ { n }$ for $n = 0 , 1 , 2 , 3 , \ldots$ by 

$$
a _ {n} := 2 \int_ {[ 0, 1 ]} f (x) \cos (2 \pi n x) d x; b _ {n} := 2 \int_ {[ 0, 1 ]} f (x) \sin (2 \pi n x) d x.
$$

(a) Show that the series 

$$
\frac {1}{2} a _ {0} + \sum_ {n = 1} ^ {\infty} (a _ {n} \cos (2 \pi n x) + b _ {n} \sin (2 \pi n x))
$$

converges in $L ^ { 2 }$ metric to $f .$ (Hint: use the Fourier theorem, and break up the exponentials into sines and cosines. Combine the positive n terms with the negative n terms.) 

(b) Show that if $\textstyle \sum _ { n = 1 } ^ { \infty } a _ { n }$ and $\textstyle \sum _ { n = 1 } ^ { \infty } b _ { n }$ are absolutely convergent, then the above series actually converges uniformly to $f ,$ , and not just in $L ^ { 2 }$ metric. (Hint: use Theorem 5.5.3). 

Exercise 5.5.2. Let $f ( x )$ be the function defined by $f ( x ) = ( 1 - 2 x ) ^ { 2 }$ when $x \in [ 0 , 1 )$ , and extended to be $\mathbf { Z } \mathbf { - }$ -periodic for the rest of the real line. 

(a) Using Exercise 5.5.1, show that the series 

$$
\frac {1}{3} + \sum_ {n = 1} ^ {\infty} \frac {4}{\pi^ {2} n ^ {2}} \cos (2 \pi n x)
$$

converges uniformly to $f .$ 

(b) Conclude that $\begin{array} { r } { \sum _ { n = 1 } ^ { \infty } \frac { 1 } { n ^ { 2 } } = \frac { \pi ^ { 2 } } { 6 } } \end{array}$ . (Hint: evaluate the above series at $x = 0 . )$ 

(c) Conclude that $\textstyle \sum _ { n = 1 } ^ { \infty } { \frac { 1 } { n ^ { 4 } } } = { \frac { \pi ^ { 4 } } { 9 0 } }$ . (Hint: expand the cosines in terms of exponentials, and use Plancherel’s theorem.) 

Exercise 5.5.3. If $f \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ and $P$ is a trigonometric polynomial, show that 

$$
\widehat {f * P} (n) = \hat {f} (n) c _ {n} = \hat {f} (n) \hat {P} (n)
$$

for all integers n. More generally, if $f , g \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ , show that 

$$
\widehat {f * g} (n) = \hat {f} (n) \hat {g} (n)
$$

for all integers $n .$ . (A fancy way of saying this is that the Fourier transform intertwines convolution and multiplication). 

Exercise 5.5.4. Let $f \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ be a function which is diferentiable, and whose derivative $f ^ { \prime }$ is also continuous. Show that $f ^ { \prime }$ also lies in $C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ , and that ${ \widehat { f ^ { \prime } } } ( n ) = 2 \pi i n { \widehat { f } } ( n )$ for all integers $n .$ . 

Exercise 5.5.5. Let $f , g \in C ( \mathbf { R } / \mathbf { Z } ; \mathbf { C } )$ . Prove the Parseval identity 

$$
\Re \int_ {0} ^ {1} f (x) \overline {{g (x)}} d x = \Re \sum_ {n \in \mathbf {Z}} \hat {f} (n) \overline {{\hat {g} (n)}}.
$$

(Hint: apply the Plancherel theorem to $f + g$ and $f - g$ , and subtract the two.) Then conclude that the real parts can be removed, thus 

$$
\int_ {0} ^ {1} f (x) \overline {{g (x)}} d x = \sum_ {n \in \mathbf {Z}} \hat {f} (n) \overline {{\hat {g} (n)}}.
$$

(Hint: apply the first identity with f replaced by $i f . )$ 

Exercise 5.5.6. In this exercise we shall develop the theory of Fourier series for functions of any fixed period $L .$ 

Let $L > 0$ , and let $f : \mathbf { R }  \mathbf { C }$ be a complex-valued function which is continuous and L-periodic. Define the numbers $c _ { n }$ for every integer n by 

$$
c _ {n} := \frac {1}{L} \int_ {[ 0, L ]} f (x) e ^ {- 2 \pi i n x / L} d x.
$$

(a) Show that the series 

$$
\sum_ {n = - \infty} ^ {\infty} c _ {n} e ^ {2 \pi i n x / L}
$$

converges in $L ^ { 2 }$ metric to $f .$ . More precisely, show that 

$$
\lim _ {N \to \infty} \int_ {[ 0, L ]} | f (x) - \sum_ {n = - N} ^ {N} c _ {n} e ^ {2 \pi i n x / L} | ^ {2} d x = 0.
$$

(Hint: apply the Fourier theorem to the function $f ( L x ) . )$ 

(b) If the series $\scriptstyle \sum _ { n = - \infty } ^ { \infty } | c _ { n } |$ is absolutely convergent, show that 

$$
\sum_ {n = - \infty} ^ {\infty} c _ {n} e ^ {2 \pi i n x / L}
$$

converges uniformly to $f .$ 

(c) Show that 

$$
\frac {1}{L} \int_ {[ 0, L ]} | f (x) | ^ {2} d x = \sum_ {n = - \infty} ^ {\infty} | c _ {n} | ^ {2}.
$$

(Hint: apply the Plancherel theorem to the function $f ( L x ) . )$ 

## Chapter 6

## Several variable diferential calculus

## 6.1 Linear transformations

We shall now switch to a diferent topic, namely that of diferentiation in several variable calculus. More precisely, we shall be dealing with maps $f : \mathbf { R } ^ { n }  \mathbf { R } ^ { m }$ from one Euclidean space to another, and trying to understand what the derivative of such a map is. 

Before we do so, however, we need to recall some notions from linear algebra, most importantly that of a linear transformation and a matrix. We shall be rather brief here; a more thorough treatment of this material can be found in any linear algebra text. 

Definition 6.1.1 (Row vectors). Let $n \geq 1$ be an integer. We refer to elements of $\mathbf { R } ^ { n }$ as n-dimensional row vectors. A typical n-dimensional row vector may take the form $x = ( x _ { 1 } , x _ { 2 } , \ldots , x _ { n } )$ , which we abbreviate as $( x _ { i } ) _ { 1 \leq i \leq n } ;$ ; the quantities $x _ { 1 } , x _ { 2 } , \ldots , x _ { n }$ are of course real numbers. If $( x _ { i } ) _ { 1 \leq i \leq n }$ and $( y _ { i } ) _ { 1 \leq i \leq n }$ are n-dimensional row vectors, we can define their vector sum by 

$$
(x _ {i}) _ {1 \leq i \leq n} + (y _ {i}) _ {1 \leq i \leq n} = (x _ {i} + y _ {i}) _ {1 \leq i \leq n},
$$

and also if $c \in \textbf { R }$ is any scalar, we can define the scalar product $c ( x _ { i } ) _ { 1 \leq i \leq n }$ by 

$$
c (x _ {i}) _ {1 \leq i \leq n} := (c x _ {i}) _ {1 \leq i \leq n}.
$$

Of course one has similar operations on $\mathbf { R } ^ { m }$ as well. However, if $n \neq m$ , then we do not define any operation of vector addition between vectors in $\mathbf { R } ^ { n }$ and vectors in ${ \bf R } ^ { m } \left( \mathrm { e . g . , ~ } ( 2 , 3 , 4 ) + ( 5 , 6 ) \right.$ is undefined). We also refer to the vector $( 0 , \ldots , 0 )$ in $\mathbf { R } ^ { n }$ as the zero vector and also denote it by 0. (Strictly speaking, we should denote the zero vector of $\mathbf { R } ^ { n }$ by $0 _ { \mathbf { R } ^ { n } }$ as they are technically distinct from each other and from the number zero, but we shall not take care to make this distinction). We abbreviate $( - 1 ) x { \mathrm { ~ a s ~ } } - x$ 

The operations of vector addition and scalar multiplication obey a number of basic properties: 

Lemma 6.1.2 $( \mathbf { R } ^ { n }$ is a vector space). Let $x , y , z$ be vectors in $\mathbf { R } ^ { n }$ and let $^ { c , }$ d be real numbers. Then we have the commutativity property $x + y = y + x$ , the additive associativity property $( x + y ) + z = x +$ $( y + z )$ , the additive identity property $x + 0 = 0 + x = x $ , the additive inverse property $x + ( - x ) = ( - x ) + x = 0$ , the multiplicative associativity property $( c d ) x = c ( d x )$ , the distributivity properties $c ( x + y ) = c x + c y$ and $( c + d ) x = c x + d x$ , and the multiplicative identity property $1 x = x$ 

Proof. See Exercise 6.1.1. 

Definition 6.1.3 (Transpose). If $( x _ { i } ) _ { 1 \leq i \leq n } = ( x _ { 1 } , x _ { 2 } , \ldots , x _ { n } )$ is an $n -$ dimensional row vector, we can define its transpose $( x _ { i } ) _ { 1 \leq i \leq n } ^ { T }$ by 

$$
(x _ {i}) _ {1 \leq i \leq n} ^ {T} = (x _ {1}, x _ {2}, \ldots , x _ {n}) ^ {T} := \left( \begin{array}{c} x _ {1} \\ x _ {2} \\ \vdots \\ x _ {n} \end{array} \right).
$$

We refer to objects such as $( x _ { i } ) _ { 1 \leq i \leq n } ^ { T }$ as n-dimensional column vectors. 

Remark 6.1.4. There is no functional diference between a row vector and a column vector $( \mathrm { e . g . }$ , one can add and scalar multiply column vectors just as well as we can row vectors), however we shall (rather annoyingly) need to transpose our row vectors into column vectors in order to be consistent with the conventions of matrix multiplication, which we will see later. Note that we view row vectors and column vectors as residing in diferent spaces; thus for instance we will not define the sum of a row vector with a column vector, even when they have the same number of elements. 

Definition 6.1.5 (Standard basis row vectors). We identify n special vectors in $\mathbf { R } ^ { n }$ , the standard basis row vectors $e _ { 1 } , \ldots , e _ { n }$ . For each $1 \leq$ $j \le n , e _ { j }$ is the vector which has 0 in all entries except for the $j ^ { t h }$ entry, which is equal to 1. 

For instance, in $\mathbf { R } ^ { 3 }$ , we have $e _ { 1 } = ( 1 , 0 , 0 ) , e _ { 2 } = ( 0 , 1 , 0 )$ , and $e _ { 3 } =$ $( 0 , 0 , 1 )$ . Note that if $x = ( x _ { j } ) _ { 1 \leq j \leq n }$ is a vector in $\mathbf { R } ^ { n }$ , then 

$$
x = x _ {1} e _ {1} + x _ {2} e _ {2} + \dots + x _ {n} e _ {n} = \sum_ {j = 1} ^ {n} x _ {j} e _ {j},
$$

or in other words every vector in $\mathbf { R } ^ { n }$ is a linear combination of the standard basis vectors $e _ { 1 } , \ldots , e _ { n }$ . (The notation $\scriptstyle \sum _ { j = 1 } ^ { n } x _ { j } e _ { j }$ is unambiguous because the operation of vector addition is both commutative and associative). Of course, just as every row vector is a linear combination of standard basis row vectors, every column vector is a linear combination of standard basis column vectors: 

$$
x ^ {T} = x _ {1} e _ {1} ^ {T} + x _ {2} e _ {2} ^ {T} + \ldots + x _ {n} e _ {n} ^ {T} = \sum_ {j = 1} ^ {n} x _ {j} e _ {j} ^ {T}.
$$

There are (many) other ways to create a basis for $\mathbf { R } ^ { n }$ , but this is a topic for a linear algebra text and will not be discussed here. 

Definition 6.1.6 (Linear transformations). A linear transformation $T$ : $\mathbf { R } ^ { n } \to \mathbf { R } ^ { m }$ is any function from one Euclidean space $\mathbf { R } ^ { n }$ to another $\mathbf { R } ^ { m }$ which obeys the following two axioms: 

(a) (Additivity) For every $x , x ^ { \prime } \in \mathbf { R } ^ { n }$ , we have $T ( x + x ^ { \prime } ) = T x + T x ^ { \prime } .$ 

(b) (Homogeneity) For every $x \in \mathbf { \Gamma } \mathbf { R } ^ { n }$ and every $c \in \textbf { R }$ , we have $T ( c x ) = c T x .$ 

Example 6.1.7. The dilation operator $T _ { 1 } : { \bf R } ^ { 3 }  { \bf R } ^ { 3 }$ defined by $T _ { 1 } x : = 5 x \ ( \mathrm { i . e . , i t }$ dilates each vector x by a factor of 5) is a linear transformation, since $5 ( x + x ^ { \prime } ) = 5 x + 5 x ^ { \prime }$ for all $x , x ^ { \prime } \in \mathbf { R } ^ { 3 }$ and $5 ( c x ) = c ( 5 x )$ for all $x \in \mathbf { R } ^ { 3 }$ and $c \in \mathbf { R }$ 

Example 6.1.8. The rotation operator $T _ { 2 } : { \bf R } ^ { 2 }  { \bf R } ^ { 2 }$ defined by a clockwise rotation by $\pi / 2$ radians around the origin (so that $T _ { 2 } ( 1 , 0 ) =$ $( 0 , 1 ) , T _ { 2 } ( 0 , 1 ) = ( - 1 , 0 )$ , etc.) is a linear transformation; this can best be seen geometrically rather than analytically. 

Example 6.1.9. The projection operator $T _ { 3 } : { \bf R } ^ { 3 }  { \bf R } ^ { 2 }$ defined by $T _ { 3 } ( x , y , z ) : = ( x , y )$ is a linear transformation (why?). The inclusion operator $T _ { 4 } : { \bf R } ^ { 2 }  { \bf R } ^ { 3 }$ defined by $T _ { 4 } ( x , y ) : = ( x , y , 0 )$ is also a linear transformation (why?). Finally, the identity operator $I _ { n } : \mathbf { R } ^ { n } \to \mathbf { R } ^ { n }$ , defined for any n by $I _ { n } x : = x$ is also a linear transformation (why?). 

As we shall shortly see, there is a connection between linear transformations and matrices. 

Definition 6.1.10 (Matrices). An $m \times n$ matrix is an object A of the form 

$$
A = \left( \begin{array}{c c c c} a _ {1 1} & a _ {1 2} & \ldots & a _ {1 n} \\ a _ {2 1} & a _ {2 2} & \ldots & a _ {2 n} \\ \vdots & \vdots & \ddots & \vdots \\ a _ {m 1} & a _ {m 2} & \ldots & a _ {m n} \end{array} \right);
$$

we shall abbreviate this as 

$$
A = (a _ {i j}) _ {1 \leq i \leq m; 1 \leq j \leq n}.
$$

In particular, n-dimensional row vectors are $1 \times n$ matrices, while $n -$ dimensional column vectors are $n \times 1$ matrices. 

Definition 6.1.11 (Matrix product). Given an $m \times n$ matrix A and an $n \times p$ matrix B, we can define the matrix product AB to be the $m \times p$ matrix defined as 

$$
(a _ {i j}) _ {1 \leq i \leq m; 1 \leq j \leq n} (b _ {j k}) _ {1 \leq j \leq n; 1 \leq k \leq p} := \left(\sum_ {j = 1} ^ {n} a _ {i j} b _ {j k}\right) _ {1 \leq i \leq m; 1 \leq k \leq p}.
$$

In particular, if $x ^ { T } = ( x _ { j } ) _ { 1 \leq j \leq n } ^ { T }$ is an n-dimensional column vector, and $A = ( a _ { i j } ) _ { 1 \leq i \leq m ; 1 \leq j \leq n }$ is an $m \times n$ matrix, then $A x ^ { T }$ is an m-dimensiona column vector: 

$$
A x ^ {T} = \left(\sum_ {j = 1} ^ {n} a _ {i j} x _ {j}\right) _ {1 \leq i \leq m} ^ {T}.
$$

We now relate matrices to linear transformations. If A is an $m \times n$ matrix, we can define the transformation $L _ { A } : \mathbf { R } ^ { n }  \mathbf { R } ^ { m }$ by the formula 

$$
(L _ {A} x) ^ {T} := A x ^ {T}.
$$

Example 6.1.12. If A is the matrix 

$$
A = \left( \begin{array}{c c c} 1 & 2 & 3 \\ 4 & 5 & 6 \end{array} \right),
$$

and $\boldsymbol { x } ~ = ~ \left( x _ { 1 } , x _ { 2 } , x _ { 3 } \right)$ is a 3-dimensional row vector, then $L _ { A } x$ is the 2-dimensional row vector defined by 

$$
(L _ {A} x) ^ {T} = \left( \begin{array}{c c c} 1 & 2 & 3 \\ 4 & 5 & 6 \end{array} \right) \left( \begin{array}{c} x _ {1} \\ x _ {2} \\ x _ {3} \end{array} \right) = \binom{x _ {1} + 2 x _ {2} + 3 x _ {3}}{4 x _ {1} + 5 x _ {2} + 6 x _ {3}}
$$

or in other words 

$$
L _ {A} (x _ {1}, x _ {2}, x _ {3}) = (x _ {1} + 2 x _ {2} + 3 x _ {3}, 4 x _ {1} + 5 x _ {2} + 6 x _ {3}).
$$

More generally, if 

$$
A = \left( \begin{array}{l l l l} a _ {1 1} & a _ {1 2} & \ldots & a _ {1 n} \\ a _ {2 1} & a _ {2 2} & \ldots & a _ {2 n} \\ \vdots & \vdots & \ddots & \vdots \\ a _ {m 1} & a _ {m 2} & \ldots & a _ {m n} \end{array} \right)
$$

then we have 

$$
L _ {A} (x _ {j}) _ {1 \leq j \leq n} = \left(\sum_ {j = 1} ^ {n} a _ {i j} x _ {j}\right) _ {1 \leq i \leq m}.
$$

For any $m \times n$ matrix $A _ { i }$ , the transformation $L _ { A }$ is automatically linear; one can easily verify that $L _ { A } ( x + y ) = L _ { A } x + L _ { A } y$ and $L _ { A } ( c x ) = c ( L _ { A } x )$ for any n-dimensional row vectors $x , y$ and any scalar c. (Why?) 

Perhaps surprisingly, the converse is also true, i.e., every linear transformation from $\mathbf { R } ^ { n }$ to $\mathbf { R } ^ { m }$ is given by a matrix: 

Lemma 6.1.13. Let $T : \mathbf { R } ^ { n }  \mathbf { R } ^ { m }$ be a linear transformation. Then there exists exactly one $m \times n$ matrix A such that $T = L _ { A }$ 

Proof. Suppose $T : \mathrm { ~ \bf ~ R } ^ { n } \to \mathrm { ~ \bf ~ R } ^ { m }$ is a linear transformation. Let $e _ { 1 } , e _ { 2 } , \ldots , e _ { n }$ be the standard basis row vectors of $\mathbf { R } ^ { n }$ Then $T e _ { 1 } , T e _ { 2 } , \ldots , T e _ { n }$ are vectors in $\mathbf { R } ^ { m }$ . For each $1 \leq j \leq n$ , we write $T e _ { j }$ in co-ordinates as 

$$
T e _ {j} = (a _ {1 j}, a _ {2 j}, \dots , a _ {m j}) = (a _ {i j}) _ {1 \leq i \leq m},
$$

i.e., we define $a _ { i j }$ to be the $i ^ { t h }$ component of $T e _ { j }$ . Then for any $n -$ dimensional row vector $x = ( x _ { 1 } , \ldots , x _ { n } )$ , we have 

$$
T x = T \left(\sum_ {j = 1} ^ {n} x _ {j} e _ {j}\right),
$$

which (since T is linear) is equal to 

$$
\begin{array}{l} = \sum_ {j = 1} ^ {n} T (x _ {j} e _ {j}) \\ = \sum_ {j = 1} ^ {n} x _ {j} T e _ {j} \\ = \sum_ {j = 1} ^ {n} x _ {j} (a _ {i j}) _ {1 \leq i \leq m} \\ = \sum_ {j = 1} ^ {n} (a _ {i j} x _ {j}) _ {1 \leq i \leq m} \\ = \left(\sum_ {j = 1} ^ {n} a _ {i j} x _ {j}\right) _ {1 \leq i \leq m}. \end{array}
$$

But if we let A be the matrix 

$$
A = \left( \begin{array}{c c c c} a _ {1 1} & a _ {1 2} & \ldots & a _ {1 n} \\ a _ {2 1} & a _ {2 2} & \ldots & a _ {2 n} \\ \vdots & \vdots & \ddots & \vdots \\ a _ {m 1} & a _ {m 2} & \ldots & a _ {m n} \end{array} \right)
$$

then the previous vector is precisely $L _ { A } x$ . Thus $T x = L _ { A } x$ for all $n -$ dimensional vectors x, and thus $T = L _ { A }$ 

Now we show that A is unique, i.e., there does not exist any other matrix 

$$
B = \left( \begin{array}{c c c c} b _ {1 1} & b _ {1 2} & \ldots & b _ {1 n} \\ b _ {2 1} & b _ {2 2} & \ldots & b _ {2 n} \\ \vdots & \vdots & \ddots & \vdots \\ b _ {m 1} & b _ {m 2} & \ldots & b _ {m n} \end{array} \right)
$$

for which T is equal to $L _ { B }$ . Suppose for sake of contradiction that we could find such a matrix B which was diferent from A. Then we would have $L _ { A } = L _ { B }$ . In particular, we have $L _ { A } e _ { j } = L _ { B } e _ { j }$ for every $1 \leq j \leq n$ But from the definition of $L _ { A }$ we see that 

$$
L _ {A} e _ {j} = (a _ {i j}) _ {1 \leq i \leq m}
$$

and 

$$
L _ {B} e _ {j} = (b _ {i j}) _ {1 \leq i \leq m}
$$

and thus we have $a _ { i j } = b _ { i j }$ for every $1 \leq i \leq m$ and $1 \leq j \leq m$ , thus A and B are equal, a contradiction. □ 

Remark 6.1.14. Lemma 6.1.13 establishes a one-to-one correspondence between linear transformations and matrices, and is one of the fundamental reasons why matrices are so important in linear algebra. One may ask then why we bother dealing with linear transformations at all, and why we don’t just work with matrices all the time. The reason is that sometimes one does not want to work with the standard basis $e _ { 1 } , \ldots , e _ { n }$ , but instead wants to use some other basis. In that case, the correspondence between linear transformations and matrices changes, and so it is still important to keep the notions of linear transformation and matrix distinct. More discussion on this somewhat subtle issue can be found in any linear algebra text. 

Remark 6.1.15. If $T = L _ { A }$ , then A is sometimes called the matrix representation of T, and is sometimes denoted $A = [ T ]$ . We shall avoid this notation here, however. 

The composition of two linear transformations is again a linear transformation (Exercise 6.1.2). The next lemma shows that the operation of composing linear transformations is connected to that of matrix multiplication. 

Lemma 6.1.16. Let A be an $m \times n$ matrix, and let B be an $n \times p$ matrix. Then $L _ { A } L _ { B } = L _ { A B }$ 

Proof. See Exercise 6.1.3. 

— Exercises — 

Exercise 6.1.1. Prove Lemma 6.1.2. 

Exercise 6.1.2. If $T : \mathbf { R } ^ { n }  \mathbf { R } ^ { m }$ is a linear transformation, and $S : \mathbf { R } ^ { p }  \mathbf { R } ^ { n }$ is a linear transformation, show that the composition $T S : \mathbf { R } ^ { p }  \mathbf { R } ^ { m }$ of the two transforms, defined by $T S ( x ) : = T ( S ( x ) )$ , is also a linear transformation. (Hint: expand $T S ( x + y )$ and TS(cx) carefully, using plenty of parentheses.) 

Exercise 6.1.3. Prove Lemma 6.1.16. 

Exercise 6.1.4. Let $T : \mathbf { R } ^ { n }  \mathbf { R } ^ { m }$ be a linear transformation. Show that there exists a number $M > 0$ such that $\| T x \| \leq M \| x \|$ for all $\boldsymbol { x } \in \mathbf { R } ^ { n }$ . (Hint: use Lemma 6.1.13 to write $T$ in terms of a matrix A, and then set M to be the sum of the absolute values of all the entries in A. Use the triangle inequality often - it’s easier than messing around with square roots etc.) Conclude in particular that every linear transformation from $\mathbf { R } ^ { n }$ to $\mathbf { R } ^ { m }$ is continuous. 

## 6.2 Derivatives in several variable calculus

Now that we’ve reviewed some linear algebra, we turn now to our main topic of this chapter, which is that of understanding diferentiation of functions of the form $f : \mathbf { R } ^ { n }  \mathbf { R } ^ { m } , { \mathrm { i . e . } }$ , functions from one Euclidean space to another. For instance, one might want to diferentiate the function $f : \mathbf { R } ^ { 3 } \to \mathbf { R } ^ { 4 }$ defined by 

$$
f (x, y, z) = (x y, y z, x z, x y z).
$$

In single variable calculus, when one wants to diferentiate a function $f : E  \mathbf { R }$ at a point $x _ { 0 }$ , where $E$ is a subset of R that contains $x _ { 0 }$ , this is given by 

$$
f ^ {\prime} (x _ {0}) := \lim _ {x \to x _ {0}; x \in E \setminus \{x _ {0} \}} \frac {f (x) - f (x _ {0})}{x - x _ {0}}.
$$

One could try to mimic this definition in the several variable case $f$ : $E  \mathbf { R } ^ { m }$ , where $E$ is now a subset of $\mathbf { R } ^ { n }$ , however we encounter a dificulty in this case: the quantity $f ( x ) - f ( x _ { 0 } )$ will live in $\mathbf { R } ^ { m }$ , and $x - x _ { 0 }$ lives in $\mathbf { R } ^ { n }$ , and we do not know how to divide an m-dimensional vector by an n-dimensional vector. 

To get around this problem, we first rewrite the concept of derivative (in one dimension) in a way which does not involve division of vectors. Instead, we view diferentiability at a point $x _ { 0 }$ as an assertion that a function f is “approximately linear” near $x _ { 0 }$ 

Lemma 6.2.1. Let E be a subset of R, $f : E  \mathbf { R }$ be a function, $x _ { 0 } \in E$ , and $L \in \mathbf { R }$ . Then the following two statements are equivalent. 

(a) $f$ is diferentiable at $x _ { 0 }$ , and $f ^ { \prime } ( x _ { 0 } ) = L$ 

$$
(b) \text {   We   have   } \lim _ {x \to x _ {0}; x \in E - \{x _ {0} \}} \frac {| f (x) - (f (x _ {0}) + L (x - x _ {0})) |}{| x - x _ {0} |} = 0.
$$

Proof. See Exercise 6.2.1. 

In light of the above lemma, we see that the derivative $f ^ { \prime } ( x _ { 0 } )$ can be interpreted as the number L for which $| f ( x ) - ( f ( x _ { 0 } ) + L ( x - x _ { 0 } ) ) |$ is small, in the sense that it tends to zero as x tends to $x _ { 0 }$ , even if we divide out by the very small number $\left| x - x _ { 0 } \right|$ . More informally, the derivative is the quantity $L$ such that we have the approximation $f ( x ) - f ( x _ { 0 } ) \approx L ( x - x _ { 0 } )$ 

This does not seem too diferent from the usual notion of diferentiation, but the point is that we are no longer explicitly dividing by $x - x _ { 0 }$ . (We are still dividing by $\left| x - x _ { 0 } \right|$ , but this will turn out to be OK). When we move to the several variable case $f : E \to \mathbf { R } ^ { m }$ , where $E \subseteq \mathbf { R } ^ { n }$ , we shall still want the derivative to be some quantity $L$ such that $f ( x ) - f ( x _ { 0 } ) \approx L ( x - x _ { 0 } )$ . However, since $f ( x ) - f ( x _ { 0 } )$ is now an m-dimensional vector and $x - x _ { 0 }$ is an n-dimensional vector, we no longer want $L$ to be a scalar; we want it to be a linear transformation. More precisely: 

Definition 6.2.2 (Diferentiability). Let $E$ be a subset of $\mathbf { R } ^ { n } , f : E $ $\mathbf { R } ^ { m }$ be a function, $x _ { 0 } \in E$ be a point, and let $L : \mathbf { R } ^ { n }  \mathbf { R } ^ { m }$ be a linear transformation. We say that $f$ is diferentiable at $x _ { 0 }$ with derivative $L$ if we have 

$$
\lim _ {x \to x _ {0}; x \in E - \{x _ {0} \}} \frac {\| f (x) - (f (x _ {0}) + L (x - x _ {0})) \|}{\| x - x _ {0} \|} = 0.
$$

Here $\lVert x \rVert$ is the length of $x$ (as measured in the $l ^ { 2 }$ metric): 

$$
\| (x _ {1}, x _ {2}, \ldots , x _ {n}) \| = (x _ {1} ^ {2} + x _ {2} ^ {2} + \ldots + x _ {n} ^ {2}) ^ {1 / 2}.
$$

Example 6.2.3. Let $f : { \bf R } ^ { 2 }  { \bf R } ^ { 2 }$ be the map $f ( x , y ) : = ( x ^ { 2 } , y ^ { 2 } )$ , let $x _ { 0 }$ be the point $x _ { 0 } : = ( 1 , 2 )$ , and let ${ \cal L } : { \bf R } ^ { 2 }  { \bf R } ^ { 2 }$ be the map $L ( x , y ) : =$ $( 2 x , 4 y )$ . We claim that $f$ is diferentiable at $x _ { 0 }$ with derivative L. To see this, we compute 

$$
\lim _ {(x, y) \to (1, 2): (x, y) \neq (1, 2)} \frac {\| f (x , y) - (f (1 , 2) + L ((x , y) - (1 , 2))) \|}{\| (x , y) - (1 , 2) \|}.
$$

Making the change of variables $( x , y ) = ( 1 , 2 ) + ( a , b )$ , this becomes 

$$
\lim _ {(a, b) \to (0, 0): (a, b) \neq (0, 0)} \frac {\| f (1 + a , 2 + b) - (f (1 , 2) + L (a , b)) \|}{\| (a , b) \|}.
$$

Substituting the formula for $f$ and for $L$ , this becomes 

$$
\lim _ {(a, b) \to (0, 0): (a, b) \neq (0, 0)} \frac {\| ((1 + a) ^ {2} , (2 + b) ^ {2}) - (1 , 4) - (2 a , 4 b)) \|}{\| (a , b) \|},
$$

which simplifies to 

$$
\lim _ {(a, b) \to (0, 0): (a, b) \neq (0, 0)} \frac {\| (a ^ {2} , b ^ {2}) \|}{\| (a , b) \|}.
$$

We use the squeeze test. The expression $\frac { \| ( a ^ { 2 } , b ^ { 2 } ) \| } { \| ( a , b ) \| }$ is clearly non-negative. On the other hand, we have by the triangle inequality 

$$
\| (a ^ {2}, b ^ {2}) \| \leq \| (a ^ {2}, 0) \| + \| (0, b ^ {2}) \| = a ^ {2} + b ^ {2}
$$

and hence 

$$
\frac {\| (a ^ {2} , b ^ {2}) \|}{\| (a , b) \|} \leq \sqrt {a ^ {2} + b ^ {2}}.
$$

Since ${ \sqrt { a ^ { 2 } + b ^ { 2 } } } \to 0$ as $( a , b ) \to 0$ , we thus see from the squeeze test that the above limit exists and is equal to 0. Thus f is diferentiable at $x _ { 0 }$ with derivative $L$ 

As you can see, verifying that a function is diferentiable from first principles can be somewhat tedious. Later on we shall find better ways to verify diferentiability, and to compute derivatives. 

Before we proceed further, we have to check a basic fact, which is that a function can have at most one derivative at any interior point of its domain: 

Lemma 6.2.4 (Uniqueness of derivatives). Let E be a subset of $\mathbf { R } ^ { n }$ $f : E \to \mathbf { R } ^ { m }$ be a function, $x _ { 0 } \in E$ be an interior point of $E _ { i }$ , and let $L _ { 1 } : \mathbf { R } ^ { n }  \mathbf { R } ^ { m }$ and $L _ { 2 } : \mathbf { R } ^ { n }  \mathbf { R } ^ { m }$ be linear transformations. Suppose that f is diferentiable at $x _ { 0 }$ with derivative $L _ { 1 }$ , and also diferentiable at $x _ { 0 }$ with derivative $L _ { 2 }$ . Then $L _ { 1 } = L _ { 2 }$ 

Proof. See Exercise 6.2.2. 

Because of Lemma 6.2.4, we can now talk about the derivative of f at interior points $x _ { 0 }$ , and we will denote this derivative by $f ^ { \prime } ( x _ { 0 } )$ . Thus $f ^ { \prime } ( x _ { 0 } )$ is the unique linear transformation from $\mathbf { R } ^ { n }$ to $\mathbf { R } ^ { m }$ such that 

$$
\lim _ {x \to x _ {0}; x \neq x _ {0}} \frac {\| f (x) - (f (x _ {0}) + f ^ {\prime} (x _ {0}) (x - x _ {0})) \|}{\| x - x _ {0} \|} = 0.
$$

Informally, this means that the derivative $f ^ { \prime } ( x _ { 0 } )$ is the linear transformation such that we have 

$$
f (x) - f (x _ {0}) \approx f ^ {\prime} (x _ {0}) (x - x _ {0})
$$

or equivalently 

$$
f (x) \approx f (x _ {0}) + f ^ {\prime} (x _ {0}) (x - x _ {0})
$$

(this is known as Newton’s approximation; compare with Proposition 10.1.7). 

Another consequence of Lemma 6.2.4 is that if you know that $f ( x ) =$ $g ( x )$ for all $x \in E$ , and $f , g$ are diferentiable at $x _ { 0 }$ , then you also know that $f ^ { \prime } ( x _ { 0 } ) = g ^ { \prime } ( x _ { 0 } )$ at every interior point of $E$ . However, this is not necessarily true if $x _ { 0 }$ is a boundary point of $E ;$ for instance, if $E$ is just a single point $E = \{ x _ { 0 } \}$ , merely knowing that $f ( x _ { 0 } ) = g ( x _ { 0 } )$ does not imply that $f ^ { \prime } ( x _ { 0 } ) = g ^ { \prime } ( x _ { 0 } )$ . We will not deal with these boundary issues here, and only compute derivatives on the interior of the domain. 

We will sometimes refer to $f ^ { \prime }$ as the total derivative of $f ,$ to distinguish this concept from that of partial and directional derivatives below. The total derivative $f$ is also closely related to the derivative matrix $D f$ , which we shall define in the next section. 

$$
- \text { Exercises } -
$$

Exercise 6.2.1. Prove Lemma 6.2.1. 

Exercise 6.2.2. Prove Lemma 6.2.4. (Hint: prove by contradiction. If $L _ { 1 } \neq L _ { 2 }$ then there exists a vector v such that $L _ { 1 } v \neq L _ { 2 } v ;$ ; this vector must be non-zero (why?). Now apply the definition of derivative, and try to specialize to the case where $x = x _ { 0 } + t v$ for some scalar t, to obtain a contradiction.) 

## 6.3 Partial and directional derivatives

We now connect the notion of diferentiability with that of partial and directional derivatives, which we now introduce. 

Definition 6.3.1 (Directional derivative). Let $E$ be a subset of $\mathbf { R } ^ { n }$ $f : E  \mathbf { R } ^ { m }$ be a function, let $x _ { 0 }$ be an interior point of $E _ { i }$ , and let $v$ be a vector in $\mathbf { R } ^ { n }$ . If the limit 

$$
\lim _ {t \to 0; t > 0, x _ {0} + t v \in E} \frac {f (x _ {0} + t v) - f (x _ {0})}{t}
$$

exists, we say that $f$ is diferentiable in the direction v at $x _ { 0 }$ , and we denote the above limit by $D _ { v } f ( x _ { 0 } )$ : 

$$
D _ {v} f (x _ {0}) := \lim _ {t \to 0; t > 0} \frac {f (x _ {0} + t v) - f (x _ {0})}{t}.
$$

Remark 6.3.2. One should compare this definition with Definition 6.2.2. Note that we are dividing by a scalar $t ,$ rather than a vector, so this definition makes sense, and $D _ { v } f ( x _ { 0 } )$ will be a vector in $\mathbf { R } ^ { m }$ . It is sometimes possible to also define directional derivatives on the boundary of $E$ , if the vector v is pointing in an “inward” direction (this generalizes the notion of left derivatives and right derivatives from single variable calculus); but we will not pursue these matters here. 

Example 6.3.3. If $f : \mathbf { R }  \mathbf { R }$ is a function, then $D _ { + 1 } f ( x )$ is the same as the right derivative of $f ( x )$ (if it exists), and similarly $D _ { - 1 } f ( x )$ is the same as the left derivative of $f ( x )$ (if it exists). 

Example 6.3.4. We use the function $f : \mathbf { R } ^ { 2 }  \mathbf { R } ^ { 2 }$ defined by $f ( x , y ) : =$ $( x ^ { 2 } , y ^ { 2 } )$ from before, and let $x _ { 0 } : = ( 1 , 2 )$ and $v : = ( 3 , 4 )$ . Then 

$$
\begin{array}{c} D _ {v} f (x _ {0}) = \lim _ {t \to 0; t > 0} \frac {f (1 + 3 t , 2 + 4 t) - f (1 , 2)}{t} \\ = \lim _ {t \to 0; t > 0} \frac {(1 + 6 t + 9 t ^ {2} , 4 + 1 6 t + 1 6 t ^ {2}) - (1 , 4)}{t} \\ = \lim _ {t \to 0; t > 0} (6 + 9 t, 1 6 + 1 6 t) = (6, 1 6). \end{array}
$$

Directional derivatives are connected with total derivatives as follows: 

Lemma 6.3.5. Let E be a subset of $\mathbf { R } ^ { n } , \ f : E \to \mathbf { R } ^ { m }$ be a function, $x _ { 0 }$ be an interior point of $E _ { i }$ , and let v be a vector in $\mathbf { R } ^ { n }$ . If f is diferentiable at $x _ { 0 }$ , then f is also diferentiable in the direction v at $x _ { 0 }$ , and 

$$
D _ {v} f (x _ {0}) = f ^ {\prime} (x _ {0}) v.
$$

Proof. See Exercise 6.3.1. 

Remark 6.3.6. One consequence of this lemma is that total diferentiability implies directional diferentiability. However, the converse is not true; see Exercise 6.3.3. 

Closely related to the concept of directional derivative is that of partial derivative: 

Definition 6.3.7 (Partial derivative). Let E be a subset of $\mathbf { R } ^ { n }$ , let $f : E \to \mathbf { R } ^ { m }$ be a function, let $x _ { 0 }$ be an interior point of $E ,$ and let $1 \ \leq \ j \ \leq \ n$ . Then the partial derivative of f with respect to the $x _ { j }$ variable at $x _ { 0 }$ , denoted $\textstyle { \frac { \partial f } { \partial x _ { j } } } ( x _ { 0 } )$ , is defined by 

$$
\frac {\partial f}{\partial x _ {j}} (x _ {0}) := \lim _ {t \to 0; t \neq 0, x _ {0} + t e _ {j} \in E} \frac {f (x _ {0} + t e _ {j}) - f (x _ {0})}{t} = \frac {d}{d t} f (x _ {0} + t e _ {j}) | _ {t = 0}
$$

provided of course that the limit exists. (If the limit does not exist, we leave $\textstyle { \frac { \partial f } { \partial x _ { j } } } ( x _ { 0 } )$ undefined). 

Informally, the partial derivative can be obtained by holding all the variables other than $x _ { j }$ fixed, and then applying the single-variable calculus derivative in the $x _ { j }$ variable. Note that if $f$ takes values in $\mathbf { R } ^ { m }$ then so will $\frac { \partial f } { \partial x _ { j } }$ . Indeed, if we write f in components as $f = ( f _ { 1 } , \ldots , f _ { m } )$ it is easy to see (why?) that 

$$
\frac {\partial f}{\partial x _ {j}} (x _ {0}) = \left(\frac {\partial f _ {1}}{\partial x _ {j}} (x _ {0}), \ldots , \frac {\partial f _ {m}}{\partial x _ {j}} (x _ {0})\right),
$$

i.e., to diferentiate a vector-valued function one just has to diferentiate each of the components separately. 

We sometimes replace the variables $x _ { j }$ in $\frac { \partial f } { \partial x _ { j } }$ with other symbols. For instance, if we are dealing with the function $\dot { f } ( x , y ) = ( x ^ { 2 } , y ^ { 2 } )$ , then we might refer to $\textstyle { \frac { \partial f } { \partial x } }$ and $\frac { \partial \stackrel { \triangledown } { f } } { \partial y }$ instead of $\frac { \partial f } { \partial x _ { 1 } }$ and $\frac { \partial f } { \partial x _ { 2 } }$ . (In this case, $\begin{array} { r } { \frac { \partial f } { \partial x } ( x , y ) = ( 2 x , 0 ) } \end{array}$ and $\begin{array} { r } { \frac { \partial f } { \partial y } ( x , \dot { y } ) = ( 0 , 2 y ) ) } \end{array}$ . One should caution however that one should only relabel the variables if it is absolutely clear which symbol refers to the first variable, which symbol refers to the second variable, etc.; otherwise one may become unintentionally confused. For instance, in the above example, the expression $\textstyle { \frac { \partial f } { \partial x } } ( x , x )$ is just $( 2 x , 0 )$ 1 however one may mistakenly compute 

$$
\frac {\partial f}{\partial x} (x, x) = \frac {\partial}{\partial x} (x ^ {2}, x ^ {2}) = (2 x, 2 x);
$$

the problem here is that the symbol $x$ is being used for more than just the first variable of $f .$ . On the other hand, it is true that ${ \frac { d } { d x } } f ( x , x )$ is equal to $( 2 x , 2 x )$ ; thus the operation of total diferentiation $\textstyle { \frac { d } { d x } }$ is not the same as that of partial diferentiation $\textstyle { \frac { \partial } { \partial x } } )$ 

From Lemma 6.3.5, we know that if a function is diferentiable at a point $x _ { 0 }$ , then all the partial derivatives $\frac { \partial f } { \partial x _ { j } }$ exist at $x _ { 0 }$ , and that 

$$
\frac {\partial f}{\partial x _ {j}} (x _ {0}) = f ^ {\prime} (x _ {0}) e _ {j}.
$$

Also, if $\begin{array} { r } { v = ( v _ { 1 } , . . . , v _ { n } ) = \sum _ { j } v _ { j } e _ { j } } \end{array}$ , then we have 

$$
D _ {v} f (x _ {0}) = f ^ {\prime} (x _ {0}) \sum_ {j} v _ {j} e _ {j} = \sum_ {j} v _ {j} f ^ {\prime} (x _ {0}) e _ {j}
$$

(since $f ^ { \prime } ( x _ { 0 } )$ is linear) and thus 

$$
D _ {v} f (x _ {0}) = \sum_ {j} v _ {j} \frac {\partial f}{\partial x _ {j}} (x _ {0}).
$$

Thus one can write directional derivatives in terms of partial derivatives, provided that the function is actually diferentiable at that point. 

Just because the partial derivatives exist at a point $x _ { 0 }$ , we cannot conclude that the function is diferentiable there (Exercise 6.3.3). However, if we know that the partial derivatives not only exist, but are continuous, then we can in fact conclude diferentiability, thanks to the following handy theorem: 

Theorem 6.3.8. Let E be a subset of $\mathbf { R } ^ { n } , f : E  \mathbf { R } ^ { m }$ be a function, F be a subset of E, and $x _ { 0 }$ be an interior point of F. If all the partial derivatives $\frac { \partial f } { \partial x _ { j } }$ exist on $F$ and are continuous at $x _ { 0 }$ , then f is diferentiable at $x _ { 0 }$ , and the linear transformation $f ^ { \prime } ( x _ { 0 } ) : \mathbf { R } ^ { n }  \mathbf { R } ^ { m }$ is defined by 

$$
f ^ {\prime} (x _ {0}) (v _ {j}) _ {1 \leq j \leq n} = \sum_ {j = 1} ^ {n} v _ {j} \frac {\partial f}{\partial x _ {j}} (x _ {0}).
$$

Proof. Let $L : \mathbf { R } ^ { n }  \mathbf { R } ^ { m }$ be the linear transformation 

$$
L (v _ {j}) _ {1 \leq j \leq m} := \sum_ {j = 1} ^ {m} v _ {j} \frac {\partial f}{\partial x _ {j}} (x _ {0}).
$$

We have to prove that 

$$
\lim _ {x \to x _ {0}; x \in E - \{x _ {0} \}} \frac {\| f (x) - (f (x _ {0}) + L (x - x _ {0})) \|}{\| x - x _ {0} \|} = 0.
$$

Let $\varepsilon > 0$ . It will sufice to find a radius $\delta > 0$ such that 

$$
\frac {\| f (x) - \left(f \left(x _ {0}\right) + L \left(x - x _ {0}\right)\right) \|}{\| x - x _ {0} \|} \leq \varepsilon
$$

for all $x \in B ( x _ { 0 } , \delta ) \backslash \{ x _ { 0 } \}$ . Equivalently, we wish to show that 

$$
\| f (x) - f (x _ {0}) - L (x - x _ {0}) \| \leq \varepsilon \| x - x _ {0} \|
$$

for all $x \in B ( x _ { 0 } , \delta ) \backslash \{ x _ { 0 } \}$ 

Because $x _ { 0 }$ is an interior point of $F _ { \mathrm { { ; } } }$ , there exists a ball $B ( x _ { 0 } , r )$ which is contained inside F. Because each partial derivative $\frac { \partial f } { \partial x _ { i } }$ is continuous on $F$ , there thus exists an $0 < \delta _ { j } < r$ such that $\begin{array} { r } { \| \frac { \partial f } { \partial x _ { i } } ( x ) - \frac { \partial f } { \partial x _ { i } } ( x _ { 0 } ) \| \leq } \end{array}$ $\varepsilon / n m$ for every $x \in B ( x _ { 0 } , \delta _ { j } )$ . If we take $\delta = \operatorname* { m i n } ( \delta _ { 1 } , \dots , \delta _ { n } )$ , then we thus have $\begin{array} { r } { \| \frac { \partial f } { \partial x _ { j } } ( x ) - \frac { \partial \dot { f } } { \partial x _ { j } } ( x _ { 0 } ) \| \le \varepsilon / n m } \end{array}$ for every $x \in B ( x _ { 0 } , \delta )$ and every $1 \leq j \leq n$ 

Let $x \in B ( x _ { 0 } , \delta )$ . We write $x = x _ { 0 } + v _ { 1 } e _ { 1 } + v _ { 2 } e _ { 2 } + . . . + v _ { n } e _ { n }$ for some scalars $v _ { 1 } , \ldots , v _ { n }$ . Note that 

$$
\| x - x _ {0} \| = \sqrt {v _ {1} ^ {2} + v _ {2} ^ {2} + \ldots + v _ {n} ^ {2}}
$$

and in particular we have $| v _ { j } | \leq \| x - x _ { 0 } \|$ for all $1 \leq j \leq n$ . Our task is to show that 

$$
\left\| f (x _ {0} + v _ {1} e _ {1} + \dots + v _ {n} e _ {n}) - f (x _ {0}) - \sum_ {j = 1} ^ {n} v _ {j} \frac {\partial f}{\partial x _ {j}} (x _ {0}) \right\| \leq \varepsilon \| x - x _ {0} \|.
$$

Write f in components as ${ \boldsymbol { f } } = \left( f _ { 1 } , f _ { 2 } , \ldots , f _ { m } \right)$ (so each $f _ { i }$ is a function from E to $\mathbf { R } )$ . From the mean value theorem in the $x _ { 1 }$ variable, we see that 

$$
f _ {i} (x _ {0} + v _ {1} e _ {1}) - f _ {i} (x _ {0}) = \frac {\partial f _ {i}}{\partial x _ {1}} (x _ {0} + t _ {i} e _ {1}) v _ {1}
$$

for some $t _ { i }$ between 0 and $v _ { 1 }$ . But we have 

$$
\left| \frac {\partial f _ {i}}{\partial x _ {j}} (x _ {0} + t _ {i} e _ {1}) - \frac {\partial f _ {i}}{\partial x _ {j}} (x _ {0}) \right| \leq \left\| \frac {\partial f}{\partial x _ {j}} (x _ {0} + t _ {i} e _ {1}) - \frac {\partial f}{\partial x _ {j}} (x _ {0}) \right\| \leq \varepsilon / n m
$$

and hence 

$$
\left| f _ {i} (x _ {0} + v _ {1} e _ {1}) - f _ {i} (x _ {0}) - \frac {\partial f _ {i}}{\partial x _ {1}} (x _ {0}) v _ {1} \right| \leq \varepsilon | v _ {1} | / n m.
$$

Summing this over all $1 \leq i \leq m$ (and noting that $\| ( y _ { 1 } , \ldots , y _ { m } ) \| \le$ $| y _ { 1 } | + . . . + | y _ { m } |$ from the triangle inequality) we obtain 

$$
\left\| f (x _ {0} + v _ {1} e _ {1}) - f (x _ {0}) - \frac {\partial f}{\partial x _ {1}} (x _ {0}) v _ {1} \right\| \leq \varepsilon | v _ {1} | / n;
$$

since $\left| v _ { 1 } \right| \leq \left. x - x _ { 0 } \right.$ , we thus have 

$$
\left\| f \left(x _ {0} + v _ {1} e _ {1}\right) - f \left(x _ {0}\right) - \frac {\partial f}{\partial x _ {1}} \left(x _ {0}\right) v _ {1} \right\| \leq \varepsilon \| x - x _ {0} \| / n.
$$

A similar argument gives 

$$
\left\| f \left(x _ {0} + v _ {1} e _ {1} + v _ {2} e _ {2}\right) - f \left(x _ {0} + v _ {1} e _ {1}\right) - \frac {\partial f}{\partial x _ {2}} \left(x _ {0}\right) v _ {2} \right\| \leq \varepsilon \| x - x _ {0} \| / n.
$$

and so forth up to 

$$
\begin{array}{c} \Big \| f (x _ {0} + v _ {1} e _ {1} + \ldots + v _ {n} e _ {n}) - f (x _ {0} + v _ {1} e _ {1} + \ldots + v _ {n - 1} e _ {n - 1}) \\ - \frac {\partial f}{\partial x _ {n}} (x _ {0}) v _ {n} \Big \| \leq \varepsilon \| x - x _ {0} \| / n. \end{array}
$$

If we sum these n inequalities and use the triangle inequality $\| x + y \| \leq$ $\| x \| + \| y \|$ , we obtain a telescoping series which simplifies to 

$$
\left\| f (x _ {0} + v _ {1} e _ {1} + \ldots + v _ {n} e _ {n}) - f (x _ {0}) - \sum_ {j = 1} ^ {n} \frac {\partial f}{\partial x _ {j}} (x _ {0}) v _ {j} \right\| \leq \varepsilon \| x - x _ {0} \|
$$

as desired. 

□ 

From Theorem 6.3.8 and Lemma 6.3.5 we see that if the partial derivatives of a function $f : E  \mathbf { R } ^ { m }$ exist and are continuous on some set $F _ { ; }$ then all the directional derivatives also exist at every interior point $x _ { 0 }$ of $F$ , and we have the formula 

$$
D _ {(v _ {1}, \dots , v _ {n})} f (x _ {0}) = \sum_ {j = 1} ^ {n} v _ {j} \frac {\partial f}{\partial x _ {j}} (x _ {0}).
$$

In particular, if $f : E  \mathbf { R }$ is a real-valued function, and we define the gradient $\nabla f ( x _ { 0 } )$ of $f$ at $x _ { 0 }$ to be the n-dimensional row vector $\begin{array} { r } { \nabla f ( \bar { x } _ { 0 } ) : = ( \frac { \partial f } { \partial x _ { 1 } } ( x _ { 0 } ) , \dots , \frac { \partial f } { \partial x _ { n } } ( x _ { 0 } ) ) } \end{array}$ , then we have the familiar formula 

$$
D _ {v} f (x _ {0}) = v \cdot \nabla f (x _ {0})
$$

whenever $x _ { 0 }$ is in the interior of the region where the gradient exists and is continuous. 

More generally, if $f : E \to \mathbf { R } ^ { m }$ is a function taking values in $\mathbf { R } ^ { m }$ with $f = ( f _ { 1 } , \ldots , f _ { m } )$ , and $x _ { 0 }$ is in the interior of the region where the partial derivatives of $f$ exist and are continuous, then we have from Theorem 6.3.8 that 

$$
\begin{array}{l} f ^ {\prime} (x _ {0}) (v _ {j}) _ {1 \leq j \leq n} = \sum_ {j = 1} ^ {n} v _ {j} \frac {\partial f}{\partial x _ {j}} (x _ {0}) \\ = \left(\sum_ {j = 1} ^ {n} v _ {j} \frac {\partial f _ {i}}{\partial x _ {j}} (x _ {0})\right) _ {i = 1} ^ {m}, \end{array}
$$

which we can rewrite as 

$$
L _ {D f (x _ {0})} (v _ {j}) _ {1 \leq j \leq n}
$$

where $D f ( x _ { 0 } )$ is the $m \times n$ matrix 

$$
\begin{array}{c} D f (x _ {0}) := \left(\frac {\partial f _ {i}}{\partial x _ {j}} (x _ {0})\right) _ {1 \leq i \leq m; 1 \leq j \leq n} \\ = \left( \begin{array}{c c c c} \frac {\partial f _ {1}}{\partial x _ {1}} (x _ {0}) & \frac {\partial f _ {1}}{\partial x _ {2}} (x _ {0}) & \ldots & \frac {\partial f _ {1}}{\partial x _ {n}} (x _ {0}) \\ \frac {\partial f _ {2}}{\partial x _ {1}} (x _ {0}) & \frac {\partial f _ {2}}{\partial x _ {2}} (x _ {0}) & \ldots & \frac {\partial f _ {2}}{\partial x _ {n}} (x _ {0}) \\ \vdots & \vdots & \ddots & \vdots \\ \frac {\partial f _ {m}}{\partial x _ {1}} (x _ {0}) & \frac {\partial f _ {m}}{\partial x _ {2}} (x _ {0}) & \ldots & \frac {\partial f _ {m}}{\partial x _ {n}} (x _ {0}) \end{array} \right). \end{array}
$$

Thus we have 

$$
(D _ {v} f (x _ {0})) ^ {T} = (f ^ {\prime} (x _ {0}) v) ^ {T} = D f (x _ {0}) v ^ {T}.
$$

The matrix $D f ( x _ { 0 } )$ is sometimes also called the derivative matrix or diferential matrix of $f$ at $x _ { 0 }$ , and is closely related to the total derivative $f ^ { \prime } ( x _ { 0 } )$ . One can also write $D f$ as 

$$
D f (x _ {0}) = \left(\frac {\partial f}{\partial x _ {1}} (x _ {0}) ^ {T}, \frac {\partial f}{\partial x _ {2}} (x _ {0}) ^ {T}, \dots , \frac {\partial f}{\partial x _ {n}} (x _ {0}) ^ {T}\right),
$$

i.e., each of the columns of $D f ( x _ { 0 } )$ is one of the partial derivatives of $f$ expressed as a column vector. Or one could write 

$$
D f (x _ {0}) = \left( \begin{array}{l} \nabla f _ {1} (x _ {0}) \\ \nabla f _ {2} (x _ {0}) \\ \vdots \\ \nabla f _ {m} (x _ {0}) \end{array} \right)
$$

i.e., the rows of $D f ( x _ { 0 } )$ are the gradient of various components of $f .$ . In particular, if f is scalar-valued $( \mathrm { i . e . , } m = 1 )$ , then $D f$ is the same as $\nabla f$ 

Example 6.3.9. Let $f : { \bf R } ^ { 2 }  { \bf R } ^ { 2 }$ be the function $f ( x , y ) = ( x ^ { 2 } +$ $x y , y ^ { 2 } )$ . Then $\begin{array} { r } { \frac { \partial f } { \partial \boldsymbol { x } } = ( 2 \boldsymbol { x } + \boldsymbol { y } , 0 ) } \end{array}$ and $\begin{array} { r } { \frac { \partial f } { \partial y } = ( x , 2 y ) } \end{array}$ . Since these partia derivatives are continuous on $\mathbf { R } ^ { 2 }$ , we see that $f$ is diferentiable on all of $\mathbf { R } ^ { 2 }$ , and 

$$
D f (x, y) = \left( \begin{array}{c c} 2 x + y & x \\ 0 & 2 y \end{array} \right).
$$

Thus for instance, the directional derivative in the direction $( v , w )$ is 

$$
D _ {(v, w)} f (x, y) = ((2 x + y) v + x w, 2 y w).
$$

— Exercises — 

Exercise 6.3.1. Prove Lemma 6.3.5. (This will be similar to Exercise 6.2.1). 

Exercise 6.3.2. Let E be a subset of $\mathbf { R } ^ { n }$ , let $f : E \to \mathbf { R } ^ { m }$ be a function, let $x _ { 0 }$ be an interior point of E, and let $1 \leq j \leq n .$ . Show that $\textstyle { \frac { \partial f } { \partial x _ { j } } } ( x _ { 0 } )$ exists if and only if $D _ { e _ { j } } f ( x _ { 0 } )$ and $D _ { - e _ { j } } f ( x _ { 0 } )$ exist and are negatives of each other (thus $D _ { e _ { j } } f ( x _ { 0 } ) = D _ { - e _ { j } } f ( x _ { 0 } ) )$ ; furthermore, one has $\begin{array} { r } { \frac { \partial f } { \partial \boldsymbol { x } _ { j } } ( \boldsymbol { x } _ { 0 } ) = D _ { \boldsymbol { e } _ { j } } f ( \boldsymbol { x } _ { 0 } ) } \end{array}$ in this case. 

Exercise 6.3.3. Let $f : { \bf R } ^ { 2 }  { \bf R }$ be the function defined by $\textstyle f ( x , y ) : = { \frac { x ^ { 3 } } { x ^ { 2 } + y ^ { 2 } } }$ when $( x , y ) \neq ( 0 , 0 )$ , and $f ( 0 , 0 ) : = 0$ . Show that f is not diferentiable at $( 0 , 0 )$ , despite being diferentiable in every direction $v \in { \mathbf { R } } ^ { 2 }$ at $( 0 , 0 )$ . Explain why this does not contradict Theorem 6.3.8. 

Exercise 6.3.4. Let $f : \mathbf { R } ^ { n }  \mathbf { R } ^ { m }$ be a diferentiable function such that $f ^ { \prime } ( x ) =$ 0 for all $\boldsymbol { x } \in \mathbf { R } ^ { n }$ . Show that f is constant. (Hint: you may use the mean-value theorem or fundamental theorem of calculus for one-dimensional functions, but bear in mind that there is no direct analogue of these theorems for severalvariable functions. I would not advise proceeding via first principles.) For a tougher challenge, replace the domain $\mathbf { R } ^ { n }$ by an open connected subset Ω of $\mathbf { R } ^ { n }$ 

## 6.4 The several variable calculus chain rule

We are now ready to state the several variable calculus chain rule. Recall that if $f : X \to Y$ and $g : Y  Z$ are two functions, then the composition $g \circ f : X \to Z$ is defined by $g \circ f ( x ) : = g ( f ( x ) )$ for all $x \in X$ 

Theorem 6.4.1 (Several variable calculus chain rule). Let E be a subset $o f \mathbf { R } ^ { n }$ , and let F be a subset of $\mathbf { R } ^ { m }$ . Let $f : E \to F$ be a function, and let $g : F \to \mathbf { R } ^ { p }$ be another function. Let x be a point in the interior of E. Suppose that f is diferentiable at $x _ { 0 }$ , and that $f ( x _ { 0 } )$ is in the interior of F. Suppose also that g is diferentiable at $f ( x _ { 0 } )$ . Then $g \circ f : E \to \mathbf { R } ^ { p }$ is also diferentiable at $x _ { 0 }$ , and we have the formula 

$$
(g \circ f) ^ {\prime} (x _ {0}) = g ^ {\prime} (f (x _ {0})) f ^ {\prime} (x _ {0}).
$$

Proof. See Exercise 6.4.3. 

One should compare this theorem with the single-variable chain rule, Theorem 10.1.15; indeed one can easily deduce the single-variable rule as a consequence of the several-variable rule. 

Intuitively, one can think of the several variable chain rule as follows. Let x be close to $x _ { 0 }$ . Then Newton’s approximation asserts that 

$$
f (x) - f (x _ {0}) \approx f ^ {\prime} (x _ {0}) (x - x _ {0})
$$

and in particular $f ( x )$ is close to $f ( x _ { 0 } )$ . Since g is diferentiable at $f ( x _ { 0 } )$ 1 we see from Newton’s approximation again that 

$$
g (f (x)) - g (f (x _ {0})) \approx g ^ {\prime} (f (x _ {0})) (f (x) - f (x _ {0})).
$$

Combining the two, we obtain 

$$
g \circ f (x) - g \circ f (x _ {0}) \approx g ^ {\prime} (f (x _ {0})) f ^ {\prime} (x _ {0}) (x - x _ {0})
$$

which then should give $( g \circ f ) ^ { \prime } ( x _ { 0 } ) = g ^ { \prime } ( f ( x _ { 0 } ) ) f ^ { \prime } ( x _ { 0 } )$ . This argument however is rather imprecise; to make it more precise one needs to manipulate limits rigorously; see Exercise 6.4.3. 

As a corollary of the chain rule and Lemma 6.1.16 (and Lemma 6.1.13), we see that 

$$
D (g \circ f) (x _ {0}) = D g (f (x _ {0})) D f (x _ {0});
$$

i.e., we can write the chain rule in terms of matrices and matrix multiplication, instead of in terms of linear transformations and composition. 

Example 6.4.2. Let $f : \mathbf { R } ^ { n }  \mathbf { R }$ and $g : \mathbf { R } ^ { n }  \mathbf { R }$ be diferentiable functions. We form the combined function $h : \mathbf { R } ^ { n }  \mathbf { R } ^ { 2 }$ by defining $h ( x ) : = ( f ( x ) , g ( x ) )$ . Now let $k : \mathbf { R } ^ { 2 }  \mathbf { R }$ be the multiplication function $k ( a , b ) : = a b$ . Note that 

$$
D h (x _ {0}) = \binom{\nabla f (x _ {0})}{\nabla g (x _ {0})}
$$

while 

$$
D k (a, b) = (b, a)
$$

(why?). By the chain rule, we thus see that 

$$
D (k \circ h) (x _ {0}) = (g (x _ {0}), f (x _ {0})) \binom{\nabla f (x _ {0})}{\nabla g (x _ {0})} = g (x _ {0}) \nabla f (x _ {0}) + f (x _ {0}) \nabla g (x _ {0}).
$$

But $k \circ h = f g \ \mathrm { ( w h y ? ) }$ , and $D ( f g ) = \nabla ( f g )$ . We have thus proven the product rule 

$$
\nabla (f g) = g \nabla f + f \nabla g.
$$

A similar argument gives the sum rule $\nabla ( f + g ) = \nabla f + \nabla g$ , or the diference rule $\nabla ( f - g ) = \nabla f - \nabla g$ , as well as the quotient rule (Exercise 6.4.4). As you can see, the several variable chain rule is quite powerful, and can be used to deduce many other rules of diferentiation. 

We do record one further useful application of the chain rule. Let $T : \mathbf { R } ^ { n }  \mathbf { R } ^ { m }$ be a linear transformation. From Exercise 6.4.1 we observe that $T$ is continuously diferentiable at every point, and in fact $T ^ { \prime } ( x ) = T$ for every $x .$ (This equation may look a little strange, but perhaps it is easier to swallow if you view it in the form $\begin{array} { r } { \frac { d } { d x } ( T x ) = T ) } \end{array}$ Thus, for any diferentiable function $f : E \to \mathbf { R } ^ { n }$ , we see that $T f : E \to$ $\mathbf { R } ^ { m }$ is also diferentiable, and hence by the chain rule 

$$
(T f) ^ {\prime} (x _ {0}) = T (f ^ {\prime} (x _ {0})).
$$

This is a generalization of the single-variable calculus rule $( c f ) ^ { \prime } = c ( f ^ { \prime } )$ for constant scalars c. 

Another special case of the chain rule which is quite useful is the following: if $f : \mathbf { R } ^ { n }  \mathbf { R } ^ { m }$ is some diferentiable function, and $x _ { j } : \mathbf { R } $ R are diferentiable functions for each $j = 1 , \dots n$ , then 

$$
\frac {d}{d t} f (x _ {1} (t), x _ {2} (t), \dots , x _ {n} (t)) = \sum_ {j = 1} ^ {n} x _ {j} ^ {\prime} (t) \frac {\partial f}{\partial x _ {j}} (x _ {1} (t), x _ {2} (t), \dots , x _ {n} (t)).
$$

(Why is this a special case of the chain rule?). 

$$
- \text { Exercises } -
$$

Exercise 6.4.1. Let $T : \mathbf { R } ^ { n }  \mathbf { R } ^ { m }$ be a linear transformation. Show that $T$ is continuously diferentiable at every point, and in fact $T ^ { \prime } ( x ) = T$ for every x. What is DT? 

Exercise 6.4.2. Let E be a subset of $\mathbf { R } ^ { n }$ . Prove that if a function $f : E \to \mathbf { R } ^ { m }$ is diferentiable at an interior point $x _ { 0 }$ of $E$ , then it is also continuous at $x _ { 0 }$ (Hint: use Exercise 6.1.4.) 

Exercise 6.4.3. Prove Theorem 6.4.1. (Hint: you may wish to review the proof of the ordinary chain rule in single variable calculus, Theorem 10.1.15. The easiest way to proceed is by using the sequence-based definition of limit (see Proposition 3.1.5(b)), and use Exercise 6.1.4.) 

Exercise 6.4.4. State and prove some version of the quotient rule for functions of several variables (i.e., functions of the form $f : E  \mathbf { R }$ for some subset E of $\mathbf { R } ^ { n } )$ . In other words, state a rule which gives a formula for the gradient of $f / g ;$ compare your answer with Theorem 10.1.13(h). Be sure to make clear what all your assumptions are. 

Exercise 6.4.5. Let $\vec { x } : \mathbf { R }  \mathbf { R } ^ { 3 }$ be a diferentiable function, and let $r : \mathbf { R }  \mathbf { R }$ be the function $r ( t ) : = \| \vec { x } ( t ) \|$ , where $\| { \vec { x } } \|$ denotes the length of $\vec { x }$ as measured in the usual $l ^ { 2 }$ metric. Let $t _ { 0 }$ be a real number. Show that if $r ( t _ { 0 } ) \neq 0$ , then $r$ is diferentiable at $t _ { 0 }$ , and 

$$
r ^ {\prime} (t _ {0}) = \frac {\vec {x} ^ {\prime} (t _ {0}) \cdot \vec {x} (t _ {0})}{r (t _ {0})}.
$$

(Hint: use Theorem 6.4.1.) 

## 6.5 Double derivatives and Clairaut’s theorem

We now investigate what happens if one diferentiates a function twice. 

Definition 6.5.1 (Twice continuous diferentiability). Let E be an open subset of $\mathbf { R } ^ { n }$ , and let $f : E \to \mathbf { R } ^ { m }$ be a function. We say that $f$ is continuously diferentiable if the partial derivatives $\frac { \partial f } { \partial x _ { 1 } } , \ldots , \frac { \partial f } { \partial x _ { n } }$ exist and are continuous on E. We say that f is twice continuously diferentiable if it is continuously diferentiable, and the partial derivatives $\textstyle \left\lceil { \frac { \partial f } { \partial x _ { 1 } } } , \ldots , { \frac { \partial f } { \partial x _ { n } } } \right\rceil$ are themselves continuously diferentiable. 

Remark 6.5.2. Continuously diferentiable functions are sometimes called $C ^ { 1 }$ functions; twice continuously diferentiable functions are sometimes called $C ^ { 2 }$ functions. One can also define $C ^ { 3 } , C ^ { 4 }$ , etc. but we shal not do so here. 

Example 6.5.3. Let $f : { \bf R } ^ { 2 }  { \bf R } ^ { 2 }$ be the function $f ( x , y ) = ( x ^ { 2 } +$ $x y , y ^ { 2 } )$ . Then $f$ is continuously diferentiable because the partial derivatives $\begin{array} { r } { \frac { \partial f } { \partial x } ( x , y ) = ( 2 x + y , 0 ) } \end{array}$ and $\begin{array} { r } { \frac { \partial f } { \partial y } ( x , y ) = ( x , 2 y ) } \end{array}$ exist and are continuous on all of $\mathbf { R } ^ { 2 }$ . It is also twice continuously diferentiable, because the double partial derivatives $\begin{array} { r } { \frac { \partial } { \partial x } \frac { \partial f } { \partial x } ( x , y ) = ( \bar { 2 , 0 } ) , \frac { \partial } { \partial y } \frac { \partial f } { \partial x } ( x , y ) = ( 1 , 0 ) } \end{array}$ $\begin{array} { r } { \frac { \partial } { \partial x } \frac { \partial f } { \partial y } ( x , y ) = ( 1 , 0 ) , \frac { \partial } { \partial y } \frac { \partial f } { \partial y } ( x , y ) = ( 0 , 2 ) } \end{array}$ all exist and are continuous. 

Observe in the above example that the double derivatives $\frac { \partial } { \partial y } \frac { \partial f } { \partial x }$ and $\frac { \partial } { \partial x } \frac { \partial f } { \partial y }$ are the same. This is a in fact a general phenomenon: 

Theorem 6.5.4 (Clairaut’s theorem). Let E be an open subset of $\mathbf { R } ^ { n }$ and let $f : E \to \mathbf { R } ^ { m }$ be a twice continuously diferentiable function on E. Then we have $\begin{array} { r } { \frac { \partial } { \partial x _ { j } } \frac { \partial f } { \partial x _ { i } } ( x _ { 0 } ) = \frac { \partial } { \partial x _ { i } } \frac { \partial f } { \partial x _ { j } } ( x _ { 0 } ) } \end{array}$ for all $1 \leq i , j \leq n$ 

Proof. By working with one component of f at a time we can assume that $m = 1$ . The claim is trivial if $i \ : = \ : j$ , so we shall assume that $i \neq j$ . We shall prove the theorem for $x _ { 0 } = 0 ;$ ; the general case is similar. (Actually, once one proves Clairaut’s theorem for $x _ { 0 } = 0$ , one can immediately obtain it for general $x _ { 0 }$ by applying the theorem with $f ( x )$ replaced by $f ( x + x _ { 0 } ) . )$ 

Let a be the number $\begin{array} { r } { \overline { { a } } : = \frac { \partial } { \partial x _ { j } } \frac { \partial f } { \partial x _ { i } } ( 0 ) } \end{array}$ , and $a ^ { \prime }$ denote the quantity $\begin{array} { r } { a ^ { \prime } : = \frac { \partial } { \partial x _ { i } } \frac { \partial f } { \partial x _ { i } } ( 0 ) } \end{array}$ . Our task is to show that $a ^ { \prime } = a$ 

Let $\varepsilon > 0$ . Because the double derivatives of $f$ are continuous, we can find $\mathrm { ~ a ~ } \delta > 0$ such that 

$$
\left| \frac {\partial}{\partial x _ {j}} \frac {\partial f}{\partial x _ {i}} (x) - a \right| \leq \varepsilon
$$

and 

$$
\left| \frac {\partial}{\partial x _ {i}} \frac {\partial f}{\partial x _ {j}} (x) - a ^ {\prime} \right| \leq \varepsilon
$$

whenever $| x | \leq 2 \delta$ 

Now we consider the quantity 

$$
X := f (\delta e _ {i} + \delta e _ {j}) - f (\delta e _ {i}) - f (\delta e _ {j}) + f (0).
$$

From the fundamental theorem of calculus in the $e _ { i }$ variable, we have 

$$
f (\delta e _ {i} + \delta e _ {j}) - f (\delta e _ {j}) = \int_ {0} ^ {\delta} \frac {\partial f}{\partial x _ {i}} (x _ {i} e _ {i} + \delta e _ {j}) d x _ {i}
$$

and 

$$
f (\delta e _ {i}) - f (0) = \int_ {0} ^ {\delta} \frac {\partial f}{\partial x _ {i}} (x _ {i} e _ {i}) d x _ {i}
$$

and hence 

$$
X = \int_ {0} ^ {\delta} \left(\frac {\partial f}{\partial x _ {i}} (x _ {i} e _ {i} + \delta e _ {j}) - \frac {\partial f}{\partial x _ {i}} (x _ {i} e _ {i})\right) d x _ {i}.
$$

But by the mean value theorem, for each $x _ { i }$ we have 

$$
\frac {\partial f}{\partial x _ {i}} (x _ {i} e _ {i} + \delta e _ {j}) - \frac {\partial f}{\partial x _ {i}} (x _ {i} e _ {i}) = \delta \frac {\partial}{\partial x _ {j}} \frac {\partial f}{\partial x _ {i}} (x _ {i} e _ {i} + x _ {j} e _ {j})
$$

for some $0 \leq x _ { j } \leq \delta$ . By our construction of $\delta .$ , we thus have 

$$
\left| \frac {\partial f}{\partial x _ {i}} (x _ {i} e _ {i} + \delta e _ {j}) - \frac {\partial f}{\partial x _ {i}} (x _ {i} e _ {i}) - \delta a \right| \leq \varepsilon \delta .
$$

Integrating this from 0 to $\delta ,$ , we thus obtain 

$$
\left| X - \delta^ {2} a \right| \leq \varepsilon \delta^ {2}.
$$

We can run the same argument with the rˆole of $i$ and $j$ reversed (note that X is symmetric in i and $j )$ , to obtain 

$$
| X - \delta^ {2} a ^ {\prime} | \leq \varepsilon \delta^ {2}.
$$

From the triangle inequality we thus obtain 

$$
| \delta^ {2} a - \delta^ {2} a ^ {\prime} | \leq 2 \varepsilon \delta^ {2},
$$

and thus 

$$
\left| a - a ^ {\prime} \right| \leq 2 \varepsilon .
$$

But this is true for all $\varepsilon > 0$ , and a and $a ^ { \prime }$ do not depend on $\varepsilon ,$ and so we must have $a = a ^ { \prime }$ , as desired. □ 

One should caution that Clairaut’s theorem fails if we do not assume the double derivatives to be continuous; see Exercise 6.5.1. 

— Exercises — 

Exercise 6.5.1. Let $f : { \bf R } ^ { 2 }  { \bf R }$ be the function defined by $\textstyle f ( x , y ) : = { \frac { x y ^ { 3 } } { x ^ { 2 } + y ^ { 2 } } }$ when $( x , y ) \neq ( 0 , 0 )$ , and $f ( 0 , 0 ) : = 0$ . Show that $f$ is continuously diferentiable, and the double derivatives $\frac { \partial } { { \partial y } } \frac { \partial f } { { \partial x } }$ and $\frac { \partial } { \partial x } \frac { \partial f } { \partial y }$ exist, but are not equal to each other at $( 0 , 0 )$ . Explain why this does not contradict Clairaut’s theorem. 

## 6.6 The contraction mapping theorem

Before we turn to the next topic - namely, the inverse function theorem - we need to develop a useful fact from the theory of complete metric spaces, namely the contraction mapping theorem. 

Definition 6.6.1 (Contraction). Let $( X , d )$ be a metric space, and let $f : X \to X$ be a map. We say that f is a contraction if we have $d ( f ( x ) , f ( y ) ) \leq d ( x , y )$ for all $x , y \in X$ . We say that $f$ is a strict contraction if there exists a constant $0 ~ < ~ c ~ < ~ 1$ such that $d ( f ( x ) , f ( y ) ) \leq c d ( x , y )$ for all $x , y \in X$ ; we call c the contraction constant of $f .$ 

Examples 6.6.2. The map $f : \mathbf { R }  \mathbf { R }$ defined by $f ( x ) : = x + 1$ is a contraction but not a strict contraction. The map $f : \mathbf { R }  \mathbf { R }$ defined by $f ( x ) : = x / 2$ is a strict contraction. The map $f : [ 0 , 1 ]  [ 0 , 1 ]$ defined by $f ( x ) : = x - x ^ { 2 }$ is a contraction but not a strict contraction. (For justifications of these statements, see Exercise 6.6.5.) 

Definition 6.6.3 (Fixed points). Let $f : X \to X$ be a map, and $x \in X$ We say that x is a fixed point of f if $f ( x ) = x$ 

Contractions do not necessarily have any fixed points; for instance, the map $f : \mathbf { R }  \mathbf { R }$ defined by $f ( x ) = x + 1$ does not. However, it turns out that strict contractions always do, at least when X is complete: 

Theorem 6.6.4 (Contraction mapping theorem). Let $( X , d )$ be a metric space, and let $f : X \to X$ be a strict contraction. Then f can have at most one fixed point. Moreover, if we also assume that X is non-empty and complete, then f has exactly one fixed point. 

Proof. See Exercise 6.6.7. 

Remark 6.6.5. The contraction mapping theorem is one example of a fixed point theorem - a theorem which guarantees, assuming certain conditions, that a map will have a fixed point. There are a number of other fixed point theorems which are also useful. One amusing one is the so-called hairy ball theorem, which (among other things) states that any continuous map $f : S ^ { 2 } \to S ^ { 2 }$ from the sphere $S ^ { 2 } : = \{ ( x , y , z ) \in$ $\mathbf { R } ^ { 3 } : x ^ { 2 } + y ^ { 2 } + z ^ { 2 } = 1 \}$ to itself, must contain either a fixed point, or an anti-fixed point (a point $x \in S ^ { 2 }$ such that $f ( x ) = - x )$ . A proof of this theorem can be found in any topology text; it is beyond the scope of this text. 

We shall give one consequence of the contraction mapping theorem which is important for our application to the inverse function theorem. Basically, this says that any map f on a ball which is a “small” perturbation of the identity map, remains one-to-one and cannot create any internal holes in the ball. 

Lemma 6.6.6. Let $B ( 0 , r )$ be a ball in $\mathbf { R } ^ { n }$ centered at the origin, and let $g : B ( 0 , r ) \to \mathbf { R } ^ { n }$ be a map such that $g ( 0 ) = 0$ and 

$$
\| g (x) - g (y) \| \leq \frac {1}{2} \| x - y \|
$$

for all x, $y \in B ( 0 , r )$ (here $\lVert x \rVert$ denotes the length of x in $\mathbf { R } ^ { n } )$ . Then the function $f : B ( 0 , r ) \to \mathbf { R } ^ { n }$ defined by $f ( x ) : = x + g ( x )$ is one-to-one, and furthermore the image $f ( B ( 0 , r ) )$ of this map contains the ball $B ( 0 , r / 2 )$ 

Proof. We first show that f is one-to-one. Suppose for sake of contradiction that we had two diferent points x, $y ~ \in ~ B ( 0 , r )$ such that $f ( x ) = f ( y )$ . But then we would have $x + g ( x ) = y + g ( y )$ , and hence 

$$
\| g (x) - g (y) \| = \| x - y \|.
$$

The only way this can be consistent with our hypothesis $\| g ( x ) - g ( y ) \| \leq$ ${ \frac { 1 } { 2 } } \left\| x - y \right\|$ is if $\| x - y \| = 0 , { \mathrm { i . e . } }$ ., if $x = y$ , a contradiction. Thus f is oneto-one. 

Now we show that $f ( B ( 0 , r ) )$ contains $B ( 0 , r / 2 )$ . Let y be any point in $B ( 0 , r / 2 )$ ; our objective is to find a point $x \ \in \ B ( 0 , r )$ such that $f ( x ) = y$ , or in other words that $x = y - g ( x )$ . So the problem is now to find a fixed point of the map $x \mapsto y - g ( x )$ 

Let ${ \boldsymbol { F } } : { \boldsymbol { B } } ( 0 , { \boldsymbol { r } } ) \to { \boldsymbol { B } } ( 0 , { \boldsymbol { r } } )$ denote the function $F ( x ) : = y - g ( x )$ Observe that if $x \in B ( 0 , r )$ , then 

$$
\| F (x) \| \leq \| y \| + \| g (x) \| \leq \frac {r}{2} + \| g (x) - g (0) \| \leq \frac {r}{2} + \frac {1}{2} \| x - 0 \| <   \frac {r}{2} + \frac {r}{2} = r,
$$

so F does indeed map $B ( 0 , r )$ to itself. The same argument shows that for a suficiently small $\varepsilon > 0 , F$ maps the closed ball $\overline { { B ( 0 , r - \varepsilon ) } }$ to itself. Also, for any $x , x ^ { \prime }$ in $B ( 0 , r )$ we have 

$$
\| F (x) - F (x ^ {\prime}) \| = \| g (x ^ {\prime}) - g (x) \| \leq \frac {1}{2} \| x ^ {\prime} - x \|
$$

so $F$ is a strict contraction on $B ( 0 , r )$ , and hence on the complete space $\overline { { B ( 0 , r - \varepsilon ) } }$ . By the contraction mapping theorem, $F$ has a fixed point, i.e., there exists an x such that $x = y - g ( x )$ . But this means that $f ( x ) = y$ , as desired. □ 

$$
- \text { Exercises } -
$$

Exercise 6.6.1. Let $f : [ a , b ]  \mathbf { R }$ be a diferentiable function of one variable such that $| f ^ { \prime } ( x ) | \leq 1$ for all $x \in [ a , b ]$ . Prove that f is a contraction. (Hint: use the mean-value theorem, Corollary 10.2.9.) If in addition $\vert f ^ { \prime } ( x ) \vert < 1$ for all $x \in [ a , b ]$ and f is continuous, show that f is a strict contraction. 

Exercise 6.6.2. Show that if $f : [ a , b ]  \mathbf { R }$ is diferentiable and is a contraction, then $| f ^ { \prime } ( x ) | \leq 1$ 

Exercise 6.6.3. Give an example of a function $f : [ a , b ]  \mathbf { R }$ which is continuously diferentiable and such that $| f ( x ) - f ( y ) | < | x - y |$ for all distinct x, $y \in [ a , b ]$ , but such that $\left| f ^ { \prime } ( x ) \right| = 1$ for at least one value of $x \in [ a , b ]$ 

Exercise 6.6.4. Given an example of a function $f : [ a , b ]  \mathbf { R }$ which is a strict contraction but which is not diferentiable for at least one point x in $[ a , b ]$ 

Exercise 6.6.5. Verify the claims in Examples 6.6.2. 

Exercise 6.6.6. Show that every contraction on a metric space $X$ is necessarily continuous. 

Exercise 6.6.7. Prove Theorem 6.6.4. (Hint: to prove that there is at most one fixed point, argue by contradiction. To prove that there is at least one fixed point, pick any $x _ { 0 } \in X$ and define recursively $x _ { 1 } = f ( x _ { 0 } ) , x _ { 2 } = f ( x _ { 1 } ) , x _ { 3 } =$ $f ( x _ { 2 } )$ , etc. Prove inductively that $d ( x _ { n + 1 } , x _ { n } ) \leq c ^ { n } d ( x _ { 1 } , x _ { 0 } )$ , and conclude (using the geometric series formula, Lemma 7.3.3) that the sequence $( x _ { n } ) _ { n = 0 } ^ { \infty }$ is a Cauchy sequence. Then prove that the limit of this sequence is a fixed point of $f . )$ 

Exercise 6.6.8. Let $( X , d )$ be a complete metric space, and let $f : X \to X$ and $g : X \to X$ be two strict contractions on $X$ with contraction coeficients c and $c ^ { \prime }$ respectively. From Theorem 6.6.4 we know that $f$ has some fixed point $x _ { 0 }$ and $g$ has some fixed point $y _ { 0 }$ . Suppose we know that there is an $\varepsilon > 0$ such that $d ( f ( x ) , g ( x ) ) \leq \varepsilon$ for all $x \in X { \mathrm { ~ ( i . e . , ~ } } f$ and $g$ are within $\varepsilon \ { \mathrm { o f } }$ each other in the uniform metric). Show that $d ( x _ { 0 } , y _ { 0 } ) \leq \varepsilon / ( 1 - \operatorname* { m i n } ( c , c ^ { \prime } ) )$ . Thus nearby contractions have nearby fixed points. 

## 6.7 The inverse function theorem in several variable calculus

We recall the inverse function theorem in single variable calculus (Theorem 10.4.2), which asserts that if a function $f : \mathbf { R }  \mathbf { R }$ is invertible, diferentiable, and $f ^ { \prime } ( x _ { 0 } )$ is non-zero, then $f ^ { - 1 }$ is diferentiable at $f ( x _ { 0 } )$ , and 

$$
(f ^ {- 1}) ^ {\prime} (f (x _ {0})) = \frac {1}{f ^ {\prime} (x _ {0})}.
$$

In fact, one can say something even when $f ^ { \prime }$ is not invertible, as long as we know that $f$ is continuously diferentiable. If $f ^ { \prime } ( x _ { 0 } )$ is nonzero, then $f ^ { \prime } ( x _ { 0 } )$ must be either strictly positive or strictly negative, which implies (since we are assuming $f ^ { \prime }$ to be continuous) that $f ^ { \prime } ( x )$ is either strictly positive for $x$ near $x _ { 0 }$ , or strictly negative for $x$ near $x _ { 0 }$ In particular, $f$ must be either strictly increasing near $x _ { 0 }$ , or strictly decreasing near $x _ { 0 }$ . In either case, $f$ will become invertible if we restrict the domain and range of $f$ to be suficiently close to $x _ { 0 }$ and to $f ( x _ { 0 } )$ 

respectively. (The technical terminology for this is that f is locally invertible near $x _ { 0 } . )$ 

The requirement that f be continuously diferentiable is important; see Exercise 6.7.1. 

It turns out that a similar theorem is true for functions $f : \mathbf { R } ^ { n }  \mathbf { R } ^ { n }$ from one Euclidean space to the same space. However, the condition that $f ^ { \prime } ( x _ { 0 } )$ is non-zero must be replaced with a slightly diferent one, namely that $f ^ { \prime } ( x _ { 0 } )$ is invertible. We first remark that the inverse of a linear transformation is also linear: 

Lemma 6.7.1. Let $T : \mathbf { R } ^ { n }  \mathbf { R } ^ { n }$ be a linear transformation which is also invertible. Then the inverse transformation $T ^ { - 1 } : \mathbf { R } ^ { n }  \mathbf { R } ^ { n }$ is also linear. 

Proof. See Exercise 6.7.2. 

We can now prove an important and useful theorem, arguably one of the most important theorems in several variable diferential calculus. 

Theorem 6.7.2 (Inverse function theorem). Let E be an open subset $o f { \mathbf { R } } ^ { n }$ , and let $f : E \to \mathbf { R } ^ { n }$ be a function which is continuously diferentiable on E. Suppose $x _ { 0 } \in E$ is such that the linear transformation $f ^ { \prime } ( x _ { 0 } ) : \mathbf { R } ^ { n }  \mathbf { R } ^ { n }$ is invertible. Then there exists an open set U in E containing $x _ { 0 }$ , and an open set V in $\mathbf { R } ^ { n }$ containing $f ( x _ { 0 } )$ , such that f is a bijection from U to V. In particular, there is an inverse map $f ^ { - 1 } : V \to U$ . Furthermore, this inverse map is diferentiable at $f ( x _ { 0 } )$ and 

$$
(f ^ {- 1}) ^ {\prime} (f (x _ {0})) = (f ^ {\prime} (x _ {0})) ^ {- 1}.
$$

Proof. We first observe that once we know the inverse map $f ^ { - 1 }$ is differentiable, the formula $( f ^ { - 1 } ) ^ { \prime } ( f ( x _ { 0 } ) ) = ( f ^ { \prime } ( x _ { 0 } ) ) ^ { - 1 }$ is automatic. This comes from starting with the identity 

$$
I = f ^ {- 1} \circ f
$$

on $U$ , where $I : \mathbf { R } ^ { n }  \mathbf { R } ^ { n }$ is the identity map $I x : = x$ , and then diferentiating both sides using the chain rule at $x _ { 0 }$ to obtain 

$$
I ^ {\prime} (x _ {0}) = (f ^ {- 1}) ^ {\prime} (f (x _ {0})) f ^ {\prime} (x _ {0}).
$$

Since $I ^ { \prime } ( x _ { 0 } ) = I $ , we thus have $( f ^ { - 1 } ) ^ { \prime } ( f ( x _ { 0 } ) ) = ( f ^ { \prime } ( x _ { 0 } ) ) ^ { - 1 }$ as desired. 

We remark that this argument shows that if $f ( x _ { 0 } )$ is not invertible, then there is no way that an inverse $f ^ { - 1 }$ can exist and be diferentiable at $f ( x _ { 0 } )$ 

Next, we observe that it sufices to prove the theorem under the additional assumption $f ( x _ { 0 } ) = 0$ . The general case then follows from the special case by replacing f by a new function ${ \tilde { f } } ( x ) : = f ( x ) - f ( x _ { 0 } )$ and then applying the special case to $\tilde { f }$ (note that V will have to shift by $f ( x _ { 0 } ) )$ . Note that $f ^ { - 1 } ( y ) = \tilde { f } ^ { - 1 } ( y - \tilde { f } ( x _ { 0 } ) )$ (why?). Henceforth we will always assume $f ( x _ { 0 } ) = 0$ 

In a similar manner, one can make the assumption $x _ { 0 } = 0$ . The general case then follows from this case by replacing f by a new function ${ \tilde { f } } ( x ) : = f ( x + x _ { 0 } )$ and applying the special case to $\tilde { f }$ (note that $E$ and U will have to shift by $x _ { 0 } )$ . Note that $f ^ { - 1 } ( y ) = \tilde { f } ^ { - 1 } ( y ) + x _ { 0 } \cdot \mathrm { w h y ? }$ Henceforth we will always assume $x _ { 0 } ~ = ~ 0$ . Thus we now have that $f ( 0 ) = 0$ and that $f ^ { \prime } ( 0 )$ is invertible. 

Finally, one can assume that $f ^ { \prime } ( 0 ) = I$ , where $I : \mathbf { R } ^ { n }  \mathbf { R } ^ { n }$ is the identity transformation $I x = x$ . The general case then follows from this case by replacing f with a new function $\tilde { f } : E \to \mathbf { R } ^ { n }$ defined by $\tilde { f } ( x ) : = f ^ { \prime } ( 0 ) ^ { - 1 } f ( x )$ , and applying the special case to this case. Note from Lemma $6 . 7 . 1$ that $f ^ { \prime } ( 0 ) ^ { - 1 }$ is a linear transformation. In particular, we note that $\tilde { f } ( 0 ) = 0$ and that 

$$
\tilde {f} ^ {\prime} (0) = f ^ {\prime} (0) ^ {- 1} f ^ {\prime} (0) = I,
$$

so by the special case of the inverse function theorem we know that there exists an open set $U ^ { \prime }$ containing 0, and an open set $V ^ { \prime }$ containing $0 ,$ such that $\tilde { f }$ is a bijection from $U ^ { \prime }$ to $V ^ { \prime }$ , and that $\tilde { f } ^ { - 1 } : V ^ { \prime } \to U ^ { \prime }$ is diferentiable at 0 with derivative I. But we have $f ( x ) = f ^ { \prime } ( 0 ) { \tilde { f } } ( x )$ and hence $f$ is a bijection from $U ^ { \prime }$ to $f ^ { \prime } ( 0 ) ( V ^ { \prime } )$ (note that $f ^ { \prime } ( 0 )$ is also a bijection). Since $f ^ { \prime } ( 0 )$ and its inverse are both continuous, $f ^ { \prime } ( 0 ) ( V ^ { \prime } )$ is open, and it certainly contains 0. Now consider the inverse function $f ^ { - 1 } : f ^ { \prime } ( 0 ) ( V ^ { \prime } ) \to U ^ { \prime }$ . Since $f ( x ) = f ^ { \prime } ( 0 ) \tilde { f } ( x )$ , we see that $f ^ { - 1 } ( y ) =$ $\tilde { f } ^ { - 1 } ( f ^ { \prime } ( 0 ) ^ { - 1 } y )$ for all $y ~ \in ~ f ^ { \prime } ( 0 ) ( V ^ { \prime } ) ~ \mathrm { { ( w h y ? } }$ use the fact that $\tilde { f }$ is a bijection from $U ^ { \prime }$ to $V ^ { \prime } )$ . In particular we see that $f ^ { - 1 }$ is diferentiable at 0. 

So all we have to do now is prove the inverse function theorem in the special case, when $x _ { 0 } = 0 , f ( x _ { 0 } ) = 0$ , and $f ^ { \prime } ( x _ { 0 } ) = I$ . Let $g : E \to \mathbf { R } ^ { n }$ denote the function $f ( x ) - x$ . Then $g ( 0 ) = 0$ and $g ^ { \prime } ( 0 ) = 0$ . In particular 

$$
\frac {\partial g}{\partial x _ {j}} (0) = 0
$$

for $j = 1 , \dotsc , n$ . Since g is continuously diferentiable, there thus exists a ball $B ( 0 , r )$ in $E$ such that 

$$
\left\| \frac {\partial g}{\partial x _ {j}} (x) \right\| \leq \frac {1}{2 n ^ {2}}
$$

for all $x \in B ( 0 , r )$ . (There is nothing particularly special about $\textstyle { \frac { 1 } { 2 n ^ { 2 } } }$ , we just need a nice small number here.) In particular, for any $x \in B ( 0 , r )$ and $v = ( v _ { 1 } , \ldots , v _ { n } )$ we have 

$$
\| D _ {v} g (x) \| = \left\| \sum_ {j = 1} ^ {n} v _ {j} \frac {\partial g}{\partial x _ {j}} (x) \right\|
$$

$$
\leq \sum_ {j = 1} ^ {n} | v _ {j} | \left\| \frac {\partial g}{\partial x _ {j}} (x) \right\|
$$

$$
\leq \sum_ {j = 1} ^ {n} \| v \| \frac {1}{2 n ^ {2}} \leq \frac {1}{2 n} \| v \|.
$$

But now for any $x , y \in B ( 0 , r )$ , we have by the fundamental theorem of calculus 

$$
\begin{array}{c} g (y) - g (x) = \int_ {0} ^ {1} \frac {d}{d t} g (x + t (y - x)) d t \\ = \int_ {0} ^ {1} D _ {y - x} g (x + t (y - x)) d t. \end{array}
$$

By the previous remark, the vectors $D _ { y - x } g ( x + t ( y - x ) )$ have a magnitude of at most ${ \frac { 1 } { 2 n } } \| y - x \|$ . Thus every component of these vectors has magnitude at most ${ \frac { 1 } { 2 n } } \left\| y - x \right\|$ . Thus every component of $g ( y ) - g ( x )$ has magnitude at most ${ \frac { 1 } { 2 n } } \| y - x \|$ , and hence $g ( y ) - g ( x )$ itself has magnitude at most ${ \frac { 1 } { 2 } } \| y - { \overline { { x } } } \|$ (actually, it will be substantially less than this, but this bound will be enough for our purposes). In other words, g is a contraction. By Lemma 6.6.6, the map $f = g + I$ is thus one-to-one on $B ( 0 , r )$ , and the image $f ( B ( 0 , r ) )$ contains $B ( 0 , r / 2 )$ . In particular we have an inverse map $f ^ { - 1 } : B ( 0 , r / 2 ) \to B ( 0 , r )$ defined on $B ( 0 , r / 2 )$ 

Applying the contraction bound with $y = 0$ we obtain in particular that 

$$
\| g (x) \| \leq \frac {1}{2} \| x \|
$$

for all $x \in B ( 0 , r )$ , and so by the triangle inequality 

$$
\frac {1}{2} \| x \| \leq \| f (x) \| \leq \frac {3}{2} \| x \|
$$

for all $x \in B ( 0 , r )$ 

Now we set $V : = B ( 0 , r / 2 )$ and $U : = f ^ { - 1 } ( B ( 0 , r / 2 ) )$ Then by construction f is a bijection from U to V. V is clearly open, and $U =$ $f ^ { - 1 } ( V )$ is also open since f is continuous. (Notice that if a set is open relative to $B ( 0 , r )$ , then it is open in $\mathbf { R } ^ { n }$ as well). Now we want to show that $f ^ { - 1 } : V \to U$ is diferentiable at 0 with derivative $I ^ { - 1 } = I$ . In other words, we wish to show that 

$$
\lim _ {x \to 0; x \in V \setminus \{0 \}} \frac {\| f ^ {- 1} (x) - f ^ {- 1} (0) - I (x - 0) \|}{\| x \|} = 0.
$$

Since $f ( 0 ) = 0$ , we have $f ^ { - 1 } ( 0 ) = 0$ , and the above simplifies to 

$$
\lim _ {x \to 0; x \in V \setminus \{0 \}} \frac {\| f ^ {- 1} (x) - x \|}{\| x \|} = 0.
$$

Let $( x _ { n } ) _ { n = 1 } ^ { \infty }$ be any sequence in $V \backslash 0$ that converges to 0. By Proposition 3.1.5(b), it sufices to show that 

$$
\lim _ {n \to \infty} \frac {\| f ^ {- 1} (x _ {n}) - x _ {n} \|}{\| x _ {n} \|} = 0.
$$

Write $y _ { n } : = f ^ { - 1 } ( x _ { n } )$ . Then $y _ { n } \in B ( 0 , r )$ and $x _ { n } = f ( y _ { n } )$ . In particular we have 

$$
\frac {1}{2} \| y _ {n} \| \leq \| x _ {n} \| \leq \frac {3}{2} \| y _ {n} \|
$$

and so since $\| x _ { n } \|$ goes to $0 , \ \| y _ { n } \|$ goes to zero also, and their ratio remains bounded. It will thus sufice to show that 

$$
\lim _ {n \to \infty} \frac {\| y _ {n} - f (y _ {n}) \|}{\| y _ {n} \|} = 0.
$$

But since $y _ { n }$ is going to 0, and f is diferentiable at 0, we have 

$$
\lim _ {n \to \infty} \frac {\| f (y _ {n}) - f (0) - f ^ {\prime} (0) (y _ {n} - 0) \|}{\| y _ {n} \|} = 0
$$

as desired (since $f ( 0 ) = 0$ and $f ^ { \prime } ( 0 ) = I )$ 

## 6.8. The implicit function theorem

The inverse function theorem gives a useful criterion for when a function is (locally) invertible at a point $x _ { 0 } \textrm { - } \mathrm { a l l }$ we need is for its derivative $f ^ { \prime } ( x _ { 0 } )$ to be invertible (and then we even get further information, for instance we can compute the derivative of $f ^ { - 1 }$ at $f ( x _ { 0 } ) )$ . Of course, this begs the question of how one can tell whether the linear transformation $f ^ { \prime } ( x _ { 0 } )$ is invertible or not. Recall that we have $f ^ { \prime } ( x _ { 0 } ) = L _ { D f ( x _ { 0 } ) }$ , so by Lemmas 6.1.13 and 6.1.16 we see that the linear transformation $f ^ { \prime } ( x _ { 0 } )$ is invertible if and only if the matrix $D f ( x _ { 0 } )$ is. There are many ways to check whether a matrix such as $D f ( x _ { 0 } )$ is invertible; for instance, one can use determinants, or alternatively Gaussian elimination methods. We will not pursue this matter here, but refer the reader to any linear algebra text. 

If $f ^ { \prime } ( x _ { 0 } )$ exists but is non-invertible, then the inverse function theorem does not apply. In such a situation it is not possible for $f ^ { - 1 }$ to exist and be diferentiable at $x _ { 0 } ;$ this was remarked in the above proof. But it is still possible for $f$ to be invertible. For instance, the single-variable function $f : \mathbf { R }  \mathbf { R }$ defined by $f ( x ) = x ^ { 3 }$ is invertible despite $f ^ { \prime } ( 0 )$ not being invertible. 

## — Exercises —

Exercise 6.7.1. Let $f : \textbf { R }  \textbf { R }$ be the function defined by $f ( x ) \ : = \ x +$ $x ^ { 2 } \sin ( 1 / x ^ { 4 } )$ for $x \neq 0$ and $f ( 0 ) : = 0$ . Show that $f$ is diferentiable and $f ^ { \prime } ( 0 ) = 1$ , but $f$ is not increasing on any open set containing 0 (Hint: show that the derivative of $f$ can turn negative arbitrarily close to 0. Drawing a graph of f may aid your intuition.) 

Exercise 6.7.2. Prove Lemma 6.7.1. 

Exercise 6.7.3. Let $f : \mathbf { R } ^ { n }  \mathbf { R } ^ { n }$ be a continuously diferentiable function such that $f ^ { \prime } ( x )$ is an invertible linear transformation for every $x \in \mathbf { R } ^ { n }$ . Show that whenever V is an open set in $\mathbf { R } ^ { n }$ , that $f ( V )$ is also open. (Hint: use the inverse function theorem.) 

## 6.8 The implicit function theorem

Recall (from Exercise 3.5.10) that a function $f : \mathbf { R }  \mathbf { R }$ gives rise to a graph 

$$
\{(x, f (x)): x \in \mathbf {R} \}
$$

which is a subset of $\mathbf { R } ^ { 2 }$ , usually looking like a curve. However, not all curves are graphs, they must obey the vertical line test, that for every x there is exactly one y such that $( x , y )$ is in the curve. For instance, the circle $\{ ( x , y ) \in \mathbf { R } ^ { 2 } : x ^ { 2 } + y ^ { 2 } = 1 \}$ is not a graph, although if one restricts to a semicircle such as $\{ ( x , y ) \in \mathbf { R } ^ { 2 } : x ^ { 2 } + y ^ { 2 } = 1 , y > 0 \}$ then one again obtains a graph. Thus while the entire circle is not a graph, certain local portions of it are. (The portions of the circle near $( 1 , 0 )$ and $( - 1 , 0 )$ are not graphs over the variable x, but they are graphs over the variable y). 

Similarly, any function $g \ \prime : \ \mathbf { R } ^ { n } \ \to \ \mathbf { R }$ gives rise to a graph $\{ ( x , g ( x ) ) : x \in \mathbf { R } ^ { n } \}$ in $\mathbf { R } ^ { n + 1 }$ , which in general looks like some sort of n-dimensional surface in $\mathbf { R } ^ { n + 1 }$ (the technical term for this is a hypersurface). Conversely, one may ask which hypersurfaces are actually graphs of some function, and whether that function is continuous or diferentiable. 

If the hypersurface is given geometrically, then one can again invoke the vertical line test to work out whether it is a graph or not. But what if the hypersurface is given algebraically, for instance the surface $\{ ( x , y , z ) \in \mathbf { R } ^ { 3 } : x y + y z + z x = - 1 \} ?$ Or more generally, a hypersurface of the form $\{ x \in \mathbf { R } ^ { n } : g ( x ) = 0 \}$ , where $g : \mathbf { R } ^ { n }  \mathbf { R }$ is some function? In this case, it is still possible to say whether the hypersurface is a graph, locally at least, by means of the implicit function theorem. 

Theorem 6.8.1 (Implicit function theorem). Let E be an open subset of $\mathbf { R } ^ { n }$ , let $f : E  \mathbf { R }$ be continuously diferentiable, and let $y = ( y _ { 1 } , \dotsc , y _ { n } )$ be a point in E such that $f ( y ) = 0$ and $\begin{array} { r } { \frac { \partial f } { \partial x _ { n } } ( y ) \neq 0 } \end{array}$ . Then there exists an open subset U of $\mathbf { R } ^ { n - 1 }$ containing $\left( y _ { 1 } , \ldots , y _ { n - 1 } \right)$ , an open subset V of E containing y, and a function $g : U  \mathbf { R }$ such that $g ( y _ { 1 } , \dots , y _ { n - 1 } ) = y _ { n }$ , and 

$$
\{(x _ {1}, \dots , x _ {n}) \in V: f (x _ {1}, \dots , x _ {n}) = 0 \}
$$

$$
= \left\{\left(x _ {1}, \dots , x _ {n - 1}, g \left(x _ {1}, \dots , x _ {n - 1}\right)\right): \left(x _ {1}, \dots , x _ {n - 1}\right) \in U \right\}.
$$

In other words, the set $\{ x \in V : f ( x ) = 0 \}$ is a graph of a function over U. Moreover, g is diferentiable at $\left( y _ { 1 } , \ldots , y _ { n - 1 } \right)$ , and we have 

$$
\frac {\partial g}{\partial x _ {j}} (y _ {1}, \dots , y _ {n - 1}) = - \frac {\partial f}{\partial x _ {j}} (y) / \frac {\partial f}{\partial x _ {n}} (y)\tag{6.1}
$$

for all $1 \leq j \leq n - 1$ 

Remark 6.8.2. The equation (6.1) is sometimes derived using implicit diferentiation. Basically, the point is that if you know that 

$$
f (x _ {1}, \ldots , x _ {n}) = 0
$$

then (as long as $\begin{array} { r } { \frac { \partial f } { \partial x _ { n } } \neq 0 ) } \end{array}$ the variable $x _ { n }$ is “implicitly” defined in terms of the other $n - 1$ variables, and one can diferentiate the above identity in, say, the $x _ { j }$ direction using the chain rule to obtain 

$$
\frac {\partial f}{\partial x _ {j}} + \frac {\partial f}{\partial x _ {n}} \frac {\partial x _ {n}}{\partial x _ {j}} = 0
$$

which is (6.1) in disguise (we are using g to represent the implicit function defining $x _ { n }$ in terms of $x _ { 1 } , \ldots , x _ { n } )$ . Thus, the implicit function theorem allows one to define a dependence implicitly, by means of a constraint rather than by a direct formula of the form $x _ { n } = g ( x _ { 1 } , . . . , x _ { n - 1 } )$ 

Proof. This theorem looks somewhat fearsome, but actually it is a fairly quick consequence of the inverse function theorem. Let $F : E \to \mathbf { R } ^ { n }$ be the function 

$$
F (x _ {1}, \dots , x _ {n}) := (x _ {1}, \dots , x _ {n - 1}, f (x _ {1}, \dots , x _ {n})).
$$

This function is continuously diferentiable. Also note that 

$$
F (y) = (y _ {1}, \ldots , y _ {n - 1}, 0)
$$

and 

$$
D F (y) = \left(\frac {\partial f}{\partial x _ {1}} (y) ^ {T}, \frac {\partial f}{\partial x _ {2}} (y) ^ {T}, \dots , \frac {\partial f}{\partial x _ {n}} (y) ^ {T}\right)
$$

$$
= \left( \begin{array}{c c c c c} 1 & 0 & \ldots & 0 & 0 \\ 0 & 1 & \ldots & 0 & 0 \\ \vdots & \vdots & \ddots & \vdots & \vdots \\ 0 & 0 & \ldots & 1 & 0 \\ \frac {\partial f}{\partial x _ {1}} (y) & \frac {\partial f}{\partial x _ {2}} (y) & \ldots & \frac {\partial f}{\partial x _ {n - 1}} (y) & \frac {\partial f}{\partial x _ {n}} (y) \end{array} \right).
$$

Since $\textstyle { \frac { \partial f } { \partial x _ { n } } } ( y )$ is assumed by hypothesis to be non-zero, this matrix is invertible; this can be seen either by computing the determinant, or using row reduction, or by computing the inverse explicitly, which is 

$$
D F (y) ^ {- 1} = \left( \begin{array}{l l l l l} 1 & 0 & \ldots & 0 & 0 \\ 0 & 1 & \ldots & 0 & 0 \\ \vdots & \vdots & \ddots & \vdots & \vdots \\ 0 & 0 & \ldots & 1 & 0 \\ - \frac {\partial f}{\partial x _ {1}} (y) / a & - \frac {\partial f}{\partial x _ {2}} (y) / a & \ldots & - \frac {\partial f}{\partial x _ {n - 1}} (y) / a & 1 / a \end{array} \right),
$$

where we have written $\begin{array} { r } { a = \frac { \partial f } { \partial x _ { n } } ( y ) } \end{array}$ for short. Thus the inverse function theorem applies, and we can find an open set V in $E$ containing $y ,$ and an open set $W$ in $\mathbf { R } ^ { n }$ containing $F ( y ) = ( y _ { 1 } , \dots , y _ { n - 1 } , 0 )$ , such that $F$ is a bijection from $V$ to $W$ , and that $F ^ { - 1 }$ is diferentiable at $( y _ { 1 } , . . . , y _ { n - 1 } , 0 )$ 

Let us write $F ^ { - 1 }$ in co-ordinates as 

$$
F ^ {- 1} (x) = \left(h _ {1} (x), h _ {2} (x), \dots , h _ {n} (x)\right)
$$

where $x \in W$ . Since $F ( F ^ { - 1 } ( x ) ) = x$ , we have $h _ { j } ( x _ { 1 } , \ldots , x _ { n } ) = x _ { j }$ for all $1 \leq j \leq n - 1$ and $x \in W$ , and 

$$
f (x _ {1}, \dots , x _ {n - 1}, h _ {n} (x _ {1}, \dots , x _ {n})) = x _ {n}.
$$

Also, $h _ { n }$ is diferentiable at $( y _ { 1 } , \dotsc , y _ { n - 1 } , 0 )$ since $F ^ { - 1 }$ is. 

Now we set $U : = \{ ( x _ { 1 } , \ldots , x _ { n - 1 } ) \in \mathbf { R } ^ { n - 1 } : ( x _ { 1 } , \ldots , x _ { n - 1 } , 0 ) \in W \}$ Note that $U$ is open and contains $\left( y _ { 1 } , \ldots , y _ { n - 1 } \right)$ . Now we define $g : U \to$ R by $g ( x _ { 1 } , \ldots , x _ { n - 1 } ) : = h _ { n } ( x _ { 1 } , \ldots , x _ { n - 1 } , 0 )$ . Then $g$ is diferentiable at $\left( y _ { 1 } , \ldots , y _ { n - 1 } \right)$ . Now we prove that 

$$
\{(x _ {1}, \dots , x _ {n}) \in V: f (x _ {1}, \dots , x _ {n}) = 0 \}
$$

$$
= \left\{\left(x _ {1}, \dots , x _ {n - 1}, g \left(x _ {1}, \dots , x _ {n - 1}\right)\right): \left(x _ {1}, \dots , x _ {n - 1}\right) \in U \right\}.
$$

First suppose that $( x _ { 1 } , \ldots , x _ { n } ) \ \in \ V$ and $f ( x _ { 1 } , \ldots , x _ { n } ) ~ = ~ 0$ Then we have $F ( x _ { 1 } , \ldots , x _ { n } ) \ = \ ( x _ { 1 } , \ldots , x _ { n - 1 } , 0 )$ , which lies in W. Thus $( x _ { 1 } , \ldots , x _ { n - 1 } )$ lies in U. Applying $F ^ { - 1 }$ , we see that $( x _ { 1 } , \ldots , x _ { n } ) \ =$ $F ^ { - 1 } ( x _ { 1 } , \dots , x _ { n - 1 } , 0 )$ . In particular $x _ { n } = h _ { n } ( x _ { 1 } , \ldots , x _ { n - 1 } , 0 )$ , and hence $x _ { n } = g ( x _ { 1 } , \dotsc , x _ { n - 1 } )$ . Thus every element of the left-hand set lies in the right-hand set. The reverse inclusion comes by reversing all the above steps and is left to the reader. 

Finally, we show the formula for the partial derivatives of $g .$ . From the preceding discussion we have 

$$
f (x _ {1}, \dots , x _ {n - 1}, g (x _ {1}, \dots , x _ {n - 1})) = 0
$$

for all $( x _ { 1 } , \ldots , x _ { n - 1 } ) \in U$ . Since g is diferentiable at $\left( y _ { 1 } , \ldots , y _ { n - 1 } \right)$ , and $f$ is diferentiable at $( y _ { 1 } , \dots , y _ { n - 1 } , g ( y _ { 1 } , \dots , y _ { n - 1 } ) ) = y$ , we may use the chain rule, diferentiating in $x _ { j }$ , to obtain 

$$
\frac {\partial f}{\partial x _ {j}} (y) + \frac {\partial f}{\partial x _ {n}} (y) \frac {\partial g}{\partial x _ {j}} (y _ {1}, \dots , y _ {n - 1}) = 0
$$

and the claim follows by simple algebra. 

Example 6.8.3. Consider the surface $S : = \{ ( x , y , z ) \in \mathbf { R } ^ { 3 } : x y + y z +$ $z x = - 1 \}$ , which we rewrite as $\{ ( x , y , z ) \in \mathbf { R } ^ { 3 } : f ( x , y , z ) = 0 \}$ , where $f : { \bf R } ^ { 3 }  { \bf R }$ is the function $f ( x , y , z ) : = x y + y z + z x + 1$ . Clearly $f$ is continuously diferentiable, and $\begin{array} { r } { \frac { \partial f } { \partial z } = y + x } \end{array}$ . Thus for any $( x _ { 0 } , y _ { 0 } , z _ { 0 } )$ in $S$ with $y _ { 0 } + x _ { 0 } \neq 0$ , one can write this surface (near $( x _ { 0 } , y _ { 0 } , z _ { 0 } ) )$ as a graph of the form $\{ ( x , y , g ( x , y ) ) : ( x , y ) \in U \}$ for some open set U containing $( x _ { 0 } , y _ { 0 } )$ , and some function g which is diferentiable at $( x _ { 0 } , y _ { 0 } )$ . Indeed one can implicitly diferentiate to obtain that 

$$
\frac {\partial g}{\partial x} (x _ {0}, y _ {0}) = - \frac {y _ {0} + z _ {0}}{y _ {0} + x _ {0}} \text { and } \frac {\partial g}{\partial y} (x _ {0}, y _ {0}) = - \frac {x _ {0} + z _ {0}}{y _ {0} + x _ {0}}.
$$

In the implicit function theorem, if the derivative $\frac { \partial f } { \partial x _ { n } }$ equals zero at some point, then it is unlikely that the set $\{ x \in \mathbf { R } ^ { n } : ^ { \prime \prime } ( x ) = 0 \}$ can be written as a graph of the $x _ { n }$ variable in terms of the other $n - 1$ variables near that point. However, if some other derivative $\frac { \partial f } { \partial x _ { j } }$ is zero, then it would be possible to write the $x _ { j }$ variable in terms of the other $n - 1$ variables, by a variant of the implicit function theorem. Thus as long as the gradient $\nabla f$ is not entirely zero, one can write this set $\{ x \in \mathbf { R } ^ { n } : f ( x ) = 0 \}$ as a graph of some variable $x _ { j }$ in terms of the other $n - 1$ variables. (The circle $\{ ( x , y ) \in \mathbf { R } ^ { 2 } : x ^ { 2 } + y ^ { 2 } - 1 = 0 \}$ is a good example of this; it is not a graph of y in terms of x, or x in terms of y, but near every point it is one of the two. And this is because the gradient of $x ^ { 2 } + y ^ { 2 } - 1$ is never zero on the circle.) However, if f does vanish at some point $x _ { 0 }$ , then we say that f has a critical point at $x _ { 0 }$ and the behavior there is much more complicated. For instance, the set $\{ ( x , y ) \in \mathbf { R } ^ { 2 } : x ^ { 2 } - y ^ { 2 } = 0 \}$ has a critical point at $( 0 , 0 )$ and there the set does not look like a graph of any sort (it is the union of two lines). 

Remark 6.8.4. Sets which look like graphs of continuous functions at every point have a name, they are called manifolds. Thus $\{ x \in \mathbf { R } ^ { n }$ $f ( x ) = 0 \}$ will be a manifold if it contains no critical points of f. The theory of manifolds is very important in modern geometry (especially diferential geometry and algebraic geometry), but we will not discuss it here as it is a graduate level topic. 

## Chapter 7

## Lebesgue measure

In the previous chapter we discussed diferentiation in several variable calculus. It is now only natural to consider the question of integration in several variable calculus. The general question we wish to answer is this: given some subset $\Omega$ of $\mathbf { R } ^ { n }$ , and some real-valued function $f : \Omega  \mathbf { R } \quad$ , is it possible to integrate f on $\Omega$ to obtain some number $\int _ { \Omega } f \colon$ (It is possible to consider other types of functions, such as complex-valued or vector-valued functions, but this turns out not to be too dificult once one knows how to integrate real-valued functions, since one can integrate a complex or vector valued function, by integrating each realvalued component of that function separately.) 

In one dimension we already have developed (in Chapter 11) the notion of a Riemann integral $\int _ { [ a , b ] } f$ , which answers this question when $\Omega$ is an interval $\Omega = [ a , b ]$ , and $f$ is Riemann integrable. Exactly what Riemann integrability means is not important here, but let us just remark that every piecewise continuous function is Riemann integrable, and in particular every piecewise constant function is Riemann integrable. However, not all functions are Riemann integrable. It is possible to extend this notion of a Riemann integral to higher dimensions, but it requires quite a bit of efort and one can still only integrate “Riemann integrable” functions, which turn out to be a rather unsatisfactorily small class of functions. (For instance, the pointwise limit of Riemann integrable functions need not be Riemann integrable, and the same goes for an $L ^ { 2 }$ limit, although we have already seen that uniform limits of Riemann integrable functions remain Riemann integrable.) 

Because of this, we must look beyond the Riemann integral to obtain a truly satisfactory notion of integration, one that can handle even very discontinuous functions. This leads to the notion of the Lebesgue integral, which we shall spend this chapter and the next constructing. The 

Lebesgue integral can handle a very large class of functions, including all the Riemann integrable functions but also many others as well; in fact, it is safe to say that it can integrate virtually any function that one actually needs in mathematics, at least if one works on Euclidean spaces and everything is absolutely integrable. (If one assumes the axiom of choice, then there are still some pathological functions one can construct which cannot be integrated by the Lebesgue integral, but these functions will not come up in real-life applications.) 

Before we turn to the details, we begin with an informal discussion. In order to understand how to compute an integral $\textstyle \int _ { \Omega } f $ , we must first understand a more basic and fundamental question: how does one compute the length/area/volume of Ω? To see why this question is connected to that of integration, observe that if one integrates the function 1 on the set $\Omega ,$ then one should obtain the length of Ω (if Ω is one-dimensional), the area of $\Omega$ (if Ω is two-dimensional), or the volume of $\Omega$ (if Ω is threedimensional). To avoid splitting into cases depending on the dimension, we shall refer to the measure of $\Omega$ as either the length, area, volume, (or hypervolume, etc.) of $\Omega ,$ depending on what Euclidean space $\mathbf { R } ^ { n }$ we are working in. 

Ideally, to every subset Ω of $\mathbf { R } ^ { n }$ we would like to associate a nonnegative number $m ( \Omega )$ , which will be the measure of Ω (i.e., the length, area, volume, etc.). We allow the possibility for $m ( \Omega )$ to be zero (e.g., if Ω is just a single point or the empty set) or for $m ( \Omega )$ to be infinite (e.g., if Ω is all of $\mathbf { R } ^ { n } )$ . This measure should obey certain reasonable properties; for instance, the measure of the unit cube $( 0 , 1 ) ^ { n } : = \{ ( x _ { 1 } , \ldots , x _ { n } ) : 0 <$ $x _ { i } < 1 \}$ should equal 1, we should have $m ( A \cup B ) = m ( A ) + m ( B )$ if A and B are disjoint, we should have $m ( A ) \leq m ( B )$ whenever $A \subseteq B$ , and we should have m $( x + A ) = m ( A )$ for any $x \in \mathbf { R } ^ { n }$ (i.e., if we shift A by the vector x the measure should be the same). 

Remarkably, it turns out that such a measure does not exist; one cannot assign a non-negative number to every subset of $\mathbf { R } ^ { n }$ which has the above properties. This is quite a surprising fact, as it goes against one’s intuitive concept of volume; we shall prove it later in these notes. (An even more dramatic example of this failure of intuition is the Banach-Tarski paradox, in which a unit ball in $\mathbf { R } ^ { 3 }$ is decomposed into five pieces, and then the five pieces are reassembled via translations and rotations to form two complete and disjoint unit balls, thus violating any concept of conservation of volume; however we will not discuss this paradox here.) 

What these paradoxes mean is that it is impossible to find a reasonable way to assign a measure to every single subset of $\mathbf { R } ^ { n }$ . However, we can salvage matters by only measuring a certain class of sets in $\mathbf { R } ^ { n }$ the measurable sets. These are the only sets Ω for which we will define the measure $m ( \Omega )$ , and once one restricts one’s attention to measurable sets, one recovers all the above properties again. Furthermore, almost all the sets one encounters in real life are measurable (e.g., all open and closed sets will be measurable), and so this turns out to be good enough to do analysis. 

## 7.1 The goal: Lebesgue measure

Let $\mathbf { R } ^ { n }$ be a Euclidean space. Our goal in this chapter is to define a concept of measurable set, which will be a special kind of subset of $\mathbf { R } ^ { n }$ , and for every such measurable set $\Omega \subset \mathbf { R } ^ { n }$ , we will define the Lebesgue measure $m ( \Omega )$ to be a certain number in $[ 0 , \infty ]$ . The concept of measurable set will obey the following properties: 

(i) (Borel property) Every open set in $\mathbf { R } ^ { n }$ is measurable, as is every closed set. 

(ii) (Complementarity) If Ω is measurable, then $\mathbf { R } ^ { n } \backslash \Omega$ is also measurable. 

(iii) (Boolean algebra property) If $( \Omega _ { j } ) _ { j \in J }$ is any finite collection of measurable sets (so J is finite), then the union $\cup _ { j \in J } \Omega _ { j }$ and intersection $\cap _ { j \in J } \Omega _ { j }$ are also measurable. 

(iv) (σ-algebra property) If $( \Omega _ { j } ) _ { j \in J }$ are any countable collection of measurable sets (so J is countable), then the union $\mathsf { U } _ { j \in J } \Omega _ { j }$ and intersection $\cap _ { j \in J } \Omega _ { j }$ are also measurable. 

Note that some of these properties are redundant; for instance, (iv) will imply (iii), and once one knows all open sets are measurable, (ii) will imply that all closed sets are measurable also. The properties (i-iv) will ensure that virtually every set one cares about is measurable; though as indicated in the introduction, there do exist non-measurable sets. 

To every measurable set Ω, we associate the Lebesgue measure $m ( \Omega )$ of Ω, which will obey the following properties: 

(v) (Empty set) The empty set $\varnothing$ has measure $m ( \emptyset ) = 0$ 

(vi) (Positivity) We have $0 \leq m ( \Omega ) \leq + \infty$ for every measurable set $\Omega$ (vii) (Monotonicity) If $A \subseteq B$ , and A and B are both measurable, then $m ( A ) \leq m ( B )$ 

(viii) (Finite sub-additivity) If $( A _ { j } ) _ { j \in J }$ are a finite collection of measurable sets, then $\begin{array} { r } { m ( \bigcup _ { j \in J } A _ { j } ) \leq \sum _ { j \in J } m ( A _ { j } ) } \end{array}$ 

(ix) (Finite additivity) If $( A _ { j } ) _ { j \in J }$ are a finite collection of disjoint measurable sets, then $\begin{array} { r } { m ( \bigcup _ { j \in J } A _ { j } ) = \sum _ { j \in J } m ( A _ { j } ) } \end{array}$ 

(x) (Countable sub-additivity) If $( A _ { j } ) _ { j \in J }$ are a countable collection of measurable sets, then $\begin{array} { r } { m ( \bigcup _ { j \in J } \bar { A _ { j } } ) \leq \sum _ { j \in J } m ( A _ { j } ) } \end{array}$ 

(xi) (Countable additivity) If $( A _ { j } ) _ { j \in J }$ are a countable collection of disjoint measurable sets, then $\begin{array} { r } { m ( \bigcup _ { j \in J } A _ { j } ) = \sum _ { j \in J } m ( A _ { j } ) } \end{array}$ 

(xii) (Normalization) The unit cube $[ 0 , 1 ] ^ { n } = \{ ( x _ { 1 } , \ldots , x _ { n } ) \in \mathbf { R } ^ { n } : 0 \leq$ $x _ { j } \leq 1$ for all $1 \leq j \leq n \}$ has measure $m ( [ 0 , 1 ] ^ { n } ) = 1$ 

(xiii) (Translation invariance) If Ω is a measurable set, and $\boldsymbol { x } \in \mathbf { R } ^ { n }$ , then $x + \Omega : = \{ x + y : y \in \Omega \}$ is also measurable, and $m ( x + \Omega ) = m ( \Omega )$ 

Again, many of these properties are redundant; for instance the countable additivity property can be used to deduce the finite additivity property, which in turn can be used to derive monotonicity (when combined with the positivity property). One can also obtain the subadditivity properties from the additivity ones. Note that $m ( \Omega )$ can be $+ \infty$ , and so in particular some of the sums in the above properties may also equal $+ \infty$ . (Since everything is positive we will never have to deal with indeterminate forms such as $- \infty + + \infty . )$ 

Our goal for this chapter can then be stated thus: 

Theorem 7.1.1 (Existence of Lebesgue measure). . There exists a concept of a measurable set, and a way to assign a number $m ( \Omega )$ to every measurable subset $\Omega \subseteq \mathbf { R } ^ { n }$ , which obeys all of the properties $( i ) -$ (xiii). 

It turns out that Lebesgue measure is pretty much unique; any other concept of measurability and measure which obeys axioms $( \mathrm { i } ) \mathrm { - } ( \mathrm { x i i i } )$ will largely coincide with the construction we give. However there are other measures which obey only some of the above axioms; also, we may be interested in concepts of measure for other domains than Euclidean spaces $\mathbf { R } ^ { n }$ . This leads to measure theory, which is an entire subject in itself and will not be pursued here; however we do remark that the concept of measures is very important in modern probability, and in the finer points of analysis (e.g., in the theory of distributions). 

## 7.2 First attempt: Outer measure

Before we construct Lebesgue measure, we first discuss a somewhat naive approach to finding the measure of a set - namely, we try to cover the set by boxes, and then add up the volume of each box. This approach will almost work, giving us a concept called outer measure which can be applied to every set and obeys all of the properties (v)-(xiii) except for the additivity properties (ix), (xi). Later we will have to modify outer measure slightly to recover the additivity property. 

We begin by starting with the notion of an open box. 

Definition 7.2.1 (Open box). An open box (or box for short) B in $\mathbf { R } ^ { n }$ is any set of the form 

$$
B = \prod_ {i = 1} ^ {n} (a _ {i}, b _ {i}) := \{(x _ {1}, \dots , x _ {n}) \in \mathbf {R} ^ {n}: x _ {i} \in (a _ {i}, b _ {i}) \text {   for   all   } 1 \leq i \leq n \},
$$

where $b _ { i } \geq a _ { i }$ are real numbers. We define the volume vol(B) of this box to be the number 

$$
\operatorname{vol} (B) := \prod_ {i = 1} ^ {n} \left(b _ {i} - a _ {i}\right) = \left(b _ {1} - a _ {1}\right) \left(b _ {2} - a _ {2}\right) \dots \left(b _ {n} - a _ {n}\right).
$$

For instance, the unit cube $( 0 , 1 ) ^ { n }$ is a box, and has volume 1. In one dimension $n = 1$ , boxes are the same as open intervals. One can easily check that in general dimension that open boxes are indeed open. Note that if we have $b _ { i } = a _ { i }$ for some i, then the box becomes empty, and has volume 0, but we still consider this to be a box (albeit a rather silly one). Sometimes we will use ${ \mathrm { v o l } } _ { n } ( B )$ instead of vol(B) to emphasize that we are dealing with n-dimensional volume, thus for instance ${ \mathrm { v o l } } _ { 1 } ( B )$ would be the length of a one-dimensional box B, $\mathrm { v o l } _ { 2 } ( B )$ would be the area of a two-dimensional box B, etc. 

Remark 7.2.2. We of course expect the measure $m ( B )$ of a box to be the same as the volume vol(B) of that box. This is in fact an inevitable consequence of the axioms (i)-(xiii) (see Exercise 7.2.5). 

Definition 7.2.3 (Covering by boxes). Let $\Omega \subseteq \mathbf { R } ^ { n }$ be a subset of $\mathbf { R } ^ { n }$ We say that a collection $( B _ { j } ) _ { j \in J }$ of boxes cover Ω if $\textstyle \Omega \subseteq \bigcup _ { j \in J } B _ { j }$ 

Suppose $\Omega \subseteq \mathbf { R } ^ { n }$ can be covered by a finite or countable collection of boxes $( B _ { j } ) _ { j \in J }$ . If we wish $\Omega$ to be measurable, and if we wish to have a measure obeying the monotonicity and sub-additivity properties (vii), (viii), (x) and if we wish m $( B _ { j } ) = \mathrm { v o l } ( B _ { j } )$ for every box $j ,$ , then we must have 

$$
m (\Omega) \leq m \left(\bigcup_ {j \in J} B _ {j}\right) \leq \sum_ {j \in J} m (B _ {j}) = \sum_ {j \in J} \operatorname{vol} (B _ {j}).
$$

We thus conclude 

$$
m (\Omega) \leq \inf \left\{\sum_ {j \in J} \operatorname{vol} (B _ {j}): (B _ {j}) _ {j \in J} \text {   covers   } \Omega ; J \text {   at   most   countable } \right\}.
$$

Inspired by this, we define 

Definition 7.2.4 (Outer measure). If Ω is a set, we define the outer measure $m ^ { * } ( \Omega )$ of Ω to be the quantity 

$$
m ^ {*} (\Omega) := \inf \left\{\sum_ {j \in J} \operatorname{vol} (B _ {j}): (B _ {j}) _ {j \in J} \text {   covers   } \Omega ; J \text {   at   most   countable } \right\}.
$$

Since $\scriptstyle \sum _ { j = 1 } ^ { \infty } { \mathrm { v o l } } ( B _ { j } )$ is non-negative, we know that $m ^ { * } ( \Omega ) \geq 0$ for all $\Omega .$ . However, it is quite possible that $m ^ { * } ( \Omega )$ could equal + . Note that because we are allowing ourselves to use a countable number of boxes, that every subset of $\mathbf { R } ^ { n }$ has at least one countable cover by boxes; in fact $\mathbf { R } ^ { n }$ itself can be covered by countably many translates of the unit cube $( 0 , 1 ) ^ { n }$ (how?). We will sometimes write $m _ { n } ^ { * } ( \Omega )$ instead of $m ^ { * } ( \Omega )$ to emphasize the fact that we are using n-dimensional outer measure. 

Note that outer measure can be defined for every single set (not just the measurable ones), because we can take the infimum of any non-empty set. It obeys several of the desired properties of a measure: 

Lemma 7.2.5 (Properties of outer measure). Outer measure has the following six properties: 

(v) (Empty set) The empty set $\varnothing$ has outer measure $m ^ { * } ( \varnothing ) = 0$ 

(vi) (Positivity) We have $0 \leq m ^ { * } ( \Omega ) \leq + \infty$ for every measurable set Ω. 

(vii) (Monotonicity) If $A \subseteq B \subseteq \mathbf { R } ^ { n }$ , then $m ^ { * } ( A ) \leq m ^ { * } ( B )$ 

(viii) (Finite sub-additivity) If $( A _ { j } ) _ { j \in J }$ are a finite collection of subsets of $\mathbf { R } ^ { n }$ , then $\begin{array} { r } { m ^ { * } ( \bigcup _ { j \in J } A _ { j } ) \leq \sum _ { j \in J } m ^ { * } ( A _ { j } ) } \end{array}$ 

(x) (Countable sub-additivity) I $f ( A _ { j } ) _ { j \in J }$ are a countable collection of subsets of $\mathbf { R } ^ { n }$ , then $\begin{array} { r } { m ^ { * } ( \bigcup _ { j \in J } A _ { j } ) \leq \sum _ { j \in J } m ^ { * } ( A _ { j } ) } \end{array}$ 

(xiii) (Translation invariance) If Ω is a subset of $\mathbf { R } ^ { n }$ , and $\boldsymbol { x } \in \mathbf { R } ^ { n }$ , then $m ^ { * } ( x + \Omega ) = m ^ { * } ( \Omega )$ 

Proof. See Exercise 7.2.1. 

The outer measure of a closed box is also what we expect: 

Proposition 7.2.6 (Outer measure of closed box). For any closed box 

$$
B = \prod_ {i = 1} ^ {n} [ a _ {i}, b _ {i} ] := \{(x _ {1}, \dots , x _ {n}) \in \mathbf {R} ^ {n}: x _ {i} \in [ a _ {i}, b _ {i} ] f o r a l l 1 \leq i \leq n \},
$$

we have 

$$
m ^ {*} (B) = \prod_ {i = 1} ^ {n} (b _ {i} - a _ {i}).
$$

Proof. Clearly, we can cover the closed box $\begin{array} { r } { B = \prod _ { i = 1 } ^ { n } [ a _ { i } , b _ { i } ] } \end{array}$ by the open box $\textstyle \prod _ { i = 1 } ^ { n } ( a _ { i } - \varepsilon , b _ { i } + \varepsilon )$ for every $\varepsilon > 0$ . Thus we have 

$$
m ^ {*} (B) \leq \operatorname{vol} \left(\prod_ {i = 1} ^ {n} \left(a _ {i} - \varepsilon , b _ {i} + \varepsilon\right)\right) = \prod_ {i = 1} ^ {n} \left(b _ {i} - a _ {i} + 2 \varepsilon\right)
$$

for every $\varepsilon > 0$ . Taking limits as $\varepsilon \to 0$ , we obtain 

$$
m ^ {*} (B) \leq \prod_ {i = 1} ^ {n} (b _ {i} - a _ {i}).
$$

To finish the proof, we need to show that 

$$
m ^ {*} (B) \geq \prod_ {i = 1} ^ {n} (b _ {i} - a _ {i}).
$$

By the definition of $m ^ { * } ( B )$ , it sufices to show that 

$$
\sum_ {j \in J} \operatorname{vol} (B _ {j}) \geq \prod_ {i = 1} ^ {n} (b _ {i} - a _ {i})
$$

whenever $( B _ { j } ) _ { j \in J }$ is a finite or countable cover of B. 

Since B is closed and bounded, it is compact (by the Heine-Borel theorem, Theorem 1.5.7), and in particular every open cover has a finite subcover (Theorem 1.5.8). Thus to prove the above inequality for countable covers, it sufices to do it for finite covers (since if $( B _ { j } ) _ { j \in J ^ { \prime } }$ is a finite subcover of $( B _ { j } ) _ { j \in J }$ then $\sum _ { j \in J } { \mathrm { v o l } } ( B _ { j } )$ will be greater than or equal to $\textstyle \sum _ { j \in J ^ { \prime } } \operatorname { v o l } ( B _ { j } ) )$ 

To summarize, our goal is now to prove that 

$$
\sum_ {j \in J} \operatorname{vol} (B ^ {(j)}) \geq \prod_ {i = 1} ^ {n} (b _ {i} - a _ {i})\tag{7.1}
$$

whenever $( B ^ { ( j ) } ) _ { j \in J }$ is a finite cover of $\textstyle \prod _ { j = 1 } ^ { n } [ a _ { i } , b _ { i } ]$ ; we have changed the subscript $B _ { j }$ to superscript $B ^ { ( j ) }$ because we will need the subscripts to denote components. 

To prove the inequality (7.1), we shall use induction on the dimension n. First we consider the base case $n = 1$ . Here B is just a closed interval $B = [ a , b ]$ , and each box $B ^ { ( j ) }$ is just an open interval $B ^ { ( j ) } = ( a _ { j } , b _ { j } )$ . We have to show that 

$$
\sum_ {j \in J} (b _ {j} - a _ {j}) \geq (b - a).
$$

To do this we use the Riemann integral. For each $j \in J$ , let $f ^ { ( j ) } : { \mathbf { R } }  { \mathbf { R } }$ be the function such that $f ^ { ( j ) } ( x ) = 1$ when $x \in ( a _ { j } , b _ { j } )$ and $f ^ { ( j ) } ( x ) = 0$ otherwise. Then we have that $f ^ { ( j ) }$ is Riemann integrable (because it is piecewise constant, and compactly supported) and 

$$
\int_ {- \infty} ^ {\infty} f ^ {(j)} = b _ {j} - a _ {j}.
$$

Summing this over all $j \in J$ , and interchanging the integral with the finite sum, we have 

$$
\int_ {- \infty} ^ {\infty} \sum_ {j \in J} f ^ {(j)} = \sum_ {j \in J} b _ {j} - a _ {j}.
$$

But since the intervals $( a _ { j } , b _ { j } )$ cover $[ a , b ]$ , we have $\begin{array} { r } { \sum _ { i \in J } f ^ { ( j ) } ( x ) \geq 1 } \end{array}$ for all $x \in [ a , b ] \ ( \mathrm { w h y ? } )$ . For all other values if $x ,$ we have $\begin{array} { r } { \sum _ { j \in J } f ^ { ( j ) } ( x ) \ge 0 } \end{array}$ Thus 

$$
\int_ {- \infty} ^ {\infty} \sum_ {j \in J} f ^ {(j)} \geq \int_ {[ a, b ]} 1 = b - a
$$

and the claim follows by combining this inequality with the previous equality. This proves $( 7 . 1 )$ when $n = 1$ 

Now assume inductively that $n > 1$ , and we have already proven the inequality (7.1) for dimensions $n - 1$ . We shall use a similar argument to the preceding one. Each box $B ^ { ( j ) }$ is now of the form 

$$
B ^ {(j)} = \prod_ {i = 1} ^ {n} (a _ {i} ^ {(j)}, b _ {i} ^ {(j)}).
$$

We can write this as 

$$
B ^ {(j)} = A ^ {(j)} \times (a _ {n} ^ {(j)}, b _ {n} ^ {(j)})
$$

where $A ^ { ( j ) }$ is the n 1-dimensional box $\begin{array} { r } { A ^ { ( j ) } : = \prod _ { i = 1 } ^ { n - 1 } ( a _ { i } ^ { ( j ) } , b _ { i } ^ { ( j ) } ) } \end{array}$ . Note that 

$$
\mathrm{vol} (B ^ {(j)}) = \mathrm{vol} _ {n - 1} (A ^ {(j)}) (b _ {n} ^ {(j)} - a _ {n} ^ {(j)})
$$

where we have subscripted $\mathrm { v o l } _ { n - 1 }$ by $n - 1$ to emphasize that this is n 1-dimensional volume being referred to here. We similarly write 

$$
B = A \times [ a _ {n}, b _ {n} ]
$$

where $\begin{array} { r } { A : = \prod _ { i = 1 } ^ { n - 1 } [ a _ { i } , b _ { i } ] } \end{array}$ , and again note that 

$$
\operatorname{vol} (B) = \operatorname{vol} _ {n - 1} (A) (b _ {n} - a _ {n}).
$$

For each $j ~ \in ~ J ,$ , let $f ^ { ( j ) }$ be the function such that $f ^ { ( j ) } ( x _ { n } ) \ =$ $\operatorname { v o l } _ { n - 1 } ( A ^ { ( j ) } )$ for all $x _ { n } \in ( a _ { n } ^ { ( j ) } , b _ { n } ^ { ( j ) } )$ , and $f ^ { ( j ) } ( x _ { n } ) = 0$ for all other $x _ { n }$ Then $f ^ { ( j ) }$ is Riemann integrable and 

$$
\int_ {- \infty} ^ {\infty} f ^ {(j)} = \mathrm{vol} _ {n - 1} (A ^ {(j)}) (b _ {n} ^ {(j)} - a _ {n} ^ {(j)}) = \mathrm{vol} (B ^ {(j)})
$$

and hence 

$$
\sum_ {j \in J} \operatorname{vol} (B ^ {(j)}) = \int_ {- \infty} ^ {\infty} \sum_ {j \in J} f ^ {(j)}.
$$

Now let $x _ { n } \in [ a _ { n } , b _ { n } ]$ and $( x _ { 1 } , \ldots , x _ { n - 1 } ) \in A$ . Then $( x _ { 1 } , \ldots , x _ { n } )$ lies in B, and hence lies in one of the $B ^ { ( j ) }$ . Clearly we have $x _ { n } \in ( a _ { n } ^ { ( j ) } , b _ { n } ^ { ( j ) } )$ , and $( x _ { 1 } , \dotsc , x _ { n - 1 } ) \in A ^ { ( j ) }$ . In particular, we see that for each $x _ { n } \in [ a _ { n } , b _ { n } ]$ the set 

$$
\{A ^ {(j)}: j \in J; x _ {n} \in (a _ {n} ^ {(j)}, b _ {n} ^ {(j)}) \}
$$

of n 1-dimensional boxes covers A. Applying the inductive hypothesis (7.1) at dimension $n - 1$ we thus see that 

$$
\sum_ {j \in J: x _ {n} \in (a _ {n} ^ {(j)}, b _ {n} ^ {(j)})} \operatorname{vol} _ {n - 1} (A ^ {(j)}) \geq \operatorname{vol} _ {n - 1} (A),
$$

or in other words 

$$
\sum_ {j \in J} f ^ {(j)} (x _ {n}) \geq \operatorname{vol} _ {n - 1} (A).
$$

Integrating this over $[ a _ { n } , b _ { n } ]$ , we obtain 

$$
\int_ {[ a _ {n}, b _ {n} ]} \sum_ {j \in J} f ^ {(j)} \geq \operatorname{vol} _ {n - 1} (A) (b _ {n} - a _ {n}) = \operatorname{vol} (B)
$$

and in particular 

$$
\int_ {- \infty} ^ {\infty} \sum_ {j \in J} f ^ {(j)} \geq \operatorname{vol} _ {n - 1} (A) (b _ {n} - a _ {n}) = \operatorname{vol} (B)
$$

since $\textstyle \sum _ { j \in J } f ^ { ( j ) }$ is always non-negative. Combining this with our previous identity for $\textstyle { \int _ { - \infty } ^ { \infty } \sum _ { j \in J } f ^ { ( j ) } }$ we obtain (7.1), and the induction is complete. □ 

Once we obtain the measure of a closed box, the corresponding result for an open box is easy: 

## Corollary 7.2.7. For any open box

$$
B = \prod_ {i = 1} ^ {n} (a _ {i}, b _ {i}) := \{(x _ {1}, \dots , x _ {n}) \in \mathbf {R} ^ {n}: x _ {i} \in (a _ {i}, b _ {i}) f o r a l l 1 \leq i \leq n \},
$$

we have 

$$
m ^ {*} (B) = \prod_ {i = 1} ^ {n} (b _ {i} - a _ {i}).
$$

In particular, outer measure obeys the normalization (xii). 

Proof. We may assume that $b _ { i } > a _ { i }$ for all i, since if $b _ { i } = a _ { i }$ this follows from Lemma $7 . 2 . 5 ( \mathrm { v } )$ . Now observe that 

$$
\prod_ {i = 1} ^ {n} \left[ a _ {i} + \varepsilon , b _ {i} - \varepsilon \right] \subset \prod_ {i = 1} ^ {n} \left(a _ {i}, b _ {i}\right) \subset \prod_ {i = 1} ^ {n} \left[ a _ {i}, b _ {i} \right]
$$

for all $\varepsilon > 0$ , assuming that ε is small enough that $b _ { i } - \varepsilon > a _ { i } + \varepsilon$ for all i. Applying Proposition 7.2.6 and Lemma 7.2.5(vii) we obtain 

$$
\prod_ {i = 1} ^ {n} (b _ {i} - a _ {i} - 2 \varepsilon) \leq m ^ {*} \left(\prod_ {i = 1} ^ {n} (a _ {i}, b _ {i})\right) \leq \prod_ {i = 1} ^ {n} (b _ {i} - a _ {i}).
$$

Sending $\varepsilon \to 0$ and using the squeeze test (Corollary 6.4.14), one obtains the result. □ 

We now compute some examples of outer measure on the real line R. 

Example 7.2.8. Let us compute the one-dimensional measure of R. Since $( - R , R ) \subset { \bf R }$ for all $R > 0$ , we have 

$$
m ^ {*} (\mathbf {R}) \geq m ^ {*} ((- R, R)) = 2 R
$$

by Corollary 7.2.7. Letting $R \to + \infty$ we thus see that $m ^ { * } ( { \bf R } ) = + \infty$ 

Example 7.2.9. Now let us compute the one-dimensional measure of Q. From Proposition 7.2.6 we see that for each rational number Q, the point $\{ { q } \}$ has outer measure $m ^ { * } ( \{ q \} ) = 0$ . Since Q is clearly the union $\begin{array} { r } { \mathbf { Q } = \bigcup _ { q \in \mathbf { Q } } \{ q \} } \end{array}$ of all these rational points q, and $\mathbf { Q }$ is countable, we have 

$$
m ^ {*} (\mathbf {Q}) \leq \sum_ {q \in \mathbf {Q}} m ^ {*} (\{q \}) = \sum_ {q \in \mathbf {Q}} 0 = 0,
$$

and so $m ^ { * } ( Q )$ must equal zero. In fact, the same argument shows that every countable set has measure zero. (This, incidentally, gives another proof that the real numbers are uncountable, Corollary 8.3.4.) 

Remark 7.2.10. One consequence of the fact that $m ^ { * } ( \mathbf { Q } ) = 0$ is that given any $\varepsilon > 0$ , it is possible to cover the rationals Q by a countable number of intervals whose total length is less than ε. This fact is somewhat un-intuitive; can you find a more explicit way to construct such a countable covering of Q by short intervals? 

Example 7.2.11. Now let us compute the one-dimensional measure of the irrationals $\mathbf { R } \backslash \mathbf { Q }$ . From finite sub-additivity we have 

$$
m ^ {*} (\mathbf {R}) \leq m ^ {*} (\mathbf {R} \backslash \mathbf {Q}) + m ^ {*} (\mathbf {Q}).
$$

Since Q has outer measure 0, and $m ^ { * } ( \mathbf { R } )$ has outer measure $+ \infty$ , we thus see that the irrationals $\mathbf { R } \backslash \mathbf { Q }$ have outer measure + . A similar argument shows that $[ 0 , 1 ] \backslash \mathbf { Q }$ , the irrationals in [0, 1], have outer measure 1 (why?). 

Example 7.2.12. By Proposition 7.2.6, the unit interval [0, 1] in R has one-dimensional outer measure 1, but the unit interval $\{ ( x , 0 ) : 0 \leq x \leq$ 1 in $\mathbf { R } ^ { 2 }$ has two-dimensional outer measure 0. Thus one-dimensional outer measure and two-dimensional outer measure are quite diferent. Note that the above remarks and countable additivity imply that the entire x-axis of $\mathbf { R } ^ { 2 }$ has two-dimensional outer measure 0, despite the fact that R has infinite one-dimensional measure. 

## — Exercises —

Exercise 7.2.1. Prove Lemma 7.2.5. (Hint: you will have to use the definition of inf, and probably introduce a parameter ε. You may have to treat separately the cases when certain outer measures are equal to + . (viii) can be deduced from (x) and (v). For (x), label the index set J as $J = \{ j _ { 1 } , j _ { 2 } , j _ { 3 } , . . . \}$ , and for each $A _ { j }$ , pick a covering of $A _ { j }$ by boxes whose total volume is no larger than $m ^ { * } ( A _ { j } ) + \varepsilon / 2 ^ { j } . )$ 

Exercise 7.2.2. Let A be a subset of $\mathbf { R } ^ { n }$ , and let B be a subset of $\mathbf { R } ^ { m }$ . Note that the Cartesian product $\{ ( a , b ) : a \in A , b \in B \}$ is then a subset of $\mathbf { R } ^ { n + m }$ . Show that $m _ { n + m } ^ { * } ( A \times B ) \leq m _ { n } ^ { * } ( A ) m _ { m } ^ { * } ( B )$ . (It is in fact true that $m _ { n + m } ^ { * } ( A \times B ) =$ $m _ { n } ^ { * } ( A ) m _ { m } ^ { * } ( B )$ , but this is substantially harder to prove). 

In Exercises 7.2.3-7.2.5, we assume that $\mathbf { R } ^ { n }$ is a Euclidean space, and we have a notion of measurable set in $\mathbf { R } ^ { n }$ (which may or may not coincide with the notion of Lebesgue measurable set) and a notion of measure (which may or may not co-incide with Lebesgue measure) which obeys axioms (i)-(xiii). 

Exercise 7.2.3. 

(a) Show that if $A _ { 1 } \subseteq A _ { 2 } \subseteq A _ { 3 } \dots$ . is an increasing sequence of measurable sets (so $A _ { j } ~ \subseteq ~ A _ { j + 1 }$ for every positive integer j), then we have $m ( \bigcup _ { j = 1 } ^ { \infty } A _ { j } ) = \bar { \operatorname* { l i m } } _ { j \to \infty } \bar { m } ( A _ { j } )$ 

(b) Show that if $A _ { 1 } \supseteq A _ { 2 } \supseteq A _ { 3 } \ldots$ . is a decreasing sequence of measurable sets (so $A _ { j } \supseteq A _ { j + 1 }$ for every positive integer j), and $m ( A _ { 1 } ) < + \infty$ , then we have $\begin{array} { r } { \dot { m } ( \bigcap _ { j = 1 } ^ { \infty } A _ { j } ) = \operatorname* { l i m } _ { j \to \infty } m ( A _ { j } ) } \end{array}$ 

Exercise 7.2.4. Show that for any positive integer $q > 1$ , that the open box 

$$
(0, 1 / q) ^ {n} := \left\{\left(x _ {1}, \dots , x _ {n}\right) \in \mathbf {R} ^ {n}: 0 <   x _ {j} <   1 / q \text {   for   all   } 1 \leq j \leq n \right\}
$$

and the closed box 

$$
[ 0, 1 / q ] ^ {n} := \left\{\left(x _ {1}, \dots , x _ {n}\right) \in \mathbf {R} ^ {n}: 0 \leq x _ {j} \leq 1 / q \text {   for   all   } 1 \leq j \leq n \right\}
$$

both measure $q ^ { - n }$ . (Hint: first show that $m ( ( 0 , 1 / q ) ^ { n } ) \leq q ^ { - n }$ for every $q \geq 1$ by covering $( 0 , 1 ) ^ { n }$ by some translates of $( 0 , 1 / q ) ^ { n }$ . Using a similar argument, show that $m ( [ 0 , 1 / q ] ^ { n } ) \geq q ^ { - n }$ . Then show that m $( [ 0 , 1 / q ] ^ { n } \backslash ( 0 , 1 / q ) ^ { n } ) \leq \varepsilon$ for every $\varepsilon > 0$ , by covering the boundary of $[ 0 , 1 / q ] ^ { n }$ with some very small boxes.) 

Exercise 7.2.5. Show that for any box B, that $m ( B ) = \operatorname { v o l } ( B )$ . (Hint: first prove this when the co-ordinates $a _ { j } , b _ { j }$ are rational, using Exercise 7.2.4. Then take limits somehow (perhaps using Q1) to obtain the general case when the co-ordinates are real.) 

Exercise 7.2.6. Use Lemma 7.2.5 and Proposition 7.2.6 to furnish another proof that the reals are uncountable (i.e., reprove Corollary 8.3.4). 

## 7.3 Outer measure is not additive

In light of Lemma 7.2.5, it would seem now that all we need to do is to verify the additivity properties (ix), (xi), and we have everything we need to have a usable measure. Unfortunately, these properties fail for outer measure, even in one dimension. 

Proposition 7.3.1 (Failure of countable additivity). There exists a countable collection $( A _ { j } ) _ { j \in J }$ of disjoint subsets of R, such that $\begin{array} { r } { m ^ { * } ( \bigcup _ { j \in J } A _ { j } ) \neq \sum _ { j \in J } m ^ { * } ( A _ { j } ) } \end{array}$ 

Proof. We shall need some notation. Let Q be the rationals, and R be the reals. We say that a set $A \subset \mathbf { R }$ is a coset of Q if it is of the form $A = x + \mathbf { Q }$ for some real number x. For instance, ${ \sqrt { 2 } } + \mathbf { Q }$ is a coset of R, as is Q itself, since $\mathbf { Q } = 0 + \mathbf { Q }$ . Note that a coset A can correspond to several values of $x ;$ for instance $2 + \mathbf { Q }$ is exactly the same coset as $0 + \mathbf { Q }$ Also observe that it is not possible for two cosets to partially overlap; if $x + \mathbf { Q }$ intersects $y + \mathbf { Q }$ in even just a single point z, then $x - y$ must be rational (why? use the identity $x - y = ( x - z ) - ( y - z ) )$ , and thus $x + \mathbf { Q }$ and $y + \mathbf { Q }$ must be equal (why?). So any two cosets are either identical or distinct. 

We observe that every coset A of the rationals R has a non-empty intersection with [0, 1]. Indeed, if A is a coset, then $A = x + \mathbf { Q }$ for some real number x. If we then pick a rational number $q$ in $[ - x , 1 - x ]$ then we see that $x + q \in [ 0 , 1 ]$ , and thus $A \cap [ 0 , 1 ]$ contains $x + q$ 

Let $\mathbf { R } / \mathbf { Q }$ denote the set of all cosets of $\mathbf { Q } ;$ note that this is a set whose elements are themselves sets (of real numbers). For each coset A in $\mathbf { R } / \mathbf { Q }$ , let us pick an element $x _ { A }$ of $A \cap [ 0 , 1 ]$ . (This requires us to make an infinite number of choices, and thus requires the axiom of choice, see Section 8.4.) Let E be the set of all such $x _ { A }$ , i.e., $E : = \{ x _ { A } : A \in \mathbf { R } / \mathbf { Q } \}$ Note that $E \subseteq [ 0 , 1 ]$ by constrution. 

Now consider the set 

$$
X = \bigcup_ {q \in \mathbf {Q} \cap [ - 1, 1 ]} (q + E).
$$

Clearly this set is contained in $[ - 1 , 2 ]$ (since $q + x \in [ - 1 , 2 ]$ whenever $q \in [ - 1 , 1 ]$ and $x \in E \subseteq [ 0 , 1 ] )$ . We claim that this set contains the interval [0, 1]. Indeed, for any $y \in [ 0 , 1 ]$ , we know that y must belong to some coset A (for instance, it belongs to the coset $y + \mathbf { Q } )$ . But we also have $x _ { A }$ belonging to the same coset, and thus $y - x _ { A }$ is equal to some rational q. Since y and $x _ { A }$ both live in [0, 1], then q lives in $[ - 1 , 1 ]$ Since $y = q + x _ { A }$ , we have $y \in q + E$ , and hence $y \in X$ as desired. 

We claim that 

$$
m ^ {*} (X) \neq \sum_ {q \in \mathbf {Q} \cap [ - 1, 1 ]} m ^ {*} (q + E),
$$

which would prove the claim. To see why this is true, observe that since $[ 0 , 1 ] \subseteq X \subseteq [ - 1 , 2 ]$ , that we have $1 \leq m ^ { * } ( X ) \leq 3$ by monotonicity and Proposition 7.2.6. For the right hand side, observe from translation invariance that 

$$
\sum_ {q \in \mathbf {Q} \cap [ - 1, 1 ]} m ^ {*} (q + E) = \sum_ {q \in \mathbf {Q} \cap [ - 1, 1 ]} m ^ {*} (E).
$$

The set ${ \bf Q } \cap [ - 1 , 1 ]$ is countably infinite (why?). Thus the right-hand side is either 0 (if $m ^ { * } ( E ) = 0 )$ or $+ \infty \ ( \mathrm { i f } \ m ^ { * } ( E ) > 0 )$ . Either way, it cannot be between 1 and 3, and the claim follows. □ 

Remark 7.3.2. The above proof used the axiom of choice. This turns out to be absolutely necessary; one can prove using some advanced techniques in mathematical logic that if one does not assume the axiom of choice, then it is possible to have a mathematical model where outer measure is countably additive. 

One can refine the above argument, and show in fact that $m ^ { * }$ is not finitely additive either: 

Proposition 7.3.3 (Failure of finite additivity). There exists a finite collection $( A _ { j } ) _ { j \in J }$ of disjoint subsets of R, such that 

$$
m ^ {*} \left(\bigcup_ {j \in J} A _ {j}\right) \neq \sum_ {j \in J} m ^ {*} (A _ {j}).
$$

Proof. This is accomplished by an indirect argument. Suppose for sake of contradiction that $m ^ { * }$ was finitely additive. Let E and X be the sets introduced in Proposition 7.3.1. From countable sub-additivity and translation invariance we have 

$$
m ^ {*} (X) \leq \sum_ {q \in \mathbf {Q} \cap [ - 1, 1 ]} m ^ {*} (q + E) = \sum_ {q \in \mathbf {Q} \cap [ - 1, 1 ]} m ^ {*} (E).
$$

Since we know that $1 \leq m ^ { * } ( X ) \leq 3$ , we thus have $m ^ { * } ( E ) \neq 0$ , since otherwise we would have $m ^ { * } ( X ) \leq 0$ , a contradiction. 

Since $m ^ { * } ( E ) \neq 0 .$ , there exists a finite integer $n ~ > ~ 0$ such that $m ^ { * } ( E ) > 1 / n$ . Now let J be a finite subset of $\mathbf { Q } \cap [ - 1 , 1 ]$ of cardinality 3n. If $m ^ { * }$ were finitely additive, then we would have 

$$
m ^ {*} \left(\sum_ {q \in J} q + E\right) = \sum_ {q \in J} m ^ {*} (q + E) = \sum_ {q \in J} m ^ {*} (E) > 3 n \frac {1}{n} = 3.
$$

But we know that $\textstyle \sum _ { q \in J } q + E$ is a subset of X, which has outer measure at most 3. This contradicts monotonicity. Hence $m ^ { * }$ cannot be finitely additive. □ 

Remark 7.3.4. The examples here are related to the Banach-Tarski paradox, which demonstrates (using the axiom of choice) that one can partition the unit ball in $\mathbf { R } ^ { 3 }$ into a finite number of pieces which, when rotated and translated, can be reassembled to form two complete unit balls! Of course, this partition involves non-measurable sets. We will not present this paradox here as it requires some group theory which is beyond the scope of this text. 

## 7.4 Measurable sets

In the previous section we saw that certain sets were badly behaved with respect to outer measure, in particular they could be used to contradict finite or countable additivity. However, those sets were rather pathological, being constructed using the axiom of choice and looking rather artificial. One would hope to be able to exclude them and then somehow recover finite and countable additivity. Fortunately, this can be done, thanks to a clever definition of Constantin Carath´eodory (1873–1950): 

Definition 7.4.1 (Lebesgue measurability). Let E be a subset of $\mathbf { R } ^ { n }$ We say that E is Lebesgue measurable, or measurable for short, if we have the identity 

$$
m ^ {*} (A) = m ^ {*} (A \cap E) + m ^ {*} (A \backslash E)
$$

for every subset A of $\mathbf { R } ^ { n }$ . If E is measurable, we define the Lebesgue measure of E to be $m ( E ) = m ^ { * } ( E )$ ; if E is not measurable, we leave $m ( E )$ undefined. 

In other words, E being measurable means that if we use the set E to divide up an arbitrary set A into two parts, we keep the additivity property. Of course, if $m ^ { * }$ were finitely additive then every set E would be measurable; but we know from Proposition 7.3.3 that not every set is finitely additive. One can think of the measurable sets as the sets for which finite additivity works. We sometimes subscript $m ( E )$ as $m _ { n } ( E )$ to emphasize the fact that we are using n-dimensional Lebesgue measure. 

The above definition is somewhat hard to work with, and in practice one does not verify a set is measurable directly from this definition. Instead, we will use this definition to prove various useful properties of measurable sets (Lemmas 7.4.2-7.4.11), and after that we will rely more or less exclusively on the properties in those lemmas, and no longer need to refer to the above definition. 

We begin by showing that a large number of sets are indeed measurable. The empty set $E = \emptyset$ and the whole space $E = \mathbf { R } ^ { n }$ are clearly measurable (why?). Here is another example of a measurable set: 

Lemma 7.4.2 (Half-spaces are measurable). The half-space 

$$
\{(x _ {1}, \dots , x _ {n}) \in \mathbf {R} ^ {n}: x _ {n} > 0 \}
$$

is measurable. 

Proof. See Exercise 7.4.3. 

Remark 7.4.3. A similar argument will also show that any half-space of the form $\left\{ \left( x _ { 1 } , \ldots , x _ { n } \right) \in \mathbf { R } ^ { n } : x _ { j } > 0 \right\} { \mathrm { o r ~ } } \{ ( x _ { 1 } , \ldots , x _ { n } ) \in \mathbf { R } ^ { n } : x _ { j } < 0 \}$ for some $1 \leq j \leq n$ is measurable. 

Now for some more properties of measurable sets. 

Lemma 7.4.4 (Properties of measurable sets). 

(a) If E is measurable, then $\mathbf { R } ^ { n } \backslash E$ is also measurable. 

(b) (Translation invariance) If E is measurable, and $x \in \mathbf { R } ^ { n }$ , then $x + E$ is also measurable, and m $( x + E ) = m ( E )$ 

(c) If $E _ { 1 }$ and $E _ { 2 }$ are measurable, then $E _ { 1 } \cap E _ { 2 }$ and $E _ { 1 } \cup E _ { 2 }$ are measurable. 

(d) (Boolean algebra property) If $E _ { 1 } , E _ { 2 } , \dots , E _ { N }$ are measurable, then $\textstyle \bigcup _ { j = 1 } ^ { N } E _ { j }$ and $\textstyle \bigcap _ { j = 1 } ^ { N } E _ { j }$ are measurable. 

(e) Every open box, and every closed box, is measurable. 

(f) Any set E of outer measure zero $( i . e . , m ^ { * } ( E ) = 0 )$ is measurable. 

Proof. See Exercise 7.4.4. 

From Lemma 7.4.4, we have proven properties (ii), (iii), (xiii) on our wish list of measurable sets, and we are making progress towards (i). We also have finite additivity (property (ix) on our wish list): 

Lemma 7.4.5 (Finite additivity). If $( E _ { j } ) _ { j \in J }$ are a finite collection of disjoint measurable sets and any set A (not necessarily measurable), we have 

$$
m ^ {*} \left(A \cap \bigcup_ {j \in J} E _ {j}\right) = \sum_ {j \in J} m ^ {*} (A \cap E _ {j}).
$$

Furthermore, we have m $\begin{array} { r } { ( \bigcup _ { j \in J } E _ { j } ) = \sum _ { j \in J } m ( E _ { j } ) } \end{array}$ 

Proof. See Exercise 7.4.6. 

Remark 7.4.6. Lemma 7.4.5 and Proposition 7.3.3, when combined, imply that there exist non-measurable sets: see Exercise 7.4.5. 

Corollary 7.4.7. If $A \subseteq B$ are two measurable sets, then $B \backslash A$ is also measurable, and 

$$
m (B \backslash A) = m (B) - m (A).
$$

Proof. See Exercise 7.4.7. 

Now we show countable additivity. 

Lemma 7.4.8 (Countable additivity). If $( E _ { j } ) _ { j \in J }$ are a countable collection of disjoint measurable sets, then $\cup _ { j \in J } E _ { j }$ is measurable, and $\begin{array} { r } { m ( \bigcup _ { j \in J } E _ { j } ) = \sum _ { j \in J } m ( E _ { j } ) } \end{array}$ 

Proof. Let $\textstyle E : = \bigcup _ { j \in J } E _ { j }$ . Our first task will be to show that $E$ is measurable. Thus, let A be an arbitrary set (not necessarily measurable); we need to show that 

$$
m ^ {*} (A) = m ^ {*} (A \cap E) + m ^ {*} (A \backslash E).
$$

Since J is countable, we may write $J = \{ j _ { 1 } , j _ { 2 } , j _ { 3 } , . . . \}$ . Note that 

$$
A \cap E = \bigcup_ {k = 1} ^ {\infty} (A \cap E _ {j _ {k}})
$$

(why?) and hence by countable sub-additivity 

$$
m ^ {*} (A \cap E) \leq \sum_ {k = 1} ^ {\infty} m ^ {*} (A \cap E _ {j _ {k}}).
$$

We rewrite this as 

$$
m ^ {*} (A \cap E) \leq \sup _ {N \geq 1} \sum_ {k = 1} ^ {N} m ^ {*} (A \cap E _ {j _ {k}}).
$$

Let $F _ { N }$ be the set $\begin{array} { r } { F _ { N } : = \bigcup _ { k = 1 } ^ { N } E _ { j _ { k } } } \end{array}$ . Since the $A \cap E _ { j _ { k } }$ are all disjoint, and their union is $A \cap F _ { N }$ , we see from Lemma 7.4.5 that 

$$
\sum_ {k = 1} ^ {N} m ^ {*} (A \cap E _ {j _ {k}}) = m ^ {*} (A \cap F _ {N})
$$

and hence 

$$
m ^ {*} (A \cap E) \leq \sup _ {N \geq 1} m ^ {*} (A \cap F _ {N}).
$$

Now we look at $A \backslash E$ . Since $F _ { N } \subseteq E { \mathrm { ~ ( w h y ? ) } }$ , we have $A \backslash E \subseteq A \backslash F _ { N }$ $\mathrm { \left( w h y ? \right) }$ . By monotonicity, we thus have 

$$
m ^ {*} (A \backslash E) \leq m ^ {*} (A \backslash F _ {N})
$$

for all N. In particular, we see that 

$$
m ^ {*} (A \cap E) + m ^ {*} (A \backslash E) \leq \sup _ {N \geq 1} m ^ {*} (A \cap F _ {N}) + m ^ {*} (A \backslash E)
$$

$$
\leq \sup _ {N \geq 1} m ^ {*} (A \cap F _ {N}) + m ^ {*} (A \backslash F _ {N}).
$$

But from Lemma 7.4.5 we know that $F _ { N }$ is measurable, and hence 

$$
m ^ {*} (A \cap F _ {N}) + m ^ {*} (A \backslash F _ {N}) = m ^ {*} (A).
$$

Putting this all together we obtain 

$$
m ^ {*} (A \cap E) + m ^ {*} (A \backslash E) \leq m ^ {*} (A).
$$

But from finite sub-additivity we have 

$$
m ^ {*} (A \cap E) + m ^ {*} (A \backslash E) \geq m ^ {*} (A)
$$

and the claim follows. This shows that E is measurable. 

To finish the lemma, we need to show that $m ( E )$ is equal to $\textstyle \sum _ { j \in J } m ( E _ { j } )$ . We first observe from countable sub-additivity that 

$$
m (E) \leq \sum_ {j \in J} m (E _ {j}) = \sum_ {k = 1} ^ {\infty} m (E _ {j _ {k}}).
$$

On the other hand, by finite additivity and monotonicity we have 

$$
m (E) \geq m (F _ {N}) = \sum_ {k = 1} ^ {N} m (E _ {j _ {k}}).
$$

Taking limits as $N \to \infty$ we obtain 

$$
m (E) \geq \sum_ {k = 1} ^ {\infty} m (E _ {j _ {k}})
$$

and thus we have 

$$
m (E) = \sum_ {k = 1} ^ {\infty} m (E _ {j _ {k}}) = \sum_ {j \in J} m (E _ {j})
$$

as desired. 

This proves property (xi) on our wish list. Next, we do countable unions and intersections. 

Lemma 7.4.9 (σ-algebra property). If $( \Omega _ { j } ) _ { j \in J }$ are any countable collection of measurable sets (so J is countable), then the union $\cup _ { j \in J } \Omega _ { j }$ and the intersection $\cap _ { j \in J } \Omega _ { j }$ are also measurable. 

## 7.4. Measurable sets

## Proof. See Exercise 7.4.8.

The final property left to verify on our wish list is (a). We first need a preliminary lemma. 

Lemma 7.4.10. Every open set can be written as a countable or finite union of open boxes. 

Proof. We first need some notation. Call a box $\begin{array} { r } { B = \prod _ { i = 1 } ^ { n } ( a _ { i } , b _ { i } ) } \end{array}$ rational if all of its components $a _ { i } , b _ { i }$ are rational numbers. Observe that there are only a countable number of rational boxes (this is since a rational box is described by 2n rational numbers, and so has the same cardinality as $\mathbf { Q } ^ { 2 n }$ . But Q is countable, and the Cartesian product of any finite number of countable sets is countable; see Corollaries 8.1.14, 8.1.15). 

We make the following claim: given any open ball $B ( x , r )$ , there exists a rational box B which is contained in $B ( x , r )$ and which contains x. To prove this claim, write $x = ( x _ { 1 } , \ldots , x _ { n } )$ . For each $1 \leq i \leq n$ , let $a _ { i }$ and $b _ { i }$ be rational numbers such that 

$$
x _ {i} - \frac {r}{n} <   a _ {i} <   x _ {i} <   b _ {i} <   x _ {i} + \frac {r}{n}.
$$

Then it is clear that the box $\textstyle \prod _ { i = 1 } ^ { n } ( a _ { i } , b _ { i } )$ is rational and contains x. A simple computation using Pythagoras’ theorem (or the triangle inequal-$\mathrm { i t y ) }$ also shows that this box is contained in $B ( x , r )$ ; we leave this to the reader. 

Now let E be an open set, and let Σ be the set of all rational boxes B which are subsets of $E ,$ and consider the union $\cup _ { B \in \Sigma } B$ of all those boxes. Clearly, this union is contained in $E _ { \mathrm { { i } } }$ , since every box in Σ is contained in $E$ by construction. On the other hand, since E is open, we see that for every $x \in E$ there is a ball $B ( x , r )$ contained in $E _ { i }$ , and by the previous claim this ball contains a rational box which contains x. In particular, x is contained in $\cup _ { B \in \Sigma } B$ . Thus we have 

$$
E = \bigcup_ {B \in \Sigma} B
$$

as desired; note that $\Sigma$ is countable or finite because it is a subset of the set of all rational boxes, which is countable. □ 

Lemma 7.4.11 (Borel property). Every open set, and every closed set, is Lebesgue measurable. 

Proof. It sufices to do this for open sets, since the claim for closed sets then follows by Lemma 7.4.4(a) (i.e., property (ii)). Let E be an open set. By Lemma 7.4.10, E is the countable union of boxes. Since we already know that boxes are measurable, and that the countable union of measurable sets is measurable, the claim follows. □ 

The construction of Lebesgue measure and its basic properties are now complete. Now we make the next step in constructing the Lebesgue integral - describing the class of functions we can integrate. 

— Exercises — 

Exercise 7.4.1. If A is an open interval in R, show that $m ^ { * } ( A ) = m ^ { * } ( A \cap$ $( 0 , \infty ) ) + m ^ { * } ( A \backslash ( 0 , \infty ) )$ 

Exercise 7.4.2. If A is an open box in $\mathbf { R } ^ { n }$ , and E is the half-plane $E : =$ $\{ ( x _ { 1 } , \ldots , x _ { n } ) \in \mathbf { R } ^ { n } : x _ { n } > 0 \}$ , show that $m ^ { * } ( A ) = m ^ { * } ( A \cap E ) + m ^ { * } ( A \backslash E )$ (Hint: use Exercise 7.4.1.) 

Exercise 7.4.3. Prove Lemma 7.4.2. (Hint: use Exercise 7.4.2.) 

Exercise 7.4.4. Prove Lemma 7.4.4. (Hints: for (c), first prove that 

$$
m ^ {*} (A) = m ^ {*} \left(A \cap E _ {1} \cap E _ {2}\right) + m ^ {*} \left(A \cap E _ {1} \backslash E _ {2}\right) + m ^ {*} \left(A \cap E _ {2} \backslash E _ {1}\right) + m ^ {*} \left(A \backslash \left(E _ {1} \cup E _ {2}\right)\right).
$$

A Venn diagram may be helpful. Also you may need the finite sub-additivity property. Use (c) to prove (d), and use (bd) and the various versions of Lemma 7.4.2 to prove (e)). 

Exercise 7.4.5. Show that the set E used in the proof of Propositions 7.3.1 and 7.3.3 is non-measurable. 

Exercise 7.4.6. Prove Lemma 7.4.5. 

Exercise 7.4.7. Use Lemma 7.4.5 to prove Corollary 7.4.7. 

Exercise 7.4.8. Prove Lemma 7.4.9. (Hint: for the countable union problem, write $J = \{ j _ { 1 } , j _ { 2 } , . . . \}$ , write $\begin{array} { r } { F _ { N } : = \bigcup _ { k = 1 } ^ { N } \Omega _ { j _ { k } } } \end{array}$ , and write $E _ { N } : = F _ { N } \backslash F _ { N - 1 }$ , with the understanding that $F _ { 0 }$ is the empty set. Then apply Lemma 7.4.8. For the countable intersection problem, use what you just did and Lemma $7 . 4 . 4 ( \mathrm { a } ) . )$ 

Exercise 7.4.9. Let $A \subseteq \mathbf { R } ^ { 2 }$ be the set $A : = [ 0 , 1 ] ^ { 2 } \backslash { \bf Q } ^ { 2 }$ ; i.e A consists of all the points $( x , y )$ in $[ 0 , 1 ] ^ { 2 }$ such that x and y are not both rational. Show that 

## 7.5. Measurable functions

A is measurable and $m ( A ) = 1$ , but that A has no interior points. (Hint: it’s easier to use the properties of outer measure and measure, including those in the exercises above, than to try to do this problem from first principles.) 

Exercise 7.4.10. Let $A \subseteq B \subseteq \mathbf { R } ^ { n }$ . Show that if B is Lebesgue measurable with measure zero, then A is also Lebesgue measurable with measure zero. 

## 7.5 Measurable functions

In the theory of the Riemann integral, we are only able to integrate a certain class of functions - the Riemann integrable functions. We will now be able to integrate a much larger range of functions - the measurable functions. More precisely, we can only integrate those measurable functions which are absolutely integrable - but more on that later. 

Definition 7.5.1 (Measurable functions). Let Ω be a measurable subset of R<sup>n</sup>, and let $f : \Omega \to \mathbf { R } ^ { m }$ be a function. A function f is measurable if $f ^ { - 1 } ( V )$ is measurable for every open set $V \subseteq \mathbf { R } ^ { m }$ 

As discussed earlier, most sets that we deal with in real life are measurable, so it is only natural to learn that most functions we deal with in real life are also measurable. For instance, continuous functions are automatically measurable: 

Lemma 7.5.2 (Continuous functions are measurable). Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f : \Omega \to \mathbf { R } ^ { m }$ be continuous. Then f is also measurable. 

Proof. Let V be any open subset of $\mathbf { R } ^ { m }$ . Then since f is continuous, $f ^ { - 1 } ( V )$ is open relative to Ω (see Theorem 2.1.5(c)), i.e., $f ^ { - 1 } ( V ) = W \cap \Omega$ for some open set $W \subseteq \mathbf { R } ^ { n }$ (see Proposition 1.3.4(a)). Since W is open, it is measurable; since Ω is measurable, W Ω is also measurable. 

Because of Lemma 7.4.10, we have an easy criterion to test whether a function is measurable or not: 

Lemma 7.5.3. Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f : \Omega \to \mathbf { R } ^ { m }$ be a function. Then f is measurable if and only if $f ^ { - 1 } ( B )$ is measurable for every open box B. 

Proof. See Exercise 7.5.1. 

Corollary 7.5.4. Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f : \Omega $ $\mathbf { R } ^ { m }$ be a function. Suppose that $f = ( f _ { 1 } , \ldots , f _ { m } )$ , where $f _ { j } : \Omega  \mathbf { R }$ is the $j ^ { t h }$ co-ordinate of f. Then f is measurable if and only if all of the $f _ { j }$ are individually measurable. 

Proof. See Exercise 7.5.2. 

Unfortunately, it is not true that the composition of two measurable functions is automatically measurable; however we can do the next best thing: a continuous function applied to a measurable function is measurable. 

Lemma 7.5.5. Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let W be an open subset of $\mathbf { R } ^ { m }$ . If $f : \Omega \to W$ is measurable, and $g : W \to \mathbf { R } ^ { p }$ is continuous, then $g \circ f : \Omega \to \mathbf { R } ^ { p }$ is measurable. 

Proof. See Exercise 7.5.3. 

This has an immediate corollary: 

Corollary 7.5.6. Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ . If $f : \Omega  \mathbf { R }$ is a measurable function, then so is $| f |$ , max(f, 0), and min $( f , 0 )$ 

Proof. Apply Lemma 7.5.5 with $g ( x ) : = | x | , g ( x ) : = \operatorname* { m a x } ( x , 0 )$ , and $g ( x ) : = \operatorname* { m i n } ( x , 0 )$ □ 

A slightly less immediate corollary: 

Corollary 7.5.7. Let Ω be a measurable subset of $\mathbf { R } ^ { n } . \textit { I f f } : \Omega  \mathbf { R }$ and $g : \Omega  \mathbf { R }$ are measurable functions, then so is $f + g , f - g , f g $ $\operatorname* { m a x } ( f , g )$ , and min $( f , g )$ . If $g ( x ) \neq 0$ for all $x \in \Omega$ , then $f / g$ is also measurable. 

Proof. Consider $f + g$ . We can write this as $k \circ h .$ , where $h : \Omega \to \mathbf { R } ^ { 2 }$ is the function $h ( x ) = ( f ( x ) , g ( x ) )$ , and $k : \mathbf { R } ^ { 2 }  \mathbf { R }$ is the function $k ( a , b ) : = a + b$ . Since $f , g$ are measurable, then h is also measurable by Corollary 7.5.4. Since k is continuous, we thus see from Lemma 7.5.5 that $k \circ h$ is measurable, as desired. A similar argument deals with all the other cases; the only thing concerning the $f / g$ case is that the space $\mathbf { R } ^ { 2 }$ must be replaced with $\{ ( a , b ) \in \mathbf { R } ^ { 2 } : b \neq 0 \}$ in order to keep the map $( a , b ) \mapsto a / b$ continuous and well-defined. □ 

<!-- === Source: MinerU_markdown_Analysis_II_Third_Edition_-_By_Terence_Tao_201_2122707919320490002.md (Page 201) === -->

## 7.5. Measurable functions

Another characterization of measurable functions is given by 

Lemma 7.5.8. Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f : \Omega $ R be a function. Then f is measurable if and only if $f ^ { - 1 } ( ( a , \infty ) )$ is measurable for every real number a. 

Proof. See Exercise 7.5.4. 

Inspired by this lemma, we extend the notion of a measurable function to the extended real number system $\mathbf { R } ^ { * } : = \mathbf { R } \cup \{ + \infty \} \cup \{ - \infty \}$ : 

Definition 7.5.9 (Measurable functions in the extended reals). Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ . A function $f : \Omega \to \mathbf { R } ^ { * }$ is said to be measurable if $f ^ { - 1 } ( ( a , + \infty ] )$ is measurable for every real number $a .$ 

Note that Lemma 7.5.8 ensures that the notion of measurability for functions taking values in the extended reals $\mathbf { R } ^ { * }$ is compatible with that for functions taking values in just the reals R. 

Measurability behaves well with respect to limits: 

Lemma 7.5.10 (Limits of measurable functions are measurable). Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ . For each positive integer $n _ { \scriptscriptstyle ; }$ , let $f _ { n } : \Omega \to$ $\mathbf { R } ^ { * }$ be a measurable function. Then the functions $\operatorname* { s u p } _ { n \geq 1 } f _ { n }$ , $\operatorname { i n f } _ { n \geq 1 } f _ { n }$ lim $\operatorname { s u p } _ { n \to \infty } f _ { n }$ , and lim in $\mathrm { f } _ { n  \infty } f _ { n }$ are also measurable. In particular, if the $f _ { n }$ converge pointwise to another function $f : \Omega \to \mathbf { R } ^ { * }$ , then f is also measurable. 

Proof. We first prove the claim about $\operatorname* { s u p } _ { n \geq 1 } f _ { n }$ . Call this function $g .$ We have to prove that $g ^ { - 1 } ( ( a , + \infty ] )$ is measurable for every $a .$ . But by the definition of supremum, we have 

$$
g ^ {- 1} ((a, + \infty ]) = \bigcup_ {n \geq 1} f _ {n} ^ {- 1} ((a, + \infty ])
$$

$\mathrm { \left( w h y ? \right) }$ , and the claim follows since the countable union of measurable sets is again measurable. 

A similar argument works for in $\operatorname { f } _ { n \geq 1 } f _ { n }$ . The claim for lim sup and lim inf then follow from the identities 

$$
\limsup _ {n \to \infty} f _ {n} = \inf _ {N \geq 1} \sup _ {n \geq N} f _ {n}
$$

and 

$$
\liminf _ {n \to \infty} f _ {n} = \sup _ {N \geq 1} \inf _ {n \geq N} f _ {n}
$$

(see Definition 6.4.6). 

□ 

As you can see, just about anything one does to a measurable function will produce another measurable function. This is basically why almost every function one deals with in mathematics is measurable. (Indeed, the only way to construct non-measurable functions is via artificial means such as invoking the axiom of choice.) 

## — Exercises —

Exercise 7.5.1. Prove Lemma 7.5.3. (Hint: use Lemma 7.4.10 and the σ-algebra property.) 

Exercise 7.5.2. Use Lemma 7.5.3 to deduce Corollary 7.5.4. 

Exercise 7.5.3. Prove Lemma 7.5.5. 

Exercise 7.5.4. Prove Lemma 7.5.8. (Hint: use Lemma 7.5.3. As a preliminary step, you may need to show that if $f ^ { - 1 } ( ( a , \infty ) )$ is measurable for all a, then $f ^ { - 1 } ( [ a , \infty ) )$ is also measurable for all a.) 

Exercise 7.5.5. Let $f : \mathbf { R } ^ { n }  \mathbf { R }$ be Lebesgue measurable, and let $g : \mathbf { R } ^ { n }  \mathbf { R }$ be a function which agrees with f outside of a set of measure zero, thus there exists a set $A \subseteq \mathbf { R } ^ { n }$ of measure zero such that $f ( x ) = g ( x )$ for all $x \in \mathbf { R } ^ { n } \backslash A$ Show that g is also Lebesgue measurable. (Hint: use Exercise 7.4.10.) 

## Chapter 8

## Lebesgue integration

In Chapter 11, we approached the Riemann integral by first integrating a particularly simple class of functions, namely the piecewise constant functions. Among other things, piecewise constant functions only attain a finite number of values (as opposed to most functions in real life, which can take an infinite number of values). Once one learns how to integrate piecewise constant functions, one can then integrate other Riemann integrable functions by a similar procedure. 

We shall use a similar philosophy to construct the Lebesgue integral. We shall begin by considering a special subclass of measurable functions - the simple functions. Then we will show how to integrate simple functions, and then from there we will integrate all measurable functions (or at least the absolutely integrable ones). 

## 8.1 Simple functions

Definition 8.1.1 (Simple functions). Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f : \Omega  \mathbf { R }$ be a measurable function. We say that f is a simple function if the image $f ( \Omega )$ is finite. In other words, there exists a finite number of real numbers $c _ { 1 } , c _ { 2 } , \dots , c _ { N }$ such that for every $x \in \Omega$ , we have $f ( x ) = c _ { j }$ for some $1 \leq j \leq N$ 

Example 8.1.2. Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let E be a measurable subset of Ω. We define the characteristic function $\chi _ { E } :$ $\Omega  \mathbf { R }$ by setting $\chi _ { E } ( x ) : = 1$ if $x \in E .$ , and $\chi _ { E } ( x ) : = 0 { \mathrm { ~ i f ~ } } x \notin E$ (In some texts, $\chi _ { E }$ is also written $1 _ { E } ,$ , and is referred to as an indicator function). Then $\chi _ { E }$ is a measurable function (why?), and is a simple function, because the image $\chi _ { E } ( \Omega )$ is 0, 1 (or 0 if E is empty, or 1 if $E = \Omega )$ . 

We remark on three basic properties of simple functions: that they form a vector space, that they are linear combinations of characteristic functions, and that they approximate measurable functions. More precisely, we have the following three lemmas: 

Lemma 8.1.3. Let $\Omega$ be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f : \Omega  \mathbf { R }$ and $g : \Omega  \mathbf { R }$ be simple functions. Then $f + g$ is also a simple function. Also, for any scalar $c \in \mathbf { R }$ , the function cf is also a simple function. 

Proof. See Exercise 8.1.1. 

Lemma 8.1.4. Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f : \Omega $ R be a simple function. Then there exists a finite number of real numbers $c _ { 1 } , \ldots , c _ { N } $ , and a finite number of disjoint measurable sets $E _ { 1 } , E _ { 2 } , \dots , E _ { N }$ in Ω, such that $\begin{array} { r } { f = \sum _ { i = 1 } ^ { N } c _ { i } \chi _ { E _ { i } } } \end{array}$ 

Proof. See Exercise 8.1.2. 

Lemma 8.1.5. Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f : \Omega  \mathbf { R }$ be a measurable function. Suppose that f is always non-negative, i.e., $f ( x ) \geq 0$ for all $x \in \Omega$ . Then there exists a sequence $f _ { 1 } , f _ { 2 } , f _ { 3 } , \ldots o f$ simple functions, $f _ { n } : \Omega \to \mathbf { R }$ , such that the $f _ { n }$ are non-negative and increasing, 

$$
0 \leq f _ {1} (x) \leq f _ {2} (x) \leq f _ {3} (x) \leq \dots \text {   for   all   } x \in \Omega
$$

and converge pointwise to f: 

$$
\lim _ {n \to \infty} f _ {n} (x) = f (x) \text {   for   all   } x \in \Omega .
$$

Proof. See Exercise 8.1.3. 

We now show how to compute the integral of simple functions. 

Definition 8.1.6 (Lebesgue integral of simple functions). Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f : \Omega  \mathbf { R }$ be a simple function which is non-negative; thus $f$ is measurable and the image $f ( \Omega )$ is finite and contained in $[ 0 , \infty )$ . We then define the Lebesgue integral $\textstyle \int _ { \Omega } f$ of $f$ on Ω by 

$$
\int_ {\Omega} f := \sum_ {\lambda \in f (\Omega); \lambda > 0} \lambda m (\{x \in \Omega : f (x) = \lambda \}).
$$

## 8.1. Simple functions

We will also sometimes write $\textstyle \int _ { \Omega } f$ as $\textstyle \int _ { \Omega } f$ dm (to emphasize the rˆole of Lebesgue measure m) or use a dummy variable such as x, e.g., $\textstyle \int _ { \Omega } f ( x ) \ d x$ 

Example 8.1.7. Let $f : \mathbf { R }  \mathbf { R }$ be the function which equals 3 on the interval [1, 2], equals 4 on the integral $( 2 , 4 )$ , and is zero everywhere else. Then 

$$
\int_ {\Omega} f := 3 \times m ([ 1, 2 ]) + 4 \times m ((2, 4)) = 3 \times 1 + 4 \times 2 = 1 1.
$$

Or if $g : \mathbf { R }  \mathbf { R }$ is the function which equals 1 on $[ 0 , \infty )$ and is zero everywhere else, then 

$$
\int_ {\Omega} g = 1 \times m ([ 0, \infty)) = 1 \times + \infty = + \infty .
$$

Thus the simple integral of a simple function can equal $+ \infty$ . (The reason why we restrict this integral to non-negative functions is to avoid ever encountering the indefinite form $+ \infty + ( - \infty ) )$ ). 

Remark 8.1.8. Note that this definition of integral corresponds to one’s intuitive notion of integration (at least of non-negative functions) as the area under the graph of the function (or volume, if one is in higher dimensions). 

Another formulation of the integral for non-negative simple functions is as follows. 

Lemma 8.1.9. Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $E _ { 1 } , \ldots , E _ { N }$ are a finite number of disjoint measurable subsets in Ω. Let $c _ { 1 } , \ldots , c _ { N }$ be non-negative numbers (not necessarily distinct). Then we have 

$$
\int_ {\Omega} \sum_ {j = 1} ^ {N} c _ {j} \chi_ {E _ {j}} = \sum_ {j = 1} ^ {n} c _ {j} m (E _ {j}).
$$

Proof. We can assume that none of the $c _ { j }$ are zero, since we can just remove them from the sum on both sides of the equation. Let $f : =$ $\Sigma _ { j = 1 } ^ { N } c _ { j } \chi _ { E _ { j } }$ . Then $f ( x )$ is either equal to one of the $c _ { j } \ ( { \mathrm { i f } } \ x \in E _ { j } )$ or equal to 0 $( { \mathrm { i f ~ } } x \not \in \bigcup _ { j = 1 } ^ { N } E _ { j } )$ . Thus f is a simple function, and $f ( \Omega ) \subseteq$ {<sup>0</sup>} $\cup \{ c _ { j } : 1 \leq j \leq N \}$ . Thus, by the definition, 

$$
\begin{array}{c} \int_ {\Omega} f = \sum_ {\lambda \in \{c _ {j}: 1 \leq j \leq N \}} \lambda m (\{x \in \Omega : f (x) = \lambda \}) \\ = \sum_ {\lambda \in \{c _ {j}: 1 \leq j \leq N \}} \lambda m (\bigcup_ {1 \leq j \leq N: c _ {j} = \lambda} E _ {j}). \end{array}
$$

But by the finite additivity property of Lebesgue measure, this is equal to 

$$
\sum_ {\lambda \in \{c _ {j}: 1 \leq j \leq N \}} \lambda \sum_ {1 \leq j \leq N: c _ {j} = \lambda} m (E _ {j})
$$

$$
\sum_ {\lambda \in \{c _ {j}: 1 \leq j \leq N \}} \sum_ {1 \leq j \leq N: c _ {j} = \lambda} c _ {j} m (E _ {j}).
$$

Each $j$ appears exactly once in this sum, since $c _ { j }$ is only equal to exactly one value of λ. So the above expression is equal to $\begin{array} { r } { \sum _ { 1 \le j \le N } c _ { j } m ( E _ { j } ) } \end{array}$ as desired. □ 

Some basic properties of Lebesgue integration of non-negative simple functions: 

Proposition 8.1.10. Let Ω be a measurable set, and let $f : \Omega  \mathbf { R }$ and $g : \Omega  \mathbf { R }$ be non-negative simple functions. 

(a) We have $\textstyle 0 \leq \int _ { \Omega } f \leq \infty$ . Furthermore, we have $\textstyle \int _ { \Omega } f = 0$ if and only if $m ( \{ x \in { \bar { \Omega } } : f ( x ) \neq 0 \} ) = 0$ 

(b) We have $\begin{array} { r } { \int _ { \Omega } ( f + g ) = \int _ { \Omega } f + \int _ { \Omega } g . } \end{array}$ 

(c) For any positive number $^ { c , }$ we have $\textstyle { \int _ { \Omega } c f = c \int _ { \Omega } f }$ 

(d) If $f ( x ) \leq g ( x )$ for all $x \in \Omega$ , then we have $\textstyle { \int _ { \Omega } f \leq \int _ { \Omega } g }$ 

We make a very convenient notational convention: if a property $P ( x )$ holds for all points in $\Omega ,$ except for a set of measure zero, then we say that P holds for almost every point in Ω. Thus (a) asserts that $\textstyle \int _ { \Omega } f = 0$ if and only if f is zero for almost every point in Ω. 

Proof. From Lemma 8.1.4 or from the formula 

$$
f = \sum_ {\lambda \in f (\Omega) \backslash \{0 \}} \lambda \chi_ {\{x \in \Omega : f (x) = \lambda \}}
$$

we can write f as a combination of characteristic functions, say 

$$
f = \sum_ {j = 1} ^ {N} c _ {j} \chi_ {E _ {j}},
$$

where $E _ { 1 } , \ldots , E _ { N }$ are disjoint subsets of Ω and the $c _ { j }$ are positive. Similarly we can write 

$$
g = \sum_ {k = 1} ^ {M} d _ {k} \chi_ {F _ {k}}
$$

where $F _ { 1 } , \ldots , F _ { M }$ are disjoint subsets of Ω and the $d _ { k }$ are positive. 

(a) Since $\begin{array} { r } { \int _ { \Omega } f = \sum _ { j = 1 } ^ { N } c _ { j } m ( E _ { j } ) } \end{array}$ it is clear that the integral is between 0 and infinity. If $f$ is zero almost everywhere, then all of the $E _ { j }$ must have measure zero (why?) and so $\textstyle \int _ { \Omega } f = 0$ . Conversely, if $\textstyle \int _ { \Omega } f = 0$ , then $\begin{array} { r } { \sum _ { j = 1 } ^ { N } c _ { j } m ( E _ { j } ) = 0 } \end{array}$ , which can only happen when all of the $m ( E _ { j } )$ are zero (since all the $c _ { j }$ are positive). But then $\textstyle \bigcup _ { j = 1 } ^ { N } E _ { j }$ has measure zero, and hence $f$ is zero almost everywhere in Ω. 

(b) Write $E _ { 0 } : = \Omega \backslash \bigcup _ { j = 1 } ^ { N } E _ { j }$ and $c _ { 0 } : = 0$ , then we have $\Omega = E _ { 0 } \cup E _ { 1 } \cup$ $\dots \cup E _ { N }$ and 

$$
f = \sum_ {j = 0} ^ {N} c _ {j} \chi_ {E _ {j}}.
$$

Similarly if we write $F _ { 0 } : = \Omega \backslash \bigcup _ { k = 1 } ^ { M } F _ { k }$ and $d _ { 0 } : = 0$ then 

$$
g = \sum_ {k = 0} ^ {M} d _ {k} \chi_ {F _ {k}}.
$$

Since $\Omega = E _ { 0 } \cup . . . \cup E _ { N } = F _ { 0 } \cup . . . \cup F _ { M }$ , we have 

$$
f = \sum_ {j = 0} ^ {N} \sum_ {k = 0} ^ {M} c _ {j} \chi_ {E _ {j} \cap F _ {k}}
$$

and 

$$
g = \sum_ {k = 0} ^ {M} \sum_ {j = 0} ^ {N} d _ {k} \chi_ {E _ {j} \cap F _ {k}}
$$

and hence 

$$
f + g = \sum_ {0 \leq j \leq N; 0 \leq k \leq M} (c _ {j} + d _ {k}) \chi_ {E _ {j} \cap F _ {k}}.
$$

By Lemma 8.1.9, we thus have 

$$
\int_ {\Omega} (f + g) = \sum_ {0 \leq j \leq N; 0 \leq k \leq M} (c _ {j} + d _ {k}) m (E _ {j} \cap F _ {k}).
$$

On the other hand, we have 

$$
\int_ {\Omega} f = \sum_ {0 \leq j \leq N} c _ {j} m (E _ {j}) = \sum_ {0 \leq j \leq N; 0 \leq k \leq M} c _ {j} m (E _ {j} \cap F _ {k})
$$

and similarly 

$$
\int_ {\Omega} g = \sum_ {0 \leq k \leq M} d _ {k} m (F _ {k}) = \sum_ {0 \leq j \leq N; 0 \leq k \leq M} d _ {k} m (E _ {j} \cap F _ {k})
$$

and the claim (b) follows. 

(c) Since $\begin{array} { r } { c f = \sum _ { j = 1 } ^ { N } c c _ { j } \chi _ { E _ { j } } } \end{array}$ , we have $\begin{array} { r } { \int _ { \Omega } c f = \sum _ { j = 1 } ^ { N } c c _ { j } m ( E _ { j } ) } \end{array}$ . Since $\begin{array} { r } { \int _ { \Omega } f = \sum _ { j = 1 } ^ { N } c _ { j } m ( E _ { j } ) } \end{array}$ , the claim follows. 

(d) Write $h : = g - f$ . Then h is simple and non-negative and $g = f + h$ hence by (b) we have $\textstyle { \int _ { \Omega } g = \int _ { \Omega } f + \int _ { \Omega } h }$ . But by (a) we have $\textstyle \int _ { \Omega } h \geq 0$ , and the claim follows. 

□ 

## — Exercises —

Exercise 8.1.1. Prove Lemma 8.1.3. 

Exercise 8.1.2. Prove Lemma 8.1.4. 

Exercise 8.1.3. Prove Lemma 8.1.5. (Hint: set 

$$
f _ {n} (x) := \sup \{\frac {j}{2 ^ {n}}: j \in {\bf Z}, \frac {j}{2 ^ {n}} \leq \min (f (x), 2 ^ {n}) \},
$$

i.e., $f _ { n } ( x )$ is the greatest integer multiple of $2 ^ { - n }$ which does not exceed either $f ( x )$ or $2 ^ { n }$ . You may wish to draw a picture to see how $f _ { 1 } , f _ { 2 } , f _ { 3 }$ , etc. works. Then prove that $f _ { n }$ obeys all the required properties.) 

## 8.2 Integration of non-negative measurable functions

We now pass from the integration of non-negative simple functions to the integration of non-negative measurable functions. We will allow our measurable functions to take the value of $+ \infty$ sometimes. 

Definition 8.2.1 (Majorization). Let $f : \Omega  \mathbf { R }$ and $g : \Omega  \mathbf { R }$ be functions. We say that $f$ majorizes $g ,$ or g minorizes $f ,$ if we have $f ( x ) \geq g ( x )$ for all $x \in \Omega$ 

We sometimes use the phrase “f dominates $g ^ { , \dag }$ instead of $^ { 6 6 } f$ majorizes $g ^ { , \dag }$ 

Definition 8.2.2 (Lebesgue integral for non-negative functions). Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f : \Omega  [ 0 , \infty ]$ be measurable and non-negative. Then we define the Lebesgue integral $\textstyle \int _ { \Omega } f$ of $f$ on Ω to be 

$$
\int_ {\Omega} f := \sup \left\{\int_ {\Omega} s: s \text {   is   simple   and   non - negative,   and   minorizes   } f \right\}.
$$

Remark 8.2.3. The reader should compare this notion to that of a lower Riemann integral from Definition 11.3.2. Interestingly, we will not need to match this lower integral with an upper integral here. 

Remark 8.2.4. Note that if $\Omega ^ { \prime }$ is any measurable subset of Ω, then we can define $\textstyle \int _ { \Omega ^ { \prime } } f$ as well by restricting $f$ to $\Omega ^ { \prime }$ , thus $\textstyle \int _ { \Omega ^ { \prime } } f : = \int _ { \Omega ^ { \prime } } f | _ { \Omega ^ { \prime } }$ 

We have to check that this definition is consistent with our previous notion of Lebesgue integral for non-negative simple functions; in other words, if $f : \Omega  \mathbf { R }$ is a non-negative simple function, then the value of $\textstyle \int _ { \Omega } f$ given by this definition should be the same as the one given in the previous definition. But this is clear because $f$ certainly minorizes itself, and any other non-negative simple function s which minorizes $f$ will have an integral s less than or equal to $\textstyle \int _ { \Omega } f$ , thanks to Proposition $8 . 1 . 1 0 ( \mathrm { d } )$ 

Remark 8.2.5. Note that $\textstyle \int _ { \Omega } f$ is always at least 0, since 0 is simple, non-negative, and minorizes f. Of course, $\textstyle \int _ { \Omega } f$ could equal + . 

Some basic properties of the Lebesgue integral on non-negative measurable functions (which supercede Proposition 8.1.10): 

Proposition 8.2.6. Let Ω be a measurable set, and let $f : \Omega  [ 0 , \infty ]$ and $g : \Omega \to [ 0 , \infty ]$ be non-negative measurable functions. 

(a) We have $\textstyle 0 \leq \int _ { \Omega } f \leq \infty$ . Furthermore, we have $\textstyle \int _ { \Omega } f = 0$ if and only if $f ( x ) = 0$ for almost every $x \in \Omega$ 

(b) For any positive number c, we have $\textstyle \int _ { \Omega } c f = c \int _ { \Omega } f$ 

(c) If $f ( x ) \leq g ( x )$ for all $x \in \Omega$ , then we have $\textstyle { \int _ { \Omega } f \leq \int _ { \Omega } g }$ 

(d) $I f f ( x ) = g ( x )$ for almost every $x \in \Omega$ , then $\textstyle { \int _ { \Omega } f = \int _ { \Omega } g }$ 

(e) $I f \Omega ^ { \prime } \subseteq \Omega$ is measurable, then $\begin{array} { r } { \int _ { \Omega ^ { \prime } } f = \int _ { \Omega } f \chi _ { \Omega ^ { \prime } } \leq \int _ { \Omega } f . } \end{array}$ 

Proof. See Exercise 8.2.1. 

Remark 8.2.7. Proposition $8 . 2 . 6 ( \mathrm { d } )$ is quite interesting; it says that one can modify the values of a function on any measure zero set (e.g., you can modify a function on every rational number), and not afect its integral at all. It is as if no individual point, or even a measure zero collection of points, has any “vote” in what the integral of a function should be; only the collective set of points has an influence on an integral. 

Remark 8.2.8. Note that we do not yet try to interchange sums and integrals. From the definition it is fairly easy to prove that $\textstyle \int _ { \Omega } ( f + g ) \geq$ $\textstyle { \int _ { \Omega } f + \int _ { \Omega } g }$ (Exercise 8.2.2), but to prove equality requires more work and will be done later. 

As we have seen in previous chapters, we cannot always interchange an integral with a limit (or with limit-like concepts such as supremum). However, with the Lebesgue integral it is possible to do so if the functions are increasing: 

Theorem 8.2.9 (Lebesgue monotone convergence theorem). Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $( f _ { n } ) _ { n = 1 } ^ { \infty }$ be a sequence of non-negative measurable functions from Ω to R which are increasing in the sense that 

$$
0 \leq f _ {1} (x) \leq f _ {2} (x) \leq f _ {3} (x) \leq \dots \text {   for   all   } x \in \Omega .
$$

(Note we are assuming that $f _ { n } ( x )$ is increasing with respect to n; this is a diferent notion from $f _ { n } ( x )$ increasing with respect to x.) Then we have 

$$
0 \leq \int_ {\Omega} f _ {1} \leq \int_ {\Omega} f _ {2} \leq \int_ {\Omega} f _ {3} \leq \dots
$$

and 

$$
\int_ {\Omega} \sup _ {n} f _ {n} = \sup _ {n} \int_ {\Omega} f _ {n}.
$$

Proof. The first conclusion is clear from Proposition $8 . 2 . 6 ( \mathrm { c } )$ . Now we prove the second conclusion. From Proposition 8.2.6(c) again we have 

$$
\int_ {\Omega} \sup _ {m} f _ {m} \geq \int_ {\Omega} f _ {n}
$$

for every $n ;$ taking suprema in n we obtain 

$$
\int_ {\Omega} \sup _ {m} f _ {m} \geq \sup _ {n} \int_ {\Omega} f _ {n}
$$

which is one half of the desired conclusion. To finish the proof we have to show 

$$
\int_ {\Omega} \sup _ {m} f _ {m} \leq \sup _ {n} \int_ {\Omega} f _ {n}.
$$

From the definition of $\int _ { \Omega } \mathrm { s u p } _ { m } f _ { m }$ , it will sufice to show that 

$$
\int_ {\Omega} s \leq \sup _ {n} \int_ {\Omega} f _ {n}
$$

for all simple non-negative functions which minorize $\operatorname { s u p } _ { m } f _ { m }$ 

Fix s. We will show that 

$$
(1 - \varepsilon) \int_ {\Omega} s \leq \sup _ {n} \int_ {\Omega} f _ {n}
$$

for every $0 < \varepsilon < 1$ ; the claim then follows by taking limits as $\varepsilon \to 0$ 

Fix ε. By construction of s, we have 

$$
s (x) \leq \sup _ {n} f _ {n} (x)
$$

for every $x \in \Omega$ . Hence, for every $x \in \Omega$ there exists an N (depending on x) such that 

$$
f _ {N} (x) \geq (1 - \varepsilon) s (x).
$$

Since the $f _ { n }$ are increasing, this will imply that $f _ { n } ( x ) \geq ( 1 - \varepsilon ) s ( x )$ for all $n \geq N$ . Thus, if we define the sets $E _ { n }$ by 

$$
E _ {n} := \{x \in \Omega : f _ {n} (x) \geq (1 - \varepsilon) s (x) \}
$$

then we have $E _ { 1 } \subset E _ { 2 } \subset E _ { 3 } \subset . .$ . and $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n } = \Omega$ 

From Proposition 8.2.6(cdf) we have 

$$
(1 - \varepsilon) \int_ {E _ {n}} s = \int_ {E _ {n}} (1 - \varepsilon) s \leq \int_ {E _ {n}} f _ {n} \leq \int_ {\Omega} f _ {n}
$$

so to finish the argument it will sufice to show that 

$$
\sup _ {n} \int_ {E _ {n}} s = \int_ {\Omega} s.
$$

Since s is a simple function, we may write $\begin{array} { r } { s = \sum _ { j = 1 } ^ { N } c _ { j } \chi _ { F _ { j } } } \end{array}$ for some measurable $F _ { j }$ and positive $c _ { j }$ . Since 

$$
\int_ {\Omega} s = \sum_ {j = 1} ^ {N} c _ {j} m (F _ {j})
$$

and 

$$
\int_ {E _ {n}} s = \int_ {E _ {n}} \sum_ {j = 1} ^ {N} c _ {j} \chi_ {F _ {j} \cap E _ {n}} = \sum_ {j = 1} ^ {N} c _ {j} m (F _ {j} \cap E _ {n})
$$

it thus sufices to show that 

$$
\sup _ {n} m (F _ {j} \cap E _ {n}) = m (F _ {j})
$$

for each $j$ . But this follows from Exercise 7.2.3(a). 

This theorem is extremely useful. For instance, we can now interchange addition and integration: 

Lemma 8.2.10 (Interchange of addition and integration). Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f : \Omega  [ 0 , \infty ]$ and $g : \Omega  [ 0 , \infty ]$ be measurable functions. Then $\textstyle { \int _ { \Omega } ( f + g ) = \int _ { \Omega } f + \int _ { \Omega } g }$ 

Proof. By Lemma 8.1.5, there exists a sequence $0 \leq s _ { 1 } \leq s _ { 2 } \leq . . . \leq f$ of simple functions such that $\operatorname* { s u p } _ { n } s _ { n } = f$ , and similarly a sequence $0 \leq t _ { 1 } \leq t _ { 2 } \leq . . . \leq g$ of simple functions such that $\operatorname* { s u p } _ { n } t _ { n } = g$ . Since the $s _ { n }$ are increasing and the $t _ { n }$ are increasing, it is then easy to check that $s _ { n } + t _ { n }$ is also increasing and $\mathrm { s u p } _ { n } ( s _ { n } + t _ { n } ) = f + g \ ( \mathrm { w h y ? } )$ . By the monotone convergence theorem (Theorem 8.2.9) we thus have 

$$
\int_ {\Omega} f = \sup _ {n} \int_ {\Omega} s _ {n}
$$

$$
\int_ {\Omega} g = \sup _ {n} \int_ {\Omega} t _ {n}
$$

$$
\int_ {\Omega} (f + g) = \sup _ {n} \int_ {\Omega} (s _ {n} + t _ {n}).
$$

But by Proposition 8.1.9(b) we have $\begin{array} { r } { \int _ { \Omega } ( s _ { n } + t _ { n } ) \ d s = \int _ { \Omega } s _ { n } + \int _ { \Omega } t _ { n } \ d s } \end{array}$ . By Proposition 8.1.9(d), $\int _ { \Omega } \boldsymbol { s } _ { n }$ and $\int _ { \Omega } t _ { n }$ are both increasing in $n _ { ; }$ , so 

$$
\sup _ {n} \left(\int_ {\Omega} s _ {n} + \int_ {\Omega} t _ {n}\right) = \left(\sup _ {n} \int_ {\Omega} s _ {n}\right) + \left(\sup _ {n} \int_ {\Omega} t _ {n}\right)
$$

and the claim follows. 

Of course, once one can interchange an integral with a sum of two functions, one can handle an integral and any finite number of functions by induction. More surprisingly, one can handle infinite sums as well of non-negative functions: 

Corollary 8.2.11. If Ω is a measurable subset of $\mathbf { R } ^ { n }$ , and $g _ { 1 } , \ g _ { 2 } , \ldots$ are a sequence of non-negative measurable functions from Ω to [0, ], then 

$$
\int_ {\Omega} \sum_ {n = 1} ^ {\infty} g _ {n} = \sum_ {n = 1} ^ {\infty} \int_ {\Omega} g _ {n}.
$$

Proof. See Exercise 8.2.3. 

Remark 8.2.12. Note that we do not need to assume anything about the convergence of the above sums; it may well happen that both sides are equal to + . However, we do need to assume non-negativity; see Exercise 8.2.4. 

One could similarly ask whether we could interchange limits and integrals; in other words, is it true that 

$$
\int_ {\Omega} \lim _ {n \to \infty} f _ {n} = \lim _ {n \to \infty} \int_ {\Omega} f _ {n}.
$$

Unfortunately, this is not true, as the following “moving bump” example shows. For each $n = 1 , 2 , 3 . . . ,$ let $f _ { n } : \mathbf { R }  \mathbf { R }$ be the function $f _ { n } =$ $\chi _ { [ n , n + 1 ) }$ . Then $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } f _ { n } ( x ) = 0 } \end{array}$ for every x, but $\textstyle \int _ { \mathbf { R } } f _ { n } = 1$ for every $n ,$ and hence $\textstyle \operatorname* { l i m } _ { n \to \infty } \int _ { \mathbf { R } } f _ { n } = 1 \neq 0$ . In other words, the limiting function $\operatorname* { l i m } _ { n \to \infty } f _ { n }$ can end up having significantly smaller integral than any of the original integrals. However, the following very useful lemma of Fatou shows that the reverse cannot happen - there is no way the limiting function has larger integral than the (limit of the) original integrals: 

Lemma 8.2.13 (Fatou’s lemma). Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ and let $f _ { 1 } , f _ { 2 } , \ldots$ be a sequence of non-negative functions from Ω to $[ 0 , \infty ]$ . Then 

$$
\int_ {\Omega} \operatorname * {l i m i n f} _ {n \to \infty} f _ {n} \leq \operatorname * {l i m i n f} _ {n \to \infty} \int_ {\Omega} f _ {n}.
$$

Proof. Recall that 

$$
\liminf _ {n \to \infty} f _ {n} = \sup _ {n} \left(\inf _ {m \geq n} f _ {m}\right)
$$

and hence by the monotone convergence theorem 

$$
\int_ {\Omega} \liminf _ {n \to \infty} f _ {n} = \sup _ {n} \int_ {\Omega} \left(\inf _ {m \geq n} f _ {m}\right).
$$

By Proposition 8.2.6(c) we have 

$$
\int_ {\Omega} \left(\inf _ {m \geq n} f _ {m}\right) \leq \int_ {\Omega} f _ {j}
$$

for every $j \geq n ;$ taking infima in j we obtain 

$$
\int_ {\Omega} \left(\inf _ {m \geq n} f _ {m}\right) \leq \inf _ {j \geq n} \int_ {\Omega} f _ {j}.
$$

Thus 

$$
\int_ {\Omega} \liminf _ {n \to \infty} f _ {n} \leq \sup _ {n} \inf _ {j \geq n} \int_ {\Omega} f _ {j} = \liminf _ {n \to \infty} \int_ {\Omega} f _ {n}
$$

as desired. 

Note that we are allowing our functions to take the value + at some points. It is even possible for a function to take the value $+ \infty$ but still have a finite integral; for instance, if $E$ is a measure zero set, and $f : \Omega  \mathbf { R }$ is equal to + on $E$ but equals 0 everywhere else, then $\textstyle \int _ { \Omega } f = 0$ by Proposition 8.2.6(a). However, if the integral is finite, the function must be finite almost everywhere: 

Lemma 8.2.14. Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f : \Omega $ $[ 0 , \infty ]$ be a non-negative measurable function such that $\textstyle \int _ { \Omega } f$ is finite. Then f is finite almost everywhere (i.e., the set $\{ x \in \Omega : { \bar { f } } ( x ) = + \infty \}$ has measure zero). 

Proof. See Exercise 8.2.5. 

Form Corollary 8.2.11 and Lemma 8.2.14 one has a useful lemma: 

Lemma 8.2.15 (Borel-Cantelli lemma). Let $\Omega _ { 1 } , \Omega _ { 2 } , \ldots$ . be measurable subsets of $\mathbf { R } ^ { n }$ such that $\Sigma _ { n = 1 } ^ { \infty } m ( \Omega _ { n } )$ is finite. Then the set 

$$
\{x \in \mathbf {R} ^ {n}: x \in \Omega_ {n} f o r i n f i n i t e l y m a n y n \}
$$

is a set of measure zero. In other words, almost every point belongs to only finitely many $\Omega _ { n }$ 

Proof. See Exercise 8.2.6. 

$$
- \text { Exercises } -
$$

Exercise 8.2.1. Prove Proposition 8.2.6. (Hint: do not attempt to mimic the proof of Proposition 8.1.10; rather, try to use Proposition 8.1.10 and Definition 8.2.2. For one direction of part (a), start with $\textstyle \int _ { \Omega } f = 0$ and conclude that m $. ( \{ x \in \Omega : f ( x ) > 1 / n \} ) = 0$ for every $n = 1 , 2 , 3 , . . . ,$ , and then use the countable sub-additivity. To prove (e), first prove it for simple functions.) 

Exercise 8.2.2. Let Ω be a measurable subset of R<sup>n</sup>, and let $f : \Omega  [ 0 , + \infty ]$ and $g : \Omega  [ 0 , + \infty ]$ be measurable functions. Without using Theorem 8.2.9 or Lemma 8.2.10, prove that $\begin{array} { r } { \int _ { \Omega } ( f + g ) \geq \int _ { \Omega } f + \int _ { \Omega } g . } \end{array}$ 

Exercise 8.2.3. Prove Corollary 8.2.11. (Hint: use the monotone convergence theorem with $\begin{array} { r } { f _ { N } : = \sum _ { n = 1 } ^ { N } g _ { n } . ) } \end{array}$ 

Exercise 8.2.4. For each $n = 1 , 2 , 3 , . . . ,$ , let $f _ { n } : \mathbf { R }  \mathbf { R }$ be the function $f _ { n } = \chi _ { [ n , n + 1 ) } - \chi _ { [ n + 1 , n + 2 ) } ;$ ; i.e., let $f _ { n } ( x )$ equal +1 when $x \in [ n , n + 1 )$ , equal 1 when $x \in [ n + 1 , n + 2 )$ , and 0 everywhere else. Show that 

$$
\int_ {\mathbf {R}} \sum_ {n = 1} ^ {\infty} f _ {n} \neq \sum_ {n = 1} ^ {\infty} \int_ {\mathbf {R}} f _ {n}.
$$

Explain why this does not contradict Corollary 8.2.11. 

Exercise 8.2.5. Prove Lemma 8.2.14. 

Exercise 8.2.6. Use Corollary 8.2.11 and Lemma 8.2.14 to prove Lemma 8.2.15. (Hint: use the indicator functions $\chi _ { \Omega _ { n } \cdot } )$ 

Exercise 8.2.7. Let $p > 2$ and $c > 0$ . Using the Borel-Cantelli lemma, show that the set 

$$
\{x \in [ 0, 1 ]: | x - \frac {a}{q} | \leq \frac {c}{q ^ {p}} \text { for   infinitely   many   positive   integers } a, q \}
$$

has measure zero. (Hint: one only has to consider those integers a in the range $0 \leq a \leq q { \mathrm { ~ ( w h y ? ) } }$ . Use Corollary 11.6.5 to show that the sum $\textstyle \sum _ { q = 1 } ^ { \infty } { \frac { c ( q + 1 ) } { q ^ { p } } }$ is finite.) 

Exercise 8.2.8. Call a real number $x \in \mathbf { R }$ diophantine if there exist real numbers $p , C > 0$ such that $\textstyle | x - { \frac { a } { q } } | > C / | q | ^ { p }$ for all non-zero integers $q$ and all integers a. Using Exercise 8.2.7, show that almost every real number is diophantine. (Hint: first work in the interval [0, 1]. Show that one can take $p$ and $C$ to be rational and one can also take $p > 2$ . Then use the fact that the countable union of measure zero sets has measure zero.) 

Exercise 8.2.9. For every positive integer $n ,$ , let $f _ { n } : \mathbf { R }  [ 0 , \infty )$ be a nonnegative measurable function such that 

$$
\int_ {\mathbf {R}} f _ {n} \leq \frac {1}{4 ^ {n}}.
$$

Show that for every $\varepsilon > 0$ , there exists a set $E$ of Lebesgue measure $m ( E ) \leq \varepsilon$ such that $f _ { n } ( x )$ converges pointwise to zero for all $x \in \mathbf { R } \backslash E$ . (Hint: first prove that $\begin{array} { r } { m ( \{ x \in \mathbf { R } : f _ { n } ( x ) > \frac { 1 } { \varepsilon 2 ^ { n } } \} ) \leq \frac { \varepsilon } { 2 ^ { n } } } \end{array}$ for all $n = 1 , 2 , 3 , \ldots$ , and then consider the union of all the sets $\{ { \bar { x } } \in \mathbf { R } : f _ { n } ^ { - } ( x ) > { \frac { 1 } { \varepsilon 2 ^ { n } } } \} . )$ 

Exercise 8.2.10. For every positive integer $n _ { : }$ , let $f _ { n } : [ 0 , 1 ] \to [ 0 , \infty )$ be a nonnegative measurable function such that $f _ { n }$ converges pointwise to zero. Show that for every $\varepsilon > 0$ , there exists a set $E$ of Lebesgue measure m $( E ) \leq \varepsilon$ such that $f _ { n } ( x )$ converges uniformly to zero for all $x \in [ 0 , 1 ] \backslash E$ . (This is a special case of Egorof’s theorem. To prove it, first show that for any positive integer m, we can find an $N > 0$ such that m $( \{ x \in [ 0 , 1 ] : f _ { n } ( x ) > 1 / m \} ) \leq \varepsilon / 2 ^ { m }$ for all $n \geq N . )$ Is the claim still true if [0, 1] is replaced by R? 

Exercise 8.2.11. Give an example of a bounded non-negative function $f :$ $\mathbf { N } \times \mathbf { N }  \mathbf { R } ^ { + }$ such that $\textstyle \sum _ { m = 1 } ^ { \infty } { \bar { f } } ( n , m )$ converges for every n, and such that $\scriptstyle \operatorname* { l i m } _ { n \to \infty } f ( n , m )$ exists for every m, but such that 

$$
\lim _ {n \to \infty} \sum_ {m = 1} ^ {\infty} f (n, m) \neq \sum_ {m = 1} ^ {\infty} \lim _ {n \to \infty} f (n, m).
$$

(Hint: modify the moving bump example. It is even possible to use a function f which only takes the values 0 and 1.) This shows that interchanging limits and infinite sums can be dangerous. 

## 8.3 Integration of absolutely integrable functions

We have now completed the theory of the Lebesgue integral for nonnegative functions. Now we consider how to integrate functions which can be both positive and negative. However, we do wish to avoid the indefinite expression $+ \infty + ( - \infty )$ , so we will restrict our attention to a subclass of measurable functions - the absolutely integrable functions. 

Definition 8.3.1 (Absolutely integrable functions). Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ . A measurable function $f : \Omega \to \mathbf { R } ^ { * }$ is said to be absolutely integrable if the integral $\textstyle \int _ { \Omega } | f |$ is finite. 

Of course, $| f |$ is always non-negative, so this definition makes sense even if f changes sign. Absolutely integrable functions are also known as $L ^ { 1 } ( \Omega )$ functions. 

If $f : \Omega \to \mathbf { R } ^ { * }$ is a function, we define the positive part $f ^ { + } : \Omega $ $[ 0 , \infty ]$ and negative part $f ^ { - } : \Omega  [ 0 , \infty ]$ by the formulae 

$$
f ^ {+} := \max (f, 0); \quad f ^ {-} := - \min (f, 0).
$$

From Corollary 7.5.6 we know that $f ^ { + }$ and $f ^ { - }$ are measurable. Observe also that $f ^ { + }$ and $f ^ { - }$ are non-negative, that $f = f ^ { + } - f ^ { - }$ , and $| f | =$ $f ^ { + } + f ^ { - } . \ \mathrm { ( W h y ? ) }$ 

Definition 8.3.2 (Lebesgue integral). Let $f : \Omega \to \mathbf { R } ^ { * }$ be an absolutely integrable function. We define the Lebesgue integral $\textstyle \int _ { \Omega } f$ of $f$ to be the quantity 

$$
\int_ {\Omega} f := \int_ {\Omega} f ^ {+} - \int_ {\Omega} f ^ {-}.
$$

Note that since f is absolutely integrable, $\int _ { \Omega } f ^ { + }$ and $\int _ { \Omega } f ^ { - }$ are less than or equal to $\textstyle \int _ { \Omega } | f |$ and hence are finite. Thus $\textstyle \int _ { \Omega } f$ is always finite; we are never encountering the indeterminate form $+ \infty - ( + \infty )$ 

Note that this definition is consistent with our previous definition of the Lebesgue integral for non-negative functions, since if $f$ is nonnegative then $f ^ { + } = f$ and $f ^ { - } = 0$ . We also have the useful triangle inequality 

$$
\left| \int_ {\Omega} f \right| \leq \int_ {\Omega} f ^ {+} + \int_ {\Omega} f ^ {-} = \int_ {\Omega} | f |\tag{8.1}
$$

(Exercise 8.3.1). 

Some other properties of the Lebesgue integral: 

Proposition 8.3.3. Let Ω be a measurable set, and let $f : \Omega  \mathbf { R }$ and $g : \Omega  \mathbf { R }$ be absolutely integrable functions. 

(a) For any real number c (positive, zero, or negative), we have that cf is absolutely integrable and $\textstyle \int _ { \Omega } c f = c \int _ { \Omega } f$ 

(b) The function $f + g$ is absolutely integrable, and $\textstyle \int _ { \Omega } ( f + g ) = \int _ { \Omega } f +$ $\scriptstyle \int _ { \Omega } g$ 

(c) $I f f ( x ) \leq g ( x )$ for all $x \in \Omega$ , then we have $\textstyle { \int _ { \Omega } f \leq \int _ { \Omega } g }$ 

(d) $I f f ( x ) = g ( x )$ for almost every $x \in \Omega$ , then $\textstyle { \int _ { \Omega } f = \int _ { \Omega } g }$ 

Proof. See Exercise 8.3.2. 

As mentioned in the previous section, one cannot necessarily interchange limits and integrals, lim $\textstyle \int f _ { n } = \int \operatorname* { l i m } f _ { n }$ , as the “moving bump example” showed. However, it is possible to exclude the moving bump example, and successfully interchange limits and integrals, if we know that the functions $f _ { n }$ are all majorized by a single absolutely integrable function. This important theorem is known as the Lebesgue dominated convergence theorem, and is extremely useful: 

Theorem 8.3.4 (Lebesgue dominated convergence thm). Let $\Omega$ be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f _ { 1 } , f _ { 2 } , \ldots$ be a sequence of measurable functions from Ω to $\mathbf { R } ^ { * }$ which converge pointwise. Suppose also that there is an absolutely integrable function $F : \Omega \to [ 0 , \infty ]$ such that $| f _ { n } ( x ) | \leq F ( x )$ for all $x \in \Omega$ and all $n = 1 , 2 , 3 , \ldots$ Then 

$$
\int_ {\Omega} \lim _ {n \to \infty} f _ {n} = \lim _ {n \to \infty} \int_ {\Omega} f _ {n}.
$$

Proof. Let $f : \Omega \to \mathbf { R } ^ { * }$ be the function $f ( x ) : = \dim _ { n \to \infty } f _ { n } ( x )$ ; this function exists by hypothesis. By Lemma 7.5.10, f is measurable. Also, since $| f _ { n } ( x ) | \leq F ( x )$ for all n and all $x \in \Omega$ , we see that each $f _ { n }$ is absolutely integrable, and by taking limits we obtain $| f ( x ) | \leq F ( x )$ for all $x \in \Omega$ , so f is also absolutely integrable. Our task is to show that $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } \int _ { \Omega } f _ { n } = \int _ { \Omega } f } \end{array}$ 

The functions $F + f _ { n }$ are non-negative and converge pointwise to $F + f$ . So by Fatou’s lemma (Lemma 8.2.13) 

$$
\int_ {\Omega} F + f \leq \liminf _ {n \to \infty} \int_ {\Omega} F + f _ {n}
$$

and thus 

$$
\int_ {\Omega} f \leq \liminf _ {n \to \infty} \int_ {\Omega} f _ {n}.
$$

But the functions $F - f _ { n }$ are also non-negative and converge pointwise to $F - f$ . So by Fatou’s lemma again 

$$
\int_ {\Omega} F - f \leq \liminf _ {n \to \infty} \int_ {\Omega} F - f _ {n}.
$$

Since the right-hand side is $\begin{array} { r } { \int _ { \Omega } F - \operatorname* { l i m } \operatorname* { s u p } _ { n \to \infty } \int _ { \Omega } f _ { n } } \end{array}$ (why did the lim inf become a lim sup?), we thus have 

$$
\int_ {\Omega} f \geq \limsup _ {n \to \infty} \int_ {\Omega} f _ {n}.
$$

Thus the lim inf and lim sup of $\int _ { \Omega } f _ { n }$ are both equal to $\textstyle \int _ { \Omega } f $ , as desired. 

Finally, we record a lemma which is not particularly interesting in itself, but will have some useful consequences later in these notes. 

Definition 8.3.5 (Upper and lower Lebesgue integral). Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f : \Omega  \mathbf { R }$ be a function (not necessarily measurable). We define the upper Lebesgue integral $\overline { { \int } } _ { \Omega } f$ to be 

${ \overline { { \int } } } _ { \Omega } f : = \operatorname* { i n f } \{ \int _ { \Omega } g : g$ is an absolutely integrable function 

from Ω to R that majorizes $f \}$ 

and the lower Lebesgue integral $\underline { { \boldsymbol { \int } } } _ { \Omega } f$ to be 

$\int _ { \Omega } f : = \operatorname* { s u p } \{ \int _ { \Omega } g : g$ is an absolutely integrable function 

from Ω to R that minorizes $f \}$ 

It is easy to see that ${ \underline { { \int } } } _ { \Omega } f \leq { \overline { { \int } } } _ { \Omega } f \ ( \mathrm { w h y } ?$ use Proposition $8 . 3 . 3 ( \mathrm { c } ) )$ When f is absolutely integrable then equality occurs $\mathrm { \left( w h y ? \right) }$ . The converse is also true: 

Lemma 8.3.6. Let Ω be a measurable subset of $\mathbf { R } ^ { n }$ , and let $f : \Omega  \mathbf { R }$ be a function (not necessarily measurable). Let A be a real number, and suppose $\textstyle { \overline { { \int } } } _ { \Omega } f = { \underline { { \int } } } _ { \Omega } f = A$ . Then f is absolutely integrable, and 

$$
\int_ {\Omega} f = \overline {{\int}} _ {\Omega} f = \underline {{\int}} _ {\Omega} f = A.
$$

Proof. By definition of upper Lebesgue integral, for every integer $n \geq$ 1 we may find an absolutely integrable function $f _ { n } ^ { + } : \Omega \to \mathbf { R }$ which majorizes f such that 

$$
\int_ {\Omega} f _ {n} ^ {+} \leq A + \frac {1}{n}.
$$

Similarly we may find an absolutely integrable function $f _ { n } ^ { - } : \Omega \to \mathbf { R }$ which minorizes f such that 

$$
\int_ {\Omega} f _ {n} ^ {-} \leq A - \frac {1}{n}.
$$

Let $F ^ { + } : = \operatorname* { i n f } _ { n } f _ { n } ^ { + }$ and $F ^ { - } : = \operatorname* { s u p } _ { n } f _ { n } ^ { - }$ . Then $F ^ { + }$ and $F ^ { - }$ are measurable (by Lemma 7.5.10) and absolutely integrable (because they are squeezed between the absolutely integrable functions $f _ { 1 } ^ { + }$ and $f _ { 1 } ^ { - }$ , for instance). Also, $F ^ { + }$ majorizes $f$ and $F ^ { - }$ minorizes $f .$ . Finally, we have 

$$
\int_ {\Omega} F ^ {+} \leq \int_ {\Omega} f _ {n} ^ {+} \leq A + \frac {1}{n}
$$

for every n, and hence 

$$
\int_ {\Omega} F ^ {+} \leq A.
$$

Similarly we have 

$$
\int_ {\Omega} F ^ {-} \geq A.
$$

but $F ^ { + }$ majorizes $F ^ { - }$ −, and hence $\begin{array} { r } { \int _ { \Omega } F ^ { + } \geq \int _ { \Omega } F ^ { } } \end{array}$ −. Hence we must have 

$$
\int_ {\Omega} F ^ {+} = \int_ {\Omega} F ^ {-} = A.
$$

In particular 

$$
\int_ {\Omega} F ^ {+} - F ^ {-} = 0.
$$

By Proposition $8 . 2 . 6 ( \mathrm { a } )$ , we thus have $F ^ { + } ( x ) = F ^ { - } ( x )$ for almost every x. But since f is squeezed between $F ^ { - }$ and $F ^ { + }$ , we thus have $f ( x ) =$ $F ^ { + } ( x ) = F ^ { - } ( x )$ for almost every x. In particular, $f$ difers from the absolutely integrable function $F ^ { + }$ only on a set of measure zero and is thus measurable (see Exercise 7.5.5) and absolutely integrable, with 

$$
\int_ {\Omega} f = \int_ {\Omega} F ^ {+} = \int_ {\Omega} F ^ {-} = A
$$

as desired. 

— Exercises — 

Exercise 8.3.1. Prove (8.1) whenever Ω is a measurable subset of $\mathbf { R } ^ { n }$ and f is an absolutely integrable function. 

Exercise 8.3.2. Prove Proposition 8.3.3. (Hint: for (b), break $f , g ,$ and $f + g$ up into positive and negative parts, and try to write everything in terms of integrals of non-negative functions only, using Lemma 8.2.10.) 

Exercise 8.3.3. Let $f : \mathbf { R }  \mathbf { R }$ and $g : \mathbf { R }  \mathbf { R }$ be absolutely integrable, measurable functions such that $f ( x ) \leq g ( x )$ for all $x \in \mathbf { R }$ , and that $\textstyle \int _ { \mathbf { R } } f = \int _ { R } g .$ Show that $f ( x ) = g ( x )$ for almost every $x \in \mathbf { R }$ (i.e., that $f ( x ) = { \\\overset { \vartriangle } { g ( x ) } }$ for all $x \in \mathbf { R }$ except possibly for a set of measure zero). 

## 8.4 Comparison with the Riemann integral

We have spent a lot of efort constructing the Lebesgue integral, but have not yet addressed the question of how to actually compute any Lebesgue integrals, and whether Lebesgue integration is any diferent from the Riemann integral (say for integrals in one dimension). Now we show that the Lebesgue integral is a generalization of the Riemann integral. To clarify the following discussion, we shall temporarily distinguish the Riemann integral from the Lebesgue integral by writing the Riemann integral $\textstyle \int _ { I } f$ as $R . \int _ { I } f$ 

Our objective here is to prove 

Proposition 8.4.1. Let $I \subseteq \mathbf { R }$ be an interval, and let $f : I  \mathbf { R }$ be a Riemann integrable function. Then f is also absolutely integrable, and $\textstyle \int _ { I } f = R . \int _ { I } f$ 

Proof. Write $\textstyle A : = R . \int _ { I } f$ . Since f is Riemann integrable, we know that the upper and lower Riemann integrals are equal to A. Thus, for every $\varepsilon > 0$ , there exists a partition P of I into smaller intervals J such that 

$$
A - \varepsilon \leq \sum_ {J \in \mathbf {P}} | J | \inf _ {x \in J} f (x) \leq A \leq \sum_ {J \in \mathbf {P}} | J | \sup _ {x \in J} f (x) \leq A + \varepsilon ,
$$

where $| J |$ denotes the length of J. Note that $| J |$ is the same as $m ( J )$ 1 since J is a box. 

Let $f _ { \varepsilon } ^ { - } : I  \mathbf { R }$ and $f _ { \varepsilon } ^ { + } : I  \mathbf { R }$ be the functions 

$$
f _ {\varepsilon} ^ {-} (x) = \sum_ {J \in \mathbf {P}} \inf _ {x \in J} f (x) \chi_ {J} (x)
$$

and 

$$
f _ {\varepsilon} ^ {+} (x) = \sum_ {J \in \mathbf {P}} \sup _ {x \in J} f (x) \chi_ {J} (x);
$$

these are simple functions and hence measurable and absolutely integrable. By Lemma 8.1.9 we have 

$$
\int_ {I} f _ {\varepsilon} ^ {-} = \sum_ {J \in \mathbf {P}} | J | \inf _ {x \in J} f (x)
$$

and 

$$
\int_ {I} f _ {\varepsilon} ^ {+} = \sum_ {J \in \mathbf {P}} | J | \sup _ {x \in J} f (x)
$$

and hence 

$$
A - \varepsilon \leq \int_ {I} f _ {\varepsilon} ^ {-} \leq A \leq \int_ {I} f _ {\varepsilon} ^ {+} \leq A + \varepsilon .
$$

Since $f _ { \varepsilon } ^ { + }$ majorizes $f ,$ , and $f _ { \varepsilon } ^ { - }$ minorizes $f _ { i }$ , we thus have 

$$
A - \varepsilon \leq \int_ {\Omega} f \leq \overline {{\int}} _ {\Omega} f \leq A + \varepsilon
$$

for every $\varepsilon ,$ and thus 

$$
\int_ {\Omega} f = \overline {{\int}} _ {\Omega} f = A
$$

and hence by Lemma 8.3.6, f is absolutely integrable with $\textstyle \int _ { I } f = A$ , as desired. □ 

Thus every Riemann integrable function is also Lebesgue integrable, at least on bounded intervals, and we no longer need the $R . \int _ { I } f$ notation. However, the converse is not true. Take for instance the function $f$ : $[ 0 , 1 ]  \mathbf { R }$ defined by $f ( x ) : = 1$ when x is rational, and $f ( x ) : = 0$ when x is irrational. Then from Proposition 11.7.1 we know that f is not Riemann integrable. On the other hand, f is the characteristic function of the set $\mathbf { Q } \cap [ 0 , 1 ]$ , which is countable and hence measure zero. Thus $f$ is Lebesgue integrable and $\begin{array} { r } { \int _ { [ 0 , 1 ] } f = 0 } \end{array}$ . Thus the Lebesgue integral can handle more functions than the Riemann integral; this is one of the primary reasons why we use the Lebesgue integral in analysis. (The other reason is that the Lebesgue integral interacts well with limits, as the Lebesgue monotone convergence theorem, Fatou’s lemma, and Lebesgue dominated convergence theorem already attest. There are no comparable theorems for the Riemann integral). 

## 8.5 Fubini’s theorem

In one dimension we have shown that the Lebesgue integral is connected to the Riemann integral. Now we will try to understand the connection in higher dimensions. To simplify the discussion we shall just study two-dimensional integrals, although the arguments we present here can easily be extended to higher dimensions. 

We shall study integrals of the form $\int _ { \mathbf { R } ^ { 2 } } f$ . Note that once we know how to integrate on $\mathbf { R } ^ { 2 }$ , we can integrate on measurable subsets $\Omega$ of $\mathbf { R } ^ { 2 }$ , since $\textstyle \int _ { \Omega } f$ can be rewritten as $\int _ { \mathbf { R } ^ { 2 } } f \chi _ { \Omega }$ 

Let $f ( x , y )$ be a function of two variables. In principle, we have three diferent ways to integrate $f$ on $\mathbf { R } ^ { 2 }$ . First of all, we can use the twodimensional Lebesgue integral, to obtain $\int _ { \mathbf { R } ^ { 2 } } f$ . Secondly, we can fix x and compute a one-dimensional integral in $y .$ and then take that quantity and integrate in $x ,$ thus obtaining $\textstyle \int _ { \mathbf { R } } ( \int _ { \mathbf { R } } f ( x , y ) \ d y )$ dx. Secondly, we could fix $y$ and integrate in $x ,$ and then integrate in $y ,$ , thus obtaining $\textstyle \int _ { \mathbf { R } } ( \int _ { \mathbf { R } } f ( x , y ) \ d x ) \ d y$ 

Fortunately, if the function $f$ is absolutely integrable on $f _ { i }$ , then all three integrals are equal: 

Theorem 8.5.1 (Fubini’s theorem). Let $f : { \mathbf { R } } ^ { 2 }  { \mathbf { R } }$ be an absolutely integrable function. Then there exists absolutely integrable functions $F : \mathbf { R }  \mathbf { R }$ and $G : \mathbf { R }  \mathbf { R }$ such that for almost every x, $f ( x , y )$ is absolutely integrable in y with 

$$
F (x) = \int_ {\mathbf {R}} f (x, y) d y,
$$

and for almost every y, $f ( x , y )$ is absolutely integrable in x with 

$$
G (y) = \int_ {\mathbf {R}} f (x, y) d x.
$$

Finally, we have 

$$
\int_ {\mathbf {R}} F (x) d x = \int_ {\mathbf {R} ^ {2}} f = \int_ {\mathbf {R}} G (y) d y.
$$

Remark 8.5.2. Very roughly speaking, Fubini’s theorem says that 

$$
\int_ {\mathbf {R}} \left(\int_ {\mathbf {R}} f (x, y) d y\right) d x = \int_ {\mathbf {R} ^ {2}} f = \int_ {\mathbf {R}} \left(\int_ {\mathbf {R}} f (x, y) d x\right) d y.
$$

This allows us to compute two-dimensional integrals by splitting them into two one-dimensional integrals. The reason why we do not write 

Fubini’s theorem this way, though, is that it is possible that the integral $\textstyle \int _ { \mathbf { R } } f ( x , y )$ dy does not actually exist for every x, and similarly $\textstyle \int _ { \mathbf { R } } f ( x , { \overline { { y } } } )$ dx does not exist for every $y ;$ Fubini’s theorem only asserts that these integrals only exist for almost every x and $y .$ . For instance, if $f ( x , y )$ is the function which equals 1 when $y > 0$ and $x = 0$ , equals $^ { - 1 }$ when $y < 0$ and $x = 0$ , and is zero otherwise, then $f$ is absolutely integrable on $\mathbf { R } ^ { 2 }$ and $\int _ { \mathbf { R } ^ { 2 } } f = 0$ (since $f$ equals zero almost everywhere in $\mathbf { R } ^ { 2 } )$ , but $\textstyle \int _ { \mathbf { R } } f ( x , y )$ dy is not absolutely integrable when $x = 0$ (though it is absolutely integrable for every other $x )$ 

Proof. The proof of Fubini’s theorem is quite complicated and we will only give a sketch here. We begin with a series of reductions. 

Roughly speaking (ignoring issues relating to sets of measure zero), we have to show that 

$$
\int_ {\mathbf {R}} \left(\int_ {\mathbf {R}} f (x, y) d y\right) d x = \int_ {\mathbf {R} ^ {2}} f
$$

together with a similar equality with x and y reversed. We shall just prove the above equality, as the other one is very similar. 

First of all, it sufices to prove the theorem for non-negative functions, since the general case then follows by writing a general function $f$ as a diference $f ^ { + } - f ^ { - }$ of two non-negative functions, and applying Fubini’s theorem to $f ^ { + }$ and $f ^ { - }$ separately (and using Proposition 8.3.3(a) and (b)). Thus we will henceforth assume that $f$ is non-negative. 

Next, it sufices to prove the theorem for non-negative functions $f$ supported on a bounded set such as $[ - N , N ] \times [ - N , N ]$ for some positive integer $N .$ . Indeed, once one obtains Fubini’s theorem for such functions, one can then write a general function $f$ as the supremum of such compactly supported functions as 

$$
f = \sup _ {N > 0} f \chi_ {[ - N, N ] \times [ - N, N ]},
$$

apply Fubini’s theorem to each function $f \chi _ { [ - N , N ] \times [ - N , N ] }$ separately, and then take suprema using the monotone convergence theorem. Thus we will henceforth assume that $f$ is supported on $[ - N , N ] \times [ - N , N ]$ 

By another similar argument, it sufices to prove the theorem for nonnegative simple functions supported on $[ - N , N ] \times [ - N , N ]$ , since one can use Lemma 8.1.4 to write $f$ as the supremum of simple functions (which must also be supported on $[ - N , N ] )$ , apply Fubini’s theorem to each simple function, and then take suprema using the monotone convergence theorem. Thus we may assume that f is a non-negative simple function supported on $[ - N , N ] \times [ - N , N ]$ 

Next, we see that it sufices to prove the theorem for characteristic functions supported in $[ - N , N ] \times [ - N , N ]$ . This is because every simple function is a linear combination of characteristic functions, and so we can deduce Fubini’s theorem for simple functions from Fubini’s theorem for characteristic functions. Thus we may take $f = \chi _ { E }$ for some measurable $E \subseteq [ - N , N ] \times [ - N , N ]$ . Our task is then to show (ignoring sets of measure zero) that 

$$
\int_ {[ - N, N ]} \left(\int_ {[ - N, N ]} \chi_ {E} (x, y) d y\right) d x = m (E).
$$

It will sufice to show the upper Lebesgue integral estimate 

$$
\overline {{\int}} _ {[ - N, N ]} \left(\overline {{\int}} _ {[ - N, N ]} \chi_ {E} (x, y) d y\right) d x \leq m (E).\tag{8.2}
$$

We will prove this estimate later. Once we show this for every set $E _ { \mathrm { { i } } }$ , we may substitute $E$ with $[ - N , N ] \times [ - N , N ] \backslash E$ and obtain 

$$
\overline {{\int}} _ {[ - N, N ]} \left(\overline {{\int}} _ {[ - N, N ]} (1 - \chi_ {E} (x, y)) d y\right) d x \leq 4 N ^ {2} - m (E).
$$

But the left-hand side is equal to 

$$
\overline {{\int}} _ {[ - N, N ]} (2 N - \int_ {- [ - N, N ]} \chi_ {E} (x, y) d y) d x
$$

which is in turn equal to 

$$
4 N ^ {2} - \int_ {\underline {{\text {} [ - N , N ]}}} \left(\int_ {\underline {{\text {} [ - N , N ]}}} \chi_ {E} (x, y) d y\right) d x
$$

and thus we have 

$$
\int_ {\underline {{\quad}} [ - N, N ]} \left(\int_ {\underline {{\quad}} [ - N, N ]} \chi_ {E} (x, y) d y\right) d x \geq m (E).
$$

In particular we have 

$$
\int_ {\underline {{\text {}}} [ - N, N ]} \left(\overline {{\int}} _ {[ - N, N ]} \chi_ {E} (x, y) d y\right) d x \geq m (E)
$$

and hence by Lemma 8.3.6 we see that $\overline { { \int } } _ { [ - N , N ] } \chi _ { E } ( x , y )$ dy is absolutely integrable and 

$$
\int_ {[ - N, N ]} \left(\overline {{\int}} _ {[ - N, N ]} \chi_ {E} (x, y) d y\right) d x = m (E).
$$

A similar argument shows that 

$$
\int_ {[ - N, N ]} \left(\int_ {\underline {{[ - N , N ]}}} \chi_ {E} (x, y) d y\right) d x = m (E)
$$

and hence 

$$
\int_ {[ - N, N ]} \left(\overline {{\int}} _ {[ - N, N ]} \chi_ {E} (x, y) d y - \underline {{\int}} _ {[ - N, N ]} \chi_ {E} (x, y)\right) d x = 0.
$$

Thus by Proposition 8.2.6(a) we have 

$$
\int_ {\underline {{\quad}} [ - N, N ]} \chi_ {E} (x, y) d y = \overline {{\int}} _ {[ - N, N ]} \chi_ {E} (x, y) d y
$$

for almost every $x \in [ - N , N ]$ . Thus $\chi _ { E } ( x , y )$ is absolutely integrable in $y$ for almost every x, and $\begin{array} { r } { \int _ { [ - N , N ] } \chi _ { E } ( x , y ) } \end{array}$ is thus equal (almost everywhere) to a function $F ( x )$ such that 

$$
\int_ {[ - N, N ]} F (x) d x = m (E)
$$

as desired. 

It remains to prove the bound (8.2). Let $\varepsilon > 0$ be arbitrary. Since $m ( E )$ is the same as the outer measure $m ^ { * } ( E )$ , we know that there exists an at most countable collection $( B _ { j } ) _ { j \in J }$ of boxes such that $E \subseteq \textstyle \bigcup _ { j \in J } B _ { j }$ and 

$$
\sum_ {j \in J} m (B _ {j}) \leq m (E) + \varepsilon .
$$

## 8.5. Fubini’s theorem

Each box $B _ { j }$ can be written as $B _ { j } = I _ { j } \times I _ { j } ^ { \prime }$ for some intervals $I _ { j }$ and $I _ { j } ^ { \prime }$ . Observe that 

$$
\begin{array}{l} m (B _ {j}) = | I _ {j} | | I _ {j} ^ {\prime} | = \int_ {I _ {j}} | I _ {j} ^ {\prime} | d x = \int_ {I _ {j}} \left(\int_ {I _ {j} ^ {\prime}} d y\right) d x \\ \quad = \int_ {[ - N, N ]} \left(\int_ {[ - N, N ]} \chi_ {I _ {j} \times I _ {j} ^ {\prime}} (x, y) d x\right) d y \\ \quad = \int_ {[ - N, N ]} \left(\int_ {[ - N, N ]} \chi_ {B _ {j}} (x, y) d x\right) d y. \end{array}
$$

Adding this over all $j \in J$ (using Corollary 8.2.11) we obtain 

$$
\sum_ {j \in J} m (B _ {j}) = \int_ {[ - N, N ]} \left(\int_ {[ - N, N ]} \sum_ {j \in J} \chi_ {B _ {j}} (x, y) d x\right) d y.
$$

In particular we have 

$$
\overline {{\int}} _ {[ - N, N ]} \left(\overline {{\int}} _ {[ - N, N ]} \sum_ {j \in J} \chi_ {B _ {j}} (x, y) d x\right) d y \leq m (E) + \varepsilon .
$$

But $\sum _ { j \in J } \chi _ { B _ { j } }$ majorizes $\chi _ { E }$ (why?) and thus 

$$
\overline {{\int}} _ {[ - N, N ]} \left(\overline {{\int}} _ {[ - N, N ]} \chi_ {E} (x, y) d x\right) d y \leq m (E) + \varepsilon .
$$

But $\varepsilon$ is arbitrary, and so we have (8.2) as desired. This completes the proof of Fubini’s theorem. □ 

## Index

π, 103, 104 σ-algebra, 164, 180 

Abel’s theorem, 84 absolute value for complex numbers, 96 absolutely integrable, 201 abstraction, 1 addition of complex numbers, 94 (countably) additive measure, 164, 178 adherent point of sets, 12 ambient space, 15 approximation to the identity, 67, 70, 118 arctangent:, see trigonometric functions associativity of addition in C, 94 of scalar multiplication, 131 of vector addition, 128 

ball, 11 Banach-Tarski paradox, 163, 176 base of the natural logarithm:, see e 

basis standard basis of row vectors, 128 Boolean algebra, 164, 178 Borel property, 164, 181 Borel-Cantelli lemma, 199 boundary (point), 11, 41 bounded function, 54 set, 22 C, C<sup>0</sup>, C<sup>1</sup>, C<sup>2</sup>, C<sup>k</sup>, 147 Cauchy sequence, 18 Cauchy-Schwarz inequality, 9, 112 chain rule in higher dimensions, 144, 146 character, 114 characteristic function, 187 Clairaut’s theorem:, see interchanging derivatives with derivatives closed box, 168 set, 13, 41 closure, 12, 41 cocountable topology, 43 coeficient, 75 

cofinite topology, 43 column vector, 128 commutativity of addition in C, 94 of addition in vector spaces, 128 of convolution, 68, 117 ,see also: ring, field, laws of algebra compactness, 21, 42 compact support, 67 completeness of metric spaces, 19 of the space of continuous functions, 57 completion of a metric space, 21 complex numbers C, 93 complex conjugation, 96 connectedness, 36 connected component, 39 continuity, 28, 41 and compactness, 34 and connectedness, 38 and convergence, 28 contraction, 149 mapping theorem, 150 convergence in L<sup>2</sup>, 517, 112 of a function at a point, 46 of sequences, 6, 40 pointwise:, see pointwise convergence uniform:, see uniform convergence convolution, 68, 87, 117 coset, 174 cosine:, see trigonometric functions 

cotangent:, see trigonometric functions cover, 166 see also:, open cover critical point, 161 de Moivre identities, 104 degree, 66 dense, 67 derivative directional, 137 in higher dimensions, 135, 138, 143, 146 matrix, 143 partial, 138 total, 137, 146 uniqueness of, 136 diferentiability k-fold, 79, 147 continuous, 147 directional, 137 in higher dimensions, 135 infinite, 79 diferential matrix:, see derivative matrix dilation, 129 diophantine, 200 Dirac delta function, 67 direct sum of functions, 32 discrete metric, 5 distance in C, 98 in R, 2 distributive law for complex numbers, 95 dominate: see majorize dominated convergence:, see Lebesgue 

dominated convergence theorem e, 90 Egorof’s theorem, 200 empty set, 164, 167 error-correcting codes, 4 Euclidean metric, 3 Euclidean space, 3 Euler’s formula, 101, 103 Euler’s number:, see e exponential function, 90, 99 exterior (point), 11, 40 Fatou’s lemma, 198 Fej´er kernel, 118 finite intersection property, 27 fixed point theorem, 150 Fourier coeficients, 115 inversion formula, 115 series, 116 series for arbitrary periods, 125 theorem, 121 transform, 115 fractional part, 109 frequency, 114 Fubini’s theorem, 207 geodesic, 5 geometric series formula, 63 gradient, 142 graph, 158 hairy ball theorem, 150 half-space, 177 Hausdorf space, 42, 43 Heine-Borel theorem, 22 

Hermitian form, 111 homogeneity, 112, 129 hypersurface, 158 identity map (or operator), 129 imaginary, 96 implicit diferentiation, 158 implicit function theorem, 158 inconsistent, 101 indicator function:, see characteristic function induced metric, 3, 16 topology, 16, 41 inner product, 110 integer part, 109 integration by parts, 84 interchanging derivatives with derivatives, 147 integrals with integrals, 198, 206 limits with derivatives, 65 limits with integrals, 64, 194, 202 limits with limits, 54 limits with sums, 200 sums with derivatives, 65, 77 sums with integrals, 62, 77, 197, 198, 200 interior (point), 11, 40 intermediate value theorem, 38 intrinsic, 22 inverse function theorem, 153 invertible function: see bijection local, 153 

involution, 96 isometry, 15 l<sup>1</sup>, l<sup>2</sup>, l∞, L<sup>1</sup>, L<sup>2</sup>, L∞, 3–5, 111, 201 equivalence of in finite dimensions, 7 see also: absolutely integrable laws of algebra for complex numbers, 94, 95 laws of arithmetic:, see laws of algebra laws of exponentiation, 90 Lebesgue dominated convergence theorem, 202 Lebesgue integral of absolutely integrable functions, 201 of nonnegative functions, 193 of simple functions, 188 upper and lower, 203 vs. the Riemann integral, 205 Lebesgue measurable, 177 Lebesgue measure, 165 motivation of, 164, 165 Lebesgue monotone convergence theorem, 194 Leibnitz rule, 145 limit formal (LIM), 21 laws, 98 limiting values of functions, 46 

pointwise, 49 uniform, see uniform limit uniqueness of, 8, 47 limit point of sequences, 18 linear combination, 129 linearity approximate, 134 of convolution, 72, 117 of inner product, 111 of integration, 191, 196 of transformations, 129 logarithm (natural), 91 power series of, 62, 91 

majorize, 193 manifold, 161 map:, see function matrix, 130 identification with linear transformations, 130–133 maximum principle, 34 measurability for functions, 183 for sets, 177 motivation of, 163 see also:, Lebesgue measure, outer measure metric, 2 ball:, see ball on C, 98 on R, 3 space, 2 monomial, 114 monotone (increasing or decreasing) 

convergence:, see Lebesgue monotone convergence theorem measure, 165, 168 moving bump example, 50, 197 multiplication of complex numbers, 95 of matrices, 130, 133 negation of complex numbers, 96 neighbourhood, 40 Newton’s approximation, 136 non-degenerate, 112 nowhere diferentiable function, 65, 105 of sets adherent point, 41 open box, 166 cover, 23 set, 13 order topology, 43 orthogonality, 112 orthonormal, 114 non-additivity of, 175 outer measure, 167 non-additivity of, 174 Parseval identity, 125 ,see also: Plancherel formula path-connected, 38 periodic, 108 extension, 109 Plancherel formula (or theorem), 116, 123 pointwise convergence, 48 of series, 59 

topology of, 58 polar representation, 104 polynomial, 66 and convolution, 68 approximation by, 66, 71 positive complex number, 96, 100 inner product, 111 measure, 164, 167 power series, 75 formal, 75 multiplication of, 87 uniqueness of, 81 pre-image:, see inverse image product topology, 58 projection, 129 Pythagoras’ theorem, 112 Quotient rule, 146 radius of convergence, 75 real analytic, 78 real numbers R are uncountable:, see uncountability of the reals real part, 96 real-valued, 58 reciprocal of complex numbers, 97 relative topology:, see induced topology ring commutative, 95 root mean square:, see L<sup>2</sup> row vector, 127 scalar multiplication, 127 series of functions, 62 

simple function, 187 sine:, see trigonometric functions space, 2 square wave, 109, 113 Stone-Weierstrass theorem, 73, 117 sub-additive measure, 165, 168 subsequence, 17 summation by parts, 84 sup norm:, see supremum as norm support, 67 supremum (and infimum) as metric, 4 as norm, 4, 59 taxi-cab metric, 3 Taylor series, 80 Taylor’s formula:, see Taylor series topological space, 39 totally bounded, 26 translation invariance, 165, 168, 178 transpose, 128 triangle inequality for integrals, 201 in C, 97 in Euclidean space, 9 in inner product spaces, 112 in metric spaces, 2 

trigonometric functions, 101, 106 and Fourier series, 124 power series, 101, 105 trigonometric polynomials, 114 trivial topology, 42 uniform continuity, 34 uniform convergence, 51 and anti-derivatives, 64 and derivatives, 54 and integrals, 62 and limits, 53 and radius of convergence, 75 as a metric, 56, 110 of series, 59 uniform limit and Riemann integration, 61 of bounded functions, 54 of continuous functions, 53 vector space, 128 vertical line test, 68 volume, 166 Weierstrass M-test, 60 Weierstrass approximation theorem, 66, 71–72, 116 Weierstrass example:, see nowhere diferentiable function 

## Texts and Readings in Mathematics

1. R. B. Bapat: Linear Algebra and Linear Models ( Edition)Third 

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

38. Terence Tao: Analysis II ( Edition)Third 



39. W. Decker and C. Lossen: Computing in Algebraic Geometry 





40. A. Goswami and B. V. Rao: A Course in Applied Stochastic Processes 





41. K. B. Athreya and S. N. Lahiri: Probability Theory 





42. A. R. Rajwade and A. K. Bhandari: Surprises and Counterexamples in Real Function Theory 





43. G. H. Golub and C. F. Van Loan: Matrix Computations (Reprint of the Third Edition) 





44. Rajendra Bhatia: Positive Definite Matrices 





45. K. R. Parthasarathy: Coding Theorems of Classical and Quantum Information Theory (Second Edition) 





46. C. S. Seshadri: Introduction to the Theory of Standard Monomials (Second Edition) 





47. Alain Connes and Matilde Marcolli: Noncommutative Geometry, Quantum Fields and Motives 





48. Vivek S. Borkar: Stochastic Approximation: A Dynamical Systems Viewpoint 





49. B. J. Venkatachala: Inequalities: An Approach Through Problems 





50. Rajendra Bhatia: Notes on Functional Analysis 





51. A. Clebsch (ed.): Jacobi's Lectures on Dynamics (Second Revised Edition) 





52. S. Kesavan: Functional Analysis 





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

