

<!-- === Source: MinerU_markdown_An_introduction_to_measure_theory,_T._Tao,_text_1_2122707919320489992.md (Page 1) === -->

# An introduction to measure theory

Terence Tao 

Department of Mathematics<sub>,</sub> UCLA<sub>,</sub> Los Angeles<sub>,</sub> CA 90095 

E-mail address: tao@math.ucla.edu 

To Garth Gaudry, who set me on the road; 

To my family, for their constant support; 

And to the readers of my blog, for their feedback and contributions. 

## Contents

Preface ix
Notation x
Acknowledgments xvi
Chapter 1. Measure theory 1
§1.1. Prologue: The problem of measure 2
§1.2. Lebesgue measure 17
§1.3. The Lebesgue integral 46
§1.4. Abstract measure spaces 79
§1.5. Modes of convergence 114
§1.6. Differentiation theorems 131
§1.7. Outer measures, pre-measures, and product measures 179
Chapter 2. Related articles 209
§2.1. Problem solving strategies 210
§2.2. The Radamacher differentiation theorem 226
§2.3. Probability spaces 232
§2.4. Infinite product spaces and the Kolmogorov extension theorem 235
Bibliography 243 

## Preface

In the fall of 2010, I taught an introductory one-quarter course on graduate real analysis, focusing in particular on the basics of measure and integration theory, both in Euclidean spaces and in abstract measure spaces. This text is based on my lecture notes of that course, which are also available online on my blog terrytao.wordpress.com, together with some supplementary material, such as a section on problem solving strategies in real analysis (Section 2.1) which evolved from discussions with my students. 

This text is intended to form a prequel to my graduate text [Ta2010] (henceforth referred to as An epsilon of room, Vol. I), which is an introduction to the analysis of Hilbert and Banach spaces (such as L<sup>p</sup> and Sobolev spaces), point-set topology, and related topics such as Fourier analysis and the theory of distributions; together, they serve as a text for a complete first-year graduate course in real analysis. 

The approach to measure theory here is inspired by the text [StSk2005], which was used as a secondary text in my course. In particular, the first half of the course is devoted almost exclusively to measure theory on Euclidean spaces $\mathbf { R } ^ { d }$ (starting with the more elementary Jordan-Riemann-Darboux theory, and only then moving on to the more sophisticated Lebesgue theory), deferring the abstract aspects of measure theory to the second half of the course. I found that this approach strengthened the student’s intuition in the early stages of the course, and helped provide motivation for more abstract constructions, such as Carath´eodory’s general construction of a measure from an outer measure. 

Most of the material here is self-contained, assuming only an undergraduate knowledge in real analysis (and in particular, on the Heine-Borel theorem, which we will use as the foundation for our construction of Lebesgue measure); a secondary real analysis text can be used in conjunction with this one, but it is not strictly necessary. A small number of exercises however will require some knowledge of point-set topology or of set-theoretic concepts such as cardinals and ordinals. 

A large number of exercises are interspersed throughout the text, and it is intended that the reader perform a significant fraction of these exercises while going through the text. Indeed, many of the key results and examples in the subject will in fact be presented through the exercises. In my own course, I used the exercises as the basis for the examination questions, and signalled this well in advance, to encourage the students to attempt as many of the exercises as they could as preparation for the exams. 

The core material is contained in Chapter 1, and already comprises a full quarter’s worth of material. Section 2.1 is a much more informal section than the rest of the book, focusing on describing problem solving strategies, either specific to real analysis exercises, or more generally applicable to a wider set of mathematical problems; this section evolved from various discussions with students through out the course. The remaining three sections in Chapter 2 are optional topics, which require understanding of most of the material in Chapter 1 as a prerequisite (although Section 2.3 can be read after completing Section 1.4. 

## Notation

For reasons of space, we will not be able to define every single mathematical term that we use in this book. If a term is italicised for reasons other than emphasis or for definition, then it denotes a standard mathematical object, result, or concept, which can be easily looked up in any number of references. (In the blog version of the book, many of these terms were linked to their Wikipedia pages, or other on-line reference pages.) 

Given a subset E of a space $X$ , the indicator function $1 _ { E } : X  \mathbf { R }$ is defined by setting $1 _ { E } ( x )$ equal to 1 for $x \in E$ and equal to 0 for x $\notin E$ 

For any natural number $d ,$ we refer to the vector space $\mathbf { R } ^ { d } : = \mathbf { \partial }$ $\{ ( x _ { 1 } , \dotsc , x _ { d } ) : x _ { 1 } , \dotsc , x _ { d } \in \mathbf { R } \}$ as (d-dimensional) Euclidean space. A vector $( x _ { 1 } , \ldots , x _ { d } )$ in $\mathbf { R } ^ { d }$ has length 

$$
| (x _ {1}, \dots , x _ {d}) | := (x _ {1} ^ {2} + \dots + x _ {d} ^ {2}) ^ {1 / 2}
$$

and two vectors $( x _ { 1 } , \ldots , x _ { d } ) , ( y _ { 1 } , \ldots , y _ { d } )$ have dot product 

$$
(x _ {1}, \dots , x _ {d}) \cdot (y _ {1}, \dots , y _ {d}) := x _ {1} y _ {1} + \dots + x _ {d} y _ {d}.
$$

The extended non-negative real axis $[ 0 , + \infty ]$ is the non-negative real axis $[ 0 , + \infty ) : = \{ x \in \mathbf { R } : x \geq 0 \}$ with an additional element adjointed to it, which we label +∞; we will need to work with this system because many sets $( \mathrm { e . g . ~ } \ \mathbf { R } ^ { d } )$ will have infinite measure. Of course, +∞ is not a real number, but we think of it as an extended real number. We extend the addition, multiplication, and order structures on $[ 0 , + \infty )$ to $[ 0 , + \infty ]$ by declaring 

$$
+ \infty + x = x + + \infty = + \infty
$$

for all $x \in [ 0 , + \infty ]$ 

$$
+ \infty \cdot x = x \cdot + \infty = + \infty
$$

for all non-zero $x \in ( 0 , + \infty ]$ • 

$$
+ \infty \cdot 0 = 0 \cdot + \infty = 0,
$$

and 

$$
x <   + \infty \text {   for   all   } x \in [ 0, + \infty).
$$

Most of the laws of algebra for addition, multiplication, and order continue to hold in this extended number system; for instance addition and multiplication are commutative and associative, with the latter distributing over the former, and an order relation $x \le y$ is preserved under addition or multiplication of both sides of that relation by the same quantity. However, we caution that the laws of cancellation do not apply once some of the variables are allowed to be infinite; for instance, we cannot deduce $x = y { \mathrm { ~ f r o m ~ } } + \infty + x = + \infty + y$ or from $+ \infty \cdot x = + \infty \cdot y$ . This is related to the fact that the forms $+ \infty - + \infty \ \mathrm { a n d \ } + \infty / + \infty$ are indeterminate (one cannot assign a value to them without breaking a lot of the rules of algebra). A general rule of thumb is that if one wishes to use cancellation (or proxies for cancellation, such as subtraction or division), this is only safe if one can guarantee that all quantities involved are finite (and in the case of multiplicative cancellation, the quantity being cancelled also needs to be non-zero, of course). However, as long as one avoids using cancellation and works exclusively with non-negative quantities, there is little danger in working in the extended real number system. 

We note also that once one adopts the convention $+ \infty \cdot 0 \ =$ $0 \cdot + \infty = 0$ , then multiplication becomes upward continuous (in the sense that whenever $x _ { n } ~ \in ~ [ 0 , + \infty ]$ increases to $x \in [ 0 , + \infty ]$ , and $y _ { n } \in [ 0 , + \infty ]$ increases to $y \in [ 0 , + \infty ]$ , then $x _ { n } y _ { n }$ increases to xy) but not downward continuous $( \mathrm { e . g . ~ \ 1 / n \to 0 }$ but $1 / n \cdot + \infty \not  0$ $+ \infty )$ . This asymmetry will ultimately cause us to define integration from below rather than from above, which leads to other asymmetries (e.g. the monotone convergence theorem (Theorem 1.4.44) applies for monotone increasing functions, but not necessarily for monotone decreasing ones). 

Remark 0.0.1. Note that there is a tradeof here: if one wants to keep as many useful laws of algebra as one can, then one can add in infinity, or have negative numbers, but it is dificult to have both at the same time. Because of this tradeof, we will see two overlapping types of measure and integration theory: the non-negative theory, which involves quantities taking values in $[ 0 , + \infty ]$ , and the absolutely integrable theory, which involves quantities taking values in $( - \infty , + \infty )$ or C. For instance, the fundamental convergence theorem for the former theory is the monotone convergence theorem (Theorem 1.4.44), while the fundamental convergence theorem for the latter is the dominated convergence theorem (Theorem 1.4.49). Both branches of the theory are important, and both will be covered in later notes. 

One important feature of the extended nonnegative real axis is that all sums are convergent: given any sequence $x _ { 1 } , x _ { 2 } , . . . \in [ 0 , + \infty ]$ , 

we can always form the sum 

$$
\sum_ {n = 1} ^ {\infty} x _ {n} \in [ 0, + \infty ]
$$

as the limit of the partial sums $\textstyle \sum _ { n = 1 } ^ { N } x _ { n }$ , which may be either finite or infinite. An equivalent definition of this infinite sum is as the supremum of all finite subsums: 

$$
\sum_ {n = 1} ^ {\infty} x _ {n} = \sup _ {F \subset \mathbf {N}, F} \text { finite } \sum_ {n \in F} x _ {n}.
$$

Motivated by this, given any collection $( x _ { \alpha } ) _ { \alpha \in A }$ of numbers $x _ { \alpha } \in$ $[ 0 , + \infty ]$ indexed by an arbitrary set A (finite or infinite, countable or uncountable), we can define the sum $\textstyle \sum _ { \alpha \in A } x _ { \alpha }$ by the formula 

$$
\sum_ {\alpha \in A} x _ {\alpha} = \sup _ {F \subset A, F \text {   finite }} \sum_ {\alpha \in F} x _ {\alpha}.\tag{0.1}
$$

Note from this definition that one can relabel the collection in an arbitrary fashion without afecting the sum; more precisely, given any bijection $\phi : B  A$ , one has the change of variables formula 

$$
\sum_ {\alpha \in A} x _ {\alpha} = \sum_ {\beta \in B} x _ {\phi (\beta)}.\tag{0.2}
$$

Note that when dealing with signed sums, the above rearrangement identity can fail when the series is not absolutely convergent (cf. the Riemann rearrangement theorem). 

Exercise 0.0.1. If $( x _ { \alpha } ) _ { \alpha \in A }$ is a collection of numbers $x _ { \alpha } \in [ 0 , + \infty ]$ such that $\textstyle \sum _ { \alpha \in A } x _ { \alpha } \ < \ \infty$ , show that $x _ { \alpha } = 0$ for all but at most countably many $\alpha \in A$ , even if A itself is uncountable. 

We will rely frequently on the following basic fact (a special case of the Fubini-Tonelli theorem, Corollary 1.7.23): 

Theorem 0.0.2 (Tonelli’s theorem for series). Let $( x _ { n , m } ) _ { n , m \in \mathbf { N } }$ be a doubly infinite sequence ofextended non-negative reals $x _ { n , m } \in [ 0 , + \infty ]$ Then 

$$
\sum_ {(n, m) \in \mathbf {N} ^ {2}} x _ {n, m} = \sum_ {n = 1} ^ {\infty} \sum_ {m = 1} ^ {\infty} x _ {n, m} = \sum_ {m = 1} ^ {\infty} \sum_ {n = 1} ^ {\infty} x _ {n, m}.
$$

Informally, Tonelli’s theorem asserts that we may rearrange infi nite series with impunity as long as all summands are non-negative. 

Proof. We shall just show the equality of the first and second expressions; the equality of the first and third is proven similarly. 

We first show that 

$$
\sum_ {(n, m) \in \mathbf {N} ^ {2}} x _ {n, m} \leq \sum_ {n = 1} ^ {\infty} \sum_ {m = 1} ^ {\infty} x _ {n, m}.
$$

Let $F$ be any finite subset of ${ \bf N } ^ { 2 }$ . Then $F \subset \{ 1 , \dots , N \} \times \{ 1 , \dots , N \}$ for some finite N, and thus (by the non-negativity of the $x _ { n , m } )$ 

$$
\sum_ {(n, m) \in F} x _ {n, m} \leq \sum_ {(n, m) \in \{1, \dots , N \} \times \{1, \dots , N \}} x _ {n, m}.
$$

The right-hand side can be rearranged as 

$$
\sum_ {n = 1} ^ {N} \sum_ {m = 1} ^ {N} x _ {n, m},
$$

which is clearly at most $\textstyle \sum _ { n = 1 } ^ { \infty } \sum _ { m = 1 } ^ { \infty } x _ { n , m }$ (again by non-negativity of $x _ { n , m } )$ . This gives 

$$
\sum_ {(n, m) \in F} x _ {n, m} \leq \sum_ {n = 1} ^ {\infty} \sum_ {m = 1} ^ {\infty} x _ {n, m}.
$$

for any finite subset $F$ of ${ \bf N } ^ { 2 }$ , and the claim then follows from (0.1). 

It remains to show the reverse inequality 

$$
\sum_ {n = 1} ^ {\infty} \sum_ {m = 1} ^ {\infty} x _ {n, m} \leq \sum_ {(n, m) \in \mathbf {N} ^ {2}} x _ {n, m}.
$$

It sufices to show that 

$$
\sum_ {n = 1} ^ {N} \sum_ {m = 1} ^ {\infty} x _ {n, m} \leq \sum_ {(n, m) \in \mathbf {N} ^ {2}} x _ {n, m}
$$

for each finite N. 

Fix N. As each $\textstyle \sum _ { m = 1 } ^ { \infty } x _ { n , m }$ is the limit of $\textstyle \sum _ { m = 1 } ^ { M } x _ { n , m }$ , the lefthand side is the limit of $\begin{array} { r } { \sum _ { n = 1 } ^ { N } \sum _ { m = 1 } ^ { M } x _ { n , m } } \end{array}$ as $M  \infty$ . Thus it 

sufices to show that 

$$
\sum_ {n = 1} ^ {N} \sum_ {m = 1} ^ {M} x _ {n, m} \leq \sum_ {(n, m) \in \mathbf {N} ^ {2}} x _ {n, m}
$$

for each finite M. But the left-hand side is $\sum _ { \substack { ( n , m ) \in \{ 1 , \dots , N \} \times \{ 1 , \dots , M \} } } x _ { n , m ; }$ , and the claim follows. 

Remark 0.0.3. Note how important it was that the $x _ { n , m }$ were nonnegative in the above argument. In the signed case, one needs an additional assumption of absolute summability of $x _ { n , m }$ on ${ \bf N } ^ { 2 }$ before one is permitted to interchange sums; this is Fubini’s theorem for series, which we will encounter later in this text. Without absolute summability or non-negativity hypotheses, the theorem can fail (consider for instance the case when $x _ { n , m }$ equals +1 when $n = m , - 1$ when $n = m + 1$ , and 0 otherwise). 

Exercise 0.0.2 (Tonelli’s theorem for series over arbitrary sets). Let A, B be sets (possibly infinite or uncountable), and $( x _ { n , m } ) _ { n \in A , m \in B }$ be a doubly infinite sequence of extended non-negative reals $x _ { n , m } \in$ $[ 0 , + \infty ]$ indexed by A and B. Show that 

$$
\sum_ {(n, m) \in A \times B} x _ {n, m} = \sum_ {n \in A} \sum_ {m \in B} x _ {n, m} = \sum_ {m \in B} \sum_ {n \in A} x _ {n, m}.
$$

(Hint: although not strictly necessary, you may find it convenient to first establish the fact that if $\textstyle \sum _ { n \in A } x _ { n }$ is finite, then $x _ { n }$ is non-zero for at most countably many n.) 

Next, we recall the axiom of choice, which we shall be assuming throughout the text: 

Axiom 0.0.4 (Axiom of choice). Let $( E _ { \alpha } ) _ { \alpha \in A }$ be a family of nonempty sets $E _ { \alpha }$ , indexed by an index set A. Then we can find a family $( x _ { \alpha } ) _ { \alpha \in A }$ of elements $x _ { \alpha }$ of $E _ { \alpha }$ , indexed by the same set A. 

This axiom is trivial when A is a singleton set, and from mathematical induction one can also prove it without dificulty when A is finite. However, when A is infinite, one cannot deduce this axiom from the other axioms of set theory, but must explicitly add it to the list of axioms. We isolate the countable case as a particularly useful corollary (though one which is strictly weaker than the full axiom of choice): 

Corollary 0.0.5 (Axiom of countable choice). Let $E _ { 1 } , E _ { 2 } , E _ { 3 } , . . .$ be a sequence of non-empty sets. Then one can find a sequence $x _ { 1 } , x _ { 2 } , \dotsc$ such that $x _ { n } \in E _ { n }$ for all n = 1, 2, 3, . . .. 

Remark 0.0.6. The question of how much of real analysis still survives when one is not permitted to use the axiom of choice is a delicate one, involving a fair amount of logic and descriptive set theory to answer. We will not discuss these matters in this text. We will however note a theorem of G¨odel[Go1938] that states that any statement that can be phrased in the first-order language of Peano arithmetic, and which is proven with the axiom of choice, can also be proven without the axiom of choice. So, roughly speaking, G¨odel’s theorem tells us that for any “finitary” application of real analysis (which includes most of the “practical” applications of the subject), it is safe to use the axiom of choice; it is only when asking questions about “infinitary” objects that are beyond the scope of Peano arithmetic that one can encounter statements that are provable using the axiom of choice, but are not provable without it. 

## Acknowledgments

This text was strongly influenced by the real analysis text of Stein and Shakarchi[StSk2005], which was used as a secondary text when teaching the course on which these notes were based. In particular, the strategy of focusing first on Lebesgue measure and Lebesgue integration, before moving onwards to abstract measure and integration theory, was directly inspired by the treatment in [StSk2005], and the material on diferentiation theorems also closely follows that in [StSk2005]. On the other hand, our discussion here difers from that in [StSk2005] in other respects; for instance, a far greater emphasis is placed on Jordan measure and the Riemann integral as being an elementary precursor to Lebesgue measure and the Lebesgue integral. 

I am greatly indebted to my students of the course on which this text was based, as well as many further commenters on my blog, including Marco Angulo, J. Balachandran, Farzin Barekat, Marek 

Bern´at, Lewis Bowen, Chris Breeden, Danny Calegari, Yu Cao, Chandrasekhar, David Chang, Nick Cook, Damek Davis, Eric Davis, Marton Eekes, Wenying Gan, Nick Gill, Ulrich Groh, Tim Gowers, Laurens Gunnarsen, Tobias Hagge, Xueping Huang, Bo Jacoby, Apoorva Khare, Shiping Liu, Colin McQuillan, David Milovich, Hossein Naderi, Brent Nelson, Constantin Niculescu, Mircea Petrache, Walt Pohl, Jim Ralston, David Roberts, Mark Schwarzmann, Vladimir Slepnev, David Speyer, Tim Sullivan, Jonathan Weinstein, Duke Zhang, Lei Zhang, Pavel Zorin, and several anonymous commenters, for providing corrections and useful commentary on the material here. These comments can be viewed online at 

terrytao.wordpress.com/category/teaching/245a-real-analysis 

The author is supported by a grant from the MacArthur Foundation, by NSF grant DMS-0649473, and by the NSF Waterman award. 

Chapter 1 

Measure theory 

## 1.1. Prologue: The problem of measure

One of the most fundamental concepts in Euclidean geometry is that of the measure $m ( E )$ of a solid body E in one or more dimensions. In one, two, and three dimensions, we refer to this measure as the length, area, or volume of E respectively. In the classical approach to geometry, the measure of a body was often computed by partitioning that body into finitely many components, moving around each component by a rigid motion (e.g. a translation or rotation), and then reassembling those components to form a simpler body which presumably has the same area. One could also obtain lower and upper bounds on the measure of a body by computing the measure of some inscribed or circumscribed body; this ancient idea goes all the way back to the work of Archimedes at least. Such arguments can be justified by an appeal to geometric intuition, or simply by postulating the existence of a measure $m ( E )$ that can be assigned to all solid bodies E, and which obeys a collection of geometrically reasonable axioms. One can also justify the concept of measure on “physical” or “reductionistic” grounds, viewing the measure of a macroscopic body as the sum of the measures of its microscopic components. 

With the advent of analytic geometry, however, Euclidean geometry became reinterpreted as the study of Cartesian products $\mathbf { R } ^ { d }$ of the real line R. Using this analytic foundation rather than the classical geometrical one, it was no longer intuitively obvious how to define the measure $m ( E )$ of a general<sup>1</sup> subset E of $\mathbf { R } ^ { d }$ ; we will refer to this (somewhat vaguely defined) problem of writing down the “correct” definition of measure as the problem of measure. 

To see why this problem exists at all, let us try to formalise some of the intuition for measure discussed earlier. The physical intuition of defining the measure of a body E to be the sum of the measure of its component “atoms” runs into an immediate problem: a typical solid body would consist of an infinite (and uncountable) number of points, each of which has a measure of zero; and the product ∞ · 0 is indeterminate. To make matters worse, two bodies that have exactly the same number of points, need not have the same measure. For instance, in one dimension, the intervals $A : = [ 0 , 1 ]$ and $B : = [ 0 , 2 ]$ are in one-to-one correspondence (using the bijection $x \mapsto 2 x$ from A to B), but of course B is twice as long as A. So one can disassemble A into an uncountable number of points and reassemble them to form a set of twice the length. 

Of course, one can point to the infinite (and uncountable) number of components in this disassembly as being the cause of this breakdown of intuition, and restrict attention to just finite partitions. But one still runs into trouble here for a number of reasons, the most striking of which is the Banach-Tarski paradox, which shows that the unit ball $B : = \{ ( x , y , z ) \in \mathbf { R } ^ { 3 } : x ^ { 2 } + y ^ { 2 } + z ^ { 2 } \leq 1 \}$ in three dimensions<sup>2</sup> can be disassembled into a finite number of pieces (in fact, just five pieces sufice), which can then be reassembled (after translating and rotating each of the pieces) to form two disjoint copies of the ball B. 

Here, the problem is that the pieces used in this decomposition are highly pathological in nature; among other things, their construction requires use of the axiom of choice. (This is in fact necessary; there are models of set theory without the axiom of choice in which the Banach-Tarski paradox does not occur, thanks to a famous theorem of Solovay[So1970].) Such pathological sets almost never come up in practical applications of mathematics. Because of this, the standard solution to the problem of measure has been to abandon the goal of measuring every subset E of $\mathbf { R } ^ { d }$ , and instead to settle for only measuring a certain subclass of “non-pathological” subsets of $\mathbf { R } ^ { d }$ which are then referred to as the measurable sets. The problem of measure then divides into several subproblems: 

(i) What does it mean for a subset E of $\mathbf { R } ^ { d }$ to be measurable? 

(ii) If a set E is measurable, how does one define its measure? 

(iii) What nice properties or axioms does measure (or the concept of measurability) obey? 

(iv) Are “ordinary” sets such as cubes, balls, polyhedra, etc. measurable? 

(v) Does the measure of an “ordinary” set equal the “naive geometric measure” of such sets? (e.g. is the measure of an a × b rectangle equal to ab?) 

These questions are somewhat open-ended in formulation, and there is no unique answer to them; in particular, one can expand the class of measurable sets at the expense of losing one or more nice properties of measure in the process (e.g. finite or countable additivity, translation invariance, or rotation invariance). However, there are two basic answers which, between them, sufice for most applications. The first is the concept of Jordan measure (or Jordan content) of a Jordan measurable set, which is a concept closely related to that of the Riemann integral (or Darboux integral). This concept is elementary enough to be systematically studied in an undergraduate analysis course, and sufices for measuring most of the “ordinary” sets (e.g. the area under the graph of a continuous function) in many branches of mathematics. However, when one turns to the type o sets that arise in analysis, and in particular those sets that arise as limits (in various senses) of other sets, it turns out that the Jordan concept of measurability is not quite adequate, and must be extended to the more general notion of Lebesgue measurability, with the corresponding notion of Lebesgue measure that extends Jordan measure. With the Lebesgue theory (which can be viewed as a completion of the Jordan-Darboux-Riemann theory), one keeps almost all of the desirable properties of Jordan measure, but with the crucial additional property that many features of the Lebesgue theory are preserved under limits (as exemplified in the fundamental convergence theorems of the Lebesgue theory, such as the monotone convergence theorem (Theorem 1.4.44) and the dominated convergence theorem (Theorem 1.4.49), which do not hold in the Jordan-Darboux-Riemann setting). 

As such, they are particularly well suited<sup>3</sup> for applications in analysis, where limits of functions or sets arise all the time. 

In later sections, we will formally define Lebesgue measure and the Lebesgue integral, as well as the more general concept of an abstract measure space and the associated integration operation. In the rest of the current section, we will discuss the more elementary concepts of Jordan measure and the Riemann integral. This material will eventually be superceded by the more powerful theory to be treated in later sections; but it will serve as motivation for that later material, as well as providing some continuity with the treatment of measure and integration in undergraduate analysis courses. 

1.1.1. Elementary measure. Before we discuss Jordan measure, we discuss the even simpler notion of elementary measure, which allows one to measure a very simple class of sets, namely the elementary sets (finite unions of boxes). 

Definition 1.1.1 (Intervals, boxes, elementary sets). An interval is a subset of R of the form $[ a , b ] : = \{ x \in \mathbf { R } : a \leq x \leq b \} , [ a , b ) : = \{ x \in$ $\mathbf { R } : a \leq x < b \} , ( a , b ] : = \{ x \in \mathbf { R } : a < x \leq b \} , { \mathrm { o r } } ( a , b ) : = \{ x \in \mathbf { R } : a < x \leq b \} .$ $a < x < b \}$ , where $a \leq b$ are real numbers. We define the $\mathit { l e n g t h } ^ { 4 } \left| I \right|$ of an interval $I = [ a , b ] , [ a , b ) , ( a , b ] , ( a , b )$ to be $| I | : = b - a$ . A box in $\mathbf { R } ^ { d }$ is a Cartesian product $B : = I _ { 1 } \times . . . \times I _ { d }$ of d intervals $I _ { 1 } , \ldots , I _ { d }$ (not necessarily of the same length), thus for instance an interval is a one-dimensional box. The volume |B| of such a box B is defined as $| B | : = | I _ { 1 } | \times \ldots \times | I _ { d } |$ . An elementary set is any subset of $\mathbf { R } ^ { d }$ which is the union of a finite number of boxes. 

Exercise 1.1.1 (Boolean closure). Show that if $E , F \subset \mathbf { R } ^ { d }$ are elementary sets, then the union $E \cup F$ , the intersection $E \cap F$ , and the set theoretic diference $E \backslash F : = \{ x \in E : x \not \in F \}$ , and the symmetric diference $E \Delta F : = ( E \backslash F ) \cup ( F \backslash E )$ are also elementary. If $x \in \mathbf { R } ^ { d }$ , show that the translate $E + x : = \{ y + x : y \in E \}$ is also an elementary set. 

We now give each elementary set a measure. 

Lemma 1.1.2 (Measure of an elementary set). Let $E \subset \mathbf { R } ^ { d }$ be an elementary set. 

(i) E can be expressed as the finite union of disjoint boxes. 

(ii) If E is partitioned as the finite union $B _ { 1 } \cup . . . \cup B _ { k }$ of disjoint boxes, then the quantity $m ( E ) : = | B _ { 1 } | + . . . + | B _ { k } |$ is independent of the partition. In other words, given any other partition $B _ { 1 } ^ { \prime } \cup \ldots \cup B _ { k ^ { \prime } } ^ { \prime }$ of E, one has $| B _ { 1 } | + \ldots + | B _ { k } | =$ $| B _ { 1 } ^ { \prime } | + \ldots + | B _ { k ^ { \prime } } ^ { \prime } |$ 

We refer to $m ( E )$ as the elementary measure of E. (We occasionally write $m ( E )$ as $m ^ { d } ( E )$ to emphasise the d-dimensional nature of the measure.) Thus, for example, the elementary measure of $( 1 , 2 ) \cup [ 3 , 6 ]$ is 4. 

Proof. We first prove (i) in the one-dimensional case $d = 1$ . Given any finite collection of intervals $I _ { 1 } , \ldots , I _ { k }$ , one can place the 2k endpoints of these intervals in increasing order (discarding repetitions). Looking at the open intervals between these endpoints, together with the endpoints themselves (viewed as intervals of length zero), we see that there exists a finite collection of disjoint intervals $J _ { 1 } , \ldots , J _ { k ^ { \prime } }$ such that each of the $I _ { 1 } , \ldots , I _ { k }$ are a union of some subcollection of the $J _ { 1 } , \ldots , J _ { k ^ { \prime } }$ This already gives (i) when $d = 1$ . To prove the higher dimensional case, we express E as the union $B _ { 1 } , \ldots , B _ { k }$ of boxes $B _ { i } = I _ { i , 1 } \times . . . \times I _ { i , d }$ . For each $j = 1 , \dots , d _ { \colon }$ , we use the onedimensional argument to express $I _ { 1 , j } , \ldots , I _ { k , j }$ as the union of subcollections of a collection $J _ { 1 , j } , \ldots , J _ { k _ { i } ^ { \prime } , j }$ of disjoint intervals. Taking Cartesian products, we can express the $B _ { 1 } , \ldots , B _ { k }$ as finite unions of boxes $J _ { i _ { 1 } , 1 } \times \ldots \times J _ { i _ { d } , d }$ , where $1 \leq i _ { j } \leq k _ { j } ^ { \prime }$ for all $1 \leq j \leq d .$ . Such boxes are all disjoint, and the claim follows. 

To prove (ii) we use a discretisation argument. Observe (exercise!) that for any interval I, the length of I can be recovered by the limiting formula 

$$
| I | = \lim _ {N \to \infty} \frac {1}{N} \# (I \cap \frac {1}{N} {\bf Z})
$$

where $\textstyle { \frac { 1 } { N } } \mathbf { Z } : = \left\{ { \frac { n } { N } } : n \in \mathbf { Z } \right\}$ and $\# A$ denotes the cardinality of a finite set A. Taking Cartesian products, we see that 

$$
| B | = \lim _ {N \to \infty} \frac {1}{N ^ {d}} \# (B \cap \frac {1}{N} {\bf Z} ^ {d})
$$

for any box B, and in particular tha 

$$
\left| B _ {1} \right| + \dots + \left| B _ {k} \right| = \lim _ {N \rightarrow \infty} \frac {1}{N ^ {d}} \# (E \cap \frac {1}{N} \mathbf {Z} ^ {d}).
$$

Denoting the right-hand side as $m ( E )$ , we obtain the claim (ii).  

Exercise 1.1.2. Give an alternate proof of Lemma 1.1.2(ii) by showing that any two partitions of E into boxes admit a mutual refinement into boxes that arise from taking Cartesian products of elements from finite collections of disjoint intervals. 

Remark 1.1.3. One might be tempted to now define the measure $m ( E )$ of an arbitrary set $E \subset \mathbf { R } ^ { d }$ by the formula 

$$
m (E) := \lim _ {N \to \infty} \frac {1}{N ^ {d}} \# (E \cap \frac {1}{N} \mathbf {Z} ^ {d}),\tag{1.1}
$$

since this worked well for elementary sets. However, this definition is not particularly satisfactory for a number of reasons. Firstly, one can concoct examples in which the limit does not exist (Exercise!). Even when the limit does exist, this concept does not obey reasonable properties such as translation invariance. For instance, if $d = 1$ and $E : = \mathbf { Q } \cap [ 0 , 1 ] : = \left\{ x \in \mathbf { Q } : 0 \leq x \leq 1 \right\}$ , then this definition would give E a measure of 1, but would give the translate $E + { \sqrt { 2 } } : = \{ x + { \sqrt { 2 } }$ $x \in \mathbf { Q } ; 0 \leq x \leq 1 \}$ a measure of zero. Nevertheless, the formula (1.1) will be valid for all Jordan measurable sets (see Exercise 1.1.13). It also makes precise an important intuition, namely that the continuous concept of measure can be viewed<sup>5</sup> as a limit of the discrete concept of (normalised) cardinality. 

From the definitions, it is clear that $m ( E )$ is a non-negative rea number for every elementary set $E _ { : }$ , and that 

$$
m (E \cup F) = m (E) + m (F)
$$

whenever E and F are disjoint elementary sets. We refer to the latter property as finite additivity; by induction it also implies that 

$$
m (E _ {1} \cup \dots \cup E _ {k}) = m (E _ {1}) + \dots + m (E _ {k})
$$

whenever $E _ { 1 } , \ldots , E _ { k }$ are disjoint elementary sets. We also have the obvious degenerate case 

$$
m (\emptyset) = 0.
$$

Finally, elementary measure clearly extends the notion of volume, in the sense that 

$$
m (B) = | B |
$$

for all boxes B. 

From non-negativity and finite additivity (and Exercise 1.1.1) we conclude the monotonicity property 

$$
m (E) \leq m (F)
$$

whenever $E \subset F$ are nested elementary sets. From this and finite additivity (and Exercise 1.1.1) we easily obtain the finite subadditivity property 

$$
m (E \cup F) \leq m (E) + m (F)
$$

whenever $E , F$ are elementary sets (not necessarily disjoint); by induction one then has 

$$
m (E _ {1} \cup \dots \cup E _ {k}) \leq m (E _ {1}) + \dots + m (E _ {k})
$$

whenever $E _ { 1 } , \ldots , E _ { k }$ are elementary sets (not necessarily disjoint). 

It is also clear from the definition that we have the translation invariance 

$$
m (E + x) = m (E)
$$

for all elementary sets E and $x \in \mathbf { R } ^ { d }$ 

These properties in fact define elementary measure up to normalisation: 

Exercise 1.1.3 (Uniqueness of elementary measure). Let $d \geq 1$ . Let $m ^ { \prime } : \mathcal { E } ( \mathbf { R } ^ { d } )  \mathbf { R } ^ { + }$ be a map from the collection $\mathcal { E } ( \mathbf { R } ^ { d } )$ of elementary subsets of $\mathbf { R } ^ { d }$ to the nonnegative reals that obeys the non-negativity, finite additivity, and translation invariance properties. Show that there exists a constant $c \in \mathbf { R } ^ { + }$ such that $m ^ { \prime } ( E ) = c m ( E )$ for all elementary sets E. In particular, if we impose the additional normalisation $m ^ { \prime } ( [ 0 , 1 ) ^ { d } ) = 1$ , then $m ^ { \prime } \equiv m$ . (Hint: Set $c : = m ^ { \prime } ( [ 0 , 1 ) ^ { d } )$ , and then compute $m ^ { \prime } ( [ 0 , \frac { 1 } { n } ) ^ { d } )$ for any positive integer n.) 

Exercise 1.1.4. Let $d _ { 1 } , d _ { 2 } \geq 1$ , and let $E _ { 1 } \subset \mathbf { R } ^ { d _ { 1 } } , \ E _ { 2 } \subset \mathbf { R } ^ { d _ { 2 } }$ be elementary sets. Show that $E _ { 1 } \times E _ { 2 } \subset \mathbf { R } ^ { d _ { 1 } + d _ { 2 } }$ is elementary, and $m ^ { d _ { 1 } + d _ { 2 } } ( E _ { 1 } \times E _ { 2 } ) = m ^ { d _ { 1 } } ( E _ { 1 } ) \times m ^ { d _ { 2 } } ( E _ { 2 } )$ 

1.1.2. Jordan measure. We now have a satisfactory notion of measure for elementary sets. But of course, the elementary sets are a very restrictive class of sets, far too small for most applications. For instance, a solid triangle or disk in the plane will not be elementary, or even a rotated box. On the other hand, as essentially observed long ago by Archimedes, such sets E can be approximated from within and without by elementary sets $A \subset E \subset B$ , and the inscribing elementary set A and the circumscribing elementary set B can be used to give lower and upper bounds on the putative measure of E. As one makes the approximating sets A, B increasingly fine, one can hope that these two bounds eventually match. This gives rise to the following definitions. 

Definition 1.1.4 (Jordan measure). Let $E \subset \mathbf { R } ^ { d }$ be a bounded set. 

• The Jordan inner measure $m _ { * , ( J ) } ( E )$ of E is defined as 

$$
m _ {*, (J)} (E) := \sup _ {A \subset E, A \text { elementary }} m (A).
$$

• The Jordan outer measure $m ^ { * , ( J ) } ( E )$ of E is defined as 

$$
m ^ {*, (J)} (E) := \inf _ {B \supset E, B \text { elementary }} m (B).
$$

• If $m _ { * , ( J ) } ( E ) = m ^ { * , ( J ) } ( E )$ , then we say that E is Jordan measurable, and call $m ( E ) : = m _ { * , ( J ) } ( E ) = m ^ { * , ( J ) } ( E )$ the Jordan measure of E. As before, we write $m ( E )$ as $m ^ { d } ( E )$ when we wish to emphasise the dimension d. 

By convention, we do not consider unbounded sets to be Jordan measurable (they will be deemed to have infinite Jordan outer measure). 

Jordan measurable sets are those sets which are “almost elementary” with respect to Jordan outer measure. More precisely, we have 

Exercise 1.1.5 (Characterisation of Jordan measurability). Let $E \subset$ $\mathbf { R } ^ { d }$ be bounded. Show that the following are equivalent: 

(1) E is Jordan measurable. 

(2) For every $\varepsilon > 0$ , there exist elementary sets $A \subset E \subset B$ such that $m ( B \backslash A ) \leq \varepsilon$ 

(3) For every $\varepsilon > 0$ , there exists an elementary set A such that $m ^ { * , ( J ) } ( A \Delta E ) \leq \varepsilon$ 

As one corollary of this exercise, we see that every elementary set E is Jordan measurable, and that Jordan measure and elementary measure coincide for such sets; this justifies the use of $m ( E )$ to denote both. In particular, we still have $m ( \emptyset ) = 0$ 

Jordan measurability also inherits many of the properties of elementary measure: 

Exercise 1.1.6. Let $E , F \subset \mathbf { R } ^ { d }$ be Jordan measurable sets. 

(1) (Boolean closure) Show that $E \cup F , E \cap F , E \backslash F$ , and $E \Delta F$ are Jordan measurable. 

(2) (Non-negativity) m(E) ≥ 0. 

(3) (Finite additivity) If $E , F$ are disjoint, then $m ( E \cup F ) =$ m ${ \mathrm { \Omega } } _ { \mathrm { { ' } } } ( E ) + m ( F )$ 

(4) (Monotonicity) If $E \subset F$ , then $m ( E ) \leq m ( F )$ 

(5) (Finite subadditivity) $m ( E \cup F ) \leq m ( E ) + m ( F )$ 

(6) (Translation invariance) For any $x \in \mathbf { R } ^ { d } , E + x$ is Jordan measurable, and $m ( E + x ) = m ( E )$ 

Now we give some examples of Jordan measurable sets: 

Exercise 1.1.7 (Regions under graphs are Jordan measurable). Let B be a closed box in $\mathbf { R } ^ { d }$ , and let $f : B  \mathbf { R }$ be a continuous function. 

(1) Show that the graph $\{ ( x , f ( x ) ) : x \in B \} \subset \mathbf { R } ^ { d + 1 }$ is Jordan measurable in $\mathbf { R } ^ { d + 1 }$ with Jordan measure zero. (Hint: on a compact metric space, continuous functions are uniformly continuous.) 

(2) Show that the set $\{ ( x , t ) : x \in B ; 0 \leq t \leq f ( x ) \} \subset \mathbf { R } ^ { d + 1 }$ is Jordan measurable. 

Exercise 1.1.8. Let A, B, C be three points in $\mathbf { R } ^ { 2 }$ 

(1) Show that the solid triangle with vertices $A , B , C$ is Jordan measurable. 

(2) Show that the Jordan measure of the solid triangle is equal to ${ \scriptstyle { \frac { 1 } { 2 } } } | ( B - A ) \wedge ( C - A ) |$ , where $\vert ( a , b ) \wedge ( c , d ) \vert : = | a d - b c |$ 

(Hint: It may help to first do the case when one of the edges, say $A B$ , is horizontal.) 

Exercise 1.1.9. Show that every compact convex polytope<sup>6</sup> in $\mathbf { R } ^ { d }$ is Jordan measurable. 

Exercise 1.1.10. (1) Show that all open and closed Euclidean balls $B ( x , r ) : = \{ y \in { \bf R } ^ { d } : | y - x | < r \} , \ : B ( x , r ) : = \{ y \in$ $\mathbf { R } ^ { d } : | y - x | \leq r \}$ in $\mathbf { R } ^ { d }$ are Jordan measurable, with Jordan measure $c _ { d } r ^ { d }$ for some constant $c _ { d } > 0$ depending only on d. 

(2) Establish the crude bounds 

$$
\left(\frac {2}{\sqrt {d}}\right) ^ {d} \leq c _ {d} \leq 2 ^ {d}.
$$

(An exact formula for $c _ { d }$ is $c _ { d } = \textstyle { \frac { 1 } { d } } \omega _ { d }$ , where $\begin{array} { r } { \omega _ { d } : = \frac { 2 \pi ^ { d / 2 } } { \Gamma ( d / 2 ) } } \end{array}$ is the volume of the unit sphere $S ^ { d - 1 } \subset \mathbf { R } ^ { d }$ and Γ is the Gamma function, but we will not derive this formula here.) 

Exercise 1.1.11. This exercise assumes familiarity with linear algebra. Let $L : \mathbf { R } ^ { d } \to \mathbf { R } ^ { d }$ be a linear transformation. 

(1) Show that there exists a non-negative real number D such that $m ( L ( E ) ) = D m ( E )$ for every elementary set E (note from previous exercises that $L ( E )$ is Jordan measurable). (Hint: apply Exercise 1.1.3 to the map $E \mapsto m ( L ( E ) ) . )$ 

(2) Show that if E is Jordan measurable, then $L ( E )$ is also, and m $( L ( E ) ) = D m ( E )$ 

(3) Show that $D = | \operatorname* { d e t } L |$ . (Hint: Work first with the case when L is an elementary transformation, using Gaussian elimination. Alternatively, work with the cases when L is a diagonal transformation or an orthogonal transformation, using the unit ball in the latter case, and use the polar decomposition.) 

Exercise 1.1.12. Define a Jordan null set to be a Jordan measurable set of Jordan measure zero. Show that any subset of a Jordan null set is a Jordan null set. 

Exercise 1.1.13. Show that (1.1) holds for all Jordan measurable $E \subset \mathbf { R } ^ { d }$ 

Exercise 1.1.14 (Metric entropy formulation of Jordan measurability). Define a dyadic cube to be a half-open box of the form 

$$
\left[ \frac {i _ {1}}{2 ^ {n}}, \frac {i _ {1} + 1}{2 ^ {n}}\right) \times \ldots \times \left[ \frac {i _ {d}}{2 ^ {n}}, \frac {i _ {d} + 1}{2 ^ {n}}\right)
$$

for some integers $n , i _ { 1 } , \ldots , i _ { d }$ . Let $E \subset \mathbf { R } ^ { d }$ be a bounded set. For each integer n, let $\mathcal { E } _ { * } ( E , 2 ^ { - n } )$ denote the number of dyadic cubes of sidelength $2 ^ { - n }$ that are contained in $E _ { : }$ , and let ${ \mathcal { E } } ^ { * } ( E , 2 ^ { - n } )$ be the number of dyadic $\mathrm { c u b e s } ^ { 7 }$ of sidelength $2 ^ { - n }$ that intersect $E$ . Show that E is Jordan measurable if and only if 

$$
\lim _ {n \to \infty} 2 ^ {- d n} (\mathcal {E} ^ {*} (E, 2 ^ {- n}) - \mathcal {E} _ {*} (E, 2 ^ {- n})) = 0,
$$

in which case one has 

$$
m (E) = \lim _ {n \to \infty} 2 ^ {- d n} \mathcal {E} _ {*} (E, 2 ^ {- n}) = \lim _ {n \to \infty} 2 ^ {- d n} \mathcal {E} ^ {*} (E, 2 ^ {- n}).
$$

Exercise 1.1.15 (Uniqueness of Jordan measure). Let $d \geq 1$ . Let $m ^ { \prime } : \mathcal { I } ( \mathbf { R } ^ { d } )  \mathbf { R } ^ { + }$ be a map from the collection $\mathcal { I } ( \mathbf { R } ^ { d } )$ of Jordanmeasurable subsets of $\mathbf { R } ^ { d }$ to the nonnegative reals that obeys the non-negativity, finite additivity, and translation invariance properties. Show that there exists a constant $c \in \mathbf { R } ^ { + }$ such that $m ^ { \prime } ( E ) = c m ( E )$ for all Jordan measurable sets E. In particular, if we impose the additional normalisation $m ^ { \prime } ( [ 0 , 1 ) ^ { d } ) = 1$ , then $m ^ { \prime } \equiv m$ 

Exercise 1.1.16. Let $d _ { 1 } , d _ { 2 } \geq 1$ , and let $E _ { 1 } \subset { \bf R } ^ { d _ { 1 } } , E _ { 2 } \subset { \bf R } ^ { d _ { 2 } }$ be Jordan measurable sets. Show that $E _ { 1 } \times E _ { 2 } \subset \mathbf { R } ^ { d _ { 1 } + d _ { 2 } }$ is Jordan measurable, and $m ^ { d _ { 1 } + d _ { 2 } } ( E _ { 1 } \times E _ { 2 } ) = m ^ { d _ { 1 } } ( E _ { 1 } ) \times m ^ { d _ { 2 } } ( E _ { 2 } )$ 

Exercise 1.1.17. Let $P , Q$ be two polytopes in $\mathbf { R } ^ { d }$ . Suppose that $P$ can be partitioned into finitely many sub-polytopes which, after being rotated and translated, form a cover of $Q$ , with any two of the sub-polytopes in $Q$ intersecting only at their boundaries. Conclude that $P$ and $Q$ have the same Jordan measure. The converse statement is true in one and two dimensions d = 1, 2 (this is the Bolyai-Gerwien theorem), but false in higher dimensions (this was Dehn’s negative answer[De1901] to Hilbert’s third problem). 

The above exercises give a fairly large class of Jordan measurable sets. However, not every subset of $\mathbf { R } ^ { d }$ is Jordan measurable. First of all, the unbounded sets are not Jordan measurable, by construction. But there are also bounded sets that are not Jordan measurable: 

Exercise 1.1.18. Let $E \subset \mathbf { R } ^ { d }$ be a bounded set. 

(1) Show that E and the closure $\overline { E }$ of E have the same Jordan outer measure. 

(2) Show that E and the interior $E ^ { \circ }$ of E have the same Jordan inner measure. 

(3) Show that E is Jordan measurable if and only if the topological boundary $\partial E$ of E has Jordan outer measure zero. 

(4) Show that the bullet-riddled square $[ 0 , 1 ] ^ { 2 } \backslash \mathbf { Q } ^ { 2 }$ , and set of bullets $[ 0 , 1 ] ^ { 2 } \cap Q ^ { 2 }$ , both have Jordan inner measure zero and Jordan outer measure one. In particular, both sets are not Jordan measurable. 

Informally, any set with a lot of “holes”, or a very “fractal” boundary, is unlikely to be Jordan measurable. In order to measure such sets we will need to develop Lebesgue measure, which is done in the next set of notes. 

Exercise 1.1.19 (Carath´eodory type property). Let $E \subset \mathbf { R } ^ { d }$ be a bounded set, and $F ~ \subset ~ \mathbf { R } ^ { d }$ be an elementary set. Show that $m ^ { * , ( J ) } ( E ) = m ^ { * , ( J ) } ( E \cap F ) + m ^ { * , ( J ) } ( E \backslash F )$ 

1.1.3. Connection with the Riemann integral. To conclude this section, we briefly discuss the relationship between Jordan measure and the Riemann integral (or the equivalent Darboux integral). For simplicity we will only discuss the classical one-dimensional Riemann integral on an interval [a, b], though one can extend the Riemann theory without much dificulty to higher-dimensional integrals on Jordan measurable sets. (In later sections, this Riemann integral will be superceded by the Lebesgue integral.) 

Definition 1.1.5 (Riemann integrability). Let $[ a , b ]$ be an interval of positive length, and $f : [ a , b ]  \mathbf { R }$ be a function. A tagged partition $\mathcal { P } = ( ( x _ { 0 } , x _ { 1 } , \ldots , x _ { n } ) , ( x _ { 1 } ^ { * } , \ldots , x _ { n } ^ { * } ) )$ of $[ a , b ]$ is a finite sequence of real numbers $a = x _ { 0 } < x _ { 1 } < . . . < x _ { n } = b$ , together with additional numbers $x _ { i - 1 } \leq x _ { i } ^ { * } \leq x _ { i }$ for each $i = 1 , \ldots , n$ . We abbreviate ${ x } _ { i } - { x } _ { i - 1 }$ as $\delta x _ { i }$ . The quantity $\Delta ( \mathcal { P } ) : = \operatorname* { s u p } _ { 1 \leq i \leq n } \delta x _ { i }$ will be called the norm of the tagged partition. The Riemann sum $\mathcal { R } ( f , \mathcal { P } )$ of $f$ with respect to the tagged partition $\mathcal { P }$ is defined as 

$$
\mathcal {R} (f, \mathcal {P}) := \sum_ {i = 1} ^ {n} f (x _ {i} ^ {*}) \delta x _ {i}.
$$

We say that $f$ is Riemann integrable on $[ a , b ]$ if there exists a real number, denoted $\textstyle \int _ { a } ^ { b } f ( x )$ dx and referred to as the Riemann integral of $f$ on $[ a , b ]$ , for which we have 

$$
\int_ {a} ^ {b} f (x) d x = \lim _ {\Delta (\mathcal {P}) \to 0} \mathcal {R} (f, \mathcal {P})
$$

by which we mean that for every $\varepsilon > 0$ there exists $\delta > 0$ such that $\begin{array} { r } { | \mathcal { R } ( f , \mathcal { P } ) - \int _ { a } ^ { b } f ( x ) \ d x | \ \le \ \varepsilon } \end{array}$ for every tagged partition $\mathcal { P }$ with $\Delta ( \mathcal { P } ) \leq \delta$ 

If $[ a , b ]$ is an interval of zero length, we adopt the convention that every function $f : [ a , b ]  \mathbf { R }$ is Riemann integrable, with a Riemann integral of zero. 

Note that unbounded functions cannot be Riemann integrable $\mathrm { ( w h y ? ) }$ 

The above definition, while geometrically natural, can be awkward to use in practice. A more convenient formulation of the Riemann integral can be formulated using some additional machinery. 

Exercise 1.1.20 (Piecewise constant functions). Let $[ a , b ]$ be an interval. A piecewise constant function $f : [ a , b ]  \mathbf { R }$ is a function for which there exists a partition of $[ a , b ]$ into finitely many intervals $I _ { 1 } , \ldots , I _ { n }$ , such that $f$ is equal to a constant $c _ { i }$ on each of the intervals $I _ { i }$ . If $f$ is piecewise constant, show that the expression 

$$
\sum_ {i = 1} ^ {n} c _ {i} | I _ {i} |
$$

is independent of the choice of partition used to demonstrate the piecewise constant nature of $f .$ . We will denote this quantity by p.c. $\textstyle \int _ { a } ^ { b } f ( x )$ dx, and refer to it as the piecewise constant integral of $f$ on $[ a , b ]$ 

Exercise 1.1.21 (Basic properties of the piecewise constant integral). Let $[ a , b ]$ ] be an interval, and let $f , g : [ a , b ] \to \mathbf { R }$ be piecewise constant functions. Establish the following statements: 

(1) (Linearity) For any real number c, cf and $f + g$ are piecewise constant, with p.c. $\textstyle \int _ { a } ^ { b } c f ( x ) \ d x = c \mathrm { p . c . } \int _ { a } ^ { b } f ( x )$ dx and p.c. $\textstyle \int _ { a } ^ { b } f ( x ) + g ( x ) \ d x = { \mathrm { p . c . } } \int _ { a } ^ { b } f ( x ) \ d x + { \mathrm { p . c . } } \int _ { a } ^ { b } g ( x ) \ d x$ 

(2) (Monotonicity) If $f \leq g$ pointwise $( { \mathrm { i . e . } } \ f ( x ) \leq g ( x )$ for all $x \in [ a , b ] )$ then $\begin{array} { r } { \mathrm { p . c . } \int _ { a } ^ { b } f ( x ) \ d x \leq \mathrm { p . c . } \int _ { a } ^ { b } g ( x ) \ d x } \end{array}$ 

(3) (Indicator) If E is an elementary subset of $[ a , b ]$ , then the indicator function $1 _ { E } : [ a , b ]  \mathbf { R }$ (defined by setting $1 _ { E } ( x ) : =$ 1 when $x \in E$ and $1 _ { E } ( x ) : = 0$ otherwise) is piecewise constant, and p.c. $\textstyle \int _ { a } ^ { b } 1 _ { E } ( x ) \ d x = m ( E )$ 

Definition 1.1.6 (Darboux integral). Let $[ a , b ]$ be an interval, and $f : [ a , b ]  \mathbf { R }$ be a bounded function. The lower Darboux integral $\textstyle \int _ { a } ^ { b } f ( x )$ dx of f on $[ a , b ]$ is defined as 

$$
\underline {{\int_ {a} ^ {b}}} f (x) d x := \sup _ {g \leq f, \text {   piecewise   constant }} \text { p.c. } \int_ {a} ^ {b} g (x) d x,
$$

where g ranges over all piecewise constant functions that are pointwise bounded above by $f .$ . (The hypothesis that $f$ is bounded ensures that the supremum is over a non-empty set.) Similarly, we define the upper 

Darboux integral ${ \overline { { \int _ { a } ^ { b } } } } f ( x )$ dx of f on $[ a , b ]$ by the formula 

$$
\overline {{\int_ {a} ^ {b}}} f (x) d x := \inf _ {h \geq f, \text { piecewise   constant }} \text { p.c. } \int_ {a} ^ {b} h (x) d x.
$$

Clearly $\textstyle \int _ { a } ^ { b } f ( x ) \ d x \leq { \overline { { \int _ { a } ^ { b } } } } f ( x )$ dx. If these two quantities are equal, we say that f is Darboux integrable, and refer to this quantity as the Darboux integral of f on $[ a , b ]$ 

Note that the upper and lower Darboux integrals are related by the reflection identity 

$$
\overline {{\int_ {a} ^ {b}}} - f (x) d x = - \underline {{\int_ {a} ^ {b}}} f (x) d x.
$$

Exercise 1.1.22. Let $[ a , b ]$ be an interval, and $f : [ a , b ]  \mathbf { R }$ be a bounded function. Show that f is Riemann integrable if and only if it is Darboux integrable, in which case the Riemann integral and Darboux integrals are equal. 

Exercise 1.1.23. Show that any continuous function $f : [ a , b ] $ R is Riemann integrable. More generally, show that any bounded, piecewise continuous<sup>8</sup> function $f : [ a , b ]  \mathbf { R }$ is Riemann integrable. 

Now we connect the Riemann integral to Jordan measure in two ways. First, we connect the Riemann integral to one-dimensional Jordan measure: 

Exercise 1.1.24 (Basic properties of the Riemann integral). Let $[ a , b ]$ be an interval, and let $f , g : [ a , b ] \to \mathbf { R }$ be Riemann integrable. Establish the following statements: 

(1) (Linearity) For any real number $c , c f$ and $f + g$ are Riemann integrable, with $\textstyle \int _ { a } ^ { b } c f ( x ) \ d x = c \cdot \int _ { a } ^ { b } f ( x )$ dx and $\textstyle \int _ { a } ^ { b } f ( x ) +$ $\begin{array} { r } { g ( x ) \ d x = \int _ { a } ^ { b } f ( x ) \ d x + \int _ { a } ^ { b } g ( x ) \ d x . } \end{array}$ 

(2) (Monotonicity) If $f \leq g$ pointwise $( { \mathrm { i . e . } } \ f ( x ) \leq g ( x )$ for all $x \in [ a , b ] )$ then $\textstyle \int _ { a } ^ { b } f ( x ) \ d x \leq \int _ { a } ^ { b } g ( x )$ dx. 

(3) (Indicator) If E is a Jordan measurable of $[ a , b ]$ , then the indicator function $1 _ { E } : [ a , b ]  \mathbf { R }$ (defined by setting $1 _ { E } ( x ) : =$ 1 when $x \in E$ and $1 _ { E } ( x ) : = 0$ otherwise) is Riemann integrable, and $\textstyle \int _ { a } ^ { b } 1 _ { E } ( x ) \ d x = m ( E )$ 

Finally, show that these properties uniquely define the Riemann integral, in the sense that the functional $f \mapsto \textstyle \int _ { a } ^ { b } f ( x )$ dx is the only map from the space of Riemann integrable functions on $[ a , b ]$ to R which obeys all three of the above properties. 

Next, we connect the integral to two-dimensional Jordan measure: 

Exercise 1.1.25 (Area interpretation of the Riemann integral). Let $[ a , b ]$ be an interval, and let $f : [ a , b ]  \mathbf { R }$ be a bounded function. Show that f is Riemann integrable if and only if the sets $E _ { + } : =$ $\{ ( x , t ) : x \in [ a , b ] ; 0 \leq t \leq f ( x ) \}$ and $E _ { - } : = \{ ( x , t ) : x \in [ a , b ] ; f ( x ) \leq$ $t \leq 0 \}$ are both Jordan measurable in $\mathbf { R } ^ { 2 }$ , in which case one has 

$$
\int_ {a} ^ {b} f (x) d x = m ^ {2} (E _ {+}) - m ^ {2} (E _ {-}),
$$

where $m ^ { 2 }$ denotes two-dimensional Jordan measure. (Hint: First establish this in the case when f is non-negative.) 

Exercise 1.1.26. Extend the definition of the Riemann and Darboux integrals to higher dimensions, in such a way that analogues of all the previous results hold. 

## 1.2. Lebesgue measure

In Section 1.1, we recalled the classical theory of Jordan measure on Euclidean spaces $\mathbf { R } ^ { d }$ . This theory proceeded in the following stages: 

(i) First, one defined the notion of a box B and its volume |B|. 

(ii) Using this, one defined the notion of an elementary set E (a finite union of boxes), and defines the elementary measure $m ( E )$ of such sets. 

(iii) From this, one defined the inner and Jordan outer measures $m _ { * , ( J ) } ( E ) , m ^ { * , ( J ) } ( E )$ of an arbitrary bounded set $E \subset \mathbf { R } ^ { d }$ . If those measures match, we say that E is Jordan measurable, and call $m ( E ) = m _ { * , ( J ) } ( E ) = m ^ { * , ( J ) } ( E )$ the Jordan measure of $E .$ 

As long as one is lucky enough to only have to deal with Jordan measurable sets, the theory of Jordan measure works well enough. However, as noted previously, not all sets are Jordan measurable, even if one restricts attention to bounded sets. In fact, we shall see later in these notes that there even exist bounded open sets, or compact sets, which are not Jordan measurable, so the Jordan theory does not cover many classes of sets of interest. Another class that it fails to cover is countable unions or intersections of sets that are already known to be measurable: 

Exercise 1.2.1. Show that the countable union $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n }$ or countable intersection $\cap _ { n = 1 } ^ { \infty } E _ { n }$ of Jordan measurable sets $E _ { 1 } , E _ { 2 } , \ldots \subset \mathbf { R }$ need not be Jordan measurable, even when bounded. 

This creates problems with Riemann integrability (which, as we saw in Section 1.1, was closely related to Jordan measure) and pointwise limits: 

Exercise 1.2.2. Give an example of a sequence of uniformly bounded, Riemann integrable functions $f _ { n } : [ 0 , 1 ] \to \mathbf { R }$ for $n = 1 , 2 , \dots$ . that converge pointwise to a bounded function $f : [ 0 , 1 ] \to \mathbf { R }$ that is not Riemann integrable. What happens if we replace pointwise convergence with uniform convergence? 

These issues can be rectified by using a more powerful notion of measure than Jordan measure, namely Lebesgue measure. To define this measure, we first tinker with the notion of the Jordan outer measure 

$$
m ^ {*, (J)} (E) := \inf _ {B \supset E; B \text { elementary }} m (B)
$$

of a set $E \subset \mathbf { R } ^ { d }$ (we adopt the convention that $m ^ { * , ( J ) } ( E ) = + \infty$ if $E$ is unbounded, thus $m ^ { * , ( J ) }$ now takes values in the extended nonnegative reals $[ 0 , + \infty ]$ , whose properties we will briefly review below). Observe from the finite additivity and subadditivity of elementary measure that we can also write the Jordan outer measure as 

$$
m ^ {*, (J)} (E) := \inf _ {B _ {1} \cup \ldots \cup B _ {k} \supset E; B _ {1}, \ldots , B _ {k}} \text {boxes} | B _ {1} | + \ldots + | B _ {k} |,
$$

i.e. the Jordan outer measure is the infimal cost required to cover E by a finite union of boxes. (The natural number k is allowed to vary freely in the above infimum.) We now modify this by replacing the finite union of boxes by a countable union of boxes, leading to the Lebesgue outer $m e a s u r e ^ { 9 } \ m ^ { * } ( E )$ of E: 

$$
m ^ {*} (E) := \inf _ {\bigcup_ {n = 1} ^ {\infty} B _ {n} \supset E; B _ {1}, B _ {2}, \ldots} \text {boxes} \sum_ {n = 1} ^ {\infty} | B _ {n} |,
$$

thus the Lebesgue outer measure is the infimal cost required to cover E by a countable union of boxes. Note that the countable sum $\textstyle \sum _ { n = 1 } ^ { \infty } | B _ { n } |$ may be infinite, and so the Lebesgue outer measure $m ^ { * } ( E )$ could well equal $+ \infty$ 

Clearly, we always have $m ^ { * } ( E ) \leq m ^ { * , ( J ) } ( E )$ (since we can always pad out a finite union of boxes into an infinite union by adding an infinite number of empty boxes). But $m ^ { * } ( E )$ can be a lot smaller: 

Example 1.2.1. Let $E = \{ x _ { 1 } , x _ { 2 } , x _ { 3 } , \ldots \} \subset \mathbf { R } ^ { d }$ be a countable set. We know that the Jordan outer measure of E can be quite large; for instance, in one dimension, $m ^ { * , ( J ) } ( \mathbf { Q } )$ is infinite, and $m ^ { * , ( J ) } ( \mathbf { Q } \cap$ $\lbrack - R , R ] ) = m ^ { * , ( J ) } ( [ - R , R ] ) = 2 R$ since ${ \bf Q } \cap [ - R , R ]$ has $[ - R , R ]$ as its closure (see Exercise 1.1.18). On the other hand, all countable sets E have Lebesgue outer measure zero. Indeed, one simply covers E by the degenerate boxes $\{ x _ { 1 } \} , \{ x _ { 2 } \} , . . .$ . of sidelength and volume zero. 

Alternatively, if one does not like degenerate boxes, one can cover each $x _ { n }$ by a cube $B _ { n }$ of sidelength $\varepsilon / 2 ^ { n } \textrm { ( s a y ) }$ for some arbitrary $\varepsilon > 0 .$ , leading to a total cost of $\scriptstyle \sum _ { n = 1 } ^ { \infty } ( \varepsilon / 2 ^ { n } ) ^ { d }$ , which converges to $C _ { d } \varepsilon ^ { d }$ for some absolute constant $C _ { d }$ . As ε can be arbitrarily small, we see that the Lebesgue outer measure must be zero. We will refer to this type of trick as the $\varepsilon / 2 ^ { n }$ trick; it will be used many further times in this text. 

From this example we see in particular that a set may be unbounded while still having Lebesgue outer measure zero, in contrast to Jordan outer measure. 

As we shall see in Section 1.7, Lebesgue outer measure (also known as Lebesgue exterior measure) is a special case of a more general concept known as an outer measure. 

In analogy with the Jordan theory, we would also like to define a concept of “Lebesgue inner measure” to complement that of outer measure. Here, there is an asymmetry (which ultimately arises from the fact that elementary measure is subadditive rather than superadditive): one does not gain any increase in power in the Jordan inner measure by replacing finite unions of boxes with countable ones. But one can get a sort of Lebesgue inner measure by taking complements; see Exercise 1.2.18. This leads to one possible definition for Lebesgue measurability, namely the Carath´eodory criterion for Lebesgue measurability, see Exercise 1.2.17. However, this is not the most intuitive formulation of this concept to work with, and we will instead use a different (but logically equivalent) definition of Lebesgue measurability. The starting point is the observation (see Exercise 1.1.13) that Jordan measurable sets can be eficiently contained in elementary sets, with an error that has small Jordan outer measure. In a similar vein, we will define Lebesgue measurable sets to be sets that can be eficiently contained in open sets, with an error that has small Lebesgue outer measure: 

Definition 1.2.2 (Lebesgue measurability). A set $E \subset \mathbf { R } ^ { d }$ is said to be Lebesgue measurable if, for every $\varepsilon > 0$ , there exists an open set $U \subset \mathbf { R } ^ { d }$ containing E such that $m ^ { * } ( U \backslash E ) \leq \varepsilon$ . If E is Lebesgue measurable, we refer to $m ( E ) : = m ^ { * } ( E )$ as the Lebesgue measure of E (note that this quantity may be equal $\mathrm { t o } + \infty )$ . We also write $m ( E )$ as $m ^ { d } ( E )$ when we wish to emphasise the dimension d. 

Remark 1.2.3. The intuition that measurable sets are almost open is also known as Littlewood’s first principle, this principle is a triviality with our current choice of definitions, though less so if one uses other, equivalent, definitions of Lebesgue measurability. See Section 1.3.5 for a further discussion of Littlewood’s principles. 

As we shall see later, Lebesgue measure extends Jordan measure, in the sense that every Jordan measurable set is Lebesgue measurable, and the Lebesgue measure and Jordan measure of a Jordan measurable set are always equal. We will also see a few other equivalent descriptions of the concept of Lebesgue measurability. 

In the notes below we will establish the basic properties of Lebesgu measure. Broadly speaking, this concept obeys all the intuitive properties one would ask of measure, so long as one restricts attention to countable operations rather than uncountable ones, and as long as one restricts attention to Lebesgue measurable sets. The latter is not a serious restriction in practice, as almost every set one actually encounters in analysis will be measurable (the main exceptions being some pathological sets that are constructed using the axiom of choice). In the next set of notes we will use Lebesgue measure to set up the Lebesgue integral, which extends the Riemann integral in the same way that Lebesgue measure extends Jordan measure; and the many pleasant properties of Lebesgue measure will be reflected in analogous pleasant properties of the Lebesgue integral (most notably the convergence theorems). 

We will treat all dimensions $d = 1 , 2 , . . .$ . equally here, but for the purposes of drawing pictures, we recommend to the reader that one sets d equal to 2. However, for this topic at least, no additional mathematical dificulties will be encountered in the higher-dimensional case (though of course there are significant visual dificulties once d exceeds 3). 

1.2.1. Properties of Lebesgue outer measure. We begin by studying the Lebesgue outer measure $m ^ { * }$ , which was defined earlier, and takes values in the extended non-negative real axis $[ 0 , + \infty ]$ . We first record three easy properties of Lebesgue outer measure, which we will use repeatedly in the sequel without further comment: 

Exercise 1.2.3 (The outer measure axioms). 

(i) (Empty set) $m ^ { * } ( \varnothing ) = 0$ 

(ii) (Monotonicity) If $E \subset F \subset \mathbf { R } ^ { d }$ , then $m ^ { * } ( E ) \leq m ^ { * } ( F )$ 

(iii) (Countable subadditivity) If $E _ { 1 } , E _ { 2 } , \ldots \subset \mathbf { R } ^ { d }$ is a countable sequence of sets, then $\begin{array} { r } { m ^ { * } ( \bigcup _ { n = 1 } ^ { \infty } E _ { n } ) \leq \sum _ { n = 1 } ^ { \infty } m ^ { * } ( E _ { n } ) } \end{array}$ (Hint: Use the axiom of countable choice, Tonelli’s theorem for series, and the $\varepsilon / 2 ^ { n }$ trick used previously to show that countable sets had outer measure zero.) 

Note that countable subadditivity, when combined with the empty set axiom, gives as a corollary the finite subadditivity property 

$$
m ^ {*} (E _ {1} \cup \ldots \cup E _ {k}) \leq m ^ {*} (E _ {1}) + \ldots + m ^ {*} (E _ {k})
$$

for any $k \geq 0$ . These subadditivity properties will be useful in establishing upper bounds on Lebesgue outer measure. Establishing lower bounds will often be a bit trickier. (More generally, when dealing with a quantity that is defined using an infimum, it is usually easier to obtain upper bounds on that quantity than lower bounds, because the former requires one to bound just one element of the infimum, whereas the latter requires one to bound all elements.) 

Remark 1.2.4. Later on in this text, when we study abstract measure theory on a general set $X ,$ , we will define the concept of an outer measure on $X$ , which is an assigment $E \mapsto m ^ { * } ( E )$ of element of $[ 0 , + \infty ]$ to arbitrary subsets $E$ of a space $X$ that obeys the above three axioms of the empty set, monotonicity, and countable subadditivity; thus Lebesgue outer measure is a model example of an abstract outer measure. On the other hand (and somewhat confusingly), Jordan outer measure will not be an abstract outer measure (even after adopting the convention that unbounded sets have Jordan outer measure +∞): it obeys the empty set and monotonicity axioms, but is only finitely subadditive rather than countably subadditive. (For instance, the rationals $\mathbf { Q }$ have infinite Jordan outer measure, despite being the countable union of points, each of which have a Jordan outer measure of zero.) Thus we already see a major benefit of allowing countable unions of boxes in the definition of Lebesgue outer measure, in contrast to the finite unions of boxes in the definition of Jordan outer measure, in that finite subadditivity is upgraded to countable subadditivity. 

Of course, one cannot hope to upgrade countable subadditivity to uncountable subadditivity: $\mathbf { R } ^ { d }$ is an uncountable union of points, each of which has Lebesgue outer measure zero, but (as we shall shortly see), $\mathbf { R } ^ { d }$ has infinite Lebesgue outer measure. 

It is natural to ask whether Lebesgue outer measure has the finite additivity property, that is to say that $m ^ { * } ( E \cup F ) = m ^ { * } ( E ) + m ^ { * } ( F )$ whenever $E , F \subset \mathbf { R } ^ { d }$ are disjoint. The answer to this question is somewhat subtle: as we shall see later, we have finite additivity (and even countable additivity) when all sets involved are Lebesgue measurable, but that finite additivity (and hence also countable additivity) can break down in the non-measurable case. The dificulty here (which, incidentally, also appears in the theory of Jordan outer measure) is that if $E$ and $F$ are suficiently “entangled” with each other, it is not always possible to take a countable cover of $E \cup F$ by boxes and split the total volume of that cover into separate covers of $E$ and $F$ without some duplication. However, we can at least recover finite additivity if the sets $E , F$ are separated by some positive distance: 

Lemma 1.2.5 (Finite additivity for separated sets). Let E, $F \subset \mathbf { R } ^ { d }$ be such that dist $( E , F ) > 0$ , where 

$$
\operatorname{dist} (E, F) := \inf \{| x - y |: x \in E, y \in F \}
$$

is the distance<sup>10</sup> between $E$ and F. Then $m ^ { * } ( E \cup F ) = m ^ { * } ( E ) +$ $m ^ { * } ( F )$ 

Proof. From subadditivity one has $m ^ { * } ( E \cup F ) \leq m ^ { * } ( E ) + m ^ { * } ( F )$ , so it sufices to prove the other direction $m ^ { * } ( E ) + m ^ { * } ( F ) \leq m ^ { * } ( E \cup F )$ This is trivial if $E \cup F$ has infinite Lebesgue outer measure, so we may assume that it has finite Lebesgue outer measure (and then the same is true for E and $F _ { ; }$ , by monotonicity). 

We use the standard “give yourself an epsilon of room” trick (see Section 2.7 of An epsilon of room, Vol I.). Let $\varepsilon > 0$ . By definition of Lebesgue outer measure, we can cover $E \cup F$ by a countable family $B _ { 1 } , B _ { 2 } , \ldots$ . of boxes such that 

$$
\sum_ {n = 1} ^ {\infty} | B _ {n} | \leq m ^ {*} (E \cup F) + \varepsilon .
$$

Suppose it was the case that each box intersected at most one of $E$ and $F$ . Then we could divide this family into two subfamilies $B _ { 1 } ^ { \prime } , B _ { 2 } ^ { \prime } , \ldots$ and $B _ { 1 } ^ { \prime \prime } , B _ { 2 } ^ { \prime \prime } , B _ { 3 } ^ { \prime \prime } , \ldots$ , the first of which covered E, and the second of which covered $F$ . From definition of Lebesgue outer measure, we have 

$$
m ^ {*} (E) \leq \sum_ {n = 1} ^ {\infty} | B _ {n} ^ {\prime} |
$$

and 

$$
m ^ {*} (F) \leq \sum_ {n = 1} ^ {\infty} | B _ {n} ^ {\prime \prime} |;
$$

summing, we obtain 

$$
m ^ {*} (E) + m ^ {*} (F) \leq \sum_ {n = 1} ^ {\infty} | B _ {n} |
$$

and thus 

$$
m ^ {*} (E) + m ^ {*} (F) \leq m ^ {*} (E \cup F) + \varepsilon .
$$

Since $\varepsilon$ was arbitrary, this gives $m ^ { * } ( E ) + m ^ { * } ( F ) \leq m ^ { * } ( E \cup F )$ as required. 

Of course, it is quite possible for some of the boxes $B _ { n }$ to intersect both E and $F ,$ particularly if the boxes are big, in which case the above argument does not work because that box would be doublecounted. However, observe that given any $r > 0 .$ , one can always partition a large box $B _ { n }$ into a finite number of smaller boxes, each of which has diameter<sup>11</sup> at most $r _ { \mathrm { : } }$ , with the total volume of these sub-boxes equal to the volume of the original box. Applying this observation to each of the boxes $B _ { n }$ , we see that given any $r > 0$ , we may assume without loss of generality that the boxes $B _ { 1 } , B _ { 2 } , \ldots$ covering $E \cup F$ have diameter at most $r$ . In particular, we may assume that all such boxes have diameter strictly less than dist $( E , F )$ . Once we do this, then it is no longer possible for any box to intersect both $E$ and $F ,$ and then the previous argument now applies.  

In general, disjoint sets $E , F$ need not have a positive separation from each other $\left( \mathrm { e . g . } E = [ 0 , 1 \right)$ and $F = [ 1 , 2 ] )$ ). But the situation improves when E, F are closed, and at least one of $E , F$ is compact: 

Exercise 1.2.4. Let $E , F \subset \mathbf { R } ^ { d }$ be disjoint closed sets, with at least one of $E , F$ being compact. Show that dist $( E , F ) > 0$ . Give a counterexample to show that this claim fails when the compactness hypothesis is dropped. 

We already know that countable sets have Lebesgue outer measure zero. Now we start computing the outer measure of some other sets. We begin with elementary sets: 

Lemma 1.2.6 (Outer measure of elementary sets). Let E be an elementary set. Then the Lebesgue outer measure $m ^ { * } ( E )$ of E is equal to the elementary measure m(E) of E: $m ^ { * } ( E ) = m ( E )$ 

Remark 1.2.7. Since countable sets have zero outer measure, we note that we have managed to give a proof of Cantor’s theorem that $\mathbf { R } ^ { d }$ is uncountable. Of course, much quicker proofs of this theorem are available. However, this observation shows that the proof this lemma must somehow use some crucial fact about the real line which is not true for countable subfields of R, such as the rationals Q. In the proof we give here, the key fact about the real line we use is the Heine-Borel theorem, which ultimately exploits the important fact that the reals are complete. In the one-dimensional case $d = 1$ , it is also possible to exploit the fact that the reals are connected as a substitute for completeness (note that proper subfields of the reals are neither connected nor complete). 

Proof. We already know that $m ^ { * } ( E ) \leq m ^ { * , ( J ) } ( E ) = m ( E )$ , so it sufices to show that $m ( E ) \leq m ^ { * } ( E )$ 

We first establish this in the case when the elementary set E is closed. As the elementary set E is also bounded, this allows us to use the powerful Heine-Borel theorem, which asserts that every open cover of E has a finite subcover (or in other words, E is compact). 

We again use the epsilon of room strategy. Let $\varepsilon > 0$ be arbitrary, then we can find a countable family $B _ { 1 } , B _ { 2 } , \ldots$ . of boxes that cover $E$ 

$$
E \subset \bigcup_ {n = 1} ^ {\infty} B _ {n},
$$

and such that 

$$
\sum_ {n = 1} ^ {\infty} | B _ {n} | \leq m ^ {*} (E) + \varepsilon .
$$

We would like to use the Heine-Borel theorem, but the boxes $B _ { n }$ need not be open. But this is not a serious problem, as one can spend another epsilon to enlarge the boxes to be open. More precisely, for each box $B _ { n }$ one can find an open box $B _ { n } ^ { \prime }$ containing $B _ { n }$ such that $| B _ { n } ^ { \prime } | \leq | B _ { n } | + \varepsilon / 2 ^ { n }$ (say). The $B _ { n } ^ { \prime }$ still cover $E _ { : }$ , and we have 

$$
\sum_ {n = 1} ^ {\infty} | B _ {n} ^ {\prime} | \leq \sum_ {n = 1} ^ {\infty} (| B _ {n} | + \varepsilon / 2 ^ {n}) = (\sum_ {n = 1} ^ {\infty} | B _ {n} |) + \varepsilon \leq m ^ {*} (E) + 2 \varepsilon .
$$

As the $B _ { n } ^ { \prime }$ are open, we may apply the Heine-Borel theorem and conclude that 

$$
E \subset \bigcup_ {n = 1} ^ {N} B _ {n} ^ {\prime}
$$

for some finite N. Using the finite subadditivity of elementary measure, we conclude that 

$$
m (E) \leq \sum_ {n = 1} ^ {N} | B _ {n} ^ {\prime} |
$$

and thus 

$$
m (E) \leq m ^ {*} (E) + 2 \varepsilon .
$$

Since $\varepsilon > 0$ was arbitrary, the claim follows. 

Now we consider the case when the elementary E is not closed. Then we can write E as the finite union $Q _ { 1 } \cup \ldots \cup Q _ { k }$ of disjoint boxes, which need not be closed. But, similarly to before, we can use the epsilon of room strategy: for every $\varepsilon > 0$ and every $1 \leq j \leq k$ , one can find a closed sub-box $Q _ { j } ^ { \prime }$ of $Q _ { j }$ such that $| Q _ { j } ^ { \prime } | \geq | Q _ { j } | - \varepsilon / k$ (say); then $E$ contains the finite union of $Q _ { 1 } ^ { \prime } \cup . . . \cup Q _ { k } ^ { \prime }$ disjoint closed boxes, which is a closed elementary set. By the previous discussion and the finite additivity of elementary measure, we have 

$$
\begin{array}{l} m ^ {*} (Q _ {1} ^ {\prime} \cup \ldots \cup Q _ {k} ^ {\prime}) = m (Q _ {1} ^ {\prime} \cup \ldots \cup Q _ {k} ^ {\prime}) \\ \qquad = m (Q _ {1} ^ {\prime}) + \ldots + m (Q _ {k} ^ {\prime}) \\ \qquad \geq m (Q _ {1}) + \ldots + m (Q _ {k}) - \varepsilon \\ \qquad = m (E) - \varepsilon . \end{array}
$$

Applying by monotonicity of Lebesgue outer measure, we conclude that 

$$
m ^ {*} (E) \geq m (E) - \varepsilon
$$

for every $\varepsilon > 0$ . Since $\varepsilon > 0$ was arbitrary, the claim follows. 

The above lemma allows us to compute the Lebesgue outer measure of a finite union of boxes. From this and monotonicity we conclude that the Lebesgue outer measure of any set is bounded below by its Jordan inner measure. As it is also bounded above by the Jordan outer measure, we have 

$$
m _ {*, (J)} (E) \leq m ^ {*} (E) \leq m ^ {*, (J)} (E)\tag{1.2}
$$

for every $E \subset \mathbf { R } ^ { d }$ 

Remark 1.2.8. We are now able to explain why not every bounded open set or compact set is Jordan measurable. Consider the countable set $\mathbf { Q } \cap [ 0 , 1 ]$ , which we enumerate as $\{ q _ { 1 } , q _ { 2 } , q _ { 3 } , . . . \}$ , let $\varepsilon > 0$ be a small number, and consider the set 

$$
U := \bigcup_ {n = 1} ^ {\infty} (q _ {n} - \varepsilon / 2 ^ {n}, q _ {n} + \varepsilon / 2 ^ {n}).
$$

This is the union of open sets and is thus open. On the other hand, by countable subadditivity, one has 

$$
m ^ {*} (U) \leq \sum_ {n = 1} ^ {\infty} 2 \varepsilon / 2 ^ {n} = 2 \varepsilon .
$$

Finally, as $U$ is dense in [0, 1] (i.e. $\overline { U }$ contains [0, 1]), we have 

$$
m ^ {*, (J)} (U) = m ^ {*, (J)} (\overline {{U}}) \geq m ^ {*, (J)} ([ 0, 1 ]) = 1.
$$

For $\varepsilon$ small enough $( \mathrm { e . g . ~ } \ \varepsilon : = 1 / 3 )$ , we see that the Lebesgue outer measure and Jordan outer measure of U disagree. Using (1.2), we conclude that the bounded open set $U$ is not Jordan measurable. This in turn implies that the complement of $U$ in, say, [−2, 2], is also not Jordan measurable, despite being a compact set. 

Now we turn to countable unions of boxes. It is convenient to introduce the following notion: two boxes are almost disjoint if their interiors are disjoint, thus for instance [0, 1] and [1, 2] are almost disjoint. As a box has the same elementary measure as its interior, we see that the finite additivity property 

$$
m (B _ {1} \cup \dots \cup B _ {k}) = | B _ {1} | + \dots + | B _ {k} |\tag{1.3}
$$

holds for almost disjoint boxes $B _ { 1 } , \ldots , B _ { k }$ , and not just for disjoint boxes. This (and Lemma 1.2.6) has the following consequence: 

Lemma 1.2.9 (Outer measure of countable unions of almost disjoint boxes). Let $\textstyle E = \bigcup _ { n = 1 } ^ { \infty } B _ { n }$ be a countable union of almost disjoint boxes $B _ { 1 } , B _ { 2 } , \ldots$ Then 

$$
m ^ {*} (E) = \sum_ {n = 1} ^ {\infty} | B _ {n} |.
$$

Thus, for instance, $\mathbf { R } ^ { d }$ itself has an infinite outer measure. 

Proof. From countable subadditivity and Lemma 1.2.6 we have 

$$
m ^ {*} (E) \leq \sum_ {n = 1} ^ {\infty} m ^ {*} (B _ {n}) = \sum_ {n = 1} ^ {\infty} | B _ {n} |,
$$

so it sufices to show that 

$$
\sum_ {n = 1} ^ {\infty} | B _ {n} | \leq m ^ {*} (E).
$$

But for each natural number N, E contains the elementary set B ∪ $\dots \cup B _ { N }$ , so by monotonicity and Lemma 1.2.6, 

$$
\begin{array}{c} m ^ {*} (E) \geq m ^ {*} (B _ {1} \cup \ldots \cup B _ {N}) \\ = m (B _ {1} \cup \ldots \cup B _ {N}) \end{array}
$$

and thus by (1.3), one has 

$$
\sum_ {n = 1} ^ {N} | B _ {n} | \leq m ^ {*} (E).
$$

Letting $N \to \infty$ we obtain the claim. 

Remark 1.2.10. The above lemma has the following immediate corollary: if $\begin{array} { r } { E = \bigcup _ { n = 1 } ^ { \infty } B _ { n } = \bigcup _ { n = 1 } ^ { \infty } B _ { n } ^ { \prime } } \end{array}$ can be decomposed in two diferent ways as the countable union of almost disjoint boxes, then $\begin{array} { r } { \sum _ { n = 1 } ^ { \infty } \left| B _ { n } \right| = \sum _ { n = 1 } ^ { \infty } \left| B _ { n } ^ { \prime } \right| } \end{array}$ . Although this statement is intuitively obvi ous and does not explicitly use the concepts of Lebesgue outer measure or Lebesgue measure, it is remarkably dificult to prove this statement rigorously without essentially using one of these two concepts. (Try it!) 

Exercise 1.2.5. Show that if a set $E \subset \mathbf { R } ^ { d }$ is expressible as the countable union of almost disjoint boxes, then the Lebesgue outer measure of $E$ is equal to the Jordan inner measure: $m ^ { * } ( E ) = m _ { * , ( J ) } ( E )$ where we extend the definition of Jordan inner measure to unbounded sets in the obvious manner. 

Not every set can be expressed as the countable union of almost disjoint boxes (consider for instance the irrationals $\mathbf { R } \backslash \mathbf { Q }$ , which contain no boxes other than the singleton sets). However, there is an important class of sets of this form, namely the open sets: 

Lemma 1.2.11. Let $E \subset \mathbf { R } ^ { d }$ be an open set. Then E can be expressed as the countable union of almost disjoint boxes (and, in fact, as the countable union of almost disjoint closed cubes). 

Proof. We will use the dyadic mesh structure of the Euclidean space $\mathbf { R } ^ { d }$ , which is a convenient tool for “discretising” certain aspects of real analysis. 

Define a closed dyadic cube to be a cube $Q$ of the form 

$$
Q = \left[ \frac {i _ {1}}{2 ^ {n}}, \frac {i _ {1} + 1}{2 ^ {n}} \right] \times \ldots \times \left[ \frac {i _ {d}}{2 ^ {n}}, \frac {i _ {d} + 1}{2 ^ {n}} \right]
$$

for some integers $n , i _ { 1 } , \ldots , i _ { d }$ . To avoid some technical issues we shall restrict attention here to “small” cubes of sidelength at most 1, thus we restrict n to the non-negative integers, and we will completely ignore “large” cubes of sidelength greater than one. Observe that the closed dyadic cubes of a fixed sidelength $2 ^ { - n }$ are almost disjoint, and cover all of $\mathbf { R } ^ { d }$ . Also observe that each dyadic cube of sidelength $2 ^ { - n }$ is contained in exactly one “parent” cube of sidelength $2 ^ { - n + 1 }$ (which, conversely, has $2 ^ { d }$ “children” of sidelength $2 ^ { - n } )$ , giving the dyadic cubes a structure analogous to that of a binary tree (or more precisely, an infinite forest of $2 ^ { d } \mathrm { - a r y \ t r e s } )$ . As a consequence of these facts, we also obtain the important dyadic nesting property: given any two closed dyadic cubes (possibly of diferent sidelength), either they are almost disjoint, or one of them is contained in the other. 

If E is open, and $x \in E$ , then by definition there is an open ball centered at $x$ that is contained in $E _ { : }$ , and it is easy to conclude that there is also a closed dyadic cube containing x that is contained in $E$ . Thus, if we let $\mathcal { Q }$ be the collection of all the dyadic cubes $Q$ that are contained in $E _ { : }$ , we see that the union $\cup _ { Q \in \mathcal { Q } } Q$ of all these cubes is exactly equal to $E$ . 

As there are only countably many dyadic cubes, $\mathcal { Q }$ is at most countable. But we are not done yet, because these cubes are not almost disjoint (for instance, any cube $Q$ in $\mathcal { Q }$ will of course overlap with its child cubes). But we can deal with this by exploiting the dyadic nesting property. Let $\mathcal { Q } ^ { \ast }$ denote those cubes in $\mathcal { Q }$ which are maximal with respect to set inclusion, which means that they are not contained in any other cube in $\mathcal { Q } .$ From the nesting property (and the fact that we have capped the maximum size of our cubes) we see that every cube in $\mathcal { Q }$ is contained in exactly one maximal cube in $\mathcal { Q } ^ { * }$ , and that any two such maximal cubes in $\mathcal { Q } ^ { \ast }$ are almost disjoint. Thus, we see that $E$ is the union $E = \textstyle \bigcup _ { Q \in \mathcal { Q } ^ { * } } Q$ of almost disjoint cubes. ${ \mathrm { A s ~ } } { \mathcal { Q } } ^ { * }$ is at most countable, the claim follows (adding empty boxes if necessary to pad out the cardinality).  

We now have a formula for the Lebesgue outer measure of any open set: it is exactly equal to the Jordan inner measure of that set, or of the total volume of any partitioning of that set into almost disjoint boxes. Finally, we have a formula for the Lebesgue outer measure of an arbitrary set: 

Lemma 1.2.12 (Outer regularity). Let $E \subset \mathbf { R } ^ { d }$ be an arbitrary set. Then one has 

$$
m ^ {*} (E) = \inf _ {E \subset U, U o p e n} m ^ {*} (U).
$$

Proof. From monotonicity one trivially has 

$$
m ^ {*} (E) \leq \inf _ {E \subset U, U \text { open }} m ^ {*} (U)
$$

so it sufices to show that 

$$
\inf _ {E \subset U, U \text { open }} m ^ {*} (U) \leq m ^ {*} (E).
$$

This is trivial for $m ^ { * } ( E )$ infinite, so we may assume that $m ^ { * } ( E )$ is finite. 

Let $\varepsilon > 0$ . By definition of outer measure, there exists a countable family $B _ { 1 } , B _ { 2 } , \ldots$ . of boxes covering E such that 

$$
\sum_ {n = 1} ^ {\infty} | B _ {n} | \leq m ^ {*} (E) + \varepsilon .
$$

We use the $\varepsilon / 2 ^ { n }$ trick again. We can enlarge each of these boxes $B _ { n }$ to an open box $B _ { n } ^ { \prime }$ such that $| B _ { n } ^ { \prime } | \leq | B _ { n } | + \varepsilon / 2 ^ { n }$ . Then the set $\textstyle \bigcup _ { n = 1 } ^ { \infty } B _ { n } ^ { \prime }$ , being a union of open sets, is itself open, and contains $E$ ; and 

$$
\sum_ {n = 1} ^ {\infty} \left| B _ {n} ^ {\prime} \right| \leq m ^ {*} (E) + \varepsilon + \sum_ {n = 1} ^ {\infty} \varepsilon / 2 ^ {n} = m ^ {*} (E) + 2 \varepsilon .
$$

By countable subadditivity, this implies that 

$$
m ^ {*} (\bigcup_ {n = 1} ^ {\infty} B _ {n} ^ {\prime}) \leq m ^ {*} (E) + 2 \varepsilon
$$

and thus 

$$
\inf _ {E \subset U, U \text { open }} m ^ {*} (U) \leq m ^ {*} (E) + 2 \varepsilon .
$$

As $\varepsilon > 0$ was arbitrary, we obtain the claim 

Exercise 1.2.6. Give an example to show that the reverse statement 

$$
m ^ {*} (E) = \sup _ {U \subset E, U \text { open}} m ^ {*} (U)
$$

is false. (For the corrected version of this statement, see Exercise 1.2.15.) 

1.2.2. Lebesgue measurability. We now define the notion of a Lebesgue measurable set as one which can be eficiently contained in open sets in the sense of Definition 1.2.2, and set out their basic properties. 

First, we show that there are plenty of Lebesgue measurable sets. 

Lemma 1.2.13 (Existence of Lebesgue measurable sets). 

(i) Every open set is Lebesgue measurable. 

(ii) Every closed set is Lebesgue measurable. 

(iii) Every set of Lebesgue outer measure zero is measurable. (Such sets are called null sets.) 

(iv) The empty set ∅ is Lebesgue measurable. 

(v) If $E \subset \mathbf { R } ^ { d }$ is Lebesgue measurable, then so is its complement $\mathbf { R } ^ { d } \backslash E$ 

(vi) If $E _ { 1 } , E _ { 2 } , E _ { 3 } , \ldots \subset \mathbf { R } ^ { d }$ are a sequence of Lebesgue measurable sets, then the union $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n }$ is Lebesgue measurable. 

(vii) If $E _ { 1 } , E _ { 2 } , E _ { 3 } , \ldots \subset \mathbf { R } ^ { d }$ are a sequence of Lebesgue measurable sets, then the intersection $\cap _ { n = 1 } ^ { \infty } E _ { n }$ is Lebesgue measurable. 

Proof. Claim (i) is obvious from definition, as are Claims (iii) and (iv). 

To prove Claim (vi), we use the $\varepsilon / 2 ^ { n }$ trick. Let $\varepsilon > 0$ be arbitrary. By hypothesis, each $E _ { n }$ is contained in an open set $U _ { n }$ whose diference $U _ { n } \backslash E _ { n }$ has Lebesgue outer measure at most $\varepsilon / 2 ^ { n }$ . By countable subadditivity, this implies that $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n }$ is contained in $\textstyle \bigcup _ { n = 1 } ^ { \infty } U _ { n }$ , and the diference $\textstyle ( \bigcup _ { n = 1 } ^ { \infty } U _ { n } ) \backslash ( \bigcup _ { n = 1 } ^ { \infty } E _ { n } )$ has Lebesgue outer measure at most ε. The set $\textstyle \bigcup _ { n = 1 } ^ { \infty } U _ { n }$ , being a union of open sets, is itself open, and the claim follows. 

Now we establish Claim (ii). Every closed set E is the countable union of closed and bounded sets (by intersecting E with, say, the closed balls $\overline { { B ( 0 , n ) } }$ of radius n for $n = 1 , 2 , 3 , . . . )$ , so by (vi), it sufices to verify the claim when E is closed and bounded, hence compact by the Heine-Borel theorem. Note that the boundedness of E implies that $m ^ { * } ( E )$ is finite. 

Let $\varepsilon > 0$ . By outer regularity (Lemma 1.2.12), we can find an open set U containing E such that $m ^ { * } ( U ) \leq m ^ { * } ( E ) + \varepsilon$ . It sufices to show that $m ^ { * } ( U \backslash E ) \leq \varepsilon$ 

The set $U \backslash E$ is open, and so by Lemma 1.2.11 is the countable union $\textstyle { \bigcup _ { n = 1 } ^ { \infty } Q _ { n } }$ of almost disjoint closed cubes. By Lemma 1.2.9, $\begin{array} { r } { m ^ { * } ( U \backslash E ) = \sum _ { n = 1 } ^ { \infty } \left| Q _ { n } \right| } \end{array}$ . So it will sufice to show that $\begin{array} { r } { \sum _ { n = 1 } ^ { N } | Q _ { n } | \leq \varepsilon } \end{array}$ for every finite N. 

The set $\textstyle \bigcup _ { n = 1 } ^ { N } Q _ { n }$ is a finite union of closed cubes and is thus closed. It is disjoint from the compact set $E .$ , so by Exercise 1.2.4 followed by Lemma 1.2.5 one has 

$$
m ^ {*} (E \cup \bigcup_ {n = 1} ^ {N} Q _ {n}) = m ^ {*} (E) + m ^ {*} (\bigcup_ {n = 1} ^ {N} Q _ {n}).
$$

By monotonicity, the left-hand side is at most $m ^ { * } ( U )$ , which is in turn at most $m ^ { * } ( E ) + \varepsilon$ . Since $m ^ { * } ( E )$ is finite, we may cancel it and conclude that $m ^ { * } ( \bigcup _ { n = 1 } ^ { N } Q _ { n } ) \leq \varepsilon$ , as required. 

Next, we establish Claim (v). If E is Lebesgue measurable, then for every n we can find an open set $U _ { n }$ containing $E$ such that $m ^ { * } ( U _ { n } \backslash E ) \leq 1 / n$ . Letting $F _ { n }$ be the complement of $U _ { n }$ , we conclude that the complement $\mathbf { R } ^ { d } \backslash E$ of $E$ contains all of the $F _ { n }$ , and that $m ^ { * } ( ( \mathbf { R } ^ { d } \backslash E ) \backslash F _ { n } ) \leq 1 / n$ . If we let $F : = \textstyle \bigcup _ { n = 1 } ^ { \infty } F _ { n }$ , then $\mathbf { R } ^ { d } \backslash E$ contains $F _ { ; }$ , and from monotonicity $m ^ { * } ( ( { \bf R } ^ { d } \backslash E ) \backslash F ) = 0$ , thus $\mathbf { R } ^ { d } \backslash E$ is the union of $F$ and a set of Lebesgue outer measure zero. But $F$ is in turn the union of countably many closed sets $F _ { n }$ . The claim now follows from (ii), (iii), (iv). 

Finally, Claim (vii) follows from ${ \mathrm { ( v ) , ~ ( v i ) } }$ , and de Morgan’s laws $\begin{array} { r } { ( \bigcap _ { \alpha \in A } E _ { \alpha } ) ^ { c } = \bigcup _ { \alpha \in A } E _ { \alpha } ^ { c } , ( \bigcup _ { \alpha \in A } E _ { \alpha } ) ^ { c } = \bigcap _ { \alpha \in A } E _ { \alpha } ^ { c } } \end{array}$ , (which work for infinite unions and intersections without any dificulty).  

Informally, the above lemma asserts (among other things) that if one starts with such basic subsets of $\mathbf { R } ^ { d }$ as open or closed sets and then takes at most countably many boolean operations, one will always end up with a Lebesgue measurable set. This is already enough to ensure that the majority of sets that one actually encounters in real analysis will be Lebesgue measurable. (Nevertheless, using the axiom of choice one can construct sets that are not Lebesgue measurable; we will see an example of this later. As a consequence, we cannot generalise the countable closure properties here to uncountable closure properties.) 

Remark 1.2.14. The properties (iv), (v), (vi) of Lemma 1.2.13 assert that the collection of Lebesgue measurable subsets of $\mathbf { R } ^ { d }$ form a $\sigma \mathrm { - }$ algebra, which is a strengthening of the more classical concept of a boolean algebra. We will study abstract σ-algebras in more detail in Section 1.4. 

Note how this Lemma 1.2.13 is significantly stronger than the counterpart for Jordan measurability (Exercise 1.1.6), in particular by allowing countably many boolean operations instead of just finitely many. This is one of the main reasons why we use Lebesgue measure instead of Jordan measure. 

Exercise 1.2.7 (Criteria for measurability). Let $E \subset \mathbf { R } ^ { d }$ . Show that the following are equivalent: 

(i) E is Lebesgue measurable. 

(ii) (Outer approximation by open) For every $\varepsilon > 0$ , one can contain E in an open set U with $m ^ { * } ( U \backslash E ) \leq \varepsilon .$ 

(iii) (Almost open) For every $\varepsilon > 0$ , one can find an open set U such that $m ^ { * } ( U \Delta E ) \leq \varepsilon$ . (In other words, E difers from an open set by a set of outer measure at most ε.) 

(iv) (Inner approximation by closed) For every $\varepsilon > 0$ , one can find a closed set F contained in E with $m ^ { * } ( E \backslash F ) \leq \varepsilon$ 

(v) (Almost closed) For every $\varepsilon > 0$ , one can find a closed set F such that $m ^ { * } ( F \Delta E ) \leq \varepsilon$ . (In other words, E difers from a closed set by a set of outer measure at most ε.) 

(vi) (Almost measurable) For every $\varepsilon > 0$ , one can find a Lebesgue measurable set $E _ { \varepsilon }$ such that $m ^ { * } ( E _ { \varepsilon } \Delta E ) \leq \varepsilon .$ . (In other words, E difers from a measurable set by a set of outer measure at most ε.) 

(Hint: Some of these deductions are either trivial or very easy. To deduce (i) from (vi), use the $\varepsilon / 2 ^ { n }$ trick to show that E is contained in a Lebesgue measurable set $E _ { \varepsilon } ^ { \prime }$ with $m ^ { * } ( E _ { \varepsilon } ^ { \prime } \Delta E ) \ \leq \ \varepsilon .$ , and then take countable intersections to show that E difers from a Lebesgue measurable set by a null set.) 

Exercise 1.2.8. Show that every Jordan measurable set is Lebesgue measurable. 

Exercise 1.2.9 (Middle thirds Cantor set). Let $I _ { 0 } : = [ 0 \AA , 1 \AA ]$ be the unit interval, let $I _ { 1 } : = [ 0 , 1 / 3 ] \cup [ 2 / 3 , 1 ]$ be $I _ { 0 }$ with the interior of the middle third interval removed, let $I _ { 2 } : = [ 0 , 1 / 9 ] \cup [ 2 / 9 , 1 / 3 ]$ ∪ $[ 2 / 3 , 7 / 9 ] \cup [ 8 / 9 , 1 ]$ be $I _ { 1 }$ with the interior of the middle third of each of the two intervals of $I _ { 1 }$ removed, and so forth. More formally, write 

$$
I _ {n} := \bigcup_ {a _ {1}, \dots , a _ {n} \in \{0, 2 \}} [ \sum_ {i = 1} ^ {n} \frac {a _ {i}}{3 ^ {i}}, \sum_ {i = 1} ^ {n} \frac {a _ {i}}{3 ^ {i}} + \frac {1}{3 ^ {n}} ].
$$

Let $\textstyle C : = \bigcap _ { n = 1 } ^ { \infty } I _ { n }$ be the intersection of all the elementary sets $I _ { n }$ Show that $C$ is compact, uncountable, and a null set. 

Exercise 1.2.10. (This exercise presumes some familiarity with pointset topology.) Show that the half-open interval [0, 1) cannot be expressed as the countable union of disjoint closed intervals. (Hint: It is easy to prevent [0, 1) from being expressed as the finite union of disjoint closed intervals. Next, assume for sake of contradiction that [0, 1) is the union of infinitely many closed intervals, and conclude that [0, 1) is homeomorphic to the middle thirds Cantor set, which is absurd. It is also possible to proceed using the Baire category theorem (§1.7 of An epsilon of room, Vol. I.) For an additional challenge, show that [0, 1) cannot be expressed as the countable union of disjoint closed sets. 

Now we look at the Lebesgue measure $m ( E )$ of a Lebesgue measurable set $E ,$ , which is defined to equal its Lebesgue outer measure $m ^ { * } ( E )$ . If E is Jordan measurable, we see from (1.2) that the Lebesgue measure and the Jordan measure of $E$ coincide, thus Lebesgue measure extends Jordan measure. This justifies the use of the notation $m ( E )$ to denote both Lebesgue measure of a Lebesgue measurable set, and Jordan measure of a Jordan measurable set (as well as elementary measure of an elementary set). 

Lebesgue measure obeys significantly better properties than Lebesgue outer measure, when restricted to Lebesgue measurable sets: 

Lemma 1.2.15 (The measure axioms). 

(i) (Empty set) $m ( \emptyset ) = 0$ 

(ii) (Countable additivity) If $E _ { 1 } , E _ { 2 } , \ldots \subset \mathbf { R } ^ { d }$ is a countable sequence ofdisjoint Lebesgue measurable sets, then $m ( \bigcup _ { n = 1 } ^ { \infty } E _ { n } ) =$ $\scriptstyle \sum _ { n = 1 } ^ { \infty } m ( E _ { n } )$ 

Proof. The first claim is trivial, so we focus on the second. We deal with an easy case when all of the $E _ { n }$ are compact. By repeated use of Lemma 1.2.5 and Exercise 1.2.4, we have 

$$
m (\bigcup_ {n = 1} ^ {N} E _ {n}) = \sum_ {n = 1} ^ {N} m (E _ {n}).
$$

Using monotonicity, we conclude that 

$$
m (\bigcup_ {n = 1} ^ {\infty} E _ {n}) \geq \sum_ {n = 1} ^ {N} m (E _ {n}).
$$

(We can use m instead of $m ^ { * }$ throughout this argument, thanks to Lemma 1.2.13). Sending $N \to \infty$ we obtain 

$$
m (\bigcup_ {n = 1} ^ {\infty} E _ {n}) \geq \sum_ {n = 1} ^ {\infty} m (E _ {n}).
$$

On the other hand, from countable subadditivity one has 

$$
m (\bigcup_ {n = 1} ^ {\infty} E _ {n}) \leq \sum_ {n = 1} ^ {\infty} m (E _ {n}),
$$

and the claim follows. 

Next, we handle the case when the $E _ { n }$ are bounded but not necessarily compact. We use the $\varepsilon / 2 ^ { n }$ trick. Let $\varepsilon > 0$ . Applying Exercise 1.2.7, we know that each $E _ { n }$ is the union of a compact set $K _ { n }$ and a set of outer measure at most $\varepsilon / 2 ^ { n }$ . Thus 

$$
m (E _ {n}) \leq m (K _ {n}) + \varepsilon / 2 ^ {n}
$$

and hence 

$$
\sum_ {n = 1} ^ {\infty} m (E _ {n}) \leq (\sum_ {n = 1} ^ {\infty} m (K _ {n})) + \varepsilon .
$$

Finally, from the compact case of this lemma we already know that 

$$
m (\bigcup_ {n = 1} ^ {\infty} K _ {n}) = \sum_ {n = 1} ^ {\infty} m (K _ {n})
$$

while from monotonicity 

$$
m (\bigcup_ {n = 1} ^ {\infty} K _ {n}) \leq m (\bigcup_ {n = 1} ^ {\infty} E _ {n}).
$$

Putting all this together we see that 

$$
\sum_ {n = 1} ^ {\infty} m (E _ {n}) \leq m (\bigcup_ {n = 1} ^ {\infty} E _ {n}) + \varepsilon
$$

for every $\varepsilon > 0$ , while from countable subadditivity we have 

$$
m (\bigcup_ {n = 1} ^ {\infty} E _ {n}) \leq \sum_ {n = 1} ^ {\infty} m (E _ {n}).
$$

The claim follows. 

Finally, we handle the case when the $E _ { n }$ are not assumed to be bounded or closed. Here, the basic idea is to decompose each $E _ { n }$ as a countable disjoint union of bounded Lebesgue measurable sets. First, decompose $\mathbf { R } ^ { d }$ as the countable disjoint union $\textstyle \mathbf { R } ^ { d } = \bigcup _ { m = 1 } ^ { \infty } A _ { m }$ of bounded measurable sets $A _ { m }$ ; for instance one could take the annuli $A _ { m } : = \{ x \in \mathbf { R } ^ { d } : m - 1 \leq | x | < m \}$ . Then each $E _ { n }$ is the countable disjoint union of the bounded measurable sets $E _ { n } \cap A _ { m }$ for $m =$ $1 , 2 , . . . ,$ and thus 

$$
m (E _ {n}) = \sum_ {m = 1} ^ {\infty} m (E _ {n} \cap A _ {m})
$$

by the previous arguments. In a similar vein, $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n }$ is the countable disjoint union of the bounded measurable sets $E _ { n } \cap A _ { m }$ for $n , m = 1 , 2 , . . . ,$ and thus 

$$
m (\bigcup_ {n = 1} ^ {\infty} E _ {n}) = \sum_ {n = 1} ^ {\infty} \sum_ {m = 1} ^ {\infty} m (E _ {n} \cap A _ {m}),
$$

and the claim follows. 

From Lemma 1.2.15 one of course can conclude finite additivity 

$$
m (E _ {1} \cup \dots \cup E _ {k}) = m (E _ {1}) + \dots + m (E _ {k})
$$

whenever $E _ { 1 } , \ldots , E _ { k } \subset \mathbf { R } ^ { d }$ are Lebesgue measurable sets. We also have another important result: 

Exercise 1.2.11 (Monotone convergence theorem for measurable sets). 

(i) (Upward monotone convergence) Let $E _ { 1 } \subset E _ { 2 } \subset . . . \subset \mathbf { R } ^ { n }$ be a countable non-decreasing sequence of Lebesgue measurable sets. Show that $m ( \bigcup _ { n = 1 } ^ { \infty } E _ { n } ) \ = \ \operatorname* { l i m } _ { n \to \infty } m ( E _ { n } )$ (Hint: Express $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n }$ as the countable union of the lacunae $\textstyle E _ { n } \backslash \bigcup _ { n ^ { \prime } = 1 } ^ { n - 1 } E _ { n ^ { \prime } } . )$ 

(ii) (Downward monotone convergence) Let $\mathbf { R } ^ { d } \supset E _ { 1 } \supset E _ { 2 } \supset$ . . . be a countable non-increasing sequence of Lebesgue measurable sets. If at least one of the $m ( E _ { n } )$ is finite, show that $\begin{array} { r } { m ( \bigcap _ { n = 1 } ^ { \infty } E _ { n } ) = \operatorname* { l i m } _ { n \to \infty } m ( E _ { n } ) } \end{array}$ 

(iii) Give a counterexample to show that the hypothesis that at least one of the $m ( E _ { n } )$ is finite in the downward monotone convergence theorem cannot be dropped. 

Exercise 1.2.12. Show that any map $E \mapsto m ( E )$ from Lebesgue measurable sets to elements of $[ 0 , + \infty ]$ that obeys the above empty set and countable additivity axioms will also obey the monotonicity and countable subadditivity axioms from Exercise 1.2.3, when restricted to Lebesgue measurable sets of course. 

Exercise 1.2.13. We say that a sequence $E _ { n }$ of sets in $\mathbf { R } ^ { d }$ converges pointwise to another set E in $\mathbf { R } ^ { d }$ if the indicator functions $1 _ { E _ { n } }$ converge pointwise to $1 _ { E }$ 

(i) Show that if the $E _ { n }$ are all Lebesgue measurable, and converge pointwise to E, then E is Lebesgue measurable also. (Hint: use the identity $1 _ { E } ( x ) = \operatorname* { l i m } \operatorname* { i n f } _ { n \to \infty } 1 _ { E _ { n } } ( x )$ or $1 _ { E } ( x ) =$ lim $\operatorname* { s u p } _ { n \to \infty } 1 _ { E _ { n } } ( x )$ to write E in terms of countable unions and intersections of the $E _ { n } . )$ 

(ii) (Dominated convergence theorem) Suppose that the $E _ { n }$ are all contained in another Lebesgue measurable set F of finite measure. Show that m $\left( E _ { n } \right)$ converges to $m ( E )$ . (Hint: use the upward and downward monotone convergence theorems, Exercise 1.2.11.) 

(iii) Give a counterexample to show that the dominated convergence theorem fails if the $E _ { n }$ are not contained in a set of finite measure, even if we assume that the $m ( E _ { n } )$ are all uniformly bounded. 

In later sections we will generalise the monotone and dominated convergence theorems to measurable functions instead of measurable sets; see Theorem 1.4.44 and Theorem 1.4.49. 

Exercise 1.2.14. Let $E \subset \mathbf { R } ^ { d }$ . Show that E is contained in a Lebesgue measurable set of measure exactly equal to $m ^ { * } ( E )$ 

Exercise 1.2.15 (Inner regularity). Let $E \subset \mathbf { R } ^ { d }$ be Lebesgue measurable. Show that 

$$
m (E) = \sup _ {K \subset E, K \text { compact}} m (K).
$$

Remark 1.2.16. The inner and outer regularity properties of measure can be used to define the concept of a Radon measure (see §1.10 of An epsilon of room, Vol. I.). 

Exercise 1.2.16 (Criteria for finite measure). Let $E \subset \mathbf { R } ^ { d }$ . Show that the following are equivalent: 

(i) E is Lebesgue measurable with finite measure. 

(ii) (Outer approximation by open) For every $\varepsilon > 0 .$ , one can contain E in an open set U of finite measure with $m ^ { * } ( U \backslash E ) \leq$ ε. 

(iii) (Almost open bounded) E difers from a bounded open set by a set of arbitrarily small Lebesgue outer measure. (In other words, for every $\varepsilon > 0$ there exists a bounded open set U such that $m ^ { * } ( E \Delta U ) \leq \varepsilon . )$ 

(iv) (Inner approximation by compact) For every $\varepsilon > 0$ , one can find a compact set F contained in E with $m ^ { * } ( E \backslash F ) \leq \varepsilon$ 

(v) (Almost compact) E difers from a compact set by a set of arbitrarily small Lebesgue outer measure. 

(vi) (Almost bounded measurable) E difers from a bounded Lebesgue measurable set by a set of arbitrarily small Lebesgue outer measure. 

(vii) (Almost finite measure) E difers from a Lebesgue measurable set with finite measure by a set of arbitrarily small Lebesgue outer measure. 

(viii) (Almost elementary) E difers from an elementary set by a set of arbitrarily small Lebesgue outer measure. 

(ix) (Almost dyadically elementary) For every $\varepsilon > 0$ , there exists an integer n and a finite union F of closed dyadic cubes of sidelength $2 ^ { - n }$ such that $m ^ { * } ( E \Delta F ) \leq \varepsilon$ 

One can interpret the equivalence of (i) and (ix) in the above exercise as asserting that Lebesgue measurable sets are those which look (locally) “pixelated” at suficiently fine scales. This will be formalised in later sections with the Lebesgue diferentiation theorem (Exercise 1.6.24). 

Exercise 1.2.17 (Carath´eodory criterion, one direction). Let $E \subset$ $\mathbf { R } ^ { d }$ . Show that the following are equivalent: 

(i) E is Lebesgue measurable. 

(ii) For every elementary set $A .$ , one has $m ( A ) = m ^ { * } ( A \cap E ) +$ $m ^ { * } ( A \backslash E )$ 

(iii) For every box B, one has $| B | = m ^ { * } ( B \cap E ) + m ^ { * } ( B \backslash E )$ 

Exercise 1.2.18 (Inner measure). Let $E \subset \mathbf { R } ^ { d }$ be a bounded set. Define the Lebesgue inner measure $m _ { * } ( E )$ of E by the formula 

$$
m _ {*} (E) := m (A) - m ^ {*} (A \backslash E)
$$

for any elementary set A containing E. 

(i) Show that this definition is well defined, i.e. that if $A , A ^ { \prime }$ are two elementary sets containing E, that $m ( A ) - m ^ { * } ( A \backslash E )$ is equal to $m ( A ^ { \prime } ) - m ^ { * } ( A ^ { \prime } \backslash E )$ 

(ii) Show that $m _ { * } ( E ) \leq m ^ { * } ( E )$ , and that equality holds if and only if E is Lebesgue measurable. 

Define a $G _ { \delta }$ set to be a countable intersection $\cap _ { n = 1 } ^ { \infty } U _ { n }$ of open sets, and an $F _ { \sigma }$ set to be a countable union $\textstyle \bigcup _ { n = 1 } ^ { \infty } F _ { n }$ of closed sets. 

Exercise 1.2.19. Let $E \subset \mathbf { R } ^ { d }$ . Show that the following are equivalent: 

(i) E is Lebesgue measurable. 

(ii) E is a $G _ { \delta }$ set with a null set removed. 

(iii) E is the union of a $F _ { \sigma }$ set and a null set. 

Remark 1.2.17. From the above exercises, we see that when describing what it means for a set to be Lebesgue measurable, there is a tradeof between the type of approximation one is willing to bear, and the type of things one can say about the approximation. If one is only willing to approximate to within a null set, then one can only say that a measurable set is approximated by a $G _ { \delta }$ or a $F _ { \sigma }$ set, which is a fairly weak amount of structure. If one is willing to add on an epsilon of error (as measured in the Lebesgue outer measure), one can make a measurable set open; dually, if one is willing to take away an epsilon of error, one can make a measurable set closed. Finally, if one is willing to both add and subtract an epsilon of error, then one can make a measurable set (of finite measure) elementary, or even a finite union of dyadic cubes. 

Exercise 1.2.20 (Translation invariance). If $E \subset \mathbf { R } ^ { d }$ is Lebesgue measurable, show that $E + x$ is Lebesgue measurable for any $x \in \mathbf { R } ^ { d }$ , and that $m ( E + x ) = m ( E )$ 

Exercise 1.2.21 (Change of variables). If $E \subset \mathbf { R } ^ { d }$ is Lebesgue measurable, and $T : \mathbf { R } ^ { d }  \mathbf { R } ^ { d }$ is a linear transformation, show that $T ( E )$ is Lebesgue measurable, and that m $( T ( E ) ) = | \operatorname* { d e t } T | m ( E )$ . We caution that if $T : \mathbf { R } ^ { d }  \mathbf { R } ^ { d ^ { \prime } }$ is a linear map to a space $\mathbf { R } ^ { d ^ { \prime } }$ of strictly smaller dimension than $\mathbf { R } ^ { d }$ , then $T ( E )$ need not be Lebesgue measurable; see Exercise 1.2.27. 

Exercise 1.2.22. Let $d , d ^ { \prime } \geq 1$ be natural numbers. 

(i) If $E \subset \mathbf { R } ^ { d }$ and $F \subset \mathbf { R } ^ { d ^ { \prime } }$ , show that $( m ^ { d + d ^ { \prime } } ) ^ { * } ( E \times F ) \ \leq$ $( m ^ { d } ) ^ { * } ( E ) ( m ^ { d ^ { \prime } } ) ^ { * } ( F )$ , where $( m ^ { d } ) ^ { * }$ denotes d-dimensional Lebesgue measure, etc. 

(ii) Let $E \subset { \mathbf { R } } ^ { d } , F \subset { \mathbf { R } } ^ { d ^ { \prime } }$ be Lebesgue measurable sets. Show that $E \times F \subset \mathbf { R } ^ { d + d ^ { \prime } }$ is Lebesgue measurable, with $m ^ { d + d ^ { \prime } } ( E \times$ $F ) = m ^ { d } ( E ) \cdot m ^ { d ^ { \prime } } ( F )$ . (Note that we allow $E$ or $F$ to have infinite measure, and so one may have to divide into cases or take advantage of the monotone convergence theorem for Lebesgue measure, Exercise 1.2.11.) 

Exercise 1.2.23 (Uniqueness of Lebesgue measure). Show that Lebesgue measure $E \mapsto m ( E )$ is the only map from Lebesgue measurable sets to $[ 0 , + \infty ]$ that obeys the following axioms: 

(i) (Empty set) $m ( \emptyset ) = 0$ 

(ii) (Countable additivity) If $E _ { 1 } , E _ { 2 } , \ldots \subset \mathbf { R } ^ { d }$ is a countable sequence of disjoint Lebesgue measurable sets, then $m ( \bigcup _ { n = 1 } ^ { \infty } E _ { n } ) =$ $\scriptstyle \sum _ { n = 1 } ^ { \infty } m ( E _ { n } )$ 

(iii) (Translation invariance) If E is Lebesgue measurable and $x \in \mathbf { R } ^ { d }$ , then $m ( E + x ) = m ( E )$ 

(iv) (Normalisation) $m ( [ 0 , 1 ] ^ { d } ) = 1$ 

Hint: First show that m must match elementary measure on elementary sets, then show that m is bounded by outer measure. 

Exercise 1.2.24 (Lebesgue measure as the completion of elementary measure). The purpose of the following exercise is to indicate how Lebesgue measure can be viewed as a metric completion of elementary measure in some sense. To avoid some technicalities we will not work in all of $\mathbf { R } ^ { d }$ , but in some fixed elementary set $A \ ( \mathrm { e . g . } A = [ 0 , 1 ] ^ { d } )$ 

(i) Let $2 ^ { A } : = \{ E : E \subset A \}$ be the power set of A. We say that two sets E, $F \in 2 ^ { A }$ are equivalent if $E \Delta F$ is a null set. Show that this is a equivalence relation. 

(ii) Let $2 ^ { A } / \sim$ be the set of equivalence classes $[ E ] : = \{ F \in $ $2 ^ { A } : E \sim F \}$ of $2 ^ { A }$ with respect to the above equivalence relation. Define a distance d : $2 ^ { A } / \sim \times 2 ^ { A } / \sim \to \mathbf { R } ^ { + }$ between two equivalence classes $[ E ] , [ E ^ { \prime } ]$ by defining $d ( [ E ] , [ E ^ { \prime } ] ) : =$ $m ^ { * } ( E \Delta E ^ { \prime } )$ . Show that this distance is well-defined (in the sense that $m ( E \Delta E ^ { \prime } ) = m ( F \Delta F ^ { \prime } )$ whenever $[ E ] = [ F ]$ and $[ E ^ { \prime } ] = [ F ^ { \prime } ] )$ ) and gives $2 ^ { A } / \sim$ the structure of a complete metric space. 

(iii) Let ${ \mathcal { E } } \subset 2 ^ { A }$ be the elementary subsets of A, and let ${ \mathcal { L } } \subset 2 ^ { A }$ be the Lebesgue measurable subsets of A. Show that $\mathcal { L } / \sim$ is the closure of $\mathcal { E } / \sim$ with respect to the metric defined above. In particular, $\mathcal { L } / \sim$ is a complete metric space that contains $\mathcal { E } / \sim$ as a dense subset; in other words, $\mathcal { L } / \sim$ is a metric completion of $\mathcal { E } / \sim$ 

(iv) Show that Lebesgue measure m $: { \mathcal { L } }  \mathbf { R } ^ { + }$ descends to a continuous function $m : \mathcal { L } / \sim \to \mathbf { R ^ { + } }$ , which by abuse of notation we shall still call m. Show that m : $\mathcal { L } / \sim \to \mathbf { R } ^ { + }$ is the unique continuous extension of the analogous elementary measure function m : $\mathbf { \mathcal { E } } / \sim \to \mathbf { R ^ { + } }$ to $\mathcal { L } / \sim$ 

For a further discussion of how measures can be viewed as completions of elementary measures, see §2.1 of An epsilon of room, Vol. I. 

Exercise 1.2.25. Define a continuously diferentiable curve in $\mathbf { R } ^ { d }$ to be a set of the form $\{ \gamma ( t ) : a \leq t \leq b \}$ where $[ a , b ]$ is a closed interva and $\gamma : [ a , b ]  \mathbf { R } ^ { d }$ is a continuously diferentiable function. 

(i) If $d \geq 2$ , show that every continuously diferentiable curve has Lebesgue measure zero. (Why is the condition $d \geq 2$ necessary?) 

(ii) Conclude that if $d \ge 2$ , then the unit cube $[ 0 , 1 ] ^ { d }$ cannot be covered by countably many continuously diferentiable curves. 

We remark that if the curve is only assumed to be continuous, rather than continuously diferentiable, then these claims fail, thanks to the existence of space-filling curves. 

1.2.3. Non-measurable sets. In the previous section we have set out a rich theory of Lebesgue measure, which enjoys many nice properties when applied to Lebesgue measurable sets. 

Thus far, we have not ruled out the possibility that every single set is Lebesgue measurable. There is good reason for this: a famous theorem of Solovay[So1970] asserts that, if one is willing to drop the axiom of choice, there exist models of set theory in which all subsets of $\mathbf { R } ^ { d }$ are measurable. So any demonstration of the existence of nonmeasurable sets must use the axiom of choice in some essential way. 

That said, we can give an informal (and highly non-rigorous) motivation as to why non-measurable sets should exist, using intuition from probability theory rather than from set theory. The starting point is the observation that Lebesgue sets of finite measure (and in particular, bounded Lebesgue sets) have to be “almost elementary”, in the sense of Exercise 1.2.16. So all we need to do to build a non-measurable set is to exhibit a bounded set which is not almost elementary. Intuitively, we want to build a set which has oscillatory structure even at arbitrarily fine scales. 

We will non-rigorously do this as follows. We will work inside the unit interval [0, 1]. For each $x \in [ 0 , 1 ]$ , we imagine that we flip a coin to give either heads or tails (with an independent coin flip for each x), and let $E \subset [ 0 , 1 ]$ be the set of all the $x \in [ 0 , 1 ]$ for which the coin flip came up heads. We suppose for contradiction that E is Lebesgue measurable. Intuitively, since each x had a 50% chance of being heads, E should occupy about $\mathrm { \ddot { b a l f } \vec { \Omega } }$ of $[ 0 , 1 ]$ ; applying the law of large numbers (see e.g. [Ta2009, §1.4]) in an extremely nonrigorous fashion, we thus expect $m ( E )$ to equal $1 / 2$ 

Moreover, given any subinterval $[ a , b ]$ of [0, 1], the same reasoning leads us to expect that $E \cap [ a , b ]$ should occupy about half of $[ a , b ]$ so that $m ( E \cap [ a , b ] )$ should be $| [ a , b ] | / 2$ . More generally, given any elementary set $F$ in [0, 1], we should have $m ( E \cap F ) = m ( F ) / 2$ This makes it very hard for E to be approximated by an elementary set; indeed, a little algebra then shows that $m ( E \Delta F ) = 1 / 2$ for any elementary $F \subset [ 0 , 1 ]$ . Thus E is not Lebesgue measurable. 

Unfortunately, the above argument is terribly non-rigorous for a number of reasons, not the least of which is that it uses an uncountable number of coin flips, and the rigorous probabilistic theory that one would have to use to model such a system of random variables is too weak<sup>12</sup> to be able to assign meaningful probabilities to such events as $^ { 6 6 } E$ is Lebesgue measurable”. So we now turn to more rigorous arguments that establish the existence of non-measurable sets. The arguments will be fairly simple, but the sets constructed are somewhat artificial in nature. 

Proposition 1.2.18. There exists a subset $E \subset [ 0 , 1 ]$ which is not Lebesgue measurable. 

Proof. We use the fact that the rationals Q are an additive subgroup of the reals $\mathbf { R } ,$ and so partition the reals R into disjoint cosets $x + \mathbf { Q }$ This creates a quotient group $\mathbf { R } / \mathbf { Q } \ : = \ \{ x + \mathbf { Q } \ : \ x \in \ \mathbf { R } \}$ . Each coset C of $\mathbf { R } / \mathbf { Q }$ is dense in R, and so has a non-empty intersection with [0, 1]. Applying the axiom of choice, we may thus find an element $x _ { C } \in C \cap [ 0 , 1 ]$ for each $C \in \mathbf { R } / \mathbf { Q }$ . We then let $E : = \{ x _ { C } : C \in \mathbf { R } / \mathbf { Q } \}$ be the collection of all these coset representatives. By construction, $E \subset [ 0 , 1 ]$ 

Let y be any element of $[ 0 , 1 ]$ . Then it must lie in some coset C of $\mathbf { R } / \mathbf { Q }$ , and thus difers from $x _ { C }$ by some rational number in $[ - 1 , 1 ]$ In other words, we have 

$$
[ 0, 1 ] \subset \bigcup_ {q \in \mathbf {Q} \cap [ - 1, 1 ]} (E + q).\tag{1.4}
$$

On the other hand, we clearly have 

$$
\bigcup_ {q \in \mathbf {Q} \cap [ - 1, 1 ]} (E + q) \subset [ - 1, 2 ].\tag{1.5}
$$

Also, the diferent translates $E + q$ are disjoint, because E contains only one element from each coset of $\mathbf { Q } .$ 

We claim that E is not Lebesgue measurable. To see this, suppose for contradiction that E was Lebesgue measurable. Then the translates $E + q$ would also be Lebesgue measurable. By countable additivity, we thus have 

$$
m (\bigcup_ {q \in \mathbf {Q} \cap [ - 1, 1 ]} (E + q)) = \sum_ {q \in \mathbf {Q} \cap [ - 1, 1 ]} m (E + q),
$$

and thus by translation invariance and (1.4), (1.5) 

$$
1 \leq \sum_ {q \in \mathbf {Q} \cap [ - 1, 1 ]} m (E) \leq 3.
$$

On the other hand, the sum $\sum _ { q \in \mathbf { Q } \cap \left[ - 1 , 1 \right] } m ( E )$ is either zero (if $m ( E ) = 0 )$ or infinite (if $m ( E ) > 0 )$ , leading to the desired contradiction.  

Exercise 1.2.26 (Outer measure is not finitely additive). Show that there exists disjoint bounded subsets E, F of the real line such that $m ^ { * } ( E \cup F ) \neq m ^ { * } ( E ) + m ^ { * } ( F )$ . (Hint: Show that the set constructed in the proof of the above proposition has positive outer measure.) 

Exercise 1.2.27 (Projections of measurable sets need not be measurable). Let $\pi : \mathbf { R } ^ { 2 }  \mathbf { R }$ be the coordinate projection $\pi ( x , y ) : = x$ Show that there exists a measurable subset $E$ of $\mathbf { R } ^ { 2 }$ such that $\pi ( E )$ is not measurable. 

Remark 1.2.19. The above discussion shows that, in the presence of the axiom of choice, one cannot hope to extend Lebesgue measure to arbitrary subsets of R while retaining both the countable additivity and the translation invariance properties. If one drops the translation invariant requirement, then this question concerns the theory of measurable cardinals, and is not decidable from the standard ZFC axioms. On the other hand, one can construct finitely additive translation invariant extensions of Lebesgue measure to the power set of R by use of the Hahn-Banach theorem (§1.5 of An epsilon of room, Vol. I) to extend the integration functional, though we will not do so here. 

## 1.3. The Lebesgue integral

In Section 1.2, we defined the Lebesgue measure $m ( E )$ of a Lebesgue measurable set $E \subset \mathbf { R } ^ { d }$ , and set out the basic properties of this measure. In this set of notes, we use Lebesgue measure to define the Lebesgue integral 

$$
\int_ {\mathbf {R} ^ {d}} f (x) d x
$$

of functions $f : { \mathbf { R } } ^ { d }  { \mathbf { C } } \cup \{ \infty \}$ . Just as not every set can be measured by Lebesgue measure, not every function can be integrated by the Lebesgue integral; the function will need to be Lebesgue measurable. Furthermore, the function will either need to be unsigned (taking values on $\lbrack 0 , + \infty ] )$ , or absolutely integrable. 

To motivate the Lebesgue integral, let us first briefly review two simpler integration concepts. The first is that of an infinite summation 

$$
\sum_ {n = 1} ^ {\infty} c _ {n}
$$

of a sequence of numbers $c _ { n }$ , which can be viewed as a discrete analogue of the Lebesgue integral. Actually, there are two overlapping, but diferent, notions of summation that we wish to recall here. The first is that of the unsigned infinite sum, when the $c _ { n }$ lie in the extended non-negative real axis $[ 0 , + \infty ]$ . In this case, the infinite sum can be defined as the limit of the partial sums 

$$
\sum_ {n = 1} ^ {\infty} c _ {n} = \lim _ {N \to \infty} \sum_ {n = 1} ^ {N} c _ {n}\tag{1.6}
$$

or equivalently as a supremum of arbitrary finite partial sums: 

$$
\sum_ {n = 1} ^ {\infty} c _ {n} = \sup _ {A \subset \mathbf {N}, A \text {finite}} \sum_ {n \in A} c _ {n}.\tag{1.7}
$$

The unsigned infinite sum $\textstyle \sum _ { n = 1 } ^ { \infty } c _ { n }$ always exists, but its value may be infinite, even when each term is individually finite (consider e.g. $\textstyle \sum _ { n = 1 } ^ { \infty } 1 )$ 

The second notion of a summation is the absolutely summable infinite sum, in which the $c _ { n }$ lie in the complex plane C and obey the absolute summability condition 

$$
\sum_ {n = 1} ^ {\infty} | c _ {n} | <   \infty ,
$$

where the left-hand side is of course an unsigned infinite sum. When this occurs, one can show that the partial sums $\sum _ { n = 1 } ^ { N } c _ { n }$ converge to a limit, and we can then define the infinite sum by the same formula (1.6) as in the unsigned case, though now the sum takes values in C rather than [0, +∞]. The absolute summability condition confers a number of useful properties that are not obeyed by sums that are merely conditionally convergent; most notably, the value of an absolutely convergent sum is unchanged if one rearranges the terms in the series in an arbitrary fashion. Note also that the absolutely summable infinite sums can be defined in terms of the unsigned infinite sums by taking advantage of the formulae 

$$
\sum_ {n = 1} ^ {\infty} c _ {n} = (\sum_ {n = 1} ^ {\infty} \mathrm{Re} (c _ {n})) + i (\sum_ {n = 1} ^ {\infty} \mathrm{Im} (c _ {n}))
$$

for complex absolutely summable $c _ { n }$ , and 

$$
\sum_ {n = 1} ^ {\infty} c _ {n} = \sum_ {n = 1} ^ {\infty} c _ {n} ^ {+} - \sum_ {n = 1} ^ {\infty} c _ {n} ^ {-}
$$

for real absolutely summable $c _ { n }$ , where $c _ { n } ^ { + } : = \operatorname* { m a x } ( c _ { n } , 0 )$ and $c _ { n } ^ { - } : = $ max $( - c _ { n } , 0 )$ are the (magnitudes of the) positive and negative parts of $c _ { n }$ . 

In an analogous spirit, we will first define an unsigned Lebesgue integral $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx of (measurable) unsigned functions $f : \mathbf { R } ^ { d } $ $[ 0 , + \infty ]$ , and then use that to define the absolutely convergent Lebesgue integral $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx of absolutely integrable functions $f : \mathbf { R } ^ { d } \ $ $\mathbf { C } \cup \{ \infty \}$ . (In contrast to absolutely summable series, which cannot have any infinite terms, absolutely integrable functions will be allowed to occasionally become infinite. However, as we will see, this can only happen on a set of Lebesgue measure zero.) 

To define the unsigned Lebesgue integral, we now turn to another more basic notion of integration, namely the $\textstyle \int _ { a } ^ { b } f ( x )$ dx of a Riemann integrable function $f : [ a , b ]  \mathbf { R }$ . Recall from Section 1.1 that this integral is equal to the lower Darboux integral 

$$
\int_ {a} ^ {b} f (x) = \underline {{\int_ {a} ^ {b}}} f (x) d x := \sup _ {g \leq f; g \text {   piecewise   constant }} \text { p.c. } \int_ {a} ^ {b} g (x) d x.
$$

(It is also equal to the upper Darboux integral; but much as the theory of Lebesgue measure is easiest to define by relying solely on outer measure and not on inner measure, the theory of the unsigned Lebesgue integral is easiest to define by relying solely on lower integrals rather than upper ones; the upper integral is somewhat problematic when dealing with “improper” integrals of functions that are unbounded or are supported on sets of infinite measure.) Compare this formula also with (1.7). The integral p.c. $\textstyle \int _ { a } ^ { b } g ( x )$ dx is a piecewise constant integral, formed by breaking up the piecewise constant functions $g , h$ into finite linear combinations of indicator functions $1 _ { I }$ of intervals I, and then measuring the length of each interval. 

It turns out that virtually the same definition allows us to define a lower Lebesgue integral $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx of any unsigned function $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ , simply by replacing intervals with the more general class of Lebesgue measurable sets (and thus replacing piecewise constant functions with the more general class of simple functions). If the function is Lebesgue measurable (a concept that we will define presently), then we refer to the lower Lebesgue integral simply as the 

Lebesgue integral. As we shall see, it obeys all the basic properties one expects of an integral, such as monotonicity and additivity; in subsequent notes we will also see that it behaves quite well with respect to limits, as we shall see by establishing the two basic convergence theorems of the unsigned Lebesgue integral, namely Fatou’s lemma (Corollary 1.4.47) and the monotone convergence theorem (Theorem 1.4.44). 

Once we have the theory of the unsigned Lebesgue integral, we will then be able to define the absolutely convergent Lebesgue integral, similarly to how the absolutely convergent infinite sum can be defined using the unsigned infinite sum. This integral also obeys all the basic properties one expects, such as linearity and compatibility with the more classical Riemann integral; in subsequent notes we will see that it also obeys a fundamentally important convergence theorem, the dominated convergence theorem (Theorem 1.4.49). This convergence theorem makes the Lebesgue integral (and its abstract generalisations to other measure spaces than $\mathbf { R } ^ { d } )$ ) particularly suitable for analysis, as well as allied fields that rely heavily on limits of functions, such as PDE, probability, and ergodic theory. 

Remark 1.3.1. This is not the only route to setting up the unsigned and absolutely convergent Lebesgue integrals. For instance, one can proceed with the unsigned integral but then making an auxiliary stop at integration of functions that are bounded and are supported on a set of finite measure, before going to the absolutely convergent Lebesgue integral; see e.g. [StSk2005]. Another approach (which will not be discussed here) is to take the metric completion of the Riemann integral with respect to the $L ^ { 1 }$ metric. 

The Lebesgue integral and Lebesgue measure can be viewed as completions of the Riemann integral and Jordan measure respectively. This means three things. Firstly, the Lebesgue theory extends the Riemann theory: every Jordan measurable set is Lebesgue measurable, and every Riemann integrable function is Lebesgue measurable, with the measures and integrals from the two theories being compatible. Conversely, the Lebesgue theory can be approximated by the Riemann theory; as we saw in Section 1.2, every Lebesgue measurable set can be approximated (in various senses) by simpler sets, such as open sets or elementary sets, and in a similar fashion, Lebesgue measurable functions can be approximated by nicer functions, such as Riemann integrable or continuous functions. Finally, the Lebesgue theory is complete in various ways; this is formalised in §1.3 of An epsilon of room, Vol. I, but the convergence theorems mentioned above already hint at this completeness. A related fact, known as Egorov’s theorem, asserts that a pointwise converging sequence of functions can be approximated as a (locally) uniformly converging sequence of functions. The facts listed here manifestations of Littlewood’s three principles of real analysis (Section 1.3.5), which capture much of the essence of the Lebesgue theory. 

1.3.1. Integration of simple functions. Much as the Riemann integral was set up by first using the integral for piecewise constant functions, the Lebesgue integral is set up using the integral for simple functions. 

Definition 1.3.2 (Simple function). A (complex-valued) simple function $f : \mathbf { R } ^ { d }  \mathbf { C }$ is a finite linear combination 

$$
f = c _ {1} 1 _ {E _ {1}} + \ldots + c _ {k} 1 _ {E _ {k}}\tag{1.8}
$$

of indicator functions $1 _ { E _ { i } }$ of Lebesgue measurable sets $E _ { i } \subset \mathbf { R } ^ { d }$ for $i = 1 , \ldots , k$ , where $k \geq 0$ is a natural number and $c _ { 1 } , \dotsc , c _ { k } \in \mathbf { C }$ are complex numbers. An unsigned simple function $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ , is defined similarly, but with the $c _ { i }$ taking values in $[ 0 , + \infty ]$ rather than C. 

It is clear from construction that the space $\mathrm { S i m p } ( { \bf R } ^ { d } )$ of complexvalued simple functions forms a complex vector space; also, $\mathrm { S i m p } ( { \bf R } ^ { d } )$ also closed under pointwise product $f , g \mapsto f g$ and complex conjuga tion $f \mapsto { \overline { { f } } } .$ . In short, $\mathrm { S i m p } ( { \bf R } ^ { d } )$ is a commutative $* - a l g e b r a$ . Meanwhile, the space $\mathrm { S i m p } ^ { + } ( { \bf R } ^ { d } )$ of unsigned simple functions is a $[ 0 , + \infty ] -$ module; it is closed under addition, and under scalar multiplication by elements in $[ 0 , + \infty ]$ 

In this definition, we did not require the $E _ { 1 } , \ldots , E _ { k }$ to be disjoint. However, it is easy enough to arrange this, basically by exploiting Venn diagrams (or, to use fancier language, finite boolean algebras). Indeed, any k subsets $E _ { 1 } , \ldots , E _ { k }$ of $\mathbf { R } ^ { d }$ partition $\mathbf { R } ^ { d }$ into $2 ^ { k }$ disjoint sets, each of which is an intersection of $E _ { i }$ or the complement $\mathbf { R } ^ { d } \backslash E _ { i }$ for $i = 1 , \ldots , k$ (and in particular, is measurable). The (complex or unsigned) simple function is constant on each of these sets, and so can easily be decomposed as a linear combination of the indicator function of these sets. One easy consequence of this is that if f is a complexvalued simple function, then its absolute value $| f | : x \mapsto | f ( x ) |$ is an unsigned simple function. 

It is geometrically intuitive that we should define the integral $\int _ { \mathbf { R } ^ { d } } 1 _ { E } ( x )$ dx of an indicator function of a measurable set $E$ to equal $m ( E )$ 

$$
\int_ {\mathbf {R} ^ {d}} 1 _ {E} (x) d x = m (E).
$$

Using this and applying the laws of integration formally, we are led to propose the following definition for the integral of an unsigned simple function: 

Definition 1.3.3 (Integral of a unsigned simple function). If $f =$ $c _ { 1 } 1 _ { E _ { 1 } } + \ldots + c _ { k } 1 _ { E _ { k } }$ is an unsigned simple function, the integral Simp $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx is defined by the formula 

$$
\mathrm{Simp} \int_ {\mathbf {R} ^ {d}} f (x) d x := c _ {1} m (E _ {1}) + \ldots + c _ {k} m (E _ {k}),
$$

thus Simp $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx will take values in $[ 0 , + \infty ]$ 

However, one has to actually check that this definition is welldefined, in the sense that diferent representations 

$$
f = c _ {1} 1 _ {E _ {1}} + \ldots + c _ {k} 1 _ {E _ {k}} = c _ {1} ^ {\prime} 1 _ {E _ {1} ^ {\prime}} + \ldots + c _ {k ^ {\prime}} ^ {\prime} 1 _ {E _ {k ^ {\prime}} ^ {\prime}}
$$

of a function as a finite unsigned combination of indicator functions of measurable sets will give the same value for the integral Simp $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx. This is the purpose of the following lemma: 

Lemma 1.3.4 (Well-definedness of simple integral). Let $k , k ^ { \prime } \geq 0$ be 

natural numbers, $c _ { 1 } , \ldots , c _ { k } , c _ { 1 } ^ { \prime } , \ldots , c _ { k ^ { \prime } } ^ { \prime } \in [ 0 , + \infty ]$ , and let $E _ { 1 } , \ldots , E _ { k } , E _ { 1 } ^ { \prime } , \ldots , E _ { k ^ { \prime } } ^ { \prime } \subset$ $\mathbf { R } ^ { d }$ be Lebesgue measurable sets such that the identity 

$$
c _ {1} 1 _ {E _ {1}} + \ldots + c _ {k} 1 _ {E _ {k}} = c _ {1} ^ {\prime} 1 _ {E _ {1} ^ {\prime}} + \ldots + c _ {k ^ {\prime}} ^ {\prime} 1 _ {E _ {k ^ {\prime}} ^ {\prime}}\tag{1.9}
$$

holds identically on $\mathbf { R } ^ { d }$ . Then one has 

$$
c _ {1} m (E _ {1}) + \ldots + c _ {k} m (E _ {k}) = c _ {1} ^ {\prime} m (E _ {1} ^ {\prime}) + \ldots + c _ {k ^ {\prime}} ^ {\prime} m (E _ {k ^ {\prime}} ^ {\prime}).
$$

Proof. We again use a Venn diagram argument. The $k + k ^ { \prime }$ sets $E _ { 1 } , \ldots , E _ { k } , E _ { 1 } ^ { \prime } , \ldots , E _ { k ^ { \prime } } ^ { \prime }$ partition $\mathbf { R } ^ { d }$ into $2 ^ { k + k ^ { \prime } }$ disjoint sets, each of which is an intersection of some of the $E _ { 1 } , \ldots , E _ { k } , E _ { 1 } ^ { \prime } , \ldots , E _ { k ^ { \prime } } ^ { \prime }$ and their complements. We throw away any sets that are empty, leaving us with a partition of $\mathbf { R } ^ { d }$ into m non-empty disjoint sets $A _ { 1 } , \ldots , A _ { m }$ for some $0 \leq m \leq 2 ^ { k + k ^ { \prime } }$ . As the $E _ { 1 } , \ldots , E _ { k } , E _ { 1 } ^ { \prime } , \ldots , E _ { k } ^ { \prime }$ are Lebesgue measurable, the $A _ { 1 } , \ldots , A _ { m }$ are too. By construction, each of the $E _ { 1 } , \dots , E _ { k } , E _ { 1 } ^ { \prime } , \dots , E _ { k ^ { \prime } }$ arise as unions of some of the $A _ { 1 } , \ldots , A _ { m }$ thus we can write 

$$
E _ {i} = \bigcup_ {j \in J _ {i}} A _ {j}
$$

and 

$$
E _ {i ^ {\prime}} ^ {\prime} = \bigcup_ {j ^ {\prime} \in J _ {i ^ {\prime}} ^ {\prime}} A _ {j ^ {\prime}}
$$

for all $i = 1 , \ldots , k$ and $i ^ { \prime } = 1 , \ldots , k ^ { \prime }$ , and some subsets $J _ { i } , J _ { i ^ { \prime } } ^ { \prime } \subset$ $\{ 1 , \ldots , m \}$ . By finite additivity of Lebesgue measure, we thus have 

$$
m (E _ {i}) = \sum_ {j \in J _ {i}} m (A _ {j})
$$

and 

$$
m (E _ {i ^ {\prime}} ^ {\prime}) = \sum_ {j \in J _ {i ^ {\prime}} ^ {\prime}} m (A _ {j})
$$

Thus, our objective is now to show that 

$$
\sum_ {i = 1} ^ {k} c _ {i} \sum_ {j \in J _ {i}} m (A _ {j}) = \sum_ {i ^ {\prime} = 1} ^ {k ^ {\prime}} c _ {i ^ {\prime}} ^ {\prime} \sum_ {j \in J _ {i ^ {\prime}} ^ {\prime}} m (A _ {j}).\tag{1.10}
$$

To obtain this, we fix $1 \leq j \leq m$ and evaluate (1.9) at a point x in the non-empty set $A _ { j }$ . At such a point, $1 _ { E _ { i } } ( x )$ is equal to $1 _ { J _ { i } } ( j )$ , and similarly $1 _ { E _ { i ^ { \prime } } ^ { \prime } }$ is equal to $1 _ { J _ { i ^ { \prime } } ^ { \prime } } ( j )$ . From (1.9) we conclude that 

$$
\sum_ {i = 1} ^ {k} c _ {i} 1 _ {J _ {i}} (j) = \sum_ {i ^ {\prime} = 1} ^ {k ^ {\prime}} c _ {i ^ {\prime}} ^ {\prime} 1 _ {J _ {i ^ {\prime}} ^ {\prime}} (j).
$$

Multiplying this by $m ( A _ { j } )$ and then summing over all $j = 1 , \dots , m$ we obtain (1.10).  

We now make some important definitions that we will use repeatedly in this text: 

Definition 1.3.5 (Almost everywhere and support). A property $P ( x )$ of a point $x \in \mathbf { R } ^ { d }$ is said to hold (Lebesgue) almost everywhere in $\mathbf { R } ^ { d }$ , or for (Lebesgue) almost every point $x \in \mathbf { R } ^ { d }$ , if the set of $x \in \mathbf { R } ^ { d }$ for which $P ( x )$ fails has Lebesgue measure zero (i.e. P is true outside of a null set). We usually omit the prefix Lebesgue, and often abbreviate “almost everywhere” or “almost every” as a.e. 

Two functions $f , g : \mathbf { R } ^ { d }  Z$ into an arbitrary range $Z$ are said to agree almost everywhere if one has $f ( x ) = g ( x )$ for almost every $x \in \mathbf { R } ^ { d }$ 

The support of a function $f : \mathbf { R } ^ { d }  \mathbf { C }$ or $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ is defined to be the set $\{ x \in \mathbf { R } ^ { d } : f ( x ) \neq 0 \}$ where f is non-zero. 

Note that if $P ( x )$ holds for almost every x, and $P ( x )$ implies $Q ( x )$ 1 then $Q ( x )$ holds for almost every x. Also, if $P _ { 1 } ( x ) , P _ { 2 } ( x ) , . .$ . are an at most countable family of properties, each of which individually holds for almost every x, then they will simultaneously be true for almost every x, because the countable union of null sets is still a null set. Because of these properties, one can (as a rule of thumb) treat the almost universal quantifier “for almost every” as if it was the truly universal quantifier “for every”, as long as one is only concatenating at most countably many properties together, and as long as one never specialises the free variable x to a null set. Observe also that the property of agreeing almost everywhere is an equivalence relation, which we will refer to as almost everywhere equivalence. 

In An epsilon of room, Vol. I we will also see the notion of the closed support of a function $f : \mathbf { R } ^ { d }  \mathbf { C }$ , defined as the closure of the support. 

The following properties of the simple unsigned integral are easily obtained from the definitions: 

Exercise 1.3.1 (Basic properties of the simple unsigned integral). Let $f , g : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ be simple unsigned functions. 

(i) (Unsigned linearity) We have 

$$
\begin{array}{c} \operatorname{Simp} \int_ {\mathbf {R} ^ {d}} f (x) + g (x) d x = \operatorname{Simp} \int_ {\mathbf {R} ^ {d}} f (x) d x \\ + \operatorname{Simp} \int_ {\mathbf {R} ^ {d}} g (x) d x \end{array}
$$

and 

$$
\operatorname{Simp} \int_ {\mathbf {R} ^ {d}} c f (x) d x = c \times \operatorname{Simp} \int_ {\mathbf {R} ^ {d}} f (x) d x
$$

for all $c \in [ 0 , + \infty ]$ 

(ii) (Finiteness) We have Simp $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx $< \infty$ if and only if $f$ is finite almost everywhere, and its support has finite measure. 

(iii) (Vanishing) We have Simp $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx = 0 if and only if $f$ is zero almost everywhere. 

(iv) (Equivalence) If f and g agree almost everywhere, then Simp $\textstyle \int _ { \mathbf { R } ^ { d } } f ( x ) \ d x = \operatorname* { S i m p } \int _ { \mathbf { R } ^ { d } } g ( x ) \ d x$ 

(v) (Monotonicity) If $f ( x ) \leq g ( x )$ for almost every $x \in \mathbf { R } ^ { d }$ , then Simp $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx ≤ Simp $\scriptstyle \int _ { \mathbf { R } ^ { d } } g ( x )$ dx. 

(vi) (Compatibility with Lebesgue measure) For any Lebesgue measurable E, one has Simp $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } 1 _ { E } ( x ) \ d x = m ( E ) } \end{array}$ 

Furthermore, show that the simple unsigned integral f 7→ Simp $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx is the only map from the space $\mathrm { S i m p } ^ { + } ( { \bf R } ^ { d } )$ of unsigned simple functions to $[ 0 , + \infty ]$ that obeys all of the above properties. 

We can now define an absolutely convergent counterpart to the simple unsigned integral. This integral will soon be superceded by the absolutely Lebesgue integral, but we give it here as motivation for that more general notion of integration. 

Definition 1.3.6 (Absolutely convergent simple integral). A complexvalued simple function $f : \mathbf { R } ^ { d }  \mathbf { C }$ is said to be absolutely integrable of Simp $\int _ { \mathbf { R } ^ { d } } | f ( x ) |$ dx $< \infty$ . If f is absolutely integrable, the integral Simp $\scriptstyle \int _ { \mathbf { R } ^ { d } } f ( x )$ dx is defined for real signed f by the formula 

$$
\operatorname{Simp} \int_ {\mathbf {R} ^ {d}} f (x) d x := \operatorname{Simp} \int_ {\mathbf {R} ^ {d}} f _ {+} (x) d x - \operatorname{Simp} \int_ {\mathbf {R} ^ {d}} f _ {-} (x) d x
$$

where $f _ { + } ( x ) : = \operatorname* { m a x } ( f ( x ) , 0 )$ and $f _ { - } ( x ) : = \operatorname* { m a x } ( - f ( x ) , 0 )$ (note that these are unsigned simple functions that are pointwise dominated by $| f |$ and thus have finite integral), and for complex-valued f by the formula<sup>13</sup> 

$$
\begin{array}{c} \operatorname{Simp} \int_ {\mathbf {R} ^ {d}} f (x) d x := \operatorname{Simp} \int_ {\mathbf {R} ^ {d}} \operatorname{Re} f (x) d x \\ + i \operatorname{Simp} \int_ {\mathbf {R} ^ {d}} \operatorname{Im} f (x) d x. \end{array}
$$

Note from the preceding exercise that a complex-valued simple function $f$ is absolutely integrable if and only if it has finite measure support (since finiteness almost everywhere is automatic). In particular, the space $\mathrm { S i m p } ^ { a b s } ( { \bf R } ^ { d } )$ of absolutely integrable simple functions is closed under addition and scalar multiplication by complex numbers, and is thus a complex vector space. 

The properties of the unsigned simple integral then can be used to deduce analogous properties for the complex-valued integral: 

Exercise 1.3.2 (Basic properties of the complex-valued simple integral). Let $f , g : \mathbf { R } ^ { d }  \mathbf { C }$ be absolutely integrable simple functions. 

(i) (*-linearity) We have 

$$
\begin{array}{c} \text {Simp} \int_ {\mathbf {R} ^ {d}} f (x) + g (x) d x = \text {Simp} \int_ {\mathbf {R} ^ {d}} f (x) d x \\ + \text {Simp} \int_ {\mathbf {R} ^ {d}} g (x) d x \end{array}
$$

and 

$$
\operatorname{Simp} \int_ {\mathbf {R} ^ {d}} c f (x) d x = c \times \operatorname{Simp} \int_ {\mathbf {R} ^ {d}} f (x) d x\tag{1.11}
$$

for all $c \in \mathbf { C }$ . Also we have 

$$
\operatorname{Simp} \int_ {\mathbf {R} ^ {d}} \overline {{f}} (x) d x = \overline {{\operatorname{Simp} \int_ {\mathbf {R} ^ {d}} f (x) d x}}.
$$

(ii) (Equivalence) If f and g agree almost everywhere, then Simp $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } f ( x ) \ d x = \operatorname { S i m p } \int _ { \mathbf { R } ^ { d } } g ( x ) \ d x . } \end{array}$ 

(iii) (Compatibility with Lebesgue measure) For any Lebesgue measurable $E ,$ one has Simp $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } 1 _ { E } ( x ) \ d x = m ( E ) } \end{array}$ 

(Hints: Work out the real-valued counterpart of the linearity property first. To establish (1.11), treat the cases $c > 0 , c = 0 , c = - 1$ separately. To deal with the additivity for real functions $f , g .$ , start with the identity 

$$
f + g = (f + g) _ {+} - (f + g) _ {-} = \left(f _ {+} - f _ {-}\right) + \left(g _ {+} - g _ {-}\right)
$$

and rearrange the second inequality so that no subtraction appears.) Furthermore, show that the complex-valued simple integral $f \mapsto$ Simp $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx is the only map from the space $\mathrm { S i m p } ^ { a b s } ( { \bf R } ^ { d } )$ of absolutely integrable simple functions to C that obeys all of the above properties. 

We now comment further on the fact that (simple) functions that agree almost everywhere, have the same integral. We can view this as an assertion that integration is a noise-tolerant operation: one can have “noise” or “errors” in a function $f ( x )$ on a null set, and this will not afect the final value of the integral. Indeed, once one has this noise tolerance, one can even integrate functions f that are not defined everywhere on $\mathbf { R } ^ { d }$ , but merely defined almost everywhere on $\mathbf { R } ^ { d }$ (i.e. f is defined on some set $\mathbf { R } ^ { d } \backslash N$ where N is a null set), simply by extending f to all of $\mathbf { R } ^ { d }$ in some arbitrary fashion (e.g. by setting f equal to zero on N). This is extremely convenient for analysis, as there are many natural functions $( \mathrm { e . g . } \ \frac { \sin x } { x }$ in one dimension, or $\frac { 1 } { | x | ^ { \alpha } }$ for various $\alpha > 0$ in higher dimensions) that are only defined almost everywhere instead of everywhere (often due to “division by $\scriptstyle \mathrm { z e r o } ^ { \prime \prime }$ problems when a denominator vanishes). While such functions cannot be evaulated at certain singular points, they can still be integrated (provided they obey some integrability condition, of course, such as absolute integrability), and so one can still perform a large portion of analysis on such functions. 

In fact, in the subfield of analysis known as functional analysis, it is convenient to abstract the notion of an almost everywhere defined function somewhat, by replacing any such function f with the equivalence class of almost everywhere defined functions that are equal to f almost everywhere. Such classes are then no longer functions in the standard set-theoretic sense (they do not map each point in the domain to a unique point in the range, since points in $\mathbf { R } ^ { d }$ have measure zero), but the properties of various function spaces improve when one does this (various semi-norms become norms, various topologies become Hausdorf, and so forth). See §1.3 of An epsilon of room, Vol. I for further discussion. 

Remark 1.3.7. The “Lebesgue philosophy” that one is willing to lose control on sets of measure zero is a perspective that distinguishes Lebesgue-type analysis from other types of analysis, most notably that of descriptive set theory, which is also interested in studying subsets of $\mathbf { R } ^ { d }$ , but can give completely diferent structural classifications to a pair of sets that agree almost everywhere. This loss of control on null sets is the price one has to pay for gaining access to the powerful tool of the Lebesgue integral; if one needs to control a function at absolutely every point, and not just almost every point, then one often needs to use other tools than integration theory (unless one has some regularity on the function, such as continuity, that lets one pass from almost everywhere true statements to everywhere true statements). 

1.3.2. Measurable functions. Much as the piecewise constant integral can be completed to the Riemann integral, the unsigned simple integral can be completed to the unsigned Lebesgue integral, by extending the class of unsigned simple functions to the larger class of unsigned Lebesgue measurable functions. One of the shortest ways to define this class is as follows: 

Definition 1.3.8 (Unsigned measurable function). An unsigned function $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ is unsigned Lebesgue measurable, or measurable for short, if it is the pointwise limit of unsigned simple functions, i.e. if there exists a sequence $f _ { 1 } , f _ { 2 } , f _ { 3 } , \ldots : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ of unsigned simple functions such that $f _ { n } ( x )  f ( x )$ for every $x \in \mathbf { R } ^ { d }$ 

This particular definition is not always the most tractable. Fortunately, it has many equivalent forms: 

Lemma 1.3.9 (Equivalent notions of measurability). Let $f : \mathbf { R } ^ { d } $ $[ 0 , + \infty ]$ be an unsigned function. Then the following are equivalent: 

(i) f is unsigned Lebesgue measurable. 

(ii) f is the pointwise limit of unsigned simple functions $f _ { n }$ (thus the limit $\scriptstyle \operatorname* { l i m } _ { n \to \infty } f _ { n } ( x )$ exists and is equal to f(x) for all $\boldsymbol { x } \in \mathbf { R } ^ { d } )$ 

(iii) f is the pointwise almost everywhere limit ofunsigned simple functions $f _ { n }$ (thus the limit $\scriptstyle \operatorname* { l i m } _ { n \to \infty } f _ { n } ( x )$ exists and is equal to f(x) for almost every $\boldsymbol { x } \in \mathbf { R } ^ { d } )$ 

(iv) f is the supremum $f ( x ) = \operatorname* { s u p } _ { n } f _ { n } ( x )$ of an increasing sequence $0 \leq f _ { 1 } \leq f _ { 2 } \leq . . .$ of unsigned simple functions $f _ { n }$ each of which are bounded with finite measure support. 

(v) For every $\lambda \in [ 0 , + \infty ]$ , the set $\{ x \in \mathbf { R } ^ { d } : f ( x ) > \lambda \}$ is Lebesgue measurable. 

(vi) For every $\lambda \in [ 0 , + \infty ]$ , the set $\{ x \in \mathbf { R } ^ { d } : f ( x ) \geq \lambda \}$ is Lebesgue measurable. 

(vii) For every $\lambda \in [ 0 , + \infty ]$ , the set $\{ x \in \mathbf { R } ^ { d } : f ( x ) < \lambda \}$ is Lebesgue measurable. 

(ix) For every $\lambda \in [ 0 , + \infty ]$ , the set $\{ x \in \mathbf { R } ^ { d } : f ( x ) \leq \lambda \}$ is Lebesgue measurable. 

(x) For every interval $I \subset [ 0 , + \infty )$ , the set $f ^ { - 1 } ( I ) : = \{ x \in \mathbf { R } ^ { d }$ $f ( x ) \in I \}$ is Lebesgue measurable. 

(xi) For every (relatively) open set $U \subset [ 0 , + \infty )$ , the set $f ^ { - 1 } ( U ) : =$ $\{ x \in \mathbf { R } ^ { d } : f ( x ) \in U \}$ is Lebesgue measurable. 

(xii) For every (relatively) closed set $K \subset [ 0 , + \infty )$ , the set $f ^ { - 1 } ( K ) : =$ $\{ x \in \mathbf { R } ^ { d } : f ( x ) \in K \}$ is Lebesgue measurable. 

Proof. (i) and (ii) are equivalent by definition. (ii) clearly implies (iii). As every monotone sequence in $[ 0 , + \infty ]$ converges, (iv) implies (ii). Now we show that (iii) implies (v). If f is the pointwise almost everywhere limit of $f _ { n }$ , then for almost every $x \in \mathbf { R } ^ { d }$ one has 

$$
f (x) = \lim _ {n \to \infty} f _ {n} (x) = \operatorname * {l i m s u p} _ {n \to \infty} f _ {n} (x) = \inf _ {N > 0} \sup _ {n \geq N} f _ {n} (x).
$$

This implies that, for any λ, the set $\{ x \in \mathbf { R } ^ { d } : f ( x ) > \lambda \}$ is equal to 

$$
\bigcup_ {M > 0} \bigcap_ {N > 0} \left\{x \in \mathbf {R} ^ {d}: \sup _ {n \geq N} f _ {n} (x) > \lambda + \frac {1}{M} \right\}
$$

outside of a set of measure zero; this set in turn is equal to 

$$
\bigcup_ {M > 0} \bigcap_ {N > 0} \bigcup_ {n \geq N} \left\{x \in \mathbf {R} ^ {d}: f _ {n} (x) > \lambda + \frac {1}{M} \right\}
$$

outside of a set of measure zero. But as each $f _ { n }$ is an unsigned simple function, the sets $\{ x \in \mathbf { R } ^ { d } : f _ { n } ( x ) > \lambda + { \frac { 1 } { M } } \}$ are Lebesgue measurable. Since countable unions or countable intersections of Lebesgue measurable sets are Lebesgue measurable, and modifying a Lebesgue measurable set on a null set produces another Lebesgue measurable set, we obtain (v). 

To obtain the equivalence of (v) and (vi), observe that 

$$
\{x \in \mathbf {R} ^ {d}: f (x) \geq \lambda \} = \bigcap_ {\lambda^ {\prime} \in \mathbf {Q} ^ {+}: \lambda^ {\prime} <   \lambda} \{x \in \mathbf {R} ^ {d}: f (x) > \lambda^ {\prime} \}
$$

for $\lambda \in ( 0 , + \infty ]$ and 

$$
\{x \in \mathbf {R} ^ {d}: f (x) > \lambda \} = \bigcup_ {\lambda^ {\prime} \in \mathbf {Q} ^ {+}: \lambda^ {\prime} > \lambda} \left\{x \in \mathbf {R} ^ {d}: f (x) \geq \lambda^ {\prime} \right\}
$$

$\lambda \in [ 0 , + \infty )$ , where $\mathbf { Q } ^ { + } : = \mathbf { Q } \cap [ 0 , + \infty ]$ are the non-negative rationals. The claim then easily follows from the countable nature of ${ \bf Q } ^ { + }$ (treating the extreme cases $\lambda = 0 , + \infty$ separately if necessary). A similar argument lets one deduce (v) or (vi) from (ix). 

The equivalence of (v), (vi) with (vii), (viii) comes from the observation that $\{ x \ \in \ \mathbf { R } ^ { d } \ : \ f ( x ) \ \leq \ \lambda \}$ is the complement of $\{ x \in$ $\mathbf { R } ^ { d } : f ( x ) > \lambda \}$ , and $\{ x \in \mathbf { R } ^ { d } : f ( x ) < \lambda \}$ is the complement of $\{ x \in \mathbf { R } ^ { d } : f ( x ) \geq \lambda \}$ . A similar argument shows that (x) and (xi) are equivalent. 

By expressing an interval as the intersection of two half-intervals, we see that (ix) follows from $\scriptstyle ( \mathrm { v } ) - ( \mathrm { v i i i } )$ , and so all of $\scriptstyle ( \mathrm { v } ) - ( \mathrm { i x } )$ are now shown to be equivalent. 

Clearly (x) implies (vii), and hence $\scriptstyle ( \mathrm { v } ) - ( \mathrm { i x } )$ . Conversely, because every open set in $[ 0 , + \infty )$ is the union of countably many open intervals in $[ 0 , + \infty )$ , (ix) implies (x). 

The only remaining task is to show that $( \mathrm { v } ) \mathrm { - } ( \mathrm { x i } )$ implies (iv). Let f obey $( \mathrm { v } ) \mathrm { - } ( \mathrm { x i } )$ . For each positive integer n, we let $f _ { n } ( x )$ be defined to be the largest integer multiple of $2 ^ { - n }$ that is less than or equal to min $( f ( x ) , n )$ when $| x | \leq n$ , with $f _ { n } ( x ) : = 0$ for $| x | > n$ 

From construction it is easy to see that the $f _ { n } : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ are increasing and have f as their supremum. Furthermore, each $f _ { n }$ takes on only finitely many values, and for each non-zero value c it attains, the set $f _ { n } ^ { - 1 } ( c )$ takes the form $f ^ { - 1 } ( I _ { c } ) \cap \{ x \in \mathbf { R } ^ { d } : | x | \leq n \}$ for some interval or ray $I _ { c }$ , and is thus measurable. As a consequence, $f _ { n }$ is a simple function, and by construction it is bounded and has finite measure support. The claim follows.  

With these equivalent formulations, we can now generate plenty of measurable functions: 

## Exercise 1.3.3.

(i) Show that every continuous function $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ is measurable. 

(ii) Show that every unsigned simple function is measurable. 

(iii) Show that the supremum, infimum, limit superior, or limit inferior of unsigned measurable functions is unsigned measurable. 

(iv) Show that an unsigned function that is equal almost everywhere to an unsigned measurable function, is itself measurable. 

(v) Show that if a sequence $f _ { n }$ of unsigned measurable functions converges pointwise almost everywhere to an unsigned limit $f ,$ then f is also measurable. 

(vi) If $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ is measurable and $\phi : [ 0 , + \infty ] \ $ $[ 0 , + \infty ]$ is continuous, show that $\phi \circ f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ is measurable. 

(vii) If $f , g$ are unsigned measurable functions, show that $f + g$ and $f g$ are measurable. 

In view of Exercise $1 . 3 . 3 ( \mathrm { i v } )$ , one can define the concept of measurability for an unsigned function that is only defined almost everywhere on $\mathbf { R } ^ { d }$ , rather than everywhere on $\mathbf { R } ^ { d }$ , by extending that function arbitrarily to the null set where it is currently undefined. 

Exercise 1.3.4. Let $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ . Show that f is a bounded unsigned measurable function if and only if $f$ is the uniform limit of bounded simple functions. 

Exercise 1.3.5. Show that an unsigned function $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ is a simple function if and only if it is measurable and takes on at most finitely many values. 

Exercise 1.3.6. Let $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ be an unsigned measurable function. Show that the region $\{ ( x , t ) \in \mathbf { R } ^ { d } \times \mathbf { R } : 0 \leq t \leq f ( x ) \}$ is a measurable subset of $\mathbf { R } ^ { d + 1 }$ . (There is a converse to this statement, but we will wait until Exercise 1.7.24 to prove it, once we have the Fubini-Tonelli theorem (Corollary 1.7.23) available to us.) 

Remark 1.3.10. Lemma 1.3.9 tells us that if $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ is measurable, then $f ^ { - 1 } ( E )$ is Lebesgue measurable for many classes of sets $E .$ . However, we caution that it is not necessarily the case that $f ^ { - 1 } ( E )$ is Lebesgue measurable if $E$ is Lebesgue measurable. To see this, we let $C$ be the Cantor set 

$$
C := \{\sum_ {j = 1} ^ {\infty} a _ {j} 3 ^ {- j}: a _ {j} \in \{0, 2 \} \text {   for   all   } j \}
$$

and let $f : \mathbf { R }  [ 0 , + \infty ]$ be the function defined by setting 

$$
f (x) := \sum_ {j = 1} ^ {\infty} 2 b _ {j} 3 ^ {- j}
$$

whenever $x \in [ 0 , 1 ]$ is not a terminating binary decimal, and so has a unique binary expansion $\begin{array} { r } { x = \sum _ { j = 1 } ^ { \infty } b _ { j } 2 ^ { - j } } \end{array}$ for some $b _ { j } \in \{ 0 , 1 \}$ , and $f ( x ) : = 0$ otherwise. We thus see that f takes values in C, and is bijective on the set A of non-terminating decimals in [0, 1]. Using Lemma 1.3.9, it is not dificult to show that $f$ is measurable. On the other hand, by modifying the construction from the previous notes, we can find a subset $F$ of A which is non-measurable. If we set $E : = f ( F )$ , then $E$ is a subset of the null set $C$ and is thus itself a null set; but $f ^ { - 1 } ( E ) = F$ is non-measurable, and so the inverse image of a Lebesgue measurable set by a measurable function need not remain Lebesgue measurable. 

However, we will later see that it is still true that $f ^ { - 1 } ( E )$ is Lebesgue measurable if E has a slightly stronger measurability property than Lebesgue measurability, namely Borel measurability; see Exercise 1.4.29(iii). 

Now we can define the concept of a complex-valued measurable function. As discussed earlier, it will be convenient to allow for such functions to only be defined almost everywhere, rather than everywhere, to allow for the possibility that the function becomes singular or otherwise undefined on a null set. 

Definition 1.3.11 (Complex measurability). An almost everywhere defined complex-valued function $f : \mathbf { R } ^ { d }  \mathbf { C }$ is Lebesgue measurable, or measurable for short, if it is the pointwise almost everywhere limit of complex-valued simple functions. 

As before, there are several equivalent definitions: 

Exercise 1.3.7. Let $f : \mathbf { R } ^ { d }  \mathbf { C }$ be an almost everywhere defined complex-valued function. Then the following are equivalent: 

(i) f is measurable. 

(ii) f is the pointwise almost everywhere limit of complex-valued simple functions. 

(iii) The (magnitudes of the) positive and negative parts of $\operatorname { R e } ( f )$ and Im(f) are unsigned measurable functions. 

(iv) $f ^ { - 1 } ( U )$ is Lebesgue measurable for every open set $U \subset \mathbf { C }$ 

(v) $f ^ { - 1 } ( K )$ is Lebesgue measurable for every closed se $K \subset \mathbf { C }$ 

From the above exercise, we see that the notion of complex-valued measurability and unsigned measurability are compatible when applied to a function that takes values in $[ 0 , + \infty ) = [ 0 , + \infty ] \cap \mathbf { C }$ everywhere (or almost everywhere). 

Exercise 1.3.8. 

(i) Show that every continuous function $f : \mathbf { R } ^ { d }  \mathbf { C }$ is measurable. 

(ii) Show that a function $f : \mathbf { R } ^ { d }  \mathbf { C }$ is simple if and only if it is measurable and takes on at most finitely many values. 

(iii) Show that a complex-valued function that is equal almost everywhere to an measurable function, is itself measurable. 

(iv) Show that if a sequence $f _ { n }$ of complex-valued measurable functions converges pointwise almost everywhere to an complex valued limit $f$ , then $f$ is also measurable. 

(v) If $f : \mathbf { R } ^ { d }  \mathbf { C }$ is measurable and $\phi : \mathbf { C }  \mathbf { C }$ is continuous, show that $\phi \circ f : \mathbf { R } ^ { d } \to \mathbf { C }$ is measurable. 

(vi) If $f , g$ are measurable functions, show that $f + g$ and $f g$ are measurable. 

Exercise 1.3.9. Let $f : [ a , b ]  \mathbf { R }$ be a Riemann integrable function. Show that if one extends f to all of R by defining $f ( x ) = 0$ for $x \notin [ a , b ]$ , then $f$ is measurable. 

1.3.3. Unsigned Lebesgue integrals. We are now ready to integrate unsigned measurable functions. We begin with the notion of the lower unsigned Lebesgue integral, which can be defined for arbitrary unsigned functions (not necessarily measurable): 

Definition 1.3.12 (Lower unsigned Lebesgue integral). Let $f : \mathbf { R } ^ { d } $ $[ 0 , + \infty ]$ be an unsigned function (not necessarily measurable). We define the lower unsigned Lebesgue integral $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx to be the quantity 

$$
\underline {{\int_ {\mathbf {R} ^ {d}} f (x) d x : = \sup _ {0 \leq g \leq f ; g \text { simple }} \operatorname{Simp} \int_ {\mathbf {R} ^ {d}} g (x) d x}}
$$

where $g$ ranges over all unsigned simple functions $g : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ that are pointwise bounded by $f$ 

One can also define the upper unsigned Lebesgue integral 

$$
\overline {{\int_ {\mathbf {R} ^ {d}} f (x) d x : = \inf _ {h \geq f ; h \text { simple }} \operatorname{Simp} \int_ {\mathbf {R} ^ {d}} h (x) d x}}
$$

but we will use this integral much more rarely. Note that both integrals take values in $[ 0 , + \infty ]$ , and that the upper Lebesgue integral is always at least as large as the lower Lebesgue integral. 

In the definition of the lower unsigned Lebesgue integral, g is required to be bounded by $f$ pointwise everywhere, but it is easy to see that one could also require g to just be bounded by f pointwise almost everywhere without afecting the value of the integral, since the simple integral is not afected by modifications on sets of measure zero. 

The following properties of the lower Lebesgue integral are easy to establish: 

Exercise 1.3.10 (Basic properties of the lower Lebesgue integral). Let $f , g : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ be unsigned functions (not necessarily measurable). 

(i) (Compatibility with the simple integral) If f is simple, then $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } f ( x ) \ d x = \overline { { \int _ { \mathbf { R } ^ { d } } } } f ( x ) \ d x = \mathrm { S i m p } \int _ { \mathbf { R } ^ { d } } f ( x ) \ d x . } \end{array}$ 

(ii) (Monotonicity) If $f \leq g$ pointwise almost everywhere, then $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } f ( x ) \ d x \leq \int _ { \mathbf { R } ^ { d } } g ( x ) } \end{array}$ dx and $\begin{array} { r } { \overline { { \int _ { \mathbf { R } ^ { d } } } } f ( x ) \ d x \leq \overline { { \int _ { \mathbf { R } ^ { d } } } } g ( x ) } \end{array}$ dx. 

(iii) (Homogeneity) If $c \in [ 0 , + \infty )$ ), then $\textstyle \int _ { \mathbf { R } ^ { d } } c f ( x ) d x = c \int _ { \mathbf { R } ^ { d } } f ( x ) d x$ (The claim unfortunately fails for $c = + \infty$ , but this is somewhat tricky to show.) 

(iv) (Equivalence) If $f , g$ agree almost everywhere, then $\textstyle \int _ { \mathbf { R } ^ { d } } f ( x ) d x =$ $\int _ { \mathbf { R } ^ { d } } g ( x )$ dx and $\begin{array} { r } { \overline { { \int _ { \mathbf { R } ^ { d } } } } f ( x ) \ d x = \overline { { \int _ { \mathbf { R } ^ { d } } } } g ( x ) } \end{array}$ dx. 

(v) (Superadditivity) $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } f ( x ) + g ( x ) d x \geq \int _ { \mathbf { R } ^ { d } } f ( x ) d x + \int _ { \mathbf { R } ^ { d } } g ( x ) d x . } \end{array}$ 

(vi) (Subadditivity of upper integral) $\begin{array} { r } { \overline { { \int _ { \mathbf { R } ^ { d } } } } f ( x ) + g ( x ) d x \leq \overline { { \int _ { \mathbf { R } ^ { d } } } } f ( x ) d x + } \end{array}$ $\overline { { \int _ { \mathbf { R } ^ { d } } } } g ( x )$ dx 

(vii) (Divisibility) For any measurable set E, one has $\textstyle \int _ { \mathbf { R } ^ { d } } f ( x ) d x =$ $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } f ( x ) 1 _ { E } ( x ) \ d x + \int _ { \mathbf { R } ^ { d } } f ( x ) 1 _ { \mathbf { R } ^ { d } \setminus E } ( x ) \ d x } \end{array}$ 

(viii) (Horizontal truncation) As $n  \infty , \int _ { \mathbf { R } ^ { d } } \operatorname* { m i n } ( f ( x ) , n )$ dx converges to $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx. 

(ix) (Vertical truncation) As $\begin{array} { r } { n  \infty , \int _ { \mathbf { R } ^ { d } } f ( x ) 1 _ { | x | \leq n } } \end{array}$ dx converges to $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx. Hint: From Exercise 1.2.11 one has $m ( E \cap \{ x : | x | \leq n \} ) \to m ( E )$ for any measurable set E. 

(x) (Reflection) If $f + g$ is a simple function that is bounded with finite measure support (i.e. it is absolutely integrable), then Simp $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } f ( x ) + g ( x ) \ d x = \int _ { \mathbf { R } ^ { d } } f ( x ) \ d x + \overline { { \int _ { \mathbf { R } ^ { d } } } } g ( x ) \ d x } \end{array}$ 

Do the horizontal and vertical truncation properties hold if the lower Lebesgue integral is replaced with the upper Lebesgue integral? 

Now we restrict attention to measurable functions. 

Definition 1.3.13 (Unsigned Lebesgue integral). If $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ is measurable, we define the unsigned Lebesgue integra $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx of f to equal the lower unsigned Lebesgue integral $\textstyle \int _ { \mathbf { R } ^ { d } } f ( { \widehat { x } } )$ dx. (For non-measurable functions, we leave the unsigned Lebesgue integral undefined.) 

One nice feature of measurable functions is that the lower and upper Lebesgue integrals can match, if one also assumes some boundedness: 

Exercise 1.3.11. Let $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ be measurable, bounded, and vanishing outside of a set of finite measure. Show that the lower and upper Lebesgue integrals of f agree. (Hint: use Exercise 1.3.4.) There is a converse to this statement, but we will defer it to later notes. What happens if f is allowed to be unbounded, or is not supported inside a set of finite measure? 

This gives an important corollary: 

Corollary 1.3.14 (Finite additivity of the Lebesgue integral). Let $f , g : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ be measurable. Then $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } f ( x ) + g ( x ) \ d x \ = } \end{array}$ $\textstyle \int _ { \mathbf { R } ^ { d } } f ( x ) \ d x + \int _ { \mathbf { R } ^ { d } } g ( x )$ dx. 

Proof. From the horizontal truncation property and a limiting argument, we may assume that $f , g$ are bounded. From the vertical truncation property and another limiting argument, we may assume that $f , g$ are supported inside a bounded set. From Exercise 1.3.11, we now see that the lower and upper Lebesgue integrals of $f , g .$ , and $f + g \mathrm { a g r e e }$ . The claim now follows by combining the superadditivity of the lower Lebesgue integral with the subadditivity of the upper Lebesgue integral.  

In the next section we will improve this finite additivity property for the unsigned Lebesgue integral further, to countable additivity; 

this property is also known as the monotone convergence theorem (Theorem 1.4.44). 

Exercise 1.3.12 (Upper Lebesgue integral and outer Lebesgue measure). Show that for any set $E \subset { \bf R } ^ { d } , \overline { { \int _ { \mathbf { R } ^ { d } } } } 1 _ { E } ( x ) \ d x = m ^ { * } ( E )$ . Conclude that the upper and lower Lebesgue integrals are not necessarily additive if no measurability hypotheses are assumed. 

Exercise 1.3.13 (Area interpretation of integral). If $f : \mathbf { R } ^ { d } \ $ $[ 0 , + \infty ]$ is measurable, show that $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx is equal to the $d + 1 -$ dimensional Lebesgue measure of the region $\{ ( x , t ) \in \mathbf { R } ^ { d } \times \mathbf { R } : 0 \leq$ $t \leq f ( x ) \}$ . (This can be used as an alternate, and more geometrically intuitive, definition of the unsigned Lebesgue integral; it is a more convenient formulation for establishing the basic convergence theorems, but not quite as convenient for establishing basic properties such as additivity.) (Hint: use Exercise 1.2.22.) 

Exercise 1.3.14 (Uniqueness of the Lebesgue integral). Show that the Lebesgue integral $f \mapsto \int _ { \mathbf { R } ^ { d } } f ( x )$ dx is the only map from measurable unsigned functions $f : \bar { \bf R } ^ { d }  [ 0 , + \infty ] \ \mathrm { t o } \ [ 0 , + \infty ]$ that obeys the following properties for measurable $f , g : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ 

(i) (Compatibility with the simple integral) If f is simple, then $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } f ( x ) \ d x = \operatorname { S i m p } \int _ { \mathbf { R } ^ { d } } f ( x ) \ d x . } \end{array}$ 

(ii) (Finite additivity) $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } f ( x ) + g ( x ) \ d x \ = \ \int _ { \mathbf { R } ^ { d } } f ( x ) \ d x \ + } \end{array}$ $\int _ { \mathbf { R } ^ { d } } g ( x ) \ d x .$ 

(iii) (Horizontal truncation) As $n  \infty , \int _ { \mathbf { R } ^ { d } } \operatorname* { m i n } ( f ( x ) , n )$ dx converges to $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx. 

(iv) (Vertical truncation) As $\begin{array} { r } { n  \infty , \int _ { \mathbf { R } ^ { d } } f ( x ) 1 _ { | x | \leq n } } \end{array}$ dx converges to $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx. 

Exercise 1.3.15 (Translation invariance). Let $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ be measurable. Show that $\textstyle \int _ { \mathbf { R } ^ { d } } f ( x + y ) d x = \int _ { \mathbf { R } ^ { d } } f ( x )$ dx for any $\boldsymbol { y } \in \mathbf { R } ^ { d }$ 

Exercise 1.3.16 (Linear change of variables). Let $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ be measurable, and let $T : \mathbf { R } ^ { d }  \mathbf { R } ^ { d }$ be an invertible linear transformation. Show that $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } f ( T ^ { - 1 } ( x ) ) \ d x \ = \ | \operatorname* { d e t } T | \int _ { \mathbf { R } ^ { d } } f ( x ) \ } \end{array}$ dx, or equivalently $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } f ( T x ) \ \overleftarrow { d x } = \frac { 1 } { \mid \operatorname* { d e t } T \mid } \int _ { \mathbf { R } ^ { d } } f ( x ) } \end{array}$ dx. 

Exercise 1.3.17 (Compatibility with the Riemann integral). Let $f : [ a , b ]  [ 0 , + \infty ]$ be Riemann integrable. If we extend $f$ to R by declaring $f$ to equal zero outside of $[ a , b ]$ , show that $\textstyle \int _ { \mathbf { R } } f ( x ) \ d x \ =$ $\textstyle \int _ { a } ^ { b } f ( x )$ dx. 

We record a basic inequality, known as Markov’s inequality, that asserts that the Lebesgue integral of an unsigned measurable function controls how often that function can be large: 

Lemma 1.3.15 (Markov’s inequality). Let $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ be measurable. Then for any $0 < \lambda < \infty$ , one has 

$$
m (\{x \in \mathbf {R} ^ {d}: f (x) \geq \lambda \}) \leq \frac {1}{\lambda} \int_ {\mathbf {R} ^ {d}} f (x) d x.
$$

Proof. We have the trivial pointwise inequality 

$$
\lambda 1 _ {\{x \in \mathbf {R} ^ {d}: f (x) \geq \lambda \}} \leq f (x).
$$

From the definition of the lower Lebesgue integral, we conclude that 

$$
\lambda m (\{x \in \mathbf {R} ^ {d}: f (x) \geq \lambda \}) \leq \int_ {\mathbf {R} ^ {d}} f (x) d x
$$

and the claim follows. 

By sending λ to infinity or to zero, we obtain the following important corollary: 

Exercise 1.3.18. Let $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ be measurable. 

(i) Show that if $\textstyle \int _ { \mathbf { R } ^ { d } } f ( x ) \ d x < \infty$ , then f is finite almost everywhere. Give a counterexample to show that the converse statement is false. 

(ii) Show that $\textstyle \int _ { \mathbf { R } ^ { d } } f ( x ) \ d x = 0$ if and only if f is zero almost everywhere. 

Remark 1.3.16. The use of the integral $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx to control the distribution of $f$ is known as the first moment method. One can also control this distribution using higher moments such as $\int _ { \mathbf { R } ^ { d } } | f ( x ) | ^ { p }$ dx for various values of $p ,$ , or exponential moments such as $\int _ { \mathbf { R } ^ { d } } e ^ { t f ( x ) }$ dx or the Fourier moments $\int _ { \mathbf { R } ^ { d } } e ^ { i t f ( x ) }$ $d x$ for various values of $t ;$ such moment methods are fundamental to probability theory. 

1.3.4. Absolute integrability. Having set out the theory of the unsigned Lebesgue integral, we can now define the absolutely convergent Lebesgue integral. 

Definition 1.3.17 (Absolute integrability). An almost everywhere defined measurable function $f : \mathbf { R } ^ { d }  \mathbf { C }$ is said to be absolutely integrable if the unsigned integra 

$$
\| f \| _ {L ^ {1} (\mathbf {R} ^ {d})} := \int_ {\mathbf {R} ^ {d}} | f (x) | d x
$$

is finite. We refer to this quantity $\| f \| _ { L ^ { 1 } ( \mathbf { R } ^ { d } ) }$ as the $L ^ { 1 } ( \mathbf R ^ { d } )$ norm of $f ,$ and use $L ^ { 1 } ( \mathbf R ^ { d } )$ or $L ^ { 1 } ( \mathbf { R } ^ { d }  \mathbf { C } )$ to denote the space of absolutely integrable functions. If $f$ is real-valued and absolutely integrable, we define the Lebesgue integral $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx by the formula 

$$
\int_ {\mathbf {R} ^ {d}} f (x) d x := \int_ {\mathbf {R} ^ {d}} f _ {+} (x) d x - \int_ {\mathbf {R} ^ {d}} f _ {-} (x) d x\tag{1.12}
$$

where $f _ { + } : = \operatorname* { m a x } ( f , 0 ) , f _ { - } : = \operatorname* { m a x } ( - f , 0 )$ are the magnitudes of the positive and negative components of $f$ (note that the two unsigned integrals on the right-hand side are finite, as $f _ { + } , f _ { - }$ are pointwise dominated by $| f | )$ . If $f$ is complex-valued and absolutely integrable, we define the Lebesgue integral $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx by the formula 

$$
\int_ {\mathbf {R} ^ {d}} f (x) d x := \int_ {\mathbf {R} ^ {d}} \mathrm{Re} f (x) d x + i \int_ {\mathbf {R} ^ {d}} \mathrm{Im} f (x) d x
$$

where the two integrals on the right are interpreted as real-valued absolutely integrable Lebesgue integrals. It is easy to see that the unsigned, real-valued, and complex-valued Lebesgue integrals defined in this manner are compatible on their common domains of definition. 

Note from construction that the absolutely integrable Lebesgue integral extends the absolutely integrable simple integral, which is now redundant and will not be needed any further in the sequel. 

Remark 1.3.18. One can attempt to define integrals for non-absolutely integrable functions, analogous to the improper integrals $\textstyle \int _ { 0 } ^ { \infty } f ( x ) d x : =$ lim $\begin{array} { r } { { \cal R } \to \infty \int _ { 0 } ^ { R } f ( x ) } \end{array}$ dx or the principal value integrals $\textstyle p . v . \int _ { - \infty } ^ { \infty } f ( x ) d x : =$ lim $\scriptstyle { R \to \infty } \int _ { - R } ^ { R } f ( x )$ dx one sees in the classical one-dimensional Riemannian theory. While one can certainly generate any number of such extensions of the Lebesgue integral concept, such extensions tend 

to be poorly behaved with respect to various important operations, such as change of variables or exchanging limits and integrals, so it is usually not worthwhile to try to set up a systematic theory for such non-absolutely-integrable integrals that is anywhere near as complete as the absolutely integrable theory, and instead deal with such exotic integrals on an ad hoc basis. 

From the pointwise triangle inequality $| f ( x ) + g ( x ) | \leq | f ( x ) | +$ $| g ( x ) |$ |, we conclude the $L ^ { 1 }$ triangle inequality 

$$
\| f + g \| _ {L ^ {1} (\mathbf {R} ^ {d})} \leq \| f \| _ {L ^ {1} (\mathbf {R} ^ {d})} + \| g \| _ {L ^ {1} (\mathbf {R} ^ {d})}\tag{1.13}
$$

for any almost everywhere defined measurable $f , g : \mathbf { R } ^ { d }  \mathbf { C }$ . It is also easy to see that 

$$
\left\| c f \right\| _ {L ^ {1} (\mathbf {R} ^ {d})} = | c | \| f \| _ {L ^ {1} (\mathbf {R} ^ {d})}
$$

for any complex number c. As such, we see that $L ^ { 1 } ( \mathbf { R } ^ { d }  \mathbf { C } )$ is a complex vector space. (The $L ^ { 1 }$ norm is then a seminorm on this space; see §1.3 of An epsilon of room, Vol. I.) From Exercise 1.3.18 we make the important observation that a function $f \in L ^ { 1 } ( \mathbf { R } ^ { d } \to \mathbf { C } )$ has zero $L ^ { 1 }$ norm, $\| f \| _ { L ^ { 1 } ( \mathbf { R } ^ { d } ) } = 0$ , if and only if f is zero almost everywhere. 

Given two functions $f , g \in L ^ { 1 } ( \mathbf { R } ^ { d }  \mathbf { C } )$ , we can define the $L ^ { 1 }$ distance $d _ { L ^ { 1 } } ( f , g )$ between them by the formula 

$$
d _ {L ^ {1}} (f, g) := \| f - g \| _ {L ^ {1} \left(\mathbf {R} ^ {d}\right)}.
$$

Thanks to (1.13), this distance obeys almost all the axioms of a metric on $L ^ { 1 } ( \mathbf R ^ { d } )$ , with one exception: it is possible for two diferent functions $f , g \in L ^ { 1 } ( \mathbf { R } ^ { d }  \mathbf { C } )$ to have a zero $L ^ { 1 }$ distance, if they agree almost everywhere. As such, $d _ { L ^ { 1 } }$ is only a semi-metric (also known as a pseudo-metric) rather than a metric. However, if one adopts the convention that any two functions that agree almost everywhere are considered equivalent (or more formally, one works in the quotient space of $L ^ { 1 } ( \mathbf R ^ { d } )$ by the equivalence relation of almost everywhere agreement, which by abuse of notation is also denoted $L ^ { 1 } ( \mathbf R ^ { d } ) )$ ), then one recovers a genuine metric. (Later on, we will establish the important fact that this metric makes the (quotient space) $L ^ { 1 } ( \mathbf R ^ { d } )$ a complete metric space, a fact known as the $L ^ { 1 }$ Riesz-Fischer theorem; this completeness is one of the main reasons we spend so much efort setting up Lebesgue integration theory in the first place.) 

The linearity properties of the unsigned integral induce analogous linearity properties of the absolutely convergent Lebesgue integral: 

Exercise 1.3.19 (Integration is linear). Show that integration $f \mapsto$ $\int _ { \mathbf { R } ^ { d } } f ( x )$ dx is a (complex) linear operation from $L ^ { 1 } ( \mathbf R ^ { d } )$ to C. In other words, show that 

$$
\int_ {\mathbf {R} ^ {d}} f (x) + g (x) d x = \int_ {\mathbf {R} ^ {d}} f (x) d x + \int_ {\mathbf {R} ^ {d}} g (x) d x
$$

and 

$$
\int_ {\mathbf {R} ^ {d}} c f (x) d x = c \int_ {\mathbf {R} ^ {d}} f (x) d x
$$

for all absolutely integrable $f , g : \mathbf { R } ^ { d }  \mathbf { C }$ and complex numbers c. Also establish the identity 

$$
\int_ {\mathbf {R} ^ {d}} \overline {{f (x)}} d x = \overline {{\int_ {\mathbf {R} ^ {d}} f (x) d x}},
$$

which makes integration not just a linear operation, but a *-linear operation. 

Exercise 1.3.20. Show that Exercises 1.3.15, 1.3.16, and 1.3.17 also hold for complex-valued, absolutely integrable functions rather than for unsigned measurable functions. 

Exercise 1.3.21 (Absolute summability is a special case of absolute integrability). Let $( c _ { n } ) _ { n \in \mathbf { Z } }$ be a doubly infinite sequence of complex numbers, and let $f : \mathbf { R }  \mathbf { C }$ be the function 

$$
f (x) := \sum_ {n \in \mathbf {Z}} c _ {n} 1 _ {[ n, n + 1)} (x) = c _ {\lfloor x \rfloor}
$$

where $\lfloor x \rfloor$ is the greatest integer less than x. Show that $f$ is absolutely integrable if and only if the series $\sum { _ { n \in \mathbf { Z } } c _ { n } }$ is absolutely convergent, in which case one has $\textstyle \int _ { \mathbf { R } } f ( x ) \ d x = \sum _ { n \in \mathbf { Z } } c _ { n }$ 

We can localise the absolutely convergent integral to any measurable subset $E$ of $\mathbf { R } ^ { d }$ . Indeed, if $f : E \to \mathbf { C }$ is a function, we say that $f$ is measurable (resp. absolutely integrable) if its extension $\tilde { f } : \mathbf { R } ^ { d }  \mathbf { C }$ is measurable (resp. absolutely integrable), where $\tilde { f } ( x )$ is defined to equal $f ( x )$ when $x \in E$ and zero otherwise, and then we define $\textstyle \int _ { E } f ( x )$ dx $\begin{array} { r } { \mathbf { \tilde { \mathbf { \rho } } } : = \int _ { \mathbf { R } ^ { d } } \tilde { f } ( x ) } \end{array}$ dx. Thus, for instance, the absolutely integrable analogue of Exercise 1.3.17 tells us that 

$$
\int_ {a} ^ {b} f (x) d x = \int_ {[ a, b ]} f (x) d x
$$

for any Riemann-integrable $f : [ a , b ]  \mathbf { C }$ 

Exercise 1.3.22. If E, F are disjoint measurable subsets of $\mathbf { R } ^ { d }$ , and $f : E \cup F  \mathbf { C }$ is absolutely integrable, show that 

$$
\int_ {E} f (x) d x = \int_ {E \cup F} f (x) 1 _ {E} (x) d x
$$

and 

$$
\int_ {E} f (x) d x + \int_ {F} f (x) d x = \int_ {E \cup F} f (x) d x.
$$

We will study the properties of the absolutely convergent Lebesgue integral in more detail in later notes, as a special case of the more general Lebesgue integration theory on abstract measure spaces. For now, we record one very basic inequality: 

Lemma 1.3.19 (Triangle inequality). Let $f \in L ^ { 1 } ( \mathbf { R } ^ { d } \to \mathbf { C } )$ . Then 

$$
| \int_ {\mathbf {R} ^ {d}} f (x) d x | \leq \int_ {\mathbf {R} ^ {d}} | f (x) | d x.
$$

Proof. If f is real-valued, then $| f | = f _ { + } + f _ { - }$ and the claim is obvious from (1.12). When $f$ is complex-valued, one cannot argue quite so simply; a naive mimicking of the real-valued argument would lose a factor of 2, giving the inferior bound 

$$
\left| \int_ {\mathbf {R} ^ {d}} f (x) d x \right| \leq 2 \int_ {\mathbf {R} ^ {d}} | f (x) | d x.
$$

To do better, we exploit the phase rotation invariance properties of the absolute value operation and of the integral, as follows. Note that for any complex number $z ,$ one can write $| z |$ as $z e ^ { i \theta }$ for some real $\theta .$ In particular, we have 

$$
| \int_ {\mathbf {R} ^ {d}} f (x) d x | = e ^ {i \theta} \int_ {\mathbf {R} ^ {d}} f (x) d x = \int_ {\mathbf {R} ^ {d}} e ^ {i \theta} f (x) d x
$$

for some real θ. Taking real parts of both sides, we obtain 

$$
| \int_ {\mathbf {R} ^ {d}} f (x) d x | = \int_ {\mathbf {R} ^ {d}} \mathrm{Re} (e ^ {i \theta} f (x)) d x.
$$

Since $\operatorname { R e } ( e ^ { i \theta } f ( x ) ) \leq | e ^ { i \theta } f ( x ) | = | f ( x ) |$ , we obtain the claim. 

1.3.5. Littlewood’s three principles. Littlewood’s three principles are informal heuristics that convey much of the basic intuition behind the measure theory of Lebesgue. Briefly, the three principles are as follows: 

(i) Every (measurable) set is nearly a finite sum of intervals; 

(ii) Every (absolutely integrable) function is nearly continuous; and 

(iii) Every (pointwise) convergent sequence of functions is nearly uniformly convergent. 

Various manifestations of the first principle were given in Exercise 1.2.7 and Exercise 1.2.16. Now we turn to the second principle. Define a step function to be a finite linear combination of indicator functions $1 _ { B }$ of boxes B. 

Theorem 1.3.20 (Approximation of $L ^ { 1 }$ functions). Let $f \in L ^ { 1 } ( \mathbf R ^ { d } )$ and $\varepsilon > 0$ 

(i) There exists an absolutely integrable simple function g such that $\| f - g \| _ { L ^ { 1 } ( \mathbf R ^ { d } ) } \leq \varepsilon$ 

(ii) There exists a step function g such that $\| f - g \| _ { L ^ { 1 } ( \mathbf R ^ { d } ) } \leq \varepsilon$ 

(iii) There exists a continuous, compactly supported g such that $| f - g \| _ { L ^ { 1 } ( \mathbf { R } ^ { d } ) } \leq \varepsilon$ 

To put things another way, the absolutely integrable simple functions, the step functions, and the continuous, compactly supported functions are all dense subsets of $L ^ { 1 } ( \mathbf R ^ { d } )$ with respect to the $L ^ { 1 } ( \mathbf R ^ { d } )$ (semi-)metric. In §1.13 of An epsilon of room, Vol. I it is shown that a similar statement holds if one replaces continuous, compactly supported functions with smooth, compactly supported functions, also known as test functions; this is an important fact for the theory of distributions. 

Proof. We begin with part (i). When $f$ is unsigned, we see from the definition of the lower Lebesgue integral that there exists an unsigned simple function $g$ such that $g \leq f$ (so, in particular, $g$ is absolutely integrable) and 

$$
\int_ {\mathbf {R} ^ {d}} g (x) d x \geq \int_ {\mathbf {R} ^ {d}} f (x) d x - \varepsilon ,
$$

which by linearity implies that $\| f - g \| _ { L ^ { 1 } ( \mathbf { R } ^ { d } ) } \leq \varepsilon$ . This gives (i) when $f$ is unsigned. The case when $f$ is real-valued then follows by splitting $f$ into positive and negative parts (and adjusting ε as necessary), and the case when $f$ is complex-valued then follows by splitting $f$ into real and imaginary parts (and adjusting ε yet again). 

To establish part (ii), we see from (i) and the triangle inequality in $L ^ { 1 }$ that it sufices to show this when $f$ is an absolutely integrable simple function. By linearity (and more applications of the triangle inequality), it then sufices to show this when $f = 1 _ { E }$ is the indicator function of a measurable set $E \subset \mathbf { R } ^ { d }$ of finite measure. But then, by Exercise (1.2.16), such a set can be approximated (up to an error of measure at most $\varepsilon )$ by an elementary set, and the claim follows. 

To establish part (iii), we see from (ii) and the argument from the preceding paragraph that it sufices to show this when $f = 1 _ { E }$ is the indicator function of a box. But one can then establish the claim by direct construction. Indeed, if one makes a slightly larger box $F$ that contains the closure of $E$ in its interior, but has a volume at most $\varepsilon$ more than that of $E _ { : }$ , then one can directly construct a piecewise linear continuous function $g$ supported on $F$ that equals 1 on $E$ (e.g. one can set $g ( x ) = \mathrm { m a x } ( 1 - R \mathrm { d i s t } ( x , E ) , 0 )$ for some suficiently large $R ;$ one may also invoke Urysohn’s lemma, see §1.10 of An epsilon of room, Vol. I). It is then clear from construction that $\| f - g \| _ { L ^ { 1 } ( \mathbf R ^ { d } ) } \leq \varepsilon$ as required.  

This is not the only way to make Littlewood’s second principle manifest; we return to this point shortly. For now, we turn to Littlewood’s third principle. We recall three basic ways in which a sequence $f _ { n } : \mathbf { R } ^ { d }  \mathbf { C }$ of functions can converge to a limit $f : \mathbf { R } ^ { d }  \mathbf { C }$ 

(i) (Pointwise convergence) $f _ { n } ( x )  f ( x )$ for every $\boldsymbol { x } \in \mathbf { R } ^ { d }$ (ii) (Pointwise almost everywhere convergence) $f _ { n } ( x ) \to f ( x )$ for almost every $x \in \mathbf { R } ^ { d }$ 

(iii) (Uniform convergence) For every $\varepsilon > 0$ , there exists N such that $| f _ { n } ( x ) - f ( x ) | \leq \varepsilon$ for all $n \geq N$ and all $x \in \mathbf { R } ^ { d }$ 

Uniform convergence implies pointwise convergence, which in turn implies pointwise almost everywhere convergence. 

We now add a fourth mode of convergence, that is weaker than uniform convergence but stronger than pointwise convergence: 

Definition 1.3.21 (Locally uniform convergence). A sequence of functions $f _ { n } : \mathbf { R } ^ { d }  \mathbf { C }$ converges locally uniformly to a limit $f :$ $\mathbf { R } ^ { d }  \mathbf { C } \mathrm { ~ i f } .$ for every bounded subset $E$ of $\mathbf { R } ^ { d } , \mathbf { \Gamma } f _ { n }$ converges uniformly to f on E. In other words, for every bounded $E \subset \mathbf { R } ^ { d }$ and every $\varepsilon > 0$ , there exists $N > 0$ such that $| f _ { n } ( x ) - f ( x ) | \leq \varepsilon$ for all $n \geq N$ and $x \in E$ 

Remark 1.3.22. At least as far as $\mathbf { R } ^ { d }$ is concerned, an equivalent definition of local uniform convergence is: $f _ { n }$ converges locally uniformly to f if, for every point $\boldsymbol { x } _ { 0 } \in \mathbf { R } ^ { d }$ , there exists an open neighbourhood $U$ of $x _ { 0 }$ such that $f _ { n }$ converges uniformly to $f$ on U. The equivalence of the two definitions is immediate from the Heine-Borel theorem. More generally, the adverb “locally” in mathematics is usually used in this fashion; a propery $P$ is said to hold locally on some domain X if, for every point $x _ { 0 }$ in that domain, there is an open neighbourhood of $x _ { 0 }$ in $X$ on which $P$ holds. 

One should caution, though, that on domains on which the Heine-Borel theorem does not hold, the bounded-set notion of local uniform convergence is not equivalent to the open-set notion of local uniform convergence (though, for locally compact spaces, one can recover equivalence of one replaces “bounded” by “compact”). 

Example 1.3.23. The functions $x \mapsto x / n$ on R for $n = 1 , 2 , \ldots$ converge locally uniformly (and hence pointwise) to zero on R, but do not converge uniformly. 

Example 1.3.24. The partial sums $\textstyle \sum _ { n = 0 } ^ { N } { \frac { x ^ { n } } { n ! } }$ of the Taylor series $\textstyle e ^ { x } = \sum _ { n = 0 } ^ { \infty } { \frac { x ^ { n } } { n ! } }$ converges to $e ^ { x }$ locally uniformly (and hence pointwise) on R, but not uniformly. 

Example 1.3.25. The functions $\textstyle f _ { n } ( x ) : = { \frac { 1 } { n x } } 1 _ { x > 0 }$ for $n = 1 , 2 , \ldots$ (with the convention that $f _ { n } ( 0 ) = 0 )$ converge pointwise everywhere to zero, but do not converge locally uniformly. 

From the preceding example, we see that pointwise convergence (either everywhere or almost everywhere) is a weaker concept than local uniform convergence. Nevertheless, a remarkable theorem of Egorov, which demonstrates Littlewood’s third principle, asserts that one can recover local uniform convergence as long as one is willing to delete a set of small measure: 

Theorem 1.3.26 (Egorov’s theorem). Let $f _ { n } : \mathbf { R } ^ { d }  \mathbf { C }$ be a sequence of measurable functions that converge pointwise almost everywhere to another function $f : \mathbf { R } ^ { d }  \mathbf { C }$ , and let $\varepsilon > 0$ . Then there exists a Lebesgue measurable set A of measure at most $\varepsilon ,$ such that $f _ { n }$ converges locally uniformly to f outside of A. 

Note that Example 1.3.25 demonstrates that the exceptional set A in Egorov’s theorem cannot be taken to have zero measure, at least if one uses the bounded-set definition of local uniform convergence from Definition 1.3.21. (If one instead takes the “open neighbourhood” definition, then the sequence in Example 1.3.25 does converge locally uniformly on $\mathbf { R } \backslash \{ 0 \}$ in the open neighbourhood sense, even if it does not do so in the bounded-set sense. On a domain such as $\mathbf { R } ^ { d } \backslash A$ , bounded-set locally uniform convergence implies open-neighbourhood locally uniform convergence, but not conversely, so for the purposes of applying Egorov’s theorem, the distinction is not too important since one local uniform convergence in both senses.) 

Proof. By modifying $f _ { n }$ and f on a set of measure zero (that can be absorbed into A at the end of the argument) we may assume that $f _ { n }$ converges pointwise everywhere to f, thus for every $x \in \mathbf { R } ^ { d }$ and $m > 0$ there exists $N \geq 0$ such that $| f _ { n } ( x ) - f ( x ) | \leq 1 / m$ for all $n \geq N$ . We can rewrite this fact set-theoretically as 

$$
\bigcap_ {N = 0} ^ {\infty} E _ {N, m} = \emptyset
$$

for each $m ,$ , where 

$$
E _ {N, m} := \{x \in \mathbf {R} ^ {d}: | f _ {n} (x) - f (x) | > 1 / m \text {   for   some   } n \geq N \}
$$

It is clear that the $E _ { N , m }$ are Lebesgue measurable, and are decreasing in N. Applying downward monotone convergence (Exercise 1.2.11(ii)) we conclude that, for any radius $R > 0$ , one has 

$$
\lim _ {N \to \infty} m (E _ {N, m} \cap B (0, R)) = 0.
$$

(The restriction to the ball $B ( 0 , R )$ is necessary, because the downward monotone convergence property only works when the sets involved have finite measure.) In particular, for any $m \geq 1$ , we can find $N _ { m }$ such that 

$$
m (E _ {N, m} \cap B (0, m)) \leq \frac {\varepsilon}{2 ^ {m}}
$$

for all $N \geq N _ { m }$ 

Now let $\begin{array} { r } { A : = \bigcup _ { m = 1 } ^ { \infty } E _ { N _ { m } , m } \cap B ( 0 , m ) } \end{array}$ . Then A is Lebesgue measurable, and by countable subadditivity, $m ( A ) \leq \varepsilon$ . By construction, we have 

$$
\left| f _ {n} (x) - f (x) \right| \leq 1 / m
$$

whenever $m \geq 1 , \ x \in \mathbf { R } ^ { d } \backslash A , \ | x | \leq m$ , and $n \geq N _ { m }$ . In particular, we see for any ball $B ( 0 , m _ { 0 } )$ with an integer radius, $f _ { n }$ converges uniformly to $f$ on $B ( 0 , m _ { 0 } ) \backslash A$ . Since every bounded set is contained in such a ball, the claim follows.  

Remark 1.3.27. Unfortunately, one cannot in general upgrade local uniform convergence to uniform convergence in Egorov’s theorem. A basic example here is the moving bump example $f _ { n } : = 1 _ { [ n , n + 1 ] }$ on R, which “escapes to horizontal infinity”. This sequence converges pointwise (and locally uniformly) to the zero function $f \equiv 0$ . However, for any $0 < \varepsilon < 1$ and any n, we have $| f _ { n } ( x ) - f ( x ) | > \varepsilon$ on a set of measure 1, namely on the interval $[ n , n + 1 ]$ . Thus, if one wanted $f _ { n }$ to converge uniformly to f outside of a set A, then that set A has to contain a set of measure 1. In fact, it must contain the intervals $[ n , n + 1 ]$ for all suficiently large n and must therefore have infinite measure. 

However, if all the $f _ { n }$ and f were supported on a fixed set E of finite measure (e.g. on a ball $B ( 0 , R ) )$ , then the above “escape to horizontal infinity” cannot occur, it is easy to see from the above argument that one can recover uniform convergence (and not just locally uniform convergence) outside of a set of arbitrarily small measure. 

We now use Theorem 1.3.20 to give another version of Littlewood’s second principle, known as Lusin’s theorem: 

Theorem 1.3.28 (Lusin’s theorem). Let $f : \mathbf { R } ^ { d }  \mathbf { C }$ be absolutely integrable, and let $\varepsilon > 0$ . Then there exists a Lebesgue measurable set $E \subset \mathbf { R } ^ { d }$ of measure at most ε such that the restriction of f to the complementary set $\mathbf { R } ^ { d } \backslash E$ is continuous on that set. 

Caution: this theorem does not imply that the unrestricted function f is continuous on $\mathbf { R } ^ { d } \backslash E$ . For instance, the absolutely integrable function $\mathbf { 1 } _ { \mathbf { Q } } : \mathbf { R }  \mathbf { C }$ is nowhere continuous, so is certainly not continuous on $\mathbf { R } \backslash E$ for any E of finite measure; but on the other hand, if one deletes the measure zero set $E : = \mathbf { Q }$ from the reals, then the restriction of $f$ to $\mathbf { R } \backslash E$ is identically zero and thus continuous. 

Proof. By Theorem 1.3.20, for any $n \geq 1$ one can find a continuous, compactly supported function $f _ { n }$ such that $\| f - f _ { n } \| _ { L ^ { 1 } ( \mathbf { R } ^ { d } ) } \leq \varepsilon / 4 ^ { n }$ (say). By Markov’s inequality (Lemma 1.3.15), that implies that $| f ( x ) - f _ { n } ( x ) | \leq 1 / 2 ^ { n - 1 }$ for all x outside of a Lebesgue measurable set $A _ { n }$ of measure at most $\varepsilon / 2 ^ { n + 1 }$ . Letting $A : = \textstyle \bigcup _ { n = 1 } ^ { \infty } A _ { n }$ , we conclude that A is Lebesgue measurable with measure at most $\varepsilon / 2$ , and $f _ { n }$ converges uniformly to $f$ outside of A. But the uniform limit of continuous functions is continuous, and the same is true for local uniform limits (because continuity is itself a local property). We conclude that the restriction f to $\mathbf { R } ^ { d } \backslash E$ is continuous, as required.  

Exercise 1.3.23. Show that the hypothesis that $f$ is absolutely integrable in Lusin’s theorem can be relaxed to being locally absolutely integrable (i.e. absolutely integrable on every bounded set), and then relaxed further to that of being measurable (but still finite everywhere or almost everywhere). (To achieve the latter goal, one can replace f locally with a horizontal truncation $f 1 _ { | f | \leq n } \colon$ ; alternatively, one can replace f with a bounded variant, such as ${ \frac { f } { ( 1 + | f | ^ { 2 } ) ^ { 1 / 2 } } } . \Big )$ 

Exercise 1.3.24. Show that a function $f : \mathbf { R } ^ { d }  \mathbf { C }$ is measurable if and only if it is the pointwise almost everywhere limit of continuous functions $f _ { n } : \mathbf { R } ^ { d }  \mathbf { C }$ . (Hint: if $f : \mathbf { R } ^ { d }  \mathbf { C }$ is measurable and $n \geq 1$ , show that there exists a continuous function $f _ { n } : \mathbf { R } ^ { d }  \mathbf { C }$ for which the set $\{ x \in B ( 0 , n ) : | f ( x ) - f _ { n } ( x ) | \geq 1 / n \}$ has measure at most $\frac { 1 } { 2 ^ { n } }$ . You may find Exercise 1.3.25 below to be useful for this.) Use this (and Egorov’s theorem, Theorem 1.3.26) to give an alternate proof of Lusin’s theorem for arbitrary measurable functions. 

Remark 1.3.29. This is a trivial but important remark: when dealing with unsigned measurable functions such as $f : \mathbf { R } ^ { d }  [ 0 , + \infty ]$ , then Lusin’s theorem does not apply directly because $f$ could be infinite on a set of positive measure, which is clearly in contradiction with the conclusion of Lusin’s theorem (unless one allows the continuous function to also take values in the extended non-negative reals $[ 0 , + \infty ]$ with the extended topology). However, if one knows already that $f$ is almost everywhere finite (which is for instance the case when $f$ is absolutely integrable), then Lusin’s theorem applies (since one can simply zero out $f$ on the null set where it is infinite, and add that null set to the exceptional set of Lusin’s theorem). 

Remark 1.3.30. By combining Lusin’s theorem with inner regularity (Exercise 1.2.15) and the Tietze extension theorem (see §1.10 of $A n$ epsilon of room, Vol. I), one can conclude that every measurable function $f : \mathbf { R } ^ { d }  \mathbf { C }$ agrees (outside of a set of arbitrarily small measure) with a continuous function $g : \mathbf { R } ^ { d }  \mathbf { C }$ 

Exercise 1.3.25 (Littlewood-like principles). The following facts are not, strictly speaking, instances of any of Littlewood’s three principles, but are in a similar spirit. 

(i) (Absolutely integrable functions almost have bounded support) Let $f : \mathbf { R } ^ { d }  \mathbf { C }$ be an absolutely integrable function, and let $\varepsilon > 0$ . Show that there exists a ball $B ( 0 , R )$ outside of which f has an $L ^ { 1 }$ norm of at most $\varepsilon ,$ or in other words that $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } \backslash B ( 0 , R ) } | f ( x ) | ~ d x \leq \varepsilon } \end{array}$ 

(ii) (Measurable functions are almost locally bounded) Let $f$ : $\mathbf R ^ { d } \to \mathbf C$ be a measurable function supported on a set of finite measure, and let $\varepsilon > 0$ . Show that there exists a measurable set $E \subset \mathbf { R } ^ { d }$ of measure at most $\varepsilon$ outside of which $f$ is locally bounded, or in other words that for every $R > 0$ there exists $M < \infty$ such that $| f ( x ) | \leq M$ for all $x \in B ( 0 , R ) \backslash E$ 

As with Remark 1.3.29, it is important in the second part of the exercise that $f$ is known to be finite everywhere (or at least almost everywhere); the result would of course fail if $f$ was, say, unsigned but took the value +∞ on a set of positive measure. 

## 1.4. Abstract measure spaces

Thus far, we have only focused on measure and integration theory in the context of Euclidean spaces $\mathbf { R } ^ { d }$ . Now, we will work in a more abstract and general setting, in which the Euclidean space $\mathbf { R } ^ { d }$ is replaced by a more general space $X$ . 

It turns out that in order to properly define measure and integration on a general space $X$ , it is not enough to just specify the set $X$ One also needs to specify two additional pieces of data: 

(i) A collection B of subsets of X that one is allowed to measure; and 

(ii) The measure $\mu ( E ) \in [ 0 , + \infty ]$ one assigns to each measurable set $E \in B$ 

For instance, Lebesgue measure theory covers the case when X is a Euclidean space $\mathbf { R } ^ { d }$ , B is the collection $B = \mathcal { L } [ \mathbf { R } ^ { d } ]$ of all Lebesgue measurable subsets of $\mathbf { R } ^ { d }$ , and $\mu ( E )$ is the Lebesgue measure $\mu ( E ) =$ $m ( E )$ of $E$ . 

The collection B has to obey a number of axioms (e.g. being closed with respect to countable unions) that make it a $\sigma { - } a l g e b r a .$ which is a stronger variant of the more well-known concept of a boolean algebra. Similarly, the measure $\mu$ has to obey a number of axioms (most notably, a countable additivity axiom) in order to obtain a measure and integration theory comparable to the Lebesgue theory on Euclidean spaces. When all these axioms are satisfied, the triple $( X , B , \mu )$ is known as a measure space. These play much the same role in abstract measure theory that metric spaces or topological spaces play in abstract point-set topology, or that vector spaces play in abstract linear algebra. 

On any measure space, one can set up the unsigned and absolutely convergent integrals in almost exactly the same way as was done in the previous notes for the Lebesgue integral on Euclidean spaces, although the approximation theorems are largely unavailable at this level of generality due to the lack of such concepts as “elementary set” or “continuous function” for an abstract measure space. On the other hand, one does have the fundamental convergence theorems for the subject, namely Fatou’s lemma, the monotone convergence theorem and the dominated convergence theorem, and we present these results here. 

One question that will not be addressed much in this section is how one actually constructs interesting examples of measures. We will return to this issue in Section 1.7 (although one of the most powerful tools for such constructions, namely the Riesz representation theorem, will not be covered here, but instead in §1.10 of An epsilon of room, Vol. I). 

1.4.1. Boolean algebras. We begin by recalling the concept of a Boolean algebra. 

Definition 1.4.1 (Boolean algebras). Let X be a set. A (concrete) Boolean algebra on X is a collection B of X which obeys the following properties: 

(i) (Empty set) $\varnothing \in B$ 

(ii) (Complement) If $E \in B$ , then the complement $E ^ { c } : = X \backslash E$ also lies in B. 

(iii) (Finite unions) If E, $F \in B$ , then $E \cup F \in B$ 

We sometimes say that E is B-measurable, or measurable with respect to B, if $E \in B$ 

Given two Boolean algebras $B , B ^ { \prime }$ on X, we say that $B ^ { \prime }$ is finer than, a sub-algebra $o f ,$ or a refinement of B, or that B is coarser than or a coarsening of $B ^ { \prime }$ , if $B \subset B ^ { \prime }$ 

We have chosen a “minimalist” definition of a Boolean algebra, in which one is only assumed to be closed under two of the basic Boolean operations, namely complement and finite union. However, by using the laws of Boolean algebra (such as de Morgan’s laws), it is easy to see that a Boolean algebra is also closed under other 

Boolean algebra operations such as intersection $E \cap F$ , set difererence $E \backslash F$ , and symmetric diference $E \Delta F$ . So one could have placed these additional closure properties inside the definition of a Boolean algebra without any loss of generality. However, when we are verifying that a given collection $\boldsymbol { B }$ of sets is indeed a Boolean algebra, it is convenient to have as minimal a set of axioms as possible. 

Remark 1.4.2. One can also consider abstract Boolean algebras $B { \mathrm { . } }$ which do not necessarily live in an ambient domain $X$ , but for which one has a collection of abstract Boolean operations such as meet ∧ and join ∨ instead of the concrete operations of intersection ∩ and union ∪. We will not take this abstract perspective here, but see §2.3 of An epsilon of room, Vol. I for some further discussion of the relationship between concrete and abstract Boolean algebras, which is codified by Stone’s theorem. 

Example 1.4.3 (Trivial and discrete algebra). Given any set $X$ , the coarsest Boolean algebra is the trivial algebra $\{ \emptyset , X \}$ , in which the only measurable sets are the empty set and the whole set. The finest Boolean algebra is the discrete algebra $2 ^ { X } : = \{ E : E \subset X \}$ , in which every set is measurable. All other Boolean algebras are intermediate between these two extremes: finer than the trivial algebra, but coarser than the discrete one. 

Exercise 1.4.1 (Elementary algebra). Let $\overline { { \mathcal { E } [ { \bf R } ^ { d } ] } }$ be the collection of those sets $E \subset \mathbf { R } ^ { d }$ that are either elementary sets, or co-elementary sets (i.e. the complement of an elementary set). Show that $\overline { { \mathcal { E } [ \mathbf { R } ^ { d } ] } }$ is a Boolean algebra. We will call this algebra the elementary Boolean algebra of $\mathbf { R } ^ { d }$ 

Example 1.4.4 (Jordan algebra). Let $\overline { { \mathcal { I } [ \mathbf { R } ^ { d } ] } }$ be the collection of subsets of $\mathbf { R } ^ { d }$ that are either Jordan measurable or co-Jordan measurable (i.e. the complement of a Jordan measurable set). Then $\overline { { \mathcal { I } [ \mathbf { R } ^ { d } ] } }$ is a Boolean algebra that is finer than the elementary algebra. We refer to this algebra as the Jordan algebra on $\mathbf { R } ^ { d }$ (but caution that there is a completely diferent concept of a Jordan algebra in abstract algebra.) 

Example 1.4.5 (Lebesgue algebra). Le $\mathcal { L } [ \mathbf { R } ^ { d } ]$ be the collection of Lebesgue measurable subsets of $\mathbf { R } ^ { d }$ . Then $\mathcal { L } [ \mathbf { R } ^ { d } ]$ is a Boolean algebra that is finer than the Jordan algebra; we refer to this as the Lebesgue algebra on $\mathbf { R } ^ { d }$ 

Example 1.4.6 (Null algebra). Let $\mathcal { N } ( \mathbf { R } ^ { d } )$ be the collection of subsets of $\mathbf { R } ^ { d }$ that are either Lebesgue null sets or Lebesgue co-null sets (the complement of null sets). Then $\mathcal { N } ( \mathbf { R } ^ { d } )$ is a Boolean algebra that is coarser than the Lebesgue algebra; we refer to it as the null algebra on $\mathbf { R } ^ { d }$ 

Exercise 1.4.2 (Restriction). Let B be a Boolean algebra on a set X, and let Y be a subset of X (not necessarily B-measurable). Show that the restriction $B \ \lvert \boldsymbol { \mathrm { { r } } } : = \left\{ E \cap \boldsymbol { \mathrm { { Y } } } : E \in \boldsymbol { B } \right\}$ of B to Y is a Boolean algebra on Y. If Y is B-measurable, show that 

$$
\mathcal {B} \mid_ {Y} = \mathcal {B} \cap 2 ^ {Y} = \{E \subset Y: E \in \mathcal {B} \}.
$$

Example 1.4.7 (Atomic algebra). Let X be partitioned into a union $\textstyle X = \bigcup _ { \alpha \in I } A _ { \alpha }$ of disjoint sets $A _ { \alpha }$ , which we refer to as atoms. Then this partition generates a Boolean algebra $\mathcal { A } ( ( A _ { \alpha } ) _ { \alpha \in I } )$ , defined as the collection of all the sets E of the form $E = \textstyle \bigcup _ { \alpha \in J } A _ { \alpha }$ for some $J \subset I$ , i.e. $\mathcal { A } ( ( A _ { \alpha } ) _ { \alpha \in I } )$ is the collection of all sets that can be represented as the union of one or more atoms. This is easily verified to be a Boolean algebra, and we refer to it as the atomic algebra with atoms $( A _ { \alpha } ) _ { \alpha \in I }$ The trivial algebra corresponds to the trivial partition $X = X$ into a single atom; at the other extreme, the discrete algebra corresponds to the discrete partition $\textstyle X = \bigcup _ { x \in X } \{ x \}$ into singleton atoms. More generally, note that finer (resp. coarser) partitions lead to finer (resp. coarser) atomic algebra. In this definition, we permit some of the atoms in the partition to be empty; but it is clear that empty atoms have no impact on the final atomic algebra, and so without loss of generality one can delete all empty atoms and assume that all atoms are non-empty if one wishes. 

Example 1.4.8 (Dyadic algebras). Let n be an integer. The dyadic algebra $\mathcal { D } _ { n } ( \mathbf { R } ^ { d } )$ at scale $2 ^ { - n }$ in $\mathbf { R } ^ { d }$ is defined to be the atomic algebra generated by the half-open dyadic cubes 

$$
\left[ \frac {i _ {1}}{2 ^ {n}}, \frac {i _ {1} + 1}{2 ^ {n}}\right) \times \dots \times \left[ \frac {i _ {d}}{2 ^ {n}}, \frac {i _ {d} + 1}{2 ^ {n}}\right)
$$

of length $2 ^ { - n }$ (see Exercise 1.1.14). These are Boolean algebras which are increasing in n: $\mathcal { D } _ { n + 1 } \supset \mathcal { D } _ { n }$ . Draw a diagram to indicate how these algebras sit in relation to the elementary, Jordan, and Lebesgue, null, discrete, and trivial algebras. 

Remark 1.4.9. The dyadic algebras are analogous to the finite resolution one has on modern computer monitors, which subdivide space into square pixels. A low resolution monitor (in which each pixel has a large size) can only resolve a very small set of “blocky” images, as opposed to the larger class of images that can be resolved by a finer resolution monitor. 

Exercise 1.4.3. Show that the non-empty atoms of an atomic algebra are determined up to relabeling. More precisely, show that if $\begin{array} { r } { X = \bigcup _ { \alpha \in I } A _ { \alpha } = \bigcup _ { \alpha ^ { \prime } \in I ^ { \prime } } A _ { \alpha ^ { \prime } } ^ { \prime } } \end{array}$ are two partitions of X into non-empty atoms $A _ { \alpha } , A _ { \alpha ^ { \prime } } ^ { \prime }$ , then $\bar { \mathcal { A } } ( ( A _ { \alpha } ) _ { \alpha \in I } ) = \mathcal { A } ( ( A _ { \alpha ^ { \prime } } ^ { \prime } ) _ { \alpha ^ { \prime } \in I ^ { \prime } } )$ if and only if exists a bijection $\phi : I  I ^ { \prime }$ such that $A _ { \phi ( \alpha ) } ^ { \prime } = A _ { \alpha }$ for all $\alpha \in I$ 

While many Boolean algebras are atomic, many are not, as the following two exercises indicate. 

Exercise 1.4.4. Show that every finite Boolean algebra is an atomic algebra. (A Boolean algebra B is finite if its cardinality is finite, i.e. there are only finitely many measurable sets.) Conclude that every finite Boolean algebra has a cardinality of the form $2 ^ { n }$ for some natural number n. From this exercise and Exercise 1.4.3 we see that there is a one-to-one correspondence between finite Boolean algebras on X and finite partitions of X into non-empty sets (up to relabeling). 

Exercise 1.4.5. Show that the elementary, Jordan, Lebesgue, and null algebras are not atomic algebras. (Hint: argue by contradiction. If these algebras were atomic, what must the atoms be?) 

Now we describe some further ways to generate Boolean algebras. 

Exercise 1.4.6 (Intersection of algebras). Let $( B _ { \alpha } ) _ { \alpha \in I }$ be a family of Boolean algebras on a set X, indexed by a (possibly infinite or uncountable) label set I. Show that the intersection $\textstyle \bigwedge _ { \alpha \in I } B _ { \alpha } \ : =$ $\cap _ { \alpha \in I } B _ { \alpha }$ of these algebras is still a Boolean algebra, and is the finest 

Boolean algebra that is coarser than all of the $B _ { \alpha }$ . (If I is empty, we adopt the convention that $\textstyle \bigwedge _ { \alpha \in I } B _ { \alpha }$ is the discrete algebra.) 

Definition 1.4.10 (Generation of algebras). Let $\mathcal { F }$ be any family of sets in $X$ . We define $\langle \mathcal { F } \rangle _ { \mathrm { b o o l } }$ to be the intersection of all the Boolean algebras that contain ${ \mathcal { F } } _ { : }$ , which is again a Boolean algebra by Exercise 1.4.6. Equivalently, $\langle \mathcal { F } \rangle _ { \mathrm { b o o l } }$ is the coarsest Boolean algebra that contains $\mathcal { F }$ . We say that $\langle \mathcal { F } \rangle _ { \mathrm { b o o l } }$ is the Boolean algebra generated by $\mathcal { F }$ 

Example 1.4.11. $\mathcal { F }$ is a Boolean algebra if and only if $\langle \mathcal { F } \rangle _ { \mathrm { b o o l } } = \mathcal { F }$ ; thus each Boolean algebra is generated by itself. 

Exercise 1.4.7. Show that the elementary algebra $\mathcal { E } ( \mathbf { R } ^ { d } )$ is generated by the collection of boxes in $\mathbf { R } ^ { d }$ 

Exercise 1.4.8. Let n be a natural number. Show that if $\mathcal { F }$ is a finite collection of n sets, then $\langle \mathcal { F } \rangle _ { \mathrm { b o o l } }$ is a finite Boolean algebra of cardinality at most $2 ^ { 2 ^ { n } }$ (in particular, finite sets generate finite algebras). Give an example to show that this bound is best possible. (Hint: for the latter, it may be convenient to use a discrete ambient space such as the discrete cube $X = \{ 0 , 1 \} ^ { n } . )$ 

The Boolean algebra $\langle \mathcal { F } \rangle _ { \mathrm { b o o l } }$ can be described explicitly in terms of $\mathcal { F }$ as follows: 

Exercise 1.4.9 (Recursive description of a generated Boolean algebra). Let $\mathcal { F }$ be a collection of sets in a set $X$ . Define the sets $\mathcal { F } _ { 0 } , \mathcal { F } _ { 1 } , \mathcal { F } _ { 2 } , . . .$ . recursively as follows: 

(i) $\mathcal { F } _ { 0 } : = \mathcal { F } .$ 

(ii) For each $n \geq 1$ , we define $\mathcal { F } _ { n }$ to be the collection of all sets that either the union of a finite number of sets in $\mathcal { F } _ { n - 1 }$ (including the empty union $\varnothing )$ , or the complement of such a union. 

Show that $\textstyle \langle { \mathcal { F } } \rangle _ { \mathrm { b o o l } } = \bigcup _ { n = 0 } ^ { \infty } { \mathcal { F } } _ { n }$ 

1.4.2. σ-algebras and measurable spaces. In order to obtain a measure and integration theory that can cope well with limits, the finite union axiom of a Boolean algebra is insuficient, and must be improved to a countable union axiom: 

Definition 1.4.12 (Sigma algebras). Let X be a set. A σ-algebra on X is a collection B of X which obeys the following properties: 

(i) (Empty set) $\varnothing \in B .$ 

(ii) (Complement) If $E \in B$ , then the complement $E ^ { c } : = X \backslash E$ also lies in B. 

(iii) (Countable unions) If $E _ { 1 } , E _ { 2 } , \dots \in B$ , then $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n } \in B$ 

We refer to the pair (X, B) of a set X together with a σ-algebra on that set as a measurable space. 

Remark 1.4.13. The prefix $\sigma$ usually denotes “countable union”. Other instances of this prefix include a σ-compact topological space (a countable union of compact sets), a σ-finite measure space (a countable union of sets of finite measure), or $F _ { \sigma }$ set (a countable union of closed sets) for other instances of this prefix. 

From de Morgan’s law (which is just as valid for infinite unions and intersections as it is for finite ones), we see that σ-algebras are closed under countable intersections as well as countable unions. 

By padding a finite union into a countable union by using the empty set, we see that every σ-algebra is automatically a Boolean algebra. Thus, we automatically inherit the notion of being measurable with respect to a σ-algebra, or of one σ-algebra being coarser or finer than another. 

Exercise 1.4.10. Show that all atomic algebras are σ-algebras. In particular, the discrete algebra and trivial algebra are σ-algebras, as are the finite algebras and the dyadic algebras on Euclidean spaces. 

Exercise 1.4.11. Show that the Lebesgue and null algebras are $\sigma -$ algebras, but the elementary and Jordan algebras are not. 

Exercise 1.4.12. Show that any restriction B  of a σ-algebra B to a subspace Y of X (as defined in Exercise 1.4.2) is again a σ-algebra on the subspace Y. 

There is an exact analogue of Exercise 1.4.6: 

Exercise 1.4.13 (Intersection of $\sigma { \mathrm { - a l g e b r a s } } )$ . Show that the intersection $\textstyle \bigwedge _ { \alpha \in I } B _ { \alpha } : = \bigcap _ { \alpha \in I } B _ { \alpha }$ of an arbitrary (and possibly infinite or uncountable) number of σ-algebras $B _ { \alpha }$ is again a σ-algebra, and is the finest σ-algebra that is coarser than all of the $B _ { \alpha }$ 

Similarly, we have a notion of generation: 

Definition 1.4.14 (Generation of σ-algebras). Let $\mathcal { F }$ be any family of sets in $X$ . We define $\langle \mathcal { F } \rangle$ to be the intersection of all the σ-algebras that contain $\mathcal { F }$ , which is again a σ-algebra by Exercise 1.4.13. Equivalently, $\langle \mathcal { F } \rangle$ is the coarsest σ-algebra that contains $\mathcal { F }$ . We say that $\langle \mathcal { F } \rangle$ is the σ-algebra generated by $\mathcal { F }$ 

Since every σ-algebra is a Boolean algebra, we have the trivial inclusion 

$$
\langle \mathcal {F} \rangle_ {\mathrm{bool}} \subset \langle \mathcal {F} \rangle .
$$

However, equality need not hold; it only holds if and only if $\langle \mathcal { F } \rangle _ { \mathrm { b o o l } }$ is a σ-algebra. For instance, if $\mathcal { F }$ is the collection of all boxes in $\mathbf { R } ^ { d }$ , then $\langle \mathcal { F } \rangle _ { \mathrm { b o o l } }$ is the elementary algebra (Exercise 1.4.7), bu $\langle \mathcal { F } \rangle$ cannot equal this algebra, as it is not a σ-algebra. 

Remark 1.4.15. From the definitions, it is clear that we have the following principle, somewhat analogous to the principle of mathematical induction: if $\mathcal { F }$ is a family of sets in $X$ , and $P ( E )$ is a property of sets $E \subset X$ which obeys the following axioms: 

(i) $P ( \varnothing )$ is true. 

(ii) $P ( E )$ is true for al $E \in { \mathcal { F } }$ 

(iii) If $P ( E )$ is true for some $E \subset X$ , then $P ( X \backslash E )$ is true also. 

(iv) If $E _ { 1 } , E _ { 2 } , \dots \subset X$ are such that $P ( E _ { n } )$ is true for all $n ,$ , then $\textstyle P ( \bigcup _ { n = 1 } ^ { \infty } E _ { n } )$ is true also. 

Then one can conclude that $P ( E )$ is true for all $E \in \langle { \mathcal { F } } \rangle$ i. Indeed, the set of all $E$ for which $P ( E )$ holds is a σ-algebra that contains $\mathcal { F }$ whence the claim. This principle is particularly useful for establishing properties of Borel measurable sets (see below). 

We now turn to an important example of a σ-algebra: 

Definition 1.4.16 (Borel σ-algebra). Let X be a metric space, or more generally a topological space. The Borel σ-algebra $B [ X ]$ of X is defined to be the σ-algebra generated by the open subsets of X. Elements of $B [ X ]$ will be called Borel measurable. 

Thus, for instance, the Borel σ-algebra contains the open sets, the closed sets (which are complements of open sets), the countable unions of closed sets (known as $F _ { \sigma }$ sets), the countable intersections of open sets (known as $G _ { \delta }$ sets), the countable intersections of $F _ { \sigma }$ sets, and so forth. 

In $\mathbf { R } ^ { d } .$ , every open set is Lebesgue measurable, and so we see that the Borel σ-algebra is coarser than the Lebesgue σ-algebra. We wil shortly see, though, that the two σ-algebras are not equal. 

We defined the Borel σ-algebra to be generated by the open sets. However, they are also generated by several other sets: 

Exercise 1.4.14. Show that the Borel σ-algebra $B [ \mathbf { R } ^ { d } ]$ of a Euclidean set is generated by any of the following collections of sets: 

(i) The open subsets of $\mathbf { R } ^ { d }$ 

(ii) The closed subsets of $\mathbf { R } ^ { d } .$ 

(iii) The compact subsets of $\mathbf { R } ^ { d } .$ 

(iv) The open balls of $\mathbf { R } ^ { d }$ 

(v) The boxes in $\mathbf { R } ^ { d }$ 

(vi) The elementary sets in $\mathbf { R } ^ { d }$ 

(Hint: To show that two families ${ \mathcal { F } } , { \mathcal { F } } ^ { \prime }$ of sets generate the same σ-algebra, it sufices to show that every σ-algebra that contains $\mathcal { F }$ contains ${ \mathcal { F } } ^ { \prime }$ also, and conversely.) 

There is an analogue of Exercise 1.4.9, which illustrates the extent to which a generated σ-algebra is “larger” than the analogous generated Boolean algebra: 

Exercise 1.4.15 (Recursive description of a generated σ-algebra). (This exercise requires familiarity with the theory of ordinals, which is reviewed in §2.4 of An epsilon of room, Vol. I. Recall that we are assuming the axiom of choice throughout this text.) Let $\mathcal { F }$ be a collection of sets in a set X, and let $\omega _ { 1 }$ be the first uncountable ordinal. Define the sets ${ \mathcal { F } } _ { \alpha }$ for every countable ordinal $\alpha \in \omega _ { 1 }$ via transfinite induction as follows: 

(i) $\mathcal { F } _ { \alpha } : = \mathcal { F } .$ 

(ii) For each countable successor ordinal $\alpha = \beta + 1$ , we define ${ \mathcal { F } } _ { \alpha }$ to be the collection of all sets that either the union of an at most countable number of sets in $\mathcal { F } _ { n - 1 }$ (including the empty union ∅), or the complement of such a union. 

(iii) For each countable limit ordina $\alpha = \operatorname* { s u p } _ { \beta < \alpha } \beta$ , we define $\textstyle { \mathcal { F } } _ { \alpha } : = \bigcup _ { \beta < \alpha } { \mathcal { F } } _ { \beta }$ 

Show that $\textstyle \langle { \mathcal { F } } \rangle = \bigcup _ { \alpha \in \omega _ { 1 } } { \mathcal { F } } _ { \alpha }$ 

Remark 1.4.17. The first uncountable ordinal $\omega _ { 1 }$ will make several further cameo appearances here and in An epsilon of room, Vol. I, for instance by generating counterexamples to various plausible statements in point-set topology. In the case when $\mathcal { F }$ is the collection of open sets in a topological space, so that $\langle \mathcal { F } \rangle$ , then the sets ${ \mathcal { F } } _ { \alpha }$ are essentially the Borel hierarchy (which starts at the open and closed sets, then moves on to the $F _ { \sigma }$ and $G _ { \delta }$ sets, and so forth); these play an important role in descriptive set theory. 

Exercise 1.4.16. (This exercise requires familiarity with the theory of cardinals.) Let $\mathcal { F }$ be an infinite family of subsets of X of cardinality κ (thus κ is an infinite cardinal). Show that $\langle \mathcal { F } \rangle$ has cardinality at most $\kappa ^ { \aleph _ { 0 } }$ . (Hint: use Exercise 1.4.15.) In particular, show that the Borel σ-algebra $B [ \mathbf { R } ^ { d } ]$ has cardinality at most $c : = 2 ^ { \aleph _ { 0 } }$ 

Conclude that there exist Jordan measurable (and hence Lebesgue measurable) subsets of $\mathbf { R } ^ { d }$ which are not Borel measurable. (Hint: How many subsets of the Cantor set are there?) Use this to place the Borel σ-algebra on the diagram that you drew for Exercise 1.4.8. 

Remark 1.4.18. Despite this demonstration that not all Lebesgue measurable subsets are Borel measurable, it is remarkably dificult (though not impossible) to exhibit a specific set that is not Borel measurable. Indeed, a large majority of the explicitly constructible sets that one actually encounters in practice tend to be Borel measurable, and one can view the property of Borel measurability intuitively as a kind of “constructibility” property. (Indeed, as a very crude first approximation, one can view the Borel measurable sets as those sets of “countable descriptive complexity”; in contrast, sets of finite descriptive complexity tend to be Jordan measurable (assuming they are bounded, of course). 

Exercise 1.4.17. Let E, F be Borel measurable subsets of $\mathbf { R } ^ { d _ { 1 } } , \mathbf { R } ^ { d _ { 2 } }$ respectively. Show that $E \times F$ is a Borel measurable subset of $\mathbf { R } ^ { d _ { 1 } + d _ { 2 } }$ (Hint: first establish this in the case when $F$ is a box, by using Remark 1.4.15. To obtain the general case, apply Remark 1.4.15 yet again.) 

The above exercise has a partial converse: 

Exercise 1.4.18. Let E be a Borel measurable subset of $\mathbf { R } ^ { d _ { 1 } + d _ { 2 } }$ 

(i) Show that for any $x _ { 1 } \in \mathbf { R } ^ { d _ { 1 } }$ , the slice $\{ x _ { 2 } \in \mathbf { R } ^ { d _ { 2 } } : ( x _ { 1 } , x _ { 2 } ) \in$ $E \}$ is a Borel measurable subset of $\mathbf { R } ^ { d _ { 2 } }$ . Similarly, show that for every $x _ { 2 } \in \mathbf { R } ^ { d _ { 2 } }$ , the slice $\{ x _ { 1 } \in \mathbf { R } ^ { d _ { 1 } } : ( x _ { 1 } , x _ { 2 } ) \in E \}$ is a Borel measurable subset of $\mathbf { R } ^ { d _ { 1 } }$ 

(ii) Give a counterexample to show that this claim is not true if “Borel” is replaced with “Lebesgue” throughout. (Hint: the Cartesian product of any set with a point is a null set, even if the first set was not measurable.) 

Exercise 1.4.19. Show that the Lebesgue σ-algebra on $\mathbf { R } ^ { d }$ is generated by the union of the Borel σ-algebra and the null σ-algebra. 

1.4.3. Countably additive measures and measure spaces. Having set out the concept of a σ-algebra a measurable space, we now endow these structures with a measure. 

We begin with the finitely additive theory, although this theory is too weak for our purposes and will soon be supplanted by the countably additive theory. 

Definition 1.4.19 (Finitely additive measure). Let $\boldsymbol { B }$ be a Boolean algebra on a space X. An (unsigned) finitely additive measure $\mu$ on B is a map $\mu : B \to [ 0 , + \infty ]$ that obeys the following axioms: 

(i) (Empty set) µ(∅) = 0. 

(ii) (Finite additivity) Whenever E, $F \in B$ are disjoint, then $\mu ( E \cup F ) = \mu ( E ) + \mu ( F )$ 

Remark 1.4.20. The empty set axiom is needed in order to rule out the degenerate situation in which every set (including the empty set) has infinite measure. 

Example 1.4.21. Lebesgue measure m is a finitely additive measure on the Lebesgue σ-algebra, and hence on all sub-algebras (such as the null algebra, the Jordan algebra, or the elementary algebra). In particular, Jordan measure and elementary measure are finitely additive (adopting the convention that co-Jordan measurable sets have infinite Jordan measure, and co-elementary sets have infinite elementary measure). 

On the other hand, as we saw in previous notes, Lebesgue outer measure is not finitely additive on the discrete algebra, and Jordan outer measure is not finitely additive on the Lebesgue algebra. 

Example 1.4.22 (Dirac measure). Let $x \in X$ and B be an arbitrary Boolean algebra on X. Then the Dirac measure $\delta _ { x }$ at x, defined by setting $\delta _ { x } ( E ) : = 1 _ { E } ( x )$ , is finitely additive. 

Example 1.4.23 (Zero measure). The zero measure $0 : E \mapsto 0$ is a finitely additive measure on any Boolean algebra. 

Example 1.4.24 (Linear combinations of measures). If B is a Boolean algebra on X, and $\mu , \nu : B \to [ 0 , + \infty ]$ are finitely additive measures on B, then $\mu + \nu : E \mapsto \mu ( E ) + \nu ( E )$ is also a finitely additive measure, as is $c \mu : E \mapsto c \times \mu ( E )$ for any $c \in [ 0 , + \infty ]$ . Thus, for instance, the sum of Lebesgue measure and a Dirac measure is also a finitely additive measure on the Lebesgue algebra (or on any of its sub-algebras). 

Example 1.4.25 (Restriction of a measure). If B is a Boolean algebra on X, $\mu : B \to [ 0 , + \infty ]$ is a finitely additive measure, and Y is a $B .$ measurable subset of X, then the restriction $\mu \mid _ { Y } : B \mid _ { Y }  [ 0 , + \infty ]$ of B to Y, defined by setting $\mu \mid _ { Y } ( E ) : = \mu ( E )$ whenever $E \in B \ \vert _ { Y }$ (i.e. if $E \in B$ and $E \subset Y )$ , is also a finitely additive measure. 

Example 1.4.26 (Counting measure). If B is a Boolean algebra on X, then the function $\# : B \to [ 0 , + \infty ]$ defined by setting $\# ( E )$ to be the cardinality of E if E is finite, and $\# ( E ) : = + \infty$ if E is infinite, is a finitely additive measure, known as counting measure. 

As with our definition of Boolean algebras and σ-algebras, we adopted a “minimalist” definition so that the axioms are easy to verify. But they imply several further useful properties: 

Exercise 1.4.20. Let $\mu : B \to [ 0 , + \infty ]$ be a finitely additive measure on a Boolean σ-algebra B. Establish the following facts: 

(i) (Monotonicity) If $E , F$ are B-measurable and $E \subset F$ , then $\mu ( E ) \leq \mu ( F )$ 

(ii) (Finite additivity) If k is a natural number, and $E _ { 1 } , \ldots , E _ { k }$ are B-measurable and disjoint, then $\mu ( E _ { 1 } \cup . . . \cup E _ { k } ) \ =$ $\mu ( E _ { 1 } ) + . . . + \mu ( E _ { k } )$ 

(iii) (Finite subadditivity) If k is a natural number, and $E _ { 1 } , \ldots , E _ { k }$ are B-measurable, then $\mu ( E _ { 1 } \cup . . . \cup E _ { k } ) \leq \mu ( E _ { 1 } ) + . . . +$ $\mu ( E _ { k } )$ 

(iv) (Inclusion-exclusion for two sets) If E, F are B-measurable, then $\mu ( E \cup F ) + \mu ( E \cap F ) = \mu ( E ) + \mu ( F )$ 

(Caution: remember that the cancellation law $a + c = b + c \implies a = b$ does not hold in $[ 0 , + \infty ]$ if c is infinite, and so the use of cancellation (or subtraction) should be avoided if possible.) 

One can characterise measures completely for any finite algebra: 

Exercise 1.4.21. Let B be a finite Boolean algebra, generated by a finite family $A _ { 1 } , \ldots , A _ { k }$ of non-empty atoms. Show that for every finitely additive measure $\mu$ on $\boldsymbol { B }$ there exists $c _ { 1 } , \ldots , c _ { k } \in [ 0 , + \infty ]$ such that 

$$
\mu (E) = \sum_ {1 \leq j \leq k: A _ {j} \subset E} c _ {j}.
$$

Equivalently, if $x _ { j }$ is a point in $A _ { j }$ for each $1 \le j \le k$ , then 

$$
\mu = \sum_ {j = 1} ^ {k} c _ {j} \delta_ {x _ {j}}.
$$

Furthermore, show that the $c _ { 1 } , \ldots , c _ { k }$ are uniquely determined by $\mu .$ 

This is about the limit of what one can say about finitely additive measures at this level of generality. We now specialise to the countably additive measures on σ-algebras. 

Definition 1.4.27 (Countably additive measure). Let $( X , B )$ be a measurable space. An (unsigned) countably additive measure $\mu$ on $B { \mathrm { . } }$ or measure for short, is a map $\mu : \mathcal { B }  [ 0 , + \infty ]$ that obeys the following axioms: 

(i) (Empty set) $\mu ( \varnothing ) = 0 .$ 

(ii) (Countable additivity) Whenever $E _ { 1 } , E _ { 2 } , \dots \in B$ are a countable sequence of disjoint measurable sets, then $\textstyle \mu ( \bigcup _ { n = 1 } ^ { \infty } E _ { n } ) =$ $\textstyle \sum _ { n = 1 } ^ { \infty } \mu ( E _ { n } )$ 

A triplet $( X , B , \mu )$ , where $( X , B )$ is a measurable space and $\mu : B \to$ $[ 0 , + \infty ]$ is a countably additive measure, is known as a measure space. 

Note the distinction between a measure space and a measurable space. The latter has the capability to be equipped with a measure, but the former is actually equipped with a measure. 

Example 1.4.28. Lebesgue measure is a countably additive measure on the Lebesgue σ-algebra, and hence on every sub-σ-algebra (such as the Borel σ-algebra). 

Example 1.4.29. The Dirac measures from Exercise 1.4.22 are count ably additive, as is counting measure. 

Example 1.4.30. Any restriction of a countably additive measure to a measurable subspace is again countably additive. 

Exercise 1.4.22 (Countable combinations of measures). Let (X, B) be a measurable space. 

(i) If $\mu$ is a countably additive measure on $B ,$ , and $c \in [ 0 , + \infty ]$ ], then $c \mu$ is also countably additive. 

(ii) If $\mu _ { 1 } , \mu _ { 2 } , \ldots \mathrm { a r e }$ a sequence of countably additive measures on B, then the sum $\begin{array} { r } { \sum _ { n = 1 } ^ { \infty } \mu _ { n } : E \mapsto \sum _ { n = 1 } ^ { \infty } \mu _ { n } ( E ) } \end{array}$ is also a countably additive measure. 

Note that countable additivity measures are necessarily finitely additive (by padding out a finite union into a countable union using the empty set), and so countably additive measures inherit all the properties of finitely additive properties, such as monotonicity and finite subadditivity. But one also has additional properties: 

Exercise 1.4.23. Let $( X , B , \mu )$ be a measure space. 

(i) (Countable subadditivity) If $E _ { 1 } , E _ { 2 } , \ldots$ . are B-measurable, then $\begin{array} { r } { \mu ( \bigcup _ { n = 1 } ^ { \infty } E _ { n } ) \leq \sum _ { n = 1 } ^ { \infty } \mu ( E _ { n } ) } \end{array}$ 

(ii) (Upwards monotone convergence) If $E _ { 1 } \subset E _ { 2 } \subset . .$ . are $B _ { - }$ measurable, then 

$$
\mu (\bigcup_ {n = 1} ^ {\infty} E _ {n}) = \lim _ {n \to \infty} \mu (E _ {n}) = \sup _ {n} \mu (E _ {n}).
$$

(iii) (Downwards monotone convergence) If $E _ { 1 } \supset E _ { 2 } \supset . .$ . are B-measurable, and $\mu ( E _ { n } ) < \infty$ for at least one n, then 

$$
\mu (\bigcap_ {n = 1} ^ {\infty} E _ {n}) = \lim _ {n \to \infty} \mu (E _ {n}) = \inf _ {n} \mu (E _ {n}).
$$

Show that the downward monotone convergence claim can fail if the hypothesis that $\mu ( E _ { n } ) < \infty$ for at least one n is dropped. (Hint: mimic the solution to Exercise 1.2.11.) 

Exercise 1.4.24 (Dominated convergence for sets). Let $( X , B , \mu )$ be a measure space. Let $E _ { 1 } , E _ { 2 } , \ldots .$ . be a sequence of B-measurable sets that converge to another set $E ,$ in the sense that $1 _ { E _ { n } }$ converges pointwise to $1 _ { E }$ 

(i) Show that E is also B-measurable. 

(ii) If there exists a B-measurable set F of finite measure (i.e. $\mu ( F ) < \infty )$ that contains all of the $E _ { n }$ , show that $\scriptstyle \operatorname* { l i m } _ { n \to \infty } \mu ( E _ { n } ) =$ $\mu ( E )$ . (Hint: Apply downward monotonicity to the sets $\begin{array} { r } { \bigcup _ { n > N } ( E _ { n } \Delta E ) . ) } \end{array}$ 

(iii) Show that the previous part of this exercise can fail if the hypothesis that all the $E _ { n }$ are contained in a set of finite measure is omitted. 

Exercise 1.4.25. Let X be an at most countable set with the discrete σ-algebra. Show that every measure $\mu$ on this measurable space can be uniquely represented in the form 

$$
\mu = \sum_ {x \in X} c _ {x} \delta_ {x}
$$

for some $c _ { x } \in [ 0 , + \infty ]$ , thus 

$$
\mu (E) = \sum_ {x \in E} c _ {x}
$$

for all $E \subset X$ . (This claim fails in the uncountable case, although showing this is slightly tricky.) 

A useful technical property, enjoyed by some measure spaces, is that of completeness: 

Definition 1.4.31 (Completeness). A null set of a measure space $( X , B , \mu )$ is defined to be a B-measurable set of measure zero. A subnull set is any subset of a null set. A measure space is said to be complete if every sub-null set is a null set. 

Thus, for instance, the Lebesgue measure space $( \mathbf { R } ^ { d } , \mathcal { L } [ \mathbf { R } ^ { d } ] , m )$ is complete, but the Borel measure space $( \mathbf { R } ^ { d } , B [ \mathbf { R } ^ { d } ] , m )$ is not (as can be seen from the solution to Exercise 1.4.16). 

Completion is a convenient property to have in some cases, particularly when dealing with properties that hold almost everywhere. Fortunately, it is fairly easy to modify any measure space to be complete: 

Exercise 1.4.26 (Completion). Let $( X , B , \mu )$ be a measure space. Show that there exists a unique refinement $( X , { \overline { { B } } } , { \overline { { \mu } } } )$ , known as the completion of $( X , B , \mu )$ , which is the coarsest refinement of $( X , B , \mu )$ that is complete. Furthermore, show that $\overline { { B } }$ consists precisely of those sets that difer from a B-measurable set by a B-subnull set. 

Exercise 1.4.27. Show that the Lebesgue measure space $( \mathbf { R } ^ { d } , \mathcal { L } [ \mathbf { R } ^ { d } ] , m )$ is the completion of the Borel measure space $( \mathbf { R } ^ { d } , B [ \mathbf { R } ^ { d } ] , m )$ 

Exercise 1.4.28 (Approximation by an algebra). Let $\mathcal { A }$ be a Boolean algebra on X, and let $\mu$ be a measure on $\langle \mathcal { A } \rangle$ 

(i) If $\mu ( X ) < \infty$ , show that for every $E \in \langle { \mathcal { A } } \rangle$ and $\varepsilon > 0$ there exists $F \in { \mathcal { A } }$ such that $\mu ( E \Delta F ) < \varepsilon$ 

(ii) More generally, if $\textstyle X = \bigcup _ { n = 1 } ^ { \infty } A _ { n }$ for some $A _ { 1 } , A _ { 2 } , \dotsc \in { \mathcal { A } }$ with $\mu ( A _ { n } ) < \infty$ for all $n , E \in \langle A \rangle$ has finite measure, and $\varepsilon > 0$ , show that there exists $F \in { \mathcal { A } }$ such that $\mu ( E \Delta F ) < \varepsilon$ 

1.4.4. Measurable functions, and integration on a measure space. Now we are ready to define integration on measure spaces. We first need the notion of a measurable function, which is analogous to that of a continuous function in topology. Recall that a function $f : X \to Y$ between two topological spaces $X , Y$ is continuous if the inverse image $f ^ { - 1 } ( U )$ of any open set is open. In a similar spirit, we have 

Definition 1.4.32. Let $( X , B )$ be a measurable space, and let $f :$ $X \ \to \ [ 0 , + \infty ]$ or $f : X \to \mathbf { C }$ be an unsigned or complex-valued function. We say that f is measurable if $f ^ { - 1 } ( U )$ is B-measurable for every open subset U of $[ 0 , + \infty ] \mathrm { ~ o r ~ } \mathbf { C }$ 

From Lemma 1.3.9, we see that this generalises the notion of a Lebesgue measurable function. 

Exercise 1.4.29. Let $( X , B )$ be a measurable space. 

(i) Show that a function $f : X \to [ 0 , + \infty ]$ is measurable if and only if the level sets $\{ x \in X : f ( x ) > \lambda \}$ are B-measurable. 

(ii) Show that an indicator function $1 _ { E }$ of a set $E \subset X$ is measurable if and only if E itself is B-measurable. 

(iii) Show that a function $f : X \to [ 0 , + \infty ]$ or $f : X \to \mathbf { C }$ is measurable if and only if $f ^ { - 1 } ( E )$ is B-measurable for every Borel-measurable subset E of $[ 0 , + \infty ] \mathrm { ~ o r ~ } \mathbf { C }$ 

(iv) Show that a function $f : X \to \mathbf { C }$ is measurable if and only if its real and imaginary parts are measurable. 

(v) Show that a function $f : X \to \mathbf { R }$ is measurable if and only if the magnitudes $f _ { + } : = \operatorname* { m a x } ( f , 0 ) , f _ { - } : = \operatorname* { m a x } ( - f , 0 )$ of its positive and negative parts are measurable. 

(vi) If $f _ { n } : X \to [ 0 , + \infty ]$ are a sequence of measurable functions that converge pointwise to a limit $f : X  [ 0 , + \infty ]$ , then show that $f$ is also measurable. Obtain the same claim if $[ 0 , + \infty ]$ is replaced by C. 

(vii) If $f : X \to [ 0 , + \infty ]$ is measurable and $\phi : [ 0 , + \infty ]  [ 0 , + \infty ]$ is continuous, show that $\phi \circ f$ is measurable. Obtain the same claim if $[ 0 , + \infty ]$ is replaced by C. 

(viii) Show that the sum or product of two measurable functions in $[ 0 , + \infty ]$ or C is still measurable. 

Remark 1.4.33. One can also view measurable functions in a more category theoretic fashion. Define measurable morphism or measurable map f from one measurable space $( X , B )$ to another $( Y , { \mathcal { C } } )$ to be a function $f : X \to Y$ with the property that $f ^ { - 1 } ( E )$ is $B _ { - }$ measurable for every C-measurable set $E .$ . Then a measurable function $f : X \to [ 0 , + \infty ]$ or $f : X \to \mathbf { C }$ is the same thing as a measurable morphism from $X$ to $[ 0 , + \infty ]$ or C, where the latter is equipped with the Borel σ-algebra. Also, one σ-algebra $\boldsymbol { B }$ on a space $X$ is coarser than another $B ^ { \prime }$ precisely when the identity map id $x : X \to X$ is a measurable morphism from $( X , B ^ { \prime } )$ to $( X , B )$ . The main purpose of adopting this viewpoint is that it is obvious that the composition of measurable morphisms is again a measurable morphism. This is important in those fields of mathematics, such as ergodic theory (discussed in [Ta2009]), in which one frequently wishes to compose measurable transformations (and in particular, to compose a transformation $T : ( X , B ) \to ( X , B )$ with itself repeatedly); but it will not play a major role in this text. 

Measurable functions are particularly easy to describe on atomic spaces: 

Exercise 1.4.30. Let $( X , B )$ be a measurable space that is atomic, thus $B = \mathcal { A } ( ( A _ { \alpha } ) _ { \alpha \in I } )$ for some partition $\textstyle X = \bigcup _ { \alpha \in I } A _ { \alpha }$ of $X$ into disjoint non-empty atoms. Show that a function $f : X \to [ 0 , + \infty ]$ or $f : X \to \mathbf { C }$ is measurable if and only if it is constant on each atom, or equivalently if one has a representation of the form 

$$
f = \sum_ {\alpha \in I} c _ {\alpha} 1 _ {A _ {\alpha}}
$$

for some constants $c _ { \alpha }$ in $[ 0 , + \infty ]$ or in C as appropriate. Furthermore, the $c _ { \alpha }$ are uniquely determined by $f .$ 

Exercise 1.4.31 (Egorov’s theorem). Let $( X , B , \mu )$ be a finite measure space (so $\mu ( X ) < \infty )$ , and let $f _ { n } : X \to \mathbf { C }$ be a sequence of measurable functions that converge pointwise almost everywhere to a limit $f : X \to \mathbf { C }$ , and let $\varepsilon > 0$ . Show that there exists a measurable set $E$ of measure at most ε such that $f _ { n }$ converges uniformly to $f$ outside of $E .$ . Give an example to show that the claim can fail when the measure $\mu$ is not finite. 

In Section 1.3 we defined first an simple integral, then an unsigned integral, and then finally an absolutely convergent integral. We perform the same three stages here. We begin with the simple integral, which in the abstract setting becomes integration in the case when the σ-algebra is finite: 

Definition 1.4.34 (Simple integral). Let $( X , B , \mu )$ be a measure space with B finite. By Exercise 1.4.4, X is partitioned into a finite number of atoms $A _ { 1 } , \ldots , A _ { n }$ . If $f : X \to [ 0 , + \infty ]$ is measurable, then by Exercise 1.4.30 it has a unique representation of the form 

$$
f = \sum_ {i = 1} ^ {n} c _ {i} 1 _ {A _ {i}}
$$

for some $c _ { 1 } , \ldots , c _ { n } \in [ 0 , + \infty ]$ . We then define the simple integral Simp $\textstyle \int _ { X } f$ dµ of f by the formula 

$$
\operatorname{Simp} \int_ {X} f d \mu := \sum_ {i = 1} ^ {n} c _ {i} \mu (A _ {i}).
$$

Note that, thanks to Exercise 1.4.3, the precise decomposition into atoms does not afect the definition of the simple integral. 

Exercise 1.4.32. Propose a definition for the simple integral for absolutely convergent complex-valued functions on a measurable space with a finite σ-algebra. 

With this definition, it is clear that one has the monotonicity property 

$$
\operatorname{Simp} \int_ {X} f d \mu \leq \operatorname{Simp} \int_ {X} g d \mu
$$

whenever $f \ \leq \ g$ are unsigned measurable, as well as the linearity properties 

$$
\operatorname{Simp} \int_ {X} f + g d \mu = \operatorname{Simp} \int_ {X} f d \mu + \operatorname{Simp} \int_ {X} g d \mu
$$

and 

$$
\operatorname{Simp} \int_ {X} c f d \mu = c \times \operatorname{Simp} \int_ {X} f d \mu
$$

for unsigned measurable $f , g$ and $c \in [ 0 , + \infty ]$ . We also make the following important technical observation: 

Exercise 1.4.33 (Simple integral unafected by refinements). Let $( X , B , \mu )$ be a measure space, and let $( X , B ^ { \prime } , \mu ^ { \prime } )$ be a refinement of $( X , B , \mu )$ , which means that $B ^ { \prime }$ contains B and $\mu ^ { \prime } : B ^ { \prime } \to [ 0 , + \infty ]$ agrees with $\mu : B \to [ 0 , + \infty ]$ on $B .$ . Suppose that both $B , B ^ { \prime }$ are finite, and let $f : B \to [ 0 , + \infty ]$ be measurable. Show that 

$$
\mathrm{Simp} \int_ {X} f d \mu = \mathrm{Simp} \int_ {X} f d \mu^ {\prime}.
$$

This allows one to extend the simple integral to simple functions: 

Definition 1.4.35 (Integral of simple functions). An (unsigned) simple function $f : X \to [ 0 , + \infty ]$ on a measurable space $( X , B )$ is a measurable function that takes on finitely many values $a _ { 1 } , \ldots , a _ { k }$ . Note that such a function is then automatically measurable with respect to at least one finite sub-σ-algebra $B ^ { \prime }$ of $B { \mathrm { . } }$ , namely the σ-algebra $B ^ { \prime }$ generated by the preimages $f ^ { - 1 } ( \{ a _ { 1 } \} ) , \ldots , f ^ { - 1 } ( \{ a _ { k } \} )$ ) of $a _ { 1 } , \ldots , a _ { k }$ We then define the simple integral Simp $\textstyle \int _ { X } f  d \mu$ by the formula 

$$
\mathrm{Simp} \int_ {X} f d \mu := \mathrm{Simp} \int_ {X} f d \mu \mathbin {\lrcorner} _ {\mathcal {B ^ {\prime}}},
$$

where $\mu \ \lfloor \boldsymbol { B } ^ { \prime } \colon \boldsymbol { B } ^ { \prime } \to [ 0 , + \infty ]$ is the restriction of $\mu : B \to [ 0 , + \infty ]$ to $B ^ { \prime }$ 

Note that there could be multiple finite σ-algebras with respect to which $f$ is measurable, but Exercise 1.4.33 guarantees that all such extensions will give the same simple integral. Indeed, if $f$ were measurable with respect to two separate finite sub-σ-algebras $B ^ { \prime }$ and $B ^ { \prime \prime }$ of $B { \mathrm { . } }$ , then it would also be measurable with respect to their common refinement $\begin{array} { r } { B ^ { \prime } \vee B ^ { \prime \prime } : = \langle B ^ { \prime } \cup B ^ { \prime \prime } \rangle } \end{array}$ i, which is also finite (by Exercise 1.4.8), and then by Exercise 1.4.33, $\int _ { X } f \ d \mu \ l _ { B ^ { \prime } }$ and $\int _ { X } f \ d \mu \ l _ { B ^ { \prime \prime } }$ are both equal to $\textstyle \int _ { X } f \ d \mu \ \lfloor _ { B ^ { \prime } \vee B ^ { \prime \prime } }$ , and hence equal to each other. 

From this we can deduce the following properties of the simple integral. As with the Lebesgue theory, we say that a property $P ( x )$ of an element $x \in X$ of a measure space $( X , B , \mu )$ holds $\mu { - } a l m o s t$ everywhere if it holds outside of a sub-null set. 

Exercise 1.4.34 (Basic properties of the simple integral). Let $( X , B , \mu )$ be a measure space, and let $f , g : X \to [ 0 , + \infty ]$ be simple functions. 

(i) (Monotonicity) If $f \ \leq \ g$ pointwise, then Simp $\textstyle \int _ { X } f \ d \mu \ \leq$ Simp $\textstyle \int _ { X } g \ d \mu$ 

(ii) (Compatibility with measure) For every B-measurable set $E _ { i }$ , we have Simp $\textstyle \int _ { X } 1 _ { E } \ d \mu = \mu ( E )$ 

(iii) (Homogeneity) For every $c \in [ 0 , + \infty ]$ , one has Simp $\textstyle \int _ { X } c f d \mu =$ $c \times \operatorname { S i m p } \int _ { X } f \ d \mu$ 

(iv) (Finite additivity) Simp $\begin{array} { r } { \int _ { X } ( f + g ) ~ d \mu = \operatorname* { S i m p } \int _ { X } f ~ d \mu + } \end{array}$ Simp $\textstyle \int _ { X } g \ d \mu$ 

(v) (Insensitivity to refinement) If $( X , B ^ { \prime } , \mu ^ { \prime } )$ is a refinement of $( X , B , \mu )$ (as defined in Exercise 1.4.33), then Simp $\textstyle \int _ { X } f d \mu =$ Simp $\int _ { X } f \ d \mu ^ { \prime }$ 

(vi) (Almost everywhere equivalence) If $f ( x ) = g ( x )$ for µ-almost every $x \in X$ , then Simp $\textstyle \int _ { X } f \ d \mu = \operatorname { S i m p } \int _ { X } g \ d \mu$ 

(vii) (Finiteness) Simp $\textstyle \int _ { X } f \ d \mu < \infty$ if and only if f is finite almost everywhere, and is supported on a set of finite measure. 

(viii) (Vanishing) Simp $\textstyle \int _ { X } f d \mu = 0$ if and only if f is zero almost everywhere. 

Exercise 1.4.35 (Inclusion-exclusion principle). Let $( X , B , \mu )$ be a measure space, and let $A _ { 1 } , \ldots , A _ { n }$ be B-measurable sets of finite measure. Show that 

$$
\mu \left(\bigcup_ {i = 1} ^ {n} A _ {i}\right) = \sum_ {J \subset \{1, \dots , n \}: J \neq \emptyset} (- 1) ^ {| J | - 1} \mu \left(\bigcap_ {i \in J} A _ {i}\right).
$$

(Hint: Compute Simp $\begin{array} { r } { \int _ { X } ( 1 - \prod _ { i = 1 } ^ { n } ( 1 - 1 _ { A _ { i } } ) ) } \end{array}$ dµ in two diferent ways.) 

Remark 1.4.36. The simple integral could also be defined on finitely additive measure spaces, rather than countably additive ones, and all the above properties would still apply. However, on a finitely additive measure space one would have dificulty extending the integral beyond simple functions, as we will now do. 

From the simple integral, we can now define the unsigned integral, in analogy to how the unsigned Lebesgue integral was constructed in Section 1.3.3. 

Definition 1.4.37. Let $( X , B , \mu )$ be a measure space, and let $f$ : $X \to [ 0 , + \infty ]$ be measurable. Then we define the unsigned integral $\textstyle \int _ { X } f  d \mu$ of f by the formula 

$$
\int_ {X} f d \mu := \sup _ {0 \leq g \leq f; g \text { simple }} \operatorname{Simp} \int_ {X} g d \mu .\tag{1.14}
$$

Clearly, this definition generalises Definition 1.3.13. Indeed, if $f$ : $\mathbf { R } ^ { d }  [ 0 , + \infty ]$ is Lebesgue measurable, then $\textstyle \int _ { \mathbf { R } ^ { d } } f ( x ) d x = \int _ { \mathbf { R } ^ { d } } f$ dm. 

We record some easy properties of this integral: 

Exercise 1.4.36 (Easy properties of the unsigned integral). Let $( X , B , \mu )$ be a measure space, and let $f , g : X \to [ 0 , + \infty ]$ be measurable. 

(i) (Almost everywhere equivalence) If $f = g$ µ-almost everywhere, then $\textstyle \int _ { X } f \ d \mu = \int _ { X } g \ d \mu$ 

(ii) (Monotonicity) If f ≤ g µ-almost everywhere, then $\int _ { X } f d \mu \leq$ $\textstyle \int _ { X } g \ d \mu$ 

(iii) (Homogeneity) We have $\textstyle { \int _ { X } c f ~ d \mu = c \int _ { X } f }$ dµ for every $c \in [ 0 , + \infty ]$ 

(iv) (Superadditivity) We have $\begin{array} { r } { \int _ { X } ( f + g ) \ d \mu \geq \int _ { X } f \ d \mu + \int _ { X } g \ d \mu . } \end{array}$ 

(v) (Compatibility with the simple integral) If f is simple, then $\textstyle \int _ { X } f \ d \mu = \operatorname { S i m p } \int _ { X } f \ d \mu .$ 

(vi) (Markov’s inequality) For any $0 < \lambda < \infty$ , one has 

$$
\mu (\{x \in X: f (x) \geq \lambda \}) \leq \frac {1}{\lambda} \int_ {X} f d \mu .
$$

In particular, if $\textstyle \int _ { X } f d \mu < \infty$ , then the sets $\{ x \in X : f ( x ) \geq$ $\lambda \}$ have finite measure for each $\lambda > 0$ 

(vii) (Finiteness) If $\textstyle \int _ { X } f d \mu < \infty$ , then $f ( x )$ is finite for µ-almost every x. 

(viii) (Vanishing) If $\textstyle \int _ { X } f  d \mu = 0$ , then $f ( x )$ is zero for µ-almost every x. 

(ix) (Vertical truncation) We have $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } \int _ { X } \operatorname* { m i n } ( f , n ) \ d \mu \ = } \end{array}$ $\textstyle \int _ { X } f \ d \mu .$ 

(x) (Horizontal truncation) If $E _ { 1 } \subset E _ { 2 } \subset . .$ . is an increasing sequence of B-measurable sets, then 

$$
\lim _ {n \to \infty} \int_ {X} f 1 _ {E _ {n}} d \mu = \int_ {X} f 1 _ {\bigcup_ {n = 1} ^ {\infty} E _ {n}} d \mu .
$$

(xi) (Restriction) If Y is a measurable subset of $X$ , then $\textstyle \int _ { X } f 1 _ { Y } d \mu =$ $\int _ { Y } f \mid _ { Y } d \mu \mid _ { Y }$ , where $f \ \lfloor \gamma \colon Y \to [ 0 , + \infty ]$ is the restriction of $f : X \to [ 0 , + \infty ]$ to $Y .$ , and the restriction $\mu \ \lfloor \gamma$ was defined in Example 1.4.25. We will often abbreviate $\textstyle \int _ { Y } f$ <sub>Y</sub> dµ $\lfloor \gamma$ (by slight abuse of notation) as $\int _ { Y } f \ d \mu$ 

As before, one of the key properties of this integral is its additivity: 

Theorem 1.4.38. Let $( X , B , \mu )$ be a measure space, and let $f , g$ $X \to [ 0 , + \infty ]$ be measurable. Then 

$$
\int_ {X} (f + g) d \mu = \int_ {X} f d \mu + \int_ {X} g d \mu .
$$

Proof. In view of superadditivity, it sufices to establish the subadditivity property 

$$
\int_ {X} (f + g) d \mu \leq \int_ {X} f d \mu + \int_ {X} g d \mu
$$

We establish this in stages. We first deal with the case when $\mu$ is a finite measure (which means that $\mu ( X ) < \infty )$ and $f , g$ are bounded. Pick an $\varepsilon > 0$ , and let $f _ { \varepsilon }$ be $f$ rounded down to the nearest integer multiple of $\varepsilon .$ , and $f ^ { \varepsilon }$ be $f$ rounded up to the nearest integer multiple. Clearly, we have the pointwise bounds 

$$
f _ {\varepsilon} (x) \leq f (x) \leq f ^ {\varepsilon} (x)
$$

and 

$$
f ^ {\varepsilon} (x) - f _ {\varepsilon} (x) \leq \varepsilon .
$$

Since $f$ is bounded, $f _ { \varepsilon }$ and $f ^ { \varepsilon }$ are simple. Similarly define $g _ { \varepsilon } , g ^ { \varepsilon }$ . We then have the pointwise bound 

$$
f + g \leq f ^ {\varepsilon} + g ^ {\varepsilon} \leq f _ {\varepsilon} + g _ {\varepsilon} + 2 \varepsilon ,
$$

hence by Exercise 1.4.36 and the properties of the simple integral, 

$$
\begin{array}{l} \int_ {X} f + g d \mu \leq \int_ {X} f _ {\varepsilon} + g _ {\varepsilon} + 2 \varepsilon d \mu \\ \qquad = \operatorname{Simp} \int_ {X} f _ {\varepsilon} + g _ {\varepsilon} + 2 \varepsilon d \mu \\ \qquad = \operatorname{Simp} \int_ {X} f _ {\varepsilon} d \mu + \operatorname{Simp} \int_ {X} g _ {\varepsilon} d \mu + 2 \varepsilon \mu (X). \end{array}
$$

From (1.14) we conclude that 

$$
\int_ {X} f + g d \mu \leq \int_ {X} f d \mu + \int_ {X} g d \mu + 2 \varepsilon \mu (X).
$$

Letting $\varepsilon \to 0$ and using the assumption that $\mu ( X )$ is finite, we obtain the claim. 

Now we continue to assume that $\mu$ is a finite measure, but now do not assume that $f , g$ are bounded. Then for any natural number $n ,$ we can use the previous case to deduce that 

$$
\int_ {X} \min (f, n) + \min (g, n) d \mu \leq \int_ {X} \min (f, n) d \mu + \int_ {X} \min (g, n) d \mu .
$$

Since min $( f + g , n ) \leq \operatorname* { m i n } ( f , n ) + \operatorname* { m i n } ( g , n )$ , we conclude that 

$$
\int_ {X} \min (f + g, n) \leq \int_ {X} \min (f, n) d \mu + \int_ {X} \min (g, n) d \mu .
$$

Taking limits as $n  \infty$ using vertical truncation, we obtain the claim. 

Finally, we no longer assume that $\mu$ is of finite measure, and also do not require $f , g$ to be bounded. If either $\textstyle \int _ { X } f$ dµ or $\textstyle \int _ { X } g \ d \mu$ is infinite, then by monotonicity, $\textstyle \int _ { X } f + g$ dµ is infinite as well, and the claim follows; so we may assume that $\textstyle \int _ { X } f$ dµ and $\textstyle \int _ { X } g$ dµ are both finite. By Markov’s inequality (Exercise $1 . 4 . 3 6 ( \mathrm { v i } ) )$ , we conclude that for each natural number $n ,$ the set $E _ { n } : = \{ x \in X : f ( x ) > { \frac { 1 } { n } } \} \cup \{ x \in$ $\begin{array} { r } { X : g ( x ) > \frac { 1 } { n } \rbrace } \end{array}$ has finite measure. These sets are increasing in $n ,$ , and $f , g , f + g$ are supported on $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n }$ , and so by horizontal truncation 

$$
\int_ {X} (f + g) d \mu = \lim _ {n \rightarrow \infty} \int_ {X} (f + g) 1 _ {E _ {n}} d \mu .
$$

From the previous case, we have 

$$
\int_ {X} (f + g) 1 _ {E _ {n}} d \mu \leq \int_ {X} f 1 _ {E _ {n}} d \mu + \int_ {X} g 1 _ {E _ {n}} d \mu .
$$

Letting $n \to \infty$ and using horizontal truncation we obtain the claim.  

Exercise 1.4.37 (Linearity in $\mu )$ . Let $( X , B , \mu )$ be a measure space, and let $f : X \to [ 0 , + \infty ]$ be measurable. 

(i) Show that $\textstyle { \int _ { X } f \ d ( c \mu ) = c \times \int _ { X } f }$ dµ for every $c \in [ 0 , + \infty ]$ 

(ii) If $\mu _ { 1 } , \mu _ { 2 } , \ldots .$ . are a sequence of measures on $B ,$ , show that 

$$
\int_ {X} f d \sum_ {n = 1} ^ {\infty} \mu_ {n} = \sum_ {n = 1} ^ {\infty} \int_ {X} f d \mu_ {n}.
$$

Exercise 1.4.38 (Change of variables formula). Let $( X , B , \mu )$ be a measure space, and let $\phi : X \to Y$ be a measurable morphism (as defined in Remark 1.4.33) from $( X , B )$ to another measurable space $( Y , { \mathcal { C } } )$ . Define the pushforward $\phi _ { * } \mu : { \mathcal { C } } \to [ 0 , + \infty ]$ of $\mu$ by $\phi$ by the formula $\phi _ { * } \mu ( E ) : = \mu ( \phi ^ { - 1 } ( E ) )$ . 

(i) Show that $\phi _ { * } \mu$ is a measure on ${ \mathcal { C } } ,$ so that $( Y , { \mathcal { C } } , \phi _ { * } \mu )$ is a measure space. 

(ii) If $f : Y  [ 0 , + \infty ]$ is measurable, show that $\textstyle \int _ { Y } f \ d \phi _ { * } \mu =$ $\textstyle \int _ { X } ( f \circ \phi ) \ d \mu$ 

(Hint: the quickest proof here is via the monotone convergence theorem (Theorem 1.4.44) below, but it is also possible to prove the exercise without this theorem.) 

Exercise 1.4.39. Let $T : \mathbf { R } ^ { d }  \mathbf { R } ^ { d }$ be an invertible linear transformation, and let $m$ be Lebesgue measure on $\mathbf { R } ^ { d }$ . Show that $T _ { * } m =$ ${ \frac { 1 } { | \operatorname* { d e t } T | } } m$ , where the pushforward $T _ { * } m$ of m was defined in Exercise 1.4.38. 

Exercise 1.4.40 (Sums as integrals). Let $X$ be an arbitrary set (with the discrete σ-algebra), let $\#$ be counting measure (see Exercise 1.4.26), and let $f : X \to [ 0 , + \infty ]$ be an arbitrary unsigned function. 

Show that $f$ is measurable with 

$$
\int_ {X} f d \# = \sum_ {x \in X} f (x).
$$

Once one has the unsigned integral, one can define the absolutely convergent integral exactly as in the Lebesgue case: 

Definition 1.4.39 (Absolutely convergent integral). Let $( X , B , \mu )$ be a measure space. A measurable function $f : X \to \mathbf { C }$ is said to be absolutely integrable if the unsigned integral 

$$
\| f \| _ {L ^ {1} (X, \mathcal {B}, \mu)} := \int_ {X} | f | d \mu
$$

is finite, and use $L ^ { 1 } ( X , B , \mu ) , \ L ^ { 1 } ( X )$ , or $L ^ { 1 } ( \mu )$ to denote the space of absolutely integrable functions. If f is real-valued and absolutely integrable, we define the integral $\textstyle \int _ { X } f  d \mu$ by the formula 

$$
\int_ {X} f d \mu := \int_ {X} f _ {+} d \mu - \int_ {X} f _ {-} d \mu
$$

where $f _ { + } : = \operatorname* { m a x } ( f , 0 ) , f _ { - } : = \operatorname* { m a x } ( - f , 0 )$ are the magnitudes of the positive and negative components of $f .$ . If $f$ is complex-valued and absolutely integrable, we define the integral $\textstyle \int _ { X } f$ dµ by the formula 

$$
\int_ {X} f d \mu := \int_ {X} \mathrm{Re} f d \mu + i \int_ {X} \mathrm{Im} f d \mu
$$

where the two integrals on the right are interpreted as real-valued integrals. It is easy to see that the unsigned, real-valued, and complexvalued integrals defined in this manner are compatible on their common domains of definition. 

Clearly, this definition generalises the Definition 1.3.17. 

We record some of the key facts about the absolutely convergent integral: 

Exercise 1.4.41. Let $( X , B , \mu )$ be a measure space. 

(i) Show that $L ^ { 1 } ( X , B , \mu )$ is a complex vector space. 

(ii) Show that the integration map $f \mapsto \textstyle \int _ { X } f$ dµ is a complexlinear map from $L ^ { 1 } ( X , B , \mu )$ to C. 

(iii) Establish the triangle inequality $\| f + g \| _ { L ^ { 1 } ( \mu ) } \leq \| f \| _ { L ^ { 1 } ( \mu ) } +$ $\| g \| _ { L ^ { 1 } ( \mu ) }$ and the homogeneity property $\| c f \| _ { L ^ { 1 } ( \mu ) } = | c | \| f \| _ { L ^ { 1 } ( \mu ) }$ for all $f , g \in L ^ { 1 } ( X , B , \mu )$ and $c \in \mathbf { C }$ 

(iv) Show that if $f , g \in L ^ { 1 } ( X , B , \mu )$ are such that $f ( x ) = g ( x )$ for µ-almost every $x \in X$ , then $\textstyle \int _ { X } f \ d \mu = \int _ { X } g \ d \mu .$ 

(v) If $f \in L ^ { 1 } ( X , B , \mu )$ , and $( X , B ^ { \prime } , \mu ^ { \prime } )$ is a refinement of $( X , B , \mu )$ then $f \in L ^ { 1 } ( X , B ^ { \prime } , \mu ^ { \prime } )$ , and $\textstyle \int _ { X } f \ d \mu ^ { \prime } = \int _ { X } f \ d \mu .$ . (Hint: it is easy to get one inequality. To get the other inequality, first work in the case when f is both bounded and has finite measure support (i.e. is both vertically and horizontally truncated).) 

(vi) Show that if $f \in L ^ { 1 } ( X , B , \mu )$ , then $\| f \| _ { L ^ { 1 } ( \mu ) } = 0$ if and only if f is zero µ-almost everywhere. 

(vii) If $Y \subset X$ is B-measurable and $f \in L ^ { 1 } ( X , B , \mu )$ , then $f \ \lfloor _ { Y } \in$ $L ^ { 1 } ( Y , B \downarrow _ { Y } , \mu \downarrow _ { Y } )$ and $\textstyle \int _ { Y } f \ \downarrow _ { Y } d \mu \ l _ { Y } = \ \int _ { X } f 1 _ { Y } \ d \mu$ . As before, by abuse of notation we write $\int _ { Y } f \ d \mu$ for $\textstyle \int _ { Y } f$ <sub>Y</sub> $d \mu \mid _ { Y }$ 

1.4.5. The convergence theorems. Let $( X , B , \mu )$ be a measure space, and let $f _ { 1 } , f _ { 2 } , \dots : X \to [ 0 , + \infty ]$ be a sequence of measurable functions. Suppose that as $n \to \infty , f _ { n } ( x )$ converges pointwise either everywhere, or µ-almost everywhere, to a measurable limit f. A basic question in the subject is to determine the conditions under which such pointwise convergence would imply convergence of the integral: 

$$
\int_ {X} f _ {n} d \mu \stackrel {?} {\rightarrow} \int_ {X} f d \mu .
$$

To put it another way: when can we ensure that one can interchange integrals and limits, 

$$
\lim _ {n \to \infty} \int_ {X} f _ {n} d \mu \stackrel {?} {=} \int_ {X} \lim _ {n \to \infty} f _ {n} d \mu ?
$$

There are certainly some cases in which one can safely do this: 

Exercise 1.4.42 (Uniform convergence on a finite measure space). Suppose that $( X , B , \mu )$ is a finite measure space (so $\mu ( X ) < \infty )$ , and $f _ { n } : X \to [ 0 , + \infty ]$ (resp. $f _ { n } : X \to \mathbf { C } )$ are a sequence of unsigned measurable functions (resp. absolutely integrable functions) 

that converge uniformly to a limit f. Show that $\int _ { X } f _ { n }$ dµ converges to $\textstyle \int _ { X } f  d \mu$ 

However, there are also cases in which one cannot interchange limits and integrals, even when the $f _ { n }$ are unsigned. We give the three classic examples, all of “moving bump” type, though the way in which the bump moves varies from example to example: 

Example 1.4.40 (Escape to horizontal infinity). Let X be the real line with Lebesgue measure, and let $f _ { n } : = 1 _ { [ n , n + 1 ] }$ . Then $f _ { n }$ converges pointwise to $f : = 0 .$ , but $\textstyle \int _ { \mathbf { R } } f _ { n } ( x ) \ d x \ = 1$ does not converge to $\textstyle \int _ { \mathbf { R } } f ( x ) \ d x = 0$ . Somehow, all the mass in the $f _ { n }$ has escaped by moving of to infinity in a horizontal direction, leaving none behind for the pointwise limit $f .$ 

Example 1.4.41 (Escape to width infinity). Let X be the real line with Lebesgue measure, and let $f _ { n } : = \frac { 1 } { n } 1 _ { [ 0 , n ] }$ . Then $f _ { n }$ now converges uniformly $f : = 0$ , but $\textstyle \int _ { \mathbf { R } } f _ { n } ( x )$ dx = 1 still does not converge to $\textstyle \int _ { \mathbf { R } } f ( x ) \ d x = 0$ . Exercise 1.4.42 would prevent this from happening if all the $f _ { n }$ were supported in a single set of finite measure, but the increasingly wide nature of the support of the $f _ { n }$ prevents this from happening. 

Example 1.4.42 (Escape to vertical infinity). Let X be the unit interval [0, 1] with Lebesgue measure (restricted from R), and let $f _ { n } : = n 1 _ { [ \frac { 1 } { n } , \frac { 2 } { n } ] }$ . Now, we have finite measure, and $f _ { n }$ converges pointwise to $f$ , but no uniform convergence. And again, $\textstyle \int _ { [ 0 , 1 ] } f _ { n } ( x ) d x = 1$ is not converging to $\begin{array} { r } { \int _ { [ 0 , 1 ] } f ( x ) \ d x = 0 } \end{array}$ . This time, the mass has escaped vertically, through the increasingly large values of $f _ { n }$ 

Remark 1.4.43. From the perspective of time-frequency analysis (or perhaps more accurately, space-frequency analysis), these three escapes are analogous (though not quite identical) to escape to spatial infinity, escape to zero frequency, and escape to infinite frequency respectively, thus describing the three diferent ways in which phase space fails to be compact (if one excises the zero frequency as being singular). 

However, once one shuts down these avenues of escape to infinity, it turns out that one can recover convergence of the integral. There are two major ways to accomplish this. One is to enforce monotonic-$i t y .$ , which prevents each $f _ { n }$ from abandoning the location where the mass of the preceding $f _ { 1 } , \ldots , f _ { n - 1 }$ was concentrated and which thus shuts down the above three escape scenarios. More precisely, we have the monotone convergence theorem: 

Theorem 1.4.44 (Monotone convergence theorem). Let $( X , B , \mu )$ be a measure space, and let $0 \leq f _ { 1 } \leq f _ { 2 } \leq . . .$ . be a monotone nondecreasing sequence of unsigned measurable functions on $X$ . Then we have 

$$
\lim _ {n \to \infty} \int_ {X} f _ {n} d \mu = \int_ {X} \lim _ {n \to \infty} f _ {n} d \mu .
$$

Note that in the special case when each $f _ { n }$ is an indicator function $f _ { n } = 1 _ { E _ { n } }$ , this theorem collapses to the upwards monotone convergence property (Exercise 1.4.23(ii)). Conversely, the upwards monotone convergence property will play a key role in the proof of this theorem. 

Proof. Write $f : = \mathrm { l i m } _ { n \to \infty } f _ { n } = \operatorname* { s u p } _ { n } f _ { n }$ , then $f : X \to [ 0 , + \infty ]$ is measurable. Since the $f _ { n }$ are non-decreasing to $f ,$ , we see from monotonicity that $\int _ { X } f _ { n }$ dµ are non-decreasing and bounded above by $\textstyle \int _ { X } f  d \mu$ , which gives the bound 

$$
\lim _ {n \to \infty} \int_ {X} f _ {n} d \mu \leq \int_ {X} f d \mu .
$$

It remains to establish the reverse inequality 

$$
\int_ {X} f d \mu \leq \lim _ {n \rightarrow \infty} \int_ {X} f _ {n} d \mu .
$$

By definition, it sufices to show that 

$$
\int_ {X} g d \mu \leq \lim _ {n \rightarrow \infty} \int_ {X} f _ {n} d \mu .
$$

whenever $g$ is a simple function that is bounded pointwise by $f .$ . By vertical truncation we may assume without loss of generality that $g$ also is finite everywhere, then we can write 

$$
g = \sum_ {i = 1} ^ {k} c _ {i} 1 _ {A _ {i}}
$$

for some $0 \leq c _ { i } < \infty$ and some disjoint $B .$ -measurable sets $A _ { 1 } , \ldots , A _ { k }$ , thus 

$$
\int_ {X} g d \mu = \sum_ {i = 1} ^ {k} c _ {i} \mu (A _ {i}).
$$

Let $0 < \varepsilon < 1$ be arbitrary. Then we have 

$$
f (x) = \sup _ {n} f _ {n} (x) > (1 - \varepsilon) c _ {i}
$$

for all $x \in A _ { i }$ . Thus, if we define the sets 

$$
A _ {i, n} := \{x \in A _ {i}: f _ {n} (x) > (1 - \varepsilon) c _ {i} \}
$$

then the $A _ { i , n }$ increase to $A _ { i }$ and are measurable. By upwards monotonicity of measure, we conclude that 

$$
\lim _ {n \to \infty} \mu (A _ {i, n}) = \mu (A _ {i}).
$$

On the other hand, observe the pointwise bound 

$$
f _ {n} \geq \sum_ {i = 1} ^ {k} (1 - \varepsilon) c _ {i} 1 _ {A _ {i, n}}
$$

for any $n ;$ integrating this, we obtain 

$$
\int_ {X} f _ {n} d \mu \geq (1 - \varepsilon) \sum_ {i = 1} ^ {k} c _ {i} \mu (A _ {i, n}).
$$

Taking limits as $n \to \infty$ , we obtain 

$$
\lim _ {n \rightarrow \infty} \int_ {X} f _ {n} d \mu \geq (1 - \varepsilon) \sum_ {i = 1} ^ {k} c _ {i} \mu (A _ {i});
$$

sending $\varepsilon \to 0$ we then obtain the claim. 

Remark 1.4.45. It is easy to see that the result still holds if the monotonicity $f _ { n } \leq f _ { n + 1 }$ only holds almost everywhere rather than everywhere. 

This has a number of important corollaries. Firstly, we can generalise (part of) Tonelli’s theorem for exchanging sums (see Theorem 0.0.2): 

Corollary 1.4.46 (Tonelli’s theorem for sums and integrals). Let $( X , B , \mu )$ be a measure space, and let $f _ { 1 } , f _ { 2 } , \ldots : X \to [ 0 , + \infty ]$ be a sequence of unsigned measurable functions. Then one has 

$$
\int_ {X} \sum_ {n = 1} ^ {\infty} f _ {n} d \mu = \sum_ {n = 1} ^ {\infty} \int_ {X} f _ {n} d \mu .
$$

Proof. Apply the monotone convergence theorem (Theorem 1.4.44) to the partial sums $\begin{array} { r } { F _ { N } : = \sum _ { n = 1 } ^ { N } f _ { n } } \end{array}$  

Exercise 1.4.43. Give an example to show that this corollary can fail if the $f _ { n }$ are assumed to be absolutely integrable rather than unsigned measurable, even if the sum $\textstyle \sum _ { n = 1 } ^ { \infty } f _ { n } ( x )$ is absolutely convergent for each x. (Hint: think about the three escapes to infinity.) 

Exercise 1.4.44 (Borel-Cantelli lemma). Let $( X , B , \mu )$ be a measure space, and let $E _ { 1 } , E _ { 2 } , E _ { 3 } , . . .$ . be a sequence of B-measurable sets such that $\textstyle \sum _ { n = 1 } ^ { \infty } \mu ( E _ { n } ) < \infty$ . Show that almost every $x \in X$ is contained in at most finitely many of the $E _ { n } { \mathrm { ~ } } ( { \mathrm { i . e . ~ } } \left\{ n \in \mathbf { N } : x \in E _ { n } \right\}$ is finite for almost every $x \in X )$ . (Hint: Apply Tonelli’s theorem to the indicator functions $1 _ { E _ { n } \cdot } )$ 

Exercise 1.4.45. 

(i) Give an alternate proof of the Borel-Cantelli lemma (Exercise 1.4.44) that does not go through any of the convergence theorems, but instead exploits the more basic properties of measure from Exercise 1.4.23. 

(ii) Give a counterexample that shows that the Borel-Cantelli lemma can fail if the condition $\textstyle \sum _ { n = 1 } ^ { \infty } \mu ( E _ { n } ) < \infty$ is relaxed to $\begin{array} { r } { \operatorname* { l i m } _ { n \to \infty } \mu ( E _ { n } ) = 0 } \end{array}$ 

Secondly, when one does not have monotonicity, one can at least obtain an important inequality, known as Fatou’s lemma: 

Corollary 1.4.47 (Fatou’s lemma). Let $( X , B , \mu )$ be a measure space, and let $f _ { 1 } , f _ { 2 } , \dots : X \to [ 0 , + \infty ]$ be a sequence of unsigned measurable functions. Then 

$$
\int_ {X} \operatorname * {l i m i n f} _ {n \to \infty} f _ {n} d \mu \leq \operatorname * {l i m i n f} _ {n \to \infty} \int_ {X} f _ {n} d \mu .
$$

Proof. Write $F _ { N } : = \operatorname* { i n f } _ { n \geq N } f _ { n }$ for each N. Then the $F _ { N }$ are measurable and non-decreasing, and hence by the monotone convergence theorem (Theorem 1.4.44) 

$$
\int_ {X} \sup _ {N > 0} F _ {N} d \mu = \sup _ {N > 0} \int_ {X} F _ {N} d \mu .
$$

By definition of lim inf, we have su ${ } _ { N > 0 } F _ { N } = \operatorname* { l i m } \operatorname* { i n f } _ { n \to \infty } f _ { n }$ . By monotonicity, we have $\textstyle \int _ { X } F _ { N } ~ d \mu \leq \int _ { X } f _ { n }$ dµ for all $n \geq N$ , and thus 

$$
\int_ {X} F _ {N} d \mu \leq \inf _ {n \geq N} \int_ {X} f _ {n} d \mu .
$$

Hence we have 

$$
\int_ {X} \operatorname * {l i m i n f} _ {n \to \infty} f _ {n} d \mu \leq \sup _ {N > 0} \inf _ {n \geq N} \int_ {X} f _ {n} d \mu .
$$

The claim then follows by another appeal to the definition of the lim inferior.  

Remark 1.4.48. Informally, Fatou’s lemma tells us that when taking the pointwise limit of unsigned functions $f _ { n }$ , that mass $\int _ { X } f _ { n }$ dµ can be destroyed in the limit (as was the case in the three key moving bump examples), but it cannot be created in the limit. Of course the unsigned hypothesis is necessary here (consider for instance multiplying any of the moving bump examples by −1). While this lemma was stated only for pointwise limits, the same general principle (that mass can be destroyed, but not created, by the process of taking limits) tends to hold for other “weak” notions of convergence. See §1.9 of An epsilon of room, Vol. I for some examples of this. 

Finally, we give the other major way to shut down loss of mass via escape to infinity, which is to dominate all of the functions involved by an absolutely convergent one. This result is known as the dominated convergence theorem: 

Theorem 1.4.49 (Dominated convergence theorem). Let $( X , B , \mu )$ be a measure space, and let $f _ { 1 } , f _ { 2 } , \ldots : X \to \mathbf { C }$ be a sequence of measurable functions that converge pointwise µ-almost everywhere to a measurable limit $f : X \to \mathbf { C }$ . Suppose that there is an unsigned absolutely integrable function $G : X  [ 0 , + \infty ]$ such that $\left| f _ { n } \right|$ are pointwise µ-almost everywhere bounded by G for each n. Then we have 

$$
\lim _ {n \to \infty} \int_ {X} f _ {n} d \mu = \int_ {X} f d \mu .
$$

From the moving bump examples we see that this statement fails if there is no absolutely integrable dominating function G. The reader is encouraged to see why, in each of the moving bump examples, no such dominating function exists, without appealing to the above theorem. Note also that when each of the $f _ { n }$ is an indicator function $f _ { n } = 1 _ { E _ { n } }$ , the dominated convergence theorem collapses to Exercise 1.4.24. 

Proof. By modifying $f _ { n } , f$ on a null set, we may assume without loss of generality that the $f _ { n }$ converge to f pointwise everywhere rather than µ-almost everywhere, and similarly we can assume that $\left| f _ { n } \right.$ are bounded by G pointwise everywhere rather than µ-almost everywhere. 

By taking real and imaginary parts we may assume without loss of generality that $f _ { n } , f$ are real, thus $- G \leq f _ { n } \leq G$ pointwise. Of course, this implies that $- G \leq f \leq G$ pointwise also. 

If we apply Fatou’s lemma (Corollary1.4.47) to the unsigned functions $f _ { n } + G$ , we see that 

$$
\int_ {X} f + G d \mu \leq \operatorname * {l i m i n f} _ {n \to \infty} \int_ {X} f _ {n} + G d \mu ,
$$

which on subtracting the finite quantity $\textstyle \int _ { X } G$ dµ gives 

$$
\int_ {X} f d \mu \leq \operatorname * {l i m i n f} _ {n \to \infty} \int_ {X} f _ {n} d \mu .
$$

Similarly, if we apply that lemma to the unsigned functions $G - f _ { n }$ , we obtain 

$$
\int_ {X} G - f d \mu \leq \operatorname * {l i m i n f} _ {n \to \infty} \int_ {X} G - f _ {n} d \mu ;
$$

negating this inequality and then cancelling $\textstyle \int _ { X } G \ d \mu$ again we conclude that 

$$
\limsup _ {n \to \infty} \int_ {X} f _ {n} d \mu \leq \int_ {X} f d \mu .
$$

The claim then follows by combining these inequalities. 

Remark 1.4.50. We deduced the dominated convergence theorem from Fatou’s lemma, and Fatou’s lemma from the monotone convergence theorem. However, one can obtain these theorems in a diferent order, depending on one’s taste, as they are so closely related. For instance, in [StSk2005], the logic is somewhat diferent; one first obtains the slightly simpler bounded convergence theorem, which is the dominated convergence theorem under the assumption that the functions are uniformly bounded and all supported on a single set of finite measure, and then uses that to deduce Fatou’s lemma, which in turn is used to deduce the monotone convergence theorem; and then the horizontal and vertical truncation properties are used to extend the bounded convergence theorem to the dominated convergence theorem. It is instructive to view a couple diferent derivations of these key theorems to get more of an intuitive understanding as to how they work. 

Exercise 1.4.46. Under the hypotheses of the dominated convergence theorem (Theorem 1.4.49), establish also that $\| f _ { n } - f \| _ { L ^ { 1 } } \to 0$ as $n \to \infty$ 

Exercise 1.4.47 (Almost dominated convergence). Let $( X , B , \mu )$ be a measure space, and let $f _ { 1 } , f _ { 2 } , \ldots : X \to \mathbf { C }$ be a sequence of measurable functions that converge pointwise µ-almost everywhere to a measurable limit $f : X \to \mathbf { C } .$ . Suppose that there is an unsigned absolutely integrable functions $G , g _ { 1 } , g _ { 2 } , . . . : X \to [ 0 , + \infty ]$ such that the $\left| f _ { n } \right|$ are pointwise µ-almost everywhere bounded by $G + g _ { n }$ , and that $\textstyle \int _ { X } g _ { n } \ d \mu \to 0$ as $n \to \infty$ . Show that 

$$
\lim _ {n \to \infty} \int_ {X} f _ {n} d \mu = \int_ {X} f d \mu .
$$

Exercise 1.4.48 (Defect version of Fatou’s lemma). Let $( X , B , \mu )$ be a measure space, and let $f _ { 1 } , f _ { 2 } , \ldots : X \to [ 0 , + \infty ]$ be a sequence of unsigned absolutely integrable functions that converges pointwise to an absolutely integrable limit $f .$ . Show that 

$$
\int_ {X} f _ {n} d \mu - \int_ {X} f d \mu - \| f - f _ {n} \| _ {L ^ {1} (\mu)} \rightarrow 0
$$

as $n \to \infty$ . (Hint: Apply the dominated convergence theorem (Theorem 1.4.49) to min $( f _ { n } , f ) . )$ Informally, this tells us that the gap between the left and right hand sides of Fatou’s lemma can be measured by the quantity $\| f - f _ { n } \| _ { L ^ { 1 } ( \mu ) }$ 

Exercise 1.4.49. Let $( X , B , \mu )$ be a measure space, and let $g : X $ $[ 0 , + \infty ]$ be measurable. Show that the function $\mu _ { g } : B \to [ 0 , + \infty ]$ defined by the formula 

$$
\mu_ {g} (E) := \int_ {X} 1 _ {E} g d \mu = \int_ {E} g d \mu
$$

is a measure. (Such measures are studied in greater detail in §1.2 of An epsilon of room, Vol. I.) 

The monotone convergence theorem is, in some sense, a defining property of the unsigned integral, as the following exercise illustrates. 

Exercise 1.4.50 (Characterisation of the unsigned integral). Let $( X , B )$ be a measurable space. $I : f \mapsto I ( f )$ be a map from the space $\boldsymbol { \mathcal { U } } ( \boldsymbol { X } , \boldsymbol { B } )$ of unsigned measurable functions $f : X \to [ 0 , + \infty ]$ to $[ 0 , + \infty ]$ that obeys the following axioms: 

(i) (Homogeneity) For every $f \in \mathcal { U } ( X , B )$ and $c \in [ 0 , + \infty ]$ ], one has $I ( c f ) = c I ( f )$ 

(ii) (Finite additivity) For every $f , g \in \mathcal { U } ( X , B )$ , one has $I ( f +$ $g ) = I ( f ) + I ( g )$ 

(iii) (Monotone convergence) If $0 \leq f _ { 1 } \leq f _ { 2 } \leq . . .$ . are a nondecreasing sequence of unsigned measurable functions, then $\begin{array} { r } { I ( \operatorname* { l i m } _ { n \to \infty } f _ { n } ) = \operatorname* { l i m } _ { n \to \infty } I ( f _ { n } ) } \end{array}$ 

Then there exists a unique measure $\mu$ on $( X , B )$ such that $I ( f ) =$ $\textstyle \int _ { X } f  d \mu$ for all $f \in \mathcal { U } ( X , B )$ . Furthermore, $\mu$ is given by the formula $\mu ( E ) : = I ( 1 _ { E } )$ for all B-measurable sets $E$ 

Exercise 1.4.51. Let $( X , B , \mu )$ be a finite measure space $( \mathrm { i . e . } \ \mu ( X ) <$ $\infty )$ , and let $f : X \to \mathbf { R }$ be a bounded function. Suppose that $\mu$ is complete (see Definition 1.4.31). Suppose that the upper integral 

$$
\overline {{\int}} _ {X} f d \mu := \inf _ {g \geq f; g \text {simple}} \int_ {X} g d \mu
$$

and lower integral 

$$
\int_ {\underline {{X}}} f d \mu := \sup _ {h \leq f; h \text {   simple }} \int_ {X} h d \mu
$$

agree. Show that $f$ is measurable. (This is a converse to Exercise 1.3.11.) 

We will continue to see the monotone convergence theorem, Fatou’s lemma, and the dominated convergence theorem make an appearance throughout the rest of this text (and in An epsilon of room, Vol. I). 

## 1.5. Modes of convergence

If one has a sequence $x _ { 1 } , x _ { 2 } , x _ { 3 } , . . . \in \textbf { R }$ of real numbers $x _ { n }$ , it is unambiguous what it means for that sequence to converge to a limit $x \in \mathbf { R }$ : it means that for every $\varepsilon > 0$ , there exists an N such that $| x _ { n } - x | \leq \varepsilon$ for all $n > N$ . Similarly for a sequence $z _ { 1 } , z _ { 2 } , z _ { 3 } , . . . \in \mathbf { C }$ of complex numbers $z _ { n }$ converging to a limit $z \in \mathbf { C }$ 

More generally, if one has a sequence $v _ { 1 } , v _ { 2 } , v _ { 3 } , . . .$ . of d-dimensional vectors $v _ { n }$ in a real vector space $\mathbf { R } ^ { d }$ or complex vector space $\mathbf { C } ^ { d }$ , it is also unambiguous what it means for that sequence to converge to a limit $\boldsymbol { v } ~ \in ~ \mathbf { R } ^ { d }$ or $v \in \mathbf { C } ^ { d } ;$ ; it means that for every $\varepsilon \ > \ 0$ , there exists an $N$ such that $\| v _ { n } - v \| \ \leq \varepsilon$ for all $n \geq N$ . Here, the norm $\lVert v \rVert$ of a vector $v = ( v ^ { ( 1 ) } , \ldots , v ^ { ( d ) } )$ can be chosen to be the Euclidean norm $\begin{array} { r } { \| \boldsymbol { v } \| _ { 2 } : = ( \sum _ { j = 1 } ^ { d } ( \boldsymbol { v } ^ { ( j ) } ) ^ { 2 } ) ^ { 1 / 2 } } \end{array}$ , the supremum norm $\begin{array} { r } { \| v \| _ { \infty } : = \operatorname* { s u p } _ { 1 \leq j \leq d } | v ^ { ( j ) } | } \end{array}$ , or any other number of norms, but for the purposes of convergence, these norms are all equivalent; a sequence of vectors converges in the Euclidean norm if and only if it converges in the supremum norm, and similarly for any other two norms on the finite-dimensional space $\mathbf { R } ^ { d }$ or $\mathbf { C } ^ { d }$ 

If however one has a sequence $f _ { 1 } , f _ { 2 } , f _ { 3 } , \ldots$ . of functions $f _ { n } : X \to$ R or $f _ { n } : X \to \mathbf { C }$ on a common domain $X$ , and a putative limit $f : X \to \mathbf { R }$ or $f : X \to \mathbf { C }$ , there can now be many diferent ways in which the sequence $f _ { n }$ may or may not converge to the limit $f .$ . (One could also consider convergence of functions $f _ { n } : X _ { n } \to \mathbf { C }$ on diferent domains $X _ { n }$ , but we will not discuss this issue at all here.) This is contrast with the situation with scalars $x _ { n }$ or $z _ { n }$ (which corresponds to the case when X is a single point) or vectors $v _ { n }$ (which corresponds to the case when X is a finite set such as $\{ 1 , \ldots , d \} )$ . Once X becomes infinite, the functions $f _ { n }$ acquire an infinite number of degrees of freedom, and this allows them to approach $f$ in any number of inequivalent ways. 

What diferent types of convergence are there? As an undergrad uate, one learns of the following two basic modes of convergence: 

(i) We say that $f _ { n }$ converges to f pointwise if, for every $x \in X$ $f _ { n } ( x )$ converges to $f ( x )$ . In other words, for every $\varepsilon > 0$ and $x \in X$ , there exists N (that depends on both $\varepsilon$ and x) such that $| f _ { n } ( x ) - f ( x ) | \leq \varepsilon$ whenever $n \geq N$ 

(ii) We say that $f _ { n }$ converges to f uniformly if, for every $\varepsilon > 0$ there exists N such that for every $n \geq N , | f _ { n } ( x ) - f ( x ) | \leq \varepsilon$ for every $x \in X$ . The diference between uniform convergence and pointwise convergence is that with the former, the time N at which $f _ { n } ( x )$ must be permanently ε-close to $f ( x )$ is not permitted to depend on $x _ { \ast }$ , but must instead be chosen uniforml in $x .$ 

Uniform convergence implies pointwise convergence, but not conversely. A typical example: the functions $f _ { n } : \mathbf { R }  \mathbf { R }$ defined by $f _ { n } ( x ) : = x / n$ converge pointwise to the zero function $f ( x ) : = 0$ , but not uniformly. 

However, pointwise and uniform convergence are only two of dozens of many other modes of convergence that are of importance in analysis. We will not attempt to exhaustively enumerate these modes here (but see §1.9 of An epsilon of room, Vol. I). We will, however, discuss some of the modes of convergence that arise from measure theory, when the domain X is equipped with the structure of a measure space $( X , B , \mu )$ , and the functions $f _ { n }$ (and their limit f) are measurable with respect to this space. In this context, we have some additional modes of convergence: 

(i) We say that $f _ { n }$ converges to f pointwise almost everywhere if, for $( \mu - )$ almost everywhere $x \in X , f _ { n } ( x )$ converges to $f ( x )$ 

(ii) We say that $f _ { n }$ converges to f uniformly almost everywhere, essentially uniformly, or in $L ^ { \infty }$ norm if, for every $\varepsilon > 0$ there exists N such that for every $n \geq N , | f _ { n } ( x ) - f ( x ) | \leq \varepsilon$ for µ-almost every $x \in X$ 

(iii) We say that $f _ { n }$ converges to f almost uniformly if, for every $\varepsilon > 0$ , there exists an exceptional set $E \in B$ of measure $\mu ( E ) \ \leq \ \varepsilon$ such that $f _ { n }$ converges uniformly to $f$ on the complement of E. 

(iv) We say that $f _ { n }$ converges to f in $L ^ { 1 }$ norm if the quantity $\begin{array} { r } { \| f _ { n } - f \| _ { L ^ { 1 } ( \mu ) } = \int _ { X } | f _ { n } ( x ) - f ( x ) | } \end{array}$ dµ converges to 0 as $n $ ∞. 

(v) We say that $f _ { n }$ converges to f in measure if, for every $\varepsilon > 0$ the measures $\mu ( \{ x \in X : | f _ { n } ( x ) - f ( x ) | \geq \varepsilon \} )$ ) converge to zero as $n \to \infty$ 

Observe that each of these five modes of convergence is unafected if one modifies $f _ { n }$ or $f$ on a set of measure zero. In contrast, the pointwise and uniform modes of convergence can be afected if one modifies $f _ { n }$ or $f$ even on a single point. The $L ^ { 1 }$ and $L ^ { \infty }$ modes of converges are special cases of the $L ^ { p }$ mode of convergence, which is discussed in §1.3 of An epsilon of room, Vol. I. 

Remark 1.5.1. In the context of probability theory (see Section 2.3), in which $f _ { n }$ and f are interpreted as random variables, convergence in $L ^ { 1 }$ norm is often referred to as convergence in mean, pointwise convergence almost everywhere is often referred to as almost sure convergence, and convergence in measure is often referred to as convergence in probability. 

Exercise 1.5.1 (Linearity of convergence). Let $( X , B , \mu )$ be a measure space, let $f _ { n } , g _ { n } : X \to \mathbf { C }$ be sequences of measurable functions, and let $f , g : X \to \mathbf { C }$ be measurable functions. 

(i) Show that $f _ { n }$ converges to f along one of the above seven modes of convergence if and only if $\left| f _ { n } - f \right|$ converges to 0 along the same mode. 

(ii) If $f _ { n }$ converges to f along one of the above seven modes of convergence, and $g _ { n }$ converges to g along the same mode, show that $f _ { n } + g _ { n }$ converges to $f + g$ along the same mode, and that $c f _ { n }$ converges to cf along the same mode for any $c \in \mathbf { C }$ 

(iii) (Squeeze test) If $f _ { n }$ converges to 0 along one of the above seven modes, and $| g _ { n } | \leq f _ { n }$ pointwise for each $n .$ , show that $g _ { n }$ converges to 0 along the same mode. 

We have some easy implications between modes: 

Exercise 1.5.2 (Easy implications). Let $( X , B , \mu )$ be a measure space, and let $f _ { n } : X \to \mathbf { C }$ and $f : X \to \mathbf { C }$ be measurable functions. 

(i) If $f _ { n }$ converges to f uniformly, then $f _ { n }$ converges to f pointwise. 

(ii) If $f _ { n }$ converges to f uniformly, then $f _ { n }$ converges to $f$ in $L ^ { \infty }$ norm. Conversely, if $f _ { n }$ converges to f in $L ^ { \infty }$ norm, then $f _ { n }$ converges to f uniformly outside of a null set (i.e. there exists a null set E such that the restriction $f _ { n } \mid _ { X \backslash E }$ of $f _ { n }$ to the complement of $E$ converges to the restriction $f \ \lfloor _ { X \backslash E }$ of $f )$ . 

(iii) If $f _ { n }$ converges to $f$ in $L ^ { \infty }$ norm, then $f _ { n }$ converges to $f$ almost uniformly. 

(iv) If $f _ { n }$ converges to f almost uniformly, then $f _ { n }$ converges to f pointwise almost everywhere. 

(v) If $f _ { n }$ converges to f pointwise, then $f _ { n }$ converges to f pointwise almost everywhere. 

(vi) If $f _ { n }$ converges to $f$ in $L ^ { 1 }$ norm, then $f _ { n }$ converges to $f$ in measure. 

(vii) If $f _ { n }$ converges to f almost uniformly, then $f _ { n }$ converges to $f$ in measure. 

The reader is encouraged to draw a diagram that summarises the logical implications between the seven modes of convergence that the above exercise describes. 

We give four key examples that distinguish between these modes, in the case when X is the real line R with Lebesgue measure. The first three of these examples already were introduced in Section 1.4, but the fourth is new, and also important. 

Example 1.5.2 (Escape to horizontal infinity). Let $f _ { n } : = 1 _ { [ n , n + 1 ] }$ Then $f _ { n }$ converges to zero pointwise (and thus, pointwise almost everywhere), but not uniformly, in $L ^ { \infty }$ norm, almost uniformly, in $L ^ { 1 }$ norm, or in measure. 

Example 1.5.3 (Escape to width infinity). Let $f _ { n } : = \frac { 1 } { n } 1 _ { [ 0 , n ] }$ . Then $f _ { n }$ converges to zero uniformly (and thus, pointwise, pointwise almost everywhere, in $L ^ { \infty }$ norm, almost uniformly, and in measure), but not in $L ^ { 1 }$ norm. 

Example 1.5.4 (Escape to vertical infinity). Let $f _ { n }     : = n 1 _ { [ \frac { 1 } { n } , \frac { 2 } { n } ] }$ Then $f _ { n }$ converges to zero pointwise (and thus, pointwise almost everywhere) and almost uniformly (and hence in measure), but not uniformly, in $L ^ { \infty }$ norm, or in $L ^ { 1 }$ norm. 

Example 1.5.5 (Typewriter sequence). Let $f _ { n }$ be defined by the formula 

$$
f _ {n} := 1 _ {[ \frac {n - 2 ^ {k}}{2 ^ {k}}, \frac {n - 2 ^ {k} + 1}{2 ^ {k}} ]}
$$

whenever $k \geq 0$ and $2 ^ { k } \leq n < 2 ^ { k + 1 }$ . This is a sequence of indicator functions of intervals of decreasing length, marching across the unit interval [0, 1] over and over again. Then $f _ { n }$ converges to zero in measure and in $L ^ { 1 }$ norm, but not pointwise almost everywhere (and hence also not pointwise, not almost uniformly, nor in $L ^ { \infty }$ norm, nor uniformly). 

Remark 1.5.6. The $L ^ { \infty }$ norm $\| f \| _ { L ^ { \infty } ( \mu ) }$ of a measurable function $f : X \to \mathbf { C }$ is defined to the infimum of all the quantities $M \in [ 0 , + \infty ]$ that are essential upper bounds for $f$ in the sense that $| f ( x ) | \leq M$ for almost every x. Then $f _ { n }$ converges to $f$ in $L ^ { \infty }$ norm if and only if $\| f _ { n } - f \| _ { L ^ { \infty } ( \mu ) } \to 0$ as $n \to \infty$ . The $L ^ { \infty }$ and $L ^ { 1 }$ norms are part of the larger family of $L ^ { p }$ norms, studied in $\ S 1 . 3$ of An epsilon of room, Vol. I. 

One particular advantage of $L ^ { 1 }$ convergence is that, in the case when the $f _ { n }$ are absolutely integrable, it implies convergence of the integrals, 

$$
\int_ {X} f _ {n} d \mu \rightarrow \int_ {X} f d \mu ,
$$

as one sees from the triangle inequality. Unfortunately, none of the other modes of convergence automatically imply this convergence of the integral, as the above examples show. 

The purpose of these notes is to compare these modes of convergence with each other. Unfortunately, the relationship between these modes is not particularly simple; unlike the situation with pointwise and uniform convergence, one cannot simply rank these modes in a linear order from strongest to weakest. This is ultimately because the diferent modes react in diferent ways to the three “escape to infinity” scenarios described above, as well as to the “typewriter” behaviour when a single set is “overwritten” many times. On the other hand, if one imposes some additional assumptions to shut down one or more of these escape to infinity scenarios, such as a finite measure hypothesis $\mu ( X ) < \infty$ or a uniform integrability hypothesis, then one can obtain some additional implications between the diferent modes. 

1.5.1. Uniqueness. Throughout these notes, $( X , B , \mu )$ denotes a measure space. We abbreviate “µ-almost everywhere” as “almost everywhere” throughout. 

Even though the modes of convergence all difer from each other, they are all compatible in the sense that they never disagree about which function $f$ a sequence of functions $f _ { n }$ converges to, outside of a set of measure zero. More precisely: 

Proposition 1.5.7. Let $f _ { n } : X \to \mathbf { C }$ be a sequence of measurable functions, and let $f , g : X \to \mathbf { C }$ be two additional measurable functions. Suppose that $f _ { n }$ converges to f along one of the seven modes of convergence defined above, and $f _ { n }$ converges to g along another of the seven modes of convergence (or perhaps the same mode of convergence as $f o r \ f )$ . Then f and g agree almost everywhere. 

Note that the conclusion is the best one can hope for in the case of the last five modes of convergence, since as remarked earlier, these modes of convergence are unafected if one modifies $f$ or g on a set of measure zero. 

Proof. In view of Exercise 1.5.2, we may assume that $f _ { n }$ converges to $f$ either pointwise almost everywhere, or in measure, and similarly that $f _ { n }$ converges to $g$ either pointwise almost everywhere, or in measure. 

Suppose first that $f _ { n }$ converges to both $f$ and g pointwise almost everywhere. Then by Exercise 1.5.1, 0 converges to $f - g$ pointwise almost everywhere, which clearly implies that $f - g$ is zero almost everywhere, and the claim follows. A similar argument applies if $f _ { n }$ converges to both $f$ and g in measure. 

By symmetry, the only remaining case that needs to be considered is when $f _ { n }$ converges to $f$ pointwise almost everywhere, and $f _ { n }$ converges to $g$ in measure. We need to show that $f = g$ almost everywhere. It sufices to show that for every $\varepsilon > 0$ , that $| f ( x ) - g ( x ) | \leq \varepsilon$ for almost every $x ,$ , as the claim then follows by setting $\varepsilon = 1 / m$ for $m = 1 , 2 , 3 , . . .$ . and using the fact that the countable union of null sets is again a null set. 

Fix $\varepsilon > 0$ , and let $A : = \{ x \in X : | f ( x ) - g ( x ) | > \varepsilon \}$ . This is a measurable set; our task is to show that it has measure zero. Suppose for contradiction that $\mu ( A ) > 0$ . We consider the sets 

$$
A _ {N} := \{x \in A: | f _ {n} (x) - f (x) | \leq \varepsilon / 2 \text {   for   all   } n \geq N \}.
$$

These are measurable sets that are increasing in N. As $f _ { n }$ converges to $f$ almost everywhere, we see that almost every $x \in A$ belongs to at least one of the $A _ { N }$ , thus $\textstyle \bigcup _ { N = 1 } ^ { \infty } A _ { N }$ is equal to A outside of a nul 

set. In particular, 

$$
\mu (\bigcup_ {N = 1} ^ {\infty} A _ {N}) > 0.
$$

Applying monotone convergence for sets, we conclude that 

$$
\mu (A _ {N}) > 0
$$

for some finite N. But by the triangle inequality, we have $| f _ { n } ( x ) -$ $g ( x ) | > \varepsilon / 2$ for all $x \in A _ { N }$ and all $n \geq N$ . As a consequence, $f _ { n }$ cannot converge in measure to $g _ { ; }$ , which gives the desired contradiction.  

1.5.2. The case of a step function. One way to appreciate the distinctions between the above modes of convergence is to focus on the case when $f = 0$ , and when each of the $f _ { n }$ is a step function, by which we mean a constant multiple $f _ { n } = A _ { n } 1 _ { E _ { n } }$ of a measurable set $E _ { n }$ . For simplicity we will assume that the $A _ { n } \mathrm { ~ > ~ } 0$ are positive reals, and that the $E _ { n }$ have a positive measure $\mu ( E _ { n } ) > 0$ . We also assume the $A _ { n }$ exhibit one of two modes of behaviour: either the $A _ { n }$ converge to zero, or else they are bounded away from zero (i.e. there exists $c > 0$ such that $A _ { n } \geq c$ for every n. It is easy to see that if a sequence $A _ { n }$ does not converge to zero, then it has a subsequence that is bounded away from zero, so it does not cause too much loss of generality to restrict to one of these two cases. 

Given such a sequence $f _ { n } = A _ { n } 1 _ { E _ { n } }$ of step functions, we now ask, for each of the seven modes of convergence, what it means for this sequence to converge to zero along that mode. It turns out that the answer to question is controlled more or less completely by the following three quantities: 

(i) The height $A _ { n }$ of the $n ^ { t h }$ function $f _ { n }$ ; 

(ii) The width $\mu ( E _ { n } )$ of the $n ^ { t h }$ function $f _ { n } i$ ; and 

(iii) The $N ^ { t h }$ tail support $\begin{array} { r } { E _ { N } ^ { * } \ : = \ \bigcup _ { n > N } E _ { n } } \end{array}$ of the sequence $f _ { 1 } , f _ { 2 } , f _ { 3 } ,$ 

Indeed, we have: 

Exercise 1.5.3 (Convergence for step functions). Let the notation and assumptions be as above. Establish the following claims: 

(i) $f _ { n }$ converges uniformly to zero if and only if $A _ { n } \  \ 0$ as $n \to \infty$ 

(ii) $f _ { n }$ converges in $L ^ { \infty }$ norm to zero if and only if $A _ { n } \to 0$ as $n \to \infty$ 

(iii) $f _ { n }$ converges almost uniformly to zero if and only if $A _ { n } \to 0$ as $n \to \infty$ , or $\mu ( E _ { N } ^ { * } ) \to 0$ as $N \to \infty$ 

(iv) $f _ { n }$ converges pointwise to zero if and only if $A _ { n } \ \to \ 0$ as $\begin{array} { r } { n  \infty , \mathrm { o r } \bigcap _ { N = 1 } ^ { \infty } E _ { N } ^ { * } = \emptyset } \end{array}$ 

(v) $f _ { n }$ converges pointwise almost everywhere to zero if and only if $A _ { n } \to 0$ as $n  \infty .$ , or $\cap _ { N = 1 } ^ { \infty } E _ { N } ^ { * }$ is a null set. 

(vi) $f _ { n }$ converges in measure to zero if and only if $A _ { n } \to 0$ as $n \to \infty$ , or $\mu ( E _ { n } ) \to 0$ as $n \to \infty$ 

(vii) $f _ { n }$ converges in $L ^ { 1 }$ norm if and only if $A _ { n } \mu ( E _ { n } ) \to 0$ as $n \to \infty$ 

To put it more informally: when the height goes to zero, then one has convergence to zero in all modes except possibly for $L ^ { 1 }$ convergence, which requires that the product of the height and the width goes to zero. If instead the height is bounded away from zero and the width is positive, then we never have uniform or L<sup>∞</sup> $L ^ { \infty }$ convergence, but we have convergence in measure if the width goes to zero, we have almost uniform convergence if the tail support (which has larger measure than the width) has measure that goes to zero, we have pointwise almost everywhere convergence if the tail support shrinks to a null set, and pointwise convergence if the tail support shrinks to the empty set. 

It is instructive to compare this exercise with Exercise 1.5.2, or with the four examples given in the introduction. In particular: 

(i) In the escape to horizontal infinity scenario, the height and width do not shrink to zero, but the tail set shrinks to the empty set (while remaining of infinite measure throughout). 

(ii) In the escape to width infinity scenario, the height goes to zero, but the width (and tail support) go to infinity, causing the $L ^ { 1 }$ norm to stay bounded away from zero. 

(iii) In the escape to vertical infinity, the height goes to infinity, but the width (and tail support) go to zero (or the empty set), causing the $L ^ { 1 }$ norm to stay bounded away from zero. 

(iv) In the typewriter example, the width goes to zero, but the height and the tail support stay fixed (and thus bounded away from zero). 

Remark 1.5.8. The monotone convergence theorem (Theorem 1.4.44) can also be specialised to this case. Observe that the $f _ { n } = A _ { n } 1 _ { E _ { \tau } }$ n are monotone increasing if and only if $A _ { n } \leq A _ { n + 1 }$ and $E _ { n } \subset E _ { n + 1 }$ for each n. In such cases, observe that the $f _ { n }$ converge pointwise to $f : = A 1 _ { E }$ , where $A : = \operatorname* { l i m } _ { n \to \infty } A _ { n }$ and $\textstyle E : = \bigcup _ { n = 1 } ^ { \infty } E _ { n }$ . The monotone convergence theorem then asserts that $A _ { n } \mu ( E _ { n } ) \to A \mu ( E )$ as $n  \infty$ , which is a consequence of the monotone convergence theorem $\mu ( E _ { n } ) \to \mu ( E )$ for sets. 

1.5.3. Finite measure spaces. The situation simplifies somewhat if the space X has finite measure (and in particular, in the case when $( X , B , \mu )$ is a probability space, see Section 2.3). This shuts down two of the four examples (namely, escape to horizontal infinity or width infinity) and creates a few more equivalences. Indeed, from Egorov’s theorem (Exercise 1.4.31), we now have 

Theorem 1.5.9 (Egorov’s theorem, again). Let X have finite measure, and let $f _ { n } : X \to \mathbf { C }$ and $f : X \to \mathbf { C }$ be measurable functions. Then $f _ { n }$ converges to f pointwise almost everywhere if and only if $f _ { n }$ converges to f almost uniformly. 

Note that when one specialises to step functions using Exercise 1.5.3, then Egorov’s theorem collapses to the downward monotone convergence property for sets (Exercise 1.4.23(iii)). 

Another nice feature of the finite measure case is that $L ^ { \infty }$ convergence implies $L ^ { 1 }$ convergence: 

Exercise 1.5.4. Let X have finite measure, and let $f _ { n } : X \to \mathbf { C }$ and $f : X \to \mathbf { C }$ be measurable functions. Show that if $f _ { n }$ converges to $f$ in $L ^ { \infty }$ norm, then $f _ { n }$ also converges to f in $L ^ { 1 }$ norm. 

1.5.4. Fast convergence. The typewriter example shows that $L ^ { 1 }$ convergence is not strong enough to force almost uniform or pointwise almost everywhere convergence. However, this can be rectified if one assumes that the $L ^ { 1 }$ convergence is suficiently fast: 

Exercise 1.5.5 (Fast $L ^ { 1 }$ convergence). Suppose that $f _ { n } , f : X \to \mathbf { C }$ are measurable functions such that $\begin{array} { r } { \sum _ { n = 1 } ^ { \infty } \| f _ { n } - f \| _ { L ^ { 1 } ( \mu ) } < \infty ; } \end{array}$ thus, not only do the quantities $\| f _ { n } - f \| _ { L ^ { 1 } ( \mu ) } ~ \mathrm { g o }$ to zero (which would mean $L ^ { 1 }$ convergence), but they converge in an absolutely summable fashion. 

(i) Show that $f _ { n }$ converges pointwise almost everywhere to $f .$ 

(ii) Show that $f _ { n }$ converges almost uniformly to $f .$ 

(Hint: If you have trouble getting started, try working first in the special case in which $f _ { n } = A _ { n } 1 _ { E _ { n } }$ are step functions and $f = 0$ and use Exercise 1.5.3 in order to gain some intuition. The second part of the exercise implies the first, but the first is a little easier to prove and may thus serve as a useful warmup. The $\varepsilon / 2 ^ { n }$ trick may come in handy for the second part.) 

As a corollary, we see that $L ^ { 1 }$ convergence implies almost uniform or pointwise almost everywhere convergence if we are allowed to pass to a subsequence: 

Corollary 1.5.10. Suppose that $f _ { n } : X \to \mathbf { C }$ are a sequence $o f$ measurable functions that converge in $L ^ { 1 }$ norm to a limit $f$ . Then there exists a subsequence $f _ { n _ { j } }$ that converges almost uniformly (and hence, pointwise almost everywhere) to $f$ (while remaining convergent in $L ^ { 1 }$ norm, of course). 

Proof. Since $\| f _ { n } - f \| _ { L ^ { 1 } ( \mu ) } \to 0$ as $n \to \infty$ , we can select $n _ { 1 } < n _ { 2 } <$ $n _ { 3 } < . . .$ . such that $\| f _ { n _ { j } } - f \| _ { L ^ { 1 } ( \mu ) } \leq 2 ^ { - j }$ (say). This is enough for the previous exercise to apply.  

Actually, one can strengthen this corollary a bit by relaxing $L ^ { 1 }$ convergence to convergence in measure: 

Exercise 1.5.6. Suppose that $f _ { n } : X \to \mathbf { C }$ are a sequence of measurable functions that converge in measure to a limit $f .$ . Then there exists a subsequence $f _ { n _ { j } }$ that converges almost uniformly (and hence, pointwise almost everywhere) to $f .$ . (Hint: Choose the $n _ { j }$ so that the sets $\{ x \in X : | f _ { n _ { j } } ( x ) - f ( x ) | > 1 / j \}$ have a suitably small measure.) 

It is instructive to see how this subsequence is extracted in the case of the typewriter sequence. In general, one can view the operation of passing to a subsequence as being able to eliminate “typewriter” situations in which the tail support is much larger than the width. 

Exercise 1.5.7. Let $( X , B , \mu )$ be a measure space, let $f _ { n } : X \to \mathbf { C }$ be a sequence of measurable functions converging pointwise almost everywhere as $n $ ∞ to a measurable limit $f : X \to \mathbf { C }$ , and for each $n ,$ , let $f _ { n , m } : X \to \mathbf { C }$ be a sequence of measurable functions converging pointwise almost everywhere as $m  \infty$ (keeping n fixed) to $f _ { n }$ 

(i) $\operatorname { I f } \mu ( X )$ is finite, show that there exists a sequence $m _ { 1 } , m _ { 2 } , . . .$ such that $f _ { n , m _ { \tau } }$ converges pointwise almost everywhere to $f .$ 

(ii) Show the same claim is true if, instead of assuming that $\mu ( X )$ is finite, we merely assume that $X$ is $\sigma { - } f i n i t e .$ , i.e. it is the countable union of sets of finite measure 

(The claim can fail if X is not σ-finite. A counterexample is if $X =$ ${ \bf N } ^ { \bf N }$ with counting measure, $f _ { n }$ and $f$ are identically zero for all $n \in \mathbf N$ , and $f _ { n , m }$ is the indicator function the space of all sequences $( a _ { i } ) _ { i \in \mathbf { N } } \in$ ${ \bf N } ^ { \bf N }$ with $a _ { n } \geq m . )$ 

Exercise 1.5.8. Let $f _ { n } : X \to \mathbf { C }$ be a sequence of measurable functions, and let $f : X \to \mathbf { C }$ be another measurable function. Show that the following are equivalent: 

(i) $f _ { n }$ converges in measure to $f .$ . 

(ii) Every subsequence $f _ { n _ { j } }$ of the $f _ { n }$ has a further subsequence $f _ { n _ { j _ { i } } }$ that converges almost uniformly to $f .$ 

1.5.5. Domination and uniform integrability. Now we turn to the reverse question, of whether almost uniform convergence, pointwise almost everywhere convergence, or convergence in measure can imply $L ^ { 1 }$ convergence. The escape to vertical and width infinity examples shows that without any further hypotheses, the answer to this question is no. However, one can do better if one places some domination hypotheses on the $f _ { n }$ that shut down both of these escape routes. 

We say that a sequence $f _ { n } : X \to \mathbf { C }$ is dominated if there exists an absolutely integrable function $g : X \to \mathbf { C }$ such that $| f _ { n } ( x ) | \leq g ( x )$ for all $n$ and almost every x. For instance, if X has finite measure and the $f _ { n }$ are uniformly bounded, then they are dominated. Observe that the sequences in the vertical and width escape to infinity examples are not dominated (why?). 

The dominated convergence theorem (Theorem 1.4.49) then asserts that if $f _ { n }$ converges to $f$ pointwise almost everywhere, then it necessarily converges to $f$ in $L ^ { 1 }$ norm (and hence also in measure). Here is a variant: 

Exercise 1.5.9. Suppose that $f _ { n } : X \to \mathbf { C }$ are a dominated sequence of measurable functions, and let $f : X \to \mathbf { C }$ be another measurable function. Show that $f _ { n }$ converges in $L ^ { 1 }$ norm to $f$ if and only if $f _ { n }$ converges in measure to $f .$ . (Hint: one way to establish the $ { \mathrm { ^ 6 6 } } _ { 1 }  { \mathrm { f } } ^ { \mathfrak { P } }$ direction is first show that every subsequence of the $f _ { n }$ has a further subsequence that converges in $L ^ { 1 }$ to $f ,$ , using Exercise 1.5.6 and the dominated convergence theorem (Theorem 1.4.49). Alternatively, use monotone convergence to find a set $E$ of finite measure such that $\int _ { X \setminus E } g \ d \mu$ , and hence $\int _ { X \backslash E } f _ { n }$ dµ and $\int _ { X \setminus E } f \ d \mu$ , are small.) 

There is a more general notion than domination, known as uniform integrability, which serves as a substitute for domination in many (but not all) contexts. 

Definition 1.5.11 (Uniform integrability). A sequence $f _ { n } : X \to \mathbf { C }$ of absolutely integrable functions is said to be uniformly integrable if the following three statements hold: 

(i) (Uniform bound on $L ^ { 1 }$ norm) One has $\operatorname* { s u p } _ { n } \| f _ { n } \| _ { L ^ { 1 } ( \mu ) } =$ s $\begin{array} { r } { \operatorname* { l p } _ { n } \int _ { X } \left| f _ { n } \right| d \mu < + \infty } \end{array}$ 

(ii) (No escape to vertical infinity) One has sup<sub>n</sub> $\textstyle \int _ { | f _ { n } | \geq M } | f _ { n } | d \mu \to$ 0 as $M \to + \infty$ 

(iii) (No escape to width infinity) One has sup $\begin{array} { r } { \int _ { | f _ { n } | \leq \delta } | f _ { n } | d \mu  } \end{array}$ 0 as $\delta  0$ 

Remark 1.5.12. It is instructive to understand uniform integrability in the step function case $f _ { n } = A _ { n } 1 _ { E _ { n } }$ . The uniform bound on the 

$L ^ { 1 }$ norm then asserts that $A _ { n } \mu ( E _ { n } )$ stays bounded. The lack of escape to vertical infinity means that along any subsequence for which $A _ { n } \to \infty , A _ { n } \mu ( E _ { n } )$ must go to zero. Similarly, the lack of escape to width infinity means that along any subsequence for which $A _ { n } \to 0$ $A _ { n } \mu ( E _ { n } )$ must go to zero. 

Exercise 1.5.10. (i) Show that if f is an absolutely integrable function, then the constant sequence $f _ { n } = f$ is uniformly integrable. (Hint: use the monotone convergence theorem.) 

(ii) Show that every dominated sequence of measurable functions is uniformly integrable. 

(iii) Give an example of a sequence that is uniformly integrable but not dominated. 

In the case of a finite measure space, there is no escape to width infinity, and the criterion for uniform integrability simplifies to just that of excluding vertical infinity: 

Exercise 1.5.11. Suppose that X has finite measure, and let $f _ { n }$ : $X  \mathbf { C }$ be a sequence of measurable functions. Show that $f _ { n }$ is uniformly integrable if and only if sup $\begin{array} { r } { { \bf \Gamma } _ { n } \int _ { | f _ { n } | \geq M } | f _ { n } | ~ d \mu  0 } \end{array}$ as $M $ +∞. 

Exercise 1.5.12 (Uniform L<sup>p</sup> bound on finite measure implies uniform integrability). Suppose that X have finite measure, let $1 < p <$ ∞, an d suppose that $f _ { n } : X \to \mathbf { C }$ is a sequence of measurable functions such that $\begin{array} { r } { \operatorname* { s u p } _ { n } \int _ { X } | f _ { n } | ^ { p } \ d \mu < \infty } \end{array}$ . Show that the sequence $f _ { n }$ is uniformly integrable. 

Exercise 1.5.13. Let $f _ { n } : X \to \mathbf { C }$ be a uniformly integrable sequence of functions. Show that for every $\varepsilon > 0$ there exists a $\delta > 0$ such that 

$$
\int_ {E} | f _ {n} | d \mu \leq \varepsilon
$$

whenever $n \geq 1$ and E is a measurable set with $\mu ( E ) \leq \delta$ 

Exercise 1.5.14. This exercise is a partial converse to Exercise 1.5.13. Let X be a probability space, and let $f _ { n } : X \to \mathbf { C }$ be a sequence of absolutely integrable functions with $\operatorname* { s u p } _ { n } \| f _ { n } \| _ { L ^ { 1 } } < \infty$ 

Suppose that for every $\varepsilon > 0$ there exists a $\delta > 0$ such that 

$$
\int_ {E} | f _ {n} | d \mu \leq \varepsilon
$$

whenever $n \geq 1$ and E is a measurable set with $\mu ( E ) \leq \delta$ . Show that the sequence $f _ { n }$ is uniformly integrable. 

The dominated convergence theorem (Theorem 1.4.49) does not have an analogue in the uniformly integrable setting: 

Exercise 1.5.15. Give an example of a sequence $f _ { n }$ of uniformly integrable functions that converge pointwise almost everywhere to zero, but do not converge almost uniformly, in measure, or in $L ^ { 1 }$ norm. 

However, one does have an analogue of Exercise 1.5.9: 

Theorem 1.5.13 (Uniformly integrable convergence in measure). Let $f _ { n } : X \to \mathbf { C }$ be a uniformly integrable sequence of functions, and let $f : X \to \mathbf { C }$ be another function. Then $f _ { n }$ converges in $L ^ { 1 }$ norm to f if and only if $f _ { n }$ converges to f in measure. 

Proof. The “only $\mathrm { i f } ^ { \dag }$ part follows from Exercise 1.5.2, so we establish the $ { \mathbf { \hat { \rho } } } _ { \mathrm { 1 f } }  { \mathbf { \vec { \rho } } } _ { \mathrm { 1 } } ,$ part. 

By uniform integrability, there exists a finite $A > 0$ such that 

$$
\int_ {X} | f _ {n} | d \mu \leq A
$$

for all n. By Exercise 1.5.6, there is a subsequence of the $f _ { n }$ that converges pointwise almost everywhere to $f$ . Applying Fatou’s lemma (Corollary1.4.47), we conclude that 

$$
\int_ {X} | f | d \mu \leq A,
$$

thus $f$ is absolutely integrable. 

Now let $\varepsilon > 0$ be arbitrary. By uniform integrability, one can find $\delta > 0$ such that 

$$
\int_ {| f _ {n} | \leq \delta} | f _ {n} | d \mu \leq \varepsilon\tag{1.15}
$$

for all $n .$ . By monotone convergence, and decreasing $\delta$ if necessary, we may say the same for $f ,$ , thus 

$$
\int_ {| f | \leq \delta} | f | d \mu \leq \varepsilon .\tag{1.16}
$$

Let $0 < \kappa < \delta / 2$ be another small quantity (that can depend on $A , \varepsilon , \delta )$ that we will choose a bit later. From (1.15), (1.16) and the hypothesis $\kappa < \delta / 2$ we have 

$$
\int_ {| f _ {n} - f | <   \kappa ; | f | \leq \delta / 2} | f _ {n} | d \mu \leq \varepsilon
$$

and 

$$
\int_ {| f _ {n} - f | <   \kappa ; | f | \leq \delta / 2} | f | d \mu \leq \varepsilon
$$

and hence by the triangle inequality 

$$
\int_ {| f _ {n} - f | <   \kappa ; | f | \leq \delta / 2} | f - f _ {n} | d \mu \leq 2 \varepsilon .\tag{1.17}
$$

Finally, from Markov’s inequality (Exercise 1.4.36(vi)) we have 

$$
\mu (\{x: | f (x) | > \delta / 2 \}) \leq \frac {A}{\delta / 2}
$$

and thus 

$$
\int_ {| f _ {n} - f | <   \kappa ; | f | > \delta / 2} | f - f _ {n} | d \mu \leq \varepsilon \leq \frac {A}{\delta / 2} \kappa .
$$

In particular, by shrinking κ further if necessary we see that 

$$
\int_ {| f _ {n} - f | <   \kappa ; | f | > \delta / 2} | f - f _ {n} | d \mu \leq \varepsilon
$$

and hence by (1.17) 

$$
\int_ {| f _ {n} - f | <   \kappa} | f - f _ {n} | d \mu \leq 3 \varepsilon\tag{1.18}
$$

for all n. 

Meanwhile, since $f _ { n }$ converges in measure to $f ,$ , we know that there exists an $N$ (depending on $\kappa )$ such that 

$$
\mu (| f _ {n} (x) - f (x) | \geq \kappa) \leq \kappa
$$

for all $n \geq N$ . Applying Exercise 1.5.13, we conclude (making κ smaller if necessary) that 

$$
\int_ {| f _ {n} - f | \geq \kappa} | f _ {n} | d \mu \leq \varepsilon
$$

and 

$$
\int_ {| f _ {n} - f | \geq \kappa} | f | d \mu \leq \varepsilon
$$

and hence by the triangle inequality 

$$
\int_ {| f _ {n} - f | \geq \kappa} | f - f _ {n} | d \mu \leq 2 \varepsilon
$$

for all $n \geq N$ . Combining this with (1.18) we conclude that 

$$
\left\| f _ {n} - f \right\| _ {L ^ {1} (\mu)} = \int_ {X} | f - f _ {n} | d \mu \leq 5 \varepsilon
$$

for all $n \geq N$ , and so $f _ { n }$ converges to $f$ in $L ^ { 1 }$ norm as desired.  

Finally, we recall two results from the previous notes for unsigned functions. 

Exercise 1.5.16 (Monotone convergence theorem). Suppose that $f _ { n } : X \to [ 0 , + \infty )$ are measurable, monotone non-decreasing in n and are such that $\begin{array} { r } { \operatorname* { s u p } _ { n } \int _ { X } f _ { n } \ d \mu < \infty } \end{array}$ . Show that $f _ { n }$ converges in $L ^ { 1 }$ norm to $\operatorname { s u p } _ { n } f _ { n }$ . (Note that $\operatorname { s u p } _ { n } f _ { n }$ can be infinite on a null set, but the definition of $L ^ { 1 }$ convergence can be easily modified to accomodate this.) 

Exercise 1.5.17 (Defect version of Fatou’s lemma). Suppose that $f _ { n } : X \to [ 0 , + \infty )$ are measurable, are such that $\begin{array} { r } { \operatorname* { s u p } _ { n } \int _ { X } f _ { n } \ d \mu < \infty } \end{array}$ , and converge pointwise almost everywhere to some measurable limit $f : X \to [ 0 , + \infty )$ . Show that $f _ { n }$ converges in $L ^ { 1 }$ norm to $f$ if and only if $\textstyle { \int _ { X } f _ { n } \ d \mu }$ converges to $\textstyle \int _ { X } f  d \mu$ . Informally, we see that in the unsigned, bounded mass case, pointwise convergence implies $L ^ { 1 }$ norm convergence if and only if there is no loss of mass. 

Exercise 1.5.18. Suppose that $f _ { n } : X \to \mathbf { C }$ are a dominated sequence of measurable functions, and let $f : X \to \mathbf { C }$ be another measurable function. Show that $f _ { n }$ converges pointwise almost everywhere to $f$ if and only if $f _ { n }$ converges in almost uniformly to $f .$ 

Exercise 1.5.19. Let X be a probability space (see Section 2.3). Given any real-valued measurable function $f : X \to \mathbf { R }$ , we define the cumulative distribution function $F : \mathbf { R }  [ 0 , 1 ]$ of $f$ to be the function $F ( \lambda ) : = \mu ( \{ x \in X : f ( x ) \leq \lambda \} )$ . Given another sequence $f _ { n } : X \to$ R of real-valued measurable functions, we say that $f _ { n }$ converges in distribution to $f$ if the cumulative distribution function $F _ { n } ( \lambda )$ of $f _ { n }$ converges pointwise to the cumulative distribution function $F ( \lambda )$ of $f$ at all $\lambda \in \mathbf { R }$ for which $F$ is continuous. 

(i) Show that if $f _ { n }$ converges to $f$ in any of the seven senses discussed above (uniformly, essentially uniformly, almost uniformly pointwise, pointwise almost everywhere, in $L ^ { 1 }$ , or in measure), then it converges in distribution to $f$ . 

(ii) Give an example in which $f _ { n }$ converges to f in distribution, but not in any of the above seven senses. 

(iii) Show that convergence in distribution is not linear, in the sense that if $f _ { n }$ converges to $f$ in distribution, and $g _ { n }$ converges to $^ { g , }$ then $f _ { n } + g _ { n }$ need not converge to $f + g$ 

(iv) Show that a sequence $f _ { n }$ can converge in distribution to two diferent limits $f , g$ , which are not equal almost everywhere. 

Convergence in distribution (not to be confused with convergence in the sense of distributions, which is studied in S 1.13 of An epsilon of room, Vol. I is commonly used in probability; but, as the above exercise demonstrates, it is quite a weak notion of convergence, lacking many of the properties of the modes of convergence discussed here. 

## 1.6. Diferentiation theorems

Let [a, b] be a compact interval of positive length $( \mathrm { t h u s \ - \infty } < a < b <$ $+ \infty )$ . Recall that a function $F : [ a , b ] \to \mathbf { R }$ is said to be diferentiable at a point $x \in [ a , b ]$ if the limit 

$$
F ^ {\prime} (x) := \lim _ {y \to x; y \in [ a, b ] \setminus \{x \}} \frac {F (y) - F (x)}{y - x}\tag{1.19}
$$

exists. In that case, we call $F ^ { \prime } ( x )$ the strong derivative, classical derivative, or just derivative for short, of $F$ at x. We say that F is everywhere diferentiable, or diferentiable for short, if it is diferentiable at all points $x \in [ a , b ]$ , and diferentiable almost everywhere if it is diferentiable at almost every point $x \in [ a , b ]$ . If $F$ is diferentiable everywhere and its derivative $F ^ { \prime }$ is continuous, then we say that $F$ is continuously diferentiable. 

Remark 1.6.1. In §1.13 of An epsilon of room, Vol. I, the notion of a weak derivative or distributional derivative is introduced. This type of derivative can be applied to a much rougher class of functions and is in many ways more suitable than the classical derivative for doing “Lebesgue” type analysis (i.e. analysis centred around the Lebesgue integral, and in particular allowing functions to be uncontrolled, infinite, or even undefined on sets of measure zero). However, for now we will stick with the classical approach to diferentiation. 

Exercise 1.6.1. If $F : [ a , b ]  \mathbf { R }$ is everywhere diferentiable, show that $F$ is continuous and $F ^ { \prime }$ is measurable. If $F$ is almost everywhere diferentiable, show that the (almost everywhere defined) function $F ^ { \prime }$ is measurable (i.e. it is equal to an everywhere defined measurable function on $[ a , b ]$ outside of a null set), but give an example to demonstrate that $F$ need not be continuous. 

Exercise 1.6.2. Give an example of a function $F : [ a , b ] \ \to \ \mathbf { R }$ which is everywhere diferentiable, but not continuously diferentiable. (Hint: choose an $F$ that vanishes quickly at some point, say at the origin 0, but which also oscillates rapidly near that point.) 

In single-variable calculus, the operations of integration and differentiation are connected by a number of basic theorems, starting with Rolle’s theorem. 

Theorem 1.6.2 (Rolle’s theorem). Let $[ a , b ]$ be a compact interval of positive length, and let $F : [ a , b ]  \mathbf { R }$ be a diferentiable function such that $F ( a ) = F ( b )$ . Then there exists $x \in ( a , b )$ such that $F ^ { \prime } ( x ) = 0$ 

Proof. By subtracting a constant from $F$ (which does not afect differentiability or the derivative) we may assume that $F ( a ) = F ( b ) = 0$ If F is identically zero then the claim is trivial, so assume that $F$ is non-zero somewhere. By replacing $F$ with $- \boldsymbol { F }$ if necessary, we may assume that $F$ is positive somewhere, thus $\textstyle \operatorname* { s u p } _ { x \in [ a , b ] } F ( x ) > 0$ . On the other hand, as $F$ is continuous and $[ a , b ]$ is compact, $F$ must attain its maximum somewhere, thus there exists $x \in [ a , b ]$ such that $F ( x ) \geq F ( y )$ for all $y \in [ a , b ]$ . Then $F ( x )$ must be positive and so x cannot equal either a or $b ,$ and thus must lie in the interior. From the right limit of (1.19) we see that $F ^ { \prime } ( x ) \leq 0$ , while from the left limit we have $F ^ { \prime } ( x ) \geq 0$ . Thus $F ^ { \prime } ( x ) = 0$ and the claim follows.  

Remark 1.6.3. Observe that the same proof also works if $F$ is only diferentiable in the interior $( a , b )$ of the interval $[ a , b ]$ , so long as it is continuous all the way up to the boundary of $[ a , b ]$ 

Exercise 1.6.3. Give an example to show that Rolle’s theorem can fail if f is merely assumed to be almost everywhere diferentiable, even if one adds the additional hypothesis that f is continuous. This example illustrates that everywhere diferentiability is a significantly stronger property than almost everywhere diferentiability. We will see further evidence of this fact later in these notes; there are many theorems that assert in their conclusion that a function is almost everywhere diferentiable, but few that manage to conclude everywhere diferentiability. 

Remark 1.6.4. It is important to note that Rolle’s theorem only works in the real scalar case when $F$ is real-valued, as it relies heavily on the least upper bound property for the domain R. If, for instance, we consider complex-valued scalar functions $F : [ a , b ] \to \mathbf { C }$ , then the theorem can fail; for instance, the function $F : [ 0 , 1 ] \to \mathbf { C }$ defined by $F ( x ) : = e ^ { 2 \pi i x } - 1$ vanishes at both endpoints and is diferentiable, but its derivative $F ^ { \prime } ( x ) = 2 \pi i e ^ { 2 \pi i x }$ is never zero. (Rolle’s theorem does imply that the real and imaginary parts of the derivative $F ^ { \prime }$ both vanish somewhere, but the problem is that they don’t simultaneously vanish at the same point.) Similar remarks to functions taking values in a finite-dimensional vector space, such as $\mathbf { R } ^ { n }$ 

One can easily amplify Rolle’s theorem to the mean value theorem: 

Corollary 1.6.5 (Mean value theorem). Let $[ a , b ]$ be a compact interval of positive length, and let $F : [ a , b ] \to \mathbf { R }$ be a diferentiable function. Then there exists $x \in ( a , b )$ such that $\begin{array} { r } { F ^ { \prime } ( x ) = \frac { \dot { F ( b ) } - F ( a ) } { b - a } } \end{array}$ 

Proof. Apply Rolle’s theorem to the function $\begin{array} { r } { x \mapsto F ( x ) - \frac { F ( b ) - F ( a ) } { b - a } ( x - } \end{array}$ a).  

Remark 1.6.6. As Rolle’s theorem is only applicable to real scalarvalued functions, the more general mean value theorem is also only applicable to such functions. 

Exercise 1.6.4 (Uniqueness of antiderivatives up to constants). Let $[ a , b ]$ be a compact interval of positive length, and let $F : [ a , b ] \to \mathbf { R }$ and $G : [ a , b ] \to \mathbf { R }$ be diferentiable functions. Show that $F ^ { \prime } ( x ) =$ $G ^ { \prime } ( x )$ for every $x \in [ a , b ]$ if and only if $F ( x ) = G ( x ) + C$ for some constant $C \in \mathbf { R }$ and all $x \in [ a , b ]$ 

We can use the mean value theorem to deduce one of the fundamental theorems of calculus: 

Theorem 1.6.7 (Second fundamental theorem of calculus). Let $F$ : $[ a , b ] \to \mathbf { R }$ be a diferentiable function, such that $F ^ { \prime }$ is Riemann integrable. Then the Riemann integral $\textstyle \int _ { a } ^ { b } F ^ { \prime } ( x )$ dx of $F ^ { \prime }$ is equal to $F ( b ) - F ( a )$ . In particular, we have $\textstyle \int _ { a } ^ { b } F ^ { \prime } ( x ) \ d x = F ( b ) - F ( a )$ ) whenever F is continuously diferentiable. 

Proof. Let $\varepsilon > 0$ . By the definition of Riemann integrability, there exists a finite partition $a = t _ { 0 } < t _ { 1 } < . . . < t _ { k } = b$ such that 

$$
\left| \sum_ {j = 1} ^ {k} F ^ {\prime} \left(t _ {j} ^ {*}\right) \left(t _ {j} - t _ {j - 1}\right) - \int_ {a} ^ {b} F ^ {\prime} (x) \right| \leq \varepsilon
$$

for every choice of $t _ { j } ^ { \ast } \in [ t _ { j - 1 } , t _ { j } ]$ 

Fix this partition. From the mean value theorem, for each $1 \leq$ $j \le k$ one can find $t _ { j } ^ { \ast } \in [ t _ { j - 1 } , t _ { j } ]$ such that 

$$
F ^ {\prime} (t _ {j} ^ {*}) (t _ {j} - t _ {j - 1}) = F (t _ {j}) - F (t _ {j - 1})
$$

and thus by telescoping series 

$$
\left| (F (b) - F (a)) - \int_ {a} ^ {b} F ^ {\prime} (x) \right| \leq \varepsilon .
$$

Since $\varepsilon > 0$ was arbitrary, the claim follows. 

Remark 1.6.8. Even though the mean value theorem only holds for real scalar functions, the fundamental theorem of calculus holds for complex or vector-valued functions, as one can simply apply that theorem to each component of that function separately. 

Of course, we also have the other half of the fundamental theorem of calculus: 

Theorem 1.6.9 (First fundamental theorem of calculus). Let $[ a , b ]$ be a compact interval of positive length. Let $f : [ a , b ] \ \to \ \mathbf { C }$ be a continuous function, and let $F : [ a , b ] \to \mathbf { C }$ be the indefinite integral $\textstyle F ( x ) : = \int _ { a } ^ { x } f ( t )$ dt. Then F is diferentiable on $[ a , b ]$ , with derivative $F ^ { \prime } ( x ) = f ( x )$ for all $x \in [ a , b ]$ . In particular, $F$ is continuously diferentiable. 

Proof. It sufices to show that 

$$
\lim _ {h \to 0 ^ {+}} \frac {F (x + h) - F (x)}{h} = f (x)
$$

for all $x \in [ a , b )$ , and 

$$
\lim _ {h \to 0 ^ {-}} \frac {F (x + h) - F (x)}{h} = f (x)
$$

for all $x \in ( a , b ]$ . After a change of variables, we can write 

$$
{\frac {F (x + h) - F (x)}{h}} = \int_ {0} ^ {1} f (x + h t) d t
$$

for any $x \in [ a , b )$ and any suficiently small $h > 0$ , or any $x \in ( a , b ]$ and any suficiently small $h < 0$ . As f is continuous, the function $t \mapsto f ( x { + } h t )$ converges uniformly to $f ( x )$ on $[ 0 , 1 ]$ as $h  0$ (keeping x fixed). As the interval [0, 1] is bounded, $\textstyle \int _ { 0 } ^ { 1 } f ( x + h t )$ dt thus converges to $\begin{array} { r } { \int _ { 0 } ^ { 1 } f ( x ) \ d t = f ( x ) } \end{array}$ , and the claim follows.  

Corollary 1.6.10 (Diferentiation theorem for continuous functions). Let $f : [ a , b ] \to \mathbf { C }$ be a continuous function on a compact interval. Then we have 

$$
\lim _ {h \to 0 ^ {+}} \frac {1}{h} \int_ {[ x, x + h ]} f (t) d t = f (x)
$$

for all $x \in [ a , b )$ 

$$
\lim _ {h \rightarrow 0 ^ {+}} \frac {1}{h} \int_ {[ x - h, x ]} f (t) d t = f (x)
$$

for all $x \in ( a , b ]$ , and thus 

$$
\lim _ {h \to 0 ^ {+}} \frac {1}{2 h} \int_ {[ x - h, x + h ]} f (t) d t = f (x)
$$

for all $x \in ( a , b )$ 

In these notes we explore the question of the extent to which these theorems continue to hold when the diferentiability or integrability conditions on the various functions $F , F ^ { \prime } , f$ are relaxed. Among the results proven in these notes are 

(i) The Lebesgue diferentiation theorem, which roughly speaking asserts that Corollary 1.6.10 continues to hold for almost every x if f is merely absolutely integrable, rather than continuous; 

(ii) A number of diferentiation theorems, which assert for instance that monotone, Lipschitz, or bounded variation functions in one dimension are almost everywhere diferentiable; and 

(iii) The second fundamental theorem of calculus for absolutely continuous functions. 

## 1.6.1. The Lebesgue diferentiation theorem in one dimension. The main objective of this section is to show

Theorem 1.6.11 (Lebesgue diferentiation theorem, one-dimensional case). Let $f : \mathbf { R }  \mathbf { C }$ be an absolutely integrable function, and let $F : \mathbf { R }  \mathbf { C }$ be the definite integral $\begin{array} { r } { F ( x ) : = \int _ { [ - \infty , x ] } f ( t ) } \end{array}$ dt. Then F is continuous and almost everywhere diferentiable, and $F ^ { \prime } ( x ) = f ( x )$ for almost every $x \in \mathbf { R }$ 

This can be viewed as a variant of Corollary 1.6.10; the hypotheses are weaker because f is only assumed to be absolutely integrable, rather than continuous (and can live on the entire real line, and not just on a compact interval); but the conclusion is weaker too, because 

$F$ is only found to be almost everywhere diferentiable, rather than everywhere diferentiable. (But such a relaxation of the conclusion is necessary at this level of generality; consider for instance the example when $f = 1 _ { [ 0 , 1 ] } .  )$ 

The continuity is an easy exercise: 

Exercise 1.6.5. Let $f : \mathbf { R }  \mathbf { C }$ be an absolutely integrable function, and let $F : \mathbf { R }  \mathbf { C }$ be the definite integral $\begin{array} { r } { F ( x ) : = \int _ { [ - \infty , x ] } f ( t ) } \end{array}$ dt. Show that F is continuous. 

The main dificulty is to show that $F ^ { \prime } ( x ) = f ( x )$ for almost every $x \in \mathbf { R }$ . This will follow from 

Theorem 1.6.12 (Lebesgue diferentiation theorem, second formulation). Let $f : \mathbf { R }  \mathbf { C }$ be an absolutely integrable function. Then 

$$
\lim _ {h \to 0 ^ {+}} \frac {1}{h} \int_ {[ x, x + h ]} f (t) d t = f (x)\tag{1.20}
$$

for almost every $x \in \mathbf { R }$ , and 

$$
\lim _ {h \rightarrow 0 ^ {+}} \frac {1}{h} \int_ {[ x - h, x ]} f (t) d t = f (x)\tag{1.21}
$$

for almost every $x \in \mathbf { R }$ 

Exercise 1.6.6. Show that Theorem 1.6.11 follows from Theorem 1.6.12. 

We will just prove the first fact (1.20); the second fact (1.21) is similar (or can be deduced from (1.20) by replacing f with the reflected function $x \mapsto f ( - x )$ 

We are taking f to be complex valued, but it is clear from taking real and imaginary parts that it sufices to prove the claim when $f$ is real-valued, and we shall thus assume this for the rest of the argument. 

The conclusion (1.20) we want to prove is a convergence theorem - an assertion that for all functions $f$ in a given class (in this case, the class of absolutely integrable functions $f : \mathbf { R }  \mathbf { R } )$ , a certain sequence of linear expressions $T _ { h } f$ (in this case, the right averages $\begin{array} { r } { T _ { h } f ( x ) ~ = ~ \frac { 1 } { h } \int _ { [ x , x + h ] } f ( t ) ~ d t ) } \end{array}$ converge in some sense (in this case, pointwise almost everywhere) to a specified limit (in this case, $f )$ 

There is a general and very useful argument to prove such convergence theorems, known as the density argument. This argument requires two ingredients, which we state informally as follows: 

(i) A verification of the convergence result for some “dense subclass” of “nice” functions $f ,$ such as continuous functions, smooth functions, simple functions, etc.. By “dense”, we mean that a general function $f$ in the original class can be approximated to arbitrary accuracy in a suitable sense by a function in the nice subclass. 

(ii) A quantitative estimate that upper bounds the maximal fluctuation of the linear expressions $T _ { h } f$ in terms of the “size” of the function f (where the precise definition of “size” depends on the nature of the approximation in the first ingredient). 

Once one has these two ingredients, it is usually not too hard to put them together to obtain the desired convergence theorem for general functions f (not just those in the dense subclass). We illustrate this with a simple example: 

Proposition 1.6.13 (Translation is continuous in $L ^ { 1 } )$ . Let $f : \mathbf { R } ^ { d } $ C be an absolutely integrable function, and for each $h \in \mathbf { R } ^ { d }$ , let $f _ { h }$ : $\mathbf R ^ { d } \to \mathbf C$ be the shifted function 

$$
f _ {h} (x) := f (x - h).
$$

Then $f _ { h }$ converges in $L ^ { 1 }$ norm to f as $h  0$ , thus 

$$
\lim _ {h \to 0} \int_ {\mathbf {R} ^ {d}} | f _ {h} (x) - f (x) | d x = 0.
$$

Proof. We first verify this claim for a dense subclass of $f ,$ , namely the functions $f$ which are continuous and compactly supported (i.e. they vanish outside of a compact set). Such functions are continuous, and thus $f _ { h }$ converges uniformly to f as $h  0$ . Furthermore, as $f$ is compactly supported, the support of $f _ { h } - f$ stays uniformly bounded for h in a bounded set. From this we see that $f _ { h }$ also converges to f in $L ^ { 1 }$ norm as required. 

Next, we observe the quantitative estimate 

$$
\int_ {\mathbf {R} ^ {d}} | f _ {h} (x) - f (x) | d x \leq 2 \int_ {\mathbf {R} ^ {d}} | f (x) | d x\tag{1.22}
$$

for any $h \in \mathbf { R } ^ { d }$ . This follows easily from the triangle inequality 

$$
\int_ {\mathbf {R} ^ {d}} | f _ {h} (x) - f (x) | d x \leq \int_ {\mathbf {R} ^ {d}} | f _ {h} (x) | d x + \int_ {\mathbf {R} ^ {d}} | f (x) | d x
$$

together with the translation invariance of the Lebesgue integral: 

$$
\int_ {\mathbf {R} ^ {d}} | f _ {h} (x) | d x = \int_ {\mathbf {R} ^ {d}} | f (x) | d x.
$$

Now we put the two ingredients together. Let $f : \mathbf { R } ^ { d }  \mathbf { C }$ be absolutely integrable, and let $\varepsilon > 0$ be arbitrary. Applying Littlewood’s second principle (Theorem 1.3.20(iii)) to the absolutely integrable function $F ^ { \prime }$ , we can find a continuous, compactly supported function $g : \mathbf { R } ^ { d }  \mathbf { C }$ such that 

$$
\int_ {\mathbf {R} ^ {d}} | f (x) - g (x) | d x \leq \varepsilon .
$$

Applying (1.22), we conclude that 

$$
\int_ {\mathbf {R} ^ {d}} | (f - g) _ {h} (x) - (f - g) (x) | d x \leq 2 \varepsilon ,
$$

which we rearrange as 

$$
\int_ {\mathbf {R} ^ {d}} | (f _ {h} - f) _ {h} (x) - (g _ {h} - g) (x) | d x \leq 2 \varepsilon .
$$

By the dense subclass result, we also know that 

$$
\int_ {\mathbf {R} ^ {d}} | g _ {h} (x) - g (x) | d x \leq \varepsilon
$$

for all h suficiently close to zero. From the triangle inequality, we conclude that 

$$
\int_ {\mathbf {R} ^ {d}} | f _ {h} (x) - f (x) | d x \leq 3 \varepsilon
$$

for all h suficiently close to zero, and the claim follows. 

Remark 1.6.14. In the above application of the density argument, we proved the required quantitative estimate directly for all functions f in the original class of functions. However, it is also possible to use the density argument a second time and initially verify the quantitative estimate just for functions $f$ in a nice subclass (e.g. continuous functions of compact support). In many cases, one can then extend that estimate to the general case by using tools such as Fatou’s lemma (Corollary1.4.47), which are particularly suited for showing that upper bound estimates are preserved with respect to limits. 

Exercise 1.6.7. Let $f : \mathbf { R } ^ { d }  \mathbf { C } , g : \mathbf { R } ^ { d }  \mathbf { C }$ be Lebesgue measurable functions such that $f$ is absolutely integrable and $g$ is essentially bounded (i.e. bounded outside of a null set). Show that the convolution $f * g : \mathbf { R } ^ { d }  \mathbf { C }$ defined by the formula 

$$
f * g (x) = \int_ {\mathbf {R} ^ {d}} f (y) g (x - y) d y
$$

is well-defined (in the sense that the integrand on the right-hand side is absolutely integrable) and that $f * g$ is a bounded, continuous function. 

The above exercise is illustrative of a more general intuition, which is that convolutions tend to be smoothing in nature; the convolution $f * g$ of two functions is usually at least as regular as, and often more regular than, either of the two factors $f , g .$ 

This smoothing phenomenon gives rise to an important fact, namely the Steinhaus theorem: 

Exercise 1.6.8 (Steinhaus theorem). Let $E \subset \mathbf { R } ^ { d }$ be a Lebesgue measurable set of positive measure. Show that the set $E - E : = \{ x -$ $y : x , y \in E \}$ contains an open neighbourhood of the origin. (Hint: reduce to the case when $E$ is bounded, and then apply the previous exercise to the convolution $1 _ { E } * 1 _ { - E }$ , where $- E : = \{ - y : y \in E \} . )$ 

Exercise 1.6.9. A homomorphism $f : \mathbf { R } ^ { d }  \mathbf { C }$ is a map with the property that $f ( x + y ) = f ( x ) + f ( y )$ for all $x , y \in \mathbf { R } ^ { d }$ 

(i) Show that all measurable homomorphisms are continuous. (Hint: for any disk D centered at the origin in the complex plane, show that $f ^ { - 1 } ( z + D )$ has positive measure for at least one $z \in \mathbf { C }$ , and then use the Steinhaus theorem from the previous exercise.) 

• Show that $f$ is a measurable homomorphism if and only if it takes the form $f ( x _ { 1 } , \ldots , x _ { d } ) = x _ { 1 } z _ { 1 } + \ldots + x _ { d } z _ { d }$ for all $x _ { 1 } , \dotsc , x _ { d } \in \mathbf { R }$ and some complex coeficients $z _ { 1 } , \ldots , z _ { d }$ (Hint: first establish this for rationa $x _ { 1 } , \ldots , x _ { d }$ , and then use the previous part of this exercise.) 

(ii) (For readers familiar with Zorn’s lemma, see §2.4 of An epsilon ofroom, Vol. I) Show that there exist homomorphisms $f : \mathbf { R } ^ { d }  \mathbf { C }$ which are not of the form in the previous exercise. (Hint: view $\mathbf { R } ^ { d }$ (or C) as a vector space over the rationals $\mathbf { Q } ,$ , and use the fact (from Zorn’s lemma) that every vector space - even an infinite-dimensional one - has at least one basis.) This gives an alternate construction of a non-measurable set to that given in previous notes. 

Remark 1.6.15. One drawback with the density argument is it gives convergence results which are qualitative rather than quantitative - there is no explicit bound on the rate of convergence. For instance, in Proposition 1.6.13, we know that for any $\varepsilon > 0 ,$ , there exists $\delta > 0$ such that $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } | f _ { h } ( x ) - f ( x ) | \ d x \leq \varepsilon } \end{array}$ whenever $| h | \leq \delta .$ , but we do not know exactly how $\delta$ depends on ε and $f .$ . Actually, the proof does eventually give such a bound, but it depends on “how measurable” the function $f$ is, or more precisely how “easy” it is to approximate $f$ by a “nice” function. To illustrate this issue, let’s work in one dimension and consider the function $f ( x ) : = \sin ( N x ) 1 _ { [ 0 , 2 \pi ] } ( x )$ , where $N \geq 1$ is a large integer. On the one hand, f is bounded in the $L ^ { 1 }$ norm uniformly in N: $\textstyle \int _ { \mathbf { R } } | f ( x ) | \ d x \leq 2 \pi$ (indeed, the left-hand side is equal to 2). On the other hand, it is not hard to see that $\begin{array} { r } { \int _ { \mathbf { R } } | f _ { \pi / N } ( x ) - f ( x ) | \ d x \geq c } \end{array}$ for some absolute constant $c > 0$ . Thus, if one force $\begin{array} { r } { \int _ { \mathbf { R } } | f _ { h } ( x ) - f ( x ) | } \end{array}$ dx to drop below $^ { c , }$ one has to make $h$ at most $\pi / N$ from the origin. Making N large, we thus see that the rate of convergence of $\begin{array} { r } { \int _ { \mathbf { R } } | f _ { h } ( x ) - f ( x ) | } \end{array}$ dx to zero can be arbitrarily slow, even though $f$ is bounded in $L ^ { 1 }$ . The problem is that as $N$ gets large, it becomes increasingly dificult to approximate $f$ well by a “nice” function, by which we mean a uniformly continuous function with a reasonable modulus of continuity, due to the increasingly oscillatory nature of $f .$ . See [Ta2008, §1.4] for some further discussion of this issue, and what quantitative substitutes are available for such qualitative results. 

Now we return to the Lebesgue diferentiation theorem, and apply the density argument. The dense subclass result is already contained in Corollary 1.6.10, which asserts that (1.20) holds for all continuous functions $f .$ . The quantitative estimate we will need is the following special case of the Hardy-Littlewood maximal inequality: 

Lemma 1.6.16 (One-sided Hardy-Littlewood maximal inequality). Let $f : \mathbf { R }  \mathbf { C }$ be an absolutely integrable function, and let $\lambda > 0$ Then 

$$
m (\{x \in \mathbf {R}: \sup _ {h > 0} \frac {1}{h} \int_ {[ x, x + h ]} | f (t) | d t \geq \lambda \}) \leq \frac {1}{\lambda} \int_ {\mathbf {R}} | f (t) | d t.
$$

We will prove this lemma shortly, but let us first see how this, combined with the dense subclass result, will give the Lebesgue differentiation theorem. Let $f : \mathbf { R }  \mathbf { C }$ be absolutely integrable, and let $\varepsilon , \lambda > 0$ be arbitrary. Then by Littlewood’s second principle, we can find a function $g : \mathbf { R }  \mathbf { C }$ which is continuous and compactly supported, with 

$$
\int_ {\mathbf {R}} | f (x) - g (x) | d x \leq \varepsilon .
$$

Applying the one-sided Hardy-Littlewood maximal inequality, we conclude that 

$$
m (\{x \in \mathbf {R}: \sup _ {h > 0} \frac {1}{h} \int_ {[ x, x + h ]} | f (t) - g (t) | d t \geq \lambda \}) \leq \frac {\varepsilon}{\lambda}.
$$

In a similar spirit, from Markov’s inequality (Lemma 1.3.15) we have 

$$
m (\{x \in \mathbf {R}: | f (x) - g (x) | \geq \lambda \}) \leq \frac {\varepsilon}{\lambda}.
$$

By subadditivity, we conclude that for all $x \in \mathbf { R }$ outside of a set $E$ of measure at most $2 \varepsilon / \lambda$ , one has both 

$$
\frac {1}{h} \int_ {[ x, x + h ]} | f (t) - g (t) | d t <   \lambda\tag{1.23}
$$

and 

$$
| f (x) - g (x) | <   \lambda\tag{1.24}
$$

for all $h > 0$ 

Now let $x \in \mathbf { R } \backslash E$ . From the dense subclass result (Corollary 1.6.10) applied to the continuous function $g _ { \mathrm { : } }$ , we have 

$$
\left| \frac {1}{h} \int_ {[ x, x + h ]} g (t) d t - g (x) \right| <   \lambda
$$

whenever $h$ is suficiently close to x. Combining this with (1.23), (1.24), and the triangle inequality, we conclude that 

$$
\left| \frac {1}{h} \int_ {[ x, x + h ]} f (t) d t - f (x) \right| <   3 \lambda
$$

for all h suficiently close to zero. In particular we have 

$$
\operatorname * {l i m s u p} _ {h \to 0} | \frac {1}{h} \int_ {[ x, x + h ]} f (t) d t - f (x) | <   3 \lambda
$$

for all x outside of a set of measure $2 \varepsilon / \lambda$ . Keeping λ fixed and sending $\varepsilon$ to zero, we conclude that 

$$
\operatorname * {l i m s u p} _ {h \to 0} | \frac {1}{h} \int_ {[ x, x + h ]} f (t) d t - f (x) | <   3 \lambda
$$

for almost every $x \in \mathbf { R }$ . If we then let λ go to zero along a countable sequence $( \mathrm { e . g . ~ } \lambda : = 1 / n$ for $n = 1 , 2 , \ldots )$ , we conclude that 

$$
\operatorname * {l i m s u p} _ {h \to 0} | \frac {1}{h} \int_ {[ x, x + h ]} f (t) d t - f (x) | = 0
$$

for almost every $x \in \mathbf { R }$ , and the claim follows. 

The only remaining task is to establish the one-sided Hardy-Littlewood maximal inequality. We will do so by using the rising sun lemma: 

Lemma 1.6.17 (Rising sun lemma). Let $[ a , b ]$ be a compact interval, and let $F : [ a , b ] \to \mathbf { R }$ be a continuous function. Then one can find an at most countable family of disjoint non-empty open intervals $I _ { n } =$ $\left( a _ { n } , b _ { n } \right)$ in $[ a , b ]$ with the following properties: 

(i) For each n, either $F ( a _ { n } ) ~ = ~ F ( b _ { n } )$ , or else $ { \boldsymbol { a } } _ { n } ~ = ~  { \boldsymbol { a } }$ and $F ( b _ { n } ) \geq F ( a _ { n } )$ 

(ii) $I f x \in [ a , b ]$ does not lie in any of the intervals $I _ { n }$ , then one must have $F ( y ) \leq F ( x )$ for all $x \leq y \leq b$ 

Remark 1.6.18. To explain the name “rising sun lemma”, imagine the graph $\{ ( x , F ( x ) ) : x \in [ a , b ] \}$ of $F$ as depicting a hilly landscape, with the sun shining horizontally from the rightward infinity $( + \infty , 0 )$ (or rising from the east, if you will). Those x for which $F ( y ) \leq F ( x )$ are the locations on the landscape which are illuminated by the sun. The intervals $I _ { n }$ then represent the portions of the landscape that are in shadow. The reader is encouraged to draw a picture<sup>14</sup> to illustrate this perspective. 

## This lemma is proven using the following basic fact:

Exercise 1.6.10. Show that any open subset U of R can be written as the union of at most countably many disjoint non-empty open intervals, whose endpoints lie outside of U. (Hint: first show that every x in U is contained in a maximal open subinterval $( a , b )$ of $U$ and that these maximal open subintervals are disjoint, with each such interval containing at least one rational number.) 

Proof. (Proof of rising sun lemma) Let U be the set of all $x \in ( a , b )$ such that $F ( y ) > F ( x )$ for at least one $x < y < b$ . As F is continuous, U is open, and so U is the union of at most countably many disjoint non-empty open intervals ${ \cal I } _ { n } ~ = ~ ( a _ { n } , b _ { n } )$ , with the endpoints $a _ { n } , b _ { n }$ lying outside of U. 

The second conclusion of the rising sun lemma is clear from construction, so it sufices to establish the first. Suppose first that ${ \cal I } _ { n } ~ = ~ ( a _ { n } , b _ { n } )$ is such that $a _ { n } \ \neq \ a _ { }$ . As the endpoint $a _ { n }$ does not lie in U, we must have $F ( y ) \leq F ( a _ { n } )$ for all $a _ { n } \leq y \leq b ;$ similarly we have $F ( y ) \leq F ( b _ { n } )$ for all $b _ { n } \leq y \leq b .$ . In particular we have $F ( b _ { n } ) \leq F ( a _ { n } )$ . By the continuity of F, it will then sufice to show that $F ( b _ { n } ) \geq F ( t )$ for all $a _ { n } < t < b _ { n }$ 

Suppose for contradiction that there was $a _ { n } ~ < ~ t ~ < ~ b _ { n }$ with $F ( b _ { n } ) ~ < ~ F ( t )$ . Let $A : = \{ s \in [ t , b ] : F ( s ) \geq F ( t ) \}$ , then A is a closed set that contains t but not b. Set $t _ { * } ~ : = \operatorname* { s u p } ( A )$ , then $t _ { * } \in [ t , b ) \subset I _ { n } \subset U$ , and thus there exists $t _ { * } < y \le b$ such that $F ( y ) > F ( t _ { * } )$ . Since $F ( t _ { * } ) \geq F ( t ) > F ( b _ { n } )$ , and $F ( b _ { n } ) \geq F ( z )$ for all 

dt 

$b _ { n } \leq z \leq b$ , we see that $y$ cannot exceed $b _ { n }$ , and thus lies in $A .$ , but this contradicts the fact that $t _ { * }$ is the supremum of A. 

The case when $a _ { n } = a$ is similar and is left to the reader; the only diference is that we can no longer assert that $F ( y ) \leq F ( a _ { n } )$ for all $a _ { n } \leq y \leq b$ , and so do not have the upper bound $F ( b _ { n } ) \leq F ( a _ { n } )$  

Now we can prove the one-sided Hardy-Littlewood maximal inequality. By upwards monotonicity, it will sufice to show that 

$$
m (\{x \in [ a, b ]: \sup _ {h > 0; [ x, x + h ] \subset [ a, b ]} \frac {1}{h} \int_ {[ x, x + h ]} | f (t) | d t \geq \lambda \}) \leq \frac {1}{\lambda} \int_ {\mathbf {R}} | f (t) |
$$

for any compact interval $[ a , b ]$ . By modifying λ by an epsilon, we may replace the non-strict inequality here with strict inequality: 

$$
m (\{x \in [ a, b ]: \sup _ {h > 0; [ x, x + h ] \subset [ a, b ]} \frac {1}{h} \int_ {[ x, x + h ]} | f (t) | d t > \lambda \}) \leq \frac {1}{\lambda} \int_ {\mathbf {R}} | f (t) | d t\tag{1.25}
$$

Fix $[ a , b ]$ . We apply the rising sun lemma to the function $F$ : $[ a , b ] \to \mathbf { R }$ defined as 

$$
F (x) := \int_ {[ a, x ]} | f (t) | d t - (x - a) \lambda .
$$

By Lemma 1.6.5, F is continuous, and so we can find an at most countable sequence of intervals $\boldsymbol { I _ { n } } = \left( a _ { n } , b _ { n } \right)$ with the properties given by the rising sun lemma. From the second property of that lemma, we observe that 

$$
\{x \in [ a, b ]: \sup _ {h > 0; [ x, x + h ] \subset [ a, b ]} \frac {1}{h} \int_ {[ x, x + h ]} | f (t) | d t > \lambda \} \subset \bigcup_ {n} I _ {n},
$$

since the property $\begin{array} { r } { \frac { 1 } { h } \int _ { [ x , x + h ] } | f ( t ) | \ d t > \lambda } \end{array}$ can be rearranged as $F ( x +$ $h ) > F ( x )$ . By countable additivity, we may thus upper bound the left-hand side of (1.25) by $\textstyle \sum _ { n } ( b _ { n } - a _ { n } )$ . On the other hand, since $F ( b _ { n } ) - F ( a _ { n } ) \geq 0$ , we have 

$$
\int_ {I _ {n}} | f (t) | d t \geq \lambda (b _ {n} - a _ {n})
$$

and thus 

$$
\sum_ {n} (b _ {n} - a _ {n}) \leq \frac {1}{\lambda} \sum_ {n} \int_ {I _ {n}} | f (t) | d t.
$$

As the $I _ { n }$ are disjoint intervals in I, we may apply monotone convergence and monotonicity to conclude that 

$$
\sum_ {n} \int_ {I _ {n}} | f (t) | d t \leq \int_ {[ a, b ]} | f (t) | d t,
$$

and the claim follows. 

Exercise 1.6.11 (Two-sided Hardy-Littlewood maximal inequality). Let $f : \mathbf { R }  \mathbf { C }$ be an absolutely integrable function, and let $\lambda > 0$ Show that 

$$
m (\{x \in \mathbf {R}: \sup _ {x \in I} \frac {1}{| I |} \int_ {I} | f (t) | d t \geq \lambda \}) \leq \frac {2}{\lambda} \int_ {\mathbf {R}} | f (t) | d t,
$$

where the supremum ranges over all intervals I of positive length that contain x. 

Exercise 1.6.12 (Rising sun inequality). Let $f : \textbf { R }  \textbf { R }$ be an absolutely integrable function, and let $f ^ { * } : \mathbf { R }  \mathbf { R }$ be the one-sided signed Hardy-Littlewood maximal function 

$$
f ^ {*} (x) := \sup _ {h > 0} \frac {1}{h} \int_ {[ x, x + h ]} f (t) d t.
$$

Establish the rising sun inequality 

$$
\lambda m (\{f ^ {*} (x) > \lambda \}) \leq \int_ {x: f ^ {*} (x) > \lambda} f (x) d x
$$

for all real λ (note here that we permit λ to be zero or negative), and show that this inequality implies Lemma 1.6.16. (Hint: First do the $\lambda = 0$ case, by invoking the rising sun lemma.) See [Ta2009, §2.9] for some further discussion of inequalities of this type, and applications to ergodic theory (and in particular the maximal ergodic theorem). 

Exercise 1.6.13. Show that the left and right-hand sides in Lemma 1.6.16 are in fact equal. (Hint: one may first wish to try this in the case when $f$ has compact support, in which case one can apply the rising sun lemma to a suficiently large interval containing the support of f.) 

1.6.2. The Lebesgue diferentiation theorem in higher dimensions. Now we extend the Lebesgue diferentiation theorem to higher dimensions. Theorem 1.6.11 does not have an obvious high dimensional analogue, but Theorem 1.6.12 does: 

Theorem 1.6.19 (Lebesgue diferentiation theorem in general dimension). Let $f : \mathbf { R } ^ { d }  \mathbf { C }$ be an absolutely integrable function. Then for almost every $x \in \mathbf { R } ^ { d }$ , one has 

$$
\lim _ {r \to 0} \frac {1}{m (B (x , r))} \int_ {B (x, r)} | f (y) - f (x) | d y = 0\tag{1.26}
$$

and 

$$
\lim _ {r \to 0} \frac {1}{m (B (x , r))} \int_ {B (x, r)} f (y) d y = f (x),
$$

where $B ( x , r ) : = \{ y \in \mathbf { R } ^ { d } : | x - y | < r \}$ is the open ball of radius r centred at x. 

From the triangle inequality we see that 

$$
\begin{array}{c} | \frac {1}{m (B (x , r))} \int_ {B (x, r)} f (y) d y - f (x) | = | \frac {1}{m (B (x , r))} \int_ {B (x, r)} f (y) - f (x) d y | \\ \leq \frac {1}{m (B (x , r))} \int_ {B (x, r)} | f (y) - f (x) | d y, \end{array}
$$

so we see that the first conclusion of Theorem 1.6.19 implies the second. A point x for which (1.26) holds is called a Lebesgue point of $f ;$ thus, for an absolutely integrable function $f _ { : }$ , almost every point in $\mathbf { R } ^ { d }$ will be a Lebesgue point for $\mathbf { R } ^ { d }$ 

Exercise 1.6.14. Call a function $f : \mathbf { R } ^ { d }  \mathbf { C }$ locally integrable if, for every $x \in \mathbf { R } ^ { d }$ , there exists an open neighbourhood of x on which $f$ is absolutely integrable. 

(i) Show that $f$ is locally integrable if and only if $\begin{array} { r } { \int _ { B ( 0 , r ) } \left| f ( x ) \right| d x < } \end{array}$ $\infty$ for all $r > 0$ 

(ii) Show that Theorem 1.6.19 implies a generalisation of itself in which the condition of absolute integrability of f is weakened to local integrability. 

Exercise 1.6.15. For each $h > 0$ , let $E _ { h }$ be a subset of $B ( 0 , h )$ with the property that $m ( E _ { h } ) \ge c m ( B ( 0 , h ) )$ for some $c > 0$ independent of h. Show that if $f : \mathbf { R } ^ { d }  \mathbf { C }$ is locally integrable, and x is a Lebesgue point of $f _ { : }$ , then 

$$
\lim _ {h \to 0} \frac {1}{m (E _ {h})} \int_ {x + E _ {h}} f (y) d y = f (x).
$$

Conclude that Theorem 1.6.19 implies Theorem 1.6.12. 

To prove Theorem 1.6.19, we use the density argument. The dense subclass case is easy: 

Exercise 1.6.16. Show that Theorem 1.6.19 holds whenever $f$ is continuous. 

The quantitative estimate needed is the following: 

Theorem 1.6.20 (Hardy-Littlewood maximal inequality). Let $f$ : $\mathbf R ^ { d } \to \mathbf C$ be an absolutely integrable function, and let $\lambda > 0$ . Then $m ( \{ x \in \mathbf { R } ^ { d } : \operatorname* { s u p } _ { r > 0 } { \frac { 1 } { m ( B ( x , r ) ) } } \int _ { B ( x , r ) } | f ( y ) | d y \geq \lambda \} ) \leq { \frac { C _ { d } } { \lambda } } \int _ { \mathbf { R } } | f ( t ) | d t$ for some constant $C _ { d } > 0$ depending only on d. 

Remark 1.6.21. The expression $\begin{array} { r } { \operatorname* { s u p } _ { r > 0 } \frac { 1 } { m ( B ( x , r ) ) } \int _ { B ( x , r ) } | f ( y ) | \ d y \ge } \end{array}$ λ} is known as the Hardy-Littlewood maximal function of $f ,$ , and is often denoted $M f ( x )$ . It is an important function in the field of (real-variable) harmonic analysis. 

Exercise 1.6.17. Use the density argument to show that Theorem 1.6.20 implies Theorem 1.6.19. 

In the one-dimensional case, this estimate was established via the rising sun lemma. Unfortunately, that lemma relied heavily on the ordered nature of R, and does not have an obvious analogue in higher dimensions. Instead, we will use the following covering lemma. Given an open ball $B = B ( x , r )$ in $\mathbf { R } ^ { d }$ and a real number $c > 0$ , we write $c B : = B ( x , c r )$ for the ball with the same centre as $B .$ , but $c$ times the radius. (Note that this is slightly diferent from the set $c \cdot B : = \{ c y : y \in B \} \mathrm { ~ - ~ } \mathrm { w h y ? } )$ Note that $| c B | = c ^ { d } | B |$ for any open ball $B \subset \mathbf { R } ^ { d }$ and any $c > 0$ 

Lemma 1.6.22 (Vitali-type covering lemma). Let $B _ { 1 } , \ldots , B _ { n }$ be a finite collection of open balls in $\mathbf { R } ^ { d }$ (not necessarily disjoint). Then there exists a subcollection $B _ { 1 } ^ { \prime } , \ldots , B _ { m } ^ { \prime }$ of disjoint balls in this collection, such that 

$$
\bigcup_ {i = 1} ^ {n} B _ {i} \subset \bigcup_ {j = 1} ^ {m} 3 B _ {j} ^ {\prime}.\tag{1.27}
$$

In particular, by finite subadditivity, 

$$
m (\bigcup_ {i = 1} ^ {n} B _ {i}) \leq 3 ^ {d} \sum_ {j = 1} ^ {m} m (B _ {j} ^ {\prime}).
$$

Proof. We use a greedy algorithm argument, selecting the balls $B _ { i } ^ { \prime }$ to be as large as possible while remaining disjoint. More precisely, we run the following algorithm: 

Step 0. Initialise $m = 0$ (so that, initially, there are no balls $B _ { 1 } ^ { \prime } , \ldots , B _ { m } ^ { \prime }$ in the desired collection). 

Step 1. Consider all the balls $B _ { j }$ that do not already intersect one of the $B _ { 1 } ^ { \prime } , \ldots , B _ { m } ^ { \prime }$ (so, initially, all of the balls $B _ { 1 } , \ldots , B _ { n }$ will be considered). If there are no such balls, STOP. Otherwise, go on to Step 2. 

Step 2. Locate the largest ball $B _ { j }$ that does not already intersect one of the $B _ { 1 } ^ { \prime } , \ldots , B _ { m } ^ { \prime }$ . (If there are multiple largest balls with exactly the same radius, break the tie arbitrarily.) Add this ball to the collection $B _ { 1 } ^ { \prime } , \ldots , B _ { m } ^ { \prime }$ by setting $B _ { m + 1 } ^ { \prime } : = B _ { j }$ and then incrementing m to $m + 1$ . Then return to Step 1. 

Note that at each iteration of this algorithm, the number of available balls amongst the $B _ { 1 } , \ldots , B _ { n }$ drops by at least one (since each ball selected certainly intersects itself and so cannot be selected again). So this algorithm terminates in finite time. It is also clear from construction that the $B _ { 1 } ^ { \prime } , \ldots , B _ { m } ^ { \prime }$ are a subcollection of the $B _ { 1 } , \ldots , B _ { n }$ consisting of disjoint balls. So the only task remaining is to verify that (1.27) holds at the completion of the algorithm, i.e. to show that each ball $B _ { i }$ in the original collection is covered by the triples $3 B _ { j } ^ { \prime }$ of the subcollection. 

For this, we argue as follows. Take any ball $B _ { i }$ in the original collection. Because the algorithm only halts when there are no more balls that are disjoint from the $B _ { 1 } ^ { \prime } , \ldots , B _ { m } ^ { \prime }$ , the ball $B _ { i }$ must intersect at least one of the balls $B _ { j } ^ { \prime }$ in the subcollection. Let $B _ { j } ^ { \prime }$ be the first ball with this property, thus $B _ { i }$ is disjoint from $B _ { 1 } ^ { \prime } , \ldots , B _ { j - 1 } ^ { \prime }$ , but intersects $B _ { j } ^ { \prime }$ . Because $B _ { j } ^ { \prime }$ was chosen to be largest amongst all balls that did not intersect $B _ { 1 } ^ { \prime } , \dotsc , B _ { j - 1 } ^ { \prime }$ , we conclude that the radius of $B _ { i }$ cannot exceed that of $B _ { j } ^ { \prime }$ . From the triangle inequality, this implies that $B _ { i } \subset 3 B _ { j } ^ { \prime }$ , and the claim follows.  

Exercise 1.6.18. Technically speaking, the above algorithmic argument was not phrased in the standard language of formal mathematical deduction, because in that language, any mathematical object (such as the natural number $m )$ can only be defined once, and not redefined multiple times as is done in most algorithms. Rewrite the above argument in a way that avoids redefining any variable. (Hint: introduce a “time” variable t, and recursively construct families $B _ { 1 , t } ^ { \prime } , \ldots , B _ { m _ { t } , t } ^ { \prime }$ of balls that represent the outcome of the above algorithm after t iterations (or $t _ { * }$ iterations, if the algorithm halted at some previous time $t _ { * } < t )$ . For this particular algorithm, there are also more ad hoc approaches that exploit the relatively simple nature of the algorithm to allow for a less notationally complicated construction.) More generally, it is possible to use this time parameter trick to convert any construction involving a provably terminating algorithm into a construction that does not redefine any variable. (It is however dangerous to work with any algorithm that has an infinite run time, unless one has a suitably strong convergence result for the algorithm that allows one to take limits, either in the classical sense or in the more general sense of jumping to limit ordinals; in the latter case, one needs to use transfinite induction in order to ensure that the use of such algorithms is rigorous; see §2.4 of An epsilon of room, Vol. I.) 

Remark 1.6.23. The actual Vitali covering lemma[Vi1908] is slightly diferent to this one, but we will not need it here. Actually there is a family of related covering lemmas which are useful for a variety of tasks in harmonic analysis, see for instance [deG1981] for further discussion. 

Now we can prove the Hardy-Littlewood inequality, which we will do with the constant $C _ { d } : = 3 ^ { d }$ . It sufices to verify the claim with strict inequality, 

$$
m (\{x \in \mathbf {R} ^ {d}: \sup _ {r > 0} \frac {1}{m (B (x , r))} \int_ {B (x, r)} | f (y) | d y > \lambda \}) \leq \frac {C _ {d}}{\lambda} \int_ {\mathbf {R}} | f (t) | d t
$$

as the non-strict case then follows by perturbing λ slightly and then taking limits. 

Fix f and λ. By inner regularity, it sufices to show that 

$$
m (K) \leq \frac {3 ^ {d}}{\lambda} \int_ {\mathbf {R}} | f (t) | d t
$$

whenever $K$ is a compact set that is contained in $\begin{array} { r } { \{ x \in \mathbf { R } ^ { d } : \operatorname* { s u p } _ { r > 0 } \frac { 1 } { m ( B ( x , r ) ) } \int _ { B ( x , r ) } | f ( y ) | } \end{array}$ $\lambda \}$ 

By construction, for every $x \in K$ , there exists an open bal $B ( x , r )$ such that 

$$
\frac {1}{m (B (x , r))} \int_ {B (x, r)} | f (y) | d y > \lambda .\tag{1.28}
$$

By compactness of $K$ , we can cover K by a finite number $B _ { 1 } , \ldots , B _ { n }$ of such balls. Applying the Vitali-type covering lemma, we can find a subcollection $B _ { 1 } ^ { \prime } , \ldots , B _ { m } ^ { \prime }$ of disjoint balls such that 

$$
m (\bigcup_ {i = 1} ^ {n} B _ {i}) \leq 3 ^ {d} \sum_ {j = 1} ^ {m} m (B _ {j} ^ {\prime}).
$$

By (1.28), on each ball $B _ { j } ^ { \prime }$ we have 

$$
m (B _ {j} ^ {\prime}) <   \frac {1}{\lambda} \int_ {B _ {j} ^ {\prime}} | f (y) | d y;
$$

summing in $j$ and using the disjointness of the $B _ { j } ^ { \prime }$ we conclude that 

$$
m (\bigcup_ {i = 1} ^ {n} B _ {i}) \leq \frac {3 ^ {d}}{\lambda} \int_ {\mathbf {R} ^ {d}} | f (y) | d y.
$$

Since the $B _ { 1 } , \ldots , B _ { n }$ cover $K .$ , we obtain Theorem 1.6.20 as desired. 

Exercise 1.6.19. Improve the constant $3 ^ { d }$ in the Hardy-Littlewood maximal inequality to $2 ^ { d }$ . (Hint: observe that with the construction used to prove the Vitali covering lemma, the centres of the balls $B _ { i }$ are contained in $\cup _ { j = 1 } ^ { m } 2 B _ { j } ^ { \prime }$ and not just in $\mathsf { U } _ { j = 1 } ^ { m } 3 B _ { j } ^ { \prime }$ . To exploit this observation one may need to first create an epsilon of room, as the centers are not by themselves suficient to cover the required set.) 

Remark 1.6.24. The optimal value of $C _ { d }$ is not known in general, although a fairly recent result of Melas[Me2003] gives the surprising conclusion that the optimal value of $C _ { 1 }$ is $\begin{array} { r } { C _ { 1 } = \frac { 1 1 + \sqrt { 6 1 } } { 1 2 } = 1 . 5 6 \dots } \end{array}$ It is known that $C _ { d }$ grows at most linearly in $d ,$ thanks to a result of Stein and Str¨omberg[StSt1983], but it is not known if $C _ { d }$ is bounded in d or grows as $d \to \infty$ 

Exercise 1.6.20 (Dyadic maximal inequality). If $f : \mathbf { R } ^ { d }  \mathbf { C }$ is an absolutely integrable function, establish the dyadic Hardy-Littlewood maximal inequality 

$$
m (\{x \in \mathbf {R} ^ {d}: \sup _ {x \in Q} \frac {1}{| Q |} \int_ {Q} | f (y) | d y \geq \lambda \}) \leq \frac {1}{\lambda} \int_ {\mathbf {R}} | f (t) | d t
$$

where the supremum ranges over all dyadic cubes $Q$ that contain x. (Hint: the nesting property of dyadic cubes will be useful when it comes to the covering lemma stage of the argument, much as it was in Exercise 1.1.14.) 

Exercise 1.6.21 (Besicovich covering lemma in one dimension). Let $I _ { 1 } , \ldots , I _ { n }$ be a finite family of open intervals in R (not necessarily disjoint). Show that there exist a subfamily $I _ { 1 } ^ { \prime } , \ldots , I _ { m } ^ { \prime }$ of intervals such that 

(i) $\textstyle \bigcup _ { i = 1 } ^ { n } I _ { n } = \bigcup _ { j = 1 } ^ { m } I _ { m } ^ { \prime } ; \mathrm { a n }$ d 

(ii) Each point $x \in \mathbf { R }$ is contained in at most two of the $I _ { m } ^ { \prime }$ 

(Hint: First refine the family of intervals so that no interval $I _ { i }$ is contained in the union of the the other intervals. At that point, show that it is no longer possible for a point to be contained in three of the intervals.) There is a variant of this lemma that holds in higher dimensions, known as the Besicovitch covering lemma. 

Exercise 1.6.22. Let $\mu$ be a Borel measure (i.e. a countably additive measure on the Borel σ-algebra) on R, such that $0 < \mu ( I ) < \infty$ for every interval I of positive length. Assume that $\mu$ is inner regular, in the sense that $\mu ( E ) = \operatorname* { s u p } _ { K \subset E }$ , compact $\mu ( K )$ for every Borel measurable set $E$ . (As it turns out, from the theory of Radon measures, all locally finite Borel measures have this property, but we will not prove this here; see §1.10 of An epsilon of room, Vol. I.) Establish the Hardy-Littlewood maximal inequality 

$$
\mu (\{x \in \mathbf {R}: \sup _ {x \in I} \frac {1}{\mu (I)} \int_ {I} | f (y) | d \mu (y) \geq \lambda \}) \leq \frac {2}{\lambda} \int_ {\mathbf {R}} | f (y) | d \mu (y)
$$

for any absolutely integrable function $f \in L ^ { 1 } ( \mu )$ , where the supremum ranges over all open intervals I that contain $x .$ . Note that this essentially generalises Exercise 1.6.11, in which $\mu$ is replaced by Lebesgue measure. (Hint: Repeat the proof of the usual Hardy-Littlewood maximal inequality, but use the Besicovich covering lemma in place of the Vitali-type covering lemma. Why do we need the former lemma here instead of the latter?) 

Exercise 1.6.23 (Cousin’s theorem). Prove Cousin’s theorem: given any function $\delta : [ a , b ]  ( 0 , + \infty )$ on a compact interval $[ a , b ]$ of positive length, there exists a partition $a = t _ { 0 } < t _ { 1 } < . . . < t _ { k } = b$ with $k \geq 1$ , together with real numbers $t _ { j } ^ { \ast } \in [ t _ { j - 1 } , t _ { j } ]$ for each $1 \leq j \leq k$ and $t _ { j } - t _ { j - 1 } \leq \delta ( t _ { j } ^ { * } )$ . (Hint: use the Heine-Borel theorem, which asserts that any open cover of $[ a , b ]$ has a finite subcover, followed by the Besicovitch covering lemma.) This theorem is useful in a variety of applications related to the second fundamental theorem of calculus, as we shall see below. The positive function $\delta$ is known as a gauge function. 

Now we turn to consequences of the Lebesgue diferentiation theorem. Given a Lebesgue measurable set $E \subset \mathbf { R } ^ { d }$ , call a point $x \in \mathbf { R } ^ { d }$ a point of density for E if $\begin{array} { r } { \frac { m ( E \cap B ( x , r ) ) } { m ( B ( x , r ) ) }  1 } \end{array}$ as $r  0$ . Thus, for instance, if $E = [ - 1 , 1 ] \backslash \{ 0 \}$ , then every point in $( - 1 , 1 )$ (including the boundary point 0) is a point of density for $E ,$ , but the endpoints $- 1$ , 1 (as well as the exterior of $E )$ are not points of density. One can think of a point of density as being an “almost interior” point of $E ;$ it is not necessarily the case that one can fit an small ball $B ( x , r )$ centred at x inside of $E _ { : }$ but one can fit most of that small ball inside $E$ 

Exercise 1.6.24. If $E \subset \mathbf { R } ^ { d }$ is Lebesgue measurable, show that almost every point in $E$ is a point of density for $E ,$ and almost every point in the complement of $E$ is not a point of density for $E$ 

Exercise 1.6.25. Let $E \subset \mathbf { R } ^ { d }$ be a measurable set of positive measure, and let $\varepsilon > 0$ 

(i) Using Exercise 1.6.15 and Exercise 1.6.24, show that there exists a cube $Q \subset \mathbf { R } ^ { d }$ of positive sidelength such that $m ( E \cap$ $Q ) > ( 1 - \varepsilon ) m ( Q )$ 

(ii) Give an alternate proof of the above claim that avoids the Lebesgue diferentiation theorem. (Hint: reduce to the case when E is bounded, then approximate E by an almost disjoint union of cubes.) 

(iii) Use the above result to give an alternate proof of the Steinhaus theorem (Exercise 1.6.8). 

Of course, one can replace cubes here by other comparable shapes, such as balls. (Indeed, a good principle to adopt in analysis is that cubes and balls are “equivalent up to constants”, in that a cube of some sidelength can be contained in a ball of comparable radius, and vice versa. This type of mental equivalence is analogous to, though not identical with, the famous dictum that a topologist cannot distinguish a doughnut from a cofee cup.) 

Exercise 1.6.26. se 1.6.26. 

(i) Give an example of a compact set $K \subset$ R of positive measure such that $m ( K \cap I ) < | I |$ for every interval I of positive length. (Hint: first construct an open dense subset of [0, 1] of measure strictly less than 1.) 

(ii) Give an example of a measurable set $E \subset \mathbf { R }$ such that $0 < m ( E \cap I ) < | I |$ for every interval I of positive length. (Hint: first work in a bounded interval, such as (−1, 2). The complement of the set K in the first example is the union of at most countably many open intervals, thanks to Exercise 1.6.10. Now fill in these open intervals and iterate.) 

Exercise 1.6.27 (Approximations to the identity). Define a good $k e r n e l ^ { 1 5 }$ to be a measurable function $P : \mathbf { R } ^ { d }  \mathbf { R } ^ { + }$ which is nonnegative, radial (which means that there is a function $\tilde { P } : [ 0 , + \infty ) $ $\mathbf { R } ^ { + }$ such that $P ( x ) = \tilde { P } ( | x | ) )$ , radially non-increasing (so that $\tilde { P }$ is a non-increasing function), and has total mass $\int _ { \mathbf { R } ^ { d } } P ( x )$ dx equal to 1. The functions $\begin{array} { r } { P _ { t } ( x ) : = \frac { 1 } { t ^ { d } } P ( \frac { x } { t } ) } \end{array}$ for $t > 0$ are then said to be a good family of approximations to the identity. 

(i) Show that the heat kernels<sup>16</sup> $\begin{array} { r } { P _ { t } ( x ) : = \frac { 1 } { ( 4 \pi t ^ { 2 } ) ^ { d / 2 } } e ^ { - | x | ^ { 2 } / 4 t ^ { 2 } } } \end{array}$ and Poisson kernels $\begin{array} { r } { P _ { t } ( x ) : = c _ { d } \frac { t } { ( t ^ { 2 } + | x | ^ { 2 } ) ^ { ( d + 1 ) / 2 } } } \end{array}$ are good families of approximations to the identity, if the constant $c _ { d } > 0$ is chosen correctly (in fact one has $c _ { d } = \Gamma ( ( d + 1 ) / 2 ) / \pi ^ { ( d + 1 ) / 2 }$ , but you are not required to establish this). 

(ii) Show that if P is a good kernel, then 

$$
c _ {d} <   \sum_ {n = - \infty} ^ {\infty} 2 ^ {d n} \tilde {P} (2 ^ {n}) \leq C _ {d}
$$

for some constants $0 < c _ { d } < C _ { d }$ depending only on $d .$ (Hint: compare P with such “horizontal wedding cake” functions as $\begin{array} { r } { \sum _ { n = - \infty } ^ { \infty } 1 _ { 2 ^ { n - 1 } < | x | \leq 2 ^ { n } } \tilde { P } ( 2 ^ { n } ) . ) } \end{array}$ 

(iii) Establish the quantitative upper bound 

$$
| \int_ {\mathbf {R} ^ {d}} f (y) P _ {t} (x - y) d y | \leq C _ {d} ^ {\prime} \sup _ {r > 0} \frac {1}{| B (x , r) |} \int_ {B (x, r)} | f (y) | d y
$$

for any absolutely integrable function f and some constant $C _ { d } ^ { \prime } > 0$ depending only on d. 

(iv) Show that if $f : \mathbf { R } ^ { d }  \mathbf { C }$ is absolutely integrable and x is a Lebesgue point of $f ,$ , then the convolution 

$$
f * P _ {t} (x) := \int_ {\mathbf {R} ^ {d}} f (y) P _ {t} (x - y) d y
$$

converges to $f ( x )$ as $t  0$ . (Hint: split $f ( y )$ as the sum of $f ( x )$ and $f ( y ) - f ( x ) . )$ In particular, $f * P _ { t }$ converges pointwise almost everywhere to $f .$ 

1.6.3. Almost everywhere diferentiability. As we see in undergraduate real analysis, not every continuous function $f : \mathbf { R }  \mathbf { R }$ is diferentiable, with the standard example being the absolute value function $f ( x ) \ : = \ | x |$ , which is continuous not diferentiable at the origin $x = 0$ . Of course, this function is still almost everywhere differentiable. With a bit more efort, one can construct continuous functions that are in fact nowhere diferentiable: 

Exercise 1.6.28 (Weierstrass function). Let $F : \mathbf { R }  \mathbf { R }$ be the function 

$$
F (x) := \sum_ {n = 1} ^ {\infty} 4 ^ {- n} \sin (8 ^ {n} \pi x).
$$

(i) Show that $F$ is well-defined (in the sense that the series is absolutely convergent) and that $F$ is a bounded continuous function. 

(ii) Show that for every 8-dyadic interval $\textstyle { \bigl [ } { \frac { j } { 8 ^ { n } } } , { \frac { j + 1 } { 8 ^ { n } } } { \bigr ] }$ with $n \geq 1$ one has $\textstyle | F ( { \frac { j + 1 } { 8 ^ { n } } } ) - F ( { \frac { j } { 8 ^ { n } } } ) | \geq c 4 ^ { - n }$ for some absolute constant $c > 0$ 

(iii) Show that $F$ is not diferentiable at any point $x \in \mathbf { R }$ . (Hint: argue by contradiction and use the previous part of this exercise.) Note that it is not enough to formally diferentiate the series term by term and observe that the resulting series is divergent - why not? 

The dificulty here is that a continuous function can still contain a large amount of oscillation, which can lead to breakdown of diferentiability. However, if one can somehow limit the amount of oscillation present, then one can often recover a fair bit of diferentiability. For instance, we have 

Theorem 1.6.25 (Monotone diferentiation theorem). Any function $F : \mathbf { R }  \mathbf { R }$ which is monotone (either monotone non-decreasing or monotone non-increasing) is diferentiable almost everywhere. 

Exercise 1.6.29. Show that every monotone function is measurable. 

To prove this theorem, we just treat the case when $F$ is monotone non-decreasing, as the non-increasing case is similar (and can be deduced from the non-decreasing case by replacing $F$ with −F). 

We also first focus on the case when $F$ is continuous, as this allows us to use the rising sun lemma. To understand the diferentiability of $F$ , we introduce the four Dini derivatives of $F$ at x: 

(i) The upper right derivative $\begin{array} { r } { \overline { { D ^ { + } } } F ( x ) : = \operatorname* { l i m } \operatorname* { s u p } _ { h \to 0 ^ { + } } \frac { F ( x + h ) - F ( x ) } { h } } \end{array}$ ; 

(ii) The lower right derivative $\begin{array} { r } { \underline { { D ^ { + } } } F ( x ) : = \operatorname* { l i m } \operatorname* { i n f } _ { h \to 0 ^ { + } } \frac { F ( x + h ) - F ( x ) } { h } } \end{array}$ ; 

(iii) The upper left derivative $\begin{array} { r } { \overline { { D ^ { - } } } F ( x ) : = \operatorname* { l i m } \operatorname* { s u p } _ { h \to 0 ^ { - } } \frac { F ( x + h ) - F ( x ) } { h } } \end{array}$ ; 

(iv) The lower right derivative $\begin{array} { r } { \underline { { D ^ { - } } } F ( x ) : = \operatorname* { l i m } \operatorname* { i n f } _ { h \to 0 ^ { - } } \frac { F ( x + h ) - F ( x ) } { h } } \end{array}$ 

Regardless of whether F is diferentiable or not (or even whether F is continuous or not), the four Dini derivatives always exist and take values in the extended real line $[ - \infty , \infty ]$ . (If F is only defined on an interval $[ a , b ]$ , rather than on the endpoints, then some of the Dini derivatives may not exist at the endpoints, but this is a measure zero set and will not impact our analysis.) 

Exercise 1.6.30. If $F$ is monotone, show that the four Dini derivatives of $F$ are measurable. (Hint: the main dificulty is to reformulate the derivatives so that h ranges over a countable set rather than an uncountable one.) 

A function F is diferentiable at x precisely when the four derivatives are equal and finite: 

$$
\overline {{D ^ {+}}} F (x) = \underline {{D ^ {+}}} F (x) = \overline {{D ^ {-}}} F (x) = \underline {{D ^ {-}}} F (x) \in (- \infty , + \infty).\tag{1.29}
$$

We also have the trivial inequalities 

$$
\underline {{D ^ {+}}} F (x) \leq \overline {{D ^ {+}}} F (x); \quad \underline {{D ^ {-}}} F (x) \leq \overline {{D ^ {-}}} F (x).
$$

If $F$ is non-decreasing, all these quantities are non-negative, thus 

$$
0 \leq \underline {{D ^ {+}}} F (x) \leq \overline {{D ^ {+}}} F (x); \quad 0 \leq \underline {{D ^ {-}}} F (x) \leq \overline {{D ^ {-}}} F (x).
$$

The one-sided Hardy-Littlewood maximal inequality has an analogue in this setting: 

Lemma 1.6.26 (One-sided Hardy-Littlewood inequality). Let $F$ : $[ a , b ]  \mathbf { R }$ be a continuous monotone non-decreasing function, and let $\lambda > 0$ . Then we have 

$$
m (\{x \in [ a, b ]: \overline {{D ^ {+}}} F (x) \geq \lambda \}) \leq \frac {F (b) - F (a)}{\lambda}.
$$

Similarly for the other three Dini derivatives of $F$ . 

If F is not assumed to be continuous, then we have the weaker inequality 

$$
m (\{x \in [ a, b ]: \overline {{D ^ {+}}} F (x) \geq \lambda \}) \leq C \frac {F (b) - F (a)}{\lambda}
$$

for some absolute constant $C > 0$ 

Remark 1.6.27. Note that if one naively applies the fundamental theorems of calculus, one can formally see that the first part of Lemma 1.6.26 is equivalent to Lemma 1.6.16. We cannot however use this argument rigorously because we have not established the necessary fundamental theorems of calculus to do this. Nevertheless, we can borrow the proof of Lemma 1.6.16 without dificulty to use here, and this is exactly what we will do. 

Proof. We just prove the continuous case and leave the discontinuous case as an exercise. 

It sufices to prove the claim fo ${ \overline { { D ^ { + } } } } F ;$ by reflection (replacing $F ( x )$ with $- F ( - x )$ , and $[ a , b ]$ with $[ - b , - a ] )$ , the same argument works for $\overline { { D ^ { - } F } }$ , and then this trivially implies the same inequalities for ${ \underline { { D ^ { + } } } } F$ and $\underline { { D ^ { - } } } F$ . By modifying λ by an epsilon, and dropping the endpoints from $[ a , b ]$ as they have measure zero, it sufices to show that 

$$
m (\{x \in (a, b): \overline {{D ^ {+}}} F (x) > \lambda \}) \leq \frac {F (b) - F (a)}{\lambda}
$$

We may apply the rising sun lemma (Lemma 1.6.17) to the continuous function $G ( x ) : = F ( x ) - \lambda x$ . This gives us an at most countable family of intervals $I _ { n } = ( a _ { n } , b _ { n } )$ in $( a , b )$ , such that $G ( b _ { n } ) \geq G ( a _ { n } )$ for each $n .$ , and such that $G ( y ) \leq G ( x )$ whenever $a \leq x \leq y \leq b$ and x lies outside of all of the $I _ { n }$ 

Observe that if $x \in ( a , b )$ , and $G ( y ) \leq G ( x )$ for all $x \leq y \leq b$ , then $\overline { { D ^ { + } } } F ( x ) \leq \lambda$ . Thus we see that the set $\{ x \in ( a , b ) : { \overline { { D ^ { + } } } } F ( x ) > \lambda \}$ is contained in the union of the $I _ { n }$ , and so by countable additivity 

$$
m (\{x \in (a, b): \overline {{D ^ {+}}} F (x) > \lambda \}) \leq \sum_ {n} b _ {n} - a _ {n}.
$$

But we can rearrange the inequality $G ( b _ { n } ) \leq G ( a _ { n } )$ as $b _ { n } - a _ { n } \leq$ ${ \underline { { F ( b _ { n } ) - F ( a _ { n } ) } } } $ λ <sup>)</sup> . From telescoping series and the monotone nature of $F$ we have $\begin{array} { r } { \sum _ { n } F ( b _ { n } ) - F ( a _ { n } ) \leq F ( b ) - F ( a ) } \end{array}$ (this is easiest to prove by first working with a finite subcollection of the intervals $\left( a _ { n } , b _ { n } \right)$ , and then taking suprema), and the claim follows. 

The discontinuous case is left as an exercise. 

Exercise 1.6.31. Prove Lemma 1.6.26 in the discontinuous case. (Hint: the rising sun lemma is no longer available, but one can use either the Vitali-type covering lemma (which will give $C = 3 )$ or the Besicovitch lemma (which will give $C = 2 )$ , by modifying the proof of Theorem 1.6.20. 

Sending $\lambda \to \infty$ in the above lemma (cf. Exercise 1.3.18), and then sending $[ a , b ]$ to $\mathbf { R }$ , we conclude as a corollary that all the four Dini derivatives of a continuous monotone non-decreasing function are finite almost everywhere. So to prove Theorem 1.6.25 for continuous monotone non-decreasing functions, it sufices to show that (1.29) holds for almost every x. In view of the trivial inequalities, it sufices to show that $\overline { { D _ { + } } } F ( x ) \leq D _ { - } F ( x )$ and $\overline { { D _ { - } } } F ( x ) \leq D _ { + } F ( x )$ for almost every x. We will just show the first inequality, as the second follows by replacing F with its reflection $x \mapsto - F ( - x )$ ). It will sufice to show that for every pair $0 < r < R$ of real numbers, the set 

$$
E = E _ {r, R} := \{x \in \mathbf {R}: \overline {{D _ {+}}} F (x) > R > r > D _ {-} F (x) \}
$$

is a null set, since by letting $R , r$ range over rationals with $R > r > 0$ and taking countable unions, we would conclude that the set $\{ x \in \mathbf { R }$ $\overline { { D _ { + } } } F ( x ) > D _ { - } F ( x ) \}$ is a null set (recall that the Dini derivatives are all non-negative when F is non-decreasing), and the claim follows. 

Clearly E is a measurable set. To prove that it is null, we will establish the following estimate: 

Lemma 1.6.28 (E has density less than one). For any interval $[ a , b ]$ and any $0 < r < R$ , one has m $\begin{array} { r } { ( E _ { r , R } \cap [ a , b ] ) \leq \frac { r } { R } | b - a | } \end{array}$ 

Indeed, this lemma implies that E has no points of density, which by Exercise 1.6.24 forces E to be a null set. 

Proof. We begin by applying the rising sun lemma to the function $G ( x ) : = r x + F ( - x ) { \mathrm { ~ o n ~ } } [ - b , - a ]$ ; the large number of negative signs present here is needed in order to properly deal with the lower left Dini derivative $D _ { - } F$ . This gives an at most countable family of disjoint intervals $- I _ { n } = \left( - b _ { n } , - a _ { n } \right)$ in $( - b , - a )$ , such that $G ( - a _ { n } ) \geq G ( - b _ { n } )$ for all n, and such that $G ( - x ) \leq G ( - y )$ whenever $- x \leq - y \leq - a$ and $- x \in ( - b , - a )$ lies outside of all of the $- I _ { n }$ . Observe that if $x \in ( a , b )$ , and $G ( - x ) \leq G ( - y )$ for all $- x \leq - y \leq - a$ , then $D _ { - } F ( x ) \geq r$ Thus we see that $E _ { r , R }$ is contained inside the union of the intervals $\boldsymbol { I _ { n } } = \left( a _ { n } , b _ { n } \right)$ . On the other hand, from the first part of Lemma 1.6.26 we have 

$$
m (E _ {r, R} \cap (a _ {n}, b _ {n})) \leq \frac {F (b _ {n}) - F (a _ {n})}{R}.
$$

But we can rearrange the inequality $G ( - a _ { n } ) \leq G ( - b _ { n } )$ as $F ( b _ { n } ) \mathrm { ~ - ~ }$ $F ( a _ { n } ) \leq r ( b _ { n } - a _ { n } )$ . From countable additivity, one thus has 

$$
m (E _ {r, R}) \leq \frac {r}{R} \sum_ {n} b _ {n} - a _ {n}.
$$

But the $\left( a _ { n } , b _ { n } \right)$ are disjoint inside $( a , b )$ , so from countable additivity again, we have $\begin{array} { r } { \sum _ { n } b _ { n } - a _ { n } \leq b - a } \end{array}$ , and the claim follows.  

Remark 1.6.29. Note if F was not assumed to be continuous, then one would lose a factor of C here from the second part of Lemma 1.6.26, and one would then be unable to prevent $\overline { { D ^ { + } } } F$ from being up to C times as large as $D _ { - } F$ . So sometimes, even when all one is seeking is a qualitative result such as diferentiability, it is still important to keep track of constants. (But this is the exception rather than the rule: for a large portion of arguments in analysis, the constants are not terribly important.) 

This concludes the proof of Theorem 1.6.25 in the continuous monotone non-decreasing case. Now we work on removing the continuity hypothesis (which was needed in order to make the rising sun lemma work properly). If we naively try to run the density argument as we did in previous sections, then (for once) the argument does not work very well, as the space of continuous monotone functions are not suficiently dense in the space of all monotone functions in the relevant sense (which, in this case, is in the total variation sense, which is what is needed to invoke such tools as Lemma 1.6.26.). To bridge this gap, we have to supplement the continuous monotone functions with another class of monotone functions, known as the jump functions. 

Definition 1.6.30 (Jump function). A basic jump function J is a function of the form 

$$
J (x) := \left\{ \begin{array}{l l} 0 & \text {when x <   x_{0}} \\ \theta & \text {when x = x_{0}} \\ 1 & \text {when x > x_{0}} \end{array} \right.
$$

for some real numbers $x _ { 0 } \in \mathbf { R }$ and $0 \leq \theta \leq 1$ ; we call $x _ { 0 }$ the point of discontinuity for J and θ the fraction. Observe that such functions are monotone non-decreasing, but have a discontinuity at one point. A jump function is any absolutely convergent combination of basic jump functions, i.e. a function of the form $\textstyle F = \sum _ { n } c _ { n } J _ { n }$ , where n ranges over an at most countable set, each $J _ { n }$ is a basic jump function, and the $c _ { n }$ are positivereals with $\textstyle \sum _ { n } c _ { n } < \infty$ . If there are only finitely many n involved, we say that F is a piecewise constant jump function. 

Thus, for instance, if $q _ { 1 } , q _ { 2 } , q _ { 3 } , . . .$ is any enumeration of the rationals, then $\scriptstyle \sum _ { n = 1 } ^ { \infty } 2 ^ { - n } 1 _ { [ q _ { n } , + \infty ) }$ is a jump function. 

Clearly, all jump functions are monotone non-decreasing. From the absolute convergence of the $c _ { n }$ we see that every jump function is the uniform limit of piecewise constant jump functions, for instance $\textstyle \sum _ { n = 1 } ^ { \infty } c _ { n } J _ { n }$ is the uniform limit of $\textstyle \sum _ { n = 1 } ^ { N } c _ { n } J _ { n }$ . One consequence of this is that the points of discontinuity of a jump function $\textstyle \sum _ { n = 1 } ^ { \infty } c _ { n } J _ { n }$ are precisely those of the individual summands $c _ { n } J _ { n }$ , i.e. of the points $x _ { n }$ where each $J _ { n }$ jumps. 

The key fact is that these functions, together with the continuous monotone functions, essentially generate all monotone functions, at least in the bounded case: 

Lemma 1.6.31 (Continuous-singular decomposition for monotone functions). Let $F : \mathbf { R }  \mathbf { R }$ be a monotone non-decreasing function. 

(i) The only discontinuities of F are jump discontinuities. More precisely, if x is a point where F is discontinuous, then the limits lim $\mathfrak { l } _ { y \to x ^ { - } } F ( y )$ and $\scriptstyle \operatorname* { l i m } _ { y \to x ^ { + } } F ( y )$ both exist, but are unequal, with lim $\begin{array} { r } { { } _ { y \to x ^ { - } } F ( y ) < \operatorname* { l i m } _ { y \to x ^ { + } } F ( y ) } \end{array}$ 

(ii) There are at most countably many discontinuities of $F$ . 

(iii) If F is bounded, then F can be expressed as the sum of a continuous monotone non-decreasing function $F _ { c }$ and a jump function $F _ { p p }$ 

Remark 1.6.32. This decomposition is part of the more general Lebesgue decomposition, discussed in §1.2 of An epsilon of room, Vol. I. 

Proof. By monotonicity, the limits $F _ { - } ( x ) : = \mathrm { l i m } _ { y  x ^ { - } } F ( y )$ and $F ^ { + } ( x ) : =$ $\scriptstyle \operatorname* { l i m } _ { y \to x ^ { + } } F ( y )$ always exist, with $F _ { - } ( x ) \leq F ( x ) \leq F _ { + } ( x )$ for all x. This gives (i). 

By (i), whenever there is a discontinuity x of F, there is at least one rational number $q _ { x }$ strictly between $F _ { - } ( x )$ and $F _ { + } ( x )$ , and from monotonicity, each rational number can be assigned to at most one discontinuity. This gives (ii). 

Now we prove (iii). Let A be the set of discontinuities of F, thus A is at most countable. For each $x \in A$ , we define the jump $c _ { x } : = F _ { + } ( x ) - F _ { - } ( x ) > 0$ , and the fraction $\begin{array} { r } { \theta _ { x } : = \frac { F \left( x \right) - F - \left( x \right) } { F + \left( x \right) - F - \left( x \right) } \in \overline { { \left[ 0 , 1 \right] } } } \end{array}$ Thus 

$$
F _ {+} (x) = F _ {-} (x) + c _ {x} \text { and } F (x) = F _ {-} (x) + \theta_ {x} c _ {x}.
$$

Note that $c _ { x }$ is the measure of the interval $( F _ { - } ( x ) , F _ { + } ( x ) )$ . By monotonicity, these intervals are disjoint; by the boundedness of $F$ , their union is bounded. By countable additivity, we thus have $\textstyle \sum _ { x \in A } c _ { x } <$ $\infty$ , and so if we let $J _ { x }$ be the basic jump function with point of discontinuity x and fraction $\theta _ { x }$ , then the function 

$$
F _ {p p} := \sum_ {x \in A} c _ {x} J _ {x}
$$

is a jump function. 

As discussed previously, G is discontinuous only at $A$ , and for each $x \in A$ one easily checks that 

$$
(F _ {p p}) _ {+} (x) = (F _ {p p}) _ {-} (x) + c _ {x} \mathrm{and} F _ {p p} (x) = (F _ {p p}) _ {-} (x) + \theta_ {x} c _ {x}
$$

where $\begin{array} { r } { ( F _ { p p } ) _ { - } ( x ) : = \operatorname* { l i m } _ { y  x ^ { - } } F _ { p p } ( y ) } \end{array}$ , and $\begin{array} { r } { ( F _ { p p } ) _ { + } ( x ) : = \operatorname* { l i m } _ { y  x ^ { + } } F _ { p p } ( y ) } \end{array}$ We thus see that the diference $F _ { c } : = F - F _ { p p }$ is continuous. The only remaining task is to verify that $F _ { c }$ is monotone non-decreasing, thus we need 

$$
F _ {p p} (b) - F _ {p p} (a) \leq F (b) - F (a)
$$

for all $a < b$ . But the left-hand side can be rewritten as $\textstyle \sum _ { x \in A \cap [ a , b ] } c _ { x }$ As each $c _ { x }$ is the measure of the interval $( F _ { - } ( x ) , F _ { + } ( x ) )$ , and these intervals for $x \in A \cap [ a , b ]$ are disjoint and lie in $( F ( a ) , F ( b ) )$ , the claim follows from countable additivity.  

Exercise 1.6.32. Show that the decomposition of a bounded monotone non-decreasing function F into continuous $F _ { c }$ and jump components $F _ { p p }$ given by the above lemma is unique. 

Exercise 1.6.33. Find a suitable generalisation of the notion of a jump function that allows one to extend the above decomposition to unbounded monotone functions, and then prove this extension. (Hint: the notion to shoot for here is that of a “locally jump function”.) 

Now we can finish the proof of Theorem 1.6.25. As noted previously, it sufices to prove the claim for monotone non-decreasing functions. As diferentiability is a local condition, we can easily reduce to the case of bounded monotone non-decreasing functions, since to test diferentiability of a monotone non-decreasing function $F$ in any compact interval $[ a , b ]$ we may replace $F$ by the bounded monotone non-decreasing function max $( \operatorname* { m i n } ( F , F ( b ) ) , F ( a ) )$ ) with no change in the diferentiability in $[ a , b ]$ (except perhaps at the endpoints $a , b ,$ but these form a set of measure zero). As we have already proven the claim for continuous functions, it sufices by Lemma 1.6.31 (and linearity of the derivative) to verify the claim for jump functions. 

Now, finally, we are able to use the density argument, using the piecewise constant jump functions as the dense subclass, and using the second part of Lemma 1.6.26 for the quantitative estimate; fortunately for us, the density argument does not particularly care that there is a loss of a constant factor in this estimate. 

For piecewise constant jump functions, the claim is clear (indeed, the derivative exists and is zero outside of finitely many discontinuities). Now we run the density argument. Let F be a bounded jump function, and let $\varepsilon > 0$ and $\lambda > 0$ be arbitrary. As every jump function is the uniform limit of piecewise constant jump functions, we can find a piecewise constant jump function $F _ { \varepsilon }$ such that $| F ( x ) - F _ { \varepsilon } ( x ) | \leq \varepsilon$ for all x. Indeed, by taking $F _ { \varepsilon }$ to be a partial sum of the basic jump functions that make up $F$ , we can ensure that $F - F _ { \varepsilon }$ is also a monotone non-decreasing function. Applying the second part of Lemma 1.6.26, we have 

$$
\{x \in \mathbf {R}: \overline {{D ^ {+}}} (F - F _ {\varepsilon}) (x) \geq \lambda \} \leq \frac {2 C \varepsilon}{\lambda}
$$

for some absolute constant $C ,$ , and similarly for the other four Dini derivatives. Thus, outside of a set of measure at most $8 C \varepsilon / \lambda$ , all of the Dini derivatives of $F - F _ { \varepsilon }$ are less than λ. Since $F _ { \varepsilon } ^ { \prime }$ is almost everywhere diferentiable, we conclude that outside of a set of measure at most $8 C \varepsilon / \lambda$ , all the Dini derivatives of $F ( x )$ lie within $\lambda$ of $F _ { \varepsilon } ^ { \prime } ( x )$ , and in particular are finite and lie within 2λ of each other. Sending $\varepsilon$ to zero (holding $\lambda$ fixed), we conclude that for almost every $x ,$ the Dini derivatives of $F$ are finite and lie within 2λ of each other. If we then send $\lambda$ to zero, we see that for almost every x, the Dini derivatives of $F$ agree with each other and are finite, and the claim follows. This concludes the proof of Theorem 1.6.25. 

Just as the integration theory of unsigned functions can be used to develop the integration theory of the absolutely convergent functions (see Section 1.3.4), the diferentiation theory of monotone functions can be used to develop a parallel diferentiation theory for the class of functions of bounded variation: 

Definition 1.6.33 (Bounded variation). Let $F : \mathbf { R }  \mathbf { R }$ be a function. The total variation $\| F \| _ { T V ( \mathbf { R } ) } \ ( \mathrm { o r } \ \| F \| _ { T V }$ for short) of $F$ is defined to be the supremum 

$$
\| F \| _ {T V (\mathbf {R})} := \sup _ {x _ {0} <   \dots <   x _ {n}} \sum_ {i = 1} ^ {n} | F (x _ {i}) - F (x _ {i + 1}) |
$$

where the supremum ranges over all finite increasing sequences $x _ { 0 } , \ldots , x _ { n }$ of real numbers with $n \geq 0 ;$ this is a quantity in $[ 0 , + \infty ]$ . We say that $F$ has bounded variation (on R) if $\| F \| _ { T V ( \mathbf { R } ) }$ is finite. (In this case, $\| F \| _ { T V ( \mathbf { R } ) }$ is often written as $\| F \| _ { B V ( \mathbf { R } ) }$ or just $\| F \| _ { B V } . \quad$ 

Given any interval $[ a , b ]$ , we define the total variation $\| F \| _ { T V ( [ a , b ] ) }$ of $F$ on $[ a , b ]$ as 

$$
\| F \| _ {T V ([ a, b ])} := \sup _ {a \leq x _ {0} <   \dots <   x _ {n} \leq b} \sum_ {i = 1} ^ {n} | F (x _ {i}) - F (x _ {i + 1}) |;
$$

thus the definition is the same, but the points $x _ { 0 } , \ldots , x _ { n }$ are restricted to lie in $[ a , b ]$ . Thus for instance $\begin{array} { r } { \| F \| _ { T V ( \mathbf { R } ) } = \operatorname* { s u p } _ { N \to \infty } \| F \| _ { T V ( [ - N , N ] ) } } \end{array}$ We say that a function F has bounded variation on $[ a , b ] \operatorname { i f } \| F \| _ { B V ( [ a , b ] ) }$ is finite. 

Exercise 1.6.34. If $F : \mathbf { R }  \mathbf { R }$ is a monotone function, show that $\| F \| _ { T V ( [ a , b ] ) } = | F ( b ) - F ( a ) |$ for any interval $[ a , b ]$ , and that $F$ has bounded variation on R if and only if it is bounded. 

Exercise 1.6.35. For any functions $F , G : \mathbf { R }  \mathbf { R }$ , establish the triangle property $\| F + G \| _ { T V ( \mathbf { R } ) } \leq \| F \| _ { T V ( \mathbf { R } ) } + \| G \| _ { T V ( \mathbf { R } ) }$ and the homogeneity property $\| c F \| _ { T V ( \mathbf { R } ) } = | c | \| F \| _ { T V ( \mathbf { R } ) }$ for any $c \in \mathbf { R }$ . Also show that $\| F \| _ { T V } = 0$ if and only if F is constant. 

Exercise 1.6.36. If $F : \mathbf { R }  \mathbf { R }$ is a function, show that $\| F \| _ { T V ( [ a , b ] ) } +$ $\| F \| _ { T V ( [ b , c ] ) } = \| F \| _ { T V ( [ a , c ] ) }$ whenever $a \leq b \leq c$ 

Exercise 1.6.37. (i) Show that every function $f : \mathbf { R }  \mathbf { R }$ of bounded variation is bounded, and that the limits $\scriptstyle \operatorname* { l i m } _ { x \to + \infty } f ( x )$ and $\scriptstyle \operatorname* { l i m } _ { x \to - \infty } f ( x )$ , are well-defined. 

(ii) Give a counterexample of a bounded, continuous, compactly supported function f that is not of bounded variation. 

Exercise 1.6.38. Let $f : \mathbf { R }  \mathbf { R }$ be an absolutely integrable function, and let $F : \mathbf { R }  \mathbf { R }$ be the indefinite integral $\begin{array} { r } { F ( x ) : = \int _ { [ - \infty , x ] } f ( x ) } \end{array}$ Show that F is of bounded variation, and that $\| F \| _ { T V ( \mathbf { R } ) } = \| f \| _ { L ^ { 1 } ( \mathbf { R } ) }$ (Hint: the upper bound $\| F \| _ { T V ( \mathbf { R } ) } \leq \| f \| _ { L ^ { 1 } ( \mathbf { R } ) }$ is relatively easy to establish. To obtain the lower bound, use the density argument.) 

Much as an absolutely integrable function can be expressed as the diference of its positive and negative parts, a bounded variation function can be expressed as the diference of two bounded monotone functions: 

Proposition 1.6.34. A function $F : \mathbf { R }  \mathbf { R }$ is of bounded variation if and only if it is the diference of two bounded monotone functions. 

Proof. It is clear from Exercises 1.6.34, 1.6.35 that the diference of two bounded monotone functions is bounded. Now define the positive variation $F ^ { + } : \mathbf { R }  \mathbf { R }$ of $F$ by the formula 

$$
F ^ {+} (x) := \sup _ {x _ {0} <   \dots <   x _ {n} \leq x} \sum_ {i = 1} ^ {n} \max (F (x _ {i + 1}) - F (x _ {i}), 0).\tag{1.30}
$$

It is clear from construction that this is a monotone increasing function, taking values between 0 and $\| F \| _ { T V ( \mathbf { R } ) }$ , and is thus bounded. To conclude the proposition, it sufices to (by writing $F = F _ { + } - ( F _ { + } - F _ { - } )$ to show that $F _ { + } - F$ is non-decreasing, or in other words to show that 

$$
F ^ {+} (b) \geq F ^ {+} (a) + F (b) - F (a).
$$

If $F ( b ) - F ( a )$ is negative then this is clear from the monotone nondecreasing nature of $F ^ { + }$ , so assume that $F ( b ) - F ( a ) \geq 0$ . But then the claim follows because any sequence of real numbers $x _ { 0 } < \ldots <$ $x _ { n } \leq a$ can be extended by one or two elements by adding a and $b ,$ thus increasing the sum $\begin{array} { r } { \operatorname* { s u p } _ { x _ { 0 } < \ldots < x _ { n } } \sum _ { i = 1 } ^ { n } \operatorname* { m a x } ( F ( x _ { i } ) - F ( x _ { i + 1 } ) , 0 ) } \end{array}$ by at least $F ( b ) - F ( a )$  

Exercise 1.6.39. Let $F : \mathbf { R }  \mathbf { R }$ be of bounded variation. Define the positive variation $F ^ { + }$ by (1.30), and the negative variation $F ^ { - }$ by 

$$
F ^ {-} (x) := \sup _ {x _ {0} <   \dots <   x _ {n} \leq x} \sum_ {i = 1} ^ {n} \max (- F (x _ {i + 1}) + F (x _ {i}), 0).
$$

Establish the identities 

$$
F (x) = F (- \infty) + F ^ {+} (x) - F ^ {-} (x),
$$

$$
\| F \| _ {T V [ a, b ]} = F ^ {+} (b) - F ^ {+} (a) + F ^ {-} (b) - F ^ {-} (a),
$$

and 

$$
\| F \| _ {T V} = F ^ {+} (+ \infty) + F ^ {-} (+ \infty)
$$

for every interval $[ a , b ]$ , where $\begin{array} { r } { F ( - \infty ) : = \operatorname* { l i m } _ { x  - \infty } F ( x ) , F ^ { + } ( + \infty ) : = } \end{array}$ $\scriptstyle \operatorname* { l i m } _ { x \to + \infty } F ^ { + } ( x )$ , and $F ^ { - } ( + \infty ) : = \operatorname* { l i m } _ { x \to + \infty } F ^ { - } ( x )$ . (Hint: The main dificulty comes from the fact that a partition $x _ { 0 } < . . . < x _ { n } \leq x$ that is good for $F ^ { + }$ need not be good for $F ^ { - }$ , and vice versa. However, this can be fixed by taking a good partition for $F ^ { + }$ and a good partition for $F ^ { - }$ and combining them together into a common refinement.) 

From Proposition 1.6.34 and Theorem 1.6.25 we immediately obtain 

Corollary 1.6.35 (BV diferentiation theorem). Every bounded variation function is diferentiable almost everywhere. 

Exercise 1.6.40. Call a function locally of bounded variation if it is of bounded variation on every compact interval $[ a , b ]$ . Show that every function that is locally of bounded variation is diferentiable almost everywhere. 

Exercise 1.6.41 (Lipschitz diferentiation theorem, one-dimensional case). A function $f : \textbf { R }  \textbf { R }$ is said to be Lipschitz continuous if there exists a constant $C > 0$ such that $| f ( x ) - f ( y ) | \leq C | x -$ $y |$ for all $x , y \in \mathbf { R } ;$ the smallest $C$ with this property is known as the Lipschitz constant of $f .$ . Show that every Lipschitz continuous function $F$ is locally of bounded variation, and hence diferentiable almost everywhere. Furthermore, show that the derivative $F ^ { \prime }$ , when it exists, is bounded in magnitude by the Lipschitz constant of $F$ . 

Remark 1.6.36. The same result is true in higher dimensions, and is known as the Radamacher diferentiation theorem, but we will defer the proof of this theorem to Section 2.2, when we have the powerful tool of the Fubini-Tonelli theorem (Corollary 1.7.23) available, that is particularly useful for deducing higher-dimensional results in analysis from lower-dimensional ones. 

Exercise 1.6.42. A function $f : \mathbf { R }  \mathbf { R }$ is said to be convex if one has $f ( ( 1 - t ) x + t y ) \leq ( 1 - t ) f ( x ) + t f ( y )$ for all $x < y$ and $0 < t < 1$ Show that if $f$ is convex, then it is continuous and almost everywhere diferentiable, and its derivative $f ^ { \prime }$ is equal almost everywhere to a monotone non-decreasing function, and so is itself almost everywhere diferentiable. (Hint: Drawing the graph of $f ,$ , together with a number of chords and tangent lines, is likely to be very helpful in providing visual intuition.) Thus we see that in some sense, convex functions are “almost everywhere twice diferentiable”. Similar claims also hold for concave functions, of course. 

1.6.4. The second fundamental theorem of calculus. We are now finally ready to attack the second fundamental theorem of calculus in the cases where $F$ is not assumed to be continuously diferentiable. We begin with the case when $F : [ a , b ] \to \mathbf { R }$ is monotone non-decreasing. From Theorem 1.6.25 (extending $F$ to the rest of the real line if needed), this implies that $F$ is diferentiable almost everywhere in $[ a , b ]$ , so $F ^ { \prime }$ is defined a.e.; from monotonicity we see that $F ^ { \prime }$ is non-negative whenever it is defined. Also, an easy modification of Exercise 1.6.1 shows that $F ^ { \prime }$ is measurable. 

One half of the second fundamental theorem is easy: 

Proposition 1.6.37 (Upper bound for second fundamental theorem). Let $F : [ a , b ] \to \mathbf { R }$ be monotone non-decreasing (so that, as discussed above, $F ^ { \prime }$ is defined almost everywhere, is unsigned, and is measurable). Then 

$$
\int_ {[ a, b ]} F ^ {\prime} (x) d x \leq F (b) - F (a).
$$

In particular, $F ^ { \prime }$ is absolutely integrable. 

Proof. It is convenient to extend $F$ to all of R by declaring $F ( x ) : =$ $F ( b )$ for $x > b$ and $F ( x ) : = F ( a )$ for $x < a$ , then $F$ is now a bounded monotone function on $\mathbf { R } ,$ , and $F ^ { \prime }$ vanishes outside of $[ a , b ]$ . As $F$ is almost everywhere diferentiable, the Newton quotients 

$$
f _ {n} (x) := \frac {F (x + 1 / n) - F (x)}{1 / n}
$$

converge pointwise almost everywhere to $F ^ { \prime }$ . Applying Fatou’s lemma (Corollary1.4.47), we conclude that 

$$
\int_ {[ a, b ]} F ^ {\prime} (x) d x \leq \operatorname * {l i m i n f} _ {n \to \infty} \int_ {[ a, b ]} \frac {F (x + 1 / n) - F (x)}{1 / n} d x.
$$

The right-hand side can be rearranged as 

$$
\operatorname * {l i m i n f} _ {n \to \infty} n (\int_ {[ a + 1 / n, b + 1 / n ]} F (y) d y - \int_ {[ a, b ]} F (x) d x)
$$

which can be rearranged further as 

$$
\operatorname * {l i m i n f} _ {n \to \infty} n (\int_ {[ b, b + 1 / n ]} F (x) d x - \int_ {[ a, a + 1 / n ]} F (x) d x).
$$

Since $F$ is equal to $F ( b )$ for the first integral and is at least $F ( a )$ for the second integral, this expression is at most 

$$
\leq \liminf _ {n \to \infty} n (F (b) / n - F (a) / n) = F (b) - F (a)
$$

and the claim follows. 

Exercise 1.6.43. Show that any function of bounded variation has an (almost everywhere defined) derivative that is absolutely integrable. 

In the Lipschitz case, one can do better: 

Exercise 1.6.44 (Second fundamental theorem for Lipschitz functions). Let $F : [ a , b ] \ \to \ \mathbf { R }$ be Lipschitz continuous. Show that $\begin{array} { r } { \int _ { [ a , b ] } F ^ { \prime } ( x ) ~ d x = F ( b ) - F ( a ) } \end{array}$ . (Hint: Argue as in the proof of Proposition 1.6.37, but use the dominated convergence theorem (Theorem 1.4.49) in place of Fatou’s lemma (Corollary1.4.47).) 

Exercise 1.6.45 (Integration by parts formula). Let $F , G : [ a , b ] \to$ R be Lipschitz continuous functions. Show that 

$$
\begin{array}{c} \int_ {[ a, b ]} F ^ {\prime} (x) G (x) d x = F (b) G (b) - F (a) G (a) \\ - \int_ {[ a, b ]} F (x) G ^ {\prime} (x) d x. \end{array}
$$

(Hint: first show that the product of two Lipschitz continuous functions on $[ a , b ]$ is again Lipschitz continuous.) 

Now we return to the monotone case. Inspired by the Lipschitz case, one may hope to recover equality in Proposition 1.6.37 for such functions $F$ . However, there is an important obstruction to this, which is that all the variation of $F$ may be concentrated in a set of measure zero, and thus undetectable by the Lebesgue integral of $F ^ { \prime }$ This is most obvious in the case of a discontinuous monotone function, such as the (appropriately named) Heaviside function $F : = 1 _ { [ 0 , + \infty ) } ;$ it is clear that $F ^ { \prime }$ vanishes almost everywhere, but $F ( b ) - F ( a )$ is not equal to $\int _ { [ a , b ] } F ^ { \prime } ( x )$ dx if b and $a$ lie on opposite sides of the discontinuity at 0. In fact, the same problem arises for all jump functions: 

Exercise 1.6.46. Show that if $F$ is a jump function, then $F ^ { \prime }$ vanishes almost everywhere. (Hint: use the density argument, starting from piecewise constant jump functions and using Proposition 1.6.37 as the quantitative estimate.) 

One may hope that jump functions - in which all the fluctuation is concentrated in a countable set - are the only obstruction to the second fundamental theorem of calculus holding for monotone functions, and that as long as one restricts attention to continuous monotone functions, that one can recover the second fundamental theorem. However, this is still not true, because it is possible for all the fluctuation to now be concentrated, not in a countable collection of jump discontinuities, but instead in an uncountable set of zero measure, such as the middle thirds Cantor set (Exercise 1.2.9). This can be illustrated by the key counterexample of the Cantor function, also known as the Devil’s staircase function. The construction of this function is detailed in the exercise below. 

Exercise 1.6.47 (Cantor function). Define the functions $F _ { 0 } , F _ { 1 } , F _ { 2 } , \dots ;$ $[ 0 , 1 ]  \mathbf { R }$ recursively as follows: 

1. Set $F _ { 0 } ( x ) : = x$ for all $x \in [ 0 , 1 ]$ 

2. For each $n = 1 , 2 , \ldots$ in turn, define 

$$
F _ {n} (x) := \left\{ \begin{array}{l l} \frac {1}{2} F _ {n - 1} (3 x) & \text { if } x \in [ 0, 1 / 3 ]; \\ \frac {1}{2} & \text { if } x \in (1 / 3, 2 / 3); \\ \frac {1}{2} + \frac {1}{2} F _ {n - 1} (3 x - 2) & \text { if } x \in [ 2 / 3, 1 ] \end{array} \right.
$$

(i) Graph $F _ { 0 } , F _ { 1 } , F _ { 2 }$ , and $F _ { 3 }$ (preferably on a single graph). 

(ii) Show that for each $n = 0 , 1 , . . . , F _ { n }$ is a continuous monotone non-decreasing function with $F _ { n } ( 0 ) = 0$ and $F _ { n } ( 1 ) = 1$ (Hint: induct on n.) 

(iii) Show that for each $n = 0 , 1 , . . . ,$ one has $| F _ { n + 1 } ( x ) - F _ { n } ( x ) | \leq$ $2 ^ { - n }$ for each $x \in [ 0 , 1 ]$ . Conclude that the $F _ { n }$ converge uniformly to a limit $F : [ 0 , 1 ]  \mathbf { R }$ . This limit is known as the Cantor function. 

(iv) Show that the Cantor function F is continuous and monotone non-decreasing, with $F ( 0 ) = 0$ and $F ( 1 ) = 1$ 

(v) Show that if $x \in [ 0 , 1 ]$ lies outside the middle thirds Cantor set (Exercise 1.2.9), then F is constant in a neighbourhood of x, and in particular $F ^ { \prime } ( x ) = 0$ . Conclude that $\begin{array} { r } { \int _ { [ 0 , 1 ] } F ^ { \prime } ( x ) \ d x = 0 \neq 1 = F ( 1 ) - F ( 0 ) } \end{array}$ , so that the second fundamental theorem of calculus fails for this function. 

(vi) Show that $\begin{array} { r } { F ( \sum _ { n = 1 } ^ { \infty } a _ { n } 3 ^ { - n } ) = \sum _ { n = 1 } ^ { \infty } \frac { a _ { n } } { 2 } 2 ^ { - n } } \end{array}$ for any digits $a _ { 1 } , a _ { 2 } , \ldots \in \{ 0 , 2 \}$ . Thus the Cantor function, in some sense, converts base three expansions to base two expansions. 

(1) Let $\begin{array} { r } { I = [ \sum _ { i = 1 } ^ { n } \frac { a _ { i } } { 3 ^ { i } } , \sum _ { i = 1 } ^ { n } \frac { a _ { i } } { 3 ^ { i } } + \frac { 1 } { 3 ^ { n } } ] } \end{array}$ be one of the intervals used in the $n ^ { t h }$ cover $I _ { n }$ of $C$ (see Exercise 1.2.9), thus $n \geq 0$ and $a _ { 1 } , \ldots , a _ { n } \in \{ 0 , 2 \}$ . Show that I is an interval of length $3 ^ { - n }$ but $F ( I )$ is an interval of length $2 ^ { - n }$ 

(2) Show that F is not diferentiable at any element of the Cantor set C. 

Remark 1.6.38. This example shows that the classical derivative $\begin{array} { r } { F ^ { \prime } ( x ) : = \operatorname* { l i m } _ { h \to 0 ; h \neq 0 } \frac { F ( x + h ) - \hat { F } ( x ) } { h } } \end{array}$ of a function has some defects; it cannot $\mathrm { { ^ { 6 6 } s e e ^ { 5 } } }$ some of the variation of a continuous monotone function such as the Cantor function. In §1.13 of An epsilon of room, Vol. I, this will be rectified by introducing the concept of the weak derivative of a function, which despite the name, is more able than the strong derivative to detect this type of singular variation behaviour. (We will also encounter in Section 1.7.3 the Lebesgue-Stieltjes integral, which is another (closely related) way to capture all of the variation of a monotone function, and which is related to the classical derivative via the Lebesgue-Radon-Nikodym theorem, see §1.2 of An epsilon of room, Vol. I.) 

In view of this counterexample, we see that we need to add an additional hypothesis to the continuous monotone non-increasing function F before we can recover the second fundamental theorem. One such hypothesis is absolute continuity. To motivate this definition, let us recall two existing definitions: 

(i) A function $F : \mathbf { R }  \mathbf { R }$ is continuous if, for every $\varepsilon > 0$ and $x _ { 0 } \in \mathbf { R }$ , there exists a $\delta > 0$ such that $| F ( b ) - F ( a ) | \leq$ ε whenever $( a , b )$ is an interval of length at most $\delta$ that contains $x _ { 0 }$ . 

(ii) A function $F : \mathbf { R }  \mathbf { R }$ is uniformly continuous if, for every $\varepsilon > 0$ , there exists a $\delta > 0$ such that $| F ( b ) - F ( a ) | \leq \varepsilon$ whenever $( a , b )$ is an interval of length at most $\delta .$ 

Definition 1.6.39. A function $F : \mathbf { R }  \mathbf { R }$ is said to be absolutely continuous if, for every $\varepsilon > 0$ , there exists a $\delta > 0$ such that $\begin{array} { r } { \sum _ { j = 1 } ^ { n } | F ( b _ { j } ) - F ( a _ { j } ) | \leq \varepsilon } \end{array}$ whenever $( a _ { 1 } , b _ { 1 } ) , \dotsc , ( a _ { n } , b _ { n } )$ is a finite collection of disjoint intervals of total length $\textstyle \sum _ { j = 1 } ^ { n } b _ { j } - a _ { j }$ at most $\delta .$ . 

We define absolute continuity for a function $F : [ a , b ]  \mathbf { R }$ defined on an interval $[ a , b ]$ similarly, with the only diference being that the intervals $[ a _ { j } , b _ { j } ]$ are of course now required to lie in the domain $[ a , b ]$ of F. 

The following exercise places absolute continuity in relation to other regularity properties: 

Exercise 1.6.48. (i) Show that every absolutely continuous function is uniformly continuous and therefore continuous. 

(ii) Show that every absolutely continuous function is of bounded variation on every compact interval $[ a , b ]$ . (Hint: first show this is true for any suficiently small interval.) In particular (by Exercise 1.6.40), absolutely continuous functions are diferentiable almost everywhere. 

(iii) Show that every Lipschitz continuous function is absolutely continuous. 

(iv) Show that the function $x \mapsto { \sqrt { x } }$ is absolutely continuous, but not Lipschitz continuous, on the interval [0, 1]. 

(v) Show that the Cantor function from Exercise 1.6.47 is continuous, monotone, and uniformly continuous, but not absolutely continuous, on [0, 1]. 

(vi) If $f : \mathbf { R }  \mathbf { R }$ is absolutely integrable, show that the indefinite integral $\begin{array} { r } { F ( x ) : = \int _ { [ - \infty , x ] } f ( y ) } \end{array}$ dy is absolutely continuous, and that F is diferentiable almost everywhere with $F ^ { \prime } ( x ) = f ( x )$ for almost every x. 

(vii) Show that the sum or product of two absolutely continuous functions on an interval $[ a , b ]$ remains absolutely continuous. What happens if we work on R instead of on $[ a , b ] ?$ 

Exercise 1.6.49. (i) Show that absolutely continuous functions map null sets to null sets, i.e. if $F : \mathbf { R }  \mathbf { R }$ is absolutely continuous and E is a null set then $F ( E ) : = \{ F ( x ) : x \in E \}$ is also a null set. 

(ii) Show that the Cantor function does not have this property. 

For absolutely continuous functions, we can recover the second fundamental theorem of calculus: 

Theorem 1.6.40 (Second fundamental theorem for absolutely continuous functions). Let $F : [ a , b ]  \mathbf { R }$ be absolutely continuous. Then $\begin{array} { r } { \int _ { [ a , b ] } F ^ { \prime } ( x ) ~ d x = F ( b ) - F ( a ) } \end{array}$ 

Proof. Our main tool here will be Cousin’s theorem (Exercise 1.6.23). 

By Exercise $1 . 6 . 4 3 , F ^ { \prime }$ is absolutely integrable. By Exercise 1.5.10, $F ^ { \prime }$ is thus uniformly integrable. Now let $\varepsilon > 0$ . By Exercise 1.5.13, we can find $\kappa > 0$ such that $\begin{array} { r } { \int _ { U } | F ^ { \prime } ( x ) | \ d x \leq \varepsilon } \end{array}$ whenever $U \subset [ a , b ]$ is a measurable set of measure at most κ. (Here we adopt the convention that $F ^ { \prime }$ vanishes outside of $[ a , b ] . )$ By making κ small enough, we may also assume from absolute continuity that $\begin{array} { r } { \sum _ { j = 1 } ^ { n } | F ( b _ { j } ) - F ( a _ { j } ) | \leq \varepsilon } \end{array}$ whenever $( a _ { 1 } , b _ { 1 } ) , \dotsc , ( a _ { n } , b _ { n } )$ is a finite collection of disjoint intervals of total length $\textstyle \sum _ { j = 1 } ^ { n } b _ { j } - a _ { j }$ at most κ. 

Let $E \subset [ a , b ]$ be the set of points x where $F$ is not diferentiable, together with the endpoints $a , b .$ , as well as the points where x is not a Lebesgue point of $F ^ { \prime }$ . thus E is a null set. By outer regularity (or the definition of outer measure) we can find an open set U containing $E$ of measure $m ( U ) < \kappa$ . In particular, $\begin{array} { r } { \int _ { U } \left| F ^ { \prime } ( x ) \right| d x \le \varepsilon } \end{array}$ 

Now define a gauge function $\delta : [ a , b ]  ( 0 , + \infty )$ as follows. 

(i) If $x \in E$ , we define $\delta ( x ) > 0$ to be small enough that the open interval $( x - \delta ( x ) , x + \delta ( x ) )$ lies in $U$ 

(ii) If $x \notin E ,$ then F is diferentiable at x and x is a Lebesgue point of $F ^ { \prime }$ . We let $\delta ( x ) > 0$ be small enough that $\left| F ( y ) - \right.$ $F ( x ) - ( y - x ) F ^ { \prime } ( x ) | \leq \varepsilon | y - x |$ holds whenever $| y - x | \leq \delta ( x )$ and such that $\begin{array} { r } { | \frac { 1 } { | I | } \int _ { I } F ^ { \prime } ( y ) \ d y - F ^ { \prime } ( x ) | \le \varepsilon } \end{array}$ whenever I is an interval containing x of length at most $\delta ( x )$ ; such a $\delta ( x )$ exists by the definition of diferentiability, and of Lebesgue point. We rewrite these properties using $b i g \ – O$ notation $\boldsymbol { \downarrow ^ { 1 7 } }$ as $F ( y ) - F ( x ) = ( y - x ) F ^ { \prime } ( x ) + O ( \varepsilon | y - x | )$ and $\begin{array} { r } { \int _ { I } F ^ { \prime } ( y ) \ d y = } \end{array}$ |I|F<sup>0</sup>(x) + O(ε|I|). 

Applying Cousin’s theorem, we can find a partition $a = t _ { 0 } < t _ { 1 } <$ $\dots < t _ { k } = b$ with $k \geq 1$ , together with real numbers $t _ { j } ^ { \ast } \in [ t _ { j - 1 } , t _ { j } ]$ for each $1 \le j \le k$ and $t _ { j } - t _ { j - 1 } \leq \delta ( t _ { j } ^ { * } )$ 

We can express $F ( b ) - F ( a )$ as a telescoping series 

$$
F (b) - F (a) = \sum_ {j = 1} ^ {k} F (t _ {j}) - F (t _ {j - 1}).
$$

To estimate the size of this sum, let us first consider those $j$ for which $t _ { j } ^ { * } \in E$ . Then, by construction, the intervals $( t _ { j - 1 } , t _ { j } )$ are disjoint in $U$ . By construction of $\kappa ,$ we thus have 

$$
\sum_ {j: t _ {j} ^ {*} \in E} | F (t _ {j}) - F (t _ {j - 1}) | \leq \varepsilon
$$

and thus 

$$
\sum_ {j: t _ {j} ^ {*} \in E} F (t _ {j}) - F (t _ {j - 1}) = O (\varepsilon).
$$

Next, we consider those $j$ for which $t _ { j } ^ { * } \notin E$ . By construction, for those $j$ we have 

$$
F (t _ {j}) - F (t _ {j} ^ {*}) = (t _ {j} - t _ {j} ^ {*}) F ^ {\prime} (t _ {j} ^ {*}) + O (\varepsilon | t _ {j} - t _ {j} ^ {*} |)
$$

and 

$$
F (t _ {j} ^ {*}) - F (t _ {j - 1}) = (t _ {j} ^ {*} - t _ {j - 1}) F ^ {\prime} (t _ {j} ^ {*}) + O (\varepsilon | t _ {j} ^ {*} - t _ {j - 1} |)
$$

and thus 

$$
F (t _ {j}) - F (t _ {j - 1}) = (t _ {j} - t _ {j - 1}) F ^ {\prime} (t _ {j} ^ {*}) + O (\varepsilon | t _ {j} - t _ {j - 1} |).
$$

On the other hand, from construction again we have 

$$
\int_ {[ t _ {j - 1}, t _ {j} ]} F ^ {\prime} (y) d y = (t _ {j} - t _ {j - 1}) F ^ {\prime} (t _ {j} ^ {*}) + O (\varepsilon | t _ {j} - t _ {j - 1} |)
$$

and thus 

$$
F (t _ {j}) - F (t _ {j - 1}) = \int_ {[ t _ {j - 1}, t _ {j} ]} F ^ {\prime} (y) d y + O (\varepsilon | t _ {j} - t _ {j - 1} |).
$$

Summing in $j ,$ , we conclude that 

$$
\sum_ {j: t _ {j} ^ {*} \not \in E} F (t _ {j}) - F (t _ {j - 1}) = \int_ {S} F ^ {\prime} (y) d y + O (\varepsilon (b - a)),
$$

where $S$ is the union of all the $[ t _ { j - 1 } , t _ { j } ]$ with $t _ { j } ^ { * } ~ \notin ~ E$ . By construction, this set is contained in $[ a , b ]$ and contains $[ a , b ] \backslash U$ . Since $\begin{array} { r } { \int _ { U } \left| F ^ { \prime } ( x ) \right| d x \le \varepsilon . } \end{array}$ , we conclude that 

$$
\int_ {S} F ^ {\prime} (y) d y = \int_ {[ a, b ]} F ^ {\prime} (y) d y + O (\varepsilon).
$$

Putting everything together, we conclude that 

$$
F (b) - F (a) = \int_ {[ a, b ]} F ^ {\prime} (y) d y + O (\varepsilon) + O (\varepsilon | b - a |).
$$

Since $\varepsilon > 0$ was arbitrary, the claim follows. 

Combining this result with Exercise 1.6.48, we obtain a satisfactory classification of the absolutely continuous functions: 

Exercise 1.6.50. Show that a function $F : [ a , b ]  \mathbf { R }$ is absolutely continuous if and only if it takes the form $\begin{array} { r } { F ( x ) = \int _ { [ a , x ] } f ( y ) \ d y + C } \end{array}$ for some absolutely integrable $f : [ a , b ]  \mathbf { R }$ and a constant $C .$ . 

Exercise 1.6.51 (Compatibility of the strong and weak derivatives in the absolutely continuous case). Let $F : [ a , b ] \to \mathbf { R }$ be an absolutely continuous function, and let $\phi : [ a , b ] \to \mathbf { R }$ be $\mathrm { a }$ continuously diferentiable function supported in a compact subset of $( a , b )$ . Show that $\begin{array} { r } { \int _ { [ a , b ] } F ^ { \prime } \phi ( x ) \ d x = - \int _ { [ a , b ] } F \phi ^ { \prime } ( x ) } \end{array}$ dx. 

Inspecting the proof of Theorem 1.6.40, we see that the absolute continuity was used primarily in two ways: firstly, to ensure the almost everywhere existence, and to control an exceptional null set $E$ . It turns out that one can achieve the latter control by making a diferent hypothesis, namely that the function $F$ is everywhere diferentiable rather than merely almost everywhere diferentiable. More precisely, we have 

Proposition 1.6.41 (Second fundamental theorem of calculus, again). Let $[ a , b ]$ be a compact interval of positive length, let $F : [ a , b ]  \mathbf { R }$ be a diferentiable function, such that $F ^ { \prime }$ is absolutely integrable. Then the Lebesgue integral $\int _ { [ a , b ] } F ^ { \prime } ( x )$ dx of $F ^ { \prime }$ is equal to $F ( b ) - F ( a )$ 

Proof. This will be similar to the proof of Theorem 1.6.40, the one main new twist being that we need several open sets U instead of just one. Let $E \subset [ a , b ]$ be the set of points x which are not Lebesgue points of $F ^ { \prime }$ , together with the endpoints $a , b .$ . This is a null set. Let $\varepsilon > 0$ , and then let $\kappa > 0$ be small enough that $\begin{array} { r } { \int _ { U } | F ^ { \prime } ( x ) | \ d x \ \leq \varepsilon } \end{array}$ whenever $U$ is measurable with $m ( U ) \leq \kappa .$ . We can also ensure that $\kappa \leq \varepsilon$ 

For every natural number $m = 1 , 2 , . . .$ . we can find an open set $U _ { m }$ containing E of measure $m ( U _ { m } ) \leq \kappa / 4 ^ { m }$ . In particular we see that $m ( \bigcup _ { m = 1 } ^ { \infty } U _ { m } ) \leq \kappa$ and thus $\begin{array} { r } { \int _ { \bigcup _ { m = 1 } ^ { \infty } U _ { m } } | F ^ { \prime } ( x ) | \ d x \leq \varepsilon } \end{array}$ 

Now define a gauge function $\delta : [ a , b ]  ( 0 , + \infty )$ as follows. 

(i) If $x \in E$ , we define $\delta ( x ) > 0$ to be small enough that the open interval $( x - \delta ( x ) , x + \delta ( x ) )$ lies in $U _ { m }$ , where m is the first natural number such that $| F ^ { \prime } ( x ) | \leq 2 ^ { m }$ , and also small enough that $| F ( y ) - F ( x ) - ( y - x ) F ^ { \prime } ( x ) | \leq \varepsilon | y - x |$ holds whenever $| y - x | \leq \delta ( x )$ . (Here we crucially use the everywhere diferentiability to ensure that $f ^ { \prime } ( x )$ exists and is finite here.) 

(ii) If $x \notin E .$ , we let $\delta ( x ) > 0$ be small enough that $| F ( y ) - F ( x ) -$ $( y - x ) F ^ { \prime } ( x ) | \leq \varepsilon | y - x |$ holds whenever $| y - x | \leq \delta ( x )$ , and such that $\begin{array} { r } { | \frac { 1 } { | I | } \int _ { I } F ^ { \prime } ( y ) \ d y - F ^ { \prime } ( x ) | \ \le \ \varepsilon } \end{array}$ whenever I is an interval containing x of length at most $\delta ( x )$ , exactly as in the proof of Theorem 1.6.40. 

Applying Cousin’s theorem, we can find a partition $a = t _ { 0 } < t _ { 1 } <$ $\dots < t _ { k } = b$ with $k \geq 1$ , together with real numbers $t _ { j } ^ { \ast } \in [ t _ { j - 1 } , t _ { j } ]$ for each $1 \le j \le k$ and $t _ { j } - t _ { j - 1 } \leq \delta ( t _ { j } ^ { * } )$ . 

As before, we express $F ( b ) - F ( a )$ as a telescoping series 

$$
F (b) - F (a) = \sum_ {j = 1} ^ {k} F (t _ {j}) - F (t _ {j - 1}).
$$

For the contributions of those $j$ with $t _ { j } ^ { * } \notin E$ , we argue exactly as in the proof of Theorem 1.6.40 to conclude eventually that 

$$
\sum_ {j: t _ {j} ^ {*} \not \in E} F (t _ {j}) - F (t _ {j - 1}) = \int_ {S} F ^ {\prime} (y) d y + O (\varepsilon (b - a)),
$$

where $S$ is the union of all the $[ t _ { j - 1 } , t _ { j } ]$ with $t _ { j } ^ { * } \not \in E$ . Since 

$$
\int_ {[ a, b ] \setminus S} | F ^ {\prime} (x) | d x \leq \int_ {\bigcup_ {m = 1} ^ {\infty} U _ {m}} | F ^ {\prime} (x) | d x \leq \varepsilon
$$

we thus have 

$$
\int_ {S} F ^ {\prime} (y) d y = \int_ {[ a, b ]} F ^ {\prime} (y) d y + O (\varepsilon).
$$

Now we turn to those $j$ with $t _ { j } ^ { * } \in E$ . By construction, we have 

$$
F (t _ {j}) - F (t _ {j - 1}) = (t _ {j} - t _ {j - 1}) F ^ {\prime} (t _ {j} ^ {*}) + O (\varepsilon | t _ {j} - t _ {j - 1} |)
$$

fir these intervals, and so 

$$
\sum_ {j: t _ {j} ^ {*} \in E} F (t _ {j}) - F (t _ {j - 1}) = (\sum_ {j: t _ {j} ^ {*} \in E} (t _ {j} - t _ {j - 1}) F ^ {\prime} (t _ {j} ^ {*})) + O (\varepsilon (b - a)).
$$

Next, for each $j$ we have $F ^ { \prime } ( t _ { i } ^ { * } ) \leq 2 ^ { m }$ and $[ t _ { j - 1 } , t _ { j } ] \subset U _ { m }$ for some natural number $m = 1 , 2 , . . . ,$ by construction. By countable additivity, we conclude that 

$$
(\sum_ {j: t _ {j} ^ {*} \in E} (t _ {j} - t _ {j - 1}) F ^ {\prime} (t _ {j} ^ {*})) \leq \sum_ {m = 1} ^ {\infty} 2 ^ {m} m (U _ {m}) \leq \sum_ {m = 1} ^ {\infty} 2 ^ {m} \varepsilon / 4 ^ {m} = O (\varepsilon).
$$

Putting all this together, we again have 

$$
F (b) - F (a) = \int_ {[ a, b ]} F ^ {\prime} (y) d y + O (\varepsilon) + O (\varepsilon | b - a |).
$$

Since $\varepsilon > 0$ was arbitrary, the claim follows. 

Remark 1.6.42. The above proposition is yet another illustration of how the property of everywhere diferentiability is significantly better than that of almost everywhere diferentiability. In practice, though, the above proposition is not as useful as one might initially think, because there are very few methods that establish the everywhere diferentiability of a function that do not also establish continuous diferentiability (or at least Riemann integrability of the derivative), at which point one could just use Theorem 1.6.7 instead. 

Exercise 1.6.52. Let $F : [ - 1 , 1 ] \to \mathbf { R }$ be the function defined by setting $F ( x ) : = x ^ { 2 } \sin ( { \frac { 1 } { x ^ { 3 } } } )$ when x is non-zero, and $F ( 0 ) : = 0$ . Show that $F$ is everywhere diferentiable, but the deriative $F ^ { \prime }$ is not absolutely integrable, and so the second fundamental theorem of calculus does not apply in this case (at least if we interpret $\int _ { [ a , b ] } F ^ { \prime } ( x )$ dx using the absolutely convergent Lebesgue integral). See however the next exercise. 

Exercise 1.6.53 (Henstock-Kurzweil integral). Let $[ a , b ]$ be a compact interval of positive length. We say that a function $f : [ a , b ]  \mathbf { R }$ is Henstock-Kurzweil integrable with integral $L \in \mathbf { R }$ if for every $\varepsilon > 0$ there exists a gauge function $\delta : [ a , b ]  ( 0 , + \infty )$ such that one has 

$$
\left| \sum_ {j = 1} ^ {k} f \left(t _ {j} ^ {*}\right) \left(t _ {j} - t _ {j - 1}\right) - L \right| \leq \varepsilon
$$

whenever $k \geq 1$ and $a = t _ { 0 } < t _ { 1 } < . . . < t _ { k } = b$ and $t _ { 1 } ^ { * } , \ldots , t _ { k } ^ { * }$ are such that $t _ { j } ^ { \ast } \in [ t _ { j - 1 } , t _ { j } ]$ and $| t _ { j } - t _ { j - 1 } | \leq \delta ( t _ { j } ^ { * } )$ for every $1 \leq j \leq k$ When this occurs, we call $L$ the Henstock-Kurzweil integral of $f$ and write it as $\textstyle \int _ { [ a , b ] } f ( x )$ dx. 

(i) Show that if a function is Henstock-Kurzweil integrable, it has a unique Henstock-Kurzweil integral. (Hint: use Cousin’s theorem.) 

(ii) Show that if a function is Riemann integrable, then it is Henstock-Kurzweil integrable, and the Henstock-Kurzweil integral $\textstyle \int _ { [ a , b ] } f ( x )$ dx is equal to the Riemann integral $\textstyle \int _ { a } ^ { b } f ( x )$ dx. 

(iii) Show that if a function $f : [ a , b ]  \mathbf { R }$ is everywhere defined, everywhere finite, and is absolutely integrable, then it is Henstock-Kurzweil integrable, and the Henstock-Kurzweil integral $\textstyle \int _ { [ a , b ] } f ( x )$ dx is equal to the Lebesgue integral $\int _ { [ a , b ] } f ( x ) d x$ (Hint: this is a variant of the proof of Theorem 1.6.40 or Proposition 1.6.41.) 

(iv) Show that if $F : [ a , b ] \to \mathbf { R }$ is everywhere diferentiable, then $F ^ { \prime }$ is Henstock-Kurzweil integrable, and the Henstock-Kurzweil integral $\int _ { [ a , b ] } F ^ { \prime } ( x )$ dx is equal to $F ( b ) - F ( a )$ (Hint: this is a variant of the proof of Theorem 1.6.40 or Proposition 1.6.41.) 

(v) Explain why the above results give an alternate proof of Exercise 1.6.4 and of Proposition 1.6.41. 

Remark 1.6.43. As the above exercise indicates, the Henstock-Kurzweil integral (also known as the Denjoy integral or Perron integral) extends the Riemann integral and the absolutely convergent Lebesgue integral, at least as long as one restricts attention to functions that are defined and are finite everywhere (in contrast to the Lebesgue integral, which is willing to tolerate functions being infinite or undefined so long as this only occurs on a null set). It is the notion of integration that is most naturally associated with the fundamental theorem of calculus for everywhere diferentiable functions, as seen in part 4 of the above exercise; it can also be used as a unified framework for all the proofs in this section that invoked Cousin’s theorem. The Henstock-Kurzweil integral can also integrate some (highly oscillatory) functions that the Lebesgue integral cannot, such as the derivative $F ^ { \prime }$ of the function $F$ appearing in Exercise 1.6.52. This is analogous to how conditional summation lim $\begin{array} { r } { N \to \infty \sum _ { n = 1 } ^ { N } a _ { n } } \end{array}$ can sum conditionally convergent series $\textstyle \sum _ { n = 1 } ^ { \infty } a _ { n }$ , even if they are not absolutely integrable. However, much as conditional summation is not always well-behaved with respect to rearrangement, the Henstock-Kurzweil integral does not always react well to changes of variable; also, due to its reliance on the order structure of the real line R, it is dificult to extend the Henstock-Kurzweil integral to more general spaces, such as the Euclidean space $\mathbf { R } ^ { d }$ , or to abstract measure spaces. 

## 1.7. Outer measures, pre-measures, and product measures

In this text so far, we have focused primarily on one specific example of a countably additive measure, namely Lebesgue measure. This measure was constructed from a more primitive concept of Lebesgue outer measure, which in turn was constructed from the even more primitive concept of elementary measure. 

It turns out that both of these constructions can be abstracted. In this section, we will give the Carath´eodory extension theorem, which constructs a countably additive measure from any abstract outer measure; this generalises the construction of Lebesgue measure from Lebesgue outer measure. One can in turn construct outer measures from another concept known as a pre-measure, of which elementary measure is a typical example. 

With these tools, one can start constructing many more measures, such as Lebesgue-Stieltjes measures, product measures, and Hausdorf measures. With a little more efort, one can also establish the Kolmogorov extension theorem, which allows one to construct a variety of measures on infinite-dimensional spaces, and is of particular importance in the foundations of probability theory, as it allows one to set up probability spaces associated to both discrete and continuous random processes, even if they have infinite length. 

The most important result about product measure, beyond the fact that it exists, is that one can use it to evaluate iterated integrals, and to interchange their order, provided that the integrand is either unsigned or absolutely integrable. This fact is known as the Fubini-Tonelli theorem, and is an absolutely indispensable tool for computing integrals, and for deducing higher-dimensional results from lower-dimensional ones. 

In this section we will however omit a very important way to construct measures, namely the Riesz representation theorem, which is discussed in §1.10 of An epsilon of room, Vol. I. 

1.7.1. Outer measures and the Carath´eodory extension theorem. We begin with the abstract concept of an outer measure. 

Definition 1.7.1 (Abstract outer measure). Let X be a set. An abstract outer measure (or outer measure for short) is a map $\mu ^ { * } : 2 ^ { X } \to$ $[ 0 , + \infty ]$ that assigns an unsigned extended real number $\mu ^ { \ast } ( E ) \ \in$ $[ 0 , + \infty ]$ to every set $E \subset X$ which obeys the following axioms: 

(i) (Empty set) $\mu ^ { * } ( \varnothing ) = 0$ 

(ii) (Monotonicity) If $E \subset F$ , then $\mu ^ { * } ( E ) \leq \mu ^ { * } ( F )$ 

(iii) (Countable subadditivity) If $E _ { 1 } , E _ { 2 } , \dots \subset X$ is a countable sequence of subsets of X, then $\begin{array} { r } { \mu ^ { * } ( \bigcup _ { n = 1 } ^ { \infty } E _ { n } ) \leq \sum _ { n = 1 } ^ { \infty } \mu ^ { * } ( E _ { n } ) } \end{array}$ 

Outer measures are also known as exterior measures. 

Thus, for instance, Lebesgue outer measure $m ^ { * }$ is an outer measure (see Exercise 1.2.3). On the other hand, Jordan outer measure $m ^ { * , ( J ) }$ is only finitely subadditive rather than countably subadditive and thus is not, strictly speaking, an outer measure; for this reason this concept is often referred to as Jordan outer content rather than Jordan outer measure. 

Note that outer measures are weaker than measures in that they are merely countably subadditive, rather than countably additive. On the other hand, they are able to measure all subsets of X, whereas measures can only measure a σ-algebra of measurable sets. 

In Definition 1.2.2, we used Lebesgue outer measure together with the notion of an open set to define the concept of Lebesgue measurability. This definition is not available in our more abstract setting, as we do not necessarily have the notion of an open set. An alternative definition of measurability was put forth in Exercise 1.2.17, but this still required the notion of a box or an elementary set, which is still not available in this setting. Nevertheless, we can modify that definition to give an abstract definition of measurability: 

Definition 1.7.2 (Carath´eodory measurability). Let $\mu ^ { * }$ be an outer measure on a set X. A set $E \subset X$ is said to be Carath´eodory measurable with respect to $\mu ^ { * }$ if one has 

$$
\mu^ {*} (A) = \mu^ {*} (A \cap E) + \mu^ {*} (A \backslash E)
$$

for every set $A \subset X$ 

Exercise 1.7.1 (Null sets are Carath´eodory measurable). Suppose that E is a null set for an outer measure $\mu ^ { * } \ ( \mathrm { i . e . } \ \mu ^ { * } ( E ) = 0 )$ . Show that E is Carath´eodory measurable with respect to $\mu ^ { * }$ 

Exercise 1.7.2 (Compatibility with Lebesgue measurability). Show that a set $E ~ \subset ~ \mathbf { R } ^ { d }$ is Carath´eodory measurable with respect to Lebesgue outer measurable if and only if it is Lebesgue measurable. (Hint: one direction follows from Exercise 1.2.17. For the other direction, first verify simple cases, such as when E is a box, or when E or A are bounded.) 

The construction of Lebesgue measure can then be abstracted as follows: 

Theorem 1.7.3 (Carath´eodory extension theorem). Let $\mu ^ { * } : 2 ^ { X } \to$ $[ 0 , + \infty ]$ be an outer measure on a set $X$ , let B be the collection of all subsets of X that are Carath´eodory measurable with respect to $\mu ^ { * }$ , and let $\mu : B \to [ 0 , + \infty ]$ be the restriction of $\mu ^ { * }$ to B (thus $\mu ( E ) : = \mu ^ { * } ( E )$ whenever $E \in B )$ . Then B is a σ-algebra, and $\mu$ is a measure. 

Proof. We begin with the σ-algebra property. It is easy to see that the empty set lies in $B ,$ and that the complement of a set in B lies in B also. Next, we verify that B is closed under finite unions (which will make B a Boolean algebra). Let E, $F \in B .$ , and let $A \subset X$ be arbitrary. By definition, it sufices to show that 

$$
\mu^ {*} (A) = \mu^ {*} (A \cap (E \cup F)) + \mu^ {*} (A \backslash (E \cup F)).\tag{1.31}
$$

To simplify the notation, we partition A into the four disjoint sets 

$$
\begin{array}{l} A _ {0 0} := A \backslash (E \cup F); \\ A _ {1 0} := (A \backslash F) \cap E; \\ A _ {0 1} := (A \backslash E) \cap F; \\ A _ {1 1} := A \cap E \cap F \end{array}
$$

(the reader may wish to draw a Venn diagram here to understand the nature of these sets). Thus (1.31) becomes 

$$
\mu^ {*} (A _ {0 0} \cup A _ {0 1} \cup A _ {1 0} \cup A _ {1 1}) = \mu^ {*} (A _ {0 1} \cup A _ {1 0} \cup A _ {1 1}) + \mu^ {*} (A _ {0 0}).\tag{1.32}
$$

On the other hand, from the Carath´eodory measurability of $E .$ , one has 

$$
\mu^ {*} (A _ {0 0} \cup A _ {0 1} \cup A _ {1 0} \cup A _ {1 1}) = \mu^ {*} (A _ {0 0} \cup A _ {0 1}) + \mu^ {*} (A _ {1 0} \cup A _ {1 1})
$$

and 

$$
\mu^ {*} (A _ {0 1} \cup A _ {1 0} \cup A _ {1 1}) = \mu^ {*} (A _ {0 1}) + \mu^ {*} (A _ {1 0} \cup A _ {1 1})
$$

while from the Carath´eodory measurability of F one has 

$$
\mu^ {*} (A _ {0 0} \cup A _ {0 1}) = \mu^ {*} (A _ {0 0}) + \mu^ {*} (A _ {0 1});
$$

putting these identities together we obtain (1.32). (Note that no subtraction is employed here, and so the arguments still work when some sets have infinite outer measure.) 

Now we verify that B is a σ-algebra. As it is already a Boolean algebra, it sufices (see Exercise 1.7.3 below) to verify that B is closed with respect to countable disjoint unions. Thus, let $E _ { 1 } , E _ { 2 } , . . .$ . be a disjoint sequence of Carath´eodory-measurable sets, and let A be arbitrary. We wish to show that 

$$
\mu^ {*} (A) = \mu^ {*} (A \cap \bigcup_ {n = 1} ^ {\infty} E _ {n}) + \mu^ {*} (A \backslash \bigcup_ {n = 1} ^ {\infty} E _ {n}).
$$

In view of subadditivity, it sufices to show that 

$$
\mu^ {*} (A) \geq \mu^ {*} (A \cap \bigcup_ {n = 1} ^ {\infty} E _ {n}) + \mu^ {*} (A \backslash \bigcup_ {n = 1} ^ {\infty} E _ {n}).
$$

For any $N \geq 1 , \bigcup _ { n = 1 } ^ { N } E _ { n }$ is Carath´eodory measurable (as $\boldsymbol { B }$ is a Boolean algebra), and so 

$$
\mu^ {*} (A) \geq \mu^ {*} (A \cap \bigcup_ {n = 1} ^ {N} E _ {n}) + \mu^ {*} (A \backslash \bigcup_ {n = 1} ^ {N} E _ {n}).
$$

By monotonicity, $\textstyle \mu ^ { * } ( A \backslash \bigcup _ { n = 1 } ^ { N } E _ { n } ) \geq \mu ^ { * } ( A \backslash \bigcup _ { n = 1 } ^ { \infty } E _ { n } )$ . Taking limits as $N \to \infty$ , it thus sufices to show that 

$$
\mu^ {*} (A \cap \bigcup_ {n = 1} ^ {\infty} E _ {n}) \leq \lim _ {N \rightarrow \infty} \mu^ {*} (A \cap \bigcup_ {n = 1} ^ {N} E _ {n}).
$$

But by the Carath´eodory measurability of $\textstyle \bigcup _ { n = 1 } ^ { N } E _ { n }$ , we have 

$$
\mu^ {*} (A \cap \bigcup_ {n = 1} ^ {N + 1} E _ {n}) = \mu^ {*} (A \cap \bigcup_ {n = 1} ^ {N} E _ {n}) + \mu^ {*} (A \cap E _ {N + 1} \backslash \bigcup_ {n = 1} ^ {N} E _ {n})
$$

for any $N \geq 0$ , and thus on iteration 

$$
\lim _ {N \to \infty} \mu^ {*} (A \cap \bigcup_ {n = 1} ^ {N} E _ {n}) = \sum_ {N = 0} ^ {\infty} \mu^ {*} (A \cap E _ {N + 1} \backslash \bigcup_ {n = 1} ^ {N} E _ {n})
$$

On the other hand, from countable subadditivity one has 

$$
\mu^ {*} (A \cap \bigcup_ {n = 1} ^ {\infty} E _ {n}) \leq \sum_ {N = 0} ^ {\infty} \mu^ {*} (A \cap E _ {N + 1} \backslash \bigcup_ {n = 1} ^ {N} E _ {n})
$$

and the claim follows. 

Finally, we show that $\mu$ is a measure. It is clear that $\mu ( \varnothing ) = 0$ , so it sufices to establish countable additivity, thus we need to show 

that 

$$
\mu^ {*} (\bigcup_ {n = 1} ^ {\infty} E _ {n}) = \sum_ {n = 1} ^ {\infty} \mu^ {*} (E _ {n})
$$

whenever $E _ { 1 } , E _ { 2 } , . . .$ . are Carath´eodory-measurable and disjoint. By subadditivity it sufices to show that 

$$
\mu^ {*} (\bigcup_ {n = 1} ^ {\infty} E _ {n}) \geq \sum_ {n = 1} ^ {\infty} \mu^ {*} (E _ {n}).
$$

By monotonicity it sufices to show that 

$$
\mu^ {*} (\bigcup_ {n = 1} ^ {N} E _ {n}) = \sum_ {n = 1} ^ {N} \mu^ {*} (E _ {n})
$$

for any finite N. But from the Carath´eodory measurability of $\textstyle \bigcup _ { n = 1 } ^ { N } E _ { n }$ one has 

$$
\mu^ {*} (\bigcup_ {n = 1} ^ {N + 1} E _ {n}) = \mu^ {*} (\bigcup_ {n = 1} ^ {N} E _ {n}) + \mu^ {*} (E _ {N + 1})
$$

for any $N \geq 0$ , and the claim follows from induction. 

Exercise 1.7.3. Let B be a Boolean algebra on a set $X$ . Show that $\boldsymbol { B }$ is a σ-algebra if and only if it is closed under countable disjoint unions, which means that $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n } \in B$ whenever $E _ { 1 } , E _ { 2 } , E _ { 3 } , . . . \in B$ are a countable sequence of disjoint sets in $B .$ 

Remark 1.7.4. Note that the above theorem, combined with Exercise 1.7.2 gives a slightly alternate way to construct Lebesgue measure from Lebesgue outer measure than the construction given in Section 1.2. This is arguably a more eficient way to proceed, but is also less geometrically intuitive than the approach taken in Section 1.2. 

Remark 1.7.5. From Exercise 1.7.1 we see that the measure µ constructed by the Carath´eodory extension theorem is automatically complete (see Definition 1.4.31). 

Remark 1.7.6. In §1.15 of An epsilon of room, Vol. I, an important example of a measure constructed by Carath´eodory’s theorem is given, namely the d-dimensional Hausdorf measure $\mathcal { H } ^ { d }$ on $\mathbf { R } ^ { n }$ that is good for measuring the size of d-dimensional subsets of $\mathbf { R } ^ { n }$ . 

<!-- === Source: MinerU_markdown_An_introduction_to_measure_theory,_T._Tao,_text_201_2122707919320489993.md (Page 201) === -->

1.7.2. Pre-measures. In previous notes, we saw that finitely additive measures, such as elementary measure or Jordan measure, could be extended to a countably additive measure, namely Lebesgue measure. It is natural to ask whether this property is true in general. In other words, given a finitely additive measure $\mu _ { 0 } : \mathcal { B } _ { 0 } \to [ 0 , + \infty ]$ on a Boolean algebra $B _ { 0 }$ , is it possible to find a σ-algebra B refining $B _ { 0 }$ and a countably additive measure $\mu : B \to [ 0 , + \infty ]$ that extends $\mu _ { 0 } ?$ 

There is an obvious necessary condition in order for $\mu _ { 0 }$ to have a countably additive extension, namely that $\mu _ { 0 }$ already has to be countably additive within $B _ { 0 }$ . More precisely, suppose that $E _ { 1 } , E _ { 2 } , E _ { 3 } , . . . \in$ $B _ { 0 }$ were disjoint sets such that their union $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n }$ was also in $B _ { 0 }$ (Note that this latter property is not automatic as $B _ { 0 }$ is merely a Boolean algebra rather than a σ-algebra.) Then, in order for $\mu _ { 0 }$ to be extendible to a countably additive measure, it is clearly necessary that 

$$
\mu_ {0} (\bigcup_ {n = 1} ^ {\infty} E _ {n}) = \sum_ {n = 1} ^ {\infty} \mu_ {0} (E _ {n}).
$$

Using the Carath´eodory extension theorem, we can show that this necessary condition is also suficient. More precisely, we have 

Definition 1.7.7 (Pre-measure). A pre-measure on a Boolean algebra $B _ { 0 }$ is a finitely additive measure $\mu _ { 0 } : B _ { 0 } \to [ 0 , + \infty ]$ with the property that $\begin{array} { r } { \mu _ { 0 } ( \bigcup _ { n = 1 } ^ { \infty } E _ { n } ) = \sum _ { n = 1 } ^ { \infty } \mu _ { 0 } ( E _ { n } ) } \end{array}$ whenever $E _ { 1 } , E _ { 2 } , E _ { 3 } , . . . \in B _ { 0 }$ are disjoint sets such that $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n }$ is in $B _ { 0 }$ 

## Exercise 1.7.4.

(i) Show that the requirement that $\mu _ { 0 }$ is finitely additive can be relaxed to the condition that $\mu _ { 0 } ( \emptyset ) = 0$ without afecting the definition of a pre-measure. 

(ii) Show that the condition $\begin{array} { r } { \mu _ { 0 } ( \bigcup _ { n = 1 } ^ { \infty } E _ { n } ) = \sum _ { n = 1 } ^ { \infty } \mu _ { 0 } ( E _ { n } ) } \end{array}$ can be relaxed to $\begin{array} { r } { \mu _ { 0 } ( \bigcup _ { n = 1 } ^ { \infty } E _ { n } ) \leq \sum _ { n = 1 } ^ { \infty } \mu _ { 0 } ( E _ { n } ) } \end{array}$ without afecting the definition of a pre-measure. 

(iii) On the other hand, give an example to show that if one performs both of the above two relaxations at once, one starts admitting objects $\mu _ { 0 }$ that are not pre-measures. 

Exercise 1.7.5. Without using the theory of Lebesgue measure, show that elementary measure (on the elementary Boolean algebra) is a pre-measure. (Hint: use Lemma 1.2.6. Note that one has to also deal with co-elementary sets as well as elementary sets in the elementary Boolean algebra.) 

Exercise 1.7.6. Construct a finitely additive measure $\mu _ { 0 } : B _ { 0 } \to $ $[ 0 , + \infty ]$ that is not a pre-measure. (Hint: take $X$ to be the natural numbers, take $B _ { 0 } = 2 ^ { \mathbf { N } }$ to be the discrete algebra, and define $\mu _ { 0 }$ separately for finite and infinite sets.) 

Theorem 1.7.8 (Hahn-Kolmogorov theorem). Every pre-measure $\mu _ { 0 } : \mathcal { B } _ { 0 } \to [ 0 , + \infty ]$ on a Boolean algebra $B _ { 0 }$ in X can be extended to a countably additive measure $\mu : B \to [ 0 , + \infty ]$ 

Proof. We mimic the construction of Lebesgue measure from elementary measure. Namely, for any set $E \subset X$ , define the outer measure $\mu ^ { * } ( E )$ of $E$ to be the quantity 

$$
\mu^ {*} (E) := \inf \left\{\sum_ {n = 1} ^ {\infty} \mu_ {0} \left(E _ {n}\right): E \subset \bigcup_ {n = 1} ^ {\infty} E _ {n}; E _ {n} \in \mathcal {B} _ {0} \text {   for   all   } n \right\}.
$$

It is easy to verify (cf. Exercise 1.2.3) that $\mu ^ { * }$ is indeed an outer measure. Let $\boldsymbol { B }$ be the collection of all sets $E \subset X$ that are Carath´eodory measurable with respect to $\mu ^ { * }$ , and let $\mu$ be the restriction of $\mu ^ { * }$ to $B .$ By the Carath´eodory extension theorem, $\boldsymbol { B }$ is a σ-algebra and $\mu$ is a countably additive measure. 

It remains to show that B contains $B _ { 0 }$ and that $\mu$ extends $\mu _ { 0 }$ Thus, let $E \in B _ { 0 } ;$ we need to show that E is Carath´eodory measurable with respect to $\mu ^ { * }$ and that $\mu ^ { * } ( E ) = \mu _ { 0 } ( E )$ . To prove the first claim, let $A \subset X$ be arbitrary. We need to show that 

$$
\mu^ {*} (A) = \mu^ {*} (A \cap E) + \mu^ {*} (A \backslash E);
$$

by subadditivity, it sufices to show that 

$$
\mu^ {*} (A) \geq \mu^ {*} (A \cap E) + \mu^ {*} (A \backslash E).
$$

We may assume that $\mu ^ { * } ( A )$ is finite, since the claim is trivial otherwise. 

Fix $\varepsilon > 0$ . By definition of $\mu ^ { * }$ , one can find $E _ { 1 } , E _ { 2 } , \dots \in \mathcal { B } _ { 0 }$ covering A such that 

$$
\sum_ {n = 1} ^ {\infty} \mu_ {0} (E _ {n}) \leq \mu^ {*} (A) + \varepsilon .
$$

The sets $E _ { n } \cap E$ lie in $B _ { 0 }$ and cover $A \cap E$ and thus 

$$
\mu^ {*} (A \cap E) \leq \sum_ {n = 1} ^ {\infty} \mu_ {0} (E _ {n} \cap E).
$$

Similarly we have 

$$
\mu^ {*} (A \backslash E) \leq \sum_ {n = 1} ^ {\infty} \mu_ {0} (E _ {n} \backslash E).
$$

Meanwhile, from finite additivity we have 

$$
\mu_ {0} (E _ {n} \cap E) + \mu_ {0} (E _ {n} \backslash E) = \mu_ {0} (E _ {n}).
$$

Combining all of these estimates, we obtain 

$$
\mu^ {*} (A \cap E) + \mu^ {*} (A \backslash E) \leq \mu^ {*} (A) + \varepsilon ;
$$

since $\varepsilon > 0$ was arbitrary, the claim follows. 

Finally, we have to show that $\mu ^ { * } ( E ) = \mu _ { 0 } ( E )$ . Since E covers itself, we certainly have $\mu ^ { * } ( E ) \leq \mu _ { 0 } ( E )$ . To show the converse inequality, it sufices to show that 

$$
\sum_ {n = 1} ^ {\infty} \mu_ {0} (E _ {n}) \geq \mu_ {0} (E)
$$

whenever $E _ { 1 } , E _ { 2 } , \dots \in \mathcal { B } _ { 0 }$ cover E. By replacing each $E _ { n }$ with the smaller set $\textstyle E _ { n } \backslash \bigcup _ { m = 1 } ^ { n - 1 } E _ { m }$ (which still lies in $B _ { 0 }$ , and still covers $E )$ we may assume without loss of generality (thanks to the monotonicity of $\mu _ { 0 } )$ that the $E _ { n }$ are disjoint. Similarly, by replacing each $E _ { n }$ with the smaller set $E _ { n } \cap E$ we may assume without loss of generality that the union of the $E _ { n }$ is exactly equal to $E .$ . But then the claim follows from the hypothesis that $\mu _ { 0 }$ is a pre-measure (and not merely a finitely additive measure).  

Let us call the measure $\mu$ constructed in the above proof the Hahn-Kolmogorov extension of the pre-measure $\mu _ { 0 }$ . Thus, for instance, from Exercise 1.7.2, the Hahn-Kolmogorov extension of elementary measure (with the convention that co-elementary sets have infinite elementary measure) is Lebesgue measure. This is not quite the unique extension of $\mu _ { 0 }$ to a countably additive measure, though. For instance, one could restrict Lebesgue measure to the Borel $\sigma -$ algebra, and this would still be a countably additive extension of elementary measure. However, the extension is unique within its own σ-algebra: 

Exercise 1.7.7. Let $\mu _ { 0 } : B _ { 0 } \to [ 0 , + \infty ]$ be a pre-measure, let $\mu :$ $B \to [ 0 , + \infty ]$ be the Hahn-Kolmogorov extension of $\mu _ { 0 }$ , and let $\mu ^ { \prime }$ : $B ^ { \prime } \to [ 0 , + \infty ]$ be another countably additive extension of $\mu _ { 0 }$ . Suppose also that $\mu _ { 0 }$ is $\sigma { - } f i n i t e .$ , which means that one can express the whole space $X$ as the countable union of sets $E _ { 1 } , E _ { 2 } , \dots \in \mathcal { B } _ { 0 }$ for which $\mu _ { 0 } ( E _ { n } ) < \infty$ for all $n .$ . Show that $\mu$ and $\mu ^ { \prime }$ agree on their common domain of definition. In other words, show that $\mu ( E ) = \mu ^ { \prime } ( E )$ for all $E \in B \cap B ^ { \prime }$ . (Hint: first show that $\mu ^ { \prime } ( E ) \leq \mu ^ { * } ( E )$ for all $E \in B ^ { \prime } .$ ) 

Exercise 1.7.8. The purpose of this exercise is to show that the $\sigma -$ finite hypothesis in Exercise 1.7.7 cannot be removed. Let $\mathcal { A }$ be the collection of all subsets in R that can be expressed as finite unions of half-open intervals $[ a , b )$ . Let $\mu _ { 0 } : { \mathcal { A } }  [ 0 , + \infty ]$ be the function such that $\mu _ { 0 } ( E ) = + \infty$ for non-empty E and $\mu _ { 0 } ( \emptyset ) = 0$ 

(i) Show that $\mu _ { 0 }$ is a pre-measure. 

(ii) Show that $\langle \mathcal { A } \rangle$ is the Borel σ-algebra $B [ \mathbf { R } ]$ 

(iii) Show that the Hahn-Kolmogorov extension $\mu : B [ { \bf R } ] \ $ $[ 0 , + \infty ]$ of $\mu _ { 0 }$ assigns an infinite measure to any non-empty Borel set. 

(iv) Show that counting measure $\#$ (or more generally, $c \#$ for any $c \in ( 0 , + \infty ] )$ is another extension of $\mu _ { 0 }$ on $B [ \mathbf { R } ]$ 

Exercise 1.7.9. Let $\mu _ { 0 } : B _ { 0 } \to [ 0 , + \infty ]$ be a pre-measure which is $\sigma -$ finite (thus X is the countable union of sets in $B _ { 0 }$ of finite $\mu _ { \mathrm { 0 } } { \mathrm { - m e a s u r e } } )$ and let $\mu : B \to [ 0 , + \infty ]$ be the Hahn-Kolmogorov extension of $\mu _ { 0 }$ 

(i) Show that if $E \in B$ , then there exists $F \in \langle B _ { 0 } \rangle$ containing E such that $\mu ( F \backslash E ) = 0$ (thus F consists of the union of E and a null set). Furthermore, show that F can be chosen to be a countable intersection $\textstyle F = \bigcap _ { n = 1 } ^ { \infty } F _ { n }$ of sets $F _ { n }$ , each of which is a countable union $\textstyle F _ { n } = \bigcup _ { m = 1 } ^ { \infty } F _ { n , m }$ of sets $F _ { n , m }$ in $B _ { 0 }$ 

(ii) If $E \in B$ has finite measure $( \mathrm { i . e . } ~ \ \mu ( E ) < \infty )$ , and $\varepsilon > 0$ show that there exists $F \in B _ { 0 }$ such that $\mu ( E \Delta F ) \leq \varepsilon$ 

(iii) Conversely, if E is a set such that for every $\varepsilon > 0$ there exists $F \in B _ { 0 }$ such that $\mu ^ { \ast } ( E \Delta F ) \leq \varepsilon .$ , show that $E \in B$ 

1.7.3. Lebesgue-Stieltjes measure. Now we use the Hahn-Kolmogorov extension theorem to construct a variety of measures. We begin with Lebesgue-Stieltjes measure. 

Theorem 1.7.9 (Existence of Lebesgue-Stieltjes measure). Let F : $\mathbf R  \mathbf R$ be a monotone non-decreasing function, and define the left and right limits 

$$
F _ {-} (x) := \sup _ {y <   x} F (y); \quad F _ {+} (x) := \inf _ {y > x} F (y),
$$

thus one has $F _ { - } ( x ) \leq F ( x ) \leq F _ { + } ( x )$ for all x. Let $B [ \mathbf { R } ]$ be the Borel σ-algebra on R. Then there exists a unique Borel measure $\mu _ { F } : \mathcal { B } [ \mathbf { R } ] \to [ 0 , + \infty ]$ such that 

$$
\mu_ {F} ([ a, b ]) = F _ {+} (b) - F _ {-} (a), \mu_ {F} ([ a, b)) = F _ {-} (b) - F _ {-} (a),\tag{1.33}
$$

$$
\mu_ {F} ((a, b ]) = F _ {+} (b) - F _ {+} (a), \mu_ {F} ((a, b)) = F _ {-} (b) - F _ {+} (a)
$$

for all $- \infty < b < a < \infty$ , and 

$$
\mu_ {F} (\{a \}) = F _ {+} (a) - F _ {-} (a)\tag{1.34}
$$

for all $a \in \mathbf { R }$ 

Proof. (Sketch) For this proof, we will deviate from our previous notational conventions, and allow intervals to be unbounded, thus in particular including the half-infinite intervals $[ a , + \infty ) , ( a , + \infty )$ , $( - \infty , a ] , \ ( - \infty , a )$ and the doubly infinite interval $( - \infty , + \infty )$ as intervals. 

Define the F-volume $| I | _ { F } \in [ 0 , + \infty ]$ of any interval I, adopting the obvious conventions that $F _ { - } ( + \infty ) = \operatorname* { s u p } _ { y \in \mathbf { R } } F ( y )$ and $F _ { + } ( - \infty ) =$ $\operatorname { i n f } _ { y \in \mathbf { R } } F ( y )$ , and also adopting the convention that the empty interval ∅ has zero F-volume, $| \emptyset | _ { F } = 0$ . Note that $F _ { - } ( + \infty )$ could equal $+ \infty$ and $F _ { + } ( - \infty )$ could equal −∞, but in all circumstances the $F _ { - }$ volume $| I | _ { F }$ is well-defined and takes values in $[ 0 , + \infty ]$ , after adopting the obvious conventions to evaluate expressions such as $+ \infty - ( - \infty )$ 

A somewhat tedious case check (Exercise!) gives the additivity property 

$$
| I \cup J | _ {F} = | I | _ {F} + | J | _ {F}
$$

whenever $I , J$ are disjoint intervals that share a common endpoint. As a corollary, we see that if a interval I is partitioned into finitely many disjoint sub-intervals $I _ { 1 } , \ldots , I _ { k }$ , we have $| I | = | I _ { 1 } | + \ldots + | I _ { k } |$ 

Let $B _ { 0 }$ be the Boolean algebra generated by the (possibly infinite) intervals, then $B _ { 0 }$ consists of those sets that can be expressed as a finite union of intervals. (This is slightly larger than the elementary algebra, as it allows for half-infinite intervals such as $[ 0 , + \infty )$ , whereas the elementary algebra does not.) We can define a measure $\mu _ { 0 }$ on this algebra by declaring 

$$
\mu_ {0} (E) = | I _ {1} | _ {F} + \ldots + | I _ {k} | _ {F}
$$

whenever $E = I _ { 1 } \cup \dots \cup I _ { k }$ is the disjoint union of finitely many intervals. One can check (Exercise!) that this measure is well-defined (in the sense that it gives a unique value to $\mu _ { 0 } ( E )$ for each $E \in B _ { 0 } )$ and is finitely additive. We now claim that $\mu _ { 0 }$ is a pre-measure: thus we suppose that $E = B _ { 0 }$ is the disjoint union of countably many sets $E _ { 1 } , E _ { 2 } , \dots \in \mathcal { B } _ { 0 }$ , and wish to show that 

$$
\mu_ {0} (E) = \sum_ {n = 1} ^ {\infty} \mu_ {0} (E _ {n}).
$$

By splitting up $E$ into intervals and then intersecting each of the $E _ { n }$ with these intervals and using finite additivity, we may assume that E is a single interval. By splitting up the $E _ { n }$ into their component intervals and using finite additivity, we may assume that the $E _ { n }$ are also individual intervals. By subadditivity, it sufices to show that 

$$
\mu_ {0} (E) \leq \sum_ {n = 1} ^ {\infty} \mu_ {0} (E _ {n}).
$$

By the definition of $\mu _ { 0 } ( E )$ , one can check that 

$$
\mu_ {0} (E) = \sup _ {K \subset E} \mu_ {0} (K)\tag{1.35}
$$

where $K$ ranges over all compact intervals contained in $E$ (Exercise!). Thus, it sufices to show that 

$$
\mu_ {0} (K) \leq \sum_ {n = 1} ^ {\infty} \mu_ {0} (E _ {n})
$$

for each compact sub-interval K of $E .$ . In a similar spirit, one can show that 

$$
\mu_ {0} (E _ {n}) = \inf _ {U \supset E _ {n}} \mu_ {0} (E _ {n})
$$

where $U$ ranges over all open intervals containing $E _ { n }$ (Exercise!). Using the $\varepsilon / 2 ^ { n }$ trick, it thus sufices to show that 

$$
\mu_ {0} (K) \leq \sum_ {n = 1} ^ {\infty} \mu_ {0} (U _ {n})
$$

whenever $U _ { n }$ is an open interval containing $E _ { n }$ . But by the Heine-Borel theorem, one can cover K by a finite number $\textstyle \bigcup _ { n = 1 } ^ { N } U _ { n }$ of the $U _ { n }$ , hence by finite subadditivity 

$$
\mu_ {0} (K) \leq \sum_ {n = 1} ^ {N} \mu_ {0} (U _ {n})
$$

and the claim follows. 

As $\mu _ { 0 }$ is now verified to be a pre-measure, we may use the Hahn-Kolmogorov extension theorem to extend it to a countably additive measure $\mu$ on a σ-algebra B that contains $B _ { 0 }$ . In particular, B contains all the elementary sets and hence (by Exercise 1.4.14) contains the Borel σ-algebra. Restricting $\mu$ to the Borel σ-algebra we obtain the existence claim. 

Finally, we establish uniqueness. If $\mu ^ { \prime }$ is another Borel measure with the stated properties, then $\mu ^ { \prime } ( K ) = | K | _ { F }$ for every compact interval K, and hence by (1.35) and upward monotone convergence, one has $\mu ^ { \prime } ( I ) = | I | _ { F }$ for every interval (including the unbounded ones). This implies that $\mu ^ { \prime }$ agrees with $\mu _ { 0 }$ on $B _ { 0 }$ , and thus (by Exercise 1.7.7, noting that $\mu _ { 0 }$ is σ-finite) agrees with $\mu$ on Borel measurable sets.  

Exercise 1.7.10. Verify the claims marked “Exercise!” in the above proof. 

The measure $\mu _ { F }$ given by the above theorem is known as the Lebesgue-Stieltjes measure $\mu _ { F }$ of $F$ . (In some texts, this measure is only defined when $F$ is right-continuous, or equivalently if $F = F _ { + } . )$ 

Exercise 1.7.11. Define a Radon measure on R to be a Borel measure $\mu$ obeying the following additional properties: 

(i) (Local finiteness) $\mu ( K ) < \infty$ for every compact $K$ . 

(ii) (Inner regularity) One has $\mu ( E ) = \operatorname* { s u p } _ { K \subset E , K }$ compact $\mu ( K )$ for every Borel set $E .$ 

(iii) (Outer regularity) One has $\begin{array} { r } { \mu ( E ) = \operatorname* { i n f } _ { U \supset E , U } \mathrm { o p e n } \mu ( U ) } \end{array}$ for every Borel set $E$ 

Show that for every monotone function $F : \mathbf { R }  \mathbf { R }$ , the Lebesgue-Stieltjes measure $\mu _ { F }$ is a Radon measure on $\mathbf { R } ;$ conversely, if $\mu$ is a Radon measure on R, show that there exists a monotone function $F : \mathbf { R }  \mathbf { R }$ such that $\mu = \mu _ { F }$ 

Radon measures are studied in more detail in $\ S 1 . 1 0$ of An epsilon of room, Vol. I. 

Exercise 1.7.12 (Near uniqueness). If $F , F ^ { \prime } : \mathbf { R }  \mathbf { R }$ are monotone non-decreasing functions, show that $\mu _ { F } = \mu _ { F ^ { \prime } }$ if and only if there exists a constant $C \in \mathbf { R }$ such that $F _ { + } ( x ) = F _ { + } ^ { \prime } ( x ) + C$ and $F _ { - } ( x ) =$ $F _ { - } ^ { \prime } ( x ) + C$ for all $x \in \textbf { R }$ . Note that this implies that the value of $F$ at its points of discontinuity are irrelevant for the purposes of determining the Lebesgue-Stieltjes measure $\mu _ { F } ;$ in particular, $\mu _ { F } =$ $\mu _ { \boldsymbol { F } _ { + } } = \mu _ { \boldsymbol { F } _ { - } }$ 

In the special case when $F _ { + } ( - \infty ) = 0$ and $F _ { - } ( + \infty ) = 1$ , then $\mu _ { F }$ is a probability measure, and $F _ { + } ( x ) = \mu _ { F } ( ( - \infty , x ] )$ is known as the cumulative distribution function of $\mu _ { F }$ 

Now we give some examples of Lebesgue-Stieltjes measure. 

Exercise 1.7.13 (Lebesgue-Stieltjes measure, absolutely continuous case). 

(i) If $F : \mathbf { R }  \mathbf { R }$ is the identity function $F ( x ) = x$ , show that $\mu _ { F }$ is equal to Lebesgue measure m. 

(ii) If $F : \mathbf { R }  \mathbf { R }$ is monotone non-decreasing and absolutely continuous (which in particular implies that $F ^ { \prime }$ exists and is absolutely integrable, show that $\mu _ { F } = m _ { F ^ { \prime } }$ in the sense of Exercise 1.4.49, thus 

$$
\mu_ {F} (E) = \int_ {E} F ^ {\prime} (x) d x
$$

for any Borel measurable $E _ { : }$ , and 

$$
\int_ {\mathbf {R}} f (x) d \mu_ {F} (x) = \int_ {\mathbf {R}} f (x) F ^ {\prime} (x) d x
$$

for any unsigned Borel measurable $f : \mathbf { R }  [ 0 , + \infty ]$ 

In view of the above exercise, the integral $\int _ { \mathbf { R } } f \ d \mu _ { F }$ is often abbreviated $\textstyle \int _ { \mathbf { R } } f \ d F$ , and referred to as the Lebesgue-Stieltjes integral of $f$ with respect to $F$ . In particular, observe the identity 

$$
\int_ {[ a, b ]} d F = F _ {+} (b) - F _ {-} (a)
$$

for any monotone non-decreasing $F : \mathbf { R }  \mathbf { R }$ and any $- \infty < b <$ $a \ < \ + \infty$ , which can be viewed as yet another formulation of the fundamental theorem of calculus. 

Exercise 1.7.14 (Lebesgue-Stieltjes measure, pure point case). 

(i) If $H : \textbf { R }  \textbf { R }$ is the Heaviside function $H : = 1 _ { [ 0 , + \infty ) }$ ， show that $\mu _ { H }$ is equal to the Dirac measure $\delta _ { 0 }$ at the origin (defined in Example 1.4.22). 

(ii) If $\begin{array} { r } { F = \sum _ { n } c _ { n } J _ { n } } \end{array}$ is a jump function (as defined in Definition 1.6.30), show that $\mu _ { F }$ is equal to the linear combination $\sum c _ { n } \delta _ { x _ { n } }$ of delta functions (as defined in Exercise 1.4.22), where $x _ { n }$ is the point of discontinuity for the basic jump function $J _ { n }$ 

Exercise 1.7.15 (Lebesgue-Stieltjes measure, singular continuous case). 

(i) If $F : \mathbf { R }  \mathbf { R }$ is a monotone non-decreasing function, show that F is continuous if and only if $\mu _ { F } ( \{ x \} ) = 0$ for all $x \in \mathbf { R }$ 

(ii) If F is the Cantor function (defined in Exercise 1.6.47), show that $\mu _ { F }$ is a probability measure supported on the middle-thirds Cantor set (see Exercise 1.2.9) in the sense that $\mu _ { F } ( { \bf R } \backslash { \cal C } ) = 0$ . The measure $\mu _ { F }$ is known as Cantor measure. 

(iii) If $\mu _ { F }$ is Cantor measure, establish the self-similarity properties $\begin{array} { r } { \mu ( \frac { 1 } { 3 } \cdot E ) = \frac { 1 } { 2 } \mu ( E ) } \end{array}$ and $\begin{array} { r } { \mu ( \frac { 1 } { 3 } \cdot E + \frac { 2 } { 3 } ) = \frac { 1 } { 2 } \mu ( E ) } \end{array}$ for every Borel-measurable $E \subset [ 0 , 1 ]$ , where ${ \begin{array} { r } { { \frac { 1 } { 3 } } \cdot E : = \left\{ { \frac { 1 } { 3 } } x : x \in E \right\} } \end{array} }$ 

Exercise 1.7.16 (Connection with Riemann-Stieltjes integral). Let $F : \mathbf { R }  \mathbf { R }$ be monotone non-decreasing, let $[ a , b ]$ be a compact interval, and let $f : [ a , b ]  \mathbf { R }$ be continuous. Suppose that $F$ is continuous at the endpoints $a , b$ of the interval. Show that for every $\varepsilon > 0$ there exists $\delta > 0$ such that 

$$
\left| \sum_ {i = 1} ^ {n} f \left(t _ {i} ^ {*}\right) \left(F \left(t _ {i}\right) - F \left(t _ {i - 1}\right)\right) - \int_ {[ a, b ]} f d F \right| \leq \varepsilon
$$

whenever $a = t _ { 0 } < t _ { 1 } < . . . < t _ { n } = b$ and $t _ { i } ^ { * } \in [ t _ { i - 1 } , t _ { i } ]$ for $1 \ \leq$ $\textit { i } \leq n$ are such that $\begin{array} { r } { \operatorname* { s u p } _ { 1 \leq i \leq n } | t _ { i } - t _ { i - 1 } | \leq \delta } \end{array}$ . In the language of the Riemann-Stieltjes integral, this result asserts that the Lebesgue-Stieltjes integral extends the Riemann-Stieltjes integral. 

Exercise 1.7.17 (Integration by parts formula). Let $F , G : \mathbf { R }  \mathbf { R }$ be monotone non-decreasing and continuous. Show that 

$$
\int_ {[ a, b ]} F d G = - \int_ {[ a, b ]} G d F + F (b) G (b) - F (a) G (a)
$$

for any compact interval $[ a , b ]$ . (Hint: use Exercise 1.7.16.) This formula can be partially extended to the case when one or both of $F , G$ have discontinuities, but care must be taken when $F$ and $G$ are simultaneously discontinuous at the same location. 

1.7.4. Product measure. Given two sets X and Y, one can form their Cartesian product $X \times Y = \{ ( x , y ) : x \in X , y \in Y \}$ . This set is naturally equipped with the coordinate projection maps π<sub>X</sub> : $X \times Y  X$ and $\pi _ { Y } : X \times Y \to Y$ defined by setting $\pi _ { \boldsymbol { X } } ( x , y ) : = x$ and $\pi _ { Y } ( x , y ) : = y$ . One can certainly take Cartesian products $X _ { 1 } \times \ldots \times X _ { d }$ of more than two sets, or even take an infinite product $\Pi _ { \alpha \in A } X _ { \alpha }$ , but for simplicity we will only discuss the theory for products of two sets for now. 

Now suppose that $( X , B _ { X } )$ and $( Y , B _ { Y } )$ are measurable spaces. Then we can still form the Cartesian product $X \times Y$ and the projection maps $\pi _ { X } : X \times Y \to X$ and $\pi _ { Y } : X \times Y \to Y$ . But now we can also form the pullback σ-algebras 

$$
\pi_ {X} ^ {*} (\mathcal {B} _ {X}) := \{\pi_ {X} ^ {- 1} (E): E \in \mathcal {B} _ {X} \} = \{E \times Y: E \in \mathcal {B} _ {X} \}
$$

and 

$$
\pi_ {Y} ^ {*} (\mathcal {B} _ {Y}) := \left\{\pi_ {Y} ^ {- 1} (E): E \in \mathcal {B} _ {Y} \right\} = \left\{X \times F: F \in \mathcal {B} _ {Y} \right\}.
$$

We then define the product σ-algebra $B _ { X } \times B _ { Y }$ to be the σ-algebra generated by the union of these two σ-algebras: 

$$
\mathcal {B} _ {X} \times \mathcal {B} _ {Y} := \langle \pi_ {X} ^ {*} (\mathcal {B} _ {X}) \cup \pi_ {Y} ^ {*} (\mathcal {B} _ {Y}) \rangle .
$$

This definition has several equivalent formulations: 

Exercise 1.7.18. Let $( X , B _ { X } )$ and $( Y , B _ { Y } )$ be measurable spaces. 

(i) Show that $B _ { X } \times B _ { Y }$ is the σ-algebra generated by the sets $E \times F$ with $E \in B _ { X } , Y \in B _ { Y }$ . In other words, $B _ { X } \times B _ { Y }$ is the coarsest σ-algebra on $X \times Y$ with the property that the product of a B -measurable set and a B -measurable set is always $B _ { X } \times B _ { Y }$ measurable. 

(ii) Show that $B _ { X } \times B _ { Y }$ is the coarsest σ-algebra on $X \times Y$ that makes the projection maps $\pi _ { \boldsymbol { X } } , \pi _ { \boldsymbol { Y } }$ both measurable morphisms (see Remark 1.4.33). 

(iii) If $E \in B _ { X } \times B _ { Y }$ , show that the sets $E _ { x } : = \{ y \in Y : ( x , y ) \in$ $E \}$ lie in $B _ { Y }$ for every $x \in X$ , and similarly that the sets $E ^ { y } : = \{ x \in X : ( x , y ) \in E \}$ lie in $\boldsymbol { { B } _ { X } }$ for every $y \in Y$ 

(iv) If $f : X \times Y \to [ 0 , + \infty ]$ is measurable (with respect to $B _ { X } \times B _ { Y } )$ , show that the function $f _ { x } : y \mapsto f ( x , y )$ is $B _ { Y ^ { - } }$ measurable for every $x \in X$ , and similarly that the function $f ^ { y } : x \mapsto f ( x , y )$ is B<sub>X</sub>-measurable for every $y \in Y$ 

(v) If $E \in B _ { X } \times B _ { Y }$ , show that the slices $E _ { x } \ : = \ \{ y \in \ Y$ $( x , y ) \in E \}$ lie in a countably generated σ-algebra. In other words, show that there exists an at most countable collection $\mathcal { A } = \mathcal { A } _ { E }$ of sets (which can depend on E) such that $\{ E _ { x } : x \in X \} \subset \langle A \rangle$ . Conclude in particular that the number of distinct slices $E _ { x }$ is at most $^ { c , }$ the cardinality of the continuum. (The last part of this exercise is only suitable for students who are comfortable with cardinal arithmetic.) 

## Exercise 1.7.19.

(i) Show that the product of two trivial σ-algebras (on two diferent spaces $X , Y )$ is again trivial. 

(ii) Show that the product of two atomic σ-algebras is again atomic. 

(iii) Show that the product of two finite σ-algebras is again finite. 

(iv) Show that the product of two Borel σ-algebras (on two Euclidean spaces $\mathbf { R } ^ { d } , \mathbf { R } ^ { d ^ { \prime } }$ with $d , d ^ { \prime } \geq 1 )$ is again the Borel σ-algebra (on $\mathbf { R } ^ { d } \times \mathbf { R } ^ { d ^ { \prime } } \equiv \mathbf { R } ^ { d + d ^ { \prime } } )$ 

(v) Show that the product of two Lebesgue σ-algebras (on two Euclidean spaces $\mathbf { R } ^ { d } , \mathbf { R } ^ { d ^ { \prime } }$ with d, $d ^ { \prime } \geq 1 )$ is not the Lebesgue σ-algebra. (Hint: argue by contradiction and use Exercise 1.7.18(iii).) 

(vi) However, show that the Lebesgue σ-algebra on $\mathbf { R } ^ { d + d ^ { \prime } }$ is the completion (see Exercise 1.4.26) of the product of the Lebesgue σ-algebras of $\mathbf { R } ^ { d }$ and $\mathbf { R } ^ { d ^ { \prime } }$ with respect to $d + d ^ { \prime } .$ dimensional Lebesgue measure. 

(vii) This part of the exercise is only for students who are comfortable with cardinal arithmetic. Give an example to show that the product of two discrete σ-algebras is not necessarily discrete. 

(viii) On the other hand, show that the product of two discrete σ-algebras $2 ^ { X } , 2 ^ { Y }$ is again a discrete σ-algebra if at least one of the domains $X , Y$ is at most countably infinite. 

Now suppose we have two measure spaces $\left( X , B _ { X } , \mu _ { X } \right)$ and $( Y , B _ { Y } , \mu _ { Y } )$ Given that we can multiply together the sets X and Y to form a product set $X \times Y$ , and can multiply the σ-algebras $\boldsymbol { { B } _ { X } }$ and $B _ { Y }$ together to form a product σ-algebra $B _ { X } \times B _ { Y }$ , it is natural to expect that we 

can multiply the two measures $\mu _ { X } : B _ { X } \to [ 0 , + \infty ]$ and $\mu _ { Y } : B _ { Y } $ $[ 0 , + \infty ]$ to form a product measure $\mu _ { X } \times \mu _ { Y } : \mathcal { B } _ { X } \times \mathcal { B } _ { Y } \to [ 0 , + \infty ]$ ]. In view of the “base times height formula” that one learns in elementary school, one expects to have 

$$
\mu_ {X} \times \mu_ {Y} (E \times F) = \mu_ {X} (E) \mu_ {Y} (F)\tag{1.36}
$$

whenever $E \in B _ { X }$ and $F \in B _ { Y }$ 

To construct this measure, it is convenient to make the assumption that both spaces are $\sigma { - } f i n i t e { : }$ 

Definition 1.7.10 $( \sigma { \mathrm { - f i n i t e } } )$ . A measure space $( X , B , \mu )$ is $\sigma { - } f i n i t e$ if X can be expressed as the countable union of sets of finite measure. 

Thus, for instance, $\mathbf { R } ^ { d }$ with Lebesgue measure is $\sigma { \mathrm { - f i n i t e } }$ , as $\mathbf { R } ^ { d }$ can be expressed as the union of (for instance) the balls $B ( 0 , n )$ for $n = 1 , 2 , 3 , . . . ,$ each of which has finite measure. On the other hand, $\mathbf { R } ^ { d }$ with counting measure is not σ-finite (why?). But most measure spaces that one actually encounters in analysis (including, clearly, all probability spaces) are $\sigma { \mathrm { - f i n i t e } }$ . It is possible to partially extend the theory of product spaces to the non-σ-finite setting, but there are a number of very delicate technical issues that arise and so we will not discuss them here. 

As long as we restrict attention to the σ-finite case, product measure always exists and is unique: 

Proposition 1.7.11 (Existence and uniqueness of product measure). Let $\left( X , B _ { X } , \mu _ { X } \right)$ and $( Y , B _ { Y } , \mu _ { Y } )$ be σ-finite measure spaces. Then there exists a unique measure $\mu _ { X } \times \mu _ { Y }$ on $B _ { X } \times B _ { Y }$ that obeys $\mu _ { X } \times$ $\mu _ { Y } ( E \times F ) = \mu _ { X } ( E ) \mu _ { Y } ( F )$ whenever $E \in B _ { X }$ and $F \in B _ { Y }$ 

Proof. We first show existence. Inspired by the fact that Lebesgue measure is the Hahn-Kolmogorov completion of elementary (pre-)measure, we shall first construct an “elementary product pre-measure” that we will then apply Theorem 1.7.8 to. 

Let $B _ { 0 }$ be the collection of all finite unions 

$$
S := \left(E _ {1} \times F _ {1}\right) \cup \dots \cup \left(E _ {k} \times F _ {k}\right)
$$

of Cartesian products of $B _ { X } { \mathrm { - m e a s u r a b l e } }$ sets $E _ { 1 } , \ldots , E _ { k }$ and $B _ { Y }$ measurable sets $F _ { 1 } , \ldots , F _ { k }$ . (One can think of such sets as being somewhat analogous to elementary sets in Euclidean space, although the analogy is not perfectly exact.) It is not dificult to verify that this is a Boolean algebra (though it is not, in general, a σ-algebra). Also, any set in $B _ { 0 }$ can be easily decomposed into a disjoint union of product sets $E _ { 1 } \times F _ { 1 } , \ldots , E _ { k } \times F _ { k }$ of $B _ { X } { \mathrm { - m e a s u r a b l e } }$ sets and $B _ { Y ^ { - } }$ measurable sets (cf. Exercise 1.1.2). We then define the quantity $\mu _ { 0 } ( S )$ associated such a disjoint union S by the formula 

$$
\mu_ {0} (S) := \sum_ {j = 1} ^ {k} \mu_ {X} (E _ {j}) \mu_ {Y} (F _ {j})
$$

whenever $S$ is the disjoint union of products $E _ { 1 } \times F _ { 1 } , \ldots , E _ { k } \times F _ { k }$ of $\boldsymbol { { B } _ { X } }$ -measurable sets and B -measurable sets. One can show that this definition does not depend on exactly how $S$ is decomposed, and gives a finitely additive measure $\mu _ { 0 } : B _ { 0 } \to [ 0 , + \infty ]$ (cf. Exercise 1.1.2 and Exercise 1.4.33). 

Now we show that $\mu _ { 0 }$ is a pre-measure. It sufices to show that if $S \in B _ { 0 }$ is the countable disjoint union of sets $S _ { 1 } , S _ { 2 } , \ldots \in \mathcal { B } _ { 0 }$ , then $\begin{array} { r } { \mu _ { 0 } ( S ) = \sum _ { n = 1 } ^ { \infty } \mu ( S _ { n } ) } \end{array}$ 

Splitting $S$ up into disjoint product sets, and restricting the $S _ { n }$ to each of these product sets in turn, we may assume without loss of generality (using the finite additivity of $\mu _ { 0 } )$ that $S = E \times F$ for some $E \in B _ { X }$ and $F \in B _ { Y }$ . In a similar spirit, by breaking each $S _ { n }$ up into component product sets and using finite additivity again, we may assume without loss of generality that each $S _ { n }$ takes the form $S _ { n } = E _ { n } \times F _ { n }$ for some $E _ { n } \in B _ { X }$ and $F _ { n } \in B _ { Y }$ . By definition of $\mu _ { 0 }$ our objective is now to show that 

$$
\mu_ {X} (E) \mu_ {Y} (F) = \sum_ {n = 1} ^ {\infty} \mu_ {X} (E _ {n}) \mu_ {Y} (F _ {n}).
$$

To do this, first observe from construction that we have the pointwise identity 

$$
1 _ {E} (x) 1 _ {F} (y) = \sum_ {n = 1} ^ {\infty} 1 _ {E _ {n}} (x) 1 _ {F _ {n}} (y)
$$

for all $x \in X$ and $y \in Y$ . We fix $x \in X$ , and integrate this identity in $y$ (noting that both sides are measurable and unsigned) to conclude that 

$$
\int_ {Y} 1 _ {E} (x) 1 _ {F} (y) d \mu_ {Y} (y) = \int_ {Y} \sum_ {n = 1} ^ {\infty} 1 _ {E _ {n}} (x) 1 _ {F _ {n}} (y) d \mu_ {Y} (y).
$$

The left-hand side simplifies to $1 _ { E } ( x ) \mu _ { Y } ( F )$ . To compute the righthand side, we use the monotone convergence theorem (Theorem 1.4.44) to interchange the summation and integration, and soon see that the right-hand side is $\begin{array} { r } { \sum _ { n = 1 } ^ { \infty } 1 _ { E _ { n } } ( x ) \mu _ { Y } ( F _ { n } ) } \end{array}$ , thus 

$$
1 _ {E} (x) \mu_ {Y} (F) = \sum_ {n = 1} ^ {\infty} 1 _ {E _ {n}} (x) \mu_ {Y} (F _ {n})
$$

for all $x .$ . Both sides are measurable and unsigned in $x ,$ , so we may integrate in X and conclude that 

$$
\int_ {X} 1 _ {E} (x) \mu_ {Y} (F) d \mu_ {X} = \int_ {X} \sum_ {n = 1} ^ {\infty} 1 _ {E _ {n}} (x) \mu_ {Y} (F _ {n}) d \mu_ {X} (x).
$$

The left-hand side here is $\mu _ { X } ( E ) \mu _ { Y } ( F )$ . Using monotone convergence as before, the right-hand side simplifies to $\scriptstyle \sum _ { n = 1 } ^ { \infty } \mu _ { X } ( E _ { n } ) \mu _ { Y } ( F _ { n } )$ , and the claim follows. 

Now that we have established that $\mu _ { 0 }$ is a pre-measure, we may apply Theorem 1.7.8 to extend this measure to a countably additive measure $\mu _ { X } \times \mu _ { Y }$ on a σ-algebra containing $B _ { 0 }$ . By Exercise 1.7.18(2), $\mu _ { X } \times \mu _ { Y }$ is a countably additive measure on $B _ { X } \times B _ { Y }$ , and as it extends $\mu _ { 0 }$ , it will obey (1.36). Finally, to show uniqueness, observe from finite additivity that any measure $\mu _ { X } \times \mu _ { Y }$ on $B _ { X } \times B _ { Y }$ that obeys (1.36) must extend $\mu _ { 0 }$ , and so uniqueness follows from Exercise 1.7.7.  

Remark 1.7.12. When X, Y are not both σ-finite, then one can still construct at least one product measure, but it will, in general, not be unique. This makes the theory much more subtle, and we will not discuss it in these notes. 

Example 1.7.13. From Exercise 1.2.22, we see that the product $m ^ { d } \times m ^ { d ^ { \prime } }$ of the Lebesgue measures $m ^ { d } , m ^ { d ^ { \prime } }$ on $( \mathbf { R } ^ { d } , \mathcal { L } [ \mathbf { R } ^ { d } ] )$ ) and $( \mathbf { R } ^ { d } , \mathcal { L } [ \mathbf { R } ^ { d ^ { \prime } } ] )$ respectively will agree with Lebesgue measure $m ^ { d + d ^ { \prime } }$ on the product space $\mathcal { L } [ \mathbf { R } ^ { d } ] \times \mathcal { L } [ \mathbf { R } ^ { d ^ { \prime } } ]$ , which as noted in Exercise 1.7.19 is a subalgebra of $\mathcal { L } [ \mathbf { R } ^ { d + d ^ { \prime } } ]$ . After taking the completion $\overline { { m ^ { d } \times m ^ { d ^ { \prime } } } }$ of this product measure, one obtains the full Lebesgue measure $m ^ { d + d ^ { \prime } }$ 

Exercise 1.7.20. Let $( X , B _ { X } ) , ( Y , B _ { Y } )$ be measurable spaces. 

(i) Show that the product of two Dirac measures on $( X , B _ { X } )$ $( Y , B _ { Y } )$ is a Dirac measure on $( X \times Y , B _ { X } \times B _ { Y } )$ 

(ii) If $X , Y$ are at most countable, show that the product of the two counting measures on $( X , B _ { X } ) , ( Y , B _ { Y } )$ is the counting measure on $( X \times Y , B _ { X } \times B _ { Y } )$ 

Exercise 1.7.21 (Associativity of product). Let $( X , B _ { X } , \mu _ { X } ) , ( Y , B _ { Y } , \mu _ { Y } )$ $\left( Z , B _ { Z } , \mu _ { Z } \right)$ be σ-finite sets. We may identify the Cartesian products $( X \times Y ) \times Z$ and $X \times ( Y \times Z )$ with each other in the obvious manner. If we do so, show that $\left( \boldsymbol { B } _ { X } \times \boldsymbol { B } _ { Y } \right) \times \boldsymbol { B } _ { Z } = \boldsymbol { B } _ { X } \times \left( \boldsymbol { B } _ { Y } \times \boldsymbol { B } _ { Z } \right)$ and $( \mu _ { X } \times \mu _ { Y } ) \times \mu _ { Z } = \mu _ { X } \times ( \mu _ { Y } \times \mu _ { Z } )$ 

Now we integrate using this product measure. We will need the following technical lemma. Define a monotone class in X is a collection B of subsets of X with the following two closure properties: 

(i) If $E _ { 1 } \subset E _ { 2 } \subset . .$ . are a countable increasing sequence of sets in $B ,$ , then $\textstyle \bigcup _ { n = 1 } ^ { \infty } E _ { n } \in B$ 

(ii) If $E _ { 1 } \supset E _ { 2 } \supset . .$ . are a countable decreasing sequence of sets in B, then $\textstyle \bigcap _ { n = 1 } ^ { \infty } E _ { n } \in B$ 

Lemma 1.7.14 (Monotone class lemma). Let A be a Boolean algebra on X. Then hAi is the smallest monotone class that contains A. 

Proof. Let B be the intersection of all the monotone classes that contain A. Since $\langle \mathcal { A } \rangle$ is clearly one such class, $\boldsymbol { B }$ is a subset of $\langle \mathcal { A } \rangle$ $\mathrm { O u r }$ task is then to show that B contains hAi. 

It is also clear that B is a monotone class that contains ${ \mathcal { A } } .$ . By replacing all the elements of B with their complements, we see that $\boldsymbol { B }$ is necessarily closed under complements. 

For any $E \in { \mathcal { A } }$ , consider the set $\mathcal { C } _ { E }$ of all sets $F \in B$ such that $F \backslash E , E \backslash F , F \cap E$ , and $X \backslash ( E \cup F )$ all lie in $B _ { \cdot }$ . It is clear that $\mathcal { C } _ { E }$ contains $\mathcal { A } ;$ since $\boldsymbol { B }$ is a monotone class, we see that $\mathcal { C } _ { E }$ is also. By definition of $B ,$ , we conclude that $\mathcal { C } _ { E } = B$ for all $E \in { \mathcal { A } }$ 

Next, let D be the set of all $E \in B$ such that $F \backslash E , E \backslash F , F \cap E$ and $X \backslash ( E \cup F )$ all lie in B for all $F \in B$ . By the previous discussion, we see that D contains ${ \mathcal { A } } .$ . One also easily verifies that D is a monotone class. By definition of $B { \mathrm { . } }$ , we conclude that $\mathcal { D } = B$ . Since B is also closed under complements, this implies that B is closed with respect to finite unions. Since this class also contains $\mathcal { A }$ , which contains $\varnothing .$ , we conclude that $\boldsymbol { B }$ is a Boolean algebra. Since $\boldsymbol { B }$ is also closed under increasing countable unions, we conclude that it is closed under arbitrary countable unions, and is thus a σ-algebra. As it contains ${ \mathcal { A } } ,$ it must also contain hAi.  

Theorem 1.7.15 (Tonelli’s theorem, incomplete version). Let $\left( X , B _ { X } , \mu _ { X } \right)$ and $( Y , B _ { Y } , \mu _ { Y } )$ be $\sigma { - } f i n i t e$ measure spaces, and let $f : X \times Y $ $[ 0 , + \infty ]$ be measurable with respect to $B _ { X } \times B _ { Y }$ . Then: 

(i) The functions x $\begin{array} { r } { \mapsto \int _ { Y } f ( x , y ) d \mu _ { Y } ( y ) } \end{array}$ and $\begin{array} { r } { y \mapsto \int _ { X } f ( x , y ) d \mu _ { X } ( x ) } \end{array}$ (which are well-defined, thanks to Exercise 1.7.18) are measurable with respect to $\boldsymbol { { B } _ { X } }$ and $B _ { Y }$ respectively. 

(ii) We have 

$$
\begin{array}{c} \int_ {X \times Y} f (x, y) d \mu_ {X} \times \mu_ {Y} (x, y) \\ = \int_ {X} (\int_ {Y} f (x, y) d \mu_ {Y} (y)) d \mu_ {X} (x) \\ = \int_ {Y} (\int_ {X} f (x, y) d \mu_ {X} (x)) d \mu_ {Y} (y). \end{array}
$$

Proof. By writing the σ-finite space X as an increasing union $X =$ $\textstyle \bigcup _ { n = 1 } ^ { \infty } X _ { n }$ of finite measure sets, we see from several applications of the monotone convergence theorem (Theorem 1.4.44) that it sufices to prove the claims with X replaced by $X _ { n }$ . Thus we may assume without loss of generality that X has finite measure. Similarly we may assume $Y$ has finite measure. Note from (1.36) that this implies that $X \times Y$ has finite measure also. 

Every unsigned measurable function is the increasing limit of unsigned simple functions. By several applications of the monotone convergence theorem (Theorem 1.4.44), we thus see that it sufices to verify the claim when f is a simple function. By linearity, it then suffices to verify the claim when $f$ is an indicator function, thus $f = 1 _ { S }$ for some $S \in B _ { X } \times B _ { Y }$ 

Let C be the set of all $S \in B _ { X } \times B _ { Y }$ for which the claims hold. From the repeated applications of the monotone convergence theorem (Theorem 1.4.44) and the downward monotone convergence theorem (which is available in this finite measure setting) we see that C is a monotone class. 

By direct computation (using (1.36)), we see that C contains as an element any product $S = E \times F$ with $E \in B _ { X }$ and $F \in B _ { Y }$ . By finite additivity, we conclude that C also contains as an element any a disjoint finite union $\boldsymbol { S } = E _ { 1 } \times \boldsymbol { F } _ { 1 } \cup . . . \cup E _ { k } \times \boldsymbol { F } _ { k }$ of such products. This implies that C also contains the Boolean algebra $B _ { 0 }$ in the proof of Proposition 1.7.11, as such sets can always be expressed as the disjoint finite union of Cartesian products of measurable sets. Applying the monotone class lemma, we conclude that C contains $\langle B _ { 0 } \rangle = B _ { X } \times B _ { Y }$ , and the claim follows.  

Remark 1.7.16. Note that Tonelli’s theorem for sums (Theorem 0.0.2) is a special case of the above result when $\mu _ { X } , \mu _ { Y }$ are counting measure. In a similar spirit, Corollary 1.4.46 is the special case when just one of $\mu _ { X } , \mu _ { Y }$ is counting measure. 

Corollary 1.7.17. Let $\left( X , B _ { X } , \mu _ { X } \right)$ and $( Y , B _ { Y } , \mu _ { Y } )$ be σ-finite measure spaces, and let $E \in B _ { X } \times B _ { Y }$ be a null set with respect to $\mu _ { X } \times \mu _ { Y }$ Then for $\mu _ { X }$ -almost every $x \in X$ , the set $E _ { x } : = \{ y \in Y : ( x , y ) \in E \}$ is a µ -null set; and similarly, for µ -almost every $y \in Y$ , the set $E ^ { y } : = \{ x \in X : ( x , y ) \in E \}$ is a $\mu _ { X } - n u l l$ set. 

Proof. Applying the Tonelli theorem to the indicator function $1 _ { E }$ , we conclude that 

$$
0 = \int_ {X} (\int_ {Y} 1 _ {E} (x, y) d \mu_ {Y} (y)) d \mu_ {X} (x) = \int_ {Y} (\int_ {X} 1 _ {E} (x, y) d \mu_ {X} (x)) d \mu_ {Y} (y)
$$

and thus 

$$
0 = \int_ {X} \mu_ {Y} (E _ {x}) d \mu_ {X} (x) = \int_ {Y} \mu_ {X} (E ^ {y}) d \mu_ {Y} (y),
$$

and the claim follows. 

With this corollary, we can extend Tonelli’s theorem to the completion $( X \times Y , \overline { { B _ { X } \times B _ { Y } } } , \overline { { \mu _ { X } \times \mu _ { Y } } } )$ of the product space $( X \times Y , B _ { X } \times$ $B _ { Y } , \mu _ { X } \times \mu _ { Y } )$ , as constructed in Exercise 1.4.26. But we can easily extend the Tonelli theorem to this context: 

Theorem 1.7.18 (Tonelli’s theorem, complete version). Let $\left( X , B _ { X } , \mu _ { X } \right)$ and $( Y , B _ { Y } , \mu _ { Y } )$ be complete σ-finite measure spaces, and let $f : X \times$ $Y  [ 0 , + \infty ]$ be measurable with respect to $\overline { { B _ { X } \times B _ { Y } } }$ . Then: 

(i) For µ<sub>X</sub>-almost every $x \in X$ , the function $y \mapsto f ( x , y )$ is B -measurable, and in particular $\textstyle \int _ { Y } f ( x , y ) \ d \mu _ { Y } ( y )$ exists. Furthermore, the (µ -almost everywhere defined) map $x \mapsto$ $\textstyle { \int _ { Y } f ( x , y ) }$ dµ is B -measurable. 

(ii) For µ -almost every $y \in Y$ , the function x $\mapsto \ f ( x , y )$ is B -measurable, and in particular $\textstyle \int _ { X } f ( x , y ) \ d \mu _ { X } ( x )$ exists. Furthermore, the (µ -almost everywhere defined) map $y \mapsto$ $\textstyle \int _ { X } f ( x , y )$ dµ is B -measurable. 

(iii) We have 

(1.37) 

$$
\begin{array}{c} \int_ {X \times Y} f (x, y) d \overline {{\mu_ {X} \times \mu_ {Y}}} (x, y) = \int_ {X} (\int_ {Y} f (x, y) d \mu_ {Y} (y)) d \mu_ {X} (x) \\ = \int_ {X} (\int_ {Y} f (x, y) d \mu_ {Y} (y)) d \mu_ {X} (x). \end{array}
$$

Proof. From Exercise 1.4.28, every measurable set in $\overline { { B _ { X } \times B _ { Y } } }$ is equal to a measurable set in $B _ { X } \times B _ { Y }$ outside of a $\mu _ { X } \times \mu _ { Y } \mathrm { - n u l l }$ set. This implies that the $\overline { { B _ { X } \times B _ { Y } } } \mathrm { - m e a s u r a b l e }$ function f agrees with a $\ B _ { X } \times B _ { Y } { \mathrm { - m e a s u r a b l e } }$ function $\tilde { f }$ outside of a $\mu _ { X } \times \mu _ { Y } \mathrm { - n u l l }$ set $E$ (as can be seen by expressing $f$ as the limit of simple functions). From Corollary 1.7.17, we see that for $\mu _ { X }$ -almost every $x \in X$ , the function $y \mapsto f ( x , y )$ agrees with $y \mapsto { \tilde { f } } ( x , y )$ outside of a $\mu _ { Y } \mathrm { - n u l l }$ set (and is in particular measurable, as $( Y , B _ { Y } , \mu _ { Y } )$ is complete); and similarly for $\mu _ { Y } { \mathrm { - a l m o s t } }$ every $y \in Y$ , the function $x \mapsto f ( x , y )$ agrees with $x \mapsto { \tilde { f } } ( x , y )$ outside of a $\mu _ { X } \mathrm { - n u l l }$ set and is measurable, and the claim follows.  

Specialising to the case when $f$ is an indicator function $f = 1 _ { E }$ , we conclude 

Corollary 1.7.19 (Tonelli’s theorem for sets). Let $\left( X , B _ { X } , \mu _ { X } \right)$ and $( Y , B _ { Y } , \mu _ { Y } )$ be complete σ-finite measure spaces, and let $E \in \overline { { B _ { X } \times B _ { Y } } }$ Then: 

(i) For µ -almost every $x \in X$ , the set $E _ { x } : = \{ y \in Y : ( x , y ) \in$ $E \}$ lies in $B _ { Y }$ , and the (µ -almost everywhere defined) map $x \mapsto \mu _ { Y } ( E _ { x } )$ is B -measurable. 

(ii) For µ -almost every $y \in Y$ , the set $E ^ { y } : = \{ x \in X : ( x , y ) \in$ $E \}$ lies in $\boldsymbol { { B } _ { X } }$ , and the (µ -almost everywhere defined) map $y \mapsto \mu _ { X } ( E ^ { y } )$ is B -measurable. 

(iii) We have 

$$
\begin{array}{c} \overline {{\mu_ {X} \times \mu_ {Y}}} (E) = \int_ {X} \mu_ {Y} (E _ {x}) d \mu_ {X} (x) \\ = \int_ {X} \mu_ {X} (E ^ {y}) d \mu_ {X} (x). \end{array}\tag{1.38}
$$

Exercise 1.7.22. The purpose of this exercise is to demonstrate that Tonelli’s theorem can fail if the σ-finite hypothesis is removed, and also that product measure need not be unique. Let X is the unit interval [0, 1] with Lebesgue measure m (and the Lebesgue σ-algebra ${  { \mathcal { L } } } ( [ 0 , 1 ] ) )$ ) and Y is the unit interval [0, 1] with counting measure (and the discrete σ-algebra $2 ^ { [ 0 , 1 ] } ) \#$ . Let $f : = 1 _ { E }$ be the indicator function of the diagonal $E : = \{ ( x , x ) : x \in [ 0 , 1 ] \}$ 

(i) Show that f is measurable in the product σ-algebra. 

(ii) Show that $\begin{array} { r } { \int _ { X } ( \int _ { Y } f ( x , y ) \ d \# ( y ) ) d m ( x ) = 1 } \end{array}$ 

(iii) Show that $\begin{array} { r } { \int _ { Y } ( \int _ { X } f ( x , y ) \ d m ( x ) ) d \# ( y ) = 0 . } \end{array}$ 

(iv) Show that there is more than one measure $\mu$ on $\mathcal { L } ( [ 0 , 1 ] ) \times$ 2<sup>[0,1]</sup> with the property that $\mu ( E \times F ) = m ( E ) \# ( F )$ for all $E \in \mathcal { L } ( [ 0 , 1 ] )$ and $F \in 2 ^ { [ 0 , 1 ] }$ . (Hint: use the two diferent ways to perform a double integral to create two diferent measures.) 

Remark 1.7.20. If $f$ is not assumed to be measurable in the product space (or its completion), then of course the expression $\begin{array} { r } { \int _ { X \times Y } f ( x , y ) d \overline { { \mu _ { X } \times \mu _ { Y } } } ( x , y ) } \end{array}$ does not make sense. Furthermore, in this case the remaining two expressions in (1.37) may become diferent as well (in some models of set theory, at least), even when X and $Y$ are finite measure. For 

instance, let us assume the continuum hypothesis, which implies that the unit interval [0, 1] can be placed in one-to-one correspondence with the first uncountable ordinal $\omega _ { 1 }$ . Let ≺ be the ordering of [0, 1] that is associated to this ordinal, let $E : = \{ ( x , y ) \in [ 0 , 1 ] ^ { 2 } : x \prec y \}$ and let $f : = 1 _ { E }$ . Then, for any $y \in [ 0 , 1 ]$ , there are at most countably many x such that $x \prec y$ , and so $\int _ { [ 0 , 1 ] } f ( x , y )$ dx exists and is equal to zero for every y. On the other hand, for every $x \in [ 0 , 1 ]$ , one has $x \prec y$ for all but countably many $y \in [ 0 , 1 ]$ , and so $\int _ { [ 0 , 1 ] } f ( x , y )$ dy exists and is equal to one for every y, and so the last two expressions in (1.37) exist but are unequal. (In particular, Tonelli’s theorem implies that E cannot be a Lebesgue measurable subset of $[ 0 , 1 ] ^ { 2 } . )$ Thus we see that measurability in the product space is an important hypothesis. (There do however exist models of set theory (with the axiom of choice) in which such counterexamples cannot be constructed, at least in the case when X and Y are the unit interval with Lebesgue measure.) 

Tonelli’s theorem is for the unsigned integral, but it leads to an important analogue for the absolutely integral, known as Fubini’s theorem: 

Theorem 1.7.21 (Fubini’s theorem). Let $\left( X , B _ { X } , \mu _ { X } \right)$ and $( Y , B _ { Y } , \mu _ { Y } )$ be complete σ-finite measure spaces, and let $f : X \times Y \to \mathbf { C }$ be absolutely integrable with respect to $B _ { X } \times B _ { Y }$ . Then: 

(i) For $\mu _ { X }$ -almost every $x \in X$ , the function $y \mapsto f ( x , y )$ is absolutely integrable with respect to $\mu _ { Y }$ , and in particular $\textstyle \int _ { Y } f ( x , y ) \ d \mu _ { Y } ( y )$ exists. Furthermore, the (µ -almost everywhere defined) map $\begin{array} { r } { x \mapsto \int _ { Y } f ( x , y ) \ d \mu _ { Y } ( y ) } \end{array}$ is absolutely integrable with respect to $\mu _ { X }$ 

(ii) For µ -almost every $y \in Y$ , the function $x \mapsto f ( x , y )$ is absolutely integrable with respect to $\mu _ { X }$ , and in particular $\textstyle \int _ { X } f ( x , y ) \ d \mu _ { X } ( x )$ exists. Furthermore, the (µ -almost everywhere defined) map $\begin{array} { r } { y \mapsto \int _ { X } f ( x , y ) \ d \mu _ { X } ( x ) } \end{array}$ is absolutely integrable with respect to $\mu _ { Y }$ 

(iii) We have 

$$
\begin{array}{c} \int_ {X \times Y} f (x, y) d \overline {{\mu_ {X} \times \mu_ {Y}}} (x, y) = \int_ {X} (\int_ {Y} f (x, y) d \mu_ {Y} (y)) d \mu_ {X} (x) \\ = \int_ {X} (\int_ {Y} f (x, y) d \mu_ {Y} (y)) d \mu_ {X} (x). \end{array}
$$

Proof. By taking real and imaginary parts we may assume that $f$ is real; by taking positive and negative parts we may assume that $f$ is unsigned. But then the claim follows from Tonelli’s theorem; note from (1.37) that $\begin{array} { r } { \int _ { X } ( \int _ { Y } f ( x , y ) \ d \mu _ { Y } ( y ) ) \ d \mu _ { X } ( x ) } \end{array}$ is finite, and so $\textstyle \int _ { Y } f ( x , y ) \ d \mu _ { Y } ( y ) < \infty$ for µ -almost every $x \in X$ , and similarly $\textstyle \int _ { X } f ( x , y ) d \mu _ { X } ( x ) < \infty$ for $\mu _ { Y } { \mathrm { - a l m o s t } }$ every $y \in Y$  

Exercise 1.7.23. Give an example of a Borel measurable function $f$ : $[ 0 , 1 ] ^ { 2 }  \mathbf { R }$ such that the integrals $\int _ { [ 0 , 1 ] } f ( x , y )$ dy and $\textstyle \int _ { [ 0 , 1 ] } f ( x , y )$ dx exist and are absolutely integrable for all $x \in [ 0 , 1 ]$ and $\dot { y ^ { \mathrm { ~ \scriptsize ~ \in ~ } [ 0 , 1 ] } }$ respectively, and that $\begin{array} { r l } { \int _ { [ 0 , 1 ] } ( \int _ { [ 0 , 1 ] } f ( x , y ) d y ) } \end{array}$ dx and $\begin{array} { r l } { \int _ { [ 0 , 1 ] } ( \int _ { [ 0 , 1 ] } f ( x , y ) d y ) } \end{array}$ dx exist and are absolutely integrable, but such that 

$$
\int_ {[ 0, 1 ]} \left(\int_ {[ 0, 1 ]} f (x, y) d y\right) d x \neq \int_ {[ 0, 1 ]} \left(\int_ {[ 0, 1 ]} f (x, y) d y\right) d x.
$$

are unequal. (Hint: adapt the example from Remark 0.0.3.) Thus we see that Fubini’s theorem fails when one drops the hypothesis that f is absolutely integrable with respect to the product space. 

Remark 1.7.22. Despite the failure of Tonelli’s theorem in the $\sigma -$ finite setting, it is possible to (carefully) extend Fubini’s theorem to the non-σ-finite setting, as the absolute integrability hypotheses, when combined with Markov’s inequality (Exercise 1.4.36(vi)), can provide a substitute for the σ-finite property. However, we will not do so here, and indeed I would recommend proceeding with extreme caution when performing any sort of interchange of integrals or invoking of product measure when one is not in the σ-finite setting. 

Informally, Fubini’s theorem allows one to always interchange the order of two integrals, as long as the integrand is absolutely integrable in the product space (or its completion). In particular, specialising 

to Lebesgue measure, we have 

$$
\int_ {\mathbf {R} ^ {d + d ^ {\prime}}} f (x, y) d (x, y) = \int_ {\mathbf {R} ^ {d}} (\int_ {\mathbf {R} ^ {d ^ {\prime}}} f (x, y) d y) d x = \int_ {\mathbf {R} ^ {d ^ {\prime}}} (\int_ {\mathbf {R} ^ {d}} f (x, y) d x) d y
$$

whenever $f : \mathbf { R } ^ { d + d ^ { \prime } }  \mathbf { C }$ is absolutely integrable. In view of this, we often write dxdy (or dydx) for $d ( x , y )$ 

By combining Fubini’s theorem with Tonelli’s theorem, we can recast the absolute integrability hypothesis: 

Corollary 1.7.23 (Fubini-Tonelli theorem). Let $\left( X , B _ { X } , \mu _ { X } \right)$ and $( Y , B _ { Y } , \mu _ { Y } )$ be complete σ-finite measure spaces, and let $f : X \times Y $ C be measurable with respect to $\overline { { B _ { X } \times B _ { Y } } }$ . If 

$$
\int_ {X} (\int_ {Y} | f (x, y) | d \mu_ {Y} (y)) d \mu_ {X} (x) <   \infty
$$

(note the left-hand side always exists, by Tonelli’s theorem) then f is absolutely integrable with respect to $\overline { { B _ { X } \times B _ { Y } } }$ , and in particular the conclusions ofFubini’s theorem hold. Similarly ifwe use $\begin{array} { r } { \int _ { Y } ( \int _ { X } | f ( x , y ) | d \mu _ { X } ( x ) ) d \mu _ { Y } ( y ) } \end{array}$ instead of $\textstyle { \int _ { X } ( \int _ { Y } | f ( x , y ) | ~ d \mu _ { Y } ) ~ d \mu _ { X } }$ 

The Fubini-Tonelli theorem is an indispensable tool for computing integrals. We give some basic examples below: 

Exercise 1.7.24 (Area interpretation of integral). Let $( X , B , \mu )$ be a σ-finite measure space, and let R be equipped with Lebesgue measure m and the Borel σ-algebra $B [ \mathbf { R } ]$ . Show that if $f : X \to [ 0 , + \infty ]$ is measurable if and only if the set $\{ ( x , t ) \in X \times \mathbf { R } : 0 \leq t \leq f ( x ) \}$ is measurable in $B \times B [ \mathbf { R } ]$ , in which case we have 

$$
(\mu \times m) (\{(x, t) \in X \times \mathbf {R}: 0 \leq t \leq f (x) \}) = \int_ {X} f (x) d \mu (x).
$$

Similarly if we replace $\{ ( x , t ) \in X \times \mathbf { R } : 0 \leq t \leq f ( x ) \} { \mathrm { ~ b y ~ } } \{ ( x , t ) \in$ $X \times \mathbf { R } : 0 \leq t < f ( x ) \}$ 

Exercise 1.7.25 (Distribution formula). Let $( X , B , \mu )$ be a $\sigma { \mathrm { - f i n i t e } }$ measure space, and let $f : X \to [ 0 , + \infty ]$ be measurable. Show that 

$$
\int_ {X} f (x) d \mu (x) = \int_ {[ 0, + \infty ]} \mu (\{x \in X: f (x) \geq \lambda \}) d \lambda .
$$

(Note that the integrand on the right-hand side is monotone and thus Lebesgue measurable.) Similarly if we replace $\{ x \in X : f ( x ) \geq \lambda \}$ } by $\{ x \in X : f ( x ) > \lambda \}$ 

Exercise 1.7.26 (Approximations to the identity). Let $P : \mathbf { R } ^ { d } $ $\mathbf { R } ^ { + }$ be a good kernel (see Exercise 1.6.27), and let $\begin{array} { r } { P _ { t } ( x ) : = \frac { 1 } { t ^ { d } } P ( \frac { x } { t } ) } \end{array}$ be the associated rescaled functions. Show that if $f : \mathbf { R } ^ { d }  \mathbf { C }$ is absolutely integrable, that $f * P _ { t }$ converges in $L ^ { 1 }$ norm to $f$ as $t \to 0$ (Hint: use the density argument. You will need an upper bound on $\| f * { \cal P } _ { t } \| _ { L ^ { 1 } ( { \bf R } ^ { d } ) }$ which can be obtained using Tonelli’s theorem.) 

Chapter 2 

Related articles 

## 2.1. Problem solving strategies

The purpose of this section is to list (in no particular order) a number of common problem solving strategies for attacking real analysis exercises such as that presented in this text. Some of these strategies are specific to real analysis type problems, but others are quite general and would be applicable to other mathematical exercises. 

2.1.1. Split up equalities into inequalities. If one has to show that two numerical quantities X and Y are equal, try proving that $X \leq Y$ and $Y \leq X$ separately. Often one of these will be very easy, and the other one harder; but the easy direction may still provide some clue as to what needs to be done to establish the other direction. Exercise 1.1.6(iii) is a typical problem in which this strategy can be applied. 

In a similar spirit, to show that two sets E and F are equal, try proving that $E \subset F$ and $F \subset E$ . See for instance the proof of Lemma 1.2.11 for a simple example of this. 

2.1.2. Give yourself an epsilon of room. If one has to show that $X \ \leq \ Y$ , try proving that $X \leq Y + \varepsilon$ for any $\varepsilon > 0$ . (This trick combines well with §2.1.1.) See for instance Lemma 1.2.5 for an example of this. 

In a similar spirit: 

• if one needs to show that a quantity X vanishes, try showing that $| X | \leq \varepsilon$ for every $\varepsilon > 0$ . (Exercise 1.2.19 is a simple application of this strategy.) 

• if one wishes to show that two functions $f , g$ agree almost everywhere, try showing first that $| f ( x ) - g ( x ) | \leq \varepsilon$ holds for almost every x, or even just outside of a set of measure at most $\varepsilon ,$ for any given $\varepsilon > 0$ . (See for instance the proof of Lemma 1.5.7 for an example of this.) 

• if one wants to show that a sequence $x _ { n }$ of real numbers converges to zero, try showing that lim $\quad \operatorname* { s u p } _ { n \to \infty } | x _ { n } | \leq \varepsilon$ for every $\varepsilon > 0$ . (The proof of the Lebesgue diferentiation theorem, Theorem 1.6.12, is in this spirit.) 

## 2.1. Problem solving strategies

Don’t be too focused on getting all your error terms adding up to exactly ε - usually, as long as the final error bound consists of terms that can all be made as small as one wishes by choosing parameters in a suitable way, that is enough. For instance, an error term such as 10ε is certainly OK, or even more complicated expressions such as $1 0 \varepsilon / \delta + 4 \delta$ if one has the ability to choose $\delta$ as small as one wishes, and then after $\delta$ is chosen, one can then also set $\varepsilon$ as small as one wishes (in a manner that can depend on $\delta )$ 

One caveat: for finite x, and any $\varepsilon > 0$ , it is true that $x + \varepsilon > x$ and $x - \varepsilon < x$ , but this statement is not true when x is equal to +∞ $\left( \mathrm { o r - } \infty \right)$ . So remember to exercise some care with the epsilon of room trick when some quantities are infinite. 

See also §2.7 of An epsilon of room, Vol. I. 

2.1.3. Decompose (or approximate) a rough or general object into (or by) a smoother or simpler one. If one has to prove something about an unbounded (or infinite measure) set, consider proving it for bounded (or finite measure) sets first if this looks easier. 

In a similar spirit: 

• If one has to prove something about a measurable set, try proving it for open, closed, compact, bounded, or elementary sets first. 

• If one has to prove something about a measurable function, try proving it for functions that are continuous, bounded, compactly supported, simple, absolutely integrable, etc.. 

• If one has to prove something about an infinite sum or sequence, try proving it first for finite truncations of that sum or sequence (but try to get all the bounds independent of the number of terms in that truncation, so that you can still pass to the limit!). 

• If one has to prove something about a complex-valued function, try it for real-valued functions first. 

• If one has to prove something about a real-valued function, try it for unsigned functions first. 

• If one has to prove something about a simple function, try it for indicator functions first. 

In order to pass back to the general case from these special cases, one will have to somehow decompose the general object into a combination of special ones, or approximate general objects by special ones (or as a limit of a sequence of special objects). In the latter case, one may need an epsilon of room (§2.1.2), and some sort of limiting analysis may be needed to deal with the errors in the approximation (it is not always enough to just “pass to the limit”, as one has to justify that the desirable properties of the approximating object are preserved in the limit). Littlewood’s principles (Section 1.3.5) and their variants are often useful for thus purpose. 

Note: one should not do this blindly, as one might then be loading on a bunch of distracting but ultimately useless hypotheses that end up being a lot less help than one might hope. But they should be kept in mind as something to try if one starts having thoughts such as “Gee, it would be nice at this point if I could assume that f is continuous / real-valued / simple / unsigned / etc.”. 

In the more quantitative areas of analysis and PDE, one sees a common variant of the above technique, namely the method of a priori estimates. Here, one needs to prove an estimate or inequality for all functions in a large, rough class (e.g. all rough solutions to a PDE). One can often then first prove this inequality in a much smaller (but still “dense”) class of “nice” functions, so that there is little dificulty justifying the various manipulations (e.g. exchanging integrals, sums, or limits, or integrating by parts) that one wishes to perform. Once one obtains these a priori estimates, one can then often take some sort of limiting argument to recover the general case. 

2.1.4. If one needs to flip an upper bound to a lower bound or vice versa, look for a way to take reflections or complements. Sometimes one needs a lower bound for some quantity, but only has techniques that give upper bounds. In some cases, though, one can “reflect” an upper bound into a lower bound (or vice versa) by replacing a set E contained in some space X with its complement X\E, or a function f with its negation −f (or perhaps subtracting f from some dominating function F to obtain $F - f )$ . This trick works best when the objects being reflected are contained in some sort of “bounded”, “finite measure”, or “absolutely integrable” container, so that one avoids having the dangerous situation of having to subtract infinite quantities from each other. 

A typical example of this is when one deduces downward monotone convergence for sets from upward monotone convergence for sets (Exercise 1.2.11). 

2.1.5. Uncountable unions can sometimes be replaced by countable or finite unions. Uncountable unions are not well-behaved in measure theory; for instance, an uncountable union of null sets need not be a null set (or even a measurable set). (On the other hand, the uncountable union of open sets remains open; this can often be important to know.) However, in many cases one can replace an uncountable union by a countable one. For instance, if one needs to prove a statement for all $\varepsilon > 0$ , then there are an uncountable number of $\varepsilon ^ { \prime }$ s one needs to check, which may threaten measurability; but in many cases it is enough to only work with a countable sequence of εs, such as the numbers $1 / m$ for m = 1, 2, 3, . . .. (Exercise 1.6.30 relies heavily on this trick.) 

In a similar spirit, given a real parameter λ, this parameter initially ranges over uncountably many values, but in some cases one can get away with only working with a countable set of such values, such as the rationals. In a similar spirit, rather than work with all boxes (of which there are uncountably many), one might work with the dyadic boxes (of which there are only countably many; also, they obey nicer nesting properties than general boxes and so are often desirable to work with in any event). 

If you are working on a compact set, then one can often replace even uncountable unions with finite ones, so long as one is working with open sets. (The proof of Theorem 1.6.20 is a good example of this strategy.) When this option is available, it is often worth spending an epsilon of measure (or whatever other resource is available to spend) to make one’s sets open, just so that one can take advantage of compactness. 

2.1.6. If it is dificult to work globally, work locally instead. A domain such as Euclidean space $\mathbf { R } ^ { d }$ has infinite measure, and this creates a number of technical dificulties when trying to do measure theory directly on such spaces. Sometimes it is best to work more locally, for instance working on a large ball $B ( 0 , R )$ or even a small ball such as $B ( x , \varepsilon )$ first, and then figuring out how to patch things together later. Compactness (or the closely related property of total boundedness) is often useful for patching together small balls to cover a large ball. Patching together large balls into the whole space tends to work well when the properties one are trying to establish are local in nature (such as continuity, or pointwise convergence) or behave well with respect to countable unions. For instance, to prove that a sequence of functions $f _ { n }$ converges pointwise almost everywhere to f on $\mathbf { R } ^ { d }$ , it sufices to verify this pointwise almost everywhere convergence on the ball $B ( 0 , R )$ for every $R > 0$ (which one can take to be an integer to get countability, see §2.1.5). The application of vertical truncation (as done, for instance, in the proof of Corollary 1.3.14) is an instance of this idea. 

2.1.7. Be willing to throw away an exceptional set. The “Lebesgue philosophy” to measure theory is that null sets are often “irrelevant”, and so one should be very willing to cut out a set of measure zero on which bad things are happening (e.g. a function is undefined or infinite, a sequence of functions is not converging, etc.). One should also be only slightly less willing to throw away sets of positive but small measure, e.g. sets of measure at most ε. If such sets can be made arbitrarily small in measure, this is often almost as good as just throwing away a null set. 

Many things in measure theory improve after throwing away a small set. The most notable examples of this are Egorov’s theorem (Theorem 1.3.26) and Lusin’s theorem (Theorem 1.3.28); see also Exercise 1.3.25 for some other examples of this idea. 

It is also common to see a similar trick<sup>1</sup> of throwing away most of a sequence and working with a subsequence instead. See §2.1.17 below. 

2.1.8. Draw pictures and try to build counterexamples. Measure theory, particularly on Euclidean spaces, has a significant geometric aspect to it, and you should be exploiting your geometric intuition. Drawing pictures and graphs of all the objects being studied is a good way to start. These pictures need not be completely realistic; they should be just complicated enough to hint at the complexities of the problem, but not more. For instance, usually one- or twodimensional pictures sufice for understanding problems in $\mathbf { R } ^ { d } \colon$ ; drawing intricate 3D (or 4D, etc.) pictures does not often make things simpler. To indicate that a function is not continuous, one or two discontinuities or oscillations might sufice; make it too ornate and it becomes less clear what to do about that function. One should view these pictures as providing a “cartoon sketch” of the situation, which exaggerates key features and downplays others, rather than a photorealistic image of the situation; too much detail or accuracy in a picture may be a waste of time, or otherwise counterproductive. 

A common mistake is to try to draw a picture in which both the hypotheses and conclusion of the problem hold. This is actually not all that useful, as it often does not reveal the causal relationship between the former and the latter. One should try instead to draw a picture in which the hypotheses hold but for which the conclusion does not - in other words, a counterexample to the problem. Of course, you should be expected to fail at this task, given that the statement of the problem is presumably true. However, the way in which your picture fails to accomplish this task is often very instructive, and can reveal vital clues as to how the solution to the problem is supposed to proceed. 

I have deliberately avoided drawing pictures in this book. This is not because I feel that pictures are not useful - far from it - but because I have found that it is far more informative for a reader to draw his or her own pictures of a given mathematical situation, rather than rely on the author’s images (except in situations where the geometric situation is particularly complicated or subtle), as such pictures will naturally be adapted to the reader’s mindset rather than the author’s. Besides, the process of actually drawing the picture is at least as instructive as the picture itself. 

2.1.9. Try simpler cases first. This advice of course extends well beyond measure theory, but if one is completely stuck on a problem, try making the problem simpler (while still capturing at least one of the dificulties of the problem that you cannot currently resolve). For instance, if faced with a problem in $\mathbf { R } ^ { d }$ , try the one-dimensional case $d = 1$ first. Faced with a problem about a general measurable function f, try a much simpler case first, such as an indicator function $f = 1 _ { E }$ . Faced with a problem about a general measurable set, try an elementary set first. Faced with a problem about a sequence of functions, try a monotone sequence of functions first. And so forth. (Note that this trick overlaps quite a bit with §2.1.3.) 

The problem should not be made so simple that it becomes trivial, as this doesn’t really gain you any new insight about the original problem; instead, one should try to keep the “essential” dificulties of the problem while throwing away those aspects that you think are less important (but are still serving to add to the overall dificulty level). 

On the other hand, if the simplified problem is unexpectedly easy, but one cannot extend the methods to the general case (or somehow leverage the simplified case to the general case, as in §2.1.3), this is an indication that the true dificulty lies elsewhere. For instance, if a problem involving general functions could be solved easily for monotone functions, but one cannot then extend that argument to the general case, this suggests that the true enemy is oscillation, and perhaps one should try another simple case in which the function is allowed to be highly oscillatory (but perhaps simple in other ways, e.g. bounded with compact support). 

2.1.10. Abstract away any information that you believe or suspect to be irrelevant. Sometimes one is faced with an embarrassment of riches when it comes to what choice of technique to use on a problem; there are so many diferent facts that one knows about the problem, and so many diferent pieces of theory that one could apply, that one doesn’t quite know where to begin. 

When this happens, abstraction can be a vital tool to clear away some of the conceptual clutter. Here, one wants to “forget” part of the setting that the problem is phrased in, and only keep the part that seems to be most relevant to the hypotheses and conclusions of the problem (and thus, presumably, to the solution as well). 

For instance, if one is working in a problem that is set in Euclidean space $\mathbf { R } ^ { d }$ , but the hypotheses and conclusions only involve measure-theoretic concepts (e.g. measurability, integrability, measure, etc.) rather than topological structure, metric structure, etc., then it may be worthwhile to try abstracting the problem to the more general setting of an abstract measure space, thus forgetting that one was initially working in $\mathbf { R } ^ { d }$ . The point of doing this is that it cuts down on the number of possible ways to start attacking the problem. For instance, facts such as outer regularity (every measurable set can be approximated from above by an open set) do not hold in abstract measure spaces (which do not even have a meaningful notion of an open set), and so presumably will not play a role in the solution; similarly for any facts involving boxes. Instead, one should be trying to use general facts about measure, such as countable additivity, which are not specific to $\mathbf { R } ^ { d }$ 

Remark 2.1.1. It is worth noting that sometimes this abstraction method does not always work; for instance, when viewed as a measure space, $\mathbf { R } ^ { d }$ is not completely arbitrary, but does have one or two features that distinguish it from a generic measure space, most notably the fact that it is σ-finite. So, even if the hypotheses and conclusion of a problem about $\mathbf { R } ^ { d }$ is purely measure-theoretic in nature, one may still need to use some measure-theoretic facts specific to $\mathbf { R } ^ { d }$ . Here, it becomes useful to know a little bit about the classification of measure spaces to have some intuition as to how “generic” a measure space such as $\mathbf { R } ^ { d }$ really is. This intuition is hard to convey at this level of the subject, but in general, measure spaces form a very “non-rigid” category, with very few invariants, and so it is largely true that one measure space usually behaves much the same as any other. 

Another example of abstraction: suppose that a problem involves a large number of sets $\textstyle ( \mathrm { e . g . } E _ { n }$ and $F _ { n } )$ and their measures, but that the conclusion of the problem only involves the measures $m ( E _ { n } ) , m ( F _ { n } )$ of the sets, rather than the sets themselves. Then one can try to abstract the sets out of the problem, by trying to write down every single relationship between the numerical quantities $m ( E _ { n } ) , m ( F _ { n } )$ that one can easily deduce from the given hypotheses (together with basic properties of measure, such as monotonicity or countable additivity). One can then rename these quantities (e.g. $a _ { n } : = m ( E _ { n } )$ and $b _ { n } : = m ( F _ { n } ) )$ ) to ”forget” that these quantities arose from a measure-theoretic context, and then work with a purely numerical problem, in which one is starting with hypotheses on some sequences $a _ { n } , b _ { n }$ of numbers and trying to deduce a conclusion about such sequences. Such a problem is often easier to solve than the original problem due to the simpler context. Sometimes, this simplified problem will end up being false, but the counterexample will often be instructive, either in indicating the need to add an additional hypothesis connecting the $a _ { n } , b _ { n }$ , or to indicate that one cannot work at this level of abstraction but must introduce some additional concrete ingredient. 

Note that this trick is in many ways the antithesis of §2.1.9, because by passing to a special case, one often makes the problem more concrete, with more things that one is now able to start trying. However, the two tricks can work together. One particularly useful “advanced move” in mathematical problem solving is to first abstract the problem to a more general one, and then consider a special case of that more abstract problem which is not directly related to the original one, but is somehow simpler than the original while still capturing some of the essence of the dificulty. Attacking this alternate problem can then lead to some indirect but important ways to make progress on the original problem. 

2.1.11. Exploit Zeno’s paradox: a single epsilon can be cut up into countably many sub-epsilons. A particularly useful fact in measure theory is that one can cut up a single epsilon into countably many pieces, for instance by using the geometric series identit 

$$
\varepsilon = \varepsilon / 2 + \varepsilon / 4 + \varepsilon / 8 + \ldots ;
$$

this observation arguably goes all the way back to Zeno. As such, even if one only has an epsilon of room budgeted for a problem, one can still use this budget to do a countably infinite number of things. This fact underlies many of the countable additivity and subadditivity properties in measure theory, and also makes the ability to approximate rough objects by smoother ones to be useful even when countably many rough objects need to be approximated. (Exercise 1.2.3 is a typical example in which this trick is used.) 

In general, one should be alert to this sort of trick when one has to spend an epsilon or so on an infinite number of objects. If one was forced to spend the same epsilon on each object, one would soon end up with an unacceptable loss; but if one can get away with using a diferent epsilon each time, then Zeno’s trick comes in very handy. 

2.1.12. If you expand your way to a double sum, a double integral, a sum of an integral, or an integral of a sum, try interchanging the two operations. Or, to put it another way: “The Fubini-Tonelli theorem (Corollary 1.7.23) is your friend”. Provided that one is either in the unsigned or absolutely convergent worlds, this theorem allows you to interchange sums and integrals with each other. In many cases, a double sum or integral that is dificult to sum in one direction can become easier to sum (or at least to upper bound, which is often all that one needs in analysis). In fact, if in the course of expanding an expression, you encounter such a double sum or integral, you should reflexively try interchanging the operations to see if the resulting expression looks any simpler. 

Note that in some cases the parameters in the summation may be constrained, and one may have to take a little care to sum it properly. 

For instance, 

$$
\sum_ {n = - \infty} ^ {\infty} \sum_ {m = n} ^ {\infty} a _ {m, n}\tag{2.1}
$$

interchanges (assuming that the $a _ { n , m }$ are either unsigned or absolutely convergent) to 

$$
\sum_ {m = - \infty} ^ {\infty} \sum_ {n = - \infty} ^ {m} a _ {m, n}
$$

(why? try plotting the set of pairs $( m , n )$ that appear in both). If one is having trouble interchanging constrained sums or integrals, one solution is to re-express the constraint using indicator functions. For instance, one can rewrite the constrained sum (2.1) as the unconstrained sum 

$$
\sum_ {n = - \infty} ^ {\infty} \sum_ {m = - \infty} ^ {\infty} 1 _ {m \geq n} a _ {m, n}
$$

(extending the domain of $a _ { m , n }$ if necessary), at which point interchanging the summations is easily accomplished. 

The following point is obvious, but bears mentioning explicitly: while the interchanging sums/integrals trick can be very powerful, one should not apply it twice in a row to the same double sum or double operation, unless one is doing something genuinely non-trivial in between those two applications. So, after one exchanges a sum or integral, the next move should be something other than another exchange (unless one is dealing with a triple or higher sum or integral). 

A related move (not so commonly used in measure theory, but occurring in other areas of analysis, particularly those involving the geometry of Euclidean spaces) is to merge two sums or integrals into a single sum or integral over the product space, in order to use some additional feature of the product space (e.g. rotation symmetry) that is not readily visible in the factor spaces. The classic example of this trick is the evaluation of the gaussian integral $\int _ { - \infty } ^ { \infty } e ^ { - x ^ { 2 } }$ dx by squaring it, rewriting that square as the two-dimensional gaussian integral $\int _ { \mathbf { R } ^ { 2 } } e ^ { - x ^ { 2 } - y ^ { 2 } }$ dxdy, and then switching to polar coordinates. 

2.1.13. Pointwise control, uniform control, and integrated (average) control are all partially convertible to each other. 

There are three main ways to control functions (or sequences of functions, etc.) in analysis. Firstly, there is pointwise control, in which one can control the function at every point (or almost every point), but in a non-uniform way. Then there is uniform control, where one can control the function in the same way at most points (possibly throwing out a set of zero measure, or small measure). Finally, there is integrated control (or control “on the average”), in which one controls the integral of a function, rather than the pointwise values of that function. 

It is important to realise that control of one type can often be partially converted to another type. Simple examples include the deduction of pointwise convergence from uniform convergence, or integrating a pointwise bound $f ( x ) ~ \leq ~ g ( x )$ to obtain an integrated bound $\begin{array} { r } { \int f \ \le \ \int g . } \end{array}$ Of course, these conversions are not reversible and thus lose some information; not every pointwise convergent sequence is uniformly convergent, and an integral bound does not imply a pointwise bound. However, one can partially reverse such implications if one is willing to throw away an exceptional set (§2.1.7). For instance, Egorov’s theorem (Theorem 1.3.26) lets one convert pointwise convergence to (local) uniform convergence after throwing away an exceptional set, and Markov’s inequality (Exercise 1.4.36(vi)) lets one convert integral bounds to pointwise bounds, again after throwing away an exceptional set. 

2.1.14. If the conclusion and hypotheses look particularly close to each other, just expand out all the definitions and follow your nose. This trick is particularly useful when building the most basic foundations of a theory. Here, one may not need to experiment too much with generalisations, abstractions, or special cases, or try to marshall a lot of possibly relevant facts about the objects being studied: sometimes, all one has to do is go back to first principles, write out all the definitions with their epsilons and deltas, and start plugging away at the problem. 

Knowing when to just follow one’s nose, and when to instead look for a more high-level approach to a problem, can require some judgement or experience. A direct approach tends to work best when the conclusion and hypothesis already look quite similar to each other (e.g. they both state that a certain set or family of sets is measurable, or they both state that a certain function or family of functions is continuous, etc.). But when the conclusion looks quite diferent from the hypotheses (e.g. the conclusion is some sort of integral identity, and the hypotheses involve measurability or convergence properties), then one may need to use more sophisticated tools than what one can easily get from using first principles. 

2.1.15. Don’t worry too much about exactly what $\varepsilon$ (or δ, or N, etc.) needs to be. It can usually be chosen or tweaked later if necessary. Often in the middle of an argument, you will want to use some fact that involves a parameter, such as ε, that you are completely free to choose (subject of course to reasonable constraints, such as requiring $\varepsilon$ to be positive). For instance, you may have a measurable set and decide to approximate it from above by an open set of at most ε more measure. But it may not be obvious exactly what value to give this parameter ε; you have so many choices available that you don’t know which one to pick! 

In many cases, one can postpone thinking about this problem by leaving $\varepsilon$ undetermined for now, and continuing on with one’s argument, which will gradually start being decorated with ε’s all over the place. At some point, one will need $\varepsilon$ to do something (and, in the particular case of $\varepsilon ,$ “doing something” almost always means “being small enough”), e.g. one may need $3 n \varepsilon$ to be less than $\delta ,$ , where $n , \delta$ are some other positive quantities in one’s problem that do not depend on $\varepsilon .$ . At this point, one could now set $\varepsilon$ to be whatever is needed to get past this step in the argument, e.g. one could set $\varepsilon$ to equal $\delta / 4 n$ . But perhaps one still wishes to retain the freedom to set $\varepsilon$ because it might come in handy later. In that case, one sets aside the requirement $^ { \mathrm { \scriptsize ~ 4 6 } } 3 n \varepsilon < \delta ^ { \mathrm { \scriptsize ~ 5 } }$ and keeps going. Perhaps a bit later on, one might need $\varepsilon$ to do something else; for instance, one might also need $5 \varepsilon \le 2 ^ { - n }$ . Once one has compiled the complete “wish list” of everything one wishes one’s parameters to do, then one can finally make the decision of what value to set those parameters equal to. For instance, if the above two inequalities are the only inequalities required of $\varepsilon ,$ one can choose ε equal to min $( \delta / 4 n , 2 ^ { - n } / 5 )$ . This may be a choice of $\varepsilon$ which was not obvious at the start of the argument, but becomes so as the argument progresses. 

There is however one big caveat when adopting this “choose parameters later” approach, which is that one needs to avoid a circular dependence of constants. For instance, it is perfectly fine to have two arbitrary parameters $\varepsilon$ and $\delta$ floating around unspecified for most of the argument, until at some point you realise that you need $\varepsilon$ to be smaller than $\delta ,$ , and so one chooses $\varepsilon$ accordingly (e.g. one sets it to equal $\delta / 2 )$ . Or, perhaps instead one needs $\delta$ to be smaller than $\varepsilon ,$ , and so sets $\delta$ equal to $\varepsilon / 2$ . One can execute either of these two choices separately, but of course one cannot perform them simultaneously; this sets up an inconsistent circular dependency in which $\varepsilon$ needs to be defined after $\delta$ is chosen, and $\delta$ can only be chosen after $\varepsilon$ is fixed. ${ \mathrm { S o } } ,$ if one is going to delay choosing a parameter such as $\varepsilon$ until later, it becomes important to mentally keep track of what objects in one’s argument depend on $\varepsilon ,$ and which ones are independent of $\varepsilon .$ . One can choose $\varepsilon$ in terms of the latter quantities, but one usually cannot do so in terms of the former quantities (unless one takes the care to show that the interlinked constraints between the quantities are still consistent, and thus simultaneously satisfiable). 

2.1.16. Once one has started to lose some constants, don’t be hesitant to lose some more. Many techniques in analysis end up giving inequalities that are ineficient by a constant factor. For instance, any argument involving dyadic decomposition and powers of two tends to involve losses of factors of 2. When arguing using balls in Euclidean space, one sometimes loses factors involving the volume of the unit ball (although this factor often cancels itself out if one tracks it more carefully). And so forth. However, in many cases these constant factors end up being of little importance: an upper bound of $2 \varepsilon$ or 100ε is often just as good as an upper bound of $\varepsilon$ for the purposes of analysis (cf. §2.1.15). So it is often best not to invest too much energy in carefully computing and optimising these constants; giving these constants a symbol such as $C ,$ , and not worrying about their exact value, is often the simplest approach. (One can also use asymptotic notation, such as $O ( )$ , which is very convenient to use once you know how it works.) 

Now there are some cases in which one really does not want to lose any constants at all. For instance, if one is using §2.1.1 to prove that $X = Y$ , it is not enough to show that $X \le 2 Y$ and $Y \le 2 X$ ; one really needs to show $X \ \leq \ Y$ and $Y \ \leq \ X$ without losing any constants. (But proving $X \le ( 1 + \varepsilon ) Y$ and $Y \le ( 1 + \varepsilon ) X$ is OK, by §2.1.2.) But once one has already performed one step that loses a constant, there is little further to be lost by losing more; there can be a big diference between $X \leq Y$ and $X \le 2 Y$ , but there is little diference in practice between $X \le 2 Y$ and $X \le 1 0 0 Y$ , at least for the purposes of mathematical analysis. At that stage, one should put oneself in the mental mode of thought where “constants don’t matter”, which can lead to some simplifications. For instance, if one has to estimate a sum $X + Y$ of two positive quantities, one can start using such estimates as 

$$
\max (X, Y) \leq X + Y \leq 2 \max (X, Y),
$$

which says that, up to a factor of 2, $X + Y$ is the same thing as max $( X , Y )$ . In some cases the latter is easier to work with (e.g. max $( X , Y ) ^ { n }$ is equal to max $( X ^ { n } , Y ^ { n } )$ , whereas the formula for $( X +$ $Y ) ^ { n }$ is messier). 

2.1.17. One can often pass to a subsequence to improve the convergence properties. In real analysis, one often ends up possessing a sequence of objects, such as a sequence of functions $f _ { n }$ which may converge in some rather slow or weak fashion to a limit $f .$ Often, one can improve the convergence of this sequence by passing to a subsequence. For instance: 

• In a metric space, if a sequence $x _ { n }$ converges to a limit $x ,$ then one can find a subsequence $x _ { n _ { j } }$ which converges quickly to the same limit $x ,$ , for instance one can ensure that $d ( x _ { n _ { j } } , x ) \leq 2 ^ { - j }$ (or one can replace $2 ^ { - j }$ with any other positive expression depending on $j )$ . In particular, one can make $\textstyle \sum _ { j = 1 } ^ { \infty } d ( x _ { n _ { j } } , x )$ and $\textstyle \sum _ { j = 1 } ^ { \infty } d ( x _ { n _ { j } } , x _ { n _ { j + 1 } } )$ absolutely convergent, which is sometimes useful. 

• A sequence of functions that converges in $L ^ { 1 }$ norm or in measure can be refined to a subsequence that converges pointwise almost everywhere as well. 

• A sequence in a (sequentially) compact space may not converge at all, but some subsequence of it will always converge. 

• The pigeonhole principle: A sequence which takes only finitely many values has a subsequence that is constant. More generally, a sequence which lives in the union of finitely many sets has a subsequence that lives in just one of these sets. 

Often, the subsequence is good enough for one’s applications, and there are also a number of ways to get back from a subsequence to the original sequence, such as: 

• In a metric space, if you know that $x _ { n }$ is a Cauchy sequence, and some subsequence of $x _ { n }$ already converges to x, then this drags the entire sequence with it, i.e. $x _ { n }$ converges to x also. 

• The Urysohn subsequence principle: in a topological space, if every subsequence of a sequence $x _ { n }$ itself has a subsequence that converges to a limit $x ,$ , then the entire sequence converges to x. 

2.1.18. A real limit can be viewed as a meeting of the limit superior and limit inferior. A sequence $x _ { n }$ of real numbers does not necessarily have a limit $\scriptstyle \operatorname* { l i m } _ { n \to \infty } x _ { n }$ , but the limit superior lim $\scriptstyle \operatorname* { s u p } _ { n \to \infty } x _ { n } : =$ inf $N { \mathrm { ~ S u p } } _ { n > N } x _ { n }$ and the limit inferior lim in $\begin{array} { r } { \mathrm { f } _ { n \to \infty } x _ { n } = \operatorname* { s u p } _ { N } \operatorname* { i n f } _ { n > N } x _ { n } } \end{array}$ always exist (though they may be infinite), and can be easily defined in terms of infima and suprema. Because of this, it is often convenient to work with the lim sup and lim inf instead of a limit. For instance, to show that a limit $\scriptstyle \operatorname* { l i m } _ { n \to \infty } x _ { n }$ exists, it sufices to show that 

$$
\limsup _ {n \to \infty} x _ {n} \leq \operatorname * {l i m i n f} _ {n \to \infty} x _ {n} + \varepsilon
$$

for all $\varepsilon > 0$ . In a similar spirit, to show that a sequence $x _ { n }$ of real numbers converges to zero, it sufices to show that 

$$
\limsup _ {n \to \infty} \left| x _ {n} \right| \leq \varepsilon
$$

for all $\varepsilon > 0$ . It can be more convenient to work with lim sups and lim infs instead of limits because one does not need to worry about the issue of whether the limit exists or not, and many tools (notably Fatou’s lemma and its relatives) still work in this setting. One should however be cautious that lim sups and lim infs tend to have only one half of the linearity properties that limits do; for instance, lim sups are subadditive but not necessarily additive, while lim infs are superadditive but not necessarily additive. 

The proof of the monotone diferentiation theorem (Theorem 1.6.25) given in the text relies quite heavily on this strategy. 

## 2.2. The Radamacher diferentiation theorem

The Fubini-Tonelli theorem (Corollary 1.7.23) is often used in extending lower-dimensional results to higher-dimensional ones. We illustrate this by extending the one-dimensional Lipschitz diferentiation theorem (Exercise 1.6.41) to higher dimensions, obtaining the Radamacher diferentiation theorem. 

We first recall some higher-dimensional definitions: 

Definition 2.2.1 (Lipschitz continuity). A function $f : X \to Y$ from one metric space $( X , d _ { X } )$ to another $( Y , d _ { Y } )$ is said to be Lipschitz continuous if there exists a constant $C > 0$ such that $d _ { Y } ( f ( x ) , f ( x ^ { \prime } ) ) \leq$ $C d _ { X } ( x , x ^ { \prime } )$ for all $x , x ^ { \prime } \in X$ . (In the applications of this section, X will be $\mathbf { R } ^ { d }$ and $Y$ will be R, with the usual metrics.) 

Exercise 2.2.1. Show that Lipschitz continuous functions are uniformly continuous, and hence continuous. Then give an example of a uniformly continuous function $f : [ 0 , 1 ]  [ 0 , 1 ]$ that is not Lipschitz continuous. 

Definition 2.2.2 (Diferentiability). Let $f : \mathbf { R } ^ { d }  \mathbf { R }$ be a function, and let $x _ { 0 } \in \mathbf { R } ^ { d }$ . For any $v \in \mathbf { R } ^ { d }$ , we say that $f$ is directionally diferentiable at $x _ { 0 }$ in the direction v if the limit 

$$
D _ {v} f (x _ {0}) := \lim _ {h \to 0; h \in \mathbf {R} \setminus \{0 \}} \frac {f (x _ {0} + h v) - f (x _ {0})}{h}
$$

exists, in which case we call $D _ { v } f ( x _ { 0 } )$ the directional derivative of $f$ at $x _ { 0 }$ in this direction. If $v = e _ { i }$ is one of the standard basis vectors $e _ { 1 } , \ldots , e _ { d }$ of $\mathbf { R } ^ { d }$ , we write $D _ { v } f ( x _ { 0 } )$ as $\textstyle { \frac { \partial f } { \partial x _ { i } } } ( x _ { 0 } )$ , and refer to this as the partial derivative of $f$ at $x _ { 0 }$ in the $e _ { i }$ direction. 

We say that f is totally diferentiable at $x _ { 0 }$ if there exists a vector $\nabla f ( x _ { 0 } ) \in \mathbf { R } ^ { d }$ with the property that 

$$
\lim _ {h \to 0; h \to \mathbf {R} ^ {d} \setminus \{0 \}} \frac {f (x _ {0} + h) - f (x _ {0}) - h \cdot \nabla f (x _ {0})}{| h |} = 0,
$$

where $v \cdot w$ is the usual dot product on $\mathbf { R } ^ { d }$ . We refer to $\nabla f ( x _ { 0 } )$ (if it exists) as the gradient of $f$ at $x _ { 0 }$ 

Remark 2.2.3. From the viewpoint of diferential geometry, it is better to work not with the gradient vector $\nabla f ( x _ { 0 } ) \in \mathbf { R } ^ { d }$ , but rather with the derivative covector $d f ( x _ { 0 } ) : \mathbf { R } ^ { d }  \mathbf { R }$ given by $d f ( x _ { 0 } )$ $v \mapsto \nabla f ( x _ { 0 } ) \cdot v .$ . This is because one can then define the notion of total diferentiability without any mention of the Euclidean dot product, which allows one to extend this notion to other manifolds in which there is no Euclidean (or more generally, Riemannian) structure. However, as we are working exclusively in Euclidean space for this application, this distinction will not be important for us. 

Total diferentiability implies directional and partial diferentiability, but not conversely, as the following three exercises demonstrate. 

Exercise 2.2.2 (Total diferentiability implies directional and partial diferentiability). Show that if $f : \mathbf { R } ^ { d }  \mathbf { R }$ is totally diferentiable at $x _ { 0 }$ , then it is directionally diferentiable at $x _ { 0 }$ in each direction $v \in \mathbf { R } ^ { d }$ , and one has the formula 

$$
D _ {v} f (x _ {0}) = v \cdot \nabla f (x _ {0}).\tag{2.2}
$$

In particular, the partial derivatives $\textstyle { \frac { \partial f } { \partial x _ { i } } } f ( x _ { 0 } )$ exist for $i = 1 , \ldots , d$ and 

$$
\nabla f (x _ {0}) = \left(\frac {\partial f}{\partial x _ {1}} (x _ {0}), \dots , \frac {\partial f}{\partial x _ {d}} (x _ {0})\right).\tag{2.3}
$$

Exercise 2.2.3 (Continuous partial diferentiability implies total differentiability). Let $f : \mathbf { R } ^ { d }  \mathbf { R }$ be such that the partial derivatives $\begin{array} { r } { \frac { \partial f } { \partial x _ { i } } : { \bf R } ^ { d }  } \end{array}$ R exist everywhere and are continuous. Then show that $f$ is totally diferentiable everywhere, which in particular implies that the gradient is given by the formula (2.3) and the directional derivatives are given by (2.2). 

Exercise 2.2.4 (Directional diferentiability does not imply total differentiability). Let $f : { \mathbf { R } } ^ { 2 }  { \mathbf { R } }$ be defined by setting $f ( 0 , 0 ) : = 0$ and $\begin{array} { r } { f ( x _ { 1 } , x _ { 2 } ) : = \frac { x _ { 1 } x _ { 2 } ^ { 2 } } { x _ { 1 } ^ { 2 } + x _ { 2 } ^ { 2 } } } \end{array}$ for $( x _ { 1 } , x _ { 2 } ) \in { \bf R } ^ { 2 } \backslash \{ ( 0 , 0 ) \}$ . Show that the directional derivatives $D _ { v } f ( x )$ exist for all $x , v \in \mathbf { R } ^ { 2 }$ (so in particular, the partial derivatives exist), but that f is not totally diferentiable at the origin (0, 0). 

Now we can state the Rademacher diferentiation theorem. 

Theorem 2.2.4 (Rademacher diferentiation theorem). Let $f : \mathbf { R } ^ { d } $ R be Lipschitz continuous. Then f is totally diferentiable at $x _ { 0 }$ for almost every $\boldsymbol { x } _ { 0 } \in \mathbf { R } ^ { d }$ 

Note that the $d = 1$ case of this theorem is Exercise 1.6.41, and indeed we will use the one-dimensional theorem to imply the higherdimensional one, though there will be some technical issues due to the gap between directional and total diferentiability. 

Proof. The strategy here is to first aim for the more modest goal of directional diferentiability, and then find a way to link the directional derivatives together to get total diferentiability. 

Let $v , x _ { 0 } \in \mathbf { R } ^ { d }$ . As f is continuous, we see that in order for the directional derivative 

$$
D _ {v} f (x _ {0}) := \lim _ {h \to 0; h \in \mathbf {R} \setminus \{0 \}} \frac {f (x _ {0} + h v) - f (x _ {0})}{h}
$$

to exist, it sufices to let h range in the dense subset $\mathbf { Q } \backslash \{ 0 \}$ of $\mathbf { R } \backslash \{ 0 \}$ for the purposes of determing whether the limit exists. In particular, $D _ { v } f ( x _ { 0 } )$ exists if and only if 

$$
\operatorname * {l i m s u p} _ {h \to 0; h \in \mathbf {Q} \setminus \{0 \}} \frac {f (x _ {0} + h v) - f (x _ {0})}{h} = \operatorname * {l i m i n f} _ {h \to 0; h \in \mathbf {Q} \setminus \{0 \}} \frac {f (x _ {0} + h v) - f (x _ {0})}{h}.
$$

From this we easily conclude that for each direction $v \in \mathbf { R } ^ { d }$ , the set 

$$
E _ {v} := \{x _ {0} \in \mathbf {R} ^ {d}: D _ {v} f (x _ {0}) \text {   does   not   exist } \}
$$

is Lebesgue measurable in $\mathbf { R } ^ { d }$ (indeed, it is even Borel measurable). A similar argument reveals that $D _ { v } f$ is a measurable function outside of $E _ { v }$ . From the Lipschitz nature of $f ,$ , we see that $D _ { v } f$ is also a bounded function. 

Now we claim that $E _ { v }$ is a null set for each $v .$ . For $v = 0 ~ E _ { v }$ is clearly empty, so we may assume $v \neq 0$ . Applying an invertible linear transformation to map $v$ to $e _ { 1 }$ (noting that such transformations will map Lipschitz functions to Lispchitz functions, and null sets to null sets) we may assume without loss of generality that $v$ is the basis vector $e _ { 1 }$ . Thus our task is now to show that $\begin{array} { r } { \frac { \partial f } { \partial x _ { 1 } } ( x ) } \end{array}$ exists for almost every $\boldsymbol { x } \in \mathbf { R } ^ { d }$ 

We now split $\mathbf { R } ^ { d }$ as $\mathbf { R } \times \mathbf { R } ^ { d - 1 }$ . For each $x _ { 0 } \in \mathbf { R }$ and $y _ { 0 } \in \mathbf { R } ^ { d - 1 }$ we see from the definitions that $\frac { \partial f } { \partial x _ { 1 } } ( x _ { 0 } , y _ { 0 } )$ exists if and only if the one-dimensional function $x \mapsto f ( x , y _ { 0 } )$ is diferentiable at $x _ { 0 }$ . But this function is Lipschitz continuous (this is inherited from the Lipschitz continuity of $f )$ , and so we see that for each fixed $y _ { 0 } \in \mathbf { R } ^ { d - 1 }$ , the set $E ^ { y _ { 0 } } : = \{ x _ { 0 } \in \mathbf { R } : ( x _ { 0 } , y _ { 0 } ) \in E \}$ is a null set in R. Applying Tonelli’s theorem for sets (Corollary 1.7.19), we conclude that $E$ is a null set as required. 

We would like to now conclude that $\textstyle \bigcup _ { v \in \mathbf { R } ^ { d } } E _ { v }$ is a null set, but there are uncountably many $v { \mathrm { { s } } } .$ , so this is not directly possible. However, as $\mathbf { Q } ^ { d }$ is rational, we can at least assert that $\begin{array} { r } { E : = \bigcup _ { v \in \mathbf { Q } ^ { d } } E _ { v } } \end{array}$ is a null set. In particular, for almost every $\boldsymbol { x } _ { 0 } \in \mathbf { R } ^ { d }$ , f is directionally diferentiable in every rational direction $v \in \mathbf { Q } ^ { d }$ 

Now we perform an important trick, in which we interpret the directional derivative $D _ { v } f$ as a weak derivative. We already know that $D _ { v } f$ is almost everywhere defined, bounded and measurable. Now let $g : \mathbf { R } ^ { d }  \mathbf { R }$ be any function that is compactly supported and Lipschitz continuous. We investigate the integral 

$$
\int_ {\mathbf {R} ^ {d}} D _ {v} f (x) g (x) d x.
$$

This integral is absolutely convergent since $D _ { v } f ( x )$ is bounded and measurable, and $g ( x )$ is continuous and compactly supported, hence bounded. We expand this out as 

$$
\int_ {\mathbf {R} ^ {d}} \lim _ {h \to 0; h \in \mathbf {R} \setminus \{0 \}} \frac {f (x + h v) - f (x)}{h} g (x) d x.
$$

Note (from the Lipschitz nature of $f )$ that the expression ${ \frac { f ( x + h v ) - f ( x ) } { h } } g ( x )$ is bounded uniformly in h and $x ,$ , and is also uniformly compactly 

supported in x for h in a bounded set. We may thus apply the dominated convergence theorem (Theorem 1.4.49) to pull the limit out of the integral to obtain 

$$
\lim _ {h \to 0; h \in \mathbf {R} \setminus \{0 \}} \int_ {\mathbf {R} ^ {d}} \frac {f (x + h v) - f (x)}{h} g (x) d x.
$$

Now, from translation invariance of the Lebesgue integral (Exercise 1.3.15) we have 

$$
\int_ {\mathbf {R} ^ {d}} f (x + h v) g (x) d x = \int_ {\mathbf {R} ^ {d}} f (x) g (x - h v) d x
$$

and so (by the lienarity of the Lebesgue integral) we may rearrange the previous expression as 

$$
\lim _ {h \to 0; h \in \mathbf {R} \backslash \{0 \}} \int_ {\mathbf {R} ^ {d}} f (x) \frac {g (x - h v) - g (x)}{h} d x.
$$

Now, as $g$ is Lipschitz, we know that $\frac { g ( x - h v ) - g ( x ) } { h }$ is uniformly bounded and converges pointwise almost everywhere to $D _ { - v } g ( x )$ as $h  0$ . We may thus apply the dominated convergence theorem again and end up with the integration by parts formula 

$$
\int_ {\mathbf {R} ^ {d}} D _ {v} f (x) g (x) d x = \int_ {\mathbf {R} ^ {d}} f (x) D _ {- v} g (x) d x.\tag{2.4}
$$

This formula moves the directional derivative operator $D _ { v }$ from $f$ over to $g .$ At present, this does not look like much of an advantage, because $g$ is the same sort of function that f is. However, the key point is that we can choose $g$ to be whatever we please, whereas f is fixed. In particular, we can choose $g$ to be a compactly supported, continuously diferentiable function (such functions are Lipschitz from the fundamental theorem of calculus, as their derivatives are bounded). By Exercise 2.2.3, one has $D _ { - v } g = - v \cdot \nabla g$ for such functions, and so 

$$
\int_ {\mathbf {R} ^ {d}} D _ {v} f (x) g (x) d x = - \int_ {\mathbf {R} ^ {d}} f (x) (v \cdot \nabla g) (x) d x.
$$

The right-hand side is linear in $v ,$ and so the left-hand side must be linear in v also. In particular, if $v = ( v _ { 1 } , \ldots , v _ { d } )$ , then we have 

$$
\int_ {\mathbf {R} ^ {d}} D _ {v} f (x) g (x) d x = \sum_ {j = 1} ^ {d} v _ {j} \int_ {\mathbf {R} ^ {d}} D _ {e _ {j}} f (x) g (x) d x.
$$

If we define the gradient candidate function 

$$
\nabla f (x) := (D _ {e _ {1}} f (x), \ldots , D _ {e _ {d}} f (x)) = (\frac {\partial f}{\partial x _ {1}} (x), \ldots , \frac {\partial f}{\partial x _ {d}} (x))
$$

(note that this function is well-defined almost everywhere, even though we don’t know yet whether f is totally diferentiable almost everywhere), we thus have 

$$
\int_ {\mathbf {R} ^ {d}} (D _ {v} f - v \cdot \nabla f) (x) g (x) d x = 0
$$

for all compactly supported, continuously diferentiable $g .$ . This implies (see Exercise 2.2.5 below) that $F _ { v } : = D _ { v } f - v \cdot \nabla f$ vanishes almost everywhere, thus (by countable subadditivity) we have 

$$
D _ {v} f (x _ {0}) = v \cdot \nabla f (x _ {0})\tag{2.5}
$$

for almost every $\boldsymbol { x } _ { 0 } \in \mathbf { R } ^ { d }$ and every $v \in \mathbf { Q } ^ { d }$ 

Let $x _ { 0 }$ be such that (2.5) holds for all $v \in \mathbf { Q } ^ { d }$ . We claim that this forces f to be totally diferentiable at $x _ { 0 }$ , which would give the claim. Let $F : \mathbf { R } ^ { d }  \mathbf { R } ^ { d }$ be the modified function 

$$
F (h) := f \left(x _ {0} + h\right) - f \left(x _ {0}\right) - h \cdot \nabla f \left(x _ {0}\right).
$$

Our objective is to show that 

$$
\lim _ {h \to 0; h \in \mathbf {R} ^ {d} \setminus \{0 \}} | F (h) | / | h | = 0.
$$

On the other hand, we have $F ( 0 ) = 0 , F$ is Lipschitz, and from (2.5) we see that $D _ { v } F ( 0 ) = 0$ for every $v \in \mathbf { Q } ^ { d }$ 

Let $\varepsilon > 0$ , and suppose that $h \in \mathbf { R } ^ { d } \backslash \{ 0 \}$ . Then we can write $h = r u$ where $r : = | h |$ and $u : = h / | h |$ lies on the unit sphere. This u need not lie in $\mathbf { Q } ^ { d }$ , but we can approximate it by some vector $v \in \mathbf { Q } ^ { d }$ with $| u - v | \leq \varepsilon$ . Furthermore, by the total boundedness of the unit sphere, we can make v lie in a finite subset $V _ { \varepsilon }$ of $\mathbf { Q } ^ { d }$ that only depends $\mathrm { o n } \ \varepsilon \ ( \mathrm { a n d \ o n \ } d )$ 

Since $D _ { v } F ( 0 ) = 0$ for all $v \in V _ { \varepsilon }$ , we see (by making $| h |$ small enough depending on $V _ { \varepsilon } )$ that we have 

$$
| \frac {F (r v) - F (0)}{r} | \leq \varepsilon
$$

for all $v \in V _ { \varepsilon }$ , and thus 

$$
| F (r v) | \leq \varepsilon r.
$$

On the other hand, from the Lipschitz nature of $F _ { ; }$ , we have 

$$
| F (r u) - F (r v) | \leq C r | u - v | \leq C r \varepsilon
$$

where C is the Lipschitz constant of F. As $h = r u$ , we conclude that 

$$
| F (h) | \leq (C + 1) r \varepsilon .
$$

In other words, we have shown that 

$$
| F (h) | / | h | \leq (C + 1) \varepsilon
$$

whenever $| h |$ is suficiently small depending on $\varepsilon .$ . Letting $\varepsilon \to 0$ , we obtain the claim.  

Exercise 2.2.5. Let $F : \mathbf { R } ^ { d }  \mathbf { R }$ be a locally integrable function with the property that $\begin{array} { r } { \int _ { \mathbf { R } ^ { d } } F ( x ) g ( x ) } \end{array}$ dx $= 0$ whenever $g$ is a compactly supported, continuously diferentiable function. Show that $F$ is zero almost everywhere. (Hint: if not, use the Lebesgue diferentiation theorem to find a Lebesgue point $x _ { 0 }$ of $F$ for which $F ( x _ { 0 } ) \neq 0$ , then pick a $g$ which is supported in a suficiently small neighbourhood of $x _ { 0 } . )$ 

## 2.3. Probability spaces

In this section we isolate an important special type of measure space, namely a probability space. As the name suggests, these spaces are of fundamental importance in the foundations of probability, although it should be emphasised that probability theory should not be viewed as the study of probability spaces, as these are merely models for the true objects of study of that theory, namely the behaviour of random events and random variables. (See §??? of ??? for further discussion of this point. Crossreference will be added once the remaining sections of the blog are converted to book form - T.) This text will however not be focused on applications to probability theory 

Definition 2.3.1 (Probability space). A probability space is a measure space $( \Omega , { \mathcal { F } } , { \mathbf { P } } )$ of total measure 1: $\mathbf { P } ( \Omega ) = 1$ . The measure P is known as a probability measure. 

Note the change of notation: whereas measure spaces are traditionally denoted by symbols such as $( X , B , \mu )$ , probability spaces are traditionally denoted by symbols such as $( \Omega , { \mathcal { F } } , { \mathbf { P } } )$ ). Of course, such notational changes have no impact on the underlying mathematical formalism, but they reflect the diferent cultures of measure theory and probability theory. In particular, the various components $\Omega , { \mathcal { F } }$ P carry the following interpretations in probability theory, that are absent in other applications of measure theory: 

(i) The space $\Omega$ is known as the sample space, and is interpreted as the set of all possible states $\omega \in \Omega$ that a random system could be in. 

(ii) The σ-algebra $\mathcal { F }$ is known as the event space, and is interpreted as the set of all possible events $E \in { \mathcal { F } }$ that one can measure. 

(iii) The measure $\mathbf { P } ( E )$ of an event is known as the probability of that event. 

The various axioms of a probability space then formalise the foundational axioms of probability, as set out by Kolmogorov. 

Example 2.3.2 (Normalised measure). Given any measure space $( X , B , \mu )$ with $0 < \mu ( X ) < + \infty$ , the space $\begin{array} { r } { ( X , B , \frac { 1 } { \mu ( X ) } \mu ) } \end{array}$ is a probability space. For instance, if Ω is a non-empty finite set with the discrete σ-algebra $2 ^ { \Omega }$ and the counting measure $\#$ , then the normalised counting measure $\frac { 1 } { \# \Omega } \#$ is a probability measure (known as the (discrete) uniform probability measure on Ω), and $( \Omega , 2 ^ { \Omega } , \frac { 1 } { \# \Omega } \# )$ is a probability space. In probability theory, this probability spaces models the act of drawing an element of the discrete set Ω uniformly at random. 

Similarly, if $\Omega \subset \mathbf { R } ^ { d }$ is a Lebesgue measurable set of positive finite Lebesgue measure, $0 < m ( \Omega ) < \infty$ , then $\begin{array} { r } { ( \Omega , { \mathcal { L } } [ { \bf R } ^ { d } ] \ \vert _ { \Omega } , \frac { 1 } { m ( \Omega ) } m \ \vert _ { \Omega } ) } \end{array}$ is a probability space. The probability measure $\begin{array} { r } { \frac { 1 } { m ( \Omega ) } m } \end{array}$  is known as the (continuous) uniform probability measure on Ω. In probability theory, this probability spaces models the act of drawing an element of the continuous set Ω uniformly at random. 

Example 2.3.3 (Discrete and continuous probability measures). If Ω is a (possibly infinite) non-empty set with the discrete σ-algebra $2 ^ { \Omega }$ , and if $( p _ { \omega } ) _ { \omega \in \Omega }$ are a collection of real numbers in [0, 1] with $\begin{array} { r } { \sum _ { \omega \in \Omega } p _ { \omega } \ = \ 1 } \end{array}$ , then the probability measure P defined by $\mathrm { ~ \bf ~ P ~ } : =$ 

$\textstyle \sum _ { \omega \in \Omega } p _ { \omega } \delta _ { \omega }$ , or in other words 

$$
\mathbf {P} (E) := \sum_ {\omega \in E} p _ {\omega},
$$

is indeed a probability measure, and $( \Omega , 2 ^ { \Omega } , { \bf P } )$ is a probability space. The function $\omega \mapsto p _ { \omega }$ is known as the (discrete) probability distribution of the state variable $\omega .$ 

Similarly, if Ω is a Lebesgue measurable subset of $\mathbf { R } ^ { d }$ of positive (and possibly infinite) measure, and $f : \Omega  [ 0 , + \infty ]$ is a Lebesgue measurable function on Ω (where of course we restrict the Lebesgue measure space on $\mathbf { R } ^ { d }$ to Ω in the usual fashion) with $\textstyle \int _ { \Omega } f ( x ) \ d x = 1$ , then $\left( \Omega , { \mathcal { L } } [ \mathbf { R } ^ { d } ] \ \backslash \Omega , \mathbf { P } \right)$ is a probability space, where $\mathbf { P } : = m _ { f }$ is the measure 

$$
\mathbf {P} (E) := \int_ {\Omega} 1 _ {E} (x) f (x) d x = \int_ {E} f (x) d x.
$$

The function $f$ is known as the (continuous) probability density of the state variable $\omega .$ . (This density is not quite unique, since one can modify it on a set of probability zero, but it is well-defined up to this ambiguity. See §1.2 of An epsilon of room, Vol. I for further discussion.) 

Exercise 2.3.1 (No translation-invariant random integer). Show that there is no probability measure $\mathbf { P }$ on the integers Z with the discrete σ-algebra $2 ^ { \mathbf { Z } }$ with the translation-invariance property $\mathbf { P } ( E + n ) \mathbf { \Psi } =$ $\mathbf { P } ( E )$ for every event $E \in 2 ^ { \mathbf { Z } }$ and every integer n. 

Exercise 2.3.2 (No translation-invariant random real). Show that there is no probability measure P on the reals R with the Lebesgue σ-algebra $\mathcal { L } [ \mathbf { R } ]$ with the translation-invariance property $\mathbf { P } ( E + x ) =$ $\mathbf { P } ( E )$ for every event $E \in { \mathcal { L } } [ \mathbf { R } ]$ and every real x. 

Many concepts in measure theory are of importance in probability theory, although the terminology is changed to reflect the diferent perspective on the subject. For instance, the notion of a property holding almost everywhere is now replaced with that of a property holding almost surely. A measurable function is now referred to as a random variable and is often denoted by symbols such as $X$ , and the integral of that function on the probability space (if the random variable is unsigned or absolutely convergent) is known as the expectation of that random variable, and is denoted E(X). Thus, for instance, the Borel-Cantelli lemma (Exercise 1.4.44) now reads as follows: given any sequence $E _ { 1 } , E _ { 2 } , E _ { 3 } , . . .$ . of events such that $\textstyle \sum _ { n = 1 } ^ { \infty } \mathbf { P } ( E _ { n } ) < \infty$ , it is almost surely true that at most finitely many of these events hold. In a similar spirit, Markov’s inequality (Exercise 1.4.36(vi)) becomes the assertion that $\mathbf { P } ( X \geq \lambda ) \leq { \frac { 1 } { \lambda } } \mathbf { E } X$ for any non-negative random variable X and any $0 < \lambda < \infty$ 

## 2.4. Infinite product spaces and the Kolmogorov extension theorem

In Section 1.7.4 we considered the product of two sets, measurable spaces, or (σ-finite) measure spaces. We now consider how to generalise this concept to products of more than two such spaces. The axioms of set theory allow us to form a Cartesian product $X _ { A } : =$ $\Pi _ { \alpha \in A } X _ { \alpha }$ of any family $( X _ { \alpha } ) _ { \alpha \in A }$ of sets indexed by another set A, which consists of the space of all tuples $x _ { A } = ( x _ { \alpha } ) _ { \alpha \in A }$ indexed by A, for which $x _ { \alpha } \in X _ { \alpha }$ for all $\alpha \in A$ . This concept allows for a succinct formulation of the axiom of choice (Axiom 0.0.4), namely that an arbitrary Cartesian product of non-empty sets remains non-empty. 

For any $\beta \in A .$ , we have the coordinate projection maps $\pi _ { \beta } :$ $X _ { A } \to X _ { \beta }$ defined by $\pi _ { \beta } ( ( x _ { \alpha } ) _ { \alpha \in A } ) : = x _ { \beta }$ . More generally, given any $B \subset A$ , we define the partial projections $\pi _ { B } : X _ { A }  X _ { B }$ to the partial product space $\begin{array} { r } { X _ { B } : = \prod _ { \alpha \in B } X _ { \alpha } } \end{array}$ by $\pi _ { B } ( ( x _ { \alpha } ) _ { \alpha \in A } ) : = ( x _ { \alpha } ) _ { \alpha \in B }$ . More generally still, given two subsets $C \subset B \subset A$ , we have the partial subprojections $\pi _ { C \left. B \right.} : X _ { B }  X _ { C }$ defined by $\pi _ { C  B } ( ( x _ { \alpha } ) _ { \alpha \in B } ) : =$ $( x _ { \alpha } ) _ { \alpha \in C }$ . These partial subprojections obey the composition law $\pi _ { D  C } \circ \pi _ { C  B } : = \pi _ { D  B }$ for all $D \subset C \subset B \subset A$ (and thus form a very simple example of a category). 

As before, given any σ-algebra $B _ { \beta }$ on $X _ { \beta }$ , we can pull it back by $\pi _ { \beta }$ to create a σ-algebra 

$$
\pi_ {\beta} ^ {*} (\mathcal {B} _ {\beta}) := \{\pi_ {\beta} ^ {- 1} (E _ {\beta}): E _ {\beta} \in \mathcal {B} _ {\beta} \}
$$

on $X _ { A }$ . One easily verifies that this is indeed a σ-algebra. Informally, $\pi _ { \beta } ^ { * } ( B _ { \beta } )$ describes those sets (or “events”, if one is thinking in probabilistic terms) that depend only on the $x _ { \beta }$ coordinate of the state $x _ { A } = ( x _ { \alpha } ) _ { \alpha \in A }$ , and whose dependence on $x _ { \beta }$ is $B _ { \beta }$ -measurable. We can then define the product σ-algebra 

$$
\prod_ {\beta \in A} \mathcal {B} _ {\beta} := \langle \bigcup_ {\beta \in A} \pi_ {\beta} ^ {*} (\mathcal {B} _ {\beta}) \rangle .
$$

We have a generalisation of Exercise 1.7.18: 

Exercise 2.4.1. Let $( ( X _ { \alpha } , B _ { \alpha } ) ) _ { \alpha \in A }$ be a family of measurable spaces. For any $B \subset A$ , write $\begin{array} { r } { B _ { B } : = \prod _ { \beta \in B } B _ { \beta } } \end{array}$ 

(1) Show that $B _ { A }$ is the coarsest σ-algebra on $X _ { A }$ that makes the projection maps $\pi _ { \beta }$ measurable morphisms for all $\beta \in A$ 

(2) Show that for each $B \subset A$ , that $\pi _ { B }$ is a measurable morphism from $( X _ { A } , B _ { A } )$ to $\left( { { X } _ { B } } , { { B } _ { B } } \right)$ 

(3) If E in $B _ { A }$ , show that there exists an at most countable set $B \subset A$ and a set $E _ { B } \in \mathcal { B } _ { B }$ such that $E _ { A } = \pi _ { B } ^ { - 1 } ( E _ { B } )$ Informally, this asserts that a measurable event can only depend on at most countably many of the coeficients. 

(4) If $f : X _ { A } \to [ 0 , + \infty ]$ is $B _ { A }$ -measurable, show that there exists an at most countable set $B \subset A$ and a $\boldsymbol { B } _ { B }$ -measurable function $f _ { B } : X _ { B }  [ 0 , + \infty ]$ such that $f = f _ { B } \circ \pi _ { B }$ 

(5) If A is at most countable, show that $B _ { A }$ is the σ-algebra generated by the sets $\prod _ { \beta \in A } E _ { \beta }$ with $E _ { \beta } \in B _ { \beta }$ for all $\beta \in A$ 

(6) On the other hand, show that if A is uncountable and the $B _ { \alpha }$ are all non-trivial, show that $B _ { A }$ is not the σ-algebra generated by sets $\prod _ { \beta \in A } E _ { \beta }$ with $E _ { \beta } \in B _ { \beta }$ for all $\beta \in A$ 

(7) If $B \subset A , E \in B _ { A }$ , and $x _ { A \backslash B } \in X _ { A \backslash B }$ , show that the set $E _ { x _ { A \setminus B } , B } : = \{ x _ { B } \in X _ { B } : ( x _ { B } , x _ { A \setminus B } ) \in E \}$ lies in $\boldsymbol { B } _ { B }$ , where we identify $X _ { B } \times X _ { A \setminus B }$ with $X _ { A }$ in the obvious manner. 

(8) If $B \subset A , f : X _ { A } \to [ 0 , + \infty ]$ is $B _ { A } { \mathrm { - m e a s u r a b l e } }$ , and $x _ { A \backslash B } \in$ $X _ { A \backslash B }$ , show that the function $f _ { x _ { A \setminus B } , B } : x _ { B }  f ( x _ { B } , x _ { A \setminus B } )$ is $\boldsymbol { B } _ { B }$ -measurable. 

Now we consider the problem of constructing a measure $\mu _ { A }$ on the product space $X _ { A }$ . Any such measure $\mu _ { A }$ will induce pushforward measures $\mu _ { B } : = ( \pi _ { B } ) _ { * } \mu _ { A }$ on $X _ { B }$ (introduced in Exercise 1.4.38), thus 

$$
\mu_ {B} (E _ {B}) := \mu_ {A} (\pi_ {B} ^ {- 1} (E _ {B}))
$$

for all $E _ { B } \in \boldsymbol { B } _ { B }$ . These measures obey the compatibility relation 

$$
\left(\pi_ {C \leftarrow B}\right) _ {*} \mu_ {B} = \mu_ {C}\tag{2.6}
$$

whenever $C \subset B \subset A$ , as can be easily seen by chasing the definitions. 

One can then ask whether one can reconstruct $\mu _ { A }$ from just from the projections $\mu _ { B }$ to finite subsets B. This is possible in the important special case when the $\mu _ { B }$ (and hence $\mu _ { A } )$ are probability measures, provided one imposes an additional inner regularity hypothesis on the measures $\mu _ { B }$ . More precisely: 

Definition 2.4.1 (Inner regularity). A (metrisable) inner regular measure space $( X , B , \mu , d )$ is a measure space $( X , B , \mu )$ equipped with a metric d such that 

(1) Every compact set is measurable; and 

(2) One has $\mu ( E ) = \operatorname* { s u p } _ { K \subset E , K }$ compact $\mu ( K )$ for all measurable E. 

We say that $\mu$ is inner regular if it is associated to an inner regular measure space. 

Thus for instance Lebesgue measure is inner regular, as are Dirac measures and counting measures. Indeed, most measures that one actually encounters in applications will be inner regular. For instance, any finite Borel measure on $\mathbf { R } ^ { d }$ (or more generally, on a locally compact, σ-compact space) is inner regular, as is any Radon measure; see §1.10 of An epsilon of room, Vol. I. 

Remark 2.4.2. One can generalise the concept of an inner regular measure space to one which is given by a topology rather than a metric; Kolmogorov’s extension theorem still holds in this more general setting, but requires Tychonof’s theorem, which is discussed in §1.8 of An epsilon of room, Vol. I. However, some minimal regularity hypotheses of a topological nature are needed to make the Kolmogorov extension theorem work, although this is usually not a severe restriction in practice. 

Theorem 2.4.3 (Kolmogorov extension theorem). Let $( ( X _ { \alpha } , B _ { \alpha } ) , \mathcal { F } _ { \alpha } ) _ { \alpha \in A }$ be a family of measurable spaces $\left( X _ { \alpha } , B _ { \alpha } \right)$ , equipped with a topology 

${ \mathcal { F } } _ { \alpha }$ . For each finite $B \subset A$ , let $\mu _ { B }$ be an inner regular probability measure on $\begin{array} { r } { B _ { B } : = \prod _ { \alpha \in B } B _ { \alpha } } \end{array}$ with the product topology $\begin{array} { r } { \mathcal { F } _ { B } : = \prod _ { \alpha \in B } \mathcal { F } _ { \alpha } } \end{array}$ , obeying the compatibility condition (2.6) whenever $C \subset B \subset A$ are two nested finite subsets of A. Then there exists a unique probability measure $\mu _ { A }$ on $B _ { A }$ with the property that $( \pi _ { B } ) _ { * } \mu _ { A } = \mu _ { B }$ for all finite $B \subset A$ 

Proof. Our main tool here will be the Hahn-Kolmogorov extension theorem for pre-measures (Theorem 1.7.8), combined with the Heine-Borel theorem. 

Let $B _ { 0 }$ be the set of all subsets of $X _ { A }$ that are of the form $\pi _ { B } ^ { - 1 } ( E _ { B } )$ for some finite $B \subset A$ and some $E _ { B } \in \mathcal { B } _ { B }$ . One easily verifies that this is a Boolean algebra that is contained in $B _ { A }$ . We define a function $\mu _ { 0 } : B _ { 0 } \to [ 0 , + \infty ]$ by setting 

$$
\mu_ {0} (E) := \mu_ {B} (E _ {B})
$$

whenever E takes the form $\pi _ { B } ^ { - 1 } ( E _ { B } )$ for some finite $B \subset A$ and $E _ { B } \in$ $\boldsymbol { B } _ { B }$ . Note that a set $E \in B _ { 0 }$ may have two diferent representations $E = \pi _ { B } ^ { - 1 } ( E _ { B } ) = \pi _ { B ^ { \prime } } ^ { - 1 } ( E _ { B ^ { \prime } } )$ for some finite $B , B ^ { \prime } \subset A .$ , but then one must have $E _ { B } = \pi _ { B  B \cup B ^ { \prime } } ( E _ { B \cup B ^ { \prime } } )$ and $E _ { B ^ { \prime } } = \pi _ { B ^ { \prime }  B \cup B ^ { \prime } } ( E _ { B \cup B ^ { \prime } } )$ where $E _ { B \cup B ^ { \prime } } : = \pi _ { B \cup B ^ { \prime } } ( E )$ . Applying (2.6), we see that 

$$
\mu_ {B} (E _ {B}) = \mu_ {B \cup B ^ {\prime}} (E _ {B \cup B ^ {\prime}})
$$

and 

$$
\mu_ {B ^ {\prime}} (E _ {B ^ {\prime}}) = \mu_ {B \cup B ^ {\prime}} (E _ {B \cup B ^ {\prime}})
$$

and thus $\mu _ { B } ( E _ { B } ) = \mu _ { B ^ { \prime } } ( E _ { B ^ { \prime } } )$ . This shows that $\mu _ { 0 } ( E )$ is well defined. As the $\mu _ { B }$ are probability measures, we see that $\mu _ { 0 } ( X _ { A } ) = 1$ 

It is not dificult to see that $\mu _ { 0 }$ is finitely additive. We now claim that $\mu _ { 0 }$ is a pre-measure. In other words, we claim that if $E \in B _ { 0 }$ is the disjoint countable union $\textstyle E = \bigcup _ { n = 1 } ^ { \infty } E _ { n }$ of sets $E _ { n } \in B _ { 0 }$ , then $\begin{array} { r } { \mu _ { 0 } ( E ) = \sum _ { n = 1 } ^ { \infty } \mu _ { 0 } ( E _ { n } ) } \end{array}$ 

For each $N \geq 1$ , let $F _ { N } : = E \backslash \bigcup _ { n = 1 } ^ { N } E _ { N }$ . Then the $F _ { N }$ lie in $B _ { 0 }$ , are decreasing, and are such that $\bigcap _ { N = 1 } ^ { \infty } F _ { N } = \varnothing$ . By finite additivity (and the finiteness of $\mu _ { 0 } )$ , we see that it sufices to show that lim $_ { N \to \infty } \mu _ { 0 } ( F _ { N } ) = 0$ 

Suppose this is not the case, then there exists $\varepsilon > 0$ such that $\mu _ { 0 } ( F _ { N } ) > \varepsilon$ for all N. As each $F _ { N }$ lies in $B _ { 0 }$ , we have $F _ { N } = \pi _ { B _ { N } } ^ { - 1 } ( G _ { N } )$ for some finite sets $B _ { N } \subset A$ and some $\boldsymbol { B } _ { B _ { N } }$ -measurable sets $G _ { N }$ . By enlarging each $B _ { N }$ as necessary we may assume that the $B _ { N }$ are increasing in N. The decreasing nature of the $F _ { N }$ then gives the inclusions 

$$
G _ {N + 1} \subset \pi_ {B _ {N} \leftarrow B _ {N + 1}} ^ {- 1} (G _ {N}).
$$

By inner regularity, one can find a compact subset $K _ { N }$ of each $G _ { N }$ such that 

$$
\mu_ {B _ {N}} (K _ {N}) \geq \mu_ {B _ {N}} (G _ {N}) - \varepsilon / 2 ^ {N + 1}.
$$

If we then set 

$$
K _ {N} ^ {\prime} := \bigcup_ {N ^ {\prime} = 1} ^ {N} \pi_ {B _ {N ^ {\prime}} \leftarrow B _ {N}} ^ {- 1} (K _ {N})
$$

then we see that each $K _ { N } ^ { \prime }$ is compact and 

$$
\mu_ {B _ {N}} (K _ {N} ^ {\prime}) \geq \mu_ {B _ {N}} (G _ {N}) - \varepsilon / 2 ^ {N} \geq \varepsilon - \varepsilon / 2 ^ {N}.
$$

In particular, the sets $K _ { N } ^ { \prime }$ are non-empty. By construction, we also have the inclusions 

$$
K _ {N + 1} ^ {\prime} \subset \pi_ {B _ {N} \leftarrow B _ {N + 1}} ^ {- 1} (K _ {N} ^ {\prime})
$$

and thus the sets $H _ { N } : = \pi _ { B _ { N } } ^ { - 1 } ( K _ { N } ^ { \prime } )$ are decreasing in N. On the other hand, since these sets are contained in $F _ { N }$ , we have $\bigcap _ { N = 1 } ^ { \infty } H _ { N } = \varnothing$ 

By the axiom of choice, we can select an element $x _ { N } \in H _ { N }$ from $H _ { N }$ for each $N$ . Observe that for any $N _ { 0 }$ , that $\pi _ { B _ { N _ { 0 } } } ( x _ { N } )$ will lie in the compact set $K _ { N _ { 0 } } ^ { \prime }$ whenever $N \ge N _ { 0 }$ . Applying the Heine-Borel theorem repeatedly, we may thus find a subsequence $x _ { N _ { 1 , m } }$ of the $x _ { N }$ for $m = 1 , 2 , . . .$ . such that $\pi _ { B _ { 1 } } ( x _ { N _ { 1 , m } } )$ converges; then we can find a further subsequence $x _ { N _ { 2 , m } }$ of that subsequence such that $\pi _ { B _ { 2 } } ( x _ { N _ { 2 , m } } )$ , and more generally obtain nested subsequences $x _ { N _ { j , m } }$ for $m = 1 , 2 , . . .$ . and $j = 1 , 2 , . . .$ . such that for each $j = 1 , 2 , . . . ,$ the sequence $m \mapsto \pi _ { B _ { j } } ( x _ { N _ { j , m } } )$ converges. 

Now we use the diagonalisation trick. Consier the sequence $x _ { N _ { m , m } } = :$ $( y _ { m , \alpha } ) _ { \alpha \in A }$ for $m = 1 , 2 , \ldots$ . By construction, we see that for each $j ,$ $\pi _ { B _ { j } } ( x _ { N _ { m , m } } )$ converges to a limit as $m  \infty$ . This implies that for each $\textstyle \alpha \in \bigcup _ { j = 1 } ^ { \infty } B _ { j } , y _ { m , \alpha }$ converges to a limit $y _ { \alpha }$ as $m  \infty$ . As $K _ { j } ^ { \prime }$ is closed, we see that $( y _ { \alpha } ) _ { \alpha \in B _ { j } } \in K _ { j } ^ { \prime }$ for each $j$ . If we then extend $y _ { \alpha }$ 

arbitrarily from $\alpha \in \textstyle \bigcup _ { j = 1 } ^ { \infty } B _ { j }$ to $\alpha \in A$ , then the point $y : = ( y _ { \alpha } ) _ { \alpha \in A }$ lies in $H _ { j }$ for each $j$ . But this contradicts the fact that $\bigcap _ { N = 1 } ^ { \infty } H _ { N } = \varnothing$ This contradiction completes the proof that $\mu _ { 0 }$ is a pre-measure. 

If we then let $\mu$ be the Hahn-Kolmogorov extension of $\mu _ { 0 }$ , one easily verifies that $\mu$ obeys all the required properties, and the uniqueness follows from Exercise 1.7.7.  

The Kolmogorov extension theorem is a fundamental tool in the foundations of probability theory, as it allows one to construct a probability space to hold a variety of random processes $( X _ { t } ) _ { t \in T }$ , both in the discrete case (when the set of times $T$ is something like the integers $\mathbf { Z } )$ and in the continuous case (when the set of times $T$ is something like R). In particular, it can be used to rigorously construct a process for Brownian motion, known as the Wiener process. We will however not focus on this topic, which can be found in many graduate probability texts. But we will give one common special case of the Kolmogorov extension theorem, which is to construct product probability measures: 

Theorem 2.4.4 (Existence of product measures). Let A be an $a r \mathrm { - }$ bitrary set. For each $\alpha \in A$ , let $\left( X _ { \alpha } , B _ { \alpha } , \mu _ { \alpha } \right)$ be a probability space in which $X _ { \alpha }$ is a locally compact, σ-compact metric space, with $B _ { \alpha }$ being its Borel σ-algebra (i.e. the σ-algebra generated by the open sets). Then there exists a unique probability measure $\textstyle \mu _ { A } = \prod _ { \alpha \in A } \mu _ { \alpha }$ on $\begin{array} { r } { ( X _ { A } , { \mathcal { B } } _ { A } ) : = ( \prod _ { \alpha \in A } X _ { \alpha } , \prod _ { \alpha \in A } { \mathcal { B } } _ { \alpha } ) } \end{array}$ with the property that 

$$
\mu_ {A} (\prod_ {\alpha \in A} E _ {\alpha}) = \prod_ {\alpha \in A} \mu_ {\alpha} (E _ {\alpha})
$$

whenever $E _ { \alpha } \in B _ { \alpha }$ for each $\alpha \in A$ , and one has $E _ { \alpha } = X _ { \alpha }$ for all but finitely many of the α. 

Proof. We apply the Kolmogorov extension theorem to the finite product measures $\textstyle \mu _ { B } : = \prod _ { \alpha \in B } \mu _ { \alpha }$ for finite $B \subset A$ , which can be constructed using the machinery in Section 1.7.4. These are Borel probability measures on a locally compact, σ-compact space and are thus inner regular (see §1.10 of An epsilon of room, Vol. I). The compatibility condition (2.6) can be verified from the uniqueness properties of finite product measures.  

Remark 2.4.5. This result can also be obtained from the Riesz representation theorem, which is covered in §1.10 of An epsilon of room, Vol. I. 

Example 2.4.6 (Bernoulli cube). Let A := N, and for each $\alpha \in A$ let $\left( X _ { \alpha } , B _ { \alpha } , \mu _ { \alpha } \right)$ be the two-element set ${ \cal { X } } _ { \alpha } = \{ 0 , 1 \}$ with the discrete metric (and thus discrete σ-algebra) and the uniform probability measure $\mu _ { \alpha }$ . Then Theorem 2.4.4 gives a probability measure µ on the infinite discrete cube $X _ { A } : = \{ 0 , 1 \} ^ { \mathbf { N } }$ , known as the (uniform) Bernoulli measure on this cube. The coordinate functions $\pi _ { \alpha } : X _ { A } \to \{ 0 , 1 \}$ can then be interpreted as a countable sequence of random variables taking values in {0, 1}. From the properties of product measure one can easily check that these random variables are uniformly distributed on {0, 1} and are jointly independent<sup>2</sup>. Informally, Bernoulli measure allows one to model an infinite number of “coin flips”. One can replace the natural numbers here by any other index set, and have a similar construction. 

Example 2.4.7 (Continuous cube). We repeat the previous example, but replace {0, 1} with the unit interval [0, 1] (with the usual metric, the Borel σ-algebra, and the uniform probability measure). This gives a probability measure on the infinite continuous cube $[ 0 , 1 ] ^ { \mathbf { N } }$ , and the coordinate functions $\pi _ { \alpha } : X _ { A } \to [ 0 , 1 ]$ can now be interpreted as jointly independent random variables, each having the uniform distribution on [0, 1]. 

Example 2.4.8 (Independent gaussians). We repeat the previous example, but now replace [0, 1] with R (with the usual metric, and the Borel σ-algebra), and the normal probability distribution $d \mu _ { \alpha } =$ $\scriptstyle { \frac { 1 } { \sqrt { 2 \pi } } } e ^ { - x ^ { 2 } / 2 }$ dx (thus $\begin{array} { r } { \mu _ { \alpha } ( E ) = \int _ { E } \frac { 1 } { \sqrt { 2 \pi } } e ^ { - x ^ { 2 } / 2 } } \end{array}$ dx for every Borel set E). This gives a probability space that supports a countable sequence of jointly independent gaussian random variables $\pi _ { \alpha }$ 

## Bibliography



[De1901] M. Dehn, Uber den Rauminhalt<sup>¨</sup> , Mathematische Annalen 55 (1901), no. 3, pages 465-478. 





[deG1981] M. de Guzm´an, Real variable methods in Fourier analysis. North-Holland Mathematics Studies, 46. Notas de Matem´atica , 75. North-Holland Publishing Co., Amsterdam-New York, 1981. 





[Go1938] K. G¨odel, Consistency of the axiom of choice and of the generalized continuum-hypothesis with the axioms of set theory, Proc. Nat. Acad. Sci. 24 (1938), 556–557. 





[Me2003] A. Melas, The best constant for the centered Hardy-Littlewood maximal inequality, Ann. of Math. 157 (2003), no. 2, 647-688. 





[So1970] R. Solovaly, A model of set-theory in which every set of reals is Lebesgue measurable, Annals of Mathematics 92 (1970), 1-56. 





[StSk2005] E. Stein, R. Shakarchi, Real analysis. Measure theory, integration, and Hilbert spaces. Princeton Lectures in Analysis, III. Princeton University Press, Princeton, NJ, 2005. 





[StSt1983] E. Stein, J.-O. Str¨omberg, Behavior of maximal functions in $R ^ { n }$ for large n, Ark. Mat. 21 (1983), no. 2, 259-269. 





[Ta2008] T. Tao, Structure and Randomness: pages from year one of a mathematical blog, American Mathematical Society, Providence RI, 2008. 





[Ta2009] T. Tao, Poincar´e’s Legacies: pages from year two of a mathematical blog, Vol. I, American Mathematical Society, Providence RI, 2009. 





[Ta2010] T. Tao, An epsilon of room, Vol. I, American Mathematical Society, Providence RI, 2010. 





[Vi1908] G. Vitali, Sui gruppi di punti e sulle funzioni di variabili reali, Atti dell’Accademia delle Scienze di Torino 43 (1908), 75-92. 



## Index

F<sub>σ</sub> set, 40, 87 G set, 40, 87 L<sup>p</sup> norm, 119, 127 σ-algebra, 85 σ-compact, 85 σ-finite, 85, 197 

a priori estimate, 212 absolute continuity, 172 absolute integrability, 54, 68, 104 absolutely convergent integral, 104 almost disjoint, 28 almost dominated convergence, 112 almost everywhere, 53 almost everywhere diferentiability, 132 almost sure convergence, 116 almost uniform convergence, 116 approximation by an algebra, 95 approximation to the identity, 155, 208 area interpretation of integral, 207 area interpretation of Lebesgue integral, 66 area interpretation of Riemann integral, 17 atomic algebra, 82 axiom of choice, xv axiom of countable choice, xvi 

ball, 11 Banach-Tarski paradox, 3 basic jump function, 160 Bernoulli random variables, 241 Besicovitch covering lemma, 152 Bolyai-Gerwien theorem, 13 Boolean algebra, 10, 80 Borel σ-algebra, 87 Borel hierarchy, 88 Borel measure, 153 Borel-Cantelli lemma, 109 bounded variation, 165 bounded variation diferentiation theorem, 167 box, 5 bullet-riddled square, 13 

Cantor function, 170 Cantor set, 35, 61 Cantor’s theorem, 25 Carath´eodory measurability, 40, 181 category of measure spaces, 96 change of variables (linear), 41, 66 change of variables (measure), 103 change of variables (series), xii classical derivative. 132 closed dyadic cube, 29 coarsening, 80 compactness, 25 

complete measure, 94 completion (measure), 94 continuity of translation, 138 continuous diferentiability, 132 continuous probability distribution, 234 continuously diferentiable curve, 43 convergence in L<sup>1</sup> norm, 116 convergence in L<sup>∞</sup> norm, 116 convergence in distribution, 131 convergence in mean, 116 convergence in measure, 116 convergence in probability, 116 convolution, 140 countable additivity, 36, 92 countable subadditivity, 22, 93 Cousin’s theorem, 153 create an epsilon of room, 23, 25, 210 cumulative distribution function 131 Darboux integrability, 16 Darboux integral, 16 de Morgan’s laws, 33 defect version of Fatou’s lemma, 113, 130 density argument, 138 Devil’s staircase, 170 diameter, 24 diferentiability, 132 Dini derivative, 156 Dirac measure, 90 directional diferentiability, 226 discrete algebra, 81 discrete probability distribution, 234 discretisation, 7 distance (L<sup>1</sup>), 69 dominated convergence theorem, 111 dominated convergence theorem (sets), 38, 93 domination, 126 dot product, xi downward monotone convergence (sets), 38 

downwards monotone convergence, 93 Dyadic algebra, 83 dyadic cube, 12 dyadic maximal inequality, 152 dyadic mesh, 29 dyadic nesting property, 30 Egorov’s theorem, 75, 97, 123 elementary algebra, 81 elementary measure, 6 elementary set, 5 escape to horizontal infinity, 76, 106, 118 escape to vertical infinity, 106, 118, 126 escape to width infinity, 106, 118, 126 essential upper bound, 119 essentially uniform convergence, 116 Euclidean space, xi event space, 233 existence of non-measurable sets, 44 extended real, xi exterior measure, 180 fast convergence, 124 Fatou’s lemma, 110 finite additivity, 8, 10, 23, 65, 90, 91, 99, 101 finite subadditivity, 10, 22, 91 first fundamental theorem of calculus, 135 first uncountable ordinal, 88 Fubini’s theorem, 205 Fubini-Tonelli theorem, 207 gauge function, 153 generation of algebras, 84, 86 good kernel, 155 gradient, 227 graphs, 10 greedy algorithm, 149 Hahn-Kolmogorov extension, 18 Hahn-Kolmogorov theorem, 186 

## Index

Hardy-Littlewood maximal inequality, 142, 146, 148, 157 heat kernel, 155 Heaviside function, 193 height (step function), 121 Heine-Borel theorem, 25 Henstock-Kurzweil integral, 178 Hilbert’s third problem, 13 homogeneity, 100 homogeneity (integral), 64, 99 homomorphism, 141 horizontal truncation, 64, 101 

inclusion-exclusion principle, 91, 99 indeterminate forms, xii indicator function, xi infinite series (absolutely summable), 47 infinite series (unsigned), xiii, 47 inner regularity, 39, 237 integration by parts, 169, 194, 230 interval, 5, 189 

Jordan algebra, 81 Jordan inner measure, 9 Jordan measurability, 9 Jordan null set, 12 Jordan outer measure, 9, 18 jump function, 160 

Kolmogorov extension theorem, 238 

Lebesgue algebra, 82 

Lebesgue decomposition, 162 

Lebesgue diferentiation theorem, 136, 137, 147 

Lebesgue exterior measure, 20 

Lebesgue inner measure, 40 

Lebesgue integral (absolutely integrable), 68 

Lebesgue integral (unsigned), 65 

Lebesgue measurability, 20 

Lebesgue measurability (complex functions), 62 

Lebesgue measurability (unsigned functions), 57 

Lebesgue outer measure, 19 

Lebesgue philosophy, 57 

Lebesgue point, 147 

Lebesgue-Stieltjes measure, 189 

length, xi 

length (intervals), 5 

linearity (integral), 15, 16, 54, 55, 70, 98 

Lipschitz continuity, 226 

Lipschitz diferentiation theorem, 167 

Littlewood’s first principle, 20, 34, 40, 72 

Littlewood’s second principle, 72, 77 

Littlewood’s third principle, 72, 75 

Littlewood-like principles, 78 

local integrability, 147 

locally uniform convergence, 74 

lower Darboux integral, 15 

lower unsigned Lebesgue integral, 63 

Lusin’s theorem, 77 

Markov’s inequality, 67, 100 

mean value theorem, 134 

measurability (function), 95 

measurability (set), 80 

measurable map, 96 

measurable morphism, 96 

measure, 36, 92 

measure space, 92 

metric completion, 42 

metric entropy, 12 

monotone class lemma, 200 

monotone convergence theorem, 107, 130 

monotone convergence theorem (sets), 38, 93 

monotone diferentiation theorem, 156 

monotonicity (integral), 15, 16, 54, 64, 97, 99, 100 

monotonicity (measure), 8, 10, 21, 91 

moving bump example, 76 

moving bump function, 106 

noise tolerance, 56 non-atomic algebra, 83 non-negativity (measure), 10 norm (partition), 14 Notation, x null algebra, 82 null set, 32, 94 outer measure, 20, 22, 180, 186 outer regularity, 30 partial derivative, 226 piecewise constant function, 15 piecewise constant integral, 15 pointwise almost everywhere convergence, 74, 116 pointwise convergence, 73, 115 pointwise convergence (sets), 38 Poisson kernel, 155 polytope, 11 pre-measure, 185 probability, 233 probability density, 234 probability measure, 232 probability space, 232 problem of measure, 2 product σ-algebra, 195, 236 product measure, 197, 240 product space, 235 pullback (σ-algebra), 195 pushforward, 103, 237 Radamacher diferentiation theorem, 228 Radon measure, 192 recursive description of a σ-algebra, 88 recursive description of Boolean algebra, 84 refinement, 80 reflection, 16, 213 restriction (Boolean algebra), 82 restriction (measure), 101 Riemann integrability, 14 Riemann integral, 14 Riemann sum, 14 Riemann-Stieltjes integral, 194 rising sun inequality, 146 rising sun lemma, 143 Rolle’s theorem, 132 

sample space, 233 second fundamental theorem of calculus, 134, 168, 169, 173, 176 seminorm, 69 simple function, 50 simple integral, 51, 97, 98 Solovay’s theorem, 43 space-filling curve, 43 Steinhaus theorem, 140, 154 step function, 72 strong derivative, 132 sub-null set, 94 subadditivity (integral), 64 sums of measures, 92 superadditivity, 100 superadditivity (integral), 64 support, 53 symmetric diference, 5 

tagged partition, 14 tail support, 121 Tonelli’s theorem, 201, 203, 204 Tonelli’s theorem (series), xiii, xv Tonelli’s theorem (sums and integrals), 109 total diferentiability, 227 total variation, 165 translation (of a set in Euclidean space), 5 translation invariance, 8, 10, 41, 66 triangle inequality, 71 trivial algebra, 81 typewriter sequence, 118 

uniform continuity, 172 uniform convergence, 74, 115 uniform integrability, 126 uniformly almost everywhere convergence, 116 uniqueness of antiderivative, 134 uniqueness of Jordan measure, 12 uniqueness of Lebesgue measure, 42 uniqueness of the Lebesgue integral, 66 uniqueness of the Riemann integral, 17 

uniqueness of the unsigned integral, 113 unsigned integral, 100 upper Darboux integral, 16 upper unsigned Lebesgue integral, 63 upward monotone convergence (sets), 37 upwards monotone convergence, 93 vertical truncation, 64, 101 Vitali-type covering lemma, 149 volume (box), 5 weak derivative, 229 Weierstrass function, 156 width (step function), 121 

zero measure, 90 