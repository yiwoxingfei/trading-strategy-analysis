

<!-- === Source: MinerU_markdown_Set_theory_for_the_working_mathematician,_K._Ciesielski,_CUP,_1997_1_2122706224590991362.md (Page 1) === -->

# Set Theory for the Working Mathematician

Krzysztof Ciesielski 

London Mathematical Society Student Texts 39 

London Mathematical Society Student Texts 39 

# Set Theory for the Working Mathematician

Krzysztof Ciesielski 

West Virginia University 

PUBLISHED BY THE PRESS SYNDICATE OF THE UNIVERSITY OF CAMBRIDGE The Pitt Building, Trumpington Street, Cambridge CB2 1RP, United Kingdom 

CAMBRIDGE UNIVERSITY PRESS Thc Edinburgh Building. Cambridge CB2 2RU. United Kingdom 40 West 20th Street, New York, NY 1001 1-4211, USA 10 Stamford Road, Oakleigh. Melbourne 3166. Australia 

© Cambridge University Press 1997 

This book is in copyright. Subject to statutory exception and to the provisions of relevant collective licensing agreements, no reproduction of any part may take place without the written permission of Cambridge University Press. 

First published 1997 

Typeset in Computer Modern 

Library of Congress Cataloging-in-Publication Data 

Ciesielski, Krzysztof, 1957 

Set theory for the working mathematician / Krzysztof Ciesielski 

p. cm. - (London Mathematical Society student texts : 39) 

Includes bibliographical references and index. 

ISBN 0-521-59441-3 (hardback). – ISBN (0-521-59465-0 (paperback) 

1. Set theory. I. Titte. I1. Series. QA248.C475 1997 511.3'22 – dc21 

97-10533 CIP 

A catalog record for this book is available from the British Library 

ISBN 0-521-59441-3 hardback ISBN 0-521-59465-0 paperback 

Transferred to digital printing 2001 

To Monika, Agata, and Victoria 

and to the memory of my Mother, who taught me mathematics 

## Contents

Preface ix
Part I Basics of set theory 1
1 Axiomatic set theory 3
1.1 Why axiomatic set theory? 3
1.2 The language and the basic axioms 6
2 Relations, functions, and Cartesian product 12
2.1 Relations and the axiom of choice 12
2.2 Functions and the replacement scheme axiom 16
2.3 Generalized union, intersection, and Cartesian product 19
2.4 Partial- and linear-order relations 21
3 Natural numbers, integers, and real numbers 25
3.1 Natural numbers 25
3.2 Integers and rational numbers 30
3.3 Real numbers 31
Part II Fundamental tools of set theory 35
4 Well orderings and transfinite induction 37
4.1 Well-ordered sets and the axiom of foundation 37
4.2 Ordinal numbers 44
4.3 Definitions by transfinite induction 49
4.4 Zorn's lemma in algebra, analysis, and topology 54
5 Cardinal numbers 61
5.1 Cardinal numbers and the continuum hypothesis 61
5.2 Cardinal arithmetic 68
5.3 Cofinality 74 

viii Contents
Part III The power of recursive definitions 77
6 Subsets of $\mathbb{R}^n$ 79
6.1 Strange subsets of $\mathbb{R}^n$ and the diagonalization argument 79
6.2 Closed sets and Borel sets 89
6.3 Lebesgue-measurable sets and sets with the Baire property 98
7 Strange real functions 104
7.1 Measurable and nonmeasurable functions 104
7.2 Darboux functions 106
7.3 Additive functions and Hamel bases 111
7.4 Symmetrically discontinuous functions 118
Part IV When induction is too short 127
8 Martin's axiom 129
8.1 Rasiowa–Sikorski lemma 129
8.2 Martin's axiom 139
8.3 Suslin hypothesis and diamond principle 154
9 Forcing 164
9.1 Elements of logic and other forcing preliminaries 164
9.2 Forcing method and a model for $\neg\text{CH}$ 168
9.3 Model for CH and $\Diamond$ 182
9.4 Product lemma and Cohen model 189
9.5 Model for MA+ $\neg\text{CH}$ 196
A Axioms of set theory 211
B Comments on the forcing method 215
C Notation 220
References 225
Index 229 

## Preface

The course presented in this text concentrates on the typical methods of modern set theory: transfinite induction, Zorn’s lemma, the continuum hypothesis, Martin’s axiom, the diamond principle ♦, and elements of forcing. The choice of the topics and the way in which they are presented is subordinate to one purpose – to get the tools that are most useful in applications, especially in abstract geometry, analysis, topology, and algebra. In particular, most of the methods presented in this course are accompanied by many applications in abstract geometry, real analysis, and, in a few cases, topology and algebra. Thus the text is dedicated to all readers that would like to apply set-theoretic methods outside set theory. 

The course is presented as a textbook that is appropriate for either a lower-level graduate course or an advanced undergraduate course. However, the potential readership should also include mathematicians whose expertise lies outside set theory but who would like to learn more about modern set-theoretic techniques that might be applicable in their field. 

The reader of this text is assumed to have a good understanding of abstract proving techniques, and of the basic geometric and topological structure of the n-dimensional Euclidean space R<sup>n</sup>. In particular, a comfort in dealing with the continuous functions from R<sup>n</sup> into R is assumed. A basic set-theoretic knowledge is also required. This includes a good understanding of the basic set operations (union, intersection, Cartesian product of arbitrary families of sets, and diference of two sets), abstract functions (the operations of taking images and preimages of sets with respect to functions), and elements of the theory of cardinal numbers (finite, countable, and uncountable sets.) Most of this knowledge is included in any course in analysis, topology, or algebra. These prerequisites are also discussed briefly in Part I of the text. 

The book is organized as follows. Part I introduces the reader to axiomatic set theory and uses it to develop basic set-theoretic concepts. In particular, Chapter 1 contains the necessary background in logic, discusses the most fundamental axioms of ZFC, and uses them to define basic settheoretic operations. In Chapter 2 the notions of relation, function, and Cartesian product are defined within the framework of ZFC theory. Related notions are also introduced and their fundamental properties are discussed. Chapter 3 describes the set-theoretic interpretation of the sets of natural numbers, integers, and real numbers. Most of the facts presented in Part I are left without proof. 

Part II deals with the fundamental concepts of “classical set theory.” The ordinal and cardinal numbers are introduced and their arithmetic is developed. A theorem on definition by recursion is proved and used to prove Zorn’s lemma. Section 4.4 contains some standard applications of Zorn’s lemma in analysis, topology, and algebra. 

Part III is designed to familiarize the reader with proofs by transfinite induction. In particular, Section 6.1 illustrates a typical transfiniteinduction construction and the diagonalization argument by describing several diferent constructions of subsets of R<sup>n</sup> with strange geometric properties. The two remaining sections of Chapter 6 introduce the basic elements of descriptive set theory and discuss Borel and Lebesgue-measurable sets and sets with the Baire property. Chapter 7 is designed to help the reader master the recursive-definitions technique. Most of the examples presented there concern real functions, and in many cases consist of the newest research results in this area. 

Part IV is designed to introduce the tools of “modern set theory”: Martin’s axiom, the diamond principle ♦, and the forcing method. The overall idea behind their presentation is to introduce them as natural refinements of the method of transfinite induction. Thus, based on the solid foundation built in Part III, the forcing notions and forcing arguments presented there are obtained as “transformed” transfinite-induction arguments. In particular, the more standard axiomatic approach to these methods is described in Chapter 8, where Martin’s axiom and the diamond principle are introduced and discussed. Chapter 9 is the most advanced part of this text and describes the forcing method. Section 9.1 consists of some additional prerequisites, mainly logical, necessary to follow the other sections. In Section 9.2 the main theoretical basis for the forcing theory is introduced while proving the consistency of ZFC and the negation of CH. In Section 9.3 is constructed a generic model for ZFC+♦ (thus, also for ZFC+CH). Section 9.4 discusses the product lemma and uses it to deduce a few more properties of the Cohen model, that is, the model from Section 9.2. The book finishes with Section 9.5 in which is proved the simultaneous consistency of Martin’s axiom and the negation of the continuum hypothesis. This proof, done by iterated forcing, shows that even in the world of the “sophisticated recursion method” of forcing the “classical” recursion technique is still a fundamental method of set theory – the desired model is obtained by constructing forcing extensions by transfinite induction. 

It is also worthwhile to point out here that readers with diferent backgrounds will certainly be interested in diferent parts of this text. Most advanced graduate students as well as mathematical researchers using this book will almost certainly just skim Part I. The same may be also true for some of these readers for at least some portion of Part II. Part III and the first chapter of Part IV should be considered as the core of this text and are written for the widest group of readers. Finally, the last chapter (concerning forcing) is the most dificult and logic oriented, and will probably be of interest only to the most dedicated readers. It certainly can be excluded from any undergraduate course based on this text. 

Part I 

Basics of set theory 

## Chapter 1

# Axiomatic set theory

## 1.1 Why axiomatic set theory?

Essentially all mathematical theories deal with sets in one way or another. In most cases, however, the use of set theory is limited to its basics: elementary operations on sets, fundamental facts about functions, and, in some cases, rudimentary elements of cardinal arithmetic. This basic part of set theory is very intuitive and can be developed using only our “good” intuition for what sets are. The theory of sets developed in that way is called “naive” set theory, as opposed to “axiomatic” set theory, where all properties of sets are deduced from a fixed set of axioms. 

Clearly the “naive” approach is very appealing. It allows us to prove a lot of facts on sets in a quick and convincing way. Also, this was the way the first mathematicians studied sets, including Georg Cantor, a “father of set theory.” However, modern set theory departed from the “paradise” of this simple-minded approach, replacing it with “axiomatic set theory,” the highly structured form of set theory. What was the reason for such a replacement? 

Intuitively, a set is any collection of all elements that satisfy a certain given property. Thus, the following axiom schema of comprehension, due to Frege (1893), seems to be very intuitive. 

If $\varphi$ is a property, then there exists a set $Y = \{ X \colon \varphi ( X ) \}$ of all elements having property $\varphi$ . 

This principle, however, is false! It follows from the following theorem of Russell (1903) known as Russell’s antinomy or Russell’s paradox. 

Russell’s paradox There is no set $S = \{ X \colon X \notin X \}$ 

The axiom schema of comprehension fails for the formula $\varphi ( X )$ defined as ${ } ^ { \mathfrak { s c } } X \notin X . { } ^ { \mathfrak { s } }$ To see it, notice that if S had been a set we would have had for every Y 

$$
Y \in S \Leftrightarrow Y \notin Y.
$$

Substituting S for Y we obtain 

$$
S \in S \Leftrightarrow S \notin S,
$$

which evidently is impossible. 

This paradox, and other similar to it, convinced mathematicians that we cannot rely on our intuition when dealing with abstract objects such as arbitrary sets. To avoid this trouble, “naive” set theory has been replaced with axiomatic set theory. 

The task of finding one “universal” axiomatic system for set theory that agrees with our intuition and is free of paradoxes was not easy, and was not without some disagreement. Some of the disagreement still exists today. However, after almost a century of discussions, the set of ten axioms/schemas, known as the Zermelo–Fraenkel axioms (abbreviated as ZFC, where C stands for the axiom of choice), has been chosen as the most natural. These axioms will be introduced and explained in the next chapters. The full list of these axioms with some comments is also included in Appendix A. 

It should be pointed out here that the ZFC axioms are far from “perfect.” It could be expected that a “perfect” set of axioms should be complete, that is, that for any statement $\varphi$ expressed in the language of set theory (which is described in the next section) either $\varphi$ or its negation is a consequence of the axioms. Also, a “good” set of axioms should certainly be consistent, that is, should not lead to a contradiction. Unfortunately, we cannot prove either of these properties for the ZFC axioms. More precisely, we do believe that the ZFC axioms are consistent. However, if this belief is correct, we can’t prove it using the ZFC axioms alone. Does it mean that we should search for a better system of set-theory axioms that would be without such a deficiency? Unfortunately, there is no use in searching for it, since no “reasonable” set of axioms of set theory can prove its own consistency. This follows from the following celebrated theorem of G¨odel. 

Theorem 1.1.1 (G¨odel’s second incompleteness theorem) Let T be a set of axioms expressed in a formal language $\mathcal { L }$ (such as the language of set theory described in Section 1.2) and assume that T has the following “reasonable” properties. 

(1) $T$ is consistent. 

(2) There is an efective algorithm that decides for an arbitrary sentence of the language L whether it is in T or not. 

(3) T is complicated enough to encode simple arithmetic of the natural numbers. 

Then there is a sentence ϕ of the language L that encodes the statement “T is consistent.” However, ϕ is not a consequence of the axioms T. 

In other words, Theorem 1.1.1 shows us that for whatever “reasonable” systems of axioms of set theory we choose, we will always have to rely on our intuition for its consistency. Thus, the ZFC axioms are as good (or bad) in this aspect as any other “reasonable” system of axioms. 

So what about the completeness of the ZFC axioms? Can we prove at least that much? The answer is again negative and once again it is a common property for all “reasonable” systems of axioms, as follows from another theorem of G¨odel. 

Theorem 1.1.2 (G¨odel’s first incompleteness theorem) Let T be a set of axioms expressed in a formal language L (such as the language of set theory described in Section 1.2) and assume that T has the following “reasonable” properties. 

(1) T is consistent. 

(2) There is an efective algorithm that decides for an arbitrary sentence of the language L whether it is in T or not. 

(3) T is complicated enough to encode simple arithmetic of the natural numbers. 

Then there is a sentence ϕ of the language L such that neither ϕ nor its negation ¬ϕ can be deduced from the axioms T. 

A sentence ϕ as in Theorem 1.1.2 is said to be independent of the axioms T. It is not dificult to prove that a sentence $\varphi$ is independent of the consistent set of axioms T if and only if both $T \cup \{ \varphi \}$ and $T \cup \{ \lnot \varphi \}$ are consistent too. Part of this course will be devoted to studying the sentences of set theory that are independent of the ZFC axioms. 

The preceding discussion shows that there is no way to find a good complete set of axioms for set theory. On the other hand, we can find a set of axioms that reach far enough to allow encoding of all set-theoretic operations and all classical mathematical structures. Indeed, the ZFC axioms do satisfy this requirement, and the rest of Part I will be devoted to describing such encodings of all structures of interest. 

## 1.2 The language and the basic axioms

Any mathematical theory must begin with undefined concepts. In the case of set theory these concepts are the notion of a “set” and the relation ${ } ^ { 6 6 } \mathrm { { \dot { 1 } s } }$ an element $\mathrm { o f } ^ { \mathrm { 7 } }$ between the sets. In particular, we write $\mathbf { \boldsymbol { \hat { \mathbf { \mathit { x } } } } } \in { \boldsymbol { y } } ^ { \mathfrak { \prime } }$ for $^ { 6 6 } x$ is an element of $y . \overset { \underset { \mathrm { ~ \tiny ~ , ~ } } { ~ } }$ 

The relation $\in$ is primitive for set theory, that is, we do not define it. All other objects, including the notion of a set, are described by the axioms. In particular, all objects considered in formal set theory are sets. (Thus, the word “set” is superfluous.) 

In order to talk about any formal set theory it is necessary to specify first the language that we will use and in which we will express the axioms. The correct expressions in our language are called formulas. The basic formulas are $^ { \ast } x \in y ^ { \mathfrak { Y } }$ and $\mathbf { \boldsymbol { \mathbf { \mathit { z } } } } = t , \mathbf { \boldsymbol { \mathbf { \mathit { \varepsilon } } } } ^ { \prime }$ where $x , y , z$ , and t (or some other variable symbols) stand for the sets. We can combine these expressions using the basic logical connectors of negation ¬, conjunction $\&$ , disjunction $\vee .$ , implication →, and equivalence . Thus, for example, $\neg \varphi$ means “not $\varphi ^ { , \mathfrak { p } }$ and $\varphi {  } \psi$ stands for $^ { 6 6 } \varphi$ implies $\psi . ^ { \mathfrak { v } }$ In addition, we will use two quantifiers: existential ∃ and universal $\forall .$ Thus, an expression $\forall x \varphi$ is interpreted as “for all x formula $\varphi$ holds.” In addition, the parentheses $^ { 6 6 } ( ^ { 9 } )$ and “)” are used, when appropriate. 

Formally, the formulas can be created only as just described. However, for convenience, we will also often use some shortcuts. For example, an expression $\exists x \in A \varphi ( x )$ will be used as an abbreviation for $\exists x ( x \in A \ \& \ \varphi ( x ) )$ , and we will write $\forall x \in A \varphi ( x )$ to abbreviate the formula $\forall x ( x \in A { \xrightarrow { } } \varphi ( x ) )$ Also we will use the shortcuts x $\neq y , x \notin y , x \subset y$ , and $x \not \subset y$ , where, for example, $x \subset y$ stands for $\forall z ( z \in x {  } z \in y )$ 

Finally, only variables, the relations = and ∈, and logical symbols already mentioned are allowed in formal formulas. However, we will often use some other constants. For example, we will write $x = \emptyset$ (x is an empty set) in place of $\neg \exists y ( y \in x )$ 

We will discuss ZFC axioms throughout the next few sections as they are needed. Also, in most cases, we won’t write in the main text the formulas representing the axioms. However, the full list of ZFC axioms together with the formulas can be found in Appendix A. 

Let us start with the two most basic axioms. 

Set existence axiom There exists a set: $\exists x ( x = x )$ 

Extensionality axiom If x and y have the same elements, then x is equal to y. 

The set existence axiom follows from the others. However, it is the most basic of all the axioms, since it ensures that set theory is not a trivial theory. The extensionality axiom tells us that the sets can be distinguish only by their elements. 

Comprehension scheme (or schema of separation) For every formula $\varphi ( s , t )$ with free variables s and t, set $x ,$ and parameter $p$ there exists a set $y = \{ u \in x \colon \varphi ( u , p ) \}$ that contains all those $u \in x$ that have the property $\varphi$ 

Notice that the comprehension scheme is, in fact, the scheme for infinitely many axioms, one for each formula $\varphi$ . It is a weaker version of Frege’s axiom schema of comprehension. However, the contradiction of Russell’s paradox can be avoided, since the elements of the new set $y = \{ u \in x \colon \varphi ( u , p ) \}$ are chosen from a fixed set $x _ { i }$ , rather than from an undefined object such as “the class of all sets.” 

From the set existence axiom and the comprehension scheme used with the formula $^ { \ast } u \neq u , ^ { \ast }$ we can conclude the following stronger version of the set existence axiom. 

Empty set axiom There exists the empty set $\varnothing .$ 

To see the implication, simply define $\emptyset = \{ y \in x \colon y \neq y \}$ , where $x$ is a set from the set existence axiom. Notice that by the extensionality axiom the empty set is unique. 

An interesting consequence of the comprehension scheme axiom is the following theorem. 

Theorem 1.2.1 There is no set of all sets. 

Proof If there were a set S of all sets then the following set 

$$
Z = \{X \in S \colon X \notin X \}
$$

would exist by the comprehension scheme axiom. However, with $S$ being the set of all sets, we would have that $Z = \{ X \colon X \notin X \}$ , the set from Russell’s paradox. This contradiction shows that the set $S$ of all sets cannot exist.  

By the previous theorem all sets do not form a set. However, we sometimes like to talk about this object. In such a case we will talk about a class of sets or the set-theoretic universe. We will talk about classes only on an intuitive level. It is worth mentioning, however, that the theory of classes can also be formalized similarly to the theory of sets. This, however, is far beyond the scope of this course. Let us mention only that there are other proper classes of sets (i.e., classes that are not sets) that are strictly smaller than the class of all sets. 

The comprehension scheme axiom is a conditional existence axiom, that is, it describes how to obtain a set (subset) from another set. Other basic conditional existence axioms are listed here. 

Pairing axiom For any a and b there exists a set x that contains a and b. 

Union axiom For every family F there exists a set U containing the union F of all elements of $\mathcal { F }$ 

Power set axiom For every set X there exists a set P containing the set P(X) (the power set) of all subsets of X. 

In particular, the pairing axiom states that for any a and b there exists a set x such that $\{ a , b \} \subset x$ . Although it does not state directly that there exists a set $\{ a , b \}$ , the existence of this set can easily be concluded from the existence of x and the comprehension scheme axiom: 

$$
\{a, b \} = \{u \in x: u = a \lor u = b \}.
$$

Similarly, we can conclude from the union and power set axioms that for every sets $\mathcal { F }$ and X there exist the union of $\mathcal { F }$ 

$$
\bigcup \mathcal {F} = \{x \colon \exists F \in \mathcal {F} (x \in F) \} = \{x \in U \colon \exists F \in \mathcal {F} (x \in F) \}
$$

and the power set of X 

$$
\mathcal {P} (X) = \{z \colon z \subset X \} = \{z \in P \colon z \subset X \}.
$$

It is also easy to see that these sets are defined uniquely. Notice also that the existence of a set $\{ a , b \}$ implies the existence of a singleton set {a}, since $\{ a \} = \{ a , a \}$ 

The other basic operations on sets can be defined as follows: the union of two sets x and y by 

$$
x \cup y = \bigcup \{x, y \};
$$

the diference of sets x and y by 

$$
x \setminus y = \{z \in x \colon z \not \in y \};
$$

the arbitrary intersections of a family $\mathcal { F }$ by 

$$
\bigcap \mathcal {F} = \left\{z \in \bigcup \mathcal {F}: \forall F \in \mathcal {F} (z \in F) \right\};
$$

and the intersections of sets x and y by 

$$
x \cap y = \bigcap \{x, y \}.
$$

The existence of sets $x \backslash y$ and $\cap \mathcal { F }$ follows from the axiom of comprehension. 

We will also sometimes use the operation of symmetric diference of two sets, defined by 

$$
x \triangle y = (x \setminus y) \cup (y \setminus x).
$$

Its basic properties are listed in the next theorem. Its proof is left as an exercise. 

## Theorem 1.2.2 For every $x , y .$ , and $z$

(a) $x \triangle y = y \triangle x .$ 

(b) $x \triangle y = ( x \cup y ) \setminus ( x \cap y ) ,$ 

(c) $( x \triangle y ) \triangle z = x \triangle ( y \triangle z ) .$ 

We will define an ordered pair $\langle a , b \rangle$ for arbitrary a and b by 

$$
\langle a, b \rangle = \{\{a \}, \{a, b \} \}.\tag{1.1}
$$

It is dificult to claim that this definition is natural. However, it is commonly accepted in modern set theory, and the next theorem justifies it by showing that it maintains the intuitive properties we usually associate with the ordered pair. 

Theorem 1.2.3 For arbitrary $a , b , c ,$ and d 

$$
\langle a, b \rangle = \langle c, d \rangle \text {   if   and   only   if   } a = c \text {   and   } b = d.
$$

Proof Implication $\Leftarrow$ is obvious. 

To see the other implication, assume that $\langle a , b \rangle = \langle c , d \rangle$ . This means that $\{ \{ a \} , \{ a , b \} \} = \{ \{ c \} , \{ c , d \} \}$ . In particular, by the axiom of extensionality, {a} is equal to either $\{ c \}$ or $\{ c , d \}$ 

If $\{ a \} = \{ c \}$ then $a = c .$ . If $\{ a \} = \{ c , d \}$ , then c must belong to $\{ a \}$ and we also conclude that $a = c$ . In any case, $a = c$ and we can deduce that $\{ \{ a \} , \{ a , b \} \} = \{ \{ a \} , \{ a , d \} \}$ . We wish to show that this implies $b = d .$ 

But $\{ a , b \}$ belongs to $\{ \{ a \} , \{ a , d \} \}$ . Thus we have two cases. 

Case 1: $\{ a , b \} = \{ a , d \}$ . Then $b = a$ or $b = d .$ . If $b = d$ we are done. If $b = a$ then $\{ a , b \} = \{ a \}$ and so $\{ a , d \} = \{ a \}$ . But d belongs then to $\{ a \}$ and so $d = a$ . Since we had also $a = b$ we conclude $b = d .$ 

Case 2: $\{ a , b \} = \{ a \}$ . Then b belongs to $\{ a \}$ and so $b = a$ . Hence we conclude that $\{ a , d \} = \{ a \}$ , and as in case 1 we can conclude that $b = d$ 

Now we can define an ordered triple $\langle a , b , c \rangle$ by identifying it with $\langle \langle a , b \rangle , c \rangle$ and, in general, an ordered n-tuple by 

$$
\langle a _ {1}, a _ {2}, \ldots , a _ {n - 1}, a _ {n} \rangle = \langle \langle a _ {1}, a _ {2}, \ldots , a _ {n - 1} \rangle , a _ {n} \rangle .
$$

The agreement of this definition with our intuition is given by the following theorem, presented without proof. 

Theorem 1.2.4 $\langle a _ { 1 } , a _ { 2 } , \ldots , a _ { n - 1 } , a _ { n } \rangle = \langle a _ { 1 } ^ { \prime } , a _ { 2 } ^ { \prime } , \ldots , a _ { n - 1 } ^ { \prime } , a _ { n } ^ { \prime } \rangle$ if and only $i f a _ { i } = a _ { i } ^ { \prime }$ for all $i = 1 , 2 , \dots , n$ 

Next we will define a Cartesian product $X \times Y$ as the set of all ordered pairs $\langle x , y \rangle$ such that $x \in X$ and $y \in Y$ . To make this definition formal, we have to use the comprehension axiom. For this, notice that for every $x \in X$ and $y \in Y$ we have 

$$
\langle x, y \rangle = \{\{x \}, \{x, y \} \} \in \mathcal {P} (\mathcal {P} (X \cup Y)).
$$

Hence, we can define 

$$
X \times Y = \{z \in \mathcal {P} (\mathcal {P} (X \cup Y)): \exists x \in X \exists y \in Y (z = \langle x, y \rangle) \}.\tag{1.2}
$$

The basic properties of the Cartesian product and its relation to other set-theoretic operations are described in the exercises. 

The last axiom we would like to discuss in this section is the infinity axiom. It states that there exists at least one infinite set. This is the only axiom that implies the existence of an infinite object. Without it, the family $\mathcal { F }$ of all finite subsets of the set of natural numbers would be a good $\mathrm { \ddot { m o d e l } \vec { \Omega } }$ of set theory, that is, $\mathcal { F }$ satisfies all the axioms of set theory except the infinity axiom. 

To make the statements of the infinity axiom more readable we introduce the following abbreviation. We say that $y$ is a successor of $x$ and write $y = S ( x )$ if $y = x \cup \{ x \}$ , that is, when 

$$
\forall z [ z \in y \leftrightarrow (z \in x \lor z = x) ].
$$

Infinity axiom (Zermelo 1908) There exists an infinite set (of some special form): 

$$
\exists x \left[ \forall z (z = \emptyset \rightarrow z \in x) \&\forall y \in x \forall z (z = S (y) \rightarrow z \in x) \right].
$$

Notice that the infinity axiom obviously implies the set existence axiom. 

## EXERCISES

1 Prove that if $F \in { \mathcal { F } }$ then $\cap { \mathcal { F } } \subset F \subset \bigcup { \mathcal { F } }$ 

2 Show that for every family F and every set A 

(a) if $A \subset F$ for every $F \in { \mathcal { F } }$ then $A \subset \cap { \mathcal { F } }$ , and 

(b) if $F \subset A$ for every $F \in { \mathcal { F } }$ then $\cup { \mathcal { F } } \subset A .$ 

3 Prove that if $\mathcal { F } \cap \mathcal { G } \neq \emptyset$ then $\bigcap { \mathcal { F } } \cap \bigcap { \mathcal { G } } \subset \bigcap ( { \mathcal { F } } \cap { \mathcal { G } } )$ . Give examples   showing that the inclusion cannot be replaced by equality and that the assumption $\mathcal { F } \cap \mathcal { G } \neq \emptyset$ is essential. 

4 Prove Theorem 1.2.2. 

5 Show that $\langle \langle a , b \rangle , c \rangle = \langle \langle a ^ { \prime } , b ^ { \prime } \rangle , c ^ { \prime } \rangle$ if and only if $\langle a , \langle b , c \rangle \rangle = \langle a ^ { \prime } , \langle b ^ { \prime } , c ^ { \prime } \rangle \rangle$ if and only if $a = a ^ { \prime } , b = b ^ { \prime }$ , and $c = c ^ { \prime }$ . Conclude that we could define an ordered triple $\langle a , b , c \rangle$ as $\langle a , \langle b , c \rangle \rangle$ instead of $\langle \langle a , b \rangle , c \rangle$ 

6 Prove that $X \times Y = \emptyset$ if and only if $X = \varnothing \ \mathrm { o r } \ Y = \varnothing$ 

7 Show that for arbitrary sets $X , Y ,$ and Z the following holds. 

(a) $( X \cup Y ) \times Z = ( X \times Z ) \cup ( Y \times Z ) .$ 

(b) $( X \cap Y ) \times Z = ( X \times Z ) \cap ( Y \times Z ) .$ 

(c) $( X \setminus Y ) \times Z = ( X \times Z ) \setminus ( Y \times Z ) .$ 

8 Prove that if $X \times Z \subset Y \times T$ and $X \times Z \neq \emptyset$ then $X \subset Y$ and $Z \subset T$ Give an example showing that the assumption $X \times Z \neq \emptyset$ is essential. 

# Relations, functions, and Cartesian product

## 2.1 Relations and the axiom of choice

A subset R of a Cartesian product $X \times Y$ is called a (binary) relation. 

For a relation R of a Cartesian product $X \times Y$ , we usually write aRb instead of $\langle a , b \rangle \in R$ and read: a is in the relation R to b, or the relation R between a and b holds. 

The domain dom(R) of a relation R is defined as the set of all x such that $\langle x , y \rangle \in R$ for some $y \in Y$ , that is, 

$$
\operatorname{dom} (R) = \{x \in X: \exists y \in Y (\langle x, y \rangle \in R) \};
$$

the range range(R) of a relation R is defined as the set of all y such that $\langle x , y \rangle \in R$ for some $x \in X$ , that is, 

$$
\operatorname{range} (R) = \{y \in Y \colon \exists x \in X (\langle x, y \rangle \in R) \}.
$$

The set Z = dom(R) ∪ range(R) for relation R is called a field of R. Notice that $R \subset Z \times Z$ . In this case we often say that R is defined on Z. 

Examples 1. The relation $R _ { < }$ on the set of real numbers R defined as $\langle x , y \rangle \in R _ { < }$ if and only if $x \ < \ y$ is usually denoted by $< . ^ { 1 }$ Notice that 

$R _ { < }$ is the subset of the plane consisting of those points that are above the identity line $y = x$ . The domain and the range of this relation are equal to R. 

2. Consider the relation $R _ { \mathrm { d i v } }$ on the set of natural numbers N defined as $\langle x , y \rangle \in R _ { \mathrm { d i v } }$ if and only if x and y are diferent natural numbers greater than 1 and x divides $y .$ Then dom $( R _ { \mathrm { d i v } } ) = \{ 2 , 3 , 4 , \dots \}$ and range $( R _ { \mathrm { d i v } } )$ is the set of all composite natural numbers. 

Let $R \subset X \times Y$ and $S \subset Y \times Z$ . The relation 

$$
\{\langle y, x \rangle \in Y \times X: x R y \}
$$

is called the inverse of R and is denoted by $R ^ { - 1 }$ . The relation 

$$
\{\langle x, z \rangle \in X \times Z: \exists y \in Y (x R y \& y S z) \}
$$

is called the composition of R and S and is denoted by $S \circ R$ 

Note that $( R ^ { - 1 } ) ^ { - 1 } = R , \mathrm { d o m } ( R ^ { - 1 } ) = \mathrm { r a n g e } ( R ) , \mathrm { r a n g e } ( R ^ { - 1 } ) = \mathrm { d o m } ( R )$ $\operatorname { d o m } ( S \circ R ) \subset \operatorname { d o m } ( R )$ , and range $( S \circ R ) \subset \mathrm { r a n g e } ( S )$ . Moreover, $( S \circ R ) ^ { - 1 } =$ $R ^ { - 1 } \circ S ^ { - 1 }$ 

Examples 1. $\mathrm { I f } ~ \leq ~ \mathrm { a n d } ~ \geq ~ \mathrm { a r e }$ defined on R in the natural way then $( \leq ) ^ { - 1 } = \geq$ 

2. $( \geq ) \circ ( \leq )$ is equal to the relation $\mathbb { R } \times \mathbb { R }$ 

3. $( \leq ) \circ ( \leq )$ is equal to $\leq$ 

Let R be a binary relation on $X \times X$ . We say that R is 

reflexive if xRx for every $x \in X$ ; 

symmetric if xRy implies yRx for every $x , y \in X$ ; and 

transitive if xRy and yRz imply xRz for every $x , y , z \in X$ 

Examples 1. The relations < and $>$ on R are transitive, but they are neither reflexive nor symmetric. 

2. The relations $\leq \mathrm { a n d } \geq \mathrm { o n }$ R are transitive and reflexive, but not symmetric. 

3. The relation $\neq$ on R is symmetric, but is neither reflexive nor transitive. 

4. The relation $\varnothing \subset \mathbb { R } \times \mathbb { R }$ is symmetric and transitive, but is not reflexive. 

5. The relation R on R defined by xRy if and only if $y = x ^ { 2 }$ has neither of the three properties. 

6. The relation = on R is reflexive, symmetric, and transitive. 

A binary relation $R \subset X \times X$ is an equivalence relation on X if it is reflexive, symmetric, and transitive. Equivalence relations are usually denoted by symbols such as $\sim , \approx , \mathrm { o r } \equiv$ 

Examples 1. The relation = on any set X is an equivalence relation. 

2. If L is the family of all straight lines on the plane and R is the relation on L of being parallel, then R is an equivalence relation. 

3. Let C be the family of all Cauchy sequences $\langle a _ { n } \rangle = \langle a _ { 1 } , a _ { 2 } , . . . \rangle$ of rational numbers. Define relation ∼ on C by $\left. a _ { n } \right. \sim \left. b _ { n } \right.$ if and only if $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } ( a _ { n } - b _ { n } ) = 0 } \end{array}$ . Then ∼ is an equivalence relation. 

4. A nonempty family ${ \mathcal { T } } \subset { \mathcal { P } } ( X )$ is said to be an ideal on X if for every $A , B \in { \mathcal { P } } ( X )$ 

$$
A \subset B \& B \in \mathcal {I} \to A \in \mathcal {I} \quad \text { and } \quad A, B \in \mathcal {I} \to A \cup B \in \mathcal {I}.
$$

For every ideal I on a set ${ \mathcal { P } } ( X )$ the relation 

$$
A r B \text { if   and   only   if } A \triangle B \in \mathcal {I}
$$

is an equivalence relation. 

Let X be a set. A family F of nonempty subsets of X is said to be a partition of X if $\cup { \mathcal { F } } = X$ and sets belonging to $\mathcal { F }$ are pairwise disjoint, that is, for every $A , B \in { \mathcal { F } }$ either $A = B$ or $A \cap B = \emptyset$ 

For an equivalence relation E on X and $x \in X$ the set 

$$
[ x ] = \{y \in X: x E y \}
$$

is called the equivalence class of x (with respect to E). The family 

$$
\{[ x ] \in \mathcal {P} (X) \colon x \in X \}
$$

of all equivalence classes for E is denoted by $X / E$ and is called the quotient class of X with respect to E. 

For a partition F of a set X let us define a relation $R _ { \mathcal { F } }$ on X by 

$$
x R _ {\mathcal {F}} y \Leftrightarrow \exists F \in \mathcal {F} (x \in F \& y \in F).
$$

## Theorem 2.1.1

(A) If E is an equivalence relation on X then the family $X / E$ of all equivalence classes forms a partition of X, that is, for every x, $y \in X$ either $[ x ] = [ y ] o r [ x ] \cap [ y ] = \emptyset$ 

(B) If F is a partition of X then $R _ { \mathcal { F } }$ is an equivalence relation on X. Moreover, $X / R _ { \mathscr { F } } = \mathscr { F }$ and $R _ { X / E } = E$ 

The proof is left as an exercise. 

Theorem 2.1.1 shows that there is a one-to-one correspondence between the class of all partitions of X and the family of all equivalence relations on X. In general, equivalence classes generalize the notion of equality. Elements within one equivalence class are identified by the relation. 

An element x of an equivalence class C is called a representative of C. A set of representatives of an equivalence relation E is a set that contains exactly one element in common with each equivalence class. Notice that, by Theorem 2.1.1 and the axiom of choice, to be stated shortly, a set of representatives exists for every equivalence relation. 

Axiom of choice For every family F of nonempty disjoint sets there exists a selector, that is, a set S that intersects every $F \in { \mathcal { F } }$ in precisely one point. 

The axiom of choice (usually abbreviated as AC) has the conditional existence character of the pairing, union, and power set axioms. However, it has also a very diferent character, since a selector, which exists by this axiom, does not have to be unique. This nonconstructive character of the axiom of choice was, in the past, the reason that some mathematicians (including Borel and Lebesgue) did not like to accept it. However, the discussion on the validity of the axiom of choice has been for the most part resolved today, in favor of accepting it. 

The axiom of choice will be one of the most important tools in this course. 

## EXERCISES

1 Let $R \subset X \times Y$ and $S \subset Y \times Z$ be the relations. Prove that dom $( R ^ { - 1 } ) =$ range $( R ) , \mathrm { d o m } ( S \circ R ) \subset \mathrm { d o m } ( R )$ , and range $( S \circ R ) \subset \mathrm { r a n g e } ( S )$ 

2 Show the formulas $( R \cup S ) ^ { - 1 } = R ^ { - 1 } \cup S ^ { - 1 } , ( R \cap S ) ^ { - 1 } = R ^ { - 1 } \cap S ^ { - 1 }$ , and $( S \circ R ) ^ { - 1 } = R ^ { - 1 } \circ S ^ { - 1 }$ 

3 Prove the formulas 

$$
(R \cup S) \circ T = (R \circ T) \cup (S \circ T), \quad T \circ (R \cup S) = (T \circ R) \cup (T \circ S),
$$

$$
(R \cap S) \circ T \subset (R \circ T) \cap (S \circ T), \quad T \circ (R \cap S) \subset (T \circ R) \cap (T \circ S).
$$

Find examples of relations R, S, and T that show that the inclusions in the display cannot be replaced with equations. 

4 Find examples of relations on R that are 

(a) reflexive, but neither symmetric nor transitive; 

(b) reflexive and symmetric but not transitive. 

5 Prove Theorem 2.1.1. 

## 2.2 Functions and the replacement scheme axiom

A relation $R \subset X \times Y$ is called a function if 

$$
(\forall x, y _ {1}, y _ {2}) (x R y _ {1} \&x R y _ {2} \rightarrow y _ {1} = y _ {2}).
$$

Functions are usually denoted by the letters $f , g , h , \ldots$ The domain dom $( f )$ and the range range(f) of a function f are defined as for relations. For a function f if dom $( f ) = X$ and range $( f ) \subset Y$ then f is called a function (or map or transformation) from $X$ into Y and it is denoted by $f \colon X \to$ $Y , \ \operatorname { I f } ,$ moreover, $\mathrm { r a n g e } ( f ) = Y$ then f is said to be a function (map or transformation) from X onto Y, or a surjective function. The set of all functions from X into Y is denoted by $Y ^ { X }$ 

If $f \in Y ^ { X }$ and $x \in X$ then there exists precisely one $y \in Y$ such that $x f y$ . The element y is called the value of f at x and is denoted by $f ( x )$ Thus, the formula $y = f ( x )$ has the same meaning as $x f y$ 

Notice that for $f , g \in Y ^ { X }$ 

$$
f = g \Leftrightarrow \forall x \in X (f (x) = g (x)).
$$

A function $f \colon X \to Y$ is a one-to-one (or injective) function if 

$$
f (x) = f (y) \rightarrow x = y
$$

for all $x , y \in X$ . A function $f \colon X \to Y$ is a bijection if it is one-to-one and onto Y. 

For $f \colon X \to Y , A \subset X$ , and $B \subset Y$ we define 

$$
f [ A ] = \{f (x) \colon x \in X \} = \{y \in Y \colon \exists x \in X (y = f (x)) \}
$$

and 

$$
f ^ {- 1} (B) = \{x \in X \colon f (x) \in B \}.
$$

We use square brackets in $f [ A ]$ rather than regular parentheses to avoid a double meaning for the symbol $f ( A )$ when A is at the same time an element of X and its subset. A similar double meaning may happen when the symbol $f ^ { - 1 } ( B )$ is used. However, in this case it will be always clear from the context which meaning of the symbol we have in mind. The sets $f [ A ]$ and $f ^ { - 1 } ( B )$ are called the image of A and the preimage of B with respect to $f ,$ respectively. 

Theorem 2.2.1 If $f \in Y ^ { X }$ then $f ^ { - 1 } \textit { i s }$ a function $i f$ and only $\textit { i f f } \textit { i s }$ one-to-one. Moreover, $i f \ f ^ { - 1 }$ is a function then $f ^ { - 1 } \in X ^ { Z }$ , where $Z =$ range(f), and $f ^ { - 1 }$ is one-to-one. 

Theorem 2.2.2 If $f \in Y ^ { X }$ and $g \in Z ^ { Y }$ then $g \circ f$ is also a function and $g \circ f \in Z ^ { X }$ . Moreover, $( g \circ f ) ( x ) = g ( f ( x ) )$ for every $x \in X$ 

Theorem 2.2.3 Let $f \in Y ^ { X }$ and $g \in Z ^ { Y }$ . If f and g are one-to-one, then so is $g \circ f$ . If f and g are onto, then so is $g \circ f$ 

The proofs are left as exercises. 

For the proof of the next theorem we need one more axiom scheme. 

Replacement scheme axiom (Fraenkel 1922; Skolem 1922) For every formula $\varphi ( s , t , U , w )$ with free variables $s , \ t , \ U$ , and $w ,$ set $A ,$ , and parameter p if $\varphi ( s , t , A , p )$ defines a function $F$ on $A$ by $F ( x ) =$ $y \Leftrightarrow \varphi ( x , y , A , p )$ , then there exists a set $Y$ containing the range $F [ A ]$ of the function $F _ { ; }$ where $F [ A ] = \{ F ( x ) \colon x \in A \}$ 

As with the comprehension scheme axiom, the replacement scheme axiom is in fact a scheme for infinitely many axioms, one for each formula $\varphi$ . In conjunction with the comprehension scheme axiom, the replacement scheme axiom implies that for a function defined by formula $F ( x ) = y \Leftrightarrow \varphi ( x , y , A , p )$ on a set $A$ , the range of $F$ exists, since it can be defined: 

$$
F [ A ] = \{y \in Y: \exists x \in A (y = F (x)) \}.
$$

Sometimes the replacement scheme axiom is formulated in a stronger version, which states that the set $Y$ existing by the axiom is equal to the range of $F$ . It is worth noticing that such a stronger version of the replacement scheme axiom implies the comprehension scheme axiom. 

Now we are ready for the next theorem. 

Theorem 2.2.4 If F is a family of nonempty sets then there is a function $f \colon { \mathcal { F } } \to \bigcup { \mathcal { F } }$ such that $f ( X ) \in X$ for every $X \in { \mathcal { F } }$ 

Proof Take a formula $\varphi ( X , Y )$ that can be abbreviated to 

$$
Y = \{X \} \times X.
$$

Notice that if $\varphi ( X , Y )$ and $\varphi ( X , Y ^ { \prime } )$ hold then $Y = \{ X \} \times X = Y ^ { \prime }$ . In particular, $\varphi$ satisfies the assumptions of the replacement scheme axiom. So there exists a family 

$$
\mathcal {G} = \{Y \colon \exists X \in \mathcal {F} (\varphi (X, Y)) \} = \{\{X \} \times X \colon X \in \mathcal {F} \}.
$$

Notice that elements of $\mathcal { G }$ are nonempty and that they are pairwise disjoint, since 

$$
(\{X \} \times X) \cap (\{X ^ {\prime} \} \times X ^ {\prime}) = (\{X \} \cap \{X ^ {\prime} \}) \times (X \cap X ^ {\prime}).
$$

Thus, by the axiom of choice, there is a selector f for $\mathcal { G }$ . Notice that $f$ is the desired function.  

The function from Theorem 2.2.4 is called a choice function for the family ${ \mathcal F } .$ . In fact, the statement that for every family of nonempty sets there exists a choice function is equivalent to the axiom of choice. The statement follows from the axiom of choice by Theorem 2.2.4. To see that the axiom of choice follows from it define a selector $S$ for a family $\mathcal { F }$ of nonempty pairwise-disjoint sets as $S = { \mathrm { r a n g e } } ( f )$ when f is a choice function for $\mathcal { F }$ 

For a function $f \in Y ^ { X }$ and $A \subset X$ the relation $f \cap ( A \times Y )$ is a function that belongs to $Y ^ { A }$ . It is called the restriction of $f$ to the set A and is denoted by $f | _ { A }$ 

A function g is said to be an extension of a function f if $f \subset g$ . We also say that f is a restriction of $g$ 

Theorem 2.2.5 If f and g are functions then g extends f if and only if dom $( f ) \subset \mathop { \mathrm { d o m } } ( g )$ and $f ( x ) = g ( x )$ for every $x \in \operatorname { d o m } ( f )$ 

The proof is left as an exercise. 

Functions for which the domain is the set N of natural numbers are called $( i n f i n i t e )$ sequences. A $( f i n i t e )$ sequence is any function whose domain is any natural number n $( = \{ 0 , 1 , \ldots , n - 1 \} )$ . If a is any sequence, then we usually write $a _ { m }$ in place of $a ( m )$ . We will sometimes represent such a sequence by the symbol $\left. \boldsymbol { a } _ { m } \right.$ or $\{ a _ { m } \}$ , indicating the domain of the sequence if necessary. 

## EXERCISES

1 Prove Theorem 2.2.1. 

2 Prove Theorem 2.2.2. 

3 Prove Theorem 2.2.3. 

4 Prove Theorem 2.2.5. 

## 2.3 Generalized union, intersection, and Cartesian product

Let F be a function from a nonempty set T into a family of sets $\mathcal { G }$ . We will usually write $F _ { t }$ instead of $F ( t )$ and $\{ F _ { t } \colon t \in T \}$ or $\{ F _ { t } \} _ { t \in T }$ for range(F). The family $\mathcal { F } = \{ F _ { t } \} _ { t \in T }$ is called an indexed family, with T being the index set. 

The following notation will be used for $\mathcal { F } = \{ F _ { t } \} _ { t \in T }$ 

$$
\bigcup_ {t \in T} F _ {t} = \bigcup \mathcal {F}, \quad \bigcap_ {t \in T} F _ {t} = \bigcap \mathcal {F}.
$$

In the text these sets will also appear as $\textstyle \bigcup _ { t \in T } F _ { t }$ and $\cap _ { t \in T } F _ { t }$ , respectively.  When the set T is fixed, we will sometimes abbreviate this notation and write $\{ F _ { t } \} _ { t }$ or $\{ F _ { t } \}$ in place of $\{ F _ { t } \} _ { t \in T }$ , and $\textstyle \bigcup _ { t } F _ { t }$ and $\bigcap _ { t } F _ { t }$ for $\textstyle \bigcup _ { t \in T } F _ { t }$ and $\cap _ { t \in T } F _ { t }$ . When the index set of the index family $\mathcal { F }$  is a Cartesian product $S \times T$ then we usually denote its elements by $F _ { s t }$ instead of $F _ { \langle s , t \rangle }$ and we say that $\mathcal { F }$ is a doubly indexed family. We denote it as $\{ F _ { s t } \colon s \in \dot { S } , \ t \in T \}$ or simply $\{ F _ { s t } \}$ . In such a case we will write $\textstyle \bigcup _ { s \in S , t \in T } F _ { s t }$ or $\textstyle \bigcup _ { s , t } F _ { s t }$ for $\textstyle \bigcup _ { \langle s , t \rangle \in S \times T } F _ { s t }$ and $\cap _ { s \in S , t \in T } F _ { s t }$ or $\cap _ { s , t } F _ { s t }$ for $\textstyle \bigcap _ { \langle s , t \rangle \in S \times T } F _ { s t }$ . If $S = T$ we will also write $\textstyle \bigcup _ { s , t \in T } F _ { s t }$ and $\textstyle \bigcap _ { s , t \in T } F _ { s t }$ 

 The following properties are easy to verify: 

$$
x \in \bigcup_ {t \in T} F _ {t} \Leftrightarrow \exists t \in T (x \in F _ {t}) \qquad \text { and } \qquad x \in \bigcap_ {t \in T} F _ {t} \Leftrightarrow \forall t \in T (x \in F _ {t});
$$

$$
\bigcup_ {t \in T} F _ {t} = F _ {p} = \bigcap_ {t \in T} F _ {t} \qquad \text { for } T = \{p \};
$$

$$
\bigcup_ {t \in T} F _ {t} = F _ {p} \cup F _ {q} \quad \text { and } \quad \bigcap_ {t \in T} F _ {t} = F _ {p} \cap F _ {q} \quad \text { for } T = \{p, q \}.
$$

It is also easy to see that for any formula $\varphi ( t , x )$ and sets $T , X$ 

$$
\bigcup_ {t \in T} \{x \in X \colon \varphi (t, x) \} = \{x \in X \colon \exists t \in T (\varphi (t, x)) \}
$$

$$
\bigcap_ {t \in T} \{x \in X \colon \varphi (t, x) \} = \{x \in X \colon \forall t \in T (\varphi (t, x)) \}.
$$

Other properties of these operations are listed in the exercises. 

The behavior of generalized union and intersection under the action of image and preimage of a function is described in the next theorem. 

Theorem 2.3.1 If $f \in Y ^ { X } , \{ F _ { t } \} _ { t \in T }$ is an indexed family of subsets of X, $\{ G _ { t } \} _ { t \in T }$ is an indexed family of subsets of $Y , A , B \subset X$ , and $C , D \subset Y$ then 

(a) $\begin{array} { r } { f \left[ \bigcup _ { t \in T } F _ { t } \right] = \bigcup _ { t \in T } f [ F _ { t } ] , } \end{array}$ 

(b) $\begin{array} { r } { f \left[ \bigcap _ { t \in T } F _ { t } \right] \subset \bigcap _ { t \in T } f [ F _ { t } ] . } \end{array}$ ; 

(c) $f [ A ] \setminus f [ B ] \subset f [ A \setminus B ]$ ; 

(d) $\textstyle f ^ { - 1 } \left( \bigcup _ { t \in T } G _ { t } \right) = \bigcup _ { t \in T } f ^ { - 1 } ( G _ { t } )$ ; 

(e) $\begin{array} { r } { f ^ { - 1 } \left( \bigcap _ { t \in T } G _ { t } \right) = \bigcap _ { t \in T } f ^ { - 1 } ( G _ { t } ) , } \end{array}$ ; 

(f) $f ^ { - 1 } ( A ) \setminus f ^ { - 1 } ( B ) = f ^ { - 1 } ( A \setminus B ) .$ 

The proof is left as an exercise. 

For an indexed family $\{ F _ { t } \colon t \in T \}$ we define its Cartesian product by 

$$
\prod_ {t \in T} F _ {t} = \{h \in Z ^ {T}: \forall t \in T (h (t) \in F _ {t}) \},
$$

where $\textstyle Z = \bigcup _ { t \in T } F _ { t }$ . If all the sets $F _ { t }$ are identical, $F _ { t } = Y$ , then $\textstyle \prod _ { t \in T } F _ { t } =$ $Y ^ { T }$ . The set $\bar { Y } ^ { T }$ is called a Cartesian power of the set Y. 

For $t \in T$ the function $p _ { t } \colon \prod _ { t \in T } F _ { t } \to F _ { t }$ defined by $p _ { t } ( x ) = x ( t )$ is called the projection of $\Pi _ { t \in T } F _ { t }$ onto $F _ { t }$ 

Remark For $T$ a two-element set $\{ a , b \}$ the Cartesian products $\Pi _ { t \in T } F _ { t }$ and $F _ { a } \times F _ { b }$ are diferent. (The first one is a set of functions on $T$ , the second one is a set of ordered pairs.) However, there is a natural identification of every element $\{ \langle a , x \rangle , \langle b , y \rangle \}$ from $\Pi _ { t \in T } F _ { t }$ with $\langle x , y \rangle \in F _ { a } \times F _ { b }$ . Therefore we will usually identify these products. 

Theorem 2.3.2 A product $\Pi _ { t \in T } F _ { t }$ of nonempty sets $F _ { t }$ is nonempty. 

Proof The choice function f for the family $\{ F _ { t } \colon t \in T \}$ , which exists by Theorem 2.2.4, is an element of $\Pi _ { t \in T } F _ { t }$  

Remark Theorem 2.3.2 easily implies Theorem 2.2.4. Thus its statement is equivalent to the axiom of choice. However, we do not need the axiom of choice to prove Theorem 2.3.2 if either $T$ is finite or $\begin{array} { r } { \prod _ { t \in T } F _ { t } = Y ^ { T } } \end{array}$ 

## EXERCISES

1 Prove that for every indexed families $\{ F _ { t } \} _ { t \in T }$ and $\{ G _ { t } \} _ { t \in T }$ 

$$
\bigcap_ {t \in T} (F _ {t} \cap G _ {t}) = \bigcap_ {t \in T} F _ {t} \cap \bigcap_ {t \in T} G _ {t},
$$

$$
\text {(b)} \quad \bigcup_ {t \in T} (F _ {t} \cup G _ {t}) = \bigcup_ {t \in T} F _ {t} \cup \bigcup_ {t \in T} G _ {t},
$$

(c) $\begin{array} { r } { \bigcap _ { t \in T } F _ { t } \cup \bigcap _ { t \in T } G _ { t } = \bigcap _ { s , t \in T } ( F _ { s } \cup G _ { t } ) \subset \bigcap _ { t \in T } ( F _ { t } \cup G _ { t } ) . } \end{array}$ , and 

$$
\bigcup_ {t \in T} F _ {t} \cap \bigcup_ {t \in T} G _ {t} = \bigcup_ {s, t \in T} (F _ {s} \cap G _ {t}) \supset \bigcup_ {t \in T} (F _ {t} \cap G _ {t}).
$$

Give examples showing that the inclusions cannot be replaced by equalities. 

2 Show that for every indexed family $\{ F _ { t } \} _ { t \in T }$ and every set A 

$$
\text {(a)} \quad A \setminus \bigcap_ {t \in T} F _ {t} = \bigcup_ {t \in T} (A \setminus F _ {t}) \text {and} A \setminus \bigcup_ {t \in T} F _ {t} = \bigcap_ {t \in T} (A \setminus F _ {t}),
$$

$$
\text {(b)} \quad \bigcap_ {t \in T} (A \cup F _ {t}) = A \cup \bigcap_ {t \in T} F _ {t} \text {and} \bigcup_ {t \in T} (A \cap F _ {t}) = A \cap \bigcup_ {t \in T} F _ {t}.
$$

3 Prove that for every indexed families $\{ F _ { t } \} _ { t \in T }$ and $\{ G _ { t } \} _ { t \in T }$ 

$$
\mathrm{(a)} \quad \left(\bigcup_ {t \in T} F _ {t}\right) \times \left(\bigcup_ {t \in T} G _ {t}\right) = \bigcup_ {s, t \in T} (F _ {s} \times G _ {t}),
$$

$$
\text {(b)} \quad \left(\bigcap_ {t \in T} F _ {t}\right) \times \left(\bigcap_ {t \in T} G _ {t}\right) = \bigcap_ {s, t \in T} (F _ {s} \times G _ {t}).
$$

4 Show that $\begin{array} { r } { \bigcup _ { s \in S } \bigcap _ { t \in T } F _ { s t } \subset \bigcap _ { t \in T } \bigcup _ { s \in S } F _ { s t } } \end{array}$ for every doubly indexed family $\{ F _ { s t } \colon s \in \tilde { S } , \ t \in \top \}$ 

5 Prove Theorem 2.3.1(a), (b), and (c). Show, by giving examples, that the inclusions in parts (b) and (c) cannot be replaced by equality. 

6 Prove Theorem 2.3.1(d), (e), and (f). 

7 For $r , s \in \mathbb { R }$ let $A _ { r } = \left[ r , r + 1 \right]$ and $\boldsymbol { B _ { r s } } = [ r , s )$ . Calculate $\textstyle \bigcup _ { s \leq 0 } \bigcap _ { r \geq s } A _ { r }$ , $\begin{array} { r } { \bigcap _ { s \leq 0 } \bigcup _ { r \geq s } A _ { r } , \bigcup _ { r \leq 0 } \bigcap _ { s > r } B _ { r s } } \end{array}$ , and $\cap _ { r \leq 0 } \bigcup _ { s > r } B _ { r s }$ 

## 2.4 Partial- and linear-order relations

A binary relation R on X is antisymmetric if 

$$
x R y \&y R x \rightarrow x = y
$$

for every $x , y \in X$ 

A relation R on X is a (partial-)order relation if it is reflexive, transitive, and antisymmetric. Order relations are usually denoted by the symbols ≤, $\preceq , \mathrm { ~ o r \ll . ~ H \leq }$ is a partial-order relation then the ordered pair $\langle X , \leq \rangle$ is called a partially ordered set (abbreviated also as poset). 

Examples 1. The relations ≤ and ≥ on R are order relations. 

2. For any set X the relation ⊂ is an order relation on ${ \mathcal { P } } ( X )$ 

3. The relation | on the set $\{ 2 , 3 , 4 , \hdots \}$ defined by 

n|m if and only if n divides m 

is an order relation. 

An element $m \in X$ of an ordered set $\langle X , \leq \rangle$ is minimal if for every $x \in X$ the condition $x \leq m$ implies $x = m$ . Similarly, an element $M \in X$ is maximal if for every $x \in X$ the condition $x \ge M$ implies $x = M$ 

An element $m \in X$ is the smallest element (least element or first element) in X if $m \leq x$ for every $x \in X$ , and $M \in X$ is the greatest element (largest element or last element) in X if $x \leq M$ for every $x \in X$ 

Theorem 2.4.1 Let $\langle X , \leq \rangle$ be a partially ordered set. 

(a) X can have at most one greatest and one smallest element. 

(b) The smallest element of X, if it exists, is the only minimal element of X. 

(c) The greatest element of X, if it exists, is the only maximal element of X. 

Proof (a) If a and b are the smallest elements of X then $a \leq b$ and $b \leq a$ Hence $a = b .$ The argument for the greatest element is the same. 

(b) If a is the smallest element of X then it is minimal, since the condition $x \leq a$ combined with $a \leq x .$ , which is true for every x, implies $x = a$ Moreover, if m is minimal, then $a \leq m$ , since a is the smallest element, and, by minimality of $m , m = a .$ 

(c) The argument is the same as in (b). 

Examples 1. $\langle \mathbb { R } , \leq \rangle$ has neither minimal nor maximal elements. 

2. $\langle [ 0 , 1 ] , \leq \rangle$ has 0 as the least element and 1 as the last element. 

3. ∅ is the smallest element of $\langle { \mathcal { P } } ( X ) , \subset \rangle$ . X is the greatest element of $\langle { \mathcal { P } } ( X ) , \subset \rangle$ 

4. Let $\langle \{ 2 , 3 , 4 , \dots \} , | \rangle$ be defined as before. It does not have any maximal element. A number m is minimal in this order if and only if m is a prime number. (Thus $\langle \{ 2 , 3 , 4 , \dots \} , | \rangle$ has infinitely many minimal elements!) 

A relation R on X is connected if 

$$
x R y \vee y R x
$$

for every x, $y \in X$ . An order relation $\leq$ is called a linear-order relation if it is connected. In this case we also say that $\langle X , \leq \rangle$ (or just X) is linearly ordered. 

Examples 1. $\langle \mathbb { R } , \leq \rangle$ is linearly ordered. 

2. $\langle { \mathcal { P } } ( X ) , \subset \rangle$ is linearly ordered if and only if X has at most one element. 

3. $\langle \{ 2 , 3 , 4 , \dots \} , | \rangle$ is not linearly ordered, since neither $2 | 3$ nor 3|2. 

4. The relation $\leq$ on N is a linear-order relation. 

Theorem 2.4.2 If $\langle X , \leq \rangle$ is linearly ordered then every minimal element in X is the smallest element and every maximal element in X is the greatest element. In particular, linearly ordered sets can have at most one maximal element and at most one minimal element. 

The proof is left as an exercise. 

Notice that $\mathrm { i f ~ \le ~ }$ is an order relation on a set X and $Y \subset X$ then the relation $\leq \cap ( Y \times Y )$ is an order relation on Y. It is called the restriction of $\leq \mathrm { t o ~ } Y$ . We often write $\langle Y , \leq \rangle$ in place of $\langle Y , \leq \cap ( Y \times Y ) \rangle$ 

Notice also that a subset of a partially ordered set is partially ordered and a subset of a linearly ordered set is linearly ordered. 

In general, for any partial order denoted by $\leq$ we will write $\geq \mathrm { f o r } \ ( \leq ) ^ { - 1 }$ and define relations $< \mathrm { a n d } >$ by 

$$
x <   y \Leftrightarrow x \leq y \& x \neq y
$$

and 

$$
x > y \Leftrightarrow x \geq y \& x \neq y.
$$

## EXERCISES

1 Prove that the restriction $\leq \cap ( Y \times Y )$ of an order relation $\leq$ on $X$ is an order relation, provided $Y \subset X$ . Show that $\langle Y , \leq \rangle$ is linearly ordered if $\langle X , \leq \rangle$ is linearly ordered. Give an example such that $\langle Y , \leq \rangle$ is linearly ordered, while $\langle X , \leq \rangle$ is not. 

2 Find all minimal, maximal, greatest, and smallest elements of $\langle { \mathcal { F } } , \subset \rangle$ , where $\mathcal { F } = \{ X \subset \mathbb { N } \colon X$ is finite}. 

3 Prove Theorem 2.4.2. 

4 A binary relation $R \subset X \times X$ is said to be a preorder relation if it is transitive and reflexive. 

Let $\preceq ( X \times X$ be a preorder relation. 

(a) Show that the relation ∼ on X defined by 

$$
x \sim y \Leftrightarrow x \preceq y \& y \preceq x
$$

is an equivalence relation on $X$ 

(b) Define the relation $\leq$ on the family $X / \sim$ of all equivalence classes for $\sim$ by 

$$
[ x ] \leq [ y ] \Leftrightarrow x \preceq y.
$$

Show that the relation $\leq$ is well defined and that it is a partial-order relation. 

Chapter 3 

# Natural numbers, integers, and real numbers

From the results of Section 1.2 it is clear that sets such as $\emptyset , \{ \emptyset \} , \{ \emptyset , \{ \emptyset \} \}$ $\{ \{ \emptyset \} \}$ , and so forth exist. Using the axiom of infinity we can also conclude that we can build similar infinite sets. But how do we construct complicated sets, such as the sets of natural and real numbers, if the only tools we have to build them are the empty set $\varnothing$ and “braces” $\{ \cdot \} \ ?$ We will solve this problem by identifying the aforementioned objects with some specific sets. 

Briefly, we will identify the number 0 with the empty set ∅, and the other natural numbers will be constructed by induction, identifying n with $\{ 0 , \ldots , n - 1 \}$ . The existence of the set N of all natural numbers is guaranteed by the infinity axiom. The real numbers from the interval [0, 1] will be identified with the set of functions $\{ 0 , 1 \} ^ { \mathbb { N } }$ , where an infinite sequence $a \colon \mathbb { N } \to \{ 0 , 1 \}$ is identified with the binary expansion of a number, that is, with $\textstyle \sum _ { n \in \mathbb { N } } { \bar { a ( n ) } } / 2 ^ { n + 1 }$ . The details of these constructions are described in the rest of this chapter. 

## 3.1 Natural numbers

In this section we will find a set that represents the set N of natural numbers in our set-theoretic universe. For this, we need to find for each natural number n a set that represents it. Moreover, we will have to show that the class of all such defined natural numbers forms a set. 

When picking the natural numbers, we will have to pick also the ordering relation < between them. Essentially, the only relation that we have available for this purpose is the relation ∈. Thus, we will choose the natural numbers to satisfy the following principle: 

$$
m <   n \text {   if   and   only   if   } m \in n.
$$

Also, since natural numbers are going to be distinguished by the relation ∈ of being an element, it seems to be natural to have the following intuitive principle: 

Each natural number n should have n elements. 

These two principles give us no choice about our definition. 

By the second principle we have $0 = \emptyset$ 

Now suppose that we have already defined n and want to define $n + 1$ Since $n < n + 1$ we have $n \in n + 1$ . Also, for every $m \in n$ we have $m < n$ so $m < n + 1$ and $m \in n + 1$ . In particular, $n \subset n + 1$ and $n \cup \{ n \} \subset n + 1$ But n has n elements, so $n \cup \{ n \}$ has $n + 1$ elements, since $n \not \in n ,$ , as $n \not \prec n$ . Therefore $n \cup \{ n \} \subset n + 1$ and both sets have $n + 1$ elements. Thus, $n + 1 = n \cup \{ n \}$ 

By the foregoing discussion we see that $0 = \emptyset , 1 = \{ 0 \} = \{ \emptyset \} , 2 =$ $\{ 0 , 1 \} = \{ \varnothing , \{ \varnothing \} \} , 3 = \{ 0 , 1 , 2 \} = \{ \varnothing , \{ \varnothing \} , \{ \varnothing , \{ \varnothing \} \} \}$ , and so forth. 

Now, showing that the class of all such numbers forms a set is another problem. We will use for this the axiom of infinity. We will also make sure that the following three principles are satisfied, where $S ( n ) = n + 1$ is known as a successor of n and P stands for some property of natural numbers. 

P1 $0 \neq S ( n )$ for every $n \in \mathbb { N }$ 

P2 If $S ( n ) = S ( m )$ then $n = m$ for every n, $m \in \mathbb { N }$ 

P3 If 0 has property P and for every $n \in \mathbb { N }$ 

S(n) has property P provided n has property P 

then n has property P for every $n \in \mathbb { N }$ 

Principles P1–P3, known as the Peano axioms of arithmetic, are the most commonly accepted axioms for the natural numbers. Axiom P3 is the principle of mathematical induction. 

Notice that the definition of the successor operator $S ( x ) = x \cup \{ x \}$ from the axiom of infinity coincides with the definition given in this section, since $S ( n ) = n + 1 = n \cup \{ n \}$ 

Now we are ready to construct the set N. 

Theorem 3.1.1 There exists exactly one set N such that 

(1) $\varnothing \in \mathbb { N } .$ 

(2) $x \in \mathbb { N } \to S ( x ) \in \mathbb { N }$ for every x, and 

(3) if K is any set that satisfies (1) and (2) then $\mathbb { N } \subset K$ 

Proof By the axiom of infinity there exists at least one set X satisfying (1) and (2). Let 

$$
\mathcal {F} = \{Y \in \mathcal {P} (X) \colon \emptyset \in Y \& \forall x \in Y (S (x) \in Y) \}
$$

and put $\mathbb { N } = \cap \mathscr { F }$ . It is easy to see that the intersection of any nonempty family of sets satisfying (1) and (2) still satisfies (1) and (2). To see that (3) holds let K satisfy (1) and (2). Then $X \cap K \in { \mathcal { F } }$ and $\mathbb { N } = \cap \mathcal { F } \subset$ $X \cap K \subset K$ . Theorem 3.1.1 is proved.  

The set N from Theorem 3.1.1 will be called the set of natural numbers. Natural numbers will usually be denoted by the letters $m , n , p , \ldots .$ The operation $S ( n )$ is the counterpart to $( n + 1 )$ . Thus for a natural number n we will henceforth write $n + 1$ instead of $S ( n )$ 

The set of natural numbers will also be denoted by the symbol $\omega .$ 

Notice that condition (3) of Theorem 3.1.1 can be rephrased as follows: 

$$
[ 0 \in K \&\forall x (x \in K \rightarrow S (x) \in K) ] \text { implies } \mathbb {N} \subset K.\tag{3.1}
$$

If we additionally know that $K \subset \mathbb { N }$ then (3.1) can be expressed as 

$$
[ 0 \in K \&\forall n (n \in K \rightarrow n + 1 \in K) ] \text { implies } \mathbb {N} = K.\tag{3.2}
$$

Property (3.2) is called the induction property of the set of natural numbers and the proofs that use it are cited as proofs by induction. 

It is easy to see that the induction property (3.2) implies axiom P3 if we put $K = \{ n \in \mathbb { N } \colon n$ has property $P \}$ . Axiom P2 follows from Theorem 3.1.2(f). To see that N satisfies P1 just notice that $0 ~ = ~ \emptyset$ and $S ( n ) = n \cup \{ n \}$ is clearly nonempty. 

Essentially all the known properties of the natural numbers can be deduced from these definitions and the ZFC axioms.<sup>1</sup> However, we will restrict ourselves only to those properties that are more connected with our representation of the natural numbers and to those that will be of more use in what follows. 

Theorem 3.1.2 For every natural numbers m, n, and p 

(a) $m \subset m + 1$ and $m \in m + 1$ ; 

(b) if $x \in m$ then $x \in \mathbb { N }$ 

(c) $i f m \in n$ then $m + 1 \subset n ;$ 

(d) if $m \in n$ and $n \in p$ then $m \in p$ ; 

(e) $m \not \in m ;$ 

(f) $i f n + 1 = m + 1 \ t h e n \ n = m ;$ 

(g) $m \subset n$ if and only if $m = n \ o r \ m \in n .$ 

(h) $m \subset n o r n \subset m .$ 

Proof (a) This follows immediately from the definition $m + 1 = m \cup \{ m \}$ 

(b) The proof follows by induction. Let 

$$
K = \{n \in \mathbb {N} \colon \forall x (x \in n \rightarrow x \in \mathbb {N}) \}.
$$

Notice that $0 = \varnothing \in K$ , since there is no $x \in 0 .$ . Now let $n \in K$ and $x \in n + 1$ . Since $n + 1 = n \cup \{ n \}$ we have two cases: If $x \in n$ then $x \in \mathbb { N }$ since $n \in K$ ; if $x \in \{ n \}$ then $x = n$ and also $x \in \mathbb { N } .$ . Thus $n \in K$ implies $n + 1 \in K$ . Hence, by (3.2), $K = \mathbb { N }$ and (b) is proved. 

(c) The proof is left as an exercise. 

(d) Since $m \in n$ and, by $( \mathrm { a } ) , n \subset n + 1$ we have $m \in n + 1$ . But, by (c), $n \in p$ implies $n + 1 \subset p . \mathrm { ~ S o ~ } m \in p .$ 

(e) This can be easily proved by induction. It is left as an exercise. 

(f) This is left as an exercise. 

(g) ⇐: If m = n then $m \subset n .$ . If $m \in n$ then, by (a) and $( \mathrm { c } ) , m \subset$ $m + 1 \subset n$ 

⇒: Fix $m \in \mathbb { N }$ and consider the set 

$$
K = \{n \in \mathbb {N} \colon m \subset n \to [ m \in n \lor m = n ] \}.
$$

It is enough to show that $K = \mathbb { N } .$ 

First notice that $0 \in K$ since $m \subset 0 = \emptyset$ implies $m = \varnothing = 0$ 

Now assume that $n \in K$ . By induction it is enough to show that $n + 1 \in K$ . So assume that $m \subset n + 1 = n \cup \{ n \}$ . If $m \not \subset n$ then $n \in m$ and, by $( \mathrm { c } ) , n + 1 \subset m \subset n + 1$ , that is, $m = n + 1$ . If $m \subset n$ then, since $n \in K$ , either $m \in n { \mathrm { ~ o r ~ } } m = n$ . But in both cases $m \in n \cup \{ n \} = n + 1$ ; so $n + 1 \in K$ 

(h) Define the set 

$$
K = \{m \in \mathbb {N} \colon \forall n \in \mathbb {N} (n \not \in m \to m \subset n) \}.
$$

First we will show that $K = \mathbb { N }$ 

First notice that $0 \in K$ , since $0 = \varnothing \subset n$ for every n. 

Now assume that $m \in K$ . We will show that this implies $m + 1 \in K$ So let $n \in \mathbb { N }$ be such that $n \not \in m + 1 = m \cup \{ m \}$ . Then $n \neq m$ and $n \not \in m$ But $m \in K$ and $n \not \in$ m imply that $m \subset n$ . This last condition and $n \neq m$ imply in turn, by (g), that m ∈ n and, by (c), $m + 1 \subset n$ . Thus we conclude that $n \in K$ implies $n + 1 \in K$ and, by induction, that $K = \mathbb { N }$ 

Now, to finish the proof, let $n , m \in \mathbb { N }$ . If $n \subset m$ then the conclusion is correct. So assume that n $\not \subset m$ . Then, by $( \mathbf { g } ) , n \notin m$ . Since $m \in \mathbb { N } = K$ we conclude $m \subset n$  

From Theorem 3.1.2 it follows immediately that every natural number $n = \{ 0 , 1 , 2 , \ldots , n - 1 \}$ . However, we cannot express it in the formal language of set theory, since the symbol $\cdots$ does not belong to its language. We can only express it using infinitely many sentences, one for each natural number. On the other hand, this informal expression is more intuitive for most mathematicians than the formal definition. We will often use it to describe the set of natural numbers less than a fixed number. In particular, we will very often write 2 instead of $\{ 0 , 1 \}$ 

Let us also define for natural numbers m and n 

$$
m <   n \text { if   and   only   if } m \in n
$$

and 

$$
m \leq n \text { if   and   only   if } m \subset n.
$$

It is not dificult to see that these definitions imply the properties of < and $\leq$ that we usually associate with them. 

We will finish this section by defining on the set N the arithmetic operations of sum, product, and exponentiation. The definitions are by induction and go as follows: 

$$
n + 0 = n; \quad n + (m + 1) = (n + m) + 1, \text {   where   } k + 1 \text {   stands   for   } S (k).
$$

$$
\begin{array}{c} n   0 = 0; \quad n   (m + 1) = (n   m) + n. \\ n ^ {0} = 1; \quad n ^ {m + 1} = n ^ {m}   n. \end{array}
$$

It can be proved, by induction, that these operations satisfy all known properties of the standard operations. 

## EXERCISES

1 Prove that if $\mathcal { F }$ is a nonempty family such that every $F \in { \mathcal { F } }$ satisfies (1) and (2) from Theorem 3.1.1 then $\cap { \mathcal { F } }$ also satisfies these conditions. 

2 Prove by induction Theorem 3.1.2(c), (e), and (f). 

## 3.2 Integers and rational numbers

Intuitively, we will define integers as diferences $n - m$ of two natural numbers. The formalization of this intuition has, however, two problems. First, we do not have an operation − defined as of yet. Thus we will talk about ordered pairs $\langle n , m \rangle$ of natural numbers, thinking of them as $n - m$ . However, representing the number $n - m$ as $\langle n , m \rangle$ is not unique: $1 = 2 - 1 = 3 - 2$ $\mathrm { S o }$ , instead, we will use equivalence classes of pairs of natural numbers, where the equivalence relation $E$ on $\mathbb { N } \times \mathbb { N }$ is defined by the formula: 

$$
\langle n, m \rangle E \langle n ^ {\prime}, m ^ {\prime} \rangle \Leftrightarrow n + m ^ {\prime} = n ^ {\prime} + m.\tag{3.3}
$$

Now the set of integers $\mathbb { Z }$ is defined as the quotient class $( \mathbb { N } \times \mathbb { N } ) / E$ 

We define a relation $\leq$ on $\mathbb { Z }$ by 

$$
[ \langle n, m \rangle ] \leq [ \langle n ^ {\prime}, m ^ {\prime} \rangle ] \Leftrightarrow n + m ^ {\prime} \leq n ^ {\prime} + m.\tag{3.4}
$$

The arithmetic operations on $\mathbb { Z }$ are defined as follows: 

$$
\begin{array}{c} [ \langle n, m \rangle ] + [ \langle n ^ {\prime}, m ^ {\prime} \rangle ] = [ \langle n + n ^ {\prime}, m + m ^ {\prime} \rangle ]. \\ [ \langle n, m \rangle ] - [ \langle n ^ {\prime}, m ^ {\prime} \rangle ] = [ \langle n, m \rangle ] + [ \langle m ^ {\prime}, n ^ {\prime} \rangle ]. \\ [ \langle n, m \rangle ] [ \langle n ^ {\prime}, m ^ {\prime} \rangle ] = [ \langle n   n ^ {\prime} + m   m ^ {\prime}, n   m ^ {\prime} + m   n ^ {\prime} \rangle ]. \end{array}
$$

We will leave as an exercise the proof that $E$ is an equivalence relation, that the preceding operations are well defined (i.e., they do not depend on the choice of representatives of equivalence classes), and that they have the properties we know from algebra. 

Following the same path, we define the set $\mathbb { Q }$ of rational numbers as ordered pairs $\langle a , b \rangle$ of integers representing of $a / b .$ . More precisely, we define an equivalence relation $E ^ { \prime }$ on $\mathbb { Z } \times \mathbb { Z }$ by 

$$
\langle a, b \rangle E ^ {\prime} \langle a ^ {\prime}, b ^ {\prime} \rangle \Leftrightarrow [ a b ^ {\prime} = a ^ {\prime} b \& b \neq 0 \neq b ^ {\prime} ] \text {or} [ b = b ^ {\prime} = 0 ].
$$

Then 

$$
\mathbb {Q} = \{[ \langle a, b \rangle ]: a, b \in \mathbb {Z} \& b \neq 0 \},
$$

where $[ \langle a , b \rangle ]$ is an equivalence class with respect to $E ^ { \prime }$ . We define a relation $\leq$ and arithmetic operations on $\mathbb { Z }$ as follows: 

$$
\begin{array}{c} [ \langle a, b \rangle ] + [ \langle a ^ {\prime}, b ^ {\prime} \rangle ] = [ \langle a   b ^ {\prime} + a ^ {\prime}   b, b   b ^ {\prime} \rangle ]; \\ [ \langle a, b \rangle ]   [ \langle a ^ {\prime}, b ^ {\prime} \rangle ] = [ \langle a   a ^ {\prime}, b   b ^ {\prime} \rangle ]; \\ [ \langle a, b \rangle ] \leq [ \langle a ^ {\prime}, b ^ {\prime} \rangle ] \Leftrightarrow b \geq 0   \&   b ^ {\prime} \geq 0   \&   a   b ^ {\prime} \leq a ^ {\prime} b. \end{array}
$$

As before, we will leave as an exercise the proof that $E ^ { \prime }$ is an equivalence relation, that the preceding definitions are well defined, and that they have the desired properties. 

## EXERCISES

1 Prove that the relation E defined by (3.3) is an equivalence relation. 

2 Show that $\leq$ on Z defined by (3.4) is well defined and is a linear-order relation. 

## 3.3 Real numbers

In the previous section we constructed integers from the natural numbers and rational numbers from the integers. Both constructions were primarily algebraic. This was possible since the rational numbers are the algebraic completion of the set of natural numbers. The same approach, however, cannot be used in a construction of the real numbers, since there are real numbers of no simple algebraic relation to rational numbers. 

The crucial geometric property that is often used to described real numbers is that the real line “does not have holes.” This intuition was used by Dedekind to define the set R of real numbers as follows. 

A subset A of Q is said to be a Dedekind cut if A does not contain a largest element and is a proper initial segment of Q, that is, $\varnothing \neq A \neq \mathbb { Q }$ and A contains every $p \leq q$ provided $q \in A$ . Now, R can be defined as the set of all Dedekind cuts, intuitively identifying A with a real number sup A. Then for Dedekind cuts A and B we can define 

$$
A + B = \{p + q \colon p \in A \& q \in B \}
$$

and 

$$
A \leq B \Leftrightarrow A \subset B.
$$

Similarly, we can define the product A B of two numbers (though the definition must be done more carefully, since the product of two negative numbers is positive). 

Another approach for the definition of real numbers is to use their numerical expansions. This approach is a little more messy, but it better fits the methods of this course. So we will include it here too. 

The construction of real numbers that follows will be done in two steps. First, consider the set $2 ^ { \mathbb { N } }$ of all sequences $s \colon \mathbb { N }  \{ 0 , 1 \}$ . It is usually called the Cantor set. (The classical Cantor “ternary” set can be obtained from this set by identifying a sequence $a \in 2 ^ { \mathbb { N } }$ with $\textstyle \sum _ { n \in \mathbb { N } } { 2 a _ { n } } / 3 ^ { n + 1 }$ . See Section 6.2 for more details.) We would like to identify a sequence $a \in 2 ^ { \mathbb { N } }$ with the real number $\scriptstyle \sum _ { n \in \mathbb { N } } { a _ { n } } / 2 ^ { n + 1 }$ . However, this identification function is not one-to-one. To correct it, we will define [0, 1] as the quotient class 

$2 ^ { \mathbb { N } } / E$ , where $a E b$ if and only if $a = b$ or there exists an $n \in \mathbb N$ such that for every $k \in \mathbb N$ 

$$
[ k <   n \rightarrow a _ {k} = b _ {k} ] \&[ a _ {n} = 1 \&b _ {n} = 0 ] \&[ k > n \rightarrow (a _ {k} = 0 \&b _ {k} = 1) ].\tag{3.5}
$$

We will leave as an exercise the proof that E is indeed an equivalence relation. 

The linear-order relation $\leq$ on [0, 1] can be defined by 

$$
[ a ] \leq [ b ] \Leftrightarrow [ a ] = [ b ] \vee \exists n \in \mathbb {N} \left[ a _ {n} <   b _ {n} \& \forall k \in n (a _ {k} = b _ {k}) \right].\tag{3.6}
$$

Again, we will not prove the correctness of this definition. 

Numbers 0 and 1 in [0, 1] are defined as equivalence classes of functions constantly equal to 0 and 1, respectively. Then we define 

$$
[ 0, 1) = [ 0, 1 ] \setminus \{1 \}, (0, 1 ] = [ 0, 1 ] \setminus \{0 \}, (0, 1) = [ 0, 1 ] \setminus \{0, 1 \}.
$$

The set R of real numbers is defined as $\mathbb { Z } \times [ 0 , 1 )$ , where intuitively we identify a pair $\langle k , r \rangle$ with $k + r$ . In particular, we can define $\leq$ on R by 

$$
\langle k, r \rangle \leq \langle l, s \rangle \Leftrightarrow k <   l \vee (k = l \& r \leq s).\tag{3.7}
$$

In the remainder of this section we will recall some geometric and topological properties of the n-dimensional Euclidean space $\mathbb { R } ^ { n } \ ( n \in \mathbb { N } )$ . In particular, the distance between two points $p ~ = ~ \langle p _ { 1 } , \ldots , p _ { n } \rangle$ and $q =$ $\langle q _ { 1 } , \ldots , q _ { n } \rangle$ of $\mathbb { R } ^ { n }$ is given by the formula 

$$
d (p, q) = \sqrt {\sum_ {i = 1} ^ {n} \left(p _ {i} - q _ {i}\right) ^ {2}}.
$$

The open ball in $\mathbb { R } ^ { n }$ centered at $p \in \mathbb { R } ^ { n }$ and with radius $\varepsilon > 0$ is defined as 

$$
B (p, \varepsilon) = \{q \in \mathbb {R} ^ {n} \colon d (p, q) <   \varepsilon \}.
$$

A subset $U$ of $\mathbb { R } ^ { n }$ is open if $U$ is a union of some family of open balls in $\mathbb { R } ^ { n }$ . The family $\tau$ of all open subsets of $\mathbb { R } ^ { n }$ is called the (natural) topology on $\mathbb { R } ^ { n }$ and is closed under finite intersections and arbitrary unions. 

A set $F \subset \mathbb { R } ^ { n }$ is closed if its complement $\mathbb { R } ^ { n } \setminus F$ is open. Notice that finite unions of closed sets and arbitrary intersections of closed sets are also closed. 

For a subset $S$ of $\mathbb { R } ^ { n }$ its interior int(S) is defined as the largest open subset of $S _ { ; }$ , that is, 

$$
\operatorname{int} (S) = \bigcup \left\{U \subset \mathbb {R} ^ {n}: U \text {is open in} \mathbb {R} ^ {n} \right\}.
$$

The closure of $S$ is the smallest closed set containing $S _ { ; }$ , that is, 

$$
\operatorname{cl} (S) = \bigcap \left\{F \supset S: F \text {   is   closed   in   } \mathbb {R} ^ {n} \right\}.
$$

A subset D of $\mathbb { R } ^ { n }$ is dense in $\mathbb { R } ^ { n }$ if c $. ( D ) = \mathbb { R } ^ { n }$ or, equivalently, when $D \cap U \neq \emptyset$ for every nonempty open set $U \subset \mathbb { R } ^ { n }$ . In particular, $\mathbb { Q } ^ { n }$ is a dense subset of $\mathbb { R } ^ { n }$ . A subset N of $\mathbb { R } ^ { n }$ is nowhere dense if int $( \mathrm { c l } ( N ) ) = \emptyset$ 

Now let us recall a few more specific properties of $\mathbb { R } ^ { n }$ . A function $f \colon  { \mathbb { R } } ^ { n } \to  { \mathbb { R } } ^ { m }$ is continuous if $f ^ { - 1 } ( U ) = \{ x \in \mathbb { R } ^ { n } \colon f ( x ) \in U \}$ is open in $\mathbb { R } ^ { n }$ for every open set $U \subset \mathbb { R } ^ { m }$ . It is easy to see that for every dense subset D of $\mathbb { R } ^ { n }$ and continuous functions $f \colon  { \mathbb { R } } ^ { n } \to  { \mathbb { R } } ^ { m }$ and $g \colon { \mathbb { R } } ^ { n }  { \mathbb { R } } ^ { m }$ if $f ( d ) = g ( d )$ for every $d \in D$ then $f = g$ 

A subset B of $\mathbb { R } ^ { n }$ is bounded ${ \mathrm { i f ~ } } B \subset B ( p , \varepsilon )$ for some $p \in \mathbb { R } ^ { n }$ and $\varepsilon > 0$ . Closed, bounded subsets of $\mathbb { R } ^ { n }$ are called compact. One of the most important properties of compact subsets of $\mathbb { R } ^ { n }$ is given in the next theorem. 

Theorem 3.3.1 If $K _ { 0 } \supset K _ { 1 } \supset K _ { 2 } \supset \cdots$ is a decreasing sequence of compact nonempty subsets of $\mathbb { R } ^ { n }$ then their intersection $\cap _ { i = 0 } ^ { \infty } K _ { i }$ is nonempty. 

A subset C of $\mathbb { R } ^ { n }$ is connected if there do not exist two disjoint open sets $U , V \subset \mathbb { R } ^ { n }$ such that $U \cap C \neq \emptyset , V \cap C \neq \emptyset$ , and $C \subset U \cup V$ . Recall that any interval in R as well as any $\mathbb { R } ^ { n }$ are connected. 

A sequence $\{ p _ { k } \} _ { k = 0 } ^ { \infty }$ of points in $\mathbb { R } ^ { n }$ is a Cauchy sequence if for every $\varepsilon > 0$ there is a number N such that $d ( p _ { i } , p _ { j } ) < \varepsilon$ for every $i , j > N$ . Every Cauchy sequence in $\mathbb { R } ^ { n }$ has a limit point. This fact serves as a basis for the proof of the Baire category theorem, which follows. 

Theorem 3.3.2 (Baire category theorem) If $N _ { 0 } , N _ { 1 } , N _ { 2 } , \ldots$ is a sequence of nowhere-dense subsets of $\mathbb { R } ^ { n }$ then its union $\textstyle \bigcup _ { i = 0 } ^ { \infty } N _ { i }$ has an empty interior. 

## EXERCISES

1 Define the product of two real numbers using Dedekind’s definition of R. Show that your product has the distributive property, that is, that $a ( b + c ) = a b + a c$ for every $a , b , c \in \mathbb { R }$ 

2 Prove that the relation E defined by (3.5) is an equivalence relation. 

3 Show that $\leq \mathrm { o n } \left[ 0 , 1 \right]$ defined by (3.6) is well defined and is a linear-order relation. 

4 Prove that $\leq$ on R defined by (3.7) is a linear-order relation. 

Part II 

# Fundamental tools of set theory

Chapter 4 

# Well orderings and transfinite induction

## 4.1 Well-ordered sets and the axiom of foundation

A binary relation R on a set X is said to be well founded if every nonempty subset Y of X has an R-minimal element, that is, if 

$$
\forall Y \subset X [ Y \neq \emptyset \rightarrow \exists m \in Y \neg \exists y \in Y (y R m) ].
$$

Examples 1. For every finite linearly ordered set $\langle X , \leq \rangle$ the relation $<$ is well founded. 

2. The relation < on the set N of all natural numbers is well founded. This is known as the well-ordering principle for the natural numbers. It can be easily deduced from the principle of mathematical induction P3. (See also (3.2).) It is also a special case of the next example. 

3. The relation ∈ is well founded on every nonempty set X. This, however, does not follow from the axioms we have studied so far. For this we need the following axiom known as the axiom of foundation or regularity. This is the last of the axioms of ZFC. 

Foundation axiom (Skolem 1922; von Neumann 1925) Every nonempty set has an ∈-minimal element: 

$$
\forall x \left[ \exists y (y \in x) \rightarrow \exists y [ y \in x \&\neg \exists z (z \in x \&z \in y) ] \right].
$$

This axiom is not essential for this course. However, it is good to know some of its basic consequences. 

Theorem 4.1.1 x ∈ x for every x. 

Proof To obtain a contradiction assume that there exists a t such that $t \in t . { \mathrm { ~ P u t ~ } } x = \{ t \}$ . We will see that the axiom of foundation fails for x. 

Evidently, there exists a $y \in x$ , since $t \in x$ . Moreover, if $y \in x$ then $y \ = \ t$ But then, there exists a $z , \ z \ = \ t ,$ such that $z ~ = ~ t ~ \in ~ x$ and $z = t \in t = y$ , contradicting the axiom of foundation.  

Theorem 4.1.2 There is no infinite ∈-decreasing sequence, that is, there is no sequence $\langle x _ { n } \colon n \in \mathbb { N } \rangle$ such that $x _ { n + 1 } \in x _ { n }$ for all $n \in \mathbb { N }$ 

Proof Otherwise the set $\{ x _ { n } \colon n \in \mathbb { N } \}$ would have no ∈-minimal element.  

A binary relation $\leq$ on X is a well-ordering relation if $\langle X , \leq \rangle$ is linearly ordered and the relation < is well founded. In other words, a linearly ordered set $\langle X , \leq \rangle$ is well ordered if every nonempty subset A of X has a smallest element $a \in A$ , usually denoted by min A. 

It is pretty easy to see that a linearly ordered set $\langle X , \leq \rangle$ is well ordered if and only if it does not contain an infinite strictly decreasing sequence, that is, a sequence $\langle x _ { n } \ \in \ X \colon n \ \in \ \mathbb { N } \rangle$ such that $x _ { n + 1 } ~ < ~ x _ { n }$ for every $n \in \mathbb N$ . However, a formal proof of this fact requires a recursive definition technique, which is still not available to us. Thus its proof will be postponed until Section 4.3 (see Theorem 4.3.2). 

Notice also that a subset of a well-ordered set is well ordered. 

Examples 1. Every finite linearly ordered set is well ordered. 

2. The set N of all natural numbers is well ordered by the usual order $\leq .$ 3. The set $S = \{ 1 - 1 / n \colon n \in \mathbb { N } , \ n > 0 \} \cup \{ 1 \}$ is a well-ordered subset of $\langle \mathbb { R } , \leq \rangle$ since $S _ { 0 } = \{ 1 - 1 / n \colon n \in \mathbb { N } , \ n > 0 \}$ is ordered the same way as N and 1 is greater than any number from $S _ { 0 }$ 

4. The interval [0, 1] with the usual order is linearly ordered and has the smallest element. However, it is not well ordered, since its subset (0, 1) does not have a smallest element (0 is not an element of (0, 1)). 

5. Any family of sets linearly ordered by the relation 

$$
x \varepsilon y \Leftrightarrow x \in y \lor x = y
$$

is well ordered by $\varepsilon .$ . This follows from the axiom of foundation. 

The partially ordered sets $\langle X , \leq \rangle$ and $\langle Y , \preceq \rangle$ are (order) isomorphic (or have the same order type) if there is a bijection $f \colon X \to Y$ such that 

$$
a \leq b \text { if   and   only   if } f (a) \preceq f (b)
$$

for every $a , b \in X$ . The function $f$ is called an order isomorphism (or just isomorphism) between X and Y. 

The next two propositions list some basic properties of order isomorphisms. Their proofs are left as exercises. 

Proposition 4.1.3 Let $\langle X , \leq \rangle , \langle Y , \preceq \rangle$ , and $\langle Z , \ll \rangle$ be partially ordered sets. 

(1) If $f \colon X \to Y$ is an order isomorphism between X and Y then the inverse function $f ^ { - 1 } \colon Y \to X$ is an order isomorphism between $Y$ and X. 

(2) $I f f \colon X \to Y$ is an order isomorphism between X and Y and $g \colon Y \to$ Z is an order isomorphism between Y and Z then $g \circ f \colon X \to Z$ is an order isomorphism between X and Z. 

Proposition 4.1.4 Let $f \colon X \to Y$ be an order isomorphism between partially ordered sets $\langle X , \leq \rangle$ and $\langle Y , \preceq \rangle$ . Then 

(1) X is linearly ordered (well ordered) if and only if Y is linearly ordered (well ordered); 

(2) $x \in X$ is the smallest (the greatest, a minimal, a maximal) element of X if and only if f(x) is the smallest (the greatest, a minimal, a maximal) element of Y. 

Examples 1. The intervals [0, 1] and (0, 1) are not order isomorphic since [0, 1] has a smallest element and (0, 1) does not have one. The set $\langle { \mathcal { P } } ( \mathbb { R } ) , \subset \rangle$ is isomorphic to neither of these sets, since it is not linearly ordered. 

2. The sets N of natural numbers and P of even natural numbers have the same order type. The isomorphism is established by the function $f ( n ) =$ $2 n$ . The order type of this set is denoted by $\omega$ and represents an infinite strictly increasing sequence. (In Section 4.2 we will make the notion of “order type” of well-ordered sets more formal.) 

3. The order type of the set $S = \{ 1 - 1 / n \colon n \in \mathbb { N } , \ n > 0 \} \cup \{ 1 \}$ is denoted by $\omega + 1$ and it is not the same as $\omega _ { i }$ , since S has a greatest element and N does not. 

4. The set $\{ - n \colon n \in \mathbb { N } \}$ ordered by $\leq$ is isomorphic to $\langle \mathbb { N } , ( \leq ) ^ { - 1 } \rangle = \langle \mathbb { N } , \geq \rangle$ by the isomorphism $f ( n ) = - n$ . The order type of this set is denoted by $\omega ^ { \star }$ . The sets with order type $\omega ^ { \star }$ are infinite strictly decreasing sequences. 

A subset $S$ of a partially ordered set $\langle X , \leq \rangle$ is an initial segment of $X$ if for every x, $y \in X$ 

$$
x \leq y \& y \in S \Rightarrow x \in S.
$$

An initial segment S of X is proper if $S \ne X$ . It is easy to see that if $f \colon X \to Y$ is an order isomorphism between $\langle X , \leq \rangle$ and $\langle Y , \preceq \rangle$ then $S \subset X$ is a (proper) initial segment of X if and only if $f [ S ]$ is a (proper) initial segment of Y. 

Note that for every element $x _ { 0 }$ of a partially ordered set $\langle X , \leq \rangle$ the set 

$$
O (x _ {0}) = \{x \in X: x <   x _ {0} \}
$$

is a proper initial segment of X. However, not every proper initial segment of a partially (even linearly) ordered set is of the form $O ( x _ { 0 } )$ , as is shown by the subset $( - \infty , 0 ] = \{ x \in \mathbb { R } \colon x \leq 0 \}$ of R. On the other hand, such an example cannot be found in a well-ordered set, as is asserted by the next theorem. 

Theorem 4.1.5 Every proper initial segment S of a well-ordered set W is of the form $O ( \xi )$ for some $\xi \in W$ 

Proof Since S is a proper subset of W the set $W \backslash S$ is nonempty. Let $\xi = \operatorname* { m i n } \left( W \setminus S \right)$ . Then $S = O ( \xi )$  

Theorem 4.1.6 (Principle of transfinite induction) If a set A is wellordered, $B \subset A$ , and for every $x \in A$ the set B satisfies the condition 

$$
O (x) \subset B \Rightarrow x \in B,\tag{4.1}
$$

then $B = A$ 

Proof It is enough to show that $A \setminus B = \emptyset$ . To arrive at a contradiction assume that $A \setminus B \neq \emptyset$ and let x = min $( A \backslash B )$ . Then, by minimality of x, $O ( x ) \subset B$ . Hence, by (4.1), $x \in B$ . This contradicts $x \in A \setminus B$  

If we apply Theorem 4.1.6 to A = N then we obtain the following version of the induction schema for the set of natural numbers. 

Corollary 4.1.7 If $B \subset \mathbb { N }$ and for every $n \in \mathbb N$ the set B satisfies the condition 

$$
n \subset B \Rightarrow n \in B,\tag{4.2}
$$

then $B = \mathbb { N }$ 

The statement of Corollary 4.1.7 also follows immediately from the induction property (3.2). The converse implication is also easy to prove and can be concluded directly, without the use of Theorem 4.1.6. 

Proofs using Theorem 4.1.6 are called proofs by transfinite induction. Such proofs are the basic techniques of set theory and will be used as a main tool in this course. The proof of the next theorem is a classic example of the use of this technique. To formulate it we need the following definition. 

Let $\langle A , \leq \rangle$ and $\langle B , \leq \rangle$ be partially ordered sets. A function $f \colon A \to B$ is an increasing function if $x \leq y$ implies $f \left( x \right) \leq f \left( y \right)$ for every $x , y \in A$ ; f is strictly increasing if $x \textless y$ implies $f \left( x \right) < f \left( y \right)$ . Similarly we define decreasing and strictly decreasing functions. 

Notice that if $f \colon A  B$ is strictly increasing then it establishes an order isomorphism between A and $f [ A ]$ 

Theorem 4.1.8 If $f \colon A \to A$ is a strictly increasing function defined on a well-ordered set A then $x \leq f ( x )$ for all $x \in A$ 

Proof Let $B = \{ x \in A \colon x \leq f ( x ) \}$ . We will show that $B = A$ . Let $x \in A$ be such that $O ( x ) \subset B$ . By Theorem 4.1.6 it is enough to show that $x \in B$ So take $y \in O ( x )$ . Then $y \le f ( y )$ . Moreover, $f ( y ) < f ( x )$ , since $y < x$ Hence $y < f ( x )$ for every $y \in O ( x )$ . In particular, $f ( x ) \in A \setminus O ( x )$ . Since x is the first element of $A \setminus O ( x )$ we conclude that $x \leq f ( x )$ . Thus $x \in B$  

Corollary 4.1.9 If well-ordered sets A and B are isomorphic, then the isomorphism $f \colon A \to B$ is unique. 

Proof Let $g \colon A  B$ be another order isomorphism. We will show that $f = g$ . So let $x \in A$ . The function $g ^ { - 1 } \circ f \colon A \to A$ is also an isomorphism. Using Theorem 4.1.8 applied to $g ^ { - 1 } \circ$ f we conclude that $x \leq g ^ { - 1 } ( f ( x ) )$ and, applying function g to both sides, $g ( x ) \leq f ( x )$ . Similarly we argue for $f ( x ) \leq g ( x )$ . Thus $f ( x ) = g ( x )$ . Since x was arbitrary, $f = g$  

Corollary 4.1.10 No well-ordered set is isomorphic to any of its proper initial segments. 

Proof If a well-ordered set A were isomorphic to an initial segment $O ( x )$ for $x \in A$ , and $f \colon A \to O ( x )$ were an isomorphism establishing this fact, then we would have $f ( x ) \in O ( x )$ , that is, $f ( x ) < x$ , contradicting Theorem 4.1.8.  

Corollary 4.1.11 No two distinct initial segments of a well-ordered set are isomorphic. 

Theorem 4.1.12 If A and B are well-ordered sets then either 

(i) A and B are isomorphic, 

(ii) A is isomorphic to a proper initial segment of B, or 

(iii) B is isomorphic to a proper initial segment of A. 

Proof Let 

$Z = \{ x \in A \colon \exists y _ { x } \in B ( O ( x )$ and $O ( y _ { x } )$ are order isomorphic)}. 

Notice that if $x \in Z$ then, by Corollary 4.1.11, $y _ { x }$ from the definition of the set $Z$ is unique. Define $f \colon Z \to B$ by putting $f ( x ) = y _ { x }$ , that is, 

$f = \{ \langle x , y \rangle \in A \times B \colon O ( x )$ and $O ( y )$ are order isomorphic}. 

First we will show that $Z$ is an initial segment of $A .$ . To see it, let $x < z$ and $z \in Z$ . We have to show that $x \in Z$ . Since $z \in Z$ , there is an isomorphism $h$ between $O ( z )$ and $O ( f ( z ) )$ . The restriction of $h$ to $O ( x )$ gives an isomorphism, whose range must be a proper initial segment $S$ of $O ( f ( z ) )$ , and, by Theorem $4 . 1 . 5 , \ S = O ( y )$ for some $y \in O ( f ( z ) )$ . Thus $x \in Z$ and we conclude that $Z$ is an initial segment of $A$ 

This argument shows also that f is strictly increasing, since $x < z$ and $z \in Z$ imply that $O ( x )$ is isomorphic to $O ( y )$ for some $y \in O ( f ( z ) )$ , that is, $f ( x ) = y < f ( z )$ 

Similarly as for $Z$ we can also prove that $f [ Z ]$ is an initial segment of $B$ . (Just note that $f [ Z ] = \{ y \in B \colon \exists x \in A ( O ( y )$ and $O ( x )$ are isomorphic)}.) So $f \colon Z \to f [ Z ]$ is an order isomorphism. 

If $Z = A$ then f establishes an isomorphism between $A$ and either $B$ or a proper initial segment of B. Similarly, if $f [ Z ] = B$ then $f ^ { - 1 }$ shows that $B$ is isomorphic to either A or a proper initial segment of A. Thus, it is enough to prove that either $Z = A$ or $f [ Z ] = B$ 

To obtain a contradiction assume that $Z \neq A$ and $f [ Z ] \neq B$ . Then $Z$ is a proper initial segment of A and $f [ Z ]$ is a proper initial segment of $B .$ Hence, by Theorem 4.1.5, $Z = O ( x )$ for some $x \in A$ and $f [ Z ] = O ( y )$ for some $y \in B$ . But then, $f$ is an isomorphism between $Z = O ( x )$ and $O ( y )$ , contradicting the fact that $x \not \in Z$ 

We will finish this section with the following construction of an ordering relation on a product space. 

Theorem 4.1.13 Let $\{ F _ { t } \} _ { t \in T }$ be an indexed family of nonempty linearly ordered sets $\langle F _ { t } , \leq _ { t } \rangle$ and let T be well ordered by $\leq . \ I f \preceq i s$ a binary relation on the Cartesian product $\textstyle P = \prod _ { t \in T } F _ { t }$ defined by the formula 

$$
f \preceq g \Leftrightarrow f = g \vee \exists s (s = \min \{t \in T: f (t) \neq g (t) \} \& f (s) \leq_ {s} g (s))
$$

for every $f , g \in P _ { ; }$ , then $\preceq \ * i s$ a linear order on $P$ . 

Moreover, if T is finite then P is well ordered $b y \preceq i f$ and only if all sets $F _ { t }$ are well ordered. 

The proof is left as an exercise. 

The relation $\preceq$ defined in Theorem 4.1.13 is called the lexicographic order of $\prod _ { t \in T } F _ { t }$ and is sometimes denoted by $\leq _ { \mathrm { l e x } }$ 

## EXERCISES

1 Prove Proposition 4.1.3. 

2 Prove Proposition 4.1.4. 

3 Let $f \colon X \to Y$ be an isomorphism between partially ordered sets $\langle X , \leq \rangle$ and $\langle Y , \preceq \rangle$ . Show that $S \subset X$ is a (proper) initial segment of X if and only if f[S] is a (proper) initial segment of Y. 

4 Complete the proof of Theorem 4.1.5 by showing that $S = O ( \xi )$ 

5 Prove Theorem 4.1.13. 

6 Show that in the additional part of Theorem 4.1.13 the assumption that $T$ is finite is essential by giving an example of well-ordered sets $T$ and $F$ for which the lexicographic order on $F ^ { T }$ is not a well-ordering relation. 

7 Let $\langle K , \leq \rangle$ and $\langle X , \leq \rangle$ be nonempty linearly ordered sets such that X has a fixed element $0 \in X$ . For $f \colon K \to X$ let $\operatorname { s u p p } ( f ) = \{ k \in K \colon f ( k ) \neq 0 \}$ and put 

$$
\mathcal {F} (K, X) = \{f \in X ^ {K} \colon \operatorname{supp} (f) \text {   is   finite } \}.
$$

Define a binary relation % on ${ \mathcal { F } } ( K , X )$ by putting 

$$
f \preceq g \Leftrightarrow f = g \text { or } f (m) \leq g (m), \text { where } m = \max \{k \in K: f (k) \neq g (k) \},
$$

for every $f , g \in { \mathcal { F } } ( K , X )$ . Prove that 

(a) the relation $\preceq$ is a linear-order relation on ${ \mathcal { F } } ( K , X )$ ; 

(b) if X has at least two elements and 0 is the minimal element of X then $\langle { \mathcal { F } } ( K , X ) , { \preceq } \rangle$ is well ordered if and only if $\langle X , \leq \rangle$ and $\langle K , \leq \rangle$ are well ordered. 

The relation $\preceq$ is usually called an antilexicographic-order relation. 

## 4.2 Ordinal numbers

In the previous section we were informally talking about the “order type” of a given partially ordered set $\langle X , \leq \rangle$ . The natural way of thinking about such an object is to consider it as a representative from the equivalence class $[ X ] _ { \leq }$ of all ordered sets order isomorphic to $\langle X , \leq \rangle$ . This equivalence class, however, is not a set! (The argument is similar to that for the class of all sets.) Moreover, if we want to talk about all order types, we find also that there are too many of them; that is, even if we discover a good way of choosing a representative from each equivalence class $[ X ] _ { \leq }$ , the class of all such representatives will not be a set. 

One way to avoid this problem is to consider the sentences $^ { 6 6 } \langle Y , \leq \rangle$ has the order type $\tau$ of $\langle X , \leq \rangle ^ { \mathfrak { s } }$ and $^ { 6 6 } \langle Y , \leq \rangle$ and $\langle X , \leq \rangle$ have the same order $\mathrm { t y p e } ^ { , , , }$ just as abbreviations for the well-defined sentence $^ { 6 6 } \langle Y , \leq \rangle$ and $\langle X , \leq \rangle$ are order isomorphic.” That is the way we will think about the order types of arbitrary partially ordered sets. For the well-ordered sets, however, we can indeed follow the path of our intuition described in the previous paragraph. This section is dedicated to fulfilling this goal by constructing the canonical order types of well-ordered sets, called ordinal numbers. The construction is due to von Neumann (1929). 

The class of all ordinal numbers is still too big to be a set. Thus, instead of constructing it as a set, we will define a formula $\varphi ( \alpha )$ that will represent an intuitive sentence $^ { 6 6 } \alpha$ is an ordinal number.” The definition is as follows. 

A set α is said to be an ordinal number (or just an ordinal) if it has the following properties: 

(A<sub>α</sub>) If β ∈ α then β ⊂ α; 

$$
\left(\mathrm{B} _ {\alpha}\right) \quad \text {   If   } \beta , \gamma \in \alpha \text {   then   } \beta = \gamma , \beta \in \gamma , \text {   or   } \gamma \in \beta ;
$$

(C<sub>α</sub>) If $\emptyset \neq B \subset \alpha$ then there exists a $\gamma \in B$ such that $\gamma \cap B = \emptyset$ 

It follows from Theorem 3.1.2 that if α stands for either any natural number or the set N of natural numbers then α satisfies conditions $\left( \operatorname { A } _ { \alpha } \right)$ and $\left( \operatorname { B } _ { \alpha } \right)$ . Also, the well-ordering principle for the natural numbers implies condition $\left( \operatorname { C } _ { \alpha } \right)$ in this case. So every natural number is an ordinal number and so is N. It is also easy to see that the set $\mathbb { N } \cup \left\{ \mathbb { N } \right\}$ is an ordinal number. The sets N and $\mathbb { N } \cup \{ \mathbb { N } \}$ , when considered as ordinal numbers, are traditionally denoted as ω and $\omega + 1$ , respectively. 

We will start with the following basic property. 

Theorem 4.2.1 If α is an ordinal number and $\eta \in \alpha$ then η is also an ordinal number. 

Proof Assume that α satisfies $\left( \operatorname { A } _ { \alpha } \right) - \left( \operatorname { C } _ { \alpha } \right)$ and let $\eta \in \alpha$ . We have to show that η satisfies $\bigl ( \mathrm { A } _ { \eta } \bigr ) - \bigl ( \mathrm { C } _ { \eta } \bigr )$ 

First notice that $\left( \operatorname { A } _ { \alpha } \right)$ implies $\eta \subset \alpha$ . To see $\left( \mathrm { C } _ { \eta } \right)$ let $\emptyset \neq B \subset \eta$ . Then $\varnothing \neq B \subset$ α and $\left( \mathrm { C } _ { \eta } \right)$ follows from $\left( \operatorname { C } _ { \alpha } \right)$ . To see $\left( \operatorname { B } _ { \eta } \right)$ take $\beta , \gamma \in \eta$ . Then $\beta , \gamma \in \alpha$ and $\left( \operatorname { B } _ { \eta } \right)$ follows from $\left( \operatorname { B } _ { \alpha } \right)$ 

Finally, to see $( \mathrm { A } _ { \eta } )$ let $\beta \in \eta$ . We have to show that $\beta \subset \eta$ . So choose $\xi \in \beta$ . The proof will be finished when we show that $\xi \in \eta$ . But $\beta \in \eta \subset \alpha$ So, by $( \mathrm { A } _ { \alpha } ) , \beta \subset$ α and $\xi \in \alpha$ , since $\xi \in \beta$ . We have proved that $\xi , \eta \in \alpha$ Now, using $\left( \operatorname { B } _ { \alpha } \right)$ , we conclude that $\xi \in \eta , \xi = \eta$ , or $\eta \in \xi . \ \mathrm { H } \xi \in \eta$ then we are done. We will prove that the other two cases are impossible. 

To obtain a contradiction, assume first that $\eta \in \xi$ . Then, in particular, $\eta \in \xi \in \beta \in \eta$ . Put $B = \{ \xi , \beta , \eta \}$ . Then $\emptyset \neq B \subset \alpha$ . But then $\left( \operatorname { C } _ { \alpha } \right)$ fails for this $B$ , since $\eta \in \xi \cap B , \xi \in \beta \cap B$ , and $\beta \in \eta \cap B$ , that is, the sets $\xi \cap B$ $\beta \cap B$ , and η ∩ B are nonempty. 

So assume $\xi = \eta$ . Then $\eta = \xi \in \beta \in \eta$ . Choosing $B = \{ \beta , \eta \}$ gives a contradiction similar to that in the previous case.  

Now notice that for an ordinal number α and for arbitrary $\beta , \gamma \in \alpha$ 

$$
\gamma \subset \beta \text { if   and   only   if } \gamma = \beta \vee \gamma \in \beta .\tag{4.3}
$$

The implication $\Lt = \mathrm { f o l l o w s }$ immediately from $\left( \operatorname { A } _ { \beta } \right)$ , which holds by Theorem 4.2.1. To see the other implication let $\gamma \subset \beta$ . Since $\beta , \gamma \in \alpha .$ condition $\left( \operatorname { B } _ { \alpha } \right)$ implies that $\gamma = \beta , \gamma \in \beta$ , or $\beta \in \gamma$ . If either of the first two conditions holds, we are done. But if $\beta \in \gamma$ then, by $( \mathrm { A } _ { \gamma } ) , \beta \subset \gamma .$ , and combining this with $\gamma \subset \beta$ we obtain $\gamma = \beta$ 

Theorem 4.2.2 If α is an ordinal number then the relation $\subset$ is a wellordering relation on α. 

Proof Inclusion $\subset$ is clearly a partial-order relation on any family of sets, so it is on α. It is a linear order on α by $\left( \operatorname { B } _ { \alpha } \right)$ and (4.3). 

To see that $\alpha$ is well ordered by ⊂, let $\emptyset \neq B \subset \alpha$ and let $\gamma \in B$ be as in $\left( \operatorname { C } _ { \alpha } \right)$ , that is, such that $\gamma \cap B = \emptyset$ . We will show that $\gamma$ is minimal with respect to $\subset \cdot$ So choose arbitrary $\beta \in B$ . Then, by $\left( \operatorname { B } _ { \alpha } \right)$ and (4.3), either $\gamma \subset \beta$ or $\beta \in \gamma$ . But $\beta \in \gamma$ implies $\gamma \cap B \neq \emptyset$ , which is impossible. Thus $\gamma \subset \beta$ . Since $\beta$ was an arbitrary element of B we conclude that $\gamma$ is a minimal element in $B$  

It is customary that the relation $\subset \ \mathrm { o n }$ an ordinal number is denoted by $\leq$ . It is also easy to see that, according to our general agreement, the relation $<$ on an ordinal number is identical to $\in$ 

Notice also that by Theorem 4.1.5 every proper initial segment of an ordinal number α is of the form $O ( \beta )$ for some $\beta \in \alpha$ and that $O ( \beta ) = \beta$ Thus every initial segment of an ordinal number is an ordinal number. 

The basic properties of ordinal numbers are as follows. 

Theorem 4.2.3 For every ordinal numbers α and $\beta$ 

(i) if α and $\beta$ are order isomorphic then $\alpha = \beta _ { i }$ 

(ii) $\alpha = \beta , \ : \alpha < \beta , \ : o r \ : \beta < \alpha ;$ 

(iii) $i f ~ \mathcal { F }$ is a nonempty family of ordinal numbers then $\cup \mathcal { F }$ is also an ordinal number. 

Proof (i) Let $f \colon \alpha  \beta$ be an order isomorphism and let 

$$
Z = \{\gamma \in \alpha \colon f (\gamma) = \gamma \}.
$$

We will show, by transfinite induction, that $Z = \alpha ,$ . This will finish the proof, since $Z = \alpha$ implies that $f$ is the identity function on α, and thus $\alpha = f [ \alpha ] = \beta$ 

To see that $Z = \alpha$ let $\gamma \in \alpha$ be such that $O ( \gamma ) \subset Z$ . Then $f [ O ( \gamma ) ] =$ $O ( f ( \gamma ) )$ and $f ( \delta ) = \delta$ for all $\delta < \gamma$ . Hence 

$$
f (\gamma) = O (f (\gamma)) = f [ O (\gamma) ] = \{f (\delta): \delta <   \gamma \} = \{\delta : \delta <   \gamma \} = \gamma .
$$

Thus we have proved that for every $\gamma \in \alpha$ condition $O ( \gamma ) \subset Z$ implies that $\gamma \in Z$ . Hence $Z = \alpha$ . Condition (i) has been proved. 

(ii) By Theorem 4.1.12 either α and $\beta$ are isomorphic, or $\alpha$ is isomorphic to a proper initial segment of $\beta ,$ or $\beta$ is isomorphic to a proper initial segment of α. By (i), this implies (ii). 

(iii) We have to check that $\delta = \cup \mathcal { F }$ satisfies $\left( \operatorname { A } _ { \delta } \right) - \left( \operatorname { C } _ { \delta } \right)$ 

$\left( \operatorname { A } _ { \delta } \right)$ : If $\beta \in \cup \mathcal { F }$ then there is an α $\in ~ \mathcal { F }$ such that $\beta \in \alpha$ . Then $\beta \subset \alpha \subset \bigcup { \mathcal { F } }$ 

$\left( \operatorname { B } _ { \delta } \right)$ : If $\beta , \gamma \in \cup { \mathcal { F } }$ then there are $\alpha _ { 1 } , \alpha _ { 2 } \in { \mathcal { F } }$ such that $\beta \in \alpha _ { 1 }$ and $\gamma \in \alpha _ { 2 }$ . By (ii) either $\alpha _ { 1 } \leq \alpha _ { 2 }$ or $\alpha _ { 2 } \leq \alpha _ { 1 }$ . Let α be the greater of these two. Then $\beta , \gamma \in \alpha$ and, $\begin{array} { r } { \mathrm { b y } \ ( \mathrm { B } _ { \alpha } ) , \beta = \gamma , \beta \in \gamma , \mathrm { o r } \gamma \in \beta . } \end{array}$ 

$\left( \mathrm { C } _ { \delta } \right)$ : Let $\emptyset \neq B \subset \bigcup { \mathcal { F } }$ and let $\alpha \in B$ . Then there is an $\eta \in { \mathcal { F } }$ such that $\alpha \in \eta$ . Hence, by Theorem 4.2.1, α is an ordinal. If $\alpha \cap B = \varnothing$ put $\gamma = \alpha$ . Otherwise, put $\gamma = \operatorname* { m i n } ( \alpha \cap B )$ , which exists by $\left( \operatorname { C } _ { \alpha } \right)$ . It is easy to see that $\gamma \cap B = \emptyset$  

It is not dificult to see that for an ordinal number α the set $\alpha \cup \{ \alpha \}$ is also an ordinal number. We will denote it by $\alpha + 1$ and call it the (ordinal immediate) successor of α. Number α is also called the (ordinal immediate) predecessor of $\alpha { + 1 }$ . It is also easy to check that $\alpha { + 1 }$ is the smallest ordinal number greater than α. Thus every ordinal number has its successor. Not every number, however, has an immediate predecessor; for example, 0 and $\omega$ do not have one. The ordinal numbers that have immediate predecessors $( { \mathrm { i . e . } }$ , those in the form $\alpha + 1 )$ are called ordinal successors. Those that do not have immediate predecessors are called limit ordinals. 

The next theorem justifies our intuition of considering ordinal numbers as representatives of the abstract classes of all order-isomorphic wellordered sets. 

Theorem 4.2.4 For every well-ordered set $\langle W , \leq \rangle$ there exists precisely one ordinal number α that is order isomorphic to W. 

Proof The uniqueness of α follows immediately from Theorem 4.2.3(i). 

For $w \in W$ let $O [ w ] = O ( w ) \cup \{ w \}$ and define 

$Z = \{ w \in W \colon O [ w ]$ is order isomorphic to some ordinal number $\alpha _ { w } \}$ 

Notice that by Theorem 4.2.3(i) and Corollary 4.1.9 the ordinal number $\alpha _ { w }$ and the isomorphism $f _ { w } \colon O [ w ] \to \alpha _ { w }$ are unique. 

Now, if $v , w \in Z$ and $v \leq w$ then $f _ { w } [ O [ v ] ]$ is an ordinal number α, as an initial segment of $\alpha _ { w }$ . In particular, $f _ { w } | _ { { \cal { O } } [ v ] } \colon { \cal { O } } [ v ]  \alpha$ is an order isomorphism and, by the preceding uniqueness remark, $f _ { w } | _ { O [ v ] } = f _ { v }$ . So we have shown that 

$$
f _ {v} \subset f _ {w} \text { for   every } v, w \in Z, v \leq w.\tag{4.4}
$$

We will prove, by transfinite induction, that $Z = W$ 

So let $O ( w ) \subset Z$ . Then, by (4.4), $\textstyle f = \bigcup _ { v \in O ( w ) }$ f is a strictly increasing function from $\textstyle \bigcup _ { v \in O ( w ) } O [ v ]$ onto $\textstyle \bigcup _ { v \in O ( w ) } \alpha _ { v }$ . But $\begin{array} { r } { \bigcup _ { v \in O ( w ) } O [ v ] = O ( w ) } \end{array}$ and, by Theorem 4.2.3(iii), $\begin{array} { r } { \alpha = \bigcup _ { v \in O ( w ) } \alpha _ { v } } \end{array}$ is an ordinal number. So $f \colon O ( w ) \to \alpha$ is an order isomorphism. Extend f to a function $F \colon O [ w ] \to$ $\alpha + 1$ by putting $F ( w ) = \alpha$ . Then the existence of F proves that $w \in Z$ We have shown that $Z = W$ 

Now, by (4.4), the function $f = \textstyle \bigcup _ { w \in W } f _ { w }$ is an isomorphism between $\begin{array} { r } { W = \bigcup _ { w \in W } O [ w ] } \end{array}$ and an ordinal number $\textstyle \bigcup _ { w \in W } \alpha _ { w }$  

In what follows it will be convenient to use the following theorems. 

Theorem 4.2.5 If α and $\beta$ are ordinal numbers and $f \colon \alpha  \beta$ is a strictly increasing function then $\alpha \leq \beta$ . Moreover, $\xi \leq f ( \xi )$ for every $\xi < \alpha$ 

Proof If $\beta < \alpha$ then $\beta \subset \alpha$ and f is a strictly increasing function from α into α. But then $f ( \beta ) \in \beta$ , that is, $f ( \beta ) < \beta$ , contradicting Theorem 4.1.8. So, by Theorem $4 . 2 . 3 ( \mathrm { i i } ) , \alpha \leq \beta$ 

The additional part follows from Theorem 4.1.8. 

For a well-ordered set W let $\operatorname { O t p } ( W )$ stand for the order type of W, that is, the unique ordinal number that is order isomorphic to $W$ 

Corollary 4.2.6 IfW is well ordered and $B \subset W$ then $\operatorname { O t p } ( B ) \leq \operatorname { O t p } ( W )$ 

Proof Let $f \colon \mathrm { O t p } ( B ) \to B$ and $g \colon W \to \operatorname { O t p } ( W )$ be order isomorphisms. Then $g \circ f \colon { \mathrm { O t p } } ( B ) \to { \mathrm { O t p } } ( W )$ is strictly increasing, and by Theorem 4.2.5 $\operatorname { O t p } ( B ) \leq \operatorname { O t p } ( W )$  

We will also introduce the following arithmetic for ordinal numbers. For ordinal numbers α and $\beta$ we define the sum $\alpha + \beta$ of α and $\beta$ as the order type of the well-ordered set $( \{ 0 \} \times \alpha ) \cup ( \{ 1 \} \times \beta )$ ordered by 

$$
\langle i, \xi \rangle \leq \langle j, \zeta \rangle \Leftrightarrow i <   j \vee (i = j \& \xi \leq \zeta).
$$

Thus, we “append” $\beta$ to α. It is easy to see that the relation so defined is indeed a well-ordering relation. 

Similarly, we define the product $\alpha \beta$ of ordinal numbers α and $\beta$ as the order type of the set $\beta \times \alpha$ ordered lexicographically. By Theorem 4.1.13 it is well ordered. 

It is not dificult to see that, in general, $\alpha + \beta \neq \beta + \alpha$ and $\alpha \beta \neq \beta \alpha$ (see Exercise 1). We have the following monotonic laws for these operations. 

Theorem 4.2.7 For arbitrary ordinal numbers $\alpha , \beta , \gamma$ 

(a) $\alpha < \beta$ implies $\gamma + \alpha < \gamma + \beta ,$ 

(b) $\alpha \leq \beta$ implies $\alpha + \gamma \leq \beta + \gamma ;$ 

(c) $\alpha < \beta$ and $\gamma > 0$ imply $\gamma \alpha < \gamma \beta$ ; 

(d) $\alpha \leq \beta$ implies $\alpha \gamma \le \beta \gamma$ 

Moreover, the inequalities $\leq i n \ ( b )$ and $( d )$ cannot be replaced by < even $i f \alpha < \beta$ 

Proof To see (a) let $f \colon ( \{ 0 \} \times \gamma ) \cup ( \{ 1 \} \times \alpha )  ( \{ 0 \} \times \gamma ) \cup ( \{ 1 \} \times \beta )$ be the identity map. Notice that f is an isomorphism between $( \{ 0 \} \times \gamma ) \cup ( \{ 1 \} \times \alpha )$ and the initial segment $O ( \langle 1 , \alpha \rangle )$ of $( \{ 0 \} \times \gamma ) \cup ( \{ 1 \} \times \beta )$ . Thus $\gamma + \alpha$ is isomorphic to a proper initial segment of $\gamma + \beta , \mathrm { s o } \gamma + \alpha < \gamma + \beta .$ 

To see (b) let $f \colon ( \{ 0 \} \times \alpha ) \cup ( \{ 1 \} \times \gamma )  ( \{ 0 \} \times \beta ) \cup ( \{ 1 \} \times \gamma )$ be the identity map. Notice that f is strictly increasing. Thus, via an appropriate isomorphism, f can be transformed into a strictly increasing function from $\alpha + \gamma$ into $\beta + \gamma$ . But then, by Theorem $4 . 2 . 5 , \alpha + \gamma \leq \beta + \gamma$ 

To see that equality can hold even if $\alpha < \beta$ , notice that $1 + \omega = \omega = 0 + \omega$ (see Exercise 1). 

Parts (c) and (d) are left as exercises. 

For an ordinal number α any function a on α is called a transfinite sequence and is usually denoted by $\{ a _ { \xi } \} _ { \xi < \alpha } ~ \mathrm { o r } ~ \langle a _ { \xi } : \xi < \alpha \rangle$ , where $a _ { \xi } =$ $a ( \xi )$ . If $\alpha$ is a domain of a transfinite sequence a then we also often say that a is an α-sequence. 

## EXERCISES

1 Show that for ordinal numbers α and $\beta$ we might have $\alpha + \beta \neq \beta + \alpha$ and $\alpha \beta \neq \beta \alpha$ by proving that 

(a) 1 + ω = ω, so 1 + ω = ω + 1; 

(b) 2ω = ω, ω2 = ω + ω, and ω = ω + ω. 

2 Prove parts (c) and (d) of Theorem 4.2.7. 

## 4.3 Definitions by transfinite induction

Most mathematicians take for granted that if we have a procedure associating a number $a _ { n + 1 }$ to a number $a _ { n }$ and we have defined $a _ { 0 }$ , then the sequence $\{ a _ { n } \} _ { n \in \mathbb { N } }$ constructed in such a way exists. The proof of this fact for a finite portion $\{ a _ { n } \} _ { n \leq m } , m \in \mathbb { N }$ , of such a sequence does not require any special axioms. The proof of existence of the infinite sequence $\{ a _ { n } \} _ { n \in \mathbb { N } }$ however, requires some form of argument, and the axiom of choice is needed to prove any procedure justifying such an argument. (For example, if we stay only within the framework of Peano arithmetic, we have no way to prove the existence of an infinite object $\{ a _ { n } \} _ { n \in \mathbb { N } }$ , since we operate in a world with finite objects only.) This argument is given in the next theorem. 

Theorem 4.3.1 (Recursion theorem) Let $Z$ be a set, α be an ordinal number, and $\mathcal { F }$ be the family of all ξ-sequences $f o r \xi < \alpha$ with values in $Z _ { i }$ , that is, $\textstyle { \mathcal { F } } = \bigcup _ { \xi < \alpha } Z ^ { \xi }$ . Then for each function h: $\mathcal { F }  Z$ there exists precisely one function $f \colon \alpha  Z$ such that 

$$
f (\xi) = h (f | _ {\xi}) \text {   for   all   } \xi <   \alpha .\tag{4.5}
$$

The function h from the theorem tells us how to choose $f ( \xi )$ knowing the values of the sequence $\langle f ( \zeta ) : \zeta < \xi \rangle$ chosen so far. Because of this, we will sometimes call it an “oracle” function. 

Proof of Theorem 4.3.1 First we prove the uniqueness of f. So let $g$ be another function satisfying (4.5) and let $W = \{ \xi < \alpha \colon f ( \xi ) = g ( \xi ) \}$ It is enough to show that $W = \alpha$ . But if $\xi = O ( \xi ) \subset W$ then $f | _ { \xi } = g | _ { \xi }$ and $f ( \xi ) = h ( f | _ { \xi } ) = h ( g | _ { \xi } ) = g ( \xi )$ . Hence $\xi \in W$ , and by a transfinite induction argument $W = \alpha .$ . The uniqueness of f has been proved. 

To prove the main body of the theorem assume, to obtain a contradiction, that the theorem fails for some ordinal number $\alpha .$ . We may assume that α is the smallest ordinal number for which the theorem fails, since if it is not, we can replace it by the minimum 

$$
\min \{\beta <   \alpha \colon \text { theorem   fails   for } \beta \}.
$$

Let h be a function for which the theorem fails for ordinal α. For every $\xi < \alpha$ there is a function $f _ { \xi } \colon \xi \to Z$ such that 

$$
f _ {\xi} (\gamma) = h (f _ {\xi} | _ {\gamma}) \text { for   all } \gamma <   \xi .\tag{4.6}
$$

But for any $\xi \le \zeta < \alpha$ the function $f _ { \zeta } | _ { \xi }$ also satisfies (4.6). Thus, by the uniqueness part that we have already proved, $f _ { \zeta } | _ { \xi } = f _ { \xi }$ . In particular, 

$$
f _ {\xi} (\gamma) = f _ {\zeta} (\gamma) \mathrm{forevery} \gamma <   \xi \leq \zeta <   \alpha .
$$

Now, if α is a successor ordinal, say $\alpha = \beta + 1$ , then define $f \colon \alpha  Z$ as an extension of $f _ { \beta }$ by putting $f ( \beta ) = h ( f _ { \beta } )$ . Then f satisfies (4.5) since $f | _ { \xi } = f _ { \beta } | _ { \xi }$ for every $\xi < \alpha$ . This contradicts the choice of $\alpha .$ 

Thus assume that α is a limit ordinal. Then $\xi + 1 < \alpha$ for every $\xi < \alpha$ Define $f \colon \alpha  Z$ by 

$$
f (\xi) = f _ {\xi + 1} (\xi) \mathrm{for} \xi <   \alpha
$$

and notice that such a function satisfies (4.5), since 

$$
f (\xi) = f _ {\xi + 1} (\xi) = h (f _ {\xi + 1} | _ {\xi}) = h (f | _ {\xi})
$$

for every $\xi < \alpha$ . This contradicts the choice of α. 

Most commonly, the oracle function h is defined as a choice function $C$ on some family of sets. In such a case a particular value $h ( \xi )$ is chosen as a value of C on some set, whose definition depends on the previously chosen values of f, that is, it is of the form 

$$
h (p) = C (\{z \in Z \colon \varphi (z, p) \}),
$$

where $C \colon { \mathcal { P } } ( Z ) \to Z$ is a choice function and $\varphi ( z , p )$ is some formula. Of course, such a function h is not defined for the values of $p \in { \mathcal { F } }$ for which the set $\{ z \in Z \colon \varphi ( z , p ) \}$ is empty. Formally, to use the recursion theorem we have to define it for these values of p as well; however, in most cases we are not interested in such values anyway. Thus, we usually assume that $h$ is arbitrarily defined somehow for such values and we don’t even bother to mention it. (The same is true for the other values for the oracle function in which we are not interested.) Also, it is customary in such situations to simply write that we choose in the inductive step 

$$
f (\xi) \in \{z \in Z \colon \varphi (z, f | _ {\xi}) \}
$$

or simply 

$$
f (\xi) = z \text { such   that } z \text { satisfies } \varphi (z, f | _ {\xi})
$$

without mentioning explicitly the oracle function at all. 

In the applications using the recursion theorem we often separately specify the value of the function h for the empty sequence by $h ( 0 ) = A$ and for successor ordinals $\xi + 1$ by $h ( \phi ) = F ( \phi ( \xi ) )$ for some function $F \in Z ^ { Z }$ where $\phi \in Z ^ { \xi + 1 }$ . Thus the value of h on successor ordinal $\xi + 1$ depends only on the value $\phi ( \xi )$ of $\phi$ on its last element $\xi .$ . The α-sequence f obtained that way satisfies the conditions 

$$
f (0) = A, \quad f (\xi + 1) = F (f (\xi)) \text { for   any   ordinal } \xi <   \alpha ,
$$

$$
f (\lambda) = h (f | _ {\lambda}) \text {   for   any   limit   ordinal   } \lambda <   \alpha .
$$

Notice that to define the function $f$ only on $\alpha = \omega$ we don’t need the very last condition. Then the first two conditions can be rewritten as 

$$
f (0) = A, \quad f (n + 1) = F (f (n)) \text { for   any } n <   \omega .
$$

The existence of such a sequence is usually deduced from the standard (not transfinite) recursion theorem. 

There is probably no need to explain to the reader the importance of this last theorem. Without this theorem it is sometimes hard to prove even very intuitive theorems. As an example we can state here the following characterization of well orderings. 

Theorem 4.3.2 A linearly ordered set $\langle X , \leq \rangle$ is well ordered if and only $i f \ i t$ does not contain a subset of order type $\omega ^ { \star } ~ ( i . e .$ , a strictly decreasing $\omega \mathrm { - } s e q u e n c e )$ 

Proof $\Rightarrow :$ If there exists a strictly decreasing sequence $\langle x _ { n } \colon n < \omega \rangle$ then the set $\{ x _ { n } : n < \omega \}$ does not have a smallest element. 

$\Leftarrow : \mathrm { ~ A ~ }$ ssume that X is not well ordered and construct, by induction on $n < \omega$ , a strictly decreasing sequence $\langle x _ { n } \colon n < \omega \rangle$ . The details are left as an exercise.  

The next theorem is one of the most fundamental theorems in set theory. 

Theorem 4.3.3 (Well-ordering or Zermelo’s theorem) Every nonempty set X can be well ordered. 

Proof Let C be a choice function on the family ${ \mathcal { P } } ( X ) \setminus \{ \emptyset \}$ . Choose an arbitrary $p \not \in X$ , for example, $p = X$ , and define $F \colon { \mathcal { P } } ( X \cup \{ p \} ) \to X \cup \{ p \}$ by 

$$
F (Z) = \left\{ \begin{array}{l l} C (Z) & \text { for } Z \in \mathcal {P} (X) \setminus \{\emptyset \}, \\ p & \text { otherwise }. \end{array} \right.
$$

Let $\mathcal { G }$ be the family of all ordinal numbers $\xi$ such that there is a oneto-one ξ-sequence in $X$ . Notice that $\mathcal { G }$ is a set by the replacement axiom, since 

$$
\mathcal {G} = \{\operatorname{Otp} (\langle Y, \leq \rangle) \colon Y \in \mathcal {P} (X) \& \leq \in \mathcal {P} (X \times X) \& \langle Y, \leq \rangle \text {is well ordered} \}.
$$

Let α be an ordinal number that does not belong to ${ \mathcal { G } } .$ For example, take $\alpha = ( \bigcup \mathcal { G } ) + 1$ . By the recursion theorem there exists a function $f \colon \alpha  X \cup \{ p \}$ such that 

$$
f (\xi) = F (X \setminus \{f (\zeta): \zeta <   \xi \})\tag{4.7}
$$

for all $\xi < \alpha$ . (The function h is defined by $h ( s ) = F { ( X \backslash \mathrm { r a n g e } ( s ) ) } . )$ Notice that for every $\beta \leq \alpha$ 

$$
\text { if } f [ \beta ] \subset X \text { then } f | _ {\beta} \text { is   one - to - one. }\tag{4.8}
$$

This is the case since, by (4.7), $f ( \xi ) \in X \setminus \{ f ( \zeta ) \colon \zeta < \xi \}$ for $\xi < \beta .$ . In particular, $f [ \alpha ] \not \subset X$ since there is no one-to-one α-sequence in X. So the set $S = \{ \beta \leq \alpha \colon f ( \beta ) = p \}$ is nonempty. Let $\beta = \operatorname* { m i n } S$ . Then $f | _ { \beta }$ is one-to-one and it establishes a well ordering of X of type $\beta$ by 

$$
x \preceq y \Leftrightarrow f ^ {- 1} (x) \leq f ^ {- 1} (y).
$$

Remark It is clear that we used the axiom of choice in the proof of Theorem 4.3.3. It is also easy to prove in $\mathrm { Z F }$ that Theorem 4.3.3 implies the axiom of choice.<sup>1</sup> To argue for this it is enough to show that Theorem 4.3.3 implies the existence of a choice function for every family $\mathcal { F }$ of nonempty sets. But $\mathrm { i f ~ \le ~ }$ is a well ordering of $\cup \mathcal { F }$ then the function $f ( F ) = \operatorname* { m i n } F$ for $F \in { \mathcal { F } }$ is a choice function defined only with help of the comprehension schema. 

The combination of the recursion and well-ordering theorems gives a very strong proving technique. However, for its use usually some kind of cardinal argument is needed, a tool that we still have not developed. Thus, the direct use of this technique will be postponed until subsequent chapters. On the other hand, the next theorem will give us a way to prove the results that require some kind of transfinite induction argument without doing it explicitly. To state it we need the following definitions. 

For a partially ordered set $\langle P , \leq \rangle$ we say that a set $S \subset P$ is a chain in P if S is linearly ordered by $\leq$ . An element $b \in P$ is said to be an upper bound of a set $S \subset P { \mathrm { ~ i f ~ } } s \leq b$ for every $s \in S$ . Similarly, $b \in P$ is a lower bound of $S \subset P$ if $b \leq s$ for every $s \in S$ 

Notice that not all subsets of a partially ordered set must have upper or lower bounds. For example, $( 0 , \infty ) \subset$ R does not have an upper bound and every number $r \leq 0$ is a lower bound of $( 0 , \infty )$ 

Let us also recall that $m \in P$ is a maximal element of $\langle P , \leq \rangle$ if there is no $p \in P$ such that $m < p$ 

Theorem 4.3.4 (Zorn’s lemma<sup>2</sup>) $I f \ \langle P , \leq \rangle$ is a partially ordered set such that every chain in P has an upper bound then P has a maximal element m. 

Proof The proof is similar to that of Theorem 4.3.3. Let C be a choice function on the family ${ \mathcal { P } } ( P ) \backslash \{ \emptyset \}$ . Choose an arbitrary $x \notin P$ , for example, $x = P ,$ and define $F \colon { \mathcal { P } } ( P \cup \{ x \} )  P \cup \{ x \}$ by 

$$
F (Z) = \left\{ \begin{array}{l l} C (Z) & \text { for } Z \in \mathcal {P} (P) \setminus \{\emptyset \}, \\ x & \text { otherwise }. \end{array} \right.
$$

Let $\mathcal { G }$ be the family of all ordinal numbers $\xi$ such that there is a strictly increasing sequence $\langle p _ { \zeta } \colon \zeta < \xi \rangle$ in P. Let α be an ordinal number that does not belong to $\mathcal { G }$ . For example, take $\alpha = ( \bigcup \mathcal { G } ) + 1$ 

Define a function h on the family of all ξ-sequences $\langle p _ { \zeta } : \zeta ~ < ~ \xi \rangle$ in $P \cup \{ x \} , \xi < \alpha$ , by putting 

$$
h (\langle p _ {\zeta} \colon \zeta <   \xi \rangle) = F (B \setminus \{p _ {\zeta} \colon \zeta <   \xi \}),\tag{4.9}
$$

where $B = \{ b \in P \colon b$ is an upper bound of $\{ p _ { \zeta } \colon \zeta < \xi \} \}$ . (Notice that $B = \emptyset$ if $\{ p _ { \zeta } \colon \zeta < \xi \} \not \subset P . )$ By the recursion theorem, there is a function $f$ such that 

$$
f (\xi) = h (f | _ {\xi}) \text { for   all } \xi <   \alpha .
$$

Notice that for every $\beta \leq \alpha$ 

$$
\text { if   } f [ \beta ] \subset P \text {   then   } f | _ {\beta} \text {   is   strictly   increasing. }\tag{4.10}
$$

This is the case, since then, by (4.9), $f ( \xi ) \in B \setminus \{ p _ { \zeta } \colon \zeta < \xi \}$ for $\xi < \beta .$ . In particular, $f [ \alpha ] \parallel { } \parallel { } P$ since there is no strictly increasing α-sequence in $P .$ $\mathrm { S o }$ the set $S = \{ \beta \leq \alpha \colon f ( \beta ) = x \}$ is nonempty. Let $\beta = \operatorname* { m i n } S$ . Then $f | _ { \beta }$ is strictly increasing, so $B = \{ b \in P \colon$ : b is an upper bound of $\{ p \xi \colon \xi < \beta \} \}$ is nonempty, $\{ p \xi \colon \xi < \beta \}$ being a chain. Let $m \in B$ . It is enough to argue that m is a maximal element of P. But if there is a $y \in P$ with $y > m$ 2 then $y > m \ge p _ { \xi }$ for every $\xi < \beta$ . In particular, $y \in B \setminus \{ p _ { \xi } \colon \xi < \beta \}$ , so 

$B \setminus \{ p _ { \xi } \colon \xi < \beta \} \ne \emptyset$ . Thus, by $( 4 . 9 ) , f ( \beta ) \in P$ , contradicting the choice of $\beta$ .  

Zorn’s lemma is used most often in the situation when P is a family of subsets of a set A ordered by inclusion and such that for every chain $S \subset P$ its union S is also in $P .$ . (Notice that S is an upper bound for $S$ with respect $\mathrm { t o } \ \subset . )$ In this particular case Zorn’s lemma has an especially nice form, stated as the following corollary. 

Corollary 4.3.5 (Hausdorf maximal principle) $I f { \mathcal { F } }$ is a nonempty family of subsets of a set A such that for every chain $S \subset { \mathcal { F } }$ its union $\cup S$ belongs to $\mathcal { F }$ then $\mathcal { F }$ has an ⊂-maximal element. 

Remark Zorn’s lemma and the Hausdorf maximal principle are equivalent to the axiom of choice within the ZF theory. To see this first notice that Zorn’s lemma follows from the axiom of choice (Theorem 4.3.4) and that the Hausdorf maximal principle follows from Zorn’s lemma (Corollary 4.3.5). To see that the Hausdorf maximal principle implies the axiom of choice let $\mathcal { G }$ be a nonempty family of pairwise-disjoint nonempty sets. We have to find a selector $S$ for $\mathcal { G }$ . So let $\mathcal { F }$ be the family of all $T \subset \cup \mathcal { G }$ such that $T \cap G$ has at most one element for every $G \in { \mathcal { G } }$ . Notice that $\mathcal { F }$ satisfies the assumptions of the Hausdorf maximal principle. Let $S \in { \mathcal { F } }$ be maximal. We will show that $S$ is a selector for $\mathcal { G }$ . But if $S$ is not a selector for $\mathcal { G }$ then $G \cap S = \emptyset$ for some $G \in { \mathcal { G } }$ . Then there is a $g \in G$ and $S \cup \{ g \}$ is in $\mathcal { F }$ , contradicting the maximality of S. 

## EXERCISE

1 Complete the details of the proof of Theorem 4.3.2. 

## 4.4 Zorn’s lemma in algebra, analysis, and topology

In this section we will see three standard applications of Zorn’s lemma in three main branches of mathematics: algebra, analysis, and topology. Each of these areas will be represented, respectively, by the theorem that every linear space has a basis, the Hahn–Banach theorem, and the Tychonof theorem. Going through these proofs should help the reader to appreciate the power of $\operatorname { Z o r n } ^ { \prime }$ s lemma and, implicitly, the axiom of choice. The Hahn–Banach theorem and the Tychonof theorem will not be used in the remaining part of this text. 

Algebraic application To state the algebraic example let us recall the following definitions. A set $G$ with a binary operation $+ \colon G \times G \to G$ is a group if + is associative $( { \mathrm { i . e . , ~ } } ( u + v ) + w = u + ( v + w )$ for all $u , v , w \in G )$ G has the identity element $0 \ ( { \mathrm { i . e . , ~ } } 0 + v = v + 0 = v$ for every $v \in G )$ , and every element of G has an inverse element (i.e., for every $v \in G$ there exists $- v \in G$ such that $( - v ) + v = v + ( - v ) = 0 )$ . A group $\langle G , + \rangle$ is Abelian if $a + b = b + a$ for every a, $b \in G$ . A set K with two binary operations + and · on K is a field if $\langle K , + \rangle$ is an Abelian group with 0 as an identity element, $\langle K \backslash \{ 0 \} , \cdot \rangle$ is an Abelian group with 1 as an identity element, and $a ( b + c ) = a b + a c$ for every $a , b , c \in K$ . In what follows we will mainly be concerned with the fields $\langle \mathbb { R } , + , \cdot \rangle$ of real numbers and $\langle \mathbb { Q } , + , \cdot \rangle$ of rational numbers. 

An Abelian group $\langle V , + \rangle$ is said to be a linear space (or vector space) over a field K if there is an operation from $K \times V \ \mathrm { t o } \ V , \langle k , v \rangle  k v$ , such that $( k + l ) v = k v + l v , k ( v + w ) = k v + k w , k ( l v ) = ( k l ) v , 0 v = 0$ , and $1 v = v$ for every $k , l \in K$ and $v , w \in V$ . A subset S of a vector space V over a field K is a linear subspace of V if it is a linear space when considered with the same operations. The main examples of vector spaces considered in this text will be $\mathbb { R } ^ { n }$ over either R or Q. 

A subset S of a vector space V over a field K is linearly independent if for every finite number of distinct elements $v _ { 1 } , \ldots , v _ { n }$ of S and every $k _ { 1 } , \dots , k _ { n } \in K$ the condition $k _ { 1 } v _ { 1 } + \cdot \cdot \cdot + k _ { n } v _ { n } = 0$ implies $k _ { 1 } = \cdots = k _ { n } =$ 0. A subset S of a vector space V over a field K spans V if every $v \in V$ can be represented as $v = k _ { 1 } v _ { 1 } + \cdot \cdot \cdot + k _ { n } v _ { n }$ for some $v _ { 1 } , \ldots , v _ { n } \in S$ and $k _ { 1 } , \dots , k _ { n } \in K$ . A basis of V is a linearly independent subset of V that spans V. 

It is easy to see that if B is a basis of V then every $v \in V$ has a unique representation $v = k _ { 1 } v _ { 1 } + \cdot \cdot \cdot + k _ { n } v _ { n }$ , where $v _ { 1 } , \dots , v _ { n } \in B$ are diferent and $k _ { 1 } , \dots , k _ { n } \in K$ (and where we ignore the $v _ { i } \mathrm { s }$ for which $k _ { i } = 0 )$ . This is the case since if $v = l _ { 1 } v _ { 1 } + \cdot \cdot \cdot + l _ { n } v _ { n }$ is a diferent representation of v, then $( l _ { 1 } - k _ { 1 } ) v _ { 1 } + \cdot \cdot \cdot + ( l _ { n } - k _ { n } ) v _ { n } = v - v = 0 \ s o \ l _ { 1 } - k _ { 1 } = \cdot \cdot \cdot = l _ { n } - k _ { n } = 0$ Thus $l _ { i } = k _ { i }$ for $i \in \{ 1 , \ldots , n \}$ 

Theorem 4.4.1 $I f S _ { 0 }$ is a linearly independent subset of a vector space V over K then there exists a basis B of V that contains $S _ { 0 }$ 

In particular, every vector space has a basis. 

Proof The additional part follows from the main part, since the empty set is linearly independent in any vector space. 

To prove the main part of the theorem, let 

${ \mathcal { F } } = \{ S \subset V \colon S _ { 0 } \subset S$ and S is linearly independent in V}. 

Notice first that $\mathcal { F }$ satisfies the assumptions of the Hausdorf maximal principle. 

Clearly $\mathcal { F }$ is nonempty, since $S _ { 0 } \in { \mathcal { F } }$ . To check the main assumption, let $\mathcal { G } \subset \mathcal { F }$ be a chain in F with respect to $\subset$ . We will show that $\cup \mathcal { G }$ is linearly independent in V. So let $v _ { 1 } , \ldots , v _ { n }$ be diferent elements of $\cup \mathcal { G }$ and choose $k _ { 1 } , \dots , k _ { n } \in K$ such that $k _ { 1 } v _ { 1 } + \cdot \cdot \cdot + k _ { n } v _ { n } = 0$ . For every $i \in \{ 1 , \ldots , n \}$ let $G _ { i } \in \mathcal G$ be such that $v _ { i } \in G _ { i }$ . Since $\{ G _ { 1 } , \ldots , G _ { n } \}$ is a finite subset of a linearly ordered set G, we can find the largest element, say $G _ { j }$ , in this set. Then $v _ { i } \in G _ { i } \subset G _ { j }$ for all $i \in \{ 1 , \ldots , n \}$ . Hence all $v _ { i } \mathrm { s }$ are in a linearly independent set $G _ { j }$ . Thus $k _ { 1 } v _ { 1 } + \cdot \cdot \cdot + k _ { n } v _ { n } = 0$ implies $k _ { 1 } = \cdot \cdot \cdot = k _ { n } = 0$ . So we can use the Hausdorf maximal principle on $\mathcal { F }$ 

Let B be a maximal element in F. We will show that it is a basis of V. It is linearly independent, since it belongs to $\mathcal { F }$ . So it is enough to prove that B spans V. 

To obtain a contradiction assume that there is a $v \in V$ such that 

$$
v \neq k _ {1} v _ {1} + \dots + k _ {n} v _ {n}\tag{4.11}
$$

for every $v _ { 1 } , \ldots , v _ { n } \in V$ and $k _ { 1 } , \ldots , k _ { n } \in K$ . We will show that this implies that $B \cup \{ v \}$ is linearly independent in V, which contradicts the maximality of B in $\mathcal { F }$ . So choose diferent elements $v _ { 1 } , \ldots , v _ { n }$ from $\boldsymbol { B }$ and $k _ { 0 } , \dots , k _ { n } \in K$ such that $k _ { 0 } v + k _ { 1 } v _ { 1 } + \cdot \cdot \cdot + k _ { n } v _ { n } = 0$ . There are two cases. Case 1: $k _ { 0 } = 0$ . Then $k _ { 1 } v _ { 1 } + \cdot \cdot \cdot + k _ { n } v _ { n } = 0$ and $v _ { 1 } , \ldots , v _ { n }$ are from B. Hence, also $k _ { 1 } = \cdot \cdot \cdot = k _ { n } = 0$ 

Case 2: $k _ { 0 } \neq 0$ . Then $v = - ( k _ { 1 } / k _ { 0 } ) v _ { 1 } + \cdot \cdot \cdot - ( k _ { n } / k _ { 0 } ) v _ { n }$ , contradicting (4.11).  

Analytic application For the next theorem the term vector space will be used for the vector spaces over the field R of real numbers. Recall that a function f is said to be a linear functional on a vector space V if $f \colon V \to$ R is such that $f ( a x + b y ) = a f ( x ) + b f ( y )$ for every $x , y \in V$ and $a , b \in \mathbb { R }$ 

Theorem 4.4.2 (Hahn–Banach theorem) Let V be a vector space and $p \colon V  \mathbb { R }$ be such that $p ( x + y ) \leq p ( x ) + p ( y )$ and $p ( a x ) \ : = \ : a p ( x )$ for all $x , y \in V$ and $a \geq 0$ . If f is a linear functional on a linear subspace S of V such that $f ( s ) \leq p ( s )$ for all $s \in S$ , then there exists a linear functional F on V such that F extends f and $F ( x ) \leq p ( x )$ for all $x \in V$ 

Proof Let $\mathcal { F }$ be the family of all functionals g on a linear subspace $T$ of V such that g extends f and $g ( x ) \leq p ( x )$ for all $x \in T$ . First we will show that $\mathcal { F }$ satisfies the assumptions of the Hausdorf maximal principle. 

So let $\mathcal { G } \subset \mathcal { F }$ be a chain in $\mathcal { F }$ with respect to ⊂. We will show that $\bigcup { \mathcal { G } } \in { \mathcal { F } }$ . Clearly $f \subset \bigcup { \mathcal { G } }$ . To see that $g = \cup \mathcal { G }$ is a functional, notice first  that g is a function since for $\langle x , s _ { 0 } \rangle , \langle x , s _ { 1 } \rangle \in g$ we can find $g _ { 0 } , g _ { 1 } \in \mathcal { G }$ such that $\langle x , s _ { i } \rangle \in g _ { i }$ for $i \ : < \ : 2$ . Then, for $g _ { 0 } \subset g _ { 1 } , s _ { 0 } = g _ { 0 } ( x ) = g _ { 1 } ( x ) = s _ { 1 }$ Similarly, if $g _ { 1 } \subset g _ { 0 }$ then $s _ { 1 } = g _ { 1 } ( x ) = g _ { 0 } ( x ) = s _ { 0 }$ 

In a similar way we show that the domain of $g$ is a linear subspace and that $g$ is a linear functional on its domain. Since also $g ( x ) \leq p ( x )$ for all $x \in \operatorname { d o m } ( g )$ , we conclude that $g \in { \mathcal { F } }$ , that is, $\mathcal { F }$ satisfies the assumptions of the Hausdorf maximal principle. 

Now let $F \colon T  \mathbb { R }$ be a maximal element of $\mathcal { F }$ . Then $F$ is a linear functional extending f such that $F ( x ) \leq p ( x )$ for every $x \in T$ . It is enough to prove that $T = V$ 

To obtain a contradiction assume that $V \neq T$ and let $w \in V \backslash T$ . We will show that this contradicts the maximality of $F$ by constructing a $G \in { \mathcal { F } }$ that extends $F$ and is defined on a linear subspace $V _ { 0 } = \operatorname { S p a n } ( T \cup \{ w \} ) =$ $\{ a w + t \colon a \in \mathbb { R } , \ t \in T \}$ of $V$ . 

First notice that for every s, $t \in T$ 

$$
F (s) + F (t) = F (s + t) \leq p (s + t) = p (s - w + t + w) \leq p (s - w) + p (t + w)
$$

and so 

$$
- p (s - w) + F (s) \leq p (t + w) - F (t).
$$

Hence, in particular, 

$$
\sup _ {t \in T} [ - p (t - w) + F (t) ] \leq \inf _ {t \in T} [ p (t + w) - F (t) ].
$$

Choose α such that sup $\left[ - p ( t - w ) + F ( t ) \right] \leq \alpha \leq \operatorname* { i n f } [ p ( t + w ) - F ( t ) ]$ . Then 

$$
\alpha \leq \inf [ p (t + w) - F (t) ] \& - \alpha \leq \inf [ p (t - w) - F (t) ].\tag{4.12}
$$

Now for $a \in \mathbb { R }$ and $t \in T$ define 

$$
G (a w + t) = a \alpha + F (t).
$$

Clearly G is a functional on $V _ { 0 }$ that extends F. We have to show only that $G ( s ) \leq p ( s )$ for all $s \in V _ { 0 }$ . So let $\boldsymbol { s } = a \boldsymbol { w } + t$ with $t \in T , a \in \mathbb { R }$ 

If $a = 0$ then $G ( a w + t ) = F ( t ) \leq p ( t ) = p ( a w + t )$ 

If $a > 0$ then, by the first part of (4.12), 

$$
\begin{array}{r c l} G (a w + t) & = & a \alpha + F (t) \\ & = & a [ \alpha + F (t / a) ] \\ & \leq & a [ [ p (t / a + w) - F (t / a) ] + F (t / a) ] \\ & = & a p (t / a + w) \\ & = & p (t + a w). \end{array}
$$

If $a = - b < 0$ then, by the second part of (4.12), 

$$
\begin{array}{r c l} G (a w + t) & = & - b \alpha + F (t) \\ & = & b [ - \alpha + F (t / b) ] \\ & \leq & b [ [ p (t / b - w) - F (t / b) ] + F (t / b) ] \\ & = & b p (t / b - w) \\ & = & p (t + a w). \end{array}
$$

This finishes the proof of Theorem 4.4.2. 

Topological application Let us start by recalling some definitions. A family $\mathcal { F }$ of subsets of a set $X$ is said to be a cover of a set $A \subset X$ if $A \subset \bigcup { \mathcal { F } }$ . If $\mathcal { F }$ is a cover of A then a family $\mathcal { G } \subset \mathcal { F }$ is said to be a subcover of $\mathcal { F }$ if $A \subset \cup \mathcal { G }$ . If $\langle X , \tau \rangle$ is a topological space then $\mathcal { F }$ is said to be an open cover of $A \subset X { \mathrm { ~ i f ~ } } A \subset \bigcup { \mathcal { F } }$ and $\mathcal { F } \subset \tau$ . A topological space $\langle X , \tau \rangle$ is compact if every open cover of X has a finite subcover. 

For a topological space $\langle X , \tau \rangle$ a family $B \subset \tau$ is said to be a base for X if for every $U \in \tau$ and every $x \in U$ there exists a $B \in B$ such that $x \in B \subset U$ . A family $s \subset \tau$ is said to be a subbase of topological space $\langle X , \tau \rangle$ if the family 

$$
\mathcal {B} (\mathcal {S}) = \left\{\bigcap_ {i <   n} S _ {i} \in \mathcal {P} (X) \colon n \in \mathbb {N} \& \forall i <   n \left(S _ {i} \in \mathcal {S}\right) \right\}
$$

forms a base for $X$ . It is easy to see that for any family $s$ of subsets of a set X the family 

$$
\mathcal {T} (\mathcal {S}) = \left\{\bigcup \mathcal {G}: \mathcal {G} \subset \mathcal {B} (\mathcal {S}) \right\}
$$

forms a topology on X. This topology is said to be generated by ${ \mathcal { S } } .$ The family $s$ is also a subbase for the topology $\mathcal { T } ( \boldsymbol { S } )$ 

Finally, let us recall that for a family $\{ \langle X _ { \alpha } , \tau _ { \alpha } \rangle \} _ { \alpha \in \mathcal { A } }$ of topological spaces their Tychonof product is a topological space defined on the product set $\begin{array} { r } { X = \prod _ { \alpha \in \mathcal { A } } X _ { \alpha } } \end{array}$ with topology generated by the subbase 

$$
\{p _ {\alpha} ^ {- 1} (U) \colon \alpha \in \mathcal {A} \& U \in \tau_ {\alpha} \},
$$

where $p _ { \alpha } \colon X \to X _ { \alpha }$ is the projection of X onto its αth coordinate $X _ { \alpha }$ 

Theorem 4.4.3 (Tychonof theorem) The product of an arbitrary family of compact spaces is compact. 

The proof will be based on the following lemma. 

Lemma 4.4.4 (Alexander subbase theorem) If there is a subbase $s$ of a topological space X such that every open cover $\nu \subset s$ of X has a finite subcover then X is compact. 

Proof Let S be a subbase of X such that any cover $\nu \subset s$ of X has a finite subcover. Let $\boldsymbol { B } = \boldsymbol { B } ( \boldsymbol { S } )$ be a base for X generated by $s$ and, to obtain a contradiction, assume that X is not compact. Then there is a subfamily $\mathcal { U } _ { 0 }$ of $B ( S )$ that covers X but does not have a finite subcover. (We use here an elementary fact that for any base B of a topological space $X ,$ the space X is compact if and only if every cover $u \subset B$ of X has a finite subcover.) 

Define $\mathcal { F }$ as 

$$
\left\{\mathcal {U} \subset \mathcal {B}: \mathcal {U} _ {0} \subset \mathcal {U}, X \subset \bigcup \mathcal {U}, \text { and   there   is   no   finite   subcover } \mathcal {V} \subset \mathcal {U} \text { of } X \right\}.
$$

To see that $\mathcal { F }$ satisfies the assumptions of the Hausdorf maximal principle let $\mathcal { G } \subset \mathcal { F }$ be a chain. If $\mathcal { T } \subset \bigcup \mathcal { G }$ is finite then there is a $\mathcal { U } \in \mathcal { G }$ such that $\tau \subset \mathcal { U }$ . So $\tau$ cannot cover X, since $\mathcal { U } \in \mathcal { F }$ . Thus $\cup \mathcal { G }$ does not have a finite subcover, that is, $\bigcup { \mathcal { G } } \in { \mathcal { F } }$ 

So, by the Hausdorf maximal principle, there is a maximal element $\mathcal { U } \in \mathcal { F }$ . Now let $U \in \mathcal { U }$ . Then $\textstyle U = \bigcap _ { i < n } U _ { i }$ for some $U _ { i } \in { \cal S }$ . We claim that 

$$
\text { there   is   a } j <   n \text { such   that } U _ {j} \in \mathcal {U}.\tag{4.13}
$$

Otherwise, for every $i < n$ we can find a finite $u _ { i } \subset \mathcal { U }$ such that $\mathcal { U } _ { i } \cup \{ U _ { i } \}$ covers $X$ , that is, $\boldsymbol { \mathcal { U } } _ { i }$ covers $X \backslash U _ { i }$ . But then $\cup _ { i < n } \mathcal { U } _ { i }$ covers $\begin{array} { r } { \bigcup _ { i < n } ( X \backslash U _ { i } ) = } \end{array}$ $\textstyle X \setminus \bigcap _ { i < n } U _ { i } = X \setminus U$ . So $\textstyle \bigcup _ { i < n } { \mathcal { U } } _ { i } \cup \{ U \} \subset { \bar { \mathcal { U } } }$ is a finite subcover of X, contradicting the fact that $\mathcal { U } \in \mathcal { F }$ 

But (4.13) implies that for every $U \in \mathcal { U }$ there is a $V = U _ { j } \in \mathcal { U } \cap \mathcal { S }$ such that $U \subset V . \ \mathrm { S o } \ { \mathcal { V } } = { \mathcal { U } } \cap { \mathcal { S } }$ is also a cover of $X$ . Hence, by our assumption, V has a finite subcover of X. This contradiction finishes the proof.  

Proof of the Tychonof theorem Let 

$$
\mathcal {S} = \{p _ {\alpha} ^ {- 1} (U) \colon \alpha \in \mathcal {A} \& U \in \tau_ {\alpha} \}
$$

be a subbase of $\begin{array} { r } { X = \prod _ { \alpha \in \mathcal { A } } X _ { \alpha } } \end{array}$ and let $u \subset s$ be a cover of $X$ . By the Alexander subbase theorem it is enough to find a finite subcover of $\mathcal { U }$ . For $\alpha \in { \mathcal { A } }$ let 

$$
\mathcal {U} _ {\alpha} = \{U \subset X _ {\alpha} \colon U \text { is   open   in } X _ {\alpha} \text { and } p _ {\alpha} ^ {- 1} (U) \in \mathcal {U} \}.
$$

If for some $\alpha \in { \mathcal { A } }$ the family $\mathcal { U } _ { \alpha }$ covers $X _ { \alpha }$ then, by the compactness of $X _ { \alpha }$ , there is a finite subcover $\nu \subset \mathcal { U } _ { \alpha }$ that covers $X _ { \alpha }$ . But then $\mathcal { U } ^ { \prime } = \{ p _ { \alpha } ^ { - 1 } ( U ) : U \in \mathcal { V } \} \subset \mathcal { U }$ is a finite subcover of $X , \mathrm { ~ \tiny ~ \textnormal ~ { ~ S o ~ } ~ }$ , to obtain a contradiction, assume that no $\mathcal { U } _ { \alpha }$ covers $X _ { \alpha }$ and let $x ( \alpha ) \in X _ { \alpha } \backslash \bigcup { \mathcal { U } } _ { \alpha }$ for every $\alpha \in { \mathcal { A } }$ . Then $x \in X \setminus \bigcup _ { \alpha \in { \mathcal { A } } } \bigcup \{ p _ { \alpha } ^ { - 1 } ( U ) \colon U \in { \mathcal { U } } _ { \alpha } \} = X \setminus \bigcup { \dot { \mathcal { U } } }$ . This finishes the proof.  

## EXERCISES

1 Prove that every partial-order relation% on a set X can be extended to a linear-order relation≤ on X. (Here ≤ extends $\preceq { \mathrm { i f ~ } } \preceq { \mathsf { C } } { \leq } . )$ 

2 We say that a subset $A \subset \mathbb { R }$ is algebraically independent if for every nonzero polynomial $p ( x _ { 1 } , \ldots , x _ { n } )$ of n variables with rational coeficients and any sequence $a _ { 1 } , \ldots , a _ { n }$ of diferent elements from A, $p ( a _ { 1 } , \ldots , a _ { n } ) \neq$ 0. Show that there exists an algebraically independent subset A of R such that if $\mathbb { Q } ( \mathcal { A } )$ is a field generated by Q and A then for every $b \in \mathbb { R } \setminus \mathbb { Q } ( { \mathcal { A } } )$ there exists a nonzero polynomial $p ( x )$ with coeficients in $\mathbb { Q } ( A )$ such that $p ( b ) = 0$ . (A family A with this property is called a transcendental basis of R over Q.) 

3 A filter on a set X is a nonempty family $\mathcal { F }$ of subsets of X such that (1) $A \cap B \in { \mathcal { F } }$ provided A, $B \in { \mathcal { F } } ;$ and (2) if $A \subset B \subset X$ and $A \in { \mathcal { F } }$ then $B \in { \mathcal { F } }$ . A filter F on X is proper if ${ \mathcal { F } } \neq { \mathcal { P } } ( X )$ , and it is prime if for every $A \subset X$ either $A \in { \mathcal { F } }$ or $X \setminus A \in { \mathcal { F } }$ . Show that every proper filter on a set X can be extended to a proper prime filter. 

4 A graph on a (finite or infinite) set V is an ordered pair $\langle V , E \rangle$ such that $E \subset [ V ] ^ { 2 }$ , where $[ V ] ^ { 2 }$ is the set of all two-element subsets of V. For $E _ { 0 } \subset E$ a graph $\langle V , E _ { 0 } \rangle$ is a forest in graph $\langle V , E \rangle$ if it does not contain any cycle, that is, if there is no sequence $v _ { 0 } , v _ { 1 } , \ldots , v _ { n } = v _ { 0 }$ with $n > 2$ such that $\{ v _ { i } , v _ { i + 1 } \} \in E _ { 0 }$ for $i \in n$ . For $E _ { 0 } \subset E$ a graph $\langle V , E _ { 0 } \rangle$ spans $\langle V , E \rangle$ if for every $v \in V$ there is a $w \in V$ such that $\{ v , w \} \in E _ { 0 }$ 

Let $\langle V , E \rangle$ be a graph that spans itself. Show that there exists a forest $\langle V , E _ { 0 } \rangle$ that spans $\langle V , E \rangle$ 

# Cardinal numbers

## 5.1 Cardinal numbers and the continuum hypothesis

We say that the sets A and B have the same cardinality and write $A \approx B$ if there exists a bijection $f \colon A \to B$ 

It is easy to see that for every A, B, and C 

$A \approx A$ 

• if $A \approx B$ then $B \approx A ;$ ; and 

• if $A \approx B$ and $B \approx C$ then $A \approx C$ 

Thus the “relation” ≈ of having the same cardinality is an equivalence $^ { 6 } \mathrm { r e } -$ lation.” We put the word relation in quotation marks since our definition does not specify any field for ≈. This means that the “field” of this “relation” is the class of all sets. However, the restriction of ≈ to any set X is an equivalence relation on X. Thus we will use the term relation for ≈ in this sense. 

By Zermelo’s theorem (Theorem 4.3.3) and Theorem 4.2.4, for every set A there exists an ordinal number α such that $A \approx \alpha$ . The smallest ordinal number with this property is called the cardinality of A and is denoted by $| A |$ . Thus 

$$
| A | = \min \{\alpha : \alpha \text {   is   an   ordinal   number   and   } A \approx \alpha \}.
$$

In particular, $A \approx | A |$ for every A. It is not dificult to see that $A \approx B$ if and only if $| A | = | B |$ . Thus the terminology “sets A and B have the same cardinality” can be used for $A \approx B$ as well as for $| A | = | B |$ 

Notice also that 

|α| ≤ α for every ordinal number $\alpha ,$ 

since $\alpha \approx \alpha$ and $| \alpha |$ is the smallest ordinal $\beta$ such that $\alpha \approx \beta$ . This implies also that 

$$
| \alpha | \leq | \beta | \text {   for   all   ordinal   numbers   } \alpha \leq \beta .
$$

An ordinal number κ is said to be a cardinal number (or just a cardinal) provided $\kappa = | A |$ for some set A. We can distinguish the cardinal numbers from all other ordinal numbers by using the following properties. 

Proposition 5.1.1 For an ordinal number α the following conditions are equivalent: 

(i) α is a cardinal number; 

(ii) $| \alpha | = \alpha ,$ 

(iii) $\beta < | \alpha |$ for every $\beta < \alpha$ 

(iv) $| \beta | < | \alpha |$ for every $\beta < \alpha ,$ 

(v) $| \beta | \neq | \alpha | ~ f o r ~ e v e r y ~ \beta < \alpha .$ 

Proof $( \mathrm { i } ) { \Rightarrow } ( \mathrm { i i } )$ : If α is a cardinal number then there exists a set A such that $| A | = \alpha$ . This means, in particular, that $A \approx \alpha ,$ that is, $| A | = | \alpha |$ . So $| \alpha | = | A | = \alpha$ 

(ii)⇒(iii): It is obvious. 

$( \mathrm { i i i } ) { \Rightarrow } ( \mathrm { i v } )$ : It follows from the fact that $| \beta | \le \beta$ for every ordinal $\beta .$ 

$( \mathrm { i v } ) { \Rightarrow } ( \mathrm { v } )$ : It is obvious. 

(v)⇒(i): Condition (v) implies that $\beta \not \approx \alpha$ for every $\beta < \alpha$ . Thus $\alpha$ is the smallest ordinal $\gamma$ such that $\alpha \approx \gamma$ . But this means, by the definition of cardinality, that α is a cardinal number, as then $\alpha = | \alpha |$  

Property $\mathrm { ( v ) }$ of Proposition 5.1.1 explains why we often say that the cardinal numbers are the initial ordinals, that is, ordinals that are the smallest of a given cardinality. 

Let us also note the following theorem. 

Theorem 5.1.2 Let A and B be arbitrary sets. The following conditions are equivalent: 

(i) $| A | \leq | B |$ ; 

(ii) there exists a one-to-one function $g \colon A  B$ 

Moreover, $i f A \neq \emptyset$ then these conditions are equivalent to the condition that 

(iii) there exists a function f : $B  A$ from B onto A. 

Proof For $A = \emptyset$ the equivalence of (i) and (ii) is obvious. So assume that $A \neq \emptyset$ 

$( \mathrm { i } ) { \Rightarrow } ( \mathrm { i i i } )$ : Let $h \colon B \to | B |$ and $g \colon | A |  A$ be bijections. Pick $a \in A$ Notice that $| A | \subset | B |$ and $h ^ { - 1 } ( | A | ) \subset B$ 

Define $f \colon B \to A$ by 

$$
f (b) = \left\{ \begin{array}{l l} g (h (b)) & \text { for } b \in h ^ {- 1} (| A |), \\ a & \text { otherwise }. \end{array} \right.
$$

Then 

$$
A \supset f [ B ] \supset f [ h ^ {- 1} (| A |) ] = (g \circ h) [ h ^ {- 1} (| A |) ] = g [ | A | ] = A.
$$

So f is onto A. 

$( \mathrm { i i i } ) { \Rightarrow } ( \mathrm { i i } )$ : Let $f \colon B \to A$ be onto. Let G be a choice function for the family $\{ f ^ { - 1 } ( a ) \colon a \in A \}$ . Then $g ( a ) = G ( f ^ { - 1 } ( a ) )$ is a one-to-one function from A into B. 

$( \mathrm { i i } ) { \Rightarrow } ( \mathrm { i } )$ : Let $g \colon A \ \to \ B$ be a one-to-one function and h: $B  | B |$ be a bijection. Then $( h \circ g ) \colon A  | B |$ is a one-to-one function from A onto $( h \circ g ) [ A ] \subset | B |$ . Hence $| A | = | ( h \circ g ) [ A ] |$ and, by Corollary 4.2.6, $\operatorname { O t p } ( ( h \circ g ) [ A ] ) \leq | B |$ . So 

$$
| A | = | (h \circ g) [ A ] | = | \operatorname{Otp} ((h \circ g) [ A ]) | \leq \operatorname{Otp} ((h \circ g) [ A ]) \leq | B |.
$$

Corollary 5.1.3 If $A \subset B$ then $| A | \leq | B |$ 

Proof Since the identity function from A into B is one-to-one, the corollary follows immediately from Theorem 5.1.2.  

Corollary 5.1.4 If $A \subset B \subset C \ a n d | A | = | C | \ t h e n \ | B | = | A | .$ 

Proof By Corollary 5.1.3 we have $| A | \leq | B | \leq | C | = | A | . \mathrm { \ S o } \ | B | = | A |$ .  

Remark It is often the case that the relation $A \preceq B$ for a set A having cardinality less than or equal to the cardinality of $B , \left| A \right| \leq \left| B \right|$ , is defined as in Theorem 5.1.2(ii), that is, by saying that there exists a one-to-one function $f \colon A \to B$ . Then it is necessary to prove that $A \preceq B$ and $B \preceq A$ imply that there exists a bijection from A onto B. This fact is known as the Schr¨oder–Bernstein theorem and follows immediately from our definition and Theorem 5.1.2. 

Theorem 5.1.5 $\omega$ is a cardinal number and every $n \in \omega$ is a cardinal number. 

Proof First we show that every $n \in \omega$ is a cardinal number. So let $n \in \omega$ By Proposition 5.1.1(iv) it is enough to prove that $| k | < | n |$ for every $k < n$ Thus it is enough to show that the inequality $| n | \leq | k |$ is false, that is, by Theorem 5.1.2, that 

there is no one-to-one function $f \colon n  k$ for every $k < n$ 

(5.1) 

We will prove (5.1) by induction on $n < \omega$ 

Notice that for $n = 0$ condition (5.1) is true, since there is no $k < n$ So assume that it is true for some $n < \omega$ . We will show that this implies (5.1) for $n + 1$ 

To obtain a contradiction assume that for some $k < n { + } 1$ there is a oneto-one function $f \colon ( n + 1 )  k$ . If $k < n$ then $f | _ { n } \colon n \to k$ contradicts (5.1). So $k = n , f \colon ( n + 1 ) \to n$ , and $f [ n + 1 ] \not \subset ( n - 1 )$ , that is, $n - 1 \in f [ n + 1 ]$ (Notice that n − 1 exists, since the existence of $f \colon ( n + 1 )  n$ implies that $n \neq 0 . )$ 

Let $i < n + 1$ be such that $f ( i ) = n - 1$ . Define $g \colon n  n - 1$ by putting $g ( j ) = f ( j )$ for $j < n , j \neq i$ , and $g ( i ) = f ( n )$ $( \operatorname { I f } i = n$ this last condition is redundant and can simply be ignored.) Notice that the values of g indeed belong to $n - 1$ and that g is one-to-one. Thus g contradicts (5.1) for n. This contradiction finishes the proof of (5.1) and the fact that every $n \in \omega$ is a cardinal number. 

To see that $\omega$ is a cardinal number notice that $n \subset ( n + 1 ) \subset \omega$ for every $n < \omega$ . Hence, by Corollary $5 . 1 . 3 , | n | \leq | n + 1 | \leq | \omega |$ . But by what we have already proved, $\left| n \right| = n < n + 1 = \left| n + 1 \right|$ . So $| n | < | n + 1 | \leq | \omega |$ , that is, we conclude that $| n | < | \omega |$ for every $n < \omega$ . Therefore, by Proposition 5.1.1, we deduce that $\omega$ is a cardinal number.  

The sets with cardinality less than $\omega .$ , that is, equal to some $n < \omega$ , are called finite sets. A set A is countable if $| A | = \omega$ . A set is infinite if it is not finite. A set is uncountable if it is infinite and not countable. 

We have already established a convention that general infinite ordinal numbers are denoted by the greek letters $\alpha , \beta , \gamma , \zeta , \eta , \xi$ . The infinite cardinal numbers will usually be denoted by the letters $\kappa , \mu , \lambda$ 

The natural numbers and $\omega$ are cardinal numbers. Are there any other $( \mathrm { i . e . , }$ , uncountable) cardinal numbers? The next theorem gives us a tool to construct a lot of uncountable cardinal numbers. 

Theorem 5.1.6 (Cantor’s theorem) $| X | < | P ( X ) |$ for every set $X$ . 

Proof Fix a set X. First notice that $| X | \leq | P ( X ) |$ , since the function $f \colon X \to { \mathcal { P } } ( X )$ defined by $f ( x ) = \{ x \}$ for $x \in X$ is one-to-one. 

To finish the proof it is enough to show that $| X | \neq | { \mathcal { P } } ( X ) |$ . So let $f \colon X \to { \mathcal { P } } ( X )$ . We will prove that $f$ is not a bijection by showing that $f$ is not onto ${ \mathcal { P } } ( X )$ . To see it, put 

$$
Y = \{x \in X \colon x \not \in f (x) \}.
$$

Then $Y \in { \mathcal { P } } ( X )$ is not in the range of $f .$ , since if there were a $z \in X$ such that $f ( z ) = Y$ then we would have 

$$
z \in Y \Leftrightarrow z \in \{x \in X: x \notin f (x) \} \Leftrightarrow z \notin f (z) \Leftrightarrow z \notin Y,
$$

a contradiction. 

Cantor’s theorem tell us, in particular, that for any cardinal number κ there is a cardinal number λ larger than κ, namely, $\lambda = | \mathcal { P } ( \kappa ) |$ . We will denote this cardinal number by $2 ^ { \kappa }$ . That way, the symbol $2 ^ { \kappa }$ will stand for two objects: a cardinal number and the family of all functions from κ into 2. Although these two object are definitely diferent, this notation is consistent in the sense that 

$$
| \mathcal {P} (X) | = \left| 2 ^ {X} \right| \text {   for   every   set   } X.\tag{5.2}
$$

This last equation is established by a bijection $\chi \colon { \mathcal { P } } ( X ) \to 2 ^ { X }$ defined by $\chi ( A ) = \chi _ { A }$ , where $\chi _ { A }$ is the characteristic function of A, that is, $\chi _ { A } ( x ) = 1$ for $x \in A$ and $\chi _ { A } ( x ) = 0$ for $x \in X \setminus A$ 

The notation $2 ^ { \kappa }$ is also consistent with the cardinal exponentiation operation that will be introduced in the next section. 

Notice also that for every cardinal number κ there is the smallest cardinal number λ greater than κ, namely, a cardinal equal to the minimum of the set 

$$
K = \{\mu \in 2 ^ {2 ^ {\kappa}}: \mu \text {   is   a   cardinal   and   } \kappa <   \mu \}.
$$

The minimum exists, since K is a nonempty $( 2 ^ { \kappa } \in K )$ subset of a wellordered set $2 ^ { 2 ^ { \kappa } }$ . This unique cardinal number is denoted by $\kappa ^ { + }$ and is called the cardinal successor of κ. 

It is also worthwhile to note the following property of cardinal numbers. 

Proposition 5.1.7 If $\mathcal { F }$ is a family of cardinal numbers then $\alpha = \cup { \mathcal { F } }$ is also a cardinal number. 

Proof By Theorem 4.2.3(iii) α is an ordinal number. Moreover, if $\beta <$ α then $\beta \in \alpha$ and there exists a $\kappa \in \mathcal { F }$ such that $\beta \in \kappa$ . So $\beta < \kappa = | { \boldsymbol { \kappa } } | \leq | { \boldsymbol { \alpha } } |$ Thus, by Proposition 5.1.1(iii), α is a cardinal number.  

With the use of Proposition 5.1.7 and the operation of cardinal successor we can construct for every ordinal number α a cardinal number $\omega _ { \alpha }$ by induction on $\xi \le \alpha$ in the following way: 

$$
\omega_ {0} = \omega ;
$$

$$
\omega_ {\xi + 1} = (\omega_ {\xi}) ^ {+} \mathrm{forevery} \xi <   \alpha ;
$$

$$
\omega_ {\lambda} = \bigcup_ {\xi <   \lambda} \omega_ {\xi} \text {   for   every   limit   } \lambda \leq \alpha .
$$

It is easy to see that $\omega _ { \alpha }$ is the αth infinite cardinal number. It is also worthwhile to mention that very often $\omega _ { \alpha }$ is denoted by $\aleph _ { \alpha }$ . (ℵ is a Hebrew letter pronounced aleph.) 

Similarly, for every ordinal number α we can construct a cardinal number $\beth _ { \alpha }$ by induction on $\xi \le \alpha$ as follows: 

$$
\beth_ {0} = \omega ;
$$

$$
\beth_ {\xi + 1} = 2 ^ {\beth_ {\xi}} \mathrm{forevery} \xi <   \alpha ;
$$

$$
\beth_ {\lambda} = \bigcup_ {\xi <   \lambda} \beth_ {\xi} \text {   for   every   limit   } \lambda \leq \alpha .
$$

( is a Hebrew letter, which we read bet.) In particular, the cardinality of $\mathcal { P } ( \omega )$ is equal to $\beth _ { 1 } = 2 ^ { \omega }$ . This number is usually denoted by c, a Hebrew letter $c ,$ which we read continuum. 

Obviously, $\omega _ { 0 } ~ = ~ \omega ~ = ~ \beth _ { 0 }$ and, by Cantor’s theorem, $\omega _ { 1 } \leq \beth _ { 1 } = { \mathfrak { c } } .$ It is also not dificult to prove that $\omega _ { \alpha } \leq \exists _ { \alpha }$ for every ordinal number $\alpha .$ Two natural questions that arise in this context are the following: Is $\omega _ { 1 } = { \mathfrak { c } } ? \ { \mathrm { I s } } \ \omega _ { \alpha } = \exists _ { \alpha }$ for every ordinal number $\alpha ?$ Surprisingly, both these questions cannot be decided within ZFC set theory. The statement that $\omega _ { 1 } = \mathfrak { c }$ is called the continuum hypothesis (usually abbreviated by CH) and is independent of ZFC set theory (see Section 1.1). Similarly, the statement ${ ^ { 6 } \omega } _ { \alpha } = \beth _ { \alpha }$ for every ordinal number $\alpha ^ { \mathfrak { N } }$ is called the generalized continuum hypothesis (usually abbreviated by GCH) and is also independent of ZFC set theory. 

The independence of CH from the ZFC axioms will be proved in Chapter 9. Meanwhile, we will often use CH as an additional assumption to deduce other properties of interest. That way, we will know that the deduced properties are consistent with ZFC set theory, that is, that we have no way to prove their negations using only ZFC axioms. 

The last theorem of this section gives some rules on comparing the cardinalities of sets. 

Theorem 5.1.8 $I f \left| A \right| = \left| B \right|$ and $| C | = | D |$ then 

(a) $| A \times C | = | B \times D |$ ; 

(b) $| A \cup C | = | B \cup D |$ , provided $A \cap C = \varnothing = B \cap D$ ; 

(c) $\left| A ^ { C } \right| = \left| B ^ { D } \right|$ 

Proof Let $f \colon A \to B$ and $g \colon C \to D$ be bijections. Define the bijections for $\mathrm { ( a ) - ( c ) }$ as follows: 

(a) $F \colon A \times C \to B \times D , F ( a , c ) = \langle f ( a ) , g ( c ) \rangle .$ 

(b) $F \colon A \cup C \to B \cup D , F = f \cup g .$ 

(c) $F \colon A ^ { C } \to B ^ { D }$ , and $F ( h ) \in B ^ { D }$ for $h \in A ^ { C }$ is defined by the formula $F ( h ) ( d ) = f ( h ( g ^ { - 1 } ( d ) ) )$ for every $d \in D$ 

It is left as an exercise to show that the functions F so defined are indeed bijections.  

We will finish this section with the following remark. The only cardinal numbers that were defined in a “natural” way (i.e., without an essential use of the axiom of choice) are the natural numbers and $\omega .$ . The infinite ordinal numbers that we can easily construct, that is, construct with the use of ordinal number operations, are of the form $\omega + 1 , \omega + 2 , \omega + \omega .$ ωω, and so forth, and are not cardinal numbers. (For example, notice that $| \omega \omega | \le \omega$ by defining the one-to-one function $f \colon \omega \omega  \omega$ with the formula $f ( n , m ) = 2 ^ { n } 3 ^ { m }$ , where we identify ωω with the set $\omega \times \omega$ from the definition of ωω.) In fact, there is no way to prove without the axiom of choice the existence of uncountable ordinal numbers. This might seem strange, since the proof of Cantor’s theorem evidently did not use the axiom of choice. However, we in fact proved there only that $| X | \neq | P ( X ) |$ . The proof that the set ${ \mathcal { P } } ( X )$ can indeed be well ordered requires the use of Zermelo’s theorem, which is equivalent to the axiom of choice. 

## EXERCISES

1 Let $n \in \omega$ . Show that if α is an ordinal number such that $| { \boldsymbol { \alpha } } | = n$ then $\alpha = n$ 

2 Prove that $\omega _ { \alpha } \leq \beth _ { \alpha }$ for every ordinal number $\alpha .$ 

3 Complete the proof of Theorem 5.1.8 by showing that all functions $F$ defined in this proof are bijections. 

## 5.2 Cardinal arithmetic

For cardinal numbers κ and λ define their cardinal sum by 

$$
\kappa \oplus \lambda = | (\kappa \times \{0 \}) \cup (\lambda \times \{1 \}) |,
$$

their cardinal product by 

$$
\kappa \otimes \lambda = | \kappa \times \lambda |,
$$

and a cardinal exponentiation operation by 

$$
\kappa^ {\lambda} = \left| \kappa^ {\lambda} \right|.
$$

Notice that the exponentiation operation for $\kappa = 2$ gives us another definition of $2 ^ { \lambda }$ . However, it is consistent with the previous definition, since $\left| 2 ^ { \lambda } \right| = 2 ^ { \lambda }$ . Notice also that by the foregoing definitions and Theorem 5.1.8,  for all sets A and B, 

$$
| A \cup B | = | A | \oplus | B | \quad \text { for } A \text { and } B \text { disjoint }\tag{5.3}
$$

and 

$$
\left| A \times B \right| = \left| A \right| \otimes \left| B \right|, \quad \left| A ^ {B} \right| = \left| A \right| ^ {\left| B \right|}.\tag{5.4}
$$

Proposition 5.2.1 For all cardinal numbers κ and λ 

(i) $\kappa \oplus \lambda = \lambda \oplus \kappa ,$ 

(ii) $\kappa \otimes \lambda = \lambda \otimes \kappa .$ 

Proof From Theorem 5.1.8 we have 

$$
\kappa \oplus \lambda = | (\kappa \times \{0 \}) \cup (\lambda \times \{1 \}) | = | (\lambda \times \{0 \}) \cup (\kappa \times \{1 \}) | = \lambda \oplus \kappa ,
$$

where the second equation follows from the fact that $| \kappa \times \{ 0 \} | = | \kappa \times \{ 1 \} |$ and $| \lambda \times \{ 1 \} | = | \lambda \times \{ 0 \} |$ . Also, 

$$
\kappa \otimes \lambda = | \kappa \times \lambda | = | \lambda \times \kappa | = \lambda \otimes \kappa ,
$$

since $f ( \zeta , \xi ) = \langle \xi , \zeta \rangle$ is a bijection between $\kappa \times \lambda$ and $\lambda \times \kappa$ 

Thus, unlike the ordinal operations + and ·, the cardinal operations ⊕ and $\otimes$ are commutative. 

Proposition 5.2.2 For every m, $n \in \omega$ 

(i) $m \oplus n = m + n < \omega ,$ 

(ii) $m \otimes n = m n < \omega .$ 

The proof is left as an exercise. 

Lemma 5.2.3 Every infinite cardinal number is a limit ordinal number. 

Proof First notice that 

$$
| \omega \cup \{x \} | = | \omega |.
$$

If $x \in \omega$ then this is obvious. Otherwise this is justified by a function $f \colon \omega \cup \{ x \}  \omega$ defined by $f ( x ) = 0$ and $f ( n ) = n + 1$ for $n < \omega$ . Hence, by Theorem 5.1.8(ii), for every infinite ordinal number α 

$$
| \alpha + 1 | = | \alpha \cup \{\alpha \} | = | (\alpha \setminus \omega) \cup (\omega \cup \{\alpha \}) | = | (\alpha \setminus \omega) \cup \omega | = | \alpha |.
$$

Therefore, by Proposition 5.1.1, an ordinal number $\alpha + 1$ is not a cardinal number for any infinite α.  

Theorem 5.2.4 If κ is an infinite cardinal then $\kappa \otimes \kappa = \kappa$ 

Proof Let κ be an infinite cardinal number. We will prove by transfinite induction on $\omega \leq \alpha \leq \kappa$ that 

$$
| \alpha | \otimes | \alpha | = | \alpha |.\tag{5.5}
$$

So let $\omega \leq \lambda \leq \kappa$ be such that (5.5) holds for every $\omega \leq \alpha < \lambda$ . We will show that (5.5) holds for λ as well. This will finish the proof. 

If there is an $\alpha < \lambda$ such that $| \alpha | = | \lambda |$ then 

$$
| \lambda | \otimes | \lambda | = | \alpha | \otimes | \alpha | = | \alpha | = | \lambda |.
$$

Hence we may assume that λ is a cardinal number. 

Now notice that for every α $< \lambda$ 

$$
| \alpha \times \alpha | <   \lambda .\tag{5.6}
$$

It follows from Proposition 5.2.2(ii) for a finite α and from (5.5) for an infinite α. Define a well ordering % on $\lambda \times \lambda$ by putting $\langle \alpha , \beta \rangle \preceq \langle \gamma , \delta \rangle$ if and only if 

$$
\max \{\alpha , \beta \} <   \max \{\gamma , \delta \}
$$

or 

$$
\max \{\alpha , \beta \} = \max \{\gamma , \delta \} \text { and } \langle \alpha , \beta \rangle \leq_ {\mathrm{lex}} \langle \gamma , \delta \rangle ,
$$

where $\leq _ { \mathrm { l e x } }$ stands for the lexicographic order on $\kappa \times \kappa$ (see Theorem 4.1.13). The proof that % is indeed a well ordering is left as an exercise. 

Now let $\langle \gamma , \delta \rangle \in \lambda \times \lambda$ and let $\varepsilon = \operatorname* { m a x } \{ \gamma + 1 , \delta + 1 \}$ . Then $\varepsilon < \lambda$ by Lemma 5.2.3. Moreover, the initial segment $O _ { \preceq } ( \langle \gamma , \delta \rangle )$ (generated by $\langle \gamma , \delta \rangle$ with respect to $\preceq )$ is a subset of $\varepsilon \times \varepsilon .$ since $\langle \alpha , \beta \rangle \preceq \langle \gamma , \delta \rangle$ implies that max $\{ \alpha , \beta \} \le$ max $\{ \gamma , \delta \} < \varepsilon$ . Hence, by (5.6), 

$$
| \operatorname{Otp} (O _ {\preceq} (\langle \gamma , \delta \rangle)) | = | O _ {\preceq} (\langle \gamma , \delta \rangle) | \leq | \varepsilon \times \varepsilon | = | \varepsilon | <   \lambda
$$

and so also 

$$
\mathrm{Otp} (O _ {\preceq} (\langle \gamma , \delta \rangle)) <   \lambda .
$$

(Otherwise, we would have $\lambda = | \lambda | \leq | \operatorname { O t p } ( O _ { \prec } ( \langle \gamma , \delta \rangle ) ) | . )$ Since every ordinal number $\beta \in \operatorname { O t p } ( \lambda \times \lambda , \preceq )$ is of the form $\operatorname { O t p } ( O _ { \preceq } ( \langle \gamma , \delta \rangle ) )$ we can conclude that $\operatorname { O t p } ( \lambda \times \lambda , \preceq ) \leq \lambda$ . So 

$$
| \lambda \times \lambda | = | \operatorname{Otp} (\lambda \times \lambda , \preceq) | \leq \operatorname{Otp} (\lambda \times \lambda , \preceq) \leq \lambda = | \lambda |.
$$

Thus $| \lambda \times \lambda | = | \lambda |$ , since the inequality $| \lambda | \leq | \lambda \times \lambda |$ is obvious. 

Corollary 5.2.5 If λ and κ are infinite cardinals then 

$$
\kappa \oplus \lambda = \kappa \otimes \lambda = \max \{\kappa , \lambda \}.
$$

Proof We may assume that $\lambda \leq \kappa$ . Then 

$$
\kappa \oplus \lambda = | (\kappa \times \{0 \}) \cup (\lambda \times \{1 \}) | \leq | \kappa \times 2 | \leq | \kappa \times \lambda | = \kappa \otimes \lambda
$$

and 

$$
\kappa \otimes \lambda = | \kappa \times \lambda | \leq | \kappa \times \kappa | = \kappa .
$$

Since evidently $\kappa \leq \kappa \oplus \lambda$ we obtain 

$$
\kappa \leq \kappa \oplus \lambda \leq \kappa \otimes \lambda \leq \kappa .
$$

Corollary 5.2.6 A countable union of countable sets is countable. 

Proof Let $\mathcal { F }$ be a countable family of countable sets, $\mathcal { F } = \{ F _ { n } : n < \omega \}$ Then for every $n < \omega$ there is a bijection $f _ { n } \colon \omega \to F _ { n }$ . Define function $f \colon \omega \times \omega  \bigcup \mathcal { F }$ by putting $f ( n , m ) = f _ { n } ( m )$ . Notice that f is onto. So, by Theorem 5.1.2, $| \bigcup { \mathcal { F } } | \leq | \omega \times \omega | = \omega$ . Hence $| \cup \mathcal { F } | = \omega .$  

Similarly, we can prove the following. 

Corollary 5.2.7 If κ is an infinite cardinal and $| X _ { \alpha } | \le \kappa$ for all $\alpha < \kappa$ then $\begin{array} { r } { \left| \bigcup _ { \alpha < \kappa } X _ { \alpha } \right| \le \kappa } \end{array}$ 

## 5.2 Cardinal arithmetic

The proof is left as an exercise. 

Corollary 5.2.8 A finite union of finite sets is finite. 

The proof is similar to that of Corollary 5.2.6 (use Proposition 5.2.2). 

For a set A let $\begin{array} { r } { A ^ { < \omega } = \bigcup _ { n < \omega } A ^ { n } } \end{array}$ . Thus $A ^ { < \omega }$ is the set of all finite sequences with values in A. 

Corollary 5.2.9 If κ is an infinite cardinal, then $| \kappa ^ { < \omega } | = \kappa$ 

Proof It is easy to prove, by induction on $n < \omega$ , that $| \kappa ^ { n } | = \kappa$ for every $0 < n < \omega$ . So, by Corollary 5.2.7, 

$$
\kappa \leq \left| \kappa^ {<   \omega} \right| = \left| \bigcup_ {n <   \omega} \kappa^ {n} \right| \leq \kappa .
$$

Corollary 5.2.10 $| \mathbb { Q } | = | \mathbb { Z } | = \omega$ 

Proof Clearly $\omega = | \mathbb { N } | \leq | \mathbb { Z } | \leq | \mathbb { Q } |$ . To see that $| \mathbb { Q } | \leq \omega$ it is enough to show that $| \mathbb { Q } | \leq | 2 \times \omega \times \omega |$ , since $| 2 \times \omega \times \omega | = 2 \otimes \omega \otimes \omega = \omega .$ . So let $f \colon 2 \times \omega \times \omega  \mathbb { Q }$ be defined by $\begin{array} { r } { f ( i , m , n ) = ( - 1 ) ^ { i } \frac { m } { n + 1 } } \end{array}$ . It is easy to see that f is onto Q.  

Theorem 5.2.11 $| \mathbb { R } | = | 2 ^ { \omega } | = | \mathcal { P } ( \omega ) | = { \mathfrak { c } } .$ 

Proof $| 2 ^ { \omega } | = 2 ^ { \omega } = { \mathfrak { c } }$ by the definition of ${ \mathfrak { c . } } \ \left| 2 ^ { \omega } \right| = \left| { \mathcal { P } } ( \omega ) \right|$ was proved in (5.2). The equation $| \mathbb { R } | = | 2 ^ { \omega } |$ is proved by two inequalities. 

The first inequality $\left| 2 ^ { \omega } \right| \leq \left| \mathbb { R } \right|$ is established by a one-to-one function $f \colon 2 ^ { \omega }  \mathbb { R }$ defined by 

$$
f (\langle a _ {0}, a _ {1}, \dots \rangle) = \sum_ {n <   \omega} \frac {2 a _ {n}}{3 ^ {n + 1}}.
$$

(The range of f is Cantor’s classical “ternary” set; see Section 6.2.) 

To see that $| \mathbb { R } | \leq | 2 ^ { \omega } |$ define a one-to-one function $g \colon \mathbb { R } \to \mathcal { P } ( \mathbb { Q } )$ by $g ( r ) = \{ q \in \mathbb { Q } \colon q < r \} \ ( { \mathrm { i . e . , ~ } } g ( r )$ is the Dedekind cut associated with r). So 

$$
| \mathbb {R} | \leq | \mathcal {P} (\mathbb {Q}) | = \left| 2 ^ {\mathbb {Q}} \right| = 2 ^ {| \mathbb {Q} |} = 2 ^ {\omega}.
$$

Theorem 5.2.12 If λ and κ are cardinal numbers such that $\lambda \geq \omega$ and $2 \leq \kappa \leq \lambda$ then $\kappa ^ { \lambda } = 2 ^ { \lambda }$ 

In particular, $\lambda ^ { \lambda } = 2 ^ { \lambda }$ for every infinite cardinal number λ. 

Proof Notice that 

$$
2 ^ {\lambda} \subset \kappa^ {\lambda} \subset \lambda^ {\lambda} \subset \mathcal {P} (\lambda \times \lambda).
$$

Hence 

$$
2 ^ {\lambda} \leq \kappa^ {\lambda} \leq \lambda^ {\lambda} \leq | \mathcal {P} (\lambda \times \lambda) | = | 2 ^ {\lambda \times \lambda} | = 2 ^ {| \lambda \times \lambda |} = 2 ^ {\lambda}.
$$

Theorem 5.2.13 If κ, λ, and $\mu$  are cardinals, then 

$$
\kappa^ {\lambda \oplus \mu} = \kappa^ {\lambda} \otimes \kappa^ {\mu} \quad a n d \quad (\kappa^ {\lambda}) ^ {\mu} = \kappa^ {\lambda \otimes \mu}.
$$

Proof It follows immediately from the following properties: 

$$
A ^ {(B \cup C)} \approx (A ^ {B}) \times (A ^ {C}) \quad \text { for } B \cap C = \emptyset ,\tag{5.7}
$$

and 

$$
(A ^ {B}) ^ {C} \approx A ^ {B \times C}.\tag{5.8}
$$

Their proof is left as an exercise. 

For a set $X$ and a cardinal number κ define 

$$
[ X ] ^ {\leq \kappa} = \{A \in \mathcal {P} (X) \colon | A | \leq \kappa \}, [ X ] ^ {<   \kappa} = \{A \in \mathcal {P} (X) \colon | A | <   \kappa \},
$$

$$
[ X ] ^ {\kappa} = \{A \in \mathcal {P} (X) \colon | A | = \kappa \}.
$$

Proposition 5.2.14 For every infinite set X and nonzero cardinal $\kappa \leq | X |$ 

$$
\left| [ X ] ^ {\kappa} \right| = \left| [ X ] ^ {\leq \kappa} \right| = | X | ^ {\kappa}.
$$

Proof Define ψ : $X ^ { \kappa }  [ X ] ^ { \leq \kappa }$ by $\psi ( f ) = f [ \kappa ]$ . Since $\psi$ is clearly onto, and $[ X ] ^ { \kappa } \subset [ X ] ^ { \leq \kappa }$ , we have 

$$
\left| [ X ] ^ {\kappa} \right| \leq \left| [ X ] ^ {\leq \kappa} \right| \leq | X | ^ {\kappa}.
$$

 To finish the proof it is enough to show that $| X | ^ { \kappa } \leq | [ X ] ^ { \kappa } |$ 

To prove it define ψ : $X ^ { \kappa }  [ \kappa \times X ] ^ { \kappa }$ by $\psi ( f ) = f$ . Clearly $\psi$ is one-toone. Hence 

$$
\begin{array}{r c l} | X | ^ {\kappa} & = & | X ^ {\kappa} | \\ & \leq & | [ \kappa \times X ] ^ {\kappa} | \\ & = & | [ | \kappa \times X | ] ^ {\kappa} | \\ & = & | [ | X | ] ^ {\kappa} | \\ & = & | [ X ] ^ {\kappa} |  , \end{array}\tag{5.9}
$$

(5.10) 

where equations (5.9) and (5.10) follow from the fact that $| Y | = | Z |$ implies $| [ Y ] ^ { \kappa } | = | [ Z ] ^ { \kappa } |$ , which is left as an exercise.  

We will finish this section with the following important fact. 

Theorem 5.2.15 The family $\mathcal { C } ( \mathbb { R } ) = \{ f \in \mathbb { R } ^ { \mathbb { R } }$ : f is continuous} has cardinality continuum. 

Proof Define a function $R \colon { \mathcal { C } } ( \mathbb { R } ) \to \mathbb { R } ^ { \mathbb { Q } }$ by $R ( f ) = f | _ { \mathbb { Q } }$ . By the density of Q in R and the continuity of our functions it follows that R is one-to-one (see Section 3.3). Hence 

$$
| \mathcal {C} (\mathbb {R}) | \leq | \mathbb {R} ^ {\mathbb {Q}} | = | \mathbb {R} | ^ {| \mathbb {Q} |} = | 2 ^ {\omega} | ^ {\omega} = (2 ^ {\omega}) ^ {\omega} = 2 ^ {\omega \otimes \omega} = 2 ^ {\omega}.
$$

The other inequality is proved by a one-to-one function $c \colon \mathbb { R } \to { \mathcal { C } } ( \mathbb { R } )$ , where $c ( a ) \colon \mathbb { R } \to \mathbb { R }$ is a constant function with value a.  

## EXERCISES

1 Use the definitions of cardinal arithmetic operations and Theorem 5.1.8 to prove (5.3) and (5.4). 

2 Prove Proposition 5.2.2. Hint: Show by induction on n that $m + n < \omega$ and $m n < \omega$ . Then use Exercise 1 from Section 5.1. 

3 Prove that the relation $\preceq$ defined in the proof of Theorem 5.2.4 is a well-ordering relation on $\lambda \times \lambda$ 

4 Prove Corollary 5.2.7. 

5 Complete the proof of Theorem 5.2.13 by proving (5.7) and (5.8). 

6 Complete the proof of Proposition 5.2.14 by showing that $| Y | = | Z |$ implies $\lvert [ Y ] ^ { \kappa } \rvert = \lvert [ Z ] ^ { \kappa } \rvert$ for every sets Y and Z and any cardinal number κ. 

7 A real number r is an algebraic number if there is a polynomial $p ( x )$ with rational coeficients such that $p ( r ) = 0$ . Show that the set $A \subset$ R of all algebraic numbers is countable. Conclude that the set R \ A of all nonalgebraic real numbers has cardinality continuum. 

8 A function $f \colon  { \mathbb { R } } \ \to \  { \mathbb { R } }$ is a Baire class-one function if there exists a sequence $f _ { n } \colon  { \mathbb { R } } \to  { \mathbb { R } }$ of continuous functions such that $f _ { n }$ converges to f pointwise, that is, such that li $1 _ { n \to \infty } f _ { n } ( x ) = f ( x )$ for every $x \in \mathbb { R }$ . Find the cardinality of the family $\boldsymbol { B } _ { 1 }$ of all Baire class-one functions. 

## 5.3 Cofinality

We say that a subset A of an ordinal number α is unbounded in α if A has no strict upper bound in α, that is, when there is no $\gamma \in \alpha$ with $\xi < \gamma$ for all $\xi \in A$ . It is also easy to see that $A \subset \alpha$ is unbounded in α when $\alpha = \bigcup \{ \xi + 1 \colon \xi \in A \}$ or when 

$$
\forall \gamma <   \alpha \exists \xi \in A (\gamma \leq \xi).
$$

For an ordinal number α let $\operatorname { c f } ( \alpha )$ be the smallest ordinal number $\beta$ such that there exists a function $f \colon \beta  \alpha$ with the property that $f [ \beta ]$ is unbounded in $\alpha .$ Such a function f is called a cofinal map $( i n \alpha )$ . The number cf(α) is called the cofinality of α. Thus $f \colon \beta  \alpha$ is cofinal in α if 

$$
\forall \xi \in \alpha \exists \eta \in \beta (\xi \leq f (\eta))
$$

and 

$$
\operatorname{cf} (\alpha) = \min \{\beta \colon \text { there   is   a   cofinal   map } f \colon \beta \to \alpha \}.
$$

Notice that 

$$
\operatorname{cf} (\alpha) \leq \alpha \text { for   every   ordinal   number } \alpha ,
$$

since the identity map is a cofinal map. Also, 

$$
\operatorname{cf} (\alpha + 1) = 1 \text { for   every   ordinal   number } \alpha ,
$$

since $f \colon 1 \to \alpha + 1 , f ( 0 ) = \alpha$ , is cofinal in $\alpha + 1$ . It is also easy to see that if $\operatorname { c f } ( \alpha ) = 1$ then α has a greatest element. Thus cf $( \alpha ) = 1$ if and only if cf $( \alpha ) < \omega$ if and only if α is a successor ordinal. 

We will be interested mainly in cofinalities of limit ordinal numbers. 

Lemma 5.3.1 For every ordinal number α there is a strictly increasing cofinal map $f \colon \operatorname { c f } ( \alpha )  \alpha$ 

Proof For α a successor ordinal the map just shown works. 

If α is a limit ordinal and $g \colon \operatorname { c f } ( \alpha )  \alpha$ is a cofinal map, define by transfinite induction on $\eta < \operatorname { c f } ( \alpha )$ 

$$
f (\eta) = \max \left\{g (\eta), \bigcup_ {\xi <   \eta} (f (\xi) + 1) \right\}.
$$

Clearly $f ( \xi ) < f ( \xi ) + 1 \leq f ( \eta )$ for every $\xi < \eta < \operatorname { c f } ( \alpha )$ . Thus f is strictly increasing. 

## 5.3 Cofinality

The fact that 

$$
f (\eta) \in \alpha \text { for every } \eta <   \operatorname{cf} (\alpha)\tag{5.11}
$$

is proved by induction on $\eta < \operatorname { c f } ( \alpha )$ . If for some $\eta < \operatorname { c f } ( \alpha )$ condition (5.11) holds for all $\xi < \eta$ then $f ( \eta ) = \operatorname* { m a x } \{ g ( \eta ) , \bigcup _ { \xi < \eta } ( f ( \xi ) + 1 ) \} \le \alpha$ . But $f ( \eta )$ can’t be equal to α since otherwise the restriction of f to η would be a cofinal map in α and this would contradict the minimality of $\operatorname { c f } ( \alpha )$ . Thus $\eta < \operatorname { c f } ( \alpha )$ . Condition (5.11) has been proved. 

Finally, f is cofinal in α since for every $\xi \in \alpha$ there is an $\eta < \operatorname { c f } ( \alpha )$ with $\xi \le g ( \eta ) \le f ( \eta )$  

Corollary 5.3.2 cf $\left( \operatorname { c f } ( \alpha ) \right) = \operatorname { c f } ( \alpha )$ for every ordinal number $\alpha .$ 

Proof Let $f \colon \operatorname { c f } ( \operatorname { c f } ( \alpha ) )  \operatorname { c f } ( \alpha )$ and $g \colon \operatorname { c f } ( \alpha )  \alpha$ be strictly increasing cofinal maps. Then $g \circ f \colon \operatorname { c f } ( \operatorname { c f } ( \alpha ) )  \alpha$ is also cofinal, since for every $\xi < \alpha$ there exist $\eta \in \operatorname { c f } ( \alpha )$ with $\xi \le g ( \eta )$ and $\zeta \in \operatorname { c f } ( \operatorname { c f } ( \alpha ) )$ with $\eta \leq f ( \zeta )$ so 

$$
\xi \leq g (\eta) \leq g (f (\zeta)) = (g \circ f) (\zeta).
$$

Thus, by the minimality of cf(α), we have cf $\left( \operatorname { c f } ( \alpha ) \right) \geq \operatorname { c f } ( \alpha )$ . So cf $( \operatorname { c f } ( \alpha ) ) =$ cf(α).  

An ordinal number α is regular if it is a limit ordinal and $\operatorname { c f } ( \alpha ) = \alpha$ 

Theorem 5.3.3 If α is a regular ordinal number then α is a cardinal number. 

Proof $\mathrm { P u t } \ \beta = | \operatorname { c f } ( \alpha ) |$ , and choose a bijection $f \colon \beta \to \operatorname { c f } ( \alpha )$ and a cofinal function $g \colon \operatorname { c f } ( \alpha )  \alpha .$ . Then $( g \circ f ) \colon \beta \to \alpha$ is cofinal in α, since $( g \circ f ) [ \beta ] =$ $g [ f [ \beta ] ] = g [ \operatorname { c f } ( \alpha ) ]$ . Hence, by minimality of cf(α), cf $\displaystyle ( \alpha ) \leq \beta = \lvert \operatorname { c f } ( \alpha ) \rvert$ .  

Proposition 5.3.4 $\omega$ is regular. 

Proof It follows easily from Corollary 5.2.8. 

Theorem 5.3.5 $\kappa ^ { + }$ is regular for every infinite cardinal number $\kappa$ 

Proof Let $\alpha < \kappa ^ { + }$ and $f \colon \alpha  \kappa ^ { + }$ . Then $| \alpha | \le \kappa$ and $| f ( \xi ) | \le \kappa$ for every $\xi < \alpha$ . Hence $\begin{array} { r } { | \bigcup _ { \xi < \alpha } [ f ( \xi ) + 1 ] | \le \kappa } \end{array}$ since a union of $\le \kappa$ sets of cardinality $\le \kappa$ has cardinality $\le \kappa$ (see Corollary 5.2.7). Thus $\begin{array} { r } { \bigcup _ { \xi < \alpha } [ f ( \xi ) + 1 ] \ne \kappa ^ { + } } \end{array}$ , that is, cf $( \kappa ^ { + } ) \neq \alpha$ for every $\alpha < \kappa ^ { + }$ . So cf $\left( \kappa ^ { + } \right) = \kappa ^ { + }$  

One of the most useful properties of regular cardinals is given in the following proposition. 

Proposition 5.3.6 If λ is a regular cardinal, $A \subset \lambda$ , and $| A | < \lambda$ then there is an $\alpha < \lambda$ such that $A \subset \alpha$ 

Proof Let $\beta = \operatorname { O t p } ( A )$ and let $f \colon \beta \to A \subset \lambda$ be an order isomorphism. Notice that $\beta < \operatorname { c f } ( \lambda )$ , since $| \beta | = | A | < \lambda = \operatorname { c f } ( \lambda )$ . So the set $A = f [ \beta ]$ cannot be unbounded in λ. This implies the existence of an $\alpha < \lambda$ such that $\xi < \alpha$ for all $\xi \in A$ . Thus $A \subset \alpha$  

Another useful fact is the following. 

Proposition 5.3.7 If $\alpha < \omega _ { 1 }$ is a limit ordinal, then cf $( \alpha ) = \omega$ 

The proof is left as an exercise. 

We will finish this section with the following cardinal inequality. 

Theorem 5.3.8 For every infinite cardinal κ 

$$
\kappa^ {\operatorname{cf} (\kappa)} > \kappa .
$$

Proof Let $f \colon \operatorname { c f } ( \kappa )  \kappa$ be a cofinal map and let $G \colon \kappa \to \kappa ^ { \operatorname { c f } ( \kappa ) }$ . We will show that G is not onto $\kappa ^ { \mathrm { c f } ( \kappa ) }$ 

Define h: cf $( \kappa ) \to \kappa$ by 

$$
h (\alpha) = \min (\kappa \setminus \{G (\xi) (\alpha): \xi <   f (\alpha) \})
$$

for $\alpha < \operatorname { c f } ( \kappa )$ . Such a definition makes sense, since $| \{ G ( \xi ) ( \alpha ) \colon \xi < f ( \alpha ) \} | \le$ $| f ( \alpha ) | < \kappa$ . But for every $\xi ~ < ~ \kappa$ there exists an $\alpha ~ < \operatorname { c f } ( \kappa )$ such that $\xi < f ( \alpha )$ , that is, such that $h ( \alpha ) \neq G ( \xi ) ( \alpha )$ . Hence $h \neq G ( \xi )$ for every $\xi < \kappa$ and $h \not \in G [ \kappa ]$  

Corollary 5.3.9 cf $( { \mathfrak { c } } ) > \omega$ 

Proof Assume, to obtain a contradiction, that c $\mathbf { \bar { \rho } } ( \mathbf { c } ) = { \boldsymbol { \omega } }$ . Then ${ \mathfrak { c } } ^ { \mathrm { c f } ( \mathfrak { c } ) } =$ $( 2 ^ { \omega } ) ^ { \omega } = 2 ^ { \omega } = { \mathfrak { c } }$ , contradicting Theorem 5.3.8.  

## EXERCISE

1 Prove Proposition 5.3.7. 

Part III 

# The power of recursive definitions

## Subsets of R<sup>n</sup>

## 6.1 Strange subsets of $\mathbb { R } ^ { n }$ and the diagonalization argument

In this section we will illustrate some typical constructions by transfinite induction. We will do so by constructing recursively some subsets of $\mathbb { R } ^ { n }$ with strange geometric properties. The choice of geometric descriptions of these sets is not completely arbitrary here – we still have not developed the basic facts concerning “nice” subsets of $\mathbb { R } ^ { n }$ that are necessary for most of our applications. This will be done in the remaining sections of this chapter. 

To state the next theorem, we will need the following notation. For a subset A of the plane $\mathbb { R } ^ { 2 }$ the horizontal section of A generated by $y \in \mathbb { R }$ (or, more precisely, its projection onto the first coordinate) will be denoted by $A ^ { y }$ and defined as $A ^ { y } = \{ x \in \mathbb { R } \colon \langle x , y \rangle \in A \}$ . The vertical section of A generated by $x \in \mathbb { R }$ is defined by $A _ { x } = \{ y \in \mathbb { R } \colon \langle x , y \rangle \in A \}$ 

We will start with the following example. 

Theorem 6.1.1 There exists a subset A of the plane with every horizontal section $A ^ { y }$ being dense in R and with every vertical section $A _ { x }$ having precisely one element. 

Proof We will define the desired set by induction. To do so, we will first reduce our problem to the form that is most appropriate for a recursive construction. 

The requirement that every horizontal section of A is dense in R tells us that A is “reasonably big.” More precisely, the condition says that $A ^ { y } \cap ( a , b ) \neq \emptyset$ for every $a \ < \ b$ and $y \in \mathbb { R }$ . Therefore if we put ${ \mathcal { F } } =$ $\{ ( a , b ) \times \{ y \} \colon a , b , y \in \mathbb { R } \ \& \ a < b \}$ then we can restate it as 

$$
A \cap J \neq \emptyset \quad \text {   for   every   } J \in \mathcal {F}.\tag{6.1}
$$

The requirement that every vertical section of A has precisely one point tells us that A is “reasonably small.” It can be restated as 

$$
\left| A \cap [ \{x \} \times \mathbb {R} ] \right| = 1 \quad \text { for   every } x \in \mathbb {R}.\tag{6.2}
$$

The idea of constructing $A$ is to “grow it bit by bit” to obtain at the end a set satisfying (6.1), while keeping approximations “reasonably small.” More precisely, by transfinite induction on $\xi < { \mathfrak { c } }$ , we will define a sequence $\langle \langle x _ { \xi } , y _ { \xi } \rangle : \xi < { \mathfrak { c } } \rangle$ such that $A _ { 0 } = \{ \langle x _ { \xi } , y _ { \xi } \rangle \colon \xi < \mathfrak { c } \}$ satisfies (6.1) and has the property that $| A _ { 0 } \cap [ \{ x \} \times \mathbb { R } ] | \leq 1$ for every $x \in \mathbb { R }$ . It is enough, since then the set $A = A _ { 0 } \cup \{ \langle x , 0 \rangle \colon A _ { 0 } \cap [ \{ x \} \times \mathbb { R } ] = \emptyset \}$ satisfies the theorem. 

To describe our construction of the sequence, notice first that $| { \mathcal { F } } | = { \mathfrak { c } } ,$ since ${ \mathfrak { c } } = | \mathbb { R } | \leq | { \mathcal { F } } | \leq | \mathbb { R } ^ { 3 } | = { \mathfrak { c } }$ . Let $\{ J _ { \xi } \colon \xi < \mathfrak { c } \}$ be an enumeration of the family ${ \mathcal F }$ . If for some $\xi < { \mathfrak { c } }$ the sequence $\langle \langle x _ { \zeta } , y _ { \zeta } \rangle \colon \zeta < \xi \rangle$ is already defined, choose 

$$
\left\langle x _ {\xi}, y _ {\xi} \right\rangle \in J _ {\xi} \setminus \left[ \bigcup_ {\zeta <   \xi} \left\{x _ {\zeta} \right\} \times \mathbb {R} \right].\tag{6.3}
$$

The choice can be made, since for every $\xi < { \mathfrak { c } }$ we have $| J _ { \xi } | = | \mathbb { R } | = { \mathfrak { c } } >$ $\begin{array} { r } { | \xi | \ge \left| J _ { \xi } \cap \left[ \bigcup _ { \zeta < \xi } \{ x _ { \zeta } \} \times \mathbb { R } \right] \right| } \end{array}$ . So, by the recursion theorem, the sequence $\langle \langle x _ { \xi } , \dot { y _ { \xi } } \rangle : \xi \bar { < } \mathfrak { c } \rangle$ exists. (More precisely, we define $\langle x _ { \xi } , y _ { \xi } \rangle = f ( \xi ) = h ( f | _ { \xi } )$ where the oracle function h is defined implicitly by formula $\left( 6 . 3 \right)$ . Explicitly, $h ( \langle \langle x _ { \zeta } , y _ { \zeta } \rangle \colon \zeta < \xi \rangle )$ is defined as $C ( J _ { \xi } \setminus \{ \langle x _ { \zeta } , y _ { \zeta } \rangle \colon \zeta < \xi \} )$ , where C is a choice function from the family ${ \mathcal { P } } ( \mathbb { R } ^ { 2 } ) { \backslash } \{ \emptyset \} . ) \qquad $ 

It is clear that $A _ { 0 } = \{ \langle x _ { \xi } , y _ { \xi } \rangle \colon \xi < \mathfrak { c } \}$ satisfies (6.1), since for every $J \in { \mathcal { F } }$ there exists a $\xi < { \mathfrak { c } }$ such that $J = J _ { \xi }$ and $\langle x _ { \xi } , y _ { \xi } \rangle \in A _ { 0 } \cap J _ { \xi } = A _ { 0 } \cap J ,$ It is also easy to see that the choice as in (6.3) implies that every vertical section of $A _ { 0 }$ has at most one point.  

The proof of Theorem 6.1.1 is a typical example of a diagonalization technique. In order to prove the theorem we had to find for every $J \in { \mathcal { F } }$ a point $\langle x _ { J } , y _ { J } \rangle \in J$ that would belong to a future set A. The choice was supposed to be done while preserving at every step the property that no two points chosen so far belong to the same vertical line. In order to prove the theorem we listed all elements of $\mathcal { F }$ and made our construction, taking care of each of its elements one at a time, using the fact that we still had “enough room” to make our choice. This technique of making inductive constructions by listing all important objects for the desired property and then taking care of each of them one at a time is called the diagonalization technique. It is typical for such constructions that the inductive step is possible because of some cardinal argument similar to the one given earlier. The preservation part, like that mentioned before, is usually the hard part of the argument. 

The next theorem, due to Mazurkiewicz (1914), is very similar in character to Theorem 6.1.1. 

Theorem 6.1.2 There exists a subset A of the plane $\mathbb { R } ^ { 2 }$ that intersects every straight line in exactly two points. 

Proof Let $\{ L _ { \xi } \colon \xi ~ < ~ \mathfrak { c } \}$ be an enumeration of all straight lines in the plane $\mathbb { R } ^ { 2 }$ . By transfinite induction on $\xi < { \mathfrak { c } }$ we will construct a sequence $\{ A _ { \xi } \colon \xi < \mathfrak { c } \}$ of subsets of $\mathbb { R } ^ { 2 }$ such that for every $\xi < { \mathfrak { c } }$ 

(I) $A _ { \xi }$ has at most two points; 

(P) $\cup _ { \zeta \leq \xi } A _ { \zeta }$ does not have three collinear points; 

(D) $\cup _ { \zeta \leq \xi } A _ { \zeta }$ contains precisely two points of $L _ { \xi }$ . 

Then the set $A = \textstyle \bigcup _ { \xi < \mathfrak { c } } A _ { \xi }$ will have the desired property. This is the case since the preservation condition (P) implies that every line contains at most two points of $A$ , while the diagonal condition (D) makes sure that every line $L$ contains at least two points from $A$ . Thus, it is enough to show that we can choose a set $A _ { \xi }$ satisfying (I), (P), and (D) for every $\xi < { \mathfrak { c } }$ This will be proved by induction on $\xi < { \mathfrak { c } }$ 

So assume that for some $\xi < { \mathfrak { c } }$ the sequence $\{ A _ { \zeta } \colon \zeta < \xi \}$ is already constructed. By condition (I) the set $B = \textstyle \bigcup _ { \zeta < \xi } A _ { \zeta }$ has cardinality $< { \mathfrak { c } } .$ being a union of $| \xi | < { \mathfrak { c } }$ many finite sets. Similarly, the family $\mathcal { G }$ of all lines containing two points from B has cardinality $\le | B ^ { 2 } | < { \mathfrak { c } }$ . Notice that by the inductive assumption (P) the set $B \cap L _ { \xi }$ has at most two points. If it has precisely two points put $A _ { \xi } = \varnothing$ and notice that (P) and (D) are satisfied. If $B \cap L _ { \xi }$ contains less than two points then $L _ { \xi }$ intersects every line from $\mathcal { G }$ in at most one point. Thus $L _ { \xi } \cap \bigcup \mathcal { G } = \bigcup _ { L \in \mathcal { G } } L _ { \xi } \cap L$ has at most $| \mathcal { G } | < \mathfrak { c }$ many points. 

Choose $A _ { \xi } \subset L _ { \xi } \setminus \cup \mathcal { G }$ to have two elements if $B \cap L _ { \xi } = \varnothing$ and to have one element if $B \cap L _ { \xi }$ has one point. It is easy to see that conditions (P) and (D) are satisfied with either choice of $A _ { \xi }$ . The construction has now been completed.  

The next theorem is yet another example of a geometric problem solved with help of the recursion theorem. In this theorem a circle in $\mathbb { R } ^ { 3 }$ is understood to be a set of points forming any nontrivial circle in any plane in $\mathbb { R } ^ { 3 }$ 

Theorem 6.1.3 $\mathbb { R } ^ { 3 }$ is a union of disjoint circles. 

Proof We have to construct a family $\mathcal { C }$ of subsets of $\mathbb { R } ^ { 3 }$ such that (1) each $C \in { \mathcal { C } }$ is a circle, (2) the family C covers $\mathbb { R } ^ { 3 }$ , and (3) diferent elements of $\mathcal { C }$ are disjoint. We will construct the family C as $\{ C _ { \xi } \colon \xi < \mathfrak { c } \}$ by induction on $\xi \ < \ \mathfrak { c }$ For this, the natural approach is the following. Choose an enumeration $\{ p \xi : \xi < { \mathfrak { c } } \}$ of $\mathbb { R } ^ { 3 }$ , and for each $p _ { \xi }$ choose a circle $C _ { \xi }$ such that $p _ { \xi } \in C _ { \xi }$ . This certainly would take care of (2); however, then we could not keep circles disjoint: For $p _ { \xi } \in C _ { 0 } \setminus \{ p _ { 0 } \}$ the circles $C _ { 0 }$ and $C _ { \xi }$ would not be disjoint. Thus we have to settle for a slightly weaker condition: We will choose $C _ { \xi }$ such that 

$$
\mathrm{(D)} \quad p _ {\xi} \in \bigcup_ {\zeta \leq \xi} C _ {\zeta}.
$$

This is the “diagonal” condition that will imply that C covers $\mathbb { R } ^ { 3 }$ . However, we have to make the choice in such a way that circles in $\mathcal { C }$ are pairwise disjoint. We will do this by assuming that for each $\xi ~ < ~ { \mathfrak { c } }$ the circles constructed so far are pairwise disjoint and we will choose $C _ { \xi }$ preserving this property. More precisely, we will choose $C _ { \xi }$ such that the following “preservation” condition is satisfied: 

$$
\text {(P)} \quad C _ {\xi} \cap \bigcup_ {\zeta <   \xi} C _ {\zeta} = \emptyset .
$$

Evidently, if we could construct $C = \{ C _ { \xi } \colon \xi < \mathfrak { c } \}$ such that conditions (D) and (P) are satisfied for every $\xi < { \mathfrak { c } }$ , then C would be the desired family of circles. 

On the other hand, the recursion theorem tells us that we can find such a sequence $\langle C _ { \xi } \colon \xi < { \mathfrak { c } } \rangle$ as long as the family of all circles $C _ { \xi }$ satisfying (D) and (P) is nonempty for every $\xi < { \mathfrak { c } }$ . (Since then the choice function will work as an oracle function.) 

So assume that for some $\xi < { \mathfrak { c } }$ the sequence $\{ C _ { \zeta } \colon \zeta < \xi \}$ is already constructed satisfying (D) and (P). We will prove that there exists a circle $C _ { \xi }$ satisfying (D) and (P). 

If $p _ { \xi } \notin \bigcup _ { \zeta < \xi } C _ { \zeta }$ define $p = p _ { \xi }$ Otherwise, choose an arbitrary point $p \in \mathbb { R } ^ { 3 } \backslash \cup _ { \zeta < \xi } C _ { \zeta }$ . This can be done since for every straight line $L$ in $\mathbb { R } ^ { 3 }$ the set $L \cap \cup _ { \zeta < \xi } \mathbf { \vec { C } } _ { \zeta } = \cup _ { \zeta < \xi } ( L \cap C _ { \zeta } )$ has cardinality less than continuum, being  a union of less than continuum many finite sets $L \cap C _ { \zeta }$ . We will choose $C _ { \xi }$ containing $p$ and satisfying (P). To do this, take a plane $P$ containing $p$ that does not contain any of the circles $C _ { \zeta }$ for $\zeta < \xi$ . This can be done since there are continuum many planes passing through $p$ and there are only $\le \left| \xi \right| < { \mathfrak { c } }$ many planes containing circles from $\{ C _ { \zeta } \colon \zeta < \xi \}$ . Now notice that the plane $P$ intersects each circle $C _ { \zeta }$ in at most two points. Thus the set $S = P \cap \bigcup _ { \zeta < \xi } C _ { \zeta }$ has cardinality less than continuum. Fix a line $L$ in $P$ containing $p$ and let $\mathcal { C } _ { 0 }$ be the family of all circles in $P$ containing $p$ and tangent to L. Notice that diferent circles from $\mathcal { C } _ { 0 }$ intersect only at the point $p .$ . Thus there is a circle $C _ { \xi } \in \mathcal { C } _ { 0 }$ disjoint from $S .$ . This finishes the inductive construction and the proof.  

If in the previous three theorems the reader got the impression that we can construct a subset or a partition of $\mathbb { R } ^ { n }$ with almost arbitrary paradoxical geometric properties, the next theorem will prove that this impression is wrong. 

## Theorem 6.1.4 The plane $\mathbb { R } ^ { 2 }$ is not a union of disjoint circles.

Proof Assume, to obtain a contradiction, that there is a family $\mathcal { F }$ of disjoint circles in $\mathbb { R } ^ { 2 }$ such that $\mathbb { R } ^ { 2 } = \bigcup \mathcal { F }$ . Construct, by induction on $n < \omega$ , a sequence $\{ C _ { n } \colon n \prec \omega \}$ of circles from $\mathcal { F }$ in the following way: Start with an arbitrary circle $C _ { 0 } \in \mathcal { F }$ and in step $n + 1$ choose a circle $C _ { n + 1 } \in \mathcal { F }$ that contains the center $c _ { n }$ of circle $C _ { n }$ 

Notice that if $r _ { n }$ is the radius of $C _ { n }$ then $| c _ { n + 1 } - c _ { n } | = r _ { n + 1 } < r _ { n } / 2$ Thus $\langle c _ { n } : n ~ < ~ \omega \rangle$ is a Cauchy sequence. Let $p = \operatorname* { l i m } _ { n \to \infty } c _ { n }$ . Then p belongs to the closed disk $D _ { n }$ bounded by $C _ { n }$ for every $n < \omega$ . So $p$ cannot belong to any circle $C _ { n }$ since it belongs to $D _ { n + 1 }$ , which is disjoint from $C _ { n }$ 

Now let $C \in { \mathcal { F } }$ be such that $p \in C$ . Then $C \neq C _ { n }$ for every $n < \omega$ . But if $n < \omega$ is such that $r _ { n }$ is smaller than the radius of $C$ then $C \cap C _ { n } \neq \emptyset$ This contradicts the choice of $\mathcal { F }$ .  

The next theorem shows that a simple diagonalization may lead to messy multiple-case considerations. In the theorem $\mathbb { R } ^ { 2 }$ will be considered as a vector space. In particular, $A + r$ will stand for the algebraic sum of a set $A \subset \mathbb { R } ^ { 2 }$ and $r \in \mathbb { R } ^ { 2 }$ , that is, $A + r = \{ a + r \colon a \in A \}$ 

Theorem 6.1.5 There is a subset A of $\mathbb { R } ^ { 2 }$ that intersects every one of its translations in a singleton, that is, such that the set $( A { + } r ) \cap A$ has precisely one element for every $r \in \mathbb { R } ^ { 2 } , r \neq 0$ 

Proof Enumerate $\mathbb { R } ^ { 2 } \setminus \{ 0 \}$ as $\{ r _ { \xi } \colon \xi < \mathfrak { c } \}$ . We will define, by induction on $\xi < { \mathfrak { c } }$ , the sequences $\langle a _ { \xi } \in \mathbb { R } ^ { 2 } \colon \bar { \xi } < \mathfrak { c } \rangle , \ : \langle \bar { b } _ { \xi } \in \mathbb { R } ^ { 2 } \colon \xi < \mathfrak { c } \rangle$ , and $\langle A _ { \xi } \colon \xi < { \mathfrak { c } } \rangle$ such that for every $\xi < { \mathfrak { c } }$ 

(I) $A _ { \xi } = \{ a _ { \zeta } \colon \zeta \leq \xi \} \cup \{ b _ { \zeta } \colon \zeta \leq \xi \} ;$ 

(D) $b _ { \xi } - a _ { \xi } = r _ { \xi } { : }$ 

(P) if $a , b , a ^ { \prime } , b ^ { \prime } \in A _ { \xi }$ are such that $b - a = b ^ { \prime } - a ^ { \prime } \neq 0$ then $a = a ^ { \prime }$ and $b = b ^ { \prime } .$ 

Before we describe the construction notice that $A = \textstyle \bigcup _ { \xi < \mathfrak { c } } A _ { \xi }$ has the desired properties: $( A + r ) \cap A$ has at least one element by the “diagonal” 

condition (D) for $r = r _ { \xi }$ , since $b _ { \xi } \in ( A + r _ { \xi } ) \cap A$ ; it has at most one element by the “preservation” condition (P), where we take $r = b - a = b ^ { \prime } - a ^ { \prime }$ 

To make an inductive step assume that for some $\xi < { \mathfrak { c } }$ the sequences are already constructed. The dificulty will be to find points $a _ { \xi }$ and $b _ { \xi }$ satisfying (D) while preserving (P). 

Let $\textstyle B = \bigcup _ { \zeta < \xi } A _ { \zeta }$ . Notice that B satisfies (P). 

If $B \cap ( B + r _ { \xi } ) \neq \varnothing$ and $b \in B \cap ( B + r _ { \xi } )$ then $a = b - r _ { \xi } \in B$ and we can define $a _ { \xi } = a$ and $b _ { \xi } = b$ . Condition (D) is satisfied by the choice of $a$ and b, and condition (P) holds, since $A _ { \xi } = B$ 

So assume that $B \cap ( B + r _ { \xi } ) = \varnothing$ and notice that if we find $a _ { \xi } = x$ then $b _ { \xi } = a _ { \xi } + r _ { \xi } = x + r _ { \xi }$ would be uniquely defined. Thus, it is enough to find x guaranteeing satisfaction of (P). In order to find it we have to avoid the situation 

$$
b - a = b ^ {\prime} - a ^ {\prime} \neq 0 \text { and } b \neq b ^ {\prime},\tag{6.4}
$$

where $a , b , a ^ { \prime } , b ^ { \prime } \in A _ { \xi } = B \cup \{ x , x + r _ { \xi } \}$ . So take $x , a , b , a ^ { \prime } , b ^ { \prime }$ that satisfy (6.4). 

There are several cases to consider. First notice that by our inductive hypothesis $\{ a , b , a ^ { \prime } , b ^ { \prime } \} \cap \{ x , x + r _ { \xi } \} \neq \emptyset .$ 

In the first group of cases we assume that all elements $a , b , a ^ { \prime } , b ^ { \prime }$ are diferent. Then there are the following possibilities: 

$\{ a , b , a ^ { \prime } , b ^ { \prime } \} \cap \{ x , x + r _ { \xi } \} = \{ x \}$ . Then $x = c + d - e$ for some $c , d , e \in$ B. To avoid this situation it is enough to take x outside the set $S _ { 1 } =$ $\{ c + d - e \colon c , d , e \in B \}$ 

$\{ a , b , a ^ { \prime } , b ^ { \prime } \} \cap \{ x , x + r _ { \xi } \} = \{ x + r _ { \xi } \}$ . Then $x = c + d - e - r _ { \xi }$ for some $c , d , e \in B$ . To avoid this situation it is enough to take x outside the set $S _ { 2 } = \{ c + d - e - r _ { \xi } \colon c , d , e \in B \}$ 

• {a, b, a<sup>-</sup>, b<sup>-</sup>} ∩ {x, x + r<sub>ξ</sub>} = {x, x + r<sub>ξ</sub>}. 

If $\{ a , b \} = \{ x , x + r _ { \xi } \}$ then $\pm r _ { \xi } = b ^ { \prime } - a ^ { \prime }$ . However, this would contradict the fact that $B \cap ( B + r _ { \xi } ) = \varnothing$ . Similarly $\{ x , x + r _ { \xi } \}$ cannot be equal to $\{ a ^ { \prime } , b ^ { \prime } \} , \{ a , a ^ { \prime } \} , \mathrm { o r } \{ b , \bar { b ^ { \prime } } \}$ 

If $\{ x , x + r _ { \xi } \} = \{ a , b ^ { \prime } \}$ or $\{ x , x + r _ { \xi } \} = \{ a ^ { \prime } , b \}$ then $2 x = c + d - r _ { \xi }$ for some $c , d \in B$ . To avoid this situation it is enough to take x outside the set $S _ { 3 } = \{ ( c + d - r _ { \xi } ) / 2 \colon c , d \in B \}$ 

The second group of cases consists of the situations in which some of the elements $a , b , a ^ { \prime } , b ^ { \prime }$ are equal to each other. It is easy to see that there are only two possibilities for such equations: $b = a ^ { \prime }$ and $a = b ^ { \prime }$ . Moreover, these equations cannot happen at the same time. Thus assume that $\boldsymbol { a } ^ { \prime } = \boldsymbol { b }$ and that the other elements are diferent (the case when $a = b ^ { \prime }$ is identical). Then $2 b = a + b ^ { \prime }$ 

All the cases when $b \ \notin \ \{ x , x + r _ { \xi } \}$ are identical to those previously considered. So assume that $b \in \{ x , x + r _ { \xi } \}$ . Then there are the following possibilities: 

$b = x$ . Then $2 x = a + b ^ { \prime }$ 

If $x + r _ { \xi } \notin \{ a , b ^ { \prime } \}$ then $2 x = c + d$ for some $c , d \in B$ . To avoid this case it is enough to take x outside the set $S _ { 4 } = \{ ( c + d ) / 2 \colon c , d \in B \}$ 

If $x + r _ { \xi } \in \{ a , b ^ { \prime } \}$ then $2 x = c + x + r _ { \xi }$ for some $c \in B$ . To avoid this situation it is enough to take x outside the set $S _ { 5 } = \{ c + r _ { \xi } \colon c \in B \}$ 

$b = x + r _ { \xi }$ . Then $2 x = a + b ^ { \prime } - 2 r _ { \xi }$ 

If $x \notin \{ a , b ^ { \prime } \}$ then $2 x = c + d - 2 r _ { \xi }$ for some points $c , d \in B$ . To avoid this particular situation it is enough to choose x outside the set $S _ { 6 } = \{ ( c + d - 2 r _ { \xi } ) / 2 \colon c , d \in B \}$ 

If $x \in \{ a , b ^ { \prime } \}$ then $2 x = c + x - 2 r _ { \xi }$ for some $c \in B$ . To avoid this case it is enough to take x outside the set $S _ { 7 } = \{ c - 2 r _ { \xi } \colon c \in B \}$ 

It is easy to see that each of the sets $S _ { i }$ for $i = 1 , . . . , 7$ has cardinality $\leq | \xi | ^ { 3 } < { \mathfrak { c } }$ . Thus we can take x from the set $\textstyle \mathbb { R } ^ { 2 } \setminus \bigcup _ { i = 1 } ^ { 7 } S _ { i }$  

In all of the previous examples of this section we used preservation conditions of finite character such as noncollinearity, finite intersections of diferent circles, and so forth. This made obvious the fact that these conditions were preserved when we took a union of previously constructed sets. This approach, however, does not always work. For example, the next theorem will state that $\mathbb { R } ^ { 2 }$ is a union of countably many sets $S _ { i }$ such that no set $S _ { i }$ contains two diferent points of rational distance apart. If we try to prove this theorem starting with an arbitrary well ordering $\{ p \xi : \xi < \mathfrak { c } \}$ of $\mathbb { R } ^ { 2 }$ and at step $\xi$ try to add the point $p _ { \xi }$ to some set $S _ { i }$ , then already at step $\omega$ we might find ourselves in trouble – it might happen that for every $i < \omega$ there is already an element $p _ { n } \in S _ { i } , n < \omega$ , of rational distance from $p _ { \omega }$ . If so, we could not assign $p _ { \omega }$ to any $S _ { i }$ . To solve these dificulties we will proceed in a diferent manner, to be described subsequently. 

We will start with the following easy but very useful lemma that will also be used very often in the rest of this text. To state it, we need the following definitions. Let $F \colon X ^ { k } \to [ X ] ^ { \leq \omega }$ for some $k < \omega$ . We say that a subset $Y$ of X is closed under the action of F if $F ( y _ { 1 } , . . . , y _ { k } ) \subset Y$ for every $y _ { 1 } , . . . , y _ { k } \in Y$ . If $f \colon X ^ { k } \to X$ then $Y \subset X$ is closed under the action of f if it is closed under the action of $F$ , where $F ( x ) = \{ f ( x ) \}$ . Finally, if $\mathcal { F }$ is a family of functions from finite powers of X into either $[ X ] ^ { \leq \omega }$ or X then $Y \subset X$ is closed under the action of $\mathcal { F }$ if it is closed under the action of F for every $F \in { \mathcal { F } }$ 

Lemma 6.1.6 Let $\mathcal { F }$ be an at most countable family of functions from finite powers of X into $[ X ] ^ { \leq \omega }$ or X. Then 

(a) for every $Z \subset X$ there exists a smallest subset $Y$ of $X$ closed under the action of F and containing $Z _ { i }$ ; this set, denoted by $\operatorname { c l } _ { \mathcal { F } } ( Z )$ , has cardinality less than or equal to $| Z | + \omega ;$ in particular, $| \mathrm { c l } _ { \mathcal { F } } ( Z ) | = | Z |$ for every infinite $Z _ { i }$ ; 

(b) $i f \left| X \right| = \kappa > \omega$ then there exists an increasing sequence $\langle X _ { \alpha } \colon \alpha < \kappa \rangle$ $o f$ subsets of X closed under the action $o f \mathcal { F }$ such that $\begin{array} { r } { X = \bigcup _ { \alpha < \kappa } X _ { \alpha } , } \end{array}$ $| X _ { \alpha } | < \kappa$ for all $\alpha < \kappa$ , and $\textstyle X _ { \lambda } = \bigcup _ { \alpha < \lambda } X _ { \alpha }$ for every limit ordinal $\lambda < \kappa$ 

Proof In the proof we will identify functions $f \colon X \to X$ from $\mathcal { F }$ with $F \colon X \to [ X ] ^ { 1 } , F ( x ) = \{ f ( x ) \}$ 

(a) Let $\mu = | Z | + \omega . \mathrm { ~ C ~ }$ onstruct, by induction on $n < \omega$ , an increasing sequence $\langle Z _ { n } \in [ X ] ^ { \mu } : n < \omega \rangle$ by putting $Z _ { 0 } = Z$ and defining $Z _ { n + 1 }$ as 

$$
Z _ {n} \cup \bigcup \left\{F \left(z _ {1}, \dots , z _ {m}\right): F \in \mathcal {F} \& \text {dom} F = X ^ {m} \& \left\langle z _ {1}, \dots , z _ {m} \right\rangle \in Z _ {n} ^ {m} \right\}.
$$

Notice that $| Z _ { n + 1 } | \leq \mu .$ . This is the case since $\left| Z _ { n } \right| \le \mu$ and the second set is a union of a family of sets of cardinality $\leq \omega$ indexed by a set of cardinality $\leq | \mathcal { F } | \otimes | Z _ { n } | ^ { < \omega } \leq \mu$ 

Define c $\begin{array} { r } { { 1 } _ { \mathcal { F } } ( Z ) = { \bigcup _ { n < \omega } Z _ { n } } } \end{array}$ . Obviously $Z \subset \mathrm { c l } _ { \mathcal { F } } ( Z ) \subset X$ and $| \mathrm { c l } _ { \mathcal { F } } ( Z ) | \le$ $\mu ,$ as $\mathrm { c l } _ { \mathcal F } ( Z )$ is a union of countably many sets of cardinality at most $\mu .$ To see that $\mathrm { c l } _ { \mathcal F } ( Z )$ is closed under the action of $\mathcal { F }$ take $F \in { \mathcal { F } }$ . If $X ^ { m }$ is the domain of F and $z _ { 1 } , \dotsc , z _ { m } \in \mathrm { c l } _ { \mathcal { F } } ( Z )$ then there is an $n < \omega$ such that $z _ { 1 } , \ldots , z _ { m } \in Z _ { n }$ , and so $F ( z _ { 1 } , \ldots , z _ { m } ) \subset Z _ { n + 1 } \subset \mathrm { c l } _ { \mathcal { F } } ( Z )$ 

In order to prove that $\operatorname { c l } _ { \mathcal { F } } ( Z )$ is the smallest subset of X closed under the action of $\mathcal { F }$ and containing $Z$ let Y be another such set. Then $Z _ { 0 } = Z \subset Y$ and by an easy induction we can prove that $Z _ { n } \subset Y$ for every $n < \omega$ . So $\begin{array} { r } { \operatorname { c l } _ { \mathcal { F } } ( Z ) = \bigcup _ { n < \omega } Z _ { n } \subset Y } \end{array}$ 

(b) Enumerate X as $\{ x \varepsilon \colon \xi < \kappa \}$ and define $X _ { \alpha } = \mathrm { c l } _ { \mathcal { F } } ( \{ x _ { \xi } \colon \xi < \alpha \} )$ Then the equation $\textstyle X = \bigcup _ { \alpha < \kappa } X _ { \alpha }$ is obvious and $| X _ { \alpha } | \leq | \alpha | + \omega < \kappa$ for $\alpha < \kappa$ follows immediately from (a). The two other conditions are simple consequences of the fact that $\mathrm { c l } _ { \mathcal F } ( Z )$ is the smallest subset of X containing $Z$ and being closed under the action of $\mathcal { F }$  

The next theorem is due to Erd˝os and Hajnal (Erd˝os 1969). 

Theorem 6.1.7 There is a countable partition $\{ S _ { i } \colon i < \omega \}$ of $\mathbb { R } ^ { 2 }$ such that the distance between any two diferent points of the same set $S _ { i }$ is irrational. 

Proof By induction on $\kappa = | X |$ we are going to prove that every set $X \subset \mathbb { R } ^ { 2 }$ can be decomposed as described in the theorem. 

So let $X \subset \mathbb { R } ^ { 2 }$ be such that $| X | = \kappa$ and suppose that the foregoing statement is true for every $Y \subset \mathbb { R } ^ { 2 }$ of cardinality $< \kappa$ . We have to prove the statement for $X$ 

If $\kappa \leq \omega$ then the statement is obvious, since we can put every element of X in a diferent set $S _ { i }$ . So assume $\kappa > \omega$ 

For every $p , q \in \mathbb { Q }$ define $F _ { p q } : ( \mathbb { R } ^ { 2 } ) ^ { 2 }  [ \mathbb { R } ^ { 2 } ] ^ { < \omega }$ by 

$$
F _ {p q} (x, y) = \{z \in \mathbb {R} ^ {2} \colon | x - z | = p \& | y - z | = q \}.
$$

Notice that indeed $F _ { p q } ( x , y ) \in [ \mathbb { R } ^ { 2 } ] ^ { < \omega }$ since it has at most two points. Let $\mathcal { F } = \{ F _ { p q } : p , q \in \bar { \mathbb { Q } } \}$ and let $\begin{array} { r } { X = \bigcup _ { \alpha < \kappa } X _ { \alpha } , } \end{array}$ where $\langle X _ { \alpha } \colon \alpha \ < \ \kappa \rangle$ is a sequence of subsets closed under the action of $\mathcal { F }$ as in Lemma $6 . 1 . 6 ( \mathrm { b } )$ 

We will define a decomposition of X into sets $S _ { i }$ by defining $g \colon X \to \omega$ and $S _ { i } = g ^ { - 1 } ( i )$ . (Thus the function g tells us that an element $x \in X$ is put into $S _ { g ( x ) } . )$ The function $g$ must have the property that 

$$
\text { if } g (x) = g (y) \text { for   different } x, y \in X \text { then } | x - y | \not \in \mathbb {Q}.\tag{6.5}
$$

We will define the function g inductively on the sets $X _ { \alpha }$ for $\alpha < \kappa$ 

Assume that for some $\beta < \kappa$ the function $g$ is already defined on each $X _ { \alpha }$ for all $\alpha < \beta$ . If $\beta$ is a limit ordinal, then $g$ is already defined on $\begin{array} { r } { X _ { \beta } = \bigcup _ { \alpha < \beta } X _ { \alpha } } \end{array}$ and it is easy to see that it satisfies property (6.5). Assume that $\beta$ is a successor ordinal, say $\beta = \alpha + 1$ . Then g is defined on $X _ { \alpha }$ . We have to extend our definition to the set $Z = X _ { \alpha + 1 } \setminus X _ { \alpha }$ 

Since $| Z | \le | X _ { \alpha + 1 } | < \kappa$ we can find a function $h \colon Z \to \omega$ satisfying (6.5). We might try to define g on $Z$ as h. However, this might not work, since for $z \in Z$ there might be an $x \in X _ { \alpha }$ such that $| z - x | \in \mathbb { Q }$ . But $X _ { \alpha }$ is closed under the action of $\mathcal { F }$ . Thus for every $z \in Z$ there is at most one $x _ { z } \in X _ { \alpha }$ such that $| z - x _ { z } | \in \mathbb { Q }$ . So we will define g on $Z$ such that for every $z \in Z$ and $h ( z ) = n$ we have $g ( z ) \in \{ 2 n , 2 n + 1 \}$ . Then $g | _ { Z }$ will satisfy (6.5), as h did. Now it is enough to choose $g ( z )$ diferent from $g ( x _ { z } )$ , if $x _ { z }$ exists, and arbitrarily otherwise.  

It can be proved also that $\mathbb { R } ^ { n }$ can be decomposed as in Theorem 6.1.7 for all $n \in \mathbb { N }$ . However, the proof for $n > 2$ is considerably more dificult. 

The last theorem of this section is due to Sierpi´nski (1919). Although its proof is essentially easier that those of previous theorems it has its own flavor – the set constructed in the theorem exists if and only if the continuum hypothesis is assumed. 

Theorem 6.1.8 The continuum hypothesis is equivalent to the existence of a subset A of $\mathbb { R } ^ { 2 }$ with the property that 

$$
\left| A ^ {y} \right| \leq \omega \quad a n d \quad \left| \left(\mathbb {R} ^ {2} \setminus A\right) _ {x} \right| \leq \omega
$$

for every $x , y \in \mathbb { R }$ 

Proof $\Rightarrow :$ First assume the continuum hypothesis ${ \mathfrak { c } } = \omega _ { 1 }$ and let $\preceq$ be a well ordering of R of type $\omega _ { 1 }$ . (To find it, take a bijection $f \colon \mathbb { R }  \omega _ { 1 }$ and define $x \preceq y$ if and only if $f ( x ) \leq f ( y ) . )$ Define $A = \{ \langle x , y \rangle \colon x \preceq y \}$ 

Now $A ^ { y } = \{ x \in \mathbb { R } \colon \langle x , y \rangle \in A \} = \{ x \in \mathbb { R } \colon x \preceq y \}$ is an initial segment of a set with order type $\omega _ { 1 }$ , so it has cardinality $< \ \omega _ { 1 }$ , that is, $\leq \omega$ Similarly, 

$$
\begin{array}{r c l} (\mathbb {R} ^ {2} \setminus A) _ {x} & = & (\{\langle x, y \rangle \in \mathbb {R} ^ {2} \colon \langle x, y \rangle \not \in A \}) _ {x} \\ & = & (\{\langle x, y \rangle \in \mathbb {R} ^ {2} \colon y \prec x \}) _ {x} \\ & = & \{y \in \mathbb {R} \colon y \prec x \} \end{array}
$$

is an initial segment of a set with order type $\omega _ { 1 }$ , that is, has cardinality $\leq \omega$ 

⇐: Assume that $| \mathbb { R } | = { \mathfrak { c } } > \omega _ { 1 }$ and let $A \subset \mathbb { R } ^ { 2 }$ be such that $| A ^ { y } | \le \omega$ for every $y \in \mathbb { R }$ . We will show that the complement of A has an uncountable vertical section. 

Let $Y \subset$ R be such that $| Y | = \omega _ { 1 } { \mathrm { ~ } } ( { \mathrm { i f ~ } } f \colon { \mathfrak { c } } \to \mathbb { R }$ is a bijection, take $Y = f [ \omega _ { 1 } ] )$ . Let $\textstyle X = \bigcup _ { y \in Y } A ^ { y }$ . Then $| X | \le \omega _ { 1 }$ as it is a union of $\omega _ { 1 }$ sets of cardinality $< \omega _ { 1 }$ . Take $x \in \mathbb { R } \setminus X$ . Then $\langle x , y \rangle \not \in A$ for every $y \in Y$ , since x $\notin A ^ { y }$ . Hence $\{ x \} \times Y \subset \mathbb { R } ^ { 2 } \setminus A$ and so $Y \subset ( \mathbb { R } ^ { 2 } \setminus A ) _ { x }$ . Therefore $\left| ( \mathbb { R } ^ { 2 } \setminus A ) _ { x } \right| \geq \omega _ { 1 } > \omega$  

## EXERCISES

1 Complete the proof of Lemma $6 . 1 . 6 ( \mathrm { b } )$ by showing that for every limit ordinal $\lambda < \omega _ { 1 }$ the set $\textstyle X _ { \lambda } = \bigcup _ { \alpha < \lambda } X _ { \alpha }$ is closed under the action of $\mathcal { F }$ as long as every $X _ { \alpha }$ is closed under the action of $\mathcal { F }$ for $\alpha < \lambda$ 

2 Prove that $\mathbb { R } ^ { 3 } \setminus \mathbb { Q } ^ { 3 }$ is a union of disjoint lines. 

3 Generalize Theorem 6.1.3 by proving that $\mathbb { R } ^ { 3 }$ is a union of disjoint circles of radius 1. 

4 Modify Mazurkiewicz’s theorem (Theorem 6.1.2) by proving that there exists a subset A of the plane $\mathbb { R } ^ { 2 }$ that intersects every circle in exactly three points. 

5 Modify Sierpi´nski’s theorem (Theorem 6.1.8) by proving that the continuum hypothesis is equivalent to the following statement: There exist sets $A _ { 0 } , A _ { 1 } , A _ { 2 } \subset \mathbb { R } ^ { 3 }$ such that $\mathbb { R } ^ { 3 } = A _ { 0 } \cup A _ { 1 } \cup A _ { 2 }$ and 

$$
\left| \left\{\langle x _ {0}, x _ {1}, x _ {2} \rangle \in A _ {i}: x _ {i} = x \right\} \right| \leq \omega
$$

for every $i < 3$ and $x \in \mathbb { R }$ 

Try to generalize this and Theorem 6.1.8 to $\mathbb { R } ^ { n }$ for all $1 < n < \omega$ . Prove your claim. 

6 (Challenging) Prove the following theorem of Ceder: There is a decomposition $\{ S _ { i } \} _ { i < \omega }$ of $\mathbb { R } ^ { 2 }$ with no $S _ { i }$ spanning an equilateral triangle. Remark: It is also possible to find a decomposition $\{ S _ { i } \} _ { i < \omega }$ of $\mathbb { R } ^ { 2 }$ with no $S _ { i }$ spanning an isosceles triangle. This has been proved recently by Schmerl. 

## 6.2 Closed sets and Borel sets

In what follows we will concentrate on the topological structure of $\mathbb { R } ^ { n }$ Recall that $\mathbb { Q } ^ { n }$ is a countable dense subset of $\mathbb { R } ^ { n }$ and that the family $\begin{array} { r } { B = \{ B ( p , \varepsilon ) \colon p \in \mathbb { Q } ^ { n } \ \& \ \varepsilon \in \mathbb { Q } \} } \end{array}$ of open balls forms a countable base for $\mathbb { R } ^ { n }$ , that is, for every open set $U$ in $\mathbb { R } ^ { n }$ and every $p \in U$ there is a $B \in B$ such that $p \in B \subset U$ 

A point $p$ of a subset P of $\mathbb { R } ^ { n }$ is an isolated point of $P$ if there is an open set $U$ (in $\mathbb { R } ^ { n }$ or in $P )$ such that $U \cap P = \{ p \}$ . A subset $S$ of $\mathbb { R } ^ { n }$ is discrete if every point of S is isolated in S. A nonempty closed subset $F$ of $\mathbb { R } ^ { n }$ is said to be perfect if it has no isolated points. 

We will start this section with a study of the structure of closed subsets of $\mathbb { R } ^ { n }$ . For this we will need a few theorems that are of interest in their own right. 

## Theorem 6.2.1

(i) Every family U of pairwise-disjoint open subsets of $\mathbb { R } ^ { n }$ is at most countable. 

(ii) Every discrete subset S of $\mathbb { R } ^ { n }$ is at most countable. 

(iii) If α is an ordinal number and $\{ S _ { \xi } \colon \xi < \alpha \}$ is a strictly increasing (decreasing) sequence of open (closed) sets in $\mathbb { R } ^ { n }$ then α is at most countable. 

Proof (i) Define $f \colon \mathcal { U } \setminus \{ \emptyset \} \to \mathbb { Q } ^ { n }$ by choosing $f ( U ) \in U \cap \mathbb { Q } ^ { n }$ for every $U \in \mathcal { U }$ . Then $f$ is one-to-one, and so $| \mathcal { U } | \leq | \mathbb { Q } ^ { n } | + 1 = \omega$ 

(ii) For every $s \in S$ let $r _ { s } > 0$ be such that $S \cap B ( s , 2 r _ { s } ) = \{ s \}$ and let $\mathcal { U } = \{ B ( s , r _ { s } ) \colon s \in S \}$ . Notice that $B ( s , r _ { s } ) \cap B ( t , r _ { t } ) = \varnothing$ for distinct $s , t \in S$ . Thus, by (i), U is at most countable. Hence $| S | \leq | \mathcal { U } | \leq \omega$ 

(iii) We assume that $\mathcal { U } = \{ S \varepsilon \colon \xi < \alpha \}$ is a strictly increasing sequence of open sets. The argument for the other case is essentially the same. 

To obtain a contradiction assume that α is uncountable. Thus α $\geq \omega _ { 1 }$ For $\xi < \omega _ { 1 }$ choose $x _ { \xi } \in S _ { \xi + 1 } \setminus S _ { \xi }$ and let $B _ { \xi } \in B$ be such that $x _ { \xi } \in B _ { \xi } \subset$ $S _ { \xi + 1 }$ . Then the set $X = \{ x _ { \xi } \colon \xi < \omega _ { 1 } \}$ is uncountable, since $x _ { \xi } \neq x _ { \zeta }$ for $\zeta < \xi < \omega _ { 1 }$ . But the function $f \colon X  B , f ( x _ { \xi } ) = B _ { \xi }$ , is one-to-one, since for $\zeta < \xi < \omega _ { 1 } , x _ { \xi } \in B _ { \xi } \backslash B _ { \zeta }$ , that is, $B _ { \xi } \neq B _ { \zeta }$ . However, this is impossible, since it would imply $\omega _ { 1 } = | X | \leq | B | = \omega$ 

This contradiction finishes the proof. 

Theorem 6.2.2 For an ordinal number α the following conditions are equivalent: 

(i) $\alpha < \omega _ { 1 }$ ; 

(ii) there exists an $S \subset \mathbb { R }$ well ordered by the standard relation $\leq$ of order type α. 

Proof $( \mathrm { i i } ) { \Rightarrow } ( \mathrm { i } )$ : Assume, to obtain a contradiction, that for some α $\geq \omega _ { 1 }$ there exists an $S \subset \mathbb { R }$ with order type α. Let $h \colon \alpha  S$ be an order isomorphism and define $U _ { \xi } = ( h ( \xi ) , h ( \xi + 1 ) )$ for $\xi < \omega _ { 1 }$ . Then $\{ U _ { \xi } \colon \xi < \omega _ { 1 } \}$ is an uncountable family of nonempty, open, and pairwise-disjoint subsets of R. This contradicts Theorem 6.2.1(i). 

$( \mathrm { i } ) { \Rightarrow } ( \mathrm { i i } )$ : For the other implication we will prove the following fact by induction on $\alpha < \omega _ { 1 }$ : 

(G) for every $a , b \in \mathbb { R }$ with $a < b$ there exists an $S \subset [ a , b )$ with $\mathrm { O t p } ( S ) = \alpha$ 

For $\alpha = 0$ the condition is clearly true. So let $0 < \alpha < \omega _ { 1 }$ be such that (G) holds for all $\beta < \alpha$ . We will show that (G) holds for α. 

Take $a , b \in \mathbb { R }$ with $a < b$ . If $\alpha = \beta + 1$ is an ordinal successor, pick c with $a < c < b$ and $S \subset [ a , c )$ with $\mathrm { O t p } ( S ) = \beta$ . This can be done by the inductive assumption. Then $S \cup \{ c \} \subset [ a , b )$ and $\operatorname { O t p } ( S \cup \{ c \} ) = \beta + 1 = \alpha .$ 

If α is a limit ordinal, then cf $( \alpha ) \leq \alpha < \omega _ { 1 }$ and cf(α) is infinite. So cf $( \alpha ) = \omega$ . Let $\lbrace \alpha _ { n } < \alpha \colon n < \omega \rbrace$ be a strictly increasing sequence that is cofinal in α with $\alpha _ { 0 } = 0$ . Find a strictly increasing sequence $a = a _ { 0 } < a _ { 1 } <$ $\cdot \cdot \cdot < a _ { n } < \cdot \cdot \cdot < b$ (for example, put $a _ { n } = b - [ ( b - a ) / ( n + 1 ) ] )$ . For every $n < \omega$ choose $S _ { n } \subset [ a _ { n } , a _ { n + 1 } )$ with ${ \mathrm { O t p } } ( S _ { n } ) = { \mathrm { O t p } } ( \alpha _ { n + 1 } \backslash \alpha _ { n } )$ . This can be done by the inductive hypothesis, since $\mathrm { O t p } ( \alpha _ { n + 1 } \setminus \alpha _ { n } ) \le \alpha _ { n + 1 } < \alpha$ . Put $\textstyle S = \bigcup _ { n < \omega } S _ { n }$ . Then $S \subset [ a , b )$ . Moreover, if $f _ { n } \colon \left( \alpha _ { n + 1 } \atop \ldots \right) \sim S _ { n }$ is an order isomorphism then $\begin{array} { r } { f = \bigcup _ { n < \omega } f _ { n } \colon \alpha  S } \end{array}$ is also an order isomorphism, that is, $\mathrm { O t p } ( S ) = \alpha$ . Condition (G) has been proved for every $\alpha < \omega _ { 1 }$ 

Now (G) clearly implies (ii). 

Theorem 6.2.3 Every perfect subset P of $\mathbb { R } ^ { n }$ has cardinality continuum. 

Proof Clearly $| P | \leq | \mathbb { R } ^ { n } | = { \mathfrak { c } }$ . Thus it is enough to show that $| P | \geq { \mathfrak { c } }$ Before we prove it we notice the following easy fact. 

(A) If $R \subset \mathbb { R } ^ { n }$ is perfect, $U \subset \mathbb { R } ^ { n }$ is open, and $R \cap U = R \cap \operatorname { c l } ( U ) \neq \emptyset$ then $R \cap { \mathrm { c l } } ( U )$ is perfect. 

Clearly $R \cap { \mathrm { c l } } ( U )$ is closed. Also, $p \in R \cap \operatorname { c l } ( U )$ cannot be isolated since otherwise there would exist an open set $W \subset \mathbb { R } ^ { n }$ with the property that $\{ p \} = ( R \cap \operatorname { c l } ( U ) ) \cap W = ( R \cap U ) \cap W = R \cap ( U \cap W )$ and the set $U \cap W$ would show that p is an isolated point of R. 

Now let $p _ { i } \colon \mathbb { R } ^ { n } \ \to \ \mathbb { R }$ be the projection onto the ith coordinate. If there exists an $i < n$ such that $| p _ { i } [ P ] | = { \mathfrak { c } }$ , then $| P | \geq { \mathfrak { c } }$ . So, to obtain a contradiction, assume that 

(B) $| p _ { i } [ P ] | < { \mathfrak { c } }$ for every $i < n$ 

Notice also that 

(C) if $R \subset P$ is perfect, then there are disjoint perfect sets $R _ { 0 } , R _ { 1 } \subset R$ 

To see it, let $i < n$ be such that $p _ { i } [ R ]$ contains two numbers $a < b . { \mathrm { ~ B y ~ ( B ) } }$ we can find $r \in ( a , b ) \backslash p _ { i } [ R ]$ . Then, by (A), the sets $R _ { 0 } = R \cap p _ { i } ^ { - 1 } ( ( - \infty , r ] )$ and $R _ { 1 } = R \cap p _ { i } ^ { - 1 } ( [ r , \infty ) )$ are disjoint and perfect. 

Now we construct a family $\{ P _ { s } \subset P \colon s \in 2 ^ { < \omega } \}$ of perfect bounded sets by induction on the length |s| of a sequence s. 

We put $P _ { \varnothing } = P \cap [ a , b ] ^ { n }$ , where $a < b$ are chosen in such a way that $P _ { \varnothing } \neq \varnothing$ and $\textstyle a , b \in \mathbb { R } \backslash \bigcup _ { i < n } p _ { i } [ P ]$ . This can be done by (B). So $P \cap ( a , b ) ^ { n } =$ $P \cap [ a , b ] ^ { n }$ . In particular, $P _ { \varnothing }$ is compact and, by $\mathrm { ( A ) }$ , perfect. We will continue the induction, maintaining the following inductive condition to be satisfied for every $s \in 2 ^ { < \omega }$ 

(I) $P _ { s 0 }$ and $P _ { s 1 }$ are disjoint perfect subsets of $P _ { s }$ , 

where s0 and s1 stand for the sequences of length $| s | + 1$ extending s by 0 and 1, respectively. We can find such sets by (C). 

Now notice that for $f \in 2 ^ { \omega }$ the sets $P _ { f \mid _ { k } }$ for $k < \omega$ form a decreasing sequence of nonempty compact sets. Thus, the sets $\begin{array} { r } { P _ { f } = \bigcap _ { k < \omega } P _ { f | _ { k } } } \end{array}$ are nonempty. Notice also that the sets $P _ { f }$ and $P _ { g }$ are disjoint for different $f , g \in 2 ^ { \omega }$ . To see this, let $k = \mathrm { m i n } \{ i \in \tilde { \omega } \colon f ( i ) \neq g ( i ) \}$ . Then $\{ f ( k ) , g ( k ) \} = \{ 0 , 1 \}$ and 

$$
P _ {f} \cap P _ {g} \subset P _ {f | _ {k + 1}} \cap P _ {g | _ {k + 1}} = P _ {s 0} \cap P _ {s 1} = \emptyset ,
$$

where $s = f | _ { k } = g | _ { k }$ 

Let $\psi : 2 ^ { \omega }  P$ be such that $\psi ( f ) \in P _ { f }$ (this is a choice function). Then $\psi$ is clearly one-to-one and so $| P | \geq { \mathfrak { c } } .$  

The induction constructions of the preceding proof are often referred to as tree constructions, since $T \ = \ 2 ^ { < \omega }$ is called a tree. (We imagine every $s \in T$ as a “tree-branching point,” where the tree is splitting into s0 and s1.) 

For $F \subset \mathbb { R } ^ { n }$ we denote by $F ^ { \prime }$ the set of all limit points of $F$ , that is, all points of $\operatorname { c l } ( F )$ that are not isolated. Clearly $F \setminus F ^ { \prime }$ is equal to the set of all isolated points of $F$ 

Now we are ready to prove the following theorem characterizing closed subsets of $\mathbb { R } ^ { n }$ 

Theorem 6.2.4 (Cantor–Bendixson theorem) Every uncountable, closed subset $F$ of $\mathbb { R } ^ { n }$ can be represented as a disjoint union of a perfect set $P$ and an at most countable set C. 

Proof By induction on $\alpha < \omega _ { 1 }$ we construct a sequence $\{ F _ { \alpha } \colon \alpha < \omega _ { 1 } \}$ of closed subsets of $\mathbb { R } ^ { n }$ by defining: 

$$
F _ {0} = F, \quad F _ {\lambda} = \bigcap_ {\xi <   \lambda} F _ {\xi} \text { for } \lambda <   \omega_ {1}, \lambda \text { a   limit   ordinal },
$$

and 

$$
F _ {\alpha + 1} = (F _ {\alpha}) ^ {\prime}.
$$

The sequence $\{ F _ { \alpha } \colon \alpha < \omega _ { 1 } \}$ is decreasing and formed of closed sets. It can’t be strictly decreasing by Theorem 6.2.1(iii). Thus there exists an $\alpha <$ $\omega _ { 1 }$ such that $F _ { \alpha } = F _ { \alpha + 1 }$ . This means that $F _ { \alpha }$ does not have any isolated points, that is, $F _ { \alpha }$ is either perfect or empty. But $\begin{array} { r } { F \backslash F _ { \alpha } = \bigcup _ { \beta < \alpha } ( F _ { \beta } \backslash F _ { \beta + 1 } ) } \end{array}$ and every set $F _ { \beta } \setminus F _ { \beta + 1 } = F _ { \beta } \setminus ( F _ { \beta } ) ^ { \prime }$ is discrete, so, by Theorem 6.2.1(ii), it is at most countable. Hence $F \setminus F _ { \alpha }$ is a union of $| \alpha | \le \omega$ sets, each of which is at most countable. Therefore $C = F \setminus F _ { \alpha }$ is at most countable, and $P = F _ { \alpha } = F \setminus C$ cannot be empty. So P is perfect.  

Corollary 6.2.5 The cardinality of a closed subset of $\mathbb { R } ^ { n }$ is either equal to continuum $o r$ is at most countable. 

Theorems 6.2.3 and 6.2.4 tell us the properties that closed subsets of $\mathbb { R } ^ { n }$ must have. Can we tell anything more? Exercise 1 shows that we cannot expect much improvement in the case of Theorem 6.2.4. But what about Theorem 6.2.3? How can perfect sets look? They can certainly be formed as a union of some number of closed intervals. But for such sets Theorem 6.2.3 is obvious. Are there any other perfect sets? The afirmative answer is given by a set $C \subset \mathbb { R }$ to be constructed and known as the Cantor set (or Cantor ternary set). It is constructed as follows. 

First, we define the family $\{ I _ { s } \subset P \colon s \in 2 ^ { < \omega } \}$ of closed intervals by induction on the length |s| of s. We p ut $I _ { \emptyset } = [ 0 , 1 ]$ . If the interval $I _ { s } = $ $[ a _ { s } , b _ { s } ]$ is already constructed, we remove from it the middle third interval, and define $I _ { s 0 }$ and $I _ { s 1 }$ as the left interval and the right interval, respectively, of the remaining two intervals, that is, $I _ { s 0 } = [ a _ { s } , a _ { s } + ( b _ { s } - a _ { s } ) / 3 ]$ and $I _ { s 1 } = [ b _ { s } - ( b _ { s } - a _ { s } ) / 3 , b _ { s } ]$ . Put $C _ { n } = \bigcup \{ I _ { s } \colon | s | = n \}$ . Thus $C _ { n }$ is the union of all $2 ^ { n }$ internals of length $1 / 3 ^ { n }$ constructed at step n. Notice that $[ 0 , 1 ] = C _ { 0 } \supset C _ { 1 } \supset \cdot \cdot .$ and that each $C _ { n }$ is closed, being a finite union of closed intervals. We define $\begin{array} { r } { C = \bigcap _ { n < \omega } C _ { n } } \end{array}$ 

The set C is clearly closed and nonempty. To see that it is perfect, let $p \in C$ and let J be an open interval containing p. Then there is an $s \in 2 ^ { < \omega }$ such that the interval $I _ { s }$ (of length $1 / 3 ^ { | s | } )$ contains p and is contained in J. Let $j < 2$ be such that $p \notin I _ { s j }$ . Since $\begin{array} { r } { C \cap I _ { s j } = \bigcap _ { n < \omega } ( C _ { n } \cap I _ { s j } ) } \end{array}$ is nonempty, being the intersection of a decreasing sequence of nonempty compact sets, we conclude that $C \cap J \neq \{ p \}$ . So C is perfect. 

Notice also that C does not contain any nonempty interval. This is so since for any interval J of length $\varepsilon > 0$ we can find an $n < \omega$ such that $1 / 3 ^ { n } < \varepsilon$ . But $C _ { n }$ is a union of intervals of length $1 / 3 ^ { n } < \varepsilon$ . So $J \not \subset C _ { n }$ , and $J \not \subset C$ since $C \subset C _ { n }$ 

Finally, it is worthwhile to mention that C is the set of all numbers from [0, 1] whose ternary representations do not contain the digit 1, that is, 

$$
C = \left\{\sum_ {n = 0} ^ {\infty} \frac {d (n)}{3 ^ {n + 1}}: d \in \{0, 2 \} ^ {\omega} \right\}.
$$

This will be left without a proof. 

To define Borel subsets of topological spaces we need the following definitions. A family ${ \mathcal { A } } \subset { \mathcal { P } } ( X )$ is a σ-algebra on X if A is nonempty and closed under complements and under countable unions, that is, such that 

(i) $\varnothing , X \in A ;$ ; 

(ii) if $A \in { \mathcal { A } }$ then $X \setminus A \in { \mathcal { A } }$ 

(iii) if $A _ { k } \in { \mathcal { A } }$ for every $k < \omega$ then $\textstyle \bigcup _ { k < \omega } A _ { k } \in { \mathcal { A } }$ 

Notice also that every σ-algebra is also closed under countable intersections, since 

$$
\bigcap_ {k <   \omega} A _ {k} = X \setminus \bigcup_ {k <   \omega} (X \setminus A _ {k}).
$$

Examples For every nonempty set X the following families form σ-algebras: 

(1) ${ \mathcal A } = \{ \emptyset , X \}$ 

(2) $\mathcal { A } = \mathcal { P } ( \boldsymbol { X } )$ 

(3) $\mathcal A = \{ A \in \mathcal P ( X ) \colon | A | \leq \kappa \mathrm { ~ o r ~ } | X \setminus A | \leq \kappa \}$ for any infinite cardinal κ. 

Notice that for every ${ \mathcal { F } } \subset { \mathcal { P } } ( X )$ there is a smallest σ-algebra $\sigma [ \mathcal { F } ]$ on X containing $\mathcal { F }$ , namely, 

$$
\sigma [ \mathcal {F} ] = \bigcap \{\mathcal {A} \subset \mathcal {P} (X) \colon \mathcal {F} \subset \mathcal {A} \& \mathcal {A} \text { is   a } \sigma \text {-algebra   on } X \}.\tag{6.6}
$$

In particular, for every topological space $\langle X , \tau \rangle$ we define the σ-algebra Bor of Borel sets by $B o r = \sigma [ \tau ]$ 

It is obvious from the definition that the following sets are Borel: 

$G _ { \delta }$ sets, that is, the countable intersections of open sets; 

$F _ { \sigma }$ sets, that is, the countable unions of closed sets; 

$G _ { \delta \sigma }$ sets, that is, the countable unions of $G _ { \delta }$ sets; 

$F _ { \sigma \delta }$ sets, that is, the countable intersections of $F _ { \sigma }$ sets; 

and so on. 

Is an arbitrary subset of a topological space $\langle X , \tau \rangle$ Borel? The answer to this question depends on the topological space. For example, in a discrete space $\langle X , { \mathcal { P } } ( X ) \rangle$ every set is open and hence Borel. This is, however, quite an exceptional example and more often $\mathcal { P } ( X ) \neq B o r$ . We will not approach this question in general. However, we will address it in the case of $\mathbb { R } ^ { n }$ 

To shed more light on the structure of Borel sets, define inductively the following hierarchy of sets for a topological space $\langle X , \tau \rangle$ : 

$$
\Sigma_ {1} ^ {0} = \tau ,
$$

$$
\Sigma_ {\alpha} ^ {0} = \left\{\bigcup_ {k <   \omega} (X \setminus A _ {k}) \colon A _ {k} \in \bigcup_ {0 <   \beta <   \alpha} \Sigma_ {\beta} ^ {0} \text {for all} k <   \omega \right\} \quad \text {for} 1 <   \alpha <   \omega_ {1}.
$$

<sub>Define also</sub> 

$$
\Pi_ {\alpha} ^ {0} = \{X \setminus A \colon A \in \Sigma_ {\alpha} ^ {0} \} \quad \text { for } 0 <   \alpha <   \omega_ {1}.
$$

Thus 

$$
\Sigma_ {\alpha} ^ {0} = \left\{\bigcup_ {k <   \omega} A _ {k} \colon A _ {k} \in \bigcup_ {0 <   \beta <   \alpha} \Pi_ {\beta} ^ {0} \text {for all} k <   \omega \right\} \quad \text {for} 1 <   \alpha <   \omega_ {1}.
$$

It is very easy to prove, by induction on $0 < \alpha < \omega _ { 1 }$ , that 

$$
\Sigma_ {\alpha} ^ {0}, \Pi_ {\alpha} ^ {0} \subset \mathcal {B} o r \quad \text { for   every } 0 <   \alpha <   \omega_ {1}.\tag{6.7}
$$

Notice that $\Pi _ { 1 } ^ { 0 }$ is equal to the family of all closed subsets of X, $\Sigma _ { 2 } ^ { 0 } = F _ { \sigma }$ , $\Pi _ { 2 } ^ { 0 } = G _ { \delta } , \Sigma _ { 3 } ^ { 0 } = \bar { G _ { \delta \sigma } }$ , and $\Pi _ { 3 } ^ { 0 } = F _ { \sigma \delta }$ 

From now on we will assume that $X = \mathbb { R } ^ { n }$ . In particular, any closed subset $F$ of $\mathbb { R } ^ { n }$ is $G _ { \delta }$ , as 

$$
F = \bigcap_ {k <   \omega} \left\{x \in \mathbb {R} ^ {n}: \exists y \in F (d (y, x) <   1 / (k + 1)) \right\} = \bigcap_ {k <   \omega} \bigcup_ {y \in F} B (y, 1 / (k + 1)).
$$

Similarly, every open set in $\mathbb { R } ^ { n }$ is $F _ { \sigma }$ . Hence 

$$
\Sigma_ {1} ^ {0} \subset \Sigma_ {2} ^ {0} \quad \mathrm{and} \quad \Pi_ {1} ^ {0} \subset \Pi_ {2} ^ {0}.\tag{6.8}
$$

Using these inclusions it is not dificult to prove 

Proposition 6.2.6 For every $0 < \beta < \alpha < \omega _ { 1 }$ 

$$
\Sigma_ {\beta} ^ {0} \subset \Sigma_ {\alpha} ^ {0}, \quad \Pi_ {\beta} ^ {0} \subset \Pi_ {\alpha} ^ {0}, \quad \Sigma_ {\beta} ^ {0} \subset \Pi_ {\alpha} ^ {0}, \quad \Pi_ {\beta} ^ {0} \subset \Sigma_ {\alpha} ^ {0}.
$$

Proof Inclusion $\Pi _ { \beta } ^ { 0 } \subset \Sigma _ { \alpha } ^ { 0 }$ follows immediately from the definition of $\Sigma _ { \alpha } ^ { 0 }$ Now, to see $\Sigma _ { \beta } ^ { 0 } \subset \dot { \Pi } _ { \alpha } ^ { 0 }$ notice that 

$$
A \in \Sigma_ {\beta} ^ {0} \Rightarrow \mathbb {R} ^ {n} \setminus A \in \Pi_ {\beta} ^ {0} \subset \Sigma_ {\alpha} ^ {0} \Rightarrow A \in \Pi_ {\alpha} ^ {0}.
$$

We prove 

$$
\Sigma_ {\beta} ^ {0} \subset \Sigma_ {\alpha} ^ {0}, \quad \Pi_ {\beta} ^ {0} \subset \Pi_ {\alpha} ^ {0} \quad \mathrm{forevery} \quad 0 <   \beta <   \alpha
$$

by joint induction on α. So assume that for some $1 < \gamma < \omega _ { 1 }$ this condition holds for every $\alpha < \gamma$ and let $0 < \delta < \gamma$ . We have to prove that $\Sigma _ { \delta } ^ { 0 } \subset \Sigma _ { \gamma } ^ { 0 }$ and $\Pi _ { \delta } ^ { 0 } \subset \Pi _ { \gamma } ^ { 0 }$ 

But then $\textstyle \bigcup _ { \beta < \delta } \Pi _ { \beta } ^ { 0 } \subset \bigcup _ { \beta < \gamma } \Pi _ { \beta } ^ { 0 }$ , and so 

$$
\Sigma_ {\delta} ^ {0} = \left\{\bigcup_ {k <   \omega} A _ {k} \colon A _ {k} \in \bigcup_ {\beta <   \delta} \Pi_ {\beta} ^ {0} \right\} \subset \left\{\bigcup_ {k <   \omega} A _ {k} \colon A _ {k} \in \bigcup_ {\beta <   \gamma} \Pi_ {\beta} ^ {0} \right\} = \Sigma_ {\gamma} ^ {0}.
$$

Now $\Pi _ { \delta } ^ { 0 } \subset \Pi _ { \gamma } ^ { 0 }$ follows from 

$$
A \in \Pi_ {\delta} ^ {0} \Rightarrow \mathbb {R} ^ {n} \setminus A \in \Sigma_ {\delta} ^ {0} \subset \Sigma_ {\gamma} ^ {0} \Rightarrow A \in \Pi_ {\gamma} ^ {0}.
$$

Proposition 6.2.6 has been proved. 

Theorem 6.2.7 The family Bor of Borel subsets of $\mathbb { R } ^ { n }$ is equal to 

$$
\mathcal {B} o r = \bigcup_ {0 <   \alpha <   \omega_ {1}} \Sigma_ {\alpha} ^ {0} = \bigcup_ {0 <   \alpha <   \omega_ {1}} \Pi_ {\alpha} ^ {0}.
$$

Proof First notice that Proposition 6.2.6 implies 

$$
\bigcup_ {0 <   \alpha <   \omega_ {1}} \Sigma_ {\alpha} ^ {0} = \bigcup_ {0 <   \alpha <   \omega_ {1}} \Pi_ {\alpha} ^ {0}.
$$

Let $\mathcal { F }$ denote this set. Notice also that $( 6 . 7 )$ implies that $\mathcal { F } \subset B o r$ . Since $\mathcal { F }$ contains the topology $\tau$ of $\mathbb { R } ^ { n }$ it is enough to show that $\mathcal { F }$ is a σ-algebra, since $B o r = \sigma [ \tau ]$ is the smallest σ-algebra containing $\tau .$ . Thus we have to prove that $\mathcal { F }$ is closed under complements and countable unions. 

If $A \in { \mathcal { F } }$ then $A \in \Sigma _ { \alpha } ^ { 0 }$ for some $0 < \alpha < \omega _ { 1 }$ . Hence $\mathbb { R } ^ { n } \setminus A \in \Pi _ { \alpha } ^ { 0 } \subset { \mathcal { F } }$ 

If $A _ { k } \in \mathcal { F }$ for $k < \omega$ then for every $k < \omega$ there exists $0 < \alpha _ { k } < \omega _ { 1 }$ such that $A _ { k } \in \Pi _ { \alpha _ { k } } ^ { 0 }$ . But $\omega _ { 1 } = \omega ^ { + }$ is regular, so there exists an $\alpha < \omega _ { 1 }$ such that $\alpha _ { k } < \alpha$ for every $k < \omega$ . Hence 

$$
A _ {k} \in \Pi_ {\alpha_ {k}} ^ {0} \subset \bigcup_ {0 <   \beta <   \alpha} \Pi_ {\beta} ^ {0}
$$

for every $k < \omega$ , and so $\begin{array} { r } { \bigcup _ { k < \omega } A _ { k } \in \Sigma _ { \alpha } ^ { 0 } \subset \mathcal { F } . } \end{array}$ 

Theorem 6.2.8 The family Bor of all Borel subsets of $\mathbb { R } ^ { n }$ has cardinality continuum. 

Proof First we will prove by induction that 

$$
\left| \Pi_ {\alpha} ^ {0} \right| = \left| \Sigma_ {\alpha} ^ {0} \right| = \mathfrak {c} \text {   for   every   } 0 <   \alpha <   \omega_ {1}.\tag{6.9}
$$

Equation $| \Pi _ { \alpha } ^ { 0 } | = | \Sigma _ { \alpha } ^ { 0 } |$ is established by a bijection $f \colon \Sigma _ { \alpha } ^ { 0 } \to \Pi _ { \alpha } ^ { 0 }$ defined by $f ( A ) = X \setminus A$ . Next we will prove that $| \Sigma _ { 1 } ^ { 0 } | = { \mathfrak { c } }$ . The inequality $| \Sigma _ { 1 } ^ { 0 } | =$ $| \tau | \leq { \mathfrak { c } }$ is justified by a surjective function $f \colon { \mathcal { P } } ( { \mathcal { B } } ) \to \tau , f ( { \mathcal { U } } ) = \bigcup { \mathcal { U } } .$ where $\boldsymbol { B }$ is a countable base for $\mathbb { R } ^ { n }$ . The inequality $| \tau | \geq { \mathfrak { c } }$ follows from the facts that the base $\boldsymbol { B }$ contains an infinite subfamily $\mathcal { G }$ of pairwise-disjoint sets and that $f$ restricted to ${ \mathcal { P } } ( { \mathcal { G } } )$ is one-to-one, while $| { \mathcal { P } } ( { \mathcal { G } } ) | = { \mathfrak { c } }$ 

Now assume that for some $1 < \alpha < \omega _ { 1 }$ we have $| \Pi _ { \beta } ^ { 0 } | = | \Sigma _ { \beta } ^ { 0 } | = { \mathfrak { c } }$ for all $0 < \beta < \alpha$ . We have to prove $| \Sigma _ { \alpha } ^ { 0 } | = { \mathfrak { c } }$ 

But, by the inductive hypothesis, $\begin{array} { r } { | \bigcup _ { \beta < \alpha } \Pi _ { \beta } ^ { 0 } | = \mathfrak { c } } \end{array}$ since it is a union of $| \alpha | < \omega _ { 1 } \le { \mathfrak { c } }$ sets of cardinality c. Moreover, $F \colon ( \bigcup _ { \beta < \alpha } \Pi _ { \beta } ^ { 0 } ) ^ { \omega }  \Sigma _ { \alpha } ^ { 0 }$ defined by $\begin{array} { r } { F ( \left. A _ { 0 } , A _ { 1 } , \ldots \right. ) = \bigcup _ { n < \omega } A _ { n } } \end{array}$ is onto $\Sigma _ { \alpha } ^ { 0 }$ , so 

$$
\left| \Sigma_ {\alpha} ^ {0} \right| \leq \left| \left(\bigcup_ {\beta <   \alpha} \Pi_ {\beta} ^ {0}\right) ^ {\omega} \right| = \left| \bigcup_ {\beta <   \alpha} \Pi_ {\beta} ^ {0} \right| ^ {\omega} = (2 ^ {\omega}) ^ {\omega} = \mathfrak {c}.
$$

Since ${ \mathfrak { c } } = | \Sigma _ { 1 } ^ { 0 } | \leq | \Sigma _ { \alpha } ^ { 0 } |$ , condition (6.9) has been proved. 

Now, by Theorem 6.2.7, $\begin{array} { r } { B o r = \bigcup _ { 0 < \alpha < \omega _ { 1 } } \Sigma _ { \alpha } ^ { 0 } } \end{array}$ is a union of $\omega _ { 1 } \leq \mathfrak { c }$ sets of cardinality c, that is, it has cardinality continuum.  

Corollary 6.2.9 There is a non-Borel subset of $\mathbb { R } ^ { n }$ . 

Proof By Theorem 6.2.8 we have 

$$
\left| \mathcal {P} \left(\mathbb {R} ^ {n}\right) \right| = 2 ^ {\left| \mathbb {R} ^ {n} \right|} = 2 ^ {\mathfrak {c}} > \mathfrak {c} = | \mathcal {B o r} |,
$$

that is, $\mathcal { P } ( \mathbb { R } ^ { n } ) \setminus B o r \ne \emptyset$ 

We will construct some explicit examples of non-Borel sets in the next section. 

## EXERCISES

1 For a closed set $F \subset \mathbb { R }$ let $\{ F _ { \alpha } \colon \alpha < \omega _ { 1 } \}$ be a sequence from the proof of Theorem 6.2.4. Show that for every $\alpha < \omega _ { 1 }$ there exists a closed subset $F \subset \mathbb { R }$ for which $F _ { \alpha + 1 } \neq F _ { \alpha }$ 

2 Prove that the family $\sigma [ \mathcal { F } ]$ defined by (6.6) is indeed a σ-algebra on X. 

3 Show that Theorem 6.2.7 remains true for an arbitrary topological space. 

4 Prove the following generalization of Lemma 6.1.6. 

Let X be a set and let $\mathcal { F }$ be a family of functions of the form $f \colon X ^ { \alpha } \to$ $X$ , where $\alpha \leq \omega$ . If $| \mathcal F | \le { \mathfrak c }$ then for every $Z \subset X$ there exists a $Y \subset X$ such that 

(i) $Z \subset Y$ ; 

(ii) Y is closed under the action of ${ \mathcal { F } } _ { : }$ , that is, for every $f \colon X ^ { \alpha } \to X$ from $\mathcal { F }$ and $S \in Y ^ { \alpha }$ we have $f ( S ) \in Y$ ; 

(iii) $| Y | \leq | Z | ^ { \omega } + \mathfrak { c } .$ 

Notice that this fact (used with $X = \mathcal { P } ( \mathbb { R } ^ { n } ) , Z = \tau$ , and $\mathcal { F }$ composed of countable unions and complements) implies Theorem 6.2.8. 

5 Prove that every uncountable Borel subset of R contains a perfect subset. 

## 6.3 Lebesgue-measurable sets and sets with the Baire property

To construct the most useful σ-algebras we need the following definitions. 

Recall, from Section 2.1, that a nonempty family I of subsets of a set X is an ideal on X if it is closed under the subset operation and under finite unions, that is, such that 

(i) if $A , B \in \mathcal { T }$ then $A \cup B \in { \mathcal { T } } ;$ ; 

(ii) if $A \in \mathcal { T }$ and $B \subset A$ then $B \in \mathcal { T }$ 

An ideal I is said to be a σ-ideal if it is closed under countable unions, that is, if 

(i<sup>-</sup>) $\textstyle \bigcup _ { k \in \omega } A _ { k } \in { \mathcal { T } }$ provided $A _ { k } \in \mathcal { T }$ for all $k < \omega$ 

The elements of an ideal on X are usually considered as “small” in some sense. 

Examples 1. ${ \mathcal { T } } = \{ \emptyset \}$ is a σ-ideal on every set $X$ . 

2. For every $A \subset X$ the family ${ \mathcal { T } } = { \mathcal { P } } ( A )$ forms a σ-ideal on X. In the case when $A = X$ we obtain ${ \mathcal { T } } = { \mathcal { P } } ( X )$ This ideal does not agree with our intuitive notion of a family of small sets. Thus, usually we will work with the proper ideals on X, that is, the ideals that are not equal to ${ \mathcal { P } } ( X )$ 

3. For every infinite cardinal number κ and every set X the family $\mathcal { T } =$ $[ X ] ^ { < \kappa }$ is an ideal on X. For $\kappa = \omega$ this is the ideal of finite subsets of X. For cf $( \kappa ) > \omega$ it is also a σ-ideal. Notice also that for $\kappa = \omega _ { 1 }$ this is the ideal $[ X ] ^ { \leq \omega }$ of at most countable subsets of $X$ 

4. For every topological space $\langle X , \tau \rangle$ the family $\mathcal { N D }$ of all nowhere-dense subsets of X (i.e., the subsets S of X such that int $( \operatorname { c l } ( S ) ) = \varnothing )$ is an ideal on X. 

5. For a topological space $\langle X , \tau \rangle$ the family 

$$
\mathcal {M} = \left\{\bigcup_ {k <   \omega} A _ {k}: A _ {k} \text { is   nowhere   dense   in } X \right\}
$$

is a σ-ideal on X. If $X = \mathbb { R } ^ { n }$ (or, more generally, X is a complete metric space or a compact space) then, by the Baire category theorem, $\mathcal { M }$ is proper. If moreover X does not have any isolated points, then $[ X ] ^ { \leq \omega } \subset { \mathcal { M } }$ The ideal M is usually called the ideal of Meager (or first-category) subsets of X. 

6. For n-dimensional Euclidean space $\mathbb { R } ^ { n }$ we say that $X ~ \subset ~ \mathbb { R } ^ { n }$ is a (Lebesgue) measure-zero set or a null set in $\mathbb { R } ^ { n }$ if for every $\varepsilon > 0$ there is a family of open balls $\{ B ( x _ { k } , r _ { k } ) \colon k < \omega \}$ such that $\textstyle X \subset \bigcup _ { k < \omega } B ( x _ { k } , r _ { k } )$ and $\textstyle \sum _ { k < \omega } r _ { k } ^ { n } < \varepsilon$ . The family 

$$
\mathcal {N} = \{X \subset \mathbb {R} ^ {n}: X \text { is   a   null   set   in } \mathbb {R} ^ {n} \}
$$

forms a proper σ-ideal in $\mathbb { R } ^ { n }$ called the σ-ideal of (Lebesgue) measure-zero sets or null sets. 

The ideals M and $\mathcal { N }$ on $\mathbb { R } ^ { n }$ are of main interest in real analysis. It is easy to see that every countable set belongs to both M and ${ \mathcal { N } } .$ . Also, for $n = 1$ , the Cantor set $C$ (see Section 6.2) is in $\mathcal { M } \cap \mathcal { N }$ . It belongs to M since it is closed and does not contain any nonempty open interval. It belongs to N since the total length of intervals forming $C _ { n } \supset C$ is $\begin{array} { r } { 2 ^ { n } \frac { 1 } { 3 ^ { n } } = \left( \frac { 2 } { 3 } \right) ^ { n } } \end{array}$ 

In what follows we will study σ-ideals M and N from the set-theoretic point of view. It is worthwhile to notice, however, that both these ideals measure “smallness” in a very diferent sense. Ideal M describes the smallness in a topological sense whereas $\mathcal { N }$ does so in a measure sense. The diference between these two “smallness” notions is best captured by the following example. 

Proposition 6.3.1 There exists a dense $G _ { \delta }$ set $G \subset \mathbb { R } ^ { n }$ such that $G \in \mathcal N$ and $\mathbb { R } ^ { n } \setminus G \in { \mathcal { M } }$ 

Proof Recall that $\mathbb { Q } ^ { n }$ is a countable dense subset of $\mathbb { R } ^ { n }$ . Let $\{ q _ { k } \colon k < \omega \}$ be an enumeration of $\mathbb { Q } ^ { n }$ . For $m < \omega$ let 

$$
G _ {m} = \bigcup_ {k <   \omega} B (q _ {k}, 2 ^ {- (m + k) / n})
$$

and let $\begin{array} { r } { G = \bigcap _ { m < \omega } G _ { m } } \end{array}$ 

$G \in \mathcal N$ <sub>since for every</sub> $\varepsilon > 0$ there exists an $m < \omega$ with $2 ^ { - ( m - 1 ) } < \varepsilon$ and 

$$
G \subset G _ {m} = \bigcup_ {k <   \omega} B (q _ {k}, 2 ^ {- (m + k) / n}),
$$

while $\begin{array} { r } { \sum _ { k < \omega } \left[ 2 ^ { - ( m + k ) / n } \right] ^ { n } = 2 ^ { - ( m - 1 ) } < \varepsilon , } \end{array}$ 

To see that $\mathbb { R } ^ { n } \setminus G \in { \mathcal { M } }$ notice that 

$$
\mathbb {R} ^ {n} \setminus G = \mathbb {R} ^ {n} \setminus \bigcap_ {m <   \omega} G _ {m} = \bigcup_ {m <   \omega} \left(\mathbb {R} ^ {n} \setminus G _ {m}\right)
$$

and each of the sets $\mathbb { R } ^ { n } \backslash G _ { m }$ is closed and nowhere dense, since $G _ { m }$ is open and dense.  

To continue our journey through the special subsets of $\mathbb { R } ^ { n }$ we need the following definitions and constructions. For a σ-ideal I on a set X define a binary relation $\sim _ { \tau }$ on ${ \mathcal { P } } ( X )$ by 

$$
A \sim_ {\mathcal {I}} B \Leftrightarrow A \triangle B \in \mathcal {I}.
$$

Notice the following easy facts. 

Proposition 6.3.2 Let I be a σ-ideal on X. 

(i) For every $A , B \subset X$ 

$A \sim _ { \mathcal { T } } B$ if and only if $A \setminus D = B \setminus D$ for some $D \in \mathcal { T }$ 

(ii) $\sim _ { \mathcal { T } }$ is an equivalence relation on ${ \mathcal { P } } ( X )$ 

(iii) $I f A \sim _ { \cal { T } }$ B then $X \setminus A \sim _ { \mathcal { T } } X \setminus B$ 

(iv) If $A _ { n } \sim _ { \cal T } B _ { n }$ for every $n < \omega$ then $\begin{array} { r } { \bigcup _ { n < \omega } A _ { n } \sim _ { \mathcal { T } } \bigcup _ { n < \omega } B _ { n } } \end{array}$ 

Proof (i) If $A \sim _ { \mathcal { T } } B$ then $D = A \triangle B \in \mathcal { T }$ and $A \setminus D = B \setminus D$ . Conversely, if $A \setminus D = B \setminus D$ for some $D \in \mathcal { T }$ then $A \triangle B \subset D \in \mathcal { T }$ 

(ii) It is easy to see that $A \sim _ { \mathcal { T } } A$ and that $A \sim _ { \mathcal { T } } B$ implies $B \sim _ { \mathcal { T } } A$ for every $A , B \subset X$ . Now, if $A \sim _ { \mathcal { T } } B$ and $B \sim _ { \mathbb { Z } } C$ then $A \setminus D = B \setminus D$ and $B \backslash E = C \backslash E$ for some $D , E \in { \mathcal { T } }$ . So $A \backslash ( D \cup E ) = B \backslash ( D \cup E ) = C \backslash ( D \cup E )$ and $D \cup E \in { \mathcal { T } }$ . So $A \sim _ { \mathbb { Z } } C$ 

(iii) If $A \sim _ { \mathcal { T } }$ B then $A \backslash D = B \backslash D$ for some $D \in \mathcal { T }$ and so $( X \backslash A ) \backslash D =$ $( X \setminus B ) \setminus D$ . Hence $X \setminus A \sim _ { \mathcal { T } } X \setminus B$ 

(iv) Let $A _ { n } , B _ { n } \subset X$ be such that $A _ { n } \sim _ { \cal T } B _ { n }$ for every $n < \omega$ and let $D _ { n } \in \mathcal { T }$ be such that $A _ { n } \backslash D _ { n } = B _ { n } \backslash D _ { n }$ for $n < \omega$ . Then $\begin{array} { r } { D = \bigcup _ { n < \omega } D _ { n } \in \mathbb { Z } } \end{array}$ and so $\begin{array} { r } { \bigcup _ { n < \omega } A _ { n } \setminus D = \bigcup _ { n < \omega } B _ { n } \setminus D } \end{array}$ . Therefore $\begin{array} { r } { \bigcup _ { n < \omega } A _ { n } \sim _ { \mathcal { T } } \bigcup _ { n < \omega } B _ { n } . ~ \big \Pi } \end{array}$ 

Theorem 6.3.3 Let I be a σ-ideal on X and let ${ \mathcal { A } } \subset { \mathcal { P } } ( X )$ be nonempty. The family 

$$
\mathcal {A} [ \mathcal {I} ] = \{A \triangle D: A \in \mathcal {A} \& D \in \mathcal {I} \}
$$

forms a σ-algebra on X if and only if 

(1) $X \setminus A \in { \mathcal { A } } [ { \mathcal { T } } ]$ for every $A \in { \mathcal { A } }$ , and 

(2) $\textstyle \bigcup _ { n < \omega } A _ { n } \in { \mathcal { A } } [ { \mathcal { T } } ]$ provided $A _ { n } \in { \mathcal { A } }$ for every $n < \omega$ 

In particular, if A is a σ-algebra on X then $A [ \mathcal { T } ]$ is a σ-algebra generated $b y \mathcal { A } \cup \mathcal { T }$ 

Proof The implication ⇒ as well as the additional part of the theorem are obvious. To prove the other implication we have to prove that $A [ \mathcal { T } ]$ is closed under complements and under countable unions. First notice that 

$$
C \sim_ {\mathcal {I}} B \& B \in \mathcal {A} [ \mathcal {I} ] \Rightarrow C \in \mathcal {A} [ \mathcal {I} ],\tag{6.10}
$$

since $B \in A [ \mathcal { T } ]$ implies that $B \sim _ { \mathcal { Z } } A$ for some $A \in A .$ , so $C \sim _ { \mathcal { Z } } A$ and $C = A \triangle D \in { \mathcal { A } } [ { \mathcal { T } } ]$ , where $D = A \triangle C \in { \mathcal { T } }$ 

Now, if $B = A \triangle D$ for some $A \in { \mathcal { A } }$ and $D \in \mathcal { T }$ then $B \triangle A \in { \mathcal { T } }$ and, by Proposition 6.3.1(iii), $X \backslash B \sim _ { \mathbb { Z } } X \backslash A$ . But, by our assumption, $X \backslash A \in { \mathcal { A } } [ \mathcal { T } ]$ and so, by (6.10), $X \setminus B \in { \mathcal { A } } [ { \mathcal { T } } ]$ 

Similarly, if $B _ { n } = A _ { n } \triangle D _ { n }$ for some $A _ { n } \in { \mathcal { A } }$ and $D _ { n } \in \mathcal { T }$ then $B _ { n } \triangle A _ { n } \in$ $\mathcal { T }$ and, by Proposition 6.3.1(iv), $\begin{array} { r } { \bigcup _ { n < \omega } B _ { n } \sim _ { \mathcal { T } } \bigcup _ { n < \omega } A _ { n } } \end{array}$ . Since $\textstyle \bigcup _ { n < \omega } A _ { n } \in$ $A [ \mathcal { T } ]$ , condition (6.10) implies that $\textstyle { \bigcup _ { n < \omega } B _ { n } \in \mathcal { A } [ \dot { \mathcal { T } } ] }$  

The most important σ-algebras on $\mathbb { R } ^ { n }$ generated as in Theorem 6.3.3 are the σ-algebras ${ \mathcal { L } } = B o r [ { \mathcal { N } } ]$ of Lebesgue-measurable sets and the $\sigma -$ algebra $B a i r e = B o r [ \mathcal { M } ]$ of sets with the Baire property, where $B o r$ stands for the σ-algebra of Borel subsets of $\mathbb { R } ^ { n }$ . Both these families are very rich. In fact, without use of the axiom of choice we cannot prove the existence of a subset of $\mathbb { R } ^ { n }$ that does not have the Baire property. A similar theorem for the family $\mathcal { L }$ of all measurable sets can also be proved. 

In what follows we prove that there is a subset of $\mathbb { R } ^ { n }$ that is nonmeasurable and does not have the Baire property. For this, however, we need some structural theorems about Baire and ${ \mathcal { L } } .$ 

Theorem 6.3.4 Baire $\ d \cdot = \tau [ \mathcal { M } ] = \{ U \triangle M$ : U is open in $\mathbb { R } ^ { n }$ and $M \in \mathcal { M } \}$ 

Proof This follows immediately from Theorem 6.3.3 since a union of open sets is open and since for every open set A its complement $F = \mathbb { R } ^ { n } \setminus A$ is closed, and $F = \operatorname { i n t } ( F ) \cup ( F \setminus \operatorname { i n t } ( F ) )$ , where $F \setminus \operatorname { i n t } ( F )$ is closed and nowhere dense.  

The similar characterization for L is more complicated and is given by the next theorem. 

Theorem 6.3.5 For every $A \in { \mathcal { L } }$ there exists an $F _ { \sigma }$ set F and $a ~ G _ { \delta }$ set G such that $F \subset A \subset G$ and $G \setminus F \in { \mathcal { N } }$ 

In particular, 

$$
\begin{array}{r c l} \mathcal {L} & = & \{G \triangle N \colon G \text {is} G _ {\delta} \text {in} \mathbb {R} ^ {n} \text {and} N \in \mathcal {N} \} \\ & = & \{F \triangle N \colon F \text {is} F _ {\sigma} \text {in} \mathbb {R} ^ {n} \text {and} N \in \mathcal {N} \}. \end{array}
$$

The property described in this theorem is called the regularity of the family $\mathcal { L }$ and is a basic fact about Lebesgue measure. We will leave it here without proof (see, e.g., Royden 1988). 

Theorem 6.3.6 If $A \in \mathcal { L } \backslash \mathcal { N }$ or $A \in B a i r e \backslash \mathcal { M }$ then there exists a perfect set P such that $P \subset A$ 

Proof First assume that $A \in \mathcal { L } \backslash \mathcal { N }$ . Then, by Theorem 6.3.5, there exists an $F _ { \sigma }$ set $F$ such that $F \subset A$ and $A \setminus F \in { \mathcal { N } }$ . Thus $F \in { \mathcal { L } } \setminus N$ . Let $F = \textstyle \bigcup _ { n < \omega } F _ { n }$ , where the sets $F _ { n }$ are closed in R<sup>n</sup>. Notice that at least one of the sets $F _ { n }$ must be uncountable, since otherwise $F$ would be at most countable and then it would belong to N. So let $F _ { n }$ be uncountable. Then, by the Cantor–Bendixson theorem (Theorem 6.2.4), there is a perfect set $P \subset F _ { n } \subset F \subset A$ 

Now assume that $A \in B a i r e \backslash \mathcal { M }$ and let $A = U \triangle S$ for some nonempty open set U and $S \in { \mathcal { M } }$ . Let $\textstyle S = \bigcup _ { n < \omega } S _ { n }$ for some $S _ { n } \in \mathcal { N D }$ 

As in Theorem 6.2.3 we will use a “tree-construction” argument to define a family $\{ U _ { s } \subset U \colon s \in 2 ^ { < \omega } \}$ of nonempty open sets; that is, the construction will be done by induction on the length $| s |$ of a sequence s. 

We choose a bounded $U _ { \emptyset }$ such that c $. ( U _ { \varnothing } ) \subset U \setminus S _ { 0 }$ and continue the induction, maintaining the following condition to be satisfied for every $s \in 2 ^ { < \omega }$ : 

(I) $U _ { s 0 }$ and $U _ { s 1 }$ are open balls such that 

$$
\operatorname{cl} (U _ {s 0}) \cap \operatorname{cl} (U _ {s 1}) = \emptyset , \quad \operatorname{cl} (U _ {s 0}) \cup \operatorname{cl} (U _ {s 1}) \subset U _ {s} \setminus S _ {| s |}.
$$

To make an inductive step assume that $U _ { s }$ is already constructed. Since $\operatorname { c l } ( S _ { \left| s \right| } ) \in \mathcal { N } \mathcal { D }$ we have $U _ { s } \setminus \mathrm { c l } ( S _ { | s | } ) \ne \emptyset$ and we can find two open disjoint balls in $U _ { s } \ \backslash \ \mathrm { c l } ( S _ { | s | } )$ . Decreasing their radii, if necessary, we can satisfy condition (I). This completes the construction. 

Now let $F _ { n } = \bigcup \{ \operatorname { c l } ( U _ { s } ) \colon s \in 2 ^ { < \omega } , \quad | s | = n \}$ and $\textstyle F = \bigcap _ { n < \omega } F _ { n }$ . By our construction, $F \subset U$ and $F _ { n } \cap S _ { n } \ : = \ : \emptyset$ for every $n \ < \ \omega$ Hence, $F \subset U \backslash S \subset A$ . Also, each of the sets $F _ { n }$ is compact, being a finite union of closed bounded sets. Thus F is compact. To finish the proof it is enough to show that F is uncountable, since then, by the Cantor–Bendixson theorem, there is a perfect set $P \subset F \subset A$ 

To see this, for every $f \in 2 ^ { \omega }$ consider a set $\begin{array} { r } { F _ { f } ~ = ~ \bigcap _ { n < \omega } \operatorname { c l } ( U _ { f \mid n } ) ~ \subset \ \complement } \end{array}$ $F$ . Notice that, by Theorem 3.3.1, each set $F _ { f }$ is nonempty. Note also that the sets $\{ F _ { f } \colon f \in 2 ^ { \omega } \}$ are pairwise disjoint. Indeed, if $f , g \in 2 ^ { \omega }$ are diferent, n = min $\{ i < \omega \colon f ( i ) \neq g ( i ) \}$ , and $s = f | _ { n } ~ = ~ g | _ { n }$ then $F _ { f } \cap F _ { g } \subset \operatorname { c l } ( U _ { s 0 } ) \cap \operatorname { c l } ( U _ { s 1 } ) = \emptyset$ . Now let $c \colon 2 ^ { \omega }  F$ be a choice function for the family $\{ F _ { f } \colon f \in 2 ^ { \omega } \}$ , that is, $c ( f ) \in F _ { f }$ for every $f \in 2 ^ { \omega }$ . Then c is one-to-one and so $\left| 2 ^ { \omega } \right| \leq | F |$ , proving that F is indeed uncountable. 

This finishes the proof. 

We conclude this section with the following two theorems. 

Theorem 6.3.7 There exists a set $B \subset \mathbb { R } ^ { n }$ such that neither B nor $\mathbb { R } ^ { n } \backslash B$ contains any perfect subset. 

Proof First notice that the family $\mathcal { F }$ of all perfect subsets of $\mathbb { R } ^ { n }$ has $\mathrm { c a r d i n a l i t y } \le { \mathfrak { c } }$ , since $\mathcal { F } \subset B o r$ and $| B o r | = { \mathfrak { c } }$ 

Let $\mathcal { F } = \{ P _ { \xi } \colon \xi < \mathfrak { c } \}$ . By transfinite induction on $\xi < \mathfrak { c }$ define the sequences $\langle a _ { \xi } : \xi < { \mathfrak { c } } \rangle$ and $\left. b _ { \xi } \colon \xi \ < \ \mathfrak { c } \right.$ by choosing in step $\xi < { \mathfrak { c } }$ points $a _ { \xi } \neq b _ { \xi }$ from $\mathbb { R } ^ { n }$ such that 

$$
a _ {\xi}, b _ {\xi} \in P _ {\xi} \setminus (\{a _ {\zeta}: \zeta <   \xi \} \cup \{b _ {\zeta}: \zeta <   \xi \}).
$$

This can be done since 

$$
\left| \left\{a _ {\zeta}: \zeta <   \xi \right\} \cup \left\{b _ {\zeta}: \zeta <   \xi \right\} \right| = 2 \otimes | \xi | <   \mathfrak {c}
$$

and, by Theorem 6.2.3, $| P _ { \xi } | = { \mathfrak { c } } .$ . This finishes the construction. 

Now define $B = \{ a \varepsilon \colon \xi < { \mathfrak { c } } \}$ . Then for every perfect set P there is a $\xi < { \mathfrak { c } }$ such that $P = P _ { \varepsilon }$ . Hence $a _ { \xi } \in P \cap B$ and $b _ { \xi } \in P \cap ( \mathbb { R } ^ { n } \setminus B )$ . Thus $P \ \mathcal { L } \ B$ and $P \neq \mathbb { R } ^ { n } \setminus B$  

The set B from Theorem 6.3.7 is called a Bernstein set. 

Theorem 6.3.8 A Bernstein subset B of $\mathbb { R } ^ { n }$ neither is measurable nor has the Baire property. 

Proof To obtain a contradiction assume that $B \in { \mathcal { L } }$ . Then, by Theorem $6 . 3 . 6 , \ B \in \mathcal N$ . Similarly, $\mathbb { R } ^ { n } \setminus B \in { \mathcal { L } }$ and $\mathbb { R } ^ { n } \setminus B \in \mathcal { N }$ . But then $\mathbb { R } ^ { n } = B \cup ( \mathbb { R } ^ { n } \setminus B ) \in \mathcal { N }$ , which is false. So $B \notin { \mathcal { L } }$ 

The proof that $B \notin$ Baire is exactly the same. 

## EXERCISES

1 Show that there exists a Bernstein set B such that $B + B = \mathbb { R }$ , where $B + B = \{ b _ { 0 } + b _ { 1 } \colon b _ { 0 } , b _ { 1 } \in B \}$ 

2 Show that there exists a Bernstein set B such that $B + B$ is also a Bernstein set. 

# Chapter 7

# Strange real functions

This chapter is designed to help the reader to master the technique of recursive definitions. Thus, most of the examples presented will involve constructions by transfinite induction. 

## 7.1 Measurable and nonmeasurable functions

Let B be a σ-algebra on $\mathbb { R } ^ { n }$ . A function $f \colon  { \mathbb { R } } ^ { n } \to  { \mathbb { R } }$ is said to be a $B _ { - }$ measurable function if $f ^ { - 1 } ( U ) \in B$ for every open set $U \subset \mathbb { R }$ . Notice that if f is B-measurable then $f ^ { - 1 } ( B ) \in B$ for every Borel set $B \subset \mathbb { R }$ . This is the case since the family $\{ B \subset \mathbb { R } \colon f ^ { - 1 } ( B ) \in \mathcal { B } \}$ is a σ-algebra containing all open sets. 

We will use this notion mainly for the σ-algebras of Borel, Lebesguemeasurable, and Baire subsets of $\mathbb { R } ^ { n }$ , respectively. In each of these cases B-measurable functions will be termed, respectively, as Borel functions (or Borel-measurable functions), measurable functions (or Lebesgue-measurable functions), and Baire functions (or Baire-measurable functions). Clearly, every continuous function is Borel-measurable and every Borel-measurable function is measurable and Baire. 

A function $f \colon  { \mathbb { R } } ^ { n } \to  { \mathbb { R } }$ is non-Borel (or non–Borel-measurable) if it is not Borel. Similarly, we define non-Baire(-measurable) functions and non-(Lebesgue-)measurable functions. 

Also recall that the characteristic function $\chi _ { A }$ of a subset A of a set X is defined by putting $\chi _ { A } ( x ) = 1 { \mathrm { ~ i f ~ } } x \in A$ and $\chi _ { A } ( x ) = 0$ for $x \in X \setminus A$ 

The first theorem is a corollary to Theorems 6.3.7 and 6.3.8. 

Theorem 7.1.1 The characteristic function $\chi _ { B }$ of a Bernstein subset B of $\mathbb { R } ^ { n }$ is neither a measurable nor a Baire function. In particular, there exists a nonmeasurable, non-Baire function from $\mathbb { R } ^ { n }$ to R. 

Proof The set $( \boldsymbol { \chi } _ { B } ) ^ { - 1 } ( \{ 1 \} ) = B$ neither is measurable nor has the Baire property.  

Let us recall that the Fubini–Tonelli theorem says that for a measurable function $f \colon  { \mathbb { R } } ^ { 2 } \to  { \mathbb { R } }$ that is either integrable or nonnegative we have 

$$
\iint f d m _ {2} = \int \left(\int f _ {x} d m _ {1}\right) d m _ {1} = \int \left(\int f ^ {y} d m _ {1}\right) d m _ {1},
$$

where $m _ { 2 }$ and $m _ { 1 }$ stand for the Lebesgue measures on $\mathbb { R } ^ { 2 }$ and R, respectively, and $f _ { x } , f ^ { y } \colon  { \mathbb { R } } \to  { \mathbb { R } }$ are defined by $f _ { x } ( y ) = f ( x , y )$ and $f ^ { y } ( x ) =$ $f ( x , y )$ . The integrals $\textstyle { \int } \left( \int f _ { x } d m _ { 1 } \right)$ $d m _ { 1 }$ and $\int \left( \int f ^ { y } d m _ { 1 } \right)$ dm are called * 	* * 	*iterated integrals. Thus, the Fubini–Tonelli theorem tells us for measurable functions what for the continuous functions is taught in every multivariate calculus course: A two-dimensional integral is equal to both iterated integrals. But what if the function f is nonmeasurable? Then we can’t talk about the integral $\int \int f d m _ { 2 }$ . However, it is still possible that both iterated **integrals exist. Must they be equal? The next theorem, due to Sierpi´nski (1920), gives a negative answer to this question. 

Theorem 7.1.2 Ifthe continuum hypothesis holds then there exists a function $f \colon [ 0 , 1 ] ^ { 2 }  [ 0 , 1 ]$ such that $f _ { x } d m _ { 1 } = 1$ and $f ^ { y } d m _ { 1 } = 0$ for all $x , y \in [ 0 , 1 ]$ . In particular, 

$$
\int \left(\int f _ {x} d m _ {1}\right) d m _ {1} = 1 \quad a n d \quad \int \left(\int f ^ {y} d m _ {1}\right) d m _ {1} = 0.
$$

Proof Let A be as in Theorem 6.1.8, put $B = A \cap [ 0 , 1 ] ^ { 2 }$ , and define $f = \chi _ { B }$ . Notice that $| B ^ { y } | \le \omega$ and $| ( [ 0 , 1 ] ^ { 2 } \setminus B ) _ { x } | \leq \omega$ for all $x , y \in [ 0 , 1 ]$ Thus $f ^ { y } ( x ) = 0$ for all but countably many $x \in \mathbb { R }$ , and so $\begin{array} { r } { \int f ^ { y } d m _ { 1 } = } \end{array}$ $\begin{array} { r } { \int 0 d m _ { 1 } = 0 } \end{array}$ . Similarly, for every $x \in [ 0 , 1 ]$ we have $f _ { x } ( y ) = 1$ for all but *countably many $y \in [ 0 , 1 ]$ . Thus $\begin{array} { r } { \int f _ { x } d m _ { 1 } = \int _ { [ 0 , 1 ] } 1 d m _ { 1 } = 1 } \end{array}$  

A set $B \subset [ 0 , 1 ] ^ { 2 }$ for which the function $f = \chi _ { B }$ satisfies Theorem 7.1.2 is usually called a 0-1 set. Its existence is not equivalent to the continuum hypothesis; that is, it might exist when the continuum hypothesis fails. $\mathrm { O n }$ the other hand, the existence of the function f from Theorem 7.1.2 cannot be proved in ZFC, which has been shown by H. Friedman (1980) and, independently, by C. Freiling (1986). 

## EXERCISE

1 Prove that there exists a function $f \colon  { \mathbb { R } } \ \to \  { \mathbb { R } }$ such that $f ^ { - 1 } ( r )$ is a Bernstein set for every $r \in \mathbb { R }$ 

## 7.2 Darboux functions

To motivate what follows let us recall one of the most fundamental theorems of calculus – the intermediate value theorem. It tells us that every continuous function $f : \mathbb { R } \to \mathbb { R }$ has the following property: 

(DP) For every $a < b$ and every number y between $f ( a )$ and $f ( b )$ there is an $x \in ( a , b )$ such that $f ( x ) = y$ 

The functions satisfying property (DP) form an important class of functions known as Darboux functions. In particular, we say that a function $f : \mathbb { R } \to$ R has the Darboux property (or is a Darboux function) if it satisfies property (DP). Thus, the intermediate value theorem says that every continuous function $f \colon  { \mathbb { R } } \to  { \mathbb { R } }$ has the Darboux property. 

Not every Darboux function, however, is continuous. For example, the function $f ( x ) = \sin ( 1 / x )$ for $x \neq 0$ and $f ( 0 ) = 0$ is a discontinuous Darboux function. The next theorem tells us that there are also everywherediscontinuous Darboux functions (that is, Darboux functions that are discontinuous at every point). For this we will need one more definition. We say that a function $f \colon  { \mathbb { R } } \to  { \mathbb { R } }$ is strongly Darboux if 

(SD) for every $a < b$ and every number y there is an $x \in ( a , b )$ such that $f ( x ) = y .$ 

Thus f is strongly Darboux if $f [ ( a , b ) ] = \mathbb { R }$ for every $a < b$ . Clearly, every strongly Darboux function is Darboux and everywhere discontinuous. 

Theorem 7.2.1 There exists a strongly Darboux function $f \colon  { \mathbb { R } } \to  { \mathbb { R } }$ . In particular, f is Darboux and everywhere discontinuous. 

Proof The set A constructed in Theorem 6.1.1 is the graph of the desired function $f .$  

The next theorem is a generalization of Theorem 7.2.1. 

Theorem 7.2.2 Let G be a family of real functions, $\mathcal { G } \subset \mathbb { R } ^ { \mathbb { R } }$ , with $| \mathcal { G } | \leq \mathfrak { c }$ Then there exists a function $f \colon  { \mathbb { R } } \to  { \mathbb { R } }$ such that $f + g$ is strongly Darboux for every $g \in { \mathcal { G } }$ 

Proof Let $\mathcal { F } = \{ \langle g , I , r \rangle \colon g \in \mathcal { G } \ \& \ r \in \mathbb { R } \ \& \ I = ( a , b )$ for some $a < b \}$ Then $| { \mathcal F } | = { \mathfrak c } ,$ , since ${ \mathfrak { c } } = | \mathbb { R } | \leq | { \mathcal { F } } | \leq | { \mathcal { G } } | \otimes | \mathbb { R } ^ { 3 } | = { \mathfrak { c . \ L e t \ } } \{ \langle g _ { \xi } , I _ { \xi } , r _ { \xi } \rangle \colon \xi < { \mathfrak { c } } \}$ be an enumeration of family F. By transfinite induction define a sequence $\{ x _ { \xi } \colon \xi < \mathfrak { c } \}$ such that 

$$
x _ {\xi} \in I _ {\xi} \setminus \{x _ {\zeta}: \zeta <   \xi \}.
$$

Such a choice can be made since $| I _ { \xi } | = | \mathbb { R } | = \mathfrak { c } > | \xi | \ge | \{ x _ { \zeta } \colon \zeta < \xi \} |$ for every $\xi < { \mathfrak { c } }$ 

Define $f ( x _ { \xi } ) = r _ { \xi } - g _ { \xi } ( x _ { \xi } )$ and extend it to all of R arbitrarily. Notice that it has the desired property, since for every nonempty interval $( a , b )$ , every $r \in \mathbb { R }$ , and every $g \in { \mathcal { G } }$ there exists a $\xi < { \mathfrak { c } }$ such that $\langle g _ { \xi } , I _ { \xi } , r _ { \xi } \rangle =$ $\langle g , ( a , b ) , r \rangle$ , and so 

$$
r = r _ {\xi} = f (x _ {\xi}) + g _ {\xi} (x _ {\xi}) \in (f + g _ {\xi}) [ I _ {\xi} ] = (f + g) [ (a, b) ].
$$

Notice that Theorem 7.2.2 generalizes Theorem 7.2.1, since we can assume that the function that is identically zero belongs to $\mathcal { G }$ . In particular, the function f in Theorem 7.2.2 can be chosen to be strongly Darboux. 

Corollary 7.2.3 Let $\mathcal { G }$ be a family of real functions such that $| \mathcal { G } | \leq \mathfrak { c } ,$ Then there exists a (strongly) Darboux function $f : \mathbb { R } \to \mathbb { R }$ such that $f + g$ is (strongly) Darboux for every $g \in { \mathcal { G } }$ 

Another way to look at Corollary 7.2.3 is to use the language of cardinal functions as follows. Let D stand for the family of all Darboux functions from R to R and let $\mathcal { A } ( \mathcal { D } )$ be the minimal cardinality of a family $\mathcal { G }$ for which Corollary 7.2.3 fails, that is, 

$$
\mathcal {A} (\mathcal {D}) = \min \{| \mathcal {G} |: \forall f \in \mathbb {R} ^ {\mathbb {R}} \exists g \in \mathcal {G} (f + g \notin \mathcal {D}) \}.
$$

Notice that the set $\{ | \mathcal { G } | : \forall f \in \mathbb { R } ^ { \mathbb { R } } \ \exists g \in \mathcal { G } \ ( f + g \ \notin \ \mathcal { D } ) \}$ is not empty, since $| \mathbb { R } ^ { \mathbb { R } } | = { \mathfrak { c } } ^ { \mathfrak { c } } = 2 ^ { \mathfrak { c } }$ belongs to this set: For every $f \in \mathbb { R } ^ { \mathbb { R } }$ there exists a $g \in \mathcal { G } = \mathbb { R } ^ { \mathbb { R } }$ such that $f + g$ is equal to any fixed function $h ,$ , and such that h can be chosen to be not Darboux. So $\mathcal { A } ( \mathcal { D } ) \leq 2 ^ { \mathfrak { c } }$ . In this language Corollary 7.2.3 can be stated as follows: 

$$
\mathfrak {c} <   \mathcal {A} (\mathcal {D}) \leq 2 ^ {\mathfrak {c}}.\tag{7.1}
$$

If $2 ^ { \mathfrak { c } } = { \mathfrak { c } } ^ { + }$ , which follows from the generalized continuum hypothesis, then $\mathcal { A } ( \mathcal { D } ) = 2 ^ { \mathfrak { c } }$ . However, this equation cannot be proved in ZFC alone. It has been proved by K. Ciesielski and A. W. Miller (1994–5) that (7.1) is essentially everything that can be proved in ZFC about $\mathcal { A } ( \mathcal { D } )$ 

In what follows we will consider some other generalizations of Theorem 7.2.1. We start by noticing that the sum of a Darboux function and a continuous function does not have to be Darboux. To see it, modify the proof of Theorem 7.2.2 to get a strongly Darboux function $f$ such that $g ( x ) = f ( x ) - x$ is not Darboux, by choosing 

$$
x _ {\xi} \in I _ {\xi} \setminus \left(\left\{x _ {\zeta}: \zeta <   \xi \right\} \cup \left\{r _ {\xi} \right\}\right)
$$

and defining $f ( x _ { \xi } ) = r _ { \xi }$ . Then $f ( x _ { \xi } ) \neq x _ { \xi }$ and we can extend $f$ to all of R to have $f ( x ) \neq x$ for all $x \in \mathbb { R }$ . So $g ( x ) = f ( x ) - x \neq 0$ for every $x \in \mathbb { R }$ and Proposition 7.2.4, stated next, implies that $g$ is not Darboux. 

Proposition 7.2.4 If f is strongly Darboux, then for every continuous function $g _ { \mathrm { ; } }$ 

$$
f + g \text {is strongly Darboux iff} f + g \text {is Darboux.}
$$

Proof Implication ⇒ is obvious. The other implication follows from the fact that on any interval $\boldsymbol { I } = ( c , d )$ , with $c < d ,$ , the continuous function $g$ is bounded, while $f [ I ] = \mathbb { R }$ . So $f + g$ must be unbounded from below and from above. In particular, for every $y \in \mathbb R$ there exist $A < y < B$ and $a , b \in I$ such that $( f + g ) ( a ) = A$ and $( f + g ) ( b ) = B$ . Thus there exists an x between a and b with $( f + g ) ( x ) = y .$ , since $f + g$ is Darboux. Hence $( f + g ) [ I ] = \mathbb { R }$  

The next theorem, due to Kirchheim and Natkaniec (1990–1), generalizes the preceding observation. It concerns continuous nowhere-constant functions, that is, continuous functions that are not constant on any open nonempty interval. 

Theorem 7.2.5 If the continuum hypothesis holds then there is a strongly Darboux function f such that $f + h$ is not Darboux for every continuous nowhere-constant function h. 

Proof Let $\{ h _ { \xi } \colon \xi ~ < ~ { \mathfrak { c } } \}$ be an enumeration of all continuous nowhereconstant functions from R to R. Notice that for any such function h the set $h ^ { - 1 } ( r )$ is closed and nowhere dense for every $r \in \mathbb { R }$ 

By Proposition 7.2.4 it is enough to find $f : \mathbb { R } \to \mathbb { R }$ such that 

$$
\forall \xi <   \mathfrak {c} \exists r _ {\xi} \in \mathbb {R} \forall x \in \mathbb {R} (f (x) + h _ {\xi} (x) \neq r _ {\xi}).\tag{7.2}
$$

For this we will construct sequences $\{ x _ { \xi } \in \mathbb { R } \colon \xi < { \mathfrak { c } } \} , \ \{ y _ { \xi } \in \mathbb { R } \colon \xi < { \mathfrak { c } } \}$ , and $\{ r _ { \xi } \in \mathbb { R } \colon \xi < { \mathfrak { c } } \}$ such that the function f defined by 

$$
f (x _ {\xi}) = y _ {\xi}\tag{7.3}
$$

is strongly Darboux and satisfies condition (7.2). As we know from Theorems 7.2.1 and 7.2.2, it is relatively easy to construct the sequences $\{ x _ { \xi } \}$ and $\{ y _ { \xi } \}$ such that f defined by (7.3) is strongly Darboux. In previous constructions, however, we did not have to worry about $\{ x _ { \xi } \colon \xi < \mathfrak { c } \}$ being equal to R, since any extension of the part of $f$ given by (7.3) was still strongly Darboux. But this time, we also have to take care of condition (7.2), and the extension may fail to have this property. To avoid this problem we will arrange our construction to have 

$$
\{x _ {\xi}: \xi <   \mathfrak {c} \} = \mathbb {R}.\tag{7.4}
$$

Now let $S$ and $T$ be subsets of c of cardinality c. Let $\{ s _ { \xi } \colon \xi \in S \}$ be an enumeration of R and let $\{ \langle I _ { \xi } , t _ { \xi } \rangle \colon \xi \in T \}$ be an enumeration of the family $\mathcal { F } = \{ \langle I , t \rangle \colon t \in \mathbb { R } \ \& \ I = ( a , b )$ for some $a < b \}$ . To satisfy (7.4) it is enough to have 

(S1) $x _ { \xi } = s _ { \xi }$ for every $\xi \in S$ 

To make sure that f is strongly Darboux it is enough to proceed as in Theorems 7.2.1 and 7.2.2; that is, for every $\xi \in T$ choose 

$$
x _ {\xi} \in I _ {\xi} \setminus \{x _ {\zeta}: \zeta <   \xi \}\tag{7.5}
$$

and put 

(T1) $y _ { \xi } = t _ { \xi } .$ 

Notice, however, that for $s _ { \xi } \notin I _ { \xi }$ conditions (S1) and (7.5) cannot be satisfied simultaneously. To avoid this problem we will assume that the sets $S$ and $T$ are disjoint. We can also assume that $S \cup T = { \mathfrak { c } } .$ 

Property (7.2) will hold if we construct the sequences in such a way that for every $\xi < { \mathfrak { c } }$ 

$$
\forall \zeta <   \xi \forall \eta <   \xi (y _ {\eta} + h _ {\zeta} (x _ {\eta}) \neq r _ {\zeta}).\tag{7.6}
$$

To preserve this condition while constructing $x _ { \xi } , y _ { \xi }$ , and $r _ { \xi }$ we will have to choose $r _ { \xi }$ such that $y _ { \eta } + h _ { \xi } ( x _ { \eta } ) \neq r _ { \xi }$ for every $\eta < \xi$ , that is, pick 

$$
(\star) \quad r _ {\xi} \in \mathbb {R} \setminus \{y _ {\eta} + h _ {\xi} (x _ {\eta}) \colon \eta <   \xi \},
$$

and choose $x _ { \xi }$ and $y _ { \xi }$ such that 

$$
y _ {\xi} + h _ {\zeta} (x _ {\xi}) \neq r _ {\zeta} \quad \text { for   every } \quad \zeta \leq \xi .\tag{7.7}
$$

Now for $\xi \in T$ we have no freedom in choosing y since, by (T1), $y _ { \xi } = t _ { \xi }$ . But to satisfy (7.7) it is enough to choose $x _ { \xi } \overset { \cdot } { \in } \bar { \bigcup } _ { \zeta \leq \xi } h _ { \zeta } ^ { - 1 } ( \bar { r _ { \zeta } } - y _ { \xi } )$ Combining this with (7.5) we need only choose 

(T2) x<sub>ξ</sub> ∈ I<sub>ξ</sub> \ {x<sub>ζ</sub> : ζ < ξ} ∪ {h<sup>−1</sup><sub>ζ</sub> (r<sub>ζ</sub> − y<sub>ξ</sub>) : ζ ≤ ξ} for every $\xi \in T$ 

For $\xi \in S$ , by (S1), we have $x _ { \xi } = s _ { \xi }$ . If $x _ { \xi } = x _ { \zeta }$ for some $\zeta < \xi$ then, by (7.3), we have to define 

$$
y _ {\xi} = y _ {\zeta}.\tag{S2}
$$

But then conditions (7.6) and (7.7) will be preserved. On the other hand, if $x _ { \xi } \neq x _ { \zeta }$ for every $\zeta < \xi$ , in order to maintain $( 7 . 7 )$ it is enough to choose 

$$
y _ {\xi} \in \mathbb {R} \setminus \{r _ {\eta} - h _ {\eta} (x _ {\xi}) \colon \eta \leq \xi \}.\tag{S3}
$$

The foregoing discussion shows that the function f can be constructed if we can construct the sequences $\{ x _ { \xi } \in \mathbb { R } \colon \xi < { \mathfrak { c } } \} , \ \{ y _ { \xi } \in \mathbb { R } \colon \xi < { \mathfrak { c } } \}$ , and $\{ r _ { \xi } \in \mathbb { R } \colon \xi < { \mathfrak { c } } \}$ such that the following conditions hold for every $\xi < { \mathfrak { c } } \colon$ 

$$
(\star) \quad r _ {\xi} \in \mathbb {R} \setminus \{y _ {\eta} + h _ {\xi} (x _ {\eta}) \colon \eta <   \xi \};
$$

$$
y _ {\xi} = t _ {\xi} \text {   for   } \xi \in T; \tag {T1}
$$

$$
\text {(T2)} \quad x _ {\xi} \in I _ {\xi} \setminus \left(\{x _ {\zeta}: \zeta <   \xi \} \cup \bigcup \{h _ {\zeta} ^ {- 1} (r _ {\zeta} - y _ {\xi}): \zeta \leq \xi \}\right) \text {for} \xi \in T;
$$

$$
x _ {\xi} = s _ {\xi} \text {   for   } \xi \in S; \tag {S1}
$$

$$
\text {(S2)} \quad y _ {\xi} = y _ {\zeta} \text { for } \xi \in S \text { if } x _ {\xi} = x _ {\zeta} \text { for some } \zeta <   \xi ;
$$

$$
\text {(S3)} \quad y _ {\xi} \in \mathbb {R} \setminus \{r _ {\zeta} - h _ {\zeta} (x _ {\xi}) \colon \zeta \leq \xi \} \text { for } \xi \in S \text { if } x _ {\xi} \neq x _ {\zeta} \text { for all } \zeta <   \xi .
$$

By the recursion theorem it is enough just to argue that such a choice is always possible. 

The possibility of the choices in (G), (T1), (S1), (S2), and (S3) is obvious. The choice of $x _ { \xi }$ in (T2) is possible by the Baire category theorem, since the set $\{ x _ { \zeta } : \zeta < \xi \} \cup \bigcup \{ h _ { \zeta } ^ { - 1 } ( r _ { \zeta } - y _ { \xi } ) : \zeta \leq \xi \}$ is of first category, being an at most countable union of nowhere-dense sets (this is the place where we used the continuum hypothesis!).  

It is worthwhile to mention that the conclusion of Theorem 7.2.5 is not equivalent to the continuum hypothesis. Essentially the same proof works with a weaker additional set-theoretic axiom, known as the additivity of category, that the union of less than continuum many meager sets is still a meager set (see Theorem 8.2.6). However, it has been recently proved by Stepr¯ans (1993) that the conclusion of Theorem 7.2.5 is independent of ZFC set theory. 

## EXERCISES

1 Show that every function $f \colon C \to \mathbb { R }$ on a nowhere-dense subset C of R can be extended to a Darboux function $g \colon { \mathbb { R } }  { \mathbb { R } }$ 

Since there are nowhere-dense subsets C of R of cardinality c, for example, the Cantor set, conclude that the family D of Darboux functions has cardinality $2 ^ { \mathfrak { c } }$ 

## 2 Generalize Theorem 7.2.5 to prove the following:

Let $\mathcal { G }$ be the family of all continuous functions from R to R such that for every $h$ in $\mathcal { G }$ there exists a nonempty open interval I such that $h$ is not constant on any nonempty open subinterval of I. If the continuum hypothesis holds then there exists a strongly Darboux function f such that $f + h$ is not Darboux for every $h \in { \mathcal { G } }$ 

3 Show that if h is a continuous function with the property that every nonempty open interval contains a nonempty open subinterval on which h is constant then $f + h$ is strongly Darboux for every strongly Darboux function $f$ 

Remark: There are continuous nonconstant functions with the property just described. For example, if C is the Cantor set then we can define a function $h \colon [ 0 , 1 ] \to \mathbb { R }$ by $\begin{array} { r } { h ( x ) = \sum _ { n = 1 } ^ { \infty } x _ { n } / 2 ^ { n + 1 } } \end{array}$ , where $\scriptstyle \sum _ { n = 1 } ^ { \infty } x _ { n } / 3 ^ { n } \ =$ $\operatorname* { m a x } ( C \cap [ 0 , x ] )$ and $x _ { n } \in \{ 0 , 2 \}$ 

4 Find uncountable sets $X , Y \subset \mathbb { R } \setminus \mathbb { Q }$ such that for every continuous function $f \colon \mathbb { R } \to \mathbb { R } { \mathrm { ~ i f ~ } } f [ X ] \subset Y$ then f is constant. 

5 Prove the following theorem of Sierpi´nski and Zygmund: There exists a function $f \colon  { \mathbb { R } } \to  { \mathbb { R } }$ such that for every continuous function $g \colon { \mathbb { R } }  { \mathbb { R } }$ the set $\{ x \in \mathbb { R } \colon f ( x ) = g ( x ) \}$ has cardinality less than c. Hint: Use the fact that every continuous function $h \colon X \to \mathbb { R }$ , with $X \subset \mathbb { R }$ , has a continuous extension $\bar { h } \colon G \to \mathbb { R }$ to a $G _ { \delta }$ set $G \subset \mathbb { R }$ . (This can be proved by noticing that the set of all $z \in \mathbb { R }$ for which the limit $\scriptstyle \operatorname* { l i m } _ { x \to z } h ( x )$ does not exist is an $F _ { \sigma } \ \mathrm { s e t . } )$ 

## 7.3 Additive functions and Hamel bases

A function $F \colon  { \mathbb { R } } \to  { \mathbb { R } }$ is an additive function if $F ( x + y ) = F ( x ) + F ( y )$ for every $x , y \in \mathbb { R }$ . Every linear function $F ( x ) = a x$ is clearly additive and continuous, and it is quite easy to see that these are the only continuous additive functions. However, there exist discontinuous additive functions. The first example of such a function was constructed by Hamel, with the use of a Hamel basis, that is, a linear basis of R over Q, which exists by Theorem 4.4.1. For its construction we will need some easy facts. 

For $B \subset \mathbb { R }$ let $\mathrm { L I N } _ { \mathbb { Q } } ( B )$ denote the smallest linear subspace of R over $\mathbb { Q }$ containing B. Notice that $\mathrm { L I N } _ { \mathbb { Q } } ( B )$ can be obtained by closing set B under the action of the family $\mathcal { F }$ of operations $\langle x , y \rangle \mapsto x + y$ and $x \mapsto q x$ for every $q \in \mathbb { Q }$ . Thus $\mathrm { L I N } _ { \mathbb { Q } } ( B ) = \mathrm { c l } _ { \mathcal { F } } ( B )$ , where we are using the notation of Lemma 6.1.6. In particular, Lemma $6 . 1 . 6 ( \mathrm { a } )$ implies that 

$$
| \mathrm{LIN} _ {\mathbb {Q}} (B) | = | B | + \omega \text { for   every } B \subset \mathbb {R}.\tag{7.8}
$$

From this we immediately conclude that 

every Hamel basis H has cardinality continuum 

(7.9) 

since $\mathrm { L I N } _ { \mathbb { Q } } ( H ) = \mathbb { R }$ 

Proposition 7.3.1 If $F$ : R → R is additive then it is linear over $\mathbb { Q }$ , that is, 

$$
F (p x + q y) = p F (x) + q F (y)
$$

for every $p , q \in \mathbb { Q }$ and $x , y \in \mathbb { R }$ 

Proof Let $F \colon  { \mathbb { R } } \to  { \mathbb { R } }$ be additive. Then $F ( 0 ) + F ( 0 ) = F ( 0 + 0 ) = F ( 0 )$ so 

$$
F (0) = 0.
$$

It is easy to prove by induction on $n \in \omega$ that $F ( n x ) = n F ( x )$ for every $x \in \mathbb { R }$ . Since $F ( - x ) + F ( x ) = F ( - x + x ) = F ( 0 ) = 0 .$ , we have also that $F ( - x ) = - F ( x )$ . Therefore we conclude that 

$$
F (n x) = n F (x) \text {   for   every   } x \in \mathbb {R} \text {   and   } n \in \mathbb {Z}.
$$

In particular, for $0 < m < \omega$ we have m $\begin{array} { r } { F \left( \frac { 1 } { m } x \right) = F \left( m \frac { 1 } { m } x \right) = F ( x ) } \end{array}$ , that is, $\begin{array} { r } { F \left( \frac { 1 } { m } x \right) = \frac { 1 } { m } F ( x ) } \end{array}$ . So 

$$
F (p x) = p F (x) \text {   for   every   } x \in \mathbb {R} \text {   and   } p \in \mathbb {Q},
$$

and $F ( p x + q y ) = F ( p x ) + F ( q y ) = p F ( x ) + q F ( y )$ for every $p , q \in \mathbb { Q }$ and $x , y \in \mathbb { R }$  

Theorem 7.3.2 If $H \subset \mathbb { R }$ is a Hamel basis then every function $f \colon H \to$ R can be extended uniquely to an additive function $F \colon  { \mathbb { R } } \to  { \mathbb { R } }$ 

Proof Since every $x \in \mathbb { R }$ has a unique representation $x = q _ { 1 } b _ { 1 } + \cdot \cdot \cdot + q _ { m } b _ { m }$ in the basis H (that is, $b _ { 1 } < \cdots < b _ { m }$ are from H and $q _ { 1 } , \ldots , q _ { m } \in \mathbb { Q } \backslash \{ 0 \}$ ; see Section 4.4), we can define 

$$
F (x) = \sum_ {i = 1} ^ {m} q _ {i} f (b _ {i}).\tag{7.10}
$$

This function is clearly additive and extends f. Its uniqueness follows from Proposition 7.3.1.  

Corollary 7.3.3 There are additive discontinuous functions $F \colon \mathbb { R } \to \mathbb { Q }$ 

Proof Let H be a Hamel basis and let $x \in H$ . Define $f \colon H  \mathbb { R }$ by putting $f ( x ) = 1$ and $f ( y ) = 0$ for $y \in H \setminus \{ x \}$ . Extend f to the additive function $F . { \mathrm { B y ~ } } ( 7 . 1 0 )$ the range of f is equal to Q. Thus, F cannot be continuous, since it does not have the Darboux property.  

The function from Corollary 7.3.3 has a small (countable) range. It is not dificult to modify the argument from Corollary 7.3.3 to get an additive discontinuous function onto R. The next theorem shows that we can even do a lot better than this. 

Theorem 7.3.4 There exists a Hamel basis H and a function $f \colon H \to$ R such that $f ^ { - 1 } ( r )$ is a Bernstein set for every $r \in \mathbb { R }$ 

Proof First notice that if $f \colon H \to \mathbb { R }$ is such that 

$$
f ^ {- 1} (r) \cap P \neq \emptyset \text { for every } r \in \mathbb {R} \text { and perfect set } P \subset \mathbb {R}
$$

then f has the desired property, since the complement of each $f ^ { - 1 } ( r )$ contains $f ^ { - 1 } ( r + 1 )$ and so it must also intersect every perfect set. 

Let $\{ \langle P _ { \xi } , r _ { \xi } \rangle : \xi < \mathfrak { c } \}$ be an enumeration of $\{ P \subset \mathbb { R } \colon P$ is perfect} × R. We will construct, by induction on $\xi < { \mathfrak { c } } .$ , a one-to-one sequence $\{ x _ { \xi } \colon \xi < \mathfrak { c } \}$ that is linearly independent over $\mathbb { Q }$ and such that $x _ { \xi } \in P _ { \xi }$ for every $\xi < { \mathfrak { c } } .$ 

Notice that this will be enough to construct function f. To see it, extend $\{ x _ { \xi } \colon \xi < \mathfrak { c } \}$ to a Hamel basis (see Theorem 4.4.1). Define $f ( x _ { \xi } ) = r _ { \xi }$ for $\xi < { \mathfrak { c } }$ and extend $f$ arbitrarily to H. Then for every perfect set $P \subset \mathbb { R }$ and every $r \in \mathbb { R }$ there exists a $\xi < { \mathfrak { c } }$ such that $\langle P , r \rangle = \langle P _ { \xi } , r _ { \xi } \rangle$ , so that $f ( x _ { \xi } ) = r _ { \xi } = r$ and $x _ { \xi } \in P _ { \xi } = P$ . Therefore $f ^ { - 1 } ( r ) \cap P \neq \varnothing$ 

To make the sequence $\{ x _ { \xi } : \xi < { \mathfrak { c } } \}$ linearly independent over Q for every $\xi < { \mathfrak { c } }$ we will choose 

$$
x _ {\xi} \in P _ {\xi} \setminus \operatorname{LIN} _ {\mathbb {Q}} (\{x _ {\zeta}: \zeta <   \xi \}).\tag{i}
$$

The choice is possible since, by $( 7 . 8 ) , \ : | \mathrm { L I N } _ { \mathbb { Q } } ( \{ x _ { \zeta } \colon \zeta < \xi \} ) | = | \xi | + \omega \ : <$ c. Thus, by the recursion theorem, we can find a sequence satisfying (i). To finish the proof it is enough to show that the choice of $x _ { \xi } \mathrm { s }$ from the complement of $\mathrm { L I N } _ { \mathbb { Q } } ( \{ x _ { \zeta } \colon \zeta < \xi \} )$ makes the sequence $\{ x _ { \xi } \colon \xi < { \mathfrak { c } } \}$ linearly independent over Q. This part is left as an exercise.  

Corollary 7.3.5 There exists a nonmeasurable non-Baire additive function $F \colon  { \mathbb { R } } \to  { \mathbb { R } }$ that is strongly Darboux. 

Proof Let F be an additive extension of $f$ from Theorem 7.3.4. Then ${ \boldsymbol { F } } ^ { - 1 } ( { \boldsymbol { r } } )$ is a Bernstein set for every $r \in \mathbb { R }$  

In fact it can be proved that every discontinuous additive function is neither measurable nor Baire. 

Corollary 7.3.6 There exists a Hamel basis H that is neither measurable nor has the Baire property. 

Proof It is enough to notice that the Hamel basis H from Theorem 7.3.4 is a Bernstein set. 

It clearly intersects every perfect set. On the other hand, if $a \in H$ , then $a + H = \{ a + x \colon x \in H \}$ is disjoint from H. This is the case since otherwise there would exist $x , y \in H$ such that $a + x = y$ and so $\{ a , x , y \} \subset H$ would be linearly dependent. Thus $a + H \subset \mathbb { R } \setminus H$ . But $a + H$ intersects every perfect set $P ,$ since $H \cap ( - a + P ) \neq \emptyset$ for every perfect set $P _ { \mathrm { : } }$ , the set $- a + P$ being perfect.  

Notice that there are Hamel bases that are measurable and have the Baire property (see Exercise 2). 

Corollary 7.3.7 There exists a Hamel basis H such that $| H \cap P | = { \mathfrak { c } }$ for every perfect set P. 

Proof It is clear that the basis H from Theorem 7.3.4 has the desired property, since $\begin{array} { r } { H \cap P = \bigcup _ { r \in \mathbb { R } } ( f ^ { - 1 } ( r ) \cap P ) } \end{array}$ is the union of continuum many nonempty disjoint sets.  

Next, we will construct an additive function $F$ whose graph is connected as a subset of the plane. The graph of such a function is called a Jones space. 

Theorem 7.3.8 There exists a discontinuous additive function $F \colon  { \mathbb { R } } \to  { \mathbb { R } }$ whose graph is connected. 

Proof Let H be the Hamel basis from Corollary 7.3.7 and let $\mathcal { F }$ be the family of all closed subsets P of the plane such that $p [ P ]$ contains a perfect set, where $p$ is the projection of the plane onto the x-axis. Let $\{ P _ { \xi } \colon \xi < \mathfrak { c } \}$ be an enumeration of ${ \mathcal F } .$ . Define, by induction on $\xi < { \mathfrak { c } } ,$ , a sequence $\{ \langle x _ { \xi } , y _ { \xi } \rangle \in \mathbb { R } ^ { 2 } \colon \xi < { \mathfrak { c } } \}$ such that 

(i) $\begin{array} { r } { x _ { \xi } \in ( H \cap p [ P _ { \xi } ] ) \setminus \{ x _ { \zeta } \colon \zeta < \xi \} , } \end{array}$ 

(ii) $\langle x _ { \xi } , y _ { \xi } \rangle \in P _ { \xi }$ 

The choice as in (i) can be made, since $| H \cap p [ P _ { \xi } ] | = { \mathfrak { c } }$ 

Now define $f ( x _ { \xi } ) = y _ { \xi }$ and extend f to H in an arbitrary way. Let $F$ be the additive extension of $f$ . We will show that the graph of $F$ is connected. 

To obtain a contradiction assume that the graph of $F$ is not connected. Then there exist disioint open subsets U and V of $\mathbb { R } ^ { 2 }$ such that $U \cap F \neq$ $\emptyset \neq V \cap F$ and $F \subset U \cup V$ . Let $P = \mathbb { R } ^ { 2 } \setminus ( U \cup V )$ . We will show that $P \cap F \neq \emptyset$ , which will give us the desired contradiction. 

If $P \in { \mathcal { F } }$ then there exists a $\xi < { \mathfrak { c } }$ such that $P = P _ { \xi }$ , and so $\langle x _ { \xi } , y _ { \xi } \rangle \in$ $P _ { \xi } \cap F = P \cap F$ . Thus it is enough to prove that $P \in { \mathcal { F } }$ . Clearly, $P$ is closed. So we have to show only that 

p[P] contains a perfect subset. 

In order to prove it we first show that there exists an $x \in \mathbb { R }$ such that 

$$
U \cap (\{x \} \times \mathbb {R}) \neq \emptyset \neq V \cap (\{x \} \times \mathbb {R}).\tag{7.11}
$$

To obtain a contradiction, assume that (7.11) is false. Then the sets $U _ { 1 } =$ $p [ U ]$ and $V _ { 1 } = p [ V ]$ are disjoint. But they are open in R, since the projection of an open set is open. They are clearly nonempty, since $U$ and V are nonempty. Finally, $U _ { 1 } \cup V _ { 1 } = p [ U \cup V ] \supset p [ F ] = \mathbb { R }$ , that is, sets $U _ { 1 }$ and $V _ { 1 }$ violate the connectedness of R. Condition $( 7 . 1 1 )$ has been proved. 

Now let $x _ { 0 } \in \mathbb { R }$ be such that $U \cap ( \{ x _ { 0 } \} \times \mathbb { R } ) \neq \emptyset \neq V \cap ( \{ x _ { 0 } \} \times \mathbb { R } )$ and let $y _ { 1 } , y _ { 2 } \in \mathbb { R }$ be such that $\langle x _ { 0 } , y _ { 1 } \rangle \in U$ and $\langle x _ { 0 } , y _ { 2 } \rangle \in V$ . Then there exists an open interval $\boldsymbol { I } = \left( a , b \right)$ containing x such that $I \times \{ y _ { 1 } \} \subset U$ and $I \times \{ y _ { 2 } \} \subset V$ . But for every $x \in I$ the interval $J _ { x } = \{ x \} \times [ y _ { 1 } , y _ { 2 } ]$ is a connected set intersecting both U and V. Thus $J _ { x }$ must intersect $P$ as well, since it is connected. Therefore $\{ x \} = p [ J _ { x } \cap P ] \subset p [ P ]$ for every $x \in I$ , that is, $p [ P ] \supset I$ . This finishes the proof that $P \in { \mathcal { F } }$  

We will finish this section with following theorem of Erd˝os and Kakutani (1943). 

Theorem 7.3.9 The continuum hypothesis is equivalent to the existence of a countable partition $\{ H _ { n } \colon n < \omega \}$ of $\mathbb { R } \backslash \{ 0 \}$ such that every $H _ { n }$ is a Hamel basis. 

In the proof of the theorem we will use the following two lemmas, the first of which is due to Erd˝os and Hajnal (Erd˝os 1978–9). They are also very interesting in their own right. 

Lemma 7.3.10 If $f \colon A \times B \to \omega$ , where $| A | = \omega _ { 2 }$ and $| B | = \omega _ { 1 }$ , then for every $n < \omega$ there exist $B _ { 0 } \in [ B ] ^ { n }$ and $A _ { 0 } \in [ A ] ^ { \omega _ { 2 } }$ such that $f ( a _ { 0 } , b _ { 0 } ) =$ $f ( a _ { 1 } , b _ { 1 } )$ for every $a _ { 0 } , a _ { 1 } \in A _ { 0 }$ and $b _ { 0 } , b _ { 1 } \in B _ { 0 }$ 

Proof Fix $n < \omega$ . First we will show that 

$$
\forall a \in A \exists B _ {a} \in [ B ] ^ {n} \exists m _ {a} <   \omega \forall b \in B _ {a} (f (a, b) = m _ {a}).\tag{7.12}
$$

To see this, notice that for every $a \in A$ the sets $S _ { a } ^ { m } = \{ b \in B \colon f ( a , b ) = m \}$ form a countable partition of an uncountable set B. Thus there is an $m = m _ { a }$ for which the set ${ \cal S } _ { a } ^ { m }$ is uncountable and any n-element subset $B _ { a }$ of ${ \cal S } _ { a } ^ { m }$ satisfies (7.12). 

Now let $F \colon A \ \to \ [ B ] ^ { n } \times \omega$ be such that for every $a \ \in \ A$ the pair $F ( a ) = \left. B _ { a } , m _ { a } \right.$ satisfies (7.12). The set $[ B ] ^ { n } \times \omega$ has cardinality $\omega _ { 1 }$ , so there exists $\langle B _ { 0 } , m \rangle \in [ B ] ^ { n } \times \omega$ such that $A _ { 0 } = F ^ { - 1 } ( B _ { 0 } , m )$ has cardinality $\omega _ { 2 }$ . But then, if $a _ { i } \in A _ { 0 }$ for $i < 2$ then $F ( a _ { i } ) = \left. B _ { 0 } , m \right.$ and 

$$
f (a _ {i}, b) = m _ {a _ {i}} = m
$$

for every $b \in B _ { a _ { i } } = B _ { 0 }$ . So the sets $A _ { 0 }$ and $B _ { 0 }$ have the desired property.  

Notice that Lemma 7.3.10 can also be expressed in the following graphtheoretic language. Let A and B be disjoint sets of cardinality $\omega _ { 2 }$ and $\omega _ { 1 }$ , respectively, and let $G = \langle V , E \rangle$ be the bipartite graph between A and B, that is, $V = A \cup B$ and $E = \{ \{ a , b \} \colon a \in A \ \& \ b \in B \}$ . Then for any $n < \omega$ and any coloring $f \colon E \to \omega$ of the edges of graph G there are $A _ { 0 } \in [ A ] ^ { \omega _ { 2 } }$ and $B _ { 0 } \in [ B ] ^ { n }$ such that the subgraph $G _ { 0 } = \langle A _ { 0 } \cup B _ { 0 } , E \cap \mathcal { P } ( A _ { 0 } \cup B _ { 0 } ) \rangle$ of $G$ generated by $A _ { 0 } \cup B _ { 0 }$ is monochromatic, that is, the coloring function f is constant on the edges of $G _ { 0 }$ 

Lemma 7.3.11 Assume that ${ \mathfrak { c } } > \omega _ { 1 }$ and let $H \in [ \mathbb { R } ] ^ { \omega _ { 2 } }$ . Then for every partition $\{ H _ { n } \colon n < \omega \}$ of R there exist $n < \omega$ and disjoint sets $A _ { 0 } \in [ H ] ^ { \omega _ { 2 } }$ and $B _ { 0 } \in [ H ] ^ { 2 }$ such that 

$$
a + b \in H _ {n} \text {   for   every   } a \in A _ {0} \text {   and   } b \in B _ {0}.
$$

Proof Choose disjoint $A \in [ H ] ^ { \omega _ { 2 } }$ and $B \in [ H ] ^ { \omega _ { 1 } }$ . Define $f \colon A \times B \to \omega$ by 

$$
f (a, b) = m \text { if   and   only   if } a + b \in H _ {m}.
$$

Then the sets $A _ { 0 }$ and $B _ { 0 }$ from Lemma 7.3.10 used with f and $n = 2$ have the desired properties.  

Proof of Theorem ${ \mathbf { 7 . 3 . 9 \ 4 } } = :$ Let H be any Hamel basis and suppose that there exists a partition $\{ H _ { n } \colon n < \omega \}$ of $\mathbb { R } \backslash \{ 0 \}$ into Hamel bases. 

To obtain a contradiction assume that ${ \mathfrak { c } } > \omega _ { 1 }$ . Then $| H | = { \mathfrak { c } } \geq \omega _ { 2 }$ so we can choose $A _ { 0 }$ and $B _ { 0 }$ as in Lemma 7.3.11. Take diferent $a _ { 0 } , a _ { 1 } \in A _ { 0 }$ and $b _ { 0 } , b _ { 1 } \in B _ { 0 }$ . Then the numbers $x _ { i j } = a _ { i } + b _ { j }$ for $i , j \in 2$ are diferent and belong to the same $H _ { n }$ . However, 

$$
x _ {0 0} - x _ {1 0} = (a _ {0} + b _ {0}) - (a _ {1} + b _ {0}) = (a _ {0} + b _ {1}) - (a _ {1} + b _ {1}) = x _ {0 1} - x _ {1 1},
$$

contradicting the fact that $x _ { 0 0 } , x _ { 1 0 } , x _ { 0 1 } , x _ { 1 1 } \in H _ { n }$ are linearly independent over Q. 

⇒: Let $\{ z _ { \xi } \in \mathbb { R } \colon \xi < \omega _ { 1 } \}$ be a Hamel basis and for every $\xi \le \omega _ { 1 }$ define $L _ { \xi } \ = \ \mathrm { L I N } _ { \mathbb { Q } } ( \{ z _ { \zeta } \colon \zeta \ < \ \xi \} )$ . Notice that $L _ { \xi } \subset L _ { \eta }$ for $\xi \ : < \ : \eta \ : \le \ : \omega _ { 1 }$ , that $\textstyle L _ { \lambda } = \bigcup _ { \xi < \lambda } L _ { \xi }$ for limit $\lambda \leq \omega _ { 1 }$ , and that $L _ { \omega _ { 1 } } = \mathbb { R }$ (compare this with Lemma 6.1.6). Thus the sets $\{ L _ { \xi + 1 } - L _ { \xi } \colon \xi < \omega _ { 1 } \}$ form a partition of $\mathbb { R } \setminus L _ { 0 } = \mathbb { R } \setminus \{ 0 \}$ . For every $\xi < \omega _ { 1 }$ choose a bijection $f _ { \xi } \colon L _ { \xi + 1 } - L _ { \xi } \to \omega$ and let $f = \textstyle \bigcup _ { \xi < \omega _ { 1 } } f _ { \xi }$ . Then $f \colon \mathbb { R } \setminus \{ 0 \}  \omega$ . Let $H _ { n } = f ^ { - 1 } ( n )$ 

The sets $\{ \bar { H } _ { n } \colon n < \omega \}$ form a partition of $\mathbb { R } \backslash \{ 0 \}$ . To finish the proof it is enough to show that every $H _ { n }$ is a Hamel basis. 

So choose $n < \omega$ and let $\{ x _ { \xi } \} = ( L _ { \xi + 1 } - L _ { \xi } ) \cap f ^ { - 1 } ( n )$ for $\xi < \omega _ { 1 }$ . It is enough to prove that 

$$
L _ {\eta} = \mathrm{LIN} _ {\mathbb {Q}} (\{x _ {\zeta}: \zeta <   \eta \})\tag{7.13}
$$

for every $\eta \leq \omega _ { 1 }$ , since then $H _ { n } = \{ x _ { \xi } \colon \xi < \mathfrak { c } \}$ spans R and $\{ x _ { \xi } \colon \xi < \mathfrak { c } \}$ is linearly independent by Exercise 1. Condition (7.13) can be proved by induction on $\eta \leq \omega _ { 1 }$ . So let $\alpha \leq \omega _ { 1 }$ be such that (7.13) holds for every $\eta < \alpha$ 

If α is a limit ordinal then 

$$
L _ {\alpha} = \bigcup_ {\eta <   \alpha} L _ {\eta} = \bigcup_ {\eta <   \alpha} \operatorname{LIN} _ {\mathbb {Q}} (\{x _ {\zeta}: \zeta <   \eta \}) = \operatorname{LIN} _ {\mathbb {Q}} (\{x _ {\zeta}: \zeta <   \alpha \}).
$$

If $\alpha = \eta + 1$ then $L _ { \eta } = \mathrm { L I N } _ { \mathbb { Q } } ( \{ x _ { \zeta } \colon \zeta < \eta \} )$ and 

$$
\{x _ {\eta} \} \cup \operatorname{LIN} _ {\mathbb {Q}} (\{x _ {\zeta}: \zeta <   \eta \}) = \{x _ {\eta} \} \cup L _ {\eta} \subset L _ {\eta + 1}
$$

so $\operatorname { L I N } _ { \mathbb { Q } } ( \{ x _ { \zeta } \colon \zeta < \eta + 1 \} ) \subset L _ { \eta + 1 }$ 

To prove the other inclusion, recall that $x _ { \eta } \in L _ { \eta + 1 } - L _ { \eta }$ . Therefore $\begin{array} { r } { x _ { \eta } = q z _ { \eta } + \sum _ { i < m } q _ { i } b _ { i } } \end{array}$ for some $q , q _ { 0 } , \dots , q _ { m - 1 } \in \mathbb { Q }$ and $b _ { 0 } , \dots , b _ { m - 1 } \in$ $\{ x _ { \zeta } \colon \zeta < \eta \}$ . Moreover, $q \neq 0$ because $x _ { \eta } \notin L _ { \eta } = \mathrm { L I N } _ { \mathbb { Q } } ( \{ x _ { \zeta } : \zeta < \eta \} )$ . So 

$$
z _ {\eta} = \frac {1}{q} \left(x _ {\eta} - \sum_ {i <   m} q _ {i} b _ {i}\right) \in \mathrm{LIN} _ {\mathbb {Q}} (\{x _ {\zeta}: \zeta <   \eta + 1 \}).
$$

Now $\{ z _ { \eta } \} \cup L _ { \eta } \subset \mathrm { L I N } _ { \mathbb { Q } } ( \{ x _ { \zeta } \colon \zeta < \eta + 1 \} )$ , and so we can conclude that $L _ { \eta + 1 } \subset \mathrm { L I N } _ { \mathbb { Q } } ( \{ x _ { \zeta } : \zeta < \eta + 1 \} )$  

## EXERCISES

1 Complete the proof of Theorem 7.3.4 by showing that if $\{ x _ { \xi } \in \mathbb { R } \colon \xi < { \mathfrak { c } } \}$ is such that $x _ { \xi } \notin \mathrm { L I N } _ { \mathbb { Q } } ( \{ x _ { \zeta } \colon \zeta < \xi \} )$ for every $\xi < { \mathfrak { c } } .$ , then $\{ x _ { \xi } \in \mathbb { R } \colon \xi < { \mathfrak { c } } \}$ is linearly independent over Q. 

2 Let $C \subset \mathbb { R }$ be the Cantor set. Show that there is a Hamel basis contained in C. Since C is nowhere dense and has measure zero, it follows that Hamel bases can be measurable and have the Baire property. Hint: Use the fact that $C + C = \{ a + b \colon a , b \in C \}$ contains the unit interval [0, 1]. 

3 Let ∼ be an equivalence relation on R defined by $x \sim y$ if and only if $x - y \in \mathbb { Q }$ . If V is a selector from the family of all equivalence classes of ∼ then V is called a Vitali set. It is known that any Vitali set is neither measurable nor has the Baire property. 

Construct a Vitali set V such that 

(a) $V + V = \mathbb { R } ,$ 

(b) $V + V$ is a Bernstein set. 

4 Prove that the graph of any additive discontinuous function $F \colon  { \mathbb { R } } \to  { \mathbb { R } }$ is dense in $\mathbb { R } ^ { 2 }$ 

## 7.4 Symmetrically discontinuous functions

This section is motivated in part by the following generalization of the continuity of real functions. A function $f \colon  { \mathbb { R } } \to  { \mathbb { R } }$ is said to be symmetrically continuous at the point $x \in \mathbb { R }$ if 

$$
\lim _ {h \to 0 ^ {+}} [ f (x - h) - f (x + h) ] = 0,
$$

that is, if for every $\varepsilon > 0$ there exists a $d > 0$ such that 

$$
(0, d) \subset S _ {x} ^ {\varepsilon},
$$

where $S _ { x } ^ { \varepsilon } = \{ h > 0 \colon | f ( x - h ) - f ( x + h ) | < \varepsilon \}$ . A function $f \colon  { \mathbb { R } } \to  { \mathbb { R } }$ is symmetrically continuous if it is symmetrically continuous at every point $x \in \mathbb { R }$ 

Clearly, every continuous function is symmetrically continuous. The converse implication is not true, since there are symmetrically continuous functions that are not continuous in the usual sense. For example, the characteristic function $\chi _ { \{ 0 \} }$ of a singleton set {0} is symmetrically continuous and discontinuous at 0. However, symmetrically continuous functions cannot behave too badly in this respect: It can be proved that the set of points of discontinuity of a symmetrically continuous function must be of first category and have measure zero. 

The study of symmetrically continuous functions is an important subject in real analysis, motivated by Fourier analysis. In this section, however, this notion serves merely as a motivation, since we will study here the functions that are not symmetrically continuous. 

It is easy to find a function that is not symmetrically continuous. For example, a characteristic function of any nontrivial interval is symmetrically discontinuous at the endpoints of that interval. In fact, it is also not dificult to construct a function $f \colon  { \mathbb { R } } \to  { \mathbb { R } }$ that is nowhere symmetrically continuous. Such a function must have the property that for every $x \in \mathbb { R }$ there exists an $\varepsilon > 0$ such that 

$$
\forall d > 0 \exists h \in (0, d) (| f (x - h) - f (x + h) | \geq \varepsilon),\tag{7.14}
$$

or, equivalently, such that 

$$
(0, d) \not \subset S _ {x} ^ {\varepsilon} \quad \text { for   every } d > 0.\tag{7.15}
$$

To get such an example define f as the characteristic function $\chi _ { H }$ of any dense Hamel basis H. Notice that such a basis exists by Theorem 7.3.4. To see that $\chi _ { H }$ is nowhere symmetrically continuous, take $x \in \mathbb { R } , \varepsilon \in ( 0 , 1 )$ , and an arbitrary $d > 0$ . We have to find $h \in ( 0 , d )$ with the property that $| \chi _ { H } ( x - h ) - \chi _ { H } ( x + h ) | \geq \varepsilon$ . So let $q _ { 1 } b _ { 1 } + \cdots + q _ { n } b _ { n }$ be a representation of x in basis H. Then, by the density of H, there exists a $b \in H \cap ( x - d , x ) \setminus \{ b _ { 1 } , . . . \ , b _ { n } \}$ . Pick $h \ = \ x - b .$ Then $h \in ( 0 , d )$ and $\chi _ { H } ( x - h ) = \chi _ { H } ( b ) = 1 . \ \mathrm { { O n } }$ the other hand, $\chi _ { H } ( x + h ) = 0 { \mathrm { ~ a s ~ } } x + h = $ $2 x - b = 2 q _ { 1 } b _ { 1 } + \cdot \cdot \cdot + 2 q _ { n } b _ { n } - b \notin H$ . Therefore $| \chi _ { H } ( x - h ) - \chi _ { H } ( x + h ) | =$ $1 > \varepsilon .$ 

Considerations of how badly nowhere–symmetrically continuous functions can behave led several $\mathrm { p e o p l e ^ { 1 } }$ to to ask whether there exists a function f satisfying (7.14) with the quantifiers $\forall d > 0 \exists h \in ( 0 , d )$ replaced by the reversed quantifiers $\exists d > 0 \forall h \in ( 0 , d )$ , that is, whether there exists a function $f : \mathbb { R } \to \mathbb { R }$ such that for every $x \in \mathbb { R }$ there exists an $\varepsilon > 0$ with 

$$
\exists d > 0 \forall 0 <   h <   d (| f (x - h) - f (x + h) | \geq \varepsilon),
$$

or, equivalently, such that 

$$
(0, d) \cap S _ {x} ^ {\varepsilon} = \emptyset \quad \text {   for   some   } d > 0.
$$

Replacing ε and d by their minima, we can rephrase this problem by asking whether there exists a function $f \colon  { \mathbb { R } } \to  { \mathbb { R } }$ such that 

(G) for every $x \in \mathbb { R }$ there exists a $d > 0$ with 

$$
(0, d) \cap S _ {x} ^ {d} = \emptyset ,\tag{7.16}
$$

where $S _ { x } ^ { d } = \{ h > 0 \colon | f ( x - h ) - f ( x + h ) | < d \} .$ 

A function f satisfying (G) will be called a uniformly antisymmetric function. 

The existence of uniformly antisymmetric functions can be inferred from the following theorem due to Ciesielski and Larson (1993–4). 

Theorem 7.4.1 There exists a partition $\mathcal { P } = \{ P _ { n } : n \in \mathbb { N } \}$ of R such that for every $x \in \mathbb { R }$ the set 

$$
S _ {x} = \bigcup_ {n \in \mathbb {N}} \{h > 0: x - h, x + h \in P _ {n} \}\tag{7.17}
$$

is finite. 

Before proving this theorem, we first show how to use it to construct a uniformly antisymmetric function. 

Corollary 7.4.2 There exists a uniformly antisymmetric function $f : \mathbb { R } \to \mathbb { N } .$ 

Proof Let $\mathcal { P } = \{ P _ { n } : n \in \mathbb { N } \}$ be a partition satisfying (7.17) and for $x \in \mathbb { R }$ define 

$$
f (x) = n \text { if   and   only   if } x \in P _ {n}.
$$

Then f is uniformly antisymmetric, since for every $x \in \mathbb { R }$ the set 

$$
S _ {x} ^ {1} = \{h > 0: | f (x - h) - f (x + h) | <   1 \} = \{h > 0: f (x - h) = f (x + h) \} = S _ {x}
$$

is finite, so $d = \operatorname* { m i n } ( S _ { x } \cup \{ 1 \} )$ satisfies (G), as $S _ { x } ^ { d } = S _ { x } ^ { 1 }$ 

Proof of Theorem 7.4.1 Let H be a Hamel basis. Then every $x \in$ R has a unique representation $x = q _ { 1 } b _ { 1 } + \cdot \cdot \cdot + q _ { n } b _ { n }$ in the basis H (that is, $b _ { 1 } < \cdots < b _ { n }$ are from H and $q _ { 1 } , \ldots , q _ { n } \in \mathbb { Q } \setminus \{ 0 \} )$ . Let $B _ { x } =$ $\{ b _ { 1 } , \dotsc , b _ { n } \} \subset H$ and define $c _ { x } \colon B _ { x } \ \to \ \mathbb { Q }$ by putting $c _ { x } ( b _ { i } ) ~ = ~ q _ { i }$ for $1 \leq i \leq n$ . Moreover, extend each $c _ { x }$ to $\hat { c } _ { x } \colon H  \mathbb { Q }$ by putting 

$$
\hat {c} _ {x} (b) = \left\{ \begin{array}{l l} c _ {x} (b) & \text { for } b \in B _ {x}, \\ 0 & \text { otherwise }. \end{array} \right.
$$

Then, for every $x \in \mathbb { R }$ ， 

$$
x = \sum_ {b \in B _ {x}} c _ {x} (b) b = \sum_ {b \in H} \hat {c} _ {x} (b) b.
$$

We will start the argument by proving that there exists a countable set $D = \{ g _ { n } \colon n < \omega \}$ of functions from H into $\mathbb { Q }$ such that 

$$
\forall x \in \mathbb {R} \exists n <   \omega (c _ {x} \subset g _ {n}).\tag{7.18}
$$

To see it, let $\mathcal { U } = \{ ( p , q ) \cap H \colon p , q \in \mathbb { Q } \}$ and notice that U is countable. Define 

$$
D = \left\{\sum_ {i <   n} q _ {i} \chi_ {U _ {i}} \in \mathbb {Q} ^ {H}: n \in \omega \text {   and   } \langle q _ {i}, U _ {i} \rangle \in \mathbb {Q} \times \mathcal {U} \text {   for   every   } i <   n \right\}
$$

Clearly, D is countable, since it is indexed by a countable set $\textstyle \bigcup _ { n < \omega } ( \mathbb { Q } \times \mathcal { U } ) ^ { n } .$ To see that it satisfies (7.18), take $x \in \mathbb { R }$ and find a family $\{ U _ { b } \in \dot { \mathcal { U } } : b \in B _ { x } \}$ of disjoint sets such that $b \in U _ { b }$ for every $b \in B _ { x }$ . Then $\begin{array} { r } { g = \sum _ { b \in B _ { x } } c _ { x } ( b ) \chi _ { U _ { b } } } \end{array}$ belongs to $D$ and $c _ { x } ( b ) = g ( b )$ for every $b \in B _ { x }$ . So $c _ { x } \subset g$ . Condition (7.18) has been proved. 

Now let $\{ g _ { n } \colon n < \omega \}$ be as in (7.18). Define $f \colon \mathbb { R } \to \omega$ by 

$$
f (x) = \min \{n <   \omega : c _ {x} \subset g _ {n} \}
$$

and let $P _ { n } = f ^ { - 1 } ( n )$ for every $n < \omega$ . We will show that the partition ${ \mathcal { P } } = \{ P _ { n } \colon n \in \mathbb { N } \}$ of R satisfies (7.17). 

So fix $x \in \mathbb { R }$ and let $h \in S _ { x }$ . We will show that 

$$
\hat {c} _ {x + h} (b) \in \{0, \hat {c} _ {x} (b), 2 \hat {c} _ {x} (b) \} \text {   for   every   } b \in H.\tag{7.19}
$$

This will finish the proof, since $\{ 0 , \hat { c } _ { x } ( b ) , 2 \hat { c } _ { x } ( b ) \} = \{ 0 \}$ for $b \in H \backslash B _ { x }$ and so there are at most $3 ^ { | B _ { x } | } < \omega$ numbers $x + h$ such that $h \in S _ { x }$ . Thus $S _ { x }$ is finite. 

To see (7.19), notice that $( x + h ) + ( x - h ) = 2 x$ , so 

$$
\sum_ {b \in H} \hat {c} _ {x + h} (b) b + \sum_ {b \in H} \hat {c} _ {x - h} (b) b = 2 \sum_ {b \in H} \hat {c} _ {x} (b) b.
$$

In particular, 

$$
\hat {c} _ {x + h} (b) + \hat {c} _ {x - h} (b) = 2 \hat {c} _ {x} (b)\tag{7.20}
$$

for every $b \in H$ 

Now, if $x + h , x - h \in P _ { n }$ then $c _ { x + h } \subset g _ { n }$ and $c _ { x - h } \subset g _ { n }$ . Hence 

$$
c _ {x + h} (b) = g _ {n} (b) = c _ {x - h} (b) \text {   for   every   } b \in B _ {x + h} \cap B _ {x - h}.
$$

Therefore, by $( 7 . 2 0 ) , \hat { c } _ { x + h } ( b ) = \hat { c } _ { x } ( b )$ for every $b \in B _ { x + h } \cap B _ { x - h }$ . But for $b \in H \setminus B _ { x + h }$ we have ${ \hat { c } } _ { x + h } ( b ) = 0$ , and for every $b \in B _ { x + h } \setminus B _ { x - h }$ we have $\hat { c } _ { x + h } ( b ) = \hat { c } _ { x + h } ( b ) + \hat { c } _ { x - h } ( b ) = 2 \hat { c } _ { x } ( b )$ . Thus $\hat { c } _ { x + h } ( b ) \in \{ 0 , \hat { c } _ { x } ( b ) , 2 \hat { c } _ { x } ( b ) \}$ for every $b \in H$ . This finishes the proof of condition (7.20) and Theorem 7.4.1.  

An interesting open problem is whether or not there exists a uniformly antisymmetric function with finite or bounded range. Some partial results are known in this direction. Komj´ath and Shelah (1993–4) proved that there is no function $f \colon  { \mathbb { R } } \to  { \mathbb { R } }$ with finite range such that all the sets $S _ { x }$ from Theorem 7.4.1 are finite. It has also been proved by Ciesielski (1995– 6) that the range of any uniformly antisymmetric function must have at least four elements. The next theorem, due to Ciesielski and Larson (1993– 4), shows only that the range of a uniformly antisymmetric function must have at least three elements. 

Theorem 7.4.3 If $f \colon  { \mathbb { R } } \to \{ 0 , 1 \}$ then f is not uniformly antisymmetric. 

Proof To obtain a contradiction assume that there exists a uniformly antisymmetric function $f \colon  { \mathbb { R } } \to \{ 0 , 1 \}$ and for every $x \in \mathbb { R }$ let $n _ { x } \in  { \mathbb { N } }$ be such that for every $h \in ( 0 , 1 / n _ { x } )$ , 

$$
\left| f (x - h) - f (x + h) \right| \geq 1 / n _ {x}.
$$

Fix $n \in \mathbb { N }$ such that $L = \{ x \in \mathbb { R } \colon n _ { x } = n \}$ is uncountable. Then 

$$
f (x - h) \neq f (x + h) \text {   for   every   } x \in L \text {   and   } h \in (0, 1 / n).\tag{7.21}
$$

Since $\textstyle { \left\{ { \bigl ( } { \frac { k } { n } } , { \frac { k + 1 } { n } } { \bigr ] } \cap L \colon k \in \mathbb { Z } \right\} }$ forms a countable partition of $L ,$ at least one of these sets must be uncountable. In particular, we can choose $x , y , z \in L$ such that $x < y < z < x + 1 / n$ . Now we would like to find points $a , b , c \in \mathbb { R }$ such that $x , y ,$ and z are the midpoints of pairs $\langle a , b \rangle , \langle b , c \rangle$ , and $\langle a , c \rangle$ respectively, that is, such that $a + b = 2 x , b + c = 2 y$ , and $a + c = 2 z$ . It is easy to see that the points 

$$
a = x - y + z, \quad b = x + y - z, \quad c = - x + y + z
$$

have these properties. Moreover, for $h = z - y \in ( 0 , 1 / n )$ we have $a = x + h$ and $b = x - h$ . Hence, by $( 7 . 2 1 ) , f ( a ) \neq f ( b )$ . Similarly, $f ( b ) \neq f ( c )$ and $f ( c ) \neq f ( a )$ . But this is impossible, since the points $a , b ,$ and c are distinct and f attains only two values.  

We proved Corollary 7.4.2, via Theorem 7.4.1, by showing that for every $x \in \mathbb { R }$ the set $S _ { x } ^ { 1 } = S _ { x }$ of exceptional points, being finite, is bounded away from 0. What if we allow the sets $S _ { x }$ to be countable? Certainly, such sets do not have to be bounded away from 0. But we can replace the condition of being “bounded away from $0 ^ { \dag }$ by the weaker condition of being “almost bounded away from $0 , \ d s$ in the sense that $S _ { x } \cap ( 0 , d )$ is countable for some $d > 0$ Can we prove then an analog of Theorem 7.4.1? Surprisingly, the answer depends on the continuum hypothesis, as is proved in the next theorem. 

The general form of this theorem is due to Ciesielski and Larson (1993– 4). However, implication $( \mathrm { i } ) { \Rightarrow } ( \mathrm { i i } )$ was first proved by Sierpi´nski (1936). The equivalence of (i) and (ii) is also implicitly contained in a work of Freiling (1989–90). 

Theorem 7.4.4 The following conditions are equivalent. 

(i) The continuum hypothesis. 

(ii) There exists a partition $\mathcal { P } = \{ A _ { 0 } , A _ { 1 } \}$ of R such that for every $x \in \mathbb { R }$ the set $\begin{array} { r } { S _ { x } = \bigcup _ { i < 2 } \{ h > 0 \colon x - h , x + h \in A _ { i } \} } \end{array}$ is at most countable. 

(iii) There exists a function $f \colon  { \mathbb { R } } \to \{ 0 , 1 \}$ such that for every $x \in \mathbb { R }$ there is a $d > 0$ with the property that $\left| S _ { x } ^ { d } \cap ( 0 , d ) \right| \leq \omega$ 

Proof $( \mathrm { i } ) { \Rightarrow } ( \mathrm { i i } )$ : Let $H = \{ b _ { \zeta } \colon \zeta < \omega _ { 1 } \}$ be a Hamel basis. For $x \in \mathbb { R } \setminus \{ 0 \}$ let $q ( x ) = q _ { n }$ , where $x = q _ { 1 } b _ { \zeta _ { 1 } } + \cdot \cdot \cdot + q _ { n } b _ { \zeta _ { n } }$ is the unique representation of x in the basis H, with $\zeta _ { 1 } < \cdots < \zeta _ { n }$ and $q _ { i } \neq 0$ . Put 

$$
x \in A _ {0} \text { if   and   only   if } q (x) > 0,
$$

and $A _ { 1 } = \mathbb { R } \backslash A _ { 0 }$ . We will show that the partition $\mathcal { P } = \{ A _ { 0 } , A _ { 1 } \}$ satisfies (ii). 

For $\xi < \omega _ { 1 }$ let $K _ { \xi } = \mathrm { L I N } _ { \mathbb { Q } } ( \{ b _ { \zeta } \colon \zeta \leq \xi \} )$ . Notice that $\textstyle \mathbb { R } = \bigcup _ { \xi < \omega _ { 1 } } K _ { \xi }$ and that every $K _ { \xi }$ is countable. We will show that if $x \in K _ { \xi }$ then $S _ { x } \subset K _ { \xi }$ This will finish the proof. 

But it is easy to see that for $h \in \mathbb { R } \backslash K _ { \xi }$ and $x \in K _ { \xi }$ 2 

$$
h \in A _ {0} \text { if   and   only   if } x + h \in A _ {0},
$$

since $q ( h ) = q ( x + h )$ . However, h and $- h$ cannot belong to the same $A _ { i }$ for $h \neq 0$ , so $S _ { x } \subset K _ { \xi }$ 

(ii)⇒(iii): For $x \in \mathbb { R }$ define $f ( x ) = i { \mathrm { ~ i f ~ } } x \in A _ { i }$ . Then $S _ { x } ^ { d } = S _ { x }$ is countable for every $x \in \mathbb { R }$ and $d \in ( 0 , 1 )$ 

(iii)⇒(i): Let f be as in (iii), and for every $x \in \mathbb { R }$ let $n _ { x } \in \mathbb { N }$ be such that the set 

$$
C _ {x} = S _ {x} ^ {1 / n _ {x}} \cap (0, 1 / n _ {x}) = \{h \in (0, 1 / n _ {x}): f (x - h) = f (x + h) \}
$$

is countable. 

To obtain a contradiction, assume that the continuum hypothesis fails and let B be a linearly independent subset of R over Q of cardinality $\omega _ { 2 }$ Choose $K \subset B$ of cardinality $\omega _ { 2 }$ such that for some $n \in \mathbb { N }$ we have $n _ { x } = n$ for all $x \in K$ . Let U be an open interval of length less than $1 / n$ such that the set $L = K \cap U$ has cardinality $\omega _ { 2 }$ . Then, in particular, 

$$
f (x - h) \neq f (x + h) \text {   for   } x \in L \text {   and   } h \in (0, 1 / n) \setminus C _ {x},\tag{7.22}
$$

and 

$$
| x - y | <   1 / n \text { for   every } x, y \in L.\tag{7.23}
$$

Define, by transfinite induction, a sequence $\langle t _ { \xi } \in L \colon \xi < \omega _ { 2 } \rangle$ such that 

$$
t _ {\xi} \in L \setminus T _ {\xi} \text { for   every } \xi <   \omega_ {2},\tag{7.24}
$$

where $T _ { \xi }$ is the smallest linear subspace of R containing $\{ t _ { \zeta } : \zeta < \xi \}$ and such that 

$$
C _ {x} \subset T _ {\xi} \text {   for   every   } x \in T _ {\xi}.\tag{7.25}
$$

Such $T _ { \xi }$ is obtained by applying Lemma $6 . 1 . 6 ( \mathrm { a } )$ to the set $Z = \{ t _ { \zeta } \colon \zeta < \xi \}$ and the family $\mathcal { F }$ of operations $x \mapsto C _ { x } , \langle x , y \rangle \mapsto x + y$ , and $x \mapsto q x$ for every $q \in \mathbb { Q }$ . Then $T _ { \xi }$ has cardinality $\leq \omega _ { 1 }$ , so the induction can be done easily. 

Now put $x = t _ { 0 } , z = t _ { \omega _ { 1 } }$ and, for $0 < \xi < \omega _ { 1 }$ , consider the numbers $\vert - x + t _ { \xi } \vert$ . All these numbers are diferent, so there is $0 < \eta < \omega _ { 1 }$ such that 

$$
\left| - x + t _ {\eta} \right| \notin C _ {z}.\tag{7.26}
$$

Put $y = t _ { \eta }$ and proceed as in Theorem 7.4.3. Define 

$$
a = x - y + z, \quad b = x + y - z, \quad c = - x + y + z.\tag{7.27}
$$

Then $( a + b ) / 2 = x , ( b + c ) / 2 = y$ , and $( c + a ) / 2 = z$ . We will show that 

$$
f (a) \neq f (b), \quad f (b) \neq f (c), \quad f (c) \neq f (a),\tag{7.28}
$$

which will give us the desired contradiction, since the points a, b, and c are distinct and $f$ admits only two values. 

To prove (7.28), notice first that (7.28) follows from (7.22) as long as 

$$
| a - x | <   1 / n, \quad | b - y | <   1 / n, \quad | c - z | <   1 / n\tag{7.29}
$$

and 

$$
\left| a - x \right| \not \in C _ {x}, \quad \left| b - y \right| \not \in C _ {y}, \quad \left| c - z \right| \not \in C _ {z}.\tag{7.30}
$$

But (7.29) follows easily from (7.27) and (7.23). Finally, (7.30) can be proved as follows. 

$| a - x | \notin C _ { x } ,$ , since otherwise we would have $z - y = a - x \in T _ { \omega _ { 1 } }$ and $z \in y + T _ { \omega _ { 1 } } \subset T _ { \omega _ { 1 } }$ , contradicting $z = t _ { \omega _ { 1 } } \notin T _ { \omega _ { 1 } }$ 

$| b - y | \notin C _ { y }$ , since otherwise we would have $z - x = y - b \in T _ { \omega _ { 1 } }$ and $z \in x + T _ { \omega _ { 1 } } \subset T _ { \omega _ { 1 } }$ , contradicting $z = t _ { \omega _ { 1 } } \notin T _ { \omega _ { 1 } }$ 

$| c - z | \notin C _ { z }$ , since otherwise we would have $| - x + t _ { \eta } | = | - x + y | =$ $| c - z | \in C _ { z }$ , contradicting (7.26).  

To motivate the last theorem of this section we need to reformulate Theorem 7.4.1 in another language. For this we need the following definitions. We say that partition $\mathcal { P }$ of R is $\omega$ sum free if for every $x \in \mathbb { R }$ the equation $a + b = x$ has less than $\omega$ solutions with a and b being in the same element of the partition, that is, when for every $x \in \mathbb { R }$ the set 

$$
T _ {x} = \{\langle a, b \rangle : a + b = x \text { and } a, b \in P \text { for   some } P \in \mathcal {P} \}
$$

is finite. Similarly, we say that partition P of R is $\omega$ diference free if the set 

$$
D _ {x} = \{\langle a, b \rangle : a - b = x \text { and } a, b \in P \text { for   some } P \in \mathcal {P} \}
$$

is finite for every $x \in \mathbb { R } , x \neq 0$ 

In this language Theorem 7.4.1 reads as follows. 

Corollary 7.4.5 There exists a countable partition P of R that is $\omega$ sum free. 

Proof It is enough to notice that $T _ { 2 x } = \{ \langle x + h , x - h \rangle \colon | h | \in S _ { x } \cup \{ 0 \} \}$ , where $S _ { x }$ is from Theorem 7.4.1.  

Can we prove the same results about ω-diference-free partitions of R? The answer is given by the next theorem, due to Ciesielski (1996). 

Theorem 7.4.6 The continuum hypothesis is equivalent to the existence of a countable partition P of R that is ω diference free. 

Proof The proof of the theorem is similar to that of Theorem 7.3.9. 

⇐: To obtain a contradiction assume that ${ \mathfrak { c } } \geq \omega _ { 2 }$ and that there exists a countable partition $\mathcal { P }$ of R that is $\omega$ diference free. 

Let H be any Hamel basis. Since $| H | = { \mathfrak { c } } \geq \omega _ { 2 }$ by Lemma 7.3.11 we can choose disjoint sets $A _ { 0 } \in [ H ] ^ { \omega _ { 2 } }$ and $B _ { 0 } \in [ H ] ^ { 2 }$ and $P \in \mathcal { P }$ such that 

$$
a + b \in P \text { for   every } a \in A _ {0} \text { and } b \in B _ {0}.
$$

Take diferent $b _ { 0 } , b _ { 1 } \in B _ { 0 }$ . Then 

$$
(a + b _ {0}) - (a + b _ {1}) = b _ {0} - b _ {1}
$$

for every $a \in A _ { 0 }$ , that is, $D _ { b _ { 0 } - b _ { 1 } }$ contains all pairs $\langle a + b _ { 0 } , a + b _ { 1 } \rangle$ . This contradicts the assumption that $D _ { x }$ is finite for $x = b _ { 0 } - b _ { 1 } \neq 0 .$ 

⇒: Represent R as the union of an increasing sequence $\langle V _ { \alpha } \colon \alpha < \omega _ { 1 } \rangle$ of countable linear subspaces $V _ { \alpha }$ of R over Q such that $\textstyle V _ { \lambda } = \bigcup _ { \alpha < \lambda } V _ { \alpha }$ for every limit ordinal $\lambda ~ < ~ \omega _ { 1 }$ . Such a sequence exists by Lemma 6.1.6(b) applied to the family $\mathcal { F }$ of operations $\langle x , y \rangle \mapsto x + y$ and $x \mapsto q x$ for every $q \in \mathbb { Q }$ . For convenience we will also assume that $V _ { 0 } = \emptyset$ 

Thus $\left\{ V _ { \alpha + 1 } \ : \backslash \ : V _ { \alpha } : \ : \alpha < \omega _ { 1 } \right\}$ is a partition of R into countable sets. For $\alpha < \omega _ { 1 }$ let $\{ p _ { n } ^ { \alpha } \colon n < \omega \}$ be an enumeration of $V _ { \alpha + 1 } \setminus V _ { \alpha }$ . By induction on $\alpha < \omega _ { 1 }$ we will define one-to-one functions $f \colon V _ { \alpha + 1 } \setminus V _ { \alpha } \to \omega$ such that the following inductive condition holds<sup>2</sup> 

$$
f (p _ {n} ^ {\alpha}) \in \omega \setminus \{f (p) \colon p \in V _ {\alpha} \& p = p _ {n} ^ {\alpha} \pm p _ {j} ^ {\alpha} \text { for   some } j \leq n \}.
$$

We will show that the partition $\mathcal { P } = \{ f ^ { - 1 } ( n ) \colon n < \omega \}$ of R is $\omega$ diference free. 

So choose an arbitrary $x = p _ { n } ^ { \xi } \neq 0$ and consider the pairs $\langle a , b \rangle$ satisfying $a - b = x$ with a and b being from the same element of $\mathcal { P }$ , that is, such that $f ( a ) = f ( b )$ . It is enough to show that $\{ a , b \} \cap \{ p _ { i } ^ { \xi } \colon j \leq n \} \neq \emptyset$ 

Let $a \ = \ p _ { m } ^ { \alpha }$ and $b = p _ { k } ^ { \beta }$ . Then $p _ { m } ^ { \alpha } - p _ { k } ^ { \beta } \ = \ p _ { n } ^ { \xi }$ . Notice that $\delta \ =$ max $\{ \xi , \alpha , \beta \}$ must be equal to at least two of $\xi , \alpha .$ , and $\beta$ , since otherwise the number p with the index δ would belong to $V _ { \delta }$ . Moreover, α $\neq \beta .$ , since otherwise $f ( p _ { m } ^ { \alpha } ) = f ( a ) = f ( b ) = f ( p _ { k } ^ { \alpha } )$ , contradicting the fact that f is one-to-one on V \ V . We are left with two cases: 

If $\xi = \alpha > \beta \mathrm { ~ t h e n ~ } p _ { m } ^ { \xi } - p _ { n } ^ { \xi } = a - x = b = p _ { k } ^ { \beta } \in V _ { \xi } . \mathrm { ~ S o ~ } f ( p _ { m } ^ { \xi } ) = f ( a ) =$ $f ( b ) = f ( p _ { m } ^ { \xi } - p _ { n } ^ { \xi } )$ implies that $m < n$ and $a = p _ { m } ^ { \xi } \in \{ p _ { j } ^ { \xi } \colon j \leq n \}$ 

If $\xi = \beta > \alpha$ then $p _ { k } ^ { \xi } + p _ { n } ^ { \xi } = b + x = a = p _ { m } ^ { \alpha } \in V _ { \xi } . \mathrm { ~ S o ~ } f ( p _ { k } ^ { \xi } ) = f ( b ) =$ $f ( a ) = f ( p _ { k } ^ { \xi } + p _ { n } ^ { \xi } )$ implies that $k < n$ and $b = p _ { k } ^ { \xi } \in \{ p _ { j } ^ { \xi } \colon j \leq n \}$  

## EXERCISES

1 Prove that if f is uniformly antisymmetric then it does not have the Baire property. Hint: First prove the following fact due to Kuratowski: 

For every function $f \colon  { \mathbb { R } } \to  { \mathbb { R } }$ with the Baire property there exists a first-category set S such that $f | _ { \mathbb { R } \backslash S } \colon \mathbb { R } \ \backslash \ S \  \ \mathbb { R }$ is continuous. 

2 (Project) Consider the following classes of subsets of R: 

$\boldsymbol { B } = \{ \boldsymbol { B } \subset \mathbb { R } \colon \boldsymbol { B }$ is a Bernstein set}; 

$\mathcal { H } = \{ H \subset \mathbb { R } \colon H$ is a Hamel basis}; 

• V = {V ⊂ R: V is a Vitali set}; 

$\mathcal { T } = \{ T \subset \mathbb { R } \colon B$ is a transcendental basis of R over Q}. 

Moreover, if $\mathcal { F }$ is any of the preceding families let 

$$
\bullet \mathcal {F} ^ {*} = \{F \subset \mathbb {R}: F + F \in \mathcal {F} \}.
$$

Find the complete intersection/subset relations among the classes B, H, V, $\tau , B ^ { * } , \mathcal { H } ^ { * } , \mathcal { V } ^ { * }$ , and $\tau ^ { * }$ 

Part IV 

# When induction is too short

# Chapter 8

# Martin’s axiom

## 8.1 Rasiowa–Sikorski lemma

The previous chapter was devoted to constructing objects by transfinite induction. A typical scheme for such constructions was a diagonalization argument like the following. To find a subset S of a set X concerning a family $\mathcal { P } = \{ P _ { \alpha } : \alpha < \kappa \}$ we chose $S = \{ x _ { \xi } \in X \colon \xi < \kappa \}$ by picking each $x _ { \xi }$ to take care of a set $P _ { \xi }$ . But what can we do if the cardinal κ is too big compared to the freedom of choice of the $x _ { \xi } \mathrm { s }$ ; for example, if the set X has cardinality less than $\kappa ?$ 

There is no absolute answer to this question. In some cases you can do nothing. For example, if you try to construct a subset $S$ of $\omega$ diferent from every set from the family $\mathcal { P } ( \omega ) = \{ B _ { \xi } \colon \xi < { \mathfrak { c } } \}$ , then you are obviously condemned to failure. The inductive construction does not work, since you would have to take care of continuum many conditions, having the freedom to choose only countably many points for S. 

In some other cases you can reduce a family $\mathcal { P }$ to the appropriate size. This was done, for example, in Theorem 6.3.7 (on the existence of Bernstein sets) in which we constructed a nonmeasurable subset B of $\mathbb { R } ^ { n }$ : The natural family $\mathcal { P } = \mathcal { L }$ of cardinality $2 ^ { \mathfrak { c } }$ was replaced by the family $\mathcal { P } _ { 0 } = \{ P \xi : \xi < { \mathfrak { c } } \}$ of all perfect subsets of $\mathbb { R } ^ { n }$ . The dificult part of the proof, that is, Theorem 6.3.6, was to show that the family $\mathcal { P } _ { 0 }$ does the job. 

Yet in other cases, such as Theorems 7.3.9, 7.4.4, and 7.4.6, the induction could be performed in only $\omega _ { 1 }$ steps while we had to take care of a family $\mathcal { P }$ of cardinality c. These cases resulted in us assuming that ${ \mathfrak { c } } = \omega _ { 1 }$ In other words, in order to rescue a diagonal argument, we had to assume an additional set-theoretic assumption, the continuum hypothesis. In fact, in Theorems 7.3.9, 7.4.4, and 7.4.6 we also proved that this assumption was necessary. 

The continuum hypothesis was also assumed in the proof of Theorem 7.2.5. In this theorem, however, we did not show that the continuum hypothesis is a necessary assumption, though we stated that the theorem cannot be proved in ZFC alone. The reason for this is that Theorem 7.2.5 can also be proved under weaker set-theoretic assumptions, which can be true even if the continuum hypothesis fails. 

In remainder of this text we will be mainly interested in studying diferent kinds of set-theoretic axioms that will allow us to solve the problem of having a “too short induction.” For this we will need some more definitions and notations. 

Consider a partially ordered set $\langle \mathbb { P } , \leq \rangle$ . A subset $D \subset \mathbb { P }$ is said to be dense in P provided for every $p \in \mathbb { P }$ there exists a $d \in D$ such that $d \leq p$ 

Examples 1. If $X \neq \emptyset$ and $\langle \mathbb { P } , \leq \rangle = \langle { \mathcal { P } } ( X ) , \subset \rangle$ then $D = \{ \emptyset \}$ is dense in P. Notice that ∅ is the smallest element of P. 

In fact, $D = \{ m \}$ is dense in $\langle \mathbb { P } , \leq \rangle$ if and only if m is the smallest element of P. Also, if $\langle \mathbb { P } , \leq \rangle$ has the smallest element m, then $D \subset \mathbb { P }$ is dense in $\langle \mathbb { P } , \leq \rangle$ if and only if $m \in D$ . Dense sets such as these are too easy to describe to be of much interest. To avoid them, we will usually study partially ordered sets without a smallest element. 

2. If $\langle \mathbb { P } , \leq \rangle = \langle \mathbb { R } , \leq \rangle$ then the set $D = ( - \infty , 0 )$ is dense in $\langle \mathbb { P } , \leq \rangle$ . Notice that the word $^ { 6 } \mathrm { d e n s e } ^ { 3 }$ is used here in a diferent sense than it is usually used for the linearly ordered sets (see (8.1)). However, there will be very little chance to confuse these two notions of density, since we will usually use our new definition of density for partially ordered sets that are not linearly ordered. 

3. Let $\langle X , \tau \rangle$ be any topological space. If $\langle \mathbb { P } , \leq \rangle = \langle \tau \setminus \{ \emptyset \} , \subset \rangle$ then any base B in X is dense in P. 

A subset F of a partially ordered set $\langle \mathbb { P } , \leq \rangle$ is a filter in P if 

(F1) for every $p , q \in F$ there is an $r \in F$ such that $r \le p$ and $r \leq q$ , and 

(F2) if $q \in F$ and $p \in \mathbb { P }$ are such that $q \leq p$ then $p \in F$ 

Note that a simple induction argument shows that condition $( \mathrm { F 1 } )$ is equivalent to the following stronger condition. 

(F1<sup>-</sup>) For every finite subset $F _ { 0 }$ of $F$ there exists an $r \in F$ such that $r \le p$ for every $p \in F _ { 0 }$ 

Examples 1. For any chain F in a partially ordered set $\langle \mathbb { P } , \leq \rangle$ the family 

$$
F ^ {\star} = \{p \in \mathbb {P}: \exists q \in F (q \leq p) \}
$$

is a filter in P. 

2. Let $\mathcal { G }$ be any family of subsets of a nonempty set X that is closed under finite intersections and let $\langle \mathbb { P } , \leq \rangle = \langle \mathcal { G } , \subset \rangle$ . If $x \in X$ then the family $F _ { x } = \{ Y \in \mathcal { G } \colon x \in Y \}$ is a filter in P. A filter F in such $\langle \mathbb { P } , \leq \rangle$ is called a principal filter if it is of this form, that is, if $F = F _ { x }$ for some $x \in X$ 

3. Let G be a nonempty family of subsets of an infinite set X and let $\omega ~ \leq ~ \kappa ~ \leq ~ | X |$ . If G is closed under finite unions then ${ \mathcal { G } } \cap [ X ] ^ { < \kappa }$ is a filter in $\langle \mathbb { P } , \leq \rangle \ = \ \langle \mathcal { G } , \supset \rangle$ . If $\mathcal { G }$ is closed under finite intersections then $F _ { \kappa } = \{ Y \in { \mathcal { G } } \colon | X \setminus Y | < \kappa \}$ is a filter in $\langle \mathbb { P } , \leq \rangle = \langle \mathcal { G } , \subset \rangle$ 

4. Let $\langle \mathbb { P } , \boldsymbol { \leq } \rangle = \langle \mathcal { P } ( \boldsymbol { X } ) , \boldsymbol { \subset } \rangle$ . Then $F \subset \mathbb { P } { \mathrm { ~ i s ~ a ~ } }$ filter in P if $( 1 ) \ A \cap B \in F$ provided $A , B \in F ;$ and (2) if $A \subset B \subset X$ and $A \in F$ then $B \in F$ (Compare this with Exercise 3 in Section 4.4.) 

Before we formulate our next example we introduce the following notation. For nonempty sets X and Y we will use the symbol Func $( X , Y )$ to denote the family of all partial functions from X into $Y$ , that is, 

$$
\operatorname{Func} (X, Y) = \bigcup \left\{Y ^ {D} \colon D \subset X \right\}.
$$

Also, for an infinite cardinal number κ we put 

$$
\operatorname{Func} _ {\kappa} (X, Y) = \bigcup \left\{Y ^ {D}: D \in [ X ] ^ {<   \kappa} \right\} = \left\{s \in \operatorname{Func} (X, Y): | s | <   \kappa \right\}.
$$

5. Let ${ \mathcal { F } } \subset \operatorname { F u n c } ( X , Y )$ be such that for every $g _ { 0 } , g _ { 1 } \in \mathcal { F }$ 

$$
\text { if } g _ {0} \cup g _ {1} \in \operatorname{Func} (X, Y) \text { then } g _ {0} \cup g _ {1} \in \mathcal {F}.
$$

(In particular, ${ \mathrm { F u n c } } _ { \kappa } ( X , Y )$ satisfies this condition.) Then for every $f \in$ Func(X, Y) the set $G _ { f } = \{ g \in { \mathcal { F } } \colon g \subset f \}$ is a filter in $\langle \mathbb { P } , \leq \rangle = \langle { \mathcal F } , \supset \rangle$ . To see (F1) let $g _ { 0 } , g _ { 1 } \in G _ { f }$ . Then g<sub>0</sub> $\cup g _ { 1 } \subset f .$ , so $h = g _ { 0 } \cup g _ { 1 } \in \operatorname { F u n c } ( X , Y )$ Thus $h \in \mathcal { F }$ and, clearly, $h \leq g _ { 0 }$ and $h \leq g _ { 1 }$ . To see (F2) notice that $g \in G _ { f } , h \in \mathcal { F }$ , and $g \leq h$ imply that $h \subset g \subset f$ , so $h \in G _ { f }$ 

In what follows we will very often use the following fact. Its main part can be viewed as a kind of converse of the previous Example 5. 

Proposition 8.1.1 Let $\langle \mathbb { P } , \leq \rangle = \langle { \mathcal F } , \supset \rangle$ for some ${ \mathcal { F } } \subset \operatorname { F u n c } ( X , Y )$ . If $F \subset \mathbb { P }$ is a filter in P then $f = \bigcup F$ is a function and $F \subset \{ g \in { \mathcal { F } } \colon g \subset f \}$ Moreover, 

(a) if F intersects every set $D _ { x } = \{ s \in \mathbb { P } \colon x \in \operatorname { d o m } ( s ) \}$ for $x \in X$ then $\operatorname { d o m } ( f ) = X$ ; 

(b) if F intersects every set $R _ { y } = \{ s \in \mathbb { P } \colon y \in \mathrm { r a n g e } ( s ) \}$ for $y \in Y$ then $\operatorname { r a n g e } ( f ) = Y$ 

Proof Let $F \subset \mathbb { P }$ be a filter in P and let $g _ { 0 } , g _ { 1 } \in F$ . To prove that $f$ is a function it is enough to show that $g _ { 0 } ( x ) = g _ { 1 } ( x )$ for every $x \in$ dom $( g _ { 0 } ) \cap$ dom(g ). So let $x \in \mathrm { d o m } ( g _ { 0 } ) \cap \mathrm { d o m } ( g _ { 1 } )$ and let $h \in F$ be such that $h \leq g _ { 0 }$ and $h \leq g _ { 1 }$ . Then $h \supset g _ { 0 }$ and $h \supset g _ { 1 }$ . In particular, $x \in \operatorname { d o m } ( h )$ and $g _ { 0 } ( x ) = h ( x ) = g _ { 1 } ( x )$ 

The inclusion $F \subset \{ g \in { \mathcal { F } } \colon g \subset f \}$ is obvious. 

To see (a) let $x \in X$ . Then there exists an $s \in F \cap D _ { x }$ . But $s \subset f .$ , so $x \in \operatorname { d o m } ( s ) \subset \operatorname { d o m } ( f )$ 

Condition (b) is proved similarly. 

In what follows we will often use filters in partially ordered sets to construct functions in a manner similar to that of Proposition 8.1.1. Usually we will be interested in the entire functions, and part (a) of Proposition 8.1.1 suggests how to achieve this goal. This and the next theorem lead to the following definition. 

Let $\langle \mathbb { P } , \leq \rangle$ be a partially ordered set and let D be a family of dense subsets of P. We say that a filter $F$ in $\mathbb { P }$ is D-generic if 

$$
F \cap D \neq \emptyset \text {   for   all   } D \in \mathcal {D}.
$$

The partial orders used in the context of D-generic filters will often be called forcings. Also, if $\langle \mathbb { P } , \leq \rangle$ is a forcing then elements of $\mathbb { P }$ will sometimes be referred to as conditions. For conditions $p , q \in \mathbb { P }$ we say that p is stronger than q provided $p \leq q$ 

In this terminology, if all sets $D _ { x }$ are dense in $\mathbb { P }$ and $\{ D _ { x } \colon x \in \ X \} \subset { \mathcal { D } }$ then for every D-generic filter $F$ in $\mathbb { P }$ the domain of $f = \bigcup F$ is equal to X, that is, $f \colon X \to Y$ . Similarly, if all sets $R _ { y }$ are dense in $\mathbb { P }$ and $\{ R _ { y } \colon y \in \ Y \} \subset { \mathcal { D } }$ then range $( \cup F ) = Y$ for every D-generic filter $F$ in $\mathbb { P } .$ 

The next theorem, due to Rasiowa and Sikorski, shows that there are some interesting D-generic filters. 

Theorem 8.1.2 (Rasiowa–Sikorski lemma) Let $\langle \mathbb { P } , \leq \rangle$ be a partially ordered set and $p \in \mathbb { P }$ . If D is a countable family of dense subsets of P then there exists a D-generic filter F in $\mathbb { P }$ such that $p \in F$ 

Proof Let $\mathcal { D } = \{ D _ { n } \colon n < \omega \}$ . We define a sequence $\langle p _ { n } \colon n \ < \ \omega \rangle$ by induction on $n < \omega$ . We start by picking $p _ { 0 } \in D _ { 0 }$ such that $p _ { 0 } \leq p .$ . We continue by choosing $p _ { n + 1 } \in D _ { n + 1 }$ such that $p _ { n + 1 } \leq p _ { n }$ 

Now let $E = \{ p _ { n } : n < \omega \}$ and put $F = E ^ { \star } = \{ p \in \mathbb { P } \colon \exists q \in E ( q \leq p ) \}$ Then $F$ is a filter in P intersecting every $D \in \mathcal { D }$  

The Rasiowa–Sikorski lemma is one of the most fundamental facts that will be used in the remaining sections. Its importance, however, does not come from its power. Its proof is too simple for this. It is the language of generic filters it employs that makes it so useful. In particular, it motivates the diferent generalizations described in the next sections, which are consistent with ZFC and can be used for our problem of a “too short induction.” 

In most of the applications of the Rasiowa–Sikorski lemma and its generalizations the intuition behind the proofs comes from an attempt at proving the theorem by (transfinite) induction. More precisely, a partial order $\mathbb { P }$ used to construct an object will usually be built on the basis of an attempted inductive construction of the object. That is, conditions (elements of P) will be chosen as a “description of the current stage of induction.” The inductive steps will be related to the dense subsets of P in the sense that the density of a particular set $D _ { x } = \{ p \in \mathbb { P } \colon \varphi ( p , x ) \}$ will be equivalen to the fact that at an arbitrary stage q of the inductive construction we can make the next inductive step by extending the condition q to p having the property $\varphi ( p , x )$ . In particular, the family D of dense subsets of P will always represent the set of all inductive conditions of which we have to take care, and a D-generic filter in P will be an “oracle” that “takes care of all our problems,” and from which we will recover the desired object. 

Evidently, if the number |D| of conditions we have to take care of is not more than the number of steps in our induction, then usually the (transfinite) induction will be powerful enough to construct the object, and the language of forcing will be redundant. In particular, this will be the case for all the applications of the Rasiowa–Sikorski lemma presented in the rest of this section. These applications, however, are presented here to see the use of the generic-filters technique in the simplest situations. Moreover, in the next sections the same theorems will be either generalized or used for some motivation. 

To state the next theorem let us recall that, for a linearly ordered set $\langle X , \leq \rangle$ , a subset D of X is dense in X if 

for every x, $y \in X$ with $x < y$ there is a $d \in D$ such that $x < d < y$ . (8.1) 

A linearly ordered set $\langle X , \leq \rangle$ is said to be dense if it is dense in itself, that is, if X is dense in X. 

Theorem 8.1.3 Any two countable dense linearly ordered sets, neither of which has a first or a last element, are order isomorphic. 

Proof Let $\langle X , \leq \rangle$ and $\langle Y , \preceq \rangle$ be two linearly ordered sets as in the theorem. The inductive proof of the theorem may go as follows. Enumerate X and $Y$ as $X = \{ x _ { n } : n < \omega \}$ and $Y = \{ y _ { n } \colon n < \omega \}$ . Construct, by induction on $n < \omega .$ , a sequence $h _ { 0 } \subset h _ { 1 } \subset h _ { 2 } \subset \cdots$ of functions such that each $h _ { n }$ is an order isomorphism between $X _ { n } \in [ X ] ^ { < \omega }$ and $Y _ { n } \in [ Y ] ^ { < \omega }$ , where $x _ { n } \in X _ { n }$ and $y _ { n } \in Y _ { n }$ for every $n < \omega$ . Then $h = \textstyle \bigcup _ { n < \omega } h _ { n }$ is an order isomorphism between X and $Y$ . The dificult part of the proof is to extend $h _ { n }$ to $h _ { n + 1 }$ while maintaining the condition $x _ { n + 1 } \in X _ { n + 1 }$ and $y _ { n + 1 } \in Y _ { n + 1 }$ 

To translate this proof into the language of partially ordered sets, let $\mathbb { P }$ be the set of all possible functions $h _ { n } \colon X _ { n } \to Y _ { n }$ from our inductive construction, that is, the set of all finite partial isomorphisms from X to $Y$ : 

$$
\mathbb {P} = \{h \in \operatorname{Func} _ {\omega} (X, Y): h \text {   is   strictly   increasing } \}.
$$

Consider $\mathbb { P }$ to be ordered by reverse inclusion, that is, $\langle \mathbb { P } , \leq \rangle = \langle \mathbb { P } , \supset \rangle$ . For $x \in X$ and $y \in Y$ put 

$$
D _ {x} = \{h \in \mathbb {P} \colon x \in \operatorname{dom} (h) \} \quad \text { and } \quad R _ {y} = \{h \in \mathbb {P} \colon y \in \operatorname{range} (h) \}.
$$

These sets are the counterparts of the conditions $^ { \mathfrak { s } } x _ { n } \in X _ { n } ^ { \mathfrak { s } }$ and $^ { 6 } y _ { n } \in Y _ { n }$ We will show that 

$$
\text { the   sets } D _ {x} \text { and } R _ {y} \text { are   dense   in } \mathbb {P},\tag{8.2}
$$

which is a translation of the fact that the inductive step of our inductive construction can always be made. 

Before we prove (8.2), let us show how it implies the theorem. Let ${ \mathcal { D } } = \{ D _ { x } \colon x \in X \} \cup \{ R _ { y } \colon y \in Y \}$ . Then $\mathcal { D }$ is countable since the sets $X$ and $Y$ are countable. Thus, by the Rasiowa–Sikorski lemma, there exists a D-generic filter $F$ in P. Then, by Proposition 8.1.1, $f = \bigcup F$ is a function from X onto Y. It remains only to show that f is strictly increasing. 

To see this, let $x _ { 0 } , x _ { 1 } \in X$ with $x _ { 0 } < x _ { 1 }$ . Then there are $g _ { 0 } , g _ { 1 } \in F$ such that $x _ { 0 } \in \operatorname { d o m } ( g _ { 0 } )$ and $x _ { 1 } \in \operatorname { d o m } ( g _ { 1 } )$ . Let $g \in F$ be such that $g \le g _ { 0 }$ and $g \leq g _ { 1 }$ . Then $g _ { 0 } \cup g _ { 1 } \subset g \subset f$ . So $f ( x _ { 0 } ) = g ( x _ { 0 } ) \prec g ( x _ { 1 } ) = f ( x _ { 1 } )$ since g is strictly increasing. Thus f is strictly increasing. We have proved that $f \colon X \to Y$ is an order isomorphism. 

To finish the proof it is enough to show (8.2). So let $x \in X$ . To prove that $D _ { x }$ is dense, let $g \in \mathbb { P }$ . We have to find $h \in D _ { x }$ such that $h \leq g$ , that is, a function $h \in \mathbb { P }$ such that $h \supset g$ and $x \in \operatorname { d o m } ( h )$ . If $x \in \operatorname { d o m } ( g )$ then $h = g$ works. So assume that $x \not \in \operatorname { d o m } ( g )$ . Let dom $( g ) = \{ x _ { 0 } , x _ { 1 } , \ldots , x _ { n } \}$ with $x _ { 0 } < x _ { 1 } < \cdot \cdot \cdot < x _ { n }$ and let $y _ { i } = g ( x _ { i } )$ for $i \leq n$ . Then $y _ { 0 } \prec y _ { 1 } \prec \cdot \cdot \cdot \prec y _ { n } .$ since g is strictly increasing. We will define $h$ as $g \cup \{ \langle x , y \rangle \}$ , where $y \in Y$ is chosen in such a way that h is strictly increasing. To do this, it is enough to pick $y \in Y \setminus \{ y _ { 0 } , y _ { 1 } , . . . \mathrm { ~ , ~ } y _ { n } \}$ such that the following holds for every $i \leq n \colon$ 

$$
x <   x _ {i} \Leftrightarrow y \prec y _ {i}.\tag{8.3}
$$

If $x < x _ { 0 }$ , pick $y \prec  { y _ { 0 } }$ . Such y exists, since $Y$ does not have a smallest element. If $x > x _ { n }$ , pick $y \succ y _ { n }$ , which exists since $Y$ does not have a largest element. So assume that $x _ { i } < x < x _ { i + 1 }$ for some $i < n$ . Then choose $y \in Y$ such that $y _ { i } \prec y \prec y _ { i + 1 }$ , which exists since $Y$ is dense. It is easy to see that such $y$ satisfies (8.3). 

We have proved that each $D _ { x }$ is dense in $\mathbb { P } .$ . The proof that every $R _ { y }$ is dense in $\mathbb { P }$ is almost identical, and is left as an exercise.  

Evidently $\langle \mathbb { Q } , \leq \rangle$ is an example of a dense linearly ordered set with neither a first nor a last element. Thus Theorem 8.1.3 says that any countable linearly ordered dense set without a first or a last element is isomorphic to $\langle \mathbb { Q } , \leq \rangle$ . The order type of this class is usually denoted by the letter η. 

In fact, it can be proved that $\langle \mathbb { Q } , \leq \rangle$ is universal for the class of all countable linearly ordered sets, in the sense that every countable linearly ordered set is isomorphic to $\langle S , \leq \rangle$ for some $S \subset \mathbb { Q }$ (see Exercise 1). 

Clearly, $\langle \mathbb { R } , \leq \rangle$ is not isomorphic to $\langle \mathbb { Q } , \leq \rangle$ . The order type of $\langle \mathbb { R } , \leq \rangle$ is usually denoted by λ. To give a characterization of the order type λ similar to that of Theorem 8.1.3 we will need the following definition. A linearly ordered set $\langle X , \leq \rangle$ is said to be complete if every subset of X that is bounded from above has a least upper bound. That is, if the set $B ( S ) = \{ b \in X \colon \forall x \in S ( x \leq b ) \}$ is not empty for some $S \subset X$ then $B ( S )$ has a least element, denoted by sup $S$ . It is a fundamental fact that $\langle \mathbb { R } , \leq \rangle$ is complete. 

Theorem 8.1.4 Any two complete linearly ordered sets both having countable dense subsets, and having neither a least nor a largest element, are order isomorphic. 

Proof Let $\langle X , \leq \rangle$ and $\langle Y , \preceq \rangle$ be linearly ordered sets as described in the theorem. Let $X _ { 0 }$ and $Y _ { 0 }$ be countable dense subsets of $X$ and $Y .$ , respectively. It is easy to see that $X _ { 0 }$ and $Y _ { 0 }$ satisfy the assumptions of Theorem 8.1.3. 

Let $f _ { 0 } \colon X _ { 0 } \to Y _ { 0 }$ be an order isomorphism between $\langle X _ { 0 } , \leq \rangle$ and $\langle Y _ { 0 } , \preceq \rangle$ Define $f \colon X \to Y$ by $f ( x ) = \operatorname* { s u p } \{ f _ { 0 } ( x _ { 0 } ) \colon x _ { 0 } \in X _ { 0 } \ \& \ x _ { 0 } \leq x \}$ . It is not dificult to prove that f is an order isomorphism. The details are left as an exercise.  

The next theorem will show that we can also use the Rasiowa–Sikorski lemma in proofs by transfinite induction. To formulate it we need the following definition. For $f , g \colon \omega  \omega$ we define 

$$
f <   ^ {\star} g \Leftrightarrow f (n) <   g (n) \text {   for   all   but   finitely   many   } n <   \omega .\tag{8.4}
$$

It is easy to see that the relation $< ^ { \star }$ is transitive on $\omega ^ { \omega }$ 

Theorem 8.1.5 If $G \subset \omega ^ { \omega }$ has cardinality $\leq \omega _ { 1 }$ then there exists $a < ^ { \star } -$ increasing sequence $\langle f _ { \xi } \colon \xi < \omega _ { 1 } \rangle$ such that for every $g \in G$ there exists a $\xi < \omega _ { 1 }$ with $g < ^ { \star } ~ f _ { \xi }$ 

Before we prove it, notice first that it immediately implies the following corollary. For its formulation we need the following definition. A sequence $\langle f _ { \xi } \in \omega ^ { \omega } \colon \xi < \kappa \rangle$ is called a scale in $\omega ^ { \omega }$ if it is $< ^ { \star }$ -increasing and if for every $g \in \omega ^ { \omega }$ there exists a $\xi < \kappa$ such that $g < ^ { \star } ~ f _ { \xi }$ 

Corollary 8.1.6 Ifthe continuum hypothesis holds then there exists a scale $\langle f _ { \xi } \in \omega ^ { \omega } : \xi < { \mathfrak { c } } \rangle$ 

In the next section we will show that Corollary 8.1.6 can also be proved when the continuum hypothesis is false. 

The proof of Theorem 8.1.5 will be based on two lemmas. The first of these lemmas is not essential for the proof, but it serves as a good approximation for the second one. 

Lemma 8.1.7 If $G \subset \omega ^ { \omega }$ has cardinality $\leq \omega$ then there exists an $f \in \omega ^ { \omega }$ such that for every $g \in G$ 

$$
g (n) <   f (n) \text {   for   infinitely   many   } n <   \omega .
$$

Proof $\mathrm { A n }$ inductive construction of such f can be done as follows. Let $G \times \omega = \{ \langle g _ { n } , k _ { n } \rangle \colon n < \omega \}$ . Construct a sequence $f _ { 0 } \subset f _ { 1 } \subset f _ { 2 } \subset \cdots$ of functions such that each $f _ { n } \in \mathrm { F u n c } _ { \omega } ( \omega , \omega )$ and for every $n < \omega$ there exists an $m \in \operatorname { d o m } ( f _ { n } )$ with $m \geq k _ { n }$ such that $f _ { n } ( m ) > g _ { n } ( m )$ . Then $\begin{array} { r } { \hat { f } = \bigcup _ { n < \omega } f _ { n } \in \operatorname { F u n c } ( \omega , \omega ) } \end{array}$ and any extension $f$ of $\hat { f }$ to $\omega$ has the desired property, since for every $g \in G$ and $k < \omega$ there exists an $m \geq k$ with $f ( m ) > g ( m )$ 

To translate this proof into the language of partially ordered sets, let $\mathbb { P }$ be the set of all possible functions $f _ { n }$ as before, that is, take 

$$
\mathbb {P} = \operatorname{Func} _ {\omega} (\omega , \omega),
$$

and order it by reverse inclusion ⊃. For $g \in \omega ^ { \omega }$ and $k < \omega$ define 

$$
D _ {g} ^ {k} = \{s \in \mathbb {P}: \exists m \geq k (m \in \operatorname{dom} (s) \& s (m) > g (m)) \}.
$$

These sets are the counterparts of the inductive condition $^ { * } f _ { n } ( m ) > g _ { n } ( m )$ for some $m \geq k _ { n } . ^ { \prime \prime }$ 

Notice that the sets $D _ { g } ^ { k }$ are dense in P, since for every $t \in \mathbb { P }$ there exists an $m \in \omega \setminus ( k \cup \mathrm { d o m } ( t ) )$ and for $s = t \cup \{ \langle m , g ( m ) + 1 \rangle \}$ we have $s \in D _ { g } ^ { k }$ and $s \leq t$ 

Let ${ \mathcal { D } } = \{ D _ { a } ^ { k } \colon k < \omega \ \& \ g \in G \}$ and let $F$ be a D-generic filter in P. Then, by Proposition $8 . 1 . 1 , \bigcup F$ is a function. Let $f \colon \omega  \omega$ be any extension of $\cup F$ . Then f has the desired property, since for every $g \in G$ and $k < \omega$ there are $s \in F \cap D _ { g } ^ { k }$ and $m \geq k$ such that $f ( m ) = s ( m ) > g ( m )$  

The lemma that we really need for the proof of Theorem 8.1.5 is the following. 

Lemma 8.1.8 $H G \subset \omega ^ { \omega }$ has cardinality $\leq \omega$ then there exists an $f \in \omega ^ { \omega }$ such that 

$$
g <   ^ {\star} f \text {   for   every   } g \in G.
$$

Proof An inductive construction of such f can be done as follows. Let $G = \{ g _ { n } \colon n < \omega \}$ and $\omega = \{ x _ { n } : n < \omega \}$ . Construct a sequence $f _ { 0 } \subset f _ { 1 } \subset$ $f _ { 2 } \subset \cdots$ of functions such that $f _ { n } \in \operatorname { F u n c } _ { \omega } ( \omega , \omega )$ and $x _ { n } \in$ dom $\left( f _ { n } \right)$ for every $n < \omega$ . Moreover, at the inductive step $n < \omega$ choose $f _ { n }$ such that $f _ { n } ( x ) > g _ { i } ( x )$ for all functions $g _ { i }$ looked at so far and all numbers x that have not yet been considered up to this point of the induction, that is, such that 

$$
f _ {n} (x) > g _ {i} (x) \text { for   all } x \in \operatorname{dom} (f _ {n}) \setminus \operatorname{dom} (f _ {n - 1}) \text { and } i <   n.\tag{8.5}
$$

Then $\begin{array} { r } { f = \bigcup _ { n < \omega } f _ { n } \colon \omega  \omega } \end{array}$ and $g _ { i } < ^ { \star }$ f for every $i < \omega$ 

One problem in finding an appropriate forcing for this construction is that the “current stage of induction” includes information not only on “functions $f _ { n }$ constructed so $\mathrm { f a r } ^ { \prime \prime }$ but also on “all functions $g _ { i }$ considered so far.” The first part of this information is included in functions from $\mathbb { P } = \operatorname { F u n c } _ { \omega } ( \omega , \omega )$ , as in Lemma 8.1.7. However, we need the second piece of information as well, which is to be coded by finite subsets of $G .$ . Thus we define the partially ordered set $\mathbb { P } ^ { \star } = \mathbb { P } \times [ G ] ^ { < \omega }$ . Moreover, the partial order on $\mathbb { P } ^ { \star }$ , in order to describe the extension as in (8.5), must be defined as follows. For $\langle s , A \rangle , \langle t , B \rangle \in \mathbb { P } ^ { \star }$ we define $\langle s , A \rangle \leq \langle t , B \rangle$ provided $s \supset t$ $A \supset B$ , and 

$$
s (n) > g (n) \text { for   all } n \in \operatorname{dom} (s) \setminus \operatorname{dom} (t) \text { and } g \in B.\tag{8.6}
$$

Now the inductive conditions $^ { \mathfrak { a } } x _ { n } \in \mathrm { d o m } ( f _ { n } ) ^ { \mathfrak { n } }$ and “every element $g$ of $G$ is taken care of at some stage of the induction” are coded by the following subsets of $\mathbb { P } ^ { \star }$ : 

$$
D _ {n} = \{\langle s, A \rangle \in \mathbb {P} ^ {\star}: n \in \operatorname{dom} (s) \} \quad \text { and } \quad E _ {g} = \{\langle s, A \rangle \in \mathbb {P} ^ {\star}: g \in A \},
$$

where $g \in G \subset \omega ^ { \omega }$ and $n < \omega$ 

The sets $E _ { g }$ are dense in $\mathbb { P } ^ { \star }$ , since for every $\langle s , A \rangle \in \mathbb { P } ^ { \star }$ we can pick $\langle s , A \cup \{ g \} \rangle \in E _ { g }$ and clearly $\langle s , A \cup \{ g \} \rangle \leq \langle s , A \rangle$ , as condition (8.6) is then satisfied vacuously. 

To see that a set $D _ { n }$ is dense in $\mathbb { P } ^ { \star }$ take $p = \langle t , A \rangle \in \mathbb { P } ^ { \star }$ . We have to find $q \in D _ { n }$ such that $q \leq p$ . If $n \in \mathrm { d o m } ( t )$ then $p \in D _ { n }$ and $q = p$ works. So assume that $n \not \in \mathrm { d o m } ( t )$ . Define $q = \langle s , A \rangle \in D _ { n }$ with $s = t \cup \{ \langle n , k \rangle \}$ and $k = \operatorname* { s u p } \{ g ( n ) + 1 \colon g \in A \}$ . Then $q \leq p ,$ since clearly $s \supset t , A \supset A$ and (8.6) holds, $\operatorname { a s } s ( n ) = k > g ( n )$ for all $g \in A$ 

Now let ${ \mathcal { D } } = \{ D _ { n } \colon n < \omega \} \cup \{ E _ { q } \colon g \in G \}$ . Then D is a countable family of dense subsets of $\mathbb { P } ^ { \star }$ so, by the Rasiowa–Sikorski lemma, we can find a D-generic filter $F$ in $\mathbb { P } ^ { \star }$ . Notice that $F _ { 0 } = \{ s \colon \langle s , A \rangle \in F \}$ is a filter in P. Thus, by Proposition 8.1.1, $f = \bigcup F _ { 0 }$ is a function. Notice also that $D _ { n } \cap F \neq \emptyset$ implies $n \in \operatorname { d o m } ( f )$ . Therefore $f$ maps $\omega$ into itself. 

To finish the proof it is enough to show that $g < ^ { \star } \ f$ for every $g \in G$ So let $g \in G$ . Then there exists $\langle t , B \rangle \in F \cap E _ { g }$ . We will prove that 

$$
f (n) > g (n) \text { for   every } n \in \omega \setminus \operatorname{dom} (t).
$$

This is the case since for every $n \in \omega$ \ dom(t) there is $\langle t ^ { \prime } , B ^ { \prime } \rangle \in F \cap D _ { n }$ Take $\langle s , A \rangle \in F$ with $\langle s , A \rangle \leq \langle t , B \rangle$ and $\langle s , A \rangle \leq \langle t ^ { \prime } , B ^ { \prime } \rangle$ . Then $n \in$ dom $( t ^ { \prime } ) \subset \mathrm { d o m } ( s )$ so $n \in \mathrm { d o m } ( s ) \setminus \mathrm { d o m } ( t )$ and $g \in B$ . Therefore condition (8.6) for $\langle s , A \rangle \leq \langle t , B \rangle$ implies that $f ( n ) = s ( n ) > g ( n )$  

Proof of Theorem 8.1.5 Let $G = \{ g _ { \xi } \colon \xi < \omega _ { 1 } \}$ . Define $\langle f _ { \xi } \colon \xi < \omega _ { 1 } \rangle$ by induction on $\xi < \omega _ { 1 }$ by choosing $f _ { \xi }$ as the function $f$ from Lemma 8.1.8 applied to $G = \{ f _ { \zeta } \colon \zeta < \xi \} \cup \{ g _ { \zeta } \colon \zeta < \xi \}$ . It is easy to see that this sequence has the desired property.  

## EXERCISES

1 Prove that for every countable linearly ordered set $\langle X , \preceq \rangle$ there exists a strictly increasing function $f \colon X \to \mathbb { Q }$ . (Such a function f is said to be an order embedding of X into Q, and it establishes an order isomorphism between $\langle X , \preceq \rangle$ and $\langle f [ X ] , \leq \rangle . )$ 

2 Prove that $\langle \mathbb { R } , \leq \rangle$ is complete as a linearly ordered set (use Dedekind’s definition of real numbers). 

3 Complete the details of the proof of Theorem 8.1.4 by showing that 

(a) the sets $X _ { 0 }$ and $Y _ { 0 }$ are dense in themselves and have neither least nor largest elements; 

(b) the function $f \colon X \to Y$ is an order isomorphism. 

4 A subset D of a linearly ordered set $\langle X , \leq \rangle$ is weakly dense if 

for every $x , y \in X$ with $x < y$ there is a $d \in D$ such that $x \leq d \leq y$ 

Prove that for every linearly ordered set $\langle X , \leq \rangle$ containing a countable weakly dense subset there exists a strictly increasing function $f \colon X \to \mathbb { R }$ 

5 Prove that the relation $\leq$ defined on the set $\mathbb { P } ^ { \star }$ as in Lemma 8.1.8 is indeed a partial-order relation. 

6 For $f , g \colon \omega  \omega$ we define 

$$
f \leq^ {\star} g \Leftrightarrow f (n) \leq g (n) \text {   for   all   but   finitely   many   } n <   \omega .
$$

Show that $\leq ^ { \star }$ is a preorder relation on $\omega ^ { \omega }$ (see Exercise 4 from Section 2.4). The equivalence relation generated by $\leq ^ { \star }$ is usually denoted by $= ^ { \star }$ . Show also that the partial-order relation $\preceq ^ { \star }$ induced by $\leq ^ { \star }$ on the family of all equivalence classes of $= ^ { \star }$ is a linear-order relation. 

## 8.2 Martin’s axiom

In this section we would like to introduce an axiom that says that in a large number of situations the statement “for countably many” can be replaced by “for less than continuum many,” even when the continuum hypothesis fails. 

In particular, we would like to be able to make such a replacement in the Rasiowa–Sikorski lemma, which leads us to the following statement. 

(G) Let $\langle \mathbb { P } , \leq \rangle$ be a partially ordered set. If D is a family of dense subsets of $\mathbb { P }$ such that $| \mathcal { D } | < { \mathfrak { c } }$ , then there exists a D-generic filter F in $\mathbb { P } .$ 

Clearly $( { \star } )$ is implied by the continuum hypothesis. However, it is false under the negation of the continuum hypothesis. To see it, consider the partially ordered set $\langle \mathbb { P } , \Xi \rangle = \langle \mathrm { F u n c } _ { \omega } ( \omega , \omega _ { 1 } ) , \supset \rangle$ and, for $\xi < \omega _ { 1 }$ , the sets $R _ { \xi } = \{ s \in \mathbb { P } \colon \xi \in$ range(s)}. Each set $R _ { \xi }$ is dense, since for every $s \in \mathbb { P }$ we have $t = s \cup \{ \langle n , \xi \rangle \} \in R _ { \xi }$ and $t \leq s$ for any $n \in \omega \setminus \mathrm { d o m } ( s )$ . But $\mathcal { D } = \{ R _ { \xi } \colon \xi < \omega _ { 1 } \}$ has cardinality $\leq \omega _ { 1 } < { \mathfrak { c } }$ . So (G) implies the existence of a D-generic filter $F$ in $\mathbb { P } .$ , and, by Proposition 8.1.1, F is a function from a subset of $\omega$ onto $\omega _ { 1 }$ . This is clearly impossible. 

Thus, in order to find a (G)-like axiom that is consistent with the negation of the continuum hypothesis we will have to restrict the class of partially ordered sets allowed in its statement. In particular, we will have to exclude forcings such as $\langle \mathrm { F u n c } _ { \omega } ( \omega , \omega _ { 1 } ) , \supset \rangle$ . To define such a class we need some new definitions. 

Let $\langle \mathbb { P } , \leq \rangle$ be a partially ordered set. 

• x, $y \in \mathbb { P }$ are comparable if either $x \leq y \ \mathrm { o r } \ y \leq x$ . Thus a chain in $\mathbb { P }$ is a subset of P of pairwise-comparable elements. 

$x , y \in \mathbb { P }$ are compatible (in P) if there exists ${ \mathrm { ~ a ~ } } z \in \mathbb { P }$ such that $z \leq x$ and $z \le y$ . In particular, condition (F1) from the definition of a filter says that any two elements of a filter F are compatible in $F$ 

• x, $y \in \mathbb { P }$ are incompatible if they are not compatible. 

• A subset A of $\mathbb { P }$ is an antichain (in P) if every two distinct elements of A are incompatible. An antichain is maximal if it is not a proper subset of any other antichain. An elementary application of the Hausdorf maximal principle shows that every antichain in $\mathbb { P }$ is contained in some maximal antichain. 

To illustrate these notions consider $\langle \mathbb { P } , \leq \rangle = \langle \mathrm { F u n c } _ { \omega } ( X , Y ) , \supset \rangle$ . Then $s , t \in \mathbb { P }$ are compatible if and only if $s \cup t \in \mathrm { F u n c } _ { \omega } ( X , Y )$ Therefore elements $s , t \in \mathbb { P }$ are incompatible if there exists an $x \in \operatorname { d o m } ( s )$ ∩ dom(t) such that $s ( x ) \neq t ( x )$ . For any nonempty $D \in [ X ] ^ { < \omega }$ the set $\overset { \cdot } { A } = \overset { \cdot } { Y } ^ { D }$ is a maximal antichain. On the other hand, if $C \subset \mathbb { P }$ is a family of functions with pairwise-disjoint domains, then any two elements of C are compatible. 

The forcings that will be used in our (G)-like axiom are defined in terms of antichains in the following way. 

• A partially ordered set $\langle \mathbb { P } , \leq \rangle$ is ccc (or satisfies the countable chain condition) if every antichain of P is at most countable.<sup>1</sup> 

Clearly, every countable partially ordered set is ccc. In particular, the forcing $\langle \mathbb { P } , \Xi \rangle = \langle \mathrm { F u n c } _ { \omega } ( \omega , \omega ) , \supset \rangle$ from Lemma 8.1.7 is ccc. Notice also that the forcing 

$$
\mathbb {P} ^ {\star} = \mathbb {P} \times [ G ] ^ {<   \omega} \text {   from   Lemma   8.1.8   is   ccc }\tag{8.7}
$$

for an arbitrary $G \subset \omega ^ { \omega }$ , including $G = \omega ^ { \omega }$ To see this, take an uncountable subset $A = \{ p _ { \xi } \in \mathbb { P } ^ { \star } \colon \xi < \omega _ { 1 } \}$ of $\mathbb { P } ^ { \star }$ with $p _ { \xi } = \langle s _ { \xi } , A _ { \xi } \rangle$ and notice that there must be a $\zeta < \xi < \omega _ { 1 }$ such that $s _ { \zeta } = s _ { \xi }$ . But then, for $p = \langle s _ { \zeta } , A _ { \zeta } \cup A _ { \xi } \rangle \in \mathbb { P } ^ { \star }$ we have $p \leq p _ { \zeta }$ and $p \leq p _ { \xi }$ , condition (8.6) being satisfied vacuously. So A is not an antichain. 

On the other hand, the forcing $\langle \mathbb { P } , \Xi \rangle = \langle \mathrm { F u n c } _ { \omega } ( \omega , \omega _ { 1 } ) , \supset \rangle$ is not ccc, since $\{ \{ \langle 0 , \xi \rangle \} \in \mathbb { P } \colon \xi < \omega _ { 1 } \}$ is an uncountable antichain in P. Thus, restricting (G) to the ccc forcings removes the immediate threat of the previously described contradiction with ¬CH, the negation of the continuum hypothesis. In fact such a restriction also removes all possibility of any contradiction with ¬CH. More precisely, consider the following axiom, known as Martin’s axiom and usually abbreviated by MA. 

Martin’s axiom Let $\langle \mathbb { P } , \leq \rangle$ be a ccc partially ordered set. If D is a family of dense subsets of $\mathbb { P }$ such that $| \mathcal { D } | < { \mathfrak { c } }$ , then there exists a D-generic filter $F$ in P. 

Clearly CH implies MA. But MA is also consistent with ZFC and ${ \neg } \mathrm { C H }$ , as stated by the next theorem. 

Theorem 8.2.1 Martin’s axiom plus the negation of the continuum hypothesis $M A \mathrel { + } \lnot C H$ is consistent with ZFC set theory. 

The proof of Theorem 8.2.1 will be postponed until Section 9.5 where we will prove that MA is consistent with ${ \mathfrak { c } } = \omega _ { 2 }$ . However, the same proof can be used to prove the consistency of MA with ${ \mathfrak { c } } = \kappa$ for most regular cardinals κ. 

In the remainder of this section we will see several consequences of MA. First we will see the following generalization of Corollary 8.1.6. 

Theorem 8.2.2 If MA holds then there exists a scale $\langle f _ { \xi } \in \omega ^ { \omega } : \xi < { \mathfrak { c } } \rangle$ 

Proof The argument is essentially identical to that for Theorem 8.1.5. First notice that the following generalization of Lemma 8.1.8 is implied by Martin’s axiom. 

(I) If $G \subset \omega ^ { \omega }$ has cardinality $< \mathfrak { c }$ then there exists an $f \in \omega ^ { \omega }$ such that $g < ^ { \star } ~ f$ for every $g \in G$ 

To see why, consider the forcing $\mathbb { P } ^ { \star } = \operatorname { F u n c } _ { \omega } ( \omega , \omega ) \times [ G ] ^ { < \omega }$ defined as in Lemma 8.1.8, that is, ordered by 

$$
\langle s, A \rangle \leq \langle t, B \rangle \Leftrightarrow s \supset t \& A \supset B
$$

$\begin{array} { r } { \& s ( n ) > g ( n ) } \end{array}$ for all $n \in \mathrm { d o m } ( s ) \ \backslash$ dom(t) and $g \in B$ 

and its dense subsets 

$$
D _ {n} = \{\langle s, A \rangle \in \mathbb {P} ^ {\star}: n \in \operatorname{dom} (s) \} \quad \text { and } \quad E _ {g} = \{\langle s, A \rangle \in \mathbb {P} ^ {\star}: g \in A \}
$$

for $g \in \omega ^ { \omega }$ and $n \ < \ \omega$ . Then ${ \mathcal { D } } = \{ D _ { n } \colon n < \omega \} \cup \{ E _ { g } \colon g \in G \}$ has cardinality $| G | + \omega < { \mathfrak { c } }$ . Since by $( 8 . 7 ) \ \mathbb { P } ^ { \star }$ is ccc, MA implies that there exists a D-generic filter $F$ in $\mathbb { P } ^ { \star }$ . Now we argue as in Lemma 8.1.8. We define $F _ { 0 } = \{ s \colon \langle s , A \rangle \in F \}$ and notice that $f = \bigcup F _ { 0 }$ is a function. Then 

$D _ { n } \cap F \neq \emptyset$ implies that $n \in \operatorname { d o m } ( f )$ , that is, that f maps ω into $\omega .$ . Finally, we notice that $E _ { g } \cap F \neq \emptyset$ implies $g < ^ { \star } ~ f$ 

To prove the theorem from (I) enumerate $\omega ^ { \omega }$ as $\{ g _ { \xi } \colon \xi < \mathfrak { c } \}$ and define the scale $\langle f _ { \xi } \colon \xi < \mathfrak { c } \rangle$ by induction on $\xi < { \mathfrak { c } }$ by choosing $g _ { \xi }$ as a function f from (I) applied to $G = \{ f _ { \zeta } \colon \zeta < \xi \} \cup \{ g _ { \zeta } \colon \zeta < \xi \}$  

Another application of Martin’s axiom is stated in the next theorem. 

Theorem 8.2.3 Assume MA. If $X \in [ \mathbb { R } ] ^ { < \mathfrak { c } }$ then every subset Y of X is a $G _ { \delta }$ subset of X, that is, there exists a $G _ { \delta }$ set $G \subset \mathbb { R }$ such that $G \cap X = Y$ 

Proof Let $X \in [ \mathbb { R } ] ^ { < \mathfrak { c } }$ and fix $Y \subset X$ . We will show that Y is $G _ { \delta }$ in X. 

Let $B = \{ B _ { n } \colon n < \omega \}$ be a countable base for R. First notice that it is enough to find a set $\hat { A } \subset \omega$ such that for every $x \in X$ 

$$
x \in Y \Leftrightarrow x \in B _ {n} \text {   for   infinitely   many   } n \text {   from   } \hat {A}.\tag{8.8}
$$

To see why, define for every $k < \omega$ an open set $G _ { k } = \bigcup \{ B _ { n } \colon n \in \hat { A } \& n > k \}$ and put $\begin{array} { r } { G = \bigcap _ { k < \omega } G _ { k } } \end{array}$ . Then G is a $G _ { \delta }$ set and, by (8.8), for every $x \in X$ we have 

$$
x \in Y \Leftrightarrow x \in G _ {k} \text { for   all } k <   \omega .
$$

Thus $G \cap X = Y$ 

For countable X we could prove (8.8) in the following way. Let $X \backslash Y =$ $\{ z _ { n } \colon n < \omega \}$ and $Y \times \omega = \{ \langle y _ { n } , k _ { n } \rangle \colon n < \omega \}$ . Then construct A<sup>ˆ</sup> as a union of an increasing sequence $\langle A _ { n } \colon n < \omega \rangle$ of finite subsets of $\omega$ such that for every $n < \omega$ there is an $m \in A _ { n }$ such that $m > k _ { n }$ and $y _ { n } \in B _ { m }$ , and such that $z _ { i } \notin B _ { m }$ for all new ms from $A _ { n }$ and all points $z _ { i }$ considered so far, that is, such that 

$$
z _ {i} \notin B _ {m} \text {   for   all   } m \in A _ {n} \setminus A _ {n - 1} \text {   and   } i \leq n.\tag{8.9}
$$

We will transform this idea into a forcing similarly as in Lemma 8.1.8. We define the partially ordered set $\langle \mathbb { P } , \leq \rangle$ by putting $\mathbb { P } = [ \omega ] ^ { < \omega } \times [ X \backslash Y ] ^ { < \omega }$ and define $\leq$ to take care of (8.9). That is, for $\langle A _ { 1 } , C _ { 1 } \rangle , \langle A _ { 0 } , C _ { 0 } \rangle \in \mathbb { P }$ we define $\langle A _ { 1 } , C _ { 1 } \rangle \leq \langle A _ { 0 } , C _ { 0 } \rangle$ provided $A _ { 1 } \supset A _ { 0 } , C _ { 1 } \supset C _ { 0 }$ , and 

$$
c \not \in B _ {m} \text {   for   all   } m \in A _ {1} \setminus A _ {0} \text {   and   } c \in C _ {0}.\tag{8.10}
$$

Now inductive conditions are coded by the following subsets of P: 

$$
D _ {y} ^ {k} = \{\langle A, C \rangle \in \mathbb {P}: \exists m \in A (m \geq k \& y \in B _ {m}) \}
$$

and 

$$
E _ {z} = \{\langle A, C \rangle \in \mathbb {P} \colon z \in C \},
$$

where $y \in Y , k < \omega$ , and $z \in X \setminus Y$ . We will use Martin’s axiom to find a D-generic filter for 

$$
\mathcal {D} = \{D _ {y} ^ {k} \colon y \in Y   \&   k <   \omega \} \cup \{E _ {z} \colon z \in X \setminus Y \}.
$$

To use Martin’s axiom, we have to check whether its assumptions are satisfied. 

Clearly $| \mathcal D | \le | X | + \omega < { \mathfrak c } .$ 

To see that P is ccc consider an uncountable subset $\{ \langle A _ { \xi } , C _ { \xi } \rangle \colon \xi < \omega _ { 1 } \}$ of P. Since $[ \omega ] ^ { < \omega }$ is countable, there are $A \in [ \omega ] ^ { < \omega }$ and $\zeta < \xi < \omega _ { 1 }$ such that $A _ { \zeta } = A _ { \xi } = A$ . Then $\langle A _ { \zeta } , C _ { \zeta } \rangle = \langle A , C _ { \zeta } \rangle$ and $\langle A _ { \xi } , C _ { \xi } \rangle = \langle A , C _ { \xi } \rangle$ are compatible, since $\langle A , C _ { \zeta } \cup C _ { \xi } \rangle \in \mathbb { P }$ extends them both, as condition (8.10) is satisfied vacuously. 

To see that each set $E _ { z }$ is dense in $\mathbb { P }$ take $\langle A , C \rangle \in \mathbb { P }$ and notice that $\langle A , C \cup \{ z \} \rangle \in E _ { z }$ extends $\langle A , C \rangle$ 

Finally, to see that a set $D _ { y } ^ { k }$ is dense in $\mathbb { P } _ { \mathrm { : } }$ , take $\langle A , C \rangle \in \mathbb { P }$ . Notice that there exist infinitely many basic open sets $B _ { m }$ such that 

$$
y \in B _ {m} \text { and } C \cap B _ {m} = \emptyset .\tag{8.11}
$$

Take $m > k$ satisfying (8.11), and notice that $\langle A \cup \{ m \} , C \rangle \in D _ { y } ^ { k }$ extends $\langle A , C \rangle$ 

Now apply Martin’s axiom to find a D-generic filter $F$ in P, and define $\hat { A } = \bigcup \{ A \colon \langle A , C \rangle \in F \}$ . We will show that $\hat { A }$ satisfies (8.8). So let $x \in X$ If $x \in Y$ then for every $k \ < \ \omega$ there exists $\langle A , C \rangle \in F \cap D _ { x } ^ { k }$ In particular, there exists an $m \in A \subset { \hat { A } }$ with $m > k$ such that $x \in B _ { m }$ . So $x \in B _ { m }$ for infinitely many m from $\hat { A }$ 

If $x \in X \backslash Y$ then there exists $\langle A _ { 0 } , C _ { 0 } \rangle \in F \cap E _ { x }$ . In particular, $x \in C _ { 0 }$ It is enough to prove that $x \notin B _ { m }$ for every $m \in \hat { A } \backslash A _ { 0 }$ . So take $m \in \hat { A } \backslash A _ { 0 }$ By the definition of $\hat { A }$ there exists $\langle A , C \rangle \in F$ such that $m \in A$ . But, by the definition of a filter, there exists $\langle A _ { 1 } , C _ { 1 } \rangle \in F$ extending $\langle A , C \rangle$ and $\left. A _ { 0 } , C _ { 0 } \right.$ . Now $\langle A _ { 1 } , C _ { 1 } \rangle \leq \langle A _ { 0 } , C _ { 0 } \rangle , m \in A \subset A _ { 1 } , m \not \in A _ { 0 }$ , and $x \in C _ { 0 }$ Hence, by $( 8 . 1 0 ) , x \notin B _ { m }$  

Corollary 8.2.4 If MA holds then $2 ^ { \omega } ~ = ~ 2 ^ { \kappa }$ for every infinite cardinal $\kappa < { \mathfrak { c } }$ 

Proof Let $\kappa < { \mathfrak { c } }$ be an infinite cardinal number. Then clearly $2 ^ { \omega } \leq 2 ^ { \kappa }$ To see the other inequality take $X \in [ \mathbb { R } ] ^ { \kappa }$ . Then, by Theorem 8.2.3, 

$$
2 ^ {\kappa} = | \mathcal {P} (X) | = | \{B \cap X \colon B \in \mathcal {B} o r \} | \leq | \mathcal {B} o r | = 2 ^ {\omega}.
$$

Corollary 8.2.5 If MA holds then c is a regular cardinal. 

Proof Notice that by Theorem 5.3.8 

$$
2 ^ {\operatorname{cf} (\mathfrak {c})} = (2 ^ {\omega}) ^ {\operatorname{cf} (\mathfrak {c})} = \mathfrak {c} ^ {\operatorname{cf} (\mathfrak {c})} > \mathfrak {c}.
$$

Hence, by Corollary 8.2.4, cf $\mathbf { \Psi } ( \mathfrak { c } ) \geq \mathfrak { c }$ 

The next theorem tells us that MA implies the continuum additivity of category, which has been mentioned in the remark after Theorem 7.2.5. In particular, it implies that Theorem 7.2.5 can be proved when CH is replaced with MA. 

Theorem 8.2.6 If MA holds then a union of less than continuum many meager subsets of $\mathbb { R } ^ { n }$ is meager in $\mathbb { R } ^ { n }$ , that $i s ,$ 

$$
\bigcup \mathcal {F} \in \mathcal {M} \text {   for   every   } \mathcal {F} \in [ \mathcal {M} ] ^ {<   \mathfrak {c}}.
$$

Proof The idea of the proof is very similar to that of Theorem 8.2.3. 

Let $\mathcal { F } \in [ M ] ^ { < \mathfrak { c } }$ . Since every $F$ from $\mathcal { F }$ is a countable union of nowheredense sets, $\cup \mathcal { F }$ is a union of $| \mathcal { F } | + \omega < { \mathfrak { c } }$ nowhere-dense sets. Thus we may assume that every set in $\mathcal { F }$ is nowhere dense. 

Let $\mathcal { B } = \{ B _ { j } \neq \emptyset : j < \omega \}$ be a countable base for $\mathbb { R } ^ { n }$ . Notice that it is enough to find a set $\hat { A } \subset \omega$ such that 

$$
\{m \in \hat {A} \colon B _ {m} \cap F \neq \emptyset \} \text {   is   finite   for   every   } F \in \mathcal {F}\tag{8.12}
$$

and 

$$
\{m \in \hat {A} \colon B _ {m} \subset B _ {j} \} \text {   is   infinite   for   every   } j <   \omega .\tag{8.13}
$$

To see why, define $U _ { k } = \bigcup \{ B _ { m } \colon m \in \hat { A } \ \& \ m > k \}$ for every $k < \omega$ Notice that by (8.13) the sets $U _ { k }$ are dense and open. Therefore the sets $\mathbb { R } ^ { n } \setminus U _ { k }$ are nowhere dense. But condition (8.12) implies that $\cup \mathcal { F } \subset$ $\textstyle \bigcup _ { k < \omega } ( \mathbb { R } ^ { n } \setminus U _ { k } ) \in { \mathcal { M } }$ , since for every $F \in { \mathcal { F } }$ there exists a $k < \omega$ such that 

$$
U _ {k} \cap F = \bigcup \left\{B _ {m} \cap F: m \in \hat {A} \& m > k \right\} = \emptyset .
$$

To prove the existence of such a set $\hat { A }$ consider the partial order $\mathbb { P } =$ $[ \omega ] ^ { < \omega } \times [ \mathcal { F } ] ^ { < \omega }$ , where we put $\langle A _ { 1 } , \mathcal { C } _ { 1 } \rangle ~ \leq ~ \langle A _ { 0 } , \mathcal { C } _ { 0 } \rangle$ provided $A _ { 1 } ~ \supset ~ A _ { 0 }$ $\mathcal { C } _ { 1 } \supset \mathcal { C } _ { 0 }$ , and 

$$
B _ {m} \cap F = \emptyset \text {   for   all   } m \in A _ {1} \setminus A _ {0} \text {   and   } F \in \mathcal {C} _ {0}.\tag{8.14}
$$

We will define $\hat { A }$ as the union of all A such that $\langle A , C \rangle$ belongs to an appropriate generic filter in $\mathbb { P } .$ . In particular, in the condition $\langle A , { \mathcal { C } } \rangle \in \mathbb { P }$ the set $A$ approximates ${ \hat { A } } .$ . The sets $F$ from C represent “elements of $\mathcal { F }$ looked at so $\mathrm { f a r } ^ { \prime \prime }$ in our “induction” and (8.14) guarantees that the basic open sets indexed by “new elements of ${ \hat { A } } ^ { \dag }$ will not intersect these “old” $F \mathrm { s }$ . This will take care of (8.12). 

The forcing $\mathbb { P }$ is ccc since $[ \omega ] ^ { < \omega }$ is countable and any conditions $\langle A , \mathcal { C } _ { 0 } \rangle$ and $\langle A , \mathcal { C } _ { 1 } \rangle$ are compatible, having $\langle A , C _ { 0 } \cup C _ { 1 } \rangle$ as a common extension. 

Conditions (8.13) and (8.12) are related to the following dense subsets of P: 

$$
D _ {j} ^ {k} = \{\langle A, \mathcal {C} \rangle \in \mathbb {P}: \exists m \in A (m \geq k \& B _ {m} \subset B _ {j}) \}
$$

and 

$$
E _ {F} = \{\langle A, \mathcal {C} \rangle \in \mathbb {P} \colon F \in \mathcal {C} \},
$$

where $k , j < \omega$ and $F \in { \mathcal { F } }$ . The sets $E _ { F }$ are dense, since $\langle A , { \mathcal { C } } \cup \{ F \} \rangle \in E _ { F }$ extends $\langle A , { \mathcal { C } } \rangle$ for every $\langle A , { \mathcal { C } } \rangle \in \mathbb { P }$ . To see that the sets $D _ { j } ^ { k }$ are dense take $\langle A , { \mathcal { C } } \rangle \in \mathbb { P }$ . Since $\cup { \mathcal { C } }$ is nowhere dense, there exist infinitely many basic open sets $B _ { m }$ such that 

$$
B _ {m} \subset B _ {j} \setminus \bigcup \mathcal {C}.\tag{8.15}
$$

Take $m > k$ satisfying (8.15) and notice that $\langle A \cup \{ m \} , { \mathcal { C } } \rangle \in D _ { j } ^ { k }$ extends $\langle A , { \mathcal { C } } \rangle$ 

Hence, by Martin’s axiom, there exists a D-generic filter $\hat { F }$ in $\mathbb { P } ,$ , where 

$$
\mathcal {D} = \left\{D _ {j} ^ {k}: k, j <   \omega \right\} \cup \left\{E _ {F}: F \in \mathcal {F} \right\}.
$$

Define $\hat { A } = \bigcup \{ A \colon \langle A , \mathcal { C } \rangle \in \hat { F } \}$ . It is enough to show that $\hat { A }$ satisfies properties (8.13) and (8.12). 

To see (8.13) take $j < \omega$ . It is enough to prove that for every $k < \omega$ there exists an $m \in { \hat { A } }$ with $m > k$ and $B _ { m } \subset B _ { j }$ . So fix $k < \omega$ and pick $\langle A , \mathcal { C } \rangle \in \hat { F } \cap D _ { j } ^ { k }$ . Then, by the definition of $D _ { j } ^ { k }$ , there exists an $m \in A \subset { \hat { A } }$ with $m > k$ such that $B _ { m } \subset B _ { j }$ 

To see (8.12) take $F \in { \mathcal { F } }$ . Then there exists $\langle A _ { 0 } , { \mathcal { C } } _ { 0 } \rangle \in { \hat { F } } \cap E _ { F }$ . In particular, $F \in { \mathcal { C } } _ { 0 }$ . It is enough to prove that $B _ { m } \cap F = \emptyset$ for every $m \in \hat { A } \setminus A _ { 0 }$ . Take $m \in \hat { A } \setminus A _ { 0 }$ . By the definition of $\hat { A }$ there exists $\langle A , { \mathcal { C } } \rangle \in { \hat { F } }$ such that $m \in A$ . So there exists $\langle A _ { 1 } , \mathcal { C } _ { 1 } \rangle \in \hat { F }$ extending $\langle A , { \mathcal { C } } \rangle$ and $\langle A _ { 0 } , \mathcal { C } _ { 0 } \rangle$ . Now $\langle A _ { 1 } , \mathcal { C } _ { 1 } \rangle \leq \langle A _ { 0 } , \mathcal { C } _ { 0 } \rangle , m \in A \subset A _ { 1 } ,$ m $\not \in A _ { 0 }$ , and $F \in { \mathcal { C } } _ { 0 }$ Hence, by (8.14), $B _ { m } \cap F = \varnothing$  

An analog of Theorem 8.2.6 for the ideal $\mathcal { N }$ of measure-zero subsets of $\mathbb { R } ^ { n }$ is also true. 

Theorem 8.2.7 If MA holds then a union of less than continuum many null subsets of $\mathbb { R } ^ { n }$ is null in $\mathbb { R } ^ { n }$ , that is, 

$$
\bigcup \mathcal {F} \in \mathcal {N} \text {   for   every   } \mathcal {F} \in [ \mathcal {N} ] ^ {<   \mathfrak {c}}.
$$

Proof To make the argument simpler, we will prove the theorem only for R. The proof of the general case is essentially the same. 

Let $B _ { 0 }$ be the family of all open intervals in R and let $l ( I )$ stand for the length of $I \in B _ { 0 }$ . Recall that $S \in \mathcal N$ if for every $\varepsilon > 0$ there exists a sequence $\langle I _ { k } \in B _ { 0 } \colon k < \omega \rangle$ such that $\textstyle S \subset \bigcup _ { k < \omega } I _ { k }$ and $\begin{array} { r } { \sum _ { k < \omega } l ( I _ { k } ) < \varepsilon } \end{array}$ 

Now, if $B = \{ I _ { n } \colon n < \omega \}$ is the family of all intervals with rational endpoints, then the family $B _ { 0 }$ can be replaced by B. To see it, take $S \in \mathcal N$ and let $\varepsilon \ > \ 0$ Then there exists a sequence $\langle J _ { k } \ \in \ B _ { 0 } \colon k \ < \ \omega \rangle$ such that $\textstyle S \subset \bigcup _ { k < \omega } J _ { k }$ and $\begin{array} { r } { \sum _ { k < \omega } l ( J _ { k } ) < \varepsilon / 2 } \end{array}$ . But for every $k \ < \ \omega$ there exists an $I _ { k } ~ \in ~ { \cal B } _ { 0 }$ such that $J _ { k } \subset I _ { k }$ and $l ( I _ { k } ) < l ( J _ { k } ) + \varepsilon / 2 ^ { k + 2 }$ . So $\begin{array} { r } { S \subset \bigcup _ { k < \omega } J _ { k } \subset \bigcup _ { k < \omega } I _ { k } } \end{array}$ and $\begin{array} { r } { \sum _ { k < \omega } l ( I _ { k } ) \le \sum _ { k < \omega } [ l ( J _ { k } ) + \varepsilon / 2 ^ { k + 2 } ] < \varepsilon } \end{array}$ 

<sub>Let</sub> $\mathcal { F } \in [ \mathcal { N } ] ^ { < \mathfrak { c } }$ and fix $\varepsilon > 0$ . We will find an $\hat { A } \subset \omega$ such that 

$$
\bigcup \mathcal {F} \subset \bigcup_ {n \in \hat {A}} I _ {n} \quad \text { and } \quad \sum_ {n \in \hat {A}} l (I _ {n}) \leq \varepsilon .\tag{8.16}
$$

Define $\mathbb { P } = \{ A \subset \omega \colon \sum _ { n \in A } l ( I _ { n } ) < \varepsilon \}$ and order it by reverse inclusion: $A _ { 1 } \leq A _ { 0 } \Leftrightarrow A _ { 1 } \supset A _ { 0 }$ . To see that $\mathbb { P }$ is ccc let ${ \mathcal { A } } \subset \mathbb { P }$ be uncountable. We have to find diferent $A , A ^ { \prime } \in { \mathcal { A } }$ that are compatible, that is, such that $\textstyle \sum _ { n \in A \cup A ^ { \prime } } l ( I _ { n } ) < \varepsilon$ 

So for every $A \in { \mathcal { A } }$ let $m _ { A } < \omega$ be such that $\textstyle \sum _ { n \in A } l ( I _ { n } ) + 1 / m _ { A } < \varepsilon .$ Since $\mathcal { A }$ is uncountable, there exists an uncountable subset $\mathcal { A } ^ { \prime }$ of $\mathcal { A }$ and an $m < \omega$ such that $m _ { A } = m$ for every $A \in { \mathcal { A } } ^ { \prime }$ , that is, 

$$
\sum_ {n \in A} l (I _ {n}) + \frac {1}{m} <   \varepsilon \text { for   every } A \in \mathcal {A} ^ {\prime}.\tag{8.17}
$$

Next, for every $A \in { \mathcal { A } } ^ { \prime }$ choose $k _ { A } < \omega$ such that $\smash { \sum _ { n \in \boldsymbol { A } \backslash k _ { A } } l ( I _ { n } ) < 1 / m }$ Since $\mathcal { A } ^ { \prime }$ is uncountable, there exists an uncountable subset $\mathcal { A } ^ { \prime \prime }$ of $\mathcal { A } ^ { \prime }$ and a $k < \omega$ such that $k _ { A } = k$ for every $A \in { \mathcal { A } } ^ { \prime \prime }$ , that is, 

$$
\sum_ {n \in A \backslash k} l (I _ {n}) <   \frac {1}{m} \text {   for   every   } A \in \mathcal {A} ^ {\prime \prime}.\tag{8.18}
$$

Now we can find two diferent $A , A ^ { \prime } \in { \mathcal { A } } ^ { \prime \prime }$ such that $A \cap k = A ^ { \prime } \cap k$ . For such A and $A ^ { \prime }$ we have, in particular, $A \cup A ^ { \prime } = A \cup ( A ^ { \prime } \setminus k )$ . So, by (8.18) and (8.17), 

$$
\sum_ {n \in A \cup A ^ {\prime}} l (I _ {n}) \leq \sum_ {n \in A} l (I _ {n}) + \sum_ {n \in A ^ {\prime} \backslash k} l (I _ {n}) <   \sum_ {n \in A} l (I _ {n}) + \frac {1}{m} <   \varepsilon .
$$

Thus A and $A ^ { \prime }$ are compatible and $\mathbb { P }$ is ccc. 

Now for every $F \in { \mathcal { F } }$ let $\begin{array} { r } { D _ { F } = \{ A \in \mathbb { P } \colon F \subset \bigcup _ { n \in A } I _ { n } \} } \end{array}$ . Notice that every $D _ { F }$ is dense in P. To see this, let $A \in \mathbb { P }$ and put $\begin{array} { r } { \delta \bar { \mathbf { \alpha } } = \varepsilon - \sum _ { n \in A } l ( I _ { n } ) > } \end{array}$ 

0. Since $F \in \mathcal { N }$ we can find a $B \subset \omega$ such that $F \subset \bigcup _ { n \in B } I _ { n }$ and $\textstyle \sum _ { n \in B } l ( I _ { n } ) < \delta$ . But then $A \cup B \in D _ { F }$ since 

$$
\sum_ {n \in A \cup B} l (I _ {n}) \leq \sum_ {n \in A} l (I _ {n}) + \sum_ {n \in B} l (I _ {n}) <   \sum_ {n \in A} l (I _ {n}) + \delta = \varepsilon
$$

and $F \subset \textstyle \bigcup _ { n \in A \cup B } I _ { n }$ . Since $A \cup B \leq A$ , the set $D _ { F }$ is dense. 

Let $\mathcal { D } = \{ D _ { F } \colon F \in \mathcal { F } \}$ . Since P is ccc and $| \mathcal { D } | \leq | \mathcal { F } | < { \mathfrak { c } }$ , by Martin’s axiom there exists a D-generic filter $\hat { F }$ in P. Let ${ \hat { A } } = \cup { \hat { F } }$ . We will show that $\hat { A }$ satisfies (8.16). 

For every $F \in { \mathcal { F } }$ there exists an $A \in \hat { F } \cap D _ { F }$ . So $F \subset \bigcup _ { n \in A } I _ { n } \subset$ $\textstyle { \bigcup _ { n \in { \hat { A } } } I _ { n } }$ since $A \subset { \hat { A } }$ . Then $\cup \mathcal { F } \subset \bigcup _ { n \in \hat { A } } I _ { n }$ 

To see $\textstyle \sum _ { n \in { \hat { A } } } l ( I _ { n } ) \leq \varepsilon { \mathrm { ~ i t ~ } }$  is enough to show that $\textstyle \sum _ { n \in { \hat { A } } \cap k } l ( I _ { n } ) < \varepsilon$ for every $k < \omega$ . So fix $k < \omega$ . Now for every $n \in { \hat { A } } \cap k$ there exists an $A _ { n } \in { \hat { F } }$ such that $n \in A _ { n }$ . Using condition $( \mathrm { F } 1 ^ { \prime } )$ of the definition of a filter we can find an $A \in { \hat { F } }$ such that $A \leq A _ { n }$ for every $n \in { \hat { A } } \cap k$ . But then ${ \hat { A } } \cap k \subset A$ and 

$$
\sum_ {n \in \hat {A} \cap k} l (I _ {n}) \leq \sum_ {n \in A} l (I _ {n}) <   \varepsilon .
$$

This finishes the proof. 

All previous applications of Martin’s axiom could be deduced as well from the continuum hypothesis, but in the remaining part of this section we will show that this will not always be the case, by discussing the consequences of $\mathrm { M A } { + } { \lnot \mathrm { C H } }$ , which do not follow from CH. Similar results can also be found in the next section. 

In the next theorem we will use the following terminology. A subset A of a partially ordered set $\langle \mathbb { P } , \leq \rangle$ is compatible if for every finite subset $A _ { 0 }$ of A there exists a $p \in \mathbb { P }$ such that $p \leq q$ for all $q \in A _ { 0 }$ (compare this with condition (F1<sup>-</sup>) from the definition of a filter). 

Theorem 8.2.8 Assume $M A { \mathrel { + } } { \mathrel { \neg } } C H$ and let $\langle \mathbb { P } , \leq \rangle$ be a ccc partially ordered set. If $A \subset \mathbb { P }$ is uncountable, then there exists an uncountable compatible subset A<sup>ˆ</sup> of A. 

Proof Let $A \subset \mathbb { P }$ be uncountable. Without loss of generality we may assume that $| A | = \omega _ { 1 }$ 

The inductive approach to the proof is to construct a strictly increasing sequence $\langle A _ { \xi } \colon \xi \ < \ \omega _ { 1 } \rangle$ of compatible subsets of A such that $\cup _ { \xi < \omega } A _ { \xi }$ is an uncountable compatible subset of A. Although this idea is basically correct, it has a fundamental flaw. If you start with $A _ { 0 } \in [ A ] ^ { \leq \omega }$ such that $A _ { 0 }$ is compatible with at most countably many elements of A, then this construction must fail. Fortunately, there are only countably many sets 

$A _ { 0 } \in [ A ] ^ { \leq \omega }$ that may cause such a problem, and after removing them from $A$ we will be able to follow the idea just described. 

So for $p \in \mathbb { P }$ let $A _ { p } = \{ q \in A \colon q$ is compatible with $p \}$ . We will show that the set 

$$
A ^ {\prime} = \{q \in A \colon \exists p \leq q (| A _ {p} | \leq \omega) \} \quad \text { is   at   most   countable. }\tag{8.19}
$$

Indeed, consider the family ${ \mathcal { F } } ~ = ~ \{ C ~ \subset ~ B \colon C$ is an antichain in $\mathbb { P } \}$ where $B ~ = ~ \{ p \in \mathbb { P } \colon | A _ { p } | \leq \omega \}$ . It is easy to see that $\mathcal { F }$ satisfies the assumptions of the Hausdorf maximal principle. Thus we can choose a maximal element $C _ { 0 }$ of $\mathcal { F }$ . Now $C _ { 0 }$ is clearly an antichain in $\mathbb { P } .$ . So $C _ { 0 }$ is at most countable, since $\mathbb { P }$ is ccc. It is enough to prove that 

$$
A ^ {\prime} \subset \bigcup_ {r \in C _ {0}} A _ {r},
$$

since the set $\textstyle \bigcup _ { r \in C _ { 0 } } A _ { r }$ is countable, being a countable union of countable sets. To see the inclusion, take $q \in A ^ { \prime }$ . Then there exists a $p \leq q$ such that $p \in B$ . By the maximality of $C _ { 0 }$ there exists an $r \in C _ { 0 }$ such that $r$ is compatible with $p _ { : }$ , that is, $s \leq r$ and $s \leq p \leq q$ for some $s \in \mathbb { P }$ . In particular, $r$ and $q$ are compatible, so $q \in A _ { r }$ . Condition (8.19) has been proved. 

Now the set $A ^ { \star } = A \setminus A ^ { \prime }$ is uncountable. Moreover, if $p \leq q$ for some $q \in A ^ { \star }$ then $A _ { p }$ must be uncountable. In particular, 

$$
A _ {p} ^ {\star} = \left\{q \in A ^ {\star}: q \text {   is   compatible   with   } p \right\} \text {   is   uncountable }\tag{8.20}
$$

for every $p \in \mathbb { P }$ such that $p \leq q$ for some $q \in A ^ { \star }$ 

Coming back to the idea of an inductive proof, we can see that we could have a hard time extending an infinite set $A _ { \xi }$ to a compatible set $A _ { \xi + 1 }$ properly containing $A _ { \xi }$ . This problem will be solved with the help of MA. 

For this, consider a partially ordered set 

$$
\mathbb {P} ^ {\star} = \{F \in [ A ^ {\star} ] ^ {<   \omega}: F \text {   is   compatible   in   } \mathbb {P} \}
$$

ordered by reverse inclusion ⊃. Notice that the forcing $\mathbb { P } ^ { \star }$ is ccc. To see why, let $\{ F _ { \xi } \in \mathbb { P } ^ { \star } \colon \xi < \omega _ { 1 } \}$ . We will find $\zeta < \xi < \omega _ { 1 }$ such that $F _ { \zeta }$ and $F _ { \xi }$ are compatible, that is, that $F _ { \zeta } \cup F _ { \xi } \in \mathbb { P } ^ { \star }$ . But for every $\xi < \omega _ { 1 }$ there exists a $p _ { \xi } \in \mathbb { P }$ with $p _ { \xi } \le p$ for every $p \in F _ { \xi }$ . Moreover, the set $\{ p _ { \xi } \colon \xi < \omega _ { 1 } \}$ cannot be an antichain, since $\mathbb { P }$ is ccc. Thus there are compatible $p _ { \zeta }$ and $p _ { \xi }$ for some $\zeta < \xi < \omega _ { 1 }$ . Now, if $q \in \mathbb { P }$ is such that $q \leq p _ { \zeta }$ and $q \leq p _ { \xi }$ then $q \leq p$ for every $p \in F _ { \zeta } \cup F _ { \xi }$ . Therefore $F _ { \zeta } \cup F _ { \xi } \in \mathbb { P } ^ { \star }$ and $\mathbb { P } ^ { \star }$ is ccc. 

Let $\langle q _ { \xi } \colon \xi < \omega _ { 1 } \rangle$ be a one-to-one enumeration of $A ^ { \star }$ . For $\alpha < \omega _ { 1 }$ define 

$$
D _ {\alpha} = \left\{F \in \mathbb {P} ^ {\star}: \exists \xi > \alpha (q _ {\xi} \in F) \right\}
$$

and notice that the sets $D _ { \alpha }$ are dense in $\mathbb { P } ^ { \star }$ . This is so since for every $F \in \mathbb { P } ^ { \star }$ there exists a $p \in \mathbb { P }$ such that $p \leq q$ for every $q \in F$ , and, by (8.20), $p$ is compatible with uncountably many $q _ { \xi }$ . In particular, there exists a $\xi > \alpha$ such that $q _ { \xi }$ is compatible with $p _ { : }$ , and it is easy to see that $F \cup \{ q _ { \xi } \} \in D _ { \alpha }$ extends $F$ . 

Let $\mathcal { D } = \{ D _ { \alpha } \colon \alpha < \omega _ { 1 } \}$ . Then $| \mathcal { D } | \leq \omega _ { 1 } < \mathfrak { c } \ \mathrm { s o } .$ , by MA, there exists a D-generic filter $\hat { F } \mathrm { i n } \mathbb { P } ^ { \star }$ . We will show that ${ \hat { A } } = \cup { \hat { F } }$ is an uncountable compatible subset of $A$ 

Clearly, ${ \hat { A } } \subset A$ . To see that $\hat { A }$ is uncountable, notice that for every $\alpha < \omega _ { 1 }$ there exists a $\xi > \alpha$ such that $q _ { \xi } \in { \hat { A } }$ , since $\hat { F } \cap D _ { \alpha } \neq \varnothing$ . To finish the proof, it is enough to show that $\hat { A }$ is compatible. 

So let $F = \{ r _ { 0 } , \ldots , r _ { n } \} \subset { \hat { A } }$ . For every $i \leq n$ there exists an $F _ { i } \in { \hat { F } }$ such that $r _ { i } \in F _ { i \cdot } \ \mathrm { B y } \ ( \mathrm { F 1 ^ { \prime } } )$ we can find an $E \in { \hat { F } }$ such that $E \leq F _ { i }$ for all $i \leq n$ . In particular, $E \supset \{ r _ { 0 } , \ldots , r _ { n } \} = F$ , that is, $F$ is compatible. 

By definition, a forcing $\mathbb { P }$ is ccc if every uncountable set $\{ p _ { \alpha } \colon \alpha \in A \}$ contains two diferent compatible elements. Equivalently, $\mathbb { P }$ is ccc if for every sequence $\langle p _ { \alpha } \colon \alpha \in A \rangle$ (not necessarily one-to-one) with uncountable index set A there are diferent indices $\alpha , \beta \in A$ such that $p _ { \alpha }$ and $p _ { \beta }$ are compatible. In this language Theorem 8.2.8 can be restated as follows. 

Corollary 8.2.9 Assume $M A { \mathrel { + } } { \mathrel { \neg } } C H$ and let $\langle \mathbb { P } , \leq \rangle$ be a ccc partially ordered set. If $\langle p _ { \alpha } \colon \alpha \ \in \ A \rangle$ is an uncountable sequence of elements of $\mathbb { P }$ then there exists an uncountable subset $\hat { A }$ of A such that $\{ p _ { \alpha } \colon \alpha \in { \hat { A } } \}$ is compatible in P. 

To state the next corollary, we need the following important definition. Let $\langle \mathbb { P } _ { 0 } , \leq _ { 0 } \rangle$ and $\langle \mathbb { P } _ { 1 } , \leq _ { 1 } \rangle$ be partially ordered sets. Their product $\langle \mathbb { P } , \leq \rangle$ is defined by $\mathbb { P } = \mathbb { P } _ { 0 } \times \mathbb { P } _ { 1 }$ and 

$$
\left\langle p _ {0}, p _ {1} \right\rangle \leq \left\langle q _ {0}, q _ {1} \right\rangle \Leftrightarrow p _ {0} \leq_ {0} q _ {0} \& p _ {1} \leq_ {1} q _ {1}.
$$

Corollary 8.2.10 If $M A { \mathrel { + } } { \mathrel { \neg } } C H$ holds then the product of two ccc forcings is ccc. 

Proof Let $\langle \mathbb { P } , \leq \rangle$ be a product of ccc forcings $\langle \mathbb { P } _ { 0 } , \leq _ { 0 } \rangle$ and $\langle \mathbb { P } _ { 1 } , \leq _ { 1 } \rangle$ and let $\langle \langle p _ { \alpha } , q _ { \alpha } \rangle \colon \alpha \in A \rangle$ be an uncountable sequence of elements of P. By Corollary 8.2.9 used for the forcing $\mathbb { P } _ { 0 }$ and a sequence $\langle p _ { \alpha } \colon \alpha \in A \rangle$ , we can find an uncountable subset $\hat { A }$ of $A$ such that the set $\{ p _ { \alpha } \colon \alpha \in { \hat { A } } \}$ is compatible in $\mathbb { P } _ { 0 }$ . Then there are diferent $\alpha , \beta \in { \hat { A } }$ such that $q _ { \alpha }$ and $q _ { \beta }$ are compatible in $\mathbb { P } _ { 1 }$ , since $\mathbb { P } _ { 1 }$ is ccc. It is easy to see that $\langle p _ { \alpha } , q _ { \alpha } \rangle$ and $\langle p _ { \beta } , q _ { \beta } \rangle$ are compatible in $\mathbb { P } .$ .  

The last theorem of this section shows that Corollary 8.2.10 is false under CH. In its proof we will use the following lemma, which is the main combinatorial tool needed to prove that diferent kinds of forcing (built with finite sets) are ccc. 

Lemma 8.2.11 (∆-system lemma) If A is an uncountable family of finite sets then there exists an uncountable subfamily A of A and a finite set A such that $X \cap Y = A$ for every distinct $X , Y \in \mathcal { A } _ { 0 }$ 

Proof Since $| { \mathcal { A } } | > \omega$ we may assume that there is an $n < \omega$ such that each element of A has exactly n elements. The proof is by induction on n. 

By our assumption we must have $n > 0 .$ . (Otherwise ${ \mathcal { A } } \subset \{ \emptyset \}$ has cardinality $\leq 1 < \omega . )$ If $n = 1$ then elements of A must be pairwise disjoint and the theorem holds with $A = \emptyset$ and $\mathcal { A } _ { 0 } = \mathcal { A }$ . So assume that $n > 1$ and that the theorem holds for $( n - 1 )$ -element sets. Consider two cases. 

Case 1: There exists an $A _ { 0 } \in { \mathcal { A } }$ such that $A _ { 0 }$ intersects uncountably many $A \in { \mathcal { A } }$ . Then there exists an $a \in A _ { 0 }$ such that a belongs to uncountably many $A \in { \mathcal { A } }$ . In particular, 

$$
\mathcal {B} = \{A \setminus \{a \}: A \in \mathcal {A} \& a \in A \}
$$

is an uncountable family of sets of size $n - 1$ , and by the inductive hypothe sis, we can find an uncountable $B _ { 0 } \subset B$ and a finite set B such that $C \cap D =$ B for every distinct $C , D \in B _ { 0 }$ . But then $\mathcal { A } _ { 0 } = \{ C \cup \{ a \} : C \in B _ { 0 } \} \subset \mathcal { A }$ is uncountable and $X \cap Y = B \cup \{ a \}$ for every distinct $X , Y \in \mathcal { A } _ { 0 }$ 

Case 2: For every $A \in { \mathcal { A } }$ the set 

$$
S _ {A} = \{B \in \mathcal {A} \colon A \cap B \neq \emptyset \}
$$

is at most countable. Construct, by transfinite induction, a one-to-one sequence $\langle A _ { \xi } \colon \xi < \omega _ { 1 } \rangle$ of pairwise-disjoint subsets of A. This can be done since for every $\xi < \omega _ { 1 }$ the set 

$$
\{B \in \mathcal {A} \colon B \cap A _ {\zeta} \neq \emptyset \text {for some} \zeta <   \xi \} = \bigcup_ {\zeta <   \xi} S _ {A _ {\zeta}}
$$

is at most countable. Then $A _ { 0 } = \{ A _ { \xi } \colon \xi < \omega _ { 1 } \}$ and $A = \emptyset$ satisfy the desired requirements.  

In the next theorem, due to Galvin (1980), for sets A and B we will use the notation 

$$
A \otimes B = \{\{a, b \}: a \in A \& b \in B \}.
$$

Theorem 8.2.12 If CH holds then there are two ccc forcings such that their product is not ccc. 

Proof The forcings will be constructed as follows. We will construct a coloring function $f \colon [ \omega _ { 1 } ] ^ { 2 }  2$ . Then, for $i < 2$ , we put $K _ { i } = f ^ { - 1 } ( i )$ and define 

$$
\mathbb {P} _ {i} = \{F \in [ \omega_ {1} ] ^ {<   \omega}: [ F ] ^ {2} \subset K _ {i} \}
$$

ordered by reverse inclusion $\supset$ . 

First we notice that the forcing $\mathbb { P } _ { 0 } \times \mathbb { P } _ { 1 }$ is not ccc, since the family $\{ \langle \{ \xi \} , \{ \xi \} \rangle \in \mathbb { P } _ { 0 } \times \mathbb { P } _ { 1 } \colon \xi < \omega _ { 1 } \}$ forms an antichain. This is the case because compatibility of $\langle \{ \zeta \} , \{ \zeta \} \rangle$ and $\langle \{ \xi \} , \{ \xi \} \rangle$ implies $\langle \{ \zeta , \xi \} , \{ \zeta , \xi \} \rangle \in \mathbb { P } _ { 0 } \times \mathbb { P } _ { 1 }$ and this is impossible since $\mathbb { P } _ { 0 } \cap \mathbb { P } _ { 1 } = [ \omega _ { 1 } ] ^ { \leq 1 }$ is disjoint from $[ \omega _ { 1 } ] ^ { 2 }$ 

Thus it is enough to construct an $f$ such that the forcings $\mathbb { P } _ { i }$ are ccc. We will first translate the ccc property of $\mathbb { P } _ { i }$ into a condition that will be appropriate for the inductive construction of $f .$ . 

So fix $i < 2$ and let $\langle F _ { \xi } \in \mathbb { P } _ { i } \colon \xi < \omega _ { 1 } \rangle$ . To prove that $\mathbb { P } _ { i }$ is ccc we will have to find $\zeta < \xi < \omega _ { 1 }$ such that $F _ { \zeta }$ and $F _ { \xi }$ are compatible, that is, that 

$$
[ F _ {\zeta} \cup F _ {\xi} ] ^ {2} \subset K _ {i}.
$$

First notice that by the $\Delta { \mathrm { - s y s t e m } }$ lemma we can assume, choosing a subsequence, if necessary, that for some $F \in [ \omega _ { 1 } ] ^ { < \omega }$ 

$$
F _ {\zeta} \cap F _ {\xi} = F \quad \text { for   all } \zeta <   \xi <   \omega_ {1}.
$$

But $[ F _ { \zeta } \cup F _ { \xi } ] ^ { 2 } = [ F _ { \zeta } ] ^ { 2 } \cup [ F _ { \xi } ] ^ { 2 } \cup ( F _ { \zeta } \setminus F ) \otimes ( F _ { \xi } \setminus F )$ and $[ F _ { \zeta } ] ^ { 2 } \cup [ F _ { \xi } ] ^ { 2 } \subset K _ { i }$ Thus we must find $\zeta < \xi < \omega _ { 1 }$ such that 

$$
(F _ {\zeta} \setminus F) \otimes (F _ {\xi} \setminus F) \subset K _ {i}.
$$

Replacing $F _ { \xi }$ with $F _ { \xi } \setminus F ,$ , we notice that it is enough to prove that for every sequence $\langle F _ { \xi } \in \mathbb { P } _ { i } \colon \xi < \omega _ { 1 } \rangle$ of pairwise-disjoint nonempty sets there are $\zeta < \xi < \omega _ { 1 }$ such that 

$$
F _ {\zeta} \otimes F _ {\xi} \subset K _ {i}.
$$

Moreover, for every $\alpha < \omega _ { 1 }$ such that $\textstyle \bigcup _ { n < \omega } F _ { n } \subset \alpha$ there exists a $\xi < \omega _ { 1 }$ with $F = F _ { \xi } \subset \omega _ { 1 } \setminus \alpha$ . Thus we can reduce our task by showing that for every sequence $\langle F _ { n } \in \mathbb { P } _ { i } \colon n < \omega \rangle$ of pairwise-disjoint nonempty sets there exists an $\alpha < \omega _ { 1 }$ with $\textstyle \bigcup _ { n < \omega } F _ { n } \subset$ α such that for every $F \in [ \omega _ { 1 } \backslash \alpha ] ^ { < \omega }$ 

$$
\exists n <   \omega (F _ {n} \otimes F \subset K _ {i}),
$$

that is, that 

$$
\exists n <   \omega   \forall \beta \in F _ {n}   \forall \gamma \in F   (f (\{\beta , \gamma \}) = i).\tag{8.21}
$$

Now, by induction on $\xi < \omega _ { 1 }$ , we will construct an increasing sequence of partial functions $f \colon [ \xi ] ^ { 2 } \to 2$ such that the entire function $f \colon [ \omega _ { 1 } ] ^ { 2 }  2$ will satisfy condition $( 8 . 2 1 ) . ^ { 2 }$ For this, let $\langle \langle F _ { n } ^ { \xi } \rangle _ { n < \omega } : \xi < \omega _ { 1 } \rangle$ be an enumeration of all sequences $\langle F _ { n } \rangle _ { n < \omega }$ of pairwise-disjoint nonempty finite subsets of $\omega _ { 1 }$ such that each sequence appears in the list $\omega _ { 1 }$ times. Such an enumeration can be chosen by CH, since the family of all such sequences has cardinality $\leq \left| \left( [ \omega _ { 1 } ] ^ { < \omega } \right) ^ { \omega } \right| = { \mathfrak { c } }$ . The construction will be done while maintaining the  following inductive condition for every $\xi < \omega _ { 1 }$ 

$\left( { { I _ { \xi } } } \right)$ For every $i < 2 , \alpha < \xi ,$ and $F \in [ \xi \setminus \alpha ] ^ { < \omega } , { \mathrm { i f } } \bigcup _ { n < \omega } F _ { n } ^ { \alpha } \subset \alpha$ then the set 

$$
\mathcal {E} (i, \alpha , F) = \left\{F _ {n} ^ {\alpha}: \forall \beta \in F _ {n} ^ {\alpha} \forall \gamma \in F (f (\{\beta , \gamma \}) = i) \right\}\tag{8.22}
$$

is infinite. 

Notice that this will finish the proof, since then f will satisfy (8.21) for every $i < 2$ and every sequence $\langle F _ { n } \rangle _ { n < \omega }$ of pairwise-disjoint nonempty finite subsets of $\omega _ { 1 }$ . To see this, choose $\alpha < \omega _ { 1 }$ such that $\textstyle \bigcup _ { n < \omega } F _ { n } \subset \alpha$ and $\langle F _ { n } ^ { \alpha } \rangle _ { n < \omega } = \langle F _ { n } \rangle _ { n < \omega }$ , and for every $F \in [ \omega _ { 1 } \setminus \alpha ] ^ { < \omega }$ find a $\xi ~ < ~ \omega _ { 1 }$ such that $F \in [ \xi \setminus \alpha ] ^ { < \omega }$ . Then, by $\left( { { I _ { \xi } } } \right)$ , there exists an $n < \omega$ such that $F _ { n } ^ { \alpha } \in { \mathcal { E } } ( i , \alpha , F )$ . This n satisfies (8.21). 

To make an inductive step, let $\eta < \omega _ { 1 }$ be such that the construction is already made for all $\xi < \eta$ 

If $\eta$ is a limit ordinal, then $f \colon [ \eta ] ^ { 2 } \to 2$ is already constructed and it is easy to see that f satisfies $\left( { { I _ { \eta } } } \right)$ . So assume that $\eta = \xi + 1$ . We have to extend f to $\{ \{ \beta , \xi \} \colon \beta < \xi \}$ while maintaining $( I _ { \eta } )$ . So let 

$$
\mathcal {F} = \left\{\langle \mathcal {E} (i, \alpha , F), i \rangle \colon i <   2, \alpha \leq \xi , F \in [ \xi \setminus \alpha ] ^ {<   \omega}, \bigcup_ {n <   \omega} F _ {n} ^ {\alpha} \subset \alpha \right\}.
$$

Clearly $\mathcal { F }$ is countable, being indexed by a countable set. Note also that if $\langle \mathcal { E } ( i , \alpha , F ) , i \rangle \in \mathcal { F }$ then $\mathcal { E } ( i , \alpha , F )$ is infinite. For $\alpha ~ < ~ \xi$ this follows directly from the inductive assumption $\left( I _ { \xi } \right)$ . But if $\alpha = \xi$ then $F = \emptyset$ and $\mathcal { E } ( i , \alpha , F ) = \mathcal { E } ( i , \alpha , \emptyset ) = \{ F _ { n } ^ { \alpha } \colon n < \omega \}$ is infinite as well. 

Let $\langle \langle \mathcal { E } _ { m } , i _ { m } \rangle \colon m < \omega \rangle$ be an enumeration of $\mathcal { F }$ with each pair appearing infinitely many times. Since each ${ \mathcal { E } } _ { m }$ is an infinite family of pairwisedisjoint finite sets, we can construct by induction on m $< \omega$ a sequence $\langle E _ { m } \colon n < \omega \rangle$ of pairwise-disjoint sets such that $E _ { m } \in \mathcal { E } _ { m }$ for every $m \textless$ $\omega$ . Define $f ( \{ \beta , \xi \} ) = i _ { m }$ for every $\beta \in E _ { m }$ and $m < \omega _ { : }$ and extend it arbitrarily to $[ \eta ] ^ { 2 }$ . It is enough to show that $f$ satisfies condition $\left( { { I _ { \eta } } } \right)$ 

So let $i < 2 , \alpha < \eta = \xi + 1$ , and $\hat { F } \in [ \eta \backslash \alpha ] ^ { < \omega }$ be such that $\textstyle \bigcup _ { n < \omega } F _ { n } ^ { \alpha } \subset \alpha$ If ${ \hat { F } } = \emptyset$ then $\mathcal { E } ( i , \alpha , \hat { F } ) = \{ F _ { n } ^ { \alpha } \colon n < \omega \}$ <sub>is infinite, and</sub> (<sub>8.22</sub>) <sub>holds. So</sub> assume that ${ \hat { F } } \neq \emptyset$ . Now, if $\xi \not \in { \hat { F } }$ then (8.22) holds for $\hat { F }$ by $\left( I _ { \xi } \right)$ , since $\varnothing \neq { \hat { F } } \subset \xi \backslash$ α implies $\alpha < \xi$ . So assume that $\xi \in { \hat { F } }$ and let $F = \hat { F } \setminus \{ \xi \}$ Then $\langle \mathcal { E } ( i , \alpha , F ) , i \rangle \in \mathcal { F }$ and $\langle \mathcal { E } ( i , \alpha , F ) , i \rangle = \langle \mathcal { E } _ { m } , i _ { m } \rangle$ for infinitely many $m < \omega$ . In particular, for every such m we have 

$$
f (\{\beta , \xi \}) = i _ {m} = i\tag{8.23}
$$

for every $\beta \in E _ { m }$ . We claim that every such $E _ { m }$ belongs to $\mathcal { E } ( i , \alpha , \hat { F } )$ . This will finish the proof, since all sets $E _ { m }$ are diferent. But for every $\beta \in E _ { m }$ 

$$
f (\{\beta , \gamma \}) = i
$$

holds for $\gamma \in F = { \hat { F } } \setminus \{ \xi \}$ , since $E _ { m } \in \mathcal { E } _ { m } = \mathcal { E } ( i , \alpha , F )$ , and for $\gamma = \xi$ by (8.23). This finishes the proof.  

## EXERCISES

1 Let $X$ and $Y$ be nonempty sets. Show that the forcing $\langle { \mathrm { F u n c } } _ { \omega } ( X , Y ) , \supset \rangle$ is ccc if and only if $| Y | \le \omega$ . Hint: Use the ∆-system lemma. 

2 A subset $Z$ of R has strong measure zero if for every sequence $\langle \varepsilon _ { n } \colon n < \omega \rangle$ of positive numbers there exists a sequence $\langle J _ { n } \colon n < \omega \rangle$ of open intervals such that each $J _ { n }$ has length less than $\varepsilon _ { n }$ and $Z \subset \bigcup _ { n < \omega } J _ { n }$ . Assuming MA show that every $Z \in [ \mathbb { R } ] ^ { < \mathfrak { c } }$ has strong measure zero. Hint: Let B be the family of all open intervals with rational endpoints. For every $\langle \varepsilon _ { n } \colon n < \omega \rangle$ of positive numbers use forcing 

$\mathbb { P } = \{ J \in B ^ { n } \colon n < \omega$ & for every $k < n$ the length of $J ( k )$ is less than $\varepsilon _ { k } \}$ 

ordered by reverse inclusion $\supset$ 

3 (Due to Solovay) Infinite sets A and B are said to be almost disjoint provided $A \cap B$ is finite. Show that MA implies the following fact: If $\mathcal { A }$ is a family of almost-disjoint subsets of $\omega , | { \mathcal { A } } | < { \mathfrak { c } } .$ , and $\mathcal { C } \subset A$ , then there exists a set $S \subset \omega$ such that $S \cap C$ is finite for every $C \in { \mathcal { C } }$ and $S \cap A$ is infinite for $A \in { \mathcal { A } } \backslash { \mathcal { C } }$ . Hint: Use a forcing $\mathbb { P } = [ \omega ] ^ { < \omega } \times [ \mathcal { C } ] ^ { < \omega }$ ordered by $\langle s , \mathcal { E } \rangle \leq \langle s ^ { \prime } , \mathcal { E } ^ { \prime } \rangle$ if and only if $s \supset s ^ { \prime } , \mathcal { E } \supset \mathcal { E } ^ { \prime }$ , and $( s \setminus s ^ { \prime } ) \cap \bigcup \mathcal { E } ^ { \prime } = \emptyset$ 

4 We say that a set A is almost contained in $B$ and write $A \subset ^ { \star } B { \mathrm { ~ i f ~ } } A \setminus B$ is finite. Let $B \subset [ \omega ] ^ { \omega }$ be such that $\cap B _ { 0 }$ is infinite for every finite $B _ { 0 } \subset B$ If MA holds and $| B | < { \mathfrak { c } }$ show that there exists an $A \in [ \omega ] ^ { \omega }$ such that $A \subset ^ { \star } B$ for every $B \in B$ 

5 Assume MA and let B be a family of almost-disjoint subsets of ω such that $| B | < { \mathfrak { c } }$ . Show that for every $\mathcal { A } \in [ B ] ^ { \leq \omega }$ there exists a d $\subset \omega$ such that $a \subset { ^ { \star } }$ d for every $a \in { \mathcal { A } }$ and d ∩ b is finite for every $b \in B \setminus A$ . Hint: Let $\mathcal { A } ^ { \star } = \{ a \backslash n : n < \omega \ \& \ a \in \mathcal { A } \}$ and define $\mathbb { P } = [ \mathcal { A } ^ { \star } ] ^ { < \omega } \times [ \mathcal { B } \setminus \mathcal { A } ] ^ { < \omega }$ , ordered by $\langle A , B \rangle \leq \langle A ^ { \prime } , B ^ { \prime } \rangle$ if and only if $A \supset A ^ { \prime } , B \supset B ^ { \prime }$ , and $\bigcup ( A \setminus A ^ { \prime } ) \cap \bigcup B ^ { \prime } = \emptyset$  Use the forcing P to define the set d as the union of all sets A with $\langle A , B \rangle$ from an appropriate generic filter in P. 

6 (Challenging) Assume MA and let $\kappa ~ < ~ { \mathfrak { c } }$ be an uncountable regular cardinal. Show that for every family A of countable subsets of κ such that $| { \mathcal { A } } | < { \mathfrak { c } }$ there exists a $B \in [ \kappa ] ^ { \kappa }$ such that $A \cap B$ is finite for every $A \in { \mathcal { A } }$ Hint: Use a forcing similar to that from Exercise 3. Use the ∆-system lemma to prove that it is ccc. 

7 (Challenging) Generalize Exercise 6 as follows. Assume MA and let $\kappa < { \mathfrak { c } }$ be an uncountable regular cardinal. Show that for every family A of countable subsets of κ such that $| { \mathcal { A } } | < { \mathfrak { c } }$ there exists a countable cover $\{ P _ { n } \colon n < \omega \}$ of κ such that $A \cap P _ { n }$ is finite for every $A \in { \mathcal { A } }$ and $n < \omega$ Hint: If $\langle \mathbb { P } , \preceq \rangle$ is the partially ordered set used in Exercise 6, use the forcing $\mathbb { P } ^ { \star } = \operatorname { F u n c } _ { \omega } ( \omega , \mathbb { P } )$ ordered by $s \leq t { \mathrm { ~ i f ~ } } \mathrm { d o m } ( s ) \supset \mathrm { d o m } ( t )$ and $s ( n ) \preceq t ( n )$ for every $n \in \mathrm { d o m } ( t )$ 

## 8.3 Suslin hypothesis and diamond principle

Let $\langle X , \leq \rangle$ be a linear order. For $a , b \in X$ , an open interval with endpoints a and b is defined in a natural way as $( a , b ) = \{ x \in X \colon a < x < b \}$ . A linearly ordered set X is ccc provided every family of pairwise-disjoint open intervals in X is at most countable or, equivalently, when the partial order $\langle \tau \backslash \{ \varnothing \} , \subset \rangle$ is ccc, where τ is an order topology on X, that is, the topology generated by the family of all open intervals in X. 

In this terminology, Theorem 6.2.1(i) says that $\langle \mathbb { R } , \leq \rangle$ is ccc. 

Now let us turn our attention to Theorem 8.1.4. It says that a linearly ordered set $\langle X , \leq \rangle$ is isomorphic to $\langle \mathbb { R } , \leq \rangle$ if and only if it has the following properties. 

(a) X has neither a first nor a last element, and is dense in itself. 

(b) X is complete. 

(c) X contains a countable dense subset. 

In 1920 Suslin asked whether, in the preceding characterization, condi tion (c) can be replaced by the weaker condition 

(c<sup>-</sup>) X is ccc. 

The Suslin hypothesis SH is the statement that such a replacement indeed can be made, that is, that any ccc linearly ordered set $\langle X , \leq \rangle$ satisfying (a) and (b) contains a countable dense subset. 

In what follows we will use the term Suslin line for a ccc linearly ordered set $\langle X , \leq \rangle$ satisfying (a) that does not contain a countable dense subset. Thus a complete Suslin line is a counterexample for the Suslin hypothesis. In Exercise 1 we sketch the proof that the existence of a Suslin line implies the existence of a complete Suslin line. Thus the Suslin hypothesis is equivalent to the nonexistence of a Suslin line.<sup>3</sup> 

In what follows we will show that the Suslin hypothesis is independent of the ZFC axioms. We start with the following theorem. 

## Theorem 8.3.1 MA+¬CH implies the Suslin hypothesis.

Proof Assume MA+¬CH and, to obtain a contradiction, that there exists a Suslin line $\langle X , \leq \rangle$ . Then the partially ordered set $\langle \mathbb { P } , \leq \rangle = \langle \mathcal { I } , \subset \rangle$ is ccc, where J is the family of all nonempty open intervals in $\langle X , \leq \rangle$ . We will show that the product forcing $\mathbb { P } \times \mathbb { P }$ is not ccc, contradicting Corollary 8.2.10. 

For this, we construct by induction a sequence $\langle \langle a _ { \xi } , b _ { \xi } , c _ { \xi } \rangle \in X ^ { 3 } \colon \xi < \omega _ { 1 } \rangle$ such that for every $\xi < \omega _ { 1 }$ 

(i) $a _ { \xi } < b _ { \xi } < c _ { \xi }$ , and 

$$
\left(a _ {\xi}, c _ {\xi}\right) \cap \left\{b _ {\zeta}: \zeta <   \xi \right\} = \emptyset .\tag{ii}
$$

Such a construction can be easily made, since for every $\xi < \omega _ { 1 }$ the countable set $\{ b _ { \zeta } \colon \zeta < \xi \}$ cannot be dense, so there must exist $a _ { \xi } < c _ { \xi }$ in X such that $( \bar { a } _ { \xi } , c _ { \xi } ) \cap \{ b _ { \zeta } \colon \zeta < \xi \} = \varnothing$ . Thus such an element $b _ { \xi }$ can be chosen, since X is dense in itself. 

Now let $U _ { \xi } = \langle ( a _ { \xi } , b _ { \xi } ) , ( b _ { \xi } , c _ { \xi } ) \rangle \in \mathbb { P } \times \mathbb { P }$ . It is enough to show that $U _ { \zeta }$ and $U _ { \xi }$ are incompatible in $\mathbb { P } \times \mathbb { P }$ for every $\zeta < \xi < \omega _ { 1 }$ . This is the case since by (ii) either $b _ { \zeta } \leq a _ { \xi }$ , in which case $\left( a _ { \zeta } , b _ { \zeta } \right) \cap \left( a _ { \xi } , b _ { \xi } \right) = \varnothing$ , or $b _ { \zeta } \geq c _ { \xi }$ , in which case $( b _ { \zeta } , c _ { \zeta } \bar { \bf \phi } ) \cap ( b _ { \xi } , c _ { \xi } ) = \emptyset$  

The remainder of this section is devoted to the proof that the existence of a Suslin line is consistent with ZFC. 

Notice that in the proof of Theorem 8.3.1 we used MA+¬CH only to conclude that the product of ccc forcings is ccc, from which we deduced that there is no Suslin line. Moreover, from Theorem 8.2.12 we know that CH implies the existence of ccc forcings whose product is not ccc. Can we generalize this argument to construct a Suslin line $\langle X , \leq \rangle$ under CH? 

In what follows we will describe some dificulties that await any attempted inductive construction of a Suslin line. Then we will show the way to overcome these problems. In particular, the next lemma will be used to achieve both of these goals. It will illustrate the aforementioned dificulties, and will be used in our construction of a Suslin line. To state the lemma, we need the following notation, which will be used for the remainder of this section. 

For $\alpha \leq \omega _ { 1 }$ the symbol $\lambda _ { \alpha }$ will denote the αth limit ordinal number in $\omega _ { 1 } + 1$ . Thus $\lbrace \lambda _ { \alpha } \colon \alpha \leq \omega _ { 1 } \rbrace$ is a one-to-one increasing enumeration of the set of all limit ordinals in $\omega _ { 1 } + 1$ . In particular, $\lambda _ { 0 } = 0 , \lambda _ { 1 } = \omega .$ $\lambda _ { 2 } = \omega + \omega , \ldots ,$ , and 

$\lambda _ { \omega _ { 1 } } = \omega _ { 1 } \mathrm { a n d } \lambda _ { \alpha } = \bigcup _ { \beta < \alpha } \lambda _ { \beta }$ for every limit ordinal $\alpha \leq \omega _ { 1 }$ 

Also, for $\alpha < \omega _ { 1 }$ let $\mathbb { Q } _ { \alpha } = \left\{ \lambda _ { \alpha } + n \colon n < \omega \right\}$ and let $\leq _ { \alpha }$ be a linear-order relation on $\mathbb { Q } _ { \alpha }$ giving it the order type of $\langle \mathbb { Q } , \leq \rangle$ . Notice that $\lambda _ { \alpha + 1 } ~ =$ $\lambda _ { \alpha } \cup \mathbb { Q } _ { \alpha }$ for every $\alpha < \omega _ { 1 }$ and that 

$$
\alpha \leq \lambda_ {\alpha} = \bigcup \{\mathbb {Q} _ {\zeta}: \zeta <   \alpha \} \text {   for   every   } \alpha \leq \omega_ {1}.
$$

Lemma 8.3.2 Let $\alpha \leq \omega _ { 1 } . \ I f \left. S _ { \beta } \subset \lambda _ { \beta } : \beta < \alpha \right.$ and $\langle \preceq _ { \beta } \subset \lambda _ { \beta } \times \lambda _ { \beta } \colon \beta \leq \alpha \rangle$ are such that for every $\beta < \gamma \leq \alpha$ 

(1) $\preceq \beta$ is a linear-order relation on $\lambda _ { \beta }$ ; 

(2) $S _ { \beta }$ is a proper initial segment of $\langle \lambda _ { \beta } , \preceq _ { \beta } \rangle$ ; 

(3) $\scriptstyle \preceq _ { \gamma } = \bigcup _ { \delta < \gamma } ( \preceq _ { \delta } )$ if γ is a limit ordinal; 

(4) $i f \gamma = \xi + 1$ then the relation $\preceq \gamma$ on $\lambda _ { \gamma } = \lambda _ { \xi } \cup \mathbb { Q } _ { \xi }$ is defined from $\preceq \xi$ $b y ~ ^ { \it a } s t i c k i n g ^ { \it n }$ the entire $\langle \mathbb { Q } _ { \xi } , \leq _ { \xi } \rangle$ between $S _ { \xi }$ and $\lambda _ { \xi } \setminus S _ { \xi } ,$ that $i s , \preceq _ { \gamma }$ extends $\preceq \cup \leq \varepsilon$ and is defined for every $\langle x , q \rangle \in \lambda _ { \xi } \times \mathbb { Q } _ { \xi }$ by: $x \preceq _ { \gamma } q$ if $x \in S _ { \xi }$ , and $q \preceq _ { \gamma } x i f x \in \lambda _ { \xi } \setminus S _ { \xi } $ ; 

then for every $\gamma \leq \alpha$ 

(I) $\langle \lambda _ { \gamma } , \preceq _ { \gamma } \rangle$ is a linearly ordered set that is dense in itself and has neither a largest nor a smallest element. 

Moreover, if $\alpha = \omega _ { 1 }$ then $\langle \omega _ { 1 } , \preceq _ { \omega _ { 1 } } \rangle$ does not have a countable dense subset. 

Proof Condition (I) is easily proved by induction on $\alpha \leq \omega _ { 1 }$ . Its proof is left as an exercise. 

To see that $\langle \omega _ { 1 } , \preceq _ { \omega _ { 1 } } \rangle$ does not have a countable dense subset take a countable set $D \subset \omega _ { 1 } .$ . Then there is a $\xi < \omega _ { 1 }$ such that $D \subset \lambda _ { \xi }$ . Choose $a , b \in \mathbb { Q } _ { \xi }$ such that $a \prec _ { \xi } b$ . Then, by (4), there is no $d \in D$ such that $a \prec _ { \omega _ { 1 } } d \prec _ { \omega _ { 1 } } b$ . So D is not dense.  

The linear order $\langle \omega _ { 1 } , \preceq _ { \omega _ { 1 } } \rangle$ constructed as in Lemma 8.3.2 has already all the properties of a Suslin line, except possibly that of being ccc. Thus the question is, Can we make it ccc? 

Clearly, we have the freedom of choice of initial segments $S _ { \alpha }$ . Such a choice can $^ { 6 6 } \mathrm { k i l l } ^ { \mathrm { s } }$ a potential uncountable antichain $\langle ( a _ { \zeta } , b _ { \zeta } ) : \zeta < \omega _ { 1 } \rangle$ by making sure that, starting from some $\alpha ~ < ~ \omega _ { 1 }$ , all $\mathbb { Q } _ { \xi }$ for $\xi \ge \alpha$ will be placed inside some $( a _ { \zeta } , b _ { \zeta } )$ for $\zeta < \alpha$ . This would imply that there are only countably many points of $\omega _ { 1 }$ outside $\textstyle \bigcup _ { \zeta < \alpha } ( a _ { \zeta } , b _ { \zeta } )$ , making it impossible for $\langle ( a _ { \zeta } , b _ { \zeta } ) \colon \zeta \ < \ \omega _ { 1 } \rangle$ to be an antichain. There is, however, a problem in carrying out such a construction using only CH, since we have an induction of only length $\omega _ { 1 }$ , and we have to $\mathrm { ^ { 6 4 } k i l l ^ { 3 } } \ 2 ^ { \omega _ { 1 } }$ potential antichains $\langle ( a _ { \zeta } , b _ { \zeta } ) \colon \zeta < \omega _ { 1 } \rangle$ . Thus once more we face the problem of having a “too short induction.” Moreover, Theorem 8.3.1 shows that Martin’s axiom can’t help us this time. Someone may still have a hope that, through some trick, we can reduce the number of steps necessary to rescue this construction. Indeed, this is what we will do. However, such a “trick” can’t be found with the help of CH alone, as it is known that the existence of a Suslin line cannot be concluded just from the continuum hypothesis. Thus we will need another “magic” axiom, which will show us the way out of our dilemma. To formulate it, we need some new definitions. 

A subset C of $\omega _ { 1 }$ is closed if for every $S \subset C$ its union S is in $C \cup \{ \omega _ { 1 } \}$ or, equivalently, when every limit ordinal $\lambda < \omega _ { 1 }$ is in C provided $C \cap \lambda$ is unbounded in λ. (In fact, being closed in $\omega _ { 1 }$ is equivalent to being closed in the order topology of $\omega _ { 1 \cdot } )$ For example, a nonzero ordinal number $\alpha < \omega _ { 1 }$ is closed in $\omega _ { 1 }$ (as a subset) if and only if it is a successor ordinal. 

In what follows we will be primarily interested in closed unbounded subsets of $\omega _ { 1 }$ (see Section 5.3). Notice that these sets are quite big, as follows from the next proposition. 

Proposition 8.3.3 If C and D are closed, unbounded subsets of $\omega _ { 1 }$ then $C \cap D$ is also closed and unbounded. 

Proof Clearly, $C \cap D$ is closed, since for every $S \subset C \cap D$ its union $\cup S$ is both in $C \cup \{ \omega _ { 1 } \}$ and in $D \cup \{ \omega _ { 1 } \}$ 

To see that $C \cap D$ is unbounded in $\omega _ { 1 }$ , pick $\alpha ~ < ~ \omega _ { 1 }$ and define by induction the sequences $\langle \gamma _ { n } \in C : n < \omega \rangle$ and $\langle \delta _ { n } \in D \colon n < \omega \rangle$ such that $\alpha < \gamma _ { n } < \delta _ { n } < \gamma _ { n + 1 }$ for every $n < \omega$ . It can be done since sets C and 

D are unbounded in $\omega _ { 1 }$ . Then $\begin{array} { r } { \beta = \bigcup _ { n < \omega } \gamma _ { n } = \bigcup _ { n < \omega } \delta _ { n } < \omega _ { 1 } } \end{array}$ belongs to $C \cap D$ and is greater than α.  

One of the most important facts we will use about the closed unbounded sets is the following proposition. 

Proposition 8.3.4 Let $\mathcal { F }$ be a countable family of functions of the form $f \colon \omega _ { 1 } ^ { n }  \omega _ { 1 } ~ o r ~ f \colon \omega _ { 1 } ^ { n }  [ \omega _ { 1 } ] ^ { \leq \omega }$ with $n < \omega$ . If 

$D = \{ \alpha < \omega _ { 1 } \colon \alpha$ is closed under the action of ${ \mathcal { F } } \}$ 

then D is closed and unbounded. 

Proof It is easy to see that D is closed (compare the proof of Lemma 6.1.6). To see that it is unbounded pick $\beta < \omega _ { 1 }$ and let $i \colon \bar { \omega } _ { 1 }  [ \omega _ { 1 } ] ^ { \leq \omega }$ be given by $i ( \alpha ) = \alpha = \{ \beta \colon \beta < \alpha \} \in [ \omega _ { 1 } ] ^ { \leq \omega }$ . Then, by Lemma $6 . 1 . 6 ( \mathrm { a } )$ used with $Z = \beta$ , there is a countable subset $Y$ of $\omega _ { 1 }$ that is closed under the action of ${ \mathcal { F } } \cup \{ i \}$ . In particular, closure under the action of $\{ i \}$ implies that $Y$ is an ordinal number. So $Y$ is a countable ordinal number containing $\beta$ and belonging to D.  

A subset $S$ of $\omega _ { 1 }$ is stationary if $S \cap C \neq \emptyset$ for every closed unbounded set $C \subset \omega _ { 1 }$ . The theory of stationary sets is one of the most beautiful and useful parts of set theory. However, due to lack of space, we will not be able to develop it here in full. Some traces of its power can be found in the rest of this section and in the exercises. 

The additional axiom we will need is called the diamond principle and is usually denoted by the symbol $\diamondsuit$ . It reads as follows. 

Diamond principle $\diamondsuit$ There exists a sequence $\langle A _ { \alpha } \subset \omega _ { 1 } \colon \alpha \ < \ \omega _ { 1 } \rangle$ , known as a ♦-sequence, such that for every $A \subset \omega _ { 1 }$ the set 

$$
\{\alpha <   \omega_ {1} \colon A \cap \alpha = A _ {\alpha} \}
$$

is stationary. 

Notice that 

Proposition 8.3.5 $\diamondsuit$ implies CH. 

Proof Let $A \subset \omega$ . Since $C = \omega _ { 1 } \backslash \omega$ is closed and unbounded, there exists an $\alpha \in C$ such that $A _ { \alpha } = A \cap \alpha = A \cap \omega = A$ . Thus $\left\{ A _ { \alpha } \cap \omega \colon \alpha < \omega _ { 1 } \right\} =$ $\mathcal { P } ( \omega )$  

In the next chapter we will show that $\diamondsuit$ is consistent with the ZFC axioms. It is also true that it does not follow from CH. Thus we have the following implications, none of which can be reversed: 

$$
\Diamond \Rightarrow C H \Rightarrow M A.
$$

As we have just seen a ♦-sequence lists all subsets of $\omega$ . But it also captures a lot of information regarding uncountable subsets of $\omega _ { 1 }$ . This will be enough to overcome the obstacles to the construction of a Suslin line described earlier. For the construction we need the following easy lemma. 

Lemma 8.3.6 $I f \diamondsuit$ holds then there exists a sequence $\langle B _ { \alpha } \subset \alpha \times \alpha \colon \alpha < \omega _ { 1 } \rangle$ such that for every $B \subset \omega _ { 1 } \times \omega _ { 1 }$ the set 

$$
\{\alpha <   \omega_ {1} \colon B \cap (\alpha \times \alpha) = B _ {\alpha} \}
$$

is stationary. 

Proof Let $f _ { 0 } , f _ { 1 } \colon \omega _ { 1 }  \omega _ { 1 }$ be such that $f \colon \omega _ { 1 } \  \ \omega _ { 1 } ^ { 2 }$ given by $f ( \xi ) =$ $\langle f _ { 0 } ( \xi ) , f _ { 1 } ( \xi ) \rangle$ is a bijection and let $B _ { \alpha } = f [ A _ { \alpha } ] \cap ( \alpha \times \alpha )$ . Notice that, by Proposition 8.3.4 used with the family $\mathcal { F } = \{ f _ { 0 } , f _ { 1 } , f ^ { - 1 } \}$ , the set $D =$ $\{ \alpha \colon f [ \alpha ] = \alpha \times \alpha \}$ is closed and unbounded. 

To see that the sequence $\langle B _ { \alpha } \colon \alpha < \omega _ { 1 } \rangle$ has the desired properties, take $B \subset \omega _ { 1 } \times \omega _ { 1 }$ and let $C \subset \omega _ { 1 }$ be closed and unbounded. We must find an $\alpha \in C$ such that $B _ { \alpha } = B \cap ( \alpha \times \alpha )$ 

Since $C \cap D$ is closed and unbounded and $\{ \alpha < \omega _ { 1 } \colon f ^ { - 1 } ( B ) \cap \alpha = A _ { \alpha } \}$ is stationary, there is an $\alpha \in C \cap D$ such that $A _ { \alpha } = f ^ { - 1 } ( B ) \cap \alpha$ . But $\alpha \in D$ implies that 

$$
A _ {\alpha} = f ^ {- 1} (B) \cap \alpha = f ^ {- 1} (B) \cap f ^ {- 1} (\alpha \times \alpha) = f ^ {- 1} (B \cap (\alpha \times \alpha)).
$$

Hence $B _ { \alpha } = f [ A _ { \alpha } ] \cap ( \alpha \times \alpha ) = B \cap ( \alpha \times \alpha ) .$ 

Theorem 8.3.7 $I f \diamondsuit$ holds then there exists a Suslin line $\langle X , \preceq \rangle$ . In $p a r \_$ ticular, the Suslin hypothesis fails. 

Proof We will construct $\langle X , \preceq \rangle = \langle \omega _ { 1 } , \preceq _ { \omega 1 } \rangle$ as in Lemma 8.3.2, following the idea described after its proof. The sequence $\langle B _ { \alpha } \subset \alpha \times \alpha \colon \alpha < \omega _ { 1 } \rangle$ from Lemma 8.3.6 will be used as an “oracle” that will tell us how to choose initial segments $S _ { \alpha }$ so as to $^ { 6 6 } \mathrm { k i l l } ^ { \mathrm { s } }$ all potential uncountable antichains. 

Thus we will construct inductively the sequences $\langle S _ { \alpha } \subset \lambda _ { \alpha } \colon \alpha < \omega _ { 1 } \rangle$ and $\left. \preceq _ { \alpha } \subset \lambda _ { \alpha } \times \lambda _ { \alpha } \colon \alpha \leq \omega _ { 1 } \right.$ such that for every $\beta < \alpha \le \omega _ { 1 }$ 

(1) $\preceq _ { \alpha }$ is a linear-order relation on $\lambda _ { \alpha }$ ; 

(2) $S _ { \beta }$ is a proper initial segment of $\langle \lambda _ { \beta } , \preceq _ { \beta } \rangle$ ; 

(3) $\scriptstyle { \preceq _ { \alpha } } = \bigcup _ { \beta < \alpha } ( \preceq _ { \beta } )$ if α is a limit ordinal; 

(4) if $\alpha = \xi + 1 \ \mathrm { t h e n } \preceq _ { \alpha }$ extends $\preceq \cup \leq \varepsilon$ and for every $\langle x , q \rangle \in \lambda _ { \xi } \times \mathbb { Q } _ { \xi }$ is defined by: $x \preceq _ { \alpha } q$ if $x \in S _ { \xi }$ , and $q \preceq _ { \alpha }$ x if $x \in \lambda _ { \xi } \setminus S _ { \xi }$ 

Note that by Lemma 8.3.2 we know that such a construction can be made and that $\langle X , \preceq \rangle$ obtained this way is linearly ordered, is dense in itself, has neither a largest nor a smallest element, and does not have a countable dense subset. So it is enough to show that we can choose sets $S _ { \alpha }$ such that $\langle X , \preceq \rangle$ will be ccc. 

So assume that for some $\alpha < \omega _ { 1 }$ the sequences $\langle S _ { \beta } \subset \lambda _ { \beta } \colon \beta < \alpha \rangle$ and $\langle \preceq _ { \beta } \subset \lambda _ { \beta } \times \lambda _ { \beta } \colon \beta \leq \alpha \rangle$ are already constructed. We must construct the proper initial segment $S _ { \alpha }$ of $\lambda _ { \alpha }$ . It will be done as follows. 

For $a , b \in \lambda _ { \alpha }$ let $( a , b ) _ { \alpha }$ be an open interval in $\langle \lambda _ { \alpha } , \preceq _ { \alpha } \rangle$ with the endpoints a and b, that is, 

$$
(a, b) _ {\alpha} = \{x \in \lambda_ {\alpha}: a \prec_ {\alpha} x \prec_ {\alpha} b \},
$$

and for $\zeta \leq \alpha$ let 

$$
\mathcal {C} _ {\zeta} ^ {\alpha} = \{(a, b) _ {\alpha}: \langle a, b \rangle \in B _ {\zeta} \}.
$$

Notice that $B _ { \zeta } \subset \zeta \times \zeta \subset \lambda _ { \alpha } \times \lambda _ { \alpha }$ , so $\mathcal { C } _ { \zeta } ^ { \alpha }$ is well defined. Define the family ${ \mathcal { F } } _ { \alpha }$ as 

$\{ \mathcal { C } _ { \zeta } ^ { \alpha } \colon \zeta \leq \alpha$ and $\mathcal { C } _ { \zeta } ^ { \alpha }$ is a maximal family of disjoint intervals in $\langle \lambda _ { \alpha } , \preceq _ { \alpha } \rangle \}$ 

and let $\{ \mathcal { E } _ { n } : n < \omega \} = \mathcal { F } _ { \alpha } \cup \{ \hat { \mathcal { C } } \}$ , where $\hat { \mathcal { C } }$ is an arbitrary maximal family of pairwise-disjoint intervals in $\langle \lambda _ { \alpha } , \preceq \rangle$ . (We add $\hat { \mathcal { C } }$ to this list just to avoid a problem when ${ \mathcal { F } } _ { \alpha } = \varnothing . )$ 

The idea of the proof is that the elements of $\textstyle \bigcup _ { \alpha < \omega _ { 1 } } { \mathcal { F } } _ { \alpha }$ will be approxi-mations of all the potential families of pairwise-disjoint intervals in $\langle X , \preceq \rangle$ We will make sure that every family $\mathcal { C } \in \mathcal { F } _ { \alpha }$ remains maximal after step α by “sticking” every $\mathbb { Q } _ { \beta }$ for $\alpha \le \beta < \omega _ { 1 }$ inside some interval $I \in { \mathcal { C } }$ , thus adding no new elements of X outside $\cup { \mathcal { C } }$ 

So define, by induction on $n < \omega .$ , a sequence $\langle \langle a _ { n } , b _ { n } \rangle \in \lambda _ { \alpha } { \times } \lambda _ { \alpha } \colon n < \omega \rangle$ such that for every $n < \omega$ 

$$
\text {(A)} \quad a \prec_ {\alpha} a _ {n} \prec_ {\alpha} b _ {n} \prec_ {\alpha} b \text {   for   some   } (a, b) _ {\alpha} \in \mathcal {E} _ {n}; \text {   and   }\tag{B}
$$

$$
a _ {n - 1} \prec_ {\alpha} a _ {n} \prec_ {\alpha} b _ {n} \prec_ {\alpha} b _ {n - 1} \text {   for   } n > 0.
$$

Such a construction can be made since, by Lemma 8.3.2, $\langle \lambda _ { \alpha } , \preceq _ { \alpha } \rangle$ is dense in itself and, by the maximality of $\mathcal { E } _ { n } .$ , the interval $( a _ { n - 1 } , b _ { n - 1 } ) _ { \alpha }$ must intersect some $( a , b ) _ { \alpha } \in \mathcal { E } _ { n }$ . We define $S _ { \alpha } = \{ x \in \lambda _ { \alpha } \colon \exists n < \omega ~ ( x \preceq _ { \alpha } a _ { n } ) \}$ This finishes the construction. 

Now notice that if $\mathcal { C } _ { \zeta } ^ { \alpha } \in \mathcal { F } _ { \alpha }$ for some $\zeta \ \leq \ \alpha \ < \ \omega _ { 1 }$ , then there are $n < \omega$ and $a , b \in \lambda _ { \alpha }$ such that $a \prec _ { \alpha } a _ { n } \prec _ { \alpha } b _ { n } \prec _ { \alpha } b , ( a , b ) _ { \alpha } \in \mathcal { C } _ { \zeta } ^ { \alpha }$ , and $a _ { n } \in S _ { \alpha }$ but $b _ { n } \notin S _ { \alpha }$ . In particular, $\mathbb { Q } _ { \alpha } \subset ( a _ { n } , b _ { n } ) _ { \alpha + 1 } \subset \bigcup { \mathcal { C } } _ { \zeta } ^ { \alpha + 1 }$ and $\mathcal { C } _ { \zeta } ^ { \alpha + 1 }$ remains a maximal family of pairwise-disjoint intervals in $\langle \lambda _ { \alpha + 1 } , \preceq _ { \alpha + 1 } \rangle$ . So $\mathcal { C } _ { \zeta } ^ { \alpha + 1 } \in \mathcal { F } _ { \alpha + 1 }$ 

Using this, we can easily prove by induction on $\beta < \omega _ { 1 }$ that for every $\alpha < \omega _ { 1 }$ 

$$
\text { if } \mathcal {C} _ {\alpha} ^ {\alpha} \in \mathcal {F} _ {\alpha} \text { and } \alpha <   \beta <   \omega_ {1} \text { then } \bigcup_ {\alpha \leq \gamma <   \beta} \mathbb {Q} _ {\gamma} \subset \bigcup \mathcal {C} _ {\alpha} ^ {\beta} \text { and } \mathcal {C} _ {\alpha} ^ {\beta} \in \mathcal {F} _ {\beta}.
$$

This, in particular, implies that $\begin{array} { r } { \bigcup _ { \alpha \leq \gamma < \omega _ { 1 } } \mathbb { Q } _ { \gamma } \subset \bigcup \mathcal { C } _ { \alpha } ^ { \omega _ { 1 } } } \end{array}$ provided $\mathcal { C } _ { \alpha } ^ { \alpha } \in \mathcal { F } _ { \alpha }$ , that is, that 

$\mathcal { C } _ { \alpha } ^ { \omega _ { 1 } }$ is a maximal family of disjoint intervals in $\langle X , \preceq \rangle$ , if $\mathcal { C } _ { \alpha } ^ { \alpha } \in \mathcal { F } _ { \alpha }$ . (8.24) 

To see that $\langle X , \preceq \rangle$ is ccc assume, to obtain a contradiction, that there is an uncountable family $\mathcal { A } _ { \mathrm { 0 } }$ of nonempty pairwise-disjoint intervals in $\langle X , \preceq \rangle$ Using Zorn’s lemma we can extend $\mathcal { A } _ { \mathrm { 0 } }$ to a maximal family A of nonempty pairwise-disjoint intervals in $\langle X , \preceq \rangle$ . Put $B = \{ \langle a , b \rangle \colon ( a , b ) _ { \omega _ { 1 } } \in \mathcal { A } \}$ . The maximality of $\mathcal { A }$ means that for every $a , b \in X$ , with $a \prec b$ , there exists a nonempty interval $( l , r ) _ { \omega _ { 1 } } = ( l ( a , b ) , r ( a , b ) ) _ { \omega _ { 1 } } \in \mathcal { A }$ intersecting $( a , b ) _ { \omega _ { 1 } }$ Let $l , r \colon \omega _ { 1 } ^ { 2 } \  \ \omega _ { 1 }$ be functions having the foregoing property and let $\Lambda \colon \omega _ { 1 }  \omega _ { 1 }$ be given by $\Lambda ( \xi ) = \lambda _ { \xi } + 1$ . Put 

$D = \{ \alpha < \omega _ { 1 }$ : α is closed under the action of $\{ \Lambda , l , r \} \}$ 

By Proposition 8.3.4, D is closed and unbounded in $\omega _ { 1 }$ . Moreover, for every $\alpha \in D$ , 

$$
\lambda_ {\alpha} = \alpha ,\tag{8.25}
$$

and 

$$
\mathcal {D} _ {\alpha} = \left\{(l, r) _ {\alpha}: \langle l, r \rangle \in B \cap (\alpha \times \alpha) \right\}\tag{8.26}
$$

is a maximal family of pairwise-disjoint intervals in $\langle \lambda _ { \alpha } , \preceq _ { \alpha } \rangle = \langle \alpha , \preceq _ { \alpha } \rangle$ 

Condition (8.25) follows from the fact that α is closed under the action of Λ. To see why, notice first that α is a limit ordinal, since $\xi + 1 \le \lambda _ { \xi } + 1 =$ $\Lambda ( \xi ) < \alpha$ for every $\xi < \alpha$ . Now $\begin{array} { r } { \lambda _ { \alpha } = \bigcup _ { \varepsilon < \alpha } \lambda _ { \xi } \leq \alpha \leq \lambda _ { \alpha } } \end{array}$ 

Condition (8.26) follows from the closure of α under the actions of l and r, since for every $a , b \in \alpha = \lambda _ { \alpha }$ , with $a \prec _ { \alpha } b .$ , there are $l = l ( a , b ) < \alpha$ and $r = r ( a , b ) < \alpha$ with $( l , r ) _ { \omega _ { 1 } } \in \mathcal { A }$ intersecting $( a , b ) _ { \omega _ { 1 } }$ . This clearly implies that $( l , r ) _ { \alpha } \in \mathcal { D } _ { \alpha }$ intersects $( a , b ) _ { \alpha }$ , making $\mathcal { D } _ { \alpha }$ maximal in $\langle \lambda _ { \alpha } , { \preceq } _ { \alpha } \rangle =$ $\langle \alpha , \preceq _ { \alpha } \rangle$ 

By the choice of the sequence $\langle B _ { \alpha } \subset \alpha \times \alpha \colon \alpha < \omega _ { 1 } \rangle$ there exists an $\alpha \in D$ such that $B \cap ( \alpha \times \alpha ) = B _ { \alpha }$ . Hence, by (8.25) and (8.26), 

$$
\mathcal {C} _ {\alpha} ^ {\alpha} = \left\{(l, r) _ {\alpha} \colon \langle l, r \rangle \in B _ {\alpha} \right\} = \left\{(l, r) _ {\alpha} \colon \langle l, r \rangle \in B \cap (\alpha \times \alpha) \right\} = \mathcal {D} _ {\alpha}
$$

is a maximal family of pairwise-disjoint intervals in $\langle \alpha , \preceq _ { \alpha } \rangle = \langle \lambda _ { \alpha } , \preceq _ { \alpha } \rangle$ Hence, by the definition of $\mathcal { F } _ { \alpha } , \mathcal { C } _ { \alpha } ^ { \alpha } \in \mathcal { F } _ { \alpha }$ . So, by $( 8 . 2 4 ) , \mathcal { C } _ { \alpha } ^ { \omega _ { 1 } }$ is a maximal antichain in $\langle X , \preceq \rangle$ , contradicting the fact that $\mathcal { C } _ { \alpha } ^ { \omega _ { 1 } }$ is a proper subset of an uncountable antichain A. Thus we have proved that $\langle X , \preceq \rangle$ is ccc.  

## EXERCISES

1 Let $\langle X , \leq \rangle$ be a Suslin line and let $X ^ { \star }$ be the family of all proper nonempty initial segments of X without last elements. Prove that $\langle X ^ { \star } , \subset \rangle$ is a complete Suslin line. 

2 Let $\langle X , \leq \rangle$ be a ccc linearly ordered set and assume that $X$ , considered as a topological space with the order topology, does not have a countable dense subset. Show that there exists an $X _ { 0 } ~ \subset ~ X$ such that $\langle X _ { 0 } , \leq \rangle$ is a Suslin line and for every a, $b \in X _ { 0 }$ , with $a < b$ , there is no countable dense subset of $( a , b ) \cap X _ { 0 }$ Hint: Define an equivalence relation $\sim$ on $X$ by putting $x \sim y$ if and only if the interval between them contains a countable subset that is dense in it with respect to the order topology. Choose $X _ { 0 }$ to be any selector from the family of all equivalence classes of $\sim ,$ from which the least and the greatest elements are removed, if they exist. 

3 Complete the proof of Lemma 8.3.2 by proving condition (I). 

4 Prove that if sets $C _ { n } \subset \omega _ { 1 }$ are closed and unbounded then $\cap _ { n < \omega } C _ { n }$ is closed and unbounded. 

5 Let $\{ C _ { \alpha } \subset \omega _ { 1 } \colon \alpha < \omega _ { 1 } \}$ be a family of closed unbounded sets. Prove that the set 

$$
D = \{\gamma <   \omega_ {1} \colon \gamma \in C _ {\alpha} \text { for   all } \alpha <   \gamma \},
$$

known as the diagonal intersection of the sets $C _ { \alpha } .$ , is closed and unbounded. 

6 Prove the following theorem, known as the pressing-down lemma or Fodor’s theorem: 

Let $S \subset \omega _ { 1 }$ be a stationary set and let $f \colon S  \omega _ { 1 }$ be such that $f ( \gamma ) < \gamma$ for every $\gamma \in S$ (such a function is called a regressive function). Then there exists an $\alpha < \omega _ { 1 }$ such that $f ^ { - 1 } ( \{ \alpha \} )$ is stationary. 

Hint: Otherwise for every α there exists a closed and unbounded set $C _ { \alpha }$ disjoint from $f ^ { - 1 } ( \{ \alpha \} )$ . Consider the diagonal intersection D of the sets $C _ { \alpha }$ and show that it is disjoint from $S _ { ☉ }$ 

7 A tree is a partially ordered set $\langle T , \leq \rangle$ with a smallest element such that the relation < is well founded, that is, that every initial segment of $T$ is well ordered. A Suslin tree is an uncountable tree that, considered as a forcing with the reversed order $\langle T , \leq \rangle$ , has neither uncountable chains nor uncountable antichains. Show the existence of a Suslin line implies the existence of a Suslin tree. Hint: Start with a Suslin line $\langle X _ { 0 } , \leq \rangle$ as in Exercise 2. Define, by induction on $\xi < \omega _ { 1 }$ , a sequence $\langle T _ { \xi } \colon \xi < \omega _ { 1 } \rangle$ such that $T _ { 0 } = X _ { 0 }$ and each $T _ { \xi }$ for $\xi > 0$ is a maximal family of pairwise-disjoint intervals in $X _ { 0 }$ , none of which contain any endpoint of any interval from $\cup _ { \zeta < \xi } T _ { \zeta }$ . Then $T = \textstyle \bigcup _ { \xi < \omega _ { 1 } } T _ { \xi }$ ordered by reverse inclusion $\supset$ is a Suslin tree. 

8 Show that the existence of a Suslin tree $\langle T , \leq \rangle$ implies the existence of a Suslin line. (Thus the existence of a Suslin line is equivalent to the existence of a Suslin tree.) Hint: Let $\preceq$ be any linear order on $T$ and let X be the family of all strictly increasing functions $f$ from an ordinal number α into $\langle T , \leq \rangle$ such that $f [ \alpha ]$ is a maximal chain in $T$ (such an f is called a branch of $T )$ . For diferent $f , g \in X$ define $f < g { \mathrm { ~ i f ~ } } f ( \beta ) \prec g ( \beta )$ , where $\beta$ is the smallest ordinal for which $f ( \beta ) \neq g ( \beta )$ . Show that $\langle X , \leq \rangle$ is a ccc linearly ordered set such that $X$ , considered as a topological space with the order topology, does not have a countable dense subset. Then use Exercise 2. 

9 For a tree $\langle T , \leq \rangle$ and an ordinal number α, the α-level of $T$ is the set of all $t \in T$ for which the initial segment generated by t has order type α. (Thus any level of $T$ is an antichain.) An Aronszajn tree is an uncountable tree with no uncountable chains and all levels countable. (Thus every Suslin tree is an Aronszajn tree.) Show, in ZFC, that there exists an Aronszajn tree. Hint: For $f , g \colon \alpha  \omega$ write $f = ^ { \star } g$ if the set $\{ \beta < \alpha \colon f ( \beta ) \neq g ( \beta ) \}$ is finite. Define, by induction on $\alpha < \omega _ { 1 }$ , a sequence of one-to-one functions $\langle s _ { \alpha } \in \omega ^ { \alpha } \colon \alpha < \omega _ { 1 } \rangle$ such that $\omega \cdot { \mathrm { r a n g e } } ( s _ { \alpha } )$ is infinite and $s _ { \alpha } | _ { \beta } = ^ { \star } ~ s _ { \beta }$ for every $\beta < \alpha$ . Define $T = \{ s \in \omega ^ { \alpha } \colon \alpha < \omega _ { 1 } \ \& \ s = ^ { \star } \ s _ { \alpha } \}$ and relation $\leq$ as reverse inclusion ⊃. 

## Chapter 9

## Forcing

In this chapter we will describe a technique for proving that some settheoretic statements are independent of the $\mathrm { Z F C }$ axioms. This technique is known as the forcing method. We will not prove here all the theorems needed to justify this method. (Sketches of some of the missing proofs are included in Appendix B. The complete proofs can be found, for example, in Kunen (1980).) Instead, we will describe only the essentials for its use and concentrate on its applications.<sup>1</sup> 

## 9.1 Elements of logic and other forcing preliminaries

We will start here with some definitions, which will serve as technical tools to develop the forcing method. 

A set M is said to be transitive if $x \subset M$ for every $x \in M$ , that is, if $a \in x$ and $x \in M$ imply that $a \in M$ 

Lemma 9.1.1 For every set x there exists a smallest transitive set trcl(x) such that $x \subset \operatorname { t r c l } ( x )$ 

Proof Define, by induction on $n < \omega$ 

$$
U _ {0} (x) = x \text { and } U _ {n + 1} (x) = \bigcup U _ {n} (x) \text { for } n <   \omega .
$$

Then trcl $\begin{array} { r } { ( x ) \ = \bigcup _ { n < \omega } U _ { n } ( x ) } \end{array}$ is the desired set. It is transitive, since for every $y \in \operatorname { t r c l } ( x )$ there is an $n \ < \ \omega$ such that $y \in U _ { n } ( x )$ . Then $y \subset$ $\bigcup U _ { n } ( x ) = U _ { n + 1 } ( x ) \subset \operatorname { t r c l } ( x )$ 

To prove the minimality of trcl(x) it is enough to take a transitive set M with $x \subset M$ and show, by induction on $n < \omega$ , that $U _ { n } \subset M$ for every $n < \omega$ . The details are left as an exercise.  

The set trcl(x) from Lemma 9.1.1 is called the transitive closure of x. 

For an ordinal number α define inductively a sequence $\langle R ( \beta ) \colon \beta \leq \alpha \rangle$ by putting 

(a) $R ( 0 ) = \varnothing ,$ 

(b) $R ( \beta + 1 ) = \mathcal { P } ( R ( \beta ) ) \ \mathrm { f o r } \ \beta < \alpha .$ , and 

(c) $\begin{array} { r } { R ( \lambda ) = \bigcup _ { \beta < \lambda } R ( \beta ) } \end{array}$ for every limit ordinal $\lambda \leq \alpha$ 

Note that the sequence $\langle R ( \beta ) \colon \beta \leq \alpha \rangle$ is increasing, that is, that 

$R ( \beta ) \subset R ( \gamma )$ for every ordinal numbers $\gamma < \beta \leq \alpha$ 

(9.1) 

An easy inductive proof of this fact is left as an exercise. 

Lemma 9.1.2 For every set x there exists an ordinal number α such that $x \in R ( \alpha )$ 

Proof First notice that for any set x, 

(G) if for every $y \in x$ there exists an ordinal number α such that $y \in R ( \alpha )$ then $x \in R ( \alpha _ { 0 } )$ for some ordinal $\alpha _ { 0 }$ 

To see this, let r be a function such that $r ( y ) = \operatorname* { m i n } \{ \beta \colon y \in R ( \beta + 1 ) \}$ for every $y \in x$ . Such a function exists by the axiom of replacement. Let $\textstyle \gamma = \bigcup _ { u \in x } r ( y )$ . Then $\gamma$ is an ordinal number and $x \subset R ( \gamma )$ . So $x \in \mathcal { P } ( R ( \gamma ) ) { \overset { } { = } } R ( \gamma + 1 )$ 

Now, to obtain a contradiction, assume that there exists an x such that $x \not \in R ( \alpha )$ for every ordinal number α. So, by (G), there exists a $y \in x$ such that $y \not \in R ( \alpha )$ for every ordinal number α. In particular, the set 

$$
A = \{y \in \operatorname{trcl} (x) \colon y \not \in R (\alpha) \text {   for   every   ordinal   number   } \alpha \}
$$

is not empty. So, by the axiom of regularity, A contains an ∈-minimal element, that is, there exists an $x _ { 0 } \in A$ such that $A \cap x _ { 0 } = \emptyset$ . But $x _ { 0 } \in$ $A \subset \operatorname { t r c l } ( x )$ . Hence $x _ { 0 } \subset \mathop { \mathrm { t r c l } } ( x )$ , since trcl(x) is transitive. Therefore $x _ { 0 }$ satisfies the assumption of (G) so $x _ { 0 } \in R ( \alpha _ { 0 } )$ for some ordinal number $\alpha _ { 0 }$ But this contradicts $x _ { 0 } \in A$  

For a set x define the rank of x by 

$$
\operatorname{rank} (x) = \min \{\beta : x \in R (\beta + 1) \}.
$$

Notice that by Lemma 9.1.2 rank(x) is defined for every set x. 

## Lemma 9.1.3

(a) rank(x) < α if and only if $x \in R ( \alpha )$ 

(b) If x ∈ y then rank(x) < rank(y). 

Proof (a) This is obvious by (9.1) and the definition of rank(x). 

(b) If $\beta = \operatorname { r a n k } ( y )$ then $y \in R ( \beta + 1 ) = \mathcal { P } ( R ( \beta ) ) . \mathrm { S o } \ x \in y \subset R ( \beta )$ Therefore rank $( x ) < \beta = \operatorname { r a n k } ( y )$  

Before we describe the forcing method, we will reexamine some notions discussed in Sections 1.1 and 1.2. This should give us a better understanding of what we mean when we say that a property is “independent of ZFC.” 

In what follows the term “formula” will always be understood as a formula of the language of set theory, that is, the language described in Section 1.2. In particular, the set of all formulas is defined by induction on their length from only two basic kinds of formula: $^ { 6 } x \in y ^ { \mathfrak { N } }$ and ${ } ^ { \ast } x = y , { } ^ { \ast }$ where symbols x and $y$ represent variables. A more complicated formula can be built from the less complicated formulas $\varphi$ and $\psi$ only by connecting them with logical connectors, $\varphi \& \psi , \varphi \vee \psi , \varphi { \longrightarrow } \psi , \varphi {  } \psi .$ , or by preceding one of them with the negation, $\neg \varphi .$ , or a quantifier, ∃xϕ, ∀xϕ. For example, ${ } ^ { \mathrm { ~ c ~ } } x = y \mathrm { ~ } \& \mathrm { ~ } \exists x \ \forall y \ ( x \in y ) ^ { \mathfrak { N } }$ is a correct formula, whereas expressions such as ${ } ^ { \mathfrak { a } } x \in y \in z ^ { ; ; } \ \mathrm { o r } \ { } ^ { \mathfrak { a } } z = t \vee c ^ { ; }$ are not. (Although $^ { \mathfrak { s } } x \in y \in z ^ { \mathfrak { s } }$ could be interpreted as ${ } ^ { \mathfrak { a } } x \in y \ \& \ y \in z , { \mathfrak { , } }$ the latter being a correct formula.) 

A variable in a formula is any symbol that represents a set. More precisely, it is any symbol that is neither of the following: ${ } ^ { 6 6 } \in \mathcal { V } \quad { } ^ { 6 6 } = \ '$ ${ { \stackrel { \scriptscriptstyle } { \alpha } } } _ {  } , \quad { \stackrel { \scriptscriptstyle } { \alpha } } \& _ { , } , \quad { \stackrel { \scriptscriptstyle } { \alpha } } _ { \bigvee } , \quad { \stackrel { \scriptscriptstyle } { \alpha } } _ { \bigm }  , { { \stackrel { \scriptscriptstyle } { \alpha } } } _ { \bigm }  , { { \stackrel { \scriptscriptstyle } { \alpha } } } _ { \bigm } { , } \quad { \stackrel { \scriptscriptstyle } { \alpha } } _ { \bigm } \forall , \quad { \stackrel { \scriptscriptstyle } { \alpha } } _ { \bigm } ( { \mathstrut } , { \mathstrut } _ { \mathrm { ~ o r ~ } } { \mathstrut } ^ { \mathrm { ~ \scriptscriptstyle } } { \mathstrut } ) .$ ” In a given formula not all variables must be alike. For example, in the formula $\varphi$ defined as ${ } ^ {  } x = y \ \& \ \exists z \ ( z = z ) { \mathrm { } } ^ { , }$ the variables $x$ and $y$ are parameters and $\varphi$ might be either true or false, depending on what value we associate with x and y. On the other hand, the variable z lies within the scope of the quantifier $^ { 6 6 } \exists ^ { 9 }$ and is not a parameter. 

The variables of a formula $\varphi$ that are within the scope of a quantifier are said to be bound in $\varphi$ . The parameters of a formula will be referred to as free variables. Notice that the same symbol in the same formula may be used both as a bound variable and as a free variable. For example, this is the case in the formula $\begin{array} { r } { \mathfrak { U } \overset { } { \le } x ( x \in y ) \ \& \ x = y , , \mathfrak { P } } \end{array}$ where the first $x$ is bound, while the second plays the role of a free variable. (Notice the importance of the distribution of parentheses.) 

Formulas without free variables are called sentences. Since all variables in a sentence are bound, no interpretation of free variables is necessary to decide whether it is true or false. For this reason only sentences will be used as axioms. On the other hand, if $x _ { 1 } , \ldots , x _ { n }$ are free variables of a formula $\varphi _ { : }$ , we often write $\varphi ( x _ { 1 } , \ldots , x _ { n } )$ instead of $\varphi$ to emphasize its dependence on $x _ { 1 } , \ldots , x _ { n }$ . In particular, we will usually write $\exists x \varphi ( x )$ and $\forall x \varphi ( x )$ in place of ∃xϕ and ∀xϕ. 

By a theory we will mean any set of sentences. The sentences belonging to a theory T will be treated as its axioms.<sup>2</sup> In particular, ZFC is a theory, and it consists of infinitely many axioms since each of the scheme axioms (comprehension or replacement) stands for infinitely many axioms. 

We say that a sentence $\varphi$ is a consequence of a theory $T$ (or that $\varphi$ can be proved in a theory $T )$ and write it as $T \vdash \varphi$ if there is a formal proof of $\varphi$ using as axioms only sentences from T. It is also equivalent to the fact that there exists a finite set $T _ { 0 } = \{ \psi _ { 0 } , . . . , \psi _ { n } \}$ of axioms from $T$ such that $( \psi _ { 0 } \& \cdot \cdot \cdot \& \psi _ { n } ) { \longrightarrow } \varphi$ is a consequence of axioms of logic. (See Appendix B for more details.) 

A theory $T$ is said to be inconsistent if there is a sentence $\varphi$ such that $T \vdash ( \varphi \& \lnot \varphi )$ , that is, if it leads to a contradiction. Equivalently, T is inconsistent if every sentence $\psi$ is a consequence of $T$ . (The equivalence follows from the fact that the implication $( \varphi \& \to \varphi ) \to \psi$ is true for all formulas $\varphi$ and $\psi . )$ Conversely, we say that a theory $T$ is consistent and write Con(T) if $T$ is not inconsistent, that is, if $T$ does not imply a contradiction. A sentence $^ { 6 \ell } \psi ^ { \mathrm { , } \ell }$ is consistent with theory $T$ if $T + { } ^ { * } \psi ^ { * }$ is consistent. 

Evidently, from the point of view that theories should carry useful information, only consistent ones are interesting. In particular, we will be assuming here that ZFC is consistent. (Recall that by the G¨odel’s second incompleteness theorem, Theorem 1.1.1, there is no hope of proving the consistency of ZFC in itself as long as it is really consistent.) 

The relation between the notions of “being a consequence of a theory” and “being consistent with a theory” is best captured by the following fact, whose easy proof is left as an exercise: 

$$
T \not \vdash \varphi \text { if   and   only   if } \operatorname{Con} (T + ` ` \neg \varphi).\tag{9.2}
$$

Recall also that a sentence $\varphi$ is independent of theory T if neither $T \vdash \varphi$ nor $T \vdash \lnot \varphi$ or, equivalently, when both theories $T + { } ^ { 6 } \varphi ^ { , }$ and $T + \Sigma {  } $ are consistent. Thus G¨odel’s first incompleteness theorem, Theorem 1.1.2, implies that there are sentences of set theory that are independent of $\mathrm { Z F C }$ 

The forcing method will be a tool to show that a given sentence $\psi$ is consistent with ZFC. So, in order to prove that a sentence ψ is independent of ZFC, we will be proving that the theories $\mathrm { Z F C + } ^ { \mathrm { a } } \psi ^ { \mathrm { ? } }$ and $\mathrm { Z F C + } ^ { \cdots } \lnot \psi ^ { \gamma }$ are both consistent. 

## EXERCISES

1 Complete the details of the proof of Lemma 9.1.1 by showing the mini mality of trcl(x). 

2 Prove (9.1). 

3 Prove (9.2). Hint: Use the fact that $( T \cup \{ \varphi \} ) \vdash \psi$ if and only if $T \vdash ( \varphi {  } \psi )$ 

## 9.2 Forcing method and a model for ¬CH

Consider a transitive set M. For every formula ψ of the language of set theory (without any shortcuts) we define a formula $\psi ^ { M }$ , called its relativization to M. It is obtained by replacing in $\psi$ each unbounded quantifier ∀x or ∃x with its bounded counterpart $\forall x \in M$ or $\exists x \in M$ . For example, if $\psi _ { 0 }$ is a sentence from the axiom of extensionality 

$$
\forall x \forall y [ \forall z (z \in x \leftrightarrow z \in y) \rightarrow x = y ]
$$

then $\psi _ { 0 } ^ { M }$ stands for 

$$
\forall x \in M \forall y \in M [ \forall z \in M (z \in x \leftrightarrow z \in y) \rightarrow x = y ].
$$

In particular, if $\psi ( x _ { 1 } , \dots , x _ { n } )$ is a formula with free variables $x _ { 1 } , \ldots , x _ { n }$ and $t _ { 1 } , \ldots , t _ { n } \ \in \ M$ then $\psi ^ { M } ( t _ { 1 } , \dots , t _ { n } )$ says that $\psi ( t _ { 1 } , \dots , t _ { n } )$ is true under the interpretation that all variables under quantifiers are bound to M. In other words, $\psi ^ { M } ( t _ { 1 } , \dots , t _ { n } )$ represents the formula $\psi ( t _ { 1 } , \dots , t _ { n } )$ as seen by a “person living inside $M , ^ { \ast }$ that is, thinking that M represents the entire class of all sets. (This is the best way to think of $\psi ^ { M } . )$ 

For a transitive set M and a formula $\psi$ (with possible parameters from M) we say that ${ } ^ { * } \psi$ is true in $M ^ { s }$ and write $M \models \psi$ if $\psi ^ { M }$ is true. For a theory $T$ we say that $^ { 6 6 } T$ is true in $M ^ { s }$ or that $^ { 6 } M$ is a model for $T ^ { s }$ if $\psi ^ { M }$ holds for every $\psi$ from T. 

Note that a model for a theory T is just a set satisfying some properties.<sup>3</sup> Thus, if M is the empty set, then M is a model for the theory $T$ consisting of all the axioms of ZFC except the set existence and the infinity axioms. This is so since any other axiom starts with a general quantifier $\forall x .$ , and its relativization to $M = \emptyset$ starts with $\forall x \in \varnothing$ , that is, is satisfied vacuously. Similarly, if M is any transitive set, then the axiom of extensionality is satisfied in M, since for any set $x \in M$ 

$$
z \in x \text { if   and   only   if } z \in M \& z \in x.
$$

It is also relatively easy to see that $M = R ( \omega )$ is a model for ZFC minus the infinity axiom (see Exercise 1). 

Forcing consistency proofs will be based on the following fundamental principle. 

Forcing principle In order to prove that the consistency of ZFC implies the consistency of $\mathrm { Z F C + } ^ { \mathrm { a } } \psi ^ { \mathrm { ? } }$ it is enough to show (in ZFC) that 

(F) every countable transitive model M of ZFC can be extended to a countable transitive model N of ${ \mathrm { Z F C + } } ^ { \psi } \psi .$ 

We use here the word “extend” in the sense of inclusion, that is, N extends M means that $M \subset N$ 

In what follows we will use the letters CTM as an abbreviation for “countable transitive model.” Thus the forcing principle asserts that if we can prove in ZFC the implication 

[∃M(M is a CTM for $\mathrm { Z F C } ) ] { \Rightarrow } [ \exists N ( M \subset N \& N$ is a CTM for $\mathrm { Z F C + } ^ { \alpha } \psi ^ { \prime \prime } ) ]$ 

then we can conclude from it that $\mathrm { C o n } ( Z F C )$ implies Con $( Z F C + ^ { \mathfrak { c } } \psi ^ { \mathfrak { n } } )$ 

We will not prove the forcing principle here, since its proof is not important for the applications of the forcing method. However, a sketch of its proof can be found in Appendix B. 

To use the forcing principle we will assume that we have a countable transitive model M of ZFC and then will extend it to an appropriate model N. To describe the extension method we need a few more definitions. Let M be an arbitrary family of sets and let $\mathbb { P }$ be a partially ordered set. A filter $G$ in $\mathbb { P }$ is M-generic if $D \cap G \neq \emptyset$ for every dense subset D of P that belongs to M. Notice that the Rasiowa–Sikorski lemma (Theorem 8.1.2) immediately implies the following lemma since the family $\{ D \in M \colon D \subset \mathbb { P } \ \& \ D$ is dense in P} is countable for any countable set M. 

Lemma 9.2.1 For every partially ordered set $\mathbb { P } , p \in \mathbb { P }$ , and countable set M there exists an M-generic filter G in $\mathbb { P }$ such that $p \in G$ 

The model N from (F) will be constructed by using the following theorem. 

Theorem 9.2.2 For any countable transitive model M of $Z F C ,$ , partially ordered set $\mathbb { P } = \langle \mathbb { P } _ { 0 } , \underline { { < } } \rangle \in M$ , and M-generic filter G in P there exists a smallest countable transitive model N of $Z F C$ such that $M \subset N$ and $G \in N$ 

The model N from Theorem 9.2.2 is usually denoted by $M [ G ]$ and is called a generic extension of M. We will also refer to M as the ground model of $M [ G ]$ 

Before we present a construction of $M [ G ]$ we will have a closer look at Theorem 9.2.2. To make good use of it we must expect that a countable transitive model M for some property ψ (such as CH) can be extended to a model $M [ G ]$ of its negation ¬ψ. For this, $M [ G ]$ must be a proper extension of M. However, Theorem 9.2.2 does not rule out that $M [ G ] = M$ . In fact, if $G \in M$ then clearly $M [ G ] = M$ . Fortunately, the extension will be proper for a large class of partially ordered sets described in Proposition 9.2.3. 

Proposition 9.2.3 Let M be a transitive model of ZFC and let $\mathbb { P } \in M$ be a partially ordered set such that 

(G) for every $p \in \mathbb { P }$ there are two incompatible $q , r \in \mathbb { P }$ below p. 

If G is an M-generic filter in P then $G \notin M$ 

Proof Notice that (G) implies that $D = \mathbb { P } \backslash G$ is dense in P. Now if $D \in M$ then, by the definition of an M-generic filter, we would have $G \cap D \neq \emptyset$ , which is impossible, since $G \cap D = G \cap ( \mathbb { P } \setminus G ) = \emptyset$ . So $D \not \in M$ . But $\mathbb { P } \in M$ and M is closed under taking the diference of two sets, since it is a model of ZFC. Therefore $G \notin M$ , since otherwise $D = \mathbb { P } \setminus G \in M$  

Without any doubt the reader should notice a similarity between Martin’s axiom and the statement of Theorem 9.2.2. In fact, the generic filter G from the theorem will be used in $M [ G ]$ in a way similar to the way we used generic filters in the proofs where Martin’s axiom was used. To see the similarities as well as diferences between such uses in both cases consider the following example. 

Example 9.1 Let M be a countable transitive model of ZFC. For sets X and Y from M consider the forcing $\mathbb { P } ( X , Y ) = \langle \mathrm { F u n c } _ { \omega } ( X , Y ) , \supset \rangle$ . Then $\mathbb { P } ( X , Y )$ belongs to M, being defined from $X , Y \in M$ . It is easy to see that if X is infinite then the sets 

$$
D _ {x} = \{p \in \mathbb {P} (X, Y) \colon x \in \operatorname{dom} (p) \} \text { for } x \in X
$$

and 

$$
R _ {y} = \{p \in \mathbb {P} (X, Y) \colon y \in \mathrm{range} (p) \} \text { for } y \in Y
$$

are dense in $\mathbb { P } ( X , Y )$ . They belong to M, since each of them is defined from $\mathbb { P } ( X , Y )$ and either $x \in X \subset M$ or $y \in Y \subset M$ . In particular, if $G$ is an M-generic filter in $\mathbb { P } ( X , Y )$ then, by Proposition 8.1.1, $g = \bigcup G$ is a function from X onto $Y$ 

In the proof that ¬CH is consistent with ZFC we will use the forcing ${ \mathbb P } _ { 0 } = { \mathbb P } ( \omega _ { 2 } \times \omega , 2 )$ . Then, for an M-generic filter $G _ { 0 }$ in $\mathbb { P } _ { 0 }$ , we see that $g = \bigcup G _ { 0 } \colon \omega _ { 2 } \times \omega  2$ belongs to $M [ G _ { 0 } ]$ . Moreover, notice that for every $\zeta < \xi < \omega _ { 2 }$ the sets 

$$
E _ {\zeta} ^ {\xi} = \left\{p \in \mathbb {P} _ {0}: \exists n <   \omega [ \langle \zeta , n \rangle , \langle \xi , n \rangle \in \operatorname{dom} (p) \& p (\zeta , n) \neq p (\xi , n) ] \right\}
$$

are dense in $\mathbb { P } _ { 0 }$ and belong to M. Thus an M-generic filter intersects every such set, that is, 

for every $\zeta < \xi < \omega _ { 2 }$ there exists an $n < \omega$ such that $g ( \zeta , n ) \neq g ( \xi , n )$ . (9.3) 

Now for every $\xi < \omega _ { 2 }$ we can define a function $g _ { \xi } \colon \omega  2$ by $g _ { \xi } ( n ) = g ( \xi , n )$ The set $\{ g _ { \xi } \colon \xi \ < \ \omega _ { 2 } \}$ belongs to $M [ G ]$ , since it has been defined only from $g ~ \in ~ M [ G ]$ Moreover, by (9.3), all functions $g _ { \xi }$ are distinct and $\{ g _ { \xi } \colon \xi < \omega _ { 2 } \} \subset 2 ^ { \omega }$ . So we have proved that (in $M [ \bar { G } _ { 0 } ] )$ the family $2 ^ { \omega }$ contains a subset $\{ g _ { \xi } \colon \xi < \omega _ { 2 } \}$ of cardinality $\omega _ { 2 }$ , so ${ \mathfrak { c } } = | 2 ^ { \omega } | \geq \omega _ { 2 } > \omega _ { 1 }$ That is, in $M [ G _ { 0 } ]$ the continuum hypothesis is false. 

Is this really all we need to prove? Is it that simple? Unfortunately the preceding argument contains several imprecisions and gaps. To see this let us consider another forcing $\mathbb { P } ^ { \star } = \mathbb { P } ( \omega , \omega _ { 1 } ) = \langle \mathrm { F u n c } _ { \omega } ( \omega , \omega _ { 1 } ) , \supset \rangle$ and let $G ^ { \star }$ be an M-generic filter in $\mathbb { P } ^ { \star }$ . Then, as we noticed before, $g = \bigcup G ^ { \star }$ is a function from $\omega$ onto $\omega _ { 1 } !$ This looks like a clear contradiction. What is wrong? Is Theorem 9.2.2 false? 

The answer is that there is nothing wrong with Theorem 9.2.2. What is wrong with our “contradiction” is that there is a misconception of what the theorem really says. It tells us that $M [ G ]$ is a model for ZFC as long as M is such a model. In particular, $\varphi ^ { M }$ and $\varphi ^ { M [ G ] }$ are true for every sentence $\varphi$ that is a consequence of ZFC axioms. However, the constants are not a part of the formal language of set theory, and we use them only as shortcuts for the formulas representing them. Thus we write $^ { 6 6 } x$ is equal to $\omega _ { 1 } { } ^ { \mathfrak { I } }$ to express the fact that x is the unique set satisfying the formula $\varphi ( x ) : \quad { } ^ { \mathfrak { a } } x$ is the smallest uncountable ordinal number.” Theorem 9.2.2 tells us that the sentence $\psi$ defined by ∃!x $\varphi ( x )$ is true both in M and in $M [ G ]$ , since the existence of a unique $\omega _ { 1 }$ can be proved in ZFC. Thus $\psi ^ { N }$ holds for $N = M$ or $N = M [ G ]$ , and there exists a unique $\omega _ { 1 } ^ { N } \in N$ such that $\varphi ^ { N } ( \omega _ { 1 } ^ { N } )$ is true, that is, that $\omega _ { 1 } ^ { N }$ is an $^ { 6 6 } \omega _ { 1 }$ with respect to $N . ^ { \mathfrak { s } }$ However, Theorem 9.2.2 does not tell us that $\omega _ { 1 } ^ { M } = \omega _ { 1 } ^ { M [ G ] } !$ In fact, since $M$ is countable and transitive, every element of M is countable. Thus by manipulating M from outside we may be able to take any set $x \in M$ that is uncountable in M and find a generic extension $M [ G ]$ of M in which x is countable. And this is precisely what happened in $M [ G ^ { \star } ] !$ The ordinal number $\omega _ { 1 } ^ { M }$ became a countable object in $M [ G ^ { \star } ]$ , and $\omega _ { 1 } ^ { M }$ is not equal to $\omega _ { 1 } ^ { M [ G ^ { \star } ] }$ . (The argument that indeed $\omega _ { 1 } ^ { M } \neq \dot { \omega _ { 1 } ^ { M [ G ^ { \star } ] } }$ will be completed after Lemma 9.2.5.) 

In fact, so far we are not even sure whether what is an ordinal number in M remains so in $M [ G ]$ , or even whether what is 2 in M remains 2 in $M [ G ]$ . To address this issue we have to examine our set-theoretic vocabulary more carefully. In particular, the general question we would like to examine is, Which properties of elements of $M$ are preserved in its extension $M [ G ] \ ?$ (This can be viewed as an analog of the preservation problems for transfinite-induction constructions discussed in Section 6.1.) 

To address this issue recall once more that every set-theoretic term we use can be expressed by a formula of set theory. So the question may be rephrased as follows: 

For which properties $P$ does there exist a formula $\psi ( x _ { 1 } , \dots , x _ { n } )$ 

describing P such that if $\psi ( t _ { 1 } , \dots , t _ { n } )$ is true in M for some 

$t _ { 1 } , \ldots , t _ { n } \in M$ then $\psi ( t _ { 1 } , \dots , t _ { n } )$ is also true in $M [ G ] ?$ 

The properties that are always preserved in such extensions will be called absolute properties. More precisely, a property is absolute provided it can be expressed by a formula $\psi ( x _ { 1 } , \dots , x _ { n } )$ such that for every transitive models M and N of ZFC with $M \subset N$ and for every $t _ { 1 } , \ldots , t _ { n } \in M$ formula $\psi ^ { M } ( t _ { 1 } , \dots , t _ { n } )$ holds if and only if $\psi ^ { N } ( t _ { 1 } , \dots , t _ { n } )$ holds. 

The absoluteness of most properties we are interested in follows just from the fact that the models we consider are transitive. To identify a large class of such properties we need the following notion. A formula $\psi$ is a $\Delta _ { 0 } { \mathrm { - } } f o r m u l a$ if it can be written such that the only quantifiers it contains are bounded quantifiers, that is, quantifiers of the form $\exists x \in y$ or $\forall x \in y$ 

Lemma 9.2.4 Let M be a transitive set and let $\psi ( x _ { 1 } , \dots , x _ { n } )$ be a $\Delta _ { 0 } -$ formula. If $t _ { 1 } , \ldots , t _ { n } \in M$ then $\psi ^ { M } ( t _ { 1 } , \ldots , t _ { n } )$ is equivalent to $\psi ( t _ { 1 } , \dots , t _ { n } )$ in the sense that the sentence 

$\forall M [ M$ is transitive $\right. ( \forall t _ { 1 } , \dots , t _ { n } \in M ) ( \psi ^ { M } ( t _ { 1 } , \dots , t _ { n } ) \left. \psi ( t _ { 1 } , \dots , t _ { n } ) ) ]$ 

is provable in ZFC. In particular, the property expressed by ψ is absolute. 

Proof The proof goes by induction on the length of formula $\psi$ . 

Clearly it is true for any basic formula $x \in y { \mathrm { ~ o r ~ } } x = y .$ , since for any quantifier-free formula $\psi$ its relativization $\psi ^ { M }$ is identical to $\psi$ 

So assume that formula $\psi$ is built from the less complicated formulas $\varphi _ { 0 }$ and $\varphi _ { 1 }$ , that is, $\psi$ is in one of the following forms: $\varphi _ { 0 } \& \varphi _ { 1 } , \ \varphi _ { 0 } \vee \varphi _ { 1 }$ , $\varphi _ { 0 } \longrightarrow \varphi _ { 1 } , \varphi _ { 0 }  \varphi _ { 1 } , \lnot \varphi _ { 0 } , \exists x \in t \ \varphi _ { 0 }$ , or $\forall x \in t \varphi _ { 0 }$ . For example, if $\psi = \varphi _ { 1 } \vee \varphi _ { 2 }$ and the lemma is true for all formulas of length less than the length of $\psi .$ then it holds for $\varphi _ { 0 }$ and $\varphi _ { 1 }$ . In particular, 

$$
\psi^ {M} = (\varphi_ {0} \vee \varphi_ {1}) ^ {M} = \varphi_ {0} ^ {M} \vee \varphi_ {1} ^ {M} = \varphi_ {0} \vee \varphi_ {1} = \psi .
$$

We argue similarly if $\psi$ is the negation of a formula, or is obtained from two formulas by using the logical operations $\& , \to , \mathrm { o r } $ 

If $\psi$ is of the form $\exists x \in t \varphi _ { 0 } ( x )$ for some $t \in M$ then its formal representation is $\exists x [ x \in t \& \varphi _ { 0 } ( x ) ]$ . Then $\psi ^ { M }$ stands for $\exists x \in M \ [ x \in t \ \& \ \varphi _ { 0 } ^ { M } ( x ) ]$ which is equivalent to $( \exists x \in t \cap M ) \varphi _ { 0 } ( x )$ since $\varphi _ { 0 } ( x )$ is equivalent to $\varphi _ { 0 } ^ { M } ( x )$ by the inductive assumption. But $t \in M$ and M is transitive. So $t \subset M$ and $t \cap M = t$ . Therefore $\psi ^ { M }$ is equivalent to $\exists x \in t \varphi _ { 0 } ( x )$ , that is, to $\psi .$ 

The case when $\psi$ is of the form ∀x $\in t \varphi _ { 0 } ( x )$ is similar. 

For example, the property $^ { \circ } y$ is a union of $x , ^ { \prime \prime } \ y = \bigcup x$ , is absolute, since it can be written as the following $\Delta _ { \mathrm { 0 } } \mathrm { - f o r m u l a }$ $\psi _ { 1 } ( x , y )$ 

$$
\forall w \in y \exists z \in x (w \in z) \& \forall z \in x \forall w \in z (w \in y).
$$

Lemma 9.2.5 The following properties can be expressed by a $\Delta _ { 0 } { \mathrm { - } } f o r m u l a .$ In particular, they are absolute. 

(0) $x \subset y .$ 

(1) $y = \cup x .$ 

(2) $y = \bigcap x .$ 

(3) $z = x \cup y .$ 

(4) $z = x \cap y .$ 

(5) $z = x \setminus y .$ 

(6) $z = \{ x , y \}$ 

(7) z is an unordered pair. 

(8) $z = \langle x , y \rangle \ ( i . e . , \ z = \{ \{ x \} , \{ x , y \} \} ) .$ 

(9) z is an ordered pair. 

(10) $z = x \times y .$ 

(11) r is a binary relation. 

(12) d is the domain of binary relation $r .$ 

(13) R is the range of binary relation $r$ . 

(14) f is a function. 

(15) Function f is injective. 

(16) $\leq \ i s$ a partial-order relation on $\mathbb { P } \ ( i . e . , \langle \mathbb { P } , \leq \rangle$ is a partially ordered $s e t )$ 

(17) D is a dense subset of the partially ordered set $\langle \mathbb { P } , \leq \rangle$ 

(18) A is an antichain in the partially ordered set $\langle \mathbb { P } , \leq \rangle$ 

(19) Set x is transitive. 

(20) α is an ordinal number. 

(21) α is a limit ordinal number. 

(22) α is the first nonzero limit ordinal number $( i . e . , \alpha = \omega )$ 

(23) α is a finite ordinal number. 

(24) α is a successor ordinal number. 

Proof The $\Delta _ { \mathrm { 0 } } { \mathrm { - f o r m u l } }$ as for these properties can be found in Appendix B.  

Now, for a property $P$ expressed by a formula $\psi ( x )$ , a transitive model M of $\mathrm { Z F C , }$ and $t \in M$ the statement $^ { 6 6 } t$ has the property $P ^ { \ast }$ may be interpreted in two diferent ways: as either that t satisfies the formula $\psi ( x )$ , that is, that $\psi ( t )$ holds, or that $\psi ( x )$ is satisfied by t in $M .$ , that is, that $\psi ^ { M } ( t )$ is true. In the latter case we will say that $^ { 6 6 } t$ has the property $P$ in $M$ ,” reserving the statement $^ { 6 6 } t$ has the property $P ^ { \prime }$ for the former case. However, for the absolute properties, such as $^ { 6 6 } \alpha$ is an ordinal number,” such a distinction is redundant. Thus, we will say $^ { 6 } \alpha$ is an ordinal number” independently of whether we think of α as an ordinal number in M or outside it. 

A similar distinction has to be made when we talk about constants. When we write $\omega$ we think of it as $^ { 6 6 } \omega$ is the first infinite ordinal number.” In principle, an object $\omega ^ { M }$ that satisfies this property in $M$ might be diferent from the “real” $\omega .$ . However, for objects represented by absolute formulas this cannot happen. So in all these cases we will drop the superscript <sup>M</sup> from the symbol representing an absolute constant, even when we think of it as being “in $M . ^ { \mathfrak { s } }$ In particular, we will use the same symbol $\omega$ regardless of the context, since $\omega ^ { M } = \omega$ . For the cases of the constants that are not absolute, such as $\omega _ { 1 }$ or c, we will keep using the superscript <sup>M</sup> to denote $M$ their counterparts in M. For example, we will write $\omega _ { 1 } ^ { M }$ and ${ \mathfrak { c } } ^ { M }$ to express $\omega _ { 1 }$ and c in M. 

In fact, we have already used this convention when arguing that $\omega _ { 1 } ^ { M } \neq $ $\omega _ { 1 } ^ { M [ G ^ { \star } ] }$ , with $G ^ { \star }$ being an M-generic filter in $\mathbb { P } ^ { \star } = \langle \mathrm { F u n c } _ { \omega } ( \omega , \omega _ { 1 } ) , \supset \rangle$ . And now we can indeed see that $\omega _ { 1 } ^ { \bar { M } } \neq \omega _ { 1 } ^ { M [ G ^ { \star } ] }$ . This is so since $\omega _ { 1 } ^ { M }$ and $\dot { \omega } _ { 1 } ^ { M [ G ^ { \star } ] }$ are (real) ordinal numbers, and in $M [ G ^ { \star } ]$ there is a (real) function f from (true) $\omega$ onto $\omega _ { 1 } ^ { M }$ . So $\omega _ { 1 } ^ { M }$ is a countable ordinal in $M [ G ^ { \star } ]$ , whereas $\dot { \omega } _ { 1 } ^ { M [ G ^ { \star } ] }$ is an uncountable ordinal in $M [ G ^ { \star } ]$ by its definition. Thus they cannot be equal. 

Proof of Theorem 9.2.2 To construct the set $M [ G ]$ fix a countable transitive model M of ZFC, a partially ordered set $\mathbb { P } \in M$ , and an M-generic filter G in P. 

We say that $\tau$ is a P-name provided $\tau$ is a binary relation and 

$$
\forall \langle \sigma , p \rangle \in \tau (\sigma \text {   is   a   } \mathbb {P} \text {-name   \&   } p \in \mathbb {P}).
$$

Formally, we define the property $^ { 6 6 } \tau$ is a $\mathbb { P } { \mathrm { - n a m e } } ^ { \prime }$ recursively by induction on rank(τ). Thus $\tau$ is a P-name if it satisfies the following recursive formula: 

$\psi ( \tau )$ : there exists an ordinal number α and a function f such that dom $( f ) =$ $\alpha + 1 , f ( \alpha ) = \{ \tau \}$ , and for every $\beta \in \alpha + 1 , t \in f ( \beta )$ , and $z \in t$ there exist $\gamma \in \beta , \sigma \in f ( \gamma )$ , and $p \in \mathbb { P }$ such that $z = \langle \sigma , p \rangle$ 

It is not dificult to see that $\psi$ is absolute (see Exercise 2). So the property $^ { 6 6 } \tau$ is a P-name” is absolute too. 

The set of all P-names that belong to M will be denoted by $M ^ { \mathbb { P } }$ , that is, 

$$
M ^ {\mathbb {P}} = \{\tau \in M: \tau \text {is a} \mathbb {P} \text {-name} \}.
$$

It can be proved that the class of all P-names is a proper class. Thus $M ^ { \mathbb { P } }$ is a proper class in M. It particular, it does not belong to $M$ 

For a P-name $\tau$ we define the valuation of $\tau$ by 

$$
\operatorname{val} _ {G} (\tau) = \{\operatorname{val} _ {G} (\sigma) \colon \exists p \in G (\langle \sigma , p \rangle \in \tau) \}.
$$

Once again, the formal definition of $\mathrm { v a l } _ { G } ( \tau )$ should be given by a recursive formula. Now we define $M [ G ]$ by 

$$
M [ G ] = \{\mathrm{val} _ {G} (\tau) \colon \tau \in M ^ {\mathbb {P}} \}.
$$

This is the model from the statement of Theorem 9.2.2. 

We will not check here that all ZFC axioms are true in $M [ G ]$ , since it is tedious work and has little to do with the forcing applications. However, we will argue here for its other properties listed in Theorem 9.2.2. 

Transitivity of $M [ G ]$ follows immediately from the definition of $M [ G ]$ Take $y \in M [ G ]$ . Thus $y = \mathrm { v a l } _ { G } ( \tau ) = \{ \mathrm { v a l } _ { G } ( \sigma ) \colon \exists p \in G \ ( \langle \sigma , p \rangle \in \tau ) \}$ for some $\tau \in M ^ { \mathbb { P } }$ . So any $x \in y$ is in the form val (σ) for some $\langle \sigma , p \rangle \in \tau \in M$ Thus σ is a P-name that belongs to M, and $x = \operatorname { v a l } _ { G } ( \sigma ) \in M [ G ]$ 

The minimality of $M [ G ]$ is clear, since every element of M[G] is of the form $\mathrm { v a l } _ { G } ( \tau )$ and so must belong to any transitive model of ZFC that contains G and τ. 

To see that $M [ G ]$ is countable notice first that it is a set by the axiom of replacement since val is a function defined by a formula and $M [ G ] =$ $\mathrm { v a l } _ { G } [ M ^ { \mathbb { P } } ]$ . It is countable, since $M ^ { \mathbb { P } } \subset M$ is countable. 

To argue for $M \subset M [ G ]$ and $G \in M [ G ]$ we need a few more definitions. For a set x define, by recursion, its P-name ˆx by 

$$
\hat {x} = \{\langle \hat {y}, p \rangle : y \in x \& p \in \mathbb {P} \}.
$$

(Note that the definition of ˆx depends on P.) 

Lemma 9.2.6 If M is a countable transitive model of $Z F C , \ \mathbb { P } \in M$ is a partially ordered set, and G is an M-generic filter over P then for every $x \in M$ 

$$
\hat {x} \in M ^ {\mathbb {P}} a n d \operatorname{val} _ {G} (\hat {x}) = x.
$$

In particular, $M \subset M [ G ]$ 

Proof It is an easy inductive argument. First prove by induction on rank(x) that ˆx is a P-name. Then notice that the definition of ˆx is absolute and $x \in M$ . So ${ \hat { x } } \in M$ . Finally, another induction on rank(x) shows that $\operatorname { v a l } _ { G } ( { \hat { x } } ) = x$ . The details are left as an exercise.  

To see that $G \in M [ G ]$ let $\Gamma = \{ \langle \hat { p } , p \rangle \colon p \in \mathbb { P } \}$ . It is clearly a P-name defined in M from P. So $\dot { \Gamma } \in M ^ { \mathbb { P } }$ . Moreover, 

$$
\operatorname{val} _ {G} (\Gamma) = \left\{\operatorname{val} _ {G} (\hat {p}) \colon \exists p \in G (\langle \hat {p}, p \rangle \in \Gamma) \right\} = \left\{p \in \mathbb {P} \colon p \in G \right\} = G.
$$

So $G \in M [ G ]$ 

This finishes the proof of Theorem 9.2.2. 

The last important basic problem we have to face is how to check that a given property $\varphi$ is true in $M [ G ]$ . For this, we will introduce the following definition. For a formula $\varphi ( x _ { 1 } , \ldots , x _ { n } )$ , a countable transitive model M of ZFC, a partial order $\mathbb { P } \in M$ , and P-names $\tau _ { 1 } , \dots , \tau _ { n } \in M$ we say that $p \in \mathbb { P }$ forces $\varphi ( \tau _ { 1 } , \dots , \tau _ { n } )$ and write 

$$
p \left\| - _ {\mathbb {P}, M} \varphi (\tau_ {1}, \dots , \tau_ {n}) \right.
$$

provided $\varphi ( \operatorname { v a l } _ { G } ( \tau _ { 1 } ) , \dots , \operatorname { v a l } _ { G } ( \tau _ { n } ) )$ is true in $M [ G ]$ for every M-generic filter G in P that contains p. We will usually just write $\parallel -$ in place of $\| - _ { \mathbb { P } , M }$ when P and M are fixed. We will also write $\mathbb { P } \Vdash \varphi ( \tau _ { 1 } , \dots , \tau _ { n } )$ if $p \Vdash \varphi ( \tau _ { 1 } , \dots , \tau _ { n } )$ for every $p \in \mathbb { P }$ . Notice that 

$$
\text {   if   } p \left\| - \varphi (\tau_ {1}, \dots , \tau_ {n}) \right. \text {   and   } q \leq p \text {   then   } q \left\| - \varphi (\tau_ {1}, \dots , \tau_ {n}), \right.\tag{9.4}
$$

since every M-generic filter G that contains q contains also $p .$ 

Clearly, the definition of the relation @− depends on a model M and a set P and involves the knowledge of all M-generic filters in P. Thus, it is clearly defined outside M. One of the most important facts concerning forcing is that an equivalent form of $\Vdash$ can also be found inside M, in a sense described in the following theorem. 

Theorem 9.2.7 For every formula $\varphi ( x _ { 1 } , \ldots , x _ { n } )$ of set theory there exists another formula $\psi ( \pi , P , x _ { 1 } , \ldots , x _ { n } )$ , denoted by $\pi \Vdash _ { P } ^ { \star } \varphi ( x _ { 1 } , \ldots , x _ { n } )$ , such that for every countable transitive model M of $Z F C ,$ , partial order $\mathbb { P } \in M$ and $\mathbb { P } \mathrm { - } n a m e s \ \tau _ { 1 } , \ldots , \tau _ { n } \in M$ 

$$
p \left\| - _ {\mathbb {P}, M} \varphi (\tau_ {1}, \dots , \tau_ {n}) \Leftrightarrow M \right. \models (p \left\| - _ {\mathbb {P}} ^ {\star} \varphi (\tau_ {1}, \dots , \tau_ {n})\right)\tag{9.5}
$$

for every $p \in \mathbb { P }$ . Moreover, 

$$
M [ G ] \models \varphi (\operatorname{val} _ {G} (\tau_ {1}), \dots , \operatorname{val} _ {G} (\tau_ {n})) \Leftrightarrow \exists p \in G (p \| - \varphi (\tau_ {1}, \dots , \tau_ {n}))\tag{9.6}
$$

for every M-generic filter G in P. 

This theorem will be left without proof. 

The relation $\parallel - ^ { \star }$ from Theorem 9.2.7 will justify the use of all forcing arguments within a model M and will let us conclude all essential properties of $M [ G ]$ without knowledge of G. We will often write @− where formally the relation $\parallel - ^ { \star }$ should be used. 

This completes all general details concerning the forcing method. However, before we give a proof of $\operatorname { C o n } ( Z F C + \lnot C H )$ we still need some technical lemmas. The first of them tells us that a P-name representing a function with domain and range belonging to a ground model can be chosen to have a particularly nice form. 

Lemma 9.2.8 Let M be a countable transitive model of ZFC and $\mathbb { P } \in M$ be a partially ordered set. If $X , Y \in M , p _ { 0 } \in \mathbb { P }$ , and $\sigma \in M ^ { \mathbb { P } }$ are such that $p _ { 0 } \parallel - \tilde { \sigma }$ is a function from $\hat { X }$ into $\hat { Y } ^ { \dag }$ then there exists a $\tau \in { \cal M } ^ { \mathbb { P } }$ such that 

$$
\tau \subset \{\langle \langle x, y \rangle , p \rangle : x \in X \& y \in Y \& p \in \mathbb {P} \& p \leq p _ {0} \}; \tag {a}
$$

(b) $p _ { 0 } \parallel - \sigma = \tau ;$ and 

(c) $A _ { x } = \{ p \in \mathbb { P } \colon \exists y \in Y \ ( \langle \overline { { \langle x } } , \widehat { y \rangle } , p \rangle \in \tau ) \}$ is an antichain for every $x \in X$ 

Proof For $x \in X$ let 

$$
D _ {x} = \{p \in \mathbb {P}: p \leq p _ {0} \& \exists y \in Y (p \| - \widehat {\langle x , y \rangle} \in \sigma) \}.
$$

Notice that $D _ { x } \in M$ since, by condition (9.5) of Theorem 9.2.7, 

$$
D _ {x} = \{p \in \mathbb {P} \colon p \leq p _ {0} \& \exists y \in Y (p \| - ^ {\star} \widehat {\langle x , y \rangle} \in \sigma) ^ {M} \}.
$$

Let $\bar { A } _ { x }$ be a maximal subset of $D _ { x }$ of pairwise-incompatible elements. Thus every $\bar { A } _ { x }$ is an antichain. Define 

$$
\tau = \{\langle \langle x, y \rangle , p \rangle : x \in X \& y \in Y \& p \in \bar {A} _ {x} \& p \| - \widehat {\langle x , y \rangle} \in \sigma \}.
$$

Once again $\tau \in M$ follows from (9.5), since 

$$
\tau = \{\langle \widehat {\langle x , y \rangle}, p \rangle : x \in X \& y \in Y \& p \in \bar {A} _ {x} \& (p \| - ^ {\star} \widehat {\langle x , y \rangle} \in \sigma) ^ {M} \}
$$

and the family $\{ \bar { A } _ { x } \colon x \in X \}$ can be chosen from M. 

Clearly τ is a P-name satisfying (a). 

To see (c) it is enough to notice that $A _ { x } = \bar { A } _ { x }$ for every $x \in X$ . This is the case since 

$$
\begin{array}{r c l} p \in A _ {x} & \Leftrightarrow & \exists y \in Y \langle \widehat {\langle x , y \rangle}, p \rangle \in \tau \\ & \Leftrightarrow & \exists y \in Y (p \in \bar {A} _ {x} \& p | | - \widehat {\langle x , y \rangle} \in \sigma) \\ & \Leftrightarrow & p \in \bar {A} _ {x}. \end{array}
$$

To prove that p $\lVert - \sigma = \tau$ , let $G$ be an M-generic filter in $\mathbb { P }$ such that $p _ { 0 } \in G$ . Then $g = \mathrm { v a l } _ { G } ( \sigma )$ is a function from X into $Y _ { \textrm { : } }$ since $p _ { 0 }$ forces it. Also, clearly va $\operatorname { l } _ { G } ( \tau ) \subset X \times Y$ . So let $x \in X$ and $y \in Y$ . It is enough to show that $\langle x , y \rangle \in { \mathrm { v a l } } _ { G } ( \sigma )$ if and only if $\langle x , y \rangle \in \operatorname { v a l } _ { G } ( \tau )$ 

But if $\langle x , y \rangle \in \mathrm { v a l } _ { G } ( \tau )$ then there exists a $p \in G$ such that $\widehat { \langle x , y \rangle } , p \rangle \in \tau$ In particular, $p \Vdash \left. x , y \right. \in \sigma$ . But $p \in G$ . Therefore $\langle x , y \rangle \in { \mathrm { v a l } } _ { G } ( \sigma )$ 

To prove the other implication first note that the set 

$$
E _ {x} = \left\{q \leq p _ {0}: \exists p \in \bar {A} _ {x} (q \leq p) \right\} \cup \left\{q \in \mathbb {P}: q \text {   is   incompatible   with   } p _ {0} \right\}
$$

is dense in P. To see it, let $s \in \mathbb { P }$ . We have to find $q \in E _ { x }$ with $q \leq s$ 

If s is incompatible with $p _ { 0 }$ then $q = s \in E _ { x } . \mathrm { S o }$ assume that s is compatible with $p _ { 0 }$ and choose $p _ { 1 } \in \mathbb { P }$ extending s and $p _ { 0 }$ . Let H be an M-generic filter in P containing $p _ { 1 }$ . Then $h = \operatorname { v a l } _ { H } ( \sigma )$ is a function from X into Y since the condition $p _ { 0 } \in H$ forces it. Let $y = h ( x )$ . Then, by (9.6), there exists an $r \in H$ forcing it, that is, such that $r \parallel - \left. x , \hat { y } \right. \in \sigma$ . Choose $p _ { 2 } \in H$ extending $r \in H$ and $p _ { 1 } \in H$ . Then, by $( 9 . 4 ) , p _ { 2 } \ \Vdash \left. x , y \right. \in \sigma$ . In particular, $p _ { 2 } \in D _ { x }$ . But $\bar { A } _ { x }$ is a maximal antichain in $D _ { x }$ . So there exists $\mathrm { ~ a ~ } q \le p _ { 2 }$ extending some p from $\bar { A } _ { x }$ . Hence $q \le p _ { 2 } \le p _ { 0 }$ , so $q \in E _ { x }$ , and $q \leq p _ { 2 } \leq p _ { 1 } \leq s$ . The density of $E _ { x }$ has been proved. 

Now let $\langle x , y \rangle \in { \mathrm { v a l } } _ { G } ( \sigma )$ . Then, by (9.6), there exists an $r \in G$ that forces it, that is, such that $r \ \parallel - \ \langle \overline { { x } } , \overline { { y } } \rangle \ \in \ \sigma .$ . Moreover, there exists a $q \in E _ { x } \cap G$ , since G is M-generic and $E _ { x } \in M$ is dense. But $q \in G$ is compatible with $p _ { 0 } \in G$ . So there exists a $p \in \bar { A } _ { x } \subset D _ { x }$ with $q \leq { \underline { { p } } }$ . Thus, by the definition of $D _ { x }$ , there exists a $y _ { 1 } \in Y$ such that $p \parallel - \left. x , y _ { 1 } \right. \in \sigma$ In particular, $\langle \widehat { \langle x , y _ { 1 } \rangle } , p \rangle \in \tau$ and $\langle x , y _ { 1 } \rangle \in { \mathrm { v a l } } _ { G } ( \tau )$ , since $p \in G$ . To finish the proof it is enough to notice that $y _ { 1 } = y$ . So let $s \in G$ be a common extension of $r , p .$ and $p _ { 0 }$ . Then, by (9.4), 

$$
s \left\| - \widehat {\langle x , y \rangle} \in \sigma \& \widehat {\langle x , y _ {1} \rangle} \in \sigma \& \sigma \text {   is   a   function }\right).
$$

Therefore, if H is an M-generic filter in $\mathbb { P }$ containing s then $h = \operatorname { v a l } _ { H } ( \sigma )$ is a function and $y = h ( x ) = y _ { 1 }$  

Corollary 9.2.9 Let M be a countable transitive model of ZFC and $\mathbb { P } \in M$ be a partially ordered set that is ccc in M. Let G be an M-generic filter in P, and let $g \in M [ G ]$ be such that $g \colon X \to Y$ and $X , Y \in M$ . Then there exists a function $F \in M$ such that 

$$
M \models F \colon X \to [ Y ] ^ {\leq \omega}
$$

and $g ( x ) \in F ( x )$ for all $x \in X$ 

Proof Let $\sigma \in M$ be a P-name such that $\operatorname { v a l } _ { G } ( \sigma ) = g$ . Since 

$M [ G ] \models g$ is a function from X into $Y .$ , 

by Theorem 9.2.7(9.6) there exists a $p _ { 0 } \in G$ such that 

$p _ { 0 } \parallel - \sigma$ is a function from $\hat { X }$ into $\hat { Y }$ . 

Let $\tau \in M$ be a P-name from Lemma 9.2.8 and define 

$$
F (x) = \{y \in Y \colon \exists p ^ {y} \in \mathbb {P} (\langle \langle \langle x, y \rangle , p ^ {y} \rangle \in \tau) \}.
$$

Then clearly $F \in M$ and $M \ : \models \ F \colon X \ : \to \ : { \mathcal { P } } ( Y )$ . To see that for every $x \in X$ the set $F ( x )$ is countable in M note that the map $g \colon F ( x )  A _ { x } .$ , $g ( y ) = p ^ { y }$ , is one-to-one. 

Indeed, if $y , z \in F ( x )$ and $p ^ { y } = p ^ { z }$ then $p = p ^ { y } \leq p _ { 0 }$ and so 

$$
p \Vdash \left(\widehat {\langle x , y \rangle} \in \tau \& \widehat {\langle x , z \rangle} \in \tau \& \tau \text {   is   a   function }\right).
$$

Thus $y = z$ . In particular, 

$$
M \models | F (x) | \leq | A _ {x} | \leq \omega ,
$$

as $\mathbb { P }$ is ccc in M. Finally, since $g = \mathrm { v a l } _ { G } ( \sigma ) = \mathrm { v a l } _ { G } ( \tau )$ 

$$
y = g (x) \Leftrightarrow \exists p \in G (\langle \widehat {\langle x , y \rangle}, p \rangle \in \tau) \Rightarrow y \in F (x).
$$

Corollary 9.2.9 has been proved. 

Next we will show that ccc forcings are very nice with respect to the cardinal numbers. To formulate this more precisely we need a few definitions. 

Let M be a countable transitive model of $\mathrm { Z F C } , \mathbb { P } \in M$ be a partial order, and $\kappa \in M$ be an ordinal number such that $M \models { } ^ { \ast } \kappa$ is a cardinal number.” If $M [ G ] \models { } ^ { \mathfrak { a } } \kappa$ is a cardinal number” for every M-generic filter G in $\mathbb { P }$ then we say that forcing $\mathbb { P }$ preserves the cardinal κ. On the other hand, if $M [ G ] \models { } ^ { \mathfrak { s } } \kappa$ is not a cardinal number” for every M-generic filter G in P then we say that forcing $\mathbb { P }$ collapses the cardinal κ. If $\mathbb { P }$ preserves all cardinal numbers from M then we simply say that P preserves cardinals. 

Lemma 9.2.10 Let M be a countable transitive model of ZFC and $\mathbb { P } \in M$ be a partial order that preserves cardinals. If G is an M-generic in $\mathbb { P }$ then $\omega _ { \alpha } ^ { M } = \omega _ { \alpha } ^ { M [ G ] }$ for every ordinal number $\alpha \in M$ 

Proof This follows by an easy induction; it is left as an exercise. 

Theorem 9.2.11 Let M be a countable transitive model of ZFC. If $\mathbb { P } \in M$ is a partial order such that $M \Vdash ^ { \# } \mathbb { P }$ is ccc” then $\mathbb { P }$ preserves cardinals. 

Proof Let M and $\mathbb { P }$ be as in the theorem and assume, to obtain a contradiction, that there is an ordinal number κ and an M-generic filter $G$ in P such that κ is a cardinal in M but is not in M[G]. By the absoluteness of finite cardinals and $\omega$ it must be that $\kappa > \omega$ 

Since κ is still an ordinal in $M [ G ]$ it means that it is not initial, that is. there exist an ordinal $\alpha \ < \ \kappa$ and a function $g \in M [ G ]$ such that g maps α onto κ. So, by Corollary 9.2.9, there exists a function $F \in M$ such that ${ \cal M } \vert = { } ^ { \ast } F \colon \alpha  [ \kappa ] { \leq } \omega \ast \quad$ and $g ( \xi ) \in F ( \xi )$ for all $\xi \in \alpha$ . Hence $\begin{array} { r } { \kappa = g [ \alpha ] \subset \bigcup _ { \xi \in \alpha } F ( \xi ) } \end{array}$ 

But $\textstyle \bigcup _ { \xi \in { \boldsymbol { \alpha } } } { \bar { F } } ( \xi ) \in M$ , since $F \in M$ . So the following holds in M: 

$$
\kappa \leq \left| \bigcup_ {\xi \in \alpha} F (\xi) \right| \leq | \alpha | \otimes \omega <   \kappa ,
$$

since all sets $F ( \xi )$ are countable in M. This contradiction finishes the proof.  

To apply this theorem to the proof of the consistency of $\mathrm { Z F C + \lnot C H }$ we need one more fact (compare Exercise 1 from Section 8.2). 

Lemma 9.2.12 Forcing $\mathbb { P } = \langle \mathrm { F u n c } _ { \omega } ( X , Y ) , \supset \rangle$ is ccc for $| Y | \le \omega$ 

Proof Let $\langle p _ { \xi } \colon \xi < \omega _ { 1 } \rangle$ be a one-to-one sequence of elements of $\mathbb { P } .$ . We have to find $\zeta < \xi < \omega _ { 1 }$ such that $p _ { \zeta }$ and $p _ { \xi }$ are compatible. 

Consider the family $\mathcal { A } = \{ \mathrm { d o m } ( p _ { \xi } ) \colon \xi < \omega _ { 1 } \}$ of finite sets. Notice that A must be uncountable, since for every $A \in { \mathcal { A } }$ there is at most $| Y ^ { A } | \le \omega$ $p _ { \xi } \mathrm { s }$ with $A = \operatorname { d o m } ( p _ { \xi } )$ . So, by the ∆-system lemma (Lemma 8.2.11), there exist an uncountable set $S \subset \omega _ { 1 }$ and a finite A with the property that dom $( p _ { \zeta } ) \cap \mathrm { d o m } ( p _ { \xi } ) = A$ for any distinct $\zeta , \xi \in S$ . But the set $Y ^ { A }$ is at most countable. So there exist distinct $\zeta$ and $\xi$ from S such that $p _ { \zeta } | _ { A } = p _ { \xi } | _ { A }$ This implies that $p = p _ { \zeta } \cup p _ { \xi }$ is a function, that is, $p \in \mathbb { P }$ . Since p clearly extends $p _ { \zeta }$ and $p _ { \xi }$ we conclude that $p _ { \zeta }$ and $p _ { \xi }$ are compatible.  

## Theorem 9.2.13 Theory $Z F C + \lnot C H$ is consistent.

Proof We will follow the path described in Example 9.1. Let M be a countable transitive model of ZFC. Define (in M) 

$$
\mathbb {P} = \langle \mathrm{Func} _ {\omega} (\omega_ {2} ^ {M} \times \omega , 2), \supset \rangle
$$

and let G be an M-generic filter in P. We will show that ${ \mathfrak { c } } > \omega _ { 1 }$ in $M [ G ]$ For $x \in \omega _ { 2 } ^ { M } \times \omega$ let 

$$
D _ {x} = \{p \in \mathbb {P}: x \in \operatorname{dom} (p) \}.
$$

It is easy to see that all sets $D _ { x }$ belong to M since they are defined using $x , \mathbb { P } \in M$ . They are dense, since for every $p \in \mathbb { P }$ either $x \in \operatorname { d o m } ( p )$ and $p \in D _ { x }$ , or $x \not \in \operatorname { d o m } ( p )$ and $p \cup \{ \langle x , 0 \rangle \} \in D _ { x }$ extends $p .$ . Thus, by Proposition 8.1.1, $g = \bigcup G$ is a function from $\omega _ { 2 } ^ { M } \times \omega$ to 2. Clearly $g \in M [ G ]$ , since it is constructed from $G \in M [ G ]$ 

Similarly as for $D _ { x }$ we argue that for every $\zeta < \xi < \omega _ { 2 } ^ { M }$ the sets 

$$
E _ {\zeta} ^ {\xi} = \{p \in \mathbb {P}: \exists n <   \omega [ \langle \zeta , n \rangle , \langle \xi , n \rangle \in \operatorname{dom} (p) \& p (\zeta , n) \neq p (\xi , n) ] \}
$$

are dense in $\mathbb { P }$ and belong to M. Thus an M-generic filter intersects every such set, that is, for every $\zeta < \xi < \omega _ { 2 } ^ { M }$ there exists an $n < \omega$ such that $g ( \zeta , n ) \neq g ( \xi , n )$ 

Now for every $\xi < \omega _ { 2 } ^ { M }$ we can define (in $M [ G ] )$ a function $g _ { \xi } \colon \omega  2$ by $g _ { \xi } ( n ) = g ( \xi , n )$ . The set $\{ g _ { \xi } \colon \xi < \omega _ { 2 } ^ { M } \}$ belongs to $M [ G ]$ , since it has been constructed only from $g \in M [ G ]$ . Moreover, $\{ g _ { \xi } \colon \xi < \omega _ { 2 } ^ { M } \} \subset 2 ^ { \omega }$ and all the functions $g _ { \xi }$ are diferent. So 

$$
M [ G ] \models \mathfrak {c} = | 2 ^ {\omega} | \geq \omega_ {2} ^ {M}.
$$

But, by Lemma 9.2.12, forcing $\mathbb { P }$ is ccc in M and so, by Theorem 9.2.7, it preserves cardinals. In particular, by Lemma $9 . 2 . 1 0 , \omega _ { 2 } ^ { \bar { M } } = \omega _ { 2 } ^ { M [ G ] }$ , that is, 

$$
M [ G ] \models \mathfrak {c} \geq \omega_ {2} ^ {M [ G ]} > \omega_ {1}.
$$

This finishes the proof. 

A model $M [ G ]$ obtained as a generic extension of a ground model M via the forcing $\mathbb { P } = \langle \mathrm { F u n c } _ { \omega } ( X , 2 ) , \supset \rangle$ (with $X \in M )$ is called a Cohen model. The numbers $g _ { \xi }$ from Theorem 9.2.13 are called Cohen (real) numbers. 

## EXERCISES

1 Prove that $x \in R ( \omega )$ if and only if $| \operatorname { t r c l } ( x ) | < \omega$ . Use this to show that $M = R ( \omega )$ is a model for ZFC minus the infinity axiom. 

2 Let $\psi ( \tau )$ be a formula expressing the property that $^ { 6 6 } \tau$ is a $\mathbb { P } { \mathrm { - n a m e } } ^ { \mathrm { 5 } }$ and let M be a CTM of ZFC with $\mathbb { P } \in M$ . Show, by induction on rank(τ), that for every $\tau \in M$ 

$$
\psi (\tau) \text { if   and   only   if } \psi^ {M} (\tau).
$$

Thus the property “τ is a $\mathbb { P } { \mathrm { - n a m e } } ^ { \prime }$ is absolute. 

3 Complete the details of the proof of Lemma 9.2.6. 

4 Let M be a countable transitive model of ZFC, $\mathbb { P } \in M$ be a partial order, and $G$ be an M-generic filter in P. Show that $\omega _ { \alpha } ^ { M } \leq \omega _ { \alpha } ^ { M [ G ] }$ for every ordinal number $\alpha \in M$ 

5 Prove Lemma 9.2.10. 

## 9.3 Model for CH and $\diamondsuit$

The main goal of this section is to prove the following theorem. 

Theorem 9.3.1 Let M be a countable transitive model of $Z F C ,$ , and let $\mathbb { P } = ( \operatorname { F u n c } _ { \omega _ { 1 } } ( \omega _ { 1 } , 2 ) ) ^ { M }$ . If G is an M-generic filter in $\mathbb { P }$ then $\omega _ { 1 } ^ { M } = \omega _ { 1 } ^ { M [ G ] }$ , $\mathcal { P } ( \omega ) \cap M = \mathcal { P } ( \omega ) \cap M [ G ]$ , and $\diamondsuit$ holds in $M [ G ]$ 

Since $\diamondsuit$ implies CH the theorem immediately implies the following corollary. 

Corollary 9.3.2 Theories ZFC+CH and $Z F C + \diamond$ are consistent. 

Combining this with Theorem 9.2.13 we immediately obtain the following. 

Corollary 9.3.3 The continuum hypothesis is independent of $Z F C .$ 

Note that $\mathbb { P } = \operatorname { F u n c } _ { \omega _ { 1 } } ( \omega _ { 1 } , 2 )$ stands for the set of all functions $p \colon A \to 2$ , where A is an at most countable subset of $\omega _ { 1 }$ . Since the terms $^ { 6 } \omega _ { 1 } \mathfrak { I }$ and “being countable” are not absolute, the superscript $M$ in the definition of $\mathbb { P }$ in Theorem 9.3.1 is essential. 

We will prove Theorem 9.3.1 with the help of several general facts that are, in most cases, as important as the theorem itself. 

Let $\mathbb { P }$ be a partially ordered set and let $p \in \mathbb { P }$ . A set $D \subset \mathbb { P }$ is dense below p if for every $q \leq p$ there exists a $d \in D$ such that $d \leq q$ 

Proposition 9.3.4 Let M be a countable transitive model of ZFC, $\mathbb { P } \in M$ be a partially ordered set, and $p \in \mathbb { P }$ . If $D \in M$ is a subset of $\mathbb { P }$ that is dense below p then $G \cap D \neq \emptyset$ for every M-generic filter $G$ in $\mathbb { P }$ such that $p \in G$ 

Proof Let $R = \{ r \in \mathbb { P } \colon r$ is incompatible with $p \}$ . Then $D _ { 0 } = D \cup R \in M$ and $D _ { 0 }$ is dense in P. So if G is an M-generic filter in P then $G \cap D _ { 0 } \neq \emptyset$ But if $p \in G$ then $G \cap R = \emptyset$ , so $G \cap D \neq \emptyset$  

A partially ordered set P is countably closed if for every decreasing sequence $\langle p _ { n } \in \mathbb { P } \colon n < \omega \rangle$ there is a $p _ { \omega } \in \mathbb { P }$ such that $p _ { \omega } \leq p _ { n }$ for every $n \ < \ \omega$ . Notice that $\mathbb { P } ^ { \star } = \operatorname { F u n c } _ { \omega _ { 1 } } ( \omega _ { 1 } , 2 )$ is countably closed since $p _ { \omega } =$ $\textstyle \bigcup _ { n < \omega } p _ { n } \in \mathbb { P }$ extends every $p _ { n }$ . So $\mathbb { P } = ( \operatorname { F u n c } _ { \omega _ { 1 } } ( \omega _ { 1 } , 2 ) ) ^ { M }$ is countably closed in $M$ 

Theorem 9.3.5 Let M be a countable transitive model of ZFC and $\mathbb { P } \in M$ be a partially ordered set that is countably closed in M. Let $A , B \in M$ be such that A is countable in M and let G be an M-generic filter in P. If $f \in M [ G ]$ is a function from A into B then $f \in M$ 

Proof Let $\tau \in M$ be a P-name such that $\mathrm { v a l } _ { G } ( \tau ) = f$ . Then, by Theorem 9.2.7, there exists a $p \in G$ such that 

$p \Vdash \tau$ is a function from $\hat { A }$ into $\hat { B }$ . 

Define in M 

$$
D = \{q \in \mathbb {P} \colon \exists g \in B ^ {A} (q \| - \tau = \hat {g}) \}.
$$

(D belongs to M since the relation $\parallel -$ can be replaced by the formula $\| - ^ { \star } . )$ By Proposition 9.3.4 it is enough to prove that D is dense below $p$ since then there exists a $q \in G \cap D$ , that is, there is a $g \in M$ such that g maps A to B and 

$$
f = \operatorname{val} _ {G} (\tau) = \operatorname{val} _ {G} (\hat {g}) = g \in M.
$$

To prove that D is dense below p, fix $r \in \mathbb { P }$ such that $r \le p$ . We have to find a $q \in D$ with $q \leq r$ . Let $\{ a _ { n } \colon n < \omega \}$ be an enumeration of A in M. Define, in M, sequences $\langle p _ { n } \in \mathbb { P } \colon n < \omega \rangle$ and $\langle b _ { n } \in B \colon n < \omega \rangle$ such that for all $n < \omega$ 

(1) $p _ { 0 } = r ,$ 

(2) $p _ { n + 1 } \leq p _ { n } ,$ 

(3) $p _ { n + 1 } \parallel - \tau ( \hat { a } _ { n } ) = \hat { b } _ { n } .$ 

To see that such a construction can be made assume that $p _ { i }$ for $i \leq n$ and $b _ { j }$ for $j < n$ have already been constructed. It is enough to show that there exist $p _ { n + 1 }$ and $b _ { n }$ satisfying (2) and (3). 

The proof of the existence of such $p _ { n + 1 }$ and $b _ { n }$ will be done outside M. For this, let H be an M-generic filter in P with $p _ { n } \in H$ . Then $h = \operatorname { v a l } _ { H } ( \tau )$ is a function in $M [ H ]$ from A into B, since $p _ { n } \leq p$ forces it. Thus there is a $b \in B$ such that $h ( a _ { n } ) = b$ and we can find an $r \in H$ which forces it, that is, such that $r \parallel - \tau ( \hat { a } _ { n } ) = \hat { b }$ . Refining r, if necessary, we can also assume that $r \leq p _ { n }$ . Then $p _ { n + 1 } = r$ and $b _ { n } = b$ satisfy (2) and (3). 

Now let $p _ { \omega } \in \mathbb { P }$ be such that $p _ { \omega } \leq p _ { n }$ for every $n < \omega$ and let $g \colon A  B$ be such that $g ( a _ { n } ) = b _ { n }$ . Then $g \in M$ and 

$$
p _ {\omega} \parallel - \tau (\hat {a} _ {n}) = \hat {b} _ {n}
$$

for every $n < \omega$ . To finish the proof it is enough to show that 

$$
p _ {\omega} \parallel - \tau = \hat {g}
$$

since then $q = p _ { \omega } \leq r$ and belongs to $D$ . 

So let H be an arbitrary M-generic filter in P with $p _ { \omega } \in H$ . Then $h = \mathrm { v a l } _ { H } ( \tau )$ is a function in $M [ H ]$ from A into B. Moreover, $h ( a _ { n } ) = b _ { n }$ for every $n < \omega$ since $p _ { \omega } \leq p _ { n }$ forces it. In particular, 

$$
M [ H ] \models h = \operatorname{val} _ {H} (\tau) = g
$$

that is, $p _ { \omega } \parallel - \tau = \hat { g }$ 

Theorem 9.3.5 tells us that in a generic extension of a model M obtained from a countably closed forcing the extension will have the same countable sequences with elements from a fixed set from M. This implies the following corollary. 

Corollary 9.3.6 Let M be a countable transitive model of $Z F C$ and $\mathbb { P } \in M$ be a partially ordered set that is countably closed in M. If G is an Mgeneric filter in $\mathbb { P }$ then $\mathcal { P } ( \omega ) \cap M = \mathcal { P } ( \omega ) \cap M [ G ]$ and $\omega _ { 1 } ^ { M } \doteq \omega _ { 1 } ^ { M [ G ] }$ 

Proof Let $\beta = \omega _ { 1 } ^ { M }$ . If $\alpha \leq \beta$ then α is an ordinal number in M and in $M [ G ]$ . Moreover, if $\alpha < \beta$ then there exists an $f \in M \subset M [ G ]$ such that $f$ maps ω onto α. Thus every α $< \beta$ is at most countable (in M and in $M [ G ] )$ In particular, it is enough to show that $\beta$ is uncountable in $M [ G ]$ , since then it is the first uncountable ordinal in $M [ G ]$ , that is, $\omega _ { 1 } ^ { M } = \beta = \omega _ { 1 } ^ { M [ G ] }$ 

To see that $\beta$ is uncountable in $M [ G ]$ , take $f \colon \omega  \beta$ from $M [ G ]$ and notice that, by Theorem 9.3.5, $f \in M$ . So f cannot be onto $\beta = \omega _ { 1 } ^ { M }$ . Thus $\beta$ is uncountable in $M [ G ]$ 

To see that $\mathcal { P } ( \omega ) \cap M \ : = \ : \mathcal { P } ( \omega ) \cap M [ G ]$ it is enough to prove that $\mathcal { P } ( \omega ) \cap M [ G ] \subset \mathcal { P } ( \omega ) \cap M$ . So let $A \in { \mathcal { P } } ( \omega ) \cap M [ G ]$ and let $f = \chi _ { A } \colon \omega \to 2$ Then $f \in M [ G ]$ and, by Theorem 9.3.5, $f \in M$ . Therefore $A = f ^ { - 1 } ( 1 ) \in$ $\mathcal { P } ( \omega ) \cap M$  

Notice that Corollary 9.3.6 implies the statements $\omega _ { 1 } ^ { M } = \omega _ { 1 } ^ { M [ G ] }$ and $\mathcal { P } ( \omega ) \cap M = \mathcal { P } ( \omega ) \cap M [ G ]$ of Theorem 9.3.1 since the forcing P from the theorem is countably closed in M. Notice also that Corollary 9.3.6 does not imply that countably closed forcings preserve all cardinal numbers. In fact, by proving Theorem 9.3.1 we will show that in $M [ G ]$ there exists a bijection between $\omega _ { 1 } ^ { M } = \omega _ { 1 } ^ { M [ G ] }$ and $\mathcal { P } ^ { M } ( \omega ) = \mathcal { P } ^ { M [ G ] } ( \omega )$ , that is, there is a bijection between $\omega _ { 1 } ^ { M }$ and ${ \mathfrak { c } } ^ { M }$ . Thus, if $\omega _ { 1 } ^ { M } < \mathfrak { c } ^ { M }$ (which can happen by a result from the previous section) then the cardinal ${ \mathfrak { c } } ^ { M }$ is collapsed in $M [ G ]$ 

To prove that $\diamondsuit$ holds in the model $M [ G ]$ from Theorem 9.3.1 the following lemma will be useful. 

Lemma 9.3.7 Let M be a countable transitive model ofZFC and let $\mathbb { P } , \mathbb { P } _ { 1 } \in$ M be partially ordered sets such that there is an order isomorphism $f \in M$ between $\mathbb { P }$ and $\mathbb { P } _ { 1 }$ . If G is an M-generic filter in $\mathbb { P }$ then $G _ { 1 } = f [ G ]$ is an M-generic filter in $\mathbb { P } _ { 1 }$ and $M [ G ] = M [ G _ { 1 } ]$ 

Proof It is easy to see that $G _ { 1 } = f [ G ]$ is a filter in $\mathbb { P } _ { 1 }$ . To see that $G _ { 1 }$ is M-generic let $D _ { 1 } \in M$ be a dense subset of $\mathbb { P } _ { 1 }$ . Then $D = f ^ { - 1 } ( D _ { 1 } )$ belongs to M and is dense in P. So $D \cap G \neq \emptyset$ and 

$$
D _ {1} \cap G _ {1} = f [ D ] \cap f [ G ] = f [ D \cap G ] \neq \emptyset .
$$

To see that $M [ G ] = M [ G _ { 1 } ]$ notice that $M \subset M [ G ]$ and $M \subset M [ G _ { 1 } ]$ Moreover, $G _ { 1 } = f [ G ] \in M [ G ]$ ; thus, by the minimality of $M [ G _ { 1 } ]$ , we conclude $M [ G _ { 1 } ] \subset M [ G ]$ . Similarly, $G = f ^ { - 1 } ( G _ { 1 } ) \in M [ G _ { 1 } ]$ . Thus $M [ G ] \subset$ $M [ G _ { 1 } ]$  

Lemma 9.3.7 tells us that if we replace a forcing by its isomorphic copy then the appropriate generic extensions will be identical. In particular, if $X \in M$ is such that $M \models | X | = \omega _ { 1 }$ then forcings $\mathbb { P } = ( \operatorname { F u n c } _ { \omega _ { 1 } } ( \omega _ { 1 } , 2 ) ) ^ { M }$ and $\mathbb { P } _ { 1 } = ( \operatorname { F u n c } _ { \omega _ { 1 } } ( X , 2 ) ) ^ { M }$ are isomorphic in M (by an isomorphism $F \colon \mathbb { P }  \mathbb { P } _ { 1 }$ with $F ( p ) ( x ) = p ( f ( x ) )$ , where $f \colon X \to \omega _ { 1 } ^ { M }$ is a bijection with $f \in M )$ 

Before we prove that ♦ holds in the model $M [ G ]$ from Theorem 9.3.1 we will show that $M [ G ] \models C H$ . This is not used in the proof of $M [ G ] \models \emptyset$ However, the proof of CH in $M [ G ]$ is simpler than the one for $\diamondsuit .$ , and it will prepare the reader for the later one. Moreover, the reader interested only in the consistency of $\mathrm { Z F C + C H }$ can skip the latter part of this section. 

By Lemma 9.3.7 we can replace P with $\mathbb { P } _ { 1 } = ( \operatorname { F u n c } _ { \omega _ { 1 } } ( \omega _ { 1 } \times \omega , 2 ) ) ^ { M }$ . Let $G _ { 1 }$ be an M-generic filter in $\mathbb { P } _ { 1 }$ . Thus $M [ G ] = M [ G _ { 1 } ]$ . Clearly $g = \bigcup G _ { 1 }$ belongs to $M [ G ]$ and, by Proposition 8.1.1, it is a function from $\omega _ { 1 } ^ { M } \times \omega$ to 2. Notice that for every $f \in 2 ^ { \omega } \cap$ M the set 

$$
D _ {f} = \{p \in \mathbb {P} _ {1}: \exists \alpha <   \omega_ {1} ^ {M} [ \{\alpha \} \times \omega \subset \operatorname{dom} (p) \& \forall n <   \omega (p (\alpha , n) = f (n)) ] \}
$$

belongs to M and is dense in $\mathbb { P } _ { 1 }$ . (To see its denseness, choose $p \in \mathbb { P } _ { 1 }$ find $\bar { \alpha } < \omega _ { 1 } ^ { M }$ with $( \{ \alpha \} \times \omega ) \cap \mathrm { d o m } ( p ) = \emptyset .$ , and notice that the condition $p \cup \{ \langle \langle \alpha , n \rangle , f ( n ) \rangle \colon n < \omega \} \in D _ { f }$ extends $p . )$ So if $f _ { \alpha } \colon \omega  2$ for $\alpha < \omega _ { 1 } ^ { M }$ is defined by $f _ { \alpha } ( n ) = g ( \alpha , n )$ then, by Theorem 9.3.5, 

$$
2 ^ {\omega} \cap M \subset \left\{f _ {\alpha}: \alpha <   \omega_ {1} ^ {M} \right\} \subset 2 ^ {\omega} \cap M [ G ] = 2 ^ {\omega} \cap M.
$$

Thus, in $M [ G ]$ 

$$
\omega_ {1} ^ {M [ G ]} = \omega_ {1} ^ {M} = | \omega_ {1} ^ {M} | = | \{f _ {\alpha} \colon \alpha <   \omega_ {1} ^ {M} \} | = | 2 ^ {\omega} \cap M [ G ] | = \mathfrak {c} ^ {M [ G ]}.
$$

So CH holds in $M [ G ]$ 

Proof of Theorem 9.3.1 The proof is similar to that of Theorem 9.3.5. Let $X ~ = ~ \{ \langle \zeta , \xi \rangle \colon \zeta ~ < ~ \eta ~ < ~ \omega _ { 1 } ^ { M } \}$ and replace $\mathbb { P } = ( \operatorname { F u n c } _ { \omega _ { 1 } } ( \omega _ { 1 } , 2 ) ) ^ { M }$ with $\mathbb { P } _ { 2 } = ( \operatorname { F u n c } _ { \omega _ { 1 } } ( X , 2 ) ) ^ { M }$ . We can do this by Lemma 9.3.7 since these forcings are isomorphic in M. Let G be an M-generic filter in $\mathbb { P } _ { 2 }$ and let $g = \bigcup G \in M [ G ]$ . Then g is a function from X to 2. For $\alpha < \omega _ { 1 } ^ { M }$ let $g _ { \alpha } \colon \alpha \to 2$ be defined by $g _ { \alpha } ( \zeta ) = g ( \zeta , \alpha )$ and put $A _ { \alpha } = g _ { \alpha } ^ { - 1 } ( 1 )$ . It is easy to see that the sequence $\langle A _ { \alpha } \colon \alpha < \omega _ { 1 } ^ { M } \rangle$ belongs to $M [ G ]$ . We will show that it is a ♦-sequence in $M [ G ]$ 

So let $A \in M [ G ]$ be such that $A \subset \omega _ { 1 } ^ { M [ G ] } = \omega _ { 1 } ^ { M }$ and let $f = \chi _ { A }$ . We have to show that the set 

$$
S = \{\alpha <   \omega_ {1} ^ {M}: A \cap \alpha = A _ {\alpha} \} = \{\alpha <   \omega_ {1} ^ {M}: f | _ {\alpha} = g _ {\alpha} \}
$$

is stationary in $M [ G ]$ (remember that $\omega _ { 1 } ^ { M [ G ] } = \omega _ { 1 } ^ { M } )$ . For this, let $C \subset \omega _ { 1 } ^ { M }$ , $C \in M [ G ]$ , be such that 

$M [ G ] \models C$ is a closed unbounded subset of $\omega _ { 1 }$ 

We will show that $S \cap C \neq \emptyset$ , that is, that there exists an $\alpha \in C$ such that $f | _ { \alpha } = g _ { \alpha }$ 

Let $\tau , \sigma \in M$ be $\mathbb { P } _ { 2 } { \mathrm { - n a m e s } }$ such that $\mathrm { v a l } _ { G } ( \tau ) = f$ and $\mathrm { v a l } _ { G } ( \sigma ) = C$ Then there exists a $p \in G$ such that 

$p \Vdash ( \sigma$ is a closed unbounded subset of $\hat { \omega } _ { 1 } \} _ { \mathcal { X } } \tau : \hat { \omega } _ { 1 } \to \hat { 2 } )$ 

Define in M the set D by 

$$
\left. \left\{q \in \mathbb {P} _ {2}: \exists \alpha <   \omega_ {1} ^ {M} \left(q \| - (\hat {\alpha} \in \sigma \& \forall \zeta <   \hat {\alpha} (\tau (\zeta) = (\bigcup \Gamma) (\zeta , \hat {\alpha}))\right)\right) \right\},
$$

where Γ is the standard $\mathbb { P } _ { 2 } { \mathrm { - n a m e } }$ for a generic filter. It is enough to prove that D is dense below p since then there exists a $q \in G \cap D$ and so there is an $\alpha \in \mathrm { v a l } _ { G } ( \sigma ) = C$ such that 

$$
f (\zeta) = g (\zeta , \alpha) \text { for   all } \zeta <   \alpha ,
$$

that is, $\smash { f | _ { \alpha } = g _ { \alpha } }$ 

To prove that D is dense below p fix an $r \in \mathbb { P }$ such that $r \le p$ . We have to find a $q \in D$ with $q \leq r$ 

Define in M the sequences $\langle p _ { n } \in \mathbb { P } _ { 2 } : n < \omega \rangle , \langle \beta _ { n } < \omega _ { 1 } ^ { M } : n < \omega \rangle$ $\langle \delta _ { n } < \omega _ { 1 } ^ { M } : n < \omega \rangle$ , and $\langle b _ { n } \in 2 ^ { \beta _ { n } } : n < \omega \rangle$ such that for every $n < \omega$ 

(1) $p _ { 0 } = r$ and $\delta _ { 0 } = 0 :$ ; 

(2) $\operatorname { d o m } ( p _ { n } ) \subset \{ \langle \zeta , \xi \rangle \colon \zeta < \xi < \beta _ { n } \}$ ; 

(3) $p _ { n } \leq p _ { n - 1 } { \mathrm { ~ i f ~ } } n > 0 ;$ ; 

(4) $\beta _ { n - 1 } < \delta _ { n } < \beta _ { n } { \mathrm { ~ i f ~ } } n > 0 ;$ 

$$
5) \quad p _ {n} \| - \left(\hat {\delta} _ {n} \in \sigma \& \tau | _ {\hat {\beta} _ {n - 1}} = \hat {b} _ {n}\right) \text {if} n > 0.
$$

To see that such a construction can be made assume that for some $n < \omega$ the sequences are defined for all $i < n$ . If $n = 0$ then $p _ { 0 }$ and $\delta _ { 0 }$ are already constructed and $\beta _ { 0 }$ and $b _ { 0 }$ can be easily chosen, since the conditions (3), (4), and (5) do not concern this case. So assume that $n > 0$ . We have to show that the inductive step can be made, that is, that appropriate $p _ { n } , \beta _ { n }$ $\delta _ { n }$ , and $b _ { n }$ exist. 

So let $G _ { 0 }$ be an $M { \mathrm { - g e n e r i c } }$ filter in $\mathbb { P } _ { 2 }$ with $p _ { n - 1 } \in G _ { 0 }$ . Then $f _ { 0 } =$ $\mathrm { v a l } _ { G _ { 0 } } ( \tau ) \ \in \ M [ G _ { 0 } ]$ is a function from $\omega _ { 1 } ^ { M }$ to 2 and $C _ { 0 } = \mathrm { v a l } _ { G _ { 0 } } ( \sigma )$ is a closed and unbounded subset of $\omega _ { 1 }$ in $M [ G _ { 0 } ]$ , since $p _ { n - 1 } \leq p$ forces it. In particular, there exists a $d \in C _ { 0 }$ with $d > \beta _ { n - 1 }$ . Also, $b = h | _ { \beta _ { n - 1 } } \in M$ , since $\mathbb { P } _ { 2 }$ is countably closed. So there exists a $q \in G _ { 0 }$ , with $q \leq p _ { n - 1 }$ , that forces it. Then $p _ { n } = q , b _ { n } = b $ , and $\delta _ { n } = d \mathrm { s a t i s f y } ( 3 ) , ( 5 )$ , and the first part of (4). The choice of $\beta _ { n }$ satisfying (2) and (4) finishes the construction. 

Now let $\begin{array} { r } { p _ { \omega } = \bigcup _ { n < \omega } p _ { n } \in \mathbb { P } _ { 2 } } \end{array}$ . Then for all $n < \omega$ 

$$
p _ {\omega} \left\| - \left(\hat {\delta} _ {n + 1} \in \sigma \& \tau | _ {\hat {\beta} _ {n}} = \hat {b} _ {n + 1}\right). \right.
$$

Thus the functions $b _ { n + 1 }$ must be compatible, and $\textstyle b = \bigcup _ { n < \omega } b _ { n + 1 } \in M$ is a function from $\begin{array} { r } { \alpha = \bigcup _ { n < \omega } \beta _ { n } = \bigcup _ { n < \omega } \delta _ { n } } \end{array}$ into 2. 

Put $q = p _ { \omega } \cup \{ \langle \langle \zeta , \alpha \rangle , b ( \zeta ) \rangle \colon \zeta < \alpha \}$ . Notice that q is a function since, by (2), dom $\left( p _ { \omega } \right)$ is disjoint from $\{ \langle \zeta , \alpha \rangle \colon \zeta < \alpha \}$ . Since $q \leq r$ it is enough to show that q belongs to D. 

So let $G _ { 1 }$ be an M-generic filter in $\mathbb { P } _ { 2 }$ containing q and let $C _ { 1 } = \mathrm { v a l } _ { G _ { 1 } } ( \sigma )$ and $f _ { 1 } { \mathrm { \Delta } } = \operatorname { v a l } _ { G _ { 1 } } ( \tau )$ . It is enough to show that $\alpha ~ \in ~ C _ { 1 }$ and $f _ { 1 } ( \zeta ) =$ $\left( \bigcup \Gamma \right) \left( \zeta , \alpha \right)$ for every $\zeta < \alpha$ . But $C _ { 1 }$ is a closed unbounded subset of $\omega _ { 1 } ^ { \dot { M } [ G _ { 1 } ] }$ and $\delta _ { n + 1 } \in C _ { 1 }$ for every $n < \omega$ , since q forces it. Thus $\begin{array} { r } { \alpha = \bigcup _ { n < \omega } \delta _ { n } \in C _ { 1 } } \end{array}$ Also, for every $\zeta < \alpha$ there exists an $n < \omega$ such that $\zeta < \beta _ { n }$ . So 

$$
f _ {1} (\zeta) = \operatorname{val} _ {G _ {1}} (\tau) | _ {\beta_ {n}} (\zeta) = b _ {n + 1} (\zeta) = b (\zeta) = q (\zeta , \alpha) = \left(\bigcup \Gamma\right) (\zeta , \alpha).
$$

This finishes the proof. 

The proof just presented can be easily generalized to the following theorem. Its proof is left as an exercise. 

Theorem 9.3.8 Let M be a countable transitive model of ZFC, κ be a regular cardinal in M, and $\mathbb { P } = ( \operatorname { F u n c } _ { \kappa ^ { + } } ( \kappa ^ { + } \times \kappa , 2 ) ) ^ { M }$ . Then forcing P preserves all cardinals $\leq \kappa ^ { + }$ and $2 ^ { \kappa } = \kappa ^ { + }$ holds in $M [ G ]$ , where G is an M-generic filter in P. 

Theorem 9.3.8 implies immediately the following corollary, which will be used in Section 9.5. 

Corollary 9.3.9 It is relatively consistent with ZFC that $2 ^ { \omega _ { 1 } } = \omega _ { 2 }$ 

## EXERCISES

1 Complete the details of Lemma 9.3.7 by showing that for every isomorphism f between partially ordered sets P and $\mathbb { P } _ { 1 }$ and every $G , D \subset \mathbb { P }$ 

(1) G is a filter in P if and only if $f [ G ]$ is a filter in $\mathbb { P } _ { 1 }$ ; 

(2) D is dense in P if and only if $f [ D ]$ is dense in $\mathbb { P } _ { 1 }$ . 

2 Show that the functions $b _ { n + 1 }$ from the proof of Theorem 9.3.1 are indeed compatible and that $\textstyle b = \bigcup _ { n < \omega } b _ { n + 1 }$ is a function from α to 2. 

3 Prove Theorem 9.3.8 in the following steps. 

(a) Generalize the proof of Theorem 9.3.5 to show that if $f \in M [ G ]$ is a function from κ into $A \in M$ then $f \in M$ 

(b) Use (a) and the ideas from the proof of Corollary 9.3.6 to show that $\mathbb { P }$ preserves cardinals $\leq \kappa ^ { + }$ and $\mathcal { P } ( \kappa ) \cap M = \mathcal { P } ( \kappa ) \cap M [ G ]$ 

(c) Show that the function $f \colon \kappa ^ { + } \to 2 ^ { \kappa } , f ( \alpha ) ( \beta ) \ = ( \bigcup G ) ( \alpha , \beta )$ , is onto $2 ^ { \kappa }$ 

## 9.4 Product lemma and Cohen model

In the next section we will prove the consistency of $\mathrm { M A } { + } { \lnot \mathrm { C H } }$ . The method used in its proof is called iterated forcing. The idea behind this method is to repeat the forcing extension process recursively, that is, to construct by transfinite induction of some length α a sequence 

$$
M = M _ {0} \subset M _ {1} \subset \dots \subset M _ {\xi} \subset \dots \subset M _ {\alpha}
$$

of countable transitive models of ZFC such that $M _ { \xi + 1 } = M _ { \xi } [ G _ { \xi } ]$ for every $\xi < \alpha .$ , where $G _ { \xi }$ is an $M _ { \xi ^ { - } } \mathrm { g e n e r i c }$ filter in some forcing $\mathbb { P } _ { \xi } \in M _ { \xi }$ 

This description is very specific and easy to handle at successor stages. The limit stage, however, presents a problem. For a limit ordinal $\lambda \leq \alpha$ we cannot simply take $\begin{array} { r } { M _ { \lambda } = \bigcup _ { \xi < \lambda } M _ { \xi } } \end{array}$ , since such an $M _ { \lambda }$ does not have to be a model of ZFC. Intuitively, we can avoid this problem by defining $M _ { \lambda }$ as a generic extension of M by a sequence $\langle G _ { \xi } \colon \xi < \lambda \rangle$ . But in what forcing should the sequence $\langle G _ { \xi } \colon \xi < \lambda \rangle$ be a generic filter? 

To solve this problem, we will find one forcing in the ground model that will encode all forcings used in our intuitive inductive construction. In this project, however, we will find that the successor step creates more trouble than the limit one. In fact, at the moment we don’t even know whether the model $M _ { 2 } = M [ G _ { 0 } ] [ G _ { 1 } ]$ obtained by two consecutive generic extensions can also be obtained by a single generic extension, that is, whether $M _ { 2 } = M [ G ]$ for some $\mathbb { P } \in M$ and an M-generic filter G in P. 

In this section we will concentrate on this problem only in the easier case where both partially ordered sets $\mathbb { P } _ { 0 }$ and $\mathbb { P } _ { 1 }$ leading to the extensions $M _ { 1 } = M [ G _ { 1 } ]$ and $M _ { 2 } = M _ { 1 } [ G _ { 1 } ]$ , respectively, belong to the ground model M. The general iteration, including that of two-stage iteration, will be described in the next section. 

In the simple case when $\mathbb { P } _ { 0 } , \mathbb { P } _ { 1 } \in M$ the forcing $\mathbb { P }$ is just a product of forcings $\langle \mathbb { P } _ { 0 } , \leq _ { 0 } \rangle$ and $\langle \mathbb { P } _ { 1 } , \leq _ { 1 } \rangle$ , that is, $\mathbb { P } = \mathbb { P } _ { 0 } \times \mathbb { P } _ { 1 }$ and 

$$
\left\langle p _ {0}, p _ {1} \right\rangle \leq \left\langle q _ {0}, q _ {1} \right\rangle \Leftrightarrow p _ {0} \leq_ {0} q _ {0} \& p _ {1} \leq_ {1} q _ {1}.
$$

<!-- === Source: MinerU_markdown_Set_theory_for_the_working_mathematician,_K._Ciesielski,_CUP,_1997_201_2122706224590991363.md (Page 201) === -->

The relation between the forcing extensions obtained by these partially ordered sets is described in the next theorem. We will start, however, with the following simple fact. 

Proposition 9.4.1 Let P be a product of the forcings $\mathbb { P } _ { 0 }$ and $\mathbb { P } _ { 1 }$ . Then G is a filter in P if and only if $G = G _ { 0 } \times G _ { 1 }$ for some filters $G _ { 0 }$ and $G _ { 1 }$ in $\mathbb { P } _ { 0 }$ and $\mathbb { P } _ { 1 }$ , respectively. 

Proof First, assume that G is a filter in P. Let $G _ { 0 }$ and $G _ { 1 }$ be the projections of G onto the first and the second coordinates, respectively. Then $G \subset G _ { 0 } \times G _ { 1 }$ 

To see the other inclusion take $p _ { 0 } \in G _ { 0 }$ and $q _ { 1 } \in G _ { 1 }$ . Then there exist $q _ { 0 } \in G _ { 0 }$ and $p _ { 1 } \in G _ { 1 }$ such that $\langle p _ { 0 } , p _ { 1 } \rangle , \langle q _ { 0 } , q _ { 1 } \rangle \in G$ . Let $\langle r _ { 0 } , r _ { 1 } \rangle \in G$ be an extension of $\left. { p _ { 0 } , p _ { 1 } } \right.$ and $\left. q _ { 0 } , q _ { 1 } \right.$ . Then $\langle r _ { 0 } , r _ { 1 } \rangle \leq \langle p _ { 0 } , q _ { 1 } \rangle , \mathrm { s o } \langle p _ { 0 } , q _ { 1 } \rangle \in G$ 

The proof that $G _ { 0 }$ and $G _ { 1 }$ are filters is left as an exercise. It is also easy to see that $G = G _ { 0 } \times G _ { 1 }$ is a filter, provided $G _ { 0 }$ and $G _ { 1 }$ are.  

Proposition 9.4.1 tells us, in particular, that any filter in $\mathbb { P } _ { 0 } \times \mathbb { P } _ { 1 }$ is a product of filters in $\mathbb { P } _ { 0 }$ and in $\mathbb { P } _ { 1 }$ . This gives a better perspective on the next theorem. 

Theorem 9.4.2 (Product lemma) Let M be a countable transitive model of $Z F C ,$ , let $\mathbb { P } _ { 0 } , \mathbb { P } _ { 1 } \in M$ be partially ordered sets, and let $G _ { 0 } \subset \mathbb { P } _ { 0 }$ and $G _ { 1 } \subset \mathbb { P } _ { 1 }$ be filters. Then the following conditions are equivalent. 

(i) $G _ { 0 } \times G _ { 1 }$ is an M-generic filter in $\mathbb { P } _ { 0 } \times \mathbb { P } _ { 1 }$ 

(ii) $G _ { 0 }$ is an M-generic filter in $\mathbb { P } _ { 0 }$ and $G _ { 1 }$ is an M[G<sub>0</sub>]-generic filter in $\mathbb { P } _ { 1 }$ 

(iii) $G _ { 1 }$ is an M-generic filter in $\mathbb { P } _ { 1 }$ and $G _ { 0 }$ is an $M [ G _ { 1 } ]$ -generic filter in $\mathbb { P } _ { 0 }$ . 

Moreover, $i f$ any of these conditions hold then $M [ G _ { 0 } \times G _ { 1 } ] = M [ G _ { 0 } ] [ G _ { 1 } ] =$ $M [ G _ { 1 } ] [ G _ { 0 } ]$ 

Proof Note first that the natural isomorphism between $\mathbb { P } _ { 0 } \times \mathbb { P } _ { 1 }$ and $\mathbb { P } _ { 1 } \times \mathbb { P } _ { 0 }$ maps $G _ { 0 } \times G _ { 1 }$ onto $G _ { 1 } \times G _ { 0 }$ . Thus, by Lemma $9 . 3 . 7 .$ , condition (i) is equivalent to the condition 

(i<sup>-</sup>) $G _ { 1 } \times G _ { 0 }$ is an M-generic filter in $\mathbb { P } _ { 1 } \times \mathbb { P } _ { 0 }$ 

But the equivalence $( \mathrm { i } ^ { \prime } ) { \Leftrightarrow } ( \mathrm { i i i } )$ is obtained from $( \mathrm { i } ) { \Leftrightarrow } ( \mathrm { i } )$ by exchanging indices. So all equivalences follow from $( \mathrm { i } ) { \Leftrightarrow } ( \mathrm { i } )$ 

To prove $( \mathrm { i } ) { \Rightarrow } ( \mathrm { i i } )$ , assume (i). To see that $G _ { 0 }$ is M-generic in $\mathbb { P } _ { 0 }$ take a dense subset $D _ { 0 } \in M$ of $\mathbb { P } _ { 0 }$ . Then $D _ { 0 } \times \mathbb { P } _ { 1 } \in M$ is dense in $\mathbb { P } _ { 0 } \times \mathbb { P } _ { 1 }$ . Thus, by (i), $\left( D _ { 0 } \times \mathbb { P } _ { 1 } \right) \cap \left( G _ { 0 } \times G _ { 1 } \right) \neq \emptyset$ , and we conclude that $D _ { 0 } \cap G _ { 0 } \neq \emptyset$ 

To see that $G _ { 1 }$ is an M[G<sub>0</sub>]-generic filter in $\mathbb { P } _ { 1 }$ take a dense subset $D _ { 1 } \in M [ G _ { 0 } ]$ of $\mathbb { P } _ { 1 }$ . Let $\tau \in M$ be a $\mathbb { P } _ { 0 } { \mathrm { - n a m e } }$ such that $D _ { 1 } = \mathrm { v a l } _ { G _ { 0 } } ( \tau )$ and let $p _ { 0 } \in G _ { 0 }$ be such that 

$$
p _ {0} \left\| - \tau \text {   is   dense   in   } \hat {\mathbb {P}} _ {1}. \right.
$$

Choose $p _ { 1 } \in G _ { 1 }$ , define 

$$
D = \{\langle q _ {0}, q _ {1} \rangle : q _ {0} \leq p _ {0} \& q _ {0} \| - \hat {q} _ {1} \in \tau \} \in M,
$$

and note that D is dense below $\left. { p _ { 0 } , p _ { 1 } } \right.$ 

Indeed, let $\langle r _ { 0 } , r _ { 1 } \rangle \leq \langle p _ { 0 } , p _ { 1 } \rangle$ and let $G _ { 0 } ^ { \prime }$ be an M-generic filter in $\mathbb { P } _ { 0 }$ containing $r _ { 0 }$ . Then $D _ { 1 } ^ { \prime } = \operatorname { v a l } _ { G _ { 0 } ^ { \prime } } ( \tau )$ is dense in $\mathbb { P } _ { 1 }$ since $r _ { 0 } \le p _ { 0 }$ , and p<sub>0</sub> forces it. Take $q _ { 1 } \leq r _ { 1 }$ with $q _ { 1 } \in D _ { 1 } ^ { \prime }$ and find a $q _ { 0 } \in G _ { 0 } ^ { \prime }$ that forces it: 

$$
q _ {0} \left\| - \hat {q} _ {1} \in \tau . \right.
$$

Since $q _ { 0 }$ and $r _ { 0 }$ belong to the same filter $G _ { 0 } ^ { \prime }$ they are compatible, and taking their common extension, if necessary, we can assume that $q _ { 0 } \leq r _ { 0 }$ But then $\langle q _ { 0 } , q _ { 1 } \rangle \ \leq \ \langle r _ { 0 } , r _ { 1 } \rangle$ and $\langle q _ { 0 } , q _ { 1 } \rangle \in D$ . Thus D is dense below $\langle p _ { 0 } , p _ { 1 } \rangle \in G _ { 0 } \times G _ { 1 }$ 

So we can find $\langle q _ { 0 } , q _ { 1 } \rangle \in D \cap ( G _ { 0 } \times G _ { 1 } )$ . But $q _ { 0 } \in G _ { 0 }$ and q<sub>0</sub> $\Vert - \hat { q } _ { 1 } \in \tau$ Thus $q _ { 1 } \in \mathrm { v a l } _ { G _ { 0 } } ( \tau ) = D _ { 1 }$ , so we have found $q _ { 1 } \in D _ { 1 } \cap G _ { 1 }$ 

To prove that (ii) implies (i) take a dense subset D of $\mathbb { P } _ { 0 } \times \mathbb { P } _ { 1 }$ that belongs to M. We will show that $D \cap ( G _ { 0 } \times G _ { 1 } ) \neq \emptyset$ 

For this, define 

$$
D _ {1} = \left\{p _ {1} \in \mathbb {P} _ {1}: \exists p _ {0} \in G _ {0} (\langle p _ {0}, p _ {1} \rangle \in D) \right\} \in M [ G _ {0} ]
$$

and note that $D _ { 1 }$ is dense in $\mathbb { P } _ { 1 }$ . Indeed, if $r _ { 1 } \in \mathbb { P } _ { 1 }$ then the set 

$$
D _ {0} = \left\{p _ {0} \in \mathbb {P} _ {0}: \exists p _ {1} \leq r _ {1} (\langle p _ {0}, p _ {1} \rangle \in D) \right\} \in M
$$

is dense in $\mathbb { P } _ { 0 }$ and so there exists a $p _ { 0 } \in D _ { 0 } \cap G _ { 0 }$ . Thus there exists a $p _ { 1 } \leq r _ { 1 }$ with $\langle p _ { 0 } , p _ { 1 } \rangle \in D$ and $p _ { 1 } \in D _ { 1 }$ 

Now, by genericity, there exists a $p _ { 1 } \in G _ { 1 } \cap D _ { 1 }$ . So, by the definition of $D _ { 1 }$ , we can find a $p _ { 0 } ~ \in ~ G _ { 0 }$ with $\langle p _ { 0 } , p _ { 1 } \rangle \in D$ . But then $\left. p _ { 0 } , p _ { 1 } \right. ~ \in$ $D \cap ( G _ { 0 } \times G _ { 1 } )$ , that is, $D \cap ( G _ { 0 } \times G _ { 1 } ) \neq \emptyset$ 

Finally, if conditions (i)–(iii) hold then the equation $M [ G _ { 0 } \times G _ { 1 } ] =$ $M [ G _ { 0 } ] [ G _ { 1 } ]$ holds by the minimality of diferent generic extensions. 

To see that $M [ G _ { 0 } \times G _ { 1 } ] \subset M [ G _ { 0 } ] [ G _ { 1 } ]$ note that $G _ { 0 } ~ \in ~ M [ G _ { 0 } ] ~ \subset ~$ $M [ G _ { 0 } ] [ G _ { 1 } ]$ and $G _ { 1 } \in M [ G _ { 0 } ] [ G _ { 1 } ]$ . So $G _ { 0 } \times G _ { 1 } \in M [ G _ { 0 } ] [ G _ { 1 } ]$ . Moreover, 

$M \subset M [ G _ { 1 } ] \subset M [ G _ { 0 } ] [ G _ { 1 } ]$ . Thus, by the minimality of $M [ G _ { 0 } \times G _ { 1 } ]$ , the inclusion holds. 

To see the reverse inclusion note that $M \subset M [ G _ { 0 } \times G _ { 1 } ]$ and $G _ { 0 } \in$ $M [ G _ { 0 } \times G _ { 1 } ]$ . So, by the minimality of $M [ G _ { 0 } ]$ , we have $M [ G _ { 0 } ] \subset M [ G _ { 0 } \times G _ { 1 } ]$ But we have also $G _ { 1 } \in M [ G _ { 0 } \times G _ { 1 } ]$ . Thus $M [ G _ { 0 } ] [ G _ { 1 } ] { \mathrm { ~ \ ' ~ } } { \mathrm { \ ' ~ } }$ by the minimality of $M [ G _ { 0 } ] [ G _ { 1 } ]$ 

The equation $M [ G _ { 0 } \times G _ { 1 } ] = M [ G _ { 1 } ] [ G _ { 0 } ]$ is proved similarly. 

Next, we will see an application of Theorem 9.4.2 to the Cohen model, that is, the model from Section 9.2. 

First note that if $\mathbb { P } ( Z ) = \langle \mathrm { F u n c } _ { \omega } ( Z , 2 ) , \supset \rangle$ and $\{ A , B \}$ is a partition of Z then $\mathbb { P } ( Z )$ is isomorphic to $\mathbb { P } ( A ) \times \mathbb { P } ( B )$ via the isomorphism $i \colon \mathbb { P } ( Z ) \to$ $\mathbb { P } ( A ) \times \mathbb { P } ( B ) , i ( s ) = \langle s | _ { A } , s | _ { B } \rangle$ . Also, if G is a filter in $\mathbb { P } ( Z )$ and $C \subset Z$ then 

$$
G _ {C} = \{s | _ {C}: s \in G \} = G \cap \mathbb {P} (C)
$$

and $i [ G ] = G _ { A } \times G _ { B } = ( G \cap \mathbb { P } ( A ) ) \times ( G \cap \mathbb { P } ( B ) )$ 

Now, if M is a countable transitive model of $\mathrm { Z F C } , Z , A , B \in M$ are such that $\{ A , B \}$ is a partition of $Z ,$ , and G is an M-generic filter in $\mathbb { P } ( Z )$ then, by Theorem 9.4.2, $G _ { A } = G \cap \mathbb { P } ( A )$ is an M-generic filter in $\mathbb { P } ( A )$ $G _ { B } = G \cap \mathbb { P } ( B )$ is an M[G ]-generic filter in $\mathbb { P } ( B )$ , and 

$$
M [ G ] = M [ G _ {A} \times G _ {B} ] = M [ G _ {A} ] [ G _ {B} ].
$$

This fact and the next lemma are powerful tools for proving diferent facts about the Cohen model. 

Lemma 9.4.3 Let M be a countable transitive model of $Z F C , X , Y , Z \in$ M, and G an M-generic filter in $\mathbb { P } ( Z )$ . If $f \colon X \to Y$ is in $M [ G ]$ then there exists an $A \in \mathcal { P } ^ { M } ( Z )$ such that 

$$
M \models | A | \leq | X | + \omega
$$

and $f \in M [ G \cap \mathbb { P } ( A ) ]$ 

Proof By Lemma 9.2.8 we can find a $\mathbb { P } ( Z ) \mathrm { - n a m e } \ \tau \in M$ such that $f =$ $\operatorname { v a l } _ { G } ( \tau ) , \tau \subset \{ \langle \langle \hat { x } , \hat { y } \rangle , p \rangle \colon x \in X \ \& \ y \in Y \ \& \ p \in \mathbb { P } ( Z ) \}$ , and 

(G) $\begin{array} { r l } & { A _ { x } = \{ p \in \mathbb { P } ( Z ) \colon \exists y \in Y ( \langle \overline { { \langle x } , \overline { { y } \rangle } } , p \rangle \in \tau ) \} } \\ & { x \in X . } \end{array}$ is an antichain for every 

So every $A _ { x }$ is countable in $M .$ , since $\mathbb { P } ( Z )$ is ccc in M. Let 

$$
A = \bigcup_ {x \in X} \bigcup_ {p \in A _ {x}} \operatorname{dom} (p).
$$

Then $A \in M , A \subset Z$ , and $| A | \leq | X | + \omega$ in M, since every set $\cup _ { p \in A _ { x } }$ dom(p) is countable in M. To finish the proof it is enough to show that $f \in$ $M [ G \cap \mathbb { P } ( A ) ]$ 

But for every $s = \langle \widehat { \langle x , y \rangle } , p \rangle \in \tau$ we have $p \in A _ { x } \subset \mathbb { P } ( A )$ . Thus 

$$
\tau^ {\star} = \{\langle \widehat {\langle x , y \rangle} ^ {\star}, p \rangle : \langle \widehat {\langle x , y \rangle}, p \rangle \in \tau \} \in M
$$

is a $\mathbb { P } ( A ) \mathrm { - n a m e }$ , where $\widehat { \langle x , y \rangle } ^ { \star }$ is a standard P(A)-name for $\langle x , y \rangle \in M$ . So 

$$
\begin{array}{r c l} f = \mathrm{val} _ {G} (\tau) & = & \{\langle x, y \rangle \colon \exists p \in G (\langle \widehat {\langle x , y \rangle}, p \rangle \in \tau) \} \\ & = & \{\langle x, y \rangle \colon (\exists p \in G \cap \mathbb {P} (A)) (\langle \widehat {\langle x , y \rangle} ^ {\star}, p \rangle \in \tau^ {\star}) \} \\ & = & \mathrm{val} _ {G \cap \mathbb {P} (A)} (\tau^ {\star}) \in M [ G \cap \mathbb {P} (A) ]. \end{array}
$$

This finishes the proof. 

Since every real number is identified with a function $r \colon \omega  2$ , we obtain immediately the following corollary. 

Corollary 9.4.4 Let M be a countable transitive model of $Z F C , Z \in M$ and G be an M-generic filter in $\mathbb { P } ( Z )$ . If $r \in \mathbb { R } ^ { M [ G ] }$ then, in M, there exists a countable subset A of Z such that $r \in M [ G \cap \mathbb { P } ( A ) ]$ 

Our next goal is to prove that Martin’s axiom is false in the Cohen model obtained by the forcing $\mathbb { P } ( Z )$ with $| Z | > \omega _ { 1 }$ . For this, first note that the formula $^ { 6 6 } r$ is a real number,” which is identified with $^ { 6 6 } r$ is a function from $\omega$ into $2 , \ d$ is absolute. So for every countable transitive model M of ZFC we have 

$$
\mathbb {R} ^ {M} = \mathbb {R} \cap M \quad \text { and } \quad [ 0, 1 ] ^ {M} = [ 0, 1 ] \cap M.
$$

In particular, if $M [ G ]$ is any generic extension of M then 

$$
[ 0, 1 ] \cap M, \mathbb {R} \cap M \in M [ G ],
$$

since R $\cap M = \mathbb { R } ^ { M } \in M \subset M [ G ] { \mathrm { ~ a n d ~ } } [ 0 , 1 ] \cap M = [ 0 , 1 ] ^ { M } \in M \subset M [ G ] .$ 

Lemma 9.4.5 Let M be a countable transitive model of $Z F C ,$ let $Z \in { }$ M be countable in M, and let G be an M-generic filter in $\mathbb { P } ( Z )$ . Then $M \cap [ 0 , 1 ] \in M [ G ]$ has Lebesgue measure zero in $M [ G ]$ 

Proof Since the forcings $\mathbb { P } ( Z )$ and $\mathbb { P } ( \omega )$ are isomorphic in M we can assume, by Lemma 9.3.7, that $Z = \omega$ . Also, we will identify numbers from [0, 1] with their binary expansions, that is, functions from $\omega$ into 2. 

For $s \in \mathbb { P } ( \omega )$ let $[ s ] = \{ t \in [ 0 , 1 ] \colon s \subset t \}$ . Notice that the Lebesgue measure of [s] is equal to $l ( [ s ] ) = 2 ^ { - n }$ , where $n = | s |$ . Now let $r = \bigcup G \in 2 ^ { \omega }$ and for $k < \omega$ put 

$$
S _ {k} = \bigcup_ {m > k} [ r | _ {[ 2 ^ {m}, 2 ^ {m + 1})} ].
$$

Notice that 

$$
l (S _ {k}) \leq \sum_ {m > k} l ([ r | _ {[ 2 ^ {m}, 2 ^ {m + 1})} ]) = \sum_ {m > k} 2 ^ {- 2 ^ {m}} \leq \sum_ {m > k} 2 ^ {- m} = 2 ^ {- k}.
$$

Thus the set $\begin{array} { r } { S = \bigcap _ { k < \omega } S _ { k } } \end{array}$ has measure zero. It is enough to prove that $M \cap [ 0 , 1 ] \subset S _ { k }$ for every $k < \omega$ 

So fix $k < \omega$ and $t \in M \cap [ 0 , 1 ]$ and define 

$$
D = \left\{s \in \mathbb {P} (\omega) \colon \exists m > k \left(s | _ {[ 2 ^ {m}, 2 ^ {m + 1})} = t | _ {[ 2 ^ {m}, 2 ^ {m + 1})}\right) \right\} \in M.
$$

It is easy to see that D is dense in $\mathbb { P } ( \omega )$ . Thus, $G \cap D \neq \emptyset$ , that is, there is an $m > k$ such that $r | _ { [ 2 ^ { m } , 2 ^ { m + 1 } ) } = t | _ { [ 2 ^ { m } , 2 ^ { m + 1 } ) }$ . So $t \in [ r | _ { [ 2 ^ { m } , 2 ^ { m + 1 } ) } ] \subset S _ { k }$ .  

Theorem 9.4.6 Let M be a countable transitive model of $Z F C , Z \in M$ uncountable in M, and G an M-generic filter in $\mathbb { P } ( Z )$ . Then, in $M [ G ]$ , the interval $[ 0 , 1 ]$ is a union $o f \omega _ { 1 }$ sets of Lebesgue measure zero. 

Proof First assume that $Z$ has cardinality $\omega _ { 1 }$ in M. Then the forcings $\mathbb { P } ( Z )$ and $\mathbb { P } ( \omega _ { 1 } \times \omega )$ are isomorphic. So, by Lemma 9.3.7, we can assume that $Z = \omega _ { 1 } \times \omega$ 

Now, for every $\xi < \omega _ { 1 }$ 

$$
M [ G ] = M [ G \cap \mathbb {P} ((\omega_ {1} \setminus \{\xi \}) \times \omega) ] [ G \cap \mathbb {P} (\{\xi \} \times \omega) ],
$$

so, by Lemma 9.4.5 used with $M [ G \cap \mathbb { P } \left( ( \omega _ { 1 } \setminus \{ \xi \} \right) \times \omega ) ]$ as a ground model, there exists a set $S _ { \xi } \in M [ G ]$ of Lebesgue measure zero such that 

$$
M [ G \cap \mathbb {P} ((\omega_ {1} \setminus \{\xi \}) \times \omega) ] \cap [ 0, 1 ] \subset S _ {\xi}.
$$

But, by Corollary 9.4.4, for every $r \in M [ G ] \cap [ 0 , 1 ]$ there exists in M a countable subset A of Z with $r \in \ M [ G \cap \mathbb { P } ( A ) ]$ . Hence there exists a $\xi < \omega _ { 1 }$ such that $A \subset ( \omega _ { 1 } \backslash \{ \xi \} ) \times \omega$ and 

$$
r \in M [ G \cap \mathbb {P} (A) ] \subset M [ G \cap \mathbb {P} ((\omega_ {1} \setminus \{\xi \}) \times \omega) ].
$$

Therefore $\begin{array} { r } { M [ G ] \cap [ 0 , 1 ] \subset \bigcup _ { \xi < \omega _ { 1 } } S _ { \xi } } \end{array}$ . This finishes the proof of the case when $M \models | Z | = \omega _ { 1 }$ 

For the general case, take $Z _ { 0 } \in \mathcal { P } ^ { M } ( Z )$ of cardinality $\omega _ { 1 }$ in $M$ . Then $M [ G ] = M _ { 1 } [ G _ { 1 } ]$ , where $M _ { 1 } = M [ G \cap \mathbb { P } ( Z \setminus Z _ { 0 } ) ]$ and $G _ { 1 } = G \cap \mathbb { P } ( Z _ { 0 } )$ is an $M _ { \mathrm { 1 - g e n e r i c } }$ filter in $\mathbb { P } ( Z _ { 0 } )$ . The conclusion of the theorem follows from the first case.  

Corollary 9.4.7 Let M be a countable transitive model of $Z F C$ and assume that $Z \in M$ has cardinality at least $\omega _ { 2 }$ in M. If G is an M-generic filter in $\mathbb { P } ( Z )$ then, in $M [ G ]$ , the interval [0, 1] is a union of less than continuum many sets of Lebesgue measure zero. 

In particular, Martin’s axiom is false in $M [ G ]$ 

Proof Theorem 9.2.13 implies that ${ \mathfrak { c } } > \omega _ { 1 }$ in $M [ G ]$ . Hence, by Theorem 9.4.6, we can conclude the first part of the corollary. The second part follows from the first part and Theorem 8.2.7.  

We will finish this section with an estimation of the size of the continuum in the models obtained by ccc forcing extensions. 

Theorem 9.4.8 Let M be a countable transitive model of $Z F C , \mathbb { P } \in M$ be an infinite ccc forcing in M, and G be an M-generic filter in P. If $\kappa = | \mathbb { P } ^ { \omega } | ^ { \tilde { M } }$ then 

$$
M [ G ] \models \mathfrak {c} \leq \kappa .
$$

Proof Since, by Theorem 9.2.11, the models M and $M [ G ]$ have the same cardinals, we will not distinguish between them. Let $\mathcal { F }$ be the family of all P-names $\tau \subset \{ \langle \bar { \langle n , i \rangle } , p \rangle \colon n \in \omega \ \& \ i \in 2 \ \& \ p \in \mathbb { P } \}$ such that 

(G) $A _ { n } = \{ p \in \mathbb { P } \colon \exists i \in 2 ( \langle \langle n , i \rangle , p \rangle \in \tau ) \} \neq \emptyset$ is an antichain for every $n \in \omega .$ 

Then ${ \mathcal { F } } \in M$ and every $A _ { n }$ is at most countable. 

By Lemma 9.2.8 for every $f \in 2 ^ { \omega } \cap M [ G ]$ we can find a $\tau \in \mathcal { F }$ such that $f = \mathrm { v a l } _ { G } ( \tau )$ . In particular, the image $\operatorname { v a l } _ { G } [ { \mathcal { F } } ]$ of $\mathcal { F }$ under val contains $2 ^ { \omega } \cap M [ G ]$ . So ${ \mathfrak { c } } \leq | { \mathcal { F } } |$ in $M [ G ]$ , and it is enough to prove that $| { \mathcal { F } } | \leq \kappa$ We will show this in M. 

To see it, define in M a map $h \colon ( 2 \times \mathbb { P } ) ^ { \omega \times \omega }  { \mathcal { F } }$ such that for every $t \in ( 2 \times \mathbb { P } ) ^ { \omega \times \omega } { \mathrm { ~ i f ~ } } t ( n , j ) = \langle i _ { n , j } , p _ { n , j } \rangle$ then 

$$
h (t) = \{\langle \langle \widehat {n , i _ {n , j}} \rangle , p _ {n, j} \rangle : n, j \in \omega \}.
$$

Note that h is onto $\mathcal { F }$ , since every set $A _ { n }$ is at most countable. Thus 

$$
| \mathcal {F} | \leq \left| (2 \times \mathbb {P}) ^ {\omega \times \omega} \right| = \kappa .
$$

This finishes the proof. 

Corollary 9.4.9 Let M be a countable transitive model of $Z F C ,$ κ an $i n \textmd { - }$ finite cardinal in M, and $G$ an M-generic filter in $\mathbb { P } ( \kappa )$ . If $\kappa = | \kappa ^ { \omega } | ^ { M }$ then 

$$
M [ G ] \models \mathfrak {c} = \kappa .
$$

In particular, if CH holds in M and $\boldsymbol { \kappa } = \omega _ { 2 } ^ { M } \ t h e n \ { \mathfrak { c } } ^ { M [ G ] } = \omega _ { 2 } ^ { M [ G ] }$ 

Proof First note that $\left| \mathbb { P } ( \kappa ) \right| = \kappa$ , and so $\kappa = | \kappa ^ { \omega } | ^ { M } = | \mathbb { P } ( \kappa ) ^ { \omega } | ^ { M }$ . Thus, by Theorem 9.4.8, ${ \mathfrak { c } } ^ { M [ G ] } \leq { \mathfrak { r } }$ . The other inequality for $\kappa = \omega _ { 2 }$ follows from Theorem 9.2.13. The general case is left as an exercise. 

To see the additional part note that under CH the regularity of $\omega _ { 2 }$ implies 

$$
\omega_ {2} \leq \omega_ {2} ^ {\omega} = \left| \bigcup_ {\xi <   \omega_ {2}} \xi^ {\omega} \right| = \omega_ {2} \otimes \omega_ {1} ^ {\omega} = \omega_ {2} \otimes \mathfrak {c} ^ {\omega} = \omega_ {2} \otimes \mathfrak {c} = \omega_ {2} \otimes \omega_ {1} = \omega_ {2}.
$$

So, under CH, $\kappa = \omega _ { 2 }$ satisfies the assumptions of the main part of the corollary.  

## EXERCISES

1 Complete the proof of Proposition 9.4.1. 

2 Show that the set D from the proof of Lemma 9.4.5 is indeed dense in $\mathbb { P } ( \omega )$ 

3 Complete the proof of Corollary 9.4.9 for arbitrary κ by showing that ${ \mathfrak { c } } ^ { M [ G ] } \geq \kappa$ 

4 Let M be a countable transitive model of $\mathrm { Z F C } , \mathbb { P } \in M$ a partially ordered set, and G an M-generic filter in P. Prove that $M [ G ]$ and M have the same ordinal numbers. 

## 9.5 Model for MA+¬CH

The goal of this section is to prove the consistency of $\mathrm { M A } + { } ^ {  } { \mathfrak { c } } = \omega _ { 2 } . { } ^ {  }$ For this, we will follow the idea mentioned at the beginning of the previous section. We will start with a countable transitive model M of $\mathrm { Z F C + ^ {  1 } 2 ^ { \omega _ { 1 } } } \mathrm { = } { \omega _ { 2 } }$ ,” which exists by Corollary 9.3.9, and find its generic extension N via a ccc forcing $\mathbb { P } _ { \mu } \in M$ for which there exists a sequence 

$$
M = M _ {0} \subset M _ {1} \subset \dots \subset M _ {\xi} \subset \dots \subset M _ {\mu} = N
$$

with $\mu = \omega _ { 2 } ^ { M } = \omega _ { 2 } ^ { N }$ and the following properties: 

P1 $M _ { \xi + 1 } = M _ { \xi } [ G ^ { \xi } ]$ for every $\xi < \mu$ , where $G ^ { \xi }$ is an $M _ { \xi ^ { - } } \mathrm { g e n e r i c }$ filter in some forcing $\mathbb { P } ^ { \xi } \in M _ { \xi }$ 

P2 For every $Y \in M$ and $S \subset Y$ with $N \left| = | S | < \omega _ { 2 } \right.$ there exists an $\alpha < \mu$ such that $S \in M _ { \alpha }$ 

P3 $| ( \mathbb { P } _ { \mu } ) ^ { \omega } | ^ { M } \leq \omega _ { 2 } ^ { M }$ 

P4 For every forcing $\langle \lambda , \ll \rangle \in N$ such that 

$N \models \mathit { \Omega } ( \lambda $ is an ordinal number, $\lambda \leq \omega _ { 1 }$ , and $\langle \lambda , \ll \rangle$ is ccc) 

and every $\alpha < \mu$ there is a $\xi < \mu$ , with $\xi > \alpha$ , such that $\mathbb { P } ^ { \xi } = \langle \lambda , \ll \rangle$ 

To argue that P1–P4 imply $N ~ \models ~ \mathrm { M A } + { } ^ { \ast } { \mathfrak { c } } ~ = ~ \omega _ { 2 } { } ^ { , , }$ we also need the following definitions and lemma. For an uncountable cardinal number κ and a partially ordered set P we will write $\mathrm { M A } _ { \kappa } ( \mathbb { P } )$ to denote the statement 

$\mathbf { M A } _ { \kappa } ( \mathbb { P } )$ For every family D of dense subsets of P such that $| \mathcal { D } | < \kappa$ there exists a D-generic filter F in P. 

We will also use the symbol $\mathrm { M A } _ { \kappa }$ for the statement that $\mathrm { M A } _ { \kappa } ( \mathbb { P } )$ holds for every ccc forcing P. Thus MA is equivalent to MA . 

Lemma 9.5.1 For an uncountable cardinal number κ the following statements are equivalent: 

(i) $\mathrm { M A } _ { \kappa _ { 1 } }$ 

(ii) $\mathrm { M A } _ { \kappa } ( \mathbb { P } )$ holds for every ccc forcing $\mathbb { P } = \langle P , \leq \rangle$ with $| P | < \kappa$ ; 

(iii) $\mathrm { M A } _ { \kappa } ( \mathbb { P } )$ holds for every ccc forcing $\mathbb { P } = \langle \lambda , \ll \rangle$ , where λ is a cardinal number less than κ. 

Before we prove Lemma 9.5.1 let us see how it can be used to conclude $N \Vdash \mathrm { M A ^ { + } } ^ { * } { \mathfrak { c } } = \omega _ { 2 } { \ } ^ { , , }$ from $\mathrm { P 1 { - } P 4 }$ 

First, we will prove that 

$$
N \models \mathrm{MA} _ {\omega_ {2}}.\tag{9.7}
$$

By Lemma 9.5.1 it is enough to show in N that $\mathrm { M A } _ { \omega _ { 2 } } ( \mathbb { P } )$ holds for every ccc forcing $\mathbb { P } = \langle \lambda , \ll \rangle$ with λ being an ordinal number less than or equal to $\omega _ { 1 } ^ { N }$ . For this, let $\langle \lambda , \ll \rangle \ \in \ N$ be ccc in N with $\lambda \ \leq \ \omega _ { 1 } ^ { N }$ , and let $\mathcal { D } = \bar { \{ D \xi : \xi < \omega _ { 1 } ^ { N } \} } \in N$ be a family of dense subsets of $\langle \lambda , \ll \rangle$ . Since $\mathbb { P } _ { \mu }$ is ccc we have $\bar { \lambda } \le \omega _ { 1 } ^ { N } = \omega _ { 1 } ^ { M }$ , and $\ll$ as well as $U _ { \xi < \omega _ { 1 } ^ { M } } \{ \xi \} \times D _ { \xi }$ are subsets of $\omega _ { 1 } ^ { M } \times \omega _ { 1 } ^ { M } \in M$ <sub>. Hence, by P2, there exists an</sub> $\alpha < \mu$ such that $\langle \lambda , \leq \rangle , { \mathcal { D } } \in M _ { \alpha }$ . Moreover, by P4 there exists $\alpha < \xi < \mu$ with $\mathbb { P } ^ { \xi } = \langle \lambda , \ll \rangle$ In particular, $G ^ { \xi } \in M _ { \xi + 1 }$ is an $M _ { \xi ^ { - } } \mathrm { g e n e r i c }$ filter in $\mathbb { P } ^ { \xi } = \langle \lambda , \ll \rangle$ But $\mathcal { D } \subset M _ { \alpha } \subset M _ { \xi }$ . So $G ^ { \xi }$ is also D-generic in $\langle \lambda , \ll \rangle$ . Condition $( 9 . 7 )$ has been proved. 

Now $\mathrm { M A } _ { \omega _ { 2 } }$ and ${ \mathfrak { c } } = \omega _ { 2 }$ clearly imply MA. Thus, it is enough to argue that $N ~ \models \{ \mathfrak { c }  = \omega _ { 2 }$ . But the inequality ${ \mathfrak { c } } ^ { N } \leq \omega _ { 2 } ^ { N }$ follows from P3 and Theorem 9.4.8. The other inequality follows from the fact that 

$$
\mathrm{MA} _ {\omega_ {2}} \Rightarrow \forall G \in [ 2 ^ {\omega} ] ^ {\leq \omega_ {1}} \exists f \in 2 ^ {\omega} \setminus G.\tag{9.8}
$$

To see it, put $\mathbb { P } ( \omega ) = \langle \mathrm { F u n c } _ { \omega } ( \omega , 2 ) , \supset \rangle$ and for every $g \in 2 ^ { \omega }$ define $D _ { g } = $ $\{ s \in \mathbb { P } ( \omega ) \colon s \not \subset g \}$ . Then the sets $D _ { g }$ are dense in $\mathbb { P } ( \omega )$ Let $F$ be a $\{ D _ { g } \colon g \in G \}$ -generic filter in $\mathbb { P } ( \omega )$ . Then any extension of $\cup F$ to a function $f \colon \omega  2$ will have the desired property. The details are left as an exercise. 

Before we move to the technical aspects of the construction, it is worthwhile to reflect for a moment on the idea behind the foregoing argument. It is clearly of the transfinite-induction nature and the argument is of a diagonal character. Condition P1 represents an inductive step in which we take care of “one problem at a time.” Condition P2 represents a kind of closure argument. It tells us that the “small objects” from N can already be found in the earlier steps of our construction and thus we will have a chance to “take care of them” in the later part of the induction. 

The construction of the forcing $\mathbb { P } _ { \mu }$ leading to a model satisfying P1 and P2 is of a very general nature and can be compared to the recursion theorem. The specific aspects of our model are addressed mainly by condition P4, with Lemma 9.5.1 allowing us to reduce the induction to one of reasonably short length. 

This construction closes, in a way, a full circle that we have made in this course. We started with simple recursion proofs. Next, when the dificulties with the length of induction mounted, we started to use refined recursive arguments by introducing additional axioms such as CH, $\diamondsuit ,$ and MA. This led us all the way to the forcing arguments of the previous sections, and finally to finish here by coming back to a relatively simple transfiniteinduction argument. 

The preceding argument shows that in order to prove the consistency of $\mathrm { M A } + { } ^ {  } { \mathfrak { c } } = \omega _ { 2 } { } ^ {  }$ it is enough to prove Lemma 9.5.1 and find a generic extension N of M satisfying P1–P4. We will start with Lemma 9.5.1. 

Proof of Lemma 9.5.1 Clearly $( \mathrm { i } ) { \Rightarrow } ( \mathrm { i i i } )$ . Thus it is enough to show $( \mathrm { i i i } ) { \Rightarrow } ( \mathrm { i i } )$ and $( \mathrm { i i } ) { \Rightarrow } ( \mathrm { i } )$ 

$( \mathrm { i i } ) { \Rightarrow } ( \mathrm { i } )$ : Let $\mathbb { P } = \langle P , \leq \rangle$ be a ccc partially ordered set and let D be a family of dense subsets of P such that $| \mathcal { D } | < \kappa$ . Choose a function $f \colon P \times P \to P$ such that $f ( p , q )$ extends p and $q$ provided $p$ and $q$ are compatible in P, and for every $D \in \mathcal { D }$ pick $f _ { D } \colon P \to D$ such that $f _ { D } ( p ) \leq p$ for every $p \in P$ . Let $p _ { 0 } \in \mathbb { P }$ and let $Q$ be the smallest subset of P containing $p _ { 0 }$ and being closed under the operations f and $f _ { D }$ for every $D \in \mathcal { D }$ . Thus 

$$
Q = \bigcup_ {n <   \omega} Q _ {n},
$$

where $Q _ { 0 } = \{ p _ { 0 } \}$ and $\begin{array} { r } { Q _ { n + 1 } = Q _ { n } \cup f [ Q _ { n } \times Q _ { n } ] \cup \bigcup _ { D \in \mathcal { D } } f _ { D } [ Q _ { n } ] } \end{array}$ (compare with Lemma 6.1.6). Then $| Q | \leq | D | + \omega < \kappa .$ 

Note that any p, $q \in Q$ that are compatible in $\mathbb { P }$ are also compatible in $\mathbb { P } _ { 0 } = \langle Q , \leq \rangle$ , since $Q$ is closed under the action of $f .$ . Thus $\mathbb { P } _ { 0 }$ is ccc and, by (ii), $\mathrm { M A } _ { \kappa } ( \mathbb { P } _ { 0 } )$ holds. But, by the closure of $Q$ under the action of $f _ { D }$ , for every $D \in { \mathcal { D } }$ the set $D \cap Q$ is dense in $\mathbb { P } _ { 0 }$ . So there exists a $\{ D \cap Q \colon D \in { \mathcal { D } } \}$ -generic filter $F _ { 0 }$ in $\mathbb { P } _ { 0 }$ . To finish the proof it is enough to notice that $F = \{ p \in P \colon \exists q \in F _ { 0 } ~ ( q \leq p ) \}$ is a D-generic filter in P. The details are left as an exercise. 

$( \mathrm { i i i } ) { \Rightarrow } ( \mathrm { i i } )$ : The proof is very similar to that of Lemma 9.3.7. To see ${ \mathrm { i t } } ,$ let $\mathbb { P } = \langle P , \leq \rangle$ be a ccc partially ordered set such that $\lambda = | P | < \kappa$ and let D be a family of dense subsets of $\mathbb { P }$ such that $| \mathcal { D } | < \kappa$ . Choose a bijection $f$ between λ and $P$ and define a partial-order relation $\ll$ on λ by putting 

$$
\alpha \ll \beta \Leftrightarrow f (\alpha) \leq f (\beta).
$$

Notice that $f$ is an order isomorphism between $\mathbb { P } _ { 0 } = \langle \lambda , \ll \rangle$ and $\mathbb { P } =$ $\langle P , \leq \rangle$ . In particular, $f ^ { - 1 } ( D )$ is dense in $\mathbb { P } _ { 0 }$ for every $D \in { \mathcal { D } } .$ . So $\mathcal { D } _ { 0 } =$ $\{ f ^ { - 1 } ( D ) \colon D \in { \mathcal { D } } \}$ is a family of dense subsets of $\mathbb { P } _ { 0 }$ and $\left. \mathcal { D } _ { 0 } \right. = \left. \mathcal { D } \right. < \kappa$ Hence, by (iii), there exists a $\mathcal { D } _ { 0 } . mathrm { g e n e r i c }$ filter $F _ { 0 }$ in $\mathbb { P } _ { 0 }$ . To finish the proof it is enough to notice that $f [ F _ { 0 } ]$ is a D-generic filter in P. The details are left as an exercise.  

To find a model N satisfying P1–P4 we first need to come back to the problem of expressing a model obtained by two consecutive generic extensions as a single generic extension. More precisely, if $M _ { 1 } = M [ G _ { 0 } ]$ where $G _ { 0 }$ is an M-generic filter in $\mathbb { P } _ { 0 } \in M$ , and $M _ { 2 } = M [ G _ { 0 } ] [ G _ { 1 } ]$ , where $G _ { 1 }$ is an $M [ G _ { 0 } ]$ -generic filter in $\mathbb { P } _ { 1 } \in M [ G _ { 0 } ]$ , we would like to find a $\mathbb { P } \in M$ and an M-generic filter $G$ in P such that $M _ { 2 } = M [ G ]$ . The product lemma (Theorem 9.4.2) gives a solution to this problem when $\mathbb { P } _ { 1 } \in M$ . Thus, we will concentrate here on the case when $\mathbb { P } _ { 1 } \in M [ G _ { 0 } ] \backslash M$ . To define such $\mathbb { P }$ we need the following definition. 

A pair $\langle \pi , \sigma \rangle \in M$ of P-names satisfying the condition 

$$
\mathbb {P} \left\| - \sigma \right. \text { is   a   partial - order   relation   on } \pi\tag{9.9}
$$

will be called a good P-name for a partially ordered set. (Note that, formally speaking, a good P-name is not a P-name.) If $\langle \pi , \sigma \rangle$ is a good P-name for a partially ordered set we will often write $\pi$ for $\langle \pi , \sigma \rangle$ 

The following lemma tells us that any forcing $\mathbb { P } _ { 1 }$ in $M [ G _ { 0 } ]$ has a good $\mathbb { P } _ { 0 } { \mathrm { - n a m e } }$ representing it. So it explains the restriction of our attention to good names only. However, the lemma will not be used in what follows, so we will leave it without a proof. 

Lemma 9.5.2 Let M be a countable transitive model of $Z F C , \mathbb { P } \in M$ a partially ordered set, and $G _ { 0 }$ an M-generic filter in P. If $\mathbb { P } _ { 1 } = \langle P , \leq \rangle \in$ $M [ G _ { 0 } ]$ is a partially ordered set in $M [ G _ { 0 } ]$ then there are P-names π, $\sigma \in M$ satisfying (9.9) and such that $\langle P , \leq \rangle = \langle \mathrm { v a l } _ { G _ { 0 } } ( \pi ) , \mathrm { v a l } _ { G _ { 0 } } ( \sigma ) \rangle$ 

Now let $\mathbb { P }$ be a partially ordered set and $\langle \pi , \leq _ { \pi } \rangle$ be a good P-name for a partially ordered set. Then their iteration $\mathbb { P } \star \pi$ is defined by 

$$
\mathbb {P} \star \pi = \{\langle p, \tau \rangle : p \in \mathbb {P} \& \tau \in \operatorname{dom} (\pi) \& p \| - \tau \in \pi \}.
$$

Moreover, on $\mathbb { P } \star \pi$ we define a binary relation $\preceq$ by 

$$
\langle p, \tau \rangle \preceq \langle q, \sigma \rangle \quad \Leftrightarrow \quad p \leq q \& p \| - \tau \leq_ {\pi} \sigma .
$$

Notice that the relation $\preceq$ is reflexive and transitive on $\mathbb { P } \star \pi$ . It is reflexive since for any $\langle p , \tau \rangle \in \mathbb { P } \star \pi$ condition $p$ forces $\tau \in \pi$ and $\leq _ { \pi }$ to be a partial-order relation on $\pi$ (since $\langle \pi , \leq _ { \pi } \rangle$ is good). The proof that $\preceq$ is transitive is left as an exercise. 

Unfortunately, $\preceq$ does not have to be antisymmetric on $\mathbb { P } \star \pi$ . To solve this problem, we notice that the relation $\sim$ on $\mathbb { P } \star \pi$ defined by 

$$
\langle p, \tau \rangle \sim \langle q, \sigma \rangle \Leftrightarrow \langle p, \tau \rangle \preceq \langle q, \sigma \rangle \& \langle q, \sigma \rangle \preceq \langle p, \tau \rangle
$$

is an equivalence relation on $\mathbb { P } \star \pi$ (see Exercise 4 from Section 2.4). Thus, in order to consider $\langle \mathbb { P } \star \pi , \preceq \rangle$ as a partially ordered set, we will identify the elements of $\mathbb { P } \star \pi$ that are ∼-equivalent. (Formally, we should replace $\mathbb { P } \star \pi$ by the quotient class $\mathbb { P } \star \pi / { } _ { \sim }$ and the relation $\preceq$ by the quotient relation $\leq \mathrm { d e f i n e d }$ as in part (b) of Exercise 4 in Section 2.4. However, this would obscure the clarity of the “simple-identification” approach.) Upon such an identification we will consider $\mathbb { P } \star \pi$ as a partially ordered set. 

Let us also notice that if the partially ordered sets $\mathbb { P } _ { 0 }$ and $\mathbb { P } _ { 1 }$ are in the ground model M and π and $\leq _ { \pi }$ are the standard P -names for $\mathbb { P } _ { 1 }$ and its order relation then $\langle \pi , \leq _ { \pi } \rangle$ is a good name for a partially ordered set and 

$$
\mathbb {P} _ {0} \star \pi \text { is   isomorphic   to } \mathbb {P} _ {0} \times \mathbb {P} _ {1}.\tag{9.10}
$$

Thus the process of iteration is truly a generalization of the product of forcings as described in the previous section. To formulate an iteration analog of the product lemma, we need one more definition. 

Let M be a countable transitive model of $\mathrm { Z F C } , \mathbb { P } _ { 0 } \in M$ be a partially ordered set, and $G _ { 0 }$ be an M-generic filter in $\mathbb { P } _ { 0 }$ . If $\pi$ is a good $\mathbb { P } _ { 0 } \mathrm { - n a m e }$ for a partially ordered set and $G _ { 1 } \subset \mathrm { v a l } _ { G _ { 0 } } ( \pi )$ then we define 

$$
G _ {0} \star G _ {1} = \{\langle p, \tau \rangle \in \mathbb {P} _ {0} \star \pi : p \in G _ {0} \& \operatorname{val} _ {G _ {0}} (\tau) \in G _ {1} \}.
$$

Theorem 9.5.3 Let M be a countable transitive model of ZFC and $\mathbb { P } _ { 0 } \star \pi$ be an iteration of a partially ordered set $\mathbb { P } _ { 0 } ~ \in ~ M$ and a good $\mathbb { P } _ { 0 } { - } n a m e$ $\pi \in M$ for a partially ordered set. $I f G$ is an M-generic filter in $\mathbb { P } _ { 0 } \star \pi$ and 

$$
G _ {0} = \{p \in \mathbb {P} _ {0} \colon \exists \langle q, \tau \rangle \in G (q \leq p) \}
$$

then $G _ { 0 }$ is an M-generic filter in $\mathbb { P } _ { 0 }$ . Moreover, if 

$$
G _ {1} = \{\mathrm{val} _ {G _ {0}} (\tau) \colon \langle q, \tau \rangle \in G \}
$$

then $G _ { 1 }$ is an $M [ G _ { 0 } ]$ ]-generic filter in $\mathbb { P } _ { 1 } = \operatorname { v a l } _ { G _ { 0 } } ( \pi ) , G = G _ { 0 } \star G _ { 1 }$ , and $M [ G ] = M [ G _ { 0 } ] [ \bar { G _ { 1 } } ]$ 

Proof It is easy to see that $G _ { 0 }$ is a filter in $\mathbb { P } _ { 0 }$ . To show that $G _ { 0 }$ is $M -$ generic take a $D _ { 0 } \in M$ that is dense in P .Then $D = \{ \langle p , \tau \rangle \in \mathbb { P } _ { 0 } \star \pi \colon p \in D _ { 0 } \}$ is dense in $\mathbb { P } _ { 0 } { \star } \pi$ , since $\langle p , \tau \rangle \preceq \langle q , \tau \rangle$ and $\langle p , \tau \rangle \in D$ for every $\langle q , \tau \rangle \in \mathbb { P } _ { 0 } { \star } \pi$ and $p \in D _ { 0 }$ with $p \leq q .$ . Take $\langle p , \tau \rangle \in G \cap D$ . Then $p \in G _ { 0 } \cap D _ { 0 }$ . Thus $G _ { 0 }$ is an M-generic filter in $\mathbb { P } _ { 0 }$ 

Next, we will show that $G _ { 1 }$ is a filter in $\mathbb { P } _ { 1 }$ . So take $\mathrm { v a l } _ { G _ { 0 } } ( \tau ) \in G _ { 1 }$ with $\langle q , \tau \rangle \in G$ witnessing it and let $\sigma \in \mathrm { d o m } ( \pi )$ be such that $\operatorname { v a l } _ { G _ { 0 } } ( \sigma ) \in \mathbb { P } _ { 1 }$ and va $\begin{array} { r } { { \mathrm { l } } _ { G _ { 0 } } ( \tau ) \le { \mathrm { v a l } } _ { G _ { 0 } } ( \sigma ) } \end{array}$ . We will show that $\operatorname { v a l } _ { G _ { 0 } } ( \sigma ) \in G _ { 1 }$ . For this, take $p _ { 0 } \in G _ { 0 }$ with $p _ { 0 } \parallel - \tau \le \sigma$ and $\langle p , \rho \rangle \in G$ such that $p \leq p _ { 0 }$ . Pick $\langle r , \eta \rangle \in G$ with $\langle r , \eta \rangle \preceq \langle q , \tau \rangle$ and $\langle r , \eta \rangle \preceq \langle p , \rho \rangle$ . Then $r \parallel - \eta \le \tau$ and $r \parallel - \tau \leq \sigma ;$ since $r \le p _ { 0 }$ . So $r \parallel - \eta \le \sigma$ , and $\langle r , \eta \rangle \preceq \langle r , \sigma \rangle$ . Hence $\langle r , \sigma \rangle \in G$ and $\operatorname { v a l } _ { G _ { 0 } } ( \sigma ) \in G _ { 1 }$ 

To see that any two elements of $G _ { 1 }$ have a common extension in $G _ { 1 }$ take $\mathrm { v a l } _ { G _ { 0 } } ( \tau ) \in G _ { 1 }$ with $\langle q , \tau \rangle \in G$ and va $_ { G _ { 0 } } ( \sigma ) \in G _ { 1 }$ with $\langle p , \sigma \rangle \in G$ Then there exists $\langle r , \eta \rangle \in G$ such that $\langle r , \eta \rangle \preceq \langle q , \tau \rangle$ and $\langle r , \eta \rangle \preceq \langle p , \sigma \rangle$ . So $r \in G _ { 0 }$ and $r \ \lVert - \ ( \eta \leq \tau \ \& \ \eta \leq \sigma )$ . Thus $\mathrm { v a l } _ { G _ { 0 } } ( \eta ) \in G _ { 1 }$ extends $\mathrm { v a l } _ { G _ { 0 } } ( \tau )$ and $\mathrm { v a l } _ { G _ { 0 } } ( \sigma )$ 

For the proof that $G _ { 1 }$ is $M [ G _ { 0 } ] \mathrm { - g e n e r i c }$ in $\mathbb { P } _ { 1 }$ take a $D _ { 1 } \in M [ G _ { 0 } ]$ that is dense in $\mathbb { P } _ { 1 }$ and let $\delta$ be a $\mathbb { P } _ { 0 } \mathrm { - n a m e }$ such that $D _ { 1 } = \operatorname { v a l } _ { G _ { 0 } } ( \delta )$ . Pick $p \in G _ { 0 }$ that forces it, that is, 

$p \Vdash \delta$ is a dense subset of $\pi .$ , 

and define 

$$
D = \{\langle q, \tau \rangle \in \mathbb {P} _ {0} \star \pi : q \| - \tau \in \delta \}.\tag{9.11}
$$

Now, if $\langle q , \eta \rangle \in G$ is such that $q \leq p$ then it is easy to see that D is dense below $\langle q , \eta \rangle$ (the proof is left as an exercise). So there exists $\langle r , \tau \rangle \in D \cap G$ and $\mathrm { v a l } _ { G _ { 0 } } ( \tau ) \in D _ { 1 } \cap G _ { 1 }$ 

To argue that $G = G _ { 0 } { \star } G _ { 1 }$ take $\langle p , \tau \rangle \in G$ . Then $p \in G _ { 0 }$ and $\mathrm { v a l } _ { G _ { 0 } } ( \tau ) \in$ $G _ { 1 }$ by the definitions of $G _ { 0 }$ and $G _ { 1 }$ . So $G \subset G _ { 0 } \star G _ { 1 }$ . To see the other inclusion, take $\langle p , \tau \rangle \in G _ { 0 } \star G _ { 1 } \subset \mathbb { P } _ { 0 } \star \pi$ . Then $p \in G _ { 0 }$ and va $\mathrm { l } _ { G _ { 0 } } ( \tau ) \in G _ { 1 }$ So there exist $\langle q , \sigma \rangle \in G ,$ with $q \leq p .$ , and $\langle r , \tau \rangle \in G$ . Let $\langle s , \eta \rangle \in G$ be a common extension of $\langle q , \sigma \rangle$ and $\langle r , \tau \rangle$ . Then $s \leq q \leq p$ and $s \parallel - \eta \le \tau$ . So $\langle s , \eta \rangle \preceq \langle p , \tau \rangle$ and $\langle p , \tau \rangle \in G$ 

Finally, $G _ { 0 } , G _ { 1 } \in M [ G ]$ , as they are defined using G. So $M [ G _ { 0 } ] \subset M [ G ]$ by the minimality of $M [ G _ { 0 } ]$ , and $M [ G _ { 0 } ] [ G _ { 1 } ] \subset M [ { \bar { G } } ]$ by the minimality of $\dot { M } [ G _ { 0 } ] [ G _ { 1 } ]$ . Also, $G = G _ { 0 } \star G _ { 1 } \in M [ G _ { 0 } ] [ G _ { 1 } ]$ . So ${ \dot { M } } [ { \dot { G } } ] \subset M [ G _ { 0 } ] [ G _ { 1 } ]$  

Theorem 9.5.3 is an analog of the implication $( \mathrm { i } ) { \Rightarrow } ( \mathrm { i i } )$ from the product lemma. The iteration analog of the reverse implication, stated next, is also true. However, since we will not use this fact, we will leave its proof as an exercise. 

Theorem 9.5.4 Let M be a countable transitive model of $Z F C , G _ { 0 }$ an $M -$ generic filter in $\mathbb { P } _ { 0 } \in M$ , and $G _ { 1 }$ an M[G ]-generic filter in $\mathbb { P } _ { 1 } \in M [ G _ { 0 } ]$ If $\pi \in M$ is a good $\mathbb { P } _ { 0 } - n a m e$ representing $\mathbb { P } _ { 1 }$ then $G _ { 0 } \star G _ { 1 }$ is an M-generic filter in $\mathbb { P } _ { 0 } \star \pi$ and $M [ G _ { 0 } ] [ G _ { 1 } ] = M [ G _ { 0 } \star G _ { 1 } ]$ 

In the proof of the consistency of $\mathrm { M A } { + } { \lnot \mathrm { C H } }$ we will be interested only in the ccc forcings. The next lemma tells us that we will remain within this class if the iteration concerns two ccc forcings. 

Lemma 9.5.5 Let M be a countable transitive model of $Z F C , \mathbb { P } _ { 0 } \in M$ be a ccc forcing in M, and $\langle \pi , \leq _ { \pi } \rangle$ be a good $\mathbb { P } _ { 0 } { - } n a m e$ for a forcing such that 

$$
\mathbb {P} _ {0} \left\| - \langle \pi , \leq_ {\pi} \right\rangle i s c c c.\tag{9.12}
$$

Then $\mathbb { P } _ { 0 } \star \pi$ is ccc in M. 

Proof To obtain a contradiction assume that there exists an uncountable antichain $A = \{ \langle p _ { \xi } , \tau _ { \xi } \rangle \colon \xi < \omega _ { 1 } \} \in M$ in $\mathbb { P } _ { 0 } \star \pi$ . Let 

$$
\sigma = \{\langle \hat {\xi}, p _ {\xi} \rangle : \xi <   \omega_ {1} \}.
$$

Then $\sigma \in M$ is a P -name. Define, in M, 

$$
D = \{p \in \mathbb {P} _ {0} \colon \exists \beta <   \omega_ {1} (p \| - \sigma \subset \hat {\beta}) \}
$$

and notice that D is dense in $\mathbb { P } _ { 0 }$ . 

To see this, let $q \in \mathbb { P } _ { 0 }$ and let H be an M-generic filter containing q. Then 

$$
S = \operatorname{val} _ {H} (\sigma) = \{\xi <   \omega_ {1} \colon p _ {\xi} \in H \}.
$$

Notice that for distinct $\xi , \eta \in S$ the conditions va ${ } _ { H } ( \tau _ { \xi } )$ and va ${ \bf \Gamma } _ { H } ( \tau _ { \eta } )$ are incompatible in va $_ { H } ( \pi )$ 

Indeed, if $\xi , \eta \in S , \xi \neq \eta$ , and val ${ } _ { H } ( \tau _ { \xi } )$ and val ${ \bf \Gamma } _ { H } ( \tau _ { \eta } )$ are compatible in $\operatorname { v a l } _ { H } ( \pi )$ then there are $r \in H$ extending $p _ { \xi }$ and $p _ { \eta }$ and $\rho \in \mathrm { d o m } ( \pi )$ such that $r \parallel - \rho \le _ { \pi } \tau _ { \xi }$ and $r \parallel - \rho \le _ { \pi } \tau _ { \eta }$ . But then $\langle r , \rho \rangle$ would be a common extension of $\langle p _ { \xi } , \tau _ { \xi } \rangle$ and $\langle p _ { \eta } , \tau _ { \eta } \rangle$ , contradicting our assumption that A is an antichain. 

Thus $S$ is countable in $M [ H ]$ since, by (9.12), val $\mathbf { } _ { H } ( \pi )$ is ccc in $M [ H ]$ So there exists a $\beta < \omega _ { 1 }$ containing $S$ . Now, if $p \in H$ is such that $p \leq q$ and $p \parallel - S \subset { \hat { \boldsymbol { \beta } } }$ then $p \in D$ . So D is dense. 

Next consider the set 

$$
T = \{\beta <   \omega_ {1} \colon \exists p _ {\beta} \in \mathbb {P} _ {0} (p _ {\beta} \| - \sup \sigma = \hat {\beta}) \}
$$

and notice that $A _ { 1 } = \{ p _ { \beta } \colon \beta \in T \}$ is an antichain in $\mathbb { P } _ { 0 }$ . Thus $A _ { 1 }$ and $T$ are countable in M. Let $\gamma < \omega _ { 1 }$ be such that $T \subset \gamma$ . Then the set 

$$
D ^ {\prime} = \{p \in \mathbb {P} _ {0} \colon p \| - \sigma \subset \hat {\gamma} \}
$$

is dense in $\mathbb { P } _ { 0 }$ , since it contains $D$ . 

Now, to obtain a contradiction, take an M-generic filter H in $\mathbb { P } _ { 0 }$ containing $p _ { \gamma }$ . Then, by the denseness of $D ^ { \prime }$ , $\operatorname { v a l } _ { H } ( \sigma ) \subset \gamma$ . But, straight from the definition of $\sigma , \gamma \in \operatorname { v a l } _ { H } ( \sigma ) !$ This contradiction finishes the proof.  

Now we turn our attention to the α-stage iteration for an arbitrary ordinal number $\alpha .$ More precisely, we will describe a general method of defining inductively a sequence $P = \langle \langle \mathbb { P } _ { \xi } , \leq _ { \xi } \rangle \colon \xi \leq \alpha \rangle$ of forcings such that $\mathbb { P } _ { \xi + 1 }$ can be identified with $\mathbb { P } _ { \xi } \star \pi _ { \xi }$ , where $\pi _ { \xi }$ is a good $\mathbb { P } _ { \xi ^ { - } } \mathrm { n a m e }$ for a partially ordered set. This, with help of Theorem 9.5.3, will take care of the condition P1. The technical dificulty in this construction is that we have to know $\mathbb { P } _ { \xi }$ in order to talk about a good $\mathbb { P } _ { \xi ^ { - } } \mathrm { n a m e } \ \pi _ { \xi }$ . So, along with the sequence $P _ { \cdot }$ we have to construct a sequence $\Pi = \langle \langle \bar { \pi } _ { \xi } , \leq _ { \pi _ { \xi } } \rangle \colon \xi < \alpha \rangle$ of appropriate good $\mathbb { P } _ { \xi ^ { - } \mathrm { n a m e s } . }$ This obscures a simple idea that stands behind the construction. Thus we will first describe this construction with the sequence Π replaced by a sequence $\langle \langle Q _ { \xi } , \leq _ { Q _ { \xi } } \rangle \colon \xi < \alpha \rangle$ of forcings. In this case for every $\beta \leq \alpha$ we define 

$$
\mathbb {P} _ {\beta} = \bigcup \left\{\prod_ {\eta \in S} Q _ {\eta}: S \in [ \beta ] ^ {<   \omega} \right\} = \left\{f | _ {S}: f \in \prod_ {\eta <   \beta} Q _ {\eta} \& S \in [ \beta ] ^ {<   \omega} \right\}\tag{9.13}
$$

and order it by 

$$
p \leq_ {\beta} q \Leftrightarrow \operatorname{dom} (q) \subset \operatorname{dom} (p) \& (\forall \eta \in \operatorname{dom} (q)) (p (\eta) \leq_ {Q _ {\eta}} q (\eta)).
$$

In particular, 

$$
\mathbb {P} _ {0} = \{\emptyset \}, \mathbb {P} _ {\lambda} = \bigcup_ {\beta <   \lambda} \mathbb {P} _ {\beta} \text {for every limit ordinal} 0 <   \lambda \leq \alpha ,\tag{9.14}
$$

and 

$$
\mathbb {P} _ {\gamma} \subset \mathbb {P} _ {\beta} \text { and } \leq_ {\gamma} = \leq_ {\beta} \cap (\mathbb {P} _ {\gamma} \times \mathbb {P} _ {\gamma}) \text { for   every } \gamma <   \beta \leq \alpha .\tag{9.15}
$$

Notice also that ∅ is a maximal element of every $\mathbb { P } _ { \beta }$ with $\beta \leq \alpha$ and that for every $\xi < \beta \le \alpha$ 

$$
\text {   if   } r \in \mathbb {P} _ {\beta} \text {   extends   } p \in \mathbb {P} _ {\xi} \text {   then   } r | _ {\xi} \in \mathbb {P} _ {\xi} \text {   also   extends   } p\tag{9.16}
$$

and 

if $q \in \mathbb { P } _ { \beta }$ and $r \in \mathbb { P } _ { \xi }$ extends $q | _ { \xi }$ then $r \cup q | _ { ( \beta \setminus \xi ) } \in \mathbb { P } _ { \beta }$ extends q. 

(9.17) 

Moreover, if $\mathbb { P } _ { \xi + 1 } ^ { \star } = \mathbb { P } _ { \xi + 1 } \setminus \mathbb { P } _ { \xi } = \{ p \in \mathbb { P } _ { \xi + 1 } \colon \xi \in \operatorname { d o m } ( p ) \}$ for $\xi < \alpha$ then 

$$
\langle \mathbb {P} _ {\xi + 1} ^ {\star}, \leq_ {\xi + 1} \rangle \text {   is   isomorphic   to   } \langle \mathbb {P} _ {\xi} \times Q _ {\xi}, \preceq \rangle\tag{9.18}
$$

via the isomorphism $p \mapsto \langle p | _ { \xi } , p ( \xi ) \rangle$ . The easy proofs of (9.14)–(9.18) are left as an exercise. 

For the general case, when P<sub>ξ</sub>-names $\pi _ { \xi }$ do not necessary represent the forcings from the ground model, the sequence $\langle \langle \mathbb { P } _ { \xi } , \le _ { \xi } \rangle \colon \xi \le \alpha \rangle$ will be defined by simultaneous induction with a sequence $\langle \langle \pi _ { \xi } , \leq _ { \pi _ { \xi } } \rangle \colon \xi < \alpha \rangle$ . In particular, we say that a sequence $\langle \langle \mathbb { P } _ { \xi } , \le _ { \xi } \rangle \colon \xi \le \alpha \rangle$ of partially ordered sets is an α-stage forcing iteration (with finite support) if there exists a sequence $\langle \langle \pi _ { \xi } , \leq _ { \pi _ { \xi } } \rangle \colon \xi < \alpha \rangle$ such that every $\langle \pi _ { \xi } , \leq _ { \pi _ { \xi } } \rangle$ is a good $\mathbb { P } _ { \xi ^ { - } } \mathrm { n a m e }$ for a partially ordered set, and if for every $\beta \leq \alpha$ 

$$
\mathbb {P} _ {\beta} = \bigcup_ {S \in [ \beta ] ^ {<   \omega}} \left\{p \in \prod_ {\eta \in S} \operatorname{dom} \left(\pi_ {\eta}\right): \forall \eta \in S \left(p | _ {\eta} \| - p (\eta) \in \pi_ {\eta}\right) \right\}\tag{9.19}
$$

is ordered by 

$$
p \leq_ {\beta} q \Leftrightarrow \operatorname{dom} (q) \subset \operatorname{dom} (p) \& (\forall \eta \in \operatorname{dom} (q)) (p | _ {\eta} \| - p (\eta) \leq_ {\pi_ {\eta}} q (\eta)).
$$

It is not dificult to see that the definition (9.19) gives the same notion of forcing as (9.13) if every $\pi _ { \xi }$ is the standard P -name $\hat { Q } _ { \xi }$ of $Q _ { \xi }$ . Moreover, it is also easy to notice that the sequence defined by (9.19) has the properties (9.14)–(9.17) as well (the inductive proof of (9.17) is left as an exercise). Moreover, for $\mathbb { P } _ { \xi + 1 } ^ { \star } = \{ p \in \mathbb { P } _ { \xi + 1 } \colon \xi \in \operatorname { d o m } ( p ) \}$ a counterpart of (9.18) says that for every $\xi <$ α 

$$
\langle \mathbb {P} _ {\xi + 1} ^ {\star}, \leq_ {\xi + 1} \rangle \text {   is   isomorphic   to   } \langle \mathbb {P} _ {\xi} \star \pi_ {\xi}, \preceq \rangle ,\tag{9.20}
$$

where an isomorphism is given by the map $p \mapsto \langle p | _ { \xi } , p ( \xi ) \rangle$ . To see this, it is enough to notice that for every $p , q \in \mathbb { P } _ { \xi + 1 } ^ { \star }$ 

$$
\begin{array}{r l} p \leq_ {\xi + 1} q & \Leftrightarrow \mathrm{dom} (q) \subset \mathrm{dom} (p)   \&   \big (\forall \eta \in \mathrm{dom} (q) \cap \xi \big) \big (p | _ {\eta}   \| -   p (\eta) \leq_ {\pi_ {\eta}} q (\eta) \big) \\ & \quad \&   p | _ {\xi}   \| -   p (\xi) \leq_ {\pi_ {\xi}} q (\xi) \\ & \Leftrightarrow   p | _ {\xi} \leq_ {\xi} q | _ {\xi}   \&   p | _ {\xi}   \| -   p (\xi) \leq_ {\pi_ {\xi}} q (\xi) \\ & \Leftrightarrow   \langle p | _ {\xi}, p (\xi) \rangle \preceq \langle q | _ {\xi}, q (\xi) \rangle . \end{array}
$$

The next theorem is an α-stage-iteration version of Theorem 9.5.3. It implies the condition P1, where $M _ { \xi }$ is defined as $M [ G _ { \xi } ]$ from the theorem. 

Theorem 9.5.6 Let M be a countable transitive model of ZFC, let $\alpha \in M$ be an ordinal number, and let $\langle \langle \mathbb { P } _ { \xi } , \leq _ { \xi } \rangle : \xi \leq \alpha \rangle \in M$ be an α-stage forcing iteration based on the sequence $\langle \langle \pi _ { \xi } , \leq _ { \pi _ { \xi } } \rangle : \xi < \alpha \rangle$ of appropriate $\mathbb { P } _ { \xi } - n a m e s .$ If G is an M-generic filter in $\mathbb { P } _ { \alpha }$ then $G _ { \xi } = G \cap \mathbb { P } _ { \xi }$ is an M-generic filter in $\mathbb { P } _ { \xi }$ for every $\xi < \alpha$ . Moreover, for every $\xi < \alpha$ , if 

$$
G ^ {\xi} = \{\mathrm{val} _ {G _ {\xi}} (p (\xi)) \colon p \in G _ {\xi + 1} \& \xi \in \mathrm{dom} (p) \}
$$

then $G ^ { \xi }$ is an M[G<sub>ξ</sub>]-generic filter in a forcing $\mathbb { P } ^ { \xi } = \langle \mathrm { v a l } _ { G _ { \xi } } ( \pi _ { \xi } ) , \mathrm { v a l } _ { G _ { \xi } } ( \leq _ { \pi _ { \xi } } ) \rangle$ and $M [ G _ { \xi + 1 } ] = M [ G _ { \xi } ] [ G ^ { \xi } ]$ 

Proof To see that $G _ { \xi }$ is a filter in $\mathbb { P } _ { \xi }$ take $p , q \in G _ { \xi } \subset G$ . Then there exists an $r \in G$ extending p and $q .$ . But $r | _ { \xi } \in \mathbb { P } _ { \xi }$ belongs to $G ,$ since $r \leq r | _ { \xi }$ So $r | _ { \xi } \in G _ { \xi }$ and, by $( 9 . 1 6 ) , r | _ { \xi }$ extends p and q. Also, if $q \in G _ { \xi } , p \in \mathbb { P } _ { \alpha }$ and $q \leq p$ then $p \in \mathbb { P } _ { \xi }$ , and so $p \in G _ { \xi }$ . Thus $G _ { \xi }$ is a filter in $\mathbb { P } _ { \xi }$ 

To prove that $G _ { \xi }$ is M-generic in $\mathbb { P } _ { \xi }$ take a $D \in M$ that is a dense subset of $\mathbb { P } _ { \xi }$ and notice that 

$$
D ^ {\star} = \{p \in \mathbb {P} _ {\alpha} \colon p | _ {\xi} \in D \} \in M
$$

is dense in $\mathbb { P } _ { \alpha }$ . Indeed, if $q \in \mathbb { P } _ { \alpha }$ then $q | _ { \xi } \in \mathbb { P } _ { \xi }$ and there exists an $r \in D$ with $r \leq _ { \xi } q | _ { \xi }$ . But, by (9.17), $p = r \cup q | _ { ( \alpha \backslash { \xi } ) } \in \mathbb { P } _ { \alpha }$ extends $q$ and it is easy to see that $p \in D ^ { \star }$ . So $D ^ { \star }$ is dense and there exists an $r \in G \cap D ^ { \star }$ . Hence $r | _ { \xi } \in D \cap G _ { \xi }$ 

The proof of the additional part will be done in several steps. First notice that 

$$
\mathbb {P} _ {\xi + 1} ^ {\star} \text {   is   dense   in   } \mathbb {P} _ {\xi + 1},\tag{9.21}
$$

since every $p \in \mathbb { P } _ { \xi + 1 } \setminus \mathbb { P } _ { \xi + 1 } ^ { \star } = \mathbb { P } _ { \xi }$ forces $\langle \pi _ { \xi } , \leq _ { \pi _ { \xi } } \rangle$ to be a partially ordered set, so there exists a $\mathbb { P } _ { \xi ^ { - } } \mathrm { n a m e } \tau$ such that $p \parallel - \tau \in \pi _ { \xi }$ and $p \cup \{ \langle \xi , \tau \rangle \} \in \mathbb { P } _ { \xi + 1 } ^ { \star }$ extends $p .$ 

Next notice that 

$$
G _ {\xi + 1} ^ {\star} = G \cap \mathbb {P} _ {\xi + 1} ^ {\star} = G _ {\xi + 1} \setminus \mathbb {P} _ {\xi}
$$

is also an M-generic filter in $\mathbb { P } _ { \xi + 1 } ^ { \star }$ , since, by (9.21), every dense $D \in M$ subset of $\mathbb { P } _ { \xi + 1 } ^ { \star }$ is also dense in $\begin{array} { r } { \vec { \mathbb { P } } _ { \xi + 1 } } \end{array}$ and $D \cap G _ { \xi + 1 } ^ { \star } = D \cap G _ { \xi + 1 } \neq \emptyset$ . Also, $G _ { \xi + 1 } = G _ { \xi + 1 } ^ { \star ^ { \star } } \cup \{ p | _ { \xi } \colon p \in G _ { \xi + 1 } ^ { \star } \} \in M [ G _ { \xi + 1 } ^ { \star } ]$ . So $\dot { M } [ G _ { \xi + 1 } ] = M [ G _ { \xi + 1 } ^ { \star } ]$ 

Now, if i is an isomorphism from (9.20) then 

$$
i [ G _ {\xi + 1} ^ {\star} ] = \{\langle p | _ {\xi}, p (\xi) \rangle : p \in G _ {\xi + 1} ^ {\star} \}
$$

is an M-generic filter in $\mathbb { P } _ { \xi } \star \pi _ { \xi }$ and $M [ G _ { \xi + 1 } ] = M [ G _ { \xi + 1 } ^ { \star } ] = M [ i [ G _ { \xi + 1 } ^ { \star } ] ]$ So, by Theorem 9.5.3, $i [ G _ { \xi + 1 } ^ { \star } ] = G _ { \xi } \star G ^ { \xi } , G ^ { \xi }$ is an $M [ G _ { \xi } ] \mathrm { - g e n e r i c }$ filter in $\mathbb { P } ^ { \xi }$ , and $M [ G _ { \xi + 1 } ] = M [ i [ G _ { \xi + 1 } ^ { \star } ] ] = M [ G _ { \xi } ] [ G ^ { \xi } ]$  

The next theorem says that an α-stage iteration (with finite support) of ccc forcings is ccc. This will guarantee that the forcing $\mathbb { P } _ { \mu }$ from the beginning of the section will be ccc. The theorem is a generalization of Lemma 9.5.5. 

Theorem 9.5.7 Let M be a countable transitive model of ZFC, let $\alpha \in M$ be an ordinal number, and let $\langle \langle \mathbb { P } _ { \xi } , \leq _ { \xi } \rangle : \xi \leq \alpha \rangle \in$ M be an α-stage forcing iteration based on the sequence $\langle \langle \pi _ { \xi } , \leq _ { \pi _ { \xi } } \rangle \colon \xi < \alpha \rangle$ of appropriate $\mathbb { P } _ { \xi } - n a m e s .$ If 

$$
\mathbb {P} _ {\xi} \left\| - \pi_ {\xi} i s c c c \right.\tag{9.22}
$$

for every $\xi < \alpha$ , then $\mathbb { P } _ { \alpha }$ is ccc in M. 

Proof We will prove, by induction on $\beta \leq \alpha$ , that $\mathbb { P } _ { \beta }$ is ccc in M. The proof will be done in $M$ 

Clearly $\mathbb { P } _ { 0 } = \{ \varnothing \}$ is ccc. So let $0 < \beta \le$ α be such that $\mathbb { P } _ { \eta }$ is ccc in M for every $\eta < \beta$ and let $A = \{ p _ { \gamma } \colon \gamma < \omega _ { 1 } \} \subset { \mathbb { P } } _ { \beta }$ . We will find $\delta < \gamma < \omega _ { 1 }$ such that $p _ { \delta }$ and $p _ { \gamma }$ are compatible. 

If $\beta$ is a successor ordinal, say $\beta = \xi + 1$ , take $C _ { 0 } = \{ \gamma < \omega _ { 1 } : p _ { \gamma } \in \mathbb { P } _ { \xi } \}$ If $| C _ { 0 } | = \omega _ { 1 }$ then $A _ { 0 } = \{ p _ { \gamma } \colon \gamma \in C _ { 0 } \} \subset \mathbb { P } _ { \xi }$ , and $\mathbb { P } _ { \xi }$ is ccc by the inductive assumption. Hence $A _ { 0 } \subset A$ contains two compatible elements with diferent indices. So assume that $| C _ { 0 } | < \omega _ { 1 }$ . Then $C _ { 1 } = \omega _ { 1 } \setminus C _ { 0 }$ is uncountable and $A _ { 1 } = \{ p _ { \gamma } \colon \gamma \in C _ { 1 } \} \subset \mathbb { P } _ { \xi + 1 } ^ { \star }$ . But $\mathbb { P } _ { \xi + 1 } ^ { \star }$ is isomorphic to $\mathbb { P } _ { \xi } \star \pi _ { \xi }$ , which, by Lemma 9.5.5, is ccc. Thus, once more, $A _ { 1 } \subset A$ contains two compatible elements with diferent indices. 

If $\beta$ is a limit ordinal, apply to the family $\{ \mathrm { d o m } ( p _ { \gamma } ) \colon \gamma < \omega _ { 1 } \}$ the $\Delta -$ system lemma to find an uncountable set $C \subset \omega _ { 1 }$ and a finite set $D \subset \beta$ such that dom $( p _ { \gamma } ) \cap \mathrm { d o m } ( p _ { \delta } ) = D$ for all distinct $\gamma , \delta \in C$ . Let $\xi < \beta$ be such that $D \subset \xi$ and consider $\{ p _ { \gamma } | _ { \xi } \colon \gamma \in C \} \subset \mathbb { P } _ { \xi }$ . Since, by the inductive assumption, $\mathbb { P } _ { \xi }$ is ccc, we can find $p \in \mathbb { P } _ { \xi }$ and distinct $\gamma , \delta \in C$ such that $p \leq _ { \xi } p _ { \gamma } | _ { \xi }$ and $p \le _ { \xi } p _ { \delta } | _ { \xi }$ . To finish the proof it is enough to notice that 

$$
q = p \cup p _ {\gamma} | _ {(\beta \setminus \xi)} \cup p _ {\delta} | _ {(\beta \setminus \xi)}\tag{9.23}
$$

belongs to $\mathbb { P } _ { \beta }$ and extends $p _ { \gamma }$ and $p _ { \delta }$ ; this follows from (9.17). The details are left as an exercise.  

We say that an α-stage forcing iteration $\langle \langle \mathbb { P } _ { \xi } , \le _ { \xi } \rangle \colon \xi \le \alpha \rangle$ is a ccc forcing iteration if it satisfies condition (9.22). 

The next lemma is the last general fact concerning the α-stage iteration and it will imply property P2. It is an analog of Lemma 9.4.3. 

Lemma 9.5.8 Let M be a countable transitive model of ZFC, let $\kappa \in M$ be an infinite regular cardinal number, and let $\langle \langle \mathbb { P } _ { \xi } , \le _ { \xi } \rangle : \xi \le \kappa \rangle \in M$ be a $\kappa { - } s t a g e$ ccc forcing iteration. $I f Y \in M , G$ is an M-generic filter in $\mathbb { P } _ { \kappa } ,$ and $S \subset Y$ is such that $M [ G ] \models | S | < \kappa$ then there exists $a \ \zeta < \kappa$ such that $S \in M [ G _ { \zeta } ]$ , where $G _ { \zeta } = G \cap \mathbb { P } _ { \zeta }$ 

Proof By Theorem 9.5.7 the forcing $\mathbb { P } _ { \kappa }$ is ccc. So the cardinals in M and $M [ G ]$ are the same, and we will not distinguish between them. 

Let $X = \lambda$ , where λ is the cardinality of S in $M [ G ]$ . Then $X \in M$ and $| X | = \lambda < \kappa$ . Let $f \in M [ G ]$ be a map from X onto S. We will find a $\zeta < \kappa$ such that $f \in M [ G _ { \zeta } ]$ 

By Lemma 9.2.8 we can find a $\mathbb { P } _ { \kappa ^ { - \mathrm { n a m e } } } \tau \in M$ such that $f = \mathrm { v a l } _ { G } ( \tau )$ $\tau \subset \{ \langle { \widehat { \langle x , y \rangle } } , p \rangle : x \in X \ \& \ y \in Y \ \& \ p \in \mathbb { P } _ { \kappa } \}$ , and 

(G) $A _ { x } = \Bigl \{ p \in \mathbb { P } _ { \kappa } \colon \exists y \in Y \ \Bigl ( \langle \widehat { \langle x , y \rangle } , p \rangle \in \tau \Bigr ) \Bigr \}$ is an antichain for every $x \in X .$ 

So every $A _ { x }$ is countable in M, since $\mathbb { P } _ { \kappa }$ is ccc in M. Let 

$$
A = \bigcup_ {x \in X} \bigcup_ {p \in A _ {x}} \operatorname{dom} (p).
$$

Then $A \in M , A \subset \kappa$ , and $| A | \le | X | + \omega < \kappa$ in M, since every set $\textstyle \bigcup _ { p \in A _ { x } } \operatorname { d o m } ( p )$ is countable in M. Thus, by the regularity of $\kappa .$ , there exists a $\zeta < \kappa$ such that $A \subset \zeta$ . In particular, $\textstyle \bigcup _ { x \in X } A _ { x } \subset \mathbb { P } _ { \zeta }$ . So 

$$
\tau^ {\star} = \left\{\langle \widehat {\langle x , y \rangle} ^ {\star}, p \rangle : \langle \widehat {\langle x , y \rangle}, p \rangle \in \tau \right\} \in M
$$

is a $\mathbb { P } _ { \zeta ^ { - } \mathrm { n a m e } }$ , where $\widehat { \langle x , y \rangle } ^ { \star }$ is a standard $\mathbb { P } _ { \zeta } { \mathrm { - n a m e } }$ for $\langle x , y \rangle \in M$ , and 

$$
\begin{array}{r c l} f = \mathrm{val} _ {G} (\tau) & = & \left\{\langle x, y \rangle \colon \exists p \in G \left(\langle \widehat {\langle x , y \rangle}, p \rangle \in \tau\right) \right\} \\ & = & \left\{\langle x, y \rangle \colon (\exists p \in G \cap \mathbb {P} _ {\zeta}) \left(\langle \widehat {\langle x , y \rangle} ^ {\star}, p \rangle \in \tau^ {\star}\right) \right\} \\ & = & \mathrm{val} _ {G _ {\zeta}} (\tau) \in M [ G _ {\zeta} ]. \end{array}
$$

So $S = f [ X ] \in M [ G _ { \zeta } ] .$ 

 

Now we are ready for the main theorem of this section. 

Theorem 9.5.9 It is consistent with ZFC that ${ \mathfrak { c } } = \omega _ { 2 }$ and MA holds. 

Proof By the foregoing discussion, it is enough to construct a µ-stage ccc finite-support forcing iteration $\langle \langle \mathbb { P } _ { \xi } , \leq _ { \xi } \rangle \colon \xi \leq \mu \rangle$ , with $\mu = \omega _ { 2 } ^ { M }$ , that satisfies P3 and P4. The construction will be done in a countable transitive model M of ZFC in which $2 ^ { \omega _ { 1 } } = \omega _ { 2 }$ (such an M exists by Corollary 9.3.9). In what follows we will use the notation introduced in the first part of this section. We will also use repeatedly the fact, following from (9.15), that for every $\zeta \le \xi \le \mu$ any $\mathbb { P } _ { \zeta } { \mathrm { - n a m e } }$ is a $\mathbb { P } _ { \xi ^ { - } } \mathrm { n a m e ~ t o o } .$ 

Let $\langle \langle \alpha _ { \xi } , \beta _ { \xi } \rangle \colon \xi \ < \ \mu \rangle \ \in \ M$ be a one-to-one enumeration of $\mu \times \mu$ such that $\beta _ { \xi } \le \xi$ for every $\xi < \mu$ . By induction on $\xi < \mu$ we will construct a finite-support iteration $\langle \langle \mathbb { P } _ { \xi } , \leq _ { \xi } \rangle : \xi \leq \mu \rangle$ , together with a sequence $\langle \langle \pi _ { \xi } , \leq _ { \pi _ { \xi } } \rangle \colon \xi < \mu \rangle$ of appropriate $\mathbb { P } _ { \xi ^ { - } \mathrm { n a m e s } , }$ and a sequence $\langle S _ { \xi } \colon \xi \ < \ \mu \rangle$ such that the following inductive conditions are satisfied for every $\xi < \mu .$ 

(I<sub>ξ</sub>) $\begin{array} { r } { | \mathbb { P } _ { \xi } | \le \omega _ { 1 } . } \end{array}$ 

(II<sub>ξ</sub>) $S _ { \xi } = \langle \langle \lambda _ { \alpha } ^ { \xi } , \sigma _ { \alpha } ^ { \xi } \rangle \colon \alpha < \mu \rangle$ contains every pair $\langle \lambda , \sigma \rangle$ with $\lambda \leq \omega _ { 1 }$ and 

$$
\sigma \subset \{\langle \langle \gamma , \delta \rangle , p \rangle : \gamma , \delta \in \lambda \& p \in \mathbb {P} _ {\xi} \}.
$$

(σ will be used as a $\mathbb { P } _ { \xi } \mathrm { - n a m e }$ for a partial order on λ.) 

$\begin{array} { r l } { ( \mathrm { I I I } _ { \xi } ) } & { { } \pi _ { \xi } = \hat { \lambda } } \end{array}$ is a standard $\mathbb { P } _ { \xi } \mathrm { - n a m e }$ for $\lambda = \lambda _ { \alpha _ { \xi } } ^ { \beta _ { \xi } }$ and 

$$
\begin{array}{r c l} \leq_ {\pi_ {\xi}} & = & \{\langle \langle \gamma , \delta \rangle , p \rangle \in \sigma_ {\alpha_ {\xi}} ^ {\beta_ {\xi}} \colon \exists q \in A (q \leq_ {\xi} p) \} \\ & & \cup \{\langle \langle \gamma , \delta \rangle , p \rangle \colon \gamma \leq \delta <   \lambda   \&   p \in B \}, \end{array}
$$

where 

$$
A = \{q \in \mathbb {P} _ {\xi} \colon q \| - \langle \hat {\lambda}, \sigma_ {\alpha_ {\xi}} ^ {\beta_ {\xi}} \rangle \text {is a ccc forcing} \}
$$

and $B = \{ p \in \mathbb { P } _ { \xi } \colon p$ is incompatible with every $q \in A \}$ . In particular, 

$$
\mathbb {P} _ {\xi} \left\| - \langle \pi_ {\xi}, \leq_ {\pi_ {\xi}} \right\rangle \text {   is   a   ccc   forcing. }\tag{9.24}
$$

To see that this inductive construction preserves $\left( \mathrm { I } _ { \xi } \right)$ consider two cases. If $0 < \xi < \mu$ is a limit ordinal, then $\begin{array} { r } { \mathbb { P } _ { \xi } = \bigcup _ { \eta < \xi } \mathbb { P } _ { \eta } } \end{array}$ has cardinality $\leq \omega _ { 1 }$ by the inductive assumption. If $\xi = \eta + 1$ is a successor ordinal, then $\mathbb { P } _ { \xi } = \mathbb { P } _ { \eta } \cup \mathbb { P } _ { \xi } ^ { \star }$ , and $\mathbb { P } _ { \xi } ^ { \star }$ is isomorphic to $\mathbb { P } _ { \eta } \star \pi _ { \eta }$ . But by $\left( \mathrm { I } _ { \eta } \right)$ and $\left( \operatorname { I I I } _ { \eta } \right)$ we have $| \pi _ { \eta } | \leq \dot { \omega } _ { 1 }$ . So $| \mathring { \mathbb { P } } _ { \xi } | = | \mathbb { P } _ { \eta } | \oplus ( | \mathbb { P } _ { \eta } | \otimes | \dot { \pi } _ { \eta } | ) \stackrel { . } { \le } \omega _ { 1 }$ as well. 

To see that the sequence $S _ { \xi }$ in $( \mathrm { I I } _ { \xi } )$ can be found note that there are only $\omega _ { 2 }$ pairs $\langle \lambda , \sigma \rangle$ to list since, by $\left( \mathrm { I } _ { \xi } \right)$ , the set $\{ \langle \widehat { \langle \gamma , \delta \rangle } , p \rangle \colon \gamma , \delta \in \lambda$ & $p \in \mathbb { P } _ { \xi } \}$ has cardinality $\leq \omega _ { 1 }$ and so it has at most $\omega _ { 2 }$ subsets, as $2 ^ { \omega _ { 1 } } = \omega _ { 2 }$ in M. 

To finish the construction it is enough to argue for (9.24). For this, notice first that 

$$
A \cup B \text {   is   dense   in   } \mathbb {P} _ {\xi}\tag{9.25}
$$

and 

$$
p \left\| - \left(\sigma_ {\alpha_ {\xi}} ^ {\beta_ {\xi}} = \leq_ {\pi_ {\xi}}\right) \quad \text {   for   every   } p \in A. \right.\tag{9.26}
$$

To see (9.26) take $p _ { 0 } \in A$ and an M-generic filter H in $\mathbb { P } _ { \xi }$ containing $p _ { 0 }$ . Then 

$$
\begin{array}{l l l} \operatorname{val} _ {H} (\sigma_ {\alpha_ {\xi}} ^ {\beta_ {\xi}}) & = & \{\langle \gamma , \delta \rangle \colon \widehat {\langle \langle \gamma , \delta \rangle}, p \rangle \in \sigma_ {\alpha_ {\xi}} ^ {\beta_ {\xi}}   \&   p \in H \} \\ & = & \{\langle \gamma , \delta \rangle \colon \widehat {\langle \langle \gamma , \delta \rangle}, p \rangle \in \sigma_ {\alpha_ {\xi}} ^ {\beta_ {\xi}}   \&   \exists q \in A   (q \leq_ {\xi} p)   \&   p \in H \} \\ & = & \{\langle \gamma , \delta \rangle \colon \widehat {\langle \langle \gamma , \delta \rangle}, p \rangle \in \leq_ {\pi_ {\xi}}   \&   \exists q \in A   (q \leq_ {\xi} p)   \&   p \in H \} \\ & = & \{\langle \gamma , \delta \rangle \colon \widehat {\langle \langle \gamma , \delta \rangle}, p \rangle \in \leq_ {\pi_ {\xi}}   \&   p \in H \} \\ & = & \operatorname{val} _ {H} (\leq_ {\pi_ {\xi}}), \end{array}
$$

proving (9.26). 

To argue for (9.24) let H be an M-generic filter in $\mathbb { P } _ { \xi }$ . We have to show that $\left. \mathrm { v a l } _ { H } ( \pi _ { \xi } ) \right.$ , val $( \leq _ { \pi _ { \xi } } ) \rangle = \langle \lambda , \mathrm { v a l } _ { H } ( \leq _ { \pi _ { \xi } } ) \rangle$ is a ccc partially ordered set in $M [ H ]$ . But, by (9.25), either $A \cap H \neq \emptyset$ , in which case this is true since an element of $A \cap H$ forces $\langle \pi _ { \xi } , \leq _ { \pi _ { \xi } } \rangle = \langle \hat { \lambda } , \sigma _ { \alpha _ { \xi } } ^ { \beta _ { \xi } } \rangle$ to be a ccc forcing, or $B \cap H \neq \emptyset$ , in which case val $_ H \big ( \leq _ { \pi _ { \xi } } \big )$ is just a standard well ordering of λ, so it is obviously ccc. This finishes the inductive construction. 

Now, to see that P3 is satisfied note that $\textstyle \mathbb { P } _ { \mu } = \bigcup _ { \xi < \mu } \mathbb { P } _ { \xi }$ has cardinality $\leq \omega _ { 2 }$ . Thus $| ( \mathbb { P } _ { \mu } ) ^ { \omega } | \leq ( \omega _ { 2 } ) ^ { \omega _ { 1 } } = 2 ^ { \omega _ { 1 } } = \omega _ { 2 }$ 

To see that P4 holds let $G$ be an M-generic filter in $\mathbb { P } _ { \mu }$ , let $N = M [ G ]$ and let $\langle \lambda , \ll \rangle \in N$ be such that 

$$
N \models \lambda \leq \omega_ {1} \text {   and   } \langle \lambda , \ll \rangle \text {   is   ccc. }
$$

Choose an $\alpha _ { 0 } < \mu$ . By Theorem 9.5.6 it is enough to find $\alpha _ { 0 } < \xi < \mu$ such that $\mathbb { P } ^ { \xi } = \langle \mathrm { v a l } _ { G _ { \xi } } ( \pi _ { \xi } ) , \mathrm { v a l } _ { G _ { \xi } } ( \leq _ { \pi _ { \xi } } ) \rangle = \langle \lambda , \ll \rangle$ . But, by Lemma 9.5.8, there is $\alpha _ { 0 } < \zeta < \mu$ such that $\langle \lambda , \tilde { \ll } \rangle \in \mathop { M } [ G _ { \zeta } ]$ . Take a P -name $\sigma ^ { \star } \in M$ such that val $G _ { \zeta } \left( \sigma ^ { \star } \right)$ is equal to $\ll$ and let 

$$
\sigma = \{\langle \langle \gamma , \delta \rangle , p \rangle : \gamma , \delta \in \lambda \& p \in \mathbb {P} _ {\zeta} \& p \| - \widehat {\langle \gamma , \delta \rangle} \in \sigma^ {\star} \} \in M.
$$

Note that 

$$
\mathrm{val} _ {G _ {\zeta}} (\sigma) = \mathrm{val} _ {G _ {\zeta}} (\sigma^ {\star})
$$

since for every $\langle \gamma , \delta \rangle \in \lambda \times \lambda$ 

$$
\langle \gamma , \delta \rangle \in \operatorname{val} _ {G _ {\zeta}} (\sigma) \Leftrightarrow \exists p \in G _ {\zeta} (p \| - \widehat {\langle \gamma , \delta \rangle} \in \sigma^ {\star}) \Leftrightarrow \langle \gamma , \delta \rangle \in \operatorname{val} _ {G _ {\zeta}} (\sigma^ {\star}).
$$

Next, choose $\alpha < \mu$ such that $\langle \lambda _ { \alpha } ^ { \zeta } , \sigma _ { \alpha } ^ { \zeta } \rangle = \langle \lambda , \sigma \rangle$ and pick $\xi < \mu$ with $\langle \alpha _ { \xi } , \beta _ { \xi } \rangle = \langle \alpha , \zeta \rangle$ . Then $\alpha _ { 0 } < \zeta = \beta _ { \xi } \leq \xi$ and $\begin{array} { r } { \lambda _ { \alpha _ { \xi } } ^ { \beta _ { \xi } } = \lambda _ { \alpha } ^ { \zeta } = \lambda } \end{array}$ , so $\operatorname { v a l } _ { G _ { \xi } } ( \pi _ { \xi } ) =$ λ. Also, $\sigma _ { \alpha _ { \xi } } ^ { \beta _ { \xi } } = \sigma _ { \alpha } ^ { \zeta } = \sigma$ and 

$$
\operatorname{val} _ {G _ {\xi}} (\sigma) = \operatorname{val} _ {G _ {\zeta}} (\sigma) = \operatorname{val} _ {G _ {\zeta}} \left(\sigma^ {\star}\right) = (\ll) \in M \left[ G _ {\zeta} \right] \subset M \left[ G _ {\xi} \right]
$$

since $G _ { \zeta } = G _ { \xi } \cap \mathbb { P } _ { \zeta }$ 

Thus it sufices to argue that 

$$
\operatorname{val} _ {G _ {\xi}} (\leq_ {\pi_ {\xi}}) = \operatorname{val} _ {G _ {\xi}} (\sigma).\tag{9.27}
$$

But $\langle \lambda , \ll \rangle$ is a partially ordered set in $M [ G _ { \xi } ]$ , since it is a partially ordered set in N and this is an absolute property. Also, $\langle \lambda , \ll \rangle$ is ccc in $M [ G _ { \xi } ]$ because every antichain $A \in M [ G _ { \xi } ]$ is also an antichain in N and 

$$
\omega = | A | ^ {N} = | A | ^ {M} = | A | ^ {M [ G _ {\xi} ]},
$$

since $\langle \lambda , \ll \rangle$ is ccc in N and both extensions of M preserve the cardinals. Thus there is a $p \in G _ { \xi }$ that forces this to be true for $\langle \hat { \lambda } , \sigma \rangle = \langle \hat { \lambda } , \sigma _ { \alpha _ { \xi } } ^ { \beta _ { \xi } } \rangle$ . In particular, $G _ { \xi } \cap A \neq \varnothing$ so (9.26) and $\sigma _ { \alpha _ { \xi } } ^ { \beta _ { \xi } } = \sigma$ imply (9.27). This finishes the proof.  

## EXERCISES

1 Complete the details of the proof of (9.8). 

2 Complete the details of the proof of Lemma 9.5.1. 

3 Prove that the relation % defined on an iteration $\mathbb { P } \star \pi$ is transitive. 

4 Prove (9.10). 

5 Complete the proof of Theorem 9.5.3 by showing that the set D from (9.11) is indeed dense below $\langle q , \eta \rangle$ 

6 Prove Theorem 9.5.4. 

7 Prove properties (9.14)–(9.18). 

8 Prove (9.17) for the forcing defined by (9.19). 

9 Complete the proof of Theorem 9.5.7 by showing that the condition q defined by (9.23) has the desired properties. 

# Axioms of set theory

Axiom 0 (Set Existence) There exists a set: 

$$
\exists x (x = x).
$$

Axiom 1 (Extensionality) If x and y have the same elements, then x is equal to y: 

$$
\forall x \forall y [ \forall z (z \in x \leftrightarrow z \in y) \rightarrow x = y ].
$$

Axiom 2 (Comprehension scheme or schema of separation) For every formula $\varphi ( s , t )$ with free variables s and t, for every x, and for every parameter p there exists a set $y = \{ u \in x \colon \varphi ( u , p ) \}$ that contains all those $u \in x$ that have property ϕ: 

$$
\forall x \forall p \exists y [ \forall u (u \in y \leftrightarrow (u \in x \& \varphi (u, p))) ].
$$

Axiom 3 (Pairing) For any a and b there exists a set x that contains a and b: 

$$
\forall a \forall b \exists x (a \in x \& b \in x).
$$

Axiom 4 (Union) For every family $\mathcal { F }$ there exists a set U containing the union $\cup \mathcal { F }$ of all elements of $\mathcal { F }$ 。• 

$$
\forall \mathcal {F} \exists U \forall Y \forall x [ (x \in Y \&Y \in \mathcal {F}) \rightarrow x \in U ].
$$

Axiom 5 (Power set) For every set X there exists a set P containing the set ${ \mathcal { P } } ( X )$ (the power set) of all subsets of X: 

$$
\forall X \exists P \forall z [ z \subset X \rightarrow z \in P ].
$$

To make the statement of the next axiom more readable we introduce the following abbreviation. We say that y is a successor of x and write $y = S ( x ) { \mathrm { ~ i f ~ } } S ( x ) = x \cup \{ x \}$ , that is, 

$$
\forall z [ z \in y \leftrightarrow (z \in x \lor z = x) ].
$$

Axiom $\textbf { 6 } \ : ( I n f i n i t y )$ (Zermelo 1908) There exists an infinite set (of some special form): 

$$
\exists x [ \forall z (z = \emptyset \rightarrow z \in x) \&\forall y \in x \forall z (z = S (y) \rightarrow z \in x) ].
$$

Axiom 7 (Replacement scheme) (Fraenkel 1922; Skolem 1922) For every formula $\varphi ( s , t , U , w )$ with free variables s, t, U, and w, every set $A$ , and every parameter p if $\varphi ( s , t , A , p )$ defines a function F on A by $F ( x ) = y \Leftrightarrow \varphi ( x , y , A , p )$ , then there exists a set $Y$ containing the range $F [ A ] = \{ F ( x ) \colon x \in A \}$ of the function F: 

$$
\forall A \forall p [ \forall x \in A \exists ! y \varphi (x, y, A, p) \rightarrow \exists Y \forall x \in A \exists y \in Y \varphi (x, y, A, p) ],
$$

where the quantifier $\exists ! x \varphi ( x )$ is an abbreviation for “there exists precisely one x satisfying ϕ,” that is, is equivalent to the formula 

$$
\exists x \varphi (x) \&\forall x \forall y (\varphi (x) \&\varphi (y) \rightarrow x = y).
$$

Axiom 8 (Foundation or regularity) (Skolem 1922; von Neumann 1925) Every nonempty set has an ∈-minimal element: 

$$
\forall x [ \exists y (y \in x) \rightarrow \exists y (y \in x \&\neg \exists z (z \in x \&z \in y)) ].
$$

Axiom 9 (Choice) (Levi 1902; Zermelo 1904) For every family $\mathcal { F }$ of disjoint nonempty sets there exists a “selector,” that is, a set $S$ that intersects every $x \in { \mathcal { F } }$ in precisely one point: 

$$
\forall \mathcal {F} [ \forall x \in \mathcal {F} (x \neq \emptyset) \& \forall x \in \mathcal {F} \forall y \in \mathcal {F} (x = y \lor x \cap y = \emptyset) ]
$$

$$
\rightarrow \exists S \forall x \in \mathcal {F} \exists ! z (z \in S \&z \in x),
$$

where $x \cap y = \emptyset$ is an abbreviation for 

$$
\neg \exists z (z \in x \& z \in y).
$$

Using the comprehensive schema for Axioms 0, 3, 4, and 5 we may easily obtain the following strengthening of them, which is often used as the original axioms. 

Axiom $\mathbf { 0 ^ { \prime } }$ (Empty set) There exists the empty set $\varnothing$ 

$$
\exists x \forall y \neg (y \in x).
$$

Axiom $\textbf { 3 } ^ { \prime } \ ( P a i r i n g )$ For any a and b there exists a set x that contains precisely a and b. 

Axiom ${ \bf { 4 } } ^ { \prime }$ (Union) (Cantor 1899; Zermelo 1908) For every family $\mathcal { F }$ there exists a set $U = \cup \mathcal { F }$ , the union of all subsets of $\mathcal { F }$ . 

Axiom $\mathbf { 5 ^ { \prime } }$ (Power set) (Zermelo 1908) For every set x there exists a set $Y = \mathcal { P } ( x )$ , the power set of $x ,$ , that is, the set of all subsets of $x _ { \ast }$ 

The system of Axioms 0–8 is usually called Zermelo–Fraenkel set theory and is abbreviated by ZF. The system of Axioms 0–9 is usually denoted by ZFC. Thus, ZFC is the same as $\mathrm { Z F + A C }$ , where AC stands for the axiom of choice. 

Historical Remark (Levy 1979) The first similar system of axioms was introduced by Zermelo. However, he did not have the axioms of foundation and replacement. Informal versions of the axiom of replacement were suggested by Cantor (1899) and Mirimanof (1917). Formal versions were introduced by Fraenkel (1922) and Skolem (1922). The axiom of foundation was added by Skolem (1922) and von Neumann (1925). 

Notice that Axioms 2 and $7$ are in fact the schemas for infinitely many axioms, one for each formula $\varphi .$ . Thus theory ZFC has, in fact, infinitely many axioms. Axiom 1 of extensionality is the most fundamental one. Axioms 0 (or 0<sup>-</sup>) of set existence (of empty set) and 6 of infinity are “existence” axioms that postulate the existence of some sets. It is obvious that Axiom 0 follows from Axiom 6. Axioms 2 of comprehension and 7 of replacement are schemas for infinitely many axioms. Axioms 3 (or $3 ^ { \prime } )$ of pairing, 4 (or 4<sup>-</sup>) of union, and 5 (or 5<sup>-</sup>) of power set are conditional existence axioms. The existing sets postulated by $3 ^ { \prime } , 4 ^ { \prime }$ , and $5 ^ { \prime }$ are unique. It is not dificult to see that Axiom 3 of pairing follows from the others. 

The axiom of choice AC and the axiom of foundation also have the same conditional existence character. However, the sets existing by them do not have to be unique. Moreover, the axiom of foundation has a very set-theoretic meaning and is seldom used outside abstract set theory or logic. It lets us build “hierarchical models” of set theory. During this course we very seldom make use of it. The axiom of choice, on the other hand, is one of the most important tools in this course. It is true that its nonconstructive character caused, in the past, some mathematicians to reject it (for example, Borel and Lebesgue). However, this discussion has been for the most part resolved today in favor of accepting this axiom. 

It follows from the foregoing discussion that we can remove Axioms 0 and 3 from 0–8 and still have the same theory ZF. 

Appendix B 

# Comments on the forcing method

This appendix contains some comments and explanations for Section 9.1. It also includes some missing proofs of the results stated there. 

We start by explaining a few more terms. In Section 9.1 we said that a formula $\varphi$ is a consequence of a theory $T , T \vdash \varphi$ , if there is a formal proof of $\varphi$ from $T ,$ . By a formal proof in this statement we mean a formalization of what we really do in proving theorems. Thus a proof of $\varphi$ from $T$ is a finite sequence $\varphi _ { 0 } , \ldots , \varphi _ { n }$ of formulas such that $\varphi _ { n } = \varphi$ and a formula $\varphi _ { k }$ can appear in the sequence only because of one of following two reasons: 

$\varphi _ { k }$ is an axiom, that is, it belongs to $T$ or is a logic axiom; or 

$\varphi _ { k }$ is obtained from some $\varphi _ { i }$ and $\varphi _ { j } \ ( i , j < k )$ by a rule of detachment (also called a modus ponens rule), that is, if there exist $i , j < k$ such that $\varphi _ { j }$ has the form $\varphi _ { i } \longrightarrow \varphi _ { k }$ 

Since any formal proof is a finite sequence of formulas, it can contain only finitely many sentences from $T$ . Thus, if $T \vdash \varphi$ then there is a finite subtheory $T _ { 0 } \subset T$ such that $T _ { 0 } \vdash \varphi$ . In particular, if theory $T$ is inconsistent, then there is a finite subtheory $T _ { 0 }$ of $T$ that is also inconsistent. So theory $T$ is consistent if and only if every one of its finite subtheories is consistent. 

Note also that if $\varphi _ { 0 } , \ldots , \varphi _ { n }$ is a proof of $\varphi = \varphi _ { n }$ in theory $T \cup \{ \psi \}$ then $( \psi {  } \varphi _ { 0 } ) , \ldots , ( \psi {  } \varphi _ { n } )$ is a proof of $\psi {  } \varphi$ in $T$ , where formula $\psi { \longrightarrow } \left( \varphi _ { i } { \longrightarrow } \varphi _ { k } \right)$ is identified with $\varphi _ { i } { \longrightarrow } ( \psi { \longrightarrow } \varphi _ { k } )$ . Thus, if $\varphi$ is a consequence of a finite theory $T _ { 0 } ~ = ~ \{ \psi _ { 0 } , . . . , \psi _ { n } \}$ then $\emptyset \ \vdash \ ( \psi _ { 0 } { \longrightarrow } ( \cdot \cdot \cdot \longrightarrow ( \psi _ { n } { \longrightarrow } \varphi ) \cdot \cdot \cdot ) )$ , that is, $( \psi _ { 0 } \& \cdot \cdot \cdot \& \psi _ { n } ) { \longrightarrow } \varphi$ is a consequence of the axioms of logic. 

To argue for the forcing principle we will need the following theorem. 

Theorem B.1 Let $S$ and $T$ be two theories and assume that for every $f _ { - }$ nite subtheory $S _ { 0 }$ ofS we can prove in theory $T$ that there exists a nonempty transitive set M that is a model for $S _ { 0 }$ . Then Con(T) implies Con(S). 

Proof Let $S$ and $T$ be as in the theorem and assume that $S$ is inconsistent. It is enough to show that this implies the inconsistency of $T$ 

Since $S$ is inconsistent, there is a finite subtheory $S _ { 0 } = \{ \psi _ { 1 } , . . . , \psi _ { n } \}$ of $S$ such that $S _ { 0 }$ is inconsistent, that is, such that $S _ { 0 } \vdash \varphi \& \lnot \varphi$ for some sentence $\varphi .$ . In particular, $( \psi _ { 1 } \& \cdot \cdot \cdot \& \psi _ { n } ) { \longrightarrow } ( \varphi \& \lnot \varphi )$ 

But, by our assumption, in theory $T$ we can prove the existence of a nonempty transitive set M that is a model for $S _ { 0 }$ , that is, such that $\psi ^ { M }$ holds for every $\psi$ from $S _ { 0 }$ . In particular, 

$$
T \vdash \exists M (\psi_ {1} ^ {M} \& \dots \& \psi_ {n} ^ {M}).
$$

Now, it is enough to notice that the rules of formal deduction are set up in such a way that if $\varphi _ { 0 } , \ldots , \varphi _ { n }$ is a formal proof of $\varphi \& \to \varphi$ from $S _ { 0 }$ then $\varphi _ { 0 } ^ { M } , \dots , \varphi _ { n } ^ { M }$ is a formal proof of $\varphi ^ { M } \& \to \varphi ^ { M }$ from $S _ { 0 } ^ { M } = \{ \psi _ { 1 } ^ { \dot { M } } , \dots , \psi _ { n } ^ { M } \}$ . In particular, the implication 

$$
(\psi_ {1} ^ {M} \&\dots \&\psi_ {n} ^ {M}) \rightarrow (\varphi^ {M} \&\neg \varphi^ {M})
$$

is true for every M. So we have proved in $T$ that there is an M such that $\psi _ { 1 } ^ { M } \& \cdot \cdot \cdot \& \psi _ { n } ^ { M } .$ , while $( \psi _ { 1 } ^ { M } \& \cdot \cdot \hat { \& } \psi _ { n } ^ { M } ) {  } ( \varphi ^ { M } \& \lnot \varphi ^ { M } )$ is true for every M. $\mathrm { S o } \ \exists M \ ( \varphi ^ { M } \overleftarrow { \& } \lnot \varphi ^ { M } )$ is a consequence of $T _ { \ast }$ that is, T is inconsistent.  

Now assume that we have proved the following condition (F) from the forcing principle: 

(F) Every CTM M of ZFC can be extended to a CTM N of $\mathrm { Z F C + ^ { \cdots } } \psi . ^ { \prime }$ 

If we could prove in ZFC that 

$$
\exists M (M \text {   is   a   CTM   for   ZFC })
$$

then we would conclude in ZFC that there exists a model N of $\mathrm { Z F C + ^ { \omega } } \psi ,$ and this, by Theorem B.1, implies that $\operatorname { C o n } ( \mathrm { Z F C } ) { \Rightarrow } \operatorname { C o n } ( \mathrm { Z F C } + ^ { \infty } \psi ^ { , \ast } )$ . Unfortunately, the existence of a countable transitive model of $\mathrm { Z F C }$ cannot be proved from ZFC axioms (this follows from Theorem 1.1.1). Thus we need the following more refined argument. 

A closer look at the forcing method shows that it lets us extend any countable transitive set M to another countable transitive set $N = M [ G ]$ Then Theorem 9.2.2 asserts that if M satisfies ZFC then so does $M [ G ]$ However, an examination of this proof (which is not included in this text) shows that checking whether $M [ G ]$ has a given property $\varphi$ is of finitistic character in the sense that in the proof of the implication 

if M is a model for ZFC then $M [ G ]$ is a model for $^ { 6 } \varphi ^ { , 5 }$ 

(B.1) 

we use the knowledge that M is a model for a given axiom $\psi$ only for finitely many axioms $\psi$ of ZFC. In particular, for any sentence $\varphi$ for which (B.1) holds there is a finite subtheory $T _ { \varphi }$ of $\mathrm { Z F C }$ such that the implication 

if M is a model for $T _ { \varphi }$ then $M [ G ]$ is a model for $^ { 6 6 } \varphi ^ { , 9 }$ 

(B.2) 

has the same proof as (B.1). To show that such a nice proof of (F) implies $\operatorname { C o n } ( \mathrm { Z F C } ) { \Rightarrow } \operatorname { C o n } ( \mathrm { Z F C } + ^ { \infty } \psi ^ { \prime \prime } )$ we need one more theorem, which will be left without proof. 

Theorem B.2 For every finite subtheory T of ZFC it is provable in ZFC that there exists a countable transitive model M of T. 

Now, to argue for the forcing principle assume, to obtain a contradiction, that (F) holds and $\mathrm { Z F C + } ^ { \mathrm { a } } \psi ^ { \mathrm { 3 } }$ is inconsistent. Then there exists a finite subtheory S of $\mathrm { Z F C + ^ { \cdots } } \psi ^ { \ast }$ that is also inconsistent. For every $\varphi$ from $S$ let $T _ { \varphi }$ be a finite subset of ZFC for which (B.2) holds and let $T$ be the union of all $T _ { \varphi }$ for $\varphi$ from S. By Theorem B.2 there is a CTM M for $T .$ and using (B.2) we conclude that there exists a countable transitive model $N = M [ G ]$ for S. Since all of this was proved in ZFC, we can use Theorem B.1 to deduce that $\mathrm { C o n } ( \mathrm { Z F C } )$ implies Con(S). But $S$ is inconsistent, so it can only happen if ZFC is inconsistent. This finishes the argument for the forcing principle. 

We will finish this appendix with the list of $\Delta _ { 0 } .$ -formulas that constitute the 

## Proof of Lemma 9.2.5

(0) Formula $\psi _ { 0 } ( x , y )$ representing $x \subset y { \mathrm { : } }$ 

$$
\forall w \in x (w \in y).
$$

(1) Formula $\psi _ { 1 } ( x , y )$ representing $y = \cup x$ 

$$
\forall w \in y \exists z \in x (w \in z) \& \forall z \in x \forall w \in z (w \in y).
$$

(2) Formula $\psi _ { 2 } ( x , y )$ representing $y = \bigcap x !$ 

$$
\forall w \in y \forall z \in x (w \in z) \&\forall z \in x \forall w \in z [ \forall u \in x (w \in u) \rightarrow (w \in y) ].
$$

(3) Formula $\psi _ { 3 } ( x , y , z )$ representing $z = x \cup y$ : 

$$
\forall w \in z (w \in x \lor w \in y) \& \forall w \in x (w \in z) \& \forall w \in y (w \in z).
$$

(4) Formula $\psi _ { 4 } ( x , y , z )$ representing $z = x \cap y :$ 

$$
\forall w \in z (w \in x \&w \in y) \&\forall w \in x [ w \in y \rightarrow w \in z ].
$$

(5) Formula $\psi _ { 5 } ( x , y , z )$ representing $z = x \setminus y$ 

$$
\forall w \in z (w \in x \&w \notin y) \&\forall w \in x (w \notin y \rightarrow w \in z).
$$

(6) Formula $\psi _ { 6 } ( x , y , z )$ representing $z = \{ x , y \}$ : 

$$
x \in z \& y \in z \& \forall t \in z (t = x \vee t = y).
$$

(7) Formula $\psi _ { 7 } ( z )$ representing $^ { 6 6 } z$ is an unordered pair”: 

$$
\exists x \in z \exists y \in z \psi_ {6} (x, y, z).
$$

(8) Formula $\psi _ { 8 } ( x , y , z )$ representing $z = \langle x , y \rangle = \{ \{ x \} , \{ x , y \} \}$ 

$$
\exists u \in z \exists w \in z [ \psi_ {6} (x, x, u) \& \psi_ {6} (x, y, w) \& \psi_ {6} (u, w, z) ].
$$

(9) Formula $\psi _ { 9 } ( z )$ representing “z is an ordered pair”: 

$$
\exists w \in z \exists x \in w \exists y \in w \psi_ {8} (x, y, z).
$$

(10) Formula $\psi _ { 1 0 } ( x , y , z )$ representing $z = x \times y$ 

$$
\forall w \in z \exists s \in x \exists t \in y \psi_ {8} (s, t, w) \& \forall s \in x \forall t \in y \exists w \in z \psi_ {8} (s, t, w).
$$

(11) Formula $\psi _ { 1 1 } ( r )$ representing “r is a binary relation”: 

$$
\forall w \in r \psi_ {9} (w).
$$

(12) Formula $\psi _ { 1 2 } ( d , r )$ representing $^ { 6 6 } d$ is the domain of a binary relation $r ^ { \mathfrak { N } }$ 

$$
\forall x \in d \exists z \in r \exists w \in z \exists y \in w \psi_ {8} (x, y, z)
$$

$$
\&\forall z \in r \forall w \in z \forall x \in w \forall y \in w [ \psi_ {8} (x, y, z) \rightarrow x \in d ].
$$

(13) Formula $\psi _ { 1 3 } ( R , r )$ representing “R is the range of a binary relation $r ? :$ 

$$
\forall y \in R \exists z \in r \exists w \in z \exists x \in w \psi_ {8} (x, y, z)
$$

$$
\&\forall z \in r \forall w \in z \forall x \in w \forall y \in w [ \psi_ {8} (x, y, z) \rightarrow y \in R ].
$$

(14) Formula $\psi _ { 1 4 } ( f )$ representing $^ { 6 6 } f$ is a function”: 

$$
\psi_ {1 1} (f) \& \forall p \in f \forall q \in f \forall u \in p \forall w \in q \forall a \in u \forall b \in u \forall d \in w
$$

$$
[ [ \psi_ {8} (a, b, p) \&\psi_ {8} (a, d, q) ] \rightarrow b = d ].
$$

(15) Formula $\psi _ { 1 5 } ( f )$ representing “function f is injective”: 

$$
\psi_ {1 4} (f) \& \forall p \in f \forall q \in f \forall u \in p \forall w \in q \forall a \in u \forall b \in u \forall c \in w \forall d \in w
$$

$$
[ [ (\psi_ {8} (a, b, p) \&\psi_ {8} (c, d, q) \&b = d) ] \rightarrow a = c ].
$$

(16) Formula $\psi _ { 1 6 } ( \leq , \mathbb { P } )$ representing $^ { 6 6 } \leq$ is a partial-order relation on $\mathbb { P } ^ { \mathrm { , , } \mathrm { , } }$ : 

$$
\psi_ {1 1} (\leq) \& \psi_ {1 2} (\mathbb {P}, \leq) \& \psi_ {1 3} (\mathbb {P}, \leq) \& \forall x \in \mathbb {P} \exists w \in \leq \psi_ {8} (x, x, w)
$$

$$
\&\forall x \in \mathbb {P} \forall y \in \mathbb {P} \forall v \in \leq \forall w \in \leq [ (\psi_ {8} (x, y, v) \&\psi_ {8} (y, x, w)) \rightarrow x = y ]
$$

$$
\& \forall x \in \mathbb {P} \forall y \in \mathbb {P} \forall z \in \mathbb {P} \forall v \in \leq \forall w \in \leq
$$

$$
[ (\psi_ {8} (x, y, v) \&\psi_ {8} (y, z, w)) \rightarrow \exists u \in \leq \psi_ {8} (x, z, u) ].
$$

(17) Formula $\psi _ { 1 7 } ( D , \leq , \mathbb { P } )$ representing $^ { 6 6 } D$ is a dense subset of the partially ordered set $\langle \mathbb { P } , \leq \rangle \ '$ 

$$
\psi_ {1 6} (\leq , \mathbb {P}) \& \psi_ {0} (D, \mathbb {P}) \& \forall x \in \mathbb {P} \exists d \in D \exists w \in \leq \psi_ {8} (d, x, w).
$$

(18) Formula $\psi _ { 1 8 } ( A , \leq , \mathbb { P } )$ representing $^ { 6 6 } A$ is an antichain in the partially ordered set $\langle \mathbb { P } , \leq \rangle \ '$ 

$$
\psi_ {1 6} (\leq , \mathbb {P}) \& \psi_ {0} (A, \mathbb {P}) \& \forall a \in A \forall b \in A \forall x \in \mathbb {P} \forall u \in \leq \forall w \in \leq
$$

$$
[ (\psi_ {8} (x, a, u) \&\psi_ {8} (x, b, u)) \rightarrow a = b ].
$$

(19) Formula $\psi _ { 1 9 } ( x )$ representing “set x is transitive”: 

$$
\forall y \in x \forall z \in y (z \in x).
$$

(20) Formula $\psi _ { 2 0 } ( \alpha )$ representing $^ { 6 6 } \alpha$ is an ordinal number”: 

$$
\psi_ {1 9} (\alpha) \& \forall \beta \in \alpha \forall \gamma \in \alpha (\beta = \gamma \vee \beta \in \gamma \vee \gamma \in \beta).
$$

(21) Formula $\psi _ { 2 1 } ( \alpha )$ representing $^ { 6 6 } \alpha$ is a limit ordinal number”: 

$$
\psi_ {2 0} (\alpha) \& \forall \beta \in \alpha \exists \gamma \in \alpha (\beta \in \gamma).
$$

(22) Formula $\psi _ { 2 2 } ( \alpha )$ representing $^ { 6 } \alpha = \omega ^ { 5 3 }$ 

$$
\psi_ {2 1} (\alpha) \&\forall \beta \in \alpha [ \psi_ {2 1} (\beta) \rightarrow \forall x \in \beta (x \neq x) ].
$$

(23) Formula $\psi _ { 2 3 } ( \alpha )$ representing $^ { 6 6 } \alpha$ is a finite ordinal number”: 

$$
\psi_ {2 0} (\alpha) \& \neg \psi_ {2 2} (\alpha) \& \forall \beta \in \alpha (\neg \psi_ {2 2} (\beta)).
$$

(24) Formula $\psi _ { 2 3 } ( \alpha )$ representing $^ { 6 6 } \alpha$ is a successor ordinal number”: 

$$
\psi_ {2 0} (\alpha) \& \neg \psi_ {2 1} (\alpha).
$$

## Appendix C

## Notation

$x \in y - x$ is an element of y, 6. 

• ¬ϕ – the negation of formula ϕ, 6. 

• ϕ&ψ – the conjunction of formulas ϕ and ψ, 6. 

• ϕ ∨ ψ – the disjunction of formulas ϕ and ψ, 6. 

• ϕ→ψ – the implication, 6. 

• ϕ↔ψ – the equivalence of formulas ϕ and ψ, 6. 

• ∃xϕ – the existential quantifier, 6. 

• ∀xϕ – the universal quantifier, 6. 

• ∃x ∈ Aϕ – a bounded existential quantifier, 6. 

• ∀x ∈ Aϕ – a bounded universal quantifier, 6. 

• x ⊂ y – x is a subset of y, 6. 

• ∅ – the empty set, 7. 

• F – the union of a family F of sets, 8. 

• P(X) – the power set of a set X, 8. 

• x ∪ y – the union of sets x and y, 8. 

• x \ y – the diference of sets x and y, 8. 

• F – the intersection of a family F of sets, 8. 

• x ∩ y – the intersection of sets x and y, 9. 

$x \triangle y$ – the symmetric diference of sets x and y, 9. 

$\langle a , b \rangle$ – the ordered pair $\{ \{ a \} , \{ a , b \} \}$ , 9. 

$\langle a _ { 1 } , a _ { 2 } , \ldots , a _ { n - 1 } , a _ { n } \rangle$ – the ordered n-tuple, 10. 

$X \times Y$ – the Cartesian product of sets X and Y, 10. 

• S(x) – the successor of x: $x \cup \{ x \}$ , 10. 

• dom(R) – the domain of a relation (or function) R, 12. 

• range(R) – the range of a relation (or function) R, 12. 

$R ^ { - 1 } -$ the inverse of a relation (or function) R, 13. 

$S \circ R$ – the composition of the relations (or functions) R and S, 13. 

$f \colon X \to Y - \mathbf { a }$ function from a set X into a set Y, 16. 

$Y ^ { X }$ – the class of all function from a set X into a set Y, 16. 

• f[A] – the image of a set A with respect to a function f, 16. 

$f ^ { - 1 } ( B )$ – the preimage of a set B with respect to a function f, 16. 

$f | _ { A }$ – the restriction of a function f to a set A, 18. 

$\textstyle \bigcup _ { t \in T } F _ { t }$ – the union of an indexed family $\{ F _ { t } \} _ { t \in T }$ , 19. 

$\cap _ { t \in T } F _ { t }$ – the intersection of an indexed family $\{ F _ { t } \} _ { t \in T } .$ , 19. 

$\Pi _ { t \in T } F _ { t }$ – the Cartesian product of an indexed family $\{ F _ { t } \} _ { t \in T }$ , 20. 

• N – the set of natural numbers, 26. 

• ω – the set of natural numbers, 27; 

the order type of an infinite strictly increasing sequence, 39; the first infinite ordinal number, 44. 

• Z – the set of integers, 30. 

• Q – the set of rational numbers, 30. 

• R – the set of real numbers, 31. 

$B ( p , \varepsilon )$ – the open ball in $\mathbb { R } ^ { n }$ with center p and radius ε, 32. 

• int(S) – the interior of a set S in $\mathbb { R } ^ { n }$ , 33. 

• cl(S) – the closure of a set S in $\mathbb { R } ^ { n }$ , 33. 

• $\omega ^ { \star }$ – the order type of an infinite strictly decreasing sequence, 39. 

$O ( x _ { 0 } )$ – the initial segment $\{ x \in X \colon x < x _ { 0 } \}$ , 40. 

$\operatorname { O t p } ( W )$ – the order type of a well-ordered set W, 47. 

$| A |$ – the cardinality of a set A, 61. 

• $2 ^ { \kappa }$ – the cardinality of the set $\mathcal { P } ( \kappa )$ , 65. 

$\chi _ { A }$ – the characteristic function of a set A, 65. 

$\kappa ^ { + }$ – the cardinal successor of a cardinal κ, 65. 

$\omega _ { \alpha }$ – the αth infinite cardinal number, 66. 

$\aleph _ { \alpha }$ – aleph-alpha: the αth infinite cardinal number, 66. 

$\beth _ { \alpha }$ – bet-alpha, 66. 

• c – continuum: the cardinality of the set $\mathcal { P } ( \omega )$ , 66. 

$\kappa \oplus \lambda$ – the cardinal sum of cardinals κ and λ, 68. 

$\kappa \otimes \lambda$ – the cardinal product of cardinals κ and λ, 68. 

$\kappa ^ { \lambda }$ – cardinal exponentiation: the cardinality of the set $\kappa ^ { \lambda }$ , 68. 

$A ^ { < \omega }$ – the set of all finite sequences with values in $\textstyle A : \bigcup _ { n < \omega } A ^ { n } , 7 1$ 

$[ X ] ^ { \leq \kappa }$ – the family of all subsets of X of cardinality ≤ κ, 72. 

$[ X ] ^ { < \kappa }$ – the family of all subsets of X of cardinality < κ, 72. 

$[ X ] ^ { \kappa }$ – the family of all subsets of X of cardinality κ, 72. 

• C(R) – the family of all continuous functions $f \colon  { \mathbb { R } } \to  { \mathbb { R } } , 7 3$ 

$\operatorname { c f } ( \alpha )$ – the cofinality of an ordinal number α, 74. 

$\mathrm { c l } _ { \mathcal F } ( Z )$ – closure of a set Z under the action of $\mathcal { F }$ , 86. 

• $F ^ { \prime }$ – limit points of $F \subset \mathbb { R } ^ { n }$ , 92. 

$\sigma [ \mathcal { F } ]$ – the smallest σ-algebra containing $\mathcal { F }$ , 94. 

$B o r$ – the σ-algebra of Borel sets, 94. 

$\Sigma _ { \alpha } ^ { 0 }$ – subsets of Bor, 94. 

$\Pi _ { \alpha } ^ { 0 }$ – subsets of Bor, 94. 

$\mathcal { N D }$ – the ideal of nowhere-dense sets, 98. 

$\mathcal { M }$ – the σ-ideal of meager (first-category) sets, 98. 

• N – the σ-ideal of Lebesgue measure-zero (null) subsets of $\mathbb { R } ^ { n }$ , 99. 

$\mathrm { L I N } _ { \mathbb { Q } } ( B )$ – linear subspace of R over $\mathbb { Q }$ generated by $B \subset \mathbb { R }$ , 111. 

${ \mathrm { F u n c } } ( X , Y )$ – all partial functions from X into Y, 131. 

${ \mathrm { F u n c } } _ { \kappa } ( X , Y ) \ -$ all partial functions from X into Y with the domain of cardinality $< \kappa$ , 131. 

$< ^ { \star } - \mathrm { a }$ relation on $\omega ^ { \omega }$ , 135. 

$\leq ^ { \star } - \mathrm { a }$ linear-order relation on $\omega ^ { \omega }$ , 139. 

$= ^ { \star }$ – an equivalence relation on $\omega ^ { \omega }$ , 139. 

$\mathbb { P } = \mathbb { P } _ { 0 } \times \mathbb { P } _ { 1 } -$ the product of partially ordered sets $\mathbb { P } _ { 0 }$ and $\mathbb { P } _ { 1 }$ , 149, 190. 

$\operatorname { t r c l } ( x )$ – the transitive closure of x, 165. 

$R ( \alpha ) \ : - \ : 1 6 5$ 

• rank(x) – the rank of x, 166. 

$T \vdash \varphi \mathrm { ~ - ~ }$ sentence $\varphi$ is a consequence of a theory T, 167. 

• Con(T) – theory T is consistent, 167. 

$\psi ^ { M }$ – the relativization of a formula ψ to a set M, 168. 

$M \models \psi $ a formula ψ is true in M, 168. 

$M [ G ] - \mathbf { a }$ generic extension of model M, 170, 175. 

$\omega _ { 1 } ^ { M } - \omega _ { 1 }$ in model M, 175. 

${ \mathfrak { c } } ^ { M } - { \mathfrak { c } }$ in model M, 175. 

$\mathrm { v a l } _ { G } ( \tau )$ – valuation of a P-name τ, 175. 

• Γ – standard P-name for a generic filter in P, 176. 

$p \parallel { - } _ { \mathbb { P } , M } \varphi - p$ forces $\varphi ,$ 176. 

• @− – forcing relation, 176. 

$\mathbb { P } \Vdash \varphi \mathrm { - } \mathrm { e v e r y }$ $p \in \mathbb { P }$ forces $\varphi , 1 7 7$ 

$\pi \Vdash _ { P } ^ { \star } \varphi ( x _ { 1 } , \ldots , x _ { n } )$ – formula for $^ { \circ } p$ forces $\varphi ( x _ { 1 } , \ldots , x _ { n } ) , ^ { * }$ 177. 

$\| - ^ { \star } - 1 7 7 .$ 

• P(Z) – Cohen forcing on a set Z, 192. 

$\mathbb { P } \star \pi$ – iteration of P and a good P-name π, 200. 

$G _ { 0 } \star G _ { 1 } - 2 0 0$ 

## References



Cantor, G. 1899. Correspondence between Cantor and Dedekind (in German). In Cantor (1932: 443–51). 





Cantor, G. 1932. Gesammelte Abhandlungen: Mathematischen und philosophischen Inhalts. Berlin: Springer. 



Ciesielski, K. 1995–6. Uniformly antisymmetric functions and $K _ { 5 }$ . Real Anal. Exchange 21: 147–53. 

Ciesielski, K. 1996. Sum and diference free partitions of vector spaces. Colloq. Math. 71: 263–71. 



Ciesielski, K., and Larson, L. 1993–4. Uniformly antisymmetric functions. Real Anal. Exchange 19: 226–35. 





Ciesielski, K., and Miller, A. W. 1994–5. Cardinal invariants concerning functions whose sum is almost continuous. Real Anal. Exchange 20: 657–72. 





Erd˝os, P. 1969. Problems and results in chromatic graph theory. In Proof techniques in graph theory, ed. F. Harary, 27–35. New York: Academic Press. 



Erd˝os, P. 1978–9. Measure theoretic, combinatorial and number theoretic problems concerning point sets in Euclidean space. Real Anal. Exchange 4: 113–38. 



Erd˝os, P., and Kakutani, S. 1943. On non-denumerable graphs. Bull Amer. Math. Soc. 49: 457–61. 





Fraenkel, A. A. 1922. Zu den Grundlagen der Cantor-Zermeloschen Mengenlehre. Math. Ann. 86: 230–7. 



Frege, G. [1893] 1962. Grundgesetze der Arithmetik. Vol 1. Reprint. Hildesheim: Olms. 



Freiling, C. 1986. Axioms of symmetry: throwing darts at the real number line. J. Symb. Logic 51: 190–200. 





Freiling, C. 1989–90. A converse to a theorem of Sierpi´nski on almost symmetric sets. Real Anal. Exchange 15: 760–7. 





Friedman, H. 1980. A consistent Fubini-Tonelli theorem for non-measurable functions. Illinois J. Math. 24: 390–5. 





Galvin, F. 1980. Chain conditions and products. Fund. Math. 108: 33–48. 





Kirchheim, B., and Natkaniec, T. 1990–1. On universally bad Darboux functions. Real Anal. Exchange 16: 481–6. 





Komj´ath, P., and Shelah, S. 1993–4. On uniformly antisymmetric functions. Real Anal. Exchange 19: 218–25. 





Kunen, K. 1980. Set Theory. Amsterdam: North-Holland. 





Levi, B. 1902. Intorno alla teoria degli aggregati. Rendic., 2d ser. 35: 863–8. 





Levy, A. 1979. Basic Set Theory. New York: Springer-Verlag. 





Mazurkiewicz, S. 1914. Sur un ensemble plan (in Polish). Comptes Rendus Sci. et Lettres de Varsovie 7: 382–3. French translation reprinted in Travaux de Topologie et ses Applications, 46–7. Warsaw: Polish Scientific Publishers PWN, 1969. 





Mirimanof, D. 1917. Les antinomies de Russell et de Burali-Forti et le probl`eme fondamental de la th´eorie des ensembles. L’Enseignement Math. 19: 37–52. 





Royden, H. L. 1988. Real Analysis. 3d ed. New York: Macmillan. 





Russell, B. 1903. The Principles of Mathematics. Vol. 1. Cambridge: Cambridge University Press. 





Sierpi´nski, W. 1919. Sur un th´eor`em ´equivalent `a l’hypoth`ese du continu. Bull Int. Acad. Sci. Cracovie A: 1–3. Reprinted in Oeuvres Choisies, vol. 2, 272–4. Warsaw: Polish Scientific Publishers PWN, 1974. 





Sierpi´nski, W. 1920. Sur les rapports entre l’existence des int´egrales $\begin{array} { r } { \int _ { 0 } ^ { 1 } f ( x , y ) d x , \int _ { 0 } ^ { 1 } f ( x , y ) d y \mathrm { e t } \int _ { 0 } ^ { 1 } d x \int _ { 0 } ^ { 1 } f ( x , y ) d y . } \end{array}$ Fund. Math. 1: * * * *142–7. Reprinted in Oeuvres Choisies, vol. 2, 341–5. Warsaw: Polish Scientific Publishers PWN, 1974. 





Sierpi´nski, W. 1936. Sur une fonction non measurable partout presque symetrique. Acta Litt. Scient (Szeged) 8: 1–6. Reprinted in Oeuvres Choisies, vol. 3, 277–81. Warsaw: Polish Scientific Publishers PWN, 1974. 





Skolem, D. 1922. Einige Bemerkungen zur axiomatischen Begr¨undung der Mengenlehre. In Proceedings of the 5th Scandinavian Mathematicians’ Congress in Helsinki, 1922, 217–32. 





Stepr¯ans, J. 1993. A very discontinuous Borel function. J. Symbolic Logic 58: 1268–83. 





von Neumann, J. 1925. Zur Einf¨uhrung der transfiniten Zahlen. Acta Sci. Math. (Szeged) 1: 199–208. 





von Neumann, J. 1929. Eine Widerspruchsfreiheitsfrage in der axiomatischen Mengenlehre. Crelle J. 160: 227. 





Zermelo, E. 1904. Beweis, daß jede Menge wohlgeordnet werden kann. Math. Ann. 59: 514–16. 





Zermelo, E. 1908. Untersuchungen ¨uber die Grundlagen der Mengenlehre, I. Math. Ann. 65: 261–81. 



## Index

Abelian group, 55 absolute property, 172, 182 AC, 15 additive function, 111, 117 Jones space of, 114 Alexander subbase theorem, 58 algebraic numbers, 73 algebraically independent subset, 60 almost contained ⊂<sup></sup>, 153 almost-disjoint sets, 153 antichain, 140, 174, 177 maximal, 140 antilexicographic-order relation, 43 antisymmetric function, 119 antisymmetric relation, 21 arithmetic of cardinal numbers, 68 of ordinal numbers, 48 Peano axioms of, 26 Aronszajn tree, 163 axiom of choice, 4, 15, 18, 20, 52, 54, 101 axiom of empty set, 7 axiom of extensionality, 6 axiom of foundation, 37 axiom of infinity, 10, 26, 182 axiom of pairing, 8 axiom of power set, 8 axiom of regularity, 37 axiom of set existence, 6 

axiom of union, 8 axiom schema of comprehension, 3 axiom schema of separation, 7 Baire category theorem, 33, 98 Baire class-one function, 73 Baire property, 98 Baire-measurable functions, 104 base, 58 for R<sup>n</sup>, 89 basis Hamel, 111, 115 with Baire property, 117 without Baire property, 113 measurable, 117 nonmeasurable, 113 of a linear space, 55 transcendental, 60 Bernstein set, 103–5, 112, 117, 126 bijection, 16 binary relation, 12, 173 B-measurable functions, 104 Borel functions, 104 Borel sets, 89, 97 Borel σ-algebra Bor, 94 bound variables in a formula, 166 bounded quantifier, 168 bounded subset of R<sup>n</sup>, 33 branch of a tree, 163 

Cantor set, 71, 93, 111, 117 Cantor–Bendixson theorem, 92 Cantor’s theorem, 64 cardinal number, 62 collapsing of, 180, 185 preservation of, 180, 188 regular, 75, 144 successor of, 65 cardinal numbers arithmetic of, 68 exponentiation of, 68 product of, 68 sum of, 68 union of, 65 cardinality continuum c, 66, 76, 195 of a set, 61 Cartesian product, 10, 20 Cauchy sequence, 14, 33 ccc forcing, 140, 149, 150, 179–81, 195 ccc iteration, 202, 206 ccc linearly ordered set, 154, 162 Ceder’s theorem, 89 CH, 66 chain in a partially ordered set, 52 characteristic function, 65 choice function, 18 Ciesielski–Larson theorem, 119, 121 Ciesielski’s theorem, 124 class equivalence, 14 proper, of sets, 7, 44, 168 quotient, 14 of sets, 7 closed set under the action of F, 85, 97 closed subset of R<sup>n</sup>, 32, 89 closed unbounded subsets of ω , 157 diagonal intersection of, 161 

closure cl(S) of a set in R<sup>n</sup>, 33 cl (Z) of a set under the action of F, 85 transitive, trcl(x), 165 cofinality cf(α) of an ordinal num ber, 74 Cohen model, 182, 189 Cohen real numbers, 182 collapsing of cardinal numbers, 180, 185 compact subset of R<sup>n</sup>, 33 compact topological space, 58 comparable elements in a partially ordered set, 140 compatible elements in a partially ordered set, 140 compatible set, 147 complete Boolean algebra, 140 complete linearly ordered set, 135, 154 complete linear-order relation, 135, 154 complete set of axioms, 4 composition of relations, 13 comprehension, axiom schema of, 3 comprehension scheme, 7 condition. 132 ccc, 140 stronger, 132 conditions comparable, 140 compatible, 140 incompatible, 140 connected relation, 23 connected subset of R<sup>n</sup>, 33, 114 consistent set of axioms, 4 consistent theory, 167 consistent with ZFC, 66, 133, 141, 155, 168 constants in the language of set theory, 6, 168, 171, 174 

continuous function, 33, 72, 107, 111 continuum c, 66, 76, 195 continuum hypothesis, 66, 87, 89, 105, 108, 111, 115, 122, 124, 129, 136, 139, 157, 168, 183 generalized, 66, 107 countable chain condition ccc, 140 countable set, 64 countably closed forcing, 183 cover, 58 Darboux function, 106 decreasing function, 41 strictly, 41, 51 Dedekind cut, 31 definitions by recursion, 49 definitions by transfinite induction, 49 ∆ -formula, 172 ∆-system lemma, 150, 151, 153, 154, 181, 206 dense set, weakly, 139 dense set below p, 183 dense subset of a linearly ordered set, 133, 135, 154 dense subset of a partially ordered set, 130, 132, 141, 174 dense subset of R<sup>n</sup>, 33, 79, 99, 117 diagonal intersection of closed and unbounded sets, 162 diagonalization, 81, 129, 198 diamond principle ♦, 158, 182 ♦-sequence, 158 diference of sets, 8 symmetric, 9 diference-free partition, 124 discrete space, 94 discrete subset of R<sup>n</sup>, 89 distance in R<sup>n</sup>, 32, 86 domain of a function, 16 

domain of a relation, 12, 173 empty set axiom, 7 equivalence class, 14 equivalence relation, 14, 100 Erd˝os–Hajnal theorem, 86, 115 Erd˝os–Kakutani theorem, 115 Euclidean space R<sup>n</sup>, 32 exponentiation of cardinal numbers, 68 extension of a function, 18 generic, 170 extensionality axiom, 6 field, 55 of a relation, 12 filter, 60, 130 F-generic, 132 generic, 169 prime, 60 principal, 131 proper, 60 finite set, 64 first element, 22 first-category set, 98, 144 Fodor’s theorem, 162 forcing, 132 cardinal-collapsing, 180 cardinal-preserving, 180, 188 countably closed, 183 iterated, 189 forcing method, 164 forcing principle, 169 forcing relation @−, 177 forest in a graph, 60 formal proof, 167 formula, 6, 166 a consequence of a theory, 167 ∆ -, 172 @−<sup></sup> representing forcing relation, 177 relativization of, 168 

free variable, 166 F set, 94 Fubini–Tonelli theorem, 105 function, 16 GCH, 66 G set, 94, 99 generalized continuum hypothesis, 66, 107 generic extension of a model, 170 generic filter, 132, 169 G¨odel’s incompleteness theorem first, 5, 167 second, 4, 167 good P-name, 199 graph on a set, 60 bipartite, 116 forest in, 60 greatest element, 22, 39 ground model, 170 group, 55 Abelian, 55 Hahn–Banach theorem, 54, 56 Hamel basis, 111, 115 with Baire property, 117 without Baire property, 113 measurable. 117 nonmeasurable, 113 Hausdorf maximal principle, 54, 140 ideal, 14, 98 of nowhere-dense sets ND, 98 image, 16 incompatible elements in a partially ordered set, 140 inconsistent theory, 167 increasing function, 41 strictly, 41, 47, 74, 138, 139 independence algebraic, 60 of the axioms, 5 

linear, 55, 113, 123 from ZFC, 5, 66, 110, 164, 166, 168, 183 index set, 19 indexed family, 19 induction on natural numbers, 27 too short, 130 transfinite, 40, 198 definitions by, 49 infinite set, 64 infinity axiom, 10, 26, 182 initial ordinal number, 62 initial segment, 31, 39 proper, 40, 41 injective function, 16 integers, 30 integral, 105 interior int(S) of a set, 32 intermediate value theorem, 106 intersection of sets, 8, 19 diagonal, 162 inverse relation, 13 isolated point, 89 isomorphism of ordered sets, 39, 41, 47, 134, 135, 185 iterated forcing, 189 iterated integral, 105 iteration of ccc forcings, 202, 206 iteration of partially ordered sets, 200, 204 Jones space, 114 Kirchheim–Natkaniec theorem, 108 Kuratowski’s theorem, 126 language of set theory, 4, 6, 166 largest element, 22 last element, 22 least element, 22 least upper bound, 135 Lebesgue measure, 101 

## Index

Lebesgue measure-zero set, 98, 117, 145, 193, 194 Lebesgue-measurable functions, 104 Lebesgue-measurable Hamel basis, 117 Lebesgue-measurable sets, 98 lexicographic-order relation, 43 limit points F<sup>-</sup> of F ⊂ R<sup>n</sup>, 92 linear function, 111 linear functional, 56 linear space, 55 basis of, 55 linear subspace, 55, 111 linearly independent subset, 55, 113, 123 linearly ordered set, 23, 39, 42 linear-order relation, 23, 60, 139, 156 lower bound, 52 

MA, 141 map, 16 cofinal, 74 Martin’s axiom MA, 141, 155, 195, 196 maximal antichain, 140 maximal element, 22, 39, 53, 54 Mazurkiewicz’s theorem, 81 meager set, 98, 144 minimal element, 22, 39 model Cohen, 182, 189 ground, 170 for theory T, 168 for ZFC, 169 for ZFC+“c = ω ,” 195 for ZFC+♦, 182 for ZFC+MA+¬CH, 196 for ZFC+¬CH, 168 for ZFC+¬MA, 195 for ZFC+“2<sup>ω1</sup> = ω ,” 188 

natural numbers, 4, 25 non-Baire functions, 104 non-Borel functions, 104 nonmeasurable functions, 104 nowhere-constant function, 108 nowhere-dense set, 33, 98, 110, 117 nowhere–symmetrically continuous function, 118 null set, 98, 145, 193, 194 one-to-one function, 16 onto function, 16 open ball B(p, ε) in R<sup>n</sup>, 32 open cover, 58 open set in R<sup>n</sup>, 32, 89 order isomorphism, 39, 41, 47, 134, 135, 185 order relation antilexicographic-, 43 complete, 135, 154 lexicographic-, 43 linear-, 23, 60, 139, 156 partial-, 21, 60, 174 order topology, 154, 157 order type η, 135 λ, 135 ω<sup></sup>, 51 Otp(W) of a well-ordered set, 47 of a partially ordered set, 38 ordered n-tuple, 10 ordered pair, 9, 173 order-isomorphic partially ordered sets, 38 ordinal number, 44, 90, 174, 196 cofinality of, 74 initial, 62 limit, 46, 174 successor of, 46, 174 

ordinal numbers arithmetic of, 48 product of, 48 sum of, 48 pairing axiom, 8 partial functions Func(X, Y) from X into Y, 131 partially ordered set, 22 partially ordered sets iteration of, 200, 204 order isomorphic, 38 product of, 149, 150 partial-order relation, 21, 60, 174 partition, 14, 86, 115, 119 diference-free, 124 sum-free, 124 Peano axioms of arithmetic, 26 perfect subset of R<sup>n</sup>, 89, 90, 101, 102 P-name, 175, 177 good, 199 valuation of, 175 poset, 22 power set, 8 power set axiom, 8 preimage, 16 preorder relation, 24, 139 preservation, in induction proofs, 81 preservation of cardinal numbers, 180, 188 preservation of properties in generic extensions, 172 pressing-down lemma, 162 principle of mathematical induction, 26 principle of transfinite induction, 40 product of cardinal numbers, 68 Cartesian, 10, 20 of ordinal numbers, 48 

of partially ordered sets, 149, 150 Tychonof, 58 product lemma, 190 proper initial segment, 40, 41 quantifier, 6, 166 bounded, 168 unbounded, 168 quotient class, 14 range of a function, 16 range of a relation, 12, 174 rank of a set, 166 Rasiowa–Sikorski lemma, 132, 139, 169 rational numbers, 30 real function, 104 real numbers, 25, 31 Cohen, 182 recursion definitions, 49 recursion theorem, 49 reflexive relation, 13 regressive function, 162 regular cardinal numbers, 75, 144 relation antisymmetric, 21 binary, 12, 173 connected, 23 domain of, 12, 173 equivalence, 14, 100 forcing @−, 177 @−<sup></sup>, 177 inverse, 13 order antilexicographic-, 43 complete, 135, 154 lexicographic-, 43 linear-, 23, 60, 139, 156 partial-, 21, 60, 174 preorder, 24, 139 range of, 12, 174 reflexive, 13 

restriction of, 23 =<sup></sup>, 139 <<sup></sup>, 136 ≤<sup></sup>, 139 symmetric, 13 transitive, 13 well-founded, 37, 163 well-ordering, 38, 90 relations composition of, 13 in the language of set theory, 168 replacement scheme axiom, 17 restriction of a function, 18 restriction of an order relation, 23 Russell’s paradox, 3, 7 scale, 136, 141 Schr¨oder–Bernstein theorem, 64 selector, 15, 117 sentence, 167 a consequence of a theory, 167 consistent with a theory, 167 independent of a theory, 5, 167 sequence, 18 Cauchy, 14, 33 ♦-, 158 transfinite, 48 set-theoretic universe, 7 Sierpi´nski–Zygmund theorem, 111 Sierpi´nski’s theorem, 88, 105 σ-algebra, 93 of Borel sets Bor, 94 of Lebesgue-measurable sets L, 101 of sets Baire with the Baire property, 101 σ-ideal, 98 of first-category sets, 98, 144 of Lebesgue measure-zero sets, 98, 145, 193, 194 of meager sets, 98, 144 

of null sets, 98, 145, 193, 194 smallest element, 22, 39 stationary set. 158. 162 strong measure-zero set, 153 strongly Darboux function, 106 subbase of a topological space, 58 subcover, 58 successor, 10, 26 of a cardinal number, 65 of an ordinal number, 46, 174 sum of cardinal numbers, 68 sum of ordinal numbers, 48 sum-free partition, 124 surjective function, 16 Suslin hypothesis SH, 155 Suslin line, 155 Suslin tree, 163 symmetric diference, 9 symmetric relation, 13 symmetrically continuous function, 118 nowhere, 118 theory, 167 consistent, 167 inconsistent, 167 topological properties of R<sup>n</sup>, 32 topological space, 58 base of, 58 Borel structure of, 93 compact, 58 discrete, 94 subbase of, 58 topology, 58 order, 154, 157 on R<sup>n</sup>, 32 transcendental basis, 60 transfinite induction, 40, 198 definitions by, 49 transfinite sequence, 48 transformation, 16 transitive closure trcl(x) of a set, 165 

transitive model of ZFC, 169 transitive relation, 13 transitive set, 164, 174 tree, 163 Aronszajn, 163 branch of, 163 Suslin, 163 tree construction, 92, 102 Tychonof product, 58 Tychonof theorem, 54, 58 unbounded quantifier, 168 unbounded subset in an ordinal number, 74 uncountable set, 64 uniformly antisymmetric function, 119 union axiom, 8 union of cardinal numbers, 65 union of sets, 8 upper bound, 52 least, 135 

valuation, 175 variable, 6, 166 bound, 166 free, 166 vector space, 55 Vitali set, 117, 126 weakly dense set, 139 well-founded relation, 37, 163 well-ordered set, 38, 39, 42, 47, 51 type of, 47 well-ordering relation, 38, 90 well-ordering theorem, 51 Zermelo–Fraenkel axioms, 4 Zermelo’s theorem, 51 ZF, 52 ZFC, 4 Zorn’s lemma, 53, 54 