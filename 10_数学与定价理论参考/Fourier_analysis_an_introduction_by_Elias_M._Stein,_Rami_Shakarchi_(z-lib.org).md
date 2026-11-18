

<!-- === Source: MinerU_markdown_Fourier_analysis_an_introduction_by_Elias_M._Stein,_Rami_Shakarchi_(z-lib.org)_1_2122707133446336526.md (Page 1) === -->

PRINCETON LECTURES IN ANALYSIS I 

## FOURIER ANALYSIS AN INTRODUCTION

ELIAS M. STEIN & RAMI SHAKARCHI 

Ibookroot October 20, 2007 

FOURIER ANALYSIS 

# Princeton Lectures in Analysis

I Fourier Analysis: An Introduction 

II Complex Analysis 

III Real Analysis: 

Measure Theory, Integration, and 

Hilbert Spaces 

Princeton Lectures in Analysis 

I 

# FOURIER ANALYSIS an introduction

Elias M. Stein 

& Rami Shakarchi 

PRINCETON UNIVERSITY PRESS PRINCETON AND OXFORD 

Copyright © 2003 by Princeton University Press Published by Princeton University Press, 41 William Street, Princeton, New Jersey 08540 In the United Kingdom: Princeton University Press, 6 Oxford Street, Woodstock, Oxfordshire OX20 1TW 

All Rights Reserved 

Library of Congress Control Number 2003103688 ISBN 978-0-691-11384-5 

British Library Cataloging-in-Publication Data is available 

The publisher would like to acknowledge the authors of this volume for providing the camera-ready copy from which this book was printed 

Printed on acid-free paper. ∞ 

press.princeton.edu 

Printed in the United States of America 

5 7 9 10 8 6 

To my grandchildren Carolyn, Alison, Jason 

E.M.S. 

To my parents 

Mohamed & Mireille 

and my brother 

Karim 

R.S. 

# Foreword

Beginning in the spring of 2000, a series of four one-semester courses were taught at Princeton University whose purpose was to present, in an integrated manner, the core areas of analysis. The objective was to make plain the organic unity that exists between the various parts of the subject, and to illustrate the wide applicability of ideas of analysis to other fields of mathematics and science. The present series of books is an elaboration of the lectures that were given. 

While there are a number of excellent texts dealing with individual parts of what we cover, our exposition aims at a diferent goal: presenting the various sub-areas of analysis not as separate disciplines, but rather as highly interconnected. It is our view that seeing these relations and their resulting synergies will motivate the reader to attain a better understanding of the subject as a whole. With this outcome in mind, we have concentrated on the main ideas and theorems that have shaped the field (sometimes sacrificing a more systematic approach), and we have been sensitive to the historical order in which the logic of the subject developed. 

We have organized our exposition into four volumes, each reflecting the material covered in a semester. Their contents may be broadly summarized as follows: 

I. Fourier series and integrals. 

II. Complex analysis. 

III. Measure theory, Lebesgue integration, and Hilbert spaces. 

IV. A selection of further topics, including functional analysis, distributions, and elements of probability theory. 

However, this listing does not by itself give a complete picture of the many interconnections that are presented, nor of the applications to other branches that are highlighted. To give a few examples: the elements of (finite) Fourier series studied in Book I, which lead to Dirichlet characters, and from there to the infinitude of primes in an arithmetic progression; the X-ray and Radon transforms, which arise in a number of problems in Book I, and reappear in Book III to play an important role in understanding Besicovitch-like sets in two and three dimensions; Fatou’s theorem, which guarantees the existence of boundary values of bounded holomorphic functions in the disc, and whose proof relies on ideas developed in each of the first three books; and the theta function, which first occurs in Book I in the solution of the heat equation, and is then used in Book II to find the number of ways an integer can be represented as the sum of two or four squares, and in the analytic continuation of the zeta function. 

A few further words about the books and the courses on which they were based. These courses where given at a rather intensive pace, with 48 lecture-hours a semester. The weekly problem sets played an indispensable part, and as a result exercises and problems have a similarly important role in our books. Each chapter has a series of “Exercises” that are tied directly to the text, and while some are easy, others may require more efort. However, the substantial number of hints that are given should enable the reader to attack most exercises. There are also more involved and challenging “Problems”; the ones that are most dificult, or go beyond the scope of the text, are marked with an asterisk. 

Despite the substantial connections that exist between the diferent volumes, enough overlapping material has been provided so that each of the first three books requires only minimal prerequisites: acquaintance with elementary topics in analysis such as limits, series, diferentiable functions, and Riemann integration, together with some exposure to linear algebra. This makes these books accessible to students interested in such diverse disciplines as mathematics, physics, engineering, and finance, at both the undergraduate and graduate level. 

It is with great pleasure that we express our appreciation to all who have aided in this enterprise. We are particularly grateful to the students who participated in the four courses. Their continuing interest, enthusiasm, and dedication provided the encouragement that made this project possible. We also wish to thank Adrian Banner and Jose Luis Rodrigo for their special help in running the courses, and their eforts to see that the students got the most from each class. In addition, Adrian Banner also made valuable suggestions that are incorporated in the text. 

## FOREWORD

We wish also to record a note of special thanks for the following individuals: Charles Feferman, who taught the first week (successfully launching the whole project!); Paul Hagelstein, who in addition to reading part of the manuscript taught several weeks of one of the courses, and has since taken over the teaching of the second round of the series; and Daniel Levine, who gave valuable help in proof-reading. Last but not least, our thanks go to Gerree Pecht, for her consummate skill in typesetting and for the time and energy she spent in the preparation of all aspects of the lectures, such as transparencies, notes, and the manuscript. 

We are also happy to acknowledge our indebtedness for the support we received from the 250th Anniversary Fund of Princeton University, and the National Science Foundation’s VIGRE program. 

Elias M. Stein 

Rami Shakarchi 

Princeton, New Jersey August 2002 

## Preface to Book I

Any efort to present an overall view of analysis must at its start deal with the following questions: Where does one begin? What are the initial subjects to be treated, and in what order are the relevant concepts and basic techniques to be developed? 

Our answers to these questions are guided by our view of the centrality of Fourier analysis, both in the role it has played in the development of the subject, and in the fact that its ideas permeate much of the presentday analysis. For these reasons we have devoted this first volume to an exposition of some basic facts about Fourier series, taken together with a study of elements of Fourier transforms and finite Fourier analysis. Starting this way allows one to see rather easily certain applications to other sciences, together with the link to such topics as partial diferential equations and number theory. In later volumes several of these connections will be taken up from a more systematic point of view, and the ties that exist with complex analysis, real analysis, Hilbert space theory, and other areas will be explored further. 

In the same spirit, we have been mindful not to overburden the beginning student with some of the dificulties that are inherent in the subject: a proper appreciation of the subtleties and technical complications that arise can come only after one has mastered some of the initial ideas involved. This point of view has led us to the following choice of material in the present volume: 

• Fourier series. At this early stage it is not appropriate to introduce measure theory and Lebesgue integration. For this reason our treatment of Fourier series in the first four chapters is carried out in the context of Riemann integrable functions. Even with this restriction, a substantial part of the theory can be developed, detailing convergence and summability; also, a variety of connections with other problems in mathematics can be illustrated. 

• Fourier transform. For the same reasons, instead of undertaking the theory in a general setting, we confine ourselves in Chapters 5 and 6 largely to the framework of test functions. Despite these limitations, we can learn a number of basic and interesting facts about Fourier analysis in R<sup>d</sup> and its relation to other areas, including the wave equation and the Radon transform. 

• Finite Fourier analysis. This is an introductory subject par excellence, because limits and integrals are not explicitly present. Nevertheless, the subject has several striking applications, including the proof of the infinitude of primes in arithmetic progression. 

Taking into account the introductory nature of this first volume, we have kept the prerequisites to a minimum. Although we suppose some acquaintance with the notion of the Riemann integral, we provide an appendix that contains most of the results about integration needed in the text. 

We hope that this approach will facilitate the goal that we have set for ourselves: to inspire the interested reader to learn more about this fascinating subject, and to discover how Fourier analysis afects decisively other parts of mathematics and science. 

## Contents

Foreword vii
Preface xi
Chapter 1. The Genesis of Fourier Analysis 1
1 The vibrating string 2
1.1 Derivation of the wave equation 6
1.2 Solution to the wave equation 8
1.3 Example: the plucked string 16
2 The heat equation 18
2.1 Derivation of the heat equation 18
2.2 Steady-state heat equation in the disc 19
3 Exercises 22
4 Problem 27
Chapter 2. Basic Properties of Fourier Series 29
1 Examples and formulation of the problem 30
1.1 Main definitions and some examples 34
2 Uniqueness of Fourier series 39
3 Convolutions 44
4 Good kernels 48
5 Cesàro and Abel summability: applications to Fourier series 51
5.1 Cesàro means and summation 51
5.2 Fejér's theorem 52
5.3 Abel means and summation 54
5.4 The Poisson kernel and Dirichlet's problem in the unit disc 55
6 Exercises 58
7 Problems 65
Chapter 3. Convergence of Fourier Series 69
1 Mean-square convergence of Fourier series 70
1.1 Vector spaces and inner products 70
1.2 Proof of mean-square convergence 76
2 Return to pointwise convergence 81
2.1 A local result 81
2.2 A continuous function with diverging Fourier series 83 

xiv CONTENTS
3 Exercises 87
4 Problems 95
Chapter 4. Some Applications of Fourier Series 100
1 The isoperimetric inequality 101
2 Weyl's equidistribution theorem 105
3 A continuous but nowhere differentiable function 113
4 The heat equation on the circle 118
5 Exercises 120
6 Problems 125
Chapter 5. The Fourier Transform on R 129
1 Elementary theory of the Fourier transform 131
1.1 Integration of functions on the real line 131
1.2 Definition of the Fourier transform 134
1.3 The Schwartz space 134
1.4 The Fourier transform on S 136
1.5 The Fourier inversion 140
1.6 The Plancherel formula 142
1.7 Extension to functions of moderate decrease 144
1.8 The Weierstrass approximation theorem 144
2 Applications to some partial differential equations 145
2.1 The time-dependent heat equation on the real line 145
2.2 The steady-state heat equation in the upper half-plane 149
3 The Poisson summation formula 153
3.1 Theta and zeta functions 155
3.2 Heat kernels 156
3.3 Poisson kernels 157
4 The Heisenberg uncertainty principle 158
5 Exercises 161
6 Problems 169
Chapter 6. The Fourier Transform on $\mathbb{R}^d$ 175
1 Preliminaries 176
1.1 Symmetries 176
1.2 Integration on $\mathbb{R}^d$ 178
2 Elementary theory of the Fourier transform 180
3 The wave equation in $\mathbb{R}^d\times\mathbb{R}$ 184
3.1 Solution in terms of Fourier transforms 184
3.2 The wave equation in $\mathbb{R}^3\times\mathbb{R}$ 189 

CONTENTS
3.3 The wave equation in $\mathbb{R}^2\times \mathbb{R}$ : descent 194
4 Radial symmetry and Bessel functions 196
5 The Radon transform and some of its applications 198
5.1 The X-ray transform in $\mathbb{R}^2$ 199
5.2 The Radon transform in $\mathbb{R}^3$ 201
5.3 A note about plane waves 207
6 Exercises 207
7 Problems 212
Chapter 7. Finite Fourier Analysis 218
1 Fourier analysis on $\mathbb{Z}(N)$ 219
1.1 The group $\mathbb{Z}(N)$ 219
1.2 Fourier inversion theorem and Plancherel identity on $\mathbb{Z}(N)$ 221
1.3 The fast Fourier transform 224
2 Fourier analysis on finite abelian groups 226
2.1 Abelian groups 226
2.2 Characters 230
2.3 The orthogonality relations 232
2.4 Characters as a total family 233
2.5 Fourier inversion and Plancherel formula 235
3 Exercises 236
4 Problems 239
Chapter 8. Dirichlet's Theorem 241
1 A little elementary number theory 241
1.1 The fundamental theorem of arithmetic 241
1.2 The infinitude of primes 244
2 Dirichlet's theorem 252
2.1 Fourier analysis, Dirichlet characters, and reduction of the theorem 254
2.2 Dirichlet $L$ -functions 255
3 Proof of the theorem 258
3.1 Logarithms 258
3.2 $L$ -functions 261
3.3 Non-vanishing of the $L$ -function 265
4 Exercises 275
5 Problems 279
Appendix: Integration 281
1 Definition of the Riemann integral 281 

xvi CONTENTS
1.1 Basic properties 282
1.2 Sets of measure zero and discontinuities of integrable functions 286
2 Multiple integrals 289
2.1 The Riemann integral in $\mathbb{R}^d$ 289
2.2 Repeated integrals 291
2.3 The change of variables formula 292
2.4 Spherical coordinates 293
3 Improper integrals. Integration over $\mathbb{R}^d$ 294
3.1 Integration of functions of moderate decrease 294
3.2 Repeated integrals 295
3.3 Spherical coordinates 297
Notes and References 298
Bibliography 300
Symbol Glossary 303
Index 305 

# 1 <sub>The</sub> <sub>Genesis</sub> <sub>of</sub> <sub>Fourier</sub> Analysis

Regarding the researches of d’Alembert and Euler could one not add that if they knew this expansion, they made but a very imperfect use of it. They were both persuaded that an arbitrary and discontinuous function could never be resolved in series of this kind, and it does not even seem that anyone had developed a constant in cosines of multiple arcs, the first problem which I had to solve in the theory of heat. 

J. Fourier, 1808-9 

In the beginning, it was the problem of the vibrating string, and the later investigation of heat flow, that led to the development of Fourier analysis. The laws governing these distinct physical phenomena were expressed by two diferent partial diferential equations, the wave and heat equations, and these were solved in terms of Fourier series. 

Here we want to start by describing in some detail the development of these ideas. We will do this initially in the context of the problem of the vibrating string, and we will proceed in three steps. First, we describe several physical (empirical) concepts which motivate corresponding mathematical ideas of importance for our study. These are: the role of the functions cos t, sin t, and $ e ^ { i t }$ suggested by simple harmonic motion; the use of separation of variables, derived from the phenomenon of standing waves; and the related concept of linearity, connected to the superposition of tones. Next, we derive the partial diferential equation which governs the motion of the vibrating string. Finally, we will use what we learned about the physical nature of the problem (expressed mathematically) to solve the equation. In the last section, we use the same approach to study the problem of heat difusion. 

Given the introductory nature of this chapter and the subject matter covered, our presentation cannot be based on purely mathematical reasoning. Rather, it proceeds by plausibility arguments and aims to provide the motivation for the further rigorous analysis in the succeeding chapters. The impatient reader who wishes to begin immediately with the theorems of the subject may prefer to pass directly to the next chapter. 

## 1 The vibrating string

The problem consists of the study of the motion of a string fixed at its end points and allowed to vibrate freely. We have in mind physical systems such as the strings of a musical instrument. As we mentioned above, we begin with a brief description of several observable physical phenomena on which our study is based. These are: 

• simple harmonic motion, 

• standing and traveling waves, 

• harmonics and superposition of tones. 

Understanding the empirical facts behind these phenomena will motivate our mathematical approach to vibrating strings. 

## Simple harmonic motion

Simple harmonic motion describes the behavior of the most basic oscil latory system (called the simple harmonic oscillator), and is therefore a natural place to start the study of vibrations. Consider a mass {m} attached to a horizontal spring, which itself is attached to a fixed wall, and assume that the system lies on a frictionless surface. 

Choose an axis whose origin coincides with the center of the mass when it is at rest (that is, the spring is neither stretched nor compressed), as shown in Figure 1. When the mass is displaced from its initial equilibrium 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/7c821043d8e8a356085a9f0c060d8d26bf6be069efe9f15ef0289fb8196d7fb4.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/c05eef0b42728e49f3141cdd346cba4c08cf4c38db24f8e88c878537b4e655e7.jpg)



Figure 1. Simple harmonic oscillator


position and then released, it will undergo simple harmonic motion. This motion can be described mathematically once we have found the diferential equation that governs the movement of the mass. 

Let y(t) denote the displacement of the mass at time t. We assume that the spring is ideal, in the sense that it satisfies Hooke’s law: the restoring force F exerted by the spring on the mass is given by $F = - k y ( t )$ . Here 

## 1. The vibrating string

$k > 0$ is a given physical quantity called the spring constant. Applying Newton’s law (force = mass × acceleration), we obtain 

$$
- k y (t) = m y ^ {\prime \prime} (t),
$$

where we use the notation $y ^ { \prime \prime }$ to denote the second derivative of $y$ with respect to t. With $c = \sqrt { k / m }$ , this second order ordinary diferential equation becomes 

$$
y ^ {\prime \prime} (t) + c ^ {2} y (t) = 0.\tag{1}
$$

The general solution of equation (1) is given by 

$$
y (t) = a \cos c t + b \sin c t,
$$

where a and b are constants. Clearly, all functions of this form solve equation (1), and Exercise 6 outlines a proof that these are the only (twice diferentiable) solutions of that diferential equation. 

In the above expression for $y ( t )$ , the quantity c is given, but a and b can be any real numbers. In order to determine the particular solution of the equation, we must impose two initial conditions in view of the two unknown constants a and b. For example, if we are given $y ( 0 )$ and $y ^ { \prime } ( 0 )$ , the initial position and velocity of the mass, then the solution of the physical problem is unique and given by 

$$
y (t) = y (0) \cos c t + \frac {y ^ {\prime} (0)}{c} \sin c t.
$$

One can easily verify that there exist constants $A > 0$ and $\varphi \in \mathbb { R }$ such that 

$$
a \cos c t + b \sin c t = A \cos (c t - \varphi).
$$

Because of the physical interpretation given above, one calls $A = \sqrt { a ^ { 2 } + b ^ { 2 } }$ the “amplitude” of the motion, c its “natural frequency,” ϕ its “phase” (uniquely determined up to an integer multiple of 2π), and $2 \pi / c$ the “period” of the motion. 

The typical graph of the function A cos(ct − ϕ), illustrated in Figure $^ { 2 , }$ exhibits a wavelike pattern that is obtained from translating and stretching (or shrinking) the usual graph of cos t. 

We make two observations regarding our examination of simple harmonic motion. The first is that the mathematical description of the most elementary oscillatory system, namely simple harmonic motion, involves 

Chapter 1. THE GENESIS OF FOURIER ANALYSIS 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/5b87f1c519b73a7a561735e11728a8e309f770d6614bff4fe052d771ddffb12c.jpg)



Figure 2. The graph of A cos(ct − ϕ)


the most basic trigonometric functions cos t and sin t. It will be important in what follows to recall the connection between these functions and complex numbers, as given in Euler’s identity $e ^ { i t } = \cos t + i$ sin t. The second observation is that simple harmonic motion is determined as a function of time by two initial conditions, one determining the position, and the other the velocity (specified, for example, at time $t = 0 )$ . This property is shared by more general oscillatory systems, as we shall see below. 

## Standing and traveling waves

As it turns out, the vibrating string can be viewed in terms of onedimensional wave motions. Here we want to describe two kinds of motions that lend themselves to simple graphic representations. 

• First, we consider standing waves. These are wavelike motions described by the graphs $y = u ( x , t )$ developing in time t as shown in Figure 3. 

In other words, there is an initial profile $y = \varphi ( x )$ representing the wave at time $t = 0$ , and an amplifying factor $\psi ( t )$ , depending on $t ,$ so that $y = u ( x , t )$ with 

$$
u (x, t) = \varphi (x) \psi (t).
$$

The nature of standing waves suggests the mathematical idea of “separation of variables,” to which we will return later. 

• A second type of wave motion that is often observed in nature is that of a traveling wave. Its description is particularly simple: 

1. The vibrating string 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/4d4558f0e5f66cb3981c2b09dd972525b8e3e662133cee10de617cb076807757.jpg)



Figure 3. A standing wave at diferent moments in time: $t = 0$ and $t = t _ { 0 }$


there is an initial profile $F ( x )$ so that $u ( x , t )$ equals $F ( x )$ when $t = 0$ . As t evolves, this profile is displaced to the right by ct units, where c is a positive constant, namely 

$$
u (x, t) = F (x - c t).
$$

Graphically, the situation is depicted in Figure 4. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/fc39c57590da58b6fd11af42c6a794be0cbf55b821d01d5833a6e0c94bea7102.jpg)



Figure 4. A traveling wave at two diferent moments in time: $t = 0$ and $t = t _ { 0 }$


Since the movement in t is at the rate c, that constant represents the velocity of the wave. The function $F ( x - c t )$ is a one-dimensional traveling wave moving to the right. Similarly, $u ( x , t ) = F ( x + c t )$ is a one-dimensional traveling wave moving to the left. 

## Harmonics and superposition of tones

The final physical observation we want to mention (without going into any details now) is one that musicians have been aware of since time immemorial. It is the existence of harmonics, or overtones. The pure tones are accompanied by combinations of overtones which are primarily responsible for the timbre (or tone color) of the instrument. The idea of combination or superposition of tones is implemented mathematically by the basic concept of linearity, as we shall see below. 

We now turn our attention to our main problem, that of describing the motion of a vibrating string. First, we derive the wave equation, that is, the partial diferential equation that governs the motion of the string. 

## 1.1 Derivation of the wave equation

Imagine a homogeneous string placed in the $( x , y ) – \mathrm { p l a n e }$ , and stretched along the x-axis between $x = 0$ and $x = L$ . If it is set to vibrate, its displacement $y = u ( x , t )$ is then a function of x and $t ,$ and the goal is to derive the diferential equation which governs this function. 

For this purpose, we consider the string as being subdivided into a large number N of masses (which we think of as individual particles) distributed uniformly along the x-axis, so that the $n ^ { \mathrm { t h } }$ particle has its x-coordinate at $x _ { n } = n L / N$ . We shall therefore conceive of the vibrating string as a complex system of N particles, each oscillating in the vertical direction only; however, unlike the simple harmonic oscillator we considered previously, each particle will have its oscillation linked to its immediate neighbor by the tension of the string. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/72ddecf0893bbf018409468647c81ebcb21cf6534d7f1cef813649d333e08592.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/ef74d23d4b328f404574ae34fa15e23807e06744a61319be65f103531324346a.jpg)



Figure 5. A vibrating string as a discrete system of masses


## 1. The vibrating string

We then set $y _ { n } ( t ) = u ( x _ { n } , t )$ , and note that $x _ { n + 1 } - x _ { n } = h$ , with $h =$ $L / N$ . If we assume that the string has constant density $\rho > 0$ , it is reasonable to assign mass equal to $\rho h$ to each particle. By Newton’s law, $\rho h y _ { n } ^ { \prime \prime } ( t )$ equals the force acting on the $n ^ { \mathrm { t h } }$ particle. We now make the simple assumption that this force is due to the efect of the two nearby particles, the ones with x-coordinates at $x _ { n - 1 }$ and $x _ { n + 1 }$ (see Figure 5). We further assume that the force (or tension) coming from the right of the $n ^ { \mathrm { t h } }$ particle is proportional to $( y _ { n + 1 } - y _ { n } ) / h$ , where h is the distance between $x _ { n + 1 }$ <sub>1</sub> and $x _ { n } ;$ hence we can write the tension as 

$$
\left(\frac {\tau}{h}\right) (y _ {n + 1} - y _ {n}),
$$

where $\tau > 0$ is a constant equal to the coeficient of tension of the string. There is a similar force coming from the left, and it is 

$$
\left(\frac {\tau}{h}\right) (y _ {n - 1} - y _ {n}).
$$

Altogether, adding these forces gives us the desired relation between the oscillators $y _ { n } ( t )$ , namely 

$$
\rho h y _ {n} ^ {\prime \prime} (t) = \frac {\tau}{h} \left\{y _ {n + 1} (t) + y _ {n - 1} (t) - 2 y _ {n} (t) \right\}.\tag{2}
$$

On the one hand, with the notation chosen above, we see that 

$$
y _ {n + 1} (t) + y _ {n - 1} (t) - 2 y _ {n} (t) = u \left(x _ {n} + h, t\right) + u \left(x _ {n} - h, t\right) - 2 u \left(x _ {n}, t\right).
$$

On the other hand, for any reasonable function $F ( x )$ (that is, one that has continuous second derivatives) we have 

$$
\frac {F (x + h) + F (x - h) - 2 F (x)}{h ^ {2}} \rightarrow F ^ {\prime \prime} (x) \quad \text { as } h \rightarrow 0.
$$

Thus we may conclude, after dividing by h in (2) and letting h tend to zero (that is, N goes to infinity), that 

$$
\rho \frac {\partial^ {2} u}{\partial t ^ {2}} = \tau \frac {\partial^ {2} u}{\partial x ^ {2}},
$$

or 

$$
\frac {1}{c ^ {2}} \frac {\partial^ {2} u}{\partial t ^ {2}} = \frac {\partial^ {2} u}{\partial x ^ {2}}, \quad \mathrm{with} c = \sqrt {\tau / \rho}.
$$

This relation is known as the one-dimensional wave equation, or more simply as the wave equation. For reasons that will be apparent later, the coeficient $c > 0$ is called the velocity of the motion. 

In connection with this partial diferential equation, we make an important simplifying mathematical remark. This has to do with scaling, or in the language of physics, a “change of units.” That is, we can think of the coordinate x as $x = a X$ where a is an appropriate positive constant. Now, in terms of the new coordinate X, the interval $0 \le x \le L$ becomes $0 \leq X \leq L / a$ . Similarly, we can replace the time coordinate t by $t = b T$ ， where b is another positive constant. If we set $U ( X , T ) = u ( x , t )$ , then 

$$
\frac {\partial U}{\partial X} = a \frac {\partial u}{\partial x}, \quad \frac {\partial^ {2} U}{\partial X ^ {2}} = a ^ {2} \frac {\partial^ {2} u}{\partial x ^ {2}},
$$

and similarly for the derivatives in t. So if we choose a and b appropriately, we can transform the one-dimensional wave equation into 

$$
\frac {\partial^ {2} U}{\partial T ^ {2}} = \frac {\partial^ {2} U}{\partial X ^ {2}},
$$

which has the efect of setting the velocity c equal to 1. Moreover, we have the freedom to transform the interval $0 \le x \le L$ to $0 \leq X \leq \pi$ . (We shall see that the choice of π is convenient in many circumstances.) All this is accomplished by taking $a = L / \pi$ and $b = L / ( c \pi )$ . Once we solve the new equation, we can of course return to the original equation by making the inverse change of variables. Hence, we do not sacrifice generality by thinking of the wave equation as given on the interval [0, π] with velocity $c = 1$ 

## 1.2 Solution to the wave equation

Having derived the equation for the vibrating string, we now explain two methods to solve it: 

• using traveling waves, 

• using the superposition of standing waves. 

While the first approach is very simple and elegant, it does not directly give full insight into the problem; the second method accomplishes that, and moreover is of wide applicability. It was first believed that the second method applied only in the simple cases where the initial position and velocity of the string were themselves given as a superposition of standing waves. However, as a consequence of Fourier’s ideas, it became clear that the problem could be worked either way for all initial conditions. 

## 1. The vibrating string

## Traveling waves

To simplify matters as before, we assume that $c = 1$ and $L = \pi$ , so that the equation we wish to solve becomes 

$$
\frac {\partial^ {2} u}{\partial t ^ {2}} = \frac {\partial^ {2} u}{\partial x ^ {2}} \quad \mathrm{on} 0 \leq x \leq \pi .
$$

The crucial observation is the following: if $F$ is any twice diferentiable function, then $u ( x , t ) = F ( x + t )$ and $u ( x , t ) = F ( x - t )$ solve the wave equation. The verification of this is a simple exercise in diferentiation. Note that the graph of $u ( x , t ) = F ( x - t )$ at time $t = 0$ is simply the graph of F, and that at time $t = 1$ it becomes the graph of $F$ translated to the right by 1. Therefore, we recognize that $F ( x - t )$ is a traveling wave which travels to the right with speed 1. Similarly, $u ( x , t ) = F ( x + t )$ is a wave traveling to the left with speed 1. These motions are depicted in Figure 6. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/998a7e663a11dded84736f668b07f1257f04fba82df9f11f6ab4d7673fc32859.jpg)



Figure 6. Waves traveling in both directions


Our discussion of tones and their combinations leads us to observe that the wave equation is linear. This means that if $u ( x , t )$ and $\boldsymbol { v } ( \boldsymbol { x } , t )$ are particular solutions, then so is $\alpha u ( x , t ) + \beta v ( x , t )$ , where $\alpha$ and $\beta$ are any constants. Therefore, we may superpose two waves traveling in opposite directions to find that whenever $F$ and G are twice diferentiable functions, then 

$$
u (x, t) = F (x + t) + G (x - t)
$$

is a solution of the wave equation. In fact, we now show that all solutions take this form. 

We drop for the moment the assumption that $0 \leq x \leq \pi$ , and suppose that u is a twice diferentiable function which solves the wave equation for all real x and t. Consider the following new set of variables $\xi = x + t ,$ $\eta = x - t ,$ , and define $v ( \xi , \eta ) = u ( x , t )$ . The change of variables formula shows that v satisfies 

$$
\frac {\partial^ {2} v}{\partial \xi \partial \eta} = 0.
$$

Integrating this relation twice gives $v ( \xi , \eta ) = F ( \xi ) + G ( \eta )$ , which then implies 

$$
u (x, t) = F (x + t) + G (x - t),
$$

for some functions F and $G .$ 

We must now connect this result with our original problem, that is, the physical motion of a string. There, we imposed the restrictions $0 \leq$ $x \leq \pi$ , the initial shape of the string $u ( x , 0 ) = f ( x )$ , and also the fact that the string has fixed end points, namely $u ( 0 , t ) = u ( \pi , t ) = 0$ for all t. To use the simple observation above, we first extend f to all of R by making it $\mathrm { o d d ^ { 1 } }$ on $[ - \pi , \pi ]$ , and then $\operatorname { p e r i o d i c } ^ { 2 }$ in x of period 2π, and similarly for $u ( x , t )$ , the solution of our problem. Then the extension u solves the wave equation on all of R, and $u ( x , 0 ) = f ( x )$ for all $x \in \mathbb { R }$ Therefore, $u ( x , t ) = F ( x + t ) + G ( x - t )$ , and setting $t = 0$ we find that 

$$
F (x) + G (x) = f (x).
$$

Since many choices of $F$ and $G$ will satisfy this identity, this suggests imposing another initial condition on u (similar to the two initial conditions in the case of simple harmonic motion), namely the initial velocity of the string which we denote by $g ( x )$ 

$$
\frac {\partial u}{\partial t} (x, 0) = g (x),
$$

where of course $g ( 0 ) = g ( \pi ) = 0$ . Again, we extend g to R first by making it odd over $[ - \pi , \pi ]$ , and then periodic of period $2 \pi$ . The two initial conditions of position and velocity now translate into the following system: 

$$
\left\{ \begin{array}{l} F (x) + G (x) = f (x), \\ F ^ {\prime} (x) - G ^ {\prime} (x) = g (x). \end{array} \right.
$$

## 1. The vibrating string

Diferentiating the first equation and adding it to the second, we obtain 

$$
2 F ^ {\prime} (x) = f ^ {\prime} (x) + g (x).
$$

Similarly 

$$
2 G ^ {\prime} (x) = f ^ {\prime} (x) - g (x),
$$

and hence there are constants $C _ { 1 }$ and $C _ { 2 }$ so that 

$$
F (x) = \frac {1}{2} \left[ f (x) + \int_ {0} ^ {x} g (y) d y \right] + C _ {1}
$$

and 

$$
G (x) = \frac {1}{2} \left[ f (x) - \int_ {0} ^ {x} g (y) d y \right] + C _ {2}.
$$

Since $F ( x ) + G ( x ) = f ( x )$ we conclude that ${ \cal C } _ { 1 } + { \cal C } _ { 2 } = 0 ,$ and therefore, our final solution of the wave equation with the given initial conditions takes the form 

$$
u (x, t) = \frac {1}{2} [ f (x + t) + f (x - t) ] + \frac {1}{2} \int_ {x - t} ^ {x + t} g (y) d y.
$$

The form of this solution is known as d’Alembert’s formula. Observe that the extensions we chose for $f$ and g guarantee that the string always has fixed ends, that is, $u ( 0 , t ) = u ( \pi , t ) = 0$ for all t. 

A final remark is in order. The passage from $t \geq 0$ to $t \in \mathbb { R }$ , and then back to $t \geq 0 .$ , which was made above, exhibits the time reversal property of the wave equation. In other words, a solution u to the wave equation for $t \geq 0$ , leads to a solution $u ^ { - }$ defined for negative time $t < 0$ simply by setting $u ^ { - } ( x , t ) = u ( x , - t )$ , a fact which follows from the invariance of the wave equation under the transformation $t \mapsto - t$ . The situation is quite diferent in the case of the heat equation. 

## Superposition of standing waves

We turn to the second method of solving the wave equation, which is based on two fundamental conclusions from our previous physical observations. By our considerations of standing waves, we are led to look for special solutions to the wave equation which are of the form $\varphi ( x ) \psi ( t )$ This procedure, which works equally well in other contexts (in the case of the heat equation, for instance), is called separation of variables and constructs solutions that are called pure tones. Then by the linearity of the wave equation, we can expect to combine these pure tones into a more complex combination of sound. Pushing this idea further, we can hope ultimately to express the general solution of the wave equation in terms of sums of these particular solutions. 

Note that one side of the wave equation involves only diferentiation in $x ,$ while the other, only diferentiation in t. This observation provides another reason to look for solutions of the equation in the form $u ( x , t ) = \varphi ( x ) \psi ( t )$ (that is, to “separate variables”), the hope being to reduce a dificult partial diferential equation into a system of simpler ordinary diferential equations. In the case of the wave equation, with u of the above form, we get 

$$
\varphi (x) \psi^ {\prime \prime} (t) = \varphi^ {\prime \prime} (x) \psi (t),
$$

and therefore 

$$
\frac {\psi^ {\prime \prime} (t)}{\psi (t)} = \frac {\varphi^ {\prime \prime} (x)}{\varphi (x)}.
$$

The key observation here is that the left-hand side depends only on $t ,$ and the right-hand side only on x. This can happen only if both sides are equal to a constant, say λ. Therefore, the wave equation reduces to the following 

$$
\left\{ \begin{array}{l l} \psi^ {\prime \prime} (t) - \lambda \psi (t) = 0 \\ \varphi^ {\prime \prime} (x) - \lambda \varphi (x) = 0. \end{array} \right.\tag{3}
$$

We focus our attention on the first equation in the above system. At this point, the reader will recognize the equation we obtained in the study of simple harmonic motion. Note that we need to consider only the case when $\lambda < 0 ,$ , since when $\lambda \geq 0$ the solution $\psi$ will not oscillate as time varies. Therefore, we may write $\lambda = - m ^ { 2 }$ , and the solution of the equation is then given by 

$$
\psi (t) = A \cos m t + B \sin m t.
$$

Similarly, we find that the solution of the second equation in (3) is 

$$
\varphi (x) = \tilde {A} \cos m x + \tilde {B} \sin m x.
$$

Now we take into account that the string is attached at $x = 0$ and $x = \pi$ This translates into $\varphi ( 0 ) = \varphi ( \pi ) = 0$ , which in turn gives $\tilde { A } = 0$ , and if $\tilde { B } \neq 0$ , then m must be an integer. If $m = 0 ,$ , the solution vanishes identically, and if $m \le - 1$ , we may rename the constants and reduce to 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/adbe491558f7e422dc11ececb2a6b56ae4b6c3a6260a05d1fffeb93f8f8fd775.jpg)


## 1. The vibrating string

the case $m \geq 1$ since the function sin y is odd and cos y is even. Finally, we arrive at the guess that for each $m \geq 1$ , the function 

$$
u _ {m} (x, t) = (A _ {m} \cos m t + B _ {m} \sin m t) \sin m x,
$$

which we recognize as a standing wave, is a solution to the wave equation. Note that in the above argument we divided by $\varphi$ and $\psi ,$ , which sometimes vanish, so one must actually check by hand that the standing wave $u _ { m }$ solves the equation. This straightforward calculation is left as an exercise to the reader. 

Before proceeding further with the analysis of the wave equation, we pause to discuss standing waves in more detail. The terminology comes from looking at the graph of $u _ { m } ( x , t )$ for each fixed t. Suppose first that $m = 1$ , and take $u ( x , t ) = \cos t$ sin x. Then, Figure $7 \ \mathrm { { ( a ) } }$ gives the graph of u for diferent values of t. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/645ad53bb15b460ad29af5e9d7a93b9b05eebc68ee7be1d4ad9be13ff4d881e0.jpg)



(a)



(b)



Figure 7. Fundamental tone (a) and overtones (b) at diferent moments in time


The case $m = 1$ corresponds to the fundamental tone or first harmonic of the vibrating string. 

We now take $m = 2$ and look at $u ( x , t ) = \cos 2 t \sin 2 x$ This corresponds to the first overtone or second harmonic, and this motion is described in Figure $7 \ ( \mathrm { b } )$ . Note that $u ( \pi / 2 , t ) = 0$ for all t. Such points, which remain motionless in time, are called nodes, while points whose motion has maximum amplitude are named anti-nodes. 

For higher values of m we get more overtones or higher harmonics. Note that as m increases, the frequency increases, and the period $2 \pi / m$ decreases. Therefore, the fundamental tone has a lower frequency than the overtones. 

We now return to the original problem. Recall that the wave equation is linear in the sense that if u and v solve the equation, so does $\alpha u + \beta v$ for any constants $\alpha$ and $\beta .$ This allows us to construct more solutions by taking linear combinations of the standing waves $u _ { m }$ . This technique, called superposition, leads to our final guess for a solution of the wave equation 

$$
u (x, t) = \sum_ {m = 1} ^ {\infty} \left(A _ {m} \cos m t + B _ {m} \sin m t\right) \sin m x.\tag{4}
$$

Note that the above sum is infinite, so that questions of convergence arise, but since most of our arguments so far are formal, we will not worry about this point now. 

Suppose the above expression gave all the solutions to the wave equation. If we then require that the initial position of the string at time $t = 0$ is given by the shape of the graph of the function $f$ on $[ 0 , \pi ]$ , with of course $f ( 0 ) = f ( \pi ) = 0$ , we would have $u ( x , 0 ) = f ( x )$ , hence 

$$
\sum_ {m = 1} ^ {\infty} A _ {m} \sin m x = f (x).
$$

Since the initial shape of the string can be any reasonable function $f ,$ we must ask the following basic question: 

Given a function $f$ on [0, π] (with $f ( 0 ) = f ( \pi ) = 0 )$ , can we find coeficients $A _ { m }$ so that 

$$
f (x) = \sum_ {m = 1} ^ {\infty} A _ {m} \sin m x?\tag{5}
$$

This question is stated loosely, but a lot of our efort in the next two chapters of this book will be to formulate the question precisely and attempt to answer it. This was the basic problem that initiated the study of Fourier analysis. 

A simple observation allows us to guess a formula giving $A _ { m }$ if the expansion (5) were to hold. Indeed, we multiply both sides by sin nx 

## 1. The vibrating string

and integrate between $[ 0 , \pi ] ;$ working formally, we obtain 

$$
\begin{array}{c} \int_ {0} ^ {\pi} f (x) \sin n x d x = \int_ {0} ^ {\pi} \left(\sum_ {m = 1} ^ {\infty} A _ {m} \sin m x\right) \sin n x d x \\ = \sum_ {m = 1} ^ {\infty} A _ {m} \int_ {0} ^ {\pi} \sin m x \sin n x d x = A _ {n} \cdot \frac {\pi}{2}, \end{array}
$$

where we have used the fact that 

$$
\int_ {0} ^ {\pi} \sin m x \sin n x d x = \left\{ \begin{array}{l l} 0 & \mathrm{if} m \neq n, \\ \pi / 2 & \mathrm{if} m = n. \end{array} \right.
$$

Therefore, the guess for $A _ { n } ,$ , called the $n ^ { \mathrm { t h } }$ Fourier sine coeficient of $f ,$ is 

$$
A _ {n} = \frac {2}{\pi} \int_ {0} ^ {\pi} f (x) \sin n x d x.\tag{6}
$$

We shall return to this formula, and other similar ones, later. 

One can transform the question about Fourier sine series on $[ 0 , \pi ]$ to a more general question on the interval $[ - \pi , \pi ]$ . If we could express f on $[ 0 , \pi ]$ in terms of a sine series, then this expansion would also hold on $[ - \pi , \pi ]$ if we extend $f$ to this interval by making it odd. Similarly, one can ask if an even function $g ( x )$ on $[ - \pi , \pi ]$ can be expressed as a cosine series, namely 

$$
g (x) = \sum_ {m = 0} ^ {\infty} A _ {m} ^ {\prime} \cos m x.
$$

More generally, since an arbitrary function $F$ on $[ - \pi , \pi ]$ can be expressed as $f + g ,$ where $f$ is odd and $g$ is $\mathrm { e v e n } , { } ^ { 3 }$ we may ask if $F$ can be written as 

$$
F (x) = \sum_ {m = 1} ^ {\infty} A _ {m} \sin m x + \sum_ {m = 0} ^ {\infty} A _ {m} ^ {\prime} \cos m x,
$$

or by applying Euler’s identity $e ^ { i x } = \cos x + i \sin x$ , we could hope that $F$ takes the form 

$$
F (x) = \sum_ {m = - \infty} ^ {\infty} a _ {m} e ^ {i m x}.
$$

By analogy with (6), we can use the fact that 

$$
\frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} e ^ {i m x} e ^ {- i n x}   d x = \left\{ \begin{array}{l l} 0 & \text {if} n \neq m \\ 1 & \text {if} n = m, \end{array} \right.
$$

to see that one expects that 

$$
a _ {n} = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} F (x) e ^ {- i n x} d x.
$$

The quantity $a _ { n }$ is called the $n ^ { \mathrm { t h } }$ Fourier coeficient of $F .$ We can now reformulate the problem raised above: 

Question: Given any reasonable function F on $[ - \pi , \pi ]$ , with Fourier coeficients defined above, is it true that 

$$
F (x) = \sum_ {m = - \infty} ^ {\infty} a _ {m} e ^ {i m x}?\tag{7}
$$

This formulation of the problem, in terms of complex exponentials, is the form we shall use the most in what follows. 

Joseph Fourier (1768-1830) was the first to believe that an “arbitrary” function F could be given as a series (7). In other words, his idea was that any function is the linear combination (possibly infinite) of the most basic trigonometric functions sin mx and cos mx, where m ranges over the integers.<sup>4</sup> Although this idea was implicit in earlier work, Fourier had the conviction that his predecessors lacked, and he used it in his study of heat difusion; this began the subject of “Fourier analysis.” This discipline, which was first developed to solve certain physical problems, has proved to have many applications in mathematics and other fields as well, as we shall see later. 

We return to the wave equation. To formulate the problem correctly, we must impose two initial conditions, as our experience with simple harmonic motion and traveling waves indicated. The conditions assign the initial position and velocity of the string. That is, we require that u satisfy the diferential equation and the two conditions 

$$
u (x, 0) = f (x) \quad \mathrm{and} \quad {\frac {\partial u}{\partial t}} (x, 0) = g (x),
$$

## 1. The vibrating string

where f and $g$ are pre-assigned functions. Note that this is consistent with (4) in that this requires that f and g be expressible as 

$$
f (x) = \sum_ {m = 1} ^ {\infty} A _ {m} \sin m x \quad \text { and } \quad g (x) = \sum_ {m = 1} ^ {\infty} m B _ {m} \sin m x.
$$

## 1.3 Example: the plucked string

We now apply our reasoning to the particular problem of the plucked string. For simplicity we choose units so that the string is taken on the interval $[ 0 , \pi ]$ , and it satisfies the wave equation with $c = 1$ . The string is assumed to be plucked to height h at the point p with $0 < p < \pi ;$ this is the initial position. That is, we take as our initial position the triangular shape given by 

$$
f (x) = \left\{ \begin{array}{l l} \frac {x h}{p} & \text { for } 0 \leq x \leq p \\ \frac {h (\pi - x)}{\pi - p} & \text { for } p \leq x \leq \pi , \end{array} \right.
$$

which is depicted in Figure 8. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/fa606447457d3dfe024b8d1e8ea8d9e5741a6c2602b4ebef32bec30845ec8912.jpg)



Figure 8. Initial position of a plucked string


We also choose an initial velocity $g ( x )$ identically equal to 0. Then, we can compute the Fourier coeficients of $f$ (Exercise 9), and assuming that the answer to the question raised before (5) is positive, we obtain 

$$
f (x) = \sum_ {m = 1} ^ {\infty} A _ {m} \sin m x \quad \mathrm{with} \quad A _ {m} = \frac {2 h}{m ^ {2}} \frac {\sin m p}{p (\pi - p)}.
$$

Thus 

$$
u (x, t) = \sum_ {m = 1} ^ {\infty} A _ {m} \cos m t \sin m x,\tag{8}
$$

and note that this series converges absolutely. The solution can also be expressed in terms of traveling waves. In fact 

$$
u (x, t) = \frac {f (x + t) + f (x - t)}{2}.\tag{9}
$$

Here $f ( x )$ is defined for all x as follows: first, $f$ is extended to $[ - \pi , \pi ]$ by making it odd, and then $f$ is extended to the whole real line by making it periodic of period $2 \pi$ , that is, $f ( x + 2 \pi k ) = f ( x )$ for all integers $k .$ 

Observe that (8) implies (9) in view of the trigonometric identity 

$$
\cos v \sin u = \frac {1}{2} [ \sin (u + v) + \sin (u - v) ].
$$

As a final remark, we should note an unsatisfactory aspect of the solution to this problem, which however is in the nature of things. Since the initial data $f ( x )$ for the plucked string is not twice continuously differentiable, neither is the function u (given by (9)). Hence u is not truly a solution of the wave equation: while $u ( x , t )$ does represent the position of the plucked string, it does not satisfy the partial diferential equation we set out to solve! This state of afairs may be understood properly only if we realize that u does solve the equation, but in an appropriate generalized sense. A better understanding of this phenomenon requires ideas relevant to the study of “weak solutions” and the theory of “distributions.” These topics we consider only later, in Books III and IV. 

## 2 The heat equation

We now discuss the problem of heat difusion by following the same framework as for the wave equation. First, we derive the time-dependent heat equation, and then study the steady-state heat equation in the disc, which leads us back to the basic question (7). 

## 2.1 Derivation of the heat equation

Consider an infinite metal plate which we model as the plane $\mathbb { R } ^ { 2 }$ , and suppose we are given an initial heat distribution at time $t = 0$ . Let the temperature at the point $( x , y )$ at time t be denoted by $u ( x , y , t )$ 

## 2. The heat equation

Consider a small square centered at $( x _ { 0 } , y _ { 0 } )$ with sides parallel to the axis and of side length $h ,$ as shown in Figure 9. The amount of heat energy in S at time t is given by 

$$
H (t) = \sigma \iint_ {S} u (x, y, t) d x d y,
$$

where $\sigma > 0$ is a constant called the specific heat of the material. Therefore, the heat flow into S is 

$$
\frac {\partial H}{\partial t} = \sigma \iint_ {S} \frac {\partial u}{\partial t} d x d y,
$$

which is approximately equal to 

$$
\sigma h ^ {2} \frac {\partial u}{\partial t} (x _ {0}, y _ {0}, t),
$$

since the area of S is $h ^ { 2 }$ . Now we apply Newton’s law of cooling, which states that heat flows from the higher to lower temperature at a rate proportional to the diference, that is, the gradient. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/afb1799c310f9e0255e18814e4d17b698e6bad3b947bd30d3fc3dafe28fc8421.jpg)



Figure 9. Heat flow through a small square


The heat flow through the vertical side on the right is therefore 

$$
- \kappa h \frac {\partial u}{\partial x} (x _ {0} + h / 2, y _ {0}, t),
$$

where $\kappa > 0$ is the conductivity of the material. A similar argument for the other sides shows that the total heat flow through the square $S$ is 

given by 

$$
\begin{array}{l} \kappa h \left[ \frac {\partial u}{\partial x} (x _ {0} + h / 2, y _ {0}, t) - \frac {\partial u}{\partial x} (x _ {0} - h / 2, y _ {0}, t) \right. \\ \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad + \frac {\partial u}{\partial y} (x _ {0}, y _ {0} + h / 2, t) - \frac {\partial u}{\partial y} (x _ {0}, y _ {0} - h / 2, t) \Bigg ]. \end{array}
$$

Applying the mean value theorem and letting h tend to zero, we find that 

$$
\frac {\sigma}{\kappa} \frac {\partial u}{\partial t} = \frac {\partial^ {2} u}{\partial x ^ {2}} + \frac {\partial^ {2} u}{\partial y ^ {2}};
$$

this is called the time-dependent heat equation, often abbreviated to the heat equation. 

## 2.2 Steady-state heat equation in the disc

After a long period of time, there is no more heat exchange, so that the system reaches thermal equilibrium and $\partial u / \partial t = 0 .$ . In this case, the time-dependent heat equation reduces to the steady-state heat equation 

$$
\frac {\partial^ {2} u}{\partial x ^ {2}} + \frac {\partial^ {2} u}{\partial y ^ {2}} = 0.\tag{10}
$$

The operator $\partial ^ { 2 } / \partial x ^ { 2 } + \partial ^ { 2 } / \partial y ^ { 2 }$ is of such importance in mathematics and physics that it is often abbreviated as $\triangle$ and given a name: the Laplace operator or Laplacian. So the steady-state heat equation is written as 

$$
\triangle u = 0,
$$

and solutions to this equation are called harmonic functions. 

Consider the unit disc in the plane 

$$
D = \{(x, y) \in \mathbb {R} ^ {2}: x ^ {2} + y ^ {2} <   1 \},
$$

whose boundary is the unit circle $C .$ In polar coordinates $( r , \theta )$ , with $0 \leq r$ and $0 \leq \theta < 2 \pi$ , we have 

$$
D = \{(r, \theta): 0 \leq r <   1 \} \quad \text { and } \quad C = \{(r, \theta): r = 1 \}.
$$

The problem, often called the Dirichlet problem (for the Laplacian on the unit disc), is to solve the steady-state heat equation in the unit 

## 2. The heat equation

disc subject to the boundary condition $u = f$ on C. This corresponds to fixing a predetermined temperature distribution on the circle, waiting a long time, and then looking at the temperature distribution inside the disc. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/008b88b5e4f8243573b8d2ef7144d7615eed29dce21ae978d512d3f0cbc8ff74.jpg)



Figure 10. The Dirichlet problem for the disc


While the method of separation of variables will turn out to be useful for equation (10), a dificulty comes from the fact that the boundary condition is not easily expressed in terms of rectangular coordinates. Since this boundary condition is best described by the coordinates $( r , \theta )$ • namely $u ( 1 , \theta ) = f ( \theta )$ , we rewrite the Laplacian in polar coordinates. An application of the chain rule gives (Exercise 10): 

$$
\triangle u = \frac {\partial^ {2} u}{\partial r ^ {2}} + \frac {1}{r} \frac {\partial u}{\partial r} + \frac {1}{r ^ {2}} \frac {\partial^ {2} u}{\partial \theta^ {2}}.
$$

We now multiply both sides by $r ^ { 2 }$ , and since $\triangle u = 0$ , we get 

$$
r ^ {2} \frac {\partial^ {2} u}{\partial r ^ {2}} + r \frac {\partial u}{\partial r} = - \frac {\partial^ {2} u}{\partial \theta^ {2}}.
$$

Separating these variables, and looking for a solution of the form $u ( r , \theta ) = F ( r ) G ( \theta )$ , we find 

$$
\frac {r ^ {2} F ^ {\prime \prime} (r) + r F ^ {\prime} (r)}{F (r)} = - \frac {G ^ {\prime \prime} (\theta)}{G (\theta)}.
$$

Since the two sides depend on diferent variables, they must both be constant, say equal to λ. We therefore get the following equations: 

$$
\left\{ \begin{array}{l l} G ^ {\prime \prime} (\theta) + \lambda G (\theta) = 0, \\ r ^ {2} F ^ {\prime \prime} (r) + r F ^ {\prime} (r) - \lambda F (r) = 0. \end{array} \right.
$$

Since $G$ must be periodic of period $2 \pi$ , this implies that $\lambda \geq 0$ and (as we have seen before) that $\lambda = m ^ { 2 }$ where m is an integer; hence 

$$
G (\theta) = \tilde {A} \cos m \theta + \tilde {B} \sin m \theta .
$$

An application of Euler’s identity, $e ^ { i x } = \cos x + i$ sin x, allows one to rewrite G in terms of complex exponentials, 

$$
G (\theta) = A e ^ {i m \theta} + B e ^ {- i m \theta}.
$$

With $\lambda = m ^ { 2 }$ and m 6= 0, two simple solutions of the equation in $F$ are $F ( r ) = r ^ { m }$ and $F ( r ) = r ^ { - m }$ (Exercise 11 gives further information about these solutions). If $m = 0 .$ , then $F ( r ) = 1$ and $F ( r ) = \log r$ are two solutions. If $m > 0$ , we note that $r ^ { - m }$ grows unboundedly large as $r$ tends to zero, so $F ( r ) G ( \theta )$ is unbounded at the origin; the same occurs when $m = 0$ and $F ( r ) = \log r$ . We reject these solutions as contrary to our intuition. Therefore, we are left with the following special functions: 

$$
u _ {m} (r, \theta) = r ^ {| m |} e ^ {i m \theta}, \quad m \in \mathbb {Z}.
$$

We now make the important observation that (10) is linear , and so as in the case of the vibrating string, we may superpose the above special solutions to obtain the presumed general solution: 

$$
u (r, \theta) = \sum_ {m = - \infty} ^ {\infty} a _ {m} r ^ {| m |} e ^ {i m \theta}.
$$

If this expression gave all the solutions to the steady-state heat equation, then for a reasonable f we should have 

$$
u (1, \theta) = \sum_ {m = - \infty} ^ {\infty} a _ {m} e ^ {i m \theta} = f (\theta).
$$

We therefore ask again in this context: given any reasonable function $f$ on [0, 2π] with $f ( 0 ) = f ( 2 \pi )$ , can we find coeficients $a _ { m }$ so that 

$$
f (\theta) = \sum_ {m = - \infty} ^ {\infty} a _ {m} e ^ {i m \theta}?
$$

## 3. Exercises

Historical Note: D’Alembert (in 1747) first solved the equation of the vibrating string using the method of traveling waves. This solution was elaborated by Euler a year later. In 1753, D. Bernoulli proposed the solution which for all intents and purposes is the Fourier series given by (4), but Euler was not entirely convinced of its full generality, since this could hold only if an “arbitrary” function could be expanded in Fourier series. D’Alembert and other mathematicians also had doubts. This viewpoint was changed by Fourier (in 1807) in his study of the heat equation, where his conviction and work eventually led others to a complete proof that a general function could be represented as a Fourier series. 

## 3 Exercises

1. I $\mathrm { ~ f ~ } z = x + i y$ is a complex number with $x , y \in \mathbb { R }$ , we define 

$$
| z | = (x ^ {2} + y ^ {2}) ^ {1 / 2}
$$

and call this quantity the modulus or absolute value of $z .$ 

(a) What is the geometric interpretation of $| z | \cdot 2$ 

(b) Show that $\mathrm { i f } \ | z | = 0$ , then $z = 0$ 

(c) Show that if $\lambda \in \mathbb { R }$ , then $| \lambda z | = | \lambda | | z |$ , where $| \lambda |$ denotes the standard absolute value of a real number. 

(d) If z<sub>1</sub> and z<sub>2</sub> are two complex numbers, prove that 

$$
| z _ {1} z _ {2} | = | z _ {1} | | z _ {2} | \quad \text { and } \quad | z _ {1} + z _ {2} | \leq | z _ {1} | + | z _ {2} |.
$$

(e) Show that $\mathrm { i f } \ z \ne 0$ , then $| 1 / z | = 1 / | z |$ 

2. If $z = x + i y$ is a complex number with $x , y \in \mathbb { R }$ , we define the complex conjugate of z by 

$$
\overline {{z}} = x - i y.
$$

(a) What is the geometric interpretation of $\overline { { z } } ?$ 

(b) Show that $| z | ^ { 2 } = z { \overline { { z } } }$ 

(c) Prove that if z belongs to the unit circle, then $1 / z = { \overline { { z } } } .$ 

3. A sequence of complex numbers $\{ w _ { n } \} _ { n = 1 } ^ { \infty }$ is said to converge if there exists $w \in \mathbb { C }$ such that 

$$
\lim _ {n \to \infty} | w _ {n} - w | = 0,
$$

and we say that w is a limit of the sequence. 

(a) Show that a converging sequence of complex numbers has a unique limit. 

The sequence $\{ w _ { n } \} _ { n = 1 } ^ { \infty }$ is said to be a Cauchy sequence if for every $\epsilon > 0$ there exists a positive integer N such that 

$$
\left| w _ {n} - w _ {m} \right| <   \epsilon \quad \text { whenever } n, m > N.
$$

(b) Prove that a sequence of complex numbers converges if and only if it is a Cauchy sequence. [Hint: A similar theorem exists for the convergence of a sequence of real numbers. Why does it carry over to sequences of complex numbers?] 

A series $\textstyle \sum _ { n = 1 } ^ { \infty } z _ { n }$ of complex numbers is said to converge if the sequence formed by the partial sums 

$$
S _ {N} = \sum_ {n = 1} ^ {N} z _ {n}
$$

converges. Let $\{ a _ { n } \} _ { n = 1 } ^ { \infty }$ be a sequence of non-negative real numbers such that the series $\textstyle \sum _ { n } a _ { n }$ converges. 

(c) Show that if $\{ z _ { n } \} _ { n = 1 } ^ { \infty }$ is a sequence of complex numbers satisfying $| z _ { n } | \leq a _ { n }$ for all $n ,$ then the series $\sum z _ { n }$ converges. [Hint: Use the Cauchy criterion.] 

4. For $z \in \mathbb { C } .$ we define the complex exponential by 

$$
e ^ {z} = \sum_ {n = 0} ^ {\infty} \frac {z ^ {n}}{n !}.
$$

(a) Prove that the above definition makes sense, by showing that the series converges for every complex number z. Moreover, show that the convergence is uniform<sup>5</sup> on every bounded subset of C. 

(b) If $z _ { 1 } , z _ { 2 }$ are two complex numbers, prove that $e ^ { z _ { 1 } } e ^ { z _ { 2 } } = e ^ { z _ { 1 } + z _ { 2 } }$ . [Hint: Use the binomial theorem to expand $( z _ { 1 } + z _ { 2 } ) ^ { n }$ , as well as the formula for the binomial coeficients.] 

3. Exercises 

(c) Show that if z is purely imaginary, that is, $z = i y$ with $y \in \mathbb R$ , then 

$$
e ^ {i y} = \cos y + i \sin y.
$$

This is Euler’s identity. [Hint: Use power series.] 

(d) More generally, 

$$
e ^ {x + i y} = e ^ {x} (\cos y + i \sin y)
$$

whenever $x , y \in \mathbb { R }$ , and show that 

$$
| e ^ {x + i y} | = e ^ {x}.
$$

(e) Prove that $e ^ { z } = 1$ if and only $\mathrm { i f } \ z = 2 \pi k i$ for some integer k. 

(f) Show that every complex number $z = x + i y$ can be written in the form 

$$
z = r e ^ {i \theta},
$$

where r is unique and in the range $0 \leq r < \infty$ , and $\theta \in \mathbb { R }$ is unique up to an integer multiple of 2π. Check that 

$$
r = | z | \quad \mathrm{and} \quad \theta = \arctan (y / x)
$$

whenever these formulas make sense. 

(g) In particular, $i = e ^ { i \pi / 2 }$ . What is the geometric meaning of multiplying a complex number by i? Or by $e ^ { i \theta }$ for any $\theta \in \mathbb { R } ?$ 

(h) Given $\theta \in \mathbb { R } .$ , show that 

$$
\cos \theta = \frac {e ^ {i \theta} + e ^ {- i \theta}}{2} \quad \mathrm{and} \quad \sin \theta = \frac {e ^ {i \theta} - e ^ {- i \theta}}{2 i}.
$$

These are also called Euler’s identities. 

(i) Use the complex exponential to derive trigonometric identities such as 

$$
\cos (\theta + \vartheta) = \cos \theta \cos \vartheta - \sin \theta \sin \vartheta ,
$$

and then show that 

$$
\begin{array}{r c l} {2 \sin \theta \sin \varphi} & = & {\cos (\theta - \varphi) - \cos (\theta + \varphi),} \\ {2 \sin \theta \cos \varphi} & = & {\sin (\theta + \varphi) + \sin (\theta - \varphi).} \end{array}
$$

This calculation connects the solution given by d’Alembert in terms of traveling waves and the solution in terms of superposition of standing waves. 

5. Verify that $f ( x ) = e ^ { i n x }$ is periodic with period $2 \pi$ and that 

$$
\frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} e ^ {i n x} d x = \left\{ \begin{array}{l l} 1 & \text {if} n = 0, \\ 0 & \text {if} n \neq 0. \end{array} \right.
$$

Use this fact to prove that if $n , m \geq 1$ we have 

$$
\frac {1}{\pi} \int_ {- \pi} ^ {\pi} \cos n x \cos m x d x = \left\{ \begin{array}{l l} 0 & \text {if} n \neq m, \\ 1 & n = m, \end{array} \right.
$$

and similarly 

$$
\frac {1}{\pi} \int_ {- \pi} ^ {\pi} \sin n x \sin m x d x = \left\{ \begin{array}{l l} 0 & \text {if} n \neq m, \\ 1 & n = m. \end{array} \right.
$$

Finally, show that 

$$
\int_ {- \pi} ^ {\pi} \sin n x \cos m x d x = 0 \quad \text { for   any } n, m.
$$

[Hint: Calculate $e ^ { i n x } e ^ { . }$ −imx $+ e ^ { i n x } e ^ { i m x }$ and $e ^ { i n x } e ^ { - i m x } - e ^ { i n x } e ^ { i m x } . ]$ 

6. Prove that if $f$ is a twice continuously diferentiable function on R which is a solution of the equation 

$$
f ^ {\prime \prime} (t) + c ^ {2} f (t) = 0,
$$

then there exist constants a and b such that 

$$
f (t) = a \cos c t + b \sin c t.
$$

This can be done by diferentiating the two functions $g ( t ) = f ( t ) \cos c t - c ^ { - 1 } f ^ { \prime } ( t )$ sin ct and $h ( t ) = f ( t )$ sin $c t + c ^ { - 1 } f ^ { \prime } ( t )$ cos ct. 

7. Show that if a and b are real, then one can write 

$$
a \cos c t + b \sin c t = A \cos (c t - \varphi),
$$

where $A = \sqrt { a ^ { 2 } + b ^ { 2 } }$ , and $\varphi$ is chosen so that 

$$
\cos \varphi = \frac {a}{\sqrt {a ^ {2} + b ^ {2}}} \quad \mathrm{and} \quad \sin \varphi = \frac {b}{\sqrt {a ^ {2} + b ^ {2}}}.
$$

8. Suppose $F$ is a function on $( a , b )$ with two continuous derivatives. Show that whenever x and $x + h$ belong to $( a , b )$ , one may write 

$$
F (x + h) = F (x) + h F ^ {\prime} (x) + \frac {h ^ {2}}{2} F ^ {\prime \prime} (x) + h ^ {2} \varphi (h),
$$

## 4. Problem

where $\varphi ( h ) \to 0$ as $h \to 0$ 

Deduce that 

$$
\frac {F (x + h) + F (x - h) - 2 F (x)}{h ^ {2}} \to F ^ {\prime \prime} (x) \quad \text { as } h \to 0.
$$

[Hint: This is simply a Taylor expansion. It may be obtained by noting that 

$$
F (x + h) - F (x) = \int_ {x} ^ {x + h} F ^ {\prime} (y) d y,
$$

and then writing $F ^ { \prime } ( y ) = F ^ { \prime } ( x ) + ( y - x ) F ^ { \prime \prime } ( x ) + ( y - x ) \psi ( y - x )$ , where $\psi ( h ) $ 0 as $h  0 . ]$ 

9. In the case of the plucked string, use the formula for the Fourier sine coeficients to show that 

$$
A _ {m} = \frac {2 h}{m ^ {2}} \frac {\sin m p}{p (\pi - p)}.
$$

For what position of $p$ are the second, fourth, $\cdot \cdot \cdot$ harmonics missing? For what position of $p$ are the third, sixth $, \dots ,$ harmonics missing? 

10. Show that the expression of the Laplacian 

$$
\triangle = \frac {\partial^ {2}}{\partial x ^ {2}} + \frac {\partial^ {2}}{\partial y ^ {2}}
$$

is given in polar coordinates by the formula 

$$
\triangle = \frac {\partial^ {2}}{\partial r ^ {2}} + \frac {1}{r} \frac {\partial}{\partial r} + \frac {1}{r ^ {2}} \frac {\partial^ {2}}{\partial \theta^ {2}}.
$$

Also, prove that 

$$
\left| \frac {\partial u}{\partial x} \right| ^ {2} + \left| \frac {\partial u}{\partial y} \right| ^ {2} = \left| \frac {\partial u}{\partial r} \right| ^ {2} + \frac {1}{r ^ {2}} \left| \frac {\partial u}{\partial \theta} \right| ^ {2}.
$$

11. Show that if $n \in \mathbb { Z }$ the only solutions of the diferential equation 

$$
r ^ {2} F ^ {\prime \prime} (r) + r F ^ {\prime} (r) - n ^ {2} F (r) = 0,
$$

which are twice diferentiable when $r > 0 .$ , are given by linear combinations of $r ^ { n }$ and $r ^ { - n }$ when $n \neq 0 ,$ and 1 and log r when $n = 0$ 

[Hint: If $F$ solves the equation, write $\begin{array} { r } { F ( r ) = g ( r ) r ^ { n } } \end{array}$ , find the equation satisfied by $^ { g , }$ and conclude that $r g ^ { \prime } ( r ) + 2 n g ( r ) = c$ where c is a constant.] 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/1fcf9f950bc9a4d7bf93c39560d8002407a819b9312b202faeee083ae5fd00dd.jpg)



Figure 11. Dirichlet problem in a rectangle


## 4 Problem

1. Consider the Dirichlet problem illustrated in Figure 11. 

More precisely, we look for a solution of the steady-state heat equation $\triangle u = 0$ in the rectangle $R = \left\{ ( x , y ) : ~ 0 \leq x \leq \pi , ~ 0 \leq y \leq 1 \right\}$ that vanishes on the vertical sides of $R ,$ and so that 

$$
u (x, 0) = f _ {0} (x) \quad \text { and } \quad u (x, 1) = f _ {1} (x),
$$

where $f _ { 0 }$ and $f _ { 1 }$ are initial data which fix the temperature distribution on the horizontal sides of the rectangle. 

Use separation of variables to show that if $f _ { 0 }$ and $f _ { 1 }$ have Fourier expansions 

$$
f _ {0} (x) = \sum_ {k = 1} ^ {\infty} A _ {k} \sin k x \quad \text { and } \quad f _ {1} (x) = \sum_ {k = 1} ^ {\infty} B _ {k} \sin k x,
$$

then 

$$
u (x, y) = \sum_ {k = 1} ^ {\infty} \left(\frac {\sinh k (1 - y)}{\sinh k} A _ {k} + \frac {\sinh k y}{\sinh k} B _ {k}\right) \sin k x.
$$

We recall the definitions of the hyperbolic sine and cosine functions: 

$$
\sinh x = \frac {e ^ {x} - e ^ {- x}}{2} \quad \text { and } \quad \cosh x = \frac {e ^ {x} + e ^ {- x}}{2}.
$$

Compare this result with the solution of the Dirichlet problem in the strip obtained in Problem 3, Chapter 5. 

# 2 <sub>Basic</sub> <sub>Properties</sub> <sub>of</sub> <sub>Fourier</sub> Series

Nearly fifty years had passed without any progress on the question of analytic representation of an arbitrary function, when an assertion of Fourier threw new light on the subject. Thus a new era began for the development of this part of Mathematics and this was heralded in a stunning way by major developments in mathematical Physics. 

B. Riemann, 1854 

In this chapter, we begin our rigorous study of Fourier series. We set the stage by introducing the main objects in the subject, and then formulate some basic problems which we have already touched upon earlier. 

Our first result disposes of the question of uniqueness: Are two functions with the same Fourier coeficients necessarily equal? Indeed, a simple argument shows that if both functions are continuous, then in fact they must agree. 

Next, we take a closer look at the partial sums of a Fourier series. Using the formula for the Fourier coeficients (which involves an integration), we make the key observation that these sums can be written conveniently as integrals: 

$$
\frac {1}{2 \pi} \int D _ {N} (x - y) f (y) d y,
$$

where $\{ D _ { N } \}$ is a family of functions called the Dirichlet kernels. The above expression is the convolution of f with the function $D _ { N }$ . Convolutions will play a critical role in our analysis. In general, given a family of functions $\{ K _ { n } \}$ , we are led to investigate the limiting properties as n tends to infinity of the convolutions 

$$
\frac {1}{2 \pi} \int K _ {n} (x - y) f (y) d y.
$$

We find that if the family $\{ K _ { n } \}$ satisfies the three important properties of “good kernels,” then the convolutions above tend to $f ( x )$ as $n \to \infty$ (at least when f is continuous). In this sense, the family $\{ K _ { n } \}$ is an “approximation to the identity.” Unfortunately, the Dirichlet kernels $D _ { N }$ do not belong to the category of good kernels, which indicates that the question of convergence of Fourier series is subtle. 

Instead of pursuing at this stage the problem of convergence, we consider various other methods of summing the Fourier series of a function. The first method, which involves averages of partial sums, leads to convolutions with good kernels, and yields an important theorem of Fej´er. From this, we deduce the fact that a continuous function on the circle can be approximated uniformly by trigonometric polynomials. Second, we may also sum the Fourier series in the sense of Abel and again encounter a family of good kernels. In this case, the results about convolutions and good kernels lead to a solution of the Dirichlet problem for the steady-state heat equation in the disc, considered at the end of the previous chapter. 

## 1 Examples and formulation of the problem

We commence with a brief description of the types of functions with which we shall be concerned. Since the Fourier coeficients of $f$ are defined by 

$$
a _ {n} = \frac {1}{L} \int_ {0} ^ {L} f (x) e ^ {- 2 \pi i n x / L} d x, \quad \text { for } n \in \mathbb {Z},
$$

where f is complex-valued on $[ 0 , L ] .$ , it will be necessary to place some integrability conditions on $f .$ We shall therefore assume for the remainder of this book that all functions are at least Riemann integrable.<sup>1</sup> Sometimes it will be illuminating to focus our attention on functions that are more “regular,” that is, functions that possess certain continuity or diferentiability properties. Below, we list several classes of functions in increasing order of generality. We emphasize that we will not generally restrict our attention to real-valued functions, contrary to what the following pictures may suggest; we will almost always allow functions that take values in the complex numbers $\mathbb { C } .$ . Furthermore, we sometimes think of our functions as being defined on the circle rather than an interval. We elaborate upon this below. 

## 1. Examples and formulation of the problem

## Everywhere continuous functions

These are the complex-valued functions f which are continuous at every point of the segment $[ 0 , L ]$ . A typical continuous function is sketched in Figure 1 (a). We shall note later that continuous functions on the circle satisfy the additional condition $f ( 0 ) = f ( L )$ 

## Piecewise continuous functions

These are bounded functions on [0, L] which have only finitely many discontinuities. An example of such a function with simple discontinuities is pictured in Figure 1 (b). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/ec7d88d116ef0523ba30803536f3d214676d72c78635cd198e9b86eb4246b3c5.jpg)



(a)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/75e2f9732a12d6bd5d5f9e474ed8976a6e9a573ba989e38db538ddfd3736be37.jpg)



(b)



Figure 1. Functions on [0, L]: continuous and piecewise continuous


This class of functions is wide enough to illustrate many of the theorems in the next few chapters. However, for logical completeness we consider also the more general class of Riemann integrable functions. This more extended setting is natural since the formula for the Fourier coeficients involves integration. 

## Riemann integrable functions

This is the most general class of functions we will be concerned with. Such functions are bounded, but may have infinitely many discontinuities. We recall the definition of integrability. A real-valued function f defined on [0, L] is Riemann integrable (which we abbreviate as integrable<sup>2</sup>) if it is bounded, and if for every $\epsilon > 0 .$ , there is a subdivision $0 = x _ { 0 } < x _ { 1 } < \dots < x _ { N - 1 } < x _ { N } = L$ of the interval [0, L], so that if U and $\mathcal { L }$ are, respectively, the upper and lower sums of f for this subdivision, namely 

$$
\mathcal {U} = \sum_ {j = 1} ^ {N} [ \sup _ {x _ {j - 1} \leq x \leq x _ {j}} f (x) ] (x _ {j} - x _ {j - 1})
$$

and 

$$
\mathcal {L} = \sum_ {j = 1} ^ {N} [ \inf _ {x _ {j - 1} \leq x \leq x _ {j}} f (x) ] (x _ {j} - x _ {j - 1}),
$$

then we have $\mathcal { U } - \mathcal { L } < \epsilon .$ . Finally, we say that a complex-valued function is integrable if its real and imaginary parts are integrable. It is worthwhile to remember at this point that the sum and product of two integrable functions are integrable. 

A simple example of an integrable function on [0, 1] with infinitely many discontinuities is given by 

$$
f (x) = \left\{ \begin{array}{l l} 1 & \text { if } 1 / (n + 1) <   x \leq 1 / n \text { and } n \text { is   odd }, \\ 0 & \text { if } 1 / (n + 1) <   x \leq 1 / n \text { and } n \text { is   even }, \\ 0 & \text { if } x = 0. \end{array} \right.
$$

This example is illustrated in Figure 2. Note that f is discontinuous when $x = 1 / n$ and at $x = 0$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/1f2aec4e6d321e996b3d397b5a43fd9669ddf8b32570970269f3f6558fb391f2.jpg)



Figure 2. A Riemann integrable function


More elaborate examples of integrable functions whose discontinuities are dense in the interval [0, 1] are described in Problem 1. In general, while integrable functions may have infinitely many discontinuities, these functions are actually characterized by the fact that, in a precise sense, their discontinuities are not too numerous: they are “negligible,” that is, the set of points where an integrable function is discontinuous has “measure 0.” The reader will find further details about Riemann integration in the appendix. 

From now on, we shall always assume that our functions are integrable, even if we do not state this requirement explicitly. 

## Functions on the circle

There is a natural connection between 2π-periodic functions on R like the exponentials $e ^ { i n \theta }$ , functions on an interval of length $2 \pi$ , and functions on the unit circle. This connection arises as follows. 

A point on the unit circle takes the form $e ^ { i \theta }$ , where θ is a real number that is unique up to integer multiples of $2 \pi$ . If $F$ is a function on the circle, then we may define for each real number θ 

$$
f (\theta) = F (e ^ {i \theta}),
$$

and observe that with this definition, the function f is periodic on R of period 2π, that is, $f ( \theta + 2 \pi ) = f ( \theta )$ for all θ. The integrability, continuity and other smoothness properties of F are determined by those of $f .$ For instance, we say that F is integrable on the circle if f is integrable on every interval of length 2π. Also, F is continuous on the circle if f is continuous on R, which is the same as saying that $f$ is continuous on any interval of length 2π. Moreover, F is continuously diferentiable if f has a continuous derivative, and so forth. 

Since f has period $2 \pi$ , we may restrict it to any interval of length 2π, say [0, 2π] or $[ - \pi , \pi ]$ , and still capture the initial function F on the circle. We note that f must take the same value at the end-points of the interval since they correspond to the same point on the circle. Conversely, any function on [0, 2π] for which $f ( 0 ) = f ( 2 \pi )$ can be extended to a periodic function on R which can then be identified as a function on the circle. In particular, a continuous function $f$ on the interval [0, 2π] gives rise to a continuous function on the circle if and only if $f ( 0 ) = f ( 2 \pi )$ 

In conclusion, functions on R that 2π-periodic, and functions on an interval of length 2π that take on the same value at its end-points, are two equivalent descriptions of the same mathematical objects, namely, functions on the circle. 

In this connection, we mention an item of notational usage. When our functions are defined on an interval on the line, we often use x as the independent variable; however, when we consider these as functions on the circle, we usually replace the variable x by θ. As the reader will note, we are not strictly bound by this rule since this practice is mostly a matter of convenience. 

## 1.1 Main definitions and some examples

We now begin our study of Fourier analysis with the precise definition of the Fourier series of a function. Here, it is important to pin down where our function is originally defined. If f is an integrable function given on an interval $[ a , b ]$ [a, b] of length $L$ (that is, $b - a = L )$ , then the $n ^ { \mathrm { t h } }$ Fourier coeficient of $f$ is defined by 

$$
\hat {f} (n) = \frac {1}{L} \int_ {a} ^ {b} f (x) e ^ {- 2 \pi i n x / L} d x, \quad n \in \mathbb {Z}.
$$

The Fourier series of $f$ is given formally<sup>3</sup> by 

$$
\sum_ {n = - \infty} ^ {\infty} \hat {f} (n) e ^ {2 \pi i n x / L}.
$$

We shall sometimes write $a _ { n }$ for the Fourier coeficients of $f ,$ , and use the notation 

$$
f (x) \sim \sum_ {n = - \infty} ^ {\infty} a _ {n} e ^ {2 \pi i n x / L}
$$

to indicate that the series on the right-hand side is the Fourier series of $f .$ 

For instance, if f is an integrable function on the interval $[ - \pi , \pi ]$ , then the $n ^ { \mathrm { t h } }$ Fourier coeficient of $f$ is 

$$
\hat {f} (n) = a _ {n} = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (\theta) e ^ {- i n \theta} d \theta , \quad n \in \mathbb {Z},
$$

and the Fourier series of $f$ is 

$$
f (\theta) \sim \sum_ {n = - \infty} ^ {\infty} a _ {n} e ^ {i n \theta}.
$$

Here we use $\theta$ as a variable since we think of it as an angle ranging from −π to π. 

Also, if f is defined on [0, 2π], then the formulas are the same as above, except that we integrate from 0 to 2π in the definition of the Fourier coeficients. 

We may also consider the Fourier coeficients and Fourier series for a function defined on the circle. By our previous discussion, we may think of a function on the circle as a function f on R which is 2π-periodic. We may restrict the function $f$ to any interval of length $2 \pi$ , for instance [0, 2π] or $[ - \pi , \pi ]$ , and compute its Fourier coeficients. Fortunately, $f$ is periodic and Exercise 1 shows that the resulting integrals are independent of the chosen interval. Thus the Fourier coeficients of a function on the circle are well defined. 

Finally, we shall sometimes consider a function g given on [0, 1]. Then 

$$
\hat {g} (n) = a _ {n} = \int_ {0} ^ {1} g (x) e ^ {- 2 \pi i n x} d x \quad \mathrm{and} \quad g (x) \sim \sum_ {n = - \infty} ^ {\infty} a _ {n} e ^ {2 \pi i n x}.
$$

Here we use x for a variable ranging from 0 to 1. 

Of course, if $f$ is initially given on [0, 2π], then $g ( x ) = f ( 2 \pi x )$ is defined on [0, 1] and a change of variables shows that the $n ^ { \mathrm { t h } }$ Fourier coeficient of $f$ equals the $n ^ { \mathrm { t h } }$ Fourier coeficient of $g .$ 

Fourier series are part of a larger family called the trigonometric series which, by definition, are expressions of the form $\scriptstyle \sum _ { n = - \infty } ^ { \infty } c _ { n } e ^ { 2 \pi i n x / L }$ where $c _ { n } \in \mathbb { C }$ . If a trigonometric series involves only finitely many nonzero terms, that is, $c _ { n } = 0$ for all large $| n | .$ , it is called a trigonometric polynomial; its degree is the largest value of $| n |$ for which $c _ { n } \neq 0$ 

The $N ^ { \mathrm { t h } }$ partial sum of the Fourier series of $f ,$ , for N a positive integer, is a particular example of a trigonometric polynomial. It is given by 

$$
S _ {N} (f) (x) = \sum_ {n = - N} ^ {N} \hat {f} (n) e ^ {2 \pi i n x / L}.
$$

Note that by definition, the above sum is symmetric since n ranges from $- N$ to $N ,$ a choice that is natural because of the resulting decomposition of the Fourier series as sine and cosine series. As a consequence, the convergence of Fourier series will be understood (in this book) as the “limit” as N tends to infinity of these symmetric sums. 

In fact, using the partial sums of the Fourier series, we can reformulate the basic question raised in Chapter 1 as follows: 

Problem: In what sense does $S _ { N } ( f )$ converge to f as $N  \infty ?$ 

Before proceeding further with this question, we turn to some simple examples of Fourier series. 

Example 1. Let $f ( \theta ) = \theta$ for $- \pi \leq \theta \leq \pi$ . The calculation of the Fourier coeficients requires a simple integration by parts. First, if $n \neq 0 .$ , then 

$$
\begin{array}{r l} & {\hat {f} (n) = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} \theta e ^ {- i n \theta} d \theta} \\ & {\qquad = \frac {1}{2 \pi} \left[ - \frac {\theta}{i n} e ^ {- i n \theta} \right] _ {- \pi} ^ {\pi} + \frac {1}{2 \pi i n} \int_ {- \pi} ^ {\pi} e ^ {- i n \theta} d \theta} \\ & {\qquad = \frac {(- 1) ^ {n + 1}}{i n},} \end{array}
$$

and if $n = 0$ we clearly have 

$$
\hat {f} (0) = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} \theta d \theta = 0.
$$

Hence, the Fourier series of f is given by 

$$
f (\theta) \sim \sum_ {n \neq 0} \frac {(- 1) ^ {n + 1}}{i n} e ^ {i n \theta} = 2 \sum_ {n = 1} ^ {\infty} (- 1) ^ {n + 1} \frac {\sin n \theta}{n}.
$$

The first sum is over all non-zero integers, and the second is obtained by an application of Euler’s identities. It is possible to prove by elementary means that the above series converges for every $\theta ,$ , but it is not obvious that it converges to $f ( \theta )$ . This will be proved later (Exercises 8 and 9 deal with a similar situation). 

Example 2. Define $f ( \theta ) = ( \pi - \theta ) ^ { 2 } / 4$ for $0 \leq \theta \leq 2 \pi$ . Then successive integration by parts similar to that performed in the previous example yield 

$$
f (\theta) \sim \frac {\pi^ {2}}{1 2} + \sum_ {n = 1} ^ {\infty} \frac {\cos n \theta}{n ^ {2}}.
$$

Example 3. The Fourier series of the function 

$$
f (\theta) = \frac {\pi}{\sin \pi \alpha} e ^ {i (\pi - \theta) \alpha}
$$

on [0, 2π] is 

$$
f (\theta) \sim \sum_ {n = - \infty} ^ {\infty} \frac {e ^ {i n \theta}}{n + \alpha},
$$

1. Examples and formulation of the problem 

whenever α is not an integer. 

Example 4. The trigonometric polynomial defined for $x \in [ - \pi , \pi ]$ by 

$$
D _ {N} (x) = \sum_ {n = - N} ^ {N} e ^ {i n x}
$$

is called the $N ^ { \mathrm { t h } }$ Dirichlet kernel and is of fundamental importance in the theory (as we shall see later). Notice that its Fourier coeficients $a _ { n }$ have the property that $a _ { n } = 1 { \mathrm { ~ i f ~ } } | n | \leq N$ and $a _ { n } = 0$ otherwise. A closed form formula for the Dirichlet kernel is 

$$
D _ {N} (x) = \frac {\sin ((N + \frac {1}{2}) x)}{\sin (x / 2)}.
$$

This can be seen by summing the geometric progressions 

$$
\sum_ {n = 0} ^ {N} \omega^ {n} \quad \mathrm{and} \quad \sum_ {n = - N} ^ {- 1} \omega^ {n}
$$

with $\omega = e ^ { i x }$ . These sums are, respectively, equal to 

$$
\frac {1 - \omega^ {N + 1}}{1 - \omega} \quad \mathrm{and} \quad \frac {\omega^ {- N} - 1}{1 - \omega}.
$$

Their sum is then 

$$
\frac {\omega^ {- N} - \omega^ {N + 1}}{1 - \omega} = \frac {\omega^ {- N - 1 / 2} - \omega^ {N + 1 / 2}}{\omega^ {- 1 / 2} - \omega^ {1 / 2}} = \frac {\sin ((N + \frac {1}{2}) x)}{\sin (x / 2)},
$$

giving the desired result. 

Example 5. The function $P _ { r } ( \theta )$ , called the Poisson kernel, is defined for $\theta \in [ - \pi , \pi ]$ and $0 \leq r < 1$ by the absolutely and uniformly convergent series 

$$
P _ {r} (\theta) = \sum_ {n = - \infty} ^ {\infty} r ^ {| n |} e ^ {i n \theta}.
$$

This function arose implicitly in the solution of the steady-state heat equation on the unit disc discussed in Chapter 1. Note that in calculating the Fourier coeficients of $P _ { r } ( \theta )$ we can interchange the order of integration and summation since the sum converges uniformly in θ for each fixed $r ,$ and obtain that the $n ^ { \mathrm { t h } }$ Fourier coeficient equals $r ^ { | n | }$ . One can also sum the series for $P _ { r } ( \theta )$ and see that 

$$
P _ {r} (\theta) = \frac {1 - r ^ {2}}{1 - 2 r \cos \theta + r ^ {2}}.
$$

In fact, 

$$
P _ {r} (\theta) = \sum_ {n = 0} ^ {\infty} \omega^ {n} + \sum_ {n = 1} ^ {\infty} \overline {{\omega}} ^ {n} \quad \text { with } \omega = r e ^ {i \theta},
$$

where both series converge absolutely. The first sum (an infinite geometric progression) equals $1 / ( 1 - \omega )$ , and likewise, the second is $\overline { { \omega } } / ( 1 - \overline { { \omega } } )$ Together, they combine to give 

$$
\frac {1 - \overline {{\omega}} + (1 - \omega) \overline {{\omega}}}{(1 - \omega) (1 - \overline {{\omega}})} = \frac {1 - | \omega | ^ {2}}{| 1 - \omega | ^ {2}} = \frac {1 - r ^ {2}}{1 - 2 r \cos \theta + r ^ {2}},
$$

as claimed. The Poisson kernel will reappear later in the context of Abel summability of the Fourier series of a function. 

Let us return to the problem formulated earlier. The definition of the Fourier series of $f$ is purely formal, and it is not obvious whether it converges to $f .$ . In fact, the solution of this problem can be very hard, or relatively easy, depending on the sense in which we expect the series to converge, or on what additional restrictions we place on $f .$ 

Let us be more precise. Suppose, for the sake of this discussion, that the function $f$ (which is always assumed to be Riemann integrable) is defined on $[ - \pi , \pi ]$ . The first question one might ask is whether the partial sums of the Fourier series of $f$ converge to $f$ pointwise. That is, do we have 

$$
\lim _ {N \to \infty} S _ {N} (f) (\theta) = f (\theta) \quad \mathrm{forevery} \theta ?\tag{1}
$$

We see quite easily that in general we cannot expect this result to be true at every $\theta ,$ since we can always change an integrable function at one point without changing its Fourier coeficients. As a result, we might ask the same question assuming that $f$ is continuous and periodic. For a long time it was believed that under these additional assumptions the answer would be “yes.” It was a surprise when Du Bois-Reymond showed that there exists a continuous function whose Fourier series diverges at a point. We will give such an example in the next chapter. Despite this negative result, we might ask what happens if we add more smoothness conditions on $f \colon$ for example, we might assume that $f$ is continuously 

## 2. Uniqueness of Fourier series

diferentiable, or twice continuously diferentiable. We will see that then the Fourier series of $f$ converges to $f$ uniformly. 

We will also interpret the limit (1) by showing that the Fourier series sums, in the sense of Ces`aro or Abel, to the function $f$ at all of its points of continuity. This approach involves appropriate averages of the partial sums of the Fourier series of $f .$ 

Finally, we can also define the limit (1) in the mean square sense. In the next chapter, we will show that if $f$ is merely integrable, then 

$$
\frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} | S _ {N} (f) (\theta) - f (\theta) | ^ {2} d \theta \rightarrow 0 \quad \text { as } N \rightarrow \infty .
$$

It is of interest to know that the problem of pointwise convergence of Fourier series was settled in 1966 by L. Carleson, who showed, among other things, that if $f$ is integrable in our sense,<sup>4</sup> then the Fourier series of $f$ converges to $f$ except possibly on a set of “measure 0.” $0 . { } ^ { \mathfrak { N } }$ The proof of this theorem is dificult and beyond the scope of this book. 

## 2 Uniqueness of Fourier series

If we were to assume that the Fourier series of functions f converge to f in an appropriate sense, then we could infer that a function is uniquely determined by its Fourier coeficients. This would lead to the following statement: if $f$ and $g$ have the same Fourier coeficients, then $f$ and $g$ are necessarily equal. By taking the diference $f - g .$ , this proposition can be reformulated as: if ${ \hat { f } } ( n ) = 0$ for all $n \in \mathbb { Z } .$ , then $f = 0$ . As stated, this assertion cannot be correct without reservation, since calculating Fourier coeficients requires integration, and we see that, for example, any two functions which difer at finitely many points have the same Fourier series. However, we do have the following positive result. 

Theorem 2.1 Suppose that f is an integrable function on the circle with ${ \hat { f } } ( n ) = 0$ for all $n \in \mathbb { Z }$ . Then $f ( \theta _ { 0 } ) = 0$ whenever f is continuous at the point $\theta _ { 0 }$ . 

Thus, in terms of what we know about the set of discontinuities of integrable functions $, ^ { 5 }$ we can conclude that $f$ vanishes for “most” values of θ. 

Proof. We suppose first that f is real-valued, and argue by contradiction. Assume, without loss of generality, that $f$ is defined on $[ - \pi , \pi ]$ , that $\theta _ { 0 } = 0$ , and $f ( 0 ) > 0$ . The idea now is to construct a family of trigonometric polynomials $\{ p _ { k } \}$ that “peak” at 0, and so that $\begin{array} { r } { \int p _ { k } ( \theta ) f ( \theta ) d \theta \to \infty \ \mathrm { a s } \ k \to \infty . } \end{array}$ . This will be our desired contradiction since these integrals are equal to zero by assumption. 

Since $f$ is continuous at 0, we can choose $0 < \delta \le \pi / 2$ , so that $f ( \theta ) >$ $f ( 0 ) / 2$ whenever $| \theta | < \delta$ . Let 

$$
p (\theta) = \epsilon + \cos \theta ,
$$

where $\epsilon > 0$ is chosen so small that $| p ( \theta ) | < 1 - \epsilon / 2$ , whenever $\delta \leq | \theta | \leq$ π. Then, choose a positive $\eta$ with $\eta < \delta$ , so that $p ( \theta ) \geq 1 + \epsilon / 2$ , for $| \theta | < \eta$ . Finally, let 

$$
p _ {k} (\theta) = [ p (\theta) ] ^ {k},
$$

and select $B \ \mathrm { s o }$ that $| f ( \theta ) | \le B$ for all $\theta .$ This is possible since $f$ is integrable, hence bounded. Figure 3 illustrates the family $\{ p _ { k } \}$ . By 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/0d6b515b4362e46c58f6522b7f33e044fc277d45f2479b5f3f68605ecca46e8d.jpg)



Figure 3. The functions $p , p _ { 6 }$ , and $p _ { 1 5 }$ when $\epsilon = 0 . 1$


construction, each $p _ { k }$ is a trigonometric polynomial, and since ${ \hat { f } } ( n ) = 0$ for all n, we must have 

$$
\int_ {- \pi} ^ {\pi} f (\theta) p _ {k} (\theta) d \theta = 0 \quad \mathrm{forall} k.
$$

However, we have the estimate 

$$
\left| \int_ {\delta \leq | \theta |} f (\theta) p _ {k} (\theta) d \theta \right| \leq 2 \pi B (1 - \epsilon / 2) ^ {k}.
$$

## 2. Uniqueness of Fourier series

Also, our choice of δ guarantees that $p ( \theta )$ and $f ( \theta )$ are non-negative whenever $| \theta | < \delta$ , thus 

$$
\int_ {\eta \leq | \theta | <   \delta} f (\theta) p _ {k} (\theta) d \theta \geq 0.
$$

Finally, 

$$
\int_ {| \theta | <   \eta} f (\theta) p _ {k} (\theta) d \theta \geq 2 \eta \frac {f (0)}{2} (1 + \epsilon / 2) ^ {k}.
$$

Therefore, $\begin{array} { r } { \int p _ { k } ( \theta ) f ( \theta ) d \theta \longrightarrow \infty \ \mathrm { a s } \ k \longrightarrow \infty } \end{array}$ , and this concludes the proof when f is real-valued. In general, write $f ( \theta ) = u ( \theta ) + i v ( \theta )$ , where u and v are real-valued. If we define ${ \overline { { f } } } ( \theta ) = { \overline { { f ( \theta ) } } }$ , then 

$$
u (\theta) = \frac {f (\theta) + \overline {{f}} (\theta)}{2} \quad \text { and } \quad v (\theta) = \frac {f (\theta) - \overline {{f}} (\theta)}{2 i},
$$

and since ${ \hat { \overline { { f } } } } ( n ) = { \overline { { { \hat { f } } ( - n ) } } }$ , we conclude that the Fourier coeficients of u and v all vanish, hence $f = 0$ at its points of continuity. The idea 

of constructing a family of functions (trigonometric polynomials in this case) which peak at the origin, together with other nice properties, will play an important role in this book. Such families of functions will be taken up later in Section 4 in connection with the notion of convolution. For now, note that the above theorem implies the following. 

Corollary 2.2 If f is continuous on the circle and ${ \hat { f } } ( n ) = 0$ for all $n \in \mathbb { Z } .$ , then $f = 0$ 

The next corollary shows that the problem (1) formulated earlier has a simple positive answer under the assumption that the series of Fourier coeficients converges absolutely. 

Corollary 2.3 Suppose that f is a continuous function on the circle and that the Fourier series of f is absolutely convergent, $\scriptstyle \sum _ { n = - \infty } ^ { \infty } | { \hat { f } } ( n ) | < \infty$ Then, the Fourier series converges uniformly to f, that is, 

$$
\lim _ {N \to \infty} S _ {N} (f) (\theta) = f (\theta) \quad u n i f o r m l y i n \theta .
$$

Proof. Recall that if a sequence of continuous functions converges uniformly, then the limit is also continuous. Now observe that the assumption $\textstyle \sum | { \hat { f } } ( n ) | < \infty$ implies that the partial sums of the Fourier series of $f$ converge absolutely and uniformly, and therefore the function $g$ defined by 

$$
g (\theta) = \sum_ {n = - \infty} ^ {\infty} \hat {f} (n) e ^ {i n \theta} = \lim _ {N \to \infty} \sum_ {n = - N} ^ {N} \hat {f} (n) e ^ {i n \theta}
$$

is continuous on the circle. Moreover, the Fourier coeficients of $g$ are precisely ${ \hat { f } } ( n )$ since we can interchange the infinite sum with the integral (a consequence of the uniform convergence of the series). Therefore, the previous corollary applied to the function $f - g$ yields $f = g$ , as desired. 

What conditions on $f$ would guarantee the absolute convergence of its 

Fourier series? $\mathrm { A s }$ it turns out, the smoothness of $f$ is directly related to the decay of the Fourier coeficients, and in general, the smoother the function, the faster this decay. As a result, we can expect that relatively smooth functions equal their Fourier series. This is in fact the case, as we now show. 

In order to state the result concisely we introduce the standard $^ { 6 6 } O ^ { 9 9 }$ notation, which we will use freely in the rest of this book. For example, the statement $\hat { f } ( n ) = O ( 1 / | n | ^ { 2 } )$ as $| n | \to \infty$ , means that the lefthand side is bounded by a constant multiple of the right-hand side; that is, there exists $C > 0$ with $| { \hat { f } } ( n ) | \leq C / | n | ^ { 2 }$ for all large $| n |$ . More generally, $f ( x ) = O ( g ( x ) )$ as $x \longrightarrow a$ means that for some constant $C ,$ $| f ( x ) | \leq C | g ( x ) |$ as x approaches $a .$ In particular, $f ( x ) = O ( 1 )$ means that $f$ is bounded. 

Corollary 2.4 Suppose that $f$ is a twice continuously diferentiable function on the circle. Then 

$$
\hat {f} (n) = O (1 / | n | ^ {2}) \quad a s | n | \to \infty ,
$$

so that the Fourier series of f converges absolutely and uniformly to $f .$ 

## 2. Uniqueness of Fourier series

Proof. The estimate on the Fourier coeficients is proved by integrating by parts twice for $n \neq 0$ . We obtain 

$$
\begin{array}{l} 2 \pi \hat {f} (n) = \int_ {0} ^ {2 \pi} f (\theta) e ^ {- i n \theta} d \theta \\ \qquad = \left[ f (\theta) \cdot \frac {- e ^ {- i n \theta}}{i n} \right] _ {0} ^ {2 \pi} + \frac {1}{i n} \int_ {0} ^ {2 \pi} f ^ {\prime} (\theta) e ^ {- i n \theta} d \theta \\ \qquad = \frac {1}{i n} \int_ {0} ^ {2 \pi} f ^ {\prime} (\theta) e ^ {- i n \theta} d \theta \\ \qquad = \frac {1}{i n} \left[ f ^ {\prime} (\theta) \cdot \frac {- e ^ {- i n \theta}}{i n} \right] _ {0} ^ {2 \pi} + \frac {1}{(i n) ^ {2}} \int_ {0} ^ {2 \pi} f ^ {\prime \prime} (\theta) e ^ {- i n \theta} d \theta \\ \qquad = \frac {- 1}{n ^ {2}} \int_ {0} ^ {2 \pi} f ^ {\prime \prime} (\theta) e ^ {- i n \theta} d \theta . \end{array}
$$

The quantities in brackets vanish since $f$ and $f ^ { \prime }$ are periodic. Therefore 

$$
2 \pi | n | ^ {2} | \hat {f} (n) | \leq \left| \int_ {0} ^ {2 \pi} f ^ {\prime \prime} (\theta) e ^ {- i n \theta} d \theta \right| \leq \int_ {0} ^ {2 \pi} | f ^ {\prime \prime} (\theta) | d \theta \leq C,
$$

where the constant C is independent of $n .$ (We can take $C = 2 \pi B$ where $B$ is a bound for $f ^ { \prime \prime } . )$ Since $\textstyle \sum 1 / { n ^ { 2 } }$ converges, the proof of the corollary is complete. 

Incidentally, we have also established the following important identity: 

$$
\widehat {f} ^ {\prime} (n) = i n \widehat {f} (n), \quad \text {   for   all   } n \in \mathbb {Z}.
$$

If $\iota \neq 0$ the proof is given above, and if $n = 0$ it is left as an exercise to the reader. So if $f$ is diferentiable and $f \sim \sum a _ { n } e ^ { i n \theta }$ , then $\begin{array} { r } { f ^ { \prime } \sim \sum a _ { n } i n e ^ { i n \theta } } \end{array}$ Also, if $f$ is twice continuously diferentiable, then $f ^ { \prime \prime } \sim \sum \overline { { a _ { n } } } ( i n ) ^ { 2 } e ^ { i n \theta }$ and so on. Further smoothness conditions on $f$ imply even better decay of the Fourier coeficients (Exercise 10). 

There are also stronger versions of Corollary 2.4. It can be shown, for example, that the Fourier series of $f$ converges absolutely, assuming only that $f$ has one continuous derivative. Even more generally, the Fourier series of $f$ converges absolutely (and hence uniformly to $f )$ if $f$ satisfies a H¨older condition of order $\alpha ,$ with $\alpha > 1 / 2$ , that is, 

$$
\sup _ {\theta} | f (\theta + t) - f (\theta) | \leq A | t | ^ {\alpha} \quad \text { for   all } t.
$$

For more on these matters, see the exercises at the end of Chapter 3. 

At this point it is worthwhile to introduce a common notation: we say that $f$ belongs to the class $C ^ { k }$ if $f$ is k times continuously diferentiable. Belonging to the class $C ^ { k }$ or satisfying a H¨older condition are two possible ways to describe the smoothness of a function. 

## 3 Convolutions

The notion of convolution of two functions plays a fundamental role in Fourier analysis; it appears naturally in the context of Fourier series but also serves more generally in the analysis of functions in other settings. 

Given two 2π-periodic integrable functions $f$ and $g$ on $\mathbb { R }$ , we define their convolution $f * g$ on $[ - \pi , \pi ]$ by 

$$
(f * g) (x) = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (y) g (x - y) d y.\tag{2}
$$

The above integral makes sense for each $x ,$ since the product of two integrable functions is again integrable. Also, since the functions are periodic, we can change variables to see that 

$$
(f * g) (x) = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (x - y) g (y) d y.
$$

Loosely speaking, convolutions correspond to “weighted averages.” For instance, ${ \mathrm { i f } } g = 1 { \mathrm { i n } } ( 2 )$ , then $f * g$ is constant and equal to $\begin{array} { r } { { \frac { 1 } { 2 \pi } } \int _ { - \pi } ^ { \pi } f ( y ) d y . } \end{array}$ which we may interpret as the average value of $f$ on the circle. Also, the convolution $( f * g ) ( x )$ ) plays a role similar to, and in some sense replaces, the pointwise product $f ( x ) g ( x )$ of the two functions $f$ and $g .$ 

In the context of this chapter, our interest in convolutions originates from the fact that the partial sums of the Fourier series of $f$ can be expressed as follows: 

$$
\begin{array}{l} S _ {N} (f) (x) = \sum_ {n = - N} ^ {N} \hat {f} (n) e ^ {i n x} \\ \qquad = \sum_ {n = - N} ^ {N} \left(\frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (y) e ^ {- i n y} d y\right) e ^ {i n x} \\ \qquad = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (y) \left(\sum_ {n = - N} ^ {N} e ^ {i n (x - y)}\right) d y \\ \qquad = (f * D _ {N}) (x), \end{array}
$$

## 3. Convolutions

where $D _ { N }$ is the $N ^ { \mathrm { t h } }$ Dirichlet kernel (see Example 4) given by 

$$
D _ {N} (x) = \sum_ {n = - N} ^ {N} e ^ {i n x}.
$$

So we observe that the problem of understanding $S _ { N } ( f )$ reduces to the understanding of the convolution $f * D _ { N }$ 

We begin by gathering some of the main properties of convolutions. 

Proposition 3.1 Suppose that $f , \ g ,$ , and h are 2π-periodic integrable functions. Then: 

(i) $f * ( g + h ) = ( f * g ) + ( f * h ) .$ 

(ii) $( c f ) * g = c ( f * g ) = f * ( c g ) \ f o r \ a n y \ c \in \mathbb { C } .$ 

(iii) $f * g = g * f .$ 

(iv) $( f * g ) * h = f * ( g * h ) .$ 

(v) $f * g$ is continuous. 

(vi) ${ \widehat { f * g } } ( n ) = { \hat { f } } ( n ) { \hat { g } } ( n )$ 

The first four points describe the algebraic properties of convolutions: linearity, commutativity, and associativity. Property (v) exhibits an important principle: the convolution of $f * g$ is “more regular” than $f$ or $g .$ Here, $f * g$ is continuous while $f$ and g are merely (Riemann) integrable. Finally, (vi) is key in the study of Fourier series. In general, the Fourier coeficients of the product $f g$ are not the product of the Fourier coeficients of f and $g .$ . However, (vi) says that this relation holds if we replace the product of the two functions $f$ and g by their convolution $f * g$ 

Proof. Properties (i) and (ii) follow at once from the linearity of the integral. 

The other properties are easily deduced if we assume also that $f$ and $g$ are continuous. In this case, we may freely interchange the order of integration. For instance, to establish (vi) we write 

$$
\begin{array}{r l} & {\widehat {f * g} (n) = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} (f * g) (x) e ^ {- i n x} d x} \\ & {\quad = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} \frac {1}{2 \pi} \left(\int_ {- \pi} ^ {\pi} f (y) g (x - y) d y\right) e ^ {- i n x} d x} \\ & {\quad = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (y) e ^ {- i n y} \left(\frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} g (x - y) e ^ {- i n (x - y)} d x\right) d y} \\ & {\quad = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (y) e ^ {- i n y} \left(\frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} g (x) e ^ {- i n x} d x\right) d y} \\ & {\quad = \hat {f} (n) \hat {g} (n).} \end{array}
$$

To prove (iii), one first notes that if $F$ is continuous and 2π-periodic, then 

$$
\int_ {- \pi} ^ {\pi} F (y) d y = \int_ {- \pi} ^ {\pi} F (x - y) d y \quad \text {for any} x \in \mathbb {R}.
$$

The verification of this identity consists of a change of variables $y \mapsto - y .$ followed by a translation $y \mapsto y - x$ . Then, one takes $F ( y ) = f ( y ) g ( x - y )$ 

Also, (iv) follows by interchanging two integral signs, and an appropriate change of variables. 

Finally, we show that if $f$ and $g$ are continuous, then $f * g$ is continuous. First, we may write 

$$
(f * g) (x _ {1}) - (f * g) (x _ {2}) = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (y) [ g (x _ {1} - y) - g (x _ {2} - y) ] d y.
$$

Since $g$ is continuous it must be uniformly continuous on any closed and bounded interval. But $g$ is also periodic, so it must be uniformly continuous on all of $\mathbb { R } ;$ given $\epsilon > 0$ there exists $\delta > 0$ so that $| g ( s ) -$ $g ( t ) | < \epsilon$ whenever $| s - t | < \delta$ . Then, $| x _ { 1 } - x _ { 2 } | < \delta$ implies $\left| ( x _ { 1 } - y ) - \right.$ $\left( x _ { 2 } - y \right) | < \delta$ for any $y .$ hence 

$$
\begin{array}{l} | (f * g) (x _ {1}) - (f * g) (x _ {2}) | \leq \frac {1}{2 \pi} \left| \int_ {- \pi} ^ {\pi} f (y) [ g (x _ {1} - y) - g (x _ {2} - y) ] d y \right| \\ \leq \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} | f (y) | | g (x _ {1} - y) - g (x _ {2} - y) | d y \\ \leq \frac {\epsilon}{2 \pi} \int_ {- \pi} ^ {\pi} | f (y) | d y \\ \leq \frac {\epsilon}{2 \pi} 2 \pi B, \end{array}
$$

## 3. Convolutions

where B is chosen so that $| f ( x ) | \leq B$ for all x. As a result, we conclude that $f * g$ is continuous, and the proposition is proved, at least when $f$ and $g$ are continuous. 

In general, when $f$ and g are merely integrable, we may use the results established so far (when f and g are continuous), together with the following approximation lemma, whose proof may be found in the appendix. 

Lemma 3.2 Suppose f is integrable on the circle and bounded by $B .$ Then there exists a sequence $\{ f _ { k } \} _ { k = 1 } ^ { \infty }$ of continuous functions on the circle so that 

$$
\sup _ {x \in [ - \pi , \pi ]} | f _ {k} (x) | \leq B \quad \text {   for   all   } k = 1, 2, \ldots ,
$$

and 

$$
\int_ {- \pi} ^ {\pi} | f (x) - f _ {k} (x) | d x \rightarrow 0 \quad a s k \rightarrow \infty .
$$

Using this result, we may complete the proof of the proposition as follows. Apply Lemma 3.2 to f and $g$ to obtain sequences $\{ f _ { k } \}$ and $\left\{ g _ { k } \right\}$ of approximating continuous functions. Then 

$$
f * g - f _ {k} * g _ {k} = (f - f _ {k}) * g + f _ {k} * (g - g _ {k}).
$$

By the properties of the sequence $\{ f _ { k } \}$ 

$$
\begin{array}{l}| (f - f _ {k}) * g (x) | \leq \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} | f (x - y) - f _ {k} (x - y) |   | g (y) |   d y\\\quad \leq \frac {1}{2 \pi} \sup _ {y} | g (y) | \int_ {- \pi} ^ {\pi} | f (y) - f _ {k} (y) |   d y\\\rightarrow 0 \quad \text { as } k \rightarrow \infty .\end{array}
$$

Hence $\left( f - f _ { k } \right) * g \longrightarrow 0$ uniformly in $x .$ . Similarly, $f _ { k } * \left( g - g _ { k } \right) \to 0$ uniformly, and therefore $f _ { k } * g _ { k }$ tends uniformly to $f * g .$ . Since each $f _ { k } * g _ { k }$ is continuous, it follows that $f * g$ is also continuous, and we have (v). 

Next, we establish (vi). For each fixed integer n we must have ${ \widehat { f _ { k } * g _ { k } } } ( n ) \to { \widehat { f * g } } ( n )$ as k tends to infinity since $f _ { k } * g _ { k }$ converges uniformly to $f * g .$ . However, we found earlier that ${ \widehat { f _ { k } } } ( n ) { \widehat { g _ { k } } } ( n ) = { \widehat { f _ { k } * g _ { k } } } ( n )$ because both $f _ { k }$ and $g _ { k }$ are continuous. Hence 

$$
\begin{array}{c} | \hat {f} (n) - \hat {f} _ {k} (n) | = \frac {1}{2 \pi} \left| \int_ {- \pi} ^ {\pi} (f (x) - f _ {k} (x)) e ^ {- i n x} d x \right| \\ \leq \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} | f (x) - f _ {k} (x) | d x, \end{array}
$$

and as a result we find that ${ \widehat { f _ { k } } } ( n ) \to { \hat { f } } ( n )$ as k goes to infinity. Similarly ${ \widehat { g _ { k } } } ( n ) \to { \hat { g } } ( n )$ , and the desired property is established once we let k tend to infinity. Finally, properties (iii) and (iv) follow from the same kind of arguments. 

## 4 Good kernels

In the proof of Theorem 2.1 we constructed a sequence of trigonometric polynomials $\{ p _ { k } \}$ with the property that the functions $p _ { k }$ peaked at the origin. As a result, we could isolate the behavior of $f$ at the origin. In this section, we return to such families of functions, but this time in a more general setting. First, we define the notion of good kernel, and discuss the characteristic properties of such functions. Then, by the use of convolutions, we show how these kernels can be used to recover a given function. 

A family of kernels $\{ K _ { n } ( x ) \} _ { n = 1 } ^ { \infty }$ on the circle is said to be a family of good kernels if it satisfies the following properties: 

(a) For all $n \geq 1$ 

$$
\frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} K _ {n} (x) d x = 1.
$$

(b) There exists $M > 0$ such that for all $n \geq 1$ ， 

$$
\int_ {- \pi} ^ {\pi} | K _ {n} (x) | d x \leq M.
$$

(c) For every $\delta > 0$ 

$$
\int_ {\delta \leq | x | \leq \pi} | K _ {n} (x) | d x \to 0, \quad \text { as } n \to \infty .
$$

In practice we shall encounter families where $K _ { n } ( x ) \geq 0$ , in which case (b) is a consequence of (a). We may interpret the kernels $K _ { n } ( x )$ as weight distributions on the circle: property (a) says that $K _ { n }$ assigns unit mass to the whole circle $[ - \pi , \pi ]$ , and (c) that this mass concentrates near the origin as n becomes large.<sup>6</sup> Figure 4 (a) illustrates the typical character of a family of good kernels. 

The importance of good kernels is highlighted by their use in connection with convolutions. 

## 4. Good kernels

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/32a3f4ccf74f988ed5257ba506b6be9db4ae7cc58f528a963762691875ef3851.jpg)



(a)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/458842a830fe93f786304e15e8e8eeda7486a7181a793d3b595699e845bc7972.jpg)



(b)



Figure 4. Good kernels


Theorem 4.1 Let $\{ K _ { n } \} _ { n = 1 } ^ { \infty }$ be a family of good kernels, and f an integrable function on the circle. Then 

$$
\lim _ {n \to \infty} (f * K _ {n}) (x) = f (x)
$$

whenever f is continuous at x. If f is continuous everywhere, then the above limit is uniform. 

Because of this result, the family $\{ K _ { n } \}$ is sometimes referred to as an approximation to the identity. 

We have previously interpreted convolutions as weighted averages. In this context, the convolution 

$$
(f * K _ {n}) (x) = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (x - y) K _ {n} (y) d y
$$

is the average of $f ( x - y )$ , where the weights are given by $K _ { n } ( y )$ . However, the weight distribution $K _ { n }$ concentrates its mass at $y = 0$ as n becomes large. Hence in the integral, the value $f ( x )$ is assigned the full mass as $n \to \infty$ . Figure 4 (b) illustrates this point. 

Proof of Theorem 4.1. If $\epsilon > 0$ and f is continuous at $x ,$ choose $\delta$ so that $| y | < \delta$ implies $| f ( x - y ) - f ( x ) | < \epsilon$ . Then, by the first property of good kernels, we can write 

$$
\begin{array}{c} (f * K _ {n}) (x) - f (x) = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} K _ {n} (y) f (x - y) d y - f (x) \\ = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} K _ {n} (y) [ f (x - y) - f (x) ] d y. \end{array}
$$

Hence, 

$$
\begin{array}{l} | (f * K _ {n}) (x) - f (x) | = \left| \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} K _ {n} (y) [ f (x - y) - f (x) ]   d y \right| \\ \leq \frac {1}{2 \pi} \int_ {| y | <   \delta} | K _ {n} (y) |   | f (x - y) - f (x) |   d y \\ \qquad + \frac {1}{2 \pi} \int_ {\delta \leq | y | \leq \pi} | K _ {n} (y) |   | f (x - y) - f (x) |   d y \\ \leq \frac {\epsilon}{2 \pi} \int_ {- \pi} ^ {\pi} | K _ {n} (y) |   d y + \frac {2 B}{2 \pi} \int_ {\delta \leq | y | \leq \pi} | K _ {n} (y) |   d y, \end{array}
$$

where $B$ is a bound for $f .$ The first term is bounded by $\epsilon M / 2 \pi$ because of the second property of good kernels. $\mathrm { B y }$ the third property we see that for all large $n ,$ the second term will be less than ². Therefore, for some constant $C > 0$ and all large n we have 

$$
| (f * K _ {n}) (x) - f (x) | \leq C \epsilon ,
$$

thereby proving the first assertion in the theorem. If $f$ is continuous everywhere, then it is uniformly continuous, and $\delta$ can be chosen independent of x. This provides the desired conclusion that $f * K _ { n } \to f$ uniformly. 

Recall from the beginning of Section 3 that 

$$
S _ {N} (f) (x) = (f * D _ {N}) (x),
$$

where $\begin{array} { r } { D _ { N } ( x ) = \sum _ { n = - N } ^ { N } e ^ { i n x } } \end{array}$ is the Dirichlet kernel. It is natural now for us to ask whether $D _ { N }$ is a good kernel, since if this were true, Theorem 4.1 would imply that the Fourier series of $f$ converges to $f ( x )$ whenever $f$ is continuous at x. Unfortunately, this is not the case. Indeed, an estimate shows that $D _ { N }$ violates the second property; more precisely, one has (see Problem 2) 

$$
\int_ {- \pi} ^ {\pi} | D _ {N} (x) | d x \geq c \log N, \quad \mathrm{as} N \to \infty .
$$

However, we should note that the formula for $D _ { N }$ as a sum of exponentials immediately gives 

$$
\frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} D _ {N} (x) d x = 1,
$$

so the first property of good kernels is actually verified. The fact that the mean value of $D _ { N }$ is 1, while the integral of its absolute value is large, is a result of cancellations. Indeed, Figure 5 shows that the function $D _ { N } ( x )$ takes on positive and negative values and oscillates very rapidly as N gets large. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/bc85677f558ff9799de1e58148fe497bded75cdddb95dee0da0c53975cbea5d1.jpg)



Figure 5. The Dirichlet kernel for large N


This observation suggests that the pointwise convergence of Fourier series is intricate, and may even fail at points of continuity. This is indeed the case, as we will see in the next chapter. 

## 5 Ces`aro and Abel summability: applications to Fourier series

Since a Fourier series may fail to converge at individual points, we are led to try to overcome this failure by interpreting the limit 

$$
\lim _ {N \to \infty} S _ {N} (f) = f
$$

in a diferent sense. 

## 5.1 Ces`aro means and summation

We begin by taking ordinary averages of the partial sums, a technique which we now describe in more detail. 

Suppose we are given a series of complex numbers 

$$
c _ {0} + c _ {1} + c _ {2} + \dots = \sum_ {k = 0} ^ {\infty} c _ {k}.
$$

We define the $n ^ { \mathrm { t h } }$ partial sum $s _ { n }$ by 

$$
s _ {n} = \sum_ {k = 0} ^ {n} c _ {k},
$$

and say that the series converges to s if lim ${ \it n \to \infty } s _ { n } = s$ . This is the most natural and most commonly used type of “summability.” Consider, however, the example of the series 

$$
1 - 1 + 1 - 1 + \dots = \sum_ {k = 0} ^ {\infty} (- 1) ^ {k}.\tag{3}
$$

Its partial sums form the sequence $\{ 1 , 0 , 1 , 0 , \ldots \}$ which has no limit. Because these partial sums alternate evenly between 1 and 0, one might therefore suggest that $1 / 2$ is the “limit” of the sequence, and hence $1 / 2$ equals the “sum” of that particular series. We give a precise meaning to this by defining the average of the first N partial sums by 

$$
\sigma_ {N} = \frac {s _ {0} + s _ {1} + \cdots + s _ {N - 1}}{N}.
$$

The quantity $\sigma _ { N }$ is called the $N ^ { \mathrm { t h } }$ Ces`aro mean<sup>7</sup> of the sequence $\{ s _ { k } \}$ or the $N ^ { \mathrm { t h } }$ Ces`aro sum of the series $\textstyle \sum _ { k = 0 } ^ { \infty } c _ { k }$ 

If $\sigma _ { N }$ converges to a limit $\sigma$ as N tends to infinity, we say that the series $\sum c _ { n }$ is Ces`aro summable to $\sigma$ . In the case of series of functions, we shall understand the limit in the sense of either pointwise or uniform convergence, depending on the situation. 

The reader will have no dificulty checking that in the above example (3), the series is Ces`aro summable to $1 / 2$ . Moreover, one can show that Ces`aro summation is a more inclusive process than convergence. In fact, if a series is convergent to $s ,$ then it is also Ces`aro summable to the same limit s (Exercise 12). 

## 5.2 Fej´er’s theorem

An interesting application of Ces`aro summability appears in the context of Fourier series. 

We mentioned earlier that the Dirichlet kernels fail to belong to the family of good kernels. Quite surprisingly, their averages are very well behaved functions, in the sense that they do form a family of good kernels. 

To see this, we form the $N ^ { \mathrm { t h } }$ Ces`aro mean of the Fourier series, which by definition is 

$$
\sigma_ {N} (f) (x) = \frac {S _ {0} (f) (x) + \cdots + S _ {N - 1} (f) (x)}{N}.
$$

Since $S _ { n } ( f ) = f * D _ { n }$ , we find that 

$$
\sigma_ {N} (f) (x) = \left(f * F _ {N}\right) (x),
$$

where $F _ { N } ( x )$ is the N-th Fej´er kernel given by 

$$
F _ {N} (x) = \frac {D _ {0} (x) + \cdots + D _ {N - 1} (x)}{N}.
$$

Lemma 5.1 We have 

$$
F _ {N} (x) = \frac {1}{N} \frac {\sin^ {2} (N x / 2)}{\sin^ {2} (x / 2)},
$$

and the Fej´er kernel is a good kernel. 

The proof of the formula for $F _ { N }$ (a simple application of trigonometric identities) is outlined in Exercise 15. To prove the rest of the lemma, note that $F _ { N }$ is positive and $\begin{array} { r } { \frac { 1 } { 2 \pi } \int _ { - \pi } ^ { \pi } F _ { N } ( x ) d x = 1 } \end{array}$ , in view of the fact that a similar identity holds for the Dirichlet kernels $D _ { n }$ . However, sin $\iota ^ { 2 } ( x / 2 ) \geq$ $c _ { \delta } > 0 , { \mathrm { i f ~ } } \delta \leq | x | \leq \pi$ , hence ${ \cal F } _ { N } ( x ) \le 1 / ( N c _ { \delta } )$ , from which it follows that 

$$
\int_ {\delta \leq | x | \leq \pi} | F _ {N} (x) | d x \to 0 \quad \text {as} N \to \infty .
$$

Applying Theorem 4.1 to this new family of good kernels yields the following important result. 

Theorem 5.2 If f is integrable on the circle, then the Fourier series of f is Ces`aro summable to f at every point of continuity of f. 

Moreover, if f is continuous on the circle, then the Fourier series of f is uniformly Ces`aro summable to $f$ 

We may now state two corollaries. The first is a result that we have already established. The second is new, and of fundamental importance. 

Corollary 5.3 If f is integrable on the circle and ${ \hat { f } } ( n ) = 0$ for all $n ,$ then $f = 0$ at all points of continuity of $f .$ . 

The proof is immediate since all the partial sums are 0, hence all the Ces`aro means are 0. 

Corollary 5.4 Continuous functions on the circle can be uniformly approximated $b y$ trigonometric polynomials. 

This means that if f is continuous on $[ - \pi , \pi ]$ with $f ( - \pi ) = f ( \pi )$ and $\epsilon > 0$ , then there exists a trigonometric polynomial P such that 

$$
| f (x) - P (x) | <   \epsilon \quad \text { for   all } - \pi \leq x \leq \pi .
$$

This follows immediately from the theorem since the partial sums, hence the Ces`aro means, are trigonometric polynomials. Corollary 5.4 is the periodic analogue of the Weierstrass approximation theorem for polynomials which can be found in Exercise 16. 

## 5.3 Abel means and summation

Another method of summation was first considered by Abel and actually predates the Ces`aro method. 

A series of complex numbers $\textstyle \sum _ { k = 0 } ^ { \infty } c _ { k }$ is said to be Abel summable to s if for every $0 \leq r < 1$ , the series 

$$
A (r) = \sum_ {k = 0} ^ {\infty} c _ {k} r ^ {k}
$$

converges, and 

$$
\lim _ {r \to 1} A (r) = s.
$$

The quantities $A ( r )$ are called the Abel means of the series. One can prove that if the series converges to s, then it is Abel summable to s. Moreover, the method of Abel summability is even more powerful than the Ces`aro method: when the series is Ces`aro summable, it is always Abel summable to the same sum. However, if we consider the series 

$$
1 - 2 + 3 - 4 + 5 - \dots = \sum_ {k = 0} ^ {\infty} (- 1) ^ {k} (k + 1),
$$

then one can show that it is Abel summable to $1 / 4$ since 

$$
A (r) = \sum_ {k = 0} ^ {\infty} (- 1) ^ {k} (k + 1) r ^ {k} = \frac {1}{(1 + r) ^ {2}},
$$

but this series is not Ces`aro summable; see Exercise 13. 

## 5.4 The Poisson kernel and Dirichlet’s problem in the unit disc

To adapt Abel summability to the context of Fourier series, we define the Abel means of the function $\begin{array} { r } { f ( \theta ) \sim \sum _ { n = - \infty } ^ { \infty } a _ { n } e ^ { i n \theta } } \end{array}$ by 

$$
A _ {r} (f) (\theta) = \sum_ {n = - \infty} ^ {\infty} r ^ {| n |} a _ {n} e ^ {i n \theta}.
$$

Since the index n takes positive and negative values, it is natural to write $c _ { 0 } = a _ { 0 }$ , and $c _ { n } = a _ { n } e ^ { i n \theta } + a _ { - n } e ^ { - i n \theta }$ for $n > 0$ , so that the Abel means of the Fourier series correspond to the definition given in the previous section for numerical series. 

We note that since $f$ is integrable, $\left| a _ { n } \right|$ is uniformly bounded in n, so that $A _ { r } ( f )$ converges absolutely and uniformly for each $0 \leq r < 1$ . Just as in the case of Ces`aro means, the key fact is that these Abel means can be written as convolutions 

$$
A _ {r} (f) (\theta) = (f * P _ {r}) (\theta),
$$

where $P _ { r } ( \theta )$ is the Poisson kernel given by 

$$
P _ {r} (\theta) = \sum_ {n = - \infty} ^ {\infty} r ^ {| n |} e ^ {i n \theta}.\tag{4}
$$

In fact, 

$$
\begin{array}{l} A _ {r} (f) (\theta) = \sum_ {n = - \infty} ^ {\infty} r ^ {| n |} a _ {n} e ^ {i n \theta} \\ \qquad = \sum_ {n = - \infty} ^ {\infty} r ^ {| n |} \left(\frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (\varphi) e ^ {- i n \varphi} d \varphi\right) e ^ {i n \theta} \\ \qquad = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (\varphi) \left(\sum_ {n = - \infty} ^ {\infty} r ^ {| n |} e ^ {- i n (\varphi - \theta)}\right) d \varphi , \end{array}
$$

where the interchange of the integral and infinite sum is justified by the uniform convergence of the series. 

Lemma 5.5 $I f 0 \leq r < 1$ , then 

$$
P _ {r} (\theta) = \frac {1 - r ^ {2}}{1 - 2 r \cos \theta + r ^ {2}}.
$$

The Poisson kernel is a good kernel,<sup>8</sup> as r tends to 1 from below. 

Proof. The identity $\begin{array} { r } { P _ { r } ( \theta ) = \frac { 1 - r ^ { 2 } } { 1 - 2 r \cos \theta + r ^ { 2 } } } \end{array}$ has already been derived in Section 1.1. Note that 

$$
1 - 2 r \cos \theta + r ^ {2} = (1 - r) ^ {2} + 2 r (1 - \cos \theta).
$$

Hence if $1 / 2 \le r \le 1$ and $\delta \le | \theta | \le \pi$ , then 

$$
1 - 2 r \cos \theta + r ^ {2} \geq c _ {\delta} > 0.
$$

Thus $P _ { r } ( \theta ) \leq ( 1 - r ^ { 2 } ) / c \delta$ when $\delta \le | \theta | \le \pi$ , and the third property of good kernels is verified. Clearly $P _ { r } ( \theta ) \geq 0 .$ , and integrating the expression $( 4 )$ term by term (which is justified by the absolute convergence of the series) yields 

$$
\frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} P _ {r} (\theta) d \theta = 1,
$$

thereby concluding the proof that $P _ { r }$ is a good kernel. 

Combining this lemma with Theorem 4.1, we obtain our next result. 

Theorem 5.6 The Fourier series of an integrable function on the circle is Abel summable to f at every point of continuity. Moreover, if f is continuous on the circle, then the Fourier series of f is uniformly Abel summable to f. 

We now return to a problem discussed in Chapter 1, where we sketched the solution of the steady-state heat equation $\triangle u = 0$ in the unit disc with boundary condition $u = f$ on the circle. We expressed the Laplacian in terms of polar coordinates, separated variables, and expected that a solution was given by 

$$
u (r, \theta) = \sum_ {m = - \infty} ^ {\infty} a _ {m} r ^ {| m |} e ^ {i m \theta},\tag{5}
$$

where $a _ { m }$ was the $m ^ { \mathrm { t h } }$ Fourier coeficient of $f .$ In other words, we were led to take 

$$
u (r, \theta) = A _ {r} (f) (\theta) = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (\varphi) P _ {r} (\theta - \varphi) d \varphi .
$$

We are now in a position to show that this is indeed the case. 

Theorem 5.7 Let f be an integrable function defined on the unit circle. Then the function u defined in the unit disc by the Poisson integral 

$$
u (r, \theta) = (f * P _ {r}) (\theta)\tag{6}
$$

has the following properties: 

(i) u has two continuous derivatives in the unit disc and satisfies $\triangle u = 0$ 

(ii) $I f \theta$ is any point of continuity of $f _ { i }$ , then 

$$
\lim _ {r \to 1} u (r, \theta) = f (\theta).
$$

If f is continuous everywhere, then this limit is uniform. 

(iii) If f is continuous, then u $( r , \theta )$ is the unique solution to the steadystate heat equation in the disc which satisfies conditions (i) and (ii). 

Proof. For (i), we recall that the function u is given by the series (5). Fix $\rho < 1$ ; inside each disc of radius $r < \rho < 1$ centered at the origin, the series for u can be diferentiated term by term, and the diferentiated series is uniformly and absolutely convergent. Thus u can be diferentiated twice (in fact infinitely many times), and since this holds for all $\rho < 1$ we conclude that u is twice diferentiable inside the unit disc. Moreover, in polar coordinates, 

$$
\triangle u = \frac {\partial^ {2} u}{\partial r ^ {2}} + \frac {1}{r} \frac {\partial u}{\partial r} + \frac {1}{r ^ {2}} \frac {\partial^ {2} u}{\partial \theta^ {2}},
$$

so term by term diferentiation shows that $\triangle u = 0$ 

The proof of (ii) is a simple application of the previous theorem. To prove (iii) we argue as follows. Suppose v solves the steady-state heat equation in the disc and converges to f uniformly as r tends to 1 from below. For each fixed r with $0 < r < 1$ , the function $v ( r , \theta )$ has a Fourier series 

$$
\sum_ {n = - \infty} ^ {\infty} a _ {n} (r) e ^ {i n \theta} \quad \mathrm{where} \quad a _ {n} (r) = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} v (r, \theta) e ^ {- i n \theta} d \theta .
$$

Taking into account that $v ( r , \theta )$ solves the equation 

$$
\frac {\partial^ {2} v}{\partial r ^ {2}} + \frac {1}{r} \frac {\partial v}{\partial r} + \frac {1}{r ^ {2}} \frac {\partial^ {2} v}{\partial \theta^ {2}} = 0,\tag{7}
$$

we find that 

$$
a _ {n} ^ {\prime \prime} (r) + \frac {1}{r} a _ {n} ^ {\prime} (r) - \frac {n ^ {2}}{r ^ {2}} a _ {n} (r) = 0.\tag{8}
$$

Indeed, we may first multiply (7) by $e ^ { - i n \theta }$ and integrate in θ. Then, since v is periodic, two integrations by parts give 

$$
\frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} \frac {\partial^ {2} v}{\partial \theta^ {2}} (r, \theta) e ^ {- i n \theta} d \theta = - n ^ {2} a _ {n} (r).
$$

Finally, we may interchange the order of diferentiation and integration, which is permissible since v has two continuous derivatives; this yields (8). 

Therefore, we must have $a _ { n } ( r ) = A _ { n } r ^ { n } + B _ { n } r ^ { - n }$ for some constants $A _ { n }$ and $B _ { n }$ , when $n \neq 0$ (see Exercise 11 in Chapter 1). To evaluate the constants, we first observe that each term $a _ { n } ( r )$ is bounded because v is bounded, therefore $B _ { n } = 0$ . To find $A _ { n }$ we let $r \to 1$ . Since v converges uniformly to $f$ as $r \to 1$ we find that 

$$
A _ {n} = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (\theta) e ^ {- i n \theta} d \theta .
$$

By a similar argument, this formula also holds when $n = 0$ . Our conclusion is that for each $0 < r < 1$ , the Fourier series of v is given by the series of $u ( r , \theta )$ , so by the uniqueness of Fourier series for continuous functions, we must have $u = v .$ 

Remark. By part (iii) of the theorem, we may conclude that if u solves $\triangle u = 0$ in the disc, and converges to 0 uniformly as $r \to 1$ , then u must be identically 0. However, if uniform convergence is replaced by pointwise convergence, this conclusion may fail; see Exercise 18. 

## 6 Exercises

1. Suppose $f$ is 2π-periodic and integrable on any finite interval. Prove that if $a , b \in \mathbb { R }$ , then 

$$
\int_ {a} ^ {b} f (x) d x = \int_ {a + 2 \pi} ^ {b + 2 \pi} f (x) d x = \int_ {a - 2 \pi} ^ {b - 2 \pi} f (x) d x.
$$

Also prove that 

$$
\int_ {- \pi} ^ {\pi} f (x + a) d x = \int_ {- \pi} ^ {\pi} f (x) d x = \int_ {- \pi + a} ^ {\pi + a} f (x) d x.
$$

## 6. Exercises

2. In this exercise we show how the symmetries of a function imply certain properties of its Fourier coeficients. Let f be a 2π-periodic Riemann integrable function defined on R. 

(a) Show that the Fourier series of the function $f$ can be written as 

$$
f (\theta) \sim \hat {f} (0) + \sum_ {n \geq 1} [ \hat {f} (n) + \hat {f} (- n) ] \cos n \theta + i [ \hat {f} (n) - \hat {f} (- n) ] \sin n \theta .
$$

(b) Prove that if f is even, then ${ \hat { f } } ( n ) = { \hat { f } } ( - n )$ , and we get a cosine series. 

(c) Prove that if f is odd, then ${ \hat { f } } ( n ) = - { \hat { f } } ( - n )$ , and we get a sine series. 

(d) Suppose that $f ( \theta + \pi ) = f ( \theta )$ for all $\theta \in \mathbb { R }$ . Show that ${ \hat { f } } ( n ) = 0$ for all odd n. 

(e) Show that $f$ is real-valued if and only if ${ \overline { { { \hat { f } } ( n ) } } } = { \hat { f } } ( - n )$ for all $n .$ 

3. We return to the problem of the plucked string discussed in Chapter 1. Show that the initial condition $f$ is equal to its Fourier sine series 

$$
f (x) = \sum_ {m = 1} ^ {\infty} A _ {m} \sin m x \quad \text { with } \quad A _ {m} = \frac {2 h}{m ^ {2}} \frac {\sin m p}{p (\pi - p)}.
$$

[Hint: Note that $| A _ { m } | \leq C / m ^ { 2 } . ]$ 

4. Consider the 2π-periodic odd function defined on $[ 0 , \pi ]$ by $f ( \theta ) = \theta ( \pi - \theta )$ 

(a) Draw the graph of f. 

(b) Compute the Fourier coeficients of $f ,$ and show that 

$$
f (\theta) = \frac {8}{\pi} \sum_ {k \text { odd } \geq 1} \frac {\sin k \theta}{k ^ {3}}.
$$

5. On the interval $[ - \pi , \pi ]$ consider the function 

$$
f (\theta) = \left\{ \begin{array}{l l} 0 & \text { if } | \theta | > \delta , \\ 1 - | \theta | / \delta & \text { if } | \theta | \leq \delta . \end{array} \right.
$$

Thus the graph of f has the shape of a triangular tent. Show that 

$$
f (\theta) = \frac {\delta}{2 \pi} + 2 \sum_ {n = 1} ^ {\infty} \frac {1 - \cos n \delta}{n ^ {2} \pi \delta} \cos n \theta .
$$

6. Let f be the function defined on $[ - \pi , \pi ]$ by $f ( \theta ) = | \theta |$ 

(a) Draw the graph of $f .$ 

(b) Calculate the Fourier coeficients of $f ,$ and show that 

$$
\hat {f} (n) = \left\{ \begin{array}{l l} \frac {\pi}{2} & \text {if n = 0 ,} \\ \frac {- 1 + (- 1) ^ {n}}{\pi n ^ {2}} & \text {if n\neq 0 .} \end{array} \right.
$$

(c) What is the Fourier series of f in terms of sines and cosines? 

(d) Taking $\theta = 0 ,$ prove that 

$$
\sum_ {n \text {odd} \geq 1} \frac {1}{n ^ {2}} = \frac {\pi^ {2}}{8} \quad \text {and} \quad \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {2}} = \frac {\pi^ {2}}{6}.
$$

See also Example 2 in Section 1.1. 

7. Suppose $\{ a _ { n } \} _ { n = 1 } ^ { N }$ and $\{ b _ { n } \} _ { n = 1 } ^ { N }$ are two finite sequences of complex numbers. Let $\begin{array} { r } { B _ { k } = \sum _ { n = 1 } ^ { k } b _ { n } } \end{array}$ denote the partial sums of the series $\sum b _ { n }$ with the convention $B _ { 0 } = 0$ 

(a) Prove the summation by parts formula 

$$
\sum_ {n = M} ^ {N} a _ {n} b _ {n} = a _ {N} B _ {N} - a _ {M} B _ {M - 1} - \sum_ {n = M} ^ {N - 1} (a _ {n + 1} - a _ {n}) B _ {n}.
$$

(b) Deduce from this formula Dirichlet’s test for convergence of a series: if the partial sums of the series $\sum b _ { n }$ are bounded, and $\left\{ a _ { n } \right\}$ is a sequence of real numbers that decreases monotonically to 0, then $\sum a _ { n } b _ { n }$ converges. 

8. Verify that $\frac { 1 } { 2 i } \sum _ { n \neq 0 } \frac { e ^ { i n x } } { n }$ is the Fourier series of the 2π-periodic sawtooth function illustrated in Figure 6, defined by $f ( 0 ) = 0$ , and 

$$
f (x) = \left\{ \begin{array}{l l} - \frac {\pi}{2} - \frac {x}{2} & \text { if } - \pi <   x <   0, \\ \frac {\pi}{2} - \frac {x}{2} & \text { if } 0 <   x <   \pi . \end{array} \right.
$$

Note that this function is not continuous. Show that nevertheless, the series converges for every x (by which we mean, as usual, that the symmetric partial sums of the series converge). In particular, the value of the series at the origin, namely $0 ,$ is the average of the values of $f ( x )$ as x approaches the origin from the left and the right. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/dbfb2ec473e91899578934e382e83705c6e5926e2ec5383ecc067a5885a1f397.jpg)



Figure 6. The sawtooth function


[Hint: Use Dirichlet’s test for convergence of a series $\textstyle \sum a _ { n } b _ { n } . ]$ 

9. Let $f ( x ) = \chi _ { [ a , b ] } ( x )$ be the characteristic function of the interval $[ a , b ] \subset$ $[ - \pi , \pi ]$ , that is, 

$$
\chi_ {[ a, b ]} (x) = \left\{ \begin{array}{l l} 1 & \text { if } x \in [ a, b ], \\ 0 & \text { otherwise }. \end{array} \right.
$$

(a) Show that the Fourier series of f is given by 

$$
f (x) \sim \frac {b - a}{2 \pi} + \sum_ {n \neq 0} \frac {e ^ {- i n a} - e ^ {- i n b}}{2 \pi i n} e ^ {i n x}.
$$

The sum extends over all positive and negative integers excluding 0. 

(b) Show that if $a \neq - \pi$ or $b \neq \pi$ and $a \neq b .$ then the Fourier series does not converge absolutely for any x. [Hint: It sufices to prove that for many values of n one has | sin $n \theta _ { 0 } | \geq c > 0$ where $\theta _ { 0 } = ( b - a ) / 2 .$ ] 

(c) However, prove that the Fourier series converges at every point x. What happens if $a = - \pi$ and $b = \pi ?$ 

10. Suppose $f$ is a periodic function of period 2π which belongs to the class $C ^ { k }$ Show that 

$$
\hat {f} (n) = O (1 / | n | ^ {k}) \quad \mathrm{as} | n | \to \infty .
$$

This notation means that there exists a constant C such $| { \hat { f } } ( n ) | \leq C / | n | ^ { k }$ . We could also write this as $| n | ^ { k } { \hat { f } } ( n ) = O ( 1 )$ , where $O ( 1 )$ means bounded. 

[Hint: Integrate by parts.] 

11. Suppose that $\{ f _ { k } \} _ { k = 1 } ^ { \infty }$ is a sequence of Riemann integrable functions on the interval [0, 1] such that 

$$
\int_ {0} ^ {1} | f _ {k} (x) - f (x) | d x \to 0 \quad \text { as } k \to \infty .
$$

Show that ${ \hat { f } } _ { k } ( n ) \to { \hat { f } } ( n )$ uniformly in n as $k \to \infty$ 

12. Prove that if a series of complex numbers $\sum c _ { n }$ converges to s, then $\sum c _ { n }$ is Ces`aro summable to s. 

[Hint: Assume $s _ { n } \to 0 \mathrm { ~ a s ~ } n \to \infty . ]$ 

13. The purpose of this exercise is to prove that Abel summability is stronger than the standard or Ces`aro methods of summation. 

(a) Show that if the series $\sum _ { n = 1 } ^ { \infty } c _ { n }$ of complex numbers converges to a finite limit s, then the series is Abel summable to s. [Hint: Why is it enough to prove the theorem when $s = 0 ?$ Assuming $s = 0$ , show that if $s _ { N } = c _ { 1 } +$ $\cdots + c _ { N }$ , then $\begin{array} { r } { \sum _ { n = 1 } ^ { N } c _ { n } r ^ { n } = ( 1 - r ) \sum _ { n = 1 } ^ { N ^ { \smile } } s _ { n } r ^ { n } + s _ { N } r ^ { N + 1 } } \end{array}$ . Let $N \to \infty$ to show that 

$$
\sum c _ {n} r ^ {n} = (1 - r) \sum s _ {n} r ^ {n}.
$$

Finally, prove that the right-hand side converges to 0 as $r  1 . ]$ 

(b) However, show that there exist series which are Abel summable, but that do not converge. [Hint: Try $c _ { n } = ( - 1 ) ^ { n }$ . What is the Abel limit of $\sum c _ { n } ? ]$ 

(c) Argue similarly to prove that if a series $\sum _ { n = 1 } ^ { \infty } c _ { n }$ is Ces`aro summable to σ, then it is Abel summable to σ. [Hint: Note that 

$$
\sum_ {n = 1} ^ {\infty} c _ {n} r ^ {n} = (1 - r) ^ {2} \sum_ {n = 1} ^ {\infty} n \sigma_ {n} r ^ {n},
$$

and assume $\sigma = 0 . ]$ 

(d) Give an example of a series that is Abel summable but not Ces`aro summable. [Hint: Try $c _ { n } = ( - 1 ) ^ { n - 1 } n$ . Note that if $\sum c _ { n }$ is Ces`aro summable, then $c _ { n } / n$ tends to 0.] 

The results above can be summarized by the following implications about series: 

$$
\text { convergent } \Longrightarrow \text { Cesàro   summable } \Longrightarrow \text { Abel   summable },
$$

and the fact that none of the arrows can be reversed. 

14. This exercise deals with a theorem of Tauber which says that under an additional condition on the coeficients $c _ { n } .$ the above arrows can be reversed. 

(a) $\operatorname { I f } \sum c _ { n }$ is Ces`aro summable to σ and $c _ { n } = o ( 1 / n )$ (that $\mathrm { i s } , n c _ { n }  0 )$ , then $\sum c _ { n }$ converges to σ. [Hint: $s _ { n } - \sigma _ { n } = [ ( n - 1 ) c _ { n } + \cdots + c _ { 2 } ] / n . ]$ 

(b) The above statement holds if we replace Ces`aro summable by Abel summable. [Hint: Estimate the diference between $\sum _ { n = 1 } ^ { N } c _ { n }$ and $\textstyle \sum _ { n = 1 } ^ { N } c _ { n } r ^ { n }$ where $\dot { r } = 1 - 1 / N . ]$ 

## 6. Exercises

15. Prove that the Fej´er kernel is given by 

$$
F _ {N} (x) = \frac {1}{N} \frac {\sin^ {2} (N x / 2)}{\sin^ {2} (x / 2)}.
$$

[Hint: Remember that $N F _ { N } ( x ) = D _ { 0 } ( x ) + \cdot \cdot \cdot + D _ { N - 1 } ( x )$ where $D _ { n } ( x )$ is the Dirichlet kernel. Therefore, if $\omega = e ^ { i x }$ we have 

$$
N F _ {N} (x) = \sum_ {n = 0} ^ {N - 1} \frac {\omega^ {- n} - \omega^ {n + 1}}{1 - \omega}. ]
$$

16. The Weierstrass approximation theorem states: Let $f$ be a continuous function on the closed and bounded interval $[ a , b ] \subset \mathbb { R }$ . Then, for any $\epsilon > 0 ,$ there exists a polynomial $P$ such that 

$$
\sup _ {x \in [ a, b ]} | f (x) - P (x) | <   \epsilon .
$$

Prove this by applying Corollary 5.4 of Fej´er’s theorem and using the fact that the exponential function $e ^ { i x }$ can be approximated by polynomials uniformly on any interval. 

17. In Section 5.4 we proved that the Abel means of $f$ converge to $f$ at all points of continuity, that is, 

$$
\lim _ {r \to 1} A _ {r} (f) (\theta) = \lim _ {r \to 1} (P _ {r} * f) (\theta) = f (\theta), \quad \mathrm{with} 0 <   r <   1,
$$

whenever $f$ is continuous at $\theta .$ In this exercise, we will study the behavior of $A _ { r } ( f ) ( \theta )$ at certain points of discontinuity. 

An integrable function is said to have a jump discontinuity at θ if the two limits 

$$
\lim_{\substack{h  \to   0\\ h  > 0}}f(\theta +h) = f(\theta^{+})\quad \text{and}\quad \lim_{\substack{h  \to   0\\ h  > 0}}f(\theta -h) = f(\theta^{-})
$$

exist. 

(a) Prove that if f has a jump discontinuity at $\theta ,$ then 

$$
\lim _ {r \to 1} A _ {r} (f) (\theta) = \frac {f (\theta^ {+}) + f (\theta^ {-})}{2}, \quad \text { with } 0 \leq r <   1.
$$

[Hint: Explain why $\begin{array} { r } { { \frac { 1 } { 2 \pi } } \int _ { - \pi } ^ { 0 } P _ { r } ( \theta ) d \theta = { \frac { 1 } { 2 \pi } } \int _ { 0 } ^ { \pi } P _ { r } ( \theta ) d \theta = { \frac { 1 } { 2 } } } \end{array}$ , then modify the proof given in the text.] 

(b) Using a similar argument, show that if f has a jump discontinuity at $\theta ,$ the Fourier series of $f$ at θ is Ces`aro summable to $\frac { f ( \theta ^ { + } ) + f ( \theta ^ { - } ) } { 2 }$ 

18. If $P _ { r } ( \theta )$ denotes the Poisson kernel, show that the function 

$$
u (r, \theta) = \frac {\partial P _ {r}}{\partial \theta},
$$

defined for $0 \leq r < 1$ and $\theta \in \mathbb { R }$ , satisfies: 

(i) $\triangle u = 0$ in the disc. 

(ii) lim $\boldsymbol { \mathrm { 1 } } _ { r \to 1 } \boldsymbol { u } ( r , \theta ) = 0$ for each θ. 

However, u is not identically zero. 

19. Solve Laplace’s equation $\triangle u = 0$ in the semi infinite strip 

$$
S = \{(x, y): 0 <   x <   1, 0 <   y \},
$$

subject to the following boundary conditions 

$$
\left\{ \begin{array}{r l} u (0, y) = 0 & \text { when } 0 \leq y, \\ u (1, y) = 0 & \text { when } 0 \leq y, \\ u (x, 0) = f (x) & \text { when } 0 \leq x \leq 1 \end{array} \right.
$$

where $f$ is a given function, with of course $f ( 0 ) = f ( 1 ) = 0$ . Write 

$$
f (x) = \sum_ {n = 1} ^ {\infty} a _ {n} \sin (n \pi x)
$$

and expand the general solution in terms of the special solutions given by 

$$
u _ {n} (x, y) = e ^ {- n \pi y} \sin (n \pi x).
$$

Express u as an integral involving $f ,$ analogous to the Poisson integral formula (6). 

20. Consider the Dirichlet problem in the annulus defined by $\{ ( r , \theta ) : \rho < r < 1 \}$ , where $0 < \rho < 1$ is the inner radius. The problem is to solve 

$$
\frac {\partial^ {2} u}{\partial r ^ {2}} + \frac {1}{r} \frac {\partial u}{\partial r} + \frac {1}{r ^ {2}} \frac {\partial^ {2} u}{\partial \theta^ {2}} = 0
$$

subject to the boundary conditions 

$$
\left\{ \begin{array}{l} u (1, \theta) = f (\theta), \\ u (\rho , \theta) = g (\theta), \end{array} \right.
$$

## 7. Problems

where $f$ and $g$ are given continuous functions. 

Arguing as we have previously for the Dirichlet problem in the disc, we can hope to write 

$$
u (r, \theta) = \sum c _ {n} (r) e ^ {i n \theta}
$$

with $c _ { n } ( r ) = A _ { n } r ^ { n } + B _ { n } r ^ { - n } , n \neq 0 ,$ . Set 

$$
f (\theta) \sim \sum a _ {n} e ^ {i n \theta} \quad \mathrm{and} \quad g (\theta) \sim \sum b _ {n} e ^ {i n \theta}.
$$

We want $c _ { n } ( 1 ) = a _ { n }$ and $c _ { n } ( \rho ) = b _ { n }$ . This leads to the solution 

$$
\begin{array}{l} u (r, \theta) = \sum_ {n \neq 0} \left(\frac {1}{\rho^ {n} - \rho^ {- n}}\right) \left[ ((\rho / r) ^ {n} - (r / \rho) ^ {n})   a _ {n} + (r ^ {n} - r ^ {- n}) b _ {n} \right] e ^ {i n \theta} \\ \quad + a _ {0} + (b _ {0} - a _ {0}) \frac {\log r}{\log \rho}. \end{array}
$$

Show that as a result we have 

$$
u (r, \theta) - (P _ {r} * f) (\theta) \rightarrow 0 \quad \text {   as   } r \rightarrow 1 \text {   uniformly   in   } \theta ,
$$

and 

$$
u (r, \theta) - (P _ {\rho / r} * g) (\theta) \rightarrow 0 \quad \text { as } r \rightarrow \rho \text { uniformly   in } \theta .
$$

## 7 Problems

1. One can construct Riemann integrable functions on $[ 0 , 1 ]$ that have a dense set of discontinuities as follows. 

(a) Let $f ( x ) = 0$ when $x < 0 .$ , and $f ( x ) = 1 \operatorname { i f } x \geq 0$ . Choose a countable dense sequence $\{ r _ { n } \}$ in $[ 0 , 1 ]$ . Then, show that the function 

$$
F (x) = \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {2}} f (x - r _ {n})
$$

is integrable and has discontinuities at all points of the sequence $\left\{ r _ { n } \right\}$ [Hint: $\bar { F }$ is monotonic and bounded.] 

(b) Consider next 

$$
F (x) = \sum_ {n = 1} ^ {\infty} 3 ^ {- n} g (x - r _ {n}),
$$

where $g ( x ) = \sin { 1 / x }$ when $x \neq 0 ,$ and $g ( 0 ) = 0$ . Then $F$ is integrable, discontinuous at each $x = r _ { n } ,$ , and fails to be monotonic in any subinterval of [0, 1]. [Hint: Use the fact that $\begin{array} { r } { 3 ^ { - k } > \sum _ { n > k } 3 ^ { - n } . ] } \end{array}$ 

(c) The original example of Riemann is the function 

$$
F (x) = \sum_ {n = 1} ^ {\infty} \frac {(n x)}{n ^ {2}},
$$

where $( x ) = x$ for $x \in ( - 1 / 2 , 1 / 2 ]$ and $( x )$ is continued to R by periodicity, that is, $( x + 1 ) = ( x )$ . It can be shown that $F$ is discontinuous whenever $x = m / 2 n$ , where $m , n \in \mathbb { Z }$ with m odd and $n \neq 0$ 

2. Let $D _ { N }$ denote the Dirichlet kernel 

$$
D _ {N} (\theta) = \sum_ {k = - N} ^ {N} e ^ {i k \theta} = \frac {\sin ((N + 1 / 2) \theta)}{\sin (\theta / 2)},
$$

and define 

$$
L _ {N} = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} | D _ {N} (\theta) | d \theta .
$$

(a) Prove that 

$$
L _ {N} \geq c \log N
$$

for some constant $c > 0 .$ . [Hint: Show that $\begin{array} { r } { | D _ { N } ( \theta ) | \ge c ^ { \frac { \sin ( ( N + 1 / 2 ) \theta ) } { | \theta | } } } \end{array}$ , change variables, and prove that 

$$
L _ {N} \geq c \int_ {\pi} ^ {N \pi} \frac {| \sin \theta |}{| \theta |} d \theta + O (1).
$$

Write the integral as a sum $\begin{array} { r l } { \sum _ { k = 1 } ^ { N - 1 } \int _ { k \pi } ^ { ( k + 1 ) \pi } } & { { } } \end{array}$ . To conclude, use the fact that $\textstyle \sum _ { k = 1 } ^ { n } 1 / k \geq c \log n . ]$ A more careful estimate gives 

$$
L _ {N} = \frac {4}{\pi^ {2}} \log N + O (1).
$$

(b) Prove the following as a consequence: for each $n \geq 1$ , there exists a continuous function $f _ { n }$ such that $| f _ { n } | \leq 1$ and $\vert S _ { n } ( f _ { n } ) ( 0 ) \vert \geq c ^ { \prime }$ log n. [Hint: The function $g _ { n }$ which is equal to 1 when $D _ { n }$ is positive and −1 when $D _ { n }$ is negative has the desired property but is not continuous. Approximate $g _ { n }$ in the integral norm (in the sense of Lemma 3.2) by continuous functions $h _ { k }$ satisfying $| h _ { k } | \leq 1 . ]$ 

3.<sup>∗</sup> Littlewood provided a refinement of Tauber’s theorem: 

7. Problems 

(a) If $\sum c _ { n }$ is Abel summable to s and $c _ { n } = O ( 1 / n )$ , then $\sum c _ { n }$ converges to s. 

(b) As a consequence, $\operatorname { i f } \sum c _ { n }$ is Ces`aro summable to s and $c _ { n } = O ( 1 / n )$ , then $\sum c _ { n }$ converges to s. 

These results may be applied to Fourier series. By Exercise 17, they imply that if f is an integrable function that satisfies ${ \hat { f } } ( \nu ) = O ( 1 / | \nu | )$ , then: 

(i) If f is continuous at $\theta ,$ then 

$$
S _ {N} (f) (\theta) \to f (\theta) \quad \mathrm{as} N \to \infty .
$$

(ii) If f has a jump discontinuity at θ, then 

$$
S _ {N} (f) (\theta) \rightarrow \frac {f (\theta^ {+}) + f (\theta^ {-})}{2} \quad \mathrm{as} N \rightarrow \infty .
$$

(iii) If f is continuous on $[ - \pi , \pi ]$ , then $S _ { N } ( f ) \to f$ uniformly. 

For the simpler assertion (b), hence a proof of (i), (ii), and (iii), see Problem 5 in Chapter 4. 

## 3 <sub>Convergence</sub> <sub>of</sub> <sub>Fourier</sub> <sub>Series</sub>

The sine and cosine series, by which one can represent an arbitrary function in a given interval, enjoy among other remarkable properties that of being convergent. This property did not escape the great geometer (Fourier) who began, through the introduction of the representation of functions just mentioned, a new career for the applications of analysis; it was stated in the Memoir which contains his first research on heat. But no one so far, to my knowledge, gave a general proof of it . . . 

G. Dirichlet, 1829 

In this chapter, we continue our study of the problem of convergence of Fourier series. We approach the problem from two diferent points of view. 

The first is “global” and concerns the overall behavior of a function f over the entire interval $[ 0 , 2 \pi ]$ . The result we have in mind is “meansquare convergence”: if $f$ is integrable on the circle, then 

$$
\frac {1}{2 \pi} \int_ {0} ^ {2 \pi} | f (\theta) - S _ {N} (f) (\theta) | ^ {2} d \theta \rightarrow 0 \quad \mathrm{as} N \rightarrow \infty .
$$

At the heart of this result is the fundamental notion of “orthogonal-$\mathrm { i t y ^ { \dag } }$ ; this idea is expressed in terms of vector spaces with inner products, and their related infinite dimensional variants, the Hilbert spaces. A connected result is the Parseval identity which equates the mean-square “norm” of the function with a corresponding norm of its Fourier coeficients. Orthogonality is a fundamental mathematical notion which has many applications in analysis. 

The second viewpoint is “local” and concerns the behavior of $f$ near a given point. The main question we consider is the problem of pointwise convergence: does the Fourier series of $f$ converge to the value $f ( \theta )$ for a given $\theta ?$ We first show that this convergence does indeed hold whenever $f$ is diferentiable at θ. As a corollary, we obtain the Riemann localization principle, which states that the question of whether or not $S _ { N } ( f ) ( \theta ) \to f ( \theta )$ is completely determined by the behavior of $f$ in an arbitrarily small interval about θ. This is a remarkable result since the Fourier coeficients, hence the Fourier series, of $f$ depend on the values of $f$ on the whole interval [0, 2π]. 

Even though convergence of the Fourier series holds at points where $f$ is diferentiable, it may fail if $f$ is merely continuous. The chapter concludes with the presentation of a continuous function whose Fourier series does not converge at a given point, as promised earlier. 

## 1 Mean-square convergence of Fourier series

The aim of this section is the proof of the following theorem. 

Theorem 1.1 Suppose f is integrable on the circle. Then 

$$
\frac {1}{2 \pi} \int_ {0} ^ {2 \pi} | f (\theta) - S _ {N} (f) (\theta) | ^ {2} d \theta \to 0 \quad a s N \to \infty .
$$

As we remarked earlier, the key concept involved is that of orthogonality. The correct setting for orthogonality is in a vector space equipped with an inner product. 

## 1.1 Vector spaces and inner products

We now review the definitions of a vector space over R or $\mathbb { C } ,$ an inner product, and its associated norm. In addition to the familiar finitedimensional vector spaces $\mathbb { R } ^ { d }$ and $\mathbb { C } ^ { d }$ , we also examine two infinitedimensional examples which play a central role in the proof of Theorem 1.1. 

## Preliminaries on vector spaces

A vector space V over the real numbers R is a set whose elements may be “added” together, and “multiplied” by scalars. More precisely, we may associate to any pair $X , Y \in V$ an element in V called their sum and denoted by $X + Y$ . We require that this addition respects the usual laws of arithmetic, such as commutativity $X + Y = Y + X$ , and associativity $X + ( Y + Z ) = ( X + Y ) + Z ,$ , etc. Also, given any $X \in V$ and real number $\lambda ,$ , we assign an element $\lambda X \in V$ called the product of X by λ. This scalar multiplication must satisfy the standard properties, for instance $\lambda _ { 1 } ( \lambda _ { 2 } X ) = ( \lambda _ { 1 } \lambda _ { 2 } ) X$ and $\lambda ( X + Y ) = \lambda X + \lambda Y$ . We may instead allow scalar multiplication by numbers in $\mathbb { C } ;$ we then say that V is a vector space over the complex numbers. 

## 1. Mean-square convergence of Fourier series

For example, the set $\mathbb { R } ^ { d }$ of d-tuples of real numbers $( x _ { 1 } , x _ { 2 } , \ldots , x _ { d } )$ is a vector space over the reals. Addition is defined componentwise by 

$$
(x _ {1}, \ldots , x _ {d}) + (y _ {1}, \ldots , y _ {d}) = (x _ {1} + y _ {1}, \ldots , x _ {d} + y _ {d}),
$$

and so is multiplication by a scalar $\lambda \in \mathbb { R }$ 

$$
\lambda (x _ {1}, \dots , x _ {d}) = (\lambda x _ {1}, \dots , \lambda x _ {d}).
$$

Similarly, the space $\mathbb { C } ^ { d }$ (the complex version of the previous example) is the set of d-tuples of complex numbers $( z _ { 1 } , z _ { 2 } , \ldots , z _ { d } )$ . It is a vector space over C with addition defined componentwise by 

$$
(z _ {1}, \ldots , z _ {d}) + (w _ {1}, \ldots , w _ {d}) = (z _ {1} + w _ {1}, \ldots , z _ {d} + w _ {d}).
$$

Multiplication by scalars $\lambda \in \mathbb { C }$ is given by 

$$
\lambda (z _ {1}, \dots , z _ {d}) = (\lambda z _ {1}, \dots , \lambda z _ {d}).
$$

An inner product on a vector space $V$ over R associates to any pair $X , Y$ of elements in V a real number which we denote by $( X , Y )$ . In particular, the inner product must be symmetric $( X , Y ) = ( Y , X )$ and linear in both variables; that is, 

$$
(\alpha X + \beta Y, Z) = \alpha (X, Z) + \beta (Y, Z)
$$

whenever $\alpha , \beta \in \mathbb { R }$ and $X , Y , Z \in V$ . Also, we require that the inner product be positive-definite, that is, $( X , X ) \geq 0$ for all X in V . In particular, given an inner product $( \cdot , \cdot )$ we may define the norm of X by 

$$
\| X \| = (X, X) ^ {1 / 2}.
$$

If in addition $\| X \| = 0$ implies $X = 0$ , we say that the inner product is strictly positive-definite. 

For example, the space $\mathbb { R } ^ { d }$ is equipped with a (strictly positive-definite) inner product defined by 

$$
(X, Y) = x _ {1} y _ {1} + \dots + x _ {d} y _ {d}
$$

when $X = ( x _ { 1 } , \ldots , x _ { d } )$ and $Y = \left( y _ { 1 } , \dots , y _ { d } \right)$ . Then 

$$
\| X \| = (X, X) ^ {1 / 2} = \sqrt {x _ {1} ^ {2} + \cdots + x _ {d} ^ {2}},
$$

which is the usual Euclidean distance. One also uses the notation $| X |$ instead of $\| X \|$ 

For vector spaces over the complex numbers, the inner product of two elements is a complex number. Moreover, these inner products are called Hermitian (instead of symmetric) since they must satisfy $( X , Y ) = { \overline { { ( Y , X ) } } }$ . Hence the inner product is linear in the first variable, but conjugate-linear in the second: 

$$
(\alpha X + \beta Y, Z) = \alpha (X, Z) + \beta (Y, Z) \quad \text { and }
$$

$$
(X, \alpha Y + \beta Z) = \overline {{\alpha}} (X, Y) + \overline {{\beta}} (X, Z).
$$

Also, we must have $( X , X ) \geq 0$ , and the norm of X is defined by $\| X \| = ( X , X ) ^ { 1 / 2 }$ as before. Again, the inner product is strictly positivedefinite if $\| X \| = 0$ implies $X = 0$ 

For example, the inner product of two vectors $Z = ( z _ { 1 } , \ldots , z _ { d } )$ and $W = \left( w _ { 1 } , \ldots , w _ { d } \right)$ in $\mathbb { C } ^ { d }$ is defined by 

$$
(Z, W) = z _ {1} \overline {{w _ {1}}} + \dots + z _ {d} \overline {{w _ {d}}}.
$$

The norm of the vector Z is then given by 

$$
\| Z \| = (Z, Z) ^ {1 / 2} = \sqrt {| z _ {1} | ^ {2} + \cdots + | z _ {d} | ^ {2}}.
$$

The presence of an inner product on a vector space allows one to define the geometric notion of “orthogonality.” Let V be a vector space (over R or C) with inner product $( \cdot , \cdot )$ and associated norm $\| \cdot \|$ . Two elements $X$ and $Y$ are orthogonal if $( X , Y ) = 0$ , and we write $X \perp Y$ . Three important results can be derived from this notion of orthogonality: 

(i) The Pythagorean theorem: if X and $Y$ are orthogonal, then 

$$
\left\| X + Y \right\| ^ {2} = \left\| X \right\| ^ {2} + \left\| Y \right\| ^ {2}.
$$

(ii) The Cauchy-Schwarz inequality: for any $X , Y \in V$ we have 

$$
| (X, Y) | \leq \| X \| \| Y \|.
$$

(iii) The triangle inequality: for any $X , Y \in V$ we have 

$$
\| X + Y \| \leq \| X \| + \| Y \|.
$$

## 1. Mean-square convergence of Fourier series

The proofs of these facts are simple. For (i) it sufices to expand $( X + Y , X + Y )$ and use the assumption that $( X , Y ) = 0$ 

For (ii), we first dispose of the case when $\| Y \| = 0$ by showing that this implies $( X , Y ) = 0$ for all X. Indeed, for all real t we have 

$$
0 \leq \| X + t Y \| ^ {2} = \| X \| ^ {2} + 2 t \operatorname{Re} (X, Y)
$$

and $\operatorname { R e } ( X , Y ) \neq 0$ contradicts the inequality if we take t to be large and positive (or negative). Similarly, by considering $\| X + i t Y \| ^ { 2 }$ , we find that Im $( X , Y ) = 0$ 

If $\| Y \| \neq 0 ,$ , we may set $c = ( X , Y ) / ( Y , Y ) ;$ then $X - c Y$ is orthogonal to $Y ,$ , and therefore also to $c Y$ . If we write $X = X - c Y + c Y$ and apply the Pythagorean theorem, we get 

$$
\| X \| ^ {2} = \| X - c Y \| ^ {2} + \| c Y \| ^ {2} \geq | c | ^ {2} \| Y \| ^ {2}.
$$

Taking square roots on both sides gives the result. Note that we have equality in the above precisely when $X = c Y$ 

Finally, for (iii) we first note that 

$$
\left\| X + Y \right\| ^ {2} = (X, X) + (X, Y) + (Y, X) + (Y, Y).
$$

But $( X , X ) = \| X \| ^ { 2 } , ( Y , Y ) = \| Y \| ^ { 2 }$ , and by the Cauchy-Schwarz inequality 

$$
\left| (X, Y) + (Y, X) \right| \leq 2 \| X \| \| Y \|,
$$

therefore 

$$
\left\| X + Y \right\| ^ {2} \leq \left\| X \right\| ^ {2} + 2 \left\| X \right\| \left\| Y \right\| + \left\| Y \right\| ^ {2} = \left(\left\| X \right\| + \left\| Y \right\|\right) ^ {2}.
$$

## Two important examples

The vector spaces $\mathbb { R } ^ { d }$ and $\mathbb { C } ^ { d }$ are finite dimensional. In the context of Fourier series, we need to work with two infinite-dimensional vector spaces, which we now describe. 

Example 1. The vector space $\ell ^ { 2 } ( \mathbb { Z } )$ over $\mathbb { C }$ is the set of all (two-sided) infinite sequences of complex numbers 

$$
(\ldots , a _ {- n}, \ldots , a _ {- 1}, a _ {0}, a _ {1}, \ldots , a _ {n}, \ldots)
$$

such that 

$$
\sum_ {n \in \mathbb {Z}} | a _ {n} | ^ {2} <   \infty ;
$$

that is, the series converges. Addition is defined componentwise, and so is scalar multiplication. The inner product between the two vectors $A = ( \dots , a _ { - 1 } , a _ { 0 } , a _ { 1 } , \dots )$ and $B = ( \dots , b _ { - 1 } , b _ { 0 } , b _ { 1 } , \dots )$ is defined by the absolutely convergent series 

$$
(A, B) = \sum_ {n \in \mathbb {Z}} a _ {n} \overline {{b _ {n}}}.
$$

The norm of A is then given by 

$$
\| A \| = (A, A) ^ {1 / 2} = \left(\sum_ {n \in \mathbb {Z}} | a _ {n} | ^ {2}\right) ^ {1 / 2}.
$$

We must first check that $\ell ^ { 2 } ( \mathbb { Z } )$ is a vector space. This requires that if A and B are two elements in $\ell ^ { 2 } ( \mathbb { Z } )$ , then so is the vector $A + B$ . To see this, for each integer $N > 0$ we let $A _ { N }$ denote the truncated element 

$$
A _ {N} = (\dots , 0, 0, a _ {- N}, \dots , a _ {- 1}, a _ {0}, a _ {1}, \dots , a _ {N}, 0, 0, \dots),
$$

where we have set $a _ { n } = 0$ whenever $| n | > N$ . We define the truncated element $B _ { N }$ similarly. Then, by the triangle inequality which holds in a finite dimensional Euclidean space, we have 

$$
\| A _ {N} + B _ {N} \| \leq \| A _ {N} \| + \| B _ {N} \| \leq \| A \| + \| B \|.
$$

Thus 

$$
\sum_ {| n | \leq N} | a _ {n} + b _ {n} | ^ {2} \leq (\| A \| + \| B \|) ^ {2},
$$

and letting N tend to infinity gives $\begin{array} { r } { \sum _ { n \in \mathbb { Z } } | a _ { n } + b _ { n } | ^ { 2 } < \infty } \end{array}$ . It also follows that $\| A + B \| \leq \| A \| + \| B \|$ , which is the triangle inequality. The Cauchy-Schwarz inequality, which states that the sum $\textstyle \sum _ { n \in \mathbb { Z } } a _ { n } { \bar { b } } _ { n }$ converges absolutely and that $| ( A , B ) | \leq \| A \| \| B \|$ , can be deduced in the same way from its finite analogue. 

In the three examples $\mathbb { R } ^ { d } , \mathbb { C } ^ { d } ;$ and $\ell ^ { 2 } ( \mathbb { Z } )$ , the vector spaces with their inner products and norms satisfy two important properties: 

(i) The inner product is strictly positive-definite, that is, $\| X \| = 0$ implies $X = 0$ 

(ii) The vector space is complete, which by definition means that every Cauchy sequence in the norm converges to a limit in the vector space. 

## 1. Mean-square convergence of Fourier series

An inner product space with these two properties is called a Hilbert space. We see that $\mathbb { R } ^ { d }$ and $\mathbb { C } ^ { d }$ are examples of finite-dimensional Hilbert spaces, while $\ell ^ { 2 } ( \mathbb { Z } )$ is an example of an infinite-dimensional Hilbert space (see Exercises 1 and 2). If either of the conditions above fail, the space is called a pre-Hilbert space. 

We now give an important example of a pre-Hilbert space where both conditions (i) and (ii) fail. 

Example 2. Let R denote the set of complex-valued Riemann integrable functions on [0, 2π] (or equivalently, integrable functions on the circle). This is a vector space over C. Addition is defined pointwise by 

$$
(f + g) (\theta) = f (\theta) + g (\theta).
$$

Naturally, multiplication by a scalar $\lambda \in \mathbb { C }$ is given by 

$$
(\lambda f) (\theta) = \lambda \cdot f (\theta).
$$

An inner product is defined on this vector space by 

$$
(f, g) = \frac {1}{2 \pi} \int_ {0} ^ {2 \pi} f (\theta) \overline {{g (\theta)}} d \theta .\tag{1}
$$

The norm of f is then 

$$
\| f \| = \left(\frac {1}{2 \pi} \int_ {0} ^ {2 \pi} | f (\theta) | ^ {2} d \theta\right) ^ {1 / 2}.
$$

One needs to check that the analogue of the Cauchy-Schwarz and triangle inequalities hold in this example; that is, $| ( f , g ) | \leq \| f \| \| g \|$ and $\| f + g \| \leq \| f \| + \| g \|$ . While these facts can be obtained as consequences of the corresponding inequalities in the previous examples, the argument is a little elaborate and we prefer to proceed diferently. 

We first observe that $2 A B \le ( A ^ { 2 } + B ^ { 2 } )$ for any two real numbers A and B. If we set $A = \lambda ^ { 1 / 2 } | f ( \theta ) |$ and $B = \lambda ^ { - 1 / 2 } | g ( \theta ) |$ with $\lambda > 0$ , we get 

$$
| f (\theta) \overline {{g (\theta)}} | \leq \frac {1}{2} (\lambda | f (\theta) | ^ {2} + \lambda^ {- 1} | g (\theta) | ^ {2}).
$$

We then integrate this in θ to obtain 

$$
| (f, g) | \leq \frac {1}{2 \pi} \int_ {0} ^ {2 \pi} | f (\theta) | | \overline {{g (\theta)}} | d \theta \leq \frac {1}{2} (\lambda \| f \| ^ {2} + \lambda^ {- 1} \| g \| ^ {2}).
$$

Then, put $\lambda = \| g \| / \| f \|$ to get the Cauchy-Schwarz inequality. The triangle inequality is then a simple consequence, as we have seen above. 

Of course, in our choice of λ we must assume that $\| f \| \neq 0$ and $\| g \| \neq 0$ which leads us to the following observation. 

In R, condition (i) for a Hilbert space fails, since $\| f \| = 0$ implies only that f vanishes at its points of continuity. This is not a very serious problem since in the appendix we show that an integrable function is continuous except for a “negligible” set, so that $\| f \| = 0$ implies that $f$ vanishes except on a set of “measure zero.” One can get around the dificulty that $f$ is not identically zero by adopting the convention that such functions are actually the zero function, since for the purpose of integration, $f$ behaves precisely like the zero function. 

A more essential dificulty is that the space $\mathcal { R }$ is not complete. One way to see this is to start with the function 

$$
f (\theta) = \left\{ \begin{array}{l l} 0 & \text { for } \theta = 0, \\ \log (1 / \theta) & \text { for } 0 <   \theta \leq 2 \pi . \end{array} \right.
$$

Since $f$ is not bounded, it does not belong to the space $\mathcal { R }$ . Moreover, the sequence of truncations $f _ { n }$ defined by 

$$
f _ {n} (\theta) = \left\{ \begin{array}{l l} 0 & \text { for } 0 \leq \theta \leq 1 / n, \\ f (\theta) & \text { for } 1 / n <   \theta \leq 2 \pi \end{array} \right.
$$

can easily be seen to form a Cauchy sequence in $\mathcal { R }$ (see Exercise 5). However, this sequence cannot converge to an element in $\mathcal { R }$ , since that limit, if it existed, would have to be $f ;$ for another example, see Exercise 7. 

This and more complicated examples motivate the search for the completion of $\mathcal { R }$ , the class of Riemann integrable functions on [0, 2π]. The construction and identification of this completion, the Lebesgue class $L ^ { 2 } ( [ 0 , 2 \pi ] )$ , represents an important turning point in the development of analysis (somewhat akin to the much earlier completion of the rationals, that is, the passage from $\mathbb { Q }$ to R). A further discussion of these fundamental ideas will be postponed until Book III, where we take up the Lebesgue theory of integration. 

We now turn to the proof of Theorem 1.1. 

## 1.2 Proof of mean-square convergence

Consider the space R of integrable functions on the circle with inner product 

$$
(f, g) = \frac {1}{2 \pi} \int_ {0} ^ {2 \pi} f (\theta) \overline {{g (\theta)}} d \theta
$$

## 1. Mean-square convergence of Fourier series

and norm $\| f \|$ defined by 

$$
\| f \| ^ {2} = (f, f) = \frac {1}{2 \pi} \int_ {0} ^ {2 \pi} | f (\theta) | ^ {2} d \theta .
$$

With this notation, we must prove that $\| f - S _ { N } ( f ) \| \to 0$ as N tends to infinity. 

For each integer $n$ , let $e _ { n } ( \theta ) = e ^ { i n \theta }$ , and observe that the family $\{ e _ { n } \} _ { n \in \mathbb { Z } }$ is orthonormal; that is, 

$$
(e _ {n}, e _ {m}) = \left\{ \begin{array}{l l} 1 & \text { if } n = m \\ 0 & \text { if } n \neq m. \end{array} \right.
$$

Let $f$ be an integrable function on the circle, and let $a _ { n }$ denote its Fourier coeficients. An important observation is that these Fourier coeficients are represented by inner products of f with the elements in the orthonormal set $\{ e _ { n } \} _ { n \in \mathbb { Z } } \colon$ 

$$
(f, e _ {n}) = \frac {1}{2 \pi} \int_ {0} ^ {2 \pi} f (\theta) e ^ {- i n \theta} d \theta = a _ {n}.
$$

In particular, $\begin{array} { r } { S _ { N } ( f ) = \sum _ { | n | \leq N } a _ { n } e _ { n } } \end{array}$ . Then the orthonormal property of the family $\{ e _ { n } \}$ and the fact that $a _ { n } = \left( f , e _ { n } \right)$ imply that the diference $\begin{array} { r } { f - \sum _ { | n | \leq N } a _ { n } e _ { n } } \end{array}$ is orthogonal to $e _ { n }$ for all $| n | \leq N$ . Therefore, we must have 

$$
\left(f - \sum_ {| n | \leq N} a _ {n} e _ {n}\right) \perp \sum_ {| n | \leq N} b _ {n} e _ {n}\tag{2}
$$

for any complex numbers $b _ { n }$ . We draw two conclusions from this fact. First, we can apply the Pythagorean theorem to the decomposition 

$$
f = f - \sum_ {| n | \leq N} a _ {n} e _ {n} + \sum_ {| n | \leq N} a _ {n} e _ {n},
$$

where we now choose $b _ { n } = a _ { n } ,$ , to obtain 

$$
\| f \| ^ {2} = \| f - \sum_ {| n | \leq N} a _ {n} e _ {n} \| ^ {2} + \| \sum_ {| n | \leq N} a _ {n} e _ {n} \| ^ {2}.
$$

Since the orthonormal property of the family $\{ e _ { n } \} _ { n \in \mathbb { Z } }$ implies that 

$$
\| \sum_ {| n | \leq N} a _ {n} e _ {n} \| ^ {2} = \sum_ {| n | \leq N} | a _ {n} | ^ {2},
$$

we deduce that 

$$
\| f \| ^ {2} = \| f - S _ {N} (f) \| ^ {2} + \sum_ {| n | \leq N} | a _ {n} | ^ {2}.\tag{3}
$$

The second conclusion we may draw from (2) is the following simple lemma. 

Lemma 1.2 (Best approximation) $I f f$ is integrable on the circle with Fourier coeficients $a _ { n } ,$ , then 

$$
\| f - S _ {N} (f) \| \leq \| f - \sum_ {| n | \leq N} c _ {n} e _ {n} \|
$$

for any complex numbers $c _ { n }$ . Moreover, equality holds precisely when $c _ { n } = a _ { n }$ for all $| n | \leq N$ 

Proof. This follows immediately by applying the Pythagorean theorem to 

$$
f - \sum_ {| n | \leq N} c _ {n} e _ {n} = f - S _ {N} (f) + \sum_ {| n | \leq N} b _ {n} e _ {n},
$$

where $b _ { n } = a _ { n } - c _ { n }$ 

This lemma has a clear geometric interpretation. It says that the trigonometric polynomial of degree at most N which is closest to $f$ in the norm $\| \cdot \|$ is the partial sum $S _ { N } ( f )$ . This geometric property of the partial sums is depicted in Figure 1, where the orthogonal projection of $f$ in the plane spanned by $\left\{ e _ { - N } , \ldots , e _ { 0 } , \ldots , e _ { N } \right\}$ is simply $S _ { N } ( f )$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/d7498d01a5bfb7202d1d7abc6843ba88d709b1aaece6415048d43406bca22a2d.jpg)



Figure 1. The best approximation lemma


We can now give the proof that $\| S _ { N } ( f ) - f \| \to 0$ using the best approximation lemma, as well as the important fact that trigonometric polynomials are dense in the space of continuous functions on the circle. 

## 1. Mean-square convergence of Fourier series

Suppose that $f$ is continuous on the circle. Then, given $\epsilon > 0$ , there exists (by Corollary 5.4 in Chapter 2) a trigonometric polynomial $P ,$ say of degree M, such that 

$$
| f (\theta) - P (\theta) | <   \epsilon \quad \text { for   all } \theta .
$$

In particular, taking squares and integrating this inequality yields $\| f - P \| < \epsilon$ , and by the best approximation lemma we conclude that 

$$
\| f - S _ {N} (f) \| <   \epsilon \quad \text { whenever } N \geq M.
$$

This proves Theorem 1.1 when $f$ is continuous. 

If $f$ is merely integrable, we can no longer approximate f uniformly by trigonometric polynomials. Instead, we apply the approximation Lemma 3.2 in Chapter 2 and choose a continuous function g on the circle which satisfies 

$$
\sup _ {\theta \in [ 0, 2 \pi ]} | g (\theta) | \leq \sup _ {\theta \in [ 0, 2 \pi ]} | f (\theta) | = B,
$$

and 

$$
\int_ {0} ^ {2 \pi} | f (\theta) - g (\theta) | d \theta <   \epsilon^ {2}.
$$

Then we get 

$$
\begin{array}{l} \| f - g \| ^ {2} = \frac {1}{2 \pi} \int_ {0} ^ {2 \pi} | f (\theta) - g (\theta) | ^ {2} d \theta \\ \qquad = \frac {1}{2 \pi} \int_ {0} ^ {2 \pi} | f (\theta) - g (\theta) | | f (\theta) - g (\theta) | d \theta \\ \qquad \leq \frac {2 B}{2 \pi} \int_ {0} ^ {2 \pi} | f (\theta) - g (\theta) | d \theta \\ \qquad \leq C \epsilon^ {2}. \end{array}
$$

Now we may approximate g by a trigonometric polynomial $P$ so that $\| g - P \| < \epsilon$ . Then $\| f - P \| < C ^ { \prime } \epsilon$ , and we may again conclude by applying the best approximation lemma. This completes the proof that the partial sums of the Fourier series of $f$ converge to $f$ in the mean square norm k · k. 

Note that this result and the relation (3) imply that if $a _ { n }$ is the $n ^ { \mathrm { t h } }$ Fourier coeficient of an integrable function $f ,$ then the series $\scriptstyle \sum _ { n = - \infty } ^ { \infty } | a _ { n } | ^ { 2 }$ converges, and in fact we have Parseval’s identity 

$$
\sum_ {n = - \infty} ^ {\infty} | a _ {n} | ^ {2} = \| f \| ^ {2}.
$$

This identity provides an important connection between the norms in the two vector spaces $\ell ^ { 2 } ( \mathbb { Z } )$ and R. 

We now summarize the results of this section. 

Theorem 1.3 Let f be an integrable function on the circle with $\textstyle f \sim \sum _ { n = - \infty } ^ { \infty } a _ { n } e ^ { i n \theta }$ . Then we have: 

(i) Mean-square convergence of the Fourier series 

$$
\frac {1}{2 \pi} \int_ {0} ^ {2 \pi} | f (\theta) - S _ {N} (f) (\theta) | ^ {2} d \theta \to 0 \quad a s N \to \infty .
$$

(ii) Parseval’s identity 

$$
\sum_ {n = - \infty} ^ {\infty} | a _ {n} | ^ {2} = \frac {1}{2 \pi} \int_ {0} ^ {2 \pi} | f (\theta) | ^ {2} d \theta .
$$

Remark 1. If $\{ e _ { n } \}$ is any orthonormal family of functions on the circle, and $a _ { n } = \left( f , e _ { n } \right)$ , then we may deduce from the relation (3) that 

$$
\sum_ {n = - \infty} ^ {\infty} | a _ {n} | ^ {2} \leq \| f \| ^ {2}.
$$

This is known as Bessel’s inequality. Equality holds (as in Parseval’s identity) precisely when the family $\{ e _ { n } \}$ is also a “basis,” in the sense that $\begin{array} { r } { \| \sum _ { | n | \leq N } a _ { n } e _ { n } - f \| \to 0 } \end{array}$ as $N \to \infty$ 

Remark 2. We may associate to every integrable function the sequence $\left\{ a _ { n } \right\}$ formed by its Fourier coeficients. Parseval’s identity guarantees that $\{ a _ { n } \} \in \ell ^ { 2 } ( \mathbb { Z } )$ . Since $\ell ^ { 2 } ( \mathbb { Z } )$ is a Hilbert space, the failure of R to be complete, discussed earlier, may be understood as follows: there exist sequences $\{ a _ { n } \} _ { n \in \mathbb { Z } }$ such that $\textstyle \sum _ { n \in \mathbb { Z } } | a _ { n } | ^ { 2 } < \infty$ , yet no Riemann integrable function F has $n ^ { \mathrm { t h } }$ Fourier coeficient equal to $a _ { n }$ for all n. An example is given in Exercise 6. 

Since the terms of a converging series tend to 0, we deduce from Parseval’s identity or Bessel’s inequality the following result. 

Theorem 1.4 (Riemann-Lebesgue lemma) If f is integrable on the circle, then ${ \hat { f } } ( n ) \to 0 \ a s \ | n | \to \infty$ 

An equivalent reformulation of this proposition is that if f is integrable on [0, 2π], then 

$$
\int_ {0} ^ {2 \pi} f (\theta) \sin (N \theta) d \theta \rightarrow 0 \quad \mathrm{as} N \rightarrow \infty
$$

2. Return to pointwise convergence 

and 

$$
\int_ {0} ^ {2 \pi} f (\theta) \cos (N \theta) d \theta \rightarrow 0 \quad \mathrm{as} N \rightarrow \infty .
$$

To conclude this section, we give a more general version of the Parseval identity which we will use in the next chapter. 

Lemma 1.5 Suppose F and G are integrable on the circle with 

$$
F \sim \sum a _ {n} e ^ {i n \theta} \quad a n d \quad G \sim \sum b _ {n} e ^ {i n \theta}.
$$

Then 

$$
\frac {1}{2 \pi} \int_ {0} ^ {2 \pi} F (\theta) \overline {{G (\theta)}} d \theta = \sum_ {n = - \infty} ^ {\infty} a _ {n} \overline {{b _ {n}}}.
$$

Recall from the discussion in Example 1 that the series $\scriptstyle \sum _ { n = - \infty } ^ { \infty } a _ { n } { \overline { { b _ { n } } } }$ converges absolutely. 

Proof. The proof follows from Parseval’s identity and the fact that 

$$
(F, G) = \frac {1}{4} \left[ \| F + G \| ^ {2} - \| F - G \| ^ {2} + i \left(\| F + i G \| ^ {2} - \| F - i G \| ^ {2}\right) \right]
$$

which holds in every Hermitian inner product space. The verification of this fact is left to the reader. 

## 2 Return to pointwise convergence

The mean-square convergence theorem does not provide further insight into the problem of pointwise convergence. Indeed, Theorem 1.1 by itself does not guarantee that the Fourier series converges for any θ. Exercise 3 helps to explain this statement. However, if a function is diferentiable at a point $\theta _ { 0 }$ , then its Fourier series converges at $\theta _ { 0 }$ . After proving this result, we give an example of a continuous function with diverging Fourier series at one point. These phenomena are indicative of the intricate nature of the problem of pointwise convergence in the theory of Fourier series. 

## 2.1 A local result

Theorem 2.1 Let f be an integrable function on the circle which is differentiable at a point $\theta _ { 0 }$ . Then $S _ { N } ( f ) ( \theta _ { 0 } ) \to f ( \theta _ { 0 } )$ as N tends to infinity. 

Proof. Define 

$$
F (t) = \left\{ \begin{array}{l l} \frac {f (\theta_ {0} - t) - f (\theta_ {0})}{t} & \text { if } t \neq 0 \text { and } | t | <   \pi \\ - f ^ {\prime} (\theta_ {0}) & \text { if } t = 0. \end{array} \right.
$$

First, $F$ is bounded near 0 since $f$ is diferentiable there. Second, for all small δ the function $F$ is integrable on $[ - \pi , - \delta ] \cup [ \delta , \pi ]$ because $f$ has this property and $| t | > \delta$ there. As a consequence of Proposition 1.4 in the appendix, the function F is integrable on all of $[ - \pi , \pi ]$ . We know that $S _ { N } ( f ) ( \theta _ { 0 } ) = ( f * D _ { N } ) ( \theta _ { 0 } )$ , where $D _ { N }$ is the Dirichlet kernel. Since $\begin{array} { r } { { \frac { 1 } { 2 \pi } } \int D _ { N } = 1 } \end{array}$ , we find that 

$$
\begin{array}{l} S _ {N} (f) (\theta_ {0}) - f (\theta_ {0}) = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (\theta_ {0} - t) D _ {N} (t) d t - f (\theta_ {0}) \\ \qquad = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} [ f (\theta_ {0} - t) - f (\theta_ {0}) ] D _ {N} (t) d t \\ \qquad = \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} F (t) t D _ {N} (t) d t. \end{array}
$$

We recall that 

$$
t D _ {N} (t) = \frac {t}{\sin (t / 2)} \sin ((N + 1 / 2) t),
$$

where the quotient $\frac { t } { \sin ( { t } / { 2 } ) }$ is continuous in the interval $[ - \pi , \pi ]$ . Since we can write 

$$
\sin ((N + 1 / 2) t) = \sin (N t) \cos (t / 2) + \cos (N t) \sin (t / 2),
$$

we can apply the Riemann-Lebesgue lemma to the Riemann integrable functions $F ( t ) t \cos ( t / 2 ) / \sin ( t / 2 )$ and $F ( t ) t$ to finish the proof of the theorem. 

Observe that the conclusion of the theorem still holds if we only assume that $f$ satisfies a Lipschitz condition at $\theta _ { 0 } ;$ that is, 

$$
| f (\theta) - f \left(\theta_ {0}\right) | \leq M | \theta - \theta_ {0} |
$$

for some $M \geq 0$ and all θ. This is the same as saying that f satisfies a H¨older condition of order $\alpha = 1$ 

A striking consequence of this theorem is the localization principle of Riemann. This result states that the convergence of $S _ { N } ( f ) ( \theta _ { 0 } )$ depends only on the behavior of $f$ near $\theta _ { 0 }$ . This is not clear at first, since forming the Fourier series requires integrating $f$ over the whole circle. 

## 2. Return to pointwise convergence

Theorem 2.2 Suppose f and g are two integrable functions defined on the circle, and for some $\theta _ { 0 }$ there exists an open interval I containing $\theta _ { 0 }$ such that 

$$
f (\theta) = g (\theta) \quad f o r a l l \theta \in I.
$$

Then $S _ { N } ( f ) ( \theta _ { 0 } ) - S _ { N } ( g ) ( \theta _ { 0 } ) \to 0$ as N tends to infinity. 

Proof. The function $f - g$ is 0 in I, so it is diferentiable at $\theta _ { 0 }$ , and we may apply the previous theorem to conclude the proof. 

## 2.2 A continuous function with diverging Fourier series

We now turn our attention to an example of a continuous periodic function whose Fourier series diverges at a point. Thus, Theorem 2.1 fails if the diferentiability assumption is replaced by the weaker assumption of continuity. Our counter-example shows that this hypothesis which had appeared plausible, is in fact false; moreover, its construction also illuminates an important principle of the theory. 

The principle that is involved here will be referred to as “symmetrybreaking.”<sup>1</sup> The symmetry that we have in mind is the symmetry between the frequencies $e ^ { i n \theta }$ and $e ^ { - i n \theta }$ which appear in the Fourier expansion of a function. For example, the partial sum operator $S _ { N }$ is defined in a way that reflects this symmetry. Also, the Dirichlet, Fej`er, and Poisson kernels are symmetric in this sense. When we break the symmetry, that is, when we split the Fourier series $\scriptstyle \sum _ { n = - \infty } ^ { \infty } a _ { n } e ^ { i n \theta }$ into the two pieces $\textstyle \sum _ { n \geq 0 } a _ { n } e ^ { i n \theta }$ and $\textstyle \sum _ { n < 0 } a _ { n } e ^ { i n \theta }$ , we introduce new and far-reaching phenomena. 

We give a simple example. Start with the sawtooth function f which is odd in θ and which equals $i ( \pi - \theta )$ when $0 < \theta < \pi$ . Then, by Exercise 8 in Chapter 2, we know that 

$$
f (\theta) \sim \sum_ {n \neq 0} \frac {e ^ {i n \theta}}{n}.\tag{4}
$$

Consider now the result of breaking the symmetry and the resulting series 

$$
\sum_ {n = - \infty} ^ {n = - 1} \frac {e ^ {i n \theta}}{n}.
$$

Then, unlike (4), the above is no longer the Fourier series of a Riemann integrable function. Indeed, suppose it were the Fourier series of an integrable function, say ${ \tilde { f } } ,$ where in particular $\tilde { f }$ is bounded. Using the Abel means, we then have 

$$
| A _ {r} (\tilde {f}) (0) | = \sum_ {n = 1} ^ {\infty} \frac {r ^ {n}}{n},
$$

which tends to infinity as r tends to 1, because $\textstyle \sum 1 / n$ diverges. This gives the desired contradiction since 

$$
| A _ {r} (\tilde {f}) (0) | \leq \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} | \tilde {f} (\theta) | P _ {r} (\theta) d \theta \leq \sup _ {\theta} | \tilde {f} (\theta) |,
$$

where $P _ { r } ( \theta )$ denotes the Poisson kernel discussed in the previous chapter. 

The sawtooth function is the object from which we will fashion our counter-example. We proceed as follows. For each $N \geq 1$ we define the following two functions on $[ - \pi , \pi ]$ 2 

$$
f _ {N} (\theta) = \sum_ {1 \leq | n | \leq N} \frac {e ^ {i n \theta}}{n} \quad \text {and} \quad \tilde {f} _ {N} (\theta) = \sum_ {- N \leq n \leq - 1} \frac {e ^ {i n \theta}}{n}.
$$

We contend that: 

(i) $| \tilde { f } _ { N } ( 0 ) | \geq c \log N .$ 

(ii) $f _ { N } ( \theta )$ is uniformly bounded in N and θ. 

The first statement is a consequence of the fact that $\textstyle \sum _ { n = 1 } ^ { N } 1 / n \geq$ log N, which is easily established (see also Figure 2): 

$$
\sum_ {n = 1} ^ {N} \frac {1}{n} \geq \sum_ {n = 1} ^ {N - 1} \int_ {n} ^ {n + 1} \frac {d x}{x} = \int_ {1} ^ {N} \frac {d x}{x} = \log N.
$$

To prove (ii), we argue in the same spirit as in the proof of Tauber’s theorem, which says that if the series $\sum c _ { n }$ is Abel summable to s and $c _ { n } = o ( 1 / n )$ , then $\sum c _ { n }$ actually converges to s (see Exercise 14 in Chapter 2). In fact, the proof of Tauber’s theorem is quite similar to that of the lemma below. 

Lemma 2.3 Suppose that the Abel means $\textstyle A _ { r } = \sum _ { n = 1 } ^ { \infty } r ^ { n } c _ { n }$ of the series $\sum _ { n = 1 } ^ { \infty } c _ { n }$ are bounded as r tends to 1 (with $r < 1 ) . \ I f c _ { n } = O ( 1 / n )$ , then the partial sums $\begin{array} { r } { S _ { N } = \sum _ { n = 1 } ^ { N } c _ { n } } \end{array}$ are bounded. 

2. Return to pointwise convergence 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/87bf58100b000f596c60e9118244c687d8a007bd1594f27a7d900dbc50b1f5fe.jpg)



Figure 2. Comparing a sum with an integral


Proof. Let $r = 1 - 1 / N$ and choose M so that $n | c _ { n } | \leq M$ . We estimate the diference 

$$
S _ {N} - A _ {r} = \sum_ {n = 1} ^ {N} (c _ {n} - r ^ {n} c _ {n}) - \sum_ {n = N + 1} ^ {\infty} r ^ {n} c _ {n}
$$

as follows: 

$$
\begin{array}{l} | S _ {N} - A _ {r} | \leq \sum_ {n = 1} ^ {N} | c _ {n} | (1 - r ^ {n}) + \sum_ {n = N + 1} ^ {\infty} r ^ {n} | c _ {n} | \\ \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \\ \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qend{array}
$$

where we have used the simple observation that 

$$
1 - r ^ {n} = (1 - r) \left(1 + r + \dots + r ^ {n - 1}\right) \leq n (1 - r).
$$

So we see that if M satisfies both $| A _ { r } | \leq M$ and $n | c _ { n } | \leq M .$ , then $| S _ { N } | \leq$ 3M. 

We apply the lemma to the series 

$$
\sum_ {n \neq 0} \frac {e ^ {i n \theta}}{n},
$$

which is the Fourier series of the sawtooth function f used above. Here $c _ { n } = e ^ { i n \theta } / n + e ^ { - i n \theta } / ( - n )$ for $n \neq 0 .$ , so clearly $c _ { n } = O ( 1 / | n | )$ . Finally, the Abel means of this series are $A _ { r } ( f ) ( \theta ) = ( f * P _ { r } ) ( \theta )$ . But f is bounded and $P _ { r }$ is a good kernel, so $S _ { N } ( f ) ( \theta )$ is uniformly bounded in N and θ, as was to be shown. 

We now come to the heart of the matter. Notice that $f _ { N }$ and $\tilde { f } _ { N }$ are trigonometric polynomials of degree N (that is, they have non-zero Fourier coeficients only when $| n | \leq N )$ . From these, we form trigonometric polynomials $P _ { N }$ and $\ddot { P } _ { N }$ , now of degrees 3N and $2 N - 1$ , by displacing the frequencies of $f _ { N }$ and $\tilde { f } _ { N }$ by 2N units. In other words, we define $P _ { N } ( \theta ) = e ^ { i ( 2 N ) \theta } f _ { N } ( \theta )$ and $\overset { \sim } { P } _ { N } ( \theta ) = e ^ { i ( 2 N ) \theta } \overset { \sim } { f } _ { N } ( \theta )$ . So while $f _ { N }$ has non-vanishing Fourier coeficients when $0 < | n | \leq N$ , now the coefficients of $P _ { N }$ are non-vanishing for $N \leq n \leq 3 N , n \neq 2 N$ . Moreover, while $n = 0$ is the center of symmetry of $f _ { N }$ , now $n = 2 N$ is the center of symmetry of $P _ { N }$ . We next consider the partial sums $S _ { M }$ 

Lemma 2.4 

$$
S _ {M} (P _ {N}) = \left\{ \begin{array}{l l} P _ {N} & \text { if } M \geq 3 N, \\ \tilde {P} _ {N} & \text { if } M = 2 N, \\ 0 & \text { if } M <   N. \end{array} \right.
$$

This is clear from what has been said above and from Figure 3. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/167ca7359c6c1d6ab3c149c5c36c1d6e111028ce1a7e012db4e5df6fb19c31a0.jpg)



Figure 3. Breaking symmetry in Lemma 2.4


The efect is that when $M = 2 N$ , the operator $S _ { M }$ breaks the symmetry of $P _ { N }$ , but in the other cases covered in the lemma, the action of $S _ { M }$ 

## 3. Exercises

is relatively benign, since then the outcome is either $P _ { N }$ or 0. 

Finally, we need to find a convergent series of positive terms $\sum \alpha _ { k }$ and a sequence of integers $\{ N _ { k } \}$ which increases rapidly enough so that: 

(i) $N _ { k + 1 } > 3 N _ { k } .$ 

(ii) $\alpha _ { k }$ log $N _ { k } \to \infty$ as $k \to \infty$ 

We choose (for example) $\alpha _ { k } = 1 / k ^ { 2 }$ and $N _ { k } = 3 ^ { 2 ^ { k } }$ which are easily seen to satisfy the above criteria. 

Finally, we can write down our desired function. It is 

$$
f (\theta) = \sum_ {k = 1} ^ {\infty} \alpha_ {k} P _ {N _ {k}} (\theta).
$$

Due to the uniform boundedness of the $P _ { N }$ (recall that $| P _ { N } ( \theta ) | = | f _ { N } ( \theta ) | )$ the series above converges uniformly to a continuous periodic function. However, by our lemma we get 

$$
| S _ {2 N _ {m}} (f) (0) | \geq c \alpha_ {m} \log N _ {m} + O (1) \to \infty \quad \text { as } m \to \infty .
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/f8fb85bd7541aae80551f88ebfab5e64b700fa989480a9aa41b37e327af311fc.jpg)



Figure 4. Symmetry broken in the middle interval $\left( N _ { k } , 3 N _ { k } \right)$


Indeed, the terms that correspond to $N _ { k }$ with $k < m$ or $k > m$ contribute $O ( 1 )$ or 0, respectively (because the $P _ { N } \mathrm { { ' s } }$ are uniformly bounded), while the term that corresponds to $N _ { m }$ is in absolute value greater than $c \alpha _ { m }$ log $N _ { m }$ because $| \tilde { P } _ { N } ( \boldsymbol { \bar { \theta } } ) | = | \tilde { f } _ { N } ( \boldsymbol { \theta } ) | \geq c \log N$ . So the partial sums of the Fourier series of $f$ at 0 are not bounded, and we are done since this proves the divergence of the Fourier series of $f$ at $\theta = 0$ . To produce a function whose series diverges at any other preassigned $\theta = \theta _ { 0 }$ , it sufices to consider the function $f ( \theta - \theta _ { 0 } )$ 

## 3 Exercises

1. Show that the first two examples of inner product spaces, namely $\mathbb { R } ^ { d }$ and $\mathbb { C } ^ { d }$ are complete. 

[Hint: Every Cauchy sequence in R has a limit.] 

2. Prove that the vector space $\ell ^ { 2 } ( \mathbb { Z } )$ is complete. 

[Hint: Suppose $A _ { k } = \{ a _ { k , n } \} _ { n \in \mathbb { Z } }$ with $k = 1 , 2 , \dots$ . is a Cauchy sequence. Show that for each $n , \{ a _ { k , n } \} _ { k = 1 } ^ { \infty }$ is a Cauchy sequence of complex numbers, therefore it converges to a limit, say $b _ { n }$ . By taking partial sums of $\| A _ { k } - A _ { k ^ { \prime } } \|$ and letting $k ^ { \prime } \to \infty$ , show that $\| A _ { k } - B \| \to 0$ as $k  \infty ,$ where $B = ( \dots , b _ { - 1 } , b _ { 0 } , b _ { 1 } , \dots )$ Finally, prove that $B \in \ell ^ { 2 } ( \mathbb { Z } ) . ]$ 

3. Construct a sequence of integrable functions $\left\{ f _ { k } \right\}$ on $[ 0 , 2 \pi ]$ such that 

$$
\lim _ {k \to \infty} \frac {1}{2 \pi} \int_ {0} ^ {2 \pi} | f _ {k} (\theta) | ^ {2} d \theta = 0
$$

but lim $1 _ { k \to \infty } f _ { k } ( \theta )$ fails to exist for any θ. 

[Hint: Choose a sequence of intervals $I _ { k } \subset [ 0 , 2 \pi ]$ whose lengths tend to $0 ,$ and so that each point belongs to infinitely many of them; then let $f _ { k } = \chi _ { I _ { k } } . ]$ 

4. Recall the vector space $\mathcal { R }$ of integrable functions, with its inner product and norm 

$$
\| f \| = \left(\frac {1}{2 \pi} \int_ {0} ^ {2 \pi} | f (x) | ^ {2} d x\right) ^ {1 / 2}.
$$

(a) Show that there exist non-zero integrable functions $f$ for which $\| f \| = 0$ 

(b) However, show that if $f \in \mathcal R$ with $\| f \| = 0$ , then $f ( x ) = 0$ whenever $f$ is continuous at x. 

(c) Conversely, show that if $f \in \mathcal R$ vanishes at all of its points of continuity, then $\| f \| = 0$ 

5. Let 

$$
f (\theta) = \left\{ \begin{array}{l l} 0 & \text {for} \theta = 0 \\ \log (1 / \theta) & \text {for} 0 <   \theta \leq 2 \pi , \end{array} \right.
$$

and define a sequence of functions in $\mathcal { R }$ by 

$$
f _ {n} (\theta) = \left\{ \begin{array}{l l} 0 & \text { for } 0 \leq \theta \leq 1 / n \\ f (\theta) & \text { for } 1 / n <   \theta \leq 2 \pi . \end{array} \right.
$$

Prove that $\{ f _ { n } \} _ { n = 1 } ^ { \infty }$ is a Cauchy sequence in $\mathcal { R }$ . However, $f$ does not belong to $\mathcal { R }$ 

## 3. Exercises

[Hint: Show that $\textstyle \int _ { a } ^ { b } ( \log \theta ) ^ { 2 } d \theta \to 0 { \mathrm { ~ i f ~ } } 0 < a < b$ and $b  0 .$ , by using the fact that the derivative of $\dot { \theta } ( \log \theta ) ^ { 2 } - 2 \theta$ θ log $\theta + 2 \theta$ is equal to $( \log \theta ) ^ { 2 } . ]$ 

6. Consider the sequence $\{ a _ { k } \} _ { k = - \infty } ^ { \infty }$ defined by 

$$
a _ {k} = \left\{ \begin{array}{c l} 1 / k & \text { if } k \geq 1 \\ 0 & \text { if } k \leq 0. \end{array} \right.
$$

Note that $\{ a _ { k } \} \in \ell ^ { 2 } ( \mathbb { Z } )$ , but that no Riemann integrable function has $k ^ { \mathrm { t h } }$ Fourier coeficient equal to $a _ { k }$ for all k. 

7. Show that the trigonometric series 

$$
\sum_ {n \geq 2} \frac {1}{\log n} \sin n x
$$

converges for every x, yet it is not the Fourier series of a Riemann integrable function. 

The same is true for $\sum { \frac { \sin n x } { n ^ { \alpha } } }$ for $0 < \alpha < 1$ , but the case $1 / 2 < \alpha < 1$ is more dificult. See Problem 1. 

8. Exercise 6 in Chapter 2 dealt with the sums 

$$
\sum_ {n \text {odd} \geq 1} \frac {1}{n ^ {2}} \quad \text {and} \quad \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {2}}.
$$

Similar sums can be derived using the methods of this chapter. 

(a) Let $f$ be the function defined on $[ - \pi , \pi ]$ by $f ( \theta ) = | \theta |$ . Use Parseval’s identity to find the sums of the following two series: 

$$
\sum_ {n = 0} ^ {\infty} \frac {1}{(2 n + 1) ^ {4}} \quad \text { and } \quad \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {4}}.
$$

In fact, they are $\pi ^ { 4 } / 9 6$ and $\pi ^ { 4 } / 9 0$ , respectively. 

(b) Consider the 2π-periodic odd function defined on $[ 0 , \pi ]$ by $f ( \theta ) = \theta ( \pi - \theta )$ Show that 

$$
\sum_ {n = 0} ^ {\infty} \frac {1}{(2 n + 1) ^ {6}} = \frac {\pi^ {6}}{9 6 0} \quad \text { and } \quad \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {6}} = \frac {\pi^ {6}}{9 4 5}.
$$

Remark. The general expression when k is even for $\textstyle \sum _ { n = 1 } ^ { \infty } 1 / n ^ { k }$ in terms of $\pi ^ { k }$ is given in Problem 4. However, finding a formula for the sum $\textstyle \sum _ { n = 1 } ^ { \infty } 1 / n ^ { 3 }$ , or more generally $\textstyle \sum _ { n = 1 } ^ { \infty } 1 / n ^ { k }$ with k odd, is a famous unresolved question. 

9. Show that for α not an integer, the Fourier series of 

$$
\frac {\pi}{\sin \pi \alpha} e ^ {i (\pi - x) \alpha}
$$

on [0, 2π] is given by 

$$
\sum_ {n = - \infty} ^ {\infty} \frac {e ^ {i n x}}{n + \alpha}.
$$

Apply Parseval’s formula to show that 

$$
\sum_ {n = - \infty} ^ {\infty} \frac {1}{(n + \alpha) ^ {2}} = \frac {\pi^ {2}}{(\sin \pi \alpha) ^ {2}}.
$$

10. Consider the example of a vibrating string which we analyzed in Chapter 1. The displacement $\boldsymbol { u } ( \boldsymbol { x } , t )$ of the string at time t satisfies the wave equation 

$$
\frac {1}{c ^ {2}} \frac {\partial^ {2} u}{\partial t ^ {2}} = \frac {\partial^ {2} u}{\partial x ^ {2}}, \quad c ^ {2} = \tau / \rho .
$$

The string is subject to the initial conditions 

$$
u (x, 0) = f (x) \quad \mathrm{and} \quad \frac {\partial u}{\partial t} (x, 0) = g (x),
$$

where we assume that $f \in C ^ { 1 }$ and g is continuous. We define the total energy of the string by 

$$
E (t) = \frac {1}{2} \rho \int_ {0} ^ {L} \left(\frac {\partial u}{\partial t}\right) ^ {2} d x + \frac {1}{2} \tau \int_ {0} ^ {L} \left(\frac {\partial u}{\partial x}\right) ^ {2} d x.
$$

The first term corresponds to the “kinetic energy” of the string (in analogy with $( 1 / 2 ) m v ^ { 2 }$ , the kinetic energy of a particle of mass m and velocity v), and the second term corresponds to its “potential energy.” 

Show that the total energy of the string is conserved, in the sense that $E ( t )$ is constant. Therefore, 

$$
E (t) = E (0) = \frac {1}{2} \rho \int_ {0} ^ {L} g (x) ^ {2} d x + \frac {1}{2} \tau \int_ {0} ^ {L} f ^ {\prime} (x) ^ {2} d x.
$$

3. Exercises 

(a) If $f$ is T-periodic, continuous, and piecewise $C ^ { 1 }$ with $\begin{array} { r } { \int _ { 0 } ^ { T } f ( t ) d t = 0 } \end{array}$ , show that 

$$
\int_ {0} ^ {T} | f (t) | ^ {2} d t \leq \frac {T ^ {2}}{4 \pi^ {2}} \int_ {0} ^ {T} | f ^ {\prime} (t) | ^ {2} d t,
$$

with equality if and only $\begin{array} { r l } { \mathrm { i f } } & { { } f ( t ) = A \sin ( 2 \pi t / T ) + B \cos ( 2 \pi t / T ) } \end{array}$ [Hint: Apply Parseval’s identity.] 

(b) If f is as above and $g$ is just $C ^ { 1 }$ and T-periodic, prove that 

$$
\left| \int_ {0} ^ {T} \overline {{f (t)}} g (t) d t \right| ^ {2} \leq \frac {T ^ {2}}{4 \pi^ {2}} \int_ {0} ^ {T} | f (t) | ^ {2} d t \int_ {0} ^ {T} | g ^ {\prime} (t) | ^ {2} d t.
$$

(c) For any compact interval $[ a , b ]$ and any continuously diferentiable function f with $f ( a ) = f ( b ) = 0$ , show that 

$$
\int_ {a} ^ {b} | f (t) | ^ {2} d t \leq \frac {(b - a) ^ {2}}{\pi^ {2}} \int_ {a} ^ {b} | f ^ {\prime} (t) | ^ {2} d t.
$$

Discuss the case of equality, and prove that the constant $( b - a ) ^ { 2 } / \pi ^ { 2 }$ cannot be improved. [Hint: Extend f to be odd with respect to a and periodic of period $T = 2 ( b ^ { \cdot } - a )$ so that its integral over an interval of length $T$ is 0. Apply part a) to get the inequality, and conclude that equality holds if and only if $\begin{array} { r } { f ( t ) = A \sin ( \pi \frac { t - a } { b - a } ) ] } \end{array}$ 

12. Prove that $\int _ { 0 } ^ { \infty } { \frac { \sin { x } } { x } } d x = { \frac { \pi } { 2 } } .$ 

[Hint: Start with the fact that the integral of $D _ { N } ( \theta )$ equals $2 \pi ,$ , and note that the diference $( 1 / \sin ( \theta / 2 ) ) - 2 / \theta$ is continuous on $[ - \pi , \pi ]$ . Apply the Riemann-Lebesgue lemma.] 

13. Suppose that f is periodic and of class $C ^ { k }$ . Show that 

$$
\hat {f} (n) = o (1 / | n | ^ {k}),
$$

that is, $| n | ^ { k } { \hat { f } } ( n )$ goes to 0 as $| n | \to \infty$ . This is an improvement over Exercise 10 in Chapter 2. 

[Hint: Use the Riemann-Lebesgue lemma.] 

14. Prove that the Fourier series of a continuously diferentiable function $f$ on the circle is absolutely convergent. 

[Hint: Use the Cauchy-Schwarz inequality and Parseval’s identity for $f ^ { \prime } . ]$ 

15. Let f be 2π-periodic and Riemann integrable on $[ - \pi , \pi ]$ 

(a) Show that 

$$
\hat {f} (n) = - \frac {1}{2 \pi} \int_ {- \pi} ^ {\pi} f (x + \pi / n) e ^ {- i n x} d x
$$

hence 

$$
\hat {f} (n) = \frac {1}{4 \pi} \int_ {- \pi} ^ {\pi} [ f (x) - f (x + \pi / n) ] e ^ {- i n x} d x.
$$

(b) Now assume that f satisfies a H¨older condition of order $\alpha ,$ namely 

$$
| f (x + h) - f (x) | \leq C | h | ^ {\alpha}
$$

for some $0 < \alpha \leq 1$ , some $C > 0$ , and all $x , h$ . Use part a) to show that 

$$
\hat {f} (n) = O (1 / | n | ^ {\alpha}).
$$

(c) Prove that the above result cannot be improved by showing that the function 

$$
f (x) = \sum_ {k = 0} ^ {\infty} 2 ^ {- k \alpha} e ^ {i 2 ^ {k} x},
$$

where $0 < \alpha < 1$ , satisfies 

$$
| f (x + h) - f (x) | \leq C | h | ^ {\alpha},
$$

and $\hat { f } ( N ) = 1 / N ^ { \alpha }$ whenever $N = 2 ^ { k }$ 

[Hint: For (c), break up the sum as follows $\begin{array} { r } { f ( x + h ) - f ( x ) = \sum _ { 2 ^ { k } \leq 1 / | h | } + } \end{array}$ $\sum 2 ^ { k } > 1 / \vert h \vert ^ { \prime }$ . To estimate the first sum use the fact that $| 1 - e ^ { i \theta } | \leq | \theta |$ whenever θ is small. To estimate the second sum, use the obvious inequality $| e ^ { i x } - e ^ { i y } | \leq 2 . ]$ 

16. Let f be a 2π-periodic function which satisfies a Lipschitz condition with constant $K ;$ that is, 

$$
| f (x) - f (y) | \leq K | x - y | \quad \text {   for   all   } x, y.
$$

This is simply the H¨older condition with $\alpha = 1$ , so by the previous exercise, we see that ${ \hat { f } } ( n ) = O ( 1 / | n | )$ . Since the harmonic series $\textstyle \sum 1 / n$ diverges, we cannot say anything (yet) about the absolute convergence of the Fourier series of $f .$ The outline below actually proves that the Fourier series of $f$ converges absolutely and uniformly. 

## 3. Exercises

(a) For every positive h we define $g _ { h } ( x ) = f ( x + h ) - f ( x - h )$ . Prove that 

$$
\frac {1}{2 \pi} \int_ {0} ^ {2 \pi} | g _ {h} (x) | ^ {2} d x = \sum_ {n = - \infty} ^ {\infty} 4 | \sin n h | ^ {2} | \hat {f} (n) | ^ {2},
$$

and show that 

$$
\sum_ {n = - \infty} ^ {\infty} | \sin n h | ^ {2} | \hat {f} (n) | ^ {2} \leq K ^ {2} h ^ {2}.
$$

(b) Let $p$ be a positive integer. By choosing $h = \pi / 2 ^ { p + 1 }$ , show that 

$$
\sum_ {2 ^ {p - 1} <   | n | \leq 2 ^ {p}} | \hat {f} (n) | ^ {2} \leq \frac {K ^ {2} \pi^ {2}}{2 ^ {2 p + 1}}.
$$

(c) Estimate $\sum _ { 2 ^ { p - 1 } < | n | \leq 2 ^ { p } } | { \hat { f } } ( n ) |$ , and conclude that the Fourier series of $f$ converges absolutely, hence uniformly. [Hint: Use the Cauchy-Schwarz inequality to estimate the sum.] 

(d) In fact, modify the argument slightly to prove Bernstein’s theorem: If f satisfies a H¨older condition of order $\alpha > 1 / 2$ , then the Fourier series of $f$ converges absolutely. 

17. If f is a bounded monotonic function on $[ - \pi , \pi ]$ , then 

$$
\hat {f} (n) = O (1 / | n |).
$$

[Hint: One may assume that $f$ is increasing, and say $| f | \leq M$ . First check that the Fourier coeficients of the characteristic function of $[ a , b ]$ satisfy $O ( 1 / | n | )$ Now show that a sum of the form 

$$
\sum_ {k = 1} ^ {N} \alpha_ {k} \chi_ {[ a _ {k}, a _ {k + 1} ]} (x)
$$

with $- \pi = a _ { 1 } < a _ { 2 } < \cdot \cdot \cdot < a _ { N } < a _ { N + 1 } = \pi$ and $- M \leq \alpha _ { 1 } \leq \cdot \cdot \cdot \leq \alpha _ { N } \leq M$ has Fourier coeficients that are $O ( 1 / | n | )$ uniformly in N. Summing by parts one gets a telescopic sum $\sum ( \alpha _ { k + 1 } - \alpha _ { k } )$ which can be bounded by 2M. Now approximate $f$ by functions of the above type.] 

18. Here are a few things we have learned about the decay of Fourier coeficients: 

(a) if f is of class $C ^ { k }$ , then ${ \hat { f } } ( n ) = o ( 1 / | n | ^ { k } )$ ; 

(b) if $f$ is Lipschitz, then ${ \hat { f } } ( n ) = O ( 1 / | n | )$ ; 

(c) if f is monotonic, then ${ \hat { f } } ( n ) = O ( 1 / | n | ) ;$ 

(d) if f is satisfies a H¨older condition with exponent α where $0 < \alpha < 1$ , then ${ \hat { f } } ( n ) = O ( 1 / | n | ^ { \alpha } )$ ; 

(e) if f is merely Riemann integrable, then $\sum | { \hat { f } } ( n ) | ^ { 2 } < \infty$ and therefore ${ \hat { f } } ( n ) = o ( 1 )$ 

Nevertheless, show that the Fourier coeficients of a continuous function can tend to 0 arbitrarily slowly by proving that for every sequence of nonnegative real numbers $\left\{ \epsilon _ { n } \right\}$ converging to 0, there exists a continuous function $f$ such that $| { \hat { f } } ( n ) | \geq \epsilon _ { n }$ for infinitely many values of n. 

[Hint: Choose a subsequence $\left\{ \epsilon _ { n _ { k } } \right\}$ so that $\textstyle \sum _ { k } \epsilon _ { n _ { k } } < \infty . ]$ 

19. Give another proof that the sum $\sum _ { 0 < | n | \leq N } e ^ { i n x } / n$ is uniformly bounded in N and $x \in [ - \pi , \pi ]$ by using the fact that 

$$
\frac {1}{2 i} \sum_ {0 <   | n | \leq N} \frac {e ^ {i n x}}{n} = \sum_ {n = 1} ^ {N} \frac {\sin n x}{n} = \frac {1}{2} \int_ {0} ^ {x} (D _ {N} (t) - 1) d t,
$$

where $D _ { N }$ is the Dirichlet kernel. Now use the fact that $\textstyle \int _ { 0 } ^ { \infty } { \frac { \sin { t } } { t } } d t < \infty$ which was proved in Exercise 12. 

20. Let $f ( x )$ denote the sawtooth function defined by $f ( x ) = ( \pi - x ) / 2$ on the interval $( 0 , 2 \pi )$ with $f ( 0 ) = 0$ and extended by periodicity to all of R. The Fourier series of $f$ is 

$$
f (x) \sim \frac {1}{2 i} \sum_ {| n | \neq 0} \frac {e ^ {i n x}}{n} = \sum_ {n = 1} ^ {\infty} \frac {\sin n x}{n},
$$

and f has a jump discontinuity at the origin with 

$$
f (0 ^ {+}) = \frac {\pi}{2}, \quad f (0 ^ {-}) = - \frac {\pi}{2}, \quad \text { and   hence } \quad f (0 ^ {+}) - f (0 ^ {-}) = \pi .
$$

Show that 

$$
\max _ {0 <   x \leq \pi / N} S _ {N} (f) (x) - \frac {\pi}{2} = \int_ {0} ^ {\pi} \frac {\sin t}{t} d t - \frac {\pi}{2},
$$

which is roughly 9% of the jump π. This result is a manifestation of Gibbs’s phenomenon which states that near a jump discontinuity, the Fourier series of a function overshoots (or undershoots) it by approximately 9% of the jump. 

[Hint: Use the expression for $S _ { N } ( f )$ given in Exercise 19.] 

4. Problems 

## 4 Problems

1. For each $0 < \alpha < 1$ the series 

$$
\sum_ {n = 1} ^ {\infty} \frac {\sin n x}{n ^ {\alpha}}
$$

converges for every x but is not the Fourier series of a Riemann integrable function. 

(a) If the conjugate Dirichlet kernel is defined by 

$$
\tilde {D} _ {N} (x) = \sum_ {| n | \leq N} \operatorname{sign} (x)   e ^ {i n x} \quad \text { where } \operatorname{sign} (x) = \left\{ \begin{array}{r l} 1 & \text { if } n > 0 \\ 0 & \text { if } n = 0 \\ - 1 & \text { if } n <   0, \end{array} \right.
$$

then show that 

$$
\tilde {D} _ {N} (x) = \frac {\cos (x / 2) - \cos ((N + 1 / 2) x)}{\sin (x / 2)},
$$

and 

$$
\int_ {- \pi} ^ {\pi} | \tilde {D} _ {N} (x) | d x \leq c \log N.
$$

(b) As a result, if f is Riemann integrable, then 

$$
(f * \tilde {D} _ {N}) (0) = O (\log N).
$$

(c) In the present case, this leads to 

$$
\sum_ {n = 1} ^ {N} \frac {1}{n ^ {\alpha}} = O (\log N),
$$

which is a contradiction. 

2. An important fact we have proved is that the family $\{ e ^ { i n x } \} _ { n \in \mathbb { Z } }$ is orthonormal in R and it is also complete, in the sense that the Fourier series of $f$ converges to $f$ in the norm. In this exercise, we consider another family possessing these same properties. 

On [−1, 1] define 

$$
L _ {n} (x) = \frac {d ^ {n}}{d x ^ {n}} (x ^ {2} - 1) ^ {n}, \qquad n = 0, 1, 2, \ldots .
$$

Then $L _ { n }$ is a polynomial of degree n which is called the $n ^ { \mathrm { t h } }$ Legendre polynomial. 

(a) Show that if f is indefinitely diferentiable on $[ - 1 , 1 ]$ , then 

$$
\int_ {- 1} ^ {1} L _ {n} (x) f (x) d x = (- 1) ^ {n} \int_ {- 1} ^ {1} (x ^ {2} - 1) ^ {n} f ^ {(n)} (x) d x.
$$

In particular, show that $L _ { n }$ is orthogonal to $x ^ { m }$ whenever $m < n$ . Hence $\{ L _ { n } \} _ { n = 0 } ^ { \infty }$ is an orthogonal family. 

(b) Show that 

$$
\left\| L _ {n} \right\| ^ {2} = \int_ {- 1} ^ {1} | L _ {n} (x) | ^ {2} d x = \frac {(n !) ^ {2} 2 ^ {2 n + 1}}{2 n + 1}.
$$

[Hint: First, note that $\begin{array} { r } { \| L _ { n } \| ^ { 2 } = ( - 1 ) ^ { n } ( 2 n ) ! \int _ { - 1 } ^ { 1 } ( x ^ { 2 } - 1 ) ^ { n } d x } \end{array}$ Write $( x ^ { 2 } - 1 ) ^ { n } = ( x - 1 ) ^ { n } ( x + 1 ) ^ { n }$ and integrate by parts n times to calculate this last integral.] 

(c) Prove that any polynomial of degree n that is orthogonal to $1 , x , x ^ { 2 } , \ldots , x ^ { n - 1 }$ is a constant multiple of $L _ { n }$ 

(d) Let $\mathcal { L } _ { n } = L _ { n } / \Vert L _ { n } \Vert$ , which are the normalized Legendre polynomials. Prove that $\{ { \mathcal { L } } _ { n } \}$ is the family obtained by applying the “Gram-Schmidt process” to $\{ 1 , x , \ldots , x ^ { n } , \ldots \}$ , and conclude that every Riemann integrable function $f$ on $[ - 1 , 1 ]$ has a Legendre expansion 

$$
\sum_ {n = 0} ^ {\infty} \langle f, \mathcal {L} _ {n} \rangle \mathcal {L} _ {n}
$$

which converges to f in the mean-square sense. 

3. Let α be a complex number not equal to an integer. 

(a) Calculate the Fourier series of the 2π-periodic function defined on $[ - \pi , \pi ]$ by $f ( x ) = \cos ( \alpha x )$ 

(b) Prove the following formulas due to Euler: 

$$
\sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {2} - \alpha^ {2}} = \frac {1}{2 \alpha^ {2}} - \frac {\pi}{2 \alpha \tan (\alpha \pi)}.
$$

For all $u \in \mathbb { C } - \pi \mathbb { Z }$ 

$$
\cot u = \frac {1}{u} + 2 \sum_ {n = 1} ^ {\infty} \frac {u}{u ^ {2} - n ^ {2} \pi^ {2}}.
$$

4. Problems 

(c) Show that for all $\alpha \in \mathbb { C } - \mathbb { Z }$ we have 

$$
{\frac {\alpha \pi}{\sin (\alpha \pi)}} = 1 + 2 \alpha^ {2} \sum_ {n = 1} ^ {\infty} {\frac {(- 1) ^ {n - 1}}{n ^ {2} - \alpha^ {2}}}.
$$

(d) For all $0 < \alpha < 1 _ { : }$ , show that 

$$
\int_ {0} ^ {\infty} \frac {t ^ {\alpha - 1}}{t + 1} d t = \frac {\pi}{\sin (\alpha \pi)}.
$$

[Hint: Split the integral as $\textstyle \int _ { 0 } ^ { 1 } + \int _ { 1 } ^ { \infty }$ and change variables $t = 1 / u$ in the second integral. Now both integrals are of the form 

$$
\int_ {0} ^ {1} \frac {t ^ {\gamma - 1}}{1 + t} d t, \quad 0 <   \gamma <   1,
$$

which one can show is equal to $\scriptstyle \sum _ { k = 0 } ^ { \infty } { \frac { ( - 1 ) ^ { k } } { k + \gamma } }$ . Use part (c) to conclude the proof.] 

4. In this problem, we find the formula for the sum of the series 

$$
\sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {k}}
$$

where $k$ is any even integer. These sums are expressed in terms of the Bernoulli numbers; the related Bernoulli polynomials are discussed in the next problem. 

Define the Bernoulli numbers $B _ { n }$ by the formula 

$$
{\frac {z}{e ^ {z} - 1}} = \sum_ {n = 0} ^ {\infty} {\frac {B _ {n}}{n !}} z ^ {n}.
$$

(a) Show that $B _ { 0 } = 1 , B _ { 1 } = - 1 / 2 , B _ { 2 } = 1 / 6 , B _ { 3 } = 0 , B _ { 4 } = - 1 / 3 0$ , and $B _ { 5 } = 0 .$ 

(b) Show that for $n \geq 1$ we have 

$$
B _ {n} = - \frac {1}{n + 1} \sum_ {k = 0} ^ {n - 1} {\binom {n + 1} {k}} B _ {k}.
$$

(c) By writing 

$$
{\frac {z}{e ^ {z} - 1}} = 1 - {\frac {z}{2}} + \sum_ {n = 2} ^ {\infty} {\frac {B _ {n}}{n !}} z ^ {n},
$$

show that $B _ { n } = 0$ if n is odd and $> 1$ . Also prove that 

$$
z \cot z = 1 + \sum_ {n = 1} ^ {\infty} (- 1) ^ {n} \frac {2 ^ {2 n} B _ {2 n}}{(2 n) !} z ^ {2 n}.
$$

(d) The zeta function is defined by 

$$
\zeta (s) = \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {s}}, \quad \text { for   all } s > 1.
$$

Deduce from the result in (c), and the expression for the cotangent function obtained in the previous problem, that 

$$
x \cot x = 1 - 2 \sum_ {m = 1} ^ {\infty} \frac {\zeta (2 m)}{\pi^ {2 m}} x ^ {2 m}.
$$

(e) Conclude that 

$$
2 \zeta (2 m) = (- 1) ^ {m + 1} \frac {(2 \pi) ^ {2 m}}{(2 m) !} B _ {2 m}.
$$

5. Define the Bernoulli polynomials $B _ { n } ( x )$ by the formula 

$$
{\frac {z e ^ {x z}}{e ^ {z} - 1}} = \sum_ {n = 0} ^ {\infty} {\frac {B _ {n} (x)}{n !}} z ^ {n}.
$$

(a) The functions $B _ { n } ( x )$ are polynomials in $x$ and 

$$
B _ {n} (x) = \sum_ {k = 0} ^ {n} {\binom {n} {k}} B _ {k} x ^ {n - k}.
$$

Show that $B _ { 0 } ( x ) = 1 , B _ { 1 } ( x ) = x - 1 / 2 , B _ { 2 } ( x ) = x ^ { 2 } - x + 1 / 6 ,$ and $\begin{array} { r } { B _ { 3 } ( x ) = x ^ { 3 } - \frac { 3 } { 2 } x ^ { 2 } + \frac { 1 } { 2 } x . } \end{array}$ 

(b) If $n \geq 1$ , then 

$$
B _ {n} (x + 1) - B _ {n} (x) = n x ^ {n - 1},
$$

and if $n \geq 2 .$ , then 

$$
B _ {n} (0) = B _ {n} (1) = B _ {n}.
$$

(c) Define $S _ { m } ( n ) = 1 ^ { m } + 2 ^ { m } + \cdot \cdot \cdot + ( n - 1 ) ^ { m }$ . Show that 

$$
(m + 1) S _ {m} (n) = B _ {m + 1} (n) - B _ {m + 1}.
$$

## 4. Problems

(d) Prove that the Bernoulli polynomials are the only polynomials that satisfy 

(i) $B _ { 0 } ( x ) = 1 { \mathrm { . } }$ 

(ii) $B _ { n } ^ { \prime } ( x ) = n B _ { n - 1 } ( x )$ for $n \geq 1$ 

(iii) $\begin{array} { r } { \int _ { 0 } ^ { 1 } B _ { n } ( x ) d x = 0 } \end{array}$ for $n \geq 1$ , and show that from (b) one obtains 

$$
\int_ {x} ^ {x + 1} B _ {n} (t) d t = x ^ {n}.
$$

(e) Calculate the Fourier series of $B _ { 1 } ( x )$ to conclude that for $0 < x < 1$ we have 

$$
B _ {1} (x) = x - 1 / 2 = \frac {- 1}{\pi} \sum_ {k = 1} ^ {\infty} \frac {\sin (2 \pi k x)}{k}.
$$

Integrate and conclude that 

$$
B _ {2 n} (x) = (- 1) ^ {n + 1} \frac {2 (2 n) !}{(2 \pi) ^ {2 n}} \sum_ {k = 1} ^ {\infty} \frac {\cos (2 \pi k x)}{k ^ {2 n}},
$$

$$
B _ {2 n + 1} (x) = (- 1) ^ {n + 1} \frac {2 (2 n + 1) !}{(2 \pi) ^ {2 n + 1}} \sum_ {k = 1} ^ {\infty} \frac {\sin (2 \pi k x)}{k ^ {2 n + 1}}.
$$

Finally, show that for $0 < x < 1$ - 

$$
B _ {n} (x) = - \frac {n !}{(2 \pi i) ^ {n}} \sum_ {k \neq 0} \frac {e ^ {2 \pi i k x}}{k ^ {n}}.
$$

We observe that the Bernoulli polynomials are, up to normalization, successive integrals of the sawtooth function. 

# 4 <sub>Some</sub> <sub>Applications</sub> <sub>of</sub> <sub>Fourier</sub> Series

Fourier series and analogous expansions intervene very naturally in the general theory of curves and surfaces. In efect, this theory, conceived from the point of view of analysis, deals obviously with the study of arbitrary functions. I was thus led to use Fourier series in several questions of geometry, and I have obtained in this direction a number of results which will be presented in this work. One notes that my considerations form only a beginning of a principal series of researches, which would without doubt give many new results. 

A. Hurwitz, 1902 

In the previous chapters we introduced some basic facts about Fourier analysis, motivated by problems that arose in physics. The motion of a string and the difusion of heat were two instances that led naturally to the expansion of a function in terms of a Fourier series. We propose next to give the reader a flavor of the broader impact of Fourier analysis, and illustrate how these ideas reach out to other areas of mathematics. In particular, consider the following three problems: 

I. Among all simple closed curves of length ` in the plane R<sup>2</sup>, which one encloses the largest area? 

II. Given an irrational number γ, what can be said about the distribution of the fractional parts of the sequence of numbers nγ, for $n = 1 , 2 , 3 , \dotsc 2$ 

III. Does there exist a continuous function that is nowhere diferen tiable? 

The first problem is clearly geometric in nature, and at first sight, would seem to have little to do with Fourier series. The second question lies on the border between number theory and the study of dynamical systems, and gives us the simplest example of the idea of “ergodicity.” The third problem, while analytic in nature, resisted many attempts before the 

## 1. The isoperimetric inequality

solution was finally discovered. It is remarkable that all three questions can be resolved quite simply and directly by the use of Fourier series. 

In the last section of this chapter, we return to a problem that provided our initial motivation. We consider the time-dependent heat equation on the circle. Here our investigation will lead us to the important but enigmatic heat kernel for the circle. However, the mysteries surrounding its basic properties will not be fully understood until we can apply the Poisson summation formula, which we will do in the next chapter. 

## 1 The isoperimetric inequality

Let Γ denote a closed curve in the plane which does not intersect itself. Also, let ` denote the length of Γ, and A the area of the bounded region in $\mathbb { R } ^ { 2 }$ enclosed by Γ. The problem now is to determine for a given ` the curve Γ which maximizes A (if any such curve exists). 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/8c121a90fd611bec399e454fa49b00e13a5a8345acb67df6aa484f4124119934.jpg)



Figure 1. The isoperimetric problem


A little experimentation and reflection suggests that the solution should be a circle. This conclusion can be reached by the following heuristic considerations. The curve can be thought of as a closed piece of string lying flat on a table. If the region enclosed by the string is not convex (for example), one can deform part of the string and increase the area enclosed by it. Also, playing with some simple examples, one can convince oneself that the “flatter” the curve is in some portion, the less eficient it is in enclosing area. Therefore we want to maximize the “roundness” of the curve at each point. 

Although the circle is the correct guess, making the above ideas precise is a dificult matter. 

The key idea in the solution we give to the isoperimetric problem consists of an application of Parseval’s identity for Fourier series. However, before we can attempt a solution to this problem, we must define the notion of a simple closed curve, its length, and what we mean by the area of the region enclosed by it. 

## Curves, length and area

A parametrized curve $\gamma$ is a mapping 

$$
\gamma : [ a, b ] \to \mathbb {R} ^ {2}.
$$

The image of $\gamma$ is a set of points in the plane which we call a curve and denote by Γ. The curve Γ is simple if it does not intersect itself, and closed if its two end-points coincide. In terms of the parametrization above, these two conditions translate into $\gamma ( s _ { 1 } ) \neq \gamma ( s _ { 2 } )$ unless $s _ { 1 } = a$ and $s _ { 2 } = b ,$ , in which case $\gamma ( a ) = \gamma ( b )$ . We may extend $\gamma$ to a periodic function on R of period $b - a .$ , and think of $\gamma$ as a function on the circle. We also always impose some smoothness on our curves by assuming that $\gamma$ is of class $C ^ { 1 }$ , and that its derivative $\gamma ^ { \prime }$ satisfies $\gamma ^ { \prime } ( s ) \neq 0$ . Altogether, these conditions guarantee that Γ has a well-defined tangent at each point, which varies continuously as the point on the curve varies. Moreover, the parametrization $\gamma$ induces an orientation on $\Gamma$ as the parameter s travels from a to b. 

Any $C ^ { 1 }$ bijective mapping $s : [ c , d ] \to [ a , b ]$ gives rise to another parametrization of Γ by the formula 

$$
\eta (t) = \gamma (s (t)).
$$

Clearly, the conditions that $\Gamma$ be closed and simple are independent of the chosen parametrization. Also, we say that the two parametrizations $\gamma$ and $\eta$ are equivalent if $s ^ { \prime } ( t ) > 0$ for all $t ;$ this means that $\eta$ and $\gamma$ induce the same orientation on the curve Γ. If, however, $s ^ { \prime } ( t ) < 0$ , then η reverses the orientation. 

If Γ is parametrized by $\gamma ( s ) = ( x ( s ) , y ( s ) )$ , then the length of the curve Γ is defined by 

$$
\ell = \int_ {a} ^ {b} | \gamma^ {\prime} (s) | d s = \int_ {a} ^ {b} \left(x ^ {\prime} (s) ^ {2} + y ^ {\prime} (s) ^ {2}\right) ^ {1 / 2} d s.
$$

The length of $\Gamma$ is a notion intrinsic to the curve, and does not depend on its parametrization. To see that this is indeed the case, suppose that $\gamma ( s ( t ) ) = \eta ( t )$ . Then, the change of variables formula and the chain rule imply that 

$$
\int_ {a} ^ {b} | \gamma^ {\prime} (s) | d s = \int_ {c} ^ {d} | \gamma^ {\prime} (s (t)) | | s ^ {\prime} (t) | d t = \int_ {c} ^ {d} | \eta^ {\prime} (t) | d t,
$$

## 1. The isoperimetric inequality

as desired. 

In the proof of the theorem below, we shall use a special type of parametrization for Γ. We say that $\gamma$ is a parametrization by arclength if $\left| \gamma ^ { \prime } ( s ) \right| = 1$ for all s. This means that $\gamma ( s )$ travels at a constant speed, and as a consequence, the length of Γ is precisely $b - a .$ . Therefore, after a possible additional translation, a parametrization by arc-length will be defined on [0, `]. Any curve admits a parametrization by arclength (Exercise 1). 

We now turn to the isoperimetric problem. 

The attempt to give a precise formulation of the area A of the region enclosed by a simple closed curve Γ raises a number of tricky questions. In a variety of simple situations, it is evident that the area is given by the following familiar formula of the calculus: 

$$
\begin{array}{l} \mathcal {A} = \frac {1}{2} \left| \int_ {\Gamma} (x d y - y d x) \right| \\ = \frac {1}{2} \left| \int_ {a} ^ {b} x (s) y ^ {\prime} (s) - y (s) x ^ {\prime} (s) d s \right|; \end{array}\tag{1}
$$

see, for example, Exercise 3. Thus in formulating our result we shall adopt the easy expedient of taking (1) as our definition of area. This device allows us to give a quick and neat proof of the isoperimetric inequality. A listing of issues this simplification leaves unresolved can be found after the proof of the theorem. 

## Statement and proof of the isoperimetric inequality

Theorem 1.1 Suppose that Γ is a simple closed curve in $\mathbb { R } ^ { 2 }$ of length $\ell ,$ and let A denote the area of the region enclosed by this curve. Then 

$$
\mathcal {A} \leq \frac {\ell^ {2}}{4 \pi},
$$

with equality if and only if Γ is a circle. 

The first observation is that we can rescale the problem. This means that we can change the units of measurement by a factor of $\delta > 0$ as follows. Consider the mapping of the plane $\mathbb { R } ^ { 2 }$ to itself, which sends the point $( x , y )$ to $( \delta x , \delta y )$ . A look at the formula defining the length of a curve shows that if Γ is of length $\ell ,$ then its image under this mapping has length $\delta \ell .$ So this operation magnifies or contracts lengths by a factor of δ depending on whether $\delta \geq 1$ or $\delta \leq 1$ . Similarly, we see that the mapping magnifies (or contracts) areas by a factor of $\delta ^ { 2 }$ . By taking $\delta = 2 \pi / \ell$ , we see that it sufices to prove that if $\ell = 2 \pi$ then $A \le \pi$ , with equality only if Γ is a circle. 

Let $\gamma : [ 0 , 2 \pi ] \to \mathbb { R } ^ { 2 }$ with $\gamma ( s ) = ( x ( s ) , y ( s ) )$ ) be a parametrization by arc-length of the curve Γ, that is, $x ^ { \prime } ( s ) ^ { 2 } + y ^ { \prime } ( s ) ^ { 2 } = 1$ for all $s \in [ 0 , 2 \pi ]$ This implies that 

$$
\frac {1}{2 \pi} \int_ {0} ^ {2 \pi} (x ^ {\prime} (s) ^ {2} + y ^ {\prime} (s) ^ {2}) d s = 1.\tag{2}
$$

Since the curve is closed, the functions $x ( s )$ and $y ( s )$ are 2π-periodic, so we may consider their Fourier series 

$$
x (s) \sim \sum a _ {n} e ^ {i n s} \quad \mathrm{and} \quad y (s) \sim \sum b _ {n} e ^ {i n s}.
$$

Then, as we remarked in the later part of Section 2 of Chapter 2, we have 

$$
x ^ {\prime} (s) \sim \sum a _ {n} i n e ^ {i n s} \quad \mathrm{and} \quad y ^ {\prime} (s) \sim \sum b _ {n} i n e ^ {i n s}.
$$

Parseval’s identity applied to (2) gives 

$$
\sum_ {n = - \infty} ^ {\infty} | n | ^ {2} \left(| a _ {n} | ^ {2} + | b _ {n} | ^ {2}\right) = 1.\tag{3}
$$

We now apply the bilinear form of Parseval’s identity (Lemma 1.5, Chapter 3) to the integral defining A. Since $x ( s )$ and $y ( s )$ are real-valued, we have $a _ { n } = \overline { { a _ { - n } } }$ and $b _ { n } = { \overline { { b _ { - n } } } } ,$ so we find that 

$$
\mathcal {A} = \frac {1}{2} \left| \int_ {0} ^ {2 \pi} x (s) y ^ {\prime} (s) - y (s) x ^ {\prime} (s) d s \right| = \pi \left| \sum_ {n = - \infty} ^ {\infty} n \left(a _ {n} \overline {{b _ {n}}} - b _ {n} \overline {{a _ {n}}}\right) \right|.
$$

We observe next that 

$$
| a _ {n} \overline {{b _ {n}}} - b _ {n} \overline {{a _ {n}}} | \leq 2 | a _ {n} | | b _ {n} | \leq | a _ {n} | ^ {2} + | b _ {n} | ^ {2},\tag{4}
$$

and since $| n | \leq | n | ^ { 2 }$ , we may use (3) to get 

$$
\begin{array}{l} \mathcal {A} \leq \pi \sum_ {n = - \infty} ^ {\infty} | n | ^ {2} \left(| a _ {n} | ^ {2} + | b _ {n} | ^ {2}\right) \\ \leq \pi , \end{array}
$$

2. Weyl’s equidistribution theorem 

as desired. 

When $A = \pi$ , we see from the above argument that 

$$
x (s) = a _ {- 1} e ^ {- i s} + a _ {0} + a _ {1} e ^ {i s} \quad \mathrm{and} \quad y (s) = b _ {- 1} e ^ {- i s} + b _ {0} + b _ {1} e ^ {i s}
$$

because $| n | < | n | ^ { 2 }$ as soon as $| n | \geq 2 .$ . We know that $x ( s )$ and $y ( s )$ are real-valued, so $a _ { - 1 } = \overline { { a _ { 1 } } }$ and $b _ { - 1 } = \overline { { b _ { 1 } } }$ . The identity (3) implies that $2 \left( | a _ { 1 } | ^ { 2 } + | b _ { 1 } | ^ { 2 } \right) = 1$ , and since we have equality in (4) we must have $| a _ { 1 } | = | b _ { 1 } | = 1 / 2$ . We write 

$$
a _ {1} = \frac {1}{2} e ^ {i \alpha} \quad \mathrm{and} \quad b _ {1} = \frac {1}{2} e ^ {i \beta}.
$$

The fact that $1 = 2 | a _ { 1 } \overline { { b _ { 1 } } } - \overline { { a _ { 1 } } } b _ { 1 } |$ implies that $| \sin ( \alpha - \beta ) | = 1$ , hence $\alpha - \beta = k \pi / 2$ where k is an odd integer. From this we find that 

$$
x (s) = a _ {0} + \cos (\alpha + s) \quad \mathrm{and} \quad y (s) = b _ {0} \pm \sin (\alpha + s),
$$

where the sign in $y ( s )$ depends on the parity of $( k - 1 ) / 2$ . In any case, we see that Γ is a circle, for which the case of equality obviously holds, and the proof of the theorem is complete. 

The solution given above (due to Hurwitz in 1901) is indeed very elegant, but clearly leaves some important issues unanswered. We list these as follows. Suppose Γ is a simple closed curve. 

(i) How is the “region enclosed by $\Gamma ^ { \prime \prime }$ defined? 

(ii) What is the geometric definition of the “area” of this region? Does this definition accord with (1)? 

(iii) Can these results be extended to the most general class of simple closed curves relevant to the problem—those curves which are “rectifiable”—that is, those to which we can ascribe a finite length? 

It turns out that the clarifications of the problems raised are connected to a number of other significant ideas in analysis. We shall return to these questions in succeeding books of this series. 

## 2 Weyl’s equidistribution theorem

We now apply ideas coming from Fourier series to a problem dealing with properties of irrational numbers. We begin with a brief discussion of congruences, a concept needed to understand our main theorem. 

## The reals modulo the integers

If x is a real number, we let [x] denote the greatest integer less than or equal to $x$ and call the quantity $[ x ]$ the integer part of $x .$ The fractional part of x is then defined by $\langle x \rangle = x - [ x ]$ . In particular, $\langle x \rangle \in [ 0 , 1 )$ for every $x \in \mathbb { R }$ . For example, the integer and fractional parts of $2 . 7$ are 2 and $0 . 7 ,$ , respectively, while the integer and fractional parts of −3.4 are $- 4$ and $0 . 6 .$ , respectively. 

We may define a relation on R by saying that the two numbers x and y are equivalent, or congruent, if $x - y \in \mathbb { Z }$ . We then write 

$$
x = y \bmod {\mathbb {Z}} \quad \text { or } \quad x = y \bmod 1.
$$

This means that we identify two real numbers if they difer by an integer. Observe that any real number $x$ is congruent to a unique number in $[ 0 , 1 )$ which is precisely $\langle x \rangle$ , the fractional part of x. In efect, reducing a real number modulo $\mathbb { Z }$ means looking only at its fractional part and disregarding its integer part. 

Now start with a real number $\gamma \neq 0$ and look at the sequence $\gamma , 2 \gamma , 3 \gamma , \ldots ,$ . An intriguing question is to ask what happens to this sequence if we reduce it modulo $\mathbb { Z } ,$ , that ${ \mathrm { i s } } ,$ if we look at the sequence of fractional parts 

$$
\langle \gamma \rangle , \langle 2 \gamma \rangle , \langle 3 \gamma \rangle , \dots .
$$

Here are some simple observations: 

(i) If $\gamma$ is rational, then only finitely many numbers appearing in $\langle n \gamma \rangle$ are distinct. 

(ii) If $\gamma$ is irrational, then the numbers $\langle n \gamma \rangle$ are all distinct. 

Indeed, for part (i), note that if $\gamma = p / q$ , the first q terms in the sequence are 

$$
\langle p / q \rangle , \langle 2 p / q \rangle , \dots , \langle (q - 1) p / q \rangle , \langle q p / q \rangle = 0.
$$

The sequence then begins to repeat itse $\operatorname { l f } ,$ since 

$$
\langle (q + 1) p / q \rangle = \langle 1 + p / q \rangle = \langle p / q \rangle ,
$$

and so on. However, see Exercise 6 for a more refined result. 

Also, for part (ii) assume that not all numbers are distinct. We therefore have $\langle n _ { 1 } \gamma \rangle = \langle n _ { 2 } \gamma \rangle$ for some $n _ { 1 } \neq n _ { 2 } ;$ then $n _ { 1 } \gamma - n _ { 2 } \gamma \in \mathbb { Z } .$ , hence $\gamma$ is rational, a contradiction. 

## 2. Weyl’s equidistribution theorem

In fact, it can be shown that if γ is irrational, then $\langle n \gamma \rangle$ is dense in the interval [0, 1), a result originally proved by Kronecker. In other words, the sequence $\langle n \gamma \rangle$ hits every sub-interval of $[ 0 , 1 )$ (and hence it does so infinitely many times). We will obtain this fact as a corollary of a deeper theorem dealing with the uniform distribution of the sequence $\langle n \gamma \rangle$ 

A sequence of numbers $\xi _ { 1 } , \xi _ { 2 } , \ldots , \xi _ { n } , \ldots$ . in [0, 1) is said to be equidistributed if for every interval $( a , b ) \subset [ 0 , 1 )$ 

$$
\lim _ {N \to \infty} \frac {\# \{1 \leq n \leq N : \xi_ {n} \in (a , b) \}}{N} = b - a
$$

where #A denotes the cardinality of the finite set A. This means that for large N, the proportion of numbers $\xi _ { n }$ in $( a , b )$ with $n \leq N$ is equal to the ratio of the length of the interval $( a , b )$ to the length of the interval $[ 0 , 1 )$ . In other words, the sequence $\xi _ { n }$ sweeps out the whole interval evenly, and every sub-interval gets its fair share. Clearly, the ordering of the sequence is very important, as the next two examples illustrate. 

Example 1. The sequence 

$$
0, \frac {1}{2}, 0, \frac {1}{3}, \frac {2}{3}, 0, \frac {1}{4}, \frac {2}{4}, \frac {3}{4}, 0, \frac {1}{5}, \frac {2}{5}, \dots
$$

appears to be equidistributed since it passes over the interval $[ 0 , 1 )$ very evenly. Of course this is not a proof, and the reader is invited to give one. For a somewhat related example, see Exercise 8 with $\sigma = 1 / 2$ 

Example 2. Let $\{ r _ { n } \} _ { n = 1 } ^ { \infty }$ be any enumeration of the rationals in [0, 1). Then the sequence defined by 

$$
\xi_ {n} = \left\{ \begin{array}{l l} r _ {n / 2} & \text { if   } n \text {   is   even }, \\ 0 & \text { if   } n \text {   is   odd }, \end{array} \right.
$$

is not equidistributed since “half” of the sequence is at 0. Nevertheless, this sequence is obviously dense. 

We now arrive at the main theorem of this section. 

Theorem 2.1 $I f \gamma$ is irrational, then the sequence of fractional parts $\langle \gamma \rangle , \langle 2 \gamma \rangle , \langle 3 \gamma \rangle , \dots .$ is equidistributed in [0, 1). 

In particular, $\langle n \gamma \rangle$ is dense in [0, 1), and we get Kronecker’s theorem as a corollary. In Figure 2 we illustrate the set of points $\langle \gamma \rangle , \langle 2 \gamma \rangle$ ， $\langle 3 \gamma \rangle , \ldots , \langle N \gamma \rangle$ for three diferent values of N when $\gamma = \sqrt { 2 }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/7e34c11cf248ce20f4390325a116221741ae179e68d6f6f390cb8eca72b13941.jpg)



Figure 2. The sequence $\langle \gamma \rangle , \langle 2 \gamma \rangle , \langle 3 \gamma \rangle , \dots , \langle N \gamma \rangle$ when $\gamma = \sqrt { 2 }$


Fix $( a , b ) \subset [ 0 , 1 )$ and let $\chi _ { ( a , b ) } ( \boldsymbol { x } )$ denote the characteristic function of the interval $( a , b )$ , that is, the function equal to 1 in $( a , b )$ and 0 in $[ 0 , 1 ) - ( a , b )$ . We may extend this function to R by periodicity (period 1), and still denote this extension by $\chi _ { ( a , b ) } ( \boldsymbol { x } )$ . Then, as a consequence of the definitions, we find that 

$$
\# \{1 \leq n \leq N: \langle n \gamma \rangle \in (a, b) \} = \sum_ {n = 1} ^ {N} \chi_ {(a, b)} (n \gamma),
$$

and the theorem can be reformulated as the statement that 

$$
\frac {1}{N} \sum_ {n = 1} ^ {N} \chi_ {(a, b)} (n \gamma) \rightarrow \int_ {0} ^ {1} \chi_ {(a, b)} (x) d x, \quad \text { as } N \rightarrow \infty .
$$

This step removes the dificulty of working with fractional parts and reduces the number theory to analysis. 

The heart of the matter lies in the following result. 

Lemma 2.2 If f is continuous and periodic of period 1, and $\gamma$ is irrational, then 

$$
\frac {1}{N} \sum_ {n = 1} ^ {N} f (n \gamma) \rightarrow \int_ {0} ^ {1} f (x) d x \quad a s N \rightarrow \infty .
$$

The proof of the lemma is divided into three steps. 

Step 1. We first check the validity of the limit in the case when $f$ is one of the exponentials 1, $e ^ { 2 \pi i x } , \ldots , e ^ { 2 \pi i k x } , \ldots . \mathrm { ~ I f ~ } f = 1$ , the limit 

## 2. Weyl’s equidistribution theorem

surely holds. If $f = e ^ { 2 \pi i k x }$ with $k \neq 0$ , then the integral is 0. Since $\gamma$ is irrational, we have $e ^ { 2 \pi i k \gamma } \neq 1$ , therefore 

$$
\frac {1}{N} \sum_ {n = 1} ^ {N} f (n \gamma) = \frac {e ^ {2 \pi i k \gamma}}{N} \frac {1 - e ^ {2 \pi i k N \gamma}}{1 - e ^ {2 \pi i k \gamma}},
$$

which goes to 0 as $N \to \infty$ 

Step 2. It is clear that if f and g satisfy the lemma, then so does $A f + B g$ for any $A , B \in \mathbb { C }$ . Therefore, the first step implies that the lemma is true for all trigonometric polynomials. 

Step 3. Let $\epsilon > 0$ . If f is any continuous periodic function of period 1, choose a trigonometric polynomial $P$ so that $\begin{array} { r } { \operatorname* { s u p } _ { x \in \mathbb { R } } | f ( x ) - P ( x ) | < \epsilon / 3 } \end{array}$ (this is possible by Corollary 5.4 in Chapter 2). Then, by step 1, for all large N we have 

$$
\left| \frac {1}{N} \sum_ {n = 1} ^ {N} P (n \gamma) - \int_ {0} ^ {1} P (x) d x \right| <   \epsilon / 3.
$$

Therefore 

$$
\begin{array}{l} \left| \frac {1}{N} \sum_ {n = 1} ^ {N} f (n \gamma) - \int_ {0} ^ {1} f (x) d x \right| \leq \frac {1}{N} \sum_ {n = 1} ^ {N} | f (n \gamma) - P (n \gamma) | + \\ \qquad \qquad \qquad + \left| \frac {1}{N} \sum_ {n = 1} ^ {N} P (n \gamma) - \int_ {0} ^ {1} P (x) d x \right| + \\ \qquad \qquad \qquad + \int_ {0} ^ {1} | P (x) - f (x) | d x \\ <   \epsilon , \end{array}
$$

and the lemma is proved. 

Now we can finish the proof of the theorem. Choose two continuous periodic functions $f _ { \epsilon } ^ { + }$ and $f _ { \epsilon } ^ { - }$ of period 1 which approximate $\chi _ { ( a , b ) } ( \boldsymbol { x } )$ on [0, 1) from above and below; both $f _ { \epsilon } ^ { + }$ and $f _ { \epsilon } ^ { - }$ are bounded by 1 and agree with $\chi _ { ( a , b ) } ( \boldsymbol { x } )$ except in intervals of total length 2² (see Figure 3). 

In particular, $f _ { \epsilon } ^ { - } ( x ) \leq \chi _ { ( a , b ) } ( x ) \leq f _ { \epsilon } ^ { + } ( x )$ , and 

$$
b - a - 2 \epsilon \leq \int_ {0} ^ {1} f _ {\epsilon} ^ {-} (x) d x \quad \text { and } \quad \int_ {0} ^ {1} f _ {\epsilon} ^ {+} (x) d x \leq b - a + 2 \epsilon .
$$

If $\begin{array} { r } { S _ { N } = \frac { 1 } { N } \sum _ { n = 1 } ^ { N } \chi _ { ( a , b ) } ( n \gamma ) } \end{array}$ , then we get 

$$
\frac {1}{N} \sum_ {n = 1} ^ {N} f _ {\epsilon} ^ {-} (n \gamma) \leq S _ {N} \leq \frac {1}{N} \sum_ {n = 1} ^ {N} f _ {\epsilon} ^ {+} (n \gamma).
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/1b594d8cb0ecc82725fd163de1ac37698fc732fd244fe468f916cffd5b22b25d.jpg)



Figure 3. Approximations of $\chi _ { ( a , b ) } ( \boldsymbol { x } )$


Therefore 

$$
b - a - 2 \epsilon \leq \liminf _ {N \to \infty} S _ {N} \quad \text { and } \quad \limsup _ {N \to \infty} S _ {N} \leq b - a + 2 \epsilon .
$$

Since this is true for every $\epsilon > 0 .$ , the limit lim $. { \cal N } \to \infty  \stackrel { } { S } _ { N }$ exists and must equal $b - a$ . This completes the proof of the equidistribution theorem. 

This theorem has the following consequence. 

Corollary 2.3 The conclusion of Lemma 2.2 holds for every function f which is Riemann integrable in [0, 1], and periodic of period 1. 

Proof. Assume f is real-valued, and consider a partition of the interval [0, 1], say $0 = x _ { 0 } < x _ { 1 } < \cdot \cdot \cdot < x _ { N } = 1$ . Next, define $f _ { U } ( x ) =$ $\begin{array} { r } { \operatorname* { s u p } _ { x _ { j - 1 } \leq y \leq x _ { j } } f ( y ) \mathrm { i f } x \in [ x _ { j - 1 } , x _ { j } ) } \end{array}$ and $\begin{array} { r } { f _ { L } ( x ) = \operatorname* { i n f } _ { x _ { j - 1 } \leq y \leq x _ { j } } f ( y ) } \end{array}$ for $x \in$ $( x _ { j - 1 } , x _ { j } )$ . Then clearly $f _ { L } \leq f \leq f _ { U }$ and 

$$
\int_ {0} ^ {1} f _ {L} (x) d x \leq \int_ {0} ^ {1} f (x) d x \leq \int_ {0} ^ {1} f _ {U} (x) d x.
$$

Moreover, by making the partition suficiently fine we can guarantee that for a given $\epsilon > 0$ 2 

$$
\int_ {0} ^ {1} f _ {U} (x) d x - \int_ {0} ^ {1} f _ {L} (x) d x \leq \epsilon .
$$

However, 

$$
\frac {1}{N} \sum_ {n = 1} ^ {N} f _ {L} (n \gamma) \rightarrow \int_ {0} ^ {1} f _ {L} (x) d x
$$

## 2. Weyl’s equidistribution theorem

by the theorem, because each $f _ { L }$ is a finite linear combination of characteristic functions of intervals; similarly we have 

$$
\frac {1}{N} \sum_ {n = 1} ^ {N} f _ {U} (n \gamma) \rightarrow \int_ {0} ^ {1} f _ {U} (x) d x.
$$

From these two assertions we can conclude the proof of the corollary by using the previous approximation argument. 

There is an interesting interpretation of the lemma and its corollary, in terms of a simple dynamical system. In this example, the underlying space is the circle parametrized by the angle $\theta .$ . We also consider a mapping of this space to itself: here, we choose a rotation $\rho$ of the circle by the angle 2πγ, that is, the transformation $\rho : \theta \mapsto \theta + 2 \pi \gamma$ 

We want next to consider how this space, with its underlying action $\rho ,$ evolves in time. In other words, we wish to consider the iterates of $\rho ,$ namely $\rho , \rho ^ { 2 } , \rho ^ { 3 } , . . . , \rho ^ { n }$ where 

$$
\rho^ {n} = \rho \circ \rho \circ \dots \circ \rho : \theta \mapsto \theta + 2 \pi n \gamma ,
$$

and where we think of the action $\rho ^ { n }$ taking place at the time $t = n$ 

To each Riemann integrable function $f$ on the circle, we can also associate the corresponding efects of the rotation $\rho ,$ and obtain a sequence of functions 

$$
f (\theta), f (\rho (\theta)), f (\rho^ {2} (\theta)), \ldots , f (\rho^ {n} (\theta)), \ldots
$$

with $f ( \rho ^ { n } ( \theta ) ) = f ( \theta + 2 \pi n \gamma )$ . In this special context, the ergodicity of this system is then the statement that the “time average” 

$$
\lim _ {N \to \infty} \frac {1}{N} \sum_ {n = 1} ^ {N} f (\rho^ {n} (\theta))
$$

exists for each θ and equals the “space average” 

$$
\frac {1}{2 \pi} \int_ {0} ^ {2 \pi} f (\theta) d \theta ,
$$

whenever $\gamma$ is irrational. In fact, this assertion is merely a rephrasing of Corollary 2.3, once we make the change of variables $\theta = 2 \pi x$ 

Returning to the problem of equidistributed sequences, we observe that the proof of Theorem 2.1 gives the following characterization. 

Weyl’s criterion. A sequence of real numbers $\xi _ { 1 } , \xi _ { 2 } \ldots$ . in $[ 0 , 1 )$ is equidistributed if and only if for all integers $k \neq 0$ one has 

$$
\frac {1}{N} \sum_ {n = 1} ^ {N} e ^ {2 \pi i k \xi_ {n}} \rightarrow 0, \quad \mathrm{as} N \rightarrow \infty .
$$

One direction of this theorem was in efect proved above, and the converse can be found in Exercise 7. In particular, we find that to understand the equidistributive properties of a sequence $\xi _ { n } ,$ it sufices to estimate the size of the corresponding “exponential sum” $\textstyle \sum _ { n = 1 } ^ { N } e ^ { 2 \pi i k \xi _ { n } }$ . For example, it can be shown using Weyl’s criterion that the sequence $\langle n ^ { 2 } \gamma \rangle$ is equidistributed whenever $\gamma$ is irrational. This and other examples can be found in Exercises 8, and 9; also Problems 2, and 3. 

As a last remark, we mention a nice geometric interpretation of the distribution properties of $\langle n \gamma \rangle$ . Suppose that the sides of a square are reflecting mirrors and that a ray of light leaves a point inside the square. What kind of path will the light trace out? 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/49fc0e4a37f2399b5ece6d83f0b2d3413ada0a22ee79e45df9e6696a26e540ce.jpg)



Figure 4. Reflection of a ray of light in a square


To solve this problem, the main idea is to consider the grid of the plane formed by successively reflecting the initial square across its sides. With an appropriate choice of axis, the path traced by the light in the square corresponds to the straight line $P + ( t , \gamma t )$ in the plane. As a result, the reader may observe that the path will be either closed and periodic, or it will be dense in the square. The first of these situations 

## 3. A continuous but nowhere differentiable function

will happen if and only if the slope $\gamma$ of the initial direction of the light (determined with respect to one of the sides of the square) is rational. In the second situation, when $\gamma$ is irrational, the density follows from Kronecker’s theorem. What stronger conclusion does one get from the equidistribution theorem? 

## 3 A continuous but nowhere diferentiable function

There are many obvious examples of continuous functions that are not diferentiable at one point, say $f ( x ) = \left| x \right|$ . It is almost as easy to construct a continuous function that is not diferentiable at any given finite set of points, or even at appropriate sets containing countably many points. A more subtle problem is whether there exists a continuous function that is nowhere diferentiable. In 1861, Riemann guessed that the function defined by 

$$
R (x) = \sum_ {n = 1} ^ {\infty} \frac {\sin (n ^ {2} x)}{n ^ {2}}\tag{5}
$$

was nowhere diferentiable. He was led to consider this function because of its close connection to the theta function which will be introduced in Chapter 5. Riemann never gave a proof, but mentioned this example in one of his lectures. This triggered the interest of Weierstrass who, in an attempt to find a proof, came across the first example of a continuous but nowhere diferentiable function. Say $0 < b < 1$ and a is an integer $> 1$ In 1872 he proved that if $a b > 1 + 3 \pi / 2$ , then the function 

$$
W (x) = \sum_ {n = 1} ^ {\infty} b ^ {n} \cos (a ^ {n} x)
$$

is nowhere diferentiable. 

But the story is not complete without a final word about Riemann’s original function. In 1916 Hardy showed that R is not diferentiable at all irrational multiples of π, and also at certain rational multiples of π. However, it was not until much later, in 1969, that Gerver completely settled the problem, first by proving that the function R is actually diferentiable at all the rational multiples of π of the form $\pi p / q$ with p and q odd integers, and then by showing that R is not diferentiable in all of the remaining cases. 

In this section, we prove the following theorem. 

Theorem 3.1 If $0 < \alpha < 1$ , then the function 

$$
f _ {\alpha} (x) = f (x) = \sum_ {n = 0} ^ {\infty} 2 ^ {- n \alpha} e ^ {i 2 ^ {n} x}
$$

is continuous but nowhere diferentiable. 

The continuity is clear because of the absolute convergence of the series. The crucial property of $f$ which we need is that it has many vanishing Fourier coeficients. A Fourier series that skips many terms, like the one given above, or like $W ( x )$ , is called a lacunary Fourier series. 

The proof of the theorem is really the story of three methods of summing a Fourier series. First, there is the ordinary convergence in terms of the partial sums $S _ { N } ( g ) = g * D _ { N }$ . Next, there is Ces`aro summability $\sigma _ { N } ( g ) = g * F _ { N }$ , with $F _ { N }$ the Fej´er kernel. A third method, clearly connected with the second, involves the delayed means defined by 

$$
\triangle_ {N} (g) = 2 \sigma_ {2 N} (g) - \sigma_ {N} (g).
$$

Hence $\triangle _ { N } ( g ) = g * [ 2 F _ { 2 N } - F _ { N } ]$ . These methods can best be visualized as in Figure 5. 

Suppose $\begin{array} { r } { g ( x ) \sim \sum a _ { n } e ^ { i n x } } \end{array}$ . Then: 

$S _ { N }$ arises by multiplying the term $a _ { n } e ^ { i n x }$ by $1 { \mathrm { ~ i f ~ } } | n | \leq N$ , and 0 if $| n | > N$ 

$\sigma _ { N }$ arises by multiplying $a _ { n } e ^ { i n x }$ by $1 - | n | / N$ for $| n | \leq N$ and 0 for $| n | > N$ 

$\triangle _ { N }$ arises by multiplying $a _ { n } e ^ { i n x }$ by $1 { \mathrm { i f } } | n | \leq N$ , by $2 ( 1 - | n | / ( 2 N ) )$ for $N \leq | n | \leq 2 N$ , and 0 for $| n | > 2 N$ 

For example, note that 

$$
\begin{array}{l} \sigma_ {N} (g) (x) = \frac {S _ {0} (g) (x) + S _ {1} (g) (x) + \cdots + S _ {N - 1} (g) (x)}{N} \\ \qquad = \frac {1}{N} \sum_ {\ell = 0} ^ {N - 1} \sum_ {| k | \leq \ell} a _ {k} e ^ {i k x} \\ \qquad = \frac {1}{N} \sum_ {| n | \leq N} (N - | n |) a _ {n} e ^ {i n x} \\ \qquad = \sum_ {| n | \leq N} \left(1 - \frac {| n |}{N}\right) a _ {n} e ^ {i n x}. \end{array}
$$


σ<sub>N</sub> (g)(x) = P<sub>|n|≤N</sub> ³1 − |n|<sub>N</sub> a<sub>n</sub>e<sup>inx</sup>


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/6d9dcfd763fb75407c50f317c2a0bfa1544986383c211c7ce8143d91ac37385f.jpg)



S<sub>N</sub> (g)(x) = $\textstyle \sum _ { | n | \leq N } a _ { n } e ^ { i n x }$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/273d3a2d1f9975eecad1c3cbfa59df5b94e1a3f5bce10edbaa4067b648fba8f4.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/503e84e96217435691ddd1a0bf0a224ea1d79f42fd02c8da07100e5576544ece.jpg)



∆<sub>N</sub>(g)(x) = 2σ<sub>2N</sub>(g)(x) − σ<sub>N</sub>(g)(x)



Figure 5. Three summation methods


The proof of the other assertion is similar. 

The delayed means have two important features. On the one hand, their properties are closely related to the (good) features of the Ces`aro means. On the other hand, for series that have lacunary properties like those of $f ,$ the delayed means are essentially equal to the partial sums. In particular, note that for our function $f = f _ { \alpha }$ 

$$
S _ {N} (f) = \triangle_ {N ^ {\prime}} (f),\tag{6}
$$

where $N ^ { \prime }$ is the largest integer of the form $2 ^ { k }$ with $N ^ { \prime } \leq N$ . This is clear by examining Figure 5 and the definition of $f$ . 

We turn to the proof of the theorem proper and argue by contradiction; that is, we assume that $f ^ { \prime } ( x _ { 0 } )$ exists for some $x _ { 0 }$ 

Lemma 3.2 Let g be any continuous function that is diferentiable at $x _ { 0 }$ . Then, the Ces`aro means satisfy $\sigma _ { N } ( g ) ^ { \prime } ( x _ { 0 } ) = { \cal O } ( \log N )$ , therefore 

$$
\triangle_ {N} (g) ^ {\prime} (x _ {0}) = O (\log N).
$$

Proof. First we have 

$$
\sigma_ {N} (g) ^ {\prime} (x _ {0}) = \int_ {- \pi} ^ {\pi} F _ {N} ^ {\prime} (x _ {0} - t) g (t) d t = \int_ {- \pi} ^ {\pi} F _ {N} ^ {\prime} (t) g (x _ {0} - t) d t,
$$

where $F _ { N }$ is the Fej´er kernel. Since $F _ { N }$ is periodic, we have $\textstyle \int _ { - \pi } ^ { \pi } F _ { N } ^ { \prime } ( t ) d t = 0$ and this implies that 

$$
\sigma_ {N} (g) ^ {\prime} (x _ {0}) = \int_ {- \pi} ^ {\pi} F _ {N} ^ {\prime} (t) [ g (x _ {0} - t) - g (x _ {0}) ] d t.
$$

From the assumption that $g$ is diferentiable at $x _ { 0 }$ we get 

$$
| \sigma_ {N} (g) ^ {\prime} (x _ {0}) | \leq C \int_ {- \pi} ^ {\pi} | F _ {N} ^ {\prime} (t) | | t | d t.
$$

Now observe that $F _ { N } ^ { \prime }$ satisfies the two estimates 

$$
| F _ {N} ^ {\prime} (t) | \leq A N ^ {2} \quad \mathrm{and} \quad | F _ {N} ^ {\prime} (t) | \leq \frac {A}{| t | ^ {2}}.
$$

For the first inequality, recall that $F _ { N }$ is a trigonometric polynomial of degree N whose coeficients are bounded by 1. Therefore, $F _ { N } ^ { \prime }$ is a trigonometric polynomial of degree N whose coeficients are no bigger than N. Hence $| F ^ { \prime } ( t ) | \le ( 2 N + 1 ) N \le A N ^ { 2 }$ 

## 3. A continuous but nowhere differentiable function

For the second inequality, we recall that 

$$
F _ {N} (t) = \frac {1}{N} \frac {\sin^ {2} (N t / 2)}{\sin^ {2} (t / 2)}.
$$

Diferentiating this expression, we get two terms: 

$$
\frac {\sin (N t / 2) \cos (N t / 2)}{\sin^ {2} (t / 2)} - \frac {1}{N} \frac {\cos (t / 2) \sin^ {2} (N t / 2)}{\sin^ {3} (t / 2)}.
$$

If we then use the facts that $| \sin ( N t / 2 ) | \le C N | t |$ and $| \sin ( t / 2 ) | \geq c | t |$ (for $| t | \leq \pi )$ , we get the desired estimates for $F _ { N } ^ { \prime } ( t )$ 

Using all of these estimates we find that 

$$
\begin{array}{l} | \sigma_ {N} (g) ^ {\prime} (x _ {0}) | \leq C \int_ {| t | \geq 1 / N} | F _ {N} ^ {\prime} (t) |   | t |   d t + C \int_ {| t | \leq 1 / N} | F _ {N} ^ {\prime} (t) |   | t |   d t \\ \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \\ \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \qquad \q
$$

The proof of the lemma is complete once we invoke the definition of $\triangle _ { N } ( g )$ 

Lemma 3.3 $I f 2 N = 2 ^ { n }$ , then 

$$
\triangle_ {2 N} (f) - \triangle_ {N} (f) = 2 ^ {- n \alpha} e ^ {i 2 ^ {n} x}.
$$

This follows from our previous observation (6) because $\triangle _ { 2 N } ( f ) =$ $S _ { 2 N } ( f )$ and $\triangle _ { N } ( f ) = S _ { N } ( f )$ 

Now, by the first lemma we have 

$$
\triangle_ {2 N} (f) ^ {\prime} \left(x _ {0}\right) - \triangle_ {N} (f) ^ {\prime} \left(x _ {0}\right) = O (\log N),
$$

and the second lemma also implies 

$$
| \triangle_ {2 N} (f) ^ {\prime} (x _ {0}) - \triangle_ {N} (f) ^ {\prime} (x _ {0}) | = 2 ^ {n (1 - \alpha)} \geq c N ^ {1 - \alpha}.
$$

This is the desired contradiction since $N ^ { 1 - \alpha }$ grows faster than log $N .$ . 

A few additional remarks about our function $\begin{array} { r } { f _ { \alpha } ( x ) = \sum _ { n = 0 } ^ { \infty } 2 ^ { - n \alpha } e ^ { i 2 ^ { n } x } } \end{array}$ are in order. 

This function is complex-valued as opposed to the examples R and $W$ above, and so the nowhere diferentiability of $f _ { \alpha }$ does not imply the same property for its real and imaginary parts. However, a small modification of our proof shows that, in fact, the real part of $f _ { \alpha }$ 

$$
\sum_ {n = 0} ^ {\infty} 2 ^ {- n \alpha} \cos 2 ^ {n} x,
$$

as well as its imaginary part, are both nowhere diferentiable. To see this, observe first that by the same proof, Lemma 3.2 has the following generalization: if $g$ is a continuous function which is diferentiable at $x _ { 0 } ,$ then 

$$
\triangle_ {N} (g) ^ {\prime} \left(x _ {0} + h\right) = O (\log N) \quad \text { whenever } | h | \leq c / N.
$$

We then proceed with $\textstyle F ( x ) = \sum _ { n = 0 } ^ { \infty } 2 ^ { - n \alpha }$ cos $2 ^ { n } x$ , noting as above that $\triangle _ { 2 N } ( F ) - \triangle _ { N } ( F ) = 2 ^ { - n \alpha }$ cos $2 ^ { n } x ;$ as a result, assuming that $F$ is diferentiable at $x _ { 0 }$ , we get that 

$$
| 2 ^ {n (1 - \alpha)} \sin (2 ^ {n} (x _ {0} + h)) | = O (\log N)
$$

when $2 N = 2 ^ { n }$ , and $| h | \leq c / N$ . To get a contradiction, we need only choose h so that $| \sin ( 2 ^ { n } ( x _ { 0 } + h ) ) | = 1 ;$ this is accomplished by setting δ equal to the distance from $2 ^ { n } x _ { 0 }$ to the nearest number of the form $( k + 1 / 2 ) \pi , k \in \mathbb { Z } { \mathrm { ~ ( s o ~ } } \delta \leq \pi / 2 )$ , and taking $h = \pm \delta / 2 ^ { n }$ 

Clearly, when $\alpha > 1$ the function $f _ { \alpha }$ is continuously diferentiable since the series can be diferentiated term by term. Finally, the nowhere differentiability we have proved for $\alpha < 1$ actually extends to $\alpha = 1$ by a suitable refinement of the argument (see Problem 8 in Chapter 5). In fact, using these more elaborate methods one can also show that the Weierstrass function W is nowhere diferentiable if $a b \geq 1$ 

## 4 The heat equation on the circle

As a final illustration, we return to the original problem of heat difusion considered by Fourier. 

Suppose we are given an initial temperature distribution at $t = 0$ on a ring and that we are asked to describe the temperature at points on the ring at times $t > 0$ 

The ring is modeled by the unit circle. A point on this circle is described by its angle $\theta = 2 \pi x$ , where the variable x lies between 0 and 1. If $u ( x , t )$ denotes the temperature at time t of a point described by the 

## 4. The heat equation on the circle

angle θ, then considerations similar to the ones given in Chapter 1 show that u satisfies the diferential equation 

$$
\frac {\partial u}{\partial t} = c \frac {\partial^ {2} u}{\partial x ^ {2}}.\tag{7}
$$

The constant c is a positive physical constant which depends on the material of which the ring is made (see Section 2.1 in Chapter 1). After rescaling the time variable, we may assume that $c = 1$ . If f is our initial data, we impose the condition 

$$
u (x, 0) = f (x).
$$

To solve the problem, we separate variables and look for special solutions of the form 

$$
u (x, t) = A (x) B (t).
$$

Then inserting this expression for u into the heat equation we get 

$$
\frac {B ^ {\prime} (t)}{B (t)} = \frac {A ^ {\prime \prime} (x)}{A (x)}.
$$

Both sides are therefore constant, say equal to λ. Since A must be periodic of period 1, we see that the only possibility is $\lambda = - 4 \pi ^ { 2 } n ^ { 2 }$ where $n \in \mathbb { Z }$ . Then A is a linear combination of the exponentials e<sup>2πinx</sup> and $e ^ { - 2 \pi i n x }$ , and $B ( t )$ is a multiple of $e ^ { - 4 \pi ^ { 2 } n ^ { 2 } t }$ . By superposing these solutions, we are led to 

$$
u (x, t) = \sum_ {n = - \infty} ^ {\infty} a _ {n} e ^ {- 4 \pi^ {2} n ^ {2} t} e ^ {2 \pi i n x},\tag{8}
$$

where, setting $t = 0 ,$ we see that $\left\{ a _ { n } \right\}$ are the Fourier coeficients of $f .$ Note that when f is Riemann integrable, the coeficients $a _ { n }$ are bounded, and since the factor $e ^ { - 4 \pi ^ { 2 } n ^ { 2 } t }$ tends to zero extremely fast, the series defining u converges. In fact, in this case, u is twice diferentiable and solves equation (7). 

The natural question with regard to the boundary condition is the following: do we have $u ( x , t ) \to f ( x )$ as t tends to 0, and in what sense? A simple application of the Parseval identity shows that this limit holds in the mean square sense (Exercise 11). For a better understanding of the properties of our solution (8), we write it as 

$$
u (x, t) = (f * H _ {t}) (x),
$$

where $H _ { t }$ is the heat kernel for the circle, given by 

$$
H _ {t} (x) = \sum_ {n = - \infty} ^ {\infty} e ^ {- 4 \pi^ {2} n ^ {2} t} e ^ {2 \pi i n x},\tag{9}
$$

and where the convolution for functions with period 1 is defined by 

$$
(f * g) (x) = \int_ {0} ^ {1} f (x - y) g (y) d y.
$$

An analogy between the heat kernel and the Poisson kernel (of Chapter 2) is given in Exercise 12. However, unlike in the case of the Poisson kernel, there is no elementary formula for the heat kernel. Nevertheless, it turns out that it is a good kernel (in the sense of Chapter 2). The proof is not obvious and requires the use of the celebrated Poisson summation formula, which will be taken up in Chapter 5. As a corollary, we will also find that $H _ { t }$ is everywhere positive, a fact that is also not obvious from its defining expression (9). We can, however, give the following heuristic argument for the positivity of $H _ { t } .$ . Suppose that we begin with an initial temperature distribution f which is everywhere $\leq 0$ . Then it is physically reasonable to expect $u ( x , t ) \leq 0$ for all t since heat travels from hot to cold. Now 

$$
u (x, t) = \int_ {0} ^ {1} f (x - y) H _ {t} (y) d y.
$$

If $H _ { t }$ is negative for some $x _ { 0 }$ , then we may choose $f \leq 0$ supported near $x _ { 0 }$ , and this would imply $u ( x _ { 0 } , t ) > 0$ , which is a contradiction. 

## 5 Exercises

1. Let $\gamma : [ a , b ] \to \mathbb { R } ^ { 2 }$ be a parametrization for the closed curve Γ. 

(a) Prove that γ is a parametrization by arc-length if and only if the length of the curve from $\gamma ( a )$ to $\gamma ( s )$ is precisely $s - a$ , that is, 

$$
\int_ {a} ^ {s} | \gamma^ {\prime} (t) | d t = s - a.
$$

(b) Prove that any curve Γ admits a parametrization by arc-length. [Hint: If η is any parametrization, let $\begin{array} { r } { h ( s ) = \int _ { a } ^ { s } | \eta ^ { \prime } ( t ) | } \end{array}$ dt and consider $\gamma = \overset { \cdot } { \eta } \circ h ^ { - 1 } . ]$ 

2. Suppose $\gamma : [ a , b ] \to \mathbb { R } ^ { 2 }$ is a parametrization for a closed curve $\Gamma ,$ with $\gamma ( t ) = ( x ( t ) , y ( t ) )$ 

5. Exercises 

(a) Show that 

$$
\frac {1}{2} \int_ {a} ^ {b} (x (s) y ^ {\prime} (s) - y (s) x ^ {\prime} (s)) d s = \int_ {a} ^ {b} x (s) y ^ {\prime} (s) d s = - \int_ {a} ^ {b} y (s) x ^ {\prime} (s) d s.
$$

(b) Define the reverse parametrization of $\gamma$ by $\gamma ^ { - } : [ a , b ] \to \mathbb { R } ^ { 2 }$ with $\gamma ^ { - } ( t ) = \gamma ( b + a - t )$ . The image of $\gamma ^ { - }$ is precisely $\Gamma ,$ except that the points $\gamma ^ { - } ( t )$ and $\gamma ( t )$ travel in opposite directions. Thus $\gamma ^ { - }$ “reverses” the orientation of the curve. Prove that 

$$
\int_ {\gamma} (x d y - y d x) = - \int_ {\gamma^ {-}} (x d y - y d x).
$$

In particular, we may assume (after a possible change in orientation) that 

$$
\mathcal {A} = \frac {1}{2} \int_ {a} ^ {b} (x (s) y ^ {\prime} (s) - y (s) x ^ {\prime} (s)) d s = \int_ {a} ^ {b} x (s) y ^ {\prime} (s) d s.
$$

3. Suppose Γ is a curve in the plane, and that there exists a set of coordinates x and y so that the x-axis divides the curve into the union of the graph of two continuous functions $y = f ( x )$ and $y = g ( x )$ for $0 \leq x \leq 1$ , and with $f ( x ) \geq$ $g ( x )$ (see Figure 6). Let Ω denote the region between the graphs of these two functions: 

$$
\Omega = \{(x, y): 0 \leq x \leq 1 \text {and} g (x) \leq y \leq f (x) \}.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/624f5ed65ecd3046cc351bcb167a09ff251b614a94fdcec371aadcd7d910959d.jpg)



Figure 6. Simple version of the area formula


With the familiar interpretation that the integral $\textstyle \int h ( x )$ dx gives the area under the graph of the function $h ,$ we see that the area of Ω is $\textstyle \int _ { 0 } ^ { 1 } f ( x )$ dx − $\textstyle \int _ { 0 } ^ { 1 } g ( x ) d x$ . Show that this definition coincides with the area formula A given in the text, that is, 

$$
\int_ {0} ^ {1} f (x) d x - \int_ {0} ^ {1} g (x) d x = \left| - \int_ {\Gamma} y d x \right| = \mathcal {A}.
$$

Also, note that if the orientation of the curve is chosen so that Ω “lies to the left” of Γ, then the above formula holds without the absolute value signs. 

This formula generalizes to any set that can be written as a finite union of domains like Ω above. 

4. Observe that with the definition of ` and A given in the text, the isoperimetric inequality continues to hold (with the same proof) even when Γ is not simple. 

Show that this stronger version of the isoperimetric inequality is equivalent to Wirtinger’s inequality, which says that if f is 2π-periodic, of class $C ^ { 1 }$ , and satisfies $\begin{array} { r } { \int _ { 0 } ^ { \infty } f ( t ) d t = 0 } \end{array}$ , then 

$$
\int_ {0} ^ {2 \pi} | f (t) | ^ {2} d t \leq \int_ {0} ^ {2 \pi} | f ^ {\prime} (t) | ^ {2} d t
$$

with equality if and only if $f ( t ) = A \sin t + B$ cos t (Exercise 11, Chapter 3). 

[Hint: In one direction, note that if the length of the curve is 2π and $\gamma$ is an appropriate arc-length parametrization, then 

$$
2 (\pi - \mathcal {A}) = \int_ {0} ^ {2 \pi} \left[ x ^ {\prime} (s) + y (s) \right] ^ {2} d s + \int_ {0} ^ {2 \pi} \left(y ^ {\prime} (s) ^ {2} - y (s) ^ {2}\right) d s.
$$

A change of coordinates will guarantee $\begin{array} { r } { \int _ { 0 } ^ { 2 \pi } y ( s ) d s = 0 } \end{array}$ . For the other direction, start with a real-valued $f$ satisfying all the hypotheses of Wirtinger’s inequality, and construct $^ { g , }$ 2π-periodic and so that the term in brackets above vanishes.] 

5. Prove that the sequence $\{ \gamma _ { n } \} _ { n = 1 } ^ { \infty } .$ , where $\gamma _ { n }$ is the fractional part of 

$$
\left(\frac {1 + \sqrt {5}}{2}\right) ^ {n},
$$

is not equidistributed in [0, 1]. 

[Hint: Show that $\begin{array} { r } { U _ { n } = \left( \frac { 1 + \sqrt { 5 } } { 2 } \right) ^ { n } + \left( \frac { 1 - \sqrt { 5 } } { 2 } \right) ^ { n } } \end{array}$ is the solution of the diference equation $U _ { r + 1 } = U _ { r } + U _ { r - 1 } \ '$ with $U _ { 0 } \dot { = } 2$ and $U _ { 1 } = 1$ . The $U _ { n }$ satisfy the same diference equation as the Fibonacci numbers.] 

6. Let $\theta = p / q$ be a rational number where $p$ and q are relatively prime integers (that is, θ is in lowest form). We assume without loss of generality that $q > 0$ . Define a sequence of numbers in [0, 1) by $\xi _ { n } = \langle n \theta \rangle$ where $\langle \cdot \rangle$ denotes the 

## 5. Exercises

fractional part. Show that the sequence $\left\{ \xi _ { 1 } , \xi _ { 2 } , \ldots \right\}$ is equidistributed on the points of the form 

$$
0, 1 / q, 2 / q, \dots , (q - 1) / q.
$$

In fact, prove that for any $0 \leq a < q .$ , one has 

$$
\frac {\# \{n : 1 \leq n \leq N , \langle n \theta \rangle = a / q \}}{N} = \frac {1}{q} + O \left(\frac {1}{N}\right).
$$

[Hint: For each integer $k \geq 0 ,$ , there exists a unique integer n with kq $\leq n < ( k +$ 1)q and so that $\langle n \theta \rangle = a / q$ . Why can one assume $k = 0 ?$ Prove the existence of n by using the fact<sup>1</sup> that if p and q are relatively prime, there exist integers x, y such that $x p + y q = 1$ . Next, divide $N$ by $q$ with remainder, that is, write $N = \ell q + r$ where $0 \leq \ell$ and $0 \leq r < q$ . Establish the inequalities 

$$
\ell \leq \# \{n: 1 \leq n \leq N, \langle n \theta \rangle = a / q \} \leq \ell + 1. ]
$$

7. Prove the second part of Weyl’s criterion: if a sequence of numbers $\xi _ { 1 } , \xi _ { 2 } , \ldots .$ in [0, 1) is equidistributed, then for all $k \in \mathbb { Z } - \{ 0 \}$ 

$$
\frac {1}{N} \sum_ {n = 1} ^ {N} e ^ {2 \pi i k \xi_ {n}} \rightarrow 0 \quad \text { as } N \rightarrow \infty .
$$

[Hint: It sufices to show that $\begin{array} { r } { \frac { 1 } { N } \sum _ { n = 1 } ^ { N } f ( \xi _ { n } ) \to \int _ { 0 } ^ { 1 } f ( x ) } \end{array}$ dx for all continuous $f .$ Prove this first when $f$ is the characteristic function of an interval.] 

8. Show that for any $a \neq 0$ , and σ with $0 < \sigma < 1$ , the sequence $\left. a n ^ { \sigma } \right.$ is equidistributed in $[ 0 , 1 )$ 

[Hint: Prove that $\begin{array} { r } { \sum _ { n = 1 } ^ { N } e ^ { 2 \pi i b n ^ { \sigma } } = O ( N ^ { \sigma } ) + O ( N ^ { 1 - \sigma } ) } \end{array}$ if $b \neq 0 . ]$ In fact, note the following 

$$
\sum_ {n = 1} ^ {N} e ^ {2 \pi i b n ^ {\sigma}} - \int_ {1} ^ {N} e ^ {2 \pi i b x ^ {\sigma}} d x = O \left(\sum_ {n = 1} ^ {N} n ^ {- 1 + \sigma}\right).
$$

9. In contrast with the result in Exercise $^ { 8 , }$ prove that $\left. a \log n \right.$ is not equidistributed for any a. 

[Hint: Compare the sum $\textstyle \sum _ { n = 1 } ^ { N }$ e<sup>2πib</sup> <sup>log</sup> <sup>n</sup> with the corresponding integral.] 

10. Suppose that f is a periodic function on R of period 1, and $\left\{ \xi _ { n } \right\}$ is a sequence which is equidistributed in [0, 1). Prove that: 

(a) If $f$ is continuous and satisfies $\begin{array} { r } { \int _ { 0 } ^ { 1 } f ( x ) d x = 0 } \end{array}$ , then 

$$
\lim _ {N \to \infty} \frac {1}{N} \sum_ {n = 1} ^ {N} f (x + \xi_ {n}) = 0 \quad \text { uniformly   in } x.
$$

[Hint: Establish this result first for trigonometric polynomials.] 

(b) If $f$ is merely integrable on [0, 1] and satisfies $\begin{array} { r } { \int _ { 0 } ^ { 1 } f ( x ) d x = 0 } \end{array}$ , then 

$$
\lim _ {N \to \infty} \int_ {0} ^ {1} \left| \frac {1}{N} \sum_ {n = 1} ^ {N} f (x + \xi_ {n}) \right| ^ {2} d x = 0.
$$

11. Show that if $u ( x , t ) = ( f * H _ { t } ) ( x )$ where $H _ { t }$ is the heat kernel, and $f$ is Riemann integrable, then 

$$
\int_ {0} ^ {1} | u (x, t) - f (x) | ^ {2} d x \to 0 \quad \mathrm{as} t \to 0.
$$

12. A change of variables in (8) leads to the solution 

$$
u (\theta , \tau) = \sum a _ {n} e ^ {- n ^ {2} \tau} e ^ {i n \theta} = (f * h _ {\tau}) (\theta)
$$

of the equation 

$$
\frac {\partial u}{\partial \tau} = \frac {\partial^ {2} u}{\partial \theta^ {2}} \quad \mathrm{with} 0 \leq \theta \leq 2 \pi \mathrm{and} \tau > 0,
$$

with boundary condition $\begin{array} { r } { u ( \theta , 0 ) = f ( \theta ) \sim \sum a _ { n } e ^ { i n \theta } , } \end{array}$ Here $h _ { \tau } ( \theta ) =$ $\scriptstyle \sum _ { n = - \infty } ^ { \infty } e ^ { - n ^ { 2 } \tau } e ^ { i n \theta }$ . This version of the heat kernel on $[ 0 , 2 \pi ]$ is the analogue of the Poisson kernel, which can be written as $\begin{array} { r } { P _ { r } ( \theta ) = \sum _ { n = - \infty } ^ { \infty } e ^ { - | n | \tau } e ^ { i n \theta } } \end{array}$ with $r = e ^ { - \tau }$ (and so $0 < r < 1$ corresponds to $\tau > 0 )$ ). 

13. The fact that the kernel $H _ { t } ( x )$ is a good kernel, hence $u ( x , t ) \to f ( x )$ at each point of continuity of $f ,$ is not easy to prove. This will be shown in the next chapter. However, one can prove directly that $H _ { t } ( x )$ is “peaked” at $x = 0$ as $t \to 0$ in the following sense: 

(a) Show that $\int _ { - 1 / 2 } ^ { 1 / 2 } | H _ { t } ( x ) | ^ { 2 }$ dx is of the order of magnitude of $t ^ { - 1 / 2 }$ as $t \longrightarrow 0$ More precisely, prove that $t ^ { 1 / 2 } \int _ { - 1 / 2 } ^ { 1 / 2 } | H _ { t } ( x ) | ^ { 2 }$ dx converges to a non-zero limit as $t \longrightarrow 0$ 

(b) Prove that $\begin{array} { r } { \int _ { - 1 / 2 } ^ { 1 / 2 } x ^ { 2 } | H _ { t } ( x ) | ^ { 2 } d x = O ( t ^ { 1 / 2 } ) ~ \mathrm { a s } ~ t  0 . } \end{array}$ 

## 6. Problems

[Hint: For (a) compare the sum $\textstyle \sum _ { - \infty } ^ { \infty } e ^ { - c n ^ { 2 } t }$ with the integral $\textstyle \int _ { - \infty } ^ { \infty } e ^ { - c x ^ { 2 } t } d x$ where $c > 0$ . For (b) use $x ^ { 2 } \leq C ( \sin \pi x ) ^ { 2 }$ for $- 1 / 2 \le x \le 1 / 2$ , and apply the mean value theorem to $e ^ { - c x ^ { 2 } t } . ]$ 

## 6 Problems

1.<sup>∗</sup> This problem explores another relationship between the geometry of a curve and Fourier series. The diameter of a closed curve Γ parametrized by $\gamma ( t ) = ( x ( t ) , y ( t ) )$ on $[ - \pi , \pi ]$ is defined by 

$$
d = \sup _ {P, Q \in \Gamma} | P - Q | = \sup _ {t _ {1}, t _ {2} \in [ - \pi , \pi ]} | \gamma (t _ {1}) - \gamma (t _ {2}) |.
$$

If $a _ { n }$ is the $n ^ { \mathrm { t h } }$ Fourier coeficient of $\gamma ( t ) = x ( t ) + i y ( t )$ and ` denotes the length of $\Gamma ,$ then 

(a) $2 | a _ { n } | \leq d$ for all $n \neq 0 .$ 

(b) $\ell \leq \pi d ,$ , whenever $\Gamma$ is convex. 

Property (a) follows from the fact that $\begin{array} { r } { 2 a _ { n } = \frac { 1 } { 2 \pi } \int _ { - \pi } ^ { \pi } [ \gamma ( t ) - \gamma ( t + \pi / n ) ] e ^ { - i n t } d t } \end{array}$ 

The equality $\ell = \pi d$ is satisfied when Γ is a circle, but surprisingly, this is not the only case. In fact, one finds that $\ell = \pi d$ is equivalent to $2 | a _ { 1 } | = d$ . We re-parametrize γ so that for each t in $[ - \pi , \pi ]$ the tangent to the curve makes an angle t with the y-axis. Then, if $a _ { 1 } = 1$ we have 

$$
\gamma^ {\prime} (t) = i e ^ {i t} (1 + r (t)),
$$

where r is a real-valued function which satisfies $r ( t ) + r ( t + \pi ) = 0$ , and $| r ( t ) | \leq 1$ . Figure $7 \ \mathrm { ( a ) }$ shows the curve obtained by setting $r ( t ) = \cos { 5 t }$ . Also, Figure $7 \ ( \mathrm { b } )$ consists of the curve where $r ( t ) = h ( 3 t )$ , with $h ( s ) = - 1 { \mathrm { ~ i f ~ } } - \pi \leq$ $s \leq 0$ and $h ( s ) = 1 { \mathrm { ~ i f ~ } } 0 < s < \pi$ . This curve (which is only piecewise of class $C ^ { 1 } )$ is known as the Reuleaux triangle and is the classical example of a convex curve of constant width which is not a circle. 

2.<sup>∗</sup> Here we present an estimate of Weyl which leads to some interesting results. 

(a) Let $\begin{array} { r } { S _ { N } = \sum _ { n = 1 } ^ { N } e ^ { 2 \pi i f ( n ) } } \end{array}$ . Show that for $H \leq N$ , one has 

$$
\left| S _ {N} \right| ^ {2} \leq c \frac {N}{H} \sum_ {h = 0} ^ {H} \left| \sum_ {n = 1} ^ {N - h} e ^ {2 \pi i (f (n + h) - f (n))} \right|,
$$

for some constant $c > 0$ independent of N, H, and $f .$ 

(b) Use this estimate to show that the sequence $\langle n ^ { 2 } \gamma \rangle$ is equidistributed in [0, 1) whenever γ is irrational. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/7f19b1a5295edb954fe7089c5ec9d4a82ab1043304079fec77b286d461286cc4.jpg)



(a)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/46cb1f0645e7bb745faebd122f4724237eb2f659f5ff3e3942ee510a3d096d4a.jpg)



(b)



Figure 7. Some curves with maximal length for a given diameter


(c) More generally, show that if $\left\{ \xi _ { n } \right\}$ is a sequence of real numbers so that for all positive integers h the diference $\langle \xi _ { n + h } - \xi _ { n } \rangle$ is equidistributed in $[ 0 , 1 )$ , then $\langle \xi _ { n } \rangle$ is also equidistributed in $[ 0 , 1 )$ 

(d) Suppose that $P ( x ) = c _ { n } x ^ { n } + \cdot \cdot \cdot + c _ { 0 }$ is a polynomial with real coeficients, where at least one of $c _ { 1 } , \ldots , c _ { n }$ is irrational. Then the sequence $\langle P ( n ) \rangle$ is equidistributed in [0, 1). 

[Hint: For (a), let $a _ { n } = e ^ { 2 \pi i f ( n ) }$ when $1 \leq n \leq N$ and 0 otherwise. Then write $\begin{array} { r } { H \sum _ { n } a _ { n } = \sum _ { k = 1 } ^ { H } \sum _ { n } a _ { \underline { { n } } + k } } \end{array}$ and apply the Cauchy-Schwarz inequality. For (b), note that $( n \overline { { + } } \tilde { h } ) ^ { 2 } \overline { { \gamma - } } n ^ { 2 } \gamma = 2 n h \gamma + h ^ { 2 } \gamma$ , and use the fact that for each integer $h ,$ the sequence $\langle 2 n h \gamma \rangle$ is equidistributed. Finally, to prove $\mathrm { ( d ) }$ , assume first that $P ( x ) = Q ( x ) + c _ { 1 } x + c _ { 0 }$ where $c _ { 1 }$ is irrational, and estimate the exponential sum $\scriptstyle \sum _ { n = 1 } ^ { N } e ^ { 2 \pi i k P ( n ) }$ . Then, argue by induction on the highest degree term which has an irrational coeficient, and use part (c).] 

3.<sup>∗</sup> If $\sigma > 0$ is not an integer and $a \neq 0$ , then $\left. a n ^ { \sigma } \right.$ is equidistributed in $[ 0 , 1 )$ See also Exercise 8. 

4. An elementary construction of a continuous but nowhere diferentiable function is obtained by “piling up singularities,” as follows. 

On [−1, 1] consider the function 

$$
\varphi (x) = | x |
$$

and extend $\varphi$ to R by requiring it to be periodic of period 2. Clearly, $\varphi$ is continuous on R and $| \varphi ( x ) | \leq 1$ for all x so the function $f$ defined by 

$$
f (x) = \sum_ {n = 0} ^ {\infty} \left(\frac {3}{4}\right) ^ {n} \varphi (4 ^ {n} x)
$$

is continuous on $\mathbb { R } .$ 

6. Problems 

(a) Fix $x _ { 0 } \in \mathbb { R }$ . For every positive integer $m ,$ let $\delta _ { m } = \pm \frac { 1 } { 2 } 4 ^ { - m }$ where the sign is chosen so that no integer lies in between $4 ^ { m } x _ { 0 }$ and $4 ^ { m } ( x _ { 0 } + \delta _ { m } )$ Consider the quotient 

$$
\gamma_ {n} = \frac {\varphi (4 ^ {n} (x _ {0} + \delta_ {m})) - \varphi (4 ^ {n} x _ {0})}{\delta_ {m}}.
$$

Prove that if $n > m$ , then $\gamma _ { n } = 0$ , and for $0 \leq n \leq m$ one has $| \gamma _ { n } | \leq 4 ^ { n }$ with $| \gamma _ { m } | = 4 ^ { m }$ 

(b) From the above observations prove the estimate 

$$
\left| \frac {f (x _ {0} + \delta_ {m}) - f (x _ {0})}{\delta_ {m}} \right| \geq \frac {1}{2} (3 ^ {m} + 1),
$$

and conclude that $f$ is not diferentiable at $x _ { 0 }$ 

5. Let $f$ be a Riemann integrable function on the interval $[ - \pi , \pi ]$ . We define the generalized delayed means of the Fourier series of $f$ by 

$$
\sigma_ {N, K} = \frac {S _ {N} + \cdots + S _ {N + K - 1}}{K}.
$$

Note that in particular 

$$
\sigma_ {0, N} = \sigma_ {N}, \quad \sigma_ {N, 1} = S _ {N} \quad \mathrm{and} \quad \sigma_ {N, N} = \Delta_ {N},
$$

where $\Delta _ { N }$ are the specific delayed means used in Section $3 .$ 

(a) Show that 

$$
\sigma_ {N, K} = \frac {1}{K} \left((N + K) \sigma_ {N + K} - N \sigma_ {N}\right),
$$

and 

$$
\sigma_ {N, K} = S _ {N} + \sum_ {N + 1 \leq | \nu | \leq N + K - 1} \left(1 - \frac {| \nu | - N}{K}\right) \hat {f} (\nu) e ^ {i \nu \theta}.
$$

From this last expression for $\sigma _ { N , K }$ conclude that 

$$
| \sigma_ {N, K} - S _ {M} | \leq \sum_ {N + 1 \leq | \nu | \leq N + K - 1} | \hat {f} (\nu) |
$$

for all $N \leq M < N + K$ 

(b) Use one of the above formulas and Fej´er’s theorem to show that with $N = k n$ and $K = n$ , then 

$$
\sigma_ {k n, n} (f) (\theta) \rightarrow f (\theta) \quad \mathrm{as} n \rightarrow \infty
$$

whenever f is continuous at θ, and also 

$$
\sigma_ {k n, n} (f) (\theta) \rightarrow \frac {f (\theta^ {+}) + f (\theta^ {-})}{2} \quad \mathrm{as} n \rightarrow \infty
$$

at a jump discontinuity (refer to the preceding chapters and their exercises for the appropriate definitions and results). In the case when $f$ is continuous on $[ - \pi , \pi ]$ , show that $\sigma _ { k n , n } ( f ) \to f$ uniformly as $n \to \infty$ 

(c) Using part (a), show that if ${ \hat { f } } ( \nu ) = O ( 1 / | \nu | )$ and $k n \leq m < ( k + 1 ) n$ , we get 

$$
\left| \sigma_ {k n, n} - S _ {m} \right| \leq \frac {C}{k} \quad \text {   for   some   constant   } C > 0.
$$

(d) Suppose that ${ \hat { f } } ( \nu ) = O ( 1 / | \nu | )$ . Prove that if $f$ is continuous at θ then 

$$
S _ {N} (f) (\theta) \to f (\theta) \quad \mathrm{as} N \to \infty ,
$$

and if f has a jump discontinuity at θ then 

$$
S _ {N} (f) (\theta) \to \frac {f (\theta^ {+}) + f (\theta^ {-})}{2} \quad \text { as } N \to \infty .
$$

Also, show that if f is continuous on $[ - \pi , \pi ]$ , then $S _ { N } ( f ) \to f$ uniformly. 

(e) The above arguments show that $\operatorname { i f } \sum c _ { n }$ is Ces`aro summable to s and $c _ { n } =$ $O ( 1 / n )$ , then $\sum c _ { n }$ converges to s. This is a weak version of Littlewood’s theorem (Problem 3, Chapter 2). 

6. Dirichlet’s theorem states that the Fourier series of a real continuous periodic function f which has only a finite number of relative maxima and minima converges everywhere to f (and uniformly). 

Prove this theorem by showing that such a function satisfies ${ \hat { f } } ( n ) = O ( 1 / | n | )$ [Hint: Argue as in Exercise 17, Chapter 3; then use conclusion (d) in Problem 5 above.] 

# 5 <sub>The</sub> <sub>Fourier</sub> <sub>Transform</sub> <sub>on</sub> R

The theory of Fourier series and integrals has always had major dificulties and necessitated a large mathematical apparatus in dealing with questions of convergence. It engendered the development of methods of summation, although these did not lead to a completely satisfactory solution of the problem.. . . For the Fourier transform, the introduction of distributions (hence the space S) is inevitable either in an explicit or hidden form.. . . As a result one may obtain all that is desired from the point of view of the continuity and inversion of the Fourier transform. 

L. Schwartz, 1950 

The theory of Fourier series applies to functions on the circle, or equivalently, periodic functions on R. In this chapter, we develop an analogous theory for functions on the entire real line which are non-periodic. The functions we consider will be suitably “small” at infinity. There are several ways of defining an appropriate notion of “smallness,” but it will nevertheless be vital to assume some sort of vanishing at infinity. 

On the one hand, recall that the Fourier series of a periodic function associates a sequence of numbers, namely the Fourier coeficients, to that function; on the other hand, given a suitable function f on R, the analogous object associated to f will in fact be another function $\hat { f }$ on R which is called the Fourier transform of $f .$ . Since the Fourier transform of a function on R is again a function on R, one can observe a symmetry between a function and its Fourier transform, whose analogue is not as apparent in the setting of Fourier series. 

Roughly speaking, the Fourier transform is a continuous version of the Fourier coeficients. Recall that the Fourier coeficients $a _ { n }$ of a function f defined on the circle are given by 

$$
a _ {n} = \int_ {0} ^ {1} f (x) e ^ {- 2 \pi i n x} d x,\tag{1}
$$

and then in the appropriate sense we have 

$$
f (x) = \sum_ {n = - \infty} ^ {\infty} a _ {n} e ^ {2 \pi i n x}.\tag{2}
$$

Here we have replaced θ by 2πx, as we have frequently done previously. 

Now, consider the following analogy where we replace all of the discrete symbols (such as integers and sums) by their continuous counterparts (such as real numbers and integrals). In other words, given a function f on all of R, we define its Fourier transform by changing the domain of integration from the circle to all of R, and by replacing $n \in \mathbb { Z }$ by $\xi \in \mathbb { R }$ in (1), that is, by setting 

$$
\hat {f} (\xi) = \int_ {- \infty} ^ {\infty} f (x) e ^ {- 2 \pi i x \xi} d x.\tag{3}
$$

We push our analogy further, and consider the following continuous version of (2): replacing the sum by an integral, and $a _ { n }$ by ${ \hat { f } } ( \xi )$ , leads to the Fourier inversion formula, 

$$
f (x) = \int_ {- \infty} ^ {\infty} \hat {f} (\xi) e ^ {2 \pi i x \xi} d \xi .\tag{4}
$$

Under a suitable hypotheses on $f ,$ the identity (4) actually holds, and much of the theory in this chapter aims at proving and exploiting this relation. The validity of the Fourier inversion formula is also suggested by the following simple observation. Suppose f is supported in a finite interval contained in $I = [ - L / 2 , L / 2 ]$ , and we expand f in a Fourier series on I. Then, letting L tend to infinity, we are led to (4) (see Exercise 1). 

The special properties of the Fourier transform make it an important tool in the study of partial diferential equations. For instance, we shall see how the Fourier inversion formula allows us to analyze some equations that are modeled on the real line. In particular, following the ideas developed on the circle, we solve the time-dependent heat equation for an infinite rod and the steady-state heat equation in the upper half-plane. 

In the last part of the chapter we discuss further topics related to the Poisson summation formula, 

$$
\sum_ {n \in \mathbb {Z}} f (n) = \sum_ {n \in \mathbb {Z}} \hat {f} (n),
$$

which gives another remarkable connection between periodic functions (and their Fourier series) and non-periodic functions on the line (and their Fourier transforms). This identity allows us to prove an assertion made in the previous chapter, namely, that the heat kernel $H _ { t } ( x )$ satisfies the properties of a good kernel. In addition, the Poisson summation formula arises in many other settings, in particular in parts of number theory, as we shall see in Book II. 

We make a final comment about the approach we have chosen. In our study of Fourier series, we found it useful to consider Riemann integrable functions on the circle. In particular, this generality assured us that even functions that had certain discontinuities could be treated by the theory. In contrast, our exposition of the elementary properties of the Fourier transform is stated in terms of the Schwartz space S of testing functions. These are functions that are indefinitely diferentiable and that, together with their derivatives, are rapidly decreasing at infinity. The reliance on this space of functions is a device that allows us to come quickly to the main conclusions, formulated in a direct and transparent fashion. Once this is carried out, we point out some easy extensions to a somewhat wider setting. The more general theory of Fourier transforms (which must necessarily be based on Lebesgue integration) will be treated in Book III. 

## 1 Elementary theory of the Fourier transform

We begin by extending the notion of integration to functions that are defined on the whole real line. 

## 1.1 Integration of functions on the real line

Given the notion of the integral of a function on a closed and bounded interval, the most natural extension of this definition to continuous functions over R is 

$$
\int_ {- \infty} ^ {\infty} f (x) d x = \lim _ {N \to \infty} \int_ {- N} ^ {N} f (x) d x.
$$

Of course, this limit may not exist. For example, it is clear that if $f ( x ) = 1$ , or even if $f ( x ) = 1 / ( 1 + | x | )$ , then the above limit is infinite. A moment’s reflection suggests that the limit will exist if we impose on $f$ enough decay as $| x |$ tends to infinity. A useful condition is as follows. 

A function $f$ defined on R is said to be of moderate decrease if $f$ is continuous and there exists a constant $A > 0$ so that 

$$
| f (x) | \leq \frac {A}{1 + x ^ {2}} \quad \mathrm{forall} x \in \mathbb {R}.
$$

This inequality says that f is bounded (by A for instance), and also that it decays at infinity at least as fast as $1 / x ^ { 2 }$ , since $A / ( 1 + x ^ { 2 } ) \leq A / x ^ { 2 }$ 

For example, the function $f ( x ) = 1 / ( 1 + | x | ^ { n } )$ is of moderate decrease as long as $n \geq 2$ . Another example is given by the function $e ^ { - a | x | }$ for $a > 0$ 

We shall denote by $\mathcal { M } ( \mathbb { R } )$ the set of functions of moderate decrease on R. As an exercise, the reader can check that under the usual addition of functions and multiplication by scalars, M(R) forms a vector space over C. 

We next see that whenever f belongs to $\mathcal { M } ( \mathbb { R } )$ , then we may define 

$$
\int_ {- \infty} ^ {\infty} f (x) d x = \lim _ {N \to \infty} \int_ {- N} ^ {N} f (x) d x,\tag{5}
$$

where the limit now exists. Indeed, for each N the integral $I _ { N } =$ $\textstyle \int _ { - N } ^ { N } f ( x )$ dx is well defined because f is continuous. It now sufices to show that $\left\{ { { I } _ { N } } \right\}$ is a Cauchy sequence, and this follows because if $M > N$ 2 then 

$$
\begin{array}{l} | I _ {M} - I _ {N} | \leq \left| \int_ {N \leq | x | \leq M} f (x)   d x \right| \\ \quad \leq A \int_ {N \leq | x | \leq M} \frac {d x}{x ^ {2}} \\ \quad \leq \frac {2 A}{N} \to 0 \quad \text { as } N \to \infty . \end{array}
$$

Notice we have also proved that $\scriptstyle \int _ { | x | \geq N } f ( x )$ dx → 0 as $N \to \infty$ . At this point, we remark that we may replace the exponent 2 in the definition of moderate decrease by $1 + \epsilon$ where $\epsilon > 0 ;$ that is, 

$$
| f (x) | \leq \frac {A}{1 + | x | ^ {1 + \epsilon}} \quad \text { for   all } x \in \mathbb {R}.
$$

This definition would work just as well for the purpose of the theory developed in this chapter. We chose $\epsilon = 1$ merely as a matter of conve nience. 

We summarize some elementary properties of integration over R in a proposition. 

Proposition 1.1 The integral of a function of moderate decrease defined by (5) satisfies the following properties: 

1. Elementary theory of the Fourier transform 

(i) Linearity: if $f , g \in { \mathcal { M } } ( \mathbb { R } )$ and $a , b \in \mathbb { C }$ , then 

$$
\int_ {- \infty} ^ {\infty} (a f (x) + b g (x)) d x = a \int_ {- \infty} ^ {\infty} f (x) d x + b \int_ {- \infty} ^ {\infty} g (x) d x.
$$

(ii) Translation invariance: for every $h \in \mathbb { R }$ we have 

$$
\int_ {- \infty} ^ {\infty} f (x - h) d x = \int_ {- \infty} ^ {\infty} f (x) d x.
$$

(iii) Scaling under dilations: if $\delta > 0$ , then 

$$
\delta \int_ {- \infty} ^ {\infty} f (\delta x) d x = \int_ {- \infty} ^ {\infty} f (x) d x.
$$

(iv) Continuity: if $f \in \mathcal { M } ( \mathbb { R } )$ , then 

$$
\int_ {- \infty} ^ {\infty} | f (x - h) - f (x) | d x \rightarrow 0 \quad a s h \rightarrow 0.
$$

We say a few words about the proof. Property (i) is immediate. To verify property (ii), it sufices to see that 

$$
\int_ {- N} ^ {N} f (x - h) d x - \int_ {- N} ^ {N} f (x) d x \to 0 \quad \text {as} N \to \infty .
$$

Since $\begin{array} { r } { \int _ { - N } ^ { N } f ( x - h ) d x = \int _ { - N - h } ^ { N - h } f ( x ) d  x } \end{array}$ x, the above diference is majorized by 

$$
\left| \int_ {- N - h} ^ {- N} f (x) d x \right| + \left| \int_ {N - h} ^ {N} f (x) d x \right| \leq \frac {A ^ {\prime}}{1 + N ^ {2}}
$$

for large N, which tends to 0 as N tends to infinity. 

The proof of property (iii) is similar once we observe that $\begin{array} { r l } { \delta \int _ { - N } ^ { N } f ( \delta x ) d x = } \end{array}$ $\textstyle \int _ { - \delta N } ^ { \delta N } f ( x ) d x$ 

To prove property (iv) it sufices to take $| h | \leq 1$ . For a preassigned $\epsilon > 0$ we first choose N so large that 

$$
\int_ {| x | \geq N} | f (x) | d x \leq \epsilon / 4 \quad \text {and} \quad \int_ {| x | \geq N} | f (x - h) | d x \leq \epsilon / 4.
$$

Now with N fixed, we use the fact that since f is continuous, it is uniformly continuous in the interval $[ - N - 1 , N + 1 ]$ Hence $\operatorname* { s u p } _ { | x | \leq N } | f ( x - h ) - f ( x ) | \to 0$ as $h$ tends to 0. $\mathrm { S o }$ we can take $h$ so small that this supremum is less than $\epsilon / 4 N$ . Altogether, then, 

$$
\begin{array}{r l} & {\int_ {- \infty} ^ {\infty} | f (x - h) - f (x) |   d x \leq \int_ {- N} ^ {N} | f (x - h) - f (x) |   d x} \\ & {\qquad + \int_ {| x | \geq N} | f (x - h) |   d x} \\ & {\qquad + \int_ {| x | \geq N} | f (x) |   d x} \\ & {\qquad \leq \epsilon / 2 + \epsilon / 4 + \epsilon / 4 = \epsilon ,} \end{array}
$$

and thus conclusion (iv) follows. 

## 1.2 Definition of the Fourier transform

If $f \in { \mathcal { M } } ( \mathbb { R } )$ , we define its Fourier transform for $\xi \in \mathbb { R }$ by 

$$
\hat {f} (\xi) = \int_ {- \infty} ^ {\infty} f (x) e ^ {- 2 \pi i x \xi} d x.
$$

Of course, $| e ^ { - 2 \pi i x \xi } | = 1$ , so the integrand is of moderate decrease, and the integral makes sense. 

In fact, this last observation implies that $\hat { f }$ is bounded, and moreover, a simple argument shows that $\hat { f }$ is continuous and tends to 0 as $| \xi | \to \infty$ (Exercise 5). However, nothing in the definition above guarantees that $\hat { f }$ is of moderate decrease, or has a specific decay. In particular, it is not clear in this context how to make sense of the integral $\textstyle { \int _ { - \infty } ^ { \infty } \hat { f } ( \xi ) e ^ { 2 \pi i x \xi } }$ dξ and the resulting Fourier inversion formula. To remedy this, we introduce a more refined space of functions considered by Schwartz which is very useful in establishing the initial properties of the Fourier transform. 

The choice of the Schwartz space is motivated by an important principle which ties the decay of $\hat { \hat { f } }$ to the continuity and diferentiability properties of $f$ (and vice versa): the faster $\hat { f } ( \xi )$ decreases as $| \xi | \to \infty ,$ the “smoother” f must be. An example that reflects this principle is given in Exercise 3. We also note that this relationship between f and $\hat { f }$ is reminiscent of a similar one between the smoothness of a function on the circle and the decay of its Fourier coeficients; see the discussion of Corollary 2.4 in Chapter 2. 

## 1.3 The Schwartz space

The Schwartz space on $\mathbb { R }$ consists of the set of all indefinitely diferentiable functions $f$ so that $f$ and all its derivatives $f ^ { \prime } , f ^ { \prime \prime } , \ldots , f ^ { ( \ell ) }$ 

1. Elementary theory of the Fourier transform 

are rapidly decreasing, in the sense that 

$$
\sup _ {x \in \mathbb {R}} | x | ^ {k} | f ^ {(\ell)} (x) | <   \infty \quad \text {   for   every   } k, \ell \geq 0.
$$

We denote this space by ${ \mathcal { S } } = { \mathcal { S } } ( \mathbb { R } )$ , and again, the reader should verify that $S ( \mathbb { R } )$ is a vector space over C. Moreover, if $f \in S ( \mathbb { R } )$ , we have 

$$
f ^ {\prime} (x) = \frac {d f}{d x} \in \mathcal {S} (\mathbb {R}) \quad \text { and } \quad x f (x) \in \mathcal {S} (\mathbb {R}).
$$

This expresses the important fact that the Schwartz space is closed under diferentiation and multiplication by polynomials. 

A simple example of a function in $S ( \mathbb { R } )$ is the Gaussian defined by 

$$
f (x) = e ^ {- x ^ {2}},
$$

which plays a central role in the theory of the Fourier transform, as well as other fields (for example, probability theory and physics). The reader can check that the derivatives of $f$ are of the form $\stackrel { \cdot } { P } ( x ) e ^ { - x ^ { 2 } }$ where $P$ is a polynomial, and this immediately shows that $f \in S ( \mathbb { R } )$ . In fact, $e ^ { - a x ^ { 2 } }$ belongs to $S ( \mathbb { R } )$ whenever $a > 0$ . Later, we will normalize the Gaussian by choosing $a = \pi$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/5041c09bfbee4b9f8c626a1bb27b9b4727b1af99bc6efeaca5a618ff05b459a7.jpg)



Figure 1. The Gaussian $e ^ { - \pi x ^ { 2 } }$


An important class of other examples in $S ( \mathbb { R } )$ are the “bump functions” which vanish outside bounded intervals (Exercise 4). 

As a final remark, note that although $e ^ { - | x | }$ decreases rapidly at infinity, it is not diferentiable at 0 and therefore does not belong to $S ( \mathbb { R } )$ 

## 1.4 The Fourier transform on $s$

The Fourier transform of a function $f \in S ( \mathbb { R } )$ is defined by 

$$
\hat {f} (\xi) = \int_ {- \infty} ^ {\infty} f (x) e ^ {- 2 \pi i x \xi} d x.
$$

Some simple properties of the Fourier transform are gathered in the following proposition. We use the notation 

$$
f (x) \longrightarrow \hat {f} (\xi)
$$

to mean that $\hat { f }$ denotes the Fourier transform of $f .$ 

Proposition 1.2 $I f \ f \in S ( \mathbb { R } )$ then: 

(i) $f ( x + h ) \longrightarrow { \hat { f } } ( \xi ) e ^ { 2 \pi i h \xi }$ whenever $h \in \mathbb { R }$ 

(ii) $f ( x ) e ^ { - 2 \pi i x h } \longrightarrow { \hat { f } } ( \xi + h )$ whenever $h \in \mathbb { R }$ 

(iii) $f ( \delta x ) \longrightarrow \delta ^ { - 1 } \hat { f } ( \delta ^ { - 1 } \xi )$ whenever $\delta > 0$ 

(iv) $f ^ { \prime } ( x ) \longrightarrow 2 \pi i \xi \hat { f } ( \xi )$ 

(v) $- 2 \pi i x f ( x ) \longrightarrow \frac { d } { d \xi } \hat { f } ( \xi ) .$ 

In particular, except for factors of 2πi, the Fourier transform interchanges diferentiation and multiplication by x. This is the key property that makes the Fourier transform a central object in the theory of diferential equations. We shall return to this point later. 

Proof. Property (i) is an immediate consequence of the translation invariance of the integral, and property (ii) follows from the definition. Also, the third property of Proposition 1.1 establishes (iii). 

Integrating by parts gives 

$$
\int_ {- N} ^ {N} f ^ {\prime} (x) e ^ {- 2 \pi i x \xi} d x = \left[ f (x) e ^ {- 2 \pi i x \xi} \right] _ {- N} ^ {N} + 2 \pi i \xi \int_ {- N} ^ {N} f (x) e ^ {- 2 \pi i x \xi} d x,
$$

so letting $N$ tend to infinity gives (iv). 

Finally, to prove property $\mathrm { ( v ) }$ , we must show that $\hat { f }$ is diferentiable and find its derivative. Let $\epsilon > 0$ and consider 

$$
\begin{array}{r l} & {\frac {\widehat {f} (\xi + h) - \widehat {f} (\xi)}{h} - (\widehat {- 2 \pi i x} f) (\xi) =} \\ & {\qquad \int_ {- \infty} ^ {\infty} f (x) e ^ {- 2 \pi i x \xi} \left[ \frac {e ^ {- 2 \pi i x h} - 1}{h} + 2 \pi i x \right] d x.} \end{array}
$$

Since $f ( x )$ and $x f ( x )$ are of rapid decrease, there exists an integer N so that $\textstyle \int _ { | x | > N } | f ( x ) | d x \leq \epsilon$ and $\begin{array} { r } { \int _ { | x | > N } | x | | f ( x ) | d x \le \epsilon } \end{array}$ . Moreover, for $| x | \leq N$ , there exists $h _ { 0 }$ so that $| h | < h _ { 0 }$ implies 

$$
\left| \frac {e ^ {- 2 \pi i x h} - 1}{h} + 2 \pi i x \right| \leq \frac {\epsilon}{N}.
$$

Hence for $| h | < h _ { 0 }$ we have 

$$
\begin{array}{r l} & {\left| \frac {\widehat {f} (\xi + h) - \widehat {f} (\xi)}{h} - (\widehat {- 2 \pi i x f}) (\xi) \right|} \\ & {\qquad \leq \int_ {- N} ^ {N} \left| f (x) e ^ {- 2 \pi i x \xi} \left[ \frac {e ^ {- 2 \pi i x h} - 1}{h} + 2 \pi i x \right] \right| d x + C \epsilon} \\ & {\qquad \leq C ^ {\prime} \epsilon .} \end{array}
$$

Theorem 1.3 $I f \ f \in S ( \mathbb { R } )$ , then ${ \hat { f } } \in { \mathcal { S } } ( \mathbb { R } )$ 

The proof is an easy application of the fact that the Fourier transform interchanges diferentiation and multiplication. In fact, note that if $f \in$ $S ( \mathbb { R } )$ , its Fourier transform $\hat { f }$ is bounded; then also, for each pair of non-negative integers ` and k, the expression 

$$
\xi^ {k} \left(\frac {d}{d \xi}\right) ^ {\ell} \hat {f} (\xi)
$$

is bounded, since by the last proposition, it is the Fourier transform of 

$$
\frac {1}{(2 \pi i) ^ {k}} \left(\frac {d}{d x}\right) ^ {k} [ (- 2 \pi i x) ^ {\ell} f (x) ].
$$

The proof of the inversion formula 

$$
f (x) = \int_ {- \infty} ^ {\infty} \hat {f} (\xi) e ^ {2 \pi i x \xi} d \xi \quad \text { for } f \in \mathcal {S} (\mathbb {R}),
$$

which we give in the next section, is based on a careful study of the function $e ^ { - a x ^ { 2 } }$ , which, as we have already observed, is in $S ( \mathbb { R } )$ if $a > 0$ 

## The Gaussians as good kernels

We begin by considering the case $a = \pi$ because of the normalization: 

$$
\int_ {- \infty} ^ {\infty} e ^ {- \pi x ^ {2}} d x = 1.\tag{6}
$$

To see why (6) is true, we use the multiplicative property of the exponential to reduce the calculation to a two-dimensional integral. More precisely, we can argue as follows: 

$$
\begin{array}{r l} & {\left(\int_ {- \infty} ^ {\infty} e ^ {- \pi x ^ {2}} d x\right) ^ {2} = \int_ {- \infty} ^ {\infty} \int_ {- \infty} ^ {\infty} e ^ {- \pi (x ^ {2} + y ^ {2})} d x d y} \\ & {\qquad = \int_ {0} ^ {2 \pi} \int_ {0} ^ {\infty} e ^ {- \pi r ^ {2}} r d r d \theta} \\ & {\qquad = \int_ {0} ^ {\infty} 2 \pi r e ^ {- \pi r ^ {2}} d r} \\ & {\qquad = \left[ - e ^ {- \pi r ^ {2}} \right] _ {0} ^ {\infty}} \\ & {\qquad = 1,} \end{array}
$$

where we have evaluated the two-dimensional integral using polar coordinates. 

The fundamental property of the Gaussian which is of interest to us, and which actually follows from (6), is that $e ^ { - \pi x ^ { 2 } }$ equals its Fourier transform! We isolate this important result in a theorem. 

Theorem 1.4 If $f ( x ) = e ^ { - \pi x ^ { 2 } }$ , then ${ \hat { f } } ( \xi ) = f ( \xi )$ 

Proof. Define 

$$
F (\xi) = \hat {f} (\xi) = \int_ {- \infty} ^ {\infty} e ^ {- \pi x ^ {2}} e ^ {- 2 \pi i x \xi} d x,
$$

and observe that $F ( 0 ) = 1$ , by our previous calculation. By property (v) in Proposition 1.2, and the fact that $f ^ { \prime } ( x ) = - 2 \pi x f ( x )$ , we obtain 

$$
F ^ {\prime} (\xi) = \int_ {- \infty} ^ {\infty} f (x) (- 2 \pi i x) e ^ {- 2 \pi i x \xi} d x = i \int_ {- \infty} ^ {\infty} f ^ {\prime} (x) e ^ {- 2 \pi i x \xi} d x.
$$

By (iv) of the same proposition, we find that 

$$
F ^ {\prime} (\xi) = i (2 \pi i \xi) \hat {f} (\xi) = - 2 \pi \xi F (\xi).
$$

## 1. Elementary theory of the Fourier transform

If we define $G ( \xi ) = F ( \xi ) e ^ { \pi \xi ^ { 2 } }$ , then from what we have seen above, it follows that $G ^ { \prime } ( \xi ) = 0$ , hence G is constant. Since $F ( 0 ) = 1$ , we conclude that G is identically equal to 1, therefore $F ( \xi ) = e ^ { - \pi \xi ^ { 2 } }$ , as was to be shown. 

The scaling properties of the Fourier transform under dilations yield the following important transformation law, which follows from (iii) in Proposition 1.2 (with δ replaced by $\delta ^ { - 1 / 2 } )$ . 

Corollary 1.5 $I f \delta > 0$ and $K _ { \delta } ( x ) = \delta ^ { - 1 / 2 } e ^ { - \pi x ^ { 2 } / \delta }$ , then $\widehat { K _ { \delta } } ( \xi ) = e ^ { - \pi \delta \xi ^ { 2 } }$ 

We pause to make an important observation. As δ tends to 0, the function $K _ { \delta }$ peaks at the origin, while its Fourier transform $\widehat { K _ { \delta } }$ gets flatter. So in this particular example, we see that $K _ { \delta }$ and $\widehat { K _ { \delta } }$ cannot both be localized (that is, concentrated) at the origin. This is an example of a general phenomenon called the Heisenberg uncertainty principle, which we will discuss at the end of this chapter. 

We have now constructed a family of good kernels on the real line, analogous to those on the circle considered in Chapter 2. Indeed, with 

$$
K _ {\delta} (x) = \delta^ {- 1 / 2} e ^ {- \pi x ^ {2} / \delta},
$$

we have: 

(i) $\begin{array} { r } { \int _ { - \infty } ^ { \infty } K _ { \delta } ( x ) d x = 1 . } \end{array}$ 

(ii) $\begin{array} { r } { \int _ { - \infty } ^ { \infty } | K _ { \delta } ( x ) | d x \leq M . } \end{array}$ 

(iii) For every $\eta > 0$ , we have $\begin{array} { r } { \int _ { | x | > \eta } | K _ { \delta } ( x ) | d x \to 0 \mathrm { ~ a s ~ } \delta \to 0 . } \end{array}$ 

To prove (i), we may change variables and use (6), or note that the integral equals $\widehat { K _ { \delta } } ( 0 )$ , which is 1 by Corollary 1.5. Since $K _ { \delta } \geq 0$ , it is clear that property (ii) is also true. Finally we can again change variables to get 

$$
\int_ {| x | > \eta} | K _ {\delta} (x) | d x = \int_ {| y | > \eta / \delta^ {1 / 2}} e ^ {- \pi y ^ {2}} d y \to 0
$$

as $\delta$ tends to 0. We have thus proved the following result. 

Theorem 1.6 The collection $\{ K _ { \delta } \} _ { \delta > 0 }$ is a family of good kernels as $\delta \to 0$ 

We next apply these good kernels via the operation of convolution, which is given as follows. If $f , g \in S ( \mathbb { R } )$ , their convolution is defined by 

$$
(f * g) (x) = \int_ {- \infty} ^ {\infty} f (x - t) g (t) d t.\tag{7}
$$

For a fixed value of $x ,$ the function $f ( x - t ) g ( t )$ is of rapid decrease in $t ,$ hence the integral converges. 

By the argument in Section 4 of Chapter 2 (with a slight modification), we $\mathrm { g e t }$ the following corollary. 

Corollary 1.7 $I f \ f \in S ( \mathbb { R } )$ , then 

$$
(f * K _ {\delta}) (x) \rightarrow f (x) \quad \text { uniformly   in   } x \text {   as   } \delta \rightarrow 0.
$$

Proof. First, we claim that $f$ is uniformly continuous on R. Indeed, given $\epsilon > 0$ there exists $R > 0$ so that $| f ( x ) | < \epsilon / 4$ whenever $| x | \geq R$ Moreover, $f$ is continuous, hence uniformly continuous on the compact interval $[ - R , R ]$ , and together with the previous observation, we can find $\eta > 0$ so that $| f ( x ) - f ( y ) | < \epsilon$ whenever $| x - y | < \eta$ . Now we argue as usual. Using the first property of good kernels, we can write 

$$
(f * K _ {\delta}) (x) - f (x) = \int_ {- \infty} ^ {\infty} K _ {\delta} (t) [ f (x - t) - f (x) ] d t,
$$

and since $K _ { \delta } \ge 0$ , we find 

$$
| (f * K _ {\delta}) (x) - f (x) | \leq \int_ {| t | > \eta} + \int_ {| t | \leq \eta} K _ {\delta} (t) | f (x - t) - f (x) | d t.
$$

The first integral is small by the third property of good kernels, and the fact that $f$ is bounded, while the second integral is also small since $f$ is uniformly continuous and $\begin{array} { r } { \int K _ { \delta } = 1 } \end{array}$ . This concludes the proof of the corollary. 

## 1.5 The Fourier inversion

The next result is an identity sometimes called the multiplication formula. 

Proposition 1.8 If $f , g \in S ( \mathbb { R } )$ , then 

$$
\int_ {- \infty} ^ {\infty} f (x) \hat {g} (x) d x = \int_ {- \infty} ^ {\infty} \hat {f} (y) g (y) d y.
$$

To prove the proposition, we need to digress briefly to discuss the interchange of the order of integration for double integrals. Suppose $F ( x , y )$ is a continuous function in the plane $( x , y ) \in \mathbb { R } ^ { 2 }$ . We will assume the following decay condition on $F ;$ 

$$
| F (x, y) | \leq A / (1 + x ^ {2}) (1 + y ^ {2}).
$$

## 1. Elementary theory of the Fourier transform

Then, we can state that for each $x$ the function $F ( x , y )$ is of moderate decrease in $y ,$ and similarly for each fixed $y$ the function $F ( x , y )$ is of moderate decrease in x. Moreover, the function $\begin{array} { r } { F _ { 1 } ( x ) = \int _ { - \infty } ^ { \infty } F ( x , y ) d y } \end{array}$ is continuous and of moderate decrease; similarly for the function $F _ { 2 } ( y ) =$ $\textstyle \int _ { - \infty } ^ { \infty } F ( x , y )$ dx. Finally 

$$
\int_ {- \infty} ^ {\infty} F _ {1} (x) d x = \int_ {- \infty} ^ {\infty} F _ {2} (y) d y.
$$

The proof of these facts may be found in the appendix. 

We now apply this to $F ( x , y ) = f ( x ) g ( y ) e ^ { - 2 \pi i x y }$ Then $F _ { 1 } ( x ) =$ $f ( x ) { \hat { g } } ( x )$ , and $F _ { 2 } ( y ) = { \hat { f } } ( y ) g ( y )$ so 

$$
\int_ {- \infty} ^ {\infty} f (x) \hat {g} (x) d x = \int_ {- \infty} ^ {\infty} \hat {f} (y) g (y) d y,
$$

which is the assertion of the proposition. 

The multiplication formula and the fact that the Gaussian is its own Fourier transform lead to a proof of the first major theorem. 

Theorem 1.9 (Fourier inversion) $I f \in S ( \mathbb { R } )$ , then 

$$
f (x) = \int_ {- \infty} ^ {\infty} \hat {f} (\xi) e ^ {2 \pi i x \xi} d \xi .
$$

Proof. We first claim that 

$$
f (0) = \int_ {- \infty} ^ {\infty} \hat {f} (\xi) d \xi .
$$

Let $G _ { \delta } ( x ) = e ^ { - \pi \delta x ^ { 2 } }$ so that $\widehat { G _ { \delta } } ( \xi ) = K _ { \delta } ( \xi )$ . By the multiplication formula we get 

$$
\int_ {- \infty} ^ {\infty} f (x) K _ {\delta} (x) d x = \int_ {- \infty} ^ {\infty} \hat {f} (\xi) G _ {\delta} (\xi) d \xi .
$$

Since $K _ { \delta }$ is a good kernel, the first integral goes to $f ( 0 )$ as δ tends to 0. Since the second integral clearly converges to $\textstyle { \int _ { - \infty } ^ { \infty } { \hat { f } } ( \xi ) \ d \xi }$ as δ tends to 0, our claim is proved. In general, let $F ( y ) = f ( y + x )$ so that 

$$
f (x) = F (0) = \int_ {- \infty} ^ {\infty} \hat {F} (\xi) d \xi = \int_ {- \infty} ^ {\infty} \hat {f} (\xi) e ^ {2 \pi i x \xi} d \xi .
$$

As the name of Theorem 1.9 suggests, it provides a formula that inverts the Fourier transform; in fact we see that the Fourier transform is its own inverse except for the change of x to $- x$ . More precisely, we may define two mappings $\mathcal { F } : \mathcal { S } ( \mathbb { R } )  \mathcal { S } ( \mathbb { R } )$ and $\mathcal { F } ^ { * } : S ( \mathbb { R } )  S ( \mathbb { R } )$ by 

$$
\mathcal {F} (f) (\xi) = \int_ {- \infty} ^ {\infty} f (x) e ^ {- 2 \pi i x \xi} d x \quad \text { and } \quad \mathcal {F} ^ {*} (g) (x) = \int_ {- \infty} ^ {\infty} g (\xi) e ^ {2 \pi i x \xi} d \xi .
$$

Thus $\mathcal { F }$ is the Fourier transform, and Theorem 1.9 guarantees that $\mathcal { F } ^ { * } \circ \mathcal { F } = I$ on $S ( \mathbb { R } )$ , where I is the identity mapping. Moreover, since the definitions of $\mathcal { F }$ and ${ \mathcal { F } } ^ { * }$ difer only by a sign in the exponential, we see that $\mathcal { F } ( f ) ( y ) = \mathcal { F } ^ { * } ( f ) ( - y )$ , so we also have $\mathcal { F } \circ \mathcal { F } ^ { * } = I$ . As a consequence, we conclude that ${ \mathcal { F } } ^ { * }$ is the inverse of the Fourier transform on $S ( \mathbb { R } )$ , and we get the following result. 

Corollary 1.10 The Fourier transform is a bijective mapping on the Schwartz space. 

## 1.6 The Plancherel formula

We need a few further results about convolutions of Schwartz functions. The key fact is that the Fourier transform interchanges convolutions with pointwise products, a result analogous to the situation for Fourier series. 

Proposition 1.11 If $f , g \in S ( \mathbb { R } )$ then: 

(i) $f * g \in S ( \mathbb { R } )$ 

(ii) $f * g = g * f .$ 

(iii) $\widehat { ( f * g ) } ( \xi ) = \hat { f } ( \xi ) \hat { g } ( \xi ) .$ 

Proof. To prove that $f * g$ is rapidly decreasing, observe first that for any $\ell \geq 0$ we have sup ${ \ u { x } } | x | ^ { \ell } | g ( x - y ) | \leq A _ { \ell } ( 1 + | y | ) ^ { \ell }$ , because $g$ is rapidly decreasing (to check this assertion, consider separately the two cases $| x | \leq 2 | y |$ and $| x | \geq 2 | y | )$ . From this, we see that 

$$
\sup _ {x} | x ^ {\ell} (f * g) (x) | \leq A _ {\ell} \int_ {- \infty} ^ {\infty} | f (y) | (1 + | y |) ^ {\ell} d y,
$$

so that $x ^ { \ell } ( f * g ) ( x )$ is a bounded function for every $\ell \geq 0$ . These estimates carry over to the derivatives of $f * g$ , thereby proving that $f * g \in S ( \mathbb { R } )$ because 

$$
\left(\frac {d}{d x}\right) ^ {k} (f * g) (x) = \left(f * \left(\frac {d}{d x}\right) ^ {k} g\right) (x) \quad \text { for } k = 1, 2, \dots .
$$

This identity is proved first for $k = 1$ by diferentiating under the integral defining $f * g$ . The interchange of diferentiation and integration is justified in this case by the rapid decrease of $d g / d x$ . The identity then follows for every k by iteration. 

For fixed $x ,$ the change of variables $x - y = u$ shows that 

$$
(f * g) (x) = \int_ {- \infty} ^ {\infty} f (x - u) g (u) d u = (g * f) (x).
$$

This change of variables is a composition of two changes, $y \mapsto - y$ and $y \mapsto y - h$ (with $h = x )$ . For the first one we use the observation that $\textstyle \int _ { - \infty } ^ { \infty } F ( x ) d x = \int _ { - \infty } ^ { \infty } F ( - x )$ dx for any Schwartz function $F$ , and for the second, we apply (ii) of Proposition 1.1 

Finally, consider $F ( x , y ) = f ( y ) g ( x - y ) e ^ { - 2 \pi i x \xi }$ . Since f and $g$ are rapidly decreasing, considering separately the two cases $| x | \leq 2 | y |$ and $| x | \geq 2 | y |$ , we see that the discussion of the change of order of integration after Proposition 1.8 applies to $F$ . In this case $F _ { 1 } ( x ) = ( f * g ) ( x ) e ^ { - 2 \pi i x \xi }$ 2 and $F _ { 2 } ( y ) = f ( y ) e ^ { - 2 \pi i y \xi } \hat { g } ( \xi )$ . Thus $\begin{array} { r } { \int _ { - \infty } ^ { \infty } F _ { 1 } ( x ) d x = \int _ { - \infty } ^ { \infty } F _ { 2 } ( y ) d y } \end{array}$ , which implies (iii). The proposition is therefore proved. 

We now use the properties of convolutions of Schwartz functions to prove the main result of this section. The result we have in mind is the analogue for functions on R of Parseval’s identity for Fourier series. 

The Schwartz space can be equipped with a Hermitian inner product 

$$
(f, g) = \int_ {- \infty} ^ {\infty} f (x) \overline {{g (x)}} d x
$$

whose associated norm is 

$$
\| f \| = \left(\int_ {- \infty} ^ {\infty} | f (x) | ^ {2} d x\right) ^ {1 / 2}.
$$

The second major theorem in the theory states that the Fourier transform is a unitary transformation on $S ( \mathbb { R } )$ . 

Theorem 1.12 (Plancherel) $I f \ f \in S ( \mathbb { R } )$ then $\| { \hat { f } } \| = \| f \|$ 

Proof. If $f \in S ( \mathbb { R } )$ define $f ^ { \flat } ( x ) = { \overline { { f ( - x ) } } }$ . Then ${ \widehat { f ^ { \flat } } } ( \xi ) = { \widehat { \hat { f } } } ( \xi )$ . Now let $h = f * f ^ { \flat }$ . Clearly, we have 

$$
\hat {h} (\xi) = | \hat {f} (\xi) | ^ {2} \quad \text { and } \quad h (0) = \int_ {- \infty} ^ {\infty} | f (x) | ^ {2}   d x.
$$

The theorem now follows from the inversion formula applied with $x = 0$ 2 that is, 

$$
\int_ {- \infty} ^ {\infty} \hat {h} (\xi) d \xi = h (0).
$$

## 1.7 Extension to functions of moderate decrease

In the previous sections, we have limited our assertion of the Fourier inversion and Plancherel formulas to the case when the function involved belonged to the Schwartz space. It does not really involve further ideas to extend these results to functions of moderate decrease, once we make the additional assumption that the Fourier transform of the function under consideration is also of moderate decrease. Indeed, the key observation, which is easy to prove, is that the convolution $f * g$ of two functions $f$ and $g$ of moderate decrease is again a function of moderate decrease (Exercise $^ { 7 ) }$ ; also $\widehat { f * g } = \widehat { f } \widehat { g }$ . Moreover, the multiplication formula continues to hold, and we deduce the Fourier inversion and Plancherel formulas when $f$ and $\hat { f }$ are both of moderate decrease. 

This generalization, although modest in scope, is nevertheless useful in some circumstances. 

## 1.8 The Weierstrass approximation theorem

We now digress briefly by further exploiting our good kernels to prove the Weierstrass approximation theorem. This result was already alluded to in Chapter 2. 

Theorem 1.13 Let f be a continuous function on the closed and bounded interval $[ a , b ] \subset \mathbb { R }$ . Then, for any $\epsilon > 0$ , there exists a polynomial $P$ such that 

$$
\sup _ {x \in [ a, b ]} | f (x) - P (x) | <   \epsilon .
$$

In other words, f can be uniformly approximated by polynomials. 

Proof. Let $[ - M , M ]$ denote any interval that contains $[ a , b ]$ in its interior, and let $g$ be a continuous function on R that equals 0 outside $[ - M , M ]$ and equals $f$ in $[ a , b ]$ . For example, extend $f$ as follows: from b to M define $g$ by a straight line segment going from $f ( b )$ to $0 ,$ , and from a to $- M$ by a straight line segment from $f ( a )$ also to 0. Let $B$ be a 

## 2. Applications to some partial differential equations

bound for $^ { g , }$ that is, $| g ( x ) | \le B$ for all $x .$ Then, since $\{ K _ { \delta } \}$ is a family of good kernels, and g is continuous with compact support, we may argue as in the proof of Corollary 1.7 to see that $g * K _ { \delta }$ converges uniformly to $g$ as $\delta$ tends to 0. In fact, we choose $\delta _ { 0 }$ so that 

$$
| g (x) - \left(g * K _ {\delta_ {0}}\right) (x) | <   \epsilon / 2 \quad \text { for   all } x \in \mathbb {R}.
$$

Now, we recall that $e ^ { x }$ is given by the power series expansion $e ^ { x } = { }$ $\textstyle \sum _ { n = 0 } ^ { \infty } x ^ { n } / n !$ which converges uniformly in every compact interval of R. Therefore, there exists an integer N so that 

$$
| K _ {\delta_ {0}} (x) - R (x) | \leq \frac {\epsilon}{4 M B} \quad \text { for   all } x \in [ - 2 M, 2 M ]
$$

where $\begin{array} { r } { R ( x ) = \delta _ { 0 } ^ { - 1 / 2 } \sum _ { n = 0 } ^ { N } \frac { ( - \pi x ^ { 2 } / \delta _ { 0 } ) ^ { n } } { n ! } } \end{array}$ Then, recalling that g vanishes outside the interval $[ - M , M ]$ , we have that for all $x \in [ - M , M ]$ 

$$
\begin{array}{l} | (g * K _ {\delta_ {0}}) (x) - (g * R) (x) | = \left| \int_ {- M} ^ {M} g (t) \left[ K _ {\delta_ {0}} (x - t) - R (x - t) \right] d t \right| \\ \leq \int_ {- M} ^ {M} | g (t) |   | K _ {\delta_ {0}} (x - t) - R (x - t) |   d t \\ \leq 2 M B \sup _ {z \in [ - 2 M, 2 M ]} | K _ {\delta_ {0}} (z) - R (z) | \\ <   \epsilon / 2. \end{array}
$$

Therefore, the triangle inequality implies that $| g ( x ) - ( g * R ) ( x ) | < \epsilon$ whenever $x \in [ - M , M ]$ , hence $| f ( x ) - ( g * R ) ( x ) | < \epsilon$ when $x \in [ a , b ]$ 

Finally, note that $g * R$ is a polynomial in the x variable. Indeed, by definition we have $\begin{array} { r } { ( g * R ) ( x ) = \int _ { - M } ^ { M } g ( t ) R ( x - t ) d t } \end{array}$ , and $R ( x - t )$ is a polynomial in x since it can be expressed, after several expansions, as $\begin{array} { r } { R ( x - t ) = \sum _ { n } a _ { n } ( t ) x ^ { n } } \end{array}$ where the sum is finite. This concludes the proof of the theorem. 

## 2 Applications to some partial diferential equations

We mentioned earlier that a crucial property of the Fourier transform is that it interchanges diferentiation and multiplication by polynomials. We now use this crucial fact together with the Fourier inversion theorem to solve some specific partial diferential equations. 

## 2.1 The time-dependent heat equation on the real line

In Chapter 4 we considered the heat equation on the circle. Here we study the analogous problem on the real line. 

Consider an infinite rod, which we model by the real line, and suppose that we are given an initial temperature distribution $f ( x )$ on the rod at time $t = 0$ . We wish now to determine the temperature $u ( x , t )$ at a point x at time $t > 0$ . Considerations similar to the ones given in Chapter 1 show that when u is appropriately normalized, it solves the following partial diferential equation: 

$$
\frac {\partial u}{\partial t} = \frac {\partial^ {2} u}{\partial x ^ {2}},\tag{8}
$$

called the heat equation. The initial condition we impose is $u ( x , 0 ) = f ( x )$ 

Just as in the case of the circle, the solution is given in terms of a convolution. Indeed, define the heat kernel of the line by 

$$
\mathcal {H} _ {t} (x) = K _ {\delta} (x), \quad \mathrm{with} \delta = 4 \pi t,
$$

so that 

$$
\mathcal {H} _ {t} (x) = \frac {1}{(4 \pi t) ^ {1 / 2}} e ^ {- x ^ {2} / 4 t} \quad \mathrm{and} \quad \hat {\mathcal {H}} _ {t} (\xi) = e ^ {- 4 \pi^ {2} t \xi^ {2}}.
$$

Taking the Fourier transform of equation (8) in the x variable (formally) leads to 

$$
\frac {\partial \hat {u}}{\partial t} (\xi , t) = - 4 \pi^ {2} \xi^ {2} \hat {u} (\xi , t).
$$

Fixing $\xi ,$ this is an ordinary diferential equation in the variable t (with unknown $\hat { u } ( \xi , \cdot ) )$ , so there exists a constant $A ( \xi )$ so that 

$$
\hat {u} (\xi , t) = A (\xi) e ^ {- 4 \pi^ {2} \xi^ {2} t}.
$$

We may also take the Fourier transform of the initial condition and obtain ${ \hat { u } } ( \xi , 0 ) = { \hat { f } } ( \xi )$ , hence $A ( \xi ) = { \hat { f } } ( \xi )$ . This leads to the following theorem. 

Theorem 2.1 Given $f \in S ( \mathbb { R } )$ , let 

$$
u (x, t) = (f * \mathcal {H} _ {t}) (x) \quad f o r t > 0
$$

where $\mathcal { H } _ { t }$ is the heat kernel. Then: 

(i) The function u is $C ^ { 2 }$ when $x \in \mathbb { R }$ and $t > 0$ , and u solves the heat equation. 

(ii) $u ( x , t ) \to f ( x )$ uniformly in x as $t \to 0$ . Hence if we set $u ( x , 0 ) =$ $f ( x )$ , then u is continuous on the closure of the upper half-plane $\overline { { \mathbb { R } _ { + } ^ { 2 } } } = \{ ( x , t ) : x \in \mathbb { R } , \ t \geq 0 \} .$ 

<sub>(iii)</sub> R ∞ <sub>|u(x,</sub> <sub>t)</sub> <sub>−</sub> <sub>f(x)|</sub>2 <sub>dx</sub> <sub>→</sub> <sub>0</sub> <sub>as</sub> <sub>t</sub> <sub>→</sub> <sub>0.</sub> 

Proof. Because $u = f * { \mathcal { H } } _ { t }$ , taking the Fourier transform in the xvariable gives $\hat { u } = \hat { f } \hat { \mathcal { H } } _ { t }$ , and so $\hat { u } ( \xi , t ) = \hat { f } ( \xi ) e ^ { - 4 \pi ^ { 2 } \xi ^ { 2 } t }$ . The Fourier inversion formula gives 

$$
u (x, t) = \int_ {- \infty} ^ {\infty} \hat {f} (\xi) e ^ {- 4 \pi^ {2} t \xi^ {2}} e ^ {2 \pi i \xi x} d \xi .
$$

By diferentiating under the integral sign, one verifies (i). In fact, one observes that u is indefinitely diferentiable. Note that (ii) is an immediate consequence of Corollary 1.7. Finally, by Plancherel’s formula, we have 

$$
\begin{array}{c} \int_ {- \infty} ^ {\infty} | u (x, t) - f (x) | ^ {2} d x = \int_ {- \infty} ^ {\infty} | \hat {u} (\xi , t) - \hat {f} (\xi) | ^ {2} d \xi \\ = \int_ {- \infty} ^ {\infty} | \hat {f} (\xi) | ^ {2} | e ^ {- 4 \pi^ {2} t \xi^ {2}} - 1 | d \xi . \end{array}
$$

To see that this last integral goes to 0 as $t \to 0$ , we argue as follows: since $| e ^ { - 4 \pi ^ { 2 } t \xi ^ { 2 } } - 1 | \le 2$ and $f \in S ( \mathbb { R } )$ , we can find N so that 

$$
\int_ {| \xi | \geq N} | \hat {f} (\xi) | ^ {2} | e ^ {- 4 \pi^ {2} t \xi^ {2}} - 1 | d \xi <   \epsilon ,
$$

and for all small t we have su $\begin{array} { r } { \mathrm { p } _ { | \xi | \leq N } | \hat { f } ( \xi ) | ^ { 2 } | e ^ { - 4 \pi ^ { 2 } t \xi ^ { 2 } } - 1 | < \epsilon / 2 N } \end{array}$ since $\hat { f }$ is bounded. Thus 

$$
\int_ {| \xi | \leq N} | \hat {f} (\xi) | ^ {2}   | e ^ {- 4 \pi^ {2} t \xi^ {2}} - 1 |   d \xi <   \epsilon \quad \text { for   all   small } t.
$$

This completes the proof of the theorem. 

The above theorem guarantees the existence of a solution to the heat equation with initial data $f .$ This solution is also unique, if uniqueness is formulated appropriately. In this regard, we note that $u = f * { \mathcal { H } } _ { t }$ $f \in S ( \mathbb { R } )$ , satisfies the following additional property. 

Corollary 2.2 $u ( \cdot , t )$ belongs to $S ( \mathbb { R } )$ uniformly in t, in the sense that for any $T > 0$ 

$$
\sup_{\substack{x  \in   \mathbb{R}\\ 0  <   t  <   T}}  |x|^{k}\left|\frac{\partial^{\ell}}{\partial x^{\ell}} u(x,t)\right| <   \infty \quad for each k,\ell \geq 0.\tag{9}
$$

Proof. This result is a consequence of the following estimate: 

$$
\begin{array}{l} | u (x, t) | \leq \int_ {| y | \leq | x | / 2} | f (x - y) | \mathcal {H} _ {t} (y) d y + \int_ {| y | \geq | x | / 2} | f (x - y) | \mathcal {H} _ {t} (y) d y \\ \leq \frac {C _ {N}}{(1 + | x |) ^ {N}} + \frac {C}{\sqrt {t}} e ^ {- c x ^ {2} / t}. \end{array}
$$

Indeed, since f is rapidly decreasing, we have $| f ( x - y ) | \leq C _ { N } / ( 1 + | x | ) ^ { N }$ when $| y | \leq | x | / 2$ . Also, if $| y | \geq | x | / 2$ then $\mathcal { H } _ { t } ( y ) \leq C t ^ { - 1 / 2 } e ^ { - c x ^ { 2 } / t }$ , and we obtain the above inequality. Consequently, we see that $u ( x , t )$ is rapidly decreasing uniformly for $0 < t < T$ 

The same argument can be applied to the derivatives of u in the x variable since we may diferentiate under the integral sign and apply the above estimate with $f$ replaced by $f ^ { \prime } { } .$ , and so on. 

This leads to the following uniqueness theorem. 

Theorem 2.3 Suppose $u ( x , t )$ satisfies the following conditions: 

(i) u is continuous on the closure of the upper half-plane. 

(ii) u satisfies the heat equation for $t > 0$ 

(iii) u satisfies the boundary condition $u ( x , 0 ) = 0$ 

(iv) $u ( \cdot , t ) \in S ( \mathbb { R } )$ uniformly in t, as in $( 9 )$ 

Then, we conclude that $u = 0$ 

Below we use the abbreviations $\partial _ { x } ^ { \ell } u$ and $\partial _ { t } \boldsymbol { u }$ to denote $\partial ^ { \ell } u / \partial x ^ { \ell }$ and $\partial \boldsymbol u / \partial t$ , respectively. 

Proof. We define the energy at time t of the solution $u ( x , t )$ by 

$$
E (t) = \int_ {\mathbb {R}} | u (x, t) | ^ {2} d x.
$$

Clearly $E ( t ) \geq 0$ . Since $E ( 0 ) = 0$ it sufices to show that E is a decreasing function, and this is achieved by proving that $d E / d t \leq 0$ . The assumptions on u allow us to diferentiate $E ( t )$ under the integral sign 

$$
\frac {d E}{d t} = \int_ {\mathbb {R}} \left[ \partial_ {t} u (x, t) \overline {{u}} (x, t) + u (x, t) \partial_ {t} \overline {{u}} (x, t) \right] d x.
$$

But u satisfies the heat equation, therefore $\partial _ { t } u = \partial _ { x } ^ { 2 } u$ and $\partial _ { t } \overline { { u } } = \partial _ { x } ^ { 2 } \overline { { u } } .$ , so that after an integration by parts, where we use the fact that u and its 

## 2. Applications to some partial differential equations

x derivatives decrease rapidly as $| x | \to \infty ,$ we find 

$$
\begin{array}{l} \frac {d E}{d t} = \int_ {\mathbb {R}} \left[ \partial_ {x} ^ {2} u (x, t) \overline {{u}} (x, t) + u (x, t) \partial_ {x} ^ {2} \overline {{u}} (x, t) \right] d x \\ = - \int_ {\mathbb {R}} \left[ \partial_ {x} u (x, t) \partial_ {x} \overline {{u}} (x, t) + \partial_ {x} u (x, t) \partial_ {x} \overline {{u}} (x, t) \right] d x \\ = - 2 \int_ {\mathbb {R}} | \partial_ {x} u (x, t) | ^ {2} d x \\ \leq 0, \end{array}
$$

as claimed. Thus $E ( t ) = 0$ for all t, hence $u = 0$ 

Another uniqueness theorem for the heat equation, with a less restrictive assumption than (9), can be found in Problem 6. Examples when uniqueness fails are given in Exercise 12 and Problem 4. 

## 2.2 The steady-state heat equation in the upper half-plane

The equation we are now concerned with is 

$$
\triangle u = \frac {\partial^ {2} u}{\partial x ^ {2}} + \frac {\partial^ {2} u}{\partial y ^ {2}} = 0\tag{10}
$$

in the upper half-plane $\mathbb { R } _ { + } ^ { 2 } = \{ ( x , y ) : x \in \mathbb { R } , y > 0 \}$ . The boundary condition we require is $u ( x , 0 ) = f ( x )$ . The operator 4 is the Laplacian and the above partial diferential equation describes the steady-state heat distribution in $\mathbb { R } _ { + } ^ { 2 }$ subject to $u = f$ on the boundary. The kernel that solves this problem is called the Poisson kernel for the upper half-plane, and is given by 

$$
\mathcal {P} _ {y} (x) = \frac {1}{\pi} \frac {y}{x ^ {2} + y ^ {2}} \quad \text { where } x \in \mathbb {R} \text { and } y > 0.
$$

This is the analogue of the Poisson kernel for the disc discussed in Section 5.4 of Chapter 2. 

Note that for each fixed y the kernel $\mathcal { P } _ { y }$ is only of moderate decrease as a function of $x ,$ so we will use the theory of the Fourier transform appropriate for these types of functions (see Section 1.7). 

We proceed as in the case of the time-dependent heat equation, by taking the Fourier transform of equation (10) (formally) in the x variable, thereby obtaining 

$$
- 4 \pi^ {2} \xi^ {2} \hat {u} (\xi , y) + \frac {\partial^ {2} \hat {u}}{\partial y ^ {2}} (\xi , y) = 0
$$

with the boundary condition ${ \hat { u } } ( \xi , 0 ) = { \hat { f } } ( \xi )$ . The general solution of this ordinary diferential equation in y (with ξ fixed) takes the form 

$$
\hat {u} (\xi , y) = A (\xi) e ^ {- 2 \pi | \xi | y} + B (\xi) e ^ {2 \pi | \xi | y}.
$$

If we disregard the second term because of its rapid exponential increase we find, after setting $y = 0$ , that 

$$
\hat {u} (\xi , y) = \hat {f} (\xi) e ^ {- 2 \pi | \xi | y}.
$$

Therefore u is given in terms of the convolution of $f$ with a kernel whose Fourier transform is $e ^ { - 2 \pi | \xi | y }$ . This is precisely the Poisson kernel given above, as we prove next. 

Lemma 2.4 The following two identities hold: 

$$
\begin{array}{r l} & {\int_ {- \infty} ^ {\infty} e ^ {- 2 \pi | \xi | y} e ^ {2 \pi i \xi x} d \xi = \mathcal {P} _ {y} (x),} \\ & {\int_ {- \infty} ^ {\infty} \mathcal {P} _ {y} (x) e ^ {- 2 \pi i x \xi} d x = e ^ {- 2 \pi | \xi | y}.} \end{array}
$$

Proof. The first formula is fairly straightforward since we can split the integral from $- \infty$ to 0 and 0 to ∞. Then, since $y > 0$ we have 

$$
\begin{array}{r} \int_ {0} ^ {\infty} e ^ {- 2 \pi \xi y} e ^ {2 \pi i \xi x} d \xi = \int_ {0} ^ {\infty} e ^ {2 \pi i (x + i y) \xi} d \xi = \left[ \frac {e ^ {2 \pi i (x + i y) \xi}}{2 \pi i (x + i y)} \right] _ {0} ^ {\infty} = \\ - \frac {1}{2 \pi i (x + i y)}, \end{array}
$$

and similarly, 

$$
\int_ {- \infty} ^ {0} e ^ {2 \pi \xi y} e ^ {2 \pi i \xi x} d \xi = \frac {1}{2 \pi i (x - i y)}.
$$

Therefore 

$$
\int_ {- \infty} ^ {\infty} e ^ {- 2 \pi | \xi | y} e ^ {2 \pi i \xi x} d \xi = \frac {1}{2 \pi i (x - i y)} - \frac {1}{2 \pi i (x + i y)} = \frac {y}{\pi (x ^ {2} + y ^ {2})}.
$$

The second formula is now a consequence of the Fourier inversion theorem applied in the case when $f$ and $\hat { f }$ are of moderate decrease. 

Lemma 2.5 The Poisson kernel is a good kernel on $\mathbb { R }$ as $y \to 0$ 

Proof. Setting $\xi = 0$ in the second formula of the lemma shows that $\begin{array} { r } { \int _ { - \infty } ^ { \infty } \mathcal { P } _ { y } ( x ) d x = 1 } \end{array}$ , and clearly $\mathcal { P } _ { y } ( x ) \geq 0$ , so it remains to check the last property of good kernels. Given a fixed $\delta > 0$ , we may change variables $u = x / y$ so that 

$$
\int_ {\delta} ^ {\infty} \frac {y}{x ^ {2} + y ^ {2}} d x = \int_ {\delta / y} ^ {\infty} \frac {d u}{1 + u ^ {2}} = [ \arctan u ] _ {\delta / y} ^ {\infty} = \pi / 2 - \arctan (\delta / y),
$$

and this quantity goes to 0 as $y \to 0$ . Since $\mathcal { P } _ { y } ( x )$ is an even function, the proof is complete. 

The following theorem establishes the existence of a solution to our problem. 

Theorem 2.6 Given $f \in S ( \mathbb { R } )$ , let $u ( x , y ) = ( f * \mathcal { P } _ { y } ) ( x )$ . Then: 

(i) $u ( x , y )$ is $C ^ { 2 }$ in $\mathbb { R } _ { + } ^ { 2 }$ and $\triangle u = 0$ 

(ii) $u ( x , y ) \to f ( x )$ uniformly as $y \to 0$ 

(iii) $\begin{array} { r } { \int _ { - \infty } ^ { \infty } | u ( x , y ) - f ( x ) | ^ { 2 } d x \to 0 \ a s \ y \to 0 . } \end{array}$ 

(iv) If $u ( x , 0 ) = f ( x )$ , then u is continuous on the closure $\overline { { \mathbb { R } _ { + } ^ { 2 } } }$ of the upper $h a l f - p l a n e ,$ and vanishes at infinity in the sense that 

$$
u (x, y) \rightarrow 0 \quad a s | x | + y \rightarrow \infty .
$$

Proof. The proofs of parts $( \mathrm { i } ) , ( \mathrm { i i } )$ , and (iii) are similar to the case of the heat equation, and so are left to the reader. Part $( \mathrm { i v } )$ is a consequence of two easy estimates whenever $f$ is of moderate decrease. First, we have 

$$
| (f * \mathcal {P} _ {y}) (x) | \leq C \left(\frac {1}{(1 + x ^ {2})} + \frac {y}{x ^ {2} + y ^ {2}}\right)
$$

which is proved (as in the case of the heat equation) by splitting the integral $\textstyle \int _ { - \infty } ^ { \infty } f ( x - t ) { \mathcal { P } } _ { y } ( t )$ dt into the part where $| t | \leq | x | / 2$ and the part where $| t | \geq | x | / 2$ . Also, we have $| ( f \ast \mathcal { P } _ { y } ) ( x ) | \leq C / y$ , since $\operatorname* { s u p } _ { x } \mathcal { P } _ { y } ( x ) \leq$ $c / y$ 

Using the first estimate when $| x | \geq | y |$ and the second when $| x | \le | y |$ gives the desired decrease at infinity. 

We next show that the solution is essentially unique. 

Theorem 2.7 Suppose u is continuous on the closure of the upper halfplane $\overline { { \mathbb { R } _ { + } ^ { 2 } } }$ , satisfies $\triangle u = 0 \ f o r \left( x , y \right) \in \mathbb { R } _ { + } ^ { 2 } , \ u ( x , 0 ) = 0$ , and $u ( x , y )$ vanishes at infinity. Then $u = 0$ 

A simple example shows that a condition concerning the decay of u at infinity is needed: take $u ( x , y ) = y$ . Clearly u satisfies the steady-state heat equation and vanishes on the real line, yet u is not identically zero. 

The proof of the theorem relies on a basic fact about harmonic functions, which are functions satisfying $\triangle u = 0$ . The fact is that the value of a harmonic function at a point equals its average value around any circle centered at that point. 

Lemma 2.8 (Mean-value property) Suppose Ω is an open set in $\mathbb { R } ^ { 2 }$ and let u be a function of class $C ^ { 2 }$ with $\triangle u = 0$ in Ω. If the closure of the disc centered at $( x , y )$ and of radius R is contained in Ω, then 

$$
u (x, y) = \frac {1}{2 \pi} \int_ {0} ^ {2 \pi} u (x + r \cos \theta , y + r \sin \theta) d \theta
$$

for all $0 \leq r \leq R$ 

Proof. Let $U ( r , \theta ) = u ( x + r \cos \theta , y + r \sin \theta )$ . Expressing the Laplacian in polar coordinates, the equation $\triangle u = 0$ then implies 

$$
0 = \frac {\partial^ {2} U}{\partial \theta^ {2}} + r \frac {\partial}{\partial r} \left(r \frac {\partial U}{\partial r}\right).
$$

If we define $\begin{array} { r } { F ( r ) = \frac { 1 } { 2 \pi } \int _ { 0 } ^ { 2 \pi } U ( r , \theta ) d \theta } \end{array}$ , the above gives 

$$
r \frac {\partial}{\partial r} \left(r \frac {\partial F}{\partial r}\right) = \frac {1}{2 \pi} \int_ {0} ^ {2 \pi} - \frac {\partial^ {2} U}{\partial \theta^ {2}} (r, \theta) d \theta .
$$

The integral of $\partial ^ { 2 } U / \partial \theta ^ { 2 }$ over the circle vanishes since $\partial U / \partial \theta$ is periodic, hence $\begin{array} { r } { r \frac { \partial } { \partial r } \left( r \frac { \partial F } { \partial r } \right) = 0 } \end{array}$ , and consequently $r \partial F / \partial r$ must be constant. Evaluating this expression at $r = 0$ we find that ${ { \partial F } \mathord { \left/ { \vphantom { { \partial F } { \partial r } } } \right. \kern - delimiterspace } { \partial r } } = 0$ . Thus $F$ is constant, but since $F ( 0 ) = u ( x , y )$ , we finally find that $F ( r ) = u ( x , y )$ for all $0 \leq r \leq R$ , which is the mean-value property. 

Finally, note that the argument above is implicit in the proof of Theorem 5.7, Chapter 2. 

To prove Theorem 2.7 we argue by contradiction. Considering separately the real and imaginary parts of $u ,$ , we may suppose that u itself is real-valued, and is somewhere strictly positive, say $u ( x _ { 0 } , y _ { 0 } ) > 0$ for some $x _ { 0 } \in \mathbb { R }$ and $y _ { 0 } > 0$ . We shall see that this leads to a contradiction. First, since u vanishes at infinity, we can find a large semi-disc of radius R, $D _ { R } ^ { + } = \{ ( x , y ) : \ x ^ { 2 } + y ^ { 2 } \leq R , y \geq 0 \}$ outside of which $u ( x , y ) \leq$ ${ \scriptstyle { \frac { 1 } { 2 } } } u ( x _ { 0 } , y _ { 0 } )$ . Next, since u is continuous in $D _ { R } ^ { + } ,$ it attains its maximum M there, so there exists a point $( x _ { 1 } , y _ { 1 } ) \in D _ { R } ^ { + }$ with $u ( x _ { 1 } , y _ { 1 } ) = M$ , while 

## 3. The Poisson summation formula

$u ( x , y ) \leq M$ in the semi-disc; also, since $u ( x , y ) \leq \textstyle { \frac { 1 } { 2 } } u ( x _ { 0 } , y _ { 0 } ) \leq M / 2$ outside of the semi-disc, we have $u ( x , y ) \leq M$ throughout the entire upper half-plane. Now the mean-value property for harmonic functions implies 

$$
u (x _ {1}, y _ {1}) = \frac {1}{2 \pi} \int_ {0} ^ {2 \pi} u (x _ {1} + \rho \cos \theta , y _ {1} + \rho \sin \theta) d \theta
$$

whenever the circle of integration lies in the upper half-plane. In particular, this equation holds if $0 < \rho < y _ { 1 }$ Since $u ( x _ { 1 } , y _ { 1 } )$ equals the maximum value $M$ , and $u ( x _ { 1 } + \rho$ cos $\theta , y _ { 1 } + \rho$ sin $\theta ) \leq M$ , it follows by continuity that $u ( x _ { 1 } + \rho$ cos $\theta , y _ { 1 } + \rho \sin \theta ) = M$ on the whole circle. For otherwise $u ( x , y ) \leq M - \epsilon$ , on an arc of length $\delta > 0$ on the circle, and this would give 

$$
\frac {1}{2 \pi} \int_ {0} ^ {2 \pi} u (x _ {1} + \rho \cos \theta , y _ {1} + \rho \sin \theta) d \theta \leq M - \frac {\epsilon \delta}{2 \pi} <   M,
$$

contradicting the fact that $u ( x _ { 1 } , y _ { 1 } ) = M .$ . Now letting $\rho \longrightarrow y _ { 1 }$ , and using the continuity of u again, we see that this implies $u ( x _ { 1 } , 0 ) = M > 0$ which contradicts the fact that $u ( x , 0 ) = 0$ for all $x .$ 

## 3 The Poisson summation formula

The definition of the Fourier transform was motivated by the desire for a continuous version of Fourier series, applicable to functions defined on the real line. We now show that there exists a further remarkable connection between the analysis of functions on the circle and related functions on R. 

Given a function $f \in S ( \mathbb { R } )$ on the real line, we can construct a new function on the circle by the recipe 

$$
F _ {1} (x) = \sum_ {n = - \infty} ^ {\infty} f (x + n).
$$

Since $f$ is rapidly decreasing, the series converges absolutely and uniformly on every compact subset of $\mathbb { R } ,$ , so $F _ { 1 }$ is continuous. Note that $F _ { 1 } ( x + 1 ) = F _ { 1 } ( x )$ because passage from n to $n + 1$ in the above sum merely shifts the terms on the series defining $F _ { 1 } ( x )$ . Hence $F _ { 1 }$ is periodic with period 1. The function $F _ { 1 }$ is called the periodization of $f .$ . 

There is another way to arrive at a “periodic version” of $f ,$ this time by Fourier analysis. Start with the identity 

$$
f (x) = \int_ {- \infty} ^ {\infty} \hat {f} (\xi) e ^ {2 \pi i \xi x} d \xi ,
$$

and consider its discrete analogue, where the integral is replaced by a sum 

$$
F _ {2} (x) = \sum_ {n = - \infty} ^ {\infty} \hat {f} (n) e ^ {2 \pi i n x}.
$$

Once again, the sum converges absolutely and uniformly since $\hat { f }$ belongs to the Schwartz space, hence $F _ { 2 }$ is continuous. Moreover, $F _ { 2 }$ is also periodic of period 1 since this is the case for each one of the exponentials e<sup>2πinx</sup>. 

The fundamental fact is that these two approaches, which produce $F _ { 1 }$ and $F _ { 2 } .$ actually lead to the same function. 

Theorem 3.1 (Poisson summation formula) If $f \in S ( \mathbb { R } )$ , then 

$$
\sum_ {n = - \infty} ^ {\infty} f (x + n) = \sum_ {n = - \infty} ^ {\infty} \hat {f} (n) e ^ {2 \pi i n x}.
$$

In particular, setting $x = 0$ we have 

$$
\sum_ {n = - \infty} ^ {\infty} f (n) = \sum_ {n = - \infty} ^ {\infty} \hat {f} (n).
$$

In other words, the Fourier coeficients of the periodization of $f$ are given precisely by the values of the Fourier transform of f on the integers. 

Proof. To check the first formula it sufices, by Theorem 2.1 in Chapter 2, to show that both sides (which are continuous) have the same Fourier coeficients (viewed as functions on the circle). Clearly, the $m ^ { \mathrm { t h } }$ Fourier coeficient of the right-hand side is ${ \hat { f } } ( m )$ . For the left-hand side we have 

$$
\begin{array}{r l} \int_ {0} ^ {1} \left(\sum_ {n = - \infty} ^ {\infty} f (x + n)\right) e ^ {- 2 \pi i m x} d x & = \sum_ {n = - \infty} ^ {\infty} \int_ {0} ^ {1} f (x + n) e ^ {- 2 \pi i m x} d x \\ & = \sum_ {n = - \infty} ^ {\infty} \int_ {n} ^ {n + 1} f (y) e ^ {- 2 \pi i m y} d y \\ & = \int_ {- \infty} ^ {\infty} f (y) e ^ {- 2 \pi i m y} d y \\ & = \hat {f} (m), \end{array}
$$

where the interchange of the sum and integral is permissible since $f$ is rapidly decreasing. This completes the proof of the theorem. 

## 3. The Poisson summation formula

We observe that the theorem extends to the case when we merely assume that both $f$ and $\hat { f }$ are of moderate decrease; the proof is in fact unchanged. 

It turns out that the operation of periodization is important in a number of questions, even when the Poisson summation formula does not apply. We give an example by considering the elementary function $f ( x ) = 1 / x , x \neq 0$ . The result is that ${ \textstyle \sum _ { n = - \infty } ^ { \infty } 1 } / ( x + n )$ , when summed symmetrically, gives the partial fraction decomposition of the cotangent function. In fact this sum equals π cot πx, when x is not an integer. Similarly with $f ( x ) = 1 / x ^ { 2 }$ , we get $\scriptstyle \sum _ { n = - \infty } ^ { \infty } 1 / ( x + n ) ^ { 2 } = \pi ^ { 2 } / ( \sin \pi x ) ^ { 2 }$ whenever x $\notin \mathbb { Z }$ (see Exercise 15). 

## 3.1 Theta and zeta functions

We define the theta function $\vartheta ( s )$ for $s > 0$ by 

$$
\vartheta (s) = \sum_ {n = - \infty} ^ {\infty} e ^ {- \pi n ^ {2} s}.
$$

The condition on s ensures the absolute convergence of the series. A crucial fact about this special function is that it satisfies the following functional equation. 

Theorem 3.2 $s ^ { - 1 / 2 } \vartheta ( 1 / s ) = \vartheta ( s )$ whenever $s > 0$ 

The proof of this identity consists of a simple application of the Poisson summation formula to the pair 

$$
f (x) = e ^ {- \pi s x ^ {2}} \quad \mathrm{and} \quad \hat {f} (\xi) = s ^ {- 1 / 2} e ^ {- \pi \xi^ {2} / s}.
$$

The theta function $\vartheta ( s )$ also extends to complex values of s when $\operatorname { R e } ( s ) > 0$ , and the functional equation is still valid then. The theta function is intimately connected with an important function in number theory, the zeta function $\zeta ( s )$ defined for $\operatorname { R e } ( s ) > 1$ by 

$$
\zeta (s) = \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {s}}.
$$

Later we will see that this function carries essential information about the prime numbers (see Chapter 8). 

It also turns out that $\zeta , \vartheta ,$ and another important function Γ are related by the following identity: 

$$
\pi^ {- s / 2} \Gamma (s / 2) \zeta (s) = \frac {1}{2} \int_ {0} ^ {\infty} t ^ {s / 2 - 1} (\vartheta (t) - 1) d t,
$$

which is valid for $s > 1$ (Exercises 17 and 18). 

Returning to the function ϑ, define the generalization $\Theta ( z | \tau )$ given by 

$$
\Theta (z | \tau) = \sum_ {n = - \infty} ^ {\infty} e ^ {i \pi n ^ {2} \tau} e ^ {2 \pi i n z}
$$

whenever Im $. ( \tau ) > 0$ and $z \in \mathbb { C }$ . Taking $z = 0$ and $\tau = i s$ we get $\Theta ( z | \tau ) =$ $\vartheta ( s )$ 

## 3.2 Heat kernels

Another application related to the Poisson summation formula and the theta function is the time-dependent heat equation on the circle. A solution to the equation 

$$
\frac {\partial u}{\partial t} = \frac {\partial^ {2} u}{\partial x ^ {2}}
$$

subject to $u ( x , 0 ) = f ( x )$ , where f is periodic of period 1, was given in the previous chapter by 

$$
u (x, t) = (f * H _ {t}) (x)
$$

where $H _ { t } ( x )$ is the heat kernel on the circle, that is, 

$$
H _ {t} (x) = \sum_ {n = - \infty} ^ {\infty} e ^ {- 4 \pi^ {2} n ^ {2} t} e ^ {2 \pi i n x}.
$$

Note in particular that with our definition of the generalized theta function in the previous section, we have $\Theta ( x | 4 \pi i t ) = H _ { t } ( x )$ . Also, recall that the heat equation on R gave rise to the heat kernel 

$$
\mathcal {H} _ {t} (x) = \frac {1}{(4 \pi t) ^ {1 / 2}} e ^ {- x ^ {2} / 4 t}
$$

where $\hat { \mathcal { H } } _ { t } ( \xi ) = e ^ { - 4 \pi ^ { 2 } \xi ^ { 2 } t }$ . The fundamental relation between these two objects is an immediate consequence of the Poisson summation formula: 

Theorem 3.3 The heat kernel on the circle is the periodization of the heat kernel on the real line: 

$$
H _ {t} (x) = \sum_ {n = - \infty} ^ {\infty} \mathcal {H} _ {t} (x + n).
$$

## 3. The Poisson summation formula

Although the proof that $\mathcal { H } _ { t }$ is a good kernel on R was fairly straightforward, we left open the harder problem that $H _ { t }$ is a good kernel on the circle. The above results allow us to resolve this matter. 

Corollary 3.4 The kernel $H _ { t } ( x )$ is a good kernel for $t \to 0$ 

Proof. We already observed that $\begin{array} { r } { \int _ { | x | \leq 1 / 2 } H _ { t } ( x ) d x = 1 } \end{array}$ . Now note that $H _ { t } \geq 0$ , which is immediate from the above formula since $\mathcal { H } _ { t } \geq 0$ Finally, we claim that when $| x | \le 1 / 2$ 2 

$$
H _ {t} (x) = \mathcal {H} _ {t} (x) + \mathcal {E} _ {t} (x),
$$

where the error satisfies $| \mathcal { E } _ { t } ( x ) | \leq c _ { 1 } e ^ { - c _ { 2 } / t }$ with $c _ { 1 } , c _ { 2 } > 0$ and $0 < t \leq 1$ To see this, note again that the formula in the theorem gives 

$$
H _ {t} (x) = \mathcal {H} _ {t} (x) + \sum_ {| n | \geq 1} \mathcal {H} _ {t} (x + n);
$$

therefore, since $| x | \leq 1 / 2 .$ 

$$
\mathcal {E} _ {t} (x) = \frac {1}{\sqrt {4 \pi t}} \sum_ {| n | \geq 1} e ^ {- (x + n) ^ {2} / 4 t} \leq C t ^ {- 1 / 2} \sum_ {n \geq 1} e ^ {- c n ^ {2} / t}.
$$

Note that $n ^ { 2 } / t \geq n ^ { 2 }$ and $n ^ { 2 } / t \geq 1 / t$ whenever $0 < t \leq 1$ , so $e ^ { - c n ^ { 2 } / t } \leq$ $e ^ { - \frac { c } { 2 } n ^ { 2 } } e ^ { - \frac { c } { 2 } \frac { 1 } { t } }$ . Hence 

$$
| \mathcal {E} _ {t} (x) | \leq C t ^ {- 1 / 2} e ^ {- \frac {c}{2} \frac {1}{t}} \sum_ {n \geq 1} e ^ {- \frac {c}{2} n ^ {2}} \leq c _ {1} e ^ {- c _ {2} / t}.
$$

The proof of the claim is complete, and as a result $\begin{array} { r } { \int _ { | x | \leq 1 / 2 } | \mathcal { E } _ { t } ( x ) | d x \to 0 } \end{array}$ as $t \to 0$ . It is now clear that $H _ { t }$ satisfies 

$$
\int_ {\eta <   | x | \leq 1 / 2} | H _ {t} (x) | d x \to 0 \quad \text { as } t \to 0,
$$

because $\mathcal { H } _ { t }$ does. 

## 3.3 Poisson kernels

In a similar manner to the discussion above about the heat kernels, we state the relation between the Poisson kernels for the disc and the upper half-plane where 

$$
P _ {r} (\theta) = \frac {1 - r ^ {2}}{1 - 2 r \cos \theta + r ^ {2}} \quad \mathrm{and} \quad \mathcal {P} _ {y} (x) = \frac {1}{\pi} \frac {y}{y ^ {2} + x ^ {2}}.
$$

Theorem 3.5 $\begin{array} { r } { P _ { r } ( 2 \pi x ) = \sum _ { n \in \mathbb { Z } } \mathcal { P } _ { y } ( x + n ) \ w h e r e \ r = e ^ { - 2 \pi y } . } \end{array}$ 

This is again an immediate corollary of the Poisson summation formula applied to $f ( x ) = \mathcal { P } _ { y } ( x )$ and ${ \hat { f } } ( \xi ) = { \dot { e } } ^ { - 2 \pi | \xi | y }$ . Of course, here we use the Poisson summation formula under the assumptions that $f$ and $\hat { f }$ are of moderate decrease. 

## 4 The Heisenberg uncertainty principle

The mathematical thrust of the principle can be formulated in terms of a relation between a function and its Fourier transform. The basic underlying law, formulated in its vaguest and most general form, states that a function and its Fourier transform cannot both be essentially localized. Somewhat more precisely, if the “preponderance” of the mass of a function is concentrated in an interval of length $L ,$ then the preponderance of the mass of its Fourier transform cannot lie in an interval of length essentially smaller than $L ^ { - 1 }$ . The exact statement is as follows. 

Theorem 4.1 Suppose $\psi$ is a function in $S ( \mathbb { R } )$ which satisfies the normalizing condition $\int _ { - \infty } ^ { \infty } | \psi ( x ) | ^ { 2 }$ dx = 1. Then 

$$
\left(\int_ {- \infty} ^ {\infty} x ^ {2} | \psi (x) | ^ {2} d x\right) \left(\int_ {- \infty} ^ {\infty} \xi^ {2} | \hat {\psi} (\xi) | ^ {2} d \xi\right) \geq \frac {1}{1 6 \pi^ {2}},
$$

and equality holds if and only $i f \psi ( x ) = A e ^ { - B x ^ { 2 } }$ where $B > 0$ and $| A | ^ { 2 } =$ $\sqrt { 2 B / \pi }$ 

In fact, we have 

$$
\left(\int_ {- \infty} ^ {\infty} (x - x _ {0}) ^ {2} | \psi (x) | ^ {2} d x\right) \left(\int_ {- \infty} ^ {\infty} (\xi - \xi_ {0}) ^ {2} | \hat {\psi} (\xi) | ^ {2} d \xi\right) \geq \frac {1}{1 6 \pi^ {2}}
$$

for every $x _ { 0 } , \xi _ { 0 } \in \mathbb { R }$ 

Proof. The second inequality actually follows from the first by replacing $\psi ( x )$ by $e ^ { - 2 \pi i x \xi _ { 0 } } \psi ( x + x _ { 0 } )$ and changing variables. To prove the first inequality, we argue as follows. Beginning with our normalizing assumption $\textstyle \int | \psi | ^ { 2 } = 1$ , and recalling that $\psi$ and $\psi ^ { \prime }$ are rapidly decreasing, an integration by parts gives 

$$
\begin{array}{r l} & {1 = \int_ {- \infty} ^ {\infty} | \psi (x) | ^ {2} d x} \\ & {\quad = - \int_ {- \infty} ^ {\infty} x \frac {d}{d x} | \psi (x) | ^ {2} d x} \\ & {\quad = - \int_ {- \infty} ^ {\infty} \left(x \psi^ {\prime} (x) \overline {{\psi (x)}} + x \overline {{\psi^ {\prime} (x)}} \psi (x)\right) d x.} \end{array}
$$

4. The Heisenberg uncertainty principle 

The last identity follows because $| \psi | ^ { 2 } = \psi \overline { { \psi } }$ . Therefore 

$$
\begin{array}{l} 1 \leq 2 \int_ {- \infty} ^ {\infty} | x |   | \psi (x) |   | \psi^ {\prime} (x) |   d x \\ \quad \leq 2 \left(\int_ {- \infty} ^ {\infty} x ^ {2} | \psi (x) | ^ {2}   d x\right) ^ {1 / 2} \left(\int_ {- \infty} ^ {\infty} | \psi^ {\prime} (x) | ^ {2}   d x\right) ^ {1 / 2}, \end{array}
$$

where we have used the Cauchy-Schwarz inequality. The identity 

$$
\int_ {- \infty} ^ {\infty} | \psi^ {\prime} (x) | ^ {2} d x = 4 \pi^ {2} \int_ {- \infty} ^ {\infty} \xi^ {2} | \hat {\psi} (\xi) | ^ {2} d \xi ,
$$

which holds because of the properties of the Fourier transform and the Plancherel formula, concludes the proof of the inequality in the theorem. 

If equality holds, then we must also have equality where we applied the Cauchy-Schwarz inequality, and as a result we find that $\psi ^ { \prime } ( x ) = \beta x \psi ( x )$ for some constant $\beta .$ The solutions to this equation are $\psi ( \stackrel { \cdot } { x } ) = A e ^ { \beta x ^ { 2 } / 2 } ,$ where A is constant. Since we want $\psi$ to be a Schwartz function, we must take $\beta = - 2 B < 0$ , and since we impose the condition $\begin{array} { r } { \int _ { - \infty } ^ { \infty } | \psi ( x ) | ^ { 2 } d x = 1 } \end{array}$ we find that $| A | ^ { 2 } = { \sqrt { 2 B / \pi } }$ , as was to be shown. 

The precise assertion contained in Theorem 4.1 first came to light in the study of quantum mechanics. It arose when one considered the extent to which one could simultaneously locate the position and momentum of a particle. Assuming we are dealing with (say) an electron that travels along the real line, then according to the laws of physics, matters are governed by a “state function” $\psi _ { ; }$ which we can assume to be in $S ( \mathbb { R } )$ ， and which is normalized according to the requirement that 

$$
\int_ {- \infty} ^ {\infty} | \psi (x) | ^ {2} d x = 1.\tag{11}
$$

The position of the particle is then determined not as a definite point x; instead its probable location is given by the rules of quantum mechanics as follows: 

• The probability that the particle is located in the interval $( a , b )$ is $\textstyle \int _ { a } ^ { b } | \psi ( x ) | ^ { 2 } d x$ 

According to this law we can calculate the probable location of the particle with the aid of $\psi :$ in fact, there may be only a small probability that the particle is located in a given interval $( a ^ { \prime } , b ^ { \prime } )$ , but nevertheless it is somewhere on the real line since $\begin{array} { r } { \int _ { - \infty } ^ { \infty } | \psi ( x ) | ^ { 2 } d x = 1 } \end{array}$ 

In addition to the probability density $| \psi ( x ) | ^ { 2 } d x$ , there is the expectation of where the particle might be. This expectation is the best guess of the position of the particle, given its probability distribution determined by $| \psi ( x ) | ^ { 2 } d x$ , and is the quantity defined by 

$$
\overline {{x}} = \int_ {- \infty} ^ {\infty} x | \psi (x) | ^ {2} d x.\tag{12}
$$

Why is this our best guess? Consider the simpler (idealized) situation where we are given that the particle can be found at only finitely many diferent points, $x _ { 1 } , x _ { 2 } , \dotsc , x _ { N }$ on the real axis, with $p _ { i }$ the probability that the particle is at $x _ { i } ,$ , and $p _ { 1 } + p _ { 2 } + \cdot \cdot \cdot + p _ { N } = 1$ . Then, if we knew nothing else, and were forced to make one choice as to the position of the particle, we would naturally take $\begin{array} { r } { \overline { { x } } = \sum _ { i = 1 } ^ { N } x _ { i } p _ { i } } \end{array}$ , which is the appropriate weighted average of the possible positions. The quantity (12) is clearly the general (integral) version of this. 

We next come to the notion of variance, which in our terminology is the uncertainty attached to our expectation. Having determined that the expected position of the particle is x (given by (12)), the resulting uncertainty is the quantity 

$$
\int_ {- \infty} ^ {\infty} (x - \overline {{x}}) ^ {2} | \psi (x) | ^ {2} d x.\tag{13}
$$

Notice that if $\psi$ is highly concentrated near ${ \overline { { x } } } ,$ it means that there is a high probability that $x$ is near ${ \overline { { x } } } ,$ and so (13) is small, because most of the contribution to the integral takes place for values of x near x. Here we have a small uncertainty. On the other hand, if ψ(x) is rather flat (that is, the probability distribution $| \psi ( x ) | ^ { 2 } d x$ is not very concentrated), then the integral (13) is rather big, because large values of $( x - { \overline { { x } } } ) ^ { 2 }$ will come into play, and as a result the uncertainty is relatively large. 

$$
\int_ {- \infty} ^ {\infty} (x - \overline {{x}}) ^ {2} | \psi (x) | ^ {2}
$$

$$
\overline {{x}},
$$

$$
2 \int_ {- \infty} ^ {\infty} (x - \bar {x}) | \psi (x) | ^ {2} d x = 0
$$

So far, we have discussed the “expectation” and “uncertainty” related to the position of the particle. Of equal relevance are the corresponding notions regarding its momentum. The corresponding rule of quantum mechanics is: 

• The probability that the momentum $\xi$ of the particle belongs to the interval $( a , b )$ is $\textstyle { \int _ { a } ^ { b } | \hat { \psi } ( \xi ) | ^ { 2 } d \xi }$ where ψ<sup>ˆ</sup> is the Fourier transform of ψ. 

## 5. Exercises

Combining these two laws with Theorem 4.1 gives $1 / 1 6 \pi ^ { 2 }$ as the lower bound for the product of the uncertainty of the position and the uncertainty of the momentum of a particle. So the more certain we are about the location of the particle, the less certain we can be about its momentum, and vice versa. However, we have simplified the statement of the two laws by rescaling to change the units of measurement. Actually, there enters a fundamental but small physical number ~ called Planck’s constant. When properly taken into account, the physical conclusion is 

(uncertainty of position)×(uncertainty of momentum) $\ge \hbar / 1 6 \pi ^ { 2 }$ 

## 5 Exercises

1. Corollary 2.3 in Chapter 2 leads to the following simplified version of the Fourier inversion formula. Suppose f is a continuous function supported on an interval $[ - M , M ]$ , whose Fourier transform <sup>ˆ</sup>f is of moderate decrease. 

(a) Fix L with $L / 2 > M$ , and show that $\begin{array} { r } { f ( x ) = \sum a _ { n } ( L ) e ^ { 2 \pi i n x / L } } \end{array}$ where 

$$
a _ {n} (L) = \frac {1}{L} \int_ {- L / 2} ^ {L / 2} f (x) e ^ {- 2 \pi i n x / L} d x = \frac {1}{L} \hat {f} (n / L).
$$

Alternatively, we may write $\begin{array} { r } { f ( x ) = \delta \sum _ { n = - \infty } ^ { \infty } \hat { f } ( n \delta ) e ^ { 2 \pi i n \delta x } \mathrm { ~ w i t h ~ } \delta = 1 / L } \end{array}$ 

(b) Prove that if F is continuous and of moderate decrease, then 

$$
\int_{-\infty}^{\infty}F(\xi)d\xi = \lim_{\substack{\delta \to 0\\ \delta >0}}\delta \sum_{n = -\infty}^{\infty}F(\delta n).
$$

(c) Conclude that $f ( x ) = \int _ { - \infty } ^ { \infty } { \hat { f } } ( \xi ) e ^ { 2 \pi i x \xi } d \xi .$ 

[Hint: For (a), note that the Fourier series of $f$ on $[ - L / 2 , L / 2 ]$ converges absolutely. For (b), first approximate the integral by $\int _ { - N } ^ { N } F$ and the sum by $\delta \sum _ { | n | \leq N / \delta } F ( n \delta )$ . Then approximate the second integral by Riemann sums.] 

2. Let f and g be the functions defined by 

$$
f (x) = \chi_ {[ - 1, 1 ]} (x) = \left\{ \begin{array}{l l} 1 & \text {if |x|\leq 1 ,} \\ 0 & \text {otherwise,} \end{array} \right. \quad \text {and} \quad g (x) = \left\{ \begin{array}{l l} 1 - | x | & \text {if |x|\leq 1 ,} \\ 0 & \text {otherwise.} \end{array} \right.
$$

Although $f$ is not continuous, the integral defining its Fourier transform still makes sense. Show that 

$$
\hat {f} (\xi) = \frac {\sin 2 \pi \xi}{\pi \xi} \quad \mathrm{and} \quad \hat {g} (\xi) = \left(\frac {\sin \pi \xi}{\pi \xi}\right) ^ {2},
$$

with the understanding that ${ \hat { f } } ( 0 ) = 2$ and $\hat { g } ( 0 ) = 1$ 

3. The following exercise illustrates the principle that the decay of $\hat { f }$ is related to the continuity properties of $f .$ 

(a) Suppose that $f$ is a function of moderate decrease on R whose Fourier transform $\hat { f }$ is continuous and satisfies 

$$
\hat {f} (\xi) = O \left(\frac {1}{| \xi | ^ {1 + \alpha}}\right) \quad \text { as } | \xi | \to \infty
$$

for some $0 < \alpha < 1$ . Prove that $f$ satisfies a H¨older condition of order $\alpha ,$ that is, that 

$$
| f (x + h) - f (x) | \leq M | h | ^ {\alpha} \quad \text {   for   some   } M > 0 \text {   and   all   } x, h \in \mathbb {R}.
$$

(b) Let f be a continuous function on R which vanishes for $| x | \geq 1$ , with $f ( 0 ) = 0$ , and which is equal to $1 / \log ( 1 / | x | )$ for all x in a neighborhood of the origin. Prove that $\hat { f }$ is not of moderate decrease. In fact, there is no $\epsilon > 0$ so that $\hat { f } ( \xi ) = O ( 1 / | \xi | ^ { 1 + \epsilon } )$ as $| \xi | \to \infty$ 

[Hint: For part $\mathrm { ( a ) }$ , use the Fourier inversion formula to express $f ( x + h ) - f ( x )$ as an integral involving ${ \hat { f } } ,$ and estimate this integral separately for $\xi$ in the two ranges $| \xi | \leq 1 / | h |$ and $| \xi | \geq 1 / | h | . ]$ 

4. Bump functions. Examples of compactly supported functions in $S ( \mathbb { R } )$ are very handy in many applications in analysis. Some examples are: 

(a) Suppose $a < b ,$ and $f$ is the function such that $f ( x ) = 0 { \mathrm { ~ i f ~ } } x \leq a { \mathrm { ~ o r ~ } } x \geq b$ and 

$$
f (x) = e ^ {- 1 / (x - a)} e ^ {- 1 / (b - x)} \quad \text { if } a <   x <   b.
$$

Show that $f$ is indefinitely diferentiable on R. 

(b) Prove that there exists an indefinitely diferentiable function F on R such that $F ( x ) = 0 { \mathrm { ~ i f ~ } } x \leq a , F ( x ) = 1 { \mathrm { ~ i f ~ } } x \geq b ,$ , and $F$ is strictly increasing on $[ a , b ]$ 

(c) Let $\delta > 0$ be so small that $a + \delta < b - \delta .$ . Show that there exists an indefinitely diferentiable function g such that g is $0 { \mathrm { ~ i f ~ } } x \leq$ a or $x \geq b ,$ g is 1 on $[ a + \delta , b - \delta ]$ , and $g$ is strictly monotonic on $[ a , a + \delta ]$ and $[ b - \delta , b ]$ 

[Hint: For (b) consider $\textstyle F ( x ) = c \int _ { - \infty } ^ { x } f ( t )$ dt where c is an appropriate constant.] 

5. Suppose $f$ is continuous and of moderate decrease. 

(a) Prove that $\hat { f }$ is continuous and ${ \hat { f } } ( \xi ) \to 0 { \mathrm { ~ a s ~ } } | \xi | \to \infty$ 

## 5. Exercises

(b) Show that if ${ \hat { f } } ( \xi ) = 0$ for all $\xi ,$ then f is identically 0. 

[Hint: For part (a), show that $\begin{array} { r } { \hat { f } ( \xi ) = \frac { 1 } { 2 } \int _ { - \infty } ^ { \infty } [ f ( x ) - f ( x - 1 / ( 2 \xi ) ) ] e ^ { - 2 \pi i x \xi } d x . } \end{array}$ For part (b), verify that the multiplication formula $\begin{array} { r } { \int f ( x ) \hat { g } ( x ) d x = \int \hat { f } ( y ) g ( y ) d y } \end{array}$ still holds whenever $g \in S ( \mathbb { R } ) .$ ] 

6. The function $e ^ { - \pi x ^ { 2 } }$ is its own Fourier transform. Generate other functions that (up to a constant multiple) are their own Fourier transforms. What must the constant multiples be? To decide this, prove that $\mathcal { F } ^ { 4 } = I$ . Here $\textstyle { \mathcal { F } } ( f ) = { \hat { f } }$ is the Fourier transform, $\mathcal { F } ^ { 4 } = \mathcal { F } \circ \mathcal { F } \circ \mathcal { F } \circ \mathcal { F }$ , and I is the identity operator $( I f ) ( x ) = f ( x )$ (see also Problem 7). 

7. Prove that the convolution of two functions of moderate decrease is a function of moderate decrease. 

[Hint: Write 

$$
\int f (x - y) g (y) d y = \int_ {| y | \leq | x | / 2} + \int_ {| y | \geq | x | / 2}.
$$

In the first integral $f ( x - y ) = O ( 1 / ( 1 + x ^ { 2 } ) )$ while in the second integral $g ( y ) = O ( 1 / ( 1 + x ^ { 2 } ) ) . ]$ ] 

8. Prove that $f$ is continuous, of moderate decrease, and $\begin{array} { r } { \int _ { - \infty } ^ { \infty } f ( y ) e ^ { - y ^ { 2 } } e ^ { 2 x y } d y = 0 } \end{array}$ for all $x \in \mathbb { R }$ , then $f = 0$ 

[Hint: Consider $f * e ^ { - x ^ { 2 } } . ]$ 

9. If $f$ is of moderate decrease, then 

$$
\int_ {- R} ^ {R} \left(1 - \frac {| \xi |}{R}\right) \hat {f} (\xi) e ^ {2 \pi i x \xi} d \xi = (f * \mathcal {F} _ {R}) (x),\tag{14}
$$

where the Fej´er kernel on the real line is defined by 

$$
\mathcal {F} _ {R} (t) = \left\{ \begin{array}{c l} R \left(\frac {\sin \pi t R}{\pi t R}\right) ^ {2} & \text { if } t \neq 0, \\ R & \text { if } t = 0. \end{array} \right.
$$

Show that $\{ \mathcal F _ { R } \}$ is a family of good kernels as $R \to \infty$ , and therefore (14) tends uniformly to $f ( x )$ as $R \to \infty$ . This is the analogue of Fej´er’s theorem for Fourier series in the context of the Fourier transform. 

10. Below is an outline of a diferent proof of the Weierstrass approximation theorem. 

Define the Landau kernels by 

$$
L _ {n} (x) = \left\{ \begin{array}{l l} \frac {(1 - x ^ {2}) ^ {n}}{c _ {n}} & \text { if } - 1 \leq x \leq 1, \\ 0 & \text { if } | x | \geq 1, \end{array} \right.
$$

where $c _ { n }$ is chosen so that $\textstyle \int _ { - \infty } ^ { \infty } L _ { n } ( x ) d x = 1$ . Prove that $\{ { L } _ { n } \} _ { n \geq 0 }$ is a family of good kernels as $n \to \infty$ . As a result, show that if f is a continuous function supported in $[ - 1 / 2 , 1 / 2 ]$ , then $( f * L _ { n } ) ( x )$ is a sequence of polynomials on $[ - 1 / 2 , 1 / 2 ]$ which converges uniformly to $f .$ 

[Hint: First show that $c _ { n } \geq 2 / ( n + 1 ) . ]$ 

11. Suppose that u is the solution to the heat equation given by $u = f * { \mathcal { H } } _ { t }$ where $f \in S ( \mathbb { R } )$ . If we also set $u ( x , 0 ) = f ( x )$ , prove that u is continuous on the closure of the upper half-plane, and vanishes at infinity, that is, 

$$
u (x, t) \rightarrow 0 \quad \mathrm{as} | x | + t \rightarrow \infty .
$$

[Hint: To prove that u vanishes at infinity, show that $( \mathrm { i } ) \ | u ( x , t ) | \leq C / \sqrt { t }$ and (ii) $\vert u ( x , t ) \vert \leq C / ( 1 + \vert x \vert ^ { 2 } ) + C t ^ { - 1 / 2 } e ^ { - c x ^ { 2 } / t }$ . Use (i) when $| x | \leq t ,$ and (ii) otherwise.] 

## 12. Show that the function defined by

$$
u (x, t) = \frac {x}{t} \mathcal {H} _ {t} (x)
$$

satisfies the heat equation for $t > 0$ and lim<sub>t</sub> $_ { + 0 } u ( x , t ) = 0$ for every $x ,$ but u is not continuous at the origin. 

[Hint: Approach the origin with $( x , t )$ on the parabola $x ^ { 2 } / 4 t = c$ where c is a constant.] 

13. Prove the following uniqueness theorem for harmonic functions in the strip $\{ ( x , y ) : 0 < y < 1$ , −∞ $< x < \infty \}$ : if u is harmonic in the strip, continuous on its closure with $u ( x , 0 ) = u ( x , 1 ) = 0$ for all $x \in \mathbb { R }$ , and u vanishes at infinity, then $u = 0$ 

14. Prove that the periodization of the Fej´er kernel $\mathcal { F } _ { N }$ on the real line (Exercise 9) is equal to the Fej´er kernel for periodic functions of period 1. In other words, 

$$
\sum_ {n = - \infty} ^ {\infty} \mathcal {F} _ {N} (x + n) = F _ {N} (x),
$$

when $N \geq 1$ is an integer, and where 

$$
F _ {N} (x) = \sum_ {n = - N} ^ {N} \left(1 - \frac {| n |}{N}\right) e ^ {2 \pi i n x} = \frac {1}{N} \frac {\sin^ {2} (N \pi x)}{\sin^ {2} (\pi x)}.
$$

5. Exercises 

15. This exercise provides another example of periodization. 

(a) Apply the Poisson summation formula to the function $g$ in Exercise 2 to obtain 

$$
\sum_ {n = - \infty} ^ {\infty} \frac {1}{(n + \alpha) ^ {2}} = \frac {\pi^ {2}}{(\sin \pi \alpha) ^ {2}}
$$

whenever α is real, but not equal to an integer. 

(b) Prove as a consequence that 

$$
\sum_ {n = - \infty} ^ {\infty} \frac {1}{(n + \alpha)} = \frac {\pi}{\tan \pi \alpha}\tag{15}
$$

whenever α is real but not equal to an integer. [Hint: First prove it when $0 < \alpha < 1$ . To do so, integrate the formula in (b). What is the precise meaning of the series on the left-hand side of (15)? Evaluate at $\alpha = 1 / 2 . ]$ 

16. The Dirichlet kernel on the real line is defined by 

$$
\int_ {- R} ^ {R} \hat {f} (\xi) e ^ {2 \pi i x \xi} d \xi = (f * \mathcal {D} _ {R}) (x) \quad \text {so that} \quad \mathcal {D} _ {R} (x) = \widehat {\chi_ {[ - R , R ]}} (x) = \frac {\sin (2 \pi R x)}{\pi x}.
$$

Also, the modified Dirichlet kernel for periodic functions of period 1 is defined by 

$$
D _ {N} ^ {*} (x) = \sum_ {| n | \leq N - 1} e ^ {2 \pi i n x} + \frac {1}{2} (e ^ {- 2 \pi i N x} + e ^ {2 \pi i N x}).
$$

Show that the result in Exercise 15 gives 

$$
\sum_ {n = - \infty} ^ {\infty} \mathcal {D} _ {N} (x + n) = D _ {N} ^ {*} (x),
$$

where $N \geq 1$ is an integer, and the infinite series must be summed symmetrically. In other words, the periodization of $\mathcal { D } _ { N }$ is the modified Dirichlet kernel $D _ { N } ^ { * }$ 

17. The gamma function is defined for $s > 0$ by 

$$
\Gamma (s) = \int_ {0} ^ {\infty} e ^ {- x} x ^ {s - 1} d x.
$$

(a) Show that for $s > 0$ the above integral makes sense, that ${ \mathrm { i s } } ,$ that the following two limits exist: 

$$
\lim_{\substack{\delta \to 0\\ \delta >0}}\int_{\delta}^{1}e^{-x}x^{s - 1}  dx\quad \text{and}\quad \lim_{A\to \infty}\int_{1}^{A}e^{-x}x^{s - 1}  dx.
$$

(b) Prove that $\Gamma ( s + 1 ) = s \Gamma ( s )$ whenever $s > 0 ,$ , and conclude that for every integer $n \geq 1$ we have $\Gamma ( n + 1 ) = n !$ 

(c) Show that 

$$
\Gamma \left(\frac {1}{2}\right) = \sqrt {\pi} \quad \text { and } \quad \Gamma \left(\frac {3}{2}\right) = \frac {\sqrt {\pi}}{2}.
$$

[Hint: For (c), use $\textstyle \int _ { - \infty } ^ { \infty } e ^ { - \pi x ^ { 2 } } d x = 1 . ]$ 

18. The zeta function is defined for $s > 1$ by $\textstyle \zeta ( s ) = \sum _ { n = 1 } ^ { \infty } 1 / n ^ { s }$ . Verify the identity 

$$
\pi^ {- s / 2} \Gamma (s / 2) \zeta (s) = \frac {1}{2} \int_ {0} ^ {\infty} t ^ {\frac {s}{2} - 1} (\vartheta (t) - 1) d t \quad \text { whenever } s > 1
$$

where Γ and ϑ are the gamma and theta functions, respectively: 

$$
\Gamma (s) = \int_ {0} ^ {\infty} e ^ {- t} t ^ {s - 1} d t \quad \text { and } \quad \vartheta (s) = \sum_ {n = - \infty} ^ {\infty} e ^ {- \pi n ^ {2} s}.
$$

More about the zeta function and its relation to the prime number theorem can be found in Book II. 

19. The following is a variant of the calculation of $\begin{array} { r } { \zeta ( 2 m ) = \sum _ { n = 1 } ^ { \infty } 1 / n ^ { 2 m } } \end{array}$ found in Problem 4, Chapter 3. 

(a) Apply the Poisson summation formula $\begin{array} { r l } { \mathrm { t o } } & { { } f ( x ) = t / ( \pi ( x ^ { 2 } + t ^ { 2 } ) ) } \end{array}$ and ${ \hat { f } } ( \xi ) = e ^ { - 2 \pi t | \xi | }$ where $t > 0$ in order to get 

$$
\frac {1}{\pi} \sum_ {n = - \infty} ^ {\infty} \frac {t}{t ^ {2} + n ^ {2}} = \sum_ {n = - \infty} ^ {\infty} e ^ {- 2 \pi t | n |}.
$$

(b) Prove the following identity valid for $0 < t < 1$ : 

$$
\frac {1}{\pi} \sum_ {n = - \infty} ^ {\infty} \frac {t}{t ^ {2} + n ^ {2}} = \frac {1}{\pi t} + \frac {2}{\pi} \sum_ {m = 1} ^ {\infty} (- 1) ^ {m + 1} \zeta (2 m) t ^ {2 m - 1}
$$

as well as 

$$
\sum_ {n = - \infty} ^ {\infty} e ^ {- 2 \pi t | n |} = \frac {2}{1 - e ^ {- 2 \pi t}} - 1.
$$

5. Exercises 

(c) Use the fact that 

$$
{\frac {z}{e ^ {z} - 1}} = 1 - {\frac {z}{2}} + \sum_ {m = 1} ^ {\infty} {\frac {B _ {2 m}}{(2 m) !}} z ^ {2 m},
$$

where $B _ { k }$ are the Bernoulli numbers to deduce from the above formula, 

$$
2 \zeta (2 m) = (- 1) ^ {m + 1} \frac {(2 \pi) ^ {2 m}}{(2 m) !} B _ {2 m}.
$$

20. The following results are relevant in information theory when one tries to recover a signal from its samples. 

Suppose $f$ is of moderate decrease and that its Fourier transform $\hat { f }$ is supported in $I = [ - 1 / 2 , 1 / 2 ]$ . Then, $f$ is entirely determined by its restriction to $\mathbb { Z } .$ This means that if g is another function of moderate decrease whose Fourier transform is supported in I and $f ( n ) = g ( n )$ for all $n \in \mathbb { Z }$ , then $f = g$ . More precisely: 

(a) Prove that the following reconstruction formula holds: 

$$
f (x) = \sum_ {n = - \infty} ^ {\infty} f (n) K (x - n) \quad \text { where } K (y) = \frac {\sin \pi y}{\pi y}.
$$

Note that $K ( y ) = O ( 1 / | y | ) { \mathrm { ~ a s ~ } } | y | \to \infty$ 

(b) If $\lambda > 1$ , then 

$$
f (x) = \sum_ {n = - \infty} ^ {\infty} \frac {1}{\lambda} f \left(\frac {n}{\lambda}\right) K _ {\lambda} \left(x - \frac {n}{\lambda}\right) \quad \text {where} K _ {\lambda} (y) = \frac {\cos \pi y - \cos \pi \lambda y}{\pi^ {2} (\lambda - 1) y ^ {2}}.
$$

Thus, if one samples $f$ “more often $, ^ { , }$ the series in the reconstruction formula converges faster since $K _ { \lambda } ( y ) = O ( 1 / | y | ^ { 2 } )$ as $| y | \to \infty$ . Note that $K _ { \lambda } ( y ) \to K ( y )$ as $\lambda \to 1$ 

$$
\text {(c)} \text { Prove   that } \int_ {- \infty} ^ {\infty} | f (x) | ^ {2} d x = \sum_ {n = - \infty} ^ {\infty} | f (n) | ^ {2}.
$$

[Hint: For part (a) show that if $\chi$ is the characteristic function of $I ,$ then ${ \hat { f } } ( \xi ) = \chi ( \xi ) \sum _ { n = - \infty } ^ { \infty } { f ( n ) e }$ <sup>−2πinξ</sup>. For (b) use the function in Figure 2 instead of $\chi ( \xi ) . ]$ 

21. Suppose that $f$ is continuous on R. Show that $f$ and $\hat { f }$ cannot both be compactly supported unless $f = 0$ . This can be viewed in the same spirit as the uncertainty principle. 

Chapter 5. THE FOURIER TRANSFORM ON R 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/e516722f9beadbe327cba4e5c338142733b7d6195bf6fa2e273fca1f86ba6809.jpg)



Figure 2. The function in Exercise 20


[Hint: Assume $f$ is supported in $[ 0 , 1 / 2 ]$ . Expand f in a Fourier series in the interval [0, 1], and note that as a result, f is a trigonometric polynomial.] 

22. The heuristic assertion stated before Theorem 4.1 can be made precise as follows. If F is a function on R, then we say that the preponderance of its mass is contained in an interval I (centered at the origin) if 

$$
\int_ {I} x ^ {2} | F (x) | ^ {2} d x \geq \frac {1}{2} \int_ {\mathbb {R}} x ^ {2} | F (x) | ^ {2} d x.\tag{16}
$$

Now suppose $f \in S$ , and (16) holds with $F = f$ and $I = I _ { 1 } ;$ also with $\boldsymbol { F } = \boldsymbol { \hat { f } }$ and $I = I _ { 2 }$ . Then if $L _ { j }$ denotes the length of $I _ { j } { \mathrm { : } }$ , we have 

$$
L _ {1} L _ {2} \geq \frac {1}{2 \pi}.
$$

A similar conclusion holds if the intervals are not necessarily centered at the origin. 

23. The Heisenberg uncertainty principle can be formulated in terms of the operator $\textstyle L = - { \frac { d ^ { 2 } } { d x ^ { 2 } } } + x ^ { 2 }$ , which acts on Schwartz functions by the formula 

$$
L (f) = - \frac {d ^ {2} f}{d x ^ {2}} + x ^ {2} f.
$$

This operator, sometimes called the Hermite operator, is the quantum analogue of the harmonic oscillator. Consider the usual inner product on $s$ given by 

$$
(f, g) = \int_ {- \infty} ^ {\infty} f (x) \overline {{g (x)}} d x \quad \text { whenever } f, g \in \mathcal {S}.
$$

6. Problems 

(a) Prove that the Heisenberg uncertainty principle implies 

$$
(L f, f) \geq (f, f) \quad \text {   for   all   } f \in \mathcal {S}.
$$

This is usually denoted by $L \geq I .$ [Hint: Integrate by parts.] 

(b) Consider the operators A and $A ^ { * }$ defined on $s$ by 

$$
A (f) = \frac {d f}{d x} + x f \quad \text { and } \quad A ^ {*} (f) = - \frac {d f}{d x} + x f.
$$

The operators A and $A ^ { * }$ are sometimes called the annihilation and creation operators, respectively. Prove that for all $f , g \in S$ we have 

(i) $( A f , g ) = ( f , A ^ { * } g ) ,$ 

(ii) $( A f , A f ) = ( A ^ { * } A f , f ) \geq 0 ,$ 

(iii) $A ^ { * } A = L - I .$ 

In particular, this again shows that $L \geq I$ 

(c) Now for $t \in \mathbb { R }$ , let 

$$
A _ {t} (f) = \frac {d f}{d x} + t x f \quad \text { and } \quad A _ {t} ^ {*} (f) = - \frac {d f}{d x} + t x f.
$$

Use the fact that $\left( A _ { t } ^ { \ast } A _ { t } f , f \right) \geq 0$ to give another proof of the Heisenberg uncertainty principle which says that whenever $\begin{array} { r } { \int _ { - \infty } ^ { \infty } | f ( x ) | ^ { 2 } d x = 1 } \end{array}$ then 

$$
\left(\int_ {- \infty} ^ {\infty} x ^ {2} | f (x) | ^ {2} d x\right) \left(\int_ {- \infty} ^ {\infty} \left| \frac {d f}{d x} \right| ^ {2} d x\right) \geq 1 / 4.
$$

[Hint: Think of $( A _ { t } ^ { * } A _ { t } f , f )$ as a quadratic polynomial in $t . ]$ 

## 6 Problems

1. The equation 

$$
x ^ {2} \frac {\partial^ {2} u}{\partial x ^ {2}} + a x \frac {\partial u}{\partial x} = \frac {\partial u}{\partial t}\tag{17}
$$

with $u ( x , 0 ) = f ( x )$ for $0 < x < \infty$ and $t > 0$ is a variant of the heat equation which occurs in a number of applications. To solve $( 1 7 )$ , make the change of variables $x = e ^ { - y } \quad \mathrm { s o }$ that $- \infty < y < \infty$ Set $U ( y , t ) = u ( e ^ { - y } , t )$ and $F ( y ) = f ( e ^ { - y } )$ . Then the problem reduces to the equation 

$$
\frac {\partial^ {2} U}{\partial y ^ {2}} + (1 - a) \frac {\partial U}{\partial y} = \frac {\partial U}{\partial t},
$$

with $U ( y , 0 ) = F ( y )$ . This can be solved like the usual heat equation (the case $a = 1 )$ by taking the Fourier transform in the y variable. One must then compute the integral $\begin{array} { r } { \int _ { - \infty } ^ { \infty } e ^ { ( - 4 \pi ^ { 2 } \xi ^ { 2 } + ( 1 - a ) 2 \pi i \xi ) t } e ^ { 2 \pi i \xi v } d \xi } \end{array}$ . Show that the solution of the original problem is then given by 

$$
u (x, t) = \frac {1}{(4 \pi t) ^ {1 / 2}} \int_ {0} ^ {\infty} e ^ {- (\log (v / x) + (1 - a) t) ^ {2} / (4 t)} f (v) \frac {d v}{v}.
$$

2. The Black-Scholes equation from finance theory is 

$$
\frac {\partial V}{\partial t} + r s \frac {\partial V}{\partial s} + \frac {\sigma^ {2} s ^ {2}}{2} \frac {\partial^ {2} V}{\partial s ^ {2}} - r V = 0, \quad 0 <   t <   T,\tag{18}
$$

subject to the “final” boundary condition $V ( s , T ) = F ( s )$ . An appropriate change of variables reduces this to the equation in Problem 1. Alternatively, the substitution $V ( s , t ) = e ^ { a x + b \tau } U ( x , \tau )$ where x = log $\begin{array} { r } { s , \tau = \frac { \sigma ^ { 2 } } { 2 } ( T - t ) , a = \frac { 1 } { 2 } - \frac { r } { \sigma ^ { 2 } } } \end{array}$ , and $\begin{array} { r } { b = - \left( { \frac { 1 } { 2 } } + { \frac { r } { \sigma ^ { 2 } } } \right) ^ { 2 } } \end{array}$ reduces (18) to the one-dimensional heat equation with the initial condition $\stackrel { \prime } { U } ( x , 0 ) = e ^ { - a x } F ( e ^ { x } )$ . Thus a solution to the Black-Scholes equation is 

$$
V (s, t) = \frac {e ^ {- r (T - t)}}{\sqrt {2 \pi \sigma^ {2} (T - t)}} \int_ {0} ^ {\infty} e ^ {- \frac {(\log (s / s ^ {*}) + (r - \sigma^ {2} / 2) (T - t)) ^ {2}}{2 \sigma^ {2} (T - t)}} F (s ^ {*}) d s ^ {*}.
$$

3. <sup>∗</sup> The Dirichlet problem in a strip. Consider the equation $\triangle u = 0$ in the horizontal strip 

$$
\{(x, y): 0 <   y <   1, - \infty <   x <   \infty \}
$$

with boundary conditions $u ( x , 0 ) = f _ { 0 } ( x )$ and $u ( x , 1 ) = f _ { 1 } ( x )$ , where $f _ { 0 }$ and $f _ { 1 }$ are both in the Schwartz space. 

(a) Show (formally) that if u is a solution to this problem, then 

$$
\hat {u} (\xi , y) = A (\xi) e ^ {2 \pi \xi y} + B (\xi) e ^ {- 2 \pi \xi y}.
$$

Express A and B in terms of $\widehat { f } _ { 0 }$ and $\widehat { f } _ { 1 }$ , and show that 

$$
\hat {u} (\xi , y) = \frac {\sinh (2 \pi (1 - y) \xi)}{\sinh (2 \pi \xi)} \widehat {f} _ {0} (\xi) + \frac {\sinh (2 \pi y \xi)}{\sinh (2 \pi \xi)} \widehat {f} _ {0} (\xi).
$$

(b) Prove as a result that 

$$
\int_ {- \infty} ^ {\infty} | u (x, y) - f _ {0} (x) | ^ {2} d x \rightarrow 0 \quad \text { as } y \rightarrow 0
$$

and 

$$
\int_ {- \infty} ^ {\infty} | u (x, y) - f _ {1} (x) | ^ {2} d x \to 0 \quad \text { as } y \to 1.
$$

6. Problems 

(c) If $\Phi ( \xi ) = ( \sinh 2 \pi a \xi ) / ( \sinh 2 \pi \xi )$ , with $0 \leq a < 1$ , then Φ is the Fourier transform of $\varphi$ where 

$$
\varphi (x) = \frac {\sin \pi a}{2} \cdot \frac {1}{\cosh \pi x + \cos \pi a}.
$$

This can be shown, for instance, by using contour integration and the residue formula from complex analysis (see Book II, Chapter 3). 

(d) Use this result to express u in terms of Poisson-like integrals involving $f _ { 0 }$ and $f _ { 1 }$ as follows: 

$$
u (x, y) = \frac {\sin \pi y}{2} \left(\int_ {- \infty} ^ {\infty} \frac {f _ {0} (x - t)}{\cosh \pi t - \cos \pi y} d t + \int_ {- \infty} ^ {\infty} \frac {f _ {1} (x - t)}{\cosh \pi t + \cos \pi y} d t\right).
$$

(e) Finally, one can check that the function $u ( x , y )$ defined by the above expression is harmonic in the strip, and converges uniformly to $f _ { 0 } ( x )$ as $y  0 .$ , and to $f _ { 1 } ( x )$ as $y  1$ . Moreover, one sees that $u ( x , y )$ vanishes at infinity, that is, lim $1 _ { | x |  \infty } u ( x , y ) = 0$ , uniformly in $y .$ 

In Exercise 12, we gave an example of a function that satisfies the heat equation in the upper half-plane, with boundary value 0, but which was not identically 0. We observed in this case that u was in fact not continuous up to the boundary. 

In Problem 4 we exhibit examples illustrating non-uniqueness, but this time with continuity up to the boundary $t = 0$ . These examples satisfy a growth condition at infinity, namely $| u ( x , t ) | \leq C e ^ { c x ^ { 2 + \epsilon } }$ , for any $\epsilon > 0$ . Problems 5 and 6 show that under the more restrictive growth condition $| u ( x , t ) | \leq C e ^ { c x ^ { 2 } }$ , uniqueness does hold. 

4.<sup>∗</sup> If $g$ is a smooth function on $\mathbb { R } ,$ define the formal power series 

$$
u (x, t) = \sum_ {n = 0} ^ {\infty} g ^ {(n)} (t) \frac {x ^ {2 n}}{(2 n !)}.\tag{19}
$$

(a) Check formally that u solves the heat equation. 

(b) For $a > 0 ,$ consider the function defined by 

$$
g (t) = \left\{ \begin{array}{l l} e ^ {- t ^ {- a}} & \text { if } t > 0 \\ 0 & \text { if } t \leq 0. \end{array} \right.
$$

One can show that there exists $0 < \theta < 1$ depending on a so that 

$$
| g ^ {(k)} (t) | \leq \frac {k !}{(\theta t) ^ {k}} e ^ {- \frac {1}{2} t ^ {- a}} \quad \text { for } t > 0.
$$

(c) As a result, for each x and t the series (19) converges; u solves the heat equation; u vanishes for $t = 0 ;$ ; and u satisfies the estimate $| u ( x , t ) | \leq$ $\bar { C e ^ { c | x | ^ { 2 a / ( a - 1 ) } } }$ for some constants $C , c > 0$ 

(d) Conclude that for every $\epsilon > 0$ there exists a non-zero solution to the heat equation which is continuous for $x \in$ R and $t \geq 0 ,$ , which satisfies $u ( x , 0 ) =$ 0 and $| u ( x , t ) | \leq C e ^ { c | x | ^ { 2 + \epsilon } }$ 

5.<sup>∗</sup> The following “maximum principle” for solutions of the heat equation will be used in the next problem. 

Theorem. Suppose that $u ( x , t )$ is a real-valued solution of the heat equation in the upper half-plane, which is continuous on its closure. Let R denote the rectangle 

$$
R = \{(x, y) \in \mathbb {R} ^ {2}: a \leq x \leq b, 0 \leq t \leq c \}
$$

and $\partial ^ { \prime } R$ be the part of the boundary of R which consists of the two vertical sides and its base on the line $t = 0$ (see Figure 3). Then 

$$
\min _ {(x, t) \in \partial^ {\prime} R} u (x, t) = \min _ {(x, t) \in R} u (x, t) \quad a n d \quad \max _ {(x, t) \in \partial^ {\prime} R} u (x, t) = \max _ {(x, t) \in R} u (x, t).
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/c829883d-1499-46d4-87be-49f87e08c5bf/2ea6c4f8eb2c48fbd6716ac437bd75d13aff40172208e0a8b632002f57b957cc.jpg)



Figure 3. The rectangle R and part of its boundary $\partial ^ { \prime } R$


The steps leading to a proof of this result are outlined below. 

(a) Show that it sufices to prove that if $u \geq 0$ on $\partial ^ { \prime } R ,$ , then $u \geq 0$ in R. 

(b) For $\epsilon > 0 ,$ , let 

$$
v (x, t) = u (x, t) + \epsilon t.
$$

Then, v has a minimum on R, say at $( x _ { 1 } , t _ { 1 } )$ . Show that $x _ { 1 } = a$ or b, or else $t _ { 1 } = 0 .$ . To do so, suppose on the contrary that $a < x _ { 1 } < b$ and $0 < t _ { 1 } \le c$ , and prove that $v _ { x x } ( x _ { 1 } , t _ { 1 } ) - v _ { t } ( x _ { 1 } , t _ { 1 } ) \leq - \epsilon$ . However, show also that the left-hand side must be non-negative. 

(c) Deduce from (b) that $u ( x , t ) \geq \epsilon ( t _ { 1 } - t )$ for any $( x , t ) \in R$ and let $\epsilon \to 0$ 

## 6. Problems

Theorem. Suppose $\boldsymbol { u } ( \boldsymbol { x } , t )$ satisfies the following conditions: 

(i) $u ( x , t )$ solves the heat equation for all $x \in \mathbb { R }$ and and all $t > 0$ 

(ii) $u ( x , t )$ is continuous for all $x \in \mathbb { R }$ and $0 \leq t \leq c .$ 

(iii) $u ( x , 0 ) = 0 .$ 

(iv) $| u ( x , t ) | \leq M e ^ { a x ^ { 2 } }$ for some $M , a ,$ , and all $x \in \mathbb { R } , 0 \leq t < c$ 

Then u is identically equal to 0. 

$^ { 7 . ^ { * } }$ The Hermite functions $h _ { k } ( x )$ are defined by the generating identity 

$$
\sum_ {k = 0} ^ {\infty} h _ {k} (x) \frac {t ^ {k}}{k !} = e ^ {- (x ^ {2} / 2 - 2 t x + t ^ {2})}.
$$

(a) Show that an alternate definition of the Hermite functions is given by the formula 

$$
h _ {k} (x) = (- 1) ^ {k} e ^ {x ^ {2} / 2} \left(\frac {d}{d x}\right) ^ {k} e ^ {- x ^ {2}}.
$$

[Hint: Write $e ^ { - ( x ^ { 2 } / 2 - 2 t x + t ^ { 2 } ) } = e ^ { x ^ { 2 } / 2 } e ^ { - ( x - t ) ^ { 2 } }$ and use Taylor’s formula.] Conclude from the above expression that each $h _ { k } ( x )$ is of the form $P _ { k } ( x ) e ^ { - x ^ { 2 } / 2 }$ , where $P _ { k }$ is a polynomial of degree k. In particular, the Hermite functions belong to the Schwartz space and $h _ { 0 } ( x ) = e ^ { - x ^ { 2 } / 2 }$ $h _ { 1 } ( x ) = 2 x e ^ { - x ^ { 2 } / 2 }$ 

(b) Prove that the family $\{ h _ { k } \} _ { k = 0 } ^ { \infty }$ is complete in the sense that if $f$ is a Schwartz function, and 

$$
(f, h _ {k}) = \int_ {- \infty} ^ {\infty} f (x) h _ {k} (x) d x = 0 \quad \text { for   all } k \geq 0,
$$

then $f = 0 .$ [Hint: Use Exercise 8.] 

(c) Define $h _ { k } ^ { * } ( x ) = h _ { k } ( ( 2 \pi ) ^ { 1 / 2 } x )$ . Then 

$$
\widehat {h _ {k} ^ {*}} (\xi) = (- i) ^ {k} h _ {k} ^ {*} (\xi).
$$

Therefore, each $h _ { k } ^ { * }$ is an eigenfunction for the Fourier transform. 

(d) Show that $h _ { k }$ is an eigenfunction for the operator defined in Exercise 23, and in fact, prove that 

$$
L h _ {k} = (2 k + 1) h _ {k}.
$$

In particular, we conclude that the functions $h _ { k }$ are mutually orthogonal for the $L ^ { 2 }$ inner product on the Schwartz space. 

(e) Finally, show that $\begin{array} { r } { \int _ { - \infty } ^ { \infty } [ h _ { k } ( x ) ] ^ { 2 } d x = \pi ^ { 1 / 2 } 2 ^ { k } k ! . } \end{array}$ . [Hint: Square the generating relation.] 

8.<sup>∗</sup> To refine the results in Chapter 4, and to prove that 

$$
f _ {\alpha} (x) = \sum_ {n = 0} ^ {\infty} 2 ^ {- n \alpha} e ^ {2 \pi i 2 ^ {n} x}
$$

is nowhere diferentiable even in the case $\alpha = 1$ , we need to consider a variant of the delayed means $\triangle _ { N }$ , which in turn will be analyzed by the Poisson summation formula. 

(a) Fix an indefinitely diferentiable function Φ satisfying 

$$
\Phi (\xi) = \left\{ \begin{array}{l l} 1 & \text { when } | \xi | \leq 1, \\ 0 & \text { when } | \xi | \geq 2. \end{array} \right.
$$

By the Fourier inversion formula, there exists $\varphi \in { S }$ so that ${ \hat { \varphi } } ( \xi ) = \Phi ( \xi )$ Let $\varphi _ { N } ( x ) = N \varphi ( N x )$ so that $\widehat { \varphi _ { N } } ( \xi ) = \Phi ( \xi / N )$ . Finally, set 

$$
\tilde {\triangle} _ {N} (x) = \sum_ {n = - \infty} ^ {\infty} \varphi_ {N} (x + n).
$$

Observe by the Poisson summation formula that $\tilde { \triangle } _ { N } ( x ) =$ $\stackrel { \infty } { \sum _ { n = - \infty } ^ { \infty } } \Phi ( \stackrel {  } { n } / N ) e ^ { 2 \pi i n x }$ , thus $\tilde { \triangle } _ { N }$ is a trigonometric polynomial of degree $\leq 2 N$ , with terms whose coeficients are 1 when $| n | \leq N$ . Let 

$$
\tilde {\triangle} _ {N} (f) = f * \tilde {\triangle} _ {N}.
$$

Note that 

$$
S _ {N} (f _ {\alpha}) = \tilde {\triangle} _ {N ^ {\prime}} (f _ {\alpha})
$$

where $N ^ { \prime }$ is the largest integer of the form $2 ^ { k }$ with $N ^ { \prime } \leq N$ 

(b) If we set $\tilde { \triangle } _ { N } ( x ) = \varphi _ { N } ( x ) + E _ { N } ( x )$ where 

$$
E _ {N} (x) = \sum_ {| n | \geq 1} \varphi_ {N} (x + n),
$$

then one sees that: 

(i) $\begin{array} { r } { \operatorname* { s u p } _ { | x | \leq 1 / 2 } | E _ { N } ^ { \prime } ( x ) | \to 0 \mathrm { ~ a s ~ } N \to \infty . } \end{array}$ 

(ii) $| \tilde { \triangle } _ { N } ^ { \prime } ( x ) | \leq c N ^ { 2 } .$ 

(iii) $| \tilde { \triangle } _ { N } ^ { \prime } ( x ) | \leq c / ( N | x | ^ { 3 } ) , \mathrm { f o r } | x | \leq 1 / 2 .$ 

Moreover, $\begin{array} { r } { \int _ { | x | \leq 1 / 2 } \tilde { \triangle } _ { N } ^ { \prime } ( x ) d x = 0 . } \end{array}$ , and − $\begin{array} { r } { \int _ { | x | \leq 1 / 2 } x \tilde { \triangle } _ { N } ^ { \prime } ( x ) d x \to 1 } \end{array}$ as $N $ ∞. 

(c) The above estimates imply that if $f ^ { \prime } ( x _ { 0 } )$ exists, then 

$$
(f * \tilde {\triangle} _ {N} ^ {\prime}) (x _ {0} + h _ {N}) \to f ^ {\prime} (x _ {0}) \quad \mathrm{as} N \to \infty ,
$$

whenever $| h _ { N } | \leq C / N$ . Then, conclude that both the real and imaginary parts of $f _ { 1 }$ are nowhere diferentiable, as in the proof given in Section $^ { 3 , }$ Chapter 4. 

# 6 <sub>The</sub> <sub>Fourier</sub> <sub>Transform</sub> <sub>on</sub> $\mathbb { R } ^ { d }$

It occurred to me that in order to improve treatment planning one had to know the distribution of the attenuation coeficient of tissues in the body. This information would be useful for diagnostic purposes and would constitute a tomogram or series of tomograms. 

It was immediately evident that the problem was a mathematical one. If a fine beam of gamma rays of intensity $I _ { 0 }$ is incident on the body and the emerging density is $I ,$ then the measurable quantity g equals $\textstyle \log ( I _ { 0 } / I ) = \int _ { L } f d s$ , where f is the variable absorption coeficient along the line $L .$ Hence if f is a function of two dimensions, and g is known for all lines intersecting the body, the question is, can $f$ be determined if g is known? 

Fourteen years would elapse before I learned that Radon had solved this problem in 1917. 

A. M. Cormack, 1979 

The previous chapter introduced the theory of the Fourier transform on R and illustrated some of its applications to partial diferential equations. Here, our aim is to present an analogous theory for functions of several variables. 

After a brief review of some relevant notions in $\mathbb { R } ^ { d }$ , we begin with some general facts about the Fourier transform on the Schwartz space $S ( \mathbb { R } ^ { d } )$ Fortunately, the main ideas and techniques have already been considered in the one-dimensional case. In fact, with the appropriate notation, the statements (and proofs) of the key theorems, such as the Fourier inversion and Plancherel formulas, remain unchanged. 

Next, we highlight the connection to some higher dimensional problems in mathematical physics, and in particular we investigate the wave equation in d dimensions, with a detailed analysis in the cases $d = 3$ and $d = 2$ . At this stage, we discover a rich interplay between the Fourier transform and rotational symmetry, that arises only in $\mathbb { R } ^ { d }$ when $d \geq 2$ 

Finally, the chapter ends with a discussion of the Radon transform. This topic is of substantial interest in its own right, but in addition has significant relevance in its application to the use of X-ray scans as well 

as to other parts of mathematics. 

## 1 Preliminaries

The setting in this chapter will be $\mathbb { R } ^ { d } .$ , the vector $\mathrm { s p a c e } ^ { 1 }$ of all d-tuples of real numbers $( x _ { 1 } , \ldots , x _ { d } )$ with $x _ { i } \in \mathbb { R }$ . Addition of vectors is componentwise, and so is multiplication by real scalars. Given $x = ( x _ { 1 } , \ldots , x _ { d } ) \in \mathbb { R } ^ { d }$ we define 

$$
| x | = (x _ {1} ^ {2} + \dots + x _ {d} ^ {2}) ^ {1 / 2},
$$

so that |x| is simply the length of the vector x in the usual Euclidean norm. In fact, we equip $\mathbb { R } ^ { d }$ with the standard inner product defined by 

$$
x \cdot y = x _ {1} y _ {1} + \dots + x _ {d} y _ {d},
$$

so that $| x | ^ { 2 } = x \cdot x$ . We use the notation $x \cdot y$ in place of $( x , y )$ of Chapter 3. 

Given a d-tuple $\alpha = ( \alpha _ { 1 } , \ldots , \alpha _ { d } )$ of non-negative integers (sometimes called a multi-index), the monomial $x ^ { \alpha }$ is defined by 

$$
x ^ {\alpha} = x _ {1} ^ {\alpha_ {1}} x _ {2} ^ {\alpha_ {2}} \dots x _ {d} ^ {\alpha_ {d}}.
$$

Similarly, we define the diferential operator $( \partial / \partial x ) ^ { \alpha }$ by 

$$
\left(\frac {\partial}{\partial x}\right) ^ {\alpha} = \left(\frac {\partial}{\partial x _ {1}}\right) ^ {\alpha_ {1}} \left(\frac {\partial}{\partial x _ {2}}\right) ^ {\alpha_ {2}} \dots \left(\frac {\partial}{\partial x _ {d}}\right) ^ {\alpha_ {d}} = \frac {\partial^ {| \alpha |}}{\partial x _ {1} ^ {\alpha_ {1}} \cdots \partial x _ {d} ^ {\alpha_ {d}}},
$$

where $| \alpha | = \alpha _ { 1 } + \cdot \cdot \cdot + \alpha _ { d }$ is the order of the multi-index $\alpha$ . 

## 1.1 Symmetries

Analysis in $\mathbb { R } ^ { d }$ , and in particular the theory of the Fourier transform, is shaped by three important groups of symmetries of the underlying space: 

(i) Translations 

(ii) Dilations 

(iii) Rotations 

## 1. Preliminaries

We have seen that translations $x \mapsto x + h$ , with $h \in \mathbb { R } ^ { d }$ fixed, and dilations $x \mapsto \delta x .$ , with $\delta > 0$ , play an important role in the one-dimensional theory. In R, the only two rotations are the identity and multiplication by −1. However, in $\mathbb { R } ^ { d }$ with $d \geq 2$ there are more rotations, and the understanding of the interaction between the Fourier transform and rotations leads to fruitful insights regarding spherical symmetries. 

A rotation in $\mathbb { R } ^ { d }$ is a linear transformation $R : \mathbb { R } ^ { d }  \mathbb { R } ^ { d }$ which preserves the inner product. In other words, 

$R ( a x + b y ) = a R ( x ) + b R ( y )$ for all x, $\boldsymbol { y } \in \mathbb { R } ^ { d }$ and $a , b \in \mathbb { R }$ 

$R ( x ) \cdot R ( y ) = x \cdot y$ for all $x , y \in \mathbb { R } ^ { d }$ 

Equivalently, this last condition can be replaced by $| R ( x ) | = | x |$ for all x $\mathbf { \chi } ) \in \mathbb { R } ^ { d }$ , or $R ^ { t } = R ^ { - 1 }$ where $R ^ { t }$ and $R ^ { - 1 }$ denote the transpose and inverse of $R ,$ respectively.<sup>2</sup> In particular, we have det $( R ) = \pm 1$ , where det(R) is the determinant of R. If $\operatorname* { d e t } ( R ) = 1$ we say that R is a proper rotation; otherwise, we say that R is an improper rotation. 

Example 1. On the real line R, there are two rotations: the identity which is proper, and multiplication by −1 which is improper. 

Example 2. The rotations in the plane $\mathbb { R } ^ { 2 }$ can be described in terms of complex numbers. We identify $\mathbb { R } ^ { 2 }$ with C by assigning the point $( x , y )$ to the complex number $z = x + i y$ . Under this identification, all proper rotations are of the form $z \mapsto z e ^ { i \varphi }$ for some $\varphi \in \mathbb { R }$ , and all improper rotations are of the form $z \mapsto { \overline { { z } } } e ^ { i \varphi }$ for some $\varphi \in \mathbb { R }$ (here, ${ \overline { { z } } } = x - i y$ denotes the complex conjugate of z). See Exercise 1 for the argument leading to this result. 

Example 3. Euler gave the following very simple geometric description of rotations in $\mathbb { R } ^ { 3 }$ . Given a proper rotation $R ,$ there exists a unit vector γ so that: 

(i) R fixes $\gamma ,$ that is, $R ( \gamma ) = \gamma$ 

(ii) If $\mathcal { P }$ denotes the plane passing through the origin and perpendicular to $\gamma ,$ then $R : \mathcal P \to \mathcal P$ , and the restriction of R to $\mathcal { P }$ is a rotation in $\mathbb { R } ^ { 2 }$ 

Geometrically, the vector γ gives the direction of the axis of rotation. A proof of this fact is given in Exercise 2. Finally, if R is improper, then $- R$ is proper (since in $\mathbb { R } ^ { 3 } \operatorname* { d e t } ( - R ) = - \operatorname* { d e t } ( R ) )$ , so R is the composition of a proper rotation and a symmetry with respect to the origin. 

Example 4. Given two orthonormal bases $\{ e _ { 1 } , \ldots , e _ { d } \}$ and $\{ e _ { 1 } ^ { \prime } , \ldots , e _ { d } ^ { \prime } \}$ in $\mathbb { R } ^ { d }$ , we can define a rotation R by letting $R ( e _ { i } ) = e _ { i } ^ { \prime }$ for $i = 1 , \ldots , d .$ Conversely, if R is a rotation and $\{ e _ { 1 } , \ldots , e _ { d } \}$ is an orthonormal basis, then $\{ e _ { 1 } ^ { \prime } , \ldots , e _ { d } ^ { \prime } \}$ , where $e _ { j } ^ { \prime } = R ( e _ { j } )$ , is another orthonormal basis. 

## 1.2 Integration on $\mathbb { R } ^ { d }$

Since we shall be dealing with functions on $\mathbb { R } ^ { d }$ , we will need to discuss some aspects of integration of such functions. A more detailed review of integration on $\mathbb { R } ^ { d }$ is given in the appendix. 

A continuous complex-valued function $f$ on $\mathbb { R } ^ { d }$ is said to be rapidly decreasing if for every multi-index α the function $| x ^ { \alpha } f ( x ) |$ is bounded. Equivalently, a continuous function is of rapid decrease if 

$$
\sup _ {x \in \mathbb {R} ^ {d}} | x | ^ {k}   | f (x) | <   \infty \quad \text { for   every } k = 0, 1, 2, \ldots .
$$

Given a function of rapid decrease, we define 

$$
\int_ {\mathbb {R} ^ {d}} f (x) d x = \lim _ {N \to \infty} \int_ {Q _ {N}} f (x) d x,
$$

where $Q _ { N }$ denotes the closed cube centered at the origin, with sides of length N parallel to the coordinate axis, that is, 

$$
Q _ {N} = \{x \in \mathbb {R} ^ {d}: | x _ {i} | \leq N / 2 \quad \text { for } i = 1, \dots , d \}.
$$

The integral over $Q _ { N }$ is a multiple integral in the usual sense of Riemann integration. That the limit exists follows from the fact that the integrals $\begin{array} { r } { I _ { N } = \int _ { Q _ { N } } f ( x ) } \end{array}$ dx form a Cauchy sequence as $N$ tends to infinity. 

Two observations are in order. First, we may replace the square $Q _ { N }$ by the ball $B _ { N } = \{ { \boldsymbol x } \in  { \mathbb { R } } ^ { d } : | { \boldsymbol x } | \leq N \}$ without changing the definition. Second, we do not need the full force of rapid decrease to show that the limit exists. In fact it sufices to assume that $f$ is continuous and 

$$
\sup _ {x \in \mathbb {R} ^ {d}} | x | ^ {d + \epsilon} | f (x) | <   \infty \quad \text {   for   some   } \epsilon > 0.
$$

## 1. Preliminaries

For example, functions of moderate decrease on $\mathbb { R }$ correspond to $\epsilon = 1$ In keeping with this we define functions of moderate decrease on $\mathbb { R } ^ { d }$ as those that are continuous and satisfy the above inequality with $\epsilon = 1$ 

The interaction of integration with the three important groups of symmetries is as follows: if $f$ is of moderate decrease, then 

$$
\text {(i)} \int_ {\mathbb {R} ^ {d}} f (x + h) d x = \int_ {\mathbb {R} ^ {d}} f (x) d x \text {for all} h \in \mathbb {R} ^ {d},
$$

$$
\mathrm{(ii)} \delta^ {d} \int_ {\mathbb {R} ^ {d}} f (\delta x) d x = \int_ {\mathbb {R} ^ {d}} f (x) d x \mathrm{forall} \delta > 0,
$$

$$
\text {(iii)} \int_ {\mathbb {R} ^ {d}} f (R (x)) d x = \int_ {\mathbb {R} ^ {d}} f (x) d x \text {for every rotation} R.
$$

## Polar coordinates

It will be convenient to introduce polar coordinates in $\mathbb { R } ^ { d }$ and find the corresponding integration formula. We begin with two examples which correspond to the case $d = 2$ and $d = 3$ . (A more elaborate discussion applying to all d is contained in the appendix.) 

Example 1. In $\mathbb { R } ^ { 2 }$ , polar coordinates are given by $( r , \theta )$ with $r \geq 0$ and $0 \leq \theta < 2 \pi$ . The Jacobian of the change of variables is equal to r, so that 

$$
\int_ {\mathbb {R} ^ {2}} f (x) d x = \int_ {0} ^ {2 \pi} \int_ {0} ^ {\infty} f (r \cos \theta , r \sin \theta) r d r d \theta .
$$

Now we may write a point on the unit circle $S ^ { 1 }$ as $\gamma = ( \cos \theta , \sin \theta )$ , and given a function $g$ on the circle, we define its integral over $S ^ { 1 }$ by 

$$
\int_ {S ^ {1}} g (\gamma) d \sigma (\gamma) = \int_ {0} ^ {2 \pi} g (\cos \theta , \sin \theta) d \theta .
$$

With this notation we then have 

$$
\int_ {\mathbb {R} ^ {2}} f (x) d x = \int_ {S ^ {1}} \int_ {0} ^ {\infty} f (r \gamma) r d r d \sigma (\gamma).
$$

Example 2. In $\mathbb { R } ^ { 3 }$ one uses spherical coordinates given by 

$$
\left\{ \begin{array}{l l} x _ {1} & = r \sin \theta \cos \varphi , \\ x _ {2} & = r \sin \theta \sin \varphi , \\ x _ {3} & = r \cos \theta , \end{array} \right.
$$

where $0 < r , 0 \le \theta \le \pi$ and $0 \leq \varphi \leq 2 \pi$ . The Jacobian of the change of variables is $r ^ { 2 }$ sin θ so that 

$$
\begin{array}{l} {\int_ {\mathbb {R} ^ {3}} f (x) d x =} \\ {\int_ {0} ^ {2 \pi} \int_ {0} ^ {\pi} \int_ {0} ^ {\infty} f (r \sin \theta \cos \varphi , r \sin \theta \sin \varphi , r \cos \theta) r ^ {2} d r \sin \theta d \theta d \varphi .} \end{array}
$$

If $g$ is a function on the unit sphere $S ^ { 2 } = \{ x \in \mathbb { R } ^ { 3 } : | x | = 1 \}$ , and $\gamma =$ (sin θ cos $\varphi _ { ; }$ , sin $\theta$ sin $\varphi ,$ cos $\theta )$ , we define the surface element $d \sigma ( \gamma )$ by 

$$
\int_ {S ^ {2}} g (\gamma) d \sigma (\gamma) = \int_ {0} ^ {2 \pi} \int_ {0} ^ {\pi} g (\gamma) \sin \theta d \theta d \varphi .
$$

As a result, 

$$
\int_ {\mathbb {R} ^ {3}} f (x) d x = \int_ {S ^ {2}} \int_ {0} ^ {\infty} f (r \gamma) r ^ {2} d r d \sigma (\gamma).
$$

In general, it is possible to write any point in $\mathbb { R } ^ { d } - \{ 0 \}$ uniquely as 

$$
x = r \gamma
$$

where $\gamma$ lies on the unit sphere $S ^ { d - 1 } \subset \mathbb { R } ^ { d }$ and $r > 0$ . Indeed, take $r = | \boldsymbol { x } |$ and $\gamma = x / | x |$ . Thus one may proceed as in the cases $d = 2 { \mathrm { ~ o r ~ } } d = 3$ to define spherical coordinates. The formula we shall use is 

$$
\int_ {\mathbb {R} ^ {d}} f (x) d x = \int_ {S ^ {d - 1}} \int_ {0} ^ {\infty} f (r \gamma) r ^ {d - 1} d r d \sigma (\gamma),
$$

whenever $f$ is of moderate decrease. Here $d \sigma ( \gamma )$ denotes the surface element on the sphere $S ^ { d - 1 }$ obtained from the spherical coordinates. 

## 2 Elementary theory of the Fourier transform

The Schwartz space $S ( \mathbb { R } ^ { d } )$ (sometimes abbreviated as $s )$ consists of all indefinitely diferentiable functions $f$ on $\mathbb { R } ^ { d }$ such that 

$$
\sup _ {x \in \mathbb {R} ^ {d}} \left| x ^ {\alpha} \left(\frac {\partial}{\partial x}\right) ^ {\beta} f (x) \right| <   \infty ,
$$

for every multi-index $\alpha$ and $\beta .$ In other words, $f$ and all its derivatives are required to be rapidly decreasing. 

## 2. Elementary theory of the Fourier transform

Example 1. An example of a function in $S ( \mathbb { R } ^ { d } )$ is the d-dimensional Gaussian given by $e ^ { - \pi | { \dot { x } } | ^ { 2 } }$ . The theory in Chapter 5 already made clear the central role played by this function in the case $d = 1$ 

The Fourier transform of a Schwartz function f is defined by 

$$
\hat {f} (\xi) = \int_ {\mathbb {R} ^ {d}} f (x) e ^ {- 2 \pi i x \cdot \xi} d x, \quad \text { for } \xi \in \mathbb {R} ^ {d}.
$$

Note the resemblance with the formula in one-dimension, except that we are now integrating on $\mathbb { R } ^ { d }$ , and the product of x and $\xi$ is replaced by the inner product of the two vectors. 

We now list some simple properties of the Fourier transform. In the next proposition the arrow indicates that we have taken the Fourier transform, so $F ( x ) \longrightarrow G ( \xi )$ means that $G ( \xi ) = \hat { F } ( \xi )$ 

Proposition 2.1 Let $f \in { \mathcal { S } } ( \mathbb { R } ^ { d } )$ 

(i) $f ( x + h ) \longrightarrow { \hat { f } } ( \xi ) e ^ { 2 \pi i \xi \cdot h }$ whenever $h \in \mathbb { R } ^ { d }$ 

(ii) $f ( x ) e ^ { - 2 \pi i x h } \longrightarrow { \hat { f } } ( \xi + h )$ whenever $h \in \mathbb { R } ^ { d }$ 

(iii) $f ( \delta x ) \longrightarrow \delta ^ { - d } { \hat { f } } ( \delta ^ { - 1 } \xi )$ whenever $\delta > 0$ 

(iv) $\left( { \frac { \partial } { \partial x } } \right) ^ { \alpha } f ( x ) \longrightarrow ( 2 \pi i \xi ) ^ { \alpha } \hat { f } ( \xi ) .$ 

(v) $( - 2 \pi i x ) ^ { \alpha } f ( x ) \longrightarrow \left( \frac { \partial } { \partial \xi } \right) ^ { \alpha } \hat { f } ( \xi ) .$ 

(vi) $f ( R x ) \longrightarrow { \hat { f } } ( R \xi )$ whenever $R$ is a rotation. 

The first five properties are proved in the same way as in the onedimensional case. To verify the last property, simply change variables $y = R x$ in the integral. Then, recall that $| \operatorname* { d e t } ( R ) | = 1$ and $R ^ { - 1 } y \cdot \xi = y \cdot R \xi$ , because R is a rotation. 

Properties (iv) and (v) in the proposition show that, up to factors of 2πi, the Fourier transform interchanges diferentiation and multiplication by monomials. This motivates the definition of the Schwartz space and leads to the next corollary. 

## Corollary 2.2 The Fourier transform maps $S ( \mathbb { R } ^ { d } )$ to itself.

At this point we disgress to observe a simple fact concerning the interplay between the Fourier transform and rotations. We say that a function f is radial if it depends only on $| x | ;$ in other words, $f$ is radial if there is a function $f _ { 0 } ( u )$ , defined for $u \geq 0$ , such that $f ( x ) = f _ { 0 } ( | x | )$ We note that $f$ is radial if and only if $f ( R x ) = f ( x )$ for every rotation $R .$ In one direction, this is obvious since $| R x | = | x |$ . Converse $\mathrm { \Omega } \backslash \mathrm { y } ,$ , suppose that $f ( R x ) = f ( x )$ , for all rotations R. Now define $f _ { 0 }$ by 

$$
f _ {0} (u) = \left\{ \begin{array}{l l} f (0) & \text { if } u = 0, \\ f (x) & \text { if } | x | = u. \end{array} \right.
$$

Note that $f _ { 0 }$ is well defined, since if x and $x ^ { \prime }$ are points with $| x | = | x ^ { \prime } |$ there is always a rotation R so that $x ^ { \prime } = R x$ 

Corollary 2.3 The Fourier transform of a radial function is radial. 

This follows at once from property (vi) in the last proposition. Indeed, the condition $f ( R x ) = f ( x )$ for all R implies that ${ \hat { f } } ( R \xi ) = { \hat { f } } ( \xi )$ for all $R ,$ thus $\hat { f }$ is radial whenever $f$ is. 

An example of a radial function in $\mathbb { R } ^ { d }$ is the Gaussian $e ^ { - \pi | x | ^ { 2 } }$ . Also, we observe that when $d = 1$ , the radial functions are precisely the even functions, that is, those for which $f ( x ) = f ( - x )$ 

After these preliminaries, we retrace the steps taken in the previous chapter to obtain the Fourier inversion formula and Plancherel theorem for $\mathbb { R } ^ { d }$ 

Theorem 2.4 Suppose $f \in S ( \mathbb { R } ^ { d } )$ . Then 

$$
f (x) = \int_ {\mathbb {R} ^ {d}} \hat {f} (\xi) e ^ {2 \pi i x \cdot \xi} d \xi .
$$

Moreover 

$$
\int_ {\mathbb {R} ^ {d}} | \hat {f} (\xi) | ^ {2} d \xi = \int_ {\mathbb {R} ^ {d}} | f (x) | ^ {2} d x.
$$

The proof proceeds in the following stages. 

Step 1. The Fourier transform of $e ^ { - \pi | x | ^ { 2 } } { \mathrm { ~ i s ~ } } e ^ { - \pi | \xi | ^ { 2 } }$ . To prove this, notice that the properties of the exponential functions imply that 

$$
e ^ {- \pi | x | ^ {2}} = e ^ {- \pi x _ {1} ^ {2}} \dots e ^ {- \pi x _ {d} ^ {2}} \quad \text {and} \quad e ^ {- 2 \pi i x \cdot \xi} = e ^ {- 2 \pi i x _ {1} \cdot \xi_ {1}} \dots e ^ {- 2 \pi i x _ {d} \cdot \xi_ {d}},
$$

so that the integrand in the Fourier transform is a product of $d$ functions, each depending on the variable $x _ { j } \ ( 1 \leq j \leq d )$ only. Thus the assertion 

## 2. Elementary theory of the Fourier transform

follows by writing the integral over $\mathbb { R } ^ { d }$ as a series of repeated integrals, each taken over R. For example, when $d = 2$ 7 

$$
\begin{array}{r l} & {\int_ {\mathbb {R} ^ {2}} e ^ {- \pi | x | ^ {2}} e ^ {- 2 \pi i x \cdot \xi} d x = \int_ {\mathbb {R}} e ^ {- \pi x _ {2} ^ {2}} e ^ {- 2 \pi i x _ {2} \cdot \xi_ {2}} \left(\int_ {\mathbb {R}} e ^ {- \pi x _ {1} ^ {2}} e ^ {- 2 \pi i x _ {1} \cdot \xi_ {1}} d x _ {1}\right) d x _ {2}} \\ & {\qquad = \int_ {\mathbb {R}} e ^ {- \pi x _ {2} ^ {2}} e ^ {- 2 \pi i x _ {2} \cdot \xi_ {2}} e ^ {- \pi \xi_ {1} ^ {2}} d x _ {2}} \\ & {\qquad = e ^ {- \pi \xi_ {1} ^ {2}} e ^ {- \pi \xi_ {2} ^ {2}}} \\ & {\qquad = e ^ {- \pi | \xi | ^ {2}}.} \end{array}
$$

As a consequence of Proposition 2.1, applied with $\delta ^ { 1 / 2 }$ instead of $\delta ,$ we find that $\widehat { ( e ^ { - \pi \delta | x | ^ { 2 } } ) } = \delta ^ { - d / 2 } e ^ { - \pi | \xi | ^ { 2 } / \delta }$ 

Step 2. The family $K _ { \delta } ( x ) = \delta ^ { - d / 2 } e ^ { - \pi | x | ^ { 2 } / \delta }$ is a family of good kernels in $\mathbb { R } ^ { d }$ . By this we mean that 

$$
\text {(i)} \int_ {\mathbb {R} ^ {d}} K _ {\delta} (x) d x = 1,
$$

$$
\text {(ii)} \int_ {\mathbb {R} ^ {d}} | K _ {\delta} (x) | d x \leq M (\text {in fact} K _ {\delta} (x) \geq 0),
$$

(iii) For every $\eta > 0 , \int _ { | x | \geq \eta } | K _ { \delta } ( x ) | d x \to 0 { \mathrm { ~ a s ~ } } \delta \to 0 .$ 

The proofs of these assertions are almost identical to the case $d = 1$ . As a result 

$$
\int_ {\mathbb {R} ^ {d}} K _ {\delta} (x) F (x) d x \rightarrow F (0) \quad \text { as } \delta \rightarrow 0
$$

when $F$ is a Schwartz function, or more generally when $F$ is bounded and continuous at the origin. 

Step 3. The multiplication formula 

$$
\int_ {\mathbb {R} ^ {d}} f (x) \hat {g} (x) d x = \int_ {\mathbb {R} ^ {d}} \hat {f} (y) g (y) d y
$$

holds whenever $f$ and $g$ are in ${ \mathcal { S } } .$ The proof requires the evaluation of the integral of $f ( x ) g ( y ) e ^ { - 2 \pi i x \cdot y }$ over $( x , \overset { \cdot } { y } ) \in \mathbb { R } ^ { 2 d } = \mathbb { R } ^ { d } \times \mathbb { R } ^ { d }$ as a repeated integral, with each separate integration taken over $\mathbb { R } ^ { d }$ . The justification is similar to that in the proof of Proposition 1.8 in the previous chapter. (See the appendix.) 

The Fourier inversion is then a simple consequence of the multiplication formula and the family of good kernels $K _ { \delta }$ , as in Chapter 5. It also 

<!-- === Source: MinerU_markdown_Fourier_analysis_an_introduction_by_Elias_M._Stein,_Rami_Shakarchi_(z-lib.org)_201_2122707133446336527.md (Page 201) === -->

follows that the Fourier transform $\mathcal { F }$ is a bijective map of $S ( \mathbb { R } ^ { d } )$ to itself, whose inverse is 

$$
\mathcal {F} ^ {*} (g) (x) = \int_ {\mathbb {R} ^ {d}} g (\xi) e ^ {2 \pi i x \cdot \xi} d \xi .
$$

Step 4. Next we turn to the convolution, defined by 

$$
(f * g) (x) = \int_ {\mathbb {R} ^ {d}} f (y) g (x - y) d y, \quad f, g \in \mathcal {S}.
$$

We have that $f * g \in S ( \mathbb { R } ^ { d } ) , \ f * g = g * f$ , and $\widehat { ( f * g ) } ( \xi ) = \hat { f } ( \xi ) \hat { g } ( \xi )$ The argument is similar to that in one-dimension. The calculation of the Fourier transform of $f * g$ involves an integration of $f ( y ) g ( x - y ) e ^ { - 2 \pi i x \cdot \xi }$ (over $\mathbb { R } ^ { 2 d } = \mathbb { R } ^ { d } \times \mathbb { R } ^ { d } )$ expressed as a repeated integral. 

Then, following the same argument in the previous chapter, we obtain the d-dimensional Plancherel formula, thereby concluding the proof of Theorem 2.4. 

## 3 The wave equation in $\mathbb { R } ^ { d } \times \mathbb { R }$

Our next goal is to apply what we have learned about the Fourier transform to the study of the wave equation. Here, we once again simplify matters by restricting ourselves to functions in the Schwartz class S. We note that in any further analysis of the wave equation it is important to allow functions that have much more general behavior, and in particular that may be discontinuous. However, what we lose in generality by only considering Schwartz functions, we gain in transparency. Our study in this restricted context will allow us to explain certain basic ideas in their simplest form. 

## 3.1 Solution in terms of Fourier transforms

The motion of a vibrating string satisfies the equation 

$$
\frac {\partial^ {2} u}{\partial x ^ {2}} = \frac {1}{c ^ {2}} \frac {\partial^ {2} u}{\partial t ^ {2}},
$$

which we referred to as the one-dimensional wave equation. 

A natural generalization of this equation to d space variables is 

$$
\frac {\partial^ {2} u}{\partial x _ {1} ^ {2}} + \dots + \frac {\partial^ {2} u}{\partial x _ {d} ^ {2}} = \frac {1}{c ^ {2}} \frac {\partial^ {2} u}{\partial t ^ {2}}.\tag{1}
$$

In fact, it is known that in the case $d = 3 ,$ this equation determines the behavior of electromagnetic waves in vacuum (with c = speed of light). 

## 3. The wave equation in $\mathbb { R } ^ { d } \times \mathbb { R }$

Also, this equation describes the propagation of sound waves. Thus (1) is called the d-dimensional wave equation. 

Our first observation is that we may assume $c = 1$ , since we can rescale the variable t if necessary. Also, if we define the Laplacian in d dimensions by 

$$
\triangle = \frac {\partial^ {2}}{\partial x _ {1} ^ {2}} + \dots + \frac {\partial^ {2}}{\partial x _ {d} ^ {2}},
$$

then the wave equation can be rewritten as 

$$
\triangle u = \frac {\partial^ {2} u}{\partial t ^ {2}}.\tag{2}
$$

The goal of this section is to find a solution to this equation, subject to the initial conditions 

$$
u (x, 0) = f (x) \quad \text { and } \quad \frac {\partial u}{\partial t} (x, 0) = g (x),
$$

where $f , g \in { \mathcal { S } } ( \mathbb { R } ^ { d } )$ . This is called the Cauchy problem for the wave equation. 

Before solving this problem, we note that while we think of the variable t as time, we do not restrict ourselves to $t > 0$ . As we will see, the solution we obtain makes sense for all $t \in \mathbb { R }$ . This is a manifestation of the fact that the wave equation can be reversed in time (unlike the heat equation). 

A formula for the solution of our problem is given in the next theorem. The heuristic argument which leads to this formula is important since, as we have already seen, it applies to some other boundary value problems as well. 

Suppose u solves the Cauchy problem for the wave equation. The technique employed consists of taking the Fourier transform of the equation and of the initial conditions, with respect to the space variables $x _ { 1 } , \ldots , x _ { d }$ . This reduces the problem to an ordinary diferential equation in the time variable. Indeed, recalling that diferentiation with respect to $x _ { j }$ becomes multiplication by $2 \pi i \xi _ { j }$ , and the diferentiation with respect to t commutes with the Fourier transform in the space variables, we find that (2) becomes 

$$
- 4 \pi^ {2} | \xi | ^ {2} \hat {u} (\xi , t) = \frac {\partial^ {2} \hat {u}}{\partial t ^ {2}} (\xi , t).
$$

For each fixed $\xi \in \mathbb { R } ^ { d }$ , this is an ordinary diferential equation in t whose solution is given by 

$$
\hat {u} (\xi , t) = A (\xi) \cos (2 \pi | \xi | t) + B (\xi) \sin (2 \pi | \xi | t),
$$

where for each $\xi , A ( \xi )$ and $B ( \xi )$ are unknown constants to be determined by the initial conditions. In fact, taking the Fourier transform (in x) of the initial conditions yields 

$$
\hat {u} (\xi , 0) = \hat {f} (\xi) \quad \text { and } \quad \frac {\partial \hat {u}}{\partial t} (\xi , 0) = \hat {g} (\xi).
$$

We may now solve for $A ( \xi )$ and $B ( \xi )$ to obtain 

$$
A (\xi) = \hat {f} (\xi) \quad \mathrm{and} \quad 2 \pi | \xi | B (\xi) = \hat {g} (\xi).
$$

Therefore, we find that 

$$
\hat {u} (\xi , t) = \hat {f} (\xi) \cos (2 \pi | \xi | t) + \hat {g} (\xi) \frac {\sin (2 \pi | \xi | t)}{2 \pi | \xi |},
$$

and the solution u is given by taking the inverse Fourier transform in the $\xi$ variables. This formal derivation then leads to a precise existence theorem for our problem. 

Theorem 3.1 A solution of the Cauchy problem for the wave equation is 

$$
u (x, t) = \int_ {\mathbb {R} ^ {d}} \left[ \hat {f} (\xi) \cos (2 \pi | \xi | t) + \hat {g} (\xi) \frac {\sin (2 \pi | \xi | t)}{2 \pi | \xi |} \right] e ^ {2 \pi i x \cdot \xi} d \xi .\tag{3}
$$

Proof. We first verify that u solves the wave equation. This is straightforward once we note that we can diferentiate in x and t under the integral sign (because $f$ and $g$ are both Schwartz functions) and therefore u is at least $C ^ { 2 }$ . On the one hand we diferentiate the exponential with respect to the x variables to get 

$$
\triangle u (x, t) = \int_ {\mathbb {R} ^ {d}} \left[ \hat {f} (\xi) \cos (2 \pi | \xi | t) + \hat {g} (\xi) \frac {\sin (2 \pi | \xi | t)}{2 \pi | \xi |} \right] (- 4 \pi^ {2} | \xi | ^ {2}) e ^ {2 \pi i x \cdot \xi} d \xi ,
$$

while on the other hand we diferentiate the terms in brackets with respect to t twice to get 

$$
\frac {\partial^ {2} u}{\partial t ^ {2}} (x, t) =
$$

$$
\int_ {\mathbb {R} ^ {d}} \left[ - 4 \pi^ {2} | \xi | ^ {2} \hat {f} (\xi) \cos (2 \pi | \xi | t) - 4 \pi^ {2} | \xi | ^ {2} \hat {g} (\xi) \frac {\sin (2 \pi | \xi | t)}{2 \pi | \xi |} \right] e ^ {2 \pi i x \cdot \xi} d \xi .
$$

This shows that u solves equation (2). Setting $t = 0$ we get 

$$
u (x, 0) = \int_ {\mathbb {R} ^ {d}} \hat {f} (\xi) e ^ {2 \pi i x \cdot \xi} d \xi = f (x)
$$

## 3. The wave equation in $\mathbb { R } ^ { d } \times \mathbb { R }$

by the Fourier inversion theorem. Finally, diferentiating once with respect to $t ,$ setting $t = 0$ , and using the Fourier inversion shows that 

$$
\frac {\partial u}{\partial t} (x, 0) = g (x).
$$

Thus u also verifies the initial conditions, and the proof of the theorem is complete. 

As the reader will note, both ${ \hat { f } } ( \xi ) \cos ( 2 \pi | \xi | t )$ and ${ \hat { g } } ( \xi ) { \frac { \sin ( 2 \pi | \xi | t ) } { 2 \pi | \xi | } }$ are functions in $s ,$ assuming as we do that $f$ and g are in ${ \mathcal { S } } .$ . This is because both cos u and $( \sin u ) / u$ are even functions that are indefinitely diferentiable. 

Having proved the existence of a solution to the Cauchy problem for the wave equation, we raise the question of uniqueness. Are there solutions to the problem 

$$
\triangle u = \frac {\partial^ {2} u}{\partial t ^ {2}} \quad \text { subject   to } \quad u (x, 0) = f (x) \quad \text { and } \quad \frac {\partial u}{\partial t} (x, 0) = g (x),
$$

other than the one given by the formula in the theorem? In fact the answer is, as expected, no. The proof of this fact, which will not be given here (but see Problem 3), can be based on a conservation of energy argument. This is a local counterpart of a global conservation of energy statement which we will now present. 

We observed in Exercise 10, Chapter 3, that in the one-dimensional case, the total energy of the vibrating string is conserved in time. The analogue of this fact holds in higher dimensions as well. Define the energy of a solution by 

$$
E (t) = \int_ {\mathbb {R} ^ {d}} \left| \frac {\partial u}{\partial t} \right| ^ {2} + \left| \frac {\partial u}{\partial x _ {1}} \right| ^ {2} + \dots + \left| \frac {\partial u}{\partial x _ {d}} \right| ^ {2} d x.
$$

Theorem 3.2 If u is the solution of the wave equation given by formula (3), then $E ( t )$ is conserved, that is, 

$$
E (t) = E (0), \quad f o r a l l t \in \mathbb {R}.
$$

The proof requires the following lemma. 

Lemma 3.3 Suppose a and b are complex numbers and α is real. Then 

$$
\left| a \cos \alpha + b \sin \alpha \right| ^ {2} + \left| - a \sin \alpha + b \cos \alpha \right| ^ {2} = \left| a \right| ^ {2} + \left| b \right| ^ {2}.
$$

This follows directly because $e _ { 1 } = ( \cos \alpha , \sin \alpha )$ and $e _ { 2 } = ( - \sin \alpha , \cos \alpha )$ are a pair of orthonormal vectors, hence with $Z = ( a , b ) \in \mathbb { C } ^ { 2 }$ , we have 

$$
| Z | ^ {2} = | Z \cdot e _ {1} | ^ {2} + | Z \cdot e _ {2} | ^ {2},
$$

where · represents the inner product in $\mathbb { C } ^ { 2 }$ 

Now by Plancherel’s theorem, 

$$
\int_ {\mathbb {R} ^ {d}} \left| \frac {\partial u}{\partial t} \right| ^ {2} d x = \int_ {\mathbb {R} ^ {d}} \left| - 2 \pi | \xi | \hat {f} (\xi) \sin (2 \pi | \xi | t) + \hat {g} (\xi) \cos (2 \pi | \xi | t) \right| ^ {2} d \xi .
$$

Similarly, 

$$
\int_ {\mathbb {R} ^ {d}} \sum_ {j = 1} ^ {d} \left| \frac {\partial u}{\partial x _ {j}} \right| ^ {2} d x = \int_ {\mathbb {R} ^ {d}} \left| 2 \pi | \xi | \hat {f} (\xi) \cos (2 \pi | \xi | t) + \hat {g} (\xi) \sin (2 \pi | \xi | t) \right| ^ {2} d \xi .
$$

We now apply the lemma with 

$$
a = 2 \pi | \xi | \hat {f} (\xi), \quad b = \hat {g} (\xi) \quad \mathrm{and} \quad \alpha = 2 \pi | \xi | t.
$$

The result is that 

$$
\begin{array}{c} E (t) = \int_ {\mathbb {R} ^ {d}} \left| \frac {\partial u}{\partial t} \right| ^ {2} + \left| \frac {\partial u}{\partial x _ {1}} \right| ^ {2} + \dots + \left| \frac {\partial u}{\partial x _ {d}} \right| ^ {2} d x \\ = \int_ {\mathbb {R} ^ {d}} (4 \pi^ {2} | \xi | ^ {2} | \hat {f} (\xi) | ^ {2} + | \hat {g} (\xi) | ^ {2}) d \xi , \end{array}
$$

which is clearly independent of t. Thus Theorem 3.2 is proved. 

The drawback with formula (3), which does give the solution of the wave equation, is that it is quite indirect, involving the calculation of the Fourier transforms of $f$ and $^ { g , }$ and then a further inverse Fourier transform. However, for every dimension d there is a more explicit formula. This formula is very simple when $d = 1$ and a little less so when $d = 3$ More generally, the formula is “elementary” whenever d is odd, and more complicated when d is even (see Problems 4 and 5). 

In what follows we consider the cases $d = 1 , d = 3$ , and $d = 2 .$ , which together give a picture of the general situation. Recall that in Chapter 1, when discussing the wave equation over the interval $[ 0 , L ]$ , we found that the solution is given by d’Alembert’s formula 

$$
u (x, t) = \frac {f (x + t) + f (x - t)}{2} + \frac {1}{2} \int_ {x - t} ^ {x + t} g (y) d y.\tag{4}
$$

## 3. The wave equation in $\mathbb { R } ^ { d } \times \mathbb { R }$

with the interpretation that both $f$ and $g$ are extended outside $[ 0 , L ]$ by making them odd in $[ - L , L ]$ , and periodic on the real line, with period $2 L$ . The same formula (4) holds for the solution of the wave equation when $d = 1$ and when the initial data are functions in $S ( \mathbb { R } )$ . In fact, this follows directly from (3) if we note that 

$$
\cos (2 \pi | \xi | t) = \frac {1}{2} (e ^ {2 \pi i | \xi | t} + e ^ {- 2 \pi i | \xi | t})
$$

and 

$$
\frac {\sin (2 \pi | \xi | t)}{2 \pi | \xi |} = \frac {1}{4 \pi i | \xi |} (e ^ {2 \pi i | \xi | t} - e ^ {- 2 \pi i | \xi | t}).
$$

Finally, we note that the two terms that appear in d’Alembert’s formula (4) consist of appropriate averages. Indeed, the first term is precisely the average of $f$ over the two points that are the boundary of the interval $[ x - t , x + t ] ;$ the second term is, up to a factor of $t ,$ the mean value of $g$ over this interval, that is, $\begin{array} { r } { ( 1 / 2 t ) \int _ { x - t } ^ { x + t } g ( y ) d y } \end{array}$ . This suggests a generalization to higher dimensions, where we might expect to write the solution of our problem as averages of the initial data. This is in fact the case, and we now treat in detail the particular situation $d = 3$ 

## 3.2 The wave equation in $\mathbb { R } ^ { 3 } \times \mathbb { R }$

If $S ^ { 2 }$ denotes the unit sphere in $\mathbb { R } ^ { 3 }$ , we define the spherical mean of the function $f$ over the sphere of radius t centered at x by 

$$
M _ {t} (f) (x) = \frac {1}{4 \pi} \int_ {S ^ {2}} f (x - t \gamma) d \sigma (\gamma),\tag{5}
$$

where $d \sigma ( \gamma )$ is the element of surface area for $S ^ { 2 }$ . Since 4π is the area of the unit sphere, we can interpret $M _ { t } ( f )$ as the average value of $f$ over the sphere centered at x of radius t. 

Lemma 3.4 $I f f \in S ( \mathbb { R } ^ { 3 } )$ and t is fixed, then $M _ { t } ( f ) \in S ( \mathbb { R } ^ { 3 } )$ . Moreover, $M _ { t } ( f )$ is indefinitely diferentiable in $t ,$ and each t-derivative also belongs to $S ( \mathbb { R } ^ { 3 } )$ . 

Proof. Let $F ( x ) = M _ { t } ( f ) ( x )$ . To show that $F$ is rapidly decreasing, start with the inequality $| f ( x ) | \le A _ { N } / ( 1 + | x | ^ { N } )$ which holds for every fixed $N \geq 0$ . As a simple consequence, whenever t is fixed, we have 

$$
| f (x - \gamma t) | \leq A _ {N} ^ {\prime} / (1 + | x | ^ {N}) \quad \text { for   all } \gamma \in S ^ {2}.
$$

To see this consider separately the cases when $| x | \leq 2 | t |$ , and $| x | > 2 | t |$ Therefore, by integration 

$$
| F (x) | \leq A _ {N} ^ {\prime} / (1 + | x | ^ {N}),
$$

and since this holds for every $N$ , the function $F$ is rapidly decreasing. One next observes that F is indefinitely diferentiable, and 

$$
\left(\frac {\partial}{\partial x}\right) ^ {\alpha} F (x) = M _ {t} \left(f ^ {(\alpha)}\right) (x)\tag{6}
$$

where $f ^ { ( \alpha ) } ( x ) = ( \partial / \partial x ) ^ { \alpha } f ,$ . It sufices to prove this when $( \partial / \partial x ) ^ { \alpha } =$ $\partial / \partial x _ { k } .$ and then proceed by induction to get the general case. Furthermore, it is enough to take $k = 1$ . Now 

$$
\frac {F (x _ {1} + h , x _ {2} , x _ {3}) - F (x _ {1} , x _ {2} , x _ {3})}{h} = \frac {1}{4 \pi} \int_ {S ^ {2}} g _ {h} (\gamma) d \sigma (\gamma)
$$

where 

$$
g _ {h} (\gamma) = \frac {f (x + e _ {1} h - \gamma t) - f (x - \gamma t)}{h},
$$

and $e _ { 1 } = ( 1 , 0 , 0 )$ . Now, it sufices to observe that $\begin{array} { r } { g _ { h } \longrightarrow \frac { \partial } { \partial x _ { 1 } } f ( x - \gamma t ) } \end{array}$ as $h \to 0$ uniformly in $\gamma .$ . As a result, we find that (6) holds, and by the first argument, it follows that $\begin{array} { r } { \left( \frac { \partial } { \partial x } \right) ^ { \dot { \alpha } } F ( x ) } \end{array}$ is also rapidly decreasing, hence $F \in S$ . The same argument applies to each t-derivative of $M _ { t } ( f )$ 

The basic fact about integration on spheres that we shall need is the following Fourier transform formula. 

$$
\text { Lemma   3.5 } \frac {1}{4 \pi} \int_ {S ^ {2}} e ^ {- 2 \pi i \xi \cdot \gamma} d \sigma (\gamma) = \frac {\sin (2 \pi | \xi |)}{2 \pi | \xi |}.
$$

This formula, as we shall see in the following section, is connected to the fact that the Fourier transform of a radial function is radial. 

Proof. Note that the integral on the left is radial in $\xi .$ . Indeed, if R is a rotation then 

$$
\int_ {S ^ {2}} e ^ {- 2 \pi i R (\xi) \cdot \gamma} d \sigma (\gamma) = \int_ {S ^ {2}} e ^ {- 2 \pi i \xi \cdot R ^ {- 1} (\gamma)} d \sigma (\gamma) = \int_ {S ^ {2}} e ^ {- 2 \pi i \xi \cdot \gamma} d \sigma (\gamma)
$$

because we may change variables $\gamma \to R ^ { - 1 } ( \gamma )$ . (For this, see formula (4) in the appendix.) So ${ \mathrm { i f ~ } } | \xi | = \rho .$ it sufices to prove the lemma with 

## 3. The wave equation in $\mathbb { R } ^ { d } \times \mathbb { R }$

$\xi = ( 0 , 0 , \rho )$ . If $\rho = 0$ , the lemma is obvious. If $\rho > 0$ , we choose spherical coordinates to find that the left-hand side is equal to 

$$
\frac {1}{4 \pi} \int_ {0} ^ {2 \pi} \int_ {0} ^ {\pi} e ^ {- 2 \pi i \rho \cos \theta} \sin \theta d \theta d \varphi .
$$

The change of variables $u = - \cos \theta$ gives 

$$
\begin{array}{r l} & {\frac {1}{4 \pi} \int_ {0} ^ {2 \pi} \int_ {0} ^ {\pi} e ^ {- 2 \pi i \rho \cos \theta} \sin \theta d \theta d \varphi = \frac {1}{2} \int_ {0} ^ {\pi} e ^ {- 2 \pi i \rho \cos \theta} \sin \theta d \theta} \\ & {\qquad = \frac {1}{2} \int_ {- 1} ^ {1} e ^ {2 \pi i \rho u} d u} \\ & {\qquad = \frac {1}{4 \pi i \rho} \left[ e ^ {2 \pi i \rho u} \right] _ {- 1} ^ {1}} \\ & {\qquad = \frac {\sin (2 \pi \rho)}{2 \pi \rho},} \end{array}
$$

and the formula is proved. 

By the defining formula (5) we may interpret $M _ { t } ( f )$ as a convolution of the function f with the element $d { \boldsymbol { \sigma } } .$ and since the Fourier transform interchanges convolutions with products, we are led to believe that $\widehat { M _ { t } ( f ) }$ is the product of the corresponding Fourier transforms. Indeed, we have the identity 

(7) 

$$
\widehat {M _ {t} (f)} (\xi) = \hat {f} (\xi) \frac {\sin (2 \pi | \xi | t)}{2 \pi | \xi | t}.
$$

To see this, write 

$$
\widehat {M _ {t} (f)} (\xi) = \int_ {\mathbb {R} ^ {3}} e ^ {- 2 \pi i x \cdot \xi} \left(\frac {1}{4 \pi} \int_ {S ^ {2}} f (x - \gamma t) d \sigma (\gamma)\right) d x,
$$

and note that we may interchange the order of integration and make a simple change of variables to achieve the desired identity. 

As a result, we find that the solution of our problem may be expressed by using the spherical means of the initial data. 

Theorem 3.6 The solution when $d = 3$ of the Cauchy problem for the wave equation 

$$
\triangle u = \frac {\partial^ {2} u}{\partial t ^ {2}} \quad s u b j e c t t o \quad u (x, 0) = f (x) \quad a n d \quad \frac {\partial u}{\partial t} (x, 0) = g (x)
$$

is given $b y$ 

$$
u (x, t) = \frac {\partial}{\partial t} (t M _ {t} (f) (x)) + t M _ {t} (g) (x).
$$

Proof. Consider first the problem 

$$
\triangle u = \frac {\partial^ {2} u}{\partial t ^ {2}} \quad \text { subject   to } \quad u (x, 0) = 0 \quad \text { and } \quad \frac {\partial u}{\partial t} (x, 0) = g (x).
$$

Then by Theorem 3.1, we know that its solution $u _ { 1 }$ is given by 

$$
\begin{array}{r l} & u _ {1} (x, t) = \int_ {\mathbb {R} ^ {3}} \left[ \hat {g} (\xi) \frac {\sin (2 \pi | \xi | t)}{2 \pi | \xi |} \right] e ^ {2 \pi i x \cdot \xi} d \xi \\ & \qquad = t \int_ {\mathbb {R} ^ {3}} \left[ \hat {g} (\xi) \frac {\sin (2 \pi | \xi | t)}{2 \pi | \xi | t} \right] e ^ {2 \pi i x \cdot \xi} d \xi \\ & \qquad = t M _ {t} (g) (x), \end{array}
$$

where we have used (7) applied to $^ { g , }$ and the Fourier inversion formula. 

According to Theorem 3.1 again, the solution to the problem 

$$
\triangle u = \frac {\partial^ {2} u}{\partial t ^ {2}} \quad \text { subject   to } \quad u (x, 0) = f (x) \quad \text { and } \quad \frac {\partial u}{\partial t} (x, 0) = 0
$$

is given by 

$$
\begin{array}{r l} & u _ {2} (x, t) = \int_ {\mathbb {R} ^ {3}} \left[ \hat {f} (\xi) \cos (2 \pi | \xi | t) \right] e ^ {2 \pi i x \cdot \xi} d \xi \\ & \qquad = \frac {\partial}{\partial t} \left(t \int_ {\mathbb {R} ^ {3}} \left[ \hat {f} (\xi) \frac {\sin (2 \pi | \xi | t)}{2 \pi | \xi | t} \right] e ^ {2 \pi i x \cdot \xi} d \xi\right) \\ & \qquad = \frac {\partial}{\partial t} (t M _ {t} (f) (x)). \end{array}
$$

We may now superpose these two solutions to obtain $u = u _ { 1 } + u _ { 2 }$ as the solution of our original problem. 

## Huygens principle

The solutions to the wave equation in one and three dimensions are given, respectively, by 

$$
u (x, t) = \frac {f (x + t) + f (x - t)}{2} + \frac {1}{2} \int_ {x - t} ^ {x + t} g (y) d y
$$

and 

$$
u (x, t) = \frac {\partial}{\partial t} (t M _ {t} (f) (x)) + t M _ {t} (g) (x).
$$

3. The wave equation in $\mathbb { R } ^ { d }$ × R 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2ab5d4b2-da28-455b-b554-908156ef0c8e/54324abecd3190667ce08f73d91ddebab057d2b009538dd7c017f1cf7350a8c3.jpg)



Figure 1. Huygens principle, $d = 1$


We observe that in the one-dimensional problem, the value of the solution at $( x , t )$ depends only on the values of $f$ and $g$ in the interval centered at x of length ${ 2 t } ,$ as shown in Figure 1. 

If in addition $g = 0 .$ , then the solution depends only on the data at the two boundary points of this interval. In three dimensions, this boundary dependence always holds. More precisely, the solution $u ( x , t )$ depends only on the values of $f$ and $g$ in an immediate neighborhood of the sphere centered at x and of radius t. This situation is depicted in Figure 2, where we have drawn the cone originating at $( x , t )$ and with its base the ball centered at x of radius t. This cone is called the backward light cone originating at $( x , t )$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2ab5d4b2-da28-455b-b554-908156ef0c8e/73dba63682540f1eb03c6c78720365e787f2c8d545760ce9b6be305e70cb4f5f.jpg)



Figure 2. Backward light cone originating at $( x , t )$


Alternatively, the data at a point $x _ { 0 }$ in the plane $t = 0$ influences the solution only on the boundary of a cone originating at $x _ { 0 }$ , called the forward light cone and depicted in Figure 3. 

This phenomenon, known as the Huygens principle, is immediate from the formulas for u given above. 

Another important aspect of the wave equation connected with these 

Chapter 6. THE FOURIER TRANSFORM ON $\mathbb { R } ^ { d }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2ab5d4b2-da28-455b-b554-908156ef0c8e/55ce14e60f9993e520d8e7decbfe482b21fe4ceaf3562ea9fa64b45cb9b9b48d.jpg)



Figure 3. The forward light cone originating at $x _ { 0 }$


considerations is that of the finite speed of propagation. (In the case where $c = 1$ , the speed is 1.) This means that if we have an initial disturbance localized at $x = x _ { 0 }$ , then after a finite time $t ,$ its efects will have propagated only inside the ball centered at $x _ { 0 }$ of radius |t|. To state this precisely, suppose the initial conditions $f$ and $g$ are supported in the ball of radius $\delta ,$ centered at $x _ { 0 }$ (think of $\delta$ as small). Then $u ( x , t )$ is supported in the ball of radius $| t | + \delta$ centered at $x _ { 0 }$ . This assertion is clear from the above discussion. 

## 3.3 The wave equation in $\mathbb { R } ^ { 2 } \times \mathbb { R }$ : descent

It is a remarkable fact that the solution of the wave equation in three dimensions leads to a solution of the wave equation in two dimensions. Define the corresponding means by 

$$
\widetilde {M} _ {t} (F) (x) = \frac {1}{2 \pi} \int_ {| y | \leq 1} F (x - t y) (1 - | y | ^ {2}) ^ {- 1 / 2} d y.
$$

Theorem 3.7 A solution of the Cauchy problem for the wave equation in two dimensions with initial data $f , g \in { \mathcal { S } } ( \mathbb { R } ^ { 2 } )$ is given by 

$$
u (x, t) = \frac {\partial}{\partial t} (t \widetilde {M _ {t}} (f) (x)) + t \widetilde {M _ {t}} (g) (x).\tag{8}
$$

Notice the diference between this case and the case $d = 3$ . Here, u at $( x , t )$ depends on $f$ and $g$ in the whole disc (of radius |t| centered at $x )$ and not just on the values of the initial data near the boundary of that disc. 

Formally, the identity in the theorem arises as follows. If we start with an initial pair of functions $f$ and $g$ in $S ( \mathbb { R } ^ { 2 } )$ , we may consider the corresponding functions $\tilde { f }$ and $\tilde { g }$ on $\mathbb { R } ^ { 3 }$ that are merely extensions of $f$ and $g$ that are constant in the $x _ { 3 }$ variable, that is, 

$$
\tilde {f} (x _ {1}, x _ {2}, x _ {3}) = f (x _ {1}, x _ {2}) \quad \text { and } \quad \tilde {g} (x _ {1}, x _ {2}, x _ {3}) = g (x _ {1}, x _ {2}).
$$

## 3. The wave equation in $\mathbb { R } ^ { d } \times \mathbb { R }$

Now, if ˜u is the solution (given in the previous section) of the 3-dimensional wave equation with initial data $\tilde { f }$ and ${ \tilde { g } } ,$ then one can expect that ˜u is also constant in $x _ { 3 }$ so that ˜u satisfies the 2-dimensional wave equation. A dificulty with this argument is that $\tilde { f }$ and $\tilde { g }$ are not rapidly decreasing since they are constant in $x _ { 3 } .$ so that our previous methods do not apply. However, it is easy to modify the argument so as to obtain a proof of Theorem 3.7. 

We fix $T > 0$ and consider a function $\eta ( x _ { 3 } )$ that is in $S ( \mathbb { R } )$ , such that $\eta ( x _ { 3 } ) = 1 \mathrm { i f } | x _ { 3 } | \le 3 T$ . The trick is to truncate $\tilde { f }$ and $\tilde { g }$ in the $x _ { 3 } .$ -variable, and consider instead 

$$
\tilde {f} ^ {\flat} (x _ {1}, x _ {2}, x _ {3}) = f (x _ {1}, x _ {2}) \eta (x _ {3}) \quad \text { and } \quad \tilde {g} ^ {\flat} (x _ {1}, x _ {2}, x _ {3}) = g (x _ {1}, x _ {2}) \eta (x _ {3}).
$$

Now both $\tilde { f } ^ { \flat }$ and $\tilde { g } ^ { \flat }$ are in $S ( \mathbb { R } ^ { 3 } )$ , so Theorem 3.6 provides a solution $\tilde { u } ^ { \flat }$ of the wave equation with initial data $\tilde { f } ^ { \flat }$ and $\tilde { g } ^ { \flat }$ . It is easy to see from the formula that $\tilde { u } ^ { \flat } ( x , t )$ is independent of $x _ { 3 }$ , whenever $| x _ { 3 } | \le T$ and $| t | \leq T$ . In particular, if we define $u ( x _ { 1 } , x _ { 2 } , t ) = \tilde { u } ^ { \flat } ( x _ { 1 } , x _ { 2 } , 0 , t )$ , then u satisfies the 2-dimensional wave equation when $| t | \leq T$ . Since $T$ is arbitrary, u is a solution to our problem, and it remains to see why u has the desired form. 

By definition of the spherical coordinates, we recall that the integral of a function H over the sphere $S ^ { 2 }$ is given by 

$$
\begin{array}{c} \frac {1}{4 \pi} \int_ {S ^ {2}} H (\gamma) d \sigma (\gamma) = \\ \frac {1}{4 \pi} \int_ {0} ^ {2 \pi} \int_ {0} ^ {\pi} H (\sin \theta \cos \varphi , \sin \theta \sin \varphi , \cos \theta) \sin \theta d \theta d \varphi . \end{array}
$$

If H does not depend on the last variable, that is, $H ( x _ { 1 } , x _ { 2 } , x _ { 3 } ) = h ( x _ { 1 } , x _ { 2 } )$ for some function h of two variables, then 

$$
\begin{array}{l} M _ {t} (H) (x _ {1}, x _ {2}, 0) = \\ \frac {1}{4 \pi} \int_ {0} ^ {2 \pi} \int_ {0} ^ {\pi} h (x _ {1} - t \sin \theta \cos \varphi , x _ {2} - t \sin \theta \sin \varphi) \sin \theta d \theta d \varphi . \end{array}
$$

To calculate this last integral, we split the θ-integral from 0 to $\pi / 2$ and then $\pi / 2$ to $\pi .$ . By making the change of variables $r = \sin \theta$ , we find, after a final change to polar coordinates, that 

$$
\begin{array}{c} M _ {t} (H) (x _ {1}, x _ {2}, 0) = \frac {1}{2 \pi} \int_ {| y | \leq 1} h (x - t y) (1 - | y | ^ {2}) ^ {- 1 / 2}   d y \\ = \widetilde {M} _ {t} (h) (x _ {1}, x _ {2}). \end{array}
$$

Applying this to $H = \tilde { f } ^ { \flat } , h = f .$ , and $H = \tilde { g } ^ { \flat } , h = g ,$ we find that u is given by the formula (8), and the proof of Theorem 3.7 is complete. 

Remark. In the case of general $d ,$ the solution of the wave equation shares many of the properties we have discussed in the special cases $d = 1 , 2 $ , and 3. 

• At a given time t, the initial data at a point x only afects the solution u in a specific region. When $d > 1$ is odd, the data influences only the points on the boundary of the forward light cone originating at $x ,$ while when $d = 1$ or d is even, it afects all points of the forward light cone. Alternatively, the solution at a point $( x , t )$ depends only on the data at the base of the backward light cone originating at $( x , t )$ . In fact, when $d > 1$ is odd, only the data in an immediate neighborhood of the boundary of the base will influence $u ( x , t )$ 

• Waves propagate with finite speed: if the initial data is supported in a bounded set, then the support of the solution u spreads with velocity 1 (or more generally c, if the wave equation is not normalized). 

We can illustrate some of these facts by the following observation about the diferent behavior of the propagation of waves in three and two dimensions. Since the propagation of light is governed by the three-dimensional wave equation, if at $t = 0$ a light flashes at the origin, the following happens: any observer will see the flash (after a finite amount of time) only for an instant. In contrast, consider what happens in two dimensions. If we drop a stone in a lake, any point on the surface will begin (after some time) to undulate; although the amplitude of the oscillations will decrease over time, the undulations will continue (in principle) indefinitely. 

The diference in character of the formulas for the solutions of the wave equation when $d = 1$ and $d = 3$ on the one hand, and $d = 2$ on the other hand, illustrates a general principle in d-dimensional Fourier analysis: a significant number of formulas that arise are simpler in the case of odd dimensions, compared to the corresponding situations in even dimensions. We will see several further examples of this below. 

## 4 Radial symmetry and Bessel functions

We observed earlier that the Fourier transform of a radial function in $\mathbb { R } ^ { d }$ is also radial. In other words, if $f ( x ) = f _ { 0 } ( | x | )$ for some $f _ { 0 }$ , then ${ \hat { f } } ( \xi ) = F _ { 0 } ( | \xi | )$ for some $F _ { 0 }$ . A natural problem is to determine a relation between $f _ { 0 }$ and $F _ { 0 }$ . 

This problem has a simple answer in dimensions one and three. If $d = 1$ the relation we seek is 

$$
F _ {0} (\rho) = 2 \int_ {0} ^ {\infty} \cos (2 \pi \rho r) f _ {0} (r) d r.\tag{9}
$$

If we recall that R has only two rotations, the identity and multiplication by −1, we find that a function is radial precisely when it is even. Having made this observation it is easy to see that if $f$ is radial, and $| \xi | = \rho ,$ then 

$$
\begin{array}{l} F _ {0} (\rho) = \hat {f} (| \xi |) = \int_ {- \infty} ^ {\infty} f (x) e ^ {- 2 \pi i x | \xi |} d x \\ \qquad = \int_ {0} ^ {\infty} f _ {0} (r) (e ^ {- 2 \pi i r | \xi |} + e ^ {2 \pi i r | \xi |}) d r \\ \qquad = 2 \int_ {0} ^ {\infty} \cos (2 \pi \rho r) f _ {0} (r) d r. \end{array}
$$

In the case $d = 3 .$ the relation between $f _ { 0 }$ and $F _ { 0 }$ is also quite simple and given by the formula 

$$
F _ {0} (\rho) = 2 \rho^ {- 1} \int_ {0} ^ {\infty} \sin (2 \pi \rho r) f _ {0} (r) r d r.\tag{10}
$$

The proof of this identity is based on the formula for the Fourier transform of the surface element dσ given in Lemma 3.5: 

$$
\begin{array}{r l} & F _ {0} (\rho) = \hat {f} (\xi) = \int_ {\mathbb {R} ^ {3}} f (x) e ^ {- 2 \pi i x \cdot \xi} d x \\ & \qquad = \int_ {0} ^ {\infty} f _ {0} (r) \int_ {S ^ {2}} e ^ {- 2 \pi i r \gamma \cdot \xi} d \sigma (\gamma) r ^ {2} d r \\ & \qquad = \int_ {0} ^ {\infty} f _ {0} (r) \frac {2 \sin (2 \pi \rho r)}{\rho r} r ^ {2} d r \\ & \qquad = 2 \rho^ {- 1} \int_ {0} ^ {\infty} \sin (2 \pi \rho r) f _ {0} (r) r d r. \end{array}
$$

More generally, the relation between $f _ { 0 }$ and $F _ { 0 }$ has a nice description in terms of a family of special functions that arise naturally in problems that exhibit radial symmetry. 

The Bessel function of order $n \in \mathbb { Z }$ , denoted $J _ { n } ( \rho )$ , is defined as the $n ^ { \mathrm { t h } }$ Fourier coeficient of the function $e ^ { i \rho \sin \theta }$ . So 

$$
J _ {n} (\rho) = \frac {1}{2 \pi} \int_ {0} ^ {2 \pi} e ^ {i \rho \sin \theta} e ^ {- i n \theta} d \theta ,
$$

therefore 

$$
e ^ {i \rho \sin \theta} = \sum_ {n = - \infty} ^ {\infty} J _ {n} (\rho) e ^ {i n \theta}.
$$

As a result of this definition, we find that when $d = 2$ , the relation between $f _ { 0 }$ and $F _ { 0 }$ is 

$$
F _ {0} (\rho) = 2 \pi \int_ {0} ^ {\infty} J _ {0} (2 \pi r \rho) f _ {0} (r) r d r.\tag{11}
$$

Indeed, since $\hat { f } ( \xi )$ is radial we take $\xi = ( 0 , - \rho )$ so that 

$$
\begin{array}{r l} & {\hat {f} (\xi) = \int_ {\mathbb {R} ^ {2}} f (x) e ^ {2 \pi i x \cdot (0, \rho)} d x} \\ & {\qquad = \int_ {0} ^ {2 \pi} \int_ {0} ^ {\infty} f _ {0} (r) e ^ {2 \pi i r \rho \sin \theta} r d r d \theta} \\ & {\qquad = 2 \pi \int_ {0} ^ {\infty} J _ {0} (2 \pi r \rho) f _ {0} (r) r d r,} \end{array}
$$

as desired. 

In general, there are corresponding formulas relating $f _ { 0 }$ and $F _ { 0 }$ in $\mathbb { R } ^ { d }$ in terms of Bessel functions of order $d / 2 - 1$ (see Problem 2). In even dimensions, these are the Bessel functions we have defined above. For odd dimensions, we need a more general definition of Bessel functions to encompass half-integral orders. Note that the formulas for the Fourier transform of radial functions give another illustration of the diferences between odd and even dimensions. When $d = 1$ or $d = 3$ (as well as d > 3, d odd) the formulas are in terms of elementary functions, but this is not the case when d is even. 

## 5 The Radon transform and some of its applications

Invented by Johann Radon in 1917, the integral transform we discuss next has many applications in mathematics and other sciences, including a significant achievement in medicine. To motivate the definitions and the central problem of reconstruction, we first present the close connection between the Radon transform and the development of X-ray scans (or CAT scans) in the theory of medical imaging. The solution of the reconstruction problem, and the introduction of new algorithms and faster computers, all contributed to a rapid development of computerized tomography. In practice, X-ray scans provide a “picture” of an internal organ, one that helps to detect and locate many types of abnormalities. 

After a brief description of X-ray scans in two dimensions, we define the X-ray transform and formulate the basic problem of inverting this mapping. Although this problem has an explicit solution in $\mathbb { R } ^ { 2 }$ , it is more complicated than the analogous problem in three dimensions, hence we give a complete solution of the reconstruction problem only in $\mathbb { R } ^ { 3 }$ Here we have another example where results are simpler in the odddimensional case than in the even-dimensional situation. 

## 5.1 The X-ray transform in $\mathbb { R } ^ { 2 }$

Consider a two-dimensional object O lying in the plane $\mathbb { R } ^ { 2 }$ , which we may think of as a planar cross section of a human organ. 

First, we assume that O is homogeneous, and suppose that a very narrow beam of X-ray photons traverses this object. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2ab5d4b2-da28-455b-b554-908156ef0c8e/95c41efb5f4f825dcfa10ce3b5c307b342fdd7e826be4072ad7ca3724a271e0a.jpg)



Figure 4. Attenuation of an X-ray beam


If $I _ { 0 }$ and I denote the intensity of the beam before and after passing through O, respectively, the following relation holds: 

$$
I = I _ {0} e ^ {- d \rho}.
$$

Here d is the distance traveled by the beam in the object, and $\rho$ denotes the attenuation coeficient (or absorption coeficient), which depends on the density and other physical characteristics of O. If the object is not homogeneous, but consists of two materials with attenuation coeficients $\rho _ { 1 }$ and $\rho _ { 2 }$ , then the observed decrease in the intensity of the beam is 

given by 

$$
I = I _ {0} e ^ {- d _ {1} \rho_ {1} - d _ {2} \rho_ {2}}
$$

where $d _ { 1 }$ and $d _ { 2 }$ denote the distances traveled by the beam in each material. In the case of an arbitrary object whose density and physical characteristics vary from point to point, the attenuation factor is a function $\rho$ in $\mathbb { R } ^ { 2 }$ , and the above relations become 

$$
I = I _ {0} e ^ {\int_ {L} \rho}.
$$

Here $L$ is the line in $\mathbb { R } ^ { 2 }$ traced by the beam, and $\textstyle \int _ { L } \rho$ denotes the line integral of $\rho$ over $L .$ Since we observe I and $I _ { 0 }$ , the data we gather after sending the X-ray beam through the object along the line $L$ is the quantity 

$$
\int_ {L} \rho .
$$

Since we may initially send the beam in any given direction, we may calculate the above integral for every line in $\mathbb { R } ^ { 2 }$ . We define the X-ray transform (or Radon transform in $\mathbb { R } ^ { 2 } )$ of $\rho$ by 

$$
X (\rho) (L) = \int_ {L} \rho .
$$

Note that this transform assigns to each appropriate function $\rho$ on $\mathbb { R } ^ { 2 }$ (for example, $\rho \in { \mathcal { S } } ( \mathbb { R } ^ { 2 } ) ,$ ) another function $X ( \rho )$ whose domain is the set of lines $L$ in $\mathbb { R } ^ { 2 }$ . 

The unknown is $\rho ,$ and since our original interest lies precisely in the composition of the object, the problem now becomes to reconstruct the function $\rho$ from the collected data, that is, its X-ray transform. We therefore pose the following reconstruction problem: Find a formula for $\rho$ in terms of $X ( \rho )$ 

Mathematically, the problem asks for a formula giving the inverse of $X$ . Does such an inverse even exist? As a first step, we pose the following simpler uniqueness question: If $X ( \rho ) = X ( \rho ^ { \prime } )$ , can we conclude that $\rho =$ $\rho ^ { \prime } \ ?$ 

There is a reasonable a priori expectation that $X ( \rho )$ actually determines $\rho ,$ as one can see by counting the dimensionality (or degrees of freedom) involved. A function $\rho$ on $\mathbb { R } ^ { 2 }$ depends on two parameters (the $x _ { 1 }$ and $x _ { 2 }$ coordinates, for example). Similarly, the function $X ( \rho )$ , which is a function of lines $L ,$ is also determined by two parameters (for example, the slope of $L$ and its $x _ { 2 } { \mathrm { - i n t e r c e p t } } )$ . In this sense, $\rho$ and $X ( \rho )$ 

convey an equivalent amount of information, so it is not unreasonable to suppose that $X ( \rho )$ determines $\rho .$ 

While there is a satisfactory answer to the reconstruction problem, and a positive answer to the uniqueness question in $\mathbb { R } ^ { 2 }$ , we shall forego giving them here. (However, see Exercise 13 and Problem 8.) Instead we shall deal with the analogous but simpler situation in $\mathbb { R } ^ { 3 }$ 

Let us finally remark that in fact, one can sample the X-ray transform, and determine $X ( \rho ) ( L )$ for only finitely many lines. Therefore, the reconstruction method implemented in practice is based not only on the general theory, but also on sampling procedures, numerical approximations, and computer algorithms. It turns out that a method used in developing efective relevant algorithms is the fast Fourier transform, which incidentally we take up in the next chapter. 

## 5.2 The Radon transform in $\mathbb { R } ^ { 3 }$

The experiment described in the previous section applies in three dimensions as well. If O is an object in $\mathbb { R } ^ { 3 }$ determined by a function $\rho$ which describes the density and physical characteristics of this object, sending an X-ray beam through O determines the quantity 

$$
\int_ {L} \rho ,
$$

for every line in $\mathbb { R } ^ { 3 }$ . In $\mathbb { R } ^ { 2 }$ this knowledge was enough to uniquely determine $\rho ,$ but in $\mathbb { R } ^ { 3 }$ we do not need as much data. In fact, by using the heuristic argument above of counting the number of degrees of freedom, we see that for functions $\rho$ in $\mathbb { R } ^ { 3 }$ the number is three, while the number of parameters determining a line $L$ in $\mathbb { R } ^ { 3 }$ is four (for example, two for the intercept in the $( x _ { 1 } , x _ { 2 } )$ plane, and two more for the direction of the line). Thus in this sense, the problem is over-determined. 

We turn instead to the natural mathematical generalization of the twodimensional problem. Here we wish to determine the function in $\mathbb { R } ^ { 3 }$ by knowing its integral over all $p l a n e s ^ { 3 }$ in $\mathbb { R } ^ { 3 }$ . To be precise, when we speak of a plane, we mean a plane not necessarily passing through the origin. If $\mathcal { P }$ is such a plane, we define the Radon transform $\textstyle { \mathcal { R } } ( f )$ by 

$$
\mathcal {R} (f) (\mathcal {P}) = \int_ {\mathcal {P}} f.
$$

To simplify our presentation, we shall follow our practice of assuming that we are dealing with functions in the class $S ( \mathbb { R } ^ { 3 } )$ . However, many of the results obtained below can be shown to be valid for much larger classes of functions. 

First, we explain what we mean by the integral of f over a plane. The description we use for planes in $\mathbb { R } ^ { 3 }$ is the following: given a unit vector $\gamma \in S ^ { 2 }$ and a number $t \in \mathbb { R }$ , we define the plane $\mathcal { P } _ { t , \gamma }$ by 

$$
\mathcal {P} _ {t, \gamma} = \{x \in \mathbb {R} ^ {3}: x \cdot \gamma = t \}.
$$

So we parametrize a plane by a unit vector γ orthogonal to it, and by its “distance” t to the origin (see Figure 5). Note that $\mathcal { P } _ { t , \gamma } = \mathcal { P } _ { - t , - \gamma } ,$ , and we allow t to take negative values. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2ab5d4b2-da28-455b-b554-908156ef0c8e/84cd8d9f2705f34a3008700e870cbc5ebb0da6cec5202999730449fcff4f83c1.jpg)



Figure 5. Description of a plane in $\mathbb { R } ^ { 3 }$


Given a function $f \in S ( \mathbb { R } ^ { d } )$ , we need to make sense of its integral over $\mathcal { P } _ { t , \gamma }$ . We proceed as follows. Choose unit vectors $e _ { 1 } , e _ { 2 }$ so that $e _ { 1 } , e _ { 2 } , \gamma$ is an orthonormal basis for $\mathbb { R } ^ { 3 }$ . Then any $x \in \mathcal { P } _ { t , \gamma }$ can be written uniquely as 

$$
x = t \gamma + u \quad \text { where } \quad u = u _ {1} e _ {1} + u _ {2} e _ {2} \quad \text { with } u _ {1}, u _ {2} \in \mathbb {R}.
$$

If $f \in { \mathcal { S } } ( \mathbb { R } ^ { 3 } )$ , we define 

$$
\int_ {\mathcal {P} _ {t, \gamma}} f = \int_ {\mathbb {R} ^ {2}} f (t \gamma + u _ {1} e _ {1} + u _ {2} e _ {2}) d u _ {1} d u _ {2}.\tag{12}
$$

To be consistent, we must check that this definition is independent of the choice of the vectors $e _ { 1 } , e _ { 2 }$ 

Proposition 5.1 If $f \in { \cal S } ( \mathbb { R } ^ { 3 } )$ , then for each $\gamma$ the definition of $\int _ { \mathcal { P } _ { t , \gamma } } f$ is independent of the choice $o f e _ { 1 }$ and $e _ { 2 }$ . Moreover 

$$
\int_ {- \infty} ^ {\infty} \left(\int_ {\mathcal {P} _ {t, \gamma}} f\right) d t = \int_ {\mathbb {R} ^ {3}} f (x) d x.
$$

Proof. If $e _ { 1 } ^ { \prime } , e _ { 2 } ^ { \prime }$ is another choice of basis vectors so that $\gamma , e _ { 1 } ^ { \prime } , e _ { 2 } ^ { \prime }$ is orthonormal, consider the rotation $R$ in $\mathbb { R } ^ { 2 }$ which takes $e _ { 1 }$ to $e _ { 1 } ^ { \prime }$ and $e _ { 2 }$ to $e _ { 2 } ^ { \prime }$ . Changing variables $u ^ { \prime } = R ( u )$ in the integral proves that our definition (12) is independent of the choice of basis. 

To prove the formula, let R denote the rotation which takes the standard basis of unit vectors<sup>4</sup> in $\mathbb { R } ^ { 3 }$ to $\gamma , e _ { 1 }$ , and $e _ { 2 }$ . Then 

$$
\begin{array}{l} \int_ {\mathbb {R} ^ {3}} f (x) d x = \int_ {\mathbb {R} ^ {3}} f (R x) d x \\ \qquad = \int_ {\mathbb {R} ^ {3}} f (x _ {1} \gamma + x _ {2} e _ {1} + x _ {3} e _ {2}) d x _ {1} d x _ {2} d x _ {3} \\ \qquad = \int_ {- \infty} ^ {\infty} \left(\int_ {\mathcal {P} _ {t, \gamma}} f\right) d t. \end{array}
$$

Remark. We digress to point out that the X-ray transform determines the Radon transform, since two-dimensional integrals can be expressed as iterated one-dimensional integrals. In other words, the knowledge of the integral of a function over all lines determines the integral of that function over any plane. 

Having disposed of these preliminary matters, we turn to the study of the original problem. The Radon transform of a function $f \in { \cal S } ( \mathbb { R } ^ { 3 } )$ is defined by 

$$
\mathcal {R} (f) (t, \gamma) = \int_ {\mathcal {P} _ {t, \gamma}} f.
$$

In particular, we see that the Radon transform is a function on the set of planes in $\mathbb { R } ^ { 3 }$ . From the parametrization given for a plane, we may equivalently think of $\textstyle { \mathcal { R } } ( f )$ as a function on the product $\mathbb { R } \times S ^ { 2 } =$ $\{ ( t , \gamma ) : \ t \in \mathbb { R } , \ \gamma \in S ^ { 2 } \}$ , where $S ^ { 2 }$ denotes the unit sphere in $\mathbb { R } ^ { 3 }$ . The relevant class of functions on $\mathbb { R } \times S ^ { 2 }$ consists of those that satisfy the Schwartz condition in t uniformly in $\gamma$ . In other words, we define $S ( \mathbb { R } \times$ $S ^ { 2 } )$ to be the space of all continuous functions $F ( t , \gamma )$ that are indefinitely 

diferentiable in t, and that satisfy 

$$
\sup _ {t \in \mathbb {R}, \gamma \in S ^ {2}} | t | ^ {k} \left| \frac {d ^ {\ell} F}{\partial t ^ {\ell}} (t, \gamma) \right| <   \infty \quad \text { for   all   integers } k, \ell \geq 0.
$$

Our goal is to solve the following problems. 

Uniqueness problem: If $\mathcal { R } ( f ) = \mathcal { R } ( g )$ , then $f = g$ 

## Reconstruction problem: Express f in terms of $\textstyle { \mathcal { R } } ( f )$

The solutions will be obtained by using the Fourier transform. In fact, the key point is a very elegant and essential relation between the Radon and Fourier transforms. 

Lemma 5.2 $I f f \in { \cal S } ( \mathbb { R } ^ { 3 } )$ , then $\mathcal { R } ( f ) ( t , \gamma ) \in S ( \mathbb { R } )$ for each fixed $\gamma$ . Moreover, 

$$
\widehat {\mathcal {R}} (f) (s, \gamma) = \widehat {f} (s \gamma).
$$

To be precise, $\hat { f }$ denotes the (three-dimensional) Fourier transform of $f ,$ while $\widehat { \mathcal { R } } ( f ) ( s , \gamma )$ denotes the one-dimensional Fourier transform of $\mathcal { R } ( f ) ( t , \gamma )$ as a function of $t ,$ with $\gamma$ fixed. 

Proof. Since $f \in { \mathcal { S } } ( \mathbb { R } ^ { 3 } )$ , for every positive integer N there is a constant $A _ { N } < \infty$ so that 

$$
(1 + | t |) ^ {N} (1 + | u |) ^ {N} | f (t \gamma + u) | \leq A _ {N},
$$

if we recall that $x = t \gamma + u _ { \mathrm { { i } } }$ where $\gamma$ is orthogonal to $u .$ Therefore, as soon as $N \geq 3$ , we find 

$$
(1 + | t |) ^ {N} \mathcal {R} (f) (t, \gamma) \leq A _ {N} \int_ {\mathbb {R} ^ {2}} \frac {d u}{(1 + | u |) ^ {N}} <   \infty .
$$

A similar argument for the derivatives shows that $\mathcal { R } ( f ) ( t , \gamma ) \in S ( \mathbb { R } )$ for each fixed $\gamma$ . 

To establish the identity, we first note that 

$$
\begin{array}{c} \widehat {\mathcal {R}} (f) (s, \gamma) = \int_ {- \infty} ^ {\infty} \left(\int_ {\mathcal {P} _ {t, \gamma}} f\right) e ^ {- 2 \pi i s t} d t \\ = \int_ {- \infty} ^ {\infty} \int_ {\mathbb {R} ^ {2}} f (t \gamma + u _ {1} e _ {1} + u _ {2} e _ {2}) d u _ {1} d u _ {2} e ^ {- 2 \pi i s t} d t. \end{array}
$$

5. The Radon transform and some of its applications 

However, since $\gamma \cdot u = 0$ and $| \gamma | = 1$ , we may write 

$$
e ^ {- 2 \pi i s t} = e ^ {- 2 \pi i s \gamma \cdot (t \gamma + u)}.
$$

As a result, we find that 

$$
\begin{array}{r} \widehat {\mathcal {R}} (f) (s, \gamma) = \int_ {- \infty} ^ {\infty} \int_ {\mathbb {R} ^ {2}} f (t \gamma + u _ {1} e _ {1} + u _ {2} e _ {2}) e ^ {- 2 \pi i s \gamma \cdot (t \gamma + u)} d u _ {1} d u _ {2} d t \\ = \int_ {- \infty} ^ {\infty} \int_ {\mathbb {R} ^ {2}} f (t \gamma + u) e ^ {- 2 \pi i s \gamma \cdot (t \gamma + u)} d u d t. \end{array}
$$

A final rotation from $\gamma , e _ { 1 } , e _ { 2 }$ to the standard basis in $\mathbb { R } ^ { 3 }$ proves that $\widehat { \mathcal { R } } ( f ) ( s , \gamma ) = \widehat { f } ( s \gamma )$ , as desired. 

As a consequence of this identity, we can answer the uniqueness question for the Radon transform in $\mathbb { R } ^ { 3 }$ in the afirmative. 

Corollary 5.3 If $f , g \in { \mathcal { S } } ( \mathbb { R } ^ { 3 } )$ and $\mathcal { R } ( f ) = \mathcal { R } ( g )$ , then $f = g$ 

The proof of the corollary follows from an application of the lemma to the diference $f - g$ and use of the Fourier inversion theorem. 

Our final task is to give the formula that allows us to recover $f$ from its Radon transform. Since $\textstyle { \mathcal { R } } ( f )$ is a function on the set of planes in $\mathbb { R } ^ { 3 }$ , and $f$ is a function of the space variables $\boldsymbol { x } \in \mathbb { R } ^ { 3 }$ , to recover $f$ we introduce the dual Radon transform, which passes from functions defined on planes to functions in $\mathbb { R } ^ { 3 }$ 

Given a function $F$ on $\mathbb { R } \times S ^ { 2 }$ , we define its dual Radon transform by 

$$
\mathcal {R} ^ {*} (F) (x) = \int_ {S ^ {2}} F (x \cdot \gamma , \gamma) d \sigma (\gamma).\tag{13}
$$

Observe that a point x belongs to $\mathcal { P } _ { t , \gamma }$ if and only if $x \cdot \gamma = t ,$ , so the idea here is that given $x \in \mathbb { R } ^ { 3 }$ , we obtain ${ \dot { \mathcal { R } } } ^ { * } ( F ) ( x )$ by integrating $F$ over the subset of all planes passing through $x ,$ that is, 

$$
\mathcal {R} ^ {*} (F) (x) = \int_ {\{\mathcal {P} _ {t, \gamma} \mathrm{suchthat} x \in \mathcal {P} _ {t, \gamma} \}} F,
$$

where the integral on the right is given the precise meaning in (13). We use the terminology “dual” because of the following observation. If $V _ { 1 } = S ( \mathbb { R } ^ { 3 } )$ ) with the usual Hermitian inner product 

$$
(f, g) _ {1} = \int_ {\mathbb {R} ^ {3}} f (x) \overline {{g (x)}} d x,
$$

and $V _ { 2 } = S ( \mathbb { R } \times S ^ { 2 } )$ with the Hermitian inner product 

$$
(F, G) _ {2} = \int_ {\mathbb {R}} \int_ {S ^ {2}} F (t, \gamma) \overline {{G (t , \gamma)}} d \sigma (\gamma) d t,
$$

then 

$$
\mathcal {R}: V _ {1} \to V _ {2}, \quad \mathcal {R} ^ {*}: V _ {2} \to V _ {1},
$$

with 

(14) 

$$
(\mathcal {R} f, F) _ {2} = (f, \mathcal {R} ^ {*} F) _ {1}.
$$

The validity of this identity is not needed in the argument below, and its verification is left as an exercise for the reader. 

We can now state the reconstruction theorem. 

Theorem 5.4 $I f f \in S ( \mathbb { R } ^ { 3 } )$ , then 

$$
\triangle (\mathcal {R} ^ {*} \mathcal {R} (f)) = - 8 \pi^ {2} f.
$$

We recall that $\begin{array} { r } { \triangle = \frac { \partial ^ { 2 } } { \partial x _ { 1 } ^ { 2 } } + \frac { \partial ^ { 2 } } { \partial x _ { 2 } ^ { 2 } } + \frac { \partial ^ { 2 } } { \partial x _ { 3 } ^ { 2 } } } \end{array}$ is the Laplacian. 

Proof. By our previous lemma, we have 

$$
\mathcal {R} (f) (t, \gamma) = \int_ {- \infty} ^ {\infty} \hat {f} (s \gamma) e ^ {2 \pi i t s} d s.
$$

Therefore 

$$
\mathcal {R} ^ {*} \mathcal {R} (f) (x) = \int_ {S ^ {2}} \int_ {- \infty} ^ {\infty} \hat {f} (s \gamma) e ^ {2 \pi i x \cdot \gamma s} d s d \sigma (\gamma),
$$

hence 

$$
\begin{array}{r l} & {\triangle (\mathcal {R} ^ {*} \mathcal {R} (f)) (x) = \int_ {S ^ {2}} \int_ {- \infty} ^ {\infty} \hat {f} (s \gamma) (- 4 \pi^ {2} s ^ {2}) e ^ {2 \pi i x \cdot \gamma s} d s d \sigma (\gamma)} \\ & {\qquad = - 4 \pi^ {2} \int_ {S ^ {2}} \int_ {- \infty} ^ {\infty} \hat {f} (s \gamma) e ^ {2 \pi i x \cdot \gamma s} s ^ {2} d s d \sigma (\gamma)} \\ & {\qquad = - 4 \pi^ {2} \int_ {S ^ {2}} \int_ {- \infty} ^ {0} \hat {f} (s \gamma) e ^ {2 \pi i x \cdot \gamma s} s ^ {2} d s d \sigma (\gamma)} \\ & {\qquad - 4 \pi^ {2} \int_ {S ^ {2}} \int_ {0} ^ {\infty} \hat {f} (s \gamma) e ^ {2 \pi i x \cdot \gamma s} s ^ {2} d s d \sigma (\gamma)} \\ & {\qquad = - 8 \pi^ {2} \int_ {S ^ {2}} \int_ {0} ^ {\infty} \hat {f} (s \gamma) e ^ {2 \pi i x \cdot \gamma s} s ^ {2} d s d \sigma (\gamma)} \\ & {\qquad = - 8 \pi^ {2} f (x).} \end{array}
$$

## 6. Exercises

In the first line, we have diferentiated under the integral sign and used the fact $\triangle ( e ^ { 2 \pi i x \cdot \gamma s } ) = ( - 4 \pi ^ { 2 } s ^ { 2 } ) e ^ { 2 \pi i x \cdot \gamma s }$ , since $| \gamma | = 1$ . The last step follows from the formula for polar coordinates in $\mathbb { R } ^ { 3 }$ and the Fourier inversion theorem. 

## 5.3 A note about plane waves

We conclude this chapter by briefly mentioning a nice connection between the Radon transform and solutions of the wave equation. This comes about in the following way. Recall that when $d = 1$ , the solution of the wave equation can be expressed as the sum of traveling waves (see Chapter 1), and it is natural to ask if an analogue of such traveling waves exists in higher dimensions. The answer is as follows. Let $F$ be a function of one variable, which we assume is suficiently smooth (say $C ^ { 2 } )$ , and consider $u ( x , t )$ defined by 

$$
u (x, t) = F ((x \cdot \gamma) - t),
$$

where $x \in \mathbb { R } ^ { d }$ and $\gamma$ is a unit vector in $\mathbb { R } ^ { d }$ . It is easy to verify directly that u is $\mathrm { a }$ solution of the wave equation in $\mathbb { R } ^ { d } \ ( \mathrm { w i t h \ } c = 1 )$ . Such a solution is called a plane wave; indeed, notice that u is constant on every plane perpendicular to the direction $\gamma ,$ and as time t increases, the wave travels in the $\gamma$ direction. (It should be remarked that plane waves are never functions in $S ( \mathbb { R } ^ { d } )$ when $d > 1$ because they are constant in directions perpendicular to $\gamma )$ .<sup>5</sup> 

The basic fact is that when $d > 1$ , the solution of the wave equation can be written as an integral (as opposed to sum, when $d = 1 )$ of plane waves; this can in fact be done via the Radon transform of the initial data $f$ and $g .$ For the relevant formulas when $d = 3 .$ see Problem 6. 

## 6 Exercises

1. Suppose that R is a rotation in the plane $\mathbb { R } ^ { 2 }$ , and let 

$$
R = \left( \begin{array}{c c} a & b \\ c & d \end{array} \right)
$$

denote its matrix with respect to the standard basis vectors $e _ { 1 } = ( 1 , 0 )$ and $e _ { 2 } = ( 0 , 1 )$ 

(a) Write the conditions $R ^ { t } = R ^ { - 1 }$ and det $( R ) = \pm 1$ in terms of equations in $a , b , c , d .$ 

(b) Show that there exists $\varphi \in \mathbb { R }$ such that $a + i b = e ^ { i \varphi }$ 

(c) Conclude that if R is proper, then it can be expressed as $z \mapsto z e ^ { i \varphi }$ , and if R is improper, then it takes the form $z \mapsto { \overline { { z } } } e ^ { i \varphi }$ , where ${ \overline { { z } } } = x - i y$ 

2. Suppose that $R : \mathbb { R } ^ { 3 } \longrightarrow \mathbb { R } ^ { 3 }$ is a proper rotation. 

(a) Show that $p ( t ) = \operatorname* { d e t } ( R - t I )$ is a polynomial of degree $^ { 3 , }$ and prove that there exists $\gamma \in S ^ { 2 }$ (where $S ^ { \overset { \cdot } { 2 } }$ denotes the unit sphere in $\mathbb { R } ^ { 3 } )$ with 

$$
R (\gamma) = \gamma .
$$

[Hint: Use the fact that $p ( 0 ) > 0$ to see that there is $\lambda > 0$ with $p ( \lambda ) = 0$ Then $R - \lambda I$ is singular, so its kernel is non-trivial.] 

(b) If P denotes the plane perpendicular to $\gamma$ and passing through the origin, show that 

$$
R: \mathcal {P} \to \mathcal {P},
$$

and that this linear map is a rotation. 

## 3. Recall the formula

$$
\int_ {\mathbb {R} ^ {d}} F (x) d x = \int_ {S ^ {d - 1}} \int_ {0} ^ {\infty} F (r \gamma) r ^ {d - 1} d r d \sigma (\gamma).
$$

Apply this to the special case when $\begin{array} { r } { F ( x ) = g ( r ) f ( \gamma ) } \end{array}$ , where $x = r \gamma _ { \mathrm { { } } }$ , to prove that for any rotation $R ,$ one has 

$$
\int_ {S ^ {d - 1}} f (R (\gamma)) d \sigma (\gamma) = \int_ {S ^ {d - 1}} f (\gamma) d \sigma (\gamma),
$$

whenever $f$ is a continuous function on the sphere $S ^ { d - 1 }$ 

4. Let $A _ { d }$ and $V _ { d }$ denote the area and volume of the unit sphere and unit ball in $\mathbb { R } ^ { d }$ , respectively. 

(a) Prove the formula 

$$
A _ {d} = \frac {2 \pi^ {d / 2}}{\Gamma (d / 2)}
$$

so that $A _ { 2 } = 2 \pi , \ A _ { 3 } = 4 \pi , \ A _ { 4 } = 2 \pi ^ { 2 } , \ldots$ . Here $\textstyle \Gamma ( x ) = \int _ { 0 } ^ { \infty } e ^ { - t } t ^ { x - 1 } d t$ is the Gamma function. [Hint: Use polar coordinates and the fact that $\begin{array} { r } { \int _ { \mathbb { R } ^ { d } } e ^ { - \pi | x | ^ { 2 } } d x = 1 . } \end{array}$ 

6. Exercises 

(b) Show that d $V _ { d } = A _ { d } .$ , hence 

$$
V _ {d} = \frac {\pi^ {d / 2}}{\Gamma (d / 2 + 1)}.
$$

In particular $V _ { 2 } = \pi , V _ { 3 } = 4 \pi / 3 ,$ 

5. Let A be a $d \times d$ positive definite symmetric matrix with real coeficients. Show that 

$$
\int_ {\mathbb {R} ^ {d}} e ^ {- \pi (x, A (x))} d x = (\det (A)) ^ {- 1 / 2}.
$$

This generalizes the fact that $\begin{array} { r } { \int _ { \mathbb { R } ^ { d } } e ^ { - \pi | x | ^ { 2 } } d x = 1 } \end{array}$ , which corresponds to the case where A is the identity. 

[Hint: Apply the spectral theorem to write $A = R D R ^ { - 1 }$ where R is a rotation and, D is diagonal with entries $\lambda _ { 1 } , \ldots , \lambda _ { d } .$ , where $\{ \lambda _ { i } \}$ are the eigenvalues of $A . ]$ 

6. Suppose $\psi \in { \mathcal { S } } ( \mathbb { R } ^ { d } )$ satisfies $\textstyle \int { | \psi ( x ) | ^ { 2 } d x = 1 }$ . Show that 

$$
\left(\int_ {\mathbb {R} ^ {d}} | x | ^ {2} | \psi (x) | ^ {2} d x\right) \left(\int_ {\mathbb {R} ^ {d}} | \xi | ^ {2} | \hat {\psi} (\xi) | ^ {2} d \xi\right) \geq \frac {d ^ {2}}{1 6 \pi^ {2}}.
$$

This is the statement of the Heisenberg uncertainty principle in d dimensions. 

7. Consider the time-dependent heat equation in $\mathbb { R } ^ { d } \mathrm { : }$ 

$$
\frac {\partial u}{\partial t} = \frac {\partial^ {2} u}{\partial x _ {1} ^ {2}} + \dots + \frac {\partial^ {2} u}{\partial x _ {d} ^ {2}}, \quad \mathrm{where} t > 0,\tag{15}
$$

with boundary values $u ( x , 0 ) = f ( x ) \in S ( \mathbb R ^ { d } )$ . If 

$$
\mathcal {H} _ {t} ^ {(d)} (x) = \frac {1}{(4 \pi t) ^ {d / 2}} e ^ {- | x | ^ {2} / 4 t} = \int_ {\mathbb {R} ^ {d}} e ^ {- 4 \pi^ {2} t | \xi | ^ {2}} e ^ {2 \pi i x \cdot \xi} d \xi
$$

is the d-dimensional heat kernel, show that the convolution 

$$
u (x, t) = (f * \mathcal {H} _ {t} ^ {(d)}) (x)
$$

is indefinitely diferentiable when $x \in \mathbb { R } ^ { d }$ and $t > 0$ . Moreover, u solves (15), and is continuous up to the boundary $t = 0$ with $u ( x , 0 ) = f ( x )$ 

The reader may also wish to formulate the d-dimensional analogues of Theorem 2.1 and 2.3 in Chapter $5 .$ 

8. In Chapter $5 ,$ we found that a solution to the steady-state heat equation in the upper half-plane with boundary values $f$ is given by the convolution $u = f * \mathcal { P } _ { y }$ where the Poisson kernel is 

$$
\mathcal {P} _ {y} (x) = \frac {1}{\pi} \frac {y}{x ^ {2} + y ^ {2}} \quad \text { where } x \in \mathbb {R} \text { and } y > 0.
$$

More generally, one can calculate the d-dimensional Poisson kernel using the Fourier transform as follows. 

(a) The subordination principle allows one to write expressions involving the function $e ^ { - x }$ in terms of corresponding expressions involving the function $e ^ { - x ^ { 2 } }$ . One form of this is the identity 

$$
e ^ {- \beta} = \int_ {0} ^ {\infty} \frac {e ^ {- u}}{\sqrt {\pi u}} e ^ {- \beta^ {2} / 4 u} d u
$$

when $\beta \geq 0$ . Prove this identity with $\beta = 2 \pi | x |$ by taking the Fourier transform of both sides. 

(b) Consider the steady-state heat equation in the upper half-space $\{ ( x , y )$ : $x \in \mathbb { R } ^ { d } , \ y > 0 \}$ 

$$
\sum_ {j = 1} ^ {d} \frac {\partial^ {2} u}{\partial x _ {j} ^ {2}} + \frac {\partial^ {2} u}{\partial y ^ {2}} = 0
$$

with the Dirichlet boundary condition $u ( x , 0 ) = f ( x )$ . A solution to this problem is given by the convolution $u ( x , y ) = ( f * P _ { y } ^ { ( d ) } ) ( x )$ where $P _ { y } ^ { ( d ) } ( x )$ is the d-dimensional Poisson kernel 

$$
P _ {y} ^ {(d)} (x) = \int_ {\mathbb {R} ^ {d}} e ^ {2 \pi i x \cdot \xi} e ^ {- 2 \pi | \xi | y} d \xi .
$$

Compute $P _ { y } ^ { ( d ) } ( x )$ by using the subordination principle and the d-dimensional heat kernel. (See Exercise 7.) Show that 

$$
P _ {y} ^ {(d)} (x) = \frac {\Gamma ((d + 1) / 2)}{\pi^ {(d + 1) / 2}} \frac {y}{(| x | ^ {2} + y ^ {2}) ^ {(d + 1) / 2}}.
$$

9. A spherical wave is a solution $\boldsymbol { u } ( \boldsymbol { x } , t )$ of the Cauchy problem for the wave equation in $\mathbb { R } ^ { d }$ , which as a function of $x$ is radial. Prove that u is a spherical wave if and only if the initial data $f , g \in S$ are both radial. 

10. Let $u ( x , t )$ be a solution of the wave equation, and let $E ( t )$ denote the energy of this wave 

$$
E (t) = \int_ {\mathbb {R} ^ {d}} \left| \frac {\partial u}{\partial t} (x, t) \right| ^ {2} + \sum_ {j = 1} ^ {d} \int_ {\mathbb {R} ^ {d}} \left| \frac {\partial u}{\partial x _ {j}} (x, t) \right| ^ {2} d x.
$$

We have seen that $E ( t )$ is constant using Plancherel’s formula. Give an alternate proof of this fact by diferentiating the integral with respect to t and showing that 

$$
\frac {d E}{d t} = 0.
$$

6. Exercises 

[Hint: Integrate by parts.] 

11. Show that the solution of the wave equation 

$$
\frac {\partial^ {2} u}{\partial t ^ {2}} = \frac {\partial^ {2} u}{\partial x _ {1} ^ {2}} + \frac {\partial^ {2} u}{\partial x _ {2} ^ {2}} + \frac {\partial^ {2} u}{\partial x _ {3} ^ {2}}
$$

subject to $u ( x , 0 ) = f ( x )$ and $\begin{array} { r } { \frac { \partial u } { \partial t } ( x , 0 ) = g ( x ) } \end{array}$ , where $f , g \in S ( \mathbb { R } ^ { 3 } )$ , is given by 

$$
u (x, t) = \frac {1}{| S (x , t) |} \int_ {S (x, t)} [ t g (y) + f (y) + \nabla f (y) \cdot (y - x) ] d \sigma (y),
$$

where $S ( x , t )$ denotes the sphere of center x and radius $t ,$ and $\vert S ( x , t ) \vert$ its area. This is an alternate expression for the solution of the wave equation given in Theorem 3.6. It is sometimes called Kirchhof’s formula. 

12. Establish the identity (14) about the dual transform given in the text. In other words, prove that 

$$
\int_ {\mathbb {R}} \int_ {S ^ {2}} \mathcal {R} (f) (t, \gamma) \overline {{F (t , \gamma)}} d \sigma (\gamma) d t = \int_ {\mathbb {R} ^ {3}} f (x) \overline {{\mathcal {R} ^ {*} (F) (x)}} d x\tag{16}
$$

where $f \in { \cal S } ( \mathbb { R } ^ { 3 } ) , F \in { \cal S } ( \mathbb { R } \times { \cal S } ^ { 2 } )$ , and 

$$
\mathcal {R} (f) = \int_ {\mathcal {P} _ {t, \gamma}} f \quad \text { and } \quad \mathcal {R} ^ {*} (F) (x) = \int_ {S ^ {2}} F (x \cdot \gamma , \gamma)   d \sigma (\gamma).
$$

[Hint: Consider the integral 

$$
\int \int \int f (t \gamma + u _ {1} e _ {2} + u _ {2} e _ {2}) \overline {{F (t , \gamma)}} d t d \sigma (\gamma) d u _ {1} d u _ {2}.
$$

Integrating first in u gives the left-hand side of (16), while integrating in u and t and setting $x = t \gamma + u _ { 1 } e _ { 2 } + u _ { 2 } e _ { 2 }$ gives the right-hand side.] 

13. For each $( t , \theta )$ with $t \in \mathbb { R }$ and $| \theta | \leq \pi ,$ , let $L = L _ { t , \theta }$ denote the line in the $( x , y )$ -plane given by 

$$
x \cos \theta + y \sin \theta = t.
$$

This is the line perpendicular to the direction (cos θ, sin θ) at “distance” t from the origin (we allow negative t). For $f \in { \mathcal { S } } ( \mathbb { R } ^ { 2 } )$ the X-ray transform or twodimensional Radon transform of f is defined by 

$$
X (f) (t, \theta) = \int_ {L _ {t, \theta}} f = \int_ {- \infty} ^ {\infty} f (t \cos \theta + u \sin \theta , t \sin \theta - u \cos \theta) d u.
$$

Calculate the X-ray transform of the function $f ( x , y ) = e ^ { - \pi ( x ^ { 2 } + y ^ { 2 } ) }$ 

14. Let X be the X-ray transform. Show that if $f \in S$ and $X ( f ) = 0$ , then $f = 0 ,$ , by taking the Fourier transform in one variable. 

15. For $F \in { \mathcal { S } } ( \mathbb { R } \times S ^ { 1 } )$ , define the dual X-ray transform $X ^ { * } ( F )$ by integrating F over all lines that pass through the point $( x , y )$ (that is, those lines $L _ { t , \theta }$ with x cos $\theta + y$ sin $\theta = t )$ 

$$
X ^ {*} (F) (x, y) = \int F (x \cos \theta + y \sin \theta , \theta) d \theta .
$$

Check that in this case, if $f \in { \cal S } ( \mathbb { R } ^ { 2 } )$ and $F \in { \mathcal { S } } ( \mathbb { R } \times S ^ { 1 } )$ , then 

$$
\int \int X (f) (t, \theta) \overline {{F (t , \theta)}} d t d \theta = \int \int f (x, y) \overline {{X ^ {*} (F) (x , y)}} d x d y.
$$

## 7 Problems

1. Let $J _ { n }$ denote the $n ^ { \mathrm { t h } }$ order Bessel function, for $n \in \mathbb { Z }$ . Prove that 

(a) $J _ { n } ( \rho )$ is real for all real $\rho .$ 

(b) $J _ { - n } ( \rho ) = ( - 1 ) ^ { n } J _ { n } ( \rho )$ 

(c) $2 J _ { n } ^ { \prime } ( \rho ) = J _ { n - 1 } ( \rho ) - J _ { n + 1 } ( \rho ) .$ 

(d) $\begin{array} { r } { \left( \frac { 2 n } { \rho } \right) J _ { n } ( \rho ) = J _ { n - 1 } ( \rho ) + J _ { n + 1 } ( \rho ) . } \end{array}$ 

(e) $( \rho ^ { - n } J _ { n } ( \rho ) ) ^ { \prime } = - \rho ^ { - n } J _ { n + 1 } ( \rho ) .$ 

(f) $( \rho ^ { n } J _ { n } ( \rho ) ) ^ { \prime } = \rho ^ { n } J _ { n - 1 } ( \rho )$ 

(g) $J _ { n } ( \rho )$ satisfies the second order diferential equation 

$$
J _ {n} ^ {\prime \prime} (\rho) + \rho^ {- 1} J _ {n} ^ {\prime} (\rho) + (1 - n ^ {2} / \rho^ {2}) J _ {n} (\rho) = 0.
$$

(h) Show that 

$$
J _ {n} (\rho) = \left(\frac {\rho}{2}\right) ^ {n} \sum_ {m = 0} ^ {\infty} (- 1) ^ {m} \frac {\rho^ {2 m}}{2 ^ {2 m} m ! (n + m) !}.
$$

(i) Show that for all integers n and all real numbers a and b we have 

$$
J _ {n} (a + b) = \sum_ {\ell \in \mathbb {Z}} J _ {\ell} (a) J _ {n - \ell} (b).
$$

## 7. Problems

2. Another formula for $J _ { n } ( \rho )$ that allows one to define Bessel functions for non-integral values of $n , ( n > - 1 / 2 )$ is 

$$
J _ {n} (\rho) = \frac {(\rho / 2) ^ {n}}{\Gamma (n + 1 / 2) \sqrt {\pi}} \int_ {- 1} ^ {1} e ^ {i \rho t} (1 - t ^ {2}) ^ {n - (1 / 2)} d t.
$$

(a) Check that the above formula agrees with the definition of $J _ { n } ( \rho )$ for integral $n \geq 0$ . [Hint: Verify it for $n = 0$ and then check that both sides satisfy the recursion formula (e) in Problem 1.] 

(b) Note that $\begin{array} { r } { J _ { 1 / 2 } ( \rho ) = \sqrt { \frac { 2 } { \pi } } \rho ^ { - 1 / 2 } \sin \rho . } \end{array}$ 

(c) Prove that 

$$
\lim _ {n \to - 1 / 2} J _ {n} (\rho) = \sqrt {\frac {2}{\pi}} \rho^ {- 1 / 2} \cos \rho .
$$

(d) Observe that the formulas we have proved in the text giving $F _ { 0 }$ in terms of $f _ { 0 }$ (when describing the Fourier transform of a radial function) take the form 

$$
F _ {0} (\rho) = 2 \pi \rho^ {- (d / 2) + 1} \int_ {0} ^ {\infty} J _ {(d / 2) - 1} (2 \pi \rho r) f _ {0} (r) r ^ {d / 2} d r,\tag{17}
$$

for $d = 1 , 2 ,$ and 3, if one uses the formulas above with the understanding that $\begin{array} { r } { J _ { - 1 / 2 } ( \rho ) = \operatorname* { l i m } _ { n \to - 1 / 2 } J _ { n } ( \rho ) } \end{array}$ . It turns out that the relation between $F _ { 0 }$ and $f _ { 0 }$ given by (17) is valid in all dimensions d. 

3. We observed that the solution $u ( x , t )$ of the Cauchy problem for the wave equation given by formula (3) depends only on the initial data on the base on the backward light cone. It is natural to ask if this property is shared by any solution of the wave equation. An afirmative answer would imply uniqueness of the solution. 

Let $B ( x _ { 0 } , r _ { 0 } )$ denote the closed ball in the hyperplane $t = 0$ centered at $x _ { 0 }$ and of radius $r _ { 0 }$ . The backward light cone with base $B ( x _ { 0 } , r _ { 0 } )$ is defined by 

$$
\mathcal {L} _ {B (x _ {0}, r _ {0})} = \{(x, t) \in \mathbb {R} ^ {d} \times \mathbb {R}: | x - x _ {0} | \leq r _ {0} - t, 0 \leq t \leq r _ {0} \}.
$$

Theorem Suppose that $u ( x , t )$ is a $C ^ { 2 }$ function on the closed upper half-plane $\{ ( x , t ) : \ x \in \mathbb { R } ^ { d } , t \geq 0 \}$ that solves the wave equation 

$$
\frac {\partial^ {2} u}{\partial t ^ {2}} = \triangle u.
$$

If $\begin{array} { r } { \dot { \mathbf { \sigma } } _ { u ( x , 0 ) } = \frac { \partial u } { \partial t } ( x , 0 ) = 0 } \end{array}$ for all $x \in B ( x _ { 0 } , r _ { 0 } )$ , then $u ( x , t ) = 0$ for all $( x , t ) \in$ $\mathcal { L } _ { B ( x _ { 0 } , r _ { 0 } ) }$ 

In words, if the initial data of the Cauchy problem for the wave equation vanishes on a ball $B ,$ then any solution u of the problem vanishes in the backward light cone with base B. The following steps outline a proof of the theorem. 

(a) Assume that u is real. For $0 \leq t \leq r _ { 0 }$ let $B _ { t } ( x _ { 0 } , r _ { 0 } ) = \{ x : | x - x _ { 0 } | \leq r _ { 0 }$ t}, and also define 

$$
\nabla u (x, t) = \left(\frac {\partial u}{\partial x _ {1}}, \dots , \frac {\partial u}{\partial x _ {d}}, \frac {\partial u}{\partial t}\right).
$$

Now consider the energy integral 

$$
\begin{array}{l} E (t) = \frac {1}{2} \int_ {B _ {t} (x _ {0}, r _ {0})} | \nabla u | ^ {2} d x \\ = \frac {1}{2} \int_ {B _ {t} (x _ {0}, r _ {0})} \left(\frac {\partial u}{\partial t}\right) ^ {2} + \sum_ {j = 1} ^ {d} \left(\frac {\partial u}{\partial x _ {j}}\right) ^ {2} d x. \end{array}
$$

Observe that $E ( t ) \geq 0$ and $E ( 0 ) = 0$ . Prove that 

$$
E ^ {\prime} (t) = \int_ {B _ {t} (x _ {0}, r _ {0})} \frac {\partial u}{\partial t} \frac {\partial^ {2} u}{\partial t ^ {2}} + \sum_ {j = 1} ^ {d} \frac {\partial u}{\partial x _ {j}} \frac {\partial^ {2} u}{\partial x _ {j} \partial t} d x - \frac {1}{2} \int_ {\partial B _ {t} (x _ {0}, r _ {0})} | \nabla u | ^ {2} d \sigma (\gamma).
$$

(b) Show that 

$$
\frac {\partial}{\partial x _ {j}} \left[ \frac {\partial u}{\partial x _ {j}} \frac {\partial u}{\partial t} \right] = \frac {\partial u}{\partial x _ {j}} \frac {\partial^ {2} u}{\partial x _ {j} \partial t} + \frac {\partial^ {2} u}{\partial x _ {j} ^ {2}} \frac {\partial u}{\partial t}.
$$

(c) Use the last identity, the divergence theorem, and the fact that u solves the wave equation to prove that 

$$
E ^ {\prime} (t) = \int_ {\partial B _ {t} (x _ {0}, r _ {0})} \sum_ {j = 1} ^ {d} \frac {\partial u}{\partial x _ {j}} \frac {\partial u}{\partial t} \nu_ {j} d \sigma (\gamma) - \frac {1}{2} \int_ {\partial B _ {t} (x _ {0}, r _ {0})} | \nabla u | ^ {2} d \sigma (\gamma),
$$

where $\nu _ { j }$ denotes the $j ^ { \mathrm { t h } }$ coordinate of the outward normal to $B _ { t } ( x _ { 0 } , r _ { 0 } )$ 

(d) Use the Cauchy-Schwarz inequality to conclude that 

$$
\sum_ {j = 1} ^ {d} \frac {\partial u}{\partial x _ {j}} \frac {\partial u}{\partial t} \nu_ {j} \leq \frac {1}{2} | \nabla u | ^ {2},
$$

and as a result, $E ^ { \prime } ( t ) \leq 0$ . Deduce from this that $E ( t ) = 0$ and $u = 0$ 

## 7. Problems

4.<sup>∗</sup> There exist formulas for the solution of the Cauchy problem for the wave equation 

$$
\frac {\partial^ {2} u}{\partial t ^ {2}} = \frac {\partial^ {2} u}{\partial x _ {1} ^ {2}} + \dots + \frac {\partial^ {2} u}{\partial x _ {d} ^ {2}} \quad \mathrm{with} u (x, 0) = f (x) \mathrm{and} \frac {\partial u}{\partial t} (x, 0) = g (x)
$$

in $\mathbb { R } ^ { d } \times \mathbb { R }$ in terms of spherical means which generalize the formula given in the text for $d = 3$ . In fact, the solution for even dimensions is deduced from that for odd dimensions, so we discuss this case first. 

Suppose that $d > 1$ is odd and let $h \in { \mathcal { S } } ( \mathbb { R } ^ { d } )$ . The spherical mean of h on the ball centered at x of radius t is defined by 

$$
M _ {r} h (x) = M h (x, r) = \frac {1}{A _ {d}} \int_ {S ^ {d - 1}} h (x - r \gamma) d \sigma (\gamma),
$$

where $A _ { d }$ denotes the area of the unit sphere $S ^ { d - 1 }$ in $\mathbb { R } ^ { d }$ 

(a) Show that 

$$
\triangle_ {x} M h (x, r) = \left[ \partial_ {r} ^ {2} + \frac {d - 1}{r} \right] M h (x, r),
$$

where $\triangle _ { x }$ denotes the Laplacian in the space variables x, and $\partial _ { r } = \partial / \partial r$ 

(b) Show that a twice diferentiable function $u ( x , t )$ satisfies the wave equation if and only if 

$$
\left[ \partial_ {r} ^ {2} + \frac {d - 1}{r} \right] M u (x, r, t) = \partial_ {t} ^ {2} M u (x, r, t),
$$

where $M u ( x , r , t )$ denote the spherical means of the function $\boldsymbol { u } ( \boldsymbol { x } , t )$ 

(c) If $d = 2 k + 1$ , define $T \varphi ( r ) = ( r ^ { - 1 } \partial _ { r } ) ^ { k - 1 } [ r ^ { 2 k - 1 } \varphi ( r ) ]$ , and let $\tilde { u } = T M u$ Then this function solves the one-dimensional wave equation for each fixed x: 

$$
\partial_ {t} ^ {2} \tilde {u} (x, r, t) = \partial_ {r} ^ {2} \tilde {u} (x, r, t).
$$

One can then use d’Alembert’s formula to find the solution $\tilde { u } ( \boldsymbol { x } , \boldsymbol { r } , t )$ of this problem expressed in terms of the initial data. 

(d) Now show that 

$$
u (x, t) = M u (x, 0, t) = \lim _ {r \to 0} \frac {\tilde {u} (x , r , t)}{\alpha r}
$$

where $\alpha = 1 \cdot 3 \cdot \cdot \cdot ( d - 2 )$ 

(e) Conclude that the solution of the Cauchy problem for the d-dimensional wave equation, when $d > 1$ is odd, is 

$$
u (x, t) = \frac {1}{1 \cdot 3 \cdots (d - 2)} \left[ \partial_ {t} (t ^ {- 1} \partial_ {t}) ^ {(d - 3) / 2} \left(t ^ {d - 2} M _ {t} f (x)\right) + \right.
$$

$$
\left. \left(t ^ {- 1} \partial_ {t}\right) ^ {(d - 3) / 2} \left(t ^ {d - 2} M _ {t} g (x)\right) \right].
$$

5.<sup>∗</sup> The method of descent can be used to prove that the solution of the Cauchy problem for the wave equation in the case when d is even is given by the formula 

$$
u (x, t) = \frac {1}{1 \cdot 3 \cdot \cdot \cdot (d - 2)} \left[ \partial_ {t} (t ^ {- 1} \partial_ {t}) ^ {(d - 3) / 2} \left(t ^ {d - 2} \widetilde {M _ {t}} f (x)\right) + \right.
$$

$$
\left. (t ^ {- 1} \partial_ {t}) ^ {(d - 3) / 2} \left(t ^ {d - 2} \widetilde {M _ {t}} g (x)\right) \right],
$$

where $\widetilde { M _ { t } }$ denotes the modified spherical means defined by 

$$
\widetilde {M _ {t}} h (x) = \frac {2}{A _ {d + 1}} \int_ {B ^ {d}} \frac {f (x + t y)}{\sqrt {1 - | y | ^ {2}}} d y.
$$

${ { \bf 6 . } ^ { * } }$ Given initial data f and g of the form 

$$
f (x) = F (x \cdot \gamma) \quad \text { and } \quad g (x) = G (x \cdot \gamma),
$$

check that the plane wave given by 

$$
u (x, t) = \frac {F (x \cdot \gamma + t) + F (x \cdot \gamma - t)}{2} + \frac {1}{2} \int_ {x \cdot \gamma - t} ^ {x \cdot \gamma + t} G (s) d s
$$

is a solution of the Cauchy problem for the d-dimensional wave equation. 

In general, the solution is given as a superposition of plane waves. For the case $d = 3$ , this can be expressed in terms of the Radon transform as follows. Let 

$$
\tilde {\mathcal {R}} (f) (t, \gamma) = - \frac {1}{8 \pi^ {2}} \left(\frac {d}{d t}\right) ^ {2} R (f) (t, \gamma).
$$

Then $u ( x , t ) =$ 

$$
\frac {1}{2} \int_ {S ^ {2}} \left[ \tilde {\mathcal {R}} (f) (x \cdot \gamma - t, \gamma) + \tilde {\mathcal {R}} (f) (x \cdot \gamma + t, \gamma) + \int_ {x \cdot \gamma - t} ^ {x \cdot \gamma + t} \tilde {\mathcal {R}} (g) (s, \gamma) d s \right] d \sigma (\gamma).
$$

## 7. Problems

7. For every real number $a > 0 ,$ , define the operator $( - \triangle ) ^ { a }$ by the formula 

$$
(- \triangle) ^ {a} f (x) = \int_ {\mathbb {R} ^ {d}} (2 \pi | \xi |) ^ {2 a} \hat {f} (\xi) e ^ {2 \pi i \xi \cdot x} d \xi
$$

whenever $f \in { \mathcal { S } } ( \mathbb { R } ^ { d } )$ 

(a) Check that $( - \triangle ) ^ { a }$ agrees with the usual definition of the $a ^ { \mathrm { t h } }$ power of $- \triangle$ (that is, a compositions of minus the Laplacian) when a is a positive integer. 

(b) Verify that $( - \triangle ) ^ { a } ( f )$ is indefinitely diferentiable. 

(c) Prove that if a is not an integer, then in general $( - \triangle ) ^ { a } ( f )$ is not rapidly decreasing. 

(d) Let $u ( x , y )$ be the solution of the steady-state heat equation 

$$
\frac {\partial^ {2} u}{\partial y ^ {2}} + \sum_ {j = 1} ^ {d} \frac {\partial^ {2} u}{\partial x _ {j} ^ {2}} = 0, \quad \text { with } u (x, 0) = f (x),
$$

given by convolving f with the Poisson kernel (see Exercise $^ { 8 ) }$ . Check that 

$$
(- \triangle) ^ {1 / 2} f (x) = - \lim _ {y \rightarrow 0} \frac {\partial u}{\partial y} (x, y),
$$

and more generally that 

$$
(- \triangle) ^ {k / 2} f (x) = (- 1) ^ {k} \lim _ {y \to 0} \frac {\partial^ {k} u}{\partial y ^ {k}} (x, y)
$$

for any positive integer k. 

8.<sup>∗</sup> The reconstruction formula for the Radon transform in $\mathbb { R } ^ { d }$ is as follows: 

(a) When $d = 2 ,$ 

$$
\frac {(- \triangle) ^ {1 / 2}}{4 \pi} \mathcal {R} ^ {*} (\mathcal {R} (f)) = f,
$$

where $( - \triangle ) ^ { 1 / 2 }$ is defined in Problem $7 .$ 

(b) If the Radon transform and its dual are defined by analogy to the cases $d = 2$ and $d = 3$ , then for general $d ,$ 

$$
\frac {(2 \pi) ^ {1 - d}}{2} (- \triangle) ^ {(d - 1) / 2} \mathcal {R} ^ {*} (\mathcal {R} (f)) = f.
$$

# 7 <sub>Finite</sub> <sub>Fourier</sub> <sub>Analysis</sub>

This past year has seen the birth, or rather the rebirth, of an exciting revolution in computing Fourier transforms. A class of algorithms known as the fast Fourier transform or FFT, is forcing a complete reassessment of many computational paths, not only in frequency analysis, but in any fields where problems can be reduced to Fourier transforms and/or convolutions... 

C. Bingham and J. W. Tukey, 1966 

In the previous chapters we studied the Fourier series of functions on the circle and the Fourier transform of functions defined on the Euclidean space $\mathbb { R } ^ { d }$ . The goal here is to introduce another version of Fourier analysis, now for functions defined on finite sets, and more precisely, on finite abelian groups. This theory is particularly elegant and simple since infinite sums and integrals are replaced by finite sums, and thus questions of convergence disappear. 

In turning our attention to finite Fourier analysis, we begin with the simplest example, $\mathbb { Z } ( N )$ , where the underlying space is the (multiplicative) group of $N ^ { \mathrm { t h } }$ roots of unity on the circle. This group can also be realized in additive form, as $\mathbb { Z } / N \mathbb { Z } ,$ the equivalence classes of integers modulo N. The group $\mathbb { Z } ( N )$ arises as the natural approximation to the circle (as N tends to infinity) since in the first picture the points of $\mathbb { Z } ( N )$ correspond to $N$ points on the circle which are uniformly distributed. For this reason, in practical applications, the group $\mathbb { Z } ( N )$ becomes a natural candidate for the storage of information of a function on the circle, and for the resulting numerical computations involving Fourier series. The situation is particularly nice when N is large and of the form $N = 2 ^ { n }$ The computations of the Fourier coeficients now lead to the “fast Fourier transform,” which exploits the fact that an induction in n requires only about log N steps to go from $N = 1$ to $N = 2 ^ { n }$ . This yields a substantial saving in time in practical applications. 

In the second part of the chapter we undertake the more general theory of Fourier analysis on finite abelian groups. Here the fundamental example is the multiplicative group $\mathbb { Z } ^ { \ast } ( q )$ . The Fourier inversion formula 

## 1. Fourier analysis on Z(N)

for $\mathbb { Z } ^ { \ast } ( q )$ will be seen to be a key step in the proof of Dirichlet’s theorem on primes in arithmetic progression, which we will take up in the next chapter. 

## 1 Fourier analysis on $\mathbb { Z } ( N )$

We turn to the group of $N ^ { \mathrm { t h } }$ roots of unity. This group arises naturally as the simplest finite abelian group. It also gives a uniform partition of the circle, and is therefore a good choice if one wishes to sample appropriate functions on the circle. Moreover, this partition gets finer as N tends to infinity, and one might expect that the discrete Fourier theory that we discuss here tends to the continuous theory of Fourier series on the circle. In a broad sense, this is the case, although this aspect of the problem is not one that we develop. 

## 1.1 The group $\mathbb { Z } ( N )$

Let N be a positive integer. A complex number z is an $N ^ { \mathrm { t h } }$ root of unity if $z ^ { N } = 1$ . The set of $N ^ { \mathrm { t h } }$ roots of unity is precisely 

$$
\left\{1, e ^ {2 \pi i / N}, e ^ {2 \pi i 2 / N}, \ldots , e ^ {2 \pi i (N - 1) / N} \right\}.
$$

Indeed, suppose that $z ^ { N } = 1$ with $z = r e ^ { i \theta }$ . Then we must have $r ^ { N } e ^ { i N \theta } =$ 1, and taking absolute values yields $r = 1$ . Therefore $e ^ { i N \theta } = 1$ , and this means that $N \theta = 2 \pi k$ where $k \in \mathbb { Z }$ . So if $\zeta = e ^ { 2 \pi i / N }$ we find that $\zeta ^ { k }$ exhausts all the $N ^ { \mathrm { t h } }$ roots of unity. However, notice that $\zeta ^ { N } = 1$ so if n and m difer by an integer multiple of $N$ , then $\zeta ^ { n } = \zeta ^ { m }$ . In fact, it is clear that 

$$
\zeta^ {n} = \zeta^ {m} \quad \text {   if   and   only   if   } \quad n - m \text {   is   divisible   by   } N.
$$

We denote the set of all $N ^ { \mathrm { t h } }$ roots of unity by $\mathbb { Z } ( N )$ . The fact that this set gives a uniform partition of the circle is clear from its definition. Note that the set $\mathbb { Z } ( N )$ satisfies the following properties: 

(i) If $z , w \in \mathbb { Z } ( N )$ , then $z w \in \mathbb { Z } ( N )$ and $z w = w z$ 

(ii) $1 \in \mathbb { Z } ( N )$ 

(iii) $\mathrm { I f } ~ z \in \mathbb { Z } ( N )$ , then $z ^ { - 1 } = 1 / z \in \mathbb { Z } ( N )$ and of course $z z ^ { - 1 } = 1$ 

As a result we can conclude that $\mathbb { Z } ( N )$ is an abelian group under complex multiplication. The appropriate definitions are set out in detail later in Section 2.1. 


Chapter 7. FINITE FOURIER ANALYSIS


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2ab5d4b2-da28-455b-b554-908156ef0c8e/71eb1aee2cf995ed8371f7c3c16bc7c283eb680ab8da77672d9452a60aa9b3a3.jpg)



Figure 1. The group of $N ^ { \mathrm { t h } }$ roots of unity when $N = 9$ and $N = 2 ^ { 6 } =$ 64


There is another way to visualize the group $\mathbb { Z } ( N )$ This consists of choosing the integer power of ζ that determines each root of unity. We observed above that this integer is not unique since $\zeta ^ { n } = \zeta ^ { m }$ whenever n and m difer by an integer multiple of N. Naturally, we might select the integer which satisfies $0 \leq n \leq N - 1$ . Although this choice is perfectly reasonable in terms of $\mathrm { ^ { 6 6 } s , ^ { 5 } }$ we ask what happens when we multiply roots of unity. Clearly, we must add the corresponding integers since $\zeta ^ { n } \zeta ^ { m } = \zeta ^ { n + m }$ but nothing guarantees that $0 \leq n + m \leq N - 1$ . In fact, if $\zeta ^ { n } \zeta ^ { m } = \zeta ^ { k }$ with $0 \leq k \leq N - 1$ , then n + m and k difer by an integer multiple of N. So, to find the integer in $[ 0 , N - 1 ]$ corresponding to the root of unity $\zeta ^ { n } \zeta ^ { m }$ , we see that after adding the integers n and m we must reduce modulo N, that is, find the unique integer $0 \leq k \leq N - 1$ so that $( n + m ) - k$ is an integer multiple of N. 

An equivalent approach is to associate to each root of unity ω the class of integers n so that $\zeta ^ { n } = \omega$ . Doing so for each root of unity we obtain a partition of the integers in N disjoint infinite classes. To add two of these classes, choose any integer in each one of them, say n and m, respectively, and define the sum of the classes to be the class which contains the integer $n + m$ 

We formalize the above notions. Two integers x and y are congruent modulo N if the diference $x - y$ is divisible by N, and we write $x \equiv y$ mod N. In other words, this means that x and y difer by an integer multiple of N. It is an easy exercise to check the following three properties: 

## 1. Fourier analysis on $\mathbb { Z } ( N )$

$x \equiv x$ mod N for all integers x. 

• If $x \equiv y$ mod $N ,$ then $y \equiv x$ mod $N .$ 

• If $x \equiv y$ mod N and $y \equiv z$ mod N, then $x \equiv z$ mod N. 

The above defines an equivalence relation on $\mathbb { Z } .$ Let $R ( x )$ denote the equivalence class, or residue class, of the integer x. Any integer of the form $x + k N$ with $k \in \mathbb { Z }$ is an element (or “representative”) of $R ( x )$ In fact, there are precisely N equivalence classes, and each class has a unique representative between 0 and $N - 1$ . We may now add equivalence classes by defining 

$$
R (x) + R (y) = R (x + y).
$$

This definition is of course independent of the representatives x and y because if $x ^ { \prime } \in R ( x )$ and $y ^ { \prime } \in R ( y )$ , then one checks easily that $x ^ { \prime } + y ^ { \prime } \in$ $R ( x + y )$ . This turns the set of equivalence classes into an abelian group called the group of integers modulo $N$ , which is sometimes denoted by $\mathbb { Z } / N \mathbb { Z }$ . The association 

$$
R (k) \longleftrightarrow e ^ {2 \pi i k / N}
$$

gives a correspondence between the two abelian groups, $\mathbb { Z } / N \mathbb { Z }$ and $\mathbb { Z } ( N )$ Since the operations are respected, in the sense that addition of integers modulo N becomes multiplication of complex numbers, we shall also denote the group of integers modulo N by $\mathbb { Z } ( N )$ . Observe that $0 \in \mathbb { Z } / N \mathbb { Z }$ corresponds to 1 on the unit circle. 

Let V and $W$ denote the vector spaces of complex-valued functions on the group of integers modulo $N$ and the $N ^ { \mathrm { t h } }$ roots of unity, respectively. Then, the identification given above carries over to V and $W$ as follows: 

$$
F (k) \longleftrightarrow f (e ^ {2 \pi i k / N}),
$$

where F is a function on the integers modulo N and $f$ is a function on the $N ^ { \mathrm { t h } }$ roots of unity. 

From now on, we write $\mathbb { Z } ( N )$ but think of either the group of integers modulo N or the group of $N ^ { \mathrm { t h } }$ roots of unity. 

## 1.2 Fourier inversion theorem and Plancherel identity on $\mathbb { Z } ( N )$

The first and most crucial step in developing Fourier analysis on $\mathbb { Z } ( N )$ is to find the functions which correspond to the exponentials $e _ { n } ( x ) = e ^ { 2 }$ πinx in the case of the circle. Some important properties of these exponentials are: 

(i) $\{ e _ { n } \} _ { n \in \mathbb { Z } }$ is an orthonormal set for the inner product (1) (in Chapter 3) on the space of Riemann integrable functions on the circle. 

(ii) Finite linear combinations of the $e _ { n } \mathrm { { ' s } }$ (the trigonometric polynomials) are dense in the space of continuous functions on the circle. 

(iii) $e _ { n } ( x + y ) = e _ { n } ( x ) e _ { n } ( y )$ 

On $\mathbb { Z } ( N )$ , the appropriate analogues are the N functions $e _ { 0 } , \ldots , e _ { N - 1 }$ defined by 

$$
e _ {\ell} (k) = \zeta^ {\ell k} = e ^ {2 \pi i \ell k / N} \quad \text { for } \ell = 0, \dots , N - 1 \text { and } k = 0, \dots , N - 1,
$$

where $\zeta = e ^ { 2 \pi i / N }$ . To understand the parallel with (i) and (ii), we can think of the complex-valued functions on $\mathbb { Z } ( N )$ as a vector space $V ,$ endowed with the Hermitian inner product 

$$
(F, G) = \sum_ {k = 0} ^ {N - 1} F (k) \overline {{G (k)}}
$$

and associated norm 

$$
\| F \| ^ {2} = \sum_ {k = 0} ^ {N - 1} | F (k) | ^ {2}.
$$

Lemma 1.1 The family $\{ e _ { 0 } , \ldots , e _ { N - 1 } \}$ is orthogonal. In fact, 

$$
(e _ {m}, e _ {\ell}) = \left\{ \begin{array}{l l} N & \text {if m = \ell ,} \\ 0 & \text {if m\neq\ell .} \end{array} \right.
$$

Proof. We have 

$$
(e _ {m}, e _ {\ell}) = \sum_ {k = 0} ^ {N - 1} \zeta^ {m k} \zeta^ {- \ell k} = \sum_ {k = 0} ^ {N - 1} \zeta^ {(m - \ell) k}.
$$

If $m = \ell ,$ each term in the sum is equal to 1, and the sum equals N. If m $\neq \ell ,$ then $q = \zeta ^ { m - \ell }$ is not equal to 1, and the usual formula 

$$
1 + q + q ^ {2} + \dots + q ^ {N - 1} = \frac {1 - q ^ {N}}{1 - q}
$$

shows that $( e _ { m } , e _ { \ell } ) = 0$ , because $\boldsymbol q ^ { N } = 1$ 

Since the N functions $e _ { 0 } , \ldots , e _ { N - 1 }$ are orthogonal, they must be linearly independent, and since the vector space V is N-dimensional, we 

## 1. Fourier analysis on $\mathbb { Z } ( N )$

conclude that $\{ e _ { 0 } , \ldots , e _ { N - 1 } \}$ is an orthogonal basis for V . Clearly, property (iii) also holds, that is, $e _ { \ell } ( k + m ) = e _ { \ell } ( k ) e _ { \ell } ( m )$ for all $\ell ,$ and all $k , m \in \mathbb { Z } ( N )$ . 

By the lemma each vector $e _ { \ell }$ has norm $\sqrt { N }$ , so if we define 

$$
e _ {\ell} ^ {*} = \frac {1}{\sqrt {N}} e _ {\ell},
$$

then $\{ e _ { 0 } ^ { * } , \ldots , e _ { N - 1 } ^ { * } \}$ is an orthonormal basis for $V .$ . Hence for any $F \in V$ we have 

$$
F = \sum_ {n = 0} ^ {N - 1} (F, e _ {n} ^ {*}) e _ {n} ^ {*} \quad \text { as   well   as } \quad \| F \| ^ {2} = \sum_ {n = 0} ^ {N - 1} | (F, e _ {n} ^ {*}) | ^ {2}.\tag{1}
$$

If we define the $n ^ { \mathrm { t h } }$ Fourier coeficient of $F$ by 

$$
a _ {n} = \frac {1}{N} \sum_ {k = 0} ^ {N - 1} F (k) e ^ {- 2 \pi i k n / N},
$$

the above observations give the following fundamental theorem which is the $\mathbb { Z } ( N )$ version of the Fourier inversion and the Parseval-Plancherel formulas. 

Theorem 1.2 If $F$ is a function on $\mathbb { Z } ( N )$ , then 

$$
F (k) = \sum_ {n = 0} ^ {N - 1} a _ {n} e ^ {2 \pi i n k / N}.
$$

Moreover, 

$$
\sum_ {n = 0} ^ {N - 1} | a _ {n} | ^ {2} = \frac {1}{N} \sum_ {k = 0} ^ {N - 1} | F (k) | ^ {2}.
$$

The proof follows directly from (1) once we observe that 

$$
a _ {n} = \frac {1}{N} (F, e _ {n}) = \frac {1}{\sqrt {N}} (F, e _ {n} ^ {*}).
$$

Remark. It is possible to recover the Fourier inversion on the circle for suficiently smooth functions (say $C ^ { 2 } )$ by letting $N \to \infty$ in the finite model $\mathbb { Z } ( N )$ (see Exercise 3). 

## 1.3 The fast Fourier transform

The fast Fourier transform is a method that was developed as a means of calculating eficiently the Fourier coeficients of a function $F$ on $\mathbb { Z } ( N )$ 

The problem, which arises naturally in numerical analysis, is to determine an algorithm that minimizes the amount of time it takes a computer to calculate the Fourier coeficients of a given function on $\mathbb { Z } ( N )$ . Since this amount of time is roughly proportional to the number of operations the computer must perform, our problem becomes that of minimizing the number of operations necessary to obtain all the Fourier coeficients $\left\{ a _ { n } \right\}$ given the values of $F$ on $\mathbb { Z } ( N )$ . By operations we mean either an addition or a multiplication of complex numbers. 

We begin with a naive approach to the problem. Fix $N$ , and suppose that we are given $F ( 0 ) , \ldots , F ( N - 1 )$ and $\omega _ { N } = e ^ { - 2 \pi i / N }$ . If we denote by $a _ { k } ^ { N } ( F )$ the $k ^ { \mathrm { t h } }$ Fourier coeficient of $F$ on $\mathbb { Z } ( N )$ , then by definition 

$$
a _ {k} ^ {N} (F) = \frac {1}{N} \sum_ {r = 0} ^ {N - 1} F (r) \omega_ {N} ^ {k r},
$$

and crude estimates show that the number of operations needed to calculate all Fourier coeficients is $\leq 2 N ^ { 2 } + N$ . Indeed, it takes at most $N - 2$ multiplications to determine $\omega _ { N } ^ { 2 } , \dots , \omega _ { N } ^ { N - 1 }$ , and each coeficient $a _ { k } ^ { N }$ requires $N + 1$ multiplications and $N - 1$ additions. 

We now present the fast Fourier transform, an algorithm that improves the bound $O ( N ^ { 2 } )$ obtained above. Such an improvement is possible if, for example, we restrict ourselves to the case where the partition of the circle is dyadic, that is, $N = 2 ^ { n }$ . (See also Exercise 9.) 

Theorem 1.3 Given $\omega _ { N } = e ^ { - 2 \pi i / N }$ with $N = 2 ^ { n }$ , it is possible to calculate the Fourier coeficients of a function on $\mathbb { Z } ( N )$ with at most 

$$
4 \cdot 2 ^ {n} n = 4 N \log_ {2} (N) = O (N \log N)
$$

operations. 

The proof of the theorem consists of using the calculations for M division points, to obtain the Fourier coeficients for 2M division points. Since we choose $N = 2 ^ { n }$ , we obtain the desired formula as a consequence of a recurrence which involves $n = O ( \log N )$ steps. 

Let $\# ( M )$ denote the minimum number of operations needed to calculate all the Fourier coeficients of any function on $\mathbb { Z } ( M )$ . The key to the proof of the theorem is contained in the following recursion step. 

## 1. Fourier analysis on $\mathbb { Z } ( N )$

Lemma 1.4 If we are given $\omega _ { 2 M } = e ^ { - 2 \pi i / ( 2 M ) }$ , then 

$$
\# (2 M) \leq 2 \# (M) + 8 M.
$$

Proof. The calculation of $\omega _ { 2 M } , \dots , \omega _ { 2 M } ^ { 2 M }$ requires no more than 2M operations. Note that in particular we get $\omega _ { M } \bar { = } e ^ { - 2 \pi i / M } = \omega _ { 2 M } ^ { 2 }$ . The main idea is that for any given function $F$ on $\mathbb { Z } ( 2 M )$ , we consider two functions $F _ { 0 }$ and $F _ { 1 }$ on $\mathbb { Z } ( M )$ defined by 

$$
F _ {0} (r) = F (2 r) \quad \text { and } \quad F _ {1} (r) = F (2 r + 1).
$$

We assume that it is possible to calculate the Fourier coeficients of $F _ { 0 }$ and $F _ { 1 }$ in no more than $\# ( M )$ operations each. If we denote the Fourier coeficients corresponding to the groups $\mathbb { Z } ( 2 M )$ and $\mathbb { Z } ( M )$ by $a _ { k } ^ { 2 M }$ and $a _ { k } ^ { M }$ , respectively, then we have 

$$
a _ {k} ^ {2 M} (F) = \frac {1}{2} \left(a _ {k} ^ {M} (F _ {0}) + a _ {k} ^ {M} (F _ {1}) \omega_ {2 M} ^ {k}\right).
$$

To prove this, we sum over odd and even integers in the definition of the Fourier coeficient $a _ { k } ^ { 2 M } ( F )$ , and find 

$$
\begin{array}{l} a _ {k} ^ {2 M} (F) = \frac {1}{2 M} \sum_ {r = 0} ^ {2 M - 1} F (r) \omega_ {2 M} ^ {k r} \\ \qquad = \frac {1}{2} \left(\frac {1}{M} \sum_ {\ell = 0} ^ {M - 1} F (2 \ell) \omega_ {2 M} ^ {k (2 \ell)} + \frac {1}{M} \sum_ {m = 0} ^ {M - 1} F (2 m + 1) \omega_ {2 M} ^ {k (2 m + 1)}\right) \\ \qquad = \frac {1}{2} \left(\frac {1}{M} \sum_ {\ell = 0} ^ {M - 1} F _ {0} (\ell) \omega_ {M} ^ {k \ell} + \frac {1}{M} \sum_ {m = 0} ^ {M - 1} F _ {1} (m) \omega_ {M} ^ {k m} \omega_ {2 M} ^ {k}\right), \end{array}
$$

which establishes our assertion. 

As a result, knowing $a _ { k } ^ { M } ( F _ { 0 } ) , ~ a _ { k } ^ { M } ( F _ { 1 } )$ , and $\omega _ { 2 M } ^ { k }$ , we see that each $a _ { k } ^ { 2 M } ( F )$ can be computed using no more than three operations (one addition and two multiplications). So 

$$
\# (2 M) \leq 2 M + 2 \# (M) + 3 \times 2 M = 2 \# (M) + 8 M,
$$

and the proof of the lemma is complete. 

An induction on n, where $N = 2 ^ { n }$ , will conclude the proof of the theorem. The initial step $n = 1$ is easy, since $N = 2$ and the two Fourier coeficients are 

$$
a _ {0} ^ {N} (F) = \frac {1}{2} \left(F (1) + F (- 1)\right) \quad \mathrm{and} \quad a _ {1} ^ {N} (F) = \frac {1}{2} \left(F (1) + (- 1) F (- 1)\right).
$$

Calculating these Fourier coeficients requires no more than five operations, which is less than $4 \times 2 = 8$ . Suppose the theorem is true up to $N = 2 ^ { n - 1 }$ so that $\# ( N ) \leq 4 \cdot 2 ^ { n - 1 } ( n - 1 )$ . By the lemma we must have 

$$
\# (2 N) \leq 2 \cdot 4 \cdot 2 ^ {n - 1} (n - 1) + 8 \cdot 2 ^ {n - 1} = 4 \cdot 2 ^ {n} n,
$$

which concludes the inductive step and the proof of the theorem. 

## 2 Fourier analysis on finite abelian groups

The main goal in the rest of this chapter is to generalize the results about Fourier series expansions obtained in the special case of $\mathbb { Z } ( N )$ . 

After a brief introduction to some notions related to finite abelian groups, we turn to the important concept of a character. In our setting, we find that characters play the same role as the exponentials $e _ { 0 } , \ldots , e _ { N - 1 }$ on the group $\mathbb { Z } ( N )$ , and thus provide the key ingredient in the development of the theory on arbitrary finite abelian groups. In fact, it sufices to prove that a finite abelian group has “enough” characters, and this leads automatically to the desired Fourier theory. 

## 2.1 Abelian groups

An abelian group (or commutative group) is a set G together with a binary operation on pairs of elements of $G , ( a , b ) \mapsto a \cdot b .$ that satisfies the following conditions: 

(i) Associativity: $a \cdot ( b \cdot c ) = ( a \cdot b )$ · c for all $a , b , c \in G$ 

(ii) Identity: There exists an element $u \in G$ (often written as either 1 or 0) such that $a \cdot u = u \cdot a = a$ for all $a \in G$ 

(iii) Inverses: For every $a \in G ,$ there exists an element $a ^ { - 1 } \in G$ such that $\boldsymbol { a } \cdot \boldsymbol { a } ^ { - 1 } = \boldsymbol { a } ^ { - 1 } \cdot \boldsymbol { a } = \boldsymbol { u }$ 

(iv) Commutativity: For $a , b \in G$ , we have $a \cdot b = b \cdot a .$ 

We leave as simple verifications the facts that the identity element and inverses are unique. 

Warning. In the definition of an abelian group, we used the “multiplicative” notation for the operation in G. Sometimes, one uses the $^ { 6 6 } \mathrm { a d } .$ ditive” notation $a + b$ and $- a ,$ instead of $a \cdot b$ and $a ^ { - 1 }$ . There are times when one notation may be more appropriate than the other, and the examples below illustrate this point. The same group may have diferent interpretations, one where the multiplicative notation is more suggestive, and another where it is natural to view the group with addition, as the operation. 

## 2. Fourier analysis on finite abelian groups

## Examples of abelian groups

• The set of real numbers R with the usual addition. The identity is 0 and the inverse of x is −x. 

Also, $\mathbb { R } - \{ 0 \}$ and $\mathbb { R } ^ { + } = \{ x \in \mathbb { R } : x > 0 \}$ equipped, with the standard multiplication, are abelian groups. In both cases the unit is 1 and the inverse of x is $1 / x .$ 

• With the usual addition, the set of integers $\mathbb { Z }$ is an abelian group. However, $\mathbb { Z } - \{ 0 \}$ is not an abelian group with the standard multiplication, since, for example, 2 does not have a multiplicative inverse in $\mathbb { Z } .$ . In contrast, $\mathbb { Q } - \{ 0 \}$ is an abelian group with the standard multiplication. 

• The unit circle $S ^ { 1 }$ in the complex plane. If we view the circle as the set of points $\{ e ^ { i \theta } : \theta \in \mathbb { R } \}$ , the group operation is the standard multiplication of complex numbers. However, if we identify points on $S ^ { 1 }$ with their angle $\theta ,$ then $S ^ { 1 }$ becomes R modulo $2 \pi$ , where the operation is addition modulo $2 \pi$ 

$\mathbb { Z } ( N )$ is an abelian group. Viewed as the $N ^ { \mathrm { t h } }$ roots of unity on the circle, $\mathbb { Z } ( N )$ is a group under multiplication of complex numbers. However, if $\mathbb { Z } ( N )$ is interpreted as $\mathbb { Z } / N \mathbb { Z }$ , the integers modulo N, then it is an abelian group where the operation is addition modulo $N$ 

• The last example consists of $\mathbb { Z } ^ { \ast } ( q )$ . This group is defined as the set of all integers modulo q that have multiplicative inverses, with the group operation being multiplication modulo $q .$ This important example is discussed in more detail below. 

A homomorphism between two abelian groups G and H is a map $f : G \to H$ which satisfies the property 

$$
f (a \cdot b) = f (a) \cdot f (b),
$$

where the dot on the left-hand side is the operation in $G ,$ and the dot on the right-hand side the operation in $H$ 

We say that two groups G and H are isomorphic, and write $G \approx H$ if there is a bijective homomorphism from G to $H .$ . Equivalently, G and H are isomorphic if there exists another homomorphism ${ \tilde { f } } : H \to G ,$ so that for all $a \in G$ and $b \in H$ 

$$
(\tilde {f} \circ f) (a) = a \quad \text { and } \quad (f \circ \tilde {f}) (b) = b.
$$

Roughly speaking, isomorphic groups describe the “same” object because they have the same underlying group structure (which is really all that matters); however, their particular notational representations might be diferent. 

Example 1. A pair of isomorphic abelian groups arose already when we considered the group $\mathbb { Z } ( N )$ . In one representation it was given as the multiplicative group of $N ^ { \mathrm { t h } }$ roots of unity in C. In a second representation it was the additive group $\mathbb { Z } / N \mathbb { Z }$ of residue classes of integers modulo $N$ . The mapping $n \mapsto R ( n )$ , which associates to a root of unity $z = e ^ { 2 \pi i n / N } = \zeta ^ { n }$ the residue class in $\mathbb { Z } / N \mathbb { Z }$ determined by n, provides an isomorphism between the two diferent representations. 

Example 2. In parallel with the previous example, we see that the circle (with multiplication) is isomorphic to the real numbers modulo $2 \pi$ (with addition). 

Example 3. The properties of the exponential and logarithm guarantee that 

$$
\exp : \mathbb {R} \to \mathbb {R} ^ {+} \quad \mathrm{and} \quad \log : \mathbb {R} ^ {+} \to \mathbb {R}
$$

are two homomorphisms that are inverses of each other. Thus R (with addition) and $\mathbb { R } ^ { + }$ (with multiplication) are isomorphic. 

In what follows, we are primarily interested in abelian groups that are finite. In this case, we denote by |G| the number of elements in $G ,$ and call |G| the order of the group. For example, the order of $\mathbb { Z } ( N )$ is N. 

A few additional remarks are in order: 

• If $G _ { 1 }$ and $G _ { 2 }$ are two finite abelian groups, their direct product $G _ { 1 } \times G _ { 2 }$ is the group whose elements are pairs $\left( g _ { 1 } , g _ { 2 } \right)$ with $g _ { 1 } \in G _ { 1 }$ and $g _ { 2 } \in G _ { 2 }$ . The operation in $G _ { 1 } \times G _ { 2 }$ is then defined by 

$$
(g _ {1}, g _ {2}) \cdot (g _ {1} ^ {\prime}, g _ {2} ^ {\prime}) = (g _ {1} \cdot g _ {1} ^ {\prime}, g _ {2} \cdot g _ {2} ^ {\prime}).
$$

Clearly, if $G _ { 1 }$ and $G _ { 2 }$ are finite abelian groups, then so is $G _ { 1 } \times G _ { 2 }$ The definition of direct product generalizes immediately to the case of finitely many factors $G _ { 1 } \times G _ { 2 } \times \cdot \cdot \cdot \times G _ { n }$ 

• The structure theorem for finite abelian groups states that such a group is isomorphic to a direct product of groups of the type $\mathbb { Z } ( N )$ see Problem 2. This is a nice result which gives us an overview of the class of all finite abelian groups. However, since we shall not use this theorem below, we omit its proof. 

## 2. Fourier analysis on finite abelian groups

We now discuss briefly the examples of abelian groups that play a central role in the proof of Dirichlet’s theorem in the next chapter. 

## The group $\mathbb { Z } ^ { \ast } ( q )$

Let $q$ be a positive integer. We see that multiplication in $\mathbb { Z } ( q )$ can be unambiguously defined, because if n is congruent to $n ^ { \prime }$ and m is congruent to $m ^ { \prime }$ (both modulo $q )$ , then nm is congruent to $n ^ { \prime } m ^ { \prime }$ modulo $q . \mathrm { ~ \ A r ~ }$ n integer $n \in \mathbb { Z } ( q )$ is a unit if there exists an integer $m \in \mathbb { Z } ( q )$ so that 

$$
n m \equiv 1 \mod q.
$$

The set of all units in $\mathbb { Z } ( q )$ is denoted by $\mathbb { Z } ^ { \ast } ( q )$ , and it is clear from our definition that $\mathbb { Z } ^ { \ast } ( q )$ is an abelian group under multiplication modulo $q .$ Thus within the additive group $\mathbb { Z } ( q )$ lies a set $\mathbb { Z } ^ { \ast } ( q )$ that is a group under multiplication. An alternative characterization of $\mathbb { Z } ^ { \ast } ( q )$ will be given in the next chapter, as those elements in $\mathbb { Z } ( q )$ that are relatively prime to $q .$ 

Example 4. The group of units in $\mathbb { Z } ( 4 ) = \{ 0 , 1 , 2 , 3 \}$ is 

$$
\mathbb {Z} ^ {*} (4) = \{1, 3 \}.
$$

This reflects the fact that odd integers are divided into two classes depending on whether they are of the form $4 k + 1$ or $4 k + 3$ . In fact, $\mathbb { Z } ^ { \ast } ( 4 )$ is isomorphic to $\mathbb { Z } ( 2 )$ . Indeed, we can make the following association: 

$$
\begin{array}{c c c} \mathbb {Z} ^ {*} (4) & & \mathbb {Z} (2) \\ 1 & \longleftrightarrow & 0 \\ 3 & \longleftrightarrow & 1 \end{array}
$$

and then notice that multiplication in $\mathbb { Z } ^ { \ast } ( 4 )$ corresponds to addition in $\mathbb { Z } ( 2 )$ 

Example 5. The units in $\mathbb { Z } ( 5 )$ are 

$$
\mathbb {Z} ^ {*} (5) = \{1, 2, 3, 4 \}.
$$

Moreover, $\mathbb { Z } ^ { \ast } ( 5 )$ is isomorphic to $\mathbb { Z } ( 4 )$ with the following identification: 

$$
\begin{array}{c c c} \mathbb {Z} ^ {*} (5) & & \mathbb {Z} (4) \\ 1 & \longleftrightarrow & 0 \\ 2 & \longleftrightarrow & 1 \\ 3 & \longleftrightarrow & 3 \\ 4 & \longleftrightarrow & 2 \end{array}
$$

Example 6. The units in $\mathbb { Z } ( 8 ) = \{ 0 , 1 , 2 , 3 , 4 , 5 , 6 , 7 \}$ are given by 

$$
\mathbb {Z} ^ {*} (8) = \{1, 3, 5, 7 \}.
$$

In fact, $\mathbb { Z } ^ { \ast } ( 8 )$ is isomorphic to the direct product $\mathbb { Z } ( 2 ) \times \mathbb { Z } ( 2 )$ . In this case, an isomorphism between the groups is given by the identification 

<table><tr><td><eq>\mathbb{Z}^{*}(8)</eq></td><td></td><td><eq>\mathbb{Z}(2) \times \mathbb{Z}(2)</eq></td></tr><tr><td>1</td><td><eq>\longleftrightarrow</eq></td><td><eq>(0,0)</eq></td></tr><tr><td>3</td><td><eq>\longleftrightarrow</eq></td><td><eq>(1,0)</eq></td></tr><tr><td>5</td><td><eq>\longleftrightarrow</eq></td><td><eq>(0,1)</eq></td></tr><tr><td>7</td><td><eq>\longleftrightarrow</eq></td><td><eq>(1,1)</eq></td></tr></table>

## 2.2 Characters

Let G be a finite abelian group (with the multiplicative notation) and $S ^ { 1 }$ the unit circle in the complex plane. A character on G is a complexvalued function $e : G \to S ^ { 1 }$ which satisfies the following condition: 

$$
e (a \cdot b) = e (a) e (b) \quad \text { for   all } a, b \in G.\tag{2}
$$

In other words, a character is a homomorphism from G to the circle group. The trivial or unit character is defined by $e ( a ) = 1$ for all $a \in G$ 

Characters play an important role in the context of finite Fourier series, primarily because the multiplicative property (2) generalizes the analogous identity for the exponential functions on the circle and the law 

$$
e _ {\ell} (k + m) = e _ {\ell} (k) e _ {\ell} (m),
$$

which held for the exponentials $e _ { 0 } , \ldots , e _ { N - 1 }$ used in the Fourier theory on $\mathbb { Z } ( N )$ . There we had $\begin{array} { r } { e _ { \ell } ( k ) = \zeta ^ { \ell k } = e ^ { 2 \pi i \ell k / N } } \end{array}$ , with $0 \leq \ell \leq N - 1$ and $k \in \mathbb { Z } ( N )$ , and in fact, the functions $e _ { 0 } , \ldots , e _ { N - 1 }$ are precisely all the characters of the group $\mathbb { Z } ( N )$ 

If G is a finite abelian group, we denote by $\hat { G }$ the set of all characters of $G ,$ and observe next that this set inherits the structure of an abelian group. 

Lemma 2.1 The set $\hat { G }$ is an abelian group under multiplication defined $b y$ 

$$
(e _ {1} \cdot e _ {2}) (a) = e _ {1} (a) e _ {2} (a) \quad f o r a l l a \in G.
$$

The proof of this assertion is straightforward if one observes that the trivial character plays the role of the unit. We call $\hat { G }$ the dual group of $G .$ . 

In light of the above analogy between characters for a general abelian group and the exponentials on $\mathbb { Z } ( N )$ , we gather several more examples of groups and their duals. This provides further evidence of the central role played by characters. (See Exercises 4, 5, and 6.) 

Example 1. If $G = \mathbb { Z } ( N )$ , all characters of G take the form $\begin{array} { r } { e _ { \ell } ( k ) = \zeta ^ { \ell k } = } \end{array}$ $e ^ { 2 \pi i \ell k / N }$ for some $0 \leq \ell \leq N - 1$ , and it is easy to check that $e \ell \mapsto \ell$ gives an isomorphism from $\widehat { \mathbb { Z } ( N ) }$ to $\mathbb { Z } ( N )$ 

Example 2. The dual group of the circle<sup>1</sup> is precisely $\{ e _ { n } \} _ { n \in \mathbb { Z } }$ (where $e _ { n } ( x ) = e ^ { 2 \pi i n x } )$ . Moreover, $e _ { n } \mapsto n$ gives an isomorphism between $\widehat { S ^ { 1 } }$ and the integers Z. 

Example 3. Characters on R are described by 

$$
e _ {\xi} (x) = e ^ {2 \pi i \xi x} \quad \text { where } \xi \in \mathbb {R}.
$$

Thus $e _ { \xi } \mapsto \xi$ is an isomorphism from $\widehat { \mathbb R }$ to R. 

Example 4. Since exp : $\mathbb { R } \to \mathbb { R } ^ { + }$ is an isomorphism, we deduce from the previous example that the characters on $\mathbb { R } ^ { + }$ are given by 

$$
e _ {\xi} (x) = x ^ {2 \pi i \xi} = e ^ {2 \pi i \xi \log x} \quad \text { where } \xi \in \mathbb {R},
$$

and $\widehat { \mathbb { R } ^ { + } }$ is isomorphic to $\mathbb { R } \ ( \mathrm { o r } \ \mathbb { R } ^ { + } )$ 

The following lemma says that a nowhere vanishing multiplicative function is a character, a result that will be useful later. 

Lemma 2.2 Let G be a finite abelian group, and $e : G \to \mathbb { C } - \{ 0 \}$ a multiplicative function, namely $\boldsymbol { e } ( a \cdot b ) = \boldsymbol { e } ( a ) \boldsymbol { e } ( b )$ for all $a , b \in G$ . Then e is a character. 

Proof. The group G being finite, the absolute value of $e ( a )$ is bounded above and below as a ranges over $G$ . Since $| e ( b ^ { n } ) | = | e ( b ) | ^ { n }$ , we conclude that $| e ( b ) | = 1$ for all $b \in G$ 

The next step is to verify that the characters form an orthonormal basis of the vector space $V$ of functions over the group G. This fact was obtained directly in the special case $G = \mathbb { Z } ( N )$ from the explicit description of the characters $e _ { 0 } , \ldots , e _ { N - 1 } $ 

In the general case, we begin with the orthogonality relations; then we prove that there are “enough” characters by showing that there are as many as the order of the group. 

## 2.3 The orthogonality relations

Let V denote the vector space of complex-valued functions defined on the finite abelian group G. Note that the dimension of $V$ is $| G |$ , the order of G. We define a Hermitian inner product on V by 

$$
(f, g) = \frac {1}{| G |} \sum_ {a \in G} f (a) \overline {{g (a)}}, \quad \text { whenever } f, g \in V.\tag{3}
$$

Here the sum is taken over the group and is therefore finite. 

Theorem 2.3 The characters of G form an orthonormal family with respect to the inner product defined above. 

Since $| e ( a ) | = 1$ for any character, we find that 

$$
(e, e) = \frac {1}{| G |} \sum_ {a \in G} e (a) \overline {{e (a)}} = \frac {1}{| G |} \sum_ {a \in G} | e (a) | ^ {2} = 1.
$$

If $e \neq e ^ { \prime }$ and both are characters, we must prove that $( e , e ^ { \prime } ) = 0 ;$ we isolate the key step in a lemma. 

Lemma 2.4 If e is a non-trivial character of the group $G _ { i }$ , then $\textstyle \sum _ { a \in G } e ( a ) = 0$ 

Proof. Choose $b \in G$ such that $e ( b ) \neq 1$ . Then we have 

$$
e (b) \sum_ {a \in G} e (a) = \sum_ {a \in G} e (b) e (a) = \sum_ {a \in G} e (a b) = \sum_ {a \in G} e (a).
$$

The last equality follows because as a ranges over the group, ab ranges over G as well. Therefore $\textstyle \sum _ { a \in G } e ( a ) = 0$ 

## 2. Fourier analysis on finite abelian groups

We can now conclude the proof of the theorem. Suppose $e ^ { \prime }$ is a character distinct from e. Because $e ( e ^ { \prime } ) ^ { - 1 }$ is non-trivial, the lemma implies that 

$$
\sum_ {a \in G} e (a) (e ^ {\prime} (a)) ^ {- 1} = 0.
$$

Since $( e ^ { \prime } ( a ) ) ^ { - 1 } = { \overline { { e ^ { \prime } ( a ) } } }$ , the theorem is proved. 

As a consequence of the theorem, we see that distinct characters are linearly independent. Since the dimension of $V$ over $\mathbb { C }$ is |G|, we conclude that the order of $\hat { G }$ is finite and $\leq | G |$ |. The main result to which we now turn is that, in fact, $| { \hat { G } } | = | G |$ 

## 2.4 Characters as a total family

The following completes the analogy between characters and the complex exponentials. 

Theorem 2.5 The characters of a finite abelian group G form a basis for the vector space of functions on G. 

There are several proofs of this theorem. One consists of using the structure theorem for finite abelian groups we have mentioned earlier, which states that any such group is the direct product of cyclic groups, that is, groups of the type $\mathbb { Z } ( N )$ . Since cyclic groups are self-dual, using this fact we would conclude that $| \hat { G } | = | G |$ , and therefore the characters form a basis for G. (See Problem 3.) 

Here we shall prove the theorem directly without these considerations. 

Suppose V is a vector space of dimension d with inner product $( \cdot , \cdot )$ A linear transformation $T : V  V$ is unitary if it preserves the inner product, $( T v , T w ) = ( v , w )$ for all $v , w \in V$ . The spectral theorem from linear algebra asserts that any unitary transformation is diagonalizable. In other words, there exists a basis $\{ v _ { 1 } , \ldots , v _ { d } \}$ (eigenvectors) of $V$ such that $T ( v _ { i } ) = \lambda _ { i } v _ { i }$ , where $\lambda _ { i } \in \mathbb { C }$ is the eigenvalue attached to $v _ { i }$ 

The proof of Theorem 2.5 is based on the following extension of the spectral theorem. 

Lemma 2.6 Suppose $\{ T _ { 1 } , \dots , T _ { k } \}$ is a commuting family ofunitary transformations on the finite-dimensional inner product space $V ;$ that $i s ,$ 

$$
T _ {i} T _ {j} = T _ {j} T _ {i} \quad f o r a l l i, j.
$$

Then $T _ { 1 } , \ldots , T _ { k }$ are simultaneously diagonalizable. In other words, there exists a basis for V which consists of eigenvectors for every $T _ { i } , i = 1 , \ldots , k$ 

Proof. We use induction on k. The case $k = 1$ is simply the spectral theorem. Suppose that the lemma is true for any family of $k - 1$ commuting unitary transformations. The spectral theorem applied to $T _ { k }$ says that $V$ is the direct sum of its eigenspaces 

$$
V = V _ {\lambda_ {1}} \oplus \dots \oplus V _ {\lambda_ {s}},
$$

where $V _ { \lambda _ { i } }$ denotes the subspace of all eigenvectors with eigenvalue $\lambda _ { i }$ We claim that each one of the $T _ { 1 } , \ldots , T _ { k - 1 }$ maps each eigenspace $V _ { \lambda _ { i } }$ to itself. Indeed, if $v \in V _ { \lambda _ { i } }$ and $1 \leq j \leq k - 1$ , then 

$$
T _ {k} T _ {j} (v) = T _ {j} T _ {k} (v) = T _ {j} (\lambda_ {i} v) = \lambda_ {i} T _ {j} (v)
$$

so $T _ { j } ( v ) \in V _ { \lambda _ { i } }$ , and the claim is proved. 

Since the restrictions to $V _ { \lambda _ { i } }$ of $T _ { 1 } , \ldots , T _ { k - 1 }$ form a family of commuting unitary linear transformations, the induction hypothesis guarantees that these are simultaneously diagonalizable on each subspace $V _ { \lambda _ { i } }$ . This diagonalization provides us with the desired basis for each $V _ { \lambda _ { i } }$ , and thus for V. 

We can now prove Theorem 2.5. Recall that the vector space $V$ of complex-valued functions defined on G has dimension |G|. For each $a \in G$ we define a linear transformation $T _ { a } : V \to V$ by 

$$
(T _ {a} f) (x) = f (a \cdot x) \quad \text { for } x \in G.
$$

Since G is abelian it is clear that $T _ { a } T _ { b } = T _ { b } T _ { a }$ for all $a , b \in G$ , and one checks easily that $T _ { a }$ is unitary for the Hermitian inner product (3) defined on V. By Lemma 2.6 the family $\{ T _ { a } \} _ { a \in G }$ is simultaneously diagonalizable. This means there is a basis $\{ v _ { b } ( x ) \} _ { b \in G }$ for $V$ such that each $v _ { b } ( x )$ is an eigenfunction for $T _ { a }$ , for every a. Let v be one of these basis elements and 1 the unit element in G. We must have $v ( 1 ) \neq 0$ for otherwise 

$$
v (a) = v (a \cdot 1) = (T _ {a} v) (1) = \lambda_ {a} v (1) = 0,
$$

where $\lambda _ { a }$ is the eigenvalue of v for $T _ { a }$ . Hence $v = 0$ , and this is a contradiction. We claim that the function defined by $w ( x ) = \lambda _ { x } = v ( x ) / v ( 1 )$ is a character of G. Arguing as above we find that $w ( x ) \neq 0$ for every $x ,$ and 

$$
w (a \cdot b) = \frac {v (a \cdot b)}{v (1)} = \frac {\lambda_ {a} v (b)}{v (1)} = \lambda_ {a} \lambda_ {b} \frac {v (1)}{v (1)} = \lambda_ {a} \lambda_ {b} = w (a) w (b).
$$

We now invoke Lemma 2.2 to conclude the proof. 

2. Fourier analysis on finite abelian groups 

## 2.5 Fourier inversion and Plancherel formula

We now put together the results obtained in the previous sections to discuss the Fourier expansion of a function on a finite abelian group G. Given a function $f$ on G and character e of G, we define the Fourier coeficient of f with respect to e, by 

$$
\hat {f} (e) = (f, e) = \frac {1}{| G |} \sum_ {a \in G} f (a) \overline {{e (a)}},
$$

and the Fourier series of $f$ as 

$$
f \sim \sum_ {e \in \hat {G}} \hat {f} (e) e.
$$

Since the characters form a basis, we know that 

$$
f = \sum_ {e \in \hat {G}} c _ {e} e
$$

for some set of constants $c _ { e }$ . By the orthogonality relations satisfied by the characters, we find that 

$$
(f, e) = c _ {e},
$$

so f is indeed equal to its Fourier series, namely, 

$$
f = \sum_ {e \in \hat {G}} \hat {f} (e) e.
$$

We summarize our results. 

Theorem 2.7 Let G be a finite abelian group. The characters of G form an orthonormal basis for the vector space V of functions on G equipped with the inner product 

$$
(f, g) = \frac {1}{| G |} \sum_ {a \in G} f (a) \overline {{g (a)}}.
$$

In particular, any function f on G is equal to its Fourier series 

$$
f = \sum_ {e \in \hat {G}} \hat {f} (e) e.
$$

Finally, we have the Parseval-Plancherel formula for finite abelian groups. 

Theorem 2.8 If f is a function on $G ,$ then $\| f \| ^ { 2 } = \sum _ { e \in \hat { G } } | \hat { f } ( e ) | ^ { 2 }$ 

Proof. Since the characters of G form an orthonormal basis for the vector space $V ,$ and $( f , e ) = { \hat { f } } ( e )$ , we have that 

$$
\| f \| ^ {2} = (f, f) = \sum_ {e \in \hat {G}} (f, e) \overline {{\hat {f} (e)}} = \sum_ {e \in \hat {G}} | \hat {f} (e) | ^ {2}.
$$

The apparent diference of this statement with that of Theorem 1.2 is due to the diferent normalizations of the Fourier coeficients that are used. 

## 3 Exercises

1. Let f be a function on the circle. For each $N \geq 1$ the discrete Fourier coeficients of f are defined by 

$$
a _ {N} (n) = \frac {1}{N} \sum_ {k = 1} ^ {N} f (e ^ {2 \pi i k / N}) e ^ {- 2 \pi i k n / N}, \quad \text { for } n \in \mathbb {Z}.
$$

We also let 

$$
a (n) = \int_ {0} ^ {1} f (e ^ {2 \pi i x}) e ^ {- 2 \pi i n x} d x
$$

denote the ordinary Fourier coeficients of $f .$ 

(a) Show that $a _ { N } ( n ) = a _ { N } ( n + N )$ 

(b) Prove that if f is continuous, then $a _ { N } ( n ) \to a ( n )$ as $N \to \infty$ 

2. If $f$ is $\textbf { a } C ^ { 1 }$ function on the circle, prove that $| a _ { N } ( n ) | \leq c / | n |$ whenever $0 < | n | \leq N / 2$ 

[Hint: Write 

$$
a _ {N} (n) [ 1 - e ^ {2 \pi i \ell n / N} ] = \frac {1}{N} \sum_ {k = 1} ^ {N} [ f (e ^ {2 \pi i k / N}) - f (e ^ {2 \pi i (k + \ell) / N}) ] e ^ {- 2 \pi i k n / N},
$$

and choose ` so that $\ell n / N$ is nearly $1 / 2 . ]$ 

3. By a similar method, show that if $f$ is a $C ^ { 2 }$ function on the circle, then 

$$
\left| a _ {N} (n) \right| \leq c / | n | ^ {2}, \quad \text { whenever } 0 <   | n | \leq N / 2.
$$

## 3. Exercises

As a result, prove the inversion formula for $f \in C ^ { 2 }$ 

$$
f (e ^ {2 \pi i x}) = \sum_ {n = - \infty} ^ {\infty} a (n) e ^ {2 \pi i n x}
$$

from its finite version. 

[Hint: For the first part, use the second symmetric diference 

$$
f (e ^ {2 \pi i (k + \ell) / N}) + f (e ^ {2 \pi i (k - \ell) / N}) - 2 f (e ^ {2 \pi i k / N}).
$$

For the second part, if N is odd (say), write the inversion formula as 

$$
f (e ^ {2 \pi i k / N}) = \sum_ {| n | <   N / 2} a _ {N} (n) e ^ {2 \pi i k n / N}. ]
$$

4. Let e be a character on $G = \mathbb { Z } ( N )$ , the additive group of integers modulo $N .$ Show that there exists a unique $0 \leq \ell \leq N - 1$ so that 

$$
e (k) = e _ {\ell} (k) = e ^ {2 \pi i \ell k / N} \quad \text {   for   all   } k \in \mathbb {Z} (N).
$$

Conversely, every function of this type is a character on $\mathbb { Z } ( N )$ . Deduce that $e _ { \ell } \mapsto \ell$ defines an isomorphism from $\hat { G }$ to $G .$ 

[Hint: Show that e(1) is an $N ^ { \mathrm { t h } }$ root of unity.] 

5. Show that all characters on $S ^ { 1 }$ are given by 

$$
e _ {n} (x) = e ^ {2 \pi i n x} \quad \text { with } n \in \mathbb {Z},
$$

and check that $e _ { n } \mapsto n$ defines an isomorphism from $\widehat { S ^ { 1 } }$ to $\mathbb { Z } .$ 

[Hint: If F is continuous and $F ( x + y ) = F ( x ) F ( y )$ , then $F$ is diferentiable. To see this, note that if $F ( 0 ) \neq 0$ , then for appropriate $\begin{array} { r } { \delta , c = \int _ { 0 } ^ { \delta } F ( y ) d y \neq 0 } \end{array}$ , and $\begin{array} { r } { c F ( x ) = \int _ { x } ^ { \delta + x } F ( y ) d y } \end{array}$ . Diferentiate to conclude that $F ( x ) = e ^ { A x }$ for some $A . ]$ 

6. Prove that all characters on R take the form 

$$
e _ {\xi} (x) = e ^ {2 \pi i \xi x} \quad \text { with } \xi \in \mathbb {R},
$$

and that $e \xi \mapsto \xi$ defines an isomorphism from $\widehat { \mathbb { R } }$ to R. The argument in Exercise 5 applies here as well. 

7. Let $\zeta = e ^ { 2 \pi i / N }$ . Define the $N \times N$ matrix $M = ( a _ { j k } ) _ { 1 \leq j , k \leq N }$ by $a _ { j k } =$ $N ^ { - 1 / 2 } \zeta ^ { j k }$ 

(a) Show that M is unitary. 

(b) Interpret the identity $( M u , M v ) = ( u , v )$ and the fact that $M ^ { * } = M ^ { - 1 }$ in terms of Fourier series on $\mathbb { Z } ( N )$ 

8. Suppose that $P ( x ) = \sum _ { n = 1 } ^ { N } a _ { n } e ^ { 2 \pi i n x } .$ 

(a) Show by using the Parseval identities for the circle and $\mathbb { Z } ( N )$ , that 

$$
\int_ {0} ^ {1} | P (x) | ^ {2} d x = \frac {1}{N} \sum_ {j = 1} ^ {N} | P (j / N) | ^ {2}.
$$

(b) Prove the reconstruction formula 

$$
P (x) = \sum_ {j = 1} ^ {N} P (j / N) K (x - (j / N))
$$

where 

$$
K (x) = \frac {e ^ {2 \pi i x}}{N} \frac {1 - e ^ {2 \pi i N x}}{1 - e ^ {2 \pi i x}} = \frac {1}{N} (e ^ {2 \pi i x} + e ^ {2 \pi i 2 x} + \dots + e ^ {2 \pi i N x}).
$$

Observe that $P$ is completely determined by the values $P ( j / N )$ for $1 \leq j \leq N$ Note also that $K ( 0 ) = 1$ , and $K ( j / N ) = 0$ whenever $j$ is not congruent to 0 modulo $N$ 

9. To prove the following assertions, modify the argument given in the text. 

(a) Show that one can compute the Fourier coeficients of a function on $\mathbb { Z } ( N )$ when $N = 3 ^ { n }$ with at most $6 N \log _ { 3 } N$ operations. 

(b) Generalize this to $N = \alpha ^ { n }$ where α is an integer $> 1$ 

10. A group G is cyclic if there exists $g \in G$ that generates all of G, that is, if any element in G can be written as $g ^ { n }$ for some $n \in \mathbb { Z }$ . Prove that a finite abelian group is cyclic if and only if it is isomorphic to $\mathbb { Z } ( N )$ for some $N$ 

11. Write down the multiplicative tables for the groups $\mathbb { Z } ^ { \ast } ( 3 ) , \ \mathbb { Z } ^ { \ast } ( 4 ) , \ \mathbb { Z } ^ { \ast } ( 5 )$ ， $\mathbb { Z } ^ { \ast } ( 6 ) , \mathbb { Z } ^ { \ast } ( 8 )$ , and $\mathbb { Z } ^ { \ast } ( 9 )$ . Which of these groups are cyclic? 

12. Suppose that G is a finite abelian group and $e : G \to \mathbb { C }$ is a function that satisfies $e ( x \cdot y ) = e ( x ) e ( y )$ for all $x , y \in G$ . Prove that either e is identically $0 ,$ or e never vanishes. In the second case, show that for each $x , e ( x ) = e ^ { 2 \pi i r }$ for some $r \in \mathbb { Q }$ of the form $r = p / q$ , where $q = | G |$ 

## 4. Problems

13. In analogy with ordinary Fourier series, one may interpret finite Fourier expansions using convolutions as follows. Suppose $G$ is a finite abelian group, $1 _ { G }$ its unit, and V the vector space of complex-valued functions on $G .$ 

(a) The convolution of two functions f and $g$ in $V$ is defined for each $a \in G$ by 

$$
(f * g) (a) = \frac {1}{| G |} \sum_ {b \in G} f (b) g (a \cdot b ^ {- 1}).
$$

Show that for all $e \in { \hat { G } }$ one has $\widehat { ( f * g ) } ( e ) = \widehat { f } ( e ) \widehat { g } ( e )$ 

(b) Use Theorem 2.5 to show that if e is a character on $G ,$ then 

$$
\sum_ {e \in \hat {G}} e (c) = 0 \quad \text { whenever } c \in G \text { and } c \neq 1 _ {G}.
$$

(c) As a result of (b), show that the Fourier series $\begin{array} { r } { S f ( \boldsymbol { a } ) = \sum _ { e \in \hat { G } } \hat { f } ( e ) e ( \boldsymbol { a } ) } \end{array}$ of a function $f \in V$ takes the form 

$$
S f = f * D,
$$

where D is defined by 

$$
D (c) = \sum_ {e \in \hat {G}} e (c) = \left\{ \begin{array}{c l} | G | & \text {if} c = 1 _ {G}, \\ 0 & \text {otherwise.} \end{array} \right.\tag{4}
$$

Since $f * D = f ,$ we recover the fact that $S f = f .$ Loosely speaking, D corresponds to a “Dirac delta function”; it has unit mass 

$$
\frac {1}{| G |} \sum_ {c \in G} D (c) = 1,
$$

and (4) says that this mass is concentrated at the unit element in $G .$ Thus D has the same interpretation as the “limit” of a family of good kernels. (See Section 4, Chapter 2.) 

Note. The function D reappears in the next chapter as $\delta _ { 1 } ( n )$ 

## 4 Problems

1. Prove that if n and m are two positive integers that are relatively prime, then 

$$
\mathbb {Z} (n m) \approx \mathbb {Z} (n) \times \mathbb {Z} (m).
$$

[Hint: Consider the map $\mathbb { Z } ( n m ) \to \mathbb { Z } ( n ) \times \mathbb { Z } ( m )$ given by $k \mapsto ( k$ mod $n ,$ k mod $m )$ , and use the fact that there exist integers x and y such that $x n + y m = 1 . ]$ 

$\mathbf { 2 . ^ { * } }$ Every finite abelian group $G$ is isomorphic to a direct product of cyclic groups. Here are two more precise formulations of this theorem. 

• If $p _ { 1 } , \ldots , p _ { s }$ are the distinct primes appearing in the factorization of the order of $G ,$ then 

$$
G \approx G (p _ {1}) \times \dots \times G (p _ {s}),
$$

where each $G ( p )$ is of the form $G ( p ) = \mathbb { Z } ( p ^ { r _ { 1 } } ) \times \cdot \cdot \cdot \times \mathbb { Z } ( p ^ { r _ { \ell } } )$ , with $0 \leq$ $r _ { 1 } \le \cdots \le r _ { \ell }$ (this sequence of integers depends on p of course). This decomposition is unique. 

• There exist unique integers $d _ { 1 } , \ldots , d _ { k }$ such that 

$$
d _ {1} | d _ {2}, d _ {2} | d _ {3}, \dots , d _ {k - 1} | d _ {k}
$$

and 

$$
G \approx \mathbb {Z} (d _ {1}) \times \dots \times \mathbb {Z} (d _ {k}).
$$

Deduce the second formulation from the first. 

3. Let $\hat { G }$ denote the collection of distinct characters of the finite abelian group G. 

(a) Note that ${ \mathrm { i f ~ } } G = \mathbb { Z } ( N )$ , then $\hat { G }$ is isomorphic to $G .$ 

(b) Prove that $\widehat { G _ { 1 } \times G _ { 2 } } = \hat { G } _ { 1 } \times \hat { G } _ { 2 }$ 

(c) Prove using Problem 2 that if G is a finite abelian group, then $\hat { G }$ is isomorphic to G. 

4.<sup>∗</sup> When $p$ is prime the group $\mathbb { Z } ^ { \ast } ( p )$ is cyclic, and $\mathbb { Z } ^ { * } ( p ) \approx \mathbb { Z } ( p - 1 )$ . 

# 8 <sub>Dirichlet’s</sub> <sub>Theorem</sub>

Dirichlet, Gustav Lejeune (D¨uren 1805-G¨ottingen 1859), German mathematician. He was a number theorist at heart. But, while studying in Paris, being a very likeable person, he was befriended by Fourier and other like-minded mathematicians, and he learned analysis from them. Thus equipped, he was able to lay the foundation for the application of Fourier analysis to (analytic) theory of numbers. 

S. Bochner, 1966 

As a striking application of the theory of finite Fourier series, we now prove Dirichlet’s theorem on primes in arithmetic progression. This theorem states that if $q$ and ` are positive integers with no common factor, then the progression 

$$
\ell , \ell + q, \ell + 2 q, \ell + 3 q, \ldots , \ell + k q, \ldots
$$

contains infinitely many prime numbers. This change of subject matter that we undertake illustrates the wide applicability of ideas from Fourier analysis to various areas outside its seemingly narrower confines. In this particular case, it is the theory of Fourier series on the finite abelian group $\mathbb { Z } ^ { \ast } ( q )$ that plays a key role in the solution of the problem. 

## 1 A little elementary number theory

We begin by introducing the requisite background. This involves elementary ideas of divisibility of integers, and in particular properties regarding prime numbers. Here the basic fact, called the fundamental theorem of arithmetic, is that every integer is the product of primes in an essentially unique way. 

## 1.1 The fundamental theorem of arithmetic

The following theorem is a mathematical formulation of long division. 

Theorem 1.1 (Euclid’s algorithm) For any integers a and b with $b > 0$ , there exist unique integers $q$ and r with $0 \leq r < b$ such that 

$$
a = q b + r.
$$

Here $q$ denotes the quotient of a by $b ,$ and $r$ is the remainder, which is smaller than b. 

Proof. First we prove the existence of $q$ and $r .$ Let $S$ denote the set of all non-negative integers of the form $a - q b$ with $q \in \mathbb { Z }$ . This set is non-empty and in fact $S$ contains arbitrarily large positive integers since $b \neq 0$ . Let $r$ denote the smallest element in $S ,$ so that 

$$
r = a - q b
$$

for some integer q. $\mathrm { B y }$ construction $0 \leq r ,$ , and we claim that $r < b$ . If not, we may write $r = b + s$ with $0 \leq s < r ,$ so $b + s = a - q b$ , which then implies 

$$
s = a - (q + 1) b.
$$

Hence $s \in S$ with $s < r$ , and this contradicts the minimality of $r .$ So $r < b ,$ , hence $q$ and r satisfy the conditions of the theorem. 

To prove uniqueness, suppose we also had $a = q _ { 1 } b + r _ { 1 }$ where $0 \leq r _ { 1 } < b$ . By subtraction we find 

$$
(q - q _ {1}) b = r _ {1} - r.
$$

The left-hand side has absolute value 0 or $\geq b ,$ , while the right-hand side has absolute value $< b .$ Hence both sides of the equation must be $0 ,$ which gives $q = q _ { 1 }$ and $r = r _ { 1 }$ 

An integer a divides b if there exists another integer c such that $a c = b ;$ we then write $a | b$ and say that a is a divisor of $b .$ Note that in particular 1 divides every integer, and a|a for all integers a. A prime number is a positive integer greater than 1 that has no positive divisors besides 1 and itself. The main theorem in this section says that any positive integer can be written uniquely as the product of prime numbers. 

The greatest common divisor of two positive integers a and b is the largest integer that divides both a and b. We usually denote the greatest common divisor by $\operatorname { g c d } ( a , b )$ . Two positive integers are relatively prime if their greatest common divisor is 1. In other words, 1 is the only positive divisor common to both a and b. 

## 1. A little elementary number theory

Theorem 1.2 If $\operatorname* { g c d } ( a , b ) = d ;$ , then there exist integers x and $y$ such that 

$$
a x + b y = d.
$$

Proof. Consider the set S of all positive integers of the form $a x + b y$ where $x , y \in \mathbb { Z }$ , and let s be the smallest element in S. We claim that $s =$ d. By construction, there exist integers x and y such that 

$$
a x + b y = s.
$$

Clearly, any divisor of a and b divides s, so we must have $d \leq s$ . The proof will be complete if we can show that s|a and s|b. By Euclid’s algorithm, we can write $a = q s + r$ with $0 \leq r < s$ . Multiplying the above by q we find $q a x + q b y = q s$ , and therefore 

$$
q a x + q b y = a - r.
$$

Hence $r = a ( 1 - q x ) + b ( - q y )$ . Since s was minimal in S and $0 \leq r < s .$ we conclude that $r = 0 .$ , therefore s divides a. A similar argument shows that s divides b, hence $s = d$ as desired. 

In particular we record the following three consequences of the theorem. 

Corollary 1.3 Two positive integers a and b are relatively prime $i f$ and only if there exist integers x and y such that $a x + b y = 1$ 

Proof. If a and b are relatively prime, two integers x and y with the desired property exist by Theorem 1.2. Conversely, if $a x + b y = 1$ holds and d is positive and divides both a and $b ,$ then d divides 1, hence $d = 1$ 

Corollary 1.4 If a and c are relatively prime and c divides ab, then c divides b. In particular, if p is a prime that does not divide a and p divides ab, then p divides b. 

Proof. We can write $1 = a x + c y .$ , so multiplying by b we find $b =$ $a b x + c b y$ . Hence $c | b$ 

Corollary 1.5 If p is prime and p divides the product $a _ { 1 } \cdots a _ { r }$ , then $p$ divides $a _ { i }$ for some i. 

Proof. By the previous corollary, if $p$ does not divide $a _ { 1 } .$ , then $p$ divides $a _ { 2 } \cdots a _ { r } ,$ so eventually $p | a _ { i }$ 

We can now prove the main result of this section. 

Theorem 1.6 Every positive integer greater than 1 can be factored uniquely into a product of primes. 

Proof. First, we show that such a factorization is possible. We do so by proving that the set S of positive integers $> 1$ which do not have a factorization into primes is empty. Arguing by contradiction, we assume that $S \neq \emptyset .$ . Let n be the smallest element of S. Since n cannot be a prime, there exist integers $a > 1$ and $b > 1$ such that $a b = n$ . But then $a < n$ and $b < n ,$ so a $\notin S$ as well as $b \notin S$ . Hence both a and b have prime factorizations and so does their product $n .$ This implies n $\notin S ,$ , therefore S is empty, as desired. 

We now turn our attention to the uniqueness of the factorization. Suppose that n has two factorizations into primes 

$$
\begin{array}{r} n = p _ {1} p _ {2} \dots p _ {r} \\ = q _ {1} q _ {2} \dots q _ {s}. \end{array}
$$

So $p _ { 1 }$ divides $q _ { 1 } q _ { 2 } \cdots q _ { s }$ , and we can apply Corollary 1.5 to conclude that $p _ { 1 } | q _ { i }$ for some i. Since $q _ { i }$ is prime, we must have $p _ { 1 } = q _ { i }$ . Continuing with this argument we find that the two factorizations of n are equal up to a permutation of the factors. 

We briefly digress to give an alternate definition of the group $\mathbb { Z } ^ { \ast } ( q )$ which appeared in the previous chapter. According to our initial definition, $\mathbb { Z } ^ { \ast } ( q )$ is the multiplicative group of units in $\mathbb { Z } ( q )$ : those $n \in \mathbb { Z } ( q )$ for which there exists an integer m so that 

$$
n m \equiv 1 \mod q.\tag{1}
$$

Equivalently, $\mathbb { Z } ^ { \ast } ( q )$ is the group under multiplication of all integers in $\mathbb { Z } ( q )$ that are relatively prime to $q .$ Indeed, notice that if (1) is satisfied, then automatically n and $q$ are relatively prime. Conversely, suppose we assume that n and $q$ are relatively prime. Then, if we put $a = n$ and $b = q$ in Corollary 1.3, we find 

$$
n x + q y = 1.
$$

Hence $n x \equiv 1$ mod $q ,$ and we can take $m = x$ to establish the equivalence. 

## 1.2 The infinitude of primes

The study of prime numbers has always been a central topic in arithmetic, and the first fundamental problem that arose was to determine whether 

## 1. A little elementary number theory

there are infinitely many primes or not. This problem was solved in Euclid’s Elements with a simple and very elegant argument. 

Theorem 1.7 There are infinitely many primes. 

Proof. Suppose not, and denote by $p _ { 1 } , \ldots , p _ { n }$ the complete set of primes. Define 

$$
N = p _ {1} p _ {2} \cdot \cdot \cdot p _ {n} + 1.
$$

Since N is larger than any $p _ { i }$ , the integer $N$ cannot be prime. Therefore, N is divisible by a prime that belongs to our list. But this is also an absurdity since every prime divides the product, yet no prime divides 1. This contradiction concludes the proof. 

Euclid’s argument actually can be modified to deduce finer results about the infinitude of primes. To see this, consider the following problem. Prime numbers (except for 2) can be divided into two classes depending on whether they are of the form $4 k + 1$ or $4 k + 3$ , and the above theorem says that at least one of these classes has to be infinite. A natural question is to ask whether both classes are infinite, and if not, which one is? In the case of primes of the form $4 k + 3$ , the fact that the class is infinite has a proof that is similar to Euclid’s, but with a twist. If there are only finitely many such primes, enumerate them in increasing order omitting 3, 

$$
p _ {1} = 7, p _ {2} = 1 1, \ldots , p _ {n},
$$

and let 

$$
N = 4 p _ {1} p _ {2} \cdot \cdot \cdot p _ {n} + 3.
$$

Clearly, N is of the form $4 k + 3$ and cannot be prime since $N > p _ { n }$ Since the product of two numbers of the form 4m + 1 is again of the form $4 m + 1$ , one of the prime divisors of N, say $p ,$ must be of the form $4 k + 3$ . We must have $p \neq 3 ,$ , since 3 does not divide the product in the definition of N. Also, p cannot be one of the other primes of the form $4 k + 3$ , that is, $p \neq p _ { i }$ for $i = 1 , \dots n$ , because then $p$ divides the product $p _ { 1 } \cdots p _ { n }$ but does not divide 3. 

It remains to determine if the class of primes of the form $4 k + 1$ is infinite. A simple-minded modification of the above argument does not work since the product of two numbers of the form $4 m + 3$ is never of the form 4m + 3. More generally, in an attempt to prove the law of quadratic reciprocity, Legendre formulated the following statement: 

If $q$ and ` are relatively prime, then the sequence 

$$
\ell + k q, \quad k \in \mathbb {Z}
$$

contains infinitely many primes (hence at least one prime!). 

Of course, the condition that q and ` be relatively prime is necessary, for otherwise $\ell + k q$ is never prime. In other words, this hypothesis says that any arithmetic progression that could contain primes necessarily contains infinitely many of them. 

Legendre’s assertion was proved by Dirichlet. The key idea in his proof is Euler’s analytical approach to prime numbers involving his product formula, which gives a strengthened version of Theorem 1.7. This insight of Euler led to a deep connection between the theory of primes and analysis. 

## The zeta function and its Euler product

We begin with a rapid review of infinite products. If $\{ A _ { n } \} _ { n = 1 } ^ { \infty }$ is a sequence of real numbers, we define 

$$
\prod_ {n = 1} ^ {\infty} A _ {n} = \lim _ {N \to \infty} \prod_ {n = 1} ^ {N} A _ {n}
$$

if the limit exists, in which case we say that the product converges. The natural approach is to take logarithms and transform products into sums. We gather in a lemma the properties we shall need of the function log x, defined for positive real numbers. 

Lemma 1.8 The exponential and logarithm functions satisfy the following properties: 

(i) $e ^ { \log x } = x .$ 

(ii) $\log ( 1 + x ) = x + E ( x )$ where $| E ( x ) | \leq x ^ { 2 } \ i f \ | x | < 1 / 2$ 

(iii) $I f \log ( 1 + x ) = y$ and $| x | < 1 / 2$ , then $| y | \leq 2 | x |$ 

In terms of the O notation, property (ii) will be recorded as $\log ( 1 + x ) = x + O ( x ^ { 2 } )$ 

Proof. Property (i) is standard. To prove property (ii) we use the power series expansion of $\log ( 1 + x )$ for $| x | < 1$ , that is, 

$$
\log (1 + x) = \sum_ {n = 1} ^ {\infty} \frac {(- 1) ^ {n + 1}}{n} x ^ {n}.\tag{2}
$$

1. A little elementary number theory 

Then we have 

$$
E (x) = \log (1 + x) - x = - \frac {x ^ {2}}{2} + \frac {x ^ {3}}{3} - \frac {x ^ {4}}{4} + \dots ,
$$

and the triangle inequality implies 

$$
| E (x) | \leq \frac {x ^ {2}}{2} \left(1 + | x | + | x | ^ {2} + \dots\right).
$$

Therefore, if $| x | \le 1 / 2$ we can sum the geometric series on the right-hand side to find that 

$$
\begin{array}{l} | E (x) | \leq \frac {x ^ {2}}{2} \left(1 + \frac {1}{2} + \frac {1}{2 ^ {2}} + \dots\right) \\ \quad \leq \frac {x ^ {2}}{2} \left(\frac {1}{1 - 1 / 2}\right) \\ \quad \leq x ^ {2}. \end{array}
$$

The proof of property (iii) is now immediate; if $x \neq 0$ and $| x | \le 1 / 2$ , then 

$$
\begin{array}{r l} \left| \frac {\log (1 + x)}{x} \right| & \leq 1 + \left| \frac {E (x)}{x} \right| \\ & \leq 1 + | x | \\ & \leq 2, \end{array}
$$

and if $x = 0$ , (iii) is clearly also true. 

We can now prove the main result on infinite products of real numbers. 

Proposition 1.9 If $A _ { n } = 1 + a _ { n }$ and $\sum \left| a _ { n } \right|$ converges, then the product $\prod _ { n } A _ { n }$ converges, and this product vanishes $i f$ and only if one of its factors $A _ { n }$ vanishes. Also, if $a _ { n } \neq 1$ for all $n _ { ; }$ , then $\textstyle \prod _ { n } { 1 / ( 1 - a _ { n } ) }$ converges. 

Proof. $\operatorname { I f } \sum \left| a _ { n } \right|$ converges, then for all large n we must have $| a _ { n } | <$ $1 / 2$ . Disregarding finitely many terms if necessary, we may assume that this inequality holds for all $n$ . Then we may write the partial products as follows: 

$$
\prod_ {n = 1} ^ {N} A _ {n} = \prod_ {n = 1} ^ {N} e ^ {\log (1 + a _ {n})} = e ^ {B _ {N}},
$$

where $\begin{array} { r } { B _ { N } = \sum _ { n = 1 } ^ { N } b _ { n } } \end{array}$ with $b _ { n } = \log ( 1 + a _ { n } )$ . By the lemma, we know that $| b _ { n } | \leq 2 | a _ { n } |$ , so that $B _ { N }$ converges to a real number, say $B .$ Since the exponential function is continuous, we conclude that $e ^ { B _ { N } }$ converges to $e ^ { B }$ as N goes to infinity, proving the first assertion of the proposition. Observe also that if $1 + a _ { n } \neq 0$ for all $n _ { ; }$ , the product converges to a non-zero limit since it is expressed as $e ^ { B }$ 

Finally observe that the partial products of $\textstyle \prod _ { n } { 1 / ( 1 - a _ { n } ) }$ are $\scriptstyle 1 / \prod _ { n = 1 } ^ { N } ( 1 - a _ { n } )$ , so the same argument as above proves that the product in the denominator converges to a non-zero limit. 

With these preliminaries behind us, we can now return to the heart of the matter. For s a real number (strictly) greater than 1, we define the zeta function by 

$$
\zeta (s) = \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {s}}.
$$

To see that the series defining ζ converges, we use the principle that whenever $f$ is a decreasing function one can compare $\textstyle \sum f ( n )$ with $\textstyle { \int f ( x ) d x }$ , as is suggested by Figure 1. Note also that a similar technique was used in Chapter 3, that time bounding a sum from below by an integral. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2ab5d4b2-da28-455b-b554-908156ef0c8e/c2ad05945ca21004815051896378b57e4a2bc81d2b988fd688886c5608aba3a6.jpg)



Figure 1. Comparing sums with integrals


Here we take $f ( x ) = 1 / x ^ { s }$ to see that 

$$
\sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {s}} \leq 1 + \sum_ {n = 2} ^ {\infty} \int_ {n - 1} ^ {n} \frac {d x}{x ^ {s}} = 1 + \int_ {1} ^ {\infty} \frac {d x}{x ^ {s}},
$$

1. A little elementary number theory 

and therefore, 

$$
\zeta (s) \leq 1 + \frac {1}{s - 1}.\tag{3}
$$

Clearly, the series defining $\zeta$ converges uniformly on each half-line $s > s _ { 0 } > 1$ , hence $\zeta$ is continuous when $s > 1$ . The zeta function was already mentioned earlier in the discussion of the Poisson summation formula and the theta function. 

The key result is Euler’s product formula. 

Theorem 1.10 For every $s > 1$ , we have 

$$
\zeta (s) = \prod_ {p} \frac {1}{1 - 1 / p ^ {s}},
$$

where the product is taken over all primes. 

It is important to remark that this identity is an analytic expression of the fundamental theorem of arithmetic. In fact, each factor of the product $1 / ( 1 - p ^ { - s } )$ can be written as a convergent geometric series 

$$
1 + \frac {1}{p ^ {s}} + \frac {1}{p ^ {2 s}} + \dots + \frac {1}{p ^ {M s}} + \dots .
$$

$\mathrm { S o }$ we consider 

$$
\prod_ {p _ {j}} \left(1 + \frac {1}{p _ {j} ^ {s}} + \frac {1}{p _ {j} ^ {2 s}} + \dots + \frac {1}{p _ {j} ^ {M s}} + \dots\right),
$$

where the product is taken over all primes, which we order in increasing order $p _ { 1 } < p _ { 2 } < \cdots$ . Proceeding formally (these manipulations will be justified below), we calculate the product as a sum of terms, each term originating by picking out a term $1 / p _ { j } ^ { k s }$ (in the sum corresponding to $p _ { j } )$ with a $k ,$ which of course will depend on $j ,$ , and with $k = 0$ for $j$ suficiently large. The product obtained this way is 

$$
\frac {1}{(p _ {1} ^ {k _ {1}} p _ {2} ^ {k _ {2}} \cdots p _ {m} ^ {k _ {m}}) ^ {s}} = \frac {1}{n ^ {s}},
$$

where the integer n is written as a product of primes $n = p _ { 1 } ^ { k _ { 1 } } p _ { 2 } ^ { k _ { 2 } } \cdot \cdot \cdot p _ { m } ^ { k _ { m } }$ By the fundamental theorem of arithmetic, each integer $\geq 1$ occurs in this way uniquely, hence the product equals 

$$
\sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {s}}.
$$

We now justify this heuristic argument. 

Proof. Suppose M and N are positive integers with $M > N$ . Observe now that any positive integer $n \leq N$ can be written uniquely as a product of primes, and that each prime must be less than or equal to N and repeated less than M times. Therefore 

$$
\begin{array}{r l} & {\sum_ {n = 1} ^ {N} \frac {1}{n ^ {s}} \leq \prod_ {p \leq N} \left(1 + \frac {1}{p ^ {s}} + \frac {1}{p ^ {2 s}} + \dots + \frac {1}{p ^ {M s}}\right)} \\ & {\quad \leq \prod_ {p \leq N} \left(\frac {1}{1 - p ^ {- s}}\right)} \\ & {\quad \leq \prod_ {p} \left(\frac {1}{1 - p ^ {- s}}\right).} \end{array}
$$

Letting N tend to infinity now yields 

$$
\sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {s}} \leq \prod_ {p} \left(\frac {1}{1 - p ^ {- s}}\right).
$$

For the reverse inequality, we argue as follows. Again, by the fundamental theorem of arithmetic, we find that 

$$
\prod_ {p \leq N} \left(1 + \frac {1}{p ^ {s}} + \frac {1}{p ^ {2 s}} + \dots + \frac {1}{p ^ {M s}}\right) \leq \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {s}}.
$$

Letting M tend to infinity gives 

$$
\prod_ {p \leq N} \left(\frac {1}{1 - p ^ {- s}}\right) \leq \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {s}}.
$$

Hence 

$$
\prod_ {p} \left(\frac {1}{1 - p ^ {- s}}\right) \leq \sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {s}},
$$

and the proof of the product formula is complete. 

We now come to Euler’s version of Theorem 1.7, which inspired Dirichlet’s approach to the general problem of primes in arithmetic progression. The point is the following proposition. 

1. A little elementary number theory 

Proposition 1.11 The series 

$$
\sum_ {p} 1 / p
$$

diverges, when the sum is taken over all primes p. 

Of course, if there were only finitely many primes the series would converge automatically. 

Proof. We take logarithms of both sides of the Euler formula. Since log x is continuous, we may write the logarithm of the infinite product as the sum of the logarithms. Therefore, we obtain for $s > 1$ 

$$
- \sum_ {p} \log (1 - 1 / p ^ {s}) = \log \zeta (s).
$$

Since log $( 1 + x ) = x + O ( | x | ^ { 2 } )$ whenever $| x | \le 1 / 2$ , we get 

$$
- \sum_ {p} \left[ - 1 / p ^ {s} + O (1 / p ^ {2 s}) \right] = \log \zeta (s),
$$

which gives 

$$
\sum_ {p} 1 / p ^ {s} + O (1) = \log \zeta (s).
$$

The term O(1) appears because $\textstyle \sum _ { p } 1 / p ^ { 2 s } \leq \sum _ { n = 1 } ^ { \infty } 1 / n ^ { 2 }$ . Now we let s tend to 1 from above, namely $s \to 1 ^ { + }$ , and note that $\zeta ( s ) \to \infty$ since $\textstyle \sum _ { n = 1 } ^ { \infty } 1 / n ^ { s } \geq \sum _ { n = 1 } ^ { M } 1 / n ^ { s }$ , and therefore 

$$
\liminf _ {s \to 1 ^ {+}} \sum_ {n = 1} ^ {\infty} 1 / n ^ {s} \geq \sum_ {n = 1} ^ {M} 1 / n \quad \text { for   every } M.
$$

We conclude that $\begin{array} { r } { \sum _ { p } 1 / p ^ { s } \to \infty \mathrm { ~ a s ~ } s \to 1 ^ { + } } \end{array}$ , and since $1 / p > 1 / p ^ { s }$ for all $s > 1$ , we finally have that 

$$
\sum_ {p} 1 / p = \infty .
$$

In the rest of this chapter we see how Dirichlet adapted Euler’s insight. 

## 2 Dirichlet’s theorem

We remind the reader of our goal: 

Theorem 2.1 $I f q$ and ` are relatively prime positive integers, then there are infinitely many primes of the form ` + kq with $k \in \mathbb { Z }$ 

Following Euler’s argument, Dirichlet proved this theorem by showing that the series 

$$
\sum_ {p \equiv \ell \mod q} \frac {1}{p}
$$

diverges, where the sum is over all primes congruent to ` modulo $q .$ Once $q$ is fixed and no confusion is possible, we write $p \equiv \ell$ to denote a prime congruent to $\ell$ modulo $q .$ The proof consists of several steps, one of which requires Fourier analysis on the group $\mathbb { Z } ^ { \ast } ( q )$ . Before proceeding with the theorem in its complete generality, we outline the solution to the particular problem raised earlier: are there infinitely many primes of the form $4 k + 1 ?$ This example, which consists of the special case $q = 4$ and $\ell = 1$ , illustrates all the important steps in the proof of Dirichlet’s theorem. 

We begin with the character on $\mathbb { Z } ^ { \ast } ( 4 )$ defined by $\chi ( 1 ) = 1$ and $\chi ( 3 ) = - 1$ . We extend this character to all of $\mathbb { Z }$ as follows: 

$$
\chi (n) = \left\{ \begin{array}{r l} 0 & \text { if } n \text { is   even }, \\ 1 & \text { if } n = 4 k + 1, \\ - 1 & \text { if } n = 4 k + 3. \end{array} \right.
$$

Note that this function is multiplicative, that is, $\chi ( n m ) = \chi ( n ) \chi ( m )$ on all of $\mathbb { Z } .$ Let $\begin{array} { r } { L ( s , \chi ) = \sum _ { n = 1 } ^ { \infty } \chi ( n ) / n ^ { s } } \end{array}$ , so that 

$$
L (s, \chi) = 1 - \frac {1}{3 ^ {s}} + \frac {1}{5 ^ {s}} - \frac {1}{7 ^ {s}} + \dots .
$$

Then $L ( 1 , \chi )$ is the convergent series given by 

$$
1 - \frac {1}{3} + \frac {1}{5} - \frac {1}{7} + \dots .
$$

Since the terms in the series are alternating and their absolute values decrease to zero we have $L ( 1 , \chi ) \neq 0$ . Because $\chi$ is multiplicative, the Euler product generalizes (as we will prove later) to $\mathrm { g i }$ ve 

$$
\sum_ {n = 1} ^ {\infty} \frac {\chi (n)}{n ^ {s}} = \prod_ {p} \frac {1}{1 - \chi (p) / p ^ {s}}.
$$

## 2. Dirichlet’s theorem

Taking the logarithm of both sides, we find that 

$$
\log L (s, \chi) = \sum_ {p} \frac {\chi (p)}{p ^ {s}} + O (1).
$$

Letting $s \to 1 ^ { + }$ , the observation that $L ( 1 , \chi ) \neq 0$ shows that $\textstyle \sum _ { p } \chi ( p ) / p ^ { s }$ remains bounded. Hence 

$$
\sum_ {p \equiv 1} \frac {1}{p ^ {s}} - \sum_ {p \equiv 3} \frac {1}{p ^ {s}}
$$

is bounded as $s \to 1 ^ { + }$ . However, we know from Proposition 1.11 that 

$$
\sum_ {p} \frac {1}{p ^ {s}}
$$

is unbounded as $s \to 1 ^ { + }$ , so putting these two facts together, we find that 

$$
2 \sum_ {p \equiv 1} \frac {1}{p ^ {s}}
$$

is unbounded as $s \to 1 ^ { + }$ . Hence $\sum _ { p \equiv 1 } 1$ /p diverges, and as a consequence there are infinitely many primes of the form $4 k + 1$ 

We digress briefly to show that in fact $L ( 1 , \chi ) = \pi / 4$ . To see this, we integrate the identity 

$$
{\frac {1}{1 + x ^ {2}}} = 1 - x ^ {2} + x ^ {4} - x ^ {6} + \dots ,
$$

and get 

$$
\int_ {0} ^ {y} \frac {d x}{1 + x ^ {2}} = y - \frac {y ^ {3}}{3} + \frac {y ^ {5}}{5} - \dots , \quad 0 <   y <   1.
$$

We then let y tend to 1. The integral can be calculated as 

$$
\int_ {0} ^ {1} \frac {d x}{1 + x ^ {2}} = \left. \arctan u \right| _ {0} ^ {1} = \frac {\pi}{4},
$$

so this proves that the series $1 - 1 / 3 + 1 / 5 - \cdot \cdot \cdot$ is Abel summable to $\pi / 4$ . Since we know the series converges, its limit is the same as its Abel limit, hence $1 - 1 / 3 + 1 / 5 - \cdot \cdot \cdot = \pi / 4$ 

The rest of this chapter gives the full proof of Dirichlet’s theorem. We begin with the Fourier analysis (which is actually the last step in the example given above), and reduce the theorem to the non-vanishing of L-functions. 

## 2.1 Fourier analysis, Dirichlet characters, and reduction of the theorem

In what follows we take the abelian group $G$ to be $\mathbb { Z } ^ { \ast } ( q )$ . Our formulas below involve the order of $G .$ , which is the number of integers $0 \leq n <$ $q$ that are relatively prime to $q ;$ this number defines the Euler phifunction $\varphi ( q )$ , and $| G | = \varphi ( q )$ 

Consider the function $\delta _ { \ell }$ on $G$ , which we think of as the characteristic function of $\ell ;$ if $n \in \mathbb { Z } ^ { \ast } ( q )$ , then 

$$
\delta_ {\ell} (n) = \left\{ \begin{array}{l l} 1 & \text { if } n \equiv \ell \mod q, \\ 0 & \text { otherwise }. \end{array} \right.
$$

We can expand this function in a Fourier series as follows: 

$$
\delta_ {\ell} (n) = \sum_ {e \in \hat {G}} \widehat {\delta_ {\ell}} (e) e (n),
$$

where 

$$
\widehat {\delta_ {\ell}} (e) = \frac {1}{| G |} \sum_ {m \in G} \delta_ {\ell} (m) \overline {{e (m)}} = \frac {1}{| G |} \overline {{e (\ell)}}.
$$

Hence 

$$
\delta_ {\ell} (n) = \frac {1}{| G |} \sum_ {e \in \hat {G}} \overline {{e (\ell)}} e (n).
$$

We can extend the function $\delta _ { \ell }$ to all of Z by setting $\delta _ { \ell } ( m ) = 0$ whenever m and $q$ are not relatively prime. Similarly, the extensions of the characters $e \in { \hat { G } }$ to all of $\mathbb { Z }$ which are given by the recipe 

$$
\chi (m) = \left\{ \begin{array}{c l} e (m) & \text { if } m \text { and } q \text { are   relatively   prime } \\ 0 & \text { otherwise }, \end{array} \right.
$$

are called the Dirichlet characters modulo $q .$ We shall denote the extension to $\mathbb { Z }$ of the trivial character of $G$ by $\chi _ { 0 } .$ , so that $\chi _ { 0 } ( m ) = 1$ if m and $q$ are relatively prime, and 0 otherwise. Note that the Dirichlet characters modulo $q$ are multiplicative on all of $\mathbb { Z } .$ , in the sense that 

$$
\chi (n m) = \chi (n) \chi (m) \quad \mathrm{forall} n, m \in \mathbb {Z}.
$$

Since the integer $q$ is fixed, we may without fear of confusion, speak of “Dirichlet characters” omitting reference to $\boldsymbol { q . } ^ { 1 }$ 

With $| G | = \varphi ( q )$ , we may restate the above results as follows: 

## 2. Dirichlet’s theorem

Lemma 2.2 The Dirichlet characters are multiplicative. Moreover, 

$$
\delta_ {\ell} (m) = \frac {1}{\varphi (q)} \sum_ {\chi} \overline {{\chi (\ell)}} \chi (m),
$$

where the sum is over all Dirichlet characters. 

With the above lemma we have taken our first step towards a proof of the theorem, since this lemma shows that 

$$
\begin{array}{c} \sum_ {p \equiv \ell} \frac {1}{p ^ {s}} = \sum_ {p} \frac {\delta_ {\ell} (p)}{p ^ {s}} \\ = \frac {1}{\varphi (q)} \sum_ {\chi} \overline {{\chi (\ell)}} \sum_ {p} \frac {\chi (p)}{p ^ {s}}. \end{array}
$$

Thus it sufices to understand the behavior of $\begin{array} { r } { \sum _ { p } \chi ( p ) p ^ { - s } } \end{array}$ as $s \to 1 ^ { + }$ . In fact, we divide the above sum in two parts depending on whether or not $\chi$ is trivial. So we have 

$$
\begin{array}{c} \sum_ {p \equiv \ell} \frac {1}{p ^ {s}} = \frac {1}{\varphi (q)} \sum_ {p} \frac {\chi_ {0} (p)}{p ^ {s}} + \frac {1}{\varphi (q)} \sum_ {\chi \neq \chi_ {0}} \overline {{\chi (\ell)}} \sum_ {p} \frac {\chi (p)}{p ^ {s}} \\ = \frac {1}{\varphi (q)} \sum_ {p \text {   not   dividing   } q} \frac {1}{p ^ {s}} + \frac {1}{\varphi (q)} \sum_ {\chi \neq \chi_ {0}} \overline {{\chi (\ell)}} \sum_ {p} \frac {\chi (p)}{p ^ {s}}. \end{array}\tag{4}
$$

Since there are only finitely many primes dividing $q ,$ Euler’s theorem (Proposition 1.11) implies that the first sum on the right-hand side diverges when s tends to 1. These observations show that Dirichlet’s theorem is a consequence of the following assertion. 

Theorem 2.3 $I f \chi$ is a nontrivial Dirichlet character, then the sum 

$$
\sum_ {p} \frac {\chi (p)}{p ^ {s}}
$$

remains bounded as $s \to 1 ^ { + }$ 

The proof of Theorem 2.3 requires the introduction of the L-functions, to which we now turn. 

## 2.2 Dirichlet L-functions

We proved earlier that the zeta function $\textstyle \zeta ( s ) = \sum _ { n } 1 / n ^ { s }$ could be expressed as a product, namely 

$$
\sum_ {n = 1} ^ {\infty} \frac {1}{n ^ {s}} = \prod_ {p} \frac {1}{(1 - p ^ {- s})}.
$$

Dirichlet observed an analogue of this formula for the so-called L-functions defined for $s > 1$ by 

$$
L (s, \chi) = \sum_ {n = 1} ^ {\infty} \frac {\chi (n)}{n ^ {s}},
$$

where $\chi$ is a Dirichlet character. 

Theorem 2.4 If $s > 1$ , then 

$$
\sum_ {n = 1} ^ {\infty} \frac {\chi (n)}{n ^ {s}} = \prod_ {p} \frac {1}{(1 - \chi (p) p ^ {- s})},
$$

where the product is over all primes. 

Assuming this theorem for now, we can follow Euler’s argument formally: taking the logarithm of the product and using the fact that $\log ( 1 + x ) = x + O ( x ^ { 2 } )$ whenever x is small, we would get 

$$
\begin{array}{r l} & {\log L (s, \chi) = - \sum_ {p} \log (1 - \chi (p) / p ^ {s})} \\ & {\qquad = - \sum_ {p} \left[ - \frac {\chi (p)}{p ^ {s}} + O \left(\frac {1}{p ^ {2 s}}\right) \right]} \\ & {\qquad = \sum_ {p} \frac {\chi (p)}{p ^ {s}} + O (1).} \end{array}
$$

If $L ( 1 , \chi )$ is finite and non-zero, then log $L ( s , \chi )$ is bounded as $s \to 1 ^ { + }$ ， and we can conclude that the sum 

$$
\sum_ {p} \frac {\chi (p)}{p ^ {s}}
$$

is bounded as $s \to 1 ^ { + }$ . We now make several observations about the above formal argument. 

First, we must prove the product formula in Theorem 2.4. Since the Dirichlet characters $\chi$ can be complex-valued we will extend the logarithm to complex numbers $w$ of the form $w = 1 / ( 1 - z )$ with $| z | < 1$ (This will be done in terms of a power series.) Then we show that with this definition of the logarithm, the proof of Euler’s product formula given earlier carries over to L-functions. 

Second, we must make sense of taking the logarithm of both sides of the product formula. If the Dirichlet characters are real, this argument works 

## 2. Dirichlet’s theorem

and is precisely the one given in the example corresponding to primes of the form $4 k + 1$ . In general, the dificulty lies in the fact that $\chi ( p )$ is a complex number, and the complex logarithm is not single valued; in particular, the logarithm of a product is not the sum of the logarithms. 

Third, it remains to prove that whenever $\chi \neq \chi _ { 0 }$ , then log $L ( s , \chi )$ is bounded as $s \to 1 ^ { + }$ . If (as we shall see) $L ( s , \chi )$ is continuous at $s = 1$ 2 then it sufices to show that 

$$
L (1, \chi) \neq 0.
$$

This is the non-vanishing we mentioned earlier, which corresponds to the alternating series being non-zero in the previous example. The fact that $L ( 1 , \chi ) \neq 0$ is the most dificult part of the argument. 

So we will focus on three points: 

1. Complex logarithms and infinite products. 

2. Study of $L ( s , \chi )$ 

3. Proof that $L ( 1 , \chi ) \neq 0 \mathrm { i f } \chi$ is non-trivial. 

However, before we enter further into the details, we pause briefly to discuss some historical facts surrounding Dirichlet’s theorem. 

## Historical digression

In the following list, we have gathered the names of those mathematicians whose work dealt most closely with the series of achievements related to Dirichlet’s theorem. To give a better perspective, we attach the years in which they reached the age of 35: 

Euler 1742 

Legendre 1787 

Gauss 1812 

Dirichlet 1840 

Riemann 1861 

As we mentioned earlier, Euler’s discovery of the product formula for the zeta function is the starting point in Dirichlet’s argument. Legendre in efect conjectured the theorem because he needed it in his proof of the law of quadratic reciprocity. However, this goal was first accomplished by Gauss who, while not knowing how to establish the theorem about primes in arithmetic progression, nevertheless found a number of diferent proofs of quadratic reciprocity. Later, Riemann extended the study of the zeta function to the complex plane and indicated how properties related to the non-vanishing of that function were central in the further understanding of the distribution of prime numbers. 

Dirichlet proved his theorem in 1837. It should be noted that Fourier, who had befriended Dirichlet when the latter was a young mathematician visiting Paris, had died several years before. Besides the great activity in mathematics, that period was also a very fertile time in the arts, and in particular music. The era of Beethoven had ended only ten years earlier, and Schumann was now reaching the heights of his creativity. But the musician whose career was closest to Dirichlet was Felix Mendelssohn (four years his junior). It so happens that the latter began composing his famous violin concerto the year after Dirichlet succeeded in proving his theorem. 

## 3 Proof of the theorem

We return to the proof of Dirichlet’s theorem and to the three dificulties mentioned above. 

## 3.1 Logarithms

The device to deal with the first point is to define two logarithms, one for complex numbers of the form $1 / ( 1 - z )$ with $| z | < 1$ which we denote by log<sub>1</sub>, and one for the function $L ( s , \chi )$ which we will denote by log<sub>2</sub>. 

For the first logarithm, we define 

$$
\log_ {1} \left(\frac {1}{1 - z}\right) = \sum_ {k = 1} ^ {\infty} \frac {z ^ {k}}{k} \quad \text { for } | z | <   1.
$$

Note that log w is then defined if $\operatorname { R e } ( w ) > 1 / 2$ , and because of equation (2), log w gives an extension of the usual log x when x is a real number $> 1 / 2$ 

Proposition 3.1 The logarithm function log<sub>1</sub> satisfies the following properties: 

(i) $I f \mid z \mid < 1$ , then 

$$
e ^ {\log_ {1} \left(\frac {1}{1 - z}\right)} = \frac {1}{1 - z}.
$$

(ii) $I f \mid z \mid < 1$ , then 

$$
\log_ {1} \left(\frac {1}{1 - z}\right) = z + E _ {1} (z),
$$

where the error $E _ { 1 }$ satisfies $| E _ { 1 } ( z ) | \le | z | ^ { 2 } \ i f | z | < 1 / 2$ 

3. Proof of the theorem 

(iii) $I f \left| z \right| < 1 / 2$ , then 

$$
\left| \log_ {1} \left(\frac {1}{1 - z}\right) \right| \leq 2 | z |.
$$

Proof. To establish the first property, let $z = r e ^ { i \theta }$ with $0 \leq r < 1$ 2 and observe that it sufices to show that 

$$
\left(1 - r e ^ {i \theta}\right) e ^ {\sum_ {k = 1} ^ {\infty} (r e ^ {i \theta}) ^ {k} / k} = 1.\tag{5}
$$

To do so, we diferentiate the left-hand side with respect to r, and this gives 

$$
\left[ - e ^ {i \theta} + (1 - r e ^ {i \theta}) \left(\sum_ {k = 1} ^ {\infty} (r e ^ {i \theta}) ^ {k} / k\right) ^ {\prime} \right] e ^ {\sum_ {k = 1} ^ {\infty} (r e ^ {i \theta}) ^ {k} / k}.
$$

The term in brackets equals 

$$
- e ^ {i \theta} + (1 - r e ^ {i \theta}) e ^ {i \theta} \left(\sum_ {k = 1} ^ {\infty} (r e ^ {i \theta}) ^ {k - 1}\right) = - e ^ {i \theta} + (1 - r e ^ {i \theta}) e ^ {i \theta} \frac {1}{1 - r e ^ {i \theta}} = 0.
$$

Having found that the left-hand side of the equation (5) is constant, we set $r = 0$ and get the desired result. 

The proofs of the second and third properties are the same as their real counterparts given in Lemma 1.8. 

Using these results we can state a suficient condition guaranteeing the convergence of infinite products of complex numbers. Its proof is the same as in the real case, except that we now use the logarithm $\log _ { 1 }$ 

Proposition 3.2 $I f \sum | a _ { n } |$ converges, and $a _ { n } \neq 1$ for all n, then 

$$
\prod_ {n = 1} ^ {\infty} \left(\frac {1}{1 - a _ {n}}\right)
$$

converges. Moreover, this product is non-zero. 

Proof. For n large enough, $\vert a _ { n } \vert < 1 / 2$ , so we may assume without loss of generality that this inequality holds for all $n \geq 1$ . Then 

$$
\prod_ {n = 1} ^ {N} \left(\frac {1}{1 - a _ {n}}\right) = \prod_ {n = 1} ^ {N} e ^ {\log_ {1} \left(\frac {1}{1 - a _ {n}}\right)} = e ^ {\sum_ {n = 1} ^ {N} \log_ {1} \left(\frac {1}{1 - a _ {n}}\right)}.
$$

But we know from the previous proposition that 

$$
\left| \log_ {1} \left(\frac {1}{1 - z}\right) \right| \leq 2 | z |,
$$

so the fact that the series $\sum \left| a _ { n } \right|$ converges, immediately implies that the limit 

$$
\lim _ {N \to \infty} \sum_ {n = 1} ^ {N} \log_ {1} \left(\frac {1}{1 - a _ {n}}\right) = A
$$

exists. Since the exponential function is continuous, we conclude that the product converges to $e ^ { A }$ , which is clearly non-zero. 

We may now prove the promised Dirichlet product formula 

$$
\sum_ {n} \frac {\chi (n)}{n ^ {s}} = \prod_ {p} \frac {1}{(1 - \chi (p) p ^ {- s})}.
$$

For simplicity of notation, let L denote the left-hand side of the above equation. Define 

$$
S _ {N} = \sum_ {n \leq N} \chi (n) n ^ {- s} \quad \text { and } \quad \Pi_ {N} = \prod_ {p \leq N} \left(\frac {1}{1 - \chi (p) p ^ {- s}}\right).
$$

The infinite product $\begin{array} { r } { \Pi = \operatorname* { l i m } _ { N \to \infty } \Pi _ { N } = \prod _ { p } \left( \frac { 1 } { 1 - \chi ( p ) p ^ { - s } } \right) } \end{array}$ converges by the previous proposition. Indeed, if we set $a _ { n } = \chi ( p _ { n } ) p _ { n } ^ { - s }$ , where $p _ { n }$ is the $n ^ { \mathrm { t h } }$ prime, we note that if $s > 1$ , then $\sum \left| a _ { n } \right| < \infty$ 

Also, define 

$$
\Pi_ {N, M} = \prod_ {p \leq N} \left(1 + \frac {\chi (p)}{p ^ {s}} + \dots + \frac {\chi (p ^ {M})}{p ^ {M s}}\right).
$$

Now fix $\epsilon > 0$ and choose N so large that 

$$
\left| S _ {N} - L \right| <   \epsilon \quad \text { and } \quad \left| \Pi_ {N} - \Pi \right| <   \epsilon .
$$

We can next select M large enough so that 

$$
\left| S _ {N} - \Pi_ {N, M} \right| <   \epsilon \quad \mathrm{and} \quad \left| \Pi_ {N, M} - \Pi_ {N} \right| <   \epsilon .
$$

To see the first inequality, one uses the fundamental theorem of arithmetic and the fact that the Dirichlet characters are multiplicative. The 

## 3. Proof of the theorem

second inequality follows merely because each series $\scriptstyle \sum _ { n = 1 } ^ { \infty } { \frac { \chi ( p ^ { n } ) } { p ^ { n s } } }$ converges. 

Therefore 

$$
| L - \Pi | \leq | L - S _ {N} | + | S _ {N} - \Pi_ {N, M} | + | \Pi_ {N, M} - \Pi_ {N} | + | \Pi_ {N} - \Pi | <   4 \epsilon ,
$$

as was to be shown. 

## 3.2 L-functions

The next step is a better understanding of the L-functions. Their behavior as functions of s (especially near $s = 1 )$ depends on whether or not χ is trivial. In the first case, $L ( s , \chi _ { 0 } )$ is up to some simple factors just the zeta function. 

Proposition 3.3 Suppose $\chi _ { 0 }$ is the trivial Dirichlet character, 

$$
\chi_ {0} (n) = \left\{ \begin{array}{l l} 1 & \text {   if   } n \text {   and   } q \text {   are   relatively   prime,   } \\ 0 & \text {   otherwise,   } \end{array} \right.
$$

and $q = p _ { 1 } ^ { a _ { 1 } } \cdot \cdot \cdot p _ { N } ^ { a _ { N } }$ is the prime factorization of q. Then 

$$
L (s, \chi_ {0}) = (1 - p _ {1} ^ {- s}) (1 - p _ {2} ^ {- s}) \dots (1 - p _ {N} ^ {- s}) \zeta (s).
$$

Therefore $L ( s , \chi _ { 0 } ) \longrightarrow \infty \ a s \ s \longrightarrow 1 ^ { + }$ 

Proof. The identity follows at once on comparing the Dirichlet and Euler product formulas. The final statement holds because $\zeta ( s ) \to \infty$ as $s \to 1 ^ { + }$ 

The behavior of the remaining L-functions, those for which $\chi \neq$ χ<sub>0</sub>, is more subtle. A remarkable property is that these functions are now defined and continuous for $s > 0$ . In fact, more is true. 

Proposition 3.4 $I f \chi$ is a non-trivial Dirichlet character, then the series 

$$
\sum_ {n = 1} ^ {\infty} \chi (n) / n ^ {s}
$$

converges $f o r \ s > 0$ , and we denote its sum by $L ( s , \chi )$ . Moreover: 

(i) The function $L ( s , \chi )$ is continuously diferentiable for $0 < s < \infty$ 

(ii) There exists constants $c , c ^ { \prime } > 0$ so that 

$$
L (s, \chi) = 1 + O (e ^ {- c s}) \quad a s s \to \infty , a n d
$$

$$
L ^ {\prime} (s, \chi) = O (e ^ {- c ^ {\prime} s}) \qquad a s s \to \infty .
$$

We first isolate the key cancellation property that non-trivial Dirichlet characters possess, which accounts for the behavior of the L-function described in the proposition. 

Lemma 3.5 $I f \chi$ is a non-trivial Dirichlet character, then 

$$
\left| \sum_ {n = 1} ^ {k} \chi (n) \right| \leq q, \quad f o r a n y k.
$$

Proof. First, we recall that 

$$
\sum_ {n = 1} ^ {q} \chi (n) = 0.
$$

In fact, if $S$ denotes the sum and $a \in \mathbb { Z } ^ { \ast } ( q )$ , then the multiplicative property of the Dirichlet character $\chi$ gives 

$$
\chi (a) S = \sum \chi (a) \chi (n) = \sum \chi (a n) = \sum \chi (n) = S.
$$

Since $\chi$ is non-trivial, $\chi ( a ) \neq 1$ for some $a ,$ hence $S = 0$ . We now write $k = a q + b$ with $0 \leq b < q ,$ and note that 

$$
\sum_ {n = 1} ^ {k} \chi (n) = \sum_ {n = 1} ^ {a q} \chi (n) + \sum_ {a q <   n \leq a q + b} \chi (n) = \sum_ {a q <   n \leq a q + b} \chi (n),
$$

and there are no more than q terms in the last sum. The proof is complete once we recall that $| \chi ( n ) | \leq 1$ 

We can now prove the proposition. Let $\begin{array} { r } { s _ { k } = \sum _ { n = 1 } ^ { k } \chi ( n ) } \end{array}$ , and $s _ { 0 } = 0$ We know that $L ( s , \chi )$ is defined for $s > 1$ by the series 

$$
\sum_ {n = 1} ^ {\infty} \frac {\chi (n)}{n ^ {s}}
$$

which converges absolutely and uniformly for $s > \delta > 1$ . Moreover, the diferentiated series also converges absolutely and uniformly for $s > \delta >$ 1, which shows that $L ( s , \chi )$ is continuously diferentiable for $s > 1$ . We 

## 3. Proof of the theorem

sum by $\mathrm { p a r t s ^ { 2 } }$ to extend this result to $s > 0 ,$ . Indeed, we have 

$$
\begin{array}{l} \sum_ {k = 1} ^ {N} \frac {\chi (k)}{k ^ {s}} = \sum_ {k = 1} ^ {N} \frac {s _ {k} - s _ {k - 1}}{k ^ {s}} \\ \qquad = \sum_ {k = 1} ^ {N - 1} s _ {k} \left[ \frac {1}{k ^ {s}} - \frac {1}{(k + 1) ^ {s}} \right] + \frac {s _ {N}}{N ^ {s}} \\ \qquad = \sum_ {k = 1} ^ {N - 1} f _ {k} (s) + \frac {s _ {N}}{N ^ {s}}, \end{array}
$$

where $f _ { k } ( s ) = s _ { k } [ k ^ { - s } - ( k + 1 ) ^ { - s } ] . \mathrm { ~ I f ~ } g ( x ) = x ^ { - s }$ , then $g ^ { \prime } ( x ) = - s x ^ { - s - 1 }$ so applying the mean-value theorem between $x = k$ and $x = k + 1$ , and the fact that $| s _ { k } | \le q$ , we find that 

$$
| f _ {k} (s) | \leq q s k ^ {- s - 1}.
$$

Therefore, the series $\textstyle \sum f _ { k } ( s )$ converges absolutely and uniformly for $s >$ $\delta > 0$ , and this proves that $L ( s , \chi )$ is continuous for $s > 0$ . To prove that it is also continuously diferentiable, we diferentiate the series term by term, obtaining 

$$
\sum (\log n) \frac {\chi (n)}{n ^ {s}}.
$$

Again, we rewrite this series using summation by parts as 

$$
\sum s _ {k} \left[ - k ^ {- s} \log k + (k + 1) ^ {- s} \log (k + 1) \right],
$$

and an application of the mean-value theorem to the function $g ( x ) =$ $x ^ { - s }$ log x shows that the terms are $O ( k ^ { - \delta / 2 - 1 } )$ , thus proving that the diferentiated series converges uniformly for $s > \delta > 0$ . Hence $L ( s , \chi )$ is continuously diferentiable for $s > 0$ 

Now, observe that for all s large, 

$$
\begin{array}{c} | L (s, \chi) - 1 | \leq 2 q \sum_ {n = 2} ^ {\infty} n ^ {- s} \\ \leq 2 ^ {- s} O (1), \end{array}
$$

and we can take $c = \log 2$ , to see that $L ( s , \chi ) = 1 + O ( e ^ { - c s } )$ as $s \to \infty$ A similar argument also shows that $L ^ { \prime } ( s , \chi ) = O ( e ^ { - c ^ { \prime } s } )$ as $s \to \infty$ with in fact $c ^ { \prime } = c ,$ and the proof of the proposition is complete. 

With the facts gathered so far about $L ( s , \chi )$ we are in a position to define the logarithm of the L-functions. This is done by integrating its logarithmic derivative. In other words, if $\chi$ is a non-trivial Dirichlet character and $s > 1$ we define<sup>3</sup> 

$$
\log_ {2} L (s, \chi) = - \int_ {s} ^ {\infty} \frac {L ^ {\prime} (t , \chi)}{L (t , \chi)} d t.
$$

We know that $L ( t , \chi ) \neq 0$ for every $t > 1$ since it is given by a product (Proposition 3.2), and the integral is convergent because 

$$
\frac {L ^ {\prime} (t , \chi)}{L (t , \chi)} = O (e ^ {- c t}),
$$

which follows from the behavior at infinity of $L ( t , \chi )$ and $L ^ { \prime } ( t , \chi )$ recorded earlier. 

The following links the two logarithms. 

Proposition 3.6 $I f s > 1$ , then 

$$
e ^ {\log_ {2} L (s, \chi)} = L (s, \chi).
$$

Moreover 

$$
\log_ {2} L (s, \chi) = \sum_ {p} \log_ {1} \left(\frac {1}{1 - \chi (p) / p ^ {s}}\right).
$$

Proof. Diferentiating $e ^ { - \log _ { 2 } { L ( s , \chi ) } } L ( s , \chi )$ with respect to s gives 

$$
- \frac {L ^ {\prime} (s , \chi)}{L (s , \chi)} e ^ {- \log_ {2} L (s, \chi)} L (s, \chi) + e ^ {- \log_ {2} L (s, \chi)} L ^ {\prime} (s, \chi) = 0.
$$

So $e ^ { - \log _ { 2 } { L ( s , \chi ) } } L ( s , \chi )$ is constant, and this constant can be seen to be 1 by letting s tend to infinity. This proves the first conclusion. 

To prove the equality between the logarithms, we fix s and take the exponential of both sides. The left-hand side becomes $e ^ { \log _ { 2 } L ( s , \chi ) } = L ( s , \chi )$ 2 and the right-hand side becomes 

$$
e ^ {\sum_ {p} \log_ {1} \left(\frac {1}{1 - \chi (p) / p ^ {s}}\right)} = \prod_ {p} e ^ {\log_ {1} \left(\frac {1}{1 - \chi (p) / p ^ {s}}\right)} = \prod_ {p} \left(\frac {1}{1 - \chi (p) / p ^ {s}}\right) = L (s, \chi),
$$

## 3. Proof of the theorem

by (i) in Proposition 3.1 and the Dirichlet product formula. Therefore, for each s there exists an integer $M ( s )$ so that 

$$
\log_ {2} L (s, \chi) - \sum_ {p} \log_ {1} \left(\frac {1}{1 - \chi (p) / p ^ {s}}\right) = 2 \pi i M (s).
$$

As the reader may verify, the left-hand side is continuous in $s ,$ and this implies the continuity of the function $M ( s )$ . But $M ( s )$ is integer-valued so we conclude that $M ( s )$ is constant, and this constant can be seen to be 0 by letting s go to infinity. 

Putting together the work we have done so far gives rigorous meaning to the formal argument presented earlier. Indeed, the properties of $\log _ { 1 }$ show that 

$$
\begin{array}{r} \sum_ {p} \log_ {1} \left(\frac {1}{1 - \chi (p) / p ^ {s}}\right) = \sum_ {p} \frac {\chi (p)}{p ^ {s}} + O \left(\sum_ {p} \frac {1}{p ^ {2 s}}\right) \\ = \sum_ {p} \frac {\chi (p)}{p ^ {s}} + O (1). \end{array}
$$

Now if $L ( 1 , \chi ) \neq 0$ for a non-trivial Dirichlet character, then by its integral representation lo $\mathfrak { \xi } _ { 2 } L ( s , \chi )$ remains bounded as $s \to 1 ^ { + }$ . Thus the identity between the logarithms implies that $\begin{array} { r } { \sum _ { p } \chi ( p ) p ^ { - s } } \end{array}$ remains bounded as $s \to 1 ^ { + }$ , which is the desired result. Therefore, to finish the proof of Dirichlet’s theorem, we need to see that $L ( 1 , \chi ) \neq 0$ when $\chi$ is non-trivial. 

## 3.3 Non-vanishing of the L-function

We now turn to a proof of the following deep result: 

Theorem 3.7 $I f \chi \neq \chi _ { 0 }$ , then $L ( 1 , \chi ) \neq 0$ 

There are several proofs of this fact, some involving algebraic number theory (among them Dirichlet’s original argument), and others involving complex analysis. Here we opt for a more elementary argument that requires no special knowledge of either of these areas. The proof splits in two cases, depending on whether $\chi$ is complex or real. A Dirichlet character is said to be real if it takes on only real values (that is, $+ 1 , - 1 , \mathrm { o r } \ 0 )$ and complex otherwise. In other words, $\chi$ is real if and only if $\chi ( n ) = { \overline { { \chi ( n ) } } }$ for all integers n. 

## Case I: complex Dirichlet characters

This is the easier of the two cases. The proof is by contradiction, and we use two lemmas. 

Lemma 3.8 $I f s > 1$ , then 

$$
\prod_ {\chi} L (s, \chi) \geq 1,
$$

where the product is taken over all Dirichlet characters. In particular the product is real-valued. 

Proof. We have shown earlier that for $s > 1$ 

$$
L (s, \chi) = \exp \left(\sum_ {p} \log_ {1} \left(\frac {1}{1 - \chi (p) p ^ {- s}}\right)\right).
$$

Hence, 

$$
\begin{array}{r l} \prod_ {\chi} L (s, \chi) = & \exp \left(\sum_ {\chi} \sum_ {p} \log_ {1} \left(\frac {1}{1 - \chi (p) p ^ {- s}}\right)\right) \\ & = \exp \left(\sum_ {\chi} \sum_ {p} \sum_ {k = 1} ^ {\infty} \frac {1}{k} \frac {\chi (p ^ {k})}{p ^ {k s}}\right) \\ & = \exp \left(\sum_ {p} \sum_ {k = 1} ^ {\infty} \sum_ {\chi} \frac {1}{k} \frac {\chi (p ^ {k})}{p ^ {k s}}\right). \end{array}
$$

Because of Lemma 2.2 (with $\ell = 1 )$ we have $\begin{array} { r } { \sum _ { \chi } \chi ( p ^ { k } ) = \varphi ( q ) \delta _ { 1 } ( p ^ { k } ) } \end{array}$ , and hence 

$$
\prod_ {\chi} L (s, \chi) = \exp \left(\varphi (q) \sum_ {p} \sum_ {k = 1} ^ {\infty} \frac {1}{k} \frac {\delta_ {1} (p ^ {k})}{p ^ {k s}}\right) \geq 1,
$$

since the term in the exponential is non-negative. 

Lemma 3.9 The following three properties hold: 

(i) $I f L ( 1 , \chi ) = 0$ , then $L ( 1 , { \overline { { \chi } } } ) = 0$ 

(ii) $I f \chi$ is non-trivial and $L ( 1 , \chi ) = 0$ , then 

$$
| L (s, \chi) | \leq C | s - 1 | \quad w h e n 1 \leq s \leq 2.
$$

3. Proof of the theorem 

(iii) For the trivial Dirichlet character $\chi _ { 0 ; }$ , we have 

$$
| L (s, \chi_ {0}) | \leq \frac {C}{| s - 1 |} \quad w h e n 1 <   s \leq 2.
$$

Proof. The first statement is immediate because $L ( 1 , \overline { { \chi } } ) = \overline { { L ( 1 , \chi ) } }$ The second statement follows from the mean-value theorem since $L ( s , \chi )$ is continuously diferentiable for $s > 0$ when χ is non-trivial. Finally, the last statement follows because by Proposition 3.3 

$$
L (s, \chi_ {0}) = (1 - p _ {1} ^ {- s}) (1 - p _ {2} ^ {- s}) \dots (1 - p _ {N} ^ {- s}) \zeta (s),
$$

and ζ satisfies the similar estimate (3). 

We can now conclude the proof that $L ( 1 , \chi ) \neq 0$ for χ a non-trivial complex Dirichlet character. If not, say $L ( 1 , \chi ) = 0$ , then we also have $L ( 1 , { \overline { { \chi } } } ) = 0$ . Since $\chi \neq \overline { { \chi } }$ , there are at least two terms in the product 

$$
\prod_ {\chi} L (s, \chi),
$$

that vanish like $| s - 1 |$ as $s \to 1 ^ { + }$ . Since only the trivial character contributes a term that grows, and this growth is no worse than $O ( 1 / | s - 1 | )$ 2 we find that the product goes to 0 as $s \to 1 ^ { + }$ , contradicting the fact that it is $\geq 1$ by Lemma 3.8. 

## Case II: real Dirichlet characters

The proof that $L ( 1 , \chi ) \neq 0$ when χ is a non-trivial real Dirichlet character is very diferent from the earlier complex case. The method we shall exploit involves summation along hyperbolas. It is a curious fact that this method was introduced by Dirichlet himself, twelve years after the proof of his theorem on arithmetic progressions, to establish another famous result of his: the average order of the divisor function. However, he made no connection between the proofs of these two theorems. We will instead proceed by proving first Dirichlet’s divisor theorem, as a simple example of the method of summation along hyperbolas. Then, we shall adapt these ideas to prove the fact that $L ( 1 , \chi ) \neq 0$ . As a preliminary matter, we need to deal with some simple sums, and their corresponding integral analogues. 

## Sums vs. Integrals

Here we use the idea of comparing a sum with its corresponding integral, which already occurred in the estimate (3) for the zeta function. 

Proposition 3.10 If N is a positive integer, then: 

$$
\text {(i)} \sum_ {1 \leq n \leq N} \frac {1}{n} = \int_ {1} ^ {N} \frac {d x}{x} + O (1) = \log N + O (1).
$$

(ii) More precisely, there exists a real number $\cdot \gamma _ { ; }$ , called Euler’s constant, so that 

$$
\sum_ {1 \leq n \leq N} \frac {1}{n} = \log N + \gamma + O (1 / N).
$$

Proof. It sufices to establish the more refined estimate given in part (ii). Let 

$$
\gamma_ {n} = \frac {1}{n} - \int_ {n} ^ {n + 1} \frac {d x}{x}.
$$

Since $1 / x$ is decreasing, we clearly have 

$$
0 \leq \gamma_ {n} \leq \frac {1}{n} - \frac {1}{n + 1} \leq \frac {1}{n ^ {2}},
$$

so the series $\sum \infty _ { \mathrm { { } } } \infty _ { } $ converges to a limit which we denote by $\gamma .$ . Moreover, if we estimate $\textstyle \sum f ( n )$ by $\textstyle \int f ( x )$ dx, where $f ( x ) = 1 / x ^ { 2 }$ , we find 

$$
\sum_ {n = N + 1} ^ {\infty} \gamma_ {n} \leq \sum_ {n = N + 1} ^ {\infty} \frac {1}{n ^ {2}} \leq \int_ {N} ^ {\infty} \frac {d x}{x ^ {2}} = O (1 / N).
$$

Therefore 

$$
\sum_ {n = 1} ^ {N} \frac {1}{n} - \int_ {1} ^ {N} \frac {d x}{x} = \gamma - \sum_ {n = N + 1} ^ {\infty} \gamma_ {n} + \int_ {N} ^ {N + 1} \frac {d x}{x},
$$

and this last integral is $O ( 1 / N )$ as $N \to \infty$ 

Proposition 3.11 If N is a positive integer, then 

$$
\begin{array}{c} \sum_ {1 \leq n \leq N} \frac {1}{n ^ {1 / 2}} = \int_ {1} ^ {N} \frac {d x}{x ^ {1 / 2}} + c ^ {\prime} + O (1 / N ^ {1 / 2}) \\ = 2 N ^ {1 / 2} + c + O (1 / N ^ {1 / 2}). \end{array}
$$

The proof is essentially a repetition of the proof of the previous proposition, this time using the fact that 

$$
\left| \frac {1}{n ^ {1 / 2}} - \frac {1}{(n + 1) ^ {1 / 2}} \right| \leq \frac {C}{n ^ {3 / 2}}.
$$

## 3. Proof of the theorem

This last inequality follows from the mean-value theorem applied to $f ( x ) = x ^ { - 1 / 2 }$ , between $x = n$ and $x = n + 1$ 

## Hyperbolic sums

If F is a function defined on pairs of positive integers, there are three ways to calculate 

$$
S _ {N} = \sum \sum F (m, n),
$$

where the sum is taken over all pairs of positive integers $( m , n )$ which satisfy $m n \leq N$ 

We may carry out the summation in any one of the following three ways. (See Figure 2.) 

(a) Along hyperbolas: 

$$
S _ {N} = \sum_ {1 \leq k \leq N} \left(\sum_ {n m = k} F (m, n)\right)
$$

(b) Vertically: 

$$
S _ {N} = \sum_ {1 \leq m \leq N} \left(\sum_ {1 \leq n \leq N / m} F (m, n)\right)
$$

(c) Horizontally: 

$$
S _ {N} = \sum_ {1 \leq n \leq N} \left(\sum_ {1 \leq m \leq N / n} F (m, n)\right)
$$

It is a remarkable fact that one can obtain interesting conclusions from the obvious fact that these three methods of summation give the same sum. We apply this idea first in the study of the divisor problem. 

## Intermezzo: the divisor problem

For a positive integer k, let $d ( k )$ denote the number of positive divisors of k. For example, 

<table><tr><td>k</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>7</td><td>8</td><td>9</td><td>10</td><td>11</td><td>12</td><td>13</td><td>14</td><td>15</td><td>16</td><td>17</td></tr><tr><td>d(k)</td><td>1</td><td>2</td><td>2</td><td>3</td><td>2</td><td>4</td><td>2</td><td>4</td><td>3</td><td>4</td><td>2</td><td>6</td><td>2</td><td>4</td><td>4</td><td>5</td><td>2</td></tr></table>


270


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2ab5d4b2-da28-455b-b554-908156ef0c8e/9792ee9c214a14269d6a3d4ab87c03bcfb9605c969925bc30e1ce03ff424c5fc.jpg)



(a)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2ab5d4b2-da28-455b-b554-908156ef0c8e/c7a3ccfb06ed88e2e029f28a7a635720d08bbc53a98c15c2c579383e8cdc9d97.jpg)



(b)



Chapter 8. DIRICHLET’S THEOREM


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2ab5d4b2-da28-455b-b554-908156ef0c8e/34e2ce2e38d0b5c551fa8e7f3526b3f886cc5f38567542fd7ef9cb9b11a183fa.jpg)



(c)



Figure 2. The three methods of summation


One observes that the behavior of $d ( k )$ as k tends to infinity is rather irregular, and in fact, it does not seem possible to approximate $d ( k )$ by a simple analytic expression in k. However, it is natural to inquire about the average size of $d ( k )$ . In other words, one might ask, what is the behavior of 

$$
\frac {1}{N} \sum_ {k = 1} ^ {N} d (k) \quad \mathrm{as} N \to \infty ?
$$

The answer was provided by Dirichlet, who made use of hyperbolic sums. Indeed, we observe that 

$$
d (k) = \sum_ {n m = k, 1 \leq n, m} 1.
$$

Theorem 3.12 If k is a positive integer, then 

$$
\frac {1}{N} \sum_ {k = 1} ^ {N} d (k) = \log N + O (1).
$$

More precisely, 

$$
\frac {1}{N} \sum_ {k = 1} ^ {N} d (k) = \log N + (2 \gamma - 1) + O (1 / N ^ {1 / 2}),
$$

where $\gamma$ is Euler’s constant. 

Proof. Let $\begin{array} { r } { S _ { N } = \sum _ { k = 1 } ^ { N } d ( k ) } \end{array}$ . We observed that summing $F = 1$ along hyperbolas gives $S _ { N }$ . Summing vertically, we find 

$$
S _ {N} = \sum_ {1 \leq m \leq N} \sum_ {1 \leq n \leq N / m} 1.
$$

## 3. Proof of the theorem

But $\begin{array} { r } { \sum _ { 1 < n < N / m } 1 = [ N / m ] = N / m + O ( 1 ) } \end{array}$ , where [x] denote the greatest integer $\leq x .$ . Therefore 

$$
S _ {N} = \sum_ {1 \leq m \leq N} (N / m + O (1)) = N \left(\sum_ {1 \leq m \leq N} 1 / m\right) + O (N).
$$

Hence, by part (i) of Proposition 3.10, 

$$
\frac {S _ {N}}{N} = \log N + O (1)
$$

which gives the first conclusion. 

For the more refined estimate we proceed as follows. Consider the three regions I, II, and III shown in Figure 3. These are defined by 

$$
\begin{array}{c} {I = \{1 \leq m <   N ^ {1 / 2}, N ^ {1 / 2} <   n \leq N / m \},} \\ {I I = \{1 \leq m \leq N ^ {1 / 2}, 1 \leq n \leq N ^ {1 / 2} \},} \\ {I I I = \{N ^ {1 / 2} <   m \leq N / n, 1 \leq n <   N ^ {1 / 2} \}.} \end{array}
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2ab5d4b2-da28-455b-b554-908156ef0c8e/4890f0f3e393542c46c5802a460f6489ec9850af21d89d9304537b92bec22833.jpg)



Figure 3. The three regions I, II, and III


If $S _ { I } , S _ { I I }$ , and $S _ { I I I }$ denote the sums taken over the regions I, II, and III, respectively, then 

$$
\begin{array}{r} S _ {N} = S _ {I} + S _ {I I} + S _ {I I I} \\ = 2 (S _ {I} + S _ {I I}) - S _ {I I}, \end{array}
$$

since by symmetry $S _ { I } = S _ { I I I }$ . Now we sum vertically, and use (ii) of Proposition 3.10 to obtain 

$$
\begin{array}{l} S _ {I} + S _ {I I} = \sum_ {1 \leq m \leq N ^ {1 / 2}} \left(\sum_ {1 \leq n \leq N / m} 1\right) \\ \quad = \sum_ {1 \leq m \leq N ^ {1 / 2}} [ N / m ] \\ \quad = \sum_ {1 \leq m \leq N ^ {1 / 2}} (N / m + O (1)) \\ \quad = N \left(\sum_ {1 \leq m \leq N ^ {1 / 2}} 1 / m\right) + O (N ^ {1 / 2}) \\ \quad = N \log N ^ {1 / 2} + N \gamma + O (N ^ {1 / 2}). \end{array}
$$

Finally, $S _ { I I }$ corresponds to a square so 

$$
S _ {I I} = \sum_ {1 \leq m \leq N ^ {1 / 2}} \sum_ {1 \leq n \leq N ^ {1 / 2}} 1 = [ N ^ {1 / 2} ] ^ {2} = N + O (N ^ {1 / 2}).
$$

Putting these estimates together and dividing by N yields the more refined statement in the theorem. 

## Non-vanishing of the L-function

Our essential application of summation along hyperbolas is to the main point of this section, namely that $L ( 1 , \chi ) \neq 0$ for a non-trivial real Dirichlet character χ. 

Given such a character, let 

$$
F (m, n) = \frac {\chi (n)}{(n m) ^ {1 / 2}},
$$

and define 

$$
S _ {N} = \sum \sum F (m, n),
$$

where the sum is over all integers $m , n \geq 1$ that satisfy mn $\leq N$ 

Proposition 3.13 The following statements are true: 

(i) $S _ { N } \geq c \log N$ for some constant $c > 0$ 

(ii) $S _ { N } = 2 N ^ { 1 / 2 } L ( 1 , \chi ) + O ( 1 )$ 

## 3. Proof of the theorem

It sufices to prove the proposition, since the assumption $L ( 1 , \chi ) = 0$ would give an immediate contradiction. 

We first sum along hyperbolas. Observe that 

$$
\sum_ {n m = k} \frac {\chi (n)}{(n m) ^ {1 / 2}} = \frac {1}{k ^ {1 / 2}} \sum_ {n | k} \chi (n).
$$

For conclusion (i) it will be enough to show the following lemma. 

Lemma 3.14 $\sum _ { n | k } \chi ( n ) \geq { \left\{ \begin{array} { l l } { 0 } & { f o r ~ a l l ~ k } \\ { 1 } & { i f ~ k = \ell ^ { 2 } } \end{array} \right. }$ for some $\ell \in \mathbb { Z } .$ 

From the lemma, we then get 

$$
S _ {N} \geq \sum_ {k = \ell^ {2}, \ell \leq N ^ {1 / 2}} \frac {1}{k ^ {1 / 2}} \geq c \log N,
$$

where the last inequality follows from (i) in Proposition 3.10. 

The proof of the lemma is simple. If k is a power of a prime, say $k = p ^ { a }$ , then the divisors of k are $1 , p , p ^ { 2 } , \ldots , p ^ { a }$ and 

$$
\begin{array}{c} \sum_ {n | k} \chi (n) = \chi (1) + \chi (p) + \chi (p ^ {2}) + \dots + \chi (p ^ {a}) \\ = 1 + \chi (p) + \chi (p) ^ {2} + \dots + \chi (p) ^ {a}. \end{array}
$$

So this sum is equal to 

$$
\left\{ \begin{array}{r l} a + 1 & \text {if} \chi (p) = 1, \\ 1 & \text {if} \chi (p) = - 1 \text {and} a \text {is even}, \\ 0 & \text {if} \chi (p) = - 1 \text {and} a \text {is odd}, \\ 1 & \text {if} \chi (p) = 0, \text {that is} p | q. \end{array} \right.
$$

In general, i $\mathrm { ~ f ~ } k = p _ { 1 } ^ { a _ { 1 } } \cdot \cdot \cdot p _ { N } ^ { a _ { N } }$ , then any divisor of k is of the form $p _ { 1 } ^ { b _ { 1 } } \cdot \cdot \cdot p _ { N } ^ { b _ { N } }$ where $0 \leq b _ { j } \leq a _ { j }$ for all $j$ . Therefore, the multiplicative property of $\chi$ gives 

$$
\sum_ {n \mid k} \chi (n) = \prod_ {j = 1} ^ {N} \left(\chi (1) + \chi (p _ {j}) + \chi (p _ {j} ^ {2}) + \dots + \chi (p _ {j} ^ {a _ {j}})\right),
$$

and the proof is complete. 

To prove the second statement in the proposition, we write 

$$
S _ {N} = S _ {I} + (S _ {I I} + S _ {I I I}),
$$

where the sums $S _ { I } , S _ { I I }$ , and $S _ { I I I }$ were defined earlier (see also Figure 3). We evaluate $S _ { I }$ by summing vertically, and $S _ { I I } + S _ { I I I }$ by summing horizontally. In order to carry this out we need the following simple results. 

Lemma 3.15 For all integers $0 < a < b$ we have 

$$
\mathrm{(i)} \sum_ {n = a} ^ {b} \frac {\chi (n)}{n ^ {1 / 2}} = O (a ^ {- 1 / 2}),
$$

$$
\mathrm{(ii)} \sum_ {n = a} ^ {b} \frac {\chi (n)}{n} = O (a ^ {- 1}).
$$

Proof. This argument is similar to the proof of Proposition 3.4; we use summation by parts. Let $\begin{array} { r } { s _ { n } = \sum _ { 1 \leq k \leq n } \chi ( k ) } \end{array}$ , and remember that $\left. s _ { n } \right. \leq q$ for all n. Then 

$$
\begin{array}{c} \sum_ {n = a} ^ {b} \frac {\chi (n)}{n ^ {1 / 2}} = \sum_ {n = a} ^ {b - 1} s _ {n} \left[ n ^ {- 1 / 2} - (n + 1) ^ {- 1 / 2} \right] + O (a ^ {- 1 / 2}) \\ = O \left(\sum_ {n = a} ^ {\infty} n ^ {- 3 / 2}\right) + O (a ^ {- 1 / 2}). \end{array}
$$

By comparing the sum $\scriptstyle \sum _ { n = a } ^ { \infty } n ^ { - 3 / 2 }$ with the integral of $f ( x ) = x ^ { - 3 / 2 }$ we find that the former is also $O ( a ^ { - 1 / 2 } )$ 

A similar argument establishes (ii). 

We may now finish the proof of the proposition. Summing vertically we find 

$$
S _ {I} = \sum_ {m <   N ^ {1 / 2}} \frac {1}{m ^ {1 / 2}} \left(\sum_ {N ^ {1 / 2} <   n \leq N / m} \chi (n) / n ^ {1 / 2}\right).
$$

The lemma together with Proposition 3.11 shows that $S _ { I } = O ( 1 )$ . Finally 

## 4. Exercises

we sum horizontally to get 

$$
\begin{array}{l} S _ {I I} + S _ {I I I} = \sum_ {1 \leq n \leq N ^ {1 / 2}} \frac {\chi (n)}{n ^ {1 / 2}} \left(\sum_ {m \leq N / n} 1 / m ^ {1 / 2}\right) \\ = \sum_ {1 \leq n \leq N ^ {1 / 2}} \frac {\chi (n)}{n ^ {1 / 2}} \left\{2 (N / n) ^ {1 / 2} + c + O ((n / N) ^ {1 / 2}) \right\} \\ = 2 N ^ {1 / 2} \sum_ {1 \leq n \leq N ^ {1 / 2}} \frac {\chi (n)}{n} + c \sum_ {1 \leq n \leq N ^ {1 / 2}} \frac {\chi (n)}{n ^ {1 / 2}} \\ \quad + O \left(\frac {1}{N ^ {1 / 2}} \sum_ {1 \leq n \leq N ^ {1 / 2}} 1\right) \\ = A + B + C. \end{array}
$$

Now observe that the lemma, together with the definition of $L ( s , \chi )$ 2 implies 

$$
A = 2 N ^ {1 / 2} L (1, \chi) + O (N ^ {1 / 2} N ^ {- 1 / 2}).
$$

Moreover, part (i) of the lemma gives $B = O ( 1 )$ , and we also clearly have $C = O ( 1 )$ . Thus $S _ { N } = 2 N ^ { 1 / 2 } L ( 1 , \chi ) + O ( 1 )$ , which is part (ii) in Proposition 3.13. 

This completes the proof that $L ( 1 , \chi ) \neq 0$ , and thus the proof of Dirichlet’s theorem. 

## 4 Exercises

1. Prove that there are infinitely many primes by observing that if there were only finitely many, $p _ { 1 } , \ldots , p _ { N }$ , then 

$$
\prod_ {j = 1} ^ {N} \frac {1}{1 - 1 / p _ {j}} \geq \sum_ {n = 1} ^ {\infty} \frac {1}{n}.
$$

2. In the text we showed that there are infinitely many primes of the form $4 k + 3$ by a modification of Euclid’s original argument. Adapt this technique to prove the similar result for primes of the form $3 k + 2$ , and for those of the form $6 k + 5$ 

3. Prove that if $p$ and $q$ are relatively prime, then $\mathbb { Z } ^ { * } ( p ) \times \mathbb { Z } ^ { * } ( q )$ is isomorphic to $\mathbb { Z } ^ { \ast } ( p q )$ 

4. Let $\varphi ( n )$ denote the number of positive integers $\leq n$ that are relatively prime to n. Use the previous exercise to show that if n and m are relatively prime, then 

$$
\varphi (n m) = \varphi (n) \varphi (m).
$$

One can give a formula for the Euler phi-function as follows: 

(a) Calculate $\varphi ( p )$ when $p$ is prime by counting the number of elements in $\mathbb { Z } ^ { \ast } ( p )$ 

(b) Give a formula for $\varphi ( p ^ { k } )$ when $p$ is prime and $k \geq 1$ by counting the number of elements in $\mathbb { Z } ^ { * } ( p ^ { k } )$ 

(c) Show that 

$$
\varphi (n) = n \prod_ {i} \left(1 - \frac {1}{p _ {i}}\right),
$$

where $p _ { i }$ are the primes that divide $n .$ 

5. If n is a positive integer, show that 

$$
n = \sum_ {d | n} \varphi (d),
$$

where $\varphi$ is the Euler phi-function. 

[Hint: There are precisely $\varphi ( n / d )$ integers $1 \leq m \leq$ n with $\operatorname* { g c d } ( m , n ) = d . ]$ 

6. Write down the characters of the groups $\mathbb { Z } ^ { \ast } ( 3 ) , \ \mathbb { Z } ^ { \ast } ( 4 ) , \ \mathbb { Z } ^ { \ast } ( 5 ) , \ \mathbb { Z } ^ { \ast } ( 6 )$ , and $\mathbb { Z } ^ { \ast } ( 8 )$ 

(a) Which ones are real, or complex? 

(b) Which ones are even, or odd? (A character is even if $\chi ( - 1 ) = 1$ , and odd otherwise). 

7. Recall that for $| z | < 1$ 

$$
\log_ {1} \left(\frac {1}{1 - z}\right) = \sum_ {k \geq 1} \frac {z ^ {k}}{k}.
$$

We have seen that 

$$
e ^ {\log_ {1} \left(\frac {1}{1 - z}\right)} = \frac {1}{1 - z}.
$$

4. Exercises 

(a) Show that if $w = 1 / ( 1 - z )$ , then $| z | < 1$ if and only if $\operatorname { R e } ( w ) > 1 / 2$ 

(b) Show that if $\mathrm { R e } ( w ) > 1 / 2$ and $w = \rho e ^ { i \varphi }$ with $\rho > 0 , | \varphi | < \pi .$ , then 

$$
\log_ {1} w = \log \rho + i \varphi .
$$

[Hint: If $e ^ { \zeta } = w ,$ , then the real part of $\zeta$ is uniquely determined and its imaginary part is determined modulo 2π.] 

8. Let $\zeta$ denote the zeta function defined for $s > 1$ 

(a) Compare ζ(s) with $\int _ { 1 } ^ { \infty } x ^ { - s }$ dx to show that 

$$
\zeta (s) = \frac {1}{s - 1} + O (1) \quad \mathrm{as} s \to 1 ^ {+}.
$$

(b) Prove as a consequence that 

$$
\sum_ {p} \frac {1}{p ^ {s}} = \log \left(\frac {1}{s - 1}\right) + O (1) \quad \mathrm{as} s \to 1 ^ {+}.
$$

9. Let $\chi _ { 0 }$ denote the trivial Dirichlet character mod q, and $p _ { 1 } , \ldots , p _ { k }$ the distinct prime divisors of $q .$ Recall that $L ( s , \chi _ { 0 } ) = ( 1 - p _ { 1 } ^ { - s } ) \cdot \cdot \cdot ( 1 - p _ { k } ^ { - s } ) \zeta ( s )$ , and show as a consequence 

$$
L (s, \chi_ {0}) = \frac {\varphi (q)}{q} \frac {1}{s - 1} + O (1) \quad \mathrm{as} s \to 1 ^ {+}.
$$

[Hint: Use the asymptotics for ζ in Exercise 8.] 

10. Show that if ` is relatively prime to $q ,$ then 

$$
\sum_ {p \equiv \ell} \frac {1}{p ^ {s}} = \frac {1}{\varphi (q)} \log \left(\frac {1}{s - 1}\right) + O (1) \quad \text { as } s \to 1 ^ {+}.
$$

This is a quantitative version of Dirichlet’s theorem. 

[Hint: Recall (4).] 

11. Use the characters for $\mathbb { Z } ^ { \ast } ( 3 ) , \mathbb { Z } ^ { \ast } ( 4 ) , \mathbb { Z } ^ { \ast } ( 5 )$ , and $\mathbb { Z } ^ { \ast } ( 6 )$ to verify directly that $L ( 1 , \chi ) \neq 0$ for all non-trivial Dirichlet characters modulo $q$ when $q = 3 , 4 , 5$ and 6. 

[Hint: Consider in each case the appropriate alternating series.] 

12. Suppose $\chi$ is real and non-trivial; assuming the theorem that $L ( 1 , \chi ) \neq 0$ 2 show directly that $L ( 1 , \chi ) > 0$ 

[Hint: Use the product formula for $L ( s , \chi ) . ]$ 

13. Let $\{ a _ { n } \} _ { n = - \infty } ^ { \infty }$ be a sequence of complex numbers such that $a _ { n } = a _ { m }$ if $n = m$ mod q. Show that the series 

$$
\sum_ {n = 1} ^ {\infty} \frac {a _ {n}}{n}
$$

converges if and only $\begin{array} { r } { \mathrm { i f } \sum _ { n = 1 } ^ { q } a _ { n } = 0 } \end{array}$ 

[Hint: Sum by parts.] 

## 14. The series

$$
F (\theta) = \sum_ {| n | \neq 0} \frac {e ^ {i n \theta}}{n}, \quad \mathrm{for} | \theta | <   \pi ,
$$

converges for every θ and is the Fourier series of the function defined on $[ - \pi , \pi ]$ by $F ( 0 ) = 0$ and 

$$
F (\theta) = \left\{ \begin{array}{c l} i (- \pi - \theta) & \text {if} - \pi \leq \theta <   0 \\ i (\pi - \theta) & \text {if} 0 <   \theta \leq \pi , \end{array} \right.
$$

and extended by periodicity (period 2π) to all of R (see Exercise 8 in Chapter 2). 

$$
\theta \neq 0
$$

$$
E (\theta) = \sum_ {n = 1} ^ {\infty} \frac {e ^ {i n \theta}}{n}
$$

converges, and that 

$$
E (\theta) = \frac {1}{2} \log \left(\frac {1}{2 - 2 \cos \theta}\right) + \frac {i}{2} F (\theta).
$$

15. To sum the series $\textstyle \sum _ { n = 1 } ^ { \infty } a _ { n } / n .$ , with $a _ { n } = a _ { m } { \mathrm { i f } } n = m$ mod q and $\textstyle \sum _ { n = 1 } ^ { q } a _ { n } =$ 0, proceed as follows. 

(a) Define 

$$
A (m) = \sum_ {n = 1} ^ {q} a _ {n} \zeta^ {- m n} \quad \text { where } \zeta = e ^ {2 \pi i / q}.
$$

Note that $A ( q ) = 0$ . With the notation of the previous exercise, prove that 

$$
\sum_ {n = 1} ^ {\infty} \frac {a _ {n}}{n} = \frac {1}{q} \sum_ {m = 1} ^ {q - 1} A (m) E (2 \pi m / q).
$$

[Hint: Use Fourier inversion on $\mathbb { Z } ( q ) . ]$ 

(b) If $\{ a _ { m } \}$ is odd, $\left( a _ { - m } = - a _ { m } \right)$ for $m \in \mathbb { Z } ,$ observe that $a _ { 0 } = a _ { q } = 0$ and show that 

$$
A (m) = \sum_ {1 \leq n <   q / 2} a _ {n} (\zeta^ {- m n} - \zeta^ {m n}).
$$

(c) Still assuming that $\{ a _ { m } \}$ is odd, show that 

$$
\sum_ {n = 1} ^ {\infty} \frac {a _ {n}}{n} = \frac {1}{2 q} \sum_ {m = 1} ^ {q - 1} A (m) F (2 \pi m / q).
$$

[Hint: Define $\begin{array} { r } { \tilde { A } ( m ) = \sum _ { n = 1 } ^ { q } a _ { n } \zeta ^ { m n } } \end{array}$ and apply the Fourier inversion formula.] 

16. Use the previous exercises to show that 

$$
{\frac {\pi}{3 \sqrt {3}}} = 1 - {\frac {1}{2}} + {\frac {1}{4}} - {\frac {1}{5}} + {\frac {1}{7}} - {\frac {1}{8}} + \dots ,
$$

which is $L ( 1 , \chi )$ for the non-trivial (odd) Dirichlet character modulo 3. 

## 5 Problems

1.<sup>∗</sup> Here are other series that can be summed by the methods in Exercise 15. 

(a) For the non-trivial Dirichlet character modulo $6 , L ( 1 , \chi )$ equals 

$$
{\frac {\pi}{2 \sqrt {3}}} = 1 - {\frac {1}{5}} + {\frac {1}{7}} - {\frac {1}{1 1}} + {\frac {1}{1 3}} + \dots .
$$

(b) $\operatorname { I f } \chi$ is the odd Dirichlet character modulo 8, then $L ( 1 , \chi )$ equals 

$$
{\frac {\pi}{2 \sqrt {2}}} = 1 + {\frac {1}{3}} - {\frac {1}{5}} - {\frac {1}{7}} + {\frac {1}{9}} + {\frac {1}{1 1}} \dots .
$$

(c) For an odd Dirichlet character modulo 7, $L ( 1 , \chi )$ equals 

$$
{\frac {\pi}{\sqrt {7}}} = 1 + {\frac {1}{2}} - {\frac {1}{3}} + {\frac {1}{4}} - {\frac {1}{5}} - {\frac {1}{6}} \dots .
$$

(d) For an even Dirichlet character modulo 8, $L ( 1 , \chi )$ equals 

$$
\frac {\log (1 + \sqrt {2})}{\sqrt {2}} = 1 - \frac {1}{3} - \frac {1}{5} + \frac {1}{7} + \frac {1}{9} - \frac {1}{1 1} \dots .
$$

(e) For an even Dirichlet character modulo 5, $L ( 1 , \chi )$ equals 

$$
{\frac {2}{\sqrt {5}}} \log \left({\frac {1 + {\sqrt {5}}}{2}}\right) = 1 - {\frac {1}{2}} - {\frac {1}{3}} + {\frac {1}{4}} + {\frac {1}{6}} - {\frac {1}{7}} - {\frac {1}{8}} + {\frac {1}{9}} + {\frac {1}{1 1}} \dots .
$$

2. Let $d ( k )$ denote the number of positive divisors of $k .$ 

(a) Show that if $k = p _ { 1 } ^ { a _ { 1 } } \cdot \cdot \cdot p _ { n } ^ { a _ { n } }$ is the prime factorization of $k ,$ then 

$$
d (k) = \left(a _ {1} + 1\right) \dots \left(a _ {n} + 1\right).
$$

Although Theorem 3.12 shows that on “average” d(k) is of the order of log $k ,$ , prove the following on the basis of (a): 

(b) $d ( k ) = 2$ for infinitely many $k .$ 

(c) For any positive integer $N ,$ there is a constant $c > 0$ so that $d ( k ) \geq$ $c ( \log k ) ^ { N }$ for infinitely many k. [Hint: Let $p _ { 1 } , \ldots , p _ { N }$ be N distinct primes, and consider k of the form $( p _ { 1 } p _ { 2 } \cdot \cdot \cdot p _ { N } ) ^ { m }$ for $m = 1 , 2 , \ldots ]$ 

3. Show that if $p$ is relatively prime to $q ,$ then 

$$
\prod_ {\chi} \left(1 - \frac {\chi (p)}{p ^ {s}}\right) = \left(\frac {1}{1 - p ^ {f s}}\right) ^ {g},
$$

where $g = \varphi ( q ) / f ,$ and $f$ is the order of $p$ in $\mathbb { Z } ^ { \ast } ( q )$ (that is, the smallest $n$ for which $p ^ { n } \equiv 1$ mod $q )$ . Here the product is taken over all Dirichlet characters modulo q. 

4. Prove as a consequence of the previous problem that 

$$
\prod_ {\chi} L (s, \chi) = \sum_ {n \geq 1} \frac {a _ {n}}{n ^ {s}},
$$

where $a _ { n } \geq 0$ , and the product is over all Dirichlet characters modulo $q .$ 

## Appendix : Integration

This appendix is meant as a quick review of the definition and main properties of the Riemann integral on R, and integration of appropriate continuous functions on $\mathbb { R } ^ { d }$ . Our exposition is brief since we assume that the reader already has some familiarity with this material. 

We begin with the theory of Riemann integration on a closed and bounded interval on the real line. Besides the standard results about the integral, we also discuss the notion of sets of measure 0, and give a necessary and suficient condition on the set of discontinuities of a function that guarantee its integrability. 

We also discuss multiple and repeated integrals. In particular, we extend the notion of integration to the entire space $\mathbb { R } ^ { d }$ by restricting ourselves to functions that decay fast enough at infinity. 

## 1 Definition of the Riemann integral

Let f be a bounded real-valued function defined on the closed interval $[ a , b ] \subset \mathbb { R }$ . By a partition $P$ of $[ a , b ]$ we mean a finite sequence of numbers $x _ { 0 } , x _ { 1 } , \ldots , x _ { N }$ with 

$$
a = x _ {0} <   x _ {1} <   \dots <   x _ {N - 1} <   x _ {N} = b.
$$

Given such a partition, we let $I _ { j }$ denote the interval $[ x _ { j - 1 } , x _ { j } ]$ and write $| I _ { j } |$ for its length, namely $| I _ { j } | = x _ { j } - x _ { j - 1 }$ . We define the upper and lower sums of $f$ with respect to $P$ by 

$$
\mathcal {U} (P, f) = \sum_ {j = 1} ^ {N} \left[ \sup _ {x \in I _ {j}} f (x) \right] | I _ {j} | \quad \text { and } \quad \mathcal {L} (P, f) = \sum_ {j = 1} ^ {N} \left[ \inf _ {x \in I _ {j}} f (x) \right] | I _ {j} |.
$$

Note that the infimum and supremum exist because by assumption, $f$ is bounded. Clearly $\mathcal { U } ( P , f ) \ge \mathcal { L } ( P , f )$ , and the function $f$ is said to be Riemann integrable, or simply integrable, if for every $\epsilon > 0$ there exists a partition $P$ such that 

$$
\mathcal {U} (P, f) - \mathcal {L} (P, f) <   \epsilon .
$$

To define the value of the integral of $f ,$ we need to make a simple yet important observation. A partition $P ^ { \prime }$ is said to be a refinement of the partition $P \operatorname { i f } P ^ { \prime }$ is obtained from $P$ by adding points. Then, adding one point at a time, it is easy to check that 

$$
\mathcal {U} (P ^ {\prime}, f) \leq \mathcal {U} (P, f) \quad \text { and } \quad \mathcal {L} (P ^ {\prime}, f) \geq \mathcal {L} (P, f).
$$

From this, we see that if $P _ { 1 }$ and $P _ { 2 }$ are two partitions of $[ a , b ]$ ， then 

$$
\mathcal {U} (P _ {1}, f) \geq \mathcal {L} (P _ {2}, f),
$$

since it is possible to take $P ^ { \prime }$ as a common refinement of both $P _ { 1 }$ and $P _ { 2 }$ to obtain 

$$
\mathcal {U} (P _ {1}, f) \geq \mathcal {U} (P ^ {\prime}, f) \geq \mathcal {L} (P ^ {\prime}, f) \geq \mathcal {L} (P _ {2}, f).
$$

Since f is bounded we see that both 

$$
U = \inf _ {P} \mathcal {U} (P, f) \quad \text { and } \quad L = \sup _ {P} \mathcal {L} (P, f)
$$

exist (where the infimum and supremum are taken over all partitions of $[ a , b ] )$ , and also that $U \geq L$ . Moreover, if f is integrable we must have $U = L$ , and we define $\textstyle \int _ { a } ^ { b } f ( x )$ dx to be this common value. 

Finally, a bounded complex-valued function $f = u + i v$ is said to be integrable if its real and imaginary parts u and v are integrable, and we define 

$$
\int_ {a} ^ {b} f (x) d x = \int_ {a} ^ {b} u (x) d x + i \int_ {a} ^ {b} v (x) d x.
$$

For example, the constants are integrable functions and it is clear that if $c \in \mathbb { C }$ , then $\textstyle \int _ { a } ^ { b } c d x = c ( b - a )$ . Also, continuous functions are integrable. This is because a continuous function on a closed and bounded interval $[ a , b ]$ is uniformly continuous, that is, given $\epsilon > 0$ there exists δ such that if $| x - y | < \delta$ then $| f ( x ) - f ( y ) | < \epsilon$ . So if we choose n with $( b - a ) / n < \delta _ { \mathrm { f } }$ , then the partition $P$ given by 

$$
a, a + \frac {b - a}{n}, \dots , a + k \frac {b - a}{n}, \dots , a + (n - 1) \frac {b - a}{n}, b
$$

satisfies $\mathcal { U } ( P , f ) - \mathcal { L } ( P , f ) \leq \epsilon ( b - a )$ 

## 1.1 Basic properties

Proposition 1.1 If f and g are integrable on $[ a , b ]$ , then: 

(i) $f + g$ is integrable, and $\textstyle \int _ { a } ^ { b } f ( x ) + g ( x ) d x = \int _ { a } ^ { b } f ( x ) d x + \int _ { a } ^ { b } g ( x ) d x$ 

1. Definition of the Riemann integral 

(ii) $I f c \in \mathbb { C }$ , then $\textstyle \int _ { a } ^ { b } c f ( x ) d x = c \int _ { a } ^ { b } f ( x ) d x$ 

(iii) $_ { I f } \textit { f }$ and g are real-valued and $f ( x ) \leq g ( x )$ , then $\textstyle \int _ { a } ^ { b } f ( x )$ dx $\begin{array} { r } { \leq \int _ { a } ^ { b } g ( x ) } \end{array}$ dx. 

(iv) $\boldsymbol { I f c } \in [ a , b ]$ , then $\textstyle { \int _ { a } ^ { b } f ( x ) d x = \int _ { a } ^ { c } f ( x ) d x + \int _ { c } ^ { b } f ( x ) d x } .$ 

Proof. For property (i) we may assume that $f$ and $g$ are real-valued. If $P$ is a partition of $[ a , b ]$ , then 

$$
\mathcal {U} (P, f + g) \leq \mathcal {U} (P, f) + \mathcal {U} (P, g) \quad \text { and } \quad \mathcal {L} (P, f + g) \geq \mathcal {L} (P, f) + \mathcal {L} (P, g).
$$

Given $\epsilon > 0 .$ , there exist partitions $P _ { 1 }$ and $P _ { 2 }$ such that $\mathcal { U } ( P _ { 1 } , f ) - \mathcal { L } ( P _ { 1 } , f ) <$ ² and $\mathcal { U } ( P _ { 2 } , g ) - \mathcal { L } ( P _ { 2 } , g ) < \epsilon _ { : }$ so that if $P _ { 0 }$ is a common refinement of $P _ { 1 }$ and $P _ { 2 }$ , we get 

$$
\mathcal {U} (P _ {0}, f + g) - \mathcal {L} (P _ {0}, f + g) <   2 \epsilon .
$$

So $f + g$ is integrable, and if we let $\begin{array} { r } { I = \operatorname* { i n f } _ { P } \mathcal { U } ( P , f + g ) = \operatorname* { s u p } _ { P } \mathcal { L } ( P , f + } \end{array}$ $g )$ , then we see that 

$$
\begin{array}{l} I \leq \mathcal {U} (P _ {0}, f + g) + 2 \epsilon \leq \mathcal {U} (P _ {0}, f) + \mathcal {U} (P _ {0}, g) + 2 \epsilon \\ \leq \int_ {a} ^ {b} f (x)   d x + \int_ {a} ^ {b} g (x)   d x + 4 \epsilon . \end{array}
$$

Similarly $\begin{array} { r } { I \geq \int _ { a } ^ { b } f ( x ) d x + \int _ { a } ^ { b } g ( x ) d x - 4 \epsilon } \end{array}$ , which proves that $\textstyle \int _ { a } ^ { b } f ( x ) +$ $\begin{array} { r } { g ( x ) d x = \int _ { a } ^ { b } f ( x ) d x + \int _ { a } ^ { b } g ( x ) d x } \end{array}$ . The second and third parts of the proposition are just as easy to prove. For the last property, simply refine partitions of $[ a , b ]$ by adding the point c. 

Another important property we need to prove is that $f g$ is integrable whenever f and g are integrable. 

Lemma 1.2 If f is real-valued integrable on $[ a , b ]$ and $\varphi$ is a real-valued continuous function on $\mathbb { R } _ { . }$ , then $\varphi \circ f$ is also integrable on $[ a , b ]$ 

Proof. Let $\epsilon > 0$ and remember that $f$ is bounded, say $| f | \leq M$ . Since $\varphi$ is uniformly continuous on $[ - M , M ]$ we may choose $\delta > 0$ so that if $s , t \in [ - M , M ]$ and $| s - t | < \delta ,$ , then $| \varphi ( s ) - \varphi ( t ) | < \epsilon$ . Now choose a partition $P = \{ x _ { 0 } , \ldots , x _ { N } \}$ of $[ a , b ]$ with $\mathcal { U } ( P , f ) - \mathcal { L } ( P , f ) < \delta ^ { 2 }$ . Let $I _ { j } =$ $[ x _ { j - 1 } , x _ { j } ]$ and distinguish two classes: we write $j \in \Lambda { \mathrm { ~ i f ~ } } \operatorname* { s u p } _ { x \in I _ { j } } f ( x ) -$ $\textstyle \operatorname* { i n f } _ { x \in I _ { j } } f ( x ) < \delta$ so that by construction 

$$
\sup _ {x \in I _ {j}} \varphi \circ f (x) - \inf _ {x \in I _ {j}} \varphi \circ f (x) <   \epsilon .
$$

Otherwise, we write $j \in \Lambda ^ { \prime }$ and note that 

$$
\delta \sum_ {j \in \Lambda^ {\prime}} | I _ {j} | \leq \sum_ {j \in \Lambda^ {\prime}} \left[ \sup _ {x \in I _ {j}} f (x) - \inf _ {x \in I _ {j}} f (x) \right] | I _ {j} | \leq \delta^ {2}
$$

so $\textstyle \sum _ { j \in \Lambda ^ { \prime } } \left| I _ { j } \right| < \delta$ . Therefore, separating the cases $j \in \Lambda$ and $j \in \Lambda ^ { \prime }$ we find that 

$$
\mathcal {U} (P, \varphi \circ f) - \mathcal {L} (P, \varphi \circ f) \leq \epsilon (b - a) + 2 \mathcal {B} \delta ,
$$

where $\boldsymbol { B }$ is a bound for $\varphi$ on $[ - M , M ]$ . Since we can also choose $\delta < \epsilon .$ we see that the proposition is proved. 

¿From the lemma we get the following facts: 

• If $f$ and $g$ are integrable on $[ a , b ]$ , then the product $f g$ is integrable on $[ a , b ]$ 

This follows from the lemma with $\varphi ( t ) = t ^ { 2 }$ , and the fact that $f g =$ $\begin{array} { l c r } { { \frac 1 4 } } \left( { [ f + g ] ^ { 2 } - [ f - g ] ^ { 2 } } \right)  \end{array}$ 

• If f is integrable on $[ a , b ]$ , then the function $| f |$ is integrable, and $\textstyle \left| \int _ { a } ^ { b } f ( x ) d x \right| \leq \int _ { a } ^ { b } | f ( x ) | d x$ 

We can take $\varphi ( t ) = | t |$ to see that $| f |$ is integrable. Moreover, the inequality follows from (iii) in Proposition 1.1. 

We record two results that imply integrability. 

Proposition 1.3 A bounded monotonic function f on an interval $[ a , b ]$ is integrable. 

Proof. We may assume without loss of generality that $a = 0 , b = 1$ and $f$ is monotonically increasing. Then, for each $N$ , we choose the uniform partition $P _ { N }$ given by $x _ { j } = j / N$ for all $j = 0 , \ldots , N$ . If $\alpha _ { j } =$ $f ( x _ { j } )$ , then we have 

$$
\mathcal {U} (P _ {N}, f) = \frac {1}{N} \sum_ {j = 1} ^ {N} \alpha_ {j} \quad \text { and } \quad \mathcal {L} (P _ {N}, f) = \frac {1}{N} \sum_ {j = 1} ^ {N} \alpha_ {j - 1}.
$$

Therefore, ${ \mathrm { i f ~ } } | f ( x ) | \leq B$ for all x we have 

$$
\mathcal {U} (P _ {N}, f) - \mathcal {L} (P _ {N}, f) = \frac {\alpha_ {N} - \alpha_ {0}}{N} \leq \frac {2 B}{N},
$$

and the proposition is proved. 

Proposition 1.4 Let f be a bounded function on the compact interval [a, b]. $I f c \in ( a , b )$ , and if for all small $\delta > 0$ the function f is integrable on the intervals $[ a , c - \delta ]$ and $[ c + \delta , b ]$ , then f is integrable on $[ a , b ]$ 

Proof. Suppose $| f | \leq M$ and let $\epsilon > 0$ . Choose $\delta > 0$ (small) so that $4 \delta M \le \epsilon / 3$ . Now let $P _ { 1 }$ and $P _ { 2 }$ be partitions of $[ a , c - \delta ]$ and [c + $\delta , b ]$ so that for each $i = 1 , 2$ we have $\mathcal { U } ( P _ { i } , f ) - \mathcal { L } ( P _ { i } , f ) < \epsilon / 3$ . This is possible since $f$ is integrable on each one of the intervals. Then by taking as a partition $P = P _ { 1 } \cup \{ c - \delta \} \cup \{ c + \delta \} \cup P _ { 2 }$ we immediately see that $\mathcal { U } ( P , f ) - \mathcal { L } ( P , f ) < \epsilon$ 

We end this section with a useful approximation lemma. Recall that a function on the circle is the same as a 2π-periodic function on R. 

Lemma 1.5 Suppose f is integrable on the circle and f is bounded by B. Then there exists a sequence $\{ f _ { k } \} _ { k = 1 } ^ { \infty }$ of continuous functions on the circle so that 

$$
\sup _ {x \in [ - \pi , \pi ]} | f _ {k} (x) | \leq B \quad \text {   for   all   } k = 1, 2, \ldots ,
$$

and 

$$
\int_ {- \pi} ^ {\pi} | f (x) - f _ {k} (x) | d x \rightarrow 0 \quad a s k \rightarrow \infty .
$$

Proof. Assume f is real-valued (in general apply the following argument to the real and imaginary parts separately). Given $\epsilon > 0$ , we may choose a partition $- \pi = x _ { 0 } < x _ { 1 } < \dots < x _ { N } = \pi$ of the interval $[ - \pi , \pi ]$ so that the upper and lower sums of $f$ difer by at most ². Denote by $f ^ { * }$ the step function defined by 

$$
f ^ {*} (x) = \sup _ {x _ {j - 1} \leq y \leq x _ {j}} f (y) \quad \text { if } x \in [ x _ {j - 1}, x _ {j}) \text { for } 1 \leq j \leq N.
$$

By construction we have $| f ^ { * } | \le B$ , and moreover 

$$
\int_ {- \pi} ^ {\pi} | f ^ {*} (x) - f (x) | d x = \int_ {- \pi} ^ {\pi} (f ^ {*} (x) - f (x)) d x <   \epsilon .\tag{1}
$$

Now we can modify $f ^ { * }$ to make it continuous and periodic yet still approximate $f$ in the sense of the lemma. For small $\delta > 0$ , let $\tilde { f } ( x ) = f ^ { * } ( \tilde { x } )$ when the distance of x from any of the division points $x _ { 0 } , \ldots , x _ { N }$ is $\ge \delta .$ . In the δ-neighborhood of $x _ { j }$ for $j = 1 , \ldots , N - 1$ , define $\tilde { f } ( x )$ to be the linear function for which $\tilde { f } ( x _ { j } \pm \delta ) = f ^ { * } ( x _ { j } \pm \delta )$ . Near $x _ { 0 } = - \pi$ , <sup>˜</sup>f is linear with $\tilde { f } ( - \pi ) = 0$ and $\tilde { f } ( - \pi + \delta ) = f ^ { * } ( - \pi + \delta )$ . Similarly, near $x _ { N } = \pi$ the function $\tilde { f }$ is linear with $\tilde { f } ( \pi ) = 0$ and $\tilde { f } ( \pi - \delta ) = f ^ { * } ( \pi - \delta )$ In Figure 1 we illustrate the situation near $x _ { 0 } = - \pi$ . In the second picture the graph of $\tilde { f }$ is shifted slightly below to clarify the situation. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/2ab5d4b2-da28-455b-b554-908156ef0c8e/511b1005101d046730047eb366c37406af8f15924d4ca6cc5516a44e836185ef.jpg)



Figure 1. Portions of the functions $f ^ { * }$ and $\tilde { f }$


Then, since $\tilde { f } ( - \pi ) = \tilde { f } ( \pi )$ , we may extend $\tilde { f }$ to a continuous and $2 \pi \cdot$ periodic function on R. The absolute value of this extension is also bounded by B. Moreover, $\tilde { f }$ difers from $f ^ { * }$ only in the N intervals of length 2δ surrounding the division points. Thus 

$$
\int_ {- \pi} ^ {\pi} | f ^ {*} (x) - \tilde {f} (x) | d x \leq 2 B N (2 \delta).
$$

If we choose δ suficiently small, we get 

$$
\int_ {- \pi} ^ {\pi} | f ^ {*} (x) - \tilde {f} (x) | d x <   \epsilon .\tag{2}
$$

As a result, equations (1), (2), and the triangle inequality yield 

$$
\int_ {- \pi} ^ {\pi} | f (x) - \tilde {f} (x) | d x <   2 \epsilon .
$$

Denoting by $f _ { k }$ the $\tilde { f }$ so constructed, when $2 \epsilon = 1 / k$ , we see that the sequence $\{ f _ { k } \}$ has the properties required by the lemma. 

## 1.2 Sets of measure zero and discontinuities of integrable functions

We observed that all continuous functions are integrable. $\mathrm { B y }$ modifying the argument slightly, one can show that all piecewise continuous functions are also integrable. In fact, this is a consequence of Proposition 1.4 

## 1. Definition of the Riemann integral

applied finitely many times. We now turn to a more careful study of the discontinuities of integrable functions. 

We start with a definition<sup>1</sup>: a subset E of R is said to have measure 0 if for every $\epsilon > 0$ there exists a countable family of open intervals $\{ I _ { k } \} _ { k = 1 } ^ { \infty }$ such that 

(i) $E \subset \bigcup _ { k = 1 } ^ { \infty } I _ { k } ,$ 

(ii) $\textstyle \sum _ { k = 1 } ^ { \infty } | I _ { k } | < \epsilon$ , where $\left| I _ { k } \right|$ denotes the length of the interval $I _ { k }$ 

The first condition says that the union of the intervals covers E, and the second that this union is small. The reader will have no dificulty proving that any finite set of points has measure 0. A more subtle argument is needed to prove that a countable set of points has measure 0. In fact, this result is contained in the following lemma. 

Lemma 1.6 The union of countably many sets of measure 0 has measure 0. 

Proof. Say $E _ { 1 } , E _ { 2 } , \ldots$ . are sets of measure 0, and let $E = \cup _ { i = 1 } ^ { \infty } E _ { i }$ . Let $\epsilon > 0$ , and for each i choose open interval $I _ { i , 1 } , I _ { i , 2 } , \ldots$ . so that 

$$
E _ {i} \subset \bigcup_ {k = 1} ^ {\infty} I _ {i, k} \quad \mathrm{and} \quad \sum_ {k = 1} ^ {\infty} | I _ {i, k} | <   \epsilon / 2 ^ {i}.
$$

Now clearly we have $E \subset \cup _ { i , k = 1 } ^ { \infty } I _ { i , k }$ , and 

$$
\sum_ {i = 1} ^ {\infty} \sum_ {k = 1} ^ {\infty} | I _ {i, k} | \leq \sum_ {i = 1} ^ {\infty} \frac {\epsilon}{2 ^ {i}} \leq \epsilon ,
$$

as was to be shown. 

An important observation is that if E has measure 0 and is compact, then it is possible to find a finite number of open intervals $I _ { k }$ $k = 1 , \ldots , N$ , that satisfy the two conditions (i) and (ii) above. 

We can prove the characterization of Riemann integrable functions in terms of their discontinuities. 

Theorem 1.7 A bounded function f on $[ a , b ]$ is integrable if and only if its set of discontinuities has measure 0. 

We write $J = [ a , b ]$ and $I ( c , r ) = ( c - r , c + r )$ for the open interval centered at c of radius $r > 0$ . Define the oscillation of $f$ on $I ( c , r )$ by 

$$
\operatorname{osc} (f, c, r) = \sup | f (x) - f (y) |
$$

where the supremum is taken over all $x , y \in J \cap I ( c , r )$ . This quantity exists since $f$ is bounded. Define the oscillation of $f$ at c by 

$$
\operatorname{osc} (f, c) = \lim _ {r \to 0} \operatorname{osc} (f, c, r).
$$

This limit exists because osc $( f , c , r )$ is $\geq 0$ and a decreasing function of $r .$ . The point is that $f$ is continuous at c if and only if osc $( f , c ) = 0$ . This is clear from the definitions. For each $\epsilon > 0$ we define a set $A _ { \epsilon }$ <sub>²</sub> by 

$$
A _ {\epsilon} = \{c \in J: \mathrm{osc} (f, c) \geq \epsilon \}.
$$

Having done that, we see that the set of points in $J$ where $f$ is discontinuous is simply $\cup _ { \epsilon > 0 } A _ { \epsilon }$ . This is an important step in the proof of our theorem. 

Lemma 1.8 $I f \epsilon > 0$ , then the set $A _ { \epsilon }$ is closed and therefore compact. 

Proof. The argument is simple. Suppose $c _ { n } \in A _ { \epsilon }$ converges to $c$ and assume that $c \notin A _ { \epsilon }$ . Write osc $( f , c ) = \epsilon - \delta$ where $\delta > 0$ . Select $r$ so that osc $( f , c , r ) < \epsilon - \delta / 2$ , and choose n with $| c _ { n } - c | < r / 2$ . Then $\mathrm { o s c } ( f , c _ { n } , r / 2 ) < \epsilon$ which implies osc $( f , c _ { n } ) < \epsilon ,$ a contradiction. 

We are now ready to prove the first part of the theorem. Suppose that the set D of discontinuities of $f$ has measure $0 ,$ and let $\epsilon > 0$ Since $A _ { \epsilon } \subset \mathcal { D }$ , we can cover $A _ { \epsilon }$ by a finite number of open intervals, say $I _ { 1 } , \ldots , I _ { N }$ , whose total length is $< \epsilon .$ . The complement of this union I of intervals is compact, and around each point z in this complement we can find an interval $F _ { z }$ with su $\begin{array} { r } { \mathrm { p } _ { x , y \in F _ { z } } | f ( x ) - f ( y ) | \le \epsilon , } \end{array}$ , simply because $z \not \in A _ { \epsilon }$ . We may now choose a finite subcovering of $\cup _ { z \in I ^ { c } } I _ { z } .$ , which we denote by $I _ { N + 1 } , \ldots , I _ { N ^ { \prime } }$ . Now, taking all the end points of the intervals $I _ { 1 } , I _ { 2 } , \ldots , I _ { N ^ { \prime } }$ we obtain a partition $P$ of $[ a , b ]$ with 

$$
\mathcal {U} (P, f) - \mathcal {L} (P, f) \leq 2 M \sum_ {j = 1} ^ {N} | I _ {j} | + \epsilon (b - a) \leq C \epsilon .
$$

Hence $f$ is integrable on $[ a , b ]$ , as was to be shown. 

Conversely, suppose that $f$ is integrable on $[ a , b ]$ , and let $\mathcal { D }$ be its set of discontinuities. Since D equals $\cup _ { n = 1 } ^ { \infty } A _ { 1 / n }$ , it sufices to prove 

## 2. Multiple integrals

that each $A _ { 1 / n }$ has measure 0. Let $\epsilon > 0$ and choose a partition $P =$ $\{ x _ { 0 } , x _ { 1 } , \ldots , x _ { N } \}$ so that $\mathcal { U } ( P , f ) - \mathcal { L } ( P , f ) < \epsilon / n$ . Then, if $A _ { 1 / n }$ intersects $I _ { j } = ( x _ { j - 1 } , x _ { j } )$ we must have $\begin{array} { r } { \operatorname* { s u p } _ { x \in I _ { j } } f ( x ) - \operatorname* { i n f } _ { x \in I _ { j } } f ( x ) \geq 1 / n } \end{array}$ , and this shows that 

$$
\frac {1}{n} \sum_ {\{j: I _ {j} \cap A _ {1 / n} \neq \emptyset \}} | I _ {j} | \leq \mathcal {U} (P, f) - \mathcal {L} (P, f) <   \epsilon / n.
$$

So by taking intervals intersecting $A _ { 1 / n }$ and making them slightly larger, we can cover $A _ { 1 / n }$ with open intervals of total length $\leq 2 \epsilon$ . Therefore $A _ { 1 / n }$ has measure 0, and we are done. 

Note that incidentally, this gives another proof that $f g$ is integrable whenever $f$ and g are. 

## 2 Multiple integrals

We assume that the reader is familiar with the standard theory of multiple integrals of functions defined on bounded sets. Here, we give a quick review of the main definitions and results of this theory. Then, we describe the notion of “improper” multiple integration where the range of integration is extended to all of $\mathbb { R } ^ { d }$ . This is relevant to our study of the Fourier transform. In the spirit of Chapters 5 and 6, we shall define the integral of functions that are continuous and satisfy an adequate decay condition at infinity. 

Recall that the vector space $\mathbb { R } ^ { d }$ consists of all d-tuples of real numbers $\boldsymbol { x } = \left( x _ { 1 } , x _ { 2 } , \ldots , x _ { d } \right)$ with $x _ { j } \in \mathbb { R }$ , where addition and multiplication by scalars are defined componentwise. 

## 2.1 The Riemann integral in $\mathbb { R } ^ { d }$

## Definitions

The notion of Riemann integration on a rectangle $R \subset \mathbb { R } ^ { d }$ is an immediate generalization of the notion of Riemann integration on an interval $[ a , b ] \subset \mathbb { R }$ . We restrict our attention to continuous functions; these are always integrable. 

By a closed rectangle in $\mathbb { R } ^ { d }$ , we mean a set of the form 

$$
R = \left\{a _ {j} \leq x _ {j} \leq b _ {j}: 1 \leq j \leq d \right\}
$$

$$
R = \left[ a _ {1}, b _ {1} \right] \times \dots \times \left[ a _ {d}, b _ {d} \right].
$$

where $a _ { j } , b _ { j } \in \mathbb { R }$ for $1 \leq j \leq n$ . In other words, R is the product of the one-dimensional intervals $[ a _ { j } , b _ { j } ]$ : 

If $P _ { j }$ is a partition of the closed interval $[ a _ { j } , b _ { j } ]$ , then we call $P = ( P _ { 1 } , \ldots , P _ { d } )$ a partition of $R ;$ and if $S _ { j }$ is a subinterval of the partition $P _ { j }$ , then $S = S _ { 1 } \times \cdots \times S _ { d }$ is a subrectangle of the partition $P .$ The volume |S| of a subrectangle $S$ is naturally given by the product of the length of its sides $| S | = | S _ { 1 } | \times \cdots \times | S _ { d } |$ , where $\vert S _ { j } \vert$ denotes the length of the interval $S _ { j }$ 

We are now ready to define the notion of integral over $R .$ Given a bounded real-valued function $f$ defined on R and a partition $P ,$ , we define the upper and lower sums of $f$ with respect to $P$ by 

$$
\mathcal {U} (P, f) = \sum [ \sup _ {x \in S} f (x) ] | S | \quad \text { and } \quad \mathcal {L} (P, f) = \sum [ \inf _ {x \in S} f (x) ] | S |,
$$

where the sums are taken over all subrectangles of the partition $P .$ These definitions are direct generalizations of the analogous notions in one dimension. 

A partition $P ^ { \prime } = ( P _ { 1 } ^ { \prime } , \ldots , P _ { d } ^ { \prime } )$ is a refinement of $P = ( P _ { 1 } , \ldots , P _ { d } )$ if each $P _ { j } ^ { \prime }$ is a refinement of $P _ { j }$ . Arguing with these refinements as we did in the one-dimensional case, we see that if we define 

$$
U = \inf _ {P} \mathcal {U} (P, f) \quad \text { and } \quad L = \sup _ {P} \mathcal {L} (P, f),
$$

then both $U$ and $L$ exist, are finite, and $U \geq L$ . We say that $f$ is Riemann integrable on R if for every $\epsilon > 0$ there exists a partition $P$ so that 

$$
\mathcal {U} (P, f) - \mathcal {L} (P, f) <   \epsilon .
$$

This implies that $U = L$ , and this common value, which we shall denote by either 

$$
\int_ {R} f (x _ {1}, \ldots , x _ {d}) d x _ {1} \cdot \cdot \cdot d x _ {d}, \quad \int_ {R} f (x) d x, \quad \mathrm{or} \quad \int_ {R} f,
$$

is by definition the integral of $f$ over $R .$ . If $f$ is complex-valued, say $f ( x ) = u ( x ) + i v ( x )$ , where u and v are real-valued, we naturally define 

$$
\int_ {R} f (x) d x = \int_ {R} u (x) d x + i \int_ {R} v (x) d x.
$$

In the results that follow, we are primarily interested in continuous functions. Clearly, if $f$ is continuous on a closed rectangle R then $f$ is integrable since it is uniformly continuous on R. Also, we note that if $f$ is continuous on, say, a closed ball $B _ { ; }$ , then we may define its integral 

## 2. Multiple integrals

over B in the following way: if g is the extension of f defined by $g ( x ) = 0$ if x $\notin B ,$ then $g$ is integrable on any rectangle R that contains $B ,$ , and we may set 

$$
\int_ {B} f (x) d x = \int_ {R} g (x) d x.
$$

## 2.2 Repeated integrals

The fundamental theorem of calculus allows us to compute many one dimensional integrals, since it is possible in many instances to find an antiderivative for the integrand. In $\mathbb { R } ^ { d }$ , this permits the calculation of multiple integrals, since a d-dimensional integral actually reduces to d one-dimensional integrals. A precise statement describing this fact is given by the following. 

Theorem 2.1 Let f be a continuous function defined on a closed rectangle $R \subset \mathbb { R } ^ { d }$ . Suppose $R = R _ { 1 } \times R _ { 2 }$ where $R _ { 1 } \subset \mathbb { R } ^ { d _ { 1 } }$ and $R _ { 2 } \subset \mathbb { R } ^ { d _ { 2 } }$ with $d = d _ { 1 } + d _ { 2 }$ . If we write $\boldsymbol { x } = ( x _ { 1 } , x _ { 2 } )$ with $x _ { i } \in \mathbb { R } ^ { d _ { i } }$ , then $F ( x _ { 1 } ) =$ $\textstyle \int _ { R _ { 2 } } f ( x _ { 1 } , x _ { 2 } )$ dx<sub>2</sub> is continuous on $R _ { 1 }$ , and we have 

$$
\int_ {R} f (x) d x = \int_ {R _ {1}} \left(\int_ {R _ {2}} f (x _ {1}, x _ {2}) d x _ {2}\right) d x _ {1}.
$$

Proof. The continuity of $F$ follows from the uniform continuity of f on R and the fact that 

$$
\left| F \left(x _ {1}\right) - F \left(x _ {1} ^ {\prime}\right) \right| \leq \int_ {R _ {2}} \left| f \left(x _ {1}, x _ {2}\right) - f \left(x _ {1} ^ {\prime}, x _ {2}\right) \right| d x _ {2}.
$$

To prove the identity, let $P _ { 1 }$ and $P _ { 2 }$ be partitions of $R _ { 1 }$ and $R _ { 2 }$ , respectively. If S and $T$ are subrectangles in $P _ { 1 }$ and $P _ { 2 } { \mathrm { . } }$ , respectively, then the key observation is that 

$$
\sup _ {S \times T} f (x _ {1}, x _ {2}) \geq \sup _ {x _ {1} \in S} \left(\sup _ {x _ {2} \in T} f (x _ {1}, x _ {2})\right)
$$

and 

$$
\inf _ {S \times T} f (x _ {1}, x _ {2}) \leq \inf _ {x _ {1} \in S} \left(\inf _ {x _ {2} \in T} f (x _ {1}, x _ {2})\right).
$$

Then, 

$$
\begin{array}{l} \mathcal {U} (P, f) = \sum_ {S, T} [ \sup _ {S \times T} f (x _ {1}, x _ {2}) ]   | S \times T | \\ \qquad \qquad \qquad \geq \sum_ {S} \sum_ {T} \sup _ {x _ {1} \in S} [ \sup _ {x _ {2} \in T} f (x _ {1}, x _ {2}) ]   | T | \times | S | \\ \qquad \qquad \qquad \geq \sum_ {S} \sup _ {x _ {1} \in S} \left(\int_ {R _ {2}} f (x _ {1}, x _ {2})   d x _ {2}\right) | S | \\ \qquad \qquad \qquad \geq \mathcal {U} \left(P _ {1}, \int_ {R _ {2}} f (x _ {1}, x _ {2})   d x _ {2}\right). \end{array}
$$

Arguing similarly for the lower sums, we find that 

$$
\mathcal {L} (P, f) \leq \mathcal {L} (P _ {1}, \int_ {R _ {2}} f (x _ {1}, x _ {2}) d x _ {2}) \leq \mathcal {U} (P _ {1}, \int_ {R _ {2}} f (x _ {1}, x _ {2}) d x _ {2}) \leq \mathcal {U} (P, f),
$$

and the theorem follows from these inequalities. 

Repeating this argument, we find as a corollary that if f is continuous on the rectangle $R \subset \mathbb { R } ^ { d }$ given by $R = [ a _ { 1 } , b _ { 1 } ] \times \cdot \cdot \cdot [ a _ { d } , b _ { d } ]$ , then 

$$
\int_ {R} f (x) d x = \int_ {a _ {1}} ^ {b _ {1}} \left(\int_ {a _ {2}} ^ {b _ {2}} \dots \left(\int_ {a _ {d}} ^ {b _ {d}} f (x _ {1}, \dots , x _ {d}) d x _ {d}\right) \dots d x _ {2}\right) d x _ {1},
$$

where the right-hand side denotes d-iterates of one-dimensional integrals. It is also clear from the theorem that we can interchange the order of integration in the repeated integral as desired. 

## 2.3 The change of variables formula

A difeomorphism of class $C ^ { 1 } , g : A \to B ;$ , is a mapping that is continuously diferentiable, invertible, and whose inverse $g ^ { - 1 } : B  A$ is also continuously diferentiable. We denote by ${ \cal D } g$ the Jacobian or derivative of $g .$ . Then, the change of variables formula says the following. 

Theorem 2.2 Suppose A and B are compact subsets of $\mathbb { R } ^ { d }$ and $g : A  B$ is a difeomorphism of class $C ^ { 1 }$ . If f is continuous on $B _ { \cdot }$ then 

$$
\int_ {g (A)} f (x) d x = \int_ {A} f (g (y)) | \det (D g) (y) | d y.
$$

The proof of this theorem consists first of an analysis of the special situation when $g$ is a linear transformation L. In this case, if $R$ is a rectangle, then 

$$
| g (R) | = | \det (L) | | R |,
$$

which explains the term $| \operatorname* { d e t } ( D g ) |$ . Indeed, this term corresponds to the new infinitesimal element of volume after the change of variables. 

## 2.4 Spherical coordinates

An important application of the change of variables formula is to the case of polar coordinates in $\mathbb { R } ^ { 2 }$ , spherical coordinates in $\mathbb { R } ^ { 3 }$ , and their generalization in $\mathbb { R } ^ { d }$ . These are particularly important when the function, or set we are integrating over, exhibit some rotational (or spherical) symmetries. The cases $d = 2$ and $d = 3$ were given in Chapter 6. More generally, the spherical coordinates system in $\mathbb { R } ^ { d }$ is given by $x = g ( r , \theta _ { 1 } , \ldots , \theta _ { d - 1 } )$ where 

$$
\left\{ \begin{array}{l l} x _ {1} & = r \sin \theta_ {1} \sin \theta_ {2} \dots \sin \theta_ {d - 2} \cos \theta_ {d - 1}, \\ x _ {2} & = r \sin \theta_ {1} \sin \theta_ {2} \dots \sin \theta_ {d - 2} \sin \theta_ {d - 1}, \\ \vdots \\ x _ {d - 1} & = r \sin \theta_ {1} \sin \theta_ {2}, \\ x _ {d} & = r \cos \theta_ {1}, \end{array} \right.
$$

with $0 \leq \theta _ { i } \leq \pi$ for $1 \leq i \leq d - 2$ and $0 \leq \theta _ { d - 1 } \leq 2 \pi$ . The determinant of the Jacobian of this transformation is given by 

$$
r ^ {d - 1} \sin^ {d - 2} \theta_ {1} \sin^ {d - 3} \theta_ {2} \dots \sin \theta_ {d - 2}.
$$

Any point in $x \in \mathbb { R } ^ { d } - \{ 0 \}$ can be written uniquely as $r \gamma$ with $\gamma \in S ^ { d - 1 }$ the unit sphere in $\mathbb { R } ^ { d }$ . If we define 

$$
\int_ {S ^ {d - 1}} f (\gamma) d \sigma (\gamma) =
$$

$$
\int_ {0} ^ {\pi} \int_ {0} ^ {\pi} \dots \int_ {0} ^ {2 \pi} f (g (r, \theta)) \sin^ {d - 2} \theta_ {1} \sin^ {d - 3} \theta_ {2} \dots \sin \theta_ {d - 2} d \theta_ {d - 1} \dots d \theta_ {1},
$$

then we see that if $B ( 0 , N )$ denotes the ball of radius N centered at the origin, then 

$$
\int_ {B (0, N)} f (x) d x = \int_ {S ^ {d - 1}} \int_ {0} ^ {N} f (r \gamma) r ^ {d - 1} d r d \sigma (\gamma).\tag{3}
$$

In fact, we define the area of the unit sphere $S ^ { d - 1 } \subset \mathbb { R } ^ { d }$ as 

$$
\omega_ {d} = \int_ {S ^ {d - 1}} d \sigma (\gamma).
$$

An important application of spherical coordinates is to the calculation of the integral $\begin{array} { r } { \int _ { A ( R _ { 1 } , R _ { 2 } ) } | x | ^ { \lambda } d x } \end{array}$ , where $A ( R _ { 1 } , R _ { 2 } )$ denotes the annulus 

$A ( R _ { 1 } , R _ { 2 } ) = \{ R _ { 1 } \leq | x | \leq R _ { 2 } \}$ and $\lambda \in \mathbb { R }$ . Applying polar coordinates, we find 

$$
\int_ {A (R _ {1}, R _ {2})} | x | ^ {\lambda} d x = \int_ {S ^ {d - 1}} \int_ {R _ {1}} ^ {R _ {2}} r ^ {\lambda + d - 1} d r d \sigma (\gamma).
$$

Therefore 

$$
\int_ {A (R _ {1}, R _ {2})} | x | ^ {\lambda}   d x = \left\{ \begin{array}{c l} \frac {\omega_ {d}}{\lambda + d} [ R _ {2} ^ {\lambda + d} - R _ {1} ^ {\lambda + d} ] & \text {if} \lambda \neq - d, \\ \omega_ {d} [ \log (R _ {2}) - \log (R _ {1}) ] & \text {if} \lambda = - d. \end{array} \right.
$$

## 3 Improper integrals. Integration over $\mathbb { R } ^ { d }$

Most of the theorems we just discussed extend to functions integrated over all of $\mathbb { R } ^ { d }$ once we impose some decay at infinity on the functions we integrate. 

## 3.1 Integration of functions of moderate decrease

For each fixed $N > 0$ consider the closed cube in $\mathbb { R } ^ { d }$ centered at the origin with sides parallel to the axis, and of side length N: $Q _ { N } = \{ | x _ { j } | \leq N / 2$ : $1 \leq j \leq d \}$ . Let $f$ be a continuous function on $\mathbb { R } ^ { d }$ . If the limit 

$$
\lim _ {N \to \infty} \int_ {Q _ {N}} f (x) d x
$$

exists, we denote it by 

$$
\int_ {\mathbb {R} ^ {d}} f (x) d x.
$$

We deal with a special class of functions whose integrals over $\mathbb { R } ^ { d }$ exist. A continuous function $f$ on $\mathbb { R } ^ { d }$ is said to be of moderate decrease if there exists $A > 0$ such that 

$$
| f (x) | \leq \frac {A}{1 + | x | ^ {d + 1}}.
$$

Note that if $d = 1$ we recover the definition given in Chapter 5. An important example of a function of moderate decrease in R is the Poisson kernel given by $\begin{array} { r } { \mathcal { P } _ { y } ( x ) = \frac { 1 } { \pi } \frac { y } { x ^ { 2 } + y ^ { 2 } } } \end{array}$ 

We claim that if $f$ is of moderate decrease, then the above limit exists. Let $\begin{array} { r } { I _ { N } = \int _ { Q _ { N } } f ( x ) } \end{array}$ dx. Each $I _ { N }$ exists because $f$ is continuous hence integrable. For $M > N$ , we have 

$$
\left| I _ {M} - I _ {N} \right| \leq \int_ {Q _ {M} - Q _ {N}} | f (x) | d x.
$$

## 3. Improper integrals. Integration over $\mathbb { R } ^ { d }$

Now observe that the set $Q _ { M } - Q _ { N }$ is contained in the annulus $A ( a N , b M ) = \{ a N \leq | x | \leq b M \}$ , where a and b are constants that depend only on the dimension $d .$ This is because the cube $Q _ { N }$ is contained in the annulus $N / 2 \leq | x | \leq N \sqrt { d } / 2$ , so that we can take $a = 1 / 2$ and $b = \sqrt { d } / 2$ . Therefore, using the fact that $f$ is of moderate decrease yields 

$$
| I _ {M} - I _ {N} | \leq A \int_ {a N \leq | x | \leq b M} | x | ^ {- d - 1} d x.
$$

Now putting $\lambda = - d - 1$ in the calculation of the integral of the previous section, we find that 

$$
\left| I _ {M} - I _ {N} \right| \leq C \left(\frac {1}{a N} - \frac {1}{b M}\right).
$$

So if f is of moderate decrease, we conclude that $\{ I _ { N } \} _ { N = 1 } ^ { \infty }$ is a Cauchy sequence, and therefore $\textstyle \int _ { \mathbb { R } ^ { d } } f ( x )$ dx exists. 

Instead of the rectangles $Q _ { N }$ , we could have chosen the balls $B _ { N }$ centered at the origin and of radius N. Then, if $f$ is of moderate decrease, the reader should have no dificulties proving that $\begin{array} { r } { \operatorname* { l i m } _ { N \to \infty } \int _ { B _ { N } } f ( x ) } \end{array}$ dx exists, and that this limit equals lim $_ { \cdot N  \infty } \int _ { Q _ { N } } f ( x ) d x$ 

Some elementary properties of the integrals of functions of moderate decrease are summarized in Chapter 6. 

## 3.2 Repeated integrals

In Chapters 5 and 6 we claimed that the multiplication formula held for functions of moderate decrease. This required an appropriate interchange of integration. Similarly for operators defined in terms of convolutions (with the Poisson kernel for example). 

We now justify the necessary formula for iterated integrals. We only consider the case $d = 2$ , although the reader will have no dificulty extending this result to arbitrary dimensions. 

Theorem 3.1 Suppose f is continuous on $\mathbb { R } ^ { 2 }$ and of moderate decrease. Then 

$$
F (x _ {1}) = \int_ {\mathbb {R}} f (x _ {1}, x _ {2}) d x _ {2}
$$

is of moderate decrease on R, and 

$$
\int_ {\mathbb {R} ^ {2}} f (x) d x = \int_ {\mathbb {R}} \left(\int_ {\mathbb {R}} f (x _ {1}, x _ {2}) d x _ {2}\right) d x _ {1}.
$$

Proof. To see why F is of moderate decrease, note first that 

$$
| F (x _ {1}) | \leq \int_ {\mathbb {R}} \frac {A d x _ {2}}{1 + (x _ {1} ^ {2} + x _ {2} ^ {2}) ^ {3 / 2}} \leq \int_ {| x _ {2} | \leq | x _ {1} |} + \int_ {| x _ {2} | \geq | x _ {1} |}.
$$

In the first integral, we observe that the integrand is $\leq A / ( 1 + | x _ { 1 } | ^ { 3 } )$ , so 

$$
\int_ {| x _ {2} | \leq | x _ {1} |} \frac {A d x _ {2}}{1 + (x _ {1} ^ {2} + x _ {2} ^ {2}) ^ {3 / 2}} \leq \frac {A}{1 + | x _ {1} | ^ {3}} \int_ {| x _ {2} | \leq | x _ {1} |} d x _ {2} \leq \frac {A ^ {\prime}}{1 + | x _ {1} | ^ {2}}.
$$

For the second integral, we have 

$$
\int_ {| x _ {2} | \geq | x _ {1} |} \frac {A d x _ {2}}{1 + (x _ {1} ^ {2} + x _ {2} ^ {2}) ^ {3 / 2}} \leq A ^ {\prime \prime} \int_ {| x _ {2} | \geq | x _ {1} |} \frac {d x _ {2}}{1 + | x _ {2} | ^ {3}} \leq \frac {A ^ {\prime \prime \prime}}{| x _ {1} | ^ {2}},
$$

thus $F$ is of moderate decrease. In fact, this argument together with Theorem 2.1 shows that $F$ is the uniform limit of continuous functions, thus is also continuous. 

To establish the identity we simply use an approximation and Theorem 2.1 over finite rectangles. Write $S ^ { c }$ to denote the complement of a set S. Given $\epsilon > 0$ choose N so large that 

$$
\left| \int_ {\mathbb {R} ^ {2}} f (x _ {1}, x _ {2}) d x _ {1} d x _ {2} - \int_ {I _ {N} \times I _ {N}} f (x _ {1}, x _ {2}) d x _ {1} d x _ {2} \right| <   \epsilon ,
$$

where $I _ { N } = [ - N , N ]$ . Now we know that 

$$
\int_ {I _ {N} \times I _ {N}} f (x _ {1}, x _ {2}) d x _ {1} d x _ {2} = \int_ {I _ {N}} \left(\int_ {I _ {N}} f (x _ {1}, x _ {2}) d x _ {2}\right) d x _ {1}.
$$

But this last iterated integral can be written as 

$$
\begin{array}{c} = \int_ {\mathbb {R}} \left(\int_ {\mathbb {R}} f (x _ {1}, x _ {2})   d x _ {2}\right)   d x _ {1} - \int_ {I _ {N} ^ {c}} \left(\int_ {\mathbb {R}} f (x _ {1}, x _ {2})   d x _ {2}\right)   d x _ {1} \\ - \int_ {I _ {N}} \left(\int_ {I _ {N} ^ {c}} f (x _ {1}, x _ {2})   d x _ {2}\right)   d x _ {1}. \end{array}
$$

We can now estimate 

$$
\begin{array}{l} \left| \int_ {I _ {N}} \left(\int_ {I _ {N} ^ {c}} f (x _ {1}, x _ {2})   d x _ {2}\right)   d x _ {1} \right| \leq O \left(\frac {1}{N ^ {2}}\right) \\ \qquad + C \int_ {1 \leq | x _ {1} | \leq N} \left(\int_ {| x _ {2} | \geq N} \frac {d x _ {2}}{(| x _ {1} | + | y _ {1} |) ^ {3}}\right)   d x _ {1} \\ \qquad \leq O \left(\frac {1}{N}\right). \end{array}
$$

3. Improper integrals. Integration over $\mathbb { R } ^ { d }$ 

A similar argument shows that 

$$
\left| \int_ {I _ {N} ^ {\mathrm{c}}} \left(\int_ {\mathbb {R}} f (x _ {1}, x _ {2}) d x _ {2}\right) d x _ {1} \right| \leq \frac {C}{N}.
$$

Therefore, we can find N so large that 

$$
\left| \int_ {I _ {N} \times I _ {N}} f (x _ {1}, x _ {2}) d x _ {1} d x _ {2} - \int_ {\mathbb {R}} \left(\int_ {\mathbb {R}} f (x _ {1}, x _ {2}) d x _ {2}\right) d x _ {1} \right| <   \epsilon ,
$$

and we are done. 

## 3.3 Spherical coordinates

In $\mathbb { R } ^ { d }$ , spherical coordinates are given by $x = r \gamma$ , where $r \geq 0$ and $\gamma$ belongs to the unit sphere $S ^ { d - 1 }$ . If $f$ is of moderate decrease, then for each fixed $\gamma \in S ^ { d - 1 }$ , the function of $f$ given by $f ( r \gamma ) r ^ { d - 1 }$ is also of moderate decrease on R. Indeed, we have 

$$
\left| f (r \gamma) r ^ {d - 1} \right| \leq A \frac {r ^ {d - 1}}{1 + | r \gamma | ^ {d + 1}} \leq \frac {B}{1 + r ^ {2}}.
$$

As a result, by letting $R \to \infty$ in (3) we obtain the formula 

$$
\int_ {\mathbb {R} ^ {d}} f (x) d x = \int_ {S ^ {d - 1}} \int_ {0} ^ {\infty} f (r \gamma) r ^ {d - 1} d r d \sigma (\gamma).
$$

As a consequence, if we combine the fact that 

$$
\int_ {\mathbb {R} ^ {d}} f (R (x)) d x = \int_ {\mathbb {R} ^ {d}} f (x) d x,
$$

whenever R is a rotation, with the identity (3), then we obtain that 

$$
\int_ {S ^ {d - 1}} f (R (\gamma)) d \sigma (\gamma) = \int_ {S ^ {d - 1}} f (\gamma) d \sigma (\gamma).\tag{4}
$$

# Notes and References

Seeley [29] gives an elegant and brief introduction to Fourier series and the Fourier transform. The authoritative text on Fourier series is Zygmund [36]. For further applications of Fourier analysis to a variety of other topics, see Dym and McKean [8] and K¨orner [21]. The reader should also consult the book by Kahane and Lemari´e-Rieusset [20], which contains many historical facts and other results related to Fourier series. 

## Chapter 1

The citation is taken from a letter of Fourier to an unknown correspondent (probably Lagrange), see Herivel [15]. 

More facts about the early history of Fourier series can be found in Sections I-III of Riemann’s memoir [27]. 

## Chapter 2

The quote is a translation of an excerpt in Riemann’s paper [27]. 

For a proof of Littlewood’s theorem (Problem 3), as well as other related “Tauberian theorems,” see Chapter 7 in Titchmarsh [32]. 

## Chapter 3

The citation is a translation of a passage in Dirichlet’s memoir [6]. 

## Chapter 4

The quote is translated from Hurwitz [17]. 

The problem of a ray of light reflecting inside a square is discussed in Chapter 23 of Hardy and Wright [13]. 

The relationship between the diameter of a curve and Fourier coeficients (Problem 1) is explored in Pfluger [26]. 

Many topics concerning equidistribution of sequences, including the results in Problems 2 and 3, are taken up in Kuipers and Niederreiter [22]. 

## Chapter 5

The citation is a free translation of a passage in Schwartz [28]. 

For topics in finance, see Dufie [7], and in particular Chapter 5 for the Black-Scholes theory (Problems 1 and 2). 

The results in Problems 4, 5, and 6 are worked out in John [19] and Widder [34]. 

For Problem 7, see Chapter 2 in Wiener [35]. 

The original proof of the nowhere diferentiability of $f _ { 1 }$ (Problem 8) is in Hardy [12]. 

## Chapter 6

The quote is an excerpt from Cormack’s Nobel Prize lecture [5]. 

More about the wave equation, as well as the results in Problems 3, 4, and 5 can be found in Chapter 5 of Folland [9]. 

A discussion of the relationship between rotational symmetry, the Fourier transform, and Bessel functions is in Chapter 4 of Stein and Weiss [31]. 

For more on the Radon transform, see Chapter 1 in John [18], Helgason [14], and Ludwig [25]. 

## Chapter 7

The citation is taken from Bingham and Tukey [2]. 

Proofs of the structure theorem for finite abelian groups (Problem 2) can be found in Chapter 2 of Herstein [16], Chapter 2 in Lang [23], or Chapter 104 in K¨orner [21]. 

For Problem 4, see Andrews [1], which contains a short proof. 

## Chapter 8

The citation is from Bochner [3]. 

For more on the divisor function, see Chapter 18 in Hardy and Wright [13]. 

Another “elementary” proof that $L ( 1 , \chi ) \neq 0$ can be found in Chapter 3 of Gelfond and Linnik [11]. 

An alternate proof that $L ( 1 , \chi ) \neq 0$ based on algebraic number theory is in Weyl [33]. Also, two other analytic variants of the proof that $L ( 1 , \chi ) \neq 0$ can be found in Chapter 109 in K¨orner [21] and Chapter 6 in Serre [30]. See also the latter reference for Problems 3 and 4. 

## Appendix

Further details about the results on integration reviewed in the appendix can be found in Folland [10] (Chapter 4), Buck [4] (Chapter 4), or Lang [24] (Chapter 20). 

## Bibliography



[1] G. E. Andrews. Number theory. Dover Publications, New York, 1994. Corrected reprint of the 1971 originally published by W.B. Saunders Company. 





[2] C. Bingham and J.W. Tukey. Fourier methods in the frequency analysis of data. The Collected Works of John W Tukey, Volume II Time Series: 1965-1984(Wadsworth Advanced Books & Software), 1984. 





[3] S. Bochner. The role of Mathematics in the Rise of Science. Princeton University Press, Princeton, NJ, 1966. 





[4] R. C. Buck. Advanced Calculus. McGraw-Hill, New York, third edition, 1978. 





[5] A. M. Cormack. Nobel Prize in Physiology and Medicine Lecture, volume Volume 209. Science, 1980. 





[6] G. L. Dirichlet. Sur la convergence des s´eries trigonometriques qui servent `a representer une fonction arbitraire entre des limites donn´ees. Crelle, Journal f¨ur die reine angewandte Mathematik, 4:157–169, 1829. 





[7] D. Dufie. Dynamic Asset Pricing Theory. Princeton University Press, Princeton, NJ, 2001. 





[8] H. Dym and H. P. McKean. Fourier Series and Integrals. Academic Press, New York, 1972. 





[9] G. B. Folland. Introduction to Partial Diferential Equations. Princeton University Press, Princeton, NJ, 1995. 





[10] G. B. Folland. Advanced Calculus. Prentice Hall, Englewood Clifs, NJ, 2002. 





[11] A. O. Gelfond and Yu. V. Linnik. Elementary Methods in Analytic Number Theory. Rand McNally & Compagny, Chicago, 1965. 





[12] G. H. Hardy. Weierstrass’s non-diferentiable function. Transactions, American Mathematical Society, 17:301–325, 1916. 





[13] G. H. Hardy and E. M. Wright. An Introduction to the Theory of Numbers. Oxford University Press, London, fifth edition, 1979. 



## BIBLIOGRAPHY



[14] S. Helgason. The Radon transform on Euclidean spaces, compact two-point homogeneous spaces and Grassman manifolds. Acta. Math., 113:153–180, 1965. 





[15] J. Herivel. Joseph Fourier The Man and the Physicist. Clarendon Press, Oxford, 1975. 





[16] I. N. Herstein. Abstract Algebra. Macmillan, New York, second edition, 1990. 





[17] A. Hurwitz. Sur quelques applications g´eometriques des s´eries de Fourier. Annales de l’Ecole Normale Sup´erieure, 19(3):357–408, 1902. 





[18] F. John. Plane Waves and Spherical Mean Applied to Partial Differential Equations. Interscience Publishers, New York, 1955. 





[19] F. John. Partial Diferential Equations. Springer-Verlag, New York, fourth edition, 1982. 





[20] J.P. Kahane and P. G. Lemari´e-Rieusset. S´eries de Fourier et ondelettes. Cassini, Paris, 1998. English version: Gordon & Breach, 1995. 





[21] T. W. K¨orner. Fourier Analysis. Cambridge University Press, Cambridge, UK, 1988. 





[22] L. Kuipers and H. Niederreiter. Uniform Distribution of Sequences. Wiley, New York, 1974. 





[23] S. Lang. Undergraduate Algebra. Springer-Verlag, New York, second edition, 1990. 





[24] S. Lang. Undergraduate Analysis. Springer-Verlag, New York, second edition, 1997. 





[25] D. Ludwig. The Radon transform on Euclidean space. Comm. Pure Appl. Math., 19:49–81, 1966. 





[26] A. Pfluger. On the diameter of planar curves and Fourier coeficients. Colloquia Mathematica Societatis J´anos Bolyai, Functions, series, operators, 35:957–965, 1983. 





[27] B. Riemann. Ueber die Darstellbarkeit einer Function durch eine trigonometrische Reihe. Habilitation an der Universit¨at zu G¨ottingen, 1854. Collected Works, Springer Verlag, New York, 1990. 





[28] L. Schwartz. Th´eorie des distributions, volume Volume I. Hermann, Paris, 1950. 





[29] R. T. Seeley. An Introduction to Fourier Series and Integrals. W. A. Benjamin, New York, 1966. 





[30] J.P. Serre. A course in Arithmetic. GTM 7. Springer Verlag, New York, 1973. 





[31] E. M. Stein and G. Weiss. Introduction to Fourier Analysis on Euclidean Spaces. Princeton University Press, Princeton, NJ, 1971. 





[32] E. C. Titchmarsh. The Theory of Functions. Oxford University Press, London, second edition, 1939. 





[33] H. Weyl. Algebraic Theory of Numbers, volume Volume 1 of Annals of Mathematics Studies. Princeton University Press, Princeton, NJ, 1940. 





[34] D. V. Widder. The Heat Equation. Academic Press, New York, 1975. 





[35] N. Wiener. The Fourier Integral and Certain of its Applications. Cambridge University Press, Cambridge, UK, 1933. 





[36] A. Zygmund. Trigonometric Series, volume Volumes I and II. Cambridge University Press, Cambridge, UK, second edition, 1959. Reprinted 1993. 



## Symbol Glossary

The page numbers on the right indicate the first time the symbol or notation is defined or used. As usual, Z, Q, R and C denote the integers, the rationals, the reals, and the complex numbers respectively. 

<table><tr><td><eq>\triangle</eq></td><td>Laplacian</td><td>20, 185</td></tr><tr><td><eq>|z|, \overline{z}</eq></td><td>Absolute value and complex conjugate</td><td>22</td></tr><tr><td><eq>e^{z}</eq></td><td>Complex exponential</td><td>24</td></tr><tr><td><eq>\sinh x, \cosh x</eq></td><td>Hyperbolic sine and hyperbolic cosine</td><td>28</td></tr><tr><td><eq>\hat{f}(n), a_{n}</eq></td><td>Fourier coefficient</td><td>34</td></tr><tr><td><eq>f(\theta) \sim \sum a_{n}e^{in\theta}</eq></td><td>Fourier series</td><td>34</td></tr><tr><td><eq>S_{N}(f)</eq></td><td>Partial sum of a Fourier series</td><td>35</td></tr><tr><td><eq>D_{N}, \mathcal{D}_{R}, \tilde{D}_{N}, D_{N}^{*}</eq></td><td>Dirichlet kernel, conjugate, and modified</td><td>37, 95, 165</td></tr><tr><td><eq>P_{r}, \mathcal{P}_{y}, \mathcal{P}_{y}^{(d)}</eq></td><td>Poisson kernels</td><td>37, 149, 210</td></tr><tr><td><eq>O, o</eq></td><td>Big <eq>O</eq> and little <eq>o</eq> notation</td><td>42, 62</td></tr><tr><td><eq>C^{k}</eq></td><td>Functions that are <eq>k</eq> times differentiable</td><td>44</td></tr><tr><td><eq>f * g</eq></td><td>Convolution</td><td>44, 139, 184, 239</td></tr><tr><td><eq>\sigma_{N}, \sigma_{N}(f)</eq></td><td>Cesàro mean</td><td>52, 53</td></tr><tr><td><eq>F_{N}, \mathcal{F}_{R}</eq></td><td>Fejér kernel</td><td>53, 163</td></tr><tr><td><eq>A(r), A_{r}(f)</eq></td><td>Abel mean</td><td>54, 55</td></tr><tr><td><eq>\chi_{[a,b]}</eq></td><td>Characteristic function</td><td>61</td></tr><tr><td><eq>f(\theta^{+}), f(\theta^{-})</eq></td><td>One-sided limits at jump discontinuities</td><td>63</td></tr><tr><td><eq>\mathbb{R}^{d}, \mathbb{C}^{d}</eq></td><td>Euclidean spaces</td><td>71</td></tr><tr><td><eq>X \perp Y</eq></td><td>Orthogonal vectors</td><td>72</td></tr><tr><td><eq>\ell^{2}(\mathbb{Z})</eq></td><td>Square summable sequences</td><td>73</td></tr><tr><td><eq>\mathcal{R}</eq></td><td>Riemann integrable functions</td><td>75</td></tr><tr><td><eq>\zeta(s)</eq></td><td>Zeta function</td><td>98</td></tr><tr><td><eq>[x], \langle x \rangle</eq></td><td>Integer and fractional parts</td><td>106</td></tr><tr><td><eq>\triangle_{N}, \sigma_{N,K}, \tilde{\triangle}_{N}</eq></td><td>Delayed means</td><td>114, 127, 174</td></tr><tr><td><eq>H_{t}, \mathcal{H}_{t}, \mathcal{H}_{t}^{(d)}</eq></td><td>Heat kernels</td><td>120, 146, 209</td></tr><tr><td><eq>\mathcal{M}(\mathbb{R})</eq></td><td>Space of functions of moderate decrease on <eq>\mathbb{R}</eq></td><td>131</td></tr><tr><td colspan="2">304</td><td>SYMBOL GLOSSARY</td></tr><tr><td><eq>\hat{f}(\xi)</eq></td><td>Fourier transform</td><td>134, 181</td></tr><tr><td><eq>\mathcal{S},\mathcal{S}(\mathbb{R}),\mathcal{S}(\mathbb{R}^{d})</eq></td><td>Schwartz space</td><td>134, 180</td></tr><tr><td><eq>\mathbb{R}_{+}^{2},\overline{\mathbb{R}_{+}^{2}}</eq></td><td>Upper half-plane and its closure</td><td>149</td></tr><tr><td><eq>\vartheta(s),\Theta(z|\tau)</eq></td><td>Theta functions</td><td>155, 156</td></tr><tr><td><eq>\Gamma(s)</eq></td><td>Gamma function</td><td>165</td></tr><tr><td><eq>\|x\|, |x|;(x,y), x\cdot y</eq></td><td>Norm and inner product in <eq>\mathbb{R}^{d}</eq></td><td>71, 176</td></tr><tr><td><eq>x^{\alpha}, |\alpha|, (\frac{\partial}{\partial x})^{\alpha}</eq></td><td>Monomial, its order, and differential operator</td><td>176</td></tr><tr><td><eq>S^{1}, S^{2}, S^{d-1}</eq></td><td>Unit circle in <eq>\mathbb{R}^{2}</eq>, and unit spheres in <eq>\mathbb{R}^{3},\mathbb{R}^{d}</eq></td><td>179, 180</td></tr><tr><td><eq>M_{t},\widetilde{M}_{t}</eq></td><td>Spherical mean</td><td>194, 216</td></tr><tr><td><eq>J_{n}</eq></td><td>Bessel function</td><td>197, 213</td></tr><tr><td><eq>\mathcal{P},\mathcal{P}_{t,\gamma}</eq></td><td>Plane</td><td>202</td></tr><tr><td><eq>\mathcal{R},\mathcal{R}^{*}</eq></td><td>Radon and dual Radon transforms</td><td>203, 205</td></tr><tr><td><eq>A_{d}, V_{d}</eq></td><td>Area and volume of the unit sphere in <eq>\mathbb{R}^{d}</eq></td><td>208</td></tr><tr><td><eq>\mathbb{Z}(N)</eq></td><td>Group of <eq>N^{\text{th}}</eq> roots of unity</td><td>219</td></tr><tr><td><eq>\mathbb{Z}/N\mathbb{Z}</eq></td><td>Group of integers modulo <eq>N</eq></td><td>221</td></tr><tr><td><eq>G, |G|</eq></td><td>Abelian group and its order</td><td>226, 228</td></tr><tr><td><eq>G\approx H</eq></td><td>Isomorphic groups</td><td>227</td></tr><tr><td><eq>G_{1}\times G_{2}</eq></td><td>Direct product of groups</td><td>228</td></tr><tr><td><eq>\mathbb{Z}^{*}(q)</eq></td><td>Group of units modulo <eq>q</eq></td><td>227, 229, 244</td></tr><tr><td><eq>\hat{G}</eq></td><td>Dual group of <eq>G</eq></td><td>231</td></tr><tr><td><eq>a|b</eq></td><td><eq>a</eq> divides <eq>b</eq></td><td>242</td></tr><tr><td><eq>\gcd(a,b)</eq></td><td>Greatest common divisor of <eq>a</eq> and <eq>b</eq></td><td>242</td></tr><tr><td><eq>\varphi(q)</eq></td><td>Number of integers relatively prime to <eq>q</eq></td><td>254</td></tr><tr><td><eq>\chi, \chi_{0}</eq></td><td>Dirichlet character, and trivial Dirichlet character</td><td>254</td></tr><tr><td><eq>L(s,\chi)</eq></td><td>Dirichlet <eq>L</eq>-function</td><td>256</td></tr><tr><td><eq>\log_{1}\left(\frac{1}{1-z}\right),\log_{2}L(s,\chi)</eq></td><td>Logarithms</td><td>258, 264</td></tr><tr><td><eq>d(k)</eq></td><td>Number of positive divisors of <eq>k</eq></td><td>269</td></tr></table>

## Index

Relevant items that also arise in Book I are listed in this index, preceeded by the numeral I. 

Abel means, 54 summable, 54 abelian group, 226 absolute value, 23 absorption coeficient, 199 amplitude, 3 annihilation operator, 169 approximation to the identity, 49 attenuation coeficient, 199 Bernoulli numbers, 97, 167 polynomials, 98 Bernstein’s theorem, 93 Bessel function, 197 Bessel’s inequality, 80 best approximation lemma, 78 Black-Scholes equation, 170 bump functions, 162 Cauchy problem (wave equation), 185 Cauchy sequence, 24 Cauchy-Schwarz inequality, 72 Ces`aro means, 52 sum, 52 summable, 52 character, 230 trivial (unit), 230 class C<sup>k</sup>, 44 

closed rectangle, 289 complete vector space, 74 complex conjugate, 23 exponential, 24 congruent integers, 220 conjugate Dirichlet kernel, 95 convolution, 44, 139, 239 coordinates spherical in R<sup>d</sup>, 293 creation operator, 169 curve, 102 area enclosed, 103 closed, 102 diameter, 125 length, 102 simple, 102 d’Alembert’s formula, 11 delayed means, 114 generalized, 127 descent (method of), 194 dilations, 133, 177 direct product of groups, 228 Dirichlet characters, 254 complex, 265 real, 265 Dirichlet kernel conjugate (on the circle), 95 modified (on the real line), 165 on the circle, 37 Dirichlet problem 

annulus, 64 rectangle, 28 strip, 170 unit disc, 20 Dirichlet product formula, 256 Dirichlet’s test, 60 Dirichlet’s theorem, 128 discontinuity jump, 63 of a Riemann integrable function, 286 divisibility of integers, 242 divisor, 242 greatest common, 242 divisor function, 269, 280 dual X-ray transform, 212 group, 231 Radon transform, 205 eigenvalues and eigenvectors, 233 energy, 148, 187 of a string, 90 equidistributed sequence, 107 ergodicity, 111 Euclid’s algorithm, 241 Euler constant γ, 268 identities, 25 phi-function, 254, 276 product formula, 249 even function, 10 expectation, 160 exponential function, 24 exponential sum, 112 fast Fourier transform, 224 Fej´er kernel on the circle, 53 on the real line, 163 Fibonacci numbers, 122 

## INDEX

Fourier coeficient (discrete), 236 coeficient, 16, 34 on Z(N), 223 on a finite abelian group, 235 series, 34 sine coeficient, 15 Fourier inversion finite abelian group, 235 on Z(N), 223 on R, 141 on R<sup>d</sup>, 182 Fourier series, 34, 235 Abel means, 55 Ces`aro mean, 53 delayed means, 114 generalized delayed means, 127 lacunary, 114 partial sum, 35 uniqueness, 39 Fourier series convergence mean square, 70 pointwise, 81, 128 Fourier series divergence, 83 Fourier transform, 134, 136, 181 fractional part, 106 function Bessel, 197 exponential, 24 gamma, 165 moderate decrease, 131, 179, 294 radial, 182 rapidly decreasing, 135, 178 sawtooth, 60, 83 Schwartz, 135, 180 theta, 155 zeta, 98 gamma function, 165 

## INDEX

Gaussian, 135, 181 Gibbs’s phenomenon, 94 good kernels, 48 greatest common divisor, 242 group (abelian), 226 cyclic, 238 dual, 231 homomorphism, 227 isomorphic, 227 of integers modulo N, 221 of units, 227, 229, 244 order, 228 H¨older condition, 43 harmonic function, 20 mean value property, 152 harmonics, 13 heat equation, 20 d-dimensions, 209 on the real line, 146 steady-state, 20 time-dependent, 20 heat kernel d-dimensions, 209 of the real line, 146, 156 of the circle, 120, 124, 156 Heisenberg uncertainty principle, 158, 168, 209 Hermite functions, 173 operator, 168 Hermitian inner product, 72 Hilbert space, 75 homomorphism, 227 Hooke’s law, 2 Huygens’ principle, 193 hyperbolic cosine and sine functions, 28 hyperbolic sums, 269 inner product, 71 Hermitian, 72 

strictly positive definite, 71 integer part, 106 integrable function (Riemann), 31, 281 inverse of a linear operator, 177 isoperimetric inequality, 103, 122 jump discontinuity, 63 Kirchhof’s formula, 211 L-function, 256 Landau kernels, 164 Laplace operator, 20 Laplacian, 20, 149, 185 polar coordinates, 27 Legendre expansion, 96 polynomial, 95 light cone backward, 193, 213 forward, 193 linearity, 6, 22 Lipschitz condition, 82 logarithm log<sub>1</sub>, 258 log<sub>2</sub>, 264 mean value propery, 152 measure zero, 287 moderate decrease (function), 131 modulus, 23 monomial, 176 multi-index, 176 multiplication formula, 140, 183 natural frequency, 3 Newton’s law, 3 of cooling, 19 nowhere diferentiable function, 113, 126 

## 308

odd function, 10 order of a group, 228 orthogonal elements, 72 orthogonality relations, 232 orthonormal family, 77 oscillation (of a function), 288 overtones, 6, 13 parametrization arc-length, 103 reverse, 121 Parseval’s identity, 79 finite abelian group, 236 part fractional, 106 integer, 106 partition of a rectangle, 290 of an interval, 281 period, 3 periodic function, 10 periodization, 153 phase, 3 Plancherel formula on Z(N), 223 on R, 143 on R<sup>d</sup>, 182 Planck’s constant, 161 plucked string, 17 Poincar´e’s inequality, 90 Poisson integral formula, 57 Poisson kernel d-dimensions, 210 on the unit disc, 37, 55 on the upper half-plane, 149 Poisson kernels,comparison, 157 Poisson summation formula, 154–156, 165, 174 polar coordinates, 179 polynomials Bernoulli, 98 Legendre, 95 

## INDEX

pre-Hilbert space, 75 prime number, 242 primes in arithmetic progression, 245, 252, 275 probability density, 160 profile, 5 pure tones, 6 Pythagorean theorem, 72 Radon transform, 200, 203 rapid decrease, 135 refinement (partition), 281, 290 relatively prime integers, 242 repeated integrals, 295 Reuleaux triangle, 125 Riemann integrable function, 31, 281, 290 Riemann localization principle, 82 Riemann-Lebesgue lemma, 80 root of unity, 219 rotation, 177 improper, 177 proper, 177 sawtooth function, 60, 83, 84, 94, 99, 278 scaling, 8 Schwartz space, 134, 180 separation of variables, 4, 11 simple harmonic motion, 2 space variables, 185 spectral theorem, 233 commuting family, 233 speed of propagation (finite), 194 spherical coordinates in R<sup>d</sup>, 293 mean, 189 wave, 210 spring constant, 3 standing wave, 4 

## INDEX

subordination principle, 210 subrectangle, 290 summable Abel, 54 Ces`aro, 52 summation by parts, 60 superposition, 6, 14 symmetry-breaking, 83 theta function, 155 functional equation, 155 tone fundamental, 13 pure, 11 translations, 133, 177 transpose of a linear operator, 177 traveling wave, 4 trigonometric polynomial, 35 degree, 35 series, 35 Tychonof’s uniqueness theorem, 172 uncertainty, 160 unit, 229 unitary transformation, 143, 233 variance, 160 vector space, 70 velocity of a wave, 5 velocity of the motion, 7 vibrating string, 90 

wave standing, 4, 13 traveling, 4 velocity, 5 wave equation, 184 d-dimensional, 185 d’Alembert’s formula, 11 is linear, 9 one-dimensional, 7 time reversal, 11 Weierstrass approximation theorem, 54, 63, 144, 163 Weyl criterion, 112, 123 estimate, 125 theorem, 107 Wirtinger’s inequality, 90, 122 

X-ray transform, 200 

zeta function, 98, 155, 166, 248 

## 309